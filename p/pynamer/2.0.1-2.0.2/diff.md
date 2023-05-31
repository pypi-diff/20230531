# Comparing `tmp/pynamer-2.0.1.tar.gz` & `tmp/pynamer-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-2.0.1.tar", last modified: Mon May 29 09:39:59 2023, max compression
+gzip compressed data, was "pynamer-2.0.2.tar", last modified: Wed May 31 14:21:50 2023, max compression
```

## Comparing `pynamer-2.0.1.tar` & `pynamer-2.0.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 09:39:59.348382 pynamer-2.0.1/
--rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.0.1/AUTHORS.md
--rw-rw-rw-   0        0        0     9767 2023-05-29 09:39:45.000000 pynamer-2.0.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.0.1/LICENSE
--rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0    18779 2023-05-29 09:39:59.348382 pynamer-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    17196 2023-05-28 18:04:36.000000 pynamer-2.0.1/README.md
--rw-rw-rw-   0        0        0     2287 2023-05-25 17:05:54.000000 pynamer-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1841 2023-05-29 09:39:59.348382 pynamer-2.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-29 09:39:58.957773 pynamer-2.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 09:39:59.067110 pynamer-2.0.1/src/pynamer/
--rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.0.1/src/pynamer/README.md
--rw-rw-rw-   0        0        0     1853 2023-05-29 09:39:46.000000 pynamer-2.0.1/src/pynamer/__init__.py
--rw-rw-rw-   0        0        0     9660 2023-05-24 15:55:39.000000 pynamer-2.0.1/src/pynamer/builder.py
--rw-rw-rw-   0        0        0     2210 2023-05-28 18:04:31.000000 pynamer-2.0.1/src/pynamer/cli.py
--rw-rw-rw-   0        0        0      726 2023-05-25 17:08:55.000000 pynamer-2.0.1/src/pynamer/config.py
--rw-rw-rw-   0        0        0       17 2023-05-28 17:55:42.000000 pynamer-2.0.1/src/pynamer/project_count.pickle
-drwxrwxrwx   0        0        0        0 2023-05-29 09:39:59.082723 pynamer-2.0.1/src/pynamer/project_name/
--rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.0.1/src/pynamer/project_name/__init__.py
--rw-rw-rw-   0        0        0     7702 2023-05-28 17:35:56.000000 pynamer-2.0.1/src/pynamer/pynamer.py
--rw-rw-rw-   0        0        0      386 2023-05-24 15:24:28.000000 pynamer-2.0.1/src/pynamer/setup.txt
--rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.0.1/src/pynamer/setup_base.txt
--rw-rw-rw-   0        0        0     9563 2023-05-28 18:04:31.000000 pynamer-2.0.1/src/pynamer/utils.py
--rw-rw-rw-   0        0        0     7738 2023-05-28 18:04:31.000000 pynamer-2.0.1/src/pynamer/validators.py
-drwxrwxrwx   0        0        0        0 2023-05-29 09:39:59.082723 pynamer-2.0.1/src/pynamer.egg-info/
--rw-rw-rw-   0        0        0    18779 2023-05-29 09:39:58.000000 pynamer-2.0.1/src/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1154 2023-05-29 09:39:58.000000 pynamer-2.0.1/src/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 09:39:58.000000 pynamer-2.0.1/src/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-29 09:39:58.000000 pynamer-2.0.1/src/pynamer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       74 2023-05-29 09:39:58.000000 pynamer-2.0.1/src/pynamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-29 09:39:58.000000 pynamer-2.0.1/src/pynamer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-29 09:39:59.348382 pynamer-2.0.1/tests/
--rw-rw-rw-   0        0        0     1869 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_args.py
--rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.0.1/tests/test_build_dist.py
--rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.0.1/tests/test_cleanup.py
--rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.0.1/tests/test_create_setup_file.py
--rw-rw-rw-   0        0        0     1541 2023-05-24 15:55:39.000000 pynamer-2.0.1/tests/test_defaults.py
--rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.0.1/tests/test_delete_director.py
--rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_feedback.py
--rw-rw-rw-   0        0        0     2698 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_final_analysis.py
--rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_find_pypirc_file.py
--rw-rw-rw-   0        0        0     1407 2023-05-24 15:55:39.000000 pynamer-2.0.1/tests/test_generate_pypi_index.py
--rw-rw-rw-   0        0        0      295 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_is_valid_package_name.py
--rw-rw-rw-   0        0        0     1721 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_ping_json.py
--rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_ping_project.py
--rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_process_input_file.py
--rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_pypi_search.py
--rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.0.1/tests/test_pypi_search_index.py
--rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.0.1/tests/test_rename_project_dir.py
--rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.0.1/tests/test_upload_dist.py
--rw-rw-rw-   0        0        0     1671 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_utils_version.py
--rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.0.1/tests/test_write_output_file.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:21:50.394847 pynamer-2.0.2/
+-rw-rw-rw-   0        0        0      172 2023-05-21 12:10:39.000000 pynamer-2.0.2/AUTHORS.md
+-rw-rw-rw-   0        0        0     9954 2023-05-31 14:21:35.000000 pynamer-2.0.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-05-21 12:10:39.000000 pynamer-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-05-21 12:10:39.000000 pynamer-2.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    18786 2023-05-31 14:21:50.394847 pynamer-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    17203 2023-05-29 12:32:43.000000 pynamer-2.0.2/README.md
+-rw-rw-rw-   0        0        0     2183 2023-05-30 13:20:57.000000 pynamer-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1818 2023-05-31 14:21:50.394847 pynamer-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      109 2023-04-21 12:29:15.000000 pynamer-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:21:50.067667 pynamer-2.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 14:21:50.131705 pynamer-2.0.2/src/pynamer/
+-rw-rw-rw-   0        0        0       11 2023-05-21 12:10:39.000000 pynamer-2.0.2/src/pynamer/README.md
+-rw-rw-rw-   0        0        0     1853 2023-05-31 14:21:35.000000 pynamer-2.0.2/src/pynamer/__init__.py
+-rw-rw-rw-   0        0        0     9736 2023-05-29 10:07:59.000000 pynamer-2.0.2/src/pynamer/builder.py
+-rw-rw-rw-   0        0        0     2210 2023-05-28 18:04:31.000000 pynamer-2.0.2/src/pynamer/cli.py
+-rw-rw-rw-   0        0        0      726 2023-05-25 17:08:55.000000 pynamer-2.0.2/src/pynamer/config.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:21:50.147333 pynamer-2.0.2/src/pynamer/project_name/
+-rw-rw-rw-   0        0        0        0 2023-05-21 12:10:39.000000 pynamer-2.0.2/src/pynamer/project_name/__init__.py
+-rw-rw-rw-   0        0        0     7524 2023-05-31 13:31:21.000000 pynamer-2.0.2/src/pynamer/pynamer.py
+-rw-rw-rw-   0        0        0      386 2023-05-24 15:24:28.000000 pynamer-2.0.2/src/pynamer/setup.txt
+-rw-rw-rw-   0        0        0      401 2023-05-21 12:10:39.000000 pynamer-2.0.2/src/pynamer/setup_base.txt
+-rw-rw-rw-   0        0        0     9587 2023-05-31 14:18:45.000000 pynamer-2.0.2/src/pynamer/utils.py
+-rw-rw-rw-   0        0        0     7788 2023-05-31 13:49:32.000000 pynamer-2.0.2/src/pynamer/validators.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:21:50.147333 pynamer-2.0.2/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0    18786 2023-05-31 14:21:49.000000 pynamer-2.0.2/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1130 2023-05-31 14:21:50.000000 pynamer-2.0.2/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 14:21:50.000000 pynamer-2.0.2/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-31 14:21:50.000000 pynamer-2.0.2/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2023-05-31 14:21:50.000000 pynamer-2.0.2/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-31 14:21:50.000000 pynamer-2.0.2/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 14:21:50.394847 pynamer-2.0.2/tests/
+-rw-rw-rw-   0        0        0     1869 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_args.py
+-rw-rw-rw-   0        0        0     2000 2023-05-24 15:55:39.000000 pynamer-2.0.2/tests/test_build_dist.py
+-rw-rw-rw-   0        0        0     1102 2023-05-24 15:55:39.000000 pynamer-2.0.2/tests/test_cleanup.py
+-rw-rw-rw-   0        0        0     1222 2023-05-24 15:55:39.000000 pynamer-2.0.2/tests/test_create_setup_file.py
+-rw-rw-rw-   0        0        0     1541 2023-05-24 15:55:39.000000 pynamer-2.0.2/tests/test_defaults.py
+-rw-rw-rw-   0        0        0      529 2023-05-24 15:55:39.000000 pynamer-2.0.2/tests/test_delete_director.py
+-rw-rw-rw-   0        0        0     1289 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_feedback.py
+-rw-rw-rw-   0        0        0     2698 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_final_analysis.py
+-rw-rw-rw-   0        0        0      738 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_find_pypirc_file.py
+-rw-rw-rw-   0        0        0     1407 2023-05-24 15:55:39.000000 pynamer-2.0.2/tests/test_generate_pypi_index.py
+-rw-rw-rw-   0        0        0      295 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_is_valid_package_name.py
+-rw-rw-rw-   0        0        0     1721 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_ping_json.py
+-rw-rw-rw-   0        0        0     1547 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_ping_project.py
+-rw-rw-rw-   0        0        0      522 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_process_input_file.py
+-rw-rw-rw-   0        0        0     1129 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_pypi_search.py
+-rw-rw-rw-   0        0        0      515 2023-05-24 15:55:39.000000 pynamer-2.0.2/tests/test_pypi_search_index.py
+-rw-rw-rw-   0        0        0      746 2023-05-24 15:55:39.000000 pynamer-2.0.2/tests/test_rename_project_dir.py
+-rw-rw-rw-   0        0        0      914 2023-05-24 15:55:39.000000 pynamer-2.0.2/tests/test_upload_dist.py
+-rw-rw-rw-   0        0        0     1707 2023-05-31 14:17:44.000000 pynamer-2.0.2/tests/test_utils_version.py
+-rw-rw-rw-   0        0        0      647 2023-05-21 12:10:39.000000 pynamer-2.0.2/tests/test_write_output_file.py
```

### Comparing `pynamer-2.0.1/CHANGELOG.md` & `pynamer-2.0.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.0.2 (2023-05-31)
+### Fix
+* Account for nonetype returned in json data ([`39f245c`](https://github.com/Stephen-RA-King/pynamer/commit/39f245c41b17add26ed9399dbb3c376cd395d79b))
+
 ## v2.0.1 (2023-05-29)
 ### Documentation
 * Final updates ([`6c85802`](https://github.com/Stephen-RA-King/pynamer/commit/6c85802a132e91586d8d21c0ceb6dcf8f011264d))
 
 ## v2.0.0 (2023-05-24)
 ### Documentation
 * Update citation ([`6cd655b`](https://github.com/Stephen-RA-King/pynamer/commit/6cd655bc1c9672fd5f64cbf63a78fc739a141328))
```

### Comparing `pynamer-2.0.1/LICENSE` & `pynamer-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/PKG-INFO` & `pynamer-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.0.1
+Version: 2.0.2
 Summary: Utility to find an available package name on the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -423,15 +423,15 @@
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/pynamer)
 [![](assets/www.png)](https://www.justpython.tech)
 [![](assets/email.png)](mailto:sking.github@gmail.com)
 
-Stephen R A King : [sking.github@gmail.com](sking.github@gmail.com)
+Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
 Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.2
 
 [![DOI](https://zenodo.org/badge/631029310.svg)](https://zenodo.org/badge/latestdoi/631029310)
```

### Comparing `pynamer-2.0.1/README.md` & `pynamer-2.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,15 @@
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/pynamer)
 [![](assets/www.png)](https://www.justpython.tech)
 [![](assets/email.png)](mailto:sking.github@gmail.com)
 
-Stephen R A King : [sking.github@gmail.com](sking.github@gmail.com)
+Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
 Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.2
 
 [![DOI](https://zenodo.org/badge/631029310.svg)](https://zenodo.org/badge/latestdoi/631029310)
```

### Comparing `pynamer-2.0.1/pyproject.toml` & `pynamer-2.0.2/pyproject.toml`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-[build-system]
-requires = [
-    "setuptools",
-    "wheel"
-]
-build-backend = "setuptools.build_meta"
-
-[tool]
-[tool.black]
-line-length = 88
-
-[tool.cruft]
-skip = [
-    "tests/",
-    "src/",
-    "*/header.png",
-    ".pypirc",
-    "CHANGELOG.md",
-    "setup.cfg"
-]
-
-[tool.isort]
-import_heading_stdlib = "Core Library modules"
-import_heading_thirdparty = "Third party modules"
-import_heading_firstparty = "First party modules"
-import_heading_localfolder = "Local modules"
-include_trailing_comma = true
-indent = '    '
-known_third_party = [
-    "click",
-    "pytest",
-    "setuptools",
-    "pip-tools",
-    "pre-commit"
-]
-known_first_party = [
-    "pathmagic"
-]
-line_length = 80
-multi_line_output = 3
-force_grid_wrap = 0
-use_parentheses = true
-ensure_newline_before_comments = true
-balanced_wrapping = true
-combine_as_imports = true
-
-[tool.mypy]
-ignore_missing_imports = true
-check_untyped_defs = true
-disallow_untyped_defs = false
-warn_unused_ignores = true
-strict_optional = true
-warn_redundant_casts = true
-warn_unused_configs = true
-disallow_untyped_calls = false
-disallow_incomplete_defs = true
-follow_imports = "skip"
-html_report = "reports/mypy"
-cache_dir = 'cache/.mypy_cache'
-mypy_path = "typeshed/pyi:typeshed/imports"
-exclude = [
-    '^tests/[\w]*.py$',
-    '^tools/[\w]*.py$',
-    '^tasks.py$'
-]
-
-[tool.semantic_release]
-version_variable = [
-    "src/pynamer/__init__.py:__version__",
-    "docs/conf.py:version",
-]
-branch = "main"
-changelog_file = "CHANGELOG.md"
-build_command = "python -m build"
-dist_path = "dist/"
-upload_to_pypi = true
-upload_to_repository = true
-remove_dist = true
-version_source = "tag"
-commit_message = "chore: generate by PSR"
-
-[tool.flakeheaven]
-# base = "https://raw.githubusercontent.com/flakeheaven/flakeheaven/main/pyproject.toml"
-exclude = ["example.py"]
-format = "grouped"
-max_line_length = 80
-show_source = true
-
-[tool.flakeheaven.plugins]
-pyflakes = ["+*", "-F401"]
-"flake8-*" = ["+*"]
-mccabe = ["+*"]
-pep8-naming = ["+*"]
-pycodestyle = ["+*"]
-pylint = ["+F*", "+E*", "-E0611", "-E1101", "-E0401", "-E1102", "-E1123"]
-
-[tool.coverage.run]
-branch = true
-parallel = true
-
-[tool.coverage.report]
-show_missing = true
-precision = 2
-skip_empty = true
+[build-system]
+requires = [
+    "setuptools",
+    "wheel"
+]
+build-backend = "setuptools.build_meta"
+
+[tool]
+[tool.black]
+line-length = 88
+
+[tool.cruft]
+skip = [
+    "tests/",
+    "src/",
+    "*/header.png",
+    ".pypirc",
+    "CHANGELOG.md",
+    "setup.cfg"
+]
+
+[tool.isort]
+import_heading_stdlib = "Core Library modules"
+import_heading_thirdparty = "Third party modules"
+import_heading_firstparty = "First party modules"
+import_heading_localfolder = "Local modules"
+include_trailing_comma = true
+indent = '    '
+known_third_party = [
+    "click",
+    "pytest",
+    "setuptools",
+    "pip-tools",
+    "pre-commit"
+]
+known_first_party = [
+    "pathmagic"
+]
+line_length = 80
+multi_line_output = 3
+force_grid_wrap = 0
+use_parentheses = true
+ensure_newline_before_comments = true
+balanced_wrapping = true
+combine_as_imports = true
+
+[tool.mypy]
+ignore_missing_imports = true
+check_untyped_defs = true
+disallow_untyped_defs = false
+warn_unused_ignores = true
+strict_optional = true
+warn_redundant_casts = true
+warn_unused_configs = true
+disallow_untyped_calls = false
+disallow_incomplete_defs = true
+follow_imports = "skip"
+html_report = "reports/mypy"
+cache_dir = 'cache/.mypy_cache'
+mypy_path = "typeshed/pyi:typeshed/imports"
+exclude = [
+    '^tests/[\w]*.py$',
+    '^tools/[\w]*.py$',
+    '^tasks.py$'
+]
+
+[tool.semantic_release]
+version_variable = [
+    "src/pynamer/__init__.py:__version__",
+    "docs/conf.py:version",
+]
+branch = "main"
+changelog_file = "CHANGELOG.md"
+build_command = "python -m build"
+dist_path = "dist/"
+upload_to_pypi = true
+upload_to_repository = true
+remove_dist = true
+version_source = "tag"
+commit_message = "chore: generate by PSR"
+
+[tool.flakeheaven]
+# base = "https://raw.githubusercontent.com/flakeheaven/flakeheaven/main/pyproject.toml"
+exclude = ["example.py"]
+format = "grouped"
+max_line_length = 80
+show_source = true
+
+[tool.flakeheaven.plugins]
+pyflakes = ["+*", "-F401"]
+"flake8-*" = ["+*"]
+mccabe = ["+*"]
+pep8-naming = ["+*"]
+pycodestyle = ["+*"]
+pylint = ["+F*", "+E*", "-E0611", "-E1101", "-E0401", "-E1102", "-E1123"]
+
+[tool.coverage.run]
+branch = true
+parallel = true
+
+[tool.coverage.report]
+show_missing = true
+precision = 2
+skip_empty = true
```

### Comparing `pynamer-2.0.1/setup.cfg` & `pynamer-2.0.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -79,38 +79,36 @@
 000004e0: 6c0d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  l....[options.pa
 000004f0: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
 00000500: 6572 6520 3d20 7372 630d 0a0d 0a5b 6f70  ere = src....[op
 00000510: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
 00000520: 7461 5d0d 0a70 796e 616d 6572 203d 200d  ta]..pynamer = .
 00000530: 0a09 5245 4144 4d45 2e6d 640d 0a09 636f  ..README.md...co
 00000540: 6e66 6967 2e70 790d 0a09 7072 6f6a 6563  nfig.py...projec
-00000550: 745f 636f 756e 742e 7069 636b 6c65 0d0a  t_count.pickle..
-00000560: 0970 726f 6a65 6374 5f6e 616d 650d 0a09  .project_name...
-00000570: 7072 6f6a 6563 745f 6e61 6d65 2f5f 5f69  project_name/__i
-00000580: 6e69 745f 5f2e 7079 0d0a 0973 6574 7570  nit__.py...setup
-00000590: 2e74 7874 0d0a 0973 6574 7570 5f62 6173  .txt...setup_bas
-000005a0: 652e 7478 740d 0a09 7574 696c 732e 7079  e.txt...utils.py
-000005b0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 6e74  ....[options.ent
-000005c0: 7279 5f70 6f69 6e74 735d 0d0a 636f 6e73  ry_points]..cons
-000005d0: 6f6c 655f 7363 7269 7074 7320 3d20 0d0a  ole_scripts = ..
-000005e0: 0970 796e 616d 6572 203d 2070 796e 616d  .pynamer = pynam
-000005f0: 6572 2e70 796e 616d 6572 3a6d 6169 6e0d  er.pynamer:main.
-00000600: 0a0d 0a5b 666c 616b 6538 5d0d 0a64 6f63  ...[flake8]..doc
-00000610: 7374 7269 6e67 2d63 6f6e 7665 6e74 696f  string-conventio
-00000620: 6e20 3d20 6e75 6d70 790d 0a6d 6178 2d63  n = numpy..max-c
-00000630: 6f6d 706c 6578 6974 7920 3d20 3138 0d0a  omplexity = 18..
-00000640: 6d61 782d 6c69 6e65 2d6c 656e 6774 6820  max-line-length 
-00000650: 3d20 3838 0d0a 7365 6c65 6374 203d 2042  = 88..select = B
-00000660: 2c20 4239 2c20 432c 2044 2c20 452c 2046  , B9, C, D, E, F
-00000670: 2c20 4e2c 2057 0d0a 6578 636c 7564 6520  , N, W..exclude 
-00000680: 3d20 7465 7374 732f 2a2c 2e74 6f78 2f2a  = tests/*,.tox/*
-00000690: 2c2e 6e6f 782f 2a2c 646f 6373 2f2a 2c2e  ,.nox/*,docs/*,.
-000006a0: 6769 742f 2a2c 2e67 6974 6875 622f 2a0d  git/*,.github/*.
-000006b0: 0a69 676e 6f72 6520 3d20 0d0a 0945 3230  .ignore = ...E20
-000006c0: 332c 0d0a 0957 3530 332c 0d0a 7065 722d  3,...W503,..per-
-000006d0: 6669 6c65 2d69 676e 6f72 6573 203d 200d  file-ignores = .
-000006e0: 0a09 7079 6e61 6d65 722e 7079 3a43 3930  ..pynamer.py:C90
-000006f0: 310d 0a09 6275 696c 6465 722e 7079 3a43  1...builder.py:C
-00000700: 3930 310d 0a0d 0a5b 6567 675f 696e 666f  901....[egg_info
-00000710: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000720: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000730: 0a                                       .
+00000550: 745f 6e61 6d65 0d0a 0970 726f 6a65 6374  t_name...project
+00000560: 5f6e 616d 652f 5f5f 696e 6974 5f5f 2e70  _name/__init__.p
+00000570: 790d 0a09 7365 7475 702e 7478 740d 0a09  y...setup.txt...
+00000580: 7365 7475 705f 6261 7365 2e74 7874 0d0a  setup_base.txt..
+00000590: 0975 7469 6c73 2e70 790d 0a0d 0a5b 6f70  .utils.py....[op
+000005a0: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
+000005b0: 7473 5d0d 0a63 6f6e 736f 6c65 5f73 6372  ts]..console_scr
+000005c0: 6970 7473 203d 200d 0a09 7079 6e61 6d65  ipts = ...pyname
+000005d0: 7220 3d20 7079 6e61 6d65 722e 7079 6e61  r = pynamer.pyna
+000005e0: 6d65 723a 6d61 696e 0d0a 0d0a 5b66 6c61  mer:main....[fla
+000005f0: 6b65 385d 0d0a 646f 6373 7472 696e 672d  ke8]..docstring-
+00000600: 636f 6e76 656e 7469 6f6e 203d 206e 756d  convention = num
+00000610: 7079 0d0a 6d61 782d 636f 6d70 6c65 7869  py..max-complexi
+00000620: 7479 203d 2031 380d 0a6d 6178 2d6c 696e  ty = 18..max-lin
+00000630: 652d 6c65 6e67 7468 203d 2038 380d 0a73  e-length = 88..s
+00000640: 656c 6563 7420 3d20 422c 2042 392c 2043  elect = B, B9, C
+00000650: 2c20 442c 2045 2c20 462c 204e 2c20 570d  , D, E, F, N, W.
+00000660: 0a65 7863 6c75 6465 203d 2074 6573 7473  .exclude = tests
+00000670: 2f2a 2c2e 746f 782f 2a2c 2e6e 6f78 2f2a  /*,.tox/*,.nox/*
+00000680: 2c64 6f63 732f 2a2c 2e67 6974 2f2a 2c2e  ,docs/*,.git/*,.
+00000690: 6769 7468 7562 2f2a 0d0a 6967 6e6f 7265  github/*..ignore
+000006a0: 203d 200d 0a09 4532 3033 2c0d 0a09 5735   = ...E203,...W5
+000006b0: 3033 2c0d 0a70 6572 2d66 696c 652d 6967  03,..per-file-ig
+000006c0: 6e6f 7265 7320 3d20 0d0a 0970 796e 616d  nores = ...pynam
+000006d0: 6572 2e70 793a 4339 3031 0d0a 0962 7569  er.py:C901...bui
+000006e0: 6c64 6572 2e70 793a 4339 3031 0d0a 0d0a  lder.py:C901....
+000006f0: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+00000700: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+00000710: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

### Comparing `pynamer-2.0.1/src/pynamer/__init__.py` & `pynamer-2.0.2/src/pynamer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pickle
 from importlib.resources import files
 
 # Third party modules
 import yaml
 
 __title__ = "pynamer"
-__version__ = "2.0.1"
+__version__ = "2.0.2"
 __author__ = "Stephen R A King"
 __description__ = (
     "Utility to find an available package name in the PyPI repository and register it "
 )
 __email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Stephen R A King"
```

### Comparing `pynamer-2.0.1/src/pynamer/builder.py` & `pynamer-2.0.2/src/pynamer/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-
+"""Collection of functions to build a minimal package and upload to PyPI."""
 # Core Library modules
 import os
 import pickle
 import re
 import shutil
 import subprocess
 import sys
```

### Comparing `pynamer-2.0.1/src/pynamer/cli.py` & `pynamer-2.0.2/src/pynamer/cli.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/src/pynamer/config.py` & `pynamer-2.0.2/src/pynamer/config.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/src/pynamer/pynamer.py` & `pynamer-2.0.2/src/pynamer/pynamer.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,15 @@
     args, parser = _parse_args(sys.argv[1:])
     logger.debug(" args: %s", args)
 
     if args.generate:
         _generate_pypi_index()
 
     if args.version:
-        version, message, result = _check_version()  # type: ignore
-        if result:
-            _feedback(f"{version} : {message}", "nominal")
-        else:
-            _feedback(f"{version} : {message}", "warning")
+        _check_version()  # type: ignore
 
     if args.projects == "None" and args.file == "None" and args.register:
         _feedback("You need to specify a project name to register it", "error")
         raise SystemExit()
 
     if args.projects == "None" and args.file == "None" and args.meta:
         _feedback(
```

### Comparing `pynamer-2.0.1/src/pynamer/utils.py` & `pynamer-2.0.2/src/pynamer/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-
+"""Collection of package support utilities."""
 # Core Library modules
 import json
 import os
 import pickle
 import re
 from importlib.resources import as_file
 from pathlib import Path
@@ -133,15 +133,15 @@
         elif diff < 0:  # pragma: no cover
             _feedback(
                 f"Project count has decreased by {diff} since last index generation",
                 "warning",
             )
 
 
-def _check_version() -> Union[tuple[version, str, bool], None]:
+def _check_version() -> None:
     """Utility function to compare package version against latest version on PyPI.
 
     Returns:
         current_version:    version of the installed package.
         str:                Message concerning the result of the comparison.
         bool:               True: if the installed package is up-to-date.
                             False: if there is a newer version on PyPI.
@@ -152,22 +152,19 @@
         project_json_raw = requests.get(url_json, timeout=5)
     except requests.RequestException:
         raise SystemExit("An error occurred with an HTTP request")
     if project_json_raw.status_code == 200:
         project_json = json.loads(project_json_raw.content)
         pypi_version = version.parse(project_json["info"]["version"])
         if pypi_version > current_version:
-            return (
-                current_version,
-                f"(There is a newer version available: {pypi_version})",
-                False,
-            )
+            message = f"(There is a newer version available: {pypi_version})"
+            _feedback(f"{current_version} : {message}", "warning")
         elif pypi_version == current_version:
-            return current_version, "(You have the most recent version)", True
-    return None
+            message = "(You have the most recent version)"
+            _feedback(f"{current_version} : {message}", "nominal")
 
 
 def _process_input_file(file: str) -> list[Union[str, Any]]:
     """Processes the contents of the file to a list of strings.
 
     Args:
         file:           simple string for the file.
```

### Comparing `pynamer-2.0.1/src/pynamer/validators.py` & `pynamer-2.0.2/src/pynamer/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+"""Collection of functions to test availability of a package name on PyPI"""
 # Core Library modules
 import json
 import re
 import string
 from datetime import datetime
 from typing import Any, Union
 
@@ -76,25 +77,19 @@
     try:
         project_json_raw = requests.get(url_json, timeout=5)
     except requests.RequestException as e:
         logger.error("An error occurred: %s", e)
         raise SystemExit("An error occurred with an HTTP request")
     if project_json_raw.status_code == 200:
         project_json = json.loads(project_json_raw.content)
-        result = "".join(
-            [
-                project_json["info"]["author"],
-                "\n",
-                project_json["info"]["author_email"],
-                "\n",
-                project_json["info"]["version"],
-                "\n",
-                project_json["info"]["summary"],
-            ]
-        )
+        author = project_json["info"]["author"] or ""
+        email = project_json["info"]["author_email"] or ""
+        version = project_json["info"]["version"] or ""
+        summary = project_json["info"]["summary"] or ""
+        result = "".join([author, "\n", email, "\n", version, "\n", summary])
         return result
     logger.debug("No response from JSON URL")
     return ""
 
 
 def _pypi_search_index(project_name: str) -> bool:
     """Open the generated index file and search for the project name.
```

### Comparing `pynamer-2.0.1/src/pynamer.egg-info/PKG-INFO` & `pynamer-2.0.2/src/pynamer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 2.0.1
+Version: 2.0.2
 Summary: Utility to find an available package name on the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
@@ -423,15 +423,15 @@
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/pynamer)
 [![](assets/www.png)](https://www.justpython.tech)
 [![](assets/email.png)](mailto:sking.github@gmail.com)
 
-Stephen R A King : [sking.github@gmail.com](sking.github@gmail.com)
+Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
 Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.2
 
 [![DOI](https://zenodo.org/badge/631029310.svg)](https://zenodo.org/badge/latestdoi/631029310)
```

### Comparing `pynamer-2.0.1/src/pynamer.egg-info/SOURCES.txt` & `pynamer-2.0.2/src/pynamer.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 AUTHORS.md
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
+setup.py
 src/pynamer/README.md
 src/pynamer/__init__.py
 src/pynamer/builder.py
 src/pynamer/cli.py
 src/pynamer/config.py
-src/pynamer/project_count.pickle
 src/pynamer/pynamer.py
 src/pynamer/setup.txt
 src/pynamer/setup_base.txt
 src/pynamer/utils.py
 src/pynamer/validators.py
 src/pynamer.egg-info/PKG-INFO
 src/pynamer.egg-info/SOURCES.txt
```

### Comparing `pynamer-2.0.1/tests/test_args.py` & `pynamer-2.0.2/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/tests/test_build_dist.py` & `pynamer-2.0.2/tests/test_build_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/tests/test_cleanup.py` & `pynamer-2.0.2/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/tests/test_create_setup_file.py` & `pynamer-2.0.2/tests/test_create_setup_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/tests/test_defaults.py` & `pynamer-2.0.2/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/tests/test_delete_director.py` & `pynamer-2.0.2/tests/test_delete_director.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/tests/test_feedback.py` & `pynamer-2.0.2/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/tests/test_final_analysis.py` & `pynamer-2.0.2/tests/test_final_analysis.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/tests/test_find_pypirc_file.py` & `pynamer-2.0.2/tests/test_find_pypirc_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/tests/test_generate_pypi_index.py` & `pynamer-2.0.2/tests/test_generate_pypi_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/tests/test_ping_json.py` & `pynamer-2.0.2/tests/test_ping_json.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/tests/test_ping_project.py` & `pynamer-2.0.2/tests/test_ping_project.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/tests/test_process_input_file.py` & `pynamer-2.0.2/tests/test_process_input_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/tests/test_pypi_search.py` & `pynamer-2.0.2/tests/test_pypi_search.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/tests/test_pypi_search_index.py` & `pynamer-2.0.2/tests/test_pypi_search_index.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/tests/test_rename_project_dir.py` & `pynamer-2.0.2/tests/test_rename_project_dir.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/tests/test_upload_dist.py` & `pynamer-2.0.2/tests/test_upload_dist.py`

 * *Files identical despite different names*

### Comparing `pynamer-2.0.1/tests/test_utils_version.py` & `pynamer-2.0.2/tests/test_utils_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,50 @@
-#!/usr/bin/env python3
-# Core Library modules
-import pickle
-from pathlib import Path
-
-# Third party modules
-import pytest
-import requests
-from requests.exceptions import ConnectTimeout
-
-# First party modules
-import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-
-
-def my_custom_get_found(url, **kwargs):
-    _pickle_file = BASE_DIR / "resources" / "requests_get_json_pynamer.pickle"
-    _pickle_bytes = _pickle_file.read_bytes()
-    pickle_content = pickle.loads(_pickle_bytes)
-    return pickle_content
-
-
-def test_utils_version_old(monkeypatch):
-    monkeypatch.setattr(requests, "get", my_custom_get_found)
-    monkeypatch.setattr(pynamer, "__version__", "1.0.0")
-
-    pypi_version, message, result = pynamer.utils._check_version()
-
-    assert str(pypi_version) == "1.0.0"
-    assert message == "(There is a newer version available: 1.1.0)"
-    assert result is False
-
-
-def test_utils_version(monkeypatch):
-    monkeypatch.setattr(requests, "get", my_custom_get_found)
-    monkeypatch.setattr(pynamer, "__version__", "1.1.0")
-
-    pypi_version, message, result = pynamer.utils._check_version()
-
-    assert str(pypi_version) == "1.1.0"
-    assert message == "(You have the most recent version)"
-    assert result is True
-
-
-def test_ping_json_error(monkeypatch):
-    def mock_requests_error(*args, **kwargs):
-        raise ConnectTimeout("Connection timed out")
-
-    monkeypatch.setattr(requests, "get", mock_requests_error)
-
-    with pytest.raises(SystemExit) as excinfo:
-        pypi_version, message, result = pynamer.utils._check_version()
-    assert str(excinfo.value) == "An error occurred with an HTTP request"
+#!/usr/bin/env python3
+# Core Library modules
+import pickle
+from pathlib import Path
+
+# Third party modules
+import pytest
+import requests
+from colorama import Back, Fore, Style
+from requests.exceptions import ConnectTimeout
+
+# First party modules
+import pynamer
+
+BASE_DIR = Path(__file__).parents[0]
+
+
+def my_custom_get_found(url, **kwargs):
+    _pickle_file = BASE_DIR / "resources" / "requests_get_json_pynamer.pickle"
+    _pickle_bytes = _pickle_file.read_bytes()
+    pickle_content = pickle.loads(_pickle_bytes)
+    return pickle_content
+
+
+def test_utils_version_old(monkeypatch, capfd):
+    monkeypatch.setattr(requests, "get", my_custom_get_found)
+    monkeypatch.setattr(pynamer, "__version__", "1.0.0")
+    result = f"{Fore.YELLOW}{Back.BLACK}{Style.BRIGHT}1.0.0 : (There is a newer version available: 1.1.0){Style.RESET_ALL}\n"
+    pynamer.utils._check_version()
+    captured = capfd.readouterr()
+    assert captured.out == result
+
+
+def test_utils_version(monkeypatch, capfd):
+    monkeypatch.setattr(requests, "get", my_custom_get_found)
+    monkeypatch.setattr(pynamer, "__version__", "1.1.0")
+    result = f"{Fore.GREEN}{Style.BRIGHT}1.1.0 : (You have the most recent version){Style.RESET_ALL}\n"
+    pynamer.utils._check_version()
+    captured = capfd.readouterr()
+    assert captured.out == result
+
+
+def test_ping_json_error(monkeypatch):
+    def mock_requests_error(*args, **kwargs):
+        raise ConnectTimeout("Connection timed out")
+
+    monkeypatch.setattr(requests, "get", mock_requests_error)
+    with pytest.raises(SystemExit) as excinfo:
+        pypi_version, message, result = pynamer.utils._check_version()
+    assert str(excinfo.value) == "An error occurred with an HTTP request"
```

### Comparing `pynamer-2.0.1/tests/test_write_output_file.py` & `pynamer-2.0.2/tests/test_write_output_file.py`

 * *Files identical despite different names*

