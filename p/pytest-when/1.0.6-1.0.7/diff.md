# Comparing `tmp/pytest_when-1.0.6.tar.gz` & `tmp/pytest_when-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_when-1.0.6.tar", last modified: Mon May 22 12:49:34 2023, max compression
+gzip compressed data, was "pytest_when-1.0.7.tar", last modified: Wed May 31 20:51:48 2023, max compression
```

## Comparing `pytest_when-1.0.6.tar` & `pytest_when-1.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11342 2023-05-22 12:48:58.509722 pytest_when-1.0.6/LICENSE
--rw-r--r--   0        0        0     2709 2023-05-22 12:48:58.509722 pytest_when-1.0.6/README.md
--rw-r--r--   0        0        0     2766 2023-05-22 12:49:34.722300 pytest_when-1.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-22 12:48:58.509722 pytest_when-1.0.6/pytest_when/__init__.py
--rw-r--r--   0        0        0       45 2023-05-22 12:48:58.509722 pytest_when-1.0.6/pytest_when/plugin.py
--rw-r--r--   0        0        0        0 2023-05-22 12:48:58.509722 pytest_when-1.0.6/pytest_when/py.typed
--rw-r--r--   0        0        0    10667 2023-05-22 12:48:58.509722 pytest_when-1.0.6/pytest_when/when.py
--rw-r--r--   0        0        0        0 2023-05-22 12:48:58.509722 pytest_when-1.0.6/tests/resources/__init__.py
--rw-r--r--   0        0        0      131 2023-05-22 12:48:58.509722 pytest_when-1.0.6/tests/resources/example_module.py
--rw-r--r--   0        0        0     2492 2023-05-22 12:48:58.509722 pytest_when-1.0.6/tests/test_create_call_key.py
--rw-r--r--   0        0        0     5848 2023-05-22 12:48:58.509722 pytest_when-1.0.6/tests/test_integration.py
--rw-r--r--   0        0        0     3128 1970-01-01 00:00:00.000000 pytest_when-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-05-31 20:51:11.910555 pytest_when-1.0.7/LICENSE
+-rw-r--r--   0        0        0     2866 2023-05-31 20:51:11.910555 pytest_when-1.0.7/README.md
+-rw-r--r--   0        0        0     2766 2023-05-31 20:51:48.095359 pytest_when-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-31 20:51:11.910555 pytest_when-1.0.7/pytest_when/__init__.py
+-rw-r--r--   0        0        0       45 2023-05-31 20:51:11.910555 pytest_when-1.0.7/pytest_when/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-31 20:51:11.910555 pytest_when-1.0.7/pytest_when/py.typed
+-rw-r--r--   0        0        0    10573 2023-05-31 20:51:11.910555 pytest_when-1.0.7/pytest_when/when.py
+-rw-r--r--   0        0        0        0 2023-05-31 20:51:11.910555 pytest_when-1.0.7/tests/resources/__init__.py
+-rw-r--r--   0        0        0      232 2023-05-31 20:51:11.910555 pytest_when-1.0.7/tests/resources/example_module.py
+-rw-r--r--   0        0        0     3435 2023-05-31 20:51:11.910555 pytest_when-1.0.7/tests/test_create_call_key.py
+-rw-r--r--   0        0        0     6280 2023-05-31 20:51:11.910555 pytest_when-1.0.7/tests/test_integration.py
+-rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 pytest_when-1.0.7/PKG-INFO
```

### Comparing `pytest_when-1.0.6/LICENSE` & `pytest_when-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_when-1.0.6/README.md` & `pytest_when-1.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 
 It is readable and gives you a way to enable the mock only for a specific
 argument's values. In this the attribute will be mocked, for specific
 first two arguments and any third argument.
 
 Inspired by <https://github.com/mockito/mockito-scala>
 
+`.called_with` method arguments are compared with the
+real callable signature and gives additional protection against
+changing the real callable interface.
+
 ## Installation
 
 ```bash
 pip install pytest-when
 ```
```

### Comparing `pytest_when-1.0.6/pyproject.toml` & `pytest_when-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 dependencies = [
     "pytest>=7.3.1",
     "pytest-mock>=3.10.0",
     "typing-extensions>=4.5.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "1.0.6"
+version = "1.0.7"
 
 [project.entry-points.pytest11]
 pytest-when = "pytest_when.plugin"
 
 [project.urls]
 repository = "https://github.com/zhukovgreen/pytest-when"
```

### Comparing `pytest_when-1.0.6/pytest_when/when.py` & `pytest_when-1.0.7/pytest_when/when.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import enum
 import inspect
 
+from collections.abc import Iterable, Mapping
 from typing import Any, Callable, Dict, Generic, Protocol, Tuple, TypeVar
 from unittest.mock import MagicMock
 
 import pytest
 
 from pytest_mock import MockerFixture
 from typing_extensions import ParamSpec
@@ -31,47 +32,45 @@
 
     Markers.any - means the argument could be anything
     """
 
     any: str = "any"  # noqa: ignore A003
 
 
+def tupleize(
+    container: Tuple[Tuple[str, Any], ...]
+) -> Tuple[Tuple[str, Any], ...]:
+    def unwrap(value):
+        if isinstance(value, str):
+            return value
+        if isinstance(value, Mapping):
+            return tuple((k, unwrap(v)) for k, v in value.items())
+        if isinstance(value, Iterable):
+            return tuple(unwrap(v) for v in value)
+        return value
+
+    return tuple((arg, unwrap(value)) for arg, value in container)
+
+
 def create_call_key(
     original_callable_sig: inspect.Signature,
     *args: _TargetMethodArgs,
     **kwargs: _TargetMethodKwargs,
 ) -> _CallKey:
     """Create a call identification key for the given function.
 
     This key represents a certain call to the function. The order
     of kwargs is not important and will be allocated based on order
     of the kwargs in the function signature.
 
     Supports normal functions as well as class methods.
     """
-    original_params = original_callable_sig.parameters
-    args_key: _CallKey = tuple(
-        zip(tuple(original_params)[: len(args)], args),
-    )
+    call = original_callable_sig.bind(*args, **kwargs)
 
-    def get_from_kwargs_or_default(k: str) -> Any:
-        maybe_result = kwargs.get(k, original_params[k].default)
-        if maybe_result is inspect.Parameter.empty:  # type: ignore
-            raise ValueError(
-                f"Not specified parameter {k}. "
-                f"Incompatible call specification args={args}, kwargs={kwargs}"
-                f" to the function with signature {original_callable_sig}"
-            )
-        return maybe_result
-
-    kwargs_key: _CallKey = tuple(
-        (k, get_from_kwargs_or_default(k))
-        for k in tuple(original_params)[len(args) :]
-    )
-    return args_key + kwargs_key
+    return tupleize(tuple(call.arguments.items()))
 
 
 def get_mocked_call_result(
     original_callable_sig: inspect.Signature,
     mocked_calls: Dict[
         _CallKey,
         _TargetMethodReturn,
@@ -166,16 +165,18 @@
             cls,
             method,
             autospec=True,
             # it is important to send the origin target to the
             # side_effect_factory in order the result side_effect stores
             # the original target.
             side_effect=side_effect_factory(
-                getattr(cls, method),
-                self.mocked_calls_registry[(cls.__name__, method)],
+                origin_callable=getattr(cls, method),
+                mocked_calls=self.mocked_calls_registry[
+                    (cls.__name__, method)
+                ],
             ),
         )
 
 
 class When(
     Generic[
         _TargetClsType,
@@ -253,21 +254,21 @@
         ](self.mocker)
 
     def __call__(
         self,
         cls: _TargetClsType,
         method: str,
     ) -> "When":
-        def match_current_obj(patch_and_function) -> bool:
+        def matched_current_obj(patch_and_function) -> bool:
             patch, _ = patch_and_function
             return patch.target is cls and patch.attribute == method
 
         # if current object was already patched, we have to re-patch it again
         for mocked_obj, func in filter(
-            match_current_obj,
+            matched_current_obj,
             self.mocker._patches_and_mocks,  # noqa: ignore SLF001
         ):
             mocked_obj.stop()
             self.mocker._patches_and_mocks.remove(  # noqa: ignore SLF001
                 (mocked_obj, func)
             )
```

### Comparing `pytest_when-1.0.6/tests/test_create_call_key.py` & `pytest_when-1.0.7/tests/test_create_call_key.py`

 * *Files 14% similar despite different names*

```diff
@@ -57,16 +57,16 @@
         ("c_kw", 3),
         ("d_kw", 4),
     )
 
 
 def test_should_raise_exception_on_incompatible_calls():
     with pytest.raises(
-        Exception,
-        match="Incompatible call",
+        TypeError,
+        match="missing a required argument: 'd_kw'",
     ):
         create_call_key(
             inspect.signature(foo),
             Markers.any,
             2,
             c_kw=3,
         )
@@ -98,20 +98,71 @@
     ):
         ...
 
     actual = create_call_key(
         inspect.signature(call_with_defaults),
         "a_arg not default",
     )
-    assert actual == (
-        ("a_arg", "a_arg not default"),
-        ("b_arg", "b_arg default"),
-        ("c_kw", "c_kw default"),
-        ("d_kw", "d_kw default"),
-    )
+    assert actual == (("a_arg", "a_arg not default"),)
 
     # check if parameter was not specified
-    with pytest.raises(ValueError, match="Not specified parameter a_arg"):
+    with pytest.raises(
+        TypeError,
+        match="missing a required argument: 'a_arg'",
+    ):
         create_call_key(
             inspect.signature(call_with_defaults),
             b_arg="b_arg not default",
         )
+
+
+def test_should_work_with_variadic_args_and_kwargs():
+    def foo_with_variadic_args_kwargs(*args, **kwargs) -> str:
+        ...
+
+    actual = create_call_key(
+        inspect.signature(foo_with_variadic_args_kwargs),
+        1,
+        2,
+        a=3,
+        b=4,
+        c=Markers.any,
+    )
+    assert actual == (
+        ("args", (1, 2)),
+        (
+            "kwargs",
+            (
+                ("a", 3),
+                ("b", 4),
+                ("c", Markers.any),
+            ),
+        ),
+    )
+
+    def foo_with_variadic_kwargs(
+        just_a_arg,
+        *just_var_arg,
+        just_b_kwarg=1,
+        **kwargs,
+    ):
+        ...
+
+    actual = create_call_key(
+        inspect.signature(foo_with_variadic_kwargs),
+        1,
+        2,
+        3,
+        c=4,
+        d=5,
+    )
+    assert actual == (
+        ("just_a_arg", 1),
+        ("just_var_arg", (2, 3)),
+        (
+            "kwargs",
+            (
+                ("c", 4),
+                ("d", 5),
+            ),
+        ),
+    )
```

### Comparing `pytest_when-1.0.6/tests/test_integration.py` & `pytest_when-1.0.7/tests/test_integration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import pytest
-
 from tests.resources import example_module
 
 
 class Klass1:
     def some_method(
         self,
         arg1: str,
@@ -282,7 +280,23 @@
             1,
             kwarg1="b",
             kwarg2="c",
         )
         == "Not mocked"
     )
     patched_klass.assert_called()
+
+
+def test_should_work_with_variadic_args_kwargs(when):
+    patched_foo = (
+        when(example_module, "some_foo_with_variadic_args_kwargs")
+        .called_with(1, a=2)
+        .then_return("Mocked")
+    )
+    assert (
+        example_module.some_foo_with_variadic_args_kwargs(1, a=2) == "Mocked"
+    )
+    assert (
+        example_module.some_foo_with_variadic_args_kwargs(1, a=3)
+        == "Not mocked"
+    )
+    patched_foo.assert_called()
```

### Comparing `pytest_when-1.0.6/PKG-INFO` & `pytest_when-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-when
-Version: 1.0.6
+Version: 1.0.7
 Summary: Utility which makes mocking more readable and controllable
 Author-Email: zhukovgreen <iam+pytest-when@zhukovgreen.pro>
 Project-URL: Repository, https://github.com/zhukovgreen/pytest-when
 Requires-Python: >=3.8
 Requires-Dist: pytest>=7.3.1
 Requires-Dist: pytest-mock>=3.10.0
 Requires-Dist: typing-extensions>=4.5.0
@@ -25,14 +25,18 @@
 
 It is readable and gives you a way to enable the mock only for a specific
 argument's values. In this the attribute will be mocked, for specific
 first two arguments and any third argument.
 
 Inspired by <https://github.com/mockito/mockito-scala>
 
+`.called_with` method arguments are compared with the
+real callable signature and gives additional protection against
+changing the real callable interface.
+
 ## Installation
 
 ```bash
 pip install pytest-when
 ```
```

