# Comparing `tmp/crio-0.0.3.tar.gz` & `tmp/crio-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\work\crio_proj\dist\.tmp-zglir_0z\crio-0.0.3.tar", last modified: Wed May 31 07:33:16 2023, max compression
+gzip compressed data, was "C:\work\crio_proj\dist\.tmp-x3mnl8cn\crio-0.0.4.tar", last modified: Wed May 31 07:34:18 2023, max compression
```

## Comparing `crio-0.0.3.tar` & `crio-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 07:33:16.942677 crio-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-02-21 00:14:59.000000 crio-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1655 2023-05-31 07:33:16.938667 crio-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       82 2023-05-31 07:02:25.000000 crio-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 07:33:16.803310 crio-0.0.3/crio/
-drwxrwxrwx   0        0        0        0 2023-05-31 07:33:16.850514 crio-0.0.3/crio/Loadini/
--rw-rw-rw-   0        0        0     4372 2022-03-19 15:07:32.000000 crio-0.0.3/crio/Loadini/Loadini.py
--rw-rw-rw-   0        0        0       28 2022-02-07 03:30:22.000000 crio-0.0.3/crio/Loadini/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:33:16.885945 crio-0.0.3/crio/UDP/
--rw-rw-rw-   0        0        0     8772 2023-02-16 04:32:48.000000 crio-0.0.3/crio/UDP/UDP.py
--rw-rw-rw-   0        0        0       20 2022-02-07 03:30:22.000000 crio-0.0.3/crio/UDP/__init__.py
--rw-rw-rw-   0        0        0       23 2023-05-31 06:07:38.000000 crio-0.0.3/crio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:33:16.891991 crio-0.0.3/crio/config/
--rw-rw-rw-   0        0        0       23 2023-05-31 06:07:38.000000 crio-0.0.3/crio/config/__init__.py
--rw-rw-rw-   0        0        0    18350 2023-05-31 07:01:53.000000 crio-0.0.3/crio/crio.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:33:16.926556 crio-0.0.3/crio/crio_hs/
--rw-rw-rw-   0        0        0       22 2022-02-07 03:30:22.000000 crio-0.0.3/crio/crio_hs/__init__.py
--rw-rw-rw-   0        0        0    15939 2022-02-07 03:30:22.000000 crio-0.0.3/crio/crio_hs/crio_hs.py
--rw-rw-rw-   0        0        0     1106 2023-02-10 02:00:30.000000 crio-0.0.3/crio/getBenchIni.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:33:16.934847 crio-0.0.3/crio/inis/
--rw-rw-rw-   0        0        0       23 2023-05-31 06:07:38.000000 crio-0.0.3/crio/inis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:33:16.817947 crio-0.0.3/crio.egg-info/
--rw-rw-rw-   0        0        0     1655 2023-05-31 07:33:16.000000 crio-0.0.3/crio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-05-31 07:33:16.000000 crio-0.0.3/crio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 07:33:16.000000 crio-0.0.3/crio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-31 07:33:16.000000 crio-0.0.3/crio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      451 2023-05-31 07:32:57.000000 crio-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 07:33:16.944112 crio-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 07:34:18.673297 crio-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 00:14:59.000000 crio-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1655 2023-05-31 07:34:18.671299 crio-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2023-05-31 07:02:25.000000 crio-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 07:34:18.627298 crio-0.0.4/crio/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:34:18.651279 crio-0.0.4/crio/Loadini/
+-rw-rw-rw-   0        0        0     4372 2022-03-19 15:07:32.000000 crio-0.0.4/crio/Loadini/Loadini.py
+-rw-rw-rw-   0        0        0       28 2022-02-07 03:30:22.000000 crio-0.0.4/crio/Loadini/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:34:18.657270 crio-0.0.4/crio/UDP/
+-rw-rw-rw-   0        0        0     8772 2023-02-16 04:32:48.000000 crio-0.0.4/crio/UDP/UDP.py
+-rw-rw-rw-   0        0        0       20 2022-02-07 03:30:22.000000 crio-0.0.4/crio/UDP/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-31 06:07:38.000000 crio-0.0.4/crio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:34:18.660276 crio-0.0.4/crio/config/
+-rw-rw-rw-   0        0        0       23 2023-05-31 06:07:38.000000 crio-0.0.4/crio/config/__init__.py
+-rw-rw-rw-   0        0        0    18350 2023-05-31 07:01:53.000000 crio-0.0.4/crio/crio.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:34:18.666287 crio-0.0.4/crio/crio_hs/
+-rw-rw-rw-   0        0        0       22 2022-02-07 03:30:22.000000 crio-0.0.4/crio/crio_hs/__init__.py
+-rw-rw-rw-   0        0        0    15939 2022-02-07 03:30:22.000000 crio-0.0.4/crio/crio_hs/crio_hs.py
+-rw-rw-rw-   0        0        0     1106 2023-02-10 02:00:30.000000 crio-0.0.4/crio/getBenchIni.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:34:18.668296 crio-0.0.4/crio/inis/
+-rw-rw-rw-   0        0        0       23 2023-05-31 06:07:38.000000 crio-0.0.4/crio/inis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:34:18.646160 crio-0.0.4/crio.egg-info/
+-rw-rw-rw-   0        0        0     1655 2023-05-31 07:34:18.000000 crio-0.0.4/crio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-05-31 07:34:18.000000 crio-0.0.4/crio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 07:34:18.000000 crio-0.0.4/crio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-31 07:34:18.000000 crio-0.0.4/crio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      451 2023-05-31 07:33:59.000000 crio-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 07:34:18.680755 crio-0.0.4/setup.cfg
```

### Comparing `crio-0.0.3/LICENSE` & `crio-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `crio-0.0.3/PKG-INFO` & `crio-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crio
-Version: 0.0.3
+Version: 0.0.4
 Summary: library for CRIO operation
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `crio-0.0.3/crio/Loadini/Loadini.py` & `crio-0.0.4/crio/Loadini/Loadini.py`

 * *Files identical despite different names*

### Comparing `crio-0.0.3/crio/UDP/UDP.py` & `crio-0.0.4/crio/UDP/UDP.py`

 * *Files identical despite different names*

### Comparing `crio-0.0.3/crio/crio.py` & `crio-0.0.4/crio/crio.py`

 * *Files identical despite different names*

### Comparing `crio-0.0.3/crio/crio_hs/crio_hs.py` & `crio-0.0.4/crio/crio_hs/crio_hs.py`

 * *Files identical despite different names*

### Comparing `crio-0.0.3/crio/getBenchIni.py` & `crio-0.0.4/crio/getBenchIni.py`

 * *Files identical despite different names*

### Comparing `crio-0.0.3/crio.egg-info/PKG-INFO` & `crio-0.0.4/crio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crio
-Version: 0.0.3
+Version: 0.0.4
 Summary: library for CRIO operation
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

