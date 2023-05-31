# Comparing `tmp/discocrash.py-0.1.0.tar.gz` & `tmp/discocrash.py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discocrash.py-0.1.0.tar", last modified: Wed May 31 21:18:44 2023, max compression
+gzip compressed data, was "discocrash.py-0.1.1.tar", last modified: Wed May 31 21:53:30 2023, max compression
```

## Comparing `discocrash.py-0.1.0.tar` & `discocrash.py-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 21:18:44.483646 discocrash.py-0.1.0/
--rw-rw-rw-   0        0        0    35823 2022-12-09 21:27:15.000000 discocrash.py-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1293 2023-05-31 21:18:44.482646 discocrash.py-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      764 2022-12-11 18:42:58.000000 discocrash.py-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 21:18:44.391306 discocrash.py-0.1.0/discocrash/
--rw-rw-rw-   0        0        0        0 2022-12-09 21:48:32.000000 discocrash.py-0.1.0/discocrash/__init__.py
--rw-rw-rw-   0        0        0      614 2023-05-23 21:22:23.000000 discocrash.py-0.1.0/discocrash/channels.py
--rw-rw-rw-   0        0        0      828 2022-12-11 21:33:38.000000 discocrash.py-0.1.0/discocrash/crash.py
--rw-rw-rw-   0        0        0     1910 2023-05-31 21:15:53.000000 discocrash.py-0.1.0/discocrash/loghooks.py
--rw-rw-rw-   0        0        0      565 2022-12-11 18:37:29.000000 discocrash.py-0.1.0/discocrash/members.py
--rw-rw-rw-   0        0        0      609 2022-12-11 18:37:18.000000 discocrash.py-0.1.0/discocrash/perms.py
--rw-rw-rw-   0        0        0      514 2022-12-11 18:37:17.000000 discocrash.py-0.1.0/discocrash/spam.py
-drwxrwxrwx   0        0        0        0 2023-05-31 21:18:44.480667 discocrash.py-0.1.0/discocrash.py.egg-info/
--rw-rw-rw-   0        0        0     1293 2023-05-31 21:18:44.000000 discocrash.py-0.1.0/discocrash.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-05-31 21:18:44.000000 discocrash.py-0.1.0/discocrash.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 21:18:44.000000 discocrash.py-0.1.0/discocrash.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-31 21:18:44.000000 discocrash.py-0.1.0/discocrash.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-31 21:18:44.000000 discocrash.py-0.1.0/discocrash.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 21:18:44.484648 discocrash.py-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      832 2023-05-31 21:08:44.000000 discocrash.py-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 21:53:30.122489 discocrash.py-0.1.1/
+-rw-rw-rw-   0        0        0    35823 2022-12-09 21:27:15.000000 discocrash.py-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1293 2023-05-31 21:53:30.122489 discocrash.py-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      764 2022-12-11 18:42:58.000000 discocrash.py-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 21:53:29.994529 discocrash.py-0.1.1/discocrash/
+-rw-rw-rw-   0        0        0        0 2022-12-09 21:48:32.000000 discocrash.py-0.1.1/discocrash/__init__.py
+-rw-rw-rw-   0        0        0      614 2023-05-23 21:22:23.000000 discocrash.py-0.1.1/discocrash/channels.py
+-rw-rw-rw-   0        0        0      828 2022-12-11 21:33:38.000000 discocrash.py-0.1.1/discocrash/crash.py
+-rw-rw-rw-   0        0        0     1910 2023-05-31 21:15:53.000000 discocrash.py-0.1.1/discocrash/loghooks.py
+-rw-rw-rw-   0        0        0      565 2022-12-11 18:37:29.000000 discocrash.py-0.1.1/discocrash/members.py
+-rw-rw-rw-   0        0        0      609 2022-12-11 18:37:18.000000 discocrash.py-0.1.1/discocrash/perms.py
+-rw-rw-rw-   0        0        0      514 2022-12-11 18:37:17.000000 discocrash.py-0.1.1/discocrash/spam.py
+drwxrwxrwx   0        0        0        0 2023-05-31 21:53:30.114166 discocrash.py-0.1.1/discocrash.py.egg-info/
+-rw-rw-rw-   0        0        0     1293 2023-05-31 21:53:29.000000 discocrash.py-0.1.1/discocrash.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-05-31 21:53:29.000000 discocrash.py-0.1.1/discocrash.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 21:53:29.000000 discocrash.py-0.1.1/discocrash.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-31 21:53:29.000000 discocrash.py-0.1.1/discocrash.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-31 21:53:29.000000 discocrash.py-0.1.1/discocrash.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 21:53:30.122489 discocrash.py-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      832 2023-05-31 21:52:57.000000 discocrash.py-0.1.1/setup.py
```

### Comparing `discocrash.py-0.1.0/LICENSE` & `discocrash.py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discocrash.py-0.1.0/PKG-INFO` & `discocrash.py-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discocrash.py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Module for creating discord crash bots
 Home-page: https://github.com/discocrash-py/discorash.py
 Author: JanekDeveloper
 Author-email: ivanbogynsky@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `discocrash.py-0.1.0/README.md` & `discocrash.py-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `discocrash.py-0.1.0/discocrash/channels.py` & `discocrash.py-0.1.1/discocrash/channels.py`

 * *Files identical despite different names*

### Comparing `discocrash.py-0.1.0/discocrash/crash.py` & `discocrash.py-0.1.1/discocrash/crash.py`

 * *Files identical despite different names*

### Comparing `discocrash.py-0.1.0/discocrash/loghooks.py` & `discocrash.py-0.1.1/discocrash/loghooks.py`

 * *Files identical despite different names*

### Comparing `discocrash.py-0.1.0/discocrash/members.py` & `discocrash.py-0.1.1/discocrash/members.py`

 * *Files identical despite different names*

### Comparing `discocrash.py-0.1.0/discocrash/perms.py` & `discocrash.py-0.1.1/discocrash/perms.py`

 * *Files identical despite different names*

### Comparing `discocrash.py-0.1.0/discocrash/spam.py` & `discocrash.py-0.1.1/discocrash/spam.py`

 * *Files identical despite different names*

### Comparing `discocrash.py-0.1.0/discocrash.py.egg-info/PKG-INFO` & `discocrash.py-0.1.1/discocrash.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discocrash.py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Module for creating discord crash bots
 Home-page: https://github.com/discocrash-py/discorash.py
 Author: JanekDeveloper
 Author-email: ivanbogynsky@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `discocrash.py-0.1.0/setup.py` & `discocrash.py-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
-requirements = ["disnake==1.7.3", "requests>=2"]
+requirements = ["discord==1.7.3", "requests>=2"]
 
 setup(
     name="discocrash.py",
-    version="0.1.0",
+    version="0.1.1",
     author="JanekDeveloper",
     author_email="ivanbogynsky@gmail.com",
     description="Module for creating discord crash bots",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/discocrash-py/discorash.py",
     packages=find_packages(),
```

