# Comparing `tmp/transkribus-client-0.3.3rc1.tar.gz` & `tmp/transkribus-client-0.3.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transkribus-client-0.3.3rc1.tar", last modified: Mon Jun 13 14:55:29 2022, max compression
+gzip compressed data, was "transkribus-client-0.3.4rc1.tar", last modified: Wed May 31 07:02:18 2023, max compression
```

## Comparing `transkribus-client-0.3.3rc1.tar` & `transkribus-client-0.3.4rc1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 14:55:29.000000 transkribus-client-0.3.3rc1/
--rw-rw-rw-   0 root         (0) root         (0)     1063 2022-06-13 14:54:33.000000 transkribus-client-0.3.3rc1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       42 2022-06-13 14:54:33.000000 transkribus-client-0.3.3rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3528 2022-06-13 14:55:29.000000 transkribus-client-0.3.3rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2504 2022-06-13 14:54:33.000000 transkribus-client-0.3.3rc1/README.md
--rw-rw-rw-   0 root         (0) root         (0)       10 2022-06-13 14:54:33.000000 transkribus-client-0.3.3rc1/VERSION
--rw-rw-rw-   0 root         (0) root         (0)       53 2022-06-13 14:54:33.000000 transkribus-client-0.3.3rc1/requirements-tests.txt
--rw-rw-rw-   0 root         (0) root         (0)       45 2022-06-13 14:54:33.000000 transkribus-client-0.3.3rc1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      111 2022-06-13 14:55:29.000000 transkribus-client-0.3.3rc1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1504 2022-06-13 14:54:33.000000 transkribus-client-0.3.3rc1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 14:55:29.000000 transkribus-client-0.3.3rc1/transkribus/
--rw-rw-rw-   0 root         (0) root         (0)       99 2022-06-13 14:54:33.000000 transkribus-client-0.3.3rc1/transkribus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4209 2022-06-13 14:54:33.000000 transkribus-client-0.3.3rc1/transkribus/api.py
--rw-rw-rw-   0 root         (0) root         (0)     7946 2022-06-13 14:54:33.000000 transkribus-client-0.3.3rc1/transkribus/models.py
--rw-rw-rw-   0 root         (0) root         (0)     7009 2022-06-13 14:54:33.000000 transkribus-client-0.3.3rc1/transkribus/pagexml.py
--rw-rw-rw-   0 root         (0) root         (0)      889 2022-06-13 14:54:33.000000 transkribus-client-0.3.3rc1/transkribus/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2598 2022-06-13 14:54:33.000000 transkribus-client-0.3.3rc1/transkribus/xml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-13 14:55:29.000000 transkribus-client-0.3.3rc1/transkribus_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3528 2022-06-13 14:55:29.000000 transkribus-client-0.3.3rc1/transkribus_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2022-06-13 14:55:29.000000 transkribus-client-0.3.3rc1/transkribus_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-13 14:55:29.000000 transkribus-client-0.3.3rc1/transkribus_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2022-06-13 14:55:29.000000 transkribus-client-0.3.3rc1/transkribus_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-06-13 14:55:29.000000 transkribus-client-0.3.3rc1/transkribus_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:02:18.582862 transkribus-client-0.3.4rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2023-05-31 06:56:13.000000 transkribus-client-0.3.4rc1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-05-31 06:56:13.000000 transkribus-client-0.3.4rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3535 2023-05-31 07:02:18.582862 transkribus-client-0.3.4rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2504 2023-05-31 06:56:13.000000 transkribus-client-0.3.4rc1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-05-31 07:02:10.000000 transkribus-client-0.3.4rc1/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-05-31 06:56:13.000000 transkribus-client-0.3.4rc1/requirements-tests.txt
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-05-31 07:02:10.000000 transkribus-client-0.3.4rc1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-05-31 07:02:18.582862 transkribus-client-0.3.4rc1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1511 2023-05-31 06:56:13.000000 transkribus-client-0.3.4rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:02:18.578862 transkribus-client-0.3.4rc1/transkribus/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-05-31 06:56:13.000000 transkribus-client-0.3.4rc1/transkribus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4209 2023-05-31 06:56:13.000000 transkribus-client-0.3.4rc1/transkribus/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     7946 2023-05-31 06:56:13.000000 transkribus-client-0.3.4rc1/transkribus/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     7009 2023-05-31 06:56:13.000000 transkribus-client-0.3.4rc1/transkribus/pagexml.py
+-rw-rw-rw-   0 root         (0) root         (0)      889 2023-05-31 06:56:13.000000 transkribus-client-0.3.4rc1/transkribus/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2598 2023-05-31 06:56:13.000000 transkribus-client-0.3.4rc1/transkribus/xml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:02:18.582862 transkribus-client-0.3.4rc1/transkribus_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3535 2023-05-31 07:02:18.000000 transkribus-client-0.3.4rc1/transkribus_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 07:02:18.000000 transkribus-client-0.3.4rc1/transkribus_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 07:02:18.000000 transkribus-client-0.3.4rc1/transkribus_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-31 07:02:18.000000 transkribus-client-0.3.4rc1/transkribus_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-31 07:02:18.000000 transkribus-client-0.3.4rc1/transkribus_client.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `transkribus-client-0.3.3rc1/LICENSE` & `transkribus-client-0.3.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `transkribus-client-0.3.3rc1/PKG-INFO` & `transkribus-client-0.3.4rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: transkribus-client
-Version: 0.3.3rc1
+Version: 0.3.4rc1
 Summary: Unofficial API client for the Transkribus project
-Home-page: https://gitlab.com/arkindex/transkribus
+Home-page: https://gitlab.com/teklia/arkindex/transkribus
 Author: Teklia <contact@teklia.com>
 License: MIT
 Keywords: api client transkribus
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Transkribus API Client
 
 `transkribus-client` provides a Python 3.6+ API client to interact with Transkribus.
```

### Comparing `transkribus-client-0.3.3rc1/README.md` & `transkribus-client-0.3.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `transkribus-client-0.3.3rc1/setup.py` & `transkribus-client-0.3.4rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,21 @@
     packages=find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests"],
     ),
     package_data={
         "": ["README.md", "LICENSE"],
     },
     install_requires=read_requirements("requirements.txt"),
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     license="MIT",
     description="Unofficial API client for the Transkribus project",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     keywords="api client transkribus",
-    url="https://gitlab.com/arkindex/transkribus",
+    url="https://gitlab.com/teklia/arkindex/transkribus",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
```

### Comparing `transkribus-client-0.3.3rc1/transkribus/api.py` & `transkribus-client-0.3.4rc1/transkribus/api.py`

 * *Files identical despite different names*

### Comparing `transkribus-client-0.3.3rc1/transkribus/models.py` & `transkribus-client-0.3.4rc1/transkribus/models.py`

 * *Files identical despite different names*

### Comparing `transkribus-client-0.3.3rc1/transkribus/pagexml.py` & `transkribus-client-0.3.4rc1/transkribus/pagexml.py`

 * *Files identical despite different names*

### Comparing `transkribus-client-0.3.3rc1/transkribus/utils.py` & `transkribus-client-0.3.4rc1/transkribus/utils.py`

 * *Files identical despite different names*

### Comparing `transkribus-client-0.3.3rc1/transkribus/xml.py` & `transkribus-client-0.3.4rc1/transkribus/xml.py`

 * *Files identical despite different names*

### Comparing `transkribus-client-0.3.3rc1/transkribus_client.egg-info/PKG-INFO` & `transkribus-client-0.3.4rc1/transkribus_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: transkribus-client
-Version: 0.3.3rc1
+Version: 0.3.4rc1
 Summary: Unofficial API client for the Transkribus project
-Home-page: https://gitlab.com/arkindex/transkribus
+Home-page: https://gitlab.com/teklia/arkindex/transkribus
 Author: Teklia <contact@teklia.com>
 License: MIT
 Keywords: api client transkribus
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Science/Research
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Transkribus API Client
 
 `transkribus-client` provides a Python 3.6+ API client to interact with Transkribus.
```

