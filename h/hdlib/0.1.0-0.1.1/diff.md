# Comparing `tmp/hdlib-0.1.0.tar.gz` & `tmp/hdlib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hdlib-0.1.0.tar", last modified: Mon Apr 25 22:39:24 2022, max compression
+gzip compressed data, was "hdlib-0.1.1.tar", last modified: Tue May 30 22:29:05 2023, max compression
```

## Comparing `hdlib-0.1.0.tar` & `hdlib-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2022-04-25 22:39:24.000000 hdlib-0.1.0/
--rw-r--r--   0 fabio      (501) staff       (20)     5169 2022-04-25 22:39:24.000000 hdlib-0.1.0/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)     4031 2022-04-25 22:31:39.000000 hdlib-0.1.0/README.md
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2022-04-25 22:39:24.000000 hdlib-0.1.0/hdlib/
--rw-r--r--   0 fabio      (501) staff       (20)        0 2022-04-25 20:59:52.000000 hdlib-0.1.0/hdlib/__init__.py
--rw-r--r--   0 fabio      (501) staff       (20)     2483 2022-04-25 21:07:00.000000 hdlib-0.1.0/hdlib/arithmetic.py
--rw-r--r--   0 fabio      (501) staff       (20)     7671 2022-04-25 21:03:51.000000 hdlib-0.1.0/hdlib/space.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2022-04-25 22:39:24.000000 hdlib-0.1.0/hdlib.egg-info/
--rw-r--r--   0 fabio      (501) staff       (20)     5169 2022-04-25 22:39:24.000000 hdlib-0.1.0/hdlib.egg-info/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)      243 2022-04-25 22:39:24.000000 hdlib-0.1.0/hdlib.egg-info/SOURCES.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2022-04-25 22:39:24.000000 hdlib-0.1.0/hdlib.egg-info/dependency_links.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2022-04-25 22:39:24.000000 hdlib-0.1.0/hdlib.egg-info/not-zip-safe
--rw-r--r--   0 fabio      (501) staff       (20)        6 2022-04-25 22:39:24.000000 hdlib-0.1.0/hdlib.egg-info/requires.txt
--rw-r--r--   0 fabio      (501) staff       (20)        6 2022-04-25 22:39:24.000000 hdlib-0.1.0/hdlib.egg-info/top_level.txt
--rw-r--r--   0 fabio      (501) staff       (20)       38 2022-04-25 22:39:24.000000 hdlib-0.1.0/setup.cfg
--rw-r--r--   0 fabio      (501) staff       (20)      926 2022-04-25 20:46:41.000000 hdlib-0.1.0/setup.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-30 22:29:05.675122 hdlib-0.1.1/
+-rw-r--r--   0 fabio      (501) staff       (20)     1068 2022-04-25 18:30:15.000000 hdlib-0.1.1/LICENSE
+-rw-r--r--   0 fabio      (501) staff       (20)     4809 2023-05-30 22:29:05.673692 hdlib-0.1.1/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)     4175 2023-05-30 22:22:49.000000 hdlib-0.1.1/README.md
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-30 22:29:05.621827 hdlib-0.1.1/hdlib/
+-rw-r--r--   0 fabio      (501) staff       (20)      102 2023-05-30 18:40:44.000000 hdlib-0.1.1/hdlib/__init__.py
+-rw-r--r--   0 fabio      (501) staff       (20)     2430 2023-05-30 20:19:23.000000 hdlib-0.1.1/hdlib/arithmetic.py
+-rw-r--r--   0 fabio      (501) staff       (20)    10675 2023-05-30 22:22:45.000000 hdlib-0.1.1/hdlib/space.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-30 22:29:05.672109 hdlib-0.1.1/hdlib.egg-info/
+-rw-r--r--   0 fabio      (501) staff       (20)     4809 2023-05-30 22:29:05.000000 hdlib-0.1.1/hdlib.egg-info/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)      251 2023-05-30 22:29:05.000000 hdlib-0.1.1/hdlib.egg-info/SOURCES.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-05-30 22:29:05.000000 hdlib-0.1.1/hdlib.egg-info/dependency_links.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-05-30 22:29:05.000000 hdlib-0.1.1/hdlib.egg-info/not-zip-safe
+-rw-r--r--   0 fabio      (501) staff       (20)       14 2023-05-30 22:29:05.000000 hdlib-0.1.1/hdlib.egg-info/requires.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        6 2023-05-30 22:29:05.000000 hdlib-0.1.1/hdlib.egg-info/top_level.txt
+-rw-r--r--   0 fabio      (501) staff       (20)       38 2023-05-30 22:29:05.675525 hdlib-0.1.1/setup.cfg
+-rw-r--r--   0 fabio      (501) staff       (20)     1160 2023-05-30 18:40:55.000000 hdlib-0.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hdlib-0.1.0/README.md` & `hdlib-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # Install with conda
 conda install -c conda-forge hdlib
 ```
 
 ## Usage
 
-The `hdlib` library provides two main modules, `space` and `arithmetic`. The first one contains constructors of `Space` and `Vector` objects that can be used to build vectors and the space that hosts them. The second module, calle `arithmetic`, contains a bunch of functions to operate on vectors.
+The `hdlib` library provides two main modules, `space` and `arithmetic`. The first one contains constructors of `Space` and `Vector` objects that can be used to build vectors and the space that hosts them. The second module, called `arithmetic`, contains a bunch of functions to operate on vectors.
 
 ```python
 from hdlib.space import Space, Vector
 from hdlib.arithmetic import bind, bundle, permute
 ```
 
 ### What is the dollar of Mexico?
@@ -54,24 +54,24 @@
 
 # Build a random bipolar vector for each feature and country information
 # Add vectors to the space
 space.bulkInsert(names)
 
 # Encode USA information in a single vector
 # USTATES = [(NAM * USA) + (CAP * WDC) + (MON * DOL)]
-USTATES_NAM = bind(space.get("NAM"), space.get("USA")) # Bind NAM with USA
-USTATES_CAP = bind(space.get("CAP"), space.get("WDC")) # Bind CAP with WDC
-USTATES_MON = bind(space.get("MON"), space.get("DOL")) # Bind MON with DOL
+USTATES_NAM = bind(space.get(names=["NAM"])[0], space.get(names=["USA"])[0]) # Bind NAM with USA
+USTATES_CAP = bind(space.get(names=["CAP"])[0], space.get(names=["WDC"])[0]) # Bind CAP with WDC
+USTATES_MON = bind(space.get(names=["MON"])[0], space.get(names=["DOL"])[0]) # Bind MON with DOL
 USTATES = bundle(bundle(USTATES_NAM, USTATES_CAP), USTATES_MON) # Bundle USTATES_NAM, USTATES_CAP, and USTATES_MON
 
 # Repeat the last step to encode MEX information in a single vector
 # MEXICO = [(NAM * MEX) + (CAP * MXC) + (MON * PES)]
-MEXICO_NAM = bind(space.get("NAM"), space.get("MEX")) # Bind NAM with MEX
-MEXICO_CAP = bind(space.get("CAP"), space.get("MXC")) # Bind CAP with MXC
-MEXICO_MON = bind(space.get("MON"), space.get("PES")) # Bind MON with PES
+MEXICO_NAM = bind(space.get(names=["NAM"])[0], space.get(names=["MEX"])[0]) # Bind NAM with MEX
+MEXICO_CAP = bind(space.get(names=["CAP"])[0], space.get(names=["MXC"])[0]) # Bind CAP with MXC
+MEXICO_MON = bind(space.get(names=["MON"])[0], space.get(names=["PES"])[0]) # Bind MON with PES
 MEXICO = bundle(bundle(MEXICO_NAM, MEXICO_CAP), MEXICO_MON) # Bundle MEXICO_NAM, MEXICO_CAP, and MEXICO_MON
 ```
 
 If we now pair `USTATES` with `MEXICO`, we get a bundle that pairs USA with Mexico, Washington DC with Mexico City, and US Dollar with Peso, plus noise.
 ```python
 # F_UM = USTATES * MEXICO
 #      = [(USA * MEX) + (WDC * MXC) + (DOL * PES) + noise]
@@ -81,15 +81,15 @@
 In order to retrieve the Monetary Unit that in Mexico corresponds to Dollar:
 ```python
 # DOL * F_UM = DOL * [(USA * MEX) + (WDC * MXC) + (DOL * PES) + noise]
 #            = [(DOL * USA * MEX) + (DOL * WDC * MXC) + (DOL * DOL * PES) + (DOL * noise)]
 #            = [noise1 + noise2 + PES + noise3]
 #            = [PES + noise4]
 #            ≈ PES
-GUESS_PES = bind(space.get("DOL"), F_UM)
+GUESS_PES = bind(space.get(names=["DOL"])[0], F_UM)
 ```
 
 Finally answer the question by searching for the closest vector in space
 ```python
 space.find(GUESS_PES)
 ```
```

### Comparing `hdlib-0.1.0/hdlib/arithmetic.py` & `hdlib-0.1.1/hdlib/arithmetic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-__authors__ = ('Fabio Cumbo (fabio.cumbo@gmail.com)')
-__version__ = '0.1.0'
-__date__ = 'Apr 24, 2022'
+"""
+Implementation of the arithmetic operators
+"""
 
 import numpy as np
+
 from hdlib.space import Vector
 
+
 def bundle(vector1: Vector, vector2: Vector) -> Vector:
     """
     Bundle vectors
 
     Properties:
     > The resulting vector is similar to the input vectors
     > The more vectors are involved in bundling, the harder it is to determine the component vectors
@@ -17,15 +19,15 @@
     :param vector1:     Vector object
     :param vector2:     Vector object
     :return:            Vector resulted from bundling vector1 and vector2
     """
 
     if not isinstance(vector1, Vector) or not isinstance(vector2, Vector):
         raise TypeError("Input is not a valid Vector object")
-    
+
     if vector1.size != vector2.size:
         raise Exception("Vectors must have the same size")
 
     vector = vector1.vector + vector2.vector
     return Vector(size=vector1.size, vector=vector, seed=vector1.seed)
 
 def bind(vector1: Vector, vector2: Vector) -> Vector:
```

### Comparing `hdlib-0.1.0/hdlib/space.py` & `hdlib-0.1.1/hdlib/space.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,108 @@
-__authors__ = ('Fabio Cumbo (fabio.cumbo@gmail.com)')
-__version__ = '0.1.0'
-__date__ = 'Apr 24, 2022'
+"""
+Implementation of hyperdimensional Vector and Space
+"""
 
+import os
+import pickle
 import uuid
+
 import numpy as np
-from typing import Tuple
+from typing import List, Optional, Tuple, Union
+
 
 class Vector(object):
     """
     Vector object
     """
 
-    def __init__(self, name: str=None, size: int=1000, vector: np.ndarray=None, seed: int=None) -> None:
+    def __init__(
+        self,
+        name: Optional[str]=None,
+        size: int=1000,
+        vector: Optional[np.ndarray]=None,
+        tags: Optional[List[Union[str, int, float]]]=None,
+        seed: Optional[int]=None
+    ) -> "Vector":
         """
         Initialize a Vector object
 
         :param name:        Vector name or id
         :param size:        Vector size
         :param vector:      Vector as numpy.ndarray
+        :param tags:        Tags for grouping vectors
         :param seed:        Random seed for reproducibility
+        :return:            A Vector object
         """
 
         # Conditions on vector name or id
         # Vector name is casted to string. For this reason, only Python primitives are allowed
         # A random name is assigned if not specified
         try:
             if name is None:
                 name = str(uuid.uuid4())
+
             else:
                 name = str(name)
+
             self.name = name
+
         except:
             raise TypeError("Vector name must be an instance of a primitive")
-        
+
         # Conditions on vector size
         # It must be an integer number greater than 1000
         if not isinstance(size, int):
             raise TypeError("Vector size must be an integer number")
+
         if size < 1000:
             raise ValueError("Vector size must be greater than 1000")
+
         self.size = size        
 
         # Register random seed for reproducibility 
         self.seed = seed
 
+        # Add tags
+        self.tags = tags if tags else list()
+
         # Conditions on vector
         # It must be a Numpy ndarray
         # A random bipolar vector is generated if not specified
         if vector is not None:
             if not isinstance(vector, np.ndarray):
                 raise TypeError("Vector must be an instance of numpy.ndarray")
 
             self.vector = vector
+
         else:
             if seed is None:
                 rand = np.random
+
             else:
                 # Conditions on random seed for reproducibility
                 # Numpy allows integers as random seeds
                 if not isinstance(seed, int):
                     raise TypeError("Seed must be an integer number")
-                
+
                 rand = np.random.default_rng(seed=self.seed)
-            
+
             # Build a random bipolar vector
             self.vector = 2*rand.randint(2, size=size)-1
-    
-    # Forward reference of Vector class
-    def dist(self, vector: 'Vector') -> float:
+
+    def __len__(self) -> int:
+        """
+        Get the vector size
+
+        :return:    The length of vector
+        """
+
+        return self.size
+
+    def dist(self, vector: "Vector") -> float:
         """
         Compute distance between vectors as cosine similarity
 
         :param vector:      Vector object
         :return:            Cosine similarity
         """
 
@@ -79,150 +110,243 @@
             raise TypeError("Input must be a Vector object")
 
         if self.size != vector.size:
             raise Exception("Vectors must have the same size")
 
         return np.dot(self.vector, vector.vector) / (np.linalg.norm(self.vector) * np.linalg.norm(vector.vector))
 
+
 class Space(object):
     """
     Vectors space
     """
 
-    def __init__(self, size: int=1000) -> None:
+    def __init__(self, size: int=1000, from_file: Optional[os.path.abspath]=None) -> "Space":
         """
         Initialize the vectors space as a dictionary of Vector objects
 
-        :size:int:      Vector size
+        :param size:        Size of vectors in the space
+        :param from_file:   Load a space from file
+        :return:            A Space object
         """
 
         self.space = dict()
+
         self.size = size
 
-    def memory(self) -> list:
+        if from_file and os.path.isfile(from_file):
+            self.size, self.space = pickle.load(open(from_file, "rb"))
+
+    def __len__(self) -> int:
+        """
+        Get the space size
+
+        :return:    The number of vectors in the space
+        """
+
+        return len(self.space)
+
+    def memory(self) -> List[str]:
         """
         Return ids of vectors in space
 
         :return:    Names or ids of vectors in space
         """
 
         return list(self.space.keys())
 
-    def get(self, name: str) -> Vector:
+    def get(
+        self,
+        names: Optional[List[str]]=None,
+        tags: Optional[List[Union[str, int, float]]]=None
+    ) -> List[Vector]:
         """
-        Get a vector from the space
+        Get vectors by names or tags
 
-        :param name:    Vector name or id
-        :return:        Vector in space
+        :param names:   List of vector names or IDs
+        :param tags:    List of tags
+        :return:        List of vectors in space
         """
 
+        if not names and not tags:
+            raise Exception("No names or tags provided!")            
+
         try:
-            name = str(name)
-            if name in self.space:
-                return self.space[name]
-            raise Exception("Vector not in space")
+            vectors = list()
+
+            if names:
+                names = [str(name) for name in names]
+
+                for vector_name in names:
+                    if vector_name in self.space:
+                        vectors.append(self.space[vector_name])
+
+            elif tags:
+                for tag in tags:
+                    if not isinstance(tag, str) and not isinstance(tag, int) and not isinstance(tag, float):
+                        raise TypeError("Tags must be string, integer, or float")
+
+                for vector_name in self.space:
+                    if set(tags).intersection(self.space[vector_name].tags):
+                        vectors.append(self.space[vector_name])
+
+            return vectors
+
         except:
             raise TypeError("Input must be an instance of a primitive")
-    
+
     def insert(self, vector: Vector) -> None:
         """
         Add a Vector object to the space
 
         :param vector:      Vector object
         """
 
         if not isinstance(vector, Vector):
             raise TypeError("Input must be a Vector object")
-        
+
         if self.size != vector.size:
             raise Exception("Space and vectors with different size are not compatible")
 
         if vector.name in self.space:
             raise Exception("Vector \"{}\" already in space".format(vector.name))
+
         self.space[vector.name] = vector
 
-    def bulkInsert(self, vectors: list, ignoreExisting: bool=True) -> None:
+    def bulkInsert(
+        self,
+        vectors: List[str],
+        tags: Optional[List[List[Union[str, int, float]]]]=None,
+        ignoreExisting: bool=True
+    ) -> None:
         """
         Add vectors to the space
 
-        :param vectors:     List of vector unique names or ids
+        :param vectors:         List of vector unique names or ids
+        :param tags:            List of tags with the same size of vectors: tags of vectors[i] is in tags[i]
+        :param ignoreExisting:  Do not throw an error in case a vector already exists in the space
         """
 
         if not isinstance(vectors, list):
-            raise TypeError("Input must be a list")
+            raise TypeError("Input must be a list of strings")
+
+        if tags and not isinstance(tags, list):
+            raise TypeError("tags must be a list of lists of strings")
+
+        if tags and len(vectors) != len(tags):
+            raise Exception("The number of vectors must match the size of the tags list")
 
         vectors = list(set(vectors))
-        for name in vectors:
+
+        for pos, name in enumerate(vectors):
             try:
                 name = str(name)
+
                 if name in self.space:
                     if not ignoreExisting:
                         raise Exception("Vector \"{}\" already in space".format(name))
+
                     else:
                         continue
-                vector = Vector(name=name, size=self.size)
+
+                vector_tags = tags[pos] if tags else list()
+
+                vector = Vector(name=name, size=self.size, tags=vector_tags)
+
                 self.space[vector.name] = vector
+
             except:
                 raise TypeError("Entries in input list must be instances of primitives")
 
     def remove(self, name: str) -> Vector:
         """
         Remove a vector from the space
 
         :param name:    Vector name or id
         :return:        Vector removed from the space
         """
 
         try:
             name = str(name)
+
             if name in self.space:
-                vector = self.get(name)
+                vector = self.space[name]
+
                 del self.space[name]
+
                 return vector
+
             raise Exception("Vector not in space")
+
         except:
             raise TypeError("Input must be an instance of a primitive")
-    
+
     def find(self, vector: Vector, threshold: float=-1.0) -> Tuple[str, float]:
         """
         Search for the closest vector in space
 
         :param vector:      Vector object
         :param threshold:   Do not consider entries in memory with a distance lower than this threshold
         :return:            Name of the closest vector in space and its distance from the input vector
         """
 
         # Exploit self.findAll() to seach for the best match
         # It will take care of raising exceptions in case of problems with input arguments
         distances, best = self.findAll(vector, threshold=threshold)
+
         return best, distances[best]
 
     def findAll(self, vector: Vector, threshold: float=-1.0) -> Tuple[dict, str]:
         """
         Compute distance of the input vector against all vectors in space
 
         :param vector:      Vector object
         :param threshold:   Do not consider entries in memory with a distance lower than this threshold
         :return:            Dictionary with distances of the input vector against all the other vectors in space, and the name of the closest vector in space
         """
 
         if not isinstance(vector, Vector):
             raise TypeError("Input must be a Vector object")
-        
+
         if self.size != vector.size:
             raise Exception("Space and vectors with different size are not compatible")
 
         if threshold < -1.0 or threshold > 1.0:
             raise ValueError("Threshold cannot be lower than -1.0 or higher than 1.0")
 
         distances = dict()
+
         distance = -1.0
+
         best = None
+
         for v in self.space:
             # Compute cosine similarity
-            dist = self.get(v).dist(vector)
+            dist = self.space[v].dist(vector)
+
             if dist >= threshold:
                 distances[v] = dist
+
                 if distances[v] > distance:
                     best = v
+
                     distance = distances[v]
+
         return distances, best
+
+    def dump(self, to_file: Optional[os.path.abspath]=None) -> None:
+        """
+        Dump the hyperdimensional space to a pickle file
+
+        :param to_file:     Path to the output pickle file
+        """
+
+        if not to_file:
+            # Dump the space to a pickle file in the current working directory
+            # if not file path is provided
+            to_file = os.path.join(os.getcwd, "space.pkl")
+
+        if os.path.isfile(to_file):
+            raise Exception("The output file already exists!\n{}".format(to_file))
+
+        with open(to_file, "wb") as pkl:
+            pickle.dump((self.size, self.space), pkl)
```

