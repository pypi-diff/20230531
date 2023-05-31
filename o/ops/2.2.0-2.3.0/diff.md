# Comparing `tmp/ops-2.2.0.tar.gz` & `tmp/ops-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops-2.2.0.tar", last modified: Mon Mar 27 23:39:09 2023, max compression
+gzip compressed data, was "ops-2.3.0.tar", last modified: Wed May 31 00:33:43 2023, max compression
```

## Comparing `ops-2.2.0.tar` & `ops-2.3.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:39:09.902178 ops-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-27 23:39:07.000000 ops-2.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-03-27 23:39:09.902178 ops-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-03-27 23:39:07.000000 ops-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:39:09.898178 ops-2.2.0/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-03-27 23:39:07.000000 ops-2.2.0/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:39:09.902178 ops-2.2.0/ops/_private/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 23:39:07.000000 ops-2.2.0/ops/_private/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-03-27 23:39:07.000000 ops-2.2.0/ops/_private/timeconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-27 23:39:07.000000 ops-2.2.0/ops/_private/yaml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    54095 2023-03-27 23:39:07.000000 ops-2.2.0/ops/charm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    53402 2023-03-27 23:39:07.000000 ops-2.2.0/ops/framework.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4775 2023-03-27 23:39:07.000000 ops-2.2.0/ops/jujuversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:39:09.902178 ops-2.2.0/ops/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     9839 2023-03-27 23:39:07.000000 ops-2.2.0/ops/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-03-27 23:39:07.000000 ops-2.2.0/ops/log.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17905 2023-03-27 23:39:07.000000 ops-2.2.0/ops/main.py
--rw-r--r--   0 runner    (1001) docker     (123)   124923 2023-03-27 23:39:07.000000 ops-2.2.0/ops/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    98073 2023-03-27 23:39:07.000000 ops-2.2.0/ops/pebble.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 23:39:07.000000 ops-2.2.0/ops/py.typed
--rwxr-xr-x   0 runner    (1001) docker     (123)    15197 2023-03-27 23:39:07.000000 ops-2.2.0/ops/storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   128167 2023-03-27 23:39:07.000000 ops-2.2.0/ops/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-27 23:39:09.000000 ops-2.2.0/ops/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:39:09.898178 ops-2.2.0/ops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-03-27 23:39:09.000000 ops-2.2.0/ops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-27 23:39:09.000000 ops-2.2.0/ops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 23:39:09.000000 ops-2.2.0/ops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-27 23:39:09.000000 ops-2.2.0/ops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-27 23:39:09.000000 ops-2.2.0/ops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-27 23:39:07.000000 ops-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 23:39:09.902178 ops-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-03-27 23:39:07.000000 ops-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:39:09.902178 ops-2.2.0/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)    21858 2023-03-27 23:39:07.000000 ops-2.2.0/test/test_charm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    64425 2023-03-27 23:39:07.000000 ops-2.2.0/test/test_framework.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4658 2023-03-27 23:39:07.000000 ops-2.2.0/test/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-03-27 23:39:07.000000 ops-2.2.0/test/test_infra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6782 2023-03-27 23:39:07.000000 ops-2.2.0/test/test_jujuversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    22453 2023-03-27 23:39:07.000000 ops-2.2.0/test/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-03-27 23:39:07.000000 ops-2.2.0/test/test_log.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    46889 2023-03-27 23:39:07.000000 ops-2.2.0/test/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   129220 2023-03-27 23:39:07.000000 ops-2.2.0/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   125097 2023-03-27 23:39:07.000000 ops-2.2.0/test/test_pebble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-03-27 23:39:07.000000 ops-2.2.0/test/test_private.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15155 2023-03-27 23:39:07.000000 ops-2.2.0/test/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)   191348 2023-03-27 23:39:07.000000 ops-2.2.0/test/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:33:43.160119 ops-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-31 00:33:40.000000 ops-2.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-05-31 00:33:43.160119 ops-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-05-31 00:33:40.000000 ops-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:33:43.156119 ops-2.3.0/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-31 00:33:40.000000 ops-2.3.0/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:33:43.156119 ops-2.3.0/ops/_private/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:33:40.000000 ops-2.3.0/ops/_private/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-31 00:33:40.000000 ops-2.3.0/ops/_private/timeconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-31 00:33:40.000000 ops-2.3.0/ops/_private/yaml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54095 2023-05-31 00:33:40.000000 ops-2.3.0/ops/charm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    53402 2023-05-31 00:33:40.000000 ops-2.3.0/ops/framework.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4775 2023-05-31 00:33:40.000000 ops-2.3.0/ops/jujuversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:33:43.156119 ops-2.3.0/ops/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     9839 2023-05-31 00:33:40.000000 ops-2.3.0/ops/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-31 00:33:40.000000 ops-2.3.0/ops/log.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17905 2023-05-31 00:33:40.000000 ops-2.3.0/ops/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125257 2023-05-31 00:33:40.000000 ops-2.3.0/ops/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98073 2023-05-31 00:33:40.000000 ops-2.3.0/ops/pebble.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:33:40.000000 ops-2.3.0/ops/py.typed
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15197 2023-05-31 00:33:40.000000 ops-2.3.0/ops/storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   128227 2023-05-31 00:33:40.000000 ops-2.3.0/ops/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-31 00:33:42.000000 ops-2.3.0/ops/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:33:43.156119 ops-2.3.0/ops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-05-31 00:33:43.000000 ops-2.3.0/ops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-31 00:33:43.000000 ops-2.3.0/ops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:33:43.000000 ops-2.3.0/ops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-31 00:33:43.000000 ops-2.3.0/ops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-31 00:33:43.000000 ops-2.3.0/ops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-31 00:33:40.000000 ops-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 00:33:43.160119 ops-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-31 00:33:40.000000 ops-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:33:43.160119 ops-2.3.0/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21858 2023-05-31 00:33:40.000000 ops-2.3.0/test/test_charm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    64425 2023-05-31 00:33:40.000000 ops-2.3.0/test/test_framework.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4658 2023-05-31 00:33:40.000000 ops-2.3.0/test/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-31 00:33:40.000000 ops-2.3.0/test/test_infra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6782 2023-05-31 00:33:40.000000 ops-2.3.0/test/test_jujuversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22453 2023-05-31 00:33:40.000000 ops-2.3.0/test/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-31 00:33:40.000000 ops-2.3.0/test/test_log.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    46889 2023-05-31 00:33:40.000000 ops-2.3.0/test/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   130069 2023-05-31 00:33:40.000000 ops-2.3.0/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125097 2023-05-31 00:33:40.000000 ops-2.3.0/test/test_pebble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-31 00:33:40.000000 ops-2.3.0/test/test_private.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15155 2023-05-31 00:33:40.000000 ops-2.3.0/test/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)   191372 2023-05-31 00:33:40.000000 ops-2.3.0/test/test_testing.py
```

### Comparing `ops-2.2.0/LICENSE.txt` & `ops-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/PKG-INFO` & `ops-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops
-Version: 2.2.0
+Version: 2.3.0
 Summary: The Python library behind great charms
 Home-page: https://github.com/canonical/operator
 Author: The Charmcraft team at Canonical Ltd.
 Author-email: charmcraft@lists.launchpad.net
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ops-2.2.0/README.md` & `ops-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/ops/__init__.py` & `ops-2.3.0/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/ops/_private/timeconv.py` & `ops-2.3.0/ops/_private/timeconv.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/ops/_private/yaml.py` & `ops-2.3.0/ops/_private/yaml.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/ops/charm.py` & `ops-2.3.0/ops/charm.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/ops/framework.py` & `ops-2.3.0/ops/framework.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/ops/jujuversion.py` & `ops-2.3.0/ops/jujuversion.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/ops/lib/__init__.py` & `ops-2.3.0/ops/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/ops/log.py` & `ops-2.3.0/ops/log.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/ops/main.py` & `ops-2.3.0/ops/main.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/ops/model.py` & `ops-2.3.0/ops/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -2927,24 +2927,29 @@
     def get_pebble(self, socket_path: str) -> 'Client':
         """Create a pebble.Client instance from given socket path."""
         return pebble.Client(socket_path=socket_path)
 
     def planned_units(self) -> int:
         """Count of "planned" units that will run this application.
 
-        Includes the current unit in the count.
+        This will include the current unit, any units that are alive, units that are in the process
+        of being started, but will not include units that are being shut down.
 
         """
         # The goal-state tool will return the information that we need. Goal state as a general
         # concept is being deprecated, however, in favor of approaches such as the one that we use
         # here.
         app_state = self._run('goal-state', return_output=True, use_json=True)
-        app_state = typing.cast(Dict[str, List[str]], app_state)
+        app_state = typing.cast(Dict[str, Dict[str, Any]], app_state)
+
         # Planned units can be zero. We don't need to do error checking here.
-        return len(app_state.get('units', []))
+        # But we need to filter out dying units as they may be reported before being deleted
+        units = app_state.get('units', {})
+        num_alive = sum(1 for unit in units.values() if unit['status'] != 'dying')
+        return num_alive
 
     def update_relation_data(self, relation_id: int, _entity: 'UnitOrApplication',
                              key: str, value: str):
         self.relation_set(relation_id, key, value, isinstance(_entity, Application))
 
     def secret_get(self, *,
                    id: Optional[str] = None,
```

### Comparing `ops-2.2.0/ops/pebble.py` & `ops-2.3.0/ops/pebble.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/ops/storage.py` & `ops-2.3.0/ops/storage.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/ops/testing.py` & `ops-2.3.0/ops/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -2533,15 +2533,15 @@
             raise pebble.PathError(
                 'generic-file-error', 'cannot remove non-empty directory without recursive=True')
         self._fs.delete_path(path)
 
     def exec(self, command, **kwargs):  # type:ignore
         raise NotImplementedError(self.exec)  # type:ignore
 
-    def send_signal(self, sig: Union[int, str], *service_names: str):
+    def send_signal(self, sig: Union[int, str], service_names: Iterable[str]):
         if not service_names:
             raise TypeError('send_signal expected at least 1 service name, got 0')
         self._check_connection()
 
         # Convert signal to str
         if isinstance(sig, int):
             sig = signal.Signals(sig).name
@@ -2560,15 +2560,16 @@
                 )
 
         # Check if signal name is valid
         try:
             signal.Signals[sig]
         except KeyError:
             # conform with the real pebble api
-            message = f'cannot send signal to "{service_names[0]}": invalid signal name "{sig}"'
+            first_service = next(iter(service_names))
+            message = f'cannot send signal to "{first_service}": invalid signal name "{sig}"'
             body = {'type': 'error', 'status-code': 500, 'status': 'Internal Server Error',
                     'result': {'message': message}}
             raise pebble.APIError(
                 body=body,
                 code=500,
                 status='Internal Server Error',
                 message=message)
```

### Comparing `ops-2.2.0/ops.egg-info/PKG-INFO` & `ops-2.3.0/ops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops
-Version: 2.2.0
+Version: 2.3.0
 Summary: The Python library behind great charms
 Home-page: https://github.com/canonical/operator
 Author: The Charmcraft team at Canonical Ltd.
 Author-email: charmcraft@lists.launchpad.net
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ops-2.2.0/ops.egg-info/SOURCES.txt` & `ops-2.3.0/ops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/pyproject.toml` & `ops-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/setup.py` & `ops-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/test/test_charm.py` & `ops-2.3.0/test/test_charm.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/test/test_framework.py` & `ops-2.3.0/test/test_framework.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/test/test_helpers.py` & `ops-2.3.0/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/test/test_infra.py` & `ops-2.3.0/test/test_infra.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/test/test_jujuversion.py` & `ops-2.3.0/test/test_jujuversion.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/test/test_lib.py` & `ops-2.3.0/test/test_lib.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/test/test_log.py` & `ops-2.3.0/test/test_log.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/test/test_main.py` & `ops-2.3.0/test/test_main.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/test/test_model.py` & `ops-2.3.0/test/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -6718,1360 +6718,1413 @@
 0001a3d0: 655f 7363 7269 7074 5f63 616c 6c73 2873  e_script_calls(s
 0001a3e0: 656c 662c 2063 6c65 6172 3d54 7275 6529  elf, clear=True)
 0001a3f0: 2c20 5b0a 2020 2020 2020 2020 2020 2020  , [.            
 0001a400: 5b27 7265 6c61 7469 6f6e 2d6c 6973 7427  ['relation-list'
 0001a410: 2c20 272d 7227 2c20 2736 272c 2027 2d2d  , '-r', '6', '--
 0001a420: 6170 7027 2c20 272d 2d66 6f72 6d61 743d  app', '--format=
 0001a430: 6a73 6f6e 275d 2c0a 2020 2020 2020 2020  json'],.        
-0001a440: 5d29 0a0a 0a63 6c61 7373 2054 6573 744c  ])...class TestL
-0001a450: 617a 794d 6170 7069 6e67 2875 6e69 7474  azyMapping(unitt
-0001a460: 6573 742e 5465 7374 4361 7365 293a 0a0a  est.TestCase):..
-0001a470: 2020 2020 6465 6620 7465 7374 5f69 6e76      def test_inv
-0001a480: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-0001a490: 2020 2020 2020 206c 6f61 6465 6420 3d20         loaded = 
-0001a4a0: 5b5d 0a0a 2020 2020 2020 2020 636c 6173  []..        clas
-0001a4b0: 7320 4d79 4c61 7a79 4d61 7028 6f70 732e  s MyLazyMap(ops.
-0001a4c0: 4c61 7a79 4d61 7070 696e 6729 3a0a 2020  LazyMapping):.  
-0001a4d0: 2020 2020 2020 2020 2020 6465 6620 5f6c            def _l
-0001a4e0: 6f61 6428 7365 6c66 293a 0a20 2020 2020  oad(self):.     
-0001a4f0: 2020 2020 2020 2020 2020 206c 6f61 6465             loade
-0001a500: 642e 6170 7065 6e64 2831 290a 2020 2020  d.append(1).    
-0001a510: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001a520: 726e 207b 2766 6f6f 273a 2027 6261 7227  rn {'foo': 'bar'
-0001a530: 7d0a 0a20 2020 2020 2020 206d 6170 203d  }..        map =
-0001a540: 204d 794c 617a 794d 6170 2829 0a20 2020   MyLazyMap().   
-0001a550: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0001a560: 4571 7561 6c28 6d61 705b 2766 6f6f 275d  Equal(map['foo']
-0001a570: 2c20 2762 6172 2729 0a20 2020 2020 2020  , 'bar').       
-0001a580: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0001a590: 6c28 6c6f 6164 6564 2c20 5b31 5d29 0a20  l(loaded, [1]). 
-0001a5a0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0001a5b0: 7274 4571 7561 6c28 6d61 705b 2766 6f6f  rtEqual(map['foo
-0001a5c0: 275d 2c20 2762 6172 2729 0a20 2020 2020  '], 'bar').     
-0001a5d0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0001a5e0: 7561 6c28 6c6f 6164 6564 2c20 5b31 5d29  ual(loaded, [1])
-0001a5f0: 0a20 2020 2020 2020 206d 6170 2e5f 696e  .        map._in
-0001a600: 7661 6c69 6461 7465 2829 0a20 2020 2020  validate().     
-0001a610: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0001a620: 7561 6c28 6d61 705b 2766 6f6f 275d 2c20  ual(map['foo'], 
-0001a630: 2762 6172 2729 0a20 2020 2020 2020 2073  'bar').        s
-0001a640: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0001a650: 6c6f 6164 6564 2c20 5b31 2c20 315d 290a  loaded, [1, 1]).
-0001a660: 0a0a 636c 6173 7320 5465 7374 5365 6372  ..class TestSecr
-0001a670: 6574 7328 756e 6974 7465 7374 2e54 6573  ets(unittest.Tes
-0001a680: 7443 6173 6529 3a0a 2020 2020 6465 6620  tCase):.    def 
-0001a690: 7365 7455 7028 7365 6c66 293a 0a20 2020  setUp(self):.   
-0001a6a0: 2020 2020 2073 656c 662e 6d6f 6465 6c20       self.model 
-0001a6b0: 3d20 6f70 732e 4d6f 6465 6c28 6f70 732e  = ops.Model(ops.
-0001a6c0: 4368 6172 6d4d 6574 6128 292c 205f 4d6f  CharmMeta(), _Mo
-0001a6d0: 6465 6c42 6163 6b65 6e64 2827 6d79 6170  delBackend('myap
-0001a6e0: 702f 3027 2929 0a20 2020 2020 2020 2073  p/0')).        s
-0001a6f0: 656c 662e 6170 7020 3d20 7365 6c66 2e6d  elf.app = self.m
-0001a700: 6f64 656c 2e61 7070 0a20 2020 2020 2020  odel.app.       
-0001a710: 2073 656c 662e 756e 6974 203d 2073 656c   self.unit = sel
-0001a720: 662e 6d6f 6465 6c2e 756e 6974 0a0a 2020  f.model.unit..  
-0001a730: 2020 6465 6620 7465 7374 5f61 7070 5f61    def test_app_a
-0001a740: 6464 5f73 6563 7265 745f 7369 6d70 6c65  dd_secret_simple
-0001a750: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0001a760: 6661 6b65 5f73 6372 6970 7428 7365 6c66  fake_script(self
-0001a770: 2c20 2773 6563 7265 742d 6164 6427 2c20  , 'secret-add', 
-0001a780: 2765 6368 6f20 7365 6372 6574 3a31 3233  'echo secret:123
-0001a790: 2729 0a0a 2020 2020 2020 2020 7365 6372  ')..        secr
-0001a7a0: 6574 203d 2073 656c 662e 6170 702e 6164  et = self.app.ad
-0001a7b0: 645f 7365 6372 6574 287b 2766 6f6f 273a  d_secret({'foo':
-0001a7c0: 2027 7827 7d29 0a20 2020 2020 2020 2073   'x'}).        s
-0001a7d0: 656c 662e 6173 7365 7274 4973 496e 7374  elf.assertIsInst
-0001a7e0: 616e 6365 2873 6563 7265 742c 206f 7073  ance(secret, ops
-0001a7f0: 2e53 6563 7265 7429 0a20 2020 2020 2020  .Secret).       
-0001a800: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0001a810: 6c28 7365 6372 6574 2e69 642c 2027 7365  l(secret.id, 'se
-0001a820: 6372 6574 3a31 3233 2729 0a20 2020 2020  cret:123').     
-0001a830: 2020 2073 656c 662e 6173 7365 7274 4973     self.assertIs
-0001a840: 4e6f 6e65 2873 6563 7265 742e 6c61 6265  None(secret.labe
-0001a850: 6c29 0a0a 2020 2020 2020 2020 7365 6c66  l)..        self
-0001a860: 2e61 7373 6572 7445 7175 616c 2866 616b  .assertEqual(fak
-0001a870: 655f 7363 7269 7074 5f63 616c 6c73 2873  e_script_calls(s
-0001a880: 656c 662c 2063 6c65 6172 3d54 7275 6529  elf, clear=True)
-0001a890: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001a8a0: 2020 2020 2020 2020 2020 205b 5b27 7365             [['se
-0001a8b0: 6372 6574 2d61 6464 272c 2027 2d2d 6f77  cret-add', '--ow
-0001a8c0: 6e65 7227 2c20 2761 7070 6c69 6361 7469  ner', 'applicati
-0001a8d0: 6f6e 272c 2027 666f 6f3d 7827 5d5d 290a  on', 'foo=x']]).
-0001a8e0: 0a20 2020 2064 6566 2074 6573 745f 6170  .    def test_ap
-0001a8f0: 705f 6164 645f 7365 6372 6574 5f61 7267  p_add_secret_arg
-0001a900: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-0001a910: 2066 616b 655f 7363 7269 7074 2873 656c   fake_script(sel
-0001a920: 662c 2027 7365 6372 6574 2d61 6464 272c  f, 'secret-add',
-0001a930: 2027 6563 686f 2073 6563 7265 743a 3233   'echo secret:23
-0001a940: 3427 290a 0a20 2020 2020 2020 2065 7870  4')..        exp
-0001a950: 6972 6520 3d20 6461 7465 7469 6d65 2e64  ire = datetime.d
-0001a960: 6174 6574 696d 6528 3230 3232 2c20 3132  atetime(2022, 12
-0001a970: 2c20 392c 2031 362c 2031 372c 2030 290a  , 9, 16, 17, 0).
-0001a980: 2020 2020 2020 2020 7365 6372 6574 203d          secret =
-0001a990: 2073 656c 662e 6170 702e 6164 645f 7365   self.app.add_se
-0001a9a0: 6372 6574 287b 2766 6f6f 273a 2027 7827  cret({'foo': 'x'
-0001a9b0: 2c20 2762 6172 273a 2027 7927 7d2c 206c  , 'bar': 'y'}, l
-0001a9c0: 6162 656c 3d27 6c62 6c27 2c20 6465 7363  abel='lbl', desc
-0001a9d0: 7269 7074 696f 6e3d 2764 6573 6327 2c0a  ription='desc',.
-0001a9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa00: 2020 2020 2065 7870 6972 653d 6578 7069       expire=expi
-0001aa10: 7265 2c20 726f 7461 7465 3d6f 7073 2e53  re, rotate=ops.S
-0001aa20: 6563 7265 7452 6f74 6174 652e 484f 5552  ecretRotate.HOUR
-0001aa30: 4c59 290a 2020 2020 2020 2020 7365 6c66  LY).        self
-0001aa40: 2e61 7373 6572 7445 7175 616c 2873 6563  .assertEqual(sec
-0001aa50: 7265 742e 6964 2c20 2773 6563 7265 743a  ret.id, 'secret:
-0001aa60: 3233 3427 290a 2020 2020 2020 2020 7365  234').        se
-0001aa70: 6c66 2e61 7373 6572 7445 7175 616c 2873  lf.assertEqual(s
-0001aa80: 6563 7265 742e 6c61 6265 6c2c 2027 6c62  ecret.label, 'lb
-0001aa90: 6c27 290a 2020 2020 2020 2020 7365 6c66  l').        self
-0001aaa0: 2e61 7373 6572 7445 7175 616c 2873 6563  .assertEqual(sec
-0001aab0: 7265 742e 6765 745f 636f 6e74 656e 7428  ret.get_content(
-0001aac0: 292c 207b 2766 6f6f 273a 2027 7827 2c20  ), {'foo': 'x', 
-0001aad0: 2762 6172 273a 2027 7927 7d29 0a0a 2020  'bar': 'y'})..  
-0001aae0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0001aaf0: 7445 7175 616c 2866 616b 655f 7363 7269  tEqual(fake_scri
-0001ab00: 7074 5f63 616c 6c73 2873 656c 662c 2063  pt_calls(self, c
-0001ab10: 6c65 6172 3d54 7275 6529 2c0a 2020 2020  lear=True),.    
-0001ab20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab30: 2020 2020 205b 5b27 7365 6372 6574 2d61       [['secret-a
-0001ab40: 6464 272c 2027 2d2d 6c61 6265 6c27 2c20  dd', '--label', 
-0001ab50: 276c 626c 272c 2027 2d2d 6465 7363 7269  'lbl', '--descri
-0001ab60: 7074 696f 6e27 2c20 2764 6573 6327 2c0a  ption', 'desc',.
-0001ab70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab80: 2020 2020 2020 2020 2020 2027 2d2d 6578             '--ex
-0001ab90: 7069 7265 272c 2027 3230 3232 2d31 322d  pire', '2022-12-
-0001aba0: 3039 5431 363a 3137 3a30 3027 2c20 272d  09T16:17:00', '-
-0001abb0: 2d72 6f74 6174 6527 2c20 2768 6f75 726c  -rotate', 'hourl
-0001abc0: 7927 2c0a 2020 2020 2020 2020 2020 2020  y',.            
-0001abd0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0001abe0: 2d2d 6f77 6e65 7227 2c20 2761 7070 6c69  --owner', 'appli
-0001abf0: 6361 7469 6f6e 272c 2027 666f 6f3d 7827  cation', 'foo=x'
-0001ac00: 2c20 2762 6172 3d79 275d 5d29 0a0a 2020  , 'bar=y']])..  
-0001ac10: 2020 6465 6620 7465 7374 5f75 6e69 745f    def test_unit_
-0001ac20: 6164 645f 7365 6372 6574 5f73 696d 706c  add_secret_simpl
-0001ac30: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-0001ac40: 2066 616b 655f 7363 7269 7074 2873 656c   fake_script(sel
-0001ac50: 662c 2027 7365 6372 6574 2d61 6464 272c  f, 'secret-add',
-0001ac60: 2027 6563 686f 2073 6563 7265 743a 3334   'echo secret:34
-0001ac70: 3527 290a 0a20 2020 2020 2020 2073 6563  5')..        sec
-0001ac80: 7265 7420 3d20 7365 6c66 2e75 6e69 742e  ret = self.unit.
-0001ac90: 6164 645f 7365 6372 6574 287b 2766 6f6f  add_secret({'foo
-0001aca0: 273a 2027 7827 7d29 0a20 2020 2020 2020  ': 'x'}).       
-0001acb0: 2073 656c 662e 6173 7365 7274 4973 496e   self.assertIsIn
-0001acc0: 7374 616e 6365 2873 6563 7265 742c 206f  stance(secret, o
-0001acd0: 7073 2e53 6563 7265 7429 0a20 2020 2020  ps.Secret).     
-0001ace0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0001acf0: 7561 6c28 7365 6372 6574 2e69 642c 2027  ual(secret.id, '
-0001ad00: 7365 6372 6574 3a33 3435 2729 0a20 2020  secret:345').   
-0001ad10: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0001ad20: 4973 4e6f 6e65 2873 6563 7265 742e 6c61  IsNone(secret.la
-0001ad30: 6265 6c29 0a0a 2020 2020 2020 2020 7365  bel)..        se
-0001ad40: 6c66 2e61 7373 6572 7445 7175 616c 2866  lf.assertEqual(f
-0001ad50: 616b 655f 7363 7269 7074 5f63 616c 6c73  ake_script_calls
-0001ad60: 2873 656c 662c 2063 6c65 6172 3d54 7275  (self, clear=Tru
-0001ad70: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
-0001ad80: 2020 2020 2020 2020 2020 2020 205b 5b27               [['
-0001ad90: 7365 6372 6574 2d61 6464 272c 2027 2d2d  secret-add', '--
-0001ada0: 6f77 6e65 7227 2c20 2775 6e69 7427 2c20  owner', 'unit', 
-0001adb0: 2766 6f6f 3d78 275d 5d29 0a0a 2020 2020  'foo=x']])..    
-0001adc0: 6465 6620 7465 7374 5f75 6e69 745f 6164  def test_unit_ad
-0001add0: 645f 7365 6372 6574 5f61 7267 7328 7365  d_secret_args(se
-0001ade0: 6c66 293a 0a20 2020 2020 2020 2066 616b  lf):.        fak
-0001adf0: 655f 7363 7269 7074 2873 656c 662c 2027  e_script(self, '
-0001ae00: 7365 6372 6574 2d61 6464 272c 2027 6563  secret-add', 'ec
-0001ae10: 686f 2073 6563 7265 743a 3435 3627 290a  ho secret:456').
-0001ae20: 0a20 2020 2020 2020 2065 7870 6972 6520  .        expire 
-0001ae30: 3d20 6461 7465 7469 6d65 2e64 6174 6574  = datetime.datet
-0001ae40: 696d 6528 3230 3232 2c20 3132 2c20 392c  ime(2022, 12, 9,
-0001ae50: 2031 362c 2032 322c 2030 290a 2020 2020   16, 22, 0).    
-0001ae60: 2020 2020 7365 6372 6574 203d 2073 656c      secret = sel
-0001ae70: 662e 756e 6974 2e61 6464 5f73 6563 7265  f.unit.add_secre
-0001ae80: 7428 7b27 666f 6f27 3a20 2777 272c 2027  t({'foo': 'w', '
-0001ae90: 6261 7227 3a20 277a 277d 2c20 6c61 6265  bar': 'z'}, labe
-0001aea0: 6c3d 276c 3227 2c20 6465 7363 7269 7074  l='l2', descript
-0001aeb0: 696f 6e3d 2778 797a 272c 0a20 2020 2020  ion='xyz',.     
-0001aec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aee0: 2065 7870 6972 653d 6578 7069 7265 2c20   expire=expire, 
-0001aef0: 726f 7461 7465 3d6f 7073 2e53 6563 7265  rotate=ops.Secre
-0001af00: 7452 6f74 6174 652e 5945 4152 4c59 290a  tRotate.YEARLY).
-0001af10: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0001af20: 6572 7445 7175 616c 2873 6563 7265 742e  ertEqual(secret.
-0001af30: 6964 2c20 2773 6563 7265 743a 3435 3627  id, 'secret:456'
-0001af40: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0001af50: 7373 6572 7445 7175 616c 2873 6563 7265  ssertEqual(secre
-0001af60: 742e 6c61 6265 6c2c 2027 6c32 2729 0a20  t.label, 'l2'). 
-0001af70: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0001af80: 7274 4571 7561 6c28 7365 6372 6574 2e67  rtEqual(secret.g
-0001af90: 6574 5f63 6f6e 7465 6e74 2829 2c20 7b27  et_content(), {'
-0001afa0: 666f 6f27 3a20 2777 272c 2027 6261 7227  foo': 'w', 'bar'
-0001afb0: 3a20 277a 277d 290a 0a20 2020 2020 2020  : 'z'})..       
-0001afc0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0001afd0: 6c28 6661 6b65 5f73 6372 6970 745f 6361  l(fake_script_ca
-0001afe0: 6c6c 7328 7365 6c66 2c20 636c 6561 723d  lls(self, clear=
-0001aff0: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
-0001b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b010: 5b5b 2773 6563 7265 742d 6164 6427 2c20  [['secret-add', 
-0001b020: 272d 2d6c 6162 656c 272c 2027 6c32 272c  '--label', 'l2',
-0001b030: 2027 2d2d 6465 7363 7269 7074 696f 6e27   '--description'
-0001b040: 2c20 2778 797a 272c 0a20 2020 2020 2020  , 'xyz',.       
-0001b050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b060: 2020 2020 272d 2d65 7870 6972 6527 2c20      '--expire', 
-0001b070: 2732 3032 322d 3132 2d30 3954 3136 3a32  '2022-12-09T16:2
-0001b080: 323a 3030 272c 2027 2d2d 726f 7461 7465  2:00', '--rotate
-0001b090: 272c 2027 7965 6172 6c79 272c 0a20 2020  ', 'yearly',.   
-0001b0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b0b0: 2020 2020 2020 2020 272d 2d6f 776e 6572          '--owner
-0001b0c0: 272c 2027 756e 6974 272c 2027 666f 6f3d  ', 'unit', 'foo=
-0001b0d0: 7727 2c20 2762 6172 3d7a 275d 5d29 0a0a  w', 'bar=z']])..
-0001b0e0: 2020 2020 6465 6620 7465 7374 5f75 6e69      def test_uni
-0001b0f0: 745f 6164 645f 7365 6372 6574 5f65 7272  t_add_secret_err
-0001b100: 6f72 7328 7365 6c66 293a 0a20 2020 2020  ors(self):.     
-0001b110: 2020 2023 2041 6464 6974 696f 6e61 6c20     # Additional 
-0001b120: 6164 645f 7365 6372 6574 2074 6573 7473  add_secret tests
-0001b130: 2061 7265 2064 6f6e 6520 696e 2054 6573   are done in Tes
-0001b140: 7441 7070 6c69 6361 7469 6f6e 0a20 2020  tApplication.   
-0001b150: 2020 2020 2065 7272 6f72 7320 3d20 5b0a       errors = [.
-0001b160: 2020 2020 2020 2020 2020 2020 287b 2778              ({'x
-0001b170: 7927 3a20 2762 6172 277d 2c20 7b7d 2c20  y': 'bar'}, {}, 
-0001b180: 5661 6c75 6545 7272 6f72 292c 0a20 2020  ValueError),.   
-0001b190: 2020 2020 2020 2020 2028 7b27 666f 6f27           ({'foo'
-0001b1a0: 3a20 2778 277d 2c20 7b27 6578 7069 7265  : 'x'}, {'expire
-0001b1b0: 273a 2037 7d2c 2054 7970 6545 7272 6f72  ': 7}, TypeError
-0001b1c0: 292c 0a20 2020 2020 2020 205d 0a20 2020  ),.        ].   
-0001b1d0: 2020 2020 2066 6f72 2063 6f6e 7465 6e74       for content
-0001b1e0: 2c20 6b77 6172 6773 2c20 6578 635f 7479  , kwargs, exc_ty
-0001b1f0: 7065 2069 6e20 6572 726f 7273 3a0a 2020  pe in errors:.  
-0001b200: 2020 2020 2020 2020 2020 6d73 6720 3d20            msg = 
-0001b210: 6627 6578 7065 6374 6564 207b 6578 635f  f'expected {exc_
-0001b220: 7479 7065 2e5f 5f6e 616d 655f 5f7d 2077  type.__name__} w
-0001b230: 6865 6e20 6164 6469 6e67 2073 6563 7265  hen adding secre
-0001b240: 7420 636f 6e74 656e 7420 7b63 6f6e 7465  t content {conte
-0001b250: 6e74 7d27 0a20 2020 2020 2020 2020 2020  nt}'.           
-0001b260: 2077 6974 6820 7365 6c66 2e61 7373 6572   with self.asser
-0001b270: 7452 6169 7365 7328 6578 635f 7479 7065  tRaises(exc_type
-0001b280: 2c20 6d73 673d 6d73 6729 3a0a 2020 2020  , msg=msg):.    
-0001b290: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001b2a0: 2e75 6e69 742e 6164 645f 7365 6372 6574  .unit.add_secret
-0001b2b0: 2863 6f6e 7465 6e74 2c20 2a2a 6b77 6172  (content, **kwar
-0001b2c0: 6773 290a 0a20 2020 2064 6566 2074 6573  gs)..    def tes
-0001b2d0: 745f 6164 645f 7365 6372 6574 5f65 7272  t_add_secret_err
-0001b2e0: 6f72 7328 7365 6c66 293a 0a20 2020 2020  ors(self):.     
-0001b2f0: 2020 2065 7272 6f72 7320 3d20 5b0a 2020     errors = [.  
-0001b300: 2020 2020 2020 2020 2020 2320 496e 7661            # Inva
-0001b310: 6c69 6420 636f 6e74 656e 7420 6469 6374  lid content dict
-0001b320: 206f 7220 7479 7065 730a 2020 2020 2020   or types.      
-0001b330: 2020 2020 2020 284e 6f6e 652c 207b 7d2c        (None, {},
-0001b340: 2054 7970 6545 7272 6f72 292c 0a20 2020   TypeError),.   
-0001b350: 2020 2020 2020 2020 2028 7b7d 2c20 7b7d           ({}, {}
-0001b360: 2c20 5661 6c75 6545 7272 6f72 292c 0a20  , ValueError),. 
-0001b370: 2020 2020 2020 2020 2020 2028 7b62 2766             ({b'f
-0001b380: 6f6f 272c 2027 6261 7227 7d2c 207b 7d2c  oo', 'bar'}, {},
-0001b390: 2054 7970 6545 7272 6f72 292c 0a20 2020   TypeError),.   
-0001b3a0: 2020 2020 2020 2020 2028 7b33 3a20 2762           ({3: 'b
-0001b3b0: 6172 277d 2c20 7b7d 2c20 5479 7065 4572  ar'}, {}, TypeEr
-0001b3c0: 726f 7229 2c0a 2020 2020 2020 2020 2020  ror),.          
-0001b3d0: 2020 287b 2766 6f6f 273a 2031 2c20 2762    ({'foo': 1, 'b
-0001b3e0: 6172 273a 2032 7d2c 207b 7d2c 2054 7970  ar': 2}, {}, Typ
-0001b3f0: 6545 7272 6f72 292c 0a20 2020 2020 2020  eError),.       
-0001b400: 2020 2020 2023 2049 6e76 616c 6964 2063       # Invalid c
-0001b410: 6f6e 7465 6e74 206b 6579 730a 2020 2020  ontent keys.    
-0001b420: 2020 2020 2020 2020 287b 2778 7927 3a20          ({'xy': 
-0001b430: 2762 6172 277d 2c20 7b7d 2c20 5661 6c75  'bar'}, {}, Valu
-0001b440: 6545 7272 6f72 292c 0a20 2020 2020 2020  eError),.       
-0001b450: 2020 2020 2028 7b27 464f 4f27 3a20 2762       ({'FOO': 'b
-0001b460: 6172 277d 2c20 7b7d 2c20 5661 6c75 6545  ar'}, {}, ValueE
-0001b470: 7272 6f72 292c 0a20 2020 2020 2020 2020  rror),.         
-0001b480: 2020 2028 7b27 666f 6f2d 273a 2027 6261     ({'foo-': 'ba
-0001b490: 7227 7d2c 207b 7d2c 2056 616c 7565 4572  r'}, {}, ValueEr
-0001b4a0: 726f 7229 2c0a 2020 2020 2020 2020 2020  ror),.          
-0001b4b0: 2020 287b 272d 666f 6f27 3a20 2762 6172    ({'-foo': 'bar
-0001b4c0: 277d 2c20 7b7d 2c20 5661 6c75 6545 7272  '}, {}, ValueErr
-0001b4d0: 6f72 292c 0a20 2020 2020 2020 2020 2020  or),.           
-0001b4e0: 2023 2049 6e76 616c 6964 2022 6578 7069   # Invalid "expi
-0001b4f0: 7265 2220 7479 7065 0a20 2020 2020 2020  re" type.       
-0001b500: 2020 2020 2028 7b27 666f 6f27 3a20 2778       ({'foo': 'x
-0001b510: 277d 2c20 7b27 6578 7069 7265 273a 2037  '}, {'expire': 7
-0001b520: 7d2c 2054 7970 6545 7272 6f72 292c 0a20  }, TypeError),. 
-0001b530: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-0001b540: 2066 6f72 2063 6f6e 7465 6e74 2c20 6b77   for content, kw
-0001b550: 6172 6773 2c20 6578 635f 7479 7065 2069  args, exc_type i
-0001b560: 6e20 6572 726f 7273 3a0a 2020 2020 2020  n errors:.      
-0001b570: 2020 2020 2020 6d73 6720 3d20 6627 6578        msg = f'ex
-0001b580: 7065 6374 6564 207b 6578 635f 7479 7065  pected {exc_type
-0001b590: 2e5f 5f6e 616d 655f 5f7d 2077 6865 6e20  .__name__} when 
-0001b5a0: 6164 6469 6e67 2073 6563 7265 7420 636f  adding secret co
-0001b5b0: 6e74 656e 7420 7b63 6f6e 7465 6e74 7d27  ntent {content}'
-0001b5c0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-0001b5d0: 6820 7365 6c66 2e61 7373 6572 7452 6169  h self.assertRai
-0001b5e0: 7365 7328 6578 635f 7479 7065 2c20 6d73  ses(exc_type, ms
-0001b5f0: 673d 6d73 6729 3a0a 2020 2020 2020 2020  g=msg):.        
-0001b600: 2020 2020 2020 2020 7365 6c66 2e61 7070          self.app
-0001b610: 2e61 6464 5f73 6563 7265 7428 636f 6e74  .add_secret(cont
-0001b620: 656e 742c 202a 2a6b 7761 7267 7329 0a20  ent, **kwargs). 
-0001b630: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-0001b640: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
-0001b650: 7328 6578 635f 7479 7065 2c20 6d73 673d  s(exc_type, msg=
-0001b660: 6d73 6729 3a0a 2020 2020 2020 2020 2020  msg):.          
-0001b670: 2020 2020 2020 7365 6c66 2e75 6e69 742e        self.unit.
-0001b680: 6164 645f 7365 6372 6574 2863 6f6e 7465  add_secret(conte
-0001b690: 6e74 2c20 2a2a 6b77 6172 6773 290a 0a20  nt, **kwargs).. 
-0001b6a0: 2020 2064 6566 2074 6573 745f 6765 745f     def test_get_
-0001b6b0: 7365 6372 6574 5f69 6428 7365 6c66 293a  secret_id(self):
-0001b6c0: 0a20 2020 2020 2020 2066 616b 655f 7363  .        fake_sc
-0001b6d0: 7269 7074 2873 656c 662c 2027 7365 6372  ript(self, 'secr
-0001b6e0: 6574 2d67 6574 272c 2022 2222 6563 686f  et-get', """echo
-0001b6f0: 2027 7b22 666f 6f22 3a20 2267 227d 2722   '{"foo": "g"}'"
-0001b700: 2222 290a 0a20 2020 2020 2020 2073 6563  "")..        sec
-0001b710: 7265 7420 3d20 7365 6c66 2e6d 6f64 656c  ret = self.model
-0001b720: 2e67 6574 5f73 6563 7265 7428 6964 3d27  .get_secret(id='
-0001b730: 3132 3327 290a 2020 2020 2020 2020 7365  123').        se
-0001b740: 6c66 2e61 7373 6572 7445 7175 616c 2873  lf.assertEqual(s
-0001b750: 6563 7265 742e 6964 2c20 2773 6563 7265  ecret.id, 'secre
-0001b760: 743a 3132 3327 290a 2020 2020 2020 2020  t:123').        
-0001b770: 7365 6c66 2e61 7373 6572 7449 734e 6f6e  self.assertIsNon
-0001b780: 6528 7365 6372 6574 2e6c 6162 656c 290a  e(secret.label).
-0001b790: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0001b7a0: 6572 7445 7175 616c 2873 6563 7265 742e  ertEqual(secret.
-0001b7b0: 6765 745f 636f 6e74 656e 7428 292c 207b  get_content(), {
-0001b7c0: 2766 6f6f 273a 2027 6727 7d29 0a0a 2020  'foo': 'g'})..  
-0001b7d0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0001b7e0: 7445 7175 616c 2866 616b 655f 7363 7269  tEqual(fake_scri
-0001b7f0: 7074 5f63 616c 6c73 2873 656c 662c 2063  pt_calls(self, c
-0001b800: 6c65 6172 3d54 7275 6529 2c0a 2020 2020  lear=True),.    
-0001b810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b820: 2020 2020 205b 5b27 7365 6372 6574 2d67       [['secret-g
-0001b830: 6574 272c 2027 7365 6372 6574 3a31 3233  et', 'secret:123
-0001b840: 272c 2027 2d2d 666f 726d 6174 3d6a 736f  ', '--format=jso
-0001b850: 6e27 5d5d 290a 0a20 2020 2064 6566 2074  n']])..    def t
-0001b860: 6573 745f 6765 745f 7365 6372 6574 5f6c  est_get_secret_l
-0001b870: 6162 656c 2873 656c 6629 3a0a 2020 2020  abel(self):.    
-0001b880: 2020 2020 6661 6b65 5f73 6372 6970 7428      fake_script(
-0001b890: 7365 6c66 2c20 2773 6563 7265 742d 6765  self, 'secret-ge
-0001b8a0: 7427 2c20 2222 2265 6368 6f20 277b 2266  t', """echo '{"f
-0001b8b0: 6f6f 223a 2022 6722 7d27 2222 2229 0a0a  oo": "g"}'""")..
-0001b8c0: 2020 2020 2020 2020 7365 6372 6574 203d          secret =
-0001b8d0: 2073 656c 662e 6d6f 6465 6c2e 6765 745f   self.model.get_
-0001b8e0: 7365 6372 6574 286c 6162 656c 3d27 6c62  secret(label='lb
-0001b8f0: 6c27 290a 2020 2020 2020 2020 7365 6c66  l').        self
-0001b900: 2e61 7373 6572 7449 734e 6f6e 6528 7365  .assertIsNone(se
-0001b910: 6372 6574 2e69 6429 0a20 2020 2020 2020  cret.id).       
-0001b920: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0001b930: 6c28 7365 6372 6574 2e6c 6162 656c 2c20  l(secret.label, 
-0001b940: 276c 626c 2729 0a20 2020 2020 2020 2073  'lbl').        s
-0001b950: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0001b960: 7365 6372 6574 2e67 6574 5f63 6f6e 7465  secret.get_conte
-0001b970: 6e74 2829 2c20 7b27 666f 6f27 3a20 2767  nt(), {'foo': 'g
-0001b980: 277d 290a 0a20 2020 2020 2020 2073 656c  '})..        sel
-0001b990: 662e 6173 7365 7274 4571 7561 6c28 6661  f.assertEqual(fa
-0001b9a0: 6b65 5f73 6372 6970 745f 6361 6c6c 7328  ke_script_calls(
-0001b9b0: 7365 6c66 2c20 636c 6561 723d 5472 7565  self, clear=True
-0001b9c0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0001b9d0: 2020 2020 2020 2020 2020 2020 5b5b 2773              [['s
-0001b9e0: 6563 7265 742d 6765 7427 2c20 272d 2d6c  ecret-get', '--l
-0001b9f0: 6162 656c 272c 2027 6c62 6c27 2c20 272d  abel', 'lbl', '-
-0001ba00: 2d66 6f72 6d61 743d 6a73 6f6e 275d 5d29  -format=json']])
-0001ba10: 0a0a 2020 2020 6465 6620 7465 7374 5f67  ..    def test_g
-0001ba20: 6574 5f73 6563 7265 745f 6964 5f61 6e64  et_secret_id_and
-0001ba30: 5f6c 6162 656c 2873 656c 6629 3a0a 2020  _label(self):.  
-0001ba40: 2020 2020 2020 6661 6b65 5f73 6372 6970        fake_scrip
-0001ba50: 7428 7365 6c66 2c20 2773 6563 7265 742d  t(self, 'secret-
-0001ba60: 6765 7427 2c20 2222 2265 6368 6f20 277b  get', """echo '{
-0001ba70: 2266 6f6f 223a 2022 6822 7d27 2222 2229  "foo": "h"}'""")
-0001ba80: 0a0a 2020 2020 2020 2020 7365 6372 6574  ..        secret
-0001ba90: 203d 2073 656c 662e 6d6f 6465 6c2e 6765   = self.model.ge
-0001baa0: 745f 7365 6372 6574 2869 643d 2731 3233  t_secret(id='123
-0001bab0: 272c 206c 6162 656c 3d27 6c27 290a 2020  ', label='l').  
-0001bac0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0001bad0: 7445 7175 616c 2873 6563 7265 742e 6964  tEqual(secret.id
-0001bae0: 2c20 2773 6563 7265 743a 3132 3327 290a  , 'secret:123').
-0001baf0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0001bb00: 6572 7445 7175 616c 2873 6563 7265 742e  ertEqual(secret.
-0001bb10: 6c61 6265 6c2c 2027 6c27 290a 2020 2020  label, 'l').    
-0001bb20: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0001bb30: 7175 616c 2873 6563 7265 742e 6765 745f  qual(secret.get_
-0001bb40: 636f 6e74 656e 7428 292c 207b 2766 6f6f  content(), {'foo
-0001bb50: 273a 2027 6827 7d29 0a0a 2020 2020 2020  ': 'h'})..      
-0001bb60: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0001bb70: 616c 2866 616b 655f 7363 7269 7074 5f63  al(fake_script_c
-0001bb80: 616c 6c73 2873 656c 662c 2063 6c65 6172  alls(self, clear
-0001bb90: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
-0001bba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bbb0: 205b 5b27 7365 6372 6574 2d67 6574 272c   [['secret-get',
-0001bbc0: 2027 7365 6372 6574 3a31 3233 272c 2027   'secret:123', '
-0001bbd0: 2d2d 6c61 6265 6c27 2c20 276c 272c 2027  --label', 'l', '
-0001bbe0: 2d2d 666f 726d 6174 3d6a 736f 6e27 5d5d  --format=json']]
-0001bbf0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-0001bc00: 6765 745f 7365 6372 6574 5f6e 6f5f 6172  get_secret_no_ar
-0001bc10: 6773 2873 656c 6629 3a0a 2020 2020 2020  gs(self):.      
-0001bc20: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
-0001bc30: 7274 5261 6973 6573 2854 7970 6545 7272  rtRaises(TypeErr
-0001bc40: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
-0001bc50: 2073 656c 662e 6d6f 6465 6c2e 6765 745f   self.model.get_
-0001bc60: 7365 6372 6574 2829 0a0a 2020 2020 6465  secret()..    de
-0001bc70: 6620 7465 7374 5f67 6574 5f73 6563 7265  f test_get_secre
-0001bc80: 745f 6e6f 745f 666f 756e 6428 7365 6c66  t_not_found(self
-0001bc90: 293a 0a20 2020 2020 2020 2073 6372 6970  ):.        scrip
-0001bca0: 7420 3d20 2222 2265 6368 6f20 2745 5252  t = """echo 'ERR
-0001bcb0: 4f52 2073 6563 7265 7420 2231 3233 2220  OR secret "123" 
-0001bcc0: 6e6f 7420 666f 756e 6427 203e 2632 3b20  not found' >&2; 
-0001bcd0: 6578 6974 2031 2222 220a 2020 2020 2020  exit 1""".      
-0001bce0: 2020 6661 6b65 5f73 6372 6970 7428 7365    fake_script(se
-0001bcf0: 6c66 2c20 2773 6563 7265 742d 6765 7427  lf, 'secret-get'
-0001bd00: 2c20 7363 7269 7074 290a 2020 2020 2020  , script).      
-0001bd10: 2020 6661 6b65 5f73 6372 6970 7428 7365    fake_script(se
-0001bd20: 6c66 2c20 2773 6563 7265 742d 696e 666f  lf, 'secret-info
-0001bd30: 2d67 6574 272c 2073 6372 6970 7429 0a0a  -get', script)..
-0001bd40: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0001bd50: 662e 6173 7365 7274 5261 6973 6573 286f  f.assertRaises(o
-0001bd60: 7073 2e53 6563 7265 744e 6f74 466f 756e  ps.SecretNotFoun
-0001bd70: 6445 7272 6f72 293a 0a20 2020 2020 2020  dError):.       
-0001bd80: 2020 2020 2073 656c 662e 6d6f 6465 6c2e       self.model.
-0001bd90: 6765 745f 7365 6372 6574 2869 643d 2731  get_secret(id='1
-0001bda0: 3233 2729 0a0a 2020 2020 6465 6620 7465  23')..    def te
-0001bdb0: 7374 5f67 6574 5f73 6563 7265 745f 6f74  st_get_secret_ot
-0001bdc0: 6865 725f 6572 726f 7228 7365 6c66 293a  her_error(self):
-0001bdd0: 0a20 2020 2020 2020 2073 6372 6970 7420  .        script 
-0001bde0: 3d20 2222 2265 6368 6f20 2745 5252 4f52  = """echo 'ERROR
-0001bdf0: 206f 7468 6572 2065 7272 6f72 2720 3e26   other error' >&
-0001be00: 323b 2065 7869 7420 3122 2222 0a20 2020  2; exit 1""".   
-0001be10: 2020 2020 2066 616b 655f 7363 7269 7074       fake_script
-0001be20: 2873 656c 662c 2027 7365 6372 6574 2d67  (self, 'secret-g
-0001be30: 6574 272c 2073 6372 6970 7429 0a20 2020  et', script).   
-0001be40: 2020 2020 2066 616b 655f 7363 7269 7074       fake_script
-0001be50: 2873 656c 662c 2027 7365 6372 6574 2d69  (self, 'secret-i
-0001be60: 6e66 6f2d 6765 7427 2c20 7363 7269 7074  nfo-get', script
-0001be70: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
-0001be80: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
-0001be90: 7328 6f70 732e 4d6f 6465 6c45 7272 6f72  s(ops.ModelError
-0001bea0: 2920 6173 2063 6d3a 0a20 2020 2020 2020  ) as cm:.       
-0001beb0: 2020 2020 2073 656c 662e 6d6f 6465 6c2e       self.model.
-0001bec0: 6765 745f 7365 6372 6574 2869 643d 2731  get_secret(id='1
-0001bed0: 3233 2729 0a20 2020 2020 2020 2073 656c  23').        sel
-0001bee0: 662e 6173 7365 7274 4e6f 7449 7349 6e73  f.assertNotIsIns
-0001bef0: 7461 6e63 6528 636d 2e65 7863 6570 7469  tance(cm.excepti
-0001bf00: 6f6e 2c20 6f70 732e 5365 6372 6574 4e6f  on, ops.SecretNo
-0001bf10: 7446 6f75 6e64 4572 726f 7229 0a0a 0a63  tFoundError)...c
-0001bf20: 6c61 7373 2054 6573 7453 6563 7265 7449  lass TestSecretI
-0001bf30: 6e66 6f28 756e 6974 7465 7374 2e54 6573  nfo(unittest.Tes
-0001bf40: 7443 6173 6529 3a0a 2020 2020 6465 6620  tCase):.    def 
-0001bf50: 7465 7374 5f69 6e69 7428 7365 6c66 293a  test_init(self):
-0001bf60: 0a20 2020 2020 2020 2069 6e66 6f20 3d20  .        info = 
-0001bf70: 6f70 732e 5365 6372 6574 496e 666f 280a  ops.SecretInfo(.
-0001bf80: 2020 2020 2020 2020 2020 2020 6964 3d27              id='
-0001bf90: 3327 2c0a 2020 2020 2020 2020 2020 2020  3',.            
-0001bfa0: 6c61 6265 6c3d 276c 626c 272c 0a20 2020  label='lbl',.   
-0001bfb0: 2020 2020 2020 2020 2072 6576 6973 696f           revisio
-0001bfc0: 6e3d 372c 0a20 2020 2020 2020 2020 2020  n=7,.           
-0001bfd0: 2065 7870 6972 6573 3d64 6174 6574 696d   expires=datetim
-0001bfe0: 652e 6461 7465 7469 6d65 2832 3032 322c  e.datetime(2022,
-0001bff0: 2031 322c 2039 2c20 3134 2c20 3130 2c20   12, 9, 14, 10, 
-0001c000: 3029 2c0a 2020 2020 2020 2020 2020 2020  0),.            
-0001c010: 726f 7461 7469 6f6e 3d6f 7073 2e53 6563  rotation=ops.Sec
-0001c020: 7265 7452 6f74 6174 652e 4d4f 4e54 484c  retRotate.MONTHL
-0001c030: 592c 0a20 2020 2020 2020 2020 2020 2072  Y,.            r
-0001c040: 6f74 6174 6573 3d64 6174 6574 696d 652e  otates=datetime.
-0001c050: 6461 7465 7469 6d65 2832 3032 332c 2031  datetime(2023, 1
-0001c060: 2c20 392c 2031 342c 2031 302c 2030 292c  , 9, 14, 10, 0),
-0001c070: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0001c080: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0001c090: 7561 6c28 696e 666f 2e69 642c 2027 7365  ual(info.id, 'se
-0001c0a0: 6372 6574 3a33 2729 0a20 2020 2020 2020  cret:3').       
-0001c0b0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0001c0c0: 6c28 696e 666f 2e6c 6162 656c 2c20 276c  l(info.label, 'l
-0001c0d0: 626c 2729 0a20 2020 2020 2020 2073 656c  bl').        sel
-0001c0e0: 662e 6173 7365 7274 4571 7561 6c28 696e  f.assertEqual(in
-0001c0f0: 666f 2e72 6576 6973 696f 6e2c 2037 290a  fo.revision, 7).
-0001c100: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0001c110: 6572 7445 7175 616c 2869 6e66 6f2e 6578  ertEqual(info.ex
-0001c120: 7069 7265 732c 2064 6174 6574 696d 652e  pires, datetime.
-0001c130: 6461 7465 7469 6d65 2832 3032 322c 2031  datetime(2022, 1
-0001c140: 322c 2039 2c20 3134 2c20 3130 2c20 3029  2, 9, 14, 10, 0)
-0001c150: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0001c160: 7373 6572 7445 7175 616c 2869 6e66 6f2e  ssertEqual(info.
-0001c170: 726f 7461 7469 6f6e 2c20 6f70 732e 5365  rotation, ops.Se
-0001c180: 6372 6574 526f 7461 7465 2e4d 4f4e 5448  cretRotate.MONTH
-0001c190: 4c59 290a 2020 2020 2020 2020 7365 6c66  LY).        self
-0001c1a0: 2e61 7373 6572 7445 7175 616c 2869 6e66  .assertEqual(inf
-0001c1b0: 6f2e 726f 7461 7465 732c 2064 6174 6574  o.rotates, datet
-0001c1c0: 696d 652e 6461 7465 7469 6d65 2832 3032  ime.datetime(202
-0001c1d0: 332c 2031 2c20 392c 2031 342c 2031 302c  3, 1, 9, 14, 10,
-0001c1e0: 2030 2929 0a0a 2020 2020 2020 2020 7365   0))..        se
-0001c1f0: 6c66 2e61 7373 6572 7454 7275 6528 7265  lf.assertTrue(re
-0001c200: 7072 2869 6e66 6f29 2e73 7461 7274 7377  pr(info).startsw
-0001c210: 6974 6828 2753 6563 7265 7449 6e66 6f28  ith('SecretInfo(
-0001c220: 2729 290a 2020 2020 2020 2020 7365 6c66  ')).        self
-0001c230: 2e61 7373 6572 7454 7275 6528 7265 7072  .assertTrue(repr
-0001c240: 2869 6e66 6f29 2e65 6e64 7377 6974 6828  (info).endswith(
-0001c250: 2729 2729 290a 0a20 2020 2064 6566 2074  ')'))..    def t
-0001c260: 6573 745f 6672 6f6d 5f64 6963 7428 7365  est_from_dict(se
-0001c270: 6c66 293a 0a20 2020 2020 2020 2075 7463  lf):.        utc
-0001c280: 203d 2064 6174 6574 696d 652e 7469 6d65   = datetime.time
-0001c290: 7a6f 6e65 2e75 7463 0a20 2020 2020 2020  zone.utc.       
-0001c2a0: 2069 6e66 6f20 3d20 6f70 732e 5365 6372   info = ops.Secr
-0001c2b0: 6574 496e 666f 2e66 726f 6d5f 6469 6374  etInfo.from_dict
-0001c2c0: 2827 7365 6372 6574 3a34 272c 207b 0a20  ('secret:4', {. 
-0001c2d0: 2020 2020 2020 2020 2020 2027 6c61 6265             'labe
-0001c2e0: 6c27 3a20 2766 726f 6d64 6963 7427 2c0a  l': 'fromdict',.
-0001c2f0: 2020 2020 2020 2020 2020 2020 2772 6576              'rev
-0001c300: 6973 696f 6e27 3a20 382c 0a20 2020 2020  ision': 8,.     
-0001c310: 2020 2020 2020 2027 6578 7069 7265 7327         'expires'
-0001c320: 3a20 2732 3032 322d 3132 2d30 3954 3134  : '2022-12-09T14
-0001c330: 3a31 303a 3030 5a27 2c0a 2020 2020 2020  :10:00Z',.      
-0001c340: 2020 2020 2020 2772 6f74 6174 696f 6e27        'rotation'
-0001c350: 3a20 2779 6561 726c 7927 2c0a 2020 2020  : 'yearly',.    
-0001c360: 2020 2020 2020 2020 2772 6f74 6174 6573          'rotates
-0001c370: 273a 2027 3230 3233 2d30 312d 3039 5431  ': '2023-01-09T1
-0001c380: 343a 3130 3a30 305a 272c 0a20 2020 2020  4:10:00Z',.     
-0001c390: 2020 207d 290a 2020 2020 2020 2020 7365     }).        se
-0001c3a0: 6c66 2e61 7373 6572 7445 7175 616c 2869  lf.assertEqual(i
-0001c3b0: 6e66 6f2e 6964 2c20 2773 6563 7265 743a  nfo.id, 'secret:
-0001c3c0: 3427 290a 2020 2020 2020 2020 7365 6c66  4').        self
-0001c3d0: 2e61 7373 6572 7445 7175 616c 2869 6e66  .assertEqual(inf
-0001c3e0: 6f2e 6c61 6265 6c2c 2027 6672 6f6d 6469  o.label, 'fromdi
-0001c3f0: 6374 2729 0a20 2020 2020 2020 2073 656c  ct').        sel
-0001c400: 662e 6173 7365 7274 4571 7561 6c28 696e  f.assertEqual(in
-0001c410: 666f 2e72 6576 6973 696f 6e2c 2038 290a  fo.revision, 8).
-0001c420: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0001c430: 6572 7445 7175 616c 2869 6e66 6f2e 6578  ertEqual(info.ex
-0001c440: 7069 7265 732c 2064 6174 6574 696d 652e  pires, datetime.
-0001c450: 6461 7465 7469 6d65 2832 3032 322c 2031  datetime(2022, 1
-0001c460: 322c 2039 2c20 3134 2c20 3130 2c20 302c  2, 9, 14, 10, 0,
-0001c470: 2074 7a69 6e66 6f3d 7574 6329 290a 2020   tzinfo=utc)).  
-0001c480: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0001c490: 7445 7175 616c 2869 6e66 6f2e 726f 7461  tEqual(info.rota
-0001c4a0: 7469 6f6e 2c20 6f70 732e 5365 6372 6574  tion, ops.Secret
-0001c4b0: 526f 7461 7465 2e59 4541 524c 5929 0a20  Rotate.YEARLY). 
-0001c4c0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0001c4d0: 7274 4571 7561 6c28 696e 666f 2e72 6f74  rtEqual(info.rot
-0001c4e0: 6174 6573 2c20 6461 7465 7469 6d65 2e64  ates, datetime.d
-0001c4f0: 6174 6574 696d 6528 3230 3233 2c20 312c  atetime(2023, 1,
-0001c500: 2039 2c20 3134 2c20 3130 2c20 302c 2074   9, 14, 10, 0, t
-0001c510: 7a69 6e66 6f3d 7574 6329 290a 0a20 2020  zinfo=utc))..   
-0001c520: 2020 2020 2069 6e66 6f20 3d20 6f70 732e       info = ops.
-0001c530: 5365 6372 6574 496e 666f 2e66 726f 6d5f  SecretInfo.from_
-0001c540: 6469 6374 2827 7365 6372 6574 3a34 272c  dict('secret:4',
-0001c550: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-0001c560: 6c61 6265 6c27 3a20 2766 726f 6d64 6963  label': 'fromdic
-0001c570: 7427 2c0a 2020 2020 2020 2020 2020 2020  t',.            
-0001c580: 2772 6576 6973 696f 6e27 3a20 382c 0a20  'revision': 8,. 
-0001c590: 2020 2020 2020 2020 2020 2027 726f 7461             'rota
-0001c5a0: 7469 6f6e 273a 2027 6261 6476 616c 7565  tion': 'badvalue
-0001c5b0: 272c 0a20 2020 2020 2020 207d 290a 2020  ',.        }).  
-0001c5c0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0001c5d0: 7445 7175 616c 2869 6e66 6f2e 6964 2c20  tEqual(info.id, 
-0001c5e0: 2773 6563 7265 743a 3427 290a 2020 2020  'secret:4').    
-0001c5f0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0001c600: 7175 616c 2869 6e66 6f2e 6c61 6265 6c2c  qual(info.label,
-0001c610: 2027 6672 6f6d 6469 6374 2729 0a20 2020   'fromdict').   
-0001c620: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0001c630: 4571 7561 6c28 696e 666f 2e72 6576 6973  Equal(info.revis
-0001c640: 696f 6e2c 2038 290a 2020 2020 2020 2020  ion, 8).        
-0001c650: 7365 6c66 2e61 7373 6572 7449 734e 6f6e  self.assertIsNon
-0001c660: 6528 696e 666f 2e65 7870 6972 6573 290a  e(info.expires).
-0001c670: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0001c680: 6572 7449 734e 6f6e 6528 696e 666f 2e72  ertIsNone(info.r
-0001c690: 6f74 6174 696f 6e29 0a20 2020 2020 2020  otation).       
-0001c6a0: 2073 656c 662e 6173 7365 7274 4973 4e6f   self.assertIsNo
-0001c6b0: 6e65 2869 6e66 6f2e 726f 7461 7465 7329  ne(info.rotates)
-0001c6c0: 0a0a 2020 2020 2020 2020 696e 666f 203d  ..        info =
-0001c6d0: 206f 7073 2e53 6563 7265 7449 6e66 6f2e   ops.SecretInfo.
-0001c6e0: 6672 6f6d 5f64 6963 7428 2735 272c 207b  from_dict('5', {
-0001c6f0: 2772 6576 6973 696f 6e27 3a20 397d 290a  'revision': 9}).
-0001c700: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0001c710: 6572 7445 7175 616c 2869 6e66 6f2e 6964  ertEqual(info.id
-0001c720: 2c20 2773 6563 7265 743a 3527 290a 2020  , 'secret:5').  
-0001c730: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0001c740: 7445 7175 616c 2869 6e66 6f2e 7265 7669  tEqual(info.revi
-0001c750: 7369 6f6e 2c20 3929 0a0a 0a63 6c61 7373  sion, 9)...class
-0001c760: 2054 6573 7453 6563 7265 7443 6c61 7373   TestSecretClass
-0001c770: 2875 6e69 7474 6573 742e 5465 7374 4361  (unittest.TestCa
-0001c780: 7365 293a 0a20 2020 206d 6178 4469 6666  se):.    maxDiff
-0001c790: 203d 2036 3420 2a20 3130 3234 0a0a 2020   = 64 * 1024..  
-0001c7a0: 2020 6465 6620 7365 7455 7028 7365 6c66    def setUp(self
-0001c7b0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0001c7c0: 6d6f 6465 6c20 3d20 6f70 732e 4d6f 6465  model = ops.Mode
-0001c7d0: 6c28 6f70 732e 4368 6172 6d4d 6574 6128  l(ops.CharmMeta(
-0001c7e0: 292c 205f 4d6f 6465 6c42 6163 6b65 6e64  ), _ModelBackend
-0001c7f0: 2827 6d79 6170 702f 3027 2929 0a0a 2020  ('myapp/0'))..  
-0001c800: 2020 6465 6620 6d61 6b65 5f73 6563 7265    def make_secre
-0001c810: 7428 7365 6c66 2c20 6964 3d4e 6f6e 652c  t(self, id=None,
-0001c820: 206c 6162 656c 3d4e 6f6e 652c 2063 6f6e   label=None, con
-0001c830: 7465 6e74 3d4e 6f6e 6529 3a0a 2020 2020  tent=None):.    
-0001c840: 2020 2020 7265 7475 726e 206f 7073 2e53      return ops.S
-0001c850: 6563 7265 7428 7365 6c66 2e6d 6f64 656c  ecret(self.model
-0001c860: 2e5f 6261 636b 656e 642c 2069 643d 6964  ._backend, id=id
-0001c870: 2c20 6c61 6265 6c3d 6c61 6265 6c2c 2063  , label=label, c
-0001c880: 6f6e 7465 6e74 3d63 6f6e 7465 6e74 290a  ontent=content).
-0001c890: 0a20 2020 2064 6566 2074 6573 745f 6964  .    def test_id
-0001c8a0: 5f61 6e64 5f6c 6162 656c 2873 656c 6629  _and_label(self)
-0001c8b0: 3a0a 2020 2020 2020 2020 7365 6372 6574  :.        secret
-0001c8c0: 203d 2073 656c 662e 6d61 6b65 5f73 6563   = self.make_sec
-0001c8d0: 7265 7428 6964 3d27 2061 6263 2027 2c20  ret(id=' abc ', 
-0001c8e0: 6c61 6265 6c3d 276c 626c 2729 0a20 2020  label='lbl').   
-0001c8f0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0001c900: 4571 7561 6c28 7365 6372 6574 2e69 642c  Equal(secret.id,
-0001c910: 2027 7365 6372 6574 3a61 6263 2729 0a20   'secret:abc'). 
-0001c920: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0001c930: 7274 4571 7561 6c28 7365 6372 6574 2e6c  rtEqual(secret.l
-0001c940: 6162 656c 2c20 276c 626c 2729 0a0a 2020  abel, 'lbl')..  
-0001c950: 2020 2020 2020 7365 6372 6574 203d 2073        secret = s
-0001c960: 656c 662e 6d61 6b65 5f73 6563 7265 7428  elf.make_secret(
-0001c970: 6964 3d27 7827 290a 2020 2020 2020 2020  id='x').        
-0001c980: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0001c990: 2873 6563 7265 742e 6964 2c20 2773 6563  (secret.id, 'sec
-0001c9a0: 7265 743a 7827 290a 2020 2020 2020 2020  ret:x').        
-0001c9b0: 7365 6c66 2e61 7373 6572 7449 734e 6f6e  self.assertIsNon
-0001c9c0: 6528 7365 6372 6574 2e6c 6162 656c 290a  e(secret.label).
-0001c9d0: 0a20 2020 2020 2020 2073 6563 7265 7420  .        secret 
-0001c9e0: 3d20 7365 6c66 2e6d 616b 655f 7365 6372  = self.make_secr
-0001c9f0: 6574 286c 6162 656c 3d27 7927 290a 2020  et(label='y').  
-0001ca00: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0001ca10: 7449 734e 6f6e 6528 7365 6372 6574 2e69  tIsNone(secret.i
-0001ca20: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
-0001ca30: 6173 7365 7274 4571 7561 6c28 7365 6372  assertEqual(secr
-0001ca40: 6574 2e6c 6162 656c 2c20 2779 2729 0a0a  et.label, 'y')..
-0001ca50: 2020 2020 6465 6620 7465 7374 5f67 6574      def test_get
-0001ca60: 5f63 6f6e 7465 6e74 5f63 6163 6865 6428  _content_cached(
-0001ca70: 7365 6c66 293a 0a20 2020 2020 2020 2066  self):.        f
-0001ca80: 616b 655f 7363 7269 7074 2873 656c 662c  ake_script(self,
-0001ca90: 2027 7365 6372 6574 2d67 6574 272c 2022   'secret-get', "
-0001caa0: 2222 6578 6974 2031 2222 2229 0a0a 2020  ""exit 1""")..  
-0001cab0: 2020 2020 2020 7365 6372 6574 203d 2073        secret = s
-0001cac0: 656c 662e 6d61 6b65 5f73 6563 7265 7428  elf.make_secret(
-0001cad0: 6964 3d27 7827 2c20 6c61 6265 6c3d 2779  id='x', label='y
-0001cae0: 272c 2063 6f6e 7465 6e74 3d7b 2766 6f6f  ', content={'foo
-0001caf0: 273a 2027 6261 7227 7d29 0a20 2020 2020  ': 'bar'}).     
-0001cb00: 2020 2063 6f6e 7465 6e74 203d 2073 6563     content = sec
-0001cb10: 7265 742e 6765 745f 636f 6e74 656e 7428  ret.get_content(
-0001cb20: 2920 2023 2077 696c 6c20 7573 6520 6361  )  # will use ca
-0001cb30: 6368 6564 2063 6f6e 7465 6e74 2c20 6e6f  ched content, no
-0001cb40: 7420 7275 6e20 7365 6372 6574 2d67 6574  t run secret-get
-0001cb50: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0001cb60: 7365 7274 4571 7561 6c28 636f 6e74 656e  sertEqual(conten
-0001cb70: 742c 207b 2766 6f6f 273a 2027 6261 7227  t, {'foo': 'bar'
-0001cb80: 7d29 0a0a 2020 2020 2020 2020 7365 6c66  })..        self
-0001cb90: 2e61 7373 6572 7445 7175 616c 2866 616b  .assertEqual(fak
-0001cba0: 655f 7363 7269 7074 5f63 616c 6c73 2873  e_script_calls(s
-0001cbb0: 656c 662c 2063 6c65 6172 3d54 7275 6529  elf, clear=True)
-0001cbc0: 2c20 5b5d 290a 0a20 2020 2064 6566 2074  , [])..    def t
-0001cbd0: 6573 745f 6765 745f 636f 6e74 656e 745f  est_get_content_
-0001cbe0: 7265 6672 6573 6828 7365 6c66 293a 0a20  refresh(self):. 
-0001cbf0: 2020 2020 2020 2066 616b 655f 7363 7269         fake_scri
-0001cc00: 7074 2873 656c 662c 2027 7365 6372 6574  pt(self, 'secret
-0001cc10: 2d67 6574 272c 2022 2222 6563 686f 2027  -get', """echo '
-0001cc20: 7b22 666f 6f22 3a20 2272 6566 7265 7368  {"foo": "refresh
-0001cc30: 6564 227d 2722 2222 290a 0a20 2020 2020  ed"}'""")..     
-0001cc40: 2020 2073 6563 7265 7420 3d20 7365 6c66     secret = self
-0001cc50: 2e6d 616b 655f 7365 6372 6574 2869 643d  .make_secret(id=
-0001cc60: 2779 272c 2063 6f6e 7465 6e74 3d7b 2766  'y', content={'f
-0001cc70: 6f6f 273a 2027 6261 7227 7d29 0a20 2020  oo': 'bar'}).   
-0001cc80: 2020 2020 2063 6f6e 7465 6e74 203d 2073       content = s
-0001cc90: 6563 7265 742e 6765 745f 636f 6e74 656e  ecret.get_conten
-0001cca0: 7428 7265 6672 6573 683d 5472 7565 290a  t(refresh=True).
-0001ccb0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0001ccc0: 6572 7445 7175 616c 2863 6f6e 7465 6e74  ertEqual(content
-0001ccd0: 2c20 7b27 666f 6f27 3a20 2772 6566 7265  , {'foo': 'refre
-0001cce0: 7368 6564 277d 290a 0a20 2020 2020 2020  shed'})..       
-0001ccf0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0001cd00: 6c28 6661 6b65 5f73 6372 6970 745f 6361  l(fake_script_ca
-0001cd10: 6c6c 7328 7365 6c66 2c20 636c 6561 723d  lls(self, clear=
-0001cd20: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
-0001cd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cd40: 5b5b 2773 6563 7265 742d 6765 7427 2c20  [['secret-get', 
-0001cd50: 2773 6563 7265 743a 7927 2c20 272d 2d72  'secret:y', '--r
-0001cd60: 6566 7265 7368 272c 2027 2d2d 666f 726d  efresh', '--form
-0001cd70: 6174 3d6a 736f 6e27 5d5d 290a 0a20 2020  at=json']])..   
-0001cd80: 2064 6566 2074 6573 745f 6765 745f 636f   def test_get_co
-0001cd90: 6e74 656e 745f 756e 6361 6368 6564 2873  ntent_uncached(s
-0001cda0: 656c 6629 3a0a 2020 2020 2020 2020 6661  elf):.        fa
-0001cdb0: 6b65 5f73 6372 6970 7428 7365 6c66 2c20  ke_script(self, 
-0001cdc0: 2773 6563 7265 742d 6765 7427 2c20 2222  'secret-get', ""
-0001cdd0: 2265 6368 6f20 277b 2266 6f6f 223a 2022  "echo '{"foo": "
-0001cde0: 6e6f 7463 6163 6865 6422 7d27 2222 2229  notcached"}'""")
-0001cdf0: 0a0a 2020 2020 2020 2020 7365 6372 6574  ..        secret
-0001ce00: 203d 2073 656c 662e 6d61 6b65 5f73 6563   = self.make_sec
-0001ce10: 7265 7428 6964 3d27 7a27 290a 2020 2020  ret(id='z').    
-0001ce20: 2020 2020 636f 6e74 656e 7420 3d20 7365      content = se
-0001ce30: 6372 6574 2e67 6574 5f63 6f6e 7465 6e74  cret.get_content
-0001ce40: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0001ce50: 6173 7365 7274 4571 7561 6c28 636f 6e74  assertEqual(cont
-0001ce60: 656e 742c 207b 2766 6f6f 273a 2027 6e6f  ent, {'foo': 'no
-0001ce70: 7463 6163 6865 6427 7d29 0a0a 2020 2020  tcached'})..    
-0001ce80: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0001ce90: 7175 616c 2866 616b 655f 7363 7269 7074  qual(fake_script
-0001cea0: 5f63 616c 6c73 2873 656c 662c 2063 6c65  _calls(self, cle
-0001ceb0: 6172 3d54 7275 6529 2c0a 2020 2020 2020  ar=True),.      
-0001cec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ced0: 2020 205b 5b27 7365 6372 6574 2d67 6574     [['secret-get
-0001cee0: 272c 2027 7365 6372 6574 3a7a 272c 2027  ', 'secret:z', '
-0001cef0: 2d2d 666f 726d 6174 3d6a 736f 6e27 5d5d  --format=json']]
-0001cf00: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-0001cf10: 7065 656b 5f63 6f6e 7465 6e74 2873 656c  peek_content(sel
-0001cf20: 6629 3a0a 2020 2020 2020 2020 6661 6b65  f):.        fake
-0001cf30: 5f73 6372 6970 7428 7365 6c66 2c20 2773  _script(self, 's
-0001cf40: 6563 7265 742d 6765 7427 2c20 2222 2265  ecret-get', """e
-0001cf50: 6368 6f20 277b 2266 6f6f 223a 2022 7065  cho '{"foo": "pe
-0001cf60: 656b 6564 227d 2722 2222 290a 0a20 2020  eked"}'""")..   
-0001cf70: 2020 2020 2073 6563 7265 7420 3d20 7365       secret = se
-0001cf80: 6c66 2e6d 616b 655f 7365 6372 6574 2869  lf.make_secret(i
-0001cf90: 643d 2761 272c 206c 6162 656c 3d27 6227  d='a', label='b'
-0001cfa0: 290a 2020 2020 2020 2020 636f 6e74 656e  ).        conten
-0001cfb0: 7420 3d20 7365 6372 6574 2e70 6565 6b5f  t = secret.peek_
-0001cfc0: 636f 6e74 656e 7428 290a 2020 2020 2020  content().      
-0001cfd0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0001cfe0: 616c 2863 6f6e 7465 6e74 2c20 7b27 666f  al(content, {'fo
-0001cff0: 6f27 3a20 2770 6565 6b65 6427 7d29 0a0a  o': 'peeked'})..
-0001d000: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0001d010: 6572 7445 7175 616c 2866 616b 655f 7363  ertEqual(fake_sc
-0001d020: 7269 7074 5f63 616c 6c73 2873 656c 662c  ript_calls(self,
-0001d030: 2063 6c65 6172 3d54 7275 6529 2c0a 2020   clear=True),.  
-0001d040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d050: 2020 2020 2020 205b 5b27 7365 6372 6574         [['secret
-0001d060: 2d67 6574 272c 2027 7365 6372 6574 3a61  -get', 'secret:a
-0001d070: 272c 2027 2d2d 6c61 6265 6c27 2c20 2762  ', '--label', 'b
-0001d080: 272c 2027 2d2d 7065 656b 272c 2027 2d2d  ', '--peek', '--
-0001d090: 666f 726d 6174 3d6a 736f 6e27 5d5d 290a  format=json']]).
-0001d0a0: 0a20 2020 2064 6566 2074 6573 745f 6765  .    def test_ge
-0001d0b0: 745f 696e 666f 2873 656c 6629 3a0a 2020  t_info(self):.  
-0001d0c0: 2020 2020 2020 6661 6b65 5f73 6372 6970        fake_scrip
-0001d0d0: 7428 7365 6c66 2c20 2773 6563 7265 742d  t(self, 'secret-
-0001d0e0: 696e 666f 2d67 6574 272c 2022 2222 6563  info-get', """ec
-0001d0f0: 686f 2027 7b22 7822 3a20 7b22 6c61 6265  ho '{"x": {"labe
-0001d100: 6c22 3a20 2279 222c 2022 7265 7669 7369  l": "y", "revisi
-0001d110: 6f6e 223a 2037 7d7d 2722 2222 290a 0a20  on": 7}}'""").. 
-0001d120: 2020 2020 2020 2023 2053 6563 7265 7420         # Secret 
-0001d130: 7769 7468 2049 4420 6f6e 6c79 0a20 2020  with ID only.   
-0001d140: 2020 2020 2073 6563 7265 7420 3d20 7365       secret = se
-0001d150: 6c66 2e6d 616b 655f 7365 6372 6574 2869  lf.make_secret(i
-0001d160: 643d 2778 2729 0a20 2020 2020 2020 2069  d='x').        i
-0001d170: 6e66 6f20 3d20 7365 6372 6574 2e67 6574  nfo = secret.get
-0001d180: 5f69 6e66 6f28 290a 2020 2020 2020 2020  _info().        
-0001d190: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0001d1a0: 2869 6e66 6f2e 6964 2c20 2773 6563 7265  (info.id, 'secre
-0001d1b0: 743a 7827 290a 2020 2020 2020 2020 7365  t:x').        se
-0001d1c0: 6c66 2e61 7373 6572 7445 7175 616c 2869  lf.assertEqual(i
-0001d1d0: 6e66 6f2e 6c61 6265 6c2c 2027 7927 290a  nfo.label, 'y').
-0001d1e0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0001d1f0: 6572 7445 7175 616c 2869 6e66 6f2e 7265  ertEqual(info.re
-0001d200: 7669 7369 6f6e 2c20 3729 0a0a 2020 2020  vision, 7)..    
-0001d210: 2020 2020 2320 5365 6372 6574 2077 6974      # Secret wit
-0001d220: 6820 6c61 6265 6c20 6f6e 6c79 0a20 2020  h label only.   
-0001d230: 2020 2020 2073 6563 7265 7420 3d20 7365       secret = se
-0001d240: 6c66 2e6d 616b 655f 7365 6372 6574 286c  lf.make_secret(l
-0001d250: 6162 656c 3d27 7927 290a 2020 2020 2020  abel='y').      
-0001d260: 2020 696e 666f 203d 2073 6563 7265 742e    info = secret.
-0001d270: 6765 745f 696e 666f 2829 0a20 2020 2020  get_info().     
-0001d280: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0001d290: 7561 6c28 696e 666f 2e69 642c 2027 7365  ual(info.id, 'se
-0001d2a0: 6372 6574 3a78 2729 0a20 2020 2020 2020  cret:x').       
-0001d2b0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0001d2c0: 6c28 696e 666f 2e6c 6162 656c 2c20 2779  l(info.label, 'y
-0001d2d0: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-0001d2e0: 6173 7365 7274 4571 7561 6c28 696e 666f  assertEqual(info
-0001d2f0: 2e72 6576 6973 696f 6e2c 2037 290a 0a20  .revision, 7).. 
-0001d300: 2020 2020 2020 2023 2053 6563 7265 7420         # Secret 
-0001d310: 7769 7468 2049 4420 616e 6420 6c61 6265  with ID and labe
-0001d320: 6c0a 2020 2020 2020 2020 7365 6372 6574  l.        secret
-0001d330: 203d 2073 656c 662e 6d61 6b65 5f73 6563   = self.make_sec
-0001d340: 7265 7428 6964 3d27 7827 2c20 6c61 6265  ret(id='x', labe
-0001d350: 6c3d 2779 2729 0a20 2020 2020 2020 2069  l='y').        i
-0001d360: 6e66 6f20 3d20 7365 6372 6574 2e67 6574  nfo = secret.get
-0001d370: 5f69 6e66 6f28 290a 2020 2020 2020 2020  _info().        
-0001d380: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0001d390: 2869 6e66 6f2e 6964 2c20 2773 6563 7265  (info.id, 'secre
-0001d3a0: 743a 7827 290a 2020 2020 2020 2020 7365  t:x').        se
-0001d3b0: 6c66 2e61 7373 6572 7445 7175 616c 2869  lf.assertEqual(i
-0001d3c0: 6e66 6f2e 6c61 6265 6c2c 2027 7927 290a  nfo.label, 'y').
-0001d3d0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0001d3e0: 6572 7445 7175 616c 2869 6e66 6f2e 7265  ertEqual(info.re
-0001d3f0: 7669 7369 6f6e 2c20 3729 0a0a 2020 2020  vision, 7)..    
-0001d400: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0001d410: 7175 616c 280a 2020 2020 2020 2020 2020  qual(.          
-0001d420: 2020 6661 6b65 5f73 6372 6970 745f 6361    fake_script_ca
-0001d430: 6c6c 7328 7365 6c66 2c20 636c 6561 723d  lls(self, clear=
-0001d440: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
-0001d450: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-0001d460: 2020 2020 205b 2773 6563 7265 742d 696e       ['secret-in
-0001d470: 666f 2d67 6574 272c 2027 7365 6372 6574  fo-get', 'secret
-0001d480: 3a78 272c 2027 2d2d 666f 726d 6174 3d6a  :x', '--format=j
-0001d490: 736f 6e27 5d2c 0a20 2020 2020 2020 2020  son'],.         
-0001d4a0: 2020 2020 2020 205b 2773 6563 7265 742d         ['secret-
-0001d4b0: 696e 666f 2d67 6574 272c 2027 2d2d 6c61  info-get', '--la
-0001d4c0: 6265 6c27 2c20 2779 272c 2027 2d2d 666f  bel', 'y', '--fo
-0001d4d0: 726d 6174 3d6a 736f 6e27 5d2c 0a20 2020  rmat=json'],.   
-0001d4e0: 2020 2020 2020 2020 2020 2020 205b 2773               ['s
-0001d4f0: 6563 7265 742d 696e 666f 2d67 6574 272c  ecret-info-get',
-0001d500: 2027 7365 6372 6574 3a78 272c 2027 2d2d   'secret:x', '--
-0001d510: 666f 726d 6174 3d6a 736f 6e27 5d2c 0a20  format=json'],. 
-0001d520: 2020 2020 2020 2020 2020 205d 290a 0a20             ]).. 
-0001d530: 2020 2064 6566 2074 6573 745f 7365 745f     def test_set_
-0001d540: 636f 6e74 656e 7428 7365 6c66 293a 0a20  content(self):. 
-0001d550: 2020 2020 2020 2066 616b 655f 7363 7269         fake_scri
-0001d560: 7074 2873 656c 662c 2027 7365 6372 6574  pt(self, 'secret
-0001d570: 2d73 6574 272c 2022 2222 6578 6974 2030  -set', """exit 0
-0001d580: 2222 2229 0a20 2020 2020 2020 2066 616b  """).        fak
-0001d590: 655f 7363 7269 7074 2873 656c 662c 2027  e_script(self, '
-0001d5a0: 7365 6372 6574 2d69 6e66 6f2d 6765 7427  secret-info-get'
-0001d5b0: 2c20 2222 2265 6368 6f20 277b 227a 223a  , """echo '{"z":
-0001d5c0: 207b 226c 6162 656c 223a 2022 7922 2c20   {"label": "y", 
-0001d5d0: 2272 6576 6973 696f 6e22 3a20 377d 7d27  "revision": 7}}'
-0001d5e0: 2222 2229 0a0a 2020 2020 2020 2020 7365  """)..        se
-0001d5f0: 6372 6574 203d 2073 656c 662e 6d61 6b65  cret = self.make
-0001d600: 5f73 6563 7265 7428 6964 3d27 7827 290a  _secret(id='x').
-0001d610: 2020 2020 2020 2020 7365 6372 6574 2e73          secret.s
-0001d620: 6574 5f63 6f6e 7465 6e74 287b 2766 6f6f  et_content({'foo
-0001d630: 273a 2027 6261 7227 7d29 0a0a 2020 2020  ': 'bar'})..    
-0001d640: 2020 2020 2320 4966 2073 6563 7265 7420      # If secret 
-0001d650: 646f 6573 6e27 7420 6861 7665 2061 6e20  doesn't have an 
-0001d660: 4944 2c20 7765 276c 6c20 7275 6e20 7365  ID, we'll run se
-0001d670: 6372 6574 2d69 6e66 6f2d 6765 7420 746f  cret-info-get to
-0001d680: 2066 6574 6368 2069 740a 2020 2020 2020   fetch it.      
-0001d690: 2020 7365 6372 6574 203d 2073 656c 662e    secret = self.
-0001d6a0: 6d61 6b65 5f73 6563 7265 7428 6c61 6265  make_secret(labe
-0001d6b0: 6c3d 2779 2729 0a20 2020 2020 2020 2073  l='y').        s
-0001d6c0: 656c 662e 6173 7365 7274 4973 4e6f 6e65  elf.assertIsNone
-0001d6d0: 2873 6563 7265 742e 6964 290a 2020 2020  (secret.id).    
-0001d6e0: 2020 2020 7365 6372 6574 2e73 6574 5f63      secret.set_c
-0001d6f0: 6f6e 7465 6e74 287b 2762 6172 273a 2027  ontent({'bar': '
-0001d700: 666f 6f27 7d29 0a20 2020 2020 2020 2073  foo'}).        s
-0001d710: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0001d720: 7365 6372 6574 2e69 642c 2027 7365 6372  secret.id, 'secr
-0001d730: 6574 3a7a 2729 0a0a 2020 2020 2020 2020  et:z')..        
-0001d740: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
-0001d750: 5261 6973 6573 2856 616c 7565 4572 726f  Raises(ValueErro
-0001d760: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-0001d770: 7365 6372 6574 2e73 6574 5f63 6f6e 7465  secret.set_conte
-0001d780: 6e74 287b 2773 273a 2027 7427 7d29 2020  nt({'s': 't'})  
-0001d790: 2320 656e 7375 7265 2069 7420 7661 6c69  # ensure it vali
-0001d7a0: 6461 7465 7320 636f 6e74 656e 7420 286b  dates content (k
-0001d7b0: 6579 2074 6f6f 2073 686f 7274 290a 0a20  ey too short).. 
-0001d7c0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0001d7d0: 7274 4571 7561 6c28 6661 6b65 5f73 6372  rtEqual(fake_scr
-0001d7e0: 6970 745f 6361 6c6c 7328 7365 6c66 2c20  ipt_calls(self, 
-0001d7f0: 636c 6561 723d 5472 7565 292c 205b 0a20  clear=True), [. 
-0001d800: 2020 2020 2020 2020 2020 205b 2773 6563             ['sec
-0001d810: 7265 742d 7365 7427 2c20 2773 6563 7265  ret-set', 'secre
-0001d820: 743a 7827 2c20 2766 6f6f 3d62 6172 275d  t:x', 'foo=bar']
-0001d830: 2c0a 2020 2020 2020 2020 2020 2020 5b27  ,.            ['
+0001a440: 5d29 0a0a 2020 2020 6465 6620 7465 7374  ])..    def test
+0001a450: 5f70 6c61 6e6e 6564 5f75 6e69 7473 2873  _planned_units(s
+0001a460: 656c 6629 3a0a 2020 2020 2020 2020 2320  elf):.        # 
+0001a470: 6e6f 2075 6e69 7473 0a20 2020 2020 2020  no units.       
+0001a480: 2066 616b 655f 7363 7269 7074 2873 656c   fake_script(sel
+0001a490: 662c 2027 676f 616c 2d73 7461 7465 272c  f, 'goal-state',
+0001a4a0: 2022 2222 0a65 6368 6f20 277b 2275 6e69   """.echo '{"uni
+0001a4b0: 7473 223a 7b7d 2c20 2272 656c 6174 696f  ts":{}, "relatio
+0001a4c0: 6e73 223a 7b7d 7d27 0a22 2222 290a 2020  ns":{}}'.""").  
+0001a4d0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0001a4e0: 7445 7175 616c 2873 656c 662e 6261 636b  tEqual(self.back
+0001a4f0: 656e 642e 706c 616e 6e65 645f 756e 6974  end.planned_unit
+0001a500: 7328 292c 2030 290a 0a20 2020 2020 2020  s(), 0)..       
+0001a510: 2023 206f 6e6c 7920 6163 7469 7665 2075   # only active u
+0001a520: 6e69 7473 0a20 2020 2020 2020 2066 616b  nits.        fak
+0001a530: 655f 7363 7269 7074 2873 656c 662c 2027  e_script(self, '
+0001a540: 676f 616c 2d73 7461 7465 272c 2022 2222  goal-state', """
+0001a550: 0a65 6368 6f20 277b 0a20 2020 2022 756e  .echo '{.    "un
+0001a560: 6974 7322 3a7b 0a20 2020 2020 2020 2022  its":{.        "
+0001a570: 6170 702f 3022 3a20 7b22 7374 6174 7573  app/0": {"status
+0001a580: 223a 2261 6374 6976 6522 2c22 7369 6e63  ":"active","sinc
+0001a590: 6522 3a22 3230 3233 2d30 352d 3233 2031  e":"2023-05-23 1
+0001a5a0: 373a 3035 3a30 355a 227d 2c0a 2020 2020  7:05:05Z"},.    
+0001a5b0: 2020 2020 2261 7070 2f31 223a 207b 2273      "app/1": {"s
+0001a5c0: 7461 7475 7322 3a22 6163 7469 7665 222c  tatus":"active",
+0001a5d0: 2273 696e 6365 223a 2232 3032 332d 3035  "since":"2023-05
+0001a5e0: 2d32 3320 3137 3a35 373a 3035 5a22 7d0a  -23 17:57:05Z"}.
+0001a5f0: 2020 2020 7d2c 0a20 2020 2022 7265 6c61      },.    "rela
+0001a600: 7469 6f6e 7322 3a20 7b7d 0a7d 2722 2222  tions": {}.}'"""
+0001a610: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0001a620: 7373 6572 7445 7175 616c 2873 656c 662e  ssertEqual(self.
+0001a630: 6261 636b 656e 642e 706c 616e 6e65 645f  backend.planned_
+0001a640: 756e 6974 7328 292c 2032 290a 0a20 2020  units(), 2)..   
+0001a650: 2020 2020 2023 2061 6374 6976 6520 616e       # active an
+0001a660: 6420 6479 696e 6720 756e 6974 730a 2020  d dying units.  
+0001a670: 2020 2020 2020 6661 6b65 5f73 6372 6970        fake_scrip
+0001a680: 7428 7365 6c66 2c20 2767 6f61 6c2d 7374  t(self, 'goal-st
+0001a690: 6174 6527 2c20 2222 220a 6563 686f 2027  ate', """.echo '
+0001a6a0: 7b0a 2020 2020 2275 6e69 7473 223a 7b0a  {.    "units":{.
+0001a6b0: 2020 2020 2020 2020 2261 7070 2f30 223a          "app/0":
+0001a6c0: 207b 2273 7461 7475 7322 3a22 6163 7469   {"status":"acti
+0001a6d0: 7665 222c 2273 696e 6365 223a 2232 3032  ve","since":"202
+0001a6e0: 332d 3035 2d32 3320 3137 3a30 353a 3035  3-05-23 17:05:05
+0001a6f0: 5a22 7d2c 0a20 2020 2020 2020 2022 6170  Z"},.        "ap
+0001a700: 702f 3122 3a20 7b22 7374 6174 7573 223a  p/1": {"status":
+0001a710: 2264 7969 6e67 222c 2273 696e 6365 223a  "dying","since":
+0001a720: 2232 3032 332d 3035 2d32 3320 3137 3a35  "2023-05-23 17:5
+0001a730: 373a 3035 5a22 7d0a 2020 2020 7d2c 0a20  7:05Z"}.    },. 
+0001a740: 2020 2022 7265 6c61 7469 6f6e 7322 3a20     "relations": 
+0001a750: 7b7d 0a7d 2722 2222 290a 2020 2020 2020  {}.}'""").      
+0001a760: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0001a770: 616c 2873 656c 662e 6261 636b 656e 642e  al(self.backend.
+0001a780: 706c 616e 6e65 645f 756e 6974 7328 292c  planned_units(),
+0001a790: 2031 290a 0a0a 636c 6173 7320 5465 7374   1)...class Test
+0001a7a0: 4c61 7a79 4d61 7070 696e 6728 756e 6974  LazyMapping(unit
+0001a7b0: 7465 7374 2e54 6573 7443 6173 6529 3a0a  test.TestCase):.
+0001a7c0: 0a20 2020 2064 6566 2074 6573 745f 696e  .    def test_in
+0001a7d0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+0001a7e0: 2020 2020 2020 2020 6c6f 6164 6564 203d          loaded =
+0001a7f0: 205b 5d0a 0a20 2020 2020 2020 2063 6c61   []..        cla
+0001a800: 7373 204d 794c 617a 794d 6170 286f 7073  ss MyLazyMap(ops
+0001a810: 2e4c 617a 794d 6170 7069 6e67 293a 0a20  .LazyMapping):. 
+0001a820: 2020 2020 2020 2020 2020 2064 6566 205f             def _
+0001a830: 6c6f 6164 2873 656c 6629 3a0a 2020 2020  load(self):.    
+0001a840: 2020 2020 2020 2020 2020 2020 6c6f 6164              load
+0001a850: 6564 2e61 7070 656e 6428 3129 0a20 2020  ed.append(1).   
+0001a860: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0001a870: 7572 6e20 7b27 666f 6f27 3a20 2762 6172  urn {'foo': 'bar
+0001a880: 277d 0a0a 2020 2020 2020 2020 6d61 7020  '}..        map 
+0001a890: 3d20 4d79 4c61 7a79 4d61 7028 290a 2020  = MyLazyMap().  
+0001a8a0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0001a8b0: 7445 7175 616c 286d 6170 5b27 666f 6f27  tEqual(map['foo'
+0001a8c0: 5d2c 2027 6261 7227 290a 2020 2020 2020  ], 'bar').      
+0001a8d0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0001a8e0: 616c 286c 6f61 6465 642c 205b 315d 290a  al(loaded, [1]).
+0001a8f0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0001a900: 6572 7445 7175 616c 286d 6170 5b27 666f  ertEqual(map['fo
+0001a910: 6f27 5d2c 2027 6261 7227 290a 2020 2020  o'], 'bar').    
+0001a920: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0001a930: 7175 616c 286c 6f61 6465 642c 205b 315d  qual(loaded, [1]
+0001a940: 290a 2020 2020 2020 2020 6d61 702e 5f69  ).        map._i
+0001a950: 6e76 616c 6964 6174 6528 290a 2020 2020  nvalidate().    
+0001a960: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0001a970: 7175 616c 286d 6170 5b27 666f 6f27 5d2c  qual(map['foo'],
+0001a980: 2027 6261 7227 290a 2020 2020 2020 2020   'bar').        
+0001a990: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0001a9a0: 286c 6f61 6465 642c 205b 312c 2031 5d29  (loaded, [1, 1])
+0001a9b0: 0a0a 0a63 6c61 7373 2054 6573 7453 6563  ...class TestSec
+0001a9c0: 7265 7473 2875 6e69 7474 6573 742e 5465  rets(unittest.Te
+0001a9d0: 7374 4361 7365 293a 0a20 2020 2064 6566  stCase):.    def
+0001a9e0: 2073 6574 5570 2873 656c 6629 3a0a 2020   setUp(self):.  
+0001a9f0: 2020 2020 2020 7365 6c66 2e6d 6f64 656c        self.model
+0001aa00: 203d 206f 7073 2e4d 6f64 656c 286f 7073   = ops.Model(ops
+0001aa10: 2e43 6861 726d 4d65 7461 2829 2c20 5f4d  .CharmMeta(), _M
+0001aa20: 6f64 656c 4261 636b 656e 6428 276d 7961  odelBackend('mya
+0001aa30: 7070 2f30 2729 290a 2020 2020 2020 2020  pp/0')).        
+0001aa40: 7365 6c66 2e61 7070 203d 2073 656c 662e  self.app = self.
+0001aa50: 6d6f 6465 6c2e 6170 700a 2020 2020 2020  model.app.      
+0001aa60: 2020 7365 6c66 2e75 6e69 7420 3d20 7365    self.unit = se
+0001aa70: 6c66 2e6d 6f64 656c 2e75 6e69 740a 0a20  lf.model.unit.. 
+0001aa80: 2020 2064 6566 2074 6573 745f 6170 705f     def test_app_
+0001aa90: 6164 645f 7365 6372 6574 5f73 696d 706c  add_secret_simpl
+0001aaa0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+0001aab0: 2066 616b 655f 7363 7269 7074 2873 656c   fake_script(sel
+0001aac0: 662c 2027 7365 6372 6574 2d61 6464 272c  f, 'secret-add',
+0001aad0: 2027 6563 686f 2073 6563 7265 743a 3132   'echo secret:12
+0001aae0: 3327 290a 0a20 2020 2020 2020 2073 6563  3')..        sec
+0001aaf0: 7265 7420 3d20 7365 6c66 2e61 7070 2e61  ret = self.app.a
+0001ab00: 6464 5f73 6563 7265 7428 7b27 666f 6f27  dd_secret({'foo'
+0001ab10: 3a20 2778 277d 290a 2020 2020 2020 2020  : 'x'}).        
+0001ab20: 7365 6c66 2e61 7373 6572 7449 7349 6e73  self.assertIsIns
+0001ab30: 7461 6e63 6528 7365 6372 6574 2c20 6f70  tance(secret, op
+0001ab40: 732e 5365 6372 6574 290a 2020 2020 2020  s.Secret).      
+0001ab50: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0001ab60: 616c 2873 6563 7265 742e 6964 2c20 2773  al(secret.id, 's
+0001ab70: 6563 7265 743a 3132 3327 290a 2020 2020  ecret:123').    
+0001ab80: 2020 2020 7365 6c66 2e61 7373 6572 7449      self.assertI
+0001ab90: 734e 6f6e 6528 7365 6372 6574 2e6c 6162  sNone(secret.lab
+0001aba0: 656c 290a 0a20 2020 2020 2020 2073 656c  el)..        sel
+0001abb0: 662e 6173 7365 7274 4571 7561 6c28 6661  f.assertEqual(fa
+0001abc0: 6b65 5f73 6372 6970 745f 6361 6c6c 7328  ke_script_calls(
+0001abd0: 7365 6c66 2c20 636c 6561 723d 5472 7565  self, clear=True
+0001abe0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0001abf0: 2020 2020 2020 2020 2020 2020 5b5b 2773              [['s
+0001ac00: 6563 7265 742d 6164 6427 2c20 272d 2d6f  ecret-add', '--o
+0001ac10: 776e 6572 272c 2027 6170 706c 6963 6174  wner', 'applicat
+0001ac20: 696f 6e27 2c20 2766 6f6f 3d78 275d 5d29  ion', 'foo=x']])
+0001ac30: 0a0a 2020 2020 6465 6620 7465 7374 5f61  ..    def test_a
+0001ac40: 7070 5f61 6464 5f73 6563 7265 745f 6172  pp_add_secret_ar
+0001ac50: 6773 2873 656c 6629 3a0a 2020 2020 2020  gs(self):.      
+0001ac60: 2020 6661 6b65 5f73 6372 6970 7428 7365    fake_script(se
+0001ac70: 6c66 2c20 2773 6563 7265 742d 6164 6427  lf, 'secret-add'
+0001ac80: 2c20 2765 6368 6f20 7365 6372 6574 3a32  , 'echo secret:2
+0001ac90: 3334 2729 0a0a 2020 2020 2020 2020 6578  34')..        ex
+0001aca0: 7069 7265 203d 2064 6174 6574 696d 652e  pire = datetime.
+0001acb0: 6461 7465 7469 6d65 2832 3032 322c 2031  datetime(2022, 1
+0001acc0: 322c 2039 2c20 3136 2c20 3137 2c20 3029  2, 9, 16, 17, 0)
+0001acd0: 0a20 2020 2020 2020 2073 6563 7265 7420  .        secret 
+0001ace0: 3d20 7365 6c66 2e61 7070 2e61 6464 5f73  = self.app.add_s
+0001acf0: 6563 7265 7428 7b27 666f 6f27 3a20 2778  ecret({'foo': 'x
+0001ad00: 272c 2027 6261 7227 3a20 2779 277d 2c20  ', 'bar': 'y'}, 
+0001ad10: 6c61 6265 6c3d 276c 626c 272c 2064 6573  label='lbl', des
+0001ad20: 6372 6970 7469 6f6e 3d27 6465 7363 272c  cription='desc',
+0001ad30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ad40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad50: 2020 2020 2020 6578 7069 7265 3d65 7870        expire=exp
+0001ad60: 6972 652c 2072 6f74 6174 653d 6f70 732e  ire, rotate=ops.
+0001ad70: 5365 6372 6574 526f 7461 7465 2e48 4f55  SecretRotate.HOU
+0001ad80: 524c 5929 0a20 2020 2020 2020 2073 656c  RLY).        sel
+0001ad90: 662e 6173 7365 7274 4571 7561 6c28 7365  f.assertEqual(se
+0001ada0: 6372 6574 2e69 642c 2027 7365 6372 6574  cret.id, 'secret
+0001adb0: 3a32 3334 2729 0a20 2020 2020 2020 2073  :234').        s
+0001adc0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001add0: 7365 6372 6574 2e6c 6162 656c 2c20 276c  secret.label, 'l
+0001ade0: 626c 2729 0a20 2020 2020 2020 2073 656c  bl').        sel
+0001adf0: 662e 6173 7365 7274 4571 7561 6c28 7365  f.assertEqual(se
+0001ae00: 6372 6574 2e67 6574 5f63 6f6e 7465 6e74  cret.get_content
+0001ae10: 2829 2c20 7b27 666f 6f27 3a20 2778 272c  (), {'foo': 'x',
+0001ae20: 2027 6261 7227 3a20 2779 277d 290a 0a20   'bar': 'y'}).. 
+0001ae30: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001ae40: 7274 4571 7561 6c28 6661 6b65 5f73 6372  rtEqual(fake_scr
+0001ae50: 6970 745f 6361 6c6c 7328 7365 6c66 2c20  ipt_calls(self, 
+0001ae60: 636c 6561 723d 5472 7565 292c 0a20 2020  clear=True),.   
+0001ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae80: 2020 2020 2020 5b5b 2773 6563 7265 742d        [['secret-
+0001ae90: 6164 6427 2c20 272d 2d6c 6162 656c 272c  add', '--label',
+0001aea0: 2027 6c62 6c27 2c20 272d 2d64 6573 6372   'lbl', '--descr
+0001aeb0: 6970 7469 6f6e 272c 2027 6465 7363 272c  iption', 'desc',
+0001aec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001aed0: 2020 2020 2020 2020 2020 2020 272d 2d65              '--e
+0001aee0: 7870 6972 6527 2c20 2732 3032 322d 3132  xpire', '2022-12
+0001aef0: 2d30 3954 3136 3a31 373a 3030 272c 2027  -09T16:17:00', '
+0001af00: 2d2d 726f 7461 7465 272c 2027 686f 7572  --rotate', 'hour
+0001af10: 6c79 272c 0a20 2020 2020 2020 2020 2020  ly',.           
+0001af20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af30: 272d 2d6f 776e 6572 272c 2027 6170 706c  '--owner', 'appl
+0001af40: 6963 6174 696f 6e27 2c20 2766 6f6f 3d78  ication', 'foo=x
+0001af50: 272c 2027 6261 723d 7927 5d5d 290a 0a20  ', 'bar=y']]).. 
+0001af60: 2020 2064 6566 2074 6573 745f 756e 6974     def test_unit
+0001af70: 5f61 6464 5f73 6563 7265 745f 7369 6d70  _add_secret_simp
+0001af80: 6c65 2873 656c 6629 3a0a 2020 2020 2020  le(self):.      
+0001af90: 2020 6661 6b65 5f73 6372 6970 7428 7365    fake_script(se
+0001afa0: 6c66 2c20 2773 6563 7265 742d 6164 6427  lf, 'secret-add'
+0001afb0: 2c20 2765 6368 6f20 7365 6372 6574 3a33  , 'echo secret:3
+0001afc0: 3435 2729 0a0a 2020 2020 2020 2020 7365  45')..        se
+0001afd0: 6372 6574 203d 2073 656c 662e 756e 6974  cret = self.unit
+0001afe0: 2e61 6464 5f73 6563 7265 7428 7b27 666f  .add_secret({'fo
+0001aff0: 6f27 3a20 2778 277d 290a 2020 2020 2020  o': 'x'}).      
+0001b000: 2020 7365 6c66 2e61 7373 6572 7449 7349    self.assertIsI
+0001b010: 6e73 7461 6e63 6528 7365 6372 6574 2c20  nstance(secret, 
+0001b020: 6f70 732e 5365 6372 6574 290a 2020 2020  ops.Secret).    
+0001b030: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0001b040: 7175 616c 2873 6563 7265 742e 6964 2c20  qual(secret.id, 
+0001b050: 2773 6563 7265 743a 3334 3527 290a 2020  'secret:345').  
+0001b060: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0001b070: 7449 734e 6f6e 6528 7365 6372 6574 2e6c  tIsNone(secret.l
+0001b080: 6162 656c 290a 0a20 2020 2020 2020 2073  abel)..        s
+0001b090: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001b0a0: 6661 6b65 5f73 6372 6970 745f 6361 6c6c  fake_script_call
+0001b0b0: 7328 7365 6c66 2c20 636c 6561 723d 5472  s(self, clear=Tr
+0001b0c0: 7565 292c 0a20 2020 2020 2020 2020 2020  ue),.           
+0001b0d0: 2020 2020 2020 2020 2020 2020 2020 5b5b                [[
+0001b0e0: 2773 6563 7265 742d 6164 6427 2c20 272d  'secret-add', '-
+0001b0f0: 2d6f 776e 6572 272c 2027 756e 6974 272c  -owner', 'unit',
+0001b100: 2027 666f 6f3d 7827 5d5d 290a 0a20 2020   'foo=x']])..   
+0001b110: 2064 6566 2074 6573 745f 756e 6974 5f61   def test_unit_a
+0001b120: 6464 5f73 6563 7265 745f 6172 6773 2873  dd_secret_args(s
+0001b130: 656c 6629 3a0a 2020 2020 2020 2020 6661  elf):.        fa
+0001b140: 6b65 5f73 6372 6970 7428 7365 6c66 2c20  ke_script(self, 
+0001b150: 2773 6563 7265 742d 6164 6427 2c20 2765  'secret-add', 'e
+0001b160: 6368 6f20 7365 6372 6574 3a34 3536 2729  cho secret:456')
+0001b170: 0a0a 2020 2020 2020 2020 6578 7069 7265  ..        expire
+0001b180: 203d 2064 6174 6574 696d 652e 6461 7465   = datetime.date
+0001b190: 7469 6d65 2832 3032 322c 2031 322c 2039  time(2022, 12, 9
+0001b1a0: 2c20 3136 2c20 3232 2c20 3029 0a20 2020  , 16, 22, 0).   
+0001b1b0: 2020 2020 2073 6563 7265 7420 3d20 7365       secret = se
+0001b1c0: 6c66 2e75 6e69 742e 6164 645f 7365 6372  lf.unit.add_secr
+0001b1d0: 6574 287b 2766 6f6f 273a 2027 7727 2c20  et({'foo': 'w', 
+0001b1e0: 2762 6172 273a 2027 7a27 7d2c 206c 6162  'bar': 'z'}, lab
+0001b1f0: 656c 3d27 6c32 272c 2064 6573 6372 6970  el='l2', descrip
+0001b200: 7469 6f6e 3d27 7879 7a27 2c0a 2020 2020  tion='xyz',.    
+0001b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b230: 2020 6578 7069 7265 3d65 7870 6972 652c    expire=expire,
+0001b240: 2072 6f74 6174 653d 6f70 732e 5365 6372   rotate=ops.Secr
+0001b250: 6574 526f 7461 7465 2e59 4541 524c 5929  etRotate.YEARLY)
+0001b260: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001b270: 7365 7274 4571 7561 6c28 7365 6372 6574  sertEqual(secret
+0001b280: 2e69 642c 2027 7365 6372 6574 3a34 3536  .id, 'secret:456
+0001b290: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+0001b2a0: 6173 7365 7274 4571 7561 6c28 7365 6372  assertEqual(secr
+0001b2b0: 6574 2e6c 6162 656c 2c20 276c 3227 290a  et.label, 'l2').
+0001b2c0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0001b2d0: 6572 7445 7175 616c 2873 6563 7265 742e  ertEqual(secret.
+0001b2e0: 6765 745f 636f 6e74 656e 7428 292c 207b  get_content(), {
+0001b2f0: 2766 6f6f 273a 2027 7727 2c20 2762 6172  'foo': 'w', 'bar
+0001b300: 273a 2027 7a27 7d29 0a0a 2020 2020 2020  ': 'z'})..      
+0001b310: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0001b320: 616c 2866 616b 655f 7363 7269 7074 5f63  al(fake_script_c
+0001b330: 616c 6c73 2873 656c 662c 2063 6c65 6172  alls(self, clear
+0001b340: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
+0001b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b360: 205b 5b27 7365 6372 6574 2d61 6464 272c   [['secret-add',
+0001b370: 2027 2d2d 6c61 6265 6c27 2c20 276c 3227   '--label', 'l2'
+0001b380: 2c20 272d 2d64 6573 6372 6970 7469 6f6e  , '--description
+0001b390: 272c 2027 7879 7a27 2c0a 2020 2020 2020  ', 'xyz',.      
+0001b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b3b0: 2020 2020 2027 2d2d 6578 7069 7265 272c       '--expire',
+0001b3c0: 2027 3230 3232 2d31 322d 3039 5431 363a   '2022-12-09T16:
+0001b3d0: 3232 3a30 3027 2c20 272d 2d72 6f74 6174  22:00', '--rotat
+0001b3e0: 6527 2c20 2779 6561 726c 7927 2c0a 2020  e', 'yearly',.  
+0001b3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b400: 2020 2020 2020 2020 2027 2d2d 6f77 6e65           '--owne
+0001b410: 7227 2c20 2775 6e69 7427 2c20 2766 6f6f  r', 'unit', 'foo
+0001b420: 3d77 272c 2027 6261 723d 7a27 5d5d 290a  =w', 'bar=z']]).
+0001b430: 0a20 2020 2064 6566 2074 6573 745f 756e  .    def test_un
+0001b440: 6974 5f61 6464 5f73 6563 7265 745f 6572  it_add_secret_er
+0001b450: 726f 7273 2873 656c 6629 3a0a 2020 2020  rors(self):.    
+0001b460: 2020 2020 2320 4164 6469 7469 6f6e 616c      # Additional
+0001b470: 2061 6464 5f73 6563 7265 7420 7465 7374   add_secret test
+0001b480: 7320 6172 6520 646f 6e65 2069 6e20 5465  s are done in Te
+0001b490: 7374 4170 706c 6963 6174 696f 6e0a 2020  stApplication.  
+0001b4a0: 2020 2020 2020 6572 726f 7273 203d 205b        errors = [
+0001b4b0: 0a20 2020 2020 2020 2020 2020 2028 7b27  .            ({'
+0001b4c0: 7879 273a 2027 6261 7227 7d2c 207b 7d2c  xy': 'bar'}, {},
+0001b4d0: 2056 616c 7565 4572 726f 7229 2c0a 2020   ValueError),.  
+0001b4e0: 2020 2020 2020 2020 2020 287b 2766 6f6f            ({'foo
+0001b4f0: 273a 2027 7827 7d2c 207b 2765 7870 6972  ': 'x'}, {'expir
+0001b500: 6527 3a20 377d 2c20 5479 7065 4572 726f  e': 7}, TypeErro
+0001b510: 7229 2c0a 2020 2020 2020 2020 5d0a 2020  r),.        ].  
+0001b520: 2020 2020 2020 666f 7220 636f 6e74 656e        for conten
+0001b530: 742c 206b 7761 7267 732c 2065 7863 5f74  t, kwargs, exc_t
+0001b540: 7970 6520 696e 2065 7272 6f72 733a 0a20  ype in errors:. 
+0001b550: 2020 2020 2020 2020 2020 206d 7367 203d             msg =
+0001b560: 2066 2765 7870 6563 7465 6420 7b65 7863   f'expected {exc
+0001b570: 5f74 7970 652e 5f5f 6e61 6d65 5f5f 7d20  _type.__name__} 
+0001b580: 7768 656e 2061 6464 696e 6720 7365 6372  when adding secr
+0001b590: 6574 2063 6f6e 7465 6e74 207b 636f 6e74  et content {cont
+0001b5a0: 656e 747d 270a 2020 2020 2020 2020 2020  ent}'.          
+0001b5b0: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
+0001b5c0: 7274 5261 6973 6573 2865 7863 5f74 7970  rtRaises(exc_typ
+0001b5d0: 652c 206d 7367 3d6d 7367 293a 0a20 2020  e, msg=msg):.   
+0001b5e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001b5f0: 662e 756e 6974 2e61 6464 5f73 6563 7265  f.unit.add_secre
+0001b600: 7428 636f 6e74 656e 742c 202a 2a6b 7761  t(content, **kwa
+0001b610: 7267 7329 0a0a 2020 2020 6465 6620 7465  rgs)..    def te
+0001b620: 7374 5f61 6464 5f73 6563 7265 745f 6572  st_add_secret_er
+0001b630: 726f 7273 2873 656c 6629 3a0a 2020 2020  rors(self):.    
+0001b640: 2020 2020 6572 726f 7273 203d 205b 0a20      errors = [. 
+0001b650: 2020 2020 2020 2020 2020 2023 2049 6e76             # Inv
+0001b660: 616c 6964 2063 6f6e 7465 6e74 2064 6963  alid content dic
+0001b670: 7420 6f72 2074 7970 6573 0a20 2020 2020  t or types.     
+0001b680: 2020 2020 2020 2028 4e6f 6e65 2c20 7b7d         (None, {}
+0001b690: 2c20 5479 7065 4572 726f 7229 2c0a 2020  , TypeError),.  
+0001b6a0: 2020 2020 2020 2020 2020 287b 7d2c 207b            ({}, {
+0001b6b0: 7d2c 2056 616c 7565 4572 726f 7229 2c0a  }, ValueError),.
+0001b6c0: 2020 2020 2020 2020 2020 2020 287b 6227              ({b'
+0001b6d0: 666f 6f27 2c20 2762 6172 277d 2c20 7b7d  foo', 'bar'}, {}
+0001b6e0: 2c20 5479 7065 4572 726f 7229 2c0a 2020  , TypeError),.  
+0001b6f0: 2020 2020 2020 2020 2020 287b 333a 2027            ({3: '
+0001b700: 6261 7227 7d2c 207b 7d2c 2054 7970 6545  bar'}, {}, TypeE
+0001b710: 7272 6f72 292c 0a20 2020 2020 2020 2020  rror),.         
+0001b720: 2020 2028 7b27 666f 6f27 3a20 312c 2027     ({'foo': 1, '
+0001b730: 6261 7227 3a20 327d 2c20 7b7d 2c20 5479  bar': 2}, {}, Ty
+0001b740: 7065 4572 726f 7229 2c0a 2020 2020 2020  peError),.      
+0001b750: 2020 2020 2020 2320 496e 7661 6c69 6420        # Invalid 
+0001b760: 636f 6e74 656e 7420 6b65 7973 0a20 2020  content keys.   
+0001b770: 2020 2020 2020 2020 2028 7b27 7879 273a           ({'xy':
+0001b780: 2027 6261 7227 7d2c 207b 7d2c 2056 616c   'bar'}, {}, Val
+0001b790: 7565 4572 726f 7229 2c0a 2020 2020 2020  ueError),.      
+0001b7a0: 2020 2020 2020 287b 2746 4f4f 273a 2027        ({'FOO': '
+0001b7b0: 6261 7227 7d2c 207b 7d2c 2056 616c 7565  bar'}, {}, Value
+0001b7c0: 4572 726f 7229 2c0a 2020 2020 2020 2020  Error),.        
+0001b7d0: 2020 2020 287b 2766 6f6f 2d27 3a20 2762      ({'foo-': 'b
+0001b7e0: 6172 277d 2c20 7b7d 2c20 5661 6c75 6545  ar'}, {}, ValueE
+0001b7f0: 7272 6f72 292c 0a20 2020 2020 2020 2020  rror),.         
+0001b800: 2020 2028 7b27 2d66 6f6f 273a 2027 6261     ({'-foo': 'ba
+0001b810: 7227 7d2c 207b 7d2c 2056 616c 7565 4572  r'}, {}, ValueEr
+0001b820: 726f 7229 2c0a 2020 2020 2020 2020 2020  ror),.          
+0001b830: 2020 2320 496e 7661 6c69 6420 2265 7870    # Invalid "exp
+0001b840: 6972 6522 2074 7970 650a 2020 2020 2020  ire" type.      
+0001b850: 2020 2020 2020 287b 2766 6f6f 273a 2027        ({'foo': '
+0001b860: 7827 7d2c 207b 2765 7870 6972 6527 3a20  x'}, {'expire': 
+0001b870: 377d 2c20 5479 7065 4572 726f 7229 2c0a  7}, TypeError),.
+0001b880: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+0001b890: 2020 666f 7220 636f 6e74 656e 742c 206b    for content, k
+0001b8a0: 7761 7267 732c 2065 7863 5f74 7970 6520  wargs, exc_type 
+0001b8b0: 696e 2065 7272 6f72 733a 0a20 2020 2020  in errors:.     
+0001b8c0: 2020 2020 2020 206d 7367 203d 2066 2765         msg = f'e
+0001b8d0: 7870 6563 7465 6420 7b65 7863 5f74 7970  xpected {exc_typ
+0001b8e0: 652e 5f5f 6e61 6d65 5f5f 7d20 7768 656e  e.__name__} when
+0001b8f0: 2061 6464 696e 6720 7365 6372 6574 2063   adding secret c
+0001b900: 6f6e 7465 6e74 207b 636f 6e74 656e 747d  ontent {content}
+0001b910: 270a 2020 2020 2020 2020 2020 2020 7769  '.            wi
+0001b920: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
+0001b930: 6973 6573 2865 7863 5f74 7970 652c 206d  ises(exc_type, m
+0001b940: 7367 3d6d 7367 293a 0a20 2020 2020 2020  sg=msg):.       
+0001b950: 2020 2020 2020 2020 2073 656c 662e 6170           self.ap
+0001b960: 702e 6164 645f 7365 6372 6574 2863 6f6e  p.add_secret(con
+0001b970: 7465 6e74 2c20 2a2a 6b77 6172 6773 290a  tent, **kwargs).
+0001b980: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0001b990: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
+0001b9a0: 6573 2865 7863 5f74 7970 652c 206d 7367  es(exc_type, msg
+0001b9b0: 3d6d 7367 293a 0a20 2020 2020 2020 2020  =msg):.         
+0001b9c0: 2020 2020 2020 2073 656c 662e 756e 6974         self.unit
+0001b9d0: 2e61 6464 5f73 6563 7265 7428 636f 6e74  .add_secret(cont
+0001b9e0: 656e 742c 202a 2a6b 7761 7267 7329 0a0a  ent, **kwargs)..
+0001b9f0: 2020 2020 6465 6620 7465 7374 5f67 6574      def test_get
+0001ba00: 5f73 6563 7265 745f 6964 2873 656c 6629  _secret_id(self)
+0001ba10: 3a0a 2020 2020 2020 2020 6661 6b65 5f73  :.        fake_s
+0001ba20: 6372 6970 7428 7365 6c66 2c20 2773 6563  cript(self, 'sec
+0001ba30: 7265 742d 6765 7427 2c20 2222 2265 6368  ret-get', """ech
+0001ba40: 6f20 277b 2266 6f6f 223a 2022 6722 7d27  o '{"foo": "g"}'
+0001ba50: 2222 2229 0a0a 2020 2020 2020 2020 7365  """)..        se
+0001ba60: 6372 6574 203d 2073 656c 662e 6d6f 6465  cret = self.mode
+0001ba70: 6c2e 6765 745f 7365 6372 6574 2869 643d  l.get_secret(id=
+0001ba80: 2731 3233 2729 0a20 2020 2020 2020 2073  '123').        s
+0001ba90: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001baa0: 7365 6372 6574 2e69 642c 2027 7365 6372  secret.id, 'secr
+0001bab0: 6574 3a31 3233 2729 0a20 2020 2020 2020  et:123').       
+0001bac0: 2073 656c 662e 6173 7365 7274 4973 4e6f   self.assertIsNo
+0001bad0: 6e65 2873 6563 7265 742e 6c61 6265 6c29  ne(secret.label)
+0001bae0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001baf0: 7365 7274 4571 7561 6c28 7365 6372 6574  sertEqual(secret
+0001bb00: 2e67 6574 5f63 6f6e 7465 6e74 2829 2c20  .get_content(), 
+0001bb10: 7b27 666f 6f27 3a20 2767 277d 290a 0a20  {'foo': 'g'}).. 
+0001bb20: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001bb30: 7274 4571 7561 6c28 6661 6b65 5f73 6372  rtEqual(fake_scr
+0001bb40: 6970 745f 6361 6c6c 7328 7365 6c66 2c20  ipt_calls(self, 
+0001bb50: 636c 6561 723d 5472 7565 292c 0a20 2020  clear=True),.   
+0001bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bb70: 2020 2020 2020 5b5b 2773 6563 7265 742d        [['secret-
+0001bb80: 6765 7427 2c20 2773 6563 7265 743a 3132  get', 'secret:12
+0001bb90: 3327 2c20 272d 2d66 6f72 6d61 743d 6a73  3', '--format=js
+0001bba0: 6f6e 275d 5d29 0a0a 2020 2020 6465 6620  on']])..    def 
+0001bbb0: 7465 7374 5f67 6574 5f73 6563 7265 745f  test_get_secret_
+0001bbc0: 6c61 6265 6c28 7365 6c66 293a 0a20 2020  label(self):.   
+0001bbd0: 2020 2020 2066 616b 655f 7363 7269 7074       fake_script
+0001bbe0: 2873 656c 662c 2027 7365 6372 6574 2d67  (self, 'secret-g
+0001bbf0: 6574 272c 2022 2222 6563 686f 2027 7b22  et', """echo '{"
+0001bc00: 666f 6f22 3a20 2267 227d 2722 2222 290a  foo": "g"}'""").
+0001bc10: 0a20 2020 2020 2020 2073 6563 7265 7420  .        secret 
+0001bc20: 3d20 7365 6c66 2e6d 6f64 656c 2e67 6574  = self.model.get
+0001bc30: 5f73 6563 7265 7428 6c61 6265 6c3d 276c  _secret(label='l
+0001bc40: 626c 2729 0a20 2020 2020 2020 2073 656c  bl').        sel
+0001bc50: 662e 6173 7365 7274 4973 4e6f 6e65 2873  f.assertIsNone(s
+0001bc60: 6563 7265 742e 6964 290a 2020 2020 2020  ecret.id).      
+0001bc70: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0001bc80: 616c 2873 6563 7265 742e 6c61 6265 6c2c  al(secret.label,
+0001bc90: 2027 6c62 6c27 290a 2020 2020 2020 2020   'lbl').        
+0001bca0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0001bcb0: 2873 6563 7265 742e 6765 745f 636f 6e74  (secret.get_cont
+0001bcc0: 656e 7428 292c 207b 2766 6f6f 273a 2027  ent(), {'foo': '
+0001bcd0: 6727 7d29 0a0a 2020 2020 2020 2020 7365  g'})..        se
+0001bce0: 6c66 2e61 7373 6572 7445 7175 616c 2866  lf.assertEqual(f
+0001bcf0: 616b 655f 7363 7269 7074 5f63 616c 6c73  ake_script_calls
+0001bd00: 2873 656c 662c 2063 6c65 6172 3d54 7275  (self, clear=Tru
+0001bd10: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+0001bd20: 2020 2020 2020 2020 2020 2020 205b 5b27               [['
+0001bd30: 7365 6372 6574 2d67 6574 272c 2027 2d2d  secret-get', '--
+0001bd40: 6c61 6265 6c27 2c20 276c 626c 272c 2027  label', 'lbl', '
+0001bd50: 2d2d 666f 726d 6174 3d6a 736f 6e27 5d5d  --format=json']]
+0001bd60: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+0001bd70: 6765 745f 7365 6372 6574 5f69 645f 616e  get_secret_id_an
+0001bd80: 645f 6c61 6265 6c28 7365 6c66 293a 0a20  d_label(self):. 
+0001bd90: 2020 2020 2020 2066 616b 655f 7363 7269         fake_scri
+0001bda0: 7074 2873 656c 662c 2027 7365 6372 6574  pt(self, 'secret
+0001bdb0: 2d67 6574 272c 2022 2222 6563 686f 2027  -get', """echo '
+0001bdc0: 7b22 666f 6f22 3a20 2268 227d 2722 2222  {"foo": "h"}'"""
+0001bdd0: 290a 0a20 2020 2020 2020 2073 6563 7265  )..        secre
+0001bde0: 7420 3d20 7365 6c66 2e6d 6f64 656c 2e67  t = self.model.g
+0001bdf0: 6574 5f73 6563 7265 7428 6964 3d27 3132  et_secret(id='12
+0001be00: 3327 2c20 6c61 6265 6c3d 276c 2729 0a20  3', label='l'). 
+0001be10: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001be20: 7274 4571 7561 6c28 7365 6372 6574 2e69  rtEqual(secret.i
+0001be30: 642c 2027 7365 6372 6574 3a31 3233 2729  d, 'secret:123')
+0001be40: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001be50: 7365 7274 4571 7561 6c28 7365 6372 6574  sertEqual(secret
+0001be60: 2e6c 6162 656c 2c20 276c 2729 0a20 2020  .label, 'l').   
+0001be70: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001be80: 4571 7561 6c28 7365 6372 6574 2e67 6574  Equal(secret.get
+0001be90: 5f63 6f6e 7465 6e74 2829 2c20 7b27 666f  _content(), {'fo
+0001bea0: 6f27 3a20 2768 277d 290a 0a20 2020 2020  o': 'h'})..     
+0001beb0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0001bec0: 7561 6c28 6661 6b65 5f73 6372 6970 745f  ual(fake_script_
+0001bed0: 6361 6c6c 7328 7365 6c66 2c20 636c 6561  calls(self, clea
+0001bee0: 723d 5472 7565 292c 0a20 2020 2020 2020  r=True),.       
+0001bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bf00: 2020 5b5b 2773 6563 7265 742d 6765 7427    [['secret-get'
+0001bf10: 2c20 2773 6563 7265 743a 3132 3327 2c20  , 'secret:123', 
+0001bf20: 272d 2d6c 6162 656c 272c 2027 6c27 2c20  '--label', 'l', 
+0001bf30: 272d 2d66 6f72 6d61 743d 6a73 6f6e 275d  '--format=json']
+0001bf40: 5d29 0a0a 2020 2020 6465 6620 7465 7374  ])..    def test
+0001bf50: 5f67 6574 5f73 6563 7265 745f 6e6f 5f61  _get_secret_no_a
+0001bf60: 7267 7328 7365 6c66 293a 0a20 2020 2020  rgs(self):.     
+0001bf70: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
+0001bf80: 6572 7452 6169 7365 7328 5479 7065 4572  ertRaises(TypeEr
+0001bf90: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
+0001bfa0: 2020 7365 6c66 2e6d 6f64 656c 2e67 6574    self.model.get
+0001bfb0: 5f73 6563 7265 7428 290a 0a20 2020 2064  _secret()..    d
+0001bfc0: 6566 2074 6573 745f 6765 745f 7365 6372  ef test_get_secr
+0001bfd0: 6574 5f6e 6f74 5f66 6f75 6e64 2873 656c  et_not_found(sel
+0001bfe0: 6629 3a0a 2020 2020 2020 2020 7363 7269  f):.        scri
+0001bff0: 7074 203d 2022 2222 6563 686f 2027 4552  pt = """echo 'ER
+0001c000: 524f 5220 7365 6372 6574 2022 3132 3322  ROR secret "123"
+0001c010: 206e 6f74 2066 6f75 6e64 2720 3e26 323b   not found' >&2;
+0001c020: 2065 7869 7420 3122 2222 0a20 2020 2020   exit 1""".     
+0001c030: 2020 2066 616b 655f 7363 7269 7074 2873     fake_script(s
+0001c040: 656c 662c 2027 7365 6372 6574 2d67 6574  elf, 'secret-get
+0001c050: 272c 2073 6372 6970 7429 0a20 2020 2020  ', script).     
+0001c060: 2020 2066 616b 655f 7363 7269 7074 2873     fake_script(s
+0001c070: 656c 662c 2027 7365 6372 6574 2d69 6e66  elf, 'secret-inf
+0001c080: 6f2d 6765 7427 2c20 7363 7269 7074 290a  o-get', script).
+0001c090: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+0001c0a0: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
+0001c0b0: 6f70 732e 5365 6372 6574 4e6f 7446 6f75  ops.SecretNotFou
+0001c0c0: 6e64 4572 726f 7229 3a0a 2020 2020 2020  ndError):.      
+0001c0d0: 2020 2020 2020 7365 6c66 2e6d 6f64 656c        self.model
+0001c0e0: 2e67 6574 5f73 6563 7265 7428 6964 3d27  .get_secret(id='
+0001c0f0: 3132 3327 290a 0a20 2020 2064 6566 2074  123')..    def t
+0001c100: 6573 745f 6765 745f 7365 6372 6574 5f6f  est_get_secret_o
+0001c110: 7468 6572 5f65 7272 6f72 2873 656c 6629  ther_error(self)
+0001c120: 3a0a 2020 2020 2020 2020 7363 7269 7074  :.        script
+0001c130: 203d 2022 2222 6563 686f 2027 4552 524f   = """echo 'ERRO
+0001c140: 5220 6f74 6865 7220 6572 726f 7227 203e  R other error' >
+0001c150: 2632 3b20 6578 6974 2031 2222 220a 2020  &2; exit 1""".  
+0001c160: 2020 2020 2020 6661 6b65 5f73 6372 6970        fake_scrip
+0001c170: 7428 7365 6c66 2c20 2773 6563 7265 742d  t(self, 'secret-
+0001c180: 6765 7427 2c20 7363 7269 7074 290a 2020  get', script).  
+0001c190: 2020 2020 2020 6661 6b65 5f73 6372 6970        fake_scrip
+0001c1a0: 7428 7365 6c66 2c20 2773 6563 7265 742d  t(self, 'secret-
+0001c1b0: 696e 666f 2d67 6574 272c 2073 6372 6970  info-get', scrip
+0001c1c0: 7429 0a0a 2020 2020 2020 2020 7769 7468  t)..        with
+0001c1d0: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
+0001c1e0: 6573 286f 7073 2e4d 6f64 656c 4572 726f  es(ops.ModelErro
+0001c1f0: 7229 2061 7320 636d 3a0a 2020 2020 2020  r) as cm:.      
+0001c200: 2020 2020 2020 7365 6c66 2e6d 6f64 656c        self.model
+0001c210: 2e67 6574 5f73 6563 7265 7428 6964 3d27  .get_secret(id='
+0001c220: 3132 3327 290a 2020 2020 2020 2020 7365  123').        se
+0001c230: 6c66 2e61 7373 6572 744e 6f74 4973 496e  lf.assertNotIsIn
+0001c240: 7374 616e 6365 2863 6d2e 6578 6365 7074  stance(cm.except
+0001c250: 696f 6e2c 206f 7073 2e53 6563 7265 744e  ion, ops.SecretN
+0001c260: 6f74 466f 756e 6445 7272 6f72 290a 0a0a  otFoundError)...
+0001c270: 636c 6173 7320 5465 7374 5365 6372 6574  class TestSecret
+0001c280: 496e 666f 2875 6e69 7474 6573 742e 5465  Info(unittest.Te
+0001c290: 7374 4361 7365 293a 0a20 2020 2064 6566  stCase):.    def
+0001c2a0: 2074 6573 745f 696e 6974 2873 656c 6629   test_init(self)
+0001c2b0: 3a0a 2020 2020 2020 2020 696e 666f 203d  :.        info =
+0001c2c0: 206f 7073 2e53 6563 7265 7449 6e66 6f28   ops.SecretInfo(
+0001c2d0: 0a20 2020 2020 2020 2020 2020 2069 643d  .            id=
+0001c2e0: 2733 272c 0a20 2020 2020 2020 2020 2020  '3',.           
+0001c2f0: 206c 6162 656c 3d27 6c62 6c27 2c0a 2020   label='lbl',.  
+0001c300: 2020 2020 2020 2020 2020 7265 7669 7369            revisi
+0001c310: 6f6e 3d37 2c0a 2020 2020 2020 2020 2020  on=7,.          
+0001c320: 2020 6578 7069 7265 733d 6461 7465 7469    expires=dateti
+0001c330: 6d65 2e64 6174 6574 696d 6528 3230 3232  me.datetime(2022
+0001c340: 2c20 3132 2c20 392c 2031 342c 2031 302c  , 12, 9, 14, 10,
+0001c350: 2030 292c 0a20 2020 2020 2020 2020 2020   0),.           
+0001c360: 2072 6f74 6174 696f 6e3d 6f70 732e 5365   rotation=ops.Se
+0001c370: 6372 6574 526f 7461 7465 2e4d 4f4e 5448  cretRotate.MONTH
+0001c380: 4c59 2c0a 2020 2020 2020 2020 2020 2020  LY,.            
+0001c390: 726f 7461 7465 733d 6461 7465 7469 6d65  rotates=datetime
+0001c3a0: 2e64 6174 6574 696d 6528 3230 3233 2c20  .datetime(2023, 
+0001c3b0: 312c 2039 2c20 3134 2c20 3130 2c20 3029  1, 9, 14, 10, 0)
+0001c3c0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+0001c3d0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0001c3e0: 7175 616c 2869 6e66 6f2e 6964 2c20 2773  qual(info.id, 's
+0001c3f0: 6563 7265 743a 3327 290a 2020 2020 2020  ecret:3').      
+0001c400: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0001c410: 616c 2869 6e66 6f2e 6c61 6265 6c2c 2027  al(info.label, '
+0001c420: 6c62 6c27 290a 2020 2020 2020 2020 7365  lbl').        se
+0001c430: 6c66 2e61 7373 6572 7445 7175 616c 2869  lf.assertEqual(i
+0001c440: 6e66 6f2e 7265 7669 7369 6f6e 2c20 3729  nfo.revision, 7)
+0001c450: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001c460: 7365 7274 4571 7561 6c28 696e 666f 2e65  sertEqual(info.e
+0001c470: 7870 6972 6573 2c20 6461 7465 7469 6d65  xpires, datetime
+0001c480: 2e64 6174 6574 696d 6528 3230 3232 2c20  .datetime(2022, 
+0001c490: 3132 2c20 392c 2031 342c 2031 302c 2030  12, 9, 14, 10, 0
+0001c4a0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0001c4b0: 6173 7365 7274 4571 7561 6c28 696e 666f  assertEqual(info
+0001c4c0: 2e72 6f74 6174 696f 6e2c 206f 7073 2e53  .rotation, ops.S
+0001c4d0: 6563 7265 7452 6f74 6174 652e 4d4f 4e54  ecretRotate.MONT
+0001c4e0: 484c 5929 0a20 2020 2020 2020 2073 656c  HLY).        sel
+0001c4f0: 662e 6173 7365 7274 4571 7561 6c28 696e  f.assertEqual(in
+0001c500: 666f 2e72 6f74 6174 6573 2c20 6461 7465  fo.rotates, date
+0001c510: 7469 6d65 2e64 6174 6574 696d 6528 3230  time.datetime(20
+0001c520: 3233 2c20 312c 2039 2c20 3134 2c20 3130  23, 1, 9, 14, 10
+0001c530: 2c20 3029 290a 0a20 2020 2020 2020 2073  , 0))..        s
+0001c540: 656c 662e 6173 7365 7274 5472 7565 2872  elf.assertTrue(r
+0001c550: 6570 7228 696e 666f 292e 7374 6172 7473  epr(info).starts
+0001c560: 7769 7468 2827 5365 6372 6574 496e 666f  with('SecretInfo
+0001c570: 2827 2929 0a20 2020 2020 2020 2073 656c  (')).        sel
+0001c580: 662e 6173 7365 7274 5472 7565 2872 6570  f.assertTrue(rep
+0001c590: 7228 696e 666f 292e 656e 6473 7769 7468  r(info).endswith
+0001c5a0: 2827 2927 2929 0a0a 2020 2020 6465 6620  (')'))..    def 
+0001c5b0: 7465 7374 5f66 726f 6d5f 6469 6374 2873  test_from_dict(s
+0001c5c0: 656c 6629 3a0a 2020 2020 2020 2020 7574  elf):.        ut
+0001c5d0: 6320 3d20 6461 7465 7469 6d65 2e74 696d  c = datetime.tim
+0001c5e0: 657a 6f6e 652e 7574 630a 2020 2020 2020  ezone.utc.      
+0001c5f0: 2020 696e 666f 203d 206f 7073 2e53 6563    info = ops.Sec
+0001c600: 7265 7449 6e66 6f2e 6672 6f6d 5f64 6963  retInfo.from_dic
+0001c610: 7428 2773 6563 7265 743a 3427 2c20 7b0a  t('secret:4', {.
+0001c620: 2020 2020 2020 2020 2020 2020 276c 6162              'lab
+0001c630: 656c 273a 2027 6672 6f6d 6469 6374 272c  el': 'fromdict',
+0001c640: 0a20 2020 2020 2020 2020 2020 2027 7265  .            're
+0001c650: 7669 7369 6f6e 273a 2038 2c0a 2020 2020  vision': 8,.    
+0001c660: 2020 2020 2020 2020 2765 7870 6972 6573          'expires
+0001c670: 273a 2027 3230 3232 2d31 322d 3039 5431  ': '2022-12-09T1
+0001c680: 343a 3130 3a30 305a 272c 0a20 2020 2020  4:10:00Z',.     
+0001c690: 2020 2020 2020 2027 726f 7461 7469 6f6e         'rotation
+0001c6a0: 273a 2027 7965 6172 6c79 272c 0a20 2020  ': 'yearly',.   
+0001c6b0: 2020 2020 2020 2020 2027 726f 7461 7465           'rotate
+0001c6c0: 7327 3a20 2732 3032 332d 3031 2d30 3954  s': '2023-01-09T
+0001c6d0: 3134 3a31 303a 3030 5a27 2c0a 2020 2020  14:10:00Z',.    
+0001c6e0: 2020 2020 7d29 0a20 2020 2020 2020 2073      }).        s
+0001c6f0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001c700: 696e 666f 2e69 642c 2027 7365 6372 6574  info.id, 'secret
+0001c710: 3a34 2729 0a20 2020 2020 2020 2073 656c  :4').        sel
+0001c720: 662e 6173 7365 7274 4571 7561 6c28 696e  f.assertEqual(in
+0001c730: 666f 2e6c 6162 656c 2c20 2766 726f 6d64  fo.label, 'fromd
+0001c740: 6963 7427 290a 2020 2020 2020 2020 7365  ict').        se
+0001c750: 6c66 2e61 7373 6572 7445 7175 616c 2869  lf.assertEqual(i
+0001c760: 6e66 6f2e 7265 7669 7369 6f6e 2c20 3829  nfo.revision, 8)
+0001c770: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001c780: 7365 7274 4571 7561 6c28 696e 666f 2e65  sertEqual(info.e
+0001c790: 7870 6972 6573 2c20 6461 7465 7469 6d65  xpires, datetime
+0001c7a0: 2e64 6174 6574 696d 6528 3230 3232 2c20  .datetime(2022, 
+0001c7b0: 3132 2c20 392c 2031 342c 2031 302c 2030  12, 9, 14, 10, 0
+0001c7c0: 2c20 747a 696e 666f 3d75 7463 2929 0a20  , tzinfo=utc)). 
+0001c7d0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001c7e0: 7274 4571 7561 6c28 696e 666f 2e72 6f74  rtEqual(info.rot
+0001c7f0: 6174 696f 6e2c 206f 7073 2e53 6563 7265  ation, ops.Secre
+0001c800: 7452 6f74 6174 652e 5945 4152 4c59 290a  tRotate.YEARLY).
+0001c810: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0001c820: 6572 7445 7175 616c 2869 6e66 6f2e 726f  ertEqual(info.ro
+0001c830: 7461 7465 732c 2064 6174 6574 696d 652e  tates, datetime.
+0001c840: 6461 7465 7469 6d65 2832 3032 332c 2031  datetime(2023, 1
+0001c850: 2c20 392c 2031 342c 2031 302c 2030 2c20  , 9, 14, 10, 0, 
+0001c860: 747a 696e 666f 3d75 7463 2929 0a0a 2020  tzinfo=utc))..  
+0001c870: 2020 2020 2020 696e 666f 203d 206f 7073        info = ops
+0001c880: 2e53 6563 7265 7449 6e66 6f2e 6672 6f6d  .SecretInfo.from
+0001c890: 5f64 6963 7428 2773 6563 7265 743a 3427  _dict('secret:4'
+0001c8a0: 2c20 7b0a 2020 2020 2020 2020 2020 2020  , {.            
+0001c8b0: 276c 6162 656c 273a 2027 6672 6f6d 6469  'label': 'fromdi
+0001c8c0: 6374 272c 0a20 2020 2020 2020 2020 2020  ct',.           
+0001c8d0: 2027 7265 7669 7369 6f6e 273a 2038 2c0a   'revision': 8,.
+0001c8e0: 2020 2020 2020 2020 2020 2020 2772 6f74              'rot
+0001c8f0: 6174 696f 6e27 3a20 2762 6164 7661 6c75  ation': 'badvalu
+0001c900: 6527 2c0a 2020 2020 2020 2020 7d29 0a20  e',.        }). 
+0001c910: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001c920: 7274 4571 7561 6c28 696e 666f 2e69 642c  rtEqual(info.id,
+0001c930: 2027 7365 6372 6574 3a34 2729 0a20 2020   'secret:4').   
+0001c940: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001c950: 4571 7561 6c28 696e 666f 2e6c 6162 656c  Equal(info.label
+0001c960: 2c20 2766 726f 6d64 6963 7427 290a 2020  , 'fromdict').  
+0001c970: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0001c980: 7445 7175 616c 2869 6e66 6f2e 7265 7669  tEqual(info.revi
+0001c990: 7369 6f6e 2c20 3829 0a20 2020 2020 2020  sion, 8).       
+0001c9a0: 2073 656c 662e 6173 7365 7274 4973 4e6f   self.assertIsNo
+0001c9b0: 6e65 2869 6e66 6f2e 6578 7069 7265 7329  ne(info.expires)
+0001c9c0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001c9d0: 7365 7274 4973 4e6f 6e65 2869 6e66 6f2e  sertIsNone(info.
+0001c9e0: 726f 7461 7469 6f6e 290a 2020 2020 2020  rotation).      
+0001c9f0: 2020 7365 6c66 2e61 7373 6572 7449 734e    self.assertIsN
+0001ca00: 6f6e 6528 696e 666f 2e72 6f74 6174 6573  one(info.rotates
+0001ca10: 290a 0a20 2020 2020 2020 2069 6e66 6f20  )..        info 
+0001ca20: 3d20 6f70 732e 5365 6372 6574 496e 666f  = ops.SecretInfo
+0001ca30: 2e66 726f 6d5f 6469 6374 2827 3527 2c20  .from_dict('5', 
+0001ca40: 7b27 7265 7669 7369 6f6e 273a 2039 7d29  {'revision': 9})
+0001ca50: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001ca60: 7365 7274 4571 7561 6c28 696e 666f 2e69  sertEqual(info.i
+0001ca70: 642c 2027 7365 6372 6574 3a35 2729 0a20  d, 'secret:5'). 
+0001ca80: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001ca90: 7274 4571 7561 6c28 696e 666f 2e72 6576  rtEqual(info.rev
+0001caa0: 6973 696f 6e2c 2039 290a 0a0a 636c 6173  ision, 9)...clas
+0001cab0: 7320 5465 7374 5365 6372 6574 436c 6173  s TestSecretClas
+0001cac0: 7328 756e 6974 7465 7374 2e54 6573 7443  s(unittest.TestC
+0001cad0: 6173 6529 3a0a 2020 2020 6d61 7844 6966  ase):.    maxDif
+0001cae0: 6620 3d20 3634 202a 2031 3032 340a 0a20  f = 64 * 1024.. 
+0001caf0: 2020 2064 6566 2073 6574 5570 2873 656c     def setUp(sel
+0001cb00: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+0001cb10: 2e6d 6f64 656c 203d 206f 7073 2e4d 6f64  .model = ops.Mod
+0001cb20: 656c 286f 7073 2e43 6861 726d 4d65 7461  el(ops.CharmMeta
+0001cb30: 2829 2c20 5f4d 6f64 656c 4261 636b 656e  (), _ModelBacken
+0001cb40: 6428 276d 7961 7070 2f30 2729 290a 0a20  d('myapp/0')).. 
+0001cb50: 2020 2064 6566 206d 616b 655f 7365 6372     def make_secr
+0001cb60: 6574 2873 656c 662c 2069 643d 4e6f 6e65  et(self, id=None
+0001cb70: 2c20 6c61 6265 6c3d 4e6f 6e65 2c20 636f  , label=None, co
+0001cb80: 6e74 656e 743d 4e6f 6e65 293a 0a20 2020  ntent=None):.   
+0001cb90: 2020 2020 2072 6574 7572 6e20 6f70 732e       return ops.
+0001cba0: 5365 6372 6574 2873 656c 662e 6d6f 6465  Secret(self.mode
+0001cbb0: 6c2e 5f62 6163 6b65 6e64 2c20 6964 3d69  l._backend, id=i
+0001cbc0: 642c 206c 6162 656c 3d6c 6162 656c 2c20  d, label=label, 
+0001cbd0: 636f 6e74 656e 743d 636f 6e74 656e 7429  content=content)
+0001cbe0: 0a0a 2020 2020 6465 6620 7465 7374 5f69  ..    def test_i
+0001cbf0: 645f 616e 645f 6c61 6265 6c28 7365 6c66  d_and_label(self
+0001cc00: 293a 0a20 2020 2020 2020 2073 6563 7265  ):.        secre
+0001cc10: 7420 3d20 7365 6c66 2e6d 616b 655f 7365  t = self.make_se
+0001cc20: 6372 6574 2869 643d 2720 6162 6320 272c  cret(id=' abc ',
+0001cc30: 206c 6162 656c 3d27 6c62 6c27 290a 2020   label='lbl').  
+0001cc40: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0001cc50: 7445 7175 616c 2873 6563 7265 742e 6964  tEqual(secret.id
+0001cc60: 2c20 2773 6563 7265 743a 6162 6327 290a  , 'secret:abc').
+0001cc70: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0001cc80: 6572 7445 7175 616c 2873 6563 7265 742e  ertEqual(secret.
+0001cc90: 6c61 6265 6c2c 2027 6c62 6c27 290a 0a20  label, 'lbl').. 
+0001cca0: 2020 2020 2020 2073 6563 7265 7420 3d20         secret = 
+0001ccb0: 7365 6c66 2e6d 616b 655f 7365 6372 6574  self.make_secret
+0001ccc0: 2869 643d 2778 2729 0a20 2020 2020 2020  (id='x').       
+0001ccd0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0001cce0: 6c28 7365 6372 6574 2e69 642c 2027 7365  l(secret.id, 'se
+0001ccf0: 6372 6574 3a78 2729 0a20 2020 2020 2020  cret:x').       
+0001cd00: 2073 656c 662e 6173 7365 7274 4973 4e6f   self.assertIsNo
+0001cd10: 6e65 2873 6563 7265 742e 6c61 6265 6c29  ne(secret.label)
+0001cd20: 0a0a 2020 2020 2020 2020 7365 6372 6574  ..        secret
+0001cd30: 203d 2073 656c 662e 6d61 6b65 5f73 6563   = self.make_sec
+0001cd40: 7265 7428 6c61 6265 6c3d 2779 2729 0a20  ret(label='y'). 
+0001cd50: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001cd60: 7274 4973 4e6f 6e65 2873 6563 7265 742e  rtIsNone(secret.
+0001cd70: 6964 290a 2020 2020 2020 2020 7365 6c66  id).        self
+0001cd80: 2e61 7373 6572 7445 7175 616c 2873 6563  .assertEqual(sec
+0001cd90: 7265 742e 6c61 6265 6c2c 2027 7927 290a  ret.label, 'y').
+0001cda0: 0a20 2020 2064 6566 2074 6573 745f 6765  .    def test_ge
+0001cdb0: 745f 636f 6e74 656e 745f 6361 6368 6564  t_content_cached
+0001cdc0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0001cdd0: 6661 6b65 5f73 6372 6970 7428 7365 6c66  fake_script(self
+0001cde0: 2c20 2773 6563 7265 742d 6765 7427 2c20  , 'secret-get', 
+0001cdf0: 2222 2265 7869 7420 3122 2222 290a 0a20  """exit 1""").. 
+0001ce00: 2020 2020 2020 2073 6563 7265 7420 3d20         secret = 
+0001ce10: 7365 6c66 2e6d 616b 655f 7365 6372 6574  self.make_secret
+0001ce20: 2869 643d 2778 272c 206c 6162 656c 3d27  (id='x', label='
+0001ce30: 7927 2c20 636f 6e74 656e 743d 7b27 666f  y', content={'fo
+0001ce40: 6f27 3a20 2762 6172 277d 290a 2020 2020  o': 'bar'}).    
+0001ce50: 2020 2020 636f 6e74 656e 7420 3d20 7365      content = se
+0001ce60: 6372 6574 2e67 6574 5f63 6f6e 7465 6e74  cret.get_content
+0001ce70: 2829 2020 2320 7769 6c6c 2075 7365 2063  ()  # will use c
+0001ce80: 6163 6865 6420 636f 6e74 656e 742c 206e  ached content, n
+0001ce90: 6f74 2072 756e 2073 6563 7265 742d 6765  ot run secret-ge
+0001cea0: 740a 2020 2020 2020 2020 7365 6c66 2e61  t.        self.a
+0001ceb0: 7373 6572 7445 7175 616c 2863 6f6e 7465  ssertEqual(conte
+0001cec0: 6e74 2c20 7b27 666f 6f27 3a20 2762 6172  nt, {'foo': 'bar
+0001ced0: 277d 290a 0a20 2020 2020 2020 2073 656c  '})..        sel
+0001cee0: 662e 6173 7365 7274 4571 7561 6c28 6661  f.assertEqual(fa
+0001cef0: 6b65 5f73 6372 6970 745f 6361 6c6c 7328  ke_script_calls(
+0001cf00: 7365 6c66 2c20 636c 6561 723d 5472 7565  self, clear=True
+0001cf10: 292c 205b 5d29 0a0a 2020 2020 6465 6620  ), [])..    def 
+0001cf20: 7465 7374 5f67 6574 5f63 6f6e 7465 6e74  test_get_content
+0001cf30: 5f72 6566 7265 7368 2873 656c 6629 3a0a  _refresh(self):.
+0001cf40: 2020 2020 2020 2020 6661 6b65 5f73 6372          fake_scr
+0001cf50: 6970 7428 7365 6c66 2c20 2773 6563 7265  ipt(self, 'secre
+0001cf60: 742d 6765 7427 2c20 2222 2265 6368 6f20  t-get', """echo 
+0001cf70: 277b 2266 6f6f 223a 2022 7265 6672 6573  '{"foo": "refres
+0001cf80: 6865 6422 7d27 2222 2229 0a0a 2020 2020  hed"}'""")..    
+0001cf90: 2020 2020 7365 6372 6574 203d 2073 656c      secret = sel
+0001cfa0: 662e 6d61 6b65 5f73 6563 7265 7428 6964  f.make_secret(id
+0001cfb0: 3d27 7927 2c20 636f 6e74 656e 743d 7b27  ='y', content={'
+0001cfc0: 666f 6f27 3a20 2762 6172 277d 290a 2020  foo': 'bar'}).  
+0001cfd0: 2020 2020 2020 636f 6e74 656e 7420 3d20        content = 
+0001cfe0: 7365 6372 6574 2e67 6574 5f63 6f6e 7465  secret.get_conte
+0001cff0: 6e74 2872 6566 7265 7368 3d54 7275 6529  nt(refresh=True)
+0001d000: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001d010: 7365 7274 4571 7561 6c28 636f 6e74 656e  sertEqual(conten
+0001d020: 742c 207b 2766 6f6f 273a 2027 7265 6672  t, {'foo': 'refr
+0001d030: 6573 6865 6427 7d29 0a0a 2020 2020 2020  eshed'})..      
+0001d040: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0001d050: 616c 2866 616b 655f 7363 7269 7074 5f63  al(fake_script_c
+0001d060: 616c 6c73 2873 656c 662c 2063 6c65 6172  alls(self, clear
+0001d070: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
+0001d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d090: 205b 5b27 7365 6372 6574 2d67 6574 272c   [['secret-get',
+0001d0a0: 2027 7365 6372 6574 3a79 272c 2027 2d2d   'secret:y', '--
+0001d0b0: 7265 6672 6573 6827 2c20 272d 2d66 6f72  refresh', '--for
+0001d0c0: 6d61 743d 6a73 6f6e 275d 5d29 0a0a 2020  mat=json']])..  
+0001d0d0: 2020 6465 6620 7465 7374 5f67 6574 5f63    def test_get_c
+0001d0e0: 6f6e 7465 6e74 5f75 6e63 6163 6865 6428  ontent_uncached(
+0001d0f0: 7365 6c66 293a 0a20 2020 2020 2020 2066  self):.        f
+0001d100: 616b 655f 7363 7269 7074 2873 656c 662c  ake_script(self,
+0001d110: 2027 7365 6372 6574 2d67 6574 272c 2022   'secret-get', "
+0001d120: 2222 6563 686f 2027 7b22 666f 6f22 3a20  ""echo '{"foo": 
+0001d130: 226e 6f74 6361 6368 6564 227d 2722 2222  "notcached"}'"""
+0001d140: 290a 0a20 2020 2020 2020 2073 6563 7265  )..        secre
+0001d150: 7420 3d20 7365 6c66 2e6d 616b 655f 7365  t = self.make_se
+0001d160: 6372 6574 2869 643d 277a 2729 0a20 2020  cret(id='z').   
+0001d170: 2020 2020 2063 6f6e 7465 6e74 203d 2073       content = s
+0001d180: 6563 7265 742e 6765 745f 636f 6e74 656e  ecret.get_conten
+0001d190: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+0001d1a0: 2e61 7373 6572 7445 7175 616c 2863 6f6e  .assertEqual(con
+0001d1b0: 7465 6e74 2c20 7b27 666f 6f27 3a20 276e  tent, {'foo': 'n
+0001d1c0: 6f74 6361 6368 6564 277d 290a 0a20 2020  otcached'})..   
+0001d1d0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001d1e0: 4571 7561 6c28 6661 6b65 5f73 6372 6970  Equal(fake_scrip
+0001d1f0: 745f 6361 6c6c 7328 7365 6c66 2c20 636c  t_calls(self, cl
+0001d200: 6561 723d 5472 7565 292c 0a20 2020 2020  ear=True),.     
+0001d210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d220: 2020 2020 5b5b 2773 6563 7265 742d 6765      [['secret-ge
+0001d230: 7427 2c20 2773 6563 7265 743a 7a27 2c20  t', 'secret:z', 
+0001d240: 272d 2d66 6f72 6d61 743d 6a73 6f6e 275d  '--format=json']
+0001d250: 5d29 0a0a 2020 2020 6465 6620 7465 7374  ])..    def test
+0001d260: 5f70 6565 6b5f 636f 6e74 656e 7428 7365  _peek_content(se
+0001d270: 6c66 293a 0a20 2020 2020 2020 2066 616b  lf):.        fak
+0001d280: 655f 7363 7269 7074 2873 656c 662c 2027  e_script(self, '
+0001d290: 7365 6372 6574 2d67 6574 272c 2022 2222  secret-get', """
+0001d2a0: 6563 686f 2027 7b22 666f 6f22 3a20 2270  echo '{"foo": "p
+0001d2b0: 6565 6b65 6422 7d27 2222 2229 0a0a 2020  eeked"}'""")..  
+0001d2c0: 2020 2020 2020 7365 6372 6574 203d 2073        secret = s
+0001d2d0: 656c 662e 6d61 6b65 5f73 6563 7265 7428  elf.make_secret(
+0001d2e0: 6964 3d27 6127 2c20 6c61 6265 6c3d 2762  id='a', label='b
+0001d2f0: 2729 0a20 2020 2020 2020 2063 6f6e 7465  ').        conte
+0001d300: 6e74 203d 2073 6563 7265 742e 7065 656b  nt = secret.peek
+0001d310: 5f63 6f6e 7465 6e74 2829 0a20 2020 2020  _content().     
+0001d320: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0001d330: 7561 6c28 636f 6e74 656e 742c 207b 2766  ual(content, {'f
+0001d340: 6f6f 273a 2027 7065 656b 6564 277d 290a  oo': 'peeked'}).
+0001d350: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001d360: 7365 7274 4571 7561 6c28 6661 6b65 5f73  sertEqual(fake_s
+0001d370: 6372 6970 745f 6361 6c6c 7328 7365 6c66  cript_calls(self
+0001d380: 2c20 636c 6561 723d 5472 7565 292c 0a20  , clear=True),. 
+0001d390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d3a0: 2020 2020 2020 2020 5b5b 2773 6563 7265          [['secre
+0001d3b0: 742d 6765 7427 2c20 2773 6563 7265 743a  t-get', 'secret:
+0001d3c0: 6127 2c20 272d 2d6c 6162 656c 272c 2027  a', '--label', '
+0001d3d0: 6227 2c20 272d 2d70 6565 6b27 2c20 272d  b', '--peek', '-
+0001d3e0: 2d66 6f72 6d61 743d 6a73 6f6e 275d 5d29  -format=json']])
+0001d3f0: 0a0a 2020 2020 6465 6620 7465 7374 5f67  ..    def test_g
+0001d400: 6574 5f69 6e66 6f28 7365 6c66 293a 0a20  et_info(self):. 
+0001d410: 2020 2020 2020 2066 616b 655f 7363 7269         fake_scri
+0001d420: 7074 2873 656c 662c 2027 7365 6372 6574  pt(self, 'secret
+0001d430: 2d69 6e66 6f2d 6765 7427 2c20 2222 2265  -info-get', """e
+0001d440: 6368 6f20 277b 2278 223a 207b 226c 6162  cho '{"x": {"lab
+0001d450: 656c 223a 2022 7922 2c20 2272 6576 6973  el": "y", "revis
+0001d460: 696f 6e22 3a20 377d 7d27 2222 2229 0a0a  ion": 7}}'""")..
+0001d470: 2020 2020 2020 2020 2320 5365 6372 6574          # Secret
+0001d480: 2077 6974 6820 4944 206f 6e6c 790a 2020   with ID only.  
+0001d490: 2020 2020 2020 7365 6372 6574 203d 2073        secret = s
+0001d4a0: 656c 662e 6d61 6b65 5f73 6563 7265 7428  elf.make_secret(
+0001d4b0: 6964 3d27 7827 290a 2020 2020 2020 2020  id='x').        
+0001d4c0: 696e 666f 203d 2073 6563 7265 742e 6765  info = secret.ge
+0001d4d0: 745f 696e 666f 2829 0a20 2020 2020 2020  t_info().       
+0001d4e0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0001d4f0: 6c28 696e 666f 2e69 642c 2027 7365 6372  l(info.id, 'secr
+0001d500: 6574 3a78 2729 0a20 2020 2020 2020 2073  et:x').        s
+0001d510: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001d520: 696e 666f 2e6c 6162 656c 2c20 2779 2729  info.label, 'y')
+0001d530: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001d540: 7365 7274 4571 7561 6c28 696e 666f 2e72  sertEqual(info.r
+0001d550: 6576 6973 696f 6e2c 2037 290a 0a20 2020  evision, 7)..   
+0001d560: 2020 2020 2023 2053 6563 7265 7420 7769       # Secret wi
+0001d570: 7468 206c 6162 656c 206f 6e6c 790a 2020  th label only.  
+0001d580: 2020 2020 2020 7365 6372 6574 203d 2073        secret = s
+0001d590: 656c 662e 6d61 6b65 5f73 6563 7265 7428  elf.make_secret(
+0001d5a0: 6c61 6265 6c3d 2779 2729 0a20 2020 2020  label='y').     
+0001d5b0: 2020 2069 6e66 6f20 3d20 7365 6372 6574     info = secret
+0001d5c0: 2e67 6574 5f69 6e66 6f28 290a 2020 2020  .get_info().    
+0001d5d0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0001d5e0: 7175 616c 2869 6e66 6f2e 6964 2c20 2773  qual(info.id, 's
+0001d5f0: 6563 7265 743a 7827 290a 2020 2020 2020  ecret:x').      
+0001d600: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0001d610: 616c 2869 6e66 6f2e 6c61 6265 6c2c 2027  al(info.label, '
+0001d620: 7927 290a 2020 2020 2020 2020 7365 6c66  y').        self
+0001d630: 2e61 7373 6572 7445 7175 616c 2869 6e66  .assertEqual(inf
+0001d640: 6f2e 7265 7669 7369 6f6e 2c20 3729 0a0a  o.revision, 7)..
+0001d650: 2020 2020 2020 2020 2320 5365 6372 6574          # Secret
+0001d660: 2077 6974 6820 4944 2061 6e64 206c 6162   with ID and lab
+0001d670: 656c 0a20 2020 2020 2020 2073 6563 7265  el.        secre
+0001d680: 7420 3d20 7365 6c66 2e6d 616b 655f 7365  t = self.make_se
+0001d690: 6372 6574 2869 643d 2778 272c 206c 6162  cret(id='x', lab
+0001d6a0: 656c 3d27 7927 290a 2020 2020 2020 2020  el='y').        
+0001d6b0: 696e 666f 203d 2073 6563 7265 742e 6765  info = secret.ge
+0001d6c0: 745f 696e 666f 2829 0a20 2020 2020 2020  t_info().       
+0001d6d0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0001d6e0: 6c28 696e 666f 2e69 642c 2027 7365 6372  l(info.id, 'secr
+0001d6f0: 6574 3a78 2729 0a20 2020 2020 2020 2073  et:x').        s
+0001d700: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001d710: 696e 666f 2e6c 6162 656c 2c20 2779 2729  info.label, 'y')
+0001d720: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001d730: 7365 7274 4571 7561 6c28 696e 666f 2e72  sertEqual(info.r
+0001d740: 6576 6973 696f 6e2c 2037 290a 0a20 2020  evision, 7)..   
+0001d750: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001d760: 4571 7561 6c28 0a20 2020 2020 2020 2020  Equal(.         
+0001d770: 2020 2066 616b 655f 7363 7269 7074 5f63     fake_script_c
+0001d780: 616c 6c73 2873 656c 662c 2063 6c65 6172  alls(self, clear
+0001d790: 3d54 7275 6529 2c0a 2020 2020 2020 2020  =True),.        
+0001d7a0: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+0001d7b0: 2020 2020 2020 5b27 7365 6372 6574 2d69        ['secret-i
+0001d7c0: 6e66 6f2d 6765 7427 2c20 2773 6563 7265  nfo-get', 'secre
+0001d7d0: 743a 7827 2c20 272d 2d66 6f72 6d61 743d  t:x', '--format=
+0001d7e0: 6a73 6f6e 275d 2c0a 2020 2020 2020 2020  json'],.        
+0001d7f0: 2020 2020 2020 2020 5b27 7365 6372 6574          ['secret
+0001d800: 2d69 6e66 6f2d 6765 7427 2c20 272d 2d6c  -info-get', '--l
+0001d810: 6162 656c 272c 2027 7927 2c20 272d 2d66  abel', 'y', '--f
+0001d820: 6f72 6d61 743d 6a73 6f6e 275d 2c0a 2020  ormat=json'],.  
+0001d830: 2020 2020 2020 2020 2020 2020 2020 5b27                ['
 0001d840: 7365 6372 6574 2d69 6e66 6f2d 6765 7427  secret-info-get'
-0001d850: 2c20 272d 2d6c 6162 656c 272c 2027 7927  , '--label', 'y'
-0001d860: 2c20 272d 2d66 6f72 6d61 743d 6a73 6f6e  , '--format=json
-0001d870: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
-0001d880: 5b27 7365 6372 6574 2d73 6574 272c 2027  ['secret-set', '
-0001d890: 7365 6372 6574 3a7a 272c 2027 6261 723d  secret:z', 'bar=
-0001d8a0: 666f 6f27 5d2c 0a20 2020 2020 2020 205d  foo'],.        ]
-0001d8b0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-0001d8c0: 7365 745f 696e 666f 2873 656c 6629 3a0a  set_info(self):.
-0001d8d0: 2020 2020 2020 2020 6661 6b65 5f73 6372          fake_scr
-0001d8e0: 6970 7428 7365 6c66 2c20 2773 6563 7265  ipt(self, 'secre
-0001d8f0: 742d 7365 7427 2c20 2222 2265 7869 7420  t-set', """exit 
-0001d900: 3022 2222 290a 2020 2020 2020 2020 6661  0""").        fa
-0001d910: 6b65 5f73 6372 6970 7428 7365 6c66 2c20  ke_script(self, 
-0001d920: 2773 6563 7265 742d 696e 666f 2d67 6574  'secret-info-get
-0001d930: 272c 2022 2222 6563 686f 2027 7b22 7a22  ', """echo '{"z"
-0001d940: 3a20 7b22 6c61 6265 6c22 3a20 2279 222c  : {"label": "y",
-0001d950: 2022 7265 7669 7369 6f6e 223a 2037 7d7d   "revision": 7}}
-0001d960: 2722 2222 290a 0a20 2020 2020 2020 2073  '""")..        s
-0001d970: 6563 7265 7420 3d20 7365 6c66 2e6d 616b  ecret = self.mak
-0001d980: 655f 7365 6372 6574 2869 643d 2778 2729  e_secret(id='x')
-0001d990: 0a20 2020 2020 2020 2065 7870 6972 6520  .        expire 
-0001d9a0: 3d20 6461 7465 7469 6d65 2e64 6174 6574  = datetime.datet
-0001d9b0: 696d 6528 3230 3232 2c20 3132 2c20 392c  ime(2022, 12, 9,
-0001d9c0: 2031 362c 2035 392c 2030 290a 2020 2020   16, 59, 0).    
-0001d9d0: 2020 2020 7365 6372 6574 2e73 6574 5f69      secret.set_i
-0001d9e0: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
-0001d9f0: 206c 6162 656c 3d27 6c61 6227 2c0a 2020   label='lab',.  
-0001da00: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-0001da10: 7074 696f 6e3d 2764 6573 6327 2c0a 2020  ption='desc',.  
-0001da20: 2020 2020 2020 2020 2020 6578 7069 7265            expire
-0001da30: 3d65 7870 6972 652c 0a20 2020 2020 2020  =expire,.       
-0001da40: 2020 2020 2072 6f74 6174 653d 6f70 732e       rotate=ops.
-0001da50: 5365 6372 6574 526f 7461 7465 2e4d 4f4e  SecretRotate.MON
-0001da60: 5448 4c59 2c0a 2020 2020 2020 2020 290a  THLY,.        ).
-0001da70: 0a20 2020 2020 2020 2023 2049 6620 7365  .        # If se
-0001da80: 6372 6574 2064 6f65 736e 2774 2068 6176  cret doesn't hav
-0001da90: 6520 616e 2049 442c 2077 6527 6c6c 2072  e an ID, we'll r
-0001daa0: 756e 2073 6563 7265 742d 696e 666f 2d67  un secret-info-g
-0001dab0: 6574 2074 6f20 6665 7463 6820 6974 0a20  et to fetch it. 
-0001dac0: 2020 2020 2020 2073 6563 7265 7420 3d20         secret = 
-0001dad0: 7365 6c66 2e6d 616b 655f 7365 6372 6574  self.make_secret
-0001dae0: 286c 6162 656c 3d27 7927 290a 2020 2020  (label='y').    
-0001daf0: 2020 2020 7365 6c66 2e61 7373 6572 7449      self.assertI
-0001db00: 734e 6f6e 6528 7365 6372 6574 2e69 6429  sNone(secret.id)
-0001db10: 0a20 2020 2020 2020 2073 6563 7265 742e  .        secret.
-0001db20: 7365 745f 696e 666f 286c 6162 656c 3d27  set_info(label='
-0001db30: 6c62 6c27 290a 2020 2020 2020 2020 7365  lbl').        se
-0001db40: 6c66 2e61 7373 6572 7445 7175 616c 2873  lf.assertEqual(s
-0001db50: 6563 7265 742e 6964 2c20 2773 6563 7265  ecret.id, 'secre
-0001db60: 743a 7a27 290a 0a20 2020 2020 2020 2073  t:z')..        s
-0001db70: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0001db80: 6661 6b65 5f73 6372 6970 745f 6361 6c6c  fake_script_call
-0001db90: 7328 7365 6c66 2c20 636c 6561 723d 5472  s(self, clear=Tr
-0001dba0: 7565 292c 205b 0a20 2020 2020 2020 2020  ue), [.         
-0001dbb0: 2020 205b 2773 6563 7265 742d 7365 7427     ['secret-set'
-0001dbc0: 2c20 2773 6563 7265 743a 7827 2c20 272d  , 'secret:x', '-
-0001dbd0: 2d6c 6162 656c 272c 2027 6c61 6227 2c20  -label', 'lab', 
-0001dbe0: 272d 2d64 6573 6372 6970 7469 6f6e 272c  '--description',
-0001dbf0: 2027 6465 7363 272c 0a20 2020 2020 2020   'desc',.       
-0001dc00: 2020 2020 2020 272d 2d65 7870 6972 6527        '--expire'
-0001dc10: 2c20 2732 3032 322d 3132 2d30 3954 3136  , '2022-12-09T16
-0001dc20: 3a35 393a 3030 272c 2027 2d2d 726f 7461  :59:00', '--rota
-0001dc30: 7465 272c 2027 6d6f 6e74 686c 7927 5d2c  te', 'monthly'],
-0001dc40: 0a20 2020 2020 2020 2020 2020 205b 2773  .            ['s
-0001dc50: 6563 7265 742d 696e 666f 2d67 6574 272c  ecret-info-get',
-0001dc60: 2027 2d2d 6c61 6265 6c27 2c20 2779 272c   '--label', 'y',
-0001dc70: 2027 2d2d 666f 726d 6174 3d6a 736f 6e27   '--format=json'
-0001dc80: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-0001dc90: 2773 6563 7265 742d 7365 7427 2c20 2773  'secret-set', 's
-0001dca0: 6563 7265 743a 7a27 2c20 272d 2d6c 6162  ecret:z', '--lab
-0001dcb0: 656c 272c 2027 6c62 6c27 5d2c 0a20 2020  el', 'lbl'],.   
-0001dcc0: 2020 2020 205d 290a 0a20 2020 2020 2020       ])..       
-0001dcd0: 2077 6974 6820 7365 6c66 2e61 7373 6572   with self.asser
-0001dce0: 7452 6169 7365 7328 5479 7065 4572 726f  tRaises(TypeErro
-0001dcf0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-0001dd00: 7365 6372 6574 2e73 6574 5f69 6e66 6f28  secret.set_info(
-0001dd10: 2920 2023 206e 6f20 6172 6773 2070 726f  )  # no args pro
-0001dd20: 7669 6465 640a 0a20 2020 2064 6566 2074  vided..    def t
-0001dd30: 6573 745f 6772 616e 7428 7365 6c66 293a  est_grant(self):
-0001dd40: 0a20 2020 2020 2020 2066 616b 655f 7363  .        fake_sc
-0001dd50: 7269 7074 2873 656c 662c 2027 7365 6372  ript(self, 'secr
-0001dd60: 6574 2d67 7261 6e74 272c 2022 2222 6578  et-grant', """ex
-0001dd70: 6974 2030 2222 2229 0a20 2020 2020 2020  it 0""").       
-0001dd80: 2066 616b 655f 7363 7269 7074 2873 656c   fake_script(sel
-0001dd90: 662c 2027 7365 6372 6574 2d69 6e66 6f2d  f, 'secret-info-
-0001dda0: 6765 7427 2c20 2222 2265 6368 6f20 277b  get', """echo '{
-0001ddb0: 227a 223a 207b 226c 6162 656c 223a 2022  "z": {"label": "
-0001ddc0: 7922 2c20 2272 6576 6973 696f 6e22 3a20  y", "revision": 
-0001ddd0: 377d 7d27 2222 2229 0a0a 2020 2020 2020  7}}'""")..      
-0001dde0: 2020 7365 6372 6574 203d 2073 656c 662e    secret = self.
-0001ddf0: 6d61 6b65 5f73 6563 7265 7428 6964 3d27  make_secret(id='
-0001de00: 7827 290a 2020 2020 2020 2020 7365 6372  x').        secr
-0001de10: 6574 2e67 7261 6e74 2874 7970 6573 2e53  et.grant(types.S
-0001de20: 696d 706c 654e 616d 6573 7061 6365 2869  impleNamespace(i
-0001de30: 643d 3132 3329 290a 2020 2020 2020 2020  d=123)).        
-0001de40: 7365 6372 6574 2e67 7261 6e74 2874 7970  secret.grant(typ
-0001de50: 6573 2e53 696d 706c 654e 616d 6573 7061  es.SimpleNamespa
-0001de60: 6365 2869 643d 3233 3429 2c20 756e 6974  ce(id=234), unit
-0001de70: 3d74 7970 6573 2e53 696d 706c 654e 616d  =types.SimpleNam
-0001de80: 6573 7061 6365 286e 616d 653d 2761 7070  espace(name='app
-0001de90: 2f30 2729 290a 0a20 2020 2020 2020 2023  /0'))..        #
-0001dea0: 2049 6620 7365 6372 6574 2064 6f65 736e   If secret doesn
-0001deb0: 2774 2068 6176 6520 616e 2049 442c 2077  't have an ID, w
-0001dec0: 6527 6c6c 2072 756e 2073 6563 7265 742d  e'll run secret-
-0001ded0: 696e 666f 2d67 6574 2074 6f20 6665 7463  info-get to fetc
-0001dee0: 6820 6974 0a20 2020 2020 2020 2073 6563  h it.        sec
-0001def0: 7265 7420 3d20 7365 6c66 2e6d 616b 655f  ret = self.make_
-0001df00: 7365 6372 6574 286c 6162 656c 3d27 7927  secret(label='y'
-0001df10: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0001df20: 7373 6572 7449 734e 6f6e 6528 7365 6372  ssertIsNone(secr
-0001df30: 6574 2e69 6429 0a20 2020 2020 2020 2073  et.id).        s
-0001df40: 6563 7265 742e 6772 616e 7428 7479 7065  ecret.grant(type
-0001df50: 732e 5369 6d70 6c65 4e61 6d65 7370 6163  s.SimpleNamespac
-0001df60: 6528 6964 3d33 3435 2929 0a20 2020 2020  e(id=345)).     
-0001df70: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0001df80: 7561 6c28 7365 6372 6574 2e69 642c 2027  ual(secret.id, '
-0001df90: 7365 6372 6574 3a7a 2729 0a0a 2020 2020  secret:z')..    
-0001dfa0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0001dfb0: 7175 616c 2866 616b 655f 7363 7269 7074  qual(fake_script
-0001dfc0: 5f63 616c 6c73 2873 656c 662c 2063 6c65  _calls(self, cle
-0001dfd0: 6172 3d54 7275 6529 2c20 5b0a 2020 2020  ar=True), [.    
-0001dfe0: 2020 2020 2020 2020 5b27 7365 6372 6574          ['secret
-0001dff0: 2d67 7261 6e74 272c 2027 7365 6372 6574  -grant', 'secret
-0001e000: 3a78 272c 2027 2d2d 7265 6c61 7469 6f6e  :x', '--relation
-0001e010: 272c 2027 3132 3327 5d2c 0a20 2020 2020  ', '123'],.     
-0001e020: 2020 2020 2020 205b 2773 6563 7265 742d         ['secret-
-0001e030: 6772 616e 7427 2c20 2773 6563 7265 743a  grant', 'secret:
-0001e040: 7827 2c20 272d 2d72 656c 6174 696f 6e27  x', '--relation'
-0001e050: 2c20 2732 3334 272c 2027 2d2d 756e 6974  , '234', '--unit
-0001e060: 272c 2027 6170 702f 3027 5d2c 0a20 2020  ', 'app/0'],.   
-0001e070: 2020 2020 2020 2020 205b 2773 6563 7265           ['secre
-0001e080: 742d 696e 666f 2d67 6574 272c 2027 2d2d  t-info-get', '--
-0001e090: 6c61 6265 6c27 2c20 2779 272c 2027 2d2d  label', 'y', '--
-0001e0a0: 666f 726d 6174 3d6a 736f 6e27 5d2c 0a20  format=json'],. 
-0001e0b0: 2020 2020 2020 2020 2020 205b 2773 6563             ['sec
-0001e0c0: 7265 742d 6772 616e 7427 2c20 2773 6563  ret-grant', 'sec
-0001e0d0: 7265 743a 7a27 2c20 272d 2d72 656c 6174  ret:z', '--relat
-0001e0e0: 696f 6e27 2c20 2733 3435 275d 2c0a 2020  ion', '345'],.  
-0001e0f0: 2020 2020 2020 5d29 0a0a 2020 2020 6465        ])..    de
-0001e100: 6620 7465 7374 5f72 6576 6f6b 6528 7365  f test_revoke(se
-0001e110: 6c66 293a 0a20 2020 2020 2020 2066 616b  lf):.        fak
-0001e120: 655f 7363 7269 7074 2873 656c 662c 2027  e_script(self, '
-0001e130: 7365 6372 6574 2d72 6576 6f6b 6527 2c20  secret-revoke', 
-0001e140: 2222 2265 7869 7420 3022 2222 290a 2020  """exit 0""").  
-0001e150: 2020 2020 2020 6661 6b65 5f73 6372 6970        fake_scrip
-0001e160: 7428 7365 6c66 2c20 2773 6563 7265 742d  t(self, 'secret-
-0001e170: 696e 666f 2d67 6574 272c 2022 2222 6563  info-get', """ec
-0001e180: 686f 2027 7b22 7a22 3a20 7b22 6c61 6265  ho '{"z": {"labe
-0001e190: 6c22 3a20 2279 222c 2022 7265 7669 7369  l": "y", "revisi
-0001e1a0: 6f6e 223a 2037 7d7d 2722 2222 290a 0a20  on": 7}}'""").. 
-0001e1b0: 2020 2020 2020 2073 6563 7265 7420 3d20         secret = 
-0001e1c0: 7365 6c66 2e6d 616b 655f 7365 6372 6574  self.make_secret
-0001e1d0: 2869 643d 2778 2729 0a20 2020 2020 2020  (id='x').       
-0001e1e0: 2073 6563 7265 742e 7265 766f 6b65 2874   secret.revoke(t
-0001e1f0: 7970 6573 2e53 696d 706c 654e 616d 6573  ypes.SimpleNames
-0001e200: 7061 6365 2869 643d 3132 3329 290a 2020  pace(id=123)).  
-0001e210: 2020 2020 2020 7365 6372 6574 2e72 6576        secret.rev
-0001e220: 6f6b 6528 7479 7065 732e 5369 6d70 6c65  oke(types.Simple
-0001e230: 4e61 6d65 7370 6163 6528 6964 3d32 3334  Namespace(id=234
-0001e240: 292c 2075 6e69 743d 7479 7065 732e 5369  ), unit=types.Si
-0001e250: 6d70 6c65 4e61 6d65 7370 6163 6528 6e61  mpleNamespace(na
-0001e260: 6d65 3d27 6170 702f 3027 2929 0a0a 2020  me='app/0'))..  
-0001e270: 2020 2020 2020 2320 4966 2073 6563 7265        # If secre
-0001e280: 7420 646f 6573 6e27 7420 6861 7665 2061  t doesn't have a
-0001e290: 6e20 4944 2c20 7765 276c 6c20 7275 6e20  n ID, we'll run 
-0001e2a0: 7365 6372 6574 2d69 6e66 6f2d 6765 7420  secret-info-get 
-0001e2b0: 746f 2066 6574 6368 2069 740a 2020 2020  to fetch it.    
-0001e2c0: 2020 2020 7365 6372 6574 203d 2073 656c      secret = sel
-0001e2d0: 662e 6d61 6b65 5f73 6563 7265 7428 6c61  f.make_secret(la
-0001e2e0: 6265 6c3d 2779 2729 0a20 2020 2020 2020  bel='y').       
-0001e2f0: 2073 656c 662e 6173 7365 7274 4973 4e6f   self.assertIsNo
-0001e300: 6e65 2873 6563 7265 742e 6964 290a 2020  ne(secret.id).  
-0001e310: 2020 2020 2020 7365 6372 6574 2e72 6576        secret.rev
-0001e320: 6f6b 6528 7479 7065 732e 5369 6d70 6c65  oke(types.Simple
-0001e330: 4e61 6d65 7370 6163 6528 6964 3d33 3435  Namespace(id=345
-0001e340: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0001e350: 6173 7365 7274 4571 7561 6c28 7365 6372  assertEqual(secr
-0001e360: 6574 2e69 642c 2027 7365 6372 6574 3a7a  et.id, 'secret:z
-0001e370: 2729 0a0a 2020 2020 2020 2020 7365 6c66  ')..        self
-0001e380: 2e61 7373 6572 7445 7175 616c 2866 616b  .assertEqual(fak
-0001e390: 655f 7363 7269 7074 5f63 616c 6c73 2873  e_script_calls(s
-0001e3a0: 656c 662c 2063 6c65 6172 3d54 7275 6529  elf, clear=True)
-0001e3b0: 2c20 5b0a 2020 2020 2020 2020 2020 2020  , [.            
-0001e3c0: 5b27 7365 6372 6574 2d72 6576 6f6b 6527  ['secret-revoke'
-0001e3d0: 2c20 2773 6563 7265 743a 7827 2c20 272d  , 'secret:x', '-
-0001e3e0: 2d72 656c 6174 696f 6e27 2c20 2731 3233  -relation', '123
-0001e3f0: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
-0001e400: 5b27 7365 6372 6574 2d72 6576 6f6b 6527  ['secret-revoke'
-0001e410: 2c20 2773 6563 7265 743a 7827 2c20 272d  , 'secret:x', '-
-0001e420: 2d72 656c 6174 696f 6e27 2c20 2732 3334  -relation', '234
-0001e430: 272c 2027 2d2d 756e 6974 272c 2027 6170  ', '--unit', 'ap
-0001e440: 702f 3027 5d2c 0a20 2020 2020 2020 2020  p/0'],.         
-0001e450: 2020 205b 2773 6563 7265 742d 696e 666f     ['secret-info
-0001e460: 2d67 6574 272c 2027 2d2d 6c61 6265 6c27  -get', '--label'
-0001e470: 2c20 2779 272c 2027 2d2d 666f 726d 6174  , 'y', '--format
-0001e480: 3d6a 736f 6e27 5d2c 0a20 2020 2020 2020  =json'],.       
-0001e490: 2020 2020 205b 2773 6563 7265 742d 7265       ['secret-re
-0001e4a0: 766f 6b65 272c 2027 7365 6372 6574 3a7a  voke', 'secret:z
-0001e4b0: 272c 2027 2d2d 7265 6c61 7469 6f6e 272c  ', '--relation',
-0001e4c0: 2027 3334 3527 5d2c 0a20 2020 2020 2020   '345'],.       
-0001e4d0: 205d 290a 0a20 2020 2064 6566 2074 6573   ])..    def tes
-0001e4e0: 745f 7265 6d6f 7665 5f72 6576 6973 696f  t_remove_revisio
-0001e4f0: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
-0001e500: 2066 616b 655f 7363 7269 7074 2873 656c   fake_script(sel
-0001e510: 662c 2027 7365 6372 6574 2d72 656d 6f76  f, 'secret-remov
-0001e520: 6527 2c20 2222 2265 7869 7420 3022 2222  e', """exit 0"""
-0001e530: 290a 2020 2020 2020 2020 6661 6b65 5f73  ).        fake_s
-0001e540: 6372 6970 7428 7365 6c66 2c20 2773 6563  cript(self, 'sec
-0001e550: 7265 742d 696e 666f 2d67 6574 272c 2022  ret-info-get', "
-0001e560: 2222 6563 686f 2027 7b22 7a22 3a20 7b22  ""echo '{"z": {"
-0001e570: 6c61 6265 6c22 3a20 2279 222c 2022 7265  label": "y", "re
-0001e580: 7669 7369 6f6e 223a 2037 7d7d 2722 2222  vision": 7}}'"""
-0001e590: 290a 0a20 2020 2020 2020 2073 6563 7265  )..        secre
-0001e5a0: 7420 3d20 7365 6c66 2e6d 616b 655f 7365  t = self.make_se
-0001e5b0: 6372 6574 2869 643d 2778 2729 0a20 2020  cret(id='x').   
-0001e5c0: 2020 2020 2073 6563 7265 742e 7265 6d6f       secret.remo
-0001e5d0: 7665 5f72 6576 6973 696f 6e28 3132 3329  ve_revision(123)
-0001e5e0: 0a0a 2020 2020 2020 2020 2320 4966 2073  ..        # If s
-0001e5f0: 6563 7265 7420 646f 6573 6e27 7420 6861  ecret doesn't ha
-0001e600: 7665 2061 6e20 4944 2c20 7765 276c 6c20  ve an ID, we'll 
-0001e610: 7275 6e20 7365 6372 6574 2d69 6e66 6f2d  run secret-info-
-0001e620: 6765 7420 746f 2066 6574 6368 2069 740a  get to fetch it.
-0001e630: 2020 2020 2020 2020 7365 6372 6574 203d          secret =
-0001e640: 2073 656c 662e 6d61 6b65 5f73 6563 7265   self.make_secre
-0001e650: 7428 6c61 6265 6c3d 2779 2729 0a20 2020  t(label='y').   
-0001e660: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0001e670: 4973 4e6f 6e65 2873 6563 7265 742e 6964  IsNone(secret.id
-0001e680: 290a 2020 2020 2020 2020 7365 6372 6574  ).        secret
-0001e690: 2e72 656d 6f76 655f 7265 7669 7369 6f6e  .remove_revision
-0001e6a0: 2832 3334 290a 2020 2020 2020 2020 7365  (234).        se
-0001e6b0: 6c66 2e61 7373 6572 7445 7175 616c 2873  lf.assertEqual(s
-0001e6c0: 6563 7265 742e 6964 2c20 2773 6563 7265  ecret.id, 'secre
-0001e6d0: 743a 7a27 290a 0a20 2020 2020 2020 2073  t:z')..        s
-0001e6e0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0001e6f0: 6661 6b65 5f73 6372 6970 745f 6361 6c6c  fake_script_call
-0001e700: 7328 7365 6c66 2c20 636c 6561 723d 5472  s(self, clear=Tr
-0001e710: 7565 292c 205b 0a20 2020 2020 2020 2020  ue), [.         
-0001e720: 2020 205b 2773 6563 7265 742d 7265 6d6f     ['secret-remo
-0001e730: 7665 272c 2027 7365 6372 6574 3a78 272c  ve', 'secret:x',
-0001e740: 2027 2d2d 7265 7669 7369 6f6e 272c 2027   '--revision', '
-0001e750: 3132 3327 5d2c 0a20 2020 2020 2020 2020  123'],.         
-0001e760: 2020 205b 2773 6563 7265 742d 696e 666f     ['secret-info
-0001e770: 2d67 6574 272c 2027 2d2d 6c61 6265 6c27  -get', '--label'
-0001e780: 2c20 2779 272c 2027 2d2d 666f 726d 6174  , 'y', '--format
-0001e790: 3d6a 736f 6e27 5d2c 0a20 2020 2020 2020  =json'],.       
-0001e7a0: 2020 2020 205b 2773 6563 7265 742d 7265       ['secret-re
-0001e7b0: 6d6f 7665 272c 2027 7365 6372 6574 3a7a  move', 'secret:z
-0001e7c0: 272c 2027 2d2d 7265 7669 7369 6f6e 272c  ', '--revision',
-0001e7d0: 2027 3233 3427 5d2c 0a20 2020 2020 2020   '234'],.       
-0001e7e0: 205d 290a 0a20 2020 2064 6566 2074 6573   ])..    def tes
-0001e7f0: 745f 7265 6d6f 7665 5f61 6c6c 5f72 6576  t_remove_all_rev
-0001e800: 6973 696f 6e73 2873 656c 6629 3a0a 2020  isions(self):.  
-0001e810: 2020 2020 2020 6661 6b65 5f73 6372 6970        fake_scrip
-0001e820: 7428 7365 6c66 2c20 2773 6563 7265 742d  t(self, 'secret-
-0001e830: 7265 6d6f 7665 272c 2022 2222 6578 6974  remove', """exit
-0001e840: 2030 2222 2229 0a20 2020 2020 2020 2066   0""").        f
-0001e850: 616b 655f 7363 7269 7074 2873 656c 662c  ake_script(self,
-0001e860: 2027 7365 6372 6574 2d69 6e66 6f2d 6765   'secret-info-ge
-0001e870: 7427 2c20 2222 2265 6368 6f20 277b 227a  t', """echo '{"z
-0001e880: 223a 207b 226c 6162 656c 223a 2022 7922  ": {"label": "y"
-0001e890: 2c20 2272 6576 6973 696f 6e22 3a20 377d  , "revision": 7}
-0001e8a0: 7d27 2222 2229 0a0a 2020 2020 2020 2020  }'""")..        
-0001e8b0: 7365 6372 6574 203d 2073 656c 662e 6d61  secret = self.ma
-0001e8c0: 6b65 5f73 6563 7265 7428 6964 3d27 7827  ke_secret(id='x'
-0001e8d0: 290a 2020 2020 2020 2020 7365 6372 6574  ).        secret
-0001e8e0: 2e72 656d 6f76 655f 616c 6c5f 7265 7669  .remove_all_revi
-0001e8f0: 7369 6f6e 7328 290a 0a20 2020 2020 2020  sions()..       
-0001e900: 2023 2049 6620 7365 6372 6574 2064 6f65   # If secret doe
-0001e910: 736e 2774 2068 6176 6520 616e 2049 442c  sn't have an ID,
-0001e920: 2077 6527 6c6c 2072 756e 2073 6563 7265   we'll run secre
-0001e930: 742d 696e 666f 2d67 6574 2074 6f20 6665  t-info-get to fe
-0001e940: 7463 6820 6974 0a20 2020 2020 2020 2073  tch it.        s
-0001e950: 6563 7265 7420 3d20 7365 6c66 2e6d 616b  ecret = self.mak
-0001e960: 655f 7365 6372 6574 286c 6162 656c 3d27  e_secret(label='
-0001e970: 7927 290a 2020 2020 2020 2020 7365 6c66  y').        self
-0001e980: 2e61 7373 6572 7449 734e 6f6e 6528 7365  .assertIsNone(se
-0001e990: 6372 6574 2e69 6429 0a20 2020 2020 2020  cret.id).       
-0001e9a0: 2073 6563 7265 742e 7265 6d6f 7665 5f61   secret.remove_a
-0001e9b0: 6c6c 5f72 6576 6973 696f 6e73 2829 0a20  ll_revisions(). 
-0001e9c0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0001e9d0: 7274 4571 7561 6c28 7365 6372 6574 2e69  rtEqual(secret.i
-0001e9e0: 642c 2027 7365 6372 6574 3a7a 2729 0a0a  d, 'secret:z')..
-0001e9f0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0001ea00: 6572 7445 7175 616c 2866 616b 655f 7363  ertEqual(fake_sc
-0001ea10: 7269 7074 5f63 616c 6c73 2873 656c 662c  ript_calls(self,
-0001ea20: 2063 6c65 6172 3d54 7275 6529 2c20 5b0a   clear=True), [.
-0001ea30: 2020 2020 2020 2020 2020 2020 5b27 7365              ['se
-0001ea40: 6372 6574 2d72 656d 6f76 6527 2c20 2773  cret-remove', 's
-0001ea50: 6563 7265 743a 7827 5d2c 0a20 2020 2020  ecret:x'],.     
-0001ea60: 2020 2020 2020 205b 2773 6563 7265 742d         ['secret-
-0001ea70: 696e 666f 2d67 6574 272c 2027 2d2d 6c61  info-get', '--la
-0001ea80: 6265 6c27 2c20 2779 272c 2027 2d2d 666f  bel', 'y', '--fo
-0001ea90: 726d 6174 3d6a 736f 6e27 5d2c 0a20 2020  rmat=json'],.   
-0001eaa0: 2020 2020 2020 2020 205b 2773 6563 7265           ['secre
-0001eab0: 742d 7265 6d6f 7665 272c 2027 7365 6372  t-remove', 'secr
-0001eac0: 6574 3a7a 275d 2c0a 2020 2020 2020 2020  et:z'],.        
-0001ead0: 5d29 0a0a 0a63 6c61 7373 2054 6573 7450  ])...class TestP
-0001eae0: 6f72 7473 2875 6e69 7474 6573 742e 5465  orts(unittest.Te
-0001eaf0: 7374 4361 7365 293a 0a20 2020 2064 6566  stCase):.    def
-0001eb00: 2073 6574 5570 2873 656c 6629 3a0a 2020   setUp(self):.  
-0001eb10: 2020 2020 2020 7365 6c66 2e6d 6f64 656c        self.model
-0001eb20: 203d 206f 7073 2e6d 6f64 656c 2e4d 6f64   = ops.model.Mod
-0001eb30: 656c 286f 7073 2e63 6861 726d 2e43 6861  el(ops.charm.Cha
-0001eb40: 726d 4d65 7461 2829 2c20 6f70 732e 6d6f  rmMeta(), ops.mo
-0001eb50: 6465 6c2e 5f4d 6f64 656c 4261 636b 656e  del._ModelBacken
-0001eb60: 6428 276d 7961 7070 2f30 2729 290a 2020  d('myapp/0')).  
-0001eb70: 2020 2020 2020 7365 6c66 2e75 6e69 7420        self.unit 
-0001eb80: 3d20 7365 6c66 2e6d 6f64 656c 2e75 6e69  = self.model.uni
-0001eb90: 740a 0a20 2020 2064 6566 2074 6573 745f  t..    def test_
-0001eba0: 6f70 656e 5f70 6f72 7428 7365 6c66 293a  open_port(self):
-0001ebb0: 0a20 2020 2020 2020 2066 616b 655f 7363  .        fake_sc
-0001ebc0: 7269 7074 2873 656c 662c 2027 6f70 656e  ript(self, 'open
-0001ebd0: 2d70 6f72 7427 2c20 2765 7869 7420 3027  -port', 'exit 0'
-0001ebe0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0001ebf0: 756e 6974 2e6f 7065 6e5f 706f 7274 2827  unit.open_port('
-0001ec00: 7463 7027 2c20 3830 3830 290a 2020 2020  tcp', 8080).    
-0001ec10: 2020 2020 7365 6c66 2e75 6e69 742e 6f70      self.unit.op
-0001ec20: 656e 5f70 6f72 7428 2755 4450 272c 2034  en_port('UDP', 4
-0001ec30: 3030 3029 0a20 2020 2020 2020 2073 656c  000).        sel
-0001ec40: 662e 756e 6974 2e6f 7065 6e5f 706f 7274  f.unit.open_port
-0001ec50: 2827 6963 6d70 2729 0a0a 2020 2020 2020  ('icmp')..      
-0001ec60: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0001ec70: 616c 2866 616b 655f 7363 7269 7074 5f63  al(fake_script_c
-0001ec80: 616c 6c73 2873 656c 662c 2063 6c65 6172  alls(self, clear
-0001ec90: 3d54 7275 6529 2c20 5b0a 2020 2020 2020  =True), [.      
-0001eca0: 2020 2020 2020 5b27 6f70 656e 2d70 6f72        ['open-por
-0001ecb0: 7427 2c20 2738 3038 302f 7463 7027 5d2c  t', '8080/tcp'],
-0001ecc0: 0a20 2020 2020 2020 2020 2020 205b 276f  .            ['o
-0001ecd0: 7065 6e2d 706f 7274 272c 2027 3430 3030  pen-port', '4000
-0001ece0: 2f75 6470 275d 2c0a 2020 2020 2020 2020  /udp'],.        
-0001ecf0: 2020 2020 5b27 6f70 656e 2d70 6f72 7427      ['open-port'
-0001ed00: 2c20 2769 636d 7027 5d2c 0a20 2020 2020  , 'icmp'],.     
-0001ed10: 2020 205d 290a 0a20 2020 2064 6566 2074     ])..    def t
-0001ed20: 6573 745f 6f70 656e 5f70 6f72 745f 6572  est_open_port_er
-0001ed30: 726f 7228 7365 6c66 293a 0a20 2020 2020  ror(self):.     
-0001ed40: 2020 2066 616b 655f 7363 7269 7074 2873     fake_script(s
-0001ed50: 656c 662c 2027 6f70 656e 2d70 6f72 7427  elf, 'open-port'
-0001ed60: 2c20 2265 6368 6f20 2745 5252 4f52 2062  , "echo 'ERROR b
-0001ed70: 6164 2070 726f 746f 636f 6c27 203e 2632  ad protocol' >&2
-0001ed80: 3b20 6578 6974 2031 2229 0a0a 2020 2020  ; exit 1")..    
-0001ed90: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
-0001eda0: 7365 7274 5261 6973 6573 286f 7073 2e4d  sertRaises(ops.M
-0001edb0: 6f64 656c 4572 726f 7229 2061 7320 636d  odelError) as cm
-0001edc0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0001edd0: 6c66 2e75 6e69 742e 6f70 656e 5f70 6f72  lf.unit.open_por
-0001ede0: 7428 2766 7470 272c 2038 3038 3029 0a20  t('ftp', 8080). 
-0001edf0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0001ee00: 7274 4571 7561 6c28 7374 7228 636d 2e65  rtEqual(str(cm.e
-0001ee10: 7863 6570 7469 6f6e 292c 2027 4552 524f  xception), 'ERRO
-0001ee20: 5220 6261 6420 7072 6f74 6f63 6f6c 5c6e  R bad protocol\n
-0001ee30: 2729 0a0a 2020 2020 2020 2020 7365 6c66  ')..        self
-0001ee40: 2e61 7373 6572 7445 7175 616c 2866 616b  .assertEqual(fak
-0001ee50: 655f 7363 7269 7074 5f63 616c 6c73 2873  e_script_calls(s
-0001ee60: 656c 662c 2063 6c65 6172 3d54 7275 6529  elf, clear=True)
-0001ee70: 2c20 5b0a 2020 2020 2020 2020 2020 2020  , [.            
-0001ee80: 5b27 6f70 656e 2d70 6f72 7427 2c20 2738  ['open-port', '8
-0001ee90: 3038 302f 6674 7027 5d2c 0a20 2020 2020  080/ftp'],.     
-0001eea0: 2020 205d 290a 0a20 2020 2064 6566 2074     ])..    def t
-0001eeb0: 6573 745f 636c 6f73 655f 706f 7274 2873  est_close_port(s
-0001eec0: 656c 6629 3a0a 2020 2020 2020 2020 6661  elf):.        fa
-0001eed0: 6b65 5f73 6372 6970 7428 7365 6c66 2c20  ke_script(self, 
-0001eee0: 2763 6c6f 7365 2d70 6f72 7427 2c20 2765  'close-port', 'e
-0001eef0: 7869 7420 3027 290a 0a20 2020 2020 2020  xit 0')..       
-0001ef00: 2073 656c 662e 756e 6974 2e63 6c6f 7365   self.unit.close
-0001ef10: 5f70 6f72 7428 2774 6370 272c 2038 3038  _port('tcp', 808
-0001ef20: 3029 0a20 2020 2020 2020 2073 656c 662e  0).        self.
-0001ef30: 756e 6974 2e63 6c6f 7365 5f70 6f72 7428  unit.close_port(
-0001ef40: 2755 4450 272c 2034 3030 3029 0a20 2020  'UDP', 4000).   
-0001ef50: 2020 2020 2073 656c 662e 756e 6974 2e63       self.unit.c
-0001ef60: 6c6f 7365 5f70 6f72 7428 2769 636d 7027  lose_port('icmp'
-0001ef70: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0001ef80: 6173 7365 7274 4571 7561 6c28 6661 6b65  assertEqual(fake
-0001ef90: 5f73 6372 6970 745f 6361 6c6c 7328 7365  _script_calls(se
-0001efa0: 6c66 2c20 636c 6561 723d 5472 7565 292c  lf, clear=True),
-0001efb0: 205b 0a20 2020 2020 2020 2020 2020 205b   [.            [
-0001efc0: 2763 6c6f 7365 2d70 6f72 7427 2c20 2738  'close-port', '8
-0001efd0: 3038 302f 7463 7027 5d2c 0a20 2020 2020  080/tcp'],.     
-0001efe0: 2020 2020 2020 205b 2763 6c6f 7365 2d70         ['close-p
-0001eff0: 6f72 7427 2c20 2734 3030 302f 7564 7027  ort', '4000/udp'
-0001f000: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-0001f010: 2763 6c6f 7365 2d70 6f72 7427 2c20 2769  'close-port', 'i
-0001f020: 636d 7027 5d2c 0a20 2020 2020 2020 205d  cmp'],.        ]
-0001f030: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-0001f040: 636c 6f73 655f 706f 7274 5f65 7272 6f72  close_port_error
-0001f050: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0001f060: 6661 6b65 5f73 6372 6970 7428 7365 6c66  fake_script(self
-0001f070: 2c20 2763 6c6f 7365 2d70 6f72 7427 2c20  , 'close-port', 
-0001f080: 2265 6368 6f20 2745 5252 4f52 2062 6164  "echo 'ERROR bad
-0001f090: 2070 726f 746f 636f 6c27 203e 2632 3b20   protocol' >&2; 
-0001f0a0: 6578 6974 2031 2229 0a0a 2020 2020 2020  exit 1")..      
-0001f0b0: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
-0001f0c0: 7274 5261 6973 6573 286f 7073 2e4d 6f64  rtRaises(ops.Mod
-0001f0d0: 656c 4572 726f 7229 2061 7320 636d 3a0a  elError) as cm:.
-0001f0e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001f0f0: 2e75 6e69 742e 636c 6f73 655f 706f 7274  .unit.close_port
-0001f100: 2827 6674 7027 2c20 3830 3830 290a 2020  ('ftp', 8080).  
-0001f110: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0001f120: 7445 7175 616c 2873 7472 2863 6d2e 6578  tEqual(str(cm.ex
-0001f130: 6365 7074 696f 6e29 2c20 2745 5252 4f52  ception), 'ERROR
-0001f140: 2062 6164 2070 726f 746f 636f 6c5c 6e27   bad protocol\n'
-0001f150: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0001f160: 6173 7365 7274 4571 7561 6c28 6661 6b65  assertEqual(fake
-0001f170: 5f73 6372 6970 745f 6361 6c6c 7328 7365  _script_calls(se
-0001f180: 6c66 2c20 636c 6561 723d 5472 7565 292c  lf, clear=True),
-0001f190: 205b 0a20 2020 2020 2020 2020 2020 205b   [.            [
-0001f1a0: 2763 6c6f 7365 2d70 6f72 7427 2c20 2738  'close-port', '8
-0001f1b0: 3038 302f 6674 7027 5d2c 0a20 2020 2020  080/ftp'],.     
-0001f1c0: 2020 205d 290a 0a20 2020 2064 6566 2074     ])..    def t
-0001f1d0: 6573 745f 6f70 656e 6564 5f70 6f72 7473  est_opened_ports
-0001f1e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0001f1f0: 6661 6b65 5f73 6372 6970 7428 7365 6c66  fake_script(self
-0001f200: 2c20 276f 7065 6e65 642d 706f 7274 7327  , 'opened-ports'
-0001f210: 2c20 2222 2265 6368 6f20 3830 3830 2f74  , """echo 8080/t
-0001f220: 6370 3b20 6563 686f 2069 636d 7022 2222  cp; echo icmp"""
-0001f230: 290a 0a20 2020 2020 2020 2070 6f72 7473  )..        ports
-0001f240: 5f73 6574 203d 2073 656c 662e 756e 6974  _set = self.unit
-0001f250: 2e6f 7065 6e65 645f 706f 7274 7328 290a  .opened_ports().
-0001f260: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0001f270: 6572 7449 7349 6e73 7461 6e63 6528 706f  ertIsInstance(po
-0001f280: 7274 735f 7365 742c 2073 6574 290a 2020  rts_set, set).  
-0001f290: 2020 2020 2020 706f 7274 7320 3d20 736f        ports = so
-0001f2a0: 7274 6564 2870 6f72 7473 5f73 6574 2c20  rted(ports_set, 
-0001f2b0: 6b65 793d 6c61 6d62 6461 2070 3a20 2870  key=lambda p: (p
-0001f2c0: 2e70 726f 746f 636f 6c2c 2070 2e70 6f72  .protocol, p.por
-0001f2d0: 7429 290a 2020 2020 2020 2020 7365 6c66  t)).        self
-0001f2e0: 2e61 7373 6572 7445 7175 616c 286c 656e  .assertEqual(len
-0001f2f0: 2870 6f72 7473 292c 2032 290a 2020 2020  (ports), 2).    
-0001f300: 2020 2020 7365 6c66 2e61 7373 6572 7449      self.assertI
-0001f310: 7349 6e73 7461 6e63 6528 706f 7274 735b  sInstance(ports[
-0001f320: 305d 2c20 6f70 732e 4f70 656e 6564 506f  0], ops.OpenedPo
-0001f330: 7274 290a 2020 2020 2020 2020 7365 6c66  rt).        self
-0001f340: 2e61 7373 6572 7445 7175 616c 2870 6f72  .assertEqual(por
-0001f350: 7473 5b30 5d2e 7072 6f74 6f63 6f6c 2c20  ts[0].protocol, 
-0001f360: 2769 636d 7027 290a 2020 2020 2020 2020  'icmp').        
-0001f370: 7365 6c66 2e61 7373 6572 7449 734e 6f6e  self.assertIsNon
-0001f380: 6528 706f 7274 735b 305d 2e70 6f72 7429  e(ports[0].port)
-0001f390: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0001f3a0: 7365 7274 4973 496e 7374 616e 6365 2870  sertIsInstance(p
-0001f3b0: 6f72 7473 5b31 5d2c 206f 7073 2e4f 7065  orts[1], ops.Ope
-0001f3c0: 6e65 6450 6f72 7429 0a20 2020 2020 2020  nedPort).       
-0001f3d0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0001f3e0: 6c28 706f 7274 735b 315d 2e70 726f 746f  l(ports[1].proto
-0001f3f0: 636f 6c2c 2027 7463 7027 290a 2020 2020  col, 'tcp').    
-0001f400: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0001f410: 7175 616c 2870 6f72 7473 5b31 5d2e 706f  qual(ports[1].po
-0001f420: 7274 2c20 3830 3830 290a 0a20 2020 2020  rt, 8080)..     
-0001f430: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0001f440: 7561 6c28 6661 6b65 5f73 6372 6970 745f  ual(fake_script_
-0001f450: 6361 6c6c 7328 7365 6c66 2c20 636c 6561  calls(self, clea
-0001f460: 723d 5472 7565 292c 205b 0a20 2020 2020  r=True), [.     
-0001f470: 2020 2020 2020 205b 276f 7065 6e65 642d         ['opened-
-0001f480: 706f 7274 7327 2c20 2727 5d2c 0a20 2020  ports', ''],.   
-0001f490: 2020 2020 205d 290a 0a20 2020 2064 6566       ])..    def
-0001f4a0: 2074 6573 745f 6f70 656e 6564 5f70 6f72   test_opened_por
-0001f4b0: 7473 5f77 6172 6e69 6e67 7328 7365 6c66  ts_warnings(self
-0001f4c0: 293a 0a20 2020 2020 2020 2066 616b 655f  ):.        fake_
-0001f4d0: 7363 7269 7074 2873 656c 662c 2027 6f70  script(self, 'op
-0001f4e0: 656e 6564 2d70 6f72 7473 272c 2022 2222  ened-ports', """
-0001f4f0: 6563 686f 2038 3038 302f 7463 703b 2065  echo 8080/tcp; e
-0001f500: 6368 6f20 3132 3334 2f66 7470 3b20 6563  cho 1234/ftp; ec
-0001f510: 686f 2031 3030 302d 3230 3030 2f75 6470  ho 1000-2000/udp
-0001f520: 2222 2229 0a0a 2020 2020 2020 2020 7769  """)..        wi
-0001f530: 7468 2073 656c 662e 6173 7365 7274 4c6f  th self.assertLo
-0001f540: 6773 2827 6f70 732e 6d6f 6465 6c27 2c20  gs('ops.model', 
-0001f550: 6c65 7665 6c3d 2757 4152 4e49 4e47 2729  level='WARNING')
-0001f560: 2061 7320 636d 3a0a 2020 2020 2020 2020   as cm:.        
-0001f570: 2020 2020 706f 7274 735f 7365 7420 3d20      ports_set = 
-0001f580: 7365 6c66 2e75 6e69 742e 6f70 656e 6564  self.unit.opened
-0001f590: 5f70 6f72 7473 2829 0a20 2020 2020 2020  _ports().       
-0001f5a0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0001f5b0: 6c28 6c65 6e28 636d 2e6f 7574 7075 7429  l(len(cm.output)
-0001f5c0: 2c20 3229 0a20 2020 2020 2020 2073 656c  , 2).        sel
-0001f5d0: 662e 6173 7365 7274 5265 6765 7828 636d  f.assertRegex(cm
-0001f5e0: 2e6f 7574 7075 745b 305d 2c20 7227 5741  .output[0], r'WA
-0001f5f0: 524e 494e 473a 6f70 732e 6d6f 6465 6c3a  RNING:ops.model:
-0001f600: 2e2a 7072 6f74 6f63 6f6c 2e2a 2729 0a20  .*protocol.*'). 
-0001f610: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0001f620: 7274 5265 6765 7828 636d 2e6f 7574 7075  rtRegex(cm.outpu
-0001f630: 745b 315d 2c20 7227 5741 524e 494e 473a  t[1], r'WARNING:
-0001f640: 6f70 732e 6d6f 6465 6c3a 2e2a 7261 6e67  ops.model:.*rang
-0001f650: 652e 2a27 290a 0a20 2020 2020 2020 2073  e.*')..        s
-0001f660: 656c 662e 6173 7365 7274 4973 496e 7374  elf.assertIsInst
-0001f670: 616e 6365 2870 6f72 7473 5f73 6574 2c20  ance(ports_set, 
-0001f680: 7365 7429 0a20 2020 2020 2020 2070 6f72  set).        por
-0001f690: 7473 203d 2073 6f72 7465 6428 706f 7274  ts = sorted(port
-0001f6a0: 735f 7365 742c 206b 6579 3d6c 616d 6264  s_set, key=lambd
-0001f6b0: 6120 703a 2028 702e 7072 6f74 6f63 6f6c  a p: (p.protocol
-0001f6c0: 2c20 702e 706f 7274 2929 0a20 2020 2020  , p.port)).     
-0001f6d0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0001f6e0: 7561 6c28 6c65 6e28 706f 7274 7329 2c20  ual(len(ports), 
-0001f6f0: 3229 0a20 2020 2020 2020 2073 656c 662e  2).        self.
-0001f700: 6173 7365 7274 4973 496e 7374 616e 6365  assertIsInstance
-0001f710: 2870 6f72 7473 5b30 5d2c 206f 7073 2e4f  (ports[0], ops.O
-0001f720: 7065 6e65 6450 6f72 7429 0a20 2020 2020  penedPort).     
-0001f730: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0001f740: 7561 6c28 706f 7274 735b 305d 2e70 726f  ual(ports[0].pro
-0001f750: 746f 636f 6c2c 2027 7463 7027 290a 2020  tocol, 'tcp').  
-0001f760: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0001f770: 7445 7175 616c 2870 6f72 7473 5b30 5d2e  tEqual(ports[0].
-0001f780: 706f 7274 2c20 3830 3830 290a 2020 2020  port, 8080).    
-0001f790: 2020 2020 7365 6c66 2e61 7373 6572 7449      self.assertI
-0001f7a0: 7349 6e73 7461 6e63 6528 706f 7274 735b  sInstance(ports[
-0001f7b0: 315d 2c20 6f70 732e 4f70 656e 6564 506f  1], ops.OpenedPo
-0001f7c0: 7274 290a 2020 2020 2020 2020 7365 6c66  rt).        self
-0001f7d0: 2e61 7373 6572 7445 7175 616c 2870 6f72  .assertEqual(por
-0001f7e0: 7473 5b31 5d2e 7072 6f74 6f63 6f6c 2c20  ts[1].protocol, 
-0001f7f0: 2775 6470 2729 0a20 2020 2020 2020 2073  'udp').        s
-0001f800: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0001f810: 706f 7274 735b 315d 2e70 6f72 742c 2031  ports[1].port, 1
-0001f820: 3030 3029 0a0a 2020 2020 2020 2020 7365  000)..        se
-0001f830: 6c66 2e61 7373 6572 7445 7175 616c 2866  lf.assertEqual(f
-0001f840: 616b 655f 7363 7269 7074 5f63 616c 6c73  ake_script_calls
-0001f850: 2873 656c 662c 2063 6c65 6172 3d54 7275  (self, clear=Tru
-0001f860: 6529 2c20 5b0a 2020 2020 2020 2020 2020  e), [.          
-0001f870: 2020 5b27 6f70 656e 6564 2d70 6f72 7473    ['opened-ports
-0001f880: 272c 2027 275d 2c0a 2020 2020 2020 2020  ', ''],.        
-0001f890: 5d29 0a0a 0a69 6620 5f5f 6e61 6d65 5f5f  ])...if __name__
-0001f8a0: 203d 3d20 225f 5f6d 6169 6e5f 5f22 3a0a   == "__main__":.
-0001f8b0: 2020 2020 756e 6974 7465 7374 2e6d 6169      unittest.mai
-0001f8c0: 6e28 290a                                n().
+0001d850: 2c20 2773 6563 7265 743a 7827 2c20 272d  , 'secret:x', '-
+0001d860: 2d66 6f72 6d61 743d 6a73 6f6e 275d 2c0a  -format=json'],.
+0001d870: 2020 2020 2020 2020 2020 2020 5d29 0a0a              ])..
+0001d880: 2020 2020 6465 6620 7465 7374 5f73 6574      def test_set
+0001d890: 5f63 6f6e 7465 6e74 2873 656c 6629 3a0a  _content(self):.
+0001d8a0: 2020 2020 2020 2020 6661 6b65 5f73 6372          fake_scr
+0001d8b0: 6970 7428 7365 6c66 2c20 2773 6563 7265  ipt(self, 'secre
+0001d8c0: 742d 7365 7427 2c20 2222 2265 7869 7420  t-set', """exit 
+0001d8d0: 3022 2222 290a 2020 2020 2020 2020 6661  0""").        fa
+0001d8e0: 6b65 5f73 6372 6970 7428 7365 6c66 2c20  ke_script(self, 
+0001d8f0: 2773 6563 7265 742d 696e 666f 2d67 6574  'secret-info-get
+0001d900: 272c 2022 2222 6563 686f 2027 7b22 7a22  ', """echo '{"z"
+0001d910: 3a20 7b22 6c61 6265 6c22 3a20 2279 222c  : {"label": "y",
+0001d920: 2022 7265 7669 7369 6f6e 223a 2037 7d7d   "revision": 7}}
+0001d930: 2722 2222 290a 0a20 2020 2020 2020 2073  '""")..        s
+0001d940: 6563 7265 7420 3d20 7365 6c66 2e6d 616b  ecret = self.mak
+0001d950: 655f 7365 6372 6574 2869 643d 2778 2729  e_secret(id='x')
+0001d960: 0a20 2020 2020 2020 2073 6563 7265 742e  .        secret.
+0001d970: 7365 745f 636f 6e74 656e 7428 7b27 666f  set_content({'fo
+0001d980: 6f27 3a20 2762 6172 277d 290a 0a20 2020  o': 'bar'})..   
+0001d990: 2020 2020 2023 2049 6620 7365 6372 6574       # If secret
+0001d9a0: 2064 6f65 736e 2774 2068 6176 6520 616e   doesn't have an
+0001d9b0: 2049 442c 2077 6527 6c6c 2072 756e 2073   ID, we'll run s
+0001d9c0: 6563 7265 742d 696e 666f 2d67 6574 2074  ecret-info-get t
+0001d9d0: 6f20 6665 7463 6820 6974 0a20 2020 2020  o fetch it.     
+0001d9e0: 2020 2073 6563 7265 7420 3d20 7365 6c66     secret = self
+0001d9f0: 2e6d 616b 655f 7365 6372 6574 286c 6162  .make_secret(lab
+0001da00: 656c 3d27 7927 290a 2020 2020 2020 2020  el='y').        
+0001da10: 7365 6c66 2e61 7373 6572 7449 734e 6f6e  self.assertIsNon
+0001da20: 6528 7365 6372 6574 2e69 6429 0a20 2020  e(secret.id).   
+0001da30: 2020 2020 2073 6563 7265 742e 7365 745f       secret.set_
+0001da40: 636f 6e74 656e 7428 7b27 6261 7227 3a20  content({'bar': 
+0001da50: 2766 6f6f 277d 290a 2020 2020 2020 2020  'foo'}).        
+0001da60: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0001da70: 2873 6563 7265 742e 6964 2c20 2773 6563  (secret.id, 'sec
+0001da80: 7265 743a 7a27 290a 0a20 2020 2020 2020  ret:z')..       
+0001da90: 2077 6974 6820 7365 6c66 2e61 7373 6572   with self.asser
+0001daa0: 7452 6169 7365 7328 5661 6c75 6545 7272  tRaises(ValueErr
+0001dab0: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+0001dac0: 2073 6563 7265 742e 7365 745f 636f 6e74   secret.set_cont
+0001dad0: 656e 7428 7b27 7327 3a20 2774 277d 2920  ent({'s': 't'}) 
+0001dae0: 2023 2065 6e73 7572 6520 6974 2076 616c   # ensure it val
+0001daf0: 6964 6174 6573 2063 6f6e 7465 6e74 2028  idates content (
+0001db00: 6b65 7920 746f 6f20 7368 6f72 7429 0a0a  key too short)..
+0001db10: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0001db20: 6572 7445 7175 616c 2866 616b 655f 7363  ertEqual(fake_sc
+0001db30: 7269 7074 5f63 616c 6c73 2873 656c 662c  ript_calls(self,
+0001db40: 2063 6c65 6172 3d54 7275 6529 2c20 5b0a   clear=True), [.
+0001db50: 2020 2020 2020 2020 2020 2020 5b27 7365              ['se
+0001db60: 6372 6574 2d73 6574 272c 2027 7365 6372  cret-set', 'secr
+0001db70: 6574 3a78 272c 2027 666f 6f3d 6261 7227  et:x', 'foo=bar'
+0001db80: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
+0001db90: 2773 6563 7265 742d 696e 666f 2d67 6574  'secret-info-get
+0001dba0: 272c 2027 2d2d 6c61 6265 6c27 2c20 2779  ', '--label', 'y
+0001dbb0: 272c 2027 2d2d 666f 726d 6174 3d6a 736f  ', '--format=jso
+0001dbc0: 6e27 5d2c 0a20 2020 2020 2020 2020 2020  n'],.           
+0001dbd0: 205b 2773 6563 7265 742d 7365 7427 2c20   ['secret-set', 
+0001dbe0: 2773 6563 7265 743a 7a27 2c20 2762 6172  'secret:z', 'bar
+0001dbf0: 3d66 6f6f 275d 2c0a 2020 2020 2020 2020  =foo'],.        
+0001dc00: 5d29 0a0a 2020 2020 6465 6620 7465 7374  ])..    def test
+0001dc10: 5f73 6574 5f69 6e66 6f28 7365 6c66 293a  _set_info(self):
+0001dc20: 0a20 2020 2020 2020 2066 616b 655f 7363  .        fake_sc
+0001dc30: 7269 7074 2873 656c 662c 2027 7365 6372  ript(self, 'secr
+0001dc40: 6574 2d73 6574 272c 2022 2222 6578 6974  et-set', """exit
+0001dc50: 2030 2222 2229 0a20 2020 2020 2020 2066   0""").        f
+0001dc60: 616b 655f 7363 7269 7074 2873 656c 662c  ake_script(self,
+0001dc70: 2027 7365 6372 6574 2d69 6e66 6f2d 6765   'secret-info-ge
+0001dc80: 7427 2c20 2222 2265 6368 6f20 277b 227a  t', """echo '{"z
+0001dc90: 223a 207b 226c 6162 656c 223a 2022 7922  ": {"label": "y"
+0001dca0: 2c20 2272 6576 6973 696f 6e22 3a20 377d  , "revision": 7}
+0001dcb0: 7d27 2222 2229 0a0a 2020 2020 2020 2020  }'""")..        
+0001dcc0: 7365 6372 6574 203d 2073 656c 662e 6d61  secret = self.ma
+0001dcd0: 6b65 5f73 6563 7265 7428 6964 3d27 7827  ke_secret(id='x'
+0001dce0: 290a 2020 2020 2020 2020 6578 7069 7265  ).        expire
+0001dcf0: 203d 2064 6174 6574 696d 652e 6461 7465   = datetime.date
+0001dd00: 7469 6d65 2832 3032 322c 2031 322c 2039  time(2022, 12, 9
+0001dd10: 2c20 3136 2c20 3539 2c20 3029 0a20 2020  , 16, 59, 0).   
+0001dd20: 2020 2020 2073 6563 7265 742e 7365 745f       secret.set_
+0001dd30: 696e 666f 280a 2020 2020 2020 2020 2020  info(.          
+0001dd40: 2020 6c61 6265 6c3d 276c 6162 272c 0a20    label='lab',. 
+0001dd50: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+0001dd60: 6970 7469 6f6e 3d27 6465 7363 272c 0a20  iption='desc',. 
+0001dd70: 2020 2020 2020 2020 2020 2065 7870 6972             expir
+0001dd80: 653d 6578 7069 7265 2c0a 2020 2020 2020  e=expire,.      
+0001dd90: 2020 2020 2020 726f 7461 7465 3d6f 7073        rotate=ops
+0001dda0: 2e53 6563 7265 7452 6f74 6174 652e 4d4f  .SecretRotate.MO
+0001ddb0: 4e54 484c 592c 0a20 2020 2020 2020 2029  NTHLY,.        )
+0001ddc0: 0a0a 2020 2020 2020 2020 2320 4966 2073  ..        # If s
+0001ddd0: 6563 7265 7420 646f 6573 6e27 7420 6861  ecret doesn't ha
+0001dde0: 7665 2061 6e20 4944 2c20 7765 276c 6c20  ve an ID, we'll 
+0001ddf0: 7275 6e20 7365 6372 6574 2d69 6e66 6f2d  run secret-info-
+0001de00: 6765 7420 746f 2066 6574 6368 2069 740a  get to fetch it.
+0001de10: 2020 2020 2020 2020 7365 6372 6574 203d          secret =
+0001de20: 2073 656c 662e 6d61 6b65 5f73 6563 7265   self.make_secre
+0001de30: 7428 6c61 6265 6c3d 2779 2729 0a20 2020  t(label='y').   
+0001de40: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001de50: 4973 4e6f 6e65 2873 6563 7265 742e 6964  IsNone(secret.id
+0001de60: 290a 2020 2020 2020 2020 7365 6372 6574  ).        secret
+0001de70: 2e73 6574 5f69 6e66 6f28 6c61 6265 6c3d  .set_info(label=
+0001de80: 276c 626c 2729 0a20 2020 2020 2020 2073  'lbl').        s
+0001de90: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001dea0: 7365 6372 6574 2e69 642c 2027 7365 6372  secret.id, 'secr
+0001deb0: 6574 3a7a 2729 0a0a 2020 2020 2020 2020  et:z')..        
+0001dec0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0001ded0: 2866 616b 655f 7363 7269 7074 5f63 616c  (fake_script_cal
+0001dee0: 6c73 2873 656c 662c 2063 6c65 6172 3d54  ls(self, clear=T
+0001def0: 7275 6529 2c20 5b0a 2020 2020 2020 2020  rue), [.        
+0001df00: 2020 2020 5b27 7365 6372 6574 2d73 6574      ['secret-set
+0001df10: 272c 2027 7365 6372 6574 3a78 272c 2027  ', 'secret:x', '
+0001df20: 2d2d 6c61 6265 6c27 2c20 276c 6162 272c  --label', 'lab',
+0001df30: 2027 2d2d 6465 7363 7269 7074 696f 6e27   '--description'
+0001df40: 2c20 2764 6573 6327 2c0a 2020 2020 2020  , 'desc',.      
+0001df50: 2020 2020 2020 2027 2d2d 6578 7069 7265         '--expire
+0001df60: 272c 2027 3230 3232 2d31 322d 3039 5431  ', '2022-12-09T1
+0001df70: 363a 3539 3a30 3027 2c20 272d 2d72 6f74  6:59:00', '--rot
+0001df80: 6174 6527 2c20 276d 6f6e 7468 6c79 275d  ate', 'monthly']
+0001df90: 2c0a 2020 2020 2020 2020 2020 2020 5b27  ,.            ['
+0001dfa0: 7365 6372 6574 2d69 6e66 6f2d 6765 7427  secret-info-get'
+0001dfb0: 2c20 272d 2d6c 6162 656c 272c 2027 7927  , '--label', 'y'
+0001dfc0: 2c20 272d 2d66 6f72 6d61 743d 6a73 6f6e  , '--format=json
+0001dfd0: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
+0001dfe0: 5b27 7365 6372 6574 2d73 6574 272c 2027  ['secret-set', '
+0001dff0: 7365 6372 6574 3a7a 272c 2027 2d2d 6c61  secret:z', '--la
+0001e000: 6265 6c27 2c20 276c 626c 275d 2c0a 2020  bel', 'lbl'],.  
+0001e010: 2020 2020 2020 5d29 0a0a 2020 2020 2020        ])..      
+0001e020: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
+0001e030: 7274 5261 6973 6573 2854 7970 6545 7272  rtRaises(TypeErr
+0001e040: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+0001e050: 2073 6563 7265 742e 7365 745f 696e 666f   secret.set_info
+0001e060: 2829 2020 2320 6e6f 2061 7267 7320 7072  ()  # no args pr
+0001e070: 6f76 6964 6564 0a0a 2020 2020 6465 6620  ovided..    def 
+0001e080: 7465 7374 5f67 7261 6e74 2873 656c 6629  test_grant(self)
+0001e090: 3a0a 2020 2020 2020 2020 6661 6b65 5f73  :.        fake_s
+0001e0a0: 6372 6970 7428 7365 6c66 2c20 2773 6563  cript(self, 'sec
+0001e0b0: 7265 742d 6772 616e 7427 2c20 2222 2265  ret-grant', """e
+0001e0c0: 7869 7420 3022 2222 290a 2020 2020 2020  xit 0""").      
+0001e0d0: 2020 6661 6b65 5f73 6372 6970 7428 7365    fake_script(se
+0001e0e0: 6c66 2c20 2773 6563 7265 742d 696e 666f  lf, 'secret-info
+0001e0f0: 2d67 6574 272c 2022 2222 6563 686f 2027  -get', """echo '
+0001e100: 7b22 7a22 3a20 7b22 6c61 6265 6c22 3a20  {"z": {"label": 
+0001e110: 2279 222c 2022 7265 7669 7369 6f6e 223a  "y", "revision":
+0001e120: 2037 7d7d 2722 2222 290a 0a20 2020 2020   7}}'""")..     
+0001e130: 2020 2073 6563 7265 7420 3d20 7365 6c66     secret = self
+0001e140: 2e6d 616b 655f 7365 6372 6574 2869 643d  .make_secret(id=
+0001e150: 2778 2729 0a20 2020 2020 2020 2073 6563  'x').        sec
+0001e160: 7265 742e 6772 616e 7428 7479 7065 732e  ret.grant(types.
+0001e170: 5369 6d70 6c65 4e61 6d65 7370 6163 6528  SimpleNamespace(
+0001e180: 6964 3d31 3233 2929 0a20 2020 2020 2020  id=123)).       
+0001e190: 2073 6563 7265 742e 6772 616e 7428 7479   secret.grant(ty
+0001e1a0: 7065 732e 5369 6d70 6c65 4e61 6d65 7370  pes.SimpleNamesp
+0001e1b0: 6163 6528 6964 3d32 3334 292c 2075 6e69  ace(id=234), uni
+0001e1c0: 743d 7479 7065 732e 5369 6d70 6c65 4e61  t=types.SimpleNa
+0001e1d0: 6d65 7370 6163 6528 6e61 6d65 3d27 6170  mespace(name='ap
+0001e1e0: 702f 3027 2929 0a0a 2020 2020 2020 2020  p/0'))..        
+0001e1f0: 2320 4966 2073 6563 7265 7420 646f 6573  # If secret does
+0001e200: 6e27 7420 6861 7665 2061 6e20 4944 2c20  n't have an ID, 
+0001e210: 7765 276c 6c20 7275 6e20 7365 6372 6574  we'll run secret
+0001e220: 2d69 6e66 6f2d 6765 7420 746f 2066 6574  -info-get to fet
+0001e230: 6368 2069 740a 2020 2020 2020 2020 7365  ch it.        se
+0001e240: 6372 6574 203d 2073 656c 662e 6d61 6b65  cret = self.make
+0001e250: 5f73 6563 7265 7428 6c61 6265 6c3d 2779  _secret(label='y
+0001e260: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+0001e270: 6173 7365 7274 4973 4e6f 6e65 2873 6563  assertIsNone(sec
+0001e280: 7265 742e 6964 290a 2020 2020 2020 2020  ret.id).        
+0001e290: 7365 6372 6574 2e67 7261 6e74 2874 7970  secret.grant(typ
+0001e2a0: 6573 2e53 696d 706c 654e 616d 6573 7061  es.SimpleNamespa
+0001e2b0: 6365 2869 643d 3334 3529 290a 2020 2020  ce(id=345)).    
+0001e2c0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0001e2d0: 7175 616c 2873 6563 7265 742e 6964 2c20  qual(secret.id, 
+0001e2e0: 2773 6563 7265 743a 7a27 290a 0a20 2020  'secret:z')..   
+0001e2f0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001e300: 4571 7561 6c28 6661 6b65 5f73 6372 6970  Equal(fake_scrip
+0001e310: 745f 6361 6c6c 7328 7365 6c66 2c20 636c  t_calls(self, cl
+0001e320: 6561 723d 5472 7565 292c 205b 0a20 2020  ear=True), [.   
+0001e330: 2020 2020 2020 2020 205b 2773 6563 7265           ['secre
+0001e340: 742d 6772 616e 7427 2c20 2773 6563 7265  t-grant', 'secre
+0001e350: 743a 7827 2c20 272d 2d72 656c 6174 696f  t:x', '--relatio
+0001e360: 6e27 2c20 2731 3233 275d 2c0a 2020 2020  n', '123'],.    
+0001e370: 2020 2020 2020 2020 5b27 7365 6372 6574          ['secret
+0001e380: 2d67 7261 6e74 272c 2027 7365 6372 6574  -grant', 'secret
+0001e390: 3a78 272c 2027 2d2d 7265 6c61 7469 6f6e  :x', '--relation
+0001e3a0: 272c 2027 3233 3427 2c20 272d 2d75 6e69  ', '234', '--uni
+0001e3b0: 7427 2c20 2761 7070 2f30 275d 2c0a 2020  t', 'app/0'],.  
+0001e3c0: 2020 2020 2020 2020 2020 5b27 7365 6372            ['secr
+0001e3d0: 6574 2d69 6e66 6f2d 6765 7427 2c20 272d  et-info-get', '-
+0001e3e0: 2d6c 6162 656c 272c 2027 7927 2c20 272d  -label', 'y', '-
+0001e3f0: 2d66 6f72 6d61 743d 6a73 6f6e 275d 2c0a  -format=json'],.
+0001e400: 2020 2020 2020 2020 2020 2020 5b27 7365              ['se
+0001e410: 6372 6574 2d67 7261 6e74 272c 2027 7365  cret-grant', 'se
+0001e420: 6372 6574 3a7a 272c 2027 2d2d 7265 6c61  cret:z', '--rela
+0001e430: 7469 6f6e 272c 2027 3334 3527 5d2c 0a20  tion', '345'],. 
+0001e440: 2020 2020 2020 205d 290a 0a20 2020 2064         ])..    d
+0001e450: 6566 2074 6573 745f 7265 766f 6b65 2873  ef test_revoke(s
+0001e460: 656c 6629 3a0a 2020 2020 2020 2020 6661  elf):.        fa
+0001e470: 6b65 5f73 6372 6970 7428 7365 6c66 2c20  ke_script(self, 
+0001e480: 2773 6563 7265 742d 7265 766f 6b65 272c  'secret-revoke',
+0001e490: 2022 2222 6578 6974 2030 2222 2229 0a20   """exit 0"""). 
+0001e4a0: 2020 2020 2020 2066 616b 655f 7363 7269         fake_scri
+0001e4b0: 7074 2873 656c 662c 2027 7365 6372 6574  pt(self, 'secret
+0001e4c0: 2d69 6e66 6f2d 6765 7427 2c20 2222 2265  -info-get', """e
+0001e4d0: 6368 6f20 277b 227a 223a 207b 226c 6162  cho '{"z": {"lab
+0001e4e0: 656c 223a 2022 7922 2c20 2272 6576 6973  el": "y", "revis
+0001e4f0: 696f 6e22 3a20 377d 7d27 2222 2229 0a0a  ion": 7}}'""")..
+0001e500: 2020 2020 2020 2020 7365 6372 6574 203d          secret =
+0001e510: 2073 656c 662e 6d61 6b65 5f73 6563 7265   self.make_secre
+0001e520: 7428 6964 3d27 7827 290a 2020 2020 2020  t(id='x').      
+0001e530: 2020 7365 6372 6574 2e72 6576 6f6b 6528    secret.revoke(
+0001e540: 7479 7065 732e 5369 6d70 6c65 4e61 6d65  types.SimpleName
+0001e550: 7370 6163 6528 6964 3d31 3233 2929 0a20  space(id=123)). 
+0001e560: 2020 2020 2020 2073 6563 7265 742e 7265         secret.re
+0001e570: 766f 6b65 2874 7970 6573 2e53 696d 706c  voke(types.Simpl
+0001e580: 654e 616d 6573 7061 6365 2869 643d 3233  eNamespace(id=23
+0001e590: 3429 2c20 756e 6974 3d74 7970 6573 2e53  4), unit=types.S
+0001e5a0: 696d 706c 654e 616d 6573 7061 6365 286e  impleNamespace(n
+0001e5b0: 616d 653d 2761 7070 2f30 2729 290a 0a20  ame='app/0')).. 
+0001e5c0: 2020 2020 2020 2023 2049 6620 7365 6372         # If secr
+0001e5d0: 6574 2064 6f65 736e 2774 2068 6176 6520  et doesn't have 
+0001e5e0: 616e 2049 442c 2077 6527 6c6c 2072 756e  an ID, we'll run
+0001e5f0: 2073 6563 7265 742d 696e 666f 2d67 6574   secret-info-get
+0001e600: 2074 6f20 6665 7463 6820 6974 0a20 2020   to fetch it.   
+0001e610: 2020 2020 2073 6563 7265 7420 3d20 7365       secret = se
+0001e620: 6c66 2e6d 616b 655f 7365 6372 6574 286c  lf.make_secret(l
+0001e630: 6162 656c 3d27 7927 290a 2020 2020 2020  abel='y').      
+0001e640: 2020 7365 6c66 2e61 7373 6572 7449 734e    self.assertIsN
+0001e650: 6f6e 6528 7365 6372 6574 2e69 6429 0a20  one(secret.id). 
+0001e660: 2020 2020 2020 2073 6563 7265 742e 7265         secret.re
+0001e670: 766f 6b65 2874 7970 6573 2e53 696d 706c  voke(types.Simpl
+0001e680: 654e 616d 6573 7061 6365 2869 643d 3334  eNamespace(id=34
+0001e690: 3529 290a 2020 2020 2020 2020 7365 6c66  5)).        self
+0001e6a0: 2e61 7373 6572 7445 7175 616c 2873 6563  .assertEqual(sec
+0001e6b0: 7265 742e 6964 2c20 2773 6563 7265 743a  ret.id, 'secret:
+0001e6c0: 7a27 290a 0a20 2020 2020 2020 2073 656c  z')..        sel
+0001e6d0: 662e 6173 7365 7274 4571 7561 6c28 6661  f.assertEqual(fa
+0001e6e0: 6b65 5f73 6372 6970 745f 6361 6c6c 7328  ke_script_calls(
+0001e6f0: 7365 6c66 2c20 636c 6561 723d 5472 7565  self, clear=True
+0001e700: 292c 205b 0a20 2020 2020 2020 2020 2020  ), [.           
+0001e710: 205b 2773 6563 7265 742d 7265 766f 6b65   ['secret-revoke
+0001e720: 272c 2027 7365 6372 6574 3a78 272c 2027  ', 'secret:x', '
+0001e730: 2d2d 7265 6c61 7469 6f6e 272c 2027 3132  --relation', '12
+0001e740: 3327 5d2c 0a20 2020 2020 2020 2020 2020  3'],.           
+0001e750: 205b 2773 6563 7265 742d 7265 766f 6b65   ['secret-revoke
+0001e760: 272c 2027 7365 6372 6574 3a78 272c 2027  ', 'secret:x', '
+0001e770: 2d2d 7265 6c61 7469 6f6e 272c 2027 3233  --relation', '23
+0001e780: 3427 2c20 272d 2d75 6e69 7427 2c20 2761  4', '--unit', 'a
+0001e790: 7070 2f30 275d 2c0a 2020 2020 2020 2020  pp/0'],.        
+0001e7a0: 2020 2020 5b27 7365 6372 6574 2d69 6e66      ['secret-inf
+0001e7b0: 6f2d 6765 7427 2c20 272d 2d6c 6162 656c  o-get', '--label
+0001e7c0: 272c 2027 7927 2c20 272d 2d66 6f72 6d61  ', 'y', '--forma
+0001e7d0: 743d 6a73 6f6e 275d 2c0a 2020 2020 2020  t=json'],.      
+0001e7e0: 2020 2020 2020 5b27 7365 6372 6574 2d72        ['secret-r
+0001e7f0: 6576 6f6b 6527 2c20 2773 6563 7265 743a  evoke', 'secret:
+0001e800: 7a27 2c20 272d 2d72 656c 6174 696f 6e27  z', '--relation'
+0001e810: 2c20 2733 3435 275d 2c0a 2020 2020 2020  , '345'],.      
+0001e820: 2020 5d29 0a0a 2020 2020 6465 6620 7465    ])..    def te
+0001e830: 7374 5f72 656d 6f76 655f 7265 7669 7369  st_remove_revisi
+0001e840: 6f6e 2873 656c 6629 3a0a 2020 2020 2020  on(self):.      
+0001e850: 2020 6661 6b65 5f73 6372 6970 7428 7365    fake_script(se
+0001e860: 6c66 2c20 2773 6563 7265 742d 7265 6d6f  lf, 'secret-remo
+0001e870: 7665 272c 2022 2222 6578 6974 2030 2222  ve', """exit 0""
+0001e880: 2229 0a20 2020 2020 2020 2066 616b 655f  ").        fake_
+0001e890: 7363 7269 7074 2873 656c 662c 2027 7365  script(self, 'se
+0001e8a0: 6372 6574 2d69 6e66 6f2d 6765 7427 2c20  cret-info-get', 
+0001e8b0: 2222 2265 6368 6f20 277b 227a 223a 207b  """echo '{"z": {
+0001e8c0: 226c 6162 656c 223a 2022 7922 2c20 2272  "label": "y", "r
+0001e8d0: 6576 6973 696f 6e22 3a20 377d 7d27 2222  evision": 7}}'""
+0001e8e0: 2229 0a0a 2020 2020 2020 2020 7365 6372  ")..        secr
+0001e8f0: 6574 203d 2073 656c 662e 6d61 6b65 5f73  et = self.make_s
+0001e900: 6563 7265 7428 6964 3d27 7827 290a 2020  ecret(id='x').  
+0001e910: 2020 2020 2020 7365 6372 6574 2e72 656d        secret.rem
+0001e920: 6f76 655f 7265 7669 7369 6f6e 2831 3233  ove_revision(123
+0001e930: 290a 0a20 2020 2020 2020 2023 2049 6620  )..        # If 
+0001e940: 7365 6372 6574 2064 6f65 736e 2774 2068  secret doesn't h
+0001e950: 6176 6520 616e 2049 442c 2077 6527 6c6c  ave an ID, we'll
+0001e960: 2072 756e 2073 6563 7265 742d 696e 666f   run secret-info
+0001e970: 2d67 6574 2074 6f20 6665 7463 6820 6974  -get to fetch it
+0001e980: 0a20 2020 2020 2020 2073 6563 7265 7420  .        secret 
+0001e990: 3d20 7365 6c66 2e6d 616b 655f 7365 6372  = self.make_secr
+0001e9a0: 6574 286c 6162 656c 3d27 7927 290a 2020  et(label='y').  
+0001e9b0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0001e9c0: 7449 734e 6f6e 6528 7365 6372 6574 2e69  tIsNone(secret.i
+0001e9d0: 6429 0a20 2020 2020 2020 2073 6563 7265  d).        secre
+0001e9e0: 742e 7265 6d6f 7665 5f72 6576 6973 696f  t.remove_revisio
+0001e9f0: 6e28 3233 3429 0a20 2020 2020 2020 2073  n(234).        s
+0001ea00: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001ea10: 7365 6372 6574 2e69 642c 2027 7365 6372  secret.id, 'secr
+0001ea20: 6574 3a7a 2729 0a0a 2020 2020 2020 2020  et:z')..        
+0001ea30: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0001ea40: 2866 616b 655f 7363 7269 7074 5f63 616c  (fake_script_cal
+0001ea50: 6c73 2873 656c 662c 2063 6c65 6172 3d54  ls(self, clear=T
+0001ea60: 7275 6529 2c20 5b0a 2020 2020 2020 2020  rue), [.        
+0001ea70: 2020 2020 5b27 7365 6372 6574 2d72 656d      ['secret-rem
+0001ea80: 6f76 6527 2c20 2773 6563 7265 743a 7827  ove', 'secret:x'
+0001ea90: 2c20 272d 2d72 6576 6973 696f 6e27 2c20  , '--revision', 
+0001eaa0: 2731 3233 275d 2c0a 2020 2020 2020 2020  '123'],.        
+0001eab0: 2020 2020 5b27 7365 6372 6574 2d69 6e66      ['secret-inf
+0001eac0: 6f2d 6765 7427 2c20 272d 2d6c 6162 656c  o-get', '--label
+0001ead0: 272c 2027 7927 2c20 272d 2d66 6f72 6d61  ', 'y', '--forma
+0001eae0: 743d 6a73 6f6e 275d 2c0a 2020 2020 2020  t=json'],.      
+0001eaf0: 2020 2020 2020 5b27 7365 6372 6574 2d72        ['secret-r
+0001eb00: 656d 6f76 6527 2c20 2773 6563 7265 743a  emove', 'secret:
+0001eb10: 7a27 2c20 272d 2d72 6576 6973 696f 6e27  z', '--revision'
+0001eb20: 2c20 2732 3334 275d 2c0a 2020 2020 2020  , '234'],.      
+0001eb30: 2020 5d29 0a0a 2020 2020 6465 6620 7465    ])..    def te
+0001eb40: 7374 5f72 656d 6f76 655f 616c 6c5f 7265  st_remove_all_re
+0001eb50: 7669 7369 6f6e 7328 7365 6c66 293a 0a20  visions(self):. 
+0001eb60: 2020 2020 2020 2066 616b 655f 7363 7269         fake_scri
+0001eb70: 7074 2873 656c 662c 2027 7365 6372 6574  pt(self, 'secret
+0001eb80: 2d72 656d 6f76 6527 2c20 2222 2265 7869  -remove', """exi
+0001eb90: 7420 3022 2222 290a 2020 2020 2020 2020  t 0""").        
+0001eba0: 6661 6b65 5f73 6372 6970 7428 7365 6c66  fake_script(self
+0001ebb0: 2c20 2773 6563 7265 742d 696e 666f 2d67  , 'secret-info-g
+0001ebc0: 6574 272c 2022 2222 6563 686f 2027 7b22  et', """echo '{"
+0001ebd0: 7a22 3a20 7b22 6c61 6265 6c22 3a20 2279  z": {"label": "y
+0001ebe0: 222c 2022 7265 7669 7369 6f6e 223a 2037  ", "revision": 7
+0001ebf0: 7d7d 2722 2222 290a 0a20 2020 2020 2020  }}'""")..       
+0001ec00: 2073 6563 7265 7420 3d20 7365 6c66 2e6d   secret = self.m
+0001ec10: 616b 655f 7365 6372 6574 2869 643d 2778  ake_secret(id='x
+0001ec20: 2729 0a20 2020 2020 2020 2073 6563 7265  ').        secre
+0001ec30: 742e 7265 6d6f 7665 5f61 6c6c 5f72 6576  t.remove_all_rev
+0001ec40: 6973 696f 6e73 2829 0a0a 2020 2020 2020  isions()..      
+0001ec50: 2020 2320 4966 2073 6563 7265 7420 646f    # If secret do
+0001ec60: 6573 6e27 7420 6861 7665 2061 6e20 4944  esn't have an ID
+0001ec70: 2c20 7765 276c 6c20 7275 6e20 7365 6372  , we'll run secr
+0001ec80: 6574 2d69 6e66 6f2d 6765 7420 746f 2066  et-info-get to f
+0001ec90: 6574 6368 2069 740a 2020 2020 2020 2020  etch it.        
+0001eca0: 7365 6372 6574 203d 2073 656c 662e 6d61  secret = self.ma
+0001ecb0: 6b65 5f73 6563 7265 7428 6c61 6265 6c3d  ke_secret(label=
+0001ecc0: 2779 2729 0a20 2020 2020 2020 2073 656c  'y').        sel
+0001ecd0: 662e 6173 7365 7274 4973 4e6f 6e65 2873  f.assertIsNone(s
+0001ece0: 6563 7265 742e 6964 290a 2020 2020 2020  ecret.id).      
+0001ecf0: 2020 7365 6372 6574 2e72 656d 6f76 655f    secret.remove_
+0001ed00: 616c 6c5f 7265 7669 7369 6f6e 7328 290a  all_revisions().
+0001ed10: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0001ed20: 6572 7445 7175 616c 2873 6563 7265 742e  ertEqual(secret.
+0001ed30: 6964 2c20 2773 6563 7265 743a 7a27 290a  id, 'secret:z').
+0001ed40: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001ed50: 7365 7274 4571 7561 6c28 6661 6b65 5f73  sertEqual(fake_s
+0001ed60: 6372 6970 745f 6361 6c6c 7328 7365 6c66  cript_calls(self
+0001ed70: 2c20 636c 6561 723d 5472 7565 292c 205b  , clear=True), [
+0001ed80: 0a20 2020 2020 2020 2020 2020 205b 2773  .            ['s
+0001ed90: 6563 7265 742d 7265 6d6f 7665 272c 2027  ecret-remove', '
+0001eda0: 7365 6372 6574 3a78 275d 2c0a 2020 2020  secret:x'],.    
+0001edb0: 2020 2020 2020 2020 5b27 7365 6372 6574          ['secret
+0001edc0: 2d69 6e66 6f2d 6765 7427 2c20 272d 2d6c  -info-get', '--l
+0001edd0: 6162 656c 272c 2027 7927 2c20 272d 2d66  abel', 'y', '--f
+0001ede0: 6f72 6d61 743d 6a73 6f6e 275d 2c0a 2020  ormat=json'],.  
+0001edf0: 2020 2020 2020 2020 2020 5b27 7365 6372            ['secr
+0001ee00: 6574 2d72 656d 6f76 6527 2c20 2773 6563  et-remove', 'sec
+0001ee10: 7265 743a 7a27 5d2c 0a20 2020 2020 2020  ret:z'],.       
+0001ee20: 205d 290a 0a0a 636c 6173 7320 5465 7374   ])...class Test
+0001ee30: 506f 7274 7328 756e 6974 7465 7374 2e54  Ports(unittest.T
+0001ee40: 6573 7443 6173 6529 3a0a 2020 2020 6465  estCase):.    de
+0001ee50: 6620 7365 7455 7028 7365 6c66 293a 0a20  f setUp(self):. 
+0001ee60: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
+0001ee70: 6c20 3d20 6f70 732e 6d6f 6465 6c2e 4d6f  l = ops.model.Mo
+0001ee80: 6465 6c28 6f70 732e 6368 6172 6d2e 4368  del(ops.charm.Ch
+0001ee90: 6172 6d4d 6574 6128 292c 206f 7073 2e6d  armMeta(), ops.m
+0001eea0: 6f64 656c 2e5f 4d6f 6465 6c42 6163 6b65  odel._ModelBacke
+0001eeb0: 6e64 2827 6d79 6170 702f 3027 2929 0a20  nd('myapp/0')). 
+0001eec0: 2020 2020 2020 2073 656c 662e 756e 6974         self.unit
+0001eed0: 203d 2073 656c 662e 6d6f 6465 6c2e 756e   = self.model.un
+0001eee0: 6974 0a0a 2020 2020 6465 6620 7465 7374  it..    def test
+0001eef0: 5f6f 7065 6e5f 706f 7274 2873 656c 6629  _open_port(self)
+0001ef00: 3a0a 2020 2020 2020 2020 6661 6b65 5f73  :.        fake_s
+0001ef10: 6372 6970 7428 7365 6c66 2c20 276f 7065  cript(self, 'ope
+0001ef20: 6e2d 706f 7274 272c 2027 6578 6974 2030  n-port', 'exit 0
+0001ef30: 2729 0a0a 2020 2020 2020 2020 7365 6c66  ')..        self
+0001ef40: 2e75 6e69 742e 6f70 656e 5f70 6f72 7428  .unit.open_port(
+0001ef50: 2774 6370 272c 2038 3038 3029 0a20 2020  'tcp', 8080).   
+0001ef60: 2020 2020 2073 656c 662e 756e 6974 2e6f       self.unit.o
+0001ef70: 7065 6e5f 706f 7274 2827 5544 5027 2c20  pen_port('UDP', 
+0001ef80: 3430 3030 290a 2020 2020 2020 2020 7365  4000).        se
+0001ef90: 6c66 2e75 6e69 742e 6f70 656e 5f70 6f72  lf.unit.open_por
+0001efa0: 7428 2769 636d 7027 290a 0a20 2020 2020  t('icmp')..     
+0001efb0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0001efc0: 7561 6c28 6661 6b65 5f73 6372 6970 745f  ual(fake_script_
+0001efd0: 6361 6c6c 7328 7365 6c66 2c20 636c 6561  calls(self, clea
+0001efe0: 723d 5472 7565 292c 205b 0a20 2020 2020  r=True), [.     
+0001eff0: 2020 2020 2020 205b 276f 7065 6e2d 706f         ['open-po
+0001f000: 7274 272c 2027 3830 3830 2f74 6370 275d  rt', '8080/tcp']
+0001f010: 2c0a 2020 2020 2020 2020 2020 2020 5b27  ,.            ['
+0001f020: 6f70 656e 2d70 6f72 7427 2c20 2734 3030  open-port', '400
+0001f030: 302f 7564 7027 5d2c 0a20 2020 2020 2020  0/udp'],.       
+0001f040: 2020 2020 205b 276f 7065 6e2d 706f 7274       ['open-port
+0001f050: 272c 2027 6963 6d70 275d 2c0a 2020 2020  ', 'icmp'],.    
+0001f060: 2020 2020 5d29 0a0a 2020 2020 6465 6620      ])..    def 
+0001f070: 7465 7374 5f6f 7065 6e5f 706f 7274 5f65  test_open_port_e
+0001f080: 7272 6f72 2873 656c 6629 3a0a 2020 2020  rror(self):.    
+0001f090: 2020 2020 6661 6b65 5f73 6372 6970 7428      fake_script(
+0001f0a0: 7365 6c66 2c20 276f 7065 6e2d 706f 7274  self, 'open-port
+0001f0b0: 272c 2022 6563 686f 2027 4552 524f 5220  ', "echo 'ERROR 
+0001f0c0: 6261 6420 7072 6f74 6f63 6f6c 2720 3e26  bad protocol' >&
+0001f0d0: 323b 2065 7869 7420 3122 290a 0a20 2020  2; exit 1")..   
+0001f0e0: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
+0001f0f0: 7373 6572 7452 6169 7365 7328 6f70 732e  ssertRaises(ops.
+0001f100: 4d6f 6465 6c45 7272 6f72 2920 6173 2063  ModelError) as c
+0001f110: 6d3a 0a20 2020 2020 2020 2020 2020 2073  m:.            s
+0001f120: 656c 662e 756e 6974 2e6f 7065 6e5f 706f  elf.unit.open_po
+0001f130: 7274 2827 6674 7027 2c20 3830 3830 290a  rt('ftp', 8080).
+0001f140: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0001f150: 6572 7445 7175 616c 2873 7472 2863 6d2e  ertEqual(str(cm.
+0001f160: 6578 6365 7074 696f 6e29 2c20 2745 5252  exception), 'ERR
+0001f170: 4f52 2062 6164 2070 726f 746f 636f 6c5c  OR bad protocol\
+0001f180: 6e27 290a 0a20 2020 2020 2020 2073 656c  n')..        sel
+0001f190: 662e 6173 7365 7274 4571 7561 6c28 6661  f.assertEqual(fa
+0001f1a0: 6b65 5f73 6372 6970 745f 6361 6c6c 7328  ke_script_calls(
+0001f1b0: 7365 6c66 2c20 636c 6561 723d 5472 7565  self, clear=True
+0001f1c0: 292c 205b 0a20 2020 2020 2020 2020 2020  ), [.           
+0001f1d0: 205b 276f 7065 6e2d 706f 7274 272c 2027   ['open-port', '
+0001f1e0: 3830 3830 2f66 7470 275d 2c0a 2020 2020  8080/ftp'],.    
+0001f1f0: 2020 2020 5d29 0a0a 2020 2020 6465 6620      ])..    def 
+0001f200: 7465 7374 5f63 6c6f 7365 5f70 6f72 7428  test_close_port(
+0001f210: 7365 6c66 293a 0a20 2020 2020 2020 2066  self):.        f
+0001f220: 616b 655f 7363 7269 7074 2873 656c 662c  ake_script(self,
+0001f230: 2027 636c 6f73 652d 706f 7274 272c 2027   'close-port', '
+0001f240: 6578 6974 2030 2729 0a0a 2020 2020 2020  exit 0')..      
+0001f250: 2020 7365 6c66 2e75 6e69 742e 636c 6f73    self.unit.clos
+0001f260: 655f 706f 7274 2827 7463 7027 2c20 3830  e_port('tcp', 80
+0001f270: 3830 290a 2020 2020 2020 2020 7365 6c66  80).        self
+0001f280: 2e75 6e69 742e 636c 6f73 655f 706f 7274  .unit.close_port
+0001f290: 2827 5544 5027 2c20 3430 3030 290a 2020  ('UDP', 4000).  
+0001f2a0: 2020 2020 2020 7365 6c66 2e75 6e69 742e        self.unit.
+0001f2b0: 636c 6f73 655f 706f 7274 2827 6963 6d70  close_port('icmp
+0001f2c0: 2729 0a0a 2020 2020 2020 2020 7365 6c66  ')..        self
+0001f2d0: 2e61 7373 6572 7445 7175 616c 2866 616b  .assertEqual(fak
+0001f2e0: 655f 7363 7269 7074 5f63 616c 6c73 2873  e_script_calls(s
+0001f2f0: 656c 662c 2063 6c65 6172 3d54 7275 6529  elf, clear=True)
+0001f300: 2c20 5b0a 2020 2020 2020 2020 2020 2020  , [.            
+0001f310: 5b27 636c 6f73 652d 706f 7274 272c 2027  ['close-port', '
+0001f320: 3830 3830 2f74 6370 275d 2c0a 2020 2020  8080/tcp'],.    
+0001f330: 2020 2020 2020 2020 5b27 636c 6f73 652d          ['close-
+0001f340: 706f 7274 272c 2027 3430 3030 2f75 6470  port', '4000/udp
+0001f350: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
+0001f360: 5b27 636c 6f73 652d 706f 7274 272c 2027  ['close-port', '
+0001f370: 6963 6d70 275d 2c0a 2020 2020 2020 2020  icmp'],.        
+0001f380: 5d29 0a0a 2020 2020 6465 6620 7465 7374  ])..    def test
+0001f390: 5f63 6c6f 7365 5f70 6f72 745f 6572 726f  _close_port_erro
+0001f3a0: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
+0001f3b0: 2066 616b 655f 7363 7269 7074 2873 656c   fake_script(sel
+0001f3c0: 662c 2027 636c 6f73 652d 706f 7274 272c  f, 'close-port',
+0001f3d0: 2022 6563 686f 2027 4552 524f 5220 6261   "echo 'ERROR ba
+0001f3e0: 6420 7072 6f74 6f63 6f6c 2720 3e26 323b  d protocol' >&2;
+0001f3f0: 2065 7869 7420 3122 290a 0a20 2020 2020   exit 1")..     
+0001f400: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
+0001f410: 6572 7452 6169 7365 7328 6f70 732e 4d6f  ertRaises(ops.Mo
+0001f420: 6465 6c45 7272 6f72 2920 6173 2063 6d3a  delError) as cm:
+0001f430: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001f440: 662e 756e 6974 2e63 6c6f 7365 5f70 6f72  f.unit.close_por
+0001f450: 7428 2766 7470 272c 2038 3038 3029 0a20  t('ftp', 8080). 
+0001f460: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001f470: 7274 4571 7561 6c28 7374 7228 636d 2e65  rtEqual(str(cm.e
+0001f480: 7863 6570 7469 6f6e 292c 2027 4552 524f  xception), 'ERRO
+0001f490: 5220 6261 6420 7072 6f74 6f63 6f6c 5c6e  R bad protocol\n
+0001f4a0: 2729 0a0a 2020 2020 2020 2020 7365 6c66  ')..        self
+0001f4b0: 2e61 7373 6572 7445 7175 616c 2866 616b  .assertEqual(fak
+0001f4c0: 655f 7363 7269 7074 5f63 616c 6c73 2873  e_script_calls(s
+0001f4d0: 656c 662c 2063 6c65 6172 3d54 7275 6529  elf, clear=True)
+0001f4e0: 2c20 5b0a 2020 2020 2020 2020 2020 2020  , [.            
+0001f4f0: 5b27 636c 6f73 652d 706f 7274 272c 2027  ['close-port', '
+0001f500: 3830 3830 2f66 7470 275d 2c0a 2020 2020  8080/ftp'],.    
+0001f510: 2020 2020 5d29 0a0a 2020 2020 6465 6620      ])..    def 
+0001f520: 7465 7374 5f6f 7065 6e65 645f 706f 7274  test_opened_port
+0001f530: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+0001f540: 2066 616b 655f 7363 7269 7074 2873 656c   fake_script(sel
+0001f550: 662c 2027 6f70 656e 6564 2d70 6f72 7473  f, 'opened-ports
+0001f560: 272c 2022 2222 6563 686f 2038 3038 302f  ', """echo 8080/
+0001f570: 7463 703b 2065 6368 6f20 6963 6d70 2222  tcp; echo icmp""
+0001f580: 2229 0a0a 2020 2020 2020 2020 706f 7274  ")..        port
+0001f590: 735f 7365 7420 3d20 7365 6c66 2e75 6e69  s_set = self.uni
+0001f5a0: 742e 6f70 656e 6564 5f70 6f72 7473 2829  t.opened_ports()
+0001f5b0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0001f5c0: 7365 7274 4973 496e 7374 616e 6365 2870  sertIsInstance(p
+0001f5d0: 6f72 7473 5f73 6574 2c20 7365 7429 0a20  orts_set, set). 
+0001f5e0: 2020 2020 2020 2070 6f72 7473 203d 2073         ports = s
+0001f5f0: 6f72 7465 6428 706f 7274 735f 7365 742c  orted(ports_set,
+0001f600: 206b 6579 3d6c 616d 6264 6120 703a 2028   key=lambda p: (
+0001f610: 702e 7072 6f74 6f63 6f6c 2c20 702e 706f  p.protocol, p.po
+0001f620: 7274 2929 0a20 2020 2020 2020 2073 656c  rt)).        sel
+0001f630: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
+0001f640: 6e28 706f 7274 7329 2c20 3229 0a20 2020  n(ports), 2).   
+0001f650: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001f660: 4973 496e 7374 616e 6365 2870 6f72 7473  IsInstance(ports
+0001f670: 5b30 5d2c 206f 7073 2e4f 7065 6e65 6450  [0], ops.OpenedP
+0001f680: 6f72 7429 0a20 2020 2020 2020 2073 656c  ort).        sel
+0001f690: 662e 6173 7365 7274 4571 7561 6c28 706f  f.assertEqual(po
+0001f6a0: 7274 735b 305d 2e70 726f 746f 636f 6c2c  rts[0].protocol,
+0001f6b0: 2027 6963 6d70 2729 0a20 2020 2020 2020   'icmp').       
+0001f6c0: 2073 656c 662e 6173 7365 7274 4973 4e6f   self.assertIsNo
+0001f6d0: 6e65 2870 6f72 7473 5b30 5d2e 706f 7274  ne(ports[0].port
+0001f6e0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0001f6f0: 7373 6572 7449 7349 6e73 7461 6e63 6528  ssertIsInstance(
+0001f700: 706f 7274 735b 315d 2c20 6f70 732e 4f70  ports[1], ops.Op
+0001f710: 656e 6564 506f 7274 290a 2020 2020 2020  enedPort).      
+0001f720: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0001f730: 616c 2870 6f72 7473 5b31 5d2e 7072 6f74  al(ports[1].prot
+0001f740: 6f63 6f6c 2c20 2774 6370 2729 0a20 2020  ocol, 'tcp').   
+0001f750: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001f760: 4571 7561 6c28 706f 7274 735b 315d 2e70  Equal(ports[1].p
+0001f770: 6f72 742c 2038 3038 3029 0a0a 2020 2020  ort, 8080)..    
+0001f780: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0001f790: 7175 616c 2866 616b 655f 7363 7269 7074  qual(fake_script
+0001f7a0: 5f63 616c 6c73 2873 656c 662c 2063 6c65  _calls(self, cle
+0001f7b0: 6172 3d54 7275 6529 2c20 5b0a 2020 2020  ar=True), [.    
+0001f7c0: 2020 2020 2020 2020 5b27 6f70 656e 6564          ['opened
+0001f7d0: 2d70 6f72 7473 272c 2027 275d 2c0a 2020  -ports', ''],.  
+0001f7e0: 2020 2020 2020 5d29 0a0a 2020 2020 6465        ])..    de
+0001f7f0: 6620 7465 7374 5f6f 7065 6e65 645f 706f  f test_opened_po
+0001f800: 7274 735f 7761 726e 696e 6773 2873 656c  rts_warnings(sel
+0001f810: 6629 3a0a 2020 2020 2020 2020 6661 6b65  f):.        fake
+0001f820: 5f73 6372 6970 7428 7365 6c66 2c20 276f  _script(self, 'o
+0001f830: 7065 6e65 642d 706f 7274 7327 2c20 2222  pened-ports', ""
+0001f840: 2265 6368 6f20 3830 3830 2f74 6370 3b20  "echo 8080/tcp; 
+0001f850: 6563 686f 2031 3233 342f 6674 703b 2065  echo 1234/ftp; e
+0001f860: 6368 6f20 3130 3030 2d32 3030 302f 7564  cho 1000-2000/ud
+0001f870: 7022 2222 290a 0a20 2020 2020 2020 2077  p""")..        w
+0001f880: 6974 6820 7365 6c66 2e61 7373 6572 744c  ith self.assertL
+0001f890: 6f67 7328 276f 7073 2e6d 6f64 656c 272c  ogs('ops.model',
+0001f8a0: 206c 6576 656c 3d27 5741 524e 494e 4727   level='WARNING'
+0001f8b0: 2920 6173 2063 6d3a 0a20 2020 2020 2020  ) as cm:.       
+0001f8c0: 2020 2020 2070 6f72 7473 5f73 6574 203d       ports_set =
+0001f8d0: 2073 656c 662e 756e 6974 2e6f 7065 6e65   self.unit.opene
+0001f8e0: 645f 706f 7274 7328 290a 2020 2020 2020  d_ports().      
+0001f8f0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0001f900: 616c 286c 656e 2863 6d2e 6f75 7470 7574  al(len(cm.output
+0001f910: 292c 2032 290a 2020 2020 2020 2020 7365  ), 2).        se
+0001f920: 6c66 2e61 7373 6572 7452 6567 6578 2863  lf.assertRegex(c
+0001f930: 6d2e 6f75 7470 7574 5b30 5d2c 2072 2757  m.output[0], r'W
+0001f940: 4152 4e49 4e47 3a6f 7073 2e6d 6f64 656c  ARNING:ops.model
+0001f950: 3a2e 2a70 726f 746f 636f 6c2e 2a27 290a  :.*protocol.*').
+0001f960: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0001f970: 6572 7452 6567 6578 2863 6d2e 6f75 7470  ertRegex(cm.outp
+0001f980: 7574 5b31 5d2c 2072 2757 4152 4e49 4e47  ut[1], r'WARNING
+0001f990: 3a6f 7073 2e6d 6f64 656c 3a2e 2a72 616e  :ops.model:.*ran
+0001f9a0: 6765 2e2a 2729 0a0a 2020 2020 2020 2020  ge.*')..        
+0001f9b0: 7365 6c66 2e61 7373 6572 7449 7349 6e73  self.assertIsIns
+0001f9c0: 7461 6e63 6528 706f 7274 735f 7365 742c  tance(ports_set,
+0001f9d0: 2073 6574 290a 2020 2020 2020 2020 706f   set).        po
+0001f9e0: 7274 7320 3d20 736f 7274 6564 2870 6f72  rts = sorted(por
+0001f9f0: 7473 5f73 6574 2c20 6b65 793d 6c61 6d62  ts_set, key=lamb
+0001fa00: 6461 2070 3a20 2870 2e70 726f 746f 636f  da p: (p.protoco
+0001fa10: 6c2c 2070 2e70 6f72 7429 290a 2020 2020  l, p.port)).    
+0001fa20: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0001fa30: 7175 616c 286c 656e 2870 6f72 7473 292c  qual(len(ports),
+0001fa40: 2032 290a 2020 2020 2020 2020 7365 6c66   2).        self
+0001fa50: 2e61 7373 6572 7449 7349 6e73 7461 6e63  .assertIsInstanc
+0001fa60: 6528 706f 7274 735b 305d 2c20 6f70 732e  e(ports[0], ops.
+0001fa70: 4f70 656e 6564 506f 7274 290a 2020 2020  OpenedPort).    
+0001fa80: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0001fa90: 7175 616c 2870 6f72 7473 5b30 5d2e 7072  qual(ports[0].pr
+0001faa0: 6f74 6f63 6f6c 2c20 2774 6370 2729 0a20  otocol, 'tcp'). 
+0001fab0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0001fac0: 7274 4571 7561 6c28 706f 7274 735b 305d  rtEqual(ports[0]
+0001fad0: 2e70 6f72 742c 2038 3038 3029 0a20 2020  .port, 8080).   
+0001fae0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0001faf0: 4973 496e 7374 616e 6365 2870 6f72 7473  IsInstance(ports
+0001fb00: 5b31 5d2c 206f 7073 2e4f 7065 6e65 6450  [1], ops.OpenedP
+0001fb10: 6f72 7429 0a20 2020 2020 2020 2073 656c  ort).        sel
+0001fb20: 662e 6173 7365 7274 4571 7561 6c28 706f  f.assertEqual(po
+0001fb30: 7274 735b 315d 2e70 726f 746f 636f 6c2c  rts[1].protocol,
+0001fb40: 2027 7564 7027 290a 2020 2020 2020 2020   'udp').        
+0001fb50: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0001fb60: 2870 6f72 7473 5b31 5d2e 706f 7274 2c20  (ports[1].port, 
+0001fb70: 3130 3030 290a 0a20 2020 2020 2020 2073  1000)..        s
+0001fb80: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0001fb90: 6661 6b65 5f73 6372 6970 745f 6361 6c6c  fake_script_call
+0001fba0: 7328 7365 6c66 2c20 636c 6561 723d 5472  s(self, clear=Tr
+0001fbb0: 7565 292c 205b 0a20 2020 2020 2020 2020  ue), [.         
+0001fbc0: 2020 205b 276f 7065 6e65 642d 706f 7274     ['opened-port
+0001fbd0: 7327 2c20 2727 5d2c 0a20 2020 2020 2020  s', ''],.       
+0001fbe0: 205d 290a 0a0a 6966 205f 5f6e 616d 655f   ])...if __name_
+0001fbf0: 5f20 3d3d 2022 5f5f 6d61 696e 5f5f 223a  _ == "__main__":
+0001fc00: 0a20 2020 2075 6e69 7474 6573 742e 6d61  .    unittest.ma
+0001fc10: 696e 2829 0a                             in().
```

### Comparing `ops-2.2.0/test/test_pebble.py` & `ops-2.3.0/test/test_pebble.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/test/test_private.py` & `ops-2.3.0/test/test_private.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/test/test_storage.py` & `ops-2.3.0/test/test_storage.py`

 * *Files identical despite different names*

### Comparing `ops-2.2.0/test/test_testing.py` & `ops-2.3.0/test/test_testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -9484,2477 +9484,2478 @@
 000250b0: 2069 7320 6e6f 7720 7374 6172 7465 642c   is now started,
 000250c0: 2062 7574 2042 6172 2069 7320 6e6f 740a   but Bar is not.
 000250d0: 0a20 2020 2020 2020 2023 2053 656e 6420  .        # Send 
 000250e0: 6120 7661 6c69 6420 7369 676e 616c 2074  a valid signal t
 000250f0: 6f20 6120 7275 6e6e 696e 6720 7365 7276  o a running serv
 00025100: 6963 650a 2020 2020 2020 2020 636c 6965  ice.        clie
 00025110: 6e74 2e73 656e 645f 7369 676e 616c 2822  nt.send_signal("
-00025120: 5349 4749 4e54 222c 2022 666f 6f22 290a  SIGINT", "foo").
-00025130: 0a20 2020 2020 2020 2023 2053 656e 6420  .        # Send 
-00025140: 6120 7661 6c69 6420 7369 676e 616c 2062  a valid signal b
-00025150: 7574 206f 6d69 7420 7365 7276 6963 6520  ut omit service 
-00025160: 6e61 6d65 0a20 2020 2020 2020 2077 6974  name.        wit
-00025170: 6820 7365 6c66 2e61 7373 6572 7452 6169  h self.assertRai
-00025180: 7365 7328 5479 7065 4572 726f 7229 3a0a  ses(TypeError):.
-00025190: 2020 2020 2020 2020 2020 2020 636c 6965              clie
-000251a0: 6e74 2e73 656e 645f 7369 676e 616c 2822  nt.send_signal("
-000251b0: 5349 4749 4e54 2229 0a0a 2020 2020 2020  SIGINT")..      
-000251c0: 2020 2320 5365 6e64 2061 6e20 696e 7661    # Send an inva
-000251d0: 6c69 6420 7369 676e 616c 2074 6f20 6120  lid signal to a 
-000251e0: 7275 6e6e 696e 6720 7365 7276 6963 650a  running service.
-000251f0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00025200: 662e 6173 7365 7274 5261 6973 6573 2870  f.assertRaises(p
-00025210: 6562 626c 652e 4150 4945 7272 6f72 293a  ebble.APIError):
-00025220: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-00025230: 656e 742e 7365 6e64 5f73 6967 6e61 6c28  ent.send_signal(
-00025240: 2273 6967 696e 7422 2c20 2266 6f6f 2229  "sigint", "foo")
-00025250: 0a0a 2020 2020 2020 2020 2320 5365 6e64  ..        # Send
-00025260: 2061 2076 616c 6964 2073 6967 6e61 6c20   a valid signal 
-00025270: 746f 2061 2073 746f 7070 6564 2073 6572  to a stopped ser
-00025280: 7669 6365 0a20 2020 2020 2020 2077 6974  vice.        wit
-00025290: 6820 7365 6c66 2e61 7373 6572 7452 6169  h self.assertRai
-000252a0: 7365 7328 7065 6262 6c65 2e41 5049 4572  ses(pebble.APIEr
-000252b0: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
-000252c0: 2020 636c 6965 6e74 2e73 656e 645f 7369    client.send_si
-000252d0: 676e 616c 2822 5349 4749 4e54 222c 2022  gnal("SIGINT", "
-000252e0: 6261 7222 290a 0a20 2020 2020 2020 2023  bar")..        #
-000252f0: 2053 656e 6420 6120 7661 6c69 6420 7369   Send a valid si
-00025300: 676e 616c 2074 6f20 6120 6e6f 6e2d 6578  gnal to a non-ex
-00025310: 6973 7469 6e67 2073 6572 7669 6365 0a20  isting service. 
-00025320: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00025330: 2e61 7373 6572 7452 6169 7365 7328 7065  .assertRaises(pe
-00025340: 6262 6c65 2e41 5049 4572 726f 7229 3a0a  bble.APIError):.
-00025350: 2020 2020 2020 2020 2020 2020 636c 6965              clie
-00025360: 6e74 2e73 656e 645f 7369 676e 616c 2822  nt.send_signal("
-00025370: 5349 4749 4e54 222c 2022 6261 7a22 290a  SIGINT", "baz").
-00025380: 0a20 2020 2020 2020 2023 2053 656e 6420  .        # Send 
-00025390: 6120 7661 6c69 6420 7369 676e 616c 2074  a valid signal t
-000253a0: 6f20 6120 6d75 6c74 6970 6c65 2073 6572  o a multiple ser
-000253b0: 7669 6365 732c 206f 6e65 206f 6620 7768  vices, one of wh
-000253c0: 6963 6820 6973 206e 6f74 2072 756e 6e69  ich is not runni
-000253d0: 6e67 0a20 2020 2020 2020 2077 6974 6820  ng.        with 
-000253e0: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
-000253f0: 7328 7065 6262 6c65 2e41 5049 4572 726f  s(pebble.APIErro
-00025400: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00025410: 636c 6965 6e74 2e73 656e 645f 7369 676e  client.send_sign
-00025420: 616c 2822 5349 4749 4e54 222c 2022 666f  al("SIGINT", "fo
-00025430: 6f22 2c20 2262 6172 2229 0a0a 0a23 2046  o", "bar")...# F
-00025440: 6f72 2074 6573 7469 6e67 2066 696c 652d  or testing file-
-00025450: 6f70 7320 6f66 2074 6865 2070 6562 626c  ops of the pebbl
-00025460: 6520 636c 6965 6e74 2e20 2054 6869 7320  e client.  This 
-00025470: 6973 2072 6566 6163 746f 7265 6420 696e  is refactored in
-00025480: 746f 2061 0a23 2073 6570 6172 6174 6520  to a.# separate 
-00025490: 6d69 7869 6e20 736f 2077 6520 6361 6e20  mixin so we can 
-000254a0: 7275 6e20 7468 6573 6520 7465 7374 7320  run these tests 
-000254b0: 6167 6169 6e73 7420 626f 7468 2074 6865  against both the
-000254c0: 206d 6f63 6b20 636c 6965 6e74 2061 730a   mock client as.
-000254d0: 2320 7765 6c6c 2061 7320 6120 7265 616c  # well as a real
-000254e0: 2070 6562 626c 6520 7365 7276 6572 2069   pebble server i
-000254f0: 6e73 7461 6e63 652e 0a63 6c61 7373 205f  nstance..class _
-00025500: 5065 6262 6c65 5374 6f72 6167 6541 5049  PebbleStorageAPI
-00025510: 7354 6573 744d 6978 696e 3a0a 2020 2020  sTestMixin:.    
-00025520: 2320 4f76 6572 7269 6465 2074 6869 7320  # Override this 
-00025530: 696e 2063 6c61 7373 6573 2075 7369 6e67  in classes using
-00025540: 2074 6869 7320 6d69 7869 6e2e 0a20 2020   this mixin..   
-00025550: 2023 2054 6869 7320 7368 6f75 6c64 2062   # This should b
-00025560: 6520 7365 7420 746f 2061 6e79 206e 6f6e  e set to any non
-00025570: 2d65 6d70 7479 2070 6174 682c 2062 7574  -empty path, but
-00025580: 2077 6974 686f 7574 2061 2074 7261 696c   without a trail
-00025590: 696e 6720 2f2e 0a20 2020 2070 7265 6669  ing /..    prefi
-000255a0: 7820 3d20 4e6f 6e65 0a0a 2020 2020 6465  x = None..    de
-000255b0: 6620 7465 7374 5f70 7573 685f 616e 645f  f test_push_and_
-000255c0: 7075 6c6c 5f62 7974 6573 2873 656c 6629  pull_bytes(self)
-000255d0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-000255e0: 7465 7374 5f70 7573 685f 616e 645f 7075  test_push_and_pu
-000255f0: 6c6c 5f64 6174 6128 0a20 2020 2020 2020  ll_data(.       
-00025600: 2020 2020 206f 7269 6769 6e61 6c5f 6461       original_da
-00025610: 7461 3d62 225c 7830 305c 7830 315c 7830  ta=b"\x00\x01\x0
-00025620: 325c 7830 335c 7830 3422 2c0a 2020 2020  2\x03\x04",.    
-00025630: 2020 2020 2020 2020 656e 636f 6469 6e67          encoding
-00025640: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-00025650: 2020 2073 7472 6561 6d5f 636c 6173 733d     stream_class=
-00025660: 696f 2e42 7974 6573 494f 290a 0a20 2020  io.BytesIO)..   
-00025670: 2064 6566 2074 6573 745f 7075 7368 5f61   def test_push_a
-00025680: 6e64 5f70 756c 6c5f 6e6f 6e5f 7574 6638  nd_pull_non_utf8
-00025690: 5f64 6174 6128 7365 6c66 293a 0a20 2020  _data(self):.   
-000256a0: 2020 2020 2073 656c 662e 5f74 6573 745f       self._test_
-000256b0: 7075 7368 5f61 6e64 5f70 756c 6c5f 6461  push_and_pull_da
-000256c0: 7461 280a 2020 2020 2020 2020 2020 2020  ta(.            
-000256d0: 6f72 6967 696e 616c 5f64 6174 613d 27e6  original_data='.
-000256e0: 97a5 e69c ace8 aa9e 272c 2020 2320 224a  ........',  # "J
-000256f0: 6170 616e 6573 6522 2069 6e20 4a61 7061  apanese" in Japa
-00025700: 6e65 7365 0a20 2020 2020 2020 2020 2020  nese.           
-00025710: 2065 6e63 6f64 696e 673d 2773 6a69 7327   encoding='sjis'
-00025720: 2c0a 2020 2020 2020 2020 2020 2020 7374  ,.            st
-00025730: 7265 616d 5f63 6c61 7373 3d69 6f2e 5374  ream_class=io.St
-00025740: 7269 6e67 494f 290a 0a20 2020 2064 6566  ringIO)..    def
-00025750: 205f 7465 7374 5f70 7573 685f 616e 645f   _test_push_and_
-00025760: 7075 6c6c 5f64 6174 6128 7365 6c66 2c20  pull_data(self, 
-00025770: 6f72 6967 696e 616c 5f64 6174 612c 2065  original_data, e
-00025780: 6e63 6f64 696e 672c 2073 7472 6561 6d5f  ncoding, stream_
-00025790: 636c 6173 7329 3a0a 2020 2020 2020 2020  class):.        
-000257a0: 636c 6965 6e74 203d 2073 656c 662e 636c  client = self.cl
-000257b0: 6965 6e74 0a20 2020 2020 2020 2063 6c69  ient.        cli
-000257c0: 656e 742e 7075 7368 2866 227b 7365 6c66  ent.push(f"{self
-000257d0: 2e70 7265 6669 787d 2f74 6573 7422 2c20  .prefix}/test", 
-000257e0: 6f72 6967 696e 616c 5f64 6174 612c 2065  original_data, e
-000257f0: 6e63 6f64 696e 673d 656e 636f 6469 6e67  ncoding=encoding
-00025800: 290a 2020 2020 2020 2020 7769 7468 2063  ).        with c
-00025810: 6c69 656e 742e 7075 6c6c 2866 227b 7365  lient.pull(f"{se
-00025820: 6c66 2e70 7265 6669 787d 2f74 6573 7422  lf.prefix}/test"
-00025830: 2c20 656e 636f 6469 6e67 3d65 6e63 6f64  , encoding=encod
-00025840: 696e 6729 2061 7320 696e 6669 6c65 3a0a  ing) as infile:.
-00025850: 2020 2020 2020 2020 2020 2020 7265 6365              rece
-00025860: 6976 6564 5f64 6174 6120 3d20 696e 6669  ived_data = infi
-00025870: 6c65 2e72 6561 6428 290a 2020 2020 2020  le.read().      
-00025880: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00025890: 616c 286f 7269 6769 6e61 6c5f 6461 7461  al(original_data
-000258a0: 2c20 7265 6365 6976 6564 5f64 6174 6129  , received_data)
-000258b0: 0a0a 2020 2020 2020 2020 2320 5765 2061  ..        # We a
-000258c0: 6c73 6f20 7375 7070 6f72 7420 6669 6c65  lso support file
-000258d0: 2d6c 696b 6520 6f62 6a65 6374 7320 6173  -like objects as
-000258e0: 2069 6e70 7574 2c20 736f 206c 6574 2773   input, so let's
-000258f0: 2074 6573 7420 7468 6174 2063 6173 6520   test that case 
-00025900: 6173 2077 656c 6c2e 0a20 2020 2020 2020  as well..       
-00025910: 2073 6d61 6c6c 5f66 696c 6520 3d20 7374   small_file = st
-00025920: 7265 616d 5f63 6c61 7373 286f 7269 6769  ream_class(origi
-00025930: 6e61 6c5f 6461 7461 290a 2020 2020 2020  nal_data).      
-00025940: 2020 636c 6965 6e74 2e70 7573 6828 6622    client.push(f"
-00025950: 7b73 656c 662e 7072 6566 6978 7d2f 7465  {self.prefix}/te
-00025960: 7374 222c 2073 6d61 6c6c 5f66 696c 652c  st", small_file,
-00025970: 2065 6e63 6f64 696e 673d 656e 636f 6469   encoding=encodi
-00025980: 6e67 290a 2020 2020 2020 2020 7769 7468  ng).        with
-00025990: 2063 6c69 656e 742e 7075 6c6c 2866 227b   client.pull(f"{
-000259a0: 7365 6c66 2e70 7265 6669 787d 2f74 6573  self.prefix}/tes
-000259b0: 7422 2c20 656e 636f 6469 6e67 3d65 6e63  t", encoding=enc
-000259c0: 6f64 696e 6729 2061 7320 696e 6669 6c65  oding) as infile
-000259d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000259e0: 6365 6976 6564 5f64 6174 6120 3d20 696e  ceived_data = in
-000259f0: 6669 6c65 2e72 6561 6428 290a 2020 2020  file.read().    
-00025a00: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00025a10: 7175 616c 286f 7269 6769 6e61 6c5f 6461  qual(original_da
-00025a20: 7461 2c20 7265 6365 6976 6564 5f64 6174  ta, received_dat
-00025a30: 6129 0a0a 2020 2020 6465 6620 7465 7374  a)..    def test
-00025a40: 5f70 7573 685f 616e 645f 7075 6c6c 5f6c  _push_and_pull_l
-00025a50: 6172 6765 725f 6669 6c65 2873 656c 6629  arger_file(self)
-00025a60: 3a0a 2020 2020 2020 2020 2320 496e 7465  :.        # Inte
-00025a70: 6e74 3a20 746f 2065 6e73 7572 6520 7468  nt: to ensure th
-00025a80: 696e 6773 2077 6f72 6b20 6170 7072 6f70  ings work approp
-00025a90: 7269 6174 656c 7920 7769 7468 206c 6172  riately with lar
-00025aa0: 6765 7220 6669 6c65 732e 0a20 2020 2020  ger files..     
-00025ab0: 2020 2023 204c 6172 6765 7220 6669 6c65     # Larger file
-00025ac0: 7320 6d61 7920 6265 2073 656e 742f 7265  s may be sent/re
-00025ad0: 6365 6976 6564 2069 6e20 6d75 6c74 6970  ceived in multip
-00025ae0: 6c65 2063 6875 6e6b 733b 2074 6869 7320  le chunks; this 
-00025af0: 7368 6f75 6c64 2068 656c 7020 666f 720a  should help for.
-00025b00: 2020 2020 2020 2020 2320 6368 6563 6b69          # checki
-00025b10: 6e67 2074 6861 7420 7375 6368 206c 6f67  ng that such log
-00025b20: 6963 2069 7320 636f 7272 6563 742e 0a20  ic is correct.. 
-00025b30: 2020 2020 2020 2064 6174 615f 7369 7a65         data_size
-00025b40: 203d 2031 3032 3420 2a20 3130 3234 0a20   = 1024 * 1024. 
-00025b50: 2020 2020 2020 206f 7269 6769 6e61 6c5f         original_
-00025b60: 6461 7461 203d 206f 732e 7572 616e 646f  data = os.urando
-00025b70: 6d28 6461 7461 5f73 697a 6529 0a0a 2020  m(data_size)..  
-00025b80: 2020 2020 2020 636c 6965 6e74 203d 2073        client = s
-00025b90: 656c 662e 636c 6965 6e74 0a20 2020 2020  elf.client.     
-00025ba0: 2020 2063 6c69 656e 742e 7075 7368 2866     client.push(f
-00025bb0: 227b 7365 6c66 2e70 7265 6669 787d 2f74  "{self.prefix}/t
-00025bc0: 6573 7422 2c20 6f72 6967 696e 616c 5f64  est", original_d
-00025bd0: 6174 612c 2065 6e63 6f64 696e 673d 4e6f  ata, encoding=No
-00025be0: 6e65 290a 2020 2020 2020 2020 7769 7468  ne).        with
-00025bf0: 2063 6c69 656e 742e 7075 6c6c 2866 227b   client.pull(f"{
-00025c00: 7365 6c66 2e70 7265 6669 787d 2f74 6573  self.prefix}/tes
-00025c10: 7422 2c20 656e 636f 6469 6e67 3d4e 6f6e  t", encoding=Non
-00025c20: 6529 2061 7320 696e 6669 6c65 3a0a 2020  e) as infile:.  
-00025c30: 2020 2020 2020 2020 2020 7265 6365 6976            receiv
-00025c40: 6564 5f64 6174 6120 3d20 696e 6669 6c65  ed_data = infile
-00025c50: 2e72 6561 6428 290a 2020 2020 2020 2020  .read().        
-00025c60: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00025c70: 286f 7269 6769 6e61 6c5f 6461 7461 2c20  (original_data, 
-00025c80: 7265 6365 6976 6564 5f64 6174 6129 0a0a  received_data)..
-00025c90: 2020 2020 6465 6620 7465 7374 5f70 7573      def test_pus
-00025ca0: 685f 746f 5f6e 6f6e 5f65 7869 7374 656e  h_to_non_existen
-00025cb0: 745f 7375 6264 6972 2873 656c 6629 3a0a  t_subdir(self):.
-00025cc0: 2020 2020 2020 2020 6461 7461 203d 2027          data = '
-00025cd0: 6461 7461 270a 2020 2020 2020 2020 636c  data'.        cl
-00025ce0: 6965 6e74 203d 2073 656c 662e 636c 6965  ient = self.clie
-00025cf0: 6e74 0a0a 2020 2020 2020 2020 7769 7468  nt..        with
-00025d00: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
-00025d10: 6573 2870 6562 626c 652e 5061 7468 4572  es(pebble.PathEr
-00025d20: 726f 7229 2061 7320 636d 3a0a 2020 2020  ror) as cm:.    
-00025d30: 2020 2020 2020 2020 636c 6965 6e74 2e70          client.p
-00025d40: 7573 6828 6622 7b73 656c 662e 7072 6566  ush(f"{self.pref
-00025d50: 6978 7d2f 6e6f 6e65 7869 7374 656e 745f  ix}/nonexistent_
-00025d60: 6469 722f 7465 7374 222c 2064 6174 612c  dir/test", data,
-00025d70: 206d 616b 655f 6469 7273 3d46 616c 7365   make_dirs=False
-00025d80: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00025d90: 7373 6572 7445 7175 616c 2863 6d2e 6578  ssertEqual(cm.ex
-00025da0: 6365 7074 696f 6e2e 6b69 6e64 2c20 276e  ception.kind, 'n
-00025db0: 6f74 2d66 6f75 6e64 2729 0a0a 2020 2020  ot-found')..    
-00025dc0: 2020 2020 636c 6965 6e74 2e70 7573 6828      client.push(
-00025dd0: 6622 7b73 656c 662e 7072 6566 6978 7d2f  f"{self.prefix}/
-00025de0: 6e6f 6e65 7869 7374 656e 745f 6469 722f  nonexistent_dir/
-00025df0: 7465 7374 222c 2064 6174 612c 206d 616b  test", data, mak
-00025e00: 655f 6469 7273 3d54 7275 6529 0a0a 2020  e_dirs=True)..  
-00025e10: 2020 6465 6620 7465 7374 5f70 7573 685f    def test_push_
-00025e20: 6173 5f63 6869 6c64 5f6f 665f 6669 6c65  as_child_of_file
-00025e30: 5f72 6169 7365 735f 6572 726f 7228 7365  _raises_error(se
-00025e40: 6c66 293a 0a20 2020 2020 2020 2064 6174  lf):.        dat
-00025e50: 6120 3d20 2764 6174 6127 0a20 2020 2020  a = 'data'.     
-00025e60: 2020 2063 6c69 656e 7420 3d20 7365 6c66     client = self
-00025e70: 2e63 6c69 656e 740a 2020 2020 2020 2020  .client.        
-00025e80: 636c 6965 6e74 2e70 7573 6828 6622 7b73  client.push(f"{s
-00025e90: 656c 662e 7072 6566 6978 7d2f 6669 6c65  elf.prefix}/file
-00025ea0: 222c 2064 6174 6129 0a20 2020 2020 2020  ", data).       
-00025eb0: 2077 6974 6820 7365 6c66 2e61 7373 6572   with self.asser
-00025ec0: 7452 6169 7365 7328 7065 6262 6c65 2e50  tRaises(pebble.P
-00025ed0: 6174 6845 7272 6f72 2920 6173 2063 6d3a  athError) as cm:
-00025ee0: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-00025ef0: 656e 742e 7075 7368 2866 227b 7365 6c66  ent.push(f"{self
-00025f00: 2e70 7265 6669 787d 2f66 696c 652f 6669  .prefix}/file/fi
-00025f10: 6c65 222c 2064 6174 6129 0a20 2020 2020  le", data).     
-00025f20: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00025f30: 7561 6c28 636d 2e65 7863 6570 7469 6f6e  ual(cm.exception
-00025f40: 2e6b 696e 642c 2027 6765 6e65 7269 632d  .kind, 'generic-
-00025f50: 6669 6c65 2d65 7272 6f72 2729 0a0a 2020  file-error')..  
-00025f60: 2020 6465 6620 7465 7374 5f70 7573 685f    def test_push_
-00025f70: 7769 7468 5f70 6572 6d69 7373 696f 6e5f  with_permission_
-00025f80: 6d61 736b 2873 656c 6629 3a0a 2020 2020  mask(self):.    
-00025f90: 2020 2020 6461 7461 203d 2027 6461 7461      data = 'data
-00025fa0: 270a 2020 2020 2020 2020 636c 6965 6e74  '.        client
-00025fb0: 203d 2073 656c 662e 636c 6965 6e74 0a20   = self.client. 
-00025fc0: 2020 2020 2020 2063 6c69 656e 742e 7075         client.pu
-00025fd0: 7368 2866 227b 7365 6c66 2e70 7265 6669  sh(f"{self.prefi
-00025fe0: 787d 2f66 696c 6522 2c20 6461 7461 2c20  x}/file", data, 
-00025ff0: 7065 726d 6973 7369 6f6e 733d 306f 3630  permissions=0o60
-00026000: 3029 0a20 2020 2020 2020 2063 6c69 656e  0).        clien
-00026010: 742e 7075 7368 2866 227b 7365 6c66 2e70  t.push(f"{self.p
-00026020: 7265 6669 787d 2f66 696c 6522 2c20 6461  refix}/file", da
-00026030: 7461 2c20 7065 726d 6973 7369 6f6e 733d  ta, permissions=
-00026040: 306f 3737 3729 0a20 2020 2020 2020 2023  0o777).        #
-00026050: 2049 6620 7065 726d 6973 7369 6f6e 7320   If permissions 
-00026060: 6172 6520 6f75 7473 6964 6520 6f66 2074  are outside of t
-00026070: 6865 2072 616e 6765 2030 6f30 3030 2074  he range 0o000 t
-00026080: 6872 6f75 6768 2030 6f37 3737 2c20 616e  hrough 0o777, an
-00026090: 2065 7863 6570 7469 6f6e 2073 686f 756c   exception shoul
-000260a0: 6420 6265 0a20 2020 2020 2020 2023 2072  d be.        # r
-000260b0: 6169 7365 642e 0a20 2020 2020 2020 2066  aised..        f
-000260c0: 6f72 2062 6164 5f70 6572 6d69 7373 696f  or bad_permissio
-000260d0: 6e20 696e 2028 0a20 2020 2020 2020 2020  n in (.         
-000260e0: 2020 2030 6f31 3030 302c 2020 2320 4578     0o1000,  # Ex
-000260f0: 6365 6564 7320 306f 3737 370a 2020 2020  ceeds 0o777.    
-00026100: 2020 2020 2020 2020 2d31 2c20 2020 2020          -1,     
-00026110: 2023 204c 6573 7320 7468 616e 2030 6f30   # Less than 0o0
-00026120: 3030 0a20 2020 2020 2020 2029 3a0a 2020  00.        ):.  
-00026130: 2020 2020 2020 2020 2020 7769 7468 2073            with s
-00026140: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
-00026150: 2870 6562 626c 652e 5061 7468 4572 726f  (pebble.PathErro
-00026160: 7229 2061 7320 636d 3a0a 2020 2020 2020  r) as cm:.      
-00026170: 2020 2020 2020 2020 2020 636c 6965 6e74            client
-00026180: 2e70 7573 6828 6622 7b73 656c 662e 7072  .push(f"{self.pr
-00026190: 6566 6978 7d2f 6669 6c65 222c 2064 6174  efix}/file", dat
-000261a0: 612c 2070 6572 6d69 7373 696f 6e73 3d62  a, permissions=b
-000261b0: 6164 5f70 6572 6d69 7373 696f 6e29 0a20  ad_permission). 
-000261c0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000261d0: 7274 4571 7561 6c28 636d 2e65 7863 6570  rtEqual(cm.excep
-000261e0: 7469 6f6e 2e6b 696e 642c 2027 6765 6e65  tion.kind, 'gene
-000261f0: 7269 632d 6669 6c65 2d65 7272 6f72 2729  ric-file-error')
-00026200: 0a0a 2020 2020 6465 6620 7465 7374 5f70  ..    def test_p
-00026210: 7573 685f 6669 6c65 735f 616e 645f 6c69  ush_files_and_li
-00026220: 7374 2873 656c 6629 3a0a 2020 2020 2020  st(self):.      
-00026230: 2020 6461 7461 203d 2027 6461 7461 270a    data = 'data'.
-00026240: 2020 2020 2020 2020 636c 6965 6e74 203d          client =
-00026250: 2073 656c 662e 636c 6965 6e74 0a0a 2020   self.client..  
-00026260: 2020 2020 2020 2320 4c65 7427 7320 7075        # Let's pu
-00026270: 7368 2074 6865 2066 6972 7374 2066 696c  sh the first fil
-00026280: 6520 7769 7468 2061 2062 756e 6368 206f  e with a bunch o
-00026290: 6620 6465 7461 696c 732e 2020 5765 276c  f details.  We'l
-000262a0: 6c20 6368 6563 6b20 6f6e 2074 6869 7320  l check on this 
-000262b0: 6c61 7465 722e 0a20 2020 2020 2020 2063  later..        c
-000262c0: 6c69 656e 742e 7075 7368 280a 2020 2020  lient.push(.    
-000262d0: 2020 2020 2020 2020 6622 7b73 656c 662e          f"{self.
-000262e0: 7072 6566 6978 7d2f 6669 6c65 3122 2c20  prefix}/file1", 
-000262f0: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
-00026300: 2020 7065 726d 6973 7369 6f6e 733d 306f    permissions=0o
-00026310: 3632 3029 0a0a 2020 2020 2020 2020 2320  620)..        # 
-00026320: 446f 2061 2071 7569 636b 2070 7573 6820  Do a quick push 
-00026330: 7769 7468 2064 6566 6175 6c74 7320 666f  with defaults fo
-00026340: 7220 7468 6520 6f74 6865 7220 6669 6c65  r the other file
-00026350: 732e 0a20 2020 2020 2020 2063 6c69 656e  s..        clien
-00026360: 742e 7075 7368 2866 227b 7365 6c66 2e70  t.push(f"{self.p
-00026370: 7265 6669 787d 2f66 696c 6532 222c 2064  refix}/file2", d
-00026380: 6174 6129 0a20 2020 2020 2020 2063 6c69  ata).        cli
-00026390: 656e 742e 7075 7368 2866 227b 7365 6c66  ent.push(f"{self
-000263a0: 2e70 7265 6669 787d 2f66 696c 6533 222c  .prefix}/file3",
-000263b0: 2064 6174 6129 0a0a 2020 2020 2020 2020   data)..        
-000263c0: 6669 6c65 7320 3d20 636c 6965 6e74 2e6c  files = client.l
-000263d0: 6973 745f 6669 6c65 7328 6622 7b73 656c  ist_files(f"{sel
-000263e0: 662e 7072 6566 6978 7d2f 2229 0a20 2020  f.prefix}/").   
-000263f0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00026400: 4571 7561 6c28 7b66 696c 652e 7061 7468  Equal({file.path
-00026410: 2066 6f72 2066 696c 6520 696e 2066 696c   for file in fil
-00026420: 6573 7d2c 0a20 2020 2020 2020 2020 2020  es},.           
-00026430: 2020 2020 2020 2020 2020 2020 2020 7b73                {s
-00026440: 656c 662e 7072 6566 6978 202b 2066 696c  elf.prefix + fil
-00026450: 6520 666f 7220 6669 6c65 2069 6e20 2827  e for file in ('
-00026460: 2f66 696c 6531 272c 2027 2f66 696c 6532  /file1', '/file2
-00026470: 272c 2027 2f66 696c 6533 2729 7d29 0a0a  ', '/file3')})..
-00026480: 2020 2020 2020 2020 2320 4c65 7427 7320          # Let's 
-00026490: 7075 6c6c 2074 6865 2066 6972 7374 2066  pull the first f
-000264a0: 696c 6520 6167 6169 6e20 616e 6420 6368  ile again and ch
-000264b0: 6563 6b20 6974 7320 6465 7461 696c 730a  eck its details.
-000264c0: 2020 2020 2020 2020 6669 6c65 203d 205b          file = [
-000264d0: 6620 666f 7220 6620 696e 2066 696c 6573  f for f in files
-000264e0: 2069 6620 662e 7061 7468 203d 3d20 6622   if f.path == f"
-000264f0: 7b73 656c 662e 7072 6566 6978 7d2f 6669  {self.prefix}/fi
-00026500: 6c65 3122 5d5b 305d 0a20 2020 2020 2020  le1"][0].       
-00026510: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00026520: 6c28 6669 6c65 2e6e 616d 652c 2027 6669  l(file.name, 'fi
-00026530: 6c65 3127 290a 2020 2020 2020 2020 7365  le1').        se
-00026540: 6c66 2e61 7373 6572 7445 7175 616c 2866  lf.assertEqual(f
-00026550: 696c 652e 7479 7065 2c20 7065 6262 6c65  ile.type, pebble
-00026560: 2e46 696c 6554 7970 652e 4649 4c45 290a  .FileType.FILE).
-00026570: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00026580: 6572 7445 7175 616c 2866 696c 652e 7369  ertEqual(file.si
-00026590: 7a65 2c20 3429 0a20 2020 2020 2020 2073  ze, 4).        s
-000265a0: 656c 662e 6173 7365 7274 4973 496e 7374  elf.assertIsInst
-000265b0: 616e 6365 2866 696c 652e 6c61 7374 5f6d  ance(file.last_m
-000265c0: 6f64 6966 6965 642c 2064 6174 6574 696d  odified, datetim
-000265d0: 652e 6461 7465 7469 6d65 290a 2020 2020  e.datetime).    
-000265e0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-000265f0: 7175 616c 2866 696c 652e 7065 726d 6973  qual(file.permis
-00026600: 7369 6f6e 732c 2030 6f36 3230 290a 2020  sions, 0o620).  
-00026610: 2020 2020 2020 2320 536b 6970 7069 6e67        # Skipping
-00026620: 206f 776e 6572 7368 6970 2063 6865 636b   ownership check
-00026630: 7320 6865 7265 3b20 6f77 6e65 7273 6869  s here; ownershi
-00026640: 7020 7769 6c6c 2062 6520 6368 6563 6b65  p will be checke
-00026650: 6420 696e 2070 7572 656c 792d 6d6f 636b  d in purely-mock
-00026660: 6564 2074 6573 7473 0a0a 2020 2020 6465  ed tests..    de
-00026670: 6620 7465 7374 5f70 7573 685f 616e 645f  f test_push_and_
-00026680: 6c69 7374 5f66 696c 6528 7365 6c66 293a  list_file(self):
-00026690: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-000266a0: 2764 6174 6127 0a20 2020 2020 2020 2063  'data'.        c
-000266b0: 6c69 656e 7420 3d20 7365 6c66 2e63 6c69  lient = self.cli
-000266c0: 656e 740a 2020 2020 2020 2020 636c 6965  ent.        clie
-000266d0: 6e74 2e70 7573 6828 6622 7b73 656c 662e  nt.push(f"{self.
-000266e0: 7072 6566 6978 7d2f 6669 6c65 222c 2064  prefix}/file", d
-000266f0: 6174 6129 0a20 2020 2020 2020 2066 696c  ata).        fil
-00026700: 6573 203d 2063 6c69 656e 742e 6c69 7374  es = client.list
-00026710: 5f66 696c 6573 2866 227b 7365 6c66 2e70  _files(f"{self.p
-00026720: 7265 6669 787d 2f22 290a 2020 2020 2020  refix}/").      
-00026730: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00026740: 616c 287b 6669 6c65 2e70 6174 6820 666f  al({file.path fo
-00026750: 7220 6669 6c65 2069 6e20 6669 6c65 737d  r file in files}
-00026760: 2c20 7b66 227b 7365 6c66 2e70 7265 6669  , {f"{self.prefi
-00026770: 787d 2f66 696c 6522 7d29 0a0a 2020 2020  x}/file"})..    
-00026780: 6465 6620 7465 7374 5f70 7573 685f 6669  def test_push_fi
-00026790: 6c65 5f77 6974 685f 7265 6c61 7469 7665  le_with_relative
-000267a0: 5f70 6174 685f 6661 696c 7328 7365 6c66  _path_fails(self
-000267b0: 293a 0a20 2020 2020 2020 2063 6c69 656e  ):.        clien
-000267c0: 7420 3d20 7365 6c66 2e63 6c69 656e 740a  t = self.client.
-000267d0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-000267e0: 662e 6173 7365 7274 5261 6973 6573 2870  f.assertRaises(p
-000267f0: 6562 626c 652e 5061 7468 4572 726f 7229  ebble.PathError)
-00026800: 2061 7320 636d 3a0a 2020 2020 2020 2020   as cm:.        
-00026810: 2020 2020 636c 6965 6e74 2e70 7573 6828      client.push(
-00026820: 2766 696c 6527 2c20 2727 290a 2020 2020  'file', '').    
-00026830: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00026840: 7175 616c 2863 6d2e 6578 6365 7074 696f  qual(cm.exceptio
-00026850: 6e2e 6b69 6e64 2c20 2767 656e 6572 6963  n.kind, 'generic
-00026860: 2d66 696c 652d 6572 726f 7227 290a 0a20  -file-error').. 
-00026870: 2020 2064 6566 2074 6573 745f 7075 6c6c     def test_pull
-00026880: 5f6e 6f74 5f66 6f75 6e64 2873 656c 6629  _not_found(self)
-00026890: 3a0a 2020 2020 2020 2020 7769 7468 2073  :.        with s
-000268a0: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
-000268b0: 2870 6562 626c 652e 5061 7468 4572 726f  (pebble.PathErro
-000268c0: 7229 2061 7320 636d 3a0a 2020 2020 2020  r) as cm:.      
-000268d0: 2020 2020 2020 7365 6c66 2e63 6c69 656e        self.clien
-000268e0: 742e 7075 6c6c 2822 2f6e 6f74 2f66 6f75  t.pull("/not/fou
-000268f0: 6e64 2229 0a20 2020 2020 2020 2073 656c  nd").        sel
-00026900: 662e 6173 7365 7274 4571 7561 6c28 636d  f.assertEqual(cm
-00026910: 2e65 7863 6570 7469 6f6e 2e6b 696e 642c  .exception.kind,
-00026920: 2022 6e6f 742d 666f 756e 6422 290a 2020   "not-found").  
-00026930: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00026940: 7449 6e28 222f 6e6f 742f 666f 756e 6422  tIn("/not/found"
-00026950: 2c20 636d 2e65 7863 6570 7469 6f6e 2e6d  , cm.exception.m
-00026960: 6573 7361 6765 290a 0a20 2020 2064 6566  essage)..    def
-00026970: 2074 6573 745f 7075 6c6c 5f64 6972 6563   test_pull_direc
-00026980: 746f 7279 2873 656c 6629 3a0a 2020 2020  tory(self):.    
-00026990: 2020 2020 7365 6c66 2e63 6c69 656e 742e      self.client.
-000269a0: 6d61 6b65 5f64 6972 2866 227b 7365 6c66  make_dir(f"{self
-000269b0: 2e70 7265 6669 787d 2f73 7562 6469 7222  .prefix}/subdir"
-000269c0: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
-000269d0: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
-000269e0: 2870 6562 626c 652e 5061 7468 4572 726f  (pebble.PathErro
-000269f0: 7229 2061 7320 636d 3a0a 2020 2020 2020  r) as cm:.      
-00026a00: 2020 2020 2020 7365 6c66 2e63 6c69 656e        self.clien
-00026a10: 742e 7075 6c6c 2866 227b 7365 6c66 2e70  t.pull(f"{self.p
-00026a20: 7265 6669 787d 2f73 7562 6469 7222 290a  refix}/subdir").
-00026a30: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00026a40: 6572 7445 7175 616c 2863 6d2e 6578 6365  ertEqual(cm.exce
-00026a50: 7074 696f 6e2e 6b69 6e64 2c20 2267 656e  ption.kind, "gen
-00026a60: 6572 6963 2d66 696c 652d 6572 726f 7222  eric-file-error"
-00026a70: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00026a80: 7373 6572 7449 6e28 6622 7b73 656c 662e  ssertIn(f"{self.
-00026a90: 7072 6566 6978 7d2f 7375 6264 6972 222c  prefix}/subdir",
-00026aa0: 2063 6d2e 6578 6365 7074 696f 6e2e 6d65   cm.exception.me
-00026ab0: 7373 6167 6529 0a0a 2020 2020 6465 6620  ssage)..    def 
-00026ac0: 7465 7374 5f6c 6973 745f 6669 6c65 735f  test_list_files_
-00026ad0: 6e6f 745f 666f 756e 645f 7261 6973 6573  not_found_raises
-00026ae0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00026af0: 636c 6965 6e74 203d 2073 656c 662e 636c  client = self.cl
-00026b00: 6965 6e74 0a20 2020 2020 2020 2077 6974  ient.        wit
-00026b10: 6820 7365 6c66 2e61 7373 6572 7452 6169  h self.assertRai
-00026b20: 7365 7328 7065 6262 6c65 2e41 5049 4572  ses(pebble.APIEr
-00026b30: 726f 7229 2061 7320 636d 3a0a 2020 2020  ror) as cm:.    
-00026b40: 2020 2020 2020 2020 636c 6965 6e74 2e6c          client.l
-00026b50: 6973 745f 6669 6c65 7328 222f 6e6f 742f  ist_files("/not/
-00026b60: 6578 6973 7469 6e67 2f66 696c 652f 2229  existing/file/")
-00026b70: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00026b80: 7365 7274 4571 7561 6c28 636d 2e65 7863  sertEqual(cm.exc
-00026b90: 6570 7469 6f6e 2e63 6f64 652c 2034 3034  eption.code, 404
-00026ba0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00026bb0: 7373 6572 7445 7175 616c 2863 6d2e 6578  ssertEqual(cm.ex
-00026bc0: 6365 7074 696f 6e2e 7374 6174 7573 2c20  ception.status, 
-00026bd0: 274e 6f74 2046 6f75 6e64 2729 0a20 2020  'Not Found').   
-00026be0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00026bf0: 4571 7561 6c28 636d 2e65 7863 6570 7469  Equal(cm.excepti
-00026c00: 6f6e 2e6d 6573 7361 6765 2c20 2773 7461  on.message, 'sta
-00026c10: 7420 2f6e 6f74 2f65 7869 7374 696e 672f  t /not/existing/
-00026c20: 6669 6c65 2f3a 206e 6f20 270a 2020 2020  file/: no '.    
-00026c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026c50: 2020 2020 2020 2020 2020 2027 7375 6368             'such
-00026c60: 2066 696c 6520 6f72 2064 6972 6563 746f   file or directo
-00026c70: 7279 2729 0a0a 2020 2020 6465 6620 7465  ry')..    def te
-00026c80: 7374 5f6c 6973 745f 6469 7265 6374 6f72  st_list_director
-00026c90: 795f 6f62 6a65 6374 5f69 7473 656c 6628  y_object_itself(
-00026ca0: 7365 6c66 293a 0a20 2020 2020 2020 2063  self):.        c
-00026cb0: 6c69 656e 7420 3d20 7365 6c66 2e63 6c69  lient = self.cli
-00026cc0: 656e 740a 0a20 2020 2020 2020 2023 2054  ent..        # T
-00026cd0: 6573 7420 7769 7468 2072 6f6f 7420 6469  est with root di
-00026ce0: 720a 2020 2020 2020 2020 2320 2853 7065  r.        # (Spe
-00026cf0: 6369 616c 2063 6173 653b 2077 6520 776f  cial case; we wo
-00026d00: 6e27 7420 7072 6566 6978 2074 6869 732c  n't prefix this,
-00026d10: 2065 7665 6e20 7768 656e 2075 7369 6e67   even when using
-00026d20: 2074 6865 2072 6561 6c20 5065 6262 6c65   the real Pebble
-00026d30: 2073 6572 7665 722e 290a 2020 2020 2020   server.).      
-00026d40: 2020 6669 6c65 7320 3d20 636c 6965 6e74    files = client
-00026d50: 2e6c 6973 745f 6669 6c65 7328 272f 272c  .list_files('/',
-00026d60: 2069 7473 656c 663d 5472 7565 290a 2020   itself=True).  
-00026d70: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00026d80: 7445 7175 616c 286c 656e 2866 696c 6573  tEqual(len(files
-00026d90: 292c 2031 290a 2020 2020 2020 2020 6469  ), 1).        di
-00026da0: 725f 203d 2066 696c 6573 5b30 5d0a 2020  r_ = files[0].  
-00026db0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00026dc0: 7445 7175 616c 2864 6972 5f2e 7061 7468  tEqual(dir_.path
-00026dd0: 2c20 272f 2729 0a20 2020 2020 2020 2073  , '/').        s
-00026de0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00026df0: 6469 725f 2e6e 616d 652c 2027 2f27 290a  dir_.name, '/').
-00026e00: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00026e10: 6572 7445 7175 616c 2864 6972 5f2e 7479  ertEqual(dir_.ty
-00026e20: 7065 2c20 7065 6262 6c65 2e46 696c 6554  pe, pebble.FileT
-00026e30: 7970 652e 4449 5245 4354 4f52 5929 0a0a  ype.DIRECTORY)..
-00026e40: 2020 2020 2020 2020 2320 5465 7374 2077          # Test w
-00026e50: 6974 6820 7375 6264 6972 730a 2020 2020  ith subdirs.    
-00026e60: 2020 2020 636c 6965 6e74 2e6d 616b 655f      client.make_
-00026e70: 6469 7228 6622 7b73 656c 662e 7072 6566  dir(f"{self.pref
-00026e80: 6978 7d2f 7375 6264 6972 2229 0a20 2020  ix}/subdir").   
-00026e90: 2020 2020 2066 696c 6573 203d 2063 6c69       files = cli
-00026ea0: 656e 742e 6c69 7374 5f66 696c 6573 2866  ent.list_files(f
-00026eb0: 227b 7365 6c66 2e70 7265 6669 787d 2f73  "{self.prefix}/s
-00026ec0: 7562 6469 7222 2c20 6974 7365 6c66 3d54  ubdir", itself=T
-00026ed0: 7275 6529 0a20 2020 2020 2020 2073 656c  rue).        sel
-00026ee0: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
-00026ef0: 6e28 6669 6c65 7329 2c20 3129 0a20 2020  n(files), 1).   
-00026f00: 2020 2020 2064 6972 5f20 3d20 6669 6c65       dir_ = file
-00026f10: 735b 305d 0a20 2020 2020 2020 2073 656c  s[0].        sel
-00026f20: 662e 6173 7365 7274 4571 7561 6c28 6469  f.assertEqual(di
-00026f30: 725f 2e6e 616d 652c 2027 7375 6264 6972  r_.name, 'subdir
-00026f40: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-00026f50: 6173 7365 7274 4571 7561 6c28 6469 725f  assertEqual(dir_
-00026f60: 2e74 7970 652c 2070 6562 626c 652e 4669  .type, pebble.Fi
-00026f70: 6c65 5479 7065 2e44 4952 4543 544f 5259  leType.DIRECTORY
-00026f80: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00026f90: 7075 7368 5f66 696c 6573 5f61 6e64 5f6c  push_files_and_l
-00026fa0: 6973 745f 6279 5f70 6174 7465 726e 2873  ist_by_pattern(s
-00026fb0: 656c 6629 3a0a 2020 2020 2020 2020 2320  elf):.        # 
-00026fc0: 4e6f 7465 3a20 676c 6f62 2070 6174 7465  Note: glob patte
-00026fd0: 726e 2064 656c 7461 7320 646f 2065 7869  rn deltas do exi
-00026fe0: 7374 2062 6574 7765 656e 2067 6f6c 616e  st between golan
-00026ff0: 6720 616e 6420 5079 7468 6f6e 2c20 6275  g and Python, bu
-00027000: 7420 6865 7265 2c0a 2020 2020 2020 2020  t here,.        
-00027010: 2320 7765 276c 6c20 6a75 7374 2075 7365  # we'll just use
-00027020: 2061 2073 696d 706c 6520 2a20 7061 7474   a simple * patt
-00027030: 6572 6e2e 0a20 2020 2020 2020 2064 6174  ern..        dat
-00027040: 6120 3d20 2764 6174 6127 0a20 2020 2020  a = 'data'.     
-00027050: 2020 2063 6c69 656e 7420 3d20 7365 6c66     client = self
-00027060: 2e63 6c69 656e 740a 2020 2020 2020 2020  .client.        
-00027070: 666f 7220 6669 6c65 6e61 6d65 2069 6e20  for filename in 
-00027080: 280a 2020 2020 2020 2020 2020 2020 272f  (.            '/
-00027090: 6669 6c65 312e 677a 272c 0a20 2020 2020  file1.gz',.     
-000270a0: 2020 2020 2020 2027 2f66 696c 6532 2e74         '/file2.t
-000270b0: 6172 2e67 7a27 2c0a 2020 2020 2020 2020  ar.gz',.        
-000270c0: 2020 2020 272f 6669 6c65 332e 7461 722e      '/file3.tar.
-000270d0: 627a 3227 2c0a 2020 2020 2020 2020 2020  bz2',.          
-000270e0: 2020 272f 6261 636b 7570 5f66 696c 652e    '/backup_file.
-000270f0: 677a 272c 0a20 2020 2020 2020 2029 3a0a  gz',.        ):.
-00027100: 2020 2020 2020 2020 2020 2020 636c 6965              clie
-00027110: 6e74 2e70 7573 6828 7365 6c66 2e70 7265  nt.push(self.pre
-00027120: 6669 7820 2b20 6669 6c65 6e61 6d65 2c20  fix + filename, 
-00027130: 6461 7461 290a 2020 2020 2020 2020 6669  data).        fi
-00027140: 6c65 7320 3d20 636c 6965 6e74 2e6c 6973  les = client.lis
-00027150: 745f 6669 6c65 7328 6622 7b73 656c 662e  t_files(f"{self.
-00027160: 7072 6566 6978 7d2f 222c 2070 6174 7465  prefix}/", patte
-00027170: 726e 3d27 6669 6c65 2a2e 677a 2729 0a20  rn='file*.gz'). 
-00027180: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00027190: 7274 4571 7561 6c28 7b66 696c 652e 7061  rtEqual({file.pa
-000271a0: 7468 2066 6f72 2066 696c 6520 696e 2066  th for file in f
-000271b0: 696c 6573 7d2c 0a20 2020 2020 2020 2020  iles},.         
-000271c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000271d0: 7b73 656c 662e 7072 6566 6978 202b 2066  {self.prefix + f
-000271e0: 696c 6520 666f 7220 6669 6c65 2069 6e20  ile for file in 
-000271f0: 2827 2f66 696c 6531 2e67 7a27 2c20 272f  ('/file1.gz', '/
-00027200: 6669 6c65 322e 7461 722e 677a 2729 7d29  file2.tar.gz')})
-00027210: 0a0a 2020 2020 6465 6620 7465 7374 5f6d  ..    def test_m
-00027220: 616b 655f 6469 7265 6374 6f72 7928 7365  ake_directory(se
-00027230: 6c66 293a 0a20 2020 2020 2020 2063 6c69  lf):.        cli
-00027240: 656e 7420 3d20 7365 6c66 2e63 6c69 656e  ent = self.clien
-00027250: 740a 2020 2020 2020 2020 636c 6965 6e74  t.        client
-00027260: 2e6d 616b 655f 6469 7228 6622 7b73 656c  .make_dir(f"{sel
-00027270: 662e 7072 6566 6978 7d2f 7375 6264 6972  f.prefix}/subdir
-00027280: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00027290: 6173 7365 7274 4571 7561 6c28 0a20 2020  assertEqual(.   
-000272a0: 2020 2020 2020 2020 2063 6c69 656e 742e           client.
-000272b0: 6c69 7374 5f66 696c 6573 2866 227b 7365  list_files(f"{se
-000272c0: 6c66 2e70 7265 6669 787d 2f22 2c20 7061  lf.prefix}/", pa
-000272d0: 7474 6572 6e3d 2773 7562 6469 7227 295b  ttern='subdir')[
-000272e0: 305d 2e70 6174 682c 0a20 2020 2020 2020  0].path,.       
-000272f0: 2020 2020 2066 227b 7365 6c66 2e70 7265       f"{self.pre
-00027300: 6669 787d 2f73 7562 6469 7222 290a 2020  fix}/subdir").  
-00027310: 2020 2020 2020 636c 6965 6e74 2e6d 616b        client.mak
-00027320: 655f 6469 7228 6622 7b73 656c 662e 7072  e_dir(f"{self.pr
-00027330: 6566 6978 7d2f 7375 6264 6972 2f73 7562  efix}/subdir/sub
-00027340: 6469 7222 290a 2020 2020 2020 2020 7365  dir").        se
-00027350: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
-00027360: 2020 2020 2020 2020 2020 2020 636c 6965              clie
-00027370: 6e74 2e6c 6973 745f 6669 6c65 7328 6622  nt.list_files(f"
-00027380: 7b73 656c 662e 7072 6566 6978 7d2f 7375  {self.prefix}/su
-00027390: 6264 6972 222c 2070 6174 7465 726e 3d27  bdir", pattern='
-000273a0: 7375 6264 6972 2729 5b30 5d2e 7061 7468  subdir')[0].path
-000273b0: 2c0a 2020 2020 2020 2020 2020 2020 6622  ,.            f"
-000273c0: 7b73 656c 662e 7072 6566 6978 7d2f 7375  {self.prefix}/su
-000273d0: 6264 6972 2f73 7562 6469 7222 290a 0a20  bdir/subdir").. 
-000273e0: 2020 2064 6566 2074 6573 745f 6d61 6b65     def test_make
-000273f0: 5f64 6972 6563 746f 7279 5f72 6563 7572  _directory_recur
-00027400: 7369 7665 6c79 2873 656c 6629 3a0a 2020  sively(self):.  
-00027410: 2020 2020 2020 636c 6965 6e74 203d 2073        client = s
-00027420: 656c 662e 636c 6965 6e74 0a0a 2020 2020  elf.client..    
-00027430: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
-00027440: 7365 7274 5261 6973 6573 2870 6562 626c  sertRaises(pebbl
-00027450: 652e 5061 7468 4572 726f 7229 2061 7320  e.PathError) as 
-00027460: 636d 3a0a 2020 2020 2020 2020 2020 2020  cm:.            
-00027470: 636c 6965 6e74 2e6d 616b 655f 6469 7228  client.make_dir(
-00027480: 6622 7b73 656c 662e 7072 6566 6978 7d2f  f"{self.prefix}/
-00027490: 7375 6264 6972 2f73 7562 6469 7222 2c20  subdir/subdir", 
-000274a0: 6d61 6b65 5f70 6172 656e 7473 3d46 616c  make_parents=Fal
-000274b0: 7365 290a 2020 2020 2020 2020 7365 6c66  se).        self
-000274c0: 2e61 7373 6572 7445 7175 616c 2863 6d2e  .assertEqual(cm.
-000274d0: 6578 6365 7074 696f 6e2e 6b69 6e64 2c20  exception.kind, 
-000274e0: 276e 6f74 2d66 6f75 6e64 2729 0a0a 2020  'not-found')..  
-000274f0: 2020 2020 2020 636c 6965 6e74 2e6d 616b        client.mak
-00027500: 655f 6469 7228 6622 7b73 656c 662e 7072  e_dir(f"{self.pr
-00027510: 6566 6978 7d2f 7375 6264 6972 2f73 7562  efix}/subdir/sub
-00027520: 6469 7222 2c20 6d61 6b65 5f70 6172 656e  dir", make_paren
-00027530: 7473 3d54 7275 6529 0a20 2020 2020 2020  ts=True).       
-00027540: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00027550: 6c28 0a20 2020 2020 2020 2020 2020 2063  l(.            c
-00027560: 6c69 656e 742e 6c69 7374 5f66 696c 6573  lient.list_files
-00027570: 2866 227b 7365 6c66 2e70 7265 6669 787d  (f"{self.prefix}
-00027580: 2f73 7562 6469 7222 2c20 7061 7474 6572  /subdir", patter
-00027590: 6e3d 2773 7562 6469 7227 295b 305d 2e70  n='subdir')[0].p
-000275a0: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
-000275b0: 2066 227b 7365 6c66 2e70 7265 6669 787d   f"{self.prefix}
-000275c0: 2f73 7562 6469 722f 7375 6264 6972 2229  /subdir/subdir")
-000275d0: 0a0a 2020 2020 6465 6620 7465 7374 5f6d  ..    def test_m
-000275e0: 616b 655f 6469 7265 6374 6f72 795f 7769  ake_directory_wi
-000275f0: 7468 5f72 656c 6174 6976 655f 7061 7468  th_relative_path
-00027600: 5f66 6169 6c73 2873 656c 6629 3a0a 2020  _fails(self):.  
-00027610: 2020 2020 2020 636c 6965 6e74 203d 2073        client = s
-00027620: 656c 662e 636c 6965 6e74 0a20 2020 2020  elf.client.     
-00027630: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
-00027640: 6572 7452 6169 7365 7328 7065 6262 6c65  ertRaises(pebble
-00027650: 2e50 6174 6845 7272 6f72 2920 6173 2063  .PathError) as c
-00027660: 6d3a 0a20 2020 2020 2020 2020 2020 2063  m:.            c
-00027670: 6c69 656e 742e 6d61 6b65 5f64 6972 2827  lient.make_dir('
-00027680: 6469 7227 290a 2020 2020 2020 2020 7365  dir').        se
-00027690: 6c66 2e61 7373 6572 7445 7175 616c 2863  lf.assertEqual(c
-000276a0: 6d2e 6578 6365 7074 696f 6e2e 6b69 6e64  m.exception.kind
-000276b0: 2c20 2767 656e 6572 6963 2d66 696c 652d  , 'generic-file-
-000276c0: 6572 726f 7227 290a 0a20 2020 2064 6566  error')..    def
-000276d0: 2074 6573 745f 6d61 6b65 5f73 7562 6469   test_make_subdi
-000276e0: 725f 6f66 5f66 696c 655f 6661 696c 7328  r_of_file_fails(
-000276f0: 7365 6c66 293a 0a20 2020 2020 2020 2063  self):.        c
-00027700: 6c69 656e 7420 3d20 7365 6c66 2e63 6c69  lient = self.cli
-00027710: 656e 740a 2020 2020 2020 2020 636c 6965  ent.        clie
-00027720: 6e74 2e70 7573 6828 6622 7b73 656c 662e  nt.push(f"{self.
-00027730: 7072 6566 6978 7d2f 6669 6c65 222c 2027  prefix}/file", '
-00027740: 6461 7461 2729 0a0a 2020 2020 2020 2020  data')..        
-00027750: 2320 4469 7265 6374 2063 6869 6c64 2063  # Direct child c
-00027760: 6173 650a 2020 2020 2020 2020 7769 7468  ase.        with
-00027770: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
-00027780: 6573 2870 6562 626c 652e 5061 7468 4572  es(pebble.PathEr
-00027790: 726f 7229 2061 7320 636d 3a0a 2020 2020  ror) as cm:.    
-000277a0: 2020 2020 2020 2020 636c 6965 6e74 2e6d          client.m
-000277b0: 616b 655f 6469 7228 6622 7b73 656c 662e  ake_dir(f"{self.
-000277c0: 7072 6566 6978 7d2f 6669 6c65 2f73 7562  prefix}/file/sub
-000277d0: 6469 7222 290a 2020 2020 2020 2020 7365  dir").        se
-000277e0: 6c66 2e61 7373 6572 7445 7175 616c 2863  lf.assertEqual(c
-000277f0: 6d2e 6578 6365 7074 696f 6e2e 6b69 6e64  m.exception.kind
-00027800: 2c20 2767 656e 6572 6963 2d66 696c 652d  , 'generic-file-
-00027810: 6572 726f 7227 290a 0a20 2020 2020 2020  error')..       
-00027820: 2023 2052 6563 7572 7369 7665 2063 7265   # Recursive cre
-00027830: 6174 696f 6e20 6361 7365 2c20 696e 2063  ation case, in c
-00027840: 6173 6520 6974 7320 666c 6f77 2069 7320  ase its flow is 
-00027850: 6469 6666 6572 656e 740a 2020 2020 2020  different.      
-00027860: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
-00027870: 7274 5261 6973 6573 2870 6562 626c 652e  rtRaises(pebble.
-00027880: 5061 7468 4572 726f 7229 2061 7320 636d  PathError) as cm
-00027890: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
-000278a0: 6965 6e74 2e6d 616b 655f 6469 7228 6622  ient.make_dir(f"
-000278b0: 7b73 656c 662e 7072 6566 6978 7d2f 6669  {self.prefix}/fi
-000278c0: 6c65 2f73 7562 6469 722f 7375 6264 6972  le/subdir/subdir
-000278d0: 222c 206d 616b 655f 7061 7265 6e74 733d  ", make_parents=
-000278e0: 5472 7565 290a 2020 2020 2020 2020 7365  True).        se
-000278f0: 6c66 2e61 7373 6572 7445 7175 616c 2863  lf.assertEqual(c
-00027900: 6d2e 6578 6365 7074 696f 6e2e 6b69 6e64  m.exception.kind
-00027910: 2c20 2767 656e 6572 6963 2d66 696c 652d  , 'generic-file-
-00027920: 6572 726f 7227 290a 0a20 2020 2064 6566  error')..    def
-00027930: 2074 6573 745f 6d61 6b65 5f64 6972 5f77   test_make_dir_w
-00027940: 6974 685f 7065 726d 6973 7369 6f6e 5f6d  ith_permission_m
-00027950: 6173 6b28 7365 6c66 293a 0a20 2020 2020  ask(self):.     
-00027960: 2020 2063 6c69 656e 7420 3d20 7365 6c66     client = self
-00027970: 2e63 6c69 656e 740a 2020 2020 2020 2020  .client.        
-00027980: 636c 6965 6e74 2e6d 616b 655f 6469 7228  client.make_dir(
-00027990: 6622 7b73 656c 662e 7072 6566 6978 7d2f  f"{self.prefix}/
-000279a0: 6469 7231 222c 2070 6572 6d69 7373 696f  dir1", permissio
-000279b0: 6e73 3d30 6f37 3030 290a 2020 2020 2020  ns=0o700).      
-000279c0: 2020 636c 6965 6e74 2e6d 616b 655f 6469    client.make_di
-000279d0: 7228 6622 7b73 656c 662e 7072 6566 6978  r(f"{self.prefix
-000279e0: 7d2f 6469 7232 222c 2070 6572 6d69 7373  }/dir2", permiss
-000279f0: 696f 6e73 3d30 6f37 3737 290a 0a20 2020  ions=0o777)..   
-00027a00: 2020 2020 2066 696c 6573 203d 2063 6c69       files = cli
-00027a10: 656e 742e 6c69 7374 5f66 696c 6573 2866  ent.list_files(f
-00027a20: 227b 7365 6c66 2e70 7265 6669 787d 2f22  "{self.prefix}/"
-00027a30: 2c20 7061 7474 6572 6e3d 2764 6972 2a27  , pattern='dir*'
-00027a40: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00027a50: 7373 6572 7445 7175 616c 285b 6620 666f  ssertEqual([f fo
-00027a60: 7220 6620 696e 2066 696c 6573 2069 6620  r f in files if 
-00027a70: 662e 7061 7468 203d 3d20 6622 7b73 656c  f.path == f"{sel
-00027a80: 662e 7072 6566 6978 7d2f 6469 7231 225d  f.prefix}/dir1"]
-00027a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00027aa0: 2020 2020 2020 2020 2020 5b30 5d2e 7065            [0].pe
-00027ab0: 726d 6973 7369 6f6e 732c 2030 6f37 3030  rmissions, 0o700
-00027ac0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00027ad0: 7373 6572 7445 7175 616c 285b 6620 666f  ssertEqual([f fo
-00027ae0: 7220 6620 696e 2066 696c 6573 2069 6620  r f in files if 
-00027af0: 662e 7061 7468 203d 3d20 6622 7b73 656c  f.path == f"{sel
-00027b00: 662e 7072 6566 6978 7d2f 6469 7232 225d  f.prefix}/dir2"]
-00027b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00027b20: 2020 2020 2020 2020 2020 5b30 5d2e 7065            [0].pe
-00027b30: 726d 6973 7369 6f6e 732c 2030 6f37 3737  rmissions, 0o777
-00027b40: 290a 0a20 2020 2020 2020 2023 2049 6620  )..        # If 
-00027b50: 7065 726d 6973 7369 6f6e 7320 6172 6520  permissions are 
-00027b60: 6f75 7473 6964 6520 6f66 2074 6865 2072  outside of the r
-00027b70: 616e 6765 2030 6f30 3030 2074 6872 6f75  ange 0o000 throu
-00027b80: 6768 2030 6f37 3737 2c20 616e 2065 7863  gh 0o777, an exc
-00027b90: 6570 7469 6f6e 2073 686f 756c 6420 6265  eption should be
-00027ba0: 0a20 2020 2020 2020 2023 2072 6169 7365  .        # raise
-00027bb0: 642e 0a20 2020 2020 2020 2066 6f72 2069  d..        for i
-00027bc0: 2c20 6261 645f 7065 726d 6973 7369 6f6e  , bad_permission
-00027bd0: 2069 6e20 656e 756d 6572 6174 6528 280a   in enumerate((.
-00027be0: 2020 2020 2020 2020 2020 2020 306f 3130              0o10
-00027bf0: 3030 2c20 2023 2045 7863 6565 6473 2030  00,  # Exceeds 0
-00027c00: 6f37 3737 0a20 2020 2020 2020 2020 2020  o777.           
-00027c10: 202d 312c 2020 2020 2020 2320 4c65 7373   -1,      # Less
-00027c20: 2074 6861 6e20 306f 3030 300a 2020 2020   than 0o000.    
-00027c30: 2020 2020 2929 3a0a 2020 2020 2020 2020      )):.        
-00027c40: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
-00027c50: 7365 7274 5261 6973 6573 2870 6562 626c  sertRaises(pebbl
-00027c60: 652e 5061 7468 4572 726f 7229 2061 7320  e.PathError) as 
-00027c70: 636d 3a0a 2020 2020 2020 2020 2020 2020  cm:.            
-00027c80: 2020 2020 636c 6965 6e74 2e6d 616b 655f      client.make_
-00027c90: 6469 7228 6622 7b73 656c 662e 7072 6566  dir(f"{self.pref
-00027ca0: 6978 7d2f 6469 7233 5f7b 697d 222c 2070  ix}/dir3_{i}", p
-00027cb0: 6572 6d69 7373 696f 6e73 3d62 6164 5f70  ermissions=bad_p
-00027cc0: 6572 6d69 7373 696f 6e29 0a20 2020 2020  ermission).     
-00027cd0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00027ce0: 7274 4571 7561 6c28 636d 2e65 7863 6570  rtEqual(cm.excep
-00027cf0: 7469 6f6e 2e6b 696e 642c 2027 6765 6e65  tion.kind, 'gene
-00027d00: 7269 632d 6669 6c65 2d65 7272 6f72 2729  ric-file-error')
-00027d10: 0a0a 2020 2020 6465 6620 7465 7374 5f72  ..    def test_r
-00027d20: 656d 6f76 655f 7061 7468 2873 656c 6629  emove_path(self)
-00027d30: 3a0a 2020 2020 2020 2020 636c 6965 6e74  :.        client
-00027d40: 203d 2073 656c 662e 636c 6965 6e74 0a20   = self.client. 
-00027d50: 2020 2020 2020 2063 6c69 656e 742e 7075         client.pu
-00027d60: 7368 2866 227b 7365 6c66 2e70 7265 6669  sh(f"{self.prefi
-00027d70: 787d 2f66 696c 6522 2c20 2727 290a 2020  x}/file", '').  
-00027d80: 2020 2020 2020 636c 6965 6e74 2e6d 616b        client.mak
-00027d90: 655f 6469 7228 6622 7b73 656c 662e 7072  e_dir(f"{self.pr
-00027da0: 6566 6978 7d2f 6469 722f 7375 6264 6972  efix}/dir/subdir
-00027db0: 222c 206d 616b 655f 7061 7265 6e74 733d  ", make_parents=
-00027dc0: 5472 7565 290a 2020 2020 2020 2020 636c  True).        cl
-00027dd0: 6965 6e74 2e70 7573 6828 6622 7b73 656c  ient.push(f"{sel
-00027de0: 662e 7072 6566 6978 7d2f 6469 722f 7375  f.prefix}/dir/su
-00027df0: 6264 6972 2f66 696c 6531 222c 2027 2729  bdir/file1", '')
-00027e00: 0a20 2020 2020 2020 2063 6c69 656e 742e  .        client.
-00027e10: 7075 7368 2866 227b 7365 6c66 2e70 7265  push(f"{self.pre
-00027e20: 6669 787d 2f64 6972 2f73 7562 6469 722f  fix}/dir/subdir/
-00027e30: 6669 6c65 3222 2c20 2727 290a 2020 2020  file2", '').    
-00027e40: 2020 2020 636c 6965 6e74 2e70 7573 6828      client.push(
-00027e50: 6622 7b73 656c 662e 7072 6566 6978 7d2f  f"{self.prefix}/
-00027e60: 6469 722f 7375 6264 6972 2f66 696c 6533  dir/subdir/file3
-00027e70: 222c 2027 2729 0a20 2020 2020 2020 2063  ", '').        c
-00027e80: 6c69 656e 742e 6d61 6b65 5f64 6972 2866  lient.make_dir(f
-00027e90: 227b 7365 6c66 2e70 7265 6669 787d 2f65  "{self.prefix}/e
-00027ea0: 6d70 7479 5f64 6972 2229 0a0a 2020 2020  mpty_dir")..    
-00027eb0: 2020 2020 636c 6965 6e74 2e72 656d 6f76      client.remov
-00027ec0: 655f 7061 7468 2866 227b 7365 6c66 2e70  e_path(f"{self.p
-00027ed0: 7265 6669 787d 2f66 696c 6522 290a 0a20  refix}/file").. 
-00027ee0: 2020 2020 2020 2063 6c69 656e 742e 7265         client.re
-00027ef0: 6d6f 7665 5f70 6174 6828 6622 7b73 656c  move_path(f"{sel
-00027f00: 662e 7072 6566 6978 7d2f 656d 7074 795f  f.prefix}/empty_
-00027f10: 6469 7222 290a 0a20 2020 2020 2020 2023  dir")..        #
-00027f20: 2052 656d 6f76 6520 6e6f 6e2d 656d 7074   Remove non-empt
-00027f30: 7920 6469 7265 6374 6f72 792c 2072 6563  y directory, rec
-00027f40: 7572 7369 7665 3d46 616c 7365 3a20 6572  ursive=False: er
-00027f50: 726f 720a 2020 2020 2020 2020 7769 7468  ror.        with
-00027f60: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
-00027f70: 6573 2870 6562 626c 652e 5061 7468 4572  es(pebble.PathEr
-00027f80: 726f 7229 2061 7320 636d 3a0a 2020 2020  ror) as cm:.    
-00027f90: 2020 2020 2020 2020 636c 6965 6e74 2e72          client.r
-00027fa0: 656d 6f76 655f 7061 7468 2866 227b 7365  emove_path(f"{se
-00027fb0: 6c66 2e70 7265 6669 787d 2f64 6972 222c  lf.prefix}/dir",
-00027fc0: 2072 6563 7572 7369 7665 3d46 616c 7365   recursive=False
-00027fd0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00027fe0: 7373 6572 7445 7175 616c 2863 6d2e 6578  ssertEqual(cm.ex
-00027ff0: 6365 7074 696f 6e2e 6b69 6e64 2c20 2767  ception.kind, 'g
-00028000: 656e 6572 6963 2d66 696c 652d 6572 726f  eneric-file-erro
-00028010: 7227 290a 0a20 2020 2020 2020 2023 2052  r')..        # R
-00028020: 656d 6f76 6520 6e6f 6e2d 656d 7074 7920  emove non-empty 
-00028030: 6469 7265 6374 6f72 792c 2072 6563 7572  directory, recur
-00028040: 7369 7665 3d54 7275 653a 2073 7563 6365  sive=True: succe
-00028050: 6564 7320 2861 6e64 2072 656d 6f76 6573  eds (and removes
-00028060: 2063 6869 6c64 206f 626a 6563 7473 290a   child objects).
-00028070: 2020 2020 2020 2020 636c 6965 6e74 2e72          client.r
-00028080: 656d 6f76 655f 7061 7468 2866 227b 7365  emove_path(f"{se
-00028090: 6c66 2e70 7265 6669 787d 2f64 6972 222c  lf.prefix}/dir",
-000280a0: 2072 6563 7572 7369 7665 3d54 7275 6529   recursive=True)
-000280b0: 0a0a 2020 2020 2020 2020 2320 5265 6d6f  ..        # Remo
-000280c0: 7665 206e 6f6e 2d65 7869 7374 656e 7420  ve non-existent 
-000280d0: 7061 7468 2c20 7265 6375 7273 6976 653d  path, recursive=
-000280e0: 4661 6c73 653a 2065 7272 6f72 0a20 2020  False: error.   
-000280f0: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
-00028100: 7373 6572 7452 6169 7365 7328 7065 6262  ssertRaises(pebb
-00028110: 6c65 2e50 6174 6845 7272 6f72 2920 6173  le.PathError) as
-00028120: 2063 6d3a 0a20 2020 2020 2020 2020 2020   cm:.           
-00028130: 2063 6c69 656e 742e 7265 6d6f 7665 5f70   client.remove_p
-00028140: 6174 6828 6622 7b73 656c 662e 7072 6566  ath(f"{self.pref
-00028150: 6978 7d2f 6469 722f 646f 6573 2f6e 6f74  ix}/dir/does/not
-00028160: 2f65 7869 7374 2f61 7364 6622 2c20 7265  /exist/asdf", re
-00028170: 6375 7273 6976 653d 4661 6c73 6529 0a20  cursive=False). 
-00028180: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00028190: 7274 4571 7561 6c28 636d 2e65 7863 6570  rtEqual(cm.excep
-000281a0: 7469 6f6e 2e6b 696e 642c 2027 6e6f 742d  tion.kind, 'not-
-000281b0: 666f 756e 6427 290a 0a20 2020 2020 2020  found')..       
-000281c0: 2023 2052 656d 6f76 6520 6e6f 6e2d 6578   # Remove non-ex
-000281d0: 6973 7465 6e74 2070 6174 682c 2072 6563  istent path, rec
-000281e0: 7572 7369 7665 3d54 7275 653a 2073 7563  ursive=True: suc
-000281f0: 6365 6564 730a 2020 2020 2020 2020 636c  ceeds.        cl
-00028200: 6965 6e74 2e72 656d 6f76 655f 7061 7468  ient.remove_path
-00028210: 2866 227b 7365 6c66 2e70 7265 6669 787d  (f"{self.prefix}
-00028220: 2f64 6972 2f64 6f65 732f 6e6f 742f 6578  /dir/does/not/ex
-00028230: 6973 742f 6173 6466 222c 2072 6563 7572  ist/asdf", recur
-00028240: 7369 7665 3d54 7275 6529 0a0a 2020 2020  sive=True)..    
-00028250: 2320 4f74 6865 7220 6e6f 7465 733a 0a20  # Other notes:. 
-00028260: 2020 2023 202a 2050 6172 656e 7420 6469     # * Parent di
-00028270: 7265 6374 6f72 6965 7320 6372 6561 7465  rectories create
-00028280: 6420 7669 6120 7075 7368 286d 616b 655f  d via push(make_
-00028290: 6469 7273 3d54 7275 6529 2064 6566 6175  dirs=True) defau
-000282a0: 6c74 2074 6f20 726f 6f74 3a72 6f6f 7420  lt to root:root 
-000282b0: 6f77 6e65 7273 6869 700a 2020 2020 2320  ownership.    # 
-000282c0: 2020 616e 6420 7768 6174 6576 6572 2070    and whatever p
-000282d0: 6572 6d69 7373 696f 6e73 2061 7265 2073  ermissions are s
-000282e0: 7065 6369 6669 6564 2076 6961 2074 6865  pecified via the
-000282f0: 2070 6572 6d69 7373 696f 6e73 2061 7267   permissions arg
-00028300: 756d 656e 743b 2061 7320 7765 2064 6566  ument; as we def
-00028310: 6175 6c74 2074 6f20 4e6f 6e65 0a20 2020  ault to None.   
-00028320: 2023 2020 2066 6f72 206f 776e 6572 7368   #   for ownersh
-00028330: 6970 2f70 6572 6d69 7373 696f 6e73 2c20  ip/permissions, 
-00028340: 7765 2064 6f20 6967 6e6f 7265 2074 6869  we do ignore thi
-00028350: 7320 6e75 616e 6365 2e0a 2020 2020 2320  s nuance..    # 
-00028360: 2a20 5061 7265 6e74 2064 6972 6563 746f  * Parent directo
-00028370: 7269 6573 2063 7265 6174 6564 2076 6961  ries created via
-00028380: 206d 616b 655f 6469 7228 6d61 6b65 5f70   make_dir(make_p
-00028390: 6172 656e 7473 3d54 7275 6529 2064 6566  arents=True) def
-000283a0: 6175 6c74 2074 6f20 726f 6f74 3a72 6f6f  ault to root:roo
-000283b0: 7420 6f77 6e65 7273 6869 700a 2020 2020  t ownership.    
-000283c0: 2320 2020 616e 6420 306f 3735 3520 7065  #   and 0o755 pe
-000283d0: 726d 6973 7369 6f6e 733b 2061 7320 7765  rmissions; as we
-000283e0: 2064 6566 6175 6c74 2074 6f20 4e6f 6e65   default to None
-000283f0: 2066 6f72 206f 776e 6572 7368 6970 2f70   for ownership/p
-00028400: 6572 6d69 7373 696f 6e73 2c20 7765 2064  ermissions, we d
-00028410: 6f20 6967 6e6f 7265 2074 6869 730a 2020  o ignore this.  
-00028420: 2020 2320 2020 6e75 616e 6365 2e0a 0a0a    #   nuance....
-00028430: 636c 6173 7320 4765 6e65 7269 6354 6573  class GenericTes
-00028440: 7469 6e67 4669 6c65 7379 7374 656d 5465  tingFilesystemTe
-00028450: 7374 733a 0a20 2020 2064 6566 2074 6573  sts:.    def tes
-00028460: 745f 6c69 7374 6469 725f 726f 6f74 5f6f  t_listdir_root_o
-00028470: 6e5f 656d 7074 795f 6f73 2873 656c 6629  n_empty_os(self)
-00028480: 3a0a 2020 2020 2020 2020 7365 6c66 2e61  :.        self.a
-00028490: 7373 6572 7445 7175 616c 2873 656c 662e  ssertEqual(self.
-000284a0: 6673 2e6c 6973 745f 6469 7228 272f 2729  fs.list_dir('/')
-000284b0: 2c20 5b5d 290a 0a20 2020 2064 6566 2074  , [])..    def t
-000284c0: 6573 745f 6c69 7374 6469 725f 6f6e 5f6e  est_listdir_on_n
-000284d0: 6f6e 6578 6973 7465 6e74 5f64 6972 2873  onexistent_dir(s
-000284e0: 656c 6629 3a0a 2020 2020 2020 2020 7769  elf):.        wi
-000284f0: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
-00028500: 6973 6573 2846 696c 654e 6f74 466f 756e  ises(FileNotFoun
-00028510: 6445 7272 6f72 2920 6173 2063 6d3a 0a20  dError) as cm:. 
-00028520: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00028530: 6673 2e6c 6973 745f 6469 7228 272f 6574  fs.list_dir('/et
-00028540: 6327 290a 2020 2020 2020 2020 7365 6c66  c').        self
-00028550: 2e61 7373 6572 7454 7275 6528 272f 6574  .assertTrue('/et
-00028560: 6327 2069 6e20 636d 2e65 7863 6570 7469  c' in cm.excepti
-00028570: 6f6e 2e61 7267 735b 305d 290a 0a20 2020  on.args[0])..   
-00028580: 2064 6566 2074 6573 745f 6c69 7374 6469   def test_listdi
-00028590: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
-000285a0: 2073 656c 662e 6673 2e63 7265 6174 655f   self.fs.create_
-000285b0: 6469 7228 272f 6f70 7427 290a 2020 2020  dir('/opt').    
-000285c0: 2020 2020 7365 6c66 2e66 732e 6372 6561      self.fs.crea
-000285d0: 7465 5f66 696c 6528 272f 6f70 742f 6669  te_file('/opt/fi
-000285e0: 6c65 3127 2c20 2764 6174 6127 290a 2020  le1', 'data').  
-000285f0: 2020 2020 2020 7365 6c66 2e66 732e 6372        self.fs.cr
-00028600: 6561 7465 5f66 696c 6528 272f 6f70 742f  eate_file('/opt/
-00028610: 6669 6c65 3227 2c20 2764 6174 6127 290a  file2', 'data').
-00028620: 2020 2020 2020 2020 6578 7065 6374 6564          expected
-00028630: 5f72 6573 756c 7473 203d 207b 0a20 2020  _results = {.   
-00028640: 2020 2020 2020 2020 2070 6174 686c 6962           pathlib
-00028650: 2e50 7572 6550 6f73 6978 5061 7468 2827  .PurePosixPath('
-00028660: 2f6f 7074 2f66 696c 6531 2729 2c0a 2020  /opt/file1'),.  
-00028670: 2020 2020 2020 2020 2020 7061 7468 6c69            pathli
-00028680: 622e 5075 7265 506f 7369 7850 6174 6828  b.PurePosixPath(
-00028690: 272f 6f70 742f 6669 6c65 3227 297d 0a20  '/opt/file2')}. 
-000286a0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000286b0: 7274 4571 7561 6c28 6578 7065 6374 6564  rtEqual(expected
-000286c0: 5f72 6573 756c 7473 2c20 7b66 2e70 6174  _results, {f.pat
-000286d0: 6820 666f 7220 6620 696e 2073 656c 662e  h for f in self.
-000286e0: 6673 2e6c 6973 745f 6469 7228 272f 6f70  fs.list_dir('/op
-000286f0: 7427 297d 290a 2020 2020 2020 2020 2320  t')}).        # 
-00028700: 456e 7375 7265 2074 6861 7420 5061 7468  Ensure that Path
-00028710: 7320 616c 736f 2077 6f72 6b20 666f 7220  s also work for 
-00028720: 6c69 7374 6469 720a 2020 2020 2020 2020  listdir.        
-00028730: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00028740: 280a 2020 2020 2020 2020 2020 2020 6578  (.            ex
-00028750: 7065 6374 6564 5f72 6573 756c 7473 2c20  pected_results, 
-00028760: 7b66 2e70 6174 6820 666f 7220 6620 696e  {f.path for f in
-00028770: 2073 656c 662e 6673 2e6c 6973 745f 6469   self.fs.list_di
-00028780: 7228 7061 7468 6c69 622e 5075 7265 506f  r(pathlib.PurePo
-00028790: 7369 7850 6174 6828 272f 6f70 7427 2929  sixPath('/opt'))
-000287a0: 7d29 0a0a 2020 2020 6465 6620 7465 7374  })..    def test
-000287b0: 5f6c 6973 7464 6972 5f6f 6e5f 6669 6c65  _listdir_on_file
-000287c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000287d0: 7365 6c66 2e66 732e 6372 6561 7465 5f66  self.fs.create_f
-000287e0: 696c 6528 272f 6669 6c65 272c 2027 6461  ile('/file', 'da
-000287f0: 7461 2729 0a20 2020 2020 2020 2077 6974  ta').        wit
-00028800: 6820 7365 6c66 2e61 7373 6572 7452 6169  h self.assertRai
-00028810: 7365 7328 4e6f 7441 4469 7265 6374 6f72  ses(NotADirector
-00028820: 7945 7272 6f72 2920 6173 2063 6d3a 0a20  yError) as cm:. 
-00028830: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00028840: 6673 2e6c 6973 745f 6469 7228 272f 6669  fs.list_dir('/fi
-00028850: 6c65 2729 0a20 2020 2020 2020 2073 656c  le').        sel
-00028860: 662e 6173 7365 7274 5472 7565 2827 2f66  f.assertTrue('/f
-00028870: 696c 6527 2069 6e20 636d 2e65 7863 6570  ile' in cm.excep
-00028880: 7469 6f6e 2e61 7267 735b 305d 290a 0a20  tion.args[0]).. 
-00028890: 2020 2064 6566 2074 6573 745f 6d61 6b65     def test_make
-000288a0: 6469 7228 7365 6c66 293a 0a20 2020 2020  dir(self):.     
-000288b0: 2020 2064 203d 2073 656c 662e 6673 2e63     d = self.fs.c
-000288c0: 7265 6174 655f 6469 7228 272f 6574 6327  reate_dir('/etc'
-000288d0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-000288e0: 7373 6572 7445 7175 616c 2864 2e6e 616d  ssertEqual(d.nam
-000288f0: 652c 2027 6574 6327 290a 2020 2020 2020  e, 'etc').      
-00028900: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00028910: 616c 2864 2e70 6174 682c 2070 6174 686c  al(d.path, pathl
-00028920: 6962 2e50 7572 6550 6f73 6978 5061 7468  ib.PurePosixPath
-00028930: 2827 2f65 7463 2729 290a 2020 2020 2020  ('/etc')).      
-00028940: 2020 6432 203d 2073 656c 662e 6673 2e63    d2 = self.fs.c
-00028950: 7265 6174 655f 6469 7228 272f 6574 632f  reate_dir('/etc/
-00028960: 696e 6974 2e64 2729 0a20 2020 2020 2020  init.d').       
-00028970: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-00028980: 6c28 6432 2e6e 616d 652c 2027 696e 6974  l(d2.name, 'init
-00028990: 2e64 2729 0a20 2020 2020 2020 2073 656c  .d').        sel
-000289a0: 662e 6173 7365 7274 4571 7561 6c28 6432  f.assertEqual(d2
-000289b0: 2e70 6174 682c 2070 6174 686c 6962 2e50  .path, pathlib.P
-000289c0: 7572 6550 6f73 6978 5061 7468 2827 2f65  urePosixPath('/e
-000289d0: 7463 2f69 6e69 742e 6427 2929 0a0a 2020  tc/init.d'))..  
-000289e0: 2020 6465 6620 7465 7374 5f6d 616b 6564    def test_maked
-000289f0: 6972 5f66 6169 6c73 5f69 665f 616c 7265  ir_fails_if_alre
-00028a00: 6164 795f 6578 6973 7473 2873 656c 6629  ady_exists(self)
-00028a10: 3a0a 2020 2020 2020 2020 7365 6c66 2e66  :.        self.f
-00028a20: 732e 6372 6561 7465 5f64 6972 2827 2f65  s.create_dir('/e
-00028a30: 7463 2729 0a20 2020 2020 2020 2077 6974  tc').        wit
-00028a40: 6820 7365 6c66 2e61 7373 6572 7452 6169  h self.assertRai
-00028a50: 7365 7328 4669 6c65 4578 6973 7473 4572  ses(FileExistsEr
-00028a60: 726f 7229 2061 7320 636d 3a0a 2020 2020  ror) as cm:.    
-00028a70: 2020 2020 2020 2020 7365 6c66 2e66 732e          self.fs.
-00028a80: 6372 6561 7465 5f64 6972 2827 2f65 7463  create_dir('/etc
-00028a90: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-00028aa0: 6173 7365 7274 5472 7565 2827 2f65 7463  assertTrue('/etc
-00028ab0: 2720 696e 2063 6d2e 6578 6365 7074 696f  ' in cm.exceptio
-00028ac0: 6e2e 6172 6773 5b30 5d29 0a0a 2020 2020  n.args[0])..    
-00028ad0: 6465 6620 7465 7374 5f6d 616b 6564 6972  def test_makedir
-00028ae0: 5f73 7563 6365 6564 735f 6966 5f61 6c72  _succeeds_if_alr
-00028af0: 6561 6479 5f65 7869 7374 735f 7768 656e  eady_exists_when
-00028b00: 5f6d 616b 655f 7061 7265 6e74 735f 7472  _make_parents_tr
-00028b10: 7565 2873 656c 6629 3a0a 2020 2020 2020  ue(self):.      
-00028b20: 2020 6431 203d 2073 656c 662e 6673 2e63    d1 = self.fs.c
-00028b30: 7265 6174 655f 6469 7228 272f 6574 6327  reate_dir('/etc'
-00028b40: 290a 2020 2020 2020 2020 6432 203d 2073  ).        d2 = s
-00028b50: 656c 662e 6673 2e63 7265 6174 655f 6469  elf.fs.create_di
-00028b60: 7228 272f 6574 6327 2c20 6d61 6b65 5f70  r('/etc', make_p
-00028b70: 6172 656e 7473 3d54 7275 6529 0a20 2020  arents=True).   
-00028b80: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00028b90: 4571 7561 6c28 6431 2e70 6174 682c 2064  Equal(d1.path, d
-00028ba0: 322e 7061 7468 290a 2020 2020 2020 2020  2.path).        
-00028bb0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00028bc0: 2864 312e 6e61 6d65 2c20 6432 2e6e 616d  (d1.name, d2.nam
-00028bd0: 6529 0a0a 2020 2020 6465 6620 7465 7374  e)..    def test
-00028be0: 5f6d 616b 6564 6972 5f66 6169 6c73 5f69  _makedir_fails_i
-00028bf0: 665f 7061 7265 6e74 5f64 6972 5f64 6f65  f_parent_dir_doe
-00028c00: 736e 745f 6578 6973 7428 7365 6c66 293a  snt_exist(self):
-00028c10: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00028c20: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
-00028c30: 4669 6c65 4e6f 7446 6f75 6e64 4572 726f  FileNotFoundErro
-00028c40: 7229 2061 7320 636d 3a0a 2020 2020 2020  r) as cm:.      
-00028c50: 2020 2020 2020 7365 6c66 2e66 732e 6372        self.fs.cr
-00028c60: 6561 7465 5f64 6972 2827 2f65 7463 2f69  eate_dir('/etc/i
-00028c70: 6e69 742e 6427 290a 2020 2020 2020 2020  nit.d').        
-00028c80: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-00028c90: 272f 6574 6327 2069 6e20 636d 2e65 7863  '/etc' in cm.exc
-00028ca0: 6570 7469 6f6e 2e61 7267 735b 305d 290a  eption.args[0]).
-00028cb0: 0a20 2020 2064 6566 2074 6573 745f 6d61  .    def test_ma
-00028cc0: 6b65 5f61 6e64 5f6c 6973 745f 6469 7265  ke_and_list_dire
-00028cd0: 6374 6f72 7928 7365 6c66 293a 0a20 2020  ctory(self):.   
-00028ce0: 2020 2020 2073 656c 662e 6673 2e63 7265       self.fs.cre
-00028cf0: 6174 655f 6469 7228 272f 6574 6327 290a  ate_dir('/etc').
-00028d00: 2020 2020 2020 2020 7365 6c66 2e66 732e          self.fs.
-00028d10: 6372 6561 7465 5f64 6972 2827 2f76 6172  create_dir('/var
-00028d20: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-00028d30: 6173 7365 7274 4571 7561 6c28 0a20 2020  assertEqual(.   
-00028d40: 2020 2020 2020 2020 207b 662e 7061 7468           {f.path
-00028d50: 2066 6f72 2066 2069 6e20 7365 6c66 2e66   for f in self.f
-00028d60: 732e 6c69 7374 5f64 6972 2827 2f27 297d  s.list_dir('/')}
-00028d70: 2c0a 2020 2020 2020 2020 2020 2020 7b70  ,.            {p
-00028d80: 6174 686c 6962 2e50 7572 6550 6f73 6978  athlib.PurePosix
-00028d90: 5061 7468 2827 2f65 7463 2729 2c20 7061  Path('/etc'), pa
-00028da0: 7468 6c69 622e 5075 7265 506f 7369 7850  thlib.PurePosixP
-00028db0: 6174 6828 272f 7661 7227 297d 290a 0a20  ath('/var')}).. 
-00028dc0: 2020 2064 6566 2074 6573 745f 6d61 6b65     def test_make
-00028dd0: 5f64 6972 6563 746f 7279 5f72 6563 7572  _directory_recur
-00028de0: 7369 7665 6c79 2873 656c 6629 3a0a 2020  sively(self):.  
-00028df0: 2020 2020 2020 7365 6c66 2e66 732e 6372        self.fs.cr
-00028e00: 6561 7465 5f64 6972 2827 2f65 7463 2f69  eate_dir('/etc/i
-00028e10: 6e69 742e 6427 2c20 6d61 6b65 5f70 6172  nit.d', make_par
-00028e20: 656e 7473 3d54 7275 6529 0a20 2020 2020  ents=True).     
-00028e30: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00028e40: 7561 6c28 5b73 7472 286f 2e70 6174 6829  ual([str(o.path)
-00028e50: 2066 6f72 206f 2069 6e20 7365 6c66 2e66   for o in self.f
-00028e60: 732e 6c69 7374 5f64 6972 2827 2f27 295d  s.list_dir('/')]
-00028e70: 2c20 5b27 2f65 7463 275d 290a 2020 2020  , ['/etc']).    
-00028e80: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00028e90: 7175 616c 285b 7374 7228 6f2e 7061 7468  qual([str(o.path
-00028ea0: 2920 666f 7220 6f20 696e 2073 656c 662e  ) for o in self.
-00028eb0: 6673 2e6c 6973 745f 6469 7228 272f 6574  fs.list_dir('/et
-00028ec0: 6327 295d 2c20 5b27 2f65 7463 2f69 6e69  c')], ['/etc/ini
-00028ed0: 742e 6427 5d29 0a0a 2020 2020 6465 6620  t.d'])..    def 
-00028ee0: 7465 7374 5f6d 616b 6564 6972 5f70 6174  test_makedir_pat
-00028ef0: 685f 6d75 7374 5f73 7461 7274 5f77 6974  h_must_start_wit
-00028f00: 685f 736c 6173 6828 7365 6c66 293a 0a20  h_slash(self):. 
-00028f10: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00028f20: 2e61 7373 6572 7452 6169 7365 7328 4e6f  .assertRaises(No
-00028f30: 6e41 6273 6f6c 7574 6550 6174 6845 7272  nAbsolutePathErr
-00028f40: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
-00028f50: 2073 656c 662e 6673 2e63 7265 6174 655f   self.fs.create_
-00028f60: 6469 7228 226e 6f73 6c61 7368 2229 0a0a  dir("noslash")..
-00028f70: 2020 2020 6465 6620 7465 7374 5f63 7265      def test_cre
-00028f80: 6174 655f 6669 6c65 5f66 6169 6c73 5f69  ate_file_fails_i
-00028f90: 665f 7061 7265 6e74 5f64 6972 5f64 6f65  f_parent_dir_doe
-00028fa0: 736e 745f 6578 6973 7428 7365 6c66 293a  snt_exist(self):
-00028fb0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00028fc0: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
-00028fd0: 4669 6c65 4e6f 7446 6f75 6e64 4572 726f  FileNotFoundErro
-00028fe0: 7229 2061 7320 636d 3a0a 2020 2020 2020  r) as cm:.      
-00028ff0: 2020 2020 2020 7365 6c66 2e66 732e 6372        self.fs.cr
-00029000: 6561 7465 5f66 696c 6528 272f 6574 632f  eate_file('/etc/
-00029010: 7061 7373 7764 272c 2022 666f 6f22 290a  passwd', "foo").
-00029020: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00029030: 6572 7454 7275 6528 272f 6574 6327 2069  ertTrue('/etc' i
-00029040: 6e20 636d 2e65 7863 6570 7469 6f6e 2e61  n cm.exception.a
-00029050: 7267 735b 305d 290a 0a20 2020 2064 6566  rgs[0])..    def
-00029060: 2074 6573 745f 6372 6561 7465 5f66 696c   test_create_fil
-00029070: 655f 7375 6363 6565 6473 5f69 665f 7061  e_succeeds_if_pa
-00029080: 7265 6e74 5f64 6972 5f64 6f65 736e 745f  rent_dir_doesnt_
-00029090: 6578 6973 745f 7768 656e 5f6d 616b 655f  exist_when_make_
-000290a0: 6469 7273 5f74 7275 6528 7365 6c66 293a  dirs_true(self):
-000290b0: 0a20 2020 2020 2020 2073 656c 662e 6673  .        self.fs
-000290c0: 2e63 7265 6174 655f 6669 6c65 2827 2f74  .create_file('/t
-000290d0: 6573 742f 7375 6264 6972 2f74 6573 7466  est/subdir/testf
-000290e0: 696c 6527 2c20 2266 6f6f 222c 206d 616b  ile', "foo", mak
-000290f0: 655f 6469 7273 3d54 7275 6529 0a20 2020  e_dirs=True).   
-00029100: 2020 2020 2077 6974 6820 7365 6c66 2e66       with self.f
-00029110: 732e 6f70 656e 2827 2f74 6573 742f 7375  s.open('/test/su
-00029120: 6264 6972 2f74 6573 7466 696c 6527 2920  bdir/testfile') 
-00029130: 6173 2069 6e66 696c 653a 0a20 2020 2020  as infile:.     
-00029140: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00029150: 7274 4571 7561 6c28 696e 6669 6c65 2e72  rtEqual(infile.r
-00029160: 6561 6428 292c 2027 666f 6f27 290a 0a20  ead(), 'foo').. 
-00029170: 2020 2064 6566 2074 6573 745f 6372 6561     def test_crea
-00029180: 7465 5f66 696c 655f 6672 6f6d 5f73 7472  te_file_from_str
-00029190: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000291a0: 7365 6c66 2e66 732e 6372 6561 7465 5f66  self.fs.create_f
-000291b0: 696c 6528 272f 7465 7374 272c 2022 666f  ile('/test', "fo
-000291c0: 6f22 290a 2020 2020 2020 2020 7769 7468  o").        with
-000291d0: 2073 656c 662e 6673 2e6f 7065 6e28 272f   self.fs.open('/
-000291e0: 7465 7374 2729 2061 7320 696e 6669 6c65  test') as infile
-000291f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00029200: 6c66 2e61 7373 6572 7445 7175 616c 2869  lf.assertEqual(i
-00029210: 6e66 696c 652e 7265 6164 2829 2c20 2766  nfile.read(), 'f
-00029220: 6f6f 2729 0a0a 2020 2020 6465 6620 7465  oo')..    def te
-00029230: 7374 5f63 7265 6174 655f 6669 6c65 5f66  st_create_file_f
-00029240: 726f 6d5f 6279 7465 7328 7365 6c66 293a  rom_bytes(self):
-00029250: 0a20 2020 2020 2020 2073 656c 662e 6673  .        self.fs
-00029260: 2e63 7265 6174 655f 6669 6c65 2827 2f74  .create_file('/t
-00029270: 6573 7427 2c20 6222 666f 6f22 290a 2020  est', b"foo").  
-00029280: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00029290: 6673 2e6f 7065 6e28 272f 7465 7374 272c  fs.open('/test',
-000292a0: 2065 6e63 6f64 696e 673d 4e6f 6e65 2920   encoding=None) 
-000292b0: 6173 2069 6e66 696c 653a 0a20 2020 2020  as infile:.     
-000292c0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000292d0: 7274 4571 7561 6c28 696e 6669 6c65 2e72  rtEqual(infile.r
-000292e0: 6561 6428 292c 2062 2766 6f6f 2729 0a0a  ead(), b'foo')..
-000292f0: 2020 2020 6465 6620 7465 7374 5f63 7265      def test_cre
-00029300: 6174 655f 6669 6c65 5f66 726f 6d5f 6669  ate_file_from_fi
-00029310: 6c65 7328 7365 6c66 293a 0a20 2020 2020  les(self):.     
-00029320: 2020 2064 6174 6120 3d20 2266 6f6f 220a     data = "foo".
-00029330: 0a20 2020 2020 2020 2073 696f 203d 2053  .        sio = S
-00029340: 7472 696e 6749 4f28 6461 7461 290a 2020  tringIO(data).  
-00029350: 2020 2020 2020 7365 6c66 2e66 732e 6372        self.fs.cr
-00029360: 6561 7465 5f66 696c 6528 272f 7465 7374  eate_file('/test
-00029370: 272c 2073 696f 290a 2020 2020 2020 2020  ', sio).        
-00029380: 7769 7468 2073 656c 662e 6673 2e6f 7065  with self.fs.ope
-00029390: 6e28 272f 7465 7374 2729 2061 7320 696e  n('/test') as in
-000293a0: 6669 6c65 3a0a 2020 2020 2020 2020 2020  file:.          
-000293b0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000293c0: 616c 2869 6e66 696c 652e 7265 6164 2829  al(infile.read()
-000293d0: 2c20 2766 6f6f 2729 0a0a 2020 2020 2020  , 'foo')..      
-000293e0: 2020 6269 6f20 3d20 4279 7465 7349 4f28    bio = BytesIO(
-000293f0: 6461 7461 2e65 6e63 6f64 6528 2929 0a20  data.encode()). 
-00029400: 2020 2020 2020 2073 656c 662e 6673 2e63         self.fs.c
-00029410: 7265 6174 655f 6669 6c65 2827 2f74 6573  reate_file('/tes
-00029420: 7432 272c 2062 696f 290a 2020 2020 2020  t2', bio).      
-00029430: 2020 7769 7468 2073 656c 662e 6673 2e6f    with self.fs.o
-00029440: 7065 6e28 272f 7465 7374 3227 2920 6173  pen('/test2') as
-00029450: 2069 6e66 696c 653a 0a20 2020 2020 2020   infile:.       
-00029460: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00029470: 4571 7561 6c28 696e 6669 6c65 2e72 6561  Equal(infile.rea
-00029480: 6428 292c 2027 666f 6f27 290a 0a20 2020  d(), 'foo')..   
-00029490: 2064 6566 2074 6573 745f 6372 6561 7465   def test_create
-000294a0: 5f61 6e64 5f72 6561 645f 7769 7468 5f64  _and_read_with_d
-000294b0: 6966 6665 7265 6e74 5f65 6e63 6f64 696e  ifferent_encodin
-000294c0: 6773 2873 656c 6629 3a0a 2020 2020 2020  gs(self):.      
-000294d0: 2020 2320 7772 6974 6520 7374 722c 2072    # write str, r
-000294e0: 6561 6420 6173 2075 7466 2d38 2062 7974  ead as utf-8 byt
-000294f0: 6573 0a20 2020 2020 2020 2073 656c 662e  es.        self.
-00029500: 6673 2e63 7265 6174 655f 6669 6c65 2827  fs.create_file('
-00029510: 2f74 6573 7427 2c20 2266 6f6f 2229 0a20  /test', "foo"). 
-00029520: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00029530: 2e66 732e 6f70 656e 2827 2f74 6573 7427  .fs.open('/test'
-00029540: 2c20 656e 636f 6469 6e67 3d4e 6f6e 6529  , encoding=None)
-00029550: 2061 7320 696e 6669 6c65 3a0a 2020 2020   as infile:.    
-00029560: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00029570: 6572 7445 7175 616c 2869 6e66 696c 652e  ertEqual(infile.
-00029580: 7265 6164 2829 2c20 6227 666f 6f27 290a  read(), b'foo').
-00029590: 0a20 2020 2020 2020 2023 2077 7269 7465  .        # write
-000295a0: 2062 7974 6573 2c20 7265 6164 2061 7320   bytes, read as 
-000295b0: 7574 662d 382d 6465 636f 6465 6420 7374  utf-8-decoded st
-000295c0: 720a 2020 2020 2020 2020 6461 7461 203d  r.        data =
-000295d0: 2022 e697 a5e6 9cac e8aa 9e22 2020 2320   "........."  # 
-000295e0: 4a61 7061 6e65 7365 2066 6f72 2022 4a61  Japanese for "Ja
-000295f0: 7061 6e65 7365 220a 2020 2020 2020 2020  panese".        
-00029600: 7365 6c66 2e66 732e 6372 6561 7465 5f66  self.fs.create_f
-00029610: 696c 6528 272f 7465 7374 3227 2c20 6461  ile('/test2', da
-00029620: 7461 2e65 6e63 6f64 6528 2775 7466 2d38  ta.encode('utf-8
-00029630: 2729 290a 2020 2020 2020 2020 7769 7468  ')).        with
-00029640: 2073 656c 662e 6673 2e6f 7065 6e28 272f   self.fs.open('/
-00029650: 7465 7374 3227 2920 6173 2069 6e66 696c  test2') as infil
-00029660: 653a 2020 2020 2020 2020 2020 2020 2020  e:              
-00029670: 2020 2020 2020 2320 496d 706c 6963 6974        # Implicit
-00029680: 2075 7466 2d38 2072 6561 640a 2020 2020   utf-8 read.    
-00029690: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-000296a0: 6572 7445 7175 616c 2869 6e66 696c 652e  ertEqual(infile.
-000296b0: 7265 6164 2829 2c20 6461 7461 290a 2020  read(), data).  
-000296c0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-000296d0: 6673 2e6f 7065 6e28 272f 7465 7374 3227  fs.open('/test2'
-000296e0: 2c20 656e 636f 6469 6e67 3d27 7574 662d  , encoding='utf-
-000296f0: 3827 2920 6173 2069 6e66 696c 653a 2020  8') as infile:  
-00029700: 2320 4578 706c 6963 6974 2075 7466 2d38  # Explicit utf-8
-00029710: 2072 6561 640a 2020 2020 2020 2020 2020   read.          
-00029720: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00029730: 616c 2869 6e66 696c 652e 7265 6164 2829  al(infile.read()
-00029740: 2c20 6461 7461 290a 0a20 2020 2064 6566  , data)..    def
-00029750: 2074 6573 745f 6f70 656e 5f64 6972 6563   test_open_direc
-00029760: 746f 7279 5f66 6169 6c73 2873 656c 6629  tory_fails(self)
-00029770: 3a0a 2020 2020 2020 2020 7365 6c66 2e66  :.        self.f
-00029780: 732e 6372 6561 7465 5f64 6972 2827 2f64  s.create_dir('/d
-00029790: 6972 3127 290a 2020 2020 2020 2020 7769  ir1').        wi
-000297a0: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
-000297b0: 6973 6573 2849 7341 4469 7265 6374 6f72  ises(IsADirector
-000297c0: 7945 7272 6f72 2920 6173 2063 6d3a 0a20  yError) as cm:. 
-000297d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000297e0: 6673 2e6f 7065 6e28 272f 6469 7231 2729  fs.open('/dir1')
-000297f0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00029800: 7365 7274 4571 7561 6c28 636d 2e65 7863  sertEqual(cm.exc
-00029810: 6570 7469 6f6e 2e61 7267 735b 305d 2c20  eption.args[0], 
-00029820: 272f 6469 7231 2729 0a0a 2020 2020 6465  '/dir1')..    de
-00029830: 6620 7465 7374 5f64 656c 6574 655f 6669  f test_delete_fi
-00029840: 6c65 2873 656c 6629 3a0a 2020 2020 2020  le(self):.      
-00029850: 2020 7365 6c66 2e66 732e 6372 6561 7465    self.fs.create
-00029860: 5f66 696c 6528 272f 7465 7374 272c 2022  _file('/test', "
-00029870: 666f 6f22 290a 2020 2020 2020 2020 7365  foo").        se
-00029880: 6c66 2e66 732e 6465 6c65 7465 5f70 6174  lf.fs.delete_pat
-00029890: 6828 272f 7465 7374 2729 0a20 2020 2020  h('/test').     
-000298a0: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
-000298b0: 6572 7452 6169 7365 7328 4669 6c65 4e6f  ertRaises(FileNo
-000298c0: 7446 6f75 6e64 4572 726f 7229 2061 7320  tFoundError) as 
-000298d0: 636d 3a0a 2020 2020 2020 2020 2020 2020  cm:.            
-000298e0: 7365 6c66 2e66 732e 6765 745f 7061 7468  self.fs.get_path
-000298f0: 2827 2f74 6573 7427 290a 0a20 2020 2020  ('/test')..     
-00029900: 2020 2023 2044 656c 6574 696e 6720 6465     # Deleting de
-00029910: 6c65 7465 6420 6669 6c65 7320 7368 6f75  leted files shou
-00029920: 6c64 2066 6169 6c20 6173 2077 656c 6c0a  ld fail as well.
-00029930: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00029940: 662e 6173 7365 7274 5261 6973 6573 2846  f.assertRaises(F
-00029950: 696c 654e 6f74 466f 756e 6445 7272 6f72  ileNotFoundError
-00029960: 2920 6173 2063 6d3a 0a20 2020 2020 2020  ) as cm:.       
-00029970: 2020 2020 2073 656c 662e 6673 2e64 656c       self.fs.del
-00029980: 6574 655f 7061 7468 2827 2f74 6573 7427  ete_path('/test'
-00029990: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-000299a0: 7373 6572 7454 7275 6528 272f 7465 7374  ssertTrue('/test
-000299b0: 2720 696e 2063 6d2e 6578 6365 7074 696f  ' in cm.exceptio
-000299c0: 6e2e 6172 6773 5b30 5d29 0a0a 2020 2020  n.args[0])..    
-000299d0: 6465 6620 7465 7374 5f63 7265 6174 655f  def test_create_
-000299e0: 6469 725f 7769 7468 5f65 7874 7261 5f61  dir_with_extra_a
-000299f0: 7267 7328 7365 6c66 293a 0a20 2020 2020  rgs(self):.     
-00029a00: 2020 2064 203d 2073 656c 662e 6673 2e63     d = self.fs.c
-00029a10: 7265 6174 655f 6469 7228 272f 6469 7231  reate_dir('/dir1
-00029a20: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-00029a30: 6173 7365 7274 4571 7561 6c28 642e 6b77  assertEqual(d.kw
-00029a40: 6172 6773 2c20 7b7d 290a 0a20 2020 2020  args, {})..     
-00029a50: 2020 2064 203d 2073 656c 662e 6673 2e63     d = self.fs.c
-00029a60: 7265 6174 655f 6469 7228 0a20 2020 2020  reate_dir(.     
-00029a70: 2020 2020 2020 2027 2f64 6972 3227 2c20         '/dir2', 
-00029a80: 7065 726d 6973 7369 6f6e 733d 306f 3730  permissions=0o70
-00029a90: 302c 2075 7365 723d 2775 6275 6e74 7527  0, user='ubuntu'
-00029aa0: 2c20 7573 6572 5f69 643d 3130 3030 2c20  , user_id=1000, 
-00029ab0: 6772 6f75 703d 2777 7777 2d64 6174 6127  group='www-data'
-00029ac0: 2c20 6772 6f75 705f 6964 3d33 3329 0a20  , group_id=33). 
-00029ad0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00029ae0: 7274 4571 7561 6c28 642e 6b77 6172 6773  rtEqual(d.kwargs
-00029af0: 2c20 7b0a 2020 2020 2020 2020 2020 2020  , {.            
-00029b00: 2770 6572 6d69 7373 696f 6e73 273a 2030  'permissions': 0
-00029b10: 6f37 3030 2c0a 2020 2020 2020 2020 2020  o700,.          
-00029b20: 2020 2775 7365 7227 3a20 2775 6275 6e74    'user': 'ubunt
-00029b30: 7527 2c0a 2020 2020 2020 2020 2020 2020  u',.            
-00029b40: 2775 7365 725f 6964 273a 2031 3030 302c  'user_id': 1000,
-00029b50: 0a20 2020 2020 2020 2020 2020 2027 6772  .            'gr
-00029b60: 6f75 7027 3a20 2777 7777 2d64 6174 6127  oup': 'www-data'
-00029b70: 2c0a 2020 2020 2020 2020 2020 2020 2767  ,.            'g
-00029b80: 726f 7570 5f69 6427 3a20 3333 2c0a 2020  roup_id': 33,.  
-00029b90: 2020 2020 2020 7d29 0a0a 2020 2020 6465        })..    de
-00029ba0: 6620 7465 7374 5f63 7265 6174 655f 6669  f test_create_fi
-00029bb0: 6c65 5f77 6974 685f 6578 7472 615f 6172  le_with_extra_ar
-00029bc0: 6773 2873 656c 6629 3a0a 2020 2020 2020  gs(self):.      
-00029bd0: 2020 6620 3d20 7365 6c66 2e66 732e 6372    f = self.fs.cr
-00029be0: 6561 7465 5f66 696c 6528 272f 6669 6c65  eate_file('/file
-00029bf0: 3127 2c20 2764 6174 6127 290a 2020 2020  1', 'data').    
-00029c00: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00029c10: 7175 616c 2866 2e6b 7761 7267 732c 207b  qual(f.kwargs, {
-00029c20: 7d29 0a0a 2020 2020 2020 2020 6620 3d20  })..        f = 
-00029c30: 7365 6c66 2e66 732e 6372 6561 7465 5f66  self.fs.create_f
-00029c40: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
-00029c50: 2027 2f66 696c 6532 272c 2027 6461 7461   '/file2', 'data
-00029c60: 272c 0a20 2020 2020 2020 2020 2020 2070  ',.            p
-00029c70: 6572 6d69 7373 696f 6e73 3d30 6f37 3534  ermissions=0o754
-00029c80: 2c20 7573 6572 3d27 7562 756e 7475 272c  , user='ubuntu',
-00029c90: 2075 7365 725f 6964 3d31 3030 302c 2067   user_id=1000, g
-00029ca0: 726f 7570 3d27 7777 772d 6461 7461 272c  roup='www-data',
-00029cb0: 2067 726f 7570 5f69 643d 3333 290a 2020   group_id=33).  
-00029cc0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00029cd0: 7445 7175 616c 2866 2e6b 7761 7267 732c  tEqual(f.kwargs,
-00029ce0: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
-00029cf0: 7065 726d 6973 7369 6f6e 7327 3a20 306f  permissions': 0o
-00029d00: 3735 342c 0a20 2020 2020 2020 2020 2020  754,.           
-00029d10: 2027 7573 6572 273a 2027 7562 756e 7475   'user': 'ubuntu
-00029d20: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
-00029d30: 7573 6572 5f69 6427 3a20 3130 3030 2c0a  user_id': 1000,.
-00029d40: 2020 2020 2020 2020 2020 2020 2767 726f              'gro
-00029d50: 7570 273a 2027 7777 772d 6461 7461 272c  up': 'www-data',
-00029d60: 0a20 2020 2020 2020 2020 2020 2027 6772  .            'gr
-00029d70: 6f75 705f 6964 273a 2033 332c 0a20 2020  oup_id': 33,.   
-00029d80: 2020 2020 207d 290a 0a20 2020 2064 6566       })..    def
-00029d90: 2074 6573 745f 6765 7461 7474 7228 7365   test_getattr(se
-00029da0: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-00029db0: 662e 6673 2e63 7265 6174 655f 6469 7228  f.fs.create_dir(
-00029dc0: 272f 6574 632f 696e 6974 2e64 272c 206d  '/etc/init.d', m
-00029dd0: 616b 655f 7061 7265 6e74 733d 5472 7565  ake_parents=True
-00029de0: 290a 0a20 2020 2020 2020 2023 2042 7920  )..        # By 
-00029df0: 7061 7468 0a20 2020 2020 2020 206f 203d  path.        o =
-00029e00: 2073 656c 662e 6673 2e67 6574 5f70 6174   self.fs.get_pat
-00029e10: 6828 7061 7468 6c69 622e 5075 7265 506f  h(pathlib.PurePo
-00029e20: 7369 7850 6174 6828 272f 6574 632f 696e  sixPath('/etc/in
-00029e30: 6974 2e64 2729 290a 2020 2020 2020 2020  it.d')).        
-00029e40: 7365 6c66 2e61 7373 6572 7449 7349 6e73  self.assertIsIns
-00029e50: 7461 6e63 6528 6f2c 205f 4469 7265 6374  tance(o, _Direct
-00029e60: 6f72 7929 0a20 2020 2020 2020 2073 656c  ory).        sel
-00029e70: 662e 6173 7365 7274 4571 7561 6c28 6f2e  f.assertEqual(o.
-00029e80: 7061 7468 2c20 7061 7468 6c69 622e 5075  path, pathlib.Pu
-00029e90: 7265 506f 7369 7850 6174 6828 272f 6574  rePosixPath('/et
-00029ea0: 632f 696e 6974 2e64 2729 290a 0a20 2020  c/init.d'))..   
-00029eb0: 2020 2020 2023 2042 7920 7374 720a 2020       # By str.  
-00029ec0: 2020 2020 2020 6f20 3d20 7365 6c66 2e66        o = self.f
-00029ed0: 732e 6765 745f 7061 7468 2827 2f65 7463  s.get_path('/etc
-00029ee0: 2f69 6e69 742e 6427 290a 2020 2020 2020  /init.d').      
-00029ef0: 2020 7365 6c66 2e61 7373 6572 7449 7349    self.assertIsI
-00029f00: 6e73 7461 6e63 6528 6f2c 205f 4469 7265  nstance(o, _Dire
-00029f10: 6374 6f72 7929 0a20 2020 2020 2020 2073  ctory).        s
-00029f20: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00029f30: 6f2e 7061 7468 2c20 7061 7468 6c69 622e  o.path, pathlib.
-00029f40: 5075 7265 506f 7369 7850 6174 6828 272f  PurePosixPath('/
-00029f50: 6574 632f 696e 6974 2e64 2729 290a 0a20  etc/init.d')).. 
-00029f60: 2020 2064 6566 2074 6573 745f 6765 7461     def test_geta
-00029f70: 7474 725f 6669 6c65 5f6e 6f74 5f66 6f75  ttr_file_not_fou
-00029f80: 6e64 2873 656c 6629 3a0a 2020 2020 2020  nd(self):.      
-00029f90: 2020 2320 4172 6775 6162 6c79 2074 6869    # Arguably thi
-00029fa0: 7320 636f 756c 6420 6265 2061 204b 6579  s could be a Key
-00029fb0: 4572 726f 7220 6769 7665 6e20 7468 6520  Error given the 
-00029fc0: 6469 6374 696f 6e61 7279 2d73 7479 6c65  dictionary-style
-00029fd0: 2061 6363 6573 732e 0a20 2020 2020 2020   access..       
-00029fe0: 2023 2048 6f77 6576 6572 2c20 4669 6c65   # However, File
-00029ff0: 4e6f 7446 6f75 6e64 4572 726f 7220 7365  NotFoundError se
-0002a000: 656d 7320 6d6f 7265 2061 7070 726f 7072  ems more appropr
-0002a010: 6961 7465 2066 6f72 2061 2066 696c 6573  iate for a files
-0002a020: 7973 7465 6d2c 2061 6e64 2069 740a 2020  ystem, and it.  
-0002a030: 2020 2020 2020 2320 6769 7665 7320 6120        # gives a 
-0002a040: 636c 6f73 6572 2073 656d 616e 7469 6320  closer semantic 
-0002a050: 6665 656c 696e 672c 2069 6e20 6d79 206f  feeling, in my o
-0002a060: 7069 6e69 6f6e 2e0a 2020 2020 2020 2020  pinion..        
-0002a070: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
-0002a080: 5261 6973 6573 2846 696c 654e 6f74 466f  Raises(FileNotFo
-0002a090: 756e 6445 7272 6f72 2920 6173 2063 6d3a  undError) as cm:
-0002a0a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0002a0b0: 662e 6673 2e67 6574 5f70 6174 6828 272f  f.fs.get_path('/
-0002a0c0: 6e6f 6e65 7869 7374 656e 745f 6669 6c65  nonexistent_file
-0002a0d0: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-0002a0e0: 6173 7365 7274 5472 7565 2827 2f6e 6f6e  assertTrue('/non
-0002a0f0: 6578 6973 7465 6e74 5f66 696c 6527 2069  existent_file' i
-0002a100: 6e20 636d 2e65 7863 6570 7469 6f6e 2e61  n cm.exception.a
-0002a110: 7267 735b 305d 290a 0a0a 636c 6173 7320  rgs[0])...class 
-0002a120: 5465 7374 5465 7374 696e 6746 696c 6573  TestTestingFiles
-0002a130: 7973 7465 6d28 4765 6e65 7269 6354 6573  ystem(GenericTes
-0002a140: 7469 6e67 4669 6c65 7379 7374 656d 5465  tingFilesystemTe
-0002a150: 7374 732c 2075 6e69 7474 6573 742e 5465  sts, unittest.Te
-0002a160: 7374 4361 7365 293a 0a20 2020 2064 6566  stCase):.    def
-0002a170: 2073 6574 5570 2873 656c 6629 3a0a 2020   setUp(self):.  
-0002a180: 2020 2020 2020 7365 6c66 2e66 7320 3d20        self.fs = 
-0002a190: 5f54 6573 7469 6e67 4669 6c65 7379 7374  _TestingFilesyst
-0002a1a0: 656d 2829 0a0a 2020 2020 6465 6620 7465  em()..    def te
-0002a1b0: 7374 5f73 746f 7261 6765 5f6d 6f75 6e74  st_storage_mount
-0002a1c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0002a1d0: 746d 7064 6972 203d 2074 656d 7066 696c  tmpdir = tempfil
-0002a1e0: 652e 5465 6d70 6f72 6172 7944 6972 6563  e.TemporaryDirec
-0002a1f0: 746f 7279 2829 0a20 2020 2020 2020 2073  tory().        s
-0002a200: 656c 662e 6673 2e61 6464 5f6d 6f75 6e74  elf.fs.add_mount
-0002a210: 2827 666f 6f27 2c20 272f 666f 6f27 2c20  ('foo', '/foo', 
-0002a220: 746d 7064 6972 2e6e 616d 6529 0a20 2020  tmpdir.name).   
-0002a230: 2020 2020 2073 656c 662e 6673 2e63 7265       self.fs.cre
-0002a240: 6174 655f 6669 6c65 2827 2f66 6f6f 2f62  ate_file('/foo/b
-0002a250: 6172 2f62 617a 2e74 7874 272c 2027 7175  ar/baz.txt', 'qu
-0002a260: 7578 272c 206d 616b 655f 6469 7273 3d54  ux', make_dirs=T
-0002a270: 7275 6529 0a0a 2020 2020 2020 2020 746d  rue)..        tm
-0002a280: 7070 6174 6820 3d20 6f73 2e70 6174 682e  ppath = os.path.
-0002a290: 6a6f 696e 2874 6d70 6469 722e 6e61 6d65  join(tmpdir.name
-0002a2a0: 2c20 2762 6172 2f62 617a 2e74 7874 2729  , 'bar/baz.txt')
-0002a2b0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0002a2c0: 7365 7274 5472 7565 286f 732e 7061 7468  sertTrue(os.path
-0002a2d0: 2e65 7869 7374 7328 746d 7070 6174 6829  .exists(tmppath)
-0002a2e0: 290a 2020 2020 2020 2020 7769 7468 206f  ).        with o
-0002a2f0: 7065 6e28 746d 7070 6174 6829 2061 7320  pen(tmppath) as 
-0002a300: 663a 0a20 2020 2020 2020 2020 2020 2073  f:.            s
-0002a310: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0002a320: 662e 7265 6164 2829 2c20 2771 7575 7827  f.read(), 'quux'
-0002a330: 290a 0a0a 636c 6173 7320 5465 7374 5465  )...class TestTe
-0002a340: 7374 696e 6753 746f 7261 6765 4d6f 756e  stingStorageMoun
-0002a350: 7428 4765 6e65 7269 6354 6573 7469 6e67  t(GenericTesting
-0002a360: 4669 6c65 7379 7374 656d 5465 7374 732c  FilesystemTests,
-0002a370: 2075 6e69 7474 6573 742e 5465 7374 4361   unittest.TestCa
-0002a380: 7365 293a 0a20 2020 2064 6566 2073 6574  se):.    def set
-0002a390: 5570 2873 656c 6629 3a0a 2020 2020 2020  Up(self):.      
-0002a3a0: 2020 7365 6c66 2e74 6d70 203d 2074 656d    self.tmp = tem
-0002a3b0: 7066 696c 652e 5465 6d70 6f72 6172 7944  pfile.TemporaryD
-0002a3c0: 6972 6563 746f 7279 2829 0a20 2020 2020  irectory().     
-0002a3d0: 2020 2073 656c 662e 6164 6443 6c65 616e     self.addClean
-0002a3e0: 7570 2873 656c 662e 746d 702e 636c 6561  up(self.tmp.clea
-0002a3f0: 6e75 7029 0a20 2020 2020 2020 2073 656c  nup).        sel
-0002a400: 662e 6673 203d 205f 5465 7374 696e 6753  f.fs = _TestingS
-0002a410: 746f 7261 6765 4d6f 756e 7428 272f 272c  torageMount('/',
-0002a420: 2070 6174 686c 6962 2e50 6174 6828 7365   pathlib.Path(se
-0002a430: 6c66 2e74 6d70 2e6e 616d 6529 290a 0a0a  lf.tmp.name))...
-0002a440: 636c 6173 7320 5465 7374 5065 6262 6c65  class TestPebble
-0002a450: 5374 6f72 6167 6541 5049 7355 7369 6e67  StorageAPIsUsing
-0002a460: 4d6f 636b 7328 0a20 2020 2020 2020 2075  Mocks(.        u
-0002a470: 6e69 7474 6573 742e 5465 7374 4361 7365  nittest.TestCase
-0002a480: 2c0a 2020 2020 2020 2020 5f54 6573 7469  ,.        _Testi
-0002a490: 6e67 5065 6262 6c65 436c 6965 6e74 4d69  ngPebbleClientMi
-0002a4a0: 7869 6e2c 0a20 2020 2020 2020 205f 5065  xin,.        _Pe
-0002a4b0: 6262 6c65 5374 6f72 6167 6541 5049 7354  bbleStorageAPIsT
-0002a4c0: 6573 744d 6978 696e 293a 0a20 2020 2064  estMixin):.    d
-0002a4d0: 6566 2073 6574 5570 2873 656c 6629 3a0a  ef setUp(self):.
-0002a4e0: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
-0002a4f0: 6669 7820 3d20 272f 7072 6566 6978 270a  fix = '/prefix'.
-0002a500: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
-0002a510: 656e 7420 3d20 7365 6c66 2e67 6574 5f74  ent = self.get_t
-0002a520: 6573 7469 6e67 5f63 6c69 656e 7428 290a  esting_client().
-0002a530: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0002a540: 7072 6566 6978 3a0a 2020 2020 2020 2020  prefix:.        
-0002a550: 2020 2020 7365 6c66 2e63 6c69 656e 742e      self.client.
-0002a560: 6d61 6b65 5f64 6972 2873 656c 662e 7072  make_dir(self.pr
-0002a570: 6566 6978 2c20 6d61 6b65 5f70 6172 656e  efix, make_paren
-0002a580: 7473 3d54 7275 6529 0a0a 2020 2020 4075  ts=True)..    @u
-0002a590: 6e69 7474 6573 742e 736b 6970 556e 6c65  nittest.skipUnle
-0002a5a0: 7373 2869 735f 6c69 6e75 782c 2027 5065  ss(is_linux, 'Pe
-0002a5b0: 6262 6c65 2072 756e 7320 6f6e 204c 696e  bble runs on Lin
-0002a5c0: 7578 2729 0a20 2020 2064 6566 2074 6573  ux').    def tes
-0002a5d0: 745f 636f 6e74 6169 6e65 725f 7374 6f72  t_container_stor
-0002a5e0: 6167 655f 6d6f 756e 7473 2873 656c 6629  age_mounts(self)
-0002a5f0: 3a0a 2020 2020 2020 2020 6861 726e 6573  :.        harnes
-0002a600: 7320 3d20 6f70 732e 7465 7374 696e 672e  s = ops.testing.
-0002a610: 4861 726e 6573 7328 6f70 732e 4368 6172  Harness(ops.Char
-0002a620: 6d42 6173 652c 206d 6574 613d 2727 270a  mBase, meta='''.
-0002a630: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-0002a640: 3a20 7465 7374 2d61 7070 0a20 2020 2020  : test-app.     
-0002a650: 2020 2020 2020 2063 6f6e 7461 696e 6572         container
-0002a660: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0002a670: 2020 2063 313a 0a20 2020 2020 2020 2020     c1:.         
-0002a680: 2020 2020 2020 2020 2020 206d 6f75 6e74             mount
-0002a690: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0002a6a0: 2020 2020 2020 2020 2020 202d 2073 746f             - sto
-0002a6b0: 7261 6765 3a20 7374 6f72 6531 0a20 2020  rage: store1.   
-0002a6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a6d0: 2020 2020 2020 206c 6f63 6174 696f 6e3a         location:
-0002a6e0: 202f 6d6f 756e 7473 2f66 6f6f 0a20 2020   /mounts/foo.   
-0002a6f0: 2020 2020 2020 2020 2020 2020 2063 323a               c2:
-0002a700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002a710: 2020 2020 206d 6f75 6e74 733a 0a20 2020       mounts:.   
-0002a720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a730: 2020 2020 202d 2073 746f 7261 6765 3a20       - storage: 
-0002a740: 7374 6f72 6532 0a20 2020 2020 2020 2020  store2.         
-0002a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a760: 206c 6f63 6174 696f 6e3a 202f 6d6f 756e   location: /moun
-0002a770: 7473 2f66 6f6f 0a20 2020 2020 2020 2020  ts/foo.         
-0002a780: 2020 2020 2020 2063 333a 0a20 2020 2020         c3:.     
-0002a790: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0002a7a0: 6f75 6e74 733a 0a20 2020 2020 2020 2020  ounts:.         
-0002a7b0: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-0002a7c0: 2073 746f 7261 6765 3a20 7374 6f72 6531   storage: store1
-0002a7d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002a7e0: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
-0002a7f0: 696f 6e3a 202f 6d6f 756e 7473 2f62 6172  ion: /mounts/bar
-0002a800: 0a20 2020 2020 2020 2020 2020 2073 746f  .            sto
-0002a810: 7261 6765 3a0a 2020 2020 2020 2020 2020  rage:.          
-0002a820: 2020 2020 2020 7374 6f72 6531 3a0a 2020        store1:.  
-0002a830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a840: 2020 7479 7065 3a20 6669 6c65 7379 7374    type: filesyst
-0002a850: 656d 0a20 2020 2020 2020 2020 2020 2020  em.             
-0002a860: 2020 2073 746f 7265 323a 0a20 2020 2020     store2:.     
-0002a870: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0002a880: 7970 653a 2066 696c 6573 7973 7465 6d0a  ype: filesystem.
-0002a890: 2020 2020 2020 2020 2020 2020 2727 2729              ''')
-0002a8a0: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
-0002a8b0: 6443 6c65 616e 7570 2868 6172 6e65 7373  dCleanup(harness
-0002a8c0: 2e63 6c65 616e 7570 290a 0a20 2020 2020  .cleanup)..     
-0002a8d0: 2020 2073 746f 7265 5f69 6420 3d20 6861     store_id = ha
-0002a8e0: 726e 6573 732e 6164 645f 7374 6f72 6167  rness.add_storag
-0002a8f0: 6528 2773 746f 7265 3127 295b 305d 0a20  e('store1')[0]. 
-0002a900: 2020 2020 2020 2068 6172 6e65 7373 2e61         harness.a
-0002a910: 7474 6163 685f 7374 6f72 6167 6528 7374  ttach_storage(st
-0002a920: 6f72 655f 6964 290a 0a20 2020 2020 2020  ore_id)..       
-0002a930: 2068 6172 6e65 7373 2e62 6567 696e 2829   harness.begin()
+00025120: 5349 4749 4e54 222c 2028 2266 6f6f 222c  SIGINT", ("foo",
+00025130: 2929 0a0a 2020 2020 2020 2020 2320 5365  ))..        # Se
+00025140: 6e64 2061 2076 616c 6964 2073 6967 6e61  nd a valid signa
+00025150: 6c20 6275 7420 6f6d 6974 2073 6572 7669  l but omit servi
+00025160: 6365 206e 616d 650a 2020 2020 2020 2020  ce name.        
+00025170: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
+00025180: 5261 6973 6573 2854 7970 6545 7272 6f72  Raises(TypeError
+00025190: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+000251a0: 6c69 656e 742e 7365 6e64 5f73 6967 6e61  lient.send_signa
+000251b0: 6c28 2253 4947 494e 5422 2c20 7475 706c  l("SIGINT", tupl
+000251c0: 6528 2929 0a0a 2020 2020 2020 2020 2320  e())..        # 
+000251d0: 5365 6e64 2061 6e20 696e 7661 6c69 6420  Send an invalid 
+000251e0: 7369 676e 616c 2074 6f20 6120 7275 6e6e  signal to a runn
+000251f0: 696e 6720 7365 7276 6963 650a 2020 2020  ing service.    
+00025200: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
+00025210: 7365 7274 5261 6973 6573 2870 6562 626c  sertRaises(pebbl
+00025220: 652e 4150 4945 7272 6f72 293a 0a20 2020  e.APIError):.   
+00025230: 2020 2020 2020 2020 2063 6c69 656e 742e           client.
+00025240: 7365 6e64 5f73 6967 6e61 6c28 2273 6967  send_signal("sig
+00025250: 696e 7422 2c20 2822 666f 6f22 2c29 290a  int", ("foo",)).
+00025260: 0a20 2020 2020 2020 2023 2053 656e 6420  .        # Send 
+00025270: 6120 7661 6c69 6420 7369 676e 616c 2074  a valid signal t
+00025280: 6f20 6120 7374 6f70 7065 6420 7365 7276  o a stopped serv
+00025290: 6963 650a 2020 2020 2020 2020 7769 7468  ice.        with
+000252a0: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
+000252b0: 6573 2870 6562 626c 652e 4150 4945 7272  es(pebble.APIErr
+000252c0: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+000252d0: 2063 6c69 656e 742e 7365 6e64 5f73 6967   client.send_sig
+000252e0: 6e61 6c28 2253 4947 494e 5422 2c20 2822  nal("SIGINT", ("
+000252f0: 6261 7222 2c29 290a 0a20 2020 2020 2020  bar",))..       
+00025300: 2023 2053 656e 6420 6120 7661 6c69 6420   # Send a valid 
+00025310: 7369 676e 616c 2074 6f20 6120 6e6f 6e2d  signal to a non-
+00025320: 6578 6973 7469 6e67 2073 6572 7669 6365  existing service
+00025330: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+00025340: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
+00025350: 7065 6262 6c65 2e41 5049 4572 726f 7229  pebble.APIError)
+00025360: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
+00025370: 6965 6e74 2e73 656e 645f 7369 676e 616c  ient.send_signal
+00025380: 2822 5349 4749 4e54 222c 2028 2262 617a  ("SIGINT", ("baz
+00025390: 222c 2929 0a0a 2020 2020 2020 2020 2320  ",))..        # 
+000253a0: 5365 6e64 2061 2076 616c 6964 2073 6967  Send a valid sig
+000253b0: 6e61 6c20 746f 2061 206d 756c 7469 706c  nal to a multipl
+000253c0: 6520 7365 7276 6963 6573 2c20 6f6e 6520  e services, one 
+000253d0: 6f66 2077 6869 6368 2069 7320 6e6f 7420  of which is not 
+000253e0: 7275 6e6e 696e 670a 2020 2020 2020 2020  running.        
+000253f0: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
+00025400: 5261 6973 6573 2870 6562 626c 652e 4150  Raises(pebble.AP
+00025410: 4945 7272 6f72 293a 0a20 2020 2020 2020  IError):.       
+00025420: 2020 2020 2063 6c69 656e 742e 7365 6e64       client.send
+00025430: 5f73 6967 6e61 6c28 2253 4947 494e 5422  _signal("SIGINT"
+00025440: 2c20 2822 666f 6f22 2c20 2262 6172 222c  , ("foo", "bar",
+00025450: 2929 0a0a 0a23 2046 6f72 2074 6573 7469  ))...# For testi
+00025460: 6e67 2066 696c 652d 6f70 7320 6f66 2074  ng file-ops of t
+00025470: 6865 2070 6562 626c 6520 636c 6965 6e74  he pebble client
+00025480: 2e20 2054 6869 7320 6973 2072 6566 6163  .  This is refac
+00025490: 746f 7265 6420 696e 746f 2061 0a23 2073  tored into a.# s
+000254a0: 6570 6172 6174 6520 6d69 7869 6e20 736f  eparate mixin so
+000254b0: 2077 6520 6361 6e20 7275 6e20 7468 6573   we can run thes
+000254c0: 6520 7465 7374 7320 6167 6169 6e73 7420  e tests against 
+000254d0: 626f 7468 2074 6865 206d 6f63 6b20 636c  both the mock cl
+000254e0: 6965 6e74 2061 730a 2320 7765 6c6c 2061  ient as.# well a
+000254f0: 7320 6120 7265 616c 2070 6562 626c 6520  s a real pebble 
+00025500: 7365 7276 6572 2069 6e73 7461 6e63 652e  server instance.
+00025510: 0a63 6c61 7373 205f 5065 6262 6c65 5374  .class _PebbleSt
+00025520: 6f72 6167 6541 5049 7354 6573 744d 6978  orageAPIsTestMix
+00025530: 696e 3a0a 2020 2020 2320 4f76 6572 7269  in:.    # Overri
+00025540: 6465 2074 6869 7320 696e 2063 6c61 7373  de this in class
+00025550: 6573 2075 7369 6e67 2074 6869 7320 6d69  es using this mi
+00025560: 7869 6e2e 0a20 2020 2023 2054 6869 7320  xin..    # This 
+00025570: 7368 6f75 6c64 2062 6520 7365 7420 746f  should be set to
+00025580: 2061 6e79 206e 6f6e 2d65 6d70 7479 2070   any non-empty p
+00025590: 6174 682c 2062 7574 2077 6974 686f 7574  ath, but without
+000255a0: 2061 2074 7261 696c 696e 6720 2f2e 0a20   a trailing /.. 
+000255b0: 2020 2070 7265 6669 7820 3d20 4e6f 6e65     prefix = None
+000255c0: 0a0a 2020 2020 6465 6620 7465 7374 5f70  ..    def test_p
+000255d0: 7573 685f 616e 645f 7075 6c6c 5f62 7974  ush_and_pull_byt
+000255e0: 6573 2873 656c 6629 3a0a 2020 2020 2020  es(self):.      
+000255f0: 2020 7365 6c66 2e5f 7465 7374 5f70 7573    self._test_pus
+00025600: 685f 616e 645f 7075 6c6c 5f64 6174 6128  h_and_pull_data(
+00025610: 0a20 2020 2020 2020 2020 2020 206f 7269  .            ori
+00025620: 6769 6e61 6c5f 6461 7461 3d62 225c 7830  ginal_data=b"\x0
+00025630: 305c 7830 315c 7830 325c 7830 335c 7830  0\x01\x02\x03\x0
+00025640: 3422 2c0a 2020 2020 2020 2020 2020 2020  4",.            
+00025650: 656e 636f 6469 6e67 3d4e 6f6e 652c 0a20  encoding=None,. 
+00025660: 2020 2020 2020 2020 2020 2073 7472 6561             strea
+00025670: 6d5f 636c 6173 733d 696f 2e42 7974 6573  m_class=io.Bytes
+00025680: 494f 290a 0a20 2020 2064 6566 2074 6573  IO)..    def tes
+00025690: 745f 7075 7368 5f61 6e64 5f70 756c 6c5f  t_push_and_pull_
+000256a0: 6e6f 6e5f 7574 6638 5f64 6174 6128 7365  non_utf8_data(se
+000256b0: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+000256c0: 662e 5f74 6573 745f 7075 7368 5f61 6e64  f._test_push_and
+000256d0: 5f70 756c 6c5f 6461 7461 280a 2020 2020  _pull_data(.    
+000256e0: 2020 2020 2020 2020 6f72 6967 696e 616c          original
+000256f0: 5f64 6174 613d 27e6 97a5 e69c ace8 aa9e  _data='.........
+00025700: 272c 2020 2320 224a 6170 616e 6573 6522  ',  # "Japanese"
+00025710: 2069 6e20 4a61 7061 6e65 7365 0a20 2020   in Japanese.   
+00025720: 2020 2020 2020 2020 2065 6e63 6f64 696e           encodin
+00025730: 673d 2773 6a69 7327 2c0a 2020 2020 2020  g='sjis',.      
+00025740: 2020 2020 2020 7374 7265 616d 5f63 6c61        stream_cla
+00025750: 7373 3d69 6f2e 5374 7269 6e67 494f 290a  ss=io.StringIO).
+00025760: 0a20 2020 2064 6566 205f 7465 7374 5f70  .    def _test_p
+00025770: 7573 685f 616e 645f 7075 6c6c 5f64 6174  ush_and_pull_dat
+00025780: 6128 7365 6c66 2c20 6f72 6967 696e 616c  a(self, original
+00025790: 5f64 6174 612c 2065 6e63 6f64 696e 672c  _data, encoding,
+000257a0: 2073 7472 6561 6d5f 636c 6173 7329 3a0a   stream_class):.
+000257b0: 2020 2020 2020 2020 636c 6965 6e74 203d          client =
+000257c0: 2073 656c 662e 636c 6965 6e74 0a20 2020   self.client.   
+000257d0: 2020 2020 2063 6c69 656e 742e 7075 7368       client.push
+000257e0: 2866 227b 7365 6c66 2e70 7265 6669 787d  (f"{self.prefix}
+000257f0: 2f74 6573 7422 2c20 6f72 6967 696e 616c  /test", original
+00025800: 5f64 6174 612c 2065 6e63 6f64 696e 673d  _data, encoding=
+00025810: 656e 636f 6469 6e67 290a 2020 2020 2020  encoding).      
+00025820: 2020 7769 7468 2063 6c69 656e 742e 7075    with client.pu
+00025830: 6c6c 2866 227b 7365 6c66 2e70 7265 6669  ll(f"{self.prefi
+00025840: 787d 2f74 6573 7422 2c20 656e 636f 6469  x}/test", encodi
+00025850: 6e67 3d65 6e63 6f64 696e 6729 2061 7320  ng=encoding) as 
+00025860: 696e 6669 6c65 3a0a 2020 2020 2020 2020  infile:.        
+00025870: 2020 2020 7265 6365 6976 6564 5f64 6174      received_dat
+00025880: 6120 3d20 696e 6669 6c65 2e72 6561 6428  a = infile.read(
+00025890: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+000258a0: 7373 6572 7445 7175 616c 286f 7269 6769  ssertEqual(origi
+000258b0: 6e61 6c5f 6461 7461 2c20 7265 6365 6976  nal_data, receiv
+000258c0: 6564 5f64 6174 6129 0a0a 2020 2020 2020  ed_data)..      
+000258d0: 2020 2320 5765 2061 6c73 6f20 7375 7070    # We also supp
+000258e0: 6f72 7420 6669 6c65 2d6c 696b 6520 6f62  ort file-like ob
+000258f0: 6a65 6374 7320 6173 2069 6e70 7574 2c20  jects as input, 
+00025900: 736f 206c 6574 2773 2074 6573 7420 7468  so let's test th
+00025910: 6174 2063 6173 6520 6173 2077 656c 6c2e  at case as well.
+00025920: 0a20 2020 2020 2020 2073 6d61 6c6c 5f66  .        small_f
+00025930: 696c 6520 3d20 7374 7265 616d 5f63 6c61  ile = stream_cla
+00025940: 7373 286f 7269 6769 6e61 6c5f 6461 7461  ss(original_data
+00025950: 290a 2020 2020 2020 2020 636c 6965 6e74  ).        client
+00025960: 2e70 7573 6828 6622 7b73 656c 662e 7072  .push(f"{self.pr
+00025970: 6566 6978 7d2f 7465 7374 222c 2073 6d61  efix}/test", sma
+00025980: 6c6c 5f66 696c 652c 2065 6e63 6f64 696e  ll_file, encodin
+00025990: 673d 656e 636f 6469 6e67 290a 2020 2020  g=encoding).    
+000259a0: 2020 2020 7769 7468 2063 6c69 656e 742e      with client.
+000259b0: 7075 6c6c 2866 227b 7365 6c66 2e70 7265  pull(f"{self.pre
+000259c0: 6669 787d 2f74 6573 7422 2c20 656e 636f  fix}/test", enco
+000259d0: 6469 6e67 3d65 6e63 6f64 696e 6729 2061  ding=encoding) a
+000259e0: 7320 696e 6669 6c65 3a0a 2020 2020 2020  s infile:.      
+000259f0: 2020 2020 2020 7265 6365 6976 6564 5f64        received_d
+00025a00: 6174 6120 3d20 696e 6669 6c65 2e72 6561  ata = infile.rea
+00025a10: 6428 290a 2020 2020 2020 2020 7365 6c66  d().        self
+00025a20: 2e61 7373 6572 7445 7175 616c 286f 7269  .assertEqual(ori
+00025a30: 6769 6e61 6c5f 6461 7461 2c20 7265 6365  ginal_data, rece
+00025a40: 6976 6564 5f64 6174 6129 0a0a 2020 2020  ived_data)..    
+00025a50: 6465 6620 7465 7374 5f70 7573 685f 616e  def test_push_an
+00025a60: 645f 7075 6c6c 5f6c 6172 6765 725f 6669  d_pull_larger_fi
+00025a70: 6c65 2873 656c 6629 3a0a 2020 2020 2020  le(self):.      
+00025a80: 2020 2320 496e 7465 6e74 3a20 746f 2065    # Intent: to e
+00025a90: 6e73 7572 6520 7468 696e 6773 2077 6f72  nsure things wor
+00025aa0: 6b20 6170 7072 6f70 7269 6174 656c 7920  k appropriately 
+00025ab0: 7769 7468 206c 6172 6765 7220 6669 6c65  with larger file
+00025ac0: 732e 0a20 2020 2020 2020 2023 204c 6172  s..        # Lar
+00025ad0: 6765 7220 6669 6c65 7320 6d61 7920 6265  ger files may be
+00025ae0: 2073 656e 742f 7265 6365 6976 6564 2069   sent/received i
+00025af0: 6e20 6d75 6c74 6970 6c65 2063 6875 6e6b  n multiple chunk
+00025b00: 733b 2074 6869 7320 7368 6f75 6c64 2068  s; this should h
+00025b10: 656c 7020 666f 720a 2020 2020 2020 2020  elp for.        
+00025b20: 2320 6368 6563 6b69 6e67 2074 6861 7420  # checking that 
+00025b30: 7375 6368 206c 6f67 6963 2069 7320 636f  such logic is co
+00025b40: 7272 6563 742e 0a20 2020 2020 2020 2064  rrect..        d
+00025b50: 6174 615f 7369 7a65 203d 2031 3032 3420  ata_size = 1024 
+00025b60: 2a20 3130 3234 0a20 2020 2020 2020 206f  * 1024.        o
+00025b70: 7269 6769 6e61 6c5f 6461 7461 203d 206f  riginal_data = o
+00025b80: 732e 7572 616e 646f 6d28 6461 7461 5f73  s.urandom(data_s
+00025b90: 697a 6529 0a0a 2020 2020 2020 2020 636c  ize)..        cl
+00025ba0: 6965 6e74 203d 2073 656c 662e 636c 6965  ient = self.clie
+00025bb0: 6e74 0a20 2020 2020 2020 2063 6c69 656e  nt.        clien
+00025bc0: 742e 7075 7368 2866 227b 7365 6c66 2e70  t.push(f"{self.p
+00025bd0: 7265 6669 787d 2f74 6573 7422 2c20 6f72  refix}/test", or
+00025be0: 6967 696e 616c 5f64 6174 612c 2065 6e63  iginal_data, enc
+00025bf0: 6f64 696e 673d 4e6f 6e65 290a 2020 2020  oding=None).    
+00025c00: 2020 2020 7769 7468 2063 6c69 656e 742e      with client.
+00025c10: 7075 6c6c 2866 227b 7365 6c66 2e70 7265  pull(f"{self.pre
+00025c20: 6669 787d 2f74 6573 7422 2c20 656e 636f  fix}/test", enco
+00025c30: 6469 6e67 3d4e 6f6e 6529 2061 7320 696e  ding=None) as in
+00025c40: 6669 6c65 3a0a 2020 2020 2020 2020 2020  file:.          
+00025c50: 2020 7265 6365 6976 6564 5f64 6174 6120    received_data 
+00025c60: 3d20 696e 6669 6c65 2e72 6561 6428 290a  = infile.read().
+00025c70: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00025c80: 6572 7445 7175 616c 286f 7269 6769 6e61  ertEqual(origina
+00025c90: 6c5f 6461 7461 2c20 7265 6365 6976 6564  l_data, received
+00025ca0: 5f64 6174 6129 0a0a 2020 2020 6465 6620  _data)..    def 
+00025cb0: 7465 7374 5f70 7573 685f 746f 5f6e 6f6e  test_push_to_non
+00025cc0: 5f65 7869 7374 656e 745f 7375 6264 6972  _existent_subdir
+00025cd0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00025ce0: 6461 7461 203d 2027 6461 7461 270a 2020  data = 'data'.  
+00025cf0: 2020 2020 2020 636c 6965 6e74 203d 2073        client = s
+00025d00: 656c 662e 636c 6965 6e74 0a0a 2020 2020  elf.client..    
+00025d10: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
+00025d20: 7365 7274 5261 6973 6573 2870 6562 626c  sertRaises(pebbl
+00025d30: 652e 5061 7468 4572 726f 7229 2061 7320  e.PathError) as 
+00025d40: 636d 3a0a 2020 2020 2020 2020 2020 2020  cm:.            
+00025d50: 636c 6965 6e74 2e70 7573 6828 6622 7b73  client.push(f"{s
+00025d60: 656c 662e 7072 6566 6978 7d2f 6e6f 6e65  elf.prefix}/none
+00025d70: 7869 7374 656e 745f 6469 722f 7465 7374  xistent_dir/test
+00025d80: 222c 2064 6174 612c 206d 616b 655f 6469  ", data, make_di
+00025d90: 7273 3d46 616c 7365 290a 2020 2020 2020  rs=False).      
+00025da0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00025db0: 616c 2863 6d2e 6578 6365 7074 696f 6e2e  al(cm.exception.
+00025dc0: 6b69 6e64 2c20 276e 6f74 2d66 6f75 6e64  kind, 'not-found
+00025dd0: 2729 0a0a 2020 2020 2020 2020 636c 6965  ')..        clie
+00025de0: 6e74 2e70 7573 6828 6622 7b73 656c 662e  nt.push(f"{self.
+00025df0: 7072 6566 6978 7d2f 6e6f 6e65 7869 7374  prefix}/nonexist
+00025e00: 656e 745f 6469 722f 7465 7374 222c 2064  ent_dir/test", d
+00025e10: 6174 612c 206d 616b 655f 6469 7273 3d54  ata, make_dirs=T
+00025e20: 7275 6529 0a0a 2020 2020 6465 6620 7465  rue)..    def te
+00025e30: 7374 5f70 7573 685f 6173 5f63 6869 6c64  st_push_as_child
+00025e40: 5f6f 665f 6669 6c65 5f72 6169 7365 735f  _of_file_raises_
+00025e50: 6572 726f 7228 7365 6c66 293a 0a20 2020  error(self):.   
+00025e60: 2020 2020 2064 6174 6120 3d20 2764 6174       data = 'dat
+00025e70: 6127 0a20 2020 2020 2020 2063 6c69 656e  a'.        clien
+00025e80: 7420 3d20 7365 6c66 2e63 6c69 656e 740a  t = self.client.
+00025e90: 2020 2020 2020 2020 636c 6965 6e74 2e70          client.p
+00025ea0: 7573 6828 6622 7b73 656c 662e 7072 6566  ush(f"{self.pref
+00025eb0: 6978 7d2f 6669 6c65 222c 2064 6174 6129  ix}/file", data)
+00025ec0: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+00025ed0: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
+00025ee0: 7065 6262 6c65 2e50 6174 6845 7272 6f72  pebble.PathError
+00025ef0: 2920 6173 2063 6d3a 0a20 2020 2020 2020  ) as cm:.       
+00025f00: 2020 2020 2063 6c69 656e 742e 7075 7368       client.push
+00025f10: 2866 227b 7365 6c66 2e70 7265 6669 787d  (f"{self.prefix}
+00025f20: 2f66 696c 652f 6669 6c65 222c 2064 6174  /file/file", dat
+00025f30: 6129 0a20 2020 2020 2020 2073 656c 662e  a).        self.
+00025f40: 6173 7365 7274 4571 7561 6c28 636d 2e65  assertEqual(cm.e
+00025f50: 7863 6570 7469 6f6e 2e6b 696e 642c 2027  xception.kind, '
+00025f60: 6765 6e65 7269 632d 6669 6c65 2d65 7272  generic-file-err
+00025f70: 6f72 2729 0a0a 2020 2020 6465 6620 7465  or')..    def te
+00025f80: 7374 5f70 7573 685f 7769 7468 5f70 6572  st_push_with_per
+00025f90: 6d69 7373 696f 6e5f 6d61 736b 2873 656c  mission_mask(sel
+00025fa0: 6629 3a0a 2020 2020 2020 2020 6461 7461  f):.        data
+00025fb0: 203d 2027 6461 7461 270a 2020 2020 2020   = 'data'.      
+00025fc0: 2020 636c 6965 6e74 203d 2073 656c 662e    client = self.
+00025fd0: 636c 6965 6e74 0a20 2020 2020 2020 2063  client.        c
+00025fe0: 6c69 656e 742e 7075 7368 2866 227b 7365  lient.push(f"{se
+00025ff0: 6c66 2e70 7265 6669 787d 2f66 696c 6522  lf.prefix}/file"
+00026000: 2c20 6461 7461 2c20 7065 726d 6973 7369  , data, permissi
+00026010: 6f6e 733d 306f 3630 3029 0a20 2020 2020  ons=0o600).     
+00026020: 2020 2063 6c69 656e 742e 7075 7368 2866     client.push(f
+00026030: 227b 7365 6c66 2e70 7265 6669 787d 2f66  "{self.prefix}/f
+00026040: 696c 6522 2c20 6461 7461 2c20 7065 726d  ile", data, perm
+00026050: 6973 7369 6f6e 733d 306f 3737 3729 0a20  issions=0o777). 
+00026060: 2020 2020 2020 2023 2049 6620 7065 726d         # If perm
+00026070: 6973 7369 6f6e 7320 6172 6520 6f75 7473  issions are outs
+00026080: 6964 6520 6f66 2074 6865 2072 616e 6765  ide of the range
+00026090: 2030 6f30 3030 2074 6872 6f75 6768 2030   0o000 through 0
+000260a0: 6f37 3737 2c20 616e 2065 7863 6570 7469  o777, an excepti
+000260b0: 6f6e 2073 686f 756c 6420 6265 0a20 2020  on should be.   
+000260c0: 2020 2020 2023 2072 6169 7365 642e 0a20       # raised.. 
+000260d0: 2020 2020 2020 2066 6f72 2062 6164 5f70         for bad_p
+000260e0: 6572 6d69 7373 696f 6e20 696e 2028 0a20  ermission in (. 
+000260f0: 2020 2020 2020 2020 2020 2030 6f31 3030             0o100
+00026100: 302c 2020 2320 4578 6365 6564 7320 306f  0,  # Exceeds 0o
+00026110: 3737 370a 2020 2020 2020 2020 2020 2020  777.            
+00026120: 2d31 2c20 2020 2020 2023 204c 6573 7320  -1,      # Less 
+00026130: 7468 616e 2030 6f30 3030 0a20 2020 2020  than 0o000.     
+00026140: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+00026150: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
+00026160: 7274 5261 6973 6573 2870 6562 626c 652e  rtRaises(pebble.
+00026170: 5061 7468 4572 726f 7229 2061 7320 636d  PathError) as cm
+00026180: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00026190: 2020 636c 6965 6e74 2e70 7573 6828 6622    client.push(f"
+000261a0: 7b73 656c 662e 7072 6566 6978 7d2f 6669  {self.prefix}/fi
+000261b0: 6c65 222c 2064 6174 612c 2070 6572 6d69  le", data, permi
+000261c0: 7373 696f 6e73 3d62 6164 5f70 6572 6d69  ssions=bad_permi
+000261d0: 7373 696f 6e29 0a20 2020 2020 2020 2073  ssion).        s
+000261e0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000261f0: 636d 2e65 7863 6570 7469 6f6e 2e6b 696e  cm.exception.kin
+00026200: 642c 2027 6765 6e65 7269 632d 6669 6c65  d, 'generic-file
+00026210: 2d65 7272 6f72 2729 0a0a 2020 2020 6465  -error')..    de
+00026220: 6620 7465 7374 5f70 7573 685f 6669 6c65  f test_push_file
+00026230: 735f 616e 645f 6c69 7374 2873 656c 6629  s_and_list(self)
+00026240: 3a0a 2020 2020 2020 2020 6461 7461 203d  :.        data =
+00026250: 2027 6461 7461 270a 2020 2020 2020 2020   'data'.        
+00026260: 636c 6965 6e74 203d 2073 656c 662e 636c  client = self.cl
+00026270: 6965 6e74 0a0a 2020 2020 2020 2020 2320  ient..        # 
+00026280: 4c65 7427 7320 7075 7368 2074 6865 2066  Let's push the f
+00026290: 6972 7374 2066 696c 6520 7769 7468 2061  irst file with a
+000262a0: 2062 756e 6368 206f 6620 6465 7461 696c   bunch of detail
+000262b0: 732e 2020 5765 276c 6c20 6368 6563 6b20  s.  We'll check 
+000262c0: 6f6e 2074 6869 7320 6c61 7465 722e 0a20  on this later.. 
+000262d0: 2020 2020 2020 2063 6c69 656e 742e 7075         client.pu
+000262e0: 7368 280a 2020 2020 2020 2020 2020 2020  sh(.            
+000262f0: 6622 7b73 656c 662e 7072 6566 6978 7d2f  f"{self.prefix}/
+00026300: 6669 6c65 3122 2c20 6461 7461 2c0a 2020  file1", data,.  
+00026310: 2020 2020 2020 2020 2020 7065 726d 6973            permis
+00026320: 7369 6f6e 733d 306f 3632 3029 0a0a 2020  sions=0o620)..  
+00026330: 2020 2020 2020 2320 446f 2061 2071 7569        # Do a qui
+00026340: 636b 2070 7573 6820 7769 7468 2064 6566  ck push with def
+00026350: 6175 6c74 7320 666f 7220 7468 6520 6f74  aults for the ot
+00026360: 6865 7220 6669 6c65 732e 0a20 2020 2020  her files..     
+00026370: 2020 2063 6c69 656e 742e 7075 7368 2866     client.push(f
+00026380: 227b 7365 6c66 2e70 7265 6669 787d 2f66  "{self.prefix}/f
+00026390: 696c 6532 222c 2064 6174 6129 0a20 2020  ile2", data).   
+000263a0: 2020 2020 2063 6c69 656e 742e 7075 7368       client.push
+000263b0: 2866 227b 7365 6c66 2e70 7265 6669 787d  (f"{self.prefix}
+000263c0: 2f66 696c 6533 222c 2064 6174 6129 0a0a  /file3", data)..
+000263d0: 2020 2020 2020 2020 6669 6c65 7320 3d20          files = 
+000263e0: 636c 6965 6e74 2e6c 6973 745f 6669 6c65  client.list_file
+000263f0: 7328 6622 7b73 656c 662e 7072 6566 6978  s(f"{self.prefix
+00026400: 7d2f 2229 0a20 2020 2020 2020 2073 656c  }/").        sel
+00026410: 662e 6173 7365 7274 4571 7561 6c28 7b66  f.assertEqual({f
+00026420: 696c 652e 7061 7468 2066 6f72 2066 696c  ile.path for fil
+00026430: 6520 696e 2066 696c 6573 7d2c 0a20 2020  e in files},.   
+00026440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026450: 2020 2020 2020 7b73 656c 662e 7072 6566        {self.pref
+00026460: 6978 202b 2066 696c 6520 666f 7220 6669  ix + file for fi
+00026470: 6c65 2069 6e20 2827 2f66 696c 6531 272c  le in ('/file1',
+00026480: 2027 2f66 696c 6532 272c 2027 2f66 696c   '/file2', '/fil
+00026490: 6533 2729 7d29 0a0a 2020 2020 2020 2020  e3')})..        
+000264a0: 2320 4c65 7427 7320 7075 6c6c 2074 6865  # Let's pull the
+000264b0: 2066 6972 7374 2066 696c 6520 6167 6169   first file agai
+000264c0: 6e20 616e 6420 6368 6563 6b20 6974 7320  n and check its 
+000264d0: 6465 7461 696c 730a 2020 2020 2020 2020  details.        
+000264e0: 6669 6c65 203d 205b 6620 666f 7220 6620  file = [f for f 
+000264f0: 696e 2066 696c 6573 2069 6620 662e 7061  in files if f.pa
+00026500: 7468 203d 3d20 6622 7b73 656c 662e 7072  th == f"{self.pr
+00026510: 6566 6978 7d2f 6669 6c65 3122 5d5b 305d  efix}/file1"][0]
+00026520: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00026530: 7365 7274 4571 7561 6c28 6669 6c65 2e6e  sertEqual(file.n
+00026540: 616d 652c 2027 6669 6c65 3127 290a 2020  ame, 'file1').  
+00026550: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00026560: 7445 7175 616c 2866 696c 652e 7479 7065  tEqual(file.type
+00026570: 2c20 7065 6262 6c65 2e46 696c 6554 7970  , pebble.FileTyp
+00026580: 652e 4649 4c45 290a 2020 2020 2020 2020  e.FILE).        
+00026590: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000265a0: 2866 696c 652e 7369 7a65 2c20 3429 0a20  (file.size, 4). 
+000265b0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+000265c0: 7274 4973 496e 7374 616e 6365 2866 696c  rtIsInstance(fil
+000265d0: 652e 6c61 7374 5f6d 6f64 6966 6965 642c  e.last_modified,
+000265e0: 2064 6174 6574 696d 652e 6461 7465 7469   datetime.dateti
+000265f0: 6d65 290a 2020 2020 2020 2020 7365 6c66  me).        self
+00026600: 2e61 7373 6572 7445 7175 616c 2866 696c  .assertEqual(fil
+00026610: 652e 7065 726d 6973 7369 6f6e 732c 2030  e.permissions, 0
+00026620: 6f36 3230 290a 2020 2020 2020 2020 2320  o620).        # 
+00026630: 536b 6970 7069 6e67 206f 776e 6572 7368  Skipping ownersh
+00026640: 6970 2063 6865 636b 7320 6865 7265 3b20  ip checks here; 
+00026650: 6f77 6e65 7273 6869 7020 7769 6c6c 2062  ownership will b
+00026660: 6520 6368 6563 6b65 6420 696e 2070 7572  e checked in pur
+00026670: 656c 792d 6d6f 636b 6564 2074 6573 7473  ely-mocked tests
+00026680: 0a0a 2020 2020 6465 6620 7465 7374 5f70  ..    def test_p
+00026690: 7573 685f 616e 645f 6c69 7374 5f66 696c  ush_and_list_fil
+000266a0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000266b0: 2064 6174 6120 3d20 2764 6174 6127 0a20   data = 'data'. 
+000266c0: 2020 2020 2020 2063 6c69 656e 7420 3d20         client = 
+000266d0: 7365 6c66 2e63 6c69 656e 740a 2020 2020  self.client.    
+000266e0: 2020 2020 636c 6965 6e74 2e70 7573 6828      client.push(
+000266f0: 6622 7b73 656c 662e 7072 6566 6978 7d2f  f"{self.prefix}/
+00026700: 6669 6c65 222c 2064 6174 6129 0a20 2020  file", data).   
+00026710: 2020 2020 2066 696c 6573 203d 2063 6c69       files = cli
+00026720: 656e 742e 6c69 7374 5f66 696c 6573 2866  ent.list_files(f
+00026730: 227b 7365 6c66 2e70 7265 6669 787d 2f22  "{self.prefix}/"
+00026740: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00026750: 7373 6572 7445 7175 616c 287b 6669 6c65  ssertEqual({file
+00026760: 2e70 6174 6820 666f 7220 6669 6c65 2069  .path for file i
+00026770: 6e20 6669 6c65 737d 2c20 7b66 227b 7365  n files}, {f"{se
+00026780: 6c66 2e70 7265 6669 787d 2f66 696c 6522  lf.prefix}/file"
+00026790: 7d29 0a0a 2020 2020 6465 6620 7465 7374  })..    def test
+000267a0: 5f70 7573 685f 6669 6c65 5f77 6974 685f  _push_file_with_
+000267b0: 7265 6c61 7469 7665 5f70 6174 685f 6661  relative_path_fa
+000267c0: 696c 7328 7365 6c66 293a 0a20 2020 2020  ils(self):.     
+000267d0: 2020 2063 6c69 656e 7420 3d20 7365 6c66     client = self
+000267e0: 2e63 6c69 656e 740a 2020 2020 2020 2020  .client.        
+000267f0: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
+00026800: 5261 6973 6573 2870 6562 626c 652e 5061  Raises(pebble.Pa
+00026810: 7468 4572 726f 7229 2061 7320 636d 3a0a  thError) as cm:.
+00026820: 2020 2020 2020 2020 2020 2020 636c 6965              clie
+00026830: 6e74 2e70 7573 6828 2766 696c 6527 2c20  nt.push('file', 
+00026840: 2727 290a 2020 2020 2020 2020 7365 6c66  '').        self
+00026850: 2e61 7373 6572 7445 7175 616c 2863 6d2e  .assertEqual(cm.
+00026860: 6578 6365 7074 696f 6e2e 6b69 6e64 2c20  exception.kind, 
+00026870: 2767 656e 6572 6963 2d66 696c 652d 6572  'generic-file-er
+00026880: 726f 7227 290a 0a20 2020 2064 6566 2074  ror')..    def t
+00026890: 6573 745f 7075 6c6c 5f6e 6f74 5f66 6f75  est_pull_not_fou
+000268a0: 6e64 2873 656c 6629 3a0a 2020 2020 2020  nd(self):.      
+000268b0: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
+000268c0: 7274 5261 6973 6573 2870 6562 626c 652e  rtRaises(pebble.
+000268d0: 5061 7468 4572 726f 7229 2061 7320 636d  PathError) as cm
+000268e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000268f0: 6c66 2e63 6c69 656e 742e 7075 6c6c 2822  lf.client.pull("
+00026900: 2f6e 6f74 2f66 6f75 6e64 2229 0a20 2020  /not/found").   
+00026910: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00026920: 4571 7561 6c28 636d 2e65 7863 6570 7469  Equal(cm.excepti
+00026930: 6f6e 2e6b 696e 642c 2022 6e6f 742d 666f  on.kind, "not-fo
+00026940: 756e 6422 290a 2020 2020 2020 2020 7365  und").        se
+00026950: 6c66 2e61 7373 6572 7449 6e28 222f 6e6f  lf.assertIn("/no
+00026960: 742f 666f 756e 6422 2c20 636d 2e65 7863  t/found", cm.exc
+00026970: 6570 7469 6f6e 2e6d 6573 7361 6765 290a  eption.message).
+00026980: 0a20 2020 2064 6566 2074 6573 745f 7075  .    def test_pu
+00026990: 6c6c 5f64 6972 6563 746f 7279 2873 656c  ll_directory(sel
+000269a0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+000269b0: 2e63 6c69 656e 742e 6d61 6b65 5f64 6972  .client.make_dir
+000269c0: 2866 227b 7365 6c66 2e70 7265 6669 787d  (f"{self.prefix}
+000269d0: 2f73 7562 6469 7222 290a 2020 2020 2020  /subdir").      
+000269e0: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
+000269f0: 7274 5261 6973 6573 2870 6562 626c 652e  rtRaises(pebble.
+00026a00: 5061 7468 4572 726f 7229 2061 7320 636d  PathError) as cm
+00026a10: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00026a20: 6c66 2e63 6c69 656e 742e 7075 6c6c 2866  lf.client.pull(f
+00026a30: 227b 7365 6c66 2e70 7265 6669 787d 2f73  "{self.prefix}/s
+00026a40: 7562 6469 7222 290a 2020 2020 2020 2020  ubdir").        
+00026a50: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00026a60: 2863 6d2e 6578 6365 7074 696f 6e2e 6b69  (cm.exception.ki
+00026a70: 6e64 2c20 2267 656e 6572 6963 2d66 696c  nd, "generic-fil
+00026a80: 652d 6572 726f 7222 290a 2020 2020 2020  e-error").      
+00026a90: 2020 7365 6c66 2e61 7373 6572 7449 6e28    self.assertIn(
+00026aa0: 6622 7b73 656c 662e 7072 6566 6978 7d2f  f"{self.prefix}/
+00026ab0: 7375 6264 6972 222c 2063 6d2e 6578 6365  subdir", cm.exce
+00026ac0: 7074 696f 6e2e 6d65 7373 6167 6529 0a0a  ption.message)..
+00026ad0: 2020 2020 6465 6620 7465 7374 5f6c 6973      def test_lis
+00026ae0: 745f 6669 6c65 735f 6e6f 745f 666f 756e  t_files_not_foun
+00026af0: 645f 7261 6973 6573 2873 656c 6629 3a0a  d_raises(self):.
+00026b00: 2020 2020 2020 2020 636c 6965 6e74 203d          client =
+00026b10: 2073 656c 662e 636c 6965 6e74 0a20 2020   self.client.   
+00026b20: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
+00026b30: 7373 6572 7452 6169 7365 7328 7065 6262  ssertRaises(pebb
+00026b40: 6c65 2e41 5049 4572 726f 7229 2061 7320  le.APIError) as 
+00026b50: 636d 3a0a 2020 2020 2020 2020 2020 2020  cm:.            
+00026b60: 636c 6965 6e74 2e6c 6973 745f 6669 6c65  client.list_file
+00026b70: 7328 222f 6e6f 742f 6578 6973 7469 6e67  s("/not/existing
+00026b80: 2f66 696c 652f 2229 0a20 2020 2020 2020  /file/").       
+00026b90: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00026ba0: 6c28 636d 2e65 7863 6570 7469 6f6e 2e63  l(cm.exception.c
+00026bb0: 6f64 652c 2034 3034 290a 2020 2020 2020  ode, 404).      
+00026bc0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00026bd0: 616c 2863 6d2e 6578 6365 7074 696f 6e2e  al(cm.exception.
+00026be0: 7374 6174 7573 2c20 274e 6f74 2046 6f75  status, 'Not Fou
+00026bf0: 6e64 2729 0a20 2020 2020 2020 2073 656c  nd').        sel
+00026c00: 662e 6173 7365 7274 4571 7561 6c28 636d  f.assertEqual(cm
+00026c10: 2e65 7863 6570 7469 6f6e 2e6d 6573 7361  .exception.messa
+00026c20: 6765 2c20 2773 7461 7420 2f6e 6f74 2f65  ge, 'stat /not/e
+00026c30: 7869 7374 696e 672f 6669 6c65 2f3a 206e  xisting/file/: n
+00026c40: 6f20 270a 2020 2020 2020 2020 2020 2020  o '.            
+00026c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026c70: 2020 2027 7375 6368 2066 696c 6520 6f72     'such file or
+00026c80: 2064 6972 6563 746f 7279 2729 0a0a 2020   directory')..  
+00026c90: 2020 6465 6620 7465 7374 5f6c 6973 745f    def test_list_
+00026ca0: 6469 7265 6374 6f72 795f 6f62 6a65 6374  directory_object
+00026cb0: 5f69 7473 656c 6628 7365 6c66 293a 0a20  _itself(self):. 
+00026cc0: 2020 2020 2020 2063 6c69 656e 7420 3d20         client = 
+00026cd0: 7365 6c66 2e63 6c69 656e 740a 0a20 2020  self.client..   
+00026ce0: 2020 2020 2023 2054 6573 7420 7769 7468       # Test with
+00026cf0: 2072 6f6f 7420 6469 720a 2020 2020 2020   root dir.      
+00026d00: 2020 2320 2853 7065 6369 616c 2063 6173    # (Special cas
+00026d10: 653b 2077 6520 776f 6e27 7420 7072 6566  e; we won't pref
+00026d20: 6978 2074 6869 732c 2065 7665 6e20 7768  ix this, even wh
+00026d30: 656e 2075 7369 6e67 2074 6865 2072 6561  en using the rea
+00026d40: 6c20 5065 6262 6c65 2073 6572 7665 722e  l Pebble server.
+00026d50: 290a 2020 2020 2020 2020 6669 6c65 7320  ).        files 
+00026d60: 3d20 636c 6965 6e74 2e6c 6973 745f 6669  = client.list_fi
+00026d70: 6c65 7328 272f 272c 2069 7473 656c 663d  les('/', itself=
+00026d80: 5472 7565 290a 2020 2020 2020 2020 7365  True).        se
+00026d90: 6c66 2e61 7373 6572 7445 7175 616c 286c  lf.assertEqual(l
+00026da0: 656e 2866 696c 6573 292c 2031 290a 2020  en(files), 1).  
+00026db0: 2020 2020 2020 6469 725f 203d 2066 696c        dir_ = fil
+00026dc0: 6573 5b30 5d0a 2020 2020 2020 2020 7365  es[0].        se
+00026dd0: 6c66 2e61 7373 6572 7445 7175 616c 2864  lf.assertEqual(d
+00026de0: 6972 5f2e 7061 7468 2c20 272f 2729 0a20  ir_.path, '/'). 
+00026df0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00026e00: 7274 4571 7561 6c28 6469 725f 2e6e 616d  rtEqual(dir_.nam
+00026e10: 652c 2027 2f27 290a 2020 2020 2020 2020  e, '/').        
+00026e20: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00026e30: 2864 6972 5f2e 7479 7065 2c20 7065 6262  (dir_.type, pebb
+00026e40: 6c65 2e46 696c 6554 7970 652e 4449 5245  le.FileType.DIRE
+00026e50: 4354 4f52 5929 0a0a 2020 2020 2020 2020  CTORY)..        
+00026e60: 2320 5465 7374 2077 6974 6820 7375 6264  # Test with subd
+00026e70: 6972 730a 2020 2020 2020 2020 636c 6965  irs.        clie
+00026e80: 6e74 2e6d 616b 655f 6469 7228 6622 7b73  nt.make_dir(f"{s
+00026e90: 656c 662e 7072 6566 6978 7d2f 7375 6264  elf.prefix}/subd
+00026ea0: 6972 2229 0a20 2020 2020 2020 2066 696c  ir").        fil
+00026eb0: 6573 203d 2063 6c69 656e 742e 6c69 7374  es = client.list
+00026ec0: 5f66 696c 6573 2866 227b 7365 6c66 2e70  _files(f"{self.p
+00026ed0: 7265 6669 787d 2f73 7562 6469 7222 2c20  refix}/subdir", 
+00026ee0: 6974 7365 6c66 3d54 7275 6529 0a20 2020  itself=True).   
+00026ef0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00026f00: 4571 7561 6c28 6c65 6e28 6669 6c65 7329  Equal(len(files)
+00026f10: 2c20 3129 0a20 2020 2020 2020 2064 6972  , 1).        dir
+00026f20: 5f20 3d20 6669 6c65 735b 305d 0a20 2020  _ = files[0].   
+00026f30: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00026f40: 4571 7561 6c28 6469 725f 2e6e 616d 652c  Equal(dir_.name,
+00026f50: 2027 7375 6264 6972 2729 0a20 2020 2020   'subdir').     
+00026f60: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00026f70: 7561 6c28 6469 725f 2e74 7970 652c 2070  ual(dir_.type, p
+00026f80: 6562 626c 652e 4669 6c65 5479 7065 2e44  ebble.FileType.D
+00026f90: 4952 4543 544f 5259 290a 0a20 2020 2064  IRECTORY)..    d
+00026fa0: 6566 2074 6573 745f 7075 7368 5f66 696c  ef test_push_fil
+00026fb0: 6573 5f61 6e64 5f6c 6973 745f 6279 5f70  es_and_list_by_p
+00026fc0: 6174 7465 726e 2873 656c 6629 3a0a 2020  attern(self):.  
+00026fd0: 2020 2020 2020 2320 4e6f 7465 3a20 676c        # Note: gl
+00026fe0: 6f62 2070 6174 7465 726e 2064 656c 7461  ob pattern delta
+00026ff0: 7320 646f 2065 7869 7374 2062 6574 7765  s do exist betwe
+00027000: 656e 2067 6f6c 616e 6720 616e 6420 5079  en golang and Py
+00027010: 7468 6f6e 2c20 6275 7420 6865 7265 2c0a  thon, but here,.
+00027020: 2020 2020 2020 2020 2320 7765 276c 6c20          # we'll 
+00027030: 6a75 7374 2075 7365 2061 2073 696d 706c  just use a simpl
+00027040: 6520 2a20 7061 7474 6572 6e2e 0a20 2020  e * pattern..   
+00027050: 2020 2020 2064 6174 6120 3d20 2764 6174       data = 'dat
+00027060: 6127 0a20 2020 2020 2020 2063 6c69 656e  a'.        clien
+00027070: 7420 3d20 7365 6c66 2e63 6c69 656e 740a  t = self.client.
+00027080: 2020 2020 2020 2020 666f 7220 6669 6c65          for file
+00027090: 6e61 6d65 2069 6e20 280a 2020 2020 2020  name in (.      
+000270a0: 2020 2020 2020 272f 6669 6c65 312e 677a        '/file1.gz
+000270b0: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
+000270c0: 2f66 696c 6532 2e74 6172 2e67 7a27 2c0a  /file2.tar.gz',.
+000270d0: 2020 2020 2020 2020 2020 2020 272f 6669              '/fi
+000270e0: 6c65 332e 7461 722e 627a 3227 2c0a 2020  le3.tar.bz2',.  
+000270f0: 2020 2020 2020 2020 2020 272f 6261 636b            '/back
+00027100: 7570 5f66 696c 652e 677a 272c 0a20 2020  up_file.gz',.   
+00027110: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+00027120: 2020 2020 636c 6965 6e74 2e70 7573 6828      client.push(
+00027130: 7365 6c66 2e70 7265 6669 7820 2b20 6669  self.prefix + fi
+00027140: 6c65 6e61 6d65 2c20 6461 7461 290a 2020  lename, data).  
+00027150: 2020 2020 2020 6669 6c65 7320 3d20 636c        files = cl
+00027160: 6965 6e74 2e6c 6973 745f 6669 6c65 7328  ient.list_files(
+00027170: 6622 7b73 656c 662e 7072 6566 6978 7d2f  f"{self.prefix}/
+00027180: 222c 2070 6174 7465 726e 3d27 6669 6c65  ", pattern='file
+00027190: 2a2e 677a 2729 0a20 2020 2020 2020 2073  *.gz').        s
+000271a0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000271b0: 7b66 696c 652e 7061 7468 2066 6f72 2066  {file.path for f
+000271c0: 696c 6520 696e 2066 696c 6573 7d2c 0a20  ile in files},. 
+000271d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000271e0: 2020 2020 2020 2020 7b73 656c 662e 7072          {self.pr
+000271f0: 6566 6978 202b 2066 696c 6520 666f 7220  efix + file for 
+00027200: 6669 6c65 2069 6e20 2827 2f66 696c 6531  file in ('/file1
+00027210: 2e67 7a27 2c20 272f 6669 6c65 322e 7461  .gz', '/file2.ta
+00027220: 722e 677a 2729 7d29 0a0a 2020 2020 6465  r.gz')})..    de
+00027230: 6620 7465 7374 5f6d 616b 655f 6469 7265  f test_make_dire
+00027240: 6374 6f72 7928 7365 6c66 293a 0a20 2020  ctory(self):.   
+00027250: 2020 2020 2063 6c69 656e 7420 3d20 7365       client = se
+00027260: 6c66 2e63 6c69 656e 740a 2020 2020 2020  lf.client.      
+00027270: 2020 636c 6965 6e74 2e6d 616b 655f 6469    client.make_di
+00027280: 7228 6622 7b73 656c 662e 7072 6566 6978  r(f"{self.prefix
+00027290: 7d2f 7375 6264 6972 2229 0a20 2020 2020  }/subdir").     
+000272a0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000272b0: 7561 6c28 0a20 2020 2020 2020 2020 2020  ual(.           
+000272c0: 2063 6c69 656e 742e 6c69 7374 5f66 696c   client.list_fil
+000272d0: 6573 2866 227b 7365 6c66 2e70 7265 6669  es(f"{self.prefi
+000272e0: 787d 2f22 2c20 7061 7474 6572 6e3d 2773  x}/", pattern='s
+000272f0: 7562 6469 7227 295b 305d 2e70 6174 682c  ubdir')[0].path,
+00027300: 0a20 2020 2020 2020 2020 2020 2066 227b  .            f"{
+00027310: 7365 6c66 2e70 7265 6669 787d 2f73 7562  self.prefix}/sub
+00027320: 6469 7222 290a 2020 2020 2020 2020 636c  dir").        cl
+00027330: 6965 6e74 2e6d 616b 655f 6469 7228 6622  ient.make_dir(f"
+00027340: 7b73 656c 662e 7072 6566 6978 7d2f 7375  {self.prefix}/su
+00027350: 6264 6972 2f73 7562 6469 7222 290a 2020  bdir/subdir").  
+00027360: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00027370: 7445 7175 616c 280a 2020 2020 2020 2020  tEqual(.        
+00027380: 2020 2020 636c 6965 6e74 2e6c 6973 745f      client.list_
+00027390: 6669 6c65 7328 6622 7b73 656c 662e 7072  files(f"{self.pr
+000273a0: 6566 6978 7d2f 7375 6264 6972 222c 2070  efix}/subdir", p
+000273b0: 6174 7465 726e 3d27 7375 6264 6972 2729  attern='subdir')
+000273c0: 5b30 5d2e 7061 7468 2c0a 2020 2020 2020  [0].path,.      
+000273d0: 2020 2020 2020 6622 7b73 656c 662e 7072        f"{self.pr
+000273e0: 6566 6978 7d2f 7375 6264 6972 2f73 7562  efix}/subdir/sub
+000273f0: 6469 7222 290a 0a20 2020 2064 6566 2074  dir")..    def t
+00027400: 6573 745f 6d61 6b65 5f64 6972 6563 746f  est_make_directo
+00027410: 7279 5f72 6563 7572 7369 7665 6c79 2873  ry_recursively(s
+00027420: 656c 6629 3a0a 2020 2020 2020 2020 636c  elf):.        cl
+00027430: 6965 6e74 203d 2073 656c 662e 636c 6965  ient = self.clie
+00027440: 6e74 0a0a 2020 2020 2020 2020 7769 7468  nt..        with
+00027450: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
+00027460: 6573 2870 6562 626c 652e 5061 7468 4572  es(pebble.PathEr
+00027470: 726f 7229 2061 7320 636d 3a0a 2020 2020  ror) as cm:.    
+00027480: 2020 2020 2020 2020 636c 6965 6e74 2e6d          client.m
+00027490: 616b 655f 6469 7228 6622 7b73 656c 662e  ake_dir(f"{self.
+000274a0: 7072 6566 6978 7d2f 7375 6264 6972 2f73  prefix}/subdir/s
+000274b0: 7562 6469 7222 2c20 6d61 6b65 5f70 6172  ubdir", make_par
+000274c0: 656e 7473 3d46 616c 7365 290a 2020 2020  ents=False).    
+000274d0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+000274e0: 7175 616c 2863 6d2e 6578 6365 7074 696f  qual(cm.exceptio
+000274f0: 6e2e 6b69 6e64 2c20 276e 6f74 2d66 6f75  n.kind, 'not-fou
+00027500: 6e64 2729 0a0a 2020 2020 2020 2020 636c  nd')..        cl
+00027510: 6965 6e74 2e6d 616b 655f 6469 7228 6622  ient.make_dir(f"
+00027520: 7b73 656c 662e 7072 6566 6978 7d2f 7375  {self.prefix}/su
+00027530: 6264 6972 2f73 7562 6469 7222 2c20 6d61  bdir/subdir", ma
+00027540: 6b65 5f70 6172 656e 7473 3d54 7275 6529  ke_parents=True)
+00027550: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00027560: 7365 7274 4571 7561 6c28 0a20 2020 2020  sertEqual(.     
+00027570: 2020 2020 2020 2063 6c69 656e 742e 6c69         client.li
+00027580: 7374 5f66 696c 6573 2866 227b 7365 6c66  st_files(f"{self
+00027590: 2e70 7265 6669 787d 2f73 7562 6469 7222  .prefix}/subdir"
+000275a0: 2c20 7061 7474 6572 6e3d 2773 7562 6469  , pattern='subdi
+000275b0: 7227 295b 305d 2e70 6174 682c 0a20 2020  r')[0].path,.   
+000275c0: 2020 2020 2020 2020 2066 227b 7365 6c66           f"{self
+000275d0: 2e70 7265 6669 787d 2f73 7562 6469 722f  .prefix}/subdir/
+000275e0: 7375 6264 6972 2229 0a0a 2020 2020 6465  subdir")..    de
+000275f0: 6620 7465 7374 5f6d 616b 655f 6469 7265  f test_make_dire
+00027600: 6374 6f72 795f 7769 7468 5f72 656c 6174  ctory_with_relat
+00027610: 6976 655f 7061 7468 5f66 6169 6c73 2873  ive_path_fails(s
+00027620: 656c 6629 3a0a 2020 2020 2020 2020 636c  elf):.        cl
+00027630: 6965 6e74 203d 2073 656c 662e 636c 6965  ient = self.clie
+00027640: 6e74 0a20 2020 2020 2020 2077 6974 6820  nt.        with 
+00027650: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
+00027660: 7328 7065 6262 6c65 2e50 6174 6845 7272  s(pebble.PathErr
+00027670: 6f72 2920 6173 2063 6d3a 0a20 2020 2020  or) as cm:.     
+00027680: 2020 2020 2020 2063 6c69 656e 742e 6d61         client.ma
+00027690: 6b65 5f64 6972 2827 6469 7227 290a 2020  ke_dir('dir').  
+000276a0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000276b0: 7445 7175 616c 2863 6d2e 6578 6365 7074  tEqual(cm.except
+000276c0: 696f 6e2e 6b69 6e64 2c20 2767 656e 6572  ion.kind, 'gener
+000276d0: 6963 2d66 696c 652d 6572 726f 7227 290a  ic-file-error').
+000276e0: 0a20 2020 2064 6566 2074 6573 745f 6d61  .    def test_ma
+000276f0: 6b65 5f73 7562 6469 725f 6f66 5f66 696c  ke_subdir_of_fil
+00027700: 655f 6661 696c 7328 7365 6c66 293a 0a20  e_fails(self):. 
+00027710: 2020 2020 2020 2063 6c69 656e 7420 3d20         client = 
+00027720: 7365 6c66 2e63 6c69 656e 740a 2020 2020  self.client.    
+00027730: 2020 2020 636c 6965 6e74 2e70 7573 6828      client.push(
+00027740: 6622 7b73 656c 662e 7072 6566 6978 7d2f  f"{self.prefix}/
+00027750: 6669 6c65 222c 2027 6461 7461 2729 0a0a  file", 'data')..
+00027760: 2020 2020 2020 2020 2320 4469 7265 6374          # Direct
+00027770: 2063 6869 6c64 2063 6173 650a 2020 2020   child case.    
+00027780: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
+00027790: 7365 7274 5261 6973 6573 2870 6562 626c  sertRaises(pebbl
+000277a0: 652e 5061 7468 4572 726f 7229 2061 7320  e.PathError) as 
+000277b0: 636d 3a0a 2020 2020 2020 2020 2020 2020  cm:.            
+000277c0: 636c 6965 6e74 2e6d 616b 655f 6469 7228  client.make_dir(
+000277d0: 6622 7b73 656c 662e 7072 6566 6978 7d2f  f"{self.prefix}/
+000277e0: 6669 6c65 2f73 7562 6469 7222 290a 2020  file/subdir").  
+000277f0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00027800: 7445 7175 616c 2863 6d2e 6578 6365 7074  tEqual(cm.except
+00027810: 696f 6e2e 6b69 6e64 2c20 2767 656e 6572  ion.kind, 'gener
+00027820: 6963 2d66 696c 652d 6572 726f 7227 290a  ic-file-error').
+00027830: 0a20 2020 2020 2020 2023 2052 6563 7572  .        # Recur
+00027840: 7369 7665 2063 7265 6174 696f 6e20 6361  sive creation ca
+00027850: 7365 2c20 696e 2063 6173 6520 6974 7320  se, in case its 
+00027860: 666c 6f77 2069 7320 6469 6666 6572 656e  flow is differen
+00027870: 740a 2020 2020 2020 2020 7769 7468 2073  t.        with s
+00027880: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
+00027890: 2870 6562 626c 652e 5061 7468 4572 726f  (pebble.PathErro
+000278a0: 7229 2061 7320 636d 3a0a 2020 2020 2020  r) as cm:.      
+000278b0: 2020 2020 2020 636c 6965 6e74 2e6d 616b        client.mak
+000278c0: 655f 6469 7228 6622 7b73 656c 662e 7072  e_dir(f"{self.pr
+000278d0: 6566 6978 7d2f 6669 6c65 2f73 7562 6469  efix}/file/subdi
+000278e0: 722f 7375 6264 6972 222c 206d 616b 655f  r/subdir", make_
+000278f0: 7061 7265 6e74 733d 5472 7565 290a 2020  parents=True).  
+00027900: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00027910: 7445 7175 616c 2863 6d2e 6578 6365 7074  tEqual(cm.except
+00027920: 696f 6e2e 6b69 6e64 2c20 2767 656e 6572  ion.kind, 'gener
+00027930: 6963 2d66 696c 652d 6572 726f 7227 290a  ic-file-error').
+00027940: 0a20 2020 2064 6566 2074 6573 745f 6d61  .    def test_ma
+00027950: 6b65 5f64 6972 5f77 6974 685f 7065 726d  ke_dir_with_perm
+00027960: 6973 7369 6f6e 5f6d 6173 6b28 7365 6c66  ission_mask(self
+00027970: 293a 0a20 2020 2020 2020 2063 6c69 656e  ):.        clien
+00027980: 7420 3d20 7365 6c66 2e63 6c69 656e 740a  t = self.client.
+00027990: 2020 2020 2020 2020 636c 6965 6e74 2e6d          client.m
+000279a0: 616b 655f 6469 7228 6622 7b73 656c 662e  ake_dir(f"{self.
+000279b0: 7072 6566 6978 7d2f 6469 7231 222c 2070  prefix}/dir1", p
+000279c0: 6572 6d69 7373 696f 6e73 3d30 6f37 3030  ermissions=0o700
+000279d0: 290a 2020 2020 2020 2020 636c 6965 6e74  ).        client
+000279e0: 2e6d 616b 655f 6469 7228 6622 7b73 656c  .make_dir(f"{sel
+000279f0: 662e 7072 6566 6978 7d2f 6469 7232 222c  f.prefix}/dir2",
+00027a00: 2070 6572 6d69 7373 696f 6e73 3d30 6f37   permissions=0o7
+00027a10: 3737 290a 0a20 2020 2020 2020 2066 696c  77)..        fil
+00027a20: 6573 203d 2063 6c69 656e 742e 6c69 7374  es = client.list
+00027a30: 5f66 696c 6573 2866 227b 7365 6c66 2e70  _files(f"{self.p
+00027a40: 7265 6669 787d 2f22 2c20 7061 7474 6572  refix}/", patter
+00027a50: 6e3d 2764 6972 2a27 290a 2020 2020 2020  n='dir*').      
+00027a60: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00027a70: 616c 285b 6620 666f 7220 6620 696e 2066  al([f for f in f
+00027a80: 696c 6573 2069 6620 662e 7061 7468 203d  iles if f.path =
+00027a90: 3d20 6622 7b73 656c 662e 7072 6566 6978  = f"{self.prefix
+00027aa0: 7d2f 6469 7231 225d 0a20 2020 2020 2020  }/dir1"].       
+00027ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027ac0: 2020 5b30 5d2e 7065 726d 6973 7369 6f6e    [0].permission
+00027ad0: 732c 2030 6f37 3030 290a 2020 2020 2020  s, 0o700).      
+00027ae0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00027af0: 616c 285b 6620 666f 7220 6620 696e 2066  al([f for f in f
+00027b00: 696c 6573 2069 6620 662e 7061 7468 203d  iles if f.path =
+00027b10: 3d20 6622 7b73 656c 662e 7072 6566 6978  = f"{self.prefix
+00027b20: 7d2f 6469 7232 225d 0a20 2020 2020 2020  }/dir2"].       
+00027b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027b40: 2020 5b30 5d2e 7065 726d 6973 7369 6f6e    [0].permission
+00027b50: 732c 2030 6f37 3737 290a 0a20 2020 2020  s, 0o777)..     
+00027b60: 2020 2023 2049 6620 7065 726d 6973 7369     # If permissi
+00027b70: 6f6e 7320 6172 6520 6f75 7473 6964 6520  ons are outside 
+00027b80: 6f66 2074 6865 2072 616e 6765 2030 6f30  of the range 0o0
+00027b90: 3030 2074 6872 6f75 6768 2030 6f37 3737  00 through 0o777
+00027ba0: 2c20 616e 2065 7863 6570 7469 6f6e 2073  , an exception s
+00027bb0: 686f 756c 6420 6265 0a20 2020 2020 2020  hould be.       
+00027bc0: 2023 2072 6169 7365 642e 0a20 2020 2020   # raised..     
+00027bd0: 2020 2066 6f72 2069 2c20 6261 645f 7065     for i, bad_pe
+00027be0: 726d 6973 7369 6f6e 2069 6e20 656e 756d  rmission in enum
+00027bf0: 6572 6174 6528 280a 2020 2020 2020 2020  erate((.        
+00027c00: 2020 2020 306f 3130 3030 2c20 2023 2045      0o1000,  # E
+00027c10: 7863 6565 6473 2030 6f37 3737 0a20 2020  xceeds 0o777.   
+00027c20: 2020 2020 2020 2020 202d 312c 2020 2020           -1,    
+00027c30: 2020 2320 4c65 7373 2074 6861 6e20 306f    # Less than 0o
+00027c40: 3030 300a 2020 2020 2020 2020 2929 3a0a  000.        )):.
+00027c50: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00027c60: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
+00027c70: 6573 2870 6562 626c 652e 5061 7468 4572  es(pebble.PathEr
+00027c80: 726f 7229 2061 7320 636d 3a0a 2020 2020  ror) as cm:.    
+00027c90: 2020 2020 2020 2020 2020 2020 636c 6965              clie
+00027ca0: 6e74 2e6d 616b 655f 6469 7228 6622 7b73  nt.make_dir(f"{s
+00027cb0: 656c 662e 7072 6566 6978 7d2f 6469 7233  elf.prefix}/dir3
+00027cc0: 5f7b 697d 222c 2070 6572 6d69 7373 696f  _{i}", permissio
+00027cd0: 6e73 3d62 6164 5f70 6572 6d69 7373 696f  ns=bad_permissio
+00027ce0: 6e29 0a20 2020 2020 2020 2020 2020 2073  n).            s
+00027cf0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00027d00: 636d 2e65 7863 6570 7469 6f6e 2e6b 696e  cm.exception.kin
+00027d10: 642c 2027 6765 6e65 7269 632d 6669 6c65  d, 'generic-file
+00027d20: 2d65 7272 6f72 2729 0a0a 2020 2020 6465  -error')..    de
+00027d30: 6620 7465 7374 5f72 656d 6f76 655f 7061  f test_remove_pa
+00027d40: 7468 2873 656c 6629 3a0a 2020 2020 2020  th(self):.      
+00027d50: 2020 636c 6965 6e74 203d 2073 656c 662e    client = self.
+00027d60: 636c 6965 6e74 0a20 2020 2020 2020 2063  client.        c
+00027d70: 6c69 656e 742e 7075 7368 2866 227b 7365  lient.push(f"{se
+00027d80: 6c66 2e70 7265 6669 787d 2f66 696c 6522  lf.prefix}/file"
+00027d90: 2c20 2727 290a 2020 2020 2020 2020 636c  , '').        cl
+00027da0: 6965 6e74 2e6d 616b 655f 6469 7228 6622  ient.make_dir(f"
+00027db0: 7b73 656c 662e 7072 6566 6978 7d2f 6469  {self.prefix}/di
+00027dc0: 722f 7375 6264 6972 222c 206d 616b 655f  r/subdir", make_
+00027dd0: 7061 7265 6e74 733d 5472 7565 290a 2020  parents=True).  
+00027de0: 2020 2020 2020 636c 6965 6e74 2e70 7573        client.pus
+00027df0: 6828 6622 7b73 656c 662e 7072 6566 6978  h(f"{self.prefix
+00027e00: 7d2f 6469 722f 7375 6264 6972 2f66 696c  }/dir/subdir/fil
+00027e10: 6531 222c 2027 2729 0a20 2020 2020 2020  e1", '').       
+00027e20: 2063 6c69 656e 742e 7075 7368 2866 227b   client.push(f"{
+00027e30: 7365 6c66 2e70 7265 6669 787d 2f64 6972  self.prefix}/dir
+00027e40: 2f73 7562 6469 722f 6669 6c65 3222 2c20  /subdir/file2", 
+00027e50: 2727 290a 2020 2020 2020 2020 636c 6965  '').        clie
+00027e60: 6e74 2e70 7573 6828 6622 7b73 656c 662e  nt.push(f"{self.
+00027e70: 7072 6566 6978 7d2f 6469 722f 7375 6264  prefix}/dir/subd
+00027e80: 6972 2f66 696c 6533 222c 2027 2729 0a20  ir/file3", ''). 
+00027e90: 2020 2020 2020 2063 6c69 656e 742e 6d61         client.ma
+00027ea0: 6b65 5f64 6972 2866 227b 7365 6c66 2e70  ke_dir(f"{self.p
+00027eb0: 7265 6669 787d 2f65 6d70 7479 5f64 6972  refix}/empty_dir
+00027ec0: 2229 0a0a 2020 2020 2020 2020 636c 6965  ")..        clie
+00027ed0: 6e74 2e72 656d 6f76 655f 7061 7468 2866  nt.remove_path(f
+00027ee0: 227b 7365 6c66 2e70 7265 6669 787d 2f66  "{self.prefix}/f
+00027ef0: 696c 6522 290a 0a20 2020 2020 2020 2063  ile")..        c
+00027f00: 6c69 656e 742e 7265 6d6f 7665 5f70 6174  lient.remove_pat
+00027f10: 6828 6622 7b73 656c 662e 7072 6566 6978  h(f"{self.prefix
+00027f20: 7d2f 656d 7074 795f 6469 7222 290a 0a20  }/empty_dir").. 
+00027f30: 2020 2020 2020 2023 2052 656d 6f76 6520         # Remove 
+00027f40: 6e6f 6e2d 656d 7074 7920 6469 7265 6374  non-empty direct
+00027f50: 6f72 792c 2072 6563 7572 7369 7665 3d46  ory, recursive=F
+00027f60: 616c 7365 3a20 6572 726f 720a 2020 2020  alse: error.    
+00027f70: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
+00027f80: 7365 7274 5261 6973 6573 2870 6562 626c  sertRaises(pebbl
+00027f90: 652e 5061 7468 4572 726f 7229 2061 7320  e.PathError) as 
+00027fa0: 636d 3a0a 2020 2020 2020 2020 2020 2020  cm:.            
+00027fb0: 636c 6965 6e74 2e72 656d 6f76 655f 7061  client.remove_pa
+00027fc0: 7468 2866 227b 7365 6c66 2e70 7265 6669  th(f"{self.prefi
+00027fd0: 787d 2f64 6972 222c 2072 6563 7572 7369  x}/dir", recursi
+00027fe0: 7665 3d46 616c 7365 290a 2020 2020 2020  ve=False).      
+00027ff0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00028000: 616c 2863 6d2e 6578 6365 7074 696f 6e2e  al(cm.exception.
+00028010: 6b69 6e64 2c20 2767 656e 6572 6963 2d66  kind, 'generic-f
+00028020: 696c 652d 6572 726f 7227 290a 0a20 2020  ile-error')..   
+00028030: 2020 2020 2023 2052 656d 6f76 6520 6e6f       # Remove no
+00028040: 6e2d 656d 7074 7920 6469 7265 6374 6f72  n-empty director
+00028050: 792c 2072 6563 7572 7369 7665 3d54 7275  y, recursive=Tru
+00028060: 653a 2073 7563 6365 6564 7320 2861 6e64  e: succeeds (and
+00028070: 2072 656d 6f76 6573 2063 6869 6c64 206f   removes child o
+00028080: 626a 6563 7473 290a 2020 2020 2020 2020  bjects).        
+00028090: 636c 6965 6e74 2e72 656d 6f76 655f 7061  client.remove_pa
+000280a0: 7468 2866 227b 7365 6c66 2e70 7265 6669  th(f"{self.prefi
+000280b0: 787d 2f64 6972 222c 2072 6563 7572 7369  x}/dir", recursi
+000280c0: 7665 3d54 7275 6529 0a0a 2020 2020 2020  ve=True)..      
+000280d0: 2020 2320 5265 6d6f 7665 206e 6f6e 2d65    # Remove non-e
+000280e0: 7869 7374 656e 7420 7061 7468 2c20 7265  xistent path, re
+000280f0: 6375 7273 6976 653d 4661 6c73 653a 2065  cursive=False: e
+00028100: 7272 6f72 0a20 2020 2020 2020 2077 6974  rror.        wit
+00028110: 6820 7365 6c66 2e61 7373 6572 7452 6169  h self.assertRai
+00028120: 7365 7328 7065 6262 6c65 2e50 6174 6845  ses(pebble.PathE
+00028130: 7272 6f72 2920 6173 2063 6d3a 0a20 2020  rror) as cm:.   
+00028140: 2020 2020 2020 2020 2063 6c69 656e 742e           client.
+00028150: 7265 6d6f 7665 5f70 6174 6828 6622 7b73  remove_path(f"{s
+00028160: 656c 662e 7072 6566 6978 7d2f 6469 722f  elf.prefix}/dir/
+00028170: 646f 6573 2f6e 6f74 2f65 7869 7374 2f61  does/not/exist/a
+00028180: 7364 6622 2c20 7265 6375 7273 6976 653d  sdf", recursive=
+00028190: 4661 6c73 6529 0a20 2020 2020 2020 2073  False).        s
+000281a0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000281b0: 636d 2e65 7863 6570 7469 6f6e 2e6b 696e  cm.exception.kin
+000281c0: 642c 2027 6e6f 742d 666f 756e 6427 290a  d, 'not-found').
+000281d0: 0a20 2020 2020 2020 2023 2052 656d 6f76  .        # Remov
+000281e0: 6520 6e6f 6e2d 6578 6973 7465 6e74 2070  e non-existent p
+000281f0: 6174 682c 2072 6563 7572 7369 7665 3d54  ath, recursive=T
+00028200: 7275 653a 2073 7563 6365 6564 730a 2020  rue: succeeds.  
+00028210: 2020 2020 2020 636c 6965 6e74 2e72 656d        client.rem
+00028220: 6f76 655f 7061 7468 2866 227b 7365 6c66  ove_path(f"{self
+00028230: 2e70 7265 6669 787d 2f64 6972 2f64 6f65  .prefix}/dir/doe
+00028240: 732f 6e6f 742f 6578 6973 742f 6173 6466  s/not/exist/asdf
+00028250: 222c 2072 6563 7572 7369 7665 3d54 7275  ", recursive=Tru
+00028260: 6529 0a0a 2020 2020 2320 4f74 6865 7220  e)..    # Other 
+00028270: 6e6f 7465 733a 0a20 2020 2023 202a 2050  notes:.    # * P
+00028280: 6172 656e 7420 6469 7265 6374 6f72 6965  arent directorie
+00028290: 7320 6372 6561 7465 6420 7669 6120 7075  s created via pu
+000282a0: 7368 286d 616b 655f 6469 7273 3d54 7275  sh(make_dirs=Tru
+000282b0: 6529 2064 6566 6175 6c74 2074 6f20 726f  e) default to ro
+000282c0: 6f74 3a72 6f6f 7420 6f77 6e65 7273 6869  ot:root ownershi
+000282d0: 700a 2020 2020 2320 2020 616e 6420 7768  p.    #   and wh
+000282e0: 6174 6576 6572 2070 6572 6d69 7373 696f  atever permissio
+000282f0: 6e73 2061 7265 2073 7065 6369 6669 6564  ns are specified
+00028300: 2076 6961 2074 6865 2070 6572 6d69 7373   via the permiss
+00028310: 696f 6e73 2061 7267 756d 656e 743b 2061  ions argument; a
+00028320: 7320 7765 2064 6566 6175 6c74 2074 6f20  s we default to 
+00028330: 4e6f 6e65 0a20 2020 2023 2020 2066 6f72  None.    #   for
+00028340: 206f 776e 6572 7368 6970 2f70 6572 6d69   ownership/permi
+00028350: 7373 696f 6e73 2c20 7765 2064 6f20 6967  ssions, we do ig
+00028360: 6e6f 7265 2074 6869 7320 6e75 616e 6365  nore this nuance
+00028370: 2e0a 2020 2020 2320 2a20 5061 7265 6e74  ..    # * Parent
+00028380: 2064 6972 6563 746f 7269 6573 2063 7265   directories cre
+00028390: 6174 6564 2076 6961 206d 616b 655f 6469  ated via make_di
+000283a0: 7228 6d61 6b65 5f70 6172 656e 7473 3d54  r(make_parents=T
+000283b0: 7275 6529 2064 6566 6175 6c74 2074 6f20  rue) default to 
+000283c0: 726f 6f74 3a72 6f6f 7420 6f77 6e65 7273  root:root owners
+000283d0: 6869 700a 2020 2020 2320 2020 616e 6420  hip.    #   and 
+000283e0: 306f 3735 3520 7065 726d 6973 7369 6f6e  0o755 permission
+000283f0: 733b 2061 7320 7765 2064 6566 6175 6c74  s; as we default
+00028400: 2074 6f20 4e6f 6e65 2066 6f72 206f 776e   to None for own
+00028410: 6572 7368 6970 2f70 6572 6d69 7373 696f  ership/permissio
+00028420: 6e73 2c20 7765 2064 6f20 6967 6e6f 7265  ns, we do ignore
+00028430: 2074 6869 730a 2020 2020 2320 2020 6e75   this.    #   nu
+00028440: 616e 6365 2e0a 0a0a 636c 6173 7320 4765  ance....class Ge
+00028450: 6e65 7269 6354 6573 7469 6e67 4669 6c65  nericTestingFile
+00028460: 7379 7374 656d 5465 7374 733a 0a20 2020  systemTests:.   
+00028470: 2064 6566 2074 6573 745f 6c69 7374 6469   def test_listdi
+00028480: 725f 726f 6f74 5f6f 6e5f 656d 7074 795f  r_root_on_empty_
+00028490: 6f73 2873 656c 6629 3a0a 2020 2020 2020  os(self):.      
+000284a0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+000284b0: 616c 2873 656c 662e 6673 2e6c 6973 745f  al(self.fs.list_
+000284c0: 6469 7228 272f 2729 2c20 5b5d 290a 0a20  dir('/'), []).. 
+000284d0: 2020 2064 6566 2074 6573 745f 6c69 7374     def test_list
+000284e0: 6469 725f 6f6e 5f6e 6f6e 6578 6973 7465  dir_on_nonexiste
+000284f0: 6e74 5f64 6972 2873 656c 6629 3a0a 2020  nt_dir(self):.  
+00028500: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00028510: 6173 7365 7274 5261 6973 6573 2846 696c  assertRaises(Fil
+00028520: 654e 6f74 466f 756e 6445 7272 6f72 2920  eNotFoundError) 
+00028530: 6173 2063 6d3a 0a20 2020 2020 2020 2020  as cm:.         
+00028540: 2020 2073 656c 662e 6673 2e6c 6973 745f     self.fs.list_
+00028550: 6469 7228 272f 6574 6327 290a 2020 2020  dir('/etc').    
+00028560: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+00028570: 7275 6528 272f 6574 6327 2069 6e20 636d  rue('/etc' in cm
+00028580: 2e65 7863 6570 7469 6f6e 2e61 7267 735b  .exception.args[
+00028590: 305d 290a 0a20 2020 2064 6566 2074 6573  0])..    def tes
+000285a0: 745f 6c69 7374 6469 7228 7365 6c66 293a  t_listdir(self):
+000285b0: 0a20 2020 2020 2020 2073 656c 662e 6673  .        self.fs
+000285c0: 2e63 7265 6174 655f 6469 7228 272f 6f70  .create_dir('/op
+000285d0: 7427 290a 2020 2020 2020 2020 7365 6c66  t').        self
+000285e0: 2e66 732e 6372 6561 7465 5f66 696c 6528  .fs.create_file(
+000285f0: 272f 6f70 742f 6669 6c65 3127 2c20 2764  '/opt/file1', 'd
+00028600: 6174 6127 290a 2020 2020 2020 2020 7365  ata').        se
+00028610: 6c66 2e66 732e 6372 6561 7465 5f66 696c  lf.fs.create_fil
+00028620: 6528 272f 6f70 742f 6669 6c65 3227 2c20  e('/opt/file2', 
+00028630: 2764 6174 6127 290a 2020 2020 2020 2020  'data').        
+00028640: 6578 7065 6374 6564 5f72 6573 756c 7473  expected_results
+00028650: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+00028660: 2070 6174 686c 6962 2e50 7572 6550 6f73   pathlib.PurePos
+00028670: 6978 5061 7468 2827 2f6f 7074 2f66 696c  ixPath('/opt/fil
+00028680: 6531 2729 2c0a 2020 2020 2020 2020 2020  e1'),.          
+00028690: 2020 7061 7468 6c69 622e 5075 7265 506f    pathlib.PurePo
+000286a0: 7369 7850 6174 6828 272f 6f70 742f 6669  sixPath('/opt/fi
+000286b0: 6c65 3227 297d 0a20 2020 2020 2020 2073  le2')}.        s
+000286c0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000286d0: 6578 7065 6374 6564 5f72 6573 756c 7473  expected_results
+000286e0: 2c20 7b66 2e70 6174 6820 666f 7220 6620  , {f.path for f 
+000286f0: 696e 2073 656c 662e 6673 2e6c 6973 745f  in self.fs.list_
+00028700: 6469 7228 272f 6f70 7427 297d 290a 2020  dir('/opt')}).  
+00028710: 2020 2020 2020 2320 456e 7375 7265 2074        # Ensure t
+00028720: 6861 7420 5061 7468 7320 616c 736f 2077  hat Paths also w
+00028730: 6f72 6b20 666f 7220 6c69 7374 6469 720a  ork for listdir.
+00028740: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00028750: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
+00028760: 2020 2020 2020 6578 7065 6374 6564 5f72        expected_r
+00028770: 6573 756c 7473 2c20 7b66 2e70 6174 6820  esults, {f.path 
+00028780: 666f 7220 6620 696e 2073 656c 662e 6673  for f in self.fs
+00028790: 2e6c 6973 745f 6469 7228 7061 7468 6c69  .list_dir(pathli
+000287a0: 622e 5075 7265 506f 7369 7850 6174 6828  b.PurePosixPath(
+000287b0: 272f 6f70 7427 2929 7d29 0a0a 2020 2020  '/opt'))})..    
+000287c0: 6465 6620 7465 7374 5f6c 6973 7464 6972  def test_listdir
+000287d0: 5f6f 6e5f 6669 6c65 2873 656c 6629 3a0a  _on_file(self):.
+000287e0: 2020 2020 2020 2020 7365 6c66 2e66 732e          self.fs.
+000287f0: 6372 6561 7465 5f66 696c 6528 272f 6669  create_file('/fi
+00028800: 6c65 272c 2027 6461 7461 2729 0a20 2020  le', 'data').   
+00028810: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
+00028820: 7373 6572 7452 6169 7365 7328 4e6f 7441  ssertRaises(NotA
+00028830: 4469 7265 6374 6f72 7945 7272 6f72 2920  DirectoryError) 
+00028840: 6173 2063 6d3a 0a20 2020 2020 2020 2020  as cm:.         
+00028850: 2020 2073 656c 662e 6673 2e6c 6973 745f     self.fs.list_
+00028860: 6469 7228 272f 6669 6c65 2729 0a20 2020  dir('/file').   
+00028870: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00028880: 5472 7565 2827 2f66 696c 6527 2069 6e20  True('/file' in 
+00028890: 636d 2e65 7863 6570 7469 6f6e 2e61 7267  cm.exception.arg
+000288a0: 735b 305d 290a 0a20 2020 2064 6566 2074  s[0])..    def t
+000288b0: 6573 745f 6d61 6b65 6469 7228 7365 6c66  est_makedir(self
+000288c0: 293a 0a20 2020 2020 2020 2064 203d 2073  ):.        d = s
+000288d0: 656c 662e 6673 2e63 7265 6174 655f 6469  elf.fs.create_di
+000288e0: 7228 272f 6574 6327 290a 2020 2020 2020  r('/etc').      
+000288f0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00028900: 616c 2864 2e6e 616d 652c 2027 6574 6327  al(d.name, 'etc'
+00028910: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00028920: 7373 6572 7445 7175 616c 2864 2e70 6174  ssertEqual(d.pat
+00028930: 682c 2070 6174 686c 6962 2e50 7572 6550  h, pathlib.PureP
+00028940: 6f73 6978 5061 7468 2827 2f65 7463 2729  osixPath('/etc')
+00028950: 290a 2020 2020 2020 2020 6432 203d 2073  ).        d2 = s
+00028960: 656c 662e 6673 2e63 7265 6174 655f 6469  elf.fs.create_di
+00028970: 7228 272f 6574 632f 696e 6974 2e64 2729  r('/etc/init.d')
+00028980: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00028990: 7365 7274 4571 7561 6c28 6432 2e6e 616d  sertEqual(d2.nam
+000289a0: 652c 2027 696e 6974 2e64 2729 0a20 2020  e, 'init.d').   
+000289b0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+000289c0: 4571 7561 6c28 6432 2e70 6174 682c 2070  Equal(d2.path, p
+000289d0: 6174 686c 6962 2e50 7572 6550 6f73 6978  athlib.PurePosix
+000289e0: 5061 7468 2827 2f65 7463 2f69 6e69 742e  Path('/etc/init.
+000289f0: 6427 2929 0a0a 2020 2020 6465 6620 7465  d'))..    def te
+00028a00: 7374 5f6d 616b 6564 6972 5f66 6169 6c73  st_makedir_fails
+00028a10: 5f69 665f 616c 7265 6164 795f 6578 6973  _if_already_exis
+00028a20: 7473 2873 656c 6629 3a0a 2020 2020 2020  ts(self):.      
+00028a30: 2020 7365 6c66 2e66 732e 6372 6561 7465    self.fs.create
+00028a40: 5f64 6972 2827 2f65 7463 2729 0a20 2020  _dir('/etc').   
+00028a50: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
+00028a60: 7373 6572 7452 6169 7365 7328 4669 6c65  ssertRaises(File
+00028a70: 4578 6973 7473 4572 726f 7229 2061 7320  ExistsError) as 
+00028a80: 636d 3a0a 2020 2020 2020 2020 2020 2020  cm:.            
+00028a90: 7365 6c66 2e66 732e 6372 6561 7465 5f64  self.fs.create_d
+00028aa0: 6972 2827 2f65 7463 2729 0a20 2020 2020  ir('/etc').     
+00028ab0: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+00028ac0: 7565 2827 2f65 7463 2720 696e 2063 6d2e  ue('/etc' in cm.
+00028ad0: 6578 6365 7074 696f 6e2e 6172 6773 5b30  exception.args[0
+00028ae0: 5d29 0a0a 2020 2020 6465 6620 7465 7374  ])..    def test
+00028af0: 5f6d 616b 6564 6972 5f73 7563 6365 6564  _makedir_succeed
+00028b00: 735f 6966 5f61 6c72 6561 6479 5f65 7869  s_if_already_exi
+00028b10: 7374 735f 7768 656e 5f6d 616b 655f 7061  sts_when_make_pa
+00028b20: 7265 6e74 735f 7472 7565 2873 656c 6629  rents_true(self)
+00028b30: 3a0a 2020 2020 2020 2020 6431 203d 2073  :.        d1 = s
+00028b40: 656c 662e 6673 2e63 7265 6174 655f 6469  elf.fs.create_di
+00028b50: 7228 272f 6574 6327 290a 2020 2020 2020  r('/etc').      
+00028b60: 2020 6432 203d 2073 656c 662e 6673 2e63    d2 = self.fs.c
+00028b70: 7265 6174 655f 6469 7228 272f 6574 6327  reate_dir('/etc'
+00028b80: 2c20 6d61 6b65 5f70 6172 656e 7473 3d54  , make_parents=T
+00028b90: 7275 6529 0a20 2020 2020 2020 2073 656c  rue).        sel
+00028ba0: 662e 6173 7365 7274 4571 7561 6c28 6431  f.assertEqual(d1
+00028bb0: 2e70 6174 682c 2064 322e 7061 7468 290a  .path, d2.path).
+00028bc0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00028bd0: 6572 7445 7175 616c 2864 312e 6e61 6d65  ertEqual(d1.name
+00028be0: 2c20 6432 2e6e 616d 6529 0a0a 2020 2020  , d2.name)..    
+00028bf0: 6465 6620 7465 7374 5f6d 616b 6564 6972  def test_makedir
+00028c00: 5f66 6169 6c73 5f69 665f 7061 7265 6e74  _fails_if_parent
+00028c10: 5f64 6972 5f64 6f65 736e 745f 6578 6973  _dir_doesnt_exis
+00028c20: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+00028c30: 2077 6974 6820 7365 6c66 2e61 7373 6572   with self.asser
+00028c40: 7452 6169 7365 7328 4669 6c65 4e6f 7446  tRaises(FileNotF
+00028c50: 6f75 6e64 4572 726f 7229 2061 7320 636d  oundError) as cm
+00028c60: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00028c70: 6c66 2e66 732e 6372 6561 7465 5f64 6972  lf.fs.create_dir
+00028c80: 2827 2f65 7463 2f69 6e69 742e 6427 290a  ('/etc/init.d').
+00028c90: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00028ca0: 6572 7454 7275 6528 272f 6574 6327 2069  ertTrue('/etc' i
+00028cb0: 6e20 636d 2e65 7863 6570 7469 6f6e 2e61  n cm.exception.a
+00028cc0: 7267 735b 305d 290a 0a20 2020 2064 6566  rgs[0])..    def
+00028cd0: 2074 6573 745f 6d61 6b65 5f61 6e64 5f6c   test_make_and_l
+00028ce0: 6973 745f 6469 7265 6374 6f72 7928 7365  ist_directory(se
+00028cf0: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+00028d00: 662e 6673 2e63 7265 6174 655f 6469 7228  f.fs.create_dir(
+00028d10: 272f 6574 6327 290a 2020 2020 2020 2020  '/etc').        
+00028d20: 7365 6c66 2e66 732e 6372 6561 7465 5f64  self.fs.create_d
+00028d30: 6972 2827 2f76 6172 2729 0a20 2020 2020  ir('/var').     
+00028d40: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00028d50: 7561 6c28 0a20 2020 2020 2020 2020 2020  ual(.           
+00028d60: 207b 662e 7061 7468 2066 6f72 2066 2069   {f.path for f i
+00028d70: 6e20 7365 6c66 2e66 732e 6c69 7374 5f64  n self.fs.list_d
+00028d80: 6972 2827 2f27 297d 2c0a 2020 2020 2020  ir('/')},.      
+00028d90: 2020 2020 2020 7b70 6174 686c 6962 2e50        {pathlib.P
+00028da0: 7572 6550 6f73 6978 5061 7468 2827 2f65  urePosixPath('/e
+00028db0: 7463 2729 2c20 7061 7468 6c69 622e 5075  tc'), pathlib.Pu
+00028dc0: 7265 506f 7369 7850 6174 6828 272f 7661  rePosixPath('/va
+00028dd0: 7227 297d 290a 0a20 2020 2064 6566 2074  r')})..    def t
+00028de0: 6573 745f 6d61 6b65 5f64 6972 6563 746f  est_make_directo
+00028df0: 7279 5f72 6563 7572 7369 7665 6c79 2873  ry_recursively(s
+00028e00: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+00028e10: 6c66 2e66 732e 6372 6561 7465 5f64 6972  lf.fs.create_dir
+00028e20: 2827 2f65 7463 2f69 6e69 742e 6427 2c20  ('/etc/init.d', 
+00028e30: 6d61 6b65 5f70 6172 656e 7473 3d54 7275  make_parents=Tru
+00028e40: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
+00028e50: 6173 7365 7274 4571 7561 6c28 5b73 7472  assertEqual([str
+00028e60: 286f 2e70 6174 6829 2066 6f72 206f 2069  (o.path) for o i
+00028e70: 6e20 7365 6c66 2e66 732e 6c69 7374 5f64  n self.fs.list_d
+00028e80: 6972 2827 2f27 295d 2c20 5b27 2f65 7463  ir('/')], ['/etc
+00028e90: 275d 290a 2020 2020 2020 2020 7365 6c66  ']).        self
+00028ea0: 2e61 7373 6572 7445 7175 616c 285b 7374  .assertEqual([st
+00028eb0: 7228 6f2e 7061 7468 2920 666f 7220 6f20  r(o.path) for o 
+00028ec0: 696e 2073 656c 662e 6673 2e6c 6973 745f  in self.fs.list_
+00028ed0: 6469 7228 272f 6574 6327 295d 2c20 5b27  dir('/etc')], ['
+00028ee0: 2f65 7463 2f69 6e69 742e 6427 5d29 0a0a  /etc/init.d'])..
+00028ef0: 2020 2020 6465 6620 7465 7374 5f6d 616b      def test_mak
+00028f00: 6564 6972 5f70 6174 685f 6d75 7374 5f73  edir_path_must_s
+00028f10: 7461 7274 5f77 6974 685f 736c 6173 6828  tart_with_slash(
+00028f20: 7365 6c66 293a 0a20 2020 2020 2020 2077  self):.        w
+00028f30: 6974 6820 7365 6c66 2e61 7373 6572 7452  ith self.assertR
+00028f40: 6169 7365 7328 4e6f 6e41 6273 6f6c 7574  aises(NonAbsolut
+00028f50: 6550 6174 6845 7272 6f72 293a 0a20 2020  ePathError):.   
+00028f60: 2020 2020 2020 2020 2073 656c 662e 6673           self.fs
+00028f70: 2e63 7265 6174 655f 6469 7228 226e 6f73  .create_dir("nos
+00028f80: 6c61 7368 2229 0a0a 2020 2020 6465 6620  lash")..    def 
+00028f90: 7465 7374 5f63 7265 6174 655f 6669 6c65  test_create_file
+00028fa0: 5f66 6169 6c73 5f69 665f 7061 7265 6e74  _fails_if_parent
+00028fb0: 5f64 6972 5f64 6f65 736e 745f 6578 6973  _dir_doesnt_exis
+00028fc0: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+00028fd0: 2077 6974 6820 7365 6c66 2e61 7373 6572   with self.asser
+00028fe0: 7452 6169 7365 7328 4669 6c65 4e6f 7446  tRaises(FileNotF
+00028ff0: 6f75 6e64 4572 726f 7229 2061 7320 636d  oundError) as cm
+00029000: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00029010: 6c66 2e66 732e 6372 6561 7465 5f66 696c  lf.fs.create_fil
+00029020: 6528 272f 6574 632f 7061 7373 7764 272c  e('/etc/passwd',
+00029030: 2022 666f 6f22 290a 2020 2020 2020 2020   "foo").        
+00029040: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
+00029050: 272f 6574 6327 2069 6e20 636d 2e65 7863  '/etc' in cm.exc
+00029060: 6570 7469 6f6e 2e61 7267 735b 305d 290a  eption.args[0]).
+00029070: 0a20 2020 2064 6566 2074 6573 745f 6372  .    def test_cr
+00029080: 6561 7465 5f66 696c 655f 7375 6363 6565  eate_file_succee
+00029090: 6473 5f69 665f 7061 7265 6e74 5f64 6972  ds_if_parent_dir
+000290a0: 5f64 6f65 736e 745f 6578 6973 745f 7768  _doesnt_exist_wh
+000290b0: 656e 5f6d 616b 655f 6469 7273 5f74 7275  en_make_dirs_tru
+000290c0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000290d0: 2073 656c 662e 6673 2e63 7265 6174 655f   self.fs.create_
+000290e0: 6669 6c65 2827 2f74 6573 742f 7375 6264  file('/test/subd
+000290f0: 6972 2f74 6573 7466 696c 6527 2c20 2266  ir/testfile', "f
+00029100: 6f6f 222c 206d 616b 655f 6469 7273 3d54  oo", make_dirs=T
+00029110: 7275 6529 0a20 2020 2020 2020 2077 6974  rue).        wit
+00029120: 6820 7365 6c66 2e66 732e 6f70 656e 2827  h self.fs.open('
+00029130: 2f74 6573 742f 7375 6264 6972 2f74 6573  /test/subdir/tes
+00029140: 7466 696c 6527 2920 6173 2069 6e66 696c  tfile') as infil
+00029150: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00029160: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00029170: 696e 6669 6c65 2e72 6561 6428 292c 2027  infile.read(), '
+00029180: 666f 6f27 290a 0a20 2020 2064 6566 2074  foo')..    def t
+00029190: 6573 745f 6372 6561 7465 5f66 696c 655f  est_create_file_
+000291a0: 6672 6f6d 5f73 7472 2873 656c 6629 3a0a  from_str(self):.
+000291b0: 2020 2020 2020 2020 7365 6c66 2e66 732e          self.fs.
+000291c0: 6372 6561 7465 5f66 696c 6528 272f 7465  create_file('/te
+000291d0: 7374 272c 2022 666f 6f22 290a 2020 2020  st', "foo").    
+000291e0: 2020 2020 7769 7468 2073 656c 662e 6673      with self.fs
+000291f0: 2e6f 7065 6e28 272f 7465 7374 2729 2061  .open('/test') a
+00029200: 7320 696e 6669 6c65 3a0a 2020 2020 2020  s infile:.      
+00029210: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00029220: 7445 7175 616c 2869 6e66 696c 652e 7265  tEqual(infile.re
+00029230: 6164 2829 2c20 2766 6f6f 2729 0a0a 2020  ad(), 'foo')..  
+00029240: 2020 6465 6620 7465 7374 5f63 7265 6174    def test_creat
+00029250: 655f 6669 6c65 5f66 726f 6d5f 6279 7465  e_file_from_byte
+00029260: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+00029270: 2073 656c 662e 6673 2e63 7265 6174 655f   self.fs.create_
+00029280: 6669 6c65 2827 2f74 6573 7427 2c20 6222  file('/test', b"
+00029290: 666f 6f22 290a 2020 2020 2020 2020 7769  foo").        wi
+000292a0: 7468 2073 656c 662e 6673 2e6f 7065 6e28  th self.fs.open(
+000292b0: 272f 7465 7374 272c 2065 6e63 6f64 696e  '/test', encodin
+000292c0: 673d 4e6f 6e65 2920 6173 2069 6e66 696c  g=None) as infil
+000292d0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000292e0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000292f0: 696e 6669 6c65 2e72 6561 6428 292c 2062  infile.read(), b
+00029300: 2766 6f6f 2729 0a0a 2020 2020 6465 6620  'foo')..    def 
+00029310: 7465 7374 5f63 7265 6174 655f 6669 6c65  test_create_file
+00029320: 5f66 726f 6d5f 6669 6c65 7328 7365 6c66  _from_files(self
+00029330: 293a 0a20 2020 2020 2020 2064 6174 6120  ):.        data 
+00029340: 3d20 2266 6f6f 220a 0a20 2020 2020 2020  = "foo"..       
+00029350: 2073 696f 203d 2053 7472 696e 6749 4f28   sio = StringIO(
+00029360: 6461 7461 290a 2020 2020 2020 2020 7365  data).        se
+00029370: 6c66 2e66 732e 6372 6561 7465 5f66 696c  lf.fs.create_fil
+00029380: 6528 272f 7465 7374 272c 2073 696f 290a  e('/test', sio).
+00029390: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+000293a0: 662e 6673 2e6f 7065 6e28 272f 7465 7374  f.fs.open('/test
+000293b0: 2729 2061 7320 696e 6669 6c65 3a0a 2020  ') as infile:.  
+000293c0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000293d0: 7373 6572 7445 7175 616c 2869 6e66 696c  ssertEqual(infil
+000293e0: 652e 7265 6164 2829 2c20 2766 6f6f 2729  e.read(), 'foo')
+000293f0: 0a0a 2020 2020 2020 2020 6269 6f20 3d20  ..        bio = 
+00029400: 4279 7465 7349 4f28 6461 7461 2e65 6e63  BytesIO(data.enc
+00029410: 6f64 6528 2929 0a20 2020 2020 2020 2073  ode()).        s
+00029420: 656c 662e 6673 2e63 7265 6174 655f 6669  elf.fs.create_fi
+00029430: 6c65 2827 2f74 6573 7432 272c 2062 696f  le('/test2', bio
+00029440: 290a 2020 2020 2020 2020 7769 7468 2073  ).        with s
+00029450: 656c 662e 6673 2e6f 7065 6e28 272f 7465  elf.fs.open('/te
+00029460: 7374 3227 2920 6173 2069 6e66 696c 653a  st2') as infile:
+00029470: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00029480: 662e 6173 7365 7274 4571 7561 6c28 696e  f.assertEqual(in
+00029490: 6669 6c65 2e72 6561 6428 292c 2027 666f  file.read(), 'fo
+000294a0: 6f27 290a 0a20 2020 2064 6566 2074 6573  o')..    def tes
+000294b0: 745f 6372 6561 7465 5f61 6e64 5f72 6561  t_create_and_rea
+000294c0: 645f 7769 7468 5f64 6966 6665 7265 6e74  d_with_different
+000294d0: 5f65 6e63 6f64 696e 6773 2873 656c 6629  _encodings(self)
+000294e0: 3a0a 2020 2020 2020 2020 2320 7772 6974  :.        # writ
+000294f0: 6520 7374 722c 2072 6561 6420 6173 2075  e str, read as u
+00029500: 7466 2d38 2062 7974 6573 0a20 2020 2020  tf-8 bytes.     
+00029510: 2020 2073 656c 662e 6673 2e63 7265 6174     self.fs.creat
+00029520: 655f 6669 6c65 2827 2f74 6573 7427 2c20  e_file('/test', 
+00029530: 2266 6f6f 2229 0a20 2020 2020 2020 2077  "foo").        w
+00029540: 6974 6820 7365 6c66 2e66 732e 6f70 656e  ith self.fs.open
+00029550: 2827 2f74 6573 7427 2c20 656e 636f 6469  ('/test', encodi
+00029560: 6e67 3d4e 6f6e 6529 2061 7320 696e 6669  ng=None) as infi
+00029570: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+00029580: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00029590: 2869 6e66 696c 652e 7265 6164 2829 2c20  (infile.read(), 
+000295a0: 6227 666f 6f27 290a 0a20 2020 2020 2020  b'foo')..       
+000295b0: 2023 2077 7269 7465 2062 7974 6573 2c20   # write bytes, 
+000295c0: 7265 6164 2061 7320 7574 662d 382d 6465  read as utf-8-de
+000295d0: 636f 6465 6420 7374 720a 2020 2020 2020  coded str.      
+000295e0: 2020 6461 7461 203d 2022 e697 a5e6 9cac    data = "......
+000295f0: e8aa 9e22 2020 2320 4a61 7061 6e65 7365  ..."  # Japanese
+00029600: 2066 6f72 2022 4a61 7061 6e65 7365 220a   for "Japanese".
+00029610: 2020 2020 2020 2020 7365 6c66 2e66 732e          self.fs.
+00029620: 6372 6561 7465 5f66 696c 6528 272f 7465  create_file('/te
+00029630: 7374 3227 2c20 6461 7461 2e65 6e63 6f64  st2', data.encod
+00029640: 6528 2775 7466 2d38 2729 290a 2020 2020  e('utf-8')).    
+00029650: 2020 2020 7769 7468 2073 656c 662e 6673      with self.fs
+00029660: 2e6f 7065 6e28 272f 7465 7374 3227 2920  .open('/test2') 
+00029670: 6173 2069 6e66 696c 653a 2020 2020 2020  as infile:      
+00029680: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00029690: 496d 706c 6963 6974 2075 7466 2d38 2072  Implicit utf-8 r
+000296a0: 6561 640a 2020 2020 2020 2020 2020 2020  ead.            
+000296b0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000296c0: 2869 6e66 696c 652e 7265 6164 2829 2c20  (infile.read(), 
+000296d0: 6461 7461 290a 2020 2020 2020 2020 7769  data).        wi
+000296e0: 7468 2073 656c 662e 6673 2e6f 7065 6e28  th self.fs.open(
+000296f0: 272f 7465 7374 3227 2c20 656e 636f 6469  '/test2', encodi
+00029700: 6e67 3d27 7574 662d 3827 2920 6173 2069  ng='utf-8') as i
+00029710: 6e66 696c 653a 2020 2320 4578 706c 6963  nfile:  # Explic
+00029720: 6974 2075 7466 2d38 2072 6561 640a 2020  it utf-8 read.  
+00029730: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00029740: 7373 6572 7445 7175 616c 2869 6e66 696c  ssertEqual(infil
+00029750: 652e 7265 6164 2829 2c20 6461 7461 290a  e.read(), data).
+00029760: 0a20 2020 2064 6566 2074 6573 745f 6f70  .    def test_op
+00029770: 656e 5f64 6972 6563 746f 7279 5f66 6169  en_directory_fai
+00029780: 6c73 2873 656c 6629 3a0a 2020 2020 2020  ls(self):.      
+00029790: 2020 7365 6c66 2e66 732e 6372 6561 7465    self.fs.create
+000297a0: 5f64 6972 2827 2f64 6972 3127 290a 2020  _dir('/dir1').  
+000297b0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+000297c0: 6173 7365 7274 5261 6973 6573 2849 7341  assertRaises(IsA
+000297d0: 4469 7265 6374 6f72 7945 7272 6f72 2920  DirectoryError) 
+000297e0: 6173 2063 6d3a 0a20 2020 2020 2020 2020  as cm:.         
+000297f0: 2020 2073 656c 662e 6673 2e6f 7065 6e28     self.fs.open(
+00029800: 272f 6469 7231 2729 0a20 2020 2020 2020  '/dir1').       
+00029810: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00029820: 6c28 636d 2e65 7863 6570 7469 6f6e 2e61  l(cm.exception.a
+00029830: 7267 735b 305d 2c20 272f 6469 7231 2729  rgs[0], '/dir1')
+00029840: 0a0a 2020 2020 6465 6620 7465 7374 5f64  ..    def test_d
+00029850: 656c 6574 655f 6669 6c65 2873 656c 6629  elete_file(self)
+00029860: 3a0a 2020 2020 2020 2020 7365 6c66 2e66  :.        self.f
+00029870: 732e 6372 6561 7465 5f66 696c 6528 272f  s.create_file('/
+00029880: 7465 7374 272c 2022 666f 6f22 290a 2020  test', "foo").  
+00029890: 2020 2020 2020 7365 6c66 2e66 732e 6465        self.fs.de
+000298a0: 6c65 7465 5f70 6174 6828 272f 7465 7374  lete_path('/test
+000298b0: 2729 0a20 2020 2020 2020 2077 6974 6820  ').        with 
+000298c0: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
+000298d0: 7328 4669 6c65 4e6f 7446 6f75 6e64 4572  s(FileNotFoundEr
+000298e0: 726f 7229 2061 7320 636d 3a0a 2020 2020  ror) as cm:.    
+000298f0: 2020 2020 2020 2020 7365 6c66 2e66 732e          self.fs.
+00029900: 6765 745f 7061 7468 2827 2f74 6573 7427  get_path('/test'
+00029910: 290a 0a20 2020 2020 2020 2023 2044 656c  )..        # Del
+00029920: 6574 696e 6720 6465 6c65 7465 6420 6669  eting deleted fi
+00029930: 6c65 7320 7368 6f75 6c64 2066 6169 6c20  les should fail 
+00029940: 6173 2077 656c 6c0a 2020 2020 2020 2020  as well.        
+00029950: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
+00029960: 5261 6973 6573 2846 696c 654e 6f74 466f  Raises(FileNotFo
+00029970: 756e 6445 7272 6f72 2920 6173 2063 6d3a  undError) as cm:
+00029980: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00029990: 662e 6673 2e64 656c 6574 655f 7061 7468  f.fs.delete_path
+000299a0: 2827 2f74 6573 7427 290a 2020 2020 2020  ('/test').      
+000299b0: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+000299c0: 6528 272f 7465 7374 2720 696e 2063 6d2e  e('/test' in cm.
+000299d0: 6578 6365 7074 696f 6e2e 6172 6773 5b30  exception.args[0
+000299e0: 5d29 0a0a 2020 2020 6465 6620 7465 7374  ])..    def test
+000299f0: 5f63 7265 6174 655f 6469 725f 7769 7468  _create_dir_with
+00029a00: 5f65 7874 7261 5f61 7267 7328 7365 6c66  _extra_args(self
+00029a10: 293a 0a20 2020 2020 2020 2064 203d 2073  ):.        d = s
+00029a20: 656c 662e 6673 2e63 7265 6174 655f 6469  elf.fs.create_di
+00029a30: 7228 272f 6469 7231 2729 0a20 2020 2020  r('/dir1').     
+00029a40: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00029a50: 7561 6c28 642e 6b77 6172 6773 2c20 7b7d  ual(d.kwargs, {}
+00029a60: 290a 0a20 2020 2020 2020 2064 203d 2073  )..        d = s
+00029a70: 656c 662e 6673 2e63 7265 6174 655f 6469  elf.fs.create_di
+00029a80: 7228 0a20 2020 2020 2020 2020 2020 2027  r(.            '
+00029a90: 2f64 6972 3227 2c20 7065 726d 6973 7369  /dir2', permissi
+00029aa0: 6f6e 733d 306f 3730 302c 2075 7365 723d  ons=0o700, user=
+00029ab0: 2775 6275 6e74 7527 2c20 7573 6572 5f69  'ubuntu', user_i
+00029ac0: 643d 3130 3030 2c20 6772 6f75 703d 2777  d=1000, group='w
+00029ad0: 7777 2d64 6174 6127 2c20 6772 6f75 705f  ww-data', group_
+00029ae0: 6964 3d33 3329 0a20 2020 2020 2020 2073  id=33).        s
+00029af0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00029b00: 642e 6b77 6172 6773 2c20 7b0a 2020 2020  d.kwargs, {.    
+00029b10: 2020 2020 2020 2020 2770 6572 6d69 7373          'permiss
+00029b20: 696f 6e73 273a 2030 6f37 3030 2c0a 2020  ions': 0o700,.  
+00029b30: 2020 2020 2020 2020 2020 2775 7365 7227            'user'
+00029b40: 3a20 2775 6275 6e74 7527 2c0a 2020 2020  : 'ubuntu',.    
+00029b50: 2020 2020 2020 2020 2775 7365 725f 6964          'user_id
+00029b60: 273a 2031 3030 302c 0a20 2020 2020 2020  ': 1000,.       
+00029b70: 2020 2020 2027 6772 6f75 7027 3a20 2777       'group': 'w
+00029b80: 7777 2d64 6174 6127 2c0a 2020 2020 2020  ww-data',.      
+00029b90: 2020 2020 2020 2767 726f 7570 5f69 6427        'group_id'
+00029ba0: 3a20 3333 2c0a 2020 2020 2020 2020 7d29  : 33,.        })
+00029bb0: 0a0a 2020 2020 6465 6620 7465 7374 5f63  ..    def test_c
+00029bc0: 7265 6174 655f 6669 6c65 5f77 6974 685f  reate_file_with_
+00029bd0: 6578 7472 615f 6172 6773 2873 656c 6629  extra_args(self)
+00029be0: 3a0a 2020 2020 2020 2020 6620 3d20 7365  :.        f = se
+00029bf0: 6c66 2e66 732e 6372 6561 7465 5f66 696c  lf.fs.create_fil
+00029c00: 6528 272f 6669 6c65 3127 2c20 2764 6174  e('/file1', 'dat
+00029c10: 6127 290a 2020 2020 2020 2020 7365 6c66  a').        self
+00029c20: 2e61 7373 6572 7445 7175 616c 2866 2e6b  .assertEqual(f.k
+00029c30: 7761 7267 732c 207b 7d29 0a0a 2020 2020  wargs, {})..    
+00029c40: 2020 2020 6620 3d20 7365 6c66 2e66 732e      f = self.fs.
+00029c50: 6372 6561 7465 5f66 696c 6528 0a20 2020  create_file(.   
+00029c60: 2020 2020 2020 2020 2027 2f66 696c 6532           '/file2
+00029c70: 272c 2027 6461 7461 272c 0a20 2020 2020  ', 'data',.     
+00029c80: 2020 2020 2020 2070 6572 6d69 7373 696f         permissio
+00029c90: 6e73 3d30 6f37 3534 2c20 7573 6572 3d27  ns=0o754, user='
+00029ca0: 7562 756e 7475 272c 2075 7365 725f 6964  ubuntu', user_id
+00029cb0: 3d31 3030 302c 2067 726f 7570 3d27 7777  =1000, group='ww
+00029cc0: 772d 6461 7461 272c 2067 726f 7570 5f69  w-data', group_i
+00029cd0: 643d 3333 290a 2020 2020 2020 2020 7365  d=33).        se
+00029ce0: 6c66 2e61 7373 6572 7445 7175 616c 2866  lf.assertEqual(f
+00029cf0: 2e6b 7761 7267 732c 207b 0a20 2020 2020  .kwargs, {.     
+00029d00: 2020 2020 2020 2027 7065 726d 6973 7369         'permissi
+00029d10: 6f6e 7327 3a20 306f 3735 342c 0a20 2020  ons': 0o754,.   
+00029d20: 2020 2020 2020 2020 2027 7573 6572 273a           'user':
+00029d30: 2027 7562 756e 7475 272c 0a20 2020 2020   'ubuntu',.     
+00029d40: 2020 2020 2020 2027 7573 6572 5f69 6427         'user_id'
+00029d50: 3a20 3130 3030 2c0a 2020 2020 2020 2020  : 1000,.        
+00029d60: 2020 2020 2767 726f 7570 273a 2027 7777      'group': 'ww
+00029d70: 772d 6461 7461 272c 0a20 2020 2020 2020  w-data',.       
+00029d80: 2020 2020 2027 6772 6f75 705f 6964 273a       'group_id':
+00029d90: 2033 332c 0a20 2020 2020 2020 207d 290a   33,.        }).
+00029da0: 0a20 2020 2064 6566 2074 6573 745f 6765  .    def test_ge
+00029db0: 7461 7474 7228 7365 6c66 293a 0a20 2020  tattr(self):.   
+00029dc0: 2020 2020 2073 656c 662e 6673 2e63 7265       self.fs.cre
+00029dd0: 6174 655f 6469 7228 272f 6574 632f 696e  ate_dir('/etc/in
+00029de0: 6974 2e64 272c 206d 616b 655f 7061 7265  it.d', make_pare
+00029df0: 6e74 733d 5472 7565 290a 0a20 2020 2020  nts=True)..     
+00029e00: 2020 2023 2042 7920 7061 7468 0a20 2020     # By path.   
+00029e10: 2020 2020 206f 203d 2073 656c 662e 6673       o = self.fs
+00029e20: 2e67 6574 5f70 6174 6828 7061 7468 6c69  .get_path(pathli
+00029e30: 622e 5075 7265 506f 7369 7850 6174 6828  b.PurePosixPath(
+00029e40: 272f 6574 632f 696e 6974 2e64 2729 290a  '/etc/init.d')).
+00029e50: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00029e60: 6572 7449 7349 6e73 7461 6e63 6528 6f2c  ertIsInstance(o,
+00029e70: 205f 4469 7265 6374 6f72 7929 0a20 2020   _Directory).   
+00029e80: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00029e90: 4571 7561 6c28 6f2e 7061 7468 2c20 7061  Equal(o.path, pa
+00029ea0: 7468 6c69 622e 5075 7265 506f 7369 7850  thlib.PurePosixP
+00029eb0: 6174 6828 272f 6574 632f 696e 6974 2e64  ath('/etc/init.d
+00029ec0: 2729 290a 0a20 2020 2020 2020 2023 2042  '))..        # B
+00029ed0: 7920 7374 720a 2020 2020 2020 2020 6f20  y str.        o 
+00029ee0: 3d20 7365 6c66 2e66 732e 6765 745f 7061  = self.fs.get_pa
+00029ef0: 7468 2827 2f65 7463 2f69 6e69 742e 6427  th('/etc/init.d'
+00029f00: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00029f10: 7373 6572 7449 7349 6e73 7461 6e63 6528  ssertIsInstance(
+00029f20: 6f2c 205f 4469 7265 6374 6f72 7929 0a20  o, _Directory). 
+00029f30: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00029f40: 7274 4571 7561 6c28 6f2e 7061 7468 2c20  rtEqual(o.path, 
+00029f50: 7061 7468 6c69 622e 5075 7265 506f 7369  pathlib.PurePosi
+00029f60: 7850 6174 6828 272f 6574 632f 696e 6974  xPath('/etc/init
+00029f70: 2e64 2729 290a 0a20 2020 2064 6566 2074  .d'))..    def t
+00029f80: 6573 745f 6765 7461 7474 725f 6669 6c65  est_getattr_file
+00029f90: 5f6e 6f74 5f66 6f75 6e64 2873 656c 6629  _not_found(self)
+00029fa0: 3a0a 2020 2020 2020 2020 2320 4172 6775  :.        # Argu
+00029fb0: 6162 6c79 2074 6869 7320 636f 756c 6420  ably this could 
+00029fc0: 6265 2061 204b 6579 4572 726f 7220 6769  be a KeyError gi
+00029fd0: 7665 6e20 7468 6520 6469 6374 696f 6e61  ven the dictiona
+00029fe0: 7279 2d73 7479 6c65 2061 6363 6573 732e  ry-style access.
+00029ff0: 0a20 2020 2020 2020 2023 2048 6f77 6576  .        # Howev
+0002a000: 6572 2c20 4669 6c65 4e6f 7446 6f75 6e64  er, FileNotFound
+0002a010: 4572 726f 7220 7365 656d 7320 6d6f 7265  Error seems more
+0002a020: 2061 7070 726f 7072 6961 7465 2066 6f72   appropriate for
+0002a030: 2061 2066 696c 6573 7973 7465 6d2c 2061   a filesystem, a
+0002a040: 6e64 2069 740a 2020 2020 2020 2020 2320  nd it.        # 
+0002a050: 6769 7665 7320 6120 636c 6f73 6572 2073  gives a closer s
+0002a060: 656d 616e 7469 6320 6665 656c 696e 672c  emantic feeling,
+0002a070: 2069 6e20 6d79 206f 7069 6e69 6f6e 2e0a   in my opinion..
+0002a080: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
+0002a090: 662e 6173 7365 7274 5261 6973 6573 2846  f.assertRaises(F
+0002a0a0: 696c 654e 6f74 466f 756e 6445 7272 6f72  ileNotFoundError
+0002a0b0: 2920 6173 2063 6d3a 0a20 2020 2020 2020  ) as cm:.       
+0002a0c0: 2020 2020 2073 656c 662e 6673 2e67 6574       self.fs.get
+0002a0d0: 5f70 6174 6828 272f 6e6f 6e65 7869 7374  _path('/nonexist
+0002a0e0: 656e 745f 6669 6c65 2729 0a20 2020 2020  ent_file').     
+0002a0f0: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+0002a100: 7565 2827 2f6e 6f6e 6578 6973 7465 6e74  ue('/nonexistent
+0002a110: 5f66 696c 6527 2069 6e20 636d 2e65 7863  _file' in cm.exc
+0002a120: 6570 7469 6f6e 2e61 7267 735b 305d 290a  eption.args[0]).
+0002a130: 0a0a 636c 6173 7320 5465 7374 5465 7374  ..class TestTest
+0002a140: 696e 6746 696c 6573 7973 7465 6d28 4765  ingFilesystem(Ge
+0002a150: 6e65 7269 6354 6573 7469 6e67 4669 6c65  nericTestingFile
+0002a160: 7379 7374 656d 5465 7374 732c 2075 6e69  systemTests, uni
+0002a170: 7474 6573 742e 5465 7374 4361 7365 293a  ttest.TestCase):
+0002a180: 0a20 2020 2064 6566 2073 6574 5570 2873  .    def setUp(s
+0002a190: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+0002a1a0: 6c66 2e66 7320 3d20 5f54 6573 7469 6e67  lf.fs = _Testing
+0002a1b0: 4669 6c65 7379 7374 656d 2829 0a0a 2020  Filesystem()..  
+0002a1c0: 2020 6465 6620 7465 7374 5f73 746f 7261    def test_stora
+0002a1d0: 6765 5f6d 6f75 6e74 2873 656c 6629 3a0a  ge_mount(self):.
+0002a1e0: 2020 2020 2020 2020 746d 7064 6972 203d          tmpdir =
+0002a1f0: 2074 656d 7066 696c 652e 5465 6d70 6f72   tempfile.Tempor
+0002a200: 6172 7944 6972 6563 746f 7279 2829 0a20  aryDirectory(). 
+0002a210: 2020 2020 2020 2073 656c 662e 6673 2e61         self.fs.a
+0002a220: 6464 5f6d 6f75 6e74 2827 666f 6f27 2c20  dd_mount('foo', 
+0002a230: 272f 666f 6f27 2c20 746d 7064 6972 2e6e  '/foo', tmpdir.n
+0002a240: 616d 6529 0a20 2020 2020 2020 2073 656c  ame).        sel
+0002a250: 662e 6673 2e63 7265 6174 655f 6669 6c65  f.fs.create_file
+0002a260: 2827 2f66 6f6f 2f62 6172 2f62 617a 2e74  ('/foo/bar/baz.t
+0002a270: 7874 272c 2027 7175 7578 272c 206d 616b  xt', 'quux', mak
+0002a280: 655f 6469 7273 3d54 7275 6529 0a0a 2020  e_dirs=True)..  
+0002a290: 2020 2020 2020 746d 7070 6174 6820 3d20        tmppath = 
+0002a2a0: 6f73 2e70 6174 682e 6a6f 696e 2874 6d70  os.path.join(tmp
+0002a2b0: 6469 722e 6e61 6d65 2c20 2762 6172 2f62  dir.name, 'bar/b
+0002a2c0: 617a 2e74 7874 2729 0a20 2020 2020 2020  az.txt').       
+0002a2d0: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+0002a2e0: 286f 732e 7061 7468 2e65 7869 7374 7328  (os.path.exists(
+0002a2f0: 746d 7070 6174 6829 290a 2020 2020 2020  tmppath)).      
+0002a300: 2020 7769 7468 206f 7065 6e28 746d 7070    with open(tmpp
+0002a310: 6174 6829 2061 7320 663a 0a20 2020 2020  ath) as f:.     
+0002a320: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0002a330: 7274 4571 7561 6c28 662e 7265 6164 2829  rtEqual(f.read()
+0002a340: 2c20 2771 7575 7827 290a 0a0a 636c 6173  , 'quux')...clas
+0002a350: 7320 5465 7374 5465 7374 696e 6753 746f  s TestTestingSto
+0002a360: 7261 6765 4d6f 756e 7428 4765 6e65 7269  rageMount(Generi
+0002a370: 6354 6573 7469 6e67 4669 6c65 7379 7374  cTestingFilesyst
+0002a380: 656d 5465 7374 732c 2075 6e69 7474 6573  emTests, unittes
+0002a390: 742e 5465 7374 4361 7365 293a 0a20 2020  t.TestCase):.   
+0002a3a0: 2064 6566 2073 6574 5570 2873 656c 6629   def setUp(self)
+0002a3b0: 3a0a 2020 2020 2020 2020 7365 6c66 2e74  :.        self.t
+0002a3c0: 6d70 203d 2074 656d 7066 696c 652e 5465  mp = tempfile.Te
+0002a3d0: 6d70 6f72 6172 7944 6972 6563 746f 7279  mporaryDirectory
+0002a3e0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0002a3f0: 6164 6443 6c65 616e 7570 2873 656c 662e  addCleanup(self.
+0002a400: 746d 702e 636c 6561 6e75 7029 0a20 2020  tmp.cleanup).   
+0002a410: 2020 2020 2073 656c 662e 6673 203d 205f       self.fs = _
+0002a420: 5465 7374 696e 6753 746f 7261 6765 4d6f  TestingStorageMo
+0002a430: 756e 7428 272f 272c 2070 6174 686c 6962  unt('/', pathlib
+0002a440: 2e50 6174 6828 7365 6c66 2e74 6d70 2e6e  .Path(self.tmp.n
+0002a450: 616d 6529 290a 0a0a 636c 6173 7320 5465  ame))...class Te
+0002a460: 7374 5065 6262 6c65 5374 6f72 6167 6541  stPebbleStorageA
+0002a470: 5049 7355 7369 6e67 4d6f 636b 7328 0a20  PIsUsingMocks(. 
+0002a480: 2020 2020 2020 2075 6e69 7474 6573 742e         unittest.
+0002a490: 5465 7374 4361 7365 2c0a 2020 2020 2020  TestCase,.      
+0002a4a0: 2020 5f54 6573 7469 6e67 5065 6262 6c65    _TestingPebble
+0002a4b0: 436c 6965 6e74 4d69 7869 6e2c 0a20 2020  ClientMixin,.   
+0002a4c0: 2020 2020 205f 5065 6262 6c65 5374 6f72       _PebbleStor
+0002a4d0: 6167 6541 5049 7354 6573 744d 6978 696e  ageAPIsTestMixin
+0002a4e0: 293a 0a20 2020 2064 6566 2073 6574 5570  ):.    def setUp
+0002a4f0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0002a500: 7365 6c66 2e70 7265 6669 7820 3d20 272f  self.prefix = '/
+0002a510: 7072 6566 6978 270a 2020 2020 2020 2020  prefix'.        
+0002a520: 7365 6c66 2e63 6c69 656e 7420 3d20 7365  self.client = se
+0002a530: 6c66 2e67 6574 5f74 6573 7469 6e67 5f63  lf.get_testing_c
+0002a540: 6c69 656e 7428 290a 2020 2020 2020 2020  lient().        
+0002a550: 6966 2073 656c 662e 7072 6566 6978 3a0a  if self.prefix:.
+0002a560: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0002a570: 2e63 6c69 656e 742e 6d61 6b65 5f64 6972  .client.make_dir
+0002a580: 2873 656c 662e 7072 6566 6978 2c20 6d61  (self.prefix, ma
+0002a590: 6b65 5f70 6172 656e 7473 3d54 7275 6529  ke_parents=True)
+0002a5a0: 0a0a 2020 2020 4075 6e69 7474 6573 742e  ..    @unittest.
+0002a5b0: 736b 6970 556e 6c65 7373 2869 735f 6c69  skipUnless(is_li
+0002a5c0: 6e75 782c 2027 5065 6262 6c65 2072 756e  nux, 'Pebble run
+0002a5d0: 7320 6f6e 204c 696e 7578 2729 0a20 2020  s on Linux').   
+0002a5e0: 2064 6566 2074 6573 745f 636f 6e74 6169   def test_contai
+0002a5f0: 6e65 725f 7374 6f72 6167 655f 6d6f 756e  ner_storage_moun
+0002a600: 7473 2873 656c 6629 3a0a 2020 2020 2020  ts(self):.      
+0002a610: 2020 6861 726e 6573 7320 3d20 6f70 732e    harness = ops.
+0002a620: 7465 7374 696e 672e 4861 726e 6573 7328  testing.Harness(
+0002a630: 6f70 732e 4368 6172 6d42 6173 652c 206d  ops.CharmBase, m
+0002a640: 6574 613d 2727 270a 2020 2020 2020 2020  eta='''.        
+0002a650: 2020 2020 6e61 6d65 3a20 7465 7374 2d61      name: test-a
+0002a660: 7070 0a20 2020 2020 2020 2020 2020 2063  pp.            c
+0002a670: 6f6e 7461 696e 6572 733a 0a20 2020 2020  ontainers:.     
+0002a680: 2020 2020 2020 2020 2020 2063 313a 0a20             c1:. 
+0002a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a6a0: 2020 206d 6f75 6e74 733a 0a20 2020 2020     mounts:.     
+0002a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a6c0: 2020 202d 2073 746f 7261 6765 3a20 7374     - storage: st
+0002a6d0: 6f72 6531 0a20 2020 2020 2020 2020 2020  ore1.           
+0002a6e0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0002a6f0: 6f63 6174 696f 6e3a 202f 6d6f 756e 7473  ocation: /mounts
+0002a700: 2f66 6f6f 0a20 2020 2020 2020 2020 2020  /foo.           
+0002a710: 2020 2020 2063 323a 0a20 2020 2020 2020       c2:.       
+0002a720: 2020 2020 2020 2020 2020 2020 206d 6f75               mou
+0002a730: 6e74 733a 0a20 2020 2020 2020 2020 2020  nts:.           
+0002a740: 2020 2020 2020 2020 2020 2020 202d 2073               - s
+0002a750: 746f 7261 6765 3a20 7374 6f72 6532 0a20  torage: store2. 
+0002a760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a770: 2020 2020 2020 2020 206c 6f63 6174 696f           locatio
+0002a780: 6e3a 202f 6d6f 756e 7473 2f66 6f6f 0a20  n: /mounts/foo. 
+0002a790: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0002a7a0: 333a 0a20 2020 2020 2020 2020 2020 2020  3:.             
+0002a7b0: 2020 2020 2020 206d 6f75 6e74 733a 0a20         mounts:. 
+0002a7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a7d0: 2020 2020 2020 202d 2073 746f 7261 6765         - storage
+0002a7e0: 3a20 7374 6f72 6531 0a20 2020 2020 2020  : store1.       
+0002a7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002a800: 2020 206c 6f63 6174 696f 6e3a 202f 6d6f     location: /mo
+0002a810: 756e 7473 2f62 6172 0a20 2020 2020 2020  unts/bar.       
+0002a820: 2020 2020 2073 746f 7261 6765 3a0a 2020       storage:.  
+0002a830: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0002a840: 6f72 6531 3a0a 2020 2020 2020 2020 2020  ore1:.          
+0002a850: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
+0002a860: 6669 6c65 7379 7374 656d 0a20 2020 2020  filesystem.     
+0002a870: 2020 2020 2020 2020 2020 2073 746f 7265             store
+0002a880: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
+0002a890: 2020 2020 2020 2074 7970 653a 2066 696c         type: fil
+0002a8a0: 6573 7973 7465 6d0a 2020 2020 2020 2020  esystem.        
+0002a8b0: 2020 2020 2727 2729 0a20 2020 2020 2020      ''').       
+0002a8c0: 2073 656c 662e 6164 6443 6c65 616e 7570   self.addCleanup
+0002a8d0: 2868 6172 6e65 7373 2e63 6c65 616e 7570  (harness.cleanup
+0002a8e0: 290a 0a20 2020 2020 2020 2073 746f 7265  )..        store
+0002a8f0: 5f69 6420 3d20 6861 726e 6573 732e 6164  _id = harness.ad
+0002a900: 645f 7374 6f72 6167 6528 2773 746f 7265  d_storage('store
+0002a910: 3127 295b 305d 0a20 2020 2020 2020 2068  1')[0].        h
+0002a920: 6172 6e65 7373 2e61 7474 6163 685f 7374  arness.attach_st
+0002a930: 6f72 6167 6528 7374 6f72 655f 6964 290a  orage(store_id).
 0002a940: 0a20 2020 2020 2020 2068 6172 6e65 7373  .        harness
-0002a950: 2e73 6574 5f63 616e 5f63 6f6e 6e65 6374  .set_can_connect
-0002a960: 2827 6331 272c 2054 7275 6529 0a20 2020  ('c1', True).   
-0002a970: 2020 2020 2068 6172 6e65 7373 2e73 6574       harness.set
-0002a980: 5f63 616e 5f63 6f6e 6e65 6374 2827 6332  _can_connect('c2
-0002a990: 272c 2054 7275 6529 0a20 2020 2020 2020  ', True).       
-0002a9a0: 2068 6172 6e65 7373 2e73 6574 5f63 616e   harness.set_can
-0002a9b0: 5f63 6f6e 6e65 6374 2827 6333 272c 2054  _connect('c3', T
-0002a9c0: 7275 6529 0a0a 2020 2020 2020 2020 2320  rue)..        # 
-0002a9d0: 7075 7368 2066 696c 6520 746f 2063 3120  push file to c1 
-0002a9e0: 7374 6f72 6167 6520 6d6f 756e 742c 2063  storage mount, c
-0002a9f0: 6865 636b 2074 6861 7420 7765 2063 616e  heck that we can
-0002aa00: 2073 6565 2069 7420 696e 2063 6861 726d   see it in charm
-0002aa10: 2063 6f6e 7461 696e 6572 2073 746f 7261   container stora
-0002aa20: 6765 2070 6174 682e 0a20 2020 2020 2020  ge path..       
-0002aa30: 2063 3120 3d20 6861 726e 6573 732e 6d6f   c1 = harness.mo
-0002aa40: 6465 6c2e 756e 6974 2e67 6574 5f63 6f6e  del.unit.get_con
-0002aa50: 7461 696e 6572 2827 6331 2729 0a20 2020  tainer('c1').   
-0002aa60: 2020 2020 2063 315f 666e 616d 6520 3d20       c1_fname = 
-0002aa70: 2766 6f6f 2e74 7874 270a 2020 2020 2020  'foo.txt'.      
-0002aa80: 2020 6331 5f66 7061 7468 203d 206f 732e    c1_fpath = os.
-0002aa90: 7061 7468 2e6a 6f69 6e28 272f 6d6f 756e  path.join('/moun
-0002aaa0: 7473 2f66 6f6f 272c 2063 315f 666e 616d  ts/foo', c1_fnam
-0002aab0: 6529 0a20 2020 2020 2020 2063 312e 7075  e).        c1.pu
-0002aac0: 7368 2863 315f 6670 6174 682c 2027 3432  sh(c1_fpath, '42
-0002aad0: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-0002aae0: 6173 7365 7274 5472 7565 2863 312e 6578  assertTrue(c1.ex
-0002aaf0: 6973 7473 2863 315f 6670 6174 6829 290a  ists(c1_fpath)).
-0002ab00: 2020 2020 2020 2020 6670 6174 6820 3d20          fpath = 
-0002ab10: 6f73 2e70 6174 682e 6a6f 696e 2873 7472  os.path.join(str
-0002ab20: 2868 6172 6e65 7373 2e6d 6f64 656c 2e73  (harness.model.s
-0002ab30: 746f 7261 6765 735b 2773 746f 7265 3127  torages['store1'
-0002ab40: 5d5b 305d 2e6c 6f63 6174 696f 6e29 2c20  ][0].location), 
-0002ab50: 2766 6f6f 2e74 7874 2729 0a20 2020 2020  'foo.txt').     
-0002ab60: 2020 2077 6974 6820 6f70 656e 2866 7061     with open(fpa
-0002ab70: 7468 2920 6173 2066 3a0a 2020 2020 2020  th) as f:.      
-0002ab80: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0002ab90: 7445 7175 616c 2827 3432 272c 2066 2e72  tEqual('42', f.r
-0002aba0: 6561 6428 2929 0a0a 2020 2020 2020 2020  ead())..        
-0002abb0: 2320 6368 6563 6b20 7468 6174 2074 6865  # check that the
-0002abc0: 2066 696c 6520 6973 206e 6f74 2076 6973   file is not vis
-0002abd0: 6962 6c65 2069 6e20 6332 2077 6869 6368  ible in c2 which
-0002abe0: 2068 6173 2061 2064 6966 6665 7265 6e74   has a different
-0002abf0: 2073 746f 7261 6765 206d 6f75 6e74 0a20   storage mount. 
-0002ac00: 2020 2020 2020 2063 3220 3d20 6861 726e         c2 = harn
-0002ac10: 6573 732e 6d6f 6465 6c2e 756e 6974 2e67  ess.model.unit.g
-0002ac20: 6574 5f63 6f6e 7461 696e 6572 2827 6332  et_container('c2
-0002ac30: 2729 0a20 2020 2020 2020 2063 325f 6670  ').        c2_fp
-0002ac40: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
-0002ac50: 696e 2827 2f6d 6f75 6e74 732f 666f 6f27  in('/mounts/foo'
-0002ac60: 2c20 6331 5f66 6e61 6d65 290a 2020 2020  , c1_fname).    
-0002ac70: 2020 2020 7365 6c66 2e61 7373 6572 7446      self.assertF
-0002ac80: 616c 7365 2863 322e 6578 6973 7473 2863  alse(c2.exists(c
-0002ac90: 325f 6670 6174 6829 290a 0a20 2020 2020  2_fpath))..     
-0002aca0: 2020 2023 2063 6865 636b 2074 6861 7420     # check that 
-0002acb0: 7468 6520 6669 6c65 2069 7320 7669 7369  the file is visi
-0002acc0: 626c 6520 696e 2063 3320 7768 6963 6820  ble in c3 which 
-0002acd0: 6861 7320 7468 6520 7361 6d65 2073 746f  has the same sto
-0002ace0: 7261 6765 206d 6f75 6e74 0a20 2020 2020  rage mount.     
-0002acf0: 2020 2063 3320 3d20 6861 726e 6573 732e     c3 = harness.
-0002ad00: 6d6f 6465 6c2e 756e 6974 2e67 6574 5f63  model.unit.get_c
-0002ad10: 6f6e 7461 696e 6572 2827 6333 2729 0a20  ontainer('c3'). 
-0002ad20: 2020 2020 2020 2063 335f 6670 6174 6820         c3_fpath 
-0002ad30: 3d20 6f73 2e70 6174 682e 6a6f 696e 2827  = os.path.join('
-0002ad40: 2f6d 6f75 6e74 732f 6261 7227 2c20 6331  /mounts/bar', c1
-0002ad50: 5f66 6e61 6d65 290a 2020 2020 2020 2020  _fname).        
-0002ad60: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
-0002ad70: 6333 2e65 7869 7374 7328 6333 5f66 7061  c3.exists(c3_fpa
-0002ad80: 7468 2929 0a20 2020 2020 2020 2077 6974  th)).        wit
-0002ad90: 6820 6333 2e70 756c 6c28 6333 5f66 7061  h c3.pull(c3_fpa
-0002ada0: 7468 2920 6173 2066 3a0a 2020 2020 2020  th) as f:.      
-0002adb0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0002adc0: 7445 7175 616c 2827 3432 272c 2066 2e72  tEqual('42', f.r
-0002add0: 6561 6428 2929 0a0a 2020 2020 2020 2020  ead())..        
-0002ade0: 2320 7465 7374 2061 6c6c 206f 7468 6572  # test all other
-0002adf0: 2063 6f6e 7461 696e 6572 2066 696c 6520   container file 
-0002ae00: 6f70 730a 2020 2020 2020 2020 7769 7468  ops.        with
-0002ae10: 2063 312e 7075 6c6c 2863 315f 6670 6174   c1.pull(c1_fpat
-0002ae20: 6829 2061 7320 663a 0a20 2020 2020 2020  h) as f:.       
-0002ae30: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0002ae40: 4571 7561 6c28 2734 3227 2c20 662e 7265  Equal('42', f.re
-0002ae50: 6164 2829 290a 2020 2020 2020 2020 6669  ad()).        fi
-0002ae60: 6c65 7320 3d20 6331 2e6c 6973 745f 6669  les = c1.list_fi
-0002ae70: 6c65 7328 6331 5f66 7061 7468 290a 2020  les(c1_fpath).  
-0002ae80: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0002ae90: 7445 7175 616c 285b 6331 5f66 7061 7468  tEqual([c1_fpath
-0002aea0: 5d2c 205b 6669 2e70 6174 6820 666f 7220  ], [fi.path for 
-0002aeb0: 6669 2069 6e20 6669 6c65 735d 290a 2020  fi in files]).  
-0002aec0: 2020 2020 2020 6331 2e72 656d 6f76 655f        c1.remove_
-0002aed0: 7061 7468 2863 315f 6670 6174 6829 0a20  path(c1_fpath). 
-0002aee0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0002aef0: 7274 4661 6c73 6528 6331 2e65 7869 7374  rtFalse(c1.exist
-0002af00: 7328 6331 5f66 7061 7468 2929 0a0a 2020  s(c1_fpath))..  
-0002af10: 2020 2020 2020 2320 7465 7374 2064 6574        # test det
-0002af20: 6163 6869 6e67 2073 746f 7261 6765 0a20  aching storage. 
-0002af30: 2020 2020 2020 2063 312e 7075 7368 2863         c1.push(c
-0002af40: 315f 6670 6174 682c 2027 3432 2729 0a20  1_fpath, '42'). 
-0002af50: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0002af60: 7274 5472 7565 2863 312e 6578 6973 7473  rtTrue(c1.exists
-0002af70: 2863 315f 6670 6174 6829 290a 2020 2020  (c1_fpath)).    
-0002af80: 2020 2020 7374 6f72 6531 5f69 6420 3d20      store1_id = 
-0002af90: 6861 726e 6573 732e 6d6f 6465 6c2e 7374  harness.model.st
-0002afa0: 6f72 6167 6573 5b27 7374 6f72 6531 275d  orages['store1']
-0002afb0: 5b30 5d2e 6675 6c6c 5f69 640a 2020 2020  [0].full_id.    
-0002afc0: 2020 2020 6861 726e 6573 732e 7265 6d6f      harness.remo
-0002afd0: 7665 5f73 746f 7261 6765 2873 746f 7265  ve_storage(store
-0002afe0: 315f 6964 290a 2020 2020 2020 2020 7365  1_id).        se
-0002aff0: 6c66 2e61 7373 6572 7446 616c 7365 2863  lf.assertFalse(c
-0002b000: 312e 6578 6973 7473 2863 315f 6670 6174  1.exists(c1_fpat
-0002b010: 6829 290a 0a20 2020 2064 6566 2074 6573  h))..    def tes
-0002b020: 745f 7075 7368 5f77 6974 685f 6f77 6e65  t_push_with_owne
-0002b030: 7273 6869 7028 7365 6c66 293a 0a20 2020  rship(self):.   
-0002b040: 2020 2020 2023 204e 6f74 653a 2054 6f20       # Note: To 
-0002b050: 7369 6d70 6c69 6679 2069 6d70 6c65 6d65  simplify impleme
-0002b060: 6e74 6174 696f 6e2c 206f 776e 6572 7368  ntation, ownersh
-0002b070: 6970 2069 7320 7369 6d70 6c79 2073 746f  ip is simply sto
-0002b080: 7265 6420 6173 2d69 7320 7769 7468 206e  red as-is with n
-0002b090: 6f20 7665 7269 6669 6361 7469 6f6e 2e0a  o verification..
-0002b0a0: 2020 2020 2020 2020 6461 7461 203d 2027          data = '
-0002b0b0: 6461 7461 270a 2020 2020 2020 2020 636c  data'.        cl
-0002b0c0: 6965 6e74 203d 2073 656c 662e 636c 6965  ient = self.clie
-0002b0d0: 6e74 0a20 2020 2020 2020 2063 6c69 656e  nt.        clien
-0002b0e0: 742e 7075 7368 2866 227b 7365 6c66 2e70  t.push(f"{self.p
-0002b0f0: 7265 6669 787d 2f66 696c 6522 2c20 6461  refix}/file", da
-0002b100: 7461 2c20 7573 6572 5f69 643d 312c 2075  ta, user_id=1, u
-0002b110: 7365 723d 2766 6f6f 272c 2067 726f 7570  ser='foo', group
-0002b120: 5f69 643d 332c 2067 726f 7570 3d27 6261  _id=3, group='ba
-0002b130: 7227 290a 2020 2020 2020 2020 6669 6c65  r').        file
-0002b140: 5f20 3d20 636c 6965 6e74 2e6c 6973 745f  _ = client.list_
-0002b150: 6669 6c65 7328 6622 7b73 656c 662e 7072  files(f"{self.pr
-0002b160: 6566 6978 7d2f 6669 6c65 2229 5b30 5d0a  efix}/file")[0].
-0002b170: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0002b180: 6572 7445 7175 616c 2866 696c 655f 2e75  ertEqual(file_.u
-0002b190: 7365 725f 6964 2c20 3129 0a20 2020 2020  ser_id, 1).     
-0002b1a0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0002b1b0: 7561 6c28 6669 6c65 5f2e 7573 6572 2c20  ual(file_.user, 
-0002b1c0: 2766 6f6f 2729 0a20 2020 2020 2020 2073  'foo').        s
-0002b1d0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0002b1e0: 6669 6c65 5f2e 6772 6f75 705f 6964 2c20  file_.group_id, 
-0002b1f0: 3329 0a20 2020 2020 2020 2073 656c 662e  3).        self.
-0002b200: 6173 7365 7274 4571 7561 6c28 6669 6c65  assertEqual(file
-0002b210: 5f2e 6772 6f75 702c 2027 6261 7227 290a  _.group, 'bar').
-0002b220: 0a20 2020 2064 6566 2074 6573 745f 6d61  .    def test_ma
-0002b230: 6b65 5f64 6972 5f77 6974 685f 6f77 6e65  ke_dir_with_owne
-0002b240: 7273 6869 7028 7365 6c66 293a 0a20 2020  rship(self):.   
-0002b250: 2020 2020 2063 6c69 656e 7420 3d20 7365       client = se
-0002b260: 6c66 2e63 6c69 656e 740a 2020 2020 2020  lf.client.      
-0002b270: 2020 636c 6965 6e74 2e6d 616b 655f 6469    client.make_di
-0002b280: 7228 6622 7b73 656c 662e 7072 6566 6978  r(f"{self.prefix
-0002b290: 7d2f 6469 7231 222c 2075 7365 725f 6964  }/dir1", user_id
-0002b2a0: 3d31 2c20 7573 6572 3d22 666f 6f22 2c20  =1, user="foo", 
-0002b2b0: 6772 6f75 705f 6964 3d33 2c20 6772 6f75  group_id=3, grou
-0002b2c0: 703d 2262 6172 2229 0a20 2020 2020 2020  p="bar").       
-0002b2d0: 2064 6972 5f20 3d20 636c 6965 6e74 2e6c   dir_ = client.l
-0002b2e0: 6973 745f 6669 6c65 7328 6622 7b73 656c  ist_files(f"{sel
-0002b2f0: 662e 7072 6566 6978 7d2f 6469 7231 222c  f.prefix}/dir1",
-0002b300: 2069 7473 656c 663d 5472 7565 295b 305d   itself=True)[0]
-0002b310: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0002b320: 7365 7274 4571 7561 6c28 6469 725f 2e75  sertEqual(dir_.u
-0002b330: 7365 725f 6964 2c20 3129 0a20 2020 2020  ser_id, 1).     
-0002b340: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0002b350: 7561 6c28 6469 725f 2e75 7365 722c 2022  ual(dir_.user, "
-0002b360: 666f 6f22 290a 2020 2020 2020 2020 7365  foo").        se
-0002b370: 6c66 2e61 7373 6572 7445 7175 616c 2864  lf.assertEqual(d
-0002b380: 6972 5f2e 6772 6f75 705f 6964 2c20 3329  ir_.group_id, 3)
-0002b390: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0002b3a0: 7365 7274 4571 7561 6c28 6469 725f 2e67  sertEqual(dir_.g
-0002b3b0: 726f 7570 2c20 2262 6172 2229 0a0a 0a40  roup, "bar")...@
-0002b3c0: 756e 6974 7465 7374 2e73 6b69 7055 6e6c  unittest.skipUnl
-0002b3d0: 6573 7328 6f73 2e67 6574 656e 7628 2752  ess(os.getenv('R
-0002b3e0: 554e 5f52 4541 4c5f 5045 4242 4c45 5f54  UN_REAL_PEBBLE_T
-0002b3f0: 4553 5453 2729 2c20 2752 554e 5f52 4541  ESTS'), 'RUN_REA
-0002b400: 4c5f 5045 4242 4c45 5f54 4553 5453 206e  L_PEBBLE_TESTS n
-0002b410: 6f74 2073 6574 2729 0a63 6c61 7373 2054  ot set').class T
-0002b420: 6573 7450 6562 626c 6553 746f 7261 6765  estPebbleStorage
-0002b430: 4150 4973 5573 696e 6752 6561 6c50 6562  APIsUsingRealPeb
-0002b440: 626c 6528 756e 6974 7465 7374 2e54 6573  ble(unittest.Tes
-0002b450: 7443 6173 652c 205f 5065 6262 6c65 5374  tCase, _PebbleSt
-0002b460: 6f72 6167 6541 5049 7354 6573 744d 6978  orageAPIsTestMix
-0002b470: 696e 293a 0a20 2020 2064 6566 2073 6574  in):.    def set
-0002b480: 5570 2873 656c 6629 3a0a 2020 2020 2020  Up(self):.      
-0002b490: 2020 736f 636b 6574 5f70 6174 6820 3d20    socket_path = 
-0002b4a0: 6f73 2e67 6574 656e 7628 2750 4542 424c  os.getenv('PEBBL
-0002b4b0: 455f 534f 434b 4554 2729 0a20 2020 2020  E_SOCKET').     
-0002b4c0: 2020 2070 6562 626c 655f 6469 7220 3d20     pebble_dir = 
-0002b4d0: 6f73 2e67 6574 656e 7628 2750 4542 424c  os.getenv('PEBBL
-0002b4e0: 4527 290a 2020 2020 2020 2020 6966 206e  E').        if n
-0002b4f0: 6f74 2073 6f63 6b65 745f 7061 7468 2061  ot socket_path a
-0002b500: 6e64 2070 6562 626c 655f 6469 723a 0a20  nd pebble_dir:. 
-0002b510: 2020 2020 2020 2020 2020 2073 6f63 6b65             socke
-0002b520: 745f 7061 7468 203d 206f 732e 7061 7468  t_path = os.path
-0002b530: 2e6a 6f69 6e28 7065 6262 6c65 5f64 6972  .join(pebble_dir
-0002b540: 2c20 272e 7065 6262 6c65 2e73 6f63 6b65  , '.pebble.socke
-0002b550: 7427 290a 2020 2020 2020 2020 6173 7365  t').        asse
-0002b560: 7274 2073 6f63 6b65 745f 7061 7468 2061  rt socket_path a
-0002b570: 6e64 2070 6562 626c 655f 6469 722c 2027  nd pebble_dir, '
-0002b580: 5045 4242 4c45 206d 7573 7420 6265 2073  PEBBLE must be s
-0002b590: 6574 2069 6620 5255 4e5f 5245 414c 5f50  et if RUN_REAL_P
-0002b5a0: 4542 424c 455f 5445 5354 5320 7365 7427  EBBLE_TESTS set'
-0002b5b0: 0a0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
-0002b5c0: 7265 6669 7820 3d20 7465 6d70 6669 6c65  refix = tempfile
-0002b5d0: 2e6d 6b64 7465 6d70 2864 6972 3d70 6562  .mkdtemp(dir=peb
-0002b5e0: 626c 655f 6469 7229 0a20 2020 2020 2020  ble_dir).       
-0002b5f0: 2073 656c 662e 636c 6965 6e74 203d 2070   self.client = p
-0002b600: 6562 626c 652e 436c 6965 6e74 2873 6f63  ebble.Client(soc
-0002b610: 6b65 745f 7061 7468 3d73 6f63 6b65 745f  ket_path=socket_
-0002b620: 7061 7468 290a 0a20 2020 2064 6566 2074  path)..    def t
-0002b630: 6561 7244 6f77 6e28 7365 6c66 293a 0a20  earDown(self):. 
-0002b640: 2020 2020 2020 2073 6875 7469 6c2e 726d         shutil.rm
-0002b650: 7472 6565 2873 656c 662e 7072 6566 6978  tree(self.prefix
-0002b660: 290a 0a20 2020 2023 2052 656d 6f76 6520  )..    # Remove 
-0002b670: 7468 6973 2065 6e74 6972 656c 7920 6f6e  this entirely on
-0002b680: 6365 2074 6865 2061 7373 6f63 6961 7465  ce the associate
-0002b690: 6420 6275 6720 6973 2066 6978 6564 3b20  d bug is fixed; 
-0002b6a0: 6974 206f 7665 7272 6964 6573 2074 6865  it overrides the
-0002b6b0: 206f 7269 6769 6e61 6c20 7465 7374 2069   original test i
-0002b6c0: 6e20 7468 650a 2020 2020 2320 7465 7374  n the.    # test
-0002b6d0: 206d 6978 696e 2063 6c61 7373 2e0a 2020   mixin class..  
-0002b6e0: 2020 4075 6e69 7474 6573 742e 736b 6970    @unittest.skip
-0002b6f0: 2827 7065 6e64 696e 6720 7265 736f 6c75  ('pending resolu
-0002b700: 7469 6f6e 206f 6620 6874 7470 733a 2f2f  tion of https://
-0002b710: 6769 7468 7562 2e63 6f6d 2f63 616e 6f6e  github.com/canon
-0002b720: 6963 616c 2f70 6562 626c 652f 6973 7375  ical/pebble/issu
-0002b730: 6573 2f38 3027 290a 2020 2020 6465 6620  es/80').    def 
-0002b740: 7465 7374 5f6d 616b 655f 6469 725f 7769  test_make_dir_wi
-0002b750: 7468 5f70 6572 6d69 7373 696f 6e5f 6d61  th_permission_ma
-0002b760: 736b 2873 656c 6629 3a0a 2020 2020 2020  sk(self):.      
-0002b770: 2020 7061 7373 0a0a 0a63 6c61 7373 2054    pass...class T
-0002b780: 6573 7453 6563 7265 7473 2875 6e69 7474  estSecrets(unitt
-0002b790: 6573 742e 5465 7374 4361 7365 293a 0a20  est.TestCase):. 
-0002b7a0: 2020 2064 6566 2074 6573 745f 6164 645f     def test_add_
-0002b7b0: 6d6f 6465 6c5f 7365 6372 6574 5f62 795f  model_secret_by_
-0002b7c0: 6170 705f 6e61 6d65 5f73 7472 2873 656c  app_name_str(sel
-0002b7d0: 6629 3a0a 2020 2020 2020 2020 6861 726e  f):.        harn
-0002b7e0: 6573 7320 3d20 6f70 732e 7465 7374 696e  ess = ops.testin
-0002b7f0: 672e 4861 726e 6573 7328 6f70 732e 4368  g.Harness(ops.Ch
-0002b800: 6172 6d42 6173 652c 206d 6574 613d 276e  armBase, meta='n
-0002b810: 616d 653a 2077 6562 6170 7027 290a 2020  ame: webapp').  
-0002b820: 2020 2020 2020 7365 6c66 2e61 6464 436c        self.addCl
-0002b830: 6561 6e75 7028 6861 726e 6573 732e 636c  eanup(harness.cl
-0002b840: 6561 6e75 7029 0a20 2020 2020 2020 2072  eanup).        r
-0002b850: 656c 6174 696f 6e5f 6964 203d 2068 6172  elation_id = har
-0002b860: 6e65 7373 2e61 6464 5f72 656c 6174 696f  ness.add_relatio
-0002b870: 6e28 2764 6227 2c20 2764 6174 6162 6173  n('db', 'databas
-0002b880: 6527 290a 2020 2020 2020 2020 6861 726e  e').        harn
-0002b890: 6573 732e 6164 645f 7265 6c61 7469 6f6e  ess.add_relation
-0002b8a0: 5f75 6e69 7428 7265 6c61 7469 6f6e 5f69  _unit(relation_i
-0002b8b0: 642c 2027 6461 7461 6261 7365 2f30 2729  d, 'database/0')
-0002b8c0: 0a0a 2020 2020 2020 2020 7365 6372 6574  ..        secret
-0002b8d0: 5f69 6420 3d20 6861 726e 6573 732e 6164  _id = harness.ad
-0002b8e0: 645f 6d6f 6465 6c5f 7365 6372 6574 2827  d_model_secret('
-0002b8f0: 6461 7461 6261 7365 272c 207b 2770 6173  database', {'pas
-0002b900: 7377 6f72 6427 3a20 2768 756e 7465 7232  sword': 'hunter2
-0002b910: 277d 290a 2020 2020 2020 2020 6861 726e  '}).        harn
-0002b920: 6573 732e 6772 616e 745f 7365 6372 6574  ess.grant_secret
-0002b930: 2873 6563 7265 745f 6964 2c20 2777 6562  (secret_id, 'web
-0002b940: 6170 7027 290a 2020 2020 2020 2020 7365  app').        se
-0002b950: 6372 6574 203d 2068 6172 6e65 7373 2e6d  cret = harness.m
-0002b960: 6f64 656c 2e67 6574 5f73 6563 7265 7428  odel.get_secret(
-0002b970: 6964 3d73 6563 7265 745f 6964 290a 2020  id=secret_id).  
-0002b980: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0002b990: 7445 7175 616c 2873 6563 7265 742e 6964  tEqual(secret.id
-0002b9a0: 2c20 7365 6372 6574 5f69 6429 0a20 2020  , secret_id).   
-0002b9b0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0002b9c0: 4571 7561 6c28 7365 6372 6574 2e67 6574  Equal(secret.get
-0002b9d0: 5f63 6f6e 7465 6e74 2829 2c20 7b27 7061  _content(), {'pa
-0002b9e0: 7373 776f 7264 273a 2027 6875 6e74 6572  ssword': 'hunter
-0002b9f0: 3227 7d29 0a0a 2020 2020 6465 6620 7465  2'})..    def te
-0002ba00: 7374 5f61 6464 5f6d 6f64 656c 5f73 6563  st_add_model_sec
-0002ba10: 7265 745f 6279 5f61 7070 5f69 6e73 7461  ret_by_app_insta
-0002ba20: 6e63 6528 7365 6c66 293a 0a20 2020 2020  nce(self):.     
-0002ba30: 2020 2068 6172 6e65 7373 203d 206f 7073     harness = ops
-0002ba40: 2e74 6573 7469 6e67 2e48 6172 6e65 7373  .testing.Harness
-0002ba50: 286f 7073 2e43 6861 726d 4261 7365 2c20  (ops.CharmBase, 
-0002ba60: 6d65 7461 3d27 6e61 6d65 3a20 7765 6261  meta='name: weba
-0002ba70: 7070 2729 0a20 2020 2020 2020 2073 656c  pp').        sel
-0002ba80: 662e 6164 6443 6c65 616e 7570 2868 6172  f.addCleanup(har
-0002ba90: 6e65 7373 2e63 6c65 616e 7570 290a 2020  ness.cleanup).  
-0002baa0: 2020 2020 2020 7265 6c61 7469 6f6e 5f69        relation_i
-0002bab0: 6420 3d20 6861 726e 6573 732e 6164 645f  d = harness.add_
-0002bac0: 7265 6c61 7469 6f6e 2827 6462 272c 2027  relation('db', '
-0002bad0: 6461 7461 6261 7365 2729 0a20 2020 2020  database').     
-0002bae0: 2020 2068 6172 6e65 7373 2e61 6464 5f72     harness.add_r
-0002baf0: 656c 6174 696f 6e5f 756e 6974 2872 656c  elation_unit(rel
-0002bb00: 6174 696f 6e5f 6964 2c20 2764 6174 6162  ation_id, 'datab
-0002bb10: 6173 652f 3027 290a 0a20 2020 2020 2020  ase/0')..       
-0002bb20: 2061 7070 203d 2068 6172 6e65 7373 2e6d   app = harness.m
-0002bb30: 6f64 656c 2e67 6574 5f61 7070 2827 6461  odel.get_app('da
-0002bb40: 7461 6261 7365 2729 0a20 2020 2020 2020  tabase').       
-0002bb50: 2073 6563 7265 745f 6964 203d 2068 6172   secret_id = har
-0002bb60: 6e65 7373 2e61 6464 5f6d 6f64 656c 5f73  ness.add_model_s
-0002bb70: 6563 7265 7428 6170 702c 207b 2770 6173  ecret(app, {'pas
-0002bb80: 7377 6f72 6427 3a20 2768 756e 7465 7233  sword': 'hunter3
-0002bb90: 277d 290a 2020 2020 2020 2020 6861 726e  '}).        harn
-0002bba0: 6573 732e 6772 616e 745f 7365 6372 6574  ess.grant_secret
-0002bbb0: 2873 6563 7265 745f 6964 2c20 2777 6562  (secret_id, 'web
-0002bbc0: 6170 7027 290a 2020 2020 2020 2020 7365  app').        se
-0002bbd0: 6372 6574 203d 2068 6172 6e65 7373 2e6d  cret = harness.m
-0002bbe0: 6f64 656c 2e67 6574 5f73 6563 7265 7428  odel.get_secret(
-0002bbf0: 6964 3d73 6563 7265 745f 6964 290a 2020  id=secret_id).  
-0002bc00: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0002bc10: 7445 7175 616c 2873 6563 7265 742e 6964  tEqual(secret.id
-0002bc20: 2c20 7365 6372 6574 5f69 6429 0a20 2020  , secret_id).   
-0002bc30: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0002bc40: 4571 7561 6c28 7365 6372 6574 2e67 6574  Equal(secret.get
-0002bc50: 5f63 6f6e 7465 6e74 2829 2c20 7b27 7061  _content(), {'pa
-0002bc60: 7373 776f 7264 273a 2027 6875 6e74 6572  ssword': 'hunter
-0002bc70: 3327 7d29 0a0a 2020 2020 6465 6620 7465  3'})..    def te
-0002bc80: 7374 5f61 6464 5f6d 6f64 656c 5f73 6563  st_add_model_sec
-0002bc90: 7265 745f 6279 5f75 6e69 745f 696e 7374  ret_by_unit_inst
-0002bca0: 616e 6365 2873 656c 6629 3a0a 2020 2020  ance(self):.    
-0002bcb0: 2020 2020 6861 726e 6573 7320 3d20 6f70      harness = op
-0002bcc0: 732e 7465 7374 696e 672e 4861 726e 6573  s.testing.Harnes
-0002bcd0: 7328 6f70 732e 4368 6172 6d42 6173 652c  s(ops.CharmBase,
-0002bce0: 206d 6574 613d 276e 616d 653a 2077 6562   meta='name: web
-0002bcf0: 6170 7027 290a 2020 2020 2020 2020 7365  app').        se
-0002bd00: 6c66 2e61 6464 436c 6561 6e75 7028 6861  lf.addCleanup(ha
-0002bd10: 726e 6573 732e 636c 6561 6e75 7029 0a20  rness.cleanup). 
-0002bd20: 2020 2020 2020 2072 656c 6174 696f 6e5f         relation_
-0002bd30: 6964 203d 2068 6172 6e65 7373 2e61 6464  id = harness.add
-0002bd40: 5f72 656c 6174 696f 6e28 2764 6227 2c20  _relation('db', 
-0002bd50: 2764 6174 6162 6173 6527 290a 2020 2020  'database').    
-0002bd60: 2020 2020 6861 726e 6573 732e 6164 645f      harness.add_
-0002bd70: 7265 6c61 7469 6f6e 5f75 6e69 7428 7265  relation_unit(re
-0002bd80: 6c61 7469 6f6e 5f69 642c 2027 6461 7461  lation_id, 'data
-0002bd90: 6261 7365 2f30 2729 0a0a 2020 2020 2020  base/0')..      
-0002bda0: 2020 756e 6974 203d 2068 6172 6e65 7373    unit = harness
-0002bdb0: 2e6d 6f64 656c 2e67 6574 5f75 6e69 7428  .model.get_unit(
-0002bdc0: 2764 6174 6162 6173 652f 3027 290a 2020  'database/0').  
-0002bdd0: 2020 2020 2020 7365 6372 6574 5f69 6420        secret_id 
-0002bde0: 3d20 6861 726e 6573 732e 6164 645f 6d6f  = harness.add_mo
-0002bdf0: 6465 6c5f 7365 6372 6574 2875 6e69 742c  del_secret(unit,
-0002be00: 207b 2770 6173 7377 6f72 6427 3a20 2768   {'password': 'h
-0002be10: 756e 7465 7234 277d 290a 2020 2020 2020  unter4'}).      
-0002be20: 2020 6861 726e 6573 732e 6772 616e 745f    harness.grant_
-0002be30: 7365 6372 6574 2873 6563 7265 745f 6964  secret(secret_id
-0002be40: 2c20 2777 6562 6170 7027 290a 2020 2020  , 'webapp').    
-0002be50: 2020 2020 7365 6372 6574 203d 2068 6172      secret = har
-0002be60: 6e65 7373 2e6d 6f64 656c 2e67 6574 5f73  ness.model.get_s
-0002be70: 6563 7265 7428 6964 3d73 6563 7265 745f  ecret(id=secret_
-0002be80: 6964 290a 2020 2020 2020 2020 7365 6c66  id).        self
-0002be90: 2e61 7373 6572 7445 7175 616c 2873 6563  .assertEqual(sec
-0002bea0: 7265 742e 6964 2c20 7365 6372 6574 5f69  ret.id, secret_i
-0002beb0: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
-0002bec0: 6173 7365 7274 4571 7561 6c28 7365 6372  assertEqual(secr
-0002bed0: 6574 2e67 6574 5f63 6f6e 7465 6e74 2829  et.get_content()
-0002bee0: 2c20 7b27 7061 7373 776f 7264 273a 2027  , {'password': '
-0002bef0: 6875 6e74 6572 3427 7d29 0a0a 2020 2020  hunter4'})..    
-0002bf00: 6465 6620 7465 7374 5f61 6464 5f6d 6f64  def test_add_mod
-0002bf10: 656c 5f73 6563 7265 745f 696e 7661 6c69  el_secret_invali
-0002bf20: 645f 636f 6e74 656e 7428 7365 6c66 293a  d_content(self):
-0002bf30: 0a20 2020 2020 2020 2068 6172 6e65 7373  .        harness
-0002bf40: 203d 206f 7073 2e74 6573 7469 6e67 2e48   = ops.testing.H
-0002bf50: 6172 6e65 7373 286f 7073 2e43 6861 726d  arness(ops.Charm
-0002bf60: 4261 7365 2c20 6d65 7461 3d27 6e61 6d65  Base, meta='name
-0002bf70: 3a20 7765 6261 7070 2729 0a20 2020 2020  : webapp').     
-0002bf80: 2020 2073 656c 662e 6164 6443 6c65 616e     self.addClean
-0002bf90: 7570 2868 6172 6e65 7373 2e63 6c65 616e  up(harness.clean
-0002bfa0: 7570 290a 0a20 2020 2020 2020 2077 6974  up)..        wit
-0002bfb0: 6820 7365 6c66 2e61 7373 6572 7452 6169  h self.assertRai
-0002bfc0: 7365 7328 5661 6c75 6545 7272 6f72 293a  ses(ValueError):
-0002bfd0: 0a20 2020 2020 2020 2020 2020 2068 6172  .            har
-0002bfe0: 6e65 7373 2e61 6464 5f6d 6f64 656c 5f73  ness.add_model_s
-0002bff0: 6563 7265 7428 2764 6174 6162 6173 6527  ecret('database'
-0002c000: 2c20 7b27 7827 3a20 2779 277d 2920 2023  , {'x': 'y'})  #
-0002c010: 206b 6579 2074 6f6f 2073 686f 7274 0a0a   key too short..
-0002c020: 2020 2020 6465 6620 7465 7374 5f73 6574      def test_set
-0002c030: 5f73 6563 7265 745f 636f 6e74 656e 7428  _secret_content(
-0002c040: 7365 6c66 293a 0a20 2020 2020 2020 2068  self):.        h
-0002c050: 6172 6e65 7373 203d 206f 7073 2e74 6573  arness = ops.tes
-0002c060: 7469 6e67 2e48 6172 6e65 7373 2845 7665  ting.Harness(Eve
-0002c070: 6e74 5265 636f 7264 6572 2c20 6d65 7461  ntRecorder, meta
-0002c080: 3d27 6e61 6d65 3a20 7765 6261 7070 2729  ='name: webapp')
-0002c090: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
-0002c0a0: 6443 6c65 616e 7570 2868 6172 6e65 7373  dCleanup(harness
-0002c0b0: 2e63 6c65 616e 7570 290a 2020 2020 2020  .cleanup).      
-0002c0c0: 2020 7265 6c61 7469 6f6e 5f69 6420 3d20    relation_id = 
-0002c0d0: 6861 726e 6573 732e 6164 645f 7265 6c61  harness.add_rela
-0002c0e0: 7469 6f6e 2827 6462 272c 2027 6461 7461  tion('db', 'data
-0002c0f0: 6261 7365 2729 0a20 2020 2020 2020 2068  base').        h
-0002c100: 6172 6e65 7373 2e61 6464 5f72 656c 6174  arness.add_relat
-0002c110: 696f 6e5f 756e 6974 2872 656c 6174 696f  ion_unit(relatio
-0002c120: 6e5f 6964 2c20 2764 6174 6162 6173 652f  n_id, 'database/
-0002c130: 3027 290a 0a20 2020 2020 2020 2073 6563  0')..        sec
-0002c140: 7265 745f 6964 203d 2068 6172 6e65 7373  ret_id = harness
-0002c150: 2e61 6464 5f6d 6f64 656c 5f73 6563 7265  .add_model_secre
-0002c160: 7428 2764 6174 6162 6173 6527 2c20 7b27  t('database', {'
-0002c170: 666f 6f27 3a20 2731 277d 290a 2020 2020  foo': '1'}).    
-0002c180: 2020 2020 6861 726e 6573 732e 6772 616e      harness.gran
-0002c190: 745f 7365 6372 6574 2873 6563 7265 745f  t_secret(secret_
-0002c1a0: 6964 2c20 2777 6562 6170 7027 290a 2020  id, 'webapp').  
-0002c1b0: 2020 2020 2020 6861 726e 6573 732e 6265        harness.be
-0002c1c0: 6769 6e28 290a 2020 2020 2020 2020 6861  gin().        ha
-0002c1d0: 726e 6573 732e 6672 616d 6577 6f72 6b2e  rness.framework.
-0002c1e0: 6f62 7365 7276 6528 6861 726e 6573 732e  observe(harness.
-0002c1f0: 6368 6172 6d2e 6f6e 2e73 6563 7265 745f  charm.on.secret_
-0002c200: 6368 616e 6765 642c 2068 6172 6e65 7373  changed, harness
-0002c210: 2e63 6861 726d 2e72 6563 6f72 645f 6576  .charm.record_ev
-0002c220: 656e 7429 0a20 2020 2020 2020 2068 6172  ent).        har
-0002c230: 6e65 7373 2e73 6574 5f73 6563 7265 745f  ness.set_secret_
-0002c240: 636f 6e74 656e 7428 7365 6372 6574 5f69  content(secret_i
-0002c250: 642c 207b 2766 6f6f 273a 2027 3227 7d29  d, {'foo': '2'})
-0002c260: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-0002c270: 7373 6572 7445 7175 616c 286c 656e 2868  ssertEqual(len(h
-0002c280: 6172 6e65 7373 2e63 6861 726d 2e65 7665  arness.charm.eve
-0002c290: 6e74 7329 2c20 3129 0a20 2020 2020 2020  nts), 1).       
-0002c2a0: 2065 7665 6e74 203d 2068 6172 6e65 7373   event = harness
-0002c2b0: 2e63 6861 726d 2e65 7665 6e74 735b 305d  .charm.events[0]
-0002c2c0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0002c2d0: 7365 7274 4973 496e 7374 616e 6365 2865  sertIsInstance(e
-0002c2e0: 7665 6e74 2c20 6f70 732e 5365 6372 6574  vent, ops.Secret
-0002c2f0: 4368 616e 6765 6445 7665 6e74 290a 2020  ChangedEvent).  
-0002c300: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0002c310: 7445 7175 616c 2865 7665 6e74 2e73 6563  tEqual(event.sec
-0002c320: 7265 742e 6765 745f 636f 6e74 656e 7428  ret.get_content(
-0002c330: 292c 207b 2766 6f6f 273a 2027 3127 7d29  ), {'foo': '1'})
-0002c340: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0002c350: 7365 7274 4571 7561 6c28 6576 656e 742e  sertEqual(event.
-0002c360: 7365 6372 6574 2e67 6574 5f63 6f6e 7465  secret.get_conte
-0002c370: 6e74 2872 6566 7265 7368 3d54 7275 6529  nt(refresh=True)
-0002c380: 2c20 7b27 666f 6f27 3a20 2732 277d 290a  , {'foo': '2'}).
-0002c390: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0002c3a0: 6572 7445 7175 616c 2865 7665 6e74 2e73  ertEqual(event.s
-0002c3b0: 6563 7265 742e 6765 745f 636f 6e74 656e  ecret.get_conten
-0002c3c0: 7428 292c 207b 2766 6f6f 273a 2027 3227  t(), {'foo': '2'
-0002c3d0: 7d29 0a0a 2020 2020 2020 2020 7365 6c66  })..        self
-0002c3e0: 2e61 7373 6572 7445 7175 616c 2868 6172  .assertEqual(har
-0002c3f0: 6e65 7373 2e67 6574 5f73 6563 7265 745f  ness.get_secret_
-0002c400: 7265 7669 7369 6f6e 7328 7365 6372 6574  revisions(secret
-0002c410: 5f69 6429 2c20 5b31 2c20 325d 290a 0a20  _id), [1, 2]).. 
-0002c420: 2020 2064 6566 2074 6573 745f 7365 745f     def test_set_
-0002c430: 7365 6372 6574 5f63 6f6e 7465 6e74 5f77  secret_content_w
-0002c440: 726f 6e67 5f6f 776e 6572 2873 656c 6629  rong_owner(self)
-0002c450: 3a0a 2020 2020 2020 2020 6861 726e 6573  :.        harnes
-0002c460: 7320 3d20 6f70 732e 7465 7374 696e 672e  s = ops.testing.
-0002c470: 4861 726e 6573 7328 6f70 732e 4368 6172  Harness(ops.Char
-0002c480: 6d42 6173 652c 206d 6574 613d 276e 616d  mBase, meta='nam
-0002c490: 653a 2077 6562 6170 7027 290a 2020 2020  e: webapp').    
-0002c4a0: 2020 2020 7365 6c66 2e61 6464 436c 6561      self.addClea
-0002c4b0: 6e75 7028 6861 726e 6573 732e 636c 6561  nup(harness.clea
-0002c4c0: 6e75 7029 0a0a 2020 2020 2020 2020 7365  nup)..        se
-0002c4d0: 6372 6574 203d 2068 6172 6e65 7373 2e6d  cret = harness.m
-0002c4e0: 6f64 656c 2e61 7070 2e61 6464 5f73 6563  odel.app.add_sec
-0002c4f0: 7265 7428 7b27 666f 6f27 3a20 2762 6172  ret({'foo': 'bar
-0002c500: 277d 290a 2020 2020 2020 2020 7769 7468  '}).        with
-0002c510: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
-0002c520: 6573 2852 756e 7469 6d65 4572 726f 7229  es(RuntimeError)
-0002c530: 3a0a 2020 2020 2020 2020 2020 2020 6861  :.            ha
-0002c540: 726e 6573 732e 7365 745f 7365 6372 6574  rness.set_secret
-0002c550: 5f63 6f6e 7465 6e74 2873 6563 7265 742e  _content(secret.
-0002c560: 6964 2c20 7b27 6261 7227 3a20 2766 6f6f  id, {'bar': 'foo
-0002c570: 277d 290a 0a20 2020 2064 6566 2074 6573  '})..    def tes
-0002c580: 745f 7365 745f 7365 6372 6574 5f63 6f6e  t_set_secret_con
-0002c590: 7465 6e74 5f69 6e76 616c 6964 5f73 6563  tent_invalid_sec
-0002c5a0: 7265 745f 6964 2873 656c 6629 3a0a 2020  ret_id(self):.  
-0002c5b0: 2020 2020 2020 6861 726e 6573 7320 3d20        harness = 
-0002c5c0: 6f70 732e 7465 7374 696e 672e 4861 726e  ops.testing.Harn
-0002c5d0: 6573 7328 6f70 732e 4368 6172 6d42 6173  ess(ops.CharmBas
-0002c5e0: 652c 206d 6574 613d 276e 616d 653a 2077  e, meta='name: w
-0002c5f0: 6562 6170 7027 290a 2020 2020 2020 2020  ebapp').        
-0002c600: 7365 6c66 2e61 6464 436c 6561 6e75 7028  self.addCleanup(
-0002c610: 6861 726e 6573 732e 636c 6561 6e75 7029  harness.cleanup)
-0002c620: 0a0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
-0002c630: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
-0002c640: 2852 756e 7469 6d65 4572 726f 7229 3a0a  (RuntimeError):.
-0002c650: 2020 2020 2020 2020 2020 2020 6861 726e              harn
-0002c660: 6573 732e 7365 745f 7365 6372 6574 5f63  ess.set_secret_c
-0002c670: 6f6e 7465 6e74 2827 6173 6466 272c 207b  ontent('asdf', {
-0002c680: 2766 6f6f 273a 2027 6261 7227 7d29 0a0a  'foo': 'bar'})..
-0002c690: 2020 2020 6465 6620 7465 7374 5f73 6574      def test_set
-0002c6a0: 5f73 6563 7265 745f 636f 6e74 656e 745f  _secret_content_
-0002c6b0: 696e 7661 6c69 645f 636f 6e74 656e 7428  invalid_content(
-0002c6c0: 7365 6c66 293a 0a20 2020 2020 2020 2068  self):.        h
-0002c6d0: 6172 6e65 7373 203d 206f 7073 2e74 6573  arness = ops.tes
-0002c6e0: 7469 6e67 2e48 6172 6e65 7373 286f 7073  ting.Harness(ops
-0002c6f0: 2e43 6861 726d 4261 7365 2c20 6d65 7461  .CharmBase, meta
-0002c700: 3d27 6e61 6d65 3a20 7765 6261 7070 2729  ='name: webapp')
-0002c710: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
-0002c720: 6443 6c65 616e 7570 2868 6172 6e65 7373  dCleanup(harness
-0002c730: 2e63 6c65 616e 7570 290a 0a20 2020 2020  .cleanup)..     
-0002c740: 2020 2073 6563 7265 745f 6964 203d 2068     secret_id = h
-0002c750: 6172 6e65 7373 2e61 6464 5f6d 6f64 656c  arness.add_model
-0002c760: 5f73 6563 7265 7428 2764 6174 6162 6173  _secret('databas
-0002c770: 6527 2c20 7b27 666f 6f27 3a20 2762 6172  e', {'foo': 'bar
-0002c780: 277d 290a 2020 2020 2020 2020 7769 7468  '}).        with
-0002c790: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
-0002c7a0: 6573 2856 616c 7565 4572 726f 7229 3a0a  es(ValueError):.
-0002c7b0: 2020 2020 2020 2020 2020 2020 6861 726e              harn
-0002c7c0: 6573 732e 7365 745f 7365 6372 6574 5f63  ess.set_secret_c
-0002c7d0: 6f6e 7465 6e74 2873 6563 7265 745f 6964  ontent(secret_id
-0002c7e0: 2c20 7b27 7827 3a20 2779 277d 290a 0a20  , {'x': 'y'}).. 
-0002c7f0: 2020 2064 6566 2074 6573 745f 6772 616e     def test_gran
-0002c800: 745f 7365 6372 6574 5f61 6e64 5f72 6576  t_secret_and_rev
-0002c810: 6f6b 655f 7365 6372 6574 2873 656c 6629  oke_secret(self)
-0002c820: 3a0a 2020 2020 2020 2020 6861 726e 6573  :.        harnes
-0002c830: 7320 3d20 6f70 732e 7465 7374 696e 672e  s = ops.testing.
-0002c840: 4861 726e 6573 7328 6f70 732e 4368 6172  Harness(ops.Char
-0002c850: 6d42 6173 652c 206d 6574 613d 276e 616d  mBase, meta='nam
-0002c860: 653a 2077 6562 6170 7027 290a 2020 2020  e: webapp').    
-0002c870: 2020 2020 7365 6c66 2e61 6464 436c 6561      self.addClea
-0002c880: 6e75 7028 6861 726e 6573 732e 636c 6561  nup(harness.clea
-0002c890: 6e75 7029 0a20 2020 2020 2020 2072 656c  nup).        rel
-0002c8a0: 6174 696f 6e5f 6964 203d 2068 6172 6e65  ation_id = harne
-0002c8b0: 7373 2e61 6464 5f72 656c 6174 696f 6e28  ss.add_relation(
-0002c8c0: 2764 6227 2c20 2764 6174 6162 6173 6527  'db', 'database'
-0002c8d0: 290a 2020 2020 2020 2020 6861 726e 6573  ).        harnes
-0002c8e0: 732e 6164 645f 7265 6c61 7469 6f6e 5f75  s.add_relation_u
-0002c8f0: 6e69 7428 7265 6c61 7469 6f6e 5f69 642c  nit(relation_id,
-0002c900: 2027 6461 7461 6261 7365 2f30 2729 0a0a   'database/0')..
-0002c910: 2020 2020 2020 2020 7365 6372 6574 5f69          secret_i
-0002c920: 6420 3d20 6861 726e 6573 732e 6164 645f  d = harness.add_
-0002c930: 6d6f 6465 6c5f 7365 6372 6574 2827 6461  model_secret('da
-0002c940: 7461 6261 7365 272c 207b 2770 6173 7377  tabase', {'passw
-0002c950: 6f72 6427 3a20 2768 756e 7465 7232 277d  ord': 'hunter2'}
-0002c960: 290a 2020 2020 2020 2020 6861 726e 6573  ).        harnes
-0002c970: 732e 6772 616e 745f 7365 6372 6574 2873  s.grant_secret(s
-0002c980: 6563 7265 745f 6964 2c20 2777 6562 6170  ecret_id, 'webap
-0002c990: 7027 290a 2020 2020 2020 2020 7365 6372  p').        secr
-0002c9a0: 6574 203d 2068 6172 6e65 7373 2e6d 6f64  et = harness.mod
-0002c9b0: 656c 2e67 6574 5f73 6563 7265 7428 6964  el.get_secret(id
-0002c9c0: 3d73 6563 7265 745f 6964 290a 2020 2020  =secret_id).    
-0002c9d0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0002c9e0: 7175 616c 2873 6563 7265 742e 6964 2c20  qual(secret.id, 
-0002c9f0: 7365 6372 6574 5f69 6429 0a20 2020 2020  secret_id).     
-0002ca00: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0002ca10: 7561 6c28 7365 6372 6574 2e67 6574 5f63  ual(secret.get_c
-0002ca20: 6f6e 7465 6e74 2829 2c20 7b27 7061 7373  ontent(), {'pass
-0002ca30: 776f 7264 273a 2027 6875 6e74 6572 3227  word': 'hunter2'
-0002ca40: 7d29 0a0a 2020 2020 2020 2020 6861 726e  })..        harn
-0002ca50: 6573 732e 7265 766f 6b65 5f73 6563 7265  ess.revoke_secre
-0002ca60: 7428 7365 6372 6574 5f69 642c 2027 7765  t(secret_id, 'we
-0002ca70: 6261 7070 2729 0a20 2020 2020 2020 2077  bapp').        w
-0002ca80: 6974 6820 7365 6c66 2e61 7373 6572 7452  ith self.assertR
-0002ca90: 6169 7365 7328 6f70 732e 5365 6372 6574  aises(ops.Secret
-0002caa0: 4e6f 7446 6f75 6e64 4572 726f 7229 3a0a  NotFoundError):.
-0002cab0: 2020 2020 2020 2020 2020 2020 6861 726e              harn
-0002cac0: 6573 732e 6d6f 6465 6c2e 6765 745f 7365  ess.model.get_se
-0002cad0: 6372 6574 2869 643d 7365 6372 6574 5f69  cret(id=secret_i
-0002cae0: 6429 0a0a 2020 2020 6465 6620 7465 7374  d)..    def test
-0002caf0: 5f67 7261 6e74 5f73 6563 7265 745f 7772  _grant_secret_wr
-0002cb00: 6f6e 675f 6170 7028 7365 6c66 293a 0a20  ong_app(self):. 
-0002cb10: 2020 2020 2020 2068 6172 6e65 7373 203d         harness =
-0002cb20: 206f 7073 2e74 6573 7469 6e67 2e48 6172   ops.testing.Har
-0002cb30: 6e65 7373 286f 7073 2e43 6861 726d 4261  ness(ops.CharmBa
-0002cb40: 7365 2c20 6d65 7461 3d27 6e61 6d65 3a20  se, meta='name: 
-0002cb50: 7765 6261 7070 2729 0a20 2020 2020 2020  webapp').       
-0002cb60: 2073 656c 662e 6164 6443 6c65 616e 7570   self.addCleanup
-0002cb70: 2868 6172 6e65 7373 2e63 6c65 616e 7570  (harness.cleanup
-0002cb80: 290a 2020 2020 2020 2020 7265 6c61 7469  ).        relati
-0002cb90: 6f6e 5f69 6420 3d20 6861 726e 6573 732e  on_id = harness.
-0002cba0: 6164 645f 7265 6c61 7469 6f6e 2827 6462  add_relation('db
-0002cbb0: 272c 2027 6461 7461 6261 7365 2729 0a20  ', 'database'). 
-0002cbc0: 2020 2020 2020 2068 6172 6e65 7373 2e61         harness.a
-0002cbd0: 6464 5f72 656c 6174 696f 6e5f 756e 6974  dd_relation_unit
-0002cbe0: 2872 656c 6174 696f 6e5f 6964 2c20 2764  (relation_id, 'd
-0002cbf0: 6174 6162 6173 652f 3027 290a 0a20 2020  atabase/0')..   
-0002cc00: 2020 2020 2073 6563 7265 745f 6964 203d       secret_id =
-0002cc10: 2068 6172 6e65 7373 2e61 6464 5f6d 6f64   harness.add_mod
-0002cc20: 656c 5f73 6563 7265 7428 2764 6174 6162  el_secret('datab
-0002cc30: 6173 6527 2c20 7b27 7061 7373 776f 7264  ase', {'password
-0002cc40: 273a 2027 6875 6e74 6572 3227 7d29 0a20  ': 'hunter2'}). 
-0002cc50: 2020 2020 2020 2068 6172 6e65 7373 2e67         harness.g
-0002cc60: 7261 6e74 5f73 6563 7265 7428 7365 6372  rant_secret(secr
-0002cc70: 6574 5f69 642c 2027 6f74 6865 7261 7070  et_id, 'otherapp
-0002cc80: 2729 0a20 2020 2020 2020 2077 6974 6820  ').        with 
-0002cc90: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
-0002cca0: 7328 6f70 732e 5365 6372 6574 4e6f 7446  s(ops.SecretNotF
-0002ccb0: 6f75 6e64 4572 726f 7229 3a0a 2020 2020  oundError):.    
-0002ccc0: 2020 2020 2020 2020 6861 726e 6573 732e          harness.
-0002ccd0: 6d6f 6465 6c2e 6765 745f 7365 6372 6574  model.get_secret
-0002cce0: 2869 643d 7365 6372 6574 5f69 6429 0a0a  (id=secret_id)..
-0002ccf0: 2020 2020 6465 6620 7465 7374 5f67 7261      def test_gra
-0002cd00: 6e74 5f73 6563 7265 745f 7772 6f6e 675f  nt_secret_wrong_
-0002cd10: 756e 6974 2873 656c 6629 3a0a 2020 2020  unit(self):.    
-0002cd20: 2020 2020 6861 726e 6573 7320 3d20 6f70      harness = op
-0002cd30: 732e 7465 7374 696e 672e 4861 726e 6573  s.testing.Harnes
-0002cd40: 7328 6f70 732e 4368 6172 6d42 6173 652c  s(ops.CharmBase,
-0002cd50: 206d 6574 613d 276e 616d 653a 2077 6562   meta='name: web
-0002cd60: 6170 7027 290a 2020 2020 2020 2020 7365  app').        se
-0002cd70: 6c66 2e61 6464 436c 6561 6e75 7028 6861  lf.addCleanup(ha
-0002cd80: 726e 6573 732e 636c 6561 6e75 7029 0a20  rness.cleanup). 
-0002cd90: 2020 2020 2020 2072 656c 6174 696f 6e5f         relation_
-0002cda0: 6964 203d 2068 6172 6e65 7373 2e61 6464  id = harness.add
-0002cdb0: 5f72 656c 6174 696f 6e28 2764 6227 2c20  _relation('db', 
-0002cdc0: 2764 6174 6162 6173 6527 290a 2020 2020  'database').    
-0002cdd0: 2020 2020 6861 726e 6573 732e 6164 645f      harness.add_
-0002cde0: 7265 6c61 7469 6f6e 5f75 6e69 7428 7265  relation_unit(re
-0002cdf0: 6c61 7469 6f6e 5f69 642c 2027 6461 7461  lation_id, 'data
-0002ce00: 6261 7365 2f30 2729 0a0a 2020 2020 2020  base/0')..      
-0002ce10: 2020 7365 6372 6574 5f69 6420 3d20 6861    secret_id = ha
-0002ce20: 726e 6573 732e 6164 645f 6d6f 6465 6c5f  rness.add_model_
-0002ce30: 7365 6372 6574 2827 6461 7461 6261 7365  secret('database
-0002ce40: 272c 207b 2770 6173 7377 6f72 6427 3a20  ', {'password': 
-0002ce50: 2768 756e 7465 7232 277d 290a 2020 2020  'hunter2'}).    
-0002ce60: 2020 2020 6861 726e 6573 732e 6772 616e      harness.gran
-0002ce70: 745f 7365 6372 6574 2873 6563 7265 745f  t_secret(secret_
-0002ce80: 6964 2c20 2777 6562 6170 702f 3127 2920  id, 'webapp/1') 
-0002ce90: 2023 2073 686f 756c 6420 6265 2077 6562   # should be web
-0002cea0: 6170 702f 300a 2020 2020 2020 2020 7769  app/0.        wi
-0002ceb0: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
-0002cec0: 6973 6573 286f 7073 2e53 6563 7265 744e  ises(ops.SecretN
-0002ced0: 6f74 466f 756e 6445 7272 6f72 293a 0a20  otFoundError):. 
-0002cee0: 2020 2020 2020 2020 2020 2068 6172 6e65             harne
-0002cef0: 7373 2e6d 6f64 656c 2e67 6574 5f73 6563  ss.model.get_sec
-0002cf00: 7265 7428 6964 3d73 6563 7265 745f 6964  ret(id=secret_id
-0002cf10: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-0002cf20: 6772 616e 745f 7365 6372 6574 5f6e 6f5f  grant_secret_no_
-0002cf30: 7265 6c61 7469 6f6e 2873 656c 6629 3a0a  relation(self):.
-0002cf40: 2020 2020 2020 2020 6861 726e 6573 7320          harness 
-0002cf50: 3d20 6f70 732e 7465 7374 696e 672e 4861  = ops.testing.Ha
-0002cf60: 726e 6573 7328 6f70 732e 4368 6172 6d42  rness(ops.CharmB
-0002cf70: 6173 652c 206d 6574 613d 276e 616d 653a  ase, meta='name:
-0002cf80: 2077 6562 6170 7027 290a 2020 2020 2020   webapp').      
-0002cf90: 2020 7365 6c66 2e61 6464 436c 6561 6e75    self.addCleanu
-0002cfa0: 7028 6861 726e 6573 732e 636c 6561 6e75  p(harness.cleanu
-0002cfb0: 7029 0a0a 2020 2020 2020 2020 7365 6372  p)..        secr
-0002cfc0: 6574 5f69 6420 3d20 6861 726e 6573 732e  et_id = harness.
-0002cfd0: 6164 645f 6d6f 6465 6c5f 7365 6372 6574  add_model_secret
-0002cfe0: 2827 6461 7461 6261 7365 272c 207b 2770  ('database', {'p
-0002cff0: 6173 7377 6f72 6427 3a20 2768 756e 7465  assword': 'hunte
-0002d000: 7232 277d 290a 2020 2020 2020 2020 7769  r2'}).        wi
-0002d010: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
-0002d020: 6973 6573 2852 756e 7469 6d65 4572 726f  ises(RuntimeErro
-0002d030: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-0002d040: 6861 726e 6573 732e 6772 616e 745f 7365  harness.grant_se
-0002d050: 6372 6574 2873 6563 7265 745f 6964 2c20  cret(secret_id, 
-0002d060: 2777 6562 6170 7027 290a 0a20 2020 2064  'webapp')..    d
-0002d070: 6566 2074 6573 745f 6765 745f 7365 6372  ef test_get_secr
-0002d080: 6574 5f67 7261 6e74 7328 7365 6c66 293a  et_grants(self):
-0002d090: 0a20 2020 2020 2020 2068 6172 6e65 7373  .        harness
-0002d0a0: 203d 206f 7073 2e74 6573 7469 6e67 2e48   = ops.testing.H
-0002d0b0: 6172 6e65 7373 286f 7073 2e43 6861 726d  arness(ops.Charm
-0002d0c0: 4261 7365 2c20 6d65 7461 3d27 6e61 6d65  Base, meta='name
-0002d0d0: 3a20 6461 7461 6261 7365 2729 0a20 2020  : database').   
-0002d0e0: 2020 2020 2073 656c 662e 6164 6443 6c65       self.addCle
-0002d0f0: 616e 7570 2868 6172 6e65 7373 2e63 6c65  anup(harness.cle
-0002d100: 616e 7570 290a 0a20 2020 2020 2020 2072  anup)..        r
-0002d110: 656c 6174 696f 6e5f 6964 203d 2068 6172  elation_id = har
-0002d120: 6e65 7373 2e61 6464 5f72 656c 6174 696f  ness.add_relatio
-0002d130: 6e28 2764 6227 2c20 2777 6562 6170 7027  n('db', 'webapp'
-0002d140: 290a 2020 2020 2020 2020 6861 726e 6573  ).        harnes
-0002d150: 732e 6164 645f 7265 6c61 7469 6f6e 5f75  s.add_relation_u
-0002d160: 6e69 7428 7265 6c61 7469 6f6e 5f69 642c  nit(relation_id,
-0002d170: 2027 7765 6261 7070 2f30 2729 0a0a 2020   'webapp/0')..  
-0002d180: 2020 2020 2020 7365 6372 6574 203d 2068        secret = h
-0002d190: 6172 6e65 7373 2e6d 6f64 656c 2e61 7070  arness.model.app
-0002d1a0: 2e61 6464 5f73 6563 7265 7428 7b27 666f  .add_secret({'fo
-0002d1b0: 6f27 3a20 2778 277d 290a 2020 2020 2020  o': 'x'}).      
-0002d1c0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0002d1d0: 616c 2868 6172 6e65 7373 2e67 6574 5f73  al(harness.get_s
-0002d1e0: 6563 7265 745f 6772 616e 7473 2873 6563  ecret_grants(sec
-0002d1f0: 7265 742e 6964 2c20 7265 6c61 7469 6f6e  ret.id, relation
-0002d200: 5f69 6429 2c20 7365 7428 2929 0a20 2020  _id), set()).   
-0002d210: 2020 2020 2073 6563 7265 742e 6772 616e       secret.gran
-0002d220: 7428 6861 726e 6573 732e 6d6f 6465 6c2e  t(harness.model.
-0002d230: 6765 745f 7265 6c61 7469 6f6e 2827 6462  get_relation('db
-0002d240: 2729 290a 2020 2020 2020 2020 7365 6c66  ')).        self
-0002d250: 2e61 7373 6572 7445 7175 616c 2868 6172  .assertEqual(har
-0002d260: 6e65 7373 2e67 6574 5f73 6563 7265 745f  ness.get_secret_
-0002d270: 6772 616e 7473 2873 6563 7265 742e 6964  grants(secret.id
-0002d280: 2c20 7265 6c61 7469 6f6e 5f69 6429 2c20  , relation_id), 
-0002d290: 7b27 7765 6261 7070 277d 290a 0a20 2020  {'webapp'})..   
-0002d2a0: 2020 2020 2073 6563 7265 742e 7265 766f       secret.revo
-0002d2b0: 6b65 2868 6172 6e65 7373 2e6d 6f64 656c  ke(harness.model
-0002d2c0: 2e67 6574 5f72 656c 6174 696f 6e28 2764  .get_relation('d
-0002d2d0: 6227 2929 0a20 2020 2020 2020 2073 656c  b')).        sel
-0002d2e0: 662e 6173 7365 7274 4571 7561 6c28 6861  f.assertEqual(ha
-0002d2f0: 726e 6573 732e 6765 745f 7365 6372 6574  rness.get_secret
-0002d300: 5f67 7261 6e74 7328 7365 6372 6574 2e69  _grants(secret.i
-0002d310: 642c 2072 656c 6174 696f 6e5f 6964 292c  d, relation_id),
-0002d320: 2073 6574 2829 290a 2020 2020 2020 2020   set()).        
-0002d330: 7365 6372 6574 2e67 7261 6e74 2868 6172  secret.grant(har
-0002d340: 6e65 7373 2e6d 6f64 656c 2e67 6574 5f72  ness.model.get_r
-0002d350: 656c 6174 696f 6e28 2764 6227 292c 2075  elation('db'), u
-0002d360: 6e69 743d 6861 726e 6573 732e 6d6f 6465  nit=harness.mode
-0002d370: 6c2e 6765 745f 756e 6974 2827 7765 6261  l.get_unit('weba
-0002d380: 7070 2f30 2729 290a 2020 2020 2020 2020  pp/0')).        
-0002d390: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0002d3a0: 2868 6172 6e65 7373 2e67 6574 5f73 6563  (harness.get_sec
-0002d3b0: 7265 745f 6772 616e 7473 2873 6563 7265  ret_grants(secre
-0002d3c0: 742e 6964 2c20 7265 6c61 7469 6f6e 5f69  t.id, relation_i
-0002d3d0: 6429 2c20 7b27 7765 6261 7070 2f30 277d  d), {'webapp/0'}
-0002d3e0: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-0002d3f0: 7472 6967 6765 725f 7365 6372 6574 5f72  trigger_secret_r
-0002d400: 6f74 6174 696f 6e28 7365 6c66 293a 0a20  otation(self):. 
-0002d410: 2020 2020 2020 2068 6172 6e65 7373 203d         harness =
-0002d420: 206f 7073 2e74 6573 7469 6e67 2e48 6172   ops.testing.Har
-0002d430: 6e65 7373 2845 7665 6e74 5265 636f 7264  ness(EventRecord
-0002d440: 6572 2c20 6d65 7461 3d27 6e61 6d65 3a20  er, meta='name: 
-0002d450: 6461 7461 6261 7365 2729 0a20 2020 2020  database').     
-0002d460: 2020 2073 656c 662e 6164 6443 6c65 616e     self.addClean
-0002d470: 7570 2868 6172 6e65 7373 2e63 6c65 616e  up(harness.clean
-0002d480: 7570 290a 0a20 2020 2020 2020 2073 6563  up)..        sec
-0002d490: 7265 7420 3d20 6861 726e 6573 732e 6d6f  ret = harness.mo
-0002d4a0: 6465 6c2e 6170 702e 6164 645f 7365 6372  del.app.add_secr
-0002d4b0: 6574 287b 2766 6f6f 273a 2027 7827 7d2c  et({'foo': 'x'},
-0002d4c0: 206c 6162 656c 3d27 6c62 6c27 290a 2020   label='lbl').  
-0002d4d0: 2020 2020 2020 6861 726e 6573 732e 6265        harness.be
-0002d4e0: 6769 6e28 290a 2020 2020 2020 2020 6861  gin().        ha
-0002d4f0: 726e 6573 732e 6672 616d 6577 6f72 6b2e  rness.framework.
-0002d500: 6f62 7365 7276 6528 6861 726e 6573 732e  observe(harness.
-0002d510: 6368 6172 6d2e 6f6e 2e73 6563 7265 745f  charm.on.secret_
-0002d520: 726f 7461 7465 2c20 6861 726e 6573 732e  rotate, harness.
-0002d530: 6368 6172 6d2e 7265 636f 7264 5f65 7665  charm.record_eve
-0002d540: 6e74 290a 2020 2020 2020 2020 6861 726e  nt).        harn
-0002d550: 6573 732e 7472 6967 6765 725f 7365 6372  ess.trigger_secr
-0002d560: 6574 5f72 6f74 6174 696f 6e28 7365 6372  et_rotation(secr
-0002d570: 6574 2e69 6429 0a20 2020 2020 2020 2068  et.id).        h
-0002d580: 6172 6e65 7373 2e74 7269 6767 6572 5f73  arness.trigger_s
-0002d590: 6563 7265 745f 726f 7461 7469 6f6e 2873  ecret_rotation(s
-0002d5a0: 6563 7265 742e 6964 2c20 6c61 6265 6c3d  ecret.id, label=
-0002d5b0: 276f 7665 7272 6964 6527 290a 0a20 2020  'override')..   
-0002d5c0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0002d5d0: 4571 7561 6c28 6c65 6e28 6861 726e 6573  Equal(len(harnes
-0002d5e0: 732e 6368 6172 6d2e 6576 656e 7473 292c  s.charm.events),
-0002d5f0: 2032 290a 2020 2020 2020 2020 6576 656e   2).        even
-0002d600: 7420 3d20 6861 726e 6573 732e 6368 6172  t = harness.char
-0002d610: 6d2e 6576 656e 7473 5b30 5d0a 2020 2020  m.events[0].    
-0002d620: 2020 2020 7365 6c66 2e61 7373 6572 7449      self.assertI
-0002d630: 7349 6e73 7461 6e63 6528 6576 656e 742c  sInstance(event,
-0002d640: 206f 7073 2e53 6563 7265 7452 6f74 6174   ops.SecretRotat
-0002d650: 6545 7665 6e74 290a 2020 2020 2020 2020  eEvent).        
-0002d660: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0002d670: 2865 7665 6e74 2e73 6563 7265 742e 6c61  (event.secret.la
-0002d680: 6265 6c2c 2027 6c62 6c27 290a 2020 2020  bel, 'lbl').    
-0002d690: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0002d6a0: 7175 616c 2865 7665 6e74 2e73 6563 7265  qual(event.secre
-0002d6b0: 742e 6765 745f 636f 6e74 656e 7428 292c  t.get_content(),
-0002d6c0: 207b 2766 6f6f 273a 2027 7827 7d29 0a20   {'foo': 'x'}). 
-0002d6d0: 2020 2020 2020 2065 7665 6e74 203d 2068         event = h
-0002d6e0: 6172 6e65 7373 2e63 6861 726d 2e65 7665  arness.charm.eve
-0002d6f0: 6e74 735b 315d 0a20 2020 2020 2020 2073  nts[1].        s
-0002d700: 656c 662e 6173 7365 7274 4973 496e 7374  elf.assertIsInst
-0002d710: 616e 6365 2865 7665 6e74 2c20 6f70 732e  ance(event, ops.
-0002d720: 5365 6372 6574 526f 7461 7465 4576 656e  SecretRotateEven
-0002d730: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
-0002d740: 6173 7365 7274 4571 7561 6c28 6576 656e  assertEqual(even
-0002d750: 742e 7365 6372 6574 2e6c 6162 656c 2c20  t.secret.label, 
-0002d760: 276f 7665 7272 6964 6527 290a 2020 2020  'override').    
-0002d770: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0002d780: 7175 616c 2865 7665 6e74 2e73 6563 7265  qual(event.secre
-0002d790: 742e 6765 745f 636f 6e74 656e 7428 292c  t.get_content(),
-0002d7a0: 207b 2766 6f6f 273a 2027 7827 7d29 0a0a   {'foo': 'x'})..
-0002d7b0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0002d7c0: 662e 6173 7365 7274 5261 6973 6573 2852  f.assertRaises(R
-0002d7d0: 756e 7469 6d65 4572 726f 7229 3a0a 2020  untimeError):.  
-0002d7e0: 2020 2020 2020 2020 2020 6861 726e 6573            harnes
-0002d7f0: 732e 7472 6967 6765 725f 7365 6372 6574  s.trigger_secret
-0002d800: 5f72 6f74 6174 696f 6e28 276e 6f73 6563  _rotation('nosec
-0002d810: 7265 7427 290a 0a20 2020 2064 6566 2074  ret')..    def t
-0002d820: 6573 745f 7472 6967 6765 725f 7365 6372  est_trigger_secr
-0002d830: 6574 5f72 656d 6f76 616c 2873 656c 6629  et_removal(self)
-0002d840: 3a0a 2020 2020 2020 2020 6861 726e 6573  :.        harnes
-0002d850: 7320 3d20 6f70 732e 7465 7374 696e 672e  s = ops.testing.
-0002d860: 4861 726e 6573 7328 4576 656e 7452 6563  Harness(EventRec
-0002d870: 6f72 6465 722c 206d 6574 613d 276e 616d  order, meta='nam
-0002d880: 653a 2064 6174 6162 6173 6527 290a 2020  e: database').  
-0002d890: 2020 2020 2020 7365 6c66 2e61 6464 436c        self.addCl
-0002d8a0: 6561 6e75 7028 6861 726e 6573 732e 636c  eanup(harness.cl
-0002d8b0: 6561 6e75 7029 0a0a 2020 2020 2020 2020  eanup)..        
-0002d8c0: 7365 6372 6574 203d 2068 6172 6e65 7373  secret = harness
-0002d8d0: 2e6d 6f64 656c 2e61 7070 2e61 6464 5f73  .model.app.add_s
-0002d8e0: 6563 7265 7428 7b27 666f 6f27 3a20 2778  ecret({'foo': 'x
-0002d8f0: 277d 2c20 6c61 6265 6c3d 276c 626c 2729  '}, label='lbl')
-0002d900: 0a20 2020 2020 2020 2068 6172 6e65 7373  .        harness
-0002d910: 2e62 6567 696e 2829 0a20 2020 2020 2020  .begin().       
-0002d920: 2068 6172 6e65 7373 2e66 7261 6d65 776f   harness.framewo
-0002d930: 726b 2e6f 6273 6572 7665 2868 6172 6e65  rk.observe(harne
-0002d940: 7373 2e63 6861 726d 2e6f 6e2e 7365 6372  ss.charm.on.secr
-0002d950: 6574 5f72 656d 6f76 652c 2068 6172 6e65  et_remove, harne
-0002d960: 7373 2e63 6861 726d 2e72 6563 6f72 645f  ss.charm.record_
-0002d970: 6576 656e 7429 0a20 2020 2020 2020 2068  event).        h
-0002d980: 6172 6e65 7373 2e74 7269 6767 6572 5f73  arness.trigger_s
-0002d990: 6563 7265 745f 7265 6d6f 7661 6c28 7365  ecret_removal(se
-0002d9a0: 6372 6574 2e69 642c 2031 290a 2020 2020  cret.id, 1).    
-0002d9b0: 2020 2020 6861 726e 6573 732e 7472 6967      harness.trig
-0002d9c0: 6765 725f 7365 6372 6574 5f72 656d 6f76  ger_secret_remov
-0002d9d0: 616c 2873 6563 7265 742e 6964 2c20 3432  al(secret.id, 42
-0002d9e0: 2c20 6c61 6265 6c3d 276f 7665 7272 6964  , label='overrid
-0002d9f0: 6527 290a 0a20 2020 2020 2020 2073 656c  e')..        sel
-0002da00: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
-0002da10: 6e28 6861 726e 6573 732e 6368 6172 6d2e  n(harness.charm.
-0002da20: 6576 656e 7473 292c 2032 290a 2020 2020  events), 2).    
-0002da30: 2020 2020 6576 656e 7420 3d20 6861 726e      event = harn
-0002da40: 6573 732e 6368 6172 6d2e 6576 656e 7473  ess.charm.events
-0002da50: 5b30 5d0a 2020 2020 2020 2020 7365 6c66  [0].        self
-0002da60: 2e61 7373 6572 7449 7349 6e73 7461 6e63  .assertIsInstanc
-0002da70: 6528 6576 656e 742c 206f 7073 2e53 6563  e(event, ops.Sec
-0002da80: 7265 7452 656d 6f76 6545 7665 6e74 290a  retRemoveEvent).
-0002da90: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0002daa0: 6572 7445 7175 616c 2865 7665 6e74 2e73  ertEqual(event.s
-0002dab0: 6563 7265 742e 6c61 6265 6c2c 2027 6c62  ecret.label, 'lb
-0002dac0: 6c27 290a 2020 2020 2020 2020 7365 6c66  l').        self
-0002dad0: 2e61 7373 6572 7445 7175 616c 2865 7665  .assertEqual(eve
-0002dae0: 6e74 2e72 6576 6973 696f 6e2c 2031 290a  nt.revision, 1).
-0002daf0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0002db00: 6572 7445 7175 616c 2865 7665 6e74 2e73  ertEqual(event.s
-0002db10: 6563 7265 742e 6765 745f 636f 6e74 656e  ecret.get_conten
-0002db20: 7428 292c 207b 2766 6f6f 273a 2027 7827  t(), {'foo': 'x'
-0002db30: 7d29 0a20 2020 2020 2020 2065 7665 6e74  }).        event
-0002db40: 203d 2068 6172 6e65 7373 2e63 6861 726d   = harness.charm
-0002db50: 2e65 7665 6e74 735b 315d 0a20 2020 2020  .events[1].     
-0002db60: 2020 2073 656c 662e 6173 7365 7274 4973     self.assertIs
-0002db70: 496e 7374 616e 6365 2865 7665 6e74 2c20  Instance(event, 
-0002db80: 6f70 732e 5365 6372 6574 5265 6d6f 7665  ops.SecretRemove
-0002db90: 4576 656e 7429 0a20 2020 2020 2020 2073  Event).        s
-0002dba0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0002dbb0: 6576 656e 742e 7365 6372 6574 2e6c 6162  event.secret.lab
-0002dbc0: 656c 2c20 276f 7665 7272 6964 6527 290a  el, 'override').
-0002dbd0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0002dbe0: 6572 7445 7175 616c 2865 7665 6e74 2e72  ertEqual(event.r
-0002dbf0: 6576 6973 696f 6e2c 2034 3229 0a20 2020  evision, 42).   
-0002dc00: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0002dc10: 4571 7561 6c28 6576 656e 742e 7365 6372  Equal(event.secr
-0002dc20: 6574 2e67 6574 5f63 6f6e 7465 6e74 2829  et.get_content()
-0002dc30: 2c20 7b27 666f 6f27 3a20 2778 277d 290a  , {'foo': 'x'}).
-0002dc40: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-0002dc50: 6c66 2e61 7373 6572 7452 6169 7365 7328  lf.assertRaises(
-0002dc60: 5275 6e74 696d 6545 7272 6f72 293a 0a20  RuntimeError):. 
-0002dc70: 2020 2020 2020 2020 2020 2068 6172 6e65             harne
-0002dc80: 7373 2e74 7269 6767 6572 5f73 6563 7265  ss.trigger_secre
-0002dc90: 745f 7265 6d6f 7661 6c28 276e 6f73 6563  t_removal('nosec
-0002dca0: 7265 7427 2c20 3129 0a0a 2020 2020 6465  ret', 1)..    de
-0002dcb0: 6620 7465 7374 5f74 7269 6767 6572 5f73  f test_trigger_s
-0002dcc0: 6563 7265 745f 6578 7069 7261 7469 6f6e  ecret_expiration
-0002dcd0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0002dce0: 6861 726e 6573 7320 3d20 6f70 732e 7465  harness = ops.te
-0002dcf0: 7374 696e 672e 4861 726e 6573 7328 4576  sting.Harness(Ev
-0002dd00: 656e 7452 6563 6f72 6465 722c 206d 6574  entRecorder, met
-0002dd10: 613d 276e 616d 653a 2064 6174 6162 6173  a='name: databas
-0002dd20: 6527 290a 2020 2020 2020 2020 7365 6c66  e').        self
-0002dd30: 2e61 6464 436c 6561 6e75 7028 6861 726e  .addCleanup(harn
-0002dd40: 6573 732e 636c 6561 6e75 7029 0a0a 2020  ess.cleanup)..  
-0002dd50: 2020 2020 2020 7365 6372 6574 203d 2068        secret = h
-0002dd60: 6172 6e65 7373 2e6d 6f64 656c 2e61 7070  arness.model.app
-0002dd70: 2e61 6464 5f73 6563 7265 7428 7b27 666f  .add_secret({'fo
-0002dd80: 6f27 3a20 2778 277d 2c20 6c61 6265 6c3d  o': 'x'}, label=
-0002dd90: 276c 626c 2729 0a20 2020 2020 2020 2068  'lbl').        h
-0002dda0: 6172 6e65 7373 2e62 6567 696e 2829 0a20  arness.begin(). 
-0002ddb0: 2020 2020 2020 2068 6172 6e65 7373 2e66         harness.f
-0002ddc0: 7261 6d65 776f 726b 2e6f 6273 6572 7665  ramework.observe
-0002ddd0: 2868 6172 6e65 7373 2e63 6861 726d 2e6f  (harness.charm.o
-0002dde0: 6e2e 7365 6372 6574 5f72 656d 6f76 652c  n.secret_remove,
-0002ddf0: 2068 6172 6e65 7373 2e63 6861 726d 2e72   harness.charm.r
-0002de00: 6563 6f72 645f 6576 656e 7429 0a20 2020  ecord_event).   
-0002de10: 2020 2020 2068 6172 6e65 7373 2e74 7269       harness.tri
-0002de20: 6767 6572 5f73 6563 7265 745f 7265 6d6f  gger_secret_remo
-0002de30: 7661 6c28 7365 6372 6574 2e69 642c 2031  val(secret.id, 1
-0002de40: 290a 2020 2020 2020 2020 6861 726e 6573  ).        harnes
-0002de50: 732e 7472 6967 6765 725f 7365 6372 6574  s.trigger_secret
-0002de60: 5f72 656d 6f76 616c 2873 6563 7265 742e  _removal(secret.
-0002de70: 6964 2c20 3432 2c20 6c61 6265 6c3d 276f  id, 42, label='o
-0002de80: 7665 7272 6964 6527 290a 0a20 2020 2020  verride')..     
-0002de90: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-0002dea0: 7561 6c28 6c65 6e28 6861 726e 6573 732e  ual(len(harness.
-0002deb0: 6368 6172 6d2e 6576 656e 7473 292c 2032  charm.events), 2
-0002dec0: 290a 2020 2020 2020 2020 6576 656e 7420  ).        event 
-0002ded0: 3d20 6861 726e 6573 732e 6368 6172 6d2e  = harness.charm.
-0002dee0: 6576 656e 7473 5b30 5d0a 2020 2020 2020  events[0].      
-0002def0: 2020 7365 6c66 2e61 7373 6572 7449 7349    self.assertIsI
-0002df00: 6e73 7461 6e63 6528 6576 656e 742c 206f  nstance(event, o
-0002df10: 7073 2e53 6563 7265 7452 656d 6f76 6545  ps.SecretRemoveE
-0002df20: 7665 6e74 290a 2020 2020 2020 2020 7365  vent).        se
-0002df30: 6c66 2e61 7373 6572 7445 7175 616c 2865  lf.assertEqual(e
-0002df40: 7665 6e74 2e73 6563 7265 742e 6c61 6265  vent.secret.labe
-0002df50: 6c2c 2027 6c62 6c27 290a 2020 2020 2020  l, 'lbl').      
-0002df60: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0002df70: 616c 2865 7665 6e74 2e72 6576 6973 696f  al(event.revisio
-0002df80: 6e2c 2031 290a 2020 2020 2020 2020 7365  n, 1).        se
-0002df90: 6c66 2e61 7373 6572 7445 7175 616c 2865  lf.assertEqual(e
-0002dfa0: 7665 6e74 2e73 6563 7265 742e 6765 745f  vent.secret.get_
-0002dfb0: 636f 6e74 656e 7428 292c 207b 2766 6f6f  content(), {'foo
-0002dfc0: 273a 2027 7827 7d29 0a20 2020 2020 2020  ': 'x'}).       
-0002dfd0: 2065 7665 6e74 203d 2068 6172 6e65 7373   event = harness
-0002dfe0: 2e63 6861 726d 2e65 7665 6e74 735b 315d  .charm.events[1]
-0002dff0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0002e000: 7365 7274 4973 496e 7374 616e 6365 2865  sertIsInstance(e
-0002e010: 7665 6e74 2c20 6f70 732e 5365 6372 6574  vent, ops.Secret
-0002e020: 5265 6d6f 7665 4576 656e 7429 0a20 2020  RemoveEvent).   
-0002e030: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0002e040: 4571 7561 6c28 6576 656e 742e 7365 6372  Equal(event.secr
-0002e050: 6574 2e6c 6162 656c 2c20 276f 7665 7272  et.label, 'overr
-0002e060: 6964 6527 290a 2020 2020 2020 2020 7365  ide').        se
-0002e070: 6c66 2e61 7373 6572 7445 7175 616c 2865  lf.assertEqual(e
-0002e080: 7665 6e74 2e72 6576 6973 696f 6e2c 2034  vent.revision, 4
-0002e090: 3229 0a20 2020 2020 2020 2073 656c 662e  2).        self.
-0002e0a0: 6173 7365 7274 4571 7561 6c28 6576 656e  assertEqual(even
-0002e0b0: 742e 7365 6372 6574 2e67 6574 5f63 6f6e  t.secret.get_con
-0002e0c0: 7465 6e74 2829 2c20 7b27 666f 6f27 3a20  tent(), {'foo': 
-0002e0d0: 2778 277d 290a 0a20 2020 2020 2020 2077  'x'})..        w
-0002e0e0: 6974 6820 7365 6c66 2e61 7373 6572 7452  ith self.assertR
-0002e0f0: 6169 7365 7328 5275 6e74 696d 6545 7272  aises(RuntimeErr
-0002e100: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
-0002e110: 2068 6172 6e65 7373 2e74 7269 6767 6572   harness.trigger
-0002e120: 5f73 6563 7265 745f 7265 6d6f 7661 6c28  _secret_removal(
-0002e130: 276e 6f73 6563 7265 7427 2c20 3129 0a0a  'nosecret', 1)..
-0002e140: 0a63 6c61 7373 2045 7665 6e74 5265 636f  .class EventReco
-0002e150: 7264 6572 286f 7073 2e43 6861 726d 4261  rder(ops.CharmBa
-0002e160: 7365 293a 0a20 2020 2064 6566 205f 5f69  se):.    def __i
-0002e170: 6e69 745f 5f28 7365 6c66 2c20 6672 616d  nit__(self, fram
-0002e180: 6577 6f72 6b29 3a0a 2020 2020 2020 2020  ework):.        
-0002e190: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
-0002e1a0: 2866 7261 6d65 776f 726b 290a 2020 2020  (framework).    
-0002e1b0: 2020 2020 7365 6c66 2e65 7665 6e74 7320      self.events 
-0002e1c0: 3d20 5b5d 0a0a 2020 2020 6465 6620 7265  = []..    def re
-0002e1d0: 636f 7264 5f65 7665 6e74 2873 656c 662c  cord_event(self,
-0002e1e0: 2065 7665 6e74 293a 0a20 2020 2020 2020   event):.       
-0002e1f0: 2073 656c 662e 6576 656e 7473 2e61 7070   self.events.app
-0002e200: 656e 6428 6576 656e 7429 0a0a 0a63 6c61  end(event)...cla
-0002e210: 7373 2054 6573 7450 6f72 7473 2875 6e69  ss TestPorts(uni
-0002e220: 7474 6573 742e 5465 7374 4361 7365 293a  ttest.TestCase):
-0002e230: 0a20 2020 2064 6566 2074 6573 745f 706f  .    def test_po
-0002e240: 7274 7328 7365 6c66 293a 0a20 2020 2020  rts(self):.     
-0002e250: 2020 2068 6172 6e65 7373 203d 206f 7073     harness = ops
-0002e260: 2e74 6573 7469 6e67 2e48 6172 6e65 7373  .testing.Harness
-0002e270: 286f 7073 2e43 6861 726d 4261 7365 2c20  (ops.CharmBase, 
-0002e280: 6d65 7461 3d27 6e61 6d65 3a20 7765 6261  meta='name: weba
-0002e290: 7070 2729 0a20 2020 2020 2020 2073 656c  pp').        sel
-0002e2a0: 662e 6164 6443 6c65 616e 7570 2868 6172  f.addCleanup(har
-0002e2b0: 6e65 7373 2e63 6c65 616e 7570 290a 2020  ness.cleanup).  
-0002e2c0: 2020 2020 2020 756e 6974 203d 2068 6172        unit = har
-0002e2d0: 6e65 7373 2e6d 6f64 656c 2e75 6e69 740a  ness.model.unit.
-0002e2e0: 0a20 2020 2020 2020 2075 6e69 742e 6f70  .        unit.op
-0002e2f0: 656e 5f70 6f72 7428 2774 6370 272c 2038  en_port('tcp', 8
-0002e300: 3038 3029 0a20 2020 2020 2020 2075 6e69  080).        uni
-0002e310: 742e 6f70 656e 5f70 6f72 7428 2775 6470  t.open_port('udp
-0002e320: 272c 2034 3030 3029 0a20 2020 2020 2020  ', 4000).       
-0002e330: 2075 6e69 742e 6f70 656e 5f70 6f72 7428   unit.open_port(
-0002e340: 2769 636d 7027 290a 0a20 2020 2020 2020  'icmp')..       
-0002e350: 2070 6f72 7473 5f73 6574 203d 2075 6e69   ports_set = uni
-0002e360: 742e 6f70 656e 6564 5f70 6f72 7473 2829  t.opened_ports()
-0002e370: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0002e380: 7365 7274 4973 496e 7374 616e 6365 2870  sertIsInstance(p
-0002e390: 6f72 7473 5f73 6574 2c20 7365 7429 0a20  orts_set, set). 
-0002e3a0: 2020 2020 2020 2070 6f72 7473 203d 2073         ports = s
-0002e3b0: 6f72 7465 6428 706f 7274 735f 7365 742c  orted(ports_set,
-0002e3c0: 206b 6579 3d6c 616d 6264 6120 703a 2028   key=lambda p: (
-0002e3d0: 702e 7072 6f74 6f63 6f6c 2c20 702e 706f  p.protocol, p.po
-0002e3e0: 7274 2929 0a20 2020 2020 2020 2073 656c  rt)).        sel
-0002e3f0: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
-0002e400: 6e28 706f 7274 7329 2c20 3329 0a20 2020  n(ports), 3).   
-0002e410: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0002e420: 4973 496e 7374 616e 6365 2870 6f72 7473  IsInstance(ports
-0002e430: 5b30 5d2c 206f 7073 2e4f 7065 6e65 6450  [0], ops.OpenedP
-0002e440: 6f72 7429 0a20 2020 2020 2020 2073 656c  ort).        sel
-0002e450: 662e 6173 7365 7274 4571 7561 6c28 706f  f.assertEqual(po
-0002e460: 7274 735b 305d 2e70 726f 746f 636f 6c2c  rts[0].protocol,
-0002e470: 2027 6963 6d70 2729 0a20 2020 2020 2020   'icmp').       
-0002e480: 2073 656c 662e 6173 7365 7274 4973 4e6f   self.assertIsNo
-0002e490: 6e65 2870 6f72 7473 5b30 5d2e 706f 7274  ne(ports[0].port
-0002e4a0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0002e4b0: 7373 6572 7449 7349 6e73 7461 6e63 6528  ssertIsInstance(
-0002e4c0: 706f 7274 735b 315d 2c20 6f70 732e 4f70  ports[1], ops.Op
-0002e4d0: 656e 6564 506f 7274 290a 2020 2020 2020  enedPort).      
-0002e4e0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0002e4f0: 616c 2870 6f72 7473 5b31 5d2e 7072 6f74  al(ports[1].prot
-0002e500: 6f63 6f6c 2c20 2774 6370 2729 0a20 2020  ocol, 'tcp').   
-0002e510: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0002e520: 4571 7561 6c28 706f 7274 735b 315d 2e70  Equal(ports[1].p
-0002e530: 6f72 742c 2038 3038 3029 0a20 2020 2020  ort, 8080).     
-0002e540: 2020 2073 656c 662e 6173 7365 7274 4973     self.assertIs
-0002e550: 496e 7374 616e 6365 2870 6f72 7473 5b32  Instance(ports[2
-0002e560: 5d2c 206f 7073 2e4f 7065 6e65 6450 6f72  ], ops.OpenedPor
-0002e570: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
-0002e580: 6173 7365 7274 4571 7561 6c28 706f 7274  assertEqual(port
-0002e590: 735b 325d 2e70 726f 746f 636f 6c2c 2027  s[2].protocol, '
-0002e5a0: 7564 7027 290a 2020 2020 2020 2020 7365  udp').        se
-0002e5b0: 6c66 2e61 7373 6572 7445 7175 616c 2870  lf.assertEqual(p
-0002e5c0: 6f72 7473 5b32 5d2e 706f 7274 2c20 3430  orts[2].port, 40
-0002e5d0: 3030 290a 0a20 2020 2020 2020 2075 6e69  00)..        uni
-0002e5e0: 742e 636c 6f73 655f 706f 7274 2827 7463  t.close_port('tc
-0002e5f0: 7027 2c20 3830 3830 290a 2020 2020 2020  p', 8080).      
-0002e600: 2020 756e 6974 2e63 6c6f 7365 5f70 6f72    unit.close_por
-0002e610: 7428 2774 6370 272c 2038 3038 3029 2020  t('tcp', 8080)  
-0002e620: 2320 636c 6f73 696e 6720 7361 6d65 2070  # closing same p
-0002e630: 6f72 7420 6167 6169 6e20 6861 7320 6e6f  ort again has no
-0002e640: 2065 6666 6563 740a 2020 2020 2020 2020   effect.        
-0002e650: 756e 6974 2e63 6c6f 7365 5f70 6f72 7428  unit.close_port(
-0002e660: 2775 6470 272c 2034 3030 3029 0a0a 2020  'udp', 4000)..  
-0002e670: 2020 2020 2020 706f 7274 735f 7365 7420        ports_set 
-0002e680: 3d20 756e 6974 2e6f 7065 6e65 645f 706f  = unit.opened_po
-0002e690: 7274 7328 290a 2020 2020 2020 2020 7365  rts().        se
-0002e6a0: 6c66 2e61 7373 6572 7449 7349 6e73 7461  lf.assertIsInsta
-0002e6b0: 6e63 6528 706f 7274 735f 7365 742c 2073  nce(ports_set, s
-0002e6c0: 6574 290a 2020 2020 2020 2020 706f 7274  et).        port
-0002e6d0: 7320 3d20 736f 7274 6564 2870 6f72 7473  s = sorted(ports
-0002e6e0: 5f73 6574 2c20 6b65 793d 6c61 6d62 6461  _set, key=lambda
-0002e6f0: 2070 3a20 2870 2e70 726f 746f 636f 6c2c   p: (p.protocol,
-0002e700: 2070 2e70 6f72 7429 290a 2020 2020 2020   p.port)).      
-0002e710: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0002e720: 616c 286c 656e 2870 6f72 7473 292c 2031  al(len(ports), 1
-0002e730: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0002e740: 7373 6572 7449 7349 6e73 7461 6e63 6528  ssertIsInstance(
-0002e750: 706f 7274 735b 305d 2c20 6f70 732e 4f70  ports[0], ops.Op
-0002e760: 656e 6564 506f 7274 290a 2020 2020 2020  enedPort).      
-0002e770: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-0002e780: 616c 2870 6f72 7473 5b30 5d2e 7072 6f74  al(ports[0].prot
-0002e790: 6f63 6f6c 2c20 2769 636d 7027 290a 2020  ocol, 'icmp').  
-0002e7a0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0002e7b0: 7449 734e 6f6e 6528 706f 7274 735b 305d  tIsNone(ports[0]
-0002e7c0: 2e70 6f72 7429 0a0a 2020 2020 2020 2020  .port)..        
-0002e7d0: 756e 6974 2e63 6c6f 7365 5f70 6f72 7428  unit.close_port(
-0002e7e0: 2769 636d 7027 290a 0a20 2020 2020 2020  'icmp')..       
-0002e7f0: 2070 6f72 7473 5f73 6574 203d 2075 6e69   ports_set = uni
-0002e800: 742e 6f70 656e 6564 5f70 6f72 7473 2829  t.opened_ports()
-0002e810: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0002e820: 7365 7274 4571 7561 6c28 706f 7274 735f  sertEqual(ports_
-0002e830: 7365 742c 2073 6574 2829 290a 0a20 2020  set, set())..   
-0002e840: 2064 6566 2074 6573 745f 6572 726f 7273   def test_errors
-0002e850: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0002e860: 6861 726e 6573 7320 3d20 6f70 732e 7465  harness = ops.te
-0002e870: 7374 696e 672e 4861 726e 6573 7328 6f70  sting.Harness(op
-0002e880: 732e 4368 6172 6d42 6173 652c 206d 6574  s.CharmBase, met
-0002e890: 613d 276e 616d 653a 2077 6562 6170 7027  a='name: webapp'
-0002e8a0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0002e8b0: 6464 436c 6561 6e75 7028 6861 726e 6573  ddCleanup(harnes
-0002e8c0: 732e 636c 6561 6e75 7029 0a20 2020 2020  s.cleanup).     
-0002e8d0: 2020 2075 6e69 7420 3d20 6861 726e 6573     unit = harnes
-0002e8e0: 732e 6d6f 6465 6c2e 756e 6974 0a0a 2020  s.model.unit..  
-0002e8f0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-0002e900: 6173 7365 7274 5261 6973 6573 286f 7073  assertRaises(ops
-0002e910: 2e4d 6f64 656c 4572 726f 7229 3a0a 2020  .ModelError):.  
-0002e920: 2020 2020 2020 2020 2020 756e 6974 2e6f            unit.o
-0002e930: 7065 6e5f 706f 7274 2827 6963 6d70 272c  pen_port('icmp',
-0002e940: 2038 3038 3029 2020 2320 6963 6d70 2063   8080)  # icmp c
-0002e950: 616e 6e6f 7420 6861 7665 2070 6f72 740a  annot have port.
-0002e960: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-0002e970: 662e 6173 7365 7274 5261 6973 6573 286f  f.assertRaises(o
-0002e980: 7073 2e4d 6f64 656c 4572 726f 7229 3a0a  ps.ModelError):.
-0002e990: 2020 2020 2020 2020 2020 2020 756e 6974              unit
-0002e9a0: 2e6f 7065 6e5f 706f 7274 2827 6674 7027  .open_port('ftp'
-0002e9b0: 2c20 3830 3830 2920 2023 2069 6e76 616c  , 8080)  # inval
-0002e9c0: 6964 2070 726f 746f 636f 6c0a 2020 2020  id protocol.    
-0002e9d0: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
-0002e9e0: 7365 7274 5261 6973 6573 286f 7073 2e4d  sertRaises(ops.M
-0002e9f0: 6f64 656c 4572 726f 7229 3a0a 2020 2020  odelError):.    
-0002ea00: 2020 2020 2020 2020 756e 6974 2e6f 7065          unit.ope
-0002ea10: 6e5f 706f 7274 2827 7463 7027 2920 2023  n_port('tcp')  #
-0002ea20: 2074 6370 206d 7573 7420 6861 7665 2070   tcp must have p
-0002ea30: 6f72 740a 2020 2020 2020 2020 7769 7468  ort.        with
-0002ea40: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
-0002ea50: 6573 286f 7073 2e4d 6f64 656c 4572 726f  es(ops.ModelErro
-0002ea60: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-0002ea70: 756e 6974 2e6f 7065 6e5f 706f 7274 2827  unit.open_port('
-0002ea80: 7564 7027 2920 2023 2075 6470 206d 7573  udp')  # udp mus
-0002ea90: 7420 6861 7665 2070 6f72 740a 2020 2020  t have port.    
-0002eaa0: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
-0002eab0: 7365 7274 5261 6973 6573 286f 7073 2e4d  sertRaises(ops.M
-0002eac0: 6f64 656c 4572 726f 7229 3a0a 2020 2020  odelError):.    
-0002ead0: 2020 2020 2020 2020 756e 6974 2e6f 7065          unit.ope
-0002eae0: 6e5f 706f 7274 2827 7463 7027 2c20 3029  n_port('tcp', 0)
-0002eaf0: 2020 2320 706f 7274 206f 7574 206f 6620    # port out of 
-0002eb00: 7261 6e67 650a 2020 2020 2020 2020 7769  range.        wi
-0002eb10: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
-0002eb20: 6973 6573 286f 7073 2e4d 6f64 656c 4572  ises(ops.ModelEr
-0002eb30: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
-0002eb40: 2020 756e 6974 2e6f 7065 6e5f 706f 7274    unit.open_port
-0002eb50: 2827 7463 7027 2c20 3635 3533 3629 2020  ('tcp', 65536)  
-0002eb60: 2320 706f 7274 206f 7574 206f 6620 7261  # port out of ra
-0002eb70: 6e67 650a                                nge.
+0002a950: 2e62 6567 696e 2829 0a20 2020 2020 2020  .begin().       
+0002a960: 2068 6172 6e65 7373 2e73 6574 5f63 616e   harness.set_can
+0002a970: 5f63 6f6e 6e65 6374 2827 6331 272c 2054  _connect('c1', T
+0002a980: 7275 6529 0a20 2020 2020 2020 2068 6172  rue).        har
+0002a990: 6e65 7373 2e73 6574 5f63 616e 5f63 6f6e  ness.set_can_con
+0002a9a0: 6e65 6374 2827 6332 272c 2054 7275 6529  nect('c2', True)
+0002a9b0: 0a20 2020 2020 2020 2068 6172 6e65 7373  .        harness
+0002a9c0: 2e73 6574 5f63 616e 5f63 6f6e 6e65 6374  .set_can_connect
+0002a9d0: 2827 6333 272c 2054 7275 6529 0a0a 2020  ('c3', True)..  
+0002a9e0: 2020 2020 2020 2320 7075 7368 2066 696c        # push fil
+0002a9f0: 6520 746f 2063 3120 7374 6f72 6167 6520  e to c1 storage 
+0002aa00: 6d6f 756e 742c 2063 6865 636b 2074 6861  mount, check tha
+0002aa10: 7420 7765 2063 616e 2073 6565 2069 7420  t we can see it 
+0002aa20: 696e 2063 6861 726d 2063 6f6e 7461 696e  in charm contain
+0002aa30: 6572 2073 746f 7261 6765 2070 6174 682e  er storage path.
+0002aa40: 0a20 2020 2020 2020 2063 3120 3d20 6861  .        c1 = ha
+0002aa50: 726e 6573 732e 6d6f 6465 6c2e 756e 6974  rness.model.unit
+0002aa60: 2e67 6574 5f63 6f6e 7461 696e 6572 2827  .get_container('
+0002aa70: 6331 2729 0a20 2020 2020 2020 2063 315f  c1').        c1_
+0002aa80: 666e 616d 6520 3d20 2766 6f6f 2e74 7874  fname = 'foo.txt
+0002aa90: 270a 2020 2020 2020 2020 6331 5f66 7061  '.        c1_fpa
+0002aaa0: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
+0002aab0: 6e28 272f 6d6f 756e 7473 2f66 6f6f 272c  n('/mounts/foo',
+0002aac0: 2063 315f 666e 616d 6529 0a20 2020 2020   c1_fname).     
+0002aad0: 2020 2063 312e 7075 7368 2863 315f 6670     c1.push(c1_fp
+0002aae0: 6174 682c 2027 3432 2729 0a20 2020 2020  ath, '42').     
+0002aaf0: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+0002ab00: 7565 2863 312e 6578 6973 7473 2863 315f  ue(c1.exists(c1_
+0002ab10: 6670 6174 6829 290a 2020 2020 2020 2020  fpath)).        
+0002ab20: 6670 6174 6820 3d20 6f73 2e70 6174 682e  fpath = os.path.
+0002ab30: 6a6f 696e 2873 7472 2868 6172 6e65 7373  join(str(harness
+0002ab40: 2e6d 6f64 656c 2e73 746f 7261 6765 735b  .model.storages[
+0002ab50: 2773 746f 7265 3127 5d5b 305d 2e6c 6f63  'store1'][0].loc
+0002ab60: 6174 696f 6e29 2c20 2766 6f6f 2e74 7874  ation), 'foo.txt
+0002ab70: 2729 0a20 2020 2020 2020 2077 6974 6820  ').        with 
+0002ab80: 6f70 656e 2866 7061 7468 2920 6173 2066  open(fpath) as f
+0002ab90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002aba0: 6c66 2e61 7373 6572 7445 7175 616c 2827  lf.assertEqual('
+0002abb0: 3432 272c 2066 2e72 6561 6428 2929 0a0a  42', f.read())..
+0002abc0: 2020 2020 2020 2020 2320 6368 6563 6b20          # check 
+0002abd0: 7468 6174 2074 6865 2066 696c 6520 6973  that the file is
+0002abe0: 206e 6f74 2076 6973 6962 6c65 2069 6e20   not visible in 
+0002abf0: 6332 2077 6869 6368 2068 6173 2061 2064  c2 which has a d
+0002ac00: 6966 6665 7265 6e74 2073 746f 7261 6765  ifferent storage
+0002ac10: 206d 6f75 6e74 0a20 2020 2020 2020 2063   mount.        c
+0002ac20: 3220 3d20 6861 726e 6573 732e 6d6f 6465  2 = harness.mode
+0002ac30: 6c2e 756e 6974 2e67 6574 5f63 6f6e 7461  l.unit.get_conta
+0002ac40: 696e 6572 2827 6332 2729 0a20 2020 2020  iner('c2').     
+0002ac50: 2020 2063 325f 6670 6174 6820 3d20 6f73     c2_fpath = os
+0002ac60: 2e70 6174 682e 6a6f 696e 2827 2f6d 6f75  .path.join('/mou
+0002ac70: 6e74 732f 666f 6f27 2c20 6331 5f66 6e61  nts/foo', c1_fna
+0002ac80: 6d65 290a 2020 2020 2020 2020 7365 6c66  me).        self
+0002ac90: 2e61 7373 6572 7446 616c 7365 2863 322e  .assertFalse(c2.
+0002aca0: 6578 6973 7473 2863 325f 6670 6174 6829  exists(c2_fpath)
+0002acb0: 290a 0a20 2020 2020 2020 2023 2063 6865  )..        # che
+0002acc0: 636b 2074 6861 7420 7468 6520 6669 6c65  ck that the file
+0002acd0: 2069 7320 7669 7369 626c 6520 696e 2063   is visible in c
+0002ace0: 3320 7768 6963 6820 6861 7320 7468 6520  3 which has the 
+0002acf0: 7361 6d65 2073 746f 7261 6765 206d 6f75  same storage mou
+0002ad00: 6e74 0a20 2020 2020 2020 2063 3320 3d20  nt.        c3 = 
+0002ad10: 6861 726e 6573 732e 6d6f 6465 6c2e 756e  harness.model.un
+0002ad20: 6974 2e67 6574 5f63 6f6e 7461 696e 6572  it.get_container
+0002ad30: 2827 6333 2729 0a20 2020 2020 2020 2063  ('c3').        c
+0002ad40: 335f 6670 6174 6820 3d20 6f73 2e70 6174  3_fpath = os.pat
+0002ad50: 682e 6a6f 696e 2827 2f6d 6f75 6e74 732f  h.join('/mounts/
+0002ad60: 6261 7227 2c20 6331 5f66 6e61 6d65 290a  bar', c1_fname).
+0002ad70: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0002ad80: 6572 7454 7275 6528 6333 2e65 7869 7374  ertTrue(c3.exist
+0002ad90: 7328 6333 5f66 7061 7468 2929 0a20 2020  s(c3_fpath)).   
+0002ada0: 2020 2020 2077 6974 6820 6333 2e70 756c       with c3.pul
+0002adb0: 6c28 6333 5f66 7061 7468 2920 6173 2066  l(c3_fpath) as f
+0002adc0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002add0: 6c66 2e61 7373 6572 7445 7175 616c 2827  lf.assertEqual('
+0002ade0: 3432 272c 2066 2e72 6561 6428 2929 0a0a  42', f.read())..
+0002adf0: 2020 2020 2020 2020 2320 7465 7374 2061          # test a
+0002ae00: 6c6c 206f 7468 6572 2063 6f6e 7461 696e  ll other contain
+0002ae10: 6572 2066 696c 6520 6f70 730a 2020 2020  er file ops.    
+0002ae20: 2020 2020 7769 7468 2063 312e 7075 6c6c      with c1.pull
+0002ae30: 2863 315f 6670 6174 6829 2061 7320 663a  (c1_fpath) as f:
+0002ae40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002ae50: 662e 6173 7365 7274 4571 7561 6c28 2734  f.assertEqual('4
+0002ae60: 3227 2c20 662e 7265 6164 2829 290a 2020  2', f.read()).  
+0002ae70: 2020 2020 2020 6669 6c65 7320 3d20 6331        files = c1
+0002ae80: 2e6c 6973 745f 6669 6c65 7328 6331 5f66  .list_files(c1_f
+0002ae90: 7061 7468 290a 2020 2020 2020 2020 7365  path).        se
+0002aea0: 6c66 2e61 7373 6572 7445 7175 616c 285b  lf.assertEqual([
+0002aeb0: 6331 5f66 7061 7468 5d2c 205b 6669 2e70  c1_fpath], [fi.p
+0002aec0: 6174 6820 666f 7220 6669 2069 6e20 6669  ath for fi in fi
+0002aed0: 6c65 735d 290a 2020 2020 2020 2020 6331  les]).        c1
+0002aee0: 2e72 656d 6f76 655f 7061 7468 2863 315f  .remove_path(c1_
+0002aef0: 6670 6174 6829 0a20 2020 2020 2020 2073  fpath).        s
+0002af00: 656c 662e 6173 7365 7274 4661 6c73 6528  elf.assertFalse(
+0002af10: 6331 2e65 7869 7374 7328 6331 5f66 7061  c1.exists(c1_fpa
+0002af20: 7468 2929 0a0a 2020 2020 2020 2020 2320  th))..        # 
+0002af30: 7465 7374 2064 6574 6163 6869 6e67 2073  test detaching s
+0002af40: 746f 7261 6765 0a20 2020 2020 2020 2063  torage.        c
+0002af50: 312e 7075 7368 2863 315f 6670 6174 682c  1.push(c1_fpath,
+0002af60: 2027 3432 2729 0a20 2020 2020 2020 2073   '42').        s
+0002af70: 656c 662e 6173 7365 7274 5472 7565 2863  elf.assertTrue(c
+0002af80: 312e 6578 6973 7473 2863 315f 6670 6174  1.exists(c1_fpat
+0002af90: 6829 290a 2020 2020 2020 2020 7374 6f72  h)).        stor
+0002afa0: 6531 5f69 6420 3d20 6861 726e 6573 732e  e1_id = harness.
+0002afb0: 6d6f 6465 6c2e 7374 6f72 6167 6573 5b27  model.storages['
+0002afc0: 7374 6f72 6531 275d 5b30 5d2e 6675 6c6c  store1'][0].full
+0002afd0: 5f69 640a 2020 2020 2020 2020 6861 726e  _id.        harn
+0002afe0: 6573 732e 7265 6d6f 7665 5f73 746f 7261  ess.remove_stora
+0002aff0: 6765 2873 746f 7265 315f 6964 290a 2020  ge(store1_id).  
+0002b000: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0002b010: 7446 616c 7365 2863 312e 6578 6973 7473  tFalse(c1.exists
+0002b020: 2863 315f 6670 6174 6829 290a 0a20 2020  (c1_fpath))..   
+0002b030: 2064 6566 2074 6573 745f 7075 7368 5f77   def test_push_w
+0002b040: 6974 685f 6f77 6e65 7273 6869 7028 7365  ith_ownership(se
+0002b050: 6c66 293a 0a20 2020 2020 2020 2023 204e  lf):.        # N
+0002b060: 6f74 653a 2054 6f20 7369 6d70 6c69 6679  ote: To simplify
+0002b070: 2069 6d70 6c65 6d65 6e74 6174 696f 6e2c   implementation,
+0002b080: 206f 776e 6572 7368 6970 2069 7320 7369   ownership is si
+0002b090: 6d70 6c79 2073 746f 7265 6420 6173 2d69  mply stored as-i
+0002b0a0: 7320 7769 7468 206e 6f20 7665 7269 6669  s with no verifi
+0002b0b0: 6361 7469 6f6e 2e0a 2020 2020 2020 2020  cation..        
+0002b0c0: 6461 7461 203d 2027 6461 7461 270a 2020  data = 'data'.  
+0002b0d0: 2020 2020 2020 636c 6965 6e74 203d 2073        client = s
+0002b0e0: 656c 662e 636c 6965 6e74 0a20 2020 2020  elf.client.     
+0002b0f0: 2020 2063 6c69 656e 742e 7075 7368 2866     client.push(f
+0002b100: 227b 7365 6c66 2e70 7265 6669 787d 2f66  "{self.prefix}/f
+0002b110: 696c 6522 2c20 6461 7461 2c20 7573 6572  ile", data, user
+0002b120: 5f69 643d 312c 2075 7365 723d 2766 6f6f  _id=1, user='foo
+0002b130: 272c 2067 726f 7570 5f69 643d 332c 2067  ', group_id=3, g
+0002b140: 726f 7570 3d27 6261 7227 290a 2020 2020  roup='bar').    
+0002b150: 2020 2020 6669 6c65 5f20 3d20 636c 6965      file_ = clie
+0002b160: 6e74 2e6c 6973 745f 6669 6c65 7328 6622  nt.list_files(f"
+0002b170: 7b73 656c 662e 7072 6566 6978 7d2f 6669  {self.prefix}/fi
+0002b180: 6c65 2229 5b30 5d0a 2020 2020 2020 2020  le")[0].        
+0002b190: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0002b1a0: 2866 696c 655f 2e75 7365 725f 6964 2c20  (file_.user_id, 
+0002b1b0: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+0002b1c0: 6173 7365 7274 4571 7561 6c28 6669 6c65  assertEqual(file
+0002b1d0: 5f2e 7573 6572 2c20 2766 6f6f 2729 0a20  _.user, 'foo'). 
+0002b1e0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0002b1f0: 7274 4571 7561 6c28 6669 6c65 5f2e 6772  rtEqual(file_.gr
+0002b200: 6f75 705f 6964 2c20 3329 0a20 2020 2020  oup_id, 3).     
+0002b210: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0002b220: 7561 6c28 6669 6c65 5f2e 6772 6f75 702c  ual(file_.group,
+0002b230: 2027 6261 7227 290a 0a20 2020 2064 6566   'bar')..    def
+0002b240: 2074 6573 745f 6d61 6b65 5f64 6972 5f77   test_make_dir_w
+0002b250: 6974 685f 6f77 6e65 7273 6869 7028 7365  ith_ownership(se
+0002b260: 6c66 293a 0a20 2020 2020 2020 2063 6c69  lf):.        cli
+0002b270: 656e 7420 3d20 7365 6c66 2e63 6c69 656e  ent = self.clien
+0002b280: 740a 2020 2020 2020 2020 636c 6965 6e74  t.        client
+0002b290: 2e6d 616b 655f 6469 7228 6622 7b73 656c  .make_dir(f"{sel
+0002b2a0: 662e 7072 6566 6978 7d2f 6469 7231 222c  f.prefix}/dir1",
+0002b2b0: 2075 7365 725f 6964 3d31 2c20 7573 6572   user_id=1, user
+0002b2c0: 3d22 666f 6f22 2c20 6772 6f75 705f 6964  ="foo", group_id
+0002b2d0: 3d33 2c20 6772 6f75 703d 2262 6172 2229  =3, group="bar")
+0002b2e0: 0a20 2020 2020 2020 2064 6972 5f20 3d20  .        dir_ = 
+0002b2f0: 636c 6965 6e74 2e6c 6973 745f 6669 6c65  client.list_file
+0002b300: 7328 6622 7b73 656c 662e 7072 6566 6978  s(f"{self.prefix
+0002b310: 7d2f 6469 7231 222c 2069 7473 656c 663d  }/dir1", itself=
+0002b320: 5472 7565 295b 305d 0a20 2020 2020 2020  True)[0].       
+0002b330: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0002b340: 6c28 6469 725f 2e75 7365 725f 6964 2c20  l(dir_.user_id, 
+0002b350: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+0002b360: 6173 7365 7274 4571 7561 6c28 6469 725f  assertEqual(dir_
+0002b370: 2e75 7365 722c 2022 666f 6f22 290a 2020  .user, "foo").  
+0002b380: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0002b390: 7445 7175 616c 2864 6972 5f2e 6772 6f75  tEqual(dir_.grou
+0002b3a0: 705f 6964 2c20 3329 0a20 2020 2020 2020  p_id, 3).       
+0002b3b0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0002b3c0: 6c28 6469 725f 2e67 726f 7570 2c20 2262  l(dir_.group, "b
+0002b3d0: 6172 2229 0a0a 0a40 756e 6974 7465 7374  ar")...@unittest
+0002b3e0: 2e73 6b69 7055 6e6c 6573 7328 6f73 2e67  .skipUnless(os.g
+0002b3f0: 6574 656e 7628 2752 554e 5f52 4541 4c5f  etenv('RUN_REAL_
+0002b400: 5045 4242 4c45 5f54 4553 5453 2729 2c20  PEBBLE_TESTS'), 
+0002b410: 2752 554e 5f52 4541 4c5f 5045 4242 4c45  'RUN_REAL_PEBBLE
+0002b420: 5f54 4553 5453 206e 6f74 2073 6574 2729  _TESTS not set')
+0002b430: 0a63 6c61 7373 2054 6573 7450 6562 626c  .class TestPebbl
+0002b440: 6553 746f 7261 6765 4150 4973 5573 696e  eStorageAPIsUsin
+0002b450: 6752 6561 6c50 6562 626c 6528 756e 6974  gRealPebble(unit
+0002b460: 7465 7374 2e54 6573 7443 6173 652c 205f  test.TestCase, _
+0002b470: 5065 6262 6c65 5374 6f72 6167 6541 5049  PebbleStorageAPI
+0002b480: 7354 6573 744d 6978 696e 293a 0a20 2020  sTestMixin):.   
+0002b490: 2064 6566 2073 6574 5570 2873 656c 6629   def setUp(self)
+0002b4a0: 3a0a 2020 2020 2020 2020 736f 636b 6574  :.        socket
+0002b4b0: 5f70 6174 6820 3d20 6f73 2e67 6574 656e  _path = os.geten
+0002b4c0: 7628 2750 4542 424c 455f 534f 434b 4554  v('PEBBLE_SOCKET
+0002b4d0: 2729 0a20 2020 2020 2020 2070 6562 626c  ').        pebbl
+0002b4e0: 655f 6469 7220 3d20 6f73 2e67 6574 656e  e_dir = os.geten
+0002b4f0: 7628 2750 4542 424c 4527 290a 2020 2020  v('PEBBLE').    
+0002b500: 2020 2020 6966 206e 6f74 2073 6f63 6b65      if not socke
+0002b510: 745f 7061 7468 2061 6e64 2070 6562 626c  t_path and pebbl
+0002b520: 655f 6469 723a 0a20 2020 2020 2020 2020  e_dir:.         
+0002b530: 2020 2073 6f63 6b65 745f 7061 7468 203d     socket_path =
+0002b540: 206f 732e 7061 7468 2e6a 6f69 6e28 7065   os.path.join(pe
+0002b550: 6262 6c65 5f64 6972 2c20 272e 7065 6262  bble_dir, '.pebb
+0002b560: 6c65 2e73 6f63 6b65 7427 290a 2020 2020  le.socket').    
+0002b570: 2020 2020 6173 7365 7274 2073 6f63 6b65      assert socke
+0002b580: 745f 7061 7468 2061 6e64 2070 6562 626c  t_path and pebbl
+0002b590: 655f 6469 722c 2027 5045 4242 4c45 206d  e_dir, 'PEBBLE m
+0002b5a0: 7573 7420 6265 2073 6574 2069 6620 5255  ust be set if RU
+0002b5b0: 4e5f 5245 414c 5f50 4542 424c 455f 5445  N_REAL_PEBBLE_TE
+0002b5c0: 5354 5320 7365 7427 0a0a 2020 2020 2020  STS set'..      
+0002b5d0: 2020 7365 6c66 2e70 7265 6669 7820 3d20    self.prefix = 
+0002b5e0: 7465 6d70 6669 6c65 2e6d 6b64 7465 6d70  tempfile.mkdtemp
+0002b5f0: 2864 6972 3d70 6562 626c 655f 6469 7229  (dir=pebble_dir)
+0002b600: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
+0002b610: 6965 6e74 203d 2070 6562 626c 652e 436c  ient = pebble.Cl
+0002b620: 6965 6e74 2873 6f63 6b65 745f 7061 7468  ient(socket_path
+0002b630: 3d73 6f63 6b65 745f 7061 7468 290a 0a20  =socket_path).. 
+0002b640: 2020 2064 6566 2074 6561 7244 6f77 6e28     def tearDown(
+0002b650: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+0002b660: 6875 7469 6c2e 726d 7472 6565 2873 656c  hutil.rmtree(sel
+0002b670: 662e 7072 6566 6978 290a 0a20 2020 2023  f.prefix)..    #
+0002b680: 2052 656d 6f76 6520 7468 6973 2065 6e74   Remove this ent
+0002b690: 6972 656c 7920 6f6e 6365 2074 6865 2061  irely once the a
+0002b6a0: 7373 6f63 6961 7465 6420 6275 6720 6973  ssociated bug is
+0002b6b0: 2066 6978 6564 3b20 6974 206f 7665 7272   fixed; it overr
+0002b6c0: 6964 6573 2074 6865 206f 7269 6769 6e61  ides the origina
+0002b6d0: 6c20 7465 7374 2069 6e20 7468 650a 2020  l test in the.  
+0002b6e0: 2020 2320 7465 7374 206d 6978 696e 2063    # test mixin c
+0002b6f0: 6c61 7373 2e0a 2020 2020 4075 6e69 7474  lass..    @unitt
+0002b700: 6573 742e 736b 6970 2827 7065 6e64 696e  est.skip('pendin
+0002b710: 6720 7265 736f 6c75 7469 6f6e 206f 6620  g resolution of 
+0002b720: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0002b730: 6f6d 2f63 616e 6f6e 6963 616c 2f70 6562  om/canonical/peb
+0002b740: 626c 652f 6973 7375 6573 2f38 3027 290a  ble/issues/80').
+0002b750: 2020 2020 6465 6620 7465 7374 5f6d 616b      def test_mak
+0002b760: 655f 6469 725f 7769 7468 5f70 6572 6d69  e_dir_with_permi
+0002b770: 7373 696f 6e5f 6d61 736b 2873 656c 6629  ssion_mask(self)
+0002b780: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+0002b790: 0a63 6c61 7373 2054 6573 7453 6563 7265  .class TestSecre
+0002b7a0: 7473 2875 6e69 7474 6573 742e 5465 7374  ts(unittest.Test
+0002b7b0: 4361 7365 293a 0a20 2020 2064 6566 2074  Case):.    def t
+0002b7c0: 6573 745f 6164 645f 6d6f 6465 6c5f 7365  est_add_model_se
+0002b7d0: 6372 6574 5f62 795f 6170 705f 6e61 6d65  cret_by_app_name
+0002b7e0: 5f73 7472 2873 656c 6629 3a0a 2020 2020  _str(self):.    
+0002b7f0: 2020 2020 6861 726e 6573 7320 3d20 6f70      harness = op
+0002b800: 732e 7465 7374 696e 672e 4861 726e 6573  s.testing.Harnes
+0002b810: 7328 6f70 732e 4368 6172 6d42 6173 652c  s(ops.CharmBase,
+0002b820: 206d 6574 613d 276e 616d 653a 2077 6562   meta='name: web
+0002b830: 6170 7027 290a 2020 2020 2020 2020 7365  app').        se
+0002b840: 6c66 2e61 6464 436c 6561 6e75 7028 6861  lf.addCleanup(ha
+0002b850: 726e 6573 732e 636c 6561 6e75 7029 0a20  rness.cleanup). 
+0002b860: 2020 2020 2020 2072 656c 6174 696f 6e5f         relation_
+0002b870: 6964 203d 2068 6172 6e65 7373 2e61 6464  id = harness.add
+0002b880: 5f72 656c 6174 696f 6e28 2764 6227 2c20  _relation('db', 
+0002b890: 2764 6174 6162 6173 6527 290a 2020 2020  'database').    
+0002b8a0: 2020 2020 6861 726e 6573 732e 6164 645f      harness.add_
+0002b8b0: 7265 6c61 7469 6f6e 5f75 6e69 7428 7265  relation_unit(re
+0002b8c0: 6c61 7469 6f6e 5f69 642c 2027 6461 7461  lation_id, 'data
+0002b8d0: 6261 7365 2f30 2729 0a0a 2020 2020 2020  base/0')..      
+0002b8e0: 2020 7365 6372 6574 5f69 6420 3d20 6861    secret_id = ha
+0002b8f0: 726e 6573 732e 6164 645f 6d6f 6465 6c5f  rness.add_model_
+0002b900: 7365 6372 6574 2827 6461 7461 6261 7365  secret('database
+0002b910: 272c 207b 2770 6173 7377 6f72 6427 3a20  ', {'password': 
+0002b920: 2768 756e 7465 7232 277d 290a 2020 2020  'hunter2'}).    
+0002b930: 2020 2020 6861 726e 6573 732e 6772 616e      harness.gran
+0002b940: 745f 7365 6372 6574 2873 6563 7265 745f  t_secret(secret_
+0002b950: 6964 2c20 2777 6562 6170 7027 290a 2020  id, 'webapp').  
+0002b960: 2020 2020 2020 7365 6372 6574 203d 2068        secret = h
+0002b970: 6172 6e65 7373 2e6d 6f64 656c 2e67 6574  arness.model.get
+0002b980: 5f73 6563 7265 7428 6964 3d73 6563 7265  _secret(id=secre
+0002b990: 745f 6964 290a 2020 2020 2020 2020 7365  t_id).        se
+0002b9a0: 6c66 2e61 7373 6572 7445 7175 616c 2873  lf.assertEqual(s
+0002b9b0: 6563 7265 742e 6964 2c20 7365 6372 6574  ecret.id, secret
+0002b9c0: 5f69 6429 0a20 2020 2020 2020 2073 656c  _id).        sel
+0002b9d0: 662e 6173 7365 7274 4571 7561 6c28 7365  f.assertEqual(se
+0002b9e0: 6372 6574 2e67 6574 5f63 6f6e 7465 6e74  cret.get_content
+0002b9f0: 2829 2c20 7b27 7061 7373 776f 7264 273a  (), {'password':
+0002ba00: 2027 6875 6e74 6572 3227 7d29 0a0a 2020   'hunter2'})..  
+0002ba10: 2020 6465 6620 7465 7374 5f61 6464 5f6d    def test_add_m
+0002ba20: 6f64 656c 5f73 6563 7265 745f 6279 5f61  odel_secret_by_a
+0002ba30: 7070 5f69 6e73 7461 6e63 6528 7365 6c66  pp_instance(self
+0002ba40: 293a 0a20 2020 2020 2020 2068 6172 6e65  ):.        harne
+0002ba50: 7373 203d 206f 7073 2e74 6573 7469 6e67  ss = ops.testing
+0002ba60: 2e48 6172 6e65 7373 286f 7073 2e43 6861  .Harness(ops.Cha
+0002ba70: 726d 4261 7365 2c20 6d65 7461 3d27 6e61  rmBase, meta='na
+0002ba80: 6d65 3a20 7765 6261 7070 2729 0a20 2020  me: webapp').   
+0002ba90: 2020 2020 2073 656c 662e 6164 6443 6c65       self.addCle
+0002baa0: 616e 7570 2868 6172 6e65 7373 2e63 6c65  anup(harness.cle
+0002bab0: 616e 7570 290a 2020 2020 2020 2020 7265  anup).        re
+0002bac0: 6c61 7469 6f6e 5f69 6420 3d20 6861 726e  lation_id = harn
+0002bad0: 6573 732e 6164 645f 7265 6c61 7469 6f6e  ess.add_relation
+0002bae0: 2827 6462 272c 2027 6461 7461 6261 7365  ('db', 'database
+0002baf0: 2729 0a20 2020 2020 2020 2068 6172 6e65  ').        harne
+0002bb00: 7373 2e61 6464 5f72 656c 6174 696f 6e5f  ss.add_relation_
+0002bb10: 756e 6974 2872 656c 6174 696f 6e5f 6964  unit(relation_id
+0002bb20: 2c20 2764 6174 6162 6173 652f 3027 290a  , 'database/0').
+0002bb30: 0a20 2020 2020 2020 2061 7070 203d 2068  .        app = h
+0002bb40: 6172 6e65 7373 2e6d 6f64 656c 2e67 6574  arness.model.get
+0002bb50: 5f61 7070 2827 6461 7461 6261 7365 2729  _app('database')
+0002bb60: 0a20 2020 2020 2020 2073 6563 7265 745f  .        secret_
+0002bb70: 6964 203d 2068 6172 6e65 7373 2e61 6464  id = harness.add
+0002bb80: 5f6d 6f64 656c 5f73 6563 7265 7428 6170  _model_secret(ap
+0002bb90: 702c 207b 2770 6173 7377 6f72 6427 3a20  p, {'password': 
+0002bba0: 2768 756e 7465 7233 277d 290a 2020 2020  'hunter3'}).    
+0002bbb0: 2020 2020 6861 726e 6573 732e 6772 616e      harness.gran
+0002bbc0: 745f 7365 6372 6574 2873 6563 7265 745f  t_secret(secret_
+0002bbd0: 6964 2c20 2777 6562 6170 7027 290a 2020  id, 'webapp').  
+0002bbe0: 2020 2020 2020 7365 6372 6574 203d 2068        secret = h
+0002bbf0: 6172 6e65 7373 2e6d 6f64 656c 2e67 6574  arness.model.get
+0002bc00: 5f73 6563 7265 7428 6964 3d73 6563 7265  _secret(id=secre
+0002bc10: 745f 6964 290a 2020 2020 2020 2020 7365  t_id).        se
+0002bc20: 6c66 2e61 7373 6572 7445 7175 616c 2873  lf.assertEqual(s
+0002bc30: 6563 7265 742e 6964 2c20 7365 6372 6574  ecret.id, secret
+0002bc40: 5f69 6429 0a20 2020 2020 2020 2073 656c  _id).        sel
+0002bc50: 662e 6173 7365 7274 4571 7561 6c28 7365  f.assertEqual(se
+0002bc60: 6372 6574 2e67 6574 5f63 6f6e 7465 6e74  cret.get_content
+0002bc70: 2829 2c20 7b27 7061 7373 776f 7264 273a  (), {'password':
+0002bc80: 2027 6875 6e74 6572 3327 7d29 0a0a 2020   'hunter3'})..  
+0002bc90: 2020 6465 6620 7465 7374 5f61 6464 5f6d    def test_add_m
+0002bca0: 6f64 656c 5f73 6563 7265 745f 6279 5f75  odel_secret_by_u
+0002bcb0: 6e69 745f 696e 7374 616e 6365 2873 656c  nit_instance(sel
+0002bcc0: 6629 3a0a 2020 2020 2020 2020 6861 726e  f):.        harn
+0002bcd0: 6573 7320 3d20 6f70 732e 7465 7374 696e  ess = ops.testin
+0002bce0: 672e 4861 726e 6573 7328 6f70 732e 4368  g.Harness(ops.Ch
+0002bcf0: 6172 6d42 6173 652c 206d 6574 613d 276e  armBase, meta='n
+0002bd00: 616d 653a 2077 6562 6170 7027 290a 2020  ame: webapp').  
+0002bd10: 2020 2020 2020 7365 6c66 2e61 6464 436c        self.addCl
+0002bd20: 6561 6e75 7028 6861 726e 6573 732e 636c  eanup(harness.cl
+0002bd30: 6561 6e75 7029 0a20 2020 2020 2020 2072  eanup).        r
+0002bd40: 656c 6174 696f 6e5f 6964 203d 2068 6172  elation_id = har
+0002bd50: 6e65 7373 2e61 6464 5f72 656c 6174 696f  ness.add_relatio
+0002bd60: 6e28 2764 6227 2c20 2764 6174 6162 6173  n('db', 'databas
+0002bd70: 6527 290a 2020 2020 2020 2020 6861 726e  e').        harn
+0002bd80: 6573 732e 6164 645f 7265 6c61 7469 6f6e  ess.add_relation
+0002bd90: 5f75 6e69 7428 7265 6c61 7469 6f6e 5f69  _unit(relation_i
+0002bda0: 642c 2027 6461 7461 6261 7365 2f30 2729  d, 'database/0')
+0002bdb0: 0a0a 2020 2020 2020 2020 756e 6974 203d  ..        unit =
+0002bdc0: 2068 6172 6e65 7373 2e6d 6f64 656c 2e67   harness.model.g
+0002bdd0: 6574 5f75 6e69 7428 2764 6174 6162 6173  et_unit('databas
+0002bde0: 652f 3027 290a 2020 2020 2020 2020 7365  e/0').        se
+0002bdf0: 6372 6574 5f69 6420 3d20 6861 726e 6573  cret_id = harnes
+0002be00: 732e 6164 645f 6d6f 6465 6c5f 7365 6372  s.add_model_secr
+0002be10: 6574 2875 6e69 742c 207b 2770 6173 7377  et(unit, {'passw
+0002be20: 6f72 6427 3a20 2768 756e 7465 7234 277d  ord': 'hunter4'}
+0002be30: 290a 2020 2020 2020 2020 6861 726e 6573  ).        harnes
+0002be40: 732e 6772 616e 745f 7365 6372 6574 2873  s.grant_secret(s
+0002be50: 6563 7265 745f 6964 2c20 2777 6562 6170  ecret_id, 'webap
+0002be60: 7027 290a 2020 2020 2020 2020 7365 6372  p').        secr
+0002be70: 6574 203d 2068 6172 6e65 7373 2e6d 6f64  et = harness.mod
+0002be80: 656c 2e67 6574 5f73 6563 7265 7428 6964  el.get_secret(id
+0002be90: 3d73 6563 7265 745f 6964 290a 2020 2020  =secret_id).    
+0002bea0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0002beb0: 7175 616c 2873 6563 7265 742e 6964 2c20  qual(secret.id, 
+0002bec0: 7365 6372 6574 5f69 6429 0a20 2020 2020  secret_id).     
+0002bed0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0002bee0: 7561 6c28 7365 6372 6574 2e67 6574 5f63  ual(secret.get_c
+0002bef0: 6f6e 7465 6e74 2829 2c20 7b27 7061 7373  ontent(), {'pass
+0002bf00: 776f 7264 273a 2027 6875 6e74 6572 3427  word': 'hunter4'
+0002bf10: 7d29 0a0a 2020 2020 6465 6620 7465 7374  })..    def test
+0002bf20: 5f61 6464 5f6d 6f64 656c 5f73 6563 7265  _add_model_secre
+0002bf30: 745f 696e 7661 6c69 645f 636f 6e74 656e  t_invalid_conten
+0002bf40: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+0002bf50: 2068 6172 6e65 7373 203d 206f 7073 2e74   harness = ops.t
+0002bf60: 6573 7469 6e67 2e48 6172 6e65 7373 286f  esting.Harness(o
+0002bf70: 7073 2e43 6861 726d 4261 7365 2c20 6d65  ps.CharmBase, me
+0002bf80: 7461 3d27 6e61 6d65 3a20 7765 6261 7070  ta='name: webapp
+0002bf90: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+0002bfa0: 6164 6443 6c65 616e 7570 2868 6172 6e65  addCleanup(harne
+0002bfb0: 7373 2e63 6c65 616e 7570 290a 0a20 2020  ss.cleanup)..   
+0002bfc0: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
+0002bfd0: 7373 6572 7452 6169 7365 7328 5661 6c75  ssertRaises(Valu
+0002bfe0: 6545 7272 6f72 293a 0a20 2020 2020 2020  eError):.       
+0002bff0: 2020 2020 2068 6172 6e65 7373 2e61 6464       harness.add
+0002c000: 5f6d 6f64 656c 5f73 6563 7265 7428 2764  _model_secret('d
+0002c010: 6174 6162 6173 6527 2c20 7b27 7827 3a20  atabase', {'x': 
+0002c020: 2779 277d 2920 2023 206b 6579 2074 6f6f  'y'})  # key too
+0002c030: 2073 686f 7274 0a0a 2020 2020 6465 6620   short..    def 
+0002c040: 7465 7374 5f73 6574 5f73 6563 7265 745f  test_set_secret_
+0002c050: 636f 6e74 656e 7428 7365 6c66 293a 0a20  content(self):. 
+0002c060: 2020 2020 2020 2068 6172 6e65 7373 203d         harness =
+0002c070: 206f 7073 2e74 6573 7469 6e67 2e48 6172   ops.testing.Har
+0002c080: 6e65 7373 2845 7665 6e74 5265 636f 7264  ness(EventRecord
+0002c090: 6572 2c20 6d65 7461 3d27 6e61 6d65 3a20  er, meta='name: 
+0002c0a0: 7765 6261 7070 2729 0a20 2020 2020 2020  webapp').       
+0002c0b0: 2073 656c 662e 6164 6443 6c65 616e 7570   self.addCleanup
+0002c0c0: 2868 6172 6e65 7373 2e63 6c65 616e 7570  (harness.cleanup
+0002c0d0: 290a 2020 2020 2020 2020 7265 6c61 7469  ).        relati
+0002c0e0: 6f6e 5f69 6420 3d20 6861 726e 6573 732e  on_id = harness.
+0002c0f0: 6164 645f 7265 6c61 7469 6f6e 2827 6462  add_relation('db
+0002c100: 272c 2027 6461 7461 6261 7365 2729 0a20  ', 'database'). 
+0002c110: 2020 2020 2020 2068 6172 6e65 7373 2e61         harness.a
+0002c120: 6464 5f72 656c 6174 696f 6e5f 756e 6974  dd_relation_unit
+0002c130: 2872 656c 6174 696f 6e5f 6964 2c20 2764  (relation_id, 'd
+0002c140: 6174 6162 6173 652f 3027 290a 0a20 2020  atabase/0')..   
+0002c150: 2020 2020 2073 6563 7265 745f 6964 203d       secret_id =
+0002c160: 2068 6172 6e65 7373 2e61 6464 5f6d 6f64   harness.add_mod
+0002c170: 656c 5f73 6563 7265 7428 2764 6174 6162  el_secret('datab
+0002c180: 6173 6527 2c20 7b27 666f 6f27 3a20 2731  ase', {'foo': '1
+0002c190: 277d 290a 2020 2020 2020 2020 6861 726e  '}).        harn
+0002c1a0: 6573 732e 6772 616e 745f 7365 6372 6574  ess.grant_secret
+0002c1b0: 2873 6563 7265 745f 6964 2c20 2777 6562  (secret_id, 'web
+0002c1c0: 6170 7027 290a 2020 2020 2020 2020 6861  app').        ha
+0002c1d0: 726e 6573 732e 6265 6769 6e28 290a 2020  rness.begin().  
+0002c1e0: 2020 2020 2020 6861 726e 6573 732e 6672        harness.fr
+0002c1f0: 616d 6577 6f72 6b2e 6f62 7365 7276 6528  amework.observe(
+0002c200: 6861 726e 6573 732e 6368 6172 6d2e 6f6e  harness.charm.on
+0002c210: 2e73 6563 7265 745f 6368 616e 6765 642c  .secret_changed,
+0002c220: 2068 6172 6e65 7373 2e63 6861 726d 2e72   harness.charm.r
+0002c230: 6563 6f72 645f 6576 656e 7429 0a20 2020  ecord_event).   
+0002c240: 2020 2020 2068 6172 6e65 7373 2e73 6574       harness.set
+0002c250: 5f73 6563 7265 745f 636f 6e74 656e 7428  _secret_content(
+0002c260: 7365 6372 6574 5f69 642c 207b 2766 6f6f  secret_id, {'foo
+0002c270: 273a 2027 3227 7d29 0a0a 2020 2020 2020  ': '2'})..      
+0002c280: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0002c290: 616c 286c 656e 2868 6172 6e65 7373 2e63  al(len(harness.c
+0002c2a0: 6861 726d 2e65 7665 6e74 7329 2c20 3129  harm.events), 1)
+0002c2b0: 0a20 2020 2020 2020 2065 7665 6e74 203d  .        event =
+0002c2c0: 2068 6172 6e65 7373 2e63 6861 726d 2e65   harness.charm.e
+0002c2d0: 7665 6e74 735b 305d 0a20 2020 2020 2020  vents[0].       
+0002c2e0: 2073 656c 662e 6173 7365 7274 4973 496e   self.assertIsIn
+0002c2f0: 7374 616e 6365 2865 7665 6e74 2c20 6f70  stance(event, op
+0002c300: 732e 5365 6372 6574 4368 616e 6765 6445  s.SecretChangedE
+0002c310: 7665 6e74 290a 2020 2020 2020 2020 7365  vent).        se
+0002c320: 6c66 2e61 7373 6572 7445 7175 616c 2865  lf.assertEqual(e
+0002c330: 7665 6e74 2e73 6563 7265 742e 6765 745f  vent.secret.get_
+0002c340: 636f 6e74 656e 7428 292c 207b 2766 6f6f  content(), {'foo
+0002c350: 273a 2027 3127 7d29 0a20 2020 2020 2020  ': '1'}).       
+0002c360: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0002c370: 6c28 6576 656e 742e 7365 6372 6574 2e67  l(event.secret.g
+0002c380: 6574 5f63 6f6e 7465 6e74 2872 6566 7265  et_content(refre
+0002c390: 7368 3d54 7275 6529 2c20 7b27 666f 6f27  sh=True), {'foo'
+0002c3a0: 3a20 2732 277d 290a 2020 2020 2020 2020  : '2'}).        
+0002c3b0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0002c3c0: 2865 7665 6e74 2e73 6563 7265 742e 6765  (event.secret.ge
+0002c3d0: 745f 636f 6e74 656e 7428 292c 207b 2766  t_content(), {'f
+0002c3e0: 6f6f 273a 2027 3227 7d29 0a0a 2020 2020  oo': '2'})..    
+0002c3f0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0002c400: 7175 616c 2868 6172 6e65 7373 2e67 6574  qual(harness.get
+0002c410: 5f73 6563 7265 745f 7265 7669 7369 6f6e  _secret_revision
+0002c420: 7328 7365 6372 6574 5f69 6429 2c20 5b31  s(secret_id), [1
+0002c430: 2c20 325d 290a 0a20 2020 2064 6566 2074  , 2])..    def t
+0002c440: 6573 745f 7365 745f 7365 6372 6574 5f63  est_set_secret_c
+0002c450: 6f6e 7465 6e74 5f77 726f 6e67 5f6f 776e  ontent_wrong_own
+0002c460: 6572 2873 656c 6629 3a0a 2020 2020 2020  er(self):.      
+0002c470: 2020 6861 726e 6573 7320 3d20 6f70 732e    harness = ops.
+0002c480: 7465 7374 696e 672e 4861 726e 6573 7328  testing.Harness(
+0002c490: 6f70 732e 4368 6172 6d42 6173 652c 206d  ops.CharmBase, m
+0002c4a0: 6574 613d 276e 616d 653a 2077 6562 6170  eta='name: webap
+0002c4b0: 7027 290a 2020 2020 2020 2020 7365 6c66  p').        self
+0002c4c0: 2e61 6464 436c 6561 6e75 7028 6861 726e  .addCleanup(harn
+0002c4d0: 6573 732e 636c 6561 6e75 7029 0a0a 2020  ess.cleanup)..  
+0002c4e0: 2020 2020 2020 7365 6372 6574 203d 2068        secret = h
+0002c4f0: 6172 6e65 7373 2e6d 6f64 656c 2e61 7070  arness.model.app
+0002c500: 2e61 6464 5f73 6563 7265 7428 7b27 666f  .add_secret({'fo
+0002c510: 6f27 3a20 2762 6172 277d 290a 2020 2020  o': 'bar'}).    
+0002c520: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
+0002c530: 7365 7274 5261 6973 6573 2852 756e 7469  sertRaises(Runti
+0002c540: 6d65 4572 726f 7229 3a0a 2020 2020 2020  meError):.      
+0002c550: 2020 2020 2020 6861 726e 6573 732e 7365        harness.se
+0002c560: 745f 7365 6372 6574 5f63 6f6e 7465 6e74  t_secret_content
+0002c570: 2873 6563 7265 742e 6964 2c20 7b27 6261  (secret.id, {'ba
+0002c580: 7227 3a20 2766 6f6f 277d 290a 0a20 2020  r': 'foo'})..   
+0002c590: 2064 6566 2074 6573 745f 7365 745f 7365   def test_set_se
+0002c5a0: 6372 6574 5f63 6f6e 7465 6e74 5f69 6e76  cret_content_inv
+0002c5b0: 616c 6964 5f73 6563 7265 745f 6964 2873  alid_secret_id(s
+0002c5c0: 656c 6629 3a0a 2020 2020 2020 2020 6861  elf):.        ha
+0002c5d0: 726e 6573 7320 3d20 6f70 732e 7465 7374  rness = ops.test
+0002c5e0: 696e 672e 4861 726e 6573 7328 6f70 732e  ing.Harness(ops.
+0002c5f0: 4368 6172 6d42 6173 652c 206d 6574 613d  CharmBase, meta=
+0002c600: 276e 616d 653a 2077 6562 6170 7027 290a  'name: webapp').
+0002c610: 2020 2020 2020 2020 7365 6c66 2e61 6464          self.add
+0002c620: 436c 6561 6e75 7028 6861 726e 6573 732e  Cleanup(harness.
+0002c630: 636c 6561 6e75 7029 0a0a 2020 2020 2020  cleanup)..      
+0002c640: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
+0002c650: 7274 5261 6973 6573 2852 756e 7469 6d65  rtRaises(Runtime
+0002c660: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
+0002c670: 2020 2020 6861 726e 6573 732e 7365 745f      harness.set_
+0002c680: 7365 6372 6574 5f63 6f6e 7465 6e74 2827  secret_content('
+0002c690: 6173 6466 272c 207b 2766 6f6f 273a 2027  asdf', {'foo': '
+0002c6a0: 6261 7227 7d29 0a0a 2020 2020 6465 6620  bar'})..    def 
+0002c6b0: 7465 7374 5f73 6574 5f73 6563 7265 745f  test_set_secret_
+0002c6c0: 636f 6e74 656e 745f 696e 7661 6c69 645f  content_invalid_
+0002c6d0: 636f 6e74 656e 7428 7365 6c66 293a 0a20  content(self):. 
+0002c6e0: 2020 2020 2020 2068 6172 6e65 7373 203d         harness =
+0002c6f0: 206f 7073 2e74 6573 7469 6e67 2e48 6172   ops.testing.Har
+0002c700: 6e65 7373 286f 7073 2e43 6861 726d 4261  ness(ops.CharmBa
+0002c710: 7365 2c20 6d65 7461 3d27 6e61 6d65 3a20  se, meta='name: 
+0002c720: 7765 6261 7070 2729 0a20 2020 2020 2020  webapp').       
+0002c730: 2073 656c 662e 6164 6443 6c65 616e 7570   self.addCleanup
+0002c740: 2868 6172 6e65 7373 2e63 6c65 616e 7570  (harness.cleanup
+0002c750: 290a 0a20 2020 2020 2020 2073 6563 7265  )..        secre
+0002c760: 745f 6964 203d 2068 6172 6e65 7373 2e61  t_id = harness.a
+0002c770: 6464 5f6d 6f64 656c 5f73 6563 7265 7428  dd_model_secret(
+0002c780: 2764 6174 6162 6173 6527 2c20 7b27 666f  'database', {'fo
+0002c790: 6f27 3a20 2762 6172 277d 290a 2020 2020  o': 'bar'}).    
+0002c7a0: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
+0002c7b0: 7365 7274 5261 6973 6573 2856 616c 7565  sertRaises(Value
+0002c7c0: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
+0002c7d0: 2020 2020 6861 726e 6573 732e 7365 745f      harness.set_
+0002c7e0: 7365 6372 6574 5f63 6f6e 7465 6e74 2873  secret_content(s
+0002c7f0: 6563 7265 745f 6964 2c20 7b27 7827 3a20  ecret_id, {'x': 
+0002c800: 2779 277d 290a 0a20 2020 2064 6566 2074  'y'})..    def t
+0002c810: 6573 745f 6772 616e 745f 7365 6372 6574  est_grant_secret
+0002c820: 5f61 6e64 5f72 6576 6f6b 655f 7365 6372  _and_revoke_secr
+0002c830: 6574 2873 656c 6629 3a0a 2020 2020 2020  et(self):.      
+0002c840: 2020 6861 726e 6573 7320 3d20 6f70 732e    harness = ops.
+0002c850: 7465 7374 696e 672e 4861 726e 6573 7328  testing.Harness(
+0002c860: 6f70 732e 4368 6172 6d42 6173 652c 206d  ops.CharmBase, m
+0002c870: 6574 613d 276e 616d 653a 2077 6562 6170  eta='name: webap
+0002c880: 7027 290a 2020 2020 2020 2020 7365 6c66  p').        self
+0002c890: 2e61 6464 436c 6561 6e75 7028 6861 726e  .addCleanup(harn
+0002c8a0: 6573 732e 636c 6561 6e75 7029 0a20 2020  ess.cleanup).   
+0002c8b0: 2020 2020 2072 656c 6174 696f 6e5f 6964       relation_id
+0002c8c0: 203d 2068 6172 6e65 7373 2e61 6464 5f72   = harness.add_r
+0002c8d0: 656c 6174 696f 6e28 2764 6227 2c20 2764  elation('db', 'd
+0002c8e0: 6174 6162 6173 6527 290a 2020 2020 2020  atabase').      
+0002c8f0: 2020 6861 726e 6573 732e 6164 645f 7265    harness.add_re
+0002c900: 6c61 7469 6f6e 5f75 6e69 7428 7265 6c61  lation_unit(rela
+0002c910: 7469 6f6e 5f69 642c 2027 6461 7461 6261  tion_id, 'databa
+0002c920: 7365 2f30 2729 0a0a 2020 2020 2020 2020  se/0')..        
+0002c930: 7365 6372 6574 5f69 6420 3d20 6861 726e  secret_id = harn
+0002c940: 6573 732e 6164 645f 6d6f 6465 6c5f 7365  ess.add_model_se
+0002c950: 6372 6574 2827 6461 7461 6261 7365 272c  cret('database',
+0002c960: 207b 2770 6173 7377 6f72 6427 3a20 2768   {'password': 'h
+0002c970: 756e 7465 7232 277d 290a 2020 2020 2020  unter2'}).      
+0002c980: 2020 6861 726e 6573 732e 6772 616e 745f    harness.grant_
+0002c990: 7365 6372 6574 2873 6563 7265 745f 6964  secret(secret_id
+0002c9a0: 2c20 2777 6562 6170 7027 290a 2020 2020  , 'webapp').    
+0002c9b0: 2020 2020 7365 6372 6574 203d 2068 6172      secret = har
+0002c9c0: 6e65 7373 2e6d 6f64 656c 2e67 6574 5f73  ness.model.get_s
+0002c9d0: 6563 7265 7428 6964 3d73 6563 7265 745f  ecret(id=secret_
+0002c9e0: 6964 290a 2020 2020 2020 2020 7365 6c66  id).        self
+0002c9f0: 2e61 7373 6572 7445 7175 616c 2873 6563  .assertEqual(sec
+0002ca00: 7265 742e 6964 2c20 7365 6372 6574 5f69  ret.id, secret_i
+0002ca10: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
+0002ca20: 6173 7365 7274 4571 7561 6c28 7365 6372  assertEqual(secr
+0002ca30: 6574 2e67 6574 5f63 6f6e 7465 6e74 2829  et.get_content()
+0002ca40: 2c20 7b27 7061 7373 776f 7264 273a 2027  , {'password': '
+0002ca50: 6875 6e74 6572 3227 7d29 0a0a 2020 2020  hunter2'})..    
+0002ca60: 2020 2020 6861 726e 6573 732e 7265 766f      harness.revo
+0002ca70: 6b65 5f73 6563 7265 7428 7365 6372 6574  ke_secret(secret
+0002ca80: 5f69 642c 2027 7765 6261 7070 2729 0a20  _id, 'webapp'). 
+0002ca90: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+0002caa0: 2e61 7373 6572 7452 6169 7365 7328 6f70  .assertRaises(op
+0002cab0: 732e 5365 6372 6574 4e6f 7446 6f75 6e64  s.SecretNotFound
+0002cac0: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
+0002cad0: 2020 2020 6861 726e 6573 732e 6d6f 6465      harness.mode
+0002cae0: 6c2e 6765 745f 7365 6372 6574 2869 643d  l.get_secret(id=
+0002caf0: 7365 6372 6574 5f69 6429 0a0a 2020 2020  secret_id)..    
+0002cb00: 6465 6620 7465 7374 5f67 7261 6e74 5f73  def test_grant_s
+0002cb10: 6563 7265 745f 7772 6f6e 675f 6170 7028  ecret_wrong_app(
+0002cb20: 7365 6c66 293a 0a20 2020 2020 2020 2068  self):.        h
+0002cb30: 6172 6e65 7373 203d 206f 7073 2e74 6573  arness = ops.tes
+0002cb40: 7469 6e67 2e48 6172 6e65 7373 286f 7073  ting.Harness(ops
+0002cb50: 2e43 6861 726d 4261 7365 2c20 6d65 7461  .CharmBase, meta
+0002cb60: 3d27 6e61 6d65 3a20 7765 6261 7070 2729  ='name: webapp')
+0002cb70: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
+0002cb80: 6443 6c65 616e 7570 2868 6172 6e65 7373  dCleanup(harness
+0002cb90: 2e63 6c65 616e 7570 290a 2020 2020 2020  .cleanup).      
+0002cba0: 2020 7265 6c61 7469 6f6e 5f69 6420 3d20    relation_id = 
+0002cbb0: 6861 726e 6573 732e 6164 645f 7265 6c61  harness.add_rela
+0002cbc0: 7469 6f6e 2827 6462 272c 2027 6461 7461  tion('db', 'data
+0002cbd0: 6261 7365 2729 0a20 2020 2020 2020 2068  base').        h
+0002cbe0: 6172 6e65 7373 2e61 6464 5f72 656c 6174  arness.add_relat
+0002cbf0: 696f 6e5f 756e 6974 2872 656c 6174 696f  ion_unit(relatio
+0002cc00: 6e5f 6964 2c20 2764 6174 6162 6173 652f  n_id, 'database/
+0002cc10: 3027 290a 0a20 2020 2020 2020 2073 6563  0')..        sec
+0002cc20: 7265 745f 6964 203d 2068 6172 6e65 7373  ret_id = harness
+0002cc30: 2e61 6464 5f6d 6f64 656c 5f73 6563 7265  .add_model_secre
+0002cc40: 7428 2764 6174 6162 6173 6527 2c20 7b27  t('database', {'
+0002cc50: 7061 7373 776f 7264 273a 2027 6875 6e74  password': 'hunt
+0002cc60: 6572 3227 7d29 0a20 2020 2020 2020 2068  er2'}).        h
+0002cc70: 6172 6e65 7373 2e67 7261 6e74 5f73 6563  arness.grant_sec
+0002cc80: 7265 7428 7365 6372 6574 5f69 642c 2027  ret(secret_id, '
+0002cc90: 6f74 6865 7261 7070 2729 0a20 2020 2020  otherapp').     
+0002cca0: 2020 2077 6974 6820 7365 6c66 2e61 7373     with self.ass
+0002ccb0: 6572 7452 6169 7365 7328 6f70 732e 5365  ertRaises(ops.Se
+0002ccc0: 6372 6574 4e6f 7446 6f75 6e64 4572 726f  cretNotFoundErro
+0002ccd0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+0002cce0: 6861 726e 6573 732e 6d6f 6465 6c2e 6765  harness.model.ge
+0002ccf0: 745f 7365 6372 6574 2869 643d 7365 6372  t_secret(id=secr
+0002cd00: 6574 5f69 6429 0a0a 2020 2020 6465 6620  et_id)..    def 
+0002cd10: 7465 7374 5f67 7261 6e74 5f73 6563 7265  test_grant_secre
+0002cd20: 745f 7772 6f6e 675f 756e 6974 2873 656c  t_wrong_unit(sel
+0002cd30: 6629 3a0a 2020 2020 2020 2020 6861 726e  f):.        harn
+0002cd40: 6573 7320 3d20 6f70 732e 7465 7374 696e  ess = ops.testin
+0002cd50: 672e 4861 726e 6573 7328 6f70 732e 4368  g.Harness(ops.Ch
+0002cd60: 6172 6d42 6173 652c 206d 6574 613d 276e  armBase, meta='n
+0002cd70: 616d 653a 2077 6562 6170 7027 290a 2020  ame: webapp').  
+0002cd80: 2020 2020 2020 7365 6c66 2e61 6464 436c        self.addCl
+0002cd90: 6561 6e75 7028 6861 726e 6573 732e 636c  eanup(harness.cl
+0002cda0: 6561 6e75 7029 0a20 2020 2020 2020 2072  eanup).        r
+0002cdb0: 656c 6174 696f 6e5f 6964 203d 2068 6172  elation_id = har
+0002cdc0: 6e65 7373 2e61 6464 5f72 656c 6174 696f  ness.add_relatio
+0002cdd0: 6e28 2764 6227 2c20 2764 6174 6162 6173  n('db', 'databas
+0002cde0: 6527 290a 2020 2020 2020 2020 6861 726e  e').        harn
+0002cdf0: 6573 732e 6164 645f 7265 6c61 7469 6f6e  ess.add_relation
+0002ce00: 5f75 6e69 7428 7265 6c61 7469 6f6e 5f69  _unit(relation_i
+0002ce10: 642c 2027 6461 7461 6261 7365 2f30 2729  d, 'database/0')
+0002ce20: 0a0a 2020 2020 2020 2020 7365 6372 6574  ..        secret
+0002ce30: 5f69 6420 3d20 6861 726e 6573 732e 6164  _id = harness.ad
+0002ce40: 645f 6d6f 6465 6c5f 7365 6372 6574 2827  d_model_secret('
+0002ce50: 6461 7461 6261 7365 272c 207b 2770 6173  database', {'pas
+0002ce60: 7377 6f72 6427 3a20 2768 756e 7465 7232  sword': 'hunter2
+0002ce70: 277d 290a 2020 2020 2020 2020 6861 726e  '}).        harn
+0002ce80: 6573 732e 6772 616e 745f 7365 6372 6574  ess.grant_secret
+0002ce90: 2873 6563 7265 745f 6964 2c20 2777 6562  (secret_id, 'web
+0002cea0: 6170 702f 3127 2920 2023 2073 686f 756c  app/1')  # shoul
+0002ceb0: 6420 6265 2077 6562 6170 702f 300a 2020  d be webapp/0.  
+0002cec0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+0002ced0: 6173 7365 7274 5261 6973 6573 286f 7073  assertRaises(ops
+0002cee0: 2e53 6563 7265 744e 6f74 466f 756e 6445  .SecretNotFoundE
+0002cef0: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
+0002cf00: 2020 2068 6172 6e65 7373 2e6d 6f64 656c     harness.model
+0002cf10: 2e67 6574 5f73 6563 7265 7428 6964 3d73  .get_secret(id=s
+0002cf20: 6563 7265 745f 6964 290a 0a20 2020 2064  ecret_id)..    d
+0002cf30: 6566 2074 6573 745f 6772 616e 745f 7365  ef test_grant_se
+0002cf40: 6372 6574 5f6e 6f5f 7265 6c61 7469 6f6e  cret_no_relation
+0002cf50: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0002cf60: 6861 726e 6573 7320 3d20 6f70 732e 7465  harness = ops.te
+0002cf70: 7374 696e 672e 4861 726e 6573 7328 6f70  sting.Harness(op
+0002cf80: 732e 4368 6172 6d42 6173 652c 206d 6574  s.CharmBase, met
+0002cf90: 613d 276e 616d 653a 2077 6562 6170 7027  a='name: webapp'
+0002cfa0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0002cfb0: 6464 436c 6561 6e75 7028 6861 726e 6573  ddCleanup(harnes
+0002cfc0: 732e 636c 6561 6e75 7029 0a0a 2020 2020  s.cleanup)..    
+0002cfd0: 2020 2020 7365 6372 6574 5f69 6420 3d20      secret_id = 
+0002cfe0: 6861 726e 6573 732e 6164 645f 6d6f 6465  harness.add_mode
+0002cff0: 6c5f 7365 6372 6574 2827 6461 7461 6261  l_secret('databa
+0002d000: 7365 272c 207b 2770 6173 7377 6f72 6427  se', {'password'
+0002d010: 3a20 2768 756e 7465 7232 277d 290a 2020  : 'hunter2'}).  
+0002d020: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+0002d030: 6173 7365 7274 5261 6973 6573 2852 756e  assertRaises(Run
+0002d040: 7469 6d65 4572 726f 7229 3a0a 2020 2020  timeError):.    
+0002d050: 2020 2020 2020 2020 6861 726e 6573 732e          harness.
+0002d060: 6772 616e 745f 7365 6372 6574 2873 6563  grant_secret(sec
+0002d070: 7265 745f 6964 2c20 2777 6562 6170 7027  ret_id, 'webapp'
+0002d080: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+0002d090: 6765 745f 7365 6372 6574 5f67 7261 6e74  get_secret_grant
+0002d0a0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+0002d0b0: 2068 6172 6e65 7373 203d 206f 7073 2e74   harness = ops.t
+0002d0c0: 6573 7469 6e67 2e48 6172 6e65 7373 286f  esting.Harness(o
+0002d0d0: 7073 2e43 6861 726d 4261 7365 2c20 6d65  ps.CharmBase, me
+0002d0e0: 7461 3d27 6e61 6d65 3a20 6461 7461 6261  ta='name: databa
+0002d0f0: 7365 2729 0a20 2020 2020 2020 2073 656c  se').        sel
+0002d100: 662e 6164 6443 6c65 616e 7570 2868 6172  f.addCleanup(har
+0002d110: 6e65 7373 2e63 6c65 616e 7570 290a 0a20  ness.cleanup).. 
+0002d120: 2020 2020 2020 2072 656c 6174 696f 6e5f         relation_
+0002d130: 6964 203d 2068 6172 6e65 7373 2e61 6464  id = harness.add
+0002d140: 5f72 656c 6174 696f 6e28 2764 6227 2c20  _relation('db', 
+0002d150: 2777 6562 6170 7027 290a 2020 2020 2020  'webapp').      
+0002d160: 2020 6861 726e 6573 732e 6164 645f 7265    harness.add_re
+0002d170: 6c61 7469 6f6e 5f75 6e69 7428 7265 6c61  lation_unit(rela
+0002d180: 7469 6f6e 5f69 642c 2027 7765 6261 7070  tion_id, 'webapp
+0002d190: 2f30 2729 0a0a 2020 2020 2020 2020 7365  /0')..        se
+0002d1a0: 6372 6574 203d 2068 6172 6e65 7373 2e6d  cret = harness.m
+0002d1b0: 6f64 656c 2e61 7070 2e61 6464 5f73 6563  odel.app.add_sec
+0002d1c0: 7265 7428 7b27 666f 6f27 3a20 2778 277d  ret({'foo': 'x'}
+0002d1d0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0002d1e0: 7373 6572 7445 7175 616c 2868 6172 6e65  ssertEqual(harne
+0002d1f0: 7373 2e67 6574 5f73 6563 7265 745f 6772  ss.get_secret_gr
+0002d200: 616e 7473 2873 6563 7265 742e 6964 2c20  ants(secret.id, 
+0002d210: 7265 6c61 7469 6f6e 5f69 6429 2c20 7365  relation_id), se
+0002d220: 7428 2929 0a20 2020 2020 2020 2073 6563  t()).        sec
+0002d230: 7265 742e 6772 616e 7428 6861 726e 6573  ret.grant(harnes
+0002d240: 732e 6d6f 6465 6c2e 6765 745f 7265 6c61  s.model.get_rela
+0002d250: 7469 6f6e 2827 6462 2729 290a 2020 2020  tion('db')).    
+0002d260: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0002d270: 7175 616c 2868 6172 6e65 7373 2e67 6574  qual(harness.get
+0002d280: 5f73 6563 7265 745f 6772 616e 7473 2873  _secret_grants(s
+0002d290: 6563 7265 742e 6964 2c20 7265 6c61 7469  ecret.id, relati
+0002d2a0: 6f6e 5f69 6429 2c20 7b27 7765 6261 7070  on_id), {'webapp
+0002d2b0: 277d 290a 0a20 2020 2020 2020 2073 6563  '})..        sec
+0002d2c0: 7265 742e 7265 766f 6b65 2868 6172 6e65  ret.revoke(harne
+0002d2d0: 7373 2e6d 6f64 656c 2e67 6574 5f72 656c  ss.model.get_rel
+0002d2e0: 6174 696f 6e28 2764 6227 2929 0a20 2020  ation('db')).   
+0002d2f0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0002d300: 4571 7561 6c28 6861 726e 6573 732e 6765  Equal(harness.ge
+0002d310: 745f 7365 6372 6574 5f67 7261 6e74 7328  t_secret_grants(
+0002d320: 7365 6372 6574 2e69 642c 2072 656c 6174  secret.id, relat
+0002d330: 696f 6e5f 6964 292c 2073 6574 2829 290a  ion_id), set()).
+0002d340: 2020 2020 2020 2020 7365 6372 6574 2e67          secret.g
+0002d350: 7261 6e74 2868 6172 6e65 7373 2e6d 6f64  rant(harness.mod
+0002d360: 656c 2e67 6574 5f72 656c 6174 696f 6e28  el.get_relation(
+0002d370: 2764 6227 292c 2075 6e69 743d 6861 726e  'db'), unit=harn
+0002d380: 6573 732e 6d6f 6465 6c2e 6765 745f 756e  ess.model.get_un
+0002d390: 6974 2827 7765 6261 7070 2f30 2729 290a  it('webapp/0')).
+0002d3a0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0002d3b0: 6572 7445 7175 616c 2868 6172 6e65 7373  ertEqual(harness
+0002d3c0: 2e67 6574 5f73 6563 7265 745f 6772 616e  .get_secret_gran
+0002d3d0: 7473 2873 6563 7265 742e 6964 2c20 7265  ts(secret.id, re
+0002d3e0: 6c61 7469 6f6e 5f69 6429 2c20 7b27 7765  lation_id), {'we
+0002d3f0: 6261 7070 2f30 277d 290a 0a20 2020 2064  bapp/0'})..    d
+0002d400: 6566 2074 6573 745f 7472 6967 6765 725f  ef test_trigger_
+0002d410: 7365 6372 6574 5f72 6f74 6174 696f 6e28  secret_rotation(
+0002d420: 7365 6c66 293a 0a20 2020 2020 2020 2068  self):.        h
+0002d430: 6172 6e65 7373 203d 206f 7073 2e74 6573  arness = ops.tes
+0002d440: 7469 6e67 2e48 6172 6e65 7373 2845 7665  ting.Harness(Eve
+0002d450: 6e74 5265 636f 7264 6572 2c20 6d65 7461  ntRecorder, meta
+0002d460: 3d27 6e61 6d65 3a20 6461 7461 6261 7365  ='name: database
+0002d470: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+0002d480: 6164 6443 6c65 616e 7570 2868 6172 6e65  addCleanup(harne
+0002d490: 7373 2e63 6c65 616e 7570 290a 0a20 2020  ss.cleanup)..   
+0002d4a0: 2020 2020 2073 6563 7265 7420 3d20 6861       secret = ha
+0002d4b0: 726e 6573 732e 6d6f 6465 6c2e 6170 702e  rness.model.app.
+0002d4c0: 6164 645f 7365 6372 6574 287b 2766 6f6f  add_secret({'foo
+0002d4d0: 273a 2027 7827 7d2c 206c 6162 656c 3d27  ': 'x'}, label='
+0002d4e0: 6c62 6c27 290a 2020 2020 2020 2020 6861  lbl').        ha
+0002d4f0: 726e 6573 732e 6265 6769 6e28 290a 2020  rness.begin().  
+0002d500: 2020 2020 2020 6861 726e 6573 732e 6672        harness.fr
+0002d510: 616d 6577 6f72 6b2e 6f62 7365 7276 6528  amework.observe(
+0002d520: 6861 726e 6573 732e 6368 6172 6d2e 6f6e  harness.charm.on
+0002d530: 2e73 6563 7265 745f 726f 7461 7465 2c20  .secret_rotate, 
+0002d540: 6861 726e 6573 732e 6368 6172 6d2e 7265  harness.charm.re
+0002d550: 636f 7264 5f65 7665 6e74 290a 2020 2020  cord_event).    
+0002d560: 2020 2020 6861 726e 6573 732e 7472 6967      harness.trig
+0002d570: 6765 725f 7365 6372 6574 5f72 6f74 6174  ger_secret_rotat
+0002d580: 696f 6e28 7365 6372 6574 2e69 6429 0a20  ion(secret.id). 
+0002d590: 2020 2020 2020 2068 6172 6e65 7373 2e74         harness.t
+0002d5a0: 7269 6767 6572 5f73 6563 7265 745f 726f  rigger_secret_ro
+0002d5b0: 7461 7469 6f6e 2873 6563 7265 742e 6964  tation(secret.id
+0002d5c0: 2c20 6c61 6265 6c3d 276f 7665 7272 6964  , label='overrid
+0002d5d0: 6527 290a 0a20 2020 2020 2020 2073 656c  e')..        sel
+0002d5e0: 662e 6173 7365 7274 4571 7561 6c28 6c65  f.assertEqual(le
+0002d5f0: 6e28 6861 726e 6573 732e 6368 6172 6d2e  n(harness.charm.
+0002d600: 6576 656e 7473 292c 2032 290a 2020 2020  events), 2).    
+0002d610: 2020 2020 6576 656e 7420 3d20 6861 726e      event = harn
+0002d620: 6573 732e 6368 6172 6d2e 6576 656e 7473  ess.charm.events
+0002d630: 5b30 5d0a 2020 2020 2020 2020 7365 6c66  [0].        self
+0002d640: 2e61 7373 6572 7449 7349 6e73 7461 6e63  .assertIsInstanc
+0002d650: 6528 6576 656e 742c 206f 7073 2e53 6563  e(event, ops.Sec
+0002d660: 7265 7452 6f74 6174 6545 7665 6e74 290a  retRotateEvent).
+0002d670: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0002d680: 6572 7445 7175 616c 2865 7665 6e74 2e73  ertEqual(event.s
+0002d690: 6563 7265 742e 6c61 6265 6c2c 2027 6c62  ecret.label, 'lb
+0002d6a0: 6c27 290a 2020 2020 2020 2020 7365 6c66  l').        self
+0002d6b0: 2e61 7373 6572 7445 7175 616c 2865 7665  .assertEqual(eve
+0002d6c0: 6e74 2e73 6563 7265 742e 6765 745f 636f  nt.secret.get_co
+0002d6d0: 6e74 656e 7428 292c 207b 2766 6f6f 273a  ntent(), {'foo':
+0002d6e0: 2027 7827 7d29 0a20 2020 2020 2020 2065   'x'}).        e
+0002d6f0: 7665 6e74 203d 2068 6172 6e65 7373 2e63  vent = harness.c
+0002d700: 6861 726d 2e65 7665 6e74 735b 315d 0a20  harm.events[1]. 
+0002d710: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0002d720: 7274 4973 496e 7374 616e 6365 2865 7665  rtIsInstance(eve
+0002d730: 6e74 2c20 6f70 732e 5365 6372 6574 526f  nt, ops.SecretRo
+0002d740: 7461 7465 4576 656e 7429 0a20 2020 2020  tateEvent).     
+0002d750: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0002d760: 7561 6c28 6576 656e 742e 7365 6372 6574  ual(event.secret
+0002d770: 2e6c 6162 656c 2c20 276f 7665 7272 6964  .label, 'overrid
+0002d780: 6527 290a 2020 2020 2020 2020 7365 6c66  e').        self
+0002d790: 2e61 7373 6572 7445 7175 616c 2865 7665  .assertEqual(eve
+0002d7a0: 6e74 2e73 6563 7265 742e 6765 745f 636f  nt.secret.get_co
+0002d7b0: 6e74 656e 7428 292c 207b 2766 6f6f 273a  ntent(), {'foo':
+0002d7c0: 2027 7827 7d29 0a0a 2020 2020 2020 2020   'x'})..        
+0002d7d0: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
+0002d7e0: 5261 6973 6573 2852 756e 7469 6d65 4572  Raises(RuntimeEr
+0002d7f0: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
+0002d800: 2020 6861 726e 6573 732e 7472 6967 6765    harness.trigge
+0002d810: 725f 7365 6372 6574 5f72 6f74 6174 696f  r_secret_rotatio
+0002d820: 6e28 276e 6f73 6563 7265 7427 290a 0a20  n('nosecret').. 
+0002d830: 2020 2064 6566 2074 6573 745f 7472 6967     def test_trig
+0002d840: 6765 725f 7365 6372 6574 5f72 656d 6f76  ger_secret_remov
+0002d850: 616c 2873 656c 6629 3a0a 2020 2020 2020  al(self):.      
+0002d860: 2020 6861 726e 6573 7320 3d20 6f70 732e    harness = ops.
+0002d870: 7465 7374 696e 672e 4861 726e 6573 7328  testing.Harness(
+0002d880: 4576 656e 7452 6563 6f72 6465 722c 206d  EventRecorder, m
+0002d890: 6574 613d 276e 616d 653a 2064 6174 6162  eta='name: datab
+0002d8a0: 6173 6527 290a 2020 2020 2020 2020 7365  ase').        se
+0002d8b0: 6c66 2e61 6464 436c 6561 6e75 7028 6861  lf.addCleanup(ha
+0002d8c0: 726e 6573 732e 636c 6561 6e75 7029 0a0a  rness.cleanup)..
+0002d8d0: 2020 2020 2020 2020 7365 6372 6574 203d          secret =
+0002d8e0: 2068 6172 6e65 7373 2e6d 6f64 656c 2e61   harness.model.a
+0002d8f0: 7070 2e61 6464 5f73 6563 7265 7428 7b27  pp.add_secret({'
+0002d900: 666f 6f27 3a20 2778 277d 2c20 6c61 6265  foo': 'x'}, labe
+0002d910: 6c3d 276c 626c 2729 0a20 2020 2020 2020  l='lbl').       
+0002d920: 2068 6172 6e65 7373 2e62 6567 696e 2829   harness.begin()
+0002d930: 0a20 2020 2020 2020 2068 6172 6e65 7373  .        harness
+0002d940: 2e66 7261 6d65 776f 726b 2e6f 6273 6572  .framework.obser
+0002d950: 7665 2868 6172 6e65 7373 2e63 6861 726d  ve(harness.charm
+0002d960: 2e6f 6e2e 7365 6372 6574 5f72 656d 6f76  .on.secret_remov
+0002d970: 652c 2068 6172 6e65 7373 2e63 6861 726d  e, harness.charm
+0002d980: 2e72 6563 6f72 645f 6576 656e 7429 0a20  .record_event). 
+0002d990: 2020 2020 2020 2068 6172 6e65 7373 2e74         harness.t
+0002d9a0: 7269 6767 6572 5f73 6563 7265 745f 7265  rigger_secret_re
+0002d9b0: 6d6f 7661 6c28 7365 6372 6574 2e69 642c  moval(secret.id,
+0002d9c0: 2031 290a 2020 2020 2020 2020 6861 726e   1).        harn
+0002d9d0: 6573 732e 7472 6967 6765 725f 7365 6372  ess.trigger_secr
+0002d9e0: 6574 5f72 656d 6f76 616c 2873 6563 7265  et_removal(secre
+0002d9f0: 742e 6964 2c20 3432 2c20 6c61 6265 6c3d  t.id, 42, label=
+0002da00: 276f 7665 7272 6964 6527 290a 0a20 2020  'override')..   
+0002da10: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0002da20: 4571 7561 6c28 6c65 6e28 6861 726e 6573  Equal(len(harnes
+0002da30: 732e 6368 6172 6d2e 6576 656e 7473 292c  s.charm.events),
+0002da40: 2032 290a 2020 2020 2020 2020 6576 656e   2).        even
+0002da50: 7420 3d20 6861 726e 6573 732e 6368 6172  t = harness.char
+0002da60: 6d2e 6576 656e 7473 5b30 5d0a 2020 2020  m.events[0].    
+0002da70: 2020 2020 7365 6c66 2e61 7373 6572 7449      self.assertI
+0002da80: 7349 6e73 7461 6e63 6528 6576 656e 742c  sInstance(event,
+0002da90: 206f 7073 2e53 6563 7265 7452 656d 6f76   ops.SecretRemov
+0002daa0: 6545 7665 6e74 290a 2020 2020 2020 2020  eEvent).        
+0002dab0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0002dac0: 2865 7665 6e74 2e73 6563 7265 742e 6c61  (event.secret.la
+0002dad0: 6265 6c2c 2027 6c62 6c27 290a 2020 2020  bel, 'lbl').    
+0002dae0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0002daf0: 7175 616c 2865 7665 6e74 2e72 6576 6973  qual(event.revis
+0002db00: 696f 6e2c 2031 290a 2020 2020 2020 2020  ion, 1).        
+0002db10: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0002db20: 2865 7665 6e74 2e73 6563 7265 742e 6765  (event.secret.ge
+0002db30: 745f 636f 6e74 656e 7428 292c 207b 2766  t_content(), {'f
+0002db40: 6f6f 273a 2027 7827 7d29 0a20 2020 2020  oo': 'x'}).     
+0002db50: 2020 2065 7665 6e74 203d 2068 6172 6e65     event = harne
+0002db60: 7373 2e63 6861 726d 2e65 7665 6e74 735b  ss.charm.events[
+0002db70: 315d 0a20 2020 2020 2020 2073 656c 662e  1].        self.
+0002db80: 6173 7365 7274 4973 496e 7374 616e 6365  assertIsInstance
+0002db90: 2865 7665 6e74 2c20 6f70 732e 5365 6372  (event, ops.Secr
+0002dba0: 6574 5265 6d6f 7665 4576 656e 7429 0a20  etRemoveEvent). 
+0002dbb0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0002dbc0: 7274 4571 7561 6c28 6576 656e 742e 7365  rtEqual(event.se
+0002dbd0: 6372 6574 2e6c 6162 656c 2c20 276f 7665  cret.label, 'ove
+0002dbe0: 7272 6964 6527 290a 2020 2020 2020 2020  rride').        
+0002dbf0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0002dc00: 2865 7665 6e74 2e72 6576 6973 696f 6e2c  (event.revision,
+0002dc10: 2034 3229 0a20 2020 2020 2020 2073 656c   42).        sel
+0002dc20: 662e 6173 7365 7274 4571 7561 6c28 6576  f.assertEqual(ev
+0002dc30: 656e 742e 7365 6372 6574 2e67 6574 5f63  ent.secret.get_c
+0002dc40: 6f6e 7465 6e74 2829 2c20 7b27 666f 6f27  ontent(), {'foo'
+0002dc50: 3a20 2778 277d 290a 0a20 2020 2020 2020  : 'x'})..       
+0002dc60: 2077 6974 6820 7365 6c66 2e61 7373 6572   with self.asser
+0002dc70: 7452 6169 7365 7328 5275 6e74 696d 6545  tRaises(RuntimeE
+0002dc80: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
+0002dc90: 2020 2068 6172 6e65 7373 2e74 7269 6767     harness.trigg
+0002dca0: 6572 5f73 6563 7265 745f 7265 6d6f 7661  er_secret_remova
+0002dcb0: 6c28 276e 6f73 6563 7265 7427 2c20 3129  l('nosecret', 1)
+0002dcc0: 0a0a 2020 2020 6465 6620 7465 7374 5f74  ..    def test_t
+0002dcd0: 7269 6767 6572 5f73 6563 7265 745f 6578  rigger_secret_ex
+0002dce0: 7069 7261 7469 6f6e 2873 656c 6629 3a0a  piration(self):.
+0002dcf0: 2020 2020 2020 2020 6861 726e 6573 7320          harness 
+0002dd00: 3d20 6f70 732e 7465 7374 696e 672e 4861  = ops.testing.Ha
+0002dd10: 726e 6573 7328 4576 656e 7452 6563 6f72  rness(EventRecor
+0002dd20: 6465 722c 206d 6574 613d 276e 616d 653a  der, meta='name:
+0002dd30: 2064 6174 6162 6173 6527 290a 2020 2020   database').    
+0002dd40: 2020 2020 7365 6c66 2e61 6464 436c 6561      self.addClea
+0002dd50: 6e75 7028 6861 726e 6573 732e 636c 6561  nup(harness.clea
+0002dd60: 6e75 7029 0a0a 2020 2020 2020 2020 7365  nup)..        se
+0002dd70: 6372 6574 203d 2068 6172 6e65 7373 2e6d  cret = harness.m
+0002dd80: 6f64 656c 2e61 7070 2e61 6464 5f73 6563  odel.app.add_sec
+0002dd90: 7265 7428 7b27 666f 6f27 3a20 2778 277d  ret({'foo': 'x'}
+0002dda0: 2c20 6c61 6265 6c3d 276c 626c 2729 0a20  , label='lbl'). 
+0002ddb0: 2020 2020 2020 2068 6172 6e65 7373 2e62         harness.b
+0002ddc0: 6567 696e 2829 0a20 2020 2020 2020 2068  egin().        h
+0002ddd0: 6172 6e65 7373 2e66 7261 6d65 776f 726b  arness.framework
+0002dde0: 2e6f 6273 6572 7665 2868 6172 6e65 7373  .observe(harness
+0002ddf0: 2e63 6861 726d 2e6f 6e2e 7365 6372 6574  .charm.on.secret
+0002de00: 5f72 656d 6f76 652c 2068 6172 6e65 7373  _remove, harness
+0002de10: 2e63 6861 726d 2e72 6563 6f72 645f 6576  .charm.record_ev
+0002de20: 656e 7429 0a20 2020 2020 2020 2068 6172  ent).        har
+0002de30: 6e65 7373 2e74 7269 6767 6572 5f73 6563  ness.trigger_sec
+0002de40: 7265 745f 7265 6d6f 7661 6c28 7365 6372  ret_removal(secr
+0002de50: 6574 2e69 642c 2031 290a 2020 2020 2020  et.id, 1).      
+0002de60: 2020 6861 726e 6573 732e 7472 6967 6765    harness.trigge
+0002de70: 725f 7365 6372 6574 5f72 656d 6f76 616c  r_secret_removal
+0002de80: 2873 6563 7265 742e 6964 2c20 3432 2c20  (secret.id, 42, 
+0002de90: 6c61 6265 6c3d 276f 7665 7272 6964 6527  label='override'
+0002dea0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0002deb0: 6173 7365 7274 4571 7561 6c28 6c65 6e28  assertEqual(len(
+0002dec0: 6861 726e 6573 732e 6368 6172 6d2e 6576  harness.charm.ev
+0002ded0: 656e 7473 292c 2032 290a 2020 2020 2020  ents), 2).      
+0002dee0: 2020 6576 656e 7420 3d20 6861 726e 6573    event = harnes
+0002def0: 732e 6368 6172 6d2e 6576 656e 7473 5b30  s.charm.events[0
+0002df00: 5d0a 2020 2020 2020 2020 7365 6c66 2e61  ].        self.a
+0002df10: 7373 6572 7449 7349 6e73 7461 6e63 6528  ssertIsInstance(
+0002df20: 6576 656e 742c 206f 7073 2e53 6563 7265  event, ops.Secre
+0002df30: 7452 656d 6f76 6545 7665 6e74 290a 2020  tRemoveEvent).  
+0002df40: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0002df50: 7445 7175 616c 2865 7665 6e74 2e73 6563  tEqual(event.sec
+0002df60: 7265 742e 6c61 6265 6c2c 2027 6c62 6c27  ret.label, 'lbl'
+0002df70: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0002df80: 7373 6572 7445 7175 616c 2865 7665 6e74  ssertEqual(event
+0002df90: 2e72 6576 6973 696f 6e2c 2031 290a 2020  .revision, 1).  
+0002dfa0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0002dfb0: 7445 7175 616c 2865 7665 6e74 2e73 6563  tEqual(event.sec
+0002dfc0: 7265 742e 6765 745f 636f 6e74 656e 7428  ret.get_content(
+0002dfd0: 292c 207b 2766 6f6f 273a 2027 7827 7d29  ), {'foo': 'x'})
+0002dfe0: 0a20 2020 2020 2020 2065 7665 6e74 203d  .        event =
+0002dff0: 2068 6172 6e65 7373 2e63 6861 726d 2e65   harness.charm.e
+0002e000: 7665 6e74 735b 315d 0a20 2020 2020 2020  vents[1].       
+0002e010: 2073 656c 662e 6173 7365 7274 4973 496e   self.assertIsIn
+0002e020: 7374 616e 6365 2865 7665 6e74 2c20 6f70  stance(event, op
+0002e030: 732e 5365 6372 6574 5265 6d6f 7665 4576  s.SecretRemoveEv
+0002e040: 656e 7429 0a20 2020 2020 2020 2073 656c  ent).        sel
+0002e050: 662e 6173 7365 7274 4571 7561 6c28 6576  f.assertEqual(ev
+0002e060: 656e 742e 7365 6372 6574 2e6c 6162 656c  ent.secret.label
+0002e070: 2c20 276f 7665 7272 6964 6527 290a 2020  , 'override').  
+0002e080: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0002e090: 7445 7175 616c 2865 7665 6e74 2e72 6576  tEqual(event.rev
+0002e0a0: 6973 696f 6e2c 2034 3229 0a20 2020 2020  ision, 42).     
+0002e0b0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0002e0c0: 7561 6c28 6576 656e 742e 7365 6372 6574  ual(event.secret
+0002e0d0: 2e67 6574 5f63 6f6e 7465 6e74 2829 2c20  .get_content(), 
+0002e0e0: 7b27 666f 6f27 3a20 2778 277d 290a 0a20  {'foo': 'x'}).. 
+0002e0f0: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+0002e100: 2e61 7373 6572 7452 6169 7365 7328 5275  .assertRaises(Ru
+0002e110: 6e74 696d 6545 7272 6f72 293a 0a20 2020  ntimeError):.   
+0002e120: 2020 2020 2020 2020 2068 6172 6e65 7373           harness
+0002e130: 2e74 7269 6767 6572 5f73 6563 7265 745f  .trigger_secret_
+0002e140: 7265 6d6f 7661 6c28 276e 6f73 6563 7265  removal('nosecre
+0002e150: 7427 2c20 3129 0a0a 0a63 6c61 7373 2045  t', 1)...class E
+0002e160: 7665 6e74 5265 636f 7264 6572 286f 7073  ventRecorder(ops
+0002e170: 2e43 6861 726d 4261 7365 293a 0a20 2020  .CharmBase):.   
+0002e180: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+0002e190: 6c66 2c20 6672 616d 6577 6f72 6b29 3a0a  lf, framework):.
+0002e1a0: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+0002e1b0: 5f5f 696e 6974 5f5f 2866 7261 6d65 776f  __init__(framewo
+0002e1c0: 726b 290a 2020 2020 2020 2020 7365 6c66  rk).        self
+0002e1d0: 2e65 7665 6e74 7320 3d20 5b5d 0a0a 2020  .events = []..  
+0002e1e0: 2020 6465 6620 7265 636f 7264 5f65 7665    def record_eve
+0002e1f0: 6e74 2873 656c 662c 2065 7665 6e74 293a  nt(self, event):
+0002e200: 0a20 2020 2020 2020 2073 656c 662e 6576  .        self.ev
+0002e210: 656e 7473 2e61 7070 656e 6428 6576 656e  ents.append(even
+0002e220: 7429 0a0a 0a63 6c61 7373 2054 6573 7450  t)...class TestP
+0002e230: 6f72 7473 2875 6e69 7474 6573 742e 5465  orts(unittest.Te
+0002e240: 7374 4361 7365 293a 0a20 2020 2064 6566  stCase):.    def
+0002e250: 2074 6573 745f 706f 7274 7328 7365 6c66   test_ports(self
+0002e260: 293a 0a20 2020 2020 2020 2068 6172 6e65  ):.        harne
+0002e270: 7373 203d 206f 7073 2e74 6573 7469 6e67  ss = ops.testing
+0002e280: 2e48 6172 6e65 7373 286f 7073 2e43 6861  .Harness(ops.Cha
+0002e290: 726d 4261 7365 2c20 6d65 7461 3d27 6e61  rmBase, meta='na
+0002e2a0: 6d65 3a20 7765 6261 7070 2729 0a20 2020  me: webapp').   
+0002e2b0: 2020 2020 2073 656c 662e 6164 6443 6c65       self.addCle
+0002e2c0: 616e 7570 2868 6172 6e65 7373 2e63 6c65  anup(harness.cle
+0002e2d0: 616e 7570 290a 2020 2020 2020 2020 756e  anup).        un
+0002e2e0: 6974 203d 2068 6172 6e65 7373 2e6d 6f64  it = harness.mod
+0002e2f0: 656c 2e75 6e69 740a 0a20 2020 2020 2020  el.unit..       
+0002e300: 2075 6e69 742e 6f70 656e 5f70 6f72 7428   unit.open_port(
+0002e310: 2774 6370 272c 2038 3038 3029 0a20 2020  'tcp', 8080).   
+0002e320: 2020 2020 2075 6e69 742e 6f70 656e 5f70       unit.open_p
+0002e330: 6f72 7428 2775 6470 272c 2034 3030 3029  ort('udp', 4000)
+0002e340: 0a20 2020 2020 2020 2075 6e69 742e 6f70  .        unit.op
+0002e350: 656e 5f70 6f72 7428 2769 636d 7027 290a  en_port('icmp').
+0002e360: 0a20 2020 2020 2020 2070 6f72 7473 5f73  .        ports_s
+0002e370: 6574 203d 2075 6e69 742e 6f70 656e 6564  et = unit.opened
+0002e380: 5f70 6f72 7473 2829 0a20 2020 2020 2020  _ports().       
+0002e390: 2073 656c 662e 6173 7365 7274 4973 496e   self.assertIsIn
+0002e3a0: 7374 616e 6365 2870 6f72 7473 5f73 6574  stance(ports_set
+0002e3b0: 2c20 7365 7429 0a20 2020 2020 2020 2070  , set).        p
+0002e3c0: 6f72 7473 203d 2073 6f72 7465 6428 706f  orts = sorted(po
+0002e3d0: 7274 735f 7365 742c 206b 6579 3d6c 616d  rts_set, key=lam
+0002e3e0: 6264 6120 703a 2028 702e 7072 6f74 6f63  bda p: (p.protoc
+0002e3f0: 6f6c 2c20 702e 706f 7274 2929 0a20 2020  ol, p.port)).   
+0002e400: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0002e410: 4571 7561 6c28 6c65 6e28 706f 7274 7329  Equal(len(ports)
+0002e420: 2c20 3329 0a20 2020 2020 2020 2073 656c  , 3).        sel
+0002e430: 662e 6173 7365 7274 4973 496e 7374 616e  f.assertIsInstan
+0002e440: 6365 2870 6f72 7473 5b30 5d2c 206f 7073  ce(ports[0], ops
+0002e450: 2e4f 7065 6e65 6450 6f72 7429 0a20 2020  .OpenedPort).   
+0002e460: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0002e470: 4571 7561 6c28 706f 7274 735b 305d 2e70  Equal(ports[0].p
+0002e480: 726f 746f 636f 6c2c 2027 6963 6d70 2729  rotocol, 'icmp')
+0002e490: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0002e4a0: 7365 7274 4973 4e6f 6e65 2870 6f72 7473  sertIsNone(ports
+0002e4b0: 5b30 5d2e 706f 7274 290a 2020 2020 2020  [0].port).      
+0002e4c0: 2020 7365 6c66 2e61 7373 6572 7449 7349    self.assertIsI
+0002e4d0: 6e73 7461 6e63 6528 706f 7274 735b 315d  nstance(ports[1]
+0002e4e0: 2c20 6f70 732e 4f70 656e 6564 506f 7274  , ops.OpenedPort
+0002e4f0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0002e500: 7373 6572 7445 7175 616c 2870 6f72 7473  ssertEqual(ports
+0002e510: 5b31 5d2e 7072 6f74 6f63 6f6c 2c20 2774  [1].protocol, 't
+0002e520: 6370 2729 0a20 2020 2020 2020 2073 656c  cp').        sel
+0002e530: 662e 6173 7365 7274 4571 7561 6c28 706f  f.assertEqual(po
+0002e540: 7274 735b 315d 2e70 6f72 742c 2038 3038  rts[1].port, 808
+0002e550: 3029 0a20 2020 2020 2020 2073 656c 662e  0).        self.
+0002e560: 6173 7365 7274 4973 496e 7374 616e 6365  assertIsInstance
+0002e570: 2870 6f72 7473 5b32 5d2c 206f 7073 2e4f  (ports[2], ops.O
+0002e580: 7065 6e65 6450 6f72 7429 0a20 2020 2020  penedPort).     
+0002e590: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0002e5a0: 7561 6c28 706f 7274 735b 325d 2e70 726f  ual(ports[2].pro
+0002e5b0: 746f 636f 6c2c 2027 7564 7027 290a 2020  tocol, 'udp').  
+0002e5c0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0002e5d0: 7445 7175 616c 2870 6f72 7473 5b32 5d2e  tEqual(ports[2].
+0002e5e0: 706f 7274 2c20 3430 3030 290a 0a20 2020  port, 4000)..   
+0002e5f0: 2020 2020 2075 6e69 742e 636c 6f73 655f       unit.close_
+0002e600: 706f 7274 2827 7463 7027 2c20 3830 3830  port('tcp', 8080
+0002e610: 290a 2020 2020 2020 2020 756e 6974 2e63  ).        unit.c
+0002e620: 6c6f 7365 5f70 6f72 7428 2774 6370 272c  lose_port('tcp',
+0002e630: 2038 3038 3029 2020 2320 636c 6f73 696e   8080)  # closin
+0002e640: 6720 7361 6d65 2070 6f72 7420 6167 6169  g same port agai
+0002e650: 6e20 6861 7320 6e6f 2065 6666 6563 740a  n has no effect.
+0002e660: 2020 2020 2020 2020 756e 6974 2e63 6c6f          unit.clo
+0002e670: 7365 5f70 6f72 7428 2775 6470 272c 2034  se_port('udp', 4
+0002e680: 3030 3029 0a0a 2020 2020 2020 2020 706f  000)..        po
+0002e690: 7274 735f 7365 7420 3d20 756e 6974 2e6f  rts_set = unit.o
+0002e6a0: 7065 6e65 645f 706f 7274 7328 290a 2020  pened_ports().  
+0002e6b0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0002e6c0: 7449 7349 6e73 7461 6e63 6528 706f 7274  tIsInstance(port
+0002e6d0: 735f 7365 742c 2073 6574 290a 2020 2020  s_set, set).    
+0002e6e0: 2020 2020 706f 7274 7320 3d20 736f 7274      ports = sort
+0002e6f0: 6564 2870 6f72 7473 5f73 6574 2c20 6b65  ed(ports_set, ke
+0002e700: 793d 6c61 6d62 6461 2070 3a20 2870 2e70  y=lambda p: (p.p
+0002e710: 726f 746f 636f 6c2c 2070 2e70 6f72 7429  rotocol, p.port)
+0002e720: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0002e730: 7373 6572 7445 7175 616c 286c 656e 2870  ssertEqual(len(p
+0002e740: 6f72 7473 292c 2031 290a 2020 2020 2020  orts), 1).      
+0002e750: 2020 7365 6c66 2e61 7373 6572 7449 7349    self.assertIsI
+0002e760: 6e73 7461 6e63 6528 706f 7274 735b 305d  nstance(ports[0]
+0002e770: 2c20 6f70 732e 4f70 656e 6564 506f 7274  , ops.OpenedPort
+0002e780: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0002e790: 7373 6572 7445 7175 616c 2870 6f72 7473  ssertEqual(ports
+0002e7a0: 5b30 5d2e 7072 6f74 6f63 6f6c 2c20 2769  [0].protocol, 'i
+0002e7b0: 636d 7027 290a 2020 2020 2020 2020 7365  cmp').        se
+0002e7c0: 6c66 2e61 7373 6572 7449 734e 6f6e 6528  lf.assertIsNone(
+0002e7d0: 706f 7274 735b 305d 2e70 6f72 7429 0a0a  ports[0].port)..
+0002e7e0: 2020 2020 2020 2020 756e 6974 2e63 6c6f          unit.clo
+0002e7f0: 7365 5f70 6f72 7428 2769 636d 7027 290a  se_port('icmp').
+0002e800: 0a20 2020 2020 2020 2070 6f72 7473 5f73  .        ports_s
+0002e810: 6574 203d 2075 6e69 742e 6f70 656e 6564  et = unit.opened
+0002e820: 5f70 6f72 7473 2829 0a20 2020 2020 2020  _ports().       
+0002e830: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0002e840: 6c28 706f 7274 735f 7365 742c 2073 6574  l(ports_set, set
+0002e850: 2829 290a 0a20 2020 2064 6566 2074 6573  ())..    def tes
+0002e860: 745f 6572 726f 7273 2873 656c 6629 3a0a  t_errors(self):.
+0002e870: 2020 2020 2020 2020 6861 726e 6573 7320          harness 
+0002e880: 3d20 6f70 732e 7465 7374 696e 672e 4861  = ops.testing.Ha
+0002e890: 726e 6573 7328 6f70 732e 4368 6172 6d42  rness(ops.CharmB
+0002e8a0: 6173 652c 206d 6574 613d 276e 616d 653a  ase, meta='name:
+0002e8b0: 2077 6562 6170 7027 290a 2020 2020 2020   webapp').      
+0002e8c0: 2020 7365 6c66 2e61 6464 436c 6561 6e75    self.addCleanu
+0002e8d0: 7028 6861 726e 6573 732e 636c 6561 6e75  p(harness.cleanu
+0002e8e0: 7029 0a20 2020 2020 2020 2075 6e69 7420  p).        unit 
+0002e8f0: 3d20 6861 726e 6573 732e 6d6f 6465 6c2e  = harness.model.
+0002e900: 756e 6974 0a0a 2020 2020 2020 2020 7769  unit..        wi
+0002e910: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
+0002e920: 6973 6573 286f 7073 2e4d 6f64 656c 4572  ises(ops.ModelEr
+0002e930: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
+0002e940: 2020 756e 6974 2e6f 7065 6e5f 706f 7274    unit.open_port
+0002e950: 2827 6963 6d70 272c 2038 3038 3029 2020  ('icmp', 8080)  
+0002e960: 2320 6963 6d70 2063 616e 6e6f 7420 6861  # icmp cannot ha
+0002e970: 7665 2070 6f72 740a 2020 2020 2020 2020  ve port.        
+0002e980: 7769 7468 2073 656c 662e 6173 7365 7274  with self.assert
+0002e990: 5261 6973 6573 286f 7073 2e4d 6f64 656c  Raises(ops.Model
+0002e9a0: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
+0002e9b0: 2020 2020 756e 6974 2e6f 7065 6e5f 706f      unit.open_po
+0002e9c0: 7274 2827 6674 7027 2c20 3830 3830 2920  rt('ftp', 8080) 
+0002e9d0: 2023 2069 6e76 616c 6964 2070 726f 746f   # invalid proto
+0002e9e0: 636f 6c0a 2020 2020 2020 2020 7769 7468  col.        with
+0002e9f0: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
+0002ea00: 6573 286f 7073 2e4d 6f64 656c 4572 726f  es(ops.ModelErro
+0002ea10: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+0002ea20: 756e 6974 2e6f 7065 6e5f 706f 7274 2827  unit.open_port('
+0002ea30: 7463 7027 2920 2023 2074 6370 206d 7573  tcp')  # tcp mus
+0002ea40: 7420 6861 7665 2070 6f72 740a 2020 2020  t have port.    
+0002ea50: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
+0002ea60: 7365 7274 5261 6973 6573 286f 7073 2e4d  sertRaises(ops.M
+0002ea70: 6f64 656c 4572 726f 7229 3a0a 2020 2020  odelError):.    
+0002ea80: 2020 2020 2020 2020 756e 6974 2e6f 7065          unit.ope
+0002ea90: 6e5f 706f 7274 2827 7564 7027 2920 2023  n_port('udp')  #
+0002eaa0: 2075 6470 206d 7573 7420 6861 7665 2070   udp must have p
+0002eab0: 6f72 740a 2020 2020 2020 2020 7769 7468  ort.        with
+0002eac0: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
+0002ead0: 6573 286f 7073 2e4d 6f64 656c 4572 726f  es(ops.ModelErro
+0002eae0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+0002eaf0: 756e 6974 2e6f 7065 6e5f 706f 7274 2827  unit.open_port('
+0002eb00: 7463 7027 2c20 3029 2020 2320 706f 7274  tcp', 0)  # port
+0002eb10: 206f 7574 206f 6620 7261 6e67 650a 2020   out of range.  
+0002eb20: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+0002eb30: 6173 7365 7274 5261 6973 6573 286f 7073  assertRaises(ops
+0002eb40: 2e4d 6f64 656c 4572 726f 7229 3a0a 2020  .ModelError):.  
+0002eb50: 2020 2020 2020 2020 2020 756e 6974 2e6f            unit.o
+0002eb60: 7065 6e5f 706f 7274 2827 7463 7027 2c20  pen_port('tcp', 
+0002eb70: 3635 3533 3629 2020 2320 706f 7274 206f  65536)  # port o
+0002eb80: 7574 206f 6620 7261 6e67 650a            ut of range.
```

