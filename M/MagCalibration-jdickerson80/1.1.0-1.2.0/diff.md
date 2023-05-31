# Comparing `tmp/MagCalibration-jdickerson80-1.1.0.tar.gz` & `tmp/MagCalibration-jdickerson80-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MagCalibration-jdickerson80-1.1.0.tar", last modified: Fri Aug 12 15:00:58 2022, max compression
+gzip compressed data, was "MagCalibration-jdickerson80-1.2.0.tar", last modified: Wed May 31 12:16:56 2023, max compression
```

## Comparing `MagCalibration-jdickerson80-1.1.0.tar` & `MagCalibration-jdickerson80-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,43 @@
-drwxrwxr-x   0 jdickerson (26650) jdickerson (26650)        0 2022-08-12 15:00:58.242163 MagCalibration-jdickerson80-1.1.0/
--rw-r--r--   0 jdickerson (26650) jdickerson (26650)     1074 2022-03-18 14:55:23.000000 MagCalibration-jdickerson80-1.1.0/LICENSE.txt
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)      486 2022-08-12 15:00:58.241163 MagCalibration-jdickerson80-1.1.0/PKG-INFO
--rw-r--r--   0 jdickerson (26650) jdickerson (26650)      179 2022-06-28 12:06:53.000000 MagCalibration-jdickerson80-1.1.0/README.md
--rw-r--r--   0 jdickerson (26650) jdickerson (26650)       85 2022-03-18 14:46:57.000000 MagCalibration-jdickerson80-1.1.0/pyproject.toml
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)       38 2022-08-12 15:00:58.242163 MagCalibration-jdickerson80-1.1.0/setup.cfg
--rw-r--r--   0 jdickerson (26650) jdickerson (26650)     1265 2022-08-12 14:59:10.000000 MagCalibration-jdickerson80-1.1.0/setup.py
-drwxrwxr-x   0 jdickerson (26650) jdickerson (26650)        0 2022-08-12 15:00:58.220162 MagCalibration-jdickerson80-1.1.0/src/
-drwxrwxr-x   0 jdickerson (26650) jdickerson (26650)        0 2022-08-12 15:00:58.229163 MagCalibration-jdickerson80-1.1.0/src/MagCalibration_jdickerson80.egg-info/
--rw-r--r--   0 jdickerson (26650) jdickerson (26650)     1074 2022-03-18 14:55:23.000000 MagCalibration-jdickerson80-1.1.0/src/MagCalibration_jdickerson80.egg-info/LICENSE.txt
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)      486 2022-08-12 15:00:58.000000 MagCalibration-jdickerson80-1.1.0/src/MagCalibration_jdickerson80.egg-info/PKG-INFO
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)     1303 2022-08-12 15:00:58.000000 MagCalibration-jdickerson80-1.1.0/src/MagCalibration_jdickerson80.egg-info/SOURCES.txt
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)        1 2022-08-12 15:00:58.000000 MagCalibration-jdickerson80-1.1.0/src/MagCalibration_jdickerson80.egg-info/dependency_links.txt
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)       84 2022-08-12 15:00:58.000000 MagCalibration-jdickerson80-1.1.0/src/MagCalibration_jdickerson80.egg-info/requires.txt
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)       15 2022-08-12 15:00:58.000000 MagCalibration-jdickerson80-1.1.0/src/MagCalibration_jdickerson80.egg-info/top_level.txt
-drwxrwxr-x   0 jdickerson (26650) jdickerson (26650)        0 2022-08-12 15:00:58.230163 MagCalibration-jdickerson80-1.1.0/src/magCalibration/
--rw-r--r--   0 jdickerson (26650) jdickerson (26650)        0 2022-03-18 14:43:37.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/__init__.py
--rw-r--r--   0 jdickerson (26650) jdickerson (26650)   173354 2022-08-12 14:48:05.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/magCalib.py
-drwxrwxr-x   0 jdickerson (26650) jdickerson (26650)        0 2022-08-12 15:00:58.241163 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/
--rw-r--r--   0 jdickerson (26650) jdickerson (26650)        0 2022-01-13 12:14:59.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/__init__.py
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)     4598 2022-03-21 18:48:36.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/aliasPS.py
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)     6513 2022-03-20 16:18:54.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/angles.py
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)     6525 2022-03-20 17:39:46.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/angles_choose.py
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)    13383 2022-04-03 17:41:46.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/autoGold.py
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)     3378 2022-08-12 08:29:56.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/calcStats.py
--rw-r--r--   0 jdickerson (26650) jdickerson (26650)     1044 2022-01-13 12:48:20.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/convertMRC.py
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)     5435 2022-08-08 17:04:41.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/correctAniso.py
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)     9353 2022-03-29 14:39:52.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/getUserAngles.py
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)     4582 2022-03-29 14:39:47.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/getUserBoxes.py
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)     7036 2022-03-29 14:40:05.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/makeAllNWPS_MTF.py
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)     5822 2022-03-29 14:40:01.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/makeAllNWPS_blank.py
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)    12788 2022-03-29 14:40:07.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/makeBlankNPS_ra.py
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)     8595 2022-03-22 10:51:26.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/makeImageNPS_ra.py
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)      776 2022-02-10 18:50:54.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/makeOneUnwhitenedPS.py
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)     1029 2022-01-13 14:30:40.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/makeUnwhitenedPSAll.py
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)     9727 2022-08-12 13:50:03.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/measurePxAllAngles.py
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)    14073 2022-08-12 08:18:00.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/measurePxAvg.py
--rw-r--r--   0 jdickerson (26650) jdickerson (26650)     5423 2022-08-12 14:53:00.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/show_FFT.py
--rw-rw-r--   0 jdickerson (26650) jdickerson (26650)     7330 2022-08-12 13:35:58.000000 MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/smooth_choose.py
+drwxrwxr-x   0 jdickerson (26650) jdickerson (26650)        0 2023-05-31 12:16:56.745506 MagCalibration-jdickerson80-1.2.0/
+-rw-r--r--   0 jdickerson (26650) jdickerson (26650)     1074 2022-03-18 14:55:23.000000 MagCalibration-jdickerson80-1.2.0/LICENSE.txt
+-rw-rw-r--   0 jdickerson (26650) jdickerson (26650)      486 2023-05-31 12:16:56.744506 MagCalibration-jdickerson80-1.2.0/PKG-INFO
+-rw-r--r--   0 jdickerson (26650) jdickerson (26650)      179 2022-06-28 12:06:53.000000 MagCalibration-jdickerson80-1.2.0/README.md
+-rw-r--r--   0 jdickerson (26650) jdickerson (26650)       85 2022-03-18 14:46:57.000000 MagCalibration-jdickerson80-1.2.0/pyproject.toml
+-rw-rw-r--   0 jdickerson (26650) jdickerson (26650)       38 2023-05-31 12:16:56.746506 MagCalibration-jdickerson80-1.2.0/setup.cfg
+-rw-r--r--   0 jdickerson (26650) jdickerson (26650)     1265 2023-05-31 12:13:51.000000 MagCalibration-jdickerson80-1.2.0/setup.py
+drwxrwxr-x   0 jdickerson (26650) jdickerson (26650)        0 2023-05-31 12:16:56.311499 MagCalibration-jdickerson80-1.2.0/src/
+drwxrwxr-x   0 jdickerson (26650) jdickerson (26650)        0 2023-05-31 12:16:56.349500 MagCalibration-jdickerson80-1.2.0/src/MagCalibration_jdickerson80.egg-info/
+-rw-r--r--   0 jdickerson (26650) jdickerson (26650)     1074 2022-03-18 14:55:23.000000 MagCalibration-jdickerson80-1.2.0/src/MagCalibration_jdickerson80.egg-info/LICENSE.txt
+-rw-rw-r--   0 jdickerson (26650) jdickerson (26650)      486 2023-05-31 12:16:56.000000 MagCalibration-jdickerson80-1.2.0/src/MagCalibration_jdickerson80.egg-info/PKG-INFO
+-rw-rw-r--   0 jdickerson (26650) jdickerson (26650)     1493 2023-05-31 12:16:56.000000 MagCalibration-jdickerson80-1.2.0/src/MagCalibration_jdickerson80.egg-info/SOURCES.txt
+-rw-rw-r--   0 jdickerson (26650) jdickerson (26650)        1 2023-05-31 12:16:56.000000 MagCalibration-jdickerson80-1.2.0/src/MagCalibration_jdickerson80.egg-info/dependency_links.txt
+-rw-rw-r--   0 jdickerson (26650) jdickerson (26650)       84 2023-05-31 12:16:56.000000 MagCalibration-jdickerson80-1.2.0/src/MagCalibration_jdickerson80.egg-info/requires.txt
+-rw-rw-r--   0 jdickerson (26650) jdickerson (26650)       15 2023-05-31 12:16:56.000000 MagCalibration-jdickerson80-1.2.0/src/MagCalibration_jdickerson80.egg-info/top_level.txt
+drwxrwxr-x   0 jdickerson (26650) jdickerson (26650)        0 2023-05-31 12:16:56.352500 MagCalibration-jdickerson80-1.2.0/src/magCalibration/
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)        0 2022-11-30 10:49:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/__init__.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)   178320 2023-05-12 16:37:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/magCalib.py
+drwxrwxr-x   0 jdickerson (26650) jdickerson (26650)        0 2023-05-31 12:16:56.726506 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)        0 2022-11-30 10:49:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/__init__.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)     4668 2022-11-30 10:49:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/aliasPS.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)     6513 2022-11-30 10:49:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/angles.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)     6525 2022-11-30 10:49:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/angles_choose.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)    13383 2022-11-30 10:49:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/autoGold.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)     3378 2022-11-30 10:49:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/calcStats.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)     1044 2022-11-30 10:49:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/convertMRC.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)     5435 2022-11-30 10:49:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/correctAniso.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)     9353 2022-11-30 10:49:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/getUserAngles.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)     4582 2022-11-30 10:49:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/getUserBoxes.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)     7036 2022-11-30 10:49:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/makeAllNWPS_MTF.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)     5822 2022-11-30 10:49:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/makeAllNWPS_blank.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)     5808 2022-12-03 17:10:51.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/makeAllNWPS_ignore.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)    12788 2022-11-30 10:49:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/makeBlankNPS_ra.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)    14505 2023-04-11 09:55:23.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/makeIgnoreNPS_ra.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)     8595 2022-11-30 10:49:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/makeImageNPS_ra.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)      776 2022-11-30 10:49:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/makeOneUnwhitenedPS.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)     1029 2022-11-30 10:49:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/makeUnwhitenedPSAll.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)     9823 2022-11-30 10:49:27.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/measurePxAllAngles.py
+-rw-rw-r--   0 jdickerson (26650) jdickerson (26650)    17056 2023-05-18 15:01:05.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/measurePxAvg.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)    17117 2023-05-18 15:01:40.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/measurePxAvg_fit.py
+-rw-rw-r--   0 jdickerson (26650) jdickerson (26650)    14169 2023-03-07 11:16:48.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/measurePxAvg_max.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)     5581 2023-05-19 15:58:20.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/show_FFT.py
+-rwxrwxrwx   0 jdickerson (26650) jdickerson (26650)     7332 2023-05-19 16:03:06.000000 MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/smooth_choose.py
```

### Comparing `MagCalibration-jdickerson80-1.1.0/LICENSE.txt` & `MagCalibration-jdickerson80-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MagCalibration-jdickerson80-1.1.0/setup.py` & `MagCalibration-jdickerson80-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 with open("README.md", 'r', encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="MagCalibration-jdickerson80",
-    version="1.1.0",
+    version="1.2.0",
     author="Joshua L. Dickerson",
     author_email="jdickerson@mrc-lmb.cam.ac.uk",
     description="A program to calibrate the pixel size of cryoEM data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
```

### Comparing `MagCalibration-jdickerson80-1.1.0/src/MagCalibration_jdickerson80.egg-info/LICENSE.txt` & `MagCalibration-jdickerson80-1.2.0/src/MagCalibration_jdickerson80.egg-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MagCalibration-jdickerson80-1.1.0/src/MagCalibration_jdickerson80.egg-info/SOURCES.txt` & `MagCalibration-jdickerson80-1.2.0/src/MagCalibration_jdickerson80.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,19 @@
 src/magCalibration/scripts/calcStats.py
 src/magCalibration/scripts/convertMRC.py
 src/magCalibration/scripts/correctAniso.py
 src/magCalibration/scripts/getUserAngles.py
 src/magCalibration/scripts/getUserBoxes.py
 src/magCalibration/scripts/makeAllNWPS_MTF.py
 src/magCalibration/scripts/makeAllNWPS_blank.py
+src/magCalibration/scripts/makeAllNWPS_ignore.py
 src/magCalibration/scripts/makeBlankNPS_ra.py
+src/magCalibration/scripts/makeIgnoreNPS_ra.py
 src/magCalibration/scripts/makeImageNPS_ra.py
 src/magCalibration/scripts/makeOneUnwhitenedPS.py
 src/magCalibration/scripts/makeUnwhitenedPSAll.py
 src/magCalibration/scripts/measurePxAllAngles.py
 src/magCalibration/scripts/measurePxAvg.py
+src/magCalibration/scripts/measurePxAvg_fit.py
+src/magCalibration/scripts/measurePxAvg_max.py
 src/magCalibration/scripts/show_FFT.py
 src/magCalibration/scripts/smooth_choose.py
```

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/magCalib.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/magCalib.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 from functools import partial
 #sys.path.insert(0, "scripts/")
 
 from magCalibration.scripts import convertMRC
 from magCalibration.scripts import makeUnwhitenedPSAll
 from magCalibration.scripts import makeOneUnwhitenedPS
 from magCalibration.scripts import makeBlankNPS_ra
+from magCalibration.scripts import makeIgnoreNPS_ra
 from magCalibration.scripts import makeAllNWPS_blank
+from magCalibration.scripts import makeAllNWPS_ignore
 from magCalibration.scripts import makeImageNPS_ra
 from magCalibration.scripts import makeAllNWPS_MTF
 from magCalibration.scripts import measurePxAllAngles
 from magCalibration.scripts import correctAniso
 from magCalibration.scripts import aliasPS
 from magCalibration.scripts import measurePxAvg
 from magCalibration.scripts import calcStats
@@ -103,14 +105,15 @@
 anglemin=0
 anglemax=180
 job_number=0
 spectra_dir = "NWPS"
 import_filename = ""
 
 latticeType = "gold-111"
+latticeRes = 2.347
 
 done_import = False
 done_PS = False
 done_Px1 = False
 done_Px2 = False
 
 
@@ -439,18 +442,18 @@
                     print(f"Saved {str(i+1)}/{str(num_tot)} images") 
                     print_text.append(f"Saved {str(i+1)}/{str(num_tot)} images") 
 
         #need to alias the right stuff, is it avg? avg/10? just the newdir???
         #make sure consistent on PS and NWPS as well
         if aliased:
             PS_dir = self.getAliasDir(False)
-            aliasPS.runScript(PS_dir, px_guess, cores)
+            aliasPS.runScript(PS_dir, px_guess, cores, latticeRes)
             if PS_dir.endswith("10/"): #then also do avg
                 PS_dir = self.getAliasDir(True)
-                aliasPS.runScript(PS_dir, px_guess, cores)
+                aliasPS.runScript(PS_dir, px_guess, cores, latticeRes)
             
         '''
         for count, filename in enumerate(file_list):
             fraction_done = round((count/images),2)*100
             print(f"Finished {fraction_done}% of files")
             #self.progress.emit(f"Finished {fraction_done}% of files")
             makeOneUnwhitenedPS.runScript(directory, filename, new_dir)
@@ -458,14 +461,15 @@
 
         #finally write the printText file
         with open(f"{write_dir}outputText.txt", 'a') as f:
             for line in print_text:
                 f.write(f"{line}\n")
         #done_PS = True
         self.finished.emit()
+ 
 
     def getAliasDir(self, second):
         global spectra_dir
         write_dir = self.getJobDir("MakePS")
         NWPS_dir = f"{write_dir}{spectra_dir}/avg/10/"
         file_list = [f for f in os.listdir(NWPS_dir) if f.endswith(".mrc")]
         num_files = len(file_list)
@@ -476,115 +480,131 @@
             images = num_images
         if images < 1:
             NWPS_dir = f"{write_dir}{spectra_dir}/avg/"
         if second == True:
             NWPS_dir = f"{write_dir}{spectra_dir}/avg/"
         return NWPS_dir
 
+    def makeBackgroundSubtractedPS(self):
+        #this is going to noise whiten by the radial profile with the peak removed
+        #print("placeholder for BackgroundSubtraction")
+        global spectra_dir
+        spectra_dir = "powerSpectra"
+        write_dir = self.getJobDir("MakePS") 
+        makeIgnoreNPS_ra.runScript(directory, cores, False, write_dir, px_guess, latticeType, latticeRes, temperature, num_images)
+        makeAllNWPS_ignore.runScript(directory, cores, spectra_dir, write_dir, num_images)
+        if aliased:
+            NWPS_dir = self.getAliasDir(False)
+            aliasPS.runScript(NWPS_dir, px_guess, cores, latticeRes)
+            if NWPS_dir.endswith("10/"): #then also do avg
+                NWPS_dir = self.getAliasDir(True)
+                aliasPS.runScript(NWPS_dir, px_guess, cores, latticeRes)
+        self.finished.emit()
+
     def makeBlankNoisePowerSpectrumWorker(self):
         global spectra_dir
         spectra_dir = "NWPS"
         write_dir = self.getJobDir("MakePS") 
         makeBlankNPS_ra.runScript(blank_directory, cores, False, write_dir)
         makeAllNWPS_blank.runScript(directory, blank_directory, cores, spectra_dir, write_dir, num_images)
         if aliased:
             NWPS_dir = self.getAliasDir(False)
-            aliasPS.runScript(NWPS_dir, px_guess, cores)
+            aliasPS.runScript(NWPS_dir, px_guess, cores, latticeRes)
             if NWPS_dir.endswith("10/"): #then also do avg
                 NWPS_dir = self.getAliasDir(True)
-                aliasPS.runScript(NWPS_dir, px_guess, cores)
+                aliasPS.runScript(NWPS_dir, px_guess, cores, latticeRes)
         self.finished.emit()
 
     def makeAngleNoisePowerSpectrumWorker(self):
         global spectra_dir
         spectra_dir = "NWPS"
         write_dir = self.getJobDir("MakePS")
         makeImageNPS_ra.runScript(blank_directory, cores, True, False, write_dir)
         makeAllNWPS_blank.runScript(directory, write_dir, cores, spectra_dir, write_dir, num_images)
         if aliased:
             NWPS_dir = self.getAliasDir(False)
-            aliasPS.runScript(NWPS_dir, px_guess, cores)
+            aliasPS.runScript(NWPS_dir, px_guess, cores, latticeRes)
             if NWPS_dir.endswith("10/"): #then also do avg
                 NWPS_dir = self.getAliasDir(True)
-                aliasPS.runScript(NWPS_dir, px_guess, cores)
+                aliasPS.runScript(NWPS_dir, px_guess, cores, latticeRes)
         self.finished.emit()
 
     def makeCropNoisePowerSpectrumWorker(self):
         global spectra_dir
         spectra_dir = "NWPS"
         write_dir = self.getJobDir("MakePS")
         makeImageNPS_ra.runScript(blank_directory, cores, False, True, write_dir)
         makeAllNWPS_blank.runScript(directory, write_dir, cores, spectra_dir, write_dir, num_images)
         if aliased:
             NWPS_dir = self.getAliasDir(False)
-            aliasPS.runScript(NWPS_dir, px_guess, cores)
+            aliasPS.runScript(NWPS_dir, px_guess, cores, latticeRes)
             if NWPS_dir.endswith("10/"): #then also do avg
                 NWPS_dir = self.getAliasDir(True)
-                aliasPS.runScript(NWPS_dir, px_guess, cores)
+                aliasPS.runScript(NWPS_dir, px_guess, cores, latticeRes)
         self.finished.emit()
 
     def makeCropAngleNoisePowerSpectrumWorker(self):
         global spectra_dir
         spectra_dir = "NWPS"
         write_dir = self.getJobDir("MakePS")
         makeImageNPS_ra.runScript(blank_directory, cores, True, True, write_dir)
         makeAllNWPS_blank.runScript(directory, write_dir, cores, spectra_dir, write_dir, num_images)
         if aliased:
             NWPS_dir = self.getAliasDir(False)
-            aliasPS.runScript(NWPS_dir, px_guess, cores)
+            aliasPS.runScript(NWPS_dir, px_guess, cores, latticeRes)
             if NWPS_dir.endswith("10/"): #then also do avg
                 NWPS_dir = self.getAliasDir(True)
-                aliasPS.runScript(NWPS_dir, px_guess, cores)
+                aliasPS.runScript(NWPS_dir, px_guess, cores, latticeRes)
         self.finished.emit()
 
     def makeMTFNWPSWorker(self):
         global spectra_dir
         spectra_dir = "NWPS"
         write_dir = self.getJobDir("MakePS")
         makeAllNWPS_MTF.runScript(directory, blank_directory, px_guess, cores, spectra_dir, write_dir, num_images)
         if aliased:
             NWPS_dir = self.getAliasDir(False)
-            aliasPS.runScript(NWPS_dir, px_guess, cores)
+            aliasPS.runScript(NWPS_dir, px_guess, cores, latticeRes)
             if NWPS_dir.endswith("10/"): #then also do avg
                 NWPS_dir = self.getAliasDir(True)
-                aliasPS.runScript(NWPS_dir, px_guess, cores)
+                aliasPS.runScript(NWPS_dir, px_guess, cores, latticeRes)
         self.finished.emit()
 
     def measureAniso(self):
         #I need a flag for aliased here 
         write_dir = self.getJobDir("MeasureAniso")
-        measurePxAllAngles.runScript(directory, temperature, px_guess, cores, aliased, spectra_dir, ps_dir, write_dir, latticeType)
+        measurePxAllAngles.runScript(directory, temperature, px_guess, cores, aliased, spectra_dir, ps_dir, write_dir, latticeType, latticeRes)
         self.finished.emit()
 
     def correctAniso(self):
         global aniso_corrected
         write_dir = self.getJobDir("CorrectAniso")
         correctAniso.runScript(directory, cores, spectra_dir, aliased, ps_dir, write_dir, aniso_param, True)
         if aliased == False:
             correctAniso.runScript(directory, cores, spectra_dir, aliased, ps_dir2, write_dir, aniso_param, False)
         aniso_corrected=True
         self.finished.emit()
 
     def measurePxAvgWorker(self):
         write_dir = self.getJobDir("MeasurePx")
-        measurePxAvg.runScript(directory, px_guess, temperature, cores, savgol_window2, supervised_angle, aliased, aniso_corrected, spectra_dir, write_dir, ps_dir, latticeType, supervised_smooth, True)
+        measurePxAvg.runScript(directory, px_guess, temperature, cores, savgol_window2, supervised_angle, aliased, aniso_corrected, spectra_dir, write_dir, ps_dir, latticeType, supervised_smooth, True, latticeRes)
         if aliased == False:
-            measurePxAvg.runScript(directory, px_guess, temperature, cores, savgol_window2, supervised_angle, aliased, aniso_corrected, spectra_dir, write_dir, ps_dir2, latticeType, supervised_smooth, False)
+            measurePxAvg.runScript(directory, px_guess, temperature, cores, savgol_window2, supervised_angle, aliased, aniso_corrected, spectra_dir, write_dir, ps_dir2, latticeType, supervised_smooth, False, latticeRes)
             #get stats if aniso need to adjust
             #calcStats.runScript(directory, aniso_corrected, spectra_dir, write_dir, aniso_param)
             calcStats.runScript(directory, spectra_dir, write_dir, aniso_param)
             #done_Px1 = True
         self.finished.emit()
 
     def measurePxAvgWorkerAuto(self, avgImage):
         this_ps_dir = ps_dir
         if avgImage == False:
             this_ps_dir = ps_dir2
         write_dir = self.getJobDir("MeasurePx")
-        measurePxAvg.runScript(directory, px_guess, temperature, cores, savgol_window2, supervised_angle, aliased, aniso_corrected, spectra_dir, write_dir, this_ps_dir, latticeType, supervised_smooth, avgImage)
+        measurePxAvg.runScript(directory, px_guess, temperature, cores, savgol_window2, supervised_angle, aliased, aniso_corrected, spectra_dir, write_dir, this_ps_dir, latticeType, supervised_smooth, avgImage, latticeRes)
         if avgImage == False:
             calcStats.runScript(directory, spectra_dir, write_dir, aniso_param)
 
     def writeProjectFileWorker(self, job_name, job_alias, job_string):
         #_translate = QtCore.QCoreApplication.translate
 
         #write new job to file
@@ -608,16 +628,17 @@
         method = "none"
         method2 = "none"
         job_alias = "noNW"
         job_name = "MakePS"     
         job_string = str(job_number)
         job_string = job_string.rjust(3,'0')
         cores = 4
-        print("Calculating power spectra without noise whitening")
+        #print("Calculating power spectra with background subtraction")
         self.makeNotWhitePS()
+        #self.makeBackgroundSubtractedPS()
         print_text.append("Power spectra calculation complete")
         writeMethod = method2.replace(" ", "_")
         #write to project file
 
         self.writeProjectFileWorker(job_name, job_alias, job_string)
             
         #write what the input was, where the output is maybe as well
@@ -1166,29 +1187,37 @@
         self.label_latticeType.setObjectName("label_latticeType")
         self.formLayout_3.setWidget(4, QtWidgets.QFormLayout.LabelRole, self.label_latticeType)
         self.comboBox_latticeType = QtWidgets.QComboBox(self.formLayoutWidget_3)
         self.comboBox_latticeType.setObjectName("comboBox_latticeType")
         self.comboBox_latticeType.addItem("")
         self.comboBox_latticeType.addItem("")
         self.comboBox_latticeType.addItem("")
+        self.comboBox_latticeType.addItem("")
         self.formLayout_3.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.comboBox_latticeType)
+
+        self.label_latticeConstant = QtWidgets.QLabel(self.formLayoutWidget_3)
+        self.label_latticeConstant.setObjectName("label_latticeConstant")
+        self.formLayout_3.setWidget(5, QtWidgets.QFormLayout.LabelRole, self.label_latticeConstant)
+        self.lineEdit_latticeConstant = QtWidgets.QLineEdit(self.formLayoutWidget_3)
+        self.lineEdit_latticeConstant.setObjectName("lineEdit_imageSubset")
+        self.formLayout_3.setWidget(5, QtWidgets.QFormLayout.FieldRole, self.lineEdit_latticeConstant)
         
 
         self.label_imageSubset = QtWidgets.QLabel(self.formLayoutWidget_3)
         self.label_imageSubset.setObjectName("label_imageSubset")
-        self.formLayout_3.setWidget(5, QtWidgets.QFormLayout.LabelRole, self.label_imageSubset)
+        self.formLayout_3.setWidget(6, QtWidgets.QFormLayout.LabelRole, self.label_imageSubset)
         self.lineEdit_imageSubset = QtWidgets.QLineEdit(self.formLayoutWidget_3)
         self.lineEdit_imageSubset.setObjectName("lineEdit_imageSubset")
-        self.formLayout_3.setWidget(5, QtWidgets.QFormLayout.FieldRole, self.lineEdit_imageSubset)
+        self.formLayout_3.setWidget(6, QtWidgets.QFormLayout.FieldRole, self.lineEdit_imageSubset)
 
 
 
         self.label_NW = QtWidgets.QLabel(self.formLayoutWidget_3)
         self.label_NW.setObjectName("label_NW")
-        self.formLayout_3.setWidget(7, QtWidgets.QFormLayout.LabelRole, self.label_NW)
+        self.formLayout_3.setWidget(8, QtWidgets.QFormLayout.LabelRole, self.label_NW)
         self.horizontalLayout_NW = QtWidgets.QHBoxLayout()
         self.horizontalLayout_NW.setSpacing(6)
         self.horizontalLayout_NW.setObjectName("horizontalLayout_NW")
         self.radioButton_aniso_yes_2 = QtWidgets.QRadioButton(self.formLayoutWidget_3)
         self.radioButton_aniso_yes_2.setObjectName("radioButton_aniso_yes_2")
         self.buttonGroup_2 = QtWidgets.QButtonGroup(self)
         self.buttonGroup_2.setObjectName("buttonGroup_2")
@@ -1196,52 +1225,52 @@
         self.radioButton_aniso_yes_2.setChecked(True)
         self.horizontalLayout_NW.addWidget(self.radioButton_aniso_yes_2)
         self.radioButton_aniso_no_2 = QtWidgets.QRadioButton(self.formLayoutWidget_3)
         #self.radioButton_aniso_no_2.setChecked(True)
         self.radioButton_aniso_no_2.setObjectName("radioButton_aniso_no_2")
         self.buttonGroup_2.addButton(self.radioButton_aniso_no_2)
         self.horizontalLayout_NW.addWidget(self.radioButton_aniso_no_2)
-        self.formLayout_3.setLayout(7, QtWidgets.QFormLayout.FieldRole, self.horizontalLayout_NW)
+        self.formLayout_3.setLayout(8, QtWidgets.QFormLayout.FieldRole, self.horizontalLayout_NW)
         self.label_method = QtWidgets.QLabel(self.formLayoutWidget_3)
         self.label_method.setObjectName("label_method")
-        self.formLayout_3.setWidget(8, QtWidgets.QFormLayout.LabelRole, self.label_method)
+        self.formLayout_3.setWidget(9, QtWidgets.QFormLayout.LabelRole, self.label_method)
         self.comboBox_method = QtWidgets.QComboBox(self.formLayoutWidget_3)
         self.comboBox_method.setObjectName("comboBox_method")
         self.comboBox_method.addItem("")
         self.comboBox_method.addItem("")
         self.comboBox_method.addItem("")
         self.comboBox_method.addItem("")
         self.comboBox_method.addItem("")
-        self.formLayout_3.setWidget(8, QtWidgets.QFormLayout.FieldRole, self.comboBox_method)
+        self.formLayout_3.setWidget(9, QtWidgets.QFormLayout.FieldRole, self.comboBox_method)
         self.label_white_directory = QtWidgets.QLabel(self.formLayoutWidget_3)
         self.label_white_directory.setObjectName("label_white_directory")
-        self.formLayout_3.setWidget(9, QtWidgets.QFormLayout.LabelRole, self.label_white_directory)
+        self.formLayout_3.setWidget(10, QtWidgets.QFormLayout.LabelRole, self.label_white_directory)
 
         self.label_cores = QtWidgets.QLabel(self.formLayoutWidget_3)
         self.label_cores.setObjectName("label_cores")
-        self.formLayout_3.setWidget(12, QtWidgets.QFormLayout.LabelRole, self.label_cores)
+        self.formLayout_3.setWidget(13, QtWidgets.QFormLayout.LabelRole, self.label_cores)
         self.lineEdit_cores = QtWidgets.QLineEdit(self.formLayoutWidget_3)
         self.lineEdit_cores.setObjectName("lineEdit_cores")
-        self.formLayout_3.setWidget(12, QtWidgets.QFormLayout.FieldRole, self.lineEdit_cores)
+        self.formLayout_3.setWidget(13, QtWidgets.QFormLayout.FieldRole, self.lineEdit_cores)
 
         
         
         self.label_importJob = QtWidgets.QLabel(self.formLayoutWidget_3)
         self.label_importJob.setObjectName("label_importJob")
-        self.formLayout_3.setWidget(6, QtWidgets.QFormLayout.LabelRole, self.label_importJob)
+        self.formLayout_3.setWidget(7, QtWidgets.QFormLayout.LabelRole, self.label_importJob)
         self.horizontalLayout_8 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_8.setSpacing(6)
         self.horizontalLayout_8.setObjectName("horizontalLayout_8")
         self.comboBox_importJob = QtWidgets.QComboBox(self.formLayoutWidget_3)
         self.comboBox_importJob.setObjectName("comboBox_importJob")
         self.horizontalLayout_8.addWidget(self.comboBox_importJob)
         #self.pushButton_browser_importJob = QtWidgets.QPushButton(self.formLayoutWidget_3)
         #self.pushButton_browser_importJob.setObjectName("pushButton_browser_importJob")
         #self.horizontalLayout_8.addWidget(self.pushButton_browser_importJob)
-        self.formLayout_3.setLayout(6, QtWidgets.QFormLayout.FieldRole, self.horizontalLayout_8)
+        self.formLayout_3.setLayout(7, QtWidgets.QFormLayout.FieldRole, self.horizontalLayout_8)
 
 
 
 
         self.horizontalLayout_6 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_6.setSpacing(6)
         self.horizontalLayout_6.setObjectName("horizontalLayout_6")
@@ -1257,95 +1286,95 @@
         self.horizontalLayout_7.setObjectName("horizontalLayout_7")
         self.lineEdit_white_filepath = QtWidgets.QLineEdit(self.formLayoutWidget_3)
         self.lineEdit_white_filepath.setObjectName("lineEdit_white_filepath")
         self.horizontalLayout_7.addWidget(self.lineEdit_white_filepath)
         self.pushButton_browser_2 = QtWidgets.QPushButton(self.formLayoutWidget_3)
         self.pushButton_browser_2.setObjectName("pushButton_browser_2")
         self.horizontalLayout_7.addWidget(self.pushButton_browser_2)
-        self.formLayout_3.setLayout(9, QtWidgets.QFormLayout.FieldRole, self.horizontalLayout_7)
+        self.formLayout_3.setLayout(10, QtWidgets.QFormLayout.FieldRole, self.horizontalLayout_7)
 
 
 
         self.label_MakePSJob = QtWidgets.QLabel(self.formLayoutWidget_3)
         self.label_MakePSJob.setObjectName("label_MakePSJob")
-        self.formLayout_3.setWidget(10, QtWidgets.QFormLayout.LabelRole, self.label_MakePSJob)
+        self.formLayout_3.setWidget(11, QtWidgets.QFormLayout.LabelRole, self.label_MakePSJob)
         self.horizontalLayout_9 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_9.setSpacing(6)
         self.horizontalLayout_9.setObjectName("horizontalLayout_9")
         #self.lineEdit_MakePSJob = QtWidgets.QLineEdit(self.formLayoutWidget_3)
         #self.lineEdit_MakePSJob.setObjectName("lineEdit_MakePSJob")
         #self.horizontalLayout_9.addWidget(self.lineEdit_MakePSJob)
         self.comboBox_MakePSJob = QtWidgets.QComboBox(self.formLayoutWidget_3)
         self.comboBox_MakePSJob.setObjectName("comboBox_MakePSJob")
         self.horizontalLayout_9.addWidget(self.comboBox_MakePSJob)
         #self.pushButton_browser_importPS = QtWidgets.QPushButton(self.formLayoutWidget_3)
         #self.pushButton_browser_importPS.setObjectName("pushButton_browser_importPS")
         #self.horizontalLayout_9.addWidget(self.pushButton_browser_importPS)
-        self.formLayout_3.setLayout(10, QtWidgets.QFormLayout.FieldRole, self.horizontalLayout_9)
+        self.formLayout_3.setLayout(11, QtWidgets.QFormLayout.FieldRole, self.horizontalLayout_9)
 
         self.label_AnisoParams = QtWidgets.QLabel(self.formLayoutWidget_3)
         self.label_AnisoParams.setObjectName("label_AnisoParams")
-        self.formLayout_3.setWidget(11, QtWidgets.QFormLayout.LabelRole, self.label_AnisoParams)
+        self.formLayout_3.setWidget(12, QtWidgets.QFormLayout.LabelRole, self.label_AnisoParams)
         self.horizontalLayout_10 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_10.setSpacing(6)
         self.horizontalLayout_10.setObjectName("horizontalLayout_10")
         #self.lineEdit_AnisoParams = QtWidgets.QLineEdit(self.formLayoutWidget_3)
         #self.lineEdit_AnisoParams.setObjectName("lineEdit_AnisoParams")
         #self.horizontalLayout_10.addWidget(self.lineEdit_AnisoParams)
         self.comboBox_AnisoParams = QtWidgets.QComboBox(self.formLayoutWidget_3)
         self.comboBox_AnisoParams.setObjectName("comboBox_AnisoParams")
         self.horizontalLayout_10.addWidget(self.comboBox_AnisoParams)
         #self.pushButton_browser_AnisoParams = QtWidgets.QPushButton(self.formLayoutWidget_3)
         #self.pushButton_browser_AnisoParams.setObjectName("pushButton_browser_AnisoParams")
         #self.horizontalLayout_10.addWidget(self.pushButton_browser_AnisoParams)
-        self.formLayout_3.setLayout(11, QtWidgets.QFormLayout.FieldRole, self.horizontalLayout_10)
+        self.formLayout_3.setLayout(12, QtWidgets.QFormLayout.FieldRole, self.horizontalLayout_10)
 
 
         self.label_smooth_choose = QtWidgets.QLabel(self.formLayoutWidget_3)
         self.label_smooth_choose.setObjectName("label_smooth_choose")
-        self.formLayout_3.setWidget(13, QtWidgets.QFormLayout.LabelRole, self.label_smooth_choose)
+        self.formLayout_3.setWidget(14, QtWidgets.QFormLayout.LabelRole, self.label_smooth_choose)
         self.horizontalLayout_5 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_5.setSpacing(6)
         self.horizontalLayout_5.setObjectName("horizontalLayout_5")
         self.radioButton_smooth_yes = QtWidgets.QRadioButton(self.formLayoutWidget_3)
         self.radioButton_smooth_yes.setObjectName("radioButton_smooth_yes")
         self.buttonGroup_4 = QtWidgets.QButtonGroup(self)
         self.buttonGroup_4.setObjectName("buttonGroup_4")
         self.buttonGroup_4.addButton(self.radioButton_smooth_yes)
         self.horizontalLayout_5.addWidget(self.radioButton_smooth_yes)
         self.radioButton_smooth_no = QtWidgets.QRadioButton(self.formLayoutWidget_3)
         self.radioButton_smooth_no.setChecked(True)
         self.radioButton_smooth_no.setObjectName("radioButton_smooth_no")
         self.buttonGroup_4.addButton(self.radioButton_smooth_no)
         self.horizontalLayout_5.addWidget(self.radioButton_smooth_no)
-        self.formLayout_3.setLayout(13, QtWidgets.QFormLayout.FieldRole, self.horizontalLayout_5)
+        self.formLayout_3.setLayout(14, QtWidgets.QFormLayout.FieldRole, self.horizontalLayout_5)
         self.label_smooth = QtWidgets.QLabel(self.formLayoutWidget_3)
         self.label_smooth.setObjectName("label_smooth")
-        self.formLayout_3.setWidget(14, QtWidgets.QFormLayout.LabelRole, self.label_smooth)
+        self.formLayout_3.setWidget(15, QtWidgets.QFormLayout.LabelRole, self.label_smooth)
         self.lineEdit_smooth = QtWidgets.QLineEdit(self.formLayoutWidget_3)
         self.lineEdit_smooth.setObjectName("lineEdit_smooth")
-        self.formLayout_3.setWidget(14, QtWidgets.QFormLayout.FieldRole, self.lineEdit_smooth)
+        self.formLayout_3.setWidget(15, QtWidgets.QFormLayout.FieldRole, self.lineEdit_smooth)
         self.label_angle = QtWidgets.QLabel(self.formLayoutWidget_3)
         self.label_angle.setObjectName("label_angle")
-        self.formLayout_3.setWidget(15, QtWidgets.QFormLayout.LabelRole, self.label_angle)
+        self.formLayout_3.setWidget(16, QtWidgets.QFormLayout.LabelRole, self.label_angle)
         self.horizontalLayout_4 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_4.setSpacing(6)
         self.horizontalLayout_4.setObjectName("horizontalLayout_4")
         self.radioButton_angle_yes = QtWidgets.QRadioButton(self.formLayoutWidget_3)
         self.radioButton_angle_yes.setObjectName("radioButton_angle_yes")
         self.buttonGroup_3 = QtWidgets.QButtonGroup(self)
         self.buttonGroup_3.setObjectName("buttonGroup_3")
         self.buttonGroup_3.addButton(self.radioButton_angle_yes)
         self.horizontalLayout_4.addWidget(self.radioButton_angle_yes)
         self.radioButton_angle_no = QtWidgets.QRadioButton(self.formLayoutWidget_3)
         self.radioButton_angle_no.setChecked(True)
         self.radioButton_angle_no.setObjectName("radioButton_angle_no")
         self.buttonGroup_3.addButton(self.radioButton_angle_no)
         self.horizontalLayout_4.addWidget(self.radioButton_angle_no)
-        self.formLayout_3.setLayout(15, QtWidgets.QFormLayout.FieldRole, self.horizontalLayout_4)
+        self.formLayout_3.setLayout(16, QtWidgets.QFormLayout.FieldRole, self.horizontalLayout_4)
         self.pushButton_Correct = QtWidgets.QPushButton(self.centralWidget)
         self.pushButton_Correct.setGeometry(QtCore.QRect(450, 565, 158, 33))
         palette = QtGui.QPalette()
         brush = QtGui.QBrush(QtGui.QColor(255, 255, 255))
         brush.setStyle(QtCore.Qt.SolidPattern)
         palette.setBrush(QtGui.QPalette.Active, QtGui.QPalette.WindowText, brush)
         brush = QtGui.QBrush(QtGui.QColor(106, 59, 119))
@@ -1687,14 +1716,15 @@
         self.listWidget.currentRowChanged.connect(self.listWidgetClicked)
         self.listWidget_jobs.currentRowChanged.connect(self.listWidgetJobsClicked)
         self.radioButton_smooth_no.toggled.connect(self.noSmoothchecked)
         self.radioButton_smooth_yes.toggled.connect(self.Smoothchecked)
         self.radioButton_aniso_no_2.toggled.connect(self.noiseWhitenNo)
         self.radioButton_aniso_yes_2.toggled.connect(self.noiseWhitenYes)
         self.comboBox_method.currentIndexChanged.connect(self.comboBoxMethodChanged)
+        self.comboBox_latticeType.currentIndexChanged.connect(self.comboBoxLatticeChanged)
         self.pushButton_Run.clicked.connect(self.runButtonClicked)
         self.pushButton_failed.clicked.connect(self.failedButtonClicked)
         self.pushButton_delete.clicked.connect(self.deleteButtonClicked)
         self.actionExit.triggered.connect(self.exitButtonClicked)
         self.actionOpen.triggered.connect(self.openButtonClicked)
         self.actionNew.triggered.connect(self.newButtonClicked)
         self.actionAbout.triggered.connect(self.aboutButtonClicked)
@@ -1741,14 +1771,17 @@
         self.comboBox_type.setItemText(0, _translate("MainWindow", "MRC"))
         self.comboBox_type.setItemText(1, _translate("MainWindow", "DM4"))
         self.comboBox_type.setItemText(2, _translate("MainWindow", "DM3"))
         self.comboBox_type.setItemText(3, _translate("MainWindow", "TIFF"))
         self.comboBox_latticeType.setItemText(0, _translate("MainWindow", "gold-111"))
         self.comboBox_latticeType.setItemText(1, _translate("MainWindow", "gold-200"))
         self.comboBox_latticeType.setItemText(2, _translate("MainWindow", "graphitized-carbon"))
+        self.comboBox_latticeType.setItemText(3, _translate("MainWindow", "define_lattice_constant"))
+        self.label_latticeConstant.setToolTip(_translate("MainWindow", "Enter your own lattice resolution"))
+        self.label_latticeConstant.setText(_translate("MainWindow", "Lattice Resolution (" + u"\u212B" +")"))
         self.label_temperture.setToolTip(_translate("MainWindow", "Sample temperature in Kelvin"))
         self.label_temperture.setText(_translate("MainWindow", "Temperature (K)"))
         self.lineEdit_temperature.setText(_translate("MainWindow", "80"))
         self.label_temperture_2.setToolTip(_translate("MainWindow", "Your best guess of your pixel size in " + u"\u212B"))
         self.label_temperture_2.setText(_translate("MainWindow", "Pixel size estimate (" + u"\u212B" +")"))
         self.lineEdit_px.setText(_translate("MainWindow", "0.67"))
         self.lineEdit_imageSubset.setText(_translate("MainWindow", "-1"))
@@ -1820,14 +1853,16 @@
 
         print("Welcome to the development version of MagCalibration")
 
     def initialHiding(self):
         self.hideMakePS(False)
         self.hideAniso(False)
         self.hidePix(False)
+        self.lineEdit_latticeConstant.setVisible(False)
+        self.label_latticeConstant.setVisible(False)
     
     def hideMakePS(self, show):
         self.label_NW.setVisible(show)
         self.radioButton_aniso_yes_2.setVisible(show)
         self.radioButton_aniso_no_2.setVisible(show)
         self.label_cores.setVisible(show)
         self.lineEdit_cores.setVisible(show)
@@ -1947,14 +1982,27 @@
         self.pushButton_RunAll.setVisible(show)
 
         self.label_filetype_2.setVisible(show)
         self.comboBox_type.setVisible(show)
         self.label_latticeType.setVisible(show)
         self.comboBox_latticeType.setVisible(show)
 
+        if show:
+            #get idx
+            idx = self.comboBox_latticeType.currentIndex()
+            if idx == 3:
+                self.label_latticeConstant.setVisible(show)
+                self.lineEdit_latticeConstant.setVisible(show)
+            else:
+                self.label_latticeConstant.setVisible(False)
+                self.lineEdit_latticeConstant.setVisible(False)
+        else:
+            self.label_latticeConstant.setVisible(show)
+            self.lineEdit_latticeConstant.setVisible(show)
+
         self.label_temperture.setVisible(show)
         self.lineEdit_temperature.setVisible(show)
 
         self.label_temperture_2.setVisible(show)
         self.lineEdit_px.setVisible(show)
 
         self.label_imageSubset.setVisible(show)
@@ -1987,15 +2035,15 @@
         cursor = self.plainTextEdit.textCursor()
         cursor.movePosition(QtGui.QTextCursor.End)
         cursor.insertText(text)
         self.plainTextEdit.setTextCursor(cursor)
         self.plainTextEdit.ensureCursorVisible()
 
     def listWidgetJobsClicked(self):
-        global temperature, directory, fileType, px_guess,cores, latticeType
+        global temperature, directory, fileType, px_guess,cores, latticeType, latticeRes
         item = self.listWidget_jobs.currentItem()
         #print(item.text())
         texts = []
         this_path = []
         split_path = []
         if item is not None:
             texts = item.text().split(' ')
@@ -2043,14 +2091,23 @@
                             if index >= 0:
                                 self.comboBox_type.setCurrentIndex(index)
                         elif field == "LatticeType":
                             latticeType = field2
                             index = self.comboBox_latticeType.findText(latticeType, QtCore.Qt.MatchFixedString)
                             if index >= 0:
                                 self.comboBox_latticeType.setCurrentIndex(index)
+                            if index == 3:
+                                self.label_latticeConstant.setVisible(True)
+                                self.lineEdit_latticeConstant.setVisible(True)
+                            else:
+                                self.label_latticeConstant.setVisible(False)
+                                self.lineEdit_latticeConstant.setVisible(False)
+                        elif field == "LatticeRes":
+                            latticeRes = float(field2)
+                            self.lineEdit_latticeConstant.setText(field2)
                 self.hideAniso(False)
                 self.hidePix(False)
                 self.hideMakePS(False)
                 self.hideImport(True)
             elif split_path[0] == "MakePS":
                 self.listWidget.setCurrentRow(1)
                 with open(f"{proj_directory}{this_path}/makePSInput.txt", 'r') as f:
@@ -2319,19 +2376,21 @@
                 else:
                     self.label_white_directory.setText("Blank/ice image directory")
             #else:
                 #self.label_white_directory.setVisible(False)
                 #self.lineEdit_white_filepath.setVisible(False)
                 #self.pushButton_browser_2.setVisible(False) 
              '''
-    def comboBoxMethodChanged(self, value):
-        if value == 4:
-            self.label_white_directory.setText("MTF file")
+    def comboBoxLatticeChanged(self, value):
+        if value == 3:
+            self.label_latticeConstant.setVisible(True)
+            self.lineEdit_latticeConstant.setVisible(True)
         else:
-            self.label_white_directory.setText("Blank/ice image directory")
+            self.label_latticeConstant.setVisible(False)
+            self.lineEdit_latticeConstant.setVisible(False)
         '''
         if value == 0 or value == 4:
             #self.label_white_directory.setVisible(True)
             #self.lineEdit_white_filepath.setVisible(True)
             #self.pushButton_browser_2.setVisible(True) 
             if value == 4:
                 self.label_white_directory.setText("MTF file")
@@ -2339,14 +2398,20 @@
                 self.label_white_directory.setText("Blank/ice image directory")
         #else:
             #self.label_white_directory.setVisible(False)
             #self.lineEdit_white_filepath.setVisible(False)
             #self.pushButton_browser_2.setVisible(False)
          '''
 
+    def comboBoxMethodChanged(self, value):
+        if value == 4:
+            self.label_white_directory.setText("MTF file")
+        else:
+            self.label_white_directory.setText("Blank/ice image directory")
+
     
     #def exitButtonClicked(self):
         #sys.stdout = sys.__stdout__
         #sys.exit()
 
 
     def resetAndClear(self):
@@ -2627,19 +2692,20 @@
             
         #append new job to items
         item = QtWidgets.QListWidgetItem()
         self.listWidget_jobs.addItem(item)
         #item = self.listWidget_jobs.item(job_number-1)
         #item.setText(_translate("MainWindow", f"{job_string}: {job_name}/job{job_string}")) 
         item.setText(f"{job_string}: {job_name}/job{job_string} {job_alias}") 
+        
 
     def doImportNoWorker(self):
         print_text = []
         input_okay = True
-        global temperature, directory, fileType, px_guess, aliased, aniso_corrected, job_number, num_images, latticeType, import_filename
+        global temperature, directory, fileType, px_guess, aliased, aniso_corrected, job_number, num_images, latticeType, import_filename, latticeRes
         job_string = ""
         aniso_corrected = False #also needs to be reset
 
         print("Importing data")
         print_text.append("Importing data")
         directory = self.lineEdit_image_filename_2.text().strip()
         if directory == "":
@@ -2673,22 +2739,30 @@
             #this needs to be changed based on lattice type
             gold_lattice_param = temperature*5.67075E-5 + 4.06111 #A 
             goldLattice_111 = gold_lattice_param / (1**2+1**2+1**2)**0.5
             goldLattice_200 = gold_lattice_param / (2**2)**0.5
             #gc_res = 3.3378
             gc_res = 3.434
             print_text.append(f"Lattice type is {latticeType}")
-            lattice_res = goldLattice_111
+            latticeRes = goldLattice_111
             if latticeType == "gold-111":
-                lattice_res = goldLattice_111
+                latticeRes = goldLattice_111
             elif latticeType == "gold-200":
-                lattice_res = goldLattice_200
+                latticeRes = goldLattice_200
             elif latticeType == "graphitized-carbon":
-                lattice_res = gc_res
-            if px_guess >= lattice_res/2:
+                latticeRes = gc_res
+            elif latticeType == "define_lattice_constant":
+                try:
+                    latticeRes = float(self.lineEdit_latticeConstant.text())
+                except ValueError:
+                    print("Error: Lattice constant must be a number")
+                    print_text.append("Error: Lattice constant must be a number")
+                    input_okay = False
+                
+            if px_guess >= latticeRes/2:
                 aliased = True
             else:
                 aliased = False
             if fileType != "mrc":
                 print(f"Converting all {fileType} to MRC")
                 print_text.append(f"Converting all {fileType} to MRC")
                 convertMRC.runConvert(directory, fileType)
@@ -2713,14 +2787,15 @@
                 f.write(f"DataDirectory:{directory}\n")
                 f.write(f"FileType:{fileType}\n")
                 f.write(f"Temperature:{str(temperature)}\n")
                 f.write(f"PxGuess:{str(px_guess)}\n")
                 f.write(f"Aliased:{str(aliased)}\n")
                 f.write(f"Images:{str(num_images)}\n")
                 f.write(f"LatticeType:{latticeType}\n")
+                f.write(f"LatticeRes:{latticeRes}\n")
 
             print("Data import complete")
             print_text.append("Data import complete")
 
         #set the PS input as this import file as default
         import_filename = f"{proj_directory}Import/job{job_string}/import_vals.txt"
         #self.lineEdit_importJob.setText(import_filename)
@@ -2730,19 +2805,20 @@
             self.comboBox_importJob.setCurrentIndex(index)
 
         #finally write the printText file
         with open(f"{proj_directory}Import/job{job_string}/outputText.txt", 'a') as f:
             for line in print_text:
                 f.write(f"{line}\n")
 
+    
 
     def doImport(self):
         print_text = []
         input_okay = True
-        global temperature, directory, fileType, px_guess, aliased, aniso_corrected, job_number, num_images, latticeType, done_import
+        global temperature, directory, fileType, px_guess, aliased, aniso_corrected, job_number, num_images, latticeType, done_import, latticeRes
         job_string = ""
         aniso_corrected = False #also needs to be reset
 
         print("Importing data")
         print_text.append("Importing data")
         directory = self.lineEdit_image_filename_2.text().strip()
         if directory == "":
@@ -2776,22 +2852,29 @@
             #this needs to be changed based on lattice type
             gold_lattice_param = temperature*5.67075E-5 + 4.06111 #A 
             goldLattice_111 = gold_lattice_param / (1**2+1**2+1**2)**0.5
             goldLattice_200 = gold_lattice_param / (2**2)**0.5
             #gc_res = 3.3378
             gc_res = 3.434
             print_text.append(f"Lattice type is {latticeType}")
-            lattice_res = goldLattice_111
+            latticeRes = goldLattice_111
             if latticeType == "gold-111":
-                lattice_res = goldLattice_111
+                latticeRes = goldLattice_111
             elif latticeType == "gold-200":
-                lattice_res = goldLattice_200
+                latticeRes = goldLattice_200
             elif latticeType == "graphitized-carbon":
-                lattice_res = gc_res
-            if px_guess >= lattice_res/2:
+                latticeRes = gc_res
+            elif latticeType == "define_lattice_constant":
+                try:
+                    latticeRes = float(self.lineEdit_latticeConstant.text())
+                except ValueError:
+                    print("Error: Lattice constant must be a number")
+                    print_text.append("Error: Lattice constant must be a number")
+                    input_okay = False
+            if px_guess >= latticeRes/2:
                 aliased = True
             else:
                 aliased = False
             if fileType != "mrc":
                 print(f"Converting all {fileType} to MRC")
                 print_text.append(f"Converting all {fileType} to MRC")
                 #convertMRC.runConvert(directory, fileType)
@@ -2835,14 +2918,15 @@
                 f.write(f"DataDirectory:{directory}\n")
                 f.write(f"FileType:{fileType}\n")
                 f.write(f"Temperature:{str(temperature)}\n")
                 f.write(f"PxGuess:{str(px_guess)}\n")
                 f.write(f"Aliased:{str(aliased)}\n")
                 f.write(f"Images:{str(num_images)}\n")
                 f.write(f"LatticeType:{latticeType}\n")
+                f.write(f"LatticeRes:{latticeRes}\n")
 
             print("Data import complete")
             print_text.append("Data import complete")
 
         #set the PS input as this import file as default
         #self.lineEdit_importJob.setText(f"{proj_directory}Import/job{job_string}/import_vals.txt")
         self.comboBox_importJob.addItem(job_string)
@@ -2855,15 +2939,15 @@
             for line in print_text:
                 f.write(f"{line}\n")
 
     def str2bool(self, v):
         return v.lower() in ("true")
 
     def readImport(self):
-        global temperature, directory, fileType, px_guess, aliased, num_images, latticeType
+        global temperature, directory, fileType, px_guess, aliased, num_images, latticeType, latticeRes
         #importFilePath = self.lineEdit_importJob.text().strip()
         import_jobNumber = self.comboBox_importJob.currentText()
         importFilePath = f"{proj_directory}Import/job{import_jobNumber}/import_vals.txt"
         with open(importFilePath, 'r') as f:
             for line in f.readlines():
                 l = line.split(':')
                 val = l[1].strip("\n")
@@ -2878,17 +2962,19 @@
                     px_guess = float(val)
                 elif l[0] == "Aliased":
                     aliased = self.str2bool(val)
                 elif l[0] == "Images":
                     num_images = int(val)
                 elif l[0] == "LatticeType":
                     latticeType = val
+                elif l[0] == "LatticeRes":
+                    latticeRes = float(val)
 
     def readImport2(self, importFilePath):
-        global temperature, directory, fileType, px_guess, aliased, num_images, latticeType
+        global temperature, directory, fileType, px_guess, aliased, num_images, latticeType, latticeRes
         #importFilePath = self.lineEdit_importJob.text()
         with open(importFilePath, 'r') as f:
             for line in f.readlines():
                 l = line.split(':')
                 val = l[1].strip("\n")
                 val = val.strip()
                 if l[0] == "DataDirectory":
@@ -2901,14 +2987,18 @@
                     px_guess = float(val)
                 elif l[0] == "Aliased":
                     aliased = self.str2bool(val)
                 elif l[0] == "Images":
                     num_images = int(val)
                 elif l[0] == "LatticeType":
                     latticeType = val
+                elif l[0] == "LatticeRes":
+                    latticeRes = float(val)
+        
+    
 
     def getCores(self):
         num_cores = 1
         try:
             num_cores = int(self.lineEdit_cores.text())
         except ValueError:
             print("Error: Number of cores must be an integer")
@@ -3128,15 +3218,15 @@
         save_filename = f"{this_pxdir}resultFFT"
         alias_string = 'f'
         px_to_pass = mean_px
         if aliased:
             alias_string = 'y'
         if multi_image == False or aliased == True:
             px_to_pass = sum_px
-        myMatProcess = subprocess.Popen([sys.executable, '-m', 'magCalibration.scripts.show_FFT', ps_dir, save_filename, str(px_to_pass), str(cores), latticeType, alias_string, str(temperature)])
+        myMatProcess = subprocess.Popen([sys.executable, '-m', 'magCalibration.scripts.show_FFT', ps_dir, save_filename, str(px_to_pass), str(cores), latticeType, alias_string, str(temperature), str(latticeRes)])
 
 
         
 
     def runMeasurePx(self):
         global supervised_angle, savgol_window2, ps_dir, ps_dir2, aniso_param, supervised_smooth, done_Px1
         supervised_angle = False
@@ -3172,14 +3262,19 @@
         if os.path.exists(f"{PS_folder}NWPS"):
             ps_base_dir = f"{PS_folder}NWPS/"
         elif os.path.exists(f"{PS_folder}powerSpectra"):
             ps_base_dir = f"{PS_folder}powerSpectra/"
         elif os.path.exists(f"{PS_folder}stretch"):
             ps_base_dir = f"{PS_folder}stretch/"
 
+        #read the relevant import via NPS/correctAniso input file to get pxGuess, temp
+        PSInputFile = self.locatePSInputFile(PS_folder)
+        importFile = self.readPSInput(PSInputFile)
+        self.readImport2(importFile.strip())
+
 
         ps_dir = f"{ps_base_dir}avg/"
         
         if ps_base_dir != f"{PS_folder}stretch/":
             if aliased:
                 ps_dir += "aliased/"
             
@@ -3196,18 +3291,15 @@
             ps_dir2 = ps_base_dir
 
 
         #PS_folder = self.lineEdit_MakePSJob.text().strip()
         #ps_dir = PS_folder
         if ps_dir.endswith('/') == False:
             ps_dir += '/'
-        #read the relevant import via NPS/correctAniso input file to get pxGuess, temp
-        PSInputFile = self.locatePSInputFile(PS_folder)
-        importFile = self.readPSInput(PSInputFile)
-        self.readImport2(importFile.strip())
+
 
         #If this was from aniso, I need to get the aniso params file
         parts = PSInputFile.split('/')
         param_file = ""
         #print(parts[len(parts)-1])
         if parts[len(parts)-1] == "CorrectAnisoInput.txt": #then aniso
             param_file = self.readAnisoInput(PSInputFile)
@@ -3326,14 +3418,15 @@
             # Step 3: Create a worker object
             self.worker = Worker()
             # Step 4: Move worker to the thread
             self.worker.moveToThread(self.thread)
                 
             # Step 5: Connect signals and slots
             self.thread.started.connect(self.worker.makeNotWhitePS)
+            #self.thread.started.connect(self.worker.makeBackgroundSubtractedPS)
             self.worker.finished.connect(self.thread.quit)
             self.worker.finished.connect(self.worker.deleteLater)
             self.thread.finished.connect(self.thread.deleteLater)
             # Step 6: Start the thread
             self.thread.start()
             # Final resets
             self.pushButton_Run.setEnabled(False)
@@ -3427,26 +3520,29 @@
             os.mkdir(new_write_dir)
 
         #read the relevant import via NPS input file to get pxGuess, temp
         #PS_folder = self.lineEdit_MakePSJob.text()
         #get PS folder
         ps_job = self.comboBox_MakePSJob.currentText()
         PS_folder = f"{proj_directory}MakePS/job{ps_job}/"
+
+        #need to find 
+        PSInputFile = self.locatePSInputFile(PS_folder)
+        importFile = self.readPSInput(PSInputFile)
+        self.readImport2(importFile.strip())
         ps_base_dir = ""
+
         if os.path.exists(f"{PS_folder}NWPS"):
             ps_base_dir = f"{PS_folder}NWPS/"
         else:
             ps_base_dir = f"{PS_folder}powerSpectra/"
         ps_dir = f"{ps_base_dir}avg/"
         if ps_dir.endswith('/') == False:
             ps_dir += '/'
-        #need to find 
-        PSInputFile = self.locatePSInputFile(PS_folder)
-        importFile = self.readPSInput(PSInputFile)
-        self.readImport2(importFile.strip())
+
 
         cores = self.getCores()
         # Step 2: Create a QThread object
         self.thread = QThread()
         # Step 3: Create a worker object
         self.worker = Worker()
         # Step 4: Move worker to the thread
@@ -3488,14 +3584,19 @@
         write_dir = f"{proj_directory}CorrectAniso/job{job_string}"
         if os.path.exists(write_dir) == False:
             os.mkdir(write_dir)
         #get PS folder 
         #PS_folder = self.lineEdit_MakePSJob.text()
         ps_job = self.comboBox_MakePSJob.currentText()
         PS_folder = f"{proj_directory}MakePS/job{ps_job}/"
+        #get import
+        PSInputFile = self.locatePSInputFile(PS_folder)
+        importFile = self.readPSInput(PSInputFile)
+        self.readImport2(importFile.strip())
+
         ps_base_dir = ""
         if os.path.exists(f"{PS_folder}NWPS"):
             ps_base_dir = f"{PS_folder}NWPS/"
         else:
             ps_base_dir = f"{PS_folder}powerSpectra/"
         ps_dir = f"{ps_base_dir}avg/"
 
@@ -3514,18 +3615,15 @@
         if ps_dir.endswith('/') == False:
             ps_dir += '/'
         #get param file
         #aniso_param = self.lineEdit_AnisoParams.text()
         aniso_job = self.comboBox_AnisoParams.currentText()
         aniso_param = f"{proj_directory}MeasureAniso/job{aniso_job}/aniso_params.csv"      
 
-        #get import
-        PSInputFile = self.locatePSInputFile(PS_folder)
-        importFile = self.readPSInput(PSInputFile)
-        self.readImport2(importFile.strip())
+
 
         cores = self.getCores()
         # Step 2: Create a QThread object
         self.thread = QThread()
         # Step 3: Create a worker object
         self.worker = Worker()
         # Step 4: Move worker to the thread
```

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/aliasPS.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/aliasPS.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from scipy.optimize import curve_fit
 from numba import jit
 from multiprocessing import Pool
 from functools import partial
 
 goldLattice = 2.347
 
-def padNWPS(fft_width, pxGuess):
+def padNWPS(fft_width, pxGuess, latticeRes):
     #first find out how far to go
-    radius_gold = fft_width*pxGuess/goldLattice
+    radius_gold = fft_width*pxGuess/latticeRes
     #now I want to do the padding with zeros
     padWidth = (radius_gold*2) + (radius_gold*0.2)
     padXY = [0, 0]
     padXYVal = (padWidth - fft_width)
     if padXYVal % 2 == 0: #even
         padXY = [int(padXYVal/2), int(padXYVal/2)]
     else: #odd
@@ -58,40 +58,40 @@
                new_NWPS[padXY[0]+fft_width+i, padXY[0]+fft_width+j] = new_NWPS[padXY[0]+fft_width-i, padXY[0]+fft_width-j]
                new_NWPS[padXY[0]+fft_width+i, j] = new_NWPS[padXY[0]+fft_width-i, 2*padXY[0]-j] 
                new_NWPS[i, padXY[0]+fft_width+j] = new_NWPS[2*padXY[0]-i, padXY[0]+fft_width-j] 
                 
  
     return new_NWPS
 
-def doAnImage(img, pxGuess):
+def doAnImage(img, pxGuess, latticeRes):
     #need to get width to make power of 2 fft
     size = img.shape
     #now I want to mirror this outward
-    padXY = padNWPS(size[0], pxGuess)
+    padXY = padNWPS(size[0], pxGuess, latticeRes)
     NWPS_pad = np.pad(img, [padXY, padXY], 'constant')
     #Next set these to mirrored values
     new_NWPS = mirrorValues(NWPS_pad, size[0], padXY)
     return new_NWPS
 
-def runScript(path, pxGuess, cores):
+def runScript(path, pxGuess, cores, latticeRes):
     #I want to check if the gold is beyond Nyquist 
     print("Dealing with aliasing")
     file_list = [f for f in os.listdir(path) if f.endswith(".mrc")]
     total = len(file_list)
 
     #load images
     NWPS = []
     for filename in file_list:
         mrc = mrcfile.open(path+filename, permissive=True)
         NWPS.append(mrc.data)
         mrc.close()
 
     #Process them
     p = Pool(processes=cores)
-    doAnImage1 = partial(doAnImage, pxGuess=pxGuess)
+    doAnImage1 = partial(doAnImage, pxGuess=pxGuess, latticeRes=latticeRes)
     results = []
     for i, str_img in enumerate(p.map(doAnImage1, NWPS)):
         results.append(str_img)
         print(f"Image {str(i+1)}/{str(total)} processed")
     p.close()
 
     #write themuser_angles_temp.csv
```

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/angles.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/angles.py`

 * *Files identical despite different names*

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/angles_choose.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/angles_choose.py`

 * *Files identical despite different names*

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/autoGold.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/autoGold.py`

 * *Files identical despite different names*

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/calcStats.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/calcStats.py`

 * *Files identical despite different names*

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/convertMRC.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/convertMRC.py`

 * *Files identical despite different names*

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/correctAniso.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/correctAniso.py`

 * *Files identical despite different names*

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/getUserAngles.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/getUserAngles.py`

 * *Files identical despite different names*

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/getUserBoxes.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/getUserBoxes.py`

 * *Files identical despite different names*

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/makeAllNWPS_MTF.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/makeAllNWPS_MTF.py`

 * *Files identical despite different names*

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/makeAllNWPS_blank.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/makeAllNWPS_blank.py`

 * *Files identical despite different names*

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/makeBlankNPS_ra.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/makeBlankNPS_ra.py`

 * *Files identical despite different names*

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/makeImageNPS_ra.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/makeImageNPS_ra.py`

 * *Files identical despite different names*

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/makeOneUnwhitenedPS.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/makeOneUnwhitenedPS.py`

 * *Files identical despite different names*

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/makeUnwhitenedPSAll.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/makeUnwhitenedPSAll.py`

 * *Files identical despite different names*

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/measurePxAllAngles.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/measurePxAllAngles.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 
     #finally write the printText file
     with open(f"{write_dir}outputText.txt", 'a') as f:
         for line in print_text:
             f.write(f"{line}\n")
     
 
-def runScript(path, temperature, pxGuess, cores, aliased, spectra_dir, ps_dir, write_dir, latticeType):
+def runScript(path, temperature, pxGuess, cores, aliased, spectra_dir, ps_dir, write_dir, latticeType, latticeRes):
     print_text = []
     print("Measuring pixel sizes across all angles")
     print_text.append("Measuring pixel sizes across all angles")
     gold_lattice_param = temperature*5.67075E-5 + 4.06111 #A 
     if temperature < 43.0:
         gold_lattice_param = 43.0*5.67075E-5 + 4.06111 #A       
     goldLattice_111 = gold_lattice_param / (1**2+1**2+1**2)**0.5
@@ -191,14 +191,16 @@
     lattice_res = goldLattice_111
     if latticeType == "gold-111":
         lattice_res = goldLattice_111
     elif latticeType == "gold-200":
         lattice_res = goldLattice_200
     elif latticeType == "graphitized-carbon":
         lattice_res = gc_res
+    elif latticeType == "define_lattice_constant":
+        lattice_res = latticeRes
 
     step = int(2)
     angles = np.arange(1, 180, step)
 
     #get directory
     '''
     NWPS_dir = f"{path}{spectra_dir}/avg/10/"
```

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/measurePxAvg.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/measurePxAvg_max.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         px = 0
     
     if (max_index <= 1):
         px = 0
     #print(px)
     return [px, end]
 
-def runScript(path, pxGuess, temperature, cores, savgol_window, supervised_angle, aliased, aniso_corrected, spectra_dir, write_dir, ps_dir, latticeType, supervised_smooth, avgImage):
+def runScript(path, pxGuess, temperature, cores, savgol_window, supervised_angle, aliased, aniso_corrected, spectra_dir, write_dir, ps_dir, latticeType, supervised_smooth, avgImage, latticeRes):
     print_text = []    
     gold_lattice_param = temperature*5.67075E-5 + 4.06111 #A
     #adjust for very low temperature
     if temperature < 43.0:
         gold_lattice_param = 43.0*5.67075E-5 + 4.06111 #A       
     goldLattice_111 = gold_lattice_param / (1**2+1**2+1**2)**0.5
     goldLattice_200 = gold_lattice_param / (2**2)**0.5
@@ -289,14 +289,16 @@
     lattice_res = goldLattice_111
     if latticeType == "gold-111":
         lattice_res = goldLattice_111
     elif latticeType == "gold-200":
         lattice_res = goldLattice_200
     elif latticeType == "graphitized-carbon":
         lattice_res = gc_res
+    elif latticeType == "define_lattice_constant":
+        lattice_res = latticeRes
 
     overall = []
     file_list = []
     #NWPS_dir = f"{path}{spectra_dir}/avg/10/"
     NWPS_dir = ps_dir
     '''
     if aniso_corrected:
```

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/show_FFT.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/show_FFT.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     plt.subplots_adjust(bottom=0.2, left=0.10, right=0.95, top=0.90)
     ax_slide_contrast = plt.axes([0.05, 0.25, 0.0225, 0.63])
     contrast_slider = Slider(ax_slide_contrast, 'Contrast', valmin=1, valmax=100, valinit=contrast_val, valstep=1, orientation="vertical")
 
 
     #now plot the circle
     size = img.shape
-    radius = minradi = int((size[0]*pxGuess)/latticeRes)
+    radius = int((size[0]*pxGuess)/latticeRes)
     size_alias =   2**(int(math.log(size[0], 2)))
     if aliased == 'y':
         radius = int((size_alias*pxGuess)/latticeRes)
     circle = Ellipse((size[0]/2, size[1]/2), 2*radius, 2*radius, color='r', fill=False, linestyle='--', linewidth=0.5)
     ax.add_artist(circle)
     
 
@@ -123,15 +123,15 @@
     px = 0
     #print(size[0])
     center = (size[0]/2, size[1]/2)
     #get the angles proper
     angles = getUserAngularRange(img, center, pxGuess, latticeRes, aliased, cores, fileSave)
     return px
 
-def getLatticeRes(temperature, latticeType):
+def getLatticeRes(temperature, latticeType, latticeResPassed):
     gold_lattice_param = temperature*5.67075E-5 + 4.06111 #A
     #adjust for very low temperature
     if temperature < 43.0:
         gold_lattice_param = 43.0*5.67075E-5 + 4.06111 #A       
     goldLattice_111 = gold_lattice_param / (1**2+1**2+1**2)**0.5
     goldLattice_200 = gold_lattice_param / (2**2)**0.5
     #gc_res = 3.3378
@@ -139,25 +139,28 @@
     lattice_res = goldLattice_111
     if latticeType == "gold-111":
         lattice_res = goldLattice_111
     elif latticeType == "gold-200":
         lattice_res = goldLattice_200
     elif latticeType == "graphitized-carbon":
         lattice_res = gc_res
+    elif latticeType == "define_lattice_constant":
+        lattice_res = latticeResPassed
     return lattice_res
 
 if __name__ == "__main__":
     path = sys.argv[1]
     fileSave = sys.argv[2]
     pxGuess = float(sys.argv[3])
     cores = int(sys.argv[4])
     latticeType = sys.argv[5]
     aliased = sys.argv[6]
     temperature = float(sys.argv[7])
-    latticeRes = getLatticeRes(temperature, latticeType)
+    latticeResPassed = float(sys.argv[8])
+    latticeRes = getLatticeRes(temperature, latticeType, latticeResPassed)
     px2 = []
     overall = []
     for filename in os.listdir(path):
         if filename.endswith(".mrc"):
             print(filename)
             mrc = mrcfile.open(path+filename)
             img = mrc.data
```

### Comparing `MagCalibration-jdickerson80-1.1.0/src/magCalibration/scripts/smooth_choose.py` & `MagCalibration-jdickerson80-1.2.0/src/magCalibration/scripts/smooth_choose.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,16 +182,16 @@
     bAccept.on_clicked(acceptClick)
     bReject.on_clicked(rejectClick)
     bEnd.on_clicked(endClick)
 
     plt.show()
 
     
-    if (max_index <= 1):
-        px = 0
+    #if (max_index <= 1):
+    #    px = 0
 
     if reject == True:
         px = 0
     if end == True:
         px = 0
 
     return [px, str(end)]
```

