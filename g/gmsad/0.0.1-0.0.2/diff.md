# Comparing `tmp/gmsad-0.0.1.tar.gz` & `tmp/gmsad-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmsad-0.0.1.tar", last modified: Wed May 31 11:24:36 2023, max compression
+gzip compressed data, was "gmsad-0.0.2.tar", last modified: Wed May 31 11:59:11 2023, max compression
```

## Comparing `gmsad-0.0.1.tar` & `gmsad-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:24:36.828142 gmsad-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 11:24:01.000000 gmsad-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-31 11:24:36.828142 gmsad-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-31 11:24:01.000000 gmsad-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:24:36.828142 gmsad-0.0.1/gmsad/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-31 11:24:01.000000 gmsad-0.0.1/gmsad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:24:36.828142 gmsad-0.0.1/gmsad/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:24:01.000000 gmsad-0.0.1/gmsad/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-31 11:24:01.000000 gmsad-0.0.1/gmsad/bin/gmsad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-31 11:24:01.000000 gmsad-0.0.1/gmsad/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-31 11:24:01.000000 gmsad-0.0.1/gmsad/enctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-05-31 11:24:01.000000 gmsad-0.0.1/gmsad/gmsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-31 11:24:01.000000 gmsad-0.0.1/gmsad/keytab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-31 11:24:01.000000 gmsad-0.0.1/gmsad/ldap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-05-31 11:24:01.000000 gmsad-0.0.1/gmsad/salt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-31 11:24:01.000000 gmsad-0.0.1/gmsad/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:24:36.828142 gmsad-0.0.1/gmsad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-31 11:24:36.000000 gmsad-0.0.1/gmsad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-31 11:24:36.000000 gmsad-0.0.1/gmsad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:24:36.000000 gmsad-0.0.1/gmsad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 11:24:36.000000 gmsad-0.0.1/gmsad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 11:24:36.000000 gmsad-0.0.1/gmsad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 11:24:36.000000 gmsad-0.0.1/gmsad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 11:24:36.828142 gmsad-0.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      938 2023-05-31 11:24:01.000000 gmsad-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:24:36.828142 gmsad-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-31 11:24:01.000000 gmsad-0.0.1/tests/test_enctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-05-31 11:24:01.000000 gmsad-0.0.1/tests/test_gmsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-31 11:24:01.000000 gmsad-0.0.1/tests/test_keytab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:59:11.042485 gmsad-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 11:58:44.000000 gmsad-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-31 11:59:11.042485 gmsad-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-31 11:58:44.000000 gmsad-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:59:11.038485 gmsad-0.0.2/gmsad/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-31 11:58:44.000000 gmsad-0.0.2/gmsad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:59:11.042485 gmsad-0.0.2/gmsad/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:58:44.000000 gmsad-0.0.2/gmsad/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-31 11:58:44.000000 gmsad-0.0.2/gmsad/bin/gmsad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-31 11:58:44.000000 gmsad-0.0.2/gmsad/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-31 11:58:44.000000 gmsad-0.0.2/gmsad/enctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-05-31 11:58:44.000000 gmsad-0.0.2/gmsad/gmsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-31 11:58:44.000000 gmsad-0.0.2/gmsad/keytab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-31 11:58:44.000000 gmsad-0.0.2/gmsad/ldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-05-31 11:58:44.000000 gmsad-0.0.2/gmsad/salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-31 11:58:44.000000 gmsad-0.0.2/gmsad/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:59:11.038485 gmsad-0.0.2/gmsad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-31 11:59:11.000000 gmsad-0.0.2/gmsad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-31 11:59:11.000000 gmsad-0.0.2/gmsad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:59:11.000000 gmsad-0.0.2/gmsad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 11:59:11.000000 gmsad-0.0.2/gmsad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 11:59:11.000000 gmsad-0.0.2/gmsad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 11:59:11.000000 gmsad-0.0.2/gmsad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 11:59:11.042485 gmsad-0.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-05-31 11:58:44.000000 gmsad-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:59:11.042485 gmsad-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-31 11:58:44.000000 gmsad-0.0.2/tests/test_enctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-05-31 11:58:44.000000 gmsad-0.0.2/tests/test_gmsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-31 11:58:44.000000 gmsad-0.0.2/tests/test_keytab.py
```

### Comparing `gmsad-0.0.1/LICENSE` & `gmsad-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gmsad-0.0.1/PKG-INFO` & `gmsad-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gmsad
-Version: 0.0.1
+Version: 0.0.2
 Summary: Linux service to manage gMSA accounts
-Author: CTSI
+Author: Vincent Ruello
 Author-email: vincent.ruello@cea.fr
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # gmsad
```

### Comparing `gmsad-0.0.1/README.md` & `gmsad-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gmsad-0.0.1/gmsad/__init__.py` & `gmsad-0.0.2/gmsad/__init__.py`

 * *Files identical despite different names*

### Comparing `gmsad-0.0.1/gmsad/bin/gmsad.py` & `gmsad-0.0.2/gmsad/bin/gmsad.py`

 * *Files identical despite different names*

### Comparing `gmsad-0.0.1/gmsad/config.py` & `gmsad-0.0.2/gmsad/config.py`

 * *Files identical despite different names*

### Comparing `gmsad-0.0.1/gmsad/enctypes.py` & `gmsad-0.0.2/gmsad/enctypes.py`

 * *Files identical despite different names*

### Comparing `gmsad-0.0.1/gmsad/gmsa.py` & `gmsad-0.0.2/gmsad/gmsa.py`

 * *Files identical despite different names*

### Comparing `gmsad-0.0.1/gmsad/keytab.py` & `gmsad-0.0.2/gmsad/keytab.py`

 * *Files identical despite different names*

### Comparing `gmsad-0.0.1/gmsad/ldap.py` & `gmsad-0.0.2/gmsad/ldap.py`

 * *Files identical despite different names*

### Comparing `gmsad-0.0.1/gmsad/salt.py` & `gmsad-0.0.2/gmsad/salt.py`

 * *Files identical despite different names*

### Comparing `gmsad-0.0.1/gmsad/utils.py` & `gmsad-0.0.2/gmsad/utils.py`

 * *Files identical despite different names*

### Comparing `gmsad-0.0.1/gmsad.egg-info/PKG-INFO` & `gmsad-0.0.2/gmsad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: gmsad
-Version: 0.0.1
+Version: 0.0.2
 Summary: Linux service to manage gMSA accounts
-Author: CTSI
+Author: Vincent Ruello
 Author-email: vincent.ruello@cea.fr
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # gmsad
```

### Comparing `gmsad-0.0.1/setup.py` & `gmsad-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # cf https://packaging.python.org/en/latest/guides/making-a-pypi-friendly-readme/
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='gmsad',
-    version='0.0.1',
-    author='CTSI',
+    version='0.0.2',
+    author='Vincent Ruello',
     author_email='vincent.ruello@cea.fr',
     description="Linux service to manage gMSA accounts",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(exclude=['tests']),
     entry_points={
         'console_scripts': [
```

### Comparing `gmsad-0.0.1/tests/test_enctypes.py` & `gmsad-0.0.2/tests/test_enctypes.py`

 * *Files identical despite different names*

### Comparing `gmsad-0.0.1/tests/test_gmsa.py` & `gmsad-0.0.2/tests/test_gmsa.py`

 * *Files identical despite different names*

### Comparing `gmsad-0.0.1/tests/test_keytab.py` & `gmsad-0.0.2/tests/test_keytab.py`

 * *Files identical despite different names*

