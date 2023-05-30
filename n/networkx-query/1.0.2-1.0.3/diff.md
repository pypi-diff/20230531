# Comparing `tmp/networkx_query-1.0.2.tar.gz` & `tmp/networkx_query-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networkx_query-1.0.2.tar", max compression
+gzip compressed data, was "networkx_query-1.0.3.tar", max compression
```

## Comparing `networkx_query-1.0.2.tar` & `networkx_query-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1100 2020-09-09 06:59:30.189856 networkx_query-1.0.2/LICENSE.md
--rw-r--r--   0        0        0     7131 2020-09-09 06:59:30.190132 networkx_query-1.0.2/README.md
--rw-r--r--   0        0        0      568 2023-05-09 10:42:29.829423 networkx_query-1.0.2/networkx_query/__init__.py
--rw-r--r--   0        0        0     4722 2020-09-09 06:59:30.234021 networkx_query-1.0.2/networkx_query/definition.py
--rw-r--r--   0        0        0     5851 2020-09-09 06:59:30.234191 networkx_query-1.0.2/networkx_query/operator.py
--rw-r--r--   0        0        0     2700 2020-09-09 06:59:30.234349 networkx_query-1.0.2/networkx_query/parser.py
--rw-r--r--   0        0        0     1310 2020-09-09 06:59:30.234497 networkx_query-1.0.2/networkx_query/query.py
--rw-r--r--   0        0        0     2060 2020-09-09 06:59:30.234632 networkx_query-1.0.2/networkx_query/relationship.py
--rw-r--r--   0        0        0     2136 2020-09-09 06:59:30.234763 networkx_query-1.0.2/networkx_query/utils.py
--rw-r--r--   0        0        0     3017 2023-05-09 11:15:01.856553 networkx_query-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     8062 2023-05-09 11:16:18.585241 networkx_query-1.0.2/setup.py
--rw-r--r--   0        0        0     8157 2023-05-09 11:16:18.585717 networkx_query-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-05-30 22:11:56.195003 networkx_query-1.0.3/LICENSE.md
+-rw-r--r--   0        0        0     8908 2023-05-30 22:11:56.195003 networkx_query-1.0.3/README.md
+-rw-r--r--   0        0        0      652 2023-05-30 22:11:56.195003 networkx_query-1.0.3/networkx_query/__init__.py
+-rw-r--r--   0        0        0     4722 2023-05-30 22:11:56.195003 networkx_query-1.0.3/networkx_query/definition.py
+-rw-r--r--   0        0        0     5851 2023-05-30 22:11:56.195003 networkx_query-1.0.3/networkx_query/operator.py
+-rw-r--r--   0        0        0     2700 2023-05-30 22:11:56.195003 networkx_query-1.0.3/networkx_query/parser.py
+-rw-r--r--   0        0        0     1310 2023-05-30 22:11:56.195003 networkx_query-1.0.3/networkx_query/query.py
+-rw-r--r--   0        0        0     4463 2023-05-30 22:11:56.195003 networkx_query-1.0.3/networkx_query/relationship.py
+-rw-r--r--   0        0        0     2136 2023-05-30 22:11:56.195003 networkx_query-1.0.3/networkx_query/utils.py
+-rw-r--r--   0        0        0     3134 2023-05-30 22:11:56.195003 networkx_query-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    10036 1970-01-01 00:00:00.000000 networkx_query-1.0.3/PKG-INFO
```

### Comparing `networkx_query-1.0.2/LICENSE.md` & `networkx_query-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.2/README.md` & `networkx_query-1.0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # networkx-query
 
-
-[![Unix Build Status](https://img.shields.io/travis/geronimo-iia/networkx-query/master.svg?label=unix)](https://travis-ci.com/geronimo-iia/networkx-query)[![Coverage Status](https://img.shields.io/coveralls/geronimo-iia/networkx-query/master.svg)](https://coveralls.io/r/geronimo-iia/networkx-query)
+[Coverage Status](https://img.shields.io/coveralls/geronimo-iia/networkx-query/master.svg)](https://coveralls.io/r/geronimo-iia/networkx-query)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/fe669a02b4aa46b5b1faf619ba2bf382)](https://www.codacy.com/app/geronimo-iia/networkx-query?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=geronimo-iia/networkx-query&amp;utm_campaign=Badge_Grade)[![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/geronimo-iia/networkx-query.svg)](https://scrutinizer-ci.com/g/geronimo-iia/networkx-query/?branch=master)
 [![PyPI Version](https://img.shields.io/pypi/v/networkx-query.svg)](https://pypi.org/project/networkx-query)
 [![PyPI License](https://img.shields.io/pypi/l/networkx-query.svg)](https://pypi.org/project/networkx-query)
 
 Versions following [Semantic Versioning](https://semver.org/)
 
 ## Overview
@@ -56,15 +55,15 @@
 ```python
 for edge_id in search_edges(g, {"eq": [("action",), "produce"]}):
     print(edge_id)
 
 >> (3, 2)
 ```
 
-### Searching relation ship
+### Searching direct relation ship
 
 With ```search_direct_relationships``` you can made a query which filter edges on their :
  - source node attributes
  - edge attributes
  - target node attributes
 
 With this graph:
@@ -110,24 +109,99 @@
             graph=g, source={"gt": ["data", 9]}, edge={"gt": ["data", 15]}, target={'lt': ["data", 22]}
         )
     )
 
 >> [(10, 20), (11, 21)]
 ```
 
+
+
+### search_relationships
+
+With :
+
+```python
+    g = nx.DiGraph()
+    g.add_node(1, product="a")
+    g.add_node(2, product="b")
+    g.add_node(3, product="c")
+    g.add_node(4, product="d")
+
+    g.add_edge(1, 2)
+    g.add_edge(1, 3, weight=2)
+    g.add_edge(1, 4)
+
+    g.add_edge(2, 4)
+    g.add_edge(3, 4)
+```
+
+
+You could find all path with multiple constraints:
+
+```python
+    list(search_relationships(
+            g,
+            {"eq": [("product",), "a"]},
+            PathCriteria(target={"eq": [("product",), "b"]}),
+            PathCriteria(target={"eq": [("product",), "d"]}),
+        )) 
+    # output: [[1, 2, 4]]
+
+     list(search_relationships(g, {"eq": [("product",), "a"]}, PathCriteria(target={"eq": [("product",), "c"]})))
+     # outptu: [[1, 3]]
+```
+
+or something more complex:
+
+```python
+
+    g.add_node(5, product="d")
+    g.add_node(6, product="d")
+    g.add_node(7, product="a")
+    g.add_node(8, product="a")
+
+    g.add_edge(7, 5, weight=2)
+    g.add_edge(7, 6, weight=2)
+    g.add_edge(8, 5, weight=2)
+
+    list(
+        search_relationships(
+            g,
+            {"eq": [("product",), "a"]},  # node 1, 7, 8
+            PathCriteria(
+                target={"eq": [("product",), "d"]}, edge={"eq": [("weight",), 2]}
+            ),  # edge 1-3, 7-5, 7-6, 8-5  node 4, 5, 6 -> no 1, 3, 4
+        )
+    )
+    # output: [[7, 5], [7, 6], [8, 5]]
+
+    list(
+        search_relationships(
+            g,
+            {"eq": [("product",), "a"]},  # node 1, 7, 8
+            PathCriteria(target={}, edge={"eq": [("weight",), 2]}),  # edge 1-3, 7-5, 7-6, 8-5
+            PathCriteria(target={"eq": [("product",), "d"]}),  # node 4, 5, 6 -> no 1, 3, 4
+        )
+    )
+    # output: [[1, 3, 4]]
+```
+
+Note the usage of `PathCriteria(target={}, ..` to define a constraint based only on edge. `{}` act as a wildcard.
+
 ## API
 
 Actually, we have:
 
-- [search_edges](https://geronimo-iia.github.io/networkx-query/api.html#networkx_query.search_edges)
-- [search_nodes](https://geronimo-iia.github.io/networkx-query/api.html#networkx_query.search_nodes) 
-- [search_direct_relationships](https://geronimo-iia.github.io/networkx-query/api.html#networkx_query.search_direct_relationships) 
+- [search_edges](https://geronimo-iia.github.io/networkx-query/reference/#networkx_query.search_edges)
+- [search_nodes](https://geronimo-iia.github.io/networkx-query/reference/#networkx_query.search_nodes) 
+- [search_direct_relationships](https://geronimo-iia.github.io/networkx-query/reference/#networkx_query.search_direct_relationships) 
+- [search_relationships](https://geronimo-iia.github.io/networkx-query/reference/#networkx_query.search_relationships) 
 
 
-All this function are based on [prepare_query](https://geronimo-iia.github.io/networkx-query/api.html#networkx_query.prepare_query) which return an Evaluator.
+All this function are based on [prepare_query](https://geronimo-iia.github.io/networkx-query/reference/#networkx_query.prepare_query) which return an Evaluator.
 
 Quickly, ```Evaluator``` are function with this signature: (context) -> bool, and ```Context``` is a dictionary like structure (with in and [] methods, and support __contains__ or  (__iter__ and __getitem__))
 With networkX, node and edge attributes are dictionary like, so implementation of this three methods are very simple.
 
 
 
 ## Query language
@@ -224,15 +298,13 @@
         {
             'eq': [('_link', 'other', 'weight'), 2]
         }
     ]
 }
 ```
 
-
 ## Wished Features
 
 - add projection expression (a return like statement)
 - add join relation ship 
-- add path condition between node
```

### Comparing `networkx_query-1.0.2/networkx_query/__init__.py` & `networkx_query-1.0.3/networkx_query/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """networkx-query."""
 from pkg_resources import DistributionNotFound, get_distribution
 
 from .definition import Evaluator, ParserException
 from .parser import prepare_query
 from .query import search_edges, search_nodes
-from .relationship import search_direct_relationships
+from .relationship import PathCriteria, search_direct_relationships, search_relationships
 
 __all__ = [
     'search_nodes',
     'search_edges',
     'search_direct_relationships',
     'prepare_query',
     'ParserException',
     'Evaluator',
+    'search_relationships',
+    'PathCriteria',
 ]
 
 try:
     __version__ = get_distribution('networkx_query').version
 except DistributionNotFound:  # pragma: no cover
     __version__ = '(local)'
```

### Comparing `networkx_query-1.0.2/networkx_query/definition.py` & `networkx_query-1.0.3/networkx_query/definition.py`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.2/networkx_query/operator.py` & `networkx_query-1.0.3/networkx_query/operator.py`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.2/networkx_query/parser.py` & `networkx_query-1.0.3/networkx_query/parser.py`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.2/networkx_query/query.py` & `networkx_query-1.0.3/networkx_query/query.py`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.2/networkx_query/utils.py` & `networkx_query-1.0.3/networkx_query/utils.py`

 * *Files identical despite different names*

### Comparing `networkx_query-1.0.2/pyproject.toml` & `networkx_query-1.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "networkx_query"
-version = "1.0.2"
+version = "1.0.3"
 description = "NetworkX Query Tool"
 license = "MIT"
 authors = ["Jerome Guibert <jguibert@gmail.com>"]
 readme = "README.md"
 homepage = "https://pypi.org/project/networkx_query"
 documentation = "https://geronimo-iia.github.io/networkx-query/"
 repository = "https://github.com/geronimo-iia/networkx-query"
@@ -30,26 +30,28 @@
 black = "22.3.0"             # The uncompromising code formatter.
 isort = "5.9.3"              #A Python utility / library to sort Python imports.
 ruff = "^0.0.264"
 mypy = "*"
 types-setuptools = "^67.7.0"
 
 # Unit Testing
-pytest = "^6"                                   # pytest: simple powerful testing with Python
-pytest-cov = "^2"                               # Pytest plugin for measuring coverage.
-pytest-mock = "^3"
+pytest = "^7"                                   # pytest: simple powerful testing with Python
+pytest-cov = "^4"                               # Pytest plugin for measuring coverage.
 xdoctest = "^0.15.0"                            # A rewrite of the builtin doctest module
 coverage = { version = "*", extras = ["toml"] }
 
 # Documentation
 mkdocs = { extras = ["markdown-include"], version = "^1.4.3" }
 mkdocstrings = { extras = ["python"], version = "^0.21.2" }
 mkdocs-material = "^9.1.9"
 mkdocs-include-markdown-plugin = "^4.0.4"
 
+# Security bumps from dependabot
+pymdown-extensions = "^10.0"
+requests = "^2.31.0"
 
 [tool.black]
 # see https://black.readthedocs.io/en/stable/
 target-version = ["py38"]
 skip-string-normalization = true
 line_length = 120
 
@@ -77,17 +79,19 @@
 exclude_lines = ["pragma: no cover", "raise NotImplementedError"]
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "--strict-markers --pdbcls=tests:Debugger -r sxX --cov=networkx_query --cov-report=html --cov-report=term-missing:skip-covered"
 
 [tool.ruff]
+cache-dir = ".cache/ruff"
 line-length = 120
 
 [tool.mypy]
+cache_dir = ".cache/mypy/"
 check_untyped_defs = true
 ignore_errors = false
 ignore_missing_imports = true
 warn_unused_ignores = true
 warn_redundant_casts = true
 warn_unused_configs = true
```

### Comparing `networkx_query-1.0.2/PKG-INFO` & `networkx_query-1.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: networkx-query
-Version: 1.0.2
+Version: 1.0.3
 Summary: NetworkX Query Tool
 Home-page: https://pypi.org/project/networkx_query
 License: MIT
 Keywords: networkx,graph,query
 Author: Jerome Guibert
 Author-email: jguibert@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: networkx (>=2.4,<3.0)
 Project-URL: Documentation, https://geronimo-iia.github.io/networkx-query/
 Project-URL: Repository, https://github.com/geronimo-iia/networkx-query
 Description-Content-Type: text/markdown
 
 # networkx-query
 
-
-[![Unix Build Status](https://img.shields.io/travis/geronimo-iia/networkx-query/master.svg?label=unix)](https://travis-ci.com/geronimo-iia/networkx-query)[![Coverage Status](https://img.shields.io/coveralls/geronimo-iia/networkx-query/master.svg)](https://coveralls.io/r/geronimo-iia/networkx-query)
+[Coverage Status](https://img.shields.io/coveralls/geronimo-iia/networkx-query/master.svg)](https://coveralls.io/r/geronimo-iia/networkx-query)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/fe669a02b4aa46b5b1faf619ba2bf382)](https://www.codacy.com/app/geronimo-iia/networkx-query?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=geronimo-iia/networkx-query&amp;utm_campaign=Badge_Grade)[![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/geronimo-iia/networkx-query.svg)](https://scrutinizer-ci.com/g/geronimo-iia/networkx-query/?branch=master)
 [![PyPI Version](https://img.shields.io/pypi/v/networkx-query.svg)](https://pypi.org/project/networkx-query)
 [![PyPI License](https://img.shields.io/pypi/l/networkx-query.svg)](https://pypi.org/project/networkx-query)
 
 Versions following [Semantic Versioning](https://semver.org/)
 
 ## Overview
@@ -82,15 +83,15 @@
 ```python
 for edge_id in search_edges(g, {"eq": [("action",), "produce"]}):
     print(edge_id)
 
 >> (3, 2)
 ```
 
-### Searching relation ship
+### Searching direct relation ship
 
 With ```search_direct_relationships``` you can made a query which filter edges on their :
  - source node attributes
  - edge attributes
  - target node attributes
 
 With this graph:
@@ -136,24 +137,99 @@
             graph=g, source={"gt": ["data", 9]}, edge={"gt": ["data", 15]}, target={'lt': ["data", 22]}
         )
     )
 
 >> [(10, 20), (11, 21)]
 ```
 
+
+
+### search_relationships
+
+With :
+
+```python
+    g = nx.DiGraph()
+    g.add_node(1, product="a")
+    g.add_node(2, product="b")
+    g.add_node(3, product="c")
+    g.add_node(4, product="d")
+
+    g.add_edge(1, 2)
+    g.add_edge(1, 3, weight=2)
+    g.add_edge(1, 4)
+
+    g.add_edge(2, 4)
+    g.add_edge(3, 4)
+```
+
+
+You could find all path with multiple constraints:
+
+```python
+    list(search_relationships(
+            g,
+            {"eq": [("product",), "a"]},
+            PathCriteria(target={"eq": [("product",), "b"]}),
+            PathCriteria(target={"eq": [("product",), "d"]}),
+        )) 
+    # output: [[1, 2, 4]]
+
+     list(search_relationships(g, {"eq": [("product",), "a"]}, PathCriteria(target={"eq": [("product",), "c"]})))
+     # outptu: [[1, 3]]
+```
+
+or something more complex:
+
+```python
+
+    g.add_node(5, product="d")
+    g.add_node(6, product="d")
+    g.add_node(7, product="a")
+    g.add_node(8, product="a")
+
+    g.add_edge(7, 5, weight=2)
+    g.add_edge(7, 6, weight=2)
+    g.add_edge(8, 5, weight=2)
+
+    list(
+        search_relationships(
+            g,
+            {"eq": [("product",), "a"]},  # node 1, 7, 8
+            PathCriteria(
+                target={"eq": [("product",), "d"]}, edge={"eq": [("weight",), 2]}
+            ),  # edge 1-3, 7-5, 7-6, 8-5  node 4, 5, 6 -> no 1, 3, 4
+        )
+    )
+    # output: [[7, 5], [7, 6], [8, 5]]
+
+    list(
+        search_relationships(
+            g,
+            {"eq": [("product",), "a"]},  # node 1, 7, 8
+            PathCriteria(target={}, edge={"eq": [("weight",), 2]}),  # edge 1-3, 7-5, 7-6, 8-5
+            PathCriteria(target={"eq": [("product",), "d"]}),  # node 4, 5, 6 -> no 1, 3, 4
+        )
+    )
+    # output: [[1, 3, 4]]
+```
+
+Note the usage of `PathCriteria(target={}, ..` to define a constraint based only on edge. `{}` act as a wildcard.
+
 ## API
 
 Actually, we have:
 
-- [search_edges](https://geronimo-iia.github.io/networkx-query/api.html#networkx_query.search_edges)
-- [search_nodes](https://geronimo-iia.github.io/networkx-query/api.html#networkx_query.search_nodes) 
-- [search_direct_relationships](https://geronimo-iia.github.io/networkx-query/api.html#networkx_query.search_direct_relationships) 
+- [search_edges](https://geronimo-iia.github.io/networkx-query/reference/#networkx_query.search_edges)
+- [search_nodes](https://geronimo-iia.github.io/networkx-query/reference/#networkx_query.search_nodes) 
+- [search_direct_relationships](https://geronimo-iia.github.io/networkx-query/reference/#networkx_query.search_direct_relationships) 
+- [search_relationships](https://geronimo-iia.github.io/networkx-query/reference/#networkx_query.search_relationships) 
 
 
-All this function are based on [prepare_query](https://geronimo-iia.github.io/networkx-query/api.html#networkx_query.prepare_query) which return an Evaluator.
+All this function are based on [prepare_query](https://geronimo-iia.github.io/networkx-query/reference/#networkx_query.prepare_query) which return an Evaluator.
 
 Quickly, ```Evaluator``` are function with this signature: (context) -> bool, and ```Context``` is a dictionary like structure (with in and [] methods, and support __contains__ or  (__iter__ and __getitem__))
 With networkX, node and edge attributes are dictionary like, so implementation of this three methods are very simple.
 
 
 
 ## Query language
@@ -250,16 +326,14 @@
         {
             'eq': [('_link', 'other', 'weight'), 2]
         }
     ]
 }
 ```
 
-
 ## Wished Features
 
 - add projection expression (a return like statement)
 - add join relation ship 
-- add path condition between node
```

