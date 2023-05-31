# Comparing `tmp/nice-sql-2.0.0.tar.gz` & `tmp/nice-sql-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nice-sql-2.0.0.tar", last modified: Wed May 31 07:24:28 2023, max compression
+gzip compressed data, was "nice-sql-2.0.1.tar", last modified: Wed May 31 07:38:24 2023, max compression
```

## Comparing `nice-sql-2.0.0.tar` & `nice-sql-2.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:24:27.997576 nice-sql-2.0.0/
--rw-r--r--   0 lichengming   (502) staff       (20)     2617 2023-05-31 07:24:27.997030 nice-sql-2.0.0/PKG-INFO
--rw-r--r--   0 lichengming   (502) staff       (20)     2316 2023-05-31 07:12:58.000000 nice-sql-2.0.0/README.md
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:24:27.988395 nice-sql-2.0.0/nice_sql.egg-info/
--rw-r--r--   0 lichengming   (502) staff       (20)     2617 2023-05-31 07:24:27.000000 nice-sql-2.0.0/nice_sql.egg-info/PKG-INFO
--rw-r--r--   0 lichengming   (502) staff       (20)      496 2023-05-31 07:24:27.000000 nice-sql-2.0.0/nice_sql.egg-info/SOURCES.txt
--rw-r--r--   0 lichengming   (502) staff       (20)        1 2023-05-31 07:24:27.000000 nice-sql-2.0.0/nice_sql.egg-info/dependency_links.txt
--rw-r--r--   0 lichengming   (502) staff       (20)       44 2023-05-31 07:24:27.000000 nice-sql-2.0.0/nice_sql.egg-info/requires.txt
--rw-r--r--   0 lichengming   (502) staff       (20)        8 2023-05-31 07:24:27.000000 nice-sql-2.0.0/nice_sql.egg-info/top_level.txt
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:24:27.988755 nice-sql-2.0.0/nicesql/
--rw-r--r--   0 lichengming   (502) staff       (20)        0 2023-05-30 06:32:39.000000 nice-sql-2.0.0/nicesql/__init__.py
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:24:27.990740 nice-sql-2.0.0/nicesql/engine/
--rw-r--r--   0 lichengming   (502) staff       (20)      213 2023-05-30 12:32:57.000000 nice-sql-2.0.0/nicesql/engine/__init__.py
--rw-r--r--   0 lichengming   (502) staff       (20)     2226 2023-05-31 02:40:04.000000 nice-sql-2.0.0/nicesql/engine/_engines.py
--rw-r--r--   0 lichengming   (502) staff       (20)      400 2023-05-31 02:47:34.000000 nice-sql-2.0.0/nicesql/engine/_execute.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1629 2023-05-30 12:29:17.000000 nice-sql-2.0.0/nicesql/engine/_register.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1128 2023-05-30 07:03:46.000000 nice-sql-2.0.0/nicesql/engine/_result.py
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:24:27.992902 nice-sql-2.0.0/nicesql/shortcut/
--rw-r--r--   0 lichengming   (502) staff       (20)       80 2023-05-30 08:54:09.000000 nice-sql-2.0.0/nicesql/shortcut/__init__.py
--rw-r--r--   0 lichengming   (502) staff       (20)     3147 2023-05-30 08:59:16.000000 nice-sql-2.0.0/nicesql/shortcut/_shortcut.py
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:24:27.994829 nice-sql-2.0.0/nicesql/sqlconv/
--rw-r--r--   0 lichengming   (502) staff       (20)       50 2023-05-29 08:40:55.000000 nice-sql-2.0.0/nicesql/sqlconv/__init__.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1355 2023-05-29 11:43:20.000000 nice-sql-2.0.0/nicesql/sqlconv/_convert.py
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:24:27.996056 nice-sql-2.0.0/nicesql/utils/
--rw-r--r--   0 lichengming   (502) staff       (20)       54 2023-05-31 02:46:13.000000 nice-sql-2.0.0/nicesql/utils/__init__.py
--rw-r--r--   0 lichengming   (502) staff       (20)      326 2023-05-23 10:10:49.000000 nice-sql-2.0.0/nicesql/utils/error.py
--rw-r--r--   0 lichengming   (502) staff       (20)       38 2023-05-31 07:24:27.997793 nice-sql-2.0.0/setup.cfg
--rw-r--r--   0 lichengming   (502) staff       (20)      749 2023-05-31 07:10:19.000000 nice-sql-2.0.0/setup.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:38:24.280526 nice-sql-2.0.1/
+-rw-r--r--   0 lichengming   (502) staff       (20)     2619 2023-05-31 07:38:24.280076 nice-sql-2.0.1/PKG-INFO
+-rw-r--r--   0 lichengming   (502) staff       (20)     2318 2023-05-31 07:31:09.000000 nice-sql-2.0.1/README.md
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:38:24.273349 nice-sql-2.0.1/nice_sql.egg-info/
+-rw-r--r--   0 lichengming   (502) staff       (20)     2619 2023-05-31 07:38:24.000000 nice-sql-2.0.1/nice_sql.egg-info/PKG-INFO
+-rw-r--r--   0 lichengming   (502) staff       (20)      496 2023-05-31 07:38:24.000000 nice-sql-2.0.1/nice_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 lichengming   (502) staff       (20)        1 2023-05-31 07:38:24.000000 nice-sql-2.0.1/nice_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 lichengming   (502) staff       (20)       44 2023-05-31 07:38:24.000000 nice-sql-2.0.1/nice_sql.egg-info/requires.txt
+-rw-r--r--   0 lichengming   (502) staff       (20)        8 2023-05-31 07:38:24.000000 nice-sql-2.0.1/nice_sql.egg-info/top_level.txt
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:38:24.273721 nice-sql-2.0.1/nicesql/
+-rw-r--r--   0 lichengming   (502) staff       (20)        0 2023-05-30 06:32:39.000000 nice-sql-2.0.1/nicesql/__init__.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:38:24.276084 nice-sql-2.0.1/nicesql/engine/
+-rw-r--r--   0 lichengming   (502) staff       (20)      213 2023-05-30 12:32:57.000000 nice-sql-2.0.1/nicesql/engine/__init__.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     2226 2023-05-31 02:40:04.000000 nice-sql-2.0.1/nicesql/engine/_engines.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      400 2023-05-31 02:47:34.000000 nice-sql-2.0.1/nicesql/engine/_execute.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1629 2023-05-30 12:29:17.000000 nice-sql-2.0.1/nicesql/engine/_register.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1128 2023-05-30 07:03:46.000000 nice-sql-2.0.1/nicesql/engine/_result.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:38:24.277086 nice-sql-2.0.1/nicesql/shortcut/
+-rw-r--r--   0 lichengming   (502) staff       (20)       80 2023-05-30 08:54:09.000000 nice-sql-2.0.1/nicesql/shortcut/__init__.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     3147 2023-05-30 08:59:16.000000 nice-sql-2.0.1/nicesql/shortcut/_shortcut.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:38:24.278066 nice-sql-2.0.1/nicesql/sqlconv/
+-rw-r--r--   0 lichengming   (502) staff       (20)       50 2023-05-29 08:40:55.000000 nice-sql-2.0.1/nicesql/sqlconv/__init__.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1355 2023-05-29 11:43:20.000000 nice-sql-2.0.1/nicesql/sqlconv/_convert.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:38:24.279230 nice-sql-2.0.1/nicesql/utils/
+-rw-r--r--   0 lichengming   (502) staff       (20)       54 2023-05-31 02:46:13.000000 nice-sql-2.0.1/nicesql/utils/__init__.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      326 2023-05-23 10:10:49.000000 nice-sql-2.0.1/nicesql/utils/error.py
+-rw-r--r--   0 lichengming   (502) staff       (20)       38 2023-05-31 07:38:24.280690 nice-sql-2.0.1/setup.cfg
+-rw-r--r--   0 lichengming   (502) staff       (20)      749 2023-05-31 07:33:11.000000 nice-sql-2.0.1/setup.py
```

### Comparing `nice-sql-2.0.0/PKG-INFO` & `nice-sql-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nice-sql
-Version: 2.0.0
+Version: 2.0.1
 Summary: easy nice sql: decorator with sql
 Home-page: https://github.com/minusli/nicesql
 Author: minusli
 Author-email: minusli@foxmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3
@@ -33,15 +33,15 @@
 
 ```python
 from nicesql.shortcut import select, update, insert, delete, ddl
 
 
 # 方式 1：直接查询
 def way1():
-    result = select("select * from t where a={a} and b in (?)", {"a": 1, "b": ["1", "2"]}).execute()
+    result = select("select * from t where a={a} and b in ({b})", {"a": 1, "b": ["1", "2"]}).execute()
 
 
 # 方式 2：装饰器查询
 @select("select * from t where a={a}")
 def get(a=1):
     pass
```

### Comparing `nice-sql-2.0.0/README.md` & `nice-sql-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 ```python
 from nicesql.shortcut import select, update, insert, delete, ddl
 
 
 # 方式 1：直接查询
 def way1():
-    result = select("select * from t where a={a} and b in (?)", {"a": 1, "b": ["1", "2"]}).execute()
+    result = select("select * from t where a={a} and b in ({b})", {"a": 1, "b": ["1", "2"]}).execute()
 
 
 # 方式 2：装饰器查询
 @select("select * from t where a={a}")
 def get(a=1):
     pass
```

### Comparing `nice-sql-2.0.0/nice_sql.egg-info/PKG-INFO` & `nice-sql-2.0.1/nice_sql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nice-sql
-Version: 2.0.0
+Version: 2.0.1
 Summary: easy nice sql: decorator with sql
 Home-page: https://github.com/minusli/nicesql
 Author: minusli
 Author-email: minusli@foxmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3
@@ -33,15 +33,15 @@
 
 ```python
 from nicesql.shortcut import select, update, insert, delete, ddl
 
 
 # 方式 1：直接查询
 def way1():
-    result = select("select * from t where a={a} and b in (?)", {"a": 1, "b": ["1", "2"]}).execute()
+    result = select("select * from t where a={a} and b in ({b})", {"a": 1, "b": ["1", "2"]}).execute()
 
 
 # 方式 2：装饰器查询
 @select("select * from t where a={a}")
 def get(a=1):
     pass
```

### Comparing `nice-sql-2.0.0/nicesql/engine/_engines.py` & `nice-sql-2.0.1/nicesql/engine/_engines.py`

 * *Files identical despite different names*

### Comparing `nice-sql-2.0.0/nicesql/engine/_register.py` & `nice-sql-2.0.1/nicesql/engine/_register.py`

 * *Files identical despite different names*

### Comparing `nice-sql-2.0.0/nicesql/engine/_result.py` & `nice-sql-2.0.1/nicesql/engine/_result.py`

 * *Files identical despite different names*

### Comparing `nice-sql-2.0.0/nicesql/shortcut/_shortcut.py` & `nice-sql-2.0.1/nicesql/shortcut/_shortcut.py`

 * *Files identical despite different names*

### Comparing `nice-sql-2.0.0/nicesql/sqlconv/_convert.py` & `nice-sql-2.0.1/nicesql/sqlconv/_convert.py`

 * *Files identical despite different names*

### Comparing `nice-sql-2.0.0/setup.py` & `nice-sql-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # upload pypi
 # python setup.py sdist bdist_wheel
 # twine upload dist/*
 
 setup(
     name='nice-sql',
-    version='2.0.0',
+    version='2.0.1',
     author='minusli',
     author_email='minusli@foxmail.com',
     url='https://github.com/minusli/nicesql',
     description='easy nice sql: decorator with sql',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests"]),
```

