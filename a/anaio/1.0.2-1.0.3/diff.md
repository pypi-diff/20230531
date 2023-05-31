# Comparing `tmp/anaio-1.0.2.tar.gz` & `tmp/anaio-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anaio-1.0.2.tar", last modified: Thu Mar  2 09:53:03 2023, max compression
+gzip compressed data, was "anaio-1.0.3.tar", last modified: Wed May 31 07:51:24 2023, max compression
```

## Comparing `anaio-1.0.2.tar` & `anaio-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 09:53:03.711463 anaio-1.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     1107 2023-03-02 09:50:22.000000 anaio-1.0.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-03-02 09:50:22.000000 anaio-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3726 2023-03-02 09:53:03.711463 anaio-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3283 2023-03-02 09:50:22.000000 anaio-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 09:53:03.707463 anaio-1.0.2/anaio/
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-03-02 09:50:22.000000 anaio-1.0.2/anaio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 09:53:03.707463 anaio-1.0.2/anaio/__pycache__/
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-03-02 09:50:22.000000 anaio-1.0.2/anaio/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0 root         (0) root         (0)     6459 2023-03-02 09:50:22.000000 anaio-1.0.2/anaio/__pycache__/anaio.cpython-38.pyc
--rwxrwxrwx   0 root         (0) root         (0)   210784 2023-03-02 09:50:22.000000 anaio-1.0.2/anaio/_anaio.cpython-38-x86_64-linux-gnu.so
--rwxrwxrwx   0 root         (0) root         (0)     6665 2023-03-02 09:50:22.000000 anaio-1.0.2/anaio/anaio.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 09:53:03.707463 anaio-1.0.2/anaio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3726 2023-03-02 09:53:03.000000 anaio-1.0.2/anaio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      478 2023-03-02 09:53:03.000000 anaio-1.0.2/anaio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-02 09:53:03.000000 anaio-1.0.2/anaio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-02 09:53:03.000000 anaio-1.0.2/anaio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-02 09:53:03.000000 anaio-1.0.2/anaio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-02 09:53:03.711463 anaio-1.0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1649 2023-03-02 09:50:22.000000 anaio-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 09:53:03.711463 anaio-1.0.2/src/
--rw-rw-rw-   0 root         (0) root         (0)     8829 2023-03-02 09:50:22.000000 anaio-1.0.2/src/_anaio.c
--rw-rw-rw-   0 root         (0) root         (0)    26787 2023-03-02 09:50:22.000000 anaio-1.0.2/src/anacompress.c
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-03-02 09:50:22.000000 anaio-1.0.2/src/anacompress.h
--rw-rw-rw-   0 root         (0) root         (0)    21226 2023-03-02 09:50:22.000000 anaio-1.0.2/src/anadecompress.c
--rw-rw-rw-   0 root         (0) root         (0)      553 2023-03-02 09:50:22.000000 anaio-1.0.2/src/anadecompress.h
--rw-rw-rw-   0 root         (0) root         (0)    11948 2023-03-02 09:50:22.000000 anaio-1.0.2/src/anarw.c
--rw-rw-rw-   0 root         (0) root         (0)     1168 2023-03-02 09:50:22.000000 anaio-1.0.2/src/anarw.h
--rw-rw-rw-   0 root         (0) root         (0)      954 2023-03-02 09:50:22.000000 anaio-1.0.2/src/testrw.c
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-03-02 09:50:22.000000 anaio-1.0.2/src/types.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:51:24.843401 anaio-1.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2023-05-31 07:49:59.000000 anaio-1.0.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-05-31 07:49:59.000000 anaio-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3742 2023-05-31 07:51:24.843401 anaio-1.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3283 2023-05-31 07:49:59.000000 anaio-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:51:24.839401 anaio-1.0.3/anaio/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-05-31 07:49:59.000000 anaio-1.0.3/anaio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:51:24.843401 anaio-1.0.3/anaio/__pycache__/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-31 07:49:59.000000 anaio-1.0.3/anaio/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0 root         (0) root         (0)     6459 2023-05-31 07:49:59.000000 anaio-1.0.3/anaio/__pycache__/anaio.cpython-38.pyc
+-rwxrwxrwx   0 root         (0) root         (0)   210784 2023-05-31 07:49:59.000000 anaio-1.0.3/anaio/_anaio.cpython-38-x86_64-linux-gnu.so
+-rwxrwxrwx   0 root         (0) root         (0)     6665 2023-05-31 07:49:59.000000 anaio-1.0.3/anaio/anaio.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:51:24.839401 anaio-1.0.3/anaio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3742 2023-05-31 07:51:24.000000 anaio-1.0.3/anaio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      478 2023-05-31 07:51:24.000000 anaio-1.0.3/anaio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 07:51:24.000000 anaio-1.0.3/anaio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-05-31 07:51:24.000000 anaio-1.0.3/anaio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 07:51:24.000000 anaio-1.0.3/anaio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 07:51:24.843401 anaio-1.0.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1711 2023-05-31 07:49:59.000000 anaio-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:51:24.843401 anaio-1.0.3/src/
+-rw-rw-rw-   0 root         (0) root         (0)     8829 2023-05-31 07:49:59.000000 anaio-1.0.3/src/_anaio.c
+-rw-rw-rw-   0 root         (0) root         (0)    26787 2023-05-31 07:49:59.000000 anaio-1.0.3/src/anacompress.c
+-rw-rw-rw-   0 root         (0) root         (0)      613 2023-05-31 07:49:59.000000 anaio-1.0.3/src/anacompress.h
+-rw-rw-rw-   0 root         (0) root         (0)    21226 2023-05-31 07:49:59.000000 anaio-1.0.3/src/anadecompress.c
+-rw-rw-rw-   0 root         (0) root         (0)      553 2023-05-31 07:49:59.000000 anaio-1.0.3/src/anadecompress.h
+-rw-rw-rw-   0 root         (0) root         (0)    11948 2023-05-31 07:49:59.000000 anaio-1.0.3/src/anarw.c
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2023-05-31 07:49:59.000000 anaio-1.0.3/src/anarw.h
+-rw-rw-rw-   0 root         (0) root         (0)      954 2023-05-31 07:49:59.000000 anaio-1.0.3/src/testrw.c
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-05-31 07:49:59.000000 anaio-1.0.3/src/types.h
```

### Comparing `anaio-1.0.2/LICENSE` & `anaio-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anaio-1.0.2/PKG-INFO` & `anaio-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: anaio
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python library for ANA f0 file I/O
 Home-page: https://gitlab.gwdg.de/hoelken/anaio
 Author: Johannes Hoelken
 Author-email: hoelken@mps.mpg.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires: setuptools
+Requires: numpy
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ANA.IO - A Python module for ANA f0 file I/O
 ==========================================
 
 This is `anaio`, a Python module to perform file input and output operations
```

### Comparing `anaio-1.0.2/README.md` & `anaio-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `anaio-1.0.2/anaio/__pycache__/anaio.cpython-38.pyc` & `anaio-1.0.3/anaio/__pycache__/anaio.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anaio-1.0.2/anaio/_anaio.cpython-38-x86_64-linux-gnu.so` & `anaio-1.0.3/anaio/_anaio.cpython-38-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `anaio-1.0.2/anaio/anaio.py` & `anaio-1.0.3/anaio/anaio.py`

 * *Files identical despite different names*

### Comparing `anaio-1.0.2/anaio.egg-info/PKG-INFO` & `anaio-1.0.3/anaio.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: anaio
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python library for ANA f0 file I/O
 Home-page: https://gitlab.gwdg.de/hoelken/anaio
 Author: Johannes Hoelken
 Author-email: hoelken@mps.mpg.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires: setuptools
+Requires: numpy
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ANA.IO - A Python module for ANA f0 file I/O
 ==========================================
 
 This is `anaio`, a Python module to perform file input and output operations
```

### Comparing `anaio-1.0.2/setup.py` & `anaio-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                          extra_link_args=None,
                          sources=['src/_anaio.c',
                                   'src/anarw.c',
                                   'src/anacompress.c',
                                   'src/anadecompress.c'])
 
 setup(name='anaio',
-      version='1.0.2',
+      version='1.0.3',
       description='Python library for ANA f0 file I/O',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Johannes Hoelken',
       author_email='hoelken@mps.mpg.de',
       url='https://gitlab.gwdg.de/hoelken/anaio',
       license="MIT",
@@ -37,11 +37,12 @@
           'Operating System :: OS Independent'
       ],
       # This is for the python wrapper module:
       package_dir={'anaio': 'anaio'},
       packages=['anaio'],
       ext_package='anaio',
       # Python dependency
-      install_requires=['numpy'],
-      requires=['setuptools'],
+      install_requires=['numpy; python_version>="3"'],
+      setup_requires=['numpy'],
+      requires=['setuptools', 'numpy'],
       # This is for the C module
       ext_modules=[module_anaio])
```

### Comparing `anaio-1.0.2/src/_anaio.c` & `anaio-1.0.3/src/_anaio.c`

 * *Files identical despite different names*

### Comparing `anaio-1.0.2/src/anacompress.c` & `anaio-1.0.3/src/anacompress.c`

 * *Files identical despite different names*

### Comparing `anaio-1.0.2/src/anacompress.h` & `anaio-1.0.3/src/anacompress.h`

 * *Files identical despite different names*

### Comparing `anaio-1.0.2/src/anadecompress.c` & `anaio-1.0.3/src/anadecompress.c`

 * *Files identical despite different names*

### Comparing `anaio-1.0.2/src/anadecompress.h` & `anaio-1.0.3/src/anadecompress.h`

 * *Files identical despite different names*

### Comparing `anaio-1.0.2/src/anarw.c` & `anaio-1.0.3/src/anarw.c`

 * *Files identical despite different names*

### Comparing `anaio-1.0.2/src/anarw.h` & `anaio-1.0.3/src/anarw.h`

 * *Files identical despite different names*

### Comparing `anaio-1.0.2/src/testrw.c` & `anaio-1.0.3/src/testrw.c`

 * *Files identical despite different names*

### Comparing `anaio-1.0.2/src/types.h` & `anaio-1.0.3/src/types.h`

 * *Files identical despite different names*

