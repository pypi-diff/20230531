# Comparing `tmp/pytest_when-1.0.7.tar.gz` & `tmp/pytest_when-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_when-1.0.7.tar", last modified: Wed May 31 20:51:48 2023, max compression
+gzip compressed data, was "pytest_when-1.0.8.tar", last modified: Wed May 31 21:33:22 2023, max compression
```

## Comparing `pytest_when-1.0.7.tar` & `pytest_when-1.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11342 2023-05-31 20:51:11.910555 pytest_when-1.0.7/LICENSE
--rw-r--r--   0        0        0     2866 2023-05-31 20:51:11.910555 pytest_when-1.0.7/README.md
--rw-r--r--   0        0        0     2766 2023-05-31 20:51:48.095359 pytest_when-1.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-31 20:51:11.910555 pytest_when-1.0.7/pytest_when/__init__.py
--rw-r--r--   0        0        0       45 2023-05-31 20:51:11.910555 pytest_when-1.0.7/pytest_when/plugin.py
--rw-r--r--   0        0        0        0 2023-05-31 20:51:11.910555 pytest_when-1.0.7/pytest_when/py.typed
--rw-r--r--   0        0        0    10573 2023-05-31 20:51:11.910555 pytest_when-1.0.7/pytest_when/when.py
--rw-r--r--   0        0        0        0 2023-05-31 20:51:11.910555 pytest_when-1.0.7/tests/resources/__init__.py
--rw-r--r--   0        0        0      232 2023-05-31 20:51:11.910555 pytest_when-1.0.7/tests/resources/example_module.py
--rw-r--r--   0        0        0     3435 2023-05-31 20:51:11.910555 pytest_when-1.0.7/tests/test_create_call_key.py
--rw-r--r--   0        0        0     6280 2023-05-31 20:51:11.910555 pytest_when-1.0.7/tests/test_integration.py
--rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 pytest_when-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-05-31 21:32:46.853017 pytest_when-1.0.8/LICENSE
+-rw-r--r--   0        0        0     2866 2023-05-31 21:32:46.853017 pytest_when-1.0.8/README.md
+-rw-r--r--   0        0        0     2766 2023-05-31 21:33:22.885145 pytest_when-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-31 21:32:46.853017 pytest_when-1.0.8/pytest_when/__init__.py
+-rw-r--r--   0        0        0       45 2023-05-31 21:32:46.853017 pytest_when-1.0.8/pytest_when/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-31 21:32:46.853017 pytest_when-1.0.8/pytest_when/py.typed
+-rw-r--r--   0        0        0    10675 2023-05-31 21:32:46.853017 pytest_when-1.0.8/pytest_when/when.py
+-rw-r--r--   0        0        0        0 2023-05-31 21:32:46.853017 pytest_when-1.0.8/tests/resources/__init__.py
+-rw-r--r--   0        0        0      232 2023-05-31 21:32:46.853017 pytest_when-1.0.8/tests/resources/example_module.py
+-rw-r--r--   0        0        0     3635 2023-05-31 21:32:46.853017 pytest_when-1.0.8/tests/test_create_call_key.py
+-rw-r--r--   0        0        0     6280 2023-05-31 21:32:46.853017 pytest_when-1.0.8/tests/test_integration.py
+-rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 pytest_when-1.0.8/PKG-INFO
```

### Comparing `pytest_when-1.0.7/LICENSE` & `pytest_when-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.7/README.md` & `pytest_when-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.7/pyproject.toml` & `pytest_when-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 [tool.coverage.paths]
 source = [
     "./pytest_when",
 ]
 
 [tool.coverage.report]
-fail_under = 53
+fail_under = 51
 skip_covered = true
 show_missing = true
 
 [tool.coverage.html]
 directory = "coverage_html"
 
 [tool.pytest.ini_options]
@@ -153,15 +153,15 @@
 dependencies = [
     "pytest>=7.3.1",
     "pytest-mock>=3.10.0",
     "typing-extensions>=4.5.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "1.0.7"
+version = "1.0.8"
 
 [project.entry-points.pytest11]
 pytest-when = "pytest_when.plugin"
 
 [project.urls]
 repository = "https://github.com/zhukovgreen/pytest-when"
```

### Comparing `pytest_when-1.0.7/pytest_when/when.py` & `pytest_when-1.0.8/pytest_when/when.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,27 +32,28 @@
 
     Markers.any - means the argument could be anything
     """
 
     any: str = "any"  # noqa: ignore A003
 
 
-def tupleize(
+def make_hashable(
     container: Tuple[Tuple[str, Any], ...]
 ) -> Tuple[Tuple[str, Any], ...]:
-    def unwrap(value):
-        if isinstance(value, str):
-            return value
+    def unwrap_mapping(value):
         if isinstance(value, Mapping):
-            return tuple((k, unwrap(v)) for k, v in value.items())
-        if isinstance(value, Iterable):
-            return tuple(unwrap(v) for v in value)
+            return tuple((k, unwrap_mapping(v)) for k, v in value.items())
+        if isinstance(value, (list, set)):
+            return tuple(unwrap_mapping(v) for v in value)
+        assert hash(
+            value
+        ), f"Not hashable function arg {value!r} is not supported currently."
         return value
 
-    return tuple((arg, unwrap(value)) for arg, value in container)
+    return tuple((arg, unwrap_mapping(value)) for arg, value in container)
 
 
 def create_call_key(
     original_callable_sig: inspect.Signature,
     *args: _TargetMethodArgs,
     **kwargs: _TargetMethodKwargs,
 ) -> _CallKey:
@@ -62,15 +63,15 @@
     of kwargs is not important and will be allocated based on order
     of the kwargs in the function signature.
 
     Supports normal functions as well as class methods.
     """
     call = original_callable_sig.bind(*args, **kwargs)
 
-    return tupleize(tuple(call.arguments.items()))
+    return make_hashable(tuple(call.arguments.items()))
 
 
 def get_mocked_call_result(
     original_callable_sig: inspect.Signature,
     mocked_calls: Dict[
         _CallKey,
         _TargetMethodReturn,
```

### Comparing `pytest_when-1.0.7/tests/test_create_call_key.py` & `pytest_when-1.0.8/tests/test_create_call_key.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,23 @@
             inspect.signature(foo),
             Markers.any,
             2,
             c_kw=3,
             d_kw=4,
         )
     ] = 1
+    {}[
+        create_call_key(
+            inspect.signature(foo),
+            {"some_inner": "container"},
+            ("some", "list"),
+            c_kw=3,
+            d_kw=4,
+        )
+    ] = 2
 
 
 def test_should_work_for_class_methods_as_well():
     class Some:
         def call(self, a_arg, b_arg, *, c_kw, d_kw):
             ...
```

### Comparing `pytest_when-1.0.7/tests/test_integration.py` & `pytest_when-1.0.8/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.7/PKG-INFO` & `pytest_when-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-when
-Version: 1.0.7
+Version: 1.0.8
 Summary: Utility which makes mocking more readable and controllable
 Author-Email: zhukovgreen <iam+pytest-when@zhukovgreen.pro>
 Project-URL: Repository, https://github.com/zhukovgreen/pytest-when
 Requires-Python: >=3.8
 Requires-Dist: pytest>=7.3.1
 Requires-Dist: pytest-mock>=3.10.0
 Requires-Dist: typing-extensions>=4.5.0
```

