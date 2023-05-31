# Comparing `tmp/lincs-0.3.3.tar.gz` & `tmp/lincs-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lincs-0.3.3.tar", last modified: Fri May 12 12:41:08 2023, max compression
+gzip compressed data, was "lincs-0.3.5.tar", last modified: Wed May 31 09:44:20 2023, max compression
```

## Comparing `lincs-0.3.3.tar` & `lincs-0.3.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:41:08.308190 lincs-0.3.3/
--rw-rw-r--   0 user      (1002) user      (1002)    35149 2023-05-12 12:03:36.000000 lincs-0.3.3/COPYING
--rw-rw-r--   0 user      (1002) user      (1002)     7652 2023-05-12 12:04:16.000000 lincs-0.3.3/COPYING.LESSER
--rw-rw-r--   0 user      (1002) user      (1002)      104 2023-05-12 11:51:00.000000 lincs-0.3.3/MANIFEST.in
--rw-r--r--   0 user      (1002) user      (1002)    17437 2023-05-12 12:41:08.308190 lincs-0.3.3/PKG-INFO
--rw-rw-r--   0 user      (1002) user      (1002)    16460 2023-05-12 12:10:40.000000 lincs-0.3.3/README.md
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:41:08.304190 lincs-0.3.3/lincs/
--rw-rw-r--   0 user      (1002) user      (1002)      796 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/__init__.py
--rw-rw-r--   0 user      (1002) user      (1002)      170 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/__main__.py
--rw-rw-r--   0 user      (1002) user      (1002)    21977 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/command_line_interface.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:41:08.308190 lincs-0.3.3/lincs/liblincs/
--rw-rw-r--   0 user      (1002) user      (1002)     1610 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/classification.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      368 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/classification.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    10039 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/generation.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1042 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/generation.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:41:08.308190 lincs-0.3.3/lincs/liblincs/io/
--rw-rw-r--   0 user      (1002) user      (1002)     2461 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/io/alternatives.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1004 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/io/alternatives.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     2582 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/io/domain.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1886 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/io/domain.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     1875 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/io/model.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1640 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/io/model.hpp
--rw-rw-r--   0 user      (1002) user      (1002)       53 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/io.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      186 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/io.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:41:08.308190 lincs-0.3.3/lincs/liblincs/learning/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:41:08.304190 lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:41:08.308190 lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/
--rw-rw-r--   0 user      (1002) user      (1002)     9494 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     2125 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:41:08.308190 lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/
--rw-rw-r--   0 user      (1002) user      (1002)     4406 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1265 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:41:08.308190 lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/
--rw-rw-r--   0 user      (1002) user      (1002)     4495 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      922 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:41:08.308190 lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/
--rw-rw-r--   0 user      (1002) user      (1002)      244 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      682 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     6757 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     3486 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     1727 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/learning.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      551 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/learning.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    15121 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/liblincs_module.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      245 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/lincs.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     2963 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/median-and-max.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      751 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/median-and-max.hpp
--rw-rw-r--   0 user      (1002) user      (1002)      776 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/randomness-utils.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1539 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs/randomness-utils.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    10418 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/liblincs_module_tests.py
--rw-rw-r--   0 user      (1002) user      (1002)      793 2023-05-12 11:51:00.000000 lincs-0.3.3/lincs/visualization.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-12 12:41:08.304190 lincs-0.3.3/lincs.egg-info/
--rw-r--r--   0 user      (1002) user      (1002)    17437 2023-05-12 12:41:08.000000 lincs-0.3.3/lincs.egg-info/PKG-INFO
--rw-r--r--   0 user      (1002) user      (1002)     1874 2023-05-12 12:41:08.000000 lincs-0.3.3/lincs.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1002) user      (1002)        1 2023-05-12 12:41:08.000000 lincs-0.3.3/lincs.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1002) user      (1002)       60 2023-05-12 12:41:08.000000 lincs-0.3.3/lincs.egg-info/entry_points.txt
--rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-12 12:41:08.000000 lincs-0.3.3/lincs.egg-info/requires.txt
--rw-r--r--   0 user      (1002) user      (1002)       15 2023-05-12 12:41:08.000000 lincs-0.3.3/lincs.egg-info/top_level.txt
--rw-rw-r--   0 user      (1002) user      (1002)       61 2023-05-12 11:51:00.000000 lincs-0.3.3/requirements.txt
--rw-r--r--   0 user      (1002) user      (1002)       38 2023-05-12 12:41:08.308190 lincs-0.3.3/setup.cfg
--rw-rw-r--   0 user      (1002) user      (1002)     2493 2023-05-12 12:40:18.000000 lincs-0.3.3/setup.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/
+-rw-rw-r--   0 user      (1002) user      (1002)    35149 2023-05-12 12:03:36.000000 lincs-0.3.5/COPYING
+-rw-rw-r--   0 user      (1002) user      (1002)     7652 2023-05-12 12:04:16.000000 lincs-0.3.5/COPYING.LESSER
+-rw-rw-r--   0 user      (1002) user      (1002)      104 2023-05-12 11:51:00.000000 lincs-0.3.5/MANIFEST.in
+-rw-r--r--   0 user      (1002) user      (1002)    17770 2023-05-31 09:44:20.783313 lincs-0.3.5/PKG-INFO
+-rw-rw-r--   0 user      (1002) user      (1002)    17129 2023-05-31 09:28:18.000000 lincs-0.3.5/README.rst
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/lincs/
+-rw-rw-r--   0 user      (1002) user      (1002)      796 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/__init__.py
+-rw-rw-r--   0 user      (1002) user      (1002)      170 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/__main__.py
+-rw-rw-r--   0 user      (1002) user      (1002)    21977 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/command_line_interface.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/lincs/liblincs/
+-rw-rw-r--   0 user      (1002) user      (1002)     1610 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/classification.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      368 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/classification.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    10039 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/generation.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1042 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/generation.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/lincs/liblincs/io/
+-rw-rw-r--   0 user      (1002) user      (1002)     2461 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/io/alternatives.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1004 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/io/alternatives.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2582 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/io/domain.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1886 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/io/domain.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1875 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/io/model.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1640 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/io/model.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)       53 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/io.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      186 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/io.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/lincs/liblincs/learning/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.779313 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/
+-rw-rw-r--   0 user      (1002) user      (1002)     9494 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2125 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/
+-rw-rw-r--   0 user      (1002) user      (1002)     4406 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1265 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/
+-rw-rw-r--   0 user      (1002) user      (1002)     4495 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      922 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/
+-rw-rw-r--   0 user      (1002) user      (1002)      244 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      682 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     6757 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     3486 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1727 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      551 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/learning.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    15121 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/liblincs_module.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      245 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/lincs.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2963 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/median-and-max.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      751 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/median-and-max.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)      776 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/randomness-utils.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1539 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs/randomness-utils.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    10418 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/liblincs_module_tests.py
+-rw-rw-r--   0 user      (1002) user      (1002)      793 2023-05-12 11:51:00.000000 lincs-0.3.5/lincs/visualization.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 09:44:20.783313 lincs-0.3.5/lincs.egg-info/
+-rw-r--r--   0 user      (1002) user      (1002)    17770 2023-05-31 09:44:20.000000 lincs-0.3.5/lincs.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1002) user      (1002)     1875 2023-05-31 09:44:20.000000 lincs-0.3.5/lincs.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1002) user      (1002)        1 2023-05-31 09:44:20.000000 lincs-0.3.5/lincs.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1002) user      (1002)       60 2023-05-31 09:44:20.000000 lincs-0.3.5/lincs.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-31 09:44:20.000000 lincs-0.3.5/lincs.egg-info/requires.txt
+-rw-r--r--   0 user      (1002) user      (1002)       15 2023-05-31 09:44:20.000000 lincs-0.3.5/lincs.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1002) user      (1002)       61 2023-05-12 11:51:00.000000 lincs-0.3.5/requirements.txt
+-rw-r--r--   0 user      (1002) user      (1002)       38 2023-05-31 09:44:20.783313 lincs-0.3.5/setup.cfg
+-rw-rw-r--   0 user      (1002) user      (1002)     2636 2023-05-31 09:44:12.000000 lincs-0.3.5/setup.py
```

### Comparing `lincs-0.3.3/COPYING` & `lincs-0.3.5/COPYING`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/COPYING.LESSER` & `lincs-0.3.5/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/PKG-INFO` & `lincs-0.3.5/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-Metadata-Version: 2.1
-Name: lincs
-Version: 0.3.3
-Summary: Learn and Infer Non Compensatory Sortings
-Home-page: https://github.com/MICS-Lab/lincs
-Author: Vincent Jacques
-Author-email: vincent@vincent-jacques.net
-License: LGPLv3
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-License-File: COPYING
-License-File: COPYING.LESSER
+.. Copyright 2023 Vincent Jacques
 
-<!-- Copyright 2023 Vincent Jacques -->
+.. WARNING, this README is rendered to HTML in several places
+    - on GitHub (https://github.com/mics-lab/lincs/)
+    - on PyPI after publication of the package (https://pypi.org/project/lincs/)
+    - on GitHub Pages (https://mics-lab.github.io/lincs/)
+    So when you change it, take care to check all those places.
 
 *lincs* is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
 
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files [COPYING](https://github.com/MICS-Lab/lincs/blob/v0.3.3/COPYING) and [COPYING.LESSER](https://github.com/MICS-Lab/lincs/blob/v0.3.3/COPYING.LESSER).
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <COPYING>`_ and `COPYING.LESSER <COPYING.LESSER>`_.
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
-Questions? Remarks? Bugs? Want to contribute? Open [an issue](https://github.com/MICS-Lab/lincs/issues) or [a discussion](https://github.com/MICS-Lab/lincs/discussions)!
+Questions? Remarks? Bugs? Want to contribute? Open `an issue <https://github.com/MICS-Lab/lincs/issues>`_ or `a discussion <https://github.com/MICS-Lab/lincs/discussions>`_!
 
-# Contributors and previous work
 
-*lincs* is developed by the [MICS](https://mics.centralesupelec.fr/) research team at [CentraleSupélec](https://www.centralesupelec.fr/).
+Contributors and previous work
+==============================
+
+*lincs* is developed by the `MICS <https://mics.centralesupelec.fr/>`_ research team at `CentraleSupélec <https://www.centralesupelec.fr/>`_.
 
 Its main authors are (alphabetical order):
-- [Laurent Cabaret](http://perso.ecp.fr/~cabaretl/) (performance optimization)
-- [Vincent Jacques](https://vincent-jacques.net) (engineering)
-- [Vincent Mousseau](https://www.centralesupelec.fr/fr/2EBDCB86-64A4-4747-96E8-C3066CB61F3D) (domain expertise and project leadership)
+
+- `Laurent Cabaret <https://cabaretl.pages.centralesupelec.fr/>`_ (performance optimization)
+- `Vincent Jacques <https://vincent-jacques.net>`_ (engineering)
+- `Vincent Mousseau <https://www.centralesupelec.fr/fr/2EBDCB86-64A4-4747-96E8-C3066CB61F3D>`_ (domain expertise)
+- `Wassila Ouerdane <https://wassilaouerdane.github.io/>`_ (domain expertise)
 
 It's based on work by:
-- [Olivier Sobrie](http://olivier.sobrie.be/) (The "weights, profiles, breed" learning strategy for MR-Sort models, and the profiles improvement heuristic, developed in his [Ph.D thesis](http://olivier.sobrie.be/papers/phd_2016_sobrie.pdf), and [implemented in Python](https://github.com/oso/pymcda))
-- Emma Dixneuf, Thibault Monsel and Thomas Vindard ([C++ implementation of Sobrie's heuristic](https://github.com/Mostah/fastPL/))
 
-# Project goals
+- `Olivier Sobrie <http://olivier.sobrie.be/>`_ (The "weights, profiles, breed" learning strategy for MR-Sort models, and the profiles improvement heuristic, developed in his `Ph.D thesis <http://olivier.sobrie.be/papers/phd_2016_sobrie.pdf>`_, and `implemented in Python <https://github.com/oso/pymcda>`_)
+- Emma Dixneuf, Thibault Monsel and Thomas Vindard (`C++ implementation of Sobrie's heuristic <https://github.com/Mostah/fastPL/>`_)
+
 
-## Provide MCDA tools usable out of the box
+Project goals
+=============
+
+Provide MCDA tools usable out of the box
+----------------------------------------
 
 You should be able to use *lincs* without being a specialist of MCDA and/or NCS models.
-Just follow the [Get started](#get-started) section below.
+Just follow the `Get started <#get-started>`_ section below.
 
-## Provide a base for developing new MCDA algorithms
+Provide a base for developing new MCDA algorithms
+-------------------------------------------------
 
 *lincs* is designed to be easy to extend with new algorithms of even replace parts of existing algorithms.
 @todo Write doc about that use case.
 
 *linc* also provides a benchmark framework to compare algorithms (@todo Write and document).
 This should make it easier to understand the relative strengths and weaknesses of each algorithm.
 
-# Get started
 
-## Install
+Get started
+===========
+
+Install
+-------
 
-First, you need to install a few dependencies (@todo build binary wheel distributions to make installation easier):
+.. highlight:: shell
+
+.. START install/dependencies.sh
+
+First, you need to install a few dependencies (@todo build binary wheel distributions to make installation easier)::
 
-<!-- START install/dependencies.sh -->
     # System packages
     sudo apt-get install --yes g++ libboost-python-dev python3-dev libyaml-cpp-dev
 
     # CUDA
     sudo apt-key adv --fetch-keys https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2204/x86_64/3bf863cc.pub
     sudo add-apt-repository 'deb https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2204/x86_64/ /'
     sudo apt-get update
@@ -83,41 +83,44 @@
 
     # Header-only libraries
     cd /usr/local/include
     sudo wget https://raw.githubusercontent.com/Neargye/magic_enum/v0.8.2/include/magic_enum.hpp
     sudo wget https://raw.githubusercontent.com/d99kris/rapidcsv/v8.75/src/rapidcsv.h
     sudo wget https://raw.githubusercontent.com/jacquev6/lov-e-cuda/13e45bc/lov-e.hpp
     sudo wget https://raw.githubusercontent.com/doctest/doctest/v2.4.11/doctest/doctest.h
-<!-- STOP -->
 
-<!-- START install/Dockerfile-pre --><!--
+.. STOP
+
+.. START install/Dockerfile-pre
     FROM ubuntu:22.04
 
     RUN apt-get update
 
     RUN DEBIAN_FRONTEND=noninteractive apt-get install --yes \
           sudo wget python3-pip dirmngr gpg-agent software-properties-common
 
     RUN useradd user --create-home
     RUN echo "user ALL=(ALL) NOPASSWD:ALL" > /etc/sudoers.d/user
     USER user
     ENV PATH=$PATH:/home/user/.local/bin
     WORKDIR /home/user
---><!-- STOP -->
 
-<!-- START install/Dockerfile-post --><!--
+.. STOP
+
+.. START install/Dockerfile-post
     WORKDIR /home/user
     # Speed-up build when requirements don't change
     ADD project/requirements.txt .
     RUN pip3 install -r requirements.txt
     ADD --chown=user project /home/user/lincs
     RUN pip3 install ./lincs
---><!-- STOP -->
 
-<!-- START install/run.sh --><!--
+.. STOP
+
+.. START install/run.sh
     set -o errexit
     set -o nounset
     set -o pipefail
     trap 'echo "Error on line $LINENO"' ERR
 
     # Transform the dependencies.sh file into a Dockerfile to benefit from the Docker build cache
     (
@@ -129,81 +132,94 @@
       | sed 's/^RUN cd/WORKDIR/'
       echo
       cat Dockerfile-post
     ) >Dockerfile
 
     mkdir project
     cp -r ../../../{lincs,requirements.txt,setup.py} project
-    touch project/README.md  # No need for the actual readme, so don't bust the Docker cache
+    touch project/README.rst  # No need for the actual readme, so don't bust the Docker cache
 
     docker build . --tag lincs-development--install --quiet >/dev/null
     docker run --rm lincs-development--install lincs --help >/dev/null
---><!-- STOP -->
 
-Finally, *lincs* is available on the [Python Package Index](https://pypi.org/project/lincs/), so `pip install lincs` should finalize the install.
+.. STOP
+
+Finally, *lincs* is available on the `Python Package Index <https://pypi.org/project/lincs/>`_, so ``pip install lincs`` should finalize the install.
 
-## Concepts and files
+Concepts and files
+------------------
 
 *lincs* is based on the following concepts:
 
 - a "domain" describes the objects to be classified (*a.k.a.* the "alternatives"), the criteria used to classify them, and the existing categories they can belong to;
 - a "model" is used to actually assign a category to each alternative, based on the values of the criteria for that alternative;
 - a "classified alternative" is an alternative, with its category.
 
-## Start using *lincs*' command-line interface
-
-The command-line interface is the easiest way to get started with *lincs*, starting with `lincs --help`, which should output something like:
+Start using *lincs*' command-line interface
+-------------------------------------------
 
-<!-- START help/run.sh --><!--
+.. START help/run.sh
     set -o errexit
     set -o nounset
     set -o pipefail
     trap 'echo "Error on line $LINENO"' ERR
 
     lincs --help >actual-help.txt
     diff expected-help.txt actual-help.txt
---><!-- STOP -->
+.. STOP
+
+.. START help/expected-help.txt
+
+.. highlight:: text
+
+The command-line interface is the easiest way to get started with *lincs*, starting with ``lincs --help``, which should output something like::
 
-<!-- START help/expected-help.txt -->
     Usage: lincs [OPTIONS] COMMAND [ARGS]...
 
       lincs (Learn and Infer Non-Compensatory Sorting) is a set of tools for
       training and using MCDA models.
 
     Options:
       --help  Show this message and exit.
 
     Commands:
       classification-accuracy  Compute a classification accuracy.
       classify                 Classify alternatives.
       generate                 Generate synthetic data.
       learn                    Learn a model.
       visualize                Make graphs from data.
-<!-- STOP -->
 
-It's organized using sub-commands, the first one being `generate`, to generate synthetic pseudo-random data.
+.. STOP
+
+It's organized using sub-commands, the first one being ``generate``, to generate synthetic pseudo-random data.
 
-<!-- START command-line-example/run.sh --><!--
+.. START command-line-example/run.sh
     set -o errexit
     set -o nounset
     set -o pipefail
     trap 'echo "Error on line $LINENO"' ERR
+.. STOP
 
---><!-- STOP -->
+.. highlight:: shell
 
-Generate a classification domain with 4 criteria and 3 categories (@todo Link to concepts and file formats):
+.. EXTEND command-line-example/run.sh
+
+Generate a classification domain with 4 criteria and 3 categories (@todo Link to concepts and file formats)::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs generate classification-domain 4 3 --output-domain domain.yml
-<!-- APPEND-TO-LAST-LINE --random-seed 40 -->
-<!-- STOP -->
 
-The generated `domain.yml` should look like:
+.. APPEND-TO-LAST-LINE --random-seed 40
+.. STOP
+
+.. highlight:: yaml
+
+.. START command-line-example/expected-domain.yml
+
+The generated ``domain.yml`` should look like::
 
-<!-- START command-line-example/expected-domain.yml -->
     kind: classification-domain
     format_version: 1
     criteria:
       - name: Criterion 1
         value_type: real
         category_correlation: growing
       - name: Criterion 2
@@ -215,30 +231,38 @@
       - name: Criterion 4
         value_type: real
         category_correlation: growing
     categories:
       - name: Category 1
       - name: Category 2
       - name: Category 3
-<!-- STOP -->
 
-<!-- EXTEND command-line-example/run.sh --><!--
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     diff expected-domain.yml domain.yml
---><!-- STOP -->
+.. STOP
+
+.. highlight:: shell
+
+.. EXTEND command-line-example/run.sh
 
-Then generate a classification model (@todo Link to concepts and file formats):
+Then generate a classification model (@todo Link to concepts and file formats)::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs generate classification-model domain.yml --output-model model.yml
-<!-- APPEND-TO-LAST-LINE --random-seed 41 -->
-<!-- STOP -->
 
-It should look like:
+.. APPEND-TO-LAST-LINE --random-seed 41
+.. STOP
+
+.. highlight:: yaml
+
+.. START command-line-example/expected-model.yml
+
+It should look like::
 
-<!-- START command-line-example/expected-model.yml -->
     kind: classification-model
     format_version: 1
     boundaries:
       - profile:
           - 0.255905151
           - 0.0551739037
           - 0.162252158
@@ -258,89 +282,118 @@
         sufficient_coalitions:
           kind: weights
           criterion_weights:
             - 0.147771254
             - 0.618687689
             - 0.406786472
             - 0.0960085914
-<!-- STOP -->
+
+.. STOP
 
 @todo Use YAML anchors and references to avoid repeating the same sufficient coalitions in all profiles
 
-<!-- EXTEND command-line-example/run.sh --><!--
+.. EXTEND command-line-example/run.sh
     diff expected-model.yml model.yml
---><!-- STOP -->
+.. STOP
 
-You can visualize it using:
+.. highlight:: shell
+
+.. EXTEND command-line-example/run.sh
+
+You can visualize it using::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs visualize classification-model domain.yml model.yml model.png
-<!-- STOP -->
-<!-- EXTEND command-line-example/run.sh --><!--
+
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     cp model.png ../../..
---><!-- STOP -->
+.. STOP
 
 It should output something like:
 
-![Model visualization](https://github.com/MICS-Lab/lincs/raw/v0.3.3/model.png)
+.. image:: model.png
+    :alt: Model visualization
+    :align: center
 
-And finally generate a set of classified alternatives (@todo Link to concepts and file formats):
+.. EXTEND command-line-example/run.sh
+
+And finally generate a set of classified alternatives (@todo Link to concepts and file formats)::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs generate classified-alternatives domain.yml model.yml 1000 --output-classified-alternatives learning-set.csv
-<!-- APPEND-TO-LAST-LINE --random-seed 42 -->
-<!-- STOP -->
 
-It should start with something like this, and contain 1000 alternatives:
+.. APPEND-TO-LAST-LINE --random-seed 42
+.. STOP
+
+.. highlight:: text
+
+.. START command-line-example/expected-learning-set.csv
+
+It should start with something like this, and contain 1000 alternatives::
 
-<!-- START command-line-example/expected-learning-set.csv -->
     name,"Criterion 1","Criterion 2","Criterion 3","Criterion 4",category
     "Alternative 1",0.37454012,0.796543002,0.95071429,0.183434784,"Category 3"
     "Alternative 2",0.731993914,0.779690981,0.598658502,0.596850157,"Category 2"
     "Alternative 3",0.156018645,0.445832759,0.15599452,0.0999749228,"Category 1"
     "Alternative 4",0.0580836125,0.4592489,0.866176128,0.333708614,"Category 3"
     "Alternative 5",0.601114988,0.14286682,0.708072603,0.650888503,"Category 2"
-<!-- STOP -->
 
-<!-- EXTEND command-line-example/run.sh --><!--
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     diff expected-learning-set.csv <(head -n 6 learning-set.csv)
---><!-- STOP -->
+.. STOP
+
+.. highlight:: shell
+
+.. EXTEND command-line-example/run.sh
 
-You can visualize its first five alternatives using:
+You can visualize its first five alternatives using::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs visualize classification-model domain.yml model.yml --alternatives learning-set.csv --alternatives-count 5 alternatives.png
-<!-- STOP -->
-<!-- EXTEND command-line-example/run.sh --><!--
+
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     cp alternatives.png ../../..
---><!-- STOP -->
+.. STOP
 
 It should output something like:
 
-![Alternatives visualization](https://github.com/MICS-Lab/lincs/raw/v0.3.3/alternatives.png)
+.. image:: alternatives.png
+    :alt: Alternatives visualization
+    :align: center
 
 @todo Improve how this graph looks:
 
 - display categories as stacked solid colors
 - display alternatives in a color that matches their assigned category
 - remove the legend, place names (categories and alternatives) directly on the graph
 
 You now have a (synthetic) learning set.
-You can use it to train a new model:
 
-<!-- EXTEND command-line-example/run.sh -->
+.. highlight:: shell
+
+.. EXTEND command-line-example/run.sh
+
+You can use it to train a new model::
+
     # @todo Rename the command to `train`?
     lincs learn classification-model domain.yml learning-set.csv --output-model trained-model.yml
-<!-- APPEND-TO-LAST-LINE --mrsort.weights-profiles-breed.accuracy-heuristic.random-seed 43 -->
-<!-- STOP -->
+
+.. APPEND-TO-LAST-LINE --mrsort.weights-profiles-breed.accuracy-heuristic.random-seed 43
+.. STOP
+
+.. highlight:: yaml
+
+.. START command-line-example/expected-trained-model.yml
 
 The trained model has the same structure as the original (synthetic) model because they are both MR-Sort models for the same domain,
-but the trained model is numerically different because information was lost in the process:
+but the trained model is numerically different because information was lost in the process::
 
-<!-- START command-line-example/expected-trained-model.yml -->
     kind: classification-model
     format_version: 1
     boundaries:
       - profile:
           - 0.00751833664
           - 0.0549556538
           - 0.162616938
@@ -360,46 +413,62 @@
         sufficient_coalitions:
           kind: weights
           criterion_weights:
             - 0.499998987
             - 0.5
             - 0.5
             - 0
-<!-- STOP -->
 
-<!-- EXTEND command-line-example/run.sh --><!--
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     diff expected-trained-model.yml trained-model.yml
---><!-- STOP -->
+.. STOP
 
 If the training is effective, the resulting trained model should behave closely to the original one.
 To see how close a trained model is to the original one, you can reclassify a testing set.
 
-First, generate a testing set:
+.. highlight:: shell
+
+.. EXTEND command-line-example/run.sh
+
+First, generate a testing set::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs generate classified-alternatives domain.yml model.yml 10000 --output-classified-alternatives testing-set.csv
-<!-- APPEND-TO-LAST-LINE --random-seed 44 -->
-<!-- STOP -->
 
-And ask the trained model to classify it:
+.. APPEND-TO-LAST-LINE --random-seed 44
+.. STOP
+
+.. highlight:: shell
+
+.. EXTEND command-line-example/run.sh
+
+And ask the trained model to classify it::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs classify domain.yml trained-model.yml testing-set.csv --output-classified-alternatives reclassified-testing-set.csv
-<!-- STOP -->
 
-There are a few differences between the original testing set and the reclassified one:
+.. STOP
+
+.. highlight:: shell
+
+.. EXTEND command-line-example/run.sh
+
+There are a few differences between the original testing set and the reclassified one::
 
-<!-- EXTEND command-line-example/run.sh -->
     diff testing-set.csv reclassified-testing-set.csv
-<!-- APPEND-TO-LAST-LINE >classification-diff.txt || true -->
-<!-- STOP -->
 
-That command should show a few alternatives that are not classified the same way by the original and the trained model:
+.. APPEND-TO-LAST-LINE >classification-diff.txt || true
+.. STOP
+
+.. highlight:: diff
+
+.. START command-line-example/expected-classification-diff.txt
+
+That command should show a few alternatives that are not classified the same way by the original and the trained model::
 
-<!-- START command-line-example/expected-classification-diff.txt -->
     2595c2595
     < "Alternative 2594",0.234433308,0.780464768,0.162389532,0.622178912,"Category 2"
     ---
     > "Alternative 2594",0.234433308,0.780464768,0.162389532,0.622178912,"Category 1"
     5000c5000
     < "Alternative 4999",0.074135974,0.496049821,0.672853291,0.782560945,"Category 2"
     ---
@@ -416,55 +485,70 @@
     < "Alternative 9688",0.940304875,0.885046899,0.162586793,0.515185535,"Category 2"
     ---
     > "Alternative 9688",0.940304875,0.885046899,0.162586793,0.515185535,"Category 1"
     9934c9934
     < "Alternative 9933",0.705289483,0.11529737,0.162508503,0.0438248962,"Category 2"
     ---
     > "Alternative 9933",0.705289483,0.11529737,0.162508503,0.0438248962,"Category 1"
-<!-- STOP -->
 
-<!-- EXTEND command-line-example/run.sh --><!--
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     diff expected-classification-diff.txt classification-diff.txt
---><!-- STOP -->
+.. STOP
+
+.. highlight:: shell
+
+.. EXTEND command-line-example/run.sh
 
-You can also measure the classification accuracy of the trained model on that testing set:
+You can also measure the classification accuracy of the trained model on that testing set::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs classification-accuracy domain.yml trained-model.yml testing-set.csv
-<!-- APPEND-TO-LAST-LINE >classification-accuracy.txt -->
-<!-- STOP -->
 
-It should be close to 100%:
+.. APPEND-TO-LAST-LINE >classification-accuracy.txt
+.. STOP
+
+.. START command-line-example/expected-classification-accuracy.txt
+
+.. highlight:: text
+
+It should be close to 100%::
 
-<!-- START command-line-example/expected-classification-accuracy.txt -->
     9994/10000
-<!-- STOP -->
 
-<!-- EXTEND command-line-example/run.sh --><!--
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     diff expected-classification-accuracy.txt classification-accuracy.txt
---><!-- STOP -->
+.. STOP
 
 Once you're comfortable with the tooling, you can use a learning set based on real-world data and train a model that you can use to classify new real-world alternatives.
 
-# User guide
+
+User guide
+==========
 
 @todo Write the user guide.
 
-# Reference
+
+Reference
+=========
 
 @todo Generate a reference documentation using Sphinx:
+
 - Python using autodoc
 - C++ using Doxygen+Breath
 - CLI using https://sphinx-click.readthedocs.io/en/latest/
 - YAML file formats using JSON Schema and https://sphinx-jsonschema.readthedocs.io/en/latest/
 
-# Develop *lincs* itself
 
-Run `./run-development-cycle.sh`.
+Develop *lincs* itself
+======================
+
+Run ``./run-development-cycle.sh``.
 
-<!-- Or:
+.. Or:
     docker run --rm -it -v $PWD:/wd --workdir /wd lincs-development
-After changes in C++:
-    pip install --user --no-build-isolation --editable .
-Then test whatever:
-    lincs --help
--->
+    After changes in C++:
+        pip install --user --no-build-isolation --editable .
+    Then test whatever:
+        lincs --help
```

### Comparing `lincs-0.3.3/README.md` & `lincs-0.3.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,94 @@
-<!-- Copyright 2023 Vincent Jacques -->
+Metadata-Version: 2.1
+Name: lincs
+Version: 0.3.5
+Summary: Learn and Infer Non Compensatory Sortings
+Home-page: https://github.com/MICS-Lab/lincs
+Author: Vincent Jacques
+Author-email: vincent@vincent-jacques.net
+License: LGPLv3
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/x-rst
+License-File: COPYING
+License-File: COPYING.LESSER
+
+.. Copyright 2023 Vincent Jacques
+
+.. WARNING, this README is rendered to HTML in several places
+    - on GitHub (https://github.com/mics-lab/lincs/)
+    - on PyPI after publication of the package (https://pypi.org/project/lincs/)
+    - on GitHub Pages (https://mics-lab.github.io/lincs/)
+    So when you change it, take care to check all those places.
 
 *lincs* is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
 
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files [COPYING](COPYING) and [COPYING.LESSER](COPYING.LESSER).
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.3.5/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.3.5/COPYING.LESSER>`_.
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
-Questions? Remarks? Bugs? Want to contribute? Open [an issue](https://github.com/MICS-Lab/lincs/issues) or [a discussion](https://github.com/MICS-Lab/lincs/discussions)!
+Questions? Remarks? Bugs? Want to contribute? Open `an issue <https://github.com/MICS-Lab/lincs/issues>`_ or `a discussion <https://github.com/MICS-Lab/lincs/discussions>`_!
 
-# Contributors and previous work
 
-*lincs* is developed by the [MICS](https://mics.centralesupelec.fr/) research team at [CentraleSupélec](https://www.centralesupelec.fr/).
+Contributors and previous work
+==============================
+
+*lincs* is developed by the `MICS <https://mics.centralesupelec.fr/>`_ research team at `CentraleSupélec <https://www.centralesupelec.fr/>`_.
 
 Its main authors are (alphabetical order):
-- [Laurent Cabaret](http://perso.ecp.fr/~cabaretl/) (performance optimization)
-- [Vincent Jacques](https://vincent-jacques.net) (engineering)
-- [Vincent Mousseau](https://www.centralesupelec.fr/fr/2EBDCB86-64A4-4747-96E8-C3066CB61F3D) (domain expertise and project leadership)
+
+- `Laurent Cabaret <https://cabaretl.pages.centralesupelec.fr/>`_ (performance optimization)
+- `Vincent Jacques <https://vincent-jacques.net>`_ (engineering)
+- `Vincent Mousseau <https://www.centralesupelec.fr/fr/2EBDCB86-64A4-4747-96E8-C3066CB61F3D>`_ (domain expertise)
+- `Wassila Ouerdane <https://wassilaouerdane.github.io/>`_ (domain expertise)
 
 It's based on work by:
-- [Olivier Sobrie](http://olivier.sobrie.be/) (The "weights, profiles, breed" learning strategy for MR-Sort models, and the profiles improvement heuristic, developed in his [Ph.D thesis](http://olivier.sobrie.be/papers/phd_2016_sobrie.pdf), and [implemented in Python](https://github.com/oso/pymcda))
-- Emma Dixneuf, Thibault Monsel and Thomas Vindard ([C++ implementation of Sobrie's heuristic](https://github.com/Mostah/fastPL/))
 
-# Project goals
+- `Olivier Sobrie <http://olivier.sobrie.be/>`_ (The "weights, profiles, breed" learning strategy for MR-Sort models, and the profiles improvement heuristic, developed in his `Ph.D thesis <http://olivier.sobrie.be/papers/phd_2016_sobrie.pdf>`_, and `implemented in Python <https://github.com/oso/pymcda>`_)
+- Emma Dixneuf, Thibault Monsel and Thomas Vindard (`C++ implementation of Sobrie's heuristic <https://github.com/Mostah/fastPL/>`_)
+
 
-## Provide MCDA tools usable out of the box
+Project goals
+=============
+
+Provide MCDA tools usable out of the box
+----------------------------------------
 
 You should be able to use *lincs* without being a specialist of MCDA and/or NCS models.
-Just follow the [Get started](#get-started) section below.
+Just follow the `Get started <#get-started>`_ section below.
 
-## Provide a base for developing new MCDA algorithms
+Provide a base for developing new MCDA algorithms
+-------------------------------------------------
 
 *lincs* is designed to be easy to extend with new algorithms of even replace parts of existing algorithms.
 @todo Write doc about that use case.
 
 *linc* also provides a benchmark framework to compare algorithms (@todo Write and document).
 This should make it easier to understand the relative strengths and weaknesses of each algorithm.
 
-# Get started
 
-## Install
+Get started
+===========
+
+Install
+-------
+
 
-First, you need to install a few dependencies (@todo build binary wheel distributions to make installation easier):
 
-<!-- START install/dependencies.sh -->
+.. START install/dependencies.sh
+
+First, you need to install a few dependencies (@todo build binary wheel distributions to make installation easier)::
+
     # System packages
     sudo apt-get install --yes g++ libboost-python-dev python3-dev libyaml-cpp-dev
 
     # CUDA
     sudo apt-key adv --fetch-keys https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2204/x86_64/3bf863cc.pub
     sudo add-apt-repository 'deb https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2204/x86_64/ /'
     sudo apt-get update
@@ -62,41 +104,44 @@
 
     # Header-only libraries
     cd /usr/local/include
     sudo wget https://raw.githubusercontent.com/Neargye/magic_enum/v0.8.2/include/magic_enum.hpp
     sudo wget https://raw.githubusercontent.com/d99kris/rapidcsv/v8.75/src/rapidcsv.h
     sudo wget https://raw.githubusercontent.com/jacquev6/lov-e-cuda/13e45bc/lov-e.hpp
     sudo wget https://raw.githubusercontent.com/doctest/doctest/v2.4.11/doctest/doctest.h
-<!-- STOP -->
 
-<!-- START install/Dockerfile-pre --><!--
+.. STOP
+
+.. START install/Dockerfile-pre
     FROM ubuntu:22.04
 
     RUN apt-get update
 
     RUN DEBIAN_FRONTEND=noninteractive apt-get install --yes \
           sudo wget python3-pip dirmngr gpg-agent software-properties-common
 
     RUN useradd user --create-home
     RUN echo "user ALL=(ALL) NOPASSWD:ALL" > /etc/sudoers.d/user
     USER user
     ENV PATH=$PATH:/home/user/.local/bin
     WORKDIR /home/user
---><!-- STOP -->
 
-<!-- START install/Dockerfile-post --><!--
+.. STOP
+
+.. START install/Dockerfile-post
     WORKDIR /home/user
     # Speed-up build when requirements don't change
     ADD project/requirements.txt .
     RUN pip3 install -r requirements.txt
     ADD --chown=user project /home/user/lincs
     RUN pip3 install ./lincs
---><!-- STOP -->
 
-<!-- START install/run.sh --><!--
+.. STOP
+
+.. START install/run.sh
     set -o errexit
     set -o nounset
     set -o pipefail
     trap 'echo "Error on line $LINENO"' ERR
 
     # Transform the dependencies.sh file into a Dockerfile to benefit from the Docker build cache
     (
@@ -108,81 +153,94 @@
       | sed 's/^RUN cd/WORKDIR/'
       echo
       cat Dockerfile-post
     ) >Dockerfile
 
     mkdir project
     cp -r ../../../{lincs,requirements.txt,setup.py} project
-    touch project/README.md  # No need for the actual readme, so don't bust the Docker cache
+    touch project/README.rst  # No need for the actual readme, so don't bust the Docker cache
 
     docker build . --tag lincs-development--install --quiet >/dev/null
     docker run --rm lincs-development--install lincs --help >/dev/null
---><!-- STOP -->
 
-Finally, *lincs* is available on the [Python Package Index](https://pypi.org/project/lincs/), so `pip install lincs` should finalize the install.
+.. STOP
 
-## Concepts and files
+Finally, *lincs* is available on the `Python Package Index <https://pypi.org/project/lincs/>`_, so ``pip install lincs`` should finalize the install.
+
+Concepts and files
+------------------
 
 *lincs* is based on the following concepts:
 
 - a "domain" describes the objects to be classified (*a.k.a.* the "alternatives"), the criteria used to classify them, and the existing categories they can belong to;
 - a "model" is used to actually assign a category to each alternative, based on the values of the criteria for that alternative;
 - a "classified alternative" is an alternative, with its category.
 
-## Start using *lincs*' command-line interface
-
-The command-line interface is the easiest way to get started with *lincs*, starting with `lincs --help`, which should output something like:
+Start using *lincs*' command-line interface
+-------------------------------------------
 
-<!-- START help/run.sh --><!--
+.. START help/run.sh
     set -o errexit
     set -o nounset
     set -o pipefail
     trap 'echo "Error on line $LINENO"' ERR
 
     lincs --help >actual-help.txt
     diff expected-help.txt actual-help.txt
---><!-- STOP -->
+.. STOP
+
+.. START help/expected-help.txt
+
+
+
+The command-line interface is the easiest way to get started with *lincs*, starting with ``lincs --help``, which should output something like::
 
-<!-- START help/expected-help.txt -->
     Usage: lincs [OPTIONS] COMMAND [ARGS]...
 
       lincs (Learn and Infer Non-Compensatory Sorting) is a set of tools for
       training and using MCDA models.
 
     Options:
       --help  Show this message and exit.
 
     Commands:
       classification-accuracy  Compute a classification accuracy.
       classify                 Classify alternatives.
       generate                 Generate synthetic data.
       learn                    Learn a model.
       visualize                Make graphs from data.
-<!-- STOP -->
 
-It's organized using sub-commands, the first one being `generate`, to generate synthetic pseudo-random data.
+.. STOP
 
-<!-- START command-line-example/run.sh --><!--
+It's organized using sub-commands, the first one being ``generate``, to generate synthetic pseudo-random data.
+
+.. START command-line-example/run.sh
     set -o errexit
     set -o nounset
     set -o pipefail
     trap 'echo "Error on line $LINENO"' ERR
+.. STOP
+
+
 
---><!-- STOP -->
+.. EXTEND command-line-example/run.sh
 
-Generate a classification domain with 4 criteria and 3 categories (@todo Link to concepts and file formats):
+Generate a classification domain with 4 criteria and 3 categories (@todo Link to concepts and file formats)::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs generate classification-domain 4 3 --output-domain domain.yml
-<!-- APPEND-TO-LAST-LINE --random-seed 40 -->
-<!-- STOP -->
 
-The generated `domain.yml` should look like:
+.. APPEND-TO-LAST-LINE --random-seed 40
+.. STOP
+
+
+
+.. START command-line-example/expected-domain.yml
+
+The generated ``domain.yml`` should look like::
 
-<!-- START command-line-example/expected-domain.yml -->
     kind: classification-domain
     format_version: 1
     criteria:
       - name: Criterion 1
         value_type: real
         category_correlation: growing
       - name: Criterion 2
@@ -194,30 +252,38 @@
       - name: Criterion 4
         value_type: real
         category_correlation: growing
     categories:
       - name: Category 1
       - name: Category 2
       - name: Category 3
-<!-- STOP -->
 
-<!-- EXTEND command-line-example/run.sh --><!--
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     diff expected-domain.yml domain.yml
---><!-- STOP -->
+.. STOP
+
+
+
+.. EXTEND command-line-example/run.sh
 
-Then generate a classification model (@todo Link to concepts and file formats):
+Then generate a classification model (@todo Link to concepts and file formats)::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs generate classification-model domain.yml --output-model model.yml
-<!-- APPEND-TO-LAST-LINE --random-seed 41 -->
-<!-- STOP -->
 
-It should look like:
+.. APPEND-TO-LAST-LINE --random-seed 41
+.. STOP
+
+
+
+.. START command-line-example/expected-model.yml
+
+It should look like::
 
-<!-- START command-line-example/expected-model.yml -->
     kind: classification-model
     format_version: 1
     boundaries:
       - profile:
           - 0.255905151
           - 0.0551739037
           - 0.162252158
@@ -237,89 +303,118 @@
         sufficient_coalitions:
           kind: weights
           criterion_weights:
             - 0.147771254
             - 0.618687689
             - 0.406786472
             - 0.0960085914
-<!-- STOP -->
+
+.. STOP
 
 @todo Use YAML anchors and references to avoid repeating the same sufficient coalitions in all profiles
 
-<!-- EXTEND command-line-example/run.sh --><!--
+.. EXTEND command-line-example/run.sh
     diff expected-model.yml model.yml
---><!-- STOP -->
+.. STOP
 
-You can visualize it using:
 
-<!-- EXTEND command-line-example/run.sh -->
+
+.. EXTEND command-line-example/run.sh
+
+You can visualize it using::
+
     lincs visualize classification-model domain.yml model.yml model.png
-<!-- STOP -->
-<!-- EXTEND command-line-example/run.sh --><!--
+
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     cp model.png ../../..
---><!-- STOP -->
+.. STOP
 
 It should output something like:
 
-![Model visualization](model.png)
+.. image:: https://github.com/MICS-Lab/lincs/raw/v0.3.5/model.png
+    :alt: Model visualization
+    :align: center
 
-And finally generate a set of classified alternatives (@todo Link to concepts and file formats):
+.. EXTEND command-line-example/run.sh
+
+And finally generate a set of classified alternatives (@todo Link to concepts and file formats)::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs generate classified-alternatives domain.yml model.yml 1000 --output-classified-alternatives learning-set.csv
-<!-- APPEND-TO-LAST-LINE --random-seed 42 -->
-<!-- STOP -->
 
-It should start with something like this, and contain 1000 alternatives:
+.. APPEND-TO-LAST-LINE --random-seed 42
+.. STOP
+
+
+
+.. START command-line-example/expected-learning-set.csv
+
+It should start with something like this, and contain 1000 alternatives::
 
-<!-- START command-line-example/expected-learning-set.csv -->
     name,"Criterion 1","Criterion 2","Criterion 3","Criterion 4",category
     "Alternative 1",0.37454012,0.796543002,0.95071429,0.183434784,"Category 3"
     "Alternative 2",0.731993914,0.779690981,0.598658502,0.596850157,"Category 2"
     "Alternative 3",0.156018645,0.445832759,0.15599452,0.0999749228,"Category 1"
     "Alternative 4",0.0580836125,0.4592489,0.866176128,0.333708614,"Category 3"
     "Alternative 5",0.601114988,0.14286682,0.708072603,0.650888503,"Category 2"
-<!-- STOP -->
 
-<!-- EXTEND command-line-example/run.sh --><!--
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     diff expected-learning-set.csv <(head -n 6 learning-set.csv)
---><!-- STOP -->
+.. STOP
+
+
 
-You can visualize its first five alternatives using:
+.. EXTEND command-line-example/run.sh
+
+You can visualize its first five alternatives using::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs visualize classification-model domain.yml model.yml --alternatives learning-set.csv --alternatives-count 5 alternatives.png
-<!-- STOP -->
-<!-- EXTEND command-line-example/run.sh --><!--
+
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     cp alternatives.png ../../..
---><!-- STOP -->
+.. STOP
 
 It should output something like:
 
-![Alternatives visualization](alternatives.png)
+.. image:: https://github.com/MICS-Lab/lincs/raw/v0.3.5/alternatives.png
+    :alt: Alternatives visualization
+    :align: center
 
 @todo Improve how this graph looks:
 
 - display categories as stacked solid colors
 - display alternatives in a color that matches their assigned category
 - remove the legend, place names (categories and alternatives) directly on the graph
 
 You now have a (synthetic) learning set.
-You can use it to train a new model:
 
-<!-- EXTEND command-line-example/run.sh -->
+
+
+.. EXTEND command-line-example/run.sh
+
+You can use it to train a new model::
+
     # @todo Rename the command to `train`?
     lincs learn classification-model domain.yml learning-set.csv --output-model trained-model.yml
-<!-- APPEND-TO-LAST-LINE --mrsort.weights-profiles-breed.accuracy-heuristic.random-seed 43 -->
-<!-- STOP -->
+
+.. APPEND-TO-LAST-LINE --mrsort.weights-profiles-breed.accuracy-heuristic.random-seed 43
+.. STOP
+
+
+
+.. START command-line-example/expected-trained-model.yml
 
 The trained model has the same structure as the original (synthetic) model because they are both MR-Sort models for the same domain,
-but the trained model is numerically different because information was lost in the process:
+but the trained model is numerically different because information was lost in the process::
 
-<!-- START command-line-example/expected-trained-model.yml -->
     kind: classification-model
     format_version: 1
     boundaries:
       - profile:
           - 0.00751833664
           - 0.0549556538
           - 0.162616938
@@ -339,46 +434,62 @@
         sufficient_coalitions:
           kind: weights
           criterion_weights:
             - 0.499998987
             - 0.5
             - 0.5
             - 0
-<!-- STOP -->
 
-<!-- EXTEND command-line-example/run.sh --><!--
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     diff expected-trained-model.yml trained-model.yml
---><!-- STOP -->
+.. STOP
 
 If the training is effective, the resulting trained model should behave closely to the original one.
 To see how close a trained model is to the original one, you can reclassify a testing set.
 
-First, generate a testing set:
 
-<!-- EXTEND command-line-example/run.sh -->
+
+.. EXTEND command-line-example/run.sh
+
+First, generate a testing set::
+
     lincs generate classified-alternatives domain.yml model.yml 10000 --output-classified-alternatives testing-set.csv
-<!-- APPEND-TO-LAST-LINE --random-seed 44 -->
-<!-- STOP -->
 
-And ask the trained model to classify it:
+.. APPEND-TO-LAST-LINE --random-seed 44
+.. STOP
+
+
+
+.. EXTEND command-line-example/run.sh
+
+And ask the trained model to classify it::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs classify domain.yml trained-model.yml testing-set.csv --output-classified-alternatives reclassified-testing-set.csv
-<!-- STOP -->
 
-There are a few differences between the original testing set and the reclassified one:
+.. STOP
+
+
+
+.. EXTEND command-line-example/run.sh
+
+There are a few differences between the original testing set and the reclassified one::
 
-<!-- EXTEND command-line-example/run.sh -->
     diff testing-set.csv reclassified-testing-set.csv
-<!-- APPEND-TO-LAST-LINE >classification-diff.txt || true -->
-<!-- STOP -->
 
-That command should show a few alternatives that are not classified the same way by the original and the trained model:
+.. APPEND-TO-LAST-LINE >classification-diff.txt || true
+.. STOP
+
+
+
+.. START command-line-example/expected-classification-diff.txt
+
+That command should show a few alternatives that are not classified the same way by the original and the trained model::
 
-<!-- START command-line-example/expected-classification-diff.txt -->
     2595c2595
     < "Alternative 2594",0.234433308,0.780464768,0.162389532,0.622178912,"Category 2"
     ---
     > "Alternative 2594",0.234433308,0.780464768,0.162389532,0.622178912,"Category 1"
     5000c5000
     < "Alternative 4999",0.074135974,0.496049821,0.672853291,0.782560945,"Category 2"
     ---
@@ -395,55 +506,70 @@
     < "Alternative 9688",0.940304875,0.885046899,0.162586793,0.515185535,"Category 2"
     ---
     > "Alternative 9688",0.940304875,0.885046899,0.162586793,0.515185535,"Category 1"
     9934c9934
     < "Alternative 9933",0.705289483,0.11529737,0.162508503,0.0438248962,"Category 2"
     ---
     > "Alternative 9933",0.705289483,0.11529737,0.162508503,0.0438248962,"Category 1"
-<!-- STOP -->
 
-<!-- EXTEND command-line-example/run.sh --><!--
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     diff expected-classification-diff.txt classification-diff.txt
---><!-- STOP -->
+.. STOP
+
+
 
-You can also measure the classification accuracy of the trained model on that testing set:
+.. EXTEND command-line-example/run.sh
+
+You can also measure the classification accuracy of the trained model on that testing set::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs classification-accuracy domain.yml trained-model.yml testing-set.csv
-<!-- APPEND-TO-LAST-LINE >classification-accuracy.txt -->
-<!-- STOP -->
 
-It should be close to 100%:
+.. APPEND-TO-LAST-LINE >classification-accuracy.txt
+.. STOP
+
+.. START command-line-example/expected-classification-accuracy.txt
+
+
+
+It should be close to 100%::
 
-<!-- START command-line-example/expected-classification-accuracy.txt -->
     9994/10000
-<!-- STOP -->
 
-<!-- EXTEND command-line-example/run.sh --><!--
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     diff expected-classification-accuracy.txt classification-accuracy.txt
---><!-- STOP -->
+.. STOP
 
 Once you're comfortable with the tooling, you can use a learning set based on real-world data and train a model that you can use to classify new real-world alternatives.
 
-# User guide
+
+User guide
+==========
 
 @todo Write the user guide.
 
-# Reference
+
+Reference
+=========
 
 @todo Generate a reference documentation using Sphinx:
+
 - Python using autodoc
 - C++ using Doxygen+Breath
 - CLI using https://sphinx-click.readthedocs.io/en/latest/
 - YAML file formats using JSON Schema and https://sphinx-jsonschema.readthedocs.io/en/latest/
 
-# Develop *lincs* itself
 
-Run `./run-development-cycle.sh`.
+Develop *lincs* itself
+======================
+
+Run ``./run-development-cycle.sh``.
 
-<!-- Or:
+.. Or:
     docker run --rm -it -v $PWD:/wd --workdir /wd lincs-development
-After changes in C++:
-    pip install --user --no-build-isolation --editable .
-Then test whatever:
-    lincs --help
--->
+    After changes in C++:
+        pip install --user --no-build-isolation --editable .
+    Then test whatever:
+        lincs --help
```

### Comparing `lincs-0.3.3/lincs/__init__.py` & `lincs-0.3.5/lincs/__init__.py`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/command_line_interface.py` & `lincs-0.3.5/lincs/command_line_interface.py`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/classification.cpp` & `lincs-0.3.5/lincs/liblincs/classification.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/generation.cpp` & `lincs-0.3.5/lincs/liblincs/generation.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/generation.hpp` & `lincs-0.3.5/lincs/liblincs/generation.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/io/alternatives.cpp` & `lincs-0.3.5/lincs/liblincs/io/alternatives.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/io/alternatives.hpp` & `lincs-0.3.5/lincs/liblincs/io/alternatives.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/io/domain.cpp` & `lincs-0.3.5/lincs/liblincs/io/domain.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/io/domain.hpp` & `lincs-0.3.5/lincs/liblincs/io/domain.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/io/model.cpp` & `lincs-0.3.5/lincs/liblincs/io/model.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/io/model.hpp` & `lincs-0.3.5/lincs/liblincs/io/model.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.cpp` & `lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.hpp` & `lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp` & `lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp` & `lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.cpp` & `lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.hpp` & `lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp` & `lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp` & `lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp` & `lincs-0.3.5/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/learning.cpp` & `lincs-0.3.5/lincs/liblincs/learning.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/learning.hpp` & `lincs-0.3.5/lincs/liblincs/learning.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/liblincs_module.cpp` & `lincs-0.3.5/lincs/liblincs/liblincs_module.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/median-and-max.cpp` & `lincs-0.3.5/lincs/liblincs/median-and-max.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/median-and-max.hpp` & `lincs-0.3.5/lincs/liblincs/median-and-max.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/randomness-utils.cpp` & `lincs-0.3.5/lincs/liblincs/randomness-utils.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs/randomness-utils.hpp` & `lincs-0.3.5/lincs/liblincs/randomness-utils.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/liblincs_module_tests.py` & `lincs-0.3.5/lincs/liblincs_module_tests.py`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs/visualization.py` & `lincs-0.3.5/lincs/visualization.py`

 * *Files identical despite different names*

### Comparing `lincs-0.3.3/lincs.egg-info/PKG-INFO` & `lincs-0.3.5/lincs.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,94 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.3.3
+Version: 0.3.5
 Summary: Learn and Infer Non Compensatory Sortings
 Home-page: https://github.com/MICS-Lab/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 License-File: COPYING
 License-File: COPYING.LESSER
 
-<!-- Copyright 2023 Vincent Jacques -->
+.. Copyright 2023 Vincent Jacques
+
+.. WARNING, this README is rendered to HTML in several places
+    - on GitHub (https://github.com/mics-lab/lincs/)
+    - on PyPI after publication of the package (https://pypi.org/project/lincs/)
+    - on GitHub Pages (https://mics-lab.github.io/lincs/)
+    So when you change it, take care to check all those places.
 
 *lincs* is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
 
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files [COPYING](https://github.com/MICS-Lab/lincs/blob/v0.3.3/COPYING) and [COPYING.LESSER](https://github.com/MICS-Lab/lincs/blob/v0.3.3/COPYING.LESSER).
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.3.5/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.3.5/COPYING.LESSER>`_.
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
-Questions? Remarks? Bugs? Want to contribute? Open [an issue](https://github.com/MICS-Lab/lincs/issues) or [a discussion](https://github.com/MICS-Lab/lincs/discussions)!
+Questions? Remarks? Bugs? Want to contribute? Open `an issue <https://github.com/MICS-Lab/lincs/issues>`_ or `a discussion <https://github.com/MICS-Lab/lincs/discussions>`_!
+
 
-# Contributors and previous work
+Contributors and previous work
+==============================
 
-*lincs* is developed by the [MICS](https://mics.centralesupelec.fr/) research team at [CentraleSupélec](https://www.centralesupelec.fr/).
+*lincs* is developed by the `MICS <https://mics.centralesupelec.fr/>`_ research team at `CentraleSupélec <https://www.centralesupelec.fr/>`_.
 
 Its main authors are (alphabetical order):
-- [Laurent Cabaret](http://perso.ecp.fr/~cabaretl/) (performance optimization)
-- [Vincent Jacques](https://vincent-jacques.net) (engineering)
-- [Vincent Mousseau](https://www.centralesupelec.fr/fr/2EBDCB86-64A4-4747-96E8-C3066CB61F3D) (domain expertise and project leadership)
+
+- `Laurent Cabaret <https://cabaretl.pages.centralesupelec.fr/>`_ (performance optimization)
+- `Vincent Jacques <https://vincent-jacques.net>`_ (engineering)
+- `Vincent Mousseau <https://www.centralesupelec.fr/fr/2EBDCB86-64A4-4747-96E8-C3066CB61F3D>`_ (domain expertise)
+- `Wassila Ouerdane <https://wassilaouerdane.github.io/>`_ (domain expertise)
 
 It's based on work by:
-- [Olivier Sobrie](http://olivier.sobrie.be/) (The "weights, profiles, breed" learning strategy for MR-Sort models, and the profiles improvement heuristic, developed in his [Ph.D thesis](http://olivier.sobrie.be/papers/phd_2016_sobrie.pdf), and [implemented in Python](https://github.com/oso/pymcda))
-- Emma Dixneuf, Thibault Monsel and Thomas Vindard ([C++ implementation of Sobrie's heuristic](https://github.com/Mostah/fastPL/))
 
-# Project goals
+- `Olivier Sobrie <http://olivier.sobrie.be/>`_ (The "weights, profiles, breed" learning strategy for MR-Sort models, and the profiles improvement heuristic, developed in his `Ph.D thesis <http://olivier.sobrie.be/papers/phd_2016_sobrie.pdf>`_, and `implemented in Python <https://github.com/oso/pymcda>`_)
+- Emma Dixneuf, Thibault Monsel and Thomas Vindard (`C++ implementation of Sobrie's heuristic <https://github.com/Mostah/fastPL/>`_)
 
-## Provide MCDA tools usable out of the box
+
+Project goals
+=============
+
+Provide MCDA tools usable out of the box
+----------------------------------------
 
 You should be able to use *lincs* without being a specialist of MCDA and/or NCS models.
-Just follow the [Get started](#get-started) section below.
+Just follow the `Get started <#get-started>`_ section below.
 
-## Provide a base for developing new MCDA algorithms
+Provide a base for developing new MCDA algorithms
+-------------------------------------------------
 
 *lincs* is designed to be easy to extend with new algorithms of even replace parts of existing algorithms.
 @todo Write doc about that use case.
 
 *linc* also provides a benchmark framework to compare algorithms (@todo Write and document).
 This should make it easier to understand the relative strengths and weaknesses of each algorithm.
 
-# Get started
 
-## Install
+Get started
+===========
+
+Install
+-------
 
-First, you need to install a few dependencies (@todo build binary wheel distributions to make installation easier):
 
-<!-- START install/dependencies.sh -->
+
+.. START install/dependencies.sh
+
+First, you need to install a few dependencies (@todo build binary wheel distributions to make installation easier)::
+
     # System packages
     sudo apt-get install --yes g++ libboost-python-dev python3-dev libyaml-cpp-dev
 
     # CUDA
     sudo apt-key adv --fetch-keys https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2204/x86_64/3bf863cc.pub
     sudo add-apt-repository 'deb https://developer.download.nvidia.com/compute/cuda/repos/ubuntu2204/x86_64/ /'
     sudo apt-get update
@@ -83,41 +104,44 @@
 
     # Header-only libraries
     cd /usr/local/include
     sudo wget https://raw.githubusercontent.com/Neargye/magic_enum/v0.8.2/include/magic_enum.hpp
     sudo wget https://raw.githubusercontent.com/d99kris/rapidcsv/v8.75/src/rapidcsv.h
     sudo wget https://raw.githubusercontent.com/jacquev6/lov-e-cuda/13e45bc/lov-e.hpp
     sudo wget https://raw.githubusercontent.com/doctest/doctest/v2.4.11/doctest/doctest.h
-<!-- STOP -->
 
-<!-- START install/Dockerfile-pre --><!--
+.. STOP
+
+.. START install/Dockerfile-pre
     FROM ubuntu:22.04
 
     RUN apt-get update
 
     RUN DEBIAN_FRONTEND=noninteractive apt-get install --yes \
           sudo wget python3-pip dirmngr gpg-agent software-properties-common
 
     RUN useradd user --create-home
     RUN echo "user ALL=(ALL) NOPASSWD:ALL" > /etc/sudoers.d/user
     USER user
     ENV PATH=$PATH:/home/user/.local/bin
     WORKDIR /home/user
---><!-- STOP -->
 
-<!-- START install/Dockerfile-post --><!--
+.. STOP
+
+.. START install/Dockerfile-post
     WORKDIR /home/user
     # Speed-up build when requirements don't change
     ADD project/requirements.txt .
     RUN pip3 install -r requirements.txt
     ADD --chown=user project /home/user/lincs
     RUN pip3 install ./lincs
---><!-- STOP -->
 
-<!-- START install/run.sh --><!--
+.. STOP
+
+.. START install/run.sh
     set -o errexit
     set -o nounset
     set -o pipefail
     trap 'echo "Error on line $LINENO"' ERR
 
     # Transform the dependencies.sh file into a Dockerfile to benefit from the Docker build cache
     (
@@ -129,81 +153,94 @@
       | sed 's/^RUN cd/WORKDIR/'
       echo
       cat Dockerfile-post
     ) >Dockerfile
 
     mkdir project
     cp -r ../../../{lincs,requirements.txt,setup.py} project
-    touch project/README.md  # No need for the actual readme, so don't bust the Docker cache
+    touch project/README.rst  # No need for the actual readme, so don't bust the Docker cache
 
     docker build . --tag lincs-development--install --quiet >/dev/null
     docker run --rm lincs-development--install lincs --help >/dev/null
---><!-- STOP -->
 
-Finally, *lincs* is available on the [Python Package Index](https://pypi.org/project/lincs/), so `pip install lincs` should finalize the install.
+.. STOP
+
+Finally, *lincs* is available on the `Python Package Index <https://pypi.org/project/lincs/>`_, so ``pip install lincs`` should finalize the install.
 
-## Concepts and files
+Concepts and files
+------------------
 
 *lincs* is based on the following concepts:
 
 - a "domain" describes the objects to be classified (*a.k.a.* the "alternatives"), the criteria used to classify them, and the existing categories they can belong to;
 - a "model" is used to actually assign a category to each alternative, based on the values of the criteria for that alternative;
 - a "classified alternative" is an alternative, with its category.
 
-## Start using *lincs*' command-line interface
-
-The command-line interface is the easiest way to get started with *lincs*, starting with `lincs --help`, which should output something like:
+Start using *lincs*' command-line interface
+-------------------------------------------
 
-<!-- START help/run.sh --><!--
+.. START help/run.sh
     set -o errexit
     set -o nounset
     set -o pipefail
     trap 'echo "Error on line $LINENO"' ERR
 
     lincs --help >actual-help.txt
     diff expected-help.txt actual-help.txt
---><!-- STOP -->
+.. STOP
+
+.. START help/expected-help.txt
+
+
+
+The command-line interface is the easiest way to get started with *lincs*, starting with ``lincs --help``, which should output something like::
 
-<!-- START help/expected-help.txt -->
     Usage: lincs [OPTIONS] COMMAND [ARGS]...
 
       lincs (Learn and Infer Non-Compensatory Sorting) is a set of tools for
       training and using MCDA models.
 
     Options:
       --help  Show this message and exit.
 
     Commands:
       classification-accuracy  Compute a classification accuracy.
       classify                 Classify alternatives.
       generate                 Generate synthetic data.
       learn                    Learn a model.
       visualize                Make graphs from data.
-<!-- STOP -->
 
-It's organized using sub-commands, the first one being `generate`, to generate synthetic pseudo-random data.
+.. STOP
+
+It's organized using sub-commands, the first one being ``generate``, to generate synthetic pseudo-random data.
 
-<!-- START command-line-example/run.sh --><!--
+.. START command-line-example/run.sh
     set -o errexit
     set -o nounset
     set -o pipefail
     trap 'echo "Error on line $LINENO"' ERR
+.. STOP
+
 
---><!-- STOP -->
 
-Generate a classification domain with 4 criteria and 3 categories (@todo Link to concepts and file formats):
+.. EXTEND command-line-example/run.sh
+
+Generate a classification domain with 4 criteria and 3 categories (@todo Link to concepts and file formats)::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs generate classification-domain 4 3 --output-domain domain.yml
-<!-- APPEND-TO-LAST-LINE --random-seed 40 -->
-<!-- STOP -->
 
-The generated `domain.yml` should look like:
+.. APPEND-TO-LAST-LINE --random-seed 40
+.. STOP
+
+
+
+.. START command-line-example/expected-domain.yml
+
+The generated ``domain.yml`` should look like::
 
-<!-- START command-line-example/expected-domain.yml -->
     kind: classification-domain
     format_version: 1
     criteria:
       - name: Criterion 1
         value_type: real
         category_correlation: growing
       - name: Criterion 2
@@ -215,30 +252,38 @@
       - name: Criterion 4
         value_type: real
         category_correlation: growing
     categories:
       - name: Category 1
       - name: Category 2
       - name: Category 3
-<!-- STOP -->
 
-<!-- EXTEND command-line-example/run.sh --><!--
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     diff expected-domain.yml domain.yml
---><!-- STOP -->
+.. STOP
+
+
 
-Then generate a classification model (@todo Link to concepts and file formats):
+.. EXTEND command-line-example/run.sh
+
+Then generate a classification model (@todo Link to concepts and file formats)::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs generate classification-model domain.yml --output-model model.yml
-<!-- APPEND-TO-LAST-LINE --random-seed 41 -->
-<!-- STOP -->
 
-It should look like:
+.. APPEND-TO-LAST-LINE --random-seed 41
+.. STOP
+
+
+
+.. START command-line-example/expected-model.yml
+
+It should look like::
 
-<!-- START command-line-example/expected-model.yml -->
     kind: classification-model
     format_version: 1
     boundaries:
       - profile:
           - 0.255905151
           - 0.0551739037
           - 0.162252158
@@ -258,89 +303,118 @@
         sufficient_coalitions:
           kind: weights
           criterion_weights:
             - 0.147771254
             - 0.618687689
             - 0.406786472
             - 0.0960085914
-<!-- STOP -->
+
+.. STOP
 
 @todo Use YAML anchors and references to avoid repeating the same sufficient coalitions in all profiles
 
-<!-- EXTEND command-line-example/run.sh --><!--
+.. EXTEND command-line-example/run.sh
     diff expected-model.yml model.yml
---><!-- STOP -->
+.. STOP
+
+
 
-You can visualize it using:
+.. EXTEND command-line-example/run.sh
+
+You can visualize it using::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs visualize classification-model domain.yml model.yml model.png
-<!-- STOP -->
-<!-- EXTEND command-line-example/run.sh --><!--
+
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     cp model.png ../../..
---><!-- STOP -->
+.. STOP
 
 It should output something like:
 
-![Model visualization](https://github.com/MICS-Lab/lincs/raw/v0.3.3/model.png)
+.. image:: https://github.com/MICS-Lab/lincs/raw/v0.3.5/model.png
+    :alt: Model visualization
+    :align: center
 
-And finally generate a set of classified alternatives (@todo Link to concepts and file formats):
+.. EXTEND command-line-example/run.sh
+
+And finally generate a set of classified alternatives (@todo Link to concepts and file formats)::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs generate classified-alternatives domain.yml model.yml 1000 --output-classified-alternatives learning-set.csv
-<!-- APPEND-TO-LAST-LINE --random-seed 42 -->
-<!-- STOP -->
 
-It should start with something like this, and contain 1000 alternatives:
+.. APPEND-TO-LAST-LINE --random-seed 42
+.. STOP
+
+
+
+.. START command-line-example/expected-learning-set.csv
+
+It should start with something like this, and contain 1000 alternatives::
 
-<!-- START command-line-example/expected-learning-set.csv -->
     name,"Criterion 1","Criterion 2","Criterion 3","Criterion 4",category
     "Alternative 1",0.37454012,0.796543002,0.95071429,0.183434784,"Category 3"
     "Alternative 2",0.731993914,0.779690981,0.598658502,0.596850157,"Category 2"
     "Alternative 3",0.156018645,0.445832759,0.15599452,0.0999749228,"Category 1"
     "Alternative 4",0.0580836125,0.4592489,0.866176128,0.333708614,"Category 3"
     "Alternative 5",0.601114988,0.14286682,0.708072603,0.650888503,"Category 2"
-<!-- STOP -->
 
-<!-- EXTEND command-line-example/run.sh --><!--
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     diff expected-learning-set.csv <(head -n 6 learning-set.csv)
---><!-- STOP -->
+.. STOP
+
+
 
-You can visualize its first five alternatives using:
+.. EXTEND command-line-example/run.sh
+
+You can visualize its first five alternatives using::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs visualize classification-model domain.yml model.yml --alternatives learning-set.csv --alternatives-count 5 alternatives.png
-<!-- STOP -->
-<!-- EXTEND command-line-example/run.sh --><!--
+
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     cp alternatives.png ../../..
---><!-- STOP -->
+.. STOP
 
 It should output something like:
 
-![Alternatives visualization](https://github.com/MICS-Lab/lincs/raw/v0.3.3/alternatives.png)
+.. image:: https://github.com/MICS-Lab/lincs/raw/v0.3.5/alternatives.png
+    :alt: Alternatives visualization
+    :align: center
 
 @todo Improve how this graph looks:
 
 - display categories as stacked solid colors
 - display alternatives in a color that matches their assigned category
 - remove the legend, place names (categories and alternatives) directly on the graph
 
 You now have a (synthetic) learning set.
-You can use it to train a new model:
 
-<!-- EXTEND command-line-example/run.sh -->
+
+
+.. EXTEND command-line-example/run.sh
+
+You can use it to train a new model::
+
     # @todo Rename the command to `train`?
     lincs learn classification-model domain.yml learning-set.csv --output-model trained-model.yml
-<!-- APPEND-TO-LAST-LINE --mrsort.weights-profiles-breed.accuracy-heuristic.random-seed 43 -->
-<!-- STOP -->
+
+.. APPEND-TO-LAST-LINE --mrsort.weights-profiles-breed.accuracy-heuristic.random-seed 43
+.. STOP
+
+
+
+.. START command-line-example/expected-trained-model.yml
 
 The trained model has the same structure as the original (synthetic) model because they are both MR-Sort models for the same domain,
-but the trained model is numerically different because information was lost in the process:
+but the trained model is numerically different because information was lost in the process::
 
-<!-- START command-line-example/expected-trained-model.yml -->
     kind: classification-model
     format_version: 1
     boundaries:
       - profile:
           - 0.00751833664
           - 0.0549556538
           - 0.162616938
@@ -360,46 +434,62 @@
         sufficient_coalitions:
           kind: weights
           criterion_weights:
             - 0.499998987
             - 0.5
             - 0.5
             - 0
-<!-- STOP -->
 
-<!-- EXTEND command-line-example/run.sh --><!--
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     diff expected-trained-model.yml trained-model.yml
---><!-- STOP -->
+.. STOP
 
 If the training is effective, the resulting trained model should behave closely to the original one.
 To see how close a trained model is to the original one, you can reclassify a testing set.
 
-First, generate a testing set:
 
-<!-- EXTEND command-line-example/run.sh -->
+
+.. EXTEND command-line-example/run.sh
+
+First, generate a testing set::
+
     lincs generate classified-alternatives domain.yml model.yml 10000 --output-classified-alternatives testing-set.csv
-<!-- APPEND-TO-LAST-LINE --random-seed 44 -->
-<!-- STOP -->
 
-And ask the trained model to classify it:
+.. APPEND-TO-LAST-LINE --random-seed 44
+.. STOP
+
+
+
+.. EXTEND command-line-example/run.sh
+
+And ask the trained model to classify it::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs classify domain.yml trained-model.yml testing-set.csv --output-classified-alternatives reclassified-testing-set.csv
-<!-- STOP -->
 
-There are a few differences between the original testing set and the reclassified one:
+.. STOP
+
+
+
+.. EXTEND command-line-example/run.sh
+
+There are a few differences between the original testing set and the reclassified one::
 
-<!-- EXTEND command-line-example/run.sh -->
     diff testing-set.csv reclassified-testing-set.csv
-<!-- APPEND-TO-LAST-LINE >classification-diff.txt || true -->
-<!-- STOP -->
 
-That command should show a few alternatives that are not classified the same way by the original and the trained model:
+.. APPEND-TO-LAST-LINE >classification-diff.txt || true
+.. STOP
+
+
+
+.. START command-line-example/expected-classification-diff.txt
+
+That command should show a few alternatives that are not classified the same way by the original and the trained model::
 
-<!-- START command-line-example/expected-classification-diff.txt -->
     2595c2595
     < "Alternative 2594",0.234433308,0.780464768,0.162389532,0.622178912,"Category 2"
     ---
     > "Alternative 2594",0.234433308,0.780464768,0.162389532,0.622178912,"Category 1"
     5000c5000
     < "Alternative 4999",0.074135974,0.496049821,0.672853291,0.782560945,"Category 2"
     ---
@@ -416,55 +506,70 @@
     < "Alternative 9688",0.940304875,0.885046899,0.162586793,0.515185535,"Category 2"
     ---
     > "Alternative 9688",0.940304875,0.885046899,0.162586793,0.515185535,"Category 1"
     9934c9934
     < "Alternative 9933",0.705289483,0.11529737,0.162508503,0.0438248962,"Category 2"
     ---
     > "Alternative 9933",0.705289483,0.11529737,0.162508503,0.0438248962,"Category 1"
-<!-- STOP -->
 
-<!-- EXTEND command-line-example/run.sh --><!--
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     diff expected-classification-diff.txt classification-diff.txt
---><!-- STOP -->
+.. STOP
+
+
 
-You can also measure the classification accuracy of the trained model on that testing set:
+.. EXTEND command-line-example/run.sh
+
+You can also measure the classification accuracy of the trained model on that testing set::
 
-<!-- EXTEND command-line-example/run.sh -->
     lincs classification-accuracy domain.yml trained-model.yml testing-set.csv
-<!-- APPEND-TO-LAST-LINE >classification-accuracy.txt -->
-<!-- STOP -->
 
-It should be close to 100%:
+.. APPEND-TO-LAST-LINE >classification-accuracy.txt
+.. STOP
+
+.. START command-line-example/expected-classification-accuracy.txt
+
+
+
+It should be close to 100%::
 
-<!-- START command-line-example/expected-classification-accuracy.txt -->
     9994/10000
-<!-- STOP -->
 
-<!-- EXTEND command-line-example/run.sh --><!--
+.. STOP
+
+.. EXTEND command-line-example/run.sh
     diff expected-classification-accuracy.txt classification-accuracy.txt
---><!-- STOP -->
+.. STOP
 
 Once you're comfortable with the tooling, you can use a learning set based on real-world data and train a model that you can use to classify new real-world alternatives.
 
-# User guide
+
+User guide
+==========
 
 @todo Write the user guide.
 
-# Reference
+
+Reference
+=========
 
 @todo Generate a reference documentation using Sphinx:
+
 - Python using autodoc
 - C++ using Doxygen+Breath
 - CLI using https://sphinx-click.readthedocs.io/en/latest/
 - YAML file formats using JSON Schema and https://sphinx-jsonschema.readthedocs.io/en/latest/
 
-# Develop *lincs* itself
 
-Run `./run-development-cycle.sh`.
+Develop *lincs* itself
+======================
+
+Run ``./run-development-cycle.sh``.
 
-<!-- Or:
+.. Or:
     docker run --rm -it -v $PWD:/wd --workdir /wd lincs-development
-After changes in C++:
-    pip install --user --no-build-isolation --editable .
-Then test whatever:
-    lincs --help
--->
+    After changes in C++:
+        pip install --user --no-build-isolation --editable .
+    Then test whatever:
+        lincs --help
```

### Comparing `lincs-0.3.3/lincs.egg-info/SOURCES.txt` & `lincs-0.3.5/lincs.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 COPYING
 COPYING.LESSER
 MANIFEST.in
-README.md
+README.rst
 requirements.txt
 setup.py
 lincs/__init__.py
 lincs/__main__.py
 lincs/command_line_interface.py
 lincs/liblincs_module_tests.py
 lincs/visualization.py
```

### Comparing `lincs-0.3.3/setup.py` & `lincs-0.3.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Copyright 2023 Vincent Jacques
 
 import glob
 import setuptools
 
 
-version = "0.3.3"
+version = "0.3.5"
 
-with open("README.md") as f:
+with open("README.rst") as f:
     long_description = f.read()
 for image in ["model", "alternatives"]:
-    long_description = long_description.replace(f"]({image}.png)", f"](https://github.com/MICS-Lab/lincs/raw/v{version}/{image}.png)")
+    long_description = long_description.replace(f".. image:: {image}.png", f".. image:: https://github.com/MICS-Lab/lincs/raw/v{version}/{image}.png")
 for file in ["COPYING", "COPYING.LESSER"]:
-    long_description = long_description.replace(f"]({file})", f"](https://github.com/MICS-Lab/lincs/blob/v{version}/{file})")
+    long_description = long_description.replace(f" <{file}>`_", f" <https://github.com/MICS-Lab/lincs/blob/v{version}/{file}>`_")
+for lang in ["yaml", "shell", "text", "diff"]:
+    long_description = long_description.replace(f".. highlight:: {lang}", "")
 
 with open("requirements.txt") as f:
     install_requires = f.readlines()
 
 
 # @todo Consider using scikit-build:
 # it should make it easier to compile CUDA code using nvcc and to run C++ unit tests during build.
@@ -38,15 +40,15 @@
 
 setuptools.setup(
     name="lincs",
     version=version,
     description="Learn and Infer Non Compensatory Sortings",
     license="LGPLv3",
     long_description=long_description,
-    long_description_content_type="text/markdown",
+    long_description_content_type="text/x-rst",
     url="https://github.com/MICS-Lab/lincs",
     author="Vincent Jacques",
     author_email="vincent@vincent-jacques.net",
     install_requires=install_requires,
     packages=setuptools.find_packages(),
     include_package_data=True,
     entry_points={
```

