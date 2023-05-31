# Comparing `tmp/flare_explorer_python-0.1.2.tar.gz` & `tmp/flare_explorer_python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flare_explorer_python-0.1.2.tar", max compression
+gzip compressed data, was "flare_explorer_python-0.1.3.tar", max compression
```

## Comparing `flare_explorer_python-0.1.2.tar` & `flare_explorer_python-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-01-22 16:09:45.273284 flare_explorer_python-0.1.2/LICENSE
--rw-r--r--   0        0        0     3020 2023-04-18 04:13:14.853407 flare_explorer_python-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-01-28 15:16:13.115891 flare_explorer_python-0.1.2/flare_explorer/__init__.py
--rw-r--r--   0        0        0     2342 2023-01-31 17:29:51.953472 flare_explorer_python-0.1.2/flare_explorer/address.py
--rw-r--r--   0        0        0     1110 2023-01-28 09:56:49.468982 flare_explorer_python-0.1.2/flare_explorer/block.py
--rw-r--r--   0        0        0      386 2023-04-18 04:13:14.853927 flare_explorer_python-0.1.2/flare_explorer/exceptions.py
--rw-r--r--   0        0        0     1513 2023-04-18 04:13:14.854282 flare_explorer_python-0.1.2/flare_explorer/gql_client.py
--rw-r--r--   0        0        0     1974 2023-02-03 18:56:57.596469 flare_explorer_python-0.1.2/flare_explorer/token_transfers.py
--rw-r--r--   0        0        0     5768 2023-01-28 17:48:10.167514 flare_explorer_python-0.1.2/flare_explorer/transaction.py
--rw-r--r--   0        0        0     1397 2023-04-18 04:58:48.241752 flare_explorer_python-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4101 1970-01-01 00:00:00.000000 flare_explorer_python-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-01-22 16:09:45.273284 flare_explorer_python-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3020 2023-04-18 04:13:14.853407 flare_explorer_python-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-01-28 15:16:13.115891 flare_explorer_python-0.1.3/flare_explorer/__init__.py
+-rw-r--r--   0        0        0     2342 2023-01-31 17:29:51.953472 flare_explorer_python-0.1.3/flare_explorer/address.py
+-rw-r--r--   0        0        0     1110 2023-01-28 09:56:49.468982 flare_explorer_python-0.1.3/flare_explorer/block.py
+-rw-r--r--   0        0        0      386 2023-04-18 04:13:14.853927 flare_explorer_python-0.1.3/flare_explorer/exceptions.py
+-rw-r--r--   0        0        0     1513 2023-04-18 04:13:14.854282 flare_explorer_python-0.1.3/flare_explorer/gql_client.py
+-rw-r--r--   0        0        0     1974 2023-02-03 18:56:57.596469 flare_explorer_python-0.1.3/flare_explorer/token_transfers.py
+-rw-r--r--   0        0        0     5768 2023-01-28 17:48:10.167514 flare_explorer_python-0.1.3/flare_explorer/transaction.py
+-rw-r--r--   0        0        0     1397 2023-05-31 17:39:18.446429 flare_explorer_python-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4101 1970-01-01 00:00:00.000000 flare_explorer_python-0.1.3/PKG-INFO
```

### Comparing `flare_explorer_python-0.1.2/LICENSE` & `flare_explorer_python-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flare_explorer_python-0.1.2/README.md` & `flare_explorer_python-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `flare_explorer_python-0.1.2/flare_explorer/address.py` & `flare_explorer_python-0.1.3/flare_explorer/address.py`

 * *Files identical despite different names*

### Comparing `flare_explorer_python-0.1.2/flare_explorer/block.py` & `flare_explorer_python-0.1.3/flare_explorer/block.py`

 * *Files identical despite different names*

### Comparing `flare_explorer_python-0.1.2/flare_explorer/gql_client.py` & `flare_explorer_python-0.1.3/flare_explorer/gql_client.py`

 * *Files identical despite different names*

### Comparing `flare_explorer_python-0.1.2/flare_explorer/token_transfers.py` & `flare_explorer_python-0.1.3/flare_explorer/token_transfers.py`

 * *Files identical despite different names*

### Comparing `flare_explorer_python-0.1.2/flare_explorer/transaction.py` & `flare_explorer_python-0.1.3/flare_explorer/transaction.py`

 * *Files identical despite different names*

### Comparing `flare_explorer_python-0.1.2/pyproject.toml` & `flare_explorer_python-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flare-explorer-python"
-version = "0.1.2"
+version = "0.1.3"
 description = "A lightweight library that works as a connector to the Flare explorer api"
 authors = ["James Davis <jamesecd@gmail.com>"]
 keywords = ["flare-explorer", "flare", "network", "api", "crypto", "blockchain"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `flare_explorer_python-0.1.2/PKG-INFO` & `flare_explorer_python-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flare-explorer-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: A lightweight library that works as a connector to the Flare explorer api
 Home-page: https://github.com/james-ecd/flare-explorer-python
 License: MIT
 Keywords: flare-explorer,flare,network,api,crypto,blockchain
 Author: James Davis
 Author-email: jamesecd@gmail.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flare-explorer-python Version: 0.1.2 Summary: A
+Metadata-Version: 2.1 Name: flare-explorer-python Version: 0.1.3 Summary: A
 lightweight library that works as a connector to the Flare explorer api Home-
 page: https://github.com/james-ecd/flare-explorer-python License: MIT Keywords:
 flare-explorer,flare,network,api,crypto,blockchain Author: James Davis Author-
 email: jamesecd@gmail.com Requires-Python: >=3.10,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
```

