# Comparing `tmp/brainwalk-0.0.1.tar.gz` & `tmp/brainwalk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainwalk-0.0.1.tar", last modified: Wed May 31 19:58:37 2023, max compression
+gzip compressed data, was "brainwalk-0.0.2.tar", last modified: Wed May 31 20:55:55 2023, max compression
```

## Comparing `brainwalk-0.0.1.tar` & `brainwalk-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tesfaasmara   (501) staff       (20)        0 2023-05-31 19:58:37.290529 brainwalk-0.0.1/
--rw-rw-r--   0 tesfaasmara   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 brainwalk-0.0.1/LICENSE
--rw-rw-r--   0 tesfaasmara   (501) staff       (20)      111 2023-04-27 10:12:58.000000 brainwalk-0.0.1/MANIFEST.in
--rw-r--r--   0 tesfaasmara   (501) staff       (20)     1104 2023-05-31 19:58:37.290387 brainwalk-0.0.1/PKG-INFO
--rw-r--r--   0 tesfaasmara   (501) staff       (20)      296 2023-05-31 19:57:04.000000 brainwalk-0.0.1/README.md
-drwxr-xr-x   0 tesfaasmara   (501) staff       (20)        0 2023-05-31 19:58:37.288762 brainwalk-0.0.1/brainwalk/
--rw-r--r--   0 tesfaasmara   (501) staff       (20)       22 2023-05-31 19:56:53.000000 brainwalk-0.0.1/brainwalk/__init__.py
--rw-r--r--   0 tesfaasmara   (501) staff       (20)     2612 2023-05-31 19:56:53.000000 brainwalk-0.0.1/brainwalk/_modidx.py
--rw-r--r--   0 tesfaasmara   (501) staff       (20)     9431 2023-05-31 19:56:53.000000 brainwalk-0.0.1/brainwalk/core.py
-drwxr-xr-x   0 tesfaasmara   (501) staff       (20)        0 2023-05-31 19:58:37.290179 brainwalk-0.0.1/brainwalk.egg-info/
--rw-r--r--   0 tesfaasmara   (501) staff       (20)     1104 2023-05-31 19:58:37.000000 brainwalk-0.0.1/brainwalk.egg-info/PKG-INFO
--rw-r--r--   0 tesfaasmara   (501) staff       (20)      344 2023-05-31 19:58:37.000000 brainwalk-0.0.1/brainwalk.egg-info/SOURCES.txt
--rw-r--r--   0 tesfaasmara   (501) staff       (20)        1 2023-05-31 19:58:37.000000 brainwalk-0.0.1/brainwalk.egg-info/dependency_links.txt
--rw-r--r--   0 tesfaasmara   (501) staff       (20)       40 2023-05-31 19:58:37.000000 brainwalk-0.0.1/brainwalk.egg-info/entry_points.txt
--rw-r--r--   0 tesfaasmara   (501) staff       (20)        1 2023-05-31 19:57:52.000000 brainwalk-0.0.1/brainwalk.egg-info/not-zip-safe
--rw-r--r--   0 tesfaasmara   (501) staff       (20)       42 2023-05-31 19:58:37.000000 brainwalk-0.0.1/brainwalk.egg-info/requires.txt
--rw-r--r--   0 tesfaasmara   (501) staff       (20)       10 2023-05-31 19:58:37.000000 brainwalk-0.0.1/brainwalk.egg-info/top_level.txt
--rw-r--r--   0 tesfaasmara   (501) staff       (20)     1006 2023-05-31 19:52:21.000000 brainwalk-0.0.1/settings.ini
--rw-r--r--   0 tesfaasmara   (501) staff       (20)       38 2023-05-31 19:58:37.290571 brainwalk-0.0.1/setup.cfg
--rw-rw-r--   0 tesfaasmara   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 brainwalk-0.0.1/setup.py
+drwxr-xr-x   0 tesfaasmara   (501) staff       (20)        0 2023-05-31 20:55:55.542688 brainwalk-0.0.2/
+-rw-rw-r--   0 tesfaasmara   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 brainwalk-0.0.2/LICENSE
+-rw-rw-r--   0 tesfaasmara   (501) staff       (20)      111 2023-04-27 10:12:58.000000 brainwalk-0.0.2/MANIFEST.in
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)     2330 2023-05-31 20:55:55.542556 brainwalk-0.0.2/PKG-INFO
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)     1522 2023-05-31 20:44:10.000000 brainwalk-0.0.2/README.md
+drwxr-xr-x   0 tesfaasmara   (501) staff       (20)        0 2023-05-31 20:55:55.541241 brainwalk-0.0.2/brainwalk/
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)       22 2023-05-31 20:55:39.000000 brainwalk-0.0.2/brainwalk/__init__.py
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)     2718 2023-05-31 20:55:39.000000 brainwalk-0.0.2/brainwalk/_modidx.py
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)     9935 2023-05-31 20:55:39.000000 brainwalk-0.0.2/brainwalk/core.py
+drwxr-xr-x   0 tesfaasmara   (501) staff       (20)        0 2023-05-31 20:55:55.542367 brainwalk-0.0.2/brainwalk.egg-info/
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)     2330 2023-05-31 20:55:55.000000 brainwalk-0.0.2/brainwalk.egg-info/PKG-INFO
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)      344 2023-05-31 20:55:55.000000 brainwalk-0.0.2/brainwalk.egg-info/SOURCES.txt
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)        1 2023-05-31 20:55:55.000000 brainwalk-0.0.2/brainwalk.egg-info/dependency_links.txt
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)       40 2023-05-31 20:55:55.000000 brainwalk-0.0.2/brainwalk.egg-info/entry_points.txt
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)        1 2023-05-31 19:57:52.000000 brainwalk-0.0.2/brainwalk.egg-info/not-zip-safe
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)       56 2023-05-31 20:55:55.000000 brainwalk-0.0.2/brainwalk.egg-info/requires.txt
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)       10 2023-05-31 20:55:55.000000 brainwalk-0.0.2/brainwalk.egg-info/top_level.txt
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)      906 2023-05-31 20:55:39.000000 brainwalk-0.0.2/settings.ini
+-rw-r--r--   0 tesfaasmara   (501) staff       (20)       38 2023-05-31 20:55:55.542725 brainwalk-0.0.2/setup.cfg
+-rw-rw-r--   0 tesfaasmara   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 brainwalk-0.0.2/setup.py
```

### Comparing `brainwalk-0.0.1/LICENSE` & `brainwalk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `brainwalk-0.0.1/brainwalk/_modidx.py` & `brainwalk-0.0.2/brainwalk/_modidx.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,15 @@
                 'lib_path': 'brainwalk'},
   'syms': { 'brainwalk.core': { 'brainwalk.core.WireWalk': ('core.html#wirewalk', 'brainwalk/core.py'),
                                 'brainwalk.core.WireWalk.__init__': ('core.html#__init__', 'brainwalk/core.py'),
                                 'brainwalk.core.WireWalk.fit': ('core.html#fit', 'brainwalk/core.py'),
                                 'brainwalk.core.WireWalk.generate_transition': ('core.html#generate_transition', 'brainwalk/core.py'),
                                 'brainwalk.core.WireWalk.generate_walks': ('core.html#generate_walks', 'brainwalk/core.py'),
                                 'brainwalk.core.adamic_adar': ('core.html#adamic_adar', 'brainwalk/core.py'),
+                                'brainwalk.core.brainwave': ('core.html#brainwave', 'brainwalk/core.py'),
                                 'brainwalk.core.common_neighbors': ('core.html#common_neighbors', 'brainwalk/core.py'),
                                 'brainwalk.core.generate_walks_for_node': ('core.html#generate_walks_for_node', 'brainwalk/core.py'),
                                 'brainwalk.core.hub_depressed': ('core.html#hub_depressed', 'brainwalk/core.py'),
                                 'brainwalk.core.hub_promoted': ('core.html#hub_promoted', 'brainwalk/core.py'),
                                 'brainwalk.core.jaccard_coefficient': ('core.html#jaccard_coefficient', 'brainwalk/core.py'),
                                 'brainwalk.core.levenshtein': ('core.html#levenshtein', 'brainwalk/core.py'),
                                 'brainwalk.core.lhn_index': ('core.html#lhn_index', 'brainwalk/core.py'),
```

### Comparing `brainwalk-0.0.1/brainwalk/core.py` & `brainwalk-0.0.2/brainwalk/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
 __all__ = ['max_flow', 'min_cost_max_flow', 'levenshtein', 'jaccard_coefficient', 'common_neighbors', 'lhn_index',
            'preferential_attachment', 'hub_promoted', 'hub_depressed', 'salton_index', 'sorenson_index', 'tversky',
-           'adamic_adar', 'resource_allocation', 'generate_walks_for_node', 'WireWalk']
+           'adamic_adar', 'resource_allocation', 'generate_walks_for_node', 'WireWalk', 'brainwave']
 
 # %% ../nbs/00_core.ipynb 2
 import numpy as np
 import networkx as nx
 import math
 import editdistance
 
@@ -280,7 +280,24 @@
             
         return walks
 
     def fit(self, transformation: callable) -> gensim.models.Word2Vec:
         transition_probability_matrix = self.generate_transition(transformation)
         walks = self.generate_walks(transition_probability_matrix)
         return gensim.models.Word2Vec(walks,window=self.window, workers=self.workers, vector_size=self.dimensions)
+
+# %% ../nbs/00_core.ipynb 4
+def brainwave(vault_dir, transformation, dimensions = 128, window = 10, walk_length = 80, num_walks = 10, workers = 1):
+    import obsidiantools.api as otools
+    from brainwalk.core import WireWalk
+
+    vault = otools.Vault(vault_dir).connect().gather()
+
+    graph = vault.graph
+
+    # Instantiate a WireWalk object
+    wireWalk = WireWalk(graph, dimensions, window, walk_length, num_walks, workers)
+
+    model = wireWalk.fit(transformation)
+
+    return model
+
```

### Comparing `brainwalk-0.0.1/setup.py` & `brainwalk-0.0.2/setup.py`

 * *Files identical despite different names*

