# Comparing `tmp/werk24-1.4.1.tar.gz` & `tmp/werk24-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/werk24-1.4.1.tar", last modified: Thu Mar 16 10:52:15 2023, max compression
+gzip compressed data, was "dist/werk24-1.5.0.tar", last modified: Wed May 31 17:42:18 2023, max compression
```

## Comparing `werk24-1.4.1.tar` & `werk24-1.5.0.tar`

### file list

```diff
@@ -1,83 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:52:15.000000 werk24-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-16 10:52:03.000000 werk24-1.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-16 10:52:03.000000 werk24-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-16 10:52:03.000000 werk24-1.4.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-03-16 10:52:15.000000 werk24-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-03-16 10:52:03.000000 werk24-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 10:52:15.000000 werk24-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-03-16 10:52:03.000000 werk24-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:52:15.000000 werk24-1.4.1/werk24/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:52:15.000000 werk24-1.4.1/werk24/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:52:15.000000 werk24-1.4.1/werk24/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   366380 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/assets/fonts/STIX2Text-Regular.otf
--rw-r--r--   0 runner    (1001) docker     (123)   238007 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/assets/fonts/STIX_2.0.2_license.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:52:15.000000 werk24-1.4.1/werk24/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/assets/images/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/assets/images/favicon-24x24.png
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/assets/images/favicon-256x256.png
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/assets/images/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/assets/images/favicon-48x48.png
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/assets/images/logo-625.png
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/auth_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:52:15.000000 werk24-1.4.1/werk24/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/cli/techread.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/cli/w24cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:52:15.000000 werk24-1.4.1/werk24/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/gui/event_feed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/gui/event_illustrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/gui/gdt_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/gui/json_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/gui/measure_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/gui/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    23860 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/gui/w24gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/gui/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:52:15.000000 werk24-1.4.1/werk24/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)    28076 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/ask.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/chamfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/file_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/gdt.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/gender.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/general_tolerances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/geometric_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/leader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/note.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/part_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/radius.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/revision_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/roughness.py
--rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/techread.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/test_dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/thread_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/title_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/tolerance.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/models/weight.py
--rw-r--r--   0 runner    (1001) docker     (123)    30023 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/techread_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/techread_client_https.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/techread_client_wss.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-16 10:52:03.000000 werk24-1.4.1/werk24/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 10:52:15.000000 werk24-1.4.1/werk24.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-03-16 10:52:14.000000 werk24-1.4.1/werk24.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-03-16 10:52:15.000000 werk24-1.4.1/werk24.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 10:52:14.000000 werk24-1.4.1/werk24.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-16 10:52:14.000000 werk24-1.4.1/werk24.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-16 10:52:14.000000 werk24-1.4.1/werk24.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-16 10:52:14.000000 werk24-1.4.1/werk24.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:42:18.000000 werk24-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-31 17:42:08.000000 werk24-1.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-31 17:42:08.000000 werk24-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-31 17:42:08.000000 werk24-1.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-05-31 17:42:18.000000 werk24-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-31 17:42:08.000000 werk24-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 17:42:18.000000 werk24-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-31 17:42:08.000000 werk24-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:42:18.000000 werk24-1.5.0/werk24/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:42:18.000000 werk24-1.5.0/werk24/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:42:18.000000 werk24-1.5.0/werk24/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   366380 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/assets/fonts/STIX2Text-Regular.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   238007 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/assets/fonts/STIX_2.0.2_license.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:42:18.000000 werk24-1.5.0/werk24/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/assets/images/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/assets/images/favicon-24x24.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/assets/images/favicon-256x256.png
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/assets/images/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/assets/images/favicon-48x48.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/assets/images/logo-625.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/auth_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:42:18.000000 werk24-1.5.0/werk24/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/cli/techread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/cli/w24cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:42:18.000000 werk24-1.5.0/werk24/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/gui/event_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/gui/event_illustrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/gui/gdt_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/gui/json_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/gui/measure_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/gui/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23860 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/gui/w24gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/gui/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:42:18.000000 werk24-1.5.0/werk24/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28683 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/ask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/base_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/chamfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/depth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:42:18.000000 werk24-1.5.0/werk24/models/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/feature/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/feature/chamfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/feature/knurl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/file_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/fraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/gdt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/gender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/general_tolerances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/geometric_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/leader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/paper_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/part_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/physical_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:42:18.000000 werk24-1.5.0/werk24/models/property/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/property/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/property/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/property/cleanness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/property/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/property/corrosion_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/property/hardness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/property/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/property/surface_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/property/weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/revision_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/roughness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/techread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/test_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/thread_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/title_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/tolerance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/typed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/models/weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29423 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/techread_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/techread_client_https.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/techread_client_wss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-31 17:42:08.000000 werk24-1.5.0/werk24/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:42:18.000000 werk24-1.5.0/werk24.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-05-31 17:42:17.000000 werk24-1.5.0/werk24.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-31 17:42:18.000000 werk24-1.5.0/werk24.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:42:17.000000 werk24-1.5.0/werk24.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-31 17:42:17.000000 werk24-1.5.0/werk24.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-31 17:42:17.000000 werk24-1.5.0/werk24.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 17:42:17.000000 werk24-1.5.0/werk24.egg-info/top_level.txt
```

### Comparing `werk24-1.4.1/PKG-INFO` & `werk24-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: werk24
-Version: 1.4.1
+Version: 1.5.0
 Summary: Werk24 Client to read PDF- and Image-based Technical Drawings / Engineering Drawings
 Home-page: https://werk24.io
 Author: W24 Service GmbH
 Author-email: info@werk24.io
 License: commercial
 Project-URL: Documentation, https://docs.werk24.io/
 Description: # Werk24 Client
@@ -13,15 +13,15 @@
             <a href="https://werk24.io/?utm_source=github&utm_medium=logo" target="_blank">
               <img src="https://github.com/W24-Service-GmbH/.github/blob/main/profile/Werk24_banner_GitHub.png?raw=true" alt="Werk24">
             </a>
           </p>
         </p>
         
         [![pypi](https://img.shields.io/pypi/v/werk24.svg)](https://pypi.python.org/pypi/werk24)
-        [![Tests | cpython 3.7, 3.8, 3.9](https://github.com/W24-Service-GmbH/werk24-python/actions/workflows/python-test.yml/badge.svg)](https://github.com/W24-Service-GmbH/werk24-python/actions/workflows/python-test.yml)
+        [![Tests | cpython 3.8, 3.9, 3.10](https://github.com/W24-Service-GmbH/werk24-python/actions/workflows/python-test.yml/badge.svg)](https://github.com/W24-Service-GmbH/werk24-python/actions/workflows/python-test.yml)
         
         
         
         # Features
         When submitting a PDF, PNG, JPEG of a Technical Drawing to Werk24's API, you receive within seconds
         the following features:
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: werk24 Version: 1.4.1 Summary: Werk24 Client to
+Metadata-Version: 2.1 Name: werk24 Version: 1.5.0 Summary: Werk24 Client to
 read PDF- and Image-based Technical Drawings / Engineering Drawings Home-page:
 https://werk24.io Author: W24 Service GmbH Author-email: info@werk24.io
 License: commercial Project-URL: Documentation, https://docs.werk24.io/
 Description: # Werk24 Client
                                    [Werk24]
 [![pypi](https://img.shields.io/pypi/v/werk24.svg)](https://pypi.python.org/
-pypi/werk24) [![Tests | cpython 3.7, 3.8, 3.9](https://github.com/W24-Service-
+pypi/werk24) [![Tests | cpython 3.8, 3.9, 3.10](https://github.com/W24-Service-
 GmbH/werk24-python/actions/workflows/python-test.yml/badge.svg)](https://
 github.com/W24-Service-GmbH/werk24-python/actions/workflows/python-test.yml) #
 Features When submitting a PDF, PNG, JPEG of a Technical Drawing to Werk24's
 API, you receive within seconds the following features: - Measures and
 Tolerances - Threads and Chamfers - Geometric Dimensioning and Tolerancing
 frames - External Dimensions - Surface Roughnesses - the Title Block
 information (Material, Drawing ID, Designation, General Tolerances) And finally
```

### Comparing `werk24-1.4.1/README.md` & `werk24-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     <a href="https://werk24.io/?utm_source=github&utm_medium=logo" target="_blank">
       <img src="https://github.com/W24-Service-GmbH/.github/blob/main/profile/Werk24_banner_GitHub.png?raw=true" alt="Werk24">
     </a>
   </p>
 </p>
 
 [![pypi](https://img.shields.io/pypi/v/werk24.svg)](https://pypi.python.org/pypi/werk24)
-[![Tests | cpython 3.7, 3.8, 3.9](https://github.com/W24-Service-GmbH/werk24-python/actions/workflows/python-test.yml/badge.svg)](https://github.com/W24-Service-GmbH/werk24-python/actions/workflows/python-test.yml)
+[![Tests | cpython 3.8, 3.9, 3.10](https://github.com/W24-Service-GmbH/werk24-python/actions/workflows/python-test.yml/badge.svg)](https://github.com/W24-Service-GmbH/werk24-python/actions/workflows/python-test.yml)
 
 
 
 # Features
 When submitting a PDF, PNG, JPEG of a Technical Drawing to Werk24's API, you receive within seconds
 the following features:
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # Werk24 Client
                                    [Werk24]
 [![pypi](https://img.shields.io/pypi/v/werk24.svg)](https://pypi.python.org/
-pypi/werk24) [![Tests | cpython 3.7, 3.8, 3.9](https://github.com/W24-Service-
+pypi/werk24) [![Tests | cpython 3.8, 3.9, 3.10](https://github.com/W24-Service-
 GmbH/werk24-python/actions/workflows/python-test.yml/badge.svg)](https://
 github.com/W24-Service-GmbH/werk24-python/actions/workflows/python-test.yml) #
 Features When submitting a PDF, PNG, JPEG of a Technical Drawing to Werk24's
 API, you receive within seconds the following features: - Measures and
 Tolerances - Threads and Chamfers - Geometric Dimensioning and Tolerancing
 frames - External Dimensions - Surface Roughnesses - the Title Block
 information (Material, Drawing ID, Designation, General Tolerances) And finally
```

### Comparing `werk24-1.4.1/setup.py` & `werk24-1.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,17 +52,19 @@
     include_package_data=True,
 
     package_data={"werk24": ["assets/*"]},
     install_requires=[
         "aiohttp >= 3.8.3",
         "boto3 >= 1.14.44",
         "devtools >=0.9.0",
-        "pydantic >= 1.4",
+        "pydantic>=1.4,<=2.0",
+        "typing-extensions==4.5.0",
         "python-dotenv>=0.10.1",
-        "websockets >= 10.3"
+        "websockets >= 10.3",
+        "pint >= 0.21"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Image Recognition"],
     keywords=[
         'Digitisation', 'Digitization', 'Engineering Drawing',
```

### Comparing `werk24-1.4.1/werk24/assets/fonts/STIX2Text-Regular.otf` & `werk24-1.5.0/werk24/assets/fonts/STIX2Text-Regular.otf`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/assets/fonts/STIX_2.0.2_license.pdf` & `werk24-1.5.0/werk24/assets/fonts/STIX_2.0.2_license.pdf`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/assets/images/favicon-256x256.png` & `werk24-1.5.0/werk24/assets/images/favicon-256x256.png`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/assets/images/favicon-32x32.png` & `werk24-1.5.0/werk24/assets/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/assets/images/favicon-48x48.png` & `werk24-1.5.0/werk24/assets/images/favicon-48x48.png`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/assets/images/logo-625.png` & `werk24-1.5.0/werk24/assets/images/logo-625.png`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/auth_client.py` & `werk24-1.5.0/werk24/auth_client.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/cli/auth.py` & `werk24-1.5.0/werk24/cli/auth.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/cli/techread.py` & `werk24-1.5.0/werk24/cli/techread.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/cli/utils.py` & `werk24-1.5.0/werk24/cli/utils.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/cli/w24cli.py` & `werk24-1.5.0/werk24/cli/w24cli.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/exceptions.py` & `werk24-1.5.0/werk24/exceptions.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/gui/event_feed.py` & `werk24-1.5.0/werk24/gui/event_feed.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/gui/event_illustrator.py` & `werk24-1.5.0/werk24/gui/event_illustrator.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/gui/gdt_table.py` & `werk24-1.5.0/werk24/gui/gdt_table.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/gui/measure_table.py` & `werk24-1.5.0/werk24/gui/measure_table.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/gui/w24gui.py` & `werk24-1.5.0/werk24/gui/w24gui.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/gui/worker.py` & `werk24-1.5.0/werk24/gui/worker.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/models/angle.py` & `werk24-1.5.0/werk24/models/angle.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,52 @@
-from typing import Tuple
-import abc
 from decimal import Decimal
-from enum import Enum
-from typing import Optional
+from typing import Optional, Tuple
 
 from pydantic import UUID4, BaseModel
 
-from .feature import W24FeatureModel
+from .base_feature import W24BaseFeatureModel
+from .tolerance import W24Tolerance
 from .unit import W24UnitAngle
 
 
-class W24AngleTolerationType(str, Enum):
-    """ Enum listing all supported AngleToleration Type
-
-    !!! note
-        Currently we are only supporting the General
-        Tolerances indicated on the drawing's Title Block.
-        If you need access to more types, e.g.,
-        MINIMUM, MAXIMUM, OFF_SIZE, APPROXIMATION, please
-        reach out to us.
-    """
-    GENERAL_TOLERANCES = "GENERAL_TOLERANCES"
-
-
-class W24AngleToleration(BaseModel, abc.ABC):
-    """ Base Class that describes Angle Tolerances
-
-    Attributes:
-
-        toleration_type: Toleration Type  of the
-            `W24AngleSize`
-
-        blurb: String representation for human consumption
-
-    !!! caution
-        This model will soon be extended to contain the
-        toleration information derived from the TitleBlock.
-        Be aware that you will need to request the TitleBlock
-        to obtain this information.
-    """
-
-    toleration_type: W24AngleTolerationType
-
-    blurb: str
-
-
 class W24AngleSize(BaseModel):
-    """ Size of an Angle including its toleration
+    """ Size of an Angle including its tolerance
 
     Attributes:
 
         blurb: Blurb for human consumption
 
         angle: Nominal angle size in [units]
 
         unit: Angle Unit. Currently only degrees are
             supported.
     """
-
     blurb: str
-
     angle: Decimal
-
     unit: W24UnitAngle = W24UnitAngle.DEGREE
 
 
 class W24AngleLabel(BaseModel):
     """ Label associated with an Angle indicated
     on the Technical Drawing
 
     Attributes:
 
         blurb: Blurb for human consumption
-
-        size: Nominal angle size
-
-        size_toleration: Tolerated deviations
+        quantity: Number of annotated angles
+        angle: Nominal angle size
+        angle_tolerance: Tolerated deviations
     """
-
     blurb: str
-
-    size: W24AngleSize
-
-    size_toleration: W24AngleToleration
+    quantity: int
+    angle: W24AngleSize
+    angle_tolerance: W24Tolerance
 
 
-class W24Angle(W24FeatureModel):
+class W24Angle(W24BaseFeatureModel):
     """ Tolerated Angle detected on a sectional of the
     Technical Drawing
 
     Attributes:
 
         angle_id: Unique identifier of the Angle. This
             allows the reference of the angle from another
```

### Comparing `werk24-1.4.1/werk24/models/ask.py` & `werk24-1.5.0/werk24/models/ask.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Definition of all W24Ask types that are understood by the Werk24 API.
 """
-from typing import Tuple
+from werk24.models.process import W24Process
 from enum import Enum
-from typing import Any, Dict, List, Optional, Type, Union
+from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 from pydantic import UUID4, BaseModel, HttpUrl
 
 from werk24.models.note import W24Note
 from werk24.models.part_family import W24PartFamilyCharacterization
 
 from .angle import W24Angle
@@ -125,14 +125,18 @@
     """Ask for the thread elements of the variant
     """
 
     VARIANT_TOLERANCE_ELEMENTS = "VARIANT_TOLERANCE_ELEMENTS"
     """Ask for the tolerance elements of the variant
     """
 
+    VARIANT_PROCESSES = "VARIANT_PROCESSES"
+    """Ask for the Processes associated with the variant.
+    """
+
     INTERNAL_SCREENING = "INTERNAL_SCREENING"
     """Ask for internal screening - not available through public API
     """
 
 
 class W24Ask(BaseModel):
     """Base model from which all Asks inherit
@@ -782,14 +786,29 @@
     """Internal Ask to trigger the file screening.
 
     NOTE: not available on the public API.
     """
     ask_type = W24AskType.INTERNAL_SCREENING
 
 
+class W24AskVariantProcesses(W24Ask):
+    """Ask to receive the processes associated with the Variant.
+    """
+    ask_type = W24AskType.VARIANT_PROCESSES
+
+
+class W24AskVariantProcessesResponse(BaseModel):
+    """Response Model for the processes.
+
+    Attributes:
+        processes (List[W24Process]): List of all the
+            processes that were identified on the drawing.
+    """
+    processes: List[W24Process]
+
 # class W24AskVariantToleranceElements(W24Ask):
 #     """Ask object to obtain the tolerance elements
 #     """
 #     ask_type = W24AskType.VARIANT_TOLERANCE_ELEMENTS
 
 # class W24AskVariantToleranceElementsResponse(BaseModel):
 #     """Response object corresponding to the W24AskVariantThreadElements
@@ -800,14 +819,15 @@
 #             Technical Drawing. Refer to the documentation on Variants
 #             for details.
 
 #     """
 #     variant_id: UUID4
 #     thread_elements: List[W24ToleranceElement]
 
+
 W24AskUnion = Union[
     W24AskCanvasThumbnail,
     W24AskNotes,
     W24AskPageThumbnail,
     W24AskPartFamilyCharacterization,
     W24AskProductPMIExtract,
     W24AskRevisionTable,
@@ -821,14 +841,15 @@
     W24AskVariantGDTs,
     W24AskVariantLeaders,
     W24AskVariantMaterial,
     W24AskVariantMeasures,
     W24AskVariantRadii,
     W24AskVariantRoughnesses,
     W24AskVariantThreadElements,
+    W24AskInternalScreening,
     # W24AskVariantToleranceElements
 ]
 """Union of all W24Asks to ensure proper de-serialization """
 
 
 def deserialize_ask(
     raw: Union[Dict[str, Any], W24Ask],
```

### Comparing `werk24-1.4.1/werk24/models/chamfer.py` & `werk24-1.5.0/werk24/models/chamfer.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/models/depth.py` & `werk24-1.5.0/werk24/models/depth.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/models/feature.py` & `werk24-1.5.0/werk24/models/base_feature.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import List, Optional
 
 from pydantic import BaseModel
 
 
-class W24FeatureCoordinate(BaseModel):
+class W24BaseFeatureCoordinate(BaseModel):
     """ Coordinate point
 
     Attributes:
         x: x position normalized by the thumbnail's width
 
         y: y position normalized by the thumbnail's height
     """
     x: float
     y: float
 
 
-class W24FeaturePosition(BaseModel):
+class W24BaseFeaturePosition(BaseModel):
     """ Position of the Feature on the individual thumbnails normalized
     by the width and height of each thumbnail.
 
     Each features position is indicated as a list of coordinates. If the
         list only has two elements, you are dealing with a line. If it
         has four or more, you are looking at a polygon
 
@@ -27,25 +27,23 @@
         page: Position of the Feature on the Page thumbnail
 
         sheet: Position of the Feature on the Sheet thumbnail
 
         sectional: Position of the Feature on the Sectional thumbnail
 
     """
-    sheet: List[W24FeatureCoordinate]
-    canvas: List[W24FeatureCoordinate]
-    sectional: List[W24FeatureCoordinate]
+    sheet: List[W24BaseFeatureCoordinate]
+    canvas: List[W24BaseFeatureCoordinate]
+    sectional: List[W24BaseFeatureCoordinate]
 
 
-class W24FeatureModel(BaseModel):
+class W24BaseFeatureModel(BaseModel):
     """ Base Model for all the features that we might
     extract from the Drawing
 
     Attributes:
         position: Position of the features on the individual
             thumbnails
     """
 
     # NOTE: position is optional for the transition period
-    position: Optional[W24FeaturePosition] = None
-
-
+    position: Optional[W24BaseFeaturePosition] = None
```

### Comparing `werk24-1.4.1/werk24/models/file_format.py` & `werk24-1.5.0/werk24/models/file_format.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/models/gdt.py` & `werk24-1.5.0/werk24/models/gdt.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import abc
 from decimal import Decimal
 from enum import Enum
 from typing import List, Optional
 
 from pydantic import UUID4, BaseModel
 
-from .feature import W24FeatureModel
+from .base_feature import W24BaseFeatureModel
 
 
 class W24GDTCharacteristic(str, Enum):
     """ Enum of all possible Characteristics
     following ISO 1101.
 
     !!! note
@@ -66,14 +66,15 @@
 
 
 class W24GDTZoneConstraint(str, Enum):
     """ Enum of the Zone Constraints
     """
     UNSPECIFIED_INCLINATION = "OZ"
     UNSPECIFIED_OFFSET = "VA"
+    ORIENTATION_ONLY = "><"
 
 
 class W24GDTDatum(BaseModel):
     """ Preliminary implementation of the GD&T Datum
 
     Attributes:
         blurb: Reference name. Typically: A,B,C ...
@@ -140,14 +141,30 @@
 
 class W24GDTFilterType(str, Enum):
     """ Preliminary list of feature filters
 
     Filters remaining: RG, S, OH, SW, AB, CW
     """
     GAUSSIAN = "G"
+    SPLINE = "S"
+    SPLINE_WAVELET = "SW"
+    COMPLEX_WAVELET = "CW"
+    ROBUST_GAUSSIAN = "RG"
+    ROBUST_SPLINE = "RS"
+    OPENING_BALL = "OB"
+    OPENING_HORIZONTAL_SEGMENT = "OH"
+    OPENING_DISC = "OC"
+    CLOSING_BALL = "CB"
+    CLOSING_HORIZONTAL_SEGMENT = "CH"
+    CLOSING_DISC = "CD"
+    ALTERNATING_BALL = "AB"
+    ALTERNATING_HORIZONTAL_SEGMENT = "AH"
+    ALTERNATING_DISC = "AD"
+    FOURIER = "F"
+    HULL = "H"
 
 
 class W24GDTFilter(BaseModel, abc.ABC):
     """ Abstract base class to describe feature filters
 
     Attributes:
         blurb: String representation of the file for human consumption
@@ -328,15 +345,15 @@
     material_condition: Optional[W24GDTMaterialCondition] = None
 
     state: Optional[W24GDTState] = None
 
     data: List[W24GDTDatum] = []
 
 
-class W24GDT(W24FeatureModel):
+class W24GDT(W24BaseFeatureModel):
     """ Parent object for Geometric Dimensionsing and Toleration
     Frames, attaching them to the physical location on the drawing.
 
     Attributes:
         frame: Representation of the GDT frame
 
     """
```

### Comparing `werk24-1.4.1/werk24/models/general_tolerances.py` & `werk24-1.5.0/werk24/models/general_tolerances.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from decimal import Decimal
 from enum import Enum
 from typing import List, Optional, Union
-from pydantic import  BaseModel, validator
+from pydantic import BaseModel, validator
+
+from .base_feature import W24BaseFeatureModel
 
-from .feature import W24FeatureModel
 
 class W24GeneralTolerancesStandard(str, Enum):
     """ Enum of all supported
     General Tolerance Standards
     """
     DIN_7168 = "DIN 7168"
     ISO_2768 = "ISO 2768"
@@ -136,15 +137,15 @@
     blurb: str
 
     property: W24ToleranceProperty
 
     table: List[W24ToleranceTableItem]
 
 
-class W24GeneralTolerances(W24FeatureModel):
+class W24GeneralTolerances(W24BaseFeatureModel):
     """ Object representing the General Tolerances indicated
     on the Title Block of the Technical Drawing.
     """
 
     blurb: str
     """ Blurb of the general tolerances for human consumption
     """
```

### Comparing `werk24-1.4.1/werk24/models/geometric_shape.py` & `werk24-1.5.0/werk24/models/geometric_shape.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/models/leader.py` & `werk24-1.5.0/werk24/models/leader.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/models/material.py` & `werk24-1.5.0/werk24/models/material.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Material Models
 """
 from enum import Enum
 from typing import Tuple, Optional, Any
-from werk24.models.feature import W24FeatureModel
+from werk24.models.base_feature import W24BaseFeatureModel
 
 
 class W24MaterialCategory1(str, Enum):
     FERROUS_ALLOY = "FERROUS_ALLOY"
     NONFERROUS_ALLOY = "NONFERROUS_ALLOY"
     POLYMER = "POLYMER"
     CERAMIC = "CERAMIC"
@@ -490,15 +490,15 @@
 
     # FOAM / POLYMER_FOAM
     POLYPHENYLENE_OR_POLYSTYRENE = "POLYPHENYLENE_OR_POLYSTYRENE"
     POLYPHENYLENE_OR_POLYSTYRENE_HIPS = "POLYPHENYLENE_OR_POLYSTYRENE_HIPS"
     POLYCARBONATE = "POLYCARBONATE"
 
 
-class W24Material(W24FeatureModel):
+class W24Material(W24BaseFeatureModel):
     """W24 Object for Materials.
 
     Parsed Material object that can either be
     associated to the TitleBlock or derived from
     all the available information (including the
     text on the canvas.
```

### Comparing `werk24-1.4.1/werk24/models/measure.py` & `werk24-1.5.0/werk24/models/measure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 
 """ Defintion of all the W24Measure class its support structures
 """
 
 from enum import Enum
-from typing import Any, Dict, List, Optional
+from typing import List, Optional
 
-from pydantic import UUID4, BaseModel, validator
+from pydantic import UUID4, BaseModel
 
 from .chamfer import W24Chamfer
 from .depth import W24Depth
-from .feature import W24FeatureModel
-from .size import (W24Size, W24SizeTolerance, W24SizeToleranceGeneral,
-                   parse_tolerance)
+from .base_feature import W24BaseFeatureModel
+from .size import W24Size
 from .test_dimension import W24TestDimension
 from .thread import W24Thread
 from .unit import W24UnitLength
+from .tolerance import W24Tolerance, W24ToleranceGeneral
+from pydantic import validator
 
 
 class W24MeasureWarningType(str, Enum):
-    """ 
+    """
     List of all warnings that can be associated with
     the returned measures.
     """
 
     UNCONVENTIONAL_TOLERANCE_ORDER = "UNCONVENTIONAL_TOLERANCE_ORDER"
-    """ 
+    """
     The UNCONVENTIONAL_TOLERANCE_ORDER warning is raised
     when the first-mentioned tolerance is lower than the second-mentioned.
 
     EXAMPLE: 3 -0.1/+0.1 (rather than 3 +0.1/-0.1)
     """
 
     UNPROPORTIONAL = "UNPROPORTIONAL"
-    """ 
+    """
     The UNPROPORTIONAL warnings is set when the size indicated
     on the MeasureLabel is unproportional to the distance between
     the Measure's end-points.
     """
 
 
 class W24MeasureWarning(BaseModel):
-    """ 
+    """
     Warnings are issued when something about the label
     or measure is not conforming with convention
     """
     warning_type: W24MeasureWarningType
 
 
 class W24MeasureWarningUnconvetionalToleranceOrder(W24MeasureWarning):
-    """ 
+    """
     The UNCONVENTIONAL_TOLERANCE_ORDER warning is raised
     when the first-mentioned tolerance is lower than the second-mentioned.
 
     EXAMPLE: 3 -0.1/+0.1 (rather than 3 +0.1/-0.1)
     """
     warning_type = W24MeasureWarningType.UNCONVENTIONAL_TOLERANCE_ORDER
 
 
 class W24MeasureWarningUnproportional(W24MeasureWarning):
-    """ 
+    """
     The UNPROPORTIONAL warnings is set when the size indicated
     on the MeasureLabel is unproportional to the distance between
     the Measure's end-points.
 
     !!! note Three things can cause this:
 
     1. The Measure is truly unpropotional and carries an associated
@@ -111,15 +112,15 @@
             By default we are referring to the general tolerances of the drawing.
             When you are also requesting the TitleBlock, we are attaching the
             applicable General Tolerances (assuming they were understood)
             to the measure. This will consider the nominal size of the
             measure.
             If the W24MeasureLabel describes a "Theoretically Exact Measure",
             i.e, the label is surrounded by a box, like: "[15]", the size_tolerance
-            refers to a W24SizeToleranceTheoreticallyExact object (and is NOT None)
+            refers to a W24ToleranceTheoreticallyExact object (and is NOT None)
 
         unit: Length unit of the size. This information is only available
             when you request the TitleBlock as well; as only the title block
             will allow us to determine the geographic origin of the drawing.
 
         thread: Optional thread details.
             The thread details describe the complete thread description
@@ -129,53 +130,40 @@
 
         chamfer: Optional Chamfer
 
         depth: Depth of the drilling or thread. Uses the same dimensions
 
     """
 
+    @validator('size_tolerance', pre=True)
+    def deserialize_size_tolerance(cls, v):
+        if isinstance(v, W24Tolerance):
+            return v
+        return W24Tolerance.parse_obj(v)
+
     blurb: str
 
     quantity: int = 1
 
     size: W24Size
 
-    size_tolerance: W24SizeTolerance = W24SizeToleranceGeneral()
+    size_tolerance: W24Tolerance = W24ToleranceGeneral()
 
     unit: Optional[W24UnitLength] = None
 
     thread: Optional[W24Thread] = None
 
     chamfer: Optional[W24Chamfer] = None
 
     depth: Optional[W24Depth] = None
 
     test_dimension: Optional[W24TestDimension] = None
 
-    @validator('size_tolerance', pre=True)
-    def asks_validator(  # NOQA
-        cls,
-        raw: Dict[str, Any]
-    ) -> Optional[W24SizeTolerance]:
-        """ Pydantic does not automatically return the correct
-        W24SizeTolerance object. This function looks at the toleration_type
-        attribute and returns the correct W24SizeTolerance subclass
-
-        Args:
-
-            size_tolerance_raw (Dict[str, str]): Raw Dictionary of
-                the size tolerance
-
-        Returns:
-            W24SizeTolerance: Correctly deserialized Size Tolerance
-        """
-        return parse_tolerance(raw)
-
 
-class W24Measure(W24FeatureModel):
+class W24Measure(W24BaseFeatureModel):
     """ Measure object
 
     Attributes:
 
         measure_id: Unique UUID4 identifier
 
         label: Measure Label
```

### Comparing `werk24-1.4.1/werk24/models/note.py` & `werk24-1.5.0/werk24/models/note.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Data Model for Canvas and Sectional Notes.
 
 Author: Jochen Mattes
 """
 from enum import Enum
 
-from werk24.models.feature import W24FeatureModel
+from werk24.models.base_feature import W24BaseFeatureModel
 
 
 class W24NoteType(str, Enum):
     """Differentiation between Canvas and Sectional Notes.
 
     Canvas Notes are sometimes referred to as "General Notes",
     they are associated with the canvas in general.
@@ -25,15 +25,15 @@
     reduce.
     """
     CANVAS_NOTE = "CANVAS NOTE"
     SECTIONAL_NOTE = "SECTIONAL NOTE"
     SECTIONAL_CALLOUT = "SECTIONAL_CALLOUT"
 
 
-class W24Note(W24FeatureModel):
+class W24Note(W24BaseFeatureModel):
     """Notes object for Sectional and Canvas Notes.
 
     Attributes:
         type (W24NoteType): Type of the note to differentiate
             between notes that are associated with the complete
             sectional and the canvas
```

### Comparing `werk24-1.4.1/werk24/models/part_family.py` & `werk24-1.5.0/werk24/models/part_family.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/models/radius.py` & `werk24-1.5.0/werk24/models/radius.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 
 """ Defintion of all the W24Radius class its support structures
 """
 
 from typing import Optional
 
-from pydantic import UUID4, BaseModel
+from pydantic import UUID4, BaseModel, validator
 
-from .feature import W24FeatureModel
-from .size import W24Size, W24SizeTolerance, W24SizeToleranceGeneral
+from .base_feature import W24BaseFeatureModel
+from .size import W24Size
+from .tolerance import W24Tolerance, W24ToleranceGeneral
 from .unit import W24UnitLength
 
 
 class W24RadiusLabel(BaseModel):
     """ Radius Label
 
     Attributes:
@@ -27,26 +28,32 @@
             mentioned on the drawing, the general tolerances apply.
 
         unit: Length units of the size and size_tolerance. In most cases this
             will be be millimeter (METRIC) or inch (IMPERIAL) and be consistent
             for the complete drawing. Exceptions are very rare, but exist.
     """
 
+    @validator('size_tolerance', pre=True)
+    def deserialize_size_tolerance(cls, v):
+        if isinstance(v, W24Tolerance):
+            return v
+        return W24Tolerance.parse_obj(v)
+
     blurb: str
 
     quality: int = 1
 
     size: W24Size
 
-    size_tolerance: W24SizeTolerance = W24SizeToleranceGeneral()
+    size_tolerance: W24Tolerance = W24ToleranceGeneral()
 
     unit: Optional[W24UnitLength] = None
 
 
-class W24Radius(W24FeatureModel):
+class W24Radius(W24BaseFeatureModel):
     """ Radius Feature
 
     Attributes:
         radius_id: Unique UUID4 identifier. This can be used to provide
             automated feedback about customer changes.
 
         label: Label of the radius.
```

### Comparing `werk24-1.4.1/werk24/models/revision_table.py` & `werk24-1.5.0/werk24/models/revision_table.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/models/roughness.py` & `werk24-1.5.0/werk24/models/roughness.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .unit import W24UnitLength
 from decimal import Decimal
 from enum import Enum
 from typing import List, Optional
 
 from pydantic import UUID4, BaseModel
 
-from .feature import W24FeatureModel
+from .base_feature import W24BaseFeatureModel
 from .unit import W24UnitSystem
 
 
 class W24RoughnessStandard(str, Enum):
     """ Most standards that define the surface roughness use
     very similar symbols. However, the position of the fields
     varies.
@@ -342,15 +342,15 @@
     conditions: List[W24RoughnessCondition]
 
     unit_system: W24UnitSystem
 
     waviness: Optional[W24RoughnessWaviness]
 
 
-class W24Roughness(W24FeatureModel):
+class W24Roughness(W24BaseFeatureModel):
     """ Roughness object
 
     Attributes:
         roughness_id: Unique UUID4 identifier
 
         label: RoughnessLabel
     """
```

### Comparing `werk24-1.4.1/werk24/models/size.py` & `werk24-1.5.0/werk24/models/tolerance.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,39 @@
-import abc
 from decimal import Decimal
 from enum import Enum
-from typing import Any, Dict, Optional
+from typing import Optional
 
 from pydantic import BaseModel
 
-from .general_tolerances import W24GeneralTolerancesStandard
+from werk24.models.standard import W24Standard
+from werk24.models.typed_model import W24TypedModel
 
-
-class W24SizeToleranceType(str, Enum):
-    """ Enum of the supported tolerations
-    """
-    APPROXIMATION = "APPROXIMATION"
-    FIT_SIZE_ISO = "FIT_SIZE_ISO"
-    GENERAL_TOLERANCES = "GENERAL_TOLERANCES"
-    MINIMUM = "MINIMUM"
-    MAXIMUM = "MAXIMUM"
-    OFF_SIZE = "OFF_SIZE"
-    THEORETICALLY_EXACT = "THEORETICALLY_EXACT"
-    REFERENCE = "REFERENCE"
+from .base_feature import W24BaseFeatureModel
+from .gender import W24Gender
 
 
-class W24SizeTolerance(BaseModel, abc.ABC):
-    """ Abstract Base Class to cover the Tolerations
+class W24Tolerance(W24TypedModel):
+    """ Abstract Base Class to cover the Tolerances.
 
     Attributes:
         blurb (str): String representation for human consumption
 
         toleration_type (W24SizeToleranceType):  Toleration Type for
             deserialization
     """
-    toleration_type: W24SizeToleranceType
+    class Config:
+        discriminators = ('toleration_type',)
 
     blurb: str
+    toleration_type: str
 
 
 class W24ToleranceGradeWarning(str, Enum):
     """ Warnings associated with the Tolerance Grade.
     """
-
     SIZE_LARGER_THAN_NORM = "SIZE_LARGER_THAN_NORM"
     TOLERANCE_WIDTH_SMALLER_THAN_NORM = "TOLERANCE_WIDTH_SMALLER_THAN_NORM"
     TOLERANCE_WIDTH_LARGER_THAN_NORM = "TOLERANCE_WIDTH_LARGER_THAN_NORM"
 
 
 class W24ToleranceGrade(BaseModel):
     """ Tolerance Grade following ISO 286-1
@@ -60,26 +51,26 @@
             ends of this norm, we return a warning.
 
         NOTE: when a tolerance is outside the norm, we still
             return the closest matching grade.
 
         NOTE: when tolerances are implausible (e.g., 3+/-6),
             Werk24 will strip the tolerance completely and
-            return an untolerated measure of nominal size 3.
+            return an untoleranced measure of nominal size 3.
 
     """
     blurb: str
 
     grade: Optional[str]
 
     warning: Optional[W24ToleranceGradeWarning]
 
 
-class W24SizeToleranceFitsizeISO(W24SizeTolerance):
-    """ ISO fit size tolerations
+class W24ToleranceFitsizeISO(W24Tolerance):
+    """ ISO fit size tolerances
 
     Attributes:
         blurb (str): Text representation for human consumption.
 
         deviation_lower (Decimal): Lower deviation from the
             nominal size
 
@@ -88,17 +79,15 @@
 
         fundamental_deviation (str): Fundamental deviation of
             the fit (e.g., 'H' for a 'H7' fit)
 
         tolerance_grade (Optional[int]): Tolerance Grade corresponding
             to ISO 286-1. In German IT-Grad.
     """
-    toleration_type = W24SizeToleranceType.FIT_SIZE_ISO
-
-    blurb: str
+    toleration_type: str = "FIT_SIZE_ISO"
 
     deviation_lower: Decimal
 
     deviation_upper: Decimal
 
     fundamental_deviation: str
 
@@ -110,52 +99,42 @@
 
         Returns:
             Decimal: Deviation width
         """
         return self.deviation_upper-self.deviation_lower
 
 
-class W24SizeToleranceReference(W24SizeTolerance):
-    """ Measures written in brackets are Reference
-    Measures that are not tolerated.
-
-    Attributes:
-        tolerantion_type (W24SizeToleranceType): Reference
-            Tolerance Type
-
-        blurb (str): Text representation for human consumption.
+class W24ToleranceReference(W24Tolerance):
+    """Measures written in brackets are Reference.
     """
-    toleration_type = W24SizeToleranceType.REFERENCE
+    toleration_type: str = "REFERENCE"
 
 
-class W24SizeToleranceOffSize(W24SizeTolerance):
+class W24ToleranceOffSize(W24Tolerance):
     """ Off-size based tolerances
 
     Attributes:
         blurb (str): Text representation for human consumption.
 
         deviation_lower (Decimal): Lower deviation from the
             nominal size
 
         deviation_upper (Decimal): Upper deviation from the
             nominal size
 
         tolerance_grade (int): Tolerance Grade corresponding to
             ISO 286-1. In German IT-Grad.
     """
-    toleration_type = W24SizeToleranceType.OFF_SIZE
-
+    toleration_type: str = "OFF_SIZE"
     deviation_lower: Decimal
-
     deviation_upper: Decimal
-
     tolerance_grade: W24ToleranceGrade
 
 
-class W24SizeToleranceGeneral(W24SizeTolerance):
+class W24ToleranceGeneral(W24Tolerance):
     """ General Tolerances
 
     Attributes:
         tolerance_type: W24SizeToleranceType General Tolerances
             as key to differentiate between the different
             tolerance types
 
@@ -175,30 +154,24 @@
 
         deviation_upper: Upper deviation from the nominal size
             if the General Tolerance is known. None otherwise.
 
         tolerance_grade (int): Tolerance Grade corresponding to
             ISO 286-1. (German: IT-Grad).
     """
-    toleration_type = W24SizeToleranceType.GENERAL_TOLERANCES
-
+    toleration_type: str = "GENERAL_TOLERANCES"
     blurb: str = ""
-
-    standard: Optional[W24GeneralTolerancesStandard]
-
+    standard: Optional[W24Standard]
     standard_class: Optional[str]
-
     deviation_lower: Optional[Decimal]
-
     deviation_upper: Optional[Decimal]
-
     tolerance_grade: Optional[W24ToleranceGrade]
 
 
-class W24SizeToleranceTheoreticallyExact(W24SizeTolerance):
+class W24ToleranceTheoreticallyExact(W24Tolerance):
     """ Theoretically Exact Measures after ISO 5458
     must not be tolerated. They are indicated by a small
     rectangular frame.
 
     Example:
         +------+
         |  15  |
@@ -209,121 +182,53 @@
         tolerated, theoretically exact measures.
         Example:
             +------------+
             | 15 +/- 0.2 |
             +------------+
         In these situations the toleration takes priority.
     """
-    toleration_type = W24SizeToleranceType.THEORETICALLY_EXACT
+    toleration_type: str = "THEORETICALLY_EXACT"
 
 
-class W24SizeToleranceMinimum(W24SizeTolerance):
+class W24ToleranceMinimum(W24Tolerance):
     """ Minimum Size of a measure
     Example:
         min. 15
     """
-    toleration_type = W24SizeToleranceType.MINIMUM
+    toleration_type: str = "MINIMUM"
 
 
-class W24SizeToleranceMaximum(W24SizeTolerance):
+class W24ToleranceMaximum(W24Tolerance):
     """ Maximum Size of a measure
     Example:
         max 15
     """
-    toleration_type = W24SizeToleranceType.MAXIMUM
+    toleration_type: str = "MAXIMUM"
 
 
-class W24SizeToleranceApproximation(W24SizeTolerance):
+class W24ToleranceApproximation(W24Tolerance):
     """ Approximation of a measure
     Example:
         ~ 15
         ca. 14
     """
-    toleration_type = W24SizeToleranceType.APPROXIMATION
-
-
-class W24SizeType(str, Enum):
-    """ Enum describing the different size types
-    """
-    NOMINAL = "NOMINAL"
-    DIAMETER = "DIAMETER"
-    WIDTH_ACROSS_FLATS = "WIDTHS_ACROSS_FLATS"
+    toleration_type: str = "APPROXIMATION"
 
 
-class W24Size(BaseModel, abc.ABC):
-    """ Abstract Base Class for the Sizes
+class W24ToleranceFeature(W24BaseFeatureModel):
+    """Characterization of a Tolerance Feature.
 
     Attributes:
-        blurb: Blurb for human consumption
-
-        size_type: Size type for deserialization
-
-        nominal_size: Unitless nominal size. The unit
-            is it attached to the parent object, that
-            also defines the toleration.
-    """
-    blurb: str
-
-    size_type: W24SizeType
-
-    nominal_size: Decimal
+        gender: Gender (male or female) of the tolerance feature.
+            This is determined by checking whether the tolerance feature is
+            located on the outer contour of the part or inside the part.
+            When the outer contour is unavailable (e.g., in detail drawings),
+            the gender is set to None.
 
+        length: Length of the slug corresponding to the tolerance feature.
 
-class W24SizeNominal(W24Size):
-    """ Exactly your nominal size
     """
-    size_type = W24SizeType.NOMINAL
-
-
-class W24SizeDiameter(W24Size):
-    """ Diameter size
-    """
-    size_type = W24SizeType.DIAMETER
-
-
-class W24SizeWidthsAcrossFlats(W24Size):
-    """ Width across flats / Wrench Sizes
-
-    Attributes:
-        width_across_flats: Size across flats
-            aka. wrench size.
-    """
-    size_type = W24SizeType.WIDTH_ACROSS_FLATS
-
-    width_across_flats: Decimal
-
-
-def parse_tolerance(
-    raw: Dict[str, Any]
-) -> Optional[W24SizeTolerance]:
-    """ Pydantic does not automatically return the correct
-    W24SizeTolerance object. This function looks at the toleration_type
-    attribute and returns the correct W24SizeTolerance subclass
-
-    Args:
-        size_tolerance_raw (Dict[str, str]): Raw Dictionary of
-            the size tolerance
-
-    Returns:
-        W24SizeTolerance: Correctly deserialized Size Tolerance
-    """
-    # get the class in question
-    type_ = raw.toleration_type \
-        if hasattr(raw, 'toleration_type')\
-        else raw.get('toleration_type')
-
-    class_ = {
-        W24SizeToleranceType.APPROXIMATION: W24SizeToleranceApproximation,
-        W24SizeToleranceType.FIT_SIZE_ISO: W24SizeToleranceFitsizeISO,
-        W24SizeToleranceType.GENERAL_TOLERANCES: W24SizeToleranceGeneral,
-        W24SizeToleranceType.MINIMUM: W24SizeToleranceMinimum,
-        W24SizeToleranceType.MAXIMUM: W24SizeToleranceMaximum,
-        W24SizeToleranceType.OFF_SIZE: W24SizeToleranceOffSize,
-        W24SizeToleranceType.REFERENCE: W24SizeToleranceReference,
-        W24SizeToleranceType.THEORETICALLY_EXACT:
-        W24SizeToleranceTheoreticallyExact,
-    }.get(type_)
+    gender: Optional[W24Gender]
 
-    if class_ is None:
-        return None
+    length: Optional[Decimal]
 
-    return class_.parse_obj(raw)
+    tolerance: W24Tolerance
```

### Comparing `werk24-1.4.1/werk24/models/techread.py` & `werk24-1.5.0/werk24/models/techread.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/models/test_dimension.py` & `werk24-1.5.0/werk24/models/test_dimension.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/models/thread.py` & `werk24-1.5.0/werk24/models/thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 import abc
 from decimal import Decimal
 from enum import Enum
 from typing import List, Dict, Any, Optional, Type
 
 from pydantic import BaseModel, validator
 
-from werk24.models.feature import W24FeatureModel
+from werk24.models.base_feature import W24BaseFeatureModel
 
 from .unit import W24UnitLength
-from .size import W24SizeTolerance
+from .tolerance import W24Tolerance
 from .gender import W24Gender
 
+
 class W24ThreadType(str, Enum):
     """ Enum for the individual thread types
 
     NOTE: UTS_COARSE, UTS_FINE, UTS_EXTRAFINE and UTS_SPECIAL
         as individual types will be deprecated. Their information
         individual `threads_per_inch` information will be stored
         in the corresponding variable.
@@ -43,14 +44,15 @@
 class W24ThreadHandedness(str, Enum):
     """ Enum describing the direction of the
     thread
     """
     LEFT = "LEFT"
     RIGHT = "RIGHT"
 
+
 class W24ThreadMultiStart(BaseModel):
     """ Multi-Start Thread Information
 
     A common example of multi-start threads are the cap on a plastic
     water bottle. The cap will screw on quickly because a multi-start thread.
 
     Attributes:
@@ -165,18 +167,18 @@
 
         outer_pitch_diameter_tolerance (str): Corresponding
             tolerance class for the pitch diameter of the outer thread.
 
     """
     thread_type = W24ThreadType.ISO_METRIC
 
-    female_major_diameter_tolerance: Optional[W24SizeTolerance]
-    female_pitch_diameter_tolerance: Optional[W24SizeTolerance]
-    male_major_diameter_tolerance: Optional[W24SizeTolerance]
-    male_pitch_diameter_tolerance: Optional[W24SizeTolerance]
+    female_major_diameter_tolerance: Optional[W24Tolerance]
+    female_pitch_diameter_tolerance: Optional[W24Tolerance]
+    male_major_diameter_tolerance: Optional[W24Tolerance]
+    male_pitch_diameter_tolerance: Optional[W24Tolerance]
 
 
 class W24ThreadUTS(W24Thread):
 
     """ Unified Thread Standard (UTS) base class for
     * UNC - Unified National Coarse Thread
     * UNF - Unified National Fine Thread
@@ -252,15 +254,15 @@
     thread_type = W24ThreadType.WHITWORTH
 
     whitworth_size: Decimal
 
     tolerance_class: Optional[str] = None
 
 
-class W24ThreadFeature(W24FeatureModel):
+class W24ThreadFeature(W24BaseFeatureModel):
     """Characterization of a Thread Feature
 
     Attributes:
         gender: Gender (male or female) of the thread feature.
             This is determined by checking whether the thread is
             located on the outer contour of the part or inside the part.
             When the outer contour is unavailable (e.g., in detail drawings),
```

### Comparing `werk24-1.4.1/werk24/models/thread_element.py` & `werk24-1.5.0/werk24/models/thread_element.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/models/title_block.py` & `werk24-1.5.0/werk24/models/title_block.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel, validator
 
-from werk24.models.color import W24Color
+from werk24.models.property.color import W24PropertyColor
 
-from .feature import W24FeatureModel
+from .base_feature import W24BaseFeatureModel
 from .general_tolerances import W24GeneralTolerances
 from .language import W24Language
 from .material import W24Material
 from .weight import W24Weight
 
 
-class W24TitleBlockItem(W24FeatureModel):
+class W24TitleBlockItem(W24BaseFeatureModel):
     """ Per-Language caption or value
 
     Attributes:
 
         language: Language in accordance with the ISO/639-2B standards
 
         text: Text of the identification
@@ -44,39 +44,39 @@
 
     captions: List[W24TitleBlockItem]
 
     values: List[W24TitleBlockItem]
 
 
 class W24FileExtensionType(str, Enum):
-    """ 
+    """
     Enum of the extension types.
 
     For example, pdf and idw extensions will be mapped to
     DRAWING, while step and stl extensions will be mapped
     to MODEL.
     """
     DRAWING = "DRAWING"
     MODEL = "MODEL"
     UNKNOWN = "UNKNOWN"
 
 
 class W24FilePathType(str, Enum):
-    """ 
+    """
     Enum of the file path types, indicating whether a
     POSIX (unix) or WINDOWS path is used. When only a filename
     is indicated, the value will be UNKNOWN
     """
     POSIX = "POSIX"
     WINDOWS = "WINDOWS"
     UNKNOWN = "UNKNOWN"
 
 
-class W24Filename(W24FeatureModel):
-    """ 
+class W24Filename(W24BaseFeatureModel):
+    """
     Object describing all the information that we can
     deduce from a filename that was found on the TitleBlock
 
     Attributes:
 
         blurb: Filename and Path as it was found on the drawing.
             Example: /path/to/drawing.pdf
@@ -103,15 +103,15 @@
 
     extension_type: W24FileExtensionType
 
     path_type: W24FilePathType
 
 
 class W24TitleBlock(BaseModel):
-    """ 
+    """
     Information that could be extracted from the Title Block.
 
     Attributes:
 
         designation: Designation of the Sheet on the Title Block
 
         drawing_id: Main Identification Number of the Drawing
@@ -150,22 +150,22 @@
 
     material: Optional[W24Material]
 
     weight: Optional[W24Weight]
 
     filename_drawing: Optional[W24Filename] = None
 
-    colors: List[W24Color] = []
+    colors: List[W24PropertyColor] = []
 
     @validator('designation', pre=True)
     def designation_validator(
         cls,
         raw: Dict[str, Any]
     ) -> Optional[W24CaptionValuePair]:
-        """ 
+        """
         Workaround to deal with the transition period
         while we move from the single-value to the multi-value
         pairs.
 
         This code can be removed after we complete the
         transition.
 
@@ -181,15 +181,15 @@
         return cls._parse_caption_value_pair(raw)
 
     @validator('drawing_id', pre=True)
     def drawing_id_validator(
         cls,
         raw: Dict[str, Any]
     ) -> Optional[W24CaptionValuePair]:
-        """ 
+        """
         Workaround to deal with the transition period
         while we move from the single-value to the multi-value
         pairs.
 
         This code can be removed after we complete the
         transition.
 
@@ -205,15 +205,15 @@
         return cls._parse_caption_value_pair(raw)
 
     @validator('reference_ids', pre=True)
     def reference_ids_validator(
         cls,
         raw: List[Dict[str, Any]]
     ) -> List[W24CaptionValuePair]:
-        """ 
+        """
         Workaround to deal with the transition period
         while we move from the single-value to the multi-value
         pairs.
 
         This code can be removed after we complete the
         transition.
 
@@ -232,15 +232,15 @@
         ]
         return [r for r in result if r is not None]
 
     @staticmethod
     def _parse_caption_value_pair(
         raw: Optional[Dict[str, Any]]
     ) -> Optional[W24CaptionValuePair]:
-        """ 
+        """
         Workaround to deal with the transition period
         while we move from the single-value to the multi-value
         pairs.
 
         This code can be removed after we complete the
         transition.
```

### Comparing `werk24-1.4.1/werk24/models/unit.py` & `werk24-1.5.0/werk24/models/unit.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24/models/weight.py` & `werk24-1.5.0/werk24/models/weight.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
-from .feature import W24FeatureModel
+from .base_feature import W24BaseFeatureModel
 from .unit import W24UnitWeight, W24UnitLength
 
 
-class W24Weight(W24FeatureModel):
+class W24Weight(W24BaseFeatureModel):
     """ Weight of a Part - for example as indicated
     on the Title Block.
 
     NOTE: this can also be a relative weight
     (e.g. kg per meter for profiles)
 
     Attributes:
```

### Comparing `werk24-1.4.1/werk24/techread_client.py` & `werk24-1.5.0/werk24/techread_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,14 @@
 from werk24.techread_client_https import TechreadClientHttps
 from werk24.techread_client_wss import TechreadClientWss
 
 # make the logger
 logger = logging.getLogger('w24_techread_client')
 
 ENVIRONS = [
-    "W24TECHREAD_SERVER_HTTPS",
-    "W24TECHREAD_SERVER_WSS",
     "W24TECHREAD_VERSION",
     "W24TECHREAD_AUTH_CLIENT_ID",
     "W24TECHREAD_AUTH_CLIENT_SECRET",
     "W24TECHREAD_AUTH_IDENTITY_POOL_ID",
     "W24TECHREAD_AUTH_USER_POOL_ID",
     "W24TECHREAD_AUTH_USERNAME",
     "W24TECHREAD_AUTH_PASSWORD",
@@ -89,17 +87,15 @@
 }
 """ Map to translate the local exceptions to official
 W24Exceptions. This allows us to mock consistent responses
 even when the files are rejected before they reach the API
 """
 
 DEFAULT_AUTH_REGION = "eu-central-1"
-DEFAULT_SERVER_HTTPS = "techread.w24.io"
-DEFAULT_SERVER_WSS = "techread-ws.w24.io"
-DEFAULT_VERSION = "v1"
+DEFAULT_SERVER_WSS = "ws-api.w24.co"
 
 
 LICENSE_ERROR_TEXT = """
 
 ////////////////////////////////////////////////////////////////////////////////
 
 ,.'xWWx'.,kWWd'.;0O,..'',,,,:Ox'..',,'',:lOWNo..:0MXd,.'lKWMNOc'.,;;'....';,....
@@ -151,27 +147,24 @@
     """ Simple W24Client that allows you to use
     learn more about the content on your Technical
     Drawings.
     """
 
     def __init__(
         self,
-        techread_server_https: str,
         techread_server_wss: str,
         techread_version: str,
         development_key: str = None
     ):
         """ Initialize a new W24TechreadClient. If you wonder
         about any of the attributes, have a look at the .env
         file that we provided to you. They contain all the
         information that you will need.
 
         Arguments:
-            techread_server_https {str} -- domain name that
-                is being used by the https client
 
             techread_server_wss {str} -- domain name that
                 is being used by the websocket client
 
             techread_version {str} -- version that you want to
                 connect to
 
@@ -186,16 +179,15 @@
         self._development_key = development_key
 
         # Create an empty reference to the authentication
         # service (currently AWS Cognito)
         self._auth_client: Optional[AuthClient] = None
 
         # Initialize an instance of the HTTPS client
-        self._techread_client_https = TechreadClientHttps(
-            techread_server_https, techread_version)
+        self._techread_client_https = TechreadClientHttps(techread_version)
 
         # Initialize an instance of the WEBSOCKET client
         self._techread_client_wss = TechreadClientWss(
             techread_server_wss, techread_version)
 
     async def __aenter__(
             self
@@ -589,15 +581,15 @@
     @classmethod
     def make_from_env(
         cls,
         license_path: Optional[str] = None,
         auth_region: Optional[str] = None,
         server_https: Optional[str] = None,
         server_wss: Optional[str] = None,
-        version: Optional[str] = None
+        version: str = "v2"
     ) -> "W24TechreadClient":
         """ Small helper function that creates a new
         W24TechreadClient from the environment info.
 
         Arguments:
             license_path:{Optional[str]} -- path to the License file.
                 By default we are looking for a .werk24 file in the current
@@ -642,35 +634,25 @@
 
         # then make sure we use the correct priorities
         auth_region = pick_env(
             auth_region,
             'W24TECHREAD_AUTH_REGION',
             DEFAULT_AUTH_REGION)
 
-        server_https = pick_env(
-            server_https,
-            'W24TECHREAD_SERVER_HTTPS',
-            DEFAULT_SERVER_HTTPS)
-
         server_wss = pick_env(
             server_wss,
-            'W24TECHREAD_SERVER_WSS',
+            'W24TECHREAD_SERVER_WSS_V2',
             DEFAULT_SERVER_WSS)
 
-        version = pick_env(
-            version,
-            'W24TECHREAD_VERSION',
-            DEFAULT_VERSION)
-
         # get the variables from the environment and ensure that they
         # are set. If not, raise an exception
         try:
 
             # create a reference to the client
-            client = W24TechreadClient(server_https, server_wss, version)
+            client = W24TechreadClient(server_wss, version)
 
             # register the credentials. This will in effect
             # only set the variabels in the authorizer. It will
             # not trigger a network request
             client.register(
                 auth_region,
                 environs['W24TECHREAD_AUTH_IDENTITY_POOL_ID'],
```

### Comparing `werk24-1.4.1/werk24/techread_client_https.py` & `werk24-1.5.0/werk24/techread_client_https.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 """ HTTPS-part of the Werk24 client
 """
-import base64
 from types import TracebackType
 from typing import Optional, Type
-from urllib.parse import urlparse
 
 import aiohttp
 from pydantic import HttpUrl
 
-from werk24.exceptions import (BadRequestException, RequestTooLargeException,
-                               ResourceNotFoundException, ServerException,
-                               UnauthorizedException,
-                               UnsupportedMediaType)
+from werk24.exceptions import (
+    BadRequestException,
+    RequestTooLargeException,
+    ResourceNotFoundException,
+    ServerException,
+    UnauthorizedException,
+    UnsupportedMediaType,
+)
 from werk24.models.techread import W24PresignedPost
 
 from .auth_client import AuthClient
 
 
 class TechreadClientHttps:
 
     """ Translation map from the server response
     to the W24TechreadArchitectureStatus enum
     """
 
-    def __init__(self, techread_server_https: str, techread_version: str):
-        """ Intialize a new session with the https server
+    def __init__(self, techread_version: str):
+        """
+        Initialize a new session with the https server.
 
         Arguments:
             techread_server_https {str} -- Domain of the Techread https server
             techread_version {str} -- Techread Version
         """
-        self._techread_server = techread_server_https
         self._techread_version = techread_version
         self._techread_session_https: Optional[aiohttp.ClientSession] = None
         self._auth_client: Optional[AuthClient] = None
 
     async def __aenter__(
             self
     ) -> 'TechreadClientHttps':
@@ -45,23 +47,15 @@
             RuntimeError  -- Raise when the developer enters the session
                 without having called register_auth_client()
 
         Returns:
             TechreadClientHttps -- TechreadClientHttps version with active
                 session
         """
-
-        # make sure that we have an AuthClient
-        if self._auth_client is None:
-            raise RuntimeError(
-                "You need to call register_auth_client() before you can start"
-                + " the session")
-
-        headers = {"Authorization": f"Bearer {self._auth_client.token}"}
-        self._techread_session_https = aiohttp.ClientSession(headers=headers)
+        self._techread_session_https = aiohttp.ClientSession()
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_value: Optional[BaseException],
         traceback: Optional[TracebackType]
@@ -140,40 +134,18 @@
             form.add_field(key, value)
         form.add_field('file', content)
 
         # create a new fresh session that does not
         # carry the authentication token
         async with aiohttp.ClientSession() as sess:
             async with sess.post(presigned_post.url, data=form) as resp:
-
                 # check the status code of the response and
                 # raise the appropriate exception
                 self._raise_for_status(presigned_post.url, resp.status)
 
-    def _make_endpoint_url(
-        self,
-        subpath: str
-    ) -> str:
-        """ Make the endpoint url of the subpath.
-        This will create a fully valid http url
-        that can be used in the post and get requests
-
-        Arguments:
-            subpath {str} -- Path of the endpoint on
-                the TechreadAPI
-
-        Returns:
-            str -- Fully qualified url including
-                the server name and api version
-        """
-        return "https://{}/{}/{}".format(
-            self._techread_server,
-            self._techread_version,
-            subpath)
-
     async def download_payload(self, payload_url: HttpUrl) -> bytes:
         """ Return the payload from the server
 
         Arguments:
             payload_url {HttpUrl} -- Url of the payload
 
         Raises:
@@ -223,15 +195,15 @@
         except (UnauthorizedException,  # pylint: disable=try-except-raise
                 RequestTooLargeException,
                 ServerException, BadRequestException,
                 ResourceNotFoundException):
             raise
 
         # otherwise return the response text
-        return base64.b64decode(await response.text())
+        return await response.content.read()
 
     async def _get(
             self,
             url: str
     ) -> aiohttp.ClientResponse:
         """ Send a GET request request and return the
         response object. The method automatically
```

### Comparing `werk24-1.4.1/werk24/techread_client_wss.py` & `werk24-1.5.0/werk24/techread_client_wss.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,15 @@
             self._techread_server_wss,
             self._techread_version)
 
         # make the ehaders
         headers = [("Authorization", f"Bearer {self._auth_client.token}")]
 
         # now make the session
-        self._techread_session_wss = await websockets.connect(
-            endpoint,
-            extra_headers=headers)
+        self._techread_session_wss = await websockets.connect(endpoint, extra_headers=headers)
 
         # return ourselfves
         return self
 
     async def __aexit__(
             self,
             exc_type: Optional[Type[BaseException]],
@@ -141,37 +139,36 @@
 
         # and finally return
         return message
 
     @staticmethod
     async def _process_message(message_raw: str) -> W24TechreadMessage:
         """ Interpret the raw websocket message and
-        turn it inot a W24TechreadMessage
+        turn it into a W24TechreadMessage
 
         Arguments:
             message_raw {str} -- Raw message
 
         Raises:
             UnauthorizedException: Exception is raised
                 when you requested an action that you
-                have no priviledges for (or that does
+                have no privileges for (or that does
                 not exist)
 
             ServerException: Exception is raised when
                 the server did not respond as expected
 
         Returns:
             W24TeachreadMessage -- interpreted message
         """
-
         # interpret and return
         try:
             message = W24TechreadMessage.parse_raw(message_raw)
 
-        # if that failes, we are probably receiving a
+        # if that fails, we are probably receiving a
         # message from the gateway directly
         except ValidationError:
 
             # The Gateway responds with the format
             # {"message": str, "connectionId":str, "requestId":str}
             # Obtain the message
             response = json.loads(message_raw)
```

### Comparing `werk24-1.4.1/werk24/utils.py` & `werk24-1.5.0/werk24/utils.py`

 * *Files identical despite different names*

### Comparing `werk24-1.4.1/werk24.egg-info/PKG-INFO` & `werk24-1.5.0/werk24.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: werk24
-Version: 1.4.1
+Version: 1.5.0
 Summary: Werk24 Client to read PDF- and Image-based Technical Drawings / Engineering Drawings
 Home-page: https://werk24.io
 Author: W24 Service GmbH
 Author-email: info@werk24.io
 License: commercial
 Project-URL: Documentation, https://docs.werk24.io/
 Description: # Werk24 Client
@@ -13,15 +13,15 @@
             <a href="https://werk24.io/?utm_source=github&utm_medium=logo" target="_blank">
               <img src="https://github.com/W24-Service-GmbH/.github/blob/main/profile/Werk24_banner_GitHub.png?raw=true" alt="Werk24">
             </a>
           </p>
         </p>
         
         [![pypi](https://img.shields.io/pypi/v/werk24.svg)](https://pypi.python.org/pypi/werk24)
-        [![Tests | cpython 3.7, 3.8, 3.9](https://github.com/W24-Service-GmbH/werk24-python/actions/workflows/python-test.yml/badge.svg)](https://github.com/W24-Service-GmbH/werk24-python/actions/workflows/python-test.yml)
+        [![Tests | cpython 3.8, 3.9, 3.10](https://github.com/W24-Service-GmbH/werk24-python/actions/workflows/python-test.yml/badge.svg)](https://github.com/W24-Service-GmbH/werk24-python/actions/workflows/python-test.yml)
         
         
         
         # Features
         When submitting a PDF, PNG, JPEG of a Technical Drawing to Werk24's API, you receive within seconds
         the following features:
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: werk24 Version: 1.4.1 Summary: Werk24 Client to
+Metadata-Version: 2.1 Name: werk24 Version: 1.5.0 Summary: Werk24 Client to
 read PDF- and Image-based Technical Drawings / Engineering Drawings Home-page:
 https://werk24.io Author: W24 Service GmbH Author-email: info@werk24.io
 License: commercial Project-URL: Documentation, https://docs.werk24.io/
 Description: # Werk24 Client
                                    [Werk24]
 [![pypi](https://img.shields.io/pypi/v/werk24.svg)](https://pypi.python.org/
-pypi/werk24) [![Tests | cpython 3.7, 3.8, 3.9](https://github.com/W24-Service-
+pypi/werk24) [![Tests | cpython 3.8, 3.9, 3.10](https://github.com/W24-Service-
 GmbH/werk24-python/actions/workflows/python-test.yml/badge.svg)](https://
 github.com/W24-Service-GmbH/werk24-python/actions/workflows/python-test.yml) #
 Features When submitting a PDF, PNG, JPEG of a Technical Drawing to Werk24's
 API, you receive within seconds the following features: - Measures and
 Tolerances - Threads and Chamfers - Geometric Dimensioning and Tolerancing
 frames - External Dimensions - Surface Roughnesses - the Title Block
 information (Material, Drawing ID, Designation, General Tolerances) And finally
```

