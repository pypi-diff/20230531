# Comparing `tmp/pyechorobotics-0.0.3.tar.gz` & `tmp/pyechorobotics-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyechorobotics-0.0.3.tar", last modified: Wed May 31 18:30:31 2023, max compression
+gzip compressed data, was "pyechorobotics-0.0.4.tar", last modified: Wed May 31 21:00:47 2023, max compression
```

## Comparing `pyechorobotics-0.0.3.tar` & `pyechorobotics-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:30:31.943752 pyechorobotics-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 18:30:17.000000 pyechorobotics-0.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-31 18:30:31.943752 pyechorobotics-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-31 18:30:17.000000 pyechorobotics-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-31 18:30:17.000000 pyechorobotics-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-31 18:30:31.947752 pyechorobotics-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-31 18:30:17.000000 pyechorobotics-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:30:31.943752 pyechorobotics-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:30:31.943752 pyechorobotics-0.0.3/src/echoroboticsapi/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 18:30:17.000000 pyechorobotics-0.0.3/src/echoroboticsapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-31 18:30:17.000000 pyechorobotics-0.0.3/src/echoroboticsapi/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-31 18:30:17.000000 pyechorobotics-0.0.3/src/echoroboticsapi/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:30:31.943752 pyechorobotics-0.0.3/src/pyechorobotics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-31 18:30:31.000000 pyechorobotics-0.0.3/src/pyechorobotics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-31 18:30:31.000000 pyechorobotics-0.0.3/src/pyechorobotics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:30:31.000000 pyechorobotics-0.0.3/src/pyechorobotics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 18:30:31.000000 pyechorobotics-0.0.3/src/pyechorobotics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 18:30:31.000000 pyechorobotics-0.0.3/src/pyechorobotics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:00:47.143195 pyechorobotics-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 21:00:35.000000 pyechorobotics-0.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-31 21:00:47.143195 pyechorobotics-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-31 21:00:35.000000 pyechorobotics-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-31 21:00:35.000000 pyechorobotics-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-31 21:00:47.143195 pyechorobotics-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-31 21:00:35.000000 pyechorobotics-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:00:47.143195 pyechorobotics-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:00:47.143195 pyechorobotics-0.0.4/src/echoroboticsapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 21:00:35.000000 pyechorobotics-0.0.4/src/echoroboticsapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-31 21:00:35.000000 pyechorobotics-0.0.4/src/echoroboticsapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-31 21:00:35.000000 pyechorobotics-0.0.4/src/echoroboticsapi/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:00:47.143195 pyechorobotics-0.0.4/src/pyechorobotics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-31 21:00:47.000000 pyechorobotics-0.0.4/src/pyechorobotics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-31 21:00:47.000000 pyechorobotics-0.0.4/src/pyechorobotics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:00:47.000000 pyechorobotics-0.0.4/src/pyechorobotics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 21:00:47.000000 pyechorobotics-0.0.4/src/pyechorobotics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 21:00:47.000000 pyechorobotics-0.0.4/src/pyechorobotics.egg-info/top_level.txt
```

### Comparing `pyechorobotics-0.0.3/LICENSE.md` & `pyechorobotics-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyechorobotics-0.0.3/PKG-INFO` & `pyechorobotics-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyechorobotics
-Version: 0.0.3
+Version: 0.0.4
 Summary: Access API for echorobotics robot lawn mowers
 Author-email: functionpointer <suspendfunction@gmail.com>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: homepage, https://github.com/functionpointer/pyechorobotics
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.10
```

### Comparing `pyechorobotics-0.0.3/README.md` & `pyechorobotics-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyechorobotics-0.0.3/pyproject.toml` & `pyechorobotics-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyechorobotics"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = [
     "aiohttp",
     "yarl",
     "pydantic",
 ]
 readme = "README.md"
 license = {text = "GNU General Public License v3 or later (GPLv3+)"}
```

### Comparing `pyechorobotics-0.0.3/src/echoroboticsapi/api.py` & `pyechorobotics-0.0.4/src/echoroboticsapi/api.py`

 * *Files identical despite different names*

### Comparing `pyechorobotics-0.0.3/src/echoroboticsapi/models.py` & `pyechorobotics-0.0.4/src/echoroboticsapi/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     longitude: float = Field(..., alias="Longitude")
     latitude: float = Field(..., alias="Latitude")
     datetime: DateTimeISO8601 = Field(..., alias="DateTime")
 
 
 class StatusInfo(BaseModel):
     robot: RobotId = Field(..., alias="Robot")
-    status: Literal["WaitStation", "Idle", "Work"] = Field(..., alias="Status")
+    status: Literal["WaitStation", "Idle", "Work", "Charge"] = Field(..., alias="Status")
     mac_address: str = Field(..., alias="MacAddress")
     date: DateTimeISO8601 = Field(..., alias="Date")
     delta: str = Field(..., alias="Delta")
     estimated_battery_level: float = Field(..., alias="EstimatedBatteryLevel")
     position: Position = Field(..., alias="Position")
     query_time: DateTimeISO8601 = Field(..., alias="QueryTime")
     has_values: bool = Field(..., alias="HasValues")
```

### Comparing `pyechorobotics-0.0.3/src/pyechorobotics.egg-info/PKG-INFO` & `pyechorobotics-0.0.4/src/pyechorobotics.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyechorobotics
-Version: 0.0.3
+Version: 0.0.4
 Summary: Access API for echorobotics robot lawn mowers
 Author-email: functionpointer <suspendfunction@gmail.com>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: homepage, https://github.com/functionpointer/pyechorobotics
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.10
```

