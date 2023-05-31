# Comparing `tmp/configwizard-1.0.0.tar.gz` & `tmp/configwizard-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configwizard-1.0.0.tar", last modified: Wed May 31 02:22:34 2023, max compression
+gzip compressed data, was "configwizard-1.0.1.tar", last modified: Wed May 31 02:26:37 2023, max compression
```

## Comparing `configwizard-1.0.0.tar` & `configwizard-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 02:22:34.405939 configwizard-1.0.0/
--rw-rw-rw-   0        0        0     2261 2023-05-31 02:22:34.404940 configwizard-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1749 2023-05-31 02:08:00.000000 configwizard-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 02:22:34.403925 configwizard-1.0.0/configwizard.egg-info/
--rw-rw-rw-   0        0        0     2261 2023-05-31 02:22:34.000000 configwizard-1.0.0/configwizard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-05-31 02:22:34.000000 configwizard-1.0.0/configwizard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 02:22:34.000000 configwizard-1.0.0/configwizard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 02:22:34.000000 configwizard-1.0.0/configwizard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 02:22:34.405939 configwizard-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-05-31 02:20:42.000000 configwizard-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:26:37.397322 configwizard-1.0.1/
+-rw-rw-rw-   0        0        0     2261 2023-05-31 02:26:37.396322 configwizard-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1749 2023-05-31 02:08:00.000000 configwizard-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 02:26:37.395322 configwizard-1.0.1/configwizard.egg-info/
+-rw-rw-rw-   0        0        0     2261 2023-05-31 02:26:37.000000 configwizard-1.0.1/configwizard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-05-31 02:26:37.000000 configwizard-1.0.1/configwizard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 02:26:37.000000 configwizard-1.0.1/configwizard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-31 02:26:37.000000 configwizard-1.0.1/configwizard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 02:26:37.000000 configwizard-1.0.1/configwizard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 02:26:37.397322 configwizard-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      804 2023-05-31 02:25:54.000000 configwizard-1.0.1/setup.py
```

### Comparing `configwizard-1.0.0/PKG-INFO` & `configwizard-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configwizard
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for handling configuration files
 Home-page: https://github.com/LapisPhoenix/Py-Config-Handler
 Author: Lapis Pheonix
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `configwizard-1.0.0/README.md` & `configwizard-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `configwizard-1.0.0/configwizard.egg-info/PKG-INFO` & `configwizard-1.0.1/configwizard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configwizard
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for handling configuration files
 Home-page: https://github.com/LapisPhoenix/Py-Config-Handler
 Author: Lapis Pheonix
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `configwizard-1.0.0/setup.py` & `configwizard-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="configwizard",
-    version="1.0.0",
+    version="1.0.1",
     author="Lapis Pheonix",
     description="A package for handling configuration files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LapisPhoenix/Py-Config-Handler",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.11",
     ],
     python_requires=">=3.11.3",
+    install_requires=["tomli_w"],
 )
```

