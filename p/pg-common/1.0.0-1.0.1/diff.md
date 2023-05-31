# Comparing `tmp/pg_common-1.0.0.tar.gz` & `tmp/pg_common-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_common-1.0.0.tar", last modified: Tue May 30 09:48:15 2023, max compression
+gzip compressed data, was "pg_common-1.0.1.tar", last modified: Wed May 31 03:02:06 2023, max compression
```

## Comparing `pg_common-1.0.0.tar` & `pg_common-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-30 09:48:15.667108 pg_common-1.0.0/
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      114 2023-05-30 09:48:15.666458 pg_common-1.0.0/PKG-INFO
-drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-30 09:48:15.663011 pg_common-1.0.0/pg_common/
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      848 2023-05-30 09:30:52.000000 pg_common-1.0.0/pg_common/date.py
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)     1131 2023-05-30 09:30:52.000000 pg_common-1.0.0/pg_common/func.py
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      430 2023-05-30 09:30:52.000000 pg_common-1.0.0/pg_common/singleton.py
-drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-30 09:48:15.665634 pg_common-1.0.0/pg_common.egg-info/
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      114 2023-05-30 09:48:15.000000 pg_common-1.0.0/pg_common.egg-info/PKG-INFO
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      199 2023-05-30 09:48:15.000000 pg_common-1.0.0/pg_common.egg-info/SOURCES.txt
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)        1 2023-05-30 09:48:15.000000 pg_common-1.0.0/pg_common.egg-info/dependency_links.txt
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)       10 2023-05-30 09:48:15.000000 pg_common-1.0.0/pg_common.egg-info/top_level.txt
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)       38 2023-05-30 09:48:15.667280 pg_common-1.0.0/setup.cfg
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      246 2023-05-30 09:30:52.000000 pg_common-1.0.0/setup.py
+drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 03:02:06.812287 pg_common-1.0.1/
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      114 2023-05-31 03:02:06.812001 pg_common-1.0.1/PKG-INFO
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      724 2023-05-31 02:53:55.000000 pg_common-1.0.1/README.md
+drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 03:02:06.810184 pg_common-1.0.1/pg_common/
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      304 2023-05-31 02:54:30.000000 pg_common-1.0.1/pg_common/__init__.py
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)     1035 2023-05-31 02:16:58.000000 pg_common-1.0.1/pg_common/date.py
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)     1718 2023-05-31 02:53:14.000000 pg_common-1.0.1/pg_common/func.py
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      514 2023-05-31 02:15:02.000000 pg_common-1.0.1/pg_common/singleton.py
+drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 03:02:06.811624 pg_common-1.0.1/pg_common.egg-info/
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      114 2023-05-31 03:02:06.000000 pg_common-1.0.1/pg_common.egg-info/PKG-INFO
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      231 2023-05-31 03:02:06.000000 pg_common-1.0.1/pg_common.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)        1 2023-05-31 03:02:06.000000 pg_common-1.0.1/pg_common.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)       10 2023-05-31 03:02:06.000000 pg_common-1.0.1/pg_common.egg-info/top_level.txt
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)       38 2023-05-31 03:02:06.812375 pg_common-1.0.1/setup.cfg
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      246 2023-05-31 02:54:02.000000 pg_common-1.0.1/setup.py
```

### Comparing `pg_common-1.0.0/pg_common/date.py` & `pg_common-1.0.1/pg_common/date.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from datetime import datetime, timedelta
 
 
+__all__ = ["datetime_now", "datetime_delta", "datetime_2_str", "datetime_2_timestamp",
+           "str_delta_str", "str_2_datetime", "timestamp_2_str"]
+__auth__ = "baozilaji@gmail.com"
+
+
 def datetime_now():
     return datetime.now()
 
 
 def datetime_delta(_date_time, _delta_hours=0):
     return _date_time + timedelta(hours=_delta_hours)
```

