# Comparing `tmp/python_omnilogic_local-0.6.2.tar.gz` & `tmp/python_omnilogic_local-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.6.2.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.7.0.tar", max compression
```

## Comparing `python_omnilogic_local-0.6.2.tar` & `python_omnilogic_local-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1696 2023-05-30 21:36:00.476754 python_omnilogic_local-0.6.2/README.md
--rw-r--r--   0        0        0        0 2023-05-30 21:36:00.480754 python_omnilogic_local-0.6.2/pyomnilogic_local/__init__.py
--rw-r--r--   0        0        0    21453 2023-05-30 21:36:00.480754 python_omnilogic_local-0.6.2/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     3921 2023-05-30 21:36:00.480754 python_omnilogic_local-0.6.2/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0      164 2023-05-30 21:36:00.480754 python_omnilogic_local-0.6.2/pyomnilogic_local/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-30 21:36:00.480754 python_omnilogic_local-0.6.2/pyomnilogic_local/models/__init__.py
--rw-r--r--   0        0        0       51 2023-05-30 21:36:00.480754 python_omnilogic_local-0.6.2/pyomnilogic_local/models/const.py
--rw-r--r--   0        0        0     1532 2023-05-30 21:36:00.480754 python_omnilogic_local-0.6.2/pyomnilogic_local/models/filter_diagnostics.py
--rw-r--r--   0        0        0      407 2023-05-30 21:36:00.480754 python_omnilogic_local-0.6.2/pyomnilogic_local/models/leadmessage.py
--rw-r--r--   0        0        0     8352 2023-05-30 21:36:00.480754 python_omnilogic_local-0.6.2/pyomnilogic_local/models/mspconfig.py
--rw-r--r--   0        0        0     9968 2023-05-30 21:36:00.480754 python_omnilogic_local-0.6.2/pyomnilogic_local/models/telemetry.py
--rw-r--r--   0        0        0     1476 2023-05-30 21:36:00.480754 python_omnilogic_local-0.6.2/pyomnilogic_local/models/util.py
--rw-r--r--   0        0        0    10185 2023-05-30 21:36:00.480754 python_omnilogic_local-0.6.2/pyomnilogic_local/protocol.py
--rw-r--r--   0        0        0     6325 2023-05-30 21:36:00.480754 python_omnilogic_local-0.6.2/pyomnilogic_local/types.py
--rw-r--r--   0        0        0      359 2023-05-30 21:36:00.480754 python_omnilogic_local-0.6.2/pyomnilogic_local/util.py
--rw-r--r--   0        0        0     5227 2023-05-30 21:36:01.480805 python_omnilogic_local-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1696 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/__init__.py
+-rw-r--r--   0        0        0    21453 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     3921 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0      164 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/models/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/models/const.py
+-rw-r--r--   0        0        0     1532 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/models/filter_diagnostics.py
+-rw-r--r--   0        0        0      407 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/models/leadmessage.py
+-rw-r--r--   0        0        0     8413 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/models/mspconfig.py
+-rw-r--r--   0        0        0     9968 2023-05-31 03:23:18.060843 python_omnilogic_local-0.7.0/pyomnilogic_local/models/telemetry.py
+-rw-r--r--   0        0        0     1476 2023-05-31 03:23:18.064843 python_omnilogic_local-0.7.0/pyomnilogic_local/models/util.py
+-rw-r--r--   0        0        0    10185 2023-05-31 03:23:18.064843 python_omnilogic_local-0.7.0/pyomnilogic_local/protocol.py
+-rw-r--r--   0        0        0     6325 2023-05-31 03:23:18.064843 python_omnilogic_local-0.7.0/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0      359 2023-05-31 03:23:18.064843 python_omnilogic_local-0.7.0/pyomnilogic_local/util.py
+-rw-r--r--   0        0        0     5227 2023-05-31 03:23:18.980826 python_omnilogic_local-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.7.0/PKG-INFO
```

### Comparing `python_omnilogic_local-0.6.2/README.md` & `python_omnilogic_local-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.6.2/pyomnilogic_local/api.py` & `python_omnilogic_local-0.7.0/pyomnilogic_local/api.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.6.2/pyomnilogic_local/cli.py` & `python_omnilogic_local-0.7.0/pyomnilogic_local/cli.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.6.2/pyomnilogic_local/models/filter_diagnostics.py` & `python_omnilogic_local-0.7.0/pyomnilogic_local/models/filter_diagnostics.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.6.2/pyomnilogic_local/models/mspconfig.py` & `python_omnilogic_local-0.7.0/pyomnilogic_local/models/mspconfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,23 +146,24 @@
 
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self.effects = list(ColorLogicShow) if self.v2_active == "yes" else [show for show in ColorLogicShow if show.value <= 16]
 
 
 class MSPBoW(OmniBase):
-    _sub_devices = {"filter", "relay", "heater", "sensor", "colorlogic_light"}
+    _sub_devices = {"filter", "relay", "heater", "sensor", "colorlogic_light", "pump"}
 
     omni_type: OmniType = OmniType.BOW
     type: BodyOfWaterType | str = Field(alias="Type")
     filter: list[MSPFilter] | None = Field(alias="Filter")
     relay: list[MSPRelay] | None = Field(alias="Relay")
     heater: MSPVirtualHeater | None = Field(alias="Heater")
     sensor: list[MSPSensor] | None = Field(alias="Sensor")
     colorlogic_light: list[MSPColorLogicLight] | None = Field(alias="ColorLogic-Light")
+    pump: list[MSPPump] | None = Field(alias="Pump")
 
     # We override the __init__ here so that we can trigger the propagation of the bow_id down to all of it's sub devices after the bow
     # itself is initialized
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self.propagate_bow_id(self.system_id)
```

### Comparing `python_omnilogic_local-0.6.2/pyomnilogic_local/models/telemetry.py` & `python_omnilogic_local-0.7.0/pyomnilogic_local/models/telemetry.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.6.2/pyomnilogic_local/models/util.py` & `python_omnilogic_local-0.7.0/pyomnilogic_local/models/util.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.6.2/pyomnilogic_local/protocol.py` & `python_omnilogic_local-0.7.0/pyomnilogic_local/protocol.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.6.2/pyomnilogic_local/types.py` & `python_omnilogic_local-0.7.0/pyomnilogic_local/types.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.6.2/pyproject.toml` & `python_omnilogic_local-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-omnilogic-local"
-version = "0.6.2"
+version = "0.7.0"
 description = "A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API"
 authors = ["cryptk <cryptk@users.noreply.github.com>", "djtimca", "garionphx"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cryptk/python-omnilogic-local"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `python_omnilogic_local-0.6.2/PKG-INFO` & `python_omnilogic_local-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.6.2
+Version: 0.7.0
 Summary: A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API
 Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0
 Author: cryptk
 Author-email: cryptk@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.6.2 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.7.0 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
 cryptk@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
```

