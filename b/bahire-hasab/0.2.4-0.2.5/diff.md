# Comparing `tmp/bahire-hasab-0.2.4.tar.gz` & `tmp/bahire-hasab-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bahire-hasab-0.2.4.tar", last modified: Sun May 28 10:57:42 2023, max compression
+gzip compressed data, was "bahire-hasab-0.2.5.tar", last modified: Wed May 31 13:08:44 2023, max compression
```

## Comparing `bahire-hasab-0.2.4.tar` & `bahire-hasab-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:57:42.589565 bahire-hasab-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-28 10:57:31.000000 bahire-hasab-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-28 10:57:42.589565 bahire-hasab-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-28 10:57:31.000000 bahire-hasab-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-28 10:57:31.000000 bahire-hasab-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 10:57:42.589565 bahire-hasab-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-28 10:57:31.000000 bahire-hasab-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:57:42.589565 bahire-hasab-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:57:42.589565 bahire-hasab-0.2.4/src/bahire_hasab/
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-05-28 10:57:31.000000 bahire-hasab-0.2.4/src/bahire_hasab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:57:42.589565 bahire-hasab-0.2.4/src/bahire_hasab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-28 10:57:42.000000 bahire-hasab-0.2.4/src/bahire_hasab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-28 10:57:42.000000 bahire-hasab-0.2.4/src/bahire_hasab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 10:57:42.000000 bahire-hasab-0.2.4/src/bahire_hasab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-28 10:57:42.000000 bahire-hasab-0.2.4/src/bahire_hasab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:08:44.757287 bahire-hasab-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-31 13:08:28.000000 bahire-hasab-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-31 13:08:44.757287 bahire-hasab-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-31 13:08:28.000000 bahire-hasab-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-31 13:08:28.000000 bahire-hasab-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:08:44.757287 bahire-hasab-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-31 13:08:28.000000 bahire-hasab-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:08:44.757287 bahire-hasab-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:08:44.757287 bahire-hasab-0.2.5/src/bahire_hasab/
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-05-31 13:08:28.000000 bahire-hasab-0.2.5/src/bahire_hasab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:08:44.757287 bahire-hasab-0.2.5/src/bahire_hasab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-31 13:08:44.000000 bahire-hasab-0.2.5/src/bahire_hasab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-31 13:08:44.000000 bahire-hasab-0.2.5/src/bahire_hasab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:08:44.000000 bahire-hasab-0.2.5/src/bahire_hasab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 13:08:44.000000 bahire-hasab-0.2.5/src/bahire_hasab.egg-info/top_level.txt
```

### Comparing `bahire-hasab-0.2.4/LICENSE` & `bahire-hasab-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bahire-hasab-0.2.4/PKG-INFO` & `bahire-hasab-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bahire-hasab
-Version: 0.2.4
+Version: 0.2.5
 Home-page: https://github.com/hunderaweke/bahire-hasab
 Author: Hundera Awoke
 Author-email: hunderaweke@gmail.com
 Keywords: bahire_hasab
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.4 Home-page: https://
+Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.5 Home-page: https://
 github.com/hunderaweke/bahire-hasab Author: Hundera Awoke Author-email:
 hunderaweke@gmail.com Keywords: bahire_hasab Description-Content-Type: text/
 markdown License-File: LICENSE
       ****** ð Bahire Hassab(á£áá¨ áá³á¥) ðªð¹ ð¦ ******
 [![Upload Python Package](https://github.com/hunderaweke/bahire-hasab/actions/
 workflows/python-publish.yml/badge.svg)](https://github.com/hunderaweke/bahire-
 hasab/actions/workflows/python-publish.yml) - A python module for calculating
```

### Comparing `bahire-hasab-0.2.4/README.md` & `bahire-hasab-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `bahire-hasab-0.2.4/src/bahire_hasab/__init__.py` & `bahire-hasab-0.2.5/src/bahire_hasab/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     @property
     def neneweh(self) -> str:
         """A function for finding the date of Nenewh Lent."""
         _l = [i for i in self.beale_metk.split()]
         _mh = self.mebaja_hamer
         if _mh > 30:
             _w = "የካቲት"
-            _mh % 30
+            _mh %= 30
         elif self.metk == 30 or self.metk == 0:
             _w = "የካቲት"
         elif _l[0] == "መስከረም":
             _w = "ጥር"
         else:
             _w = "የካቲት"
         return f"{_w} {_mh}"
```

### Comparing `bahire-hasab-0.2.4/src/bahire_hasab.egg-info/PKG-INFO` & `bahire-hasab-0.2.5/src/bahire_hasab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bahire-hasab
-Version: 0.2.4
+Version: 0.2.5
 Home-page: https://github.com/hunderaweke/bahire-hasab
 Author: Hundera Awoke
 Author-email: hunderaweke@gmail.com
 Keywords: bahire_hasab
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.4 Home-page: https://
+Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.5 Home-page: https://
 github.com/hunderaweke/bahire-hasab Author: Hundera Awoke Author-email:
 hunderaweke@gmail.com Keywords: bahire_hasab Description-Content-Type: text/
 markdown License-File: LICENSE
       ****** ð Bahire Hassab(á£áá¨ áá³á¥) ðªð¹ ð¦ ******
 [![Upload Python Package](https://github.com/hunderaweke/bahire-hasab/actions/
 workflows/python-publish.yml/badge.svg)](https://github.com/hunderaweke/bahire-
 hasab/actions/workflows/python-publish.yml) - A python module for calculating
```

