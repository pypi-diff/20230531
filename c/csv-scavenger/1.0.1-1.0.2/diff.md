# Comparing `tmp/csv_scavenger-1.0.1.tar.gz` & `tmp/csv_scavenger-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_scavenger-1.0.1.tar", max compression
+gzip compressed data, was "csv_scavenger-1.0.2.tar", max compression
```

## Comparing `csv_scavenger-1.0.1.tar` & `csv_scavenger-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3034 2023-05-31 18:04:22.703660 csv_scavenger-1.0.1/csv-scavenger/scavenger.py
--rw-r--r--   0        0        0     1094 2023-05-31 15:26:00.843242 csv_scavenger-1.0.1/LICENSE
--rw-r--r--   0        0        0      542 2023-05-31 18:05:16.380886 csv_scavenger-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      667 2023-05-31 15:26:00.844244 csv_scavenger-1.0.1/README.md
--rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 csv_scavenger-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3034 2023-05-31 18:04:22.703660 csv_scavenger-1.0.2/csv-scavenger/scavenger.py
+-rw-r--r--   0        0        0     1094 2023-05-31 15:26:00.843242 csv_scavenger-1.0.2/LICENSE
+-rw-r--r--   0        0        0      542 2023-05-31 18:15:40.388167 csv_scavenger-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      663 2023-05-31 18:15:01.226065 csv_scavenger-1.0.2/README.md
+-rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 csv_scavenger-1.0.2/PKG-INFO
```

### Comparing `csv_scavenger-1.0.1/csv-scavenger/scavenger.py` & `csv_scavenger-1.0.2/csv-scavenger/scavenger.py`

 * *Files identical despite different names*

### Comparing `csv_scavenger-1.0.1/LICENSE` & `csv_scavenger-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_scavenger-1.0.1/pyproject.toml` & `csv_scavenger-1.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "csv-scavenger"
-version = "1.0.1"
+version = "1.0.2"
 description = "CSV reader and parser with automatic detection of delimiter and start/end of data."
 authors = ["Gustave Coulombe <magikgus@gmail.com>"]
 readme = "README.md"
 packages = [{include = "scavenger.py", from = "csv-scavenger"}]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
```

### Comparing `csv_scavenger-1.0.1/README.md` & `csv_scavenger-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 ```text
 pip install csv-scavenger
 ```
 
 ## Usage
 
 ```python
-import csv-scavenger as sv
+import scavenger as sv
 
 # Read a CSV file into a pandas DataFrame
 df = sv.read_csv('data.csv')
 ```
```

### Comparing `csv_scavenger-1.0.1/PKG-INFO` & `csv_scavenger-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv-scavenger
-Version: 1.0.1
+Version: 1.0.2
 Summary: CSV reader and parser with automatic detection of delimiter and start/end of data.
 Author: Gustave Coulombe
 Author-email: magikgus@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
@@ -22,13 +22,13 @@
 ```text
 pip install csv-scavenger
 ```
 
 ## Usage
 
 ```python
-import csv-scavenger as sv
+import scavenger as sv
 
 # Read a CSV file into a pandas DataFrame
 df = sv.read_csv('data.csv')
 ```
```

