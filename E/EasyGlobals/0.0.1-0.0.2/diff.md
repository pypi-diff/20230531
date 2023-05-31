# Comparing `tmp/easyglobals-0.0.1.tar.gz` & `tmp/easyglobals-0.0.2.tar.gz`

## Comparing `easyglobals-0.0.1.tar` & `easyglobals-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 easyglobals-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 easyglobals-0.0.1/.idea/Easy_Globals.iml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 easyglobals-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 easyglobals-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 easyglobals-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 easyglobals-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 easyglobals-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 easyglobals-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 easyglobals-0.0.1/src/EasyGlobals/EasyGlobals.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyglobals-0.0.1/src/EasyGlobals/__init__.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 easyglobals-0.0.1/tests/example_complex.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 easyglobals-0.0.1/tests/example_minimal.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 easyglobals-0.0.1/tests/example_multiprocess_easyglobals.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 easyglobals-0.0.1/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 easyglobals-0.0.1/LICENSE
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 easyglobals-0.0.1/README.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 easyglobals-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 easyglobals-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 easyglobals-0.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 easyglobals-0.0.2/.idea/Easy_Globals.iml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 easyglobals-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 easyglobals-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 easyglobals-0.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 easyglobals-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 easyglobals-0.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 easyglobals-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 easyglobals-0.0.2/src/EasyGlobals/EasyGlobals.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 easyglobals-0.0.2/src/EasyGlobals/__init__.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 easyglobals-0.0.2/tests/example_complex.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 easyglobals-0.0.2/tests/example_minimal.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 easyglobals-0.0.2/tests/example_multiprocess_easyglobals.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 easyglobals-0.0.2/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 easyglobals-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 easyglobals-0.0.2/README.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 easyglobals-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 easyglobals-0.0.2/PKG-INFO
```

### Comparing `easyglobals-0.0.1/.idea/workspace.xml` & `easyglobals-0.0.2/.idea/workspace.xml`

 * *Files 3% similar despite different names*

#### Comparing `easyglobals-0.0.1/.idea/workspace.xml` & `easyglobals-0.0.2/.idea/workspace.xml`

```diff
@@ -1,18 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="f94c1167-ab5b-4afc-b6d8-c986fd0deda2" name="Changes" comment="">
-      <change afterPath="$PROJECT_DIR$/tests/example_complex.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/EasyGlobals/EasyGlobals.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/EasyGlobals/EasyGlobals.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/example_minimal.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/example_minimal.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/EasyGlobals/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/EasyGlobals/__init__.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -133,16 +131,32 @@
     <task id="LOCAL-00004" summary="Imports">
       <created>1685539692999</created>
       <option name="number" value="00004"/>
       <option name="presentableId" value="LOCAL-00004"/>
       <option name="project" value="LOCAL"/>
       <updated>1685539692999</updated>
     </task>
-    <option name="localTasksCounter" value="5"/>
+    <task id="LOCAL-00005" summary="for first upload">
+      <created>1685543504353</created>
+      <option name="number" value="00005"/>
+      <option name="presentableId" value="LOCAL-00005"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1685543504353</updated>
+    </task>
+    <task id="LOCAL-00006" summary="Version 0.0.1">
+      <created>1685543791085</created>
+      <option name="number" value="00006"/>
+      <option name="presentableId" value="LOCAL-00006"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1685543791085</updated>
+    </task>
+    <option name="localTasksCounter" value="7"/>
     <servers/>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="Added project files"/>
     <MESSAGE value="Imports"/>
-    <option name="LAST_COMMIT_MESSAGE" value="Imports"/>
+    <MESSAGE value="for first upload"/>
+    <MESSAGE value="Version 0.0.1"/>
+    <option name="LAST_COMMIT_MESSAGE" value="Version 0.0.1"/>
   </component>
 </project>
```

### Comparing `easyglobals-0.0.1/.idea/inspectionProfiles/Project_Default.xml` & `easyglobals-0.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.1/src/EasyGlobals/EasyGlobals.py` & `easyglobals-0.0.2/src/EasyGlobals/EasyGlobals.py`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.1/tests/example_complex.py` & `easyglobals-0.0.2/tests/example_complex.py`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.1/tests/example_multiprocess_easyglobals.py` & `easyglobals-0.0.2/tests/example_multiprocess_easyglobals.py`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.1/.gitignore` & `easyglobals-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.1/LICENSE` & `easyglobals-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.1/README.md` & `easyglobals-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Introduction
- EasyGlobals is An easy to use variable sharing object for Python that can quickly share complex objects between processes.
+ EasyGlobals is an easy to use variable sharing object for Python that can quickly share complex objects between processes.
 
 It uses Memcached in the background to share full objects and other complex variables between Python processes. Inspired by many closed source languages which have an easy way to share "global" variables between processes while retaining pythonic syntax.
 
 # Usage
 ```
 import EasyGlobals
 globals = EasyGlobals.Globals()
```

### Comparing `easyglobals-0.0.1/pyproject.toml` & `easyglobals-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "EasyGlobals"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
     "pymemcache"
 ]
 authors = [
   { name="Yacob", email="asnaeb2@gmail.com" },
 ]
 description = "An easy to use variable sharing library for Python that can quickly share complex objects between processes as if they had shared memory."
```

### Comparing `easyglobals-0.0.1/PKG-INFO` & `easyglobals-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: EasyGlobals
-Version: 0.0.1
+Version: 0.0.2
 Summary: An easy to use variable sharing library for Python that can quickly share complex objects between processes as if they had shared memory.
 Project-URL: Homepage, https://github.com/YacobBY/Easy_Globals
 Project-URL: Bug Tracker, https://github.com/YacobBY/Easy_Globals/issues
 Author-email: Yacob <asnaeb2@gmail.com>
 License-File: LICENSE
 Keywords: Globals,Python,Shared memory
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: pymemcache
 Description-Content-Type: text/markdown
 
 # Introduction
- EasyGlobals is An easy to use variable sharing object for Python that can quickly share complex objects between processes.
+ EasyGlobals is an easy to use variable sharing object for Python that can quickly share complex objects between processes.
 
 It uses Memcached in the background to share full objects and other complex variables between Python processes. Inspired by many closed source languages which have an easy way to share "global" variables between processes while retaining pythonic syntax.
 
 # Usage
 ```
 import EasyGlobals
 globals = EasyGlobals.Globals()
```

