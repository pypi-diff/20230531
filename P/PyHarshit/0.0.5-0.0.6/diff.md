# Comparing `tmp/PyHarshit-0.0.5.tar.gz` & `tmp/PyHarshit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyHarshit-0.0.5.tar", last modified: Tue May  9 19:15:03 2023, max compression
+gzip compressed data, was "PyHarshit-0.0.6.tar", last modified: Wed May 31 08:41:37 2023, max compression
```

## Comparing `PyHarshit-0.0.5.tar` & `PyHarshit-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,29 @@
-drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-09 19:15:03.618407 PyHarshit-0.0.5/
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      669 2023-05-09 19:15:03.618407 PyHarshit-0.0.5/PKG-INFO
-drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-09 19:15:03.614407 PyHarshit-0.0.5/PyHarshit/
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-05-09 19:13:45.000000 PyHarshit-0.0.5/PyHarshit/__init__.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      173 2023-05-09 19:13:45.000000 PyHarshit-0.0.5/PyHarshit/anim.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       19 2023-05-09 19:13:45.000000 PyHarshit-0.0.5/PyHarshit/boolset.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      106 2023-05-09 19:13:45.000000 PyHarshit-0.0.5/PyHarshit/charset.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      313 2023-05-09 19:13:45.000000 PyHarshit-0.0.5/PyHarshit/maths.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      305 2023-05-09 19:13:45.000000 PyHarshit-0.0.5/PyHarshit/tools.py
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      579 2023-05-09 19:13:45.000000 PyHarshit-0.0.5/PyHarshit/utils.py
-drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-09 19:15:03.618407 PyHarshit-0.0.5/PyHarshit.egg-info/
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      669 2023-05-09 19:15:03.000000 PyHarshit-0.0.5/PyHarshit.egg-info/PKG-INFO
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      321 2023-05-09 19:15:03.000000 PyHarshit-0.0.5/PyHarshit.egg-info/SOURCES.txt
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-05-09 19:15:03.000000 PyHarshit-0.0.5/PyHarshit.egg-info/dependency_links.txt
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        5 2023-05-09 19:15:03.000000 PyHarshit-0.0.5/PyHarshit.egg-info/requires.txt
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       10 2023-05-09 19:15:03.000000 PyHarshit-0.0.5/PyHarshit.egg-info/top_level.txt
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      455 2023-05-09 19:13:45.000000 PyHarshit-0.0.5/README.md
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       38 2023-05-09 19:15:03.618407 PyHarshit-0.0.5/setup.cfg
--rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      545 2023-05-09 19:13:45.000000 PyHarshit-0.0.5/setup.py
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-31 08:41:37.174084 PyHarshit-0.0.6/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      778 2023-05-31 08:41:37.174084 PyHarshit-0.0.6/PKG-INFO
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-31 08:41:37.170084 PyHarshit-0.0.6/PyHarshit/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/__init__.py
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-31 08:41:37.170084 PyHarshit-0.0.6/PyHarshit/tg/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)    12360 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tg/FasterTg.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tg/__init__.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     3009 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tg/extractor.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     4125 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tg/tgControl.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     1354 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tg/tgFunctions.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      478 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tg/tools.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)     2761 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tg/uploader.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      174 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tg/utils.py
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-31 08:41:37.174084 PyHarshit-0.0.6/PyHarshit/tools/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tools/__init__.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      173 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tools/anim.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       19 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tools/boolset.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      106 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tools/charset.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      313 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tools/maths.py
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      887 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/PyHarshit/tools/utils.py
+drwxrwxr-x   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        0 2023-05-31 08:41:37.170084 PyHarshit-0.0.6/PyHarshit.egg-info/
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      778 2023-05-31 08:41:37.000000 PyHarshit-0.0.6/PyHarshit.egg-info/PKG-INFO
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      559 2023-05-31 08:41:37.000000 PyHarshit-0.0.6/PyHarshit.egg-info/SOURCES.txt
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)        1 2023-05-31 08:41:37.000000 PyHarshit-0.0.6/PyHarshit.egg-info/dependency_links.txt
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      103 2023-05-31 08:41:37.000000 PyHarshit-0.0.6/PyHarshit.egg-info/requires.txt
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       10 2023-05-31 08:41:37.000000 PyHarshit-0.0.6/PyHarshit.egg-info/top_level.txt
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      564 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/README.md
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)       38 2023-05-31 08:41:37.174084 PyHarshit-0.0.6/setup.cfg
+-rw-rw-r--   0 Pyrogrammers  (1000) Pyrogrammers  (1000)      545 2023-05-31 08:41:03.000000 PyHarshit-0.0.6/setup.py
```

### Comparing `PyHarshit-0.0.5/setup.py` & `PyHarshit-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     page_description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="PyHarshit",
-    version="0.0.5",
+    version="0.0.6",
     author="Harshit Shrivastav",
     author_email="itsharshit@yandex.com",
     description="Utlity file for my codes",
     long_description=page_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=requirements,
```

