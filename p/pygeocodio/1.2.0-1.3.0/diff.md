# Comparing `tmp/pygeocodio-1.2.0.tar.gz` & `tmp/pygeocodio-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeocodio-1.2.0.tar", last modified: Wed Mar 22 15:00:26 2023, max compression
+gzip compressed data, was "pygeocodio-1.3.0.tar", last modified: Wed May 31 14:31:35 2023, max compression
```

## Comparing `pygeocodio-1.2.0.tar` & `pygeocodio-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:26.703784 pygeocodio-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-22 15:00:07.000000 pygeocodio-1.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-03-22 15:00:07.000000 pygeocodio-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-03-22 15:00:07.000000 pygeocodio-1.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-03-22 15:00:07.000000 pygeocodio-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-22 15:00:07.000000 pygeocodio-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-03-22 15:00:26.703784 pygeocodio-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-03-22 15:00:07.000000 pygeocodio-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 15:00:26.703784 pygeocodio-1.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1617 2023-03-22 15:00:07.000000 pygeocodio-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:26.699784 pygeocodio-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:26.703784 pygeocodio-1.2.0/src/geocodio/
--rwxr-xr-x   0 runner    (1001) docker     (123)      443 2023-03-22 15:00:07.000000 pygeocodio-1.2.0/src/geocodio/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10624 2023-03-22 15:00:07.000000 pygeocodio-1.2.0/src/geocodio/client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6771 2023-03-22 15:00:07.000000 pygeocodio-1.2.0/src/geocodio/data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      438 2023-03-22 15:00:07.000000 pygeocodio-1.2.0/src/geocodio/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:26.703784 pygeocodio-1.2.0/src/pygeocodio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-03-22 15:00:26.000000 pygeocodio-1.2.0/src/pygeocodio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-22 15:00:26.000000 pygeocodio-1.2.0/src/pygeocodio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 15:00:26.000000 pygeocodio-1.2.0/src/pygeocodio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 15:00:26.000000 pygeocodio-1.2.0/src/pygeocodio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-22 15:00:26.000000 pygeocodio-1.2.0/src/pygeocodio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-22 15:00:26.000000 pygeocodio-1.2.0/src/pygeocodio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:31:35.035903 pygeocodio-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-31 14:31:35.035903 pygeocodio-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:31:35.035903 pygeocodio-1.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1629 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:31:35.035903 pygeocodio-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:31:35.035903 pygeocodio-1.3.0/src/geocodio/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      443 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/src/geocodio/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10734 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/src/geocodio/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6771 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/src/geocodio/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      438 2023-05-31 14:31:22.000000 pygeocodio-1.3.0/src/geocodio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:31:35.035903 pygeocodio-1.3.0/src/pygeocodio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-31 14:31:34.000000 pygeocodio-1.3.0/src/pygeocodio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-31 14:31:35.000000 pygeocodio-1.3.0/src/pygeocodio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:31:34.000000 pygeocodio-1.3.0/src/pygeocodio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:31:34.000000 pygeocodio-1.3.0/src/pygeocodio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 14:31:34.000000 pygeocodio-1.3.0/src/pygeocodio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 14:31:34.000000 pygeocodio-1.3.0/src/pygeocodio.egg-info/top_level.txt
```

### Comparing `pygeocodio-1.2.0/AUTHORS.rst` & `pygeocodio-1.3.0/AUTHORS.rst`

 * *Files 5% similar despite different names*

```diff
@@ -19,7 +19,8 @@
 * `Pedro Machado <https://github.com/pedromachados>`_
 * `Josh Geller <https://github.com/joshgeller>`_
 * `Shea Parkes <https://github.com/shea-parkes>`_
 * `David Malakh <https://github.com/Unix-Code>`_
 * `Andrew Harrision <https://github.com/cyranix>`_
 * `Franklin Liu <https://github.com/liufran1>`_
 * `Aviv Nitsan <https://github.com/aviv>`_
+* `Bruno Gonzalez <https://github.com/bruno-uy>`_
```

### Comparing `pygeocodio-1.2.0/CONTRIBUTING.rst` & `pygeocodio-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pygeocodio-1.2.0/HISTORY.rst` & `pygeocodio-1.3.0/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .. :changelog:
 
 History
 -------
 
+1.3.0 (2023-05-31)
++++++++++++++++++++
+
+* Adds support for the 'limit' parameter to limit results (thanks bruno-uy!)
+
 1.2.0 (2023-03-21)
 +++++++++++++++++++
 
 * Adds custom_base_domain support (thanks MiniCodeMonkey!)
 * Drops Python 3.6 support
 * Adds official Python 3.11 support
```

### Comparing `pygeocodio-1.2.0/LICENSE` & `pygeocodio-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeocodio-1.2.0/PKG-INFO` & `pygeocodio-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pygeocodio
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python wrapper for Geocod.io API
 Home-page: https://github.com/bennylope/pygeocodio
 Author: Ben Lopatin
 Author-email: ben@benlopatin.com
 License: BSD
 Keywords: geocodio
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -235,14 +235,19 @@
 
 
 
 
 History
 -------
 
+1.3.0 (2023-05-31)
++++++++++++++++++++
+
+* Adds support for the 'limit' parameter to limit results (thanks bruno-uy!)
+
 1.2.0 (2023-03-21)
 +++++++++++++++++++
 
 * Adds custom_base_domain support (thanks MiniCodeMonkey!)
 * Drops Python 3.6 support
 * Adds official Python 3.11 support
```

### Comparing `pygeocodio-1.2.0/README.rst` & `pygeocodio-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `pygeocodio-1.2.0/setup.py` & `pygeocodio-1.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     package_dir={"": "src"},
     include_package_data=True,
     install_requires=["requests>=1.0.0"],
     license="BSD",
     zip_safe=False,
     keywords="geocodio",
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `pygeocodio-1.2.0/src/geocodio/client.py` & `pygeocodio-1.3.0/src/geocodio/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,18 +134,19 @@
 
     def batch_geocode(self, addresses, **kwargs):
         """
         Returns an Address dictionary with the components of the queried
         address. Accepts either a list or dictionary of addresses
         """
         fields = ",".join(kwargs.pop("fields", []))
+        limit = kwargs.pop("limit", 0)
         response = self._req(
             "post",
             verb="geocode",
-            params={"fields": fields},
+            params={"fields": fields, "limit": limit},
             data=json.dumps(addresses),
         )
         if response.status_code != 200:
             return error_response(response)
 
         results = response.json()["results"]
         if isinstance(results, list):
@@ -206,15 +207,16 @@
                 },
                 "accuracy": 0.8
                 }
             ]
         }
         """
         fields = ",".join(kwargs.pop("fields", []))
-        params = {"fields": fields}
+        limit = kwargs.pop("limit", 0)
+        params = {"fields": fields, "limit": limit}
         if address is not None:
             params["q"] = address
         else:
             params.update(components)
         response = self._req(verb="geocode", params=params)
         if response.status_code != 200:
             return error_response(response)
```

### Comparing `pygeocodio-1.2.0/src/geocodio/data.py` & `pygeocodio-1.3.0/src/geocodio/data.py`

 * *Files identical despite different names*

### Comparing `pygeocodio-1.2.0/src/pygeocodio.egg-info/PKG-INFO` & `pygeocodio-1.3.0/src/pygeocodio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pygeocodio
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python wrapper for Geocod.io API
 Home-page: https://github.com/bennylope/pygeocodio
 Author: Ben Lopatin
 Author-email: ben@benlopatin.com
 License: BSD
 Keywords: geocodio
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -235,14 +235,19 @@
 
 
 
 
 History
 -------
 
+1.3.0 (2023-05-31)
++++++++++++++++++++
+
+* Adds support for the 'limit' parameter to limit results (thanks bruno-uy!)
+
 1.2.0 (2023-03-21)
 +++++++++++++++++++
 
 * Adds custom_base_domain support (thanks MiniCodeMonkey!)
 * Drops Python 3.6 support
 * Adds official Python 3.11 support
```

