# Comparing `tmp/random_math_rmaiaaaa-1.1.0.tar.gz` & `tmp/random_math_rmaiaaaa-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/random-math/random-math/dist/.tmp-49qq_nd_/random_math_rmaiaaaa-1.1.0.tar", last modified: Tue May 30 21:53:06 2023, max compression
+gzip compressed data, was "/home/runner/work/random-math/random-math/dist/.tmp-xpg74gqy/random_math_rmaiaaaa-1.2.0.tar", last modified: Tue May 30 22:45:43 2023, max compression
```

## Comparing `random_math_rmaiaaaa-1.1.0.tar` & `random_math_rmaiaaaa-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:53:06.000000 random_math_rmaiaaaa-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-30 21:52:52.000000 random_math_rmaiaaaa-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-30 21:53:06.000000 random_math_rmaiaaaa-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 21:52:52.000000 random_math_rmaiaaaa-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-30 21:52:52.000000 random_math_rmaiaaaa-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:53:06.000000 random_math_rmaiaaaa-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:53:06.000000 random_math_rmaiaaaa-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:53:06.000000 random_math_rmaiaaaa-1.1.0/src/RandomMath/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-30 21:52:52.000000 random_math_rmaiaaaa-1.1.0/src/RandomMath/RandomMathOperations.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 21:52:52.000000 random_math_rmaiaaaa-1.1.0/src/RandomMath/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:53:06.000000 random_math_rmaiaaaa-1.1.0/src/apiRandomMath/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:52:52.000000 random_math_rmaiaaaa-1.1.0/src/apiRandomMath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-30 21:52:52.000000 random_math_rmaiaaaa-1.1.0/src/apiRandomMath/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:53:06.000000 random_math_rmaiaaaa-1.1.0/src/random_math_rmaiaaaa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-30 21:53:06.000000 random_math_rmaiaaaa-1.1.0/src/random_math_rmaiaaaa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-30 21:53:06.000000 random_math_rmaiaaaa-1.1.0/src/random_math_rmaiaaaa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:53:06.000000 random_math_rmaiaaaa-1.1.0/src/random_math_rmaiaaaa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 21:53:06.000000 random_math_rmaiaaaa-1.1.0/src/random_math_rmaiaaaa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:45:43.000000 random_math_rmaiaaaa-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-30 22:45:30.000000 random_math_rmaiaaaa-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-30 22:45:43.000000 random_math_rmaiaaaa-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 22:45:30.000000 random_math_rmaiaaaa-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-30 22:45:30.000000 random_math_rmaiaaaa-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 22:45:43.000000 random_math_rmaiaaaa-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:45:43.000000 random_math_rmaiaaaa-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:45:43.000000 random_math_rmaiaaaa-1.2.0/src/RandomMath/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-30 22:45:30.000000 random_math_rmaiaaaa-1.2.0/src/RandomMath/RandomMathOperations.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 22:45:30.000000 random_math_rmaiaaaa-1.2.0/src/RandomMath/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:45:43.000000 random_math_rmaiaaaa-1.2.0/src/apiRandomMath/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:45:30.000000 random_math_rmaiaaaa-1.2.0/src/apiRandomMath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-30 22:45:30.000000 random_math_rmaiaaaa-1.2.0/src/apiRandomMath/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:45:43.000000 random_math_rmaiaaaa-1.2.0/src/random_math_rmaiaaaa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-30 22:45:43.000000 random_math_rmaiaaaa-1.2.0/src/random_math_rmaiaaaa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-30 22:45:43.000000 random_math_rmaiaaaa-1.2.0/src/random_math_rmaiaaaa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:45:43.000000 random_math_rmaiaaaa-1.2.0/src/random_math_rmaiaaaa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 22:45:43.000000 random_math_rmaiaaaa-1.2.0/src/random_math_rmaiaaaa.egg-info/top_level.txt
```

### Comparing `random_math_rmaiaaaa-1.1.0/LICENSE` & `random_math_rmaiaaaa-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `random_math_rmaiaaaa-1.1.0/PKG-INFO` & `random_math_rmaiaaaa-1.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: random_math_rmaiaaaa
-Version: 1.1.0
+Version: 1.2.0
 Summary: Random Math Package
 Author-email: Rafael Maia de Souza <rmaiadesouza@gmail.com>
 Project-URL: Homepage, https://github.com/rmaiaaaa/random-math
 Project-URL: Bug Tracker, https://github.com/rmaiaaaa/random-math/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `random_math_rmaiaaaa-1.1.0/pyproject.toml` & `random_math_rmaiaaaa-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "random_math_rmaiaaaa"
-version = "v1.1.0"
+version = "v1.2.0"
 authors = [
   { name="Rafael Maia de Souza", email="rmaiadesouza@gmail.com" },
 ]
 description = "Random Math Package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `random_math_rmaiaaaa-1.1.0/src/RandomMath/RandomMathOperations.py` & `random_math_rmaiaaaa-1.2.0/src/RandomMath/RandomMathOperations.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,7 +15,14 @@
 
     def random_sub(self, number: int = 0) -> int:
         '''
         Realiza a subtração de um número de entrada por um número aleatório
         '''
         random_int = random.randint(1, number)
         return number - random_int
+
+    def random_mul(self, number: int = 0) -> int:
+        '''
+        Realiza a multiplicação de um número de entrada por um número aleatório
+        '''
+        random_int = random.randint(1, number)
+        return number * random_int
```

### Comparing `random_math_rmaiaaaa-1.1.0/src/random_math_rmaiaaaa.egg-info/PKG-INFO` & `random_math_rmaiaaaa-1.2.0/src/random_math_rmaiaaaa.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: random-math-rmaiaaaa
-Version: 1.1.0
+Version: 1.2.0
 Summary: Random Math Package
 Author-email: Rafael Maia de Souza <rmaiadesouza@gmail.com>
 Project-URL: Homepage, https://github.com/rmaiaaaa/random-math
 Project-URL: Bug Tracker, https://github.com/rmaiaaaa/random-math/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

