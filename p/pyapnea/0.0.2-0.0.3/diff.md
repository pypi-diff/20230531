# Comparing `tmp/pyapnea-0.0.2.tar.gz` & `tmp/pyapnea-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyapnea-0.0.2.tar", last modified: Tue May 23 15:49:00 2023, max compression
+gzip compressed data, was "pyapnea-0.0.3.tar", last modified: Wed May 31 14:31:30 2023, max compression
```

## Comparing `pyapnea-0.0.2.tar` & `pyapnea-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:49:00.854722 pyapnea-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-23 15:48:40.000000 pyapnea-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-23 15:49:00.854722 pyapnea-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-23 15:48:40.000000 pyapnea-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-23 15:48:40.000000 pyapnea-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 15:49:00.854722 pyapnea-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:49:00.854722 pyapnea-0.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:48:40.000000 pyapnea-0.0.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:49:00.854722 pyapnea-0.0.2/src/pyapnea/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 15:48:40.000000 pyapnea-0.0.2/src/pyapnea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-23 15:48:40.000000 pyapnea-0.0.2/src/pyapnea/base_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:49:00.854722 pyapnea-0.0.2/src/pyapnea/oscar/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-23 15:48:40.000000 pyapnea-0.0.2/src/pyapnea/oscar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-23 15:48:40.000000 pyapnea-0.0.2/src/pyapnea/oscar/data_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-05-23 15:48:40.000000 pyapnea-0.0.2/src/pyapnea/oscar/oscar_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-23 15:48:40.000000 pyapnea-0.0.2/src/pyapnea/oscar/oscar_getter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-23 15:48:40.000000 pyapnea-0.0.2/src/pyapnea/oscar/oscar_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:49:00.854722 pyapnea-0.0.2/src/pyapnea.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-23 15:49:00.000000 pyapnea-0.0.2/src/pyapnea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-23 15:49:00.000000 pyapnea-0.0.2/src/pyapnea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:49:00.000000 pyapnea-0.0.2/src/pyapnea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 15:49:00.000000 pyapnea-0.0.2/src/pyapnea.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:31:30.334116 pyapnea-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 14:31:11.000000 pyapnea-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-31 14:31:30.334116 pyapnea-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-31 14:31:11.000000 pyapnea-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-31 14:31:11.000000 pyapnea-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:31:30.334116 pyapnea-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:31:30.334116 pyapnea-0.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:31:11.000000 pyapnea-0.0.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:31:30.334116 pyapnea-0.0.3/src/pyapnea/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 14:31:11.000000 pyapnea-0.0.3/src/pyapnea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-31 14:31:11.000000 pyapnea-0.0.3/src/pyapnea/base_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:31:30.334116 pyapnea-0.0.3/src/pyapnea/oscar/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-31 14:31:11.000000 pyapnea-0.0.3/src/pyapnea/oscar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-31 14:31:11.000000 pyapnea-0.0.3/src/pyapnea/oscar/data_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-05-31 14:31:11.000000 pyapnea-0.0.3/src/pyapnea/oscar/oscar_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-31 14:31:11.000000 pyapnea-0.0.3/src/pyapnea/oscar/oscar_getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-31 14:31:11.000000 pyapnea-0.0.3/src/pyapnea/oscar/oscar_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:31:30.334116 pyapnea-0.0.3/src/pyapnea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-31 14:31:30.000000 pyapnea-0.0.3/src/pyapnea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-31 14:31:30.000000 pyapnea-0.0.3/src/pyapnea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:31:30.000000 pyapnea-0.0.3/src/pyapnea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 14:31:30.000000 pyapnea-0.0.3/src/pyapnea.egg-info/top_level.txt
```

### Comparing `pyapnea-0.0.2/LICENSE` & `pyapnea-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyapnea-0.0.2/PKG-INFO` & `pyapnea-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyapnea
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package related to Apnea data analysis
 Author-email: Julien Laumonier <julien.laumonier@iid.ulaval.ca>
 Project-URL: Homepage, https://github.com/iid-ulaval/pyapnea
 Project-URL: Bug Tracker, https://github.com/iid-ulaval/pyapnea/issues
 Project-URL: Documentation, https://pyapnea.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PyApnea v0.1.1
+# PyApnea v0.0.3
 
 Python package related to apnea data analysis.
 
 This version contains functions to read session files from OSCAR software (https://www.sleepfiles.com/OSCAR/)
 
 Documentation can be found on [ReadTheDocs](https://pyapnea.readthedocs.io/en/latest/)
```

### Comparing `pyapnea-0.0.2/pyproject.toml` & `pyapnea-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0", "pandas>=2.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyapnea"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Julien Laumonier", email="julien.laumonier@iid.ulaval.ca" },
 ]
 description = "Python package related to Apnea data analysis"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pyapnea-0.0.2/src/pyapnea/base_functions.py` & `pyapnea-0.0.3/src/pyapnea/base_functions.py`

 * *Files identical despite different names*

### Comparing `pyapnea-0.0.2/src/pyapnea/oscar/data_structure.py` & `pyapnea-0.0.3/src/pyapnea/oscar/data_structure.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Data structure for an Oscar session. Follow the structure of the file described in the following image:
+Data structure for an Oscar session. It follows the structure of the file described in the following image:
 
 ![image](images/oscar_format.drawio.png)
 """
 from dataclasses import dataclass, field
 
 
 @dataclass
```

### Comparing `pyapnea-0.0.2/src/pyapnea/oscar/oscar_constants.py` & `pyapnea-0.0.3/src/pyapnea/oscar/oscar_constants.py`

 * *Files identical despite different names*

### Comparing `pyapnea-0.0.2/src/pyapnea/oscar/oscar_loader.py` & `pyapnea-0.0.3/src/pyapnea/oscar/oscar_loader.py`

 * *Files identical despite different names*

### Comparing `pyapnea-0.0.2/src/pyapnea.egg-info/PKG-INFO` & `pyapnea-0.0.3/src/pyapnea.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyapnea
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python package related to Apnea data analysis
 Author-email: Julien Laumonier <julien.laumonier@iid.ulaval.ca>
 Project-URL: Homepage, https://github.com/iid-ulaval/pyapnea
 Project-URL: Bug Tracker, https://github.com/iid-ulaval/pyapnea/issues
 Project-URL: Documentation, https://pyapnea.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PyApnea v0.1.1
+# PyApnea v0.0.3
 
 Python package related to apnea data analysis.
 
 This version contains functions to read session files from OSCAR software (https://www.sleepfiles.com/OSCAR/)
 
 Documentation can be found on [ReadTheDocs](https://pyapnea.readthedocs.io/en/latest/)
```

