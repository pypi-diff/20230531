# Comparing `tmp/datareuse-0.0.1.tar.gz` & `tmp/datareuse-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datareuse-0.0.1.tar", last modified: Wed May 31 12:49:28 2023, max compression
+gzip compressed data, was "datareuse-0.0.2.tar", last modified: Wed May 31 12:58:09 2023, max compression
```

## Comparing `datareuse-0.0.1.tar` & `datareuse-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:49:28.519732 datareuse-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 12:49:16.000000 datareuse-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-31 12:49:28.519732 datareuse-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-31 12:49:16.000000 datareuse-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:49:28.519732 datareuse-0.0.1/datareuse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-31 12:49:28.000000 datareuse-0.0.1/datareuse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-31 12:49:28.000000 datareuse-0.0.1/datareuse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:49:28.000000 datareuse-0.0.1/datareuse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-31 12:49:28.000000 datareuse-0.0.1/datareuse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 12:49:28.000000 datareuse-0.0.1/datareuse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:49:28.519732 datareuse-0.0.1/pyreuse/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 12:49:16.000000 datareuse-0.0.1/pyreuse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-31 12:49:16.000000 datareuse-0.0.1/pyreuse/reuse.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 12:49:28.519732 datareuse-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-31 12:49:16.000000 datareuse-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:49:28.519732 datareuse-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 12:49:16.000000 datareuse-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-31 12:49:16.000000 datareuse-0.0.1/tests/test_reuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:58:09.549194 datareuse-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 12:57:57.000000 datareuse-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-31 12:58:09.549194 datareuse-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-31 12:57:57.000000 datareuse-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:58:09.549194 datareuse-0.0.2/datareuse/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 12:57:57.000000 datareuse-0.0.2/datareuse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-31 12:57:57.000000 datareuse-0.0.2/datareuse/reuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:58:09.549194 datareuse-0.0.2/datareuse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-31 12:58:09.000000 datareuse-0.0.2/datareuse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-31 12:58:09.000000 datareuse-0.0.2/datareuse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:58:09.000000 datareuse-0.0.2/datareuse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-31 12:58:09.000000 datareuse-0.0.2/datareuse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 12:58:09.000000 datareuse-0.0.2/datareuse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 12:58:09.549194 datareuse-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-31 12:57:57.000000 datareuse-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:58:09.549194 datareuse-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 12:57:57.000000 datareuse-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-31 12:57:57.000000 datareuse-0.0.2/tests/test_reuse.py
```

### Comparing `datareuse-0.0.1/LICENSE` & `datareuse-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datareuse-0.0.1/PKG-INFO` & `datareuse-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datareuse
-Version: 0.0.1
+Version: 0.0.2
 Summary: Reuse computed datasets
 Author: Alexis Arnaudon
 Author-email: alexis.arnaudon@epfl.ch
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `datareuse-0.0.1/datareuse.egg-info/PKG-INFO` & `datareuse-0.0.2/datareuse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datareuse
-Version: 0.0.1
+Version: 0.0.2
 Summary: Reuse computed datasets
 Author: Alexis Arnaudon
 Author-email: alexis.arnaudon@epfl.ch
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `datareuse-0.0.1/pyreuse/reuse.py` & `datareuse-0.0.2/datareuse/reuse.py`

 * *Files identical despite different names*

### Comparing `datareuse-0.0.1/setup.py` & `datareuse-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "pytest-html",
 ]
 
 setup(
     name="datareuse",
     author="Alexis Arnaudon",
     author_email="alexis.arnaudon@epfl.ch",
-    version="0.0.1",
+    version="0.0.2",
     description="Reuse computed datasets",
     long_description=Path("README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     install_requires=[
         "pandas>=1.0.2",
     ],
     extras_require={
```

### Comparing `datareuse-0.0.1/tests/test_reuse.py` & `datareuse-0.0.2/tests/test_reuse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 from pathlib import Path
 import pytest
 
-from pyreuse import Reuse
+from datareuse import Reuse
 
 
 DATA = Path(__file__).parent
 
 
 def test_reuse(tmpdir):
     """Test reuse context manager."""
```

