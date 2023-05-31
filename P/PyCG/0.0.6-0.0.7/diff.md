# Comparing `tmp/pycg-0.0.6.tar.gz` & `tmp/PyCG-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycg-0.0.6.tar", last modified: Wed Jun 29 18:11:45 2022, max compression
+gzip compressed data, was "PyCG-0.0.7.tar", last modified: Wed May 31 10:42:54 2023, max compression
```

## Comparing `pycg-0.0.6.tar` & `PyCG-0.0.7.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 vitsalis   (501) staff       (20)        0 2022-06-29 18:11:45.673878 pycg-0.0.6/
--rw-r--r--   0 vitsalis   (501) staff       (20)    11357 2022-03-11 08:38:00.000000 pycg-0.0.6/LICENCE
--rw-r--r--   0 vitsalis   (501) staff       (20)     4582 2022-06-29 18:11:45.673936 pycg-0.0.6/PKG-INFO
--rw-r--r--   0 vitsalis   (501) staff       (20)     4167 2022-06-29 18:09:34.000000 pycg-0.0.6/README.md
-drwxr-xr-x   0 vitsalis   (501) staff       (20)        0 2022-06-29 18:11:45.668877 pycg-0.0.6/micro-benchmark/
--rw-r--r--   0 vitsalis   (501) staff       (20)        0 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/__init__.py
--rw-r--r--   0 vitsalis   (501) staff       (20)      710 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/args_test.py
--rw-r--r--   0 vitsalis   (501) staff       (20)      488 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/assignments_test.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     2828 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/base.py
--rw-r--r--   0 vitsalis   (501) staff       (20)      369 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/builtins_test.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     2516 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/classes_test.py
--rwxr-xr-x   0 vitsalis   (501) staff       (20)      998 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/create_pytests.py
--rw-r--r--   0 vitsalis   (501) staff       (20)      799 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/decorators_test.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     1230 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/dicts_test.py
--rw-r--r--   0 vitsalis   (501) staff       (20)      539 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/direct_calls_test.py
--rw-r--r--   0 vitsalis   (501) staff       (20)      183 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/dynamic_test.py
--rw-r--r--   0 vitsalis   (501) staff       (20)      397 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/exceptions_test.py
--rw-r--r--   0 vitsalis   (501) staff       (20)      726 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/external_test.py
--rw-r--r--   0 vitsalis   (501) staff       (20)      522 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/functions_test.py
--rw-r--r--   0 vitsalis   (501) staff       (20)      692 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/generators_test.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     1628 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/imports_test.py
--rw-r--r--   0 vitsalis   (501) staff       (20)      389 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/kwargs_test.py
--rw-r--r--   0 vitsalis   (501) staff       (20)      605 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/lambdas_test.py
--rw-r--r--   0 vitsalis   (501) staff       (20)      904 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/lists_test.py
--rw-r--r--   0 vitsalis   (501) staff       (20)      841 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/mro_test.py
--rw-r--r--   0 vitsalis   (501) staff       (20)      510 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark/returns_test.py
-drwxr-xr-x   0 vitsalis   (501) staff       (20)        0 2022-06-29 18:11:45.669282 pycg-0.0.6/micro-benchmark-key-errs/
--rw-r--r--   0 vitsalis   (501) staff       (20)        0 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark-key-errs/__init__.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     2684 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark-key-errs/base.py
--rwxr-xr-x   0 vitsalis   (501) staff       (20)      998 2022-03-11 08:38:00.000000 pycg-0.0.6/micro-benchmark-key-errs/create_pytests.py
-drwxr-xr-x   0 vitsalis   (501) staff       (20)        0 2022-06-29 18:11:45.669745 pycg-0.0.6/pycg/
--rw-r--r--   0 vitsalis   (501) staff       (20)        0 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/__init__.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     2777 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/__main__.py
-drwxr-xr-x   0 vitsalis   (501) staff       (20)        0 2022-06-29 18:11:45.671235 pycg-0.0.6/pycg/formats/
--rw-r--r--   0 vitsalis   (501) staff       (20)      911 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/formats/__init__.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     1186 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/formats/as_graph.py
--rw-r--r--   0 vitsalis   (501) staff       (20)      956 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/formats/base.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     9877 2022-03-24 19:47:25.000000 pycg-0.0.6/pycg/formats/fasten.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     1162 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/formats/simple.py
-drwxr-xr-x   0 vitsalis   (501) staff       (20)        0 2022-06-29 18:11:45.672374 pycg-0.0.6/pycg/machinery/
--rw-r--r--   0 vitsalis   (501) staff       (20)        0 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/machinery/__init__.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     1794 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/machinery/callgraph.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     2191 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/machinery/classes.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     8207 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/machinery/definitions.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     7080 2022-06-29 18:09:34.000000 pycg-0.0.6/pycg/machinery/imports.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     1171 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/machinery/key_err.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     1996 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/machinery/modules.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     4253 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/machinery/pointers.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     4332 2022-06-29 18:09:34.000000 pycg-0.0.6/pycg/machinery/scopes.py
-drwxr-xr-x   0 vitsalis   (501) staff       (20)        0 2022-06-29 18:11:45.673394 pycg-0.0.6/pycg/processing/
--rw-r--r--   0 vitsalis   (501) staff       (20)        0 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/processing/__init__.py
--rw-r--r--   0 vitsalis   (501) staff       (20)    19892 2022-06-29 18:09:34.000000 pycg-0.0.6/pycg/processing/base.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     9364 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/processing/cgprocessor.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     2995 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/processing/keyerrprocessor.py
--rw-r--r--   0 vitsalis   (501) staff       (20)    12891 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/processing/postprocessor.py
--rw-r--r--   0 vitsalis   (501) staff       (20)    15223 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/processing/preprocessor.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     8097 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/pycg.py
-drwxr-xr-x   0 vitsalis   (501) staff       (20)        0 2022-06-29 18:11:45.673727 pycg-0.0.6/pycg/utils/
--rw-r--r--   0 vitsalis   (501) staff       (20)      873 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/utils/__init__.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     1264 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/utils/common.py
--rw-r--r--   0 vitsalis   (501) staff       (20)     1371 2022-03-11 08:38:00.000000 pycg-0.0.6/pycg/utils/constants.py
-drwxr-xr-x   0 vitsalis   (501) staff       (20)        0 2022-06-29 18:11:45.670317 pycg-0.0.6/pycg.egg-info/
--rw-r--r--   0 vitsalis   (501) staff       (20)     4582 2022-06-29 18:11:45.000000 pycg-0.0.6/pycg.egg-info/PKG-INFO
--rw-r--r--   0 vitsalis   (501) staff       (20)     1620 2022-06-29 18:11:45.000000 pycg-0.0.6/pycg.egg-info/SOURCES.txt
--rw-r--r--   0 vitsalis   (501) staff       (20)        1 2022-06-29 18:11:45.000000 pycg-0.0.6/pycg.egg-info/dependency_links.txt
--rw-r--r--   0 vitsalis   (501) staff       (20)       44 2022-06-29 18:11:45.000000 pycg-0.0.6/pycg.egg-info/entry_points.txt
--rw-r--r--   0 vitsalis   (501) staff       (20)       46 2022-06-29 18:11:45.000000 pycg-0.0.6/pycg.egg-info/top_level.txt
--rw-r--r--   0 vitsalis   (501) staff       (20)       79 2022-06-29 18:11:45.674121 pycg-0.0.6/setup.cfg
--rw-r--r--   0 vitsalis   (501) staff       (20)     1844 2022-06-29 18:09:53.000000 pycg-0.0.6/setup.py
+drwxr-xr-x   0 vitsalis   (501) staff       (20)        0 2023-05-31 10:42:54.364496 PyCG-0.0.7/
+-rw-r--r--   0 vitsalis   (501) staff       (20)    11357 2022-03-11 08:38:00.000000 PyCG-0.0.7/LICENCE
+-rw-r--r--   0 vitsalis   (501) staff       (20)     5142 2023-05-31 10:42:54.364577 PyCG-0.0.7/PKG-INFO
+drwxr-xr-x   0 vitsalis   (501) staff       (20)        0 2023-05-31 10:42:54.356176 PyCG-0.0.7/PyCG.egg-info/
+-rw-r--r--   0 vitsalis   (501) staff       (20)     5142 2023-05-31 10:42:54.000000 PyCG-0.0.7/PyCG.egg-info/PKG-INFO
+-rw-r--r--   0 vitsalis   (501) staff       (20)     1778 2023-05-31 10:42:54.000000 PyCG-0.0.7/PyCG.egg-info/SOURCES.txt
+-rw-r--r--   0 vitsalis   (501) staff       (20)        1 2023-05-31 10:42:54.000000 PyCG-0.0.7/PyCG.egg-info/dependency_links.txt
+-rw-r--r--   0 vitsalis   (501) staff       (20)       44 2023-05-31 10:42:54.000000 PyCG-0.0.7/PyCG.egg-info/entry_points.txt
+-rw-r--r--   0 vitsalis   (501) staff       (20)       46 2023-05-31 10:42:54.000000 PyCG-0.0.7/PyCG.egg-info/top_level.txt
+-rw-r--r--   0 vitsalis   (501) staff       (20)     4597 2023-05-31 09:06:35.000000 PyCG-0.0.7/README.md
+drwxr-xr-x   0 vitsalis   (501) staff       (20)        0 2023-05-31 10:42:54.359663 PyCG-0.0.7/micro-benchmark/
+-rw-r--r--   0 vitsalis   (501) staff       (20)        0 2022-03-11 08:38:00.000000 PyCG-0.0.7/micro-benchmark/__init__.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)      710 2023-05-31 09:06:35.000000 PyCG-0.0.7/micro-benchmark/args_test.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)      488 2023-05-31 09:06:35.000000 PyCG-0.0.7/micro-benchmark/assignments_test.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     3067 2023-05-31 09:06:35.000000 PyCG-0.0.7/micro-benchmark/base.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)      369 2023-05-31 09:06:35.000000 PyCG-0.0.7/micro-benchmark/builtins_test.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     2516 2023-05-31 09:06:35.000000 PyCG-0.0.7/micro-benchmark/classes_test.py
+-rwxr-xr-x   0 vitsalis   (501) staff       (20)      998 2022-03-11 08:38:00.000000 PyCG-0.0.7/micro-benchmark/create_pytests.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)      799 2023-05-31 09:06:35.000000 PyCG-0.0.7/micro-benchmark/decorators_test.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     1230 2023-05-31 09:06:35.000000 PyCG-0.0.7/micro-benchmark/dicts_test.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)      539 2023-05-31 09:06:35.000000 PyCG-0.0.7/micro-benchmark/direct_calls_test.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)      183 2022-03-11 08:38:00.000000 PyCG-0.0.7/micro-benchmark/dynamic_test.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)      397 2023-05-31 09:06:35.000000 PyCG-0.0.7/micro-benchmark/exceptions_test.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)      726 2023-05-31 09:06:35.000000 PyCG-0.0.7/micro-benchmark/external_test.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)      522 2023-05-31 09:06:35.000000 PyCG-0.0.7/micro-benchmark/functions_test.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)      692 2023-05-31 09:06:35.000000 PyCG-0.0.7/micro-benchmark/generators_test.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     1628 2023-05-31 09:06:35.000000 PyCG-0.0.7/micro-benchmark/imports_test.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)      389 2023-05-31 09:06:35.000000 PyCG-0.0.7/micro-benchmark/kwargs_test.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)      605 2023-05-31 09:06:35.000000 PyCG-0.0.7/micro-benchmark/lambdas_test.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)      904 2023-05-31 09:06:35.000000 PyCG-0.0.7/micro-benchmark/lists_test.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)      841 2023-05-31 09:06:35.000000 PyCG-0.0.7/micro-benchmark/mro_test.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)      510 2023-05-31 09:06:35.000000 PyCG-0.0.7/micro-benchmark/returns_test.py
+drwxr-xr-x   0 vitsalis   (501) staff       (20)        0 2023-05-31 10:42:54.360129 PyCG-0.0.7/micro-benchmark-key-errs/
+-rw-r--r--   0 vitsalis   (501) staff       (20)        0 2023-05-09 10:24:30.000000 PyCG-0.0.7/micro-benchmark-key-errs/__init__.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     2684 2023-05-09 10:24:30.000000 PyCG-0.0.7/micro-benchmark-key-errs/base.py
+-rwxr-xr-x   0 vitsalis   (501) staff       (20)      998 2023-05-09 10:24:30.000000 PyCG-0.0.7/micro-benchmark-key-errs/create_pytests.py
+drwxr-xr-x   0 vitsalis   (501) staff       (20)        0 2023-05-31 10:42:54.360724 PyCG-0.0.7/pycg/
+-rw-r--r--   0 vitsalis   (501) staff       (20)        0 2022-03-11 08:38:00.000000 PyCG-0.0.7/pycg/__init__.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     2640 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/__main__.py
+drwxr-xr-x   0 vitsalis   (501) staff       (20)        0 2023-05-31 10:42:54.361975 PyCG-0.0.7/pycg/formats/
+-rw-r--r--   0 vitsalis   (501) staff       (20)      953 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/formats/__init__.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     1187 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/formats/as_graph.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)      956 2022-03-11 08:38:00.000000 PyCG-0.0.7/pycg/formats/base.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     9805 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/formats/fasten.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     1163 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/formats/simple.py
+drwxr-xr-x   0 vitsalis   (501) staff       (20)        0 2023-05-31 10:42:54.363094 PyCG-0.0.7/pycg/machinery/
+-rw-r--r--   0 vitsalis   (501) staff       (20)        0 2022-03-11 08:38:00.000000 PyCG-0.0.7/pycg/machinery/__init__.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     1794 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/machinery/callgraph.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     2195 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/machinery/classes.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     8289 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/machinery/definitions.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     7222 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/machinery/imports.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     1135 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/machinery/key_err.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     1936 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/machinery/modules.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     4250 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/machinery/pointers.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     4359 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/machinery/scopes.py
+drwxr-xr-x   0 vitsalis   (501) staff       (20)        0 2023-05-31 10:42:54.363974 PyCG-0.0.7/pycg/processing/
+-rw-r--r--   0 vitsalis   (501) staff       (20)        0 2022-03-11 08:38:00.000000 PyCG-0.0.7/pycg/processing/__init__.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)    20323 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/processing/base.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     9519 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/processing/cgprocessor.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     3174 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/processing/keyerrprocessor.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)    13459 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/processing/postprocessor.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)    16198 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/processing/preprocessor.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     8636 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/pycg.py
+drwxr-xr-x   0 vitsalis   (501) staff       (20)        0 2023-05-31 10:42:54.364352 PyCG-0.0.7/pycg/utils/
+-rw-r--r--   0 vitsalis   (501) staff       (20)      895 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/utils/__init__.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     1270 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/utils/common.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)     1284 2023-05-31 09:06:35.000000 PyCG-0.0.7/pycg/utils/constants.py
+-rw-r--r--   0 vitsalis   (501) staff       (20)      894 2023-05-31 10:42:52.000000 PyCG-0.0.7/pyproject.toml
+-rw-r--r--   0 vitsalis   (501) staff       (20)       79 2023-05-31 10:42:54.364813 PyCG-0.0.7/setup.cfg
+-rw-r--r--   0 vitsalis   (501) staff       (20)     1843 2023-05-31 10:42:52.000000 PyCG-0.0.7/setup.py
```

### Comparing `pycg-0.0.6/LICENCE` & `PyCG-0.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `pycg-0.0.6/PKG-INFO` & `PyCG-0.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,21 @@
-Metadata-Version: 2.1
-Name: pycg
-Version: 0.0.6
-Summary: Practical Python Call Graphs
-Home-page: https://github.com/vitsalis/pycg
-Author: Vitalis Salis
-Author-email: vitsalis@gmail.com
-License: Apache Software License
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.4
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
 # PyCG - Practical Python Call Graphs
 
+[![Linters](https://github.com/vitsalis/PyCG/actions/workflows/linters.yml/badge.svg)](https://github.com/vitsalis/PyCG/actions/workflows/linters.yml)
+[![Tests](https://github.com/vitsalis/PyCG/actions/workflows/test.yaml/badge.svg)](https://github.com/vitsalis/PyCG/actions/workflows/test.yaml)
+
 PyCG generates call graphs for Python code using static analysis.
 It efficiently supports
 * Higher order functions
 * Twisted class inheritance schemes
 * Automatic discovery of imported modules for further analysis
 * Nested definitions
 
 You can read the full methodology as well as a complete evaluation on the
-[ICSE 2021 paper](https://vitsalis.com/papers/pycg.pdf).
+[ICSE 2021 paper](https://arxiv.org/pdf/2103.00587.pdf).
 
 You can cite PyCG as follows.
 Vitalis Salis, Thodoris Sotiropoulos, Panos Louridas, Diomidis Spinellis and Dimitris Mitropoulos.
 PyCG: Practical Call Graph Generation in Python.
 In _43rd International Conference on Software Engineering, ICSE '21_,
 25–28 May 2021.
 
@@ -140,11 +129,15 @@
 ~ >>> pycg --package pypi_pkg --fasten --product "pypipkg" --forge "PyPI" \
         --version "0.1" --timestamp 42 \
         pypi_pkg/module1.py pkg_root/subpackage/module2.py -o cg.json
 ```
 
 # Running Tests
 
-From the root directory:
+From the root directory, first install the [mock](https://pypi.org/project/mock/) package:
 ```
-make test
+pip3 install mock
 ```
+Τhen, simply run the tests by executing:
+```
+make test
+```
```

### Comparing `pycg-0.0.6/README.md` & `PyCG-0.0.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,37 @@
+Metadata-Version: 2.1
+Name: PyCG
+Version: 0.0.7
+Summary: PyCG - Practical Python Call Graphs
+Home-page: https://github.com/vitsalis/pycg
+Author: Vitalis Salis
+Author-email: vitsalis@gmail.com
+License: Apache Software License
+Project-URL: Homepage, https://github.com/vitsalis/PyCG
+Project-URL: Bug Tracker, https://github.com/vitsalis/PyCG/issues
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.4
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
 # PyCG - Practical Python Call Graphs
 
+[![Linters](https://github.com/vitsalis/PyCG/actions/workflows/linters.yml/badge.svg)](https://github.com/vitsalis/PyCG/actions/workflows/linters.yml)
+[![Tests](https://github.com/vitsalis/PyCG/actions/workflows/test.yaml/badge.svg)](https://github.com/vitsalis/PyCG/actions/workflows/test.yaml)
+
 PyCG generates call graphs for Python code using static analysis.
 It efficiently supports
 * Higher order functions
 * Twisted class inheritance schemes
 * Automatic discovery of imported modules for further analysis
 * Nested definitions
 
 You can read the full methodology as well as a complete evaluation on the
-[ICSE 2021 paper](https://vitsalis.com/papers/pycg.pdf).
+[ICSE 2021 paper](https://arxiv.org/pdf/2103.00587.pdf).
 
 You can cite PyCG as follows.
 Vitalis Salis, Thodoris Sotiropoulos, Panos Louridas, Diomidis Spinellis and Dimitris Mitropoulos.
 PyCG: Practical Call Graph Generation in Python.
 In _43rd International Conference on Software Engineering, ICSE '21_,
 25–28 May 2021.
 
@@ -126,11 +145,15 @@
 ~ >>> pycg --package pypi_pkg --fasten --product "pypipkg" --forge "PyPI" \
         --version "0.1" --timestamp 42 \
         pypi_pkg/module1.py pkg_root/subpackage/module2.py -o cg.json
 ```
 
 # Running Tests
 
-From the root directory:
+From the root directory, first install the [mock](https://pypi.org/project/mock/) package:
+```
+pip3 install mock
+```
+Τhen, simply run the tests by executing:
 ```
 make test
 ```
```

### Comparing `pycg-0.0.6/micro-benchmark/args_test.py` & `PyCG-0.0.7/micro-benchmark/args_test.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-
 import os
 
 from base import TestBase
 
+
 class ArgsTest(TestBase):
     snippet_dir = "args"
 
-    def test_nested_call(self):
-        self.validate_snippet(self.get_snippet_path("nested_call"))
-
-    def test_param_call(self):
-        self.validate_snippet(self.get_snippet_path("param_call"))
-
     def test_assigned_call(self):
         self.validate_snippet(self.get_snippet_path("assigned_call"))
 
-    def test_imported_call(self):
-        self.validate_snippet(self.get_snippet_path("imported_call"))
+    def test_call(self):
+        self.validate_snippet(self.get_snippet_path("call"))
 
     def test_imported_assigned_call(self):
         self.validate_snippet(self.get_snippet_path("imported_assigned_call"))
 
-    def test_call(self):
-        self.validate_snippet(self.get_snippet_path("call"))
+    def test_imported_call(self):
+        self.validate_snippet(self.get_snippet_path("imported_call"))
+
+    def test_nested_call(self):
+        self.validate_snippet(self.get_snippet_path("nested_call"))
+
+    def test_param_call(self):
+        self.validate_snippet(self.get_snippet_path("param_call"))
```

### Comparing `pycg-0.0.6/micro-benchmark/base.py` & `PyCG-0.0.7/micro-benchmark-key-errs/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2020 Vitalis Salis.
+# Copyright (c) 2021 Vitalis Salis.
 #
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
@@ -57,31 +57,25 @@
 
     def get_snippet_path(self, name):
         return os.path.join(self.snippets_path, self.snippet_dir, name)
 
     def get_snippet_output_cg(self, snippet_path):
         main_path = os.path.join(snippet_path, "main.py")
         try:
-            cg = self.cg_class([main_path], snippet_path, -1, utils.constants.CALL_GRAPH_OP)
+            cg = self.cg_class([main_path], snippet_path, -1, utils.constants.KEY_ERR_OP)
             cg.analyze()
-            return cg.output()
+            return cg.output_key_errs()
         except Exception as e:
             cg.tearDown()
             raise e
 
     def get_snippet_expected_cg(self, snippet_path):
-        cg_path = os.path.join(snippet_path, "callgraph.json")
+        cg_path = os.path.join(snippet_path, "key_errs.json")
         with open(cg_path, "r") as f:
             return json.loads(f.read())
 
     def assertEqual(self, actual, expected):
-        def do_sorted(d):
-            s = {}
-            for n in d:
-                s[n] = sorted(d[n])
-            return s
-
-        super().assertEqual(do_sorted(actual), do_sorted(expected))
+        super().assertEqual(actual, expected)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pycg-0.0.6/micro-benchmark/classes_test.py` & `PyCG-0.0.7/micro-benchmark/classes_test.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-
 import os
 
 from base import TestBase
 
+
 class ClassesTest(TestBase):
     snippet_dir = "classes"
 
-    def test_imported_call_without_init(self):
-        self.validate_snippet(self.get_snippet_path("imported_call_without_init"))
-
-    def test_direct_call(self):
-        self.validate_snippet(self.get_snippet_path("direct_call"))
-
-    def test_return_call_direct(self):
-        self.validate_snippet(self.get_snippet_path("return_call_direct"))
+    def test_assigned_call(self):
+        self.validate_snippet(self.get_snippet_path("assigned_call"))
 
-    def test_nested_class_calls(self):
-        self.validate_snippet(self.get_snippet_path("nested_class_calls"))
+    def test_assigned_self_call(self):
+        self.validate_snippet(self.get_snippet_path("assigned_self_call"))
 
-    def test_super_class_return(self):
-        self.validate_snippet(self.get_snippet_path("super_class_return"))
+    def test_base_class_attr(self):
+        self.validate_snippet(self.get_snippet_path("base_class_attr"))
 
     def test_base_class_calls_child(self):
         self.validate_snippet(self.get_snippet_path("base_class_calls_child"))
 
-    def test_tuple_assignment(self):
-        self.validate_snippet(self.get_snippet_path("tuple_assignment"))
-
-    def test_return_call(self):
-        self.validate_snippet(self.get_snippet_path("return_call"))
+    def test_call(self):
+        self.validate_snippet(self.get_snippet_path("call"))
 
-    def test_nested_call(self):
-        self.validate_snippet(self.get_snippet_path("nested_call"))
+    def test_direct_call(self):
+        self.validate_snippet(self.get_snippet_path("direct_call"))
 
     def test_imported_attr_access(self):
         self.validate_snippet(self.get_snippet_path("imported_attr_access"))
 
-    def test_assigned_call(self):
-        self.validate_snippet(self.get_snippet_path("assigned_call"))
-
-    def test_self_assign_func(self):
-        self.validate_snippet(self.get_snippet_path("self_assign_func"))
-
     def test_imported_call(self):
         self.validate_snippet(self.get_snippet_path("imported_call"))
 
-    def test_base_class_attr(self):
-        self.validate_snippet(self.get_snippet_path("base_class_attr"))
-
-    def test_static_method_call(self):
-        self.validate_snippet(self.get_snippet_path("static_method_call"))
+    def test_imported_call_without_init(self):
+        self.validate_snippet(self.get_snippet_path("imported_call_without_init"))
 
-    def test_call(self):
-        self.validate_snippet(self.get_snippet_path("call"))
+    def test_imported_nested_attr_access(self):
+        self.validate_snippet(self.get_snippet_path("imported_nested_attr_access"))
 
     def test_instance(self):
         self.validate_snippet(self.get_snippet_path("instance"))
 
-    def test_imported_nested_attr_access(self):
-        self.validate_snippet(self.get_snippet_path("imported_nested_attr_access"))
+    def test_nested_call(self):
+        self.validate_snippet(self.get_snippet_path("nested_call"))
+
+    def test_nested_class_calls(self):
+        self.validate_snippet(self.get_snippet_path("nested_class_calls"))
 
     def test_parameter_call(self):
         self.validate_snippet(self.get_snippet_path("parameter_call"))
 
+    def test_return_call(self):
+        self.validate_snippet(self.get_snippet_path("return_call"))
+
+    def test_return_call_direct(self):
+        self.validate_snippet(self.get_snippet_path("return_call_direct"))
+
     def test_self_assignment(self):
         self.validate_snippet(self.get_snippet_path("self_assignment"))
 
+    def test_self_assign_func(self):
+        self.validate_snippet(self.get_snippet_path("self_assign_func"))
+
     def test_self_call(self):
         self.validate_snippet(self.get_snippet_path("self_call"))
 
-    def test_assigned_self_call(self):
-        self.validate_snippet(self.get_snippet_path("assigned_self_call"))
+    def test_static_method_call(self):
+        self.validate_snippet(self.get_snippet_path("static_method_call"))
+
+    def test_super_class_return(self):
+        self.validate_snippet(self.get_snippet_path("super_class_return"))
+
+    def test_tuple_assignment(self):
+        self.validate_snippet(self.get_snippet_path("tuple_assignment"))
```

### Comparing `pycg-0.0.6/micro-benchmark/create_pytests.py` & `PyCG-0.0.7/micro-benchmark/create_pytests.py`

 * *Files identical despite different names*

### Comparing `pycg-0.0.6/micro-benchmark/decorators_test.py` & `PyCG-0.0.7/micro-benchmark/decorators_test.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-
 import os
 
 from base import TestBase
 
+
 class DecoratorsTest(TestBase):
     snippet_dir = "decorators"
 
-    def test_return_different_func(self):
-        self.validate_snippet(self.get_snippet_path("return_different_func"))
+    def test_assigned(self):
+        self.validate_snippet(self.get_snippet_path("assigned"))
 
-    def test_param_call(self):
-        self.validate_snippet(self.get_snippet_path("param_call"))
+    def test_call(self):
+        self.validate_snippet(self.get_snippet_path("call"))
+
+    def test_nested(self):
+        self.validate_snippet(self.get_snippet_path("nested"))
 
     def test_nested_decorators(self):
         self.validate_snippet(self.get_snippet_path("nested_decorators"))
 
-    def test_assigned(self):
-        self.validate_snippet(self.get_snippet_path("assigned"))
+    def test_param_call(self):
+        self.validate_snippet(self.get_snippet_path("param_call"))
 
     def test_return(self):
         self.validate_snippet(self.get_snippet_path("return"))
 
-    def test_call(self):
-        self.validate_snippet(self.get_snippet_path("call"))
-
-    def test_nested(self):
-        self.validate_snippet(self.get_snippet_path("nested"))
+    def test_return_different_func(self):
+        self.validate_snippet(self.get_snippet_path("return_different_func"))
```

### Comparing `pycg-0.0.6/micro-benchmark/dicts_test.py` & `PyCG-0.0.7/micro-benchmark/dicts_test.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-
 import os
 
 from base import TestBase
 
+
 class DictsTest(TestBase):
     snippet_dir = "dicts"
 
-    def test_type_coercion(self):
-        self.validate_snippet(self.get_snippet_path("type_coercion"))
+    def test_add_key(self):
+        self.validate_snippet(self.get_snippet_path("add_key"))
 
-    def test_update(self):
-        self.validate_snippet(self.get_snippet_path("update"))
+    def test_assign(self):
+        self.validate_snippet(self.get_snippet_path("assign"))
+
+    def test_call(self):
+        self.validate_snippet(self.get_snippet_path("call"))
 
     def test_ext_key(self):
         self.validate_snippet(self.get_snippet_path("ext_key"))
 
-    def test_return(self):
-        self.validate_snippet(self.get_snippet_path("return"))
+    def test_nested(self):
+        self.validate_snippet(self.get_snippet_path("nested"))
+
+    def test_new_key_param(self):
+        self.validate_snippet(self.get_snippet_path("new_key_param"))
 
     def test_param(self):
         self.validate_snippet(self.get_snippet_path("param"))
 
-    def test_return_assign(self):
-        self.validate_snippet(self.get_snippet_path("return_assign"))
-
-    def test_call(self):
-        self.validate_snippet(self.get_snippet_path("call"))
-
-    def test_assign(self):
-        self.validate_snippet(self.get_snippet_path("assign"))
-
     def test_param_key(self):
         self.validate_snippet(self.get_snippet_path("param_key"))
 
-    def test_new_key_param(self):
-        self.validate_snippet(self.get_snippet_path("new_key_param"))
+    def test_return(self):
+        self.validate_snippet(self.get_snippet_path("return"))
 
-    def test_nested(self):
-        self.validate_snippet(self.get_snippet_path("nested"))
+    def test_return_assign(self):
+        self.validate_snippet(self.get_snippet_path("return_assign"))
 
-    def test_add_key(self):
-        self.validate_snippet(self.get_snippet_path("add_key"))
+    def test_type_coercion(self):
+        self.validate_snippet(self.get_snippet_path("type_coercion"))
+
+    def test_update(self):
+        self.validate_snippet(self.get_snippet_path("update"))
```

### Comparing `pycg-0.0.6/micro-benchmark/direct_calls_test.py` & `PyCG-0.0.7/micro-benchmark/direct_calls_test.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-
 import os
 
 from base import TestBase
 
+
 class DirectCallsTest(TestBase):
     snippet_dir = "direct_calls"
 
-    def test_with_parameters(self):
-        self.validate_snippet(self.get_snippet_path("with_parameters"))
+    def test_assigned_call(self):
+        self.validate_snippet(self.get_snippet_path("assigned_call"))
 
     def test_imported_return_call(self):
         self.validate_snippet(self.get_snippet_path("imported_return_call"))
 
     def test_return_call(self):
         self.validate_snippet(self.get_snippet_path("return_call"))
 
-    def test_assigned_call(self):
-        self.validate_snippet(self.get_snippet_path("assigned_call"))
+    def test_with_parameters(self):
+        self.validate_snippet(self.get_snippet_path("with_parameters"))
```

### Comparing `pycg-0.0.6/micro-benchmark/external_test.py` & `PyCG-0.0.7/micro-benchmark/external_test.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-
 import os
 
 from base import TestBase
 
+
 class ExternalTest(TestBase):
     snippet_dir = "external"
 
     def test_attribute(self):
         self.validate_snippet(self.get_snippet_path("attribute"))
 
-    def test_function_assigned(self):
-        self.validate_snippet(self.get_snippet_path("function_assigned"))
-
     def test_attribute_assigned(self):
         self.validate_snippet(self.get_snippet_path("attribute_assigned"))
 
-    def test_function_asname(self):
-        self.validate_snippet(self.get_snippet_path("function_asname"))
+    def test_cls_parent(self):
+        self.validate_snippet(self.get_snippet_path("cls_parent"))
 
     def test_function(self):
         self.validate_snippet(self.get_snippet_path("function"))
 
-    def test_cls_parent(self):
-        self.validate_snippet(self.get_snippet_path("cls_parent"))
+    def test_function_asname(self):
+        self.validate_snippet(self.get_snippet_path("function_asname"))
+
+    def test_function_assigned(self):
+        self.validate_snippet(self.get_snippet_path("function_assigned"))
```

### Comparing `pycg-0.0.6/micro-benchmark/functions_test.py` & `PyCG-0.0.7/micro-benchmark/functions_test.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-
 import os
 
 from base import TestBase
 
+
 class FunctionsTest(TestBase):
     snippet_dir = "functions"
 
     def test_assigned_call(self):
         self.validate_snippet(self.get_snippet_path("assigned_call"))
 
-    def test_imported_call(self):
-        self.validate_snippet(self.get_snippet_path("imported_call"))
+    def test_assigned_call_lit_param(self):
+        self.validate_snippet(self.get_snippet_path("assigned_call_lit_param"))
 
     def test_call(self):
         self.validate_snippet(self.get_snippet_path("call"))
 
-    def test_assigned_call_lit_param(self):
-        self.validate_snippet(self.get_snippet_path("assigned_call_lit_param"))
+    def test_imported_call(self):
+        self.validate_snippet(self.get_snippet_path("imported_call"))
```

### Comparing `pycg-0.0.6/micro-benchmark/generators_test.py` & `PyCG-0.0.7/micro-benchmark/generators_test.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-
 import os
 
 from base import TestBase
 
+
 class GeneratorsTest(TestBase):
     snippet_dir = "generators"
 
+    def test_iterable(self):
+        self.validate_snippet(self.get_snippet_path("iterable"))
+
+    def test_iterable_assigned(self):
+        self.validate_snippet(self.get_snippet_path("iterable_assigned"))
+
     def test_iter_param(self):
         self.validate_snippet(self.get_snippet_path("iter_param"))
 
-    def test_no_iter(self):
-        self.validate_snippet(self.get_snippet_path("no_iter"))
-
     def test_iter_return(self):
         self.validate_snippet(self.get_snippet_path("iter_return"))
 
-    def test_iterable(self):
-        self.validate_snippet(self.get_snippet_path("iterable"))
-
-    def test_iterable_assigned(self):
-        self.validate_snippet(self.get_snippet_path("iterable_assigned"))
+    def test_no_iter(self):
+        self.validate_snippet(self.get_snippet_path("no_iter"))
 
     def test_yield(self):
         self.validate_snippet(self.get_snippet_path("yield"))
```

### Comparing `pycg-0.0.6/micro-benchmark/imports_test.py` & `PyCG-0.0.7/micro-benchmark/imports_test.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-
 import os
 
 from base import TestBase
 
+
 class ImportsTest(TestBase):
     snippet_dir = "imports"
 
-    def test_relative_import_with_name(self):
-        self.validate_snippet(self.get_snippet_path("relative_import_with_name"))
+    def test_chained_import(self):
+        self.validate_snippet(self.get_snippet_path("chained_import"))
 
-    def test_submodule_import_from(self):
-        self.validate_snippet(self.get_snippet_path("submodule_import_from"))
+    def test_import_all(self):
+        self.validate_snippet(self.get_snippet_path("import_all"))
 
     def test_import_as(self):
         self.validate_snippet(self.get_snippet_path("import_as"))
 
-    def test_submodule_import_all(self):
-        self.validate_snippet(self.get_snippet_path("submodule_import_all"))
-
-    def test_parent_import(self):
-        self.validate_snippet(self.get_snippet_path("parent_import"))
-
-    def test_chained_import(self):
-        self.validate_snippet(self.get_snippet_path("chained_import"))
+    def test_import_from(self):
+        self.validate_snippet(self.get_snippet_path("import_from"))
 
     def test_init_func_import(self):
         self.validate_snippet(self.get_snippet_path("init_func_import"))
 
-    def test_submodule_import_as(self):
-        self.validate_snippet(self.get_snippet_path("submodule_import_as"))
+    def test_init_import(self):
+        self.validate_snippet(self.get_snippet_path("init_import"))
+
+    def test_parent_import(self):
+        self.validate_snippet(self.get_snippet_path("parent_import"))
 
     def test_relative_import(self):
         self.validate_snippet(self.get_snippet_path("relative_import"))
 
-    def test_import_all(self):
-        self.validate_snippet(self.get_snippet_path("import_all"))
+    def test_relative_import_with_name(self):
+        self.validate_snippet(self.get_snippet_path("relative_import_with_name"))
 
     def test_simple_import(self):
         self.validate_snippet(self.get_snippet_path("simple_import"))
 
-    def test_init_import(self):
-        self.validate_snippet(self.get_snippet_path("init_import"))
-
     def test_submodule_import(self):
         self.validate_snippet(self.get_snippet_path("submodule_import"))
 
-    def test_import_from(self):
-        self.validate_snippet(self.get_snippet_path("import_from"))
+    def test_submodule_import_all(self):
+        self.validate_snippet(self.get_snippet_path("submodule_import_all"))
+
+    def test_submodule_import_as(self):
+        self.validate_snippet(self.get_snippet_path("submodule_import_as"))
+
+    def test_submodule_import_from(self):
+        self.validate_snippet(self.get_snippet_path("submodule_import_from"))
```

### Comparing `pycg-0.0.6/micro-benchmark/lambdas_test.py` & `PyCG-0.0.7/micro-benchmark/lambdas_test.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-
 import os
 
 from base import TestBase
 
+
 class LambdasTest(TestBase):
     snippet_dir = "lambdas"
 
+    def test_call(self):
+        self.validate_snippet(self.get_snippet_path("call"))
+
     def test_calls_parameter(self):
         self.validate_snippet(self.get_snippet_path("calls_parameter"))
 
-    def test_return_call(self):
-        self.validate_snippet(self.get_snippet_path("return_call"))
-
-    def test_call(self):
-        self.validate_snippet(self.get_snippet_path("call"))
+    def test_chained_calls(self):
+        self.validate_snippet(self.get_snippet_path("chained_calls"))
 
     def test_parameter_call(self):
         self.validate_snippet(self.get_snippet_path("parameter_call"))
 
-    def test_chained_calls(self):
-        self.validate_snippet(self.get_snippet_path("chained_calls"))
+    def test_return_call(self):
+        self.validate_snippet(self.get_snippet_path("return_call"))
```

### Comparing `pycg-0.0.6/micro-benchmark/lists_test.py` & `PyCG-0.0.7/micro-benchmark/lists_test.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-
 import os
 
 from base import TestBase
 
+
 class ListsTest(TestBase):
     snippet_dir = "lists"
 
+    def test_comprehension_if(self):
+        self.validate_snippet(self.get_snippet_path("comprehension_if"))
+
     def test_comprehension_val(self):
         self.validate_snippet(self.get_snippet_path("comprehension_val"))
 
-    def test_slice(self):
-        self.validate_snippet(self.get_snippet_path("slice"))
-
-    def test_simple(self):
-        self.validate_snippet(self.get_snippet_path("simple"))
+    def test_ext_index(self):
+        self.validate_snippet(self.get_snippet_path("ext_index"))
 
-    def test_comprehension_if(self):
-        self.validate_snippet(self.get_snippet_path("comprehension_if"))
+    def test_nested(self):
+        self.validate_snippet(self.get_snippet_path("nested"))
 
     def test_nested_comprehension(self):
         self.validate_snippet(self.get_snippet_path("nested_comprehension"))
 
     def test_param_index(self):
         self.validate_snippet(self.get_snippet_path("param_index"))
 
-    def test_nested(self):
-        self.validate_snippet(self.get_snippet_path("nested"))
+    def test_simple(self):
+        self.validate_snippet(self.get_snippet_path("simple"))
 
-    def test_ext_index(self):
-        self.validate_snippet(self.get_snippet_path("ext_index"))
+    def test_slice(self):
+        self.validate_snippet(self.get_snippet_path("slice"))
```

### Comparing `pycg-0.0.6/micro-benchmark/mro_test.py` & `PyCG-0.0.7/micro-benchmark/mro_test.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-
 import os
 
 from base import TestBase
 
+
 class MroTest(TestBase):
     snippet_dir = "mro"
 
+    def test_basic(self):
+        self.validate_snippet(self.get_snippet_path("basic"))
+
     def test_basic_init(self):
         self.validate_snippet(self.get_snippet_path("basic_init"))
 
     def test_parents_same_superclass(self):
         self.validate_snippet(self.get_snippet_path("parents_same_superclass"))
 
-    def test_basic(self):
-        self.validate_snippet(self.get_snippet_path("basic"))
-
-    def test_two_parents(self):
-        self.validate_snippet(self.get_snippet_path("two_parents"))
+    def test_self_assignment(self):
+        self.validate_snippet(self.get_snippet_path("self_assignment"))
 
     def test_super_call(self):
         self.validate_snippet(self.get_snippet_path("super_call"))
 
-    def test_self_assignment(self):
-        self.validate_snippet(self.get_snippet_path("self_assignment"))
+    def test_two_parents(self):
+        self.validate_snippet(self.get_snippet_path("two_parents"))
 
     def test_two_parents_method_defined(self):
         self.validate_snippet(self.get_snippet_path("two_parents_method_defined"))
```

### Comparing `pycg-0.0.6/micro-benchmark-key-errs/base.py` & `PyCG-0.0.7/micro-benchmark/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2021 Vitalis Salis.
+# Copyright (c) 2020 Vitalis Salis.
 #
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
@@ -14,34 +14,43 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
-import os
-import sys
 import importlib
 import json
-
+import os
+import sys
+from os.path import abspath, dirname
 from unittest import TestCase, main
+
 from pycg import utils
 
+SCRIPT_DIR = dirname(abspath(__file__))
+
+
 class TestBase(TestCase):
     snippet_dir = ""
 
     def setUp(self):
         def error():
-            print ("Invalid module %s.%s" % (cg_mod, cg_class))
-            print ("Set environment variables `CALL_GRAPH_CLASS` and `CALL_GRAPH_MODULE` properly")
+            print("Invalid module %s.%s" % (cg_mod, cg_class))
+            print(
+                "Set environment variables `CALL_GRAPH_CLASS` and `CALL_GRAPH_MODULE`"
+                " properly"
+            )
             sys.exit(1)
 
-        self.snippets_path = os.environ.get("SNIPPETS_PATH")
-        cg_class = os.environ.get('CALL_GRAPH_CLASS', None)
-        cg_mod = os.environ.get('CALL_GRAPH_MODULE', None)
+        self.snippets_path = os.environ.get(
+            "SNIPPETS_PATH", os.path.join(SCRIPT_DIR, "snippets")
+        )
+        cg_class = os.environ.get("CALL_GRAPH_CLASS", "CallGraphGenerator")
+        cg_mod = os.environ.get("CALL_GRAPH_MODULE", "pycg.pycg")
         if not cg_class or not cg_mod:
             error()
         try:
             self.cg_mod = importlib.import_module(cg_mod)
         except ImportError:
             error()
 
@@ -57,25 +66,33 @@
 
     def get_snippet_path(self, name):
         return os.path.join(self.snippets_path, self.snippet_dir, name)
 
     def get_snippet_output_cg(self, snippet_path):
         main_path = os.path.join(snippet_path, "main.py")
         try:
-            cg = self.cg_class([main_path], snippet_path, -1, utils.constants.KEY_ERR_OP)
+            cg = self.cg_class(
+                [main_path], snippet_path, -1, utils.constants.CALL_GRAPH_OP
+            )
             cg.analyze()
-            return cg.output_key_errs()
+            return cg.output()
         except Exception as e:
             cg.tearDown()
             raise e
 
     def get_snippet_expected_cg(self, snippet_path):
-        cg_path = os.path.join(snippet_path, "key_errs.json")
+        cg_path = os.path.join(snippet_path, "callgraph.json")
         with open(cg_path, "r") as f:
             return json.loads(f.read())
 
     def assertEqual(self, actual, expected):
-        super().assertEqual(actual, expected)
+        def do_sorted(d):
+            s = {}
+            for n in d:
+                s[n] = sorted(d[n])
+            return s
+
+        super().assertEqual(do_sorted(actual), do_sorted(expected))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pycg-0.0.6/micro-benchmark-key-errs/create_pytests.py` & `PyCG-0.0.7/micro-benchmark-key-errs/create_pytests.py`

 * *Files identical despite different names*

### Comparing `pycg-0.0.6/pycg/__main__.py` & `PyCG-0.0.7/pycg/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,104 +1,89 @@
-import os
-import sys
-import json
 import argparse
+import json
 
-from pycg.pycg import CallGraphGenerator
 from pycg import formats
+from pycg.pycg import CallGraphGenerator
 from pycg.utils.constants import CALL_GRAPH_OP, KEY_ERR_OP
 
+
 def main():
     parser = argparse.ArgumentParser()
-    parser.add_argument("entry_point",
-        nargs="*",
-        help="Entry points to be processed")
-    parser.add_argument(
-        "--package",
-        help="Package containing the code to be analyzed",
-        default=None
+    parser.add_argument("entry_point", nargs="*", help="Entry points to be processed")
+    parser.add_argument(
+        "--package", help="Package containing the code to be analyzed", default=None
     )
     parser.add_argument(
         "--fasten",
         help="Produce call graph using the FASTEN format",
         action="store_true",
-        default=False
-    )
-    parser.add_argument(
-        "--product",
-        help="Package name",
-        default=""
-    )
-    parser.add_argument(
-        "--forge",
-        help="Source the product was downloaded from",
-        default=""
+        default=False,
     )
+    parser.add_argument("--product", help="Package name", default="")
     parser.add_argument(
-        "--version",
-        help="Version of the product",
-        default=""
+        "--forge", help="Source the product was downloaded from", default=""
     )
+    parser.add_argument("--version", help="Version of the product", default="")
     parser.add_argument(
-        "--timestamp",
-        help="Timestamp of the package's version",
-        default=0
+        "--timestamp", help="Timestamp of the package's version", default=0
     )
     parser.add_argument(
         "--max-iter",
         type=int,
-        help=("Maximum number of iterations through source code. " +
-            "If not specified a fix-point iteration will be performed."),
-        default=-1
+        help=(
+            "Maximum number of iterations through source code. "
+            "If not specified a fix-point iteration will be performed."
+        ),
+        default=-1,
     )
     parser.add_argument(
-        '--operation',
+        "--operation",
         type=str,
         choices=[CALL_GRAPH_OP, KEY_ERR_OP],
-        help=("Operation to perform. " +
-             "Choose " + CALL_GRAPH_OP + " for call graph generation (default)" +
-             " or " + KEY_ERR_OP + " for key error detection on dictionaries."),
-        default=CALL_GRAPH_OP
+        help=(
+            "Operation to perform. Choose "
+            + CALL_GRAPH_OP
+            + " for call graph generation (default) or "
+            + KEY_ERR_OP
+            + " for key error detection on dictionaries."
+        ),
+        default=CALL_GRAPH_OP,
     )
 
     parser.add_argument(
-        "--as-graph-output",
-        help="Output for the assignment graph",
-        default=None
-    )
-    parser.add_argument(
-        "-o",
-        "--output",
-        help="Output path",
-        default=None
+        "--as-graph-output", help="Output for the assignment graph", default=None
     )
+    parser.add_argument("-o", "--output", help="Output path", default=None)
 
     args = parser.parse_args()
 
-    cg = CallGraphGenerator(args.entry_point, args.package,
-                        args.max_iter, args.operation)
+    cg = CallGraphGenerator(
+        args.entry_point, args.package, args.max_iter, args.operation
+    )
     cg.analyze()
 
     if args.operation == CALL_GRAPH_OP:
         if args.fasten:
-            formatter = formats.Fasten(cg, args.package,
-                args.product, args.forge, args.version, args.timestamp)
+            formatter = formats.Fasten(
+                cg, args.package, args.product, args.forge, args.version, args.timestamp
+            )
         else:
             formatter = formats.Simple(cg)
         output = formatter.generate()
     else:
         output = cg.output_key_errs()
 
     as_formatter = formats.AsGraph(cg)
 
     if args.output:
         with open(args.output, "w+") as f:
             f.write(json.dumps(output))
     else:
-        print (json.dumps(output))
+        print(json.dumps(output))
 
     if args.as_graph_output:
         with open(args.as_graph_output, "w+") as f:
             f.write(json.dumps(as_formatter.generate()))
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `pycg-0.0.6/pycg/formats/__init__.py` & `PyCG-0.0.7/pycg/formats/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
-from .fasten import Fasten
-from .simple import Simple
-from .as_graph import AsGraph
+from .as_graph import AsGraph  # noqa: F401
+from .fasten import Fasten  # noqa: F401
+from .simple import Simple  # noqa: F401
```

### Comparing `pycg-0.0.6/pycg/formats/as_graph.py` & `PyCG-0.0.7/pycg/formats/as_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 from .base import BaseFormatter
 
+
 class AsGraph(BaseFormatter):
     def __init__(self, cg_generator):
         self.cg_generator = cg_generator
 
     def generate(self):
         graph = self.cg_generator.get_as_graph()
         output = {}
```

### Comparing `pycg-0.0.6/pycg/formats/base.py` & `PyCG-0.0.7/pycg/formats/base.py`

 * *Files identical despite different names*

### Comparing `pycg-0.0.6/pycg/formats/fasten.py` & `PyCG-0.0.7/pycg/formats/fasten.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 # specific language governing permissions and limitations
 # under the License.
 #
 import os
 
 from pkg_resources import Requirement
 
+from pycg import utils
+
 from .base import BaseFormatter
 
-from pycg import utils
 
 class Fasten(BaseFormatter):
     def __init__(self, cg_generator, package, product, forge, version, timestamp):
         self.cg_generator = cg_generator
         self.internal_mods = self.cg_generator.output_internal_mods() or {}
         self.external_mods = self.cg_generator.output_external_mods() or {}
         self.classes = self.cg_generator.output_classes() or {}
@@ -52,49 +53,52 @@
         if name:
             if name == modname:
                 cleared = ""
             else:
                 if not name.startswith(modname + "."):
                     raise Exception("name should start with modname", name, modname)
 
-                cleared = name[len(modname)+1:]
+                cleared = name[(len(modname) + 1) :]
 
         suffix = ""
         if name in self.functions:
             suffix = "()"
 
         return "/{}/{}{}".format(modname.replace("-", "_"), cleared, suffix)
 
     def to_external_uri(self, modname, name=""):
         if modname == utils.constants.BUILTIN_NAME:
-            name = name[len(modname)+1:]
+            name = name[len(modname) + 1 :]
             modname = ".builtin"
 
         return "//{}//{}".format(modname.replace("-", "_"), name)
 
     def find_dependencies(self, package_path):
         res = []
         if not package_path:
             return res
         requirements_path = os.path.join(package_path, "requirements.txt")
 
         if not os.path.exists(requirements_path):
             return res
 
-        reqs = []
         with open(requirements_path, "r") as f:
-            lines = [l.strip() for l in f.readlines()]
+            lines = [_l.strip() for _l in f.readlines()]
 
         for line in lines:
             if not line:
                 continue
 
-            req = Requirement.parse(line)
+            try:
+                req = Requirement.parse(line)
+            except ValueError:
+                # The specific line in the requirements.txt
+                # does not follow the Requirements File Format
+                continue
 
-            product = req.unsafe_name
             specs = req.specs
 
             constraints = []
 
             def add_range(begin, end):
                 if begin and end:
                     if begin[1] and end[1]:
@@ -145,58 +149,62 @@
 
                 if key == "<":
                     end = (val, False)
                 if key == "<=":
                     end = (val, True)
             add_range(begin, end)
 
-            res.append({"forge": "PyPI", "product": req.name, "constraints": constraints})
+            res.append(
+                {"forge": "PyPI", "product": req.name, "constraints": constraints}
+            )
 
         return res
 
     def get_internal_modules(self):
         mods = {}
 
         for modname, module in self.internal_mods.items():
             name = self.to_uri(modname)
             filename = module["filename"]
             namespaces = module["methods"]
 
-            mods[name] = {
-                "sourceFile": filename,
-                "namespaces": {}
-            }
+            mods[name] = {"sourceFile": filename, "namespaces": {}}
 
             for namespace, info in namespaces.items():
-                namespace_uri = self.to_uri(modname, info['name'])
+                namespace_uri = self.to_uri(modname, info["name"])
 
                 unique = self.get_unique_and_increment()
                 mods[name]["namespaces"][unique] = dict(
-                        namespace=namespace_uri,
-                        metadata=dict(first=info['first'], last=info['last']))
+                    namespace=namespace_uri,
+                    metadata=dict(first=info["first"], last=info["last"]),
+                )
                 self.namespace_map[namespace_uri] = unique
         mods = self.add_superclasses(mods)
 
         return mods
 
     def add_superclasses(self, mods):
         for cls_name, cls in self.classes.items():
             cls_uri = self.namespace_map.get(self.to_uri(cls["module"], cls_name))
-            mods[self.to_uri(cls["module"])]["namespaces"][cls_uri]["metadata"]["superClasses"] = []
+            mods[self.to_uri(cls["module"])]["namespaces"][cls_uri]["metadata"][
+                "superClasses"
+            ] = []
             for parent in cls["mro"]:
                 if parent == cls_name:
                     continue
 
                 if self.classes.get(parent):
                     parent_uri = self.to_uri(self.classes[parent]["module"], parent)
                 else:
                     parent_mod = parent.split(".")[0]
                     parent_uri = self.to_external_uri(parent_mod, parent)
 
-                mods[self.to_uri(cls["module"])]["namespaces"][cls_uri]["metadata"]["superClasses"].append(parent_uri)
+                mods[self.to_uri(cls["module"])]["namespaces"][cls_uri]["metadata"][
+                    "superClasses"
+                ].append(parent_uri)
 
         return mods
 
     def create_namespaces_map(self):
         namespaces_maps = [{}, {}]
         for res, hmap in zip(namespaces_maps, [self.internal_mods, self.external_mods]):
             for mod in hmap:
@@ -207,37 +215,30 @@
 
     def get_external_modules(self):
         mods = {}
         for modname, module in self.external_mods.items():
             name = self.to_external_uri(modname).split("/")[2]
             namespaces = module["methods"]
 
-            mods[name] = {
-                "sourceFile": "",
-                "namespaces": {}
-            }
+            mods[name] = {"sourceFile": "", "namespaces": {}}
 
             for namespace, info in namespaces.items():
                 # We avoid saving the external module as external method
-                if info['name'] != modname:
-                    namespace_uri = self.to_external_uri(modname, info['name'])
+                if info["name"] != modname:
+                    namespace_uri = self.to_external_uri(modname, info["name"])
 
                     unique = self.get_unique_and_increment()
                     mods[name]["namespaces"][str(unique)] = dict(
-                            namespace=namespace_uri,
-                            metadata={})
+                        namespace=namespace_uri, metadata={}
+                    )
                     self.namespace_map[namespace_uri] = unique
         return mods
 
     def get_graph(self):
-        graph = {
-            "internalCalls": [],
-            "externalCalls": [],
-            "resolvedCalls": []
-        }
+        graph = {"internalCalls": [], "externalCalls": [], "resolvedCalls": []}
 
         internal, external = self.create_namespaces_map()
 
         for src, dst in self.edges:
             uris = []
             for node in [src, dst]:
                 if node in internal:
@@ -246,35 +247,27 @@
                     uris.append(self.namespace_map.get(uri, uri))
                 elif node in external:
                     mod = external[node]
                     uris.append(self.namespace_map.get(self.to_external_uri(mod, node)))
 
             if len(uris) == 2:
                 if dst in external:
-                    graph["externalCalls"].append([
-                        str(uris[0]),
-                        str(uris[1]),
-                        {}
-                    ])
+                    graph["externalCalls"].append([str(uris[0]), str(uris[1]), {}])
                 else:
-                    graph["internalCalls"].append([
-                        str(uris[0]),
-                        str(uris[1]),
-                        {}
-                    ])
+                    graph["internalCalls"].append([str(uris[0]), str(uris[1]), {}])
         return graph
 
     def generate(self):
         return {
             "product": self.product,
             "forge": self.forge,
             "generator": "PyCG",
             "depset": self.find_dependencies(self.package),
             "version": self.version,
             "timestamp": self.timestamp,
             "modules": {
                 "internal": self.get_internal_modules(),
-                "external": self.get_external_modules()
+                "external": self.get_external_modules(),
             },
             "graph": self.get_graph(),
-            "nodes": self.get_unique_and_increment()
+            "nodes": self.get_unique_and_increment(),
         }
```

### Comparing `pycg-0.0.6/pycg/formats/simple.py` & `PyCG-0.0.7/pycg/formats/simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 from .base import BaseFormatter
 
+
 class Simple(BaseFormatter):
     def __init__(self, cg_generator):
         self.cg_generator = cg_generator
 
     def generate(self):
         output = self.cg_generator.output()
         output_cg = {}
```

### Comparing `pycg-0.0.6/pycg/machinery/callgraph.py` & `PyCG-0.0.7/pycg/machinery/callgraph.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def add_node(self, name, modname=""):
         if not isinstance(name, str):
             raise CallGraphError("Only string node names allowed")
         if not name:
             raise CallGraphError("Empty node name")
 
-        if not name in self.cg:
+        if name not in self.cg:
             self.cg[name] = set()
             self.modnames[name] = modname
 
         if name in self.cg and not self.modnames[name]:
             self.modnames[name] = modname
 
     def add_edge(self, src, dest):
```

### Comparing `pycg-0.0.6/pycg/machinery/classes.py` & `PyCG-0.0.7/pycg/machinery/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,23 @@
         self.names = {}
 
     def get(self, name):
         if name in self.names:
             return self.names[name]
 
     def create(self, name, module):
-        if not name in self.names:
+        if name not in self.names:
             cls = ClassNode(name, module)
             self.names[name] = cls
         return self.names[name]
 
     def get_classes(self):
         return self.names
 
+
 class ClassNode:
     def __init__(self, ns, module):
         self.ns = ns
         self.module = module
         self.mro = [ns]
 
     def add_parent(self, parent):
@@ -48,30 +49,30 @@
             for item in parent:
                 self.mro.append(item)
         self.fix_mro()
 
     def fix_mro(self):
         new_mro = []
         for idx, item in enumerate(self.mro):
-            if self.mro[idx+1:].count(item) > 0:
+            if self.mro[idx + 1 :].count(item) > 0:
                 continue
             new_mro.append(item)
         self.mro = new_mro
 
     def get_mro(self):
         return self.mro
 
     def get_module(self):
         return self.module
 
     def compute_mro(self):
         res = []
         self.mro.reverse()
         for parent in self.mro:
-            if not parent in res:
+            if parent not in res:
                 res.append(parent)
 
         res.reverse()
         self.mro = res
 
     def clear_mro(self):
         self.mro = [self.ns]
```

### Comparing `pycg-0.0.6/pycg/machinery/definitions.py` & `PyCG-0.0.7/pycg/machinery/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
-from pycg.machinery.pointers import NamePointer, LiteralPointer
 from pycg import utils
+from pycg.machinery.pointers import LiteralPointer, NamePointer
+
 
 class DefinitionManager(object):
     def __init__(self):
         self.defs = {}
 
     def create(self, ns, def_type):
         if not ns or not isinstance(ns, str):
             raise DefinitionError("Invalid namespace argument")
-        if not def_type in Definition.types:
+        if def_type not in Definition.types:
             raise DefinitionError("Invalid def type argument")
         if self.get(ns):
             raise DefinitionError("Definition already exists")
 
         self.defs[ns] = Definition(ns, def_type)
         return self.defs[ns]
 
@@ -41,15 +42,16 @@
         self.defs[ns].merge(defi)
 
         # if it is a function def, we need to create a return pointer
         if defi.is_function_def():
             return_ns = utils.join_ns(ns, utils.constants.RETURN_NAME)
             self.defs[return_ns] = Definition(return_ns, utils.constants.NAME_DEF)
             self.defs[return_ns].get_name_pointer().add(
-                utils.join_ns(defi.get_ns(), utils.constants.RETURN_NAME))
+                utils.join_ns(defi.get_ns(), utils.constants.RETURN_NAME)
+            )
 
         return self.defs[ns]
 
     def get(self, ns):
         if ns in self.defs:
             return self.defs[ns]
 
@@ -75,19 +77,20 @@
         if not defi:
             defi = self.create(full_ns, utils.constants.CLS_DEF)
 
         return defi
 
     def transitive_closure(self):
         closured = {}
+
         def dfs(defi):
             name_pointer = defi.get_name_pointer()
             new_set = set()
             # bottom
-            if not closured.get(defi.get_ns(), None) == None:
+            if closured.get(defi.get_ns(), None) is not None:
                 return closured[defi.get_ns()]
 
             if not name_pointer.get():
                 new_set.add(defi.get_ns())
 
             closured[defi.get_ns()] = new_set
 
@@ -99,15 +102,15 @@
                     items = set([name])
                 new_set = new_set.union(items)
 
             closured[defi.get_ns()] = new_set
             return closured[defi.get_ns()]
 
         for ns, current_def in self.defs.items():
-            if closured.get(current_def, None) == None:
+            if closured.get(current_def, None) is None:
                 dfs(current_def)
 
         return closured
 
     def complete_definitions(self):
         # THE MOST expensive part of this tool's process
         # TODO: IMPROVE COMPLEXITY
@@ -125,90 +128,90 @@
                     continue
 
                 # sometimes we may end up with a cycle
                 if pointsto_arg in arg:
                     arg.remove(pointsto_arg)
 
                 for item in arg:
-                    if not item in pointsto_arg_def.get():
-                        if self.defs.get(item, None) != None:
+                    if item not in pointsto_arg_def.get():
+                        if self.defs.get(item, None) is not None:
                             changed_something = True
                     # HACK: this check shouldn't be needed
                     # if we remove this the following breaks:
                     # x = lambda x: x + 1
                     # x(1)
-                    # since on line 184 we don't discriminate between literal values and name values
+                    # since on line 184 we don't discriminate between
+                    # literal values and name values
                     if not self.defs.get(item, None):
                         continue
                     pointsto_arg_def.add(item)
             return changed_something
 
         for i in range(len(self.defs)):
             changed_something = False
             for ns, current_def in self.defs.items():
                 # the name pointer of the definition we're currently iterating
                 current_name_pointer = current_def.get_name_pointer()
                 # iterate the names the current definition points to items
                 # for name in current_name_pointer.get():
                 for name in current_name_pointer.get().copy():
-
                     # get the name pointer of the points to name
                     if not self.defs.get(name, None):
                         continue
                     if name == ns:
                         continue
 
                     pointsto_name_pointer = self.defs[name].get_name_pointer()
-                    # iterate the arguments of the definition we're currently iterating
+                    # iterate the arguments of the definition
+                    # we're currently iterating
                     for arg_name, arg in current_name_pointer.get_args().items():
                         pos = current_name_pointer.get_pos_of_name(arg_name)
-                        if not pos is None:
+                        if pos is not None:
                             pointsto_args = pointsto_name_pointer.get_pos_arg(pos)
                             if not pointsto_args:
                                 pointsto_name_pointer.add_pos_arg(pos, None, arg)
                                 continue
                         else:
                             pointsto_args = pointsto_name_pointer.get_arg(arg_name)
                             if not pointsto_args:
                                 pointsto_name_pointer.add_arg(arg_name, arg)
                                 continue
-                        changed_something = changed_something or update_pointsto_args(pointsto_args, arg, current_def.get_ns())
+                        changed_something = changed_something or update_pointsto_args(
+                            pointsto_args, arg, current_def.get_ns()
+                        )
 
             if not changed_something:
                 break
 
 
 class Definition(object):
     types = [
         utils.constants.FUN_DEF,
         utils.constants.MOD_DEF,
         utils.constants.NAME_DEF,
         utils.constants.CLS_DEF,
-        utils.constants.EXT_DEF
+        utils.constants.EXT_DEF,
     ]
 
     def __init__(self, fullns, def_type):
         self.fullns = fullns
-        self.points_to = {
-            "lit": LiteralPointer(),
-            "name": NamePointer()
-        }
+        self.points_to = {"lit": LiteralPointer(), "name": NamePointer()}
         self.def_type = def_type
 
     def get_type(self):
         return self.def_type
 
     def is_function_def(self):
         return self.def_type == utils.constants.FUN_DEF
 
     def is_ext_def(self):
         return self.def_type == utils.constants.EXT_DEF
 
     def is_callable(self):
-        return (self.is_function_def() or self.is_ext_def())
+        return self.is_function_def() or self.is_ext_def()
 
     def get_lit_pointer(self):
         return self.points_to["lit"]
 
     def get_name_pointer(self):
         return self.points_to["name"]
 
@@ -218,9 +221,10 @@
     def get_ns(self):
         return self.fullns
 
     def merge(self, to_merge):
         for name, pointer in to_merge.points_to.items():
             self.points_to[name].merge(pointer)
 
+
 class DefinitionError(Exception):
     pass
```

### Comparing `pycg-0.0.6/pycg/machinery/imports.py` & `PyCG-0.0.7/pycg/machinery/imports.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,28 +14,30 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
-import sys
-import ast
-import os
-import importlib
 import copy
+import importlib
+import os
+import sys
+from importlib import abc
 
 from pycg import utils
 
+
 def get_custom_loader(ig_obj):
     """
     Closure which returns a custom loader
     that modifies an ImportManager object
     """
-    class CustomLoader(importlib.abc.SourceLoader):
+
+    class CustomLoader(abc.SourceLoader):
         def __init__(self, fullname, path):
             self.fullname = fullname
             self.path = path
 
             ig_obj.create_edge(self.fullname)
             if not ig_obj.get_node(self.fullname):
                 ig_obj.create_node(self.fullname)
@@ -45,14 +47,15 @@
             return self.path
 
         def get_data(self, filename):
             return ""
 
     return CustomLoader
 
+
 class ImportManager(object):
     def __init__(self):
         self.import_graph = dict()
         self.current_module = ""
         self.input_file = ""
         self.mod_dir = None
         self.old_path_hooks = None
@@ -84,15 +87,14 @@
 
         node = self.get_node(self._get_module_path())
         if not node:
             raise ImportManagerError("Can't add edge to a non existing node")
 
         node["imports"].add(dest)
 
-
     def _clear_caches(self):
         importlib.invalidate_caches()
         sys.path_importer_cache.clear()
         # TODO: maybe not do that since it empties the whole cache
         for name in self.import_graph:
             if name in sys.modules:
                 del sys.modules[name]
@@ -115,46 +117,51 @@
         node = self.get_node(node_name)
         if not node:
             raise ImportManagerError("Node does not exist")
 
         node["filename"] = os.path.abspath(filename)
 
     def get_imports(self, modname):
-        if not modname in self.import_graph:
+        if modname not in self.import_graph:
             return []
         return self.import_graph[modname]["imports"]
 
-
     def _is_init_file(self):
         return self.input_file.endswith("__init__.py")
 
     def _handle_import_level(self, name, level):
         # add a dot for each level
         package = self._get_module_path().split(".")
         if level > len(package):
             raise ImportError("Attempting import beyond top level package")
 
         mod_name = ("." * level) + name
-        # When an __init__ file is analyzed, then the module name doesn't contain
-        # the __init__ part in it, so special care must be taken for levels.
+        # When an __init__ file is analyzed,
+        # then the module name doesn't contain
+        # the __init__ part in it,
+        # so special care must be taken for levels.
         if self._is_init_file() and level >= 1:
             if level != 1:
                 level -= 1
                 package = package[:-level]
         else:
             package = package[:-level]
 
         return mod_name, ".".join(package)
 
     def _do_import(self, mod_name, package):
         if mod_name in sys.modules:
             self.create_edge(mod_name)
             return sys.modules[mod_name]
 
-        module_spec = importlib.util.find_spec(mod_name, package=package)
+        try:
+            module_spec = importlib.util.find_spec(mod_name, package=package)
+        except ModuleNotFoundError:
+            module_spec = None
+
         if module_spec is None:
             return importlib.import_module(mod_name, package=package)
 
         return importlib.util.module_from_spec(module_spec)
 
     def handle_import(self, name, level):
         # We currently don't support builtin modules because they're frozen.
@@ -169,56 +176,60 @@
         try:
             mod_name, package = self._handle_import_level(name, level)
         except ImportError:
             return
 
         parent = ".".join(mod_name.split(".")[:-1])
         parent_name = ".".join(name.split(".")[:-1])
-        combos = [(mod_name, package),
-                (parent, package),
-                (utils.join_ns(package, name), ""),
-                (utils.join_ns(package, parent_name), "")]
+        combos = [
+            (mod_name, package),
+            (parent, package),
+            (utils.join_ns(package, name), ""),
+            (utils.join_ns(package, parent_name), ""),
+        ]
 
         mod = None
         for mn, pkg in combos:
             try:
                 mod = self._do_import(mn, pkg)
                 break
-            except:
+            except Exception:
                 continue
 
         if not mod:
             return
 
         if not hasattr(mod, "__file__") or not mod.__file__:
             return
         if self.mod_dir not in mod.__file__:
             return
         fname = mod.__file__
         if fname.endswith("__init__.py"):
             fname = os.path.split(fname)[0]
 
-        return utils.to_mod_name(
-            os.path.relpath(fname, self.mod_dir))
+        return utils.to_mod_name(os.path.relpath(fname, self.mod_dir))
 
     def get_import_graph(self):
         return self.import_graph
 
     def install_hooks(self):
         loader = get_custom_loader(self)
         self.old_path_hooks = copy.deepcopy(sys.path_hooks)
         self.old_path = copy.deepcopy(sys.path)
 
         loader_details = loader, importlib.machinery.all_suffixes()
-        sys.path_hooks.insert(0, importlib.machinery.FileFinder.path_hook(loader_details))
+        sys.path_hooks.insert(
+            0, importlib.machinery.FileFinder.path_hook(loader_details)
+        )
         sys.path.insert(0, os.path.abspath(self.mod_dir))
 
         self._clear_caches()
 
     def remove_hooks(self):
         sys.path_hooks = self.old_path_hooks
         sys.path = self.old_path
 
         self._clear_caches()
 
+
 class ImportManagerError(Exception):
     pass
```

### Comparing `pycg-0.0.6/pycg/machinery/key_err.py` & `PyCG-0.0.7/pycg/machinery/key_err.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,16 +19,13 @@
 # under the License.
 #
 class KeyErrors(object):
     def __init__(self):
         self.key_errs = []
 
     def add(self, filename, lineno, namespace, key):
-        self.key_errs.append({
-            "filename": filename,
-            "lineno": lineno,
-            "namespace": namespace,
-            "key": key
-        })
+        self.key_errs.append(
+            {"filename": filename, "lineno": lineno, "namespace": namespace, "key": key}
+        )
 
     def get(self):
         return self.key_errs
```

### Comparing `pycg-0.0.6/pycg/machinery/modules.py` & `PyCG-0.0.7/pycg/machinery/modules.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
     def get_internal_modules(self):
         return self.internal
 
     def get_external_modules(self):
         return self.external
 
+
 class Module:
     def __init__(self, name, filename):
         self.name = name
         self.filename = filename
         self.methods = dict()
 
     def get_name(self):
@@ -56,11 +57,8 @@
         return self.filename
 
     def get_methods(self):
         return self.methods
 
     def add_method(self, method, first=None, last=None):
         if not self.methods.get(method, None):
-            self.methods[method] = dict(
-                    name=method,
-                    first=first,
-                    last=last)
+            self.methods[method] = dict(name=method, first=first, last=last)
```

### Comparing `pycg-0.0.6/pycg/machinery/pointers.py` & `PyCG-0.0.7/pycg/machinery/pointers.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,28 +30,30 @@
 
     def get(self):
         return self.values
 
     def merge(self, pointer):
         self.values = self.values.union(pointer.values)
 
+
 class LiteralPointer(Pointer):
     STR_LIT = "STRING"
     INT_LIT = "INTEGER"
     UNK_LIT = "UNKNOWN"
 
     # no need to add the actual item
     def add(self, item):
         if isinstance(item, str):
             self.values.add(item)
         elif isinstance(item, int):
             self.values.add(item)
         else:
             self.values.add(self.UNK_LIT)
 
+
 class NamePointer(Pointer):
     def __init__(self):
         super().__init__()
         self.pos_to_name = {}
         self.name_to_pos = {}
         self.args = {}
 
@@ -60,20 +62,20 @@
             int(pos)
         except ValueError:
             raise PointerError("Invalid position for argument")
 
         return pos
 
     def get_or_create(self, name):
-        if not name in self.args:
+        if name not in self.args:
             self.args[name] = set()
         return self.args[name]
 
     def add_arg(self, name, item):
-        arg = self.get_or_create(name)
+        self.get_or_create(name)
         if isinstance(item, str):
             self.args[name].add(item)
         elif isinstance(item, set):
             self.args[name] = self.args[name].union(item)
         else:
             raise Exception()
 
@@ -138,9 +140,10 @@
         super().merge(pointer)
         if hasattr(pointer, "get_pos_names"):
             for pos, name in pointer.get_pos_names().items():
                 self.pos_to_name[pos] = name
             for name, arg in pointer.get_args().items():
                 self.add_arg(name, arg)
 
+
 class PointerError(Exception):
     pass
```

### Comparing `pycg-0.0.6/pycg/machinery/scopes.py` & `PyCG-0.0.7/pycg/machinery/scopes.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,28 +15,31 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 import symtable
+
 from pycg import utils
 
+
 class ScopeManager(object):
     """Manages the scope entries"""
 
     def __init__(self):
         self.scopes = {}
 
     def handle_module(self, modulename, filename, contents):
         functions = []
         classes = []
+
         def process(namespace, parent, table):
-            if table.get_name() == 'top' and table.get_lineno() == 0:
-                name = ''
+            if table.get_name() == "top" and table.get_lineno() == 0:
+                name = ""
             else:
                 name = table.get_name()
 
             if name:
                 fullns = utils.join_ns(namespace, name)
             else:
                 fullns = namespace
@@ -48,15 +51,17 @@
                 classes.append(fullns)
 
             sc = self.create_scope(fullns, parent)
 
             for t in table.get_children():
                 process(fullns, sc, t)
 
-        process(modulename, None, symtable.symtable(contents, filename, compile_type="exec"))
+        process(
+            modulename, None, symtable.symtable(contents, filename, compile_type="exec")
+        )
         return {"functions": functions, "classes": classes}
 
     def handle_assign(self, ns, target, defi):
         scope = self.get_scope(ns)
         if scope:
             scope.add_def(target, defi)
 
@@ -69,22 +74,23 @@
             current_scope = current_scope.parent
 
     def get_scope(self, namespace):
         if namespace in self.get_scopes():
             return self.get_scopes()[namespace]
 
     def create_scope(self, namespace, parent):
-        if not namespace in self.scopes:
+        if namespace not in self.scopes:
             sc = ScopeItem(namespace, parent)
             self.scopes[namespace] = sc
         return self.scopes[namespace]
 
     def get_scopes(self):
         return self.scopes
 
+
 class ScopeItem(object):
     def __init__(self, fullns, parent):
         if parent and not isinstance(parent, ScopeItem):
             raise ScopeError("Parent must be a ScopeItem instance")
 
         if not isinstance(fullns, str):
             raise ScopeError("Namespace should be a string")
@@ -133,15 +139,16 @@
         self.dict_counter = 0
         self.list_counter = 0
 
     def add_def(self, name, defi):
         self.defs[name] = defi
 
     def merge_def(self, name, to_merge):
-        if not name in self.defs:
+        if name not in self.defs:
             self.defs[name] = to_merge
             return
 
         self.defs[name].merge_points_to(to_merge.get_points_to())
 
+
 class ScopeError(Exception):
     pass
```

### Comparing `pycg-0.0.6/pycg/processing/base.py` & `PyCG-0.0.7/pycg/processing/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,24 +20,25 @@
 #
 import ast
 import os
 
 from pycg import utils
 from pycg.machinery.definitions import Definition
 
+
 class ProcessingBase(ast.NodeVisitor):
     def __init__(self, filename, modname, modules_analyzed):
         self.modname = modname
 
         self.modules_analyzed = modules_analyzed
         self.modules_analyzed.add(self.modname)
 
         self.filename = os.path.abspath(filename)
 
-        with open(filename, "rt") as f:
+        with open(filename, "rt", errors="replace") as f:
             self.contents = f.read()
 
         self.name_stack = []
         self.method_stack = []
         self.last_called_names = None
 
     def get_modules_analyzed(self):
@@ -71,16 +72,17 @@
                 self.visit(stmt)
         self.method_stack.pop()
         self.name_stack.pop()
 
     def visit_Lambda(self, node, lambda_name=None):
         lambda_ns = utils.join_ns(self.current_ns, lambda_name)
         if not self.scope_manager.get_scope(lambda_ns):
-            self.scope_manager.create_scope(lambda_ns,
-                    self.scope_manager.get_scope(self.current_ns))
+            self.scope_manager.create_scope(
+                lambda_ns, self.scope_manager.get_scope(self.current_ns)
+            )
         self.name_stack.append(lambda_name)
         self.method_stack.append(lambda_name)
         self.visit(node.body)
         self.method_stack.pop()
         self.name_stack.pop()
 
     def visit_For(self, node):
@@ -119,15 +121,16 @@
     def visit_BinOp(self, node):
         self.visit(node.left)
         self.visit(node.right)
 
     def visit_ClassDef(self, node):
         self.name_stack.append(node.name)
         self.method_stack.append(node.name)
-        self.scope_manager.get_scope(self.current_ns).reset_counters()
+        if self.scope_manager.get_scope(self.current_ns):
+            self.scope_manager.get_scope(self.current_ns).reset_counters()
         for stmt in node.body:
             self.visit(stmt)
         self.method_stack.pop()
         self.name_stack.pop()
 
     def visit_Tuple(self, node):
         for elt in node.elts:
@@ -187,15 +190,17 @@
             else:
                 targetns = self._get_target_ns(target)
                 for tns in targetns:
                     if not tns:
                         continue
                     defi = self._handle_assign(tns, decoded)
                     splitted = tns.split(".")
-                    self.scope_manager.handle_assign(".".join(splitted[:-1]), splitted[-1], defi)
+                    self.scope_manager.handle_assign(
+                        ".".join(splitted[:-1]), splitted[-1], defi
+                    )
 
         for target in targets:
             do_assign(decoded, target)
 
     def decode_node(self, node):
         if isinstance(node, ast.Name):
             return [self.scope_manager.get_def(self.current_ns, node.id)]
@@ -204,24 +209,31 @@
             return_defs = []
             for called_def in decoded:
                 if not isinstance(called_def, Definition):
                     continue
 
                 return_ns = utils.constants.INVALID_NAME
                 if called_def.get_type() == utils.constants.FUN_DEF:
-                    return_ns = utils.join_ns(called_def.get_ns(), utils.constants.RETURN_NAME)
-                elif called_def.get_type() == utils.constants.CLS_DEF:
+                    return_ns = utils.join_ns(
+                        called_def.get_ns(), utils.constants.RETURN_NAME
+                    )
+                elif (
+                    called_def.get_type() == utils.constants.CLS_DEF
+                    or called_def.get_type() == utils.constants.EXT_DEF
+                ):
                     return_ns = called_def.get_ns()
                 defi = self.def_manager.get(return_ns)
                 if defi:
                     return_defs.append(defi)
 
             return return_defs
         elif isinstance(node, ast.Lambda):
-            lambda_counter = self.scope_manager.get_scope(self.current_ns).get_lambda_counter()
+            lambda_counter = self.scope_manager.get_scope(
+                self.current_ns
+            ).get_lambda_counter()
             lambda_name = utils.get_lambda_name(lambda_counter)
             return [self.scope_manager.get_def(self.current_ns, lambda_name)]
         elif isinstance(node, ast.Tuple):
             decoded = []
             for elt in node.elts:
                 decoded.append(self.decode_node(elt))
             return decoded
@@ -245,23 +257,27 @@
         elif isinstance(node, ast.Num):
             return [node.n]
         elif isinstance(node, ast.Str):
             return [node.s]
         elif self._is_literal(node):
             return [node]
         elif isinstance(node, ast.Dict):
-            dict_counter = self.scope_manager.get_scope(self.current_ns).get_dict_counter()
+            dict_counter = self.scope_manager.get_scope(
+                self.current_ns
+            ).get_dict_counter()
             dict_name = utils.get_dict_name(dict_counter)
             scope_def = self.scope_manager.get_def(self.current_ns, dict_name)
-            return [self.scope_manager.get_def(self.current_ns, dict_name)]
+            return [scope_def]
         elif isinstance(node, ast.List):
-            list_counter = self.scope_manager.get_scope(self.current_ns).get_list_counter()
+            list_counter = self.scope_manager.get_scope(
+                self.current_ns
+            ).get_list_counter()
             list_name = utils.get_list_name(list_counter)
             scope_def = self.scope_manager.get_def(self.current_ns, list_name)
-            return [self.scope_manager.get_def(self.current_ns, list_name)]
+            return [scope_def]
         elif isinstance(node, ast.Subscript):
             names = self.retrieve_subscript_names(node)
             defis = []
             for name in names:
                 defi = self.def_manager.get(name)
                 if defi:
                     defis.append(defi)
@@ -293,28 +309,29 @@
                 if not cls:
                     continue
 
                 for item in cls.get_mro():
                     names.add(item)
         return names
 
-
     def _retrieve_parent_names(self, node):
         if not isinstance(node, ast.Attribute):
             raise Exception("The node is not an attribute")
 
         decoded = self.decode_node(node.value)
         if not decoded:
             return set()
 
         names = set()
         for parent in decoded:
             if not parent or not isinstance(parent, Definition):
                 continue
-            if getattr(self, "closured", None) and self.closured.get(parent.get_ns(), None):
+            if getattr(self, "closured", None) and self.closured.get(
+                parent.get_ns(), None
+            ):
                 names = names.union(self.closured.get(parent.get_ns()))
             else:
                 names.add(parent.get_ns())
         return names
 
     def _retrieve_attribute_names(self, node):
         if not getattr(self, "closured", None):
@@ -327,15 +344,18 @@
                 defi = self.def_manager.get(name)
                 if not defi:
                     continue
                 if defi.get_type() == utils.constants.CLS_DEF:
                     cls_names = self.find_cls_fun_ns(defi.get_ns(), node.attr)
                     if cls_names:
                         names = names.union(cls_names)
-                if defi.get_type() in [utils.constants.FUN_DEF, utils.constants.MOD_DEF]:
+                if defi.get_type() in [
+                    utils.constants.FUN_DEF,
+                    utils.constants.MOD_DEF,
+                ]:
                     names.add(utils.join_ns(name, node.attr))
                 if defi.get_type() == utils.constants.EXT_DEF:
                     # HACK: extenral attributes can lead to infinite loops
                     # Identify them here
                     if node.attr in name:
                         continue
                     ext_name = utils.join_ns(name, node.attr)
@@ -472,15 +492,19 @@
 
     def analyze_submodule(self, cls, imp, *args, **kwargs):
         if imp in self.get_modules_analyzed():
             return
 
         fname = self.import_manager.get_filepath(imp)
 
-        if not fname or not fname.endswith(".py") or not self.import_manager.get_mod_dir() in fname:
+        if (
+            not fname
+            or not fname.endswith(".py")
+            or self.import_manager.get_mod_dir() not in fname
+        ):
             return
 
         self.import_manager.set_current_mod(imp, fname)
 
         visitor = cls(fname, imp, *args, **kwargs)
         visitor.analyze()
         self.merge_modules_analyzed(visitor.get_modules_analyzed())
```

### Comparing `pycg-0.0.6/pycg/processing/cgprocessor.py` & `PyCG-0.0.7/pycg/processing/cgprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,35 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
-import os
 import ast
+import os
 
 from pycg import utils
-from pycg.processing.base import ProcessingBase
-from pycg.machinery.callgraph import CallGraph
 from pycg.machinery.definitions import Definition
+from pycg.processing.base import ProcessingBase
+
 
 class CallGraphProcessor(ProcessingBase):
-    def __init__(self, filename, modname, import_manager,
-            scope_manager, def_manager, class_manager,
-            module_manager, call_graph=None, modules_analyzed=None):
+    def __init__(
+        self,
+        filename,
+        modname,
+        import_manager,
+        scope_manager,
+        def_manager,
+        class_manager,
+        module_manager,
+        call_graph=None,
+        modules_analyzed=None,
+    ):
         super().__init__(filename, modname, modules_analyzed)
         # parent directory of file
         self.parent_dir = os.path.dirname(filename)
 
         self.import_manager = import_manager
         self.scope_manager = scope_manager
         self.def_manager = def_manager
@@ -105,15 +114,17 @@
             for d in decoded:
                 if not isinstance(d, Definition):
                     continue
                 names = self.closured.get(d.get_ns(), [])
                 for name in names:
                     self.call_graph.add_edge(self.current_method, name)
 
-        self.call_graph.add_node(utils.join_ns(self.current_ns, node.name), self.modname)
+        self.call_graph.add_node(
+            utils.join_ns(self.current_ns, node.name), self.modname
+        )
         super().visit_FunctionDef(node)
 
     def visit_Call(self, node):
         def create_ext_edge(name, ext_modname):
             self.add_ext_mod_node(name)
             self.call_graph.add_node(name, ext_modname)
             self.call_graph.add_edge(self.current_method, name)
@@ -128,15 +139,16 @@
             self.visit(keyword.value)
 
         self.visit(node.func)
 
         names = self.retrieve_call_names(node)
         if not names:
             if isinstance(node.func, ast.Attribute) and self.has_ext_parent(node.func):
-                # TODO: This doesn't work for cases where there is an assignment of an attribute
+                # TODO: This doesn't work for cases
+                # where there is an assignment of an attribute
                 # i.e. import os; lala = os.path; lala.dirname()
                 for name in self.get_full_attr_names(node.func):
                     ext_modname = name.split(".")[0]
                     create_ext_edge(name, ext_modname)
             elif getattr(node.func, "id", None) and self.is_builtin(node.func.id):
                 name = utils.join_ns(utils.constants.BUILTIN_NAME, node.func.id)
                 create_ext_edge(name, utils.constants.BUILTIN_NAME)
@@ -150,44 +162,54 @@
             if pointer_def.is_callable():
                 if pointer_def.get_type() == utils.constants.EXT_DEF:
                     ext_modname = pointer.split(".")[0]
                     create_ext_edge(pointer, ext_modname)
                     continue
                 self.call_graph.add_edge(self.current_method, pointer)
 
-                # TODO: This doesn't work and leads to calls from the decorators
-                #    themselves to the function, creating edges to the first decorator
-                #for decorator in pointer_def.decorator_names:
-                #    dec_names = self.closured.get(decorator, [])
-                #    for dec_name in dec_names:
-                #        if self.def_manager.get(dec_name).get_type() == utils.constants.FUN_DEF:
-                #            self.call_graph.add_edge(self.current_ns, dec_name)
+            # TODO: This doesn't work
+            # and leads to calls from the decorators
+            # themselves to the function,
+            # creating edges to the first decorator
+            # for decorator in pointer_def.decorator_names:
+            #   dec_names = self.closured.get(decorator, [])
+            #   for dec_name in dec_names:
+            #       if self.def_manager.get(dec_name).
+            #               get_type() == utils.constants.FUN_DEF:
+            #           self.call_graph.add_edge(self.current_ns, dec_name)
 
             if pointer_def.get_type() == utils.constants.CLS_DEF:
                 init_ns = self.find_cls_fun_ns(pointer, utils.constants.CLS_INIT)
 
                 for ns in init_ns:
                     self.call_graph.add_edge(self.current_method, ns)
 
     def analyze_submodules(self):
-        super().analyze_submodules(CallGraphProcessor, self.import_manager,
-                self.scope_manager, self.def_manager, self.class_manager, self.module_manager,
-                call_graph=self.call_graph, modules_analyzed=self.get_modules_analyzed())
+        super().analyze_submodules(
+            CallGraphProcessor,
+            self.import_manager,
+            self.scope_manager,
+            self.def_manager,
+            self.class_manager,
+            self.module_manager,
+            call_graph=self.call_graph,
+            modules_analyzed=self.get_modules_analyzed(),
+        )
 
     def analyze(self):
         self.visit(ast.parse(self.contents, self.filename))
         self.analyze_submodules()
 
     def get_all_reachable_functions(self):
         reachable = set()
         names = set()
         current_scope = self.scope_manager.get_scope(self.current_ns)
         while current_scope:
             for name, defi in current_scope.get_defs().items():
-                if defi.is_function_def() and not name in names:
+                if defi.is_function_def() and name not in names:
                     closured = self.closured.get(defi.get_ns())
                     for item in closured:
                         reachable.add(item)
                     names.add(name)
             current_scope = current_scope.parent
 
         return reachable
@@ -212,15 +234,15 @@
             if not name:
                 name = node.attr
             else:
                 name = node.attr + "." + name
             node = node.value
 
         names = []
-        if getattr(node, "id", None) == None:
+        if getattr(node, "id", None) is None:
             return names
 
         defi = self.scope_manager.get_def(self.current_ns, node.id)
         if defi and self.closured.get(defi.get_ns()):
             for id in self.closured.get(defi.get_ns()):
                 names.append(id + "." + name)
```

### Comparing `pycg-0.0.6/pycg/processing/keyerrprocessor.py` & `PyCG-0.0.7/pycg/processing/keyerrprocessor.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,24 +14,34 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
-import os
 import ast
+import os
 import re
 
 from pycg import utils
 from pycg.processing.base import ProcessingBase
 
+
 class KeyErrProcessor(ProcessingBase):
-    def __init__(self, filename, modname, import_manager,
-            scope_manager, def_manager, class_manager, key_errs, modules_analyzed=None):
+    def __init__(
+        self,
+        filename,
+        modname,
+        import_manager,
+        scope_manager,
+        def_manager,
+        class_manager,
+        key_errs,
+        modules_analyzed=None,
+    ):
         super().__init__(filename, modname, modules_analyzed)
         # parent directory of file
         self.parent_dir = os.path.dirname(filename)
 
         self.import_manager = import_manager
         self.scope_manager = scope_manager
         self.def_manager = def_manager
@@ -50,33 +60,42 @@
                 continue
 
             defi = self.def_manager.get(name)
             if not defi:
                 splitted = name.split(".")
 
                 self.key_errs.add(
-                    filename=os.path.relpath(self.filename, self.import_manager.get_mod_dir()),
+                    filename=os.path.relpath(
+                        self.filename, self.import_manager.get_mod_dir()
+                    ),
                     lineno=node.lineno,
                     namespace=".".join(splitted[:-1]),
-                    key=splitted[-1])
+                    key=splitted[-1],
+                )
 
     def is_subscriptable(self, name):
         if re.match(r".*<dict[0-9]+>.*", name):
             return True
 
         return False
 
     def analyze_submodules(self):
-        super().analyze_submodules(KeyErrProcessor, self.import_manager,
-                self.scope_manager, self.def_manager, self.class_manager,
-                self.key_errs, modules_analyzed=self.get_modules_analyzed())
+        super().analyze_submodules(
+            KeyErrProcessor,
+            self.import_manager,
+            self.scope_manager,
+            self.def_manager,
+            self.class_manager,
+            self.key_errs,
+            modules_analyzed=self.get_modules_analyzed(),
+        )
 
     def analyze(self):
         self.visit(ast.parse(self.contents, self.filename))
         self.analyze_submodules()
 
     def visit_Lambda(self, node):
         counter = self.scope_manager.get_scope(self.current_ns).inc_lambda_counter()
         lambda_name = utils.get_lambda_name(counter)
-        lambda_fullns = utils.join_ns(self.current_ns, lambda_name)
+        utils.join_ns(self.current_ns, lambda_name)
 
         super().visit_Lambda(node, lambda_name)
```

### Comparing `pycg-0.0.6/pycg/processing/postprocessor.py` & `PyCG-0.0.7/pycg/processing/postprocessor.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,21 +16,31 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 import ast
 
-from pycg.processing.base import ProcessingBase
-from pycg.machinery.definitions import Definition
 from pycg import utils
+from pycg.machinery.definitions import Definition
+from pycg.processing.base import ProcessingBase
+
 
 class PostProcessor(ProcessingBase):
-    def __init__(self, input_file, modname, import_manager,
-            scope_manager, def_manager, class_manager, module_manager, modules_analyzed=None):
+    def __init__(
+        self,
+        input_file,
+        modname,
+        import_manager,
+        scope_manager,
+        def_manager,
+        class_manager,
+        module_manager,
+        modules_analyzed=None,
+    ):
         super().__init__(input_file, modname, modules_analyzed)
         self.import_manager = import_manager
         self.scope_manager = scope_manager
         self.def_manager = def_manager
         self.class_manager = class_manager
         self.module_manager = module_manager
         self.closured = self.def_manager.transitive_closure()
@@ -51,50 +61,61 @@
 
         for name in names:
             defi = self.def_manager.get(name)
             if not defi:
                 continue
             if defi.get_type() == utils.constants.CLS_DEF:
                 self.update_parent_classes(defi)
-                defi = self.def_manager.get(utils.join_ns(defi.get_ns(), utils.constants.CLS_INIT))
+                defi = self.def_manager.get(
+                    utils.join_ns(defi.get_ns(), utils.constants.CLS_INIT)
+                )
                 if not defi:
                     continue
             self.iterate_call_args(defi, node)
 
     def visit_Assign(self, node):
         self._visit_assign(node.value, node.targets)
 
-    def visit_Return(self, node):
-        self._visit_return(node)
+    # Redefined in line 118, 121
+    # def visit_Return(self, node):
+    #     self._visit_return(node)
 
-    def visit_Yield(self, node):
-        self._visit_return(node)
+    # def visit_Yield(self, node):
+    #     self._visit_return(node)
 
     def visit_For(self, node):
         # only handle name targets
         if isinstance(node.target, ast.Name):
-            target_def = self.def_manager.get(utils.join_ns(self.current_ns, node.target.id))
+            target_def = self.def_manager.get(
+                utils.join_ns(self.current_ns, node.target.id)
+            )
             # if the target definition exists
             if target_def:
                 iter_decoded = self.decode_node(node.iter)
                 # assign the target to the return value
                 # of the next function
                 for item in iter_decoded:
                     if not isinstance(item, Definition):
                         continue
                     # return value for generators
                     for name in self.closured.get(item.get_ns(), []):
                         # If there exists a next method on the iterable
                         # and if yes, add a pointer to it
-                        next_defi = self.def_manager.get(utils.join_ns(name,
-                            utils.constants.NEXT_METHOD, utils.constants.RETURN_NAME))
+                        next_defi = self.def_manager.get(
+                            utils.join_ns(
+                                name,
+                                utils.constants.NEXT_METHOD,
+                                utils.constants.RETURN_NAME,
+                            )
+                        )
                         if next_defi:
                             for name in self.closured.get(next_defi.get_ns(), []):
                                 target_def.get_name_pointer().add(name)
-                        else: # otherwise, add a pointer to the name (e.g. a yield)
+                        else:  # otherwise, add a pointer to the name
+                            # (e.g. a yield)
                             target_def.get_name_pointer().add(name)
 
         super().visit_For(node)
 
     def visit_Return(self, node):
         self._visit_return(node)
 
@@ -114,31 +135,36 @@
             # the return value of the first decorator
             # since, now the function is a namespace to that point
             if hasattr(fn_def, "decorator_names") and reversed_decorators:
                 last_decoded = self.decode_node(reversed_decorators[-1])
                 for d in last_decoded:
                     if not isinstance(d, Definition):
                         continue
-                    fn_def.decorator_names.add(utils.join_ns(d.get_ns(), utils.constants.RETURN_NAME))
+                    fn_def.decorator_names.add(
+                        utils.join_ns(d.get_ns(), utils.constants.RETURN_NAME)
+                    )
 
             previous_names = self.closured.get(fn_def.get_ns(), set())
             for decorator in reversed_decorators:
-                # assign the previous_def as the first parameter of the decorator
+                # assign the previous_def
+                # as the first parameter of the decorator
                 decoded = self.decode_node(decorator)
                 new_previous_names = set()
                 for d in decoded:
                     if not isinstance(d, Definition):
                         continue
                     for name in self.closured.get(d.get_ns(), []):
                         return_ns = utils.join_ns(name, utils.constants.RETURN_NAME)
 
-                        if self.closured.get(return_ns, None) == None:
+                        if self.closured.get(return_ns, None) is None:
                             continue
 
-                        new_previous_names = new_previous_names.union(self.closured.get(return_ns))
+                        new_previous_names = new_previous_names.union(
+                            self.closured.get(return_ns)
+                        )
 
                         for prev_name in previous_names:
                             pos_arg_names = d.get_name_pointer().get_pos_arg(0)
                             if not pos_arg_names:
                                 continue
                             for name in pos_arg_names:
                                 arg_def = self.def_manager.get(name)
@@ -187,15 +213,15 @@
         # Works similarly with dicts
         current_scope = self.scope_manager.get_scope(self.current_ns)
         list_counter = current_scope.inc_list_counter()
         list_name = utils.get_list_name(list_counter)
         list_full_ns = utils.join_ns(self.current_ns, list_name)
 
         # create a scope for the list
-        list_scope = self.scope_manager.create_scope(list_full_ns, current_scope)
+        self.scope_manager.create_scope(list_full_ns, current_scope)
 
         # create a list definition
         list_def = self.def_manager.get(list_full_ns)
         if not list_def:
             list_def = self.def_manager.create(list_full_ns, utils.constants.NAME_DEF)
         current_scope.add_def(list_name, list_def)
 
@@ -258,15 +284,17 @@
                 for name in names:
                     # create a definition for the key
                     if isinstance(name, int):
                         name = utils.get_int_name(name)
                     key_full_ns = utils.join_ns(dict_def.get_ns(), str(name))
                     key_def = self.def_manager.get(key_full_ns)
                     if not key_def:
-                        key_def = self.def_manager.create(key_full_ns, utils.constants.NAME_DEF)
+                        key_def = self.def_manager.create(
+                            key_full_ns, utils.constants.NAME_DEF
+                        )
                     dict_scope.add_def(str(name), key_def)
                     for v in decoded_value:
                         if isinstance(v, Definition):
                             key_def.get_name_pointer().add(v.get_ns())
                         else:
                             key_def.get_lit_pointer().add(v)
         self.name_stack.pop()
@@ -279,15 +307,15 @@
         for parent in cls.get_mro():
             parent_def = self.def_manager.get(parent)
             if not parent_def:
                 continue
             parent_scope = self.scope_manager.get_scope(parent)
             if not parent_scope:
                 continue
-            parent_items = list(parent_scope.get_defs().keys())
+            list(parent_scope.get_defs().keys())
             for key, child_def in current_scope.get_defs().items():
                 if key == "__init__":
                     continue
                 # resolve name from the parent_def
                 names = self.find_cls_fun_ns(parent_def.get_ns(), key)
 
                 new_ns = utils.join_ns(parent_def.get_ns(), key)
@@ -295,14 +323,20 @@
                 if not new_def:
                     new_def = self.def_manager.create(new_ns, utils.constants.NAME_DEF)
 
                 new_def.get_name_pointer().add_set(names)
                 new_def.get_name_pointer().add(child_def.get_ns())
 
     def analyze_submodules(self):
-        super().analyze_submodules(PostProcessor, self.import_manager,
-                self.scope_manager, self.def_manager, self.class_manager,
-                self.module_manager, modules_analyzed=self.get_modules_analyzed())
+        super().analyze_submodules(
+            PostProcessor,
+            self.import_manager,
+            self.scope_manager,
+            self.def_manager,
+            self.class_manager,
+            self.module_manager,
+            modules_analyzed=self.get_modules_analyzed(),
+        )
 
     def analyze(self):
         self.visit(ast.parse(self.contents, self.filename))
         self.analyze_submodules()
```

### Comparing `pycg-0.0.6/pycg/processing/preprocessor.py` & `PyCG-0.0.7/pycg/processing/preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,37 +15,43 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 import ast
-import os
-import importlib
 
-from pycg.machinery.definitions import DefinitionManager, Definition
 from pycg import utils
+from pycg.machinery.definitions import Definition
 from pycg.processing.base import ProcessingBase
 
+
 class PreProcessor(ProcessingBase):
-    def __init__(self, filename, modname,
-            import_manager, scope_manager, def_manager, class_manager,
-            module_manager, modules_analyzed=None):
+    def __init__(
+        self,
+        filename,
+        modname,
+        import_manager,
+        scope_manager,
+        def_manager,
+        class_manager,
+        module_manager,
+        modules_analyzed=None,
+    ):
         super().__init__(filename, modname, modules_analyzed)
 
         self.modname = modname
         self.mod_dir = "/".join(self.filename.split("/")[:-1])
 
         self.import_manager = import_manager
         self.scope_manager = scope_manager
         self.def_manager = def_manager
         self.class_manager = class_manager
         self.module_manager = module_manager
 
-
     def _get_fun_defaults(self, node):
         defaults = {}
         start = len(node.args.args) - len(node.args.defaults)
         for cnt, d in enumerate(node.args.defaults, start=start):
             if not d:
                 continue
 
@@ -58,17 +64,24 @@
                 continue
             self.visit(d)
             defaults[node.args.kwonlyargs[cnt].arg] = self.decode_node(d)
 
         return defaults
 
     def analyze_submodule(self, modname):
-        super().analyze_submodule(PreProcessor, modname,
-            self.import_manager, self.scope_manager, self.def_manager, self.class_manager,
-            self.module_manager, modules_analyzed=self.get_modules_analyzed())
+        super().analyze_submodule(
+            PreProcessor,
+            modname,
+            self.import_manager,
+            self.scope_manager,
+            self.def_manager,
+            self.class_manager,
+            self.module_manager,
+            modules_analyzed=self.get_modules_analyzed(),
+        )
 
     def visit_Module(self, node):
         def iterate_mod_items(items, const):
             for item in items:
                 defi = self.def_manager.get(item)
                 if not defi:
                     defi = self.def_manager.create(item, const)
@@ -87,21 +100,24 @@
         if last == 0:
             first = 0
         mod.add_method(self.modname, first, last)
 
         root_sc = self.scope_manager.get_scope(self.modname)
         if not root_sc:
             # initialize module scopes
-            items = self.scope_manager.handle_module(self.modname,
-                self.filename, self.contents)
+            items = self.scope_manager.handle_module(
+                self.modname, self.filename, self.contents
+            )
 
             root_sc = self.scope_manager.get_scope(self.modname)
             root_defi = self.def_manager.get(self.modname)
             if not root_defi:
-                root_defi = self.def_manager.create(self.modname, utils.constants.MOD_DEF)
+                root_defi = self.def_manager.create(
+                    self.modname, utils.constants.MOD_DEF
+                )
             root_sc.add_def(self.modname.split(".")[-1], root_defi)
 
             # create function and class defs and add them to their scope
             # we do this here, because scope_manager doesn't have an
             # interface with def_manager, and we want function definitions
             # to have the correct points_to set
             iterate_mod_items(items["functions"], utils.constants.FUN_DEF)
@@ -109,34 +125,35 @@
 
         defi = self.def_manager.get(self.modname)
         if not defi:
             defi = self.def_manager.create(self.modname, utils.constants.MOD_DEF)
 
         super().visit_Module(node)
 
-    def visit_Import(self, node, prefix='', level=0):
+    def visit_Import(self, node, prefix="", level=0):
         """
         For imports of the form
             `from something import anything`
         prefix is set to "something".
         For imports of the form
             `from .relative import anything`
         level is set to a number indicating the number
         of parent directories (e.g. in this case level=1)
         """
+
         def handle_src_name(name):
             # Get the module name and prepend prefix if necessary
             src_name = name
             if prefix:
                 src_name = prefix + "." + src_name
             return src_name
 
         def handle_scopes(imp_name, tgt_name, modname):
             def create_def(scope, name, imported_def):
-                if not name in scope.get_defs():
+                if name not in scope.get_defs():
                     def_ns = utils.join_ns(scope.get_ns(), name)
                     defi = self.def_manager.get(def_ns)
                     if not defi:
                         defi = self.def_manager.assign(def_ns, imported_def)
                     defi.get_name_pointer().add(imported_def.get_ns())
                     current_scope.add_def(name, defi)
 
@@ -151,17 +168,28 @@
                 defi = imported_scope.get_def(imp_name)
                 if not defi:
                     # maybe its a full namespace
                     defi = self.def_manager.get(imp_name)
 
                 if defi:
                     create_def(current_scope, tgt_name, defi)
-                    current_scope.get_def(tgt_name).get_name_pointer().add(defi.get_ns())
+                    current_scope.get_def(tgt_name).get_name_pointer().add(
+                        defi.get_ns()
+                    )
 
         def add_external_def(name, target):
+            # In case we encounter an external import in the form of:
+            #  "import package.module.module...
+            # we want to treat it as: "import package"
+            # and save it as such in the definition manager,
+            # so that we will be able to later map it
+            #  with its corresponding calls
+            if (name == target) & (len(name.split(".")) > 1):
+                name = name.split(".")[0]
+                target = target.split(".")[0]
             # add an external def for the name
             defi = self.def_manager.get(name)
             if not defi:
                 defi = self.def_manager.create(name, utils.constants.EXT_DEF)
             scope = self.scope_manager.get_scope(self.current_ns)
             if target != "*":
                 # add a def for the target that points to the name
@@ -183,37 +211,42 @@
 
             fname = self.import_manager.get_filepath(imported_name)
             if not fname:
                 add_external_def(src_name, tgt_name)
                 continue
             # only analyze modules under the current directory
             if self.import_manager.get_mod_dir() in fname:
-                if not imported_name in self.modules_analyzed:
+                if imported_name not in self.modules_analyzed:
                     self.analyze_submodule(imported_name)
                 handle_scopes(import_item.name, tgt_name, imported_name)
             else:
                 add_external_def(src_name, tgt_name)
 
         # handle all modules that were not analyzed
         for modname in self.import_manager.get_imports(self.modname):
             fname = self.import_manager.get_filepath(modname)
 
             if not fname:
                 continue
             # only analyze modules under the current directory
-            if self.import_manager.get_mod_dir() in fname and \
-                not modname in self.modules_analyzed:
-                    self.analyze_submodule(modname)
-
+            if (
+                self.import_manager.get_mod_dir() in fname
+                and modname not in self.modules_analyzed
+            ):
+                self.analyze_submodule(modname)
 
     def visit_ImportFrom(self, node):
         self.visit_Import(node, prefix=node.module, level=node.level)
 
     def _get_last_line(self, node):
-        lines = sorted(list(ast.walk(node)), key=lambda x: x.lineno if hasattr(x, "lineno") else 0, reverse=True)
+        lines = sorted(
+            list(ast.walk(node)),
+            key=lambda x: x.lineno if hasattr(x, "lineno") else 0,
+            reverse=True,
+        )
         if not lines:
             return node.lineno
 
         last = getattr(lines[0], "lineno", node.lineno)
         if last < node.lineno:
             return node.lineno
 
@@ -230,54 +263,66 @@
         if not mod:
             mod = self.module_manager.create(self.modname, self.filename)
         mod.add_method(fn_def.get_ns(), node.lineno, self._get_last_line(node))
 
         defs_to_create = []
         name_pointer = fn_def.get_name_pointer()
 
-        # TODO: static methods can be created using the staticmethod() function too
+        # TODO: static methods can be created using
+        # the staticmethod() function too
         is_static_method = False
         if hasattr(node, "decorator_list"):
             for decorator in node.decorator_list:
-                if isinstance(decorator, ast.Name) and decorator.id == utils.constants.STATIC_METHOD:
+                if (
+                    isinstance(decorator, ast.Name)
+                    and decorator.id == utils.constants.STATIC_METHOD
+                ):
                     is_static_method = True
 
-        if current_def.get_type() == utils.constants.CLS_DEF and not is_static_method and node.args.args:
+        if (
+            current_def.get_type() == utils.constants.CLS_DEF
+            and not is_static_method
+            and node.args.args
+        ):
             arg_ns = utils.join_ns(fn_def.get_ns(), node.args.args[0].arg)
             arg_def = self.def_manager.get(arg_ns)
             if not arg_def:
                 arg_def = self.def_manager.create(arg_ns, utils.constants.NAME_DEF)
             arg_def.get_name_pointer().add(current_def.get_ns())
 
-            self.scope_manager.handle_assign(fn_def.get_ns(), arg_def.get_name(), arg_def)
+            self.scope_manager.handle_assign(
+                fn_def.get_ns(), arg_def.get_name(), arg_def
+            )
             node.args.args = node.args.args[1:]
 
         for pos, arg in enumerate(node.args.args):
             arg_ns = utils.join_ns(fn_def.get_ns(), arg.arg)
             name_pointer.add_pos_arg(pos, arg.arg, arg_ns)
             defs_to_create.append(arg_ns)
 
         for arg in node.args.kwonlyargs:
             arg_ns = utils.join_ns(fn_def.get_ns(), arg.arg)
             # TODO: add_name_arg function
             name_pointer.add_name_arg(arg.arg, arg_ns)
             defs_to_create.append(arg_ns)
 
         # TODO: Add support for kwargs and varargs
-        #if node.args.kwarg:
+        # if node.args.kwarg:
         #    pass
-        #if node.args.vararg:
+        # if node.args.vararg:
         #    pass
 
         for arg_ns in defs_to_create:
             arg_def = self.def_manager.get(arg_ns)
             if not arg_def:
                 arg_def = self.def_manager.create(arg_ns, utils.constants.NAME_DEF)
 
-            self.scope_manager.handle_assign(fn_def.get_ns(), arg_def.get_name(), arg_def)
+            self.scope_manager.handle_assign(
+                fn_def.get_ns(), arg_def.get_name(), arg_def
+            )
 
             # has a default
             arg_name = arg_ns.split(".")[-1]
             if defaults.get(arg_name, None):
                 for default in defaults[arg_name]:
                     if isinstance(default, Definition):
                         arg_def.get_name_pointer().add(default.get_ns())
@@ -289,25 +334,27 @@
                         arg_def.get_lit_pointer().add(default)
         return fn_def
 
     def visit_AsyncFunctionDef(self, node):
         self.visit_FunctionDef(node)
 
     def visit_FunctionDef(self, node):
-        fn_def = self._handle_function_def(node, node.name)
+        self._handle_function_def(node, node.name)
 
         super().visit_FunctionDef(node)
 
     def visit_For(self, node):
         # just create the definition for target
         if isinstance(node.target, ast.Name):
             target_ns = utils.join_ns(self.current_ns, node.target.id)
             if not self.def_manager.get(target_ns):
                 defi = self.def_manager.create(target_ns, utils.constants.NAME_DEF)
-                self.scope_manager.get_scope(self.current_ns).add_def(node.target.id, defi)
+                self.scope_manager.get_scope(self.current_ns).add_def(
+                    node.target.id, defi
+                )
         super().visit_For(node)
 
     def visit_Assign(self, node):
         self._visit_assign(node.value, node.targets)
 
     def visit_Return(self, node):
         self._visit_return(node)
@@ -319,22 +366,24 @@
         self.visit(node.func)
         # if it is not a name there's nothing we can do here
         # ModuleVisitor will be able to resolve those calls
         # since it'll have the name tracking information
         if not isinstance(node.func, ast.Name):
             return
 
-        fullns = utils.join_ns(self.current_ns, node.func.id)
+        utils.join_ns(self.current_ns, node.func.id)
 
         defi = self.scope_manager.get_def(self.current_ns, node.func.id)
         if not defi:
             return
 
         if defi.get_type() == utils.constants.CLS_DEF:
-            defi = self.def_manager.get(utils.join_ns(defi.get_ns(), utils.constants.CLS_INIT))
+            defi = self.def_manager.get(
+                utils.join_ns(defi.get_ns(), utils.constants.CLS_INIT)
+            )
             if not defi:
                 return
 
         self.iterate_call_args(defi, node)
 
     def visit_Lambda(self, node):
         # The name of a lambda is defined by the counter of the current scope
```

### Comparing `pycg-0.0.6/pycg/pycg.py` & `PyCG-0.0.7/pycg/pycg.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,29 +15,28 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 import os
-import ast
 
-from pycg.processing.preprocessor import PreProcessor
-from pycg.processing.postprocessor import PostProcessor
-from pycg.processing.cgprocessor import CallGraphProcessor
-from pycg.processing.keyerrprocessor import KeyErrProcessor
-
-from pycg.machinery.scopes import ScopeManager
+from pycg import utils
+from pycg.machinery.callgraph import CallGraph
+from pycg.machinery.classes import ClassManager
 from pycg.machinery.definitions import DefinitionManager
 from pycg.machinery.imports import ImportManager
-from pycg.machinery.classes import ClassManager
-from pycg.machinery.callgraph import CallGraph
 from pycg.machinery.key_err import KeyErrors
 from pycg.machinery.modules import ModuleManager
-from pycg import utils
+from pycg.machinery.scopes import ScopeManager
+from pycg.processing.cgprocessor import CallGraphProcessor
+from pycg.processing.keyerrprocessor import KeyErrProcessor
+from pycg.processing.postprocessor import PostProcessor
+from pycg.processing.preprocessor import PreProcessor
+
 
 class CallGraphGenerator(object):
     def __init__(self, entry_points, package, max_iter, operation):
         self.entry_points = entry_points
         self.package = package
         self.state = None
         self.max_iter = max_iter
@@ -55,20 +54,22 @@
 
     def extract_state(self):
         state = {}
         state["defs"] = {}
         for key, defi in self.def_manager.get_defs().items():
             state["defs"][key] = {
                 "names": defi.get_name_pointer().get().copy(),
-                "lit": defi.get_lit_pointer().get().copy()
+                "lit": defi.get_lit_pointer().get().copy(),
             }
 
         state["scopes"] = {}
         for key, scope in self.scope_manager.get_scopes().items():
-            state["scopes"][key] = set([x.get_ns() for (_, x) in scope.get_defs().items()])
+            state["scopes"][key] = set(
+                [x.get_ns() for (_, x) in scope.get_defs().items()]
+            )
 
         state["classes"] = {}
         for key, ch in self.class_manager.get_classes().items():
             state["classes"][key] = ch.get_mro().copy()
         return state
 
     def reset_counters(self):
@@ -79,31 +80,31 @@
         if not self.state:
             return False
 
         curr_state = self.extract_state()
 
         # check defs
         for key, defi in curr_state["defs"].items():
-            if not key in self.state["defs"]:
+            if key not in self.state["defs"]:
                 return False
             if defi["names"] != self.state["defs"][key]["names"]:
                 return False
             if defi["lit"] != self.state["defs"][key]["lit"]:
                 return False
 
         # check scopes
         for key, scope in curr_state["scopes"].items():
-            if not key in self.state["scopes"]:
+            if key not in self.state["scopes"]:
                 return False
             if scope != self.state["scopes"][key]:
                 return False
 
         # check classes
         for key, ch in curr_state["classes"].items():
-            if not key in self.state["classes"]:
+            if key not in self.state["classes"]:
                 return False
             if ch != self.state["classes"][key]:
                 return False
 
         return True
 
     def remove_import_hooks(self):
@@ -114,16 +115,15 @@
 
     def _get_mod_name(self, entry, pkg):
         # We do this because we want __init__ modules to
         # only contain the parent module
         # since pycg can't differentiate between functions
         # coming from __init__ files.
 
-        input_mod = utils.to_mod_name(
-            os.path.relpath(entry, pkg))
+        input_mod = utils.to_mod_name(os.path.relpath(entry, pkg))
         if input_mod.endswith("__init__"):
             input_mod = ".".join(input_mod.split(".")[:-1])
 
         return input_mod
 
     def do_pass(self, cls, install_hooks=False, *args, **kwargs):
         modules_analyzed = set()
@@ -134,76 +134,113 @@
 
             if not input_mod:
                 continue
 
             if not input_pkg:
                 input_pkg = os.path.dirname(input_file)
 
-            if not input_mod in modules_analyzed:
+            if input_mod not in modules_analyzed:
                 if install_hooks:
                     self.import_manager.set_pkg(input_pkg)
                     self.import_manager.install_hooks()
 
-                processor = cls(input_file, input_mod,
-                                modules_analyzed=modules_analyzed, *args, **kwargs)
+                processor = cls(
+                    input_file,
+                    input_mod,
+                    modules_analyzed=modules_analyzed,
+                    *args,
+                    **kwargs,
+                )
                 processor.analyze()
-                modules_analyzed = modules_analyzed.union(processor.get_modules_analyzed())
+                modules_analyzed = modules_analyzed.union(
+                    processor.get_modules_analyzed()
+                )
 
                 if install_hooks:
                     self.remove_import_hooks()
 
     def analyze(self):
-        self.do_pass(PreProcessor, True,
-                self.import_manager, self.scope_manager, self.def_manager,
-                self.class_manager, self.module_manager)
+        self.do_pass(
+            PreProcessor,
+            True,
+            self.import_manager,
+            self.scope_manager,
+            self.def_manager,
+            self.class_manager,
+            self.module_manager,
+        )
         self.def_manager.complete_definitions()
 
         iter_cnt = 0
-        while (self.max_iter < 0 or iter_cnt < self.max_iter) and (not self.has_converged()):
+        while (self.max_iter < 0 or iter_cnt < self.max_iter) and (
+            not self.has_converged()
+        ):
             self.state = self.extract_state()
             self.reset_counters()
-            self.do_pass(PostProcessor, False,
-                    self.import_manager, self.scope_manager, self.def_manager,
-                    self.class_manager, self.module_manager)
+            self.do_pass(
+                PostProcessor,
+                False,
+                self.import_manager,
+                self.scope_manager,
+                self.def_manager,
+                self.class_manager,
+                self.module_manager,
+            )
 
             self.def_manager.complete_definitions()
             iter_cnt += 1
 
         self.reset_counters()
         if self.operation == utils.constants.CALL_GRAPH_OP:
-            self.do_pass(CallGraphProcessor, False,
-                    self.import_manager, self.scope_manager, self.def_manager,
-                    self.class_manager, self.module_manager, call_graph=self.cg)
+            self.do_pass(
+                CallGraphProcessor,
+                False,
+                self.import_manager,
+                self.scope_manager,
+                self.def_manager,
+                self.class_manager,
+                self.module_manager,
+                call_graph=self.cg,
+            )
         elif self.operation == utils.constants.KEY_ERR_OP:
-            self.do_pass(KeyErrProcessor, False,
-                    self.import_manager, self.scope_manager, self.def_manager,
-                    self.class_manager, self.key_errs)
+            self.do_pass(
+                KeyErrProcessor,
+                False,
+                self.import_manager,
+                self.scope_manager,
+                self.def_manager,
+                self.class_manager,
+                self.key_errs,
+            )
         else:
             raise Exception("Invalid operation: " + self.operation)
 
-
     def output(self):
         return self.cg.get()
 
     def output_key_errs(self):
         return self.key_errs.get()
 
-    def output_edges(self):
-        return self.key_errors
+    # Redefined in line 227
+    # def output_edges(self):
+    #     return self.key_errors
 
     def output_edges(self):
         return self.cg.get_edges()
 
     def _generate_mods(self, mods):
         res = {}
         for mod, node in mods.items():
             res[mod] = {
-                "filename": os.path.relpath(node.get_filename(), self.package)\
-                    if node.get_filename() else None,
-                "methods": node.get_methods()
+                "filename": (
+                    os.path.relpath(node.get_filename(), self.package)
+                    if node.get_filename()
+                    else None
+                ),
+                "methods": node.get_methods(),
             }
         return res
 
     def output_internal_mods(self):
         return self._generate_mods(self.module_manager.get_internal_modules())
 
     def output_external_mods(self):
@@ -215,15 +252,12 @@
             if defi.is_function_def():
                 functions.append(ns)
         return functions
 
     def output_classes(self):
         classes = {}
         for cls, node in self.class_manager.get_classes().items():
-            classes[cls] = {
-                "mro": node.get_mro(),
-                "module": node.get_module()
-            }
+            classes[cls] = {"mro": node.get_mro(), "module": node.get_module()}
         return classes
 
     def get_as_graph(self):
         return self.def_manager.get_defs().items()
```

### Comparing `pycg-0.0.6/pycg/utils/__init__.py` & `PyCG-0.0.7/pycg/utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
-from .common import *
-from . import constants
+from . import constants  # noqa: F401
+from .common import *  # noqa
```

### Comparing `pycg-0.0.6/pycg/utils/common.py` & `PyCG-0.0.7/pycg/utils/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,30 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 import os
 
+
 def get_lambda_name(counter):
     return "<lambda{}>".format(counter)
 
+
 def get_dict_name(counter):
     return "<dict{}>".format(counter)
 
+
 def get_list_name(counter):
     return "<list{}>".format(counter)
 
+
 def get_int_name(counter):
     return "<int{}>".format(counter)
 
+
 def join_ns(*args):
     return ".".join([arg for arg in args])
 
+
 def to_mod_name(name, package=None):
     return os.path.splitext(name)[0].replace("/", ".")
```

### Comparing `pycg-0.0.6/pycg/utils/constants.py` & `PyCG-0.0.7/pycg/utils/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,29 +14,29 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
-RETURN_NAME     = "<RETURN>"
-LAMBDA_NAME     = "<LAMBDA_{}>" # needs to be formatted
-BUILTIN_NAME    = "<builtin>"
-EXT_NAME        = "<external>"
+RETURN_NAME = "<RETURN>"
+LAMBDA_NAME = "<LAMBDA_{}>"  # needs to be formatted
+BUILTIN_NAME = "<builtin>"
+EXT_NAME = "<external>"
 
-FUN_DEF         = "FUNCTIONDEF"
-NAME_DEF        = "NAMEDEF"
-MOD_DEF         = "MODULEDEF"
-CLS_DEF         = "CLASSDEF"
-EXT_DEF         = "EXTERNALDEF"
+FUN_DEF = "FUNCTIONDEF"
+NAME_DEF = "NAMEDEF"
+MOD_DEF = "MODULEDEF"
+CLS_DEF = "CLASSDEF"
+EXT_DEF = "EXTERNALDEF"
 
-OBJECT_BASE     = "object"
+OBJECT_BASE = "object"
 
-CLS_INIT        = "__init__"
-ITER_METHOD     = "__iter__"
-NEXT_METHOD     = "__next__"
-STATIC_METHOD   = "staticmethod"
+CLS_INIT = "__init__"
+ITER_METHOD = "__iter__"
+NEXT_METHOD = "__next__"
+STATIC_METHOD = "staticmethod"
 
-INVALID_NAME    = "<**INVALID**>"
+INVALID_NAME = "<**INVALID**>"
 
-CALL_GRAPH_OP   = "call-graph"
-KEY_ERR_OP      = "key-error"
+CALL_GRAPH_OP = "call-graph"
+KEY_ERR_OP = "key-error"
```

### Comparing `pycg-0.0.6/pycg.egg-info/PKG-INFO` & `PyCG-0.0.7/PyCG.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
-Name: pycg
-Version: 0.0.6
-Summary: Practical Python Call Graphs
+Name: PyCG
+Version: 0.0.7
+Summary: PyCG - Practical Python Call Graphs
 Home-page: https://github.com/vitsalis/pycg
 Author: Vitalis Salis
 Author-email: vitsalis@gmail.com
 License: Apache Software License
+Project-URL: Homepage, https://github.com/vitsalis/PyCG
+Project-URL: Bug Tracker, https://github.com/vitsalis/PyCG/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # PyCG - Practical Python Call Graphs
 
+[![Linters](https://github.com/vitsalis/PyCG/actions/workflows/linters.yml/badge.svg)](https://github.com/vitsalis/PyCG/actions/workflows/linters.yml)
+[![Tests](https://github.com/vitsalis/PyCG/actions/workflows/test.yaml/badge.svg)](https://github.com/vitsalis/PyCG/actions/workflows/test.yaml)
+
 PyCG generates call graphs for Python code using static analysis.
 It efficiently supports
 * Higher order functions
 * Twisted class inheritance schemes
 * Automatic discovery of imported modules for further analysis
 * Nested definitions
 
 You can read the full methodology as well as a complete evaluation on the
-[ICSE 2021 paper](https://vitsalis.com/papers/pycg.pdf).
+[ICSE 2021 paper](https://arxiv.org/pdf/2103.00587.pdf).
 
 You can cite PyCG as follows.
 Vitalis Salis, Thodoris Sotiropoulos, Panos Louridas, Diomidis Spinellis and Dimitris Mitropoulos.
 PyCG: Practical Call Graph Generation in Python.
 In _43rd International Conference on Software Engineering, ICSE '21_,
 25–28 May 2021.
 
@@ -140,11 +145,15 @@
 ~ >>> pycg --package pypi_pkg --fasten --product "pypipkg" --forge "PyPI" \
         --version "0.1" --timestamp 42 \
         pypi_pkg/module1.py pkg_root/subpackage/module2.py -o cg.json
 ```
 
 # Running Tests
 
-From the root directory:
+From the root directory, first install the [mock](https://pypi.org/project/mock/) package:
+```
+pip3 install mock
+```
+Τhen, simply run the tests by executing:
 ```
 make test
 ```
```

### Comparing `pycg-0.0.6/pycg.egg-info/SOURCES.txt` & `PyCG-0.0.7/PyCG.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 LICENCE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
+PyCG.egg-info/PKG-INFO
+PyCG.egg-info/SOURCES.txt
+PyCG.egg-info/dependency_links.txt
+PyCG.egg-info/entry_points.txt
+PyCG.egg-info/top_level.txt
 micro-benchmark/__init__.py
 micro-benchmark/args_test.py
 micro-benchmark/assignments_test.py
 micro-benchmark/base.py
 micro-benchmark/builtins_test.py
 micro-benchmark/classes_test.py
 micro-benchmark/create_pytests.py
```

### Comparing `pycg-0.0.6/setup.py` & `PyCG-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,40 +19,43 @@
 # under the License.
 #
 import os
 
 from setuptools import setup, find_packages
 from subprocess import call
 
+
 def get_long_desc():
     with open("README.md", "r") as readme:
         desc = readme.read()
 
     return desc
 
+
 def setup_package():
     setup(
-        name='pycg',
-        version='0.0.6',
-        description='Practical Python Call Graphs',
+        name="pycg",
+        version="0.0.7",
+        description="Practical Python Call Graphs",
         long_description=get_long_desc(),
         long_description_content_type="text/markdown",
-        url='https://github.com/vitsalis/pycg',
-        license='Apache Software License',
+        url="https://github.com/vitsalis/pycg",
+        license="Apache Software License",
         packages=find_packages(),
         install_requires=[],
-        python_requires='>=3.4',
-        entry_points = {
-            'console_scripts': [
-                'pycg=pycg.__main__:main',
+        python_requires=">=3.4",
+        entry_points={
+            "console_scripts": [
+                "pycg=pycg.__main__:main",
             ],
         },
         classifiers=[
-            'License :: OSI Approved :: Apache Software License',
-            'Programming Language :: Python :: 3'
+            "License :: OSI Approved :: Apache Software License",
+            "Programming Language :: Python :: 3",
         ],
-        author = 'Vitalis Salis',
-        author_email = 'vitsalis@gmail.com'
+        author="Vitalis Salis",
+        author_email="vitsalis@gmail.com",
     )
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     setup_package()
```

