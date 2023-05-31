# Comparing `tmp/ngscrape-1.1.0.tar.gz` & `tmp/ngscrape-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngscrape-1.1.0.tar", last modified: Mon May 29 18:02:23 2023, max compression
+gzip compressed data, was "ngscrape-1.2.0.tar", last modified: Wed May 31 00:32:32 2023, max compression
```

## Comparing `ngscrape-1.1.0.tar` & `ngscrape-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 18:02:23.513325 ngscrape-1.1.0/
--rw-rw-rw-   0        0        0    35184 2023-05-27 22:41:04.000000 ngscrape-1.1.0/LICENSE
--rw-rw-rw-   0        0        0    42296 2023-05-29 18:02:23.511322 ngscrape-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      738 2023-05-29 18:01:50.000000 ngscrape-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0     1259 2023-05-28 19:51:04.000000 ngscrape-1.1.0/readme.md
--rw-rw-rw-   0        0        0       42 2023-05-29 18:02:23.513325 ngscrape-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-29 18:02:23.479204 ngscrape-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 18:02:23.479204 ngscrape-1.1.0/src/ngscrape/
--rw-rw-rw-   0        0        0     3764 2023-05-29 18:00:06.000000 ngscrape-1.1.0/src/ngscrape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 18:02:23.509323 ngscrape-1.1.0/src/ngscrape.egg-info/
--rw-rw-rw-   0        0        0    42296 2023-05-29 18:02:23.000000 ngscrape-1.1.0/src/ngscrape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-29 18:02:23.000000 ngscrape-1.1.0/src/ngscrape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 18:02:23.000000 ngscrape-1.1.0/src/ngscrape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-29 18:02:23.000000 ngscrape-1.1.0/src/ngscrape.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 18:02:23.000000 ngscrape-1.1.0/src/ngscrape.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 00:32:32.205721 ngscrape-1.2.0/
+-rw-rw-rw-   0        0        0    35184 2023-05-27 22:41:04.000000 ngscrape-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0    42296 2023-05-31 00:32:32.203727 ngscrape-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      738 2023-05-31 00:32:09.000000 ngscrape-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1259 2023-05-28 19:51:04.000000 ngscrape-1.2.0/readme.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 00:32:32.205721 ngscrape-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 00:32:32.166724 ngscrape-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 00:32:32.174723 ngscrape-1.2.0/src/ngscrape/
+-rw-rw-rw-   0        0        0     7940 2023-05-31 00:31:45.000000 ngscrape-1.2.0/src/ngscrape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 00:32:32.199717 ngscrape-1.2.0/src/ngscrape.egg-info/
+-rw-rw-rw-   0        0        0    42296 2023-05-31 00:32:32.000000 ngscrape-1.2.0/src/ngscrape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-31 00:32:32.000000 ngscrape-1.2.0/src/ngscrape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 00:32:32.000000 ngscrape-1.2.0/src/ngscrape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-31 00:32:32.000000 ngscrape-1.2.0/src/ngscrape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-31 00:32:32.000000 ngscrape-1.2.0/src/ngscrape.egg-info/top_level.txt
```

### Comparing `ngscrape-1.1.0/LICENSE` & `ngscrape-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ngscrape-1.1.0/PKG-INFO` & `ngscrape-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngscrape
-Version: 1.1.0
+Version: 1.2.0
 Summary: Newgrounds flash game scraper powered by bs4 and requests
 Author-email: aeiea <dpthn@proton.me>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ngscrape-1.1.0/pyproject.toml` & `ngscrape-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ngscrape"
-version = "1.1.0"
+version = "1.2.0"
 description = "Newgrounds flash game scraper powered by bs4 and requests"
 readme = "readme.md"
 authors = [{ name = "aeiea", email = "dpthn@proton.me" }]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Programming Language :: Python",
```

### Comparing `ngscrape-1.1.0/readme.md` & `ngscrape-1.2.0/readme.md`

 * *Files identical despite different names*

### Comparing `ngscrape-1.1.0/src/ngscrape.egg-info/PKG-INFO` & `ngscrape-1.2.0/src/ngscrape.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngscrape
-Version: 1.1.0
+Version: 1.2.0
 Summary: Newgrounds flash game scraper powered by bs4 and requests
 Author-email: aeiea <dpthn@proton.me>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

