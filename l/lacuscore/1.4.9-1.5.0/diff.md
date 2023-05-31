# Comparing `tmp/lacuscore-1.4.9.tar.gz` & `tmp/lacuscore-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacuscore-1.4.9.tar", max compression
+gzip compressed data, was "lacuscore-1.5.0.tar", max compression
```

## Comparing `lacuscore-1.4.9.tar` & `lacuscore-1.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.4.9/LICENSE
--rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.4.9/README.md
--rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.4.9/lacuscore/__init__.py
--rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.4.9/lacuscore/lacus_monitoring.py
--rw-r--r--   0        0        0    28455 2023-04-14 13:46:44.792327 lacuscore-1.4.9/lacuscore/lacuscore.py
--rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.4.9/lacuscore/py.typed
--rw-r--r--   0        0        0     1516 2023-04-14 13:47:44.812598 lacuscore-1.4.9/pyproject.toml
--rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 lacuscore-1.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.5.0/LICENSE
+-rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.5.0/README.md
+-rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.5.0/lacuscore/__init__.py
+-rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.5.0/lacuscore/lacus_monitoring.py
+-rw-r--r--   0        0        0    28455 2023-04-14 13:46:44.792327 lacuscore-1.5.0/lacuscore/lacuscore.py
+-rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.5.0/lacuscore/py.typed
+-rw-r--r--   0        0        0     1596 2023-05-31 08:48:08.026719 lacuscore-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 lacuscore-1.5.0/PKG-INFO
```

### Comparing `lacuscore-1.4.9/LICENSE` & `lacuscore-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.9/README.md` & `lacuscore-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.9/lacuscore/lacus_monitoring.py` & `lacuscore-1.5.0/lacuscore/lacus_monitoring.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.9/lacuscore/lacuscore.py` & `lacuscore-1.5.0/lacuscore/lacuscore.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.9/pyproject.toml` & `lacuscore-1.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacuscore"
-version = "1.4.9"
+version = "1.5.0"
 description = "Core of Lacus, usable as a module"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/LacusCore"
 documentation = "https://lacuscore.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -26,27 +26,30 @@
     'Topic :: Internet',
 ]
 
 include = ['README.md']
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests = "^2.28.2"
-Sphinx = { version = "^6.1.3", optional = true }
-playwrightcapture = {extras = ["recaptcha"], version = "^1.19.9"}
+requests = "^2.31.0"
+Sphinx = { version = "^7.0.1", optional = true }
+playwrightcapture = {extras = ["recaptcha"], version = "^1.20.0"}
 defang = "^0.5.3"
 ua-parser = "^0.16.1"
-redis = {version = "^4.5.4", extras = ["hiredis"]}
+redis = {version = "^4.5.5", extras = ["hiredis"]}
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
 [tool.poetry.group.dev.dependencies]
-types-redis = {version = "^4.5.4.1"}
-mypy = "^1.2.0"
-types-requests = "^2.28.11.17"
-ipython = "^8.12.0"
-pytest = "^7.3.0"
+types-redis = {version = "^4.5.5.2"}
+mypy = "^1.3.0"
+types-requests = "^2.31.0.1"
+ipython = [
+    {version = "<8.13.0", python = "<3.9"},
+    {version = "^8.13.0", python = ">=3.9"}
+]
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry_core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lacuscore-1.4.9/PKG-INFO` & `lacuscore-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacuscore
-Version: 1.4.9
+Version: 1.5.0
 Summary: Core of Lacus, usable as a module
 Home-page: https://github.com/ail-project/LacusCore
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,19 +23,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
-Requires-Dist: Sphinx (>=6.1.3,<7.0.0) ; extra == "docs"
+Requires-Dist: Sphinx (>=7.0.1,<8.0.0) ; extra == "docs"
 Requires-Dist: defang (>=0.5.3,<0.6.0)
-Requires-Dist: playwrightcapture[recaptcha] (>=1.19.9,<2.0.0)
-Requires-Dist: redis[hiredis] (>=4.5.4,<5.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: playwrightcapture[recaptcha] (>=1.20.0,<2.0.0)
+Requires-Dist: redis[hiredis] (>=4.5.5,<5.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ua-parser (>=0.16.1,<0.17.0)
 Project-URL: Documentation, https://lacuscore.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/ail-project/LacusCore
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/lacuscore/badge/?version=latest)](https://lacuscore.readthedocs.io/en/latest/?badge=latest)
```

