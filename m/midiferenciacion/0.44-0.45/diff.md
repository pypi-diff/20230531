# Comparing `tmp/midiferenciacion-0.44.tar.gz` & `tmp/midiferenciacion-0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midiferenciacion-0.44.tar", last modified: Tue May 30 17:48:01 2023, max compression
+gzip compressed data, was "midiferenciacion-0.45.tar", last modified: Wed May 31 05:29:57 2023, max compression
```

## Comparing `midiferenciacion-0.44.tar` & `midiferenciacion-0.45.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sarboledab   (501) staff       (20)        0 2023-05-30 17:48:01.537407 midiferenciacion-0.44/
--rw-r--r--   0 sarboledab   (501) staff       (20)     1134 2023-05-16 14:58:24.000000 midiferenciacion-0.44/LICENSE
--rw-r--r--   0 sarboledab   (501) staff       (20)     2063 2023-05-30 17:48:01.536684 midiferenciacion-0.44/PKG-INFO
--rw-r--r--   0 sarboledab   (501) staff       (20)     1585 2023-05-18 18:45:10.000000 midiferenciacion-0.44/README.md
-drwxr-xr-x   0 sarboledab   (501) staff       (20)        0 2023-05-30 17:48:01.531311 midiferenciacion-0.44/midiferenciacion/
--rw-r--r--   0 sarboledab   (501) staff       (20)      158 2023-05-18 18:43:35.000000 midiferenciacion-0.44/midiferenciacion/__init__.py
-drwxr-xr-x   0 sarboledab   (501) staff       (20)        0 2023-05-30 17:48:01.535744 midiferenciacion-0.44/midiferenciacion.egg-info/
--rw-r--r--   0 sarboledab   (501) staff       (20)     2063 2023-05-30 17:48:01.000000 midiferenciacion-0.44/midiferenciacion.egg-info/PKG-INFO
--rw-r--r--   0 sarboledab   (501) staff       (20)      314 2023-05-30 17:48:01.000000 midiferenciacion-0.44/midiferenciacion.egg-info/SOURCES.txt
--rw-r--r--   0 sarboledab   (501) staff       (20)        1 2023-05-30 17:48:01.000000 midiferenciacion-0.44/midiferenciacion.egg-info/dependency_links.txt
--rw-r--r--   0 sarboledab   (501) staff       (20)       58 2023-05-30 17:48:01.000000 midiferenciacion-0.44/midiferenciacion.egg-info/entry_points.txt
--rw-r--r--   0 sarboledab   (501) staff       (20)       23 2023-05-30 17:48:01.000000 midiferenciacion-0.44/midiferenciacion.egg-info/requires.txt
--rw-r--r--   0 sarboledab   (501) staff       (20)       17 2023-05-30 17:48:01.000000 midiferenciacion-0.44/midiferenciacion.egg-info/top_level.txt
--rw-r--r--   0 sarboledab   (501) staff       (20)      131 2023-05-16 14:58:32.000000 midiferenciacion-0.44/pyproject.toml
--rw-r--r--   0 sarboledab   (501) staff       (20)       38 2023-05-30 17:48:01.537619 midiferenciacion-0.44/setup.cfg
--rw-r--r--   0 sarboledab   (501) staff       (20)     2237 2023-05-30 17:47:19.000000 midiferenciacion-0.44/setup.py
+drwxr-xr-x   0 sarboledab   (501) staff       (20)        0 2023-05-31 05:29:57.326780 midiferenciacion-0.45/
+-rw-r--r--   0 sarboledab   (501) staff       (20)     1134 2023-05-16 14:58:24.000000 midiferenciacion-0.45/LICENSE
+-rw-r--r--   0 sarboledab   (501) staff       (20)     2193 2023-05-31 05:29:57.326174 midiferenciacion-0.45/PKG-INFO
+-rw-r--r--   0 sarboledab   (501) staff       (20)     1715 2023-05-31 05:28:34.000000 midiferenciacion-0.45/README.md
+drwxr-xr-x   0 sarboledab   (501) staff       (20)        0 2023-05-31 05:29:57.321309 midiferenciacion-0.45/midiferenciacion/
+-rw-r--r--   0 sarboledab   (501) staff       (20)      927 2023-05-31 05:23:33.000000 midiferenciacion-0.45/midiferenciacion/__init__.py
+drwxr-xr-x   0 sarboledab   (501) staff       (20)        0 2023-05-31 05:29:57.325212 midiferenciacion-0.45/midiferenciacion.egg-info/
+-rw-r--r--   0 sarboledab   (501) staff       (20)     2193 2023-05-31 05:29:57.000000 midiferenciacion-0.45/midiferenciacion.egg-info/PKG-INFO
+-rw-r--r--   0 sarboledab   (501) staff       (20)      314 2023-05-31 05:29:57.000000 midiferenciacion-0.45/midiferenciacion.egg-info/SOURCES.txt
+-rw-r--r--   0 sarboledab   (501) staff       (20)        1 2023-05-31 05:29:57.000000 midiferenciacion-0.45/midiferenciacion.egg-info/dependency_links.txt
+-rw-r--r--   0 sarboledab   (501) staff       (20)       58 2023-05-31 05:29:57.000000 midiferenciacion-0.45/midiferenciacion.egg-info/entry_points.txt
+-rw-r--r--   0 sarboledab   (501) staff       (20)       23 2023-05-31 05:29:57.000000 midiferenciacion-0.45/midiferenciacion.egg-info/requires.txt
+-rw-r--r--   0 sarboledab   (501) staff       (20)       17 2023-05-31 05:29:57.000000 midiferenciacion-0.45/midiferenciacion.egg-info/top_level.txt
+-rw-r--r--   0 sarboledab   (501) staff       (20)      131 2023-05-16 14:58:32.000000 midiferenciacion-0.45/pyproject.toml
+-rw-r--r--   0 sarboledab   (501) staff       (20)       38 2023-05-31 05:29:57.326997 midiferenciacion-0.45/setup.cfg
+-rw-r--r--   0 sarboledab   (501) staff       (20)     2237 2023-05-31 05:29:40.000000 midiferenciacion-0.45/setup.py
```

### Comparing `midiferenciacion-0.44/LICENSE` & `midiferenciacion-0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `midiferenciacion-0.44/README.md` & `midiferenciacion-0.45/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,75 @@
-# PyMiau
-## Use a short explanatory subtitle like, Make a Miau and a Guau
+Metadata-Version: 2.1
+Name: midiferenciacion
+Version: 0.45
+Summary: Make a diferentiation of a given function
+Home-page: https://pypi.org/project/midiferenciacion
+Author: Sofia Arboleda-Bolivar
+Author-email: sofia.arboledab@udea.edu.co
+License: MIT
+Keywords: Dif math
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Mi diferenciación 
+## This little package proof would help you solve some derivates given a defined function. 
 
 <!-- This are visual tags that you may add to your package at the beginning with useful information on your package --> 
-[![version 0.41](https://img.shields.io/pypi/v/pymiau?color=blue)](https://pypi.org/project/midiferenciacion/)
+[![version 0.45](https://img.shields.io/pypi/v/pymiau?color=blue)](https://pypi.org/project/midiferenciacion/)
 [![downloads](https://img.shields.io/pypi/dw/midiferenciacion)](https://pypi.org/project/midiferenciacion/)
 
-Always start the README explaining clearly what your package do.  If
-you can include here some beautiful image to call the attention of the
-potential user do it!
-
-This is an example:
+Math is not easy, right? You can use some tools to make it easier at least for some calculations. 
+This simple package will help you in that. 
 
 <p align="center"><img src="https://drive.google.com/uc?export=view&id=1P4T-6cMTga6iO4rFBhVvevcg1CgBuUto" alt="Logo""/></p>
 
 ## Download and install
 
-Describe here how the package can be downloaded and install it in
-different arquitectures.
-
 If you are using `PyPI` installation it's as simple as:
 
 ```
 pip install midiferenciacion
 ```
 
 You can also test the unstable version of the package with:
 
 ```
 pip install -i https://test.pypi.org/simple/midiferenciacion
 ```
 
 ## Quick start
 
-In this section you should provide the most simple instructions to use
-your package.
-
-For instance:
+First import the midiferenciacion
 
 ```
 import midiferenciacion
-print(midiferenciacion.dif())
-```
 
-## Code examples
+```
+Now, you have to be careful with the input of the only function we have for now: derivative. This function gives you the first derivative and you can evaluate the result in two defined points. 
 
-Provide some detailed examples for more advanced users.
+The function derivative receives a function in a string format and (very important) in terms of x variable, and it also receives two values to evaluate the solution.
 
-For instance:
+Here's an example of a single function:
 
 ```
-import midiferenciacion
-print(midiferenciacion.dif(x=2))
+midiferenciacion.derivative("x**2", 1, 2)
+
 ```
 
 ## What's new
 
 
 
-Version 0.41:
+Version 0.45:
 
-- README updates
+- README updates and beautiful meme
 
 Version 0.4:
 
 - First version of the package.
 
 ------------
 
-This package has been designed and written by Fulanit@ de Tal (C) 2023
+This package has been designed and written by Fulanit@ de Tal (C) 2023
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `midiferenciacion-0.44/setup.py` & `midiferenciacion-0.45/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # CLASSIFIER
     # ######################################################################
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         ],
-    version='0.44',
+    version='0.45',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={'': '.'},
     packages=setuptools.find_packages(where='.'),
```

