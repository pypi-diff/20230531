# Comparing `tmp/merge-dictionaries-0.2.2.tar.gz` & `tmp/merge-dictionaries-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merge-dictionaries-0.2.2.tar", last modified: Tue Jan 17 05:06:33 2023, max compression
+gzip compressed data, was "merge-dictionaries-0.3.0.tar", last modified: Wed May 31 15:47:48 2023, max compression
```

## Comparing `merge-dictionaries-0.2.2.tar` & `merge-dictionaries-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 dereckson  (5001) dereckson  (5001)        0 2023-01-17 05:06:33.826086 merge-dictionaries-0.2.2/
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)     1302 2023-01-17 04:07:17.000000 merge-dictionaries-0.2.2/LICENSE
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)     3942 2023-01-17 05:06:33.826155 merge-dictionaries-0.2.2/PKG-INFO
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)     3243 2023-01-17 04:07:17.000000 merge-dictionaries-0.2.2/README.md
-drwxr-xr-x   0 dereckson  (5001) dereckson  (5001)        0 2023-01-17 05:06:33.823744 merge-dictionaries-0.2.2/bin/
--rwxr-xr-x   0 dereckson  (5001) dereckson  (5001)      525 2023-01-17 04:07:17.000000 merge-dictionaries-0.2.2/bin/merge-dictionaries
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)      390 2023-01-17 04:07:17.000000 merge-dictionaries-0.2.2/pyproject.toml
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)      889 2023-01-17 05:06:33.826573 merge-dictionaries-0.2.2/setup.cfg
-drwxr-xr-x   0 dereckson  (5001) dereckson  (5001)        0 2023-01-17 05:06:33.822738 merge-dictionaries-0.2.2/src/
-drwxr-xr-x   0 dereckson  (5001) dereckson  (5001)        0 2023-01-17 05:06:33.824394 merge-dictionaries-0.2.2/src/merge_dictionaries.egg-info/
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)     3942 2023-01-17 05:06:33.000000 merge-dictionaries-0.2.2/src/merge_dictionaries.egg-info/PKG-INFO
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)      762 2023-01-17 05:06:33.000000 merge-dictionaries-0.2.2/src/merge_dictionaries.egg-info/SOURCES.txt
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)        1 2023-01-17 05:06:33.000000 merge-dictionaries-0.2.2/src/merge_dictionaries.egg-info/dependency_links.txt
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)       17 2023-01-17 05:06:33.000000 merge-dictionaries-0.2.2/src/merge_dictionaries.egg-info/requires.txt
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)       18 2023-01-17 05:06:33.000000 merge-dictionaries-0.2.2/src/merge_dictionaries.egg-info/top_level.txt
-drwxr-xr-x   0 dereckson  (5001) dereckson  (5001)        0 2023-01-17 05:06:33.824522 merge-dictionaries-0.2.2/src/mergedictionaries/
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)        0 2023-01-17 04:07:17.000000 merge-dictionaries-0.2.2/src/mergedictionaries/__init__.py
-drwxr-xr-x   0 dereckson  (5001) dereckson  (5001)        0 2023-01-17 05:06:33.824782 merge-dictionaries-0.2.2/src/mergedictionaries/app/
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)       21 2023-01-17 04:07:17.000000 merge-dictionaries-0.2.2/src/mergedictionaries/app/__init__.py
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)     4323 2023-01-17 04:07:17.000000 merge-dictionaries-0.2.2/src/mergedictionaries/app/app.py
-drwxr-xr-x   0 dereckson  (5001) dereckson  (5001)        0 2023-01-17 05:06:33.825053 merge-dictionaries-0.2.2/src/mergedictionaries/output/
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)      439 2023-01-17 04:07:17.000000 merge-dictionaries-0.2.2/src/mergedictionaries/output/__init__.py
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)     1214 2023-01-17 04:07:17.000000 merge-dictionaries-0.2.2/src/mergedictionaries/output/jetbrains.py
-drwxr-xr-x   0 dereckson  (5001) dereckson  (5001)        0 2023-01-17 05:06:33.825585 merge-dictionaries-0.2.2/src/mergedictionaries/sources/
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)      393 2023-01-17 04:07:17.000000 merge-dictionaries-0.2.2/src/mergedictionaries/sources/__init__.py
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)     4172 2023-01-17 04:07:17.000000 merge-dictionaries-0.2.2/src/mergedictionaries/sources/git.py
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)     1429 2023-01-17 04:07:17.000000 merge-dictionaries-0.2.2/src/mergedictionaries/sources/hunspell.py
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)     1732 2023-01-17 04:51:02.000000 merge-dictionaries-0.2.2/src/mergedictionaries/sources/jetbrains.py
-drwxr-xr-x   0 dereckson  (5001) dereckson  (5001)        0 2023-01-17 05:06:33.825982 merge-dictionaries-0.2.2/src/mergedictionaries/write/
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)       42 2023-01-17 04:07:17.000000 merge-dictionaries-0.2.2/src/mergedictionaries/write/__init__.py
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)      989 2023-01-17 04:07:17.000000 merge-dictionaries-0.2.2/src/mergedictionaries/write/git.py
--rw-r--r--   0 dereckson  (5001) dereckson  (5001)      790 2023-01-17 04:07:17.000000 merge-dictionaries-0.2.2/src/mergedictionaries/write/jetbrains.py
+drwxr-xr-x   0 ssantoro   (501) staff       (20)        0 2023-05-31 15:47:48.708564 merge-dictionaries-0.3.0/
+-rw-r--r--   0 ssantoro   (501) staff       (20)     1302 2023-05-31 14:44:49.000000 merge-dictionaries-0.3.0/LICENSE
+-rw-r--r--   0 ssantoro   (501) staff       (20)     3942 2023-05-31 15:47:48.708698 merge-dictionaries-0.3.0/PKG-INFO
+-rw-r--r--   0 ssantoro   (501) staff       (20)     3243 2023-05-31 14:44:49.000000 merge-dictionaries-0.3.0/README.md
+drwxr-xr-x   0 ssantoro   (501) staff       (20)        0 2023-05-31 15:47:48.702624 merge-dictionaries-0.3.0/bin/
+-rwxr-xr-x   0 ssantoro   (501) staff       (20)      525 2023-05-31 14:44:49.000000 merge-dictionaries-0.3.0/bin/merge-dictionaries
+-rw-r--r--   0 ssantoro   (501) staff       (20)      390 2023-05-31 14:44:49.000000 merge-dictionaries-0.3.0/pyproject.toml
+-rw-r--r--   0 ssantoro   (501) staff       (20)      889 2023-05-31 15:47:48.709428 merge-dictionaries-0.3.0/setup.cfg
+drwxr-xr-x   0 ssantoro   (501) staff       (20)        0 2023-05-31 15:47:48.700113 merge-dictionaries-0.3.0/src/
+drwxr-xr-x   0 ssantoro   (501) staff       (20)        0 2023-05-31 15:47:48.704354 merge-dictionaries-0.3.0/src/merge_dictionaries.egg-info/
+-rw-r--r--   0 ssantoro   (501) staff       (20)     3942 2023-05-31 15:47:48.000000 merge-dictionaries-0.3.0/src/merge_dictionaries.egg-info/PKG-INFO
+-rw-r--r--   0 ssantoro   (501) staff       (20)      762 2023-05-31 15:47:48.000000 merge-dictionaries-0.3.0/src/merge_dictionaries.egg-info/SOURCES.txt
+-rw-r--r--   0 ssantoro   (501) staff       (20)        1 2023-05-31 15:47:48.000000 merge-dictionaries-0.3.0/src/merge_dictionaries.egg-info/dependency_links.txt
+-rw-r--r--   0 ssantoro   (501) staff       (20)       17 2023-05-31 15:47:48.000000 merge-dictionaries-0.3.0/src/merge_dictionaries.egg-info/requires.txt
+-rw-r--r--   0 ssantoro   (501) staff       (20)       18 2023-05-31 15:47:48.000000 merge-dictionaries-0.3.0/src/merge_dictionaries.egg-info/top_level.txt
+drwxr-xr-x   0 ssantoro   (501) staff       (20)        0 2023-05-31 15:47:48.704742 merge-dictionaries-0.3.0/src/mergedictionaries/
+-rw-r--r--   0 ssantoro   (501) staff       (20)        0 2023-05-31 14:44:49.000000 merge-dictionaries-0.3.0/src/mergedictionaries/__init__.py
+drwxr-xr-x   0 ssantoro   (501) staff       (20)        0 2023-05-31 15:47:48.705338 merge-dictionaries-0.3.0/src/mergedictionaries/app/
+-rw-r--r--   0 ssantoro   (501) staff       (20)       21 2023-05-31 14:44:49.000000 merge-dictionaries-0.3.0/src/mergedictionaries/app/__init__.py
+-rw-r--r--   0 ssantoro   (501) staff       (20)     4323 2023-05-31 14:44:49.000000 merge-dictionaries-0.3.0/src/mergedictionaries/app/app.py
+drwxr-xr-x   0 ssantoro   (501) staff       (20)        0 2023-05-31 15:47:48.705978 merge-dictionaries-0.3.0/src/mergedictionaries/output/
+-rw-r--r--   0 ssantoro   (501) staff       (20)      439 2023-05-31 14:44:49.000000 merge-dictionaries-0.3.0/src/mergedictionaries/output/__init__.py
+-rw-r--r--   0 ssantoro   (501) staff       (20)     1214 2023-05-31 14:44:49.000000 merge-dictionaries-0.3.0/src/mergedictionaries/output/jetbrains.py
+drwxr-xr-x   0 ssantoro   (501) staff       (20)        0 2023-05-31 15:47:48.707300 merge-dictionaries-0.3.0/src/mergedictionaries/sources/
+-rw-r--r--   0 ssantoro   (501) staff       (20)      393 2023-05-31 14:44:49.000000 merge-dictionaries-0.3.0/src/mergedictionaries/sources/__init__.py
+-rw-r--r--   0 ssantoro   (501) staff       (20)     4534 2023-05-31 15:33:07.000000 merge-dictionaries-0.3.0/src/mergedictionaries/sources/git.py
+-rw-r--r--   0 ssantoro   (501) staff       (20)     1429 2023-05-31 14:44:49.000000 merge-dictionaries-0.3.0/src/mergedictionaries/sources/hunspell.py
+-rw-r--r--   0 ssantoro   (501) staff       (20)     1978 2023-05-31 15:18:10.000000 merge-dictionaries-0.3.0/src/mergedictionaries/sources/jetbrains.py
+drwxr-xr-x   0 ssantoro   (501) staff       (20)        0 2023-05-31 15:47:48.708290 merge-dictionaries-0.3.0/src/mergedictionaries/write/
+-rw-r--r--   0 ssantoro   (501) staff       (20)       42 2023-05-31 14:44:49.000000 merge-dictionaries-0.3.0/src/mergedictionaries/write/__init__.py
+-rw-r--r--   0 ssantoro   (501) staff       (20)      989 2023-05-31 14:44:49.000000 merge-dictionaries-0.3.0/src/mergedictionaries/write/git.py
+-rw-r--r--   0 ssantoro   (501) staff       (20)      790 2023-05-31 14:44:49.000000 merge-dictionaries-0.3.0/src/mergedictionaries/write/jetbrains.py
```

### Comparing `merge-dictionaries-0.2.2/LICENSE` & `merge-dictionaries-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merge-dictionaries-0.2.2/PKG-INFO` & `merge-dictionaries-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: merge-dictionaries
-Version: 0.2.2
+Version: 0.3.0
 Summary: Merge dictionaries
 Home-page: https://devcentral.nasqueron.org/source/merge-dictionaries/
 Author: Sébastien Santoro
 Author-email: dereckson@espace-win.org
 License: BSD-2-Clause
 Project-URL: Bug Tracker, https://devcentral.nasqueron.org/tag/development_tools/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Merge dictionaries
 
 ## Root problem
```

### Comparing `merge-dictionaries-0.2.2/README.md` & `merge-dictionaries-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `merge-dictionaries-0.2.2/bin/merge-dictionaries` & `merge-dictionaries-0.3.0/bin/merge-dictionaries`

 * *Files identical despite different names*

### Comparing `merge-dictionaries-0.2.2/setup.cfg` & `merge-dictionaries-0.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = merge-dictionaries
-version = 0.2.2
+version = 0.3.0
 author = Sébastien Santoro
 author_email = dereckson@espace-win.org
 description = Merge dictionaries
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = BSD-2-Clause
 license_files = LICENSE
@@ -21,15 +21,15 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 scripts = 
 	bin/merge-dictionaries
-python_requires = >=3.6
+python_requires = >=3.7
 install_requires = 
 	PyYAML>=6.0,<7.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
```

### Comparing `merge-dictionaries-0.2.2/src/merge_dictionaries.egg-info/PKG-INFO` & `merge-dictionaries-0.3.0/src/merge_dictionaries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: merge-dictionaries
-Version: 0.2.2
+Version: 0.3.0
 Summary: Merge dictionaries
 Home-page: https://devcentral.nasqueron.org/source/merge-dictionaries/
 Author: Sébastien Santoro
 Author-email: dereckson@espace-win.org
 License: BSD-2-Clause
 Project-URL: Bug Tracker, https://devcentral.nasqueron.org/tag/development_tools/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Merge dictionaries
 
 ## Root problem
```

### Comparing `merge-dictionaries-0.2.2/src/merge_dictionaries.egg-info/SOURCES.txt` & `merge-dictionaries-0.3.0/src/merge_dictionaries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `merge-dictionaries-0.2.2/src/mergedictionaries/app/app.py` & `merge-dictionaries-0.3.0/src/mergedictionaries/app/app.py`

 * *Files identical despite different names*

### Comparing `merge-dictionaries-0.2.2/src/mergedictionaries/output/jetbrains.py` & `merge-dictionaries-0.3.0/src/mergedictionaries/output/jetbrains.py`

 * *Files identical despite different names*

### Comparing `merge-dictionaries-0.2.2/src/mergedictionaries/sources/git.py` & `merge-dictionaries-0.3.0/src/mergedictionaries/sources/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 #   -------------------------------------------------------------
 #   Manipulate a dictionary sync repository
 #   - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
 
 class GitRepository:
-
     DICTIONARY_PATH = "dictionary.txt"
 
     def __init__(self, repository_remote, cached_repositories):
         self.remote = repository_remote
         self.cache = cached_repositories
         self.path = None
 
@@ -77,16 +76,29 @@
 
             if process.returncode > 0:
                 return True
 
         return False
 
     @staticmethod
+    def get_hostname():
+        env_hostname_keys = [
+            "HOST",
+            "HOSTNAME",
+        ]
+        for key in env_hostname_keys:
+            if key in os.environ:
+                return os.environ[key]
+
+        return subprocess.run(["hostname"], capture_output=True).stdout.decode().strip()
+
+    @staticmethod
     def get_commit_message():
-        return f"Sync personal dictionary\n\nSync application: merge-dictionaries\nSync hostname: {os.environ['HOSTNAME']}"
+        hostname = GitRepository.get_hostname()
+        return f"Sync personal dictionary\n\nSync application: merge-dictionaries\nSync hostname: {hostname}"
 
     def run(self, commands):
         for command in commands:
             subprocess.run(
                 command,
                 cwd=self.path,
             )
@@ -138,10 +150,11 @@
 
 
 #   -------------------------------------------------------------
 #   Events
 #     :: on_exit
 #   - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
+
 def on_exit(cached_repos):
     for _, repository_path in cached_repos.items():
         shutil.rmtree(repository_path)
```

### Comparing `merge-dictionaries-0.2.2/src/mergedictionaries/sources/hunspell.py` & `merge-dictionaries-0.3.0/src/mergedictionaries/sources/hunspell.py`

 * *Files identical despite different names*

### Comparing `merge-dictionaries-0.2.2/src/mergedictionaries/sources/jetbrains.py` & `merge-dictionaries-0.3.0/src/mergedictionaries/sources/jetbrains.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,27 @@
 from xml.etree import ElementTree
 
 
 DICTIONARY_FILENAMES = ["cachedDictionary.xml", "spellchecker-dictionary.xml"]
 
 
 def get_configuration_path():
-    """Find JetBrains configuration folder for Windows and UNIX systems."""
+    """Find JetBrains configuration folder for Windows, macOS and other UNIX systems."""
     try:
         return os.environ["APPDATA"] + "/JetBrains"
     except KeyError:
-        return os.environ["HOME"] + "/.config/JetBrains"
+        candidates = [
+            os.environ["HOME"] + "/Library/Application Support/JetBrains",
+            os.environ["HOME"] + "/.config/JetBrains",
+        ]
+        for candidate in candidates:
+            if os.path.exists(candidate):
+                break
+
+        return candidate
 
 
 def find_application_level_dictionaries():
     # We're looking for paths like:
     # ~/.config/JetBrains/PyCharm2021.3/options/cachedDictionary.xml
     base_path = get_configuration_path()
```

### Comparing `merge-dictionaries-0.2.2/src/mergedictionaries/write/git.py` & `merge-dictionaries-0.3.0/src/mergedictionaries/write/git.py`

 * *Files identical despite different names*

### Comparing `merge-dictionaries-0.2.2/src/mergedictionaries/write/jetbrains.py` & `merge-dictionaries-0.3.0/src/mergedictionaries/write/jetbrains.py`

 * *Files identical despite different names*

