# Comparing `tmp/meta_matching_tool-1.6.0.tar.gz` & `tmp/meta_matching_tool-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meta_matching_tool-1.6.0.tar", last modified: Wed May 31 03:21:46 2023, max compression
+gzip compressed data, was "dist/meta_matching_tool-1.7.0.tar", last modified: Wed May 31 05:47:49 2023, max compression
```

## Comparing `meta_matching_tool-1.6.0.tar` & `meta_matching_tool-1.7.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-31 03:21:46.900971 meta_matching_tool-1.6.0/
--rw-r--r--   0 tlq        (501) staff       (20)     1073 2023-05-31 02:35:30.000000 meta_matching_tool-1.6.0/LICENSE.txt
--rw-r--r--   0 tlq        (501) staff       (20)      469 2023-05-31 03:21:46.899990 meta_matching_tool-1.6.0/PKG-INFO
--rw-r--r--   0 tlq        (501) staff       (20)     5752 2023-05-31 02:35:07.000000 meta_matching_tool-1.6.0/README.md
-drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-31 03:21:46.893100 meta_matching_tool-1.6.0/meta_matching_tool/
--rw-rw-r--   0 tlq        (501) staff       (20)       96 2023-05-31 02:58:57.000000 meta_matching_tool-1.6.0/meta_matching_tool/__init__.py
--rw-rw-r--   0 tlq        (501) staff       (20)     6737 2023-04-22 11:36:33.000000 meta_matching_tool-1.6.0/meta_matching_tool/model.py
--rw-rw-r--   0 tlq        (501) staff       (20)    12243 2023-04-22 11:36:33.000000 meta_matching_tool-1.6.0/meta_matching_tool/utils.py
-drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-31 03:21:46.898506 meta_matching_tool-1.6.0/meta_matching_tool.egg-info/
--rw-r--r--   0 tlq        (501) staff       (20)      469 2023-05-31 03:21:46.000000 meta_matching_tool-1.6.0/meta_matching_tool.egg-info/PKG-INFO
--rw-r--r--   0 tlq        (501) staff       (20)      367 2023-05-31 03:21:46.000000 meta_matching_tool-1.6.0/meta_matching_tool.egg-info/SOURCES.txt
--rw-r--r--   0 tlq        (501) staff       (20)        1 2023-05-31 03:21:46.000000 meta_matching_tool-1.6.0/meta_matching_tool.egg-info/dependency_links.txt
--rw-r--r--   0 tlq        (501) staff       (20)        1 2023-05-31 03:21:46.000000 meta_matching_tool-1.6.0/meta_matching_tool.egg-info/not-zip-safe
--rw-r--r--   0 tlq        (501) staff       (20)       84 2023-05-31 03:21:46.000000 meta_matching_tool-1.6.0/meta_matching_tool.egg-info/requires.txt
--rw-r--r--   0 tlq        (501) staff       (20)       19 2023-05-31 03:21:46.000000 meta_matching_tool-1.6.0/meta_matching_tool.egg-info/top_level.txt
--rw-r--r--   0 tlq        (501) staff       (20)       38 2023-05-31 03:21:46.901373 meta_matching_tool-1.6.0/setup.cfg
--rw-r--r--   0 tlq        (501) staff       (20)     1046 2023-05-31 03:21:34.000000 meta_matching_tool-1.6.0/setup.py
+drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-31 05:47:49.685210 meta_matching_tool-1.7.0/
+-rw-r--r--   0 tlq        (501) staff       (20)     1073 2023-05-31 02:35:30.000000 meta_matching_tool-1.7.0/LICENSE.txt
+-rw-r--r--   0 tlq        (501) staff       (20)      469 2023-05-31 05:47:49.684685 meta_matching_tool-1.7.0/PKG-INFO
+-rw-r--r--   0 tlq        (501) staff       (20)     5752 2023-05-31 02:35:07.000000 meta_matching_tool-1.7.0/README.md
+drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-31 05:47:49.663224 meta_matching_tool-1.7.0/meta_matching_tool/
+-rw-rw-r--   0 tlq        (501) staff       (20)       96 2023-05-31 02:58:57.000000 meta_matching_tool-1.7.0/meta_matching_tool/__init__.py
+drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-31 05:47:49.679293 meta_matching_tool-1.7.0/meta_matching_tool/data/
+-rw-rw-r--   0 tlq        (501) staff       (20)  1683575 2023-04-22 11:36:33.000000 meta_matching_tool-1.7.0/meta_matching_tool/data/adj_mtx.csv
+-rw-rw-r--   0 tlq        (501) staff       (20)   568889 2023-04-22 11:36:33.000000 meta_matching_tool-1.7.0/meta_matching_tool/data/graph.graphhml
+-rw-rw-r--   0 tlq        (501) staff       (20)     6737 2023-04-22 11:36:33.000000 meta_matching_tool-1.7.0/meta_matching_tool/model.py
+-rw-rw-r--   0 tlq        (501) staff       (20)    12243 2023-05-31 05:30:28.000000 meta_matching_tool-1.7.0/meta_matching_tool/utils.py
+drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-31 05:47:49.668465 meta_matching_tool-1.7.0/meta_matching_tool.egg-info/
+-rw-r--r--   0 tlq        (501) staff       (20)      469 2023-05-31 05:47:49.000000 meta_matching_tool-1.7.0/meta_matching_tool.egg-info/PKG-INFO
+-rw-r--r--   0 tlq        (501) staff       (20)      442 2023-05-31 05:47:49.000000 meta_matching_tool-1.7.0/meta_matching_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 tlq        (501) staff       (20)        1 2023-05-31 05:47:49.000000 meta_matching_tool-1.7.0/meta_matching_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 tlq        (501) staff       (20)        1 2023-05-31 05:47:49.000000 meta_matching_tool-1.7.0/meta_matching_tool.egg-info/not-zip-safe
+-rw-r--r--   0 tlq        (501) staff       (20)       84 2023-05-31 05:47:49.000000 meta_matching_tool-1.7.0/meta_matching_tool.egg-info/requires.txt
+-rw-r--r--   0 tlq        (501) staff       (20)       19 2023-05-31 05:47:49.000000 meta_matching_tool-1.7.0/meta_matching_tool.egg-info/top_level.txt
+-rw-r--r--   0 tlq        (501) staff       (20)       38 2023-05-31 05:47:49.685391 meta_matching_tool-1.7.0/setup.cfg
+-rw-r--r--   0 tlq        (501) staff       (20)     1200 2023-05-31 05:47:35.000000 meta_matching_tool-1.7.0/setup.py
```

### Comparing `meta_matching_tool-1.6.0/LICENSE.txt` & `meta_matching_tool-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meta_matching_tool-1.6.0/README.md` & `meta_matching_tool-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `meta_matching_tool-1.6.0/meta_matching_tool/model.py` & `meta_matching_tool-1.7.0/meta_matching_tool/model.py`

 * *Files identical despite different names*

### Comparing `meta_matching_tool-1.6.0/meta_matching_tool/utils.py` & `meta_matching_tool-1.7.0/meta_matching_tool/utils.py`

 * *Files identical despite different names*

### Comparing `meta_matching_tool-1.6.0/setup.py` & `meta_matching_tool-1.7.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import find_packages
 from setuptools import setup
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
-VERSION = '1.6.0'
+VERSION = '1.7.0'
 
 setup(
     name='meta_matching_tool',  # package name
     version=VERSION,  # package version
     description='An integrated deep learning framework for the interpretation of untargeted metabolomics data', 
     author='Leqi Tian',
     author_email='220049029@link.cuhk.edu.cn',
@@ -25,12 +25,16 @@
     ],
     python_requires=">=3.9",
     install_requires=[
         'numpy>=1.21.5',
         'pandas>=1.5.3',
         'python_igraph>=0.10.4',
        'scikit_learn>=1.0.2',
-        'torch>=1.11.0',
+        'torch >= 1.11.0',
     ],
     packages=find_packages(exclude=('Tutorial', 'docs', 'notebooks', 'real_data_preprocessing')),
+    package_data={
+        'meta_matching_tool': ['data/*'],  # Update the package name and directory accordingly
+    },
+    include_package_data=True,
     zip_safe=False,
 )
```

