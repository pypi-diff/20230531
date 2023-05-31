# Comparing `tmp/kevbits-0.4.0.tar.gz` & `tmp/kevbits-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kevbits-0.4.0.tar", max compression
+gzip compressed data, was "kevbits-0.5.0.tar", max compression
```

## Comparing `kevbits-0.4.0.tar` & `kevbits-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0        0 2022-07-06 08:47:46.812112 kevbits-0.4.0/kevbits/__init__.py
--rw-r--r--   0        0        0     2331 2022-07-06 08:47:46.595113 kevbits-0.4.0/kevbits/logconfig.py
--rw-r--r--   0        0        0      580 2022-07-06 08:47:46.614113 kevbits-0.4.0/kevbits/math.py
--rw-r--r--   0        0        0     1989 2022-07-06 08:47:46.639118 kevbits-0.4.0/kevbits/misc.py
--rw-r--r--   0        0        0      444 2022-07-06 08:47:46.673111 kevbits-0.4.0/kevbits/tests/math_test.py
--rw-r--r--   0        0        0     1928 2023-03-12 07:03:00.814455 kevbits-0.4.0/kevbits/tests/misc_test.py
--rw-r--r--   0        0        0      409 2023-03-12 07:01:29.082816 kevbits-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-12 07:05:22.955665 kevbits-0.4.0/README.md
--rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 kevbits-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-07-06 08:47:46.812112 kevbits-0.5.0/kevbits/__init__.py
+-rw-r--r--   0        0        0     2465 2023-03-12 08:27:49.741866 kevbits-0.5.0/kevbits/logconfig.py
+-rw-r--r--   0        0        0      631 2023-03-12 08:27:49.627869 kevbits-0.5.0/kevbits/math.py
+-rw-r--r--   0        0        0     2250 2023-03-12 08:27:49.744867 kevbits-0.5.0/kevbits/misc.py
+-rw-r--r--   0        0        0     5875 2023-05-31 09:41:12.200066 kevbits-0.5.0/kevbits/sgconv.py
+-rw-r--r--   0        0        0      916 2023-05-31 09:46:25.231068 kevbits-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-03-12 07:21:14.714981 kevbits-0.5.0/README.md
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 kevbits-0.5.0/PKG-INFO
```

### Comparing `kevbits-0.4.0/kevbits/logconfig.py` & `kevbits-0.5.0/kevbits/logconfig.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,58 +11,72 @@
 import logging
 import logging.config
 
 import sys
 import time
 import re
 import os
+from typing import Any
 
-from .misc import map_dict_deep
+from kevbits.misc import map_dict_deep
 
 
 class GmTimeFormatter(logging.Formatter):
     "Use UTC timestamp for log messages."
+
     def __init__(self, fmt=None, datefmt=None):
-        super(GmTimeFormatter, self).__init__(fmt=fmt, datefmt=datefmt)
+        super().__init__(fmt=fmt, datefmt=datefmt)
         self.converter = time.gmtime
 
 
 def gmtime_formatter_factory(fmt, datefmt):
     "Factory function which is referred to from .yaml file."
     return GmTimeFormatter(fmt, datefmt)
 
 
-rx_expandvars = re.compile(r'(.*?)(\${.*?})(.*)')
+rx_expandvars = re.compile(r"(.*?)(\${.*?})(.*)")
+
 
-def expandvars(s):
+def expandvars(string: str) -> str:
     "Expand env. variables when they are given in the form ${name} only."
-    m = rx_expandvars.match(s)
+    m = rx_expandvars.match(string)
     if m is None:
-        return s
+        return string
     left, curr, right = m.groups()
-    value = os.environ.get(curr[2:-1], curr)  # left the text unchanged if no such variable
+    value = os.environ.get(
+        curr[2:-1], curr
+    )  # left the text unchanged if no such variable
     return left + value + expandvars(right)
 
 
-def from_dict(config):
+def from_dict(config: dict[str, Any]):
     "Configure logging from dict."
     # Configure logging. We don't use logfiles when running under pytest (pytest.watch)
     # as this may interfer with normal application execution taking place at the same
     # moment. (On every testing iteration pytest imports this application module.
     # Without logfiles disabling this import will lead to logging reinitialization
     # and possible logfiles changes.
-    if hasattr(sys, '_called_from_test'):
+    if hasattr(sys, "_called_from_test"):
         logging.basicConfig()
     else:
         # expand environment variables
-        config = map_dict_deep(config, lambda v: v if not isinstance(v, str) else expandvars(v))
+        config = map_dict_deep(
+            config, lambda v: v if not isinstance(v, str) else expandvars(v)
+        )
         logging.config.dictConfig(config)
 
-    logging.captureWarnings(True)  # Capture warnings issued by the built-in 'warnings' module
+    logging.captureWarnings(
+        True
+    )  # Capture warnings issued by the built-in 'warnings' module
 
     # Add standard level aliases (based on forte/log/main.py)
-    for l, a in [(logging.DEBUG, 'D'), (logging.INFO, '.'),
-                 (logging.WARNING, 'w'), (logging.ERROR, 'E'), (logging.CRITICAL, '!')]:
+    for l, a in [
+        (logging.DEBUG, "D"),
+        (logging.INFO, "."),
+        (logging.WARNING, "w"),
+        (logging.ERROR, "E"),
+        (logging.CRITICAL, "!"),
+    ]:
         logging.addLevelName(l, a)
 
     # Return logger so that the user of this module does not need to import the 'logging' module.
     return logging.getLogger()
```

### Comparing `kevbits-0.4.0/kevbits/math.py` & `kevbits-0.5.0/kevbits/math.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
 Degree = pi / 180
 Hour = pi / 12
 ArcMin = Degree / 60
 ArcSec = ArcMin / 60
 
 
-def closest_mod(x, target, modulo):
+def closest_mod(x: float, target: float, modulo: float):
     """
     Add or subtract modulo to x (possible several times) to achieve
     minimal distance from the target.
     """
     assert modulo > 0.0
     return x + round((target - x) / modulo) * modulo
 
 
-def closest_mod_pi(x, target):
+def closest_mod_pi(x: float, target: float):
     "See closest_mod() function."
     return closest_mod(x, target, pi)
 
 
-def closest_mod_2pi(x, target):
+def closest_mod_2pi(x: float, target: float):
     "See closest_mod() function."
-    return closest_mod(x, target, 2*pi)
+    return closest_mod(x, target, 2 * pi)
```

### Comparing `kevbits-0.4.0/kevbits/misc.py` & `kevbits-0.5.0/kevbits/misc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,85 @@
 """
 Miscellaneous functions
 """
 
 import sys
 import traceback
+from typing import Any, Callable
 
 
-def boolstr_to_bool(s):
+def boolstr_to_bool(string: str):
     """
     Cast string that describes bool values ("False", "yes", "1", "0")
     into bool type.
     """
-    t = s.lower().replace('false', '0').replace('true', '1').\
-        replace('no', '0').replace('yes', '1')
+    t = (
+        string.lower()
+        .replace("false", "0")
+        .replace("true", "1")
+        .replace("no", "0")
+        .replace("yes", "1")
+    )
     return bool(int(t))
 
 
-def map_dict_deep(d, mapfunc):
+def map_dict_deep(
+    dict_: dict[Any, Any], mapfunc: Callable[[Any], Any]
+) -> dict[Any, Any]:
     """
     Return a new dictionary whose keys are not changed, and the values (if they are not
     dictionaries) are passed through the map function. If the value is a (nested) dictionary,
     it undergoes the same processing.
 
     Args:
-        d (dict): dictionary to process,
+        dict_ (dict): dictionary to process,
         mapfunc (function): map function of type (value) -> (value).
     """
-    result = {}
-    for k, v in d.items():
+    result: dict[Any, Any] = {}
+    for k, v in dict_.items():
         if not isinstance(v, dict):
             v = mapfunc(v)
         else:
             v = map_dict_deep(v, mapfunc)
         result[k] = v
     return result
 
 
-def map_deep(e, mapfunc, *, map_dict=True, map_list=True):
+def map_deep(
+    elem: Any,
+    mapfunc: Callable[[Any], Any],
+    *,
+    map_dict: bool = True,
+    map_list: bool = True,
+) -> Any:
     """
     Same as map_dict_deep but also map the elements of lists.
 
     Args:
-        e: element to process,
+        elem: element to process,
         mapfunc (function): map function of type (value) -> (value).
     """
-    opts = (lambda **kw: kw)(map_dict=map_dict, map_list=map_list)
-    if isinstance(e, dict) and map_dict:
-        result = {k: map_deep(v, mapfunc, **opts) for k, v in e.items()}
-    elif isinstance(e, list) and map_list:
-        result = [map_deep(v, mapfunc, **opts) for v in e]
+    opts = {"map_dict": map_dict, "map_list": map_list}
+    if isinstance(elem, dict) and map_dict:
+        result = {k: map_deep(v, mapfunc, **opts) for k, v in elem.items()}
+    elif isinstance(elem, list) and map_list:
+        result = [map_deep(v, mapfunc, **opts) for v in elem]
     else:
-        result = mapfunc(e)
+        result = mapfunc(elem)
     return result
 
 
-def format_exception(tb=False):
+def format_exception(tb: bool = False):
     """
     Formats exception message using sys.exc_info.
     Replaces newlines with spaces (only if tb==False)
 
     Args:
         tb (bool, optional): If True, prints traceback information. Defaults to False.
     """
     if tb:
         text = traceback.format_exc()
     else:
         exc_type, exc_value = sys.exc_info()[:2]
-        text = '{}: {}'.format(exc_type.__name__, str(exc_value))
-        text = text.replace('\n', ' ')
+        text = f"{exc_type.__name__}: {str(exc_value)}"
+        text = text.replace("\n", " ")
     return text
```

