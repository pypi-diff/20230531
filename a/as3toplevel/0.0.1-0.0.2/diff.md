# Comparing `tmp/as3toplevel-0.0.1.tar.gz` & `tmp/as3toplevel-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "as3toplevel-0.0.1.tar", last modified: Sat May 27 00:56:41 2023, max compression
+gzip compressed data, was "as3toplevel-0.0.2.tar", last modified: Wed May 31 20:32:03 2023, max compression
```

## Comparing `as3toplevel-0.0.1.tar` & `as3toplevel-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ajdel     (1000) ajdel     (1000)        0 2023-05-27 00:56:41.236838 as3toplevel-0.0.1/
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     1069 2023-05-26 23:44:21.000000 as3toplevel-0.0.1/LICENSE
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       42 2023-05-27 00:52:01.000000 as3toplevel-0.0.1/MANIFEST.in
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     1672 2023-05-27 00:56:41.236838 as3toplevel-0.0.1/PKG-INFO
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     1128 2023-05-26 23:44:21.000000 as3toplevel-0.0.1/README.md
-drwxrwxr-x   0 ajdel     (1000) ajdel     (1000)        0 2023-05-27 00:56:41.236838 as3toplevel-0.0.1/as3toplevel.egg-info/
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     1672 2023-05-27 00:56:41.000000 as3toplevel-0.0.1/as3toplevel.egg-info/PKG-INFO
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)      252 2023-05-27 00:56:41.000000 as3toplevel-0.0.1/as3toplevel.egg-info/SOURCES.txt
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)        1 2023-05-27 00:56:41.000000 as3toplevel-0.0.1/as3toplevel.egg-info/dependency_links.txt
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)        6 2023-05-27 00:56:41.000000 as3toplevel-0.0.1/as3toplevel.egg-info/requires.txt
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       12 2023-05-27 00:56:41.000000 as3toplevel-0.0.1/as3toplevel.egg-info/top_level.txt
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)    26222 2023-05-27 00:54:03.000000 as3toplevel-0.0.1/as3toplevel.py
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       99 2023-05-27 00:14:36.000000 as3toplevel-0.0.1/pyproject.toml
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       73 2023-05-27 00:56:41.236838 as3toplevel-0.0.1/setup.cfg
--rw-rw-r--   0 ajdel     (1000) ajdel     (1000)      868 2023-05-27 00:54:28.000000 as3toplevel-0.0.1/setup.py
+drwxrwxr-x   0 ajdel     (1000) ajdel     (1000)        0 2023-05-31 20:32:03.038374 as3toplevel-0.0.2/
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     1069 2023-05-26 23:44:21.000000 as3toplevel-0.0.2/LICENSE
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       42 2023-05-27 00:52:01.000000 as3toplevel-0.0.2/MANIFEST.in
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     6251 2023-05-31 20:32:03.038374 as3toplevel-0.0.2/PKG-INFO
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     5707 2023-05-31 20:25:51.000000 as3toplevel-0.0.2/README.md
+drwxrwxr-x   0 ajdel     (1000) ajdel     (1000)        0 2023-05-31 20:32:03.038374 as3toplevel-0.0.2/as3toplevel.egg-info/
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)     6251 2023-05-31 20:32:03.000000 as3toplevel-0.0.2/as3toplevel.egg-info/PKG-INFO
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)      252 2023-05-31 20:32:03.000000 as3toplevel-0.0.2/as3toplevel.egg-info/SOURCES.txt
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)        1 2023-05-31 20:32:03.000000 as3toplevel-0.0.2/as3toplevel.egg-info/dependency_links.txt
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)        6 2023-05-31 20:32:03.000000 as3toplevel-0.0.2/as3toplevel.egg-info/requires.txt
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       12 2023-05-31 20:32:03.000000 as3toplevel-0.0.2/as3toplevel.egg-info/top_level.txt
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)    41067 2023-05-31 20:25:22.000000 as3toplevel-0.0.2/as3toplevel.py
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       99 2023-05-27 00:14:36.000000 as3toplevel-0.0.2/pyproject.toml
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)       73 2023-05-31 20:32:03.042374 as3toplevel-0.0.2/setup.cfg
+-rw-rw-r--   0 ajdel     (1000) ajdel     (1000)      868 2023-05-30 22:11:06.000000 as3toplevel-0.0.2/setup.py
```

### Comparing `as3toplevel-0.0.1/LICENSE` & `as3toplevel-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `as3toplevel-0.0.1/setup.py` & `as3toplevel-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as ld:
       long_desc = ld.read()
 
 setup(name="as3toplevel",
-      version="0.0.1",
+      version="0.0.2",
       author="ajdelguidice",
       author_email="ajdelguidice@gmail.com",
       url="https://github.com/ajdelguidice/python-as3toplevel",
       py_modules=["as3toplevel"],
       description="Python implementation of the ActionScript3 toplevel",
       long_description=long_desc,
       long_description_content_type="text/markdown",
```

