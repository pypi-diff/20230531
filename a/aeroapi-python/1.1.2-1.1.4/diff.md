# Comparing `tmp/aeroapi-python-1.1.2.tar.gz` & `tmp/aeroapi-python-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeroapi-python-1.1.2.tar", last modified: Sun May 28 17:39:40 2023, max compression
+gzip compressed data, was "aeroapi-python-1.1.4.tar", last modified: Wed May 31 06:58:14 2023, max compression
```

## Comparing `aeroapi-python-1.1.2.tar` & `aeroapi-python-1.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:39:40.181520 aeroapi-python-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-28 17:39:40.181520 aeroapi-python-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:39:40.181520 aeroapi-python-1.1.2/aeroapi_python/
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/aeroapi_python/APICaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/aeroapi_python/AeroAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/aeroapi_python/Airports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/aeroapi_python/Flights.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/aeroapi_python/History.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/aeroapi_python/Miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/aeroapi_python/Operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/aeroapi_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:39:40.181520 aeroapi-python-1.1.2/aeroapi_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-28 17:39:40.000000 aeroapi-python-1.1.2/aeroapi_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-28 17:39:40.000000 aeroapi-python-1.1.2/aeroapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 17:39:40.000000 aeroapi-python-1.1.2/aeroapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-28 17:39:40.000000 aeroapi-python-1.1.2/aeroapi_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-28 17:39:40.000000 aeroapi-python-1.1.2/aeroapi_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 17:39:40.181520 aeroapi-python-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-28 17:39:30.000000 aeroapi-python-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:58:14.750123 aeroapi-python-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-31 06:58:01.000000 aeroapi-python-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-31 06:58:14.750123 aeroapi-python-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-31 06:58:01.000000 aeroapi-python-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:58:14.750123 aeroapi-python-1.1.4/aeroapi_python/
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-31 06:58:01.000000 aeroapi-python-1.1.4/aeroapi_python/APICaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-31 06:58:01.000000 aeroapi-python-1.1.4/aeroapi_python/AeroAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-05-31 06:58:01.000000 aeroapi-python-1.1.4/aeroapi_python/Airports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-05-31 06:58:01.000000 aeroapi-python-1.1.4/aeroapi_python/Flights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-05-31 06:58:01.000000 aeroapi-python-1.1.4/aeroapi_python/History.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-31 06:58:01.000000 aeroapi-python-1.1.4/aeroapi_python/Miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-31 06:58:01.000000 aeroapi-python-1.1.4/aeroapi_python/Operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-31 06:58:01.000000 aeroapi-python-1.1.4/aeroapi_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:58:14.750123 aeroapi-python-1.1.4/aeroapi_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-31 06:58:14.000000 aeroapi-python-1.1.4/aeroapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-31 06:58:14.000000 aeroapi-python-1.1.4/aeroapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 06:58:14.000000 aeroapi-python-1.1.4/aeroapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 06:58:14.000000 aeroapi-python-1.1.4/aeroapi_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 06:58:14.000000 aeroapi-python-1.1.4/aeroapi_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 06:58:14.750123 aeroapi-python-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-31 06:58:01.000000 aeroapi-python-1.1.4/setup.py
```

### Comparing `aeroapi-python-1.1.2/LICENSE` & `aeroapi-python-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aeroapi-python-1.1.2/aeroapi_python/APICaller.py` & `aeroapi-python-1.1.4/aeroapi_python/APICaller.py`

 * *Files identical despite different names*

### Comparing `aeroapi-python-1.1.2/aeroapi_python/AeroAPI.py` & `aeroapi-python-1.1.4/aeroapi_python/AeroAPI.py`

 * *Files identical despite different names*

### Comparing `aeroapi-python-1.1.2/aeroapi_python/Airports.py` & `aeroapi-python-1.1.4/aeroapi_python/Airports.py`

 * *Files identical despite different names*

### Comparing `aeroapi-python-1.1.2/aeroapi_python/Flights.py` & `aeroapi-python-1.1.4/aeroapi_python/Flights.py`

 * *Files identical despite different names*

### Comparing `aeroapi-python-1.1.2/aeroapi_python/History.py` & `aeroapi-python-1.1.4/aeroapi_python/History.py`

 * *Files identical despite different names*

### Comparing `aeroapi-python-1.1.2/aeroapi_python/Miscellaneous.py` & `aeroapi-python-1.1.4/aeroapi_python/Miscellaneous.py`

 * *Files identical despite different names*

### Comparing `aeroapi-python-1.1.2/aeroapi_python/Operators.py` & `aeroapi-python-1.1.4/aeroapi_python/Operators.py`

 * *Files identical despite different names*

### Comparing `aeroapi-python-1.1.2/setup.py` & `aeroapi-python-1.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     requirements = f.read().splitlines()
 
 readme_path = pathlib.Path("README.md")
 requirements_path = pathlib.Path("requirements.txt")
 
 setuptools.setup(
     name="aeroapi-python",
-    version="1.1.2",
+    version="1.1.4",
     description='FlightAware AeroAPI Caller for Python',
     long_description=readme_path.read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/derens99/aeroapi-python",
     author="Deren S",
     author_email="derens9999@gmail.com",
     license="MIT",
```

