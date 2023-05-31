# Comparing `tmp/auth_package-1.3.tar.gz` & `tmp/auth_package-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth_package-1.3.tar", last modified: Wed May 31 07:13:46 2023, max compression
+gzip compressed data, was "auth_package-1.4.tar", last modified: Wed May 31 07:45:47 2023, max compression
```

## Comparing `auth_package-1.3.tar` & `auth_package-1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 raminzamani   (501) staff       (20)        0 2023-05-31 07:13:46.668066 auth_package-1.3/
--rw-r--r--   0 raminzamani   (501) staff       (20)     1061 2023-05-29 19:53:56.000000 auth_package-1.3/LICENSE.txt
--rw-r--r--   0 raminzamani   (501) staff       (20)      989 2023-05-31 07:13:46.668159 auth_package-1.3/PKG-INFO
--rw-r--r--   0 raminzamani   (501) staff       (20)      704 2023-05-31 06:59:59.000000 auth_package-1.3/README.md
-drwxr-xr-x   0 raminzamani   (501) staff       (20)        0 2023-05-31 07:13:46.666840 auth_package-1.3/auth_package/
--rw-r--r--   0 raminzamani   (501) staff       (20)      233 2023-05-29 19:39:45.000000 auth_package-1.3/auth_package/__init__.py
--rw-r--r--   0 raminzamani   (501) staff       (20)     2938 2023-05-31 05:03:43.000000 auth_package-1.3/auth_package/permission.py
--rw-r--r--   0 raminzamani   (501) staff       (20)     1793 2023-05-31 05:04:37.000000 auth_package-1.3/auth_package/user.py
-drwxr-xr-x   0 raminzamani   (501) staff       (20)        0 2023-05-31 07:13:46.667920 auth_package-1.3/auth_package.egg-info/
--rw-r--r--   0 raminzamani   (501) staff       (20)      989 2023-05-31 07:13:46.000000 auth_package-1.3/auth_package.egg-info/PKG-INFO
--rw-r--r--   0 raminzamani   (501) staff       (20)      292 2023-05-31 07:13:46.000000 auth_package-1.3/auth_package.egg-info/SOURCES.txt
--rw-r--r--   0 raminzamani   (501) staff       (20)        1 2023-05-31 07:13:46.000000 auth_package-1.3/auth_package.egg-info/dependency_links.txt
--rw-r--r--   0 raminzamani   (501) staff       (20)        9 2023-05-31 07:13:46.000000 auth_package-1.3/auth_package.egg-info/requires.txt
--rw-r--r--   0 raminzamani   (501) staff       (20)       13 2023-05-31 07:13:46.000000 auth_package-1.3/auth_package.egg-info/top_level.txt
--rw-r--r--   0 raminzamani   (501) staff       (20)       79 2023-05-31 07:13:46.668531 auth_package-1.3/setup.cfg
--rw-r--r--   0 raminzamani   (501) staff       (20)     1862 2023-05-31 07:11:59.000000 auth_package-1.3/setup.py
+drwxr-xr-x   0 raminzamani   (501) staff       (20)        0 2023-05-31 07:45:47.159380 auth_package-1.4/
+-rw-r--r--   0 raminzamani   (501) staff       (20)     1061 2023-05-29 19:53:56.000000 auth_package-1.4/LICENSE.txt
+-rw-r--r--   0 raminzamani   (501) staff       (20)     1735 2023-05-31 07:45:47.159449 auth_package-1.4/PKG-INFO
+-rw-r--r--   0 raminzamani   (501) staff       (20)      704 2023-05-31 07:21:10.000000 auth_package-1.4/README.md
+drwxr-xr-x   0 raminzamani   (501) staff       (20)        0 2023-05-31 07:45:47.158434 auth_package-1.4/auth_package/
+-rw-r--r--   0 raminzamani   (501) staff       (20)      233 2023-05-29 19:39:45.000000 auth_package-1.4/auth_package/__init__.py
+-rw-r--r--   0 raminzamani   (501) staff       (20)     2938 2023-05-31 05:03:43.000000 auth_package-1.4/auth_package/permission.py
+-rw-r--r--   0 raminzamani   (501) staff       (20)     1793 2023-05-31 05:04:37.000000 auth_package-1.4/auth_package/user.py
+drwxr-xr-x   0 raminzamani   (501) staff       (20)        0 2023-05-31 07:45:47.159229 auth_package-1.4/auth_package.egg-info/
+-rw-r--r--   0 raminzamani   (501) staff       (20)     1735 2023-05-31 07:45:47.000000 auth_package-1.4/auth_package.egg-info/PKG-INFO
+-rw-r--r--   0 raminzamani   (501) staff       (20)      292 2023-05-31 07:45:47.000000 auth_package-1.4/auth_package.egg-info/SOURCES.txt
+-rw-r--r--   0 raminzamani   (501) staff       (20)        1 2023-05-31 07:45:47.000000 auth_package-1.4/auth_package.egg-info/dependency_links.txt
+-rw-r--r--   0 raminzamani   (501) staff       (20)        9 2023-05-31 07:45:47.000000 auth_package-1.4/auth_package.egg-info/requires.txt
+-rw-r--r--   0 raminzamani   (501) staff       (20)       13 2023-05-31 07:45:47.000000 auth_package-1.4/auth_package.egg-info/top_level.txt
+-rw-r--r--   0 raminzamani   (501) staff       (20)       79 2023-05-31 07:45:47.160284 auth_package-1.4/setup.cfg
+-rw-r--r--   0 raminzamani   (501) staff       (20)     1369 2023-05-31 07:45:36.000000 auth_package-1.4/setup.py
```

### Comparing `auth_package-1.3/LICENSE.txt` & `auth_package-1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `auth_package-1.3/README.md` & `auth_package-1.4/README.md`

 * *Files identical despite different names*

### Comparing `auth_package-1.3/auth_package/permission.py` & `auth_package-1.4/auth_package/permission.py`

 * *Files identical despite different names*

### Comparing `auth_package-1.3/auth_package/user.py` & `auth_package-1.4/auth_package/user.py`

 * *Files identical despite different names*

