# Comparing `tmp/sqdconvert-1.0.0.tar.gz` & `tmp/sqdconvert-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqdconvert-1.0.0.tar", last modified: Wed May 31 14:08:22 2023, max compression
+gzip compressed data, was "sqdconvert-1.0.1.tar", last modified: Wed May 31 14:39:38 2023, max compression
```

## Comparing `sqdconvert-1.0.0.tar` & `sqdconvert-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 14:08:22.981453 sqdconvert-1.0.0/
--rw-rw-rw-   0        0        0     1083 2023-05-27 21:58:15.000000 sqdconvert-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       33 2022-10-15 13:34:47.000000 sqdconvert-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1701 2023-05-31 14:08:22.979433 sqdconvert-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       36 2023-05-27 22:00:40.000000 sqdconvert-1.0.0/README.md
--rw-rw-rw-   0        0        0      586 2023-05-31 14:07:27.000000 sqdconvert-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 14:08:22.981453 sqdconvert-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       36 2022-10-14 07:04:07.000000 sqdconvert-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:08:22.824484 sqdconvert-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 14:08:22.910095 sqdconvert-1.0.0/src/sqdconvert/
--rw-rw-rw-   0        0        0      388 2023-05-31 14:07:39.000000 sqdconvert-1.0.0/src/sqdconvert/__init__.py
--rw-rw-rw-   0        0        0     1301 2023-05-31 13:47:28.000000 sqdconvert-1.0.0/src/sqdconvert/__main__.py
--rw-rw-rw-   0        0        0      825 2022-10-16 06:41:48.000000 sqdconvert-1.0.0/src/sqdconvert/color.py
--rw-rw-rw-   0        0        0     2482 2023-05-31 11:05:18.000000 sqdconvert-1.0.0/src/sqdconvert/config.py
--rw-rw-rw-   0        0        0      808 2023-05-31 13:22:38.000000 sqdconvert-1.0.0/src/sqdconvert/errors.py
--rw-rw-rw-   0        0        0     2570 2023-05-31 13:50:23.000000 sqdconvert-1.0.0/src/sqdconvert/start.py
--rw-rw-rw-   0        0        0      219 2023-05-31 10:23:22.000000 sqdconvert-1.0.0/src/sqdconvert/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:08:22.975432 sqdconvert-1.0.0/src/sqdconvert.egg-info/
--rw-rw-rw-   0        0        0     1701 2023-05-31 14:08:22.000000 sqdconvert-1.0.0/src/sqdconvert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-05-31 14:08:22.000000 sqdconvert-1.0.0/src/sqdconvert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 14:08:22.000000 sqdconvert-1.0.0/src/sqdconvert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-31 14:08:22.000000 sqdconvert-1.0.0/src/sqdconvert.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 14:08:22.000000 sqdconvert-1.0.0/src/sqdconvert.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-31 14:08:22.000000 sqdconvert-1.0.0/src/sqdconvert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 14:39:38.519025 sqdconvert-1.0.1/
+-rw-rw-rw-   0        0        0     1083 2023-05-27 21:58:15.000000 sqdconvert-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       33 2022-10-15 13:34:47.000000 sqdconvert-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1740 2023-05-31 14:39:38.516829 sqdconvert-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       75 2023-05-31 14:38:03.000000 sqdconvert-1.0.1/README.md
+-rw-rw-rw-   0        0        0      586 2023-05-31 14:38:54.000000 sqdconvert-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 14:39:38.519823 sqdconvert-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       36 2022-10-14 07:04:07.000000 sqdconvert-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:39:38.340208 sqdconvert-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 14:39:38.438143 sqdconvert-1.0.1/src/sqdconvert/
+-rw-rw-rw-   0        0        0      388 2023-05-31 14:38:51.000000 sqdconvert-1.0.1/src/sqdconvert/__init__.py
+-rw-rw-rw-   0        0        0     1326 2023-05-31 14:38:38.000000 sqdconvert-1.0.1/src/sqdconvert/__main__.py
+-rw-rw-rw-   0        0        0      825 2022-10-16 06:41:48.000000 sqdconvert-1.0.1/src/sqdconvert/color.py
+-rw-rw-rw-   0        0        0     2482 2023-05-31 11:05:18.000000 sqdconvert-1.0.1/src/sqdconvert/config.py
+-rw-rw-rw-   0        0        0      808 2023-05-31 13:22:38.000000 sqdconvert-1.0.1/src/sqdconvert/errors.py
+-rw-rw-rw-   0        0        0     2570 2023-05-31 13:50:23.000000 sqdconvert-1.0.1/src/sqdconvert/start.py
+-rw-rw-rw-   0        0        0      219 2023-05-31 10:23:22.000000 sqdconvert-1.0.1/src/sqdconvert/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:39:38.511685 sqdconvert-1.0.1/src/sqdconvert.egg-info/
+-rw-rw-rw-   0        0        0     1740 2023-05-31 14:39:38.000000 sqdconvert-1.0.1/src/sqdconvert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-05-31 14:39:38.000000 sqdconvert-1.0.1/src/sqdconvert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 14:39:38.000000 sqdconvert-1.0.1/src/sqdconvert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-31 14:39:38.000000 sqdconvert-1.0.1/src/sqdconvert.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 14:39:38.000000 sqdconvert-1.0.1/src/sqdconvert.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-31 14:39:38.000000 sqdconvert-1.0.1/src/sqdconvert.egg-info/top_level.txt
```

### Comparing `sqdconvert-1.0.0/LICENSE` & `sqdconvert-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqdconvert-1.0.0/PKG-INFO` & `sqdconvert-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqdconvert
-Version: 1.0.0
+Version: 1.0.1
 Summary: convert any audio or video files from one extension to another!
 Author: sqdnoises
 License: The MIT License (MIT)
         
         Copyright (c) 2023-present SqdNoises
         
         Permission is hereby granted, free of charge, to any person obtaining a
@@ -27,8 +27,13 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-a cool screenshare program in python
+a cool media convertion program
+
+help command:
+```py
+sqdconvert -h
+```
```

### Comparing `sqdconvert-1.0.0/pyproject.toml` & `sqdconvert-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqdconvert"
-version = "1.0.0"
+version = "1.0.1"
 description = "convert any audio or video files from one extension to another!"
 authors = [
     { name="sqdnoises" }
 ]
 
 readme = "README.md"
 license = { file = "LICENSE" }
```

### Comparing `sqdconvert-1.0.0/src/sqdconvert/__main__.py` & `sqdconvert-1.0.1/src/sqdconvert/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,13 +24,15 @@
     parser.add_argument("-v", "--verbose",
                         action="store_true", help="print more output")
     parser.add_argument("-V", "--version",
                         action="version", version=name+" "+version)
     parser.add_argument("-l", "--license",
                         action="version", version=copyright+" - MIT License. For more information see: https://opensource.org/license/mit/",
                         help="show program's license and exit")
+    
+    config = get_config()
 
     args = parser.parse_args()
-    start(args, get_config())
+    start(args, config)
 
 if __name__ == "__main__":
     main()
```

### Comparing `sqdconvert-1.0.0/src/sqdconvert/color.py` & `sqdconvert-1.0.1/src/sqdconvert/color.py`

 * *Files identical despite different names*

### Comparing `sqdconvert-1.0.0/src/sqdconvert/config.py` & `sqdconvert-1.0.1/src/sqdconvert/config.py`

 * *Files identical despite different names*

### Comparing `sqdconvert-1.0.0/src/sqdconvert/errors.py` & `sqdconvert-1.0.1/src/sqdconvert/errors.py`

 * *Files identical despite different names*

### Comparing `sqdconvert-1.0.0/src/sqdconvert/start.py` & `sqdconvert-1.0.1/src/sqdconvert/start.py`

 * *Files identical despite different names*

### Comparing `sqdconvert-1.0.0/src/sqdconvert.egg-info/PKG-INFO` & `sqdconvert-1.0.1/src/sqdconvert.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqdconvert
-Version: 1.0.0
+Version: 1.0.1
 Summary: convert any audio or video files from one extension to another!
 Author: sqdnoises
 License: The MIT License (MIT)
         
         Copyright (c) 2023-present SqdNoises
         
         Permission is hereby granted, free of charge, to any person obtaining a
@@ -27,8 +27,13 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-a cool screenshare program in python
+a cool media convertion program
+
+help command:
+```py
+sqdconvert -h
+```
```

