# Comparing `tmp/csv_scavenger-1.0.0.tar.gz` & `tmp/csv_scavenger-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_scavenger-1.0.0.tar", max compression
+gzip compressed data, was "csv_scavenger-1.0.1.tar", max compression
```

## Comparing `csv_scavenger-1.0.0.tar` & `csv_scavenger-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3014 2023-05-31 15:26:00.856237 csv_scavenger-1.0.0/csv-scavenger/main.py
--rw-r--r--   0        0        0     1094 2023-05-31 15:26:00.843242 csv_scavenger-1.0.0/LICENSE
--rw-r--r--   0        0        0      537 2023-05-31 17:38:40.053094 csv_scavenger-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      667 2023-05-31 15:26:00.844244 csv_scavenger-1.0.0/README.md
--rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 csv_scavenger-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3034 2023-05-31 18:04:22.703660 csv_scavenger-1.0.1/csv-scavenger/scavenger.py
+-rw-r--r--   0        0        0     1094 2023-05-31 15:26:00.843242 csv_scavenger-1.0.1/LICENSE
+-rw-r--r--   0        0        0      542 2023-05-31 18:05:16.380886 csv_scavenger-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      667 2023-05-31 15:26:00.844244 csv_scavenger-1.0.1/README.md
+-rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 csv_scavenger-1.0.1/PKG-INFO
```

### Comparing `csv_scavenger-1.0.0/csv-scavenger/main.py` & `csv_scavenger-1.0.1/csv-scavenger/scavenger.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,13 +73,13 @@
             f"CSV data is not in a recognized format. Detected delimiter is: {csv_format[0]}"
         )
 
     return data
 
 
 if __name__ == "__main__":
-    data_people = read_csv("simplecsv/example_csvs/people.csv")
-    data_faithful = read_csv("simplecsv/example_csvs/faithful.csv")
-    data_orgs = read_csv("simplecsv/example_csvs/orgs.csv")
-    data_health = read_csv("simplecsv/example_csvs/health.csv")
-    data_multimeter = read_csv("simplecsv/example_csvs/multimeter.csv")
+    data_people = read_csv("csv-scavenger/example_csvs/people.csv")
+    data_faithful = read_csv("csv-scavenger/example_csvs/faithful.csv")
+    data_orgs = read_csv("csv-scavenger/example_csvs/orgs.csv")
+    data_health = read_csv("csv-scavenger/example_csvs/health.csv")
+    data_multimeter = read_csv("csv-scavenger/example_csvs/multimeter.csv")
     print(data_health)
```

### Comparing `csv_scavenger-1.0.0/LICENSE` & `csv_scavenger-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_scavenger-1.0.0/pyproject.toml` & `csv_scavenger-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "csv-scavenger"
-version = "1.0.0"
+version = "1.0.1"
 description = "CSV reader and parser with automatic detection of delimiter and start/end of data."
 authors = ["Gustave Coulombe <magikgus@gmail.com>"]
 readme = "README.md"
-packages = [{include = "main.py", from = "csv-scavenger"}]
+packages = [{include = "scavenger.py", from = "csv-scavenger"}]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 pandas = "^2.0.0"
 tssplit = "^1.0.6"
```

### Comparing `csv_scavenger-1.0.0/README.md` & `csv_scavenger-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `csv_scavenger-1.0.0/PKG-INFO` & `csv_scavenger-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv-scavenger
-Version: 1.0.0
+Version: 1.0.1
 Summary: CSV reader and parser with automatic detection of delimiter and start/end of data.
 Author: Gustave Coulombe
 Author-email: magikgus@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
```

