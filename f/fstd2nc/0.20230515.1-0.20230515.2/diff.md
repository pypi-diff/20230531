# Comparing `tmp/fstd2nc-0.20230515.1.tar.gz` & `tmp/fstd2nc-0.20230515.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fstd2nc-0.20230515.1.tar", last modified: Thu May 25 22:34:38 2023, max compression
+gzip compressed data, was "dist/fstd2nc-0.20230515.2.tar", last modified: Wed May 31 00:14:21 2023, max compression
```

## Comparing `fstd2nc-0.20230515.1.tar` & `fstd2nc-0.20230515.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-25 22:34:38.684986 fstd2nc-0.20230515.1/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    35147 2022-04-13 02:52:23.000000 fstd2nc-0.20230515.1/COPYING
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7651 2022-04-13 02:52:23.000000 fstd2nc-0.20230515.1/COPYING.LESSER
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13943 2023-05-25 22:34:38.684718 fstd2nc-0.20230515.1/PKG-INFO
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13196 2023-02-22 19:45:21.000000 fstd2nc-0.20230515.1/README.md
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-25 22:34:38.672565 fstd2nc-0.20230515.1/cccbuffer/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      777 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      182 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/__main__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      149 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/cccdump.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-25 22:34:38.675480 fstd2nc-0.20230515.1/cccbuffer/mixins/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/mixins/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3910 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/mixins/ccc.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1193 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/mixins/char.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2289 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/mixins/grid.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4359 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/mixins/levels.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3047 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/mixins/superlabels.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6112 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/cccbuffer/mixins/times.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-25 22:34:38.676904 fstd2nc-0.20230515.1/fstd2nc/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3743 2023-05-25 22:20:27.000000 fstd2nc-0.20230515.1/fstd2nc/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     9892 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/__main__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14256 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/extra.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-25 22:34:38.610655 fstd2nc-0.20230515.1/fstd2nc/locale/
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-25 22:34:38.610728 fstd2nc-0.20230515.1/fstd2nc/locale/fr_CA/
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-25 22:34:38.678906 fstd2nc-0.20230515.1/fstd2nc/locale/fr_CA/LC_MESSAGES/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    22410 2023-05-25 22:33:03.000000 fstd2nc-0.20230515.1/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-25 22:34:38.684293 fstd2nc-0.20230515.1/fstd2nc/mixins/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    35592 2023-05-25 22:20:27.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1871 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/ascii.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20216 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/compat.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     5787 2023-05-25 22:09:25.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/dates.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3138 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/diaghacks.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3130 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/ensembles.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    19526 2023-05-25 22:09:25.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/extern.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3565 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/filter.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     9126 2023-05-25 00:10:49.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/fstd.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    17534 2023-05-25 22:20:27.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/gridhacks.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7119 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/masks.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4210 2023-05-25 22:08:50.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/mesh.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1571 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/misc.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20811 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/netcdf.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1735 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/pruneaxes.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4790 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/removestuff.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2610 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/select.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14637 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/series.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6683 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/sfc_codes.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7339 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/vardict.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    32765 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/vcoords.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    37809 2023-05-25 22:09:25.000000 fstd2nc-0.20230515.1/fstd2nc/mixins/xycoords.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2583 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/fstd2nc/stdout.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-25 22:34:38.678620 fstd2nc-0.20230515.1/fstd2nc.egg-info/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13943 2023-05-25 22:34:38.677185 fstd2nc-0.20230515.1/fstd2nc.egg-info/PKG-INFO
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1183 2023-05-25 22:34:38.677367 fstd2nc-0.20230515.1/fstd2nc.egg-info/SOURCES.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        1 2023-05-25 22:34:38.677811 fstd2nc-0.20230515.1/fstd2nc.egg-info/dependency_links.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      170 2023-05-25 22:34:38.678211 fstd2nc-0.20230515.1/fstd2nc.egg-info/entry_points.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      218 2023-05-25 22:34:38.678440 fstd2nc-0.20230515.1/fstd2nc.egg-info/requires.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       18 2023-05-25 22:34:38.678661 fstd2nc-0.20230515.1/fstd2nc.egg-info/top_level.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       59 2022-12-28 20:25:42.000000 fstd2nc-0.20230515.1/pyproject.toml
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       38 2023-05-25 22:34:38.685044 fstd2nc-0.20230515.1/setup.cfg
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2514 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.1/setup.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-31 00:14:21.539096 fstd2nc-0.20230515.2/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    35147 2022-04-13 02:52:23.000000 fstd2nc-0.20230515.2/COPYING
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7651 2022-04-13 02:52:23.000000 fstd2nc-0.20230515.2/COPYING.LESSER
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13943 2023-05-31 00:14:21.538834 fstd2nc-0.20230515.2/PKG-INFO
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13196 2023-02-22 19:45:21.000000 fstd2nc-0.20230515.2/README.md
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-31 00:14:21.525969 fstd2nc-0.20230515.2/cccbuffer/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      777 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/cccbuffer/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      182 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/cccbuffer/__main__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      149 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/cccbuffer/cccdump.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-31 00:14:21.528653 fstd2nc-0.20230515.2/cccbuffer/mixins/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/cccbuffer/mixins/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3910 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/cccbuffer/mixins/ccc.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1193 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/cccbuffer/mixins/char.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2289 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/cccbuffer/mixins/grid.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4359 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/cccbuffer/mixins/levels.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3047 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/cccbuffer/mixins/superlabels.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6112 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/cccbuffer/mixins/times.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-31 00:14:21.530062 fstd2nc-0.20230515.2/fstd2nc/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3743 2023-05-30 22:04:03.000000 fstd2nc-0.20230515.2/fstd2nc/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     9892 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/fstd2nc/__main__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14256 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/fstd2nc/extra.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-31 00:14:21.522050 fstd2nc-0.20230515.2/fstd2nc/locale/
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-31 00:14:21.522161 fstd2nc-0.20230515.2/fstd2nc/locale/fr_CA/
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-31 00:14:21.531920 fstd2nc-0.20230515.2/fstd2nc/locale/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    22475 2023-05-31 00:13:36.000000 fstd2nc-0.20230515.2/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-31 00:14:21.538423 fstd2nc-0.20230515.2/fstd2nc/mixins/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    35592 2023-05-25 22:20:27.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1871 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/ascii.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20216 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/compat.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     5787 2023-05-25 22:09:25.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/dates.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3138 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/diaghacks.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3130 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/ensembles.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    19873 2023-05-30 22:04:03.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/extern.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3565 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/filter.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     9126 2023-05-25 00:10:49.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/fstd.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    17846 2023-05-30 22:04:03.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/gridhacks.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7119 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/masks.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4210 2023-05-25 22:08:50.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/mesh.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1571 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/misc.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20811 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/netcdf.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1735 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/pruneaxes.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4790 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/removestuff.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2610 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/select.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14637 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/series.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6683 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/sfc_codes.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7339 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/vardict.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    32765 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/vcoords.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    37809 2023-05-25 22:09:25.000000 fstd2nc-0.20230515.2/fstd2nc/mixins/xycoords.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2583 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/fstd2nc/stdout.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2023-05-31 00:14:21.531634 fstd2nc-0.20230515.2/fstd2nc.egg-info/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13943 2023-05-31 00:14:20.000000 fstd2nc-0.20230515.2/fstd2nc.egg-info/PKG-INFO
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1183 2023-05-31 00:14:21.530641 fstd2nc-0.20230515.2/fstd2nc.egg-info/SOURCES.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        1 2023-05-31 00:14:21.530918 fstd2nc-0.20230515.2/fstd2nc.egg-info/dependency_links.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      170 2023-05-31 00:14:21.531138 fstd2nc-0.20230515.2/fstd2nc.egg-info/entry_points.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      218 2023-05-31 00:14:21.531406 fstd2nc-0.20230515.2/fstd2nc.egg-info/requires.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       18 2023-05-31 00:14:21.531677 fstd2nc-0.20230515.2/fstd2nc.egg-info/top_level.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       59 2022-12-28 20:25:42.000000 fstd2nc-0.20230515.2/pyproject.toml
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       38 2023-05-31 00:14:21.539153 fstd2nc-0.20230515.2/setup.cfg
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2514 2023-05-23 17:45:39.000000 fstd2nc-0.20230515.2/setup.py
```

### Comparing `fstd2nc-0.20230515.1/COPYING` & `fstd2nc-0.20230515.2/COPYING`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/COPYING.LESSER` & `fstd2nc-0.20230515.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/PKG-INFO` & `fstd2nc-0.20230515.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstd2nc
-Version: 0.20230515.1
+Version: 0.20230515.2
 Summary: Converts RPN standard files (from Environment Canada) to netCDF files.
 Home-page: https://github.com/neishm/fstd2nc
 Author: Mike Neish
 License: LGPL-3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `fstd2nc-0.20230515.1/README.md` & `fstd2nc-0.20230515.2/README.md`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/cccbuffer/__init__.py` & `fstd2nc-0.20230515.2/cccbuffer/__init__.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/cccbuffer/mixins/ccc.py` & `fstd2nc-0.20230515.2/cccbuffer/mixins/ccc.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/cccbuffer/mixins/char.py` & `fstd2nc-0.20230515.2/cccbuffer/mixins/char.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/cccbuffer/mixins/grid.py` & `fstd2nc-0.20230515.2/cccbuffer/mixins/grid.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/cccbuffer/mixins/levels.py` & `fstd2nc-0.20230515.2/cccbuffer/mixins/levels.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/cccbuffer/mixins/superlabels.py` & `fstd2nc-0.20230515.2/cccbuffer/mixins/superlabels.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/cccbuffer/mixins/times.py` & `fstd2nc-0.20230515.2/cccbuffer/mixins/times.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/__init__.py` & `fstd2nc-0.20230515.2/fstd2nc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ###############################################################################
 
 
 """
 Functionality for converting between FSTD and netCDF files.
 """
 
-__version__ = "0.20230515.1"
+__version__ = "0.20230515.2"
 
 
 # Check for bundled rpnpy package.
 # Fall back to this one if no standard rpnpy package available.
 try:
   # Importing the module will set up the appropriate search paths.
   import fstd2nc_deps
```

### Comparing `fstd2nc-0.20230515.1/fstd2nc/__main__.py` & `fstd2nc-0.20230515.2/fstd2nc/__main__.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/extra.py` & `fstd2nc-0.20230515.2/fstd2nc/extra.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo` & `fstd2nc-0.20230515.2/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: fstd2nc\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-05-25 22:33+0000\n"
+"POT-Creation-Date: 2023-05-31 00:13+0000\n"
 "PO-Revision-Date: 2022-11-25 17:40+0000\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: fr_CA\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=ISO-8859-1\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -558,14 +558,17 @@
 
 msgid "an RPN standard file"
 msgstr "un fichier standard RPN"
 
 msgid "argument \"-\" with mode %r"
 msgstr "argument \"-\" avec le mode %r"
 
+msgid "can't open '%s': %s"
+msgstr "impossible d'ouvrir '%s': %s"
+
 msgid "cannot have multiple subparser arguments"
 msgstr "impossible d'avoir plusiers arguments de sous-analyseur"
 
 msgid "cannot merge actions - two groups are named %r"
 msgstr "impossible de fusionner les actions - deux groupes sont nommés %r"
 
 msgid "conflicting option string: %s"
```

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/__init__.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/ascii.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/ascii.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/compat.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/compat.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/dates.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/dates.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/diaghacks.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/diaghacks.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/ensembles.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/ensembles.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/extern.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/extern.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,21 +79,29 @@
   _FSTD_Callback().register()
 
 # Method for reading a block from a file.
 def _read_block (filename, offset, length):
   import numpy as np
   # Scalar version first.
   if not hasattr(offset,'__len__'):
+    # Skip addresses that are -1 (indicates no data available).
+    # E.g. for masked data, if no corresponding mask available
+    if offset < 0: return None
     with open(filename,'rb') as f:
       f.seek (offset,0)
       return np.fromfile(f,'B',length)
   # Vectorized version.
   out = []
   with open(filename,'rb') as f:
     for o, l in zip(offset, length):
+      # Skip addresses that are -1 (indicates no data available).
+      # E.g. for masked data, if no corresponding mask available
+      if o < 0:
+        out.append(None)
+        continue
       f.seek (o,0)
       out.append(np.fromfile(f,'B',l))
   return out
 
 
 class ExternOutput (BufferBase):
```

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/filter.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/filter.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/fstd.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/fstd.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/gridhacks.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/gridhacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,22 @@
 # Helper method - given an interpolation grid string, return a grid id.
 def _get_interp_grid (interp):
   import rpnpy.librmn.all as rmn
   # Extract interpolation grid.
   def number(x):
     try: return int(x)
     except ValueError: return float(x)
+  # Degenerate case: already have the grid info in a dictionary.
+  if hasattr(interp,'keys'):
+    return interp
+  # Degenerate case: have a grid id, just need to look up the info.
+  if isinstance(interp,int):
+    with _lock:
+      return rmn.decodeGrid(interp)
+  # Main case: Have grid info encoded as a string.
   with _lock:
     interp = interp.split(',')
     grtyp = interp[0]
     grid_args = [number(v) for v in interp[1:] if '=' not in v]
     grid_kwargs = dict(v.split('=') for v in interp[1:] if '=' in v)
     grid_kwargs = dict((k,number(v)) for k,v in grid_kwargs.items())
     if not hasattr(rmn,'defGrid_'+grtyp):
```

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/masks.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/masks.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/mesh.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/mesh.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/misc.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/misc.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/netcdf.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/netcdf.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/pruneaxes.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/pruneaxes.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/removestuff.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/removestuff.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/select.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/select.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/series.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/series.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/sfc_codes.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/sfc_codes.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/vardict.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/vardict.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/vcoords.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/vcoords.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/mixins/xycoords.py` & `fstd2nc-0.20230515.2/fstd2nc/mixins/xycoords.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc/stdout.py` & `fstd2nc-0.20230515.2/fstd2nc/stdout.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/fstd2nc.egg-info/PKG-INFO` & `fstd2nc-0.20230515.2/fstd2nc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstd2nc
-Version: 0.20230515.1
+Version: 0.20230515.2
 Summary: Converts RPN standard files (from Environment Canada) to netCDF files.
 Home-page: https://github.com/neishm/fstd2nc
 Author: Mike Neish
 License: LGPL-3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `fstd2nc-0.20230515.1/fstd2nc.egg-info/SOURCES.txt` & `fstd2nc-0.20230515.2/fstd2nc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20230515.1/setup.py` & `fstd2nc-0.20230515.2/setup.py`

 * *Files identical despite different names*

