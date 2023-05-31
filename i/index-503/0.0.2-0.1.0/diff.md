# Comparing `tmp/index_503-0.0.2.tar.gz` & `tmp/index_503-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index_503-0.0.2.tar", max compression
+gzip compressed data, was "index_503-0.1.0.tar", max compression
```

## Comparing `index_503-0.0.2.tar` & `index_503-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1072 2023-05-31 16:05:21.959373 index_503-0.0.2/LICENSE
--rw-r--r--   0        0        0     3060 2023-05-31 16:11:36.388577 index_503-0.0.2/README.md
--rw-r--r--   0        0        0     2299 2023-05-31 20:24:27.414105 index_503-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-31 20:24:34.538491 index_503-0.0.2/src/index_503/__init__.py
--rw-r--r--   0        0        0     1336 2023-05-31 20:23:30.605747 index_503-0.0.2/src/index_503/file.py
--rw-r--r--   0        0        0     5029 2023-05-31 20:23:30.212849 index_503-0.0.2/src/index_503/index.py
--rw-r--r--   0        0        0      475 2023-05-31 20:23:39.284172 index_503-0.0.2/src/index_503/main.py
--rw-r--r--   0        0        0     2588 2023-05-31 20:23:29.549813 index_503-0.0.2/src/index_503/page_generator.py
--rw-r--r--   0        0        0        0 2023-05-31 16:05:21.960459 index_503-0.0.2/src/index_503/py.typed
--rw-r--r--   0        0        0      522 2023-05-31 20:23:39.284216 index_503-0.0.2/src/index_503/util.py
--rw-r--r--   0        0        0     3224 2023-05-31 20:23:28.705592 index_503-0.0.2/src/index_503/wheel_file.py
--rw-r--r--   0        0        0     4054 1970-01-01 00:00:00.000000 index_503-0.0.2/setup.py
--rw-r--r--   0        0        0     4425 1970-01-01 00:00:00.000000 index_503-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-31 20:36:35.113400 index_503-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3481 2023-05-31 20:36:35.113400 index_503-0.1.0/README.md
+-rw-r--r--   0        0        0     2299 2023-05-31 20:36:35.889403 index_503-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-31 20:36:35.849403 index_503-0.1.0/src/index_503/__init__.py
+-rw-r--r--   0        0        0     1336 2023-05-31 20:36:35.117400 index_503-0.1.0/src/index_503/file.py
+-rw-r--r--   0        0        0     5034 2023-05-31 20:36:35.117400 index_503-0.1.0/src/index_503/index.py
+-rw-r--r--   0        0        0      475 2023-05-31 20:36:35.117400 index_503-0.1.0/src/index_503/main.py
+-rw-r--r--   0        0        0     2588 2023-05-31 20:36:35.117400 index_503-0.1.0/src/index_503/page_generator.py
+-rw-r--r--   0        0        0        0 2023-05-31 20:36:35.117400 index_503-0.1.0/src/index_503/py.typed
+-rw-r--r--   0        0        0      522 2023-05-31 20:36:35.117400 index_503-0.1.0/src/index_503/util.py
+-rw-r--r--   0        0        0     3224 2023-05-31 20:36:35.117400 index_503-0.1.0/src/index_503/wheel_file.py
+-rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 index_503-0.1.0/PKG-INFO
```

### Comparing `index_503-0.0.2/LICENSE` & `index_503-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `index_503-0.0.2/pyproject.toml` & `index_503-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "index-503"
-version = "0.0.2"
+version = "0.1.0"
 description = "PEP 503 index builder"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bdraco/index-503"
 documentation = "https://index-503.readthedocs.io"
 classifiers = [
```

### Comparing `index_503-0.0.2/src/index_503/file.py` & `index_503-0.1.0/src/index_503/file.py`

 * *Files identical despite different names*

### Comparing `index_503-0.0.2/src/index_503/index.py` & `index_503-0.1.0/src/index_503/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     projects: Dict[str, List[WheelFile]] = defaultdict(list)
     cache_file = target_path.joinpath("cache.json")
     cache: Dict[str, Dict[str, Any]] = {}
     if cache_file.exists():
         cache = load_json_file(cache_file)
 
     with tempfile.TemporaryDirectory(
-        dir=target_path_parent, ignore_cleanup_errors=True
+        dir=str(target_path_parent), ignore_cleanup_errors=True
     ) as temp_dir:
         temp_dir_path = Path(temp_dir)
         all_wheel_files: set[str] = set()
 
         for wheel_file in glob.glob(str(origin_path.joinpath("*.whl"))):
             wheel_path = Path(wheel_file)
             wheel_file_name = wheel_path.name
```

### Comparing `index_503-0.0.2/src/index_503/page_generator.py` & `index_503-0.1.0/src/index_503/page_generator.py`

 * *Files identical despite different names*

### Comparing `index_503-0.0.2/src/index_503/util.py` & `index_503-0.1.0/src/index_503/util.py`

 * *Files identical despite different names*

### Comparing `index_503-0.0.2/src/index_503/wheel_file.py` & `index_503-0.1.0/src/index_503/wheel_file.py`

 * *Files identical despite different names*

### Comparing `index_503-0.0.2/PKG-INFO` & `index_503-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: index-503
-Version: 0.0.2
+Version: 0.1.0
 Summary: PEP 503 index builder
 Home-page: https://github.com/bdraco/index-503
 License: MIT
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -61,14 +61,26 @@
   </a>
   <img src="https://img.shields.io/pypi/pyversions/index-503.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
   <img src="https://img.shields.io/pypi/l/index-503.svg?style=flat-square" alt="License">
 </p>
 
 PEP 503 index builder
 
+## Usage
+
+If you have a directory full of wheels like `musllinux`:
+
+`index-503 musllinux`
+
+This will produce a `musllinux-index` directory with a PEP 503 index symlinked to the original directory without disturbing the original directory.
+
+Running this again will replace the original index and delete the old index in an atomic manner.
+
+The caller is responsible for ensuring that there are no simultaneous executions.
+
 ## Installation
 
 Install this via pip (or your favourite package manager):
 
 `pip install index-503`
 
 ## Credits
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: index-503 Version: 0.0.2 Summary: PEP 503 index
+Metadata-Version: 2.1 Name: index-503 Version: 0.1.0 Summary: PEP 503 index
 builder Home-page: https://github.com/bdraco/index-503 License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
@@ -16,13 +16,18 @@
 Changelog, https://github.com/bdraco/index-503/blob/main/CHANGELOG.md Project-
 URL: Documentation, https://index-503.readthedocs.io Project-URL: Repository,
 https://github.com/bdraco/index-503 Description-Content-Type: text/markdown #
 Index 503
          [CI_Status] [Documentation_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
-PEP 503 index builder ## Installation Install this via pip (or your favourite
-package manager): `pip install index-503` ## Credits This package was created
-with [Copier](https://copier.readthedocs.io/) and the [browniebroke/pypackage-
-template](https://github.com/browniebroke/pypackage-template) project template.
-This project borrows heavily from Dominic Davis-Foster's simple503 https://
-github.com/repo-helper/simple503
+PEP 503 index builder ## Usage If you have a directory full of wheels like
+`musllinux`: `index-503 musllinux` This will produce a `musllinux-index`
+directory with a PEP 503 index symlinked to the original directory without
+disturbing the original directory. Running this again will replace the original
+index and delete the old index in an atomic manner. The caller is responsible
+for ensuring that there are no simultaneous executions. ## Installation Install
+this via pip (or your favourite package manager): `pip install index-503` ##
+Credits This package was created with [Copier](https://copier.readthedocs.io/
+) and the [browniebroke/pypackage-template](https://github.com/browniebroke/
+pypackage-template) project template. This project borrows heavily from Dominic
+Davis-Foster's simple503 https://github.com/repo-helper/simple503
```

