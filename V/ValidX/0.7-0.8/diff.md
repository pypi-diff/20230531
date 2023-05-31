# Comparing `tmp/ValidX-0.7.tar.gz` & `tmp/ValidX-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ValidX-0.7.tar", last modified: Wed Jan  6 15:27:06 2021, max compression
+gzip compressed data, was "ValidX-0.8.tar", last modified: Wed May 31 16:29:55 2023, max compression
```

## Comparing `ValidX-0.7.tar` & `ValidX-0.8.tar`

### file list

```diff
@@ -1,63 +1,75 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-06 15:27:06.717002 ValidX-0.7/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1322 2021-01-06 15:18:09.000000 ValidX-0.7/CHANGES.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       92 2021-01-06 15:18:09.000000 ValidX-0.7/CONTRIBUTORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1336 2021-01-06 15:18:09.000000 ValidX-0.7/LICENCE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2021-01-06 15:18:09.000000 ValidX-0.7/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3906 2021-01-06 15:27:06.717002 ValidX-0.7/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      857 2021-01-06 15:18:09.000000 ValidX-0.7/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-06 15:27:06.709006 ValidX-0.7/ValidX.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3906 2021-01-06 15:27:06.000000 ValidX-0.7/ValidX.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1336 2021-01-06 15:27:06.000000 ValidX-0.7/ValidX.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-01-06 15:27:06.000000 ValidX-0.7/ValidX.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-01-06 15:27:06.000000 ValidX-0.7/ValidX.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2021-01-06 15:27:06.000000 ValidX-0.7/ValidX.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-01-06 15:27:06.717002 ValidX-0.7/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1965 2021-01-06 15:18:09.000000 ValidX-0.7/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-06 15:27:06.705008 ValidX-0.7/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-06 15:27:06.709006 ValidX-0.7/src/validx/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1189 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13911 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/contracts.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-06 15:27:06.713004 ValidX-0.7/src/validx/cy/
--rw-rw-r--   0 travis    (2000) travis    (2000)      938 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/cy/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      663 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/cy/abstract.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)      503 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/cy/bools.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)      964 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/cy/chars.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)      181 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/cy/classes.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)     1747 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/cy/containers.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)     2155 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/cy/datetimes.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)      250 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/cy/instances.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)     1050 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/cy/numbers.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)      492 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/cy/pipelines.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)     1219 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/cy/special.pyi
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-06 15:27:06.713004 ValidX-0.7/src/validx/exc/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1084 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/exc/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10042 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/exc/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2349 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/exc/errors.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)     5289 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/exc/formatter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      520 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/exc/formatter.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)     2869 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/exc/markers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      451 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/exc/markers.pyi
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-06 15:27:06.717002 ValidX-0.7/src/validx/py/
--rw-rw-r--   0 travis    (2000) travis    (2000)      938 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8934 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/abstract.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      663 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/abstract.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)     2239 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/bools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      503 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/bools.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)     5048 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/chars.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      964 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/chars.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)     1010 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/classes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      181 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/classes.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)    12647 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/containers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1747 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/containers.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)    15945 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/datetimes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2155 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/datetimes.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)     1473 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/instances.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      250 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/instances.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)     6348 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/numbers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1050 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/numbers.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)     2389 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/pipelines.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      492 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/pipelines.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)     7355 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/special.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1219 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py/special.pyi
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/py.typed
--rw-rw-r--   0 travis    (2000) travis    (2000)      743 2021-01-06 15:18:09.000000 ValidX-0.7/src/validx/types.py
+drwxrwxr-x   0 krat      (1000) krat      (1000)        0 2023-05-31 16:29:55.026445 ValidX-0.8/
+-rw-rw-r--   0 krat      (1000) krat      (1000)     2681 2023-05-31 15:39:05.000000 ValidX-0.8/CHANGES.rst
+-rw-rw-r--   0 krat      (1000) krat      (1000)      156 2023-03-01 14:03:51.000000 ValidX-0.8/CONTRIBUTORS.rst
+-rw-rw-r--   0 krat      (1000) krat      (1000)     1336 2023-03-01 14:03:51.000000 ValidX-0.8/LICENCE.txt
+-rw-rw-r--   0 krat      (1000) krat      (1000)       20 2023-03-01 14:03:51.000000 ValidX-0.8/MANIFEST.in
+-rw-rw-r--   0 krat      (1000) krat      (1000)     4629 2023-05-31 16:29:55.026445 ValidX-0.8/PKG-INFO
+-rw-rw-r--   0 krat      (1000) krat      (1000)      899 2023-03-01 14:03:51.000000 ValidX-0.8/README.rst
+drwxrwxr-x   0 krat      (1000) krat      (1000)        0 2023-05-31 16:29:55.022445 ValidX-0.8/ValidX.egg-info/
+-rw-rw-r--   0 krat      (1000) krat      (1000)     4629 2023-05-31 16:29:55.000000 ValidX-0.8/ValidX.egg-info/PKG-INFO
+-rw-rw-r--   0 krat      (1000) krat      (1000)     1462 2023-05-31 16:29:55.000000 ValidX-0.8/ValidX.egg-info/SOURCES.txt
+-rw-rw-r--   0 krat      (1000) krat      (1000)        1 2023-05-31 16:29:55.000000 ValidX-0.8/ValidX.egg-info/dependency_links.txt
+-rw-rw-r--   0 krat      (1000) krat      (1000)        1 2023-05-31 16:29:55.000000 ValidX-0.8/ValidX.egg-info/not-zip-safe
+-rw-rw-r--   0 krat      (1000) krat      (1000)        7 2023-05-31 16:29:55.000000 ValidX-0.8/ValidX.egg-info/top_level.txt
+-rw-rw-r--   0 krat      (1000) krat      (1000)       38 2023-05-31 16:29:55.026445 ValidX-0.8/setup.cfg
+-rw-rw-r--   0 krat      (1000) krat      (1000)     2476 2023-05-31 15:43:17.000000 ValidX-0.8/setup.py
+drwxrwxr-x   0 krat      (1000) krat      (1000)        0 2023-05-31 16:29:55.022445 ValidX-0.8/validx/
+-rw-rw-r--   0 krat      (1000) krat      (1000)     1275 2023-05-31 15:39:22.000000 ValidX-0.8/validx/__init__.py
+-rw-rw-r--   0 krat      (1000) krat      (1000)    13918 2023-03-01 14:03:51.000000 ValidX-0.8/validx/contracts.py
+drwxrwxr-x   0 krat      (1000) krat      (1000)        0 2023-05-31 16:29:55.022445 ValidX-0.8/validx/cy/
+-rw-rw-r--   0 krat      (1000) krat      (1000)     1016 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/__init__.py
+-rw-rw-r--   0 krat      (1000) krat      (1000)       31 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/abstract.pxd
+-rw-rw-r--   0 krat      (1000) krat      (1000)      802 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/abstract.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)     8539 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/abstract.pyx
+-rw-rw-r--   0 krat      (1000) krat      (1000)      561 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/bools.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)     2470 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/bools.pyx
+-rw-rw-r--   0 krat      (1000) krat      (1000)     1338 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/chars.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)     7607 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/chars.pyx
+-rw-rw-r--   0 krat      (1000) krat      (1000)       43 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/classes.pxd
+-rw-rw-r--   0 krat      (1000) krat      (1000)      181 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/classes.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)     1023 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/classes.pyx
+-rw-rw-r--   0 krat      (1000) krat      (1000)     2461 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/containers.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)    18133 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/containers.pyx
+-rw-rw-r--   0 krat      (1000) krat      (1000)     2579 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/datetimes.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)    20718 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/datetimes.pyx
+-rw-rw-r--   0 krat      (1000) krat      (1000)       97 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/instances.pxd
+-rw-rw-r--   0 krat      (1000) krat      (1000)      250 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/instances.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)     1498 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/instances.pyx
+-rw-rw-r--   0 krat      (1000) krat      (1000)     1915 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/numbers.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)    12285 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/numbers.pyx
+-rw-rw-r--   0 krat      (1000) krat      (1000)      584 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/pipelines.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)     2639 2023-03-01 14:03:51.000000 ValidX-0.8/validx/cy/pipelines.pyx
+-rw-rw-r--   0 krat      (1000) krat      (1000)     1382 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/special.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)     8367 2023-05-31 13:56:07.000000 ValidX-0.8/validx/cy/special.pyx
+drwxrwxr-x   0 krat      (1000) krat      (1000)        0 2023-05-31 16:29:55.022445 ValidX-0.8/validx/exc/
+-rw-rw-r--   0 krat      (1000) krat      (1000)     1112 2023-05-31 13:56:07.000000 ValidX-0.8/validx/exc/__init__.py
+-rw-rw-r--   0 krat      (1000) krat      (1000)    10278 2023-05-31 13:56:07.000000 ValidX-0.8/validx/exc/errors.py
+-rw-rw-r--   0 krat      (1000) krat      (1000)     2587 2023-05-31 13:56:07.000000 ValidX-0.8/validx/exc/errors.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)     5411 2023-05-31 13:56:07.000000 ValidX-0.8/validx/exc/formatter.py
+-rw-rw-r--   0 krat      (1000) krat      (1000)      520 2023-03-01 14:03:51.000000 ValidX-0.8/validx/exc/formatter.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)     2869 2023-03-01 14:03:51.000000 ValidX-0.8/validx/exc/markers.py
+-rw-rw-r--   0 krat      (1000) krat      (1000)      451 2023-03-01 14:03:51.000000 ValidX-0.8/validx/exc/markers.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)      949 2023-03-01 14:03:51.000000 ValidX-0.8/validx/platform.py
+drwxrwxr-x   0 krat      (1000) krat      (1000)        0 2023-05-31 16:29:55.026445 ValidX-0.8/validx/py/
+-rw-rw-r--   0 krat      (1000) krat      (1000)     1016 2023-03-01 14:03:51.000000 ValidX-0.8/validx/py/__init__.py
+-rw-rw-r--   0 krat      (1000) krat      (1000)     8922 2023-03-27 17:33:25.000000 ValidX-0.8/validx/py/abstract.py
+-rw-rw-r--   0 krat      (1000) krat      (1000)      802 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/abstract.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)     2239 2023-03-27 17:49:57.000000 ValidX-0.8/validx/py/bools.py
+-rw-rw-r--   0 krat      (1000) krat      (1000)      561 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/bools.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)     6481 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/chars.py
+-rw-rw-r--   0 krat      (1000) krat      (1000)     1338 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/chars.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)     1010 2023-03-01 14:03:51.000000 ValidX-0.8/validx/py/classes.py
+-rw-rw-r--   0 krat      (1000) krat      (1000)      181 2023-03-01 14:03:51.000000 ValidX-0.8/validx/py/classes.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)    15987 2023-03-01 14:03:51.000000 ValidX-0.8/validx/py/containers.py
+-rw-rw-r--   0 krat      (1000) krat      (1000)     2461 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/containers.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)    18974 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/datetimes.py
+-rw-rw-r--   0 krat      (1000) krat      (1000)     2579 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/datetimes.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)     1473 2023-03-01 14:03:51.000000 ValidX-0.8/validx/py/instances.py
+-rw-rw-r--   0 krat      (1000) krat      (1000)      250 2023-03-01 14:03:51.000000 ValidX-0.8/validx/py/instances.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)    10735 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/numbers.py
+-rw-rw-r--   0 krat      (1000) krat      (1000)     1915 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/numbers.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)     2389 2023-03-01 14:03:51.000000 ValidX-0.8/validx/py/pipelines.py
+-rw-rw-r--   0 krat      (1000) krat      (1000)      584 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/pipelines.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)     7350 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/special.py
+-rw-rw-r--   0 krat      (1000) krat      (1000)     1382 2023-05-31 13:56:07.000000 ValidX-0.8/validx/py/special.pyi
+-rw-rw-r--   0 krat      (1000) krat      (1000)        0 2023-03-01 14:03:51.000000 ValidX-0.8/validx/py.typed
```

### Comparing `ValidX-0.7/LICENCE.txt` & `ValidX-0.8/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `ValidX-0.7/README.rst` & `ValidX-0.8/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 ValidX
 ======
 
-..  image:: https://travis-ci.com/Cottonwood-Technology/ValidX.svg?branch=master
-    :target: https://travis-ci.com/Cottonwood-Technology/ValidX
+..  image:: https://github.com/Cottonwood-Technology/ValidX/actions/workflows/main.yaml/badge.svg
+    :target: https://github.com/Cottonwood-Technology/ValidX/actions/workflows/main.yaml
 
 ..  image:: https://badge.fury.io/py/ValidX.svg
     :target: https://badge.fury.io/py/ValidX
 
 ..  image:: https://readthedocs.org/projects/validx/badge/?version=latest
     :target: https://validx.readthedocs.io/en/latest/?badge=latest
```

### Comparing `ValidX-0.7/setup.py` & `ValidX-0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,77 @@
+import os
 import sys
 import platform
+from pathlib import Path
 
 from setuptools import setup, find_packages
 
 
+here = Path(__file__).parent
+os.chdir(here)
+
 ext_modules = []
 requirements = []
+package_data = []
 
 if platform.python_implementation() == "CPython":
     try:
         from Cython.Build import cythonize
     except ImportError:
         print("Unable to import Cython. Pure Python version will be used.")
     else:
-        directives = {"language_level": sys.version_info[0]}
-        ext_modules = cythonize("src/validx/cy/*.pyx", compiler_directives=directives)
+        ext_modules = cythonize(
+            str(here / "validx/cy/*.pyx"),
+            compiler_directives={"language_level": sys.version_info.major},
+        )
 
-with open("src/validx/__init__.py") as f:
+with (here / "validx/__init__.py").open("r") as f:
     version = next(line for line in f if line.startswith("__version__"))
     version = version.strip().split(" = ")[1]
     version = version.strip('"')
 
-with open("README.rst") as f:
+with (here / "README.rst").open("r") as f:
     readme = f.read()
 
-with open("CHANGES.rst") as f:
+with (here / "CHANGES.rst").open("r") as f:
     changes = f.read()
 
+
+src = here / "validx"
+package_data.append("py.typed")
+package_data.extend(str(p.relative_to(src)) for p in src.glob("**/*.pyi"))
+package_data.extend(str(p.relative_to(src)) for p in src.glob("**/*.pyx"))
+package_data.extend(str(p.relative_to(src)) for p in src.glob("**/*.pxd"))
+
+
 setup(
     name="ValidX",
     version=version,
     description="fast, powerful, and flexible validator with sane syntax",
     long_description=readme + "\n\n" + changes,
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Cython",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
+        "Development Status :: 5 - Production/Stable",
     ],
+    python_requires=">=3.6",
     keywords="validator validation validate schema",
     url="https://github.com/Cottonwood-Technology/ValidX",
     author="Cottonwood Technology",
     author_email="info@cottonwood.tech",
     license="BSD",
-    package_dir={"validx": "src/validx"},
-    packages=find_packages(where="src"),
-    package_data={"": ["*.pyi"], "validx": ["py.typed"]},
+    packages=find_packages(where=str(here)),
+    package_data={"validx": package_data},
     zip_safe=False,
     ext_modules=ext_modules,
     install_requires=requirements,
 )
```

### Comparing `ValidX-0.7/src/validx/__init__.py` & `ValidX-0.8/validx/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 
 try:
     from .cy import (
         __impl__,
         Validator,
         Int,
         Float,
+        Decimal,
         Str,
         Bytes,
         Date,
         Time,
         Datetime,
         Bool,
         List,
+        Set,
         Tuple,
         Dict,
         AllOf,
         OneOf,
         LazyRef,
         Type,
         Const,
@@ -26,21 +28,23 @@
     )
 except ImportError:  # pragma: no cover
     from .py import (  # type: ignore
         __impl__,
         Validator,
         Int,
         Float,
+        Decimal,
         Str,
         Bytes,
         Date,
         Time,
         Datetime,
         Bool,
         List,
+        Set,
         Tuple,
         Dict,
         AllOf,
         OneOf,
         LazyRef,
         Type,
         Const,
@@ -51,30 +55,32 @@
 
 
 __all__ = [
     "exc",
     "Validator",
     "Int",
     "Float",
+    "Decimal",
     "Str",
     "Bytes",
     "Date",
     "Time",
     "Datetime",
     "Bool",
     "List",
+    "Set",
     "Tuple",
     "Dict",
     "AllOf",
     "OneOf",
     "LazyRef",
     "Type",
     "Const",
     "Any",
     "classes",
     "instances",
 ]
 
 __impl__ = __impl__
-__version__ = "0.7"
+__version__ = "0.8"
 __author__ = "Cottonwood Technology <info@cottonwood.tech>"
 __license__ = "BSD"
```

### Comparing `ValidX-0.7/src/validx/contracts.py` & `ValidX-0.8/validx/contracts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from collections.abc import Container, Sequence, Mapping, Callable
-
-from .types import chars, frozendict
+from types import MappingProxyType
 
 
 def expect(
-    obj, attr, value, nullable=False, types=None, not_types=None, convert_to=None
+    obj,
+    attr,
+    value,
+    nullable=False,
+    types=None,
+    not_types=None,
+    convert_to=None,
 ):
     """
     Check, whether the value satisfies expectations
 
     :param obj:
         an object,
         which will set the value to its attribute.
@@ -73,18 +78,14 @@
     :param str attr:
         name of an attribute of the object.
         It is used to make error messages more specific.
 
     :param value:
         checked value itself.
 
-    :param bool nullable:
-        accept ``None`` as a valid value.
-        Default: ``False`` — does not accept ``None``.
-
     :raises TypeError:
         if ``not isinstance(value, (bool, int, type(None)))``.
 
     """
     return expect(obj, attr, value, types=(bool, int, type(None)), convert_to=bool)
 
 
@@ -220,15 +221,20 @@
     :returns:
         passed container converted to ``frozenset``,
         if items are hashable,
         otherwise to ``tuple``.
 
     """
     value = expect(
-        obj, attr, value, nullable=nullable, types=Container, not_types=chars
+        obj,
+        attr,
+        value,
+        nullable=nullable,
+        types=Container,
+        not_types=(str, bytes),
     )
     if value is not None:
         if not isinstance(value, frozenset):
             try:
                 value = frozenset(value)
             except TypeError:
                 # Unhashable type, fallback to tuple
@@ -298,15 +304,15 @@
     """
     value = expect(
         obj,
         attr,
         value,
         nullable=nullable,
         types=Sequence,
-        not_types=chars,
+        not_types=(str, bytes),
         convert_to=tuple,
     )
     if value is not None:
         if not value and not empty:
             raise ValueError(
                 "%s.%s.%s should not be empty"
                 % (obj.__class__.__module__, obj.__class__.__name__, attr)
@@ -362,19 +368,24 @@
         * if ``value_type is not None`` and ``isinstance(val, value_type)``,
           ``for key, val in value.items()``.
 
     :raises ValueError:
         if ``not empty`` and ``not value``.
 
     :returns:
-        passed mapping converted to ``frozendict``.
+        passed mapping converted to ``mappingproxy``.
 
     """
     value = expect(
-        obj, attr, value, nullable=nullable, types=Mapping, convert_to=frozendict
+        obj,
+        attr,
+        value,
+        nullable=nullable,
+        types=Mapping,
+        convert_to=MappingProxyType,
     )
     if value is not None:
         if not value and not empty:
             raise ValueError(
                 "%s.%s.%s should not be empty"
                 % (obj.__class__.__module__, obj.__class__.__name__, attr)
             )
@@ -432,15 +443,15 @@
     """
     value = expect(
         obj,
         attr,
         value,
         nullable=nullable,
         types=Sequence,
-        not_types=chars,
+        not_types=(str, bytes),
         convert_to=tuple,
     )
     if value is not None:
         if len(value) != len(struct):
             raise ValueError(
                 "%s.%s.%s should be a tuple of %r"
                 % (obj.__class__.__module__, obj.__class__.__name__, attr, struct)
```

### Comparing `ValidX-0.7/src/validx/cy/__init__.py` & `ValidX-0.8/validx/cy/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from .abstract import Validator
-from .numbers import Int, Float
+from .numbers import Int, Float, Decimal
 from .chars import Str, Bytes
 from .datetimes import Date, Time, Datetime
 from .bools import Bool
-from .containers import List, Tuple, Dict
+from .containers import List, Set, Tuple, Dict
 from .pipelines import AllOf, OneOf
 from .special import LazyRef, Type, Const, Any
 from . import classes, instances
 
 
 __impl__ = "Cython"
 
 __all__ = [
     "Validator",
     "Int",
     "Float",
+    "Decimal",
     "Str",
     "Bytes",
     "Date",
     "Time",
     "Datetime",
     "Bool",
     "List",
+    "Set",
     "Tuple",
     "Dict",
     "AllOf",
     "OneOf",
     "LazyRef",
     "Type",
     "Const",
@@ -33,21 +35,23 @@
     "classes",
     "instances",
 ]
 
 
 classes.add(Int)
 classes.add(Float)
+classes.add(Decimal)
 classes.add(Str)
 classes.add(Bytes)
 classes.add(Date)
 classes.add(Time)
 classes.add(Datetime)
 classes.add(Bool)
 classes.add(List)
+classes.add(Set)
 classes.add(Tuple)
 classes.add(Dict)
 classes.add(AllOf)
 classes.add(OneOf)
 classes.add(LazyRef)
 classes.add(Type)
 classes.add(Const)
```

### Comparing `ValidX-0.7/src/validx/cy/containers.pyi` & `ValidX-0.8/validx/cy/numbers.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,74 @@
 import typing as t
 from . import abstract
 
-class List(abstract.Validator):
+
+class Int(abstract.Validator):
     __slots__: t.Tuple[str, ...]
-    item: abstract.Validator
     nullable: t.Optional[bool]
-    minlen: t.Optional[int]
-    maxlen: t.Optional[int]
-    unique: t.Optional[bool]
+    coerce: t.Optional[bool]
+    min: t.Optional[int]
+    max: t.Optional[int]
+    options: t.Optional[t.Container[int]]
+
     def __init__(
         self,
-        item: abstract.Validator,
         *,
-        nullable: bool = None,
-        minlen: int = None,
-        maxlen: int = None,
-        unique: bool = None,
-        alias: str = None,
+        nullable: t.Optional[bool] = None,
+        coerce: t.Optional[bool] = None,
+        min: t.Optional[int] = None,
+        max: t.Optional[int] = None,
+        options: t.Optional[t.Container[int]] = None,
+        alias: t.Optional[str] = None,
         replace: bool = False,
-    ) -> None: ...
+    ) -> None:
+        ...
 
-class Tuple(abstract.Validator):
+
+class Float(abstract.Validator):
     __slots__: t.Tuple[str, ...]
-    items: t.List[abstract.Validator]
     nullable: t.Optional[bool]
+    coerce: t.Optional[bool]
+    nan: t.Optional[bool]
+    inf: t.Optional[bool]
+    min: t.Optional[float]
+    max: t.Optional[float]
+
     def __init__(
         self,
-        *items: abstract.Validator,
-        nullable: bool = None,
-        alias: str = None,
+        *,
+        nullable: t.Optional[bool] = None,
+        coerce: t.Optional[bool] = None,
+        nan: t.Optional[bool] = None,
+        inf: t.Optional[bool] = None,
+        min: t.Optional[float] = None,
+        max: t.Optional[float] = None,
+        alias: t.Optional[str] = None,
         replace: bool = False,
-    ) -> None: ...
+    ) -> None:
+        ...
+
 
-class Dict(abstract.Validator):
+class Decimal(abstract.Validator):
     __slots__: t.Tuple[str, ...]
-    schema: t.Optional[t.Dict[t.Any, abstract.Validator]]
     nullable: t.Optional[bool]
-    minlen: t.Optional[int]
-    maxlen: t.Optional[int]
-    extra: t.Optional[t.Tuple[abstract.Validator, abstract.Validator]]
-    defaults: t.Optional[t.Dict]
-    optional: t.Optional[t.Container]
-    dispose: t.Optional[t.Container]
-    multikeys: t.Optional[t.Container]
+    coerce: t.Optional[bool]
+    precision: t.Optional[int]
+    nan: t.Optional[bool]
+    inf: t.Optional[bool]
+    min: t.Optional[float]
+    max: t.Optional[float]
+
     def __init__(
         self,
-        schema: t.Dict[t.Any, abstract.Validator] = None,
         *,
-        nullable: bool = None,
-        minlen: int = None,
-        maxlen: int = None,
-        extra: t.Tuple[abstract.Validator, abstract.Validator] = None,
-        defaults: t.Dict = None,
-        optional: t.Container = None,
-        dispose: t.Container = None,
-        multikeys: t.Container = None,
-        alias: str = None,
+        nullable: t.Optional[bool] = None,
+        coerce: t.Optional[bool] = None,
+        precision: t.Optional[int] = None,
+        nan: t.Optional[bool] = None,
+        inf: t.Optional[bool] = None,
+        min: t.Optional[float] = None,
+        max: t.Optional[float] = None,
+        alias: t.Optional[str] = None,
         replace: bool = False,
-    ) -> None: ...
+    ) -> None:
+        ...
```

### Comparing `ValidX-0.7/src/validx/cy/numbers.pyi` & `ValidX-0.8/validx/cy/special.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,60 @@
 import typing as t
 from . import abstract
 
-class Int(abstract.Validator):
+
+class LazyRef(abstract.Validator):
     __slots__: t.Tuple[str, ...]
-    nullable: t.Optional[bool]
-    coerce: t.Optional[bool]
-    min: t.Optional[int]
-    max: t.Optional[int]
-    options: t.Optional[t.Container[int]]
+    use: str
+    maxdepth: t.Optional[int]
+
     def __init__(
         self,
+        use: str,
         *,
-        nullable: bool = None,
-        coerce: bool = None,
-        min: int = None,
-        max: int = None,
-        options: t.Container[int] = None,
-        alias: str = None,
+        maxdepth: t.Optional[int] = None,
+        alias: t.Optional[str] = None,
         replace: bool = False,
-    ) -> None: ...
+    ) -> None:
+        ...
 
-class Float(abstract.Validator):
+
+class Type(abstract.Validator):
     __slots__: t.Tuple[str, ...]
+    tp: t.Type[t.Any]
     nullable: t.Optional[bool]
     coerce: t.Optional[bool]
-    nan: t.Optional[bool]
-    inf: t.Optional[bool]
-    min: t.Optional[float]
-    max: t.Optional[float]
+    min: t.Optional[t.Any]
+    max: t.Optional[t.Any]
+    minlen: t.Optional[int]
+    maxlen: t.Optional[int]
+    options: t.Optional[t.Container[t.Any]]
+
     def __init__(
         self,
+        tp: t.Type[t.Any],
         *,
-        nullable: bool = None,
-        coerce: bool = None,
-        nan: bool = None,
-        inf: bool = None,
-        min: float = None,
-        max: float = None,
-        alias: str = None,
+        nullable: t.Optional[bool] = None,
+        coerce: t.Optional[bool] = None,
+        min: t.Optional[t.Any] = None,
+        max: t.Optional[t.Any] = None,
+        minlen: t.Optional[int] = None,
+        maxlen: t.Optional[int] = None,
+        options: t.Optional[t.Container[t.Any]] = None,
+        alias: t.Optional[str] = None,
         replace: bool = False,
-    ) -> None: ...
+    ) -> None:
+        ...
+
+
+class Const(abstract.Validator):
+    __slots__: t.Tuple[str, ...]
+    value: t.Any
+
+    def __init__(
+        self, value: t.Any, *, alias: t.Optional[str] = None, replace: bool = False
+    ) -> None:
+        ...
+
+
+class Any(abstract.Validator):
+    pass
```

### Comparing `ValidX-0.7/src/validx/cy/special.pyi` & `ValidX-0.8/validx/py/special.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 import typing as t
 from . import abstract
 
+
 class LazyRef(abstract.Validator):
     __slots__: t.Tuple[str, ...]
     use: str
     maxdepth: t.Optional[int]
+
     def __init__(
         self,
         use: str,
         *,
-        maxdepth: int = None,
-        alias: str = None,
+        maxdepth: t.Optional[int] = None,
+        alias: t.Optional[str] = None,
         replace: bool = False,
-    ) -> None: ...
+    ) -> None:
+        ...
+
 
 class Type(abstract.Validator):
     __slots__: t.Tuple[str, ...]
     tp: t.Type[t.Any]
     nullable: t.Optional[bool]
     coerce: t.Optional[bool]
     min: t.Optional[t.Any]
     max: t.Optional[t.Any]
     minlen: t.Optional[int]
     maxlen: t.Optional[int]
     options: t.Optional[t.Container[t.Any]]
+
     def __init__(
         self,
         tp: t.Type[t.Any],
         *,
-        nullable: bool = None,
-        coerce: bool = None,
-        min: t.Any = None,
-        max: t.Any = None,
-        minlen: int = None,
-        maxlen: int = None,
-        options: t.Container[t.Any] = None,
-        alias: str = None,
+        nullable: t.Optional[bool] = None,
+        coerce: t.Optional[bool] = None,
+        min: t.Optional[t.Any] = None,
+        max: t.Optional[t.Any] = None,
+        minlen: t.Optional[int] = None,
+        maxlen: t.Optional[int] = None,
+        options: t.Optional[t.Container[t.Any]] = None,
+        alias: t.Optional[str] = None,
         replace: bool = False,
-    ) -> None: ...
+    ) -> None:
+        ...
+
 
 class Const(abstract.Validator):
     __slots__: t.Tuple[str, ...]
     value: t.Any
+
     def __init__(
-        self, value: t.Any, *, alias: str = None, replace: bool = False
-    ) -> None: ...
+        self, value: t.Any, *, alias: t.Optional[str] = None, replace: bool = False
+    ) -> None:
+        ...
+
 
 class Any(abstract.Validator):
     pass
```

### Comparing `ValidX-0.7/src/validx/exc/__init__.py` & `ValidX-0.8/validx/exc/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from .errors import (
     ValidationError,
     ConditionError,
     InvalidTypeError,
     OptionsError,
+    CoerceError,
     MinValueError,
     MaxValueError,
-    FloatValueError,
+    NumberError,
     StrDecodeError,
     MinLengthError,
     MaxLengthError,
     TupleLengthError,
     PatternMatchError,
     DatetimeParseError,
     DatetimeTypeError,
@@ -24,17 +25,18 @@
 
 
 __all__ = [
     "ValidationError",
     "ConditionError",
     "InvalidTypeError",
     "OptionsError",
+    "CoerceError",
     "MinValueError",
     "MaxValueError",
-    "FloatValueError",
+    "NumberError",
     "StrDecodeError",
     "MinLengthError",
     "MaxLengthError",
     "TupleLengthError",
     "PatternMatchError",
     "DatetimeParseError",
     "DatetimeTypeError",
```

### Comparing `ValidX-0.7/src/validx/exc/errors.py` & `ValidX-0.8/validx/exc/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,26 +177,41 @@
     __slots__ = ValidationError.__slots__ + ("expected", "actual")
 
 
 class InvalidTypeError(ConditionError):
     """
     Invalid Type Error
 
-    :param type expected:
+    :param expected:
         expected type (types).
     :type expected: type or tuple
 
     :param type actual:
         actual type of value.
 
     """
 
     __slots__ = ConditionError.__slots__
 
 
+class CoerceError(ConditionError):
+    """
+    Coerce Error
+
+    :param type expected:
+        expected type.
+
+    :param actual:
+        actual value.
+
+    """
+
+    __slots__ = ConditionError.__slots__
+
+
 class OptionsError(ConditionError):
     """
     Options Error
 
     :param expected:
         list of valid values.
     :type expected: list or tuple
@@ -235,24 +250,26 @@
         actual value.
 
     """
 
     __slots__ = ConditionError.__slots__
 
 
-class FloatValueError(ConditionError):
+class NumberError(ConditionError):
     """
-    Float Value Error
+    Number Error
 
     :param str expected:
         * ``"number"`` on test for ``Not-a-Number``;
         * ``"finite"`` on test for ``Infinity``.
 
-    :param float actual:
+    :param actual:
         actual value.
+    :type actual:
+        float or decimal.Decimal
 
     """
 
     __slots__ = ConditionError.__slots__
 
 
 class StrDecodeError(ConditionError):
```

### Comparing `ValidX-0.7/src/validx/exc/errors.pyi` & `ValidX-0.8/validx/exc/errors.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,128 @@
 from collections.abc import Sequence
 import typing as t
 
+
 class ValidationError(ValueError, Sequence):
     __slots__: t.Tuple[str, ...]
     args: t.Tuple[t.Any, t.Any]
     context: t.Deque
-    def __init__(self, *, context: t.Deque = None, **kw) -> None: ...
-    def add_context(self, node: t.Any) -> ValidationError: ...
-    def __getitem__(self, index: t.Union[int, slice]) -> ValidationError: ...
-    def __len__(self) -> int: ...
-    def __iter__(self) -> t.Iterator[ValidationError]: ...
-    def sort(self, key: t.Callable = None, reverse: bool = False) -> None: ...
-    def __repr__(self) -> str: ...
-    def __str__(self) -> str: ...
-    def format_context(self) -> str: ...
-    def format_error(self) -> str: ...
+
+    def __init__(self, *, context: t.Optional[t.Deque] = None, **kw) -> None:
+        ...
+
+    def add_context(self, node: t.Any) -> ValidationError:
+        ...
+
+    def __getitem__(self, index: t.Union[int, slice]) -> ValidationError:
+        ...
+
+    def __len__(self) -> int:
+        ...
+
+    def __iter__(self) -> t.Iterator[ValidationError]:
+        ...
+
+    def sort(self, key: t.Optional[t.Callable] = None, reverse: bool = False) -> None:
+        ...
+
+    def __repr__(self) -> str:
+        ...
+
+    def __str__(self) -> str:
+        ...
+
+    def format_context(self) -> str:
+        ...
+
+    def format_error(self) -> str:
+        ...
+
 
 class ConditionError(ValidationError):
     __slots__: t.Tuple[str, ...]
     expected: t.Any
     actual: t.Any
+
     def __init__(
-        self, *, context: t.Deque = None, expected: t.Any, actual: t.Any
-    ) -> None: ...
+        self, *, context: t.Optional[t.Deque] = None, expected: t.Any, actual: t.Any
+    ) -> None:
+        ...
+
 
 class InvalidTypeError(ConditionError):
     __slots__: t.Tuple[str, ...]
 
+
 class OptionsError(ConditionError):
     __slots__: t.Tuple[str, ...]
 
+
+class CoerceError(ConditionError):
+    __slots__: t.Tuple[str, ...]
+
+
 class MinValueError(ConditionError):
     __slots__: t.Tuple[str, ...]
 
+
 class MaxValueError(ConditionError):
     __slots__: t.Tuple[str, ...]
 
-class FloatValueError(ConditionError):
+
+class NumberError(ConditionError):
     __slots__: t.Tuple[str, ...]
 
+
 class StrDecodeError(ConditionError):
     __slots__: t.Tuple[str, ...]
 
+
 class MinLengthError(ConditionError):
     __slots__: t.Tuple[str, ...]
 
+
 class MaxLengthError(ConditionError):
     __slots__: t.Tuple[str, ...]
 
+
 class TupleLengthError(ConditionError):
     __slots__: t.Tuple[str, ...]
 
+
 class PatternMatchError(ConditionError):
     __slots__: t.Tuple[str, ...]
 
+
 class DatetimeParseError(ConditionError):
     __slots__: t.Tuple[str, ...]
 
+
 class DatetimeTypeError(ConditionError):
     __slots__: t.Tuple[str, ...]
 
+
 class RecursionMaxDepthError(ConditionError):
     __slots__: t.Tuple[str, ...]
 
+
 class MappingKeyError(ValidationError):
     __slots__: t.Tuple[str, ...]
-    def __init__(self, key: t.Any, **kw) -> None: ...
+
+    def __init__(self, key: t.Any, **kw) -> None:
+        ...
+
 
 class ForbiddenKeyError(MappingKeyError):
     __slots__: t.Tuple[str, ...]
 
+
 class MissingKeyError(MappingKeyError):
     __slots__: t.Tuple[str, ...]
 
+
 class SchemaError(ValidationError):
     __slots__: t.Tuple[str, ...]
     errors: t.List[ValidationError]
-    def __init__(self, errors: t.List[ValidationError]) -> None: ...
+
+    def __init__(self, errors: t.List[ValidationError]) -> None:
+        ...
```

### Comparing `ValidX-0.7/src/validx/exc/formatter.py` & `ValidX-0.8/validx/exc/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,24 +81,27 @@
 
 format_error = Formatter(
     {
         errors.InvalidTypeError: [
             (lambda error: error.actual is type(None), "Value should not be null."),
             "Expected type “{0.expected.__name__}”, got “{0.actual.__name__}”.",
         ],
+        errors.CoerceError: [
+            "Cannot coerce “{0.actual!r}” to type “{0.expected.__name__}”.",
+        ],
         errors.OptionsError: [
             (
                 lambda error: len(error.expected) == 1,
                 "Expected {0.expected[0]}, got {0.actual}.",
             ),
             "Expected one of {0.expected}, got {0.actual}.",
         ],
         errors.MinValueError: "Expected value ≥ {0.expected}, got {0.actual}.",
         errors.MaxValueError: "Expected value ≤ {0.expected}, got {0.actual}.",
-        errors.FloatValueError: [
+        errors.NumberError: [
             (
                 lambda error: error.expected == "finite" and error.actual < 0,
                 "Expected finite number, got -∞.",
             ),
             (
                 lambda error: error.expected == "finite" and error.actual > 0,
                 "Expected finite number, got +∞.",
```

### Comparing `ValidX-0.7/src/validx/exc/formatter.pyi` & `ValidX-0.8/validx/exc/formatter.pyi`

 * *Files identical despite different names*

### Comparing `ValidX-0.7/src/validx/exc/markers.py` & `ValidX-0.8/validx/exc/markers.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.7/src/validx/py/__init__.py` & `ValidX-0.8/validx/py/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from .abstract import Validator
-from .numbers import Int, Float
+from .numbers import Int, Float, Decimal
 from .chars import Str, Bytes
 from .datetimes import Date, Time, Datetime
 from .bools import Bool
-from .containers import List, Tuple, Dict
+from .containers import List, Set, Tuple, Dict
 from .pipelines import AllOf, OneOf
 from .special import LazyRef, Type, Const, Any
 from . import classes, instances
 
 
 __impl__ = "Python"
 
 __all__ = [
     "Validator",
     "Int",
     "Float",
+    "Decimal",
     "Str",
     "Bytes",
     "Date",
     "Time",
     "Datetime",
     "Bool",
     "List",
+    "Set",
     "Tuple",
     "Dict",
     "AllOf",
     "OneOf",
     "LazyRef",
     "Type",
     "Const",
@@ -33,21 +35,23 @@
     "classes",
     "instances",
 ]
 
 
 classes.add(Int)
 classes.add(Float)
+classes.add(Decimal)
 classes.add(Str)
 classes.add(Bytes)
 classes.add(Date)
 classes.add(Time)
 classes.add(Datetime)
 classes.add(Bool)
 classes.add(List)
+classes.add(Set)
 classes.add(Tuple)
 classes.add(Dict)
 classes.add(AllOf)
 classes.add(OneOf)
 classes.add(LazyRef)
 classes.add(Type)
 classes.add(Const)
```

### Comparing `ValidX-0.7/src/validx/py/abstract.py` & `ValidX-0.8/validx/py/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from warnings import warn
 from abc import ABC, abstractmethod
 from collections.abc import Mapping, Sequence, Container
 
 from . import classes, instances
-from ..types import chars
 
 
 class Validator(ABC):
     """
     Abstract Base Validator
 
     :param str alias:
@@ -89,17 +88,17 @@
         """
 
         def _dump(value):
             if isinstance(value, Validator):
                 return value.dump()
             if isinstance(value, Mapping):
                 return {k: _dump(v) for k, v in value.items()}
-            if isinstance(value, Sequence) and not isinstance(value, chars):
+            if isinstance(value, Sequence) and not isinstance(value, (str, bytes)):
                 return [_dump(i) for i in value]
-            if isinstance(value, Container) and not isinstance(value, chars):
+            if isinstance(value, Container) and not isinstance(value, (str, bytes)):
                 return set(value)
             return value
 
         result = {"__class__": self.__class__.__name__}
         for slot, value in self.params():
             result[slot] = _dump(value)
         return result
```

### Comparing `ValidX-0.7/src/validx/py/bools.py` & `ValidX-0.8/validx/py/bools.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.7/src/validx/py/chars.py` & `ValidX-0.8/validx/py/chars.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,24 @@
     """
     Unicode String Validator
 
 
     :param bool nullable:
         accept ``None`` as a valid value.
 
+    :param bool coerce:
+        convert non-string value to ``str``,
+        **use with caution** (see notes below).
+
+    :param bool dontstrip:
+        do not strip leading & trailing whitespace.
+
+    :param bool normspace:
+        normalize spaces, i.e. replace any space sequence by single space char.
+
     :param str encoding:
         try to decode ``bytes`` to ``str`` using specified encoding.
 
     :param int minlen:
         lower length limit.
 
     :param int maxlen:
@@ -44,40 +54,67 @@
 
     :raises PatternMatchError:
         if ``value`` does not match ``self.pattern``.
 
     :raises OptionsError:
         if ``value not in self.options``.
 
+
+    :note:
+        Since any Python object can be converted to a string,
+        using ``coerce`` without other checks in fact validates nothing.
+        It can be useful though to sanitize data from sources with automatic type inferring,
+        where string data might be incorrectly interpreted as another type.
+        For example, phone number as ``int``, version number as ``float``, etc.
+
     """
 
-    __slots__ = ("nullable", "encoding", "minlen", "maxlen", "pattern", "options")
+    __slots__ = (
+        "nullable",
+        "coerce",
+        "dontstrip",
+        "normspace",
+        "encoding",
+        "minlen",
+        "maxlen",
+        "pattern",
+        "options",
+    )
 
     def __init__(
         self,
         nullable=False,
+        coerce=False,
+        dontstrip=False,
+        normspace=False,
         encoding=None,
         minlen=None,
         maxlen=None,
         pattern=None,
         options=None,
         alias=None,
         replace=False,
     ):
         nullable = contracts.expect_flag(self, "nullable", nullable)
+        coerce = contracts.expect_flag(self, "coerce", coerce)
+        dontstrip = contracts.expect_flag(self, "dontstrip", dontstrip)
+        normspace = contracts.expect_flag(self, "normspace", normspace)
         encoding = contracts.expect_str(self, "encoding", encoding, nullable=True)
         minlen = contracts.expect_length(self, "minlen", minlen, nullable=True)
         maxlen = contracts.expect_length(self, "maxlen", maxlen, nullable=True)
         pattern = contracts.expect_str(self, "pattern", pattern, nullable=True)
         options = contracts.expect_container(
             self, "options", options, nullable=True, item_type=str
         )
 
         setattr = object.__setattr__
         setattr(self, "nullable", nullable)
+        setattr(self, "coerce", coerce)
+        setattr(self, "dontstrip", dontstrip)
+        setattr(self, "normspace", normspace)
         setattr(self, "encoding", encoding)
         setattr(self, "minlen", minlen)
         setattr(self, "maxlen", maxlen)
         setattr(self, "pattern", pattern)
         setattr(self, "options", options)
 
         self._register(alias, replace)
@@ -87,16 +124,22 @@
             return value
         if not isinstance(value, str):
             if isinstance(value, bytes) and self.encoding is not None:
                 try:
                     value = value.decode(self.encoding)
                 except UnicodeDecodeError:
                     raise exc.StrDecodeError(expected=self.encoding, actual=value)
+            elif self.coerce:
+                value = str(value)
             else:
                 raise exc.InvalidTypeError(expected=str, actual=type(value))
+        if not self.dontstrip:
+            value = value.strip()
+        if self.normspace:
+            value = re.sub(r"\s+", " ", value)
         length = len(value)
         if self.minlen is not None and length < self.minlen:
             raise exc.MinLengthError(expected=self.minlen, actual=length)
         if self.maxlen is not None and length > self.maxlen:
             raise exc.MaxLengthError(expected=self.maxlen, actual=length)
         if self.pattern and not re.match(self.pattern, value):
             raise exc.PatternMatchError(expected=self.pattern, actual=value)
```

### Comparing `ValidX-0.7/src/validx/py/classes.py` & `ValidX-0.8/validx/py/classes.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.7/src/validx/py/containers.py` & `ValidX-0.8/validx/py/containers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,115 @@
 from copy import deepcopy
-from collections.abc import Sequence, Mapping
+from collections.abc import Sequence, Mapping, Iterable
 
 from .. import contracts
 from .. import exc
-from ..types import chars
 from . import abstract
 
 
 class List(abstract.Validator):
     """
     List Validator
 
 
     :param Validator item:
         validator for list items.
 
     :param bool nullable:
         accept ``None`` as a valid value.
 
+    :param int sort:
+        ``1`` for ascending,
+        ``-1`` for descending.
+
+    :param callable sort_key:
+        function to extract a comparison key.
+
     :param int minlen:
         lower length limit.
 
     :param int maxlen:
         upper length limit.
 
     :param bool unique:
         drop duplicate items.
 
 
     :raises InvalidTypeError:
-        if ``not isinstance(value, (list, tuple))``.
+        if ``not isinstance(value, Iterable)``.
 
     :raises MinLengthError:
         if ``len(value) < self.minlen``.
 
     :raises MaxLengthError:
         if ``len(value) > self.maxlen``.
 
     :raises SchemaError:
         with all errors,
         raised by item validator.
 
     """
 
-    __slots__ = ("item", "nullable", "minlen", "maxlen", "unique")
+    __slots__ = (
+        "item",
+        "nullable",
+        "sort",
+        "sort_key",
+        "minlen",
+        "maxlen",
+        "unique",
+    )
 
     def __init__(
         self,
         item,
         nullable=False,
+        sort=None,
+        sort_key=None,
         minlen=None,
         maxlen=None,
         unique=False,
         alias=None,
         replace=False,
     ):
         item = contracts.expect(self, "item", item, types=abstract.Validator)
         nullable = contracts.expect_flag(self, "nullable", nullable)
+        sort = contracts.expect(self, "sort", sort, types=int, nullable=True)
+        sort_key = contracts.expect_callable(self, "sort_key", sort_key, nullable=True)
         minlen = contracts.expect_length(self, "minlen", minlen, nullable=True)
         maxlen = contracts.expect_length(self, "maxlen", maxlen, nullable=True)
         unique = contracts.expect_flag(self, "unique", unique)
 
         setattr = object.__setattr__
         setattr(self, "item", item)
         setattr(self, "nullable", nullable)
+        setattr(self, "sort", sort)
+        setattr(self, "sort_key", sort_key)
         setattr(self, "minlen", minlen)
         setattr(self, "maxlen", maxlen)
         setattr(self, "unique", unique)
 
         self._register(alias, replace)
 
     def __call__(self, value, __context=None):
         if __context is None:
             __context = {}  # Setup context, if it's top level call
 
         if value is None and self.nullable:
             return value
-        if not isinstance(value, (list, tuple)):
-            if not isinstance(value, Sequence) or isinstance(value, chars):
-                raise exc.InvalidTypeError(expected=Sequence, actual=type(value))
+        if not isinstance(value, (list, tuple, set, frozenset)):
+            if not isinstance(value, Iterable) or isinstance(value, (str, bytes)):
+                raise exc.InvalidTypeError(expected=Iterable, actual=type(value))
 
         result = []
         errors = []
         if self.unique:
             unique = set()
 
-        for num, val in enumerate(value):
+        for num, val in _enumerate(value):
             try:
                 val = self.item(val, __context)
             except exc.ValidationError as e:
                 errors.extend(ne.add_context(num) for ne in e)
                 continue
             if self.unique:
                 if val in unique:
@@ -102,14 +122,107 @@
 
         length = len(result)
         if self.minlen is not None and length < self.minlen:
             raise exc.MinLengthError(expected=self.minlen, actual=length)
         if self.maxlen is not None and length > self.maxlen:
             raise exc.MaxLengthError(expected=self.maxlen, actual=length)
 
+        if self.sort:
+            result.sort(reverse=self.sort < 0, key=self.sort_key)
+
+        return result
+
+
+class Set(abstract.Validator):
+    """
+    Set Validator
+
+
+    :param Validator item:
+        validator for set items.
+
+    :param bool nullable:
+        accept ``None`` as a valid value.
+
+    :param int minlen:
+        lower length limit.
+
+    :param int maxlen:
+        upper length limit.
+
+
+    :raises InvalidTypeError:
+        if ``not isinstance(value, Iterable)``.
+
+    :raises MinLengthError:
+        if ``len(value) < self.minlen``.
+
+    :raises MaxLengthError:
+        if ``len(value) > self.maxlen``.
+
+    :raises SchemaError:
+        with all errors,
+        raised by item validator.
+
+    """
+
+    __slots__ = ("item", "nullable", "minlen", "maxlen")
+
+    def __init__(
+        self,
+        item,
+        nullable=False,
+        minlen=None,
+        maxlen=None,
+        alias=None,
+        replace=False,
+    ):
+        item = contracts.expect(self, "item", item, types=abstract.Validator)
+        nullable = contracts.expect_flag(self, "nullable", nullable)
+        minlen = contracts.expect_length(self, "minlen", minlen, nullable=True)
+        maxlen = contracts.expect_length(self, "maxlen", maxlen, nullable=True)
+
+        setattr = object.__setattr__
+        setattr(self, "item", item)
+        setattr(self, "nullable", nullable)
+        setattr(self, "minlen", minlen)
+        setattr(self, "maxlen", maxlen)
+
+        self._register(alias, replace)
+
+    def __call__(self, value, __context=None):
+        if __context is None:
+            __context = {}  # Setup context, if it's top level call
+
+        if value is None and self.nullable:
+            return value
+        if not isinstance(value, (list, tuple, set, frozenset)):
+            if not isinstance(value, Iterable) or isinstance(value, (str, bytes)):
+                raise exc.InvalidTypeError(expected=Iterable, actual=type(value))
+
+        result = set()
+        errors = []
+
+        for num, val in _enumerate(value):
+            try:
+                val = self.item(val, __context)
+            except exc.ValidationError as e:
+                errors.extend(ne.add_context(num) for ne in e)
+                continue
+            result.add(val)
+
+        if errors:
+            raise exc.SchemaError(errors)
+
+        length = len(result)
+        if self.minlen is not None and length < self.minlen:
+            raise exc.MinLengthError(expected=self.minlen, actual=length)
+        if self.maxlen is not None and length > self.maxlen:
+            raise exc.MaxLengthError(expected=self.maxlen, actual=length)
+
         return result
 
 
 class Tuple(abstract.Validator):
     """
     Tuple Validator
 
@@ -150,15 +263,15 @@
     def __call__(self, value, __context=None):
         if __context is None:
             __context = {}  # Setup context, if it's top level call
 
         if value is None and self.nullable:
             return value
         if not isinstance(value, (list, tuple)):
-            if not isinstance(value, Sequence) or isinstance(value, chars):
+            if not isinstance(value, Sequence) or isinstance(value, (str, bytes)):
                 raise exc.InvalidTypeError(expected=Sequence, actual=type(value))
         if len(self.items) != len(value):
             raise exc.TupleLengthError(expected=len(self.items), actual=len(value))
 
         result = []
         errors = []
 
@@ -398,7 +511,15 @@
         length = len(result)
         if self.minlen is not None and length < self.minlen:
             raise exc.MinLengthError(expected=self.minlen, actual=length)
         if self.maxlen is not None and length > self.maxlen:
             raise exc.MaxLengthError(expected=self.maxlen, actual=length)
 
         return result
+
+
+def _enumerate(iterable):
+    if isinstance(iterable, (list, tuple, Sequence)):
+        yield from enumerate(iterable)
+    else:
+        for value in iterable:
+            yield None, value
```

### Comparing `ValidX-0.7/src/validx/py/containers.pyi` & `ValidX-0.8/validx/py/numbers.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,74 @@
 import typing as t
 from . import abstract
 
-class List(abstract.Validator):
+
+class Int(abstract.Validator):
     __slots__: t.Tuple[str, ...]
-    item: abstract.Validator
     nullable: t.Optional[bool]
-    minlen: t.Optional[int]
-    maxlen: t.Optional[int]
-    unique: t.Optional[bool]
+    coerce: t.Optional[bool]
+    min: t.Optional[int]
+    max: t.Optional[int]
+    options: t.Optional[t.Container[int]]
+
     def __init__(
         self,
-        item: abstract.Validator,
         *,
-        nullable: bool = None,
-        minlen: int = None,
-        maxlen: int = None,
-        unique: bool = None,
-        alias: str = None,
+        nullable: t.Optional[bool] = None,
+        coerce: t.Optional[bool] = None,
+        min: t.Optional[int] = None,
+        max: t.Optional[int] = None,
+        options: t.Optional[t.Container[int]] = None,
+        alias: t.Optional[str] = None,
         replace: bool = False,
-    ) -> None: ...
+    ) -> None:
+        ...
 
-class Tuple(abstract.Validator):
+
+class Float(abstract.Validator):
     __slots__: t.Tuple[str, ...]
-    items: t.List[abstract.Validator]
     nullable: t.Optional[bool]
+    coerce: t.Optional[bool]
+    nan: t.Optional[bool]
+    inf: t.Optional[bool]
+    min: t.Optional[float]
+    max: t.Optional[float]
+
     def __init__(
         self,
-        *items: abstract.Validator,
-        nullable: bool = None,
-        alias: str = None,
+        *,
+        nullable: t.Optional[bool] = None,
+        coerce: t.Optional[bool] = None,
+        nan: t.Optional[bool] = None,
+        inf: t.Optional[bool] = None,
+        min: t.Optional[float] = None,
+        max: t.Optional[float] = None,
+        alias: t.Optional[str] = None,
         replace: bool = False,
-    ) -> None: ...
+    ) -> None:
+        ...
+
 
-class Dict(abstract.Validator):
+class Decimal(abstract.Validator):
     __slots__: t.Tuple[str, ...]
-    schema: t.Optional[t.Dict[t.Any, abstract.Validator]]
     nullable: t.Optional[bool]
-    minlen: t.Optional[int]
-    maxlen: t.Optional[int]
-    extra: t.Optional[t.Tuple[abstract.Validator, abstract.Validator]]
-    defaults: t.Optional[t.Dict]
-    optional: t.Optional[t.Container]
-    dispose: t.Optional[t.Container]
-    multikeys: t.Optional[t.Container]
+    coerce: t.Optional[bool]
+    precision: t.Optional[int]
+    nan: t.Optional[bool]
+    inf: t.Optional[bool]
+    min: t.Optional[float]
+    max: t.Optional[float]
+
     def __init__(
         self,
-        schema: t.Dict[t.Any, abstract.Validator] = None,
         *,
-        nullable: bool = None,
-        minlen: int = None,
-        maxlen: int = None,
-        extra: t.Tuple[abstract.Validator, abstract.Validator] = None,
-        defaults: t.Dict = None,
-        optional: t.Container = None,
-        dispose: t.Container = None,
-        multikeys: t.Container = None,
-        alias: str = None,
+        nullable: t.Optional[bool] = None,
+        coerce: t.Optional[bool] = None,
+        precision: t.Optional[int] = None,
+        nan: t.Optional[bool] = None,
+        inf: t.Optional[bool] = None,
+        min: t.Optional[float] = None,
+        max: t.Optional[float] = None,
+        alias: t.Optional[str] = None,
         replace: bool = False,
-    ) -> None: ...
+    ) -> None:
+        ...
```

### Comparing `ValidX-0.7/src/validx/py/datetimes.py` & `ValidX-0.8/validx/py/datetimes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import date, time, datetime, timedelta, timezone, tzinfo
 
 from .. import exc
 from .. import contracts
-from ..types import numbers
+from .. import platform
 from . import abstract
 
 
 class Date(abstract.Validator):
     """
     Date Validator
 
@@ -40,27 +40,32 @@
     :param tzinfo tz:
         timezone, see notes below.
 
 
     :raises InvalidTypeError:
         * if ``value is None`` and ``not self.nullable``;
         * if ``isinstance(value, (int, float))`` and ``not self.unixts``;
+        * if ``isinstance(value, bool) and self.unixts``,
+          because ``issubclass(bool, int) is True``,
+          but it is very unlikely ``bool`` could represent a valid timestamp;
         * if ``not isinstance(value, date)``.
 
     :raises DatetimeParseError:
         * if ``datetime.strptime(value, self.format)`` raises ``ValueError``;
         * if ``self.parser(value)`` raises ``ValueError``.
 
     :raises MinValueError:
         * if ``value < self.min``;
-        * if ``value < date.today() + self.relmin``.
+        * if ``value < date.today() + self.relmin``;
+        * if ``self.unixts`` and value lesser than the minimal supported timestamp.
 
     :raises MaxValueError:
         * if ``value > self.max``;
-        * if ``value > date.today() + self.relmax``.
+        * if ``value > date.today() + self.relmax``;
+        * if ``self.unixts`` and value greater than the maximal supported timestamp.
 
 
     :note:
         Relative limits are calculated adding deltas to current date,
         use negative ``relmin/relmax`` to specify date in the past.
 
     :note:
@@ -136,18 +141,35 @@
         self._register(alias, replace)
 
     def __call__(self, value, __context=None):
         if value is None and self.nullable:
             return value
 
         if not isinstance(value, (date, datetime)):
-            if isinstance(value, numbers) and self.unixts:
+            if (
+                isinstance(value, (int, float))
+                and not isinstance(value, bool)
+                and self.unixts
+            ):
                 # Value will be arranged to ``self.tz`` below.
                 tz = None if self.tz is None else timezone.utc
-                value = datetime.fromtimestamp(value, tz)
+                try:
+                    value = datetime.fromtimestamp(value, tz)
+                except (ValueError, OSError, OverflowError):
+                    raise (
+                        exc.MaxValueError(
+                            expected=platform.MAX_TIMESTAMP,
+                            actual=value,
+                        )
+                        if value > 0
+                        else exc.MinValueError(
+                            expected=platform.MIN_TIMESTAMP,
+                            actual=value,
+                        )
+                    )
             elif isinstance(value, str) and self.format is not None:
                 try:
                     value = datetime.strptime(value, self.format)
                 except ValueError:
                     raise exc.DatetimeParseError(expected=self.format, actual=value)
             elif isinstance(value, str) and self.parser is not None:
                 try:
@@ -297,65 +319,76 @@
 
     :param timedelta relmin:
         relative lower limit.
 
     :param timedelta relmax:
         relative upper limit.
 
+    :param time default_time:
+        is used to implicitly convert ``date`` to ``datetime``
+        using ``datetime.combine(value, self.default_time or time(tzinfo=self.tz))``.
+
     :param tzinfo tz:
         timezone.
 
 
     :raises InvalidTypeError:
         * if ``value is None`` and ``not self.nullable``;
         * if ``isinstance(value, (int, float))`` and ``not self.unixts``;
+        * if ``isinstance(value, bool) and self.unixts``,
+          because ``issubclass(bool, int) is True``,
+          but it is very unlikely ``bool`` could represent a valid timestamp;
         * if ``not isinstance(value, datetime)``.
 
     :raises DatetimeParseError:
         * if ``datetime.strptime(value, self.format)`` raises ``ValueError``;
         * if ``self.parser(value)`` raises ``ValueError``.
 
     :raises DatetimeTypeError:
         * if ``self.tz is None and value.tzinfo is not None``;
         * if ``self.tz is not None and value.tzinfo is None``;
 
     :raises MinValueError:
         * if ``value < self.min``;
         * if ``self.tz is None and value < datetime.now() + self.relmin``.
-        * if ``self.tz is not None and value < datetime.now(UTC).astimezone(self.tz) + self.relmin``.
+        * if ``self.tz is not None and value < datetime.now(UTC).astimezone(self.tz) + self.relmin``;
+        * if ``self.unixts`` and value lesser than the minimal supported timestamp.
 
     :raises MaxValueError:
         * if ``value > self.max``;
         * if ``self.tz is None and value > datetime.now() + self.relmax``.
-        * if ``self.tz is not None and value > datetime.now(UTC).astimezone(self.tz) + self.relmax``.
+        * if ``self.tz is not None and value > datetime.now(UTC).astimezone(self.tz) + self.relmax``;
+        * if ``self.unixts`` and value greater than the maximal supported timestamp.
 
     """
 
     __slots__ = (
         "nullable",
         "unixts",
         "format",
         "parser",
         "min",
         "max",
         "relmin",
         "relmax",
+        "default_time",
         "tz",
     )
 
     def __init__(
         self,
         nullable=False,
         unixts=False,
         format=None,
         parser=None,
         min=None,
         max=None,
         relmin=None,
         relmax=None,
+        default_time=None,
         tz=None,
         alias=None,
         replace=False,
     ):
         nullable = contracts.expect_flag(self, "nullable", nullable)
         unixts = contracts.expect_flag(self, "unixts", unixts)
         format = contracts.expect_str(self, "format", format, nullable=True)
@@ -364,14 +397,17 @@
         max = contracts.expect(self, "max", max, types=datetime, nullable=True)
         relmin = contracts.expect(
             self, "relmin", relmin, types=timedelta, nullable=True
         )
         relmax = contracts.expect(
             self, "relmax", relmax, types=timedelta, nullable=True
         )
+        default_time = contracts.expect(
+            self, "default_time", default_time, types=time, nullable=True
+        )
         tz = contracts.expect(self, "tz", tz, types=tzinfo, nullable=True)
 
         if tz is not None:
             if min is not None:
                 if min.tzinfo is None:
                     raise ValueError(
                         "%s.%s.min should be timezone-aware datetime object"
@@ -381,51 +417,83 @@
             if max is not None:
                 if max.tzinfo is None:
                     raise ValueError(
                         "%s.%s.max should be timezone-aware datetime object"
                         % (self.__class__.__module__, self.__class__.__name__)
                     )
                 max = max.astimezone(tz)
+            if default_time is not None:
+                if default_time.tzinfo is None:
+                    raise ValueError(
+                        "%s.%s.default_time should be timezone-aware time object"
+                        % (self.__class__.__module__, self.__class__.__name__)
+                    )
         else:
             if min is not None and min.tzinfo is not None:
                 raise ValueError(
                     "%s.%s.min should be naive datetime object"
                     % (self.__class__.__module__, self.__class__.__name__)
                 )
             if max is not None and max.tzinfo is not None:
                 raise ValueError(
                     "%s.%s.max should be naive datetime object"
                     % (self.__class__.__module__, self.__class__.__name__)
                 )
+            if default_time is not None and default_time.tzinfo is not None:
+                raise ValueError(
+                    "%s.%s.default_time should be naive time object"
+                    % (self.__class__.__module__, self.__class__.__name__)
+                )
 
         setattr = object.__setattr__
         setattr(self, "nullable", nullable)
         setattr(self, "unixts", unixts)
         setattr(self, "format", format)
         setattr(self, "parser", parser)
         setattr(self, "min", min)
         setattr(self, "max", max)
         setattr(self, "relmin", relmin)
         setattr(self, "relmax", relmax)
+        setattr(self, "default_time", default_time)
         setattr(self, "tz", tz)
 
         self._register(alias, replace)
 
     def __call__(self, value, __context=None):
         if value is None and self.nullable:
             return value
 
         if not isinstance(value, datetime):
             if isinstance(value, date):
                 # Implicitly convert ``date`` to ``datetime``
-                value = datetime.combine(value, time(tzinfo=self.tz))
-            elif isinstance(value, numbers) and self.unixts:
+                value = datetime.combine(
+                    value,
+                    self.default_time or time(tzinfo=self.tz),
+                )
+            elif (
+                isinstance(value, (int, float))
+                and not isinstance(value, bool)
+                and self.unixts
+            ):
                 # Value will be arranged to ``self.tz`` below.
                 tz = None if self.tz is None else timezone.utc
-                value = datetime.fromtimestamp(value, tz)
+                try:
+                    value = datetime.fromtimestamp(value, tz)
+                except (ValueError, OSError, OverflowError):
+                    raise (
+                        exc.MaxValueError(
+                            expected=platform.MAX_TIMESTAMP,
+                            actual=value,
+                        )
+                        if value > 0
+                        else exc.MinValueError(
+                            expected=platform.MIN_TIMESTAMP,
+                            actual=value,
+                        )
+                    )
             elif isinstance(value, str) and self.format is not None:
                 try:
                     value = datetime.strptime(value, self.format)
                 except ValueError:
                     raise exc.DatetimeParseError(expected=self.format, actual=value)
             elif isinstance(value, str) and self.parser is not None:
                 try:
```

### Comparing `ValidX-0.7/src/validx/py/instances.py` & `ValidX-0.8/validx/py/instances.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.7/src/validx/py/numbers.py` & `ValidX-0.8/validx/py/special.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,207 +1,259 @@
-import math
-
-from .. import contracts
 from .. import exc
-from ..types import numbers
-from . import abstract
+from .. import contracts
+from . import abstract, instances
+
+
+class LazyRef(abstract.Validator):
+    """
+    Lazy Referenced Validator
+
+    It is useful to build validators for recursive structures.
+
+    ..  testsetup:: lazyref
+
+        from validx import Dict, Int, LazyRef, instances
+
+    ..  testcleanup:: lazyref
+
+        instances.clear()
+
+    ..  doctest:: lazyref
+        :options: +ELLIPSIS, -IGNORE_EXCEPTION_DETAIL
+
+        >>> schema = Dict(
+        ...     {
+        ...         "foo": Int(),
+        ...         "bar": LazyRef("schema", maxdepth=1),
+        ...     },
+        ...     optional=("foo", "bar"),
+        ...     minlen=1,
+        ...     alias="schema",
+        ... )
+
+        >>> schema({"foo": 1})
+        {'foo': 1}
+
+        >>> schema({"bar": {"foo": 1}})
+        {'bar': {'foo': 1}}
+
+        >>> schema({"bar": {"bar": {"foo": 1}}})
+        Traceback (most recent call last):
+            ...
+        validx.exc.errors.SchemaError: <SchemaError(errors=[
+            <bar.bar: RecursionMaxDepthError(expected=1, actual=2)>
+        ])>
+
+    :param str use:
+        alias of referenced validator.
+
+    :param int maxdepth:
+        maximum recursion depth.
+
+
+    :raises RecursionMaxDepthError:
+        if ``self.maxdepth is not None``
+        and current recursion depth exceeds the limit.
+
+    """
 
+    __slots__ = ("use", "maxdepth")
 
-class Int(abstract.Validator):
+    def __init__(self, use, maxdepth=None, alias=None, replace=False):
+        use = contracts.expect_str(self, "use", use)
+        maxdepth = contracts.expect_length(self, "maxdepth", maxdepth, nullable=True)
+
+        setattr = object.__setattr__
+        setattr(self, "use", use)
+        setattr(self, "maxdepth", maxdepth)
+
+        self._register(alias, replace)
+
+    def __call__(self, value, __context=None):
+        if __context is None:
+            __context = {}  # Setup context, if it's top level call
+
+        instance = instances.get(self.use)
+        if self.maxdepth is None:
+            return instance(value, __context)
+
+        try:
+            key = self.use + ".recursion_depth"
+            depth = __context.setdefault(key, 0) + 1
+            if depth > self.maxdepth:
+                raise exc.RecursionMaxDepthError(expected=self.maxdepth, actual=depth)
+            __context[key] = depth
+            return instance(value, __context)
+        finally:
+            __context[key] -= 1
+
+
+class Type(abstract.Validator):
     """
-    Integer Number Validator
+    Custom Type Validator
 
+    :param type tp:
+        valid value type.
 
     :param bool nullable:
         accept ``None`` as a valid value.
 
     :param bool coerce:
-        try to convert non-integer value to ``int``.
+        try to convert value to ``tp``.
+
+    :param tp min:
+        lower limit, makes sense only if ``tp`` provides comparison methods.
+
+    :param tp max:
+        upper limit, makes sense only if ``tp`` provides comparison methods.
 
-    :param int min:
-        lower limit.
+    :param int minlen:
+        lower length limit, makes sense only if ``tp`` provides ``__len__()`` method.
 
-    :param int max:
-        upper limit.
+    :param int maxlen:
+        upper length limit, makes sense only if ``tp`` provides ``__len__()`` method.
 
     :param iterable options:
         explicit enumeration of valid values.
 
 
     :raises InvalidTypeError:
         * if ``value is None`` and ``not self.nullable``;
-        * if ``not isinstance(value, int)`` and ``not self.coerce``;
-        * if ``int(value)`` raises ``ValueError`` or ``TypeError``.
+        * if ``not isinstance(value, self.tp)`` and ``not self.coerce``.
+
+    :raises CoerceError:
+        if ``self.coerce`` and ``tp(value)`` raises an exception.
 
     :raises MinValueError:
         if ``value < self.min``.
 
     :raises MaxValueError:
         if ``value > self.max``.
 
-    :raises OptionsError:
-        if ``value not in self.options``.
+    :raises MinLengthError:
+        if ``len(value) < self.minlen``.
 
+    :raises MaxLengthError:
+        if ``len(value) > self.maxlen``.
 
-    :note:
-        It implicitly converts ``float`` to ``int``,
-        if ``value.is_integer() is True``.
+    :raises OptionsError:
+        if ``value not in self.options``.
 
     """
 
-    __slots__ = ("nullable", "coerce", "min", "max", "options")
+    __slots__ = (
+        "tp",
+        "nullable",
+        "coerce",
+        "min",
+        "max",
+        "minlen",
+        "maxlen",
+        "options",
+    )
 
     def __init__(
         self,
+        tp,
         nullable=False,
         coerce=False,
         min=None,
         max=None,
+        minlen=None,
+        maxlen=None,
         options=None,
         alias=None,
         replace=False,
     ):
+        tp = contracts.expect(self, "tp", tp, types=type)
         nullable = contracts.expect_flag(self, "nullable", nullable)
         coerce = contracts.expect_flag(self, "coerce", coerce)
-        min = contracts.expect(self, "min", min, nullable=True, types=int)
-        max = contracts.expect(self, "max", max, nullable=True, types=int)
+        min = contracts.expect(self, "min", min, types=tp, nullable=True)
+        max = contracts.expect(self, "max", max, types=tp, nullable=True)
+        minlen = contracts.expect_length(self, "minlen", minlen, nullable=True)
+        maxlen = contracts.expect_length(self, "maxlen", maxlen, nullable=True)
         options = contracts.expect_container(
-            self, "options", options, nullable=True, item_type=int
+            self, "options", options, nullable=True, item_type=tp
         )
 
+        if minlen is not None or maxlen is not None:
+            if not hasattr(tp, "__len__"):
+                raise TypeError("Type %r does not provide method '__len__()'" % tp)
+
         setattr = object.__setattr__
+        setattr(self, "tp", tp)
         setattr(self, "nullable", nullable)
         setattr(self, "coerce", coerce)
         setattr(self, "min", min)
         setattr(self, "max", max)
+        setattr(self, "minlen", minlen)
+        setattr(self, "maxlen", maxlen)
         setattr(self, "options", options)
 
         self._register(alias, replace)
 
     def __call__(self, value, __context=None):
         if value is None and self.nullable:
             return value
-        if not isinstance(value, int):
-            if isinstance(value, float) and value.is_integer():
-                # Implicitly convert ``float`` to ``int``,
-                # if the value represents integer number
-                value = int(value)
-            elif not self.coerce:
-                raise exc.InvalidTypeError(expected=int, actual=type(value))
+        if not isinstance(value, self.tp):
+            if not self.coerce:
+                raise exc.InvalidTypeError(expected=self.tp, actual=type(value))
             else:
                 try:
-                    value = int(value)
-                except (TypeError, ValueError):
-                    raise exc.InvalidTypeError(expected=int, actual=type(value))
+                    value = self.tp(value)
+                except Exception:
+                    raise exc.CoerceError(expected=self.tp, actual=value)
         if self.min is not None and value < self.min:
             raise exc.MinValueError(expected=self.min, actual=value)
         if self.max is not None and value > self.max:
             raise exc.MaxValueError(expected=self.max, actual=value)
+        if self.minlen is not None or self.maxlen is not None:
+            length = len(value)
+            if self.minlen is not None and length < self.minlen:
+                raise exc.MinLengthError(expected=self.minlen, actual=length)
+            if self.maxlen is not None and length > self.maxlen:
+                raise exc.MaxLengthError(expected=self.maxlen, actual=length)
         if self.options is not None and value not in self.options:
             raise exc.OptionsError(expected=self.options, actual=value)
         return value
 
 
-class Float(abstract.Validator):
+class Const(abstract.Validator):
     """
-    Floating Point Number Validator
-
-
-    :param bool nullable:
-        accept ``None`` as a valid value.
-
-    :param bool coerce:
-        try to convert non-float value to ``float``.
+    Constant Validator
 
-    :param bool nan:
-        accept ``Not-a-Number`` as a valid value.
+    It only accepts single predefined value.
 
-    :param bool inf:
-        accept ``Infinity`` as a valid value.
 
-    :param float min:
-        lower limit.
+    :param value:
+        expected valid value.
 
-    :param float max:
-        upper limit.
 
+    :raises OptionsError:
+        if ``value != self.value``.
 
-    :raises InvalidTypeError:
-        * if ``value is None`` and ``not self.nullable``;
-        * if ``not isinstance(value, float)`` and ``not self.coerce``;
-        * if ``float(value)`` raises ``ValueError`` or ``TypeError``.
+    """
 
-    :raises FloatValueError:
-        * if ``math.isnan(value)`` and ``not self.nan``;
-        * if ``math.isinf(value)`` and ``not self.inf``.
+    __slots__ = ("value",)
 
-    :raises MinValueError:
-        if ``value < self.min``.
+    def __init__(self, value, alias=None, replace=False):
+        setattr = object.__setattr__
+        setattr(self, "value", value)
 
-    :raises MaxValueError:
-        if ``value > self.max``.
+        self._register(alias, replace)
 
+    def __call__(self, value, __context=None):
+        if value != self.value:
+            raise exc.OptionsError(expected=[self.value], actual=value)
+        return value
 
-    :note: It always converts ``int`` to ``float``.
 
+class Any(abstract.Validator):
     """
+    Pass-Any Validator
 
-    __slots__ = ("nullable", "coerce", "nan", "inf", "min", "max")
-
-    def __init__(
-        self,
-        nullable=False,
-        coerce=False,
-        nan=False,
-        inf=False,
-        min=None,
-        max=None,
-        alias=None,
-        replace=False,
-    ):
-        nullable = contracts.expect_flag(self, "nullable", nullable)
-        coerce = contracts.expect_flag(self, "coerce", coerce)
-        nan = contracts.expect_flag(self, "nan", nan)
-        inf = contracts.expect_flag(self, "inf", inf)
-        min = contracts.expect(
-            self, "min", min, nullable=True, types=numbers, convert_to=float
-        )
-        max = contracts.expect(
-            self, "max", max, nullable=True, types=numbers, convert_to=float
-        )
-
-        setattr = object.__setattr__
-        setattr(self, "nullable", nullable)
-        setattr(self, "coerce", coerce)
-        setattr(self, "nan", nan)
-        setattr(self, "inf", inf)
-        setattr(self, "min", min)
-        setattr(self, "max", max)
+    It literally accepts any value.
 
-        self._register(alias, replace)
+    """
 
     def __call__(self, value, __context=None):
-        if value is None and self.nullable:
-            return value
-        if not isinstance(value, float):
-            if isinstance(value, int):
-                # Always implicitly convert ``int`` to ``float``
-                value = float(value)
-            elif not self.coerce:
-                raise exc.InvalidTypeError(expected=float, actual=type(value))
-            else:
-                try:
-                    value = float(value)
-                except (TypeError, ValueError):
-                    raise exc.InvalidTypeError(expected=float, actual=type(value))
-        if math.isnan(value):
-            if not self.nan:
-                raise exc.FloatValueError(expected="number", actual=value)
-            # It doesn't make sence to future checks if value is ``Nan``
-            return value
-        if math.isinf(value) and not self.inf:
-            raise exc.FloatValueError(expected="finite", actual=value)
-        if self.min is not None and value < self.min:
-            raise exc.MinValueError(expected=self.min, actual=value)
-        if self.max is not None and value > self.max:
-            raise exc.MaxValueError(expected=self.max, actual=value)
         return value
```

### Comparing `ValidX-0.7/src/validx/py/pipelines.py` & `ValidX-0.8/validx/py/pipelines.py`

 * *Files identical despite different names*

### Comparing `ValidX-0.7/src/validx/py/special.py` & `ValidX-0.8/validx/cy/special.pyx`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from libc cimport limits
+
 from .. import exc
 from .. import contracts
-from . import abstract, instances
+from . cimport abstract, instances
 
 
-class LazyRef(abstract.Validator):
+cdef class LazyRef(abstract.Validator):
     """
     Lazy Referenced Validator
 
     It is useful to build validators for recursive structures.
 
     ..  testsetup:: lazyref
 
@@ -54,44 +56,55 @@
         if ``self.maxdepth is not None``
         and current recursion depth exceeds the limit.
 
     """
 
     __slots__ = ("use", "maxdepth")
 
+    cdef str _use
+    cdef long _maxdepth
+
+    @property
+    def use(self):
+        return self._use
+
+    @property
+    def maxdepth(self):
+        return None if self._maxdepth == 0 else self._maxdepth
+
     def __init__(self, use, maxdepth=None, alias=None, replace=False):
         use = contracts.expect_str(self, "use", use)
         maxdepth = contracts.expect_length(self, "maxdepth", maxdepth, nullable=True)
 
-        setattr = object.__setattr__
-        setattr(self, "use", use)
-        setattr(self, "maxdepth", maxdepth)
+        self._use = use
+        self._maxdepth = 0 if maxdepth is None else maxdepth
 
         self._register(alias, replace)
 
     def __call__(self, value, __context=None):
         if __context is None:
             __context = {}  # Setup context, if it's top level call
 
         instance = instances.get(self.use)
-        if self.maxdepth is None:
+        if self._maxdepth == 0:
             return instance(value, __context)
 
+        cdef long depth
         try:
             key = self.use + ".recursion_depth"
             depth = __context.setdefault(key, 0) + 1
-            if depth > self.maxdepth:
-                raise exc.RecursionMaxDepthError(expected=self.maxdepth, actual=depth)
+            if depth > self._maxdepth:
+                raise exc.RecursionMaxDepthError(expected=self._maxdepth, actual=depth)
             __context[key] = depth
             return instance(value, __context)
         finally:
             __context[key] -= 1
 
 
-class Type(abstract.Validator):
+cdef class Type(abstract.Validator):
     """
     Custom Type Validator
 
     :param type tp:
         valid value type.
 
     :param bool nullable:
@@ -114,16 +127,18 @@
 
     :param iterable options:
         explicit enumeration of valid values.
 
 
     :raises InvalidTypeError:
         * if ``value is None`` and ``not self.nullable``;
-        * if ``not isinstance(value, self.tp)`` and ``not self.coerce``;
-        * if ``self.tp(value)`` raises ``ValueError`` or ``TypeError``.
+        * if ``not isinstance(value, self.tp)`` and ``not self.coerce``.
+
+    :raises CoerceError:
+        if ``self.coerce`` and ``tp(value)`` raises an exception.
 
     :raises MinValueError:
         if ``value < self.min``.
 
     :raises MaxValueError:
         if ``value > self.max``.
 
@@ -145,14 +160,55 @@
         "min",
         "max",
         "minlen",
         "maxlen",
         "options",
     )
 
+    cdef object _tp
+    cdef bint _nullable
+    cdef bint _coerce
+    cdef object _min
+    cdef object _max
+    cdef long _minlen
+    cdef long _maxlen
+    cdef object _options
+
+    @property
+    def tp(self):
+        return self._tp
+
+    @property
+    def nullable(self):
+        return self._nullable
+
+    @property
+    def coerce(self):
+        return self._coerce
+
+    @property
+    def min(self):
+        return self._min
+
+    @property
+    def max(self):
+        return self._max
+
+    @property
+    def minlen(self):
+        return None if self._minlen == 0 else self._minlen
+
+    @property
+    def maxlen(self):
+        return None if self._maxlen == limits.LONG_MAX else self._maxlen
+
+    @property
+    def options(self):
+        return self._options
+
     def __init__(
         self,
         tp,
         nullable=False,
         coerce=False,
         min=None,
         max=None,
@@ -173,53 +229,53 @@
             self, "options", options, nullable=True, item_type=tp
         )
 
         if minlen is not None or maxlen is not None:
             if not hasattr(tp, "__len__"):
                 raise TypeError("Type %r does not provide method '__len__()'" % tp)
 
-        setattr = object.__setattr__
-        setattr(self, "tp", tp)
-        setattr(self, "nullable", nullable)
-        setattr(self, "coerce", coerce)
-        setattr(self, "min", min)
-        setattr(self, "max", max)
-        setattr(self, "minlen", minlen)
-        setattr(self, "maxlen", maxlen)
-        setattr(self, "options", options)
+        self._tp = tp
+        self._nullable = nullable
+        self._coerce = coerce
+        self._min = min
+        self._max = max
+        self._minlen = 0 if minlen is None else minlen
+        self._maxlen = limits.LONG_MAX if maxlen is None else maxlen
+        self._options = options
 
         self._register(alias, replace)
 
     def __call__(self, value, __context=None):
         if value is None and self.nullable:
             return value
         if not isinstance(value, self.tp):
             if not self.coerce:
                 raise exc.InvalidTypeError(expected=self.tp, actual=type(value))
             else:
                 try:
                     value = self.tp(value)
-                except (TypeError, ValueError):
-                    raise exc.InvalidTypeError(expected=self.tp, actual=type(value))
+                except Exception:
+                    raise exc.CoerceError(expected=self.tp, actual=value)
         if self.min is not None and value < self.min:
             raise exc.MinValueError(expected=self.min, actual=value)
         if self.max is not None and value > self.max:
             raise exc.MaxValueError(expected=self.max, actual=value)
+        cdef long length
         if self.minlen is not None or self.maxlen is not None:
             length = len(value)
             if self.minlen is not None and length < self.minlen:
                 raise exc.MinLengthError(expected=self.minlen, actual=length)
             if self.maxlen is not None and length > self.maxlen:
                 raise exc.MaxLengthError(expected=self.maxlen, actual=length)
         if self.options is not None and value not in self.options:
             raise exc.OptionsError(expected=self.options, actual=value)
         return value
 
 
-class Const(abstract.Validator):
+cdef class Const(abstract.Validator):
     """
     Constant Validator
 
     It only accepts single predefined value.
 
 
     :param value:
@@ -229,29 +285,34 @@
     :raises OptionsError:
         if ``value != self.value``.
 
     """
 
     __slots__ = ("value",)
 
-    def __init__(self, value, alias=None, replace=False):
-        setattr = object.__setattr__
-        setattr(self, "value", value)
+    cdef object _value
+
+    @property
+    def value(self):
+        return self._value
 
+    def __init__(self, value, alias=None, replace=False):
+        self._value = value
         self._register(alias, replace)
 
     def __call__(self, value, __context=None):
         if value != self.value:
             raise exc.OptionsError(expected=[self.value], actual=value)
         return value
 
 
-class Any(abstract.Validator):
+cdef class Any(abstract.Validator):
     """
     Pass-Any Validator
 
     It literally accepts any value.
 
     """
 
     def __call__(self, value, __context=None):
         return value
+
```

