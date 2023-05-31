# Comparing `tmp/ossr_utils-0.1.4.tar.gz` & `tmp/ossr_utils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ossr_utils-0.1.4.tar", max compression
+gzip compressed data, was "ossr_utils-0.1.5.tar", max compression
```

## Comparing `ossr_utils-0.1.4.tar` & `ossr_utils-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       67 2023-05-12 16:15:06.843492 ossr_utils-0.1.4/README.md
--rw-r--r--   0        0        0      395 2023-05-30 19:00:25.150121 ossr_utils-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      116 2023-05-15 18:37:40.105429 ossr_utils-0.1.4/src/ossr_utils/__init__.py
--rw-r--r--   0        0        0      443 2023-05-12 16:08:56.032271 ossr_utils-0.1.4/src/ossr_utils/audio_utils.py
--rw-r--r--   0        0        0      981 2023-01-10 22:55:56.183254 ossr_utils-0.1.4/src/ossr_utils/fft_utils.py
--rw-r--r--   0        0        0      833 2023-05-30 18:51:27.382376 ossr_utils-0.1.4/src/ossr_utils/io_utils.py
--rw-r--r--   0        0        0     4836 2023-05-15 22:51:53.740635 ossr_utils-0.1.4/src/ossr_utils/misc_utils.py
--rw-r--r--   0        0        0      992 2023-01-27 15:44:16.196447 ossr_utils-0.1.4/src/ossr_utils/model_utils.py
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 ossr_utils-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       67 2023-05-12 16:15:06.843492 ossr_utils-0.1.5/README.md
+-rw-r--r--   0        0        0      395 2023-05-31 20:30:39.210189 ossr_utils-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      116 2023-05-15 18:37:40.105429 ossr_utils-0.1.5/src/ossr_utils/__init__.py
+-rw-r--r--   0        0        0      443 2023-05-12 16:08:56.032271 ossr_utils-0.1.5/src/ossr_utils/audio_utils.py
+-rw-r--r--   0        0        0      981 2023-01-10 22:55:56.183254 ossr_utils-0.1.5/src/ossr_utils/fft_utils.py
+-rw-r--r--   0        0        0      833 2023-05-30 18:51:27.382376 ossr_utils-0.1.5/src/ossr_utils/io_utils.py
+-rw-r--r--   0        0        0     4836 2023-05-15 22:51:53.740635 ossr_utils-0.1.5/src/ossr_utils/misc_utils.py
+-rw-r--r--   0        0        0      992 2023-01-27 15:44:16.196447 ossr_utils-0.1.5/src/ossr_utils/model_utils.py
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 ossr_utils-0.1.5/PKG-INFO
```

### Comparing `ossr_utils-0.1.4/src/ossr_utils/fft_utils.py` & `ossr_utils-0.1.5/src/ossr_utils/fft_utils.py`

 * *Files identical despite different names*

### Comparing `ossr_utils-0.1.4/src/ossr_utils/io_utils.py` & `ossr_utils-0.1.5/src/ossr_utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `ossr_utils-0.1.4/src/ossr_utils/misc_utils.py` & `ossr_utils-0.1.5/src/ossr_utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `ossr_utils-0.1.4/src/ossr_utils/model_utils.py` & `ossr_utils-0.1.5/src/ossr_utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `ossr_utils-0.1.4/PKG-INFO` & `ossr_utils-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossr-utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: Utils for the Open-Set Sound Recognition (OSSR) system
 License: MIT
 Author: Johannes Traa
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

