# Comparing `tmp/BingImageCreator-0.3.0.tar.gz` & `tmp/BingImageCreator-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BingImageCreator-0.3.0.tar", last modified: Wed May 24 10:02:53 2023, max compression
+gzip compressed data, was "BingImageCreator-0.3.1.tar", last modified: Wed May 31 09:08:00 2023, max compression
```

## Comparing `BingImageCreator-0.3.0.tar` & `BingImageCreator-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:02:53.969367 BingImageCreator-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-24 10:02:24.000000 BingImageCreator-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-24 10:02:53.969367 BingImageCreator-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-24 10:02:24.000000 BingImageCreator-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-24 10:02:53.969367 BingImageCreator-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-24 10:02:24.000000 BingImageCreator-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:02:53.965367 BingImageCreator-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:02:53.965367 BingImageCreator-0.3.0/src/BingImageCreator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-24 10:02:53.000000 BingImageCreator-0.3.0/src/BingImageCreator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-24 10:02:53.000000 BingImageCreator-0.3.0/src/BingImageCreator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 10:02:53.000000 BingImageCreator-0.3.0/src/BingImageCreator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 10:02:53.000000 BingImageCreator-0.3.0/src/BingImageCreator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-24 10:02:53.000000 BingImageCreator-0.3.0/src/BingImageCreator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-05-24 10:02:24.000000 BingImageCreator-0.3.0/src/BingImageCreator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:02:53.965367 BingImageCreator-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-24 10:02:24.000000 BingImageCreator-0.3.0/test/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:08:00.478813 BingImageCreator-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-31 09:07:38.000000 BingImageCreator-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-31 09:08:00.478813 BingImageCreator-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-31 09:07:38.000000 BingImageCreator-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 09:08:00.478813 BingImageCreator-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-31 09:07:38.000000 BingImageCreator-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:08:00.478813 BingImageCreator-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:08:00.478813 BingImageCreator-0.3.1/src/BingImageCreator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-31 09:08:00.000000 BingImageCreator-0.3.1/src/BingImageCreator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-31 09:08:00.000000 BingImageCreator-0.3.1/src/BingImageCreator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:08:00.000000 BingImageCreator-0.3.1/src/BingImageCreator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 09:08:00.000000 BingImageCreator-0.3.1/src/BingImageCreator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 09:08:00.000000 BingImageCreator-0.3.1/src/BingImageCreator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-05-31 09:07:38.000000 BingImageCreator-0.3.1/src/BingImageCreator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:08:00.478813 BingImageCreator-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-31 09:07:38.000000 BingImageCreator-0.3.1/test/test_example.py
```

### Comparing `BingImageCreator-0.3.0/LICENSE` & `BingImageCreator-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.3.0/PKG-INFO` & `BingImageCreator-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.3.0
+Version: 0.3.1
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.3.0/README.md` & `BingImageCreator-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.3.0/setup.py` & `BingImageCreator-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="BingImageCreator",
-    version="0.3.0",
+    version="0.3.1",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="High quality image generation by Microsoft. Reverse engineered API.",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/BingImageCreator",
```

### Comparing `BingImageCreator-0.3.0/src/BingImageCreator.egg-info/PKG-INFO` & `BingImageCreator-0.3.1/src/BingImageCreator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.3.0
+Version: 0.3.1
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.3.0/src/BingImageCreator.py` & `BingImageCreator-0.3.1/src/BingImageCreator.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 
 # Error messages
 error_timeout = "Your request has timed out."
 error_redirect = "Redirect failed"
 error_blocked_prompt = (
     "Your prompt has been blocked by Bing. Try to change any bad words and try again."
 )
+error_being_reviewed_prompt = (
+    "Your prompt is being reviewed by Bing. Try to change any sensitive words and try again."
+)
 error_noresults = "Could not get results"
 error_unsupported_lang = "\nthis language is currently not supported by bing"
 error_bad_images = "Bad images"
 error_no_images = "No images"
 #
 sending_message = "Sending request..."
 wait_message = "Waiting for results..."
@@ -99,14 +102,20 @@
         response = self.session.post(
             url,
             allow_redirects=False,
             data=payload,
             timeout=200,
         )
         # check for content waring message
+        if "this prompt is being reviewed" in response.text.lower():
+            if self.debug_file:
+                self.debug(f"ERROR: {error_being_reviewed_prompt}")
+            raise Exception(
+                error_being_reviewed_prompt,
+            )
         if "this prompt has been blocked" in response.text.lower():
             if self.debug_file:
                 self.debug(f"ERROR: {error_blocked_prompt}")
             raise Exception(
                 error_blocked_prompt,
             )
         if (
```

### Comparing `BingImageCreator-0.3.0/test/test_example.py` & `BingImageCreator-0.3.1/test/test_example.py`

 * *Files identical despite different names*

