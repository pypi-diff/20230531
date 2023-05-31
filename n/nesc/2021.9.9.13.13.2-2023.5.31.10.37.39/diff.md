# Comparing `tmp/nesc-2021.9.9.13.13.2.tar.gz` & `tmp/nesc-2023.5.31.10.37.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nesc-2021.9.9.13.13.2.tar", last modified: Thu Sep  9 05:13:07 2021, max compression
+gzip compressed data, was "nesc-2023.5.31.10.37.39.tar", last modified: Wed May 31 02:37:40 2023, max compression
```

## Comparing `nesc-2021.9.9.13.13.2.tar` & `nesc-2023.5.31.10.37.39.tar`

### file list

```diff
@@ -1,59 +1,129 @@
-drwxr-xr-x   0 yuanjie    (501) staff       (20)        0 2021-09-09 05:13:07.000000 nesc-2021.9.9.13.13.2/
--rw-r--r--   0 yuanjie    (501) staff       (20)      153 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/AUTHORS.rst
--rw-r--r--   0 yuanjie    (501) staff       (20)     3488 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/CONTRIBUTING.rst
--rw-r--r--   0 yuanjie    (501) staff       (20)       89 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/HISTORY.rst
--rw-r--r--   0 yuanjie    (501) staff       (20)     1067 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/LICENSE
--rw-r--r--   0 yuanjie    (501) staff       (20)      319 2021-09-09 04:33:27.000000 nesc-2021.9.9.13.13.2/MANIFEST.in
--rw-r--r--   0 yuanjie    (501) staff       (20)     1117 2021-09-09 05:13:07.000000 nesc-2021.9.9.13.13.2/PKG-INFO
--rw-r--r--   0 yuanjie    (501) staff       (20)      302 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/README.md
--rw-r--r--   0 yuanjie    (501) staff       (20)      797 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/README.rst
-drwxr-xr-x   0 yuanjie    (501) staff       (20)        0 2021-09-09 05:13:07.000000 nesc-2021.9.9.13.13.2/docs/
--rw-r--r--   0 yuanjie    (501) staff       (20)      605 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/docs/Makefile
--rw-r--r--   0 yuanjie    (501) staff       (20)       28 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/docs/authors.rst
--rwxr-xr-x   0 yuanjie    (501) staff       (20)     4727 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/docs/conf.py
--rw-r--r--   0 yuanjie    (501) staff       (20)       33 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/docs/contributing.rst
--rw-r--r--   0 yuanjie    (501) staff       (20)       28 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/docs/history.rst
--rw-r--r--   0 yuanjie    (501) staff       (20)      301 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/docs/index.rst
--rw-r--r--   0 yuanjie    (501) staff       (20)     1090 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/docs/installation.rst
--rw-r--r--   0 yuanjie    (501) staff       (20)      766 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/docs/make.bat
--rw-r--r--   0 yuanjie    (501) staff       (20)       27 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/docs/readme.rst
--rw-r--r--   0 yuanjie    (501) staff       (20)       63 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/docs/usage.rst
-drwxr-xr-x   0 yuanjie    (501) staff       (20)        0 2021-09-09 05:13:07.000000 nesc-2021.9.9.13.13.2/nesc/
--rw-r--r--   0 yuanjie    (501) staff       (20)      119 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/nesc/__init__.py
-drwxr-xr-x   0 yuanjie    (501) staff       (20)        0 2021-09-09 05:13:07.000000 nesc-2021.9.9.13.13.2/nesc/ai/
--rw-r--r--   0 yuanjie    (501) staff       (20)      238 2021-09-04 09:27:53.000000 nesc-2021.9.9.13.13.2/nesc/ai/__init__.py
-drwxr-xr-x   0 yuanjie    (501) staff       (20)        0 2021-09-09 05:13:07.000000 nesc-2021.9.9.13.13.2/nesc/clis/
--rw-r--r--   0 yuanjie    (501) staff       (20)      413 2021-08-31 05:12:27.000000 nesc-2021.9.9.13.13.2/nesc/clis/README.md
--rw-r--r--   0 yuanjie    (501) staff       (20)      283 2021-09-03 03:28:26.000000 nesc-2021.9.9.13.13.2/nesc/clis/__init__.py
--rw-r--r--   0 yuanjie    (501) staff       (20)     2094 2021-09-08 02:51:15.000000 nesc-2021.9.9.13.13.2/nesc/clis/cli.py
--rw-r--r--   0 yuanjie    (501) staff       (20)      739 2021-09-09 02:32:48.000000 nesc-2021.9.9.13.13.2/nesc/clis/gui.py
-drwxr-xr-x   0 yuanjie    (501) staff       (20)        0 2021-09-09 05:13:07.000000 nesc-2021.9.9.13.13.2/nesc/clis/guis/
--rw-r--r--   0 yuanjie    (501) staff       (20)      239 2021-09-09 02:34:08.000000 nesc-2021.9.9.13.13.2/nesc/clis/guis/__init__.py
--rw-r--r--   0 yuanjie    (501) staff       (20)    27503 2021-09-09 04:50:10.000000 nesc-2021.9.9.13.13.2/nesc/clis/guis/demo.jpg
--rw-r--r--   0 yuanjie    (501) staff       (20)     1531 2021-09-09 05:03:03.000000 nesc-2021.9.9.13.13.2/nesc/clis/guis/ocr.py
--rw-r--r--   0 yuanjie    (501) staff       (20)    11306 2021-09-09 04:21:24.000000 nesc-2021.9.9.13.13.2/nesc/clis/guis/program_icon.png
--rw-r--r--   0 yuanjie    (501) staff       (20)     1070 2021-09-09 03:55:39.000000 nesc-2021.9.9.13.13.2/nesc/clis/guis/seg.py
--rw-r--r--   0 yuanjie    (501) staff       (20)    16573 2021-09-09 05:04:14.000000 nesc-2021.9.9.13.13.2/nesc/clis/guis/test.png
-drwxr-xr-x   0 yuanjie    (501) staff       (20)        0 2021-09-09 05:13:07.000000 nesc-2021.9.9.13.13.2/nesc/extract/
--rw-r--r--   0 yuanjie    (501) staff       (20)      238 2021-09-04 09:28:08.000000 nesc-2021.9.9.13.13.2/nesc/extract/__init__.py
--rw-r--r--   0 yuanjie    (501) staff       (20)     1811 2021-09-07 00:47:58.000000 nesc-2021.9.9.13.13.2/nesc/extract/extract4ddl.py
--rw-r--r--   0 yuanjie    (501) staff       (20)     2716 2021-09-06 06:44:02.000000 nesc-2021.9.9.13.13.2/nesc/extract/extract4excel.py
--rw-r--r--   0 yuanjie    (501) staff       (20)     2849 2021-09-06 06:40:06.000000 nesc-2021.9.9.13.13.2/nesc/extract/hs.py
--rw-r--r--   0 yuanjie    (501) staff       (20)       19 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/nesc/nesc.py
-drwxr-xr-x   0 yuanjie    (501) staff       (20)        0 2021-09-09 05:13:07.000000 nesc-2021.9.9.13.13.2/nesc/sim/
--rw-r--r--   0 yuanjie    (501) staff       (20)      238 2021-09-06 09:41:10.000000 nesc-2021.9.9.13.13.2/nesc/sim/__init__.py
--rw-r--r--   0 yuanjie    (501) staff       (20)     2989 2021-09-07 07:46:51.000000 nesc-2021.9.9.13.13.2/nesc/sim/sim.py
--rw-r--r--   0 yuanjie    (501) staff       (20)     2807 2021-09-08 02:48:47.000000 nesc-2021.9.9.13.13.2/nesc/sim/simv2.py
-drwxr-xr-x   0 yuanjie    (501) staff       (20)        0 2021-09-09 05:13:07.000000 nesc-2021.9.9.13.13.2/nesc.egg-info/
--rw-r--r--   0 yuanjie    (501) staff       (20)     1117 2021-09-09 05:13:02.000000 nesc-2021.9.9.13.13.2/nesc.egg-info/PKG-INFO
--rw-r--r--   0 yuanjie    (501) staff       (20)      933 2021-09-09 05:13:02.000000 nesc-2021.9.9.13.13.2/nesc.egg-info/SOURCES.txt
--rw-r--r--   0 yuanjie    (501) staff       (20)        1 2021-09-09 05:13:02.000000 nesc-2021.9.9.13.13.2/nesc.egg-info/dependency_links.txt
--rw-r--r--   0 yuanjie    (501) staff       (20)      143 2021-09-09 05:13:02.000000 nesc-2021.9.9.13.13.2/nesc.egg-info/entry_points.txt
--rw-r--r--   0 yuanjie    (501) staff       (20)        1 2021-09-09 05:13:02.000000 nesc-2021.9.9.13.13.2/nesc.egg-info/not-zip-safe
--rw-r--r--   0 yuanjie    (501) staff       (20)       28 2021-09-09 05:13:02.000000 nesc-2021.9.9.13.13.2/nesc.egg-info/requires.txt
--rw-r--r--   0 yuanjie    (501) staff       (20)        5 2021-09-09 05:13:02.000000 nesc-2021.9.9.13.13.2/nesc.egg-info/top_level.txt
--rw-r--r--   0 yuanjie    (501) staff       (20)      387 2021-09-09 05:13:07.000000 nesc-2021.9.9.13.13.2/setup.cfg
--rw-r--r--   0 yuanjie    (501) staff       (20)     1594 2021-09-09 04:43:44.000000 nesc-2021.9.9.13.13.2/setup.py
-drwxr-xr-x   0 yuanjie    (501) staff       (20)        0 2021-09-09 05:13:07.000000 nesc-2021.9.9.13.13.2/tests/
--rw-r--r--   0 yuanjie    (501) staff       (20)       34 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/tests/__init__.py
--rw-r--r--   0 yuanjie    (501) staff       (20)      831 2021-09-04 09:22:43.000000 nesc-2021.9.9.13.13.2/tests/test_nesc.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.146785 nesc-2023.5.31.10.37.39/
+-rw-r--r--   0 betterme   (501) staff       (20)      153 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3488 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1067 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      319 2021-09-09 04:33:27.000000 nesc-2023.5.31.10.37.39/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     1518 2023-05-31 02:37:40.146878 nesc-2023.5.31.10.37.39/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      721 2021-09-09 09:24:36.000000 nesc-2023.5.31.10.37.39/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      797 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.132813 nesc-2023.5.31.10.37.39/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      605 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4727 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      301 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1090 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      766 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       63 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/docs/usage.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.133181 nesc-2023.5.31.10.37.39/nesc/
+-rw-r--r--   0 betterme   (501) staff       (20)      119 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/nesc/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.134578 nesc-2023.5.31.10.37.39/nesc/ai/
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2021-09-04 09:27:53.000000 nesc-2023.5.31.10.37.39/nesc/ai/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      326 2021-09-13 05:33:59.000000 nesc-2023.5.31.10.37.39/nesc/ai/seg.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.135255 nesc-2023.5.31.10.37.39/nesc/apps_fastapi/
+-rw-r--r--   0 betterme   (501) staff       (20)      240 2021-10-25 03:26:31.000000 nesc-2023.5.31.10.37.39/nesc/apps_fastapi/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      617 2021-10-25 03:26:31.000000 nesc-2023.5.31.10.37.39/nesc/apps_fastapi/simapp.py
+-rw-r--r--   0 betterme   (501) staff       (20)      259 2021-10-25 03:26:31.000000 nesc-2023.5.31.10.37.39/nesc/apps_fastapi/st_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.136014 nesc-2023.5.31.10.37.39/nesc/apps_streamlit/
+-rw-r--r--   0 betterme   (501) staff       (20)      240 2021-10-25 03:26:31.000000 nesc-2023.5.31.10.37.39/nesc/apps_streamlit/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5764 2021-11-12 07:02:19.000000 nesc-2023.5.31.10.37.39/nesc/apps_streamlit/_appzoo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1068 2021-11-12 09:15:16.000000 nesc-2023.5.31.10.37.39/nesc/apps_streamlit/ai_app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5058 2021-11-12 09:29:03.000000 nesc-2023.5.31.10.37.39/nesc/apps_streamlit/apps.py
+-rw-r--r--   0 betterme   (501) staff       (20)      471 2023-03-30 07:22:35.000000 nesc-2023.5.31.10.37.39/nesc/apps_streamlit/demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.136717 nesc-2023.5.31.10.37.39/nesc/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 nesc-2023.5.31.10.37.39/nesc/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      283 2021-09-03 03:28:26.000000 nesc-2023.5.31.10.37.39/nesc/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2612 2021-10-25 03:26:31.000000 nesc-2023.5.31.10.37.39/nesc/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)      739 2021-09-09 02:32:48.000000 nesc-2023.5.31.10.37.39/nesc/clis/gui.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.137628 nesc-2023.5.31.10.37.39/nesc/clis/guis/
+-rw-r--r--   0 betterme   (501) staff       (20)      239 2021-09-09 02:34:08.000000 nesc-2023.5.31.10.37.39/nesc/clis/guis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1407 2021-09-09 06:32:36.000000 nesc-2023.5.31.10.37.39/nesc/clis/guis/ocr.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11306 2021-09-09 04:21:24.000000 nesc-2023.5.31.10.37.39/nesc/clis/guis/program_icon.png
+-rw-r--r--   0 betterme   (501) staff       (20)     1068 2021-09-09 06:32:36.000000 nesc-2023.5.31.10.37.39/nesc/clis/guis/seg.py
+-rw-r--r--   0 betterme   (501) staff       (20)    16573 2021-09-09 05:04:14.000000 nesc-2023.5.31.10.37.39/nesc/clis/guis/test.png
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.138883 nesc-2023.5.31.10.37.39/nesc/crawler/
+-rw-r--r--   0 betterme   (501) staff       (20)     7214 2021-11-03 09:17:33.000000 nesc-2023.5.31.10.37.39/nesc/crawler/WorkBetter(1).py
+-rw-r--r--   0 betterme   (501) staff       (20)     4830 2021-11-03 06:19:56.000000 nesc-2023.5.31.10.37.39/nesc/crawler/WorkBetter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7662 2021-11-04 01:04:48.000000 nesc-2023.5.31.10.37.39/nesc/crawler/WorkBetter22.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5526 2021-11-03 06:06:44.000000 nesc-2023.5.31.10.37.39/nesc/crawler/WorkMe.py
+-rw-r--r--   0 betterme   (501) staff       (20)      239 2021-11-03 06:07:32.000000 nesc-2023.5.31.10.37.39/nesc/crawler/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      255 2021-11-03 08:31:13.000000 nesc-2023.5.31.10.37.39/nesc/crawler/demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.139059 nesc-2023.5.31.10.37.39/nesc/dockerfiles/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2021-10-25 03:26:31.000000 nesc-2023.5.31.10.37.39/nesc/dockerfiles/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.139213 nesc-2023.5.31.10.37.39/nesc/easydata/
+-rw-r--r--   0 betterme   (501) staff       (20)       22 2021-10-21 09:44:11.000000 nesc-2023.5.31.10.37.39/nesc/easydata/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.139561 nesc-2023.5.31.10.37.39/nesc/easydata/dask/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2021-10-21 09:44:11.000000 nesc-2023.5.31.10.37.39/nesc/easydata/dask/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3722 2021-10-21 09:44:11.000000 nesc-2023.5.31.10.37.39/nesc/easydata/dask/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.140478 nesc-2023.5.31.10.37.39/nesc/easydata/hive/
+-rw-r--r--   0 betterme   (501) staff       (20)       70 2021-11-17 03:25:13.000000 nesc-2023.5.31.10.37.39/nesc/easydata/hive/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    21873 2021-11-17 03:25:13.000000 nesc-2023.5.31.10.37.39/nesc/easydata/hive/hive.py
+-rw-r--r--   0 betterme   (501) staff       (20)      882 2021-10-21 09:44:11.000000 nesc-2023.5.31.10.37.39/nesc/easydata/hive/logger.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.141387 nesc-2023.5.31.10.37.39/nesc/easydata/hive/parsers/
+-rw-r--r--   0 betterme   (501) staff       (20)      231 2021-11-17 03:25:13.000000 nesc-2023.5.31.10.37.39/nesc/easydata/hive/parsers/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      354 2021-10-21 09:44:11.000000 nesc-2023.5.31.10.37.39/nesc/easydata/hive/parsers/base_parser.py
+-rw-r--r--   0 betterme   (501) staff       (20)      296 2021-10-21 09:44:11.000000 nesc-2023.5.31.10.37.39/nesc/easydata/hive/parsers/orc.py
+-rw-r--r--   0 betterme   (501) staff       (20)      293 2021-11-17 03:25:13.000000 nesc-2023.5.31.10.37.39/nesc/easydata/hive/parsers/parquet.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2778 2021-11-17 03:25:13.000000 nesc-2023.5.31.10.37.39/nesc/easydata/hive/parsers/text.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7600 2021-10-21 09:44:11.000000 nesc-2023.5.31.10.37.39/nesc/easydata/hive/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.142033 nesc-2023.5.31.10.37.39/nesc/extract/
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2021-09-04 09:28:08.000000 nesc-2023.5.31.10.37.39/nesc/extract/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2177 2021-09-11 12:01:49.000000 nesc-2023.5.31.10.37.39/nesc/extract/extract4ddl.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2771 2022-12-01 00:58:52.000000 nesc-2023.5.31.10.37.39/nesc/extract/extract4excel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2849 2021-09-06 06:40:06.000000 nesc-2023.5.31.10.37.39/nesc/extract/hs.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.142593 nesc-2023.5.31.10.37.39/nesc/gpus/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2021-10-25 03:26:24.000000 nesc-2023.5.31.10.37.39/nesc/gpus/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1287 2021-10-25 03:26:24.000000 nesc-2023.5.31.10.37.39/nesc/gpus/catboost_gpu.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2725 2021-10-25 03:26:24.000000 nesc-2023.5.31.10.37.39/nesc/gpus/tf_gpu.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1181 2021-10-25 03:28:28.000000 nesc-2023.5.31.10.37.39/nesc/gpus/xgboost_gpu.py
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/nesc/nesc.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.143573 nesc-2023.5.31.10.37.39/nesc/nescqdata/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.143905 nesc-2023.5.31.10.37.39/nesc/nescqdata/BondData/
+-rw-r--r--   0 betterme   (501) staff       (20)       40 2022-04-18 10:17:45.000000 nesc-2023.5.31.10.37.39/nesc/nescqdata/BondData/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      182 2022-04-18 10:17:45.000000 nesc-2023.5.31.10.37.39/nesc/nescqdata/BondData/dataProvider.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.144219 nesc-2023.5.31.10.37.39/nesc/nescqdata/FundData/
+-rw-r--r--   0 betterme   (501) staff       (20)       40 2022-04-18 10:17:45.000000 nesc-2023.5.31.10.37.39/nesc/nescqdata/FundData/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      182 2022-04-18 10:17:45.000000 nesc-2023.5.31.10.37.39/nesc/nescqdata/FundData/dataProvider.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.144376 nesc-2023.5.31.10.37.39/nesc/nescqdata/FutureData/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2022-04-18 10:17:45.000000 nesc-2023.5.31.10.37.39/nesc/nescqdata/FutureData/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.144650 nesc-2023.5.31.10.37.39/nesc/nescqdata/MarketData/
+-rw-r--r--   0 betterme   (501) staff       (20)       40 2022-04-18 10:17:45.000000 nesc-2023.5.31.10.37.39/nesc/nescqdata/MarketData/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1362 2022-04-18 10:17:45.000000 nesc-2023.5.31.10.37.39/nesc/nescqdata/MarketData/dataProvider.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.144959 nesc-2023.5.31.10.37.39/nesc/nescqdata/OptionData/
+-rw-r--r--   0 betterme   (501) staff       (20)       40 2022-04-18 10:17:45.000000 nesc-2023.5.31.10.37.39/nesc/nescqdata/OptionData/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      184 2022-04-18 10:17:45.000000 nesc-2023.5.31.10.37.39/nesc/nescqdata/OptionData/dataProvider.py
+-rw-r--r--   0 betterme   (501) staff       (20)      211 2022-04-18 10:17:45.000000 nesc-2023.5.31.10.37.39/nesc/nescqdata/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      147 2022-04-18 10:17:45.000000 nesc-2023.5.31.10.37.39/nesc/nescqdata/_version.py
+-rw-r--r--   0 betterme   (501) staff       (20)    16665 2022-04-18 10:17:45.000000 nesc-2023.5.31.10.37.39/nesc/nescqdata/baseDataProvider.py
+-rw-r--r--   0 betterme   (501) staff       (20)    16755 2022-04-18 10:17:45.000000 nesc-2023.5.31.10.37.39/nesc/nescqdata/columnsMap.py
+-rw-r--r--   0 betterme   (501) staff       (20)      658 2022-04-18 10:17:45.000000 nesc-2023.5.31.10.37.39/nesc/nescqdata/selfException.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5092 2022-04-18 10:17:45.000000 nesc-2023.5.31.10.37.39/nesc/nescqdata/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.145564 nesc-2023.5.31.10.37.39/nesc/sim/
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2021-09-06 09:41:10.000000 nesc-2023.5.31.10.37.39/nesc/sim/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2505 2021-09-15 09:23:18.000000 nesc-2023.5.31.10.37.39/nesc/sim/sim.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2989 2021-09-07 07:46:51.000000 nesc-2023.5.31.10.37.39/nesc/sim/sim_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2772 2021-10-25 03:26:24.000000 nesc-2023.5.31.10.37.39/nesc/sim/simv2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.146086 nesc-2023.5.31.10.37.39/nesc/utils/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2021-10-25 03:26:24.000000 nesc-2023.5.31.10.37.39/nesc/utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1085 2021-10-25 03:26:24.000000 nesc-2023.5.31.10.37.39/nesc/utils/db_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      120 2021-10-25 03:26:24.000000 nesc-2023.5.31.10.37.39/nesc/utils/hdfs_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      745 2021-10-25 03:26:24.000000 nesc-2023.5.31.10.37.39/nesc/utils/s3_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.146368 nesc-2023.5.31.10.37.39/nesc/word_root/
+-rw-r--r--   0 betterme   (501) staff       (20)      239 2021-09-13 05:35:49.000000 nesc-2023.5.31.10.37.39/nesc/word_root/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      232 2021-09-13 05:35:57.000000 nesc-2023.5.31.10.37.39/nesc/word_root/demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.134298 nesc-2023.5.31.10.37.39/nesc.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     1518 2023-05-31 02:37:40.000000 nesc-2023.5.31.10.37.39/nesc.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     2511 2023-05-31 02:37:40.000000 nesc-2023.5.31.10.37.39/nesc.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-31 02:37:40.000000 nesc-2023.5.31.10.37.39/nesc.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      142 2023-05-31 02:37:40.000000 nesc-2023.5.31.10.37.39/nesc.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-31 02:37:40.000000 nesc-2023.5.31.10.37.39/nesc.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       12 2023-05-31 02:37:40.000000 nesc-2023.5.31.10.37.39/nesc.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        5 2023-05-31 02:37:40.000000 nesc-2023.5.31.10.37.39/nesc.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      387 2023-05-31 02:37:40.147162 nesc-2023.5.31.10.37.39/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1596 2021-10-25 03:26:31.000000 nesc-2023.5.31.10.37.39/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-31 02:37:40.146649 nesc-2023.5.31.10.37.39/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       34 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      831 2021-09-04 09:22:43.000000 nesc-2023.5.31.10.37.39/tests/test_nesc.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nesc-2021.9.9.13.13.2/CONTRIBUTING.rst` & `nesc-2023.5.31.10.37.39/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nesc-2021.9.9.13.13.2/LICENSE` & `nesc-2023.5.31.10.37.39/LICENSE`

 * *Files identical despite different names*

### Comparing `nesc-2021.9.9.13.13.2/README.rst` & `nesc-2023.5.31.10.37.39/README.rst`

 * *Files identical despite different names*

### Comparing `nesc-2021.9.9.13.13.2/docs/Makefile` & `nesc-2023.5.31.10.37.39/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nesc-2021.9.9.13.13.2/docs/conf.py` & `nesc-2023.5.31.10.37.39/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nesc-2021.9.9.13.13.2/docs/installation.rst` & `nesc-2023.5.31.10.37.39/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `nesc-2021.9.9.13.13.2/docs/make.bat` & `nesc-2023.5.31.10.37.39/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nesc-2021.9.9.13.13.2/nesc/clis/cli.py` & `nesc-2023.5.31.10.37.39/nesc/clis/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -32,30 +32,20 @@
     p = Path(path)
     typer.echo(f"{p}")
     typer.echo(f"{p.absolute()}")
 
 
 @cli.command()
 @args
-def extract4ddl(ipath: str, opath=None, encoding='GB18030'):
+def extract4ddl(ipath: str, opath=None, encoding='GB18030', start_str='create table', end_str=')'):
     """解析ddl
     nesc extract4ddl '/Users/yuanjie/Desktop/notebook/0_TODO/mot_part.sql'
     """
     from nesc.extract import extract4ddl
-    extract4ddl.main(ipath, opath, encoding=encoding)
-
-
-@cli.command()
-@args
-def extract4excel(ipath: str, opath=None):
-    """解析excel
-    nesc extract4excel xx
-    """
-    from nesc.extract import extract4excel
-    extract4excel.main(ipath, opath)
+    extract4ddl.main(ipath, opath, encoding=encoding, start_str=start_str, end_str=end_str)
 
 
 @cli.command()
 @args
 def extract4excel(ipath: str, opath=None):
     """解析excel
     nesc extract4excel xx
@@ -80,9 +70,32 @@
     """相似文本匹配
     nesc text-match-v2 '手机号' '标准字段.txt'
     """
     from nesc.sim import simv2
     simv2.main(target, file, topn, batch_size, model_home)
 
 
+def _run_cmd(cmd, nohup=0):
+    cmd = f"nohup {cmd} &" if nohup else cmd
+    logger.debug(cmd)
+    return os.system(cmd)
+
+
+@cli.command()
+@args
+def run(app_file: str, app='fastapi', port=9993, nohup=0):
+    """Support fastapi/streamlit/gradio/gui app."""
+    if not Path(app_file).exists():
+        app_file = Path(get_module_path(f'../apps_{app}', __file__)) / app_file
+
+    if app in ('fastapi', 'gui', 'gradio'):
+        cmd = f"python {app_file}"
+    elif app == 'streamlit':
+        cmd = f"streamlit run {app_file} --server.baseUrlPath web --server.port {port}"
+    else:
+        cmd = "echo 无app可用"
+
+    _run_cmd(cmd, nohup)
+
+
 if __name__ == '__main__':
     cli()
```

### Comparing `nesc-2021.9.9.13.13.2/nesc/clis/gui.py` & `nesc-2023.5.31.10.37.39/nesc/clis/gui.py`

 * *Files identical despite different names*

### Comparing `nesc-2021.9.9.13.13.2/nesc/clis/guis/ocr.py` & `nesc-2023.5.31.10.37.39/nesc/clis/guis/ocr.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,16 @@
 # https://www.cnblogs.com/brt2/p/13232367.html
 
 from pprint import pprint
 from meutils.pipe import *
 from paddleocr import PaddleOCR
 from gooey import Gooey, GooeyParser
 
-# from PIL import Image, ImageGrab
-#
-# try:
-#     im = ImageGrab.grabclipboard()
-#     im.save("./默认读取截图")
-# except:
-#     pass
 
-ocr = PaddleOCR(use_angle_cls=True, lang="ch", use_gpu=False)
+ocr = PaddleOCR(use_angle_cls=True, lang="ch", use_gpu=False, show_log=False)
 
 
 @Gooey(
     program_name='东北证券 - 工具箱',
     language='chinese',
     clear_before_run=True,
     image_dir=get_module_path('.', __file__),
```

### Comparing `nesc-2021.9.9.13.13.2/nesc/clis/guis/program_icon.png` & `nesc-2023.5.31.10.37.39/nesc/clis/guis/program_icon.png`

 * *Files identical despite different names*

### Comparing `nesc-2021.9.9.13.13.2/nesc/clis/guis/seg.py` & `nesc-2023.5.31.10.37.39/nesc/clis/guis/seg.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,15 @@
     parser.add_argument('text', metavar='文本', default='东北证券是一家牛逼的公司', widget="TextField")  # 文件选择框
 
     # parser.add_argument('文件名', widget="FileChooser")  # 文件选择框
     # parser.add_argument('Date', widget="DateChooser")  # 日期选择框
     args = parser.parse_args()  # 接收界面传递的参数
     print('\n')
 
-
     print(lac.run(args.text))
 
-
     print(args.__dict__)
     print(time.ctime())
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `nesc-2021.9.9.13.13.2/nesc/clis/guis/test.png` & `nesc-2023.5.31.10.37.39/nesc/clis/guis/test.png`

 * *Files identical despite different names*

### Comparing `nesc-2021.9.9.13.13.2/nesc/extract/extract4excel.py` & `nesc-2023.5.31.10.37.39/nesc/extract/extract4excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,8 +87,10 @@
 
     logger.info(f"结果文件: {opath}")
 
     logger.info(bjson(dict(zip(df_all.nunique().index, df_all.nunique()))))
 
 
 if __name__ == '__main__':
-    main("/Users/yuanjie/Downloads/UF20表结构/UF20表结构/UF20表信息.xls")
+    # main("/Users/yuanjie/Downloads/UF20表结构/UF20表结构/UF20表信息.xls")
+    main("UF2.0(包含机构柜台)-表结构.xls")
+
```

### Comparing `nesc-2021.9.9.13.13.2/nesc/extract/hs.py` & `nesc-2023.5.31.10.37.39/nesc/extract/hs.py`

 * *Files identical despite different names*

### Comparing `nesc-2021.9.9.13.13.2/nesc/sim/sim.py` & `nesc-2023.5.31.10.37.39/nesc/sim/sim_.py`

 * *Files identical despite different names*

### Comparing `nesc-2021.9.9.13.13.2/nesc/sim/simv2.py` & `nesc-2023.5.31.10.37.39/nesc/sim/simv2.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from meutils.pipe import *
 
 from meutils.log_utils import logger4wecom
 from meutils.decorators.catch import wecom_catch, wecom_hook
 from meutils.annzoo.ann_faiss import ANN
 
 from bertzoo.simbert2vec import Simbert2vec
-from gensim.models import KeyedVectors
 
 tqdm.pandas()
 
 CACHE = 'cache.pkl'
 
 
 def get_vector_cache(backup=False):
@@ -77,18 +76,16 @@
         i2s = dict(zip(*_[::-1]))
 
         w2s = [(i2w_2.get(i), s) for i, s in i2s.items() if i != -1]
 
         df = pd.DataFrame(w2s)
         df.insert(0, 'target', i2w_1.get(idx))
         dfs.append(df)
-        break
-
-    return pd.concat(dfs)
 
+    return pd.concat(dfs, ignore_index=True)
 
 def main(target, file, topn=10, batch_size=512, model_home='chinese_roformer-sim-char-ft_L-6_H-384_A-6'):
     s1 = get_word_set(target)
     s2 = get_word_set(file)
 
     w2v = bert_vector(s1, s2, batch_size, model_home)
```

### Comparing `nesc-2021.9.9.13.13.2/setup.py` & `nesc-2023.5.31.10.37.39/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,17 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     description="ai for nesc",
     entry_points={
         'console_scripts': [
             'nesc=nesc.clis.cli:cli',
+
             'nesc-cli=nesc.clis.cli:cli',
+
             'nesc-seg=nesc.clis.guis.seg:main',
             'nesc-ocr=nesc.clis.guis.ocr:main',
 
         ],
     },
     install_requires=requirements,
     license="MIT license",
```

### Comparing `nesc-2021.9.9.13.13.2/tests/test_nesc.py` & `nesc-2023.5.31.10.37.39/tests/test_nesc.py`

 * *Files identical despite different names*

