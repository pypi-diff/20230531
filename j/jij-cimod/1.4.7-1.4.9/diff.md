# Comparing `tmp/jij_cimod-1.4.7.tar.gz` & `tmp/jij_cimod-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jij_cimod-1.4.7.tar", last modified: Tue Jun 28 00:10:03 2022, max compression
+gzip compressed data, was "jij_cimod-1.4.9.tar", last modified: Tue Jun 28 04:21:09 2022, max compression
```

## Comparing `jij_cimod-1.4.7.tar` & `jij_cimod-1.4.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 00:10:03.233691 jij_cimod-1.4.7/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)     1719 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/.gitattribute
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/.reviewdog.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5447 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8411 2022-06-28 00:10:03.233691 jij_cimod-1.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7331 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 00:10:03.229690 jij_cimod-1.4.7/cimod/
--rw-r--r--   0 runner    (1001) docker     (121)     1670 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cimod/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cimod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-06-28 00:10:02.000000 jij_cimod-1.4.7/cimod/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3168 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cimod/main.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    12692 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cimod/main.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 00:10:03.229690 jij_cimod-1.4.7/cimod/model/
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cimod/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31154 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cimod/model/binary_polynomial_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    13751 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cimod/model/binary_quadratic_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 00:10:03.229690 jij_cimod-1.4.7/cimod/model/legacy/
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cimod/model/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14098 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cimod/model/legacy/binary_quadratic_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 00:10:03.233691 jij_cimod-1.4.7/cimod/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cimod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      982 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cimod/utils/decolator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cimod/utils/response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cimod/vartype.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 00:10:03.233691 jij_cimod-1.4.7/cmake/
--rw-r--r--   0 runner    (1001) docker     (121)     5228 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cmake/FindGcov.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    12711 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cmake/FindLcov.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     9023 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cmake/Findcodecov.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cmake/GenerateDocs.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1937 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cmake/PythonAutoDetectOSX.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/cmake/llvm-cov-wrapper
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 00:10:03.233691 jij_cimod-1.4.7/external/
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/external/eigen.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/external/googletest.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/external/json.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/external/pybind11-json.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/external/pybind11.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 00:10:03.233691 jij_cimod-1.4.7/jij_cimod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8411 2022-06-28 00:10:02.000000 jij_cimod-1.4.7/jij_cimod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-06-28 00:10:03.000000 jij_cimod-1.4.7/jij_cimod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 00:10:02.000000 jij_cimod-1.4.7/jij_cimod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 00:10:02.000000 jij_cimod-1.4.7/jij_cimod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-06-28 00:10:03.000000 jij_cimod-1.4.7/jij_cimod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-28 00:10:03.000000 jij_cimod-1.4.7/jij_cimod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3303 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-06-28 00:10:03.237691 jij_cimod-1.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 00:10:03.233691 jij_cimod-1.4.7/src/
--rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    44450 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/src/binary_polynomial_model.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    66766 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/src/binary_quadratic_model.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    41145 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/src/binary_quadratic_model_dict.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/src/disable_eigen_warning.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/src/hash.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/src/json.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     4662 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/src/utilities.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/src/vartypes.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 00:10:03.233691 jij_cimod-1.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    56485 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/tests/test.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/tests/test_0_basic.py
--rw-r--r--   0 runner    (1001) docker     (121)    30862 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/tests/test_bqm.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    12348 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/tests/test_legacy_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    74844 2022-06-28 00:09:37.000000 jij_cimod-1.4.7/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.273041 jij_cimod-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)     1719 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/.gitattribute
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/.reviewdog.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     5447 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     8411 2022-06-28 04:21:09.273041 jij_cimod-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7331 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.261040 jij_cimod-1.4.9/cimod/
+-rw-r--r--   0 runner    (1001) docker     (121)     1670 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-06-28 04:21:08.000000 jij_cimod-1.4.9/cimod/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3168 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    12692 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/main.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.261040 jij_cimod-1.4.9/cimod/model/
+-rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31154 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/model/binary_polynomial_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13751 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/model/binary_quadratic_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.265040 jij_cimod-1.4.9/cimod/model/legacy/
+-rw-r--r--   0 runner    (1001) docker     (121)      758 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/model/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14098 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/model/legacy/binary_quadratic_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.265040 jij_cimod-1.4.9/cimod/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      803 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      982 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/utils/decolator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/utils/response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/vartype.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.265040 jij_cimod-1.4.9/cmake/
+-rw-r--r--   0 runner    (1001) docker     (121)     5228 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cmake/FindGcov.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    12711 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cmake/FindLcov.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     9023 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cmake/Findcodecov.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cmake/GenerateDocs.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1937 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cmake/PythonAutoDetectOSX.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cmake/llvm-cov-wrapper
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.265040 jij_cimod-1.4.9/external/
+-rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/external/eigen.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      699 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/external/googletest.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      756 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/external/json.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/external/pybind11-json.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/external/pybind11.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.269040 jij_cimod-1.4.9/jij_cimod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8411 2022-06-28 04:21:08.000000 jij_cimod-1.4.9/jij_cimod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-06-28 04:21:09.000000 jij_cimod-1.4.9/jij_cimod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 04:21:08.000000 jij_cimod-1.4.9/jij_cimod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 04:21:08.000000 jij_cimod-1.4.9/jij_cimod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-06-28 04:21:09.000000 jij_cimod-1.4.9/jij_cimod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-28 04:21:09.000000 jij_cimod-1.4.9/jij_cimod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3303 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-06-28 04:21:09.273041 jij_cimod-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.269040 jij_cimod-1.4.9/src/
+-rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    44450 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/src/binary_polynomial_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    66766 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/src/binary_quadratic_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    41145 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/src/binary_quadratic_model_dict.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/src/disable_eigen_warning.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/src/hash.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)      639 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/src/json.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4662 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/src/utilities.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/src/vartypes.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.273041 jij_cimod-1.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      646 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    56485 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/tests/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/tests/test_0_basic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30862 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/tests/test_bqm.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    12348 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/tests/test_legacy_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    74844 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/tests/test_model.py
```

### Comparing `jij_cimod-1.4.7/.gitattribute` & `jij_cimod-1.4.9/.gitattribute`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/CMakeLists.txt` & `jij_cimod-1.4.9/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/LICENSE` & `jij_cimod-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/MANIFEST.in` & `jij_cimod-1.4.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/PKG-INFO` & `jij_cimod-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jij_cimod
-Version: 1.4.7
+Version: 1.4.9
 Summary: C++ library for a binary (and polynomial) quadratic model.
 Home-page: https://www.openjij.org
 Author: Jij Inc.
 Author-email: info@j-ij.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/OpenJij/cimod
 Project-URL: Documentation, https://cimod.openjij.org
```

### Comparing `jij_cimod-1.4.7/README.md` & `jij_cimod-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cimod/CMakeLists.txt` & `jij_cimod-1.4.9/cimod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cimod/__init__.py` & `jij_cimod-1.4.9/cimod/__init__.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cimod/main.cpp` & `jij_cimod-1.4.9/cimod/main.cpp`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cimod/main.hpp` & `jij_cimod-1.4.9/cimod/main.hpp`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cimod/model/__init__.py` & `jij_cimod-1.4.9/cimod/model/__init__.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cimod/model/binary_polynomial_model.py` & `jij_cimod-1.4.9/cimod/model/binary_polynomial_model.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cimod/model/binary_quadratic_model.py` & `jij_cimod-1.4.9/cimod/model/binary_quadratic_model.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cimod/model/legacy/__init__.py` & `jij_cimod-1.4.9/cimod/model/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cimod/model/legacy/binary_quadratic_model.py` & `jij_cimod-1.4.9/cimod/model/legacy/binary_quadratic_model.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cimod/utils/__init__.py` & `jij_cimod-1.4.9/cimod/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cimod/utils/decolator.py` & `jij_cimod-1.4.9/cimod/utils/decolator.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cimod/utils/response.py` & `jij_cimod-1.4.9/cimod/utils/response.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cimod/vartype.py` & `jij_cimod-1.4.9/cimod/vartype.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cmake/FindGcov.cmake` & `jij_cimod-1.4.9/cmake/FindGcov.cmake`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cmake/FindLcov.cmake` & `jij_cimod-1.4.9/cmake/FindLcov.cmake`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cmake/Findcodecov.cmake` & `jij_cimod-1.4.9/cmake/Findcodecov.cmake`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cmake/GenerateDocs.cmake` & `jij_cimod-1.4.9/cmake/GenerateDocs.cmake`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cmake/PythonAutoDetectOSX.cmake` & `jij_cimod-1.4.9/cmake/PythonAutoDetectOSX.cmake`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/cmake/llvm-cov-wrapper` & `jij_cimod-1.4.9/cmake/llvm-cov-wrapper`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/external/eigen.cmake` & `jij_cimod-1.4.9/external/eigen.cmake`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/external/googletest.cmake` & `jij_cimod-1.4.9/external/googletest.cmake`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/external/json.cmake` & `jij_cimod-1.4.9/external/json.cmake`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/jij_cimod.egg-info/PKG-INFO` & `jij_cimod-1.4.9/jij_cimod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jij-cimod
-Version: 1.4.7
+Version: 1.4.9
 Summary: C++ library for a binary (and polynomial) quadratic model.
 Home-page: https://www.openjij.org
 Author: Jij Inc.
 Author-email: info@j-ij.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/OpenJij/cimod
 Project-URL: Documentation, https://cimod.openjij.org
```

### Comparing `jij_cimod-1.4.7/jij_cimod.egg-info/SOURCES.txt` & `jij_cimod-1.4.9/jij_cimod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/pyproject.toml` & `jij_cimod-1.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/setup.cfg` & `jij_cimod-1.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/setup.py` & `jij_cimod-1.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/src/CMakeLists.txt` & `jij_cimod-1.4.9/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/src/binary_polynomial_model.hpp` & `jij_cimod-1.4.9/src/binary_polynomial_model.hpp`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/src/binary_quadratic_model.hpp` & `jij_cimod-1.4.9/src/binary_quadratic_model.hpp`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/src/binary_quadratic_model_dict.hpp` & `jij_cimod-1.4.9/src/binary_quadratic_model_dict.hpp`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/src/disable_eigen_warning.hpp` & `jij_cimod-1.4.9/src/disable_eigen_warning.hpp`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/src/hash.hpp` & `jij_cimod-1.4.9/src/hash.hpp`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/src/json.hpp` & `jij_cimod-1.4.9/src/json.hpp`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/src/utilities.hpp` & `jij_cimod-1.4.9/src/utilities.hpp`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/src/vartypes.hpp` & `jij_cimod-1.4.9/src/vartypes.hpp`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/tests/CMakeLists.txt` & `jij_cimod-1.4.9/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/tests/__init__.py` & `jij_cimod-1.4.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/tests/test.cpp` & `jij_cimod-1.4.9/tests/test.cpp`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/tests/test_0_basic.py` & `jij_cimod-1.4.9/tests/test_0_basic.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/tests/test_bqm.hpp` & `jij_cimod-1.4.9/tests/test_bqm.hpp`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/tests/test_legacy_model.py` & `jij_cimod-1.4.9/tests/test_legacy_model.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.7/tests/test_model.py` & `jij_cimod-1.4.9/tests/test_model.py`

 * *Files identical despite different names*

