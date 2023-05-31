# Comparing `tmp/pg_common-1.0.2.tar.gz` & `tmp/pg_common-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_common-1.0.2.tar", last modified: Wed May 31 06:12:03 2023, max compression
+gzip compressed data, was "pg_common-1.0.3.tar", last modified: Wed May 31 06:13:59 2023, max compression
```

## Comparing `pg_common-1.0.2.tar` & `pg_common-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 06:12:03.780015 pg_common-1.0.2/
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      135 2023-05-31 06:12:03.779635 pg_common-1.0.2/PKG-INFO
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      806 2023-05-31 05:35:36.000000 pg_common-1.0.2/README.md
-drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 06:12:03.777500 pg_common-1.0.2/pg_common/
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      387 2023-05-31 05:39:06.000000 pg_common-1.0.2/pg_common/__init__.py
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)     1035 2023-05-31 02:16:58.000000 pg_common-1.0.2/pg_common/date.py
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)     2440 2023-05-31 05:37:53.000000 pg_common-1.0.2/pg_common/func.py
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      514 2023-05-31 02:15:02.000000 pg_common-1.0.2/pg_common/singleton.py
-drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 06:12:03.779182 pg_common-1.0.2/pg_common.egg-info/
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      135 2023-05-31 06:12:03.000000 pg_common-1.0.2/pg_common.egg-info/PKG-INFO
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      231 2023-05-31 06:12:03.000000 pg_common-1.0.2/pg_common.egg-info/SOURCES.txt
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)        1 2023-05-31 06:12:03.000000 pg_common-1.0.2/pg_common.egg-info/dependency_links.txt
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)       10 2023-05-31 06:12:03.000000 pg_common-1.0.2/pg_common.egg-info/top_level.txt
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)       38 2023-05-31 06:12:03.780110 pg_common-1.0.2/setup.cfg
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      270 2023-05-31 06:06:37.000000 pg_common-1.0.2/setup.py
+drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 06:13:59.176784 pg_common-1.0.3/
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      135 2023-05-31 06:13:59.176100 pg_common-1.0.3/PKG-INFO
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      806 2023-05-31 05:35:36.000000 pg_common-1.0.3/README.md
+drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 06:13:59.174151 pg_common-1.0.3/pg_common/
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      387 2023-05-31 05:39:06.000000 pg_common-1.0.3/pg_common/__init__.py
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)     1035 2023-05-31 02:16:58.000000 pg_common-1.0.3/pg_common/date.py
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)     2440 2023-05-31 05:37:53.000000 pg_common-1.0.3/pg_common/func.py
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      514 2023-05-31 02:15:02.000000 pg_common-1.0.3/pg_common/singleton.py
+drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 06:13:59.175636 pg_common-1.0.3/pg_common.egg-info/
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      135 2023-05-31 06:13:59.000000 pg_common-1.0.3/pg_common.egg-info/PKG-INFO
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      231 2023-05-31 06:13:59.000000 pg_common-1.0.3/pg_common.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)        1 2023-05-31 06:13:59.000000 pg_common-1.0.3/pg_common.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)       10 2023-05-31 06:13:59.000000 pg_common-1.0.3/pg_common.egg-info/top_level.txt
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)       38 2023-05-31 06:13:59.176907 pg_common-1.0.3/setup.cfg
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      270 2023-05-31 06:13:56.000000 pg_common-1.0.3/setup.py
```

### Comparing `pg_common-1.0.2/README.md` & `pg_common-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pg_common-1.0.2/pg_common/date.py` & `pg_common-1.0.3/pg_common/date.py`

 * *Files identical despite different names*

### Comparing `pg_common-1.0.2/pg_common/func.py` & `pg_common-1.0.3/pg_common/func.py`

 * *Files identical despite different names*

### Comparing `pg_common-1.0.2/pg_common/singleton.py` & `pg_common-1.0.3/pg_common/singleton.py`

 * *Files identical despite different names*

