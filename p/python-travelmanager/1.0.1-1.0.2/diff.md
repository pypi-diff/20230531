# Comparing `tmp/python_travelmanager-1.0.1.tar.gz` & `tmp/python_travelmanager-1.0.2.tar.gz`

## Comparing `python_travelmanager-1.0.1.tar` & `python_travelmanager-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 python_travelmanager-1.0.1/travelmanager/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 python_travelmanager-1.0.1/travelmanager/schemas.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 python_travelmanager-1.0.1/travelmanager/travelmanager_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_travelmanager-1.0.1/travelmanager/modules/__init__.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 python_travelmanager-1.0.1/travelmanager/modules/availability.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 python_travelmanager-1.0.1/travelmanager/modules/booking.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 python_travelmanager-1.0.1/travelmanager/modules/relation.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 python_travelmanager-1.0.1/travelmanager/modules/station.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 python_travelmanager-1.0.1/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 python_travelmanager-1.0.1/LICENSE
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 python_travelmanager-1.0.1/README.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 python_travelmanager-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 python_travelmanager-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 python_travelmanager-1.0.2/travelmanager/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 python_travelmanager-1.0.2/travelmanager/schemas.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 python_travelmanager-1.0.2/travelmanager/travelmanager_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_travelmanager-1.0.2/travelmanager/modules/__init__.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 python_travelmanager-1.0.2/travelmanager/modules/availability.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 python_travelmanager-1.0.2/travelmanager/modules/booking.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 python_travelmanager-1.0.2/travelmanager/modules/relation.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 python_travelmanager-1.0.2/travelmanager/modules/station.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 python_travelmanager-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 python_travelmanager-1.0.2/LICENSE
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 python_travelmanager-1.0.2/README.md
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 python_travelmanager-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 python_travelmanager-1.0.2/PKG-INFO
```

### Comparing `python_travelmanager-1.0.1/travelmanager/travelmanager_api.py` & `python_travelmanager-1.0.2/travelmanager/travelmanager_api.py`

 * *Files identical despite different names*

### Comparing `python_travelmanager-1.0.1/travelmanager/modules/booking.py` & `python_travelmanager-1.0.2/travelmanager/modules/booking.py`

 * *Files identical despite different names*

### Comparing `python_travelmanager-1.0.1/.gitignore` & `python_travelmanager-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `python_travelmanager-1.0.1/LICENSE` & `python_travelmanager-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_travelmanager-1.0.1/pyproject.toml` & `python_travelmanager-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.black]
 line-length = 80
-target-version = ["py39"]
+target-version = ["py311"]
 paths = ["travelmanager", "tests"]
 
 [tool.vulture]
 ignore_names = ["context", "*_mock"]
 make_whitelist = true
 min_confidence = 80
 paths = ["travelmanager", "tests"]
@@ -15,25 +15,24 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_travelmanager"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name="Johannes Eimer", email="johannes.eimer@jep-dev.com" },
 ]
 description = "Python TravelManager"
 readme = "README.md"
 requires-python = ">=3.9"
 license = "MIT"
 keywords = ['Python', 'TravelManager']
 dependencies = [
-    "urllib3==1.26.15",
     "requests==2.31.0",
 ]
 
 [tool.hatch.build.targets.sdist]
 include = ["travelmanager"]
 
 [tool.hatch.build.targets.wheel]
```

### Comparing `python_travelmanager-1.0.1/PKG-INFO` & `python_travelmanager-1.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: python_travelmanager
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python TravelManager
 Author-email: Johannes Eimer <johannes.eimer@jep-dev.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: Python,TravelManager
 Requires-Python: >=3.9
 Requires-Dist: requests==2.31.0
-Requires-Dist: urllib3==1.26.15
 Description-Content-Type: text/markdown
 
 # python_travelmanager
 python lib for travelmanager (https://travelmanager.de/)
 
 ## install dev
 python -m venv venv
```

