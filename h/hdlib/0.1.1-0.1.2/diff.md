# Comparing `tmp/hdlib-0.1.1.tar.gz` & `tmp/hdlib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdlib-0.1.1.tar", last modified: Tue May 30 22:29:05 2023, max compression
+gzip compressed data, was "hdlib-0.1.2.tar", last modified: Wed May 31 21:37:50 2023, max compression
```

## Comparing `hdlib-0.1.1.tar` & `hdlib-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-30 22:29:05.675122 hdlib-0.1.1/
--rw-r--r--   0 fabio      (501) staff       (20)     1068 2022-04-25 18:30:15.000000 hdlib-0.1.1/LICENSE
--rw-r--r--   0 fabio      (501) staff       (20)     4809 2023-05-30 22:29:05.673692 hdlib-0.1.1/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)     4175 2023-05-30 22:22:49.000000 hdlib-0.1.1/README.md
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-30 22:29:05.621827 hdlib-0.1.1/hdlib/
--rw-r--r--   0 fabio      (501) staff       (20)      102 2023-05-30 18:40:44.000000 hdlib-0.1.1/hdlib/__init__.py
--rw-r--r--   0 fabio      (501) staff       (20)     2430 2023-05-30 20:19:23.000000 hdlib-0.1.1/hdlib/arithmetic.py
--rw-r--r--   0 fabio      (501) staff       (20)    10675 2023-05-30 22:22:45.000000 hdlib-0.1.1/hdlib/space.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-30 22:29:05.672109 hdlib-0.1.1/hdlib.egg-info/
--rw-r--r--   0 fabio      (501) staff       (20)     4809 2023-05-30 22:29:05.000000 hdlib-0.1.1/hdlib.egg-info/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)      251 2023-05-30 22:29:05.000000 hdlib-0.1.1/hdlib.egg-info/SOURCES.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2023-05-30 22:29:05.000000 hdlib-0.1.1/hdlib.egg-info/dependency_links.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2023-05-30 22:29:05.000000 hdlib-0.1.1/hdlib.egg-info/not-zip-safe
--rw-r--r--   0 fabio      (501) staff       (20)       14 2023-05-30 22:29:05.000000 hdlib-0.1.1/hdlib.egg-info/requires.txt
--rw-r--r--   0 fabio      (501) staff       (20)        6 2023-05-30 22:29:05.000000 hdlib-0.1.1/hdlib.egg-info/top_level.txt
--rw-r--r--   0 fabio      (501) staff       (20)       38 2023-05-30 22:29:05.675525 hdlib-0.1.1/setup.cfg
--rw-r--r--   0 fabio      (501) staff       (20)     1160 2023-05-30 18:40:55.000000 hdlib-0.1.1/setup.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-31 21:37:50.781648 hdlib-0.1.2/
+-rw-r--r--   0 fabio      (501) staff       (20)     1068 2022-04-25 18:30:15.000000 hdlib-0.1.2/LICENSE
+-rw-r--r--   0 fabio      (501) staff       (20)     8162 2023-05-31 21:37:50.780271 hdlib-0.1.2/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)     7528 2023-05-31 21:27:08.000000 hdlib-0.1.2/README.md
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-31 21:37:50.727018 hdlib-0.1.2/hdlib/
+-rw-r--r--   0 fabio      (501) staff       (20)      102 2023-05-31 01:26:41.000000 hdlib-0.1.2/hdlib/__init__.py
+-rw-r--r--   0 fabio      (501) staff       (20)     2489 2023-05-31 21:27:15.000000 hdlib-0.1.2/hdlib/arithmetic.py
+-rw-r--r--   0 fabio      (501) staff       (20)    16224 2023-05-31 21:10:24.000000 hdlib-0.1.2/hdlib/space.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-31 21:37:50.757133 hdlib-0.1.2/hdlib.egg-info/
+-rw-r--r--   0 fabio      (501) staff       (20)     8162 2023-05-31 21:37:50.000000 hdlib-0.1.2/hdlib.egg-info/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)      264 2023-05-31 21:37:50.000000 hdlib-0.1.2/hdlib.egg-info/SOURCES.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-05-31 21:37:50.000000 hdlib-0.1.2/hdlib.egg-info/dependency_links.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-05-31 21:37:50.000000 hdlib-0.1.2/hdlib.egg-info/not-zip-safe
+-rw-r--r--   0 fabio      (501) staff       (20)       14 2023-05-31 21:37:50.000000 hdlib-0.1.2/hdlib.egg-info/requires.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        6 2023-05-31 21:37:50.000000 hdlib-0.1.2/hdlib.egg-info/top_level.txt
+-rw-r--r--   0 fabio      (501) staff       (20)       38 2023-05-31 21:37:50.782331 hdlib-0.1.2/setup.cfg
+-rw-r--r--   0 fabio      (501) staff       (20)     1195 2023-05-31 01:45:31.000000 hdlib-0.1.2/setup.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-31 21:37:50.777778 hdlib-0.1.2/test/
+-rw-r--r--   0 fabio      (501) staff       (20)     6586 2023-05-31 18:54:12.000000 hdlib-0.1.2/test/test.py
```

### Comparing `hdlib-0.1.1/LICENSE` & `hdlib-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.1/hdlib/arithmetic.py` & `hdlib-0.1.2/hdlib/arithmetic.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,67 +10,73 @@
 def bundle(vector1: Vector, vector2: Vector) -> Vector:
     """
     Bundle vectors
 
     Properties:
     > The resulting vector is similar to the input vectors
     > The more vectors are involved in bundling, the harder it is to determine the component vectors
-    > If several copies of any vector are included in bundling, the resulting vector is closer to the dominant vector than to the other component
+    > If several copies of any vector are included in bundling, the resulting vector is closer to the dominant vector than to the other components
 
     :param vector1:     Vector object
     :param vector2:     Vector object
     :return:            Vector resulted from bundling vector1 and vector2
     """
 
-    if not isinstance(vector1, Vector) or not isinstance(vector2, Vector):
-        raise TypeError("Input is not a valid Vector object")
-
     if vector1.size != vector2.size:
         raise Exception("Vectors must have the same size")
 
+    if vector1.vtype != vector2.vtype:
+        raise Exception("Vector types are not compatible")
+
     vector = vector1.vector + vector2.vector
-    return Vector(size=vector1.size, vector=vector, seed=vector1.seed)
+
+    tags = list(set(vector1.tags).union(set(vector2.tags)))
+
+    return Vector(size=vector1.size, vector=vector, tags=tags, vtype=vector1.vtype, seed=vector1.seed)
+
 
 def bind(vector1: Vector, vector2: Vector) -> Vector:
     """
     Bind vectors
 
     Properties:
     > Invertible (unbind)
     > It distributes over bundling
-    > It preserves distance
+    > It preserves the distance
     > The resulting vector is dissimilar to the input vectors
 
     :param vector1:     Vector object
     :param vector2:     Vector object
     :return:            Vector resulted from binding vector1 and vector2
     """
 
-    if not isinstance(vector1, Vector) or not isinstance(vector2, Vector):
-        raise TypeError("Input is not a valid Vector object")
-
     if vector1.size != vector2.size:
         raise Exception("Vectors must have the same size")
 
+    if vector1.vtype != vector2.vtype:
+        raise Exception("Vector types are not compatible")
+
     vector = vector1.vector * vector2.vector
-    return Vector(size=vector1.size, vector=vector, seed=vector1.seed)
+
+    tags = list(set(vector1.tags).union(set(vector2.tags)))
+
+    return Vector(size=vector1.size, vector=vector, tags=tags, vtype=vector1.vtype, seed=vector1.seed)
+
 
 def permute(vector: Vector, rotateby: int=1) -> Vector:
     """
     Permute vector
 
     Properties:
     > Invertible
-    > It distribute over bundling and any elementwise operation
-    > It preserves distance
+    > It distributes over bundling and any elementwise operation
+    > It preserves the distance
     > The resulting vector is dissimilar to the input vectors
 
     :param vector:      Vector object
     :param rotateby:    How many rotations
     :return:            Input vector rotated "rotateby" times
     """
 
-    if not isinstance(vector, Vector):
-        raise TypeError("Input is not a valid Vector object")
-
     rolled = np.roll(vector.vector, rotateby, axis=0)
-    return Vector(size=vector.size, vector=rolled, seed=vector.seed)
+
+    return Vector(size=vector.size, vector=rolled, tags=vector.tags, vtype=vector.vtype, seed=vector.seed)
```

### Comparing `hdlib-0.1.1/setup.py` & `hdlib-0.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,13 +21,13 @@
     description="Hyperdimensional Computing Library for building Vector Symbolic Architectures in Python",
     install_requires=["numpy>=1.22.3"],
     license="MIT",
     license_files=["LICENSE"],
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     name="hdlib",
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages(include=["hdlib"], exclude=["test"]),
     python_requires=">=3",
     url="http://github.com/cumbof/hdlib",
     version=__version__,
     zip_safe=False
 )
```

