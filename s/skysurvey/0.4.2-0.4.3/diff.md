# Comparing `tmp/skysurvey-0.4.2.tar.gz` & `tmp/skysurvey-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skysurvey-0.4.2.tar", last modified: Tue May 30 21:07:02 2023, max compression
+gzip compressed data, was "skysurvey-0.4.3.tar", last modified: Wed May 31 11:53:31 2023, max compression
```

## Comparing `skysurvey-0.4.2.tar` & `skysurvey-0.4.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-30 21:07:02.591515 skysurvey-0.4.2/
--rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-08-10 14:40:58.000000 skysurvey-0.4.2/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      257 2023-05-30 21:07:02.591377 skysurvey-0.4.2/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)     2333 2022-09-14 19:00:29.000000 skysurvey-0.4.2/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-30 21:07:02.591559 skysurvey-0.4.2/setup.cfg
--rw-r--r--   0 rigault   (2358) staff       (20)      632 2023-05-30 21:06:14.000000 skysurvey-0.4.2/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-30 21:07:02.586612 skysurvey-0.4.2/skysurvey/
--rw-r--r--   0 rigault   (2358) staff       (20)       92 2023-05-30 21:06:10.000000 skysurvey-0.4.2/skysurvey/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)      398 2022-08-16 14:00:03.000000 skysurvey-0.4.2/skysurvey/config.py
--rw-r--r--   0 rigault   (2358) staff       (20)    12346 2023-05-30 13:23:34.000000 skysurvey-0.4.2/skysurvey/dag.py
--rw-r--r--   0 rigault   (2358) staff       (20)    26322 2023-05-10 13:33:52.000000 skysurvey-0.4.2/skysurvey/dataset.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-30 21:07:02.588215 skysurvey-0.4.2/skysurvey/survey/
--rw-r--r--   0 rigault   (2358) staff       (20)      101 2022-09-17 12:56:09.000000 skysurvey-0.4.2/skysurvey/survey/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     8645 2023-05-02 20:15:06.000000 skysurvey-0.4.2/skysurvey/survey/core.py
--rw-r--r--   0 rigault   (2358) staff       (20)    10973 2023-01-04 15:12:21.000000 skysurvey-0.4.2/skysurvey/survey/healpix.py
--rw-r--r--   0 rigault   (2358) staff       (20)     5306 2022-12-17 16:44:36.000000 skysurvey-0.4.2/skysurvey/survey/polygon.py
--rw-r--r--   0 rigault   (2358) staff       (20)     1698 2022-12-20 11:13:58.000000 skysurvey-0.4.2/skysurvey/survey/ztf.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-30 21:07:02.591055 skysurvey-0.4.2/skysurvey/target/
--rw-r--r--   0 rigault   (2358) staff       (20)      113 2023-05-05 08:46:40.000000 skysurvey-0.4.2/skysurvey/target/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)    11766 2023-05-05 08:45:44.000000 skysurvey-0.4.2/skysurvey/target/collection.py
--rw-r--r--   0 rigault   (2358) staff       (20)    31265 2023-05-30 21:05:06.000000 skysurvey-0.4.2/skysurvey/target/core.py
--rw-r--r--   0 rigault   (2358) staff       (20)      391 2022-10-06 08:31:16.000000 skysurvey-0.4.2/skysurvey/target/environments.py
--rw-r--r--   0 rigault   (2358) staff       (20)      165 2022-09-17 13:52:22.000000 skysurvey-0.4.2/skysurvey/target/kilonova.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2342 2023-05-07 10:18:11.000000 skysurvey-0.4.2/skysurvey/target/sncc.py
--rw-r--r--   0 rigault   (2358) staff       (20)     9879 2023-02-08 13:19:45.000000 skysurvey-0.4.2/skysurvey/target/snia.py
--rw-r--r--   0 rigault   (2358) staff       (20)      681 2023-05-10 14:57:36.000000 skysurvey-0.4.2/skysurvey/target/stars.py
--rw-r--r--   0 rigault   (2358) staff       (20)     6216 2023-05-04 16:01:10.000000 skysurvey-0.4.2/skysurvey/target/timeserie.py
--rw-r--r--   0 rigault   (2358) staff       (20)    16507 2023-05-26 07:31:27.000000 skysurvey-0.4.2/skysurvey/template.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-30 21:07:02.587095 skysurvey-0.4.2/skysurvey.egg-info/
--rw-r--r--   0 rigault   (2358) staff       (20)      257 2023-05-30 21:07:02.000000 skysurvey-0.4.2/skysurvey.egg-info/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      647 2023-05-30 21:07:02.000000 skysurvey-0.4.2/skysurvey.egg-info/SOURCES.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-05-30 21:07:02.000000 skysurvey-0.4.2/skysurvey.egg-info/dependency_links.txt
--rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-05-30 21:07:02.000000 skysurvey-0.4.2/skysurvey.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-31 11:53:31.032300 skysurvey-0.4.3/
+-rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-08-10 14:40:58.000000 skysurvey-0.4.3/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      257 2023-05-31 11:53:31.032169 skysurvey-0.4.3/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)     2333 2022-09-14 19:00:29.000000 skysurvey-0.4.3/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-31 11:53:31.032341 skysurvey-0.4.3/setup.cfg
+-rw-r--r--   0 rigault   (2358) staff       (20)      632 2023-05-31 11:53:04.000000 skysurvey-0.4.3/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-31 11:53:31.030015 skysurvey-0.4.3/skysurvey/
+-rw-r--r--   0 rigault   (2358) staff       (20)       92 2023-05-31 11:52:58.000000 skysurvey-0.4.3/skysurvey/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      398 2022-08-16 14:00:03.000000 skysurvey-0.4.3/skysurvey/config.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    14150 2023-05-31 11:50:29.000000 skysurvey-0.4.3/skysurvey/dag.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    26322 2023-05-10 13:33:52.000000 skysurvey-0.4.3/skysurvey/dataset.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-31 11:53:31.031025 skysurvey-0.4.3/skysurvey/survey/
+-rw-r--r--   0 rigault   (2358) staff       (20)      101 2022-09-17 12:56:09.000000 skysurvey-0.4.3/skysurvey/survey/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     8645 2023-05-02 20:15:06.000000 skysurvey-0.4.3/skysurvey/survey/core.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    10973 2023-01-04 15:12:21.000000 skysurvey-0.4.3/skysurvey/survey/healpix.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     5306 2022-12-17 16:44:36.000000 skysurvey-0.4.3/skysurvey/survey/polygon.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     1698 2022-12-20 11:13:58.000000 skysurvey-0.4.3/skysurvey/survey/ztf.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-31 11:53:31.032016 skysurvey-0.4.3/skysurvey/target/
+-rw-r--r--   0 rigault   (2358) staff       (20)      113 2023-05-05 08:46:40.000000 skysurvey-0.4.3/skysurvey/target/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    11766 2023-05-05 08:45:44.000000 skysurvey-0.4.3/skysurvey/target/collection.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    31337 2023-05-31 08:44:18.000000 skysurvey-0.4.3/skysurvey/target/core.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      391 2022-10-06 08:31:16.000000 skysurvey-0.4.3/skysurvey/target/environments.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      165 2022-09-17 13:52:22.000000 skysurvey-0.4.3/skysurvey/target/kilonova.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2342 2023-05-07 10:18:11.000000 skysurvey-0.4.3/skysurvey/target/sncc.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     9879 2023-02-08 13:19:45.000000 skysurvey-0.4.3/skysurvey/target/snia.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      681 2023-05-10 14:57:36.000000 skysurvey-0.4.3/skysurvey/target/stars.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     6216 2023-05-04 16:01:10.000000 skysurvey-0.4.3/skysurvey/target/timeserie.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    16507 2023-05-26 07:31:27.000000 skysurvey-0.4.3/skysurvey/template.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-31 11:53:31.030476 skysurvey-0.4.3/skysurvey.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)      257 2023-05-31 11:53:30.000000 skysurvey-0.4.3/skysurvey.egg-info/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      647 2023-05-31 11:53:31.000000 skysurvey-0.4.3/skysurvey.egg-info/SOURCES.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2023-05-31 11:53:30.000000 skysurvey-0.4.3/skysurvey.egg-info/dependency_links.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)       10 2023-05-31 11:53:30.000000 skysurvey-0.4.3/skysurvey.egg-info/top_level.txt
```

### Comparing `skysurvey-0.4.2/LICENSE` & `skysurvey-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.2/README.md` & `skysurvey-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.2/setup.py` & `skysurvey-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from distutils.core import setup
 from setuptools import setup, find_packages
 
 
 packages = find_packages()
 
-VERSION = '0.4.2'
+VERSION = '0.4.3'
         
 setup(name='skysurvey',
       version=VERSION,
       description='Simulating Transient in the sky and how to observe them',
       author='Mickael Rigault',
       author_email='m.rigault@ipnl.in2p3.fr',
       url='https://github.com/MickaelRigault/skysurvey',
```

### Comparing `skysurvey-0.4.2/skysurvey/dag.py` & `skysurvey-0.4.3/skysurvey/dag.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,17 +51,73 @@
         import pprint
         return pprint.pformat(self.model, sort_dicts=False)
 
     def __repr__(self):
         """ """
         return self.__str__()
 
+
+    def to_graph(self, engine="networkx"):
+        """ converts the model into another graph library object 
+
+        Parameters
+        ----------
+        engine: string
+            Implemented:
+            - NetworkX (networkx.org/documentation/stable/tutorial.html)
+            - Graphviz (https://pygraphviz.github.io/documentation/stable/index.html)
+
+        Return
+        ------
+        Graph instance
+            a new instance object.
+        """
+        if engine == "networkx":
+            import networkx as nx
+            graph = nx.Graph()
+        elif engine in ["graphviz", "pygraphviz"]:
+            import pygraphviz as pgv
+            graph = pgv.AGraph(directed=True, strict=True)
+        else:
+            raise NotImplementedError(f"engine {engine} is not implemented. networkx and graphviz are")
+
+        # Nodes and Edges
+        for name in self.entries:
+            graph.add_node(name)
+    
+        for name, to_name in self.entry_inputof.items():
+            graph.add_edge(name, to_name)
+
+        return graph
+    
+    def to_networkx(self):
+        """ shortcut to to_graph('networkx') """
+        return self.to_graph(engine="networkx")
+
+    def to_graphviz(self):
+        """ shortcut to to_graph('graphviz') """
+        return self.to_graph(engine="graphviz")
+
+
     # ============ #
     #   Method     #
     # ============ #
+    def visualize(self, fileout="tmp_modelvisualize.svg"):
+        """ """
+        from IPython.display import SVG
+        
+        ag = self.to_graphviz()
+        ag.graph_attr["epsilon"] = "0.001"
+        
+        ag.layout("dot")  # layout with dot
+        ag.draw(fileout)
+        return SVG(fileout)
+
+
+    
     def get_model(self, **kwargs):
         """ get a copy of the model 
         
         Parameters
         ----------
 
         **kwargs can change the model entry parameters
@@ -154,17 +210,30 @@
             # all names individually
             _ = [forward_entries.append(name_) for name_ in list(leads_to_changing.values)]
             leads_to_changing = inputs_of.loc[inputs_of.index.isin(leads_to_changing)]
 
         return forward_entries
 
 
-    def get_modeldf(self):
-        """ """
+    def get_modeldf(self, explode=True):
+        """ get a pandas.DataFrame version of the model dict
+
+        Parameters
+        ----------
+        explode: bool
+            should the input entry be exploded ?
+
+        Returns
+        -------
+        pandas.DataFrame
+        """
         modeldf = modeldict_to_modeldf(self.model)
+        if not explode:
+            return modeldf.explode("entry").set_index("entry")
+        
         return modeldf.explode("entry").explode("input").set_index("entry")
         
     # ============ #
     #  Drawers     #
     # ============ #
     def redraw_from(self, name, data, incl_name=True, size=None, **kwargs):
         """ re-draw the data starting from the given entry name.
@@ -386,12 +455,7 @@
     @property
     def entry_inputof(self):
         """ """
         # maybe a bit overcomplicated...
         modeldf = self.get_modeldf()
         return modeldf[~modeldf["input"].isna()].reset_index().set_index("input")["entry"]
         
-
-def get_modeldf(self):
-    """ """
-    modeldf = modeldict_to_modeldf(self.model)
-    return modeldf.explode("name").explode("input")
```

### Comparing `skysurvey-0.4.2/skysurvey/dataset.py` & `skysurvey-0.4.3/skysurvey/dataset.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.2/skysurvey/survey/core.py` & `skysurvey-0.4.3/skysurvey/survey/core.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.2/skysurvey/survey/healpix.py` & `skysurvey-0.4.3/skysurvey/survey/healpix.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.2/skysurvey/survey/polygon.py` & `skysurvey-0.4.3/skysurvey/survey/polygon.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.2/skysurvey/survey/ztf.py` & `skysurvey-0.4.3/skysurvey/survey/ztf.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.2/skysurvey/target/collection.py` & `skysurvey-0.4.3/skysurvey/target/collection.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.2/skysurvey/target/core.py` & `skysurvey-0.4.3/skysurvey/target/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,44 +287,47 @@
             to the requested zeropoint. Return value is `float` if all
             input parameters are scalars, `~numpy.ndarray` otherwise.
         """
         template = self.get_target_template(index)
         return template.bandflux(band, template.get('t0')+phase, zp=zp, zpsys=zpsys)
 
 
-    def clone_target_at_redshifts(self, index, redshifts, as_dataframe=False):
+    def clone_target_change_entry(self, index, name, values, as_dataframe=False):
         """ get a clone of the given target at the given redshifts.
         This: 
         (1) copies the index entries, 
-        (2) sets the redshift to the input values
-        (3) redraw the model starting from the redshift (creating a new dataframe)
+        (2) sets the `name` to the input `values`
+        (3) redraw the model starting from `name` (creating a new dataframe)
         (4, optional) sets a new instance with the updated dataframe
         
 
         Parameters
         ----------
         index: 
             index of a target (see self.data.index)
+            
+        name: str
+            name of the entry to change
 
-        redshift: list, array
-            new redshifts to clone this target to
+        values: list, array
+            new values for this entry.
 
         as_dataframe: bool
             should this return the created new dataframe (True)
             or a new instance (False)
 
         Returns
         -------
         instance or DataFrame
         """
         dd = self.data.loc[index].to_frame().T
-        dd.loc[index, "z"] = redshifts
-        dd = dd.explode("z")
-        dd["z"] = dd["z"].astype(float)
-        data = self.model.redraw_from("z", dd, incl_name=False)
+        dd.loc[index, name] = np.atleast_1d(values)
+        dd = dd.explode(name)
+        dd[name] = dd[name].astype(float)
+        data = self.model.redraw_from(name, dd, incl_name=False)
         if as_dataframe:
             return data
         
         return self.__class__.from_data(data)
     
     # -------------- #
     #   Getter       #
```

### Comparing `skysurvey-0.4.2/skysurvey/target/sncc.py` & `skysurvey-0.4.3/skysurvey/target/sncc.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.2/skysurvey/target/snia.py` & `skysurvey-0.4.3/skysurvey/target/snia.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.2/skysurvey/target/stars.py` & `skysurvey-0.4.3/skysurvey/target/stars.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.2/skysurvey/target/timeserie.py` & `skysurvey-0.4.3/skysurvey/target/timeserie.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.2/skysurvey/template.py` & `skysurvey-0.4.3/skysurvey/template.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.4.2/skysurvey.egg-info/SOURCES.txt` & `skysurvey-0.4.3/skysurvey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

