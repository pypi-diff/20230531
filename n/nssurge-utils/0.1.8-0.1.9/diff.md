# Comparing `tmp/nssurge_utils-0.1.8.tar.gz` & `tmp/nssurge_utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nssurge_utils-0.1.8.tar", max compression
+gzip compressed data, was "nssurge_utils-0.1.9.tar", max compression
```

## Comparing `nssurge_utils-0.1.8.tar` & `nssurge_utils-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-05-24 03:07:21.792499 nssurge_utils-0.1.8/README.md
--rw-r--r--   0        0        0       22 2023-05-31 07:51:54.008960 nssurge_utils-0.1.8/nssurge_utils/__init__.py
--rwxr-xr-x   0        0        0     3964 2023-05-27 15:20:15.536311 nssurge_utils-0.1.8/nssurge_utils/add_to_section.py
--rw-r--r--   0        0        0      815 2023-05-27 14:49:39.624596 nssurge_utils-0.1.8/nssurge_utils/config.py
--rw-r--r--   0        0        0    25596 2023-05-24 13:57:27.194926 nssurge_utils-0.1.8/nssurge_utils/data/countryFlagsNamesAndDialCodes.json
--rwxr-xr-x   0        0        0     8701 2023-05-31 07:46:07.159515 nssurge_utils-0.1.8/nssurge_utils/extract_proxy.py
--rw-r--r--   0        0        0     1809 2023-05-24 12:59:45.993775 nssurge_utils-0.1.8/nssurge_utils/parsers.py
--rw-r--r--   0        0        0      880 2023-05-24 12:09:19.509286 nssurge_utils-0.1.8/nssurge_utils/predicates.py
--rw-r--r--   0        0        0     1738 2023-05-31 07:44:56.704682 nssurge_utils-0.1.8/nssurge_utils/transform.py
--rw-r--r--   0        0        0      298 2023-05-24 03:20:15.526307 nssurge_utils-0.1.8/nssurge_utils/types.py
--rw-r--r--   0        0        0     8883 2023-05-31 07:35:50.226797 nssurge_utils-0.1.8/nssurge_utils/utils.py
--rw-r--r--   0        0        0      961 2023-05-31 07:51:54.007760 nssurge_utils-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 nssurge_utils-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-24 03:07:21.792499 nssurge_utils-0.1.9/README.md
+-rw-r--r--   0        0        0       22 2023-05-31 07:56:22.436657 nssurge_utils-0.1.9/nssurge_utils/__init__.py
+-rwxr-xr-x   0        0        0     3964 2023-05-27 15:20:15.536311 nssurge_utils-0.1.9/nssurge_utils/add_to_section.py
+-rw-r--r--   0        0        0      815 2023-05-27 14:49:39.624596 nssurge_utils-0.1.9/nssurge_utils/config.py
+-rw-r--r--   0        0        0    25596 2023-05-24 13:57:27.194926 nssurge_utils-0.1.9/nssurge_utils/data/countryFlagsNamesAndDialCodes.json
+-rwxr-xr-x   0        0        0     8701 2023-05-31 07:46:07.159515 nssurge_utils-0.1.9/nssurge_utils/extract_proxy.py
+-rw-r--r--   0        0        0     1809 2023-05-24 12:59:45.993775 nssurge_utils-0.1.9/nssurge_utils/parsers.py
+-rw-r--r--   0        0        0      880 2023-05-24 12:09:19.509286 nssurge_utils-0.1.9/nssurge_utils/predicates.py
+-rw-r--r--   0        0        0     1738 2023-05-31 07:44:56.704682 nssurge_utils-0.1.9/nssurge_utils/transform.py
+-rw-r--r--   0        0        0      298 2023-05-24 03:20:15.526307 nssurge_utils-0.1.9/nssurge_utils/types.py
+-rw-r--r--   0        0        0     8883 2023-05-31 07:35:50.226797 nssurge_utils-0.1.9/nssurge_utils/utils.py
+-rw-r--r--   0        0        0      961 2023-05-31 07:56:22.435552 nssurge_utils-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 nssurge_utils-0.1.9/PKG-INFO
```

### Comparing `nssurge_utils-0.1.8/nssurge_utils/add_to_section.py` & `nssurge_utils-0.1.9/nssurge_utils/add_to_section.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.8/nssurge_utils/config.py` & `nssurge_utils-0.1.9/nssurge_utils/config.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.8/nssurge_utils/data/countryFlagsNamesAndDialCodes.json` & `nssurge_utils-0.1.9/nssurge_utils/data/countryFlagsNamesAndDialCodes.json`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.8/nssurge_utils/extract_proxy.py` & `nssurge_utils-0.1.9/nssurge_utils/extract_proxy.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.8/nssurge_utils/parsers.py` & `nssurge_utils-0.1.9/nssurge_utils/parsers.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.8/nssurge_utils/predicates.py` & `nssurge_utils-0.1.9/nssurge_utils/predicates.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.8/nssurge_utils/transform.py` & `nssurge_utils-0.1.9/nssurge_utils/transform.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.8/nssurge_utils/utils.py` & `nssurge_utils-0.1.9/nssurge_utils/utils.py`

 * *Files identical despite different names*

### Comparing `nssurge_utils-0.1.8/pyproject.toml` & `nssurge_utils-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nssurge-utils"
-version = "0.1.8"
+version = "0.1.9"
 description = "NSSurge Utilities"
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "nssurge_utils" }]
 # include = ["data"]
 license = "MIT"
 homepage = "https://github.com/tddschn/nssurge-utils"
```

### Comparing `nssurge_utils-0.1.8/PKG-INFO` & `nssurge_utils-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nssurge-utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: NSSurge Utilities
 Home-page: https://github.com/tddschn/nssurge-utils
 License: MIT
 Keywords: nssurge,surge,utils
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
```

