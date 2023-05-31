# Comparing `tmp/graphpro-0.3.3.tar.gz` & `tmp/graphpro-0.3.4.tar.gz`

## Comparing `graphpro-0.3.3.tar` & `graphpro-0.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 graphpro-0.3.3/pytest.ini
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 graphpro-0.3.3/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 graphpro-0.3.3/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 graphpro-0.3.3/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 graphpro-0.3.3/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 graphpro-0.3.3/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 graphpro-0.3.3/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 graphpro-0.3.3/src/graphpro/__init__.py
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 graphpro-0.3.3/src/graphpro/graph.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 graphpro-0.3.3/src/graphpro/graphgen.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 graphpro-0.3.3/src/graphpro/model.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 graphpro-0.3.3/src/graphpro/util/residues.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 graphpro-0.3.3/test/graphpro/graph_test.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 graphpro-0.3.3/test/graphpro/graphgen_test.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 graphpro-0.3.3/test/graphpro/model_test.py
--rw-r--r--   0        0        0   280989 2020-02-02 00:00:00.000000 graphpro-0.3.3/test/testdata/5htc.pdb
--rw-r--r--   0        0        0  3998279 2020-02-02 00:00:00.000000 graphpro-0.3.3/test/testdata/hetnam.pdb
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 graphpro-0.3.3/.gitignore
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 graphpro-0.3.3/README.md
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 graphpro-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 graphpro-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 graphpro-0.3.4/pytest.ini
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 graphpro-0.3.4/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 graphpro-0.3.4/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 graphpro-0.3.4/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 graphpro-0.3.4/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 graphpro-0.3.4/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 graphpro-0.3.4/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 graphpro-0.3.4/src/graphpro/__init__.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 graphpro-0.3.4/src/graphpro/graph.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 graphpro-0.3.4/src/graphpro/graphgen.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 graphpro-0.3.4/src/graphpro/model.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 graphpro-0.3.4/src/graphpro/util/residues.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 graphpro-0.3.4/test/graphpro/graph_test.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 graphpro-0.3.4/test/graphpro/graphgen_test.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 graphpro-0.3.4/test/graphpro/model_test.py
+-rw-r--r--   0        0        0   280989 2020-02-02 00:00:00.000000 graphpro-0.3.4/test/testdata/5htc.pdb
+-rw-r--r--   0        0        0  3998279 2020-02-02 00:00:00.000000 graphpro-0.3.4/test/testdata/hetnam.pdb
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 graphpro-0.3.4/.gitignore
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 graphpro-0.3.4/README.md
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 graphpro-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 graphpro-0.3.4/PKG-INFO
```

### Comparing `graphpro-0.3.3/.pytest_cache/v/cache/nodeids` & `graphpro-0.3.4/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.3/src/graphpro/graph.py` & `graphpro-0.3.4/src/graphpro/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         from networkx.algorithms import community
 
         c_iter = community.girvan_newman(self.graph())
         return  [(community.modularity(self.graph(), com), com) for com in c_iter]
 
     def graph(self) -> nx.Graph:
         """ Returns a networkx G undirected graph with populated attributes """
-        G = nx.from_numpy_matrix(self.distances)
+        G = nx.from_numpy_array(self.distances)
         nx.set_node_attributes(G,self._n_attr)
         return G
     
     def plot(self, 
         figsize: tuple[int,int] = (8,10),
         communities: list[set[int]] = []
         ) -> None:
```

### Comparing `graphpro-0.3.3/src/graphpro/graphgen.py` & `graphpro-0.3.4/src/graphpro/graphgen.py`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.3/src/graphpro/model.py` & `graphpro-0.3.4/src/graphpro/model.py`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.3/test/graphpro/graph_test.py` & `graphpro-0.3.4/test/graphpro/graph_test.py`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.3/test/graphpro/graphgen_test.py` & `graphpro-0.3.4/test/graphpro/graphgen_test.py`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.3/test/testdata/5htc.pdb` & `graphpro-0.3.4/test/testdata/5htc.pdb`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.3/test/testdata/hetnam.pdb` & `graphpro-0.3.4/test/testdata/hetnam.pdb`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.3/pyproject.toml` & `graphpro-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "graphpro"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="Pegerto Fernandez", email="pegerto@gmail.com" },
 ]
 description = "A python module to handle graph protein data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `graphpro-0.3.3/PKG-INFO` & `graphpro-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphpro
-Version: 0.3.3
+Version: 0.3.4
 Summary: A python module to handle graph protein data
 Project-URL: Homepage, https://github.com/pegerto/graphpro
 Project-URL: Bug Tracker, https://github.com/pegerto/graphpro
 Author-email: Pegerto Fernandez <pegerto@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

