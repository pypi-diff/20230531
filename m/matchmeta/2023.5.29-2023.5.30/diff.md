# Comparing `tmp/matchmeta-2023.5.29.tar.gz` & `tmp/matchmeta-2023.5.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matchmeta-2023.5.29.tar", last modified: Sun May 28 22:32:20 2023, max compression
+gzip compressed data, was "matchmeta-2023.5.30.tar", last modified: Wed May 31 00:29:35 2023, max compression
```

## Comparing `matchmeta-2023.5.29.tar` & `matchmeta-2023.5.30.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:32:20.587558 matchmeta-2023.5.29/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-28 22:32:09.000000 matchmeta-2023.5.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-28 22:32:20.587558 matchmeta-2023.5.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-28 22:32:09.000000 matchmeta-2023.5.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:32:20.587558 matchmeta-2023.5.29/matchmeta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-28 22:32:20.000000 matchmeta-2023.5.29/matchmeta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-28 22:32:20.000000 matchmeta-2023.5.29/matchmeta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 22:32:20.000000 matchmeta-2023.5.29/matchmeta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-28 22:32:20.000000 matchmeta-2023.5.29/matchmeta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-28 22:32:20.000000 matchmeta-2023.5.29/matchmeta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-28 22:32:20.000000 matchmeta-2023.5.29/matchmeta.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:32:20.587558 matchmeta-2023.5.29/mmi/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-28 22:32:09.000000 matchmeta-2023.5.29/mmi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-28 22:32:09.000000 matchmeta-2023.5.29/mmi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-05-28 22:32:09.000000 matchmeta-2023.5.29/mmi/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 22:32:20.587558 matchmeta-2023.5.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-28 22:32:09.000000 matchmeta-2023.5.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:29:35.569254 matchmeta-2023.5.30/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 00:29:24.000000 matchmeta-2023.5.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-31 00:29:35.569254 matchmeta-2023.5.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-31 00:29:24.000000 matchmeta-2023.5.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:29:35.565253 matchmeta-2023.5.30/matchmeta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-31 00:29:35.000000 matchmeta-2023.5.30/matchmeta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-31 00:29:35.000000 matchmeta-2023.5.30/matchmeta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:29:35.000000 matchmeta-2023.5.30/matchmeta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 00:29:35.000000 matchmeta-2023.5.30/matchmeta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 00:29:35.000000 matchmeta-2023.5.30/matchmeta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-31 00:29:35.000000 matchmeta-2023.5.30/matchmeta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:29:35.565253 matchmeta-2023.5.30/mmi/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-31 00:29:24.000000 matchmeta-2023.5.30/mmi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-31 00:29:24.000000 matchmeta-2023.5.30/mmi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-05-31 00:29:24.000000 matchmeta-2023.5.30/mmi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 00:29:35.569254 matchmeta-2023.5.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-31 00:29:24.000000 matchmeta-2023.5.30/setup.py
```

### Comparing `matchmeta-2023.5.29/LICENSE` & `matchmeta-2023.5.30/LICENSE`

 * *Files identical despite different names*

### Comparing `matchmeta-2023.5.29/PKG-INFO` & `matchmeta-2023.5.30/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,19 @@
-Metadata-Version: 2.1
-Name: matchmeta
-Version: 2023.5.29
-Summary: OS Triage for Anyone and Everyone
-Home-page: https://github.com/jblukach/mmi
-Author: John Lukach
-Author-email: hello@lukach.io
-License: Apache-2.0
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # mmi
 
 Metadata is the lowest-value indicator as easy to circumvent. Still, with the exponential volume of directories and files standard on default operating system installations, finding things hiding in plain sight has become an important analysis technique.
 
 ```
 MMI - OS Triage for Anyone and Everyone
 
 options:
   -h, --help      show this help message and exit
   -d, --download  Download Bloom Filters
   -s, --skip      Skip File Hashing
+  -u, --updated   Bloom Filters Last Updated
   -v, --version   show program's version number and exit
   ```
 
 ### DATASET
 
 GetBlocks generates the dataset using the SHA256 format for directories, files, hashes, and paths.
 
@@ -54,14 +43,26 @@
 
 https://static.matchmeta.info/mmi.sha256
 
 It is available for download if you're interested in the raw data using API keys available through self-registration.
 
 https://store.lukach.io/l/sha256
 
+### LAST UPDATED
+
+Check when the bloom filters were last updated using the command line interface (CLI).
+
+```
+mmi -u
+```
+
+Or by hitting the provided website for the last updated timestamp.
+
+https://static.matchmeta.info/mmi.updated
+
 ### DETECTIONS
 
 :purple_square: Empty File (purple) 
 
 A zero byte size determines empty files or the following hash value for this detection.
 
 ```E3B0C44298FC1C149AFBF4C8996FB92427AE41E4649B934CA495991B7852B855```
@@ -114,8 +115,8 @@
 pip install matchmeta
 ```
 
 ### DEVELOPMENT
 
 ```
 python setup.py install --user
-```
+```
```

### Comparing `matchmeta-2023.5.29/README.md` & `matchmeta-2023.5.30/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,31 @@
+Metadata-Version: 2.1
+Name: matchmeta
+Version: 2023.5.30
+Summary: OS Triage for Anyone and Everyone
+Home-page: https://github.com/jblukach/mmi
+Author: John Lukach
+Author-email: hello@lukach.io
+License: Apache-2.0
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # mmi
 
 Metadata is the lowest-value indicator as easy to circumvent. Still, with the exponential volume of directories and files standard on default operating system installations, finding things hiding in plain sight has become an important analysis technique.
 
 ```
 MMI - OS Triage for Anyone and Everyone
 
 options:
   -h, --help      show this help message and exit
   -d, --download  Download Bloom Filters
   -s, --skip      Skip File Hashing
+  -u, --updated   Bloom Filters Last Updated
   -v, --version   show program's version number and exit
   ```
 
 ### DATASET
 
 GetBlocks generates the dataset using the SHA256 format for directories, files, hashes, and paths.
 
@@ -42,14 +55,26 @@
 
 https://static.matchmeta.info/mmi.sha256
 
 It is available for download if you're interested in the raw data using API keys available through self-registration.
 
 https://store.lukach.io/l/sha256
 
+### LAST UPDATED
+
+Check when the bloom filters were last updated using the command line interface (CLI).
+
+```
+mmi -u
+```
+
+Or by hitting the provided website for the last updated timestamp.
+
+https://static.matchmeta.info/mmi.updated
+
 ### DETECTIONS
 
 :purple_square: Empty File (purple) 
 
 A zero byte size determines empty files or the following hash value for this detection.
 
 ```E3B0C44298FC1C149AFBF4C8996FB92427AE41E4649B934CA495991B7852B855```
@@ -102,8 +127,8 @@
 pip install matchmeta
 ```
 
 ### DEVELOPMENT
 
 ```
 python setup.py install --user
-```
+```
```

### Comparing `matchmeta-2023.5.29/matchmeta.egg-info/PKG-INFO` & `matchmeta-2023.5.30/matchmeta.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchmeta
-Version: 2023.5.29
+Version: 2023.5.30
 Summary: OS Triage for Anyone and Everyone
 Home-page: https://github.com/jblukach/mmi
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -17,14 +17,15 @@
 ```
 MMI - OS Triage for Anyone and Everyone
 
 options:
   -h, --help      show this help message and exit
   -d, --download  Download Bloom Filters
   -s, --skip      Skip File Hashing
+  -u, --updated   Bloom Filters Last Updated
   -v, --version   show program's version number and exit
   ```
 
 ### DATASET
 
 GetBlocks generates the dataset using the SHA256 format for directories, files, hashes, and paths.
 
@@ -54,14 +55,26 @@
 
 https://static.matchmeta.info/mmi.sha256
 
 It is available for download if you're interested in the raw data using API keys available through self-registration.
 
 https://store.lukach.io/l/sha256
 
+### LAST UPDATED
+
+Check when the bloom filters were last updated using the command line interface (CLI).
+
+```
+mmi -u
+```
+
+Or by hitting the provided website for the last updated timestamp.
+
+https://static.matchmeta.info/mmi.updated
+
 ### DETECTIONS
 
 :purple_square: Empty File (purple) 
 
 A zero byte size determines empty files or the following hash value for this detection.
 
 ```E3B0C44298FC1C149AFBF4C8996FB92427AE41E4649B934CA495991B7852B855```
```

### Comparing `matchmeta-2023.5.29/mmi/__init__.py` & `matchmeta-2023.5.30/mmi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 __largefile__ = LARGEFILE = '\033[91m{}\033[00m'        ### RED ###
 __nofilehash__ = NOFILEHASH = '\033[93m{}\033[00m'      ### YELLOW ###
 __partialmeta__ = PARTIALMETA = '\033[97m{}\033[00m'    ### GREY ###
 
 __gtfo__ = GTFO = pathlib.Path.joinpath(pathlib.Path.home(), 'gtfo.bloom')
 __mmi__ = MMI = pathlib.Path.joinpath(pathlib.Path.home(), 'mmi.bloom')
 
-__version__ = VERSION = '2023.5.29'
+__version__ = VERSION = '2023.5.30'
```

### Comparing `matchmeta-2023.5.29/mmi/cli.py` & `matchmeta-2023.5.30/mmi/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -277,24 +277,37 @@
             slash = __largefile__.format('/')
 
             if str(p.parent) == '/':
                 print(denied+' '+sha256+' '+dir+file)
             else:
                 print(denied+' '+sha256+' '+dir+slash+file)
 
+def updated():
+
+    r = requests.get('https://static.matchmeta.info/mmi.updated')
+    if r.status_code == 200:
+        print('SUCCESS: https://static.matchmeta.info/mmi.updated')
+        print('LAST UPDATED: '+r.text)
+    else:
+        print('FAILED: https://static.matchmeta.info/mmi.updated')
+        sys.exit(1)
+
 def main():
 
     parser = argparse.ArgumentParser(description='MMI - OS Triage for Anyone and Everyone')
     parser.add_argument('-d', '--download', help='Download Bloom Filters', action='store_true')
     parser.add_argument('-s', '--skip', help='Skip File Hashing', action='store_true')
+    parser.add_argument('-u', '--updated', help='Bloom Filters Last Updated', action='store_true')
     parser.add_argument('-v', '--version', action='version', version=__version__)
     args = parser.parse_args()
 
     if args.download:
         download()
+    elif args.updated:
+        updated()
     else:
         if __mmi__.is_file() == False:
             print('MISSING: '+str(__mmi__))
         elif __gtfo__.is_file() == False:
             print('MISSING: '+str(__gtfo__))
         else:
             with concurrent.futures.ThreadPoolExecutor() as executor:
```

### Comparing `matchmeta-2023.5.29/setup.py` & `matchmeta-2023.5.30/setup.py`

 * *Files identical despite different names*

