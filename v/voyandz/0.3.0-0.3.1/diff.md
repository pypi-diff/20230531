# Comparing `tmp/voyandz-0.3.0.tar.gz` & `tmp/voyandz-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voyandz-0.3.0.tar", last modified: Tue May 30 13:22:21 2023, max compression
+gzip compressed data, was "voyandz-0.3.1.tar", last modified: Wed May 31 15:10:56 2023, max compression
```

## Comparing `voyandz-0.3.0.tar` & `voyandz-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2023-05-30 13:22:21.761526 voyandz-0.3.0/
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     1103 2023-05-30 08:12:33.000000 voyandz-0.3.0/LICENSE
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       76 2023-05-30 13:21:52.000000 voyandz-0.3.0/MANIFEST.in
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     6029 2023-05-30 13:22:21.761526 voyandz-0.3.0/PKG-INFO
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     4430 2023-05-30 13:21:52.000000 voyandz-0.3.0/README.md
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      602 2023-05-30 13:22:21.761526 voyandz-0.3.0/setup.cfg
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       54 2023-05-30 13:15:38.000000 voyandz-0.3.0/setup.py
-drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2023-05-30 13:22:21.761526 voyandz-0.3.0/src/
-drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2023-05-30 13:22:21.761526 voyandz-0.3.0/src/voyandz/
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      140 2023-05-30 13:15:38.000000 voyandz-0.3.0/src/voyandz/__init__.py
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     1742 2023-05-30 13:15:38.000000 voyandz-0.3.0/src/voyandz/cli.py
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     3628 2023-05-30 13:15:38.000000 voyandz-0.3.0/src/voyandz/config.py
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     2496 2023-05-30 13:15:38.000000 voyandz-0.3.0/src/voyandz/logging.py
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)    24883 2023-05-30 13:15:38.000000 voyandz-0.3.0/src/voyandz/piping.py
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     5887 2023-05-30 13:21:52.000000 voyandz-0.3.0/src/voyandz/server.py
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     1767 2023-05-30 13:15:38.000000 voyandz-0.3.0/src/voyandz/stats.py
-drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2023-05-30 13:22:21.761526 voyandz-0.3.0/src/voyandz/templates/
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      703 2023-05-30 13:15:38.000000 voyandz-0.3.0/src/voyandz/templates/home.html
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     2150 2023-05-30 13:21:52.000000 voyandz-0.3.0/src/voyandz/templates/stat.html
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      476 2023-05-30 13:15:38.000000 voyandz-0.3.0/src/voyandz/util.py
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       76 2023-05-30 13:21:52.000000 voyandz-0.3.0/src/voyandz/version.py
-drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2023-05-30 13:22:21.761526 voyandz-0.3.0/src/voyandz.egg-info/
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     6029 2023-05-30 13:22:21.000000 voyandz-0.3.0/src/voyandz.egg-info/PKG-INFO
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      554 2023-05-30 13:22:21.000000 voyandz-0.3.0/src/voyandz.egg-info/SOURCES.txt
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)        1 2023-05-30 13:22:21.000000 voyandz-0.3.0/src/voyandz.egg-info/dependency_links.txt
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       46 2023-05-30 13:22:21.000000 voyandz-0.3.0/src/voyandz.egg-info/entry_points.txt
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)        1 2023-05-30 13:22:21.000000 voyandz-0.3.0/src/voyandz.egg-info/not-zip-safe
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       25 2023-05-30 13:22:21.000000 voyandz-0.3.0/src/voyandz.egg-info/requires.txt
--rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)        8 2023-05-30 13:22:21.000000 voyandz-0.3.0/src/voyandz.egg-info/top_level.txt
+drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2023-05-31 15:10:56.507325 voyandz-0.3.1/
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     1103 2023-05-30 08:12:33.000000 voyandz-0.3.1/LICENSE
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       76 2023-05-30 13:32:11.000000 voyandz-0.3.1/MANIFEST.in
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     6097 2023-05-31 15:10:56.507325 voyandz-0.3.1/PKG-INFO
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     4459 2023-05-31 14:55:08.000000 voyandz-0.3.1/README.md
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      626 2023-05-31 15:10:56.507325 voyandz-0.3.1/setup.cfg
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       54 2023-05-31 14:54:09.000000 voyandz-0.3.1/setup.py
+drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2023-05-31 15:10:56.507325 voyandz-0.3.1/src/
+drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2023-05-31 15:10:56.507325 voyandz-0.3.1/src/voyandz/
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      140 2023-05-31 14:55:08.000000 voyandz-0.3.1/src/voyandz/__init__.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     1719 2023-05-31 14:55:35.000000 voyandz-0.3.1/src/voyandz/cli.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     3628 2023-05-31 14:55:08.000000 voyandz-0.3.1/src/voyandz/config.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     2496 2023-05-30 13:15:38.000000 voyandz-0.3.1/src/voyandz/logging.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)    24883 2023-05-30 13:15:38.000000 voyandz-0.3.1/src/voyandz/piping.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     5887 2023-05-31 14:55:08.000000 voyandz-0.3.1/src/voyandz/server.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     1767 2023-05-30 13:15:38.000000 voyandz-0.3.1/src/voyandz/stats.py
+drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2023-05-31 15:10:56.507325 voyandz-0.3.1/src/voyandz/templates/
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      703 2023-05-30 13:15:38.000000 voyandz-0.3.1/src/voyandz/templates/home.html
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     2150 2023-05-31 10:21:12.000000 voyandz-0.3.1/src/voyandz/templates/stat.html
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      476 2023-05-30 13:15:38.000000 voyandz-0.3.1/src/voyandz/util.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       76 2023-05-31 14:57:14.000000 voyandz-0.3.1/src/voyandz/version.py
+drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2023-05-31 15:10:56.507325 voyandz-0.3.1/src/voyandz.egg-info/
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     6097 2023-05-31 15:10:56.000000 voyandz-0.3.1/src/voyandz.egg-info/PKG-INFO
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      554 2023-05-31 15:10:56.000000 voyandz-0.3.1/src/voyandz.egg-info/SOURCES.txt
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)        1 2023-05-31 15:10:56.000000 voyandz-0.3.1/src/voyandz.egg-info/dependency_links.txt
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       46 2023-05-31 15:10:56.000000 voyandz-0.3.1/src/voyandz.egg-info/entry_points.txt
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)        1 2023-05-31 15:10:56.000000 voyandz-0.3.1/src/voyandz.egg-info/not-zip-safe
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       25 2023-05-31 15:10:56.000000 voyandz-0.3.1/src/voyandz.egg-info/requires.txt
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)        8 2023-05-31 15:10:56.000000 voyandz-0.3.1/src/voyandz.egg-info/top_level.txt
```

### Comparing `voyandz-0.3.0/LICENSE` & `voyandz-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `voyandz-0.3.0/PKG-INFO` & `voyandz-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voyandz
-Version: 0.3.0
+Version: 0.3.1
 Summary: an AV HTTP piping server
 Home-page: https://github.com/Zalewa/voyandz
 Author: Robikz
 Author-email: zalewapl@gmail.com
 License: MIT
 Description: Voyandz
         =======
@@ -115,19 +115,21 @@
         
         Repository Structure
         ====================
         
         Project file structure should adhere to the practices
         recommended for Python and Flask projects.
         
+        The src layout is used.
+        
         ```
           .
           |- config - example configuration files
           |- sandbox - development scraps, experiments
-          \- voyandz - application code
+          \- src/voyandz - application code
         ```
         
         Name
         ====
         
         The name is `voyandz`, all lower-case. V stands for video,
         A stands for Audio, the rest is gibberish.
@@ -171,8 +173,9 @@
         `/etc/sysctl.d/`.
         
         More info: http://man7.org/linux/man-pages/man7/pipe.7.html
         
         Keywords: pipe-user-pages-soft, PermissionError, Operation not permitted
         
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `voyandz-0.3.0/README.md` & `voyandz-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -107,19 +107,21 @@
 
 Repository Structure
 ====================
 
 Project file structure should adhere to the practices
 recommended for Python and Flask projects.
 
+The src layout is used.
+
 ```
   .
   |- config - example configuration files
   |- sandbox - development scraps, experiments
-  \- voyandz - application code
+  \- src/voyandz - application code
 ```
 
 Name
 ====
 
 The name is `voyandz`, all lower-case. V stands for video,
 A stands for Audio, the rest is gibberish.
```

### Comparing `voyandz-0.3.0/setup.cfg` & `voyandz-0.3.1/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 include_package_data = True
 install_requires = 
 	Flask==2.2.*
 	PyYAML==6.*
 packages = find:
 package_dir = 
 	= src
+python_requires = >=3.7
 zip_safe = False
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts =
```

### Comparing `voyandz-0.3.0/src/voyandz/cli.py` & `voyandz-0.3.1/src/voyandz/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,16 +31,16 @@
             pstats = yappi.convert2pstats(yappi.get_func_stats())
             pstats.dump_stats(profile_file)
             with open(profile_file + ".threads", "w") as threads_file:
                 yappi.get_thread_stats().print_all(threads_file)
 
 
 def print_version(file=sys.stderr):
-    print("{} ({}) {} ({})".format(
-        version.FULLNAME, voyandz.__name__,
+    print("{} {} ({})".format(
+        version.FULLNAME,
         version.VERSION, version.YEARSPAN),
         file=file)
     print("On MIT License; no warranty", file=file)
 
 
 def parse_args():
     opt_parser = OptionParser()
```

### Comparing `voyandz-0.3.0/src/voyandz/config.py` & `voyandz-0.3.1/src/voyandz/config.py`

 * *Files identical despite different names*

### Comparing `voyandz-0.3.0/src/voyandz/logging.py` & `voyandz-0.3.1/src/voyandz/logging.py`

 * *Files identical despite different names*

### Comparing `voyandz-0.3.0/src/voyandz/piping.py` & `voyandz-0.3.1/src/voyandz/piping.py`

 * *Files identical despite different names*

### Comparing `voyandz-0.3.0/src/voyandz/server.py` & `voyandz-0.3.1/src/voyandz/server.py`

 * *Files identical despite different names*

### Comparing `voyandz-0.3.0/src/voyandz/stats.py` & `voyandz-0.3.1/src/voyandz/stats.py`

 * *Files identical despite different names*

### Comparing `voyandz-0.3.0/src/voyandz/templates/home.html` & `voyandz-0.3.1/src/voyandz/templates/home.html`

 * *Files identical despite different names*

### Comparing `voyandz-0.3.0/src/voyandz/templates/stat.html` & `voyandz-0.3.1/src/voyandz/templates/stat.html`

 * *Files identical despite different names*

### Comparing `voyandz-0.3.0/src/voyandz.egg-info/PKG-INFO` & `voyandz-0.3.1/src/voyandz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voyandz
-Version: 0.3.0
+Version: 0.3.1
 Summary: an AV HTTP piping server
 Home-page: https://github.com/Zalewa/voyandz
 Author: Robikz
 Author-email: zalewapl@gmail.com
 License: MIT
 Description: Voyandz
         =======
@@ -115,19 +115,21 @@
         
         Repository Structure
         ====================
         
         Project file structure should adhere to the practices
         recommended for Python and Flask projects.
         
+        The src layout is used.
+        
         ```
           .
           |- config - example configuration files
           |- sandbox - development scraps, experiments
-          \- voyandz - application code
+          \- src/voyandz - application code
         ```
         
         Name
         ====
         
         The name is `voyandz`, all lower-case. V stands for video,
         A stands for Audio, the rest is gibberish.
@@ -171,8 +173,9 @@
         `/etc/sysctl.d/`.
         
         More info: http://man7.org/linux/man-pages/man7/pipe.7.html
         
         Keywords: pipe-user-pages-soft, PermissionError, Operation not permitted
         
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `voyandz-0.3.0/src/voyandz.egg-info/SOURCES.txt` & `voyandz-0.3.1/src/voyandz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

