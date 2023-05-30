# Comparing `tmp/hive-archeology-bot-0.1.5.tar.gz` & `tmp/hive-archeology-bot-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hive-archeology-bot-0.1.5.tar", last modified: Tue May 30 22:29:17 2023, max compression
+gzip compressed data, was "hive-archeology-bot-0.1.6.tar", last modified: Tue May 30 22:33:57 2023, max compression
```

## Comparing `hive-archeology-bot-0.1.5.tar` & `hive-archeology-bot-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-30 22:29:17.274253 hive-archeology-bot-0.1.5/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1499 2023-05-19 18:51:54.000000 hive-archeology-bot-0.1.5/LICENSE
--rw-rw-r--   0 rob       (1000) rob       (1000)      773 2023-05-30 22:29:17.274253 hive-archeology-bot-0.1.5/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     2104 2023-05-19 19:43:04.000000 hive-archeology-bot-0.1.5/README.md
--rwxr-xr-x   0 rob       (1000) rob       (1000)    20940 2023-05-30 22:17:32.000000 hive-archeology-bot-0.1.5/hive_archeology.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-30 22:29:17.274253 hive-archeology-bot-0.1.5/hive_archeology_bot.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)      773 2023-05-30 22:29:16.000000 hive-archeology-bot-0.1.5/hive_archeology_bot.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      347 2023-05-30 22:29:17.000000 hive-archeology-bot-0.1.5/hive_archeology_bot.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-30 22:29:16.000000 hive-archeology-bot-0.1.5/hive_archeology_bot.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       62 2023-05-30 22:29:16.000000 hive-archeology-bot-0.1.5/hive_archeology_bot.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-19 18:53:43.000000 hive-archeology-bot-0.1.5/hive_archeology_bot.egg-info/not-zip-safe
--rw-rw-r--   0 rob       (1000) rob       (1000)       19 2023-05-30 22:29:17.000000 hive-archeology-bot-0.1.5/hive_archeology_bot.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       16 2023-05-30 22:29:17.000000 hive-archeology-bot-0.1.5/hive_archeology_bot.egg-info/top_level.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-30 22:29:17.274253 hive-archeology-bot-0.1.5/setup.cfg
--rwxr-xr-x   0 rob       (1000) rob       (1000)     1137 2023-05-30 22:29:00.000000 hive-archeology-bot-0.1.5/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-30 22:33:57.147211 hive-archeology-bot-0.1.6/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1499 2023-05-19 18:51:54.000000 hive-archeology-bot-0.1.6/LICENSE
+-rw-rw-r--   0 rob       (1000) rob       (1000)      773 2023-05-30 22:33:57.147211 hive-archeology-bot-0.1.6/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2104 2023-05-19 19:43:04.000000 hive-archeology-bot-0.1.6/README.md
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    20940 2023-05-30 22:33:49.000000 hive-archeology-bot-0.1.6/hive_archeology.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-30 22:33:57.147211 hive-archeology-bot-0.1.6/hive_archeology_bot.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      773 2023-05-30 22:33:56.000000 hive-archeology-bot-0.1.6/hive_archeology_bot.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      347 2023-05-30 22:33:57.000000 hive-archeology-bot-0.1.6/hive_archeology_bot.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-30 22:33:56.000000 hive-archeology-bot-0.1.6/hive_archeology_bot.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       62 2023-05-30 22:33:56.000000 hive-archeology-bot-0.1.6/hive_archeology_bot.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-19 18:53:43.000000 hive-archeology-bot-0.1.6/hive_archeology_bot.egg-info/not-zip-safe
+-rw-rw-r--   0 rob       (1000) rob       (1000)       26 2023-05-30 22:33:56.000000 hive-archeology-bot-0.1.6/hive_archeology_bot.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       16 2023-05-30 22:33:57.000000 hive-archeology-bot-0.1.6/hive_archeology_bot.egg-info/top_level.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-30 22:33:57.147211 hive-archeology-bot-0.1.6/setup.cfg
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     1144 2023-05-30 22:33:37.000000 hive-archeology-bot-0.1.6/setup.py
```

### Comparing `hive-archeology-bot-0.1.5/LICENSE` & `hive-archeology-bot-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hive-archeology-bot-0.1.5/PKG-INFO` & `hive-archeology-bot-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive-archeology-bot
-Version: 0.1.5
+Version: 0.1.6
 Summary: Hive Archeology Bot
 Home-page: https://github.com/pibara/hive-archeology
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: hive web3 bot
 Platform: UNKNOWN
```

### Comparing `hive-archeology-bot-0.1.5/README.md` & `hive-archeology-bot-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `hive-archeology-bot-0.1.5/hive_archeology.py` & `hive-archeology-bot-0.1.6/hive_archeology.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import operator
 from datetime import datetime
 from dateutil.parser import parse, _parser  # pylint: disable=import-private-name
 from lighthive.client import Client
 from lighthive.datastructures import Operation
 from lighthive.exceptions import RPCNodeException
 
-VERSION = "0.1.5"
+VERSION = "0.1.6"
 AUTHORS = {}
 AUTHORS["hive-archology"] = ["pibara", "croupierbot"]
 AUTHORS["lighthive"] = ["emrebeyler", "emrebeyler"]
 
 def make_body(author, benef, curation_rewards):
     """Construct the proxy comment"""
     ben2prod = {}
```

### Comparing `hive-archeology-bot-0.1.5/hive_archeology_bot.egg-info/PKG-INFO` & `hive-archeology-bot-0.1.6/hive_archeology_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive-archeology-bot
-Version: 0.1.5
+Version: 0.1.6
 Summary: Hive Archeology Bot
 Home-page: https://github.com/pibara/hive-archeology
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: hive web3 bot
 Platform: UNKNOWN
```

### Comparing `hive-archeology-bot-0.1.5/setup.py` & `hive-archeology-bot-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,9 +26,9 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
-    install_requires=["lighthive", "dateutil"],
+    install_requires=["lighthive", "python-dateutil"],
 )
```

