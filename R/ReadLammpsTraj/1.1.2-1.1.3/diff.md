# Comparing `tmp/ReadLammpsTraj-1.1.2.tar.gz` & `tmp/ReadLammpsTraj-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReadLammpsTraj-1.1.2.tar", last modified: Wed May 31 14:20:58 2023, max compression
+gzip compressed data, was "ReadLammpsTraj-1.1.3.tar", last modified: Wed May 31 14:30:21 2023, max compression
```

## Comparing `ReadLammpsTraj-1.1.2.tar` & `ReadLammpsTraj-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 14:20:58.891399 ReadLammpsTraj-1.1.2/
--rw-rw-rw-   0        0        0     1087 2023-05-31 03:57:12.000000 ReadLammpsTraj-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      106 2023-05-31 14:20:55.000000 ReadLammpsTraj-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2225 2023-05-31 14:20:58.891399 ReadLammpsTraj-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1936 2023-05-31 05:31:22.000000 ReadLammpsTraj-1.1.2/README.md
--rw-rw-rw-   0        0        0       30 2023-05-31 05:32:22.000000 ReadLammpsTraj-1.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 14:20:58.892399 ReadLammpsTraj-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      720 2023-05-31 14:20:07.000000 ReadLammpsTraj-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:20:58.878403 ReadLammpsTraj-1.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 14:20:58.888401 ReadLammpsTraj-1.1.2/src/ReadLammpsTraj.egg-info/
--rw-rw-rw-   0        0        0     2225 2023-05-31 14:20:58.000000 ReadLammpsTraj-1.1.2/src/ReadLammpsTraj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-05-31 14:20:58.000000 ReadLammpsTraj-1.1.2/src/ReadLammpsTraj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 14:20:58.000000 ReadLammpsTraj-1.1.2/src/ReadLammpsTraj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-31 14:20:58.000000 ReadLammpsTraj-1.1.2/src/ReadLammpsTraj.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-31 14:20:58.000000 ReadLammpsTraj-1.1.2/src/ReadLammpsTraj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10480 2023-05-31 14:19:00.000000 ReadLammpsTraj-1.1.2/src/ReadLammpsTraj.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:30:21.834541 ReadLammpsTraj-1.1.3/
+-rw-rw-rw-   0        0        0     1087 2023-05-31 03:57:12.000000 ReadLammpsTraj-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0      132 2023-05-31 14:29:01.000000 ReadLammpsTraj-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2225 2023-05-31 14:30:21.834541 ReadLammpsTraj-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1936 2023-05-31 05:31:22.000000 ReadLammpsTraj-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 14:30:21.817011 ReadLammpsTraj-1.1.3/demo/
+-rw-rw-rw-   0        0        0  2026571 2022-07-19 02:19:38.000000 ReadLammpsTraj-1.1.3/demo/1000.lammpstrj
+drwxrwxrwx   0        0        0        0 2023-05-31 14:30:21.820012 ReadLammpsTraj-1.1.3/demo/__pycache__/
+-rw-rw-rw-   0        0        0    15185 2023-05-31 05:24:15.000000 ReadLammpsTraj-1.1.3/demo/__pycache__/ReadLammpsTraj.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1966 2023-05-31 14:26:43.000000 ReadLammpsTraj-1.1.3/demo/cal_density.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:30:21.822010 ReadLammpsTraj-1.1.3/demo/imgs/
+-rw-rw-rw-   0        0        0   307101 2023-05-31 14:26:47.000000 ReadLammpsTraj-1.1.3/demo/imgs/density.png
+-rw-rw-rw-   0        0        0       30 2023-05-31 05:32:22.000000 ReadLammpsTraj-1.1.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 14:30:21.835538 ReadLammpsTraj-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      720 2023-05-31 14:30:12.000000 ReadLammpsTraj-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:30:21.824011 ReadLammpsTraj-1.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 14:30:21.832538 ReadLammpsTraj-1.1.3/src/ReadLammpsTraj.egg-info/
+-rw-rw-rw-   0        0        0     2225 2023-05-31 14:30:21.000000 ReadLammpsTraj-1.1.3/src/ReadLammpsTraj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-05-31 14:30:21.000000 ReadLammpsTraj-1.1.3/src/ReadLammpsTraj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 14:30:21.000000 ReadLammpsTraj-1.1.3/src/ReadLammpsTraj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-31 14:30:21.000000 ReadLammpsTraj-1.1.3/src/ReadLammpsTraj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-31 14:30:21.000000 ReadLammpsTraj-1.1.3/src/ReadLammpsTraj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10480 2023-05-31 14:19:00.000000 ReadLammpsTraj-1.1.3/src/ReadLammpsTraj.py
```

### Comparing `ReadLammpsTraj-1.1.2/LICENSE` & `ReadLammpsTraj-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ReadLammpsTraj-1.1.2/PKG-INFO` & `ReadLammpsTraj-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReadLammpsTraj
-Version: 1.1.2
+Version: 1.1.3
 Summary: Read lammps dump trajectory.
 Home-page: https://github.com/eastsheng/ReadLammpsTraj
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ReadLammpsTraj-1.1.2/README.md` & `ReadLammpsTraj-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ReadLammpsTraj-1.1.2/setup.py` & `ReadLammpsTraj-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
 
 
 setup(
 name         = 'ReadLammpsTraj',
-version      = '1.1.2',
+version      = '1.1.3',
 py_modules   = ['ReadLammpsTraj'],
 author       = 'CHENDONGSHENG',
 author_email = 'eastsheng@hotmail.com',
 packages=find_packages('src'),
 package_dir={'': 'src'},
 install_requires=required,
 url          = 'https://github.com/eastsheng/ReadLammpsTraj',
```

### Comparing `ReadLammpsTraj-1.1.2/src/ReadLammpsTraj.egg-info/PKG-INFO` & `ReadLammpsTraj-1.1.3/src/ReadLammpsTraj.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReadLammpsTraj
-Version: 1.1.2
+Version: 1.1.3
 Summary: Read lammps dump trajectory.
 Home-page: https://github.com/eastsheng/ReadLammpsTraj
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ReadLammpsTraj-1.1.2/src/ReadLammpsTraj.py` & `ReadLammpsTraj-1.1.3/src/ReadLammpsTraj.py`

 * *Files identical despite different names*

