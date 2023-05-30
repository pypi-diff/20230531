# Comparing `tmp/vector_vault-1.6.1.tar.gz` & `tmp/vector_vault-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.6.1.tar", last modified: Tue May 30 23:36:50 2023, max compression
+gzip compressed data, was "vector_vault-1.6.2.tar", last modified: Tue May 30 23:38:47 2023, max compression
```

## Comparing `vector_vault-1.6.1.tar` & `vector_vault-1.6.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-30 23:36:50.581714 vector_vault-1.6.1/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.6.1/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    21423 2023-05-30 23:36:50.581553 vector_vault-1.6.1/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    20698 2023-05-30 23:19:30.000000 vector_vault-1.6.1/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-30 23:36:50.581770 vector_vault-1.6.1/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-30 23:36:31.000000 vector_vault-1.6.1/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-30 23:36:50.578595 vector_vault-1.6.1/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    21423 2023-05-30 23:36:50.000000 vector_vault-1.6.1/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-05-30 23:36:50.000000 vector_vault-1.6.1/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-30 23:36:50.000000 vector_vault-1.6.1/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-30 23:36:50.000000 vector_vault-1.6.1/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-30 23:36:50.000000 vector_vault-1.6.1/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-30 23:36:50.581320 vector_vault-1.6.1/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      702 2023-05-24 19:36:19.000000 vector_vault-1.6.1/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6238 2023-05-28 06:54:07.000000 vector_vault-1.6.1/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3261 2023-05-30 23:18:26.000000 vector_vault-1.6.1/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1843 2023-05-30 20:06:58.000000 vector_vault-1.6.1/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.6.1/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1590 2023-05-30 23:36:22.000000 vector_vault-1.6.1/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.6.1/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    18189 2023-05-30 23:18:17.000000 vector_vault-1.6.1/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     4344 2023-05-30 21:10:57.000000 vector_vault-1.6.1/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.6.1/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-30 23:38:47.903531 vector_vault-1.6.2/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.6.2/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    21423 2023-05-30 23:38:47.903355 vector_vault-1.6.2/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    20698 2023-05-30 23:19:30.000000 vector_vault-1.6.2/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-30 23:38:47.903602 vector_vault-1.6.2/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-30 23:38:37.000000 vector_vault-1.6.2/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-30 23:38:47.899169 vector_vault-1.6.2/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    21423 2023-05-30 23:38:47.000000 vector_vault-1.6.2/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-05-30 23:38:47.000000 vector_vault-1.6.2/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-30 23:38:47.000000 vector_vault-1.6.2/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-30 23:38:47.000000 vector_vault-1.6.2/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-30 23:38:47.000000 vector_vault-1.6.2/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-30 23:38:47.902662 vector_vault-1.6.2/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.6.2/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6238 2023-05-28 06:54:07.000000 vector_vault-1.6.2/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3261 2023-05-30 23:18:26.000000 vector_vault-1.6.2/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1843 2023-05-30 20:06:58.000000 vector_vault-1.6.2/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.6.2/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1590 2023-05-30 23:36:22.000000 vector_vault-1.6.2/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.6.2/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    18189 2023-05-30 23:18:17.000000 vector_vault-1.6.2/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     4344 2023-05-30 21:10:57.000000 vector_vault-1.6.2/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.6.2/vectorvault/wrap.py
```

### Comparing `vector_vault-1.6.1/LICENSE` & `vector_vault-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.1/PKG-INFO` & `vector_vault-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.6.1
+Version: 1.6.2
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.6.1/README.md` & `vector_vault-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.1/setup.py` & `vector_vault-1.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.6.1",
+    version="1.6.2",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.6.1/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.6.2/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.6.1
+Version: 1.6.2
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.6.1/vectorvault/__init__.py` & `vector_vault-1.6.2/vectorvault/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # Dissemination of this information or reproduction of this material
 # is strictly forbidden unless prior written permission is obtained
 # from Vector Vault.
 
 from .vault import Vault
 from .download import download_url
 from .wrap import wrap
-from signup import register
+from .signup import register
```

### Comparing `vector_vault-1.6.1/vectorvault/ai.py` & `vector_vault-1.6.2/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.1/vectorvault/cloudmanager.py` & `vector_vault-1.6.2/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.1/vectorvault/creds.py` & `vector_vault-1.6.2/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.1/vectorvault/download.py` & `vector_vault-1.6.2/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.1/vectorvault/itemize.py` & `vector_vault-1.6.2/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.1/vectorvault/signup.py` & `vector_vault-1.6.2/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.1/vectorvault/vault.py` & `vector_vault-1.6.2/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.1/vectorvault/vecreq.py` & `vector_vault-1.6.2/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.6.1/vectorvault/wrap.py` & `vector_vault-1.6.2/vectorvault/wrap.py`

 * *Files identical despite different names*

