# Comparing `tmp/SPRT-TANDEM-0.1.1.tar.gz` & `tmp/SPRT-TANDEM-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPRT-TANDEM-0.1.1.tar", last modified: Wed May 31 05:27:46 2023, max compression
+gzip compressed data, was "SPRT-TANDEM-0.1.2.tar", last modified: Wed May 31 05:33:34 2023, max compression
```

## Comparing `SPRT-TANDEM-0.1.1.tar` & `SPRT-TANDEM-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 05:27:46.612267 SPRT-TANDEM-0.1.1/
--rw-r--r--   0 afe       (1000) afe       (1000)     1095 2023-05-01 05:13:22.000000 SPRT-TANDEM-0.1.1/LICENSE
--rw-rw-r--   0 afe       (1000) afe       (1000)      546 2023-05-31 05:27:46.612267 SPRT-TANDEM-0.1.1/PKG-INFO
--rw-r--r--   0 afe       (1000) afe       (1000)    15643 2023-05-31 03:32:21.000000 SPRT-TANDEM-0.1.1/README.md
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 05:27:46.612267 SPRT-TANDEM-0.1.1/SPRT_TANDEM.egg-info/
--rw-rw-r--   0 afe       (1000) afe       (1000)      546 2023-05-31 05:27:46.000000 SPRT-TANDEM-0.1.1/SPRT_TANDEM.egg-info/PKG-INFO
--rw-rw-r--   0 afe       (1000) afe       (1000)      246 2023-05-31 05:27:46.000000 SPRT-TANDEM-0.1.1/SPRT_TANDEM.egg-info/SOURCES.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)        1 2023-05-31 05:27:46.000000 SPRT-TANDEM-0.1.1/SPRT_TANDEM.egg-info/dependency_links.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)       30 2023-05-31 05:27:46.000000 SPRT-TANDEM-0.1.1/SPRT_TANDEM.egg-info/requires.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)        7 2023-05-31 05:27:46.000000 SPRT-TANDEM-0.1.1/SPRT_TANDEM.egg-info/top_level.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)       38 2023-05-31 05:27:46.612267 SPRT-TANDEM-0.1.1/setup.cfg
--rw-r--r--   0 afe       (1000) afe       (1000)      770 2023-05-31 05:27:37.000000 SPRT-TANDEM-0.1.1/setup.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 05:27:46.612267 SPRT-TANDEM-0.1.1/tandem/
--rw-r--r--   0 afe       (1000) afe       (1000)      356 2023-05-31 05:14:48.000000 SPRT-TANDEM-0.1.1/tandem/__init__.py
--rwxr--r--   0 afe       (1000) afe       (1000)     2822 2023-05-31 05:19:38.000000 SPRT-TANDEM-0.1.1/tandem/sprt_tandem_main.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 05:33:34.579323 SPRT-TANDEM-0.1.2/
+-rw-r--r--   0 afe       (1000) afe       (1000)     1095 2023-05-01 05:13:22.000000 SPRT-TANDEM-0.1.2/LICENSE
+-rw-rw-r--   0 afe       (1000) afe       (1000)    16222 2023-05-31 05:33:34.579323 SPRT-TANDEM-0.1.2/PKG-INFO
+-rw-r--r--   0 afe       (1000) afe       (1000)    15643 2023-05-31 03:32:21.000000 SPRT-TANDEM-0.1.2/README.md
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 05:33:34.579323 SPRT-TANDEM-0.1.2/SPRT_TANDEM.egg-info/
+-rw-rw-r--   0 afe       (1000) afe       (1000)    16222 2023-05-31 05:33:34.000000 SPRT-TANDEM-0.1.2/SPRT_TANDEM.egg-info/PKG-INFO
+-rw-rw-r--   0 afe       (1000) afe       (1000)      246 2023-05-31 05:33:34.000000 SPRT-TANDEM-0.1.2/SPRT_TANDEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)        1 2023-05-31 05:33:34.000000 SPRT-TANDEM-0.1.2/SPRT_TANDEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)       30 2023-05-31 05:33:34.000000 SPRT-TANDEM-0.1.2/SPRT_TANDEM.egg-info/requires.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)        7 2023-05-31 05:33:34.000000 SPRT-TANDEM-0.1.2/SPRT_TANDEM.egg-info/top_level.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)       38 2023-05-31 05:33:34.579323 SPRT-TANDEM-0.1.2/setup.cfg
+-rw-r--r--   0 afe       (1000) afe       (1000)     1063 2023-05-31 05:33:14.000000 SPRT-TANDEM-0.1.2/setup.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 05:33:34.579323 SPRT-TANDEM-0.1.2/tandem/
+-rw-r--r--   0 afe       (1000) afe       (1000)      356 2023-05-31 05:14:48.000000 SPRT-TANDEM-0.1.2/tandem/__init__.py
+-rwxr--r--   0 afe       (1000) afe       (1000)     2822 2023-05-31 05:19:38.000000 SPRT-TANDEM-0.1.2/tandem/sprt_tandem_main.py
```

### Comparing `SPRT-TANDEM-0.1.1/LICENSE` & `SPRT-TANDEM-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.1/README.md` & `SPRT-TANDEM-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.1/setup.py` & `SPRT-TANDEM-0.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 from setuptools import setup, find_packages
+from os import path
+
+# Get the long description from the README file
+with open(
+    path.join(path.abspath(path.dirname(__file__)), "README.md"), encoding="utf-8"
+) as f:
+    long_description = f.read()
 
 setup(
     name="SPRT-TANDEM",
-    version="0.1.1",
+    version="0.1.2",
     license="MIT",
     description="SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize speed and accuracy of early-classification.",
     author="Akinori F. Ebihara",
     author_email="aebihara@nec.com",
     packages=find_packages(),
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch",
     keywords=[
         "Sequential Probability Ratio Test" "likelihood ratio",
         "density ratio estimation",
         "early classification",
         "artificial intelligence",
```

### Comparing `SPRT-TANDEM-0.1.1/tandem/sprt_tandem_main.py` & `SPRT-TANDEM-0.1.2/tandem/sprt_tandem_main.py`

 * *Files identical despite different names*

