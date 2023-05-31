# Comparing `tmp/flake8-eradicate-1.4.0.tar.gz` & `tmp/flake8_eradicate-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-eradicate-1.4.0.tar", max compression
+gzip compressed data, was "flake8_eradicate-1.5.0.tar", max compression
```

## Comparing `flake8-eradicate-1.4.0.tar` & `flake8_eradicate-1.5.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1071 2022-09-20 19:37:02.063205 flake8-eradicate-1.4.0/LICENSE
--rw-r--r--   0        0        0     2496 2022-09-20 19:37:02.063568 flake8-eradicate-1.4.0/README.md
--rw-r--r--   0        0        0     5242 2022-09-20 19:57:30.204256 flake8-eradicate-1.4.0/flake8_eradicate.py
--rw-r--r--   0        0        0     1592 2022-09-20 20:05:20.851731 flake8-eradicate-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     3428 1970-01-01 00:00:00.000000 flake8-eradicate-1.4.0/setup.py
--rw-r--r--   0        0        0     3818 1970-01-01 00:00:00.000000 flake8-eradicate-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-31 09:38:26.491370 flake8_eradicate-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2496 2023-05-31 09:38:26.491473 flake8_eradicate-1.5.0/README.md
+-rw-r--r--   0        0        0     5054 2023-05-31 09:56:51.350421 flake8_eradicate-1.5.0/flake8_eradicate.py
+-rw-r--r--   0        0        0     1226 2023-05-31 09:56:51.350920 flake8_eradicate-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3755 1970-01-01 00:00:00.000000 flake8_eradicate-1.5.0/PKG-INFO
```

### Comparing `flake8-eradicate-1.4.0/LICENSE` & `flake8_eradicate-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-eradicate-1.4.0/README.md` & `flake8_eradicate-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `flake8-eradicate-1.4.0/flake8_eradicate.py` & `flake8_eradicate-1.5.0/flake8_eradicate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import tokenize
+from importlib import metadata as importlib_metadata
 from typing import (
     Any,
     ClassVar,
     Dict,
     Iterable,
     Iterator,
     List,
@@ -11,28 +12,20 @@
     Tuple,
     Type,
 )
 
 from eradicate import Eradicator
 from flake8.options.manager import OptionManager
 
-try:  # pragma: no cover
-    from importlib import metadata as importlib_metadata  # type: ignore
-except ImportError:  # pragma: no cover
-    import importlib_metadata  # type: ignore
-
 #: This is a name that we use to install this library:
 pkg_name = 'flake8-eradicate'
 
 #: We store the version number inside the `pyproject.toml`:
 pkg_version = importlib_metadata.version(pkg_name)
 
-#: Const for `stdin` mode of `flake8`:
-STDIN = 'stdin'
-
 
 class Checker(object):
     """Flake8 plugin to find commented out code."""
 
     name = pkg_name
     version = pkg_version
```

### Comparing `flake8-eradicate-1.4.0/pyproject.toml` & `flake8_eradicate-1.5.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flake8-eradicate"
-version = "1.4.0"
+version = "1.5.0"
 description = "Flake8 plugin to find commented out code"
 
 license = "MIT"
 
 authors = [
   "Nikita Sobolev <mail@sobolevn.me>"
 ]
@@ -32,42 +32,28 @@
   "Topic :: Software Development :: Quality Assurance",
 ]
 
 [tool.poetry.urls]
 "Funding" = "https://opencollective.com/wemake-python-styleguide"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 
-flake8 = ">=3.5,<6"
+flake8 = ">5"
 eradicate = "^2.0"
 attrs = "*"
-importlib-metadata = { version = "*", python = "<3.8" }
 
 [tool.poetry.group.test.dependencies]
-pytest-cov = "^3.0"
-pytest-randomly = "^3.10"
-pytest = "^7.0"
-
-flake8-print = "^4.0"
-flake8-builtins = "^1.5"
-flake8-commas = "^2.0"
-flake8-quotes = "^3.2"
-flake8-comprehensions = "^3.5"
-flake8-docstrings = "^1.6"
-flake8-string-format = "^0.3"
-flake8-pep3101 = "^1.3"
-flake8-super-call = "^1.0"
-flake8-debugger = "^4.0"
-flake8-isort = "^4.2"
-pep8-naming = "^0.13"
+pytest = "^7.3"
+pytest-cov = "^4.0"
+pytest-randomly = "^3.12"
 
-mypy = "^0.971"
-safety = "^2.1"
+mypy = "^1.3"
+safety = "^2.3"
 
 [tool.poetry.plugins."flake8.extension"]
 E8 = "flake8_eradicate:Checker"
 
 
 [build-system]
-requires = ["poetry-core>=1.2.0"]
+requires = ["poetry-core>=1.6.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `flake8-eradicate-1.4.0/PKG-INFO` & `flake8_eradicate-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: flake8-eradicate
-Version: 1.4.0
+Version: 1.5.0
 Summary: Flake8 plugin to find commented out code
 Home-page: https://github.com/wemake-services/flake8-eradicate
 License: MIT
 Keywords: flake8,plugin,linting,wemake.services,code quality
 Author: Nikita Sobolev
 Author-email: mail@sobolevn.me
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: attrs
 Requires-Dist: eradicate (>=2.0,<3.0)
-Requires-Dist: flake8 (>=3.5,<6)
-Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: flake8 (>5)
 Project-URL: Funding, https://opencollective.com/wemake-python-styleguide
 Project-URL: Repository, https://github.com/wemake-services/flake8-eradicate
 Description-Content-Type: text/markdown
 
 # flake8-eradicate
 
 [![wemake.services](https://img.shields.io/badge/-wemake.services-green.svg?label=%20&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAABGdBTUEAALGPC%2FxhBQAAAAFzUkdCAK7OHOkAAAAbUExURQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAP%2F%2F%2F5TvxDIAAAAIdFJOUwAjRA8xXANAL%2Bv0SAAAADNJREFUGNNjYCAIOJjRBdBFWMkVQeGzcHAwksJnAPPZGOGAASzPzAEHEGVsLExQwE7YswCb7AFZSF3bbAAAAABJRU5ErkJggg%3D%3D)](https://wemake-services.github.io)
```

