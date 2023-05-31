# Comparing `tmp/sprttandem-0.1.0.tar.gz` & `tmp/sprttandem-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprttandem-0.1.0.tar", last modified: Wed May 31 04:42:17 2023, max compression
+gzip compressed data, was "sprttandem-0.1.1.tar", last modified: Wed May 31 04:49:30 2023, max compression
```

## Comparing `sprttandem-0.1.0.tar` & `sprttandem-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 04:42:17.184844 sprttandem-0.1.0/
--rw-r--r--   0 afe       (1000) afe       (1000)     1095 2023-05-01 05:13:22.000000 sprttandem-0.1.0/LICENSE
--rw-rw-r--   0 afe       (1000) afe       (1000)      545 2023-05-31 04:42:17.184844 sprttandem-0.1.0/PKG-INFO
--rw-r--r--   0 afe       (1000) afe       (1000)    15643 2023-05-31 03:32:21.000000 sprttandem-0.1.0/README.md
--rw-rw-r--   0 afe       (1000) afe       (1000)       38 2023-05-31 04:42:17.184844 sprttandem-0.1.0/setup.cfg
--rw-r--r--   0 afe       (1000) afe       (1000)      759 2023-05-31 04:39:45.000000 sprttandem-0.1.0/setup.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 04:42:17.184844 sprttandem-0.1.0/sprttandem/
--rw-r--r--   0 afe       (1000) afe       (1000)      344 2023-05-31 04:01:53.000000 sprttandem-0.1.0/sprttandem/__init__.py
--rwxr--r--   0 afe       (1000) afe       (1000)     2843 2023-05-26 23:56:19.000000 sprttandem-0.1.0/sprttandem/sprt_tandem_main.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 04:42:17.184844 sprttandem-0.1.0/sprttandem.egg-info/
--rw-rw-r--   0 afe       (1000) afe       (1000)      545 2023-05-31 04:42:17.000000 sprttandem-0.1.0/sprttandem.egg-info/PKG-INFO
--rw-rw-r--   0 afe       (1000) afe       (1000)      249 2023-05-31 04:42:17.000000 sprttandem-0.1.0/sprttandem.egg-info/SOURCES.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)        1 2023-05-31 04:42:17.000000 sprttandem-0.1.0/sprttandem.egg-info/dependency_links.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)       23 2023-05-31 04:42:17.000000 sprttandem-0.1.0/sprttandem.egg-info/requires.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)       11 2023-05-31 04:42:17.000000 sprttandem-0.1.0/sprttandem.egg-info/top_level.txt
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 04:49:30.340216 sprttandem-0.1.1/
+-rw-r--r--   0 afe       (1000) afe       (1000)     1095 2023-05-01 05:13:22.000000 sprttandem-0.1.1/LICENSE
+-rw-rw-r--   0 afe       (1000) afe       (1000)      545 2023-05-31 04:49:30.340216 sprttandem-0.1.1/PKG-INFO
+-rw-r--r--   0 afe       (1000) afe       (1000)    15643 2023-05-31 03:32:21.000000 sprttandem-0.1.1/README.md
+-rw-rw-r--   0 afe       (1000) afe       (1000)       38 2023-05-31 04:49:30.340216 sprttandem-0.1.1/setup.cfg
+-rw-r--r--   0 afe       (1000) afe       (1000)      759 2023-05-31 04:48:48.000000 sprttandem-0.1.1/setup.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 04:49:30.340216 sprttandem-0.1.1/sprttandem/
+-rw-r--r--   0 afe       (1000) afe       (1000)      364 2023-05-31 04:47:52.000000 sprttandem-0.1.1/sprttandem/__init__.py
+-rwxr--r--   0 afe       (1000) afe       (1000)     2843 2023-05-26 23:56:19.000000 sprttandem-0.1.1/sprttandem/sprt_tandem_main.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 04:49:30.340216 sprttandem-0.1.1/sprttandem.egg-info/
+-rw-rw-r--   0 afe       (1000) afe       (1000)      545 2023-05-31 04:49:30.000000 sprttandem-0.1.1/sprttandem.egg-info/PKG-INFO
+-rw-rw-r--   0 afe       (1000) afe       (1000)      249 2023-05-31 04:49:30.000000 sprttandem-0.1.1/sprttandem.egg-info/SOURCES.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)        1 2023-05-31 04:49:30.000000 sprttandem-0.1.1/sprttandem.egg-info/dependency_links.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)       23 2023-05-31 04:49:30.000000 sprttandem-0.1.1/sprttandem.egg-info/requires.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)       11 2023-05-31 04:49:30.000000 sprttandem-0.1.1/sprttandem.egg-info/top_level.txt
```

### Comparing `sprttandem-0.1.0/LICENSE` & `sprttandem-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sprttandem-0.1.0/PKG-INFO` & `sprttandem-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprttandem
-Version: 0.1.0
+Version: 0.1.1
 Summary: SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize speed and accuracy of early-classification.
 Home-page: https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch
 Author: Akinori F. Ebihara
 Author-email: aebihara@nec.com
 License: MIT
 Keywords: Sequential Probability Ratio Testlikelihood ratio,density ratio estimation,early classification,artificial intelligence,machine learning
 Platform: UNKNOWN
```

### Comparing `sprttandem-0.1.0/README.md` & `sprttandem-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sprttandem-0.1.0/setup.py` & `sprttandem-0.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sprttandem",
-    version="0.1.0",
+    version="0.1.1",
     license="MIT",
     description="SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize speed and accuracy of early-classification.",
     author="Akinori F. Ebihara",
     author_email="aebihara@nec.com",
     packages=find_packages(),
     include_package_data=True,
     url="https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch",
```

### Comparing `sprttandem-0.1.0/sprttandem/sprt_tandem_main.py` & `sprttandem-0.1.1/sprttandem/sprt_tandem_main.py`

 * *Files identical despite different names*

### Comparing `sprttandem-0.1.0/sprttandem.egg-info/PKG-INFO` & `sprttandem-0.1.1/sprttandem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprttandem
-Version: 0.1.0
+Version: 0.1.1
 Summary: SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize speed and accuracy of early-classification.
 Home-page: https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch
 Author: Akinori F. Ebihara
 Author-email: aebihara@nec.com
 License: MIT
 Keywords: Sequential Probability Ratio Testlikelihood ratio,density ratio estimation,early classification,artificial intelligence,machine learning
 Platform: UNKNOWN
```

