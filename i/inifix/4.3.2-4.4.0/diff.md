# Comparing `tmp/inifix-4.3.2.tar.gz` & `tmp/inifix-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inifix-4.3.2.tar", last modified: Sat Mar 11 12:51:17 2023, max compression
+gzip compressed data, was "inifix-4.4.0.tar", last modified: Wed May 31 18:36:27 2023, max compression
```

## Comparing `inifix-4.3.2.tar` & `inifix-4.4.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:51:17.020461 inifix-4.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-11 12:51:07.000000 inifix-4.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-03-11 12:51:17.020461 inifix-4.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-03-11 12:51:07.000000 inifix-4.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:51:17.016461 inifix-4.3.2/inifix/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-11 12:51:07.000000 inifix-4.3.2/inifix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-11 12:51:07.000000 inifix-4.3.2/inifix/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-03-11 12:51:07.000000 inifix-4.3.2/inifix/enotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-03-11 12:51:07.000000 inifix-4.3.2/inifix/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-03-11 12:51:07.000000 inifix-4.3.2/inifix/io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 12:51:07.000000 inifix-4.3.2/inifix/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-11 12:51:07.000000 inifix-4.3.2/inifix/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-03-11 12:51:07.000000 inifix-4.3.2/inifix/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:51:17.020461 inifix-4.3.2/inifix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-03-11 12:51:17.000000 inifix-4.3.2/inifix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-11 12:51:17.000000 inifix-4.3.2/inifix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 12:51:17.000000 inifix-4.3.2/inifix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-11 12:51:17.000000 inifix-4.3.2/inifix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-11 12:51:17.000000 inifix-4.3.2/inifix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-11 12:51:17.000000 inifix-4.3.2/inifix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-03-11 12:51:07.000000 inifix-4.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 12:51:17.020461 inifix-4.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:51:17.020461 inifix-4.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-03-11 12:51:07.000000 inifix-4.3.2/tests/test_casting.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-11 12:51:07.000000 inifix-4.3.2/tests/test_fargo_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-11 12:51:07.000000 inifix-4.3.2/tests/test_file_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-03-11 12:51:07.000000 inifix-4.3.2/tests/test_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-03-11 12:51:07.000000 inifix-4.3.2/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-11 12:51:07.000000 inifix-4.3.2/tests/test_pluto_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-11 12:51:07.000000 inifix-4.3.2/tests/test_schema_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:36:27.488100 inifix-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 18:36:17.000000 inifix-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-05-31 18:36:27.488100 inifix-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-05-31 18:36:17.000000 inifix-4.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-31 18:36:17.000000 inifix-4.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 18:36:27.488100 inifix-4.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:36:27.480100 inifix-4.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:36:27.484100 inifix-4.4.0/src/inifix/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-31 18:36:17.000000 inifix-4.4.0/src/inifix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-31 18:36:17.000000 inifix-4.4.0/src/inifix/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-31 18:36:17.000000 inifix-4.4.0/src/inifix/enotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-31 18:36:17.000000 inifix-4.4.0/src/inifix/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-05-31 18:36:17.000000 inifix-4.4.0/src/inifix/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 18:36:17.000000 inifix-4.4.0/src/inifix/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-31 18:36:17.000000 inifix-4.4.0/src/inifix/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-31 18:36:17.000000 inifix-4.4.0/src/inifix/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:36:27.484100 inifix-4.4.0/src/inifix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-05-31 18:36:27.000000 inifix-4.4.0/src/inifix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-31 18:36:27.000000 inifix-4.4.0/src/inifix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:36:27.000000 inifix-4.4.0/src/inifix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-31 18:36:27.000000 inifix-4.4.0/src/inifix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 18:36:27.000000 inifix-4.4.0/src/inifix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 18:36:27.000000 inifix-4.4.0/src/inifix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:36:27.488100 inifix-4.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-31 18:36:17.000000 inifix-4.4.0/tests/test_casting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-31 18:36:17.000000 inifix-4.4.0/tests/test_fargo_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-31 18:36:17.000000 inifix-4.4.0/tests/test_file_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-31 18:36:17.000000 inifix-4.4.0/tests/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-05-31 18:36:17.000000 inifix-4.4.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-31 18:36:17.000000 inifix-4.4.0/tests/test_pluto_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-31 18:36:17.000000 inifix-4.4.0/tests/test_schema_validation.py
```

### Comparing `inifix-4.3.2/LICENSE` & `inifix-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inifix-4.3.2/PKG-INFO` & `inifix-4.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inifix
-Version: 4.3.2
+Version: 4.4.0
 Summary: I/O facility for Idefix/Pluto configuration files
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/inifix
 Project-URL: Changelog, https://github.com/neutrinoceros/inifix/blob/main/CHANGELOG.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -16,20 +16,20 @@
 
 # `inifix`
 
 [![PyPI](https://img.shields.io/pypi/v/inifix.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/inifix/)
 [![PyPI](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)](https://pypi.org/project/inifix/)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/inifix/main.svg)](https://results.pre-commit.ci/badge/github/neutrinoceros/inifix/main.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 
 `inifix` is a small Python library of I/O functions to read and write 'ini'
 configuration files in the style of [Pluto](http://plutocode.ph.unito.it) and
-[Idefix](https://gricad-gitlab.univ-grenoble-alpes.fr/lesurg/idefix-public).
+[Idefix](https://github.com/idefix-code/idefix).
 
 While its primary goal is to follow Idefix's 'ini' format specification, it
 supports a small superset of it.
 
 The key differences are:
 - `inifix` supports section-free definitions. This means configuration files
   from [FARGO 3D](https://fargo3d.bitbucket.io) are also supported.
```

### Comparing `inifix-4.3.2/README.md` & `inifix-4.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # `inifix`
 
 [![PyPI](https://img.shields.io/pypi/v/inifix.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/inifix/)
 [![PyPI](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)](https://pypi.org/project/inifix/)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/inifix/main.svg)](https://results.pre-commit.ci/badge/github/neutrinoceros/inifix/main.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 
 `inifix` is a small Python library of I/O functions to read and write 'ini'
 configuration files in the style of [Pluto](http://plutocode.ph.unito.it) and
-[Idefix](https://gricad-gitlab.univ-grenoble-alpes.fr/lesurg/idefix-public).
+[Idefix](https://github.com/idefix-code/idefix).
 
 While its primary goal is to follow Idefix's 'ini' format specification, it
 supports a small superset of it.
 
 The key differences are:
 - `inifix` supports section-free definitions. This means configuration files
   from [FARGO 3D](https://fargo3d.bitbucket.io) are also supported.
```

### Comparing `inifix-4.3.2/inifix/_typing.py` & `inifix-4.4.0/src/inifix/_typing.py`

 * *Files identical despite different names*

### Comparing `inifix-4.3.2/inifix/enotation.py` & `inifix-4.4.0/src/inifix/enotation.py`

 * *Files identical despite different names*

### Comparing `inifix-4.3.2/inifix/format.py` & `inifix-4.4.0/src/inifix/format.py`

 * *Files identical despite different names*

### Comparing `inifix-4.3.2/inifix/io.py` & `inifix-4.4.0/src/inifix/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         buffer.write(content.encode("utf-8"))
     else:
         buffer.write(content)
 
 
 def _write_line(key: str, values: IterableOrSingle[Scalar], buffer: IOBase) -> None:
     val_repr = [_encode(v) for v in always_iterable(values)]
-    _write(f"{key} {'  '.join([v for v in val_repr])}\n", buffer)
+    _write(f"{key} {'  '.join(list(val_repr))}\n", buffer)
 
 
 def _write_to_buffer(data: InifixConfT, buffer: IOBase) -> None:
     for _is_first, is_last, (key, val) in mark_ends(data.items()):
         if not isinstance(val, dict):
             _write_line(key, val, buffer)
             continue
```

### Comparing `inifix-4.3.2/inifix/validate.py` & `inifix-4.4.0/src/inifix/validate.py`

 * *Files identical despite different names*

### Comparing `inifix-4.3.2/inifix/validation.py` & `inifix-4.4.0/src/inifix/validation.py`

 * *Files identical despite different names*

### Comparing `inifix-4.3.2/inifix.egg-info/PKG-INFO` & `inifix-4.4.0/src/inifix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inifix
-Version: 4.3.2
+Version: 4.4.0
 Summary: I/O facility for Idefix/Pluto configuration files
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/inifix
 Project-URL: Changelog, https://github.com/neutrinoceros/inifix/blob/main/CHANGELOG.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -16,20 +16,20 @@
 
 # `inifix`
 
 [![PyPI](https://img.shields.io/pypi/v/inifix.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/inifix/)
 [![PyPI](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)](https://pypi.org/project/inifix/)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/inifix/main.svg)](https://results.pre-commit.ci/badge/github/neutrinoceros/inifix/main.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 
 `inifix` is a small Python library of I/O functions to read and write 'ini'
 configuration files in the style of [Pluto](http://plutocode.ph.unito.it) and
-[Idefix](https://gricad-gitlab.univ-grenoble-alpes.fr/lesurg/idefix-public).
+[Idefix](https://github.com/idefix-code/idefix).
 
 While its primary goal is to follow Idefix's 'ini' format specification, it
 supports a small superset of it.
 
 The key differences are:
 - `inifix` supports section-free definitions. This means configuration files
   from [FARGO 3D](https://fargo3d.bitbucket.io) are also supported.
```

### Comparing `inifix-4.3.2/pyproject.toml` & `inifix-4.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 requires = [
     "setuptools>=61.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inifix"
-version = "4.3.2"
 description = "I/O facility for Idefix/Pluto configuration files"
 authors = [
     { name = "C.M.T. Robert" },
 ]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Typing :: Typed",
 ]
 requires-python = ">=3.8"
 dependencies = [
     "more-itertools>=8.4",
 ]
+dynamic = ["version"]
+
+[tool.setuptools.dynamic]
+version = {attr = "inifix.__version__"}
 
 [project.license]
 text = "GPL-3.0"
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
@@ -45,33 +48,34 @@
 
 [tool.setuptools.package-data]
 inifix = [
     "py.typed",
 ]
 
 [tool.setuptools.packages.find]
-exclude = [
-    "tests*",
-    "testing*",
-]
+where = ["src"]
 namespaces = false
 
 [tool.ruff]
-target-version = "py38" # https://github.com/charliermarsh/ruff/issues/2039
 exclude = ["*__init__.py"]
 ignore = ["E501"]
 select = [
     "E",
     "F",
     "W",
-    "B",
-    "I",
-    "UP",
+    "C4",  # flake8-comprehensions
+    "B",   # flake8-bugbear
+    "YTT", # flake8-2020
+    "I",   # isort
+    "UP",  # pyupgrade
 ]
 
+[tool.ruff.isort]
+known-first-party = ["inifix"]
+
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 exclude_lines = [
     # a more strict default pragma
     "\\# pragma: no cover\\b",
```

### Comparing `inifix-4.3.2/tests/test_casting.py` & `inifix-4.4.0/tests/test_casting.py`

 * *Files identical despite different names*

### Comparing `inifix-4.3.2/tests/test_file_validation.py` & `inifix-4.4.0/tests/test_file_validation.py`

 * *Files identical despite different names*

### Comparing `inifix-4.3.2/tests/test_format.py` & `inifix-4.4.0/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `inifix-4.3.2/tests/test_io.py` & `inifix-4.4.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `inifix-4.3.2/tests/test_schema_validation.py` & `inifix-4.4.0/tests/test_schema_validation.py`

 * *Files identical despite different names*

