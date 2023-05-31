# Comparing `tmp/meta_matching_tool-1.5.0.tar.gz` & `tmp/meta_matching_tool-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meta_matching_tool-1.5.0.tar", last modified: Wed May 31 03:09:03 2023, max compression
+gzip compressed data, was "dist/meta_matching_tool-1.6.0.tar", last modified: Wed May 31 03:21:46 2023, max compression
```

## Comparing `meta_matching_tool-1.5.0.tar` & `meta_matching_tool-1.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-31 03:09:03.538874 meta_matching_tool-1.5.0/
--rw-r--r--   0 tlq        (501) staff       (20)     1073 2023-05-31 02:35:30.000000 meta_matching_tool-1.5.0/LICENSE.txt
--rw-r--r--   0 tlq        (501) staff       (20)      469 2023-05-31 03:09:03.537768 meta_matching_tool-1.5.0/PKG-INFO
--rw-r--r--   0 tlq        (501) staff       (20)     5752 2023-05-31 02:35:07.000000 meta_matching_tool-1.5.0/README.md
-drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-31 03:09:03.532869 meta_matching_tool-1.5.0/meta_matching_tool/
--rw-rw-r--   0 tlq        (501) staff       (20)       96 2023-05-31 02:58:57.000000 meta_matching_tool-1.5.0/meta_matching_tool/__init__.py
--rw-rw-r--   0 tlq        (501) staff       (20)     6737 2023-04-22 11:36:33.000000 meta_matching_tool-1.5.0/meta_matching_tool/model.py
--rw-rw-r--   0 tlq        (501) staff       (20)    12243 2023-04-22 11:36:33.000000 meta_matching_tool-1.5.0/meta_matching_tool/utils.py
-drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-31 03:09:03.537043 meta_matching_tool-1.5.0/meta_matching_tool.egg-info/
--rw-r--r--   0 tlq        (501) staff       (20)      469 2023-05-31 03:09:03.000000 meta_matching_tool-1.5.0/meta_matching_tool.egg-info/PKG-INFO
--rw-r--r--   0 tlq        (501) staff       (20)      367 2023-05-31 03:09:03.000000 meta_matching_tool-1.5.0/meta_matching_tool.egg-info/SOURCES.txt
--rw-r--r--   0 tlq        (501) staff       (20)        1 2023-05-31 03:09:03.000000 meta_matching_tool-1.5.0/meta_matching_tool.egg-info/dependency_links.txt
--rw-r--r--   0 tlq        (501) staff       (20)        1 2023-05-31 03:09:03.000000 meta_matching_tool-1.5.0/meta_matching_tool.egg-info/not-zip-safe
--rw-r--r--   0 tlq        (501) staff       (20)       84 2023-05-31 03:09:03.000000 meta_matching_tool-1.5.0/meta_matching_tool.egg-info/requires.txt
--rw-r--r--   0 tlq        (501) staff       (20)       19 2023-05-31 03:09:03.000000 meta_matching_tool-1.5.0/meta_matching_tool.egg-info/top_level.txt
--rw-r--r--   0 tlq        (501) staff       (20)       38 2023-05-31 03:09:03.539409 meta_matching_tool-1.5.0/setup.cfg
--rw-r--r--   0 tlq        (501) staff       (20)      983 2023-05-31 03:08:43.000000 meta_matching_tool-1.5.0/setup.py
+drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-31 03:21:46.900971 meta_matching_tool-1.6.0/
+-rw-r--r--   0 tlq        (501) staff       (20)     1073 2023-05-31 02:35:30.000000 meta_matching_tool-1.6.0/LICENSE.txt
+-rw-r--r--   0 tlq        (501) staff       (20)      469 2023-05-31 03:21:46.899990 meta_matching_tool-1.6.0/PKG-INFO
+-rw-r--r--   0 tlq        (501) staff       (20)     5752 2023-05-31 02:35:07.000000 meta_matching_tool-1.6.0/README.md
+drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-31 03:21:46.893100 meta_matching_tool-1.6.0/meta_matching_tool/
+-rw-rw-r--   0 tlq        (501) staff       (20)       96 2023-05-31 02:58:57.000000 meta_matching_tool-1.6.0/meta_matching_tool/__init__.py
+-rw-rw-r--   0 tlq        (501) staff       (20)     6737 2023-04-22 11:36:33.000000 meta_matching_tool-1.6.0/meta_matching_tool/model.py
+-rw-rw-r--   0 tlq        (501) staff       (20)    12243 2023-04-22 11:36:33.000000 meta_matching_tool-1.6.0/meta_matching_tool/utils.py
+drwxr-xr-x   0 tlq        (501) staff       (20)        0 2023-05-31 03:21:46.898506 meta_matching_tool-1.6.0/meta_matching_tool.egg-info/
+-rw-r--r--   0 tlq        (501) staff       (20)      469 2023-05-31 03:21:46.000000 meta_matching_tool-1.6.0/meta_matching_tool.egg-info/PKG-INFO
+-rw-r--r--   0 tlq        (501) staff       (20)      367 2023-05-31 03:21:46.000000 meta_matching_tool-1.6.0/meta_matching_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 tlq        (501) staff       (20)        1 2023-05-31 03:21:46.000000 meta_matching_tool-1.6.0/meta_matching_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 tlq        (501) staff       (20)        1 2023-05-31 03:21:46.000000 meta_matching_tool-1.6.0/meta_matching_tool.egg-info/not-zip-safe
+-rw-r--r--   0 tlq        (501) staff       (20)       84 2023-05-31 03:21:46.000000 meta_matching_tool-1.6.0/meta_matching_tool.egg-info/requires.txt
+-rw-r--r--   0 tlq        (501) staff       (20)       19 2023-05-31 03:21:46.000000 meta_matching_tool-1.6.0/meta_matching_tool.egg-info/top_level.txt
+-rw-r--r--   0 tlq        (501) staff       (20)       38 2023-05-31 03:21:46.901373 meta_matching_tool-1.6.0/setup.cfg
+-rw-r--r--   0 tlq        (501) staff       (20)     1046 2023-05-31 03:21:34.000000 meta_matching_tool-1.6.0/setup.py
```

### Comparing `meta_matching_tool-1.5.0/LICENSE.txt` & `meta_matching_tool-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meta_matching_tool-1.5.0/README.md` & `meta_matching_tool-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `meta_matching_tool-1.5.0/meta_matching_tool/model.py` & `meta_matching_tool-1.6.0/meta_matching_tool/model.py`

 * *Files identical despite different names*

### Comparing `meta_matching_tool-1.5.0/meta_matching_tool/utils.py` & `meta_matching_tool-1.6.0/meta_matching_tool/utils.py`

 * *Files identical despite different names*

### Comparing `meta_matching_tool-1.5.0/setup.py` & `meta_matching_tool-1.6.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,33 +5,32 @@
 
 from setuptools import find_packages
 from setuptools import setup
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
-VERSION = '1.5.0'
+VERSION = '1.6.0'
 
 setup(
     name='meta_matching_tool',  # package name
     version=VERSION,  # package version
     description='An integrated deep learning framework for the interpretation of untargeted metabolomics data', 
     author='Leqi Tian',
     author_email='220049029@link.cuhk.edu.cn',
     url='https://github.com/tianlq-prog/SPARSENN',
     classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     ],
     python_requires=">=3.9",
-    
     install_requires=[
         'numpy>=1.21.5',
         'pandas>=1.5.3',
         'python_igraph>=0.10.4',
        'scikit_learn>=1.0.2',
         'torch>=1.11.0',
     ],
+    packages=find_packages(exclude=('Tutorial', 'docs', 'notebooks', 'real_data_preprocessing')),
     zip_safe=False,
-    packages=find_packages(),
 )
```

