# Comparing `tmp/lincs-0.3.5.tar.gz` & `tmp/lincs-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lincs-0.3.5.tar", last modified: Wed May 31 09:44:20 2023, max compression
+gzip compressed data, was "lincs-0.3.6.tar", last modified: Wed May 31 14:14:17 2023, max compression
```

## Comparing `lincs-0.3.5.tar` & `lincs-0.3.6.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/
--rw-rw-r--   0 user      (1002) user      (1002)    35149 2023-05-12 12:03:36.000000 lincs-0.3.5/COPYING
--rw-rw-r--   0 user      (1002) user      (1002)     7652 2023-05-12 12:04:16.000000 lincs-0.3.5/COPYING.LESSER
--rw-rw-r--   0 user      (1002) user      (1002)      104 2023-05-12 11:51:00.000000 lincs-0.3.5/MANIFEST.in
--rw-r--r--   0 user      (1002) user      (1002)    17770 2023-05-31 09:44:20.783313 lincs-0.3.5/PKG-INFO
--rw-rw-r--   0 user      (1002) user      (1002)    17129 2023-05-31 09:28:18.000000 lincs-0.3.5/README.rst
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/lincs/
--rw-rw-r--   0 user      (1002) user      (1002)      796 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/__init__.py
--rw-rw-r--   0 user      (1002) user      (1002)      170 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/__main__.py
--rw-rw-r--   0 user      (1002) user      (1002)    21977 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/command_line_interface.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/lincs/liblincs/
--rw-rw-r--   0 user      (1002) user      (1002)     1610 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/classification.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      368 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/classification.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    10039 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/generation.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1042 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/generation.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/lincs/liblincs/io/
--rw-rw-r--   0 user      (1002) user      (1002)     2461 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/io/alternatives.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1004 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/io/alternatives.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     2582 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/io/domain.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1886 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/io/domain.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     1875 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/io/model.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1640 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/io/model.hpp
--rw-rw-r--   0 user      (1002) user      (1002)       53 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/io.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      186 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/io.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/lincs/liblincs/learning/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.779313 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/
--rw-rw-r--   0 user      (1002) user      (1002)     9494 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     2125 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/
--rw-rw-r--   0 user      (1002) user      (1002)     4406 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1265 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/
--rw-rw-r--   0 user      (1002) user      (1002)     4495 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      922 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/
--rw-rw-r--   0 user      (1002) user      (1002)      244 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      682 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     6757 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     3486 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     1727 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      551 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    15121 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/liblincs_module.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      245 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/lincs.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     2963 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/median-and-max.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      751 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/median-and-max.hpp
--rw-rw-r--   0 user      (1002) user      (1002)      776 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/randomness-utils.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1539 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/randomness-utils.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    10418 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs_module_tests.py
--rw-rw-r--   0 user      (1002) user      (1002)      793 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/visualization.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/lincs.egg-info/
--rw-r--r--   0 user      (1002) user      (1002)    17770 2023-05-31 09:44:20.000000 lincs-0.3.5/lincs.egg-info/PKG-INFO
--rw-r--r--   0 user      (1002) user      (1002)     1875 2023-05-31 09:44:20.000000 lincs-0.3.5/lincs.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1002) user      (1002)        1 2023-05-31 09:44:20.000000 lincs-0.3.5/lincs.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1002) user      (1002)       60 2023-05-31 09:44:20.000000 lincs-0.3.5/lincs.egg-info/entry_points.txt
--rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-31 09:44:20.000000 lincs-0.3.5/lincs.egg-info/requires.txt
--rw-r--r--   0 user      (1002) user      (1002)       15 2023-05-31 09:44:20.000000 lincs-0.3.5/lincs.egg-info/top_level.txt
--rw-rw-r--   0 user      (1002) user      (1002)       61 2023-05-12 11:51:00.000000 lincs-0.3.5/requirements.txt
--rw-r--r--   0 user      (1002) user      (1002)       38 2023-05-31 09:44:20.783313 lincs-0.3.5/setup.cfg
--rw-rw-r--   0 user      (1002) user      (1002)     2636 2023-05-31 09:44:12.000000 lincs-0.3.5/setup.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 14:14:17.768709 lincs-0.3.6/
+-rw-rw-r--   0 user      (1002) user      (1002)    35149 2023-05-12 12:03:36.000000 lincs-0.3.6/COPYING
+-rw-rw-r--   0 user      (1002) user      (1002)     7652 2023-05-12 12:04:16.000000 lincs-0.3.6/COPYING.LESSER
+-rw-rw-r--   0 user      (1002) user      (1002)      104 2023-05-12 11:51:00.000000 lincs-0.3.6/MANIFEST.in
+-rw-r--r--   0 user      (1002) user      (1002)    17983 2023-05-31 14:14:17.768709 lincs-0.3.6/PKG-INFO
+-rw-rw-r--   0 user      (1002) user      (1002)    17342 2023-05-31 14:14:12.000000 lincs-0.3.6/README.rst
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 14:14:17.764709 lincs-0.3.6/lincs/
+-rw-rw-r--   0 user      (1002) user      (1002)      796 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/__init__.py
+-rw-rw-r--   0 user      (1002) user      (1002)      170 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/__main__.py
+-rw-rw-r--   0 user      (1002) user      (1002)    21977 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/command_line_interface.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 14:14:17.768709 lincs-0.3.6/lincs/liblincs/
+-rw-rw-r--   0 user      (1002) user      (1002)     1610 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/classification.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      368 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/classification.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    10039 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/generation.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1042 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/generation.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 14:14:17.768709 lincs-0.3.6/lincs/liblincs/io/
+-rw-rw-r--   0 user      (1002) user      (1002)     2461 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/io/alternatives.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1004 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/io/alternatives.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2582 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/io/domain.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1886 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/io/domain.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1875 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/io/model.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1640 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/io/model.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)       53 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/io.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      186 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/io.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 14:14:17.768709 lincs-0.3.6/lincs/liblincs/learning/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 14:14:17.764709 lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 14:14:17.768709 lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/
+-rw-rw-r--   0 user      (1002) user      (1002)     9494 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2125 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 14:14:17.768709 lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/
+-rw-rw-r--   0 user      (1002) user      (1002)     4406 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1265 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 14:14:17.768709 lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/
+-rw-rw-r--   0 user      (1002) user      (1002)     4495 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      922 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 14:14:17.768709 lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/
+-rw-rw-r--   0 user      (1002) user      (1002)      244 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      682 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     6757 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     3486 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1727 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/learning.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      551 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/learning.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    15121 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/liblincs_module.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      245 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/lincs.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2963 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/median-and-max.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      751 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/median-and-max.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)      776 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/randomness-utils.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1539 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs/randomness-utils.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    10418 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/liblincs_module_tests.py
+-rw-rw-r--   0 user      (1002) user      (1002)      793 2023-05-12 11:51:00.000000 lincs-0.3.6/lincs/visualization.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 14:14:17.768709 lincs-0.3.6/lincs.egg-info/
+-rw-r--r--   0 user      (1002) user      (1002)    17983 2023-05-31 14:14:17.000000 lincs-0.3.6/lincs.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1002) user      (1002)     1875 2023-05-31 14:14:17.000000 lincs-0.3.6/lincs.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1002) user      (1002)        1 2023-05-31 14:14:17.000000 lincs-0.3.6/lincs.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1002) user      (1002)       60 2023-05-31 14:14:17.000000 lincs-0.3.6/lincs.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-31 14:14:17.000000 lincs-0.3.6/lincs.egg-info/requires.txt
+-rw-r--r--   0 user      (1002) user      (1002)       15 2023-05-31 14:14:17.000000 lincs-0.3.6/lincs.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1002) user      (1002)       61 2023-05-12 11:51:00.000000 lincs-0.3.6/requirements.txt
+-rw-r--r--   0 user      (1002) user      (1002)       38 2023-05-31 14:14:17.768709 lincs-0.3.6/setup.cfg
+-rw-rw-r--   0 user      (1002) user      (1002)     2636 2023-05-31 14:14:00.000000 lincs-0.3.6/setup.py
```

### Comparing `lincs-0.3.5/COPYING` & `lincs-0.3.6/COPYING`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/COPYING.LESSER` & `lincs-0.3.6/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/PKG-INFO` & `lincs-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.3.5
+Version: 0.3.6
 Summary: Learn and Infer Non Compensatory Sortings
 Home-page: https://github.com/MICS-Lab/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -25,15 +25,19 @@
     - on GitHub (https://github.com/mics-lab/lincs/)
     - on PyPI after publication of the package (https://pypi.org/project/lincs/)
     - on GitHub Pages (https://mics-lab.github.io/lincs/)
     So when you change it, take care to check all those places.
 
 *lincs* is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
 
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.3.5/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.3.5/COPYING.LESSER>`_.
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.3.6/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.3.6/COPYING.LESSER>`_.
+It's available on the `Python package index <https://pypi.org/project/lincs/>`_.
+Its `documentation <http://mics-lab.github.io/lincs/>`_
+and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
+
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
 Questions? Remarks? Bugs? Want to contribute? Open `an issue <https://github.com/MICS-Lab/lincs/issues>`_ or `a discussion <https://github.com/MICS-Lab/lincs/discussions>`_!
 
 
 Contributors and previous work
@@ -328,15 +332,15 @@
 
 .. EXTEND command-line-example/run.sh
     cp model.png ../../..
 .. STOP
 
 It should output something like:
 
-.. image:: https://github.com/MICS-Lab/lincs/raw/v0.3.5/model.png
+.. image:: https://github.com/MICS-Lab/lincs/raw/v0.3.6/model.png
     :alt: Model visualization
     :align: center
 
 .. EXTEND command-line-example/run.sh
 
 And finally generate a set of classified alternatives (@todo Link to concepts and file formats)::
 
@@ -376,15 +380,15 @@
 
 .. EXTEND command-line-example/run.sh
     cp alternatives.png ../../..
 .. STOP
 
 It should output something like:
 
-.. image:: https://github.com/MICS-Lab/lincs/raw/v0.3.5/alternatives.png
+.. image:: https://github.com/MICS-Lab/lincs/raw/v0.3.6/alternatives.png
     :alt: Alternatives visualization
     :align: center
 
 @todo Improve how this graph looks:
 
 - display categories as stacked solid colors
 - display alternatives in a color that matches their assigned category
```

### Comparing `lincs-0.3.5/README.rst` & `lincs-0.3.6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,18 @@
     - on PyPI after publication of the package (https://pypi.org/project/lincs/)
     - on GitHub Pages (https://mics-lab.github.io/lincs/)
     So when you change it, take care to check all those places.
 
 *lincs* is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
 
 *lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <COPYING>`_ and `COPYING.LESSER <COPYING.LESSER>`_.
+It's available on the `Python package index <https://pypi.org/project/lincs/>`_.
+Its `documentation <http://mics-lab.github.io/lincs/>`_
+and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
+
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
 Questions? Remarks? Bugs? Want to contribute? Open `an issue <https://github.com/MICS-Lab/lincs/issues>`_ or `a discussion <https://github.com/MICS-Lab/lincs/discussions>`_!
 
 
 Contributors and previous work
```

### Comparing `lincs-0.3.5/lincs/__init__.py` & `lincs-0.3.6/lincs/__init__.py`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/command_line_interface.py` & `lincs-0.3.6/lincs/command_line_interface.py`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/classification.cpp` & `lincs-0.3.6/lincs/liblincs/classification.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/generation.cpp` & `lincs-0.3.6/lincs/liblincs/generation.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/generation.hpp` & `lincs-0.3.6/lincs/liblincs/generation.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/io/alternatives.cpp` & `lincs-0.3.6/lincs/liblincs/io/alternatives.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/io/alternatives.hpp` & `lincs-0.3.6/lincs/liblincs/io/alternatives.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/io/domain.cpp` & `lincs-0.3.6/lincs/liblincs/io/domain.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/io/domain.hpp` & `lincs-0.3.6/lincs/liblincs/io/domain.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/io/model.cpp` & `lincs-0.3.6/lincs/liblincs/io/model.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/io/model.hpp` & `lincs-0.3.6/lincs/liblincs/io/model.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.cpp` & `lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.hpp` & `lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp` & `lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp` & `lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.cpp` & `lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.hpp` & `lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp` & `lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp` & `lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp` & `lincs-0.3.6/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/learning.cpp` & `lincs-0.3.6/lincs/liblincs/learning.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/learning.hpp` & `lincs-0.3.6/lincs/liblincs/learning.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/liblincs_module.cpp` & `lincs-0.3.6/lincs/liblincs/liblincs_module.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/median-and-max.cpp` & `lincs-0.3.6/lincs/liblincs/median-and-max.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/median-and-max.hpp` & `lincs-0.3.6/lincs/liblincs/median-and-max.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/randomness-utils.cpp` & `lincs-0.3.6/lincs/liblincs/randomness-utils.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs/randomness-utils.hpp` & `lincs-0.3.6/lincs/liblincs/randomness-utils.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/liblincs_module_tests.py` & `lincs-0.3.6/lincs/liblincs_module_tests.py`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs/visualization.py` & `lincs-0.3.6/lincs/visualization.py`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/lincs.egg-info/PKG-INFO` & `lincs-0.3.6/lincs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.3.5
+Version: 0.3.6
 Summary: Learn and Infer Non Compensatory Sortings
 Home-page: https://github.com/MICS-Lab/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -25,15 +25,19 @@
     - on GitHub (https://github.com/mics-lab/lincs/)
     - on PyPI after publication of the package (https://pypi.org/project/lincs/)
     - on GitHub Pages (https://mics-lab.github.io/lincs/)
     So when you change it, take care to check all those places.
 
 *lincs* is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
 
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.3.5/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.3.5/COPYING.LESSER>`_.
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.3.6/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.3.6/COPYING.LESSER>`_.
+It's available on the `Python package index <https://pypi.org/project/lincs/>`_.
+Its `documentation <http://mics-lab.github.io/lincs/>`_
+and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
+
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
 Questions? Remarks? Bugs? Want to contribute? Open `an issue <https://github.com/MICS-Lab/lincs/issues>`_ or `a discussion <https://github.com/MICS-Lab/lincs/discussions>`_!
 
 
 Contributors and previous work
@@ -328,15 +332,15 @@
 
 .. EXTEND command-line-example/run.sh
     cp model.png ../../..
 .. STOP
 
 It should output something like:
 
-.. image:: https://github.com/MICS-Lab/lincs/raw/v0.3.5/model.png
+.. image:: https://github.com/MICS-Lab/lincs/raw/v0.3.6/model.png
     :alt: Model visualization
     :align: center
 
 .. EXTEND command-line-example/run.sh
 
 And finally generate a set of classified alternatives (@todo Link to concepts and file formats)::
 
@@ -376,15 +380,15 @@
 
 .. EXTEND command-line-example/run.sh
     cp alternatives.png ../../..
 .. STOP
 
 It should output something like:
 
-.. image:: https://github.com/MICS-Lab/lincs/raw/v0.3.5/alternatives.png
+.. image:: https://github.com/MICS-Lab/lincs/raw/v0.3.6/alternatives.png
     :alt: Alternatives visualization
     :align: center
 
 @todo Improve how this graph looks:
 
 - display categories as stacked solid colors
 - display alternatives in a color that matches their assigned category
```

### Comparing `lincs-0.3.5/lincs.egg-info/SOURCES.txt` & `lincs-0.3.6/lincs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lincs-0.3.5/setup.py` & `lincs-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2023 Vincent Jacques
 
 import glob
 import setuptools
 
 
-version = "0.3.5"
+version = "0.3.6"
 
 with open("README.rst") as f:
     long_description = f.read()
 for image in ["model", "alternatives"]:
     long_description = long_description.replace(f".. image:: {image}.png", f".. image:: https://github.com/MICS-Lab/lincs/raw/v{version}/{image}.png")
 for file in ["COPYING", "COPYING.LESSER"]:
     long_description = long_description.replace(f" <{file}>`_", f" <https://github.com/MICS-Lab/lincs/blob/v{version}/{file}>`_")
```

