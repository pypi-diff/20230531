# Comparing `tmp/pytonconnect-0.2.1.tar.gz` & `tmp/pytonconnect-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytonconnect-0.2.1.tar", last modified: Fri May 19 12:28:27 2023, max compression
+gzip compressed data, was "pytonconnect-0.2.2.tar", last modified: Wed May 31 15:00:26 2023, max compression
```

## Comparing `pytonconnect-0.2.1.tar` & `pytonconnect-0.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 12:28:27.750445 pytonconnect-0.2.1/
--rw-rw-rw-   0        0        0    11558 2023-04-04 12:05:05.000000 pytonconnect-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     4688 2023-05-19 12:28:27.751443 pytonconnect-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3744 2023-04-19 17:53:09.000000 pytonconnect-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 12:28:27.214491 pytonconnect-0.2.1/pytonconnect/
--rw-rw-rw-   0        0        0      181 2023-04-25 09:15:01.000000 pytonconnect-0.2.1/pytonconnect/__init__.py
--rw-rw-rw-   0        0        0     9768 2023-05-19 08:40:25.000000 pytonconnect-0.2.1/pytonconnect/_ton_connect.py
--rw-rw-rw-   0        0        0     4737 2023-04-25 09:14:58.000000 pytonconnect-0.2.1/pytonconnect/_wallets_list_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:28:27.311916 pytonconnect-0.2.1/pytonconnect/crypto/
--rw-rw-rw-   0        0        0       84 2023-04-25 08:52:45.000000 pytonconnect-0.2.1/pytonconnect/crypto/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-04-19 17:53:09.000000 pytonconnect-0.2.1/pytonconnect/crypto/_session_crypto.py
--rw-rw-rw-   0        0        0     1928 2023-04-24 21:57:27.000000 pytonconnect-0.2.1/pytonconnect/exceptions.py
--rw-rw-rw-   0        0        0       96 2023-04-19 17:53:09.000000 pytonconnect-0.2.1/pytonconnect/logger.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:28:27.496024 pytonconnect-0.2.1/pytonconnect/parsers/
--rw-rw-rw-   0        0        0      293 2023-04-25 08:56:29.000000 pytonconnect-0.2.1/pytonconnect/parsers/__init__.py
--rw-rw-rw-   0        0        0     6329 2023-05-19 12:25:16.000000 pytonconnect-0.2.1/pytonconnect/parsers/_connect_event.py
--rw-rw-rw-   0        0        0      521 2023-04-19 17:56:13.000000 pytonconnect-0.2.1/pytonconnect/parsers/_rpc_parser.py
--rw-rw-rw-   0        0        0     1491 2023-04-25 08:54:29.000000 pytonconnect-0.2.1/pytonconnect/parsers/_send_transaction.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:28:27.716057 pytonconnect-0.2.1/pytonconnect/provider/
--rw-rw-rw-   0        0        0      153 2023-04-25 08:59:01.000000 pytonconnect-0.2.1/pytonconnect/provider/__init__.py
--rw-rw-rw-   0        0        0     4451 2023-04-26 17:08:50.000000 pytonconnect-0.2.1/pytonconnect/provider/_bridge_gateway.py
--rw-rw-rw-   0        0        0     8595 2023-04-25 08:59:03.000000 pytonconnect-0.2.1/pytonconnect/provider/_bridge_provider.py
--rw-rw-rw-   0        0        0      876 2023-04-19 17:53:09.000000 pytonconnect-0.2.1/pytonconnect/provider/_bridge_session.py
--rw-rw-rw-   0        0        0      613 2023-04-19 17:53:09.000000 pytonconnect-0.2.1/pytonconnect/provider/_provider.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:28:27.748444 pytonconnect-0.2.1/pytonconnect/storage/
--rw-rw-rw-   0        0        0      198 2023-05-10 18:51:06.000000 pytonconnect-0.2.1/pytonconnect/storage/__init__.py
--rw-rw-rw-   0        0        0      524 2023-04-25 09:00:27.000000 pytonconnect-0.2.1/pytonconnect/storage/_default_storage.py
--rw-rw-rw-   0        0        0     1401 2023-05-19 08:40:52.000000 pytonconnect-0.2.1/pytonconnect/storage/_file_storage.py
--rw-rw-rw-   0        0        0     1009 2023-04-19 17:53:09.000000 pytonconnect-0.2.1/pytonconnect/storage/_interface.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:28:27.308946 pytonconnect-0.2.1/pytonconnect.egg-info/
--rw-rw-rw-   0        0        0     4688 2023-05-19 12:28:26.000000 pytonconnect-0.2.1/pytonconnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      953 2023-05-19 12:28:26.000000 pytonconnect-0.2.1/pytonconnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 12:28:26.000000 pytonconnect-0.2.1/pytonconnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-11 12:27:07.000000 pytonconnect-0.2.1/pytonconnect.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2023-05-19 12:28:26.000000 pytonconnect-0.2.1/pytonconnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-19 12:28:26.000000 pytonconnect-0.2.1/pytonconnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1159 2023-05-19 12:28:27.752443 pytonconnect-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-04-19 17:53:09.000000 pytonconnect-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:00:26.893534 pytonconnect-0.2.2/
+-rw-rw-rw-   0        0        0    11558 2023-04-04 12:05:05.000000 pytonconnect-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     4688 2023-05-31 15:00:26.893534 pytonconnect-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3744 2023-04-19 17:53:09.000000 pytonconnect-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 15:00:26.844533 pytonconnect-0.2.2/pytonconnect/
+-rw-rw-rw-   0        0        0      181 2023-04-25 09:15:01.000000 pytonconnect-0.2.2/pytonconnect/__init__.py
+-rw-rw-rw-   0        0        0     9924 2023-05-31 14:57:30.000000 pytonconnect-0.2.2/pytonconnect/_ton_connect.py
+-rw-rw-rw-   0        0        0     4737 2023-04-25 09:14:58.000000 pytonconnect-0.2.2/pytonconnect/_wallets_list_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:00:26.873533 pytonconnect-0.2.2/pytonconnect/crypto/
+-rw-rw-rw-   0        0        0       84 2023-04-25 08:52:45.000000 pytonconnect-0.2.2/pytonconnect/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-04-19 17:53:09.000000 pytonconnect-0.2.2/pytonconnect/crypto/_session_crypto.py
+-rw-rw-rw-   0        0        0     1928 2023-04-24 21:57:27.000000 pytonconnect-0.2.2/pytonconnect/exceptions.py
+-rw-rw-rw-   0        0        0       96 2023-04-19 17:53:09.000000 pytonconnect-0.2.2/pytonconnect/logger.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:00:26.878532 pytonconnect-0.2.2/pytonconnect/parsers/
+-rw-rw-rw-   0        0        0      293 2023-04-25 08:56:29.000000 pytonconnect-0.2.2/pytonconnect/parsers/__init__.py
+-rw-rw-rw-   0        0        0     6329 2023-05-19 12:25:16.000000 pytonconnect-0.2.2/pytonconnect/parsers/_connect_event.py
+-rw-rw-rw-   0        0        0      521 2023-04-19 17:56:13.000000 pytonconnect-0.2.2/pytonconnect/parsers/_rpc_parser.py
+-rw-rw-rw-   0        0        0     1491 2023-04-25 08:54:29.000000 pytonconnect-0.2.2/pytonconnect/parsers/_send_transaction.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:00:26.885532 pytonconnect-0.2.2/pytonconnect/provider/
+-rw-rw-rw-   0        0        0      153 2023-04-25 08:59:01.000000 pytonconnect-0.2.2/pytonconnect/provider/__init__.py
+-rw-rw-rw-   0        0        0     4451 2023-04-26 17:08:50.000000 pytonconnect-0.2.2/pytonconnect/provider/_bridge_gateway.py
+-rw-rw-rw-   0        0        0     8595 2023-04-25 08:59:03.000000 pytonconnect-0.2.2/pytonconnect/provider/_bridge_provider.py
+-rw-rw-rw-   0        0        0      876 2023-04-19 17:53:09.000000 pytonconnect-0.2.2/pytonconnect/provider/_bridge_session.py
+-rw-rw-rw-   0        0        0      613 2023-04-19 17:53:09.000000 pytonconnect-0.2.2/pytonconnect/provider/_provider.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:00:26.891536 pytonconnect-0.2.2/pytonconnect/storage/
+-rw-rw-rw-   0        0        0      198 2023-05-10 18:51:06.000000 pytonconnect-0.2.2/pytonconnect/storage/__init__.py
+-rw-rw-rw-   0        0        0      524 2023-04-25 09:00:27.000000 pytonconnect-0.2.2/pytonconnect/storage/_default_storage.py
+-rw-rw-rw-   0        0        0     1401 2023-05-19 08:40:52.000000 pytonconnect-0.2.2/pytonconnect/storage/_file_storage.py
+-rw-rw-rw-   0        0        0     1009 2023-04-19 17:53:09.000000 pytonconnect-0.2.2/pytonconnect/storage/_interface.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:00:26.870532 pytonconnect-0.2.2/pytonconnect.egg-info/
+-rw-rw-rw-   0        0        0     4688 2023-05-31 15:00:26.000000 pytonconnect-0.2.2/pytonconnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      953 2023-05-31 15:00:26.000000 pytonconnect-0.2.2/pytonconnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 15:00:26.000000 pytonconnect-0.2.2/pytonconnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-11 12:27:07.000000 pytonconnect-0.2.2/pytonconnect.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2023-05-31 15:00:26.000000 pytonconnect-0.2.2/pytonconnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-31 15:00:26.000000 pytonconnect-0.2.2/pytonconnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1159 2023-05-31 15:00:26.899532 pytonconnect-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-04-19 17:53:09.000000 pytonconnect-0.2.2/setup.py
```

### Comparing `pytonconnect-0.2.1/LICENSE` & `pytonconnect-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.2.1/PKG-INFO` & `pytonconnect-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytonconnect
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python SDK for TON Connect 2.0
 Author: XaBbl4
 Author-email: xabbl4@gmail.com
 License: Apache 2.0
 Project-URL: Github, https://github.com/XaBbl4/pytonconnect
 Keywords: TON,TON Connect,TON Connect SDK
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pytonconnect-0.2.1/README.md` & `pytonconnect-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.2.1/pytonconnect/_ton_connect.py` & `pytonconnect-0.2.2/pytonconnect/_ton_connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,28 +35,30 @@
     @property
     def wallet(self):
         """Current connected wallet or None if no account is connected."""
         return self._wallet
 
 
     def __init__(self, manifest_url: str, storage: IStorage=DefaultStorage(), wallets_list_source: str = None, wallets_list_cache_ttl: int = None):
-        self._wallets_list = WalletsListManager(wallets_list_source=wallets_list_source, cache_ttl=wallets_list_cache_ttl)
+        if wallets_list_source is not None or wallets_list_cache_ttl is not None:
+            self._wallets_list = WalletsListManager(wallets_list_source=wallets_list_source, cache_ttl=wallets_list_cache_ttl)
 
         self._provider = None
         self._manifest_url = manifest_url
         self._storage = storage
 
         self._wallet = None
 
         self._status_change_subscriptions = []
         self._status_change_error_subscriptions = []
 
-    def get_wallets(self):
+
+    def get_wallets(self = None):
         """Return available wallets list."""
-        return self._wallets_list.get_wallets()
+        return TonConnect._wallets_list.get_wallets() if self is None else self._wallets_list.get_wallets()
 
 
     def on_status_change(self, callback, errors_handler = None):
         """Allows to subscribe to connection status changes and handle connection errors.
         
         :param callback: will be called after connections status changes with actual wallet or None
         :param errors_handler: will be called with some instance of TonConnectError when connect error is received
```

### Comparing `pytonconnect-0.2.1/pytonconnect/_wallets_list_manager.py` & `pytonconnect-0.2.2/pytonconnect/_wallets_list_manager.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.2.1/pytonconnect/crypto/_session_crypto.py` & `pytonconnect-0.2.2/pytonconnect/crypto/_session_crypto.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.2.1/pytonconnect/exceptions.py` & `pytonconnect-0.2.2/pytonconnect/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.2.1/pytonconnect/parsers/_connect_event.py` & `pytonconnect-0.2.2/pytonconnect/parsers/_connect_event.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.2.1/pytonconnect/parsers/_rpc_parser.py` & `pytonconnect-0.2.2/pytonconnect/parsers/_rpc_parser.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.2.1/pytonconnect/parsers/_send_transaction.py` & `pytonconnect-0.2.2/pytonconnect/parsers/_send_transaction.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.2.1/pytonconnect/provider/_bridge_gateway.py` & `pytonconnect-0.2.2/pytonconnect/provider/_bridge_gateway.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.2.1/pytonconnect/provider/_bridge_provider.py` & `pytonconnect-0.2.2/pytonconnect/provider/_bridge_provider.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.2.1/pytonconnect/provider/_bridge_session.py` & `pytonconnect-0.2.2/pytonconnect/provider/_bridge_session.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.2.1/pytonconnect/provider/_provider.py` & `pytonconnect-0.2.2/pytonconnect/provider/_provider.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.2.1/pytonconnect/storage/_default_storage.py` & `pytonconnect-0.2.2/pytonconnect/storage/_default_storage.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.2.1/pytonconnect/storage/_file_storage.py` & `pytonconnect-0.2.2/pytonconnect/storage/_file_storage.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.2.1/pytonconnect/storage/_interface.py` & `pytonconnect-0.2.2/pytonconnect/storage/_interface.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.2.1/pytonconnect.egg-info/PKG-INFO` & `pytonconnect-0.2.2/pytonconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytonconnect
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python SDK for TON Connect 2.0
 Author: XaBbl4
 Author-email: xabbl4@gmail.com
 License: Apache 2.0
 Project-URL: Github, https://github.com/XaBbl4/pytonconnect
 Keywords: TON,TON Connect,TON Connect SDK
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pytonconnect-0.2.1/pytonconnect.egg-info/SOURCES.txt` & `pytonconnect-0.2.2/pytonconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.2.1/setup.cfg` & `pytonconnect-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7974 6f6e 636f 6e6e 6563 740d   = pytonconnect.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e32 2e31  .version = 0.2.1
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e32 2e32  .version = 0.2.2
 00000030: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000040: 5079 7468 6f6e 2053 444b 2066 6f72 2054  Python SDK for T
 00000050: 4f4e 2043 6f6e 6e65 6374 2032 2e30 0d0a  ON Connect 2.0..
 00000060: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000070: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
 00000080: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
 00000090: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
```

