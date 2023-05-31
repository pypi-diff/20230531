# Comparing `tmp/pyechorobotics-0.0.2.tar.gz` & `tmp/pyechorobotics-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyechorobotics-0.0.2.tar", last modified: Wed May 31 16:41:05 2023, max compression
+gzip compressed data, was "pyechorobotics-0.0.3.tar", last modified: Wed May 31 18:30:31 2023, max compression
```

## Comparing `pyechorobotics-0.0.2.tar` & `pyechorobotics-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:41:05.207104 pyechorobotics-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 16:40:54.000000 pyechorobotics-0.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-31 16:41:05.207104 pyechorobotics-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-31 16:40:54.000000 pyechorobotics-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-31 16:40:54.000000 pyechorobotics-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-31 16:41:05.207104 pyechorobotics-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-31 16:40:54.000000 pyechorobotics-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:41:05.207104 pyechorobotics-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:41:05.207104 pyechorobotics-0.0.2/src/echoroboticsapi/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 16:40:54.000000 pyechorobotics-0.0.2/src/echoroboticsapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-31 16:40:54.000000 pyechorobotics-0.0.2/src/echoroboticsapi/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-31 16:40:54.000000 pyechorobotics-0.0.2/src/echoroboticsapi/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:41:05.207104 pyechorobotics-0.0.2/src/pyechorobotics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-31 16:41:05.000000 pyechorobotics-0.0.2/src/pyechorobotics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-31 16:41:05.000000 pyechorobotics-0.0.2/src/pyechorobotics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 16:41:05.000000 pyechorobotics-0.0.2/src/pyechorobotics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 16:41:05.000000 pyechorobotics-0.0.2/src/pyechorobotics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 16:41:05.000000 pyechorobotics-0.0.2/src/pyechorobotics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:30:31.943752 pyechorobotics-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 18:30:17.000000 pyechorobotics-0.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-31 18:30:31.943752 pyechorobotics-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-31 18:30:17.000000 pyechorobotics-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-31 18:30:17.000000 pyechorobotics-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-31 18:30:31.947752 pyechorobotics-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-31 18:30:17.000000 pyechorobotics-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:30:31.943752 pyechorobotics-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:30:31.943752 pyechorobotics-0.0.3/src/echoroboticsapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 18:30:17.000000 pyechorobotics-0.0.3/src/echoroboticsapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-31 18:30:17.000000 pyechorobotics-0.0.3/src/echoroboticsapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-31 18:30:17.000000 pyechorobotics-0.0.3/src/echoroboticsapi/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:30:31.943752 pyechorobotics-0.0.3/src/pyechorobotics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-31 18:30:31.000000 pyechorobotics-0.0.3/src/pyechorobotics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-31 18:30:31.000000 pyechorobotics-0.0.3/src/pyechorobotics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:30:31.000000 pyechorobotics-0.0.3/src/pyechorobotics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 18:30:31.000000 pyechorobotics-0.0.3/src/pyechorobotics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 18:30:31.000000 pyechorobotics-0.0.3/src/pyechorobotics.egg-info/top_level.txt
```

### Comparing `pyechorobotics-0.0.2/LICENSE.md` & `pyechorobotics-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyechorobotics-0.0.2/PKG-INFO` & `pyechorobotics-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyechorobotics
-Version: 0.0.2
+Version: 0.0.3
 Summary: Access API for echorobotics robot lawn mowers
 Author-email: functionpointer <suspendfunction@gmail.com>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: homepage, https://github.com/functionpointer/pyechorobotics
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.10
```

### Comparing `pyechorobotics-0.0.2/README.md` & `pyechorobotics-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyechorobotics-0.0.2/pyproject.toml` & `pyechorobotics-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyechorobotics"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = [
     "aiohttp",
     "yarl",
     "pydantic",
 ]
 readme = "README.md"
 license = {text = "GNU General Public License v3 or later (GPLv3+)"}
```

### Comparing `pyechorobotics-0.0.2/src/echoroboticsapi/api.py` & `pyechorobotics-0.0.3/src/echoroboticsapi/api.py`

 * *Files identical despite different names*

### Comparing `pyechorobotics-0.0.2/src/echoroboticsapi/models.py` & `pyechorobotics-0.0.3/src/echoroboticsapi/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     longitude: float = Field(..., alias="Longitude")
     latitude: float = Field(..., alias="Latitude")
     datetime: DateTimeISO8601 = Field(..., alias="DateTime")
 
 
 class StatusInfo(BaseModel):
     robot: RobotId = Field(..., alias="Robot")
-    status: Literal["WaitStation", "Idle"] = Field(..., alias="Status")
+    status: Literal["WaitStation", "Idle", "Work"] = Field(..., alias="Status")
     mac_address: str = Field(..., alias="MacAddress")
     date: DateTimeISO8601 = Field(..., alias="Date")
     delta: str = Field(..., alias="Delta")
     estimated_battery_level: float = Field(..., alias="EstimatedBatteryLevel")
     position: Position = Field(..., alias="Position")
     query_time: DateTimeISO8601 = Field(..., alias="QueryTime")
     has_values: bool = Field(..., alias="HasValues")
```

### Comparing `pyechorobotics-0.0.2/src/pyechorobotics.egg-info/PKG-INFO` & `pyechorobotics-0.0.3/src/pyechorobotics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyechorobotics
-Version: 0.0.2
+Version: 0.0.3
 Summary: Access API for echorobotics robot lawn mowers
 Author-email: functionpointer <suspendfunction@gmail.com>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: homepage, https://github.com/functionpointer/pyechorobotics
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.10
```

