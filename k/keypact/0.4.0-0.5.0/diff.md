# Comparing `tmp/keypact-0.4.0.tar.gz` & `tmp/keypact-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypact-0.4.0.tar", last modified: Mon May 29 17:19:52 2023, max compression
+gzip compressed data, was "keypact-0.5.0.tar", last modified: Wed May 31 14:56:53 2023, max compression
```

## Comparing `keypact-0.4.0.tar` & `keypact-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:19:52.981456 keypact-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-29 17:19:39.000000 keypact-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-29 17:19:52.981456 keypact-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-29 17:19:39.000000 keypact-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:19:52.981456 keypact-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-29 17:19:39.000000 keypact-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:19:52.973456 keypact-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:19:52.977456 keypact-0.4.0/src/keypact/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 17:19:39.000000 keypact-0.4.0/src/keypact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-29 17:19:39.000000 keypact-0.4.0/src/keypact/keypact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:19:52.981456 keypact-0.4.0/src/keypact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-29 17:19:52.000000 keypact-0.4.0/src/keypact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-29 17:19:52.000000 keypact-0.4.0/src/keypact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:19:52.000000 keypact-0.4.0/src/keypact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-29 17:19:52.000000 keypact-0.4.0/src/keypact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:19:52.000000 keypact-0.4.0/src/keypact.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 17:19:52.000000 keypact-0.4.0/src/keypact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 17:19:52.000000 keypact-0.4.0/src/keypact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:53.915442 keypact-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-31 14:56:44.000000 keypact-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-31 14:56:53.915442 keypact-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-31 14:56:44.000000 keypact-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:56:53.915442 keypact-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-31 14:56:44.000000 keypact-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:53.911441 keypact-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:53.911441 keypact-0.5.0/src/keypact/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 14:56:44.000000 keypact-0.5.0/src/keypact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-31 14:56:44.000000 keypact-0.5.0/src/keypact/keypact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:56:53.915442 keypact-0.5.0/src/keypact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-31 14:56:53.000000 keypact-0.5.0/src/keypact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-31 14:56:53.000000 keypact-0.5.0/src/keypact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:56:53.000000 keypact-0.5.0/src/keypact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-31 14:56:53.000000 keypact-0.5.0/src/keypact.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:56:53.000000 keypact-0.5.0/src/keypact.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 14:56:53.000000 keypact-0.5.0/src/keypact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 14:56:53.000000 keypact-0.5.0/src/keypact.egg-info/top_level.txt
```

### Comparing `keypact-0.4.0/LICENSE` & `keypact-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keypact-0.4.0/PKG-INFO` & `keypact-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.4.0
+Version: 0.5.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded.
```

### Comparing `keypact-0.4.0/README.md` & `keypact-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `keypact-0.4.0/setup.py` & `keypact-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='keypact',
-version='0.4.0',
+version='0.5.0',
 description="""Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing""",
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 long_description_content_type='text/markdown',
 url='https://github.com/onuratakan/KeyPact',
 author='Onur Atakan ULUSOY',
 author_email='atadogan06@gmail.com',
 license='MIT',
```

### Comparing `keypact-0.4.0/src/keypact/keypact.py` & `keypact-0.5.0/src/keypact/keypact.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,18 @@
             os.remove(os.path.join(self.location, self.get_file(key)))
         except OSError:
             pass
 
         self.delete(key)
         
 
+    def delete_all(self):
+        for key in self.dict():
+            self.delete(key)
+
     def dict(self):
         result ={}
         for key in os.listdir(self.location):
             the_key = self.get_key(key)
             if not the_key is None:
                 if the_key != False:
                     result_of_key = self.get(the_key)
```

### Comparing `keypact-0.4.0/src/keypact.egg-info/PKG-INFO` & `keypact-0.5.0/src/keypact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keypact
-Version: 0.4.0
+Version: 0.5.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KeyPact
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KeyPact | Multithreaded Simultaneous Writing Key-Value DB
         KeyPact is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded.
```

