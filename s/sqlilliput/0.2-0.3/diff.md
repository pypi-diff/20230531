# Comparing `tmp/sqlilliput-0.2.tar.gz` & `tmp/sqlilliput-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlilliput-0.2.tar", last modified: Wed May 31 09:25:52 2023, max compression
+gzip compressed data, was "sqlilliput-0.3.tar", last modified: Wed May 31 09:28:29 2023, max compression
```

## Comparing `sqlilliput-0.2.tar` & `sqlilliput-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-31 09:25:52.804575 sqlilliput-0.2/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    11357 2023-05-31 08:43:59.000000 sqlilliput-0.2/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      283 2023-05-31 09:25:52.804575 sqlilliput-0.2/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1361 2023-05-31 09:20:01.000000 sqlilliput-0.2/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-05-31 09:25:52.804575 sqlilliput-0.2/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1394 2023-05-31 09:25:45.000000 sqlilliput-0.2/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-31 09:25:52.804575 sqlilliput-0.2/sqlilliput/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       48 2023-05-31 09:23:57.000000 sqlilliput-0.2/sqlilliput/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    11449 2023-05-31 09:25:17.000000 sqlilliput-0.2/sqlilliput/sqlite.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-31 09:25:52.804575 sqlilliput-0.2/sqlilliput.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      283 2023-05-31 09:25:52.000000 sqlilliput-0.2/sqlilliput.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      239 2023-05-31 09:25:52.000000 sqlilliput-0.2/sqlilliput.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-05-31 09:25:52.000000 sqlilliput-0.2/sqlilliput.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       14 2023-05-31 09:25:52.000000 sqlilliput-0.2/sqlilliput.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-05-31 09:25:52.000000 sqlilliput-0.2/sqlilliput.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-31 09:28:29.226834 sqlilliput-0.3/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    11357 2023-05-31 08:43:59.000000 sqlilliput-0.3/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      283 2023-05-31 09:28:29.226834 sqlilliput-0.3/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1361 2023-05-31 09:20:01.000000 sqlilliput-0.3/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-05-31 09:28:29.226834 sqlilliput-0.3/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1372 2023-05-31 09:28:23.000000 sqlilliput-0.3/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-31 09:28:29.226834 sqlilliput-0.3/sqlilliput/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       48 2023-05-31 09:23:57.000000 sqlilliput-0.3/sqlilliput/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    11449 2023-05-31 09:25:17.000000 sqlilliput-0.3/sqlilliput/sqlite.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-31 09:28:29.226834 sqlilliput-0.3/sqlilliput.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      283 2023-05-31 09:28:29.000000 sqlilliput-0.3/sqlilliput.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      239 2023-05-31 09:28:29.000000 sqlilliput-0.3/sqlilliput.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-05-31 09:28:29.000000 sqlilliput-0.3/sqlilliput.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        7 2023-05-31 09:28:29.000000 sqlilliput-0.3/sqlilliput.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       11 2023-05-31 09:28:29.000000 sqlilliput-0.3/sqlilliput.egg-info/top_level.txt
```

### Comparing `sqlilliput-0.2/LICENSE` & `sqlilliput-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlilliput-0.2/README.md` & `sqlilliput-0.3/README.md`

 * *Files identical despite different names*

### Comparing `sqlilliput-0.2/setup.py` & `sqlilliput-0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,24 @@
 
 import setuptools
 
 
 def main():
     setuptools.setup(
         name="sqlilliput",
-        version="0.2",
+        version="0.3",
         description="Python abstraction layer for SQLite3",
         long_description="",
         long_description_content_type="text/plain",
         url="https://github.com/DinoSourceDK/sqlilliput",
         author="DinoSource ApS",
         author_email="info@dinosource.co",
         license="Apache",
         packages=["sqlilliput"],
         install_requires=[
-            "sqlite",
             "typing",
         ],
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `sqlilliput-0.2/sqlilliput/sqlite.py` & `sqlilliput-0.3/sqlilliput/sqlite.py`

 * *Files identical despite different names*

