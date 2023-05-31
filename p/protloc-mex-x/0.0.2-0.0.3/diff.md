# Comparing `tmp/protloc_mex_x-0.0.2.tar.gz` & `tmp/protloc_mex_x-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protloc_mex_x-0.0.2.tar", max compression
+gzip compressed data, was "protloc_mex_x-0.0.3.tar", max compression
```

## Comparing `protloc_mex_x-0.0.2.tar` & `protloc_mex_x-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1091 2023-04-25 08:38:35.586641 protloc_mex_x-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0        2 2023-05-09 03:41:02.000000 protloc_mex_x-0.0.2/protloc_mex_X/__init__.py
--rw-r--r--   0        0        0    36871 2023-05-31 08:20:32.000000 protloc_mex_x-0.0.2/protloc_mex_X/ESM2_fr.py
--rw-r--r--   0        0        0     2999 2023-05-08 12:33:04.000000 protloc_mex_x-0.0.2/protloc_mex_X/examples/test1.txt
--rw-r--r--   0        0        0     2749 2023-05-09 03:13:02.000000 protloc_mex_x-0.0.2/protloc_mex_X/feature_corrlation.py
--rw-r--r--   0        0        0      863 2023-05-31 08:35:47.770448 protloc_mex_x-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-10 08:06:08.458858 protloc_mex_x-0.0.2/README.md
--rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 protloc_mex_x-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-25 08:38:35.586641 protloc_mex_x-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0        2 2023-05-09 03:41:02.000000 protloc_mex_x-0.0.3/protloc_mex_X/__init__.py
+-rw-r--r--   0        0        0    36861 2023-05-31 10:09:36.000000 protloc_mex_x-0.0.3/protloc_mex_X/ESM2_fr.py
+-rw-r--r--   0        0        0     2999 2023-05-08 12:33:04.000000 protloc_mex_x-0.0.3/protloc_mex_X/examples/test1.txt
+-rw-r--r--   0        0        0     2749 2023-05-09 03:13:02.000000 protloc_mex_x-0.0.3/protloc_mex_X/feature_corrlation.py
+-rw-r--r--   0        0        0      863 2023-05-31 13:10:53.302882 protloc_mex_x-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-05-10 08:06:08.458858 protloc_mex_x-0.0.3/README.md
+-rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 protloc_mex_x-0.0.3/PKG-INFO
```

### Comparing `protloc_mex_x-0.0.2/LICENSE.txt` & `protloc_mex_x-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.2/protloc_mex_X/ESM2_fr.py` & `protloc_mex_x-0.0.3/protloc_mex_X/ESM2_fr.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,16 +180,16 @@
                             features_length['mean'] = len(mean_features)
                         features.extend(mean_features)
 
                     if segment_means is not None:
                         # In the new version, we keep each segment mean as a separate list
                         for seg, segment_mean in enumerate(segment_means):
                             features.extend(segment_mean)
-                            if f'ESM2_segment{seg}_mean' not in features_length:
-                                features_length[f'ESM2_segment{seg}_mean'] = len(segment_mean)
+                            if f'segment{seg}_mean' not in features_length:
+                                features_length[f'segment{seg}_mean'] = len(segment_mean)
 
                     # create the column names only for the first item
                     if columns is None:
                         columns = []
                         for feature_type, length in features_length.items():
                             for k in range(length):
                                 columns.append(f"ESM2_{feature_type}{k}")
```

### Comparing `protloc_mex_x-0.0.2/protloc_mex_X/examples/test1.txt` & `protloc_mex_x-0.0.3/protloc_mex_X/examples/test1.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.2/protloc_mex_X/feature_corrlation.py` & `protloc_mex_x-0.0.3/protloc_mex_X/feature_corrlation.py`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.2/pyproject.toml` & `protloc_mex_x-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "protloc_mex_X"
-version = "0.0.2"
+version = "0.0.3"
 description = "Internal use kit"
 authors = ["Ze Yu Luo <1024226968@qq.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/yujuan-zhang/ProtLoc-mexl"
 repository = "https://github.com/yujuan-zhang/ProtLoc-mexl"
 documentation = "https://github.com/yujuan-zhang/ProtLoc-mexl/issues"
```

### Comparing `protloc_mex_x-0.0.2/PKG-INFO` & `protloc_mex_x-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protloc-mex-x
-Version: 0.0.2
+Version: 0.0.3
 Summary: Internal use kit
 Home-page: https://github.com/yujuan-zhang/ProtLoc-mexl
 License: MIT
 Author: Ze Yu Luo
 Author-email: 1024226968@qq.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 3 - Alpha
```

