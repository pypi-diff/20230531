# Comparing `tmp/ippython-0.0.1.tar.gz` & `tmp/ippython-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ippython-0.0.1.tar", last modified: Wed May 31 10:17:25 2023, max compression
+gzip compressed data, was "ippython-0.0.2.tar", last modified: Wed May 31 10:30:35 2023, max compression
```

## Comparing `ippython-0.0.1.tar` & `ippython-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 10:17:25.099080 ippython-0.0.1/
--rw-rw-rw-   0        0        0      499 2023-05-31 10:17:25.096425 ippython-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-31 10:17:25.088175 ippython-0.0.1/ippython/
--rw-rw-rw-   0        0        0       53 2023-05-31 10:06:00.000000 ippython-0.0.1/ippython/__init__.py
--rw-rw-rw-   0        0        0      416 2023-05-31 10:04:30.000000 ippython-0.0.1/ippython/ip.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:17:25.094438 ippython-0.0.1/ippython.egg-info/
--rw-rw-rw-   0        0        0      499 2023-05-31 10:17:24.000000 ippython-0.0.1/ippython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-05-31 10:17:24.000000 ippython-0.0.1/ippython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 10:17:24.000000 ippython-0.0.1/ippython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-31 10:17:24.000000 ippython-0.0.1/ippython.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-31 10:17:24.000000 ippython-0.0.1/ippython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 10:17:25.099599 ippython-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      653 2023-05-31 10:15:42.000000 ippython-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:30:35.285223 ippython-0.0.2/
+-rw-rw-rw-   0        0        0      499 2023-05-31 10:30:35.283538 ippython-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-31 10:30:35.172906 ippython-0.0.2/ippython/
+-rw-rw-rw-   0        0        0       59 2023-05-31 10:28:28.000000 ippython-0.0.2/ippython/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-05-31 10:04:30.000000 ippython-0.0.2/ippython/ippython.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:30:35.281717 ippython-0.0.2/ippython.egg-info/
+-rw-rw-rw-   0        0        0      499 2023-05-31 10:30:35.000000 ippython-0.0.2/ippython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-05-31 10:30:35.000000 ippython-0.0.2/ippython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 10:30:35.000000 ippython-0.0.2/ippython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-31 10:30:35.000000 ippython-0.0.2/ippython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-31 10:30:35.000000 ippython-0.0.2/ippython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 10:30:35.285223 ippython-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      653 2023-05-31 10:30:06.000000 ippython-0.0.2/setup.py
```

### Comparing `ippython-0.0.1/setup.py` & `ippython-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A package that provides functions to retrieve IP geolocation information.'
 
 # Setting up
 setup(
     name="ippython",
     version=VERSION,
     author="Aneko",
```

