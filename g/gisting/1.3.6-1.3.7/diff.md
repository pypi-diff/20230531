# Comparing `tmp/gisting-1.3.6.tar.gz` & `tmp/gisting-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gisting-1.3.6.tar", last modified: Tue May 30 22:18:16 2023, max compression
+gzip compressed data, was "gisting-1.3.7.tar", last modified: Tue May 30 22:23:32 2023, max compression
```

## Comparing `gisting-1.3.6.tar` & `gisting-1.3.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-05-30 22:18:16.392643 gisting-1.3.6/
--rw-r--r--   0 owaiszahid   (501) staff       (20)      302 2023-05-30 22:18:16.392498 gisting-1.3.6/PKG-INFO
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-05-30 22:18:16.383374 gisting-1.3.6/gisting/
--rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-05-30 22:01:12.000000 gisting-1.3.6/gisting/__init__.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-05-30 22:18:16.391786 gisting-1.3.6/gisting/src/
--rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-05-30 21:32:24.000000 gisting-1.3.6/gisting/src/__init__.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    11076 2023-05-30 21:32:24.000000 gisting-1.3.6/gisting/src/arguments.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     3462 2023-05-30 21:32:24.000000 gisting-1.3.6/gisting/src/benchmarking.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     8737 2023-05-30 21:32:24.000000 gisting-1.3.6/gisting/src/compress.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-05-30 22:18:16.392260 gisting-1.3.6/gisting/src/data/
--rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-05-30 21:32:24.000000 gisting-1.3.6/gisting/src/data/__init__.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     8550 2023-05-30 21:32:24.000000 gisting-1.3.6/gisting/src/data/gist.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)      554 2023-05-30 21:32:24.000000 gisting-1.3.6/gisting/src/data/utils.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    21595 2023-05-30 21:32:24.000000 gisting-1.3.6/gisting/src/generation_utils.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     4748 2023-05-30 21:32:24.000000 gisting-1.3.6/gisting/src/gist_caching.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    34287 2023-05-30 21:32:24.000000 gisting-1.3.6/gisting/src/gist_llama.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    41427 2023-05-30 21:32:24.000000 gisting-1.3.6/gisting/src/gist_t5.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     2954 2023-05-30 21:32:24.000000 gisting-1.3.6/gisting/src/integrations.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     4277 2023-05-30 21:32:24.000000 gisting-1.3.6/gisting/src/metrics.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    13819 2023-05-30 21:32:24.000000 gisting-1.3.6/gisting/src/train.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    52559 2023-05-30 21:32:24.000000 gisting-1.3.6/gisting/src/trainer_seq2seq.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)      426 2023-05-30 21:32:24.000000 gisting-1.3.6/gisting/src/utils.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     7880 2023-05-30 21:32:24.000000 gisting-1.3.6/gisting/src/weight_diff.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-05-30 22:18:16.383834 gisting-1.3.6/gisting.egg-info/
--rw-r--r--   0 owaiszahid   (501) staff       (20)      302 2023-05-30 22:18:16.000000 gisting-1.3.6/gisting.egg-info/PKG-INFO
--rw-r--r--   0 owaiszahid   (501) staff       (20)      593 2023-05-30 22:18:16.000000 gisting-1.3.6/gisting.egg-info/SOURCES.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)        1 2023-05-30 22:18:16.000000 gisting-1.3.6/gisting.egg-info/dependency_links.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)       37 2023-05-30 22:18:16.000000 gisting-1.3.6/gisting.egg-info/top_level.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)       38 2023-05-30 22:18:16.392693 gisting-1.3.6/setup.cfg
--rw-r--r--   0 owaiszahid   (501) staff       (20)      516 2023-05-30 22:10:05.000000 gisting-1.3.6/setup.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-05-30 22:23:32.003496 gisting-1.3.7/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      302 2023-05-30 22:23:32.003379 gisting-1.3.7/PKG-INFO
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-05-30 22:23:31.999603 gisting-1.3.7/gisting/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       10 2023-05-30 22:22:42.000000 gisting-1.3.7/gisting/__init__.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-05-30 22:23:32.002756 gisting-1.3.7/gisting/src/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-05-30 21:32:24.000000 gisting-1.3.7/gisting/src/__init__.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    11076 2023-05-30 21:32:24.000000 gisting-1.3.7/gisting/src/arguments.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     3462 2023-05-30 21:32:24.000000 gisting-1.3.7/gisting/src/benchmarking.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     8737 2023-05-30 21:32:24.000000 gisting-1.3.7/gisting/src/compress.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-05-30 22:23:32.003195 gisting-1.3.7/gisting/src/data/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-05-30 21:32:24.000000 gisting-1.3.7/gisting/src/data/__init__.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     8550 2023-05-30 21:32:24.000000 gisting-1.3.7/gisting/src/data/gist.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      554 2023-05-30 21:32:24.000000 gisting-1.3.7/gisting/src/data/utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    21595 2023-05-30 21:32:24.000000 gisting-1.3.7/gisting/src/generation_utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     4748 2023-05-30 21:32:24.000000 gisting-1.3.7/gisting/src/gist_caching.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    34287 2023-05-30 21:32:24.000000 gisting-1.3.7/gisting/src/gist_llama.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    41427 2023-05-30 21:32:24.000000 gisting-1.3.7/gisting/src/gist_t5.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     2954 2023-05-30 21:32:24.000000 gisting-1.3.7/gisting/src/integrations.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     4277 2023-05-30 21:32:24.000000 gisting-1.3.7/gisting/src/metrics.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    13819 2023-05-30 21:32:24.000000 gisting-1.3.7/gisting/src/train.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    52559 2023-05-30 21:32:24.000000 gisting-1.3.7/gisting/src/trainer_seq2seq.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      426 2023-05-30 21:32:24.000000 gisting-1.3.7/gisting/src/utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     7880 2023-05-30 21:32:24.000000 gisting-1.3.7/gisting/src/weight_diff.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-05-30 22:23:32.000130 gisting-1.3.7/gisting.egg-info/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      302 2023-05-30 22:23:31.000000 gisting-1.3.7/gisting.egg-info/PKG-INFO
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      593 2023-05-30 22:23:31.000000 gisting-1.3.7/gisting.egg-info/SOURCES.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        1 2023-05-30 22:23:31.000000 gisting-1.3.7/gisting.egg-info/dependency_links.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       37 2023-05-30 22:23:31.000000 gisting-1.3.7/gisting.egg-info/top_level.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       38 2023-05-30 22:23:32.003536 gisting-1.3.7/setup.cfg
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      516 2023-05-30 22:23:17.000000 gisting-1.3.7/setup.py
```

### Comparing `gisting-1.3.6/gisting/src/arguments.py` & `gisting-1.3.7/gisting/src/arguments.py`

 * *Files identical despite different names*

### Comparing `gisting-1.3.6/gisting/src/benchmarking.py` & `gisting-1.3.7/gisting/src/benchmarking.py`

 * *Files identical despite different names*

### Comparing `gisting-1.3.6/gisting/src/compress.py` & `gisting-1.3.7/gisting/src/compress.py`

 * *Files identical despite different names*

### Comparing `gisting-1.3.6/gisting/src/data/gist.py` & `gisting-1.3.7/gisting/src/data/gist.py`

 * *Files identical despite different names*

### Comparing `gisting-1.3.6/gisting/src/data/utils.py` & `gisting-1.3.7/gisting/src/data/utils.py`

 * *Files identical despite different names*

### Comparing `gisting-1.3.6/gisting/src/generation_utils.py` & `gisting-1.3.7/gisting/src/generation_utils.py`

 * *Files identical despite different names*

### Comparing `gisting-1.3.6/gisting/src/gist_caching.py` & `gisting-1.3.7/gisting/src/gist_caching.py`

 * *Files identical despite different names*

### Comparing `gisting-1.3.6/gisting/src/gist_llama.py` & `gisting-1.3.7/gisting/src/gist_llama.py`

 * *Files identical despite different names*

### Comparing `gisting-1.3.6/gisting/src/gist_t5.py` & `gisting-1.3.7/gisting/src/gist_t5.py`

 * *Files identical despite different names*

### Comparing `gisting-1.3.6/gisting/src/integrations.py` & `gisting-1.3.7/gisting/src/integrations.py`

 * *Files identical despite different names*

### Comparing `gisting-1.3.6/gisting/src/metrics.py` & `gisting-1.3.7/gisting/src/metrics.py`

 * *Files identical despite different names*

### Comparing `gisting-1.3.6/gisting/src/train.py` & `gisting-1.3.7/gisting/src/train.py`

 * *Files identical despite different names*

### Comparing `gisting-1.3.6/gisting/src/trainer_seq2seq.py` & `gisting-1.3.7/gisting/src/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `gisting-1.3.6/gisting/src/weight_diff.py` & `gisting-1.3.7/gisting/src/weight_diff.py`

 * *Files identical despite different names*

### Comparing `gisting-1.3.6/gisting.egg-info/SOURCES.txt` & `gisting-1.3.7/gisting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gisting-1.3.6/setup.py` & `gisting-1.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name = "gisting",
-    version = "1.3.6",
+    version = "1.3.7",
     packages=['gisting','gisting/src','gisting/src/data'],
     include_package_data=True,
     author="Owais Zahid",
     author_email="owais.zahid@mail.utoronto.ca",
     scripts=[],
     description="A pip module for the Gisting Repo by Jesse Mu",
     url = "https://github.com/jayelm/gisting",
```

