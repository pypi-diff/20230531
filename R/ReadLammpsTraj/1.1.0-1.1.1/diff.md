# Comparing `tmp/ReadLammpsTraj-1.1.0.tar.gz` & `tmp/ReadLammpsTraj-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReadLammpsTraj-1.1.0.tar", last modified: Wed May 31 05:36:11 2023, max compression
+gzip compressed data, was "ReadLammpsTraj-1.1.1.tar", last modified: Wed May 31 05:46:12 2023, max compression
```

## Comparing `ReadLammpsTraj-1.1.0.tar` & `ReadLammpsTraj-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 05:36:11.654779 ReadLammpsTraj-1.1.0/
--rw-rw-rw-   0        0        0     1087 2023-05-31 03:57:12.000000 ReadLammpsTraj-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       90 2023-05-31 05:35:57.000000 ReadLammpsTraj-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2225 2023-05-31 05:36:11.654779 ReadLammpsTraj-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1936 2023-05-31 05:31:22.000000 ReadLammpsTraj-1.1.0/README.md
--rw-rw-rw-   0        0        0       30 2023-05-31 05:32:22.000000 ReadLammpsTraj-1.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 05:36:11.654779 ReadLammpsTraj-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      750 2023-05-31 05:27:20.000000 ReadLammpsTraj-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:36:11.645261 ReadLammpsTraj-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 05:36:11.652258 ReadLammpsTraj-1.1.0/src/ReadLammpsTraj.egg-info/
--rw-rw-rw-   0        0        0     2225 2023-05-31 05:36:11.000000 ReadLammpsTraj-1.1.0/src/ReadLammpsTraj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-05-31 05:36:11.000000 ReadLammpsTraj-1.1.0/src/ReadLammpsTraj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 05:36:11.000000 ReadLammpsTraj-1.1.0/src/ReadLammpsTraj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-31 05:36:11.000000 ReadLammpsTraj-1.1.0/src/ReadLammpsTraj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8088 2023-05-31 05:24:13.000000 ReadLammpsTraj-1.1.0/src/ReadLammpsTraj.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:46:12.892638 ReadLammpsTraj-1.1.1/
+-rw-rw-rw-   0        0        0     1087 2023-05-31 03:57:12.000000 ReadLammpsTraj-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       90 2023-05-31 05:35:57.000000 ReadLammpsTraj-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2225 2023-05-31 05:46:12.887637 ReadLammpsTraj-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1936 2023-05-31 05:31:22.000000 ReadLammpsTraj-1.1.1/README.md
+-rw-rw-rw-   0        0        0       30 2023-05-31 05:32:22.000000 ReadLammpsTraj-1.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 05:46:12.892638 ReadLammpsTraj-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      720 2023-05-31 05:46:05.000000 ReadLammpsTraj-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:46:12.874637 ReadLammpsTraj-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 05:46:12.884637 ReadLammpsTraj-1.1.1/src/ReadLammpsTraj.egg-info/
+-rw-rw-rw-   0        0        0     2225 2023-05-31 05:46:12.000000 ReadLammpsTraj-1.1.1/src/ReadLammpsTraj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-05-31 05:46:12.000000 ReadLammpsTraj-1.1.1/src/ReadLammpsTraj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 05:46:12.000000 ReadLammpsTraj-1.1.1/src/ReadLammpsTraj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-31 05:46:12.000000 ReadLammpsTraj-1.1.1/src/ReadLammpsTraj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-31 05:46:12.000000 ReadLammpsTraj-1.1.1/src/ReadLammpsTraj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8088 2023-05-31 05:24:13.000000 ReadLammpsTraj-1.1.1/src/ReadLammpsTraj.py
```

### Comparing `ReadLammpsTraj-1.1.0/LICENSE` & `ReadLammpsTraj-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ReadLammpsTraj-1.1.0/PKG-INFO` & `ReadLammpsTraj-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReadLammpsTraj
-Version: 1.1.0
+Version: 1.1.1
 Summary: Read lammps dump trajectory.
 Home-page: https://github.com/eastsheng/ReadLammpsTraj
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ReadLammpsTraj-1.1.0/README.md` & `ReadLammpsTraj-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ReadLammpsTraj-1.1.0/setup.py` & `ReadLammpsTraj-1.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 """
 
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
-# with open("src/ReadLammpsTraj.egg-info/requires.txt","r") as f:
-#     required = f.read().splitlines()
+with open("requirements.txt","r") as f:
+    required = f.read().splitlines()
 
 
 setup(
 name         = 'ReadLammpsTraj',
-version      = '1.1.0',
+version      = '1.1.1',
 py_modules   = ['ReadLammpsTraj'],
 author       = 'CHENDONGSHENG',
 author_email = 'eastsheng@hotmail.com',
 packages=find_packages('src'),
 package_dir={'': 'src'},
-# install_requires=required,
+install_requires=required,
 url          = 'https://github.com/eastsheng/ReadLammpsTraj',
 description  = 'Read lammps dump trajectory.',
 long_description=long_description,
 long_description_content_type='text/markdown'
 )
```

### Comparing `ReadLammpsTraj-1.1.0/src/ReadLammpsTraj.egg-info/PKG-INFO` & `ReadLammpsTraj-1.1.1/src/ReadLammpsTraj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReadLammpsTraj
-Version: 1.1.0
+Version: 1.1.1
 Summary: Read lammps dump trajectory.
 Home-page: https://github.com/eastsheng/ReadLammpsTraj
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ReadLammpsTraj-1.1.0/src/ReadLammpsTraj.py` & `ReadLammpsTraj-1.1.1/src/ReadLammpsTraj.py`

 * *Files identical despite different names*

