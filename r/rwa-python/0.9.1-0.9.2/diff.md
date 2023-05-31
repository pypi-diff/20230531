# Comparing `tmp/rwa-python-0.9.1.tar.gz` & `tmp/rwa-python-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwa-python-0.9.1.tar", last modified: Sat Mar 12 16:04:50 2022, max compression
+gzip compressed data, was "rwa-python-0.9.2.tar", last modified: Wed May 31 20:27:06 2023, max compression
```

## Comparing `rwa-python-0.9.1.tar` & `rwa-python-0.9.2.tar`

### file list

```diff
@@ -1,21 +1,27 @@
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2022-03-12 16:04:50.517895 rwa-python-0.9.1/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    11369 2020-10-07 12:38:42.000000 rwa-python-0.9.1/LICENSE
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3375 2022-03-12 16:04:50.517895 rwa-python-0.9.1/PKG-INFO
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     2663 2022-03-07 15:32:13.000000 rwa-python-0.9.1/README.rst
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2022-03-12 16:04:50.517895 rwa-python-0.9.1/rwa/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      425 2020-10-07 12:38:42.000000 rwa-python-0.9.1/rwa/__init__.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    35633 2021-08-16 11:49:25.000000 rwa-python-0.9.1/rwa/generic.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    15106 2022-03-12 15:07:56.000000 rwa-python-0.9.1/rwa/hdf5.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    10160 2022-03-08 18:15:12.000000 rwa-python-0.9.1/rwa/lazy.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    13377 2022-03-07 14:54:11.000000 rwa-python-0.9.1/rwa/pandas.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     7378 2022-03-12 15:31:04.000000 rwa-python-0.9.1/rwa/scipy.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     9967 2020-10-07 12:38:42.000000 rwa-python-0.9.1/rwa/sequence.py
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)    18539 2022-03-11 11:43:41.000000 rwa-python-0.9.1/rwa/storable.py
-drwxrwxr-x   0 flaurent  (1000) flaurent  (1000)        0 2022-03-12 16:04:50.517895 rwa-python-0.9.1/rwa_python.egg-info/
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     3375 2022-03-12 16:04:50.000000 rwa-python-0.9.1/rwa_python.egg-info/PKG-INFO
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)      310 2022-03-12 16:04:50.000000 rwa-python-0.9.1/rwa_python.egg-info/SOURCES.txt
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        1 2022-03-12 16:04:50.000000 rwa-python-0.9.1/rwa_python.egg-info/dependency_links.txt
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)       28 2022-03-12 16:04:50.000000 rwa-python-0.9.1/rwa_python.egg-info/requires.txt
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)        4 2022-03-12 16:04:50.000000 rwa-python-0.9.1/rwa_python.egg-info/top_level.txt
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)       38 2022-03-12 16:04:50.517895 rwa-python-0.9.1/setup.cfg
--rw-rw-r--   0 flaurent  (1000) flaurent  (1000)     1569 2022-03-12 16:02:47.000000 rwa-python-0.9.1/setup.py
+drwxr-xr-x   0 flaurent  (1000) flaurent  (1000)        0 2023-05-31 20:27:06.070110 rwa-python-0.9.2/
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)    11369 2023-05-31 09:33:20.000000 rwa-python-0.9.2/LICENSE
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     3406 2023-05-31 20:27:06.070110 rwa-python-0.9.2/PKG-INFO
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     2663 2023-05-31 09:33:20.000000 rwa-python-0.9.2/README.rst
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)      500 2023-05-31 10:36:26.000000 rwa-python-0.9.2/pyproject.toml
+drwxr-xr-x   0 flaurent  (1000) flaurent  (1000)        0 2023-05-31 20:27:06.066110 rwa-python-0.9.2/rwa/
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)      425 2023-05-31 09:33:20.000000 rwa-python-0.9.2/rwa/__init__.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)    35975 2023-05-31 19:38:43.000000 rwa-python-0.9.2/rwa/generic.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)    15106 2023-05-31 09:33:20.000000 rwa-python-0.9.2/rwa/hdf5.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)    10160 2023-05-31 09:33:20.000000 rwa-python-0.9.2/rwa/lazy.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)    14199 2023-05-31 11:15:17.000000 rwa-python-0.9.2/rwa/pandas.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     7715 2023-05-31 19:38:43.000000 rwa-python-0.9.2/rwa/scipy.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     9967 2023-05-31 09:33:20.000000 rwa-python-0.9.2/rwa/sequence.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)    18539 2023-05-31 09:33:20.000000 rwa-python-0.9.2/rwa/storable.py
+drwxr-xr-x   0 flaurent  (1000) flaurent  (1000)        0 2023-05-31 20:27:06.066110 rwa-python-0.9.2/rwa_python.egg-info/
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     3406 2023-05-31 20:27:06.000000 rwa-python-0.9.2/rwa_python.egg-info/PKG-INFO
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)      422 2023-05-31 20:27:06.000000 rwa-python-0.9.2/rwa_python.egg-info/SOURCES.txt
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)        1 2023-05-31 20:27:06.000000 rwa-python-0.9.2/rwa_python.egg-info/dependency_links.txt
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)       28 2023-05-31 20:27:06.000000 rwa-python-0.9.2/rwa_python.egg-info/requires.txt
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)        4 2023-05-31 20:27:06.000000 rwa-python-0.9.2/rwa_python.egg-info/top_level.txt
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)       38 2023-05-31 20:27:06.070110 rwa-python-0.9.2/setup.cfg
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     1521 2023-05-31 19:39:28.000000 rwa-python-0.9.2/setup.py
+drwxr-xr-x   0 flaurent  (1000) flaurent  (1000)        0 2023-05-31 20:27:06.070110 rwa-python-0.9.2/tests/
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     2729 2023-05-31 09:33:20.000000 rwa-python-0.9.2/tests/test_autoserial_hdf5.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     4288 2023-05-31 09:33:20.000000 rwa-python-0.9.2/tests/test_native_hdf5.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     9146 2023-05-31 19:59:27.000000 rwa-python-0.9.2/tests/test_pandas.py
+-rw-r--r--   0 flaurent  (1000) flaurent  (1000)     3904 2023-05-31 11:43:58.000000 rwa-python-0.9.2/tests/test_scipy.py
```

### Comparing `rwa-python-0.9.1/LICENSE` & `rwa-python-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rwa-python-0.9.1/PKG-INFO` & `rwa-python-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: rwa-python
-Version: 0.9.1
+Version: 0.9.2
 Summary: HDF5-based serialization library for Python datatypes
 Home-page: https://github.com/DecBayComp/RWA-python
 Author: François Laurent
 Author-email: francois.laurent@pasteur.fr
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
 .. image:: https://img.shields.io/badge/docs-latest-blue.svg
    :target: https://rwa-python.readthedocs.io/en/latest/
 .. image:: https://github.com/DecBayComp/RWA-python/actions/workflows/ci.yml/badge.svg
    :target: https://github.com/DecBayComp/RWA-python/actions/workflows/ci.yml
 .. image:: https://codecov.io/gh/DecBayComp/RWA-python/branch/master/graph/badge.svg
@@ -100,9 +100,7 @@
 
 
 See also
 --------
 
 **RWA-python** is on `readthedocs <https://rwa-python.readthedocs.io/en/latest/>`_.
 
-
-
```

### Comparing `rwa-python-0.9.1/README.rst` & `rwa-python-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `rwa-python-0.9.1/rwa/generic.py` & `rwa-python-0.9.2/rwa/generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -585,26 +585,29 @@
             raise
         else:
             e_new = TypeError("{}:\n\t{}".format(msg, e.args[0]))
             raise e_new
 
 
 # peeks
-def default_peek(python_type, exposes):
+def default_peek(python_type, exposes, excess_attributes=[]):
     """
     Autoserializer factory.
 
     Works best in Python 3.
 
     Arguments:
 
         python_type (type): type constructor.
 
         exposes (iterable): sequence of attributes.
 
+        excess_attributes (iterable): set of unrequired attributes that might
+            have been serialized by other versions of the provider library.
+
     Returns:
 
         callable: deserializer (`peek` routine).
 
     """
     with_args = False
     make = python_type
@@ -637,29 +640,32 @@
         def peek(store, container, _stack=None):
             obj = make()
             for attr in container:
                 val = store.peek(attr, container, _stack=_stack)
                 try:
                     setattr(obj, attr, val)
                 except AttributeError:
-                    raise missing(attr)
+                    if attr not in excess_attributes:
+                        print(excess_attributes)
+                        raise missing(attr)
             return obj
     else:
         def peek(store, container, _stack=None):
             obj = make()
             for attr in exposes: # force order instead of iterating over `container`
                 #print((attr, attr in container)) # debugging
                 if attr in container:
                     val = store.peek(attr, container, _stack=_stack)
                 else:
                     val = None
                 try:
                     setattr(obj, attr, val)
                 except AttributeError:
-                    raise missing(attr)
+                    if attr not in excess_attributes:
+                        raise missing(attr)
             return obj
     return peek
 
 def unsafe_peek(init):
     """
     Deserialize all the attributes available in the container and pass them in the same order
     as they come in the container.
```

### Comparing `rwa-python-0.9.1/rwa/hdf5.py` & `rwa-python-0.9.2/rwa/hdf5.py`

 * *Files identical despite different names*

### Comparing `rwa-python-0.9.1/rwa/lazy.py` & `rwa-python-0.9.2/rwa/lazy.py`

 * *Files identical despite different names*

### Comparing `rwa-python-0.9.1/rwa/pandas.py` & `rwa-python-0.9.2/rwa/pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,26 +148,54 @@
                 attr = tuple( tuple(item) for item in getattr(ix, attrname) )
                 service.poke(attrname, attr, container, *args, **kwargs)
         attrname = 'names'
         attr = tuple( getattr(ix, attrname) )
         service.poke(attrname, attr, container, *args, **kwargs)
 
     try:
+        # Int64Index is missing in 2.0.2
+        pandas_Int64Index = pandas.Int64Index
+        peek_int64index = peek_numerical_index(pandas.Int64Index)
+    except AttributeError:
+        # convert Int64Index into Index
+        class pandas_Int64Index(object):
+            """
+            Placeholder type.
+            """
+            __slot__ = ()
+            pass
+        peek_int64index = peek_numerical_index(pandas.Index, lambda a: a.astype(np.int64))
+
+    try:
         # UInt64Index is missing in 0.17.1
         pandas_UInt64Index = pandas.UInt64Index
         peek_uint64index = peek_numerical_index(pandas.UInt64Index)
     except AttributeError:
         # convert UInt64 into Int64
         class pandas_UInt64Index(object):
             """
             Placeholder type.
             """
             __slot__ = ()
             pass
-        peek_uint64index = peek_numerical_index(pandas.Int64Index, lambda a: a.astype(np.int64))
+        peek_uint64index = peek_int64index
+
+    try:
+        # Float64Index is missing in 2.0.2
+        pandas_Float64Index = pandas.Float64Index
+        peek_float64index = peek_numerical_index(pandas.Float64Index)
+    except AttributeError:
+        # convert Float64Index into Index
+        class pandas_Float64Index(object):
+            """
+            Placeholder type.
+            """
+            __slot__ = ()
+            pass
+        peek_float64index = peek_numerical_index(pandas.Index, lambda a: a.astype(np.float64))
 
     if True:
         poke_rangeindex = poke([('start','_start'), ('stop','_stop'), ('step','_step'), 'name'])
     else:
         poke_rangeindex = poke(['_start', '_stop', '_step', 'name'])
     try:
         # RangeIndex is missing in 0.17.1
@@ -205,27 +233,25 @@
 
     # some Pandas types have moved several times; force the key
     pandas_storables = [ \
         Storable(pandas.Index, \
          key='Python.pandas.core.index.Index', \
          handlers=StorableHandler(poke=poke_index, peek=peek_index, \
             peek_option='pandas.index.force_unicode')), \
-        Storable(pandas.Int64Index, \
+        Storable(pandas_Int64Index, \
          key='Python.pandas.core.index.Int64Index', \
-         handlers=StorableHandler(poke=poke_index, \
-            peek=peek_numerical_index(pandas.Int64Index), \
+         handlers=StorableHandler(poke=poke_index, peek=peek_int64index, \
             peek_option='pandas.index.force_unicode')), \
         Storable(pandas_UInt64Index, \
          key='Python.pandas.core.index.UInt64Index', \
          handlers=StorableHandler(poke=poke_index, peek=peek_uint64index, \
             peek_option='pandas.index.force_unicode')), \
-        Storable(pandas.Float64Index, \
+        Storable(pandas_Float64Index, \
          key='Python.pandas.core.index.Float64Index', \
-         handlers=StorableHandler(poke=poke_index, \
-            peek=peek_numerical_index(pandas.Float64Index), \
+         handlers=StorableHandler(poke=poke_index, peek=peek_float64index, \
             peek_option='pandas.index.force_unicode')), \
         Storable(pandas_RangeIndex, \
          key='Python.pandas.core.index.RangeIndex', \
          handlers=StorableHandler(poke=poke_rangeindex, peek=unicode_index(peek_rangeindex), \
              peek_option='pandas.index.force_unicode')), \
         Storable(pandas.MultiIndex, \
          key='Python.pandas.core.index.MultiIndex', \
```

### Comparing `rwa-python-0.9.1/rwa/scipy.py` & `rwa-python-0.9.2/rwa/scipy.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,21 +100,25 @@
     Voronoi_exposes = ['points', 'vertices', 'ridge_points', 'ridge_vertices', 'regions', 'point_region']
 
     Delaunay_v1_exposes = [ '_points', 'coplanar', 'equations', 'good', 'max_bound', 'min_bound', 'ndim', 'neighbors', 'npoints', 'nsimplex', 'paraboloid_scale', 'paraboloid_shift', 'simplices', 'vertices' ]
     ConvexHull_v1_exposes = [ '_points', '_vertices', 'area', 'coplanar', 'equations', 'max_bound', 'min_bound', 'ndim', 'neighbors', 'npoints', 'nsimplex', 'simplices', 'volume' ]
     Voronoi_v1_exposes = [ '_points', 'max_bound', 'min_bound', 'ndim', 'npoints', 'point_region', 'regions', 'ridge_points', 'ridge_vertices', 'vertices' ]
 
     _scipy_spatial_types = [
-        ('Delaunay', Delaunay_exposes, Delaunay_v1_exposes, ('simplices', )),
+        ('Delaunay', Delaunay_exposes, Delaunay_v1_exposes, ('vertices', 'simplices')),
         ('ConvexHull', ConvexHull_exposes, ConvexHull_v1_exposes, ('vertices', 'equations')),
         ('Voronoi', Voronoi_exposes, Voronoi_v1_exposes, ('regions', 'point_region'))]
 
     def scipy_spatial_storable(name, exposes, v1_exposes, check):
         _fallback = namedtuple(name, exposes)
-        _type = getattr(scipy.spatial.qhull, name)
+        try:
+            _type = getattr(scipy.spatial, name)
+        except AttributeError:
+            # deprecated location
+            _type = getattr(scipy.spatial.qhull, name)
         def _init(_exposes):
             def __init(*args):
                 #print(args) # debug
                 struct = _type(args[0])
                 check_attrs = list(check) # copy
                 ok = True
                 while ok and check_attrs:
@@ -142,18 +146,21 @@
                 if not ok:
                     warn("object of type '{}' could not be properly regenerated from the `points` argument only; using method-free fallback".format(name), RuntimeWarning)
                     struct = _fallback(*args)
                 return struct
             return __init
         handlers = [handler(_init(exposes), exposes, version=(0,))] # Py2
         if six.PY3:
-            auto = default_storable(_type)
+            spatial_peek = lambda _, exposes: default_peek(_type, exposes, excess_attributes=check)
+            auto = default_storable(_type, peek=spatial_peek)
             assert not auto.handlers[1:]
             assert handlers[0].version[0] < auto.handlers[0].version[0]
             handlers.append(auto.handlers[0])
         elif six.PY2 and v1_exposes:
             handlers.append(handler(_init(v1_exposes), v1_exposes, version=(1,)))
-        return ScipySpatialStorable(_type, handlers=handlers)
+        return ScipySpatialStorable(_type,
+            key='Python.scipy.spatial._qhull.' + _type.__name__,
+            handlers=handlers)
 
     spatial_storables += \
         [ scipy_spatial_storable(*_specs) for _specs in _scipy_spatial_types ]
```

### Comparing `rwa-python-0.9.1/rwa/sequence.py` & `rwa-python-0.9.2/rwa/sequence.py`

 * *Files identical despite different names*

### Comparing `rwa-python-0.9.1/rwa/storable.py` & `rwa-python-0.9.2/rwa/storable.py`

 * *Files identical despite different names*

### Comparing `rwa-python-0.9.1/rwa_python.egg-info/PKG-INFO` & `rwa-python-0.9.2/rwa_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: rwa-python
-Version: 0.9.1
+Version: 0.9.2
 Summary: HDF5-based serialization library for Python datatypes
 Home-page: https://github.com/DecBayComp/RWA-python
 Author: François Laurent
 Author-email: francois.laurent@pasteur.fr
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
 .. image:: https://img.shields.io/badge/docs-latest-blue.svg
    :target: https://rwa-python.readthedocs.io/en/latest/
 .. image:: https://github.com/DecBayComp/RWA-python/actions/workflows/ci.yml/badge.svg
    :target: https://github.com/DecBayComp/RWA-python/actions/workflows/ci.yml
 .. image:: https://codecov.io/gh/DecBayComp/RWA-python/branch/master/graph/badge.svg
@@ -100,9 +100,7 @@
 
 
 See also
 --------
 
 **RWA-python** is on `readthedocs <https://rwa-python.readthedocs.io/en/latest/>`_.
 
-
-
```

### Comparing `rwa-python-0.9.1/setup.py` & `rwa-python-0.9.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,30 +20,29 @@
     with open(os.path.join(pwd, 'README.rst'), encoding='utf-8') as f:
         long_description = f.read()
 except OSError:
     long_description = ''
 
 setup(
     name = 'rwa-python',
-    version = '0.9.1',
+    version = '0.9.2',
     description = 'HDF5-based serialization library for Python datatypes',
     long_description = long_description,
     url = 'https://github.com/DecBayComp/RWA-python',
     author = 'François Laurent',
     author_email = 'francois.laurent@pasteur.fr',
     license = 'Apache 2.0',
     classifiers = [
         'License :: OSI Approved :: Apache Software License',
-        #'Programming Language :: Python :: 2',
-        #'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     packages = ['rwa'],
     install_requires = install_requires,
     extras_require = extras_require,
 )
```

