# Comparing `tmp/aleph-message-0.4.0a1.tar.gz` & `tmp/aleph-message-0.4.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleph-message-0.4.0a1.tar", last modified: Wed May 31 12:38:01 2023, max compression
+gzip compressed data, was "aleph-message-0.4.0a2.tar", last modified: Wed May 31 13:58:12 2023, max compression
```

## Comparing `aleph-message-0.4.0a1.tar` & `aleph-message-0.4.0a2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:38:01.992991 aleph-message-0.4.0a1/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-01-12 17:02:10.000000 aleph-message-0.4.0a1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2010 2023-05-31 12:38:01.992991 aleph-message-0.4.0a1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1468 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:38:01.991991 aleph-message-0.4.0a1/aleph_message/
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/__init__.py
--rw-r--r--   0 root         (0) root         (0)       44 2023-01-12 17:02:10.000000 aleph-message-0.4.0a1/aleph_message/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:38:01.992991 aleph-message-0.4.0a1/aleph_message/models/
--rw-r--r--   0 root         (0) root         (0)    12676 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-01-12 17:02:10.000000 aleph-message-0.4.0a1/aleph_message/models/abstract.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:38:01.992991 aleph-message-0.4.0a1/aleph_message/models/execution/
--rw-r--r--   0 root         (0) root         (0)      192 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/models/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1333 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/models/execution/abstract.py
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/models/execution/base.py
--rw-r--r--   0 root         (0) root         (0)     3345 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/models/execution/environment.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-05-31 12:29:26.000000 aleph-message-0.4.0a1/aleph_message/models/execution/instance.py
--rw-r--r--   0 root         (0) root         (0)     1615 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/models/execution/program.py
--rw-r--r--   0 root         (0) root         (0)     1607 2023-05-31 12:29:26.000000 aleph-message-0.4.0a1/aleph_message/models/execution/volume.py
--rw-r--r--   0 root         (0) root         (0)     1831 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/models/item_hash.py
--rw-r--r--   0 root         (0) root         (0)      483 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/status.py
--rw-r--r--   0 root         (0) root         (0)      505 2023-05-12 16:19:21.000000 aleph-message-0.4.0a1/aleph_message/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:38:01.991991 aleph-message-0.4.0a1/aleph_message.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2010 2023-05-31 12:38:01.000000 aleph-message-0.4.0a1/aleph_message.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      708 2023-05-31 12:38:01.000000 aleph-message-0.4.0a1/aleph_message.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 12:38:01.000000 aleph-message-0.4.0a1/aleph_message.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-31 12:38:01.000000 aleph-message-0.4.0a1/aleph_message.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-31 12:38:01.000000 aleph-message-0.4.0a1/aleph_message.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 12:38:01.992991 aleph-message-0.4.0a1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1438 2023-05-31 12:31:55.000000 aleph-message-0.4.0a1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:58:12.366481 aleph-message-0.4.0a2/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-01-12 17:02:10.000000 aleph-message-0.4.0a2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-05-31 13:58:12.366481 aleph-message-0.4.0a2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1468 2023-05-12 16:19:21.000000 aleph-message-0.4.0a2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:58:12.365481 aleph-message-0.4.0a2/aleph_message/
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-12 16:19:21.000000 aleph-message-0.4.0a2/aleph_message/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       44 2023-01-12 17:02:10.000000 aleph-message-0.4.0a2/aleph_message/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:58:12.366481 aleph-message-0.4.0a2/aleph_message/models/
+-rw-r--r--   0 root         (0) root         (0)    12676 2023-05-12 16:19:21.000000 aleph-message-0.4.0a2/aleph_message/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-01-12 17:02:10.000000 aleph-message-0.4.0a2/aleph_message/models/abstract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:58:12.366481 aleph-message-0.4.0a2/aleph_message/models/execution/
+-rw-r--r--   0 root         (0) root         (0)      192 2023-05-12 16:19:21.000000 aleph-message-0.4.0a2/aleph_message/models/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-05-12 16:19:21.000000 aleph-message-0.4.0a2/aleph_message/models/execution/abstract.py
+-rw-r--r--   0 root         (0) root         (0)      465 2023-05-12 16:19:21.000000 aleph-message-0.4.0a2/aleph_message/models/execution/base.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-05-12 16:19:21.000000 aleph-message-0.4.0a2/aleph_message/models/execution/environment.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-05-31 12:29:26.000000 aleph-message-0.4.0a2/aleph_message/models/execution/instance.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2023-05-12 16:19:21.000000 aleph-message-0.4.0a2/aleph_message/models/execution/program.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-05-31 12:29:26.000000 aleph-message-0.4.0a2/aleph_message/models/execution/volume.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-05-12 16:19:21.000000 aleph-message-0.4.0a2/aleph_message/models/item_hash.py
+-rw-r--r--   0 root         (0) root         (0)      483 2023-05-12 16:19:21.000000 aleph-message-0.4.0a2/aleph_message/status.py
+-rw-r--r--   0 root         (0) root         (0)      505 2023-05-12 16:19:21.000000 aleph-message-0.4.0a2/aleph_message/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:58:12.366481 aleph-message-0.4.0a2/aleph_message.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-05-31 13:58:12.000000 aleph-message-0.4.0a2/aleph_message.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      708 2023-05-31 13:58:12.000000 aleph-message-0.4.0a2/aleph_message.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 13:58:12.000000 aleph-message-0.4.0a2/aleph_message.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-31 13:58:12.000000 aleph-message-0.4.0a2/aleph_message.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-31 13:58:12.000000 aleph-message-0.4.0a2/aleph_message.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 13:58:12.366481 aleph-message-0.4.0a2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-05-31 13:57:31.000000 aleph-message-0.4.0a2/setup.py
```

### Comparing `aleph-message-0.4.0a1/LICENSE` & `aleph-message-0.4.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.0a1/PKG-INFO` & `aleph-message-0.4.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-message
-Version: 0.4.0a1
+Version: 0.4.0a2
 Summary: Aleph.im message specification 
 Home-page: https://github.com/aleph-im/aleph-message
 Author: Hugo Herter
 Author-email: git@hugoherter.com
 License: MIT
 Keywords: aleph.im message validation specification
 Platform: UNKNOWN
```

### Comparing `aleph-message-0.4.0a1/README.md` & `aleph-message-0.4.0a2/README.md`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.0a1/aleph_message/models/__init__.py` & `aleph-message-0.4.0a2/aleph_message/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.0a1/aleph_message/models/abstract.py` & `aleph-message-0.4.0a2/aleph_message/models/abstract.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.0a1/aleph_message/models/execution/abstract.py` & `aleph-message-0.4.0a2/aleph_message/models/execution/abstract.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.0a1/aleph_message/models/execution/environment.py` & `aleph-message-0.4.0a2/aleph_message/models/execution/environment.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.0a1/aleph_message/models/execution/instance.py` & `aleph-message-0.4.0a2/aleph_message/models/execution/instance.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.0a1/aleph_message/models/execution/program.py` & `aleph-message-0.4.0a2/aleph_message/models/execution/program.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.0a1/aleph_message/models/execution/volume.py` & `aleph-message-0.4.0a2/aleph_message/models/execution/volume.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.0a1/aleph_message/models/item_hash.py` & `aleph-message-0.4.0a2/aleph_message/models/item_hash.py`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.0a1/aleph_message.egg-info/PKG-INFO` & `aleph-message-0.4.0a2/aleph_message.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-message
-Version: 0.4.0a1
+Version: 0.4.0a2
 Summary: Aleph.im message specification 
 Home-page: https://github.com/aleph-im/aleph-message
 Author: Hugo Herter
 Author-email: git@hugoherter.com
 License: MIT
 Keywords: aleph.im message validation specification
 Platform: UNKNOWN
```

### Comparing `aleph-message-0.4.0a1/aleph_message.egg-info/SOURCES.txt` & `aleph-message-0.4.0a2/aleph_message.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aleph-message-0.4.0a1/setup.py` & `aleph-message-0.4.0a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 with open('README.md') as file:
     long_description = file.read()
 
 setup(name='aleph-message',
-      version='0.4.0a1',
+      version='0.4.0a2',
       description='Aleph.im message specification ',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Hugo Herter',
       author_email='git@hugoherter.com',
       url='https://github.com/aleph-im/aleph-message',
       packages=['aleph_message', 'aleph_message.models', 'aleph_message.models.execution'],
```

