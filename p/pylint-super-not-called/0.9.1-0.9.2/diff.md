# Comparing `tmp/pylint_super_not_called-0.9.1.tar.gz` & `tmp/pylint_super_not_called-0.9.2.tar.gz`

## Comparing `pylint_super_not_called-0.9.1.tar` & `pylint_super_not_called-0.9.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.1/Makefile
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.1/requirements.txt
--rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.1/src/super_not_called.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.1/src/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.1/src/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.1/src/.ruff_cache/content/af4def8bd90437a2
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.1/LICENSE
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.1/README.md
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.2/Makefile
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.2/requirements.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.2/src/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.2/src/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.2/src/.ruff_cache/content/af4def8bd90437a2
+-rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.2/src/pylint_super_not_called/__init__.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.2/LICENSE
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.2/README.md
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pylint_super_not_called-0.9.2/PKG-INFO
```

### Comparing `pylint_super_not_called-0.9.1/src/super_not_called.py` & `pylint_super_not_called-0.9.2/src/pylint_super_not_called/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint_super_not_called-0.9.1/src/.ruff_cache/content/af4def8bd90437a2` & `pylint_super_not_called-0.9.2/src/.ruff_cache/content/af4def8bd90437a2`

 * *Files identical despite different names*

### Comparing `pylint_super_not_called-0.9.1/LICENSE` & `pylint_super_not_called-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylint_super_not_called-0.9.1/pyproject.toml` & `pylint_super_not_called-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pylint_super_not_called"
-version = "0.9.1"
+version = "0.9.2"
 authors = [
   { name="Nicolas Mussat", email="nicolas@prose.com" },
 ]
 description = "A Pylint plugin to ensure overloaded methods are calling the parent method with super"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pylint_super_not_called-0.9.1/PKG-INFO` & `pylint_super_not_called-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylint_super_not_called
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Pylint plugin to ensure overloaded methods are calling the parent method with super
 Project-URL: Homepage, https://github.com/prosehair/pylint_super_not_called_plugin
 Project-URL: Bug Tracker, https://github.com/prosehair/pylint_super_not_called_plugin/issues
 Author-email: Nicolas Mussat <nicolas@prose.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

