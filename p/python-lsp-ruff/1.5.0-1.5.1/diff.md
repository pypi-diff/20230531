# Comparing `tmp/python-lsp-ruff-1.5.0.tar.gz` & `tmp/python-lsp-ruff-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-lsp-ruff-1.5.0.tar", last modified: Tue May 30 09:06:21 2023, max compression
+gzip compressed data, was "python-lsp-ruff-1.5.1.tar", last modified: Wed May 31 08:35:02 2023, max compression
```

## Comparing `python-lsp-ruff-1.5.0.tar` & `python-lsp-ruff-1.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-05-30 09:06:21.785171 python-lsp-ruff-1.5.0/
--rw-r--r--   0 juli      (1000) juli      (1000)     1138 2022-12-05 16:14:35.000000 python-lsp-ruff-1.5.0/LICENSE
--rw-r--r--   0 juli      (1000) juli      (1000)     4733 2023-05-30 09:06:21.785171 python-lsp-ruff-1.5.0/PKG-INFO
--rw-r--r--   0 juli      (1000) juli      (1000)     4313 2023-05-30 09:00:09.000000 python-lsp-ruff-1.5.0/README.md
-drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-05-30 09:06:21.781838 python-lsp-ruff-1.5.0/pylsp_ruff/
--rw-r--r--   0 juli      (1000) juli      (1000)        0 2022-12-01 22:28:29.000000 python-lsp-ruff-1.5.0/pylsp_ruff/__init__.py
--rw-r--r--   0 juli      (1000) juli      (1000)    17445 2023-05-30 09:00:09.000000 python-lsp-ruff-1.5.0/pylsp_ruff/plugin.py
--rw-r--r--   0 juli      (1000) juli      (1000)      436 2023-05-30 07:34:43.000000 python-lsp-ruff-1.5.0/pylsp_ruff/ruff.py
--rw-r--r--   0 juli      (1000) juli      (1000)     1677 2023-05-30 09:00:09.000000 python-lsp-ruff-1.5.0/pylsp_ruff/settings.py
--rw-r--r--   0 juli      (1000) juli      (1000)      876 2023-05-30 09:01:11.000000 python-lsp-ruff-1.5.0/pyproject.toml
-drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-05-30 09:06:21.785171 python-lsp-ruff-1.5.0/python_lsp_ruff.egg-info/
--rw-r--r--   0 juli      (1000) juli      (1000)     4733 2023-05-30 09:06:21.000000 python-lsp-ruff-1.5.0/python_lsp_ruff.egg-info/PKG-INFO
--rw-r--r--   0 juli      (1000) juli      (1000)      414 2023-05-30 09:06:21.000000 python-lsp-ruff-1.5.0/python_lsp_ruff.egg-info/SOURCES.txt
--rw-r--r--   0 juli      (1000) juli      (1000)        1 2023-05-30 09:06:21.000000 python-lsp-ruff-1.5.0/python_lsp_ruff.egg-info/dependency_links.txt
--rw-r--r--   0 juli      (1000) juli      (1000)       33 2023-05-30 09:06:21.000000 python-lsp-ruff-1.5.0/python_lsp_ruff.egg-info/entry_points.txt
--rw-r--r--   0 juli      (1000) juli      (1000)      121 2023-05-30 09:06:21.000000 python-lsp-ruff-1.5.0/python_lsp_ruff.egg-info/requires.txt
--rw-r--r--   0 juli      (1000) juli      (1000)       11 2023-05-30 09:06:21.000000 python-lsp-ruff-1.5.0/python_lsp_ruff.egg-info/top_level.txt
--rw-r--r--   0 juli      (1000) juli      (1000)       38 2023-05-30 09:06:21.785171 python-lsp-ruff-1.5.0/setup.cfg
--rw-r--r--   0 juli      (1000) juli      (1000)       69 2023-01-14 19:42:55.000000 python-lsp-ruff-1.5.0/setup.py
-drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-05-30 09:06:21.785171 python-lsp-ruff-1.5.0/tests/
--rw-r--r--   0 juli      (1000) juli      (1000)     4179 2023-05-30 09:00:09.000000 python-lsp-ruff-1.5.0/tests/test_code_actions.py
--rw-r--r--   0 juli      (1000) juli      (1000)     7100 2023-05-30 09:00:09.000000 python-lsp-ruff-1.5.0/tests/test_ruff_lint.py
+drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-05-31 08:35:02.268412 python-lsp-ruff-1.5.1/
+-rw-r--r--   0 juli      (1000) juli      (1000)     1138 2022-12-05 16:14:35.000000 python-lsp-ruff-1.5.1/LICENSE
+-rw-r--r--   0 juli      (1000) juli      (1000)     4733 2023-05-31 08:35:02.268412 python-lsp-ruff-1.5.1/PKG-INFO
+-rw-r--r--   0 juli      (1000) juli      (1000)     4313 2023-05-30 09:00:09.000000 python-lsp-ruff-1.5.1/README.md
+drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-05-31 08:35:02.265079 python-lsp-ruff-1.5.1/pylsp_ruff/
+-rw-r--r--   0 juli      (1000) juli      (1000)        0 2022-12-01 22:28:29.000000 python-lsp-ruff-1.5.1/pylsp_ruff/__init__.py
+-rw-r--r--   0 juli      (1000) juli      (1000)    17445 2023-05-30 09:00:09.000000 python-lsp-ruff-1.5.1/pylsp_ruff/plugin.py
+-rw-r--r--   0 juli      (1000) juli      (1000)      436 2023-05-30 07:34:43.000000 python-lsp-ruff-1.5.1/pylsp_ruff/ruff.py
+-rw-r--r--   0 juli      (1000) juli      (1000)     1677 2023-05-30 09:00:09.000000 python-lsp-ruff-1.5.1/pylsp_ruff/settings.py
+-rw-r--r--   0 juli      (1000) juli      (1000)      876 2023-05-31 08:34:30.000000 python-lsp-ruff-1.5.1/pyproject.toml
+drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-05-31 08:35:02.268412 python-lsp-ruff-1.5.1/python_lsp_ruff.egg-info/
+-rw-r--r--   0 juli      (1000) juli      (1000)     4733 2023-05-31 08:35:02.000000 python-lsp-ruff-1.5.1/python_lsp_ruff.egg-info/PKG-INFO
+-rw-r--r--   0 juli      (1000) juli      (1000)      414 2023-05-31 08:35:02.000000 python-lsp-ruff-1.5.1/python_lsp_ruff.egg-info/SOURCES.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)        1 2023-05-31 08:35:02.000000 python-lsp-ruff-1.5.1/python_lsp_ruff.egg-info/dependency_links.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)       33 2023-05-31 08:35:02.000000 python-lsp-ruff-1.5.1/python_lsp_ruff.egg-info/entry_points.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)      121 2023-05-31 08:35:02.000000 python-lsp-ruff-1.5.1/python_lsp_ruff.egg-info/requires.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)       11 2023-05-31 08:35:02.000000 python-lsp-ruff-1.5.1/python_lsp_ruff.egg-info/top_level.txt
+-rw-r--r--   0 juli      (1000) juli      (1000)       38 2023-05-31 08:35:02.268412 python-lsp-ruff-1.5.1/setup.cfg
+-rw-r--r--   0 juli      (1000) juli      (1000)       69 2023-01-14 19:42:55.000000 python-lsp-ruff-1.5.1/setup.py
+drwxr-xr-x   0 juli      (1000) juli      (1000)        0 2023-05-31 08:35:02.268412 python-lsp-ruff-1.5.1/tests/
+-rw-r--r--   0 juli      (1000) juli      (1000)     4179 2023-05-30 09:00:09.000000 python-lsp-ruff-1.5.1/tests/test_code_actions.py
+-rw-r--r--   0 juli      (1000) juli      (1000)     7100 2023-05-30 09:00:09.000000 python-lsp-ruff-1.5.1/tests/test_ruff_lint.py
```

### Comparing `python-lsp-ruff-1.5.0/LICENSE` & `python-lsp-ruff-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-lsp-ruff-1.5.0/PKG-INFO` & `python-lsp-ruff-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lsp-ruff
-Version: 1.5.0
+Version: 1.5.1
 Summary: Ruff linting plugin for pylsp
 Author-email: Julian Hossbach <julian.hossbach@gmx.de>
 License: MIT
 Project-URL: Homepage, https://github.com/python-lsp/python-lsp-ruff
 Project-URL: Bug Tracker, https://github.com/python-lsp/python-lsp-ruff/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `python-lsp-ruff-1.5.0/README.md` & `python-lsp-ruff-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `python-lsp-ruff-1.5.0/pylsp_ruff/plugin.py` & `python-lsp-ruff-1.5.1/pylsp_ruff/plugin.py`

 * *Files identical despite different names*

### Comparing `python-lsp-ruff-1.5.0/pylsp_ruff/settings.py` & `python-lsp-ruff-1.5.1/pylsp_ruff/settings.py`

 * *Files identical despite different names*

### Comparing `python-lsp-ruff-1.5.0/pyproject.toml` & `python-lsp-ruff-1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-lsp-ruff"
 authors = [
   {name = "Julian Hossbach", email = "julian.hossbach@gmx.de"}
 ]
-version = "1.5.0"
+version = "1.5.1"
 description = "Ruff linting plugin for pylsp"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT"}
 dependencies = [
-  "ruff>=0.0.260",
+  "ruff>=0.0.267",
   "python-lsp-server",
   "lsprotocol>=2022.0.0a1",
   "tomli>=1.1.0; python_version < '3.11'",
 ]
 
 [project.optional-dependencies]
 dev = ["pytest", "pre-commit"]
```

### Comparing `python-lsp-ruff-1.5.0/python_lsp_ruff.egg-info/PKG-INFO` & `python-lsp-ruff-1.5.1/python_lsp_ruff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lsp-ruff
-Version: 1.5.0
+Version: 1.5.1
 Summary: Ruff linting plugin for pylsp
 Author-email: Julian Hossbach <julian.hossbach@gmx.de>
 License: MIT
 Project-URL: Homepage, https://github.com/python-lsp/python-lsp-ruff
 Project-URL: Bug Tracker, https://github.com/python-lsp/python-lsp-ruff/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `python-lsp-ruff-1.5.0/tests/test_code_actions.py` & `python-lsp-ruff-1.5.1/tests/test_code_actions.py`

 * *Files identical despite different names*

### Comparing `python-lsp-ruff-1.5.0/tests/test_ruff_lint.py` & `python-lsp-ruff-1.5.1/tests/test_ruff_lint.py`

 * *Files identical despite different names*

