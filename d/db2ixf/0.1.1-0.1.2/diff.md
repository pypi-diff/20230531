# Comparing `tmp/db2ixf-0.1.1.tar.gz` & `tmp/db2ixf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db2ixf-0.1.1.tar", last modified: Wed May 31 00:52:55 2023, max compression
+gzip compressed data, was "db2ixf-0.1.2.tar", last modified: Wed May 31 07:21:11 2023, max compression
```

## Comparing `db2ixf-0.1.1.tar` & `db2ixf-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:52:55.524495 db2ixf-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-31 00:51:31.000000 db2ixf-0.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34512 2023-05-31 00:51:31.000000 db2ixf-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-05-31 00:52:55.524495 db2ixf-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-05-31 00:51:31.000000 db2ixf-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-31 00:51:31.000000 db2ixf-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 00:52:55.524495 db2ixf-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-31 00:51:31.000000 db2ixf-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:52:55.524495 db2ixf-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:52:55.524495 db2ixf-0.1.1/src/db2ixf/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-31 00:51:31.000000 db2ixf-0.1.1/src/db2ixf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 00:52:55.000000 db2ixf-0.1.1/src/db2ixf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-05-31 00:51:31.000000 db2ixf-0.1.1/src/db2ixf/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-05-31 00:51:31.000000 db2ixf-0.1.1/src/db2ixf/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-31 00:51:31.000000 db2ixf-0.1.1/src/db2ixf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-31 00:51:31.000000 db2ixf-0.1.1/src/db2ixf/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-31 00:51:31.000000 db2ixf-0.1.1/src/db2ixf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-31 00:51:31.000000 db2ixf-0.1.1/src/db2ixf/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-05-31 00:51:31.000000 db2ixf-0.1.1/src/db2ixf/ixf.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-31 00:51:31.000000 db2ixf-0.1.1/src/db2ixf/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:52:55.524495 db2ixf-0.1.1/src/db2ixf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-05-31 00:52:55.000000 db2ixf-0.1.1/src/db2ixf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-31 00:52:55.000000 db2ixf-0.1.1/src/db2ixf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:52:55.000000 db2ixf-0.1.1/src/db2ixf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 00:52:55.000000 db2ixf-0.1.1/src/db2ixf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:52:54.000000 db2ixf-0.1.1/src/db2ixf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-31 00:52:55.000000 db2ixf-0.1.1/src/db2ixf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 00:52:55.000000 db2ixf-0.1.1/src/db2ixf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:21:11.621123 db2ixf-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-31 07:19:59.000000 db2ixf-0.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34512 2023-05-31 07:19:59.000000 db2ixf-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-05-31 07:21:11.621123 db2ixf-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-05-31 07:19:59.000000 db2ixf-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-31 07:19:59.000000 db2ixf-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 07:21:11.621123 db2ixf-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-31 07:19:59.000000 db2ixf-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:21:11.621123 db2ixf-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:21:11.621123 db2ixf-0.1.2/src/db2ixf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-31 07:19:59.000000 db2ixf-0.1.2/src/db2ixf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 07:21:11.000000 db2ixf-0.1.2/src/db2ixf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-05-31 07:19:59.000000 db2ixf-0.1.2/src/db2ixf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-05-31 07:19:59.000000 db2ixf-0.1.2/src/db2ixf/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-31 07:19:59.000000 db2ixf-0.1.2/src/db2ixf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-31 07:19:59.000000 db2ixf-0.1.2/src/db2ixf/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-31 07:19:59.000000 db2ixf-0.1.2/src/db2ixf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-31 07:19:59.000000 db2ixf-0.1.2/src/db2ixf/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-05-31 07:19:59.000000 db2ixf-0.1.2/src/db2ixf/ixf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-31 07:19:59.000000 db2ixf-0.1.2/src/db2ixf/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:21:11.621123 db2ixf-0.1.2/src/db2ixf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-05-31 07:21:11.000000 db2ixf-0.1.2/src/db2ixf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-31 07:21:11.000000 db2ixf-0.1.2/src/db2ixf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 07:21:11.000000 db2ixf-0.1.2/src/db2ixf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 07:21:11.000000 db2ixf-0.1.2/src/db2ixf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 07:21:10.000000 db2ixf-0.1.2/src/db2ixf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-31 07:21:11.000000 db2ixf-0.1.2/src/db2ixf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 07:21:11.000000 db2ixf-0.1.2/src/db2ixf.egg-info/top_level.txt
```

### Comparing `db2ixf-0.1.1/CHANGELOG.md` & `db2ixf-0.1.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 This project uses [*towncrier*](https://towncrier.readthedocs.io/) and the
 changes for the upcoming release can be found
 in [here](https://github.com/ismailhammounou/db2ixf/tree/main/resources/changelog/)
 .
 
 <!-- release notes start -->
 
+## [0.1.2](https://github.com/ismailhammounou/db2ixf/tree/0.1.2) - 2023-05-31
+
+### Fixed
+
+- Fix issues in ci for gh-pages
+  generation [db2ixf-10](https://github.com/ismailhammounou/db2ixf/issues/10)
+
 ## [0.1.1](https://github.com/ismailhammounou/db2ixf/tree/0.1.1) - 2023-05-31
 
 ### Added
 
 - Add ci for github
   pages [db2ixf-9](https://github.com/ismailhammounou/db2ixf/issues/9)
```

### Comparing `db2ixf-0.1.1/LICENSE` & `db2ixf-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.1/PKG-INFO` & `db2ixf-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: db2ixf
-Version: 0.1.1
+Version: 0.1.2
 Summary: Parsing and processing of IBM eXchange format (IXF)
 Author-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 Maintainer-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 License: AGPL-3.0
 Project-URL: homepage, https://github.com/ismailhammounou/db2ixf
 Project-URL: documentation, https://github.com/ismailhammounou/db2ixf/blob/main/README.md
 Project-URL: repository, https://github.com/ismailhammounou/db2ixf.git
 Project-URL: changelog, https://github.com/ismailhammounou/db2ixf/blob/main/CHANGELOG.md
-Keywords: PC,IXF,IBM,DB2,Development,Tools,Package,Parsing,Format
+Keywords: PC,IXF,IBM,DB2,Development,Tools,Package,Parsing,Format,Data,Analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -187,16 +187,16 @@
 - [ ] Add tests (Manual testing was done but need write unit tests).
 - [ ] Adding new collectors for other ixf data types: floating point ... etc.
 - [ ] Improve documentation.
 - [x] Add a CLI.
 - [x] Improve CLI: output can be optional.
 - [ ] Add better ci-cd.
 - [ ] Improve Makefile.
-- [ ] Support multiprocessing.
-- [ ] Support archived inputs: only python not CLI ?
+- [ ] ~~Support multiprocessing.~~
+- [ ] ~~Support archived inputs: only python not CLI ?~~
 - [x] Add logging.
 
 ## License
 
 IXF Parser is released under the
 [AGPL-3.0 License](https://github.com/ismailhammounou/db2ixf/blob/main/LICENSE).
```

### Comparing `db2ixf-0.1.1/README.md` & `db2ixf-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -163,16 +163,16 @@
 - [ ] Add tests (Manual testing was done but need write unit tests).
 - [ ] Adding new collectors for other ixf data types: floating point ... etc.
 - [ ] Improve documentation.
 - [x] Add a CLI.
 - [x] Improve CLI: output can be optional.
 - [ ] Add better ci-cd.
 - [ ] Improve Makefile.
-- [ ] Support multiprocessing.
-- [ ] Support archived inputs: only python not CLI ?
+- [ ] ~~Support multiprocessing.~~
+- [ ] ~~Support archived inputs: only python not CLI ?~~
 - [x] Add logging.
 
 ## License
 
 IXF Parser is released under the
 [AGPL-3.0 License](https://github.com/ismailhammounou/db2ixf/blob/main/LICENSE).
```

### Comparing `db2ixf-0.1.1/pyproject.toml` & `db2ixf-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ]
 maintainers = [
     { name = 'Ismail Hammounou', email = 'ismail.hammounou@gmail.com' },
 ]
 description = 'Parsing and processing of IBM eXchange format (IXF)'
 keywords = [
     'PC', 'IXF', 'IBM', 'DB2', 'Development', 'Tools', 'Package', 'Parsing',
-    'Format'
+    'Format', "Data", "Analysis"
 ]
 license = { text = "AGPL-3.0" }
 requires-python = '>=3.7'
 dynamic = ['version', 'readme']
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

### Comparing `db2ixf-0.1.1/src/db2ixf/__init__.py` & `db2ixf-0.1.2/src/db2ixf/__init__.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.1/src/db2ixf/cli.py` & `db2ixf-0.1.2/src/db2ixf/cli.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.1/src/db2ixf/collectors.py` & `db2ixf-0.1.2/src/db2ixf/collectors.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.1/src/db2ixf/constants.py` & `db2ixf-0.1.2/src/db2ixf/constants.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.1/src/db2ixf/exceptions.py` & `db2ixf-0.1.2/src/db2ixf/exceptions.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.1/src/db2ixf/helpers.py` & `db2ixf-0.1.2/src/db2ixf/helpers.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.1/src/db2ixf/ixf.py` & `db2ixf-0.1.2/src/db2ixf/ixf.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.1/src/db2ixf/logger.py` & `db2ixf-0.1.2/src/db2ixf/logger.py`

 * *Files identical despite different names*

### Comparing `db2ixf-0.1.1/src/db2ixf.egg-info/PKG-INFO` & `db2ixf-0.1.2/src/db2ixf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: db2ixf
-Version: 0.1.1
+Version: 0.1.2
 Summary: Parsing and processing of IBM eXchange format (IXF)
 Author-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 Maintainer-email: Ismail Hammounou <ismail.hammounou@gmail.com>
 License: AGPL-3.0
 Project-URL: homepage, https://github.com/ismailhammounou/db2ixf
 Project-URL: documentation, https://github.com/ismailhammounou/db2ixf/blob/main/README.md
 Project-URL: repository, https://github.com/ismailhammounou/db2ixf.git
 Project-URL: changelog, https://github.com/ismailhammounou/db2ixf/blob/main/CHANGELOG.md
-Keywords: PC,IXF,IBM,DB2,Development,Tools,Package,Parsing,Format
+Keywords: PC,IXF,IBM,DB2,Development,Tools,Package,Parsing,Format,Data,Analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -187,16 +187,16 @@
 - [ ] Add tests (Manual testing was done but need write unit tests).
 - [ ] Adding new collectors for other ixf data types: floating point ... etc.
 - [ ] Improve documentation.
 - [x] Add a CLI.
 - [x] Improve CLI: output can be optional.
 - [ ] Add better ci-cd.
 - [ ] Improve Makefile.
-- [ ] Support multiprocessing.
-- [ ] Support archived inputs: only python not CLI ?
+- [ ] ~~Support multiprocessing.~~
+- [ ] ~~Support archived inputs: only python not CLI ?~~
 - [x] Add logging.
 
 ## License
 
 IXF Parser is released under the
 [AGPL-3.0 License](https://github.com/ismailhammounou/db2ixf/blob/main/LICENSE).
```

### Comparing `db2ixf-0.1.1/src/db2ixf.egg-info/SOURCES.txt` & `db2ixf-0.1.2/src/db2ixf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

