# Comparing `tmp/dxsp-2.6.5.tar.gz` & `tmp/dxsp-2.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.6.5.tar", max compression
+gzip compressed data, was "dxsp-2.6.6.tar", max compression
```

## Comparing `dxsp-2.6.5.tar` & `dxsp-2.6.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-31 11:07:17.825988 dxsp-2.6.5/LICENSE
--rw-r--r--   0        0        0     2348 2023-05-31 11:07:17.825988 dxsp-2.6.5/README.md
--rw-r--r--   0        0        0       86 2023-05-31 11:07:18.658000 dxsp-2.6.5/dxsp/__init__.py
--rw-r--r--   0        0        0      386 2023-05-31 11:07:17.825988 dxsp-2.6.5/dxsp/config.py
--rw-r--r--   0        0        0     3679 2023-05-31 11:07:17.825988 dxsp-2.6.5/dxsp/default_settings.toml
--rw-r--r--   0        0        0    18920 2023-05-31 11:07:17.825988 dxsp-2.6.5/dxsp/main.py
--rw-r--r--   0        0        0     1542 2023-05-31 11:07:18.658000 dxsp-2.6.5/pyproject.toml
--rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 dxsp-2.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-31 20:19:18.937479 dxsp-2.6.6/LICENSE
+-rw-r--r--   0        0        0     2348 2023-05-31 20:19:18.937479 dxsp-2.6.6/README.md
+-rw-r--r--   0        0        0       86 2023-05-31 20:19:19.757527 dxsp-2.6.6/dxsp/__init__.py
+-rw-r--r--   0        0        0      387 2023-05-31 20:19:18.937479 dxsp-2.6.6/dxsp/config.py
+-rw-r--r--   0        0        0     3679 2023-05-31 20:19:18.937479 dxsp-2.6.6/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    18964 2023-05-31 20:19:18.937479 dxsp-2.6.6/dxsp/main.py
+-rw-r--r--   0        0        0     1542 2023-05-31 20:19:19.757527 dxsp-2.6.6/pyproject.toml
+-rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 dxsp-2.6.6/PKG-INFO
```

### Comparing `dxsp-2.6.5/LICENSE` & `dxsp-2.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.5/README.md` & `dxsp-2.6.6/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.5/dxsp/default_settings.toml` & `dxsp-2.6.6/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.5/dxsp/main.py` & `dxsp-2.6.6/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,28 +364,29 @@
                 abi=token_abi)
         except Exception as e:
             raise e
 
 # 🔒 USER RELATED
     async def get_token_balance(self, token_symbol: str) -> Optional[int]:
         """Get token balance"""
-        contract_address = await self.search_contract(token_symbol)
-        if not contract_address:
-            return None
+        # contract_address = await self.search_contract(token_symbol)
+        # if not contract_address:
+        #     return None
         contract = await self.get_token_contract(token_symbol)
         if not contract:
-            return None
-        return contract.functions.balanceOf(self.wallet_address).call() or 0
+            return 0
+        return contract.functions.balanceOf(self.wallet_address).call()
 
     async def get_token_decimals(self, token_symbol: str) -> Optional[int]:
         """Get token decimals"""
         contract = await self.get_token_contract(token_symbol)
         if not contract:
             return 18
-        return contract.functions.decimals().call()
+        token_decimals = contract.functions.decimals().call() or 18
+        return token_decimals
 
     async def get_account_balance(self):
         try:
             account_balance = self.w3.eth.get_balance(
                 self.w3.to_checksum_address(self.wallet_address))
             account_balance = self.w3.from_wei(account_balance, 'ether')
             trading_asset_balance = await self.get_trading_asset_balance()
```

### Comparing `dxsp-2.6.5/pyproject.toml` & `dxsp-2.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.6.5"
+version = "2.6.6"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-2.6.5/PKG-INFO` & `dxsp-2.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.6.5
+Version: 2.6.6
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

