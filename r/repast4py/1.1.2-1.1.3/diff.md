# Comparing `tmp/repast4py-1.1.2.tar.gz` & `tmp/repast4py-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repast4py-1.1.2.tar", last modified: Fri Apr  7 19:22:23 2023, max compression
+gzip compressed data, was "repast4py-1.1.3.tar", last modified: Wed May 31 19:53:42 2023, max compression
```

## Comparing `repast4py-1.1.2.tar` & `repast4py-1.1.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-07 19:22:23.855326 repast4py-1.1.2/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1777 2022-11-07 22:17:29.000000 repast4py-1.1.2/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       28 2022-11-07 22:16:19.000000 repast4py-1.1.2/MANIFEST.in
--rw-rw-r--   0 nick      (1000) nick      (1000)     5944 2023-04-07 19:22:23.855326 repast4py-1.1.2/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     4727 2023-02-15 18:59:58.000000 repast4py-1.1.2/README.md
--rw-rw-r--   0 nick      (1000) nick      (1000)      148 2022-11-07 22:17:29.000000 repast4py-1.1.2/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)     1386 2023-04-07 19:22:23.859326 repast4py-1.1.2/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)     1861 2022-11-07 22:16:20.000000 repast4py-1.1.2/setup.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-07 19:22:23.843326 repast4py-1.1.2/src/
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-07 19:22:23.855326 repast4py-1.1.2/src/repast4py/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1804 2022-11-07 22:16:24.000000 repast4py-1.1.2/src/repast4py/SpatialTree.cpp
--rw-rw-r--   0 nick      (1000) nick      (1000)    17254 2022-11-07 22:16:24.000000 repast4py-1.1.2/src/repast4py/SpatialTree.h
--rw-rw-r--   0 nick      (1000) nick      (1000)      225 2023-04-07 19:14:41.000000 repast4py-1.1.2/src/repast4py/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6660 2022-11-07 22:16:24.000000 repast4py-1.1.2/src/repast4py/borders.h
--rw-rw-r--   0 nick      (1000) nick      (1000)    22787 2023-03-20 13:58:24.000000 repast4py-1.1.2/src/repast4py/context.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4183 2022-11-07 22:16:24.000000 repast4py-1.1.2/src/repast4py/core.h
--rw-rw-r--   0 nick      (1000) nick      (1000)    14410 2023-02-15 18:59:58.000000 repast4py-1.1.2/src/repast4py/core.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    16125 2023-03-02 14:35:47.000000 repast4py-1.1.2/src/repast4py/coremodule.cpp
--rw-rw-r--   0 nick      (1000) nick      (1000)      781 2022-11-07 22:16:24.000000 repast4py-1.1.2/src/repast4py/coremodule.h
--rw-rw-r--   0 nick      (1000) nick      (1000)     8871 2022-11-07 22:16:24.000000 repast4py-1.1.2/src/repast4py/cspace.h
--rw-rw-r--   0 nick      (1000) nick      (1000)    17083 2022-11-07 22:16:24.000000 repast4py-1.1.2/src/repast4py/distributed_space.cpp
--rw-rw-r--   0 nick      (1000) nick      (1000)    18349 2022-11-07 22:16:24.000000 repast4py-1.1.2/src/repast4py/distributed_space.h
--rw-rw-r--   0 nick      (1000) nick      (1000)     6143 2022-11-07 22:16:24.000000 repast4py-1.1.2/src/repast4py/geometry.cpp
--rw-rw-r--   0 nick      (1000) nick      (1000)     3474 2022-11-07 22:16:24.000000 repast4py-1.1.2/src/repast4py/geometry.h
--rw-rw-r--   0 nick      (1000) nick      (1000)    10062 2023-02-15 18:59:58.000000 repast4py-1.1.2/src/repast4py/geometry.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6846 2022-11-07 22:16:24.000000 repast4py-1.1.2/src/repast4py/grid.h
--rw-rw-r--   0 nick      (1000) nick      (1000)    14525 2023-02-15 18:59:58.000000 repast4py-1.1.2/src/repast4py/logging.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    48302 2023-02-15 18:59:58.000000 repast4py-1.1.2/src/repast4py/network.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6111 2022-11-07 22:16:24.000000 repast4py-1.1.2/src/repast4py/occupancy.h
--rw-rw-r--   0 nick      (1000) nick      (1000)     2661 2023-02-15 18:59:58.000000 repast4py-1.1.2/src/repast4py/parameters.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1598 2023-02-15 18:59:58.000000 repast4py-1.1.2/src/repast4py/random.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    27226 2023-03-02 14:35:12.000000 repast4py-1.1.2/src/repast4py/schedule.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      463 2022-11-07 22:16:24.000000 repast4py-1.1.2/src/repast4py/space.cpp
--rw-rw-r--   0 nick      (1000) nick      (1000)     5474 2022-11-07 22:16:24.000000 repast4py-1.1.2/src/repast4py/space.h
--rw-rw-r--   0 nick      (1000) nick      (1000)    19665 2022-11-07 22:16:24.000000 repast4py-1.1.2/src/repast4py/space.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      411 2022-11-07 22:16:24.000000 repast4py-1.1.2/src/repast4py/space_types.h
--rw-rw-r--   0 nick      (1000) nick      (1000)   115952 2022-11-07 22:16:24.000000 repast4py-1.1.2/src/repast4py/spacemodule.cpp
--rw-rw-r--   0 nick      (1000) nick      (1000)     2504 2022-11-07 22:16:24.000000 repast4py-1.1.2/src/repast4py/util.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    51201 2023-04-07 19:01:38.000000 repast4py-1.1.2/src/repast4py/value_layer.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-07 19:22:23.855326 repast4py-1.1.2/src/repast4py.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)     5944 2023-04-07 19:22:23.000000 repast4py-1.1.2/src/repast4py.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     1119 2023-04-07 19:22:23.000000 repast4py-1.1.2/src/repast4py.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-04-07 19:22:23.000000 repast4py-1.1.2/src/repast4py.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      118 2023-04-07 19:22:23.000000 repast4py-1.1.2/src/repast4py.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       10 2023-04-07 19:22:23.000000 repast4py-1.1.2/src/repast4py.egg-info/top_level.txt
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-04-07 19:22:23.855326 repast4py-1.1.2/tests/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1501 2022-11-07 22:16:20.000000 repast4py-1.1.2/tests/test_agents.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    12554 2023-03-02 14:35:12.000000 repast4py-1.1.2/tests/test_schedule.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    28277 2022-11-07 22:16:20.000000 repast4py-1.1.2/tests/test_space.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    14758 2022-11-07 22:16:20.000000 repast4py-1.1.2/tests/test_value_layer.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 19:53:42.915564 repast4py-1.1.3/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1777 2022-11-07 22:17:29.000000 repast4py-1.1.3/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       28 2022-11-07 22:16:19.000000 repast4py-1.1.3/MANIFEST.in
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5830 2023-05-31 19:53:42.915564 repast4py-1.1.3/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4619 2023-04-07 19:45:51.000000 repast4py-1.1.3/README.md
+-rw-rw-r--   0 nick      (1000) nick      (1000)      148 2022-11-07 22:17:29.000000 repast4py-1.1.3/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1379 2023-05-31 19:53:42.915564 repast4py-1.1.3/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1861 2022-11-07 22:16:20.000000 repast4py-1.1.3/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 19:53:42.895563 repast4py-1.1.3/src/
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 19:53:42.911564 repast4py-1.1.3/src/repast4py/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1804 2022-11-07 22:16:24.000000 repast4py-1.1.3/src/repast4py/SpatialTree.cpp
+-rw-rw-r--   0 nick      (1000) nick      (1000)    17254 2022-11-07 22:16:24.000000 repast4py-1.1.3/src/repast4py/SpatialTree.h
+-rw-rw-r--   0 nick      (1000) nick      (1000)      225 2023-05-31 19:52:09.000000 repast4py-1.1.3/src/repast4py/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6660 2022-11-07 22:16:24.000000 repast4py-1.1.3/src/repast4py/borders.h
+-rw-rw-r--   0 nick      (1000) nick      (1000)    22787 2023-04-07 19:25:12.000000 repast4py-1.1.3/src/repast4py/context.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4183 2022-11-07 22:16:24.000000 repast4py-1.1.3/src/repast4py/core.h
+-rw-rw-r--   0 nick      (1000) nick      (1000)    14410 2023-02-15 18:59:58.000000 repast4py-1.1.3/src/repast4py/core.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    16125 2023-04-07 19:25:54.000000 repast4py-1.1.3/src/repast4py/coremodule.cpp
+-rw-rw-r--   0 nick      (1000) nick      (1000)      781 2022-11-07 22:16:24.000000 repast4py-1.1.3/src/repast4py/coremodule.h
+-rw-rw-r--   0 nick      (1000) nick      (1000)     8871 2022-11-07 22:16:24.000000 repast4py-1.1.3/src/repast4py/cspace.h
+-rw-rw-r--   0 nick      (1000) nick      (1000)    17083 2022-11-07 22:16:24.000000 repast4py-1.1.3/src/repast4py/distributed_space.cpp
+-rw-rw-r--   0 nick      (1000) nick      (1000)    18349 2022-11-07 22:16:24.000000 repast4py-1.1.3/src/repast4py/distributed_space.h
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6143 2022-11-07 22:16:24.000000 repast4py-1.1.3/src/repast4py/geometry.cpp
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3474 2022-11-07 22:16:24.000000 repast4py-1.1.3/src/repast4py/geometry.h
+-rw-rw-r--   0 nick      (1000) nick      (1000)    10062 2023-02-15 18:59:58.000000 repast4py-1.1.3/src/repast4py/geometry.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6846 2022-11-07 22:16:24.000000 repast4py-1.1.3/src/repast4py/grid.h
+-rw-rw-r--   0 nick      (1000) nick      (1000)    14525 2023-02-15 18:59:58.000000 repast4py-1.1.3/src/repast4py/logging.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    48302 2023-02-15 18:59:58.000000 repast4py-1.1.3/src/repast4py/network.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6111 2022-11-07 22:16:24.000000 repast4py-1.1.3/src/repast4py/occupancy.h
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2661 2023-02-15 18:59:58.000000 repast4py-1.1.3/src/repast4py/parameters.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1598 2023-02-15 18:59:58.000000 repast4py-1.1.3/src/repast4py/random.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    27226 2023-03-02 14:35:12.000000 repast4py-1.1.3/src/repast4py/schedule.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      463 2022-11-07 22:16:24.000000 repast4py-1.1.3/src/repast4py/space.cpp
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5474 2022-11-07 22:16:24.000000 repast4py-1.1.3/src/repast4py/space.h
+-rw-rw-r--   0 nick      (1000) nick      (1000)    19665 2022-11-07 22:16:24.000000 repast4py-1.1.3/src/repast4py/space.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      411 2022-11-07 22:16:24.000000 repast4py-1.1.3/src/repast4py/space_types.h
+-rw-rw-r--   0 nick      (1000) nick      (1000)   115952 2022-11-07 22:16:24.000000 repast4py-1.1.3/src/repast4py/spacemodule.cpp
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2504 2022-11-07 22:16:24.000000 repast4py-1.1.3/src/repast4py/util.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    51200 2023-04-07 19:26:24.000000 repast4py-1.1.3/src/repast4py/value_layer.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 19:53:42.915564 repast4py-1.1.3/src/repast4py.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5830 2023-05-31 19:53:42.000000 repast4py-1.1.3/src/repast4py.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1119 2023-05-31 19:53:42.000000 repast4py-1.1.3/src/repast4py.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-31 19:53:42.000000 repast4py-1.1.3/src/repast4py.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      118 2023-05-31 19:53:42.000000 repast4py-1.1.3/src/repast4py.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       10 2023-05-31 19:53:42.000000 repast4py-1.1.3/src/repast4py.egg-info/top_level.txt
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-31 19:53:42.915564 repast4py-1.1.3/tests/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1501 2022-11-07 22:16:20.000000 repast4py-1.1.3/tests/test_agents.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    12554 2023-03-02 14:35:12.000000 repast4py-1.1.3/tests/test_schedule.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    28277 2022-11-07 22:16:20.000000 repast4py-1.1.3/tests/test_space.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    14758 2022-11-07 22:16:20.000000 repast4py-1.1.3/tests/test_value_layer.py
```

### Comparing `repast4py-1.1.2/LICENSE.txt` & `repast4py-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/PKG-INFO` & `repast4py-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repast4py
-Version: 1.1.2
+Version: 1.1.3
 Summary: repast4py package
 Home-page: https://repast.github.io/repast4py.site/index.html
 Author: Nick Collier
 Author-email: ncollier@anl.gov
 Maintainer: Nick Collier
 Maintainer-email: ncollier@anl.gov
 License: BSD 3-Clause License
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Distributed Computing
-Requires-Python: <3.11,>=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Repast for Python (Repast4Py)
 
 [![codecov](https://codecov.io/gh/Repast/repast4py/branch/develop/graph/badge.svg?token=JCDU2LT8G2)](https://codecov.io/gh/Repast/repast4py/branch/develop)
 
@@ -35,16 +35,16 @@
 
 <table>
   <tr>
     <td><b>Master</b></td>
     <td><b>Develop</b></td>
   </tr>
   <tr>
-    <td><a href="https://circleci.com/gh/Repast/repast4py/tree/master"><img src="https://circleci.com/gh/Repast/repast4py/tree/master.svg?style=shield&circle-token=8eabe328704119bf3f175172e1613c52f9310c65" alt="Build Status" /></a></td>
-    <td><a href="https://circleci.com/gh/Repast/repast4py/tree/develop"><img src="https://circleci.com/gh/Repast/repast4py/tree/develop.svg?style=shield&circle-token=8eabe328704119bf3f175172e1613c52f9310c65" alt="Build Status" /></a></td>
+    <td><a href="https://circleci.com/gh/Repast/repast4py/tree/master"><img src="https://circleci.com/gh/Repast/repast4py/tree/master.svg?style=shield" alt="Build Status" /></a></td>
+    <td><a href="https://circleci.com/gh/Repast/repast4py/tree/develop"><img src="https://circleci.com/gh/Repast/repast4py/tree/develop.svg?style=shield" alt="Build Status" /></a></td>
   </tr>
 </table>
 
 ## Repast4Py
 
 Repast for Python (Repast4Py) is the newest member of the [Repast Suite](https://repast.github.io) of 
 free and open source agent-based modeling and simulation software.
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: repast4py Version: 1.1.2 Summary: repast4py package
+Metadata-Version: 2.1 Name: repast4py Version: 1.1.3 Summary: repast4py package
 Home-page: https://repast.github.io/repast4py.site/index.html Author: Nick
 Collier Author-email: ncollier@anl.gov Maintainer: Nick Collier Maintainer-
 email: ncollier@anl.gov License: BSD 3-Clause License Project-URL: Git
 Repostitory, https://github.com/Repast/repast4py Project-URL: Issue Tracker,
 https://github.com/Repast/repast4py/issues Project-URL: Documentation, https://
 repast.github.io/repast4py.site/guide/user_guide.html Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: System :: Distributed Computing Requires-Python:
-<3.11,>=3.7 Description-Content-Type: text/markdown License-File: LICENSE.txt #
+>=3.7 Description-Content-Type: text/markdown License-File: LICENSE.txt #
 Repast for Python (Repast4Py) [![codecov](https://codecov.io/gh/Repast/
 repast4py/branch/develop/graph/badge.svg?token=JCDU2LT8G2)](https://codecov.io/
 gh/Repast/repast4py/branch/develop) ## Build Status
 Master         Develop
 [Build_Status] [Build_Status]
 ## Repast4Py Repast for Python (Repast4Py) is the newest member of the [Repast
 Suite](https://repast.github.io) of free and open source agent-based modeling
```

### Comparing `repast4py-1.1.2/README.md` & `repast4py-1.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 <table>
   <tr>
     <td><b>Master</b></td>
     <td><b>Develop</b></td>
   </tr>
   <tr>
-    <td><a href="https://circleci.com/gh/Repast/repast4py/tree/master"><img src="https://circleci.com/gh/Repast/repast4py/tree/master.svg?style=shield&circle-token=8eabe328704119bf3f175172e1613c52f9310c65" alt="Build Status" /></a></td>
-    <td><a href="https://circleci.com/gh/Repast/repast4py/tree/develop"><img src="https://circleci.com/gh/Repast/repast4py/tree/develop.svg?style=shield&circle-token=8eabe328704119bf3f175172e1613c52f9310c65" alt="Build Status" /></a></td>
+    <td><a href="https://circleci.com/gh/Repast/repast4py/tree/master"><img src="https://circleci.com/gh/Repast/repast4py/tree/master.svg?style=shield" alt="Build Status" /></a></td>
+    <td><a href="https://circleci.com/gh/Repast/repast4py/tree/develop"><img src="https://circleci.com/gh/Repast/repast4py/tree/develop.svg?style=shield" alt="Build Status" /></a></td>
   </tr>
 </table>
 
 ## Repast4Py
 
 Repast for Python (Repast4Py) is the newest member of the [Repast Suite](https://repast.github.io) of 
 free and open source agent-based modeling and simulation software.
```

### Comparing `repast4py-1.1.2/setup.cfg` & `repast4py-1.1.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 	numba
 	mpi4py
 	torch
 	networkx >=2.6.2
 	pyyaml
 	Cython
 	typing_extensions;python_version < "3.8.0"
-python_requires = >= 3.7, <3.11
+python_requires = >= 3.7
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `repast4py-1.1.2/setup.py` & `repast4py-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/SpatialTree.cpp` & `repast4py-1.1.3/src/repast4py/SpatialTree.cpp`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/SpatialTree.h` & `repast4py-1.1.3/src/repast4py/SpatialTree.h`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/borders.h` & `repast4py-1.1.3/src/repast4py/borders.h`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/context.py` & `repast4py-1.1.3/src/repast4py/context.py`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/core.h` & `repast4py-1.1.3/src/repast4py/core.h`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/core.py` & `repast4py-1.1.3/src/repast4py/core.py`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/coremodule.cpp` & `repast4py-1.1.3/src/repast4py/coremodule.cpp`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/coremodule.h` & `repast4py-1.1.3/src/repast4py/coremodule.h`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/cspace.h` & `repast4py-1.1.3/src/repast4py/cspace.h`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/distributed_space.cpp` & `repast4py-1.1.3/src/repast4py/distributed_space.cpp`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/distributed_space.h` & `repast4py-1.1.3/src/repast4py/distributed_space.h`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/geometry.cpp` & `repast4py-1.1.3/src/repast4py/geometry.cpp`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/geometry.h` & `repast4py-1.1.3/src/repast4py/geometry.h`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/geometry.py` & `repast4py-1.1.3/src/repast4py/geometry.py`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/grid.h` & `repast4py-1.1.3/src/repast4py/grid.h`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/logging.py` & `repast4py-1.1.3/src/repast4py/logging.py`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/network.py` & `repast4py-1.1.3/src/repast4py/network.py`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/occupancy.h` & `repast4py-1.1.3/src/repast4py/occupancy.h`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/parameters.py` & `repast4py-1.1.3/src/repast4py/parameters.py`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/random.py` & `repast4py-1.1.3/src/repast4py/random.py`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/schedule.py` & `repast4py-1.1.3/src/repast4py/schedule.py`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/space.h` & `repast4py-1.1.3/src/repast4py/space.h`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/space.py` & `repast4py-1.1.3/src/repast4py/space.py`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/spacemodule.cpp` & `repast4py-1.1.3/src/repast4py/spacemodule.cpp`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/util.py` & `repast4py-1.1.3/src/repast4py/util.py`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/src/repast4py/value_layer.py` & `repast4py-1.1.3/src/repast4py/value_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -845,15 +845,14 @@
                                           (slice(row, stop_row), slice(col, stop_col))))
                     else:
                         break
 
             if len(slice_data) > 0:
                 recv_buf_data.append(slice_data)
 
-
         self.recv_data = ((recv_buf, (recv_counts, recv_displs)), recv_buf_data)
 
     def _init_sync_data_3d(self, topo, buffer_size):
         ngh_buffers = []
         # create send_counts, send_displs, and send_buf
         # buf_ngh: (rank, (ranges)) e.g., (1, (8, 10, 40, 42, 0, 0))
         c_trans = self.impl.pt_translation[0]
```

### Comparing `repast4py-1.1.2/src/repast4py.egg-info/PKG-INFO` & `repast4py-1.1.3/src/repast4py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repast4py
-Version: 1.1.2
+Version: 1.1.3
 Summary: repast4py package
 Home-page: https://repast.github.io/repast4py.site/index.html
 Author: Nick Collier
 Author-email: ncollier@anl.gov
 Maintainer: Nick Collier
 Maintainer-email: ncollier@anl.gov
 License: BSD 3-Clause License
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Distributed Computing
-Requires-Python: <3.11,>=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Repast for Python (Repast4Py)
 
 [![codecov](https://codecov.io/gh/Repast/repast4py/branch/develop/graph/badge.svg?token=JCDU2LT8G2)](https://codecov.io/gh/Repast/repast4py/branch/develop)
 
@@ -35,16 +35,16 @@
 
 <table>
   <tr>
     <td><b>Master</b></td>
     <td><b>Develop</b></td>
   </tr>
   <tr>
-    <td><a href="https://circleci.com/gh/Repast/repast4py/tree/master"><img src="https://circleci.com/gh/Repast/repast4py/tree/master.svg?style=shield&circle-token=8eabe328704119bf3f175172e1613c52f9310c65" alt="Build Status" /></a></td>
-    <td><a href="https://circleci.com/gh/Repast/repast4py/tree/develop"><img src="https://circleci.com/gh/Repast/repast4py/tree/develop.svg?style=shield&circle-token=8eabe328704119bf3f175172e1613c52f9310c65" alt="Build Status" /></a></td>
+    <td><a href="https://circleci.com/gh/Repast/repast4py/tree/master"><img src="https://circleci.com/gh/Repast/repast4py/tree/master.svg?style=shield" alt="Build Status" /></a></td>
+    <td><a href="https://circleci.com/gh/Repast/repast4py/tree/develop"><img src="https://circleci.com/gh/Repast/repast4py/tree/develop.svg?style=shield" alt="Build Status" /></a></td>
   </tr>
 </table>
 
 ## Repast4Py
 
 Repast for Python (Repast4Py) is the newest member of the [Repast Suite](https://repast.github.io) of 
 free and open source agent-based modeling and simulation software.
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: repast4py Version: 1.1.2 Summary: repast4py package
+Metadata-Version: 2.1 Name: repast4py Version: 1.1.3 Summary: repast4py package
 Home-page: https://repast.github.io/repast4py.site/index.html Author: Nick
 Collier Author-email: ncollier@anl.gov Maintainer: Nick Collier Maintainer-
 email: ncollier@anl.gov License: BSD 3-Clause License Project-URL: Git
 Repostitory, https://github.com/Repast/repast4py Project-URL: Issue Tracker,
 https://github.com/Repast/repast4py/issues Project-URL: Documentation, https://
 repast.github.io/repast4py.site/guide/user_guide.html Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: System :: Distributed Computing Requires-Python:
-<3.11,>=3.7 Description-Content-Type: text/markdown License-File: LICENSE.txt #
+>=3.7 Description-Content-Type: text/markdown License-File: LICENSE.txt #
 Repast for Python (Repast4Py) [![codecov](https://codecov.io/gh/Repast/
 repast4py/branch/develop/graph/badge.svg?token=JCDU2LT8G2)](https://codecov.io/
 gh/Repast/repast4py/branch/develop) ## Build Status
 Master         Develop
 [Build_Status] [Build_Status]
 ## Repast4Py Repast for Python (Repast4Py) is the newest member of the [Repast
 Suite](https://repast.github.io) of free and open source agent-based modeling
```

### Comparing `repast4py-1.1.2/src/repast4py.egg-info/SOURCES.txt` & `repast4py-1.1.3/src/repast4py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/tests/test_agents.py` & `repast4py-1.1.3/tests/test_agents.py`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/tests/test_schedule.py` & `repast4py-1.1.3/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/tests/test_space.py` & `repast4py-1.1.3/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `repast4py-1.1.2/tests/test_value_layer.py` & `repast4py-1.1.3/tests/test_value_layer.py`

 * *Files identical despite different names*

