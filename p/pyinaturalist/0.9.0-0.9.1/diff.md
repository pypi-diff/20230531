# Comparing `tmp/pyinaturalist-0.9.0.tar.gz` & `tmp/pyinaturalist-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyinaturalist-0.9.0.tar", last modified: Wed May  6 14:00:05 2020, max compression
+gzip compressed data, was "dist/pyinaturalist-0.9.1.tar", last modified: Tue May 26 10:51:33 2020, max compression
```

## Comparing `pyinaturalist-0.9.0.tar` & `pyinaturalist-0.9.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 nicolas_noe (1863200185) 1892331168        0 2020-05-06 14:00:05.000000 pyinaturalist-0.9.0/
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168      171 2020-05-06 13:51:48.000000 pyinaturalist-0.9.0/AUTHORS.rst
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168     1411 2020-05-05 14:37:25.000000 pyinaturalist-0.9.0/CONTRIBUTING.rst
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168     1324 2020-05-06 13:57:59.000000 pyinaturalist-0.9.0/HISTORY.rst
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168     1101 2020-05-05 14:37:25.000000 pyinaturalist-0.9.0/LICENSE
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168      100 2020-05-05 14:37:25.000000 pyinaturalist-0.9.0/MANIFEST.in
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168     7772 2020-05-06 14:00:05.000000 pyinaturalist-0.9.0/PKG-INFO
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168     4247 2020-05-05 14:37:25.000000 pyinaturalist-0.9.0/README.rst
-drwxr-xr-x   0 nicolas_noe (1863200185) 1892331168        0 2020-05-06 14:00:05.000000 pyinaturalist-0.9.0/pyinaturalist/
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168      299 2020-05-06 13:59:47.000000 pyinaturalist-0.9.0/pyinaturalist/__init__.py
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168      608 2020-05-06 13:51:48.000000 pyinaturalist-0.9.0/pyinaturalist/constants.py
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168       96 2020-05-05 14:37:25.000000 pyinaturalist-0.9.0/pyinaturalist/exceptions.py
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168     1012 2020-05-06 13:51:48.000000 pyinaturalist-0.9.0/pyinaturalist/helpers.py
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168     7236 2020-05-06 13:51:48.000000 pyinaturalist-0.9.0/pyinaturalist/node_api.py
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168    10263 2020-05-05 14:37:25.000000 pyinaturalist-0.9.0/pyinaturalist/rest_api.py
-drwxr-xr-x   0 nicolas_noe (1863200185) 1892331168        0 2020-05-06 14:00:05.000000 pyinaturalist-0.9.0/pyinaturalist.egg-info/
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168     7772 2020-05-06 14:00:05.000000 pyinaturalist-0.9.0/pyinaturalist.egg-info/PKG-INFO
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168      495 2020-05-06 14:00:05.000000 pyinaturalist-0.9.0/pyinaturalist.egg-info/SOURCES.txt
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168        1 2020-05-06 14:00:05.000000 pyinaturalist-0.9.0/pyinaturalist.egg-info/dependency_links.txt
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168        1 2020-05-05 14:37:48.000000 pyinaturalist-0.9.0/pyinaturalist.egg-info/not-zip-safe
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168      135 2020-05-06 14:00:05.000000 pyinaturalist-0.9.0/pyinaturalist.egg-info/requires.txt
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168       14 2020-05-06 14:00:05.000000 pyinaturalist-0.9.0/pyinaturalist.egg-info/top_level.txt
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168       61 2020-05-06 14:00:05.000000 pyinaturalist-0.9.0/setup.cfg
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168     1645 2020-05-06 13:59:23.000000 pyinaturalist-0.9.0/setup.py
-drwxr-xr-x   0 nicolas_noe (1863200185) 1892331168        0 2020-05-06 14:00:05.000000 pyinaturalist-0.9.0/test/
--rwxr-xr-x   0 nicolas_noe (1863200185) 1892331168    18045 2020-05-06 13:51:48.000000 pyinaturalist-0.9.0/test/test_pyinaturalist.py
+drwxr-xr-x   0 nicolas_noe (1863200185) 1892331168        0 2020-05-26 10:51:33.000000 pyinaturalist-0.9.1/
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168      171 2020-05-06 13:51:48.000000 pyinaturalist-0.9.1/AUTHORS.rst
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168     1411 2020-05-05 14:37:25.000000 pyinaturalist-0.9.1/CONTRIBUTING.rst
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168     1507 2020-05-26 10:49:18.000000 pyinaturalist-0.9.1/HISTORY.rst
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168     1101 2020-05-05 14:37:25.000000 pyinaturalist-0.9.1/LICENSE
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168      100 2020-05-05 14:37:25.000000 pyinaturalist-0.9.1/MANIFEST.in
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168     7995 2020-05-26 10:51:33.000000 pyinaturalist-0.9.1/PKG-INFO
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168     4247 2020-05-05 14:37:25.000000 pyinaturalist-0.9.1/README.rst
+drwxr-xr-x   0 nicolas_noe (1863200185) 1892331168        0 2020-05-26 10:51:33.000000 pyinaturalist-0.9.1/pyinaturalist/
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168      299 2020-05-26 10:50:49.000000 pyinaturalist-0.9.1/pyinaturalist/__init__.py
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168      608 2020-05-06 13:51:48.000000 pyinaturalist-0.9.1/pyinaturalist/constants.py
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168       96 2020-05-05 14:37:25.000000 pyinaturalist-0.9.1/pyinaturalist/exceptions.py
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168     1344 2020-05-26 10:34:13.000000 pyinaturalist-0.9.1/pyinaturalist/helpers.py
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168     7304 2020-05-26 10:34:13.000000 pyinaturalist-0.9.1/pyinaturalist/node_api.py
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168    10263 2020-05-05 14:37:25.000000 pyinaturalist-0.9.1/pyinaturalist/rest_api.py
+drwxr-xr-x   0 nicolas_noe (1863200185) 1892331168        0 2020-05-26 10:51:33.000000 pyinaturalist-0.9.1/pyinaturalist.egg-info/
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168     7995 2020-05-26 10:51:32.000000 pyinaturalist-0.9.1/pyinaturalist.egg-info/PKG-INFO
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168      516 2020-05-26 10:51:32.000000 pyinaturalist-0.9.1/pyinaturalist.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168        1 2020-05-26 10:51:32.000000 pyinaturalist-0.9.1/pyinaturalist.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168        1 2020-05-05 14:37:48.000000 pyinaturalist-0.9.1/pyinaturalist.egg-info/not-zip-safe
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168      141 2020-05-26 10:51:32.000000 pyinaturalist-0.9.1/pyinaturalist.egg-info/requires.txt
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168       14 2020-05-26 10:51:32.000000 pyinaturalist-0.9.1/pyinaturalist.egg-info/top_level.txt
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168       61 2020-05-26 10:51:33.000000 pyinaturalist-0.9.1/setup.cfg
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168     1665 2020-05-26 10:50:36.000000 pyinaturalist-0.9.1/setup.py
+drwxr-xr-x   0 nicolas_noe (1863200185) 1892331168        0 2020-05-26 10:51:33.000000 pyinaturalist-0.9.1/test/
+-rw-r--r--   0 nicolas_noe (1863200185) 1892331168      852 2020-05-26 10:34:13.000000 pyinaturalist-0.9.1/test/test_helpers.py
+-rwxr-xr-x   0 nicolas_noe (1863200185) 1892331168    18045 2020-05-06 13:51:48.000000 pyinaturalist-0.9.1/test/test_pyinaturalist.py
```

### Comparing `pyinaturalist-0.9.0/CONTRIBUTING.rst` & `pyinaturalist-0.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyinaturalist-0.9.0/LICENSE` & `pyinaturalist-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyinaturalist-0.9.0/PKG-INFO` & `pyinaturalist-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinaturalist
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python client for the iNaturalist APIs
 Home-page: https://github.com/niconoe/pyinaturalist
 Author: Nicolas Noé
 Author-email: nicolas@niconoe.eu
 License: MIT
 Description: =============================
         pyinaturalist
@@ -132,14 +132,19 @@
         
         
         
         
         History
         -------
         
+        0.9.1 (2020-05-26)
+        ++++++++++++++++++
+        
+        * Bugfix: proper support for boolean and integer list parameters (see https://github.com/niconoe/pyinaturalist/issues/17). Thanks Jordan Cook!
+        
         0.9.0 (2020-05-06)
         ++++++++++++++++++
         
         * new taxa-related functions: node_api.get_taxa(), node_api.get_taxa_autocomplete(), node_api.get_taxa_by_id(). Many thanks to Jordan Cook!
         
         0.8.0 (2019-07-11)
         ++++++++++++++++++
```

### Comparing `pyinaturalist-0.9.0/README.rst` & `pyinaturalist-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyinaturalist-0.9.0/pyinaturalist/constants.py` & `pyinaturalist-0.9.1/pyinaturalist/constants.py`

 * *Files identical despite different names*

### Comparing `pyinaturalist-0.9.0/pyinaturalist/node_api.py` & `pyinaturalist-0.9.1/pyinaturalist/node_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from urllib.parse import urljoin
 
 from pyinaturalist.constants import THROTTLING_DELAY, INAT_NODE_API_BASE_URL, RANKS
 from pyinaturalist.exceptions import ObservationNotFound
 from pyinaturalist.helpers import (
     merge_two_dicts,
     get_user_agent,
-    concat_list_params,
+    convert_bool_params,
+    convert_list_params,
     strip_empty_params,
 )
 
 PER_PAGE_RESULTS = 30  # Paginated queries: how many records do we ask per page?
 
 logger = getLogger(__name__)
 
@@ -27,16 +28,17 @@
     """Make an API call to iNaturalist.
 
     endpoint is a string such as 'observations'
     method: 'GET', 'HEAD', 'POST', 'PUT', 'PATCH', 'DELETE'
     kwargs are passed to requests.request
     Returns a requests.Response object
     """
+    params = convert_bool_params(params)
+    params = convert_list_params(params)
     params = strip_empty_params(params)
-    params = concat_list_params(params)
     headers = {"Accept": "application/json", "User-Agent": get_user_agent(user_agent)}
 
     response = requests.get(
         urljoin(INAT_NODE_API_BASE_URL, endpoint), params, headers=headers, **kwargs
     )
     return response
```

### Comparing `pyinaturalist-0.9.0/pyinaturalist/rest_api.py` & `pyinaturalist-0.9.1/pyinaturalist/rest_api.py`

 * *Files identical despite different names*

### Comparing `pyinaturalist-0.9.0/pyinaturalist.egg-info/PKG-INFO` & `pyinaturalist-0.9.1/pyinaturalist.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinaturalist
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python client for the iNaturalist APIs
 Home-page: https://github.com/niconoe/pyinaturalist
 Author: Nicolas Noé
 Author-email: nicolas@niconoe.eu
 License: MIT
 Description: =============================
         pyinaturalist
@@ -132,14 +132,19 @@
         
         
         
         
         History
         -------
         
+        0.9.1 (2020-05-26)
+        ++++++++++++++++++
+        
+        * Bugfix: proper support for boolean and integer list parameters (see https://github.com/niconoe/pyinaturalist/issues/17). Thanks Jordan Cook!
+        
         0.9.0 (2020-05-06)
         ++++++++++++++++++
         
         * new taxa-related functions: node_api.get_taxa(), node_api.get_taxa_autocomplete(), node_api.get_taxa_by_id(). Many thanks to Jordan Cook!
         
         0.8.0 (2019-07-11)
         ++++++++++++++++++
```

### Comparing `pyinaturalist-0.9.0/setup.py` & `pyinaturalist-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 readme = open("README.rst").read()
 
 history = open("HISTORY.rst").read().replace(".. :changelog:", "")
 
 setup(
     name="pyinaturalist",
-    version="0.9.0",
+    version="0.9.1",
     description="Python client for the iNaturalist APIs",
     long_description=readme + "\n\n" + history,
     author="Nicolas Noé",
     author_email="nicolas@niconoe.eu",
     url="https://github.com/niconoe/pyinaturalist",
     packages=["pyinaturalist"],
     package_dir={"pyinaturalist": "pyinaturalist"},
@@ -36,14 +36,15 @@
             "mypy",
             "pytest",
             "requests-mock>=1.7",
             "Sphinx",
             "sphinx-autodoc-typehints",
             "sphinx-rtd-theme",
             "tox",
+            "twine"
         ]
     },
     license="MIT",
     zip_safe=False,
     keywords="pyinaturalist",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
```

### Comparing `pyinaturalist-0.9.0/test/test_pyinaturalist.py` & `pyinaturalist-0.9.1/test/test_pyinaturalist.py`

 * *Files identical despite different names*

