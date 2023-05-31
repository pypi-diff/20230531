# Comparing `tmp/bacalhau_sdk-1.0.1.tar.gz` & `tmp/bacalhau_sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacalhau_sdk-1.0.1.tar", max compression
+gzip compressed data, was "bacalhau_sdk-1.0.2.tar", max compression
```

## Comparing `bacalhau_sdk-1.0.1.tar` & `bacalhau_sdk-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10247 2023-05-31 18:47:50.343812 bacalhau_sdk-1.0.1/LICENSE
--rw-r--r--   0        0        0     7401 2023-05-31 18:47:50.343812 bacalhau_sdk-1.0.1/README.md
--rw-r--r--   0        0        0      133 2023-05-31 18:47:50.343812 bacalhau_sdk-1.0.1/bacalhau_sdk/__init__.py
--rw-r--r--   0        0        0     3020 2023-05-31 18:47:50.343812 bacalhau_sdk-1.0.1/bacalhau_sdk/api.py
--rw-r--r--   0        0        0     5375 2023-05-31 18:47:50.343812 bacalhau_sdk-1.0.1/bacalhau_sdk/config.py
--rw-r--r--   0        0        0     2748 2023-05-31 18:48:20.930849 bacalhau_sdk-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       42 2023-05-31 18:47:50.343812 bacalhau_sdk-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     6458 2023-05-31 18:47:50.343812 bacalhau_sdk-1.0.1/tests/test_config.py
--rw-r--r--   0        0        0     9266 1970-01-01 00:00:00.000000 bacalhau_sdk-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10247 2023-05-31 20:18:31.529753 bacalhau_sdk-1.0.2/LICENSE
+-rw-r--r--   0        0        0     7401 2023-05-31 20:18:31.529753 bacalhau_sdk-1.0.2/README.md
+-rw-r--r--   0        0        0      133 2023-05-31 20:18:31.529753 bacalhau_sdk-1.0.2/bacalhau_sdk/__init__.py
+-rw-r--r--   0        0        0     3020 2023-05-31 20:18:31.529753 bacalhau_sdk-1.0.2/bacalhau_sdk/api.py
+-rw-r--r--   0        0        0     5375 2023-05-31 20:18:31.529753 bacalhau_sdk-1.0.2/bacalhau_sdk/config.py
+-rw-r--r--   0        0        0     2748 2023-05-31 20:18:58.225222 bacalhau_sdk-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-05-31 20:18:31.533753 bacalhau_sdk-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     6458 2023-05-31 20:18:31.533753 bacalhau_sdk-1.0.2/tests/test_config.py
+-rw-r--r--   0        0        0     9266 1970-01-01 00:00:00.000000 bacalhau_sdk-1.0.2/PKG-INFO
```

### Comparing `bacalhau_sdk-1.0.1/LICENSE` & `bacalhau_sdk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bacalhau_sdk-1.0.1/README.md` & `bacalhau_sdk-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bacalhau_sdk-1.0.1/bacalhau_sdk/api.py` & `bacalhau_sdk-1.0.2/bacalhau_sdk/api.py`

 * *Files identical despite different names*

### Comparing `bacalhau_sdk-1.0.1/bacalhau_sdk/config.py` & `bacalhau_sdk-1.0.2/bacalhau_sdk/config.py`

 * *Files identical despite different names*

### Comparing `bacalhau_sdk-1.0.1/pyproject.toml` & `bacalhau_sdk-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "bacalhau-sdk"
-version = "1.0.1"
+version = "1.0.2"
 homepage = "https://github.com/bacalhau-project/bacalhau/"
 repository = "https://github.com/bacalhau-project/bacalhau/"
 documentation = "https://docs.bacalhau.org/"
 keywords = ["bacalhau", "Filecoin", "IPFS", "cod", "compute over data", "verifiable computation"]
 description = "Compute over Data framework for public, transparent, and optionally verifiable computation using IPFS & Filecoin."
 authors = ["Enrico Rotundo <team@bacalhau.org>"]
 readme = "README.md"
```

### Comparing `bacalhau_sdk-1.0.1/tests/test_config.py` & `bacalhau_sdk-1.0.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `bacalhau_sdk-1.0.1/PKG-INFO` & `bacalhau_sdk-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacalhau-sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: Compute over Data framework for public, transparent, and optionally verifiable computation using IPFS & Filecoin.
 Home-page: https://github.com/bacalhau-project/bacalhau/
 License: Apache-2.0
 Keywords: bacalhau,Filecoin,IPFS,cod,compute over data,verifiable computation
 Author: Enrico Rotundo
 Author-email: team@bacalhau.org
 Requires-Python: >=3.8.1,<3.12
```

