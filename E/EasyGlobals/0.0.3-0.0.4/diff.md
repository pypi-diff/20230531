# Comparing `tmp/easyglobals-0.0.3.tar.gz` & `tmp/easyglobals-0.0.4.tar.gz`

## Comparing `easyglobals-0.0.3.tar` & `easyglobals-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 easyglobals-0.0.3/.idea/.gitignore
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 easyglobals-0.0.3/.idea/Easy_Globals.iml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 easyglobals-0.0.3/.idea/misc.xml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 easyglobals-0.0.3/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 easyglobals-0.0.3/.idea/vcs.xml
--rw-r--r--   0        0        0     8108 2020-02-02 00:00:00.000000 easyglobals-0.0.3/.idea/workspace.xml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 easyglobals-0.0.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 easyglobals-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 easyglobals-0.0.3/src/EasyGlobals/EasyGlobals.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 easyglobals-0.0.3/src/EasyGlobals/__init__.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 easyglobals-0.0.3/tests/example_complex.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 easyglobals-0.0.3/tests/example_minimal.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 easyglobals-0.0.3/tests/example_multiprocess_easyglobals.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 easyglobals-0.0.3/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 easyglobals-0.0.3/LICENSE
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 easyglobals-0.0.3/README.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 easyglobals-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 easyglobals-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 easyglobals-0.0.4/.idea/.gitignore
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 easyglobals-0.0.4/.idea/Easy_Globals.iml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 easyglobals-0.0.4/.idea/misc.xml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 easyglobals-0.0.4/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 easyglobals-0.0.4/.idea/vcs.xml
+-rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 easyglobals-0.0.4/.idea/workspace.xml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 easyglobals-0.0.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 easyglobals-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 easyglobals-0.0.4/src/EasyGlobals/EasyGlobals.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 easyglobals-0.0.4/src/EasyGlobals/__init__.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 easyglobals-0.0.4/tests/example_complex.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 easyglobals-0.0.4/tests/example_minimal.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 easyglobals-0.0.4/tests/example_multiprocess_easyglobals.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 easyglobals-0.0.4/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 easyglobals-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 easyglobals-0.0.4/README.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 easyglobals-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 easyglobals-0.0.4/PKG-INFO
```

### Comparing `easyglobals-0.0.3/.idea/workspace.xml` & `easyglobals-0.0.4/.idea/workspace.xml`

 * *Files 4% similar despite different names*

#### Comparing `easyglobals-0.0.3/.idea/workspace.xml` & `easyglobals-0.0.4/.idea/workspace.xml`

```diff
@@ -2,15 +2,15 @@
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="f94c1167-ab5b-4afc-b6d8-c986fd0deda2" name="Changes" comment="typo fix , some documentation and v0.0.3">
       <change afterPath="$PROJECT_DIR$/build_instructions.txt" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/.gitignore" beforeDir="false" afterPath="$PROJECT_DIR$/.gitignore" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -159,20 +159,35 @@
     <task id="LOCAL-00008" summary="typo fix , some documentation and v0.0.3">
       <created>1685544717130</created>
       <option name="number" value="00008"/>
       <option name="presentableId" value="LOCAL-00008"/>
       <option name="project" value="LOCAL"/>
       <updated>1685544717130</updated>
     </task>
-    <option name="localTasksCounter" value="9"/>
+    <task id="LOCAL-00009" summary="typo fix , some documentation and v0.0.3">
+      <created>1685544895248</created>
+      <option name="number" value="00009"/>
+      <option name="presentableId" value="LOCAL-00009"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1685544895248</updated>
+    </task>
+    <task id="LOCAL-00010" summary="readme update">
+      <created>1685545134632</created>
+      <option name="number" value="00010"/>
+      <option name="presentableId" value="LOCAL-00010"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1685545134632</updated>
+    </task>
+    <option name="localTasksCounter" value="11"/>
     <servers/>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="Added project files"/>
     <MESSAGE value="Imports"/>
     <MESSAGE value="for first upload"/>
     <MESSAGE value="Version 0.0.1"/>
     <MESSAGE value="Version 0.0.2 init fix"/>
     <MESSAGE value="typo fix , some documentation and v0.0.3"/>
-    <option name="LAST_COMMIT_MESSAGE" value="typo fix , some documentation and v0.0.3"/>
+    <MESSAGE value="readme update"/>
+    <option name="LAST_COMMIT_MESSAGE" value="readme update"/>
   </component>
 </project>
```

### Comparing `easyglobals-0.0.3/.idea/inspectionProfiles/Project_Default.xml` & `easyglobals-0.0.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.3/src/EasyGlobals/EasyGlobals.py` & `easyglobals-0.0.4/src/EasyGlobals/EasyGlobals.py`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.3/tests/example_complex.py` & `easyglobals-0.0.4/tests/example_complex.py`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.3/tests/example_multiprocess_easyglobals.py` & `easyglobals-0.0.4/tests/example_multiprocess_easyglobals.py`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.3/.gitignore` & `easyglobals-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.3/LICENSE` & `easyglobals-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `easyglobals-0.0.3/README.md` & `easyglobals-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 globals.test3 = {'dictkey1': globals.test1, 'dictkey2': globals.test2} #  Dict
 
 print(globals.test1)
 print(globals.test2)
 print(globals.test3)
 ```
 
+- Keep in mind that locks are not implemented here, meaning that race conditions can happen if two processes are writing to the same variable at the same time. For example when they're both incrementing the same value in a loop this can cause unwanted behavior.
+
+- To prevent this, an easy solution is to write to a variable in only one process. Reading can be done in as many processes as desired. Writing on multiple processes is not restricted but you will need to deal with the race conditions so prepare for coding headaches if you do.
 
 # Installation
 Install Memcached which acts as the server. installation with Apt is availible on Ubuntu. Different operating systems haven't been tested yet but installation guides with Windows can be found online
 ```
 sudo apt install memcached
 sudo systemctl start memcached
 ```
 
 Now you can install the easyglobals library:
 ```
 pip install easyglobals
 ```
 
-- Keep in mind that locks are not implemented here, meaning that race conditions can happen if two processes are writing to the same variable at the same time. For example when they're both incrementing the same value in a loop this can cause unwanted behavior.
-
-- To prevent this, an easy solution is to write to a variable in only one process. Reading can be done in as many processes as desired.
 
 # Limitations:
 - Any variable type that can be pickled should work. E.g. Numpy arrays, OpenCV images.
 - Directly getting and setting values from nested objects such as dicts or classes in the Globals can be problematic as the values are in binary format (pickled) while they are in memcached.
 - It's currently best to retrieve the an object from globals, modify it locally, and then store the entire object in globals again
 - If you're already using Memcached and your variable keys have the same name they will be overwritten
 - All variables will stay stored in Memcached even when your program stops. Restart memached to clear them, for example by running "service memcached restart" in the terminal.
```

### Comparing `easyglobals-0.0.3/pyproject.toml` & `easyglobals-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "EasyGlobals"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = [
     "pymemcache"
 ]
 authors = [
   { name="Yacob", email="asnaeb2@gmail.com" },
 ]
 description = "An easy to use variable sharing library for Python that can quickly share complex objects between processes as if they had shared memory."
```

### Comparing `easyglobals-0.0.3/PKG-INFO` & `easyglobals-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyGlobals
-Version: 0.0.3
+Version: 0.0.4
 Summary: An easy to use variable sharing library for Python that can quickly share complex objects between processes as if they had shared memory.
 Project-URL: Homepage, https://github.com/YacobBY/Easy_Globals
 Project-URL: Bug Tracker, https://github.com/YacobBY/Easy_Globals/issues
 Author-email: Yacob <asnaeb2@gmail.com>
 License-File: LICENSE
 Keywords: Globals,Python,Shared memory
 Classifier: License :: OSI Approved :: MIT License
@@ -29,30 +29,30 @@
 globals.test3 = {'dictkey1': globals.test1, 'dictkey2': globals.test2} #  Dict
 
 print(globals.test1)
 print(globals.test2)
 print(globals.test3)
 ```
 
+- Keep in mind that locks are not implemented here, meaning that race conditions can happen if two processes are writing to the same variable at the same time. For example when they're both incrementing the same value in a loop this can cause unwanted behavior.
+
+- To prevent this, an easy solution is to write to a variable in only one process. Reading can be done in as many processes as desired. Writing on multiple processes is not restricted but you will need to deal with the race conditions so prepare for coding headaches if you do.
 
 # Installation
 Install Memcached which acts as the server. installation with Apt is availible on Ubuntu. Different operating systems haven't been tested yet but installation guides with Windows can be found online
 ```
 sudo apt install memcached
 sudo systemctl start memcached
 ```
 
 Now you can install the easyglobals library:
 ```
 pip install easyglobals
 ```
 
-- Keep in mind that locks are not implemented here, meaning that race conditions can happen if two processes are writing to the same variable at the same time. For example when they're both incrementing the same value in a loop this can cause unwanted behavior.
-
-- To prevent this, an easy solution is to write to a variable in only one process. Reading can be done in as many processes as desired.
 
 # Limitations:
 - Any variable type that can be pickled should work. E.g. Numpy arrays, OpenCV images.
 - Directly getting and setting values from nested objects such as dicts or classes in the Globals can be problematic as the values are in binary format (pickled) while they are in memcached.
 - It's currently best to retrieve the an object from globals, modify it locally, and then store the entire object in globals again
 - If you're already using Memcached and your variable keys have the same name they will be overwritten
 - All variables will stay stored in Memcached even when your program stops. Restart memached to clear them, for example by running "service memcached restart" in the terminal.
```

