# Comparing `tmp/aiositi-mex-0.0.4.tar.gz` & `tmp/aiositi-mex-0.0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiositi-mex-0.0.4.tar", last modified: Wed Mar  1 02:11:26 2023, max compression
+gzip compressed data, was "aiositi-mex-0.0.5.dev0.tar", last modified: Wed May 31 19:53:01 2023, max compression
```

## Comparing `aiositi-mex-0.0.4.tar` & `aiositi-mex-0.0.5.dev0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:26.886771 aiositi-mex-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-03-01 02:11:26.886771 aiositi-mex-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:26.878771 aiositi-mex-0.0.4/aiositi_mex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-03-01 02:11:26.000000 aiositi-mex-0.0.4/aiositi_mex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-03-01 02:11:26.000000 aiositi-mex-0.0.4/aiositi_mex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 02:11:26.000000 aiositi-mex-0.0.4/aiositi_mex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-01 02:11:26.000000 aiositi-mex-0.0.4/aiositi_mex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-01 02:11:26.000000 aiositi-mex-0.0.4/aiositi_mex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-01 02:11:26.886771 aiositi-mex-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:26.878771 aiositi-mex-0.0.4/siti/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:26.878771 aiositi-mex-0.0.4/siti/http/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/http/oauth_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:26.878771 aiositi-mex-0.0.4/siti/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:26.878771 aiositi-mex-0.0.4/siti/resources/ifpe/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/catalogos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:26.878771 aiositi-mex-0.0.4/siti/resources/ifpe/r01/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r01/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r01/reporte_111.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:26.882771 aiositi-mex-0.0.4/siti/resources/ifpe/r08/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r08/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r08/reporte_843.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:26.882771 aiositi-mex-0.0.4/siti/resources/ifpe/r10/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r10/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r10/reporte_10111.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r10/reporte_10121.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:26.882771 aiositi-mex-0.0.4/siti/resources/ifpe/r13/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r13/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r13/reporte_13111.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r13/reporte_13161.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r13/reporte_13211.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r13/reporte_13221.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:26.882771 aiositi-mex-0.0.4/siti/resources/ifpe/r24/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r24/reporte_2471.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r24/reporte_2472.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:26.882771 aiositi-mex-0.0.4/siti/resources/ifpe/r26/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r26/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r26/reporte_2610.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r26/reporte_2611.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r26/reporte_2612.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r26/reporte_2613.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:26.882771 aiositi-mex-0.0.4/siti/resources/ifpe/r27/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r27/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r27/reporte_2701.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:26.886771 aiositi-mex-0.0.4/siti/resources/ifpe/r36/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r36/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r36/reporte_3611.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r36/reporte_3612.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/r36/reporte_3613.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/reportes.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/seguimiento.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/resources/ifpe/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/siti/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:26.886771 aiositi-mex-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:26.886771 aiositi-mex-0.0.4/tests/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/tests/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/tests/http/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/tests/http/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-03-01 02:11:18.000000 aiositi-mex-0.0.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:53:01.613429 aiositi-mex-0.0.5.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-31 19:53:01.613429 aiositi-mex-0.0.5.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:53:01.609429 aiositi-mex-0.0.5.dev0/aiositi_mex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-31 19:53:01.000000 aiositi-mex-0.0.5.dev0/aiositi_mex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-31 19:53:01.000000 aiositi-mex-0.0.5.dev0/aiositi_mex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:53:01.000000 aiositi-mex-0.0.5.dev0/aiositi_mex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-31 19:53:01.000000 aiositi-mex-0.0.5.dev0/aiositi_mex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 19:53:01.000000 aiositi-mex-0.0.5.dev0/aiositi_mex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-31 19:53:01.613429 aiositi-mex-0.0.5.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:53:01.609429 aiositi-mex-0.0.5.dev0/siti/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:53:01.609429 aiositi-mex-0.0.5.dev0/siti/http/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/http/oauth_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:53:01.609429 aiositi-mex-0.0.5.dev0/siti/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:53:01.609429 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/catalogos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:53:01.609429 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r01/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r01/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r01/reporte_111.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:53:01.609429 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r08/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r08/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r08/reporte_843.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:53:01.609429 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r10/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r10/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r10/reporte_10111.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r10/reporte_10121.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:53:01.613429 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r13/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r13/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r13/reporte_13111.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r13/reporte_13161.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r13/reporte_13211.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r13/reporte_13221.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:53:01.613429 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r24/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r24/reporte_2471.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r24/reporte_2472.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:53:01.613429 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r26/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r26/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r26/reporte_2610.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r26/reporte_2611.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r26/reporte_2612.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r26/reporte_2613.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:53:01.613429 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r27/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r27/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r27/reporte_2701.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:53:01.613429 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r36/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r36/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r36/reporte_3611.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r36/reporte_3612.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r36/reporte_3613.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/reportes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/seguimiento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/resources/ifpe/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/siti/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:53:01.613429 aiositi-mex-0.0.5.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:53:01.613429 aiositi-mex-0.0.5.dev0/tests/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/tests/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/tests/http/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/tests/http/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-31 19:52:53.000000 aiositi-mex-0.0.5.dev0/tests/test_utils.py
```

### Comparing `aiositi-mex-0.0.4/PKG-INFO` & `aiositi-mex-0.0.5.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiositi-mex
-Version: 0.0.4
+Version: 0.0.5.dev0
 Summary: Cliente para enviar reportes a la CNBV.
 Home-page: https://github.com/cuenca-mx/siti-python
 Author: Cuenca
 Author-email: dev@cuenca.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `aiositi-mex-0.0.4/README.md` & `aiositi-mex-0.0.5.dev0/README.md`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/aiositi_mex.egg-info/PKG-INFO` & `aiositi-mex-0.0.5.dev0/aiositi_mex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiositi-mex
-Version: 0.0.4
+Version: 0.0.5.dev0
 Summary: Cliente para enviar reportes a la CNBV.
 Home-page: https://github.com/cuenca-mx/siti-python
 Author: Cuenca
 Author-email: dev@cuenca.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `aiositi-mex-0.0.4/aiositi_mex.egg-info/SOURCES.txt` & `aiositi-mex-0.0.5.dev0/aiositi_mex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/setup.py` & `aiositi-mex-0.0.5.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/exc.py` & `aiositi-mex-0.0.5.dev0/siti/exc.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/http/client.py` & `aiositi-mex-0.0.5.dev0/siti/http/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         async with aiohttp.ClientSession(
             connector=conn, headers=headers
         ) as session:
             async with session.request(
                 method,
                 url,
                 json=data,
+                verify=False,
                 **kwargs,
             ) as response:
                 resultado = await response.json()
                 await self._check_response(response)
         return resultado
 
     @classmethod
```

### Comparing `aiositi-mex-0.0.4/siti/http/oauth_token.py` & `aiositi-mex-0.0.5.dev0/siti/http/oauth_token.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/base.py` & `aiositi-mex-0.0.5.dev0/siti/resources/base.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/__init__.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/__init__.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/base.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/base.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/catalogos.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/catalogos.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/r01/reporte_111.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r01/reporte_111.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/r08/reporte_843.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r08/reporte_843.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/r10/reporte_10111.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r10/reporte_10111.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/r10/reporte_10121.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r10/reporte_10121.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/r13/reporte_13111.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r13/reporte_13111.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/r13/reporte_13161.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r13/reporte_13161.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/r13/reporte_13211.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r13/reporte_13211.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/r13/reporte_13221.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r13/reporte_13221.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/r24/reporte_2471.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r24/reporte_2471.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/r24/reporte_2472.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r24/reporte_2472.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/r26/reporte_2610.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r26/reporte_2610.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/r26/reporte_2611.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r26/reporte_2611.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/r26/reporte_2612.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r26/reporte_2612.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/r26/reporte_2613.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r26/reporte_2613.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/r27/reporte_2701.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r27/reporte_2701.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/r36/reporte_3611.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r36/reporte_3611.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/r36/reporte_3612.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r36/reporte_3612.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/r36/reporte_3613.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/r36/reporte_3613.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/reportes.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/reportes.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/resources/ifpe/types.py` & `aiositi-mex-0.0.5.dev0/siti/resources/ifpe/types.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/siti/utils.py` & `aiositi-mex-0.0.5.dev0/siti/utils.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/tests/http/test_client.py` & `aiositi-mex-0.0.5.dev0/tests/http/test_client.py`

 * *Files identical despite different names*

### Comparing `aiositi-mex-0.0.4/tests/test_utils.py` & `aiositi-mex-0.0.5.dev0/tests/test_utils.py`

 * *Files identical despite different names*

