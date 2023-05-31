# Comparing `tmp/dcentrapi-0.2.2.tar.gz` & `tmp/dcentrapi-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentrapi-0.2.2.tar", last modified: Wed May 24 09:46:10 2023, max compression
+gzip compressed data, was "dcentrapi-0.2.3.tar", last modified: Wed May 31 13:36:43 2023, max compression
```

## Comparing `dcentrapi-0.2.2.tar` & `dcentrapi-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-05-24 09:46:10.641259 dcentrapi-0.2.2/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1073 2022-10-09 08:58:27.000000 dcentrapi-0.2.2/LICENSE.rst
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6780 2023-05-24 09:46:10.641123 dcentrapi-0.2.2/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6211 2022-10-09 08:58:27.000000 dcentrapi-0.2.2/README.md
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-05-24 09:46:10.640300 dcentrapi-0.2.2/dcentrapi/
--rw-r--r--   0 nivshitrit   (501) staff       (20)      829 2023-05-24 09:45:16.000000 dcentrapi-0.2.2/dcentrapi/Base.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      280 2023-03-08 10:39:09.000000 dcentrapi-0.2.2/dcentrapi/__init__.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)       63 2023-05-24 09:45:42.000000 dcentrapi-0.2.2/dcentrapi/common.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     7885 2023-05-24 09:45:16.000000 dcentrapi-0.2.2/dcentrapi/eventPolling.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)      491 2023-03-02 14:02:13.000000 dcentrapi-0.2.2/dcentrapi/gasMonitor.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     3078 2022-11-22 15:13:50.000000 dcentrapi-0.2.2/dcentrapi/merkleTree.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     3301 2023-05-24 09:45:16.000000 dcentrapi-0.2.2/dcentrapi/rpcAggregation.py
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1186 2023-05-24 09:45:16.000000 dcentrapi-0.2.2/dcentrapi/web3Index.py
-drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-05-24 09:46:10.640945 dcentrapi-0.2.2/dcentrapi.egg-info/
--rw-r--r--   0 nivshitrit   (501) staff       (20)     6780 2023-05-24 09:46:10.000000 dcentrapi-0.2.2/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 nivshitrit   (501) staff       (20)      379 2023-05-24 09:46:10.000000 dcentrapi-0.2.2/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        1 2023-05-24 09:46:10.000000 dcentrapi-0.2.2/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)        9 2023-05-24 09:46:10.000000 dcentrapi-0.2.2/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       10 2023-05-24 09:46:10.000000 dcentrapi-0.2.2/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 nivshitrit   (501) staff       (20)       38 2023-05-24 09:46:10.641299 dcentrapi-0.2.2/setup.cfg
--rw-r--r--   0 nivshitrit   (501) staff       (20)     1167 2023-04-09 07:57:53.000000 dcentrapi-0.2.2/setup.py
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-05-31 13:36:43.440873 dcentrapi-0.2.3/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     1073 2022-10-09 08:58:27.000000 dcentrapi-0.2.3/LICENSE.rst
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6780 2023-05-31 13:36:43.440712 dcentrapi-0.2.3/PKG-INFO
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6211 2022-10-09 08:58:27.000000 dcentrapi-0.2.3/README.md
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-05-31 13:36:43.439937 dcentrapi-0.2.3/dcentrapi/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      829 2023-05-24 09:45:16.000000 dcentrapi-0.2.3/dcentrapi/Base.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      280 2023-03-08 10:39:09.000000 dcentrapi-0.2.3/dcentrapi/__init__.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)       63 2023-05-31 13:36:41.000000 dcentrapi-0.2.3/dcentrapi/common.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     7885 2023-05-24 09:45:16.000000 dcentrapi-0.2.3/dcentrapi/eventPolling.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      491 2023-03-02 14:02:13.000000 dcentrapi-0.2.3/dcentrapi/gasMonitor.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     3078 2022-11-22 15:13:50.000000 dcentrapi-0.2.3/dcentrapi/merkleTree.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     3850 2023-05-31 13:35:59.000000 dcentrapi-0.2.3/dcentrapi/rpcAggregation.py
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      804 2023-05-31 13:35:59.000000 dcentrapi-0.2.3/dcentrapi/web3Index.py
+drwxr-xr-x   0 nivshitrit   (501) staff       (20)        0 2023-05-31 13:36:43.440544 dcentrapi-0.2.3/dcentrapi.egg-info/
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     6780 2023-05-31 13:36:43.000000 dcentrapi-0.2.3/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 nivshitrit   (501) staff       (20)      379 2023-05-31 13:36:43.000000 dcentrapi-0.2.3/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)        1 2023-05-31 13:36:43.000000 dcentrapi-0.2.3/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)        9 2023-05-31 13:36:43.000000 dcentrapi-0.2.3/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)       10 2023-05-31 13:36:43.000000 dcentrapi-0.2.3/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 nivshitrit   (501) staff       (20)       38 2023-05-31 13:36:43.440983 dcentrapi-0.2.3/setup.cfg
+-rw-r--r--   0 nivshitrit   (501) staff       (20)     1167 2023-04-09 07:57:53.000000 dcentrapi-0.2.3/setup.py
```

### Comparing `dcentrapi-0.2.2/LICENSE.rst` & `dcentrapi-0.2.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.2/PKG-INFO` & `dcentrapi-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.2
+Version: 0.2.3
 Summary: Dcentralab Pypi packages
 Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `dcentrapi-0.2.2/README.md` & `dcentrapi-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.2/dcentrapi/Base.py` & `dcentrapi-0.2.3/dcentrapi/Base.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.2/dcentrapi/eventPolling.py` & `dcentrapi-0.2.3/dcentrapi/eventPolling.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.2/dcentrapi/merkleTree.py` & `dcentrapi-0.2.3/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.2.2/dcentrapi/rpcAggregation.py` & `dcentrapi-0.2.3/dcentrapi/rpcAggregation.py`

 * *Files 22% similar despite different names*

```diff
@@ -36,28 +36,43 @@
 
     def get_reserves_from_pair(self, pool, network, rpc_url=None):
         url = self.url + "getReservesFromPair"
         data = {"network": network, "lp_token": pool, "rpc_url": rpc_url}
         response = requests.get(url, params=data, headers=self.headers)
         return response.json()
 
+    # DEPRECATED, use get_reserves_from_pools instead, it is more general
     def get_reserves_from_pairs(self, pools: list, network, rpc_url=None):
         url = self.url + "getReservesFromPairs"
         data = {"network": network, "lp_tokens": pools, "rpc_url": rpc_url}
         response = requests.post(url, json=data, headers=self.headers)
         return response.json()
 
+    # Accepted values for factory_type (May 2023):
+    # UNI_V2, UNI_V3, CURVE, BALANCER
+
+    def get_reserves_from_pools(self, factory_type, pools: list, network, rpc_url=None):
+        url = self.url + "getReservesFromPools"
+        data = {
+            "factory_type": factory_type,
+            "pools": pools,
+            "network": network,
+            "rpc_url": rpc_url
+        }
+        response = requests.post(url, json=data, headers=self.headers)
+        return response.json()
+
     # DEPRECATED, use get_pool_data_from_factory instead, it is more general
     def get_pair_data_from_factory(self, factory, indices: list, network, rpc_url=None):
         url = self.url + "getPairDataFromFactory"
         data = {"factory": factory, "indices": indices, "network": network, "rpc_url": rpc_url}
         response = requests.post(url, json=data, headers=self.headers)
         return response.json()
 
-    # factory_type should be a recognised type from "uni_v2", "curve", and some other types
+    # Same accepted factory_type values as for get_reserves_from_pools above
     def get_pool_data_from_factory(self, factory_type, factory, indices: list, network, rpc_url=None):
         url = self.url + "getPoolDataFromFactory"
         data = {
             "factory_type": factory_type,
             "factory": factory,
             "indices": indices,
             "network": network,
```

### Comparing `dcentrapi-0.2.2/dcentrapi/web3Index.py` & `dcentrapi-0.2.3/dcentrapi/web3Index.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,13 @@
 import requests
 
 from dcentrapi.Base import Base
 
 
 class Web3Index(Base):
-    # ----- Data from DUB Backend -----
-
-    def get_reserves_from_pairs(self, pools: list, network, rpc_url=None):
-        url = self.url + "getReservesFromPairs"
-        data = {"network": network, "lp_tokens": pools, "rpc_url": rpc_url}
-        response = requests.post(url, json=data, headers=self.headers)
-        return response.json()
-
-    # ----- Data from Web3Index -----
-
     def get_pairs(self, network_name: str, token_address: str):
         url = self.web3index_url + "pairs" + f"/{network_name}/{token_address}"
         response = requests.get(url, headers=self.headers)
         return response.json()
 
     def get_factories(self):
         url = self.web3index_url + "factories"
```

### Comparing `dcentrapi-0.2.2/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.2.3/dcentrapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.2.2
+Version: 0.2.3
 Summary: Dcentralab Pypi packages
 Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `dcentrapi-0.2.2/setup.py` & `dcentrapi-0.2.3/setup.py`

 * *Files identical despite different names*

