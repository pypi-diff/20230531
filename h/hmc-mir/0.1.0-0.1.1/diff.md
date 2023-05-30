# Comparing `tmp/hmc_mir-0.1.0.tar.gz` & `tmp/hmc_mir-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmc_mir-0.1.0.tar", last modified: Tue May 30 22:21:46 2023, max compression
+gzip compressed data, was "hmc_mir-0.1.1.tar", last modified: Tue May 30 23:47:20 2023, max compression
```

## Comparing `hmc_mir-0.1.0.tar` & `hmc_mir-0.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:46.531667 hmc_mir-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:46.523667 hmc_mir-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:46.527667 hmc_mir-0.1.0/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:46.527667 hmc_mir-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-30 22:21:46.531667 hmc_mir-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:46.527667 hmc_mir-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:46.527667 hmc_mir-0.1.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:46.523667 hmc_mir-0.1.0/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:46.527667 hmc_mir-0.1.0/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/docs/source/_templates/autosummary/function.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-30 22:21:46.531667 hmc_mir-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:46.523667 hmc_mir-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:46.527667 hmc_mir-0.1.0/src/hmc_mir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/src/hmc_mir/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:46.531667 hmc_mir-0.1.0/src/hmc_mir/align/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/src/hmc_mir/align/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/src/hmc_mir/align/dtw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/src/hmc_mir/align/flex_dtw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/src/hmc_mir/align/hstw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/src/hmc_mir/align/nwtw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:46.531667 hmc_mir-0.1.0/src/hmc_mir/bootleg_score/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/src/hmc_mir/bootleg_score/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29439 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/src/hmc_mir/bootleg_score/bootleg_score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:46.531667 hmc_mir-0.1.0/src/hmc_mir/tsm_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/src/hmc_mir/tsm_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/src/hmc_mir/tsm_tools/tsm_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:46.527667 hmc_mir-0.1.0/src/hmc_mir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-30 22:21:46.000000 hmc_mir-0.1.0/src/hmc_mir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-30 22:21:46.000000 hmc_mir-0.1.0/src/hmc_mir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:21:46.000000 hmc_mir-0.1.0/src/hmc_mir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-30 22:21:46.000000 hmc_mir-0.1.0/src/hmc_mir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 22:21:46.000000 hmc_mir-0.1.0/src/hmc_mir.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:46.531667 hmc_mir-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:21:38.000000 hmc_mir-0.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.228366 hmc_mir-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.220366 hmc_mir-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.220366 hmc_mir-0.1.1/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.224366 hmc_mir-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-30 23:47:20.228366 hmc_mir-0.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.224366 hmc_mir-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.224366 hmc_mir-0.1.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.220366 hmc_mir-0.1.1/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.224366 hmc_mir-0.1.1/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/docs/source/_templates/autosummary/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-30 23:47:20.228366 hmc_mir-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.220366 hmc_mir-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.224366 hmc_mir-0.1.1/src/hmc_mir/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.228366 hmc_mir-0.1.1/src/hmc_mir/align/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/align/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/align/dtw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/align/flex_dtw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/align/hstw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/align/nwtw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.228366 hmc_mir-0.1.1/src/hmc_mir/bootleg_score/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/bootleg_score/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29368 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/bootleg_score/bootleg_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.228366 hmc_mir-0.1.1/src/hmc_mir/tsm_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/tsm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/src/hmc_mir/tsm_tools/tsm_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.224366 hmc_mir-0.1.1/src/hmc_mir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-30 23:47:20.000000 hmc_mir-0.1.1/src/hmc_mir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-30 23:47:20.000000 hmc_mir-0.1.1/src/hmc_mir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 23:47:20.000000 hmc_mir-0.1.1/src/hmc_mir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-30 23:47:20.000000 hmc_mir-0.1.1/src/hmc_mir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 23:47:20.000000 hmc_mir-0.1.1/src/hmc_mir.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:20.228366 hmc_mir-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 23:47:11.000000 hmc_mir-0.1.1/tests/__init__.py
```

### Comparing `hmc_mir-0.1.0/.github/scripts/release.py` & `hmc_mir-0.1.1/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.0/.github/workflows/docs.yml` & `hmc_mir-0.1.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.0/LICENSE` & `hmc_mir-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.0/PKG-INFO` & `hmc_mir-0.1.1/src/hmc_mir.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hmc_mir
-Version: 0.1.0
+Name: hmc-mir
+Version: 0.1.1
 Summary: Collection of tools developed by HMCs MIR Lab
 Home-page: https://github.com/HMC-MIR/hmc-mir-tools
 Project-URL: Bug Tracker, https://github.com/HMC-MIR/hmc-mir-tools/issues
 Project-URL: Changelog, https://github.com/HMC-MIR/hmc-mir-tools/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `hmc_mir-0.1.0/docs/Makefile` & `hmc_mir-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.0/docs/make.bat` & `hmc_mir-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.0/docs/source/_templates/autosummary/class.rst` & `hmc_mir-0.1.1/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.0/docs/source/_templates/autosummary/module.rst` & `hmc_mir-0.1.1/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.0/docs/source/conf.py` & `hmc_mir-0.1.1/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "sphinx.ext.viewcode",
     "sphinx.ext.autosummary",
     'recommonmark',
     'sphinx.ext.githubpages',
     'sphinx.ext.todo'
 ]
 
-# autosummary_generate = True
+autosummary_generate = True
 autodoc_typehints = "description"
 
 napoleon_custom_sections = [('Returns', 'params_style')]
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
```

### Comparing `hmc_mir-0.1.0/setup.cfg` & `hmc_mir-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.0/src/hmc_mir/align/dtw.py` & `hmc_mir-0.1.1/src/hmc_mir/align/dtw.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.0/src/hmc_mir/align/flex_dtw.py` & `hmc_mir-0.1.1/src/hmc_mir/align/flex_dtw.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.0/src/hmc_mir/align/hstw.py` & `hmc_mir-0.1.1/src/hmc_mir/align/hstw.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.0/src/hmc_mir/align/nwtw.py` & `hmc_mir-0.1.1/src/hmc_mir/align/nwtw.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.0/src/hmc_mir/bootleg_score/bootleg_score.py` & `hmc_mir-0.1.1/src/hmc_mir/bootleg_score/bootleg_score.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-"""Extracting bootleg scores from sheet music images."""
+"""Extracting bootleg scores from sheet music images.
+"""
 
 import numpy as np
-from numpy.matlib import repmat
 import matplotlib.pyplot as plt
 from PIL import Image, ImageFilter, ImageChops
 import cv2
 from skimage import filters, measure
-from skimage.measure import label, regionprops
+from skimage.measure import regionprops
 from sklearn.cluster import KMeans
 import matplotlib.patches as mpatches
 from scipy.signal import convolve2d
 import pickle
-import librosa as lb
 import time
 import os
 import os.path
-import glob
 
 def removeBkgdLighting(pimg, filtsz=5, thumbnailW = 100, thumbnailH = 100):
     tinyimg = pimg.copy()
     tinyimg.thumbnail([thumbnailW, thumbnailH]) # resize to speed up
     shadows = tinyimg.filter(ImageFilter.GaussianBlur(filtsz)).resize(pimg.size)
     result = ImageChops.invert(ImageChops.subtract(shadows, pimg))
     return result
```

### Comparing `hmc_mir-0.1.0/src/hmc_mir/tsm_tools/tsm_tools.py` & `hmc_mir-0.1.1/src/hmc_mir/tsm_tools/tsm_tools.py`

 * *Files identical despite different names*

### Comparing `hmc_mir-0.1.0/src/hmc_mir.egg-info/SOURCES.txt` & `hmc_mir-0.1.1/src/hmc_mir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

