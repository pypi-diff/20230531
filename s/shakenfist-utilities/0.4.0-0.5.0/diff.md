# Comparing `tmp/shakenfist-utilities-0.4.0.tar.gz` & `tmp/shakenfist-utilities-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shakenfist-utilities-0.4.0.tar", last modified: Sat Sep 24 03:02:16 2022, max compression
+gzip compressed data, was "shakenfist-utilities-0.5.0.tar", last modified: Wed May 31 09:25:03 2023, max compression
```

## Comparing `shakenfist-utilities-0.4.0.tar` & `shakenfist-utilities-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-09-24 03:02:16.686316 shakenfist-utilities-0.4.0/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       34 2022-09-24 03:02:16.000000 shakenfist-utilities-0.4.0/AUTHORS
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2022-08-06 06:52:50.000000 shakenfist-utilities-0.4.0/LICENSE
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      877 2022-09-24 03:02:16.686316 shakenfist-utilities-0.4.0/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      168 2022-08-06 06:52:50.000000 shakenfist-utilities-0.4.0/README.md
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      866 2022-08-06 06:52:50.000000 shakenfist-utilities-0.4.0/release.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       82 2022-08-07 23:15:20.000000 shakenfist-utilities-0.4.0/requirements.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      652 2022-09-24 03:02:16.686316 shakenfist-utilities-0.4.0/setup.cfg
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      964 2022-08-06 06:52:50.000000 shakenfist-utilities-0.4.0/setup.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-09-24 03:02:16.682317 shakenfist-utilities-0.4.0/shakenfist_utilities/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-08-06 06:52:50.000000 shakenfist-utilities-0.4.0/shakenfist_utilities/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     5009 2022-08-08 05:08:58.000000 shakenfist-utilities-0.4.0/shakenfist_utilities/api.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     6429 2022-09-24 03:02:03.000000 shakenfist-utilities-0.4.0/shakenfist_utilities/logs.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      187 2022-08-06 06:52:50.000000 shakenfist-utilities-0.4.0/shakenfist_utilities/random.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-09-24 03:02:16.686316 shakenfist-utilities-0.4.0/shakenfist_utilities/tests/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-08-06 06:52:50.000000 shakenfist-utilities-0.4.0/shakenfist_utilities/tests/__init__.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-09-24 03:02:16.686316 shakenfist-utilities-0.4.0/shakenfist_utilities.egg-info/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      877 2022-09-24 03:02:16.000000 shakenfist-utilities-0.4.0/shakenfist_utilities.egg-info/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      583 2022-09-24 03:02:16.000000 shakenfist-utilities-0.4.0/shakenfist_utilities.egg-info/SOURCES.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2022-09-24 03:02:16.000000 shakenfist-utilities-0.4.0/shakenfist_utilities.egg-info/dependency_links.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2022-09-24 03:02:16.000000 shakenfist-utilities-0.4.0/shakenfist_utilities.egg-info/not-zip-safe
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       46 2022-09-24 03:02:16.000000 shakenfist-utilities-0.4.0/shakenfist_utilities.egg-info/pbr.json
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       39 2022-09-24 03:02:16.000000 shakenfist-utilities-0.4.0/shakenfist_utilities.egg-info/requires.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       21 2022-09-24 03:02:16.000000 shakenfist-utilities-0.4.0/shakenfist_utilities.egg-info/top_level.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      138 2022-08-06 06:52:50.000000 shakenfist-utilities-0.4.0/test-requirements.txt
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-09-24 03:02:16.686316 shakenfist-utilities-0.4.0/tools/
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      580 2022-08-06 06:52:50.000000 shakenfist-utilities-0.4.0/tools/flake8wrap.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      624 2022-08-06 06:52:50.000000 shakenfist-utilities-0.4.0/tox.ini
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 09:25:03.750668 shakenfist-utilities-0.5.0/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       34 2023-05-31 09:25:03.000000 shakenfist-utilities-0.5.0/AUTHORS
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/LICENSE
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      877 2023-05-31 09:25:03.750668 shakenfist-utilities-0.5.0/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      168 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/README.md
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      866 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/release.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       82 2022-08-07 23:15:20.000000 shakenfist-utilities-0.5.0/requirements.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      652 2023-05-31 09:25:03.754668 shakenfist-utilities-0.5.0/setup.cfg
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      964 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/setup.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 09:25:03.750668 shakenfist-utilities-0.5.0/shakenfist_utilities/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/shakenfist_utilities/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     5009 2022-08-08 05:08:58.000000 shakenfist-utilities-0.5.0/shakenfist_utilities/api.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     6467 2023-05-31 09:24:40.000000 shakenfist-utilities-0.5.0/shakenfist_utilities/logs.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      187 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/shakenfist_utilities/random.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 09:25:03.750668 shakenfist-utilities-0.5.0/shakenfist_utilities/tests/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/shakenfist_utilities/tests/__init__.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 09:25:03.750668 shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      877 2023-05-31 09:25:03.000000 shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      583 2023-05-31 09:25:03.000000 shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/SOURCES.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-05-31 09:25:03.000000 shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/dependency_links.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-05-31 09:25:03.000000 shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/not-zip-safe
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       46 2023-05-31 09:25:03.000000 shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/pbr.json
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       39 2023-05-31 09:25:03.000000 shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/requires.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       21 2023-05-31 09:25:03.000000 shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/top_level.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      138 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/test-requirements.txt
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 09:25:03.750668 shakenfist-utilities-0.5.0/tools/
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      580 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/tools/flake8wrap.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      624 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/tox.ini
```

### Comparing `shakenfist-utilities-0.4.0/LICENSE` & `shakenfist-utilities-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shakenfist-utilities-0.4.0/PKG-INFO` & `shakenfist-utilities-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakenfist-utilities
-Version: 0.4.0
+Version: 0.5.0
 Summary: Shaken Fist utility libraries
 Home-page: https://github.com/shakenfist/library-utilities
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: # Shaken Fist Utilities
```

### Comparing `shakenfist-utilities-0.4.0/release.sh` & `shakenfist-utilities-0.5.0/release.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-utilities-0.4.0/setup.cfg` & `shakenfist-utilities-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `shakenfist-utilities-0.4.0/setup.py` & `shakenfist-utilities-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `shakenfist-utilities-0.4.0/shakenfist_utilities/api.py` & `shakenfist-utilities-0.5.0/shakenfist_utilities/api.py`

 * *Files identical despite different names*

### Comparing `shakenfist-utilities-0.4.0/shakenfist_utilities/logs.py` & `shakenfist-utilities-0.5.0/shakenfist_utilities/logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,16 @@
         return self.with_fields(fields)
 
     def with_fields(self, fields=None):
         extra = copy.deepcopy(self._extra)
         fields = self._normalize(fields)
 
         # Handle "special fields" which might be internal objects
-        for key in ['artifact', 'blob', 'instance', 'network', 'networkinterface', 'node']:
+        for key in ['agentoperation', 'artifact', 'blob', 'instance', 'network',
+                    'networkinterface', 'node']:
             if key in fields:
                 value = fields[key]
                 if value and not isinstance(value, str):
                     fields[key] = value.uuid
 
         extra.update(fields)
         return SyslogAdapter(self._logger, extra, self._prefix)
```

### Comparing `shakenfist-utilities-0.4.0/shakenfist_utilities.egg-info/PKG-INFO` & `shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakenfist-utilities
-Version: 0.4.0
+Version: 0.5.0
 Summary: Shaken Fist utility libraries
 Home-page: https://github.com/shakenfist/library-utilities
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: # Shaken Fist Utilities
```

### Comparing `shakenfist-utilities-0.4.0/shakenfist_utilities.egg-info/SOURCES.txt` & `shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shakenfist-utilities-0.4.0/tools/flake8wrap.sh` & `shakenfist-utilities-0.5.0/tools/flake8wrap.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-utilities-0.4.0/tox.ini` & `shakenfist-utilities-0.5.0/tox.ini`

 * *Files identical despite different names*

