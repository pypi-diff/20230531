# Comparing `tmp/quao-0.1.8a1.tar.gz` & `tmp/quao-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.1.8a1.tar", last modified: Wed May 31 04:29:23 2023, max compression
+gzip compressed data, was "quao-0.1.9.tar", last modified: Wed May 31 04:34:34 2023, max compression
```

## Comparing `quao-0.1.8a1.tar` & `quao-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 04:29:23.528714 quao-0.1.8a1/
--rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.1.8a1/LICENSE
--rw-rw-rw-   0        0        0     2841 2023-05-31 04:29:23.527714 quao-0.1.8a1/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.1.8a1/README.md
--rw-rw-rw-   0        0        0      854 2023-05-31 04:29:02.000000 quao-0.1.8a1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 04:29:23.528714 quao-0.1.8a1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-31 04:29:23.476655 quao-0.1.8a1/src/
--rw-rw-rw-   0        0        0        0 2023-05-29 11:56:58.000000 quao-0.1.8a1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 04:29:23.482656 quao-0.1.8a1/src/quao/
--rw-rw-rw-   0        0        0      134 2023-04-25 02:47:26.000000 quao-0.1.8a1/src/quao/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 04:29:23.512714 quao-0.1.8a1/src/quao/algorithms/
--rw-rw-rw-   0        0        0        2 2023-05-31 01:58:09.000000 quao-0.1.8a1/src/quao/algorithms/__init__.py
--rw-rw-rw-   0        0        0     5305 2023-05-31 01:58:09.000000 quao-0.1.8a1/src/quao/algorithms/shor.py
--rw-rw-rw-   0        0        0     3475 2023-05-31 04:28:29.000000 quao-0.1.8a1/src/quao/backend.py
-drwxrwxrwx   0        0        0        0 2023-05-31 04:29:23.517721 quao-0.1.8a1/src/quao/config/
--rw-rw-rw-   0        0        0        0 2023-05-29 11:56:58.000000 quao-0.1.8a1/src/quao/config/__init__.py
--rw-rw-rw-   0        0        0      189 2023-05-31 01:58:09.000000 quao-0.1.8a1/src/quao/config/loggingConfig.py
--rw-rw-rw-   0        0        0      179 2023-05-31 04:07:43.000000 quao-0.1.8a1/src/quao/config/threadConfig.py
--rw-rw-rw-   0        0        0      529 2023-05-31 01:58:09.000000 quao-0.1.8a1/src/quao/dataUtils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 04:29:23.520748 quao-0.1.8a1/src/quao/enum/
--rw-rw-rw-   0        0        0      200 2023-05-31 01:58:09.000000 quao-0.1.8a1/src/quao/enum/providerType.py
-drwxrwxrwx   0        0        0        0 2023-05-31 04:29:23.523715 quao-0.1.8a1/src/quao/sdk/
--rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.8a1/src/quao/sdk/__init__.py
--rw-rw-rw-   0        0        0     6415 2023-05-31 03:35:27.000000 quao-0.1.8a1/src/quao/sdk/qiskit.py
-drwxrwxrwx   0        0        0        0 2023-05-31 04:29:23.526716 quao-0.1.8a1/src/quao/status/
--rw-rw-rw-   0        0        0        0 2023-05-29 11:57:12.000000 quao-0.1.8a1/src/quao/status/__init__.py
--rw-rw-rw-   0        0        0     2450 2023-05-31 01:58:09.000000 quao-0.1.8a1/src/quao/status/qiskit_status.py
--rw-rw-rw-   0        0        0     1636 2023-05-31 01:58:09.000000 quao-0.1.8a1/src/quao/utilities.py
-drwxrwxrwx   0        0        0        0 2023-05-31 04:29:23.509714 quao-0.1.8a1/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2841 2023-05-31 04:29:23.000000 quao-0.1.8a1/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-05-31 04:29:23.000000 quao-0.1.8a1/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 04:29:23.000000 quao-0.1.8a1/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-05-31 04:29:23.000000 quao-0.1.8a1/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-31 04:29:23.000000 quao-0.1.8a1/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 04:34:34.387019 quao-0.1.9/
+-rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-05-31 04:34:34.386019 quao-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.1.9/README.md
+-rw-rw-rw-   0        0        0      846 2023-05-31 04:34:14.000000 quao-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 04:34:34.387019 quao-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 04:34:34.345421 quao-0.1.9/src/
+-rw-rw-rw-   0        0        0        0 2023-05-29 11:56:58.000000 quao-0.1.9/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:34:34.351419 quao-0.1.9/src/quao/
+-rw-rw-rw-   0        0        0      134 2023-04-25 02:47:26.000000 quao-0.1.9/src/quao/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:34:34.373020 quao-0.1.9/src/quao/algorithms/
+-rw-rw-rw-   0        0        0        2 2023-05-31 01:58:09.000000 quao-0.1.9/src/quao/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     5305 2023-05-31 01:58:09.000000 quao-0.1.9/src/quao/algorithms/shor.py
+-rw-rw-rw-   0        0        0     3475 2023-05-31 04:28:29.000000 quao-0.1.9/src/quao/backend.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:34:34.378020 quao-0.1.9/src/quao/config/
+-rw-rw-rw-   0        0        0        0 2023-05-29 11:56:58.000000 quao-0.1.9/src/quao/config/__init__.py
+-rw-rw-rw-   0        0        0      189 2023-05-31 01:58:09.000000 quao-0.1.9/src/quao/config/loggingConfig.py
+-rw-rw-rw-   0        0        0      179 2023-05-31 04:07:43.000000 quao-0.1.9/src/quao/config/threadConfig.py
+-rw-rw-rw-   0        0        0      529 2023-05-31 01:58:09.000000 quao-0.1.9/src/quao/dataUtils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:34:34.379019 quao-0.1.9/src/quao/enum/
+-rw-rw-rw-   0        0        0      200 2023-05-31 01:58:09.000000 quao-0.1.9/src/quao/enum/providerType.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:34:34.382022 quao-0.1.9/src/quao/sdk/
+-rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.9/src/quao/sdk/__init__.py
+-rw-rw-rw-   0        0        0     6415 2023-05-31 03:35:27.000000 quao-0.1.9/src/quao/sdk/qiskit.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:34:34.384020 quao-0.1.9/src/quao/status/
+-rw-rw-rw-   0        0        0        0 2023-05-29 11:57:12.000000 quao-0.1.9/src/quao/status/__init__.py
+-rw-rw-rw-   0        0        0     2450 2023-05-31 01:58:09.000000 quao-0.1.9/src/quao/status/qiskit_status.py
+-rw-rw-rw-   0        0        0     1636 2023-05-31 01:58:09.000000 quao-0.1.9/src/quao/utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:34:34.370067 quao-0.1.9/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-05-31 04:34:34.000000 quao-0.1.9/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-05-31 04:34:34.000000 quao-0.1.9/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 04:34:34.000000 quao-0.1.9/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-05-31 04:34:34.000000 quao-0.1.9/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-31 04:34:34.000000 quao-0.1.9/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.1.8a1/LICENSE` & `quao-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.1.8a1/PKG-INFO` & `quao-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.1.8a1
+Version: 0.1.9
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.1.8a1/README.md` & `quao-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.1.8a1/pyproject.toml` & `quao-0.1.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.1.8-alpha-1"
+version = "0.1.9"
 description = "Quao Library supporting Quao Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `quao-0.1.8a1/src/quao/algorithms/shor.py` & `quao-0.1.9/src/quao/algorithms/shor.py`

 * *Files identical despite different names*

### Comparing `quao-0.1.8a1/src/quao/backend.py` & `quao-0.1.9/src/quao/backend.py`

 * *Files identical despite different names*

### Comparing `quao-0.1.8a1/src/quao/dataUtils.py` & `quao-0.1.9/src/quao/dataUtils.py`

 * *Files identical despite different names*

### Comparing `quao-0.1.8a1/src/quao/sdk/qiskit.py` & `quao-0.1.9/src/quao/sdk/qiskit.py`

 * *Files identical despite different names*

### Comparing `quao-0.1.8a1/src/quao/status/qiskit_status.py` & `quao-0.1.9/src/quao/status/qiskit_status.py`

 * *Files identical despite different names*

### Comparing `quao-0.1.8a1/src/quao/utilities.py` & `quao-0.1.9/src/quao/utilities.py`

 * *Files identical despite different names*

### Comparing `quao-0.1.8a1/src/quao.egg-info/PKG-INFO` & `quao-0.1.9/src/quao.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.1.8a1
+Version: 0.1.9
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.1.8a1/src/quao.egg-info/SOURCES.txt` & `quao-0.1.9/src/quao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

