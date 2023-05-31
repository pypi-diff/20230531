# Comparing `tmp/servalcat-0.4.15.tar.gz` & `tmp/servalcat-0.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servalcat-0.4.15.tar", last modified: Thu Apr 20 18:25:34 2023, max compression
+gzip compressed data, was "servalcat-0.4.24.tar", last modified: Wed May 31 20:36:14 2023, max compression
```

## Comparing `servalcat-0.4.15.tar` & `servalcat-0.4.24.tar`

### file list

```diff
@@ -1,88 +1,744 @@
-drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-04-20 18:25:34.759126 servalcat-0.4.15/
--rw-r--r--   0 yam        (501) staff       (20)     1818 2021-02-16 09:47:12.000000 servalcat-0.4.15/.gitignore
--rw-r--r--   0 yam        (501) staff       (20)    16725 2021-02-16 09:46:34.000000 servalcat-0.4.15/LICENSE
--rw-r--r--   0 yam        (501) staff       (20)      315 2023-04-20 18:25:34.758750 servalcat-0.4.15/PKG-INFO
--rw-r--r--   0 yam        (501) staff       (20)     1233 2023-04-20 16:43:48.000000 servalcat-0.4.15/README.md
-drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-04-20 18:25:34.725757 servalcat-0.4.15/gemmi/
-drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-04-20 18:25:34.731030 servalcat-0.4.15/gemmi/src/
--rw-r--r--   0 yam        (501) staff       (20)     5709 2023-04-20 16:43:48.000000 servalcat-0.4.15/gemmi/src/eig3.cpp
--rw-r--r--   0 yam        (501) staff       (20)    20572 2023-04-20 16:43:48.000000 servalcat-0.4.15/gemmi/src/monlib.cpp
--rw-r--r--   0 yam        (501) staff       (20)     9007 2023-04-20 16:43:48.000000 servalcat-0.4.15/gemmi/src/polyheur.cpp
--rw-r--r--   0 yam        (501) staff       (20)    24654 2023-04-20 16:43:48.000000 servalcat-0.4.15/gemmi/src/resinfo.cpp
--rw-r--r--   0 yam        (501) staff       (20)    17837 2023-04-20 16:43:48.000000 servalcat-0.4.15/gemmi/src/riding_h.cpp
--rw-r--r--   0 yam        (501) staff       (20)    39163 2023-04-20 16:43:48.000000 servalcat-0.4.15/gemmi/src/topo.cpp
--rw-r--r--   0 yam        (501) staff       (20)       51 2023-04-18 18:05:48.000000 servalcat-0.4.15/pyproject.toml
-drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-04-20 18:25:34.732588 servalcat-0.4.15/servalcat/
--rw-r--r--   0 yam        (501) staff       (20)      231 2023-04-20 17:27:15.000000 servalcat-0.4.15/servalcat/__init__.py
--rw-r--r--   0 yam        (501) staff       (20)     4297 2023-04-18 18:05:48.000000 servalcat-0.4.15/servalcat/command_line.py
-drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-04-20 18:25:34.738334 servalcat-0.4.15/servalcat/refine/
--rw-r--r--   0 yam        (501) staff       (20)        0 2023-04-18 18:00:38.000000 servalcat-0.4.15/servalcat/refine/__init__.py
--rw-r--r--   0 yam        (501) staff       (20)     3072 2023-04-18 18:00:38.000000 servalcat-0.4.15/servalcat/refine/cgsolve.py
--rw-r--r--   0 yam        (501) staff       (20)    20065 2023-04-20 16:40:18.000000 servalcat-0.4.15/servalcat/refine/refine.py
--rw-r--r--   0 yam        (501) staff       (20)     7844 2023-04-20 16:43:48.000000 servalcat-0.4.15/servalcat/refine/refine_geom.py
--rw-r--r--   0 yam        (501) staff       (20)    14762 2023-04-20 16:43:48.000000 servalcat-0.4.15/servalcat/refine/refine_spa.py
--rw-r--r--   0 yam        (501) staff       (20)     8403 2023-04-20 16:40:18.000000 servalcat-0.4.15/servalcat/refine/refine_xtal.py
--rw-r--r--   0 yam        (501) staff       (20)     5806 2023-04-18 18:05:48.000000 servalcat-0.4.15/servalcat/refine/spa.py
--rw-r--r--   0 yam        (501) staff       (20)    13940 2023-04-20 16:40:18.000000 servalcat-0.4.15/servalcat/refine/xtal.py
-drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-04-20 18:25:34.739865 servalcat-0.4.15/servalcat/refmac/
--rw-r--r--   0 yam        (501) staff       (20)        0 2023-04-18 17:58:34.000000 servalcat-0.4.15/servalcat/refmac/__init__.py
--rw-r--r--   0 yam        (501) staff       (20)     8836 2023-04-18 18:05:48.000000 servalcat-0.4.15/servalcat/refmac/exte.py
--rw-r--r--   0 yam        (501) staff       (20)    21554 2023-04-18 18:05:48.000000 servalcat-0.4.15/servalcat/refmac/refmac_keywords.py
--rw-r--r--   0 yam        (501) staff       (20)    12595 2023-04-20 16:43:48.000000 servalcat-0.4.15/servalcat/refmac/refmac_wrapper.py
-drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-04-20 18:25:34.746947 servalcat-0.4.15/servalcat/spa/
--rw-r--r--   0 yam        (501) staff       (20)        0 2022-11-13 21:58:00.000000 servalcat-0.4.15/servalcat/spa/__init__.py
--rw-r--r--   0 yam        (501) staff       (20)     3982 2022-11-13 21:58:00.000000 servalcat-0.4.15/servalcat/spa/est_local_luzzati_d.py
--rw-r--r--   0 yam        (501) staff       (20)     1754 2022-11-13 21:58:00.000000 servalcat-0.4.15/servalcat/spa/estimate_mixture.py
--rw-r--r--   0 yam        (501) staff       (20)     1860 2022-11-13 21:58:00.000000 servalcat-0.4.15/servalcat/spa/find_translation.py
--rw-r--r--   0 yam        (501) staff       (20)    21743 2023-04-18 18:00:38.000000 servalcat-0.4.15/servalcat/spa/fofc.py
--rw-r--r--   0 yam        (501) staff       (20)      996 2022-11-13 21:58:00.000000 servalcat-0.4.15/servalcat/spa/fofc_rms.py
--rw-r--r--   0 yam        (501) staff       (20)    15014 2023-04-20 16:40:18.000000 servalcat-0.4.15/servalcat/spa/fsc.py
--rw-r--r--   0 yam        (501) staff       (20)    10227 2022-11-23 16:39:29.000000 servalcat-0.4.15/servalcat/spa/fsc2.py
--rw-r--r--   0 yam        (501) staff       (20)     7945 2023-04-18 18:05:48.000000 servalcat-0.4.15/servalcat/spa/localcc.py
--rw-r--r--   0 yam        (501) staff       (20)     5275 2023-04-18 17:58:34.000000 servalcat-0.4.15/servalcat/spa/realspcc_from_var.py
--rw-r--r--   0 yam        (501) staff       (20)      372 2022-11-13 21:58:00.000000 servalcat-0.4.15/servalcat/spa/refine_emdb.py
--rw-r--r--   0 yam        (501) staff       (20)    47515 2023-04-20 16:43:48.000000 servalcat-0.4.15/servalcat/spa/run_refmac.py
--rw-r--r--   0 yam        (501) staff       (20)    13149 2023-04-18 18:00:38.000000 servalcat-0.4.15/servalcat/spa/shift_maps.py
--rw-r--r--   0 yam        (501) staff       (20)     4664 2023-04-18 17:58:34.000000 servalcat-0.4.15/servalcat/spa/shiftback.py
--rw-r--r--   0 yam        (501) staff       (20)     5091 2023-04-18 17:58:34.000000 servalcat-0.4.15/servalcat/spa/translate.py
--rw-r--r--   0 yam        (501) staff       (20)     6871 2022-11-13 21:58:00.000000 servalcat-0.4.15/servalcat/spa/tst_gemmi_mottbethe.py
--rw-r--r--   0 yam        (501) staff       (20)     1076 2022-11-13 21:58:00.000000 servalcat-0.4.15/servalcat/spa/tst_refmac_fc.py
--rw-r--r--   0 yam        (501) staff       (20)      519 2023-02-14 21:17:59.000000 servalcat-0.4.15/servalcat/test_installation.py
-drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-04-20 18:25:34.753516 servalcat-0.4.15/servalcat/utils/
--rw-r--r--   0 yam        (501) staff       (20)     1146 2023-04-18 18:05:36.000000 servalcat-0.4.15/servalcat/utils/__init__.py
--rw-r--r--   0 yam        (501) staff       (20)    49622 2023-04-20 17:23:15.000000 servalcat-0.4.15/servalcat/utils/commands.py
--rw-r--r--   0 yam        (501) staff       (20)    28768 2023-04-20 16:43:48.000000 servalcat-0.4.15/servalcat/utils/fileio.py
--rw-r--r--   0 yam        (501) staff       (20)    10867 2022-11-13 21:58:00.000000 servalcat-0.4.15/servalcat/utils/generate_operators.py
--rw-r--r--   0 yam        (501) staff       (20)    25005 2023-04-20 16:40:18.000000 servalcat-0.4.15/servalcat/utils/hkl.py
--rw-r--r--   0 yam        (501) staff       (20)     3524 2023-04-18 18:05:48.000000 servalcat-0.4.15/servalcat/utils/logger.py
--rw-r--r--   0 yam        (501) staff       (20)    13101 2023-04-18 18:05:48.000000 servalcat-0.4.15/servalcat/utils/maps.py
--rw-r--r--   0 yam        (501) staff       (20)    28626 2023-04-20 16:40:18.000000 servalcat-0.4.15/servalcat/utils/model.py
--rw-r--r--   0 yam        (501) staff       (20)    29717 2023-04-18 18:05:48.000000 servalcat-0.4.15/servalcat/utils/refmac.py
--rw-r--r--   0 yam        (501) staff       (20)      889 2022-11-13 21:58:00.000000 servalcat-0.4.15/servalcat/utils/refmac_params.py
--rw-r--r--   0 yam        (501) staff       (20)    16790 2023-04-20 16:43:48.000000 servalcat-0.4.15/servalcat/utils/restraints.py
--rw-r--r--   0 yam        (501) staff       (20)     4796 2022-11-13 21:58:00.000000 servalcat-0.4.15/servalcat/utils/scaling.py
--rw-r--r--   0 yam        (501) staff       (20)    11879 2023-04-18 18:00:38.000000 servalcat-0.4.15/servalcat/utils/symmetry.py
-drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-04-20 18:25:34.755092 servalcat-0.4.15/servalcat/xtal/
--rw-r--r--   0 yam        (501) staff       (20)        0 2022-11-13 21:58:00.000000 servalcat-0.4.15/servalcat/xtal/__init__.py
--rw-r--r--   0 yam        (501) staff       (20)     9665 2023-04-18 18:05:48.000000 servalcat-0.4.15/servalcat/xtal/french_wilson.py
--rw-r--r--   0 yam        (501) staff       (20)    11031 2023-04-20 16:40:18.000000 servalcat-0.4.15/servalcat/xtal/run_refmac_small.py
--rw-r--r--   0 yam        (501) staff       (20)    45509 2023-04-20 16:40:18.000000 servalcat-0.4.15/servalcat/xtal/sigmaa.py
-drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-04-20 18:25:34.735347 servalcat-0.4.15/servalcat.egg-info/
--rw-r--r--   0 yam        (501) staff       (20)      315 2023-04-20 18:25:34.000000 servalcat-0.4.15/servalcat.egg-info/PKG-INFO
--rw-r--r--   0 yam        (501) staff       (20)     1935 2023-04-20 18:25:34.000000 servalcat-0.4.15/servalcat.egg-info/SOURCES.txt
--rw-r--r--   0 yam        (501) staff       (20)        1 2023-04-20 18:25:34.000000 servalcat-0.4.15/servalcat.egg-info/dependency_links.txt
--rw-r--r--   0 yam        (501) staff       (20)      115 2023-04-20 18:25:34.000000 servalcat-0.4.15/servalcat.egg-info/entry_points.txt
--rw-r--r--   0 yam        (501) staff       (20)        1 2021-02-16 10:41:57.000000 servalcat-0.4.15/servalcat.egg-info/not-zip-safe
--rw-r--r--   0 yam        (501) staff       (20)       46 2023-04-20 18:25:34.000000 servalcat-0.4.15/servalcat.egg-info/requires.txt
--rw-r--r--   0 yam        (501) staff       (20)       10 2023-04-20 18:25:34.000000 servalcat-0.4.15/servalcat.egg-info/top_level.txt
--rw-r--r--   0 yam        (501) staff       (20)       38 2023-04-20 18:25:34.759263 servalcat-0.4.15/setup.cfg
--rw-r--r--   0 yam        (501) staff       (20)     4900 2023-04-20 16:43:48.000000 servalcat-0.4.15/setup.py
-drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-04-20 18:25:34.756460 servalcat-0.4.15/src/
--rw-r--r--   0 yam        (501) staff       (20)     1616 2023-04-18 18:05:48.000000 servalcat-0.4.15/src/ext.cpp
--rw-r--r--   0 yam        (501) staff       (20)    13910 2023-04-18 18:05:48.000000 servalcat-0.4.15/src/intensity.cpp
--rw-r--r--   0 yam        (501) staff       (20)    27159 2023-04-20 16:40:18.000000 servalcat-0.4.15/src/refine.cpp
-drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-04-20 18:25:34.758198 servalcat-0.4.15/tests/
--rw-r--r--   0 yam        (501) staff       (20)     1334 2023-04-18 18:05:48.000000 servalcat-0.4.15/tests/test_misc.py
--rw-r--r--   0 yam        (501) staff       (20)     1831 2023-04-18 18:05:48.000000 servalcat-0.4.15/tests/test_refine.py
--rw-r--r--   0 yam        (501) staff       (20)    12128 2023-04-18 18:05:48.000000 servalcat-0.4.15/tests/test_spa.py
--rw-r--r--   0 yam        (501) staff       (20)     5495 2023-04-18 18:05:48.000000 servalcat-0.4.15/tests/test_xtal.py
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.762642 servalcat-0.4.24/
+-rw-r--r--   0 yam        (501) staff       (20)    16725 2021-02-16 09:46:34.000000 servalcat-0.4.24/LICENSE
+-rw-r--r--   0 yam        (501) staff       (20)      185 2023-05-05 06:36:41.000000 servalcat-0.4.24/MANIFEST.in
+-rw-r--r--   0 yam        (501) staff       (20)      398 2023-05-31 20:36:14.762234 servalcat-0.4.24/PKG-INFO
+-rw-r--r--   0 yam        (501) staff       (20)     1431 2023-05-25 16:17:50.000000 servalcat-0.4.24/README.md
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.349871 servalcat-0.4.24/eigen/
+-rw-r--r--   0 yam        (501) staff       (20)    11362 2023-03-27 17:50:41.000000 servalcat-0.4.24/eigen/COPYING.APACHE
+-rw-r--r--   0 yam        (501) staff       (20)     1517 2023-03-27 17:50:41.000000 servalcat-0.4.24/eigen/COPYING.BSD
+-rw-r--r--   0 yam        (501) staff       (20)    35147 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/COPYING.GPL
+-rw-r--r--   0 yam        (501) staff       (20)    26530 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/COPYING.LGPL
+-rw-r--r--   0 yam        (501) staff       (20)     2193 2023-03-27 17:50:41.000000 servalcat-0.4.24/eigen/COPYING.MINPACK
+-rw-r--r--   0 yam        (501) staff       (20)    16726 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/COPYING.MPL2
+-rw-r--r--   0 yam        (501) staff       (20)      779 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/COPYING.README
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.360707 servalcat-0.4.24/eigen/Eigen/
+-rw-r--r--   0 yam        (501) staff       (20)     1161 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/Cholesky
+-rw-r--r--   0 yam        (501) staff       (20)     1900 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/CholmodSupport
+-rw-r--r--   0 yam        (501) staff       (20)    12799 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/Core
+-rw-r--r--   0 yam        (501) staff       (20)      122 2023-03-27 17:50:41.000000 servalcat-0.4.24/eigen/Eigen/Dense
+-rw-r--r--   0 yam        (501) staff       (20)       35 2023-03-27 17:50:41.000000 servalcat-0.4.24/eigen/Eigen/Eigen
+-rw-r--r--   0 yam        (501) staff       (20)     1777 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/Eigenvalues
+-rw-r--r--   0 yam        (501) staff       (20)     1940 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/Geometry
+-rw-r--r--   0 yam        (501) staff       (20)      829 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/Householder
+-rw-r--r--   0 yam        (501) staff       (20)     2083 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 yam        (501) staff       (20)      894 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/Jacobi
+-rw-r--r--   0 yam        (501) staff       (20)     1389 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/KLUSupport
+-rw-r--r--   0 yam        (501) staff       (20)     1268 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/LU
+-rw-r--r--   0 yam        (501) staff       (20)      991 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/MetisSupport
+-rw-r--r--   0 yam        (501) staff       (20)     2451 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/OrderingMethods
+-rw-r--r--   0 yam        (501) staff       (20)     1751 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/PaStiXSupport
+-rw-r--r--   0 yam        (501) staff       (20)     1116 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/PardisoSupport
+-rw-r--r--   0 yam        (501) staff       (20)     1272 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/QR
+-rw-r--r--   0 yam        (501) staff       (20)      900 2023-03-27 17:50:41.000000 servalcat-0.4.24/eigen/Eigen/QtAlignedMalloc
+-rw-r--r--   0 yam        (501) staff       (20)     1162 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/SPQRSupport
+-rw-r--r--   0 yam        (501) staff       (20)     1584 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/SVD
+-rw-r--r--   0 yam        (501) staff       (20)      888 2023-03-27 17:50:41.000000 servalcat-0.4.24/eigen/Eigen/Sparse
+-rw-r--r--   0 yam        (501) staff       (20)     1235 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/SparseCholesky
+-rw-r--r--   0 yam        (501) staff       (20)     2240 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/SparseCore
+-rw-r--r--   0 yam        (501) staff       (20)     1814 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/SparseLU
+-rw-r--r--   0 yam        (501) staff       (20)     1195 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/SparseQR
+-rw-r--r--   0 yam        (501) staff       (20)      797 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/StdDeque
+-rw-r--r--   0 yam        (501) staff       (20)      726 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/StdList
+-rw-r--r--   0 yam        (501) staff       (20)      803 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/StdVector
+-rw-r--r--   0 yam        (501) staff       (20)     2243 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/SuperLUSupport
+-rw-r--r--   0 yam        (501) staff       (20)     1382 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/UmfPackSupport
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.341169 servalcat-0.4.24/eigen/Eigen/src/
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.362182 servalcat-0.4.24/eigen/Eigen/src/Cholesky/
+-rw-r--r--   0 yam        (501) staff       (20)    24934 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 yam        (501) staff       (20)    18760 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 yam        (501) staff       (20)     3974 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.362677 servalcat-0.4.24/eigen/Eigen/src/CholmodSupport/
+-rw-r--r--   0 yam        (501) staff       (20)    25441 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.398756 servalcat-0.4.24/eigen/Eigen/src/Core/
+-rw-r--r--   0 yam        (501) staff       (20)    19214 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/ArithmeticSequence.h
+-rw-r--r--   0 yam        (501) staff       (20)    16782 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Array.h
+-rw-r--r--   0 yam        (501) staff       (20)     8217 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 yam        (501) staff       (20)     7018 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 yam        (501) staff       (20)     2738 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Assign.h
+-rw-r--r--   0 yam        (501) staff       (20)    41673 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/AssignEvaluator.h
+-rwxr-xr-x   0 yam        (501) staff       (20)    12488 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 yam        (501) staff       (20)    14075 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 yam        (501) staff       (20)    18648 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Block.h
+-rw-r--r--   0 yam        (501) staff       (20)     4429 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 yam        (501) staff       (20)     5981 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 yam        (501) staff       (20)     6990 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 yam        (501) staff       (20)    63841 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 yam        (501) staff       (20)     4745 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 yam        (501) staff       (20)     7909 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 yam        (501) staff       (20)    36282 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 yam        (501) staff       (20)     8256 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 yam        (501) staff       (20)     3937 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 yam        (501) staff       (20)     5551 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 yam        (501) staff       (20)    31529 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 yam        (501) staff       (20)    24484 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 yam        (501) staff       (20)    25360 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 yam        (501) staff       (20)     9870 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 yam        (501) staff       (20)    14670 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 yam        (501) staff       (20)      988 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 yam        (501) staff       (20)    11654 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Dot.h
+-rw-r--r--   0 yam        (501) staff       (20)     5841 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 yam        (501) staff       (20)     4909 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 yam        (501) staff       (20)     5759 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 yam        (501) staff       (20)    21679 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 yam        (501) staff       (20)    38812 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 yam        (501) staff       (20)    11543 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 yam        (501) staff       (20)     8238 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/IO.h
+-rw-r--r--   0 yam        (501) staff       (20)     9620 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/IndexedView.h
+-rw-r--r--   0 yam        (501) staff       (20)     3503 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 yam        (501) staff       (20)     7256 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Map.h
+-rw-r--r--   0 yam        (501) staff       (20)    11281 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 yam        (501) staff       (20)    60784 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 yam        (501) staff       (20)     7156 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 yam        (501) staff       (20)    24343 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 yam        (501) staff       (20)    23856 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 yam        (501) staff       (20)     2520 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 yam        (501) staff       (20)     3620 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 yam        (501) staff       (20)    12884 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 yam        (501) staff       (20)     9207 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-r--r--   0 yam        (501) staff       (20)    20748 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 yam        (501) staff       (20)    49193 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 yam        (501) staff       (20)     7336 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Product.h
+-rw-r--r--   0 yam        (501) staff       (20)    53832 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 yam        (501) staff       (20)     7756 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Random.h
+-rw-r--r--   0 yam        (501) staff       (20)    19195 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Redux.h
+-rw-r--r--   0 yam        (501) staff       (20)    17821 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Ref.h
+-rw-r--r--   0 yam        (501) staff       (20)     5656 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 yam        (501) staff       (20)    17033 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Reshaped.h
+-rw-r--r--   0 yam        (501) staff       (20)     4284 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 yam        (501) staff       (20)     7522 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 yam        (501) staff       (20)     6143 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Select.h
+-rw-r--r--   0 yam        (501) staff       (20)    14999 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 yam        (501) staff       (20)     1697 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 yam        (501) staff       (20)     6837 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Solve.h
+-rw-r--r--   0 yam        (501) staff       (20)     9368 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 yam        (501) staff       (20)     6170 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 yam        (501) staff       (20)     8700 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 yam        (501) staff       (20)    21641 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/StlIterators.h
+-rw-r--r--   0 yam        (501) staff       (20)     4212 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Stride.h
+-rw-r--r--   0 yam        (501) staff       (20)     2765 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Swap.h
+-rw-r--r--   0 yam        (501) staff       (20)    17606 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 yam        (501) staff       (20)    13567 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 yam        (501) staff       (20)    38277 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 yam        (501) staff       (20)     3488 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 yam        (501) staff       (20)    35168 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 yam        (501) staff       (20)    11997 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.313252 servalcat-0.4.24/eigen/Eigen/src/Core/arch/
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.402271 servalcat-0.4.24/eigen/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 yam        (501) staff       (20)    15223 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 yam        (501) staff       (20)     8102 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 yam        (501) staff       (20)    64608 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 yam        (501) staff       (20)     2564 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.404461 servalcat-0.4.24/eigen/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 yam        (501) staff       (20)    17160 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-r--r--   0 yam        (501) staff       (20)    13344 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 yam        (501) staff       (20)    87891 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-r--r--   0 yam        (501) staff       (20)     2134 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.408370 servalcat-0.4.24/eigen/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 yam        (501) staff       (20)    16540 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 yam        (501) staff       (20)     2323 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-r--r--   0 yam        (501) staff       (20)   119355 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-r--r--   0 yam        (501) staff       (20)     9490 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-r--r--   0 yam        (501) staff       (20)    24820 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rwxr-xr-x   0 yam        (501) staff       (20)   102394 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.409035 servalcat-0.4.24/eigen/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 yam        (501) staff       (20)    17317 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/CUDA/Complex.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.412556 servalcat-0.4.24/eigen/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 yam        (501) staff       (20)    26903 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-r--r--   0 yam        (501) staff       (20)     5251 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 yam        (501) staff       (20)    67696 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-r--r--   0 yam        (501) staff       (20)     3770 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-r--r--   0 yam        (501) staff       (20)    35534 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/Default/Half.h
+-rw-r--r--   0 yam        (501) staff       (20)     1746 2023-03-27 17:50:41.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/Default/Settings.h
+-rw-r--r--   0 yam        (501) staff       (20)     3746 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.414417 servalcat-0.4.24/eigen/Eigen/src/Core/arch/GPU/
+-rw-r--r--   0 yam        (501) staff       (20)     2695 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-r--r--   0 yam        (501) staff       (20)    57047 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-r--r--   0 yam        (501) staff       (20)     2256 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.312389 servalcat-0.4.24/eigen/Eigen/src/Core/arch/HIP/
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.414938 servalcat-0.4.24/eigen/Eigen/src/Core/arch/HIP/hcc/
+-rw-r--r--   0 yam        (501) staff       (20)      691 2023-03-27 17:50:41.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.416298 servalcat-0.4.24/eigen/Eigen/src/Core/arch/MSA/
+-rw-r--r--   0 yam        (501) staff       (20)    17541 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/MSA/Complex.h
+-rw-r--r--   0 yam        (501) staff       (20)    16159 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-r--r--   0 yam        (501) staff       (20)    33615 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.418846 servalcat-0.4.24/eigen/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 yam        (501) staff       (20)    22503 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 yam        (501) staff       (20)     6815 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-r--r--   0 yam        (501) staff       (20)     3083 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 yam        (501) staff       (20)   189525 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-r--r--   0 yam        (501) staff       (20)    51286 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.424354 servalcat-0.4.24/eigen/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 yam        (501) staff       (20)    14251 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 yam        (501) staff       (20)     6765 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxr-xr-x   0 yam        (501) staff       (20)    64465 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 yam        (501) staff       (20)     3650 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.425791 servalcat-0.4.24/eigen/Eigen/src/Core/arch/SVE/
+-rw-r--r--   0 yam        (501) staff       (20)     1194 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-r--r--   0 yam        (501) staff       (20)    21200 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-r--r--   0 yam        (501) staff       (20)     1351 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.427951 servalcat-0.4.24/eigen/Eigen/src/Core/arch/SYCL/
+-rw-r--r--   0 yam        (501) staff       (20)     7428 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-r--r--   0 yam        (501) staff       (20)    12539 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-r--r--   0 yam        (501) staff       (20)    27786 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-r--r--   0 yam        (501) staff       (20)    21856 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-r--r--   0 yam        (501) staff       (20)     2626 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.429294 servalcat-0.4.24/eigen/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 yam        (501) staff       (20)    16728 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 yam        (501) staff       (20)     8024 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxr-xr-x   0 yam        (501) staff       (20)    36894 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.431867 servalcat-0.4.24/eigen/Eigen/src/Core/functors/
+-rw-r--r--   0 yam        (501) staff       (20)     6686 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 yam        (501) staff       (20)    20921 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 yam        (501) staff       (20)     8334 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 yam        (501) staff       (20)     4998 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 yam        (501) staff       (20)      607 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 yam        (501) staff       (20)    40146 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.440995 servalcat-0.4.24/eigen/Eigen/src/Core/products/
+-rw-r--r--   0 yam        (501) staff       (20)   108448 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 yam        (501) staff       (20)    20104 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 yam        (501) staff       (20)    15948 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 yam        (501) staff       (20)     6936 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 yam        (501) staff       (20)     5106 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 yam        (501) staff       (20)    21724 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 yam        (501) staff       (20)     6368 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 yam        (501) staff       (20)     5582 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 yam        (501) staff       (20)    21354 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 yam        (501) staff       (20)    11570 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 yam        (501) staff       (20)     9958 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 yam        (501) staff       (20)     5209 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 yam        (501) staff       (20)     6164 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 yam        (501) staff       (20)     4126 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 yam        (501) staff       (20)    20987 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 yam        (501) staff       (20)    13867 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 yam        (501) staff       (20)    14722 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 yam        (501) staff       (20)    10571 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 yam        (501) staff       (20)    14678 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 yam        (501) staff       (20)     6707 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 yam        (501) staff       (20)     5882 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.477120 servalcat-0.4.24/eigen/Eigen/src/Core/util/
+-rwxr-xr-x   0 yam        (501) staff       (20)    23156 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 yam        (501) staff       (20)    19876 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-r--r--   0 yam        (501) staff       (20)    21931 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/util/Constants.h
+-rwxr-xr-x   0 yam        (501) staff       (20)     4892 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 yam        (501) staff       (20)    15555 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-r--r--   0 yam        (501) staff       (20)     6696 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-r--r--   0 yam        (501) staff       (20)    10949 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/util/IntegralConstant.h
+-rwxr-xr-x   0 yam        (501) staff       (20)     4268 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 yam        (501) staff       (20)    52909 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 yam        (501) staff       (20)    46661 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/util/Memory.h
+-rwxr-xr-x   0 yam        (501) staff       (20)    29336 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 yam        (501) staff       (20)       85 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 yam        (501) staff       (20)     1024 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 yam        (501) staff       (20)     1432 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/util/ReshapedHelper.h
+-rw-r--r--   0 yam        (501) staff       (20)    10676 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 yam        (501) staff       (20)    12003 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/util/SymbolicIndex.h
+-rw-r--r--   0 yam        (501) staff       (20)    35762 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.483848 servalcat-0.4.24/eigen/Eigen/src/Eigenvalues/
+-rw-r--r--   0 yam        (501) staff       (20)    12559 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 yam        (501) staff       (20)    17274 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 yam        (501) staff       (20)     4178 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 yam        (501) staff       (20)    22970 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 yam        (501) staff       (20)    17176 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 yam        (501) staff       (20)     9716 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 yam        (501) staff       (20)    14349 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 yam        (501) staff       (20)     5575 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 yam        (501) staff       (20)    23640 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 yam        (501) staff       (20)    21078 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 yam        (501) staff       (20)     3650 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 yam        (501) staff       (20)    35182 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 yam        (501) staff       (20)     4104 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 yam        (501) staff       (20)    22764 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.490716 servalcat-0.4.24/eigen/Eigen/src/Geometry/
+-rw-r--r--   0 yam        (501) staff       (20)    18939 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 yam        (501) staff       (20)     8403 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 yam        (501) staff       (20)     3624 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 yam        (501) staff       (20)    20726 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 yam        (501) staff       (20)    11962 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 yam        (501) staff       (20)     8955 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 yam        (501) staff       (20)     9812 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 yam        (501) staff       (20)    34367 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 yam        (501) staff       (20)     6862 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 yam        (501) staff       (20)     8063 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0 yam        (501) staff       (20)     6724 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 yam        (501) staff       (20)    61930 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 yam        (501) staff       (20)     7664 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 yam        (501) staff       (20)     6190 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.491120 servalcat-0.4.24/eigen/Eigen/src/Geometry/arch/
+-rw-r--r--   0 yam        (501) staff       (20)     5945 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Geometry/arch/Geometry_SIMD.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.492331 servalcat-0.4.24/eigen/Eigen/src/Householder/
+-rw-r--r--   0 yam        (501) staff       (20)     4784 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 yam        (501) staff       (20)     5365 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 yam        (501) staff       (20)    23611 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Householder/HouseholderSequence.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.496261 servalcat-0.4.24/eigen/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 yam        (501) staff       (20)     6771 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 yam        (501) staff       (20)     6850 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 yam        (501) staff       (20)     8887 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 yam        (501) staff       (20)    15036 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 yam        (501) staff       (20)    14940 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 yam        (501) staff       (20)    13379 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 yam        (501) staff       (20)     7349 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 yam        (501) staff       (20)     4212 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.496642 servalcat-0.4.24/eigen/Eigen/src/Jacobi/
+-rw-r--r--   0 yam        (501) staff       (20)    16383 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.497048 servalcat-0.4.24/eigen/Eigen/src/KLUSupport/
+-rw-r--r--   0 yam        (501) staff       (20)    11555 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/KLUSupport/KLUSupport.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.499030 servalcat-0.4.24/eigen/Eigen/src/LU/
+-rw-r--r--   0 yam        (501) staff       (20)     3439 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 yam        (501) staff       (20)    32383 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 yam        (501) staff       (20)    15727 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 yam        (501) staff       (20)    22069 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 yam        (501) staff       (20)     3555 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.499442 servalcat-0.4.24/eigen/Eigen/src/LU/arch/
+-rw-r--r--   0 yam        (501) staff       (20)    13693 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/LU/arch/InverseSize4.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.499832 servalcat-0.4.24/eigen/Eigen/src/MetisSupport/
+-rw-r--r--   0 yam        (501) staff       (20)     4588 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.501159 servalcat-0.4.24/eigen/Eigen/src/OrderingMethods/
+-rw-r--r--   0 yam        (501) staff       (20)    16105 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 yam        (501) staff       (20)    61681 2023-03-27 17:50:41.000000 servalcat-0.4.24/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 yam        (501) staff       (20)     5248 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.501531 servalcat-0.4.24/eigen/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 yam        (501) staff       (20)    22249 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.501973 servalcat-0.4.24/eigen/Eigen/src/PardisoSupport/
+-rw-r--r--   0 yam        (501) staff       (20)    20092 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.504793 servalcat-0.4.24/eigen/Eigen/src/QR/
+-rw-r--r--   0 yam        (501) staff       (20)    25498 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 yam        (501) staff       (20)     4662 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 yam        (501) staff       (20)    23429 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 yam        (501) staff       (20)    26768 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 yam        (501) staff       (20)    14641 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 yam        (501) staff       (20)     2993 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.505208 servalcat-0.4.24/eigen/Eigen/src/SPQRSupport/
+-rw-r--r--   0 yam        (501) staff       (20)    11826 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.507949 servalcat-0.4.24/eigen/Eigen/src/SVD/
+-rw-r--r--   0 yam        (501) staff       (20)    54214 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 yam        (501) staff       (20)    32988 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 yam        (501) staff       (20)     5099 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 yam        (501) staff       (20)    14743 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 yam        (501) staff       (20)    15957 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.508871 servalcat-0.4.24/eigen/Eigen/src/SparseCholesky/
+-rw-r--r--   0 yam        (501) staff       (20)    24216 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 yam        (501) staff       (20)     5830 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.522061 servalcat-0.4.24/eigen/Eigen/src/SparseCore/
+-rw-r--r--   0 yam        (501) staff       (20)    10670 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 yam        (501) staff       (20)     8743 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 yam        (501) staff       (20)    13166 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 yam        (501) staff       (20)     2191 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 yam        (501) staff       (20)    11368 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 yam        (501) staff       (20)    24360 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 yam        (501) staff       (20)     6485 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 yam        (501) staff       (20)    13606 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 yam        (501) staff       (20)    25524 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 yam        (501) staff       (20)     4757 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 yam        (501) staff       (20)    13256 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 yam        (501) staff       (20)     5808 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 yam        (501) staff       (20)     3080 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 yam        (501) staff       (20)     1107 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 yam        (501) staff       (20)    12589 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 yam        (501) staff       (20)    57475 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 yam        (501) staff       (20)    17451 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 yam        (501) staff       (20)     7329 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 yam        (501) staff       (20)     7593 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 yam        (501) staff       (20)     1699 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 yam        (501) staff       (20)    15600 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 yam        (501) staff       (20)    25889 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 yam        (501) staff       (20)     4424 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 yam        (501) staff       (20)     8704 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 yam        (501) staff       (20)     3175 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 yam        (501) staff       (20)     6437 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 yam        (501) staff       (20)     6827 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 yam        (501) staff       (20)    14832 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 yam        (501) staff       (20)     8127 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 yam        (501) staff       (20)     9657 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.528884 servalcat-0.4.24/eigen/Eigen/src/SparseLU/
+-rw-r--r--   0 yam        (501) staff       (20)    33316 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 yam        (501) staff       (20)     4303 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 yam        (501) staff       (20)     7602 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 yam        (501) staff       (20)     4974 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 yam        (501) staff       (20)    12837 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 yam        (501) staff       (20)     2049 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 yam        (501) staff       (20)     6712 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 yam        (501) staff       (20)     6584 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 yam        (501) staff       (20)     3681 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 yam        (501) staff       (20)    10217 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 yam        (501) staff       (20)     4181 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 yam        (501) staff       (20)     5723 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 yam        (501) staff       (20)     8485 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 yam        (501) staff       (20)     9028 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 yam        (501) staff       (20)     4979 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 yam        (501) staff       (20)     4545 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 yam        (501) staff       (20)     2889 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.529417 servalcat-0.4.24/eigen/Eigen/src/SparseQR/
+-rw-r--r--   0 yam        (501) staff       (20)    29167 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.531298 servalcat-0.4.24/eigen/Eigen/src/StlSupport/
+-rw-r--r--   0 yam        (501) staff       (20)     4730 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 yam        (501) staff       (20)     4155 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 yam        (501) staff       (20)     5338 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 yam        (501) staff       (20)     2809 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.531711 servalcat-0.4.24/eigen/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 yam        (501) staff       (20)    34324 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.532220 servalcat-0.4.24/eigen/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 yam        (501) staff       (20)    24456 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.562596 servalcat-0.4.24/eigen/Eigen/src/misc/
+-rw-r--r--   0 yam        (501) staff       (20)     2913 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/misc/Image.h
+-rw-r--r--   0 yam        (501) staff       (20)     2742 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 yam        (501) staff       (20)     1748 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 yam        (501) staff       (20)    30560 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/misc/blas.h
+-rw-r--r--   0 yam        (501) staff       (20)     7834 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/misc/lapack.h
+-rwxr-xr-x   0 yam        (501) staff       (20)  1058369 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 yam        (501) staff       (20)      474 2023-03-27 17:50:42.000000 servalcat-0.4.24/eigen/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.567706 servalcat-0.4.24/eigen/Eigen/src/plugins/
+-rw-r--r--   0 yam        (501) staff       (20)    14060 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 yam        (501) staff       (20)    21431 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 yam        (501) staff       (20)    59020 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 yam        (501) staff       (20)     4828 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 yam        (501) staff       (20)     6089 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 yam        (501) staff       (20)    12283 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/plugins/IndexedViewMethods.h
+-rw-r--r--   0 yam        (501) staff       (20)     6387 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 yam        (501) staff       (20)     3350 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0 yam        (501) staff       (20)     6915 2023-04-17 16:49:40.000000 servalcat-0.4.24/eigen/Eigen/src/plugins/ReshapedMethods.h
+-rw-r--r--   0 yam        (501) staff       (20)      288 2023-03-27 17:50:42.000000 servalcat-0.4.24/eigen/README.md
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.568565 servalcat-0.4.24/gemmi/
+-rw-r--r--   0 yam        (501) staff       (20)    16726 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/LICENSE.txt
+-rw-r--r--   0 yam        (501) staff       (20)     1390 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/README.md
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.341560 servalcat-0.4.24/gemmi/include/
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.639421 servalcat-0.4.24/gemmi/include/gemmi/
+-rw-r--r--   0 yam        (501) staff       (20)      844 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/addends.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    11033 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/align.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     4590 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/assembly.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     7484 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/asudata.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    11451 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/asumask.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1023 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/atof.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     3810 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/atox.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     3983 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/bessel.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     6974 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/binner.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     4864 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/blob.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     3045 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/bond_idx.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    10368 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/c4322.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     5574 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/calculate.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    17280 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/ccp4.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    13372 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/cellred.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    23755 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/chemcomp.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     4657 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/chemcomp_xyz.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    14110 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/cif.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    21584 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/cif2mtz.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    35703 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/cifdoc.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     5036 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/contact.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      543 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/crd.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     7049 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/dencalc.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     7422 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/dirwalk.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      314 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/eig3.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    14634 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/elem.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     4526 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/enumstr.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2102 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/fail.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     3810 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/fileutil.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     5139 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/floodfill.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     4468 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/formfact.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    13191 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/fourier.hpp
+-rw-r--r--   0 yam        (501) staff       (20)   271931 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/fprime.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2222 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/fstream.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    26551 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/grid.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     5182 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/gz.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     4512 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/input.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1846 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/interop.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    10429 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/it92.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     9757 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/iterator.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     4820 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/json.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     9023 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/levmar.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     6788 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/linkhunt.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    14300 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/math.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    16861 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/merge.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    13775 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/metadata.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      991 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/mmcif.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1243 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/mmcif_impl.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     9234 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/mmdb.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     3894 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/mmread.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      818 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/mmread_gz.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    36259 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/model.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     6058 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/modify.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    11568 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/monlib.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    38452 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/mtz.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     4439 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/mtz2cif.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    13422 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/neighbor.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2787 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/neutron92.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1479 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/numb.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    27207 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/pdb.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2083 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/pdb_id.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1287 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/pirfasta.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     8877 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/polyheur.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    12909 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/qcp.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      954 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/read_cif.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1117 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/read_map.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     5846 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/recgrid.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1992 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/reciproc.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     8868 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/refln.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    25493 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/remarks.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2849 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/resinfo.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1016 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/riding_h.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    11608 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/scaling.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    16331 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/select.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    10437 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/seqalign.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     5125 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/seqid.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     5432 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/sfcalc.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     4034 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/small.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     6843 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/smcif.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    17639 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/solmask.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     4668 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/span.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2244 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/sprintf.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2761 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/stats.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    93297 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/symmetry.hpp
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.641766 servalcat-0.4.24/gemmi/include/gemmi/third_party/
+-rw-r--r--   0 yam        (501) staff       (20)   114265 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/fast_float.h
+-rw-r--r--   0 yam        (501) staff       (20)   107015 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/pocketfft_hdronly.h
+-rw-r--r--   0 yam        (501) staff       (20)    95912 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/sajson.h
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.643128 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/
+-rw-r--r--   0 yam        (501) staff       (20)     1104 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/LICENSE
+-rw-r--r--   0 yam        (501) staff       (20)      359 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/NOTES
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.654458 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.657761 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/analysis/
+-rw-r--r--   0 yam        (501) staff       (20)     4544 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/analysis/analyze_cycles.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      646 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/analysis/counted.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      954 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/analysis/generic.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      943 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/analysis/grammar_info.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1705 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/analysis/insert_guard.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1099 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/analysis/insert_rules.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      749 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/analysis/rule_info.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      990 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/analysis/rule_type.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      559 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/analyze.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      451 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/apply_mode.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1339 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/argv_input.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     3463 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/ascii.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     5021 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/buffer_input.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      534 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/config.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      872 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/cstream_input.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1042 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/eol.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      440 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/eol_pair.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      961 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/file_input.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1513 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/input_error.hpp
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.695385 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/
+-rw-r--r--   0 yam        (501) staff       (20)     1439 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/action.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2869 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/action_input.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      548 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/alnum.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      538 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/alpha.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1664 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/any.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2750 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/apply.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2521 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/apply0.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1154 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/apply0_single.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1229 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/apply_single.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1626 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/at.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      862 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/bof.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      870 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/bol.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1573 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/bump_help.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1373 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/bump_impl.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1076 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/bytes.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1445 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/control.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1049 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/cr_crlf_eol.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      975 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/cr_eol.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1025 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/crlf_eol.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1389 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/cstream_reader.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1178 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/cstring_reader.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      843 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/demangle.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1045 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/demangle_cxxabi.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      567 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/demangle_nop.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1376 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/demangle_sanitise.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1382 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/disable.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1003 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/discard.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      616 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/dusel_mode.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     7228 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/duseltronik.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1377 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/enable.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1557 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/endian.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     5410 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/endian_gcc.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2938 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/endian_win.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      884 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/eof.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      920 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/eol.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      974 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/eolf.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2518 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/file_mapper.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2011 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/file_opener.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     3297 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/file_reader.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      751 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/has_apply.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      756 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/has_apply0.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      772 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/identifier.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     3802 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/if_apply.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      580 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/if_must.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      634 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/if_must_else.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1862 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/if_then_else.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      723 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/input_pair.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     3323 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/integer_sequence.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1159 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/istream_reader.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2766 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/istring.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1493 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/iterator.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1229 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/lf_crlf_eol.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      975 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/lf_eol.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      567 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/list.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      610 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/list_must.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      607 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/list_tail.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      697 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/list_tail_pad.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2409 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/marker.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2092 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/minus.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2484 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/must.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1652 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/not_at.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2429 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/one.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1648 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/opt.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      596 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/pad.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      609 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/pad_opt.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      837 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/peek_char.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2245 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/peek_utf16.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1800 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/peek_utf32.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2931 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/peek_utf8.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     4180 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/pegtl_string.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1786 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/plus.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1598 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/raise.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1684 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/range.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2994 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/ranges.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2020 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/rep.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      641 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/rep_min.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2880 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/rep_min_max.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1500 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/rep_opt.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1172 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/require.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      568 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/result_on_found.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1910 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/rule_conjunction.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1393 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/rules.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2240 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/seq.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      903 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/skip_control.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2150 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/sor.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1494 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/star.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      594 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/star_must.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2769 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/state.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1736 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/string.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      955 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/trivial.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1972 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/try_catch_type.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2874 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/internal/until.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      876 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/istream_input.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     9778 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/memory_input.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1913 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/mmap_input.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     3897 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/normal.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      586 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/nothing.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1616 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/parse.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1106 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/parse_error.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1351 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/position.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2198 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/read_input.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      459 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/rewind_mode.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     4942 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/rules.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1936 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/string_input.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      445 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/tracking_mode.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2832 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/utf16.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2832 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/utf32.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     1553 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/utf8.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      602 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl/version.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      793 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tao/pegtl.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    19235 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/third_party/tinydir.h
+-rw-r--r--   0 yam        (501) staff       (20)     2797 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/to_chemcomp.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     6242 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/to_cif.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     8862 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/to_json.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2421 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/to_mmcif.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      862 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/to_pdb.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    10769 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/topo.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    10282 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/twin.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    21692 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/unitcell.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2476 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/utf.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     8661 2023-03-16 13:45:49.000000 servalcat-0.4.24/gemmi/include/gemmi/util.hpp
+-rw-r--r--   0 yam        (501) staff       (20)      152 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/include/gemmi/version.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    14985 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/include/gemmi/xds_ascii.hpp
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.697972 servalcat-0.4.24/gemmi/src/
+-rw-r--r--   0 yam        (501) staff       (20)     5709 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/src/eig3.cpp
+-rw-r--r--   0 yam        (501) staff       (20)    20572 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/src/monlib.cpp
+-rw-r--r--   0 yam        (501) staff       (20)    12734 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/src/polyheur.cpp
+-rw-r--r--   0 yam        (501) staff       (20)    24654 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/src/resinfo.cpp
+-rw-r--r--   0 yam        (501) staff       (20)    17837 2023-05-04 08:45:27.000000 servalcat-0.4.24/gemmi/src/riding_h.cpp
+-rw-r--r--   0 yam        (501) staff       (20)    39755 2023-05-26 06:25:48.000000 servalcat-0.4.24/gemmi/src/topo.cpp
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.343282 servalcat-0.4.24/gemmi/third_party/
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.705926 servalcat-0.4.24/gemmi/third_party/zlib/
+-rw-r--r--   0 yam        (501) staff       (20)     5204 2023-03-16 13:45:50.000000 servalcat-0.4.24/gemmi/third_party/zlib/adler32.c
+-rw-r--r--   0 yam        (501) staff       (20)    14053 2023-03-16 13:45:50.000000 servalcat-0.4.24/gemmi/third_party/zlib/crc32.c
+-rw-r--r--   0 yam        (501) staff       (20)    30562 2023-03-16 13:45:50.000000 servalcat-0.4.24/gemmi/third_party/zlib/crc32.h
+-rw-r--r--   0 yam        (501) staff       (20)     6819 2023-03-16 13:45:50.000000 servalcat-0.4.24/gemmi/third_party/zlib/gzguts.h
+-rw-r--r--   0 yam        (501) staff       (20)    16599 2023-03-16 13:45:50.000000 servalcat-0.4.24/gemmi/third_party/zlib/gzlib.c
+-rw-r--r--   0 yam        (501) staff       (20)    20428 2023-03-16 13:45:50.000000 servalcat-0.4.24/gemmi/third_party/zlib/gzread.c
+-rw-r--r--   0 yam        (501) staff       (20)    12978 2023-03-16 13:45:50.000000 servalcat-0.4.24/gemmi/third_party/zlib/inffast.c
+-rw-r--r--   0 yam        (501) staff       (20)      427 2023-03-16 13:45:50.000000 servalcat-0.4.24/gemmi/third_party/zlib/inffast.h
+-rw-r--r--   0 yam        (501) staff       (20)     6332 2023-03-16 13:45:50.000000 servalcat-0.4.24/gemmi/third_party/zlib/inffixed.h
+-rw-r--r--   0 yam        (501) staff       (20)    54800 2023-03-16 13:45:50.000000 servalcat-0.4.24/gemmi/third_party/zlib/inflate.c
+-rw-r--r--   0 yam        (501) staff       (20)     6618 2023-03-16 13:45:50.000000 servalcat-0.4.24/gemmi/third_party/zlib/inflate.h
+-rw-r--r--   0 yam        (501) staff       (20)    12999 2023-03-16 13:45:50.000000 servalcat-0.4.24/gemmi/third_party/zlib/inftrees.c
+-rw-r--r--   0 yam        (501) staff       (20)     2928 2023-03-16 13:45:50.000000 servalcat-0.4.24/gemmi/third_party/zlib/inftrees.h
+-rw-r--r--   0 yam        (501) staff       (20)     1031 2023-03-16 13:45:50.000000 servalcat-0.4.24/gemmi/third_party/zlib/license
+-rw-r--r--   0 yam        (501) staff       (20)    16298 2023-03-16 13:45:50.000000 servalcat-0.4.24/gemmi/third_party/zlib/zconf.h
+-rw-r--r--   0 yam        (501) staff       (20)    96239 2023-03-16 13:45:50.000000 servalcat-0.4.24/gemmi/third_party/zlib/zlib.h
+-rw-r--r--   0 yam        (501) staff       (20)     7304 2023-03-16 13:45:50.000000 servalcat-0.4.24/gemmi/third_party/zlib/zutil.c
+-rw-r--r--   0 yam        (501) staff       (20)     7127 2023-03-16 13:45:50.000000 servalcat-0.4.24/gemmi/third_party/zlib/zutil.h
+-rw-r--r--   0 yam        (501) staff       (20)       51 2023-04-18 18:05:48.000000 servalcat-0.4.24/pyproject.toml
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.732227 servalcat-0.4.24/servalcat/
+-rw-r--r--   0 yam        (501) staff       (20)      231 2023-05-31 18:06:01.000000 servalcat-0.4.24/servalcat/__init__.py
+-rw-r--r--   0 yam        (501) staff       (20)     4317 2023-05-23 16:10:58.000000 servalcat-0.4.24/servalcat/command_line.py
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.739408 servalcat-0.4.24/servalcat/refine/
+-rw-r--r--   0 yam        (501) staff       (20)        0 2023-04-18 18:00:38.000000 servalcat-0.4.24/servalcat/refine/__init__.py
+-rw-r--r--   0 yam        (501) staff       (20)     3072 2023-04-18 18:00:38.000000 servalcat-0.4.24/servalcat/refine/cgsolve.py
+-rw-r--r--   0 yam        (501) staff       (20)    21610 2023-05-30 16:31:07.000000 servalcat-0.4.24/servalcat/refine/refine.py
+-rw-r--r--   0 yam        (501) staff       (20)     8236 2023-05-25 16:14:45.000000 servalcat-0.4.24/servalcat/refine/refine_geom.py
+-rw-r--r--   0 yam        (501) staff       (20)    15266 2023-05-26 08:20:07.000000 servalcat-0.4.24/servalcat/refine/refine_spa.py
+-rw-r--r--   0 yam        (501) staff       (20)     9355 2023-05-30 21:28:14.000000 servalcat-0.4.24/servalcat/refine/refine_xtal.py
+-rw-r--r--   0 yam        (501) staff       (20)     5994 2023-05-04 08:45:26.000000 servalcat-0.4.24/servalcat/refine/spa.py
+-rw-r--r--   0 yam        (501) staff       (20)    15739 2023-05-30 19:21:37.000000 servalcat-0.4.24/servalcat/refine/xtal.py
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.740902 servalcat-0.4.24/servalcat/refmac/
+-rw-r--r--   0 yam        (501) staff       (20)        0 2023-04-18 17:58:34.000000 servalcat-0.4.24/servalcat/refmac/__init__.py
+-rw-r--r--   0 yam        (501) staff       (20)     8836 2023-05-10 15:24:39.000000 servalcat-0.4.24/servalcat/refmac/exte.py
+-rw-r--r--   0 yam        (501) staff       (20)    21715 2023-05-10 11:00:55.000000 servalcat-0.4.24/servalcat/refmac/refmac_keywords.py
+-rw-r--r--   0 yam        (501) staff       (20)    12916 2023-05-25 16:14:45.000000 servalcat-0.4.24/servalcat/refmac/refmac_wrapper.py
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.749656 servalcat-0.4.24/servalcat/spa/
+-rw-r--r--   0 yam        (501) staff       (20)        0 2022-11-13 21:58:00.000000 servalcat-0.4.24/servalcat/spa/__init__.py
+-rw-r--r--   0 yam        (501) staff       (20)     3982 2022-11-13 21:58:00.000000 servalcat-0.4.24/servalcat/spa/est_local_luzzati_d.py
+-rw-r--r--   0 yam        (501) staff       (20)     1754 2022-11-13 21:58:00.000000 servalcat-0.4.24/servalcat/spa/estimate_mixture.py
+-rw-r--r--   0 yam        (501) staff       (20)     1860 2022-11-13 21:58:00.000000 servalcat-0.4.24/servalcat/spa/find_translation.py
+-rw-r--r--   0 yam        (501) staff       (20)    21767 2023-05-10 15:24:48.000000 servalcat-0.4.24/servalcat/spa/fofc.py
+-rw-r--r--   0 yam        (501) staff       (20)      996 2022-11-13 21:58:00.000000 servalcat-0.4.24/servalcat/spa/fofc_rms.py
+-rw-r--r--   0 yam        (501) staff       (20)    15014 2023-05-04 08:45:26.000000 servalcat-0.4.24/servalcat/spa/fsc.py
+-rw-r--r--   0 yam        (501) staff       (20)    10227 2022-11-23 16:39:29.000000 servalcat-0.4.24/servalcat/spa/fsc2.py
+-rw-r--r--   0 yam        (501) staff       (20)     7945 2023-04-18 18:05:48.000000 servalcat-0.4.24/servalcat/spa/localcc.py
+-rw-r--r--   0 yam        (501) staff       (20)     5275 2023-04-18 17:58:34.000000 servalcat-0.4.24/servalcat/spa/realspcc_from_var.py
+-rw-r--r--   0 yam        (501) staff       (20)      372 2022-11-13 21:58:00.000000 servalcat-0.4.24/servalcat/spa/refine_emdb.py
+-rw-r--r--   0 yam        (501) staff       (20)    47843 2023-05-25 16:14:45.000000 servalcat-0.4.24/servalcat/spa/run_refmac.py
+-rw-r--r--   0 yam        (501) staff       (20)    13152 2023-05-04 08:45:26.000000 servalcat-0.4.24/servalcat/spa/shift_maps.py
+-rw-r--r--   0 yam        (501) staff       (20)     4664 2023-04-18 17:58:34.000000 servalcat-0.4.24/servalcat/spa/shiftback.py
+-rw-r--r--   0 yam        (501) staff       (20)     5091 2023-04-18 17:58:34.000000 servalcat-0.4.24/servalcat/spa/translate.py
+-rw-r--r--   0 yam        (501) staff       (20)     6871 2022-11-13 21:58:00.000000 servalcat-0.4.24/servalcat/spa/tst_gemmi_mottbethe.py
+-rw-r--r--   0 yam        (501) staff       (20)     1076 2022-11-13 21:58:00.000000 servalcat-0.4.24/servalcat/spa/tst_refmac_fc.py
+-rw-r--r--   0 yam        (501) staff       (20)      519 2023-02-14 21:17:59.000000 servalcat-0.4.24/servalcat/test_installation.py
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.755873 servalcat-0.4.24/servalcat/utils/
+-rw-r--r--   0 yam        (501) staff       (20)     1146 2023-05-04 19:44:36.000000 servalcat-0.4.24/servalcat/utils/__init__.py
+-rw-r--r--   0 yam        (501) staff       (20)    52095 2023-05-25 16:14:45.000000 servalcat-0.4.24/servalcat/utils/commands.py
+-rw-r--r--   0 yam        (501) staff       (20)    29302 2023-05-31 06:59:49.000000 servalcat-0.4.24/servalcat/utils/fileio.py
+-rw-r--r--   0 yam        (501) staff       (20)    10867 2022-11-13 21:58:00.000000 servalcat-0.4.24/servalcat/utils/generate_operators.py
+-rw-r--r--   0 yam        (501) staff       (20)    25819 2023-05-23 15:24:34.000000 servalcat-0.4.24/servalcat/utils/hkl.py
+-rw-r--r--   0 yam        (501) staff       (20)     3524 2023-04-18 18:05:48.000000 servalcat-0.4.24/servalcat/utils/logger.py
+-rw-r--r--   0 yam        (501) staff       (20)    13101 2023-04-18 18:05:48.000000 servalcat-0.4.24/servalcat/utils/maps.py
+-rw-r--r--   0 yam        (501) staff       (20)    29329 2023-05-25 16:14:45.000000 servalcat-0.4.24/servalcat/utils/model.py
+-rw-r--r--   0 yam        (501) staff       (20)    29717 2023-04-18 18:05:48.000000 servalcat-0.4.24/servalcat/utils/refmac.py
+-rw-r--r--   0 yam        (501) staff       (20)      889 2022-11-13 21:58:00.000000 servalcat-0.4.24/servalcat/utils/refmac_params.py
+-rw-r--r--   0 yam        (501) staff       (20)    23781 2023-05-25 16:14:45.000000 servalcat-0.4.24/servalcat/utils/restraints.py
+-rw-r--r--   0 yam        (501) staff       (20)     4796 2022-11-13 21:58:00.000000 servalcat-0.4.24/servalcat/utils/scaling.py
+-rw-r--r--   0 yam        (501) staff       (20)    11879 2023-04-26 13:24:15.000000 servalcat-0.4.24/servalcat/utils/symmetry.py
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.757356 servalcat-0.4.24/servalcat/xtal/
+-rw-r--r--   0 yam        (501) staff       (20)        0 2022-11-13 21:58:00.000000 servalcat-0.4.24/servalcat/xtal/__init__.py
+-rw-r--r--   0 yam        (501) staff       (20)    10249 2023-05-26 14:47:10.000000 servalcat-0.4.24/servalcat/xtal/french_wilson.py
+-rw-r--r--   0 yam        (501) staff       (20)    11031 2023-05-04 08:45:26.000000 servalcat-0.4.24/servalcat/xtal/run_refmac_small.py
+-rw-r--r--   0 yam        (501) staff       (20)    52418 2023-05-31 13:28:29.000000 servalcat-0.4.24/servalcat/xtal/sigmaa.py
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.736114 servalcat-0.4.24/servalcat.egg-info/
+-rw-r--r--   0 yam        (501) staff       (20)      398 2023-05-31 20:36:14.000000 servalcat-0.4.24/servalcat.egg-info/PKG-INFO
+-rw-r--r--   0 yam        (501) staff       (20)    27921 2023-05-31 20:36:14.000000 servalcat-0.4.24/servalcat.egg-info/SOURCES.txt
+-rw-r--r--   0 yam        (501) staff       (20)        1 2023-05-31 20:36:14.000000 servalcat-0.4.24/servalcat.egg-info/dependency_links.txt
+-rw-r--r--   0 yam        (501) staff       (20)      115 2023-05-31 20:36:14.000000 servalcat-0.4.24/servalcat.egg-info/entry_points.txt
+-rw-r--r--   0 yam        (501) staff       (20)        1 2023-05-05 06:21:21.000000 servalcat-0.4.24/servalcat.egg-info/not-zip-safe
+-rw-r--r--   0 yam        (501) staff       (20)       46 2023-05-31 20:36:14.000000 servalcat-0.4.24/servalcat.egg-info/requires.txt
+-rw-r--r--   0 yam        (501) staff       (20)       10 2023-05-31 20:36:14.000000 servalcat-0.4.24/servalcat.egg-info/top_level.txt
+-rw-r--r--   0 yam        (501) staff       (20)       38 2023-05-31 20:36:14.762767 servalcat-0.4.24/setup.cfg
+-rw-r--r--   0 yam        (501) staff       (20)     5112 2023-05-25 16:16:58.000000 servalcat-0.4.24/setup.py
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.759218 servalcat-0.4.24/src/
+-rw-r--r--   0 yam        (501) staff       (20)     1616 2023-04-18 18:05:48.000000 servalcat-0.4.24/src/ext.cpp
+-rw-r--r--   0 yam        (501) staff       (20)    18448 2023-05-26 10:43:34.000000 servalcat-0.4.24/src/intensity.cpp
+-rw-r--r--   0 yam        (501) staff       (20)     2694 2023-04-18 18:05:48.000000 servalcat-0.4.24/src/lambertw.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     3228 2023-05-23 15:24:34.000000 servalcat-0.4.24/src/math.hpp
+drwxr-xr-x   0 yam        (501) staff       (20)        0 2023-05-31 20:36:14.761388 servalcat-0.4.24/src/refine/
+-rw-r--r--   0 yam        (501) staff       (20)     5677 2023-04-18 18:05:48.000000 servalcat-0.4.24/src/refine/cgsolve.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    64684 2023-05-25 16:14:45.000000 servalcat-0.4.24/src/refine/geom.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    26887 2023-05-04 08:45:26.000000 servalcat-0.4.24/src/refine/ll.hpp
+-rw-r--r--   0 yam        (501) staff       (20)     2226 2023-01-22 15:54:00.000000 servalcat-0.4.24/src/refine/params.hpp
+-rw-r--r--   0 yam        (501) staff       (20)    30505 2023-05-25 16:14:45.000000 servalcat-0.4.24/src/refine.cpp
```

### Comparing `servalcat-0.4.15/LICENSE` & `servalcat-0.4.24/LICENSE`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/gemmi/src/eig3.cpp` & `servalcat-0.4.24/gemmi/src/eig3.cpp`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/gemmi/src/monlib.cpp` & `servalcat-0.4.24/gemmi/src/monlib.cpp`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/gemmi/src/resinfo.cpp` & `servalcat-0.4.24/gemmi/src/resinfo.cpp`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/gemmi/src/riding_h.cpp` & `servalcat-0.4.24/gemmi/src/riding_h.cpp`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/gemmi/src/topo.cpp` & `servalcat-0.4.24/gemmi/src/topo.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,32 @@
   for (int n = 0; monlib.get_link(cl.id) != nullptr; ++n)
     cl.id.replace(orig_len, cl.id.size(), std::to_string(n));
 
   auto it = monlib.links.emplace(cl.id, cl);
   return it.first->first;
 }
 
+static const ChemLink* setup_link_if_matches(Topo::Link& link, const MonLib& monlib,
+                                             const std::string& atom1,
+                                             const std::string& atom2) {
+  bool invert;
+  const ChemLink* match = nullptr;
+  std::tie(match, invert, link.aliasing1, link.aliasing2) =
+    monlib.match_link(*link.res1, atom1, link.alt1, *link.res2, atom2, link.alt2);
+  if (match) {
+    link.link_id = match->id;
+    if (invert) {
+      std::swap(link.res1, link.res2);
+      std::swap(link.alt1, link.alt2);
+      std::swap(link.aliasing1, link.aliasing2);
+    }
+  }
+  return match;
+}
+
 static void add_polymer_links(PolymerType polymer_type,
                               const Topo::ResInfo& ri1,
                               Topo::ResInfo& ri2,
                               MonLib* monlib) {
   Topo::Link link;
   link.res1 = ri1.res;
   link.res2 = ri2.res;
@@ -220,18 +238,19 @@
               if (n_terminus_group == ChemComp::Group::PPeptide)
                 link.link_id = link.is_cis ? "PCIS" : "PTRANS";
               else if (n_terminus_group == ChemComp::Group::MPeptide)
                 link.link_id = link.is_cis ? "NMCIS" : "NMTRANS";
               else
                 link.link_id = link.is_cis ? "CIS" : "TRANS";
             } else if (monlib) {
-              link.link_id = add_auto_chemlink(*monlib,
-                                               ri1.res->name, c,
-                                               ri2.res->name, n,
-                                               1.34, 0.04);
+              if (!setup_link_if_matches(link, *monlib, c, n))
+                link.link_id = add_auto_chemlink(*monlib,
+                                                 ri1.res->name, c,
+                                                 ri2.res->name, n,
+                                                 1.34, 0.04);
             }
             ri2.prev.push_back(link);
           }
       }
 
   } else if (is_polynucleotide(polymer_type)) {
     std::string o3p = "O3'";
@@ -262,21 +281,23 @@
       if (a1.name == o3p && a1.element == El::O) {
         for (const Atom& a2 : ri2.res->atoms)
           if (a2.name == p && a2.element == El::P &&
               (a2.altloc == a1.altloc || a2.altloc == '\0' || a1.altloc == '\0') &&
               in_nucleotide_bond_distance(&a1, &a2)) {
             link.alt1 = a1.altloc;
             link.alt2 = a2.altloc;
-            if (groups_ok)
+            if (groups_ok) {
               link.link_id = "p";
-            else if (monlib)
-              link.link_id = add_auto_chemlink(*monlib,
-                                               ri1.res->name, o3p,
-                                               ri2.res->name, p,
-                                               1.606, 0.02);
+            } else if (monlib) {
+              if (!setup_link_if_matches(link, *monlib, o3p, p))
+                link.link_id = add_auto_chemlink(*monlib,
+                                                 ri1.res->name, o3p,
+                                                 ri2.res->name, p,
+                                                 1.606, 0.02);
+            }
             ri2.prev.push_back(link);
           }
     }
   }
 
   if (ri2.prev.empty()) {
     link.link_id = "gap";
@@ -615,27 +636,19 @@
                                conn.partner1.atom_name, extra.aliasing1) ||
         !atom_match_with_alias(match->rt.bonds[0].id2.atom,
                                conn.partner2.atom_name, extra.aliasing2)) {
       err("link from the monomer library does not match: " + conn.link_id);
       return;
     }
   } else {
-    bool invert;
     // we don't have link_id - use the best matching link (if any)
-    std::tie(match, invert, extra.aliasing1, extra.aliasing2) =
-      monlib.match_link(*extra.res1, conn.partner1.atom_name, extra.alt1,
-                        *extra.res2, conn.partner2.atom_name, extra.alt2);
-    if (match) {
+    match = setup_link_if_matches(extra, monlib,
+                                  conn.partner1.atom_name, conn.partner2.atom_name);
+    if (match)
       conn.link_id = match->id;
-      if (invert) {
-        std::swap(extra.res1, extra.res2);
-        std::swap(extra.alt1, extra.alt2);
-        std::swap(extra.aliasing1, extra.aliasing2);
-      }
-    }
   }
 
   // If a polymer link is also given in LINK/struct_conn,
   // use only one of them. If LINK has explicit name (ccp4_link_id),
   // or if it matches residue-specific link from monomer library, use it;
   // otherwise, LINK is repetition of TRANS/CIS, so ignore LINK.
   if (Link* polymer_link = find_polymer_link(conn.partner1, conn.partner2)) {
@@ -762,38 +775,40 @@
   float occ;
 };
 using NeighMap = std::unordered_multimap<int, Neigh>;
 
 // Assumes no hydrogens in the residue.
 // Position and serial number are not assigned for new atoms.
 void add_hydrogens_without_positions(Topo::ResInfo& ri, const NeighMap& neighbors) {
-  Residue& res = *ri.res;
+  std::vector<Atom>& atoms = ri.res->atoms;
   // Add H atom for each conformation (altloc) of the parent atom and its
   // first neighbors.
-  for (size_t i = 0, size = res.atoms.size(); i != size; ++i) {
-    char parent_alt = res.atoms[i].altloc;
-    float parent_occ = res.atoms[i].occ;
+  for (size_t i = 0, size = atoms.size(); i != size; ++i) {
+    if (atoms[i].calc_flag == CalcFlag::NoHydrogen)
+      continue;
+    char parent_alt = atoms[i].altloc;
+    float parent_occ = atoms[i].occ;
     std::map<char, float> altlocs; // altloc + occupancy
     if (parent_alt == '\0') {
       float max_occ = 1.001f;
-      auto range = neighbors.equal_range(res.atoms[i].serial);
+      auto range = neighbors.equal_range(atoms[i].serial);
       for (auto it = range.first; it != range.second; ++it) {
         const Neigh& neigh = it->second;
         if (neigh.alt && altlocs.count(neigh.alt) == 0 && neigh.occ < max_occ) {
           altlocs.emplace(neigh.alt, neigh.occ * parent_occ);
           max_occ -= neigh.occ;
         }
       }
     }
     if (altlocs.empty())
       altlocs.emplace(parent_alt, parent_occ);
     const ChemComp& cc = ri.get_final_chemcomp(parent_alt);
     for (const Restraints::Bond& bond : cc.rt.bonds) {
-      // res.atoms may get re-allocated, so we can't set parent earlier
-      const Atom& parent = res.atoms[i];
+      // atoms may get re-allocated, so we can't set parent earlier
+      const Atom& parent = atoms[i];
       assert(!parent.is_hydrogen());
       const Restraints::AtomId* atom_id = bond.other(parent.name);
       if (!atom_id)
         continue;
       auto it = cc.find_atom(atom_id->atom);
       if (it == cc.atoms.end())
         fail("inconsistent _chem_comp " + cc.name);
@@ -803,15 +818,15 @@
         atom.element = it->el;
         // calc_flag will be changed to Calculated when the position is set
         atom.calc_flag = CalcFlag::Dummy;
         atom.b_iso = parent.b_iso;
         for (auto alt_occ : altlocs) {
           atom.altloc = alt_occ.first;
           atom.occ = alt_occ.second;
-          res.atoms.push_back(atom);
+          atoms.push_back(atom);
         }
       }
     }
   }
 }
 
 NeighMap prepare_neighbor_data(Topo& topo, const MonLib& monlib) {
```

### Comparing `servalcat-0.4.15/servalcat/command_line.py` & `servalcat-0.4.24/servalcat/command_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         print(msg_skip)
         
     return ret
 # test_installation()        
 
 def main():
     parser = argparse.ArgumentParser(prog="servalcat",
-                                     description="A tool for model refinement and map calculation for cryo-EM SPA.")
+                                     description="A tool for model refinement and map calculation for crystallography and cryo-EM SPA.")
     parser.add_argument("--skip_test", action="store_true", help="Skip installation test")
     parser.add_argument("-v", "--version", action="version",
                         version="Servalcat {servalcat} with Python {python} ({deps})".format(servalcat=servalcat.__version__,
                                                                                              python=platform.python_version(),
                                                                                              deps=", ".join([x[0]+" "+x[1] for x in logger.dependency_versions().items()])))
     parser.add_argument("--logfile", default="servalcat.log")
     subparsers = parser.add_subparsers(dest="command")
```

### Comparing `servalcat-0.4.15/servalcat/refine/cgsolve.py` & `servalcat-0.4.24/servalcat/refine/cgsolve.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/refine/refine.py` & `servalcat-0.4.24/servalcat/refine/refine.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,47 +23,48 @@
 
 #import line_profiler
 #import atexit
 #profile = line_profiler.LineProfiler()
 #atexit.register(profile.print_stats)
 
 class Geom:
-    def __init__(self, st, topo, monlib, sigma_b=10, shake_rms=0, refmac_keywords=None, jellybody_only=False):
+    def __init__(self, st, topo, monlib, sigma_b=10, shake_rms=0,
+                 refmac_keywords=None, unrestrained=False, use_nucleus=False):
         self.st = st
+        self.atoms = [None for _ in range(self.st[0].count_atom_sites())]
+        for cra in self.st[0].all(): self.atoms[cra.atom.serial-1] = cra.atom
         self.lookup = {x.atom: x for x in self.st[0].all()}
         self.geom = ext.Geometry(self.st, monlib.ener_lib)
         self.specs = utils.model.find_special_positions(self.st)
         #cs_count = len(self.st.find_spacegroup().operations())
         for atom, images, matp, mata in self.specs:
             #n_sym = len([x for x in images if x < cs_count]) + 1
             n_sym = len(images) + 1
             self.geom.specials.append(ext.Geometry.Special(atom, matp, mata, n_sym))
         self.sigma_b = sigma_b
-        self.jellybody_only = jellybody_only
+        self.unrestrained = unrestrained
         if shake_rms > 0:
             numpy.random.seed(0)
             utils.model.shake_structure(self.st, shake_rms, copy=False)
             utils.fileio.write_model(self.st, "shaken", pdb=True, cif=True)
-        if not self.jellybody_only:
+        if not self.unrestrained:
             self.geom.load_topo(topo)
-        else:
-            self.geom.ridge_exclude_short_dist = False
-        self.use_nucleus = False
+            self.check_chemtypes(os.path.join(monlib.path(), "ener_lib.cif"), topo)
+        self.use_nucleus = use_nucleus
         self.calc_kwds = {"use_nucleus": self.use_nucleus}
         if refmac_keywords:
             exte.read_external_restraints(refmac_keywords, self.st, self.geom)
             kwds = parse_keywords(refmac_keywords)
             for k in ("wbond", "wangle", "wtors", "wplane", "wchir", "wvdw"):
                 if k in kwds:
                     self.calc_kwds[k] = kwds[k]
                     logger.writeln("setting geometry weight {}= {}".format(k, kwds[k]))
         self.geom.finalize_restraints()
-        self.outlier_sigmas = dict(bond=5, angle=5, torsion=5, vdw=5, chir=5, plane=5, staca=5, stacd=5)
+        self.outlier_sigmas = dict(bond=5, angle=5, torsion=5, vdw=5, chir=5, plane=5, staca=5, stacd=5, per_atom=5)
         self.parents = {}
-        self.check_chemtypes(os.path.join(monlib.path(), "ener_lib.cif"), topo)
     # __init__()
 
     def check_chemtypes(self, enerlib_path, topo):
         block = gemmi.cif.read(enerlib_path).sole_block()
         all_types = set(block.find_values("_lib_atom.type"))
         for ci in topo.chain_infos:
             for ri in ci.res_infos:
@@ -80,15 +81,15 @@
         for bond in self.geom.bonds:
             if bond.atoms[0].is_hydrogen():
                 self.parents[bond.atoms[0]] = bond.atoms[1]
             elif bond.atoms[1].is_hydrogen():
                 self.parents[bond.atoms[1]] = bond.atoms[0]
     # set_h_parents()
     def setup_nonbonded(self, refine_xyz):
-        skip_critical_dist = not refine_xyz or self.jellybody_only
+        skip_critical_dist = not refine_xyz or self.unrestrained
         self.geom.setup_nonbonded(skip_critical_dist=skip_critical_dist)
     def calc(self, target_only):
         return self.geom.calc(check_only=target_only, **self.calc_kwds)
     def calc_adp_restraint(self, target_only):
         return self.geom.calc_adp_restraint(target_only, self.sigma_b)
     def calc_target(self, target_only, refine_xyz, adp_mode):
         self.geom.clear_target()
@@ -143,27 +144,37 @@
                         if len(df0.index) > 0:
                             logger.writeln(" *** External bond outliers (Z >= {}) ***\n".format(self.outlier_sigmas[k]))
                             logger.writeln(df0.to_string(float_format="{:.3f}".format, index=False) + "\n")
                     else:
                         logger.writeln(" *** {} outliers (Z >= {}) ***\n".format(labs[k], self.outlier_sigmas[k]))
                         logger.writeln(df.to_string(float_format="{:.3f}".format, index=False) + "\n")
 
+        # Per-atom score
+        peratom = self.geom.reporting.per_atom_score(len(self.atoms), self.use_nucleus, "mean")
+        df = pandas.DataFrame(peratom)
+        df.insert(0, "atom", [str(self.lookup[x]) for x in self.atoms])
+        df = df[df["total"] >= self.outlier_sigmas["per_atom"]]
+        if show_outliers and len(df.index) > 0:
+            df.sort_values("total", ascending=False, inplace=True)
+            ret["outliers"]["per_atom"] = df
+            logger.writeln(" *** Per-atom violations (Z >= {}) ***\n".format(self.outlier_sigmas["per_atom"]))
+            logger.writeln(df.to_string(float_format="{:.2f}".format, index=False) + "\n")
+
         df = pandas.DataFrame(self.geom.reporting.get_summary_table(self.use_nucleus))
         df = df.set_index("Restraint type").rename_axis(index=None)
         ret["summary"] = df
         logger.writeln(df.to_string(float_format="{:.3f}".format) + "\n")
         return ret
         
 class Refine:
     def __init__(self, st, geom, ll=None, refine_xyz=True, adp_mode=1, refine_h=False, unrestrained=False):
         assert adp_mode in (0, 1, 2) # 0=fix, 1=iso, 2=aniso
         assert geom is not None
         self.st = st # clone()?
-        self.atoms = [None for _ in range(self.st[0].count_atom_sites())]
-        for cra in self.st[0].all(): self.atoms[cra.atom.serial-1] = cra.atom
+        self.atoms = geom.atoms # not a copy
         self.geom = geom
         self.ll = ll
         self.gamma = 0
         self.adp_mode = 0 if self.ll is None else adp_mode
         self.refine_xyz = refine_xyz
         self.unrestrained = unrestrained
         self.refine_h = refine_h
@@ -277,18 +288,14 @@
             ll = 0
 
         f =  w * ll + geom
         return f
 
     #@profile
     def run_cycle(self, weight=1):
-        if self.ll is not None:
-            self.ll.overall_scale()
-            self.ll.update_ml_params()
-
         self.geom.geom.setup_target(self.refine_xyz, self.adp_mode)
             
         if 0: # test of grad
             self.ll.update_fc()
             x0 = self.get_x()
             f0,ader,_ = self.calc_target(weight)
             i = 1
@@ -386,15 +393,28 @@
             self.run_cycle(weight=weight) # check ret?
             stats.append({"Ncyc": i+1})
             if debug: utils.fileio.write_model(self.st, "refined_{:02d}".format(i+1), pdb=True)#, cif=True)
             if self.refine_xyz and not self.unrestrained:
                 stats[-1]["geom"] = self.geom.show_model_stats(show_outliers=(i==ncycles-1))["summary"]
             if self.ll is not None:
                 self.ll.overall_scale()
-                stats[-1]["data"] = self.ll.calc_stats()["summary"]
+                self.ll.update_ml_params()
+                llstats = self.ll.calc_stats(bin_stats=True)#(i==ncycles-1))
+                stats[-1]["data"] = llstats["summary"]
+                if "bin_stats" in llstats:
+                    df = llstats["bin_stats"]
+                    forplot = []
+                    rlabs = [x for x in df if x.startswith("R")]
+                    cclabs = [x for x in df if x.startswith("CC")]
+                    if "fsc_model" in df: forplot.append(["FSC", ["1/resol^2", "fsc_model"]])
+                    if rlabs: forplot.append(["R", ["1/resol^2"] + rlabs])
+                    if cclabs: forplot.append(["CC", ["1/resol^2"] + cclabs])
+                    lstr = utils.make_loggraph_str(df, "Data stats in cycle {}".format(i+1), forplot,
+                                                   float_format="{:.4f}".format)
+                    logger.writeln(lstr)
             if self.adp_mode > 0:
                 utils.model.adp_analysis(self.st)
             logger.writeln("")
 
         # Make table
         data_keys, geom_keys = set(), set()
         tmp = []
@@ -415,14 +435,17 @@
         df = pandas.DataFrame(tmp)
         forplot = []
         if "FSCaverage" in data_keys:
             forplot.append(["FSC", ["Ncyc", "FSCaverage"]])
         r_keys = [x for x in data_keys if x.startswith("R")]
         if r_keys:
             forplot.append(["R", ["Ncyc"] + r_keys])
+        cc_keys = [x for x in data_keys if x.startswith("CC")]
+        if cc_keys:
+            forplot.append(["CC", ["Ncyc"] + cc_keys])
         if "-LL" in data_keys:
             forplot.append(["-LL", ["Ncyc", "-LL"]])
         rms_keys = [x for x in geom_keys if x.startswith("rms")]
         if rms_keys:
             forplot.append(["Geometry", ["Ncyc"] + rms_keys])
         z_keys = [x for x in geom_keys if x.startswith("z")]
         if z_keys:
```

### Comparing `servalcat-0.4.15/servalcat/refine/refine_geom.py` & `servalcat-0.4.24/servalcat/refine/refine_geom.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,27 +54,34 @@
         if len(st) > 0: break
     else:
         raise SystemExit("No model in the cif file")
     monlib = utils.restraints.load_monomer_library(st, monomer_dir=monomer_dir, # monlib is needed for ener_lib
                                                    cif_files=[cif_in],
                                                    stop_for_unknowns=True)
     try:
-        topo = utils.restraints.prepare_topology(st, monlib, h_change=gemmi.HydrogenChange.ReAdd,
-                                                 check_hydrogen=False)
+        topo, _ = utils.restraints.prepare_topology(st, monlib, h_change=gemmi.HydrogenChange.ReAdd,
+                                                    check_hydrogen=False)
     except RuntimeError as e:
         raise SystemExit("Error: {}".format(e))
 
     geom = Geom(st, topo, monlib, shake_rms=randomize)
     refiner = Refine(st, geom)
     logger.writeln("Running {} cycles with wchir=4 wvdw=2".format(ncycle1))
     geom.calc_kwds["wchir"] = 4
     geom.calc_kwds["wvdw"] = 2
     refiner.run_cycles(ncycle1)
+
+    # re-add hydrogen may help
+    topo = gemmi.prepare_topology(st, monlib, h_change=gemmi.HydrogenChange.ReAdd,
+                                  warnings=logger)
+    geom = Geom(st, topo, monlib)
+    refiner = Refine(st, geom)
     logger.writeln("Running {} cycles with wchir=1 wvdw=2".format(ncycle2))
     geom.calc_kwds["wchir"] = 1
+    geom.calc_kwds["wvdw"] = 2
     refiner.run_cycles(ncycle2)
 
     # replace xyz
     pos = {cra.atom.name: cra.atom.pos.tolist() for cra in refiner.st[0].all()}
     for row in block.find("_chem_comp_atom.", ["atom_id", "x", "y", "z"]):
         p = pos[row.str(0)]
         for i in range(3):
@@ -95,33 +102,35 @@
         if tag in tags: row[tags.index(tag)] = val
     loop.add_row(gemmi.cif.quote_list(row))
     doc.write_file(output_prefix + "_updated.cif", style=gemmi.cif.Style.Aligned)
 # refine_and_update_dictionary()
 
 def refine_geom(model_in, monomer_dir, cif_files, h_change, ncycle, output_prefix, randomize, refmac_keywords):
     st = utils.fileio.read_structure(model_in)
-    utils.model.setup_entities(st, clear=True, force_subchain_names=True)
+    utils.model.setup_entities(st, clear=True, force_subchain_names=True, overwrite_entity_type=True)
     if st.ncs:
         st2 = st.clone()
         logger.writeln("Take NCS constraints into account.")
         st2.expand_ncs(gemmi.HowToNameCopiedChain.Dup)
         utils.fileio.write_model(st2, file_name="input_expanded.pdb")
 
     monlib = utils.restraints.load_monomer_library(st, monomer_dir=monomer_dir,
                                                    cif_files=cif_files,
                                                    stop_for_unknowns=True)
     utils.restraints.find_and_fix_links(st, monlib) # should remove unknown id here?
     try:
-        topo = utils.restraints.prepare_topology(st, monlib, h_change=h_change,
-                                                 check_hydrogen=(h_change==gemmi.HydrogenChange.NoChange))
+        topo, metal_kws = utils.restraints.prepare_topology(st, monlib, h_change=h_change,
+                                                            check_hydrogen=(h_change==gemmi.HydrogenChange.NoChange))
     except RuntimeError as e:
         raise SystemExit("Error: {}".format(e))
+    refmac_keywords.extend(metal_kws)
     geom = Geom(st, topo, monlib, shake_rms=randomize, refmac_keywords=refmac_keywords)
     refiner = Refine(st, geom)
     stats = refiner.run_cycles(ncycle)
+    refiner.st.name = output_prefix
     utils.fileio.write_model(refiner.st, output_prefix, pdb=True, cif=True)
     with open(output_prefix + "_stats.json", "w") as ofs:
         for s in stats: s["geom"] = s["geom"].to_dict()
         json.dump(stats, ofs, indent=2)
         logger.writeln("Refinement statistics saved: {}".format(ofs.name))
 # refine_geom()
```

### Comparing `servalcat-0.4.15/servalcat/refine/refine_spa.py` & `servalcat-0.4.24/servalcat/refine/refine_spa.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,16 @@
                         help="Jelly body sigma and dmax (default: %(default)s)")
     parser.add_argument('--jellyonly', action='store_true',
                         help="Jelly body only (experimental, may not be useful)")
     utils.symmetry.add_symmetry_args(parser) # add --pg etc
     parser.add_argument('--contacting_only', action="store_true", help="Filter out non-contacting NCS")
     parser.add_argument('--ignore_symmetry',
                         help='Ignore symmetry information (MTRIX/_struct_ncs_oper) in the model file')
+    parser.add_argument('--no_link_check', action='store_true', 
+                        help='Do not find and fix link records in input model.')
     parser.add_argument('--no_check_ncs_overlaps', action='store_true', 
                         help='Disable model overlap (e.g. expanded model is used with --pg) test')
     parser.add_argument('--no_check_ncs_map', action='store_true', 
                         help='Disable map NCS consistency test')
     parser.add_argument('--no_check_mask_with_model', action='store_true', 
                         help='Disable mask test using model')
     parser.add_argument('--keywords', nargs='+', action="append",
@@ -117,45 +119,47 @@
     args.cross_validation_method = "throughout"
     check_args(args)    
     refmac_keywords = args.keywords + [l for f in args.keyword_file for l in open(f)]
 
     st = utils.fileio.read_structure(args.model)
     monlib = utils.restraints.load_monomer_library(st, monomer_dir=args.monlib, cif_files=args.ligand,
                                                    stop_for_unknowns=True)
-    utils.model.setup_entities(st, clear=True, force_subchain_names=True)
-    utils.restraints.find_and_fix_links(st, monlib)
+    utils.model.setup_entities(st, clear=True, force_subchain_names=True, overwrite_entity_type=True)
     if args.hklin:
         assert not args.cross_validation
         mtz = utils.fileio.read_mmhkl(args.hklin)
         hkldata = utils.hkl.hkldata_from_mtz(mtz, args.labin.split(","),
                                              newlabels=["FP", ""],
                                              require_types=["F", "P"])
         hkldata.df = hkldata.df.dropna() # workaround for missing data
         #hkldata.setup_relion_binning()
         hkldata.setup_binning(n_bins=10) # need to sort out
         st.cell = hkldata.cell
         st.spacegroup_hm = hkldata.sg.xhm()
+        st.setup_cell_images()
         info = {}
+        if not args.no_link_check:
+            utils.restraints.find_and_fix_links(st, monlib)
     else:
         if args.halfmaps:
             maps = utils.fileio.read_halfmaps(args.halfmaps, pixel_size=args.pixel_size)
         else:
             maps = [utils.fileio.read_ccp4_map(args.map, pixel_size=args.pixel_size)]
         hkldata, info = process_input(st, maps, resolution=args.resolution - 1e-6, monlib=monlib,
-                                      mask_in=args.mask, args=args, use_refmac=False)
-    st.setup_cell_images()
+                                      mask_in=args.mask, args=args, use_refmac=False,
+                                      fix_link=not args.no_link_check)
     h_change = {"all":gemmi.HydrogenChange.ReAddButWater,
                 "yes":gemmi.HydrogenChange.NoChange,
                 "no":gemmi.HydrogenChange.Remove}[args.hydrogen]
     try:
-        topo = utils.restraints.prepare_topology(st, monlib, h_change=h_change,
-                                                 check_hydrogen=(args.hydrogen=="yes"))
+        topo, metal_kws = utils.restraints.prepare_topology(st, monlib, h_change=h_change,
+                                                            check_hydrogen=(args.hydrogen=="yes"))
     except RuntimeError as e:
         raise SystemExit("Error: {}".format(e))
-
+    refmac_keywords.extend(metal_kws)
     # initialize ADP
     if args.adp != "fix":
         utils.model.reset_adp(st[0], args.bfactor, args.adp == "aniso")
 
     # auto weight
     if args.weight is None:
         # from 230303_weight_test using 472 test cases
@@ -174,34 +178,39 @@
                 rlmc = (-1.7588, 0.6311)
             logger.writeln("Estimating weight auto scale using resolution")
             ws =  numpy.exp(rlmc[0] + args.resolution*rlmc[1])
         args.weight = max(0.2, min(18.0, ws))
         logger.writeln(" Will use weight= {:.2f}".format(args.weight))
 
     geom = Geom(st, topo, monlib, shake_rms=args.randomize, sigma_b=args.sigma_b,
-                refmac_keywords=refmac_keywords, jellybody_only=args.jellyonly)
+                refmac_keywords=refmac_keywords, unrestrained=args.jellyonly)
     ll = spa.LL_SPA(hkldata, st, monlib,
                     lab_obs="F_map1" if args.cross_validation else "FP",
                     source=args.source)
     refiner = Refine(st, geom, ll,
                      refine_xyz=not args.fix_xyz,
                      adp_mode=dict(fix=0, iso=1, aniso=2)[args.adp],
                      refine_h=args.refine_h)
 
     geom.geom.adpr_max_dist = args.max_dist_for_adp_restraint
     if args.adp_restraint_power is not None: geom.geom.adpr_d_power = args.adp_restraint_power
     if args.adp_restraint_exp_fac is not None: geom.geom.adpr_exp_fac = args.adp_restraint_exp_fac
     if args.jellybody or args.jellyonly: geom.geom.ridge_sigma, geom.geom.ridge_dmax = args.jellybody_params
+    if args.jellyonly: geom.geom.ridge_exclude_short_dist = False
 
     #logger.writeln("TEST: shift x+0.3 A")
     #for cra in st[0].all():
     #    cra.atom.pos += gemmi.Position(0.3,0,0)
 
     stats = refiner.run_cycles(args.ncycle, weight=args.weight)
-    if not args.hklin and not args.no_trim: refiner.st.cell = maps[0][0].unit_cell
+    if not args.hklin and not args.no_trim:
+        refiner.st.cell = maps[0][0].unit_cell
+        refiner.st.setup_cell_images()
+
+    refiner.st.name = args.output_prefix
     utils.fileio.write_model(refiner.st, args.output_prefix, pdb=True, cif=True)
     with open(args.output_prefix + "_stats.json", "w") as ofs:
         for s in stats:
             if "geom" in s: s["geom"] = s["geom"].to_dict()
         json.dump(stats, ofs, indent=2)
         logger.writeln("Refinement statistics saved: {}".format(ofs.name))
```

### Comparing `servalcat-0.4.15/servalcat/refine/refine_xtal.py` & `servalcat-0.4.24/servalcat/refine/refine_xtal.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     parser.add_argument('--jellybody', action='store_true',
                         help="Use jelly body restraints")
     parser.add_argument('--jellybody_params', nargs=2, type=float,
                         metavar=("sigma", "dmax"), default=[0.01, 4.2],
                         help="Jelly body sigma and dmax (default: %(default)s)")
     parser.add_argument('--jellyonly', action='store_true',
                         help="Jelly body only (experimental, may not be useful)")
+    parser.add_argument('--no_link_check', action='store_true', 
+                        help='Do not find and fix link records in input model.')
     parser.add_argument('--keywords', nargs='+', action="append",
                         help="refmac keyword(s)")
     parser.add_argument('--keyword_file', nargs='+', action="append",
                         help="refmac keyword file(s)")
     parser.add_argument('--randomize', type=float, default=0,
                         help='Shake coordinates with specified rmsd')
     parser.add_argument('--ncycle', type=int, default=10,
@@ -59,29 +61,30 @@
     parser.add_argument('--bfactor', type=float,
                         help="reset all atomic B values to specified value")
     parser.add_argument('--fix_xyz', action="store_true")
     parser.add_argument('--adp',  choices=["fix", "iso", "aniso"], default="iso")
     parser.add_argument('--max_dist_for_adp_restraint', type=float, default=4.)
     parser.add_argument('--unrestrained',  action='store_true', help="No positional restraints")
     parser.add_argument('--refine_h', action="store_true", help="Refine hydrogen (default: restraints only)")
-    parser.add_argument("--source", choices=["electron", "xray", "neutron"], default="electron")
+    parser.add_argument("-s", "--source", choices=["electron", "xray", "neutron"], required=True)
     parser.add_argument('--no_solvent',  action='store_true',
                         help="Do not consider bulk solvent contribution")
     parser.add_argument('--use_all_in_est',  action='store_true',
                         help="Use all reflections in ML parameter estimates")
     parser.add_argument('-o','--output_prefix')
 # add_arguments()
 
 def parse_args(arg_list):
     parser = argparse.ArgumentParser()
     add_arguments(parser)
     return parser.parse_args(arg_list)
 # parse_args()
 
 def main(args):
+    if args.source == "neutron": assert not args.refine_h # we need deuterium fraction handling in LL
     if not args.output_prefix:
         args.output_prefix = utils.fileio.splitext(os.path.basename(args.model))[0] + "_refined"
 
     keywords = []
     if args.keywords or args.keyword_file:
         if args.keywords: keywords = sum(args.keywords, [])
         if args.keyword_file: keywords.extend(l for f in sum(args.keyword_file, []) for l in open(f))
@@ -108,54 +111,67 @@
                                                                   d_min=args.d_min,
                                                                   n_per_bin=n_per_bin,
                                                                   use=use_in_est,
                                                                   max_bins=30)
 
     is_int = "I" in hkldata.df
     st = sts[0]
-    monlib = utils.restraints.load_monomer_library(st, monomer_dir=args.monlib, cif_files=args.ligand,
-                                                   stop_for_unknowns=False)
-    utils.model.setup_entities(st, clear=True, force_subchain_names=True)
-    utils.restraints.find_and_fix_links(st, monlib)
-    h_change = {"all":gemmi.HydrogenChange.ReAddButWater,
-                "yes":gemmi.HydrogenChange.NoChange,
-                "no":gemmi.HydrogenChange.Remove}[args.hydrogen]
-    try:
-        topo = utils.restraints.prepare_topology(st, monlib, h_change=h_change,
-                                                 check_hydrogen=(args.hydrogen=="yes"))
-    except RuntimeError as e:
-        raise SystemExit("Error: {}".format(e))
-
+    utils.model.fix_deuterium_residues(st)
+    if args.unrestrained:
+        monlib = gemmi.MonLib()
+        topo = None
+        if args.hydrogen == "all":
+            logger.writeln("WARNING: in unrestrained refinement hydrogen atoms are not generated.")
+        elif args.hydrogen == "no":
+            st.remove_hydrogens()
+        for i, cra in enumerate(st[0].all()):
+            cra.atom.serial = i + 1
+    else:
+        monlib = utils.restraints.load_monomer_library(st, monomer_dir=args.monlib, cif_files=args.ligand,
+                                                       stop_for_unknowns=False)
+        utils.model.setup_entities(st, clear=True, force_subchain_names=True, overwrite_entity_type=True)
+        if not args.no_link_check:
+            utils.restraints.find_and_fix_links(st, monlib)
+        h_change = {"all":gemmi.HydrogenChange.ReAddButWater,
+                    "yes":gemmi.HydrogenChange.NoChange,
+                    "no":gemmi.HydrogenChange.Remove}[args.hydrogen]
+        try:
+            topo, metal_kws = utils.restraints.prepare_topology(st, monlib, h_change=h_change,
+                                                                check_hydrogen=(args.hydrogen=="yes"))
+        except RuntimeError as e:
+            raise SystemExit("Error: {}".format(e))
+        keywords.extend(metal_kws)
     # initialize ADP
     if args.adp != "fix":
         utils.model.reset_adp(st[0], args.bfactor, args.adp == "aniso")
     
     geom = Geom(st, topo, monlib, shake_rms=args.randomize, sigma_b=args.sigma_b, refmac_keywords=keywords,
-                jellybody_only=args.jellyonly)
+                unrestrained=args.unrestrained or args.jellyonly, use_nucleus=(args.source=="neutron"))
     geom.geom.adpr_max_dist = args.max_dist_for_adp_restraint
     if args.jellybody or args.jellyonly:
         geom.geom.ridge_sigma, geom.geom.ridge_dmax = args.jellybody_params
+    if args.jellyonly: geom.geom.ridge_exclude_short_dist = False
 
     ll = LL_Xtal(hkldata, centric_and_selections, args.free, st, monlib, source=args.source,
                  use_solvent=not args.no_solvent, use_in_est=use_in_est, use_in_target=use_in_target)
     refiner = Refine(st, geom, ll=ll,
                      refine_xyz=not args.fix_xyz,
                      adp_mode=dict(fix=0, iso=1, aniso=2)[args.adp],
                      refine_h=args.refine_h,
                      unrestrained=args.unrestrained)
 
     refiner.run_cycles(args.ncycle, weight=args.weight)
+    refiner.st.name = args.output_prefix
     utils.fileio.write_model(refiner.st, args.output_prefix, pdb=True, cif=True)
 
-    # CHECK ML parameters are determined from the last model?
     if is_int:
         calculate_maps_int(ll.hkldata, ll.b_aniso, ll.fc_labs, ll.D_labs, centric_and_selections,
                            use=use_in_target)
     else:
-        calculate_maps(ll.hkldata, centric_and_selections, ll.fc_labs, ll.D_labs, args.output_prefix + "_stats.log",
+        calculate_maps(ll.hkldata, ll.b_aniso, centric_and_selections, ll.fc_labs, ll.D_labs, args.output_prefix + "_stats.log",
                        use=use_in_target)
 
     # Write mtz file
     if is_int:
         labs = ["I", "SIGI"]
     else:
         labs = ["FP", "SIGFP", "FOM"]
```

### Comparing `servalcat-0.4.15/servalcat/refine/spa.py` & `servalcat-0.4.24/servalcat/refine/spa.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,18 +80,20 @@
         for i_bin, idxes in self.hkldata.binned():
             Fo = self.hkldata.df[self.lab_obs].to_numpy()[idxes]
             DFc = self.hkldata.df.FC.to_numpy()[idxes] * self.hkldata.binned_df.D[i_bin]
             ret += numpy.nansum(numpy.abs(Fo - DFc)**2) / self.hkldata.binned_df.S[i_bin]
         return ret * 2 # friedel mates
     # calc_target()
 
-    def calc_stats(self):
+    def calc_stats(self, bin_stats=False):
+        # ignore bin_stats for now. better stats are calculated after refinement
         stats = fsc.calc_fsc_all(self.hkldata, labs_fc=["FC"], lab_f=self.lab_obs)
         fsca = fsc.fsc_average(stats.ncoeffs, stats.fsc_FC_full)
         logger.writeln("FSCaverage = {:.4f}".format(fsca))
+        # XXX in fsc object, _full is misleading - it's not full in cross validation mode
         return {"fsc": stats, "summary": {"FSCaverage": fsca, "-LL": self.calc_target()}}
 
     def calc_grad(self, refine_xyz, adp_mode, refine_h, specs):
         dll_dab = numpy.empty_like(self.hkldata.df[self.lab_obs])
         d2ll_dab2 = numpy.zeros(len(self.hkldata.df.index))
         blur = utils.model.determine_blur_for_dencalc(self.st, self.d_min / 3) # TODO need more work
         logger.writeln("blur for deriv= {:.2f}".format(blur))
```

### Comparing `servalcat-0.4.15/servalcat/refine/xtal.py` & `servalcat-0.4.24/servalcat/refine/xtal.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,25 +7,77 @@
 """
 from __future__ import absolute_import, division, print_function, generators
 import gemmi
 import numpy
 import json
 import scipy.sparse
 from servalcat.utils import logger
-#from servalcat.xtal.sigmaa import determine_mlf_params, determine_mlf_params_from_cc, mlf, calc_DFc
 from servalcat.xtal import sigmaa
 from servalcat import utils
 from servalcat import ext
 b_to_u = utils.model.b_to_u
 u_to_b = utils.model.u_to_b
 
+def calc_bin_stats(hkldata, centric_and_selections):
+    has_int = "I" in hkldata.df
+    has_free = "FREE" in hkldata.df
+    stats = hkldata.binned_df[["d_max", "d_min"]].copy()
+    stats["1/resol^2"] = 1 / stats.d_min**2
+    stats["n_obs"] = 0
+    if has_free:
+        stats[["n_work", "n_free"]] = 0
+    rlab = "R2" if has_int else "R"
+    cclab = "CCI" if has_int else "CCF"
+    Fc = numpy.abs(hkldata.df.FC * hkldata.df.k_aniso)
+    if has_int:
+        obs = hkldata.df.I
+        calc = Fc**2
+    else:
+        obs = hkldata.df.FP
+        calc = Fc
+    if has_free:
+        for suf in ("work", "free"):
+            stats[cclab+suf] = numpy.nan
+            stats[rlab+suf] = numpy.nan
+    else:
+        stats[cclab] = numpy.nan
+        stats[rlab] = numpy.nan
+
+    for i_bin, idxes in hkldata.binned():
+        stats.loc[i_bin, "n_obs"] = numpy.sum(numpy.isfinite(obs[idxes]))
+        if has_free:
+            for j, suf in ((1, "work"), (2, "free")):
+                idxes2 = numpy.concatenate([sel[j] for sel in centric_and_selections[i_bin]])
+                stats.loc[i_bin, "n_"+suf] = numpy.sum(numpy.isfinite(obs[idxes2]))
+                stats.loc[i_bin, cclab+suf] = utils.hkl.correlation(obs[idxes2], calc[idxes2])
+                stats.loc[i_bin, rlab+suf] = utils.hkl.r_factor(obs[idxes2], calc[idxes2])
+        else:
+            stats.loc[i_bin, cclab] = utils.hkl.correlation(obs[idxes], calc[idxes])
+            stats.loc[i_bin, rlab] = utils.hkl.r_factor(obs[idxes], calc[idxes])
+    return stats
+# calc_bin_stats()
+
+def calc_cc_avg(stats):
+    cc_labs = [x for x in stats if x.startswith("CC")]
+    ret = {x+"avg" : numpy.nan for x in cc_labs}
+    for lab in cc_labs:
+        if lab.endswith("work"):
+            weights = stats["n_work"]
+        elif lab.endswith("free"):
+            weights = stats["n_free"]
+        else:
+            weights = stats["n_obs"]
+        ret[lab+"avg"] = numpy.average(stats[lab], weights=weights)
+    return ret
+# calc_cc_avg()
+
 class LL_Xtal:
     def __init__(self, hkldata, centric_and_selections, free, st, monlib, source="xray", mott_bethe=True,
                  use_solvent=False, use_in_est="all", use_in_target="all"):
-        assert source in ("electron", "xray") # neutron?
+        assert source in ("electron", "xray", "neutron")
         self.source = source
         self.mott_bethe = False if source != "electron" else mott_bethe
         self.hkldata = hkldata
         self.is_int = "I" in self.hkldata.df
         self.centric_and_selections = centric_and_selections
         self.free = free
         self.st = st
@@ -34,35 +86,27 @@
         self.fc_labs = ["FC0"]
         self.use_solvent = use_solvent
         if use_solvent:
             self.fc_labs.append("FCbulk")
             self.hkldata.df["FCbulk"] = 0j
         self.D_labs = ["D{}".format(i) for i in range(len(self.fc_labs))]
         self.k_overall = numpy.ones(len(self.hkldata.df.index))
-        self.b_aniso = None # used by MLI for now
+        self.b_aniso = None
         self.hkldata.df["k_aniso"] = 1.
-        if not self.is_int:
-            self.hkldata.df["FP_org"] = self.hkldata.df["FP"]
-            self.hkldata.df["SIGFP_org"] = self.hkldata.df["SIGFP"]
         self.use_in_est = use_in_est
         self.use_in_target = use_in_target
         self.ll = None
         logger.writeln("will use {} reflections for parameter estimation".format(self.use_in_est))
         logger.writeln("will use {} reflections for refinement".format(self.use_in_target))
 
     def update_ml_params(self):
-        # FIXME make sure D > 0
-        if self.is_int:
-            self.b_aniso = sigmaa.determine_mli_params(self.hkldata, self.fc_labs, self.D_labs, self.b_aniso,
-                                                       self.centric_and_selections, use=self.use_in_est,
-                                                       )#D_as_exp=True, S_as_exp=True)
-            self.hkldata.df["k_aniso"] = self.hkldata.debye_waller_factors(b_cart=self.b_aniso)
-        else:
-            sigmaa.determine_mlf_params(self.hkldata, self.fc_labs, self.D_labs,
-                                        self.centric_and_selections, use=self.use_in_est)#, D_as_exp=True, S_as_exp=True)
+        self.b_aniso = sigmaa.determine_ml_params(self.hkldata, self.is_int, self.fc_labs, self.D_labs, self.b_aniso,
+                                                   self.centric_and_selections, use=self.use_in_est,
+                                                   D_trans="splus", S_trans="splus")
+        self.hkldata.df["k_aniso"] = self.hkldata.debye_waller_factors(b_cart=self.b_aniso)
         for lab in self.D_labs + ["S"]:
             self.hkldata.binned_df[lab].where(self.hkldata.binned_df[lab] > 0, 0.01, inplace=True)
             self.hkldata.binned_df[lab].where(self.hkldata.binned_df[lab] < numpy.inf, 1, inplace=True)
         #determine_mlf_params_from_cc(self.hkldata, self.fc_labs, self.D_labs,
         #                             self.centric_and_selections)
 
 
@@ -82,115 +126,114 @@
         
     def overall_scale(self, min_b=0.1):
         fc_list = [self.hkldata.df[self.fc_labs[0]].to_numpy()]
         if self.use_solvent:
             Fmask = sigmaa.calc_Fmask(self.st, self.d_min - 1e-6, self.hkldata.miller_array())
             fc_list.append(Fmask)
 
-        obs = self.hkldata.df["I" if self.is_int else "FP_org"].to_numpy()
-        scaling = sigmaa.LsqScale(self.hkldata, obs, fc_list, self.is_int)
+        scaling = sigmaa.LsqScale(self.hkldata, fc_list, self.is_int, sigma_cutoff=0)
         scaling.scale()
-        b_aniso = scaling.b_aniso
+        self.b_aniso = scaling.b_aniso
         b = scaling.b_iso
         min_b_iso = utils.model.minimum_b(self.st[0]) # actually min of aniso too
         tmp = min_b_iso + b
         if tmp < min_b: # perhaps better only adjust b_iso that went too small, but we need to recalculate Fc
             logger.writeln(" Adjusting overall B to avoid too small value")
             b += min_b - tmp
         logger.writeln(" Applying overall B to model: {:.2f}".format(b))
         utils.model.shift_b(self.st[0], b)
         k_iso = self.hkldata.debye_waller_factors(b_iso=b)
-        k_aniso = self.hkldata.debye_waller_factors(b_cart=b_aniso)
+        self.hkldata.df["k_aniso"] = self.hkldata.debye_waller_factors(b_cart=self.b_aniso)
         if self.use_solvent:
-            solvent_scale = scaling.get_solvent_scale(scaling.k_sol, scaling.b_sol)
+            solvent_scale = scaling.get_solvent_scale(scaling.k_sol, scaling.b_sol,
+                                                      1. / self.hkldata.d_spacings().to_numpy()**2)
             self.hkldata.df[self.fc_labs[-1]] = Fmask * solvent_scale
         if self.is_int:
-            self.b_aniso = b_aniso
             self.hkldata.df["I"] /= scaling.k_overall**2
             self.hkldata.df["SIGI"] /= scaling.k_overall**2
         else:
-            self.hkldata.df["k_aniso"] = scaling.k_overall * k_aniso
-            self.hkldata.df["FP"] = self.hkldata.df["FP_org"] / self.hkldata.df.k_aniso
-            self.hkldata.df["SIGFP"] = self.hkldata.df["SIGFP_org"] /self.hkldata.df.k_aniso            
+            self.hkldata.df["FP"] /= scaling.k_overall
+            self.hkldata.df["SIGFP"] /= scaling.k_overall
 
         for lab in self.fc_labs: self.hkldata.df[lab] *= k_iso
         self.hkldata.df["FC"] = self.hkldata.df[self.fc_labs].sum(axis=1)
     # overall_scale()
 
     def calc_target(self): # -LL target for MLF or MLI
         ret = 0
-        if self.is_int:
-            k_aniso = self.hkldata.debye_waller_factors(b_cart=self.b_aniso)
-        else:
-            k_aniso = None
+        k_aniso = self.hkldata.debye_waller_factors(b_cart=self.b_aniso)
+        # in MLF, df.k_aniso is used
             
-        for i_bin, idxes in self.hkldata.binned():
+        for i_bin, _ in self.hkldata.binned():
+            Ds = [self.hkldata.binned_df.loc[i_bin, lab] for lab in self.D_labs]
             if self.is_int:
-                Ds = [self.hkldata.binned_df[lab][i_bin] for lab in self.D_labs]
-                Fcs = [self.hkldata.df[lab].to_numpy()[idxes] for lab in self.fc_labs]
-                DFc = sigmaa.calc_DFc(Ds, Fcs)
-                ll = ext.ll_int(self.hkldata.df.I[idxes], self.hkldata.df.SIGI[idxes], k_aniso[idxes],
-                                self.hkldata.binned_df.S[i_bin] * self.hkldata.df.epsilon[idxes],
-                                numpy.abs(DFc), self.hkldata.df.centric[idxes]+1)
-                ret += numpy.nansum(ll)
+                if self.use_in_target == "all":
+                    idxes = numpy.concatenate([sel[i] for sel in self.centric_and_selections[i_bin] for i in (1,2)])
+                else:
+                    i = 1 if self.use_in_target == "work" else 2
+                    idxes = numpy.concatenate([sel[i] for sel in self.centric_and_selections[i_bin]])
+                ret += sigmaa.mli(self.hkldata.df,
+                                  self.fc_labs,
+                                  Ds,
+                                  self.hkldata.binned_df.S[i_bin],
+                                  k_aniso,
+                                  idxes)
             else:
                 ret += sigmaa.mlf(self.hkldata.df,
                                   self.fc_labs,
-                                  [self.hkldata.binned_df.loc[i_bin, lab] for lab in self.D_labs],
+                                  Ds,
                                   self.hkldata.binned_df.S[i_bin],
                                   self.centric_and_selections[i_bin],
                                   use=self.use_in_target)
 
         return ret * 2 # friedel mates
     # calc_target()
 
-    def calc_stats(self):
+    def calc_stats(self, bin_stats=False):
         if self.is_int:
             calc_r = lambda sel: utils.hkl.r_factor(self.hkldata.df.I[sel],
                                                     numpy.abs(self.hkldata.df.FC[sel] * self.hkldata.df.k_aniso[sel])**2)
             rlab = "R2"
+            cclab = "CCI"
         else:
-            calc_r = lambda sel: utils.hkl.r_factor(self.hkldata.df.FP_org[sel],
+            calc_r = lambda sel: utils.hkl.r_factor(self.hkldata.df.FP[sel],
                                                     numpy.abs(self.hkldata.df.FC[sel] * self.hkldata.df.k_aniso[sel]))
             rlab = "R"
+            cclab = "CCF"
         ret = {"summary": {}}
+        stats = calc_bin_stats(self.hkldata, self.centric_and_selections)
+        ret["summary"].update(calc_cc_avg(stats))
         if "FREE" in self.hkldata.df:
             test_sel = (self.hkldata.df.FREE == self.free).fillna(False)
             r_free = calc_r(test_sel)
             r_work = calc_r(~test_sel)
             logger.writeln("{}_work = {:.4f} {}_free = {:.4f}".format(rlab, r_work, rlab, r_free))
             ret["summary"]["{}work".format(rlab)] = r_work
             ret["summary"]["{}free".format(rlab)] = r_free
+            cc_free = ret["summary"]["{}freeavg".format(cclab)]
+            cc_work = ret["summary"]["{}workavg".format(cclab)]
+            logger.writeln("{}avg_work = {:.4f} {}avg_free = {:.4f}".format(cclab, cc_work, cclab, cc_free))
         else:
-            if self.is_int:
-                r = utils.hkl.r_factor(self.hkldata.df.I,
-                                       numpy.abs(self.hkldata.df.FC * self.hkldata.df.k_aniso)**2)
-            else:
-                r = utils.hkl.r_factor(self.hkldata.df.FP_org,
-                                       numpy.abs(self.hkldata.df.FC * self.hkldata.df.k_aniso))
+            r = calc_r(slice(None))
+            cc = ret["summary"]["{}avg".format(cclab)]
             logger.writeln("{} = {:.4f}".format(rlab, r))
+            logger.writeln("{}avg = {:.4f}".format(cclab, cc))
             ret["summary"][rlab] = r
-            if self.is_int:
-                cc = utils.hkl.correlation(self.hkldata.df.I,
-                                           (numpy.abs(self.hkldata.df.FC) * self.hkldata.df.k_aniso)**2)
-                logger.writeln("CC = {:.4f}".format(cc))
-                ret["summary"]["CC"] = cc
         ret["summary"]["-LL"] = self.calc_target()
+        if bin_stats:
+            ret["bin_stats"] = stats
         return ret
 
     def calc_grad(self, refine_xyz, adp_mode, refine_h, specs):
         dll_dab = numpy.zeros(len(self.hkldata.df.FC), dtype=numpy.complex128)
         d2ll_dab2 = numpy.empty(len(self.hkldata.df.index))
         d2ll_dab2[:] = numpy.nan
         blur = utils.model.determine_blur_for_dencalc(self.st, self.d_min / 3) # TODO need more work
         logger.writeln("blur for deriv= {:.2f}".format(blur))
-        if self.is_int:
-            k_ani = self.hkldata.debye_waller_factors(b_cart=self.b_aniso)
-        else:
-            k_ani = None
+        k_ani = self.hkldata.debye_waller_factors(b_cart=self.b_aniso)
         for i_bin, _ in self.hkldata.binned():
             bin_d_min = self.hkldata.binned_df.d_min[i_bin]
             bin_d_max = self.hkldata.binned_df.d_max[i_bin]
             Ds = [max(0., self.hkldata.binned_df[lab][i_bin]) for lab in self.D_labs] # negative D is replaced with zero here
             S = self.hkldata.binned_df.S[i_bin]
             for c, work, test in self.centric_and_selections[i_bin]:
                 if self.use_in_target == "all":
@@ -218,49 +261,56 @@
                     #d2ll_dab2[cidxes] = (2-c)**2 / S / epsilon * Ds[0]**2 # approximation
                     #d2ll_dab2[cidxes] = ((2-c) / S / epsilon + ((2-c) * r / k_ani[cidxes] / epsilon / S)**2) * Ds[0]**2
                     d2ll_dab2[cidxes] =  ((2-c) * (Fc_abs - r / k_ani[cidxes]) / epsilon / S  * Ds[0])**2
                 else:
                     Fo = self.hkldata.df.FP.to_numpy()[cidxes]
                     SigFo = self.hkldata.df.SIGFP.to_numpy()[cidxes]
                     if c == 0: # acentric
-                        Sigma = 2 * SigFo**2 + epsilon * S
-                        X = 2 * Fo * Fc_abs / Sigma
+                        Sigma = 2 * SigFo**2 + epsilon * S * k_ani[cidxes]**2
+                        X = 2 * Fo * Fc_abs * k_ani[cidxes] / Sigma
                         m = gemmi.bessel_i1_over_i0(X)
-                        g = (2 * Fc_abs / Sigma - m * 2 * Fo / Sigma) * Ds[0]  # XXX assuming 0 is atomic structure
+                        g = (2 * k_ani[cidxes]**2 * Fc_abs / Sigma - m * 2 * Fo * k_ani[cidxes] / Sigma) * Ds[0]  # XXX assuming 0 is atomic structure
                         dll_dab[cidxes] = g * expip
-                        d2ll_dab2[cidxes] = (2 / Sigma - (1 - m / X - m**2) * (2 * Fo / Sigma)**2) * Ds[0]**2
+                        d2ll_dab2[cidxes] = (2 * k_ani[cidxes]**2 / Sigma - (1 - m / X - m**2) * (2 * Fo * k_ani[cidxes] / Sigma)**2) * Ds[0]**2
                     else:
-                        Sigma = SigFo**2 + epsilon * S
-                        X = Fo * Fc_abs / Sigma
+                        Sigma = SigFo**2 + epsilon * S * k_ani[cidxes]**2
+                        X = Fo * Fc_abs * k_ani[cidxes] / Sigma
                         #X = X.astype(numpy.float64)
                         m = numpy.tanh(X)
-                        g = (Fc_abs / Sigma - m * Fo / Sigma) * Ds[0]
+                        g = (Fc_abs * k_ani[cidxes]**2 / Sigma - m * Fo * k_ani[cidxes] / Sigma) * Ds[0]
                         dll_dab[cidxes] = g * expip
-                        d2ll_dab2[cidxes] = (1 / Sigma - (Fo / (Sigma * numpy.cosh(X)))**2) * Ds[0]**2
+                        d2ll_dab2[cidxes] = (k_ani[cidxes]**2 / Sigma - (Fo * k_ani[cidxes] / (Sigma * numpy.cosh(X)))**2) * Ds[0]**2
 
         if self.mott_bethe:
             dll_dab *= self.hkldata.d_spacings()**2 * gemmi.mott_bethe_const()
             d2ll_dab2 *= gemmi.mott_bethe_const()**2
 
         # we need V for Hessian and V**2/n for gradient.
         d2ll_dab2 *= self.hkldata.cell.volume
         dll_dab_den = self.hkldata.fft_map(data=dll_dab * self.hkldata.debye_waller_factors(b_iso=-blur))
         dll_dab_den.array[:] *= self.hkldata.cell.volume**2 / dll_dab_den.point_count
         #asu = dll_dab_den.masked_asu()
         #dll_dab_den.array[:] *= 1 - asu.mask_array # 0 to use
         
         self.ll = ext.LL(self.st, self.mott_bethe, refine_xyz, adp_mode, refine_h)
         self.ll.set_ncs([x.tr for x in self.st.ncs if not x.given])
-        self.ll.calc_grad_it92(dll_dab_den, blur)
+        if self.source == "neutron":
+            self.ll.calc_grad_n92(dll_dab_den, blur)
+        else:
+            self.ll.calc_grad_it92(dll_dab_den, blur)
 
         # second derivative
         d2dfw_table = ext.TableS3(*self.hkldata.d_min_max())
         valid_sel = numpy.isfinite(d2ll_dab2)
         d2dfw_table.make_table(1./self.hkldata.d_spacings().to_numpy()[valid_sel], d2ll_dab2[valid_sel])
-        self.ll.make_fisher_table_diag_fast_it92(d2dfw_table)
-        self.ll.fisher_diag_from_table_it92()
+        if self.source == "neutron":
+            self.ll.make_fisher_table_diag_fast_n92(d2dfw_table)
+            self.ll.fisher_diag_from_table_n92()
+        else:
+            self.ll.make_fisher_table_diag_fast_it92(d2dfw_table)
+            self.ll.fisher_diag_from_table_it92()
         #json.dump(dict(b=ll.table_bs, pp1=ll.pp1, bb=ll.bb),
         #          open("ll_fisher.json", "w"), indent=True)
         #a, (b,c) = ll.fisher_for_coo()
         #json.dump(([float(x) for x in a], ([int(x) for x in b], [int(x) for x in c])), open("fisher.json", "w"))
 
         self.ll.spec_correction(specs)
```

### Comparing `servalcat-0.4.15/servalcat/refmac/exte.py` & `servalcat-0.4.24/servalcat/refmac/exte.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/refmac/refmac_keywords.py` & `servalcat-0.4.24/servalcat/refmac/refmac_keywords.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,15 +472,21 @@
         pass # TODO
     elif s[0].lower().startswith("plan") and ntok > 1:
         ret["wplane"] = float(s[1])
     elif s[0].lower().startswith("chir") and ntok > 1:
         ret["wchir"] = float(s[1])
         # TODO read calp
     elif s[0].lower().startswith(("vdwr", "vand", "nonb")) and ntok > 1:
-        ret["wvdw"] = float(s[1])
+        itk = 1
+        try:
+            ret["wvdw"] = float(s[itk])
+            itk += 1
+        except ValueError:
+            pass
+        # TODO read maxr, over, sigm, incr, chan, vdwc, excl
 # parse_line()
 
 def get_lines(lines):
     ret = []
     cont = ""
     for l in lines:
         if "!" in l: l = l[:l.index("!")]
```

### Comparing `servalcat-0.4.15/servalcat/refmac/refmac_wrapper.py` & `servalcat-0.4.24/servalcat/refmac/refmac_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,21 +63,15 @@
 
 def prepare_crd(st, crdout, ligand, make, monlib_path=None, h_pos="elec",
                 no_adjust_hydrogen_distances=False):
     assert h_pos in ("elec", "nucl")
     h_change = dict(a=gemmi.HydrogenChange.ReAddButWater,
                     y=gemmi.HydrogenChange.NoChange,
                     n=gemmi.HydrogenChange.Remove)[make.get("hydr", "a")]
-    # we do not have DOD. will not change ND4->NH4 and SPW->SPK, as hydrogen atom names are different
-    for chain in st[0]:
-        for res in chain:
-            if res.name == "DOD":
-                logger.writeln("Warning: changing DOD to HOH (chain {} residue {})".format(chain.name, res.seqid))
-                res.name = "HOH"
-
+    utils.model.fix_deuterium_residues(st)
     gemmi.setup_for_crd(st)
 
     # TODO read dictionary from xyzin (priority: user cif -> monlib -> xyzin
     try:
         monlib = utils.restraints.load_monomer_library(st,
                                                        monomer_dir=monlib_path,
                                                        cif_files=ligand,
@@ -100,17 +94,17 @@
         refmac_fixes = utils.refmac.FixForRefmac(st, topo, 
                                                  fix_microheterogeneity=False,
                                                  fix_resimax=True,
                                                  fix_nonpolymer=False)
 
     if make.get("hydr") == "a": logger.writeln("(re)generating hydrogen atoms")
     try:
-        topo = utils.restraints.prepare_topology(st, monlib, h_change=h_change, ignore_unknown_links=False,
-                                                 check_hydrogen=(h_change==gemmi.HydrogenChange.NoChange),
-                                                 use_cispeps=use_cispeps)
+        topo, metal_kws = utils.restraints.prepare_topology(st, monlib, h_change=h_change, ignore_unknown_links=False,
+                                                            check_hydrogen=(h_change==gemmi.HydrogenChange.NoChange),
+                                                            use_cispeps=use_cispeps)
     except RuntimeError as e:
         raise SystemExit("Error: {}".format(e))
 
     if make.get("hydr") != "n" and st[0].has_hydrogen():
         if h_pos == "nucl" and (make.get("hydr") == "a" or not no_adjust_hydrogen_distances):
             resnames = st[0].get_all_residue_names()
             utils.restraints.check_monlib_support_nucleus_distances(monlib, resnames)
@@ -119,15 +113,15 @@
         elif h_pos == "elec" and make.get("hydr") == "y" and not no_adjust_hydrogen_distances:
             logger.writeln("adjusting hydrogen position to electron cloud")
             topo.adjust_hydrogen_distances(gemmi.Restraints.DistanceOf.ElectronCloud)
 
     doc = gemmi.prepare_refmac_crd(st, topo, monlib, h_change)
     doc.write_file(crdout, style=gemmi.cif.Style.NoBlankLines)
     logger.writeln("crd file written: {}".format(crdout))
-    return refmac_fixes
+    return refmac_fixes, [x+"\n" for x in metal_kws]
 # prepare_crd()
 
 def get_output_model_names(xyzout):
     # ref: WRITE_ATOMS_REFMAC in oppro_allocate.f
     if xyzout is None: xyzout = "XYZOUT"
     pdb, mmcif = "", ""
     if len(xyzout) > 3:
@@ -155,25 +149,29 @@
 def modify_output(pdbout, cifout, fixes, hout, cispeps, keep_original_output=False):
     st = utils.fileio.read_structure(cifout)
     st.cispeps = cispeps
     if os.path.exists(pdbout):
         st.raw_remarks = gemmi.read_pdb(pdbout).raw_remarks
     if fixes is not None:
         fixes.modify_back(st)
+    for con in st.connections:
+        if con.link_id == "disulf":
+            con.type = gemmi.ConnectionType.Disulf
+        # should we check metals and put MetalC?
 
     suffix = ".org"
     os.rename(cifout, cifout + suffix)
     utils.fileio.write_mmcif(st, cifout, cifout + suffix)
     
     chain_id_len_max = max([len(x) for x in utils.model.all_chain_ids(st)])
     seqnums = [res.seqid.num for chain in st[0] for res in chain]
     if chain_id_len_max > 1 or min(seqnums) <= -1000 or max(seqnums) >= 10000:
         logger.writeln("This structure cannot be saved as an official PDB format. Using hybrid-36. Header part may be inaccurate.")
     if hout:
-        st.expand_hd_mixture()
+        st.store_deuterium_as_fraction(False)
     else:
         st.remove_hydrogens() # remove hydrogen from pdb, while kept in mmcif
         
     os.rename(pdbout, pdbout + suffix)
     utils.fileio.write_pdb(st, pdbout)
     if not keep_original_output:
         os.remove(pdbout + suffix)
@@ -184,15 +182,15 @@
     if len(args.opts) % 2 != 0: raise SystemExit("Invalid number of args")
     args.ligand = sum(args.ligand, []) if args.ligand else []
 
     inputs, keywords = read_stdin(sys.stdin) # TODO read psrestin also?
     if not keywords["make"].get("exit"):
         refmac_ver = utils.refmac.check_version(args.exe)
         if not refmac_ver:
-            raise SystemExit("Error: Check Refmac instllation or use --exe to give the location.\n{}".format(e))
+            raise SystemExit("Error: Check Refmac instllation or use --exe to give the location.")
         if refmac_ver < (5, 8, 404):
             raise SystemExit("Error: this version of Refmac is not supported. Update to 5.8.404 or newer")
 
     opts = OrderedDict((args.opts[2*i].lower(), args.opts[2*i+1]) for i in range(len(args.opts)//2))
     xyzin = opts.get("xyzin")
     xyzout = opts.get("xyzout")
     libin = opts.pop("libin", None)
@@ -201,15 +199,19 @@
         # if --monlib is given, it has priority.
         args.monlib = opts.pop("clibd_mon", None)
     for k in ("temp1", "scrref"): # scrref has priority
         if k in opts:
             logger.writeln("updating CCP4_SCR from {}={}".format(k, opts[k]))
             os.environ["CCP4_SCR"] = os.path.dirname(opts[k]) # XXX "." may be given, which causes problem (os.path.isdir("") is False)
     utils.refmac.ensure_ccp4scr()
-    
+    if args.prefix:
+        if "xyzin" in opts and "xyzout" not in opts: opts["xyzout"] = args.prefix + ".pdb"
+        if "hklin" in opts and "hklout" not in opts: opts["hklout"] = args.prefix + ".mtz"
+        if "tlsin" in opts and "tlsout" not in opts: opts["tlsout"] = args.prefix + ".tls"
+        
     # TODO what if restin is given or make cr prepared is given?
     # TODO check make pept/link/suga/ss/conn/symm/chain
 
     # Process model
     crdout = None
     refmac_fixes = None
     cispeps = []
@@ -226,29 +228,27 @@
                 raise SystemExit("Error: unit cell is not defined in the model.")
         if any(not op.given for op in st.ncs):
             logger.writeln("WARNING: Refmac ignores MTRIX (_struct_ncs_oper) records. Add following instructions if you need:")
             logger.writeln("\n".join(utils.symmetry.ncs_ops_for_refmac(st.ncs))+"\n")
             st.ncs.clear()
             st.setup_cell_images()
             # TODO set st.ncs if ncsc instructions given - but should be done outside of this function?
-        crdout = "gemmi_{}_{}.crd".format(utils.fileio.splitext(os.path.basename(xyzin))[0], os.getpid())
-        refmac_fixes = prepare_crd(st, crdout, args.ligand, make=keywords["make"], monlib_path=args.monlib,
-                                   h_pos="nucl" if keywords.get("source")=="ne" else "elec",
-                                   no_adjust_hydrogen_distances=args.no_adjust_hydrogen_distances)
+        xyzout_dir = os.path.dirname(get_output_model_names(opts.get("xyzout"))[0])
+        crdout = os.path.join(xyzout_dir,
+                              "gemmi_{}_{}.crd".format(utils.fileio.splitext(os.path.basename(xyzin))[0], os.getpid()))
+        refmac_fixes, metal_kws = prepare_crd(st, crdout, args.ligand, make=keywords["make"], monlib_path=args.monlib,
+                                              h_pos="nucl" if keywords.get("source")=="ne" else "elec",
+                                              no_adjust_hydrogen_distances=args.no_adjust_hydrogen_distances)
+        inputs = metal_kws + inputs # add metal exte first; otherwise it may be affected by user-defined inputs
         opts["xyzin"] = crdout
         cispeps = st.cispeps
 
     if keywords["make"].get("exit"):
         return
 
-    if args.prefix:
-        if "xyzin" in opts and "xyzout" not in opts: opts["xyzout"] = args.prefix + ".pdb"
-        if "hklin" in opts and "hklout" not in opts: opts["hklout"] = args.prefix + ".mtz"
-        if "tlsin" in opts and "tlsout" not in opts: opts["tlsout"] = args.prefix + ".tls"
-        
     # Run Refmac
     cmd = [args.exe] + list(sum(tuple(opts.items()), ()))
     env = os.environ
     logger.writeln("Running REFMAC5..")
     if args.monlib:
         logger.writeln("CLIBD_MON={}".format(args.monlib))
         env["CLIBD_MON"] = os.path.join(args.monlib, "") # should end with /
@@ -260,14 +260,17 @@
     p.stdin.write("".join(inputs))
     p.stdin.close()
     for l in iter(p.stdout.readline, ""):
         logger.write(l)
     retcode = p.wait()
     logger.writeln("\nRefmac finished with exit code= {}".format(retcode))
 
+    if not args.keep_original_output and crdout and os.path.exists(crdout):
+        os.remove(crdout)
+
     # Modify output
     if xyzin is not None:
         pdbout, cifout = get_output_model_names(opts.get("xyzout"))
         if os.path.exists(cifout):
             modify_output(pdbout, cifout, refmac_fixes, keywords["make"].get("hout"), cispeps, args.keep_original_output)
 # main()
```

### Comparing `servalcat-0.4.15/servalcat/spa/est_local_luzzati_d.py` & `servalcat-0.4.24/servalcat/spa/est_local_luzzati_d.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/spa/estimate_mixture.py` & `servalcat-0.4.24/servalcat/spa/estimate_mixture.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/spa/find_translation.py` & `servalcat-0.4.24/servalcat/spa/find_translation.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/spa/fofc.py` & `servalcat-0.4.24/servalcat/spa/fofc.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 
         if has_fc:
             Fc = hkldata.df.FC.to_numpy()[idxes]
             D = hkldata.binned_df.D[i_bin]
             S = hkldata.binned_df.S[i_bin] # variance of unexplained signal
             w = 1. if no_fsc_weights or not has_halfmaps else S/(S+varn)
             delfwt = w * (Fo-D*Fc)
-            fup = w * Fo + (1.-w)*D*Fc
+            fup = 2 * w * Fo + (1 - 2*w) * D*Fc # <F> + delfwt
             if has_halfmaps: # no point making this map when half maps not given
                 tmp["DELFWT_noscale"][idxes] = delfwt
                 tmp["Fupdate_noscale"][idxes] = fup
 
         if not fsc_became_negative and fsc <= 0:
             logger.writeln(" WARNING: cutting resolution at {:.2f} A because fsc < 0".format(hkldata.binned_df.d_max[i_bin]))
             fsc_became_negative = True
```

### Comparing `servalcat-0.4.15/servalcat/spa/fofc_rms.py` & `servalcat-0.4.24/servalcat/spa/fofc_rms.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/spa/fsc.py` & `servalcat-0.4.24/servalcat/spa/fsc.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/spa/fsc2.py` & `servalcat-0.4.24/servalcat/spa/fsc2.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/spa/localcc.py` & `servalcat-0.4.24/servalcat/spa/localcc.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/spa/realspcc_from_var.py` & `servalcat-0.4.24/servalcat/spa/realspcc_from_var.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/spa/run_refmac.py` & `servalcat-0.4.24/servalcat/spa/run_refmac.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,15 +440,15 @@
 # determine_b_before_mask()
 
 def process_input(st, maps, resolution, monlib, mask_in, args,
                   shifted_model_prefix="shifted",
                   output_masked_prefix="masked_fs",
                   output_mtz_prefix="starting_map",
                   use_gemmi_prep=False, no_refmac_fix=False,
-                  use_refmac=True):
+                  use_refmac=True, fix_link=True):
     ret = {} # instructions for refinement
     maps = utils.maps.copy_maps(maps) # not to modify maps
     
     grid_start = maps[0][1]
     unit_cell = maps[0][0].unit_cell
     spacegroup = gemmi.SpaceGroup(1)
     start_xyz = numpy.array(maps[0][0].get_position(*grid_start).tolist())
@@ -467,39 +467,14 @@
     if use_refmac:
         ret["model_format"] = ".mmcif" if st.input_format == gemmi.CoorFormat.Mmcif else ".pdb"
         max_seq_num = max([max(res.seqid.num for res in chain) for model in st for chain in model])
         if max_seq_num > 9999 and ret["model_format"] == ".pdb":
             logger.writeln("Max residue number ({}) exceeds 9999. Will use mmcif format".format(max_seq_num))
             ret["model_format"] = ".mmcif"
 
-    # workaround for Refmac
-    # TODO need to check external restraints
-    if use_refmac:
-        if use_gemmi_prep:
-            h_change = {"all":gemmi.HydrogenChange.ReAddButWater,
-                        "yes":gemmi.HydrogenChange.NoChange,
-                        "no":gemmi.HydrogenChange.Remove}[args.hydrogen]
-            topo = gemmi.prepare_topology(st, monlib, h_change=h_change, warnings=logger,
-                                          reorder=True, ignore_unknown_links=False)
-        elif not no_refmac_fix:
-            topo = gemmi.prepare_topology(st, monlib, warnings=io.StringIO(), ignore_unknown_links=True)
-        else:
-            topo = None # not used
-        if not no_refmac_fix:
-            ret["refmac_fixes"] = utils.refmac.FixForRefmac(st, topo, 
-                                                            fix_microheterogeneity=not args.no_fix_microheterogeneity and not use_gemmi_prep,
-                                                            fix_resimax=not args.no_fix_resi9999,
-                                                            fix_nonpolymer=False)
-        chain_id_len_max = max([len(x) for x in utils.model.all_chain_ids(st)])
-        if chain_id_len_max > 1 and ret["model_format"] == ".pdb":
-            logger.writeln("Long chain ID (length: {}) detected. Will use mmcif format".format(chain_id_len_max))
-            ret["model_format"] = ".mmcif"
-        if not no_refmac_fix and ret["model_format"] == ".mmcif" and not use_gemmi_prep:
-            ret["refmac_fixes"].fix_nonpolymer(st)
-
     if len(st.ncs) > 0 and args.ignore_symmetry:
         logger.writeln("Removing symmetry information from model.")
         st.ncs.clear()
     utils.symmetry.update_ncs_from_args(args, st, map_and_start=maps[0], filter_contacting=args.contacting_only)
     st_expanded = st.clone()
     if len(st.ncs) > 0:
         if not args.no_check_ncs_overlaps and utils.model.check_symmetry_related_model_duplication(st):
@@ -589,14 +564,44 @@
 
             logger.writeln(" Trimming maps..")
             for i in range(len(maps)): # Update maps
                 suba = maps[i][0].get_subarray(starts, new_shape)
                 new_grid = gemmi.FloatGrid(suba, new_cell, spacegroup)
                 maps[i][0] = new_grid
 
+    st.setup_cell_images()
+    if fix_link:
+        utils.restraints.find_and_fix_links(st, monlib,
+                                            # link via ncsc is not supported as of Refmac5.8.0411
+                                            find_symmetry_related=not use_refmac)
+    # workaround for Refmac
+    # TODO need to check external restraints
+    if use_refmac:
+        if use_gemmi_prep:
+            h_change = {"all":gemmi.HydrogenChange.ReAddButWater,
+                        "yes":gemmi.HydrogenChange.NoChange,
+                        "no":gemmi.HydrogenChange.Remove}[args.hydrogen]
+            topo, metal_kws = utils.restraints.prepare_topology(st, monlib, h_change=h_change, raise_error=False)
+            args.keywords.extend(metal_kws)
+        elif not no_refmac_fix:
+            topo = gemmi.prepare_topology(st, monlib, warnings=io.StringIO(), ignore_unknown_links=True)
+        else:
+            topo = None # not used
+        if not no_refmac_fix:
+            ret["refmac_fixes"] = utils.refmac.FixForRefmac(st, topo, 
+                                                            fix_microheterogeneity=not args.no_fix_microheterogeneity and not use_gemmi_prep,
+                                                            fix_resimax=not args.no_fix_resi9999,
+                                                            fix_nonpolymer=False)
+        chain_id_len_max = max([len(x) for x in utils.model.all_chain_ids(st)])
+        if chain_id_len_max > 1 and ret["model_format"] == ".pdb":
+            logger.writeln("Long chain ID (length: {}) detected. Will use mmcif format".format(chain_id_len_max))
+            ret["model_format"] = ".mmcif"
+        if not no_refmac_fix and ret["model_format"] == ".mmcif" and not use_gemmi_prep:
+            ret["refmac_fixes"].fix_nonpolymer(st)
+
     if use_refmac and use_gemmi_prep:
         # TODO: make cispept, make link, remove unknown link id
         # TODO: cross validation?
         crdout = os.path.splitext(ret["model_file"])[0] + ".crd"
         ret["model_file"] = crdout
         ret["model_format"] = ".mmcif"
         args.keywords.append("make cr prepared")
@@ -735,18 +740,15 @@
 
     try:
         monlib = utils.restraints.load_monomer_library(st, monomer_dir=args.monlib, cif_files=args.ligand, 
                                                        stop_for_unknowns=True)
     except RuntimeError as e:
         raise SystemExit("Error: {}".format(e))
 
-    utils.model.setup_entities(st, clear=True, force_subchain_names=True)
-    if not args.no_link_check:
-        utils.restraints.find_and_fix_links(st, monlib)
-
+    utils.model.setup_entities(st, clear=True, force_subchain_names=True, overwrite_entity_type=True)
     try:
         utils.restraints.prepare_topology(st.clone(), monlib, h_change=gemmi.HydrogenChange.NoChange,
                                           check_hydrogen=(args.hydrogen=="yes"))
     except RuntimeError as e:
         raise SystemExit("Error: {}".format(e))
 
     if args.halfmaps:
@@ -754,19 +756,20 @@
     else:
         maps = [utils.fileio.read_ccp4_map(args.map, pixel_size=args.pixel_size)]
         
     shifted_model_prefix = "shifted"
     _, file_info = process_input(st, maps, resolution=args.resolution - 1e-6, monlib=monlib,
                                  mask_in=args.mask, args=args,
                                  shifted_model_prefix=shifted_model_prefix,
-                                 use_gemmi_prep=use_gemmi_prep)
+                                 use_gemmi_prep=use_gemmi_prep,
+                                 fix_link=not args.no_link_check)
     if args.prepare_only:
         logger.writeln("\n--prepare_only is given. Stopping.")
         return
-        
+
     args.mtz = file_info["mtz_file"]
     if args.halfmaps: # FIXME if no_mask?
         args.mtz_half = [file_info["mtz_file"], file_info["mtz_file"]]
     args.lab_phi = file_info["lab_phi"]  #"Pout0"
     args.lab_f = file_info["lab_f"]
     args.lab_sigf = None
     args.model = file_info["model_file"] # refmac xyzin
@@ -819,15 +822,15 @@
     # Modify output
     st, cif_ref = utils.fileio.read_structure_from_pdb_and_mmcif(refmac_prefix+model_format)
     st.entities.clear()
     st.setup_entities()
 
     if not args.no_trim:
         st.cell = maps[0][0].unit_cell
-    
+        st.setup_cell_images()
     if "refmac_fixes" in file_info:
         file_info["refmac_fixes"].modify_back(st)
     utils.model.adp_analysis(st)
     utils.fileio.write_model(st, prefix=args.output_prefix,
                              pdb=True, cif=True, cif_ref=cif_ref)
 
     # Take care of TLS out
@@ -894,15 +897,15 @@
         
         # Modify output
         st_sr, cif_ref_sr = utils.fileio.read_structure_from_pdb_and_mmcif(refmac_prefix_shaken+model_format)
         st_sr.entities.clear()
         st_sr.setup_entities()
         if not args.no_trim:
             st_sr.cell = maps[0][0].unit_cell
-            
+            st_sr.setup_cell_images()
         if "refmac_fixes" in file_info:
             file_info["refmac_fixes"].modify_back(st_sr)
 
         utils.fileio.write_model(st_sr, prefix=args.output_prefix+"_shaken_refined",
                                  pdb=True, cif=True, cif_ref=cif_ref_sr)
 
         # Expand sym here
```

### Comparing `servalcat-0.4.15/servalcat/spa/shift_maps.py` & `servalcat-0.4.24/servalcat/spa/shift_maps.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     return parser.parse_args(arg_list)
 # parse_args()
 
 def check_maps(map_files, pixel_size=None, disable_cell_check=False):
     logger.writeln("Input map files:")
     params = []
     for f in map_files:
-        g, gs = utils.fileio.read_ccp4_map(f, pixel_size=pixel_size)
+        g, gs, _ = utils.fileio.read_ccp4_map(f, pixel_size=pixel_size)
         params.append((g.unit_cell.parameters, g.shape, g.spacing, gs))
 
     shapes = set([x[1] for x in params])
     if len(shapes) > 1:
         raise RuntimeError("Error: different grid size included")
 
     starts = set([tuple(x[3]) for x in params])
```

### Comparing `servalcat-0.4.15/servalcat/spa/shiftback.py` & `servalcat-0.4.24/servalcat/spa/shiftback.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/spa/translate.py` & `servalcat-0.4.24/servalcat/spa/translate.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/spa/tst_gemmi_mottbethe.py` & `servalcat-0.4.24/servalcat/spa/tst_gemmi_mottbethe.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/spa/tst_refmac_fc.py` & `servalcat-0.4.24/servalcat/spa/tst_refmac_fc.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/test_installation.py` & `servalcat-0.4.24/servalcat/test_installation.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/utils/__init__.py` & `servalcat-0.4.24/servalcat/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/utils/commands.py` & `servalcat-0.4.24/servalcat/utils/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
     # fix_link
     parser = subparsers.add_parser("fix_link", description = 'Fix LINKR/_struct_conn records in the model')
     parser.add_argument('model')
     parser.add_argument('--ligand', nargs="*", action="append")
     parser.add_argument("--monlib",
                         help="Monomer library path. Default: $CLIBD_MON")
-    parser.add_argument('--bond_margin', type=float, default=1.1, help='(default: %(default).1f)')
+    parser.add_argument('--bond_margin', type=float, default=1.3, help='(default: %(default).1f)')
     parser.add_argument('-o','--output', help="Default: input_fixlink.{pdb|mmcif}")
 
     # merge_models
     parser = subparsers.add_parser("merge_models", description = 'Merge multiple model files')
     parser.add_argument('models', nargs="+")
     parser.add_argument('-o','--output', required=True)
 
@@ -157,16 +157,16 @@
     parser = subparsers.add_parser("geom", description = 'Calculate geometry and show outliers')
     parser.add_argument('model')
     parser.add_argument('--ligand', nargs="*", action="append")
     parser.add_argument("--monlib",
                         help="Monomer library path. Default: $CLIBD_MON")
     parser.add_argument('--sigma', type=float, default=5,
                         help="sigma cutoff to print outliers (default: %(default).1f)")
-    #parser.add_argument('--write_z_per_atom', nargs="*", 
-    #                    help="write model file(s) with sum of z values of specified metric as B values")
+    parser.add_argument('--per_atom_score_as_b', action='store_true',
+                        help="write model file with per-atom score as B values")
     parser.add_argument("--check_skew", action='store_true', help="(experimental) check bond skew to test magnification")
     parser.add_argument("--ignore_h", action='store_true', help="ignore hydrogen")
     parser.add_argument('-o', '--output_prefix', 
                         help="default: taken from input file")
 
     # power
     parser = subparsers.add_parser("power", description = 'Show power spectrum')
@@ -237,14 +237,20 @@
     parser.add_argument("--normalize", action='store_true',
                         help="Normalize map values using mean and sd within the mask")
     parser.add_argument("--trim", action='store_true', help="Write trimmed map")
     parser.add_argument('--mask_cutoff', type=float, default=0.5,
                         help="cutoff value for normalization and trimming (default: %(default)s)")
     parser.add_argument('-o', '--output_prefix')
 
+    # map2mtz
+    parser = subparsers.add_parser("map2mtz", description = 'FFT map and write an mtz')
+    parser.add_argument("--map", required=True)
+    parser.add_argument("-d", '--resolution', type=float)
+    parser.add_argument('-o', '--output')
+
     # sm2mm
     parser = subparsers.add_parser("sm2mm", description = 'Small molecule files (cif/hkl/res/ins) to macromolecules (pdb/mmcif/mtz)')
     parser.add_argument('files', nargs='+', help='Cif/ins/res/hkl files')
     parser.add_argument('-o', '--output_prefix')
 
 # add_arguments()
 
@@ -438,14 +444,15 @@
         args.output = tmp + "_h" + model_format
     logger.writeln("Output file: {}".format(args.output))
         
     args.ligand = sum(args.ligand, []) if args.ligand else []
     monlib = restraints.load_monomer_library(st,
                                              monomer_dir=args.monlib,
                                              cif_files=args.ligand)
+    model.setup_entities(st, clear=True, force_subchain_names=True, overwrite_entity_type=True)
     try:
         restraints.add_hydrogens(st, monlib, args.pos)
     except RuntimeError as e:
         raise SystemExit("Error: {}".format(e))
 
     fileio.write_model(st, file_name=args.output)
 # h_add()
@@ -682,14 +689,15 @@
         args.output = tmp + "_fixlink" + model_format
     logger.writeln("Output file: {}".format(args.output))
         
     args.ligand = sum(args.ligand, []) if args.ligand else []
     monlib = restraints.load_monomer_library(st,
                                              monomer_dir=args.monlib,
                                              cif_files=args.ligand)
+    model.setup_entities(st, clear=True, force_subchain_names=True, overwrite_entity_type=True)
     restraints.find_and_fix_links(st, monlib, bond_margin=args.bond_margin)
     fileio.write_model(st, file_name=args.output)
 # fix_link()
     
 def merge_models(args):
     logger.writeln("Reading file   1: {}".format(args.models[0]))
     st = fileio.read_structure(args.models[0])
@@ -721,23 +729,23 @@
         st.remove_hydrogens()
     try:
         monlib = restraints.load_monomer_library(st, monomer_dir=args.monlib, cif_files=args.ligand, 
                                                  stop_for_unknowns=True)
     except RuntimeError as e:
         raise SystemExit("Error: {}".format(e))
 
-    model.setup_entities(st, clear=True, force_subchain_names=True)
+    model.setup_entities(st, clear=True, force_subchain_names=True, overwrite_entity_type=True)
     restraints.find_and_fix_links(st, monlib)
     try:
-        topo = restraints.prepare_topology(st, monlib, h_change=gemmi.HydrogenChange.NoChange,
-                                           check_hydrogen=True)
+        topo, metal_keywords = restraints.prepare_topology(st, monlib, h_change=gemmi.HydrogenChange.NoChange,
+                                                           check_hydrogen=True)
     except RuntimeError as e:
         raise SystemExit("Error: {}".format(e))
     
-    geom = Geom(st, topo, monlib)
+    geom = Geom(st, topo, monlib, refmac_keywords=metal_keywords)
     for k in geom.outlier_sigmas: geom.outlier_sigmas[k] = args.sigma
     geom.geom.setup_nonbonded()
     ret = geom.show_model_stats()
     
     with open(args.output_prefix + "_summary.json", "w") as ofs:
         ret["summary"].to_json(ofs, indent=2)
         logger.writeln("saved: {}".format(ofs.name))
@@ -746,15 +754,15 @@
             ret["outliers"][k] = ret["outliers"][k].to_dict(orient="records")
         json.dump(ret["outliers"], ofs, indent=2)
         logger.writeln("saved: {}".format(ofs.name))
 
     if args.check_skew:
         logger.writeln("\nChecking skewness of bond length deviation")
         # better to ignore hydrogen
-        tab = geom.geom.reporting.get_bond_outliers(use_nucleus=False, min_z=0)
+        tab = geom.geom.reporting.get_bond_outliers(use_nucleus=geom.use_nucleus, min_z=0)
         for a in "atom1", "atom2":
             tab[a] = [str(geom.lookup[x]) for x in tab[a]]
         df = pandas.DataFrame(tab)
         df["dev"] = df["value"] - df["ideal"]
         df = df.reindex(df.dev.abs().sort_values(ascending=False).index)
         logger.writeln("Bond length deviations:")
         logger.writeln(df.to_string(max_rows=20))
@@ -790,14 +798,22 @@
   target = document.getElementById('hist');
   Plotly.newPlot(target, [trace], layout);
  </script>
 </body>
 </html>
 """ % (str(list(df.dev)), q2, sk2))
             logger.writeln("check histogram: {}".format(ofs.name))
+
+    # Note that this modifies st
+    if args.per_atom_score_as_b:
+        model_format = fileio.check_model_format(args.model)
+        peratom = geom.geom.reporting.per_atom_score(len(geom.atoms), geom.use_nucleus, "mean")
+        for i, score in enumerate(peratom["total"]):
+            geom.atoms[i].b_iso = score
+        fileio.write_model(st, file_name="{}_per_atom_score{}".format(args.output_prefix, model_format))
 # geometry()
 
 def show_power(args):
     maps_in = []
     if args.map:
         print(args.map)
         print(sum(args.map, []))
@@ -984,24 +1000,24 @@
         raise SystemExit("ERROR: Unsupported file type: {}".format(args.hklin))
 # blur()
 
 def mask_from_model(args):
     st = fileio.read_structure(args.model) # TODO option to (or not to) expand NCS
     if args.selection:
         gemmi.Selection(args.selection).remove_not_selected(st)
-    gr, grid_start = fileio.read_ccp4_map(args.map)
+    gr, grid_start, _ = fileio.read_ccp4_map(args.map)
     mask = maps.mask_from_model(st, args.radius, soft_edge=args.soft_edge, grid=gr)
     maps.write_ccp4_map(args.output, mask, grid_start=grid_start)
 # mask_from_model()
 
 def applymask(args):
     if args.output_prefix is None:
         args.output_prefix = fileio.splitext(os.path.basename(args.map))[0] + "_masked"
 
-    grid, grid_start = fileio.read_ccp4_map(args.map)
+    grid, grid_start, _ = fileio.read_ccp4_map(args.map)
     mask = fileio.read_ccp4_map(args.mask)[0]
     logger.writeln("Applying mask")
     logger.writeln(" mask min: {:.3f} max: {:.3f}".format(numpy.min(mask), numpy.max(mask)))
     grid.array[:] *= mask.array
 
     if args.normalize:
         masked = grid.array[mask.array>args.mask_cutoff]
@@ -1013,14 +1029,43 @@
 
     maps.write_ccp4_map(args.output_prefix+".mrc", grid,
                         grid_start=grid_start,
                         mask_for_extent=mask.array if args.trim else None,
                         mask_threshold=args.mask_cutoff)
 # applymask()
 
+def map2mtz(args):
+    if args.output is None:
+        args.output = fileio.splitext(os.path.basename(args.map))[0] + "_fft.mtz"
+    grid, grid_start, grid_shape = fileio.read_ccp4_map(args.map)
+    if args.resolution is None:
+        args.resolution = maps.nyquist_resolution(grid)
+        logger.writeln("WARNING: --resolution is not specified. Using Nyquist resolution: {:.2f}".format(args.resolution))
+
+    if grid_start != (0,0,0) or grid.shape != tuple(grid_shape):
+        # If only subregion of whole grid in map, unit cell needs to be re-defined.
+        if grid.shape != tuple(grid_shape):
+            new_abc = [grid.unit_cell.parameters[i] * grid_shape[i] / grid.shape[i] for i in range(3)]
+            cell = gemmi.UnitCell(*new_abc, *grid.unit_cell.parameters[3:])
+            logger.writeln("Changing unit cell to {}".format(cell.parameters))
+        else:
+            cell = grid.unit_cell
+        grid = gemmi.FloatGrid(grid.get_subarray(grid_start, grid_shape),
+                               cell, grid.spacegroup)
+    
+    f_grid = gemmi.transform_map_to_f_phi(grid)
+    asudata = f_grid.prepare_asu_data(dmin=args.resolution, with_000=True)
+    hkldata = hkl.hkldata_from_asu_data(asudata, "F")
+    if grid_start != (0,0,0):
+        shifts = grid.get_position(*grid_start)
+        hkldata.translate("F", shifts)
+        logger.writeln("Applying phase shift with translation {}".format(shifts.tolist()))
+    hkldata.write_mtz(args.output, ["F"])
+# map2mtz()
+
 def sm2mm(args):
     if args.output_prefix is None:
         args.output_prefix = fileio.splitext(args.files[0])[0]
     st, hkldata = fileio.read_small_molecule_files(args.files)
     if st is not None:
         fileio.write_model(st, prefix=args.output_prefix, pdb=True, cif=True)
     if hkldata is not None:
@@ -1061,14 +1106,15 @@
                  geom=geometry,
                  power=show_power,
                  fcalc=fcalc,
                  nemap=nemap,
                  blur=blur,
                  mask_from_model=mask_from_model,
                  applymask=applymask,
+                 map2mtz=map2mtz,
                  sm2mm=sm2mm)
     
     com = args.subcommand
     f = comms.get(com)
     if f:
         return f(args)
     else:
```

### Comparing `servalcat-0.4.15/servalcat/utils/fileio.py` & `servalcat-0.4.24/servalcat/utils/fileio.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,14 +80,15 @@
         groups.ncs = True
         groups.atoms = True
         groups.cell = True
         groups.scale = True
         groups.assembly = True
         groups.entity = True
         groups.cis = True
+        groups.conn = True
         # FIXME is this all? 
         try:
             doc = read_cif_safe(cif_ref)
         except Exception as e:
             # Sometimes refmac writes a broken mmcif file..
             logger.error("Error in mmCIF reading: {}".format(e))
             logger.error("  Give up using cif reference.")
@@ -99,22 +100,20 @@
             logger.writeln("  Give up using cif reference.")
             return write_mmcif(st, cif_out)
         block = blocks[0]
         # to remove fract_transf_matrix. maybe we should keep some (like _atom_sites.solution_hydrogens)?
         # we do not want this because cell may be updated
         block.find_mmcif_category("_atom_sites.").erase()
         st_new.update_mmcif_block(block, groups)
-        st_new.info["_entry.id"] = st_new.info["_entry.id"][:78]
+        if "_entry.id" in st_new.info: st_new.info["_entry.id"] = st_new.info["_entry.id"][:78]
         doc.write_file(cif_out, style=gemmi.cif.Style.Aligned)
     else:
         st_new.name = st_new.name[:78] # this will become _entry.id
         if "_entry.id" in st_new.info: st_new.info["_entry.id"] = st_new.info["_entry.id"][:78]
         groups = gemmi.MmcifOutputGroups(True)
-        groups.group_pdb = True
-        groups.cis = True
         doc = gemmi.cif.Document()
         block = doc.add_new_block("new")
         st_new.update_mmcif_block(block, groups)
         doc.write_file(cif_out, style=gemmi.cif.Style.Aligned)
 # write_mmcif()
 
 def write_pdb(st, pdb_out):
@@ -200,15 +199,15 @@
         logger.writeln("Overriding pixel size with {:.6f} {:.6f} {:.6f}".format(*pixel_size))
         orgc = m.grid.unit_cell.parameters
         new_abc = [orgc[i]*pixel_size[i]/voxel_size[i] for i in (0,1,2)]
         m.grid.unit_cell = gemmi.UnitCell(new_abc[0], new_abc[1], new_abc[2],
                                           orgc[3], orgc[4], orgc[5])
         logger.writeln(" New cell= {:.1f} {:.1f} {:.1f} {:.1f} {:.1f} {:.1f}".format(*m.grid.unit_cell.parameters))
 
-    return [m.grid, grid_start] # TODO should return grid_shape so that the same region can be written
+    return [m.grid, grid_start, grid_shape]
 # read_ccp4_map()
 
 def read_halfmaps(files, pixel_size=None, fail=True):
     if fail and len(files) != 2:
         raise SystemExit("Error: Give exactly two files for half maps")
     maps = [read_ccp4_map(f, pixel_size=pixel_size) for f in files]
     if numpy.array_equal(maps[0][0].array, maps[1][0].array):
@@ -305,26 +304,36 @@
     spext = splitext(xyz_in)
     st = None
     if spext[1].lower() in (".pdb", ".ent"):
         logger.writeln("Reading PDB file: {}".format(xyz_in))
         st = gemmi.read_pdb(xyz_in)
     elif spext[1].lower() in (".cif", ".mmcif"):
         doc = read_cif_safe(xyz_in)
-        blocks = list(filter(lambda b: b.find_loop("_atom_site.id"), doc))
-        if len(blocks) > 0:
-            logger.writeln("Reading mmCIF file: {}".format(xyz_in))
-            if len(blocks) > 1:
-                logger.writeln(" WARNING: more than one block having _atom_site found. Will use first one.")
-            st =  gemmi.make_structure_from_block(blocks[0])
-        else:
-            logger.writeln("Reading smCIF file: {}".format(xyz_in))
-            ss = gemmi.read_small_structure(xyz_in)
-            if not ss.sites:
-                raise RuntimeError("No atoms found in cif file.")
-            st = model.cx_to_mx(ss)
+        for block in doc:
+            if block.find_loop("_atom_site.id"):
+                if st is None:
+                    logger.writeln("Reading mmCIF file: {}".format(xyz_in))
+                    st =  gemmi.make_structure_from_block(block)
+                else:
+                    logger.writeln(" WARNING: more than one block having structure found. Will use first one.")
+                    break
+            elif block.find_loop("_atom_site_label"):
+                if st is None:
+                    logger.writeln("Reading smCIF file: {}".format(xyz_in))
+                    ss = gemmi.read_small_structure(xyz_in)
+                    if not ss.sites:
+                        raise RuntimeError("No atoms found in cif file.")
+                    st = model.cx_to_mx(ss)
+                else:
+                    logger.writeln(" WARNING: more than one block having structure found. Will use first one.")
+                    break
+            elif block.find_loop("_chem_comp_atom.x"):
+                if st is None:
+                    logger.writeln("Reading chemical component file: {}".format(xyz_in))
+                    st = gemmi.make_structure_from_chemcomp_block(block)
     elif spext[1].lower() in (".ins", ".res"):
         logger.writeln("Reading SHELX ins/res file: {}".format(xyz_in))
         st = model.cx_to_mx(read_shelx_ins(ins_in=xyz_in)[0])
         st.setup_cell_images()
     else:
         raise RuntimeError("Unsupported file type: {}".format(spext[1]))
     if st is not None:
@@ -433,15 +442,15 @@
         for b in d:
             if b.name not in list_names:
                 doc.add_copied_block(b)
 
     doc.write_file(cif_out, style=gemmi.cif.Style.Aligned)
 # merge_ligand_cif()
 
-def read_shelx_ins(ins_in=None, lines_in=None): # TODO support gz?
+def read_shelx_ins(ins_in=None, lines_in=None, ignore_q_peaks=True): # TODO support gz?
     assert (ins_in, lines_in).count(None) == 1
     ss = gemmi.SmallStructure()
 
     keywords = """
     TITL CELL ZERR LATT SYMM SFAC NEUT DISP UNIT LAUE REM  MORE END  HKLF OMIT SHEL BASF TWIN TWST EXTI SWAT
     ABIN ANSC ANSR MERG LIST SPEC RESI MOVE ANIS AFIX HFIX FRAG FEND EXYZ EADP EQIV CONN PART BIND FREE DFIX
     DANG BUMP SAME SADI CHIV FLAT DELU SIMU RIGU PRIG DEFS ISOR XNPD NCSY SUMP L.S. CGLS BLOC DAMP STIR WGHT
@@ -513,15 +522,15 @@
             site.label = sp[0]
             try:
                 site.element = sfacs[int(sp[1])-1]
             except:
                 logger.error("failed to parse: {}".format(l))
                 continue
 
-            if site.label.startswith("Q"):
+            if site.label.startswith("Q") and ignore_q_peaks:
                 logger.writeln("skip Q peak: {}".format(l))
                 continue
             
             site.fract.fromlist(list(map(float, sp[2:5])))
             if len(sp) > 5:
                 q = abs(float(sp[5]))
                 if q > 10: q = q % 10 # FIXME proper handling
```

### Comparing `servalcat-0.4.15/servalcat/utils/generate_operators.py` & `servalcat-0.4.24/servalcat/utils/generate_operators.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/utils/hkl.py` & `servalcat-0.4.24/servalcat/utils/hkl.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,41 @@
     return df
 
 def hkldata_from_asu_data(asu_data, label):
     df = df_from_asu_data(asu_data, label)
     return HklData(asu_data.unit_cell, asu_data.spacegroup, df)
 # hkldata_from_asu_data()
 
+def mtz_find_data_columns(mtz, require_sigma=True):
+    # for now (+)/(-) (types K/M and L/G) are not supported
+    col_types = {x.label:x.type for x in mtz.columns}
+    ret = {"J": [], "F": []}
+    for col in col_types:
+        typ = col_types[col]
+        if typ in ("J", "F"):
+            ret[typ].append([col])
+            sig = "SIG" + col
+            if col_types.get(sig) == "Q":
+                ret[typ][-1].append(sig)
+            elif require_sigma:
+                ret[typ].pop()
+    return ret
+# mtz_find_data_columns()
+
+def mtz_find_free_columns(mtz):
+    col_types = {x.label:x.type for x in mtz.columns}
+    free_names = ("FREE", "RFREE", "FREER", "FreeR_flag", "R-free-flags", "FreeRflag")
+    ret = []
+    for col in col_types:
+        typ = col_types[col]
+        if typ == "I" and col in free_names:
+            ret.append(col)
+    return ret
+# mtz_find_free_columns()
+
 def hkldata_from_mtz(mtz, labels, newlabels=None, require_types=None):
     assert type(mtz) == gemmi.Mtz
     notfound = set(labels) - set(mtz.column_labels())
     if notfound:
         raise RuntimeError("MTZ coulumns not found: {}".format(" ".join(notfound)))
     col_types = {x.label:x.type for x in mtz.columns}
     if require_types:
@@ -147,21 +174,14 @@
     if min_bins is not None:
         n_bins = max(n_bins, min_bins)
     if max_bins is not None:
         n_bins = min(n_bins, max_bins)
     return n_bins
 # decide_n_bins()
 
-def intensity_symmetry(sg):
-    ops = sg.operations()
-    ops.add_inversion()
-    newsg = gemmi.find_spacegroup_by_ops(ops)
-    return newsg.point_group_hm()
-# intensity_symmetry()
-    
 class HklData:
     def __init__(self, cell, sg, df=None, binned_df=None):
         self.cell = cell
         self.sg = sg
         self.df = df
         self.binned_df = binned_df
         self._bin_and_indices = []
@@ -193,14 +213,18 @@
             sel = (d >= d_min) & (d <= d_max)
             df = self.df[sel].copy()
             binned_df = None # no way to keep it
         
         return HklData(self.cell, self.sg,  df, binned_df)
     # copy()
 
+    def selected(self, sel):
+        df = self.df[sel].copy()
+        return HklData(self.cell, self.sg,  df)
+
     def merge_asu_data(self, asu_data, label, common_only=True):
         if self.df is not None and label in self.df:
             raise Exception("Duplicated label")
         
         df_tmp = df_from_asu_data(asu_data, label)
 
         if self.df is None:
```

### Comparing `servalcat-0.4.15/servalcat/utils/logger.py` & `servalcat-0.4.24/servalcat/utils/logger.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/utils/maps.py` & `servalcat-0.4.24/servalcat/utils/maps.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/utils/model.py` & `servalcat-0.4.24/servalcat/utils/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,38 +79,38 @@
     return ret
 # calc_sum_ab()
 
 def calc_fc_fft(st, d_min, source, mott_bethe=True, monlib=None, blur=None, cutoff=1e-5, rate=1.5,
                 omit_proton=False, omit_h_electron=False, miller_array=None):
     assert source in ("xray", "electron", "neutron")
     if source != "electron": assert not mott_bethe
-    if omit_proton or omit_h_electron:
-        assert mott_bethe
-        if not st[0].has_hydrogen():
-            logger.writeln("WARNING: omit_proton/h_electron requested, but no hydrogen exists!")
-            omit_proton = omit_h_electron = False
-        elif omit_proton and omit_h_electron:
-            logger.writeln("omit_proton and omit_h_electron requested. removing hydrogens")
-            st = st.clone()
-            st.remove_hydrogens()
-            omit_proton = omit_h_electron = False
-    
     if blur is None: blur = determine_blur_for_dencalc(st, d_min/2/rate)
     #blur = max(0, blur) # negative blur may cause non-positive definite in case of anisotropic Bs
     logger.writeln("Setting blur= {:.2f} in density calculation (unblurred later)".format(blur))
-        
-    if mott_bethe and not omit_proton and monlib is not None and st[0].has_hydrogen():
+    topo = None
+    if st[0].has_hydrogen():
         st = st.clone()
-        topo = gemmi.prepare_topology(st, monlib, warnings=logger, ignore_unknown_links=True)
-        resnames = st[0].get_all_residue_names()
-        restraints.check_monlib_support_nucleus_distances(monlib, resnames)
-        # Shift electron positions
-        topo.adjust_hydrogen_distances(gemmi.Restraints.DistanceOf.ElectronCloud)
-    else:
-        topo = None
+        if source == "neutron":
+            # nothing happens if not st.has_d_fraction
+            st.store_deuterium_as_fraction(False)
+        if omit_proton or omit_h_electron:
+            assert mott_bethe
+            if omit_proton and omit_h_electron:
+                logger.writeln("omit_proton and omit_h_electron requested. removing hydrogens")
+                st.remove_hydrogens()
+                omit_proton = omit_h_electron = False
+        if mott_bethe and not omit_proton and monlib is not None:
+            topo = gemmi.prepare_topology(st, monlib, warnings=logger, ignore_unknown_links=True)
+            resnames = st[0].get_all_residue_names()
+            restraints.check_monlib_support_nucleus_distances(monlib, resnames)
+            # Shift electron positions
+            topo.adjust_hydrogen_distances(gemmi.Restraints.DistanceOf.ElectronCloud)
+    elif omit_proton or omit_h_electron:
+        logger.writeln("WARNING: omit_proton/h_electron requested, but no hydrogen exists!")
+        omit_proton = omit_h_electron = False
         
     if source == "xray" or mott_bethe:
         dc = gemmi.DensityCalculatorX()
     elif source == "electron":
         dc = gemmi.DensityCalculatorE()
     elif source == "neutron":
         dc = gemmi.DensityCalculatorN()
@@ -356,17 +356,17 @@
     aa = gemmi.AtomAddress(cra.chain.name,
                            cra.residue.seqid, cra.residue.name,
                            cra.atom.name, cra.atom.altloc)
     aa.res_id.segment = cra.residue.segment
     return aa
 # cra_to_atomaddress()
 
-def find_special_positions(st, special_pos_threshold=0.1, fix_occ=True, fix_pos=True, fix_adp=True):
+def find_special_positions(st, special_pos_threshold=0.2, fix_occ=True, fix_pos=True, fix_adp=True):
     ns = gemmi.NeighborSearch(st[0], st.cell, 3).populate()
-    cs = gemmi.ContactSearch(special_pos_threshold)
+    cs = gemmi.ContactSearch(special_pos_threshold * 2)
     cs.ignore = gemmi.ContactSearch.Ignore.SameAsu
     cs.special_pos_cutoff_sq = 0
     results = cs.find_contacts(ns)
     found = {}
     cra = {}
     for r in results:
         if r.partner1.atom != r.partner2.atom: continue
@@ -744,7 +744,22 @@
         #a.charge = ?
         a.element = site.element
         a.occ = site.occ
         a.pos = site.orth(ss.cell)
         
     return st
 # cx_to_mx()
+
+def fix_deuterium_residues(st):
+    # we do not have DOD. will not change ND4->NH4 and SPW->SPK, as hydrogen atom names are different
+    n_changed = 0
+    for chain in st[0]:
+        for res in chain:
+            if res.name == "DOD":
+                res.name = "HOH"
+                n_changed += 1
+    for con in st.connections:
+        for p in (con.partner1, con.partner2):
+            if p.res_id.name == "DOD":
+                p.res_id.name = "HOH"
+    if n_changed > 0:
+        logger.writeln("Warning: {} DOD residues have been renamed to HOH".format(n_changed))
```

### Comparing `servalcat-0.4.15/servalcat/utils/refmac.py` & `servalcat-0.4.24/servalcat/utils/refmac.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/utils/refmac_params.py` & `servalcat-0.4.24/servalcat/utils/refmac_params.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/utils/restraints.py` & `servalcat-0.4.24/servalcat/utils/restraints.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from servalcat.utils import logger
 import os
 import io
 import gemmi
 import string
 import random
 import numpy
+import json
 
 default_proton_scale = 1.13 # scale of X-proton distance to X-H(e) distance
 
 def decide_new_mod_id(mod_id, mods):
     # Refmac only allows up to 8 characters
     letters = string.digits + string.ascii_lowercase
     if len(mod_id) < 8:
@@ -142,24 +143,62 @@
             logger.writeln("WARNING: ad-hoc restraints will be generated for {}".format(",".join(unknown_cc)))
             logger.writeln("         it is strongly recommended to generate them using AceDRG.")
     
     return monlib
 # load_monomer_library()
 
 def prepare_topology(st, monlib, h_change, ignore_unknown_links=False, raise_error=True, check_hydrogen=False,
-                     use_cispeps=False):
+                     use_cispeps=False, add_metal_restraints=True):
+    if add_metal_restraints:
+        metalc = MetalCoordination(monlib)
+        keywords, todel = metalc.setup_restraints(st)
+        con_bak = []
+        for i in sorted(todel, reverse=True):
+            # temporarily remove connection not to put a bond restraint
+            con = st.connections.pop(i)
+            con_bak.append((i, con))
+            # flag non-hydrogen
+            cra2 = st[0].find_cra(con.partner2, ignore_segment=True)
+            cra2.atom.calc_flag = gemmi.CalcFlag.NoHydrogen
+    else:
+        keywords = []
     # these checks can be done after sorting links
     logger.writeln("Creating restraints..")
     sio = io.StringIO()
     topo = gemmi.prepare_topology(st, monlib, h_change=h_change, warnings=sio, reorder=False,
                                   ignore_unknown_links=ignore_unknown_links, use_cispeps=use_cispeps)
     for l in sio.getvalue().splitlines(): logger.writeln(" " + l)
     unknown_cc = set()
     link_related = set()
     nan_hydr = set()
+
+    # collect info
+    info = {}
+    for cinfo in topo.chain_infos:
+        toadd = info.setdefault(cinfo.chain_ref.name, {})
+        if cinfo.polymer:
+            toadd["polymer"] = (str(cinfo.polymer_type).replace("PolymerType.", ""),
+                                cinfo.res_infos[0].res.seqid,
+                                cinfo.res_infos[-1].res.seqid,
+                                len(cinfo.res_infos))
+        else:
+            l = toadd.setdefault("nonpolymer", [])
+            for ri in cinfo.res_infos:
+                l.append(ri.res.name)
+    logger.writeln("\nChain info:")
+    for chain in info:
+        logger.writeln(" chain {}".format(chain))
+        if "polymer" in info[chain]:
+            logger.writeln("  {}: {}..{} ({} residues)".format(*info[chain]["polymer"]))
+        if "nonpolymer" in info[chain]:
+            n_res = len(info[chain]["nonpolymer"])
+            uniq = set(info[chain]["nonpolymer"])
+            logger.writeln("  ligands: {} ({} residues)".format(" ".join(uniq), n_res))
+    logger.writeln("")
+    
     for cinfo in topo.chain_infos:
         for rinfo in cinfo.res_infos:
             cc_org = monlib.monomers[rinfo.res.name] if rinfo.res.name in monlib.monomers else None
             for ia in reversed(range(len(rinfo.res))):
                 atom = rinfo.res[ia]
                 atom_str = "{}/{} {}/{}".format(cinfo.chain_ref.name, rinfo.res.name, rinfo.res.seqid, atom.name)
                 cc = rinfo.get_final_chemcomp(atom.altloc)
@@ -184,15 +223,18 @@
         if unknown_cc: msgs.append("restraint cif file(s) for {}".format(",".join(unknown_cc)))
         if link_related: msgs.append("proper link cif file(s) for {} or check your model".format(",".join(link_related)))
         raise RuntimeError("Provide {}".format(" and ".join(msgs)))
     if raise_error and nan_hydr:
         raise RuntimeError("Some hydrogen positions became NaN. The geometry of your model may be of low quality. Consider not adding hydrogen")
     if not use_cispeps:
         topo.set_cispeps_in_structure(st)
-    return topo
+    if add_metal_restraints:
+        for i, con in sorted(con_bak):
+            st.connections.insert(i, con)
+    return topo, keywords
 # prepare_topology()
 
 def check_monlib_support_nucleus_distances(monlib, resnames):
     good = True
     nucl_not_found = []
     for resn in resnames:
         if resn not in monlib.monomers:
@@ -213,132 +255,235 @@
     if nucl_not_found:
         logger.writeln("WARNING: nucleus distance is not found for: {}".format(" ".join(nucl_not_found)))
         logger.writeln("         default scale ({}) is used for nucleus distances.".format(default_proton_scale))
     return good
 # check_monlib_support_nucleus_distances()
 
 def find_and_fix_links(st, monlib, bond_margin=1.3, find_metal_links=True, add_found=True, find_symmetry_related=True):
+    metalc = MetalCoordination(monlib)
     """
     Identify link ids for st.connections and find new links
     This is required for correctly recognizing link in gemmi.prepare_topology
     Note that it ignores segment IDs
     FIXME it assumes only one bond exists in a link. It may not be the case in future.
     """
     from servalcat.utils import model
 
     logger.writeln("Checking links defined in the model")
     for con in st.connections:
         if con.type == gemmi.ConnectionType.Hydrog: continue
         cra1, cra2 = st[0].find_cra(con.partner1, ignore_segment=True), st[0].find_cra(con.partner2, ignore_segment=True)
+        if cra1.atom.element.is_metal or cra2.atom.element.is_metal:
+            con.type = gemmi.ConnectionType.MetalC
         if None in (cra1.atom, cra2.atom):
             logger.writeln(" WARNING: atom(s) not found for link: id= {} atom1= {} atom2= {}".format(con.link_id, con.partner1, con.partner2))
             continue
-        if con.asu == gemmi.Asu.Different:
+        if con.asu == gemmi.Asu.Different: # XXX info from metadata may be wrong
             nimage = st.cell.find_nearest_image(cra1.atom.pos, cra2.atom.pos, con.asu)
             image_idx = nimage.sym_idx
             dist = nimage.dist()
         else:
             image_idx = 0
             dist = cra1.atom.pos.dist(cra2.atom.pos)
+        con.reported_distance = dist
         atoms_str = "atom1= {} atom2= {} image= {}".format(cra1, cra2, image_idx)
         if con.link_id:
             link = monlib.get_link(con.link_id)
             inv = False
             if link is None:
                 logger.writeln(" WARNING: link {} not found in the library. Please provide link dictionary.".format(con.link_id))
+                con.link_id = "" # let gemmi find proper link in prepare_topology()
                 continue
             else:
                 match, _, _ = monlib.test_link(link, cra1.residue.name, cra1.atom.name, cra2.residue.name, cra2.atom.name)
                 if not match and monlib.test_link(link, cra2.residue.name, cra2.atom.name, cra1.residue.name, cra1.atom.name)[0]:
                     match = True
                     inv = True
                 if not match:
                     logger.writeln(" WARNING: link id and atoms mismatch: id= {} {}".format(link.id, atoms_str))
                     continue
         else:
             link, inv, _, _ = monlib.match_link(cra1.residue, cra1.atom.name, cra1.atom.altloc,
                                                 cra2.residue, cra2.atom.name, cra2.atom.altloc)
             if link:
                 con.link_id = link.id
+            elif find_metal_links and con.type == gemmi.ConnectionType.MetalC:
+                logger.writeln(" Metal link will be added: {} dist= {:.2f}".format(atoms_str, dist))
+                if cra2.atom.element.is_metal:
+                    inv = True # make metal first
             else:
                 ideal_dist = monlib.find_ideal_distance(cra1, cra2)
                 logger.writeln(" Link unidentified (simple bond will be used): {} dist= {:.2f} ideal= {:.2f}".format(atoms_str,
                                                                                                                      dist,
                                                                                                                      ideal_dist))
                 continue
         if link:
             logger.writeln(" Link confirmed: id= {} {} dist= {:.2f} ideal= {:.2f}".format(link.id,
                                                                                           atoms_str,
                                                                                           dist,
                                                                                           link.rt.bonds[0].value))
-            if inv:
-                con.partner1 = model.cra_to_atomaddress(cra2)
-                con.partner2 = model.cra_to_atomaddress(cra1)
+            if con.link_id == "disulf":
+                con.type = gemmi.ConnectionType.Disulf
+        if inv:
+            con.partner1 = model.cra_to_atomaddress(cra2)
+            con.partner2 = model.cra_to_atomaddress(cra1)
     if len(st.connections) == 0:
         logger.writeln(" no links defined in the model")
 
     logger.writeln("Finding new links (will {} added)".format("be" if add_found else "not be"))
     ns = gemmi.NeighborSearch(st[0], st.cell, 5.).populate()
-    cs = gemmi.ContactSearch(3.1)
+    cs = gemmi.ContactSearch(4.)
     cs.ignore = gemmi.ContactSearch.Ignore.AdjacentResidues # may miss polymer links not contiguous in a chain?
     results = cs.find_contacts(ns)
     onsb = set(gemmi.Element(x) for x in "ONSB")
     n_found = 0
     for r in results:
-        if not find_symmetry_related and r.image_idx != 0: continue
         if st.find_connection_by_cra(r.partner1, r.partner2): continue
         link, inv, _, _ = monlib.match_link(r.partner1.residue, r.partner1.atom.name, r.partner1.atom.altloc,
                                             r.partner2.residue, r.partner2.atom.name, r.partner2.atom.altloc,
                                             (r.dist / 1.4)**2)
+        if link is None and r.partner2.atom.element.is_metal:
+            inv = True # make metal first
         if inv:
             cra1, cra2 = r.partner2, r.partner1
         else:
             cra1, cra2 = r.partner1, r.partner2
+        im = st.cell.find_nearest_pbc_image(cra1.atom.pos, cra2.atom.pos, r.image_idx)
+        #assert r.image_idx == im.sym_idx # should we check this?
+        if not find_symmetry_related and not im.same_asu():
+            continue
         atoms_str = "atom1= {} atom2= {} image= {}".format(cra1, cra2, r.image_idx)
+        if im.pbc_shift != (0,0,0):
+            atoms_str += " ({},{},{})".format(*im.pbc_shift)
         if link:
             if r.dist > link.rt.bonds[0].value * bond_margin: continue
             logger.writeln(" New link found: id= {} {} dist= {:.2f} ideal= {:.2f}".format(link.id,
                                                                                           atoms_str,
                                                                                           r.dist,
                                                                                           link.rt.bonds[0].value))
         elif find_metal_links:
             # link only metal - O/N/S/B
             if r.partner1.atom.element.is_metal == r.partner2.atom.element.is_metal: continue
-            if not r.partner1.atom.element in onsb and not r.partner2.atom.element in onsb: continue
-            ideal_dist = monlib.find_ideal_distance(r.partner1, r.partner2)
-            if r.dist > ideal_dist * bond_margin: continue
-            logger.writeln(" Metal link found: {} dist= {:.2f} ideal= {:.2f}".format(atoms_str,
-                                                                                     r.dist, ideal_dist))
+            if not cra2.atom.element in onsb: continue
+            max_ideal = metalc.find_max_dist(cra1, cra2)
+            if r.dist > max_ideal * 1.1: continue # tolerance should be smaller than that for other links
+            logger.writeln(" Metal link found: {} dist= {:.2f} max_ideal= {:.2f}".format(atoms_str,
+                                                                                         r.dist, max_ideal))
         n_found += 1
         if not add_found: continue
         con = gemmi.Connection()
         con.name = "added{}".format(n_found)
         if link:
             con.link_id = link.id
-            con.type = gemmi.ConnectionType.Covale
+            con.type = gemmi.ConnectionType.Disulf if link.id == "disulf" else gemmi.ConnectionType.Covale
         else:
             con.type = gemmi.ConnectionType.MetalC
-        con.asu = gemmi.Asu.Same if r.image_idx == 0 else gemmi.Asu.Different
+        con.asu = gemmi.Asu.Same if im.same_asu() else gemmi.Asu.Different
         con.partner1 = model.cra_to_atomaddress(cra1)
         con.partner2 = model.cra_to_atomaddress(cra2)
         con.reported_distance = r.dist
         st.connections.append(con)
     if n_found == 0:
         logger.writeln(" no links found")
 # find_and_fix_links()
 
 def add_hydrogens(st, monlib, pos="elec"):
     assert pos in ("elec", "nucl")
-    # perhaps this should be done outside..
-    st.entities.clear()
-    st.setup_entities()
-
     topo = prepare_topology(st, monlib, h_change=gemmi.HydrogenChange.ReAddButWater, ignore_unknown_links=True)
     
     if pos == "nucl":
         logger.writeln("Generating hydrogens at nucleus positions")
         resnames = st[0].get_all_residue_names()
         check_monlib_support_nucleus_distances(monlib, resnames)
         topo.adjust_hydrogen_distances(gemmi.Restraints.DistanceOf.Nucleus, default_scale=default_proton_scale)
     else:
         logger.writeln("Generating hydrogens at electron positions")
 # add_hydrogens()
+
+def make_atom_spec(cra):
+    chain = cra.chain.name
+    resi = cra.residue.seqid.num
+    ins = cra.residue.seqid.icode
+    atom = cra.atom.name
+    s = "chain {} resi {} ins {} atom {}".format(chain, resi, ins if ins.strip() else ".", atom)
+    if cra.atom.altloc != "\0":
+        s += " alt {}".format(cra.atom.altloc)
+    return s
+# make_atom_spec()        
+
+class MetalCoordination:
+    def __init__(self, monlib, dbfile=None):
+        self.monlib = monlib
+        if dbfile is None:
+            dbfile = os.path.join(monlib.path(), "metals.json")
+        if os.path.exists(dbfile):
+            self.metals = json.load(open(dbfile))["metal_coordination"]
+        else:
+            self.metals = {}
+            logger.writeln("WARNING: {} not found".format(dbfile))
+    # __init__()
+
+    def find_max_dist(self, cra_metal, cra_ligand):
+        vals = self.find_ideal_distances(cra_metal.atom.element, cra_ligand.atom.element)
+        if len(vals) == 0:
+            # if not found
+            return self.monlib.find_ideal_distance(cra_metal, cra_ligand)
+        return max(x["median"] for x in vals)
+    # find_max_dist()
+
+    def find_ideal_distances(self, el_metal, el_ligand):
+        ideals = {}
+        if el_metal.name not in self.metals or el_ligand.name not in self.metals[el_metal.name]:
+            return []
+        return self.metals[el_metal.name][el_ligand.name]
+    # find_ideal_distances
+    
+    def setup_restraints(self, st):
+        ret = [] # returns Refmac keywords
+        lookup = {x.atom: x for x in st[0].all()}
+        coords = {}
+        todel = []
+        for i, con in enumerate(st.connections):
+            if con.link_id == "" and con.type == gemmi.ConnectionType.MetalC:
+                cra1 = st[0].find_cra(con.partner1, ignore_segment=True)
+                cra2 = st[0].find_cra(con.partner2, ignore_segment=True)
+                if None in (cra1.atom, cra2.atom): continue
+                coords.setdefault(cra1.atom.element, {}).setdefault(cra1.atom, []).append((cra2.atom, i))
+        if coords:
+            logger.writeln("Metal coordinations detected")
+        for metal in coords:
+            logger.writeln(" Metal: {}".format(metal.name))
+            ligand_els = {x[0].element for m in coords[metal] for x in coords[metal][m]}
+            logger.writeln("  ideal distances")
+            ideals = {}
+            for el in ligand_els:
+                logger.write("   {}: ".format(el.name))
+                vals = self.find_ideal_distances(metal, el)
+                if len(vals) == 0:
+                    logger.writeln(" uknown (values from ener_lib will be used)")
+                else:
+                    logger.writeln(" ".join("{:.4f} ({} coord)".format(x["median"], x["coord"]) for x in vals))
+                    ideals[el] = [(x["median"], x["mad"]) for x in vals if x["mad"] > 0]
+            logger.writeln("")
+            for i, am in enumerate(coords[metal]):
+                logger.writeln("  site {}: {}".format(i+1, lookup[am]))
+                for j, (lig, con_idx) in enumerate(coords[metal][am]):
+                    con = st.connections[con_idx]
+                    logger.writeln("    ligand {}: {} dist= {:.2f}".format(j+1, lookup[lig],
+                                                                           con.reported_distance))
+                    specs = [make_atom_spec(x) for x in (lookup[am], lookup[lig])]
+                    if lig.element not in ideals:
+                        continue
+                    todel.append(con_idx)
+                    for k, (ideal, sigma) in enumerate(ideals[lig.element]):
+                        exte_str  = "exte dist first {} seco {} ".format(*specs)
+                        exte_str += "valu {:.4f} sigm {:.4f} type 1 ".format(ideal, sigma)
+                        if con.asu == gemmi.Asu.Different:
+                            exte_str += "symm y"
+                        ret.append(exte_str)
+                        #b = ext.Geometry.Bond(am, lig)
+                        #b.values.append(ext.Geometry.Bond.Value(ideal, sigma, ideal, sigma))
+                        #b.type = 0 if k == 0 else 1
+                        #ret.append(b)
+                logger.writeln("")
+        return ret, list(set(todel))
+    # setup_restraints()
```

### Comparing `servalcat-0.4.15/servalcat/utils/scaling.py` & `servalcat-0.4.24/servalcat/utils/scaling.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/utils/symmetry.py` & `servalcat-0.4.24/servalcat/utils/symmetry.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/xtal/french_wilson.py` & `servalcat-0.4.24/servalcat/xtal/french_wilson.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #import atexit
 #atexit.register(profile.print_stats)
 
 def add_arguments(parser):
     parser.description = 'Convert intensity to amplitude'
     parser.add_argument('--hklin', required=True,
                         help='Input MTZ file')
-    parser.add_argument('--labin', required=True,
+    parser.add_argument('--labin', 
                         help='MTZ column for I,SIGI')
     parser.add_argument('--d_min', type=float)
     parser.add_argument('--d_max', type=float)
     parser.add_argument('--nbins', type=int,
                         help="Number of bins (default: auto)")
     parser.add_argument('-o','--output_prefix',
                         help='output file name prefix')
@@ -181,41 +181,57 @@
         S = hkldata.binned_df.S[i_bin]
         c = hkldata.df.centric.to_numpy()[idxes] + 1 # 1 for acentric, 2 for centric
         Io = hkldata.df.I.to_numpy()[idxes]
         sigo = hkldata.df.SIGI.to_numpy()[idxes]
         eps = hkldata.df.epsilon.to_numpy()[idxes]
         to = Io / sigo - sigo / c / k_ani[idxes]**2 / S / eps
         k_num = numpy.where(c == 1,  0.5, 0.)
-        F = numpy.sqrt(sigo) * ext.integ_J_ratio(k_num, k_num - 0.5, False, to, 0., 0., c)
-        Fsq = sigo * ext.integ_J_ratio(k_num + 0.5, k_num - 0.5, False, to, 0., 0., c)
+        F = numpy.sqrt(sigo) * ext.integ_J_ratio(k_num, k_num - 0.5, False, to, 0., 1., c)
+        Fsq = sigo * ext.integ_J_ratio(k_num + 0.5, k_num - 0.5, False, to, 0., 1., c)
         varF = Fsq - F**2
         hkldata.df.loc[idxes, labout[0]] = F
         hkldata.df.loc[idxes, labout[1]] = numpy.sqrt(varF)
         hkldata.df.loc[idxes, "to1"] = to
 
 def main(args):
     if not args.output_prefix:
         args.output_prefix = utils.fileio.splitext(os.path.basename(args.hklin))[0] + "_fw"
-
+    if not args.labin:
+        mtz = utils.fileio.read_mmhkl(args.hklin)
+        dlabs = utils.hkl.mtz_find_data_columns(mtz)
+        if dlabs["J"]:
+            labin = dlabs["J"][0]
+        else:
+            raise SystemExit("Intensity not found from mtz")
+        flabs = utils.hkl.mtz_find_free_columns(mtz)
+        if flabs:
+            labin += [flabs[0]]
+        logger.writeln("MTZ columns automatically selected: {}".format(labin))
+    else:
+        labin = args.labin.split(",")
+        
     hkldata, _, _, _ = process_input(hklin=args.hklin,
-                                     labin=args.labin.split(","),
+                                     labin=labin,
                                      n_bins=args.nbins,
                                      free=None,
                                      xyzins=[],
                                      source=None,
                                      d_min=args.d_min,
                                      n_per_bin=500,
                                      max_bins=30)
     
     B_aniso = determine_Sigma_and_aniso(hkldata)
     french_wilson(hkldata, B_aniso)
-
     mtz_out = args.output_prefix+".mtz"
-    hkldata.write_mtz(mtz_out, labs=["F","SIGF","I","SIGI"],
-                      types={"F":"F", "SIGF":"Q", "I":"J", "SIGI":"Q"})
+    lab_out = ["F", "SIGF", "I", "SIGI"]
+    labo_types = {"F":"F", "SIGF":"Q", "I":"J", "SIGI":"Q"}
+    if len(labin) == 3:
+        lab_out.append("FREE")
+        labo_types[lab_out[-1]] = "I"
+    hkldata.write_mtz(mtz_out, lab_out, types=labo_types)
     return B_aniso, hkldata
 # main()
 
 if __name__ == "__main__":
     import sys
     args = parse_args(sys.argv[1:])
     main(args)
```

### Comparing `servalcat-0.4.15/servalcat/xtal/run_refmac_small.py` & `servalcat-0.4.24/servalcat/xtal/run_refmac_small.py`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/servalcat/xtal/sigmaa.py` & `servalcat-0.4.24/servalcat/xtal/sigmaa.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 from __future__ import absolute_import, division, print_function, generators
 import argparse
 import gemmi
 import numpy
 import pandas
 import itertools
+import time
 import scipy.special
 import scipy.optimize
 from servalcat.utils import logger
 from servalcat import utils
 from servalcat import ext
 
 """
@@ -32,20 +33,20 @@
                         help='flag number for test set')
     parser.add_argument('--model', required=True, nargs="+", action="append",
                         help='Input atomic model file(s)')
     parser.add_argument("-d", '--d_min', type=float)
     #parser.add_argument('--d_max', type=float)
     parser.add_argument('--nbins', type=int,
                         help="Number of bins (default: auto)")
-    parser.add_argument('-s', '--source', choices=["electron", "xray", "neutron"], default="xray",
-                        help="Scattering factor choice (default: %(default)s)")
-    parser.add_argument('--D_as_exp',  action='store_true',
-                        help="estimate D through exp(x) as a positivity constraint")
-    parser.add_argument('--S_as_exp',  action='store_true',
-                        help="estimate variance of unexplained signal through exp(x) as a positivity constraint")
+    parser.add_argument('-s', '--source', choices=["electron", "xray", "neutron"], required=True,
+                        help="Scattering factor choice")
+    parser.add_argument('--D_trans', choices=["exp", "splus"],
+                        help="estimate D with positivity constraint")
+    parser.add_argument('--S_trans', choices=["exp", "splus"],
+                        help="estimate variance of unexplained signal with positivity constraint")
     parser.add_argument('--no_solvent',  action='store_true',
                         help="Do not consider bulk solvent contribution")
     parser.add_argument('--use_cc',  action='store_true',
                         help="Use CC(|F1|,|F2|) to CC(F1,F2) conversion to derive D and S")
     parser.add_argument('--use', choices=["all", "work", "test"], default="all",
                         help="Which reflections to be used for the parameter estimate.")
     parser.add_argument('-o','--output_prefix', default="sigmaa",
@@ -55,54 +56,62 @@
 def parse_args(arg_list):
     parser = argparse.ArgumentParser()
     add_arguments(parser)
     return parser.parse_args(arg_list)
 # parse_args()
 
 class VarTrans:
-    def __init__(self, D_as_exp, S_as_exp):
-        if D_as_exp:
-            self.D = numpy.exp # D = D(x)
-            self.D_deriv = numpy.exp # dD/dx
-            self.D_inv = numpy.log # x = D_inv(D)
-        else:
-            self.D = lambda x: x
-            self.D_deriv = lambda x: 1
-            self.D_inv = lambda x: x
-
-        if S_as_exp:
-            self.S = numpy.exp
-            self.S_deriv = numpy.exp
-            self.S_inv = numpy.log
-        else:
-            self.S = lambda x: x
-            self.S_deriv = lambda x: 1
-            self.S_inv = lambda x: x
+    def __init__(self, D_trans, S_trans):
+        # splus (softplus) appears to be better than exp
+        # exp sometimes results in too large parameter value
+        trans_funcs = {"exp": (numpy.exp, # D = f(x)
+                               numpy.exp, # dD/dx
+                               numpy.log), # x = f^-1(D)
+                       "splus": (lambda x: numpy.logaddexp(0, x),
+                                 scipy.special.expit, # lambda x: 1. / (1. + numpy.exp(-x))
+                                 lambda x: x + numpy.log(-numpy.expm1(-x))),
+                       None: (lambda x: x,
+                              lambda x: 1,
+                              lambda x: x)}
+        
+        self.D, self.D_deriv, self.D_inv = trans_funcs[D_trans]
+        self.S, self.S_deriv, self.S_inv = trans_funcs[S_trans]
 # class VarTrans
 
 class LsqScale:
     # parameter x = [k_overall, adp_pars, k_sol, B_sol]
-    def __init__(self, hkldata, obs, fc_list, use_int=False, k_as_exp=False):
+    def __init__(self, hkldata, fc_list, use_int=False, k_as_exp=False, sigma_cutoff=None):
         assert 0 < len(fc_list) < 3
         self.use_int = use_int
-        self.obs = obs
-        self.calc = fc_list
-        self.s2mat = hkldata.ssq_mat()
-        self.s2 = 1. / hkldata.d_spacings().to_numpy()**2
+        if sigma_cutoff is not None:
+            if use_int:
+                sel = hkldata.df.I / hkldata.df.SIGI > sigma_cutoff
+                self.labcut = "(I/SIGI>{})".format(sigma_cutoff)
+            else:
+                sel = hkldata.df.FP / hkldata.df.SIGFP > sigma_cutoff
+                self.labcut = "(F/SIGF>{})".format(sigma_cutoff)
+        else:
+            sel = hkldata.df.index
+            self.labcut = ""
+        self.obs = hkldata.df["I" if use_int else "FP"].to_numpy()[sel]
+        self.calc = [x[sel] for x in fc_list]
+        self.s2mat = hkldata.ssq_mat()[:,sel]
+        self.s2 = 1. / hkldata.d_spacings().to_numpy()[sel]**2
         self.adpdirs = utils.model.adp_constraints(hkldata.sg.operations(), hkldata.cell, tr0=False)
         self.k_trans = lambda x: numpy.exp(x) if k_as_exp else x
         self.k_trans_der = lambda x: numpy.exp(x) if k_as_exp else 1
         self.k_trans_inv = lambda x: numpy.log(x) if k_as_exp else x
         self.k_sol_ini = 0.35 # same default as gemmi/scaling.hpp
         self.b_sol_ini = 46.
         if use_int:
-            self.sqrt_obs = numpy.sqrt(numpy.maximum(self.obs, 0.1))
+            self.sqrt_obs = numpy.sqrt(numpy.maximum(self.obs, 0))
         
-    def get_solvent_scale(self, k_sol, b_sol):
-        return k_sol * numpy.exp(-b_sol * self.s2 / 4)
+    def get_solvent_scale(self, k_sol, b_sol, s2=None):
+        if s2 is None: s2 = self.s2
+        return k_sol * numpy.exp(-b_sol * s2 / 4)
     
     def scaled_fc(self, x):
         fc0 = self.calc[0]
         if len(self.calc) == 2:
             fmask = self.calc[1]
             fbulk = self.get_solvent_scale(x[-2], x[-1]) * fmask
             fc = fc0 + fbulk
@@ -174,15 +183,15 @@
         H[1,1] = numpy.sum(s2p**2/8)
         H[0,1] = H[1,0] = -numpy.sum(s2p)/2
         x = -numpy.dot(numpy.linalg.inv(H), g)
         if self.use_int: x /= 2
         k = numpy.exp(x[0])
         b = x[1]
         logger.writeln(" initial k,b = {:.2e} {:.2e}".format(k, b))
-        logger.writeln("           R = {:.4f}".format(utils.hkl.r_factor(f1p, f2p * k * numpy.exp(-b*self.s2[sel]/4))))
+        logger.writeln("           R{} = {:.4f}".format(self.labcut, utils.hkl.r_factor(f1p, f2p * k * numpy.exp(-b*self.s2[sel]/4))))
         return k, b
     
     def scale(self):
         use_sol = len(self.calc) == 2
         msg = "Scaling Fc to {} {} bulk solvent contribution".format("Io" if self.use_int else "Fo",
                                                                      "with" if use_sol else "without")
         logger.writeln(msg)
@@ -218,16 +227,16 @@
         logger.writeln(" k_ov= {:.2e} B_iso= {:.2e} B_aniso= {}".format(self.k_overall, self.b_iso, self.b_aniso))
         if use_sol:
             self.k_sol = res.x[-2] 
             self.b_sol = res.x[-1]
             logger.writeln(" k_sol= {:.2e} B_sol= {:.2e}".format(self.k_sol, self.b_sol))
         calc = numpy.abs(self.scaled_fc(res.x))
         if self.use_int: calc *= calc            
-        logger.writeln(" CC = {:.4f}".format(utils.hkl.correlation(self.obs, calc)))
-        logger.writeln(" R  = {:.4f}".format(utils.hkl.r_factor(self.obs, calc)))
+        logger.writeln(" CC{} = {:.4f}".format(self.labcut, utils.hkl.correlation(self.obs, calc)))
+        logger.writeln(" R{}  = {:.4f}".format(self.labcut, utils.hkl.r_factor(self.obs, calc)))
 
 def calc_DFc(Ds, Fcs):
     DFc = sum(Ds[i] * Fcs[i] for i in range(len(Ds)))
     return DFc
 # calc_DFc()
 
 def calc_abs_DFc(Ds, Fcs):
@@ -248,59 +257,61 @@
     for j in range(len(Ds)):
         rsq = numpy.real(Fcs[j] * DFc.conj())
         ret.append((2 * rsq,
                     rsq / DFc_abs))
     return DFc_abs, ret
 # deriv_DFc2_and_DFc_dDj()
 
-def mlf_acentric(Fo, varFo, Fcs, Ds, S, epsilon):
+def mlf_acentric(Fo, varFo, Fcs, Ds, S, epsilon, k_aniso):
     # https://doi.org/10.1107/S0907444911001314
     # eqn (4)
-    Sigma = 2 * varFo + epsilon * S
-    DFc = calc_abs_DFc(Ds, Fcs)
+    Sigma = 2 * varFo + epsilon * S * k_aniso**2
+    DFc = calc_abs_DFc(Ds, Fcs) * k_aniso
     ret = numpy.log(2) + numpy.log(Fo) - numpy.log(Sigma)
     ret += -(Fo**2 + DFc**2)/Sigma
     ret += gemmi.log_bessel_i0(2*Fo*DFc/Sigma)
     return -ret
 # mlf_acentric()
 
-def deriv_mlf_wrt_D_S_acentric(Fo, varFo, Fcs, Ds, S, epsilon):
+def deriv_mlf_wrt_D_S_acentric(Fo, varFo, Fcs, Ds, S, epsilon, k_aniso):
     deriv = numpy.zeros(1+len(Ds))
-    Sigma = 2 * varFo + epsilon * S
+    Sigma = 2 * varFo + epsilon * S * k_aniso**2
     Fo2 = Fo**2
     DFc, tmp = deriv_DFc2_and_DFc_dDj(Ds, Fcs)
+    DFc *= k_aniso
     i1_i0_x = gemmi.bessel_i1_over_i0(2*Fo*DFc/Sigma) # m
-    for i, (sqder, der) in enumerate(tmp):
-        deriv[i] = -numpy.nansum(-sqder / Sigma + i1_i0_x * 2 * Fo * der / Sigma)
-    
-    deriv[-1] = -numpy.nansum((-1/Sigma + (Fo2 + DFc**2 - i1_i0_x * 2 * Fo * DFc) / Sigma**2) * epsilon)
-    return deriv
+    ret = []
+    for sqder, der in tmp:
+        ret.append(-sqder * k_aniso**2 / Sigma + i1_i0_x * 2 * Fo * der * k_aniso / Sigma)
+    ret.append((-1/Sigma + (Fo2 + DFc**2 - i1_i0_x * 2 * Fo * DFc) / Sigma**2) * epsilon * k_aniso**2)
+    return -numpy.vstack(ret).T
 # deriv_mlf_wrt_D_S_acentric()
 
-def mlf_centric(Fo, varFo, Fcs, Ds, S, epsilon):
+def mlf_centric(Fo, varFo, Fcs, Ds, S, epsilon, k_aniso):
     # https://doi.org/10.1107/S0907444911001314
     # eqn (4)
-    Sigma = varFo + epsilon * S
-    DFc = calc_abs_DFc(Ds, Fcs)
+    Sigma = varFo + epsilon * S * k_aniso**2
+    DFc = calc_abs_DFc(Ds, Fcs) * k_aniso
     ret = 0.5 * (numpy.log(2 / numpy.pi) - numpy.log(Sigma))
     ret += -0.5 * (Fo**2 + DFc**2) / Sigma
     ret += gemmi.log_cosh(Fo * DFc / Sigma)
     return -ret
 # mlf_centric()
 
-def deriv_mlf_wrt_D_S_centric(Fo, varFo, Fcs, Ds, S, epsilon):
-    deriv = numpy.zeros(1+len(Ds))
-    Sigma = varFo + epsilon * S
+def deriv_mlf_wrt_D_S_centric(Fo, varFo, Fcs, Ds, S, epsilon, k_aniso):
+    Sigma = varFo + epsilon * S * k_aniso**2
     Fo2 = Fo**2
     DFc, tmp = deriv_DFc2_and_DFc_dDj(Ds, Fcs)
+    DFc *= k_aniso
     tanh_x = numpy.tanh(Fo*DFc/Sigma)
-    for i, (sqder, der) in enumerate(tmp):
-        deriv[i] = -numpy.nansum(-0.5 * sqder / Sigma + tanh_x * Fo * der / Sigma)
-    deriv[-1] = -numpy.nansum((-0.5 / Sigma + (0.5*(Fo2+DFc**2) - tanh_x * Fo*DFc)/Sigma**2)*epsilon)
-    return deriv
+    ret = []
+    for sqder, der in tmp:
+        ret.append(-0.5 * sqder * k_aniso**2 / Sigma + tanh_x * Fo * der * k_aniso / Sigma)
+    ret.append((-0.5 / Sigma + (0.5*(Fo2+DFc**2) - tanh_x * Fo*DFc)/Sigma**2)*epsilon * k_aniso**2)
+    return -numpy.vstack(ret).T
 # deriv_mlf_wrt_D_S_centric()
 
 #import line_profiler
 #profile = line_profiler.LineProfiler()
 #import atexit
 #atexit.register(profile.print_stats)
 #@profile
@@ -309,32 +320,85 @@
     func = (mlf_acentric, mlf_centric)
     for c, work, test in centric_sel:
         if use == "all":
             cidxes = numpy.concatenate([work, test])
         else:
             cidxes = work if use == "work" else test
         Fcs = [df[lab].to_numpy()[cidxes] for lab in fc_labs]
-        ret += numpy.nansum(func[c](df.FP.to_numpy()[cidxes], df.SIGFP.to_numpy()[cidxes]**2, Fcs, Ds, S, df.epsilon.to_numpy()[cidxes]))
+        ret += numpy.nansum(func[c](df.FP.to_numpy()[cidxes], df.SIGFP.to_numpy()[cidxes]**2,
+                                    Fcs, Ds, S, df.epsilon.to_numpy()[cidxes], df.k_aniso.to_numpy()[cidxes]))
     return ret
 # mlf()
 
 #@profile
 def deriv_mlf_wrt_D_S(df, fc_labs, Ds, S, centric_sel, use):
     ret = []
     func = (deriv_mlf_wrt_D_S_acentric, deriv_mlf_wrt_D_S_centric)
     for c, work, test in centric_sel:
         if use == "all":
             cidxes = numpy.concatenate([work, test])
         else:
             cidxes = work if use == "work" else test
         Fcs = [df[lab].to_numpy()[cidxes] for lab in fc_labs]
-        ret.append((func[c](df.FP.to_numpy()[cidxes], df.SIGFP.to_numpy()[cidxes]**2, Fcs, Ds, S, df.epsilon.to_numpy()[cidxes])))
+        r = func[c](df.FP.to_numpy()[cidxes], df.SIGFP.to_numpy()[cidxes]**2,
+                    Fcs, Ds, S, df.epsilon.to_numpy()[cidxes], df.k_aniso.to_numpy()[cidxes])
+        ret.append(numpy.nansum(r, axis=0))
     return sum(ret)
 # deriv_mlf_wrt_D_S()
 
+def mlf_shift_S(df, fc_labs, Ds, S, centric_sel, use):
+    func = (deriv_mlf_wrt_D_S_acentric, deriv_mlf_wrt_D_S_centric)
+    g, H = 0., 0.
+    for c, work, test in centric_sel:
+        if use == "all":
+            cidxes = numpy.concatenate([work, test])
+        else:
+            cidxes = work if use == "work" else test
+        Fcs = [df[lab].to_numpy()[cidxes] for lab in fc_labs]
+        r = func[c](df.FP.to_numpy()[cidxes], df.SIGFP.to_numpy()[cidxes]**2,
+                    Fcs, Ds, S, df.epsilon.to_numpy()[cidxes], df.k_aniso.to_numpy()[cidxes])
+        g += numpy.nansum(r[:,-1])
+        H += numpy.nansum(r[:,-1]**2) # approximating expectation value of second derivative
+    return -g / H
+# mlf_shift_S()
+
+def mli(df, fc_labs, Ds, S, k_ani, idxes):
+    DFc = (Ds * df.loc[idxes, fc_labs]).sum(axis=1)
+    ll = ext.ll_int(df.I[idxes], df.SIGI[idxes], k_ani[idxes], S * df.epsilon[idxes],
+                    numpy.abs(DFc), df.centric[idxes]+1)
+    if numpy.nansum(ll) == -numpy.inf:
+        dbg = numpy.where(ll == -numpy.inf)[0]
+        logger.writeln("debug: -inf params= {}".format([df.I[idxes].to_numpy()[dbg],
+                                                        df.SIGI[idxes].to_numpy()[dbg],
+                                                        k_ani[idxes][dbg],
+                                                        S * df.epsilon[idxes].to_numpy()[dbg],
+                                                        numpy.abs(DFc.to_numpy())[dbg],
+                                                        df.centric[idxes].to_numpy()[dbg]+1]))
+    return numpy.nansum(ll)
+# mli()
+
+def deriv_mli_wrt_D_S(df, fc_labs, Ds, S, k_ani, idxes):
+    r = ext.ll_int_der1_DS(df.I.to_numpy()[idxes], df.SIGI.to_numpy()[idxes], k_ani[idxes], S,
+                           df[fc_labs].to_numpy()[idxes], Ds,
+                           df.centric.to_numpy()[idxes]+1, df.epsilon.to_numpy()[idxes])
+    g = numpy.zeros(len(fc_labs)+1)
+    g[:len(fc_labs)] = numpy.nansum(r[:,:len(fc_labs)], axis=0) # D
+    g[-1] = numpy.nansum(r[:,-1]) # S
+    return g
+# deriv_mli_wrt_D_S()
+
+def mli_shift_S(df, fc_labs, Ds, S, k_ani, idxes):
+    r = ext.ll_int_der1_DS(df.I.to_numpy()[idxes], df.SIGI.to_numpy()[idxes], k_ani[idxes], S,
+                           df[fc_labs].to_numpy()[idxes], Ds,
+                           df.centric.to_numpy()[idxes]+1, df.epsilon.to_numpy()[idxes])
+    g = numpy.nansum(r[:,-1])
+    H = numpy.nansum(r[:,-1]**2) # approximating expectation value of second derivative
+    return -g / H
+# mli_shift_S()
+
 def determine_mlf_params_from_cc(hkldata, fc_labs, D_labs, centric_and_selections, use="all"):
     # theorhetical values
     cc_a = lambda cc: (numpy.pi/4*(1-cc**2)**2 * scipy.special.hyp2f1(3/2, 3/2, 1, cc**2) - numpy.pi/4) / (1-numpy.pi/4)
     cc_c = lambda cc: 2/(numpy.pi-2) * (cc**2*numpy.sqrt(1-cc**2) + cc * numpy.arctan(cc/numpy.sqrt(1-cc**2)) + (1-cc**2)**(3/2)-1)
     table_fsc = numpy.arange(0, 1, 1e-3)
     table_cc = [cc_a(table_fsc), cc_c(table_fsc)]
 
@@ -360,15 +424,15 @@
             cidxes = numpy.concatenate([sel[i] for sel in centric_and_selections[i_bin]])
         valid_sel = numpy.isfinite(hkldata.df.FP.to_numpy()[cidxes])
         cidxes = cidxes[valid_sel]
         factor = inv_sqrt_c_eps[cidxes]
         Fo = hkldata.df.FP.to_numpy()[cidxes] * factor
         mean_Fo2 = numpy.mean(Fo**2)
         SigFo = hkldata.df.SIGFP.to_numpy()[cidxes]
-        Fcs = [hkldata.df[lab].to_numpy()[cidxes] * factor for lab in fc_labs]
+        Fcs = [hkldata.df[lab].to_numpy()[cidxes] * hkldata.df.k_aniso.to_numpy()[cidxes] * factor for lab in fc_labs]
         mean_Fk2 = numpy.array([numpy.mean(numpy.abs(fk)**2) for fk in Fcs])
         
         # estimate D
         cc_fo_fj = [numpy.corrcoef(numpy.abs(fj), Fo)[1,0] for fj in Fcs]
         for i in range(len(fc_labs)): stats.loc[i_bin, "CC(FP,{})".format(fc_labs[i])] = cc_fo_fj[i]
         mat = [[numpy.sqrt(numpy.mean(numpy.abs(fk)**2)/mean_Fo2) * numpy.real(numpy.corrcoef(fk, fj)[1,0])
                 for fk in Fcs]
@@ -409,193 +473,232 @@
 
     logger.writeln("\nCC:")
     logger.writeln(stats.to_string())
     logger.writeln("\nEstimates:")
     logger.writeln(hkldata.binned_df.to_string())
 # determine_mlf_params_from_cc()
 
-def determine_mlf_params(hkldata, fc_labs, D_labs, centric_and_selections, D_as_exp=False, S_as_exp=False, use="all"):
+def determine_ml_params(hkldata, use_int, fc_labs, D_labs, b_aniso, centric_and_selections,
+                        D_trans=None, S_trans=None, use="all", n_cycle=1):
     assert use in ("all", "work", "test")
-    trans = VarTrans(D_as_exp, S_as_exp)
-    
-    # Initial values
-    for lab in D_labs: hkldata.binned_df[lab] = 1.
-    hkldata.binned_df["S"] = 10000.
-    for i_bin, _ in hkldata.binned():
-        if use == "all":
-            idxes = numpy.concatenate([sel[i] for sel in centric_and_selections[i_bin] for i in (1,2)])
-        else:
-            i = 1 if use == "work" else 2
-            idxes = numpy.concatenate([sel[i] for sel in centric_and_selections[i_bin]])
-        valid_sel = numpy.isfinite(hkldata.df.FP[idxes]) # as there is no nan-safe numpy.corrcoef
-        idxes = idxes[valid_sel]
-        FC = numpy.abs(hkldata.df.FC.to_numpy()[idxes])
-        FP = hkldata.df.FP.to_numpy()[idxes]
-        D = numpy.corrcoef(FP, FC)[1,0]
-        hkldata.binned_df.loc[i_bin, D_labs[0]] = D
-        hkldata.binned_df.loc[i_bin, "S"] = numpy.var(FP - D * FC)
-
-    for D_lab in D_labs:
-        if hkldata.binned_df[D_lab].min() <= 0:
-            min_D = hkldata.binned_df[D_lab][hkldata.binned_df[D_lab] > 0].min() * 0.1
-            logger.writeln("WARNING: negative {} is detected from initial estimates. Replacing it using minimum positive value {:.2e}".format(D_lab, min_D))
-            hkldata.binned_df[D_lab].where(hkldata.binned_df[D_lab] > 0, min_D, inplace=True) # arbitrary
-        
-    logger.writeln("Initial estimates:")
-    logger.writeln(hkldata.binned_df.to_string())
-
-    for i_bin, idxes in hkldata.binned():
-        x0 = [trans.D_inv(hkldata.binned_df[lab][i_bin]) for lab in D_labs] + [trans.S_inv(hkldata.binned_df.S[i_bin])]
-        def target(x):
-            return mlf(hkldata.df, fc_labs, trans.D(x[:-1]), trans.S(x[-1]), centric_and_selections[i_bin], use)
-        def grad(x):
-            g = deriv_mlf_wrt_D_S(hkldata.df, fc_labs, trans.D(x[:-1]), trans.S(x[-1]), centric_and_selections[i_bin], use)
-            g[:-1] *= trans.D_deriv(x[:-1])
-            g[-1] *= trans.S_deriv(x[-1])
-            return g
-
-        # test derivative
-        if 0:
-            gana = grad(x0)
-            e = 1e-4
-            for i in range(len(x0)):
-                tmp = x0.copy()
-                f0 = target(tmp)
-                tmp[i] += e
-                fe = target(tmp)
-                gnum = (fe-f0)/e
-                print("DERIV:", i, gnum, gana[i], gana[i]/gnum)
-
-        #print("Bin", i_bin)
-        res = scipy.optimize.minimize(fun=target, x0=x0, jac=grad)
-        #print(res)
-        
-        for i, lab in enumerate(D_labs):
-            hkldata.binned_df.loc[i_bin, lab] = trans.D(res.x[i])
-        hkldata.binned_df.loc[i_bin, "S"] = trans.S(res.x[-1])
-
-    logger.writeln("Refined estimates:")
-    logger.writeln(hkldata.binned_df.to_string())
-    return D_labs
-# determine_mlf_params()
-
-def determine_mli_params(hkldata, fc_labs, D_labs, b_aniso, centric_and_selections,
-                         D_as_exp=False, S_as_exp=False, use="all", n_cycle=1):
-    assert use in ("all", "work", "test")
-    trans = VarTrans(D_as_exp, S_as_exp)
+    logger.writeln("Estimating sigma-A parameters using {}..".format("intensities" if use_int else "amplitudes"))
+    trans = VarTrans(D_trans, S_trans)
+    lab_obs = "I" if use_int else "FP"
     def get_idxes(i_bin):
         if use == "all":
             return numpy.concatenate([sel[i] for sel in centric_and_selections[i_bin] for i in (1,2)])
         else:
             i = 1 if use == "work" else 2
             return numpy.concatenate([sel[i] for sel in centric_and_selections[i_bin]])
     
     # Initial values
     for lab in D_labs: hkldata.binned_df[lab] = 1.
     hkldata.binned_df["S"] = 10000.
+    k_ani = hkldata.debye_waller_factors(b_cart=b_aniso)
     for i_bin, _ in hkldata.binned():
         idxes = get_idxes(i_bin)
-        valid_sel = numpy.isfinite(hkldata.df.I[idxes]) # as there is no nan-safe numpy.corrcoef
+        valid_sel = numpy.isfinite(hkldata.df.loc[idxes, lab_obs]) # as there is no nan-safe numpy.corrcoef
+        if numpy.sum(valid_sel) < 2:
+            continue
         idxes = idxes[valid_sel]
-        FC = numpy.abs(hkldata.df.FC.to_numpy()[idxes])
-        I = hkldata.df.I.to_numpy()[idxes]
-        D = numpy.corrcoef(I, FC**2)[1,0]
+        if use_int:
+            Io = hkldata.df.I.to_numpy()[idxes]
+        else:
+            Io = hkldata.df.FP.to_numpy()[idxes]**2
+        Ic = k_ani[idxes]**2 * numpy.abs(hkldata.df.FC.to_numpy()[idxes])**2
+        mean_Io = numpy.mean(Io)
+        mean_Ic = numpy.mean(Ic)
+        cc = numpy.corrcoef(Io, Ic)[1,0]
+        if cc > 0 and mean_Io > 0:
+            D = numpy.sqrt(mean_Io / mean_Ic * cc)
+        else:
+            D = 0 # will be taken care later
         hkldata.binned_df.loc[i_bin, D_labs[0]] = D
-        hkldata.binned_df.loc[i_bin, "S"] = numpy.sqrt(numpy.var(I - (D * FC)**2)) / 4 * (2-D)
+        if mean_Io > 0:
+            S = mean_Io - 2 * numpy.sqrt(mean_Io * mean_Ic * numpy.maximum(0, cc)) + mean_Ic
+        else:
+            S = numpy.std(Io) # similar initial to french_wilson
+        hkldata.binned_df.loc[i_bin, "S"] = S
 
     for D_lab in D_labs:
         if hkldata.binned_df[D_lab].min() <= 0:
             min_D = hkldata.binned_df[D_lab][hkldata.binned_df[D_lab] > 0].min() * 0.1
             logger.writeln("WARNING: negative {} is detected from initial estimates. Replacing it using minimum positive value {:.2e}".format(D_lab, min_D))
             hkldata.binned_df[D_lab].where(hkldata.binned_df[D_lab] > 0, min_D, inplace=True) # arbitrary
         
     logger.writeln("Initial estimates:")
     logger.writeln(hkldata.binned_df.to_string())
+    refpar = "all"
     for i_cyc in range(n_cycle):
+        t0 = time.time()
+        nfev_total = 0
         k_ani = hkldata.debye_waller_factors(b_cart=b_aniso)
         for i_bin, _ in hkldata.binned():
             idxes = get_idxes(i_bin)
+            valid_sel = numpy.isfinite(hkldata.df.loc[idxes, lab_obs]) # as there is no nan-safe numpy.corrcoef
+            if numpy.sum(valid_sel) < 5:
+                logger.writeln("WARNING: bin {} has no sufficient reflections".format(i_bin))
+                continue
+
             def target(x):
-                DFc = (trans.D(x[:len(fc_labs)]) * hkldata.df.loc[idxes, fc_labs]).sum(axis=1)
-                ll = ext.ll_int(hkldata.df.I[idxes], hkldata.df.SIGI[idxes], k_ani[idxes], trans.S(x[-1]) * hkldata.df.epsilon[idxes],
-                                numpy.abs(DFc), hkldata.df.centric[idxes]+1)
-                return numpy.nansum(ll)
+                if refpar == "all":
+                    Ds = trans.D(x[:len(fc_labs)])
+                    S = trans.S(x[-1])
+                elif refpar == "D":
+                    Ds = trans.D(x[:len(fc_labs)])
+                    S = hkldata.binned_df.S[i_bin]
+                else:
+                    Ds = [hkldata.binned_df[lab][i_bin] for lab in D_labs]
+                    S = trans.S(x[-1])
+                if use_int:
+                    return mli(hkldata.df, fc_labs, Ds, S, k_ani, idxes)
+                else:
+                    return mlf(hkldata.df, fc_labs, Ds, S, centric_and_selections[i_bin], use)
             def grad(x):
-                r = ext.ll_int_der1_DS(hkldata.df.I.to_numpy()[idxes], hkldata.df.SIGI.to_numpy()[idxes], k_ani[idxes], trans.S(x[-1]),
-                                       hkldata.df[fc_labs].to_numpy()[idxes], trans.D(x[:len(fc_labs)]),
-                                       hkldata.df.centric.to_numpy()[idxes]+1, hkldata.df.epsilon.to_numpy()[idxes])
-                g = numpy.zeros(len(fc_labs)+1)
-                g[:len(fc_labs)] = numpy.nansum(r[:,:len(fc_labs)], axis=0) # D
-                g[-1] = numpy.nansum(r[:,-1]) # S
-                g[:len(fc_labs)] *= trans.D_deriv(x[:len(fc_labs)])
-                g[-1] *= trans.S_deriv(x[-1])
+                if refpar == "all":
+                    Ds = trans.D(x[:len(fc_labs)])
+                    S = trans.S(x[-1])
+                    n_par = len(fc_labs)+1
+                elif refpar == "D":
+                    Ds = trans.D(x[:len(fc_labs)])
+                    S = hkldata.binned_df.S[i_bin]
+                    n_par = len(fc_labs)
+                else:
+                    Ds = [hkldata.binned_df[lab][i_bin] for lab in D_labs]
+                    S = trans.S(x[-1])
+                    n_par = 1
+                if use_int:
+                    r = deriv_mli_wrt_D_S(hkldata.df, fc_labs, Ds, S, k_ani, idxes)
+                else:
+                    r = deriv_mlf_wrt_D_S(hkldata.df, fc_labs, Ds, S, centric_and_selections[i_bin], use)
+                g = numpy.zeros(n_par)
+                if refpar in ("all", "D"):
+                    g[:len(fc_labs)] = r[:len(fc_labs)]
+                    g[:len(fc_labs)] *= trans.D_deriv(x[:len(fc_labs)])
+                if refpar in ("all", "S"):
+                    g[-1] = r[-1]
+                    g[-1] *= trans.S_deriv(x[-1])
                 return g
 
-            def shift_DS(x):
-                r = ext.ll_int_der1_DS(hkldata.df.I.to_numpy()[idxes], hkldata.df.SIGI.to_numpy()[idxes], k_ani[idxes], trans.S(x[-1]),
-                                       hkldata.df[fc_labs].to_numpy()[idxes], trans.D(x[:len(fc_labs)]),
-                                       hkldata.df.centric.to_numpy()[idxes]+1, hkldata.df.epsilon.to_numpy()[idxes])
-                g = numpy.zeros(len(fc_labs)+1)
-                g[:len(fc_labs)] = numpy.nansum(r[:,:len(fc_labs)], axis=0) * trans.D_deriv(x[:len(fc_labs)]) # D
-                g[-1] = numpy.nansum(r[:,-1]) * trans.S_deriv(x[-1]) # S
-                tmp = numpy.hstack([r[:,:len(fc_labs)] * trans.D_deriv(x[:len(fc_labs)]),
-                                    r[:,-1,None] * trans.S_deriv(x[-1])])
-                H = numpy.nansum(numpy.matmul(tmp[:,:,None], tmp[:,None]), axis=0)
-                return -numpy.dot(g, numpy.linalg.pinv(H))
-
+            if 0:
+                refpar = "S"
+                x0 = trans.S_inv(hkldata.binned_df.S[i_bin])
+                with open("s_line_{}.dat".format(i_bin), "w") as ofs:
+                    for sval in numpy.linspace(1, x0*2, 100):
+                        ofs.write("{:.4e} {:.10e} {:.10e}\n".format(sval,
+                                                                    target([sval]),
+                                                                    grad([sval])[0]))
+                continue
             #print("Bin", i_bin)
-            if 1:
+            if 1: # refine D and S iteratively
+                vals_last = None
+                for ids in range(10):
+                    refpar = "D"
+                    x0 = [trans.D_inv(hkldata.binned_df[lab][i_bin]) for lab in D_labs]
+                    res = scipy.optimize.minimize(fun=target, x0=x0, jac=grad,
+                                                  bounds=((-5 if D_trans else 1e-5, None),)*len(x0))
+                    nfev_total += res.nfev
+                    #print(i_bin, "mini cycle", ids, refpar)
+                    #print(res)
+                    vals_now = []
+                    for i, lab in enumerate(D_labs):
+                        hkldata.binned_df.loc[i_bin, lab] = trans.D(res.x[i])
+                        vals_now.append(hkldata.binned_df.loc[i_bin, lab])
+                    refpar = "S"
+                    if 1:
+                        for cyc_s in range(1):
+                            x0 = trans.S_inv(hkldata.binned_df.S[i_bin])
+                            f0 = target([x0])
+                            Ds = [hkldata.binned_df[lab][i_bin] for lab in D_labs]
+                            nfev_total += 1
+                            if use_int:
+                                shift = mli_shift_S(hkldata.df, fc_labs, Ds, trans.S(x0), k_ani, idxes)
+                            else:
+                                shift = mlf_shift_S(hkldata.df, fc_labs, Ds, trans.S(x0),
+                                                    centric_and_selections[i_bin], use)
+                            shift /= trans.S_deriv(x0)
+                            if abs(shift) < 1e-3: break
+                            for itry in range(10):
+                                x1 = x0 + shift
+                                if (S_trans and x1 < -3) or (not S_trans and x1 < 5e-2):
+                                    #print(i_bin, cyc_s, trans.S(x0), trans.S(x1), shift, "BAD")
+                                    shift /= 2
+                                    continue
+                                f1 = target([x1])
+                                nfev_total += 1
+                                if f1 > f0:
+                                    shift /= 2
+                                    continue
+                                else: # good
+                                    #print(i_bin, cyc_s, trans.S(x0), trans.S(x1), shift)
+                                    hkldata.binned_df.loc[i_bin, "S"] = trans.S(x1)
+                                    break
+                            else:
+                                #print("all bad")
+                                break
+                    else:
+                        # somehow this does not work well.
+                        x0 = [trans.S_inv(hkldata.binned_df.S[i_bin])]
+                        res = scipy.optimize.minimize(fun=target, x0=x0, jac=grad,
+                                                      bounds=((-3 if S_trans else 5e-2, None),))
+                        nfev_total += res.nfev
+                        #print(i_bin, "mini cycle", ids, refpar)
+                        #print(res)
+                        hkldata.binned_df.loc[i_bin, "S"] = trans.S(res.x[-1])
+                    vals_now.append(hkldata.binned_df.loc[i_bin, "S"])
+                    vals_now = numpy.array(vals_now)
+                    if vals_last is not None and numpy.all(numpy.abs((vals_last - vals_now) / vals_now) < 1e-2):
+                        #logger.writeln("converged in mini cycle {}".format(ids+1))
+                        break
+                    vals_last = vals_now
+            else:
                 x0 = [trans.D_inv(hkldata.binned_df[lab][i_bin]) for lab in D_labs] + [trans.S_inv(hkldata.binned_df.S[i_bin])]
-                res = scipy.optimize.minimize(fun=target, x0=x0, jac=grad)
+                res = scipy.optimize.minimize(fun=target, x0=x0, jac=grad,
+                                              bounds=((-5 if D_trans else 1e-5, None), )*len(D_labs) + ((-3 if S_trans else 5e-2, None),))
+                nfev_total += res.nfev
+                #print(i_bin)
                 #print(res)
                 for i, lab in enumerate(D_labs):
                     hkldata.binned_df.loc[i_bin, lab] = trans.D(res.x[i])
                 hkldata.binned_df.loc[i_bin, "S"] = trans.S(res.x[-1])
-            else:
-                DS_converged = False
-                for j in range(10):
-                    x = [trans.D_inv(hkldata.binned_df[lab][i_bin]) for lab in D_labs] + [trans.S_inv(hkldata.binned_df.S[i_bin])]
-                    f0 = target(x)
-                    shift = shift_DS(x)
-                    for i in range(3):
-                        ss = shift / 2**i
-                        f1 = target(x + ss)
-                        #logger.writeln("{:2d} f0 = {:.3e} shift = {} df = {:.3e}".format(j, f0, ss, f1 - f0))
-                        if f1 < f0:
-                            for i, lab in enumerate(D_labs):
-                                hkldata.binned_df.loc[i_bin, lab] = trans.D((x+ss)[i])
-                            hkldata.binned_df.loc[i_bin, "S"] = trans.S((x+ss)[-1])
-                            if numpy.max(numpy.abs(ss)) < 1e-4: DS_converged = True
-                            break
-                    else:
-                        DS_converged = True
-                    if DS_converged: break
 
         logger.writeln("Refined estimates:")
         logger.writeln(hkldata.binned_df.to_string())
+        logger.writeln("time: {:.1f} sec ({} evaluations)".format(time.time() - t0, nfev_total))
 
+        if not use_int:
+            break # did not implement MLF B_aniso optimization
+        
         # Refine b_aniso
         adpdirs = utils.model.adp_constraints(hkldata.sg.operations(), hkldata.cell, tr0=True)
         SMattolist = lambda B: [B.u11, B.u22, B.u33, B.u12, B.u13, B.u23]
 
         def target_ani(x):
             b_aniso = gemmi.SMat33d(*numpy.dot(x, adpdirs))
             k_ani = hkldata.debye_waller_factors(b_cart=b_aniso)
             ret = 0.
             for i_bin, _ in hkldata.binned():
                 idxes = get_idxes(i_bin)
                 Ds = [hkldata.binned_df[lab][i_bin] for lab in D_labs]
-                Fcs = [hkldata.df[lab].to_numpy()[idxes] for lab in fc_labs]
-                DFc = calc_DFc(Ds, Fcs)
-                ll = ext.ll_int(hkldata.df.I[idxes], hkldata.df.SIGI[idxes], k_ani[idxes],
-                                hkldata.binned_df.S[i_bin] * hkldata.df.epsilon[idxes],
-                                numpy.abs(DFc), hkldata.df.centric[idxes]+1)
-                ret += numpy.nansum(ll)
+                ret += mli(hkldata.df, fc_labs, Ds, hkldata.binned_df.S[i_bin], k_ani, idxes)
             return ret
-
+        def grad_ani(x):
+            b_aniso = gemmi.SMat33d(*numpy.dot(x, adpdirs))
+            k_ani = hkldata.debye_waller_factors(b_cart=b_aniso)
+            S2mat = hkldata.ssq_mat() # ssqmat
+            g = numpy.zeros(6)
+            for i_bin, _ in hkldata.binned():
+                idxes = get_idxes(i_bin)
+                r = ext.ll_int_der1_ani(hkldata.df.I.to_numpy()[idxes], hkldata.df.SIGI.to_numpy()[idxes],
+                                        k_ani[idxes], hkldata.binned_df.S[i_bin],
+                                        hkldata.df[fc_labs].to_numpy()[idxes], hkldata.binned_df.loc[i_bin, D_labs],
+                                        hkldata.df.centric.to_numpy()[idxes]+1, hkldata.df.epsilon.to_numpy()[idxes])
+                S2 = S2mat[:,idxes]
+                g += -numpy.nansum(S2 * r[:,0], axis=1) # k_ani is already multiplied in r
+            return numpy.dot(g, adpdirs.T)
         def shift_ani(x):
             b_aniso = gemmi.SMat33d(*numpy.dot(x, adpdirs))
             k_ani = hkldata.debye_waller_factors(b_cart=b_aniso)
             S2mat = hkldata.ssq_mat() # ssqmat
             g = numpy.zeros(6)
             H = numpy.zeros((6, 6))
             for i_bin, _ in hkldata.binned():
@@ -608,35 +711,42 @@
                 g += -numpy.nansum(S2 * r[:,0], axis=1) # k_ani is already multiplied in r
                 H += numpy.nansum(numpy.matmul(S2[None,:].T, S2.T[:,None]) * (r[:,0]**2)[:,None,None], axis=0)
 
             g, H = numpy.dot(g, adpdirs.T), numpy.dot(adpdirs, numpy.dot(H, adpdirs.T))
             return -numpy.dot(g, numpy.linalg.pinv(H))
 
         logger.writeln("Refining B_aniso. Current = {}".format(b_aniso))
-        B_converged = False
-        for j in range(10):
-            x = numpy.dot(SMattolist(b_aniso), numpy.linalg.pinv(adpdirs))
-            f0 = target_ani(x)
-            shift = shift_ani(x)
-            for i in range(3):
-                ss = shift / 2**i
-                f1 = target_ani(x + ss)
-                #logger.writeln("{:2d} f0 = {:.3e} shift = {} df = {:.3e}".format(j, f0, ss, f1 - f0))
-                if f1 < f0:
-                    b_aniso = gemmi.SMat33d(*numpy.dot(x+ss, adpdirs))
-                    if numpy.max(numpy.abs(ss)) < 1e-4: B_converged = True
-                    break
-            else:
-                B_converged = True
-            if B_converged: break
+        if 0:
+            x0 = numpy.dot(SMattolist(b_aniso), numpy.linalg.pinv(adpdirs))
+            res = scipy.optimize.minimize(fun=target_ani, x0=x0, jac=grad_ani)
+            print(res)
+            b_aniso = gemmi.SMat33d(*numpy.dot(res.x, adpdirs))
+            f1 = res.fun
+        else:
+            B_converged = False
+            for j in range(10):
+                x = numpy.dot(SMattolist(b_aniso), numpy.linalg.pinv(adpdirs))
+                f0 = target_ani(x)
+                shift = shift_ani(x)
+                for i in range(3):
+                    ss = shift / 2**i
+                    f1 = target_ani(x + ss)
+                    #logger.writeln("{:2d} f0 = {:.3e} shift = {} df = {:.3e}".format(j, f0, ss, f1 - f0))
+                    if f1 < f0:
+                        b_aniso = gemmi.SMat33d(*numpy.dot(x+ss, adpdirs))
+                        if numpy.max(numpy.abs(ss)) < 1e-4: B_converged = True
+                        break
+                else:
+                    B_converged = True
+                if B_converged: break
 
         logger.writeln("Refined B_aniso = {}".format(b_aniso))
         logger.writeln("cycle {} f= {}".format(i_cyc, f1))
     return b_aniso
-# determine_mli_params()
+# determine_ml_params()
 
 def calculate_maps_int(hkldata, b_aniso, fc_labs, D_labs, centric_and_selections, use="all"):
     nmodels = len(fc_labs)
     hkldata.df["FWT"] = 0j * numpy.nan
     hkldata.df["DELFWT"] = 0j * numpy.nan
     hkldata.df["FOM"] = numpy.nan
     Io = hkldata.df.I.to_numpy()
@@ -683,21 +793,33 @@
                 model.add_chain(c)
     st.add_model(model)
     return st
 # merge_models()
 
 def process_input(hklin, labin, n_bins, free, xyzins, source, d_max=None, d_min=None,
                   n_per_bin=None, use="all", max_bins=None):
-    assert 1 < len(labin) < 4
+    if labin: assert 1 < len(labin) < 4
     assert use in ("all", "work", "test")
     assert n_bins or n_per_bin #if n_bins not set, n_per_bin should be given
 
     if utils.fileio.is_mmhkl_file(hklin):
         mtz = utils.fileio.read_mmhkl(hklin)
         col_types = {x.label:x.type for x in mtz.columns}
+        if not labin:
+            dlabs = utils.hkl.mtz_find_data_columns(mtz)
+            if dlabs["F"]: # F is preferred for now
+                labin = dlabs["F"][0]
+            elif dlabs["J"]:
+                labin = dlabs["J"][0]
+            else:
+                raise RuntimeError("Data not found from mtz")
+            flabs = utils.hkl.mtz_find_free_columns(mtz)
+            if flabs:
+                labin += [flabs[0]]
+            logger.writeln("MTZ columns automatically selected: {}".format(labin))
         if labin[0] not in col_types:
             raise RuntimeError("MTZ coulumn not found: {}".format(labin[0]))
         if col_types[labin[0]] == "F":
             logger.writeln("Observation type: amplitude")
             newlabels = ["FP","SIGFP"]
             require_types = ["F", "Q"]
         elif col_types[labin[0]] == "J":
@@ -713,34 +835,38 @@
         assert len(xyzins) == 1
         st, hkldata = utils.fileio.read_small_molecule_files([hklin, xyzins[0]])
         sts = [st]
         newlabels = hkldata.columns()
     
     if sts:
         assert source in ["electron", "xray", "neutron"]
+        for st in sts:
+            if st[0].count_atom_sites() == 0:
+                raise RuntimeError("No atom in the model")
         if not hkldata.cell.approx(sts[0].cell, 1e-3):
             logger.writeln("Warning: unit cell mismatch between model and reflection data")
             logger.writeln("         using unit cell from mtz")
 
         for st in sts: st.cell = hkldata.cell # mtz cell is used in any case
 
         sg_st = sts[0].find_spacegroup() # may be None
         sg_use = hkldata.sg
         if hkldata.sg != sg_st:
             logger.writeln("Warning: space group mismatch between model and mtz")
-            pg_mtz = utils.hkl.intensity_symmetry(hkldata.sg)
-            pg_st = utils.hkl.intensity_symmetry(sg_st)
-            if sg_st and pg_mtz == pg_st:
+            if sg_st and sg_st.laue_str() == hkldata.sg.laue_str():
                 logger.writeln("         using space group from model")
                 sg_use = sg_st
             else:
                 logger.writeln("         using space group from mtz")
             logger.writeln("")
 
-        for st in sts: st.spacegroup_hm = sg_use.xhm()
+        for st in sts:
+            if st.find_spacegroup() != sg_use:
+                st.spacegroup_hm = sg_use.xhm()
+            st.setup_cell_images()
         hkldata.sg = sg_use
         
     hkldata.remove_nonpositive(newlabels[1])
     hkldata.switch_to_asu()
     hkldata.remove_systematic_absences()
     #hkldata.df = hkldata.df.astype({name: 'float64' for name in ["I","SIGI"]})
 
@@ -755,15 +881,18 @@
 
     if n_bins is None:
         sel = hkldata.df[newlabels[0]].notna()
         if use == "work":
             sel &= hkldata.df.FREE != free
         elif use == "test":
             sel &= hkldata.df.FREE == free
-        n_bins = utils.hkl.decide_n_bins(n_per_bin, 1/hkldata.d_spacings()[sel], max_bins=max_bins)
+        s_array = 1/hkldata.d_spacings()[sel]
+        if len(s_array) == 0:
+            raise RuntimeError("no reflections in {} set".format(use))
+        n_bins = utils.hkl.decide_n_bins(n_per_bin, s_array, max_bins=max_bins)
         logger.writeln("n_per_bin={} requested for {}. n_bins set to {}".format(n_per_bin, use, n_bins))
 
     hkldata.setup_binning(n_bins=n_bins)
     logger.writeln("Data completeness: {:.2f}%".format(hkldata.completeness()*100.))
 
     fc_labs = []
     for i, st in enumerate(sts):
@@ -775,15 +904,15 @@
 
     # Create a centric selection table for faster look up
     centric_and_selections = {}
     stats = hkldata.binned_df.copy()
     stats["n_all"] = 0
     stats["n_obs"] = 0
     snr = "I/sigma" if newlabels[0] == "I" else "F/sigma"
-    stats[snr] = 0.
+    stats[snr] = numpy.nan
     if "FREE" in hkldata.df:
         stats["n_work"] = 0
         stats["n_test"] = 0
         
     for i_bin, idxes in hkldata.binned():
         centric_and_selections[i_bin] = []
         n_obs = 0
@@ -802,15 +931,16 @@
             centric_and_selections[i_bin].append((c, work, test))
             n_obs += numpy.sum(valid_sel)
             
         stats.loc[i_bin, "n_obs"] = n_obs
         stats.loc[i_bin, "n_all"] = len(idxes)
         obs = hkldata.df[newlabels[0]].to_numpy()[idxes]
         sigma = hkldata.df[newlabels[1]].to_numpy()[idxes]
-        stats.loc[i_bin, snr] = numpy.nanmean(obs / sigma)
+        if n_obs > 0:
+            stats.loc[i_bin, snr] = numpy.nanmean(obs / sigma)
         if "FREE" in hkldata.df:
             stats.loc[i_bin, "n_work"] = n_work
             stats.loc[i_bin, "n_test"] = n_test
             
     stats["completeness"] = stats["n_obs"] / stats["n_all"] * 100
     logger.writeln(stats.to_string())
     return hkldata, sts, fc_labs, centric_and_selections
@@ -831,112 +961,119 @@
 
 def bulk_solvent_and_lsq_scales(hkldata, sts, fc_labs, use_solvent=True, use_int=False):
     fc_list = [hkldata.df[fc_labs].sum(axis=1).to_numpy()]
     if use_solvent:
         Fmask = calc_Fmask(merge_models(sts), hkldata.d_min_max()[0] - 1e-6, hkldata.miller_array())
         fc_list.append(Fmask)
 
-    obs = hkldata.df["I" if use_int else "FP"].to_numpy()
-    scaling = LsqScale(hkldata, obs, fc_list, use_int)
+    scaling = LsqScale(hkldata, fc_list, use_int, sigma_cutoff=0)
     scaling.scale()
     b_aniso = scaling.b_aniso
     b_iso = scaling.b_iso
     k_iso = hkldata.debye_waller_factors(b_iso=b_iso)
     k_aniso = hkldata.debye_waller_factors(b_cart=b_aniso)
     hkldata.df["k_aniso"] = k_aniso # we need it later when calculating stats
     
     if use_solvent:
         fc_labs.append("Fbulk")
-        solvent_scale = scaling.get_solvent_scale(scaling.k_sol, scaling.b_sol)
+        solvent_scale = scaling.get_solvent_scale(scaling.k_sol, scaling.b_sol,
+                                                  1. / hkldata.d_spacings().to_numpy()**2)
         hkldata.df[fc_labs[-1]] = Fmask * solvent_scale
 
     # Apply scales.
     #  - k_aniso^-1 is applied to FP (isotropize), 
     #    but k_aniso should be applied to FC when calculating R or CC
     #  - k_iso should be applied to FC
     if use_int:
         # in intensity case, we try to refine b_aniso with ML. perhaps we should do it in amplitude case also
         hkldata.df.I /= scaling.k_overall**2
         hkldata.df.SIGI /= scaling.k_overall**2
     else:
-        hkldata.df.FP /= scaling.k_overall * k_aniso
-        hkldata.df.SIGFP /= scaling.k_overall * k_aniso
+        hkldata.df.FP /= scaling.k_overall
+        hkldata.df.SIGFP /= scaling.k_overall
     for lab in fc_labs: hkldata.df[lab] *= k_iso
     # total Fc
     hkldata.df["FC"] = hkldata.df[fc_labs].sum(axis=1)
     return scaling.k_overall, b_aniso
 # bulk_solvent_and_lsq_scales()
 
-def calculate_maps(hkldata, centric_and_selections, fc_labs, D_labs, log_out, use="all"):
+def calculate_maps(hkldata, b_aniso, centric_and_selections, fc_labs, D_labs, log_out, use="all"):
     nmodels = len(fc_labs)
     hkldata.df["FWT"] = 0j * numpy.nan
     hkldata.df["DELFWT"] = 0j * numpy.nan
     hkldata.df["FOM"] = numpy.nan
     hkldata.df["X"] = numpy.nan # for FOM
     stats_data = []
+    k_ani = hkldata.debye_waller_factors(b_cart=b_aniso)
     for i_bin, idxes in hkldata.binned():
         bin_d_min = hkldata.binned_df.d_min[i_bin]
         bin_d_max = hkldata.binned_df.d_max[i_bin]
         Ds = [max(0., hkldata.binned_df[lab][i_bin]) for lab in D_labs] # negative D is replaced with zero here
         DFcs = [numpy.log(Ds[i] * numpy.nanmean(numpy.abs(hkldata.df[lab].to_numpy()[idxes])))
                 for i, lab in enumerate(fc_labs)]
         S = hkldata.binned_df.S[i_bin]
         
         # 0: acentric 1: centric
-        mean_fom = [0, 0]
+        mean_fom = [numpy.nan, numpy.nan]
         nrefs = [0, 0]
         for c, work, test in centric_and_selections[i_bin]:
             cidxes = numpy.concatenate([work, test])
-            Fcs = [hkldata.df[lab].to_numpy()[cidxes] for lab in fc_labs]
-            Fc = numpy.abs(hkldata.df.FC.to_numpy()[cidxes])
+            Fcs = [hkldata.df[lab].to_numpy()[cidxes] * k_ani[cidxes] for lab in fc_labs]
             phic = numpy.angle(hkldata.df.FC.to_numpy()[cidxes])
             expip = numpy.cos(phic) + 1j*numpy.sin(phic)
             Fo = hkldata.df.FP.to_numpy()[cidxes]
             SigFo = hkldata.df.SIGFP.to_numpy()[cidxes]
             epsilon = hkldata.df.epsilon.to_numpy()[cidxes]
-            nrefs[c] = len(cidxes)
+            nrefs[c] = numpy.sum(numpy.isfinite(Fo))
             DFc = calc_abs_DFc(Ds, Fcs)
             if c == 0:
-                Sigma = 2 * SigFo**2 + epsilon * S
+                Sigma = 2 * SigFo**2 + epsilon * S * k_ani[cidxes]**2
                 X = 2 * Fo * DFc / Sigma
                 m = gemmi.bessel_i1_over_i0(X)
                 hkldata.df.loc[cidxes, "FWT"] = (2 * m * Fo - DFc) * expip
             else:
-                Sigma = SigFo**2 + epsilon * S
+                Sigma = SigFo**2 + epsilon * S * k_ani[cidxes]**2
                 X = Fo * DFc / Sigma
                 m = numpy.tanh(X)
                 hkldata.df.loc[cidxes, "FWT"] = (m * Fo) * expip
 
             hkldata.df.loc[cidxes, "DELFWT"] = (m * Fo - DFc) * expip
             hkldata.df.loc[cidxes, "FOM"] = m
             hkldata.df.loc[cidxes, "X"] = X
-            mean_fom[c] = numpy.nanmean(m)
+            if nrefs[c] > 0: mean_fom[c] = numpy.nanmean(m)
 
             # remove reflections that should be hidden
             if use != "all":
                 # usually use == "work"
                 tohide = test if use == "work" else work
                 hkldata.df.loc[tohide, "FWT"] = 0j * numpy.nan
                 hkldata.df.loc[tohide, "DELFWT"] = 0j * numpy.nan
             fill_sel = numpy.isnan(hkldata.df["FWT"][cidxes].to_numpy())
             hkldata.df.loc[cidxes[fill_sel], "FWT"] = (DFc * expip)[fill_sel]
 
-        k = hkldata.df.k_aniso.to_numpy()[idxes]
-        Fc = hkldata.df.FC.to_numpy()[idxes] * k
-        Fcs = [hkldata.df[lab].to_numpy()[idxes] * k for lab in fc_labs]
-        Fo = hkldata.df.FP.to_numpy()[idxes] * k
+        Fc = hkldata.df.FC.to_numpy()[idxes]
+        Fcs = [hkldata.df[lab].to_numpy()[idxes] for lab in fc_labs]
+        Fo = hkldata.df.FP.to_numpy()[idxes]
         DFc = calc_abs_DFc(Ds, Fcs)
-        r = numpy.nansum(numpy.abs(numpy.abs(Fc)-Fo)) / numpy.nansum(Fo)
-        cc = utils.hkl.correlation(Fo, numpy.abs(Fc))
+        if sum(nrefs) > 0:
+            r = numpy.nansum(numpy.abs(numpy.abs(Fc)-Fo)) / numpy.nansum(Fo)
+            cc = utils.hkl.correlation(Fo, numpy.abs(Fc))
+            mean_Fo2 = numpy.nanmean(numpy.abs(Fo)**2)
+        else:
+            r, cc, mean_Fo2 = numpy.nan, numpy.nan, numpy.nan
         stats_data.append([1/bin_d_min**2, i_bin, nrefs[0], nrefs[1], bin_d_max, bin_d_min,
-                           numpy.log(numpy.nanmean(numpy.abs(Fo)**2)),
+                           numpy.log(mean_Fo2),
                            numpy.log(numpy.nanmean(numpy.abs(Fc)**2)),
                            numpy.log(numpy.nanmean(DFc**2)),
                            numpy.log(S), mean_fom[0], mean_fom[1], r, cc] + Ds + DFcs)
 
+    # make maps isotropic
+    hkldata.df["FWT"] /= k_ani
+    hkldata.df["DELFWT"] /= k_ani    
+
     s2lab = "1/resol^2"
     DFc_labs = ["log(Mn(|{}{}|))".format(dl,fl) for dl,fl in zip(D_labs, fc_labs)]
     cols = [s2lab, "bin", "n_a", "n_c", "d_max", "d_min",
             "log(Mn(|Fo|^2))", "log(Mn(|Fc|^2))", "log(Mn(|DFc|^2))",
             "log(Sigma)", "FOM_a", "FOM_c", "R", "CC(|Fo|,|Fc|)"] + D_labs + DFc_labs
     stats = pandas.DataFrame(stats_data, columns=cols)
     title_labs = [["log(Mn(|F|^2)) and variances", [s2lab, "log(Mn(|Fo|^2))", "log(Mn(|Fc|^2))", "log(Mn(|DFc|^2))", "log(Sigma)"]],
@@ -969,31 +1106,26 @@
     # Overall scaling & bulk solvent
     # FP/SIGFP will be scaled. Total FC will be added.
     k_overall, b_aniso = bulk_solvent_and_lsq_scales(hkldata, sts, fc_labs, use_solvent=not args.no_solvent,
                                                      use_int=is_int)
     # Estimate ML parameters
     D_labs = ["D{}".format(i) for i in range(len(fc_labs))]
 
+    if args.use_cc:
+        assert not is_int
+        logger.writeln("Estimating sigma-A parameters from CC..")
+        determine_mlf_params_from_cc(hkldata, fc_labs, D_labs, centric_and_selections, args.use)
+    else:
+        b_aniso = determine_ml_params(hkldata, is_int, fc_labs, D_labs, b_aniso, centric_and_selections, args.D_trans, args.S_trans, args.use)
     if is_int:
-        assert not args.use_cc
-        logger.writeln("Estimating sigma-A parameters using ML..")
-        b_aniso = determine_mli_params(hkldata, fc_labs, D_labs, b_aniso, centric_and_selections, args.D_as_exp, args.S_as_exp, args.use)
         calculate_maps_int(hkldata, b_aniso, fc_labs, D_labs, centric_and_selections,
                            use={"all": "all", "work": "work", "test": "work"}[args.use])
     else:
-        if args.use_cc:
-            logger.writeln("Estimating sigma-A parameters from CC..")
-            determine_mlf_params_from_cc(hkldata, fc_labs, D_labs, centric_and_selections, args.use)
-        else:
-            logger.writeln("Estimating sigma-A parameters using ML..")
-            determine_mlf_params(hkldata, fc_labs, D_labs, centric_and_selections, args.D_as_exp, args.S_as_exp, args.use)
-
-        # Calculate maps
         log_out = "{}.log".format(args.output_prefix)
-        calculate_maps(hkldata, centric_and_selections, fc_labs, D_labs, log_out,
+        calculate_maps(hkldata, b_aniso, centric_and_selections, fc_labs, D_labs, log_out,
                        use={"all": "all", "work": "work", "test": "work"}[args.use])
 
     # Write mtz file
     if is_int:
         labs = ["I", "SIGI"]
     else:
         labs = ["FP", "SIGFP", "FOM"]
```

### Comparing `servalcat-0.4.15/setup.py` & `servalcat-0.4.24/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import division, absolute_import, print_function
 import setuptools
 from setuptools import setup, Extension
 from setuptools.command.build_ext import build_ext
 from setuptools import distutils
-from pybind11.setup_helpers import Pybind11Extension
+try:
+    from pybind11.setup_helpers import Pybind11Extension
+except ImportError:
+    from setuptools import Extension as Pybind11Extension
 import glob
 import sys
 import os
 import servalcat
 
 ext_modules = [
     Pybind11Extension(
@@ -116,23 +119,24 @@
         for ext in self.extensions:
             ext.define_macros = [('VERSION_INFO',
                                   '"%s"' % self.distribution.get_version())]
             ext.extra_compile_args = opts
             ext.extra_link_args = link_opts
         build_ext.build_extensions(self)
 
-
 setup(name='servalcat',
     version=servalcat.__version__,
     author='Keitaro Yamashita and Garib N. Murshudov',
     url='https://github.com/keitaroyam/servalcat',
     description= 'Structure refinement and validation for crystallography and single particle analysis',
+    long_description="Please see https://github.com/keitaroyam/servalcat",
+    long_description_content_type='text/markdown',
     license='MPL-2.0',
     packages=setuptools.find_packages(),
-    install_requires=['numpy>=1.15','scipy','pandas>=0.24.2', 'gemmi==0.6.1'],
+    install_requires=['numpy>=1.15','scipy','pandas>=0.24.2', 'gemmi==0.6.2'],
     entry_points={
       'console_scripts': [
           'servalcat = servalcat.command_line:main',
           'refmacat  = servalcat.refmac.refmac_wrapper:command_line',
                           ],
       },
     ext_modules=ext_modules,
```

### Comparing `servalcat-0.4.15/src/ext.cpp` & `servalcat-0.4.24/src/ext.cpp`

 * *Files identical despite different names*

### Comparing `servalcat-0.4.15/src/intensity.cpp` & `servalcat-0.4.24/src/intensity.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 // Author: "Keitaro Yamashita, Garib N. Murshudov"
 // MRC Laboratory of Molecular Biology
 
 #include <pybind11/numpy.h>
 #include <pybind11/stl.h>
 #include <pybind11/complex.h>
 #include <gemmi/bessel.hpp>
+#include <gemmi/math.hpp>
 #include "math.hpp"
 namespace py = pybind11;
 using namespace servalcat;
 
 // for MLI
 double f1_orig2(double x, double z, double to, double tf, double sig1, int c) {
   // z = 2k+1
@@ -63,62 +64,91 @@
   const double m = fom(X, c);
   const double m_der = tf == 0 ? 0 : fom_der(m, X, c);
   return ret + e_y * (3-c) * tf / sig1 * m * std::exp(y - e_y) - sq(1 + e_y) * ((3-c) * tf / sig1 * m * std::exp(y - e_y) - sq(3-c) * sq(tf / sig1) * m_der * exp2);
 }
 double find_root(double k, double to, double tf, double sig1, int c, double det, bool use_exp2) {
   if (tf == 0.) {
     if (use_exp2)
-      return solve_y_minus_exp_minus_y(0.5 * std::log(0.5 * x_plus_sqrt_xsq_plus_y(to, 4 * k + 4)), 1e-2); // XXX may not be exact
+      return solve_y_minus_exp_minus_y(0.5 * std::log(0.5 * x_plus_sqrt_xsq_plus_y(to, 4 * k + 4)), 1e-4); // XXX may not be exact
     return det;
   }
   const double z = use_exp2 ? 2 * k + 2 : 2 * k + 1;
   auto fder1 = use_exp2 ? f1_exp2_der1 : f1_orig2_der1;
   auto fder2 = use_exp2 ? f1_exp2_der2 : f1_orig2_der2;
   double x0 = det, x1 = NAN;
   if (use_exp2) {
     const double X1 = (3-c) * tf * 0.5 / sig1 * std::sqrt(0.5 * x_plus_sqrt_xsq_plus_y(to, 4 * k + 3.5));
     const double m1 = fom(X1, c);
-    x0 = solve_y_minus_exp_minus_y(0.5 * std::log(0.5 * x_plus_sqrt_xsq_plus_y(to, 4 * k + 4 * X1 * m1 + 3.5)), 1e-2);
+    x0 = solve_y_minus_exp_minus_y(0.5 * std::log(0.5 * x_plus_sqrt_xsq_plus_y(to, 4 * k + 4 * X1 * m1 + 3.5)), 1e-4);
+    if (std::isnan(x0))
+      printf("ERROR: x0= %e, use_exp2= %d, X1=%e, m1=%e in_log=%e\n", x0, use_exp2, X1, m1,
+             0.5 * x_plus_sqrt_xsq_plus_y(to, 4 * k + 4 * X1 * m1 + 3.5));
     const double A = std::max(to, std::max((3-c) * tf / 4 / sig1, k + 1));
-    x1 = solve_y_minus_exp_minus_y(std::log(0.5 * (std::sqrt(A) + std::sqrt(A + 4 * std::sqrt(A)))), 1e-2);
+    x1 = solve_y_minus_exp_minus_y(std::log(0.5 * (std::sqrt(A) + std::sqrt(A + 4 * std::sqrt(A)))), 1e-4);
+  } else {
+    const double A = std::max(to, std::max((3-c) * tf / 4 / sig1, k + 0.5));
+    x1 = 0.5 * (std::sqrt(A) + std::sqrt(A + 4 * std::sqrt(A)));
   }
   if (std::isinf(x0) || std::isnan(x0))
-    printf("ERROR: x0= %f, use_exp2= %d, z=%f, to=%f, tf=%f, sig1=%f, c=%d, det=%f\n", x0, use_exp2, z, to, tf, sig1, c, det);
+    printf("ERROR: x0= %e, use_exp2= %d, z=%e, to=%e, tf=%e, sig1=%e, c=%d, det=%e\n", x0, use_exp2, z, to, tf, sig1, c, det);
   auto func = [&](double x) { return fder1(x, z, to, tf, sig1, c); };
   auto fprime = [&](double x) { return fder2(x, z, to, tf, sig1, c); };
+  //printf("debug %d x0= %f x1= %f f'_x0= %f f'_x1= %f\n", use_exp2, x0, x1, func(x0), func(x1));
+  if (std::abs(func(x0)) < 1e-2) // need to check. 1e-2 is small enough?
+    return x0;
   double root;
   try {
     root = newton(func, fprime, x0);
+    //printf("newton %f %f\n", root, func(root));
+    if (std::abs(func(root)) < 1e-2) // need to check. 1e-2 is small enough?
+      return root;
   } catch (const std::runtime_error& err) {
-    double a = x0, b = std::isnan(x1) ? x0 : x1;
-    double fa = func(a), fb = func(b);
-    if (fa * fb > 0) { // should not happen for use_exp2 case, just for safety
-      double inc = fa < 0 ? 0.1 : -0.1;
-      for (int i = 0; i < 10000; ++i, b+=inc) { // to prevent infinite loop
-        fb = func(b);
-        if (fa * fb < 0) break;
-      }
-      if (fa * fb >= 0) throw std::runtime_error("interval not found");
+    // proceed to bisect
+  }
+
+  double a = x0, b = std::isnan(x1) ? x0 : x1;
+  double fa = func(a), fb = func(b);
+  if (fa * fb > 0) { // should not happen, just for safety
+    printf("DEBUG: bad_interval x0= %e, x1= %e, use_exp2= %d, z=%e, to=%e, tf=%e, sig1=%e, c=%d, det=%e\n",
+           x0, x1, use_exp2, z, to, tf, sig1, c, det);
+    double inc = fa < 0 ? 0.1 : -0.1;
+    for (int i = 0; i < 10000; ++i, b+=inc) { // to prevent infinite loop
+      fb = func(b);
+      if (fa * fb < 0) break;
     }
-    root = bisect(func, a, b, 100, 1e-2);
+    if (fa * fb >= 0) throw std::runtime_error("interval not found");
+  }
+  try {
+    root = bisect(func, a, b, 10000, 1e-2);
+  } catch (const std::runtime_error& err) {
+    printf("DEBUG: bisect_fail x0= %e, x1= %e, use_exp2= %d, z=%e, to=%e, tf=%e, sig1=%e, c=%d, det=%e\n",
+           x0, x1, use_exp2, z, to, tf, sig1, c, det);
+    return NAN;
+    //throw std::runtime_error(err.what());
   }
   return root;
 }
 
 double integ_j(double k, double to, double tf, double sig1, int c, bool return_log,
                double exp2_threshold=3., double h=0.5, int N=200, double ewmax=20.) {
-  if (std::isnan(to)) return NAN;
+  if (std::isnan(to) || sig1 <= 0) return NAN; // perhaps sig1<0 should not return nan.. they considered 0 in sum
   const double det = std::sqrt(0.5 * x_plus_sqrt_xsq_plus_y(to, 2 * (2 * k + 1)));
   const bool use_exp2 = det < exp2_threshold;
   const double z = use_exp2 ? 2 * k + 2 : 2 * k + 1;
   auto f = use_exp2 ? f1_exp2 : f1_orig2;
   auto fder2 = use_exp2 ? f1_exp2_der2 : f1_orig2_der2;
   const double root = find_root(k, to, tf, sig1, c, det, use_exp2);
   const double f1val = f(root, z, to, tf, sig1, c);
   const double f2der = fder2(root, z, to, tf, sig1, c);
+  if (f2der * f1val * f1val > 1e10) { // Laplace approximation threshould needs to be revisited
+    if (use_exp2) {
+      const double lap = -f1val - 0.5 * std::log(f2der) + 0.5 * std::log(gemmi::pi() * 0.5);
+      return return_log ? lap : std::exp(lap);
+    }
+  }
   const double delta = h * std::sqrt(2 / f2der);
   double s = 1; // for i = 0
   for (int sign : {-1, 1}) {
     for (int i = 1; i < N; ++i) {
       const double xx = sign * delta * i + root;
       if (!use_exp2 && xx <= 0) continue; //break?
       const double ff = f(xx, z, to, tf, sig1, c) - f1val;
@@ -130,15 +160,15 @@
   const double expon = -f1val + 0.5 * (std::log(2.) - std::log(f2der));
   return return_log ? expon + std::log(laplace_correct) : std::exp(expon) * laplace_correct;
 }
 
 double integ_j_ratio(double k_num, double k_den, bool l, double to, double tf, double sig1, int c,
                      double exp2_threshold=3., double h=0.5, int N=200, double ewmax=20.) {
   // factor of sig^{k_num - k_den} is needed, which should be done outside.
-  if (std::isnan(to)) return NAN;
+  if (std::isnan(to) || sig1 <= 0) return NAN;
   const double det = std::sqrt(0.5 * x_plus_sqrt_xsq_plus_y(to, 2 * (2 * k_den + 1)));
   const bool use_exp2 = det < exp2_threshold;
   const double z = use_exp2 ? 2 * k_den + 2 : 2 * k_den + 1;
   const double deltaz = 2 * (k_num - k_den);
   auto f = use_exp2 ? f1_exp2 : f1_orig2;
   auto fder2 = use_exp2 ? f1_exp2_der2 : f1_orig2_der2;
   const double root = find_root(k_den, to, tf, sig1, c, det, use_exp2);
@@ -163,20 +193,22 @@
     }
   }
   return sn / sd;
 }
 
 // ML intensity target; -log(Io; Fc) without constants
 double ll_int(double Io, double sigIo, double k_ani, double S, double Fc, int c) {
-  if (std::isnan(Io)) return NAN;
+  if (std::isnan(Io) || S <= 0) return NAN;
   const double k = c == 1 ? 0 : -0.5;
   const double to = Io / sigIo - sigIo / c / sq(k_ani) / S;
   const double Ic = sq(Fc);
   const double tf = k_ani * Fc / std::sqrt(sigIo);
   const double sig1 = sq(k_ani) * S / sigIo;
+  if (sig1 < 0)
+    printf("ERROR: negative sig1= %f k_ani= %f S= %f sigIo= %f\n", sig1, k_ani, S, sigIo);
   const double logj = integ_j(k, to, tf, sig1, c, true);
   if (c == 1) // acentrics
     return 2 * std::log(k_ani) + std::log(S) + Ic / S - logj;
   else
     return std::log(k_ani) + 0.5 * std::log(S) + 0.5 * Ic / S - logj;
 }
 
@@ -228,25 +260,27 @@
   auto sum_Fc = [&](int i) {
                   std::complex<double> s = Fcs_(i, 0) * Ds[0];
                   for (size_t j = 1; j < n_models; ++j)
                     s += Fcs_(i, j) * Ds[j];
                   return s;
                 };
   for (size_t i = 0; i < n_ref; ++i) {
-    if (std::isnan(Io_(i))) {
+    if (S <= 0 || std::isnan(Io_(i))) {
       for (size_t j = 0; j < n_cols; ++j)
         ptr[i * n_cols + j] = NAN;
       continue;
     }
     const std::complex<double> Fc_total_conj = std::conj(sum_Fc(i));
     const double Fc_abs = std::abs(Fc_total_conj);
     const double to = Io_(i) / sigIo_(i) - sigIo_(i) / c_(i) / sq(k_ani_(i)) / S / eps_(i);
     const double sqrt_sigIo = std::sqrt(sigIo_(i));
     const double tf = k_ani_(i) * Fc_abs / sqrt_sigIo;
     const double sig1 = sq(k_ani_(i)) * S * eps_(i) / sigIo_(i);
+    if (sig1 < 0)
+      printf("ERROR2: negative sig1= %f k_ani= %f S= %f eps= %d sigIo= %f\n", sig1, k_ani_(i), S, eps_(i), sigIo_(i));
     const double k_num_1 = c_(i) == 1 ? 1. : 0.5;
     const double k_num_2 = c_(i) == 1 ? 0.5 : 0.;
     const double j_ratio_1 = integ_j_ratio(k_num_1, k_num_1 - 1, false, to, tf, sig1, c_(i)) * sigIo_(i);
     const double j_ratio_2 = integ_j_ratio(k_num_2, k_num_2 - 0.5, true, to, tf, sig1, c_(i)) * sqrt_sigIo;
     if (for_DS) {
       const double tmp = ll_int_der1_D(k_ani_(i), S, Fc_abs, c_(i), eps_(i), j_ratio_2);
       for (size_t j = 0; j < n_models; ++j) {
@@ -257,14 +291,62 @@
     }
     else
       ptr[i] = ll_int_der1_ani(k_ani_(i), S, Fc_abs, c_(i), eps_(i), j_ratio_1, j_ratio_2);
   }
   return ret;
 }
 
+// an attemp to fast update of Sigma, but it does look good.
+double find_ll_int_S_from_current_estimates_py(py::array_t<double> Io, py::array_t<double> sigIo, py::array_t<double> k_ani,
+					       double S, py::array_t<std::complex<double>> Fcs, std::vector<double> Ds,
+					       py::array_t<int> c, py::array_t<int> eps) {
+  if (Ds.size() != (size_t)Fcs.shape(1)) throw std::runtime_error("Fc and D shape mismatch");
+  const size_t n_models = Fcs.shape(1);
+  const size_t n_ref = Fcs.shape(0);
+  auto Io_ = Io.unchecked<1>();
+  auto sigIo_ = sigIo.unchecked<1>();
+  auto k_ani_ = k_ani.unchecked<1>();
+  auto Fcs_ = Fcs.unchecked<2>();
+  auto c_ = c.unchecked<1>();
+  auto eps_ = eps.unchecked<1>();
+
+  auto sum_Fc = [&](int i) {
+                  std::complex<double> s = Fcs_(i, 0) * Ds[0];
+                  for (size_t j = 1; j < n_models; ++j)
+                    s += Fcs_(i, j) * Ds[j];
+                  return s;
+                };
+  int count = 0;
+  double ret = 0;
+  for (size_t i = 0; i < n_ref; ++i) {
+    if (S <= 0 || std::isnan(Io_(i)))
+      continue;
+    const std::complex<double> Fc_total_conj = std::conj(sum_Fc(i));
+    const double Fc_abs = std::abs(Fc_total_conj);
+    const double to = Io_(i) / sigIo_(i) - sigIo_(i) / c_(i) / sq(k_ani_(i)) / S / eps_(i);
+    const double sqrt_sigIo = std::sqrt(sigIo_(i));
+    const double tf = k_ani_(i) * Fc_abs / sqrt_sigIo;
+    const double sig1 = sq(k_ani_(i)) * S * eps_(i) / sigIo_(i);
+    if (sig1 < 0)
+      printf("ERROR2: negative sig1= %f k_ani= %f S= %f eps= %d sigIo= %f\n", sig1, k_ani_(i), S, eps_(i), sigIo_(i));
+    const double k_num_1 = c_(i) == 1 ? 1. : 0.5;
+    const double k_num_2 = c_(i) == 1 ? 0.5 : 0.;
+    const double j_ratio_1 = integ_j_ratio(k_num_1, k_num_1 - 1, false, to, tf, sig1, c_(i)) * sigIo_(i);
+    const double j_ratio_2 = integ_j_ratio(k_num_2, k_num_2 - 0.5, true, to, tf, sig1, c_(i)) * sqrt_sigIo;
+    const double tmp = ll_int_der1_D(k_ani_(i), S, Fc_abs, c_(i), eps_(i), j_ratio_2);
+    if (c_(i) == 1) // acentrics
+      ret += (sq(Fc_abs) + j_ratio_1 / sq(k_ani_(i)) / c_(i) - (3-c_(i)) * Fc_abs * j_ratio_2 / k_ani_(i)) / eps_(i);
+    else
+      ret += (sq(Fc_abs) + 2 * (j_ratio_1 / c_(i) / k_ani_(i) - (3-c_(i)) * Fc_abs * j_ratio_2) / k_ani_(i)) / eps_(i);
+    ++count;
+  }
+  if (count == 0) return NAN;
+  return ret / count;
+}
+
 // For French-Wilson
 template<bool for_S>
 py::array_t<double>
 ll_int_fw_der1_params_py(py::array_t<double> Io, py::array_t<double> sigIo, py::array_t<double> k_ani,
                          double S, py::array_t<int> c, py::array_t<int> eps) {
   size_t n_ref = Io.shape(0);
   auto Io_ = Io.unchecked<1>();
@@ -279,15 +361,15 @@
   for (size_t i = 0; i < n_ref; ++i) {
     if (std::isnan(Io_(i))) {
       ptr[i] = NAN;
       continue;
     }
     const double to = Io_(i) / sigIo_(i) - sigIo_(i) / c_(i) / sq(k_ani_(i)) / S / eps_(i);
     const double k_num = c_(i) == 1 ? 1. : 0.5;
-    const double j_ratio_1 = integ_j_ratio(k_num, k_num - 1, false, to, 0., 0., c_(i)) * sigIo_(i);
+    const double j_ratio_1 = integ_j_ratio(k_num, k_num - 1, false, to, 0., 1., c_(i)) * sigIo_(i);
     if (for_S)
       ptr[i] = ll_int_der1_S(k_ani_(i), S, 0., c_(i), eps_(i), j_ratio_1, 0.);
     else
       ptr[i] = ll_int_der1_ani(k_ani_(i), S, 0., c_(i), eps_(i), j_ratio_1, 0.);
   }
   return ret;
 }
@@ -300,11 +382,19 @@
         py::arg("k_num"), py::arg("k_den"), py::arg("l"), py::arg("to"), py::arg("tf"),
         py::arg("sig1"), py::arg("c"),
         py::arg("exp2_threshold")=10, py::arg("h")=0.5, py::arg("N")=200, py::arg("ewmax")=20.);
   m.def("ll_int", py::vectorize(ll_int),
         py::arg("Io"), py::arg("sigIo"), py::arg("k_ani"), py::arg("S"), py::arg("Fc"), py::arg("c"));
   m.def("ll_int_der1_DS", &ll_int_der1_params_py<true>);
   m.def("ll_int_der1_ani", &ll_int_der1_params_py<false>);
+  m.def("find_ll_int_S_from_current_estimates", &find_ll_int_S_from_current_estimates_py);
   m.def("ll_int_fw_der1_S", &ll_int_fw_der1_params_py<true>);
   m.def("ll_int_fw_der1_ani", &ll_int_fw_der1_params_py<false>);
   m.def("lambertw", py::vectorize(lambertw::lambertw));
+  m.def("find_root", &find_root);
+  m.def("f1_orig2", py::vectorize(f1_orig2));
+  m.def("f1_orig2_der1", py::vectorize(f1_orig2_der1));
+  m.def("f1_orig2_der2", py::vectorize(f1_orig2_der2));
+  m.def("f1_exp2", py::vectorize(f1_exp2));
+  m.def("f1_exp2_der1", py::vectorize(f1_exp2_der1));
+  m.def("f1_exp2_der2", py::vectorize(f1_exp2_der2));
 }
```

### Comparing `servalcat-0.4.15/src/refine.cpp` & `servalcat-0.4.24/src/refine.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 // Author: "Keitaro Yamashita, Garib N. Murshudov"
 // MRC Laboratory of Molecular Biology
 
 #include "refine/geom.hpp"    // for Geometry
 #include "refine/ll.hpp"      // for LL
 #include "refine/cgsolve.hpp" // for CgSolve
 #include <gemmi/it92.hpp>
+#include <gemmi/neutron92.hpp>
 #include <gemmi/monlib.hpp>
 #include <gemmi/unitcell.hpp>
 #include <gemmi/model.hpp>
 
 #include <pybind11/stl.h>
 #include <pybind11/stl_bind.h>
 #include <pybind11/numpy.h>
@@ -361,14 +362,86 @@
           zs.push_back(z);
           types.push_back(restr->type);
         }
       }
       return py::dict("atom1"_a=atom1, "atom2"_a=atom2, "value"_a=values,
                       "ideal"_a=ideals, "z"_a=zs, "type"_a=types);
     }, py::arg("min_z"))
+    .def("per_atom_score", [](const Geometry::Reporting& self, int n_atoms,
+                              bool use_nucleus, const std::string& metric) {
+      if (metric != "max" && metric != "mean" && metric != "sum")
+        gemmi::fail("invalid metric");
+      const int imet = metric == "max" ? 0 : metric == "sum" ? 1 : 2;
+      std::vector<std::vector<double>> ret(7);
+      std::vector<std::vector<int>> num(7);
+      for (auto& v : ret)
+        v.assign(n_atoms, 0.);
+      for (auto& v : num)
+        v.assign(n_atoms, 0);
+
+      auto add_residual = [&](int idx, int i, double x) {
+        if (i < 0 || i >= n_atoms) gemmi::fail("invalid atom index");
+        if (imet == 0) // max
+          ret[idx][i] = std::max(ret[idx][i], std::abs(x));
+        else if (imet == 1) // sum
+          ret[idx][i] += std::abs(x);
+        else { // mean
+          ret[idx][i] += gemmi::sq(x);
+          num[idx][i] += 1;
+        }
+      };
+      auto add = [&](int i, double x, int idx) {
+        add_residual(0, i, x); // total
+        add_residual(idx, i, x);
+      };
+
+      for (const auto& t : self.bonds) { // check restr->type?
+        const auto& restr = std::get<0>(t);
+        const auto& val = std::get<1>(t);
+        const double sigma = use_nucleus ? val->sigma_nucleus : val->sigma;
+        for (const auto& a : restr->atoms)
+          add(a->serial - 1, std::get<2>(t) / sigma, 1);
+      }
+      for (const auto& t : self.angles) {
+        const auto& restr = std::get<0>(t);
+        const auto& val = std::get<1>(t);
+        for (const auto& a : restr->atoms)
+          add(a->serial - 1, std::get<2>(t) / val->sigma, 2);
+      }
+      for (const auto& t : self.torsions) {
+        const auto& restr = std::get<0>(t);
+        const auto& val = std::get<1>(t);
+        for (const auto& a : restr->atoms)
+          add(a->serial - 1, std::get<2>(t) / val->sigma, 3);
+      }
+      for (const auto& t : self.chirs) {
+        const auto& restr = std::get<0>(t);
+        for (const auto& a : restr->atoms)
+          add(a->serial - 1, std::get<1>(t) / restr->sigma, 4);
+      }
+      for (const auto& t : self.planes) {
+        const auto& restr = std::get<0>(t);
+        for (size_t i = 0; i < restr->atoms.size(); ++i)
+          add(restr->atoms[i]->serial - 1, std::get<1>(t)[i] / restr->sigma, 5);
+      }
+      // include stac?
+      for (const auto& t : self.vdws) {
+        const auto& restr = std::get<0>(t);
+        for (const auto& a : restr->atoms)
+          add(a->serial - 1, std::get<1>(t) / restr->sigma, 6);
+      }
+      if (imet == 2) { // mean
+        for (size_t j = 0; j < ret.size(); ++j)
+          for (size_t i = 0; i < ret[j].size(); ++i)
+            ret[j][i] = std::sqrt(ret[j][i] / num[j][i]);
+      }
+      return py::dict("total"_a=ret[0], "bonds"_a=ret[1], "angles"_a=ret[2],
+                      "torsions"_a=ret[3], "chirs"_a=ret[4], "planes"_a=ret[5],
+                      "vdws"_a=ret[6]);
+    })
     ;
   py::class_<Geometry::Bond> bond(geom, "Bond");
   py::class_<Geometry::Angle> angle(geom, "Angle");
   py::class_<Geometry::Torsion> torsion(geom, "Torsion");
   py::class_<Geometry::Chirality> chirality(geom, "Chirality");
   py::class_<Geometry::Plane> plane(geom, "Plane");
   py::class_<Geometry::Vdw> vdw(geom, "Vdw");
@@ -451,14 +524,15 @@
     .def_readwrite("angle", &Geometry::Stacking::angle)
     .def_readwrite("sd_angle", &Geometry::Stacking::sd_angle)
     .def_readwrite("planes", &Geometry::Stacking::planes)
     ;
   vdw
     .def(py::init<gemmi::Atom*,gemmi::Atom*>())
     .def("set_image", &Geometry::Vdw::set_image)
+    .def("same_asu", &Geometry::Vdw::same_asu)
     .def_readwrite("type", &Geometry::Vdw::type)
     .def_readwrite("value", &Geometry::Vdw::value)
     .def_readwrite("sigma", &Geometry::Vdw::sigma)
     .def_readwrite("sym_idx", &Geometry::Vdw::sym_idx)
     .def_readwrite("pbc_shift", &Geometry::Vdw::pbc_shift)
     .def_readwrite("atoms", &Geometry::Vdw::atoms)
     ;
@@ -524,14 +598,15 @@
     .def_readwrite("hbond_dinc_ah", &Geometry::hbond_dinc_ah)
     .def_readwrite("dinc_torsion_o", &Geometry::dinc_torsion_o)
     .def_readwrite("dinc_torsion_n", &Geometry::dinc_torsion_n)
     .def_readwrite("dinc_torsion_c", &Geometry::dinc_torsion_c)
     .def_readwrite("dinc_torsion_all", &Geometry::dinc_torsion_all)
     .def_readwrite("dinc_dummy", &Geometry::dinc_dummy)
     .def_readwrite("vdw_sdi_dummy", &Geometry::vdw_sdi_dummy)
+    .def_readwrite("max_vdw_radius", &Geometry::max_vdw_radius)
     // ADP restraint parameters
     .def_readwrite("adpr_max_dist", &Geometry::adpr_max_dist)
     .def_readwrite("adpr_d_power", &Geometry::adpr_d_power)
     .def_readwrite("adpr_exp_fac", &Geometry::adpr_exp_fac)
     // jelly body parameters
     .def_readwrite("ridge_dmax", &Geometry::ridge_dmax)
     .def_readwrite("ridge_sigma", &Geometry::ridge_sigma)
@@ -548,16 +623,19 @@
     ;
   py::class_<LL>(m, "LL")
     .def(py::init<const gemmi::Structure &, bool, bool, int, bool>(),
          py::arg("st"), py::arg("mott_bethe"),
          py::arg("refine_xyz"), py::arg("adp_mode"), py::arg("refine_h"))
     .def("set_ncs", &LL::set_ncs)
     .def("calc_grad_it92", &LL::calc_grad<gemmi::IT92<double>>)
+    .def("calc_grad_n92", &LL::calc_grad<gemmi::Neutron92<double>>)
     .def("make_fisher_table_diag_fast_it92", &LL::make_fisher_table_diag_fast<gemmi::IT92<double>>)
+    .def("make_fisher_table_diag_fast_n92", &LL::make_fisher_table_diag_fast<gemmi::Neutron92<double>>)
     .def("fisher_diag_from_table_it92", &LL::fisher_diag_from_table<gemmi::IT92<double>>)
+    .def("fisher_diag_from_table_n92", &LL::fisher_diag_from_table<gemmi::Neutron92<double>>)
     .def("spec_correction", &LL::spec_correction,
          py::arg("specials"), py::arg("alpha")=1e-3, py::arg("use_rr")=true)
     .def_property_readonly("fisher_spmat", &LL::make_spmat)
     .def_readonly("table_bs", &LL::table_bs)
     .def_readonly("pp1", &LL::pp1)
     .def_readonly("bb", &LL::bb)
     .def_readonly("aa", &LL::aa)
```

