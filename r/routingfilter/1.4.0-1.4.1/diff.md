# Comparing `tmp/routingfilter-1.4.0.tar.gz` & `tmp/routingfilter-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routingfilter-1.4.0.tar", last modified: Wed May 24 09:28:05 2023, max compression
+gzip compressed data, was "routingfilter-1.4.1.tar", last modified: Wed May 31 09:00:58 2023, max compression
```

## Comparing `routingfilter-1.4.0.tar` & `routingfilter-1.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:28:05.952541 routingfilter-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-24 09:27:55.000000 routingfilter-1.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:27:55.000000 routingfilter-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-24 09:28:05.952541 routingfilter-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-24 09:27:55.000000 routingfilter-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-24 09:27:55.000000 routingfilter-1.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:28:05.948541 routingfilter-1.4.0/routingfilter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:27:55.000000 routingfilter-1.4.0/routingfilter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-05-24 09:27:55.000000 routingfilter-1.4.0/routingfilter/configfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-24 09:27:55.000000 routingfilter-1.4.0/routingfilter/dictquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-05-24 09:27:55.000000 routingfilter-1.4.0/routingfilter/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-05-24 09:27:55.000000 routingfilter-1.4.0/routingfilter/routing_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:28:05.952541 routingfilter-1.4.0/routingfilter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-24 09:28:05.000000 routingfilter-1.4.0/routingfilter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-24 09:28:05.000000 routingfilter-1.4.0/routingfilter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:28:05.000000 routingfilter-1.4.0/routingfilter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-24 09:28:05.000000 routingfilter-1.4.0/routingfilter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-24 09:28:05.000000 routingfilter-1.4.0/routingfilter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:28:05.952541 routingfilter-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-24 09:27:55.000000 routingfilter-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:58.764170 routingfilter-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-31 09:00:43.000000 routingfilter-1.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:00:43.000000 routingfilter-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-31 09:00:58.764170 routingfilter-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-31 09:00:43.000000 routingfilter-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 09:00:43.000000 routingfilter-1.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:58.764170 routingfilter-1.4.1/routingfilter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:43.000000 routingfilter-1.4.1/routingfilter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-05-31 09:00:43.000000 routingfilter-1.4.1/routingfilter/configfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-31 09:00:43.000000 routingfilter-1.4.1/routingfilter/dictquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-05-31 09:00:43.000000 routingfilter-1.4.1/routingfilter/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-05-31 09:00:43.000000 routingfilter-1.4.1/routingfilter/routing_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:00:58.764170 routingfilter-1.4.1/routingfilter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-31 09:00:58.000000 routingfilter-1.4.1/routingfilter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-31 09:00:58.000000 routingfilter-1.4.1/routingfilter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:00:58.000000 routingfilter-1.4.1/routingfilter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 09:00:58.000000 routingfilter-1.4.1/routingfilter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 09:00:58.000000 routingfilter-1.4.1/routingfilter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:00:58.764170 routingfilter-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-31 09:00:43.000000 routingfilter-1.4.1/setup.py
```

### Comparing `routingfilter-1.4.0/LICENSE.txt` & `routingfilter-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingfilter-1.4.0/PKG-INFO` & `routingfilter-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routingfilter
-Version: 1.4.0
+Version: 1.4.1
 Summary: Generic Business Logic Implementation for Routing objects as python dictionaries
 Home-page: https://github.com/certego/RoutingFilter
 Author: Certego S.r.l.
 Author-email: support@certego.net
 License: GNU LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `routingfilter-1.4.0/routingfilter/configfilter.py` & `routingfilter-1.4.1/routingfilter/configfilter.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.4.0/routingfilter/dictquery.py` & `routingfilter-1.4.1/routingfilter/dictquery.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.4.0/routingfilter/routing.py` & `routingfilter-1.4.1/routingfilter/routing.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.4.0/routingfilter/routing_test.py` & `routingfilter-1.4.1/routingfilter/routing_test.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.4.0/routingfilter.egg-info/PKG-INFO` & `routingfilter-1.4.1/routingfilter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routingfilter
-Version: 1.4.0
+Version: 1.4.1
 Summary: Generic Business Logic Implementation for Routing objects as python dictionaries
 Home-page: https://github.com/certego/RoutingFilter
 Author: Certego S.r.l.
 Author-email: support@certego.net
 License: GNU LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `routingfilter-1.4.0/setup.py` & `routingfilter-1.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 with open("README.md", "r") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='routingfilter',
-    version='1.4.0',
+    version='1.4.1',
     packages=['routingfilter'],
     include_package_data=True,
-    install_requires=["IPy"],
+    install_requires=["IPy~=1.1", "macaddress~=2.0.2"],
     url='https://github.com/certego/RoutingFilter',
     license='GNU LGPLv3',
     author='Certego S.r.l.',
     author_email='support@certego.net',
     description='Generic Business Logic Implementation for Routing objects as python dictionaries',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

