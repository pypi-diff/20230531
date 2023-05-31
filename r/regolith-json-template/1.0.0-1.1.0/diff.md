# Comparing `tmp/regolith-json-template-1.0.0.tar.gz` & `tmp/regolith-json-template-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regolith-json-template-1.0.0.tar", last modified: Sun Mar 19 19:01:36 2023, max compression
+gzip compressed data, was "regolith-json-template-1.1.0.tar", last modified: Wed May 31 19:31:08 2023, max compression
```

## Comparing `regolith-json-template-1.0.0.tar` & `regolith-json-template-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-19 19:01:36.405323 regolith-json-template-1.0.0/
--rw-rw-rw-   0        0        0     1083 2023-02-24 19:44:45.000000 regolith-json-template-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2150 2023-03-19 19:01:36.406322 regolith-json-template-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      556 2023-03-19 19:01:06.000000 regolith-json-template-1.0.0/README.rst
--rw-rw-rw-   0        0        0       90 2022-09-28 21:38:25.000000 regolith-json-template-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      764 2023-03-19 19:01:36.407323 regolith-json-template-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2022-09-28 23:50:58.000000 regolith-json-template-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-19 19:01:36.388868 regolith-json-template-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-19 19:01:36.397323 regolith-json-template-1.0.0/src/regolith_json_template/
--rw-rw-rw-   0        0        0     5412 2023-03-19 18:42:18.000000 regolith-json-template-1.0.0/src/regolith_json_template/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-19 19:01:36.404323 regolith-json-template-1.0.0/src/regolith_json_template.egg-info/
--rw-rw-rw-   0        0        0     2150 2023-03-19 19:01:36.000000 regolith-json-template-1.0.0/src/regolith_json_template.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-03-19 19:01:36.000000 regolith-json-template-1.0.0/src/regolith_json_template.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-19 19:01:36.000000 regolith-json-template-1.0.0/src/regolith_json_template.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-03-19 19:01:36.000000 regolith-json-template-1.0.0/src/regolith_json_template.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 19:31:08.570666 regolith-json-template-1.1.0/
+-rw-rw-rw-   0        0        0     1083 2023-02-24 19:44:45.000000 regolith-json-template-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2150 2023-05-31 19:31:08.571667 regolith-json-template-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2023-03-19 19:01:06.000000 regolith-json-template-1.1.0/README.rst
+-rw-rw-rw-   0        0        0       90 2022-09-28 21:38:25.000000 regolith-json-template-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      764 2023-05-31 19:31:08.572668 regolith-json-template-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2022-09-28 23:50:58.000000 regolith-json-template-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 19:31:08.554579 regolith-json-template-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 19:31:08.563661 regolith-json-template-1.1.0/src/regolith_json_template/
+-rw-rw-rw-   0        0        0     8118 2023-05-31 19:00:01.000000 regolith-json-template-1.1.0/src/regolith_json_template/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 19:31:08.569667 regolith-json-template-1.1.0/src/regolith_json_template.egg-info/
+-rw-rw-rw-   0        0        0     2150 2023-05-31 19:31:08.000000 regolith-json-template-1.1.0/src/regolith_json_template.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-05-31 19:31:08.000000 regolith-json-template-1.1.0/src/regolith_json_template.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 19:31:08.000000 regolith-json-template-1.1.0/src/regolith_json_template.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-31 19:31:08.000000 regolith-json-template-1.1.0/src/regolith_json_template.egg-info/top_level.txt
```

### Comparing `regolith-json-template-1.0.0/LICENSE` & `regolith-json-template-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `regolith-json-template-1.0.0/PKG-INFO` & `regolith-json-template-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regolith-json-template
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python package for easier reuseability of the JSON Template Regolith filter for Minecraft Bedrock Edition
 Author: Nusiq
 License: MIT
 Project-URL: Source, https://github.com/Nusiq/regolith-json-template/tree/master
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `regolith-json-template-1.0.0/README.rst` & `regolith-json-template-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `regolith-json-template-1.0.0/setup.cfg` & `regolith-json-template-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `regolith-json-template-1.0.0/src/regolith_json_template/__init__.py` & `regolith-json-template-1.1.0/src/regolith_json_template/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,19 @@
-from itertools import chain
 from copy import deepcopy, copy
 import uuid
 import math
-from pathlib import Path
-from typing import Any
-VERSION = (1, 0, 0)
-__version__ = '.'.join([str(x) for x in VERSION])
-
+from typing import Any, NamedTuple
 
-DATA_PATH = Path('data')
-BP_PATH = Path('BP')
-RP_PATH = Path('RP')
+VERSION = (1, 1, 0)
+__version__ = '.'.join([str(x) for x in VERSION])
 
 EVAL_STRING_OPEN = '`'
 EVAL_STRING_CLOSE = '`'
-
-
-def print_red(text):
-    for t in text.split('\n'):
-        print("\033[91m {}\033[00m".format(t))
-
+LIST_UNPACK_KEY = '__unpack__'
+LIST_UNPACK_OPTIONAL_VALUE = '__value__'
 
 class JsonTemplateException(Exception):
     '''Root exception for json_template.'''
     pass
 
 
 class JsonTemplateK:
@@ -35,14 +25,22 @@
     '''
 
     def __init__(self, __key: str, **kwargs):
         self.key: str = __key
         self.scope_extension: dict[str, Any] = kwargs
 
 
+class _Unpack(NamedTuple):
+    '''
+    _Unpack is an object that is used internally by the eval_json function to
+    pass lists to be unpacked up from an item of the list, to the list itself.
+    The value of the _Unpack object is a list of values to unpack.
+    '''
+    data: list[Any]
+
 def is_eval_string(text: str) -> tuple[bool, str]:
     '''
     Checks if text is a string to be evaluated and returns the result and the
     substring to be evaluated. An eval string is a string that starts with
     EVAL_STRING_OPEN and ends with EVAL_STRING_CLOSE (global variables).
 
     If it's not an eval string, returns False and the original text.
@@ -50,50 +48,103 @@
     if len(text) <= len(EVAL_STRING_OPEN) + len(EVAL_STRING_CLOSE):
         return False, text  # Too short to be an eval string
     if text.startswith(EVAL_STRING_OPEN) and text.endswith(EVAL_STRING_CLOSE):
         return True, text[len(EVAL_STRING_OPEN):-len(EVAL_STRING_CLOSE)]
     return False, text
 
 
-def eval_json(data, scope: dict[str, Any]):
+def eval_json(data, scope: dict[str, Any], _is_list_item: bool = False):
     '''
     Walks JSON file (data) yields json paths. The behavior of the function is
     undefined if the data contains objects that can't be represended as JSON
     using json.dumps (e.g. sets, functions, etc.).
+
+    :param data: JSON data to be evaluated.
+    :param scope: A dictionary that will be used as a scope for evaluating
+        the template.
+    :param _is_list_item: An internally used flag that indicates if the data
+        is a list item. List items can be unpacked into multiple items in
+        some cases.
     '''
     if isinstance(data, dict):
-        keys = list(data.keys())
-        for k in keys:
-            is_eval_key, key = is_eval_string(k)
+        keys: list[tuple[str, None | list[str | JsonTemplateK]]] = []
+        is_unpacked = False
+        for k in data.keys():
+            if k == LIST_UNPACK_KEY and _is_list_item:
+                is_unpacked = True
+                continue
+            is_eval_key, stripped_key = is_eval_string(k)
             if is_eval_key:
-                evaluated_keys = eval_key(key, scope)
-                old_data_k_value = data[k]
-                del data[k]
-                last_item_index = len(evaluated_keys) - 1
-                for i, evaluated_key in enumerate(evaluated_keys):
-                    child_scope = scope  # No need for deepcopy
-                    if isinstance(evaluated_key, JsonTemplateK):
-                        child_scope = scope | evaluated_key.scope_extension
-                        evaluated_key = evaluated_key.key
-                    # Don't copy the last item, simply use the old value. Note
-                    # that it must be the last item not for example the first
-                    # one, because the next item always is based on the
-                    # old_data_k_value so it can't be evaluated when it needs
-                    # to be a source for other items.
-                    if i == last_item_index:
-                        data[evaluated_key] = old_data_k_value
-                    else:  # copy the rest
-                        data[evaluated_key] = deepcopy(old_data_k_value)
-                    data[evaluated_key] = eval_json(
-                        data[evaluated_key], child_scope)
+                keys.append((k, eval_key(stripped_key, scope)))
             else:
-                data[k] = eval_json(data[k], scope)
+                keys.append((k, None))
+
+        if is_unpacked:
+            scopes: list[dict[str, Any]]
+            if isinstance(data[LIST_UNPACK_KEY], list):
+                scopes = data[LIST_UNPACK_KEY]
+            elif isinstance(data[LIST_UNPACK_KEY], str):
+                is_unpak_eval_val, unpack_eval_val = is_eval_string(
+                    data[LIST_UNPACK_KEY])
+                if not is_unpak_eval_val:
+                    raise JsonTemplateException(
+                        f"The value of {LIST_UNPACK_KEY} must be a list or "
+                        "an eval string.")
+                scopes = eval_value(unpack_eval_val, scope)
+            del data[LIST_UNPACK_KEY]
+            if LIST_UNPACK_OPTIONAL_VALUE in data:
+                if len(data) > 1:
+                    raise JsonTemplateException(
+                        f"{LIST_UNPACK_OPTIONAL_VALUE} can't be used with "
+                        "other keys.")
+                data_template = data[LIST_UNPACK_OPTIONAL_VALUE]
+                del data[LIST_UNPACK_OPTIONAL_VALUE]
+            else:
+                data_template = data
+            data = _Unpack([])
+            for i, scope in enumerate(scopes): 
+                if i == len(scopes) - 1:
+                    # No need to copy the last item, we can simply use the
+                    # original data_template (we don't need it anymore).
+                    data.data.append(eval_json(data_template, scope))
+                else:
+                    data.data.append(eval_json(deepcopy(data_template), scope))
+        else:
+            for k, evaluated_keys in keys:
+                if isinstance(evaluated_keys, list):
+                    old_data_k_value = data[k]
+                    del data[k]
+                    last_item_index = len(evaluated_keys) - 1
+                    for i, evaluated_key in enumerate(evaluated_keys):
+                        child_scope = scope  # No need for deepcopy
+                        if isinstance(evaluated_key, JsonTemplateK):
+                            child_scope = scope | evaluated_key.scope_extension
+                            evaluated_key = evaluated_key.key
+                        # Don't copy the last item, simply use the old value. Note
+                        # that it must be the last item not for example the first
+                        # one, because the next item always is based on the
+                        # old_data_k_value so it can't be evaluated when it needs
+                        # to be a source for other items.
+                        if i == last_item_index:
+                            data[evaluated_key] = old_data_k_value
+                        else:  # copy the rest
+                            data[evaluated_key] = deepcopy(old_data_k_value)
+                        data[evaluated_key] = eval_json(
+                            data[evaluated_key], child_scope)
+                else:
+                    data[k] = eval_json(data[k], scope)
     elif isinstance(data, list):
-        for i in range(len(data)):
-            data[i] = eval_json(data[i], scope)
+        new_data = []
+        for item in data:
+            eval_item = eval_json(item, scope, True)
+            if isinstance(eval_item, _Unpack):
+                new_data.extend(eval_item.data)
+            else:
+                new_data.append(eval_item)
+        data = new_data
     elif isinstance(data, str):
         is_eval_val, data = is_eval_string(data)
         if is_eval_val:
             return eval_value(data, scope)
         return data
     return data
```

### Comparing `regolith-json-template-1.0.0/src/regolith_json_template.egg-info/PKG-INFO` & `regolith-json-template-1.1.0/src/regolith_json_template.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regolith-json-template
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python package for easier reuseability of the JSON Template Regolith filter for Minecraft Bedrock Edition
 Author: Nusiq
 License: MIT
 Project-URL: Source, https://github.com/Nusiq/regolith-json-template/tree/master
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

