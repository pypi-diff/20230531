# Comparing `tmp/mitm_chrome-0.2.0.tar.gz` & `tmp/mitm_chrome-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitm_chrome-0.2.0.tar", max compression
+gzip compressed data, was "mitm_chrome-0.3.0.tar", last modified: Wed May 31 15:57:05 2023, max compression
```

## Comparing `mitm_chrome-0.2.0.tar` & `mitm_chrome-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,5 @@
--rw-r--r--   0        0        0      170 2022-03-23 14:57:04.978880 mitm_chrome-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1063 2022-03-23 14:57:04.978880 mitm_chrome-0.2.0/LICENSE
--rw-r--r--   0        0        0      304 2022-03-23 14:57:04.978880 mitm_chrome-0.2.0/README.md
--rw-r--r--   0        0        0     4366 2022-03-23 14:57:04.978880 mitm_chrome-0.2.0/mitm_chrome/__init__.py
--rw-r--r--   0        0        0       71 2022-03-23 14:57:04.978880 mitm_chrome-0.2.0/mitm_chrome/__main__.py
--rw-r--r--   0        0        0     1281 2022-03-23 14:57:04.978880 mitm_chrome-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1092 2022-03-23 14:57:12.647674 mitm_chrome-0.2.0/setup.py
--rw-r--r--   0        0        0     1164 2022-03-23 14:57:12.647915 mitm_chrome-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      170 2023-05-31 15:56:56.524227 mitm_chrome-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1063 2023-05-31 15:56:56.524227 mitm_chrome-0.3.0/LICENSE
+-rw-r--r--   0        0        0      304 2023-05-31 15:56:56.524227 mitm_chrome-0.3.0/README.md
+-rw-r--r--   0        0        0     1406 2023-05-31 15:57:05.828233 mitm_chrome-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 mitm_chrome-0.3.0/PKG-INFO
```

### Comparing `mitm_chrome-0.2.0/LICENSE` & `mitm_chrome-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mitm_chrome-0.2.0/pyproject.toml` & `mitm_chrome-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,63 @@
-[tool.poetry]
+[project]
 name = "mitm_chrome"
-version = "0.2.0"
+version = "0.3.0"
 description = "Integrate chrome with mitmproxy."
-license = "MIT"
-authors = ["林玮 (Jade Lin) <linw1995@icloud.com>"]
+authors = [
+    { name = "林玮 (Jade Lin)", email = "linw1995@icloud.com" },
+]
+dependencies = [
+    "mitmproxy<10,>=9",
+]
+requires-python = ">=3.10,<4.0"
 readme = "README.md"
-homepage = "https://github.com/linw1995/mitm_chrome"
-repository = "https://github.com/linw1995/mitm_chrome"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Development Status :: 4 - Beta",
     "Operating System :: POSIX",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
 ]
-include = ["CHANGELOG.md"]
 
-[tool.poetry.scripts]
-mitm_chrome = 'mitm_chrome:cli'
+[project.license]
+text = "MIT"
 
-[tool.poetry.dependencies]
-python = "^3.9"
-mitmproxy = "^8"
+[project.urls]
+homepage = "https://github.com/linw1995/mitm_chrome"
+repository = "https://github.com/linw1995/mitm_chrome"
 
-[tool.poetry.dev-dependencies]
-flake8-bugbear = "^20.11.1"
+[project.scripts]
+mitm_chrome = "mitm_chrome:cli"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 version = "0.1.2"
-version_files = ["pyproject.toml:version"]
+version_files = [
+    "pyproject.toml:version",
+]
 tag_format = "$version"
 
 [tool.isort]
-profile='black'
+profile = "black"
+import_heading_stdlib = "Standard Library"
+import_heading_thirdparty = "Third Party Library"
+import_heading_firstparty = "First Party Library"
+import_heading_localfolder = "Local Folder"
+
+[tool.pdm.dev-dependencies]
+dev = [
+    "flake8-bugbear<21.0.0,>=20.11.1",
+]
 
-import_heading_stdlib='Standard Library'
-import_heading_thirdparty='Third Party Library'
-import_heading_firstparty='First Party Library'
-import_heading_localfolder='Local Folder'
+[tool.pdm.build]
+includes = [
+    "CHANGELOG.md",
+]
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
```

### Comparing `mitm_chrome-0.2.0/PKG-INFO` & `mitm_chrome-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: mitm-chrome
-Version: 0.2.0
+Version: 0.3.0
 Summary: Integrate chrome with mitmproxy.
 Home-page: https://github.com/linw1995/mitm_chrome
+Author-Email: 林玮 (Jade Lin) <linw1995@icloud.com>
 License: MIT
-Author: 林玮 (Jade Lin)
-Author-email: linw1995@icloud.com
-Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: mitmproxy (>=8,<9)
+Classifier: Development Status :: 4 - Beta
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Project-URL: Homepage, https://github.com/linw1995/mitm_chrome
 Project-URL: Repository, https://github.com/linw1995/mitm_chrome
+Requires-Python: <4.0,>=3.10
+Requires-Dist: mitmproxy<10,>=9
 Description-Content-Type: text/markdown
 
 # mitm chrome
 
 Integrate chrome with [mitmproxy](https://mitmproxy.org/).
 
 ## installation
@@ -40,8 +38,7 @@
 ```
 
 Else
 
 ```shell
 mitm_chrome mitmproxy
 ```
-
```

