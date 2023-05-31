# Comparing `tmp/nice-sql-1.0.0.tar.gz` & `tmp/nice-sql-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nice-sql-1.0.0.tar", last modified: Tue May 23 13:26:04 2023, max compression
+gzip compressed data, was "nice-sql-2.0.0.tar", last modified: Wed May 31 07:24:28 2023, max compression
```

## Comparing `nice-sql-1.0.0.tar` & `nice-sql-2.0.0.tar`

### file list

```diff
@@ -1,31 +1,28 @@
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-23 13:26:04.956797 nice-sql-1.0.0/
--rw-r--r--   0 lichengming   (502) staff       (20)     3143 2023-05-23 13:26:04.956393 nice-sql-1.0.0/PKG-INFO
--rw-r--r--   0 lichengming   (502) staff       (20)     2840 2023-05-23 13:22:52.000000 nice-sql-1.0.0/README.md
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-23 13:26:04.945513 nice-sql-1.0.0/nice_sql.egg-info/
--rw-r--r--   0 lichengming   (502) staff       (20)     3143 2023-05-23 13:26:04.000000 nice-sql-1.0.0/nice_sql.egg-info/PKG-INFO
--rw-r--r--   0 lichengming   (502) staff       (20)      603 2023-05-23 13:26:04.000000 nice-sql-1.0.0/nice_sql.egg-info/SOURCES.txt
--rw-r--r--   0 lichengming   (502) staff       (20)        1 2023-05-23 13:26:04.000000 nice-sql-1.0.0/nice_sql.egg-info/dependency_links.txt
--rw-r--r--   0 lichengming   (502) staff       (20)       23 2023-05-23 13:26:04.000000 nice-sql-1.0.0/nice_sql.egg-info/requires.txt
--rw-r--r--   0 lichengming   (502) staff       (20)        8 2023-05-23 13:26:04.000000 nice-sql-1.0.0/nice_sql.egg-info/top_level.txt
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-23 13:26:04.945945 nice-sql-1.0.0/nicesql/
--rw-r--r--   0 lichengming   (502) staff       (20)        0 2023-05-23 10:10:49.000000 nice-sql-1.0.0/nicesql/__init__.py
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-23 13:26:04.950543 nice-sql-1.0.0/nicesql/engine/
--rw-r--r--   0 lichengming   (502) staff       (20)       54 2023-05-23 10:10:49.000000 nice-sql-1.0.0/nicesql/engine/__init__.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1002 2023-05-23 10:10:49.000000 nice-sql-1.0.0/nicesql/engine/base.py
--rw-r--r--   0 lichengming   (502) staff       (20)      330 2023-05-23 10:10:49.000000 nice-sql-1.0.0/nicesql/engine/impl_dummy.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1561 2023-05-23 13:15:25.000000 nice-sql-1.0.0/nicesql/engine/impl_mysql.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1439 2023-05-23 13:17:53.000000 nice-sql-1.0.0/nicesql/engine/impl_sqlite.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1089 2023-05-23 10:12:03.000000 nice-sql-1.0.0/nicesql/engine/reg.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1104 2023-05-23 13:14:48.000000 nice-sql-1.0.0/nicesql/engine/sqlformat.py
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-23 13:26:04.952829 nice-sql-1.0.0/nicesql/shortcut/
--rw-r--r--   0 lichengming   (502) staff       (20)      116 2023-05-23 10:10:49.000000 nice-sql-1.0.0/nicesql/shortcut/__init__.py
--rw-r--r--   0 lichengming   (502) staff       (20)      727 2023-05-23 10:10:49.000000 nice-sql-1.0.0/nicesql/shortcut/annotate.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1208 2023-05-23 12:55:23.000000 nice-sql-1.0.0/nicesql/shortcut/core.py
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-23 13:26:04.955779 nice-sql-1.0.0/nicesql/utils/
--rw-r--r--   0 lichengming   (502) staff       (20)      148 2023-05-23 13:11:34.000000 nice-sql-1.0.0/nicesql/utils/__init__.py
--rw-r--r--   0 lichengming   (502) staff       (20)      326 2023-05-23 10:10:49.000000 nice-sql-1.0.0/nicesql/utils/error.py
--rw-r--r--   0 lichengming   (502) staff       (20)      386 2023-05-23 10:10:49.000000 nice-sql-1.0.0/nicesql/utils/fill_model.py
--rw-r--r--   0 lichengming   (502) staff       (20)      556 2023-05-23 10:10:49.000000 nice-sql-1.0.0/nicesql/utils/parse_db_url.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1947 2023-05-23 12:48:20.000000 nice-sql-1.0.0/nicesql/utils/pick_value.py
--rw-r--r--   0 lichengming   (502) staff       (20)       38 2023-05-23 13:26:04.956928 nice-sql-1.0.0/setup.cfg
--rw-r--r--   0 lichengming   (502) staff       (20)      718 2023-05-23 10:12:03.000000 nice-sql-1.0.0/setup.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:24:27.997576 nice-sql-2.0.0/
+-rw-r--r--   0 lichengming   (502) staff       (20)     2617 2023-05-31 07:24:27.997030 nice-sql-2.0.0/PKG-INFO
+-rw-r--r--   0 lichengming   (502) staff       (20)     2316 2023-05-31 07:12:58.000000 nice-sql-2.0.0/README.md
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:24:27.988395 nice-sql-2.0.0/nice_sql.egg-info/
+-rw-r--r--   0 lichengming   (502) staff       (20)     2617 2023-05-31 07:24:27.000000 nice-sql-2.0.0/nice_sql.egg-info/PKG-INFO
+-rw-r--r--   0 lichengming   (502) staff       (20)      496 2023-05-31 07:24:27.000000 nice-sql-2.0.0/nice_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 lichengming   (502) staff       (20)        1 2023-05-31 07:24:27.000000 nice-sql-2.0.0/nice_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 lichengming   (502) staff       (20)       44 2023-05-31 07:24:27.000000 nice-sql-2.0.0/nice_sql.egg-info/requires.txt
+-rw-r--r--   0 lichengming   (502) staff       (20)        8 2023-05-31 07:24:27.000000 nice-sql-2.0.0/nice_sql.egg-info/top_level.txt
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:24:27.988755 nice-sql-2.0.0/nicesql/
+-rw-r--r--   0 lichengming   (502) staff       (20)        0 2023-05-30 06:32:39.000000 nice-sql-2.0.0/nicesql/__init__.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:24:27.990740 nice-sql-2.0.0/nicesql/engine/
+-rw-r--r--   0 lichengming   (502) staff       (20)      213 2023-05-30 12:32:57.000000 nice-sql-2.0.0/nicesql/engine/__init__.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     2226 2023-05-31 02:40:04.000000 nice-sql-2.0.0/nicesql/engine/_engines.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      400 2023-05-31 02:47:34.000000 nice-sql-2.0.0/nicesql/engine/_execute.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1629 2023-05-30 12:29:17.000000 nice-sql-2.0.0/nicesql/engine/_register.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1128 2023-05-30 07:03:46.000000 nice-sql-2.0.0/nicesql/engine/_result.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:24:27.992902 nice-sql-2.0.0/nicesql/shortcut/
+-rw-r--r--   0 lichengming   (502) staff       (20)       80 2023-05-30 08:54:09.000000 nice-sql-2.0.0/nicesql/shortcut/__init__.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     3147 2023-05-30 08:59:16.000000 nice-sql-2.0.0/nicesql/shortcut/_shortcut.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:24:27.994829 nice-sql-2.0.0/nicesql/sqlconv/
+-rw-r--r--   0 lichengming   (502) staff       (20)       50 2023-05-29 08:40:55.000000 nice-sql-2.0.0/nicesql/sqlconv/__init__.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1355 2023-05-29 11:43:20.000000 nice-sql-2.0.0/nicesql/sqlconv/_convert.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-31 07:24:27.996056 nice-sql-2.0.0/nicesql/utils/
+-rw-r--r--   0 lichengming   (502) staff       (20)       54 2023-05-31 02:46:13.000000 nice-sql-2.0.0/nicesql/utils/__init__.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      326 2023-05-23 10:10:49.000000 nice-sql-2.0.0/nicesql/utils/error.py
+-rw-r--r--   0 lichengming   (502) staff       (20)       38 2023-05-31 07:24:27.997793 nice-sql-2.0.0/setup.cfg
+-rw-r--r--   0 lichengming   (502) staff       (20)      749 2023-05-31 07:10:19.000000 nice-sql-2.0.0/setup.py
```

### Comparing `nice-sql-1.0.0/setup.py` & `nice-sql-2.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 
 # upload pypi
 # python setup.py sdist bdist_wheel
 # twine upload dist/*
 
 setup(
     name='nice-sql',
-    version='1.0.0',
+    version='2.0.0',
     author='minusli',
     author_email='minusli@foxmail.com',
-    url='https://github.com/657143946/nicesql',
+    url='https://github.com/minusli/nicesql',
     description='easy nice sql: decorator with sql',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests"]),
     python_requires='>=3',
     install_requires=[
         "pytest",
         "pymysql",
-        "DBUtils"
+        "DBUtils",
+        "nice-datapath==0.0.1",
     ],
     entry_points={},
     license="Apache License 2.0"
 )
```

