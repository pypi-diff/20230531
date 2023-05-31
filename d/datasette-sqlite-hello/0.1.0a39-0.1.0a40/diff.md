# Comparing `tmp/datasette_sqlite_hello-0.1.0a39-py3-none-any.whl.zip` & `tmp/datasette_sqlite_hello-0.1.0a40-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 2205 bytes, number of entries: 7
--rw-r--r--  2.0 unx      269 b- defN 23-May-29 06:32 datasette_sqlite_hello/__init__.py
--rw-r--r--  2.0 unx       80 b- defN 23-May-29 06:32 datasette_sqlite_hello/version.py
--rw-r--r--  2.0 unx      570 b- defN 23-May-29 06:32 datasette_sqlite_hello-0.1.0a39.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-29 06:32 datasette_sqlite_hello-0.1.0a39.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-May-29 06:32 datasette_sqlite_hello-0.1.0a39.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-May-29 06:32 datasette_sqlite_hello-0.1.0a39.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      660 b- defN 23-May-29 06:32 datasette_sqlite_hello-0.1.0a39.dist-info/RECORD
+-rw-r--r--  2.0 unx      269 b- defN 23-May-31 21:22 datasette_sqlite_hello/__init__.py
+-rw-r--r--  2.0 unx       80 b- defN 23-May-31 21:22 datasette_sqlite_hello/version.py
+-rw-r--r--  2.0 unx      570 b- defN 23-May-31 21:22 datasette_sqlite_hello-0.1.0a40.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 21:22 datasette_sqlite_hello-0.1.0a40.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-May-31 21:22 datasette_sqlite_hello-0.1.0a40.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-May-31 21:22 datasette_sqlite_hello-0.1.0a40.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      660 b- defN 23-May-31 21:22 datasette_sqlite_hello-0.1.0a40.dist-info/RECORD
 7 files, 1744 bytes uncompressed, 1001 bytes compressed:  42.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_hello/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_hello/version.py
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a39.dist-info/METADATA
+Filename: datasette_sqlite_hello-0.1.0a40.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a39.dist-info/WHEEL
+Filename: datasette_sqlite_hello-0.1.0a40.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a39.dist-info/entry_points.txt
+Filename: datasette_sqlite_hello-0.1.0a40.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a39.dist-info/top_level.txt
+Filename: datasette_sqlite_hello-0.1.0a40.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a39.dist-info/RECORD
+Filename: datasette_sqlite_hello-0.1.0a40.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_hello/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.39"
+__version__ = "0.1.0-alpha.40"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_hello-0.1.0a39.dist-info/METADATA` & `datasette_sqlite_hello-0.1.0a40.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-hello
-Version: 0.1.0a39
+Version: 0.1.0a40
 Home-page: https://github.com/asg017/sqlite-hello
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-hello/issues
 Project-URL: CI, https://github.com/asg017/sqlite-hello/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-hello/releases
 Requires-Python: >=3.6
```

## Comparing `datasette_sqlite_hello-0.1.0a39.dist-info/RECORD` & `datasette_sqlite_hello-0.1.0a40.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 datasette_sqlite_hello/__init__.py,sha256=GiwcIRu3EMST18OdDMuooqh_Ncg2ePiuYkVT46SHliE,269
-datasette_sqlite_hello/version.py,sha256=fq4RaHoS-XTkYimvEcLbbhiVMOX26xtim15eh-xAJCs,80
-datasette_sqlite_hello-0.1.0a39.dist-info/METADATA,sha256=dB6mlhxqYHGA0u_Uvw_D2KI0qRY-As6TvclzR9SrJAM,570
-datasette_sqlite_hello-0.1.0a39.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-datasette_sqlite_hello-0.1.0a39.dist-info/entry_points.txt,sha256=X0FnrOoDf3sGgQlWdM3s86QQSGuAZRKfOVfLJcXocpI,50
-datasette_sqlite_hello-0.1.0a39.dist-info/top_level.txt,sha256=klX1wE-1onKhiIgleurv_OT4mMGfe2GmHvNwpSMuYic,23
-datasette_sqlite_hello-0.1.0a39.dist-info/RECORD,,
+datasette_sqlite_hello/version.py,sha256=n-C-KzIuBBq1QiNrP9fenSYeowhbrCUSBWmNXeY2Too,80
+datasette_sqlite_hello-0.1.0a40.dist-info/METADATA,sha256=DZShH58fPe_6JRi3LW4BJwk4gFCx5PgbC4BjSqJQOmI,570
+datasette_sqlite_hello-0.1.0a40.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+datasette_sqlite_hello-0.1.0a40.dist-info/entry_points.txt,sha256=X0FnrOoDf3sGgQlWdM3s86QQSGuAZRKfOVfLJcXocpI,50
+datasette_sqlite_hello-0.1.0a40.dist-info/top_level.txt,sha256=klX1wE-1onKhiIgleurv_OT4mMGfe2GmHvNwpSMuYic,23
+datasette_sqlite_hello-0.1.0a40.dist-info/RECORD,,
```

