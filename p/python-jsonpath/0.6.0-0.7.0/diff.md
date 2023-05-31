# Comparing `tmp/python_jsonpath-0.6.0.tar.gz` & `tmp/python_jsonpath-0.7.0.tar.gz`

## Comparing `python_jsonpath-0.6.0.tar` & `python_jsonpath-0.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/__about__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/__init__.py
--rw-r--r--   0        0        0    15062 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/env.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/exceptions.py
--rw-r--r--   0        0        0    12756 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/filter.py
--rw-r--r--   0        0        0    11063 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/lex.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/match.py
--rw-r--r--   0        0        0    20411 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/parse.py
--rw-r--r--   0        0        0    11290 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/path.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/py.typed
--rw-r--r--   0        0        0    23681 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/selectors.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/stream.py
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/token.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/__init__.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/arguments.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/count.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/is_instance.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/keys.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/length.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/match.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/search.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/typeof.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/jsonpath/function_extensions/value.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/README.md
--rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 python_jsonpath-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/__about__.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/__init__.py
+-rw-r--r--   0        0        0    15262 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/env.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/exceptions.py
+-rw-r--r--   0        0        0    13166 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/filter.py
+-rw-r--r--   0        0        0    11063 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/lex.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/match.py
+-rw-r--r--   0        0        0    20411 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/parse.py
+-rw-r--r--   0        0        0    11290 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/path.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/py.typed
+-rw-r--r--   0        0        0    23699 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/selectors.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/stream.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/token.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/__init__.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/arguments.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/count.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/is_instance.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/keys.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/length.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/match.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/search.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/typeof.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/value.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/README.md
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/PKG-INFO
```

### Comparing `python_jsonpath-0.6.0/jsonpath/__init__.py` & `python_jsonpath-0.7.0/jsonpath/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # SPDX-FileCopyrightText: 2023-present James Prior <jamesgr.prior@gmail.com>
 #
 # SPDX-License-Identifier: MIT
 
 from .env import JSONPathEnvironment
 from .exceptions import JSONPathError
+from .exceptions import JSONPathIndexError
 from .exceptions import JSONPathNameError
 from .exceptions import JSONPathSyntaxError
 from .exceptions import JSONPathTypeError
 from .filter import UNDEFINED
 from .lex import Lexer
 from .match import JSONPathMatch
 from .parse import Parser
@@ -20,14 +21,15 @@
     "findall_async",
     "findall",
     "finditer_async",
     "finditer",
     "JSONPath",
     "JSONPathEnvironment",
     "JSONPathError",
+    "JSONPathIndexError",
     "JSONPathMatch",
     "JSONPathNameError",
     "JSONPathSyntaxError",
     "JSONPathTypeError",
     "Lexer",
     "Parser",
     "UNDEFINED",
```

### Comparing `python_jsonpath-0.6.0/jsonpath/env.py` & `python_jsonpath-0.7.0/jsonpath/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 from . import function_extensions
 from .exceptions import JSONPathNameError
 from .exceptions import JSONPathSyntaxError
 from .filter import UNDEFINED
 from .function_extensions import validate
 from .lex import Lexer
+from .match import NodeList
 from .parse import Parser
 from .path import CompoundJSONPath
 from .path import JSONPath
 from .stream import TokenStream
 from .token import TOKEN_EOF
 from .token import TOKEN_INTERSECTION
 from .token import TOKEN_UNION
@@ -67,15 +68,15 @@
 
     ## Class attributes
 
     Attributes:
         filter_context_token (str): The pattern used to select extra filter context
             data. Defaults to `"_"`.
         intersection_token (str): The pattern used as the intersection operator.
-            Defaults to `"$"`.
+            Defaults to `"&"`.
         key_token (str): The pattern used to identify the current key or index when
             filtering a, mapping or sequence. Defaults to `"#"`.
         keys_selector_token (str): The pattern used as the "keys" selector. Defaults to
             `"~"`.
         lexer_class: The lexer to use when tokenizing path strings.
         max_int_index (int): The maximum integer allowed when selecting array items by
             index. Defaults to `(2**53) - 1`.
@@ -334,14 +335,19 @@
             operator: The comparison expression's operator.
             right: The right hand side of the comparison expression.
 
         Returns:
             `True` if the comparison between _left_ and _right_, with the
             given _operator_, is truthy. `False` otherwise.
         """
+        if isinstance(left, NodeList):
+            left = left.values_or_singular()
+        if isinstance(right, NodeList):
+            right = right.values_or_singular()
+
         if operator == "&&":
             return self.is_truthy(left) and self.is_truthy(right)
         if operator == "||":
             return self.is_truthy(left) or self.is_truthy(right)
 
         if operator == "==":
             return bool(left == right)
```

### Comparing `python_jsonpath-0.6.0/jsonpath/filter.py` & `python_jsonpath-0.7.0/jsonpath/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import List
 from typing import Mapping
 from typing import Pattern
 from typing import Sequence
 from typing import TypeVar
 
 from .exceptions import JSONPathTypeError
+from .match import NodeList
 
 if TYPE_CHECKING:
     from .path import JSONPath
     from .selectors import FilterContext
 
 # ruff: noqa: D102
 
@@ -338,90 +339,90 @@
             return UNDEFINED
         if not isinstance(context.current, (Sequence, Mapping)):
             if self.path.empty():
                 return context.current
             return UNDEFINED
 
         try:
-            matches = self.path.findall(context.current)
+            matches = NodeList(self.path.finditer(context.current))
         except json.JSONDecodeError:  # this should never happen
             return UNDEFINED
 
         if not matches:
             return UNDEFINED
-        if len(matches) == 1:
-            return matches[0]
         return matches
 
     async def evaluate_async(self, context: FilterContext) -> object:  # noqa: PLR0911
         if isinstance(context.current, str):
             if self.path.empty():
                 return context.current
             return UNDEFINED
         if not isinstance(context.current, (Sequence, Mapping)):
             if self.path.empty():
                 return context.current
             return UNDEFINED
 
         try:
-            matches = await self.path.findall_async(context.current)
+            matches = NodeList(
+                [
+                    match
+                    async for match in await self.path.finditer_async(context.current)
+                ]
+            )
         except json.JSONDecodeError:
             return UNDEFINED
 
         if not matches:
             return UNDEFINED
-        if len(matches) == 1:
-            return matches[0]
         return matches
 
 
 class RootPath(Path):
     """A JSONPath starting at the root node."""
 
     def __str__(self) -> str:
         return str(self.path)
 
     def evaluate(self, context: FilterContext) -> object:
-        matches = self.path.findall(context.root)
+        matches = NodeList(self.path.finditer(context.root))
         if not matches:
             return UNDEFINED
-        if len(matches) == 1:
-            return matches[0]
         return matches
 
     async def evaluate_async(self, context: FilterContext) -> object:
-        matches = await self.path.findall_async(context.root)
+        matches = NodeList(
+            [match async for match in await self.path.finditer_async(context.root)]
+        )
         if not matches:
             return UNDEFINED
-        if len(matches) == 1:
-            return matches[0]
         return matches
 
 
 class FilterContextPath(Path):
     """A JSONPath starting at the root of any extra context data."""
 
     def __str__(self) -> str:
         path_repr = str(self.path)
         return "_" + path_repr[1:]
 
     def evaluate(self, context: FilterContext) -> object:
-        matches = self.path.findall(context.extra_context)
+        matches = NodeList(self.path.finditer(context.extra_context))
         if not matches:
             return UNDEFINED
-        if len(matches) == 1:
-            return matches[0]
         return matches
 
     async def evaluate_async(self, context: FilterContext) -> object:
-        matches = await self.path.findall_async(context.extra_context)
+        matches = NodeList(
+            [
+                match
+                async for match in await self.path.finditer_async(context.extra_context)
+            ]
+        )
         if not matches:
             return UNDEFINED
-        if len(matches) == 1:
-            return matches[0]
         return matches
 
 
 class FunctionExtension(FilterExpression):
     """A filter function."""
 
     __slots__ = ("name", "args")
@@ -436,23 +437,33 @@
 
     def evaluate(self, context: FilterContext) -> object:
         try:
             func = context.env.function_extensions[self.name]
         except KeyError:
             return UNDEFINED
         args = [arg.evaluate(context) for arg in self.args]
-        return func(*args)
+        if getattr(func, "with_node_lists", False):
+            return func(*args)
+        return func(*self._unpack_node_lists(args))
 
     async def evaluate_async(self, context: FilterContext) -> object:
         try:
             func = context.env.function_extensions[self.name]
         except KeyError:
             return UNDEFINED
         args = [await arg.evaluate_async(context) for arg in self.args]
-        return func(*args)
+        if getattr(func, "with_node_lists", False):
+            return func(*args)
+        return func(*self._unpack_node_lists(args))
+
+    def _unpack_node_lists(self, args: List[object]) -> List[object]:
+        return [
+            obj.values_or_singular() if isinstance(obj, NodeList) else obj
+            for obj in args
+        ]
 
 
 class CurrentKey(FilterExpression):
     """The key/property or index associated with the current object."""
 
     __slots__ = ()
```

### Comparing `python_jsonpath-0.6.0/jsonpath/lex.py` & `python_jsonpath-0.7.0/jsonpath/lex.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.6.0/jsonpath/match.py` & `python_jsonpath-0.7.0/jsonpath/match.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,7 +72,21 @@
 def _truncate(val: str, num: int, end: str = "...") -> str:
     # Replaces consecutive whitespace with a single newline.
     # Treats quoted whitespace the same as unquoted whitespace.
     words = val.split()
     if len(words) < num:
         return " ".join(words)
     return " ".join(words[:num]) + end
+
+
+class NodeList(List[JSONPathMatch]):
+    """List of JSONPathMatch objects, analogous to the spec's nodelist."""
+
+    def values(self) -> List[object]:
+        """Return the values from this node list."""
+        return [match.obj for match in self]
+
+    def values_or_singular(self) -> object:
+        """Return the values from this node list."""
+        if len(self) == 1:
+            return self[0].obj
+        return [match.obj for match in self]
```

### Comparing `python_jsonpath-0.6.0/jsonpath/parse.py` & `python_jsonpath-0.7.0/jsonpath/parse.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.6.0/jsonpath/path.py` & `python_jsonpath-0.7.0/jsonpath/path.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.6.0/jsonpath/selectors.py` & `python_jsonpath-0.7.0/jsonpath/selectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,15 +249,15 @@
         return f"[{start}:{stop}:{step}]"
 
     def _check_range(self, *indices: Optional[int]) -> None:
         for i in indices:
             if i is not None and (
                 i < self.env.min_int_index or i > self.env.max_int_index
             ):
-                raise JSONPathIndexError("index out of range")
+                raise JSONPathIndexError("index out of range", token=self.token)
 
     def _normalized_index(self, obj: Sequence[object], index: int) -> int:
         if index < 0 and len(obj) >= abs(index):
             return len(obj) + index
         return index
 
     def resolve(self, matches: Iterable[JSONPathMatch]) -> Iterable[JSONPathMatch]:
```

### Comparing `python_jsonpath-0.6.0/jsonpath/stream.py` & `python_jsonpath-0.7.0/jsonpath/stream.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.6.0/jsonpath/token.py` & `python_jsonpath-0.7.0/jsonpath/token.py`

 * *Files 22% similar despite different names*

```diff
@@ -74,15 +74,24 @@
 
 # Extension tokens
 TOKEN_UNION = sys.intern("UNION")
 TOKEN_INTERSECTION = sys.intern("INTERSECT")
 
 
 class Token:
-    """A token, as returned from `lex.Lexer.tokenize()`."""
+    """A token, as returned from `lex.Lexer.tokenize()`.
+
+    Attributes:
+        kind (str): The token's type. It is always one of the constants defined
+            in _jsonpath.token.py_.
+        value (str): The _path_ substring containing text for the token.
+        index (str): The index at which _value_ starts in _path_.
+        path (str): A reference to the complete JSONPath string from which this
+            token derives.
+    """
 
     __slots__ = ("kind", "value", "index", "path")
 
     def __init__(
         self,
         kind: str,
         value: str,
```

### Comparing `python_jsonpath-0.6.0/jsonpath/function_extensions/arguments.py` & `python_jsonpath-0.7.0/jsonpath/function_extensions/arguments.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.6.0/jsonpath/function_extensions/count.py` & `python_jsonpath-0.7.0/jsonpath/function_extensions/match.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,56 @@
-"""The standard `count` function extension."""
-from collections.abc import Sized
+"""The standard `match` function extension."""
+
+import re
 from typing import TYPE_CHECKING
 from typing import List
-from typing import Optional
+from typing import Pattern
+from typing import Union
 
 from ..exceptions import JSONPathTypeError
-from ..filter import Literal
+from ..filter import RegexArgument
+from ..filter import StringLiteral
 
 if TYPE_CHECKING:
     from ..env import JSONPathEnvironment
     from ..token import Token
 
 
-class Count:
-    """The built-in `count` function."""
+class Match:
+    """The built-in `match` function.
+
+    This implementation uses the standard _re_ module, without attempting to map
+    I-Regexps to Python regex.
+    """
+
+    def __call__(self, string: str, pattern: Union[str, Pattern[str], None]) -> bool:
+        """Return `True` if _pattern_ matches the given string, `False` otherwise."""
+        # The IETF JSONPath draft requires us to return `False` if the pattern was
+        # invalid. We use `None` to indicate the pattern could not be compiled.
+        if string is None or pattern is None:
+            return False
 
-    def __call__(self, obj: Sized) -> Optional[int]:
-        """Return an object's length, or `None` if the object does not have a length."""
         try:
-            return len(obj)
-        except TypeError:
-            return None
+            return bool(re.fullmatch(pattern, string))
+        except (TypeError, re.error):
+            return False
 
     def validate(
         self,
         _: "JSONPathEnvironment",
         args: List[object],
         token: "Token",
     ) -> List[object]:
         """Function argument validation."""
-        if len(args) != 1:  # noqa: PLR2004
+        if len(args) != 2:  # noqa: PLR2004
             raise JSONPathTypeError(
-                f"{token.value!r} requires 1 arguments, found {len(args)}",
+                f"{token.value!r} requires 2 arguments, found {len(args)}",
                 token=token,
             )
 
-        if isinstance(args[0], Literal):
-            raise JSONPathTypeError(
-                f"{token.value!r} requires a node list, "
-                f"found {args[0].__class__.__name__}",
-                token=token,
-            )
+        if isinstance(args[1], StringLiteral):
+            try:
+                return [args[0], RegexArgument(re.compile(args[1].value))]
+            except re.error:
+                return [None, None]
 
         return args
```

### Comparing `python_jsonpath-0.6.0/jsonpath/function_extensions/is_instance.py` & `python_jsonpath-0.7.0/jsonpath/function_extensions/is_instance.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def __call__(self, obj: object, t: str) -> bool:  # noqa: PLR0911
         """Return `True` if the type of _obj_ matches _t_.
 
         This function allows _t_ to be one of several aliases for the real
         Python "type". Some of these aliases follow JavaScript/JSON semantics.
         """
         if obj is UNDEFINED or obj is UNDEFINED_LITERAL:
-            return t == "undefined"
+            return t in ("undefined", "missing")
         if obj is None:
             return t in ("null", "nil", "None", "none")
         if isinstance(obj, str):
             return t in ("str", "string")
         if isinstance(obj, Sequence):
             return t in ("array", "list", "sequence", "tuple")
         if isinstance(obj, Mapping):
```

### Comparing `python_jsonpath-0.6.0/jsonpath/function_extensions/match.py` & `python_jsonpath-0.7.0/jsonpath/function_extensions/search.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""The standard `match` function extension."""
+"""The standard `search` function extension."""
 
 import re
 from typing import TYPE_CHECKING
 from typing import List
 from typing import Pattern
 from typing import Union
 
@@ -11,30 +11,30 @@
 from ..filter import StringLiteral
 
 if TYPE_CHECKING:
     from ..env import JSONPathEnvironment
     from ..token import Token
 
 
-class Match:
-    """The built-in `match` function.
+class Search:
+    """The built-in `search` function.
 
     This implementation uses the standard _re_ module, without attempting to map
     I-Regexps to Python regex.
     """
 
     def __call__(self, string: str, pattern: Union[str, Pattern[str], None]) -> bool:
-        """Return `True` if _pattern_ matches the given string, `False` otherwise."""
+        """Return `True` if the given string contains _pattern_, `False` otherwise."""
         # The IETF JSONPath draft requires us to return `False` if the pattern was
         # invalid. We use `None` to indicate the pattern could not be compiled.
         if string is None or pattern is None:
             return False
 
         try:
-            return bool(re.fullmatch(pattern, string))
+            return bool(re.search(pattern, string))
         except (TypeError, re.error):
             return False
 
     def validate(
         self,
         _: "JSONPathEnvironment",
         args: List[object],
```

### Comparing `python_jsonpath-0.6.0/jsonpath/function_extensions/typeof.py` & `python_jsonpath-0.7.0/jsonpath/function_extensions/typeof.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.6.0/.gitignore` & `python_jsonpath-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.6.0/LICENSE.txt` & `python_jsonpath-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.6.0/README.md` & `python_jsonpath-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.6.0/pyproject.toml` & `python_jsonpath-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 omit = ["jsonpath/__about__.py", "tests/compliance.py", "tests/consensus.py"]
 
 [tool.coverage.report]
 exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
 
 [tool.mypy]
 files = "jsonpath"
-python_version = "3.10"
+python_version = "3.11"
 disallow_subclassing_any = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 no_implicit_optional = true
 local_partial_types = true
 no_implicit_reexport = true
@@ -125,15 +125,15 @@
   "SIM",
   "SLF",
   "T10",
   "T20",
   "TCH",
   "YTT",
 ]
-ignore = ["S105", "S101", "D107", "D105"]
+ignore = ["S105", "S101", "D107", "D105", "PLR0913"]
 
 fixable = ["I"]
 unfixable = []
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
   ".bzr",
```

### Comparing `python_jsonpath-0.6.0/PKG-INFO` & `python_jsonpath-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-jsonpath
-Version: 0.6.0
+Version: 0.7.0
 Summary: Another JSONPath implementation for Python.
 Project-URL: Documentation, https://jg-rp.github.io/python-jsonpath/
 Project-URL: Issues, https://github.com/jg-rp/python-jsonpath/issues
 Project-URL: Source, https://github.com/jg-rp/python-jsonpath
 Author-email: James Prior <jamesgr.prior@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-jsonpath Version: 0.6.0 Summary: Another
+Metadata-Version: 2.1 Name: python-jsonpath Version: 0.7.0 Summary: Another
 JSONPath implementation for Python. Project-URL: Documentation, https://jg-
 rp.github.io/python-jsonpath/ Project-URL: Issues, https://github.com/jg-rp/
 python-jsonpath/issues Project-URL: Source, https://github.com/jg-rp/python-
 jsonpath Author-email: James Prior
 prior@gmail.com> License-Expression: MIT License-File: LICENSE.txt Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
```

