# Comparing `tmp/celoMine-0.0.1.tar.gz` & `tmp/celoMine-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\celoMine-0.0.1.tar", last modified: Wed May 31 18:33:07 2023, max compression
+gzip compressed data, was "dist\celoMine-0.0.2.tar", last modified: Wed May 31 20:35:31 2023, max compression
```

## Comparing `celoMine-0.0.1.tar` & `celoMine-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 18:33:07.758643 celoMine-0.0.1/
--rw-rw-rw-   0        0        0    35820 2023-05-31 18:08:15.000000 celoMine-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      518 2023-05-31 18:33:07.757653 celoMine-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2362 2023-05-31 18:08:15.000000 celoMine-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 18:33:07.741642 celoMine-0.0.1/celoMine/
--rw-rw-rw-   0        0        0     5377 2023-05-31 18:08:15.000000 celoMine-0.0.1/celoMine/PredictivePR.py
--rw-rw-rw-   0        0        0       98 2023-05-31 18:08:15.000000 celoMine-0.0.1/celoMine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 18:33:07.754643 celoMine-0.0.1/celoMine.egg-info/
--rw-rw-rw-   0        0        0      518 2023-05-31 18:33:07.000000 celoMine-0.0.1/celoMine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-05-31 18:33:07.000000 celoMine-0.0.1/celoMine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 18:33:07.000000 celoMine-0.0.1/celoMine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 18:33:07.000000 celoMine-0.0.1/celoMine.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-31 18:33:07.000000 celoMine-0.0.1/celoMine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 18:33:07.758643 celoMine-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      916 2023-05-31 18:08:15.000000 celoMine-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 20:35:31.763861 celoMine-0.0.2/
+-rw-rw-rw-   0        0        0    35820 2023-05-31 18:08:15.000000 celoMine-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2925 2023-05-31 20:35:31.761861 celoMine-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2362 2023-05-31 18:08:15.000000 celoMine-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 20:35:31.748860 celoMine-0.0.2/celoMine/
+-rw-rw-rw-   0        0        0     5377 2023-05-31 18:08:15.000000 celoMine-0.0.2/celoMine/PredictivePR.py
+-rw-rw-rw-   0        0        0       98 2023-05-31 18:08:15.000000 celoMine-0.0.2/celoMine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 20:35:31.759860 celoMine-0.0.2/celoMine.egg-info/
+-rw-rw-rw-   0        0        0     2925 2023-05-31 20:35:31.000000 celoMine-0.0.2/celoMine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-05-31 20:35:31.000000 celoMine-0.0.2/celoMine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 20:35:31.000000 celoMine-0.0.2/celoMine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 20:35:31.000000 celoMine-0.0.2/celoMine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-31 20:35:31.000000 celoMine-0.0.2/celoMine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 20:35:31.763861 celoMine-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1016 2023-05-31 20:33:51.000000 celoMine-0.0.2/setup.py
```

### Comparing `celoMine-0.0.1/LICENSE` & `celoMine-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `celoMine-0.0.1/README.md` & `celoMine-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `celoMine-0.0.1/celoMine/PredictivePR.py` & `celoMine-0.0.2/celoMine/PredictivePR.py`

 * *Files identical despite different names*

