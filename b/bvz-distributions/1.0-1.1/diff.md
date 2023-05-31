# Comparing `tmp/bvz_distributions-1.0.tar.gz` & `tmp/bvz_distributions-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bvz_distributions-1.0.tar", last modified: Wed May 31 11:55:07 2023, max compression
+gzip compressed data, was "bvz_distributions-1.1.tar", last modified: Wed May 31 12:01:29 2023, max compression
```

## Comparing `bvz_distributions-1.0.tar` & `bvz_distributions-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gulcesolay   (501) staff       (20)        0 2023-05-31 11:55:07.841169 bvz_distributions-1.0/
--rw-r--r--   0 gulcesolay   (501) staff       (20)      128 2023-05-31 11:55:07.840350 bvz_distributions-1.0/PKG-INFO
-drwxr-xr-x   0 gulcesolay   (501) staff       (20)        0 2023-05-31 11:55:07.834971 bvz_distributions-1.0/bvz_distributions/
--rw-r--r--   0 gulcesolay   (501) staff       (20)     7745 2023-05-31 11:19:43.000000 bvz_distributions-1.0/bvz_distributions/Binomialdistribution.py
--rw-r--r--   0 gulcesolay   (501) staff       (20)     4141 2023-05-31 03:43:56.000000 bvz_distributions-1.0/bvz_distributions/Gaussiandistribution.py
--rw-r--r--   0 gulcesolay   (501) staff       (20)     1109 2023-05-31 03:36:30.000000 bvz_distributions-1.0/bvz_distributions/Generaldistribution.py
--rw-r--r--   0 gulcesolay   (501) staff       (20)       43 2023-05-31 03:33:03.000000 bvz_distributions-1.0/bvz_distributions/__init__.py
-drwxr-xr-x   0 gulcesolay   (501) staff       (20)        0 2023-05-31 11:55:07.839327 bvz_distributions-1.0/bvz_distributions.egg-info/
--rw-r--r--   0 gulcesolay   (501) staff       (20)      128 2023-05-31 11:55:07.000000 bvz_distributions-1.0/bvz_distributions.egg-info/PKG-INFO
--rw-r--r--   0 gulcesolay   (501) staff       (20)      367 2023-05-31 11:55:07.000000 bvz_distributions-1.0/bvz_distributions.egg-info/SOURCES.txt
--rw-r--r--   0 gulcesolay   (501) staff       (20)        1 2023-05-31 11:55:07.000000 bvz_distributions-1.0/bvz_distributions.egg-info/dependency_links.txt
--rw-r--r--   0 gulcesolay   (501) staff       (20)        1 2023-05-31 11:55:07.000000 bvz_distributions-1.0/bvz_distributions.egg-info/not-zip-safe
--rw-r--r--   0 gulcesolay   (501) staff       (20)       18 2023-05-31 11:55:07.000000 bvz_distributions-1.0/bvz_distributions.egg-info/top_level.txt
--rw-r--r--   0 gulcesolay   (501) staff       (20)       38 2023-05-31 11:55:07.841384 bvz_distributions-1.0/setup.cfg
--rw-r--r--   0 gulcesolay   (501) staff       (20)      207 2023-05-31 11:36:08.000000 bvz_distributions-1.0/setup.py
+drwxr-xr-x   0 gulcesolay   (501) staff       (20)        0 2023-05-31 12:01:29.690926 bvz_distributions-1.1/
+-rw-r--r--   0 gulcesolay   (501) staff       (20)      128 2023-05-31 12:01:29.690141 bvz_distributions-1.1/PKG-INFO
+drwxr-xr-x   0 gulcesolay   (501) staff       (20)        0 2023-05-31 12:01:29.684638 bvz_distributions-1.1/bvz_distributions/
+-rw-r--r--   0 gulcesolay   (501) staff       (20)     7745 2023-05-31 11:19:43.000000 bvz_distributions-1.1/bvz_distributions/Binomialdistribution.py
+-rw-r--r--   0 gulcesolay   (501) staff       (20)     4141 2023-05-31 03:43:56.000000 bvz_distributions-1.1/bvz_distributions/Gaussiandistribution.py
+-rw-r--r--   0 gulcesolay   (501) staff       (20)     1109 2023-05-31 03:36:30.000000 bvz_distributions-1.1/bvz_distributions/Generaldistribution.py
+-rw-r--r--   0 gulcesolay   (501) staff       (20)       86 2023-05-31 11:59:59.000000 bvz_distributions-1.1/bvz_distributions/__init__.py
+drwxr-xr-x   0 gulcesolay   (501) staff       (20)        0 2023-05-31 12:01:29.689443 bvz_distributions-1.1/bvz_distributions.egg-info/
+-rw-r--r--   0 gulcesolay   (501) staff       (20)      128 2023-05-31 12:01:29.000000 bvz_distributions-1.1/bvz_distributions.egg-info/PKG-INFO
+-rw-r--r--   0 gulcesolay   (501) staff       (20)      367 2023-05-31 12:01:29.000000 bvz_distributions-1.1/bvz_distributions.egg-info/SOURCES.txt
+-rw-r--r--   0 gulcesolay   (501) staff       (20)        1 2023-05-31 12:01:29.000000 bvz_distributions-1.1/bvz_distributions.egg-info/dependency_links.txt
+-rw-r--r--   0 gulcesolay   (501) staff       (20)        1 2023-05-31 11:55:07.000000 bvz_distributions-1.1/bvz_distributions.egg-info/not-zip-safe
+-rw-r--r--   0 gulcesolay   (501) staff       (20)       18 2023-05-31 12:01:29.000000 bvz_distributions-1.1/bvz_distributions.egg-info/top_level.txt
+-rw-r--r--   0 gulcesolay   (501) staff       (20)       38 2023-05-31 12:01:29.691149 bvz_distributions-1.1/setup.cfg
+-rw-r--r--   0 gulcesolay   (501) staff       (20)      207 2023-05-31 12:00:37.000000 bvz_distributions-1.1/setup.py
```

### Comparing `bvz_distributions-1.0/bvz_distributions/Binomialdistribution.py` & `bvz_distributions-1.1/bvz_distributions/Binomialdistribution.py`

 * *Files identical despite different names*

### Comparing `bvz_distributions-1.0/bvz_distributions/Gaussiandistribution.py` & `bvz_distributions-1.1/bvz_distributions/Gaussiandistribution.py`

 * *Files identical despite different names*

### Comparing `bvz_distributions-1.0/bvz_distributions/Generaldistribution.py` & `bvz_distributions-1.1/bvz_distributions/Generaldistribution.py`

 * *Files identical despite different names*

