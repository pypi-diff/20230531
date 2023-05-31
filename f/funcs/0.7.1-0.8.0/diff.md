# Comparing `tmp/funcs-0.7.1.tar.gz` & `tmp/funcs-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs-0.7.1.tar", max compression
+gzip compressed data, was "funcs-0.8.0.tar", max compression
```

## Comparing `funcs-0.7.1.tar` & `funcs-0.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1092 2023-05-23 23:04:28.691680 funcs-0.7.1/LICENSE
--rw-r--r--   0        0        0     2872 2023-05-23 23:04:28.691680 funcs-0.7.1/README.md
--rw-r--r--   0        0        0     1714 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/__init__.py
--rw-r--r--   0        0        0      883 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/application.py
--rw-r--r--   0        0        0      857 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/callers.py
--rw-r--r--   0        0        0     5470 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/composition.py
--rw-r--r--   0        0        0      832 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/debug.py
--rw-r--r--   0        0        0      436 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/decorators.py
--rw-r--r--   0        0        0     6369 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/flow.py
--rw-r--r--   0        0        0     2260 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/functions.py
--rw-r--r--   0        0        0      418 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/getters.py
--rw-r--r--   0        0        0      782 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/primitives.py
--rw-r--r--   0        0        0        0 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/py.typed
--rw-r--r--   0        0        0     1113 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/reduction.py
--rw-r--r--   0        0        0     1031 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/types.py
--rw-r--r--   0        0        0     2346 2023-05-23 23:04:28.691680 funcs-0.7.1/funcs/unpacking.py
--rw-r--r--   0        0        0     3212 2023-05-23 23:04:28.691680 funcs-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     4102 1970-01-01 00:00:00.000000 funcs-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-31 10:51:46.841942 funcs-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2872 2023-05-31 10:51:46.841942 funcs-0.8.0/README.md
+-rw-r--r--   0        0        0     1724 2023-05-31 10:51:46.841942 funcs-0.8.0/funcs/__init__.py
+-rw-r--r--   0        0        0      883 2023-05-31 10:51:46.841942 funcs-0.8.0/funcs/application.py
+-rw-r--r--   0        0        0     1079 2023-05-31 10:51:46.841942 funcs-0.8.0/funcs/callers.py
+-rw-r--r--   0        0        0     5470 2023-05-31 10:51:46.841942 funcs-0.8.0/funcs/composition.py
+-rw-r--r--   0        0        0      832 2023-05-31 10:51:46.841942 funcs-0.8.0/funcs/debug.py
+-rw-r--r--   0        0        0      436 2023-05-31 10:51:46.841942 funcs-0.8.0/funcs/decorators.py
+-rw-r--r--   0        0        0     6369 2023-05-31 10:51:46.841942 funcs-0.8.0/funcs/flow.py
+-rw-r--r--   0        0        0     2644 2023-05-31 10:51:46.841942 funcs-0.8.0/funcs/functions.py
+-rw-r--r--   0        0        0      418 2023-05-31 10:51:46.841942 funcs-0.8.0/funcs/getters.py
+-rw-r--r--   0        0        0      782 2023-05-31 10:51:46.841942 funcs-0.8.0/funcs/primitives.py
+-rw-r--r--   0        0        0        0 2023-05-31 10:51:46.841942 funcs-0.8.0/funcs/py.typed
+-rw-r--r--   0        0        0     1113 2023-05-31 10:51:46.841942 funcs-0.8.0/funcs/reduction.py
+-rw-r--r--   0        0        0     1031 2023-05-31 10:51:46.841942 funcs-0.8.0/funcs/types.py
+-rw-r--r--   0        0        0     2346 2023-05-31 10:51:46.841942 funcs-0.8.0/funcs/unpacking.py
+-rw-r--r--   0        0        0     3212 2023-05-31 10:51:46.841942 funcs-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4102 1970-01-01 00:00:00.000000 funcs-0.8.0/PKG-INFO
```

### Comparing `funcs-0.7.1/LICENSE` & `funcs-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `funcs-0.7.1/README.md` & `funcs-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add funcs
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-funcs = "^0.7.1"
+funcs = "^0.8.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.funcs]
 git = "https://github.com/nekitdev/funcs.git"
```

### Comparing `funcs-0.7.1/funcs/__init__.py` & `funcs-0.8.0/funcs/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 __description__ = "Functional programming in Python."
 __url__ = "https://github.com/nekitdev/funcs"
 
 __title__ = "funcs"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "0.7.1"
+__version__ = "0.8.0"
 
 from funcs.application import apply, partial
 from funcs.callers import caller, method_caller
 from funcs.composition import compose, compose_once, pipe, pipe_once
 from funcs.debug import inspect, tap
 from funcs.decorators import wraps
 from funcs.flow import once, post_processing, reraise, reraise_with, suppress, wrap_with
-from funcs.functions import always, asyncify, complement, flip, identity, raises
+from funcs.functions import always, asyncify, awaiting, complement, flip, identity, raises
 from funcs.getters import attribute_getter, item_getter
 from funcs.primitives import decrement, increment, is_even, is_odd
 from funcs.reduction import fold, reduce
 from funcs.unpacking import (
     unpack_binary,
     unpack_nullary,
     unpack_quaternary,
```

### Comparing `funcs-0.7.1/funcs/application.py` & `funcs-0.8.0/funcs/application.py`

 * *Files identical despite different names*

### Comparing `funcs-0.7.1/funcs/callers.py` & `funcs-0.8.0/funcs/callers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 from operator import methodcaller as standard_method_caller
 from typing import Any, TypeVar
 
-from typing_aliases import DynamicCallable, Unary
-from typing_extensions import ParamSpec
+from attrs import frozen
+from typing_aliases import DynamicCallable, DynamicTuple, StringDict, Unary
+from typing_extensions import ParamSpec, final
 
 __all__ = ("caller", "method_caller")
 
 method_caller = standard_method_caller
 """An alias of the standard `method_caller` type that implements method calling."""
 
 P = ParamSpec("P")
 
 R = TypeVar("R")
 
 
+@final
+@frozen()
+class Caller:
+    """Represents function callers."""
+
+    args: DynamicTuple[Any]
+    kwargs: StringDict[Any]
+
+    def __call__(self, function: DynamicCallable[R]) -> R:
+        return function(*self.args, **self.kwargs)
+
+
 def caller(*args: Any, **kwargs: Any) -> Unary[DynamicCallable[R], R]:
-    """Creates a function that calls the given `function` with `*args` and `**kwargs`.
+    """Creates a [`Caller`][funcs.callers.Caller] that calls the given
+    `function` with `*args` and `**kwargs`.
 
     Arguments:
         *args: The arguments to use.
         **kwargs: The keyword arguments to use.
 
     Returns:
-        The function that calls the given `function` with `*args` and `**kwargs`.
+        The [`Caller`][funcs.callers.Caller] created.
     """
-
-    def call(function: DynamicCallable[R]) -> R:
-        return function(*args, **kwargs)
-
-    return call
+    return Caller(args, kwargs)
```

### Comparing `funcs-0.7.1/funcs/composition.py` & `funcs-0.8.0/funcs/composition.py`

 * *Files identical despite different names*

### Comparing `funcs-0.7.1/funcs/debug.py` & `funcs-0.8.0/funcs/debug.py`

 * *Files identical despite different names*

### Comparing `funcs-0.7.1/funcs/flow.py` & `funcs-0.8.0/funcs/flow.py`

 * *Files identical despite different names*

### Comparing `funcs-0.7.1/funcs/functions.py` & `funcs-0.8.0/funcs/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,37 @@
-from typing import Callable, TypeVar
+from typing import Awaitable, Callable, TypeVar
 
 from typing_aliases import AnyError, AsyncCallable, Binary, GenericPredicate, Nullary
 from typing_extensions import Never, ParamSpec
 
-__all__ = ("asyncify", "identity", "always", "raises", "flip", "complement")
+__all__ = ("awaiting", "asyncify", "identity", "always", "raises", "flip", "complement")
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 R = TypeVar("R")
 
 P = ParamSpec("P")
 
 
+async def awaiting(awaitable: Awaitable[T]) -> T:
+    """Wraps an awaitable into a coroutine.
+
+    This function is useful in, for example, [`asyncio`][asyncio],
+    where some functions expect coroutines only.
+
+    Arguments:
+        awaitable: The awaitable to wrap.
+
+    Returns:
+        The result of `await awaitable`.
+    """
+    return await awaitable
+
+
 def asyncify(function: Callable[P, R]) -> AsyncCallable[P, R]:
     """Wraps the synchronous function to be called asynchronously.
 
     Arguments:
         function: The synchronous function to wrap.
 
     Returns:
```

### Comparing `funcs-0.7.1/funcs/primitives.py` & `funcs-0.8.0/funcs/primitives.py`

 * *Files identical despite different names*

### Comparing `funcs-0.7.1/funcs/reduction.py` & `funcs-0.8.0/funcs/reduction.py`

 * *Files identical despite different names*

### Comparing `funcs-0.7.1/funcs/types.py` & `funcs-0.8.0/funcs/types.py`

 * *Files identical despite different names*

### Comparing `funcs-0.7.1/funcs/unpacking.py` & `funcs-0.8.0/funcs/unpacking.py`

 * *Files identical despite different names*

### Comparing `funcs-0.7.1/pyproject.toml` & `funcs-0.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "funcs"
-version = "0.7.1"
+version = "0.8.0"
 description = "Functional programming in Python."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/funcs"
@@ -136,15 +136,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "funcs"
-version = "0.7.1"
+version = "0.8.0"
 url = "https://github.com/nekitdev/funcs"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `funcs-0.7.1/PKG-INFO` & `funcs-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs
-Version: 0.7.1
+Version: 0.8.0
 Summary: Functional programming in Python.
 Home-page: https://github.com/nekitdev/funcs
 License: MIT
 Keywords: python,function,functional,paradigm
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -71,15 +71,15 @@
 $ poetry add funcs
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-funcs = "^0.7.1"
+funcs = "^0.8.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.funcs]
 git = "https://github.com/nekitdev/funcs.git"
```

