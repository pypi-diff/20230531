# Comparing `tmp/fluctuate-2.0.0b1.tar.gz` & `tmp/fluctuate-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluctuate-2.0.0b1.tar", max compression
+gzip compressed data, was "fluctuate-2.0.0b2.tar", max compression
```

## Comparing `fluctuate-2.0.0b1.tar` & `fluctuate-2.0.0b2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-26 00:43:50.058457 fluctuate-2.0.0b1/LICENSE
--rw-r--r--   0        0        0    11094 2023-05-26 00:43:50.058457 fluctuate-2.0.0b1/README.md
--rw-r--r--   0        0        0        0 2023-05-26 00:43:50.085456 fluctuate-2.0.0b1/fluctuate/__init__.py
--rw-r--r--   0        0        0     4404 2023-05-26 00:43:50.058457 fluctuate-2.0.0b1/fluctuate/cli.py
--rw-r--r--   0        0        0    30650 2023-05-26 00:43:50.059456 fluctuate-2.0.0b1/fluctuate/migrations.py
--rw-r--r--   0        0        0     1857 2023-05-26 00:43:50.059456 fluctuate-2.0.0b1/fluctuate/secrets_manager.py
--rw-r--r--   0        0        0     1409 2023-05-26 00:44:29.723621 fluctuate-2.0.0b1/pyproject.toml
--rw-r--r--   0        0        0    12019 1970-01-01 00:00:00.000000 fluctuate-2.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-31 05:24:31.924873 fluctuate-2.0.0b2/LICENSE
+-rw-r--r--   0        0        0    11094 2023-05-31 05:24:31.924873 fluctuate-2.0.0b2/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 05:24:31.948873 fluctuate-2.0.0b2/fluctuate/__init__.py
+-rw-r--r--   0        0        0     4404 2023-05-31 05:24:31.924873 fluctuate-2.0.0b2/fluctuate/cli.py
+-rw-r--r--   0        0        0    30703 2023-05-31 05:24:31.924873 fluctuate-2.0.0b2/fluctuate/migrations.py
+-rw-r--r--   0        0        0     1857 2023-05-31 05:24:31.924873 fluctuate-2.0.0b2/fluctuate/secrets_manager.py
+-rw-r--r--   0        0        0     1409 2023-05-31 05:25:14.066723 fluctuate-2.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0    12019 1970-01-01 00:00:00.000000 fluctuate-2.0.0b2/PKG-INFO
```

### Comparing `fluctuate-2.0.0b1/LICENSE` & `fluctuate-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `fluctuate-2.0.0b1/README.md` & `fluctuate-2.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `fluctuate-2.0.0b1/fluctuate/cli.py` & `fluctuate-2.0.0b2/fluctuate/cli.py`

 * *Files identical despite different names*

### Comparing `fluctuate-2.0.0b1/fluctuate/migrations.py` & `fluctuate-2.0.0b2/fluctuate/migrations.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
                     }
                 },
                 constraints: [{unique: ["name", "namespace"]}]
             }
         )
     } else {
         if (
+            migrations_collection.indexes == null ||
             migrations_collection.indexes.by_name_and_namespace == null ||
             migrations_collection.indexes.by_name_and_namespace.terms != [
                 {"field": "name"}, {"field": "namespace"}
             ]
         ) {
             migrations_collection.update(
                 {
```

### Comparing `fluctuate-2.0.0b1/fluctuate/secrets_manager.py` & `fluctuate-2.0.0b2/fluctuate/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `fluctuate-2.0.0b1/pyproject.toml` & `fluctuate-2.0.0b2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fluctuate"
-version = "2.0.0-beta.1"
+version = "2.0.0-beta.2"
 description = "A simple migration utility for Fauna DB."
 authors = ["Ryan Causey <ryan.causey@munipal.io>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://gitlab.com/munipal-oss/fluctuate"
 homepage = "https://gitlab.com/munipal-oss/fluctuate"
```

### Comparing `fluctuate-2.0.0b1/PKG-INFO` & `fluctuate-2.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluctuate
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: A simple migration utility for Fauna DB.
 Home-page: https://gitlab.com/munipal-oss/fluctuate
 License: MIT
 Author: Ryan Causey
 Author-email: ryan.causey@munipal.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

