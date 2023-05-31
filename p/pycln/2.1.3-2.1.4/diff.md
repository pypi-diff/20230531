# Comparing `tmp/pycln-2.1.3.tar.gz` & `tmp/pycln-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycln-2.1.3.tar", max compression
+gzip compressed data, was "pycln-2.1.4.tar", max compression
```

## Comparing `pycln-2.1.3.tar` & `pycln-2.1.4.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1099 2023-01-16 13:11:12.225083 pycln-2.1.3/LICENSE
--rw-r--r--   0        0        0     7625 2023-01-16 13:11:12.225083 pycln-2.1.3/README.md
--rw-r--r--   0        0        0     1160 2023-01-16 13:11:12.229083 pycln-2.1.3/pycln/__init__.py
--rw-r--r--   0        0        0      113 2023-01-16 13:11:12.229083 pycln-2.1.3/pycln/__main__.py
--rw-r--r--   0        0        0     6828 2023-01-16 13:11:12.229083 pycln-2.1.3/pycln/cli.py
--rw-r--r--   0        0        0       26 2023-01-16 13:11:12.229083 pycln-2.1.3/pycln/utils/__init__.py
--rw-r--r--   0        0        0     3192 2023-01-16 13:11:12.229083 pycln-2.1.3/pycln/utils/_exceptions.py
--rw-r--r--   0        0        0     1813 2023-01-16 13:11:12.229083 pycln-2.1.3/pycln/utils/_nodes.py
--rw-r--r--   0        0        0     7477 2023-01-16 13:11:12.229083 pycln-2.1.3/pycln/utils/config.py
--rw-r--r--   0        0        0     3759 2023-01-16 13:11:12.229083 pycln-2.1.3/pycln/utils/iou.py
--rw-r--r--   0        0        0    12487 2023-01-16 13:11:12.229083 pycln-2.1.3/pycln/utils/pathu.py
--rw-r--r--   0        0        0    20961 2023-01-16 13:11:12.229083 pycln-2.1.3/pycln/utils/refactor.py
--rw-r--r--   0        0        0     4138 2023-01-16 13:11:12.229083 pycln-2.1.3/pycln/utils/regexu.py
--rw-r--r--   0        0        0    18739 2023-01-16 13:11:12.229083 pycln-2.1.3/pycln/utils/report.py
--rw-r--r--   0        0        0    34842 2023-01-16 13:11:12.229083 pycln-2.1.3/pycln/utils/scan.py
--rw-r--r--   0        0        0     8055 2023-01-16 13:11:12.229083 pycln-2.1.3/pycln/utils/transform.py
--rw-r--r--   0        0        0     1804 2023-01-16 13:11:12.229083 pycln-2.1.3/pyproject.toml
--rw-r--r--   0        0        0       66 2023-01-16 13:11:12.229083 pycln-2.1.3/vendor/custom/__init__.py
--rw-r--r--   0        0        0     2018 2023-01-16 13:11:12.229083 pycln-2.1.3/vendor/custom/_site.py
--rw-r--r--   0        0        0     8909 1970-01-01 00:00:00.000000 pycln-2.1.3/setup.py
--rw-r--r--   0        0        0     9092 1970-01-01 00:00:00.000000 pycln-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-31 14:52:37.059019 pycln-2.1.4/LICENSE
+-rw-r--r--   0        0        0     7370 2023-05-31 14:52:37.059019 pycln-2.1.4/README.md
+-rw-r--r--   0        0        0     1160 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/__init__.py
+-rw-r--r--   0        0        0      113 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/__main__.py
+-rw-r--r--   0        0        0     6828 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/cli.py
+-rw-r--r--   0        0        0       26 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/__init__.py
+-rw-r--r--   0        0        0     3192 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/_exceptions.py
+-rw-r--r--   0        0        0     1813 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/_nodes.py
+-rw-r--r--   0        0        0     7477 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/config.py
+-rw-r--r--   0        0        0     3908 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/iou.py
+-rw-r--r--   0        0        0    12640 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/pathu.py
+-rw-r--r--   0        0        0    20961 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/refactor.py
+-rw-r--r--   0        0        0     4138 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/regexu.py
+-rw-r--r--   0        0        0    18739 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/report.py
+-rw-r--r--   0        0        0    34842 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/scan.py
+-rw-r--r--   0        0        0     8055 2023-05-31 14:52:37.063019 pycln-2.1.4/pycln/utils/transform.py
+-rw-r--r--   0        0        0     1796 2023-05-31 14:52:37.063019 pycln-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-05-31 14:52:37.067020 pycln-2.1.4/vendor/custom/__init__.py
+-rw-r--r--   0        0        0     2018 2023-05-31 14:52:37.067020 pycln-2.1.4/vendor/custom/_site.py
+-rw-r--r--   0        0        0     8637 1970-01-01 00:00:00.000000 pycln-2.1.4/PKG-INFO
```

### Comparing `pycln-2.1.3/LICENSE` & `pycln-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycln-2.1.3/README.md` & `pycln-2.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 </p>
 
 <p align="center">
     <img src="https://img.shields.io/pypi/pyversions/pycln?style=flat-square" alt="PYPI - Python Version">
     <a href="https://pypi.org/project/pycln/"><img src="https://img.shields.io/pypi/v/pycln?style=flat-square" alt="PYPI - Pycln Version"></a>
     <a href="https://pepy.tech/project/pycln/"><img src="https://static.pepy.tech/personalized-badge/pycln?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=total downloads" alt="Total Downloads"></a>
     <a href="https://pypi.org/project/pycln/"><img src="https://img.shields.io/pypi/dm/pycln?color=dark-green&style=flat-square" alt="Downloads"></a>
-    <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fhadialqattan%2Fpycln&count_bg=%2344CC10&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true"/></a>
 </p>
 
 <p align="center">
     <a href="https://github.com/hadialqattan/pycln/fork"><img src="https://img.shields.io/github/forks/hadialqattan/pycln?style=flat-square" alt="Forks"></a>
     <a href="https://github.com/hadialqattan/pycln/stargazers"><img src="https://img.shields.io/github/stars/hadialqattan/pycln?style=flat-square" alt="Stars"></a>
     <a href="https://github.com/hadialqattan/pycln/issues"><img src="https://img.shields.io/github/issues/hadialqattan/pycln?style=flat-square" alt="Issues"></a>
     <a href="https://github.com/hadialqattan/pycln/pulls"><img src="https://img.shields.io/github/issues-pr/hadialqattan/pycln?style=flat-square" alt="Pull Requests"></a>
```

#### html2text {}

```diff
@@ -1,13 +1,11 @@
 [Logo]
   ***** A formatter for finding and removing unused import statements. *****
    [Pycln_Docs] [CI] [CD] [FUZZ] [Codacy_Badge] [Codecov] [Maintainability]
  [PYPI - Python Version] [PYPI_-_Pycln_Version] [Total_Downloads] [Downloads]
-                 [https://hits.seeyoufarm.com/api/count/incr/
-badge.svg?url=https%3A%2F%2Fgithub.com%2Fhadialqattan%2Fpycln&count_bg=%2344CC10&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true]
 [Forks] [Stars] [Issues] [Pull_Requests] [Contributors] [Last_Commit] [License]
    [Docstrings:_reStructuredText] [Code_style:_black] [Code_style:_prettier]
 --- **[Read the documentation on Github pages!](https://hadialqattan.github.io/
 pycln)** --- ## Installation and usage ### Installation Pycln requires Python
 3.6+ and can be easily installed using the most common Python packaging tools.
 We recommend installing the latest stable release from PyPI with pip: ```bash $
 pip install pycln ``` ### Usage By **default** Pycln will remove any unused
```

### Comparing `pycln-2.1.3/pycln/__init__.py` & `pycln-2.1.4/pycln/__init__.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.3/pycln/cli.py` & `pycln-2.1.4/pycln/cli.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.3/pycln/utils/_exceptions.py` & `pycln-2.1.4/pycln/utils/_exceptions.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.3/pycln/utils/_nodes.py` & `pycln-2.1.4/pycln/utils/_nodes.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.3/pycln/utils/config.py` & `pycln-2.1.4/pycln/utils/config.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.3/pycln/utils/iou.py` & `pycln-2.1.4/pycln/utils/iou.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,16 +86,21 @@
 
 def safe_write(path: Path, fixed_lines: List[str], encoding: str, newline: str) -> None:
     """Write file content based on given `encoding`.
 
     :param path: `.py` file path.
     :param encoding: file encoding.
     :param fixed_lines: fixed source code lines.
-    :param newline: original file's newline (CRFL | FL).
+    :param newline: output file's newline (CRFL | FL).
     :raises WritePermissionError: when `os.W_OK` in permissions
         and the source does not have write permission.
     """
     if not os.access(path, os.W_OK):
         raise WritePermissionError(13, "Permission denied [WRITE]", path)
-    with open(path, mode="w", encoding=encoding) as destination:
+
+    fixed_lines_newline = newline
+    if fixed_lines:
+        fixed_lines_newline = CRLF if CRLF == fixed_lines[0][-2:] else LF
+
+    with open(path, mode="w", encoding=encoding, newline="") as destination:
         for line in fixed_lines:
-            destination.write(line.replace(os.linesep, newline))
+            destination.write(line.replace(fixed_lines_newline, newline))
```

### Comparing `pycln-2.1.3/pycln/utils/pathu.py` & `pycln-2.1.4/pycln/utils/pathu.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,20 @@
     "parser",
     "string",
     "operator",
     "datetime",
     "multiprocessing",
 }
 IMPORTS_WITH_SIDE_EFFECTS = {"this", "antigravity", "rlcompleter"}
+PYTHON_STDLIB_PATHS = frozenset(
+    {
+        sysconfig.get_python_lib(standard_lib=True, plat_specific=True),
+        sysconfig.get_python_lib(standard_lib=True, plat_specific=False),
+    }
+)
 
 
 def yield_sources(
     path: Path,
     include: Pattern[str],
     exclude: Pattern[str],
     extend_exclude: Pattern[str],
@@ -127,20 +133,15 @@
 def get_standard_lib_paths() -> Set[Path]:
     """Get paths to Python standard library modules.
 
     :returns: set of paths to Python standard library modules.
     """
     paths: Set[Path] = set()
 
-    for is_plat_specific in [True, False]:
-
-        # Get lib modules paths.
-        lib_path = sysconfig.get_python_lib(
-            standard_lib=True, plat_specific=is_plat_specific
-        )
+    for lib_path in PYTHON_STDLIB_PATHS:
 
         for path in os.listdir(lib_path):
             paths.add(Path(os.path.join(lib_path, path)))
 
         # Get lib dynload modules paths, if exists.
         lib_dynload_path = os.path.join(lib_path, LIB_DYNLOAD)
 
@@ -182,19 +183,22 @@
 
     :returns: a tuple of a set of paths of third party library modules
         and a set of paths from `.pth` file(s) content, respectively.
     """
     paths: Set[Path] = set()
     pth_paths: Set[Path] = set()
 
-    packages_paths: Set[str] = {
-        path
-        for path in sys.path
-        if path and Path(path).parts[-1] in [DIST_PACKAGES, SITE_PACKAGES]
-    }
+    packages_paths: Set[str] = set()
+
+    for path in sys.path:
+        ppath = Path(path)
+        if ppath.parts[-1] in (DIST_PACKAGES, SITE_PACKAGES) or (
+            ppath.is_dir() and path not in PYTHON_STDLIB_PATHS
+        ):
+            packages_paths.add(path)
 
     for path in packages_paths:
 
         for name in os.listdir(path):
             if name.endswith(PTH_EXTENSION):
                 for pth_path in _site.addpackage(path, name):
                     pth_paths.add(Path(pth_path))
```

### Comparing `pycln-2.1.3/pycln/utils/refactor.py` & `pycln-2.1.4/pycln/utils/refactor.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.3/pycln/utils/regexu.py` & `pycln-2.1.4/pycln/utils/regexu.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.3/pycln/utils/report.py` & `pycln-2.1.4/pycln/utils/report.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.3/pycln/utils/scan.py` & `pycln-2.1.4/pycln/utils/scan.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.3/pycln/utils/transform.py` & `pycln-2.1.4/pycln/utils/transform.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.3/pyproject.toml` & `pycln-2.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycln"
-version = "2.1.3"
+version = "2.1.4"
 description = "A formatter for finding and removing unused import statements."
 authors = ["Hadi Alqattan <alqattanhadizaki@gmail.com>"]
 homepage = "https://hadialqattan.github.io/pycln"
 repository = "https://github.com/hadialqattan/pycln"
 keywords = ["formatter", "linter", "quality-assurance", "tools", "cli"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -21,18 +21,18 @@
 packages = [{ include = "pycln" }, { include = "vendor" }]
 
 [tool.poetry.scripts]
 pycln = "pycln.cli:app"
 
 [tool.poetry.dependencies]
 python = ">=3.6.2, <4"
-typer = ">=0.4.1,<0.8.0"
+typer = ">=0.4.1,<0.10.0"
 dataclasses = {version = "^0.7", python = "3.6"}
 pyyaml = ">=5.3.1,<7.0.0"
-pathspec = ">=0.9.0,<0.11.0"
+pathspec = "^0.9.0"
 tomlkit = "^0.11.1"
 libcst = [{version = ">=0.3.10,<0.5.0", python = ">=3.7"}, {version = ">=0.3.10,<0.4.0", python = "<3.7"}]
 
 [tool.poetry.dev-dependencies]
 requests = "^2.24.0"
 semver = "^2.10.2"
 pytest = "^7.0"
```

### Comparing `pycln-2.1.3/vendor/custom/_site.py` & `pycln-2.1.4/vendor/custom/_site.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.3/setup.py` & `pycln-2.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,181 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pycln
+Version: 2.1.4
+Summary: A formatter for finding and removing unused import statements.
+Home-page: https://hadialqattan.github.io/pycln
+License: MIT
+Keywords: formatter,linter,quality-assurance,tools,cli
+Author: Hadi Alqattan
+Author-email: alqattanhadizaki@gmail.com
+Requires-Python: >=3.6.2,<4
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Utilities
+Requires-Dist: dataclasses (>=0.7,<0.8) ; python_version == "3.6"
+Requires-Dist: libcst (>=0.3.10,<0.4.0) ; python_version < "3.7"
+Requires-Dist: libcst (>=0.3.10,<0.5.0) ; python_version >= "3.7"
+Requires-Dist: pathspec (>=0.9.0,<0.10.0)
+Requires-Dist: pyyaml (>=5.3.1,<7.0.0)
+Requires-Dist: tomlkit (>=0.11.1,<0.12.0)
+Requires-Dist: typer (>=0.4.1,<0.10.0)
+Project-URL: Repository, https://github.com/hadialqattan/pycln
+Description-Content-Type: text/markdown
 
-packages = \
-['pycln', 'pycln.utils', 'vendor', 'vendor.custom']
+<img src="https://raw.githubusercontent.com/hadialqattan/pycln/master/docs/_media/logo-background.png" width="100%" alt="Logo">
 
-package_data = \
-{'': ['*']}
+<h2 align="center">
+    A formatter for finding and removing unused import statements.
+</h2>
 
-install_requires = \
-['pathspec>=0.9.0,<0.11.0',
- 'pyyaml>=5.3.1,<7.0.0',
- 'tomlkit>=0.11.1,<0.12.0',
- 'typer>=0.4.1,<0.8.0']
-
-extras_require = \
-{':python_version < "3.7"': ['libcst>=0.3.10,<0.4.0'],
- ':python_version == "3.6"': ['dataclasses>=0.7,<0.8'],
- ':python_version >= "3.7"': ['libcst>=0.3.10,<0.5.0']}
-
-entry_points = \
-{'console_scripts': ['pycln = pycln.cli:app']}
-
-setup_kwargs = {
-    'name': 'pycln',
-    'version': '2.1.3',
-    'description': 'A formatter for finding and removing unused import statements.',
-    'long_description': '<img src="https://raw.githubusercontent.com/hadialqattan/pycln/master/docs/_media/logo-background.png" width="100%" alt="Logo">\n\n<h2 align="center">\n    A formatter for finding and removing unused import statements.\n</h2>\n\n<p align="center">\n    <a href="https://hadialqattan.github.io/pycln"><img src="https://img.shields.io/badge/more%20info-Pycln%20Docs-B5FFB3.svg?style=flat-square" alt="Pycln Docs"></a>\n    <a href="https://github.com/hadialqattan/pycln/actions?query=workflow%3ACI"><img src="https://img.shields.io/github/actions/workflow/status/hadialqattan/pycln/ci.yml?branch=master&label=CI&logo=github&style=flat-square" alt="CI"></a>\n    <a href="https://github.com/hadialqattan/pycln/actions?query=workflow%3ACD"><img src="https://img.shields.io/github/actions/workflow/status/hadialqattan/pycln/cd.yml?label=CD&logo=github&style=flat-square" alt="CD"></a>\n    <a href="https://github.com/hadialqattan/pycln/actions?query=workflow%3AFUZZ"><img src="https://img.shields.io/github/actions/workflow/status/hadialqattan/pycln/fuzz.yml?label=FUZZ&logo=github&style=flat-square" alt="FUZZ"></a>\n    <a href="https://www.codacy.com/manual/hadialqattan/pycln/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=hadialqattan/pycln&amp;utm_campaign=Badge_Grade"><img src="https://img.shields.io/codacy/grade/e7c6c290c3c149e484634ac1905800d6/master?style=flat-square" alt="Codacy Badge"></a>\n    <a href="https://codecov.io/gh/hadialqattan/pycln"><img src="https://img.shields.io/codecov/c/gh/hadialqattan/pycln/master?token=VVYBDCZPHR&style=flat-square" alt="Codecov"></a>\n    <a href="https://codeclimate.com/github/hadialqattan/pycln/maintainability"><img src="https://img.shields.io/codeclimate/maintainability/hadialqattan/pycln?style=flat-square" alt="Maintainability"></a>\n</p>\n\n<p align="center">\n    <img src="https://img.shields.io/pypi/pyversions/pycln?style=flat-square" alt="PYPI - Python Version">\n    <a href="https://pypi.org/project/pycln/"><img src="https://img.shields.io/pypi/v/pycln?style=flat-square" alt="PYPI - Pycln Version"></a>\n    <a href="https://pepy.tech/project/pycln/"><img src="https://static.pepy.tech/personalized-badge/pycln?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=total downloads" alt="Total Downloads"></a>\n    <a href="https://pypi.org/project/pycln/"><img src="https://img.shields.io/pypi/dm/pycln?color=dark-green&style=flat-square" alt="Downloads"></a>\n    <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fhadialqattan%2Fpycln&count_bg=%2344CC10&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true"/></a>\n</p>\n\n<p align="center">\n    <a href="https://github.com/hadialqattan/pycln/fork"><img src="https://img.shields.io/github/forks/hadialqattan/pycln?style=flat-square" alt="Forks"></a>\n    <a href="https://github.com/hadialqattan/pycln/stargazers"><img src="https://img.shields.io/github/stars/hadialqattan/pycln?style=flat-square" alt="Stars"></a>\n    <a href="https://github.com/hadialqattan/pycln/issues"><img src="https://img.shields.io/github/issues/hadialqattan/pycln?style=flat-square" alt="Issues"></a>\n    <a href="https://github.com/hadialqattan/pycln/pulls"><img src="https://img.shields.io/github/issues-pr/hadialqattan/pycln?style=flat-square" alt="Pull Requests"></a>\n    <a href="https://github.com/hadialqattan/pycln/graphs/contributors"><img src="https://img.shields.io/github/contributors/hadialqattan/pycln?style=flat-square" alt="Contributors"></a>\n    <a href="https://github.com/hadialqattan/pycln/commits/master"><img src="https://img.shields.io/github/last-commit/hadialqattan/pycln.svg?style=flat-square" alt="Last Commit"></a>\n    <a href="https://github.com/hadialqattan/pycln/blob/master/LICENSE"><img src="https://img.shields.io/github/license/hadialqattan/pycln.svg?color=A31F34&style=flat-square" alt="License"></a>\n</p>\n\n<p align="center">\n    <a href="https://docutils.sourceforge.io/rst.html"><img src="https://img.shields.io/badge/docstrings-reStructuredText-gree.svg?style=flat-square" alt="Docstrings: reStructuredText"></a>\n    <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="Code style: black"></a>\n    <a href="https://github.com/prettier/prettier"><img src="https://img.shields.io/badge/code%20style-prettier-ff69b4.svg?style=flat-square" alt="Code style: prettier"></a>\n</p>\n\n---\n\n**[Read the documentation on Github pages!](https://hadialqattan.github.io/pycln)**\n\n---\n\n## Installation and usage\n\n### Installation\n\nPycln requires Python 3.6+ and can be easily installed using the most common Python\npackaging tools. We recommend installing the latest stable release from PyPI with pip:\n\n```bash\n$ pip install pycln\n```\n\n### Usage\n\nBy **default** Pycln will remove any unused import statement, So the simplest usage is\nto specify the path only:\n\n```bash\n$ pycln [PATH]\n```\n\nAlso, it\'s possible to run `pycln` as a package:\n\n```bash\n$ python3 -m pycln [PATH]\n```\n\nNOTE: you may need to use `-a/--all` option for more satisfying results. see\n[-a/--all flag](https://hadialqattan.github.io/pycln/#/?id=-a-all-flag).\n\nFurther information can be found in our docs:\n\n- [Usage and Configuration](https://hadialqattan.github.io/pycln/#/?id=usage)\n\n## Configuration\n\n**Pycln** is able to read project-specific default values for its command line options\nfrom a configuration file like `pyproject.toml` or `setup.cfg`. This is especially\nuseful for specifying custom CLI arguments/options like `path/paths`, `--include`,\n`--exclude`/`--extend-exclude`, or even `--all`.\n\nYou can find more details in our documentation:\n\n- [--config [PATH] CLI option](https://hadialqattan.github.io/pycln/#/?id=-config-path-option)\n\nAnd if you\'re looking for more general configuration documentation:\n\n- [Usage and Configuration](https://hadialqattan.github.io/pycln/#/?id=usage)\n\n## Used by\n\nThe following notable open-source projects trust and use _Pycln_:\n\n- [cibuildwheel](https://github.com/pypa/cibuildwheel)\n- [Open Event Server](https://github.com/fossasia/open-event-server)\n- [pybind11](https://github.com/pybind/pybind11)\n- [Poetry](https://github.com/python-poetry/poetry)\n- [Pyodide](https://github.com/pyodide/pyodide)\n- [Rich](https://github.com/Textualize/rich)\n- [typeshed](https://github.com/python/typeshed)\n\nThe following organizations use _Pycln_:\n\n- [FOSSASIA](https://github.com/fossasia)\n- [Poetry](https://github.com/python-poetry)\n- [Python Packaging Authority](https://github.com/pypa)\n- [Scikit-HEP](https://github.com/scikit-hep)\n\nAre we missing anyone? Let us know.\n\n## License\n\nMIT\n\n## Contributing\n\nA big welcome for considering contributing to make the project better!\n\nYou can get started by reading this:\n\n- [General guidlines](https://hadialqattan.github.io/pycln/#/CONTRIBUTING?id=general-guidelines)\n\nYou can also dive directly into the technicalities:\n\n- [Contributing technicalities](https://hadialqattan.github.io/pycln/#/CONTRIBUTING?id=technicalities)\n\n## Change log\n\nThe log has become rather long. It moved to its own file.\n\nSee [CHANGELOG](https://hadialqattan.github.io/pycln/#/CHANGELOG).\n\n## Authors\n\nThe author list is quite long nowadays, so it lives in its own file.\n\nSee [AUTHORS](https://hadialqattan.github.io/pycln/#/AUTHORS)\n\n## Code of Conduct\n\nEveryone participating in the _Pycln_ project, and in particular in the issue tracker,\nand pull requests is expected to treat other people with respect.\n\n---\n\nGive a ⭐️ if this project helped you!\n',
-    'author': 'Hadi Alqattan',
-    'author_email': 'alqattanhadizaki@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://hadialqattan.github.io/pycln',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6.2,<4',
-}
+<p align="center">
+    <a href="https://hadialqattan.github.io/pycln"><img src="https://img.shields.io/badge/more%20info-Pycln%20Docs-B5FFB3.svg?style=flat-square" alt="Pycln Docs"></a>
+    <a href="https://github.com/hadialqattan/pycln/actions?query=workflow%3ACI"><img src="https://img.shields.io/github/actions/workflow/status/hadialqattan/pycln/ci.yml?branch=master&label=CI&logo=github&style=flat-square" alt="CI"></a>
+    <a href="https://github.com/hadialqattan/pycln/actions?query=workflow%3ACD"><img src="https://img.shields.io/github/actions/workflow/status/hadialqattan/pycln/cd.yml?label=CD&logo=github&style=flat-square" alt="CD"></a>
+    <a href="https://github.com/hadialqattan/pycln/actions?query=workflow%3AFUZZ"><img src="https://img.shields.io/github/actions/workflow/status/hadialqattan/pycln/fuzz.yml?label=FUZZ&logo=github&style=flat-square" alt="FUZZ"></a>
+    <a href="https://www.codacy.com/manual/hadialqattan/pycln/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=hadialqattan/pycln&amp;utm_campaign=Badge_Grade"><img src="https://img.shields.io/codacy/grade/e7c6c290c3c149e484634ac1905800d6/master?style=flat-square" alt="Codacy Badge"></a>
+    <a href="https://codecov.io/gh/hadialqattan/pycln"><img src="https://img.shields.io/codecov/c/gh/hadialqattan/pycln/master?token=VVYBDCZPHR&style=flat-square" alt="Codecov"></a>
+    <a href="https://codeclimate.com/github/hadialqattan/pycln/maintainability"><img src="https://img.shields.io/codeclimate/maintainability/hadialqattan/pycln?style=flat-square" alt="Maintainability"></a>
+</p>
 
+<p align="center">
+    <img src="https://img.shields.io/pypi/pyversions/pycln?style=flat-square" alt="PYPI - Python Version">
+    <a href="https://pypi.org/project/pycln/"><img src="https://img.shields.io/pypi/v/pycln?style=flat-square" alt="PYPI - Pycln Version"></a>
+    <a href="https://pepy.tech/project/pycln/"><img src="https://static.pepy.tech/personalized-badge/pycln?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=total downloads" alt="Total Downloads"></a>
+    <a href="https://pypi.org/project/pycln/"><img src="https://img.shields.io/pypi/dm/pycln?color=dark-green&style=flat-square" alt="Downloads"></a>
+</p>
+
+<p align="center">
+    <a href="https://github.com/hadialqattan/pycln/fork"><img src="https://img.shields.io/github/forks/hadialqattan/pycln?style=flat-square" alt="Forks"></a>
+    <a href="https://github.com/hadialqattan/pycln/stargazers"><img src="https://img.shields.io/github/stars/hadialqattan/pycln?style=flat-square" alt="Stars"></a>
+    <a href="https://github.com/hadialqattan/pycln/issues"><img src="https://img.shields.io/github/issues/hadialqattan/pycln?style=flat-square" alt="Issues"></a>
+    <a href="https://github.com/hadialqattan/pycln/pulls"><img src="https://img.shields.io/github/issues-pr/hadialqattan/pycln?style=flat-square" alt="Pull Requests"></a>
+    <a href="https://github.com/hadialqattan/pycln/graphs/contributors"><img src="https://img.shields.io/github/contributors/hadialqattan/pycln?style=flat-square" alt="Contributors"></a>
+    <a href="https://github.com/hadialqattan/pycln/commits/master"><img src="https://img.shields.io/github/last-commit/hadialqattan/pycln.svg?style=flat-square" alt="Last Commit"></a>
+    <a href="https://github.com/hadialqattan/pycln/blob/master/LICENSE"><img src="https://img.shields.io/github/license/hadialqattan/pycln.svg?color=A31F34&style=flat-square" alt="License"></a>
+</p>
+
+<p align="center">
+    <a href="https://docutils.sourceforge.io/rst.html"><img src="https://img.shields.io/badge/docstrings-reStructuredText-gree.svg?style=flat-square" alt="Docstrings: reStructuredText"></a>
+    <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="Code style: black"></a>
+    <a href="https://github.com/prettier/prettier"><img src="https://img.shields.io/badge/code%20style-prettier-ff69b4.svg?style=flat-square" alt="Code style: prettier"></a>
+</p>
+
+---
+
+**[Read the documentation on Github pages!](https://hadialqattan.github.io/pycln)**
+
+---
+
+## Installation and usage
+
+### Installation
+
+Pycln requires Python 3.6+ and can be easily installed using the most common Python
+packaging tools. We recommend installing the latest stable release from PyPI with pip:
+
+```bash
+$ pip install pycln
+```
+
+### Usage
+
+By **default** Pycln will remove any unused import statement, So the simplest usage is
+to specify the path only:
+
+```bash
+$ pycln [PATH]
+```
+
+Also, it's possible to run `pycln` as a package:
+
+```bash
+$ python3 -m pycln [PATH]
+```
+
+NOTE: you may need to use `-a/--all` option for more satisfying results. see
+[-a/--all flag](https://hadialqattan.github.io/pycln/#/?id=-a-all-flag).
+
+Further information can be found in our docs:
+
+- [Usage and Configuration](https://hadialqattan.github.io/pycln/#/?id=usage)
+
+## Configuration
+
+**Pycln** is able to read project-specific default values for its command line options
+from a configuration file like `pyproject.toml` or `setup.cfg`. This is especially
+useful for specifying custom CLI arguments/options like `path/paths`, `--include`,
+`--exclude`/`--extend-exclude`, or even `--all`.
+
+You can find more details in our documentation:
+
+- [--config [PATH] CLI option](https://hadialqattan.github.io/pycln/#/?id=-config-path-option)
+
+And if you're looking for more general configuration documentation:
+
+- [Usage and Configuration](https://hadialqattan.github.io/pycln/#/?id=usage)
+
+## Used by
+
+The following notable open-source projects trust and use _Pycln_:
+
+- [cibuildwheel](https://github.com/pypa/cibuildwheel)
+- [Open Event Server](https://github.com/fossasia/open-event-server)
+- [pybind11](https://github.com/pybind/pybind11)
+- [Poetry](https://github.com/python-poetry/poetry)
+- [Pyodide](https://github.com/pyodide/pyodide)
+- [Rich](https://github.com/Textualize/rich)
+- [typeshed](https://github.com/python/typeshed)
+
+The following organizations use _Pycln_:
+
+- [FOSSASIA](https://github.com/fossasia)
+- [Poetry](https://github.com/python-poetry)
+- [Python Packaging Authority](https://github.com/pypa)
+- [Scikit-HEP](https://github.com/scikit-hep)
+
+Are we missing anyone? Let us know.
+
+## License
+
+MIT
+
+## Contributing
+
+A big welcome for considering contributing to make the project better!
+
+You can get started by reading this:
+
+- [General guidlines](https://hadialqattan.github.io/pycln/#/CONTRIBUTING?id=general-guidelines)
+
+You can also dive directly into the technicalities:
+
+- [Contributing technicalities](https://hadialqattan.github.io/pycln/#/CONTRIBUTING?id=technicalities)
+
+## Change log
+
+The log has become rather long. It moved to its own file.
+
+See [CHANGELOG](https://hadialqattan.github.io/pycln/#/CHANGELOG).
+
+## Authors
+
+The author list is quite long nowadays, so it lives in its own file.
+
+See [AUTHORS](https://hadialqattan.github.io/pycln/#/AUTHORS)
+
+## Code of Conduct
+
+Everyone participating in the _Pycln_ project, and in particular in the issue tracker,
+and pull requests is expected to treat other people with respect.
+
+---
+
+Give a ⭐️ if this project helped you!
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,74 +1,63 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['pycln',
-'pycln.utils', 'vendor', 'vendor.custom'] package_data = \ {'': ['*']}
-install_requires = \ ['pathspec>=0.9.0,<0.11.0', 'pyyaml>=5.3.1,<7.0.0',
-'tomlkit>=0.11.1,<0.12.0', 'typer>=0.4.1,<0.8.0'] extras_require = \ {':
-python_version < "3.7"': ['libcst>=0.3.10,<0.4.0'], ':python_version == "3.6"':
-['dataclasses>=0.7,<0.8'], ':python_version >= "3.7"':
-['libcst>=0.3.10,<0.5.0']} entry_points = \ {'console_scripts': ['pycln =
-pycln.cli:app']} setup_kwargs = { 'name': 'pycln', 'version': '2.1.3',
-'description': 'A formatter for finding and removing unused import
-statements.', 'long_description': '[Logo]\n\n
-***** \n A formatter for finding and removing unused import statements.\n *****
-\n\n
-    \n [Pycln_Docs]\n [CI]\n [CD]\n [FUZZ]\n [Codacy_Badge]\n [Codecov]\n
-                              [Maintainability]\n
-\n\n
-  \n [PYPI - Python Version]\n [PYPI_-_Pycln_Version]\n [Total_Downloads]\n
-          [Downloads]\n [https://hits.seeyoufarm.com/api/count/incr/
-badge.svg?url=https%3A%2F%2Fgithub.com%2Fhadialqattan%2Fpycln&count_bg=%2344CC10&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true]\n
-\n\n
-  \n [Forks]\n [Stars]\n [Issues]\n [Pull_Requests]\n [Contributors]\n [Last
-                             Commit]\n [License]\n
-\n\n
-    \n [Docstrings:_reStructuredText]\n [Code_style:_black]\n [Code_style:
-                                  prettier]\n
-\n\n---\n\n**[Read the documentation on Github pages!](https://
-hadialqattan.github.io/pycln)**\n\n---\n\n## Installation and usage\n\n###
-Installation\n\nPycln requires Python 3.6+ and can be easily installed using
-the most common Python\npackaging tools. We recommend installing the latest
-stable release from PyPI with pip:\n\n```bash\n$ pip install pycln\n```\n\n###
-Usage\n\nBy **default** Pycln will remove any unused import statement, So the
-simplest usage is\nto specify the path only:\n\n```bash\n$ pycln
-[PATH]\n```\n\nAlso, it\'s possible to run `pycln` as a package:\n\n```bash\n$
-python3 -m pycln [PATH]\n```\n\nNOTE: you may need to use `-a/--all` option for
-more satisfying results. see\n[-a/--all flag](https://hadialqattan.github.io/
-pycln/#/?id=-a-all-flag).\n\nFurther information can be found in our docs:\n\n-
-[Usage and Configuration](https://hadialqattan.github.io/pycln/#/
-?id=usage)\n\n## Configuration\n\n**Pycln** is able to read project-specific
-default values for its command line options\nfrom a configuration file like
-`pyproject.toml` or `setup.cfg`. This is especially\nuseful for specifying
-custom CLI arguments/options like `path/paths`, `--include`,\n`--exclude`/`--
-extend-exclude`, or even `--all`.\n\nYou can find more details in our
-documentation:\n\n- [--config [PATH] CLI option](https://
-hadialqattan.github.io/pycln/#/?id=-config-path-option)\n\nAnd if you\'re
-looking for more general configuration documentation:\n\n- [Usage and
-Configuration](https://hadialqattan.github.io/pycln/#/?id=usage)\n\n## Used
-by\n\nThe following notable open-source projects trust and use _Pycln_:\n\n-
-[cibuildwheel](https://github.com/pypa/cibuildwheel)\n- [Open Event Server]
-(https://github.com/fossasia/open-event-server)\n- [pybind11](https://
-github.com/pybind/pybind11)\n- [Poetry](https://github.com/python-poetry/
-poetry)\n- [Pyodide](https://github.com/pyodide/pyodide)\n- [Rich](https://
-github.com/Textualize/rich)\n- [typeshed](https://github.com/python/
-typeshed)\n\nThe following organizations use _Pycln_:\n\n- [FOSSASIA](https://
-github.com/fossasia)\n- [Poetry](https://github.com/python-poetry)\n- [Python
-Packaging Authority](https://github.com/pypa)\n- [Scikit-HEP](https://
-github.com/scikit-hep)\n\nAre we missing anyone? Let us know.\n\n##
-License\n\nMIT\n\n## Contributing\n\nA big welcome for considering contributing
-to make the project better!\n\nYou can get started by reading this:\n\n-
-[General guidlines](https://hadialqattan.github.io/pycln/#/
-CONTRIBUTING?id=general-guidelines)\n\nYou can also dive directly into the
-technicalities:\n\n- [Contributing technicalities](https://
-hadialqattan.github.io/pycln/#/CONTRIBUTING?id=technicalities)\n\n## Change
-log\n\nThe log has become rather long. It moved to its own file.\n\nSee
-[CHANGELOG](https://hadialqattan.github.io/pycln/#/CHANGELOG).\n\n##
-Authors\n\nThe author list is quite long nowadays, so it lives in its own
-file.\n\nSee [AUTHORS](https://hadialqattan.github.io/pycln/#/AUTHORS)\n\n##
-Code of Conduct\n\nEveryone participating in the _Pycln_ project, and in
-particular in the issue tracker,\nand pull requests is expected to treat other
-people with respect.\n\n---\n\nGive a â­ï¸ if this project helped you!\n',
-'author': 'Hadi Alqattan', 'author_email': 'alqattanhadizaki@gmail.com',
-'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://
-hadialqattan.github.io/pycln', 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'extras_require':
-extras_require, 'entry_points': entry_points, 'python_requires': '>=3.6.2,<4',
-} setup(**setup_kwargs)
+Metadata-Version: 2.1 Name: pycln Version: 2.1.4 Summary: A formatter for
+finding and removing unused import statements. Home-page: https://
+hadialqattan.github.io/pycln License: MIT Keywords: formatter,linter,quality-
+assurance,tools,cli Author: Hadi Alqattan Author-email:
+alqattanhadizaki@gmail.com Requires-Python: >=3.6.2,<4 Classifier: License ::
+OSI Approved :: MIT License Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.6 Classifier: Topic ::
+Utilities Requires-Dist: dataclasses (>=0.7,<0.8) ; python_version == "3.6"
+Requires-Dist: libcst (>=0.3.10,<0.4.0) ; python_version < "3.7" Requires-Dist:
+libcst (>=0.3.10,<0.5.0) ; python_version >= "3.7" Requires-Dist: pathspec
+(>=0.9.0,<0.10.0) Requires-Dist: pyyaml (>=5.3.1,<7.0.0) Requires-Dist: tomlkit
+(>=0.11.1,<0.12.0) Requires-Dist: typer (>=0.4.1,<0.10.0) Project-URL:
+Repository, https://github.com/hadialqattan/pycln Description-Content-Type:
+text/markdown [Logo]
+  ***** A formatter for finding and removing unused import statements. *****
+   [Pycln_Docs] [CI] [CD] [FUZZ] [Codacy_Badge] [Codecov] [Maintainability]
+ [PYPI - Python Version] [PYPI_-_Pycln_Version] [Total_Downloads] [Downloads]
+[Forks] [Stars] [Issues] [Pull_Requests] [Contributors] [Last_Commit] [License]
+   [Docstrings:_reStructuredText] [Code_style:_black] [Code_style:_prettier]
+--- **[Read the documentation on Github pages!](https://hadialqattan.github.io/
+pycln)** --- ## Installation and usage ### Installation Pycln requires Python
+3.6+ and can be easily installed using the most common Python packaging tools.
+We recommend installing the latest stable release from PyPI with pip: ```bash $
+pip install pycln ``` ### Usage By **default** Pycln will remove any unused
+import statement, So the simplest usage is to specify the path only: ```bash $
+pycln [PATH] ``` Also, it's possible to run `pycln` as a package: ```bash $
+python3 -m pycln [PATH] ``` NOTE: you may need to use `-a/--all` option for
+more satisfying results. see [-a/--all flag](https://hadialqattan.github.io/
+pycln/#/?id=-a-all-flag). Further information can be found in our docs: -
+[Usage and Configuration](https://hadialqattan.github.io/pycln/#/?id=usage) ##
+Configuration **Pycln** is able to read project-specific default values for its
+command line options from a configuration file like `pyproject.toml` or
+`setup.cfg`. This is especially useful for specifying custom CLI arguments/
+options like `path/paths`, `--include`, `--exclude`/`--extend-exclude`, or even
+`--all`. You can find more details in our documentation: - [--config [PATH] CLI
+option](https://hadialqattan.github.io/pycln/#/?id=-config-path-option) And if
+you're looking for more general configuration documentation: - [Usage and
+Configuration](https://hadialqattan.github.io/pycln/#/?id=usage) ## Used by The
+following notable open-source projects trust and use _Pycln_: - [cibuildwheel]
+(https://github.com/pypa/cibuildwheel) - [Open Event Server](https://
+github.com/fossasia/open-event-server) - [pybind11](https://github.com/pybind/
+pybind11) - [Poetry](https://github.com/python-poetry/poetry) - [Pyodide]
+(https://github.com/pyodide/pyodide) - [Rich](https://github.com/Textualize/
+rich) - [typeshed](https://github.com/python/typeshed) The following
+organizations use _Pycln_: - [FOSSASIA](https://github.com/fossasia) - [Poetry]
+(https://github.com/python-poetry) - [Python Packaging Authority](https://
+github.com/pypa) - [Scikit-HEP](https://github.com/scikit-hep) Are we missing
+anyone? Let us know. ## License MIT ## Contributing A big welcome for
+considering contributing to make the project better! You can get started by
+reading this: - [General guidlines](https://hadialqattan.github.io/pycln/#/
+CONTRIBUTING?id=general-guidelines) You can also dive directly into the
+technicalities: - [Contributing technicalities](https://hadialqattan.github.io/
+pycln/#/CONTRIBUTING?id=technicalities) ## Change log The log has become rather
+long. It moved to its own file. See [CHANGELOG](https://hadialqattan.github.io/
+pycln/#/CHANGELOG). ## Authors The author list is quite long nowadays, so it
+lives in its own file. See [AUTHORS](https://hadialqattan.github.io/pycln/#/
+AUTHORS) ## Code of Conduct Everyone participating in the _Pycln_ project, and
+in particular in the issue tracker, and pull requests is expected to treat
+other people with respect. --- Give a â­ï¸ if this project helped you!
```

