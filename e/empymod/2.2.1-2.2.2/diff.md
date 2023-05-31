# Comparing `tmp/empymod-2.2.1.tar.gz` & `tmp/empymod-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empymod-2.2.1.tar", last modified: Sat Oct 15 19:27:09 2022, max compression
+gzip compressed data, was "empymod-2.2.2.tar", last modified: Wed May 31 09:31:30 2023, max compression
```

## Comparing `empymod-2.2.1.tar` & `empymod-2.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-15 19:27:09.895101 empymod-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     2549 2022-10-15 19:27:01.000000 empymod-2.2.1/CREDITS.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-10-15 19:27:01.000000 empymod-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16435 2022-10-15 19:27:01.000000 empymod-2.2.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-10-15 19:27:09.895101 empymod-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-10-15 19:27:01.000000 empymod-2.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-15 19:27:09.895101 empymod-2.2.1/empymod/
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-10-15 19:27:01.000000 empymod-2.2.1/empymod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3234 2022-10-15 19:27:01.000000 empymod-2.2.1/empymod/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)   313921 2022-10-15 19:27:01.000000 empymod-2.2.1/empymod/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     7788 2022-10-15 19:27:01.000000 empymod-2.2.1/empymod/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    45556 2022-10-15 19:27:01.000000 empymod-2.2.1/empymod/kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)    71953 2022-10-15 19:27:01.000000 empymod-2.2.1/empymod/model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-15 19:27:09.895101 empymod-2.2.1/empymod/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-10-15 19:27:01.000000 empymod-2.2.1/empymod/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    43263 2022-10-15 19:27:01.000000 empymod-2.2.1/empymod/scripts/fdesign.py
--rw-r--r--   0 runner    (1001) docker     (121)    24270 2022-10-15 19:27:01.000000 empymod-2.2.1/empymod/scripts/tmtemod.py
--rw-r--r--   0 runner    (1001) docker     (121)    44909 2022-10-15 19:27:01.000000 empymod-2.2.1/empymod/transform.py
--rw-r--r--   0 runner    (1001) docker     (121)    65813 2022-10-15 19:27:01.000000 empymod-2.2.1/empymod/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-15 19:27:09.000000 empymod-2.2.1/empymod/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-15 19:27:09.895101 empymod-2.2.1/empymod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-10-15 19:27:09.000000 empymod-2.2.1/empymod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-10-15 19:27:09.000000 empymod-2.2.1/empymod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-15 19:27:09.000000 empymod-2.2.1/empymod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-10-15 19:27:09.000000 empymod-2.2.1/empymod.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-15 19:27:09.000000 empymod-2.2.1/empymod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-15 19:27:09.000000 empymod-2.2.1/empymod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-15 19:27:09.895101 empymod-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-10-15 19:27:01.000000 empymod-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:31:30.066267 empymod-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-31 09:31:21.000000 empymod-2.2.2/CREDITS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-31 09:31:21.000000 empymod-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-05-31 09:31:21.000000 empymod-2.2.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-31 09:31:30.062267 empymod-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-31 09:31:21.000000 empymod-2.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:31:30.062267 empymod-2.2.2/empymod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-31 09:31:21.000000 empymod-2.2.2/empymod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-31 09:31:21.000000 empymod-2.2.2/empymod/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   313952 2023-05-31 09:31:21.000000 empymod-2.2.2/empymod/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-05-31 09:31:21.000000 empymod-2.2.2/empymod/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45587 2023-05-31 09:31:21.000000 empymod-2.2.2/empymod/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72378 2023-05-31 09:31:21.000000 empymod-2.2.2/empymod/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:31:30.062267 empymod-2.2.2/empymod/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-31 09:31:21.000000 empymod-2.2.2/empymod/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43294 2023-05-31 09:31:21.000000 empymod-2.2.2/empymod/scripts/fdesign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24301 2023-05-31 09:31:21.000000 empymod-2.2.2/empymod/scripts/tmtemod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44941 2023-05-31 09:31:21.000000 empymod-2.2.2/empymod/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66281 2023-05-31 09:31:21.000000 empymod-2.2.2/empymod/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 09:31:29.000000 empymod-2.2.2/empymod/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:31:30.062267 empymod-2.2.2/empymod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-31 09:31:29.000000 empymod-2.2.2/empymod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-31 09:31:29.000000 empymod-2.2.2/empymod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:31:29.000000 empymod-2.2.2/empymod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 09:31:29.000000 empymod-2.2.2/empymod.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 09:31:29.000000 empymod-2.2.2/empymod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 09:31:29.000000 empymod-2.2.2/empymod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:31:30.066267 empymod-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-31 09:31:21.000000 empymod-2.2.2/setup.py
```

### Comparing `empymod-2.2.1/CREDITS.rst` & `empymod-2.2.2/CREDITS.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Credits
 #######
 
 This project was started by **Dieter Werthmüller** at
 `The Mexican Institute of Petroleum IMP <https://www.gob.mx/imp>`_
 (Instituto Mexicano del Petróleo), funded (till 01/2017) by
 `The Mexican National Council of Science and Technology
-<https://www.conacyt.gob.mx>`_ (Consejo Nacional de Ciencia y Tecnología).
+<https://conahcyt.mx>`_ (Consejo Nacional de Ciencia y Tecnología).
 Dieter would like to thank his past and current employers who allowed and allow
 him to maintain and further develop the code after the initial funding ended,
 namely:
 
 - 2017-2018: `The Mexican Institute of Petroleum IMP <https://www.gob.mx/imp>`_
 
 - 2018-today: `Delft University of Technology <https://www.tudelft.nl>`_
```

### Comparing `empymod-2.2.1/LICENSE` & `empymod-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `empymod-2.2.1/NOTICE` & `empymod-2.2.2/NOTICE`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 empymod
-Copyright 2016-2022 The emsig community.
+Copyright 2016 The emsig community.
 
 This software was initially (till 01/2017) developed with funding from
 *The Mexican National Council of Science and Technology*
-(*Consejo Nacional de Ciencia y Tecnología*, http://www.conacyt.gob.mx),
+(*Consejo Nacional de Ciencia y Tecnología*, http://conahcyt.mx),
 carried out at *The Mexican Institute of Petroleum IMP*
 (*Instituto Mexicano del Petróleo*, http://www.gob.mx/imp).
 
 
 This product is a derivative work of Hunziker et al, 2015, and Key, 2012,
 and their publicly available software:
```

### Comparing `empymod-2.2.1/PKG-INFO` & `empymod-2.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: empymod
-Version: 2.2.1
+Version: 2.2.2
 Summary: Open-source full 3D electromagnetic modeller for 1D VTI media
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
 License-File: LICENSE
 License-File: NOTICE
 
 .. image:: https://raw.github.com/emsig/logos/main/empymod/empymod-logo.png
    :target: https://emsig.xyz
    :alt: empymod logo
```

### Comparing `empymod-2.2.1/README.rst` & `empymod-2.2.2/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 .. image:: https://img.shields.io/pypi/v/empymod.svg
    :target: https://pypi.python.org/pypi/empymod/
    :alt: PyPI
 .. image:: https://img.shields.io/conda/v/conda-forge/empymod.svg
    :target: https://anaconda.org/conda-forge/empymod/
    :alt: conda-forge
-.. image:: https://img.shields.io/badge/python-3.7+-blue.svg
+.. image:: https://img.shields.io/badge/python-3.8+-blue.svg
    :target: https://www.python.org/downloads/
    :alt: Supported Python Versions
 .. image:: https://img.shields.io/badge/platform-linux,win,osx-blue.svg
    :target: https://anaconda.org/conda-forge/empymod/
    :alt: Linux, Windows, OSX
 
 |
```

### Comparing `empymod-2.2.1/empymod/__init__.py` & `empymod-2.2.2/empymod/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2016-2022 The emsig community.
+# Copyright 2016 The emsig community.
 #
 # This file is part of empymod.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
```

### Comparing `empymod-2.2.1/empymod/__main__.py` & `empymod-2.2.2/empymod/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Entry point for the command-line interface (CLI).
 """
-# Copyright 2016-2022 The emsig community.
+# Copyright 2016 The emsig community.
 #
 # This file is part of empymod.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
```

### Comparing `empymod-2.2.1/empymod/filters.py` & `empymod-2.2.2/empymod/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 distributed with [Key12]_ and available at https://software.seg.org/2012/0003
 ([SEG-2012-003]_). These filters are distributed under the SEG license.
 
 The filter `wer_201_2018` was designed with the add-on `fdesign`, see
 https://github.com/emsig/article-fdesign.
 
 """
-# Copyright 2016-2022 The emsig community.
+# Copyright 2016 The emsig community.
 #
 # This file is part of empymod.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
@@ -51,14 +51,18 @@
 __all__ = ['DigitalFilter', 'kong_61_2007', 'kong_241_2007', 'key_101_2009',
            'key_201_2009', 'key_401_2009', 'anderson_801_1982', 'key_51_2012',
            'key_101_2012', 'key_201_2012', 'wer_201_2018',
            'key_81_CosSin_2009', 'key_241_CosSin_2009', 'key_601_CosSin_2009',
            'key_101_CosSin_2012', 'key_201_CosSin_2012']
 
 
+def __dir__():
+    return __all__
+
+
 # 0. Filter Class and saving/loading routines
 
 class DigitalFilter:
     r"""Simple Class for Digital Linear Filters.
 
 
     Parameters
```

### Comparing `empymod-2.2.1/empymod/io.py` & `empymod-2.2.2/empymod/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Utility functions for writing and reading inputs and data.
 """
-# Copyright 2016-2022 The emsig community.
+# Copyright 2016 The emsig community.
 #
 # This file is part of empymod.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
@@ -26,14 +26,18 @@
 
 
 from empymod import utils
 
 __all__ = ["save_input", "load_input", "save_data", "load_data"]
 
 
+def __dir__():
+    return __all__
+
+
 def save_input(fname, data, **kwargs):
     """Save input dict to disk.
 
     Save the input provided to an empymod modelling routine on disk.
 
 
     Parameters
```

### Comparing `empymod-2.2.1/empymod/kernel.py` & `empymod-2.2.2/empymod/kernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [HuTS15]_, which can be found at `software.seg.org/2015/0001
 <https://software.seg.org/2015/0001>`_.  These functions are (c) 2015 by
 Hunziker et al. and the Society of Exploration Geophysicists,
 https://software.seg.org/disclaimer.txt.  Please read the NOTICE-file in the
 root directory for more information regarding the involved licenses.
 
 """
-# Copyright 2016-2022 The emsig community.
+# Copyright 2016 The emsig community.
 #
 # This file is part of empymod.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
@@ -36,14 +36,18 @@
            'reflections', 'fields', 'halfspace']
 
 # Numba-settings
 _numba_setting = {'nogil': True, 'cache': True}
 _numba_with_fm = {'fastmath': True, **_numba_setting}
 
 
+def __dir__():
+    return __all__
+
+
 # Wavenumber-frequency domain kernel
 
 @nb.njit(**_numba_setting)
 def wavenumber(zsrc, zrec, lsrc, lrec, depth, etaH, etaV, zetaH, zetaV, lambd,
                ab, xdirect, msrc, mrec):
     r"""Calculate wavenumber domain solution.
```

### Comparing `empymod-2.2.1/empymod/model.py` & `empymod-2.2.2/empymod/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 - :func:`fem`: Calculate wavenumber-domain electromagnetic field and carry out
   the Hankel transform to the frequency domain.
 - :func:`tem`: Carry out the Fourier transform to time domain after
   :func:`fem`.
 
 """
-# Copyright 2016-2022 The emsig community.
+# Copyright 2016 The emsig community.
 #
 # This file is part of empymod.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
@@ -62,14 +62,18 @@
         check_solution, get_abs, get_geo_fact, get_azm_dip, get_off_ang,
         get_layer_nr, get_kwargs, printstartfinish, conv_warning, EMArray)
 
 __all__ = ['bipole', 'dipole', 'loop', 'analytical', 'gpr', 'dipole_k', 'fem',
            'tem']
 
 
+def __dir__():
+    return __all__
+
+
 def bipole(src, rec, depth, res, freqtime, signal=None, aniso=None,
            epermH=None, epermV=None, mpermH=None, mpermV=None, msrc=False,
            srcpts=1, mrec=False, recpts=1, strength=0, **kwargs):
     r"""Return EM fields due to arbitrary rotated, finite length EM dipoles.
 
     Calculate the electromagnetic frequency- or time-domain field due to
     arbitrary rotated, finite electric or magnetic bipole sources, measured by
@@ -585,16 +589,17 @@
 
 
     Parameters
     ----------
     src, rec : list of floats or arrays
         Source and receiver coordinates [x, y, z] (m):
 
-        - The x- and y-coordinates can be arrays, z is a single value.
-        - The x- and y-coordinates must have the same dimension.
+        For `N` sources or receivers, the x- and y-coordinates must be of size
+        `N` or 1 (in the latter case it will be expanded to `N`); z is always a
+        single value.
 
         Sources or receivers placed on a layer interface are considered in the
         upper layer.
 
     depth : list
         Absolute layer interfaces z (m); #depth = #res - 1
         (excluding +/- infinity).
@@ -1201,15 +1206,17 @@
     Calculate the electromagnetic frequency- or time-domain field due to
     infinitesimal small electric or magnetic dipole source(s), measured by
     infinitesimal small electric or magnetic dipole receiver(s); sources and
     receivers are directed along the principal directions x, y, or z, and all
     sources are at the same depth, as well as all receivers are at the same
     depth.
 
-    In the case of a halfspace the air-interface is located at z = 0 m.
+    In the case of a halfspace the air-interface is located at z = 0 m, and
+    both sources and receiver must be either at the interface or within the
+    subsurface, not in the air (this is NOT checked by the code).
 
     You can call the functions :func:`empymod.kernel.fullspace` and
     :func:`empymod.kernel.halfspace` in :mod:`empymod.kernel` directly. This
     interface is just to provide a consistent interface with the same input
     parameters as for instance for :func:`dipole`.
 
     This function yields the same result if `solution='fs'` as :func:`dipole`,
@@ -1227,16 +1234,20 @@
       for ee-fields, split into TE and TM mode [SlHM10]_.
 
     Parameters
     ----------
     src, rec : list of floats or arrays
         Source and receiver coordinates [x, y, z] (m):
 
-        - The x- and y-coordinates can be arrays, z is a single value.
-        - The x- and y-coordinates must have the same dimension.
+        For `N` sources or receivers, the x- and y-coordinates must be of size
+        `N` or 1 (in the latter case it will be expanded to `N`); z is always a
+        single value.
+
+        In the case of the diffusive halfspace, ``z`` is assumed to be at the
+        interface or below.
 
     res : float
         Horizontal resistivity rho_h (Ohm.m).
 
         Alternatively, res can be a dictionary. See the main manual of empymod
         too see how to exploit this hook to re-calculate etaH, etaV, zetaH, and
         zetaV, which can be used to, for instance, use the Cole-Cole model for
@@ -1554,16 +1565,17 @@
 
 
     Parameters
     ----------
     src, rec : list of floats or arrays
         Source and receiver coordinates [x, y, z] (m):
 
-        - The x- and y-coordinates can be arrays, z is a single value.
-        - The x- and y-coordinates must have the same dimension.
+        - For `N` sources or receivers, the x- and y-coordinates must be of
+          size `N` or 1 (in the latter case it will be expanded to `N`); z is
+          always a single value.
         - The x- and y-coordinates only matter for the angle-dependent factor.
 
         Sources or receivers placed on a layer interface are considered in the
         upper layer.
 
     depth : list
         Absolute layer interfaces z (m); #depth = #res - 1
```

### Comparing `empymod-2.2.1/empymod/scripts/__init__.py` & `empymod-2.2.2/empymod/scripts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2016-2022 The emsig community.
+# Copyright 2016 The emsig community.
 #
 # This file is part of empymod.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
```

### Comparing `empymod-2.2.1/empymod/scripts/fdesign.py` & `empymod-2.2.2/empymod/scripts/fdesign.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
       :label: cos3
 
       \int^\infty_0 \frac{1}{a^2+l^2} \cos(lr) dl =
       \frac{\pi}{2a} \exp\left(-ar\right)
 
 
 """
-# Copyright 2016-2022 The emsig community.
+# Copyright 2016 The emsig community.
 #
 # This file is part of empymod.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
@@ -243,14 +243,18 @@
 
 __all__ = ['design', 'save_filter', 'load_filter', 'plot_result',
            'print_result', 'Ghosh', 'j0_1', 'j0_2', 'j0_3', 'j0_4', 'j0_5',
            'j1_1', 'j1_2', 'j1_3', 'j1_4', 'j1_5', 'sin_1', 'sin_2', 'sin_3',
            'cos_1', 'cos_2', 'cos_3', 'empy_hankel']
 
 
+def __dir__():
+    return __all__
+
+
 # 1. PRINCIPAL FILTER DESIGNING ROUTINES
 
 @np.errstate(all='ignore')
 def design(n, spacing, shift, fI, fC=False, r=None, r_def=(1, 1, 2), reim=None,
            cvar='amp', error=0.01, name=None, full_output=False, finish=False,
            save=True, path='filters', verb=2, plot=1):
     r"""Digital linear filter (DLF) design
```

### Comparing `empymod-2.2.1/empymod/scripts/tmtemod.py` & `empymod-2.2.2/empymod/scripts/tmtemod.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,15 +324,15 @@
 .. math::
     :label: hun28
 
     \cos(2\phi) = -\frac{x^2-y^2}{r^2} \ .
 
 
 """
-# Copyright 2016-2022 The emsig community.
+# Copyright 2016 The emsig community.
 #
 # This file is part of empymod.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
@@ -350,14 +350,18 @@
 from empymod.kernel import reflections, angle_factor
 from empymod.utils import (check_model, check_frequency, check_dipole, _strvar,
                            get_off_ang, get_layer_nr, printstartfinish)
 
 __all__ = ['dipole']
 
 
+def __dir__():
+    return __all__
+
+
 def dipole(src, rec, depth, res, freqtime, aniso=None, eperm=None, mperm=None,
            verb=2):
     r"""Return the electromagnetic field due to a dipole source.
 
     This is a modified version of :func:`empymod.model.dipole`. It returns the
     separated contributions of TM--, TM-+, TM+-, TM++, TMdirect, TE--, TE-+,
     TE+-, TE++, and TEdirect.
```

### Comparing `empymod-2.2.1/empymod/transform.py` & `empymod-2.2.2/empymod/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [Key12]_, which can be found at `software.seg.org/2012/0003
 <https://software.seg.org/2012/0003>`_. These functions are (c) 2012 by Kerry
 Key and the Society of Exploration Geophysicists,
 https://software.seg.org/disclaimer.txt. Please read the NOTICE-file in the
 root directory for more information regarding the involved licenses.
 
 """
-# Copyright 2016-2022 The emsig community.
+# Copyright 2016 The emsig community.
 #
 # This file is part of empymod.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
@@ -34,14 +34,18 @@
 from empymod import kernel
 
 __all__ = ['hankel_dlf', 'hankel_qwe', 'hankel_quad', 'fourier_dlf',
            'fourier_qwe', 'fourier_fftlog', 'fourier_fft', 'dlf', 'qwe',
            'get_dlf_points', 'get_fftlog_input']
 
 
+def __dir__():
+    return __all__
+
+
 # 1. Hankel transforms (wavenumber -> frequency)
 
 def hankel_dlf(zsrc, zrec, lsrc, lrec, off, ang_fact, depth, ab, etaH, etaV,
                zetaH, zetaV, xdirect, htarg, msrc, mrec):
     r"""Hankel Transform using the Digital Linear Filter method.
 
     The *Digital Linear Filter* method was introduced to geophysics by
@@ -649,15 +653,15 @@
 
 
 def fourier_fftlog(fEM, time, freq, ftarg):
     r"""Fourier Transform using FFTLog.
 
     FFTLog is the logarithmic analogue to the Fast Fourier Transform FFT.
     FFTLog was presented in Appendix B of [Hami00]_ and published at
-    http://casa.colorado.edu/~ajsh/FFTLog.
+    https://casa.colorado.edu/~ajsh/FFTLog.
 
     This function uses a simplified version of `pyfftlog`, which is a
     python-version of `FFTLog`. For more details regarding `pyfftlog` see
     https://github.com/prisae/pyfftlog.
 
     Not the full flexibility of `FFTLog` is available here: Only the
     logarithmic FFT (`fftl` in `FFTLog`), not the Hankel transform
```

### Comparing `empymod-2.2.1/empymod/utils.py` & `empymod-2.2.2/empymod/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This module consists of four groups of functions:
    0. General settings
    1. Class EMArray
    2. Input parameter checks for modelling
    3. Internal utilities
 
 """
-# Copyright 2016-2022 The emsig community.
+# Copyright 2016 The emsig community.
 #
 # This file is part of empymod.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not
 # use this file except in compliance with the License.  You may obtain a copy
 # of the License at
 #
@@ -70,14 +70,18 @@
 _min_time = 1e-20   # Minimum time       [s]
 _min_off = 1e-3     # Minimum offset     [m]
 #                   # > Also used to round src- & rec-coordinates (1e-3 => mm)
 _min_res = 1e-20    # Minimum value for horizontal/vertical resistivity
 _min_angle = 1e-10  # Angle factors smaller than that are set to 0
 
 
+def __dir__():
+    return __all__
+
+
 # 1. Class EMArray
 
 class EMArray(np.ndarray):
     r"""Create an EM-ndarray: add *amplitude* <amp> and *phase* <pha> methods.
 
     Parameters
     ----------
@@ -353,18 +357,31 @@
         List of pole coordinates [x, y, z].
 
     ninp : int
         Number of inp-elements
 
     """
 
-    # Check inp for x, y, and z; x & y must have same length, z is a float
+    # Check inp for x, y, and z; x & y must be of size N or 1, z is a float
     _check_shape(np.squeeze(np.asarray(inp, dtype=object)), name, (3,))
     inp_x = _check_var(inp[0], float, 1, name+'-x')
-    inp_y = _check_var(inp[1], float, 1, name+'-y', inp_x.shape)
+    inp_y = _check_var(inp[1], float, 1, name+'-y')
+
+    # Expand x or y coordinate if necessary.
+    if inp_x.size != inp_y.size:
+        if inp_x.size == 1:
+            inp_x = np.repeat(inp_x, inp_y.size)
+        elif inp_y.size == 1:
+            inp_y = np.repeat(inp_y, inp_x.size)
+        else:
+            raise ValueError(
+                f"Parameters {name}-x and {name}-y must be of same size or "
+                f"be a single value; provided: {inp_x.shape}; {inp_y.shape}."
+            )
+
     inp_z = _check_var(inp[2], float, 1, name+'-z', (1,))
     out = [inp_x, inp_y, inp_z]
 
     # Print spatial parameters
     if verb > 2:
         # Pole-type: src or rec
         if name == 'src':
```

### Comparing `empymod-2.2.1/empymod.egg-info/PKG-INFO` & `empymod-2.2.2/empymod.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: empymod
-Version: 2.2.1
+Version: 2.2.2
 Summary: Open-source full 3D electromagnetic modeller for 1D VTI media
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
 License-File: LICENSE
 License-File: NOTICE
 
 .. image:: https://raw.github.com/emsig/logos/main/empymod/empymod-logo.png
    :target: https://emsig.xyz
    :alt: empymod logo
```

### Comparing `empymod-2.2.1/setup.py` & `empymod-2.2.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 import os
 import re
 import sys
 from setuptools import setup
 
-if not sys.version_info[:2] >= (3, 7):
-    sys.exit(f"empymod is only meant for Python 3.7 and up.\n"
+if not sys.version_info[:2] >= (3, 8):
+    sys.exit(f"empymod is only meant for Python 3.8 and up.\n"
              f"Current version: {sys.version_info[0]}.{sys.version_info[1]}.")
 
 # Get README and remove badges.
 with open("README.rst") as f:
     readme = re.sub(r"\|.*\|", "", f.read(), flags=re.DOTALL)
 
 description = "Open-source full 3D electromagnetic modeller for 1D VTI media"
@@ -22,28 +22,28 @@
     author_email="info@emsig.xyz",
     url="https://emsig.xyz",
     license="Apache-2.0",
     packages=["empymod", "empymod.scripts"],
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
             "empymod=empymod.__main__:main",
         ],
     },
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=[
-        "scipy>=1.4",
-        "numba>=0.47",
+        "scipy>=1.5",
+        "numba>=0.50",
     ],
     use_scm_version={
         "root": ".",
         "relative_to": __file__,
         "write_to": os.path.join("empymod", "version.py"),
     },
     setup_requires=["setuptools_scm"],
```

