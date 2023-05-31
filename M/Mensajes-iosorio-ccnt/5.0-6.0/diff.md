# Comparing `tmp/Mensajes-iosorio_ccnt-5.0.tar.gz` & `tmp/Mensajes-iosorio_ccnt-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mensajes-iosorio_ccnt-5.0.tar", last modified: Wed May 31 16:42:32 2023, max compression
+gzip compressed data, was "Mensajes-iosorio_ccnt-6.0.tar", last modified: Wed May 31 16:48:50 2023, max compression
```

## Comparing `Mensajes-iosorio_ccnt-5.0.tar` & `Mensajes-iosorio_ccnt-6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 16:42:32.866132 Mensajes-iosorio_ccnt-5.0/
--rw-rw-rw-   0        0        0     1056 2023-05-31 16:13:55.000000 Mensajes-iosorio_ccnt-5.0/LICENSE
--rw-rw-rw-   0        0        0       60 2023-05-31 16:14:15.000000 Mensajes-iosorio_ccnt-5.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-31 16:42:32.844693 Mensajes-iosorio_ccnt-5.0/Mensajes_iosorio_ccnt.egg-info/
--rw-rw-rw-   0        0        0      700 2023-05-31 16:42:32.000000 Mensajes-iosorio_ccnt-5.0/Mensajes_iosorio_ccnt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2023-05-31 16:42:32.000000 Mensajes-iosorio_ccnt-5.0/Mensajes_iosorio_ccnt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 16:42:32.000000 Mensajes-iosorio_ccnt-5.0/Mensajes_iosorio_ccnt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-31 16:42:32.000000 Mensajes-iosorio_ccnt-5.0/Mensajes_iosorio_ccnt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-31 16:42:32.000000 Mensajes-iosorio_ccnt-5.0/Mensajes_iosorio_ccnt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      700 2023-05-31 16:42:32.865135 Mensajes-iosorio_ccnt-5.0/PKG-INFO
--rw-rw-rw-   0        0        0       66 2023-05-31 16:09:31.000000 Mensajes-iosorio_ccnt-5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 16:42:32.847684 Mensajes-iosorio_ccnt-5.0/mensajes/
--rw-rw-rw-   0        0        0       38 2023-05-26 22:58:28.000000 Mensajes-iosorio_ccnt-5.0/mensajes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 16:42:32.850674 Mensajes-iosorio_ccnt-5.0/mensajes/adios/
--rw-rw-rw-   0        0        0       47 2023-05-26 22:58:29.000000 Mensajes-iosorio_ccnt-5.0/mensajes/adios/__init__.py
--rw-rw-rw-   0        0        0      182 2023-05-26 22:58:29.000000 Mensajes-iosorio_ccnt-5.0/mensajes/adios/despedidas.py
-drwxrwxrwx   0        0        0        0 2023-05-31 16:42:32.857208 Mensajes-iosorio_ccnt-5.0/mensajes/hola/
--rw-rw-rw-   0        0        0       46 2023-05-26 22:58:29.000000 Mensajes-iosorio_ccnt-5.0/mensajes/hola/__init__.py
--rw-rw-rw-   0        0        0      373 2023-05-26 22:58:29.000000 Mensajes-iosorio_ccnt-5.0/mensajes/hola/saludos.py
--rw-rw-rw-   0        0        0       13 2023-05-26 22:58:28.000000 Mensajes-iosorio_ccnt-5.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 16:42:32.867129 Mensajes-iosorio_ccnt-5.0/setup.cfg
--rw-rw-rw-   0        0        0      949 2023-05-31 16:42:16.000000 Mensajes-iosorio_ccnt-5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 16:42:32.862682 Mensajes-iosorio_ccnt-5.0/tests/
--rw-rw-rw-   0        0        0        0 2023-05-26 22:58:28.000000 Mensajes-iosorio_ccnt-5.0/tests/__init__.py
--rw-rw-rw-   0        0        0      268 2023-05-26 22:58:28.000000 Mensajes-iosorio_ccnt-5.0/tests/test_hola.py
+drwxrwxrwx   0        0        0        0 2023-05-31 16:48:50.746887 Mensajes-iosorio_ccnt-6.0/
+-rw-rw-rw-   0        0        0     1056 2023-05-31 16:13:55.000000 Mensajes-iosorio_ccnt-6.0/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-05-31 16:14:15.000000 Mensajes-iosorio_ccnt-6.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-31 16:48:50.716641 Mensajes-iosorio_ccnt-6.0/Mensajes_iosorio_ccnt.egg-info/
+-rw-rw-rw-   0        0        0      700 2023-05-31 16:48:50.000000 Mensajes-iosorio_ccnt-6.0/Mensajes_iosorio_ccnt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2023-05-31 16:48:50.000000 Mensajes-iosorio_ccnt-6.0/Mensajes_iosorio_ccnt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 16:48:50.000000 Mensajes-iosorio_ccnt-6.0/Mensajes_iosorio_ccnt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-31 16:48:50.000000 Mensajes-iosorio_ccnt-6.0/Mensajes_iosorio_ccnt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-31 16:48:50.000000 Mensajes-iosorio_ccnt-6.0/Mensajes_iosorio_ccnt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      700 2023-05-31 16:48:50.745890 Mensajes-iosorio_ccnt-6.0/PKG-INFO
+-rw-rw-rw-   0        0        0       66 2023-05-31 16:09:31.000000 Mensajes-iosorio_ccnt-6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 16:48:50.720409 Mensajes-iosorio_ccnt-6.0/mensajes/
+-rw-rw-rw-   0        0        0       38 2023-05-26 22:58:28.000000 Mensajes-iosorio_ccnt-6.0/mensajes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 16:48:50.730402 Mensajes-iosorio_ccnt-6.0/mensajes/adios/
+-rw-rw-rw-   0        0        0       47 2023-05-26 22:58:29.000000 Mensajes-iosorio_ccnt-6.0/mensajes/adios/__init__.py
+-rw-rw-rw-   0        0        0      182 2023-05-26 22:58:29.000000 Mensajes-iosorio_ccnt-6.0/mensajes/adios/despedidas.py
+drwxrwxrwx   0        0        0        0 2023-05-31 16:48:50.736407 Mensajes-iosorio_ccnt-6.0/mensajes/hola/
+-rw-rw-rw-   0        0        0       46 2023-05-26 22:58:29.000000 Mensajes-iosorio_ccnt-6.0/mensajes/hola/__init__.py
+-rw-rw-rw-   0        0        0      375 2023-05-31 16:48:04.000000 Mensajes-iosorio_ccnt-6.0/mensajes/hola/saludos.py
+-rw-rw-rw-   0        0        0       13 2023-05-26 22:58:28.000000 Mensajes-iosorio_ccnt-6.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 16:48:50.746887 Mensajes-iosorio_ccnt-6.0/setup.cfg
+-rw-rw-rw-   0        0        0      949 2023-05-31 16:48:13.000000 Mensajes-iosorio_ccnt-6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 16:48:50.743895 Mensajes-iosorio_ccnt-6.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-26 22:58:28.000000 Mensajes-iosorio_ccnt-6.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      268 2023-05-26 22:58:28.000000 Mensajes-iosorio_ccnt-6.0/tests/test_hola.py
```

### Comparing `Mensajes-iosorio_ccnt-5.0/LICENSE` & `Mensajes-iosorio_ccnt-6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Mensajes-iosorio_ccnt-5.0/Mensajes_iosorio_ccnt.egg-info/PKG-INFO` & `Mensajes-iosorio_ccnt-6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Mensajes-iosorio-ccnt
-Version: 5.0
+Name: Mensajes-iosorio_ccnt
+Version: 6.0
 Summary: Un paquete para saludar y despedir
 Home-page: https://www.ccn.mx
 Author: Ivan Osorio
 Author-email: iosorio@ccn.mx
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `Mensajes-iosorio_ccnt-5.0/PKG-INFO` & `Mensajes-iosorio_ccnt-6.0/Mensajes_iosorio_ccnt.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Mensajes-iosorio_ccnt
-Version: 5.0
+Name: Mensajes-iosorio-ccnt
+Version: 6.0
 Summary: Un paquete para saludar y despedir
 Home-page: https://www.ccn.mx
 Author: Ivan Osorio
 Author-email: iosorio@ccn.mx
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `Mensajes-iosorio_ccnt-5.0/setup.py` & `Mensajes-iosorio_ccnt-6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Mensajes-iosorio_ccnt',
-    version='5.0',
+    version='6.0',
     description='Un paquete para saludar y despedir',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Ivan Osorio',
     author_email='iosorio@ccn.mx',
     url='https://www.ccn.mx',
     license_files=['LICENSE'],
```

