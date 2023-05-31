# Comparing `tmp/iris_pex_embedded_python-2.2.0.tar.gz` & `tmp/iris_pex_embedded_python-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iris_pex_embedded_python-2.2.0.tar", last modified: Fri May 19 16:26:41 2023, max compression
+gzip compressed data, was "iris_pex_embedded_python-2.3.0.tar", last modified: Wed May 31 14:34:51 2023, max compression
```

## Comparing `iris_pex_embedded_python-2.2.0.tar` & `iris_pex_embedded_python-2.3.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-05-19 16:26:41.421655 iris_pex_embedded_python-2.2.0/
--rw-r--r--   0 grongier (902446405) 1252422112     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.2.0/LICENSE
--rw-r--r--   0 grongier (902446405) 1252422112    39287 2023-05-19 16:26:41.420477 iris_pex_embedded_python-2.2.0/PKG-INFO
--rw-r--r--   0 grongier (902446405) 1252422112    38378 2023-05-19 16:25:15.000000 iris_pex_embedded_python-2.2.0/README.md
--rw-r--r--   0 grongier (902446405) 1252422112        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.2.0/pyproject.toml
--rw-r--r--   0 grongier (902446405) 1252422112       38 2023-05-19 16:26:41.421955 iris_pex_embedded_python-2.2.0/setup.cfg
--rw-r--r--   0 grongier (902446405) 1252422112     2074 2023-05-19 16:25:42.000000 iris_pex_embedded_python-2.2.0/setup.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-05-19 16:26:41.385916 iris_pex_embedded_python-2.2.0/src/
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-05-19 16:26:41.385399 iris_pex_embedded_python-2.2.0/src/grongier/
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-05-19 16:26:41.392015 iris_pex_embedded_python-2.2.0/src/grongier/iris/
--rw-r--r--   0 grongier (902446405) 1252422112        0 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/iris/__init__.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-05-19 16:26:41.410348 iris_pex_embedded_python-2.2.0/src/grongier/pex/
--rw-r--r--   0 grongier (902446405) 1252422112     1166 2023-04-18 10:17:07.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/__init__.py
--rw-r--r--   0 grongier (902446405) 1252422112    20152 2023-04-21 15:01:34.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_business_host.py
--rw-r--r--   0 grongier (902446405) 1252422112     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_business_operation.py
--rw-r--r--   0 grongier (902446405) 1252422112    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_business_process.py
--rw-r--r--   0 grongier (902446405) 1252422112     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_business_service.py
--rw-r--r--   0 grongier (902446405) 1252422112    15107 2023-04-21 08:43:30.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_common.py
--rw-r--r--   0 grongier (902446405) 1252422112     5354 2023-05-19 16:15:48.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_director.py
--rw-r--r--   0 grongier (902446405) 1252422112     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_inbound_adapter.py
--rw-r--r--   0 grongier (902446405) 1252422112      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_message.py
--rw-r--r--   0 grongier (902446405) 1252422112      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_outbound_adapter.py
--rw-r--r--   0 grongier (902446405) 1252422112      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_pickle_message.py
--rw-r--r--   0 grongier (902446405) 1252422112     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_private_session_duplex.py
--rw-r--r--   0 grongier (902446405) 1252422112     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_private_session_process.py
--rw-r--r--   0 grongier (902446405) 1252422112    10275 2023-05-17 11:46:10.000000 iris_pex_embedded_python-2.2.0/src/grongier/pex/_utils.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-05-19 16:26:41.418438 iris_pex_embedded_python-2.2.0/src/iris_pex_embedded_python.egg-info/
--rw-r--r--   0 grongier (902446405) 1252422112    39287 2023-05-19 16:26:41.000000 iris_pex_embedded_python-2.2.0/src/iris_pex_embedded_python.egg-info/PKG-INFO
--rw-r--r--   0 grongier (902446405) 1252422112      824 2023-05-19 16:26:41.000000 iris_pex_embedded_python-2.2.0/src/iris_pex_embedded_python.egg-info/SOURCES.txt
--rw-r--r--   0 grongier (902446405) 1252422112        1 2023-05-19 16:26:41.000000 iris_pex_embedded_python-2.2.0/src/iris_pex_embedded_python.egg-info/dependency_links.txt
--rw-r--r--   0 grongier (902446405) 1252422112       43 2023-05-19 16:26:41.000000 iris_pex_embedded_python-2.2.0/src/iris_pex_embedded_python.egg-info/requires.txt
--rw-r--r--   0 grongier (902446405) 1252422112        9 2023-05-19 16:26:41.000000 iris_pex_embedded_python-2.2.0/src/iris_pex_embedded_python.egg-info/top_level.txt
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 14:34:51.772402 iris_pex_embedded_python-2.3.0/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.3.0/LICENSE
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    50008 2023-05-31 14:34:51.771507 iris_pex_embedded_python-2.3.0/PKG-INFO
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    49099 2023-05-31 14:32:55.000000 iris_pex_embedded_python-2.3.0/README.md
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.3.0/pyproject.toml
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       38 2023-05-31 14:34:51.772743 iris_pex_embedded_python-2.3.0/setup.cfg
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     2074 2023-05-31 14:34:08.000000 iris_pex_embedded_python-2.3.0/setup.py
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 14:34:51.709708 iris_pex_embedded_python-2.3.0/src/
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 14:34:51.708904 iris_pex_embedded_python-2.3.0/src/grongier/
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 14:34:51.718681 iris_pex_embedded_python-2.3.0/src/grongier/iris/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/iris/__init__.py
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 14:34:51.758587 iris_pex_embedded_python-2.3.0/src/grongier/pex/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1166 2023-05-29 19:57:15.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/__init__.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      107 2023-05-31 08:54:05.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/__main__.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    20152 2023-04-21 15:01:34.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_business_host.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_business_operation.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_business_process.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_business_service.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     5491 2023-05-31 11:56:27.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_cli.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    15107 2023-04-21 08:43:30.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_common.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     6762 2023-05-31 12:39:39.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_director.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_inbound_adapter.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_message.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_outbound_adapter.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_pickle_message.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_private_session_duplex.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_private_session_process.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    15120 2023-05-31 13:10:44.000000 iris_pex_embedded_python-2.3.0/src/grongier/pex/_utils.py
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 14:34:51.769143 iris_pex_embedded_python-2.3.0/src/iris_pex_embedded_python.egg-info/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    50008 2023-05-31 14:34:51.000000 iris_pex_embedded_python-2.3.0/src/iris_pex_embedded_python.egg-info/PKG-INFO
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      878 2023-05-31 14:34:51.000000 iris_pex_embedded_python-2.3.0/src/iris_pex_embedded_python.egg-info/SOURCES.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        1 2023-05-31 14:34:51.000000 iris_pex_embedded_python-2.3.0/src/iris_pex_embedded_python.egg-info/dependency_links.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       43 2023-05-31 14:34:51.000000 iris_pex_embedded_python-2.3.0/src/iris_pex_embedded_python.egg-info/requires.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        9 2023-05-31 14:34:51.000000 iris_pex_embedded_python-2.3.0/src/iris_pex_embedded_python.egg-info/top_level.txt
```

### Comparing `iris_pex_embedded_python-2.2.0/LICENSE` & `iris_pex_embedded_python-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.2.0/PKG-INFO` & `iris_pex_embedded_python-2.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris_pex_embedded_python
-Version: 2.2.0
+Version: 2.3.0
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
@@ -65,17 +65,32 @@
   - [7.10. The `objects`](#710-the-objects)
   - [7.11. The `messages`](#711-the-messages)
   - [7.12. How to regsiter a component](#712-how-to-regsiter-a-component)
     - [7.12.1. register\_component](#7121-register_component)
     - [7.12.2. register\_file](#7122-register_file)
     - [7.12.3. register\_folder](#7123-register_folder)
     - [7.12.4. migrate](#7124-migrate)
-      - [7.12.4.1 setting.py file](#71241-settingpy-file)
+      - [7.12.4.1. setting.py file](#71241-settingpy-file)
+        - [7.12.4.1.1. CLASSES section](#712411-classes-section)
+        - [7.12.4.1.2. Productions section](#712412-productions-section)
   - [7.13. Direct use of Grongier.PEX](#713-direct-use-of-grongierpex)
-- [8. Credits](#8-credits)
+- [8. Command line](#8-command-line)
+  - [8.1. help](#81-help)
+  - [8.2. default](#82-default)
+  - [8.3. lists](#83-lists)
+  - [8.4. start](#84-start)
+  - [8.5. kill](#85-kill)
+  - [8.6. stop](#86-stop)
+  - [8.7. restart](#87-restart)
+  - [8.8. migrate](#88-migrate)
+  - [8.9. export](#89-export)
+  - [8.10. status](#810-status)
+  - [8.11. version](#811-version)
+  - [8.12. log](#812-log)
+- [9. Credits](#9-credits)
 
 ## 1.2. Example
 
 ```python
 from grongier.pex import BusinessOperation,Message
 
 class MyBusinessOperation(BusinessOperation):
@@ -727,33 +742,31 @@
 This class defines:
 
 `create_business_service`: The create_business_service() method initiates the specified business service.<br>
 **Parameters**:
 - **connection**: an IRISConnection object that specifies the connection to an IRIS instance for Java.
 - **target**: a string that specifies the name of the business service in the production definition.
 
+**Returns**:
+an object that contains an instance of IRISBusinessService
+
 `start_production`: The start_production() method starts the production.<br>
 **Parameters**:
 - **production_name**: a string that specifies the name of the production to start.
 
 `stop_production`: The stop_production() method stops the production.<br>
 **Parameters**:
 - **production_name**: a string that specifies the name of the production to stop.
 
 `restart_production`: The restart_production() method restarts the production.<br>
 **Parameters**:
 - **production_name**: a string that specifies the name of the production to restart.
 
 `list_productions`: The list_productions() method returns a dictionary of the names of the productions that are currently running.<br>
 
-**Returns**:
-an object that contains an instance of IRISBusinessService
-
-WIP example
-
 ## 7.10. The `objects`
 We will use `dataclass` to hold information in our [messages](#711-the-messages) in a `obj.py` file.
 
 Example of an object ( situated in the src/python/demo/reddit/obj.py file ):
 ```python
 from dataclasses import dataclass
 
@@ -871,15 +884,15 @@
 Then use this static method to migrate the settings file to the iris framework.
 
 ```python
 from grongier.pex import Utils
 Utils.migrate()
 ```
 
-#### 7.12.4.1 setting.py file
+#### 7.12.4.1. setting.py file
 
 This file is used to store the settings of the interoperability components.
 
 It has two sections :
 * `CLASSES` : This section is used to store the classes of the interoperability components.
 * `PRODUCTIONS` : This section is used to store the productions of the interoperability components.
 
@@ -952,26 +965,433 @@
             }
         ]
     }
     }
 ]
 ```
 
+##### 7.12.4.1.1. CLASSES section
+
+This section is used to store the classes of the interoperability components.
+
+It aims to help to register the components.
+
+This dictionary has the following structure :
+* Key : The name of the component
+* Value : 
+  * The class of the component (you have to import it before)
+  * The module of the component (you have to import it before)
+  * Another dictionary with the following structure :
+    * `module` : Name of the module of the component (optional)
+    * `class` : Name of the class of the component (optional)
+    * `path` : The path of the component (mandatory)
+
+e.g :
+
+When Value is a class or a module:
+```python
+import bo
+import bp
+from bs import RedditService
+
+CLASSES = {
+    'Python.RedditService': RedditService,
+    'Python.FilterPostRoutingRule': bp.FilterPostRoutingRule,
+    'Python.FileOperation': bo,
+}
+```
+
+When Value is a dictionary :
+```python
+CLASSES = {
+    'Python.RedditService': {
+        'module': 'bs',
+        'class': 'RedditService',
+        'path': '/irisdev/app/src/python/demo/'
+    },
+    'Python.Module': {
+        'module': 'bp',
+        'path': '/irisdev/app/src/python/demo/'
+    },
+    'Python.Package': {
+        'path': '/irisdev/app/src/python/demo/'
+    },
+}
+```
+
+##### 7.12.4.1.2. Productions section
+
+This section is used to store the productions of the interoperability components.
+
+It aims to help to register a production.
+
+This list has the following structure :
+* A list of dictionary with the following structure :
+  * `dc.Python.Production` : The name of the production
+    * `@Name` : The name of the production
+    * `@TestingEnabled` : The testing enabled of the production
+    * `@LogGeneralTraceEvents` : The log general trace events of the production
+    * `Description` : The description of the production
+    * `ActorPoolSize` : The actor pool size of the production
+    * `Item` : The list of the items of the production
+      * `@Name` : The name of the item
+      * `@Category` : The category of the item
+      * `@ClassName` : The class name of the item
+      * `@PoolSize` : The pool size of the item
+      * `@Enabled` : The enabled of the item
+      * `@Foreground` : The foreground of the item
+      * `@Comment` : The comment of the item
+      * `@LogTraceEvents` : The log trace events of the item
+      * `@Schedule` : The schedule of the item
+      * `Setting` : The list of the settings of the item
+        * `@Target` : The target of the setting
+        * `@Name` : The name of the setting
+        * `#text` : The value of the setting
+
+The minimum structure of a production is :
+```python
+PRODUCTIONS = [
+        {
+            'UnitTest.Production': {
+                "Item": [
+                    {
+                        "@Name": "Python.FileOperation",
+                        "@ClassName": "Python.FileOperation",
+                    },
+                    {
+                        "@Name": "Python.EmailOperation",
+                        "@ClassName": "UnitTest.Package.EmailOperation"
+                    }
+                ]
+            }
+        } 
+    ]
+```
+
+You can also set in `@ClassName` an item from the CLASSES section.
+
+e.g :
+```python
+from bo import FileOperation
+PRODUCTIONS = [
+        {
+            'UnitTest.Production': {
+                "Item": [
+                    {
+                        "@Name": "Python.FileOperation",
+                        "@ClassName": FileOperation,
+                    }
+                ]
+            }
+        } 
+    ]
+```
+
+As the production is a dictionary, you can add in value of the production dictionary an environment variable.
+
+e.g :
+```python
+import os
+
+PRODUCTIONS = [
+        {
+            'UnitTest.Production': {
+                "Item": [
+                    {
+                        "@Name": "Python.FileOperation",
+                        "@ClassName": "Python.FileOperation",
+                        "Setting": {
+                            "@Target": "Host",
+                            "@Name": "%settings",
+                            "#text": os.environ['SETTINGS']
+                        }
+                    }
+                ]
+            }
+        } 
+    ]
+```
+
 ## 7.13. Direct use of Grongier.PEX
 
 If you don't want to use the register_component util. You can add a Grongier.PEX.BusinessService component directly into the management portal and configure the properties :
 - %module :
   - Module name of your python code
 - %classname :
   - Classname of you component
 - %classpaths
   - Path where you component is.
     - This can one or more Classpaths (separated by '|' character) needed in addition to PYTHON_PATH
 
 e.g :
 <img width="800" alt="component-config" src="https://user-images.githubusercontent.com/47849411/131316308-e1898b19-11df-433b-b1c6-7f69d5cc9974.png">
 
-# 8. Credits
+# 8. Command line
+
+Since version 2.3.0, you can use the command line to register your components and productions.
+
+To use it, you have to use the following command :
+```bash
+/usr/irissys/bin/irispython -m grongier.pex 
+```
+
+output :
+```bash
+usage: python3 -m grongier.pex [-h] [-d DEFAULT] [-l] [-s START] [-k] [-S] [-r] [-M MIGRATE] [-e EXPORT] [-x] [-v] [-L]
+optional arguments:
+  -h, --help            display help and default production name
+  -d DEFAULT, --default DEFAULT
+                        set the default production
+  -l, --lists           list productions
+  -s START, --start START
+                        start a production
+  -k, --kill            kill a production (force stop)
+  -S, --stop            stop a production
+  -r, --restart         restart a production
+  -M MIGRATE, --migrate MIGRATE
+                        migrate production and classes with settings file
+  -e EXPORT, --export EXPORT
+                        export a production
+  -x, --status          status a production
+  -v, --version         display version
+  -L, --log             display log
+
+default production: PEX.Production
+```
+
+## 8.1. help
+
+The help command display the help and the default production name.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -h
+```
+
+output :
+```bash
+usage: python3 -m grongier.pex [-h] [-d DEFAULT] [-l] [-s START] [-k] [-S] [-r] [-M MIGRATE] [-e EXPORT] [-x] [-v] [-L]
+...
+default production: PEX.Production
+```
+
+## 8.2. default
+
+The default command set the default production.
+
+With no argument, it display the default production.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -d
+```
+
+output :
+```bash
+default production: PEX.Production
+```
+
+With an argument, it set the default production.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -d PEX.Production
+```
+
+## 8.3. lists
+
+The lists command list productions.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -l
+```
+
+output :
+```bash
+{
+    "PEX.Production": {
+        "Status": "Stopped",
+        "LastStartTime": "2023-05-31 11:13:51.000",
+        "LastStopTime": "2023-05-31 11:13:54.153",
+        "AutoStart": 0
+    }
+}
+```
+
+## 8.4. start
+
+The start command start a production.
+
+To exit the command, you have to press CTRL+C.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -s PEX.Production
+```
+
+output :
+```bash
+2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting production
+2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.FileOperation
+2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.EmailOperation
+...
+```
+
+## 8.5. kill
+
+The kill command kill a production (force stop).
+
+Kill command is the same as stop command but with a force stop.
+
+Kill command doesn't take an argument because only one production can be running.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -k 
+```
+
+## 8.6. stop
+
+The stop command stop a production.
+
+Stop command doesn't take an argument because only one production can be running.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -S 
+```
+
+## 8.7. restart
+
+The restart command restart a production.
+
+Restart command doesn't take an argument because only one production can be running.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -r 
+```
+
+## 8.8. migrate
+
+The migrate command migrate a production and classes with settings file.
+
+Migrate command must take the absolute path of the settings file.
+
+Settings file must be in the same folder as the python code.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -M /tmp/settings.json
+```
+
+## 8.9. export
+
+The export command export a production.
+
+If no argument is given, the export command export the default production.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -e
+```
+
+If an argument is given, the export command export the production given in argument.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -e PEX.Production
+```
+
+output :
+```bash
+{
+    "Production": {
+        "@Name": "PEX.Production",
+        "@TestingEnabled": "true",
+        "@LogGeneralTraceEvents": "false",
+        "Description": "",
+        "ActorPoolSize": "2",
+        "Item": [
+            {
+                "@Name": "Python.FileOperation",
+                "@Category": "",
+                "@ClassName": "Python.FileOperation",
+                "@PoolSize": "1",
+                "@Enabled": "true",
+                "@Foreground": "false",
+                "@Comment": "",
+                "@LogTraceEvents": "true",
+                "@Schedule": "",
+                "Setting": [
+                    {
+                        "@Target": "Adapter",
+                        "@Name": "Charset",
+                        "#text": "utf-8"
+                    },
+                    {
+                        "@Target": "Adapter",
+                        "@Name": "FilePath",
+                        "#text": "/irisdev/app/output/"
+                    },
+                    {
+                        "@Target": "Host",
+                        "@Name": "%settings",
+                        "#text": "path=/irisdev/app/output/"
+                    }
+                ]
+            }
+        ]
+    }
+}
+```
+
+## 8.10. status
+
+The status command status a production.
+
+Status command doesn't take an argument because only one production can be running.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -x 
+```
+
+output :
+```bash
+{
+    "Production": "PEX.Production",
+    "Status": "stopped"
+}
+```
+
+Status can be :
+- stopped
+- running
+- suspended
+- troubled
+
+## 8.11. version
+
+The version command display the version.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -v
+```
+
+output :
+```bash
+2.3.0
+```
+
+## 8.12. log
+
+The log command display the log.
+
+To exit the command, you have to press CTRL+C.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -L
+```
+
+output :
+```bash
+2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting production
+2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.FileOperation
+2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.EmailOperation
+...
+```
+
+# 9. Credits
 
 Most of the code came from PEX for Python by Mo Cheng and Summer Gerry.
 
 Works only on IRIS 2021.2 +
```

### Comparing `iris_pex_embedded_python-2.2.0/README.md` & `iris_pex_embedded_python-2.3.0/src/iris_pex_embedded_python.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: iris-pex-embedded-python
+Version: 2.3.0
+Summary: iris_pex_embedded_python
+Home-page: https://github.com/grongierisc/interoperability-embedded-python
+Author: grongier
+Author-email: guillaume.rongier@intersystems.com
+License: MIT
+Keywords: iris_pex_embedded_python
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 1. interoperability-embedded-python
 
 This proof of concept aims to show how the **iris interoperability framework** can be use with **embedded python**.
 
 ## 1.1. Table of Contents
 
 - [1. interoperability-embedded-python](#1-interoperability-embedded-python)
@@ -41,17 +65,32 @@
   - [7.10. The `objects`](#710-the-objects)
   - [7.11. The `messages`](#711-the-messages)
   - [7.12. How to regsiter a component](#712-how-to-regsiter-a-component)
     - [7.12.1. register\_component](#7121-register_component)
     - [7.12.2. register\_file](#7122-register_file)
     - [7.12.3. register\_folder](#7123-register_folder)
     - [7.12.4. migrate](#7124-migrate)
-      - [7.12.4.1 setting.py file](#71241-settingpy-file)
+      - [7.12.4.1. setting.py file](#71241-settingpy-file)
+        - [7.12.4.1.1. CLASSES section](#712411-classes-section)
+        - [7.12.4.1.2. Productions section](#712412-productions-section)
   - [7.13. Direct use of Grongier.PEX](#713-direct-use-of-grongierpex)
-- [8. Credits](#8-credits)
+- [8. Command line](#8-command-line)
+  - [8.1. help](#81-help)
+  - [8.2. default](#82-default)
+  - [8.3. lists](#83-lists)
+  - [8.4. start](#84-start)
+  - [8.5. kill](#85-kill)
+  - [8.6. stop](#86-stop)
+  - [8.7. restart](#87-restart)
+  - [8.8. migrate](#88-migrate)
+  - [8.9. export](#89-export)
+  - [8.10. status](#810-status)
+  - [8.11. version](#811-version)
+  - [8.12. log](#812-log)
+- [9. Credits](#9-credits)
 
 ## 1.2. Example
 
 ```python
 from grongier.pex import BusinessOperation,Message
 
 class MyBusinessOperation(BusinessOperation):
@@ -703,33 +742,31 @@
 This class defines:
 
 `create_business_service`: The create_business_service() method initiates the specified business service.<br>
 **Parameters**:
 - **connection**: an IRISConnection object that specifies the connection to an IRIS instance for Java.
 - **target**: a string that specifies the name of the business service in the production definition.
 
+**Returns**:
+an object that contains an instance of IRISBusinessService
+
 `start_production`: The start_production() method starts the production.<br>
 **Parameters**:
 - **production_name**: a string that specifies the name of the production to start.
 
 `stop_production`: The stop_production() method stops the production.<br>
 **Parameters**:
 - **production_name**: a string that specifies the name of the production to stop.
 
 `restart_production`: The restart_production() method restarts the production.<br>
 **Parameters**:
 - **production_name**: a string that specifies the name of the production to restart.
 
 `list_productions`: The list_productions() method returns a dictionary of the names of the productions that are currently running.<br>
 
-**Returns**:
-an object that contains an instance of IRISBusinessService
-
-WIP example
-
 ## 7.10. The `objects`
 We will use `dataclass` to hold information in our [messages](#711-the-messages) in a `obj.py` file.
 
 Example of an object ( situated in the src/python/demo/reddit/obj.py file ):
 ```python
 from dataclasses import dataclass
 
@@ -847,15 +884,15 @@
 Then use this static method to migrate the settings file to the iris framework.
 
 ```python
 from grongier.pex import Utils
 Utils.migrate()
 ```
 
-#### 7.12.4.1 setting.py file
+#### 7.12.4.1. setting.py file
 
 This file is used to store the settings of the interoperability components.
 
 It has two sections :
 * `CLASSES` : This section is used to store the classes of the interoperability components.
 * `PRODUCTIONS` : This section is used to store the productions of the interoperability components.
 
@@ -928,26 +965,433 @@
             }
         ]
     }
     }
 ]
 ```
 
+##### 7.12.4.1.1. CLASSES section
+
+This section is used to store the classes of the interoperability components.
+
+It aims to help to register the components.
+
+This dictionary has the following structure :
+* Key : The name of the component
+* Value : 
+  * The class of the component (you have to import it before)
+  * The module of the component (you have to import it before)
+  * Another dictionary with the following structure :
+    * `module` : Name of the module of the component (optional)
+    * `class` : Name of the class of the component (optional)
+    * `path` : The path of the component (mandatory)
+
+e.g :
+
+When Value is a class or a module:
+```python
+import bo
+import bp
+from bs import RedditService
+
+CLASSES = {
+    'Python.RedditService': RedditService,
+    'Python.FilterPostRoutingRule': bp.FilterPostRoutingRule,
+    'Python.FileOperation': bo,
+}
+```
+
+When Value is a dictionary :
+```python
+CLASSES = {
+    'Python.RedditService': {
+        'module': 'bs',
+        'class': 'RedditService',
+        'path': '/irisdev/app/src/python/demo/'
+    },
+    'Python.Module': {
+        'module': 'bp',
+        'path': '/irisdev/app/src/python/demo/'
+    },
+    'Python.Package': {
+        'path': '/irisdev/app/src/python/demo/'
+    },
+}
+```
+
+##### 7.12.4.1.2. Productions section
+
+This section is used to store the productions of the interoperability components.
+
+It aims to help to register a production.
+
+This list has the following structure :
+* A list of dictionary with the following structure :
+  * `dc.Python.Production` : The name of the production
+    * `@Name` : The name of the production
+    * `@TestingEnabled` : The testing enabled of the production
+    * `@LogGeneralTraceEvents` : The log general trace events of the production
+    * `Description` : The description of the production
+    * `ActorPoolSize` : The actor pool size of the production
+    * `Item` : The list of the items of the production
+      * `@Name` : The name of the item
+      * `@Category` : The category of the item
+      * `@ClassName` : The class name of the item
+      * `@PoolSize` : The pool size of the item
+      * `@Enabled` : The enabled of the item
+      * `@Foreground` : The foreground of the item
+      * `@Comment` : The comment of the item
+      * `@LogTraceEvents` : The log trace events of the item
+      * `@Schedule` : The schedule of the item
+      * `Setting` : The list of the settings of the item
+        * `@Target` : The target of the setting
+        * `@Name` : The name of the setting
+        * `#text` : The value of the setting
+
+The minimum structure of a production is :
+```python
+PRODUCTIONS = [
+        {
+            'UnitTest.Production': {
+                "Item": [
+                    {
+                        "@Name": "Python.FileOperation",
+                        "@ClassName": "Python.FileOperation",
+                    },
+                    {
+                        "@Name": "Python.EmailOperation",
+                        "@ClassName": "UnitTest.Package.EmailOperation"
+                    }
+                ]
+            }
+        } 
+    ]
+```
+
+You can also set in `@ClassName` an item from the CLASSES section.
+
+e.g :
+```python
+from bo import FileOperation
+PRODUCTIONS = [
+        {
+            'UnitTest.Production': {
+                "Item": [
+                    {
+                        "@Name": "Python.FileOperation",
+                        "@ClassName": FileOperation,
+                    }
+                ]
+            }
+        } 
+    ]
+```
+
+As the production is a dictionary, you can add in value of the production dictionary an environment variable.
+
+e.g :
+```python
+import os
+
+PRODUCTIONS = [
+        {
+            'UnitTest.Production': {
+                "Item": [
+                    {
+                        "@Name": "Python.FileOperation",
+                        "@ClassName": "Python.FileOperation",
+                        "Setting": {
+                            "@Target": "Host",
+                            "@Name": "%settings",
+                            "#text": os.environ['SETTINGS']
+                        }
+                    }
+                ]
+            }
+        } 
+    ]
+```
+
 ## 7.13. Direct use of Grongier.PEX
 
 If you don't want to use the register_component util. You can add a Grongier.PEX.BusinessService component directly into the management portal and configure the properties :
 - %module :
   - Module name of your python code
 - %classname :
   - Classname of you component
 - %classpaths
   - Path where you component is.
     - This can one or more Classpaths (separated by '|' character) needed in addition to PYTHON_PATH
 
 e.g :
 <img width="800" alt="component-config" src="https://user-images.githubusercontent.com/47849411/131316308-e1898b19-11df-433b-b1c6-7f69d5cc9974.png">
 
-# 8. Credits
+# 8. Command line
+
+Since version 2.3.0, you can use the command line to register your components and productions.
+
+To use it, you have to use the following command :
+```bash
+/usr/irissys/bin/irispython -m grongier.pex 
+```
+
+output :
+```bash
+usage: python3 -m grongier.pex [-h] [-d DEFAULT] [-l] [-s START] [-k] [-S] [-r] [-M MIGRATE] [-e EXPORT] [-x] [-v] [-L]
+optional arguments:
+  -h, --help            display help and default production name
+  -d DEFAULT, --default DEFAULT
+                        set the default production
+  -l, --lists           list productions
+  -s START, --start START
+                        start a production
+  -k, --kill            kill a production (force stop)
+  -S, --stop            stop a production
+  -r, --restart         restart a production
+  -M MIGRATE, --migrate MIGRATE
+                        migrate production and classes with settings file
+  -e EXPORT, --export EXPORT
+                        export a production
+  -x, --status          status a production
+  -v, --version         display version
+  -L, --log             display log
+
+default production: PEX.Production
+```
+
+## 8.1. help
+
+The help command display the help and the default production name.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -h
+```
+
+output :
+```bash
+usage: python3 -m grongier.pex [-h] [-d DEFAULT] [-l] [-s START] [-k] [-S] [-r] [-M MIGRATE] [-e EXPORT] [-x] [-v] [-L]
+...
+default production: PEX.Production
+```
+
+## 8.2. default
+
+The default command set the default production.
+
+With no argument, it display the default production.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -d
+```
+
+output :
+```bash
+default production: PEX.Production
+```
+
+With an argument, it set the default production.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -d PEX.Production
+```
+
+## 8.3. lists
+
+The lists command list productions.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -l
+```
+
+output :
+```bash
+{
+    "PEX.Production": {
+        "Status": "Stopped",
+        "LastStartTime": "2023-05-31 11:13:51.000",
+        "LastStopTime": "2023-05-31 11:13:54.153",
+        "AutoStart": 0
+    }
+}
+```
+
+## 8.4. start
+
+The start command start a production.
+
+To exit the command, you have to press CTRL+C.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -s PEX.Production
+```
+
+output :
+```bash
+2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting production
+2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.FileOperation
+2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.EmailOperation
+...
+```
+
+## 8.5. kill
+
+The kill command kill a production (force stop).
+
+Kill command is the same as stop command but with a force stop.
+
+Kill command doesn't take an argument because only one production can be running.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -k 
+```
+
+## 8.6. stop
+
+The stop command stop a production.
+
+Stop command doesn't take an argument because only one production can be running.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -S 
+```
+
+## 8.7. restart
+
+The restart command restart a production.
+
+Restart command doesn't take an argument because only one production can be running.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -r 
+```
+
+## 8.8. migrate
+
+The migrate command migrate a production and classes with settings file.
+
+Migrate command must take the absolute path of the settings file.
+
+Settings file must be in the same folder as the python code.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -M /tmp/settings.json
+```
+
+## 8.9. export
+
+The export command export a production.
+
+If no argument is given, the export command export the default production.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -e
+```
+
+If an argument is given, the export command export the production given in argument.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -e PEX.Production
+```
+
+output :
+```bash
+{
+    "Production": {
+        "@Name": "PEX.Production",
+        "@TestingEnabled": "true",
+        "@LogGeneralTraceEvents": "false",
+        "Description": "",
+        "ActorPoolSize": "2",
+        "Item": [
+            {
+                "@Name": "Python.FileOperation",
+                "@Category": "",
+                "@ClassName": "Python.FileOperation",
+                "@PoolSize": "1",
+                "@Enabled": "true",
+                "@Foreground": "false",
+                "@Comment": "",
+                "@LogTraceEvents": "true",
+                "@Schedule": "",
+                "Setting": [
+                    {
+                        "@Target": "Adapter",
+                        "@Name": "Charset",
+                        "#text": "utf-8"
+                    },
+                    {
+                        "@Target": "Adapter",
+                        "@Name": "FilePath",
+                        "#text": "/irisdev/app/output/"
+                    },
+                    {
+                        "@Target": "Host",
+                        "@Name": "%settings",
+                        "#text": "path=/irisdev/app/output/"
+                    }
+                ]
+            }
+        ]
+    }
+}
+```
+
+## 8.10. status
+
+The status command status a production.
+
+Status command doesn't take an argument because only one production can be running.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -x 
+```
+
+output :
+```bash
+{
+    "Production": "PEX.Production",
+    "Status": "stopped"
+}
+```
+
+Status can be :
+- stopped
+- running
+- suspended
+- troubled
+
+## 8.11. version
+
+The version command display the version.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -v
+```
+
+output :
+```bash
+2.3.0
+```
+
+## 8.12. log
+
+The log command display the log.
+
+To exit the command, you have to press CTRL+C.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -L
+```
+
+output :
+```bash
+2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting production
+2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.FileOperation
+2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.EmailOperation
+...
+```
+
+# 9. Credits
 
 Most of the code came from PEX for Python by Mo Cheng and Summer Gerry.
 
-Works only on IRIS 2021.2 +
+Works only on IRIS 2021.2 +
```

### Comparing `iris_pex_embedded_python-2.2.0/setup.py` & `iris_pex_embedded_python-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     # Do the setup
     setup(
         name='iris_pex_embedded_python',
         description='iris_pex_embedded_python',
         long_description=long_description,
         long_description_content_type='text/markdown',
-        version='2.2.0',
+        version='2.3.0',
         author='grongier',
         author_email='guillaume.rongier@intersystems.com',
         keywords='iris_pex_embedded_python',
         url='https://github.com/grongierisc/interoperability-embedded-python',
         license='MIT',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
```

### Comparing `iris_pex_embedded_python-2.2.0/src/grongier/pex/__init__.py` & `iris_pex_embedded_python-2.3.0/src/grongier/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.2.0/src/grongier/pex/_business_host.py` & `iris_pex_embedded_python-2.3.0/src/grongier/pex/_business_host.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.2.0/src/grongier/pex/_business_operation.py` & `iris_pex_embedded_python-2.3.0/src/grongier/pex/_business_operation.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.2.0/src/grongier/pex/_business_process.py` & `iris_pex_embedded_python-2.3.0/src/grongier/pex/_business_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.2.0/src/grongier/pex/_business_service.py` & `iris_pex_embedded_python-2.3.0/src/grongier/pex/_business_service.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.2.0/src/grongier/pex/_common.py` & `iris_pex_embedded_python-2.3.0/src/grongier/pex/_common.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.2.0/src/grongier/pex/_director.py` & `iris_pex_embedded_python-2.3.0/src/grongier/pex/_director.py`

 * *Files 23% similar despite different names*

```diff
@@ -53,60 +53,88 @@
         """
         iris_object = iris.cls("Grongier.PEX.Director").dispatchCreateBusinessService(target)
         return iris_object.GetClass()
     
     ### List of function to manage the production
     ### start production
     @staticmethod
-    def start_production(production_name=None):
+    def start_production(production_name=None): 
+        if production_name is None or production_name == '':
+            production_name = _Director.get_default_production()
         # create two async task
         loop = asyncio.get_event_loop()
         handler = SIGINT_handler()
         print('start production')
         loop.run_until_complete(asyncio.gather(
             _Director.start_production_async(production_name, handler),
             _Director.log_production(handler)
         ))
 
     @staticmethod
     async def start_production_async(production_name=None, handler=None):
+        if production_name is None or production_name == '':
+            production_name = _Director.get_default_production()
         signal.signal(signal.SIGINT, handler.signal_handler)
         iris.cls('Ens.Director').StartProduction(production_name)
         while True:
             if handler.SIGINT:
                 print('try to stop production')
-                _Director.stop_production(production_name)
+                _Director.stop_production()
                 print('production stopped')
                 break
             await asyncio.sleep(1)
 
     ### stop production
     @staticmethod
-    def stop_production(production_name=None):
+    def stop_production():
         iris.cls('Ens.Director').StopProduction()
 
     ### restart production
     @staticmethod
-    def restart_production(production_name=None):
+    def restart_production():
         iris.cls('Ens.Director').RestartProduction()
 
     ### shutdown production
     @staticmethod
-    def shutdown_production(production_name=None):
+    def shutdown_production():
         iris.cls('Ens.Director').StopProduction(10,1)
 
     ### update production
     @staticmethod
-    def update_production(production_name=None):
+    def update_production():
         iris.cls('Ens.Director').UpdateProduction()
 
     ### list production
     @staticmethod
     def list_productions():
         return iris.cls('Grongier.PEX.Director').dispatchListProductions()
+    
+    ### status production
+    @staticmethod
+    def status_production():
+        dikt = iris.cls('Grongier.PEX.Director').StatusProduction()
+        if dikt['Production'] is None or dikt['Production'] == '':
+            dikt['Production'] = _Director.get_default_production()
+        return dikt
+
+    ### set default production
+    @staticmethod
+    def set_default_production(production_name=''):
+        #set ^Ens.Configuration("SuperUser","LastProduction")
+        glb = iris.gref("^Ens.Configuration")
+        glb['csp', "LastProduction"] = production_name
+
+    ### get default production
+    @staticmethod
+    def get_default_production():
+        glb = iris.gref("^Ens.Configuration")
+        default_production_name = glb['csp', "LastProduction"]
+        if default_production_name is None or default_production_name == '':
+            default_production_name = 'Not defined'
+        return default_production_name
 
     @staticmethod
     def read_log(handler):
         sql = """
         SELECT 
         ID, ConfigName, Job, MessageId, SessionId, SourceClass, SourceMethod, Stack, Text, TimeLogged, TraceCat, Type
         FROM Ens_Util.Log
@@ -129,14 +157,23 @@
         """ Log production 
             if ctrl+c is pressed, the log is stopped
         """
         for line in _Director.read_log(handler):
             print(line)
             sys.stdout.flush()
 
+    @staticmethod
+    def start_log_production():
+        """ Log production 
+            if ctrl+c is pressed, the log is stopped
+        """
+        loop = asyncio.get_event_loop()
+        handler = SIGINT_handler()
+        loop.run_until_complete(_Director.log_production(handler))
+
             
 
 class SIGINT_handler():
     def __init__(self):
         self.SIGINT = False
 
     def signal_handler(self, signal, frame):
```

### Comparing `iris_pex_embedded_python-2.2.0/src/grongier/pex/_inbound_adapter.py` & `iris_pex_embedded_python-2.3.0/src/grongier/pex/_inbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.2.0/src/grongier/pex/_outbound_adapter.py` & `iris_pex_embedded_python-2.3.0/src/grongier/pex/_outbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.2.0/src/grongier/pex/_private_session_duplex.py` & `iris_pex_embedded_python-2.3.0/src/grongier/pex/_private_session_duplex.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.2.0/src/grongier/pex/_private_session_process.py` & `iris_pex_embedded_python-2.3.0/src/grongier/pex/_private_session_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.2.0/src/grongier/pex/_utils.py` & `iris_pex_embedded_python-2.3.0/src/grongier/pex/_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -38,15 +38,17 @@
         :type path: str
         :param overwrite: 0 = no, 1 = yes
         :type overwrite: int
         :param iris_classname: The name of the class in the Iris class hierarchy
         :type iris_classname: str
         :return: The return value is a string.
         """
-
+        path = os.path.normpath(path)
+        # get the absolute path of the folder
+        path = os.path.abspath(path)
         return iris.cls('Grongier.PEX.Utils').dispatchRegisterComponent(module,classname,path,overwrite,iris_classname)
 
     @staticmethod
     def register_folder(path:str,overwrite:int=1,iris_package_name:str='Python'):
         """
         > This function takes a path to a folder, and registers all the Python files in that folder as IRIS
         classes
@@ -55,14 +57,16 @@
         :type path: str
         :param overwrite: 
         :type overwrite: int
         :param iris_package_name: The name of the iris package you want to register the file to
         :type iris_package_name: str
         """
         path = os.path.normpath(path)
+        # get the absolute path of the folder
+        path = os.path.abspath(path)
         for filename in os.listdir(path):
             if filename.endswith(".py"): 
                 _Utils._register_file(filename, path, overwrite, iris_package_name)
             else:
                 continue
 
     @staticmethod
@@ -132,16 +136,16 @@
         :type path: str
         :param overwrite: 0 = don't overwrite, 1 = overwrite
         :type overwrite: int
         :param iris_package_name: The name of the package in the Iris package manager
         :type iris_package_name: str
         """
         for filename in os.listdir(os.path.join(path,package)):
-            if filename.endswith(".py"): 
-                _Utils._register_file(os.path.join(package,filename), path, overwrite, iris_package_name)
+            if filename.endswith(".py"):
+                _Utils._register_file(filename, os.path.join(path,package), overwrite, iris_package_name)
             else:
                 continue
 
     @staticmethod
     def filename_to_module(filename) -> str:
         """
         It takes a filename and returns the module name
@@ -158,29 +162,39 @@
             module = packages+'.'+mod
         else:
             module = mod
 
         return module
 
     @staticmethod
-    def migrate():
+    def migrate(filename=None):
         """ 
         Read the settings.py file and register all the components
         settings.py file has two dictionaries:
             * CLASSES
                 * key: the name of the class
                 * value: an instance of the class
             * PRODUCTIONS
                 list of dictionaries:
                 * key: the name of the production
                 * value: a dictionary containing the settings for the production
         """
         # try to load the settings file
         try:
-            from settings import CLASSES, PRODUCTIONS
+            if filename:
+                import sys
+                path = None
+                # check if the filename is absolute or relative
+                if os.path.isabs(filename):
+                    path = os.path.dirname(filename)
+                else:
+                    raise ValueError("The filename must be absolute")
+                # add the path to the system path
+                sys.path.append(path)
+                from settings import CLASSES, PRODUCTIONS
         except ImportError:
             # return an error if the settings file is not found
             # and explain how to create it
             raise ImportError("settings.py file not found. Please create it in the same directory as the main.py file. See the documentation for more information.")
         _Utils.set_classes_settings(CLASSES)
         _Utils.set_productions_settings(PRODUCTIONS)
 
@@ -190,42 +204,98 @@
         """
         It takes a dictionary of classes and returns a dictionary of settings for each class
         
         :param class_items: a dictionary of classes
         :return: a dictionary of settings for each class
         """
         for key, value in class_items.items():
-            path = os.path.dirname(inspect.getfile(value))
-            _Utils.register_component(value.__module__,value.__name__,path,1,key)
+            if inspect.isclass(value):
+                path = os.path.dirname(inspect.getfile(value))
+                _Utils.register_component(value.__module__,value.__name__,path,1,key)
+            elif inspect.ismodule(value):
+                path = os.path.dirname(inspect.getfile(value))
+                _Utils._register_file(value.__name__+'.py',path,1,key)
+            # if the value is a dict
+            elif isinstance(value,dict):
+                # if the dict has a key 'path' and a key 'module' and a key 'class'
+                if 'path' in value and 'module' in value and 'class' in value:
+                    # register the component
+                    _Utils.register_component(value['module'],value['class'],value['path'],1,key)
+                # if the dict has a key 'path' and a key 'package'
+                elif 'path' in value and 'package' in value:
+                    # register the package
+                    _Utils.register_package(value['package'],value['path'],1,key)
+                # if the dict has a key 'path' and a key 'file'
+                elif 'path' in value and 'file' in value:
+                    # register the file
+                    _Utils._register_file(value['file'],value['path'],1,key)
+                # if the dict has a key 'path'
+                elif 'path' in value:
+                    # register folder
+                    _Utils.register_folder(value['path'],1,key)
+                else:
+                    raise ValueError(f"Invalid value for {key}.")
+
 
     @staticmethod
     def set_productions_settings(production_list):
         """
         It takes a list of dictionaries and registers the productions
         """
         # for each production in the list
         for production in production_list:
             # get the production name (first key in the dictionary)
             production_name = list(production.keys())[0]
             # set the first key to 'production'
             production['Production'] = production.pop(production_name)
+            # handle Items
+            production = _Utils.handle_items(production)
             # transform the json as an xml
             xml = _Utils.dict_to_xml(production)
             # register the production
             _Utils.register_production(production_name,xml)
-    
+
+    @staticmethod
+    def handle_items(production):
+        # if an item is a class, register it and replace it with the name of the class
+        if 'Item' in production['Production']:
+            # for each item in the list
+            for i,item in enumerate(production['Production']['Item']):
+                # if the attribute "@ClassName" is a class, register it and replace it with the name of the class
+                if '@ClassName' in item:
+                    if inspect.isclass(item['@ClassName']):
+                        path = os.path.dirname(inspect.getfile(item['@ClassName']))
+                        _Utils.register_component(item['@ClassName'].__module__,item['@ClassName'].__name__,path,1,item['@Name'])
+                        # replace the class with the name of the class
+                        production['Production']['Item'][i]['@ClassName'] = item['@Name']
+                # if the attribute "@ClassName" is a dict
+                elif isinstance(item['@ClassName'],dict):
+                    # create a new dict where the key is the name of the class and the value is the dict
+                    class_dict = {item['@Name']:item['@ClassName']}
+                    # pass the new dict to set_classes_settings
+                    _Utils.set_classes_settings(class_dict)
+                    # replace the class with the name of the class
+                    production['Production']['Item'][i]['@ClassName'] = item['@Name']
+
+        return production
+
     @staticmethod
     def dict_to_xml(json):
         """
         It takes a json and returns an xml
         
         :param json: a json
         :return: an xml
         """
-        return xmltodict.unparse(json)  
+        xml = xmltodict.unparse(json,pretty=True)
+        # remove the xml version tag
+        xml = xml.replace('<?xml version="1.0" encoding="utf-8"?>','')
+        # remove the new line at the beginning of the xml
+        xml = xml[1:]
+        return xml
     
     @staticmethod
     def register_production(production_name,xml):
         """
         It takes a production name and an xml and registers the production
         
         :param production_name: the name of the production
@@ -233,9 +303,38 @@
         :param xml: the xml of the production
         :type xml: str
         """
         # split the production name in the package name and the production name
         # the production name is the last part of the string
         package = '.'.join(production_name.split('.')[:-1])
         production_name = production_name.split('.')[-1]
+        stream = iris.cls('%Stream.GlobalCharacter')._New()
+        # for each chunk of 1024 characters
+        for i in range(0, len(xml), 1024):
+            # write the chunk to the stream
+            stream.Write(xml[i:i+1024])
         # register the production
-        _Utils.raise_on_error(iris.cls('Grongier.PEX.Utils').CreateProduction(package,production_name,xml))
+        _Utils.raise_on_error(iris.cls('Grongier.PEX.Utils').CreateProduction(package,production_name,stream))
+
+    @staticmethod
+    def export_production(production_name):
+        """
+        It takes a production name and exports the production
+        
+        :param production_name: the name of the production
+        :type production_name: str
+        """
+        def postprocessor(path, key, value):
+            if value is None:
+                return key, ''
+            return key, value
+        # export the production
+        xdata = iris.cls('Grongier.PEX.Utils').ExportProduction(production_name)
+        # for each chunk of 1024 characters
+        string = ""
+        xdata.Rewind()
+        while not xdata.AtEnd:
+            string += xdata.Read(1024)
+        # convert the xml to a dictionary
+        data = xmltodict.parse(string,postprocessor=postprocessor)
+        # return the dictionary
+        return data
```

### Comparing `iris_pex_embedded_python-2.2.0/src/iris_pex_embedded_python.egg-info/PKG-INFO` & `iris_pex_embedded_python-2.3.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: iris-pex-embedded-python
-Version: 2.2.0
-Summary: iris_pex_embedded_python
-Home-page: https://github.com/grongierisc/interoperability-embedded-python
-Author: grongier
-Author-email: guillaume.rongier@intersystems.com
-License: MIT
-Keywords: iris_pex_embedded_python
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 1. interoperability-embedded-python
 
 This proof of concept aims to show how the **iris interoperability framework** can be use with **embedded python**.
 
 ## 1.1. Table of Contents
 
 - [1. interoperability-embedded-python](#1-interoperability-embedded-python)
@@ -65,17 +41,32 @@
   - [7.10. The `objects`](#710-the-objects)
   - [7.11. The `messages`](#711-the-messages)
   - [7.12. How to regsiter a component](#712-how-to-regsiter-a-component)
     - [7.12.1. register\_component](#7121-register_component)
     - [7.12.2. register\_file](#7122-register_file)
     - [7.12.3. register\_folder](#7123-register_folder)
     - [7.12.4. migrate](#7124-migrate)
-      - [7.12.4.1 setting.py file](#71241-settingpy-file)
+      - [7.12.4.1. setting.py file](#71241-settingpy-file)
+        - [7.12.4.1.1. CLASSES section](#712411-classes-section)
+        - [7.12.4.1.2. Productions section](#712412-productions-section)
   - [7.13. Direct use of Grongier.PEX](#713-direct-use-of-grongierpex)
-- [8. Credits](#8-credits)
+- [8. Command line](#8-command-line)
+  - [8.1. help](#81-help)
+  - [8.2. default](#82-default)
+  - [8.3. lists](#83-lists)
+  - [8.4. start](#84-start)
+  - [8.5. kill](#85-kill)
+  - [8.6. stop](#86-stop)
+  - [8.7. restart](#87-restart)
+  - [8.8. migrate](#88-migrate)
+  - [8.9. export](#89-export)
+  - [8.10. status](#810-status)
+  - [8.11. version](#811-version)
+  - [8.12. log](#812-log)
+- [9. Credits](#9-credits)
 
 ## 1.2. Example
 
 ```python
 from grongier.pex import BusinessOperation,Message
 
 class MyBusinessOperation(BusinessOperation):
@@ -727,33 +718,31 @@
 This class defines:
 
 `create_business_service`: The create_business_service() method initiates the specified business service.<br>
 **Parameters**:
 - **connection**: an IRISConnection object that specifies the connection to an IRIS instance for Java.
 - **target**: a string that specifies the name of the business service in the production definition.
 
+**Returns**:
+an object that contains an instance of IRISBusinessService
+
 `start_production`: The start_production() method starts the production.<br>
 **Parameters**:
 - **production_name**: a string that specifies the name of the production to start.
 
 `stop_production`: The stop_production() method stops the production.<br>
 **Parameters**:
 - **production_name**: a string that specifies the name of the production to stop.
 
 `restart_production`: The restart_production() method restarts the production.<br>
 **Parameters**:
 - **production_name**: a string that specifies the name of the production to restart.
 
 `list_productions`: The list_productions() method returns a dictionary of the names of the productions that are currently running.<br>
 
-**Returns**:
-an object that contains an instance of IRISBusinessService
-
-WIP example
-
 ## 7.10. The `objects`
 We will use `dataclass` to hold information in our [messages](#711-the-messages) in a `obj.py` file.
 
 Example of an object ( situated in the src/python/demo/reddit/obj.py file ):
 ```python
 from dataclasses import dataclass
 
@@ -871,15 +860,15 @@
 Then use this static method to migrate the settings file to the iris framework.
 
 ```python
 from grongier.pex import Utils
 Utils.migrate()
 ```
 
-#### 7.12.4.1 setting.py file
+#### 7.12.4.1. setting.py file
 
 This file is used to store the settings of the interoperability components.
 
 It has two sections :
 * `CLASSES` : This section is used to store the classes of the interoperability components.
 * `PRODUCTIONS` : This section is used to store the productions of the interoperability components.
 
@@ -952,26 +941,433 @@
             }
         ]
     }
     }
 ]
 ```
 
+##### 7.12.4.1.1. CLASSES section
+
+This section is used to store the classes of the interoperability components.
+
+It aims to help to register the components.
+
+This dictionary has the following structure :
+* Key : The name of the component
+* Value : 
+  * The class of the component (you have to import it before)
+  * The module of the component (you have to import it before)
+  * Another dictionary with the following structure :
+    * `module` : Name of the module of the component (optional)
+    * `class` : Name of the class of the component (optional)
+    * `path` : The path of the component (mandatory)
+
+e.g :
+
+When Value is a class or a module:
+```python
+import bo
+import bp
+from bs import RedditService
+
+CLASSES = {
+    'Python.RedditService': RedditService,
+    'Python.FilterPostRoutingRule': bp.FilterPostRoutingRule,
+    'Python.FileOperation': bo,
+}
+```
+
+When Value is a dictionary :
+```python
+CLASSES = {
+    'Python.RedditService': {
+        'module': 'bs',
+        'class': 'RedditService',
+        'path': '/irisdev/app/src/python/demo/'
+    },
+    'Python.Module': {
+        'module': 'bp',
+        'path': '/irisdev/app/src/python/demo/'
+    },
+    'Python.Package': {
+        'path': '/irisdev/app/src/python/demo/'
+    },
+}
+```
+
+##### 7.12.4.1.2. Productions section
+
+This section is used to store the productions of the interoperability components.
+
+It aims to help to register a production.
+
+This list has the following structure :
+* A list of dictionary with the following structure :
+  * `dc.Python.Production` : The name of the production
+    * `@Name` : The name of the production
+    * `@TestingEnabled` : The testing enabled of the production
+    * `@LogGeneralTraceEvents` : The log general trace events of the production
+    * `Description` : The description of the production
+    * `ActorPoolSize` : The actor pool size of the production
+    * `Item` : The list of the items of the production
+      * `@Name` : The name of the item
+      * `@Category` : The category of the item
+      * `@ClassName` : The class name of the item
+      * `@PoolSize` : The pool size of the item
+      * `@Enabled` : The enabled of the item
+      * `@Foreground` : The foreground of the item
+      * `@Comment` : The comment of the item
+      * `@LogTraceEvents` : The log trace events of the item
+      * `@Schedule` : The schedule of the item
+      * `Setting` : The list of the settings of the item
+        * `@Target` : The target of the setting
+        * `@Name` : The name of the setting
+        * `#text` : The value of the setting
+
+The minimum structure of a production is :
+```python
+PRODUCTIONS = [
+        {
+            'UnitTest.Production': {
+                "Item": [
+                    {
+                        "@Name": "Python.FileOperation",
+                        "@ClassName": "Python.FileOperation",
+                    },
+                    {
+                        "@Name": "Python.EmailOperation",
+                        "@ClassName": "UnitTest.Package.EmailOperation"
+                    }
+                ]
+            }
+        } 
+    ]
+```
+
+You can also set in `@ClassName` an item from the CLASSES section.
+
+e.g :
+```python
+from bo import FileOperation
+PRODUCTIONS = [
+        {
+            'UnitTest.Production': {
+                "Item": [
+                    {
+                        "@Name": "Python.FileOperation",
+                        "@ClassName": FileOperation,
+                    }
+                ]
+            }
+        } 
+    ]
+```
+
+As the production is a dictionary, you can add in value of the production dictionary an environment variable.
+
+e.g :
+```python
+import os
+
+PRODUCTIONS = [
+        {
+            'UnitTest.Production': {
+                "Item": [
+                    {
+                        "@Name": "Python.FileOperation",
+                        "@ClassName": "Python.FileOperation",
+                        "Setting": {
+                            "@Target": "Host",
+                            "@Name": "%settings",
+                            "#text": os.environ['SETTINGS']
+                        }
+                    }
+                ]
+            }
+        } 
+    ]
+```
+
 ## 7.13. Direct use of Grongier.PEX
 
 If you don't want to use the register_component util. You can add a Grongier.PEX.BusinessService component directly into the management portal and configure the properties :
 - %module :
   - Module name of your python code
 - %classname :
   - Classname of you component
 - %classpaths
   - Path where you component is.
     - This can one or more Classpaths (separated by '|' character) needed in addition to PYTHON_PATH
 
 e.g :
 <img width="800" alt="component-config" src="https://user-images.githubusercontent.com/47849411/131316308-e1898b19-11df-433b-b1c6-7f69d5cc9974.png">
 
-# 8. Credits
+# 8. Command line
+
+Since version 2.3.0, you can use the command line to register your components and productions.
+
+To use it, you have to use the following command :
+```bash
+/usr/irissys/bin/irispython -m grongier.pex 
+```
+
+output :
+```bash
+usage: python3 -m grongier.pex [-h] [-d DEFAULT] [-l] [-s START] [-k] [-S] [-r] [-M MIGRATE] [-e EXPORT] [-x] [-v] [-L]
+optional arguments:
+  -h, --help            display help and default production name
+  -d DEFAULT, --default DEFAULT
+                        set the default production
+  -l, --lists           list productions
+  -s START, --start START
+                        start a production
+  -k, --kill            kill a production (force stop)
+  -S, --stop            stop a production
+  -r, --restart         restart a production
+  -M MIGRATE, --migrate MIGRATE
+                        migrate production and classes with settings file
+  -e EXPORT, --export EXPORT
+                        export a production
+  -x, --status          status a production
+  -v, --version         display version
+  -L, --log             display log
+
+default production: PEX.Production
+```
+
+## 8.1. help
+
+The help command display the help and the default production name.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -h
+```
+
+output :
+```bash
+usage: python3 -m grongier.pex [-h] [-d DEFAULT] [-l] [-s START] [-k] [-S] [-r] [-M MIGRATE] [-e EXPORT] [-x] [-v] [-L]
+...
+default production: PEX.Production
+```
+
+## 8.2. default
+
+The default command set the default production.
+
+With no argument, it display the default production.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -d
+```
+
+output :
+```bash
+default production: PEX.Production
+```
+
+With an argument, it set the default production.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -d PEX.Production
+```
+
+## 8.3. lists
+
+The lists command list productions.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -l
+```
+
+output :
+```bash
+{
+    "PEX.Production": {
+        "Status": "Stopped",
+        "LastStartTime": "2023-05-31 11:13:51.000",
+        "LastStopTime": "2023-05-31 11:13:54.153",
+        "AutoStart": 0
+    }
+}
+```
+
+## 8.4. start
+
+The start command start a production.
+
+To exit the command, you have to press CTRL+C.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -s PEX.Production
+```
+
+output :
+```bash
+2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting production
+2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.FileOperation
+2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.EmailOperation
+...
+```
+
+## 8.5. kill
+
+The kill command kill a production (force stop).
+
+Kill command is the same as stop command but with a force stop.
+
+Kill command doesn't take an argument because only one production can be running.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -k 
+```
+
+## 8.6. stop
+
+The stop command stop a production.
+
+Stop command doesn't take an argument because only one production can be running.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -S 
+```
+
+## 8.7. restart
+
+The restart command restart a production.
+
+Restart command doesn't take an argument because only one production can be running.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -r 
+```
+
+## 8.8. migrate
+
+The migrate command migrate a production and classes with settings file.
+
+Migrate command must take the absolute path of the settings file.
+
+Settings file must be in the same folder as the python code.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -M /tmp/settings.json
+```
+
+## 8.9. export
+
+The export command export a production.
+
+If no argument is given, the export command export the default production.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -e
+```
+
+If an argument is given, the export command export the production given in argument.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -e PEX.Production
+```
+
+output :
+```bash
+{
+    "Production": {
+        "@Name": "PEX.Production",
+        "@TestingEnabled": "true",
+        "@LogGeneralTraceEvents": "false",
+        "Description": "",
+        "ActorPoolSize": "2",
+        "Item": [
+            {
+                "@Name": "Python.FileOperation",
+                "@Category": "",
+                "@ClassName": "Python.FileOperation",
+                "@PoolSize": "1",
+                "@Enabled": "true",
+                "@Foreground": "false",
+                "@Comment": "",
+                "@LogTraceEvents": "true",
+                "@Schedule": "",
+                "Setting": [
+                    {
+                        "@Target": "Adapter",
+                        "@Name": "Charset",
+                        "#text": "utf-8"
+                    },
+                    {
+                        "@Target": "Adapter",
+                        "@Name": "FilePath",
+                        "#text": "/irisdev/app/output/"
+                    },
+                    {
+                        "@Target": "Host",
+                        "@Name": "%settings",
+                        "#text": "path=/irisdev/app/output/"
+                    }
+                ]
+            }
+        ]
+    }
+}
+```
+
+## 8.10. status
+
+The status command status a production.
+
+Status command doesn't take an argument because only one production can be running.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -x 
+```
+
+output :
+```bash
+{
+    "Production": "PEX.Production",
+    "Status": "stopped"
+}
+```
+
+Status can be :
+- stopped
+- running
+- suspended
+- troubled
+
+## 8.11. version
+
+The version command display the version.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -v
+```
+
+output :
+```bash
+2.3.0
+```
+
+## 8.12. log
+
+The log command display the log.
+
+To exit the command, you have to press CTRL+C.
+
+```bash
+/usr/irissys/bin/irispython -m grongier.pex -L
+```
+
+output :
+```bash
+2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting production
+2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.FileOperation
+2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.EmailOperation
+...
+```
+
+# 9. Credits
 
 Most of the code came from PEX for Python by Mo Cheng and Summer Gerry.
 
-Works only on IRIS 2021.2 +
+Works only on IRIS 2021.2 +
```

### Comparing `iris_pex_embedded_python-2.2.0/src/iris_pex_embedded_python.egg-info/SOURCES.txt` & `iris_pex_embedded_python-2.3.0/src/iris_pex_embedded_python.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/grongier/iris/__init__.py
 src/grongier/pex/__init__.py
+src/grongier/pex/__main__.py
 src/grongier/pex/_business_host.py
 src/grongier/pex/_business_operation.py
 src/grongier/pex/_business_process.py
 src/grongier/pex/_business_service.py
+src/grongier/pex/_cli.py
 src/grongier/pex/_common.py
 src/grongier/pex/_director.py
 src/grongier/pex/_inbound_adapter.py
 src/grongier/pex/_message.py
 src/grongier/pex/_outbound_adapter.py
 src/grongier/pex/_pickle_message.py
 src/grongier/pex/_private_session_duplex.py
```

