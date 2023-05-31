# Comparing `tmp/gravitas-0.1.4.tar.gz` & `tmp/gravitas-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitas-0.1.4.tar", last modified: Wed May 31 04:50:10 2023, max compression
+gzip compressed data, was "gravitas-0.1.5.tar", last modified: Wed May 31 05:21:09 2023, max compression
```

## Comparing `gravitas-0.1.4.tar` & `gravitas-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:50:10.700694 gravitas-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-31 04:50:10.700694 gravitas-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-31 04:49:59.000000 gravitas-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:50:10.696694 gravitas-0.1.4/gravitas/
--rw-r--r--   0 runner    (1001) docker     (123)  2750335 2023-05-31 04:49:59.000000 gravitas-0.1.4/gravitas/EGM96.c
--rw-r--r--   0 runner    (1001) docker     (123)  2750581 2023-05-31 04:49:59.000000 gravitas-0.1.4/gravitas/GRGM360.c
--rw-r--r--   0 runner    (1001) docker     (123)   300782 2023-05-31 04:49:59.000000 gravitas-0.1.4/gravitas/MRO120F.c
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-31 04:49:59.000000 gravitas-0.1.4/gravitas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-05-31 04:49:59.000000 gravitas-0.1.4/gravitas/gravlib.c
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-31 04:49:59.000000 gravitas-0.1.4/gravitas/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-31 04:49:59.000000 gravitas-0.1.4/gravitas/libgrav.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:50:10.700694 gravitas-0.1.4/gravitas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-31 04:50:10.000000 gravitas-0.1.4/gravitas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-31 04:50:10.000000 gravitas-0.1.4/gravitas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:50:10.000000 gravitas-0.1.4/gravitas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:50:10.000000 gravitas-0.1.4/gravitas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 04:50:10.000000 gravitas-0.1.4/gravitas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 04:50:10.000000 gravitas-0.1.4/gravitas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-31 04:49:59.000000 gravitas-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 04:50:10.700694 gravitas-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-31 04:49:59.000000 gravitas-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:21:09.759637 gravitas-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-31 05:21:09.759637 gravitas-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-31 05:20:58.000000 gravitas-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:21:09.755638 gravitas-0.1.5/gravitas/
+-rw-r--r--   0 runner    (1001) docker     (123)  2750335 2023-05-31 05:20:58.000000 gravitas-0.1.5/gravitas/EGM96.c
+-rw-r--r--   0 runner    (1001) docker     (123)  2750581 2023-05-31 05:20:58.000000 gravitas-0.1.5/gravitas/GRGM360.c
+-rw-r--r--   0 runner    (1001) docker     (123)   300782 2023-05-31 05:20:58.000000 gravitas-0.1.5/gravitas/MRO120F.c
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-31 05:20:58.000000 gravitas-0.1.5/gravitas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-05-31 05:20:58.000000 gravitas-0.1.5/gravitas/gravlib.c
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-31 05:20:58.000000 gravitas-0.1.5/gravitas/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-31 05:20:58.000000 gravitas-0.1.5/gravitas/libgrav.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:21:09.759637 gravitas-0.1.5/gravitas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-31 05:21:09.000000 gravitas-0.1.5/gravitas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-31 05:21:09.000000 gravitas-0.1.5/gravitas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 05:21:09.000000 gravitas-0.1.5/gravitas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 05:21:09.000000 gravitas-0.1.5/gravitas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 05:21:09.000000 gravitas-0.1.5/gravitas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 05:21:09.000000 gravitas-0.1.5/gravitas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-31 05:20:58.000000 gravitas-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 05:21:09.759637 gravitas-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-31 05:20:58.000000 gravitas-0.1.5/setup.py
```

### Comparing `gravitas-0.1.4/PKG-INFO` & `gravitas-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravitas
-Version: 0.1.4
+Version: 0.1.5
 Author: Liam Robinson
 Author-email: robin502@purdue.edu
 License: GPL-2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gravitas-0.1.4/gravitas/EGM96.c` & `gravitas-0.1.5/gravitas/EGM96.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.4/gravitas/GRGM360.c` & `gravitas-0.1.5/gravitas/GRGM360.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.4/gravitas/MRO120F.c` & `gravitas-0.1.5/gravitas/MRO120F.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.4/gravitas/__init__.py` & `gravitas-0.1.5/gravitas/__init__.py`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.4/gravitas/gravlib.c` & `gravitas-0.1.5/gravitas/gravlib.c`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
     for(m = 2; m < nmax+2; m++) {
         rm[m] = stu.x*rm[m-1] - stu.y*im[m-1]; 
         im[m] = stu.x*im[m-1] + stu.y*rm[m-1];
     }
     double rho  = mu/(req*rmag);
     double rhop = req/rmag;
     double g1 = 0.00; double g2 = 0.00; double g3 = 0.00; double g4 = 0.00;
-    for (int n = 0; n <= nmax; n++) {
+    for(n = 0; n <= nmax; n++) {
         double g1t = 0.0; double g2t = 0.0; double g3t = 0.0; double g4t = 0.0;
         double sm = 0.5;
         int m;
         for(m = 0; m <= n; m++) {
             double anmp1;
             if(n == m) {
                 anmp1 = 0.0;
```

### Comparing `gravitas-0.1.4/gravitas/lib.py` & `gravitas-0.1.5/gravitas/lib.py`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.4/gravitas/libgrav.h` & `gravitas-0.1.5/gravitas/libgrav.h`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.4/gravitas.egg-info/PKG-INFO` & `gravitas-0.1.5/gravitas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravitas
-Version: 0.1.4
+Version: 0.1.5
 Author: Liam Robinson
 Author-email: robin502@purdue.edu
 License: GPL-2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gravitas-0.1.4/pyproject.toml` & `gravitas-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.4/setup.py` & `gravitas-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         #     if self.compiler.compiler_type == 'msvc':
         #         ext.extra_compile_args.append('/std:c90')
         super().build_extensions()
 
 # _LIB_DIR
 setup(
     name='gravitas',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     license='GPL-2',
     long_description="""High-fidelity gravity fields for satellite propagation""",
     long_description_content_type='text/markdown',
     author="Liam Robinson",
     author_email="robin502@purdue.edu",
     install_requires=['numpy'],
```

