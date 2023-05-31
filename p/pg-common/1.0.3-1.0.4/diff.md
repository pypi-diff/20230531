# Comparing `tmp/pg_common-1.0.3.tar.gz` & `tmp/pg_common-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_common-1.0.3.tar", last modified: Wed May 31 06:13:59 2023, max compression
+gzip compressed data, was "pg_common-1.0.4.tar", last modified: Wed May 31 11:18:23 2023, max compression
```

## Comparing `pg_common-1.0.3.tar` & `pg_common-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 06:13:59.176784 pg_common-1.0.3/
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      135 2023-05-31 06:13:59.176100 pg_common-1.0.3/PKG-INFO
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      806 2023-05-31 05:35:36.000000 pg_common-1.0.3/README.md
-drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 06:13:59.174151 pg_common-1.0.3/pg_common/
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      387 2023-05-31 05:39:06.000000 pg_common-1.0.3/pg_common/__init__.py
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)     1035 2023-05-31 02:16:58.000000 pg_common-1.0.3/pg_common/date.py
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)     2440 2023-05-31 05:37:53.000000 pg_common-1.0.3/pg_common/func.py
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      514 2023-05-31 02:15:02.000000 pg_common-1.0.3/pg_common/singleton.py
-drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 06:13:59.175636 pg_common-1.0.3/pg_common.egg-info/
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      135 2023-05-31 06:13:59.000000 pg_common-1.0.3/pg_common.egg-info/PKG-INFO
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      231 2023-05-31 06:13:59.000000 pg_common-1.0.3/pg_common.egg-info/SOURCES.txt
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)        1 2023-05-31 06:13:59.000000 pg_common-1.0.3/pg_common.egg-info/dependency_links.txt
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)       10 2023-05-31 06:13:59.000000 pg_common-1.0.3/pg_common.egg-info/top_level.txt
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)       38 2023-05-31 06:13:59.176907 pg_common-1.0.3/setup.cfg
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      270 2023-05-31 06:13:56.000000 pg_common-1.0.3/setup.py
+drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 11:18:23.338735 pg_common-1.0.4/
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      135 2023-05-31 11:18:23.338391 pg_common-1.0.4/PKG-INFO
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      892 2023-05-31 09:47:29.000000 pg_common-1.0.4/README.md
+drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 11:18:23.327804 pg_common-1.0.4/pg_common/
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      406 2023-05-31 09:45:47.000000 pg_common-1.0.4/pg_common/__init__.py
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)     1035 2023-05-31 02:16:58.000000 pg_common-1.0.4/pg_common/date.py
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)     2589 2023-05-31 09:47:51.000000 pg_common-1.0.4/pg_common/func.py
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      514 2023-05-31 02:15:02.000000 pg_common-1.0.4/pg_common/singleton.py
+drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 11:18:23.337892 pg_common-1.0.4/pg_common.egg-info/
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      135 2023-05-31 11:18:23.000000 pg_common-1.0.4/pg_common.egg-info/PKG-INFO
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      231 2023-05-31 11:18:23.000000 pg_common-1.0.4/pg_common.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)        1 2023-05-31 11:18:23.000000 pg_common-1.0.4/pg_common.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)       10 2023-05-31 11:18:23.000000 pg_common-1.0.4/pg_common.egg-info/top_level.txt
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)       38 2023-05-31 11:18:23.338846 pg_common-1.0.4/setup.cfg
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      270 2023-05-31 11:18:20.000000 pg_common-1.0.4/setup.py
```

### Comparing `pg_common-1.0.3/README.md` & `pg_common-1.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 func.log_print("INFO", A)
 
 
 func.log_print("INFO", func.rand_str(10))
 func.log_print("INFO", func.rand_num(4))
 
 func.log_print("INFO", func.json_pretty({"A": 1, "B": [1,2,3]}))
+
+func.log_info(func.is_valid_ip("0.0.0.0"))
+func.log_info(func.is_valid_ip("0.0.0."))
 ```
 
 singleton.py
 ```shell script
 from pg_common import singleton
 
 class A(singleton.SingletonBase):
```

### Comparing `pg_common-1.0.3/pg_common/date.py` & `pg_common-1.0.4/pg_common/date.py`

 * *Files identical despite different names*

### Comparing `pg_common-1.0.3/pg_common/func.py` & `pg_common-1.0.4/pg_common/func.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 import asyncio
 from .date import datetime_now
 import random
 import json
 from datetime import date, datetime
+import re
 
 
 _STR_CHARS = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789_"
 _NUM_CHARS = "0123456789"
+_IP_PATTERN = r'^(\d{1,3}\.){3}\d{1,3}$'
 
 
 __all__ = ["merge_dict", "log_print", "start_coroutines", "rand_str", "rand_num",
            "log_debug", "log_error", "log_info", "log_warn",
+           "is_valid_ip",
            "ComplexEncoder", "json_pretty"]
 __auth__ = "baozilaji@gmail.com"
 
 
+def is_valid_ip(ip):
+    return re.match(_IP_PATTERN, ip) is not None
+
+
 def _random(_len: int = 6, _type: int = 0):
     _ret = ""
     _chars = _STR_CHARS if _type == 0 else _NUM_CHARS
     _len_total = len(_chars)
     for i in range(_len):
         _ret += _chars[random.randint(0, _len_total-1)]
     return _ret
```

### Comparing `pg_common-1.0.3/pg_common/singleton.py` & `pg_common-1.0.4/pg_common/singleton.py`

 * *Files identical despite different names*

