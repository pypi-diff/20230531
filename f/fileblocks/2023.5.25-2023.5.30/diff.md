# Comparing `tmp/fileblocks-2023.5.25.tar.gz` & `tmp/fileblocks-2023.5.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fileblocks-2023.5.25.tar", last modified: Fri May 26 01:23:48 2023, max compression
+gzip compressed data, was "fileblocks-2023.5.30.tar", last modified: Wed May 31 00:48:27 2023, max compression
```

## Comparing `fileblocks-2023.5.25.tar` & `fileblocks-2023.5.30.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:23:48.661488 fileblocks-2023.5.25/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 01:23:35.000000 fileblocks-2023.5.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-26 01:23:48.661488 fileblocks-2023.5.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-05-26 01:23:35.000000 fileblocks-2023.5.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:23:48.657488 fileblocks-2023.5.25/fbi/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-26 01:23:35.000000 fileblocks-2023.5.25/fbi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-26 01:23:35.000000 fileblocks-2023.5.25/fbi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-26 01:23:35.000000 fileblocks-2023.5.25/fbi/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:23:48.661488 fileblocks-2023.5.25/fileblocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-26 01:23:48.000000 fileblocks-2023.5.25/fileblocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-26 01:23:48.000000 fileblocks-2023.5.25/fileblocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:23:48.000000 fileblocks-2023.5.25/fileblocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 01:23:48.000000 fileblocks-2023.5.25/fileblocks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 01:23:48.000000 fileblocks-2023.5.25/fileblocks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-26 01:23:48.000000 fileblocks-2023.5.25/fileblocks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 01:23:48.661488 fileblocks-2023.5.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-26 01:23:35.000000 fileblocks-2023.5.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:48:27.019164 fileblocks-2023.5.30/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 00:48:15.000000 fileblocks-2023.5.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-31 00:48:27.019164 fileblocks-2023.5.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-31 00:48:15.000000 fileblocks-2023.5.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:48:27.015164 fileblocks-2023.5.30/fbi/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-31 00:48:15.000000 fileblocks-2023.5.30/fbi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-31 00:48:15.000000 fileblocks-2023.5.30/fbi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-31 00:48:15.000000 fileblocks-2023.5.30/fbi/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:48:27.019164 fileblocks-2023.5.30/fileblocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-31 00:48:27.000000 fileblocks-2023.5.30/fileblocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-31 00:48:27.000000 fileblocks-2023.5.30/fileblocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:48:27.000000 fileblocks-2023.5.30/fileblocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 00:48:27.000000 fileblocks-2023.5.30/fileblocks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 00:48:27.000000 fileblocks-2023.5.30/fileblocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-31 00:48:27.000000 fileblocks-2023.5.30/fileblocks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 00:48:27.019164 fileblocks-2023.5.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-31 00:48:15.000000 fileblocks-2023.5.30/setup.py
```

### Comparing `fileblocks-2023.5.25/LICENSE` & `fileblocks-2023.5.30/LICENSE`

 * *Files identical despite different names*

### Comparing `fileblocks-2023.5.25/PKG-INFO` & `fileblocks-2023.5.30/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,22 @@
-Metadata-Version: 2.1
-Name: fileblocks
-Version: 2023.5.25
-Summary: Walk the line, Byte by Byte Analysis
-Home-page: https://github.com/jblukach/fbi
-Author: John Lukach
-Author-email: hello@lukach.io
-License: Apache-2.0
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # fbi
 
 Strings can be one of the quickest ways to analyze unknown binaries and memory images, even with corrupted acquisitions for low-hanging fruit.
 
 ```
 FBI - Walk the line, Byte by Byte Analysis
 
 options:
   -h, --help            show this help message and exit
   -b BLOCKS, --blocks BLOCKS
                         Input Filename
   -d, --download        Download Bloom Filter
   -o OUTPUT, --output OUTPUT
                         Output Directory
+  -u, --updated         Bloom Filter Last Updated
   -v, --version         show program's version number and exit
 ```
 
 ### CHALLENGES
 
 The first challenge is data encoding, as several applications only display ASCII characters with the potential for Unicode and UTF-8 to exist.
 
@@ -79,14 +68,26 @@
 
 https://b3.lukach.io/amzn/sector
 
 API keys are available using the self-registration process.
 
 https://store.lukach.io/l/b3
 
+### LAST UPDATED
+
+Check when the bloom filter was last updated using the command line interface (CLI).
+
+```
+fbi -u
+```
+
+Or by hitting the provided website for the last updated timestamp.
+
+https://static.fileblock.info/fbi.updated
+
 ### ANALYSIS
 
 The analyzed file allows both the absolute and relative location.
 
 ```
 fbi -b /usr/bin/df
 ```
@@ -118,8 +119,8 @@
 pip install fileblocks
 ```
 
 ### DEVELOPMENT
 
 ```
 python setup.py install --user
-```
+```
```

### Comparing `fileblocks-2023.5.25/README.md` & `fileblocks-2023.5.30/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,34 @@
+Metadata-Version: 2.1
+Name: fileblocks
+Version: 2023.5.30
+Summary: Walk the line, Byte by Byte Analysis
+Home-page: https://github.com/jblukach/fbi
+Author: John Lukach
+Author-email: hello@lukach.io
+License: Apache-2.0
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # fbi
 
 Strings can be one of the quickest ways to analyze unknown binaries and memory images, even with corrupted acquisitions for low-hanging fruit.
 
 ```
 FBI - Walk the line, Byte by Byte Analysis
 
 options:
   -h, --help            show this help message and exit
   -b BLOCKS, --blocks BLOCKS
                         Input Filename
   -d, --download        Download Bloom Filter
   -o OUTPUT, --output OUTPUT
                         Output Directory
+  -u, --updated         Bloom Filter Last Updated
   -v, --version         show program's version number and exit
 ```
 
 ### CHALLENGES
 
 The first challenge is data encoding, as several applications only display ASCII characters with the potential for Unicode and UTF-8 to exist.
 
@@ -67,14 +80,26 @@
 
 https://b3.lukach.io/amzn/sector
 
 API keys are available using the self-registration process.
 
 https://store.lukach.io/l/b3
 
+### LAST UPDATED
+
+Check when the bloom filter was last updated using the command line interface (CLI).
+
+```
+fbi -u
+```
+
+Or by hitting the provided website for the last updated timestamp.
+
+https://static.fileblock.info/fbi.updated
+
 ### ANALYSIS
 
 The analyzed file allows both the absolute and relative location.
 
 ```
 fbi -b /usr/bin/df
 ```
@@ -106,8 +131,8 @@
 pip install fileblocks
 ```
 
 ### DEVELOPMENT
 
 ```
 python setup.py install --user
-```
+```
```

### Comparing `fileblocks-2023.5.25/fbi/cli.py` & `fileblocks-2023.5.30/fbi/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,14 +90,24 @@
                                 pass
                             offset += 1
                         else:
                             offset += 512
             f.close()
         o.close()
 
+def updated():
+
+    r = requests.get('https://static.fileblock.info/fbi.updated')
+    if r.status_code == 200:
+        print('SUCCESS: https://static.fileblock.info/fbi.updated')
+        print('LAST UPDATED: '+r.text)
+    else:
+        print('FAILED: https://static.fileblock.info/fbi.updated')
+        sys.exit(1)
+
 def verify():
 
     r = requests.get('https://static.fileblock.info/fbi.sha256')
     if r.status_code == 200:
         print('SUCCESS: https://static.fileblock.info/fbi.sha256')
         return r.text
     else:
@@ -106,21 +116,24 @@
 
 def main():
 
     parser = argparse.ArgumentParser(description='FBI - Walk the line, Byte by Byte Analysis')
     parser.add_argument('-b', '--blocks', help='Input Filename', required=False)
     parser.add_argument('-d', '--download', help='Download Bloom Filter', action='store_true')
     parser.add_argument('-o', '--output', help='Output Directory', required=False)
+    parser.add_argument('-u', '--updated', help='Bloom Filter Last Updated', action='store_true')
     parser.add_argument('-v', '--version', action='version', version=__version__)
     args = parser.parse_args()
 
     if args.download:
         download()
     elif args.blocks:
         if args.output:
             output = args.output
         else:
             output = pathlib.Path().absolute()
         with concurrent.futures.ThreadPoolExecutor() as executor:
             executor.submit(blocks, args.blocks, output)
+    elif args.updated:
+        updated()
     else:
         print('USAGE: fbi -h')
```

### Comparing `fileblocks-2023.5.25/fileblocks.egg-info/PKG-INFO` & `fileblocks-2023.5.30/fileblocks.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileblocks
-Version: 2023.5.25
+Version: 2023.5.30
 Summary: Walk the line, Byte by Byte Analysis
 Home-page: https://github.com/jblukach/fbi
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -20,14 +20,15 @@
 options:
   -h, --help            show this help message and exit
   -b BLOCKS, --blocks BLOCKS
                         Input Filename
   -d, --download        Download Bloom Filter
   -o OUTPUT, --output OUTPUT
                         Output Directory
+  -u, --updated         Bloom Filter Last Updated
   -v, --version         show program's version number and exit
 ```
 
 ### CHALLENGES
 
 The first challenge is data encoding, as several applications only display ASCII characters with the potential for Unicode and UTF-8 to exist.
 
@@ -79,14 +80,26 @@
 
 https://b3.lukach.io/amzn/sector
 
 API keys are available using the self-registration process.
 
 https://store.lukach.io/l/b3
 
+### LAST UPDATED
+
+Check when the bloom filter was last updated using the command line interface (CLI).
+
+```
+fbi -u
+```
+
+Or by hitting the provided website for the last updated timestamp.
+
+https://static.fileblock.info/fbi.updated
+
 ### ANALYSIS
 
 The analyzed file allows both the absolute and relative location.
 
 ```
 fbi -b /usr/bin/df
 ```
```

### Comparing `fileblocks-2023.5.25/setup.py` & `fileblocks-2023.5.30/setup.py`

 * *Files identical despite different names*

