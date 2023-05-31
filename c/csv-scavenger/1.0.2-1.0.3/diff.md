# Comparing `tmp/csv_scavenger-1.0.2.tar.gz` & `tmp/csv_scavenger-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_scavenger-1.0.2.tar", max compression
+gzip compressed data, was "csv_scavenger-1.0.3.tar", max compression
```

## Comparing `csv_scavenger-1.0.2.tar` & `csv_scavenger-1.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3034 2023-05-31 18:04:22.703660 csv_scavenger-1.0.2/csv-scavenger/scavenger.py
--rw-r--r--   0        0        0     1094 2023-05-31 15:26:00.843242 csv_scavenger-1.0.2/LICENSE
--rw-r--r--   0        0        0      542 2023-05-31 18:15:40.388167 csv_scavenger-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      663 2023-05-31 18:15:01.226065 csv_scavenger-1.0.2/README.md
--rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 csv_scavenger-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3030 2023-05-31 19:32:23.127800 csv_scavenger-1.0.3/csv-scavenger/scavenger.py
+-rw-r--r--   0        0        0     1094 2023-05-31 15:26:00.843242 csv_scavenger-1.0.3/LICENSE
+-rw-r--r--   0        0        0      542 2023-05-31 20:03:04.960811 csv_scavenger-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      663 2023-05-31 18:15:01.226065 csv_scavenger-1.0.3/README.md
+-rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 csv_scavenger-1.0.3/PKG-INFO
```

### Comparing `csv_scavenger-1.0.2/csv-scavenger/scavenger.py` & `csv_scavenger-1.0.3/csv-scavenger/scavenger.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         )
         if num_of_columns == csv_format[1] and header_line == None:
             header_line = i
         elif num_of_columns != csv_format[1] and header_line != None:
             last_line = i
             break
     if last_line == None:
-        last_line = len(lines) - 1
+        last_line = len(lines)
     first_line: Optional[int] = header_line + 1 if header_line != None else None
     return header_line, first_line, last_line
 
 
 def read_csv(file_path: str) -> pd.DataFrame:
     try:
         with open(file_path, "r") as file:
```

### Comparing `csv_scavenger-1.0.2/LICENSE` & `csv_scavenger-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_scavenger-1.0.2/pyproject.toml` & `csv_scavenger-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "csv-scavenger"
-version = "1.0.2"
+version = "1.0.3"
 description = "CSV reader and parser with automatic detection of delimiter and start/end of data."
 authors = ["Gustave Coulombe <magikgus@gmail.com>"]
 readme = "README.md"
 packages = [{include = "scavenger.py", from = "csv-scavenger"}]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
```

### Comparing `csv_scavenger-1.0.2/README.md` & `csv_scavenger-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `csv_scavenger-1.0.2/PKG-INFO` & `csv_scavenger-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv-scavenger
-Version: 1.0.2
+Version: 1.0.3
 Summary: CSV reader and parser with automatic detection of delimiter and start/end of data.
 Author: Gustave Coulombe
 Author-email: magikgus@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
```

