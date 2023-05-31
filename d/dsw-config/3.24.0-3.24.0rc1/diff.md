# Comparing `tmp/dsw-config-3.24.0.tar.gz` & `tmp/dsw-config-3.24.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-config-3.24.0.tar", last modified: Wed May 31 09:40:30 2023, max compression
+gzip compressed data, was "dsw-config-3.24.0rc1.tar", last modified: Tue May 30 11:45:41 2023, max compression
```

## Comparing `dsw-config-3.24.0.tar` & `dsw-config-3.24.0rc1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:40:30.702585 dsw-config-3.24.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-31 09:40:25.000000 dsw-config-3.24.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-31 09:40:30.702585 dsw-config-3.24.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-31 09:40:25.000000 dsw-config-3.24.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:40:30.702585 dsw-config-3.24.0/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:40:30.702585 dsw-config-3.24.0/dsw/config/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-31 09:40:25.000000 dsw-config-3.24.0/dsw/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-31 09:40:30.000000 dsw-config-3.24.0/dsw/config/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-05-31 09:40:25.000000 dsw-config-3.24.0/dsw/config/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-31 09:40:25.000000 dsw-config-3.24.0/dsw/config/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-05-31 09:40:25.000000 dsw-config-3.24.0/dsw/config/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-31 09:40:25.000000 dsw-config-3.24.0/dsw/config/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-31 09:40:25.000000 dsw-config-3.24.0/dsw/config/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:40:30.702585 dsw-config-3.24.0/dsw_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-31 09:40:30.000000 dsw-config-3.24.0/dsw_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-31 09:40:30.000000 dsw-config-3.24.0/dsw_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:40:30.000000 dsw-config-3.24.0/dsw_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:40:30.000000 dsw-config-3.24.0/dsw_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 09:40:30.000000 dsw-config-3.24.0/dsw_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-31 09:40:30.000000 dsw-config-3.24.0/dsw_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 09:40:25.000000 dsw-config-3.24.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:40:30.702585 dsw-config-3.24.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:40:25.000000 dsw-config-3.24.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:41.017926 dsw-config-3.24.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-30 11:45:41.017926 dsw-config-3.24.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:41.017926 dsw-config-3.24.0rc1/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:41.017926 dsw-config-3.24.0rc1/dsw/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/dsw/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-30 11:45:40.000000 dsw-config-3.24.0rc1/dsw/config/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/dsw/config/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/dsw/config/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/dsw/config/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/dsw/config/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/dsw/config/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:45:41.017926 dsw-config-3.24.0rc1/dsw_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-30 11:45:41.000000 dsw-config-3.24.0rc1/dsw_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-30 11:45:41.000000 dsw-config-3.24.0rc1/dsw_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:45:41.000000 dsw-config-3.24.0rc1/dsw_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:45:41.000000 dsw-config-3.24.0rc1/dsw_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 11:45:41.000000 dsw-config-3.24.0rc1/dsw_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-30 11:45:41.000000 dsw-config-3.24.0rc1/dsw_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:45:41.017926 dsw-config-3.24.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:45:36.000000 dsw-config-3.24.0rc1/setup.py
```

### Comparing `dsw-config-3.24.0/LICENSE` & `dsw-config-3.24.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-config-3.24.0/PKG-INFO` & `dsw-config-3.24.0rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-config
-Version: 3.24.0
+Version: 3.24.0rc1
 Summary: Library for DSW config manipulation
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,config,yaml,parser
```

### Comparing `dsw-config-3.24.0/README.md` & `dsw-config-3.24.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dsw-config-3.24.0/dsw/config/keys.py` & `dsw-config-3.24.0rc1/dsw/config/keys.py`

 * *Files identical despite different names*

### Comparing `dsw-config-3.24.0/dsw/config/logging.py` & `dsw-config-3.24.0rc1/dsw/config/logging.py`

 * *Files identical despite different names*

### Comparing `dsw-config-3.24.0/dsw/config/model.py` & `dsw-config-3.24.0rc1/dsw/config/model.py`

 * *Files identical despite different names*

### Comparing `dsw-config-3.24.0/dsw/config/parser.py` & `dsw-config-3.24.0rc1/dsw/config/parser.py`

 * *Files identical despite different names*

### Comparing `dsw-config-3.24.0/dsw/config/sentry.py` & `dsw-config-3.24.0rc1/dsw/config/sentry.py`

 * *Files identical despite different names*

### Comparing `dsw-config-3.24.0/dsw_config.egg-info/PKG-INFO` & `dsw-config-3.24.0rc1/dsw_config.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-config
-Version: 3.24.0
+Version: 3.24.0rc1
 Summary: Library for DSW config manipulation
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,config,yaml,parser
```

### Comparing `dsw-config-3.24.0/pyproject.toml` & `dsw-config-3.24.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-config'
-version = "3.24.0"
+version = "3.24.0rc.1"
 description = 'Library for DSW config manipulation'
 readme = 'README.md'
 keywords = ['dsw', 'config', 'yaml', 'parser']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
```

