# Comparing `tmp/openwillis-1.0.tar.gz` & `tmp/openwillis-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openwillis-1.0.tar", last modified: Thu Apr 13 19:13:56 2023, max compression
+gzip compressed data, was "openwillis-1.1.tar", last modified: Wed May 31 14:59:07 2023, max compression
```

## Comparing `openwillis-1.0.tar` & `openwillis-1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.121919 openwillis-1.0/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    13641 2023-04-13 19:13:26.000000 openwillis-1.0/LICENSE.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      205 2023-04-13 19:13:26.000000 openwillis-1.0/MANIFEST.in
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1113 2023-04-13 19:13:56.121919 openwillis-1.0/PKG-INFO
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      814 2023-04-13 19:13:26.000000 openwillis-1.0/README.md
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      227 2023-04-13 19:13:26.000000 openwillis-1.0/RELEASE.md
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.111919 openwillis-1.0/openwillis/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      469 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/__init__.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.121919 openwillis-1.0/openwillis/features/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/__init__.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      373 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/api.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.121919 openwillis-1.0/openwillis/features/audio/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      103 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/audio/__init__.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    15855 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/audio/acoustic.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.121919 openwillis-1.0/openwillis/features/audio/config/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      706 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/audio/config/acoustic.json
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.121919 openwillis-1.0/openwillis/features/speech/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      346 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/speech/__init__.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     2388 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/speech/aws_transcribe.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.121919 openwillis-1.0/openwillis/features/speech/config/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1593 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/speech/config/speech.json
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     6061 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/speech/speech_attribute.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     7234 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/speech/speech_separation.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     9092 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/speech/speech_transcribe.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    30695 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/speech/util.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.121919 openwillis-1.0/openwillis/features/video/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      227 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/video/__init__.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.121919 openwillis-1.0/openwillis/features/video/config/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      185 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/video/config/facial.json
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    16067 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/video/face_landmark.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)    10471 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/features/video/facial_emotion.py
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      145 2023-04-13 19:13:26.000000 openwillis-1.0/openwillis/usability.py
-drwxrwxr-x   0 ssm-user  (1001) ssm-user  (1001)        0 2023-04-13 19:13:56.121919 openwillis-1.0/openwillis.egg-info/
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)     1113 2023-04-13 19:13:56.000000 openwillis-1.0/openwillis.egg-info/PKG-INFO
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      989 2023-04-13 19:13:56.000000 openwillis-1.0/openwillis.egg-info/SOURCES.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        1 2023-04-13 19:13:56.000000 openwillis-1.0/openwillis.egg-info/dependency_links.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)        1 2023-04-13 19:13:56.000000 openwillis-1.0/openwillis.egg-info/not-zip-safe
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      372 2023-04-13 19:13:56.000000 openwillis-1.0/openwillis.egg-info/requires.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)       11 2023-04-13 19:13:56.000000 openwillis-1.0/openwillis.egg-info/top_level.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      385 2023-04-13 19:13:26.000000 openwillis-1.0/requirements.txt
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)       79 2023-04-13 19:13:56.131919 openwillis-1.0/setup.cfg
--rw-rw-r--   0 ssm-user  (1001) ssm-user  (1001)      934 2023-04-13 19:13:26.000000 openwillis-1.0/setup.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.804891 openwillis-1.1/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    13641 2023-05-31 14:58:24.000000 openwillis-1.1/LICENSE.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      205 2023-05-31 14:58:24.000000 openwillis-1.1/MANIFEST.in
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1131 2023-05-31 14:59:07.804941 openwillis-1.1/PKG-INFO
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      814 2023-05-31 14:58:24.000000 openwillis-1.1/README.md
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      227 2023-05-31 14:58:24.000000 openwillis-1.1/RELEASE.md
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.801864 openwillis-1.1/openwillis/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      469 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/__init__.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.802791 openwillis-1.1/openwillis/features/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      373 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/api.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.803012 openwillis-1.1/openwillis/features/audio/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      103 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/audio/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    15855 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/audio/acoustic.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.803119 openwillis-1.1/openwillis/features/audio/config/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      706 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/audio/config/acoustic.json
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.804080 openwillis-1.1/openwillis/features/speech/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      346 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/speech/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     2388 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/speech/aws_transcribe.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.804209 openwillis-1.1/openwillis/features/speech/config/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1593 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/speech/config/speech.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     6061 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/speech/speech_attribute.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     7234 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/speech/speech_separation.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     9092 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/speech/speech_transcribe.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    30695 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/speech/util.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.804650 openwillis-1.1/openwillis/features/video/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      227 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/video/__init__.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.804763 openwillis-1.1/openwillis/features/video/config/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      185 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/video/config/facial.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    16067 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/video/face_landmark.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    10471 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/features/video/facial_emotion.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      145 2023-05-31 14:58:24.000000 openwillis-1.1/openwillis/usability.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2023-05-31 14:59:07.802599 openwillis-1.1/openwillis.egg-info/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1131 2023-05-31 14:59:07.000000 openwillis-1.1/openwillis.egg-info/PKG-INFO
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      989 2023-05-31 14:59:07.000000 openwillis-1.1/openwillis.egg-info/SOURCES.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2023-05-31 14:59:07.000000 openwillis-1.1/openwillis.egg-info/dependency_links.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2023-05-31 14:59:07.000000 openwillis-1.1/openwillis.egg-info/not-zip-safe
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      372 2023-05-31 14:59:07.000000 openwillis-1.1/openwillis.egg-info/requires.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)       11 2023-05-31 14:59:07.000000 openwillis-1.1/openwillis.egg-info/top_level.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      385 2023-05-31 14:58:24.000000 openwillis-1.1/requirements.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)       79 2023-05-31 14:59:07.805149 openwillis-1.1/setup.cfg
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      932 2023-05-31 14:58:41.000000 openwillis-1.1/setup.py
```

### Comparing `openwillis-1.0/LICENSE.txt` & `openwillis-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openwillis-1.0/PKG-INFO` & `openwillis-1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: openwillis
-Version: 1.0
+Version: 1.1
 Summary: digital health measurement
 Home-page: https://github.com/bklynhlth/openwillis
 Author: bklynhlth
 Author-email: admin@bklynhlth.com
 License: Apache
-Requires-Python: >=3.6.*
+Platform: UNKNOWN
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 Openwillis is a python library for digital measurement of health.
 
 It was developed by Brooklyn Health to establish standardized methods in digital measurement.
 
@@ -19,7 +20,9 @@
 * [Official website](https://www.bklynhlth.com/openwillis)
 * [Documentation](https://github.com/bklynhlth/openwillis/wiki)
 * [Getting started](https://github.com/bklynhlth/openwillis/wiki/1.-Getting-started)
 * [List of functions](https://github.com/bklynhlth/openwillis/wiki/2.-List-of-functions)
 * [Research guidelines](https://github.com/bklynhlth/openwillis/wiki/3.-Research-guidelines)
 
 Please report any issues using the [Issues](https://github.com/bklynhlth/openwillis/issues) tab or get in touch through openwillis@bklynhlth.com.
+
+
```

### Comparing `openwillis-1.0/README.md` & `openwillis-1.1/README.md`

 * *Files identical despite different names*

### Comparing `openwillis-1.0/openwillis/features/audio/acoustic.py` & `openwillis-1.1/openwillis/features/audio/acoustic.py`

 * *Files identical despite different names*

### Comparing `openwillis-1.0/openwillis/features/audio/config/acoustic.json` & `openwillis-1.1/openwillis/features/audio/config/acoustic.json`

 * *Files identical despite different names*

### Comparing `openwillis-1.0/openwillis/features/speech/aws_transcribe.py` & `openwillis-1.1/openwillis/features/speech/aws_transcribe.py`

 * *Files identical despite different names*

### Comparing `openwillis-1.0/openwillis/features/speech/config/speech.json` & `openwillis-1.1/openwillis/features/speech/config/speech.json`

 * *Files identical despite different names*

### Comparing `openwillis-1.0/openwillis/features/speech/speech_attribute.py` & `openwillis-1.1/openwillis/features/speech/speech_attribute.py`

 * *Files identical despite different names*

### Comparing `openwillis-1.0/openwillis/features/speech/speech_separation.py` & `openwillis-1.1/openwillis/features/speech/speech_separation.py`

 * *Files identical despite different names*

### Comparing `openwillis-1.0/openwillis/features/speech/speech_transcribe.py` & `openwillis-1.1/openwillis/features/speech/speech_transcribe.py`

 * *Files identical despite different names*

### Comparing `openwillis-1.0/openwillis/features/speech/util.py` & `openwillis-1.1/openwillis/features/speech/util.py`

 * *Files identical despite different names*

### Comparing `openwillis-1.0/openwillis/features/video/face_landmark.py` & `openwillis-1.1/openwillis/features/video/face_landmark.py`

 * *Files identical despite different names*

### Comparing `openwillis-1.0/openwillis/features/video/facial_emotion.py` & `openwillis-1.1/openwillis/features/video/facial_emotion.py`

 * *Files identical despite different names*

### Comparing `openwillis-1.0/openwillis.egg-info/PKG-INFO` & `openwillis-1.1/openwillis.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: openwillis
-Version: 1.0
+Version: 1.1
 Summary: digital health measurement
 Home-page: https://github.com/bklynhlth/openwillis
 Author: bklynhlth
 Author-email: admin@bklynhlth.com
 License: Apache
-Requires-Python: >=3.6.*
+Platform: UNKNOWN
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 Openwillis is a python library for digital measurement of health.
 
 It was developed by Brooklyn Health to establish standardized methods in digital measurement.
 
@@ -19,7 +20,9 @@
 * [Official website](https://www.bklynhlth.com/openwillis)
 * [Documentation](https://github.com/bklynhlth/openwillis/wiki)
 * [Getting started](https://github.com/bklynhlth/openwillis/wiki/1.-Getting-started)
 * [List of functions](https://github.com/bklynhlth/openwillis/wiki/2.-List-of-functions)
 * [Research guidelines](https://github.com/bklynhlth/openwillis/wiki/3.-Research-guidelines)
 
 Please report any issues using the [Issues](https://github.com/bklynhlth/openwillis/issues) tab or get in touch through openwillis@bklynhlth.com.
+
+
```

### Comparing `openwillis-1.0/openwillis.egg-info/SOURCES.txt` & `openwillis-1.1/openwillis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openwillis-1.0/setup.py` & `openwillis-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fp:
     install_requires = fp.read()
 
 setuptools.setup(name='openwillis',
-                 version='1.0',
+                 version='1.1',
                  description='digital health measurement',
                  long_description=long_description,
                  long_description_content_type="text/markdown",
                  url='https://github.com/bklynhlth/openwillis',
                  author='bklynhlth',
-                 python_requires='>=3.6.*',
+                 python_requires='>=3.6',
                  install_requires=install_requires,
                  author_email='admin@bklynhlth.com',
                  packages=setuptools.find_packages(),
                  include_package_data=True,
                  zip_safe=False,
                  license='Apache'
                 )
```

