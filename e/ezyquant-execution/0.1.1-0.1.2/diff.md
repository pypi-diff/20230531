# Comparing `tmp/ezyquant-execution-0.1.1.tar.gz` & `tmp/ezyquant-execution-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezyquant-execution-0.1.1.tar", last modified: Tue May 30 09:06:56 2023, max compression
+gzip compressed data, was "ezyquant-execution-0.1.2.tar", last modified: Wed May 31 03:21:44 2023, max compression
```

## Comparing `ezyquant-execution-0.1.1.tar` & `ezyquant-execution-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:06:56.143711 ezyquant-execution-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-30 09:06:56.143711 ezyquant-execution-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:06:56.143711 ezyquant-execution-0.1.1/ezyquant_execution/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/ezyquant_execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/ezyquant_execution/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/ezyquant_execution/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)    20382 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/ezyquant_execution/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/ezyquant_execution/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/ezyquant_execution/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/ezyquant_execution/executing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/ezyquant_execution/realtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/ezyquant_execution/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:06:56.143711 ezyquant-execution-0.1.1/ezyquant_execution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-30 09:06:56.000000 ezyquant-execution-0.1.1/ezyquant_execution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-30 09:06:56.000000 ezyquant-execution-0.1.1/ezyquant_execution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:06:56.000000 ezyquant-execution-0.1.1/ezyquant_execution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 09:06:56.000000 ezyquant-execution-0.1.1/ezyquant_execution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-30 09:06:56.000000 ezyquant-execution-0.1.1/ezyquant_execution.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-30 09:06:56.143711 ezyquant-execution-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:21:44.362013 ezyquant-execution-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-31 03:21:28.000000 ezyquant-execution-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-31 03:21:44.362013 ezyquant-execution-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-31 03:21:28.000000 ezyquant-execution-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:21:44.362013 ezyquant-execution-0.1.2/ezyquant_execution/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-31 03:21:28.000000 ezyquant-execution-0.1.2/ezyquant_execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 03:21:28.000000 ezyquant-execution-0.1.2/ezyquant_execution/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-31 03:21:28.000000 ezyquant-execution-0.1.2/ezyquant_execution/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-31 03:21:28.000000 ezyquant-execution-0.1.2/ezyquant_execution/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20872 2023-05-31 03:21:28.000000 ezyquant-execution-0.1.2/ezyquant_execution/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-05-31 03:21:28.000000 ezyquant-execution-0.1.2/ezyquant_execution/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-31 03:21:28.000000 ezyquant-execution-0.1.2/ezyquant_execution/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-31 03:21:28.000000 ezyquant-execution-0.1.2/ezyquant_execution/executing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-31 03:21:28.000000 ezyquant-execution-0.1.2/ezyquant_execution/realtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-31 03:21:28.000000 ezyquant-execution-0.1.2/ezyquant_execution/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:21:44.362013 ezyquant-execution-0.1.2/ezyquant_execution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-31 03:21:44.000000 ezyquant-execution-0.1.2/ezyquant_execution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-31 03:21:44.000000 ezyquant-execution-0.1.2/ezyquant_execution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 03:21:44.000000 ezyquant-execution-0.1.2/ezyquant_execution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-31 03:21:44.000000 ezyquant-execution-0.1.2/ezyquant_execution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-31 03:21:44.000000 ezyquant-execution-0.1.2/ezyquant_execution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-31 03:21:44.366013 ezyquant-execution-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-31 03:21:28.000000 ezyquant-execution-0.1.2/setup.py
```

### Comparing `ezyquant-execution-0.1.1/LICENSE.txt` & `ezyquant-execution-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.1.1/PKG-INFO` & `ezyquant-execution-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant-execution
-Version: 0.1.1
+Version: 0.1.2
 Summary: Ezyquant execution
 Home-page: https://pydoc.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-execution-0.1.1/ezyquant_execution/constant.py` & `ezyquant-execution-0.1.2/ezyquant_execution/constant.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.1.1/ezyquant_execution/context.py` & `ezyquant-execution-0.1.2/ezyquant_execution/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from settrade_v2.context import Context
 from settrade_v2.equity import InvestorEquity, MarketRepEquity
 from settrade_v2.market import MarketData
 from settrade_v2.realtime import RealtimeDataConnection
 from settrade_v2.user import Investor, MarketRep, _BaseUser
 
+from . import config as cfg
 from . import utils
 from .entity import (
     PRICE_TYPE,
     SIDE_BUY,
     SIDE_SELL,
     SIDE_TYPE,
     VALIDITY_TYPE,
@@ -545,39 +546,54 @@
         else:
             return self.sell_value(-value, **kwargs)
 
     """
     Validate order functions
     """
 
-    def is_buy_sufficient(
-        self, volume: float, price: float, pct_commission: float = 0.0
-    ) -> bool:
+    def is_buy_sufficient(self, volume: float, price: float = 0.0) -> bool:
         """Check if the line available is sufficient for buy order.
 
         Parameters
         ----------
         volume: float
             volume
         price: float
             price
         pct_commission: float
             percentage of commission example 0.01 for 1%
         """
-        return self.line_available >= volume * price * (1 + pct_commission)
+        return self.max_buy_volume(price) >= volume
 
     def is_sell_sufficient(self, volume: float) -> bool:
         """Check if the volume is sufficient for sell order.
 
         Parameters
         ----------
         volume: float
             volume
         """
-        return self.current_volume >= volume
+        return self.max_sell_volume() >= volume
+
+    def max_buy_volume(self, price: float = 0.0) -> float:
+        """Get maximum buy volume.
+
+        Parameters
+        ----------
+        price: float
+            price
+        """
+        # If price_type is not limit, price is not required.
+        if not price:
+            price = self.best_ask_price
+        return self.line_available / price / (1 + cfg.SETTRADE_COMMISSIION)
+
+    def max_sell_volume(self) -> float:
+        """Get maximum sell volume."""
+        return self.current_volume
 
     """
     Settrade SDK functions
     """
 
     @cached_property
     def _bo_sub(self) -> BidOfferSubscriber:
@@ -617,41 +633,42 @@
 
         Round volume to 100. If volume is 0, return None.
 
         Parameters
         ----------
         side: SIDE_TYPE
             Buy or sell
+        volume: float
+            volume to buy or sell. Will round to 100.
+        price: float
+            price to buy or sell. Must be 0 if price_type is Market.
         ...
         mode: PLACE_ORDER_MODE_TYPE
             none: no check
             skip: skip if not insufficient
             raise: raise error if not insufficient
             available: use available volume
         """
         volume = utils.round_100(volume, is_round_up_volume)
 
         if mode != "none":
             if side == SIDE_BUY:
-                if price == 0:
-                    max_volume = self.line_available / self.best_ask_price
-                else:
-                    max_volume = self.line_available / price
+                max_vol = self.max_buy_volume(price)
             else:
-                max_volume = self.current_volume
+                max_vol = self.max_sell_volume()
 
-            if max_volume < volume:
+            if max_vol < volume:
                 if mode == "skip":
                     logger.warn(f"{side} {volume} is not sufficient")
                     return
                 elif mode == "raise":
                     raise ValueError(f"{side} {volume} is not sufficient")
                 elif mode == "available":
-                    logger.info(f"{side} {volume} is not sufficient use {max_volume}")
-                    volume = max_volume
+                    logger.info(f"{side} {volume} is not sufficient use {max_vol}")
+                    volume = max_vol
                     is_round_up_volume = False
                 else:
                     raise ValueError(f"Invalid mode {mode}")
 
         return super().place_order(
             symbol=self.symbol,
             side=side,
```

### Comparing `ezyquant-execution-0.1.1/ezyquant_execution/entity.py` & `ezyquant-execution-0.1.2/ezyquant_execution/entity.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.1.1/ezyquant_execution/executing.py` & `ezyquant-execution-0.1.2/ezyquant_execution/executing.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.1.1/ezyquant_execution/realtime.py` & `ezyquant-execution-0.1.2/ezyquant_execution/realtime.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.1.1/ezyquant_execution/utils.py` & `ezyquant-execution-0.1.2/ezyquant_execution/utils.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.1.1/ezyquant_execution.egg-info/PKG-INFO` & `ezyquant-execution-0.1.2/ezyquant_execution.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant-execution
-Version: 0.1.1
+Version: 0.1.2
 Summary: Ezyquant execution
 Home-page: https://pydoc.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-execution-0.1.1/ezyquant_execution.egg-info/SOURCES.txt` & `ezyquant-execution-0.1.2/ezyquant_execution.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE.txt
 README.md
 setup.cfg
 setup.py
 ezyquant_execution/__init__.py
 ezyquant_execution/_version.py
+ezyquant_execution/config.py
 ezyquant_execution/constant.py
 ezyquant_execution/context.py
 ezyquant_execution/entity.py
 ezyquant_execution/environment.py
 ezyquant_execution/executing.py
 ezyquant_execution/realtime.py
 ezyquant_execution/utils.py
```

### Comparing `ezyquant-execution-0.1.1/setup.py` & `ezyquant-execution-0.1.2/setup.py`

 * *Files identical despite different names*

