# Comparing `tmp/autodistill-0.1.0.tar.gz` & `tmp/autodistill-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autodistill-0.1.0.tar", last modified: Sat May 27 03:01:49 2023, max compression
+gzip compressed data, was "autodistill-0.1.1.tar", last modified: Wed May 31 06:32:22 2023, max compression
```

## Comparing `autodistill-0.1.0.tar` & `autodistill-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 03:01:49.000000 autodistill-0.1.0/
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     1055 2023-05-27 02:54:55.000000 autodistill-0.1.0/LICENSE.md
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     5598 2023-05-27 03:01:49.000000 autodistill-0.1.0/PKG-INFO
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     5088 2023-05-27 02:54:55.000000 autodistill-0.1.0/README.md
-drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 03:01:49.000000 autodistill-0.1.0/autodistill/
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       22 2023-05-27 03:01:09.000000 autodistill-0.1.0/autodistill/__init__.py
-drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 03:01:49.000000 autodistill-0.1.0/autodistill/core/
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      151 2023-05-27 02:54:55.000000 autodistill-0.1.0/autodistill/core/__init__.py
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      518 2023-05-27 02:54:55.000000 autodistill-0.1.0/autodistill/core/base_model.py
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      114 2023-05-27 02:54:55.000000 autodistill-0.1.0/autodistill/core/ontology.py
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      236 2023-05-27 02:54:55.000000 autodistill-0.1.0/autodistill/core/target_model.py
-drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 03:01:49.000000 autodistill-0.1.0/autodistill/detection/
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      290 2023-05-27 02:54:55.000000 autodistill-0.1.0/autodistill/detection/__init__.py
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      372 2023-05-27 02:54:55.000000 autodistill-0.1.0/autodistill/detection/caption_ontology.py
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     1760 2023-05-27 02:54:55.000000 autodistill-0.1.0/autodistill/detection/detection_base_model.py
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      769 2023-05-27 02:54:55.000000 autodistill-0.1.0/autodistill/detection/detection_ontology.py
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      366 2023-05-27 02:54:55.000000 autodistill-0.1.0/autodistill/detection/detection_target_model.py
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     3258 2023-05-27 02:54:55.000000 autodistill-0.1.0/autodistill/helpers.py
-drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 03:01:49.000000 autodistill-0.1.0/autodistill.egg-info/
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     5598 2023-05-27 03:01:48.000000 autodistill-0.1.0/autodistill.egg-info/PKG-INFO
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      605 2023-05-27 03:01:49.000000 autodistill-0.1.0/autodistill.egg-info/SOURCES.txt
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)        1 2023-05-27 03:01:48.000000 autodistill-0.1.0/autodistill.egg-info/dependency_links.txt
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      142 2023-05-27 03:01:48.000000 autodistill-0.1.0/autodistill.egg-info/requires.txt
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       12 2023-05-27 03:01:48.000000 autodistill-0.1.0/autodistill.egg-info/top_level.txt
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       38 2023-05-27 03:01:49.000000 autodistill-0.1.0/setup.cfg
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     1232 2023-05-27 02:54:55.000000 autodistill-0.1.0/setup.py
-drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 03:01:49.000000 autodistill-0.1.0/test/
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       41 2023-05-27 02:54:55.000000 autodistill-0.1.0/test/test_hello.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-31 06:32:22.647574 autodistill-0.1.1/
+-rw-r--r--   0 james      (501) staff       (20)     1055 2023-05-30 17:10:38.000000 autodistill-0.1.1/LICENSE.md
+-rw-r--r--   0 james      (501) staff       (20)     5598 2023-05-31 06:32:22.647421 autodistill-0.1.1/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     5088 2023-05-30 17:10:38.000000 autodistill-0.1.1/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-31 06:32:22.644012 autodistill-0.1.1/autodistill/
+-rw-r--r--   0 james      (501) staff       (20)       22 2023-05-31 06:25:33.000000 autodistill-0.1.1/autodistill/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-31 06:32:22.645825 autodistill-0.1.1/autodistill/core/
+-rw-r--r--   0 james      (501) staff       (20)      151 2023-05-30 17:11:28.000000 autodistill-0.1.1/autodistill/core/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      516 2023-05-30 17:13:34.000000 autodistill-0.1.1/autodistill/core/base_model.py
+-rw-r--r--   0 james      (501) staff       (20)      114 2023-05-30 17:11:28.000000 autodistill-0.1.1/autodistill/core/ontology.py
+-rw-r--r--   0 james      (501) staff       (20)      236 2023-05-30 17:11:28.000000 autodistill-0.1.1/autodistill/core/target_model.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-31 06:32:22.646871 autodistill-0.1.1/autodistill/detection/
+-rw-r--r--   0 james      (501) staff       (20)      290 2023-05-30 17:11:28.000000 autodistill-0.1.1/autodistill/detection/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      580 2023-05-30 19:12:05.000000 autodistill-0.1.1/autodistill/detection/caption_ontology.py
+-rw-r--r--   0 james      (501) staff       (20)     1760 2023-05-30 17:11:28.000000 autodistill-0.1.1/autodistill/detection/detection_base_model.py
+-rw-r--r--   0 james      (501) staff       (20)      769 2023-05-30 17:23:36.000000 autodistill-0.1.1/autodistill/detection/detection_ontology.py
+-rw-r--r--   0 james      (501) staff       (20)      366 2023-05-30 17:11:28.000000 autodistill-0.1.1/autodistill/detection/detection_target_model.py
+-rw-r--r--   0 james      (501) staff       (20)     3258 2023-05-30 17:11:28.000000 autodistill-0.1.1/autodistill/helpers.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-31 06:32:22.644829 autodistill-0.1.1/autodistill.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     5598 2023-05-31 06:32:22.000000 autodistill-0.1.1/autodistill.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      605 2023-05-31 06:32:22.000000 autodistill-0.1.1/autodistill.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-05-31 06:32:22.000000 autodistill-0.1.1/autodistill.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      142 2023-05-31 06:32:22.000000 autodistill-0.1.1/autodistill.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       12 2023-05-31 06:32:22.000000 autodistill-0.1.1/autodistill.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-05-31 06:32:22.647624 autodistill-0.1.1/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1265 2023-05-31 06:32:18.000000 autodistill-0.1.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-31 06:32:22.647074 autodistill-0.1.1/test/
+-rw-r--r--   0 james      (501) staff       (20)       41 2023-05-30 17:10:38.000000 autodistill-0.1.1/test/test_hello.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `autodistill-0.1.0/LICENSE.md` & `autodistill-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.0/PKG-INFO` & `autodistill-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill
-Version: 0.1.0
+Version: 0.1.1
 Summary: Distill large foundational models into smaller, domain-specific models for deployment
 Home-page: https://github.com/autodistill/autodistill
 Author: Roboflow
 Author-email: jacob@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `autodistill-0.1.0/README.md` & `autodistill-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.0/autodistill/core/base_model.py` & `autodistill-0.1.1/autodistill/core/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,9 +13,9 @@
         self.ontology = ontology
 
     @abstractmethod
     def predict(self, input: Any) -> Any:
         pass
 
     @abstractmethod
-    def label(self, context_folder: str, extension: str = ".jpg", output_folder: str = None) -> sv.BaseDataset:
+    def label(self, input_folder: str, extension: str = ".jpg", output_folder: str = None) -> sv.BaseDataset:
         pass
```

### Comparing `autodistill-0.1.0/autodistill/detection/detection_base_model.py` & `autodistill-0.1.1/autodistill/detection/detection_base_model.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.0/autodistill/detection/detection_ontology.py` & `autodistill-0.1.1/autodistill/detection/detection_ontology.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.0/autodistill/helpers.py` & `autodistill-0.1.1/autodistill/helpers.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.0/autodistill.egg-info/PKG-INFO` & `autodistill-0.1.1/autodistill.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill
-Version: 0.1.0
+Version: 0.1.1
 Summary: Distill large foundational models into smaller, domain-specific models for deployment
 Home-page: https://github.com/autodistill/autodistill
 Author: Roboflow
 Author-email: jacob@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `autodistill-0.1.0/autodistill.egg-info/SOURCES.txt` & `autodistill-0.1.1/autodistill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.0/setup.py` & `autodistill-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import setuptools
 from setuptools import find_packages
 import re
+import os
 
 with open("./autodistill/__init__.py", 'r') as f:
     content = f.read()
     # from https://www.py4u.net/discuss/139845
     version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-with open("requirements.txt", "r") as fh:
-    install_requires = fh.read().split('\n')
-
 setuptools.setup(
     name="autodistill",  
     version=version,
     author="Roboflow",
     author_email="jacob@roboflow.com",
     description="Distill large foundational models into smaller, domain-specific models for deployment",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/autodistill/autodistill",
-    install_requires=install_requires,
+    install_requires=[
+        "opencv-python>=4.6.0",
+        "supervision",
+        "tqdm",
+        "Pillow>=7.1.2",
+        "PyYAML>=5.3.1"
+    ],
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel", "mkdocs-material", "mkdocs"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

