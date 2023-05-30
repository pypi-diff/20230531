# Comparing `tmp/dgopy-0.0.2.tar.gz` & `tmp/dgopy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgopy-0.0.2.tar", last modified: Tue May 30 09:02:45 2023, max compression
+gzip compressed data, was "dgopy-0.0.3.tar", last modified: Tue May 30 22:56:29 2023, max compression
```

## Comparing `dgopy-0.0.2.tar` & `dgopy-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 09:02:45.270438 dgopy-0.0.2/
--rw-rw-rw-   0        0        0      383 2023-05-30 09:02:45.270438 dgopy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-04-19 04:39:01.000000 dgopy-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 09:02:45.262753 dgopy-0.0.2/dgopy/
--rw-rw-rw-   0        0        0      638 2023-05-30 09:01:53.000000 dgopy-0.0.2/dgopy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:02:45.270438 dgopy-0.0.2/dgopy.egg-info/
--rw-rw-rw-   0        0        0      383 2023-05-30 09:02:45.000000 dgopy-0.0.2/dgopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-05-30 09:02:45.000000 dgopy-0.0.2/dgopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 09:02:45.000000 dgopy-0.0.2/dgopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-30 09:02:45.000000 dgopy-0.0.2/dgopy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 09:02:45.271839 dgopy-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      651 2023-05-30 09:02:42.000000 dgopy-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 22:56:29.960124 dgopy-0.0.3/
+-rw-rw-rw-   0        0        0      383 2023-05-30 22:56:29.960124 dgopy-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-04-19 04:39:01.000000 dgopy-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 22:56:29.956333 dgopy-0.0.3/dgopy/
+-rw-rw-rw-   0        0        0     1049 2023-05-30 22:54:28.000000 dgopy-0.0.3/dgopy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 22:56:29.959116 dgopy-0.0.3/dgopy.egg-info/
+-rw-rw-rw-   0        0        0      383 2023-05-30 22:56:29.000000 dgopy-0.0.3/dgopy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-05-30 22:56:29.000000 dgopy-0.0.3/dgopy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 22:56:29.000000 dgopy-0.0.3/dgopy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-30 22:56:29.000000 dgopy-0.0.3/dgopy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 22:56:29.960124 dgopy-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      651 2023-05-30 22:54:45.000000 dgopy-0.0.3/setup.py
```

### Comparing `dgopy-0.0.2/setup.py` & `dgopy-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'DGo Python'
 LONG_DESCRIPTION = 'DGo pilot framework data input'
 
 setup(
     name="dgopy",
     version=VERSION,
     description=DESCRIPTION,
```

