# Comparing `tmp/compensating-transaction-0.0.2.tar.gz` & `tmp/compensating-transaction-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compensating-transaction-0.0.2.tar", last modified: Fri Apr 14 09:05:35 2023, max compression
+gzip compressed data, was "compensating-transaction-0.0.3.tar", last modified: Wed May 31 10:03:19 2023, max compression
```

## Comparing `compensating-transaction-0.0.2.tar` & `compensating-transaction-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-04-14 09:05:35.946704 compensating-transaction-0.0.2/
--rw-r--r--   0 ivan       (501) staff       (20)     1064 2023-04-14 07:35:53.000000 compensating-transaction-0.0.2/LICENSE
--rw-r--r--   0 ivan       (501) staff       (20)      459 2023-04-14 09:05:35.946549 compensating-transaction-0.0.2/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)     2957 2023-04-14 08:23:35.000000 compensating-transaction-0.0.2/README.md
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-04-14 09:05:35.945626 compensating-transaction-0.0.2/compensating_transaction/
--rw-r--r--   0 ivan       (501) staff       (20)        0 2023-04-14 07:47:07.000000 compensating-transaction-0.0.2/compensating_transaction/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)      463 2023-04-14 07:39:08.000000 compensating-transaction-0.0.2/compensating_transaction/exceptions.py
--rw-r--r--   0 ivan       (501) staff       (20)     8500 2023-04-14 09:02:45.000000 compensating-transaction-0.0.2/compensating_transaction/transaction.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-04-14 09:05:35.946364 compensating-transaction-0.0.2/compensating_transaction.egg-info/
--rw-r--r--   0 ivan       (501) staff       (20)      459 2023-04-14 09:05:35.000000 compensating-transaction-0.0.2/compensating_transaction.egg-info/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)      334 2023-04-14 09:05:35.000000 compensating-transaction-0.0.2/compensating_transaction.egg-info/SOURCES.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2023-04-14 09:05:35.000000 compensating-transaction-0.0.2/compensating_transaction.egg-info/dependency_links.txt
--rw-r--r--   0 ivan       (501) staff       (20)       25 2023-04-14 09:05:35.000000 compensating-transaction-0.0.2/compensating_transaction.egg-info/top_level.txt
--rw-r--r--   0 ivan       (501) staff       (20)       38 2023-04-14 09:05:35.946750 compensating-transaction-0.0.2/setup.cfg
--rw-r--r--   0 ivan       (501) staff       (20)      747 2023-04-14 09:05:09.000000 compensating-transaction-0.0.2/setup.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-05-31 10:03:19.918025 compensating-transaction-0.0.3/
+-rw-r--r--   0 ivan       (501) staff       (20)     1064 2023-04-14 07:35:53.000000 compensating-transaction-0.0.3/LICENSE
+-rw-r--r--   0 ivan       (501) staff       (20)      459 2023-05-31 10:03:19.917587 compensating-transaction-0.0.3/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)     1430 2023-05-31 09:59:48.000000 compensating-transaction-0.0.3/README.md
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-05-31 10:03:19.915781 compensating-transaction-0.0.3/compensating_transaction/
+-rw-r--r--   0 ivan       (501) staff       (20)        0 2023-04-14 07:47:07.000000 compensating-transaction-0.0.3/compensating_transaction/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)      218 2023-05-31 09:57:44.000000 compensating-transaction-0.0.3/compensating_transaction/exceptions.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4810 2023-05-31 09:57:13.000000 compensating-transaction-0.0.3/compensating_transaction/transaction.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-05-31 10:03:19.917182 compensating-transaction-0.0.3/compensating_transaction.egg-info/
+-rw-r--r--   0 ivan       (501) staff       (20)      459 2023-05-31 10:03:19.000000 compensating-transaction-0.0.3/compensating_transaction.egg-info/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)      334 2023-05-31 10:03:19.000000 compensating-transaction-0.0.3/compensating_transaction.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        1 2023-05-31 10:03:19.000000 compensating-transaction-0.0.3/compensating_transaction.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan       (501) staff       (20)       25 2023-05-31 10:03:19.000000 compensating-transaction-0.0.3/compensating_transaction.egg-info/top_level.txt
+-rw-r--r--   0 ivan       (501) staff       (20)       38 2023-05-31 10:03:19.918099 compensating-transaction-0.0.3/setup.cfg
+-rw-r--r--   0 ivan       (501) staff       (20)      747 2023-05-31 10:00:24.000000 compensating-transaction-0.0.3/setup.py
```

### Comparing `compensating-transaction-0.0.2/LICENSE` & `compensating-transaction-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `compensating-transaction-0.0.2/setup.py` & `compensating-transaction-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author: rubbish
 #############################################
 
 from setuptools import find_packages, setup
 
 setup(
     name="compensating-transaction",
-    version="0.0.2",
+    version="0.0.3",
     keywords=("pip", "compensating-transaction", "atomicity"),
     description="compensating transaction",
     long_description="When the function execution fails, the function execution can be rolled back, and all previous function executions can be rolled back",
     license="MIT Licence",
     url="https://github.com/rubbish822/compensating-transaction",
     author="rubbish",
     author_email="rubbish@rubbish.com",
```

