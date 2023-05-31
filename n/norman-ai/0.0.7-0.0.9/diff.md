# Comparing `tmp/norman_ai-0.0.7.tar.gz` & `tmp/norman_ai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "norman_ai-0.0.7.tar", last modified: Sat May 27 20:04:22 2023, max compression
+gzip compressed data, was "norman_ai-0.0.9.tar", last modified: Wed May 31 10:37:40 2023, max compression
```

## Comparing `norman_ai-0.0.7.tar` & `norman_ai-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 20:04:22.122078 norman_ai-0.0.7/
--rw-rw-rw-   0        0        0     7818 2023-05-16 12:28:05.000000 norman_ai-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0       43 2023-05-16 12:28:05.000000 norman_ai-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0    31934 2023-05-27 20:04:22.122583 norman_ai-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    31421 2023-05-27 19:58:41.000000 norman_ai-0.0.7/README.md
--rw-rw-rw-   0        0        0      108 2023-05-16 12:28:09.000000 norman_ai-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      688 2023-05-27 20:04:22.123725 norman_ai-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 20:04:22.093852 norman_ai-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 20:04:22.113648 norman_ai-0.0.7/src/norman_ai/
--rw-rw-rw-   0        0        0       28 2023-05-23 14:39:46.000000 norman_ai-0.0.7/src/norman_ai/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 20:04:22.119990 norman_ai-0.0.7/src/norman_ai/data/
--rw-rw-rw-   0        0        0    31392 2023-05-16 12:28:09.000000 norman_ai-0.0.7/src/norman_ai/data/norman_model1.h5
--rw-rw-rw-   0        0        0    54035 2023-05-27 20:00:01.000000 norman_ai-0.0.7/src/norman_ai/norman_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-27 20:04:22.118990 norman_ai-0.0.7/src/norman_ai.egg-info/
--rw-rw-rw-   0        0        0    31934 2023-05-27 20:04:22.000000 norman_ai-0.0.7/src/norman_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-05-27 20:04:22.000000 norman_ai-0.0.7/src/norman_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 20:04:22.000000 norman_ai-0.0.7/src/norman_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-27 20:04:22.000000 norman_ai-0.0.7/src/norman_ai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 10:37:40.019447 norman_ai-0.0.9/
+-rw-rw-rw-   0        0        0     7818 2023-05-16 12:28:05.000000 norman_ai-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       43 2023-05-16 12:28:05.000000 norman_ai-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    31935 2023-05-31 10:37:40.019951 norman_ai-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    31422 2023-05-31 10:26:05.000000 norman_ai-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-16 12:28:09.000000 norman_ai-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      688 2023-05-31 10:37:40.020998 norman_ai-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 10:37:39.998869 norman_ai-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 10:37:40.014629 norman_ai-0.0.9/src/norman_ai/
+-rw-rw-rw-   0        0        0        0 2023-05-31 10:36:40.000000 norman_ai-0.0.9/src/norman_ai/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:37:40.018113 norman_ai-0.0.9/src/norman_ai/data/
+-rw-rw-rw-   0        0        0    31392 2023-05-16 12:28:09.000000 norman_ai-0.0.9/src/norman_ai/data/norman_model1.h5
+-rw-rw-rw-   0        0        0    54035 2023-05-27 20:00:01.000000 norman_ai-0.0.9/src/norman_ai/norman_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:37:40.018113 norman_ai-0.0.9/src/norman_ai.egg-info/
+-rw-rw-rw-   0        0        0    31935 2023-05-31 10:37:39.000000 norman_ai-0.0.9/src/norman_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-31 10:37:39.000000 norman_ai-0.0.9/src/norman_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 10:37:39.000000 norman_ai-0.0.9/src/norman_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-31 10:37:39.000000 norman_ai-0.0.9/src/norman_ai.egg-info/top_level.txt
```

### Comparing `norman_ai-0.0.7/LICENSE.txt` & `norman_ai-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `norman_ai-0.0.7/PKG-INFO` & `norman_ai-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: norman_ai
-Version: 0.0.7
+Version: 0.0.9
 Summary: A package for automation of the novel object recognition test.
 Home-page: https://github.com/Seyij/norman
 Author: seyij_p
 Author-email: seyi.ooj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -98,15 +98,16 @@
 ```bash
 #open the ipython program
 ipython
 ```
 ```python
 #check if your graphics card is recognised by tensorflow after installation
 
-import tensorflow as tfprint("Num GPUs Available: ", len(tf.config.list_physical_devices("GPU")))
+import tensorflow as tf
+print("Num GPUs Available: ", len(tf.config.list_physical_devices("GPU")))
 
 #check if norman was installed
 import norman_ai.norman_functions as nf
 nf.run_gui()
 #a user interface should appear
 ```
```

### Comparing `norman_ai-0.0.7/README.md` & `norman_ai-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,16 @@
 ```bash
 #open the ipython program
 ipython
 ```
 ```python
 #check if your graphics card is recognised by tensorflow after installation
 
-import tensorflow as tfprint("Num GPUs Available: ", len(tf.config.list_physical_devices("GPU")))
+import tensorflow as tf
+print("Num GPUs Available: ", len(tf.config.list_physical_devices("GPU")))
 
 #check if norman was installed
 import norman_ai.norman_functions as nf
 nf.run_gui()
 #a user interface should appear
 ```
```

### Comparing `norman_ai-0.0.7/setup.cfg` & `norman_ai-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6f72 6d61 6e5f 6169 0d0a 7665   = norman_ai..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 370d 0a61  rsion = 0.0.7..a
+00000020: 7273 696f 6e20 3d20 302e 302e 390d 0a61  rsion = 0.0.9..a
 00000030: 7574 686f 7220 3d20 7365 7969 6a5f 700d  uthor = seyij_p.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 7365 7969 2e6f 6f6a 4067 6d61 696c 2e63  seyi.ooj@gmail.c
 00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000070: 3d20 4120 7061 636b 6167 6520 666f 7220  = A package for 
 00000080: 6175 746f 6d61 7469 6f6e 206f 6620 7468  automation of th
 00000090: 6520 6e6f 7665 6c20 6f62 6a65 6374 2072  e novel object r
```

### Comparing `norman_ai-0.0.7/src/norman_ai/data/norman_model1.h5` & `norman_ai-0.0.9/src/norman_ai/data/norman_model1.h5`

 * *Files identical despite different names*

### Comparing `norman_ai-0.0.7/src/norman_ai/norman_functions.py` & `norman_ai-0.0.9/src/norman_ai/norman_functions.py`

 * *Files identical despite different names*

### Comparing `norman_ai-0.0.7/src/norman_ai.egg-info/PKG-INFO` & `norman_ai-0.0.9/src/norman_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: norman-ai
-Version: 0.0.7
+Version: 0.0.9
 Summary: A package for automation of the novel object recognition test.
 Home-page: https://github.com/Seyij/norman
 Author: seyij_p
 Author-email: seyi.ooj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -98,15 +98,16 @@
 ```bash
 #open the ipython program
 ipython
 ```
 ```python
 #check if your graphics card is recognised by tensorflow after installation
 
-import tensorflow as tfprint("Num GPUs Available: ", len(tf.config.list_physical_devices("GPU")))
+import tensorflow as tf
+print("Num GPUs Available: ", len(tf.config.list_physical_devices("GPU")))
 
 #check if norman was installed
 import norman_ai.norman_functions as nf
 nf.run_gui()
 #a user interface should appear
 ```
```

