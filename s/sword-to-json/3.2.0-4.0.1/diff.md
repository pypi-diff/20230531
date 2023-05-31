# Comparing `tmp/sword_to_json-3.2.0.tar.gz` & `tmp/sword_to_json-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sword_to_json-3.2.0.tar", max compression
+gzip compressed data, was "sword_to_json-4.0.1.tar", max compression
```

## Comparing `sword_to_json-3.2.0.tar` & `sword_to_json-4.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1817 2023-04-08 03:33:24.630350 sword_to_json-3.2.0/README.md
--rw-r--r--   0        0        0      768 2023-04-08 03:33:24.630350 sword_to_json-3.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-08 03:33:24.630350 sword_to_json-3.2.0/sword_to_json/__init__.py
--rw-r--r--   0        0        0      875 2023-04-08 03:33:24.634350 sword_to_json-3.2.0/sword_to_json/__main__.py
--rw-r--r--   0        0        0     1344 2023-04-08 03:33:24.634350 sword_to_json-3.2.0/sword_to_json/books_from_sword.py
--rw-r--r--   0        0        0        0 2023-04-08 03:33:24.634350 sword_to_json-3.2.0/sword_to_json/utils/__init__.py
--rw-r--r--   0        0        0      207 2023-04-08 03:33:24.634350 sword_to_json-3.2.0/sword_to_json/utils/metadata.py
--rw-r--r--   0        0        0      498 2023-04-08 03:33:24.634350 sword_to_json-3.2.0/sword_to_json/utils/progress.py
--rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 sword_to_json-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1794 2023-05-31 07:57:24.173336 sword_to_json-4.0.1/README.md
+-rw-r--r--   0        0        0      768 2023-05-31 07:57:24.173336 sword_to_json-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-31 07:57:24.173336 sword_to_json-4.0.1/sword_to_json/__init__.py
+-rw-r--r--   0        0        0      875 2023-05-31 07:57:24.173336 sword_to_json-4.0.1/sword_to_json/__main__.py
+-rw-r--r--   0        0        0     1344 2023-05-31 07:57:24.173336 sword_to_json-4.0.1/sword_to_json/books_from_sword.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:57:24.173336 sword_to_json-4.0.1/sword_to_json/utils/__init__.py
+-rw-r--r--   0        0        0      207 2023-05-31 07:57:24.173336 sword_to_json-4.0.1/sword_to_json/utils/metadata.py
+-rw-r--r--   0        0        0      498 2023-05-31 07:57:24.173336 sword_to_json-4.0.1/sword_to_json/utils/progress.py
+-rw-r--r--   0        0        0     2504 1970-01-01 00:00:00.000000 sword_to_json-4.0.1/PKG-INFO
```

### Comparing `sword_to_json-3.2.0/README.md` & `sword_to_json-4.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![Test](https://github.com/evnskc/sword-to-json/actions/workflows/test.yml/badge.svg)](https://github.com/evnskc/sword-to-json/actions/workflows/test.yml)
-[![Production](https://github.com/evnskc/sword-to-json/actions/workflows/deploy-production.yml/badge.svg)](https://github.com/evnskc/sword-to-json/actions/workflows/deploy-production.yml)
+[![Publish](https://github.com/evnskc/sword-to-json/actions/workflows/publish.yml/badge.svg)](https://github.com/evnskc/sword-to-json/actions/workflows/publish.yml)
 [![PyPI](https://img.shields.io/pypi/v/sword-to-json)](https://pypi.org/project/sword-to-json/)
 
 ## Generate JSON Files of Bible Translations from SWORD Modules
 
 The [SWORD project provides modules](http://crosswire.org/sword/modules/ModDisp.jsp?modType=Bibles) freely for common
 Bible translations in different languages.
```

### Comparing `sword_to_json-3.2.0/pyproject.toml` & `sword_to_json-4.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "sword-to-json"
-version = "3.2.0"
+version = "4.0.1"
 description = "Generate JSON Files of Bible Translations from SWORD Modules"
 license = "GPL-3.0-or-later"
 authors = ["Evans <evans@fundi.dev>"]
 readme = "README.md"
 homepage = "https://github.com/evnskc/sword-to-json"
 repository = "https://github.com/evnskc/sword-to-json"
 documentation = "https://github.com/evnskc/sword-to-json"
 keywords = ["sword", "bible text", "json"]
 packages = [{ include = "sword_to_json" }]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
 pysword = "^0.2.8"
 
 [tool.poetry.scripts]
 sword-to-json = "sword_to_json.__main__:main"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.2"
+pytest = "^7.3.1"
 jsonschema = "^4.17.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sword_to_json-3.2.0/sword_to_json/__main__.py` & `sword_to_json-4.0.1/sword_to_json/__main__.py`

 * *Files identical despite different names*

### Comparing `sword_to_json-3.2.0/sword_to_json/books_from_sword.py` & `sword_to_json-4.0.1/sword_to_json/books_from_sword.py`

 * *Files identical despite different names*

### Comparing `sword_to_json-3.2.0/PKG-INFO` & `sword_to_json-4.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: sword-to-json
-Version: 3.2.0
+Version: 4.0.1
 Summary: Generate JSON Files of Bible Translations from SWORD Modules
 Home-page: https://github.com/evnskc/sword-to-json
 License: GPL-3.0-or-later
 Keywords: sword,bible text,json
 Author: Evans
 Author-email: evans@fundi.dev
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pysword (>=0.2.8,<0.3.0)
 Project-URL: Documentation, https://github.com/evnskc/sword-to-json
 Project-URL: Repository, https://github.com/evnskc/sword-to-json
 Description-Content-Type: text/markdown
 
 [![Test](https://github.com/evnskc/sword-to-json/actions/workflows/test.yml/badge.svg)](https://github.com/evnskc/sword-to-json/actions/workflows/test.yml)
-[![Production](https://github.com/evnskc/sword-to-json/actions/workflows/deploy-production.yml/badge.svg)](https://github.com/evnskc/sword-to-json/actions/workflows/deploy-production.yml)
+[![Publish](https://github.com/evnskc/sword-to-json/actions/workflows/publish.yml/badge.svg)](https://github.com/evnskc/sword-to-json/actions/workflows/publish.yml)
 [![PyPI](https://img.shields.io/pypi/v/sword-to-json)](https://pypi.org/project/sword-to-json/)
 
 ## Generate JSON Files of Bible Translations from SWORD Modules
 
 The [SWORD project provides modules](http://crosswire.org/sword/modules/ModDisp.jsp?modType=Bibles) freely for common
 Bible translations in different languages.
```

