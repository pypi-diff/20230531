# Comparing `tmp/dxsp-2.6.3.tar.gz` & `tmp/dxsp-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.6.3.tar", max compression
+gzip compressed data, was "dxsp-2.6.4.tar", max compression
```

## Comparing `dxsp-2.6.3.tar` & `dxsp-2.6.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-30 20:06:34.665493 dxsp-2.6.3/LICENSE
--rw-r--r--   0        0        0     2348 2023-05-30 20:06:34.665493 dxsp-2.6.3/README.md
--rw-r--r--   0        0        0       86 2023-05-30 20:06:35.325500 dxsp-2.6.3/dxsp/__init__.py
--rw-r--r--   0        0        0      386 2023-05-30 20:06:34.665493 dxsp-2.6.3/dxsp/config.py
--rw-r--r--   0        0        0     3679 2023-05-30 20:06:34.665493 dxsp-2.6.3/dxsp/default_settings.toml
--rw-r--r--   0        0        0    18642 2023-05-30 20:06:34.665493 dxsp-2.6.3/dxsp/main.py
--rw-r--r--   0        0        0     1542 2023-05-30 20:06:35.325500 dxsp-2.6.3/pyproject.toml
--rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 dxsp-2.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-31 08:33:30.294261 dxsp-2.6.4/LICENSE
+-rw-r--r--   0        0        0     2348 2023-05-31 08:33:30.294261 dxsp-2.6.4/README.md
+-rw-r--r--   0        0        0       86 2023-05-31 08:33:30.978268 dxsp-2.6.4/dxsp/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-31 08:33:30.294261 dxsp-2.6.4/dxsp/config.py
+-rw-r--r--   0        0        0     3679 2023-05-31 08:33:30.294261 dxsp-2.6.4/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    18799 2023-05-31 08:33:30.294261 dxsp-2.6.4/dxsp/main.py
+-rw-r--r--   0        0        0     1542 2023-05-31 08:33:30.978268 dxsp-2.6.4/pyproject.toml
+-rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 dxsp-2.6.4/PKG-INFO
```

### Comparing `dxsp-2.6.3/LICENSE` & `dxsp-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.3/README.md` & `dxsp-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.3/dxsp/default_settings.toml` & `dxsp-2.6.4/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.3/dxsp/main.py` & `dxsp-2.6.4/dxsp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,16 @@
             sell_balance = await self.get_token_balance(sell_token)
             risk_percentage = settings.trading_risk_amount
             sell_amount = (sell_balance / (risk_percentage ** sell_decimals)) * (float(quantity) / 100)
 
             order = await self.get_swap(sell_token, buy_token, sell_amount)
             if order:
                 return order['confirmation']
-        except Exception as error:
-            raise error
+        except Exception:
+            raise ValueError("Order execution failed")
 
     async def get_quote(self, sell_token):
         """
         Asynchronously gets a quote for a specified sell token using the given `sell_token` parameter,
         """
         buy_address = await self.search_contract(settings.trading_asset)
         sell_address = await self.search_contract(sell_token)
@@ -91,56 +91,59 @@
             if not sell_token_address or sell_token_balance in (0, None):
                 return
 
             buy_token_address = await self.search_contract(buy_token)
             if not buy_token_address:
                 return
 
-            sell_token_amount_wei = self.w3.to_wei(amount * 10 ** (await self.get_token_decimals(sell_token)), "ether")
+            sell_token_amount_wei = self.w3.to_wei(
+                amount * 10 ** (await self.get_token_decimals(sell_token)), "ether")
 
             if await self.get_approve(sell_token) is None:
                 return
 
-            swap_order = await self.get_swap_order(sell_token_address, buy_token_address, sell_token_amount_wei)
+            swap_order = await self.get_swap_order(
+                sell_token_address, buy_token_address, sell_token_amount_wei)
             if not swap_order:
                 return
 
             if self.protocol_type == "0x":
                 await self.get_sign(swap_order)
 
             signed_order = await self.get_sign(swap_order)
             order_hash = str(self.w3.to_hex(signed_order))
 
-            if self.w3.wait_for_transaction_receipt(order_hash, timeout=120, poll_latency=0.1)["status"] != 1:
+            if self.w3.wait_for_transaction_receipt(
+                order_hash, timeout=120, poll_latency=0.1)["status"] != 1:
                 return
 
             await self.get_confirmation(order_hash)
 
         except Exception as error:
             raise error
 
 ### ------🛠️ W3 UTILS ---------
 
 
-    async def _get(self, url, params=None, headers=None):
+    async def get(self, url, params=None, headers=None):
         try:
             self.logger.debug(f"Requesting URL: {url}")
             response = requests.get(url, params=params, headers=headers, timeout=10)
             if response.status_code == 200:
                 return response.json()
 
         except Exception as error:
             raise error
 
 
     async def router(self):
         try:
             router_abi = await self.get_abi(settings.dex_router_contract_addr)
             if router_abi is None:
-                router_abi = await self._get(settings.dex_router_abi_url)
+                router_abi = await self.get(settings.dex_router_abi_url)
             router = self.w3.eth.contract(
                 address=self.w3.to_checksum_address(
                     settings.dex_router_contract_addr),
                 abi=router_abi)
             return router
         except Exception as error:
             raise error
@@ -151,29 +154,30 @@
         except Exception as error:
             raise error
 
     async def quoter(self):
         try:
             quoter_abi = await self.get_abi(settings.dex_quoter_contract_addr)
             if quoter_abi is None:
-                quoter_abi = await self._get(settings.dex_quoter_abi_url)
+                quoter_abi = await self.get(settings.dex_quoter_abi_url)
             contract = self.w3.eth.contract(
                 address=self.w3.to_checksum_address(
                     settings.dex_quoter_contract_addr),
                 abi=quoter_abi)
             return contract
         except Exception as error:
             raise error
 
     async def get_approve(self, symbol):
         try:
             if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
                 await self.get_approve_uniswap(symbol)
         except Exception as error:
-            raise error
+            self.logger.debug("error %s", error)
+            return None
 
     async def get_sign(self, transaction):
         try:
             if self.protocol_type in ['uniswap_v2', 'uniswap_v3']:
                 transaction_params = {
                     'from': self.wallet_address,
                     'gas': await self.get_gas(transaction),
@@ -198,15 +202,15 @@
             "module": "contract",
             "action": "getabi",
             "address": address,
             "apikey": settings.dex_block_explorer_api
         }
 
         try:
-            resp = await self._get(
+            resp = await self.get(
                 url=settings.dex_block_explorer_url, params=params)
             if resp['status'] == "1":
                 self.logger.debug("ABI found %s", resp)
                 return resp["result"]
             else:
                 self.logger.warning("No ABI identified")
                 return None
@@ -334,15 +338,15 @@
         except Exception as e:
             self.logger.error(" search_cg_contract: %s", e)
             return
 
     async def get_contract_address(self, token_list_url, symbol):
         """Given a token symbol and json tokenlist, get token address"""
         try:
-            token_list = await self._get(token_list_url)
+            token_list = await self.get(token_list_url)
             token_search = token_list['tokens']
             for keyval in token_search:
                 if (keyval['symbol'] == symbol and
                    keyval['chainId'] == self.chain_id):
                     return keyval['address']
         except Exception as e:
             self.logger.debug("get_contract_address %s", e)
@@ -350,15 +354,15 @@
 
     async def get_token_contract(self, token):
         """Given a token symbol, returns a contract object. """
         try:
             token_address = await self.search_contract(token)
             token_abi = await self.get_abi(token_address)
             if token_abi is None:
-                token_abi = await self._get(settings.dex_erc20_abi_url)
+                token_abi = await self.get(settings.dex_erc20_abi_url)
             return self.w3.eth.contract(
                 address=token_address,
                 abi=token_abi)
         except Exception as e:
             raise e
 
 # 🔒 USER RELATED
@@ -372,16 +376,16 @@
             return None
         return contract.functions.balanceOf(self.wallet_address).call() or 0
 
     async def get_token_decimals(self, token_symbol: str) -> Optional[int]:
         """Get token decimals"""
         contract = await self.get_token_contract(token_symbol)
         if not contract:
-            return None
-        return await contract.functions.decimals().call()
+            return 18
+        return contract.functions.decimals().call()
 
     async def get_account_balance(self):
         try:
             account_balance = self.w3.eth.get_balance(
                 self.w3.to_checksum_address(self.wallet_address))
             account_balance = self.w3.from_wei(account_balance, 'ether')
             trading_asset_balance = await self.get_trading_asset_balance()
@@ -440,22 +444,24 @@
     async def get_approve_uniswap(self, symbol):
         try:
             contract = await self.get_token_contract(symbol)
             approved_amount = self.w3.to_wei(2 ** 64 - 1, 'ether')
             owner_address = self.w3.to_checksum_address(self.wallet_address)
             dex_router_address = self.w3.to_checksum_address(settings.dex_router_contract_addr)
             allowance = contract.functions.allowance(owner_address, dex_router_address).call()
+            self.logger.debug("allowance %s", allowance)
             if allowance == 0:
                 approval_tx = contract.functions.approve(dex_router_address, approved_amount)
                 approval_tx_hash = await self.get_sign(approval_tx)
                 approval_receipt = self.w3.eth.wait_for_transaction_receipt(
                     approval_tx_hash, timeout=120, poll_latency=0.1)
                 return approval_receipt
-        except Exception as error:
-            raise error
+        except Exception as e:
+            raise e
+
 
     async def get_swap_uniswap(self, asset_out_address, asset_in_address, amount):
         try:
             path = [self.w3.to_checksum_address(asset_out_address),
                     self.w3.to_checksum_address(asset_in_address)]
             deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
             router_instance = await self.router()
@@ -475,13 +481,13 @@
 # 0️⃣x
     async def get_0x_quote(self, buy_address, sell_address, amount=1):
         try:
             out_amount = self.w3.to_wei(amount, 'ether')
             url = (settings.dex_0x_url + "/swap/v1/quote?buyToken=" + str(buy_address) +
                 "&sellToken=" + str(sell_address) + "&buyAmount=" + str(out_amount))
             headers = {"0x-api-key": settings.dex_0x_api_key}
-            response = await self._get(url, params=None, headers=headers)
+            response = await self.get(url, params=None, headers=headers)
             print(response)
             if response:
                 return round(float(response['guaranteedPrice']), 3)
         except Exception as e:
             raise e
```

### Comparing `dxsp-2.6.3/pyproject.toml` & `dxsp-2.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.6.3"
+version = "2.6.4"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-2.6.3/PKG-INFO` & `dxsp-2.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.6.3
+Version: 2.6.4
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

