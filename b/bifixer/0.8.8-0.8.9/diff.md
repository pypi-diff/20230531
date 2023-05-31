# Comparing `tmp/bifixer-0.8.8.tar.gz` & `tmp/bifixer-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bifixer-0.8.8.tar", last modified: Tue Mar 14 11:01:13 2023, max compression
+gzip compressed data, was "bifixer-0.8.9.tar", last modified: Wed May 31 09:53:00 2023, max compression
```

## Comparing `bifixer-0.8.8.tar` & `bifixer-0.8.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-14 11:01:13.901568 bifixer-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-03-14 11:01:04.000000 bifixer-0.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-03-14 11:01:04.000000 bifixer-0.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    62522 2023-03-14 11:01:13.901568 bifixer-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    20825 2023-03-14 11:01:04.000000 bifixer-0.8.8/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-03-14 11:01:04.000000 bifixer-0.8.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-14 11:01:13.901568 bifixer-0.8.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-14 11:01:13.897568 bifixer-0.8.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-14 11:01:13.897568 bifixer-0.8.8/src/bifixer/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-03-14 11:01:04.000000 bifixer-0.8.8/src/bifixer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18865 2023-03-14 11:01:04.000000 bifixer-0.8.8/src/bifixer/bifixer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-14 11:01:13.897568 bifixer-0.8.8/src/bifixer/detok/
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-03-14 11:01:04.000000 bifixer-0.8.8/src/bifixer/detok/detok.mt
--rw-r--r--   0 runner    (1001) docker     (122)    13681 2023-03-14 11:01:04.000000 bifixer-0.8.8/src/bifixer/monofixer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-14 11:01:13.901568 bifixer-0.8.8/src/bifixer/replacements/
--rw-r--r--   0 runner    (1001) docker     (122)     9227 2023-03-14 11:01:04.000000 bifixer-0.8.8/src/bifixer/replacements/replacements.da
--rw-r--r--   0 runner    (1001) docker     (122)    34077 2023-03-14 11:01:04.000000 bifixer-0.8.8/src/bifixer/replacements/replacements.de
--rw-r--r--   0 runner    (1001) docker     (122)    78820 2023-03-14 11:01:04.000000 bifixer-0.8.8/src/bifixer/replacements/replacements.en
--rw-r--r--   0 runner    (1001) docker     (122)     9073 2023-03-14 11:01:04.000000 bifixer-0.8.8/src/bifixer/replacements/replacements.es
--rw-r--r--   0 runner    (1001) docker     (122)      340 2023-03-14 11:01:04.000000 bifixer-0.8.8/src/bifixer/replacements/replacements.fr
--rw-r--r--   0 runner    (1001) docker     (122)     1913 2023-03-14 11:01:04.000000 bifixer-0.8.8/src/bifixer/replacements/replacements.nb
--rw-r--r--   0 runner    (1001) docker     (122)    46022 2023-03-14 11:01:04.000000 bifixer-0.8.8/src/bifixer/replacements/replacements.nl
--rw-r--r--   0 runner    (1001) docker     (122)    33279 2023-03-14 11:01:04.000000 bifixer-0.8.8/src/bifixer/replacements/replacements.pt
--rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-03-14 11:01:04.000000 bifixer-0.8.8/src/bifixer/replacements/replacements.tr
--rw-r--r--   0 runner    (1001) docker     (122)    25727 2023-03-14 11:01:04.000000 bifixer-0.8.8/src/bifixer/restorative_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (122)     4061 2023-03-14 11:01:04.000000 bifixer-0.8.8/src/bifixer/segmenter.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-03-14 11:01:04.000000 bifixer-0.8.8/src/bifixer/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-14 11:01:13.897568 bifixer-0.8.8/src/bifixer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    62522 2023-03-14 11:01:13.000000 bifixer-0.8.8/src/bifixer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-03-14 11:01:13.000000 bifixer-0.8.8/src/bifixer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-14 11:01:13.000000 bifixer-0.8.8/src/bifixer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-03-14 11:01:13.000000 bifixer-0.8.8/src/bifixer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-03-14 11:01:13.000000 bifixer-0.8.8/src/bifixer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-03-14 11:01:13.000000 bifixer-0.8.8/src/bifixer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-14 11:01:13.901568 bifixer-0.8.8/src/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    13930 2023-03-14 11:01:04.000000 bifixer-0.8.8/src/tests/test_bifixer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 09:53:00.919415 bifixer-0.8.9/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-31 09:52:42.000000 bifixer-0.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-31 09:52:42.000000 bifixer-0.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    62522 2023-05-31 09:53:00.919415 bifixer-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    20825 2023-05-31 09:52:42.000000 bifixer-0.8.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-05-31 09:52:42.000000 bifixer-0.8.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 09:53:00.919415 bifixer-0.8.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 09:53:00.915415 bifixer-0.8.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 09:53:00.915415 bifixer-0.8.9/src/bifixer/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-05-31 09:52:42.000000 bifixer-0.8.9/src/bifixer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18927 2023-05-31 09:52:42.000000 bifixer-0.8.9/src/bifixer/bifixer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 09:53:00.919415 bifixer-0.8.9/src/bifixer/detok/
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-31 09:52:42.000000 bifixer-0.8.9/src/bifixer/detok/detok.mt
+-rw-r--r--   0 runner    (1001) docker     (122)    13716 2023-05-31 09:52:42.000000 bifixer-0.8.9/src/bifixer/monofixer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 09:53:00.919415 bifixer-0.8.9/src/bifixer/replacements/
+-rw-r--r--   0 runner    (1001) docker     (122)     9227 2023-05-31 09:52:42.000000 bifixer-0.8.9/src/bifixer/replacements/replacements.da
+-rw-r--r--   0 runner    (1001) docker     (122)    34077 2023-05-31 09:52:42.000000 bifixer-0.8.9/src/bifixer/replacements/replacements.de
+-rw-r--r--   0 runner    (1001) docker     (122)    78820 2023-05-31 09:52:42.000000 bifixer-0.8.9/src/bifixer/replacements/replacements.en
+-rw-r--r--   0 runner    (1001) docker     (122)     9073 2023-05-31 09:52:42.000000 bifixer-0.8.9/src/bifixer/replacements/replacements.es
+-rw-r--r--   0 runner    (1001) docker     (122)      340 2023-05-31 09:52:42.000000 bifixer-0.8.9/src/bifixer/replacements/replacements.fr
+-rw-r--r--   0 runner    (1001) docker     (122)     1913 2023-05-31 09:52:42.000000 bifixer-0.8.9/src/bifixer/replacements/replacements.nb
+-rw-r--r--   0 runner    (1001) docker     (122)    46022 2023-05-31 09:52:42.000000 bifixer-0.8.9/src/bifixer/replacements/replacements.nl
+-rw-r--r--   0 runner    (1001) docker     (122)    33279 2023-05-31 09:52:42.000000 bifixer-0.8.9/src/bifixer/replacements/replacements.pt
+-rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-05-31 09:52:42.000000 bifixer-0.8.9/src/bifixer/replacements/replacements.tr
+-rw-r--r--   0 runner    (1001) docker     (122)    25727 2023-05-31 09:52:42.000000 bifixer-0.8.9/src/bifixer/restorative_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4061 2023-05-31 09:52:42.000000 bifixer-0.8.9/src/bifixer/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-05-31 09:52:42.000000 bifixer-0.8.9/src/bifixer/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 09:53:00.919415 bifixer-0.8.9/src/bifixer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    62522 2023-05-31 09:53:00.000000 bifixer-0.8.9/src/bifixer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-05-31 09:53:00.000000 bifixer-0.8.9/src/bifixer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 09:53:00.000000 bifixer-0.8.9/src/bifixer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-31 09:53:00.000000 bifixer-0.8.9/src/bifixer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-31 09:53:00.000000 bifixer-0.8.9/src/bifixer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-31 09:53:00.000000 bifixer-0.8.9/src/bifixer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 09:53:00.919415 bifixer-0.8.9/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    13930 2023-05-31 09:52:42.000000 bifixer-0.8.9/src/tests/test_bifixer.py
```

### Comparing `bifixer-0.8.8/LICENSE` & `bifixer-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bifixer-0.8.8/PKG-INFO` & `bifixer-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bifixer
-Version: 0.8.8
+Version: 0.8.9
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Marta Bañón <mbanon@prompsit.com>, Jaume Zaragoza <jzaragoza@prompsit.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bifixer-0.8.8/README.md` & `bifixer-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `bifixer-0.8.8/pyproject.toml` & `bifixer-0.8.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bifixer"
-version = "0.8.8"
+version = "0.8.9"
 license = {file = "LICENSE"}
 authors = [
     { name="Prompsit Language Engineering", email="info@prompsit.com" },
 ]
 maintainers = [
     { name="Marta Bañón", email="mbanon@prompsit.com" },
     { name="Jaume Zaragoza", email="jzaragoza@prompsit.com" },
```

### Comparing `bifixer-0.8.8/src/bifixer/bifixer.py` & `bifixer-0.8.9/src/bifixer/bifixer.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,17 @@
     if not args.ignore_orthography:
         replacements_slang = restorative_cleaning.getReplacements(args.srclang)
         replacements_tlang = restorative_cleaning.getReplacements(args.trglang)
 
     if not args.ignore_detokenization:
         detoks_slang = restorative_cleaning.getDetokenizations(args.srclang)
         detoks_tlang = restorative_cleaning.getDetokenizations(args.trglang)
+    else:
+        detoks_slang = {}
+        detoks_tlang = {}
 
     if not args.ignore_segmentation:
         source_segmenter = segmenter.NaiveSegmenter(args.srclang, args.segmenter)
         target_segmenter = segmenter.NaiveSegmenter(args.trglang, args.segmenter)
 
     if args.header:
         header = next(args.input).strip().split("\t")
```

### Comparing `bifixer-0.8.8/src/bifixer/monofixer.py` & `bifixer-0.8.9/src/bifixer/monofixer.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,14 +127,16 @@
         punctChars_lang, punctRe_lang = restorative_cleaning.getNormalizedPunctReplacements(args.lang)
 
     if not args.ignore_orthography:    
         replacements_lang = restorative_cleaning.getReplacements(args.lang)
       
     if not args.ignore_detokenization:
         detoks_lang = restorative_cleaning.getDetokenizations(args.lang)
+    else:
+        detoks_lang = {}
         
     if not args.ignore_segmentation:
         lang_segmenter = segmenter.NaiveSegmenter(args.lang, args.segmenter)
 
     if args.header:
         header = next(args.input).strip().split("\t")
```

### Comparing `bifixer-0.8.8/src/bifixer/replacements/replacements.da` & `bifixer-0.8.9/src/bifixer/replacements/replacements.da`

 * *Files identical despite different names*

### Comparing `bifixer-0.8.8/src/bifixer/replacements/replacements.de` & `bifixer-0.8.9/src/bifixer/replacements/replacements.de`

 * *Files identical despite different names*

### Comparing `bifixer-0.8.8/src/bifixer/replacements/replacements.en` & `bifixer-0.8.9/src/bifixer/replacements/replacements.en`

 * *Files identical despite different names*

### Comparing `bifixer-0.8.8/src/bifixer/replacements/replacements.es` & `bifixer-0.8.9/src/bifixer/replacements/replacements.es`

 * *Files identical despite different names*

### Comparing `bifixer-0.8.8/src/bifixer/replacements/replacements.nb` & `bifixer-0.8.9/src/bifixer/replacements/replacements.nb`

 * *Files identical despite different names*

### Comparing `bifixer-0.8.8/src/bifixer/replacements/replacements.nl` & `bifixer-0.8.9/src/bifixer/replacements/replacements.nl`

 * *Files identical despite different names*

### Comparing `bifixer-0.8.8/src/bifixer/replacements/replacements.pt` & `bifixer-0.8.9/src/bifixer/replacements/replacements.pt`

 * *Files identical despite different names*

### Comparing `bifixer-0.8.8/src/bifixer/replacements/replacements.tr` & `bifixer-0.8.9/src/bifixer/replacements/replacements.tr`

 * *Files identical despite different names*

### Comparing `bifixer-0.8.8/src/bifixer/restorative_cleaning.py` & `bifixer-0.8.9/src/bifixer/restorative_cleaning.py`

 * *Files identical despite different names*

### Comparing `bifixer-0.8.8/src/bifixer/segmenter.py` & `bifixer-0.8.9/src/bifixer/segmenter.py`

 * *Files identical despite different names*

### Comparing `bifixer-0.8.8/src/bifixer/util.py` & `bifixer-0.8.9/src/bifixer/util.py`

 * *Files identical despite different names*

### Comparing `bifixer-0.8.8/src/bifixer.egg-info/PKG-INFO` & `bifixer-0.8.9/src/bifixer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bifixer
-Version: 0.8.8
+Version: 0.8.9
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Marta Bañón <mbanon@prompsit.com>, Jaume Zaragoza <jzaragoza@prompsit.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bifixer-0.8.8/src/bifixer.egg-info/SOURCES.txt` & `bifixer-0.8.9/src/bifixer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bifixer-0.8.8/src/tests/test_bifixer.py` & `bifixer-0.8.9/src/tests/test_bifixer.py`

 * *Files identical despite different names*

