# Comparing `tmp/cg_flake8_reporter-0.1.0.tar.gz` & `tmp/cg_flake8_reporter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg_flake8_reporter-0.1.0.tar", max compression
+gzip compressed data, was "cg_flake8_reporter-0.1.1.tar", max compression
```

## Comparing `cg_flake8_reporter-0.1.0.tar` & `cg_flake8_reporter-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2390 2023-05-30 16:10:01.364601 cg_flake8_reporter-0.1.0/README.md
--rw-r--r--   0        0        0      159 2023-05-30 14:35:58.970236 cg_flake8_reporter-0.1.0/cg_flake8_reporter/__init__.py
--rw-r--r--   0        0        0     6492 2023-05-30 16:10:01.364875 cg_flake8_reporter-0.1.0/cg_flake8_reporter/plugin.py
--rw-r--r--   0        0        0     1860 2023-05-30 14:35:58.970683 cg_flake8_reporter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2819 1970-01-01 00:00:00.000000 cg_flake8_reporter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2362 2023-05-31 13:11:46.818733 cg_flake8_reporter-0.1.1/README.md
+-rw-r--r--   0        0        0      159 2023-05-31 13:19:44.972710 cg_flake8_reporter-0.1.1/cg_flake8_reporter/__init__.py
+-rw-r--r--   0        0        0     6466 2023-05-31 13:11:46.818939 cg_flake8_reporter-0.1.1/cg_flake8_reporter/plugin.py
+-rw-r--r--   0        0        0     1860 2023-05-31 13:20:06.815755 cg_flake8_reporter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 cg_flake8_reporter-0.1.1/PKG-INFO
```

### Comparing `cg_flake8_reporter-0.1.0/README.md` & `cg_flake8_reporter-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,43 +27,43 @@
 
 The `cg-points-deducted` option makes it possible to configure the amount of
 points (in percentage) that each violation deducts from the total points.
 
 The `cg-points-deducted` expectes a string in the following format as input:
 
 ```bash
-'info:<percentage>,warning:<percentage>,error:<percentage>,fatal:<percentage>'
+'info:<percentage>,warning:<percentage>,error:<percentage>'
 ```
 
 Each of the violation levels must be present in the provided string. The
 percentage provided should be an integer number **without** the `%` symbol.
 
 If you wish for a violation level to not deduct points, simply set it to `0`.
 
 ### cg-flake8-fd
 
 The `cg-flake8-fd` option makes it possible to configure where the reporter
 will write its output. By default, the value is `1`, which means the reporter
 will write to `stdout`. Within AutoTest v2 it is recommended to use file
 descriptor `3` so that the comments will be visible in CodeGrade's UI. The
-*Flake8* step will already set this up for you.
+_Flake8_ step will already set this up for you.
 
 ### cg-base-path
 
 The `cg-base-path` allows you to restrict which files the reporter will report.
 For example, if you only want files to be reported within the `server` directory
 of the student, you may want to set `--cg-base-path=~/student/server/`. Beware,
-the *Flake8* step always sets `cg-base-path` to the root of the student's
-workspace. If you want to customize this, you should use a *Custom Test* step
+the _Flake8_ step always sets `cg-base-path` to the root of the student's
+workspace. If you want to customize this, you should use a _Custom Test_ step
 instead.
 
 ## Usage
 
 To run Flake8 with the custom reporter:
 
 ```bash
 python3 -m flake8 \
     --format=jsonfd \
-    --cg-points-deducted='info:1,warning:3,error:5,fatal:10' \
+    --cg-points-deducted='info:1,warning:3,error:5' \
     --cg-flake8-fd=1 \
     ./
 ```
```

### Comparing `cg_flake8_reporter-0.1.0/cg_flake8_reporter/plugin.py` & `cg_flake8_reporter-0.1.1/cg_flake8_reporter/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,30 +24,31 @@
     # python's `len` function reports it is equal to the string's byte length.
     # Do not insert spaces after each separator.
     return json.dumps(obj, ensure_ascii=True, separators=(',', ':'))
 
 
 class CustomFormatter(flake8.formatting.base.BaseFormatter):
     """
-    Custom Formatter for flake8. 
+    Custom Formatter for flake8.
     Formats the errors/warnings as JSON objects.
     Also calculates a score based on severity of errors/warnings.
     """
     def __init__(self, options: argparse.Namespace) -> None:
         """
         Initialize buffer for comments, score, and points deducted for each severity level.
         """
         super().__init__(options)
         self._buffer: t.Mapping[str,
                                 t.Any] = {"tag": "comments", "comments": {}}
         self._score = Fraction(1, 1)
         self._buffer_size = 0
         self._points_deducted = {
-            'info': Fraction(0, 1), 'warning': Fraction(0, 1), 'error':
-                Fraction(0, 1), 'fatal': Fraction(0, 1)
+            'info': Fraction(0, 1),
+            'warning': Fraction(0, 1),
+            'error': Fraction(0, 1),
         }
         # pylint: disable=consider-using-with
         try:
             self._file = open(options.cg_flake8_fd, 'wb', buffering=0)
         except OSError as e:
             raise IOError(
                 f'Could not open file descriptor {options.cg_flake8_fd}'
@@ -75,15 +76,15 @@
             '--cg-points-deducted',
             dest='cg_points_deducted',
             action='store',
             type=str,
             parse_from_config=True,
             help="""
 Points deducted for each severity level. Should be a string of
-the form 'info:1,warning:5,error:10,fatal:10'
+the form 'info:1,warning:5,error:10'
             """,
         )
         parser.add_option(
             '--cg-flake8-fd',
             dest='cg_flake8_fd',
             action='store',
             type=int,
```

### Comparing `cg_flake8_reporter-0.1.0/pyproject.toml` & `cg_flake8_reporter-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cg-flake8-reporter"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["CodeGrade <info@codegrade.com>"]
 readme = "README.md"
 packages = [{ include = "cg_flake8_reporter" }]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `cg_flake8_reporter-0.1.0/PKG-INFO` & `cg_flake8_reporter-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg-flake8-reporter
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: CodeGrade
 Author-email: info@codegrade.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -41,44 +41,44 @@
 
 The `cg-points-deducted` option makes it possible to configure the amount of
 points (in percentage) that each violation deducts from the total points.
 
 The `cg-points-deducted` expectes a string in the following format as input:
 
 ```bash
-'info:<percentage>,warning:<percentage>,error:<percentage>,fatal:<percentage>'
+'info:<percentage>,warning:<percentage>,error:<percentage>'
 ```
 
 Each of the violation levels must be present in the provided string. The
 percentage provided should be an integer number **without** the `%` symbol.
 
 If you wish for a violation level to not deduct points, simply set it to `0`.
 
 ### cg-flake8-fd
 
 The `cg-flake8-fd` option makes it possible to configure where the reporter
 will write its output. By default, the value is `1`, which means the reporter
 will write to `stdout`. Within AutoTest v2 it is recommended to use file
 descriptor `3` so that the comments will be visible in CodeGrade's UI. The
-*Flake8* step will already set this up for you.
+_Flake8_ step will already set this up for you.
 
 ### cg-base-path
 
 The `cg-base-path` allows you to restrict which files the reporter will report.
 For example, if you only want files to be reported within the `server` directory
 of the student, you may want to set `--cg-base-path=~/student/server/`. Beware,
-the *Flake8* step always sets `cg-base-path` to the root of the student's
-workspace. If you want to customize this, you should use a *Custom Test* step
+the _Flake8_ step always sets `cg-base-path` to the root of the student's
+workspace. If you want to customize this, you should use a _Custom Test_ step
 instead.
 
 ## Usage
 
 To run Flake8 with the custom reporter:
 
 ```bash
 python3 -m flake8 \
     --format=jsonfd \
-    --cg-points-deducted='info:1,warning:3,error:5,fatal:10' \
+    --cg-points-deducted='info:1,warning:3,error:5' \
     --cg-flake8-fd=1 \
     ./
 ```
```

