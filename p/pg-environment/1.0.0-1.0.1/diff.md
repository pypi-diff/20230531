# Comparing `tmp/pg_environment-1.0.0.tar.gz` & `tmp/pg_environment-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_environment-1.0.0.tar", last modified: Wed May 31 11:11:24 2023, max compression
+gzip compressed data, was "pg_environment-1.0.1.tar", last modified: Wed May 31 11:14:55 2023, max compression
```

## Comparing `pg_environment-1.0.0.tar` & `pg_environment-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 11:11:24.501292 pg_environment-1.0.0/
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      141 2023-05-31 11:11:24.500962 pg_environment-1.0.0/PKG-INFO
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      537 2023-05-31 10:45:34.000000 pg_environment-1.0.0/README.md
-drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 11:11:24.497886 pg_environment-1.0.0/pg_env/
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      101 2023-05-31 10:46:51.000000 pg_environment-1.0.0/pg_env/__init__.py
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)     2446 2023-05-31 10:59:17.000000 pg_environment-1.0.0/pg_env/config.py
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      341 2023-05-31 10:54:58.000000 pg_environment-1.0.0/pg_env/define.py
-drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 11:11:24.500543 pg_environment-1.0.0/pg_environment.egg-info/
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      141 2023-05-31 11:11:24.000000 pg_environment-1.0.0/pg_environment.egg-info/PKG-INFO
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      260 2023-05-31 11:11:24.000000 pg_environment-1.0.0/pg_environment.egg-info/SOURCES.txt
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)        1 2023-05-31 11:11:24.000000 pg_environment-1.0.0/pg_environment.egg-info/dependency_links.txt
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)       13 2023-05-31 11:11:24.000000 pg_environment-1.0.0/pg_environment.egg-info/requires.txt
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)        7 2023-05-31 11:11:24.000000 pg_environment-1.0.0/pg_environment.egg-info/top_level.txt
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)       38 2023-05-31 11:11:24.501396 pg_environment-1.0.0/setup.cfg
--rw-r--r--   0 zhangdanfeng   (501) staff       (20)      315 2023-05-31 11:11:20.000000 pg_environment-1.0.0/setup.py
+drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 11:14:55.523012 pg_environment-1.0.1/
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      141 2023-05-31 11:14:55.522676 pg_environment-1.0.1/PKG-INFO
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      537 2023-05-31 10:45:34.000000 pg_environment-1.0.1/README.md
+drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 11:14:55.520545 pg_environment-1.0.1/pg_environment/
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      101 2023-05-31 10:46:51.000000 pg_environment-1.0.1/pg_environment/__init__.py
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)     2446 2023-05-31 10:59:17.000000 pg_environment-1.0.1/pg_environment/config.py
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      341 2023-05-31 10:54:58.000000 pg_environment-1.0.1/pg_environment/define.py
+drwxr-xr-x   0 zhangdanfeng   (501) staff       (20)        0 2023-05-31 11:14:55.522158 pg_environment-1.0.1/pg_environment.egg-info/
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      141 2023-05-31 11:14:55.000000 pg_environment-1.0.1/pg_environment.egg-info/PKG-INFO
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      284 2023-05-31 11:14:55.000000 pg_environment-1.0.1/pg_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)        1 2023-05-31 11:14:55.000000 pg_environment-1.0.1/pg_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)       13 2023-05-31 11:14:55.000000 pg_environment-1.0.1/pg_environment.egg-info/requires.txt
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)       15 2023-05-31 11:14:55.000000 pg_environment-1.0.1/pg_environment.egg-info/top_level.txt
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)       38 2023-05-31 11:14:55.523110 pg_environment-1.0.1/setup.cfg
+-rw-r--r--   0 zhangdanfeng   (501) staff       (20)      323 2023-05-31 11:14:45.000000 pg_environment-1.0.1/setup.py
```

### Comparing `pg_environment-1.0.0/README.md` & `pg_environment-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pg_environment-1.0.0/pg_env/config.py` & `pg_environment-1.0.1/pg_environment/config.py`

 * *Files identical despite different names*

