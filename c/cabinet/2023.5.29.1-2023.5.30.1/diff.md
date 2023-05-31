# Comparing `tmp/cabinet-2023.5.29.1.tar.gz` & `tmp/cabinet-2023.5.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2023.5.29.1.tar", last modified: Mon May 29 07:37:37 2023, max compression
+gzip compressed data, was "cabinet-2023.5.30.1.tar", last modified: Wed May 31 04:54:42 2023, max compression
```

## Comparing `cabinet-2023.5.29.1.tar` & `cabinet-2023.5.30.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-29 07:37:37.181556 cabinet-2023.5.29.1/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.5.29.1/LICENSE
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6580 2023-05-29 07:37:37.181556 cabinet-2023.5.29.1/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6228 2023-05-29 07:33:24.000000 cabinet-2023.5.29.1/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.5.29.1/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-05-29 07:37:37.181556 cabinet-2023.5.29.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-29 07:37:37.181556 cabinet-2023.5.29.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-29 07:37:37.181556 cabinet-2023.5.29.1/src/cabinet/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    26102 2023-05-29 07:33:24.000000 cabinet-2023.5.29.1/src/cabinet/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-05-20 07:12:29.000000 cabinet-2023.5.29.1/src/cabinet/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3687 2023-04-16 16:59:23.000000 cabinet-2023.5.29.1/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-29 07:37:37.181556 cabinet-2023.5.29.1/src/cabinet.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6580 2023-05-29 07:37:37.000000 cabinet-2023.5.29.1/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      310 2023-05-29 07:37:37.000000 cabinet-2023.5.29.1/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-05-29 07:37:37.000000 cabinet-2023.5.29.1/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-05-29 07:37:37.000000 cabinet-2023.5.29.1/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-05-29 07:37:37.000000 cabinet-2023.5.29.1/src/cabinet.egg-info/top_level.txt
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-29 07:37:37.181556 cabinet-2023.5.29.1/test/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     5868 2023-05-29 07:26:03.000000 cabinet-2023.5.29.1/test/test___init__.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 04:54:42.683674 cabinet-2023.5.30.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.5.30.1/LICENSE
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6580 2023-05-31 04:54:42.683674 cabinet-2023.5.30.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6228 2023-05-31 04:52:07.000000 cabinet-2023.5.30.1/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.5.30.1/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-05-31 04:54:42.683674 cabinet-2023.5.30.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 04:54:42.679674 cabinet-2023.5.30.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 04:54:42.683674 cabinet-2023.5.30.1/src/cabinet/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2023-05-31 04:52:36.000000 cabinet-2023.5.30.1/src/cabinet/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-05-31 04:50:50.000000 cabinet-2023.5.30.1/src/cabinet/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    26102 2023-05-31 04:48:07.000000 cabinet-2023.5.30.1/src/cabinet/cabinet.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3687 2023-04-16 16:59:23.000000 cabinet-2023.5.30.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 04:54:42.683674 cabinet-2023.5.30.1/src/cabinet.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6580 2023-05-31 04:54:42.000000 cabinet-2023.5.30.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      333 2023-05-31 04:54:42.000000 cabinet-2023.5.30.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-05-31 04:54:42.000000 cabinet-2023.5.30.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-05-31 04:54:42.000000 cabinet-2023.5.30.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-05-31 04:54:42.000000 cabinet-2023.5.30.1/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-31 04:54:42.683674 cabinet-2023.5.30.1/test/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     5868 2023-05-31 04:52:07.000000 cabinet-2023.5.30.1/test/test___init__.py
```

### Comparing `cabinet-2023.5.29.1/LICENSE` & `cabinet-2023.5.30.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cabinet-2023.5.29.1/PKG-INFO` & `cabinet-2023.5.30.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.5.29.1
+Version: 2023.5.30.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cabinet-2023.5.29.1/README.md` & `cabinet-2023.5.30.1/README.md`

 * *Files identical despite different names*

### Comparing `cabinet-2023.5.29.1/setup.cfg` & `cabinet-2023.5.30.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cabinet
-version = 2023.05.29.1
+version = 2023.05.30.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls =
```

### Comparing `cabinet-2023.5.29.1/src/cabinet/__init__.py` & `cabinet-2023.5.30.1/src/cabinet/cabinet.py`

 * *Files identical despite different names*

### Comparing `cabinet-2023.5.29.1/src/cabinet/mail.py` & `cabinet-2023.5.30.1/src/cabinet/mail.py`

 * *Files identical despite different names*

### Comparing `cabinet-2023.5.29.1/src/cabinet.egg-info/PKG-INFO` & `cabinet-2023.5.30.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.5.29.1
+Version: 2023.5.30.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cabinet-2023.5.29.1/test/test___init__.py` & `cabinet-2023.5.30.1/test/test___init__.py`

 * *Files identical despite different names*

