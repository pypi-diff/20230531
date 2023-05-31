# Comparing `tmp/FJUtils-0.0.1.tar.gz` & `tmp/FJUtils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FJUtils-0.0.1.tar", last modified: Wed May 31 08:46:33 2023, max compression
+gzip compressed data, was "FJUtils-0.0.2.tar", last modified: Wed May 31 09:17:35 2023, max compression
```

## Comparing `FJUtils-0.0.1.tar` & `FJUtils-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-05-31 08:46:33.278549 FJUtils-0.0.1/
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-05-31 08:46:33.274549 FJUtils-0.0.1/FJUtils.egg-info/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2684 2023-05-31 08:46:33.000000 FJUtils-0.0.1/FJUtils.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      291 2023-05-31 08:46:33.000000 FJUtils-0.0.1/FJUtils.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-05-31 08:46:33.000000 FJUtils-0.0.1/FJUtils.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      122 2023-05-31 08:46:33.000000 FJUtils-0.0.1/FJUtils.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-05-31 08:46:33.000000 FJUtils-0.0.1/FJUtils.egg-info/top_level.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-05-31 06:53:13.000000 FJUtils-0.0.1/LICENSE
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2684 2023-05-31 08:46:33.274549 FJUtils-0.0.1/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1925 2023-05-31 08:45:55.000000 FJUtils-0.0.1/README.md
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-05-31 08:46:33.274549 FJUtils-0.0.1/fjutils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      708 2023-05-31 08:45:55.000000 FJUtils-0.0.1/fjutils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     8231 2023-05-31 08:45:55.000000 FJUtils-0.0.1/fjutils/checkpointing.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9903 2023-05-31 08:28:39.000000 FJUtils-0.0.1/fjutils/easylm.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1800 2023-05-31 08:45:55.000000 FJUtils-0.0.1/fjutils/load.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2257 2023-05-31 08:45:55.000000 FJUtils-0.0.1/fjutils/utils.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      533 2023-05-31 08:31:14.000000 FJUtils-0.0.1/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-05-31 08:46:33.278549 FJUtils-0.0.1/setup.cfg
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1215 2023-05-31 08:45:05.000000 FJUtils-0.0.1/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-05-31 09:17:35.322928 FJUtils-0.0.2/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-05-31 09:17:35.322928 FJUtils-0.0.2/FJUtils.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2684 2023-05-31 09:17:35.000000 FJUtils-0.0.2/FJUtils.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      291 2023-05-31 09:17:35.000000 FJUtils-0.0.2/FJUtils.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-05-31 09:17:35.000000 FJUtils-0.0.2/FJUtils.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      122 2023-05-31 09:17:35.000000 FJUtils-0.0.2/FJUtils.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-05-31 09:17:35.000000 FJUtils-0.0.2/FJUtils.egg-info/top_level.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-05-31 06:53:13.000000 FJUtils-0.0.2/LICENSE
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2684 2023-05-31 09:17:35.322928 FJUtils-0.0.2/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1925 2023-05-31 08:45:55.000000 FJUtils-0.0.2/README.md
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-05-31 09:17:35.322928 FJUtils-0.0.2/fjutils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      708 2023-05-31 08:45:55.000000 FJUtils-0.0.2/fjutils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8231 2023-05-31 08:45:55.000000 FJUtils-0.0.2/fjutils/checkpointing.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9903 2023-05-31 08:28:39.000000 FJUtils-0.0.2/fjutils/easylm.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1800 2023-05-31 08:45:55.000000 FJUtils-0.0.2/fjutils/load.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2257 2023-05-31 08:45:55.000000 FJUtils-0.0.2/fjutils/utils.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      533 2023-05-31 08:31:14.000000 FJUtils-0.0.2/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-05-31 09:17:35.322928 FJUtils-0.0.2/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1215 2023-05-31 09:17:00.000000 FJUtils-0.0.2/setup.py
```

### Comparing `FJUtils-0.0.1/FJUtils.egg-info/PKG-INFO` & `FJUtils-0.0.2/FJUtils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FJUtils
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: https://github.com/erfanzar/
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@yahoo.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6, <3.11
+Requires-Python: >=3.7, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FJUtils
 
 a package for custom Jax Flax Functions and Utils
 Welcome to FJUtils - A collection of useful functions and utilities for Flax and JAX!
```

### Comparing `FJUtils-0.0.1/LICENSE` & `FJUtils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.1/PKG-INFO` & `FJUtils-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FJUtils
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: https://github.com/erfanzar/
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@yahoo.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6, <3.11
+Requires-Python: >=3.7, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FJUtils
 
 a package for custom Jax Flax Functions and Utils
 Welcome to FJUtils - A collection of useful functions and utilities for Flax and JAX!
```

### Comparing `FJUtils-0.0.1/README.md` & `FJUtils-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.1/fjutils/__init__.py` & `FJUtils-0.0.2/fjutils/__init__.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.1/fjutils/checkpointing.py` & `FJUtils-0.0.2/fjutils/checkpointing.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.1/fjutils/easylm.py` & `FJUtils-0.0.2/fjutils/easylm.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.1/fjutils/load.py` & `FJUtils-0.0.2/fjutils/load.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.1/fjutils/utils.py` & `FJUtils-0.0.2/fjutils/utils.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.1/pyproject.toml` & `FJUtils-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.1/setup.py` & `FJUtils-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="FJUtils",
-    version='0.0.1',
+    version='0.0.2',
     author="Erfan Zare Chavoshi",
     author_email="erfanzare82@yahoo.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/erfanzar/",
     packages=setuptools.find_packages(),
     install_requires=[
@@ -20,15 +20,15 @@
         'typing~=3.7.4.3',
         'numpy~=1.24.3',
         'flax~=0.6.4',
         'msgpack~=1.0.5',
         'setuptools~=59.6.0',
         'mlxu~=0.1.11'
     ],
-    python_requires=">=3.6, <3.11",
+    python_requires=">=3.7, <3.11",
     license='Apache License 2.0',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
```

