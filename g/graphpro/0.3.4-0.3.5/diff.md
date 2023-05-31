# Comparing `tmp/graphpro-0.3.4.tar.gz` & `tmp/graphpro-0.3.5.tar.gz`

## Comparing `graphpro-0.3.4.tar` & `graphpro-0.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 graphpro-0.3.4/pytest.ini
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 graphpro-0.3.4/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 graphpro-0.3.4/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 graphpro-0.3.4/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 graphpro-0.3.4/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 graphpro-0.3.4/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 graphpro-0.3.4/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 graphpro-0.3.4/src/graphpro/__init__.py
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 graphpro-0.3.4/src/graphpro/graph.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 graphpro-0.3.4/src/graphpro/graphgen.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 graphpro-0.3.4/src/graphpro/model.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 graphpro-0.3.4/src/graphpro/util/residues.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 graphpro-0.3.4/test/graphpro/graph_test.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 graphpro-0.3.4/test/graphpro/graphgen_test.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 graphpro-0.3.4/test/graphpro/model_test.py
--rw-r--r--   0        0        0   280989 2020-02-02 00:00:00.000000 graphpro-0.3.4/test/testdata/5htc.pdb
--rw-r--r--   0        0        0  3998279 2020-02-02 00:00:00.000000 graphpro-0.3.4/test/testdata/hetnam.pdb
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 graphpro-0.3.4/.gitignore
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 graphpro-0.3.4/README.md
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 graphpro-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 graphpro-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 graphpro-0.3.5/pytest.ini
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 graphpro-0.3.5/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 graphpro-0.3.5/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 graphpro-0.3.5/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 graphpro-0.3.5/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 graphpro-0.3.5/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 graphpro-0.3.5/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 graphpro-0.3.5/src/graphpro/__init__.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 graphpro-0.3.5/src/graphpro/graph.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 graphpro-0.3.5/src/graphpro/graphgen.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 graphpro-0.3.5/src/graphpro/model.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 graphpro-0.3.5/src/graphpro/util/residues.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 graphpro-0.3.5/test/graphpro/graph_test.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 graphpro-0.3.5/test/graphpro/graphgen_test.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 graphpro-0.3.5/test/graphpro/model_test.py
+-rw-r--r--   0        0        0   280989 2020-02-02 00:00:00.000000 graphpro-0.3.5/test/testdata/5htc.pdb
+-rw-r--r--   0        0        0  3998279 2020-02-02 00:00:00.000000 graphpro-0.3.5/test/testdata/hetnam.pdb
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 graphpro-0.3.5/.gitignore
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 graphpro-0.3.5/README.md
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 graphpro-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 graphpro-0.3.5/PKG-INFO
```

### Comparing `graphpro-0.3.4/.pytest_cache/v/cache/nodeids` & `graphpro-0.3.5/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.4/src/graphpro/graph.py` & `graphpro-0.3.5/src/graphpro/graph.py`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.4/src/graphpro/graphgen.py` & `graphpro-0.3.5/src/graphpro/graphgen.py`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.4/src/graphpro/model.py` & `graphpro-0.3.5/src/graphpro/model.py`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.4/test/graphpro/graph_test.py` & `graphpro-0.3.5/test/graphpro/graph_test.py`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.4/test/graphpro/graphgen_test.py` & `graphpro-0.3.5/test/graphpro/graphgen_test.py`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.4/test/testdata/5htc.pdb` & `graphpro-0.3.5/test/testdata/5htc.pdb`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.4/test/testdata/hetnam.pdb` & `graphpro-0.3.5/test/testdata/hetnam.pdb`

 * *Files identical despite different names*

### Comparing `graphpro-0.3.4/pyproject.toml` & `graphpro-0.3.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "graphpro"
-version = "0.3.4"
+version = "0.3.5"
 authors = [
   { name="Pegerto Fernandez", email="pegerto@gmail.com" },
 ]
 description = "A python module to handle graph protein data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -13,19 +13,23 @@
     "Operating System :: OS Independent",
 
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Scientific/Engineering :: Artificial Intelligence"
 ]
 
+dependencies = [
+  'MDAnalisys >= 2.5.0',
+]
+
+
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
-
 [tool.hatch.build.targets.wheel]
 packages = ["src/graphpro"]
 
 [tool.pytest.ini_options]
 pythonpath = [
   "src"
 ]
```

### Comparing `graphpro-0.3.4/PKG-INFO` & `graphpro-0.3.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: graphpro
-Version: 0.3.4
+Version: 0.3.5
 Summary: A python module to handle graph protein data
 Project-URL: Homepage, https://github.com/pegerto/graphpro
 Project-URL: Bug Tracker, https://github.com/pegerto/graphpro
 Author-email: Pegerto Fernandez <pegerto@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
+Requires-Dist: mdanalisys>=2.5.0
 Description-Content-Type: text/markdown
 
 # graphpro
```

