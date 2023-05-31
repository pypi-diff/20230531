# Comparing `tmp/tdworkflow-0.7.0.tar.gz` & `tmp/tdworkflow-0.8.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdworkflow-0.7.0.tar", last modified: Wed May 25 03:07:32 2022, max compression
+gzip compressed data, was "tdworkflow-0.8.0rc0.tar", last modified: Wed May 31 04:08:05 2023, max compression
```

## Comparing `tdworkflow-0.7.0.tar` & `tdworkflow-0.8.0rc0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:32.257456 tdworkflow-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:32.253456 tdworkflow-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:32.253456 tdworkflow-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/.github/workflows/pythonapp.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1724 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11340 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4611 2022-05-25 03:07:32.257456 tdworkflow-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3791 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:32.253456 tdworkflow-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2020 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:32.253456 tdworkflow-0.7.0/docs/references/
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/docs/references/client.rst
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/docs/references/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/docs/references/misc.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/docs/references/model.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-05-25 03:07:32.257456 tdworkflow-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:32.253456 tdworkflow-0.7.0/tdworkflow/
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tdworkflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2532 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tdworkflow/attempt.py
--rw-r--r--   0 runner    (1001) docker     (121)    35917 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tdworkflow/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tdworkflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tdworkflow/log.py
--rw-r--r--   0 runner    (1001) docker     (121)      944 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tdworkflow/project.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tdworkflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tdworkflow/resource.py
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tdworkflow/revision.py
--rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tdworkflow/schedule.py
--rw-r--r--   0 runner    (1001) docker     (121)      892 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tdworkflow/session.py
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tdworkflow/task.py
--rw-r--r--   0 runner    (1001) docker     (121)     1630 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tdworkflow/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tdworkflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:32.257456 tdworkflow-0.7.0/tdworkflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4611 2022-05-25 03:07:32.000000 tdworkflow-0.7.0/tdworkflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-05-25 03:07:32.000000 tdworkflow-0.7.0/tdworkflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-25 03:07:32.000000 tdworkflow-0.7.0/tdworkflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-05-25 03:07:32.000000 tdworkflow-0.7.0/tdworkflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-05-25 03:07:32.000000 tdworkflow-0.7.0/tdworkflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:32.257456 tdworkflow-0.7.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:32.253456 tdworkflow-0.7.0/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:32.257456 tdworkflow-0.7.0/tests/resources/sample_project/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tests/resources/sample_project/.digdag
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:32.257456 tdworkflow-0.7.0/tests/resources/sample_project/ignore_dir/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tests/resources/sample_project/ignore_dir/dummy
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tests/resources/sample_project/main.dig
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:32.257456 tdworkflow-0.7.0/tests/resources/sample_project/py_scripts/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:32.257456 tdworkflow-0.7.0/tests/resources/sample_project/py_scripts/__ignoredir__/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tests/resources/sample_project/py_scripts/__ignoredir__/dummy
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tests/resources/sample_project/py_scripts/exec.py
--rw-r--r--   0 runner    (1001) docker     (121)    24529 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-05-25 03:07:20.000000 tdworkflow-0.7.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.920309 tdworkflow-0.8.0rc0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.924309 tdworkflow-0.8.0rc0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/.github/workflows/pythonapp.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.924309 tdworkflow-0.8.0rc0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.924309 tdworkflow-0.8.0rc0/docs/references/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/docs/references/client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/docs/references/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/docs/references/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/docs/references/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/tdworkflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/attempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37083 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/tdworkflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-31 04:08:05.000000 tdworkflow-0.8.0rc0/tdworkflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-31 04:08:05.000000 tdworkflow-0.8.0rc0/tdworkflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:08:05.000000 tdworkflow-0.8.0rc0/tdworkflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-31 04:08:05.000000 tdworkflow-0.8.0rc0/tdworkflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 04:08:05.000000 tdworkflow-0.8.0rc0/tdworkflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.920309 tdworkflow-0.8.0rc0/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/tests/resources/sample_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tests/resources/sample_project/.digdag
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/tests/resources/sample_project/ignore_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tests/resources/sample_project/ignore_dir/dummy
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tests/resources/sample_project/main.dig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/tests/resources/sample_project/py_scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/tests/resources/sample_project/py_scripts/__ignoredir__/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tests/resources/sample_project/py_scripts/__ignoredir__/dummy
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tests/resources/sample_project/py_scripts/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24529 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tests/test_util.py
```

### Comparing `tdworkflow-0.7.0/.github/workflows/pythonapp.yml` & `tdworkflow-0.8.0rc0/.github/workflows/pythonapp.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 name: Python application
 
 on: [push]
 
 jobs:
   build:
-    runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.7','3.8', '3.9', '3.10']
-
+        python-version: ['3.8', '3.9', '3.10', '3.11']
+        os: [ubuntu-latest, windows-latest]
+    runs-on: ${{ matrix.os }}
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[dev]
     - name: Lint
       run: |
         black --diff --check tdworkflow tests
         isort --check-only tdworkflow tests
+        mypy --install-types --non-interactive tdworkflow
     - name: Test with pytest
       run: |
         pytest
```

### Comparing `tdworkflow-0.7.0/.gitignore` & `tdworkflow-0.8.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.7.0/.readthedocs.yml` & `tdworkflow-0.8.0rc0/.readthedocs.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Read the Docs configuration file
 # See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
 
 # Required
 version: 2
 
+build:
+  os: ubuntu-22.04
+  tools:
+    python: "3.11"
+
 # Build documentation in the docs/ directory with Sphinx
 sphinx:
   configuration: docs/conf.py
 
-# Build documentation with MkDocs
-#mkdocs:
-#  configuration: mkdocs.yml
-
 # Optionally build your docs in additional formats such as PDF and ePub
 formats: []
 
 # Optionally set the version of Python and requirements required to build your docs
 python:
-  version: 3.7
   install:
     - method: pip
       path: .
       extra_requirements:
         - docs
```

### Comparing `tdworkflow-0.7.0/CHANGES.rst` & `tdworkflow-0.8.0rc0/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.7.0/LICENSE` & `tdworkflow-0.8.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.7.0/PKG-INFO` & `tdworkflow-0.8.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: tdworkflow
-Version: 0.7.0
+Version: 0.8.0rc0
 Summary: Unofficial Treasure Workflow API client
 Home-page: https://github.com/chezou/tdworkflow
 Author: Aki Ariga
 Author-email: chezou@gmail.com
 License: Apache License, Version 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Database
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
 
 tdwokflow
 =========
 
@@ -60,18 +59,18 @@
 
    client.set_secrets(projects[0], secrets)
 
    client.secrets(projects[0])
    # ['td.apikey', 'td.apiserver', "test"]
    client.delete_secrets(projects[0], ["test", "td.apiserver"])
 
-Uplaod Project from GitHub
+Upload Project from GitHub
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Before executing example code, you have to install git-python
+Before executing the example code, you have to install git-python
 
 .. code-block:: shell
 
    pip install gitpython
 
 Clone example repository with git-python and upload a digdag project.
 
@@ -120,22 +119,22 @@
        "eu01": "https://console.eu01.treasuredata.com/app/workflows",
        "jp": "https://console.treasuredata.co.jp/app/workflows",
    }
 
    workflows = client.project_workflows(project)
    workflows = list(filter(lambda w: w.name != "test", workflows))
    if workflows:
-       print(f"Project created! Open {CONSOLE_URL[site]}/{workflows[0].id}/info on your browser and clieck 'New Run' button.")
+       print(f"Project created! Open {CONSOLE_URL[site]}/{workflows[0].id}/info on your browser and click 'New Run' button.")
    else:
        print("Project creation failed.")
 
 Start workflow session
 ^^^^^^^^^^^^^^^^^^^^^^
 
-You can start workflow session by using ``Client.start_attempt``.
+You can start a workflow session by using ``Client.start_attempt``.
 
 .. code-block:: python
 
    attempt = client.start_attempt(workflows[0])
 
    # Wait attempt until finish. This may require few minutes.
    attempt = client.wait_attempt(attempt)
@@ -156,9 +155,7 @@
     >>> import tdworkflow
     >>> import requests
     >>> session = requests.Session()
     >>> client = tdworkflow.client.Client(
     ... endpoint="localhost:65432", apikey="", _session=session, scheme="http")
     >>> client.projects()
     [Project(id=1, name='python-tdworkflow', revision='134fe2f9-ded3-4e7c-af8e-8a82d55d688b', archiveType='db', archiveMd5='5Lc6F6m3DtmBN4DA5MzK8A==', createdAt='2019-11-01T13:03:26Z', deletedAt=None, updatedAt='2019-11-01T13:03:26Z')]
-
-
```

### Comparing `tdworkflow-0.7.0/README.rst` & `tdworkflow-0.8.0rc0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,18 @@
 
    client.set_secrets(projects[0], secrets)
 
    client.secrets(projects[0])
    # ['td.apikey', 'td.apiserver', "test"]
    client.delete_secrets(projects[0], ["test", "td.apiserver"])
 
-Uplaod Project from GitHub
+Upload Project from GitHub
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Before executing example code, you have to install git-python
+Before executing the example code, you have to install git-python
 
 .. code-block:: shell
 
    pip install gitpython
 
 Clone example repository with git-python and upload a digdag project.
 
@@ -96,22 +96,22 @@
        "eu01": "https://console.eu01.treasuredata.com/app/workflows",
        "jp": "https://console.treasuredata.co.jp/app/workflows",
    }
 
    workflows = client.project_workflows(project)
    workflows = list(filter(lambda w: w.name != "test", workflows))
    if workflows:
-       print(f"Project created! Open {CONSOLE_URL[site]}/{workflows[0].id}/info on your browser and clieck 'New Run' button.")
+       print(f"Project created! Open {CONSOLE_URL[site]}/{workflows[0].id}/info on your browser and click 'New Run' button.")
    else:
        print("Project creation failed.")
 
 Start workflow session
 ^^^^^^^^^^^^^^^^^^^^^^
 
-You can start workflow session by using ``Client.start_attempt``.
+You can start a workflow session by using ``Client.start_attempt``.
 
 .. code-block:: python
 
    attempt = client.start_attempt(workflows[0])
 
    # Wait attempt until finish. This may require few minutes.
    attempt = client.wait_attempt(attempt)
```

### Comparing `tdworkflow-0.7.0/docs/Makefile` & `tdworkflow-0.8.0rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.7.0/docs/conf.py` & `tdworkflow-0.8.0rc0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.7.0/docs/make.bat` & `tdworkflow-0.8.0rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.7.0/docs/references/model.rst` & `tdworkflow-0.8.0rc0/docs/references/model.rst`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.7.0/setup.cfg` & `tdworkflow-0.8.0rc0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
 	Operating System :: OS Independent
 	License :: OSI Approved :: Apache Software License
 	Topic :: Database
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 packages = find:
-python_requires = >= 3.7
+python_requires = >= 3.8
 install_requires = 
 	requests
 setup_requires = 
 	setuptools_scm
 
 [options.package_data]
 tdworkflow = py.typed
 
 [options.extras_require]
-dev = black;flake8;isort;pytest;pytest-mock
+dev = black;flake8;isort;pytest;pytest-mock;mypy
 doc = sphinx;sphinx_rtd_theme
 
 [flake8]
 ignore = E203, W503
 max-line-length = 88
 exclue = .git, .eggs, __pycache__, docs/, build/, dist/
```

### Comparing `tdworkflow-0.7.0/tdworkflow/attempt.py` & `tdworkflow-0.8.0rc0/tdworkflow/attempt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,77 @@
 import dataclasses
 from datetime import datetime
-from typing import Dict
+from typing import Any, Dict, Optional
 
 from .project import Project
 from .resource import Resource
 from .util import parse_iso8601
 from .workflow import Workflow
 
 
 @dataclasses.dataclass
 class Attempt(Resource):
     id: int
     sessionId: int = -1
     sessionUuid: str = ""
-    sessionTime: datetime = None
-    workflow: Workflow = None
-    project: Project = None
+    sessionTime: Optional[datetime] = None
+    workflow: Optional[Workflow] = None
+    project: Optional[Project] = None
     index: int = -1
     retryAttemptName: str = ""
     done: bool = False
     success: bool = False
     cancelRequested: bool = False
-    params: Dict = None
-    createdAt: datetime = None
-    finishedAt: datetime = None
+    params: Optional[Dict[str, Any]] = None
+    createdAt: Optional[datetime] = None
+    finishedAt: Optional[datetime] = None
     status: str = ""
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         self.id = int(self.id)
-        self.sessionTime = parse_iso8601(self.sessionTime)
+        self.sessionTime = parse_iso8601(self.sessionTime)  # type: ignore
         if self.project and isinstance(self.project, dict):
             self.project = Project(**self.project)
         if self.workflow and isinstance(self.workflow, dict):
             self.workflow = Workflow(**self.workflow)
         self.done = bool(self.done)
         self.success = bool(self.success)
         self.cancelRequested = bool(self.cancelRequested)
-        self.createdAt = parse_iso8601(self.createdAt)
-        self.finishedAt = parse_iso8601(self.finishedAt)
+        self.createdAt = parse_iso8601(self.createdAt)  # type: ignore
+        self.finishedAt = parse_iso8601(self.finishedAt)  # type: ignore
         self.status = self.status
 
     @property
-    def session_id(self):
+    def session_id(self) -> int:
         return self.sessionId
 
     @property
-    def session_uuid(self):
+    def session_uuid(self) -> str:
         return self.sessionUuid
 
     @property
-    def session_time(self):
+    def session_time(self) -> Optional[datetime]:
         return self.sessionTime
 
     @property
-    def retry_attempt_name(self):
+    def retry_attempt_name(self) -> str:
         return self.retryAttemptName
 
     @property
-    def cancel_requested(self):
+    def cancel_requested(self) -> bool:
         return self.cancelRequested
 
     @property
-    def finished_at(self):
+    def finished_at(self) -> Optional[datetime]:
         return self.finishedAt
 
-    def finished(self):
+    def finished(self) -> bool:
         return bool(self.finished_at)
 
-    def update(self, **args):
+    def update(self, **args: Any) -> None:
         other_attempt = Attempt(**args)
         self.id = other_attempt.id
         self.sessionId = other_attempt.sessionId
         self.sessionUuid = other_attempt.sessionUuid
         self.workflow = other_attempt.workflow
         self.project = other_attempt.project
         self.index = other_attempt.index
```

### Comparing `tdworkflow-0.7.0/tdworkflow/client.py` & `tdworkflow-0.8.0rc0/tdworkflow/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import io
 import json
 import logging
 import os
 import time
 import uuid
 from datetime import datetime
-from typing import Any, BinaryIO, Dict, List, Optional, Tuple, Union
+from typing import Any, BinaryIO, Callable, Dict, List, Optional, Tuple, Union, cast
 
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 import tdworkflow
 
@@ -25,14 +25,16 @@
 from .util import archive_files, to_iso8601
 from .workflow import Workflow
 
 logger = logging.getLogger(__name__)
 
 
 class WorkflowAPI:
+    get: Callable
+
     def workflows(
         self,
         name_pattern: Optional[str] = None,
         search_project_name: bool = False,
         order: Optional[str] = None,
         count: Optional[int] = None,
         last_id: Optional[int] = None,
@@ -48,15 +50,15 @@
         :param count: Number of workflows to return
         :type count: Optional[int], optional
         :param last_id: List workflows whose id is grater than this id for pagination.
         :type last_id: Optional[int], optional
         :return: List of Workflow
         :rtype: List[Workflow]
         """
-        params = {}
+        params = {}  # type: Dict[str, Union[str, bool, int, None]]
         if name_pattern:
             params["name_pattern"] = name_pattern
         if search_project_name:
             params["search_project_name"] = search_project_name
         if order:
             params["order"] = order
         if count:
@@ -79,14 +81,18 @@
         """
         workflow_id = workflow.id if isinstance(workflow, Workflow) else workflow
         res = self.get(f"workflows/{workflow_id}")
         return Workflow.from_api_repr(**res)
 
 
 class ProjectAPI:
+    get: Callable
+    put: Callable
+    delete: Callable
+
     def project(self, project: Union[int, Project]) -> Project:
         """Get a project
 
         :param project: Project id or Project object
         :type project: Union[int, Project]
         :return: A Project
         """
@@ -110,15 +116,15 @@
         :param count: Number of projects to return
         :type count: Optional[int], optional
         :param last_id: List projects whose id is grater than this id for pagination.
         :type last_id: Optional[int], optional
         :return: List of Project
         :rtype: List[Project]
         """
-        params = {}
+        params = {}  # type: Dict[str, Union[str, int, None]]
         if name:
             params["name"] = name
         if name_pattern:
             params["name_pattern"] = name_pattern
         if count:
             params["count"] = count
         if last_id:
@@ -143,15 +149,15 @@
         :param workflow: Workflow name or Workflow object
         :type project: Optional[Union[str, Workflow]], optional
         :param revision: Revision name
         :type revision: Optional[str], optional
         :return: List of Workflow
         :rtype: List[Workflow]
         """
-        params = {}
+        params = {}  # type: Dict[str, Union[str, int, None]]
         if workflow:
             workflow_name = (
                 workflow.name if isinstance(workflow, Workflow) else workflow
             )
             params["workflow"] = workflow_name
         if revision:
             params["revision"] = revision
@@ -273,15 +279,15 @@
         """List schedules associated with Project
 
         :param project: Project ID or project object
         :param workflow: Workflow name or Workflow object
         :param last_id: List schedules whose id is grater than this id for pagination
         :return: List of Schedule
         """
-        params = {}
+        params = {}  # type: Dict[str, Union[str, int, None]]
         if workflow:
             workflow_name = (
                 workflow.name if isinstance(workflow, Workflow) else workflow
             )
             params["workflow"] = workflow_name
         if last_id:
             params["last_id"] = last_id
@@ -389,15 +395,15 @@
 
         :param project: Project ID or Project object
         :param workflow: Workflow name or Workflow object
         :param last_id: List sessions whose id is grater than this id for pagination
         :param page_size: Number of sessions to return
         :return: List of Session
         """
-        params = {}
+        params = {}  # type: Dict[str, Union[str, int, None]]
         if workflow:
             workflow_name = (
                 workflow.name if isinstance(workflow, Workflow) else workflow
             )
             params["workflow"] = workflow_name
         if last_id:
             params["last_id"] = last_id
@@ -408,14 +414,18 @@
         if r:
             return [Session.from_api_repr(**s) for s in r["sessions"]]
         else:
             return []
 
 
 class AttemptAPI:
+    get: Callable
+    put: Callable
+    post: Callable
+
     def attempts(
         self,
         project: Optional[Union[str, Project]] = None,
         workflow: Optional[Union[str, Workflow]] = None,
         include_retried: Optional[bool] = None,
         last_id: Optional[int] = None,
         page_size: Optional[int] = None,
@@ -431,23 +441,23 @@
         :param last_id: List attempts whose id is grater than this id for pagination
         :type last_id: Optional[int]
         :param page_size: Number of attempts to return
         :type page_size: Optional[int]
         :return: List of Attempt object
         :rtype: List[Attempt]
         """
-        params = {}
+        params = {}  # type: Dict[str, Union[str, bool, int, None]]
         if project:
             project_name = project.name if isinstance(project, Project) else project
             params.update({"project": project_name})
         if workflow:
             workflow_name = (
                 workflow.name if isinstance(workflow, Workflow) else workflow
             )
-            params.upadte({"workflow": workflow_name})
+            params.update({"workflow": workflow_name})
         if include_retried:
             params.update({"include_retried": include_retried})
         if last_id:
             params.update({"last_id": last_id})
         if page_size:
             params.update({"page_size": page_size})
 
@@ -470,15 +480,19 @@
         """
         attempt_id = attempt.id if isinstance(attempt, Attempt) else attempt
         r = self.get(f"attempts/{attempt_id}")
         if not r:
             raise ValueError(f"Unable to find attempt id {attempt_id}")
 
         if inplace:
-            attempt.update(**r)
+            if isinstance(attempt, int):
+                raise ValueError(f"Unable to use inplace with integer value {attempt=}")
+            else:
+                attempt.update(**r)
+            return None
         else:
             return Attempt.from_api_repr(**r)
 
     def attempt_tasks(self, attempt: Union[int, Attempt]) -> List[Task]:
         """Get tasks of a session
 
         :param attempt: Attempt id or Attempt object
@@ -514,15 +528,17 @@
         :param workflow: Workflow id or Workflow object
         :param session_time: Session time, optional Default: ``datetime.datetime.now()``
         :param retry_attempt_name: Retry attempt name, optional
         :param workflow_params: Extra workflow parameters
         :return:
         """
         workflow_id = workflow.id if isinstance(workflow, Workflow) else workflow
-        _params = {"workflowId": workflow_id}
+        _params = {
+            "workflowId": workflow_id
+        }  # type: Dict[str, Union[str, int, Dict, None]]
         workflow_params = workflow_params if workflow_params else {}
         _params.update({"params": workflow_params})
         if not session_time:
             session_time = to_iso8601(datetime.now())
         if retry_attempt_name:
             _params.update({"retryAttemptName": retry_attempt_name})
 
@@ -544,14 +560,15 @@
         :return: ``True`` if succeeded
         :rtype: Attempt
         """
         attempt_id = attempt.id if isinstance(attempt, Attempt) else attempt
         self.post(f"attempts/{attempt_id}/kill", content=True)
         if inplace:
             self.attempt(attempt, inplace=True)
+            return None
         else:
             return self.attempt(attempt)
 
     def wait_attempt(
         self, attempt: Union[int, Attempt], wait_interval: int = 5
     ) -> Attempt:
         """Wait until an attempt finished
@@ -559,22 +576,28 @@
         :param attempt: Attempt ID or Attempt object
         :type attempt: Union[int, Attempt]
         :param wait_interval: Wait interval in second. Default 5 sec
         :type wait_interval: int
         :return: Latest status of Attempt
         :rtype: Attempt
         """
+        if isinstance(attempt, int):
+            attempt = cast(Attempt, self.attempt(attempt))
+
         while not attempt.done:
             time.sleep(wait_interval)
             self.attempt(attempt, inplace=True)
 
         return attempt
 
 
 class ScheduleAPI:
+    get: Callable
+    post: Callable
+
     def schedules(self, last_id: Optional[int] = None) -> List[Schedule]:
         """List schedules
 
         :param last_id: List schedules whose id is grater than this id for pagination.
         :return: List of Schedule
         """
         r = self.get("schedules", params={"last_id": last_id})
@@ -610,15 +633,15 @@
         :param attempt_name: Attempt name
         :param from_time: From time e.g "2019-11-01T06:20:07.000+00:00" in ``str`` or
                           :class:`datetime.datetime`.
         :param dry_run: Flag for dry run
         :param count: Count
         :return: ScheduleAttempt
         """
-        params = {}
+        params = {}  # type: Dict[str, Union[str, int, None]]
         if from_time:
             params["fromTime"] = to_iso8601(from_time)
         if attempt_name:
             params["attemptName"] = attempt_name
         if count:
             params["count"] = count
         params["dryRun"] = dry_run
@@ -669,15 +692,15 @@
         :param schedule: Schedule ID or Schedule object
         :param from_time: From time
         :param next_time: Next time
         :param next_run_time: Next run time
         :param dry_run: Flag for dry run
         :return: New Schedule
         """
-        params = {}
+        params = {}  # type: Dict[str, Union[str, datetime, bool, None]]
         if from_time:
             params["fromTime"] = to_iso8601(from_time)
         if next_time:
             params["nextTime"] = next_time
         if next_run_time:
             params["nextRunTime"] = to_iso8601(next_run_time)
         params["dryRun"] = dry_run
@@ -686,14 +709,16 @@
         if r:
             return Schedule.from_api_repr(**r)
         else:
             raise ValueError(f"Unable to skip schedule id: {schedule_id}")
 
 
 class SessionAPI:
+    get: Callable
+
     def sessions(
         self, last_id: Optional[int] = None, page_size: Optional[int] = None
     ) -> List[Session]:
         """List sessions
 
         :param last_id: List sessions whose id is grater than this id for pagination
         :param page_size: Number of sessions to return
@@ -748,41 +773,45 @@
         if r:
             return [Attempt.from_api_repr(**e) for e in r["attempts"]]
         else:
             return []
 
 
 class LogAPI:
+    get: Callable
+
     def log_files(
         self,
         attempt: Union[Attempt, int],
         task: Optional[str] = None,
         direct_download: Optional[bool] = None,
     ) -> List[LogFile]:
         """Get log files information
 
         :param attempt: Target Attempt id or Attempt object
         :param task: Task name
         :param direct_download: Flag for direct download
         :return: List of LogFile
         """
-        params = {}
+        params = {}  # type: Dict[str, Union[int, str, bool, None]]
         if task:
             params["task"] = task
         if direct_download:
             params["direct_download"] = True
 
         attempt_id = attempt.id if isinstance(attempt, Attempt) else attempt
         r = self.get(f"logs/{attempt_id}/files")
         if r:
             return [LogFile.from_api_repr(**l) for l in r["files"]]
         else:
             return []
 
-    def log_file(self, attempt: Union[Attempt, int], file: Union[LogFile, str]) -> str:
+    def log_file(
+        self, attempt: Union[Attempt, int], file: Union[LogFile, str]
+    ) -> Union[bytes, str]:
         """Get a log string for an attempt
 
         :param attempt: Target Attempt id or Attempt object
         :param file: LogFile name or LogFile object
         :return: Log string
         """
 
@@ -792,15 +821,15 @@
         if r:
             gzfile = io.BytesIO(r)
             with gzip.open(gzfile, "rt") as f:
                 return f.read()
         else:
             raise ValueError(f"Unable to get file: {file_name}")
 
-    def logs(self, attempt: Union[Attempt, int]) -> List[str]:
+    def logs(self, attempt: Union[Attempt, int]) -> List[Union[bytes, str]]:
         """Get log string list for an attempt
 
         :param attempt: Attempt ID or Attempt object
         :return: A list of log
 
 
         .. code-block:: python
@@ -896,15 +925,15 @@
         _session.mount("https://", HTTPAdapter(max_retries=retries))
         _session.mount("http://", HTTPAdapter(max_retries=retries))
 
         self._http = _session
         self.api_base = f"{scheme}://{self.endpoint}/api/"
 
     @property
-    def http(self):
+    def http(self) -> requests.Session:
         """
         :return: Established session
         :rtype: requests.Session
         """
         return self._http
 
     def get(
@@ -919,15 +948,15 @@
         :param content: Return content body without parsing JSON if ``True``
         :type content: bool
         :return: Response data in JSON or bytes
         :rtype: Union[Dict[str, str], bytes]
         """
         url = f"{self.api_base}{path}"
         r = self.http.get(url, params=params)
-        logger.debug(f"{r.status_code}\n{r.content}")
+        logger.debug(f"{r.status_code!r}\n{r.content!r}")
 
         if not 200 <= r.status_code < 300:
             exceptions.raise_response_error(r)
 
         if content:
             return r.content
         else:
@@ -944,37 +973,39 @@
         :type body: Optional[Dict[str, str]], optional
         :param content: Return content body without parsing JSON if ``True``
         :type content: bool
         :return: ``True`` if succeeded
         """
         url = f"{self.api_base}{path}"
         r = self.http.post(url, json=body)
-        logger.debug(f"{r.status_code}\n{r.content}")
+        logger.debug(f"{r.status_code!r}\n{r.content!r}")
 
         if not 200 <= r.status_code < 300:
             exceptions.raise_response_error(r)
 
         if content:
             return r.content
         elif r.content and "application/json" in r.headers.get("Content-Type", ""):
             return r.json()
 
+        return None
+
     def put(
         self,
         path: str,
-        data: Optional[Union[Dict, List[Tuple], BinaryIO]] = None,
+        data: Optional[Union[str, Dict, List[Tuple], BinaryIO]] = None,
         _json: Optional[Dict[str, str]] = None,
         params: Optional[Dict[str, str]] = None,
     ) -> Optional[Dict[str, str]]:
         """PUT operator for REST API
 
         :param path: Treasure Workflow API path
         :type path: str
         :param data: Content body
-        :type data: Optional[Union[Dict, List[Tuple], BinaryIO]], oprional
+        :type data: Optional[str, Union[Dict, List[Tuple], BinaryIO]], optional
         :param _json: Content body as JSON
         :type _json: Optional[Dict[str, str]], optional
         :param params: Query parameters
         :type params: Optional[Dict[str, str]], optional
         :return: Response content
         :rtype: Dict[str,str]
         """
@@ -982,23 +1013,25 @@
         headers = {}
         if _json:
             headers["Content-Type"] = "application/json"
             data = json.dumps(_json)
         if not _json and data and hasattr(data, "read"):
             headers["Content-Type"] = "application/gzip"
 
-        r = self.http.put(url, data=data, headers=headers, params=params)
-        logger.debug(f"{r.status_code}\n{r.content}")
+        r = self.http.put(url, data=data, headers=headers, params=params)  # type: ignore
+        logger.debug(f"{r.status_code!r}\n{r.content!r}")
 
         if not 200 <= r.status_code < 300:
             exceptions.raise_response_error(r)
 
         if r.content and "application/json" in r.headers.get("Content-Type", ""):
             return r.json()
 
+        return None
+
     def delete(
         self, path: str, params: Optional[Dict[str, str]] = None
     ) -> Optional[Dict[str, str]]:
         """DELETE operator for REST API
 
         :param path: Treasure Workflow API path
         :type path: str
@@ -1006,14 +1039,16 @@
         :type params: Optional[Dict[str, str]], optional
         :return: ``True`` if succeeded
         :rtype: bool
         """
         url = f"{self.api_base}{path}"
 
         r = self.http.delete(url, params=params)
-        logger.debug(f"{r.status_code}\n{r.content}")
+        logger.debug(f"{r.status_code!r}\n{r.content!r}")
 
         if not 200 <= r.status_code < 300:
             exceptions.raise_response_error(r)
 
         if r.content and "application/json" in r.headers.get("Content-Type", ""):
             return r.json()
+
+        return None
```

### Comparing `tdworkflow-0.7.0/tdworkflow/log.py` & `tdworkflow-0.8.0rc0/tdworkflow/log.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import dataclasses
 from datetime import datetime
-from typing import Dict
+from typing import Any, Dict, Optional
 
 from .resource import Resource
 from .util import parse_iso8601
 
 
 @dataclasses.dataclass
 class LogFile(Resource):
     fileName: str
     taskName: str
-    direct: Dict
+    direct: Dict[Any, Any]
     fileSize: int
     agentId: str
-    fileTime: datetime = None
+    fileTime: Optional[datetime] = None
 
-    def __post_init__(self):
-        self.fileTime = parse_iso8601(self.fileTime)
+    def __post_init__(self) -> None:
+        self.fileTime = parse_iso8601(self.fileTime)  # type: ignore
 
     @property
-    def file_name(self):
+    def file_name(self) -> str:
         return self.fileName
 
     @property
-    def taks_name(self):
+    def taks_name(self) -> str:
         return self.taskName
 
     @property
-    def file_time(self):
+    def file_time(self) -> Optional[datetime]:
         return self.fileTime
 
     @property
-    def file_size(self):
+    def file_size(self) -> int:
         return self.fileSize
 
     @property
-    def agent_id(self):
+    def agent_id(self) -> str:
         return self.agentId
```

### Comparing `tdworkflow-0.7.0/tdworkflow/schedule.py` & `tdworkflow-0.8.0rc0/tdworkflow/schedule.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 import dataclasses
 from datetime import datetime
-from typing import Dict, List
+from typing import Any, Dict, List, Optional, Union
 
 from .attempt import Attempt
 from .project import Project
 from .resource import Resource
 from .util import parse_iso8601
 from .workflow import Workflow
 
+NextSchedule = Dict[str, Union[int, str, Dict[str, Any]]]
+
 
 @dataclasses.dataclass
 class Schedule(Resource):
     id: int
     project: Project
     workflow: Workflow
-    createdAt: datetime = None
-    updatedAt: datetime = None
-    disabledAt: datetime = None
-    nextScheduleTime: Dict = None
-    nextRunTime: datetime = None
+    createdAt: Optional[datetime] = None
+    updatedAt: Optional[datetime] = None
+    disabledAt: Optional[datetime] = None
+    nextScheduleTime: Optional[NextSchedule] = None
+    nextRunTime: Optional[datetime] = None
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         self.id = int(self.id)
-        self.project = Project(**self.project)
-        self.workflow = Workflow(**self.workflow)
-        self.createdAt = parse_iso8601(self.createdAt)
-        self.updatedAt = parse_iso8601(self.updatedAt)
-        self.disabledAt = parse_iso8601(self.disabledAt)
-        self.nextRunTime = parse_iso8601(self.nextRunTime)
+        self.project = Project(**self.project)  # type: ignore
+        self.workflow = Workflow(**self.workflow)  # type: ignore
+        self.createdAt = parse_iso8601(self.createdAt)  # type: ignore
+        self.updatedAt = parse_iso8601(self.updatedAt)  # type: ignore
+        self.disabledAt = parse_iso8601(self.disabledAt)  # type: ignore
+        self.nextRunTime = parse_iso8601(self.nextRunTime)  # type: ignore
 
     @property
-    def created_at(self):
+    def created_at(self) -> Optional[datetime]:
         return self.createdAt
 
     @property
-    def updated_at(self):
+    def updated_at(self) -> Optional[datetime]:
         return self.updatedAt
 
     @property
-    def disabled_at(self):
+    def disabled_at(self) -> Optional[datetime]:
         return self.disabledAt
 
     @property
-    def next_run_time(self):
+    def next_run_time(self) -> Optional[datetime]:
         return self.nextRunTime
 
     @property
-    def next_schedule_time(self):
+    def next_schedule_time(self) -> Optional[NextSchedule]:
         return self.nextScheduleTime
 
 
 @dataclasses.dataclass
 class ScheduleAttempt(Resource):
     id: int
     attempts: List[Attempt]
-    project: Project = None
-    workflow: Workflow = None
+    project: Optional[Project] = None
+    workflow: Optional[Workflow] = None
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         self.id = int(self.id)
-        self.attempts = [Attempt(**att) for att in self.attempts]
-        self.project = Project(**self.project)
-        self.workflow = Project(**self.workflow)
+        self.attempts = [Attempt(**att) for att in self.attempts]  # type: ignore
+        self.project = Project(**self.project)  # type: ignore
+        self.workflow = Project(**self.workflow)  # type: ignore
```

### Comparing `tdworkflow-0.7.0/tdworkflow/session.py` & `tdworkflow-0.8.0rc0/tdworkflow/session.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import dataclasses
 from datetime import datetime
+from typing import Optional
 
 from .attempt import Attempt
 from .project import Project
 from .resource import Resource
 from .util import parse_iso8601
 from .workflow import Workflow
 
 
 @dataclasses.dataclass
 class Session(Resource):
     id: int
     project: Project
     workflow: Workflow
     sessionUuid: str
-    sessionTime: datetime = None
-    lastAttempt: Attempt = None
+    sessionTime: Optional[datetime] = None
+    lastAttempt: Optional[Attempt] = None
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         self.id = int(self.id)
-        self.project = Project(**self.project)
-        self.workflow = Workflow(**self.workflow)
-        self.sessionTime = parse_iso8601(self.sessionTime)
-        self.lastAttempt = Attempt(**self.lastAttempt)
+        self.project = Project(**self.project)  # type: ignore
+        self.workflow = Workflow(**self.workflow)  # type: ignore
+        self.sessionTime = parse_iso8601(self.sessionTime)  # type: ignore
+        self.lastAttempt = Attempt(**self.lastAttempt)  # type: ignore
 
     @property
-    def session_uuid(self):
+    def session_uuid(self) -> str:
         return self.sessionUuid
 
     @property
-    def session_time(self):
+    def session_time(self) -> Optional[datetime]:
         return self.session_time
 
     @property
-    def last_attempt(self):
+    def last_attempt(self) -> Optional[Attempt]:
         return self.lastAttempt
```

### Comparing `tdworkflow-0.7.0/tdworkflow/task.py` & `tdworkflow-0.8.0rc0/tdworkflow/project.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,44 @@
 import dataclasses
-import json
 from datetime import datetime
-from typing import Dict, List
+from typing import Optional
 
 from .resource import Resource
 from .util import parse_iso8601
 
 
 @dataclasses.dataclass
-class Task(Resource):
+class Project(Resource):
     id: int
-    state: str
-    updatedAt: datetime = None
-    fullName: str = ""
-    parentId: int = None
-    upstreams: List[int] = None
-    retryAt: datetime = None
-    config: Dict = None
-    exportParams: Dict = None
-    storeParams: Dict = None
-    stateParams: Dict = None
-    error: Dict = None
-    startedAt: datetime = None
-    cancelRequested: bool = False
-    isGroup: bool = False
+    name: str
+    revision: str = ""
+    archiveType: str = ""
+    archiveMd5: str = ""
+    createdAt: Optional[datetime] = None
+    deletedAt: Optional[datetime] = None
+    updatedAt: Optional[datetime] = None
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         self.id = int(self.id)
-        self.updatedAt = parse_iso8601(self.updatedAt)
-        self.parentId = int(self.parentId) if self.parentId else None
-        self.upstreams = [int(_id) for _id in self.upstreams]
-        self.retryAt = parse_iso8601(self.retryAt)
-        self.startedAt = parse_iso8601(self.startedAt)
+        self.createdAt = parse_iso8601(self.createdAt)  # type: ignore
+        self.deletedAt = parse_iso8601(self.deletedAt)  # type: ignore
+        self.updatedAt = parse_iso8601(self.updatedAt)  # type: ignore
 
     @property
-    def updated_at(self):
-        return self.updatedAt
-
-    @property
-    def full_name(self):
-        return self.fullName
-
-    @property
-    def parent_id(self):
-        return self.parentId
-
-    @property
-    def retry_at(self):
-        return self.retryAt
+    def archive_type(self) -> str:
+        return self.archiveType
 
     @property
-    def export_params(self):
-        return self.exportParams
+    def archive_md5(self) -> str:
+        return self.archive_md5
 
     @property
-    def store_params(self):
-        return self.storeParams
+    def created_at(self) -> Optional[datetime]:
+        return self.createdAt
 
     @property
-    def state_params(self):
-        return self.stateParams
+    def deleted_at(self) -> Optional[datetime]:
+        return self.deletedAt
 
     @property
-    def started_at(self):
-        return self.startedAt
-
-    @property
-    def cancel_requested(self):
-        return self.cancelRequested
-
-    @property
-    def group(self):
-        return self.isGroup
-
-
-class TaskEncoder(json.JSONEncoder):
-    def default(self, obj):
-        if isinstance(obj, Task):
-            return obj.__dict__
-        return json.JSONEncoder.default(self, obj)
+    def updated_at(self) -> Optional[datetime]:
+        return self.updatedAt
```

### Comparing `tdworkflow-0.7.0/tdworkflow/util.py` & `tdworkflow-0.8.0rc0/tdworkflow/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,52 @@
-import glob
 import io
 import logging
 import os
 import re
 import tarfile
 from datetime import datetime, timedelta, timezone
-from typing import List, Optional
+from pathlib import Path
+from typing import List, Optional, Union
 
 logger = logging.getLogger(__name__)
 
 
-def exclude_files(pattern):
-    def _filter(tarinfo):
-        if re.search(pattern, tarinfo.name) or os.path.basename(
-            tarinfo.name
-        ).startswith("."):
-            return None
-        else:
-            return tarinfo
-
-    return _filter
-
-
 def archive_files(target_dir: str, exclude_patterns: List[str]) -> io.BytesIO:
     _partial = r")|(".join(exclude_patterns)
     pattern = rf"({_partial})"
 
+    target_dir_path = Path(target_dir)
     _bytes = io.BytesIO()
     with tarfile.open(mode="w:gz", fileobj=_bytes) as tar:
-        for fn in glob.glob(os.path.join(target_dir, "**"), recursive=True):
-            if not re.search(pattern, fn) and os.path.basename(fn) != "":
-                write_fn = fn.replace(f"{target_dir}/", "")
-                logger.info(f"Added {fn} as {write_fn}")
-                tar.add(fn, write_fn, recursive=False)
+        for current_dir, directories, files in os.walk(target_dir_path):
+            for file_or_dir in [*directories, *files]:
+                file_path = Path(os.path.join(current_dir, file_or_dir))
+                if re.search(pattern, str(file_path)) or file_or_dir.startswith("."):
+                    continue
+                relative_path = file_path.relative_to(target_dir_path)
+                logger.info(f"Added {file_path} as {relative_path}")
+                tar.add(
+                    file_path,
+                    relative_path,
+                    recursive=False,
+                )
 
     _bytes.seek(0)
     return _bytes
 
 
-def parse_iso8601(target: str) -> Optional[datetime]:
+def parse_iso8601(target: Optional[str]) -> Optional[datetime]:
     if not target:
         return None
 
     return datetime.fromisoformat(target.replace("Z", "+00:00"))
 
 
-def to_iso8601(dt: datetime) -> str:
-    if not datetime:
+def to_iso8601(dt: Optional[Union[str, datetime]]) -> str:
+    if not dt:
         return ""
 
     if isinstance(dt, datetime):
         # Naive object
         if not dt.tzinfo:
             return dt.astimezone(timezone(timedelta(0), "UTC")).isoformat()
         # Aware object
```

### Comparing `tdworkflow-0.7.0/tdworkflow.egg-info/PKG-INFO` & `tdworkflow-0.8.0rc0/tdworkflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: tdworkflow
-Version: 0.7.0
+Version: 0.8.0rc0
 Summary: Unofficial Treasure Workflow API client
 Home-page: https://github.com/chezou/tdworkflow
 Author: Aki Ariga
 Author-email: chezou@gmail.com
 License: Apache License, Version 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Database
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
 
 tdwokflow
 =========
 
@@ -60,18 +59,18 @@
 
    client.set_secrets(projects[0], secrets)
 
    client.secrets(projects[0])
    # ['td.apikey', 'td.apiserver', "test"]
    client.delete_secrets(projects[0], ["test", "td.apiserver"])
 
-Uplaod Project from GitHub
+Upload Project from GitHub
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Before executing example code, you have to install git-python
+Before executing the example code, you have to install git-python
 
 .. code-block:: shell
 
    pip install gitpython
 
 Clone example repository with git-python and upload a digdag project.
 
@@ -120,22 +119,22 @@
        "eu01": "https://console.eu01.treasuredata.com/app/workflows",
        "jp": "https://console.treasuredata.co.jp/app/workflows",
    }
 
    workflows = client.project_workflows(project)
    workflows = list(filter(lambda w: w.name != "test", workflows))
    if workflows:
-       print(f"Project created! Open {CONSOLE_URL[site]}/{workflows[0].id}/info on your browser and clieck 'New Run' button.")
+       print(f"Project created! Open {CONSOLE_URL[site]}/{workflows[0].id}/info on your browser and click 'New Run' button.")
    else:
        print("Project creation failed.")
 
 Start workflow session
 ^^^^^^^^^^^^^^^^^^^^^^
 
-You can start workflow session by using ``Client.start_attempt``.
+You can start a workflow session by using ``Client.start_attempt``.
 
 .. code-block:: python
 
    attempt = client.start_attempt(workflows[0])
 
    # Wait attempt until finish. This may require few minutes.
    attempt = client.wait_attempt(attempt)
@@ -156,9 +155,7 @@
     >>> import tdworkflow
     >>> import requests
     >>> session = requests.Session()
     >>> client = tdworkflow.client.Client(
     ... endpoint="localhost:65432", apikey="", _session=session, scheme="http")
     >>> client.projects()
     [Project(id=1, name='python-tdworkflow', revision='134fe2f9-ded3-4e7c-af8e-8a82d55d688b', archiveType='db', archiveMd5='5Lc6F6m3DtmBN4DA5MzK8A==', createdAt='2019-11-01T13:03:26Z', deletedAt=None, updatedAt='2019-11-01T13:03:26Z')]
-
-
```

### Comparing `tdworkflow-0.7.0/tdworkflow.egg-info/SOURCES.txt` & `tdworkflow-0.8.0rc0/tdworkflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.7.0/tests/test_client.py` & `tdworkflow-0.8.0rc0/tests/test_client.py`

 * *Files identical despite different names*

