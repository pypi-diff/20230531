# Comparing `tmp/sdss-tree-3.1.6.tar.gz` & `tmp/sdss-tree-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sdss-tree-3.1.6.tar", last modified: Mon Mar 27 15:42:16 2023, max compression
+gzip compressed data, was "dist/sdss-tree-3.1.7.tar", last modified: Wed May 31 12:55:26 2023, max compression
```

## Comparing `sdss-tree-3.1.6.tar` & `sdss-tree-3.1.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:42:16.000000 sdss-tree-3.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-03-27 15:42:16.000000 sdss-tree-3.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:42:16.000000 sdss-tree-3.1.6/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    20812 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/bin/setup_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:42:16.000000 sdss-tree-3.1.6/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:42:16.000000 sdss-tree-3.1.6/python/sdss_tree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-03-27 15:42:16.000000 sdss-tree-3.1.6/python/sdss_tree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-27 15:42:16.000000 sdss-tree-3.1.6/python/sdss_tree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 15:42:16.000000 sdss-tree-3.1.6/python/sdss_tree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 15:42:16.000000 sdss-tree-3.1.6/python/sdss_tree.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-27 15:42:16.000000 sdss-tree-3.1.6/python/sdss_tree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-27 15:42:16.000000 sdss-tree-3.1.6/python/sdss_tree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:42:16.000000 sdss-tree-3.1.6/python/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/changelog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:42:16.000000 sdss-tree-3.1.6/python/tree/data/
--rw-r--r--   0 runner    (1001) docker     (123)    22519 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/basework.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/bosswork.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/dr10.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/dr11.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/dr12.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/dr13.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/dr14.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/dr15.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/dr16.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/dr17.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/dr18.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/dr7.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/dr8.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/dr9.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/ipl1.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/ipl2.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/mpl10.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/mpl11.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/mpl3.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/mpl4.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/mpl5.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/mpl6.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/mpl7.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/mpl8.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/mpl9.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    24022 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/sdss5.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/data/sdsswork.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:42:16.000000 sdss-tree-3.1.6/python/tree/etc/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/etc/tree.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:42:16.000000 sdss-tree-3.1.6/python/tree/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/misc/docutree.py
--rw-r--r--   0 runner    (1001) docker     (123)    31512 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/python/tree/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-03-27 15:42:16.000000 sdss-tree-3.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-27 15:42:02.000000 sdss-tree-3.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20812 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/bin/setup_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/sdss_tree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/sdss_tree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/sdss_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/sdss_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/sdss_tree.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/sdss_tree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/sdss_tree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/changelog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/tree/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    22519 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/basework.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/bosswork.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr10.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr11.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr12.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr13.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr14.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr15.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr16.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr17.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr18.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr7.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr8.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr9.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/ipl1.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/ipl2.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/mpl10.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/mpl11.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/mpl3.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/mpl4.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/mpl5.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/mpl6.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/mpl7.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/mpl8.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/mpl9.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    25151 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/sdss5.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/sdsswork.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/tree/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/etc/tree.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/tree/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/misc/docutree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31512 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/setup.py
```

### Comparing `sdss-tree-3.1.6/LICENSE.md` & `sdss-tree-3.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/PKG-INFO` & `sdss-tree-3.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-tree
-Version: 3.1.6
+Version: 3.1.7
 Summary: Control and setup of SDSS tree environment and modules
 Home-page: https://github.com/sdss/tree
 Author: Brian Cherinka
 Author-email: bcherinka@stsci.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/tree
 Project-URL: Documentation, https://sdss-tree.readthedocs.org
```

### Comparing `sdss-tree-3.1.6/README.md` & `sdss-tree-3.1.7/README.md`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/bin/setup_tree.py` & `sdss-tree-3.1.7/bin/setup_tree.py`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/sdss_tree.egg-info/PKG-INFO` & `sdss-tree-3.1.7/python/sdss_tree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-tree
-Version: 3.1.6
+Version: 3.1.7
 Summary: Control and setup of SDSS tree environment and modules
 Home-page: https://github.com/sdss/tree
 Author: Brian Cherinka
 Author-email: bcherinka@stsci.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/tree
 Project-URL: Documentation, https://sdss-tree.readthedocs.org
```

### Comparing `sdss-tree-3.1.6/python/sdss_tree.egg-info/SOURCES.txt` & `sdss-tree-3.1.7/python/sdss_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/sdss_tree.egg-info/requires.txt` & `sdss-tree-3.1.7/python/sdss_tree.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/changelog.py` & `sdss-tree-3.1.7/python/tree/changelog.py`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/basework.cfg` & `sdss-tree-3.1.7/python/tree/data/basework.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/bosswork.cfg` & `sdss-tree-3.1.7/python/tree/data/bosswork.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/dr10.cfg` & `sdss-tree-3.1.7/python/tree/data/dr10.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/dr11.cfg` & `sdss-tree-3.1.7/python/tree/data/dr11.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/dr12.cfg` & `sdss-tree-3.1.7/python/tree/data/dr12.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/dr13.cfg` & `sdss-tree-3.1.7/python/tree/data/dr13.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/dr14.cfg` & `sdss-tree-3.1.7/python/tree/data/dr14.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/dr15.cfg` & `sdss-tree-3.1.7/python/tree/data/dr15.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/dr16.cfg` & `sdss-tree-3.1.7/python/tree/data/dr16.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/dr17.cfg` & `sdss-tree-3.1.7/python/tree/data/dr17.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/dr18.cfg` & `sdss-tree-3.1.7/python/tree/data/dr18.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/dr7.cfg` & `sdss-tree-3.1.7/python/tree/data/dr7.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/dr8.cfg` & `sdss-tree-3.1.7/python/tree/data/dr8.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/dr9.cfg` & `sdss-tree-3.1.7/python/tree/data/dr9.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/ipl1.cfg` & `sdss-tree-3.1.7/python/tree/data/ipl1.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -22,31 +22,41 @@
 APOGEE_REDUX = %(IPL_ROOT)s/spectro/apogee/redux
 
 
 [PATHS]
 # Astra paths
 mwmVisit = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/spectra/visit/@cat_id_groups|/mwmVisit-{v_astra}-{cat_id}@component_default|.fits
 mwmStar = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/spectra/star/@cat_id_groups|/mwmStar-{v_astra}-{cat_id}@component_default|.fits
+
 astraStarASPCAP = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/star/@cat_id_groups|/astraStar-ASPCAP-{v_astra}-{cat_id}@component_default|-{task_id}.fits
 astraStarFERRE = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/star/@cat_id_groups|/astraStar-FERRE-{v_astra}-{cat_id}@component_default|-{task_id}.fits
-astraStarCannon = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/star/@cat_id_groups|/astraStar-Cannon-{v_astra}-{cat_id}@component_default|-{task_id}.fits
+astraStarTheCannon    = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/star/@cat_id_groups|/astraStar-TheCannon-{v_astra}-{cat_id}@component_default|-{task_id}.fits
 astraStarKorg = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/star/@cat_id_groups|/astraStar-Korg-{v_astra}-{cat_id}@component_default|-{task_id}.fits
-astraStarPayne = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/star/@cat_id_groups|/astraStar-Payne-{v_astra}-{cat_id}@component_default|-{task_id}.fits
+astraStarThePayne = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/star/@cat_id_groups|/astraStar-Payne-{v_astra}-{cat_id}@component_default|-{task_id}.fits
 astraStarZetaPayne = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/star/@cat_id_groups|/astraStar-ZetaPayne-{v_astra}-{cat_id}@component_default|-{task_id}.fits
 astraStarSLAM = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/star/@cat_id_groups|/astraStar-SLAM-{v_astra}-{cat_id}@component_default|-{task_id}.fits
-astraStarWD = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/star/@cat_id_groups|/astraStar-WD-{v_astra}-{cat_id}@component_default|-{task_id}.fits
+astraStarSnowWhite = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/star/@cat_id_groups|/astraStar-WD-{v_astra}-{cat_id}@component_default|-{task_id}.fits
+
 astraVisitASPCAP = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/visit/@cat_id_groups|/astraVisit-ASPCAP-{v_astra}-{cat_id}@component_default|-{task_id}.fits
 astraVisitFERRE = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/visit/@cat_id_groups|/astraVisit-FERRE-{v_astra}-{cat_id}@component_default|-{task_id}.fits
-astraVisitCannon = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/visit/@cat_id_groups|/astraVisit-Cannon-{v_astra}-{cat_id}@component_default|-{task_id}.fits
+astraVisitTheCannon = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/visit/@cat_id_groups|/astraVisit-Cannon-{v_astra}-{cat_id}@component_default|-{task_id}.fits
 astraVisitKorg = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/visit/@cat_id_groups|/astraVisit-Korg-{v_astra}-{cat_id}@component_default|-{task_id}.fits
-astraVisitPayne = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/visit/@cat_id_groups|/astraVisit-Payne-{v_astra}-{cat_id}@component_default|-{task_id}.fits
+astraVisitThePayne = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/visit/@cat_id_groups|/astraVisit-Payne-{v_astra}-{cat_id}@component_default|-{task_id}.fits
 astraVisitZetaPayne = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/visit/@cat_id_groups|/astraVisit-ZetaPayne-{v_astra}-{cat_id}@component_default|-{task_id}.fits
 astraVisitSLAM = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/visit/@cat_id_groups|/astraVisit-SLAM-{v_astra}-{cat_id}@component_default|-{task_id}.fits
 astraVisitWD = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/visit/@cat_id_groups|/astraVisit-WD-{v_astra}-{cat_id}@component_default|-{task_id}.fits
 
+astraAllStarAPOGEENet  = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/summary/astraAllStar-ASPOGEENet-{v_astra}-{run2d}-{apred}.fits
+astraAllStarASPCAP     = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/summary/astraAllStar-ASPCAP-{v_astra}-{run2d}-{apred}.fits
+astraAllStarCannon     = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/summary/astraAllStar-Cannon-{v_astra}-{run2d}-{apred}.fits
+astraAllStarClassifier = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/summary/astraAllStar-Classifier-{v_astra}-{run2d}-{apred}.fits
+astraAllStarThePayne   = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/summary/astraAllStar-Payne-{v_astra}-{run2d}-{apred}.fits
+astraAllStarSLAM       = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/summary/astraAllStar-SLAM-{v_astra}-{run2d}-{apred}.fits
+astraAllStarSnowWhite  = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/summary/astraAllStar-SnowWhite-{v_astra}-{run2d}-{apred}.fits
+
 # apogee paths
 allCal = $APOGEE_REDUX/{apred}/allCal.fits
 allExp = $APOGEE_REDUX/{apred}/allExp.fits
 allSci = $APOGEE_REDUX/{apred}/allSci.fits
 apBPM = $APOGEE_REDUX/{apred}/cal/{instrument}/bpm/@apgprefix|BPM-{chip}-{num:0>8}.fits
 apCal = $APOGEE_REDUX/{apred}/{prefix}Cal.fits
 apDark = $APOGEE_REDUX/{apred}/cal/{instrument}/darkcorr/@apgprefix|Dark-{chip}-{num:0>8}.fits
```

### Comparing `sdss-tree-3.1.6/python/tree/data/mpl3.cfg` & `sdss-tree-3.1.7/python/tree/data/mpl3.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/mpl4.cfg` & `sdss-tree-3.1.7/python/tree/data/mpl4.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/mpl7.cfg` & `sdss-tree-3.1.7/python/tree/data/mpl7.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/mpl8.cfg` & `sdss-tree-3.1.7/python/tree/data/mpl8.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/data/sdss5.cfg` & `sdss-tree-3.1.7/python/tree/data/sdss5.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 #
 #
 [DATA]
 name = sdsswork
 DATA_ROOT = %(FILESYSTEM)s/%(name)s/data
 APO_STAGING_DATA = %(DATA_ROOT)s/staging/apo
 LCO_STAGING_DATA = %(DATA_ROOT)s/staging/lco
+AGCAM_DATA_S = %(DATA_ROOT)s/agcam/lco
 ECAM_DATA_N = %(DATA_ROOT)s/ecam/apo
 ECAM_DATA_S = %(DATA_ROOT)s/ecam/lco
 FPS_ENGINEERING = %(DATA_ROOT)s/fps/engineering
 FCAM_DATA_N = %(DATA_ROOT)s/fcam/apo
 FCAM_DATA_S = %(DATA_ROOT)s/fcam/lco
 GCAM_DATA_N = %(DATA_ROOT)s/gcam/apo
 GCAM_DATA_S = %(DATA_ROOT)s/gcam/lco
@@ -37,15 +38,18 @@
 #APO_TELEMETRY = %(DATA_ROOT)s/telemetry/apo
 BOSS_SPECTRO_DATA_N = %(DATA_ROOT)s/boss/spectro/apo
 BOSS_SPECTRO_DATA_S = %(DATA_ROOT)s/boss/spectro/lco
 BOSS_SOS_N = %(DATA_ROOT)s/boss/sos/apo
 BOSS_SOS_S = %(DATA_ROOT)s/boss/sos/lco
 APOGEE_DATA_N=%(DATA_ROOT)s/apogee/apo
 APOGEE_DATA_S=%(DATA_ROOT)s/apogee/lco
-#APOGEE_QUICK=%(DATA_ROOT)s/apogee/spectro/quickred
+APOGEE_QUICK_N=%(DATA_ROOT)s/quickred/apo
+APOGEE_QUICK_S=%(DATA_ROOT)s/quickred/lco
+# APOGEE_QUICK_N=%(DATA_ROOT)s/apogee/quickred/apo
+# APOGEE_QUICK_S=%(DATA_ROOT)s/apogee/quickred/lco
 LVM_DATA_N = %(DATA_ROOT)s/lvm/apo
 LVM_DATA_S = %(DATA_ROOT)s/lvm/lco
 LVM_QUICK_N = %(DATA_ROOT)s/lvm/quick/apo
 LVM_QUICK_S = %(DATA_ROOT)s/lvm/quick/lco
 LVM_DATA_LAB = %(DATA_ROOT)s/lvm/lab
 #
 #
@@ -96,14 +100,16 @@
 [LVM]
 name = sdsswork
 LVM_ROOT = %(FILESYSTEM)s/%(name)s/lvm
 LVM_SANDBOX = %(LVM_ROOT)s/sandbox
 LVM_SPECTRO_REDUX = %(LVM_ROOT)s/spectro/redux
 LVM_SPECTRO_ANALYSIS = %(LVM_ROOT)s/spectro/analysis
 LVM_TARGET = %(LVM_ROOT)s/target
+LVM_CONFIG_DRP = %(LVM_SPECTRO_REDUX)s/{drpver}/configs
+LVM_CONFIG_DAP = %(LVM_SPECTRO_ANALYSIS)s/{drpver}/{dapver}/configs
 #
 #
 #
 [MWM]
 name = sdsswork
 MWM_ROOT = %(FILESYSTEM)s/%(name)s/mwm
 MWM_SANDBOX = %(MWM_ROOT)s/sandbox
@@ -197,16 +203,16 @@
 apogeeObjectAll = $APOGEE_TARGET/apogeeObject_{dr}.fits
 apogeePlate = $APOGEE_TARGET/apogeePlate_{dr}.fits
 apPersist = $APOGEE_REDUX/{apred}/cal/{instrument}/persist/@apgprefix|Persist-{chip}-{num:0>8}.fits
 apPSF = $APOGEE_REDUX/{apred}/cal/{instrument}/psf/@apgprefix|PSF-{chip}-{num:0>8}.fits
 apPSFModel = $APOGEE_REDUX/{apred}/cal/{instrument}/psf/@apgprefix|PSFModel-{chip}-{num:0>8}.fits
 apR = $APOGEE_DATA_N/{mjd}/apR-{chip}-{num:0>8}.apz
 apResponse = $APOGEE_REDUX/{apred}/cal/{instrument}/flux/@apgprefix|Response-{chip}-{num:0>8}.fits
-apStar = $APOGEE_REDUX/{apred}/{telescope}/@healpixgrp|/{healpix}/apStar-{apred}-{telescope}-{obj}.fits
-apStar-1m = $APOGEE_REDUX/{apred}/{apstar}/{telescope}/{field}/@apgprefix|Star-{apred}-{reduction}.fits
+apStar = $APOGEE_REDUX/{apred}/stars/{telescope}/@healpixgrp|/{healpix}/apStar-{apred}-{telescope}-{obj}.fits
+apStar-1m = $APOGEE_REDUX/{apred}/stars/{telescope}/{field}/@apgprefix|Star-{apred}-{reduction}.fits
 apWave = $APOGEE_REDUX/{apred}/cal/{instrument}/wave/@apgprefix|Wave-{chip}-{num:0>8}.fits
 apWaveFPI = $APOGEE_REDUX/{apred}/cal/{instrument}/wave/@apgprefix|WaveFPI-{chip}-{mjd}-{num:0>8}.fits
 cannonStar = $APOGEE_CANNON/{apred}/{cannon}/{field}/cannonStar-{apred}-{obj}.pkl
 cannonStar-1m = $APOGEE_CANNON/{apred}/{cannon}/{field}/cannonStar-{apred}-{reduction}.pkl
 allPlates = $APOGEE_ASPCAP/{apred}/{aspcap}/allPlates-{apred}-{aspcap}.fits
 allStar = $APOGEE_REDUX/{apred}/summary/allStar-{apred}-{telescope}.fits
 allVisit = $APOGEE_REDUX/{apred}/summary/allVisit-{apred}-{telescope}.fits
@@ -269,14 +275,16 @@
 spAllField = $BOSS_SPECTRO_REDUX/{run2d}/spectra/full/@pad_fieldid|@isplate|/{mjd}/spAll-@pad_fieldid|-{mjd}.fits
 spAllLineField = $BOSS_SPECTRO_REDUX/{run2d}/spectra/full/@pad_fieldid|@isplate|/{mjd}/spAllLine-@pad_fieldid|-{mjd}.fits
 #
 # github products
 #
 confSummary = $SDSSCORE_DIR/{obs}/summary_files/@configgrp|/confSummary-{configid}.par
 confSummaryF = $SDSSCORE_DIR/{obs}/summary_files/@configgrp|/confSummaryF-{configid}.par
+confSummary_test = $SDSSCORE_DIR/{obs}/summary_files/@configsubmodule|/@configgrp|/confSummary-{configid}.par
+confSummaryF_test = $SDSSCORE_DIR/{obs}/summary_files/@configsubmodule|/@configgrp|/confSummaryF-{configid}.par
 
 # Astra paths
 mwmVisit = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/spectra/visit/@cat_id_groups|/mwmVisit-{v_astra}-{cat_id}@component_default|.fits
 mwmStar = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/spectra/star/@cat_id_groups|/mwmStar-{v_astra}-{cat_id}@component_default|.fits
 astraStarASPCAP = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/star/@cat_id_groups|/astraStar-ASPCAP-{v_astra}-{cat_id}@component_default|-{task_id}.fits
 astraStarFERRE = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/star/@cat_id_groups|/astraStar-FERRE-{v_astra}-{cat_id}@component_default|-{task_id}.fits
 astraStarCannon = $MWM_ASTRA/{v_astra}/{run2d}-{apred}/results/star/@cat_id_groups|/astraStar-Cannon-{v_astra}-{cat_id}@component_default|-{task_id}.fits
@@ -367,10 +375,16 @@
 
 # SSPP VAC
 AllStarSSPP = $MWM_SSPP/{v_sspp}/allStar-SSPP-{v_sspp}.fits
 
 # LVM paths
 lvm_lab = $LVM_DATA_LAB/{mjd}/sdR-{hemi}-{camspec}-{expnum:0>8}.fits.gz
 lvm_raw = $LVM_DATA_S/{mjd}/sdR-{hemi}-{camspec}-{expnum:0>8}.fits.gz
+lvm_anc = $LVM_SPECTRO_REDUX/{drpver}/{tileid}/{mjd}/ancillary/lvm-{kind}{imagetype}-{camera}-{expnum:0>8}.fits
+lvm_cal = $LVM_SPECTRO_REDUX/{drpver}/{tileid}/{mjd}/calib/lvm-{kind}-{camera}-{expnum:0>8}.{ext}
+lvm_cal_mbias = $LVM_SPECTRO_REDUX/{drpver}/{tileid}/{mjd}/calib/lvm-mbias-{camera}.fits
+lvm_cal_time = $LVM_SPECTRO_REDUX/{drpver}/{tileid}/{mjd}/calib/lvm-{kind}-{camera}-{exptime}.fits
+lvm_cal_pix = $LVM_SPECTRO_REDUX/{drpver}/{tileid}/{mjd}/calib/lvm-pixwave-{lamp}-{camera}-{expnum:0>8}.fits
+lvm_cal_through = $LVM_SPECTRO_REDUX/{drpver}/{tileid}/{mjd}/calib/lvm-throughput-{expnum:0>8}.fits
 
 # HIPS paths
 sdss_moc = $SDSS_HIPS/{release}/{survey}/Moc.{ext}
```

### Comparing `sdss-tree-3.1.6/python/tree/data/sdsswork.cfg` & `sdss-tree-3.1.7/python/tree/data/sdsswork.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/misc/docutree.py` & `sdss-tree-3.1.7/python/tree/misc/docutree.py`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/python/tree/tree.py` & `sdss-tree-3.1.7/python/tree/tree.py`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.6/setup.cfg` & `sdss-tree-3.1.7/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sdss-tree
-version = 3.1.6
+version = 3.1.7
 author = Brian Cherinka
 author_email = bcherinka@stsci.edu
 description = Control and setup of SDSS tree environment and modules
 url = https://github.com/sdss/tree
 project_urls = 
 	Repository = https://github.com/sdss/tree
 	Documentation = https://sdss-tree.readthedocs.org
```

