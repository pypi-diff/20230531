# Comparing `tmp/querynator-0.3.3.tar.gz` & `tmp/querynator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "querynator-0.3.3.tar", last modified: Fri May  5 12:11:21 2023, max compression
+gzip compressed data, was "querynator-0.4.0.tar", last modified: Wed May 31 13:06:10 2023, max compression
```

## Comparing `querynator-0.3.3.tar` & `querynator-0.4.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:11:21.601464 querynator-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-05 12:10:30.000000 querynator-0.3.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-05 12:10:30.000000 querynator-0.3.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-05 12:10:30.000000 querynator-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-05 12:10:30.000000 querynator-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-05 12:11:21.601464 querynator-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-05 12:10:30.000000 querynator-0.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:11:21.601464 querynator-0.3.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/changelog.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4881 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-05 12:10:30.000000 querynator-0.3.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:11:21.601464 querynator-0.3.3/querynator/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15304 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:11:21.601464 querynator-0.3.3/querynator/helper_functions/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/helper_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/helper_functions/helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:11:21.601464 querynator-0.3.3/querynator/query_api/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/query_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/query_api/cancertypes.js
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/query_api/cgi_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19214 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/query_api/civic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:11:21.601464 querynator-0.3.3/querynator/report_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/report_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/report_scripts/combine_cgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/report_scripts/combine_cgi_civic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/report_scripts/combine_civic.py
--rw-r--r--   0 runner    (1001) docker     (123)    23675 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/report_scripts/create_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/report_scripts/sort_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:11:21.601464 querynator-0.3.3/querynator/report_scripts/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/report_scripts/templates/template_individual.html
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/report_scripts/templates/template_overall_plotly_pieplots.html
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/report_scripts/templates/template_overall_upsetplots.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:11:21.601464 querynator-0.3.3/querynator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-05 12:11:21.000000 querynator-0.3.3/querynator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-05 12:11:21.000000 querynator-0.3.3/querynator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:11:21.000000 querynator-0.3.3/querynator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-05 12:11:21.000000 querynator-0.3.3/querynator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:10:40.000000 querynator-0.3.3/querynator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-05 12:11:21.000000 querynator-0.3.3/querynator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 12:11:21.000000 querynator-0.3.3/querynator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-05 12:10:30.000000 querynator-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:11:21.601464 querynator-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-05 12:10:30.000000 querynator-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:11:21.601464 querynator-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-05 12:10:30.000000 querynator-0.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-05 12:10:30.000000 querynator-0.3.3/tests/test_querynator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:06:10.857042 querynator-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-31 13:05:13.000000 querynator-0.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-31 13:05:13.000000 querynator-0.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-31 13:05:13.000000 querynator-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-31 13:05:13.000000 querynator-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-05-31 13:06:10.857042 querynator-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-31 13:05:13.000000 querynator-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:06:10.857042 querynator-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/changelog.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4881 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-31 13:05:13.000000 querynator-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:06:10.857042 querynator-0.4.0/querynator/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15304 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:06:10.857042 querynator-0.4.0/querynator/helper_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/helper_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/helper_functions/helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:06:10.857042 querynator-0.4.0/querynator/query_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/query_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/query_api/cancertypes.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/query_api/cgi_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19214 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/query_api/civic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:06:10.857042 querynator-0.4.0/querynator/report_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/report_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/report_scripts/combine_cgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/report_scripts/combine_cgi_civic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/report_scripts/combine_civic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24775 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/report_scripts/create_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/report_scripts/sort_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:06:10.857042 querynator-0.4.0/querynator/report_scripts/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/report_scripts/templates/template_individual.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/report_scripts/templates/template_overall_plotly_pieplots.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/report_scripts/templates/template_overall_upsetplots.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:06:10.857042 querynator-0.4.0/querynator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-05-31 13:06:10.000000 querynator-0.4.0/querynator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-31 13:06:10.000000 querynator-0.4.0/querynator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:06:10.000000 querynator-0.4.0/querynator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 13:06:10.000000 querynator-0.4.0/querynator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:05:25.000000 querynator-0.4.0/querynator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-31 13:06:10.000000 querynator-0.4.0/querynator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 13:06:10.000000 querynator-0.4.0/querynator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-31 13:05:13.000000 querynator-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:06:10.857042 querynator-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-31 13:05:13.000000 querynator-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:06:10.857042 querynator-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 13:05:13.000000 querynator-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-31 13:05:13.000000 querynator-0.4.0/tests/test_querynator.py
```

### Comparing `querynator-0.3.3/CHANGELOG.rst` & `querynator-0.4.0/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 Changelog
 ============
 
+0.4.0 - Stormy Saturn  (2023-05-31)
+---------------------------------------------
+
+**Added**
+
+**Fixed**
+
+* Fixed functionality for new CGI file structure
+* Fixed case when CIViC has no hits
+
+**Dependencies**
+
+**Deprecated**
+
 0.3.3 - Iron Mercury  (2023-05-05)
 ---------------------------------------------
 
 **Added**
 
 **Fixed**
```

### Comparing `querynator-0.3.3/CONTRIBUTING.rst` & `querynator-0.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/LICENSE` & `querynator-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/PKG-INFO` & `querynator-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querynator
-Version: 0.3.3
+Version: 0.4.0
 Summary: Python package to query cancer variant databases
 Home-page: https://github.com/qbic-pipelines/querynator
 Author: Susanne Jodoin, Mark Polster
 Author-email: susanne.jodoin@qbic.uni-tuebingen.de, mark.polster@uni-tuebingen.de
 License: MIT license
 Keywords: querynator
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -76,14 +76,28 @@
 
 
 
 
 Changelog
 ============
 
+0.4.0 - Stormy Saturn  (2023-05-31)
+---------------------------------------------
+
+**Added**
+
+**Fixed**
+
+* Fixed functionality for new CGI file structure
+* Fixed case when CIViC has no hits
+
+**Dependencies**
+
+**Deprecated**
+
 0.3.3 - Iron Mercury  (2023-05-05)
 ---------------------------------------------
 
 **Added**
 
 **Fixed**
```

### Comparing `querynator-0.3.3/README.rst` & `querynator-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/docs/Makefile` & `querynator-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/docs/conf.py` & `querynator-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/docs/installation.rst` & `querynator-0.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/docs/make.bat` & `querynator-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/docs/modules.rst` & `querynator-0.4.0/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/docs/usage.rst` & `querynator-0.4.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/querynator/__main__.py` & `querynator-0.4.0/querynator/__main__.py`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/querynator/helper_functions/helper_functions.py` & `querynator-0.4.0/querynator/helper_functions/helper_functions.py`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/querynator/query_api/cancertypes.js` & `querynator-0.4.0/querynator/query_api/cancertypes.js`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/querynator/query_api/cgi_api.py` & `querynator-0.4.0/querynator/query_api/cgi_api.py`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/querynator/query_api/civic_api.py` & `querynator-0.4.0/querynator/query_api/civic_api.py`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/querynator/report_scripts/combine_cgi.py` & `querynator-0.4.0/querynator/report_scripts/combine_cgi.py`

 * *Files 12% similar despite different names*

```diff
@@ -156,14 +156,18 @@
     :param alterations_path: Path to alterations file
     :type alterations_path: str
     :return: None
     :rtype: None
     """
     alterations_df = pd.read_csv(alterations_path, sep="\t")
 
+    # change alterations_df format to prior format
+
+    alterations_df = subset_alterations(alterations_df)
+
     # extract positional information & add to df
     alterations_df[["chr", "pos", "ref", "alt"]] = alterations_df.apply(lambda x: extract_coords(x), axis=1)
 
     # rearrange cols
     alterations_df.insert(0, "chr", alterations_df.pop("chr"))
     alterations_df.insert(1, "pos", alterations_df.pop("pos"))
     alterations_df.insert(2, "ref", alterations_df.pop("ref"))
@@ -171,14 +175,57 @@
 
     # add suffix
     alterations_df = alterations_df.add_suffix("_CGI")
 
     return alterations_df
 
 
+def subset_alterations(df):
+    """
+    subset alterations file to only include relevant columns
+    :param df: alterations DataFrame
+    :type df: pandas DataFrame
+    :return: subsetted alterations DataFrame
+    :rtype: pandas DataFrame
+    """
+    # subset df
+    df = df[
+        [
+            "CGI-INFO",
+            "CGI-Gene",
+            "CGI-Protein Change",
+            "CGI-Oncogenic Summary",
+            "CGI-Oncogenic Prediction",
+            "CGI-External oncogenic annotation",
+            "CGI-Mutation",
+            "CGI-Consequence",
+            "CGI-Transcript",
+            "CGI-STRAND",
+            "CGI-Type",
+        ]
+    ]
+
+    # rename cols
+    new_col_names = [
+        "Sample ID",
+        "Gene",
+        "Protein Change",
+        "Oncogenic Summary",
+        "Oncogenic Prediction",
+        "External oncogenic annotation",
+        "Mutation",
+        "Consequence",
+        "Transcript",
+        "Strand",
+        "Type",
+    ]
+    df.columns = new_col_names
+    return df
+
+
 def merge_alterations_vep(vep_df, alterations_df):
     """
     merge vep and CGI alterations annotations for each variant based on positional information (chr, pos, ref, alt)
 
     :param vep_df: DataFrame of variants and their VEP annotation
     :type vep_df: pandas DataFrame
     :param alterations_df: DataFrame of variants and their CGI alterations annotations
@@ -220,15 +267,19 @@
     add alteration-link column to "biomarkers.tsv"
 
     :param biomarkers_df: pd DataFrame of the projects "biomarkers.tsv"
     :type biomarkers_df: pandas DataFrame
     :return: DataFrame of biomarkers with additional alteration-link col
     :rtype: pandas DataFrame
     """
-    biomarkers_df["alterations_link"] = biomarkers_df.apply(lambda x: get_all_alterations(x), axis=1)
+    # only works when biomarkers_df is not an empty df
+    try:
+        biomarkers_df["alterations_link"] = biomarkers_df.apply(lambda x: get_all_alterations(x), axis=1)
+    except ValueError:
+        biomarkers_df["alterations_link"] = ""
 
     return biomarkers_df
 
 
 def get_highest_evidence(row, biomarkers_linked):
     """
     get highest associated CGI evidence of the current alteration (A-D) from the biomarkers datafrane
@@ -236,15 +287,20 @@
     :param row: row of a pandas DataFrame
     :type row: pandas Series
     :param biomarkers_linked: pd DataFrame of the projects "biomarkers.tsv"
     :type biomarkers_linked: pandas DataFrame
     :return: highest associated evidence
     :rtype: str
     """
+
+    x = False
     if not pd.isnull(row["Protein Change_CGI"]):
+        # escape special characters seen to be used in the Protein Change column
+        if row["Protein Change_CGI"].startswith("*"):
+            row["Protein Change_CGI"] = row["Protein Change_CGI"].replace("*", "\*")
         for evidence in ["A", "B", "C", "D"]:
             if not biomarkers_linked.loc[
                 (biomarkers_linked["alterations_link"].str.contains(row["Protein Change_CGI"]))
                 & (biomarkers_linked["Evidence"] == evidence)
             ].empty:
                 return evidence
     else:
```

### Comparing `querynator-0.3.3/querynator/report_scripts/combine_cgi_civic.py` & `querynator-0.4.0/querynator/report_scripts/combine_cgi_civic.py`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/querynator/report_scripts/create_report.py` & `querynator-0.4.0/querynator/report_scripts/create_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     plt.savefig(out_path)
 
     return fig
 
 
 def create_upsetplots(df, out_path):
     """
-    Create of (1) the number of variants per Knowledgebase and (2) the number of variants per tier
+    Create upsetplot of (1) the number of variants per Knowledgebase and (2) the number of variants per tier
 
     :param df: Variant dataframe
     :type df: pandas.DataFrame
     :param out_path: Path to output directory
     :type out_path: str
     :return: List of Upsetplot figures
     :rtype: list
@@ -199,20 +199,58 @@
     # fill tier df  & transform to upsetplot input format
     for i in ["tier_1", "tier_2", "tier_3", "tier_4"]:
         df_tiers[i] = df["report_tier"].apply(lambda x: True if x == i else False)
 
     tier_input = from_indicators(df_tiers)
 
     # create upsetplot figures
-    fig_kb = save_plot(kb_input, "Number of variants per Knowledgebase", os.path.join(out_path, "kb_upsetplot.png"))
-    fig_tiers = save_plot(tier_input, "Number of variants per Tier", os.path.join(out_path, "tier_upsetplot.png"))
+    # if only one col of df_kb is True and all others cols are False, no UpSetPlot can be generated. If that's the case, just generate a barplot
+    try:
+        fig_kb = save_plot(kb_input, "Number of variants per Knowledgebase", os.path.join(out_path, "kb_upsetplot.png"))
+    except AttributeError:
+        fig_kb = create_barplot(
+            df_kb, "Number of variants per Knowledgebase", os.path.join(out_path, "kb_upsetplot.png")
+        )
+    try:
+        fig_tiers = save_plot(tier_input, "Number of variants per Tier", os.path.join(out_path, "tier_upsetplot.png"))
+    except AttributeError:
+        fig_tiers = create_barplot(
+            tier_input, "Number of variants per Tier", os.path.join(out_path, "tier_upsetplot.png")
+        )
 
     return [fig_kb, fig_tiers]
 
 
+def create_barplot(input, title, out_path):
+    """
+    Creates and saves a barplot as png
+
+    :param input: input dataframe
+    :type input: pandas.DataFrame
+    :param title: title of the plot
+    :type title: str
+    :param out_path: output path
+    :type out_path: str
+    :return: matplotlib figure
+    :rtype: matplotlib figure
+    """
+
+    counts = input.sum().to_list()
+    kbs = input.columns.to_list()
+
+    # plot
+    fig = plt.figure(figsize=(6, 4))
+    plt.bar(kbs, counts, color="darkblue")
+
+    plt.suptitle(title)
+    plt.savefig(out_path)
+
+    return fig
+
+
 def encode_upsetplot(fig):
     """
     Encodes an upsetplot figure as base64
 
     :param fig: Upsetplot figure
     :type fig: matplotlib figure
     :return: Encoded upsetplot figure as string to add to report
```

### Comparing `querynator-0.3.3/querynator/report_scripts/sort_variants.py` & `querynator-0.4.0/querynator/report_scripts/sort_variants.py`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/querynator/report_scripts/templates/template_individual.html` & `querynator-0.4.0/querynator/report_scripts/templates/template_individual.html`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/querynator/report_scripts/templates/template_overall_plotly_pieplots.html` & `querynator-0.4.0/querynator/report_scripts/templates/template_overall_plotly_pieplots.html`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/querynator/report_scripts/templates/template_overall_upsetplots.html` & `querynator-0.4.0/querynator/report_scripts/templates/template_overall_upsetplots.html`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/querynator.egg-info/PKG-INFO` & `querynator-0.4.0/querynator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querynator
-Version: 0.3.3
+Version: 0.4.0
 Summary: Python package to query cancer variant databases
 Home-page: https://github.com/qbic-pipelines/querynator
 Author: Susanne Jodoin, Mark Polster
 Author-email: susanne.jodoin@qbic.uni-tuebingen.de, mark.polster@uni-tuebingen.de
 License: MIT license
 Keywords: querynator
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -76,14 +76,28 @@
 
 
 
 
 Changelog
 ============
 
+0.4.0 - Stormy Saturn  (2023-05-31)
+---------------------------------------------
+
+**Added**
+
+**Fixed**
+
+* Fixed functionality for new CGI file structure
+* Fixed case when CIViC has no hits
+
+**Dependencies**
+
+**Deprecated**
+
 0.3.3 - Iron Mercury  (2023-05-05)
 ---------------------------------------------
 
 **Added**
 
 **Fixed**
```

### Comparing `querynator-0.3.3/querynator.egg-info/SOURCES.txt` & `querynator-0.4.0/querynator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `querynator-0.3.3/setup.py` & `querynator-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,10 +42,10 @@
     keywords="querynator",
     name="querynator",
     packages=find_packages(exclude=("docs")),
     package_data={"": ["report_scripts/templates/*.html"]},
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/qbic-pipelines/querynator",
-    version="0.3.3",
+    version="0.4.0",
     zip_safe=False,
 )
```

### Comparing `querynator-0.3.3/tests/test_querynator.py` & `querynator-0.4.0/tests/test_querynator.py`

 * *Files identical despite different names*

