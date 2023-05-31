# Comparing `tmp/emg3d-1.8.1.tar.gz` & `tmp/emg3d-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emg3d-1.8.1.tar", last modified: Sat Oct 15 20:51:47 2022, max compression
+gzip compressed data, was "emg3d-1.8.2.tar", last modified: Wed May 31 15:08:30 2023, max compression
```

## Comparing `emg3d-1.8.1.tar` & `emg3d-1.8.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-15 20:51:47.910897 emg3d-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)     2345 2022-10-15 20:51:37.000000 emg3d-1.8.1/CREDITS.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-10-15 20:51:37.000000 emg3d-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1263 2022-10-15 20:51:47.910897 emg3d-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-10-15 20:51:37.000000 emg3d-1.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-15 20:51:47.910897 emg3d-1.8.1/emg3d/
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14208 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/_multiprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-15 20:51:47.910897 emg3d-1.8.1/emg3d/cli/
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6109 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    14426 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     9408 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (121)    85080 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    25493 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/electrodes.py
--rw-r--r--   0 runner    (1001) docker     (121)    33827 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)    16028 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    29678 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/maps.py
--rw-r--r--   0 runner    (1001) docker     (121)    55477 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/meshes.py
--rw-r--r--   0 runner    (1001) docker     (121)    27599 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/models.py
--rw-r--r--   0 runner    (1001) docker     (121)    64699 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/simulations.py
--rw-r--r--   0 runner    (1001) docker     (121)    67908 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/solver.py
--rw-r--r--   0 runner    (1001) docker     (121)    34760 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/surveys.py
--rw-r--r--   0 runner    (1001) docker     (121)    14722 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/time.py
--rw-r--r--   0 runner    (1001) docker     (121)     8305 2022-10-15 20:51:37.000000 emg3d-1.8.1/emg3d/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-15 20:51:47.000000 emg3d-1.8.1/emg3d/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-15 20:51:47.910897 emg3d-1.8.1/emg3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1263 2022-10-15 20:51:47.000000 emg3d-1.8.1/emg3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-10-15 20:51:47.000000 emg3d-1.8.1/emg3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-15 20:51:47.000000 emg3d-1.8.1/emg3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-10-15 20:51:47.000000 emg3d-1.8.1/emg3d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-15 20:51:47.000000 emg3d-1.8.1/emg3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-15 20:51:47.000000 emg3d-1.8.1/emg3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-15 20:51:47.910897 emg3d-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-10-15 20:51:37.000000 emg3d-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:08:30.386630 emg3d-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-31 15:08:22.000000 emg3d-1.8.2/.rtd-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-31 15:08:22.000000 emg3d-1.8.2/CREDITS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 15:08:22.000000 emg3d-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-31 15:08:30.386630 emg3d-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-31 15:08:22.000000 emg3d-1.8.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:08:30.382629 emg3d-1.8.2/emg3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/_multiprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:08:30.386630 emg3d-1.8.2/emg3d/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14421 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85075 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25488 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/electrodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33822 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16445 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29674 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55472 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/meshes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27594 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64694 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68027 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34755 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/surveys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14717 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-05-31 15:08:22.000000 emg3d-1.8.2/emg3d/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 15:08:30.000000 emg3d-1.8.2/emg3d/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:08:30.382629 emg3d-1.8.2/emg3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-31 15:08:30.000000 emg3d-1.8.2/emg3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-31 15:08:30.000000 emg3d-1.8.2/emg3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:08:30.000000 emg3d-1.8.2/emg3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 15:08:30.000000 emg3d-1.8.2/emg3d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-31 15:08:30.000000 emg3d-1.8.2/emg3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 15:08:30.000000 emg3d-1.8.2/emg3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 15:08:30.386630 emg3d-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-31 15:08:22.000000 emg3d-1.8.2/setup.py
```

### Comparing `emg3d-1.8.1/CREDITS.rst` & `emg3d-1.8.2/CREDITS.rst`

 * *Files identical despite different names*

### Comparing `emg3d-1.8.1/LICENSE` & `emg3d-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `emg3d-1.8.1/PKG-INFO` & `emg3d-1.8.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: emg3d
-Version: 1.8.1
+Version: 1.8.2
 Summary: A multigrid solver for 3D electromagnetic diffusion.
 Home-page: https://emsig.xyz
 Author: The emsig community
 Author-email: info@emsig.xyz
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Provides-Extra: full
 License-File: LICENSE
 
 .. image:: https://raw.github.com/emsig/logos/main/emg3d/emg3d-logo.png
    :target: https://emsig.xyz
    :alt: emg3d logo
```

### Comparing `emg3d-1.8.1/README.rst` & `emg3d-1.8.2/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 .. image:: https://img.shields.io/pypi/v/emg3d.svg
    :target: https://pypi.python.org/pypi/emg3d/
    :alt: PyPI
 .. image:: https://img.shields.io/conda/v/conda-forge/emg3d.svg
    :target: https://anaconda.org/conda-forge/emg3d/
    :alt: conda-forge
-.. image:: https://img.shields.io/badge/python-3.7+-blue.svg
+.. image:: https://img.shields.io/badge/python-3.8+-blue.svg
    :target: https://www.python.org/downloads/
    :alt: Supported Python Versions
 .. image:: https://img.shields.io/badge/platform-linux,win,osx-blue.svg
    :target: https://anaconda.org/conda-forge/emg3d/
    :alt: Linux, Windows, OSX
 
 |
```

### Comparing `emg3d-1.8.1/emg3d/__init__.py` & `emg3d-1.8.2/emg3d/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
@@ -18,15 +18,15 @@
 from emg3d.electrodes import (
     TxElectricPoint, TxMagneticPoint,
     TxElectricDipole, TxMagneticDipole,
     TxElectricWire,
     RxElectricPoint, RxMagneticPoint,
 )
 from emg3d.fields import Field, get_source_field, get_magnetic_field
-from emg3d.io import save, load
+from emg3d.io import save, load, convert
 from emg3d.meshes import TensorMesh, construct_mesh
 from emg3d.models import Model
 from emg3d.simulations import Simulation
 from emg3d.solver import solve, solve_source
 from emg3d.surveys import Survey
 from emg3d.time import Fourier
 from emg3d.utils import Report, __version__
```

### Comparing `emg3d-1.8.1/emg3d/__main__.py` & `emg3d-1.8.2/emg3d/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
```

### Comparing `emg3d-1.8.1/emg3d/_multiprocessing.py` & `emg3d-1.8.2/emg3d/_multiprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Helper routines to call functions with multiprocessing/concurrent.futures.
 """
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
```

### Comparing `emg3d-1.8.1/emg3d/cli/__init__.py` & `emg3d-1.8.2/emg3d/cli/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
```

### Comparing `emg3d-1.8.1/emg3d/cli/main.py` & `emg3d-1.8.2/emg3d/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Entry point for the command-line interface (CLI).
 """
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
```

### Comparing `emg3d-1.8.1/emg3d/cli/parser.py` & `emg3d-1.8.2/emg3d/cli/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Parser for the configuration file of the command-line interface.
 """
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
```

### Comparing `emg3d-1.8.1/emg3d/cli/run.py` & `emg3d-1.8.2/emg3d/cli/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Functions that actually call emg3d within the CLI interface.
 """
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
```

### Comparing `emg3d-1.8.1/emg3d/core.py` & `emg3d-1.8.2/emg3d/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 code of these functions if you are interested in understanding how the
 multigrid solver works, the theory and its implementation.
 
 For a developer interested in making emg3d faster this is the right place to
 start, as by far the most time is spent in these functions, particularly in
 :func:`solve`.
 """
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
```

### Comparing `emg3d-1.8.1/emg3d/electrodes.py` & `emg3d-1.8.2/emg3d/electrodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Electrodes define any type of sources and receivers used in a survey.
 """
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
```

### Comparing `emg3d-1.8.1/emg3d/fields.py` & `emg3d-1.8.2/emg3d/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Everything that is related to fields: storing the electric field, obtaining the
 magnetic field, generating the source field; obtaining the fields at receiver
 locations.
 """
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
```

### Comparing `emg3d-1.8.1/emg3d/io.py` & `emg3d-1.8.2/emg3d/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Utility functions for writing and reading data.
 """
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
@@ -27,15 +27,15 @@
 try:
     import h5py
 except ImportError:
     h5py = None
 
 from emg3d import meshes, utils
 
-__all__ = ['save', 'load']
+__all__ = ['save', 'load', 'convert']
 
 
 def __dir__():
     return __all__
 
 
 def save(fname, **kwargs):
@@ -213,14 +213,31 @@
 
     if verb < 0:
         data = (data, info)
 
     return data
 
 
+def convert(ifname, ofname, **kwargs):
+    """Convert a file that was saved with emg3d to another file format.
+
+    See functions :func:`emg3d.io.load` and :func:`emg3d.io.load` for more
+    information.
+
+
+    Parameters
+    ----------
+    ifname, ofname : str
+        {Input;Output} file names (absolute or relative path) including suffix.
+
+    """
+    data = load(ifname, **kwargs)
+    save(ofname, **data)
+
+
 def _dict_serialize(inp):
     """Serialize emg3d-classes and other objects in inp-dict.
 
     Returns a serialized dictionary <out> of <inp>, where all members of
     `emg3d.utils._KNOWN_CLASSES` are serialized with their respective
     `to_dict()` methods.
```

### Comparing `emg3d-1.8.1/emg3d/maps.py` & `emg3d-1.8.2/emg3d/maps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Mapping routines to map to and from linear conductivities (what is used
 internally) to other representations such as resistivities or logarithms
 thereof.
 
 Interpolation routines mapping values between different grids.
 """
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
@@ -810,14 +810,15 @@
        a minor factor :math:`m`.
 
 
     Parameters
     ----------
     coo : tuple of two ndarrays
         Tuple of two arrays defining the points in x and y:
+
         - If two vectors are given (of same or different size), they are taken
           as the x- and y-values of a regular grid.
         - If two 2D-arrays are given of the same shape, they are taken as the
           (regular or irregular) x- and y-values.
 
     p0, p1 : array_like
         (x, y)-coordinates of two points.
```

### Comparing `emg3d-1.8.1/emg3d/meshes.py` & `emg3d-1.8.2/emg3d/meshes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Everything related to meshes appropriate for the multigrid solver.
 """
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
```

### Comparing `emg3d-1.8.1/emg3d/models.py` & `emg3d-1.8.2/emg3d/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Everything to store electromagnetic material properties for the solver.
 """
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
```

### Comparing `emg3d-1.8.1/emg3d/simulations.py` & `emg3d-1.8.2/emg3d/simulations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 A simulation is the computation (modelling) of the electromagnetic responses
 due to a given model and survey.
 
 The simulation module combines the different pieces of ``emg3d`` providing
 a high-level, specialised modelling tool for the end user.
 """
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
```

### Comparing `emg3d-1.8.1/emg3d/solver.py` & `emg3d-1.8.2/emg3d/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 :func:`emg3d.solver.solve`. The other functions and classes are not meant to be
 called directly, they are all used by the solver internally. It can, however,
 still be insightful to look at the documentation and code of these functions if
 you are interested in understanding how the multigrid solver works, the theory
 and its implementation.
 
 """
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
@@ -87,14 +87,16 @@
 
     sslsolver : {str, bool}, default: True
         A :mod:`scipy.sparse.linalg`-solver, to use with multigrid as
         pre-conditioner or on its own (if ``cycle=None``).
 
         Current possibilities:
 
+            - ``False``: Not used, in which case multigrid acts as solver on
+              its own, not as pre-conditioner.
             - ``True`` or ``'bicgstab'``: BiConjugate Gradient STABilized
               (:func:`scipy.sparse.linalg.bicgstab`).
             - ``'cgs'``: Conjugate Gradient Squared
               (:func:`scipy.sparse.linalg.cgs`).
             - ``'gcrotmk'``: GCROT: Generalized Conjugate Residual with inner
               Orthogonalization and Outer Truncation
               (:func:`scipy.sparse.linalg.gcrotmk`).
```

### Comparing `emg3d-1.8.1/emg3d/surveys.py` & `emg3d-1.8.2/emg3d/surveys.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 A survey stores a set of sources and their frequencies, receivers, and the
 measured data.
 """
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
```

### Comparing `emg3d-1.8.1/emg3d/time.py` & `emg3d-1.8.2/emg3d/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Functionalities related to time-domain modelling using a frequency-domain code.
 """
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
```

### Comparing `emg3d-1.8.1/emg3d/utils.py` & `emg3d-1.8.2/emg3d/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Utility functions for the multigrid solver.
 """
-# Copyright 2018-2022 The emsig community.
+# Copyright 2018 The emsig community.
 #
 # This file is part of emg3d.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
```

### Comparing `emg3d-1.8.1/emg3d.egg-info/PKG-INFO` & `emg3d-1.8.2/emg3d.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: emg3d
-Version: 1.8.1
+Version: 1.8.2
 Summary: A multigrid solver for 3D electromagnetic diffusion.
 Home-page: https://emsig.xyz
 Author: The emsig community
 Author-email: info@emsig.xyz
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Provides-Extra: full
 License-File: LICENSE
 
 .. image:: https://raw.github.com/emsig/logos/main/emg3d/emg3d-logo.png
    :target: https://emsig.xyz
    :alt: emg3d logo
```

### Comparing `emg3d-1.8.1/emg3d.egg-info/SOURCES.txt` & `emg3d-1.8.2/emg3d.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.rtd-requirements.txt
 CREDITS.rst
 LICENSE
 README.rst
 setup.py
 emg3d/__init__.py
 emg3d/__main__.py
 emg3d/_multiprocessing.py
```

### Comparing `emg3d-1.8.1/setup.py` & `emg3d-1.8.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 import os
 import re
 import sys
 from setuptools import setup
 
-if not sys.version_info[:2] >= (3, 7):
-    sys.exit(f"emg3d is only meant for Python 3.7 and up.\n"
+if not sys.version_info[:2] >= (3, 8):
+    sys.exit(f"emg3d is only meant for Python 3.8 and up.\n"
              f"Current version: {sys.version_info[0]}.{sys.version_info[1]}.")
 
 # Get README and remove badges.
 with open("README.rst") as f:
     readme = re.sub(r"\|.*\|", "", f.read(), flags=re.DOTALL)
 
 setup(
@@ -20,29 +20,40 @@
     author_email="info@emsig.xyz",
     url="https://emsig.xyz",
     license="Apache-2.0",
     packages=["emg3d", "emg3d.cli"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     entry_points={
         "console_scripts": [
             "emg3d=emg3d.cli.main:main",
         ],
     },
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=[
-        "scipy>=1.4",
-        "numba>=0.45",
+        "scipy>=1.5",
+        "numba>=0.50",
     ],
+    extras_require={
+        'full': [
+            'tqdm',
+            'h5py',
+            'scooby',
+            'xarray',
+            'empymod',
+            'discretize>=0.7.3',
+            'matplotlib',
+        ],
+    },
     use_scm_version={
         "root": ".",
         "relative_to": __file__,
         "write_to": os.path.join("emg3d", "version.py"),
     },
     setup_requires=["setuptools_scm"],
 )
```

