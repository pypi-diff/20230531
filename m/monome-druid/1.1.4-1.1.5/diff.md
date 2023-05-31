# Comparing `tmp/monome-druid-1.1.4.tar.gz` & `tmp/monome-druid-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monome-druid-1.1.4.tar", last modified: Wed Nov 16 23:11:26 2022, max compression
+gzip compressed data, was "monome-druid-1.1.5.tar", last modified: Wed May 31 15:28:29 2023, max compression
```

## Comparing `monome-druid-1.1.4.tar` & `monome-druid-1.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 tehn      (1000) tehn      (1000)        0 2022-11-16 23:11:26.093773 monome-druid-1.1.4/
--rw-rw-r--   0 tehn      (1000) tehn      (1000)       23 2022-11-16 23:05:18.000000 monome-druid-1.1.4/.git_archival.txt
--rw-rw-r--   0 tehn      (1000) tehn      (1000)       32 2022-11-16 23:05:18.000000 monome-druid-1.1.4/.gitattributes
--rw-rw-r--   0 tehn      (1000) tehn      (1000)      506 2022-11-16 23:05:18.000000 monome-druid-1.1.4/.gitignore
--rw-rw-r--   0 tehn      (1000) tehn      (1000)    35149 2022-11-16 23:05:18.000000 monome-druid-1.1.4/LICENSE
--rw-rw-r--   0 tehn      (1000) tehn      (1000)     2151 2022-11-16 23:11:26.093773 monome-druid-1.1.4/PKG-INFO
--rw-rw-r--   0 tehn      (1000) tehn      (1000)     1188 2022-11-16 23:05:18.000000 monome-druid-1.1.4/README-development.md
--rw-rw-r--   0 tehn      (1000) tehn      (1000)     1686 2022-11-16 23:05:18.000000 monome-druid-1.1.4/README.md
--rw-rw-r--   0 tehn      (1000) tehn      (1000)       38 2022-11-16 23:11:26.093773 monome-druid-1.1.4/setup.cfg
--rw-rw-r--   0 tehn      (1000) tehn      (1000)     1351 2022-11-16 23:05:18.000000 monome-druid-1.1.4/setup.py
-drwxrwxr-x   0 tehn      (1000) tehn      (1000)        0 2022-11-16 23:11:26.089774 monome-druid-1.1.4/src/
-drwxrwxr-x   0 tehn      (1000) tehn      (1000)        0 2022-11-16 23:11:26.093773 monome-druid-1.1.4/src/druid/
--rw-rw-r--   0 tehn      (1000) tehn      (1000)      225 2022-11-16 23:05:18.000000 monome-druid-1.1.4/src/druid/__init__.py
--rw-rw-r--   0 tehn      (1000) tehn      (1000)     3867 2022-11-16 23:05:18.000000 monome-druid-1.1.4/src/druid/cli.py
--rw-rw-r--   0 tehn      (1000) tehn      (1000)     4444 2022-11-16 23:05:18.000000 monome-druid-1.1.4/src/druid/crow.py
--rw-rw-r--   0 tehn      (1000) tehn      (1000)      136 2022-11-16 23:05:18.000000 monome-druid-1.1.4/src/druid/exceptions.py
--rw-rw-r--   0 tehn      (1000) tehn      (1000)    18798 2022-11-16 23:05:18.000000 monome-druid-1.1.4/src/druid/pydfu.py
--rw-rw-r--   0 tehn      (1000) tehn      (1000)    13291 2022-11-16 23:05:18.000000 monome-druid-1.1.4/src/druid/repl.py
--rw-rw-r--   0 tehn      (1000) tehn      (1000)     1232 2022-11-16 23:05:18.000000 monome-druid-1.1.4/src/druid/server.py
-drwxrwxr-x   0 tehn      (1000) tehn      (1000)        0 2022-11-16 23:11:26.093773 monome-druid-1.1.4/src/monome_druid.egg-info/
--rw-rw-r--   0 tehn      (1000) tehn      (1000)     2151 2022-11-16 23:11:26.000000 monome-druid-1.1.4/src/monome_druid.egg-info/PKG-INFO
--rw-rw-r--   0 tehn      (1000) tehn      (1000)      483 2022-11-16 23:11:26.000000 monome-druid-1.1.4/src/monome_druid.egg-info/SOURCES.txt
--rw-rw-r--   0 tehn      (1000) tehn      (1000)        1 2022-11-16 23:11:26.000000 monome-druid-1.1.4/src/monome_druid.egg-info/dependency_links.txt
--rw-rw-r--   0 tehn      (1000) tehn      (1000)       40 2022-11-16 23:11:26.000000 monome-druid-1.1.4/src/monome_druid.egg-info/entry_points.txt
--rw-rw-r--   0 tehn      (1000) tehn      (1000)      162 2022-11-16 23:11:26.000000 monome-druid-1.1.4/src/monome_druid.egg-info/requires.txt
--rw-rw-r--   0 tehn      (1000) tehn      (1000)        6 2022-11-16 23:11:26.000000 monome-druid-1.1.4/src/monome_druid.egg-info/top_level.txt
--rw-rw-r--   0 tehn      (1000) tehn      (1000)      435 2022-11-16 23:05:18.000000 monome-druid-1.1.4/test_ws.py
+drwxrwxr-x   0 tehn      (1000) tehn      (1000)        0 2023-05-31 15:28:29.301946 monome-druid-1.1.5/
+-rwxr-xr-x   0 tehn      (1000) tehn      (1000)       23 2023-03-18 22:28:14.000000 monome-druid-1.1.5/.git_archival.txt
+-rwxr-xr-x   0 tehn      (1000) tehn      (1000)       32 2023-03-18 22:28:14.000000 monome-druid-1.1.5/.gitattributes
+-rwxr-xr-x   0 tehn      (1000) tehn      (1000)      506 2023-03-18 22:28:14.000000 monome-druid-1.1.5/.gitignore
+-rwxrwxr-x   0 tehn      (1000) tehn      (1000)    35149 2023-05-31 15:28:19.000000 monome-druid-1.1.5/LICENSE
+-rw-rw-r--   0 tehn      (1000) tehn      (1000)     2151 2023-05-31 15:28:29.301946 monome-druid-1.1.5/PKG-INFO
+-rwxrwxr-x   0 tehn      (1000) tehn      (1000)     1331 2023-05-31 15:28:19.000000 monome-druid-1.1.5/README-development.md
+-rwxrwxr-x   0 tehn      (1000) tehn      (1000)     1686 2023-05-31 15:28:19.000000 monome-druid-1.1.5/README.md
+-rw-rw-r--   0 tehn      (1000) tehn      (1000)       38 2023-05-31 15:28:29.301946 monome-druid-1.1.5/setup.cfg
+-rwxrwxr-x   0 tehn      (1000) tehn      (1000)     1351 2023-05-31 15:28:19.000000 monome-druid-1.1.5/setup.py
+drwxrwxr-x   0 tehn      (1000) tehn      (1000)        0 2023-05-31 15:28:29.297946 monome-druid-1.1.5/src/
+drwxrwxr-x   0 tehn      (1000) tehn      (1000)        0 2023-05-31 15:28:29.297946 monome-druid-1.1.5/src/druid/
+-rwxrwxr-x   0 tehn      (1000) tehn      (1000)      225 2023-05-31 15:28:19.000000 monome-druid-1.1.5/src/druid/__init__.py
+-rw-rw-r--   0 tehn      (1000) tehn      (1000)     3956 2023-05-31 15:28:19.000000 monome-druid-1.1.5/src/druid/cli.py
+-rwxrwxr-x   0 tehn      (1000) tehn      (1000)     4444 2023-05-31 15:28:19.000000 monome-druid-1.1.5/src/druid/crow.py
+-rwxrwxr-x   0 tehn      (1000) tehn      (1000)      136 2023-05-31 15:28:19.000000 monome-druid-1.1.5/src/druid/exceptions.py
+-rwxrwxr-x   0 tehn      (1000) tehn      (1000)    18798 2023-05-31 15:28:19.000000 monome-druid-1.1.5/src/druid/pydfu.py
+-rwxrwxr-x   0 tehn      (1000) tehn      (1000)    13291 2023-05-31 15:28:19.000000 monome-druid-1.1.5/src/druid/repl.py
+-rwxrwxr-x   0 tehn      (1000) tehn      (1000)     1232 2023-05-31 15:28:19.000000 monome-druid-1.1.5/src/druid/server.py
+drwxrwxr-x   0 tehn      (1000) tehn      (1000)        0 2023-05-31 15:28:29.301946 monome-druid-1.1.5/src/monome_druid.egg-info/
+-rw-rw-r--   0 tehn      (1000) tehn      (1000)     2151 2023-05-31 15:28:29.000000 monome-druid-1.1.5/src/monome_druid.egg-info/PKG-INFO
+-rw-rw-r--   0 tehn      (1000) tehn      (1000)      483 2023-05-31 15:28:29.000000 monome-druid-1.1.5/src/monome_druid.egg-info/SOURCES.txt
+-rw-rw-r--   0 tehn      (1000) tehn      (1000)        1 2023-05-31 15:28:29.000000 monome-druid-1.1.5/src/monome_druid.egg-info/dependency_links.txt
+-rw-rw-r--   0 tehn      (1000) tehn      (1000)       40 2023-05-31 15:28:29.000000 monome-druid-1.1.5/src/monome_druid.egg-info/entry_points.txt
+-rw-rw-r--   0 tehn      (1000) tehn      (1000)      162 2023-05-31 15:28:29.000000 monome-druid-1.1.5/src/monome_druid.egg-info/requires.txt
+-rw-rw-r--   0 tehn      (1000) tehn      (1000)        6 2023-05-31 15:28:29.000000 monome-druid-1.1.5/src/monome_druid.egg-info/top_level.txt
+-rwxrwxr-x   0 tehn      (1000) tehn      (1000)      435 2023-05-31 15:28:19.000000 monome-druid-1.1.5/test_ws.py
```

### Comparing `monome-druid-1.1.4/LICENSE` & `monome-druid-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `monome-druid-1.1.4/PKG-INFO` & `monome-druid-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monome-druid
-Version: 1.1.4
+Version: 1.1.5
 Summary: Terminal interface for crow
 Home-page: https://github.com/monome/druid
 Author: monome
 Author-email: bcrabtree@monome.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `monome-druid-1.1.4/README-development.md` & `monome-druid-1.1.5/README-development.md`

 * *Files 14% similar despite different names*

```diff
@@ -30,7 +30,16 @@
 
 If at a later point you want to start working on druid again it's enough to activate the virtual environment again using
 ```
 cd <directory where druid is checked out>
 source .venv/bin/activate
 druid
 ```
+
+## Package Update
+
+- pypi.org account, get token for __token__ entry
+
+```
+python setup.py sdist bdist_wheel
+python -m twine upload dist/*
+```
```

### Comparing `monome-druid-1.1.4/README.md` & `monome-druid-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `monome-druid-1.1.4/setup.py` & `monome-druid-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `monome-druid-1.1.4/src/druid/cli.py` & `monome-druid-1.1.5/src/druid/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,16 @@
       if local_version != "0":
         crow.write("crow.reset()")
         time.sleep(0.1)
         c = crow.read(1000000)
         crow.write("^^v")
         tmp = (crow.read(100)).split("'")
         local_version = tmp[1][1:]
+        # strip off git version info
+        local_version = local_version.split('-')[0]
 
       print(">> local version: ", local_version)
 
       if version.parse(local_version) >= version.parse(git_data[0]):
         print("Up to date.")
         exit()
```

### Comparing `monome-druid-1.1.4/src/druid/crow.py` & `monome-druid-1.1.5/src/druid/crow.py`

 * *Files identical despite different names*

### Comparing `monome-druid-1.1.4/src/druid/pydfu.py` & `monome-druid-1.1.5/src/druid/pydfu.py`

 * *Files identical despite different names*

### Comparing `monome-druid-1.1.4/src/druid/repl.py` & `monome-druid-1.1.5/src/druid/repl.py`

 * *Files identical despite different names*

### Comparing `monome-druid-1.1.4/src/druid/server.py` & `monome-druid-1.1.5/src/druid/server.py`

 * *Files identical despite different names*

### Comparing `monome-druid-1.1.4/src/monome_druid.egg-info/PKG-INFO` & `monome-druid-1.1.5/src/monome_druid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monome-druid
-Version: 1.1.4
+Version: 1.1.5
 Summary: Terminal interface for crow
 Home-page: https://github.com/monome/druid
 Author: monome
 Author-email: bcrabtree@monome.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

