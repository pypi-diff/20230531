# Comparing `tmp/annotated_types-0.4.0.tar.gz` & `tmp/annotated_types-0.5.0.tar.gz`

## Comparing `annotated_types-0.4.0.tar` & `annotated_types-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 annotated_types-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 annotated_types-0.4.0/Makefile
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 annotated_types-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     8868 2020-02-02 00:00:00.000000 annotated_types-0.4.0/annotated_types/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 annotated_types-0.4.0/annotated_types/py.typed
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 annotated_types-0.4.0/annotated_types/test_cases.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 annotated_types-0.4.0/requirements/all.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 annotated_types-0.4.0/requirements/linting.in
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 annotated_types-0.4.0/requirements/linting.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 annotated_types-0.4.0/requirements/testing.in
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 annotated_types-0.4.0/requirements/testing.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 annotated_types-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 annotated_types-0.4.0/tests/test_grouped_metadata.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 annotated_types-0.4.0/tests/test_main.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 annotated_types-0.4.0/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 annotated_types-0.4.0/LICENSE
--rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 annotated_types-0.4.0/README.md
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 annotated_types-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    13006 2020-02-02 00:00:00.000000 annotated_types-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 annotated_types-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 annotated_types-0.5.0/Makefile
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 annotated_types-0.5.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 annotated_types-0.5.0/annotated_types/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 annotated_types-0.5.0/annotated_types/py.typed
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 annotated_types-0.5.0/annotated_types/test_cases.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 annotated_types-0.5.0/requirements/all.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 annotated_types-0.5.0/requirements/linting.in
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 annotated_types-0.5.0/requirements/linting.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 annotated_types-0.5.0/requirements/testing.in
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 annotated_types-0.5.0/requirements/testing.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 annotated_types-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 annotated_types-0.5.0/tests/test_grouped_metadata.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 annotated_types-0.5.0/tests/test_main.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 annotated_types-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 annotated_types-0.5.0/LICENSE
+-rw-r--r--   0        0        0    10505 2020-02-02 00:00:00.000000 annotated_types-0.5.0/README.md
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 annotated_types-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    11685 2020-02-02 00:00:00.000000 annotated_types-0.5.0/PKG-INFO
```

### Comparing `annotated_types-0.4.0/.pre-commit-config.yaml` & `annotated_types-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `annotated_types-0.4.0/Makefile` & `annotated_types-0.5.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 .PHONY: testcov
 testcov: test
 	@coverage report --show-missing
 	@coverage html
 
 .PHONY: mypy
 mypy:
-	mypy annotated_types
+	mypy annotated_types tests
 
 .PHONY: all
 all: lint mypy testcov
 
 .PHONY: clean
 clean:
 	rm -rf `find . -name __pycache__`
```

### Comparing `annotated_types-0.4.0/.github/workflows/ci.yml` & `annotated_types-0.5.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `annotated_types-0.4.0/annotated_types/__init__.py` & `annotated_types-0.5.0/annotated_types/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import sys
 from dataclasses import dataclass
 from datetime import timezone
-from typing import Any, Callable, Iterator, Optional, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Callable, Iterator, Optional, TypeVar, Union
 
 if sys.version_info < (3, 8):
-    from typing_extensions import Protocol
+    from typing_extensions import Protocol, runtime_checkable
 else:
-    from typing import Protocol
+    from typing import Protocol, runtime_checkable
 
 if sys.version_info < (3, 9):
-    from typing_extensions import Annotated
+    from typing_extensions import Annotated, Literal
 else:
-    from typing import Annotated
+    from typing import Annotated, Literal
 
 if sys.version_info < (3, 10):
     EllipsisType = type(Ellipsis)
     KW_ONLY = {}
     SLOTS = {}
 else:
     from types import EllipsisType
@@ -40,15 +40,15 @@
     'Predicate',
     'LowerCase',
     'UpperCase',
     'IsDigits',
     '__version__',
 )
 
-__version__ = '0.4.0'
+__version__ = '0.5.0'
 
 
 T = TypeVar('T')
 
 
 # arguments that start with __ are considered
 # positional only
@@ -135,15 +135,16 @@
     It can be used with any type that supports the ``<=`` operator,
     including numbers, dates and times, strings, sets, and so on.
     """
 
     le: SupportsLe
 
 
-class GroupedMetadata:
+@runtime_checkable
+class GroupedMetadata(Protocol):
     """A grouping of multiple BaseMetadata objects.
 
     `GroupedMetadata` on its own is not metadata and has no meaning.
     All it the the constraint and metadata should be fully expressable
     in terms of the `BaseMetadata`'s returned by `GroupedMetadata.__iter__()`.
 
     Concrete implementations should override `GroupedMetadata.__iter__()`
@@ -166,23 +167,32 @@
     Parsers should recognize this and unpack it so that it can be used
     both with and without unpacking:
 
     - `Annotated[int, Field(...)]` (parser must unpack Field)
     - `Annotated[int, *Field(...)]` (PEP-646)
     """  # noqa: trailing-whitespace
 
-    __slots__ = ()
-
-    def __init_subclass__(cls, *args: Any, **kwargs: Any) -> None:
-        super().__init_subclass__(*args, **kwargs)
-        if cls.__iter__ is GroupedMetadata.__iter__:
-            raise TypeError("Can't subclass GroupedMetadata without implementing __iter__")
+    @property
+    def __is_annotated_types_grouped_metadata__(self) -> Literal[True]:
+        return True
 
     def __iter__(self) -> Iterator[BaseMetadata]:
-        raise NotImplementedError
+        ...
+
+    if not TYPE_CHECKING:
+        __slots__ = ()  # allow subclasses to use slots
+
+        def __init_subclass__(cls, *args: Any, **kwargs: Any) -> None:
+            # Basic ABC like functionality without the complexity of an ABC
+            super().__init_subclass__(*args, **kwargs)
+            if cls.__iter__ is GroupedMetadata.__iter__:
+                raise TypeError("Can't subclass GroupedMetadata without implementing __iter__")
+
+        def __iter__(self) -> Iterator[BaseMetadata]:  # noqa: F811
+            raise NotImplementedError  # more helpful than "None has no attribute..." type errors
 
 
 @dataclass(frozen=True, **KW_ONLY, **SLOTS)
 class Interval(GroupedMetadata):
     """Interval can express inclusive or exclusive bounds with a single object.
 
     It accepts keyword arguments ``gt``, ``ge``, ``lt``, and/or ``le``, which
@@ -261,15 +271,15 @@
 
 @dataclass(frozen=True, **SLOTS)
 class Timezone(BaseMetadata):
     """Timezone(tz=...) requires a datetime to be aware (or ``tz=None``, naive).
 
     ``Annotated[datetime, Timezone(None)]`` must be a naive datetime.
     ``Timezone[...]`` (the ellipsis literal) expresses that the datetime must be
-    tz-aware bug any timezone is allowed.
+    tz-aware but any timezone is allowed.
 
     You may also pass a specific timezone string or timezone object such as
     ``Timezone(timezone.utc)`` or ``Timezone("Africa/Abidjan")`` to express that
     you only allow a specific timezone, though we note that this is often
     a symptom of poor design.
     """
```

### Comparing `annotated_types-0.4.0/annotated_types/test_cases.py` & `annotated_types-0.5.0/annotated_types/test_cases.py`

 * *Files identical despite different names*

### Comparing `annotated_types-0.4.0/requirements/linting.txt` & `annotated_types-0.5.0/requirements/linting.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,77 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
 #
 #    pip-compile --output-file=requirements/linting.txt --resolver=backtracking requirements/linting.in
 #
 black==22.8.0
     # via -r requirements/linting.in
 cfgv==3.3.1
     # via pre-commit
 click==8.1.3
     # via black
 colorama==0.4.5
     # via isort
 distlib==0.3.6
     # via virtualenv
+exceptiongroup==1.1.1
+    # via pytest
 filelock==3.8.0
     # via virtualenv
 flake8==5.0.4
     # via
     #   -r requirements/linting.in
     #   flake8-pyproject
 flake8-pyproject==1.1.0.post0
     # via -r requirements/linting.in
 identify==2.5.5
     # via pre-commit
+iniconfig==2.0.0
+    # via pytest
 isort[colors]==5.10.1
     # via -r requirements/linting.in
 mccabe==0.7.0
     # via flake8
 mypy==0.971
     # via -r requirements/linting.in
 mypy-extensions==0.4.3
     # via
     #   black
     #   mypy
 nodeenv==1.7.0
     # via pre-commit
+packaging==23.1
+    # via pytest
 pathspec==0.10.1
     # via black
 platformdirs==2.5.2
     # via
     #   black
     #   virtualenv
+pluggy==1.0.0
+    # via pytest
 pre-commit==2.20.0
     # via -r requirements/linting.in
 pycodestyle==2.9.1
     # via flake8
 pyflakes==2.5.0
     # via flake8
+pytest==7.3.1
+    # via -r requirements/linting.in
 pyyaml==6.0
     # via pre-commit
 toml==0.10.2
     # via pre-commit
 tomli==2.0.1
     # via
     #   black
     #   flake8-pyproject
     #   mypy
+    #   pytest
 typing-extensions==4.3.0
     # via mypy
 virtualenv==20.16.5
     # via pre-commit
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `annotated_types-0.4.0/requirements/testing.txt` & `annotated_types-0.5.0/requirements/testing.txt`

 * *Files identical despite different names*

### Comparing `annotated_types-0.4.0/tests/test_main.py` & `annotated_types-0.5.0/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,16 @@
     for example in case.invalid_cases:
         yield pytest.param(case.annotation, example, id=f"{case.annotation} is invalid for {repr(example)}")
 
 
 @pytest.mark.parametrize(
     "annotation, example", [testcase for case in cases() for testcase in extract_valid_testcases(case)]
 )
-def test_valid_cases(annotation: type, example: Any):
+def test_valid_cases(annotation: type, example: Any) -> None:
     assert is_valid(annotation, example) is True
 
 
 @pytest.mark.parametrize(
     "annotation, example", [testcase for case in cases() for testcase in extract_invalid_testcases(case)]
 )
-def test_invalid_cases(annotation: type, example: Any):
+def test_invalid_cases(annotation: type, example: Any) -> None:
     assert is_valid(annotation, example) is False
```

### Comparing `annotated_types-0.4.0/LICENSE` & `annotated_types-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `annotated_types-0.4.0/README.md` & `annotated_types-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [PEP-593](https://peps.python.org/pep-0593/) added `typing.Annotated` as a way of
 adding context-specific metadata to existing types, and specifies that
 `Annotated[T, x]` _should_ be treated as `T` by any tool or library without special
 logic for `x`.
 
 This package provides metadata objects which can be used to represent common
 constraints such as upper and lower bounds on scalar values and collection sizes,
-a `Predicate` marker for runtime checks, and [non-normative](https://developer.mozilla.org/en-US/docs/Glossary/non-normative)
+a `Predicate` marker for runtime checks, and
 descriptions of how we intend these metadata to be interpreted. In some cases,
 we also note alternative representations which do not require this package.
 
 ## Install
 
 ```bash
 pip install annotated-types
@@ -30,18 +30,16 @@
 
 class MyClass:
     age: Annotated[int, Gt(18)]                         # Valid: 19, 20, ...
                                                         # Invalid: 17, 18, "19", 19.0, ...
     factors: list[Annotated[int, Predicate(is_prime)]]  # Valid: 2, 3, 5, 7, 11, ...
                                                         # Invalid: 4, 8, -2, 5.0, "prime", ...
 
-    my_list: Annotated[list[int], 0:10]                 # Valid: [], [10, 20, 30, 40, 50]
+    my_list: Annotated[list[int], Len(0, 10)]           # Valid: [], [10, 20, 30, 40, 50]
                                                         # Invalid: (1, 2), ["abc"], [0] * 20
-    your_set: Annotated[set[int], Len(0, 10)]           # Valid: {1, 2, 3}, ...
-                                                        # Invalid: "Well, you get the idea!"
 ```
 
 ## Documentation
 
 _While `annotated-types` avoids runtime checks for performance, users should not
 construct invalid combinations such as `MultipleOf("non-numeric")` or `Annotated[int, Len(3)]`.
 Downstream implementors may choose to raise an error, emit a warning, silently ignore
@@ -50,15 +48,14 @@
 
 ### Gt, Ge, Lt, Le
 
 Express inclusive and/or exclusive bounds on orderable values - which may be numbers,
 dates, times, strings, sets, etc. Note that the boundary value need not be of the
 same type that was annotated, so long as they can be compared: `Annotated[int, Gt(1.5)]`
 is fine, for example, and implies that the value is an integer x such that `x > 1.5`.
-No interpretation is specified for special values such as `nan`.
 
 We suggest that implementors may also interpret `functools.partial(operator.le, 1.5)`
 as being equivalent to `Gt(1.5)`, for users who wish to avoid a runtime dependency on
 the `annotated-types` package.
 
 To be explicit, these types have the following meanings:
 
@@ -128,20 +125,20 @@
 
 `Predicate(func: Callable)` expresses that `func(value)` is truthy for valid values.
 Users should prefer the statically inspectable metadata above, but if you need
 the full power and flexibility of arbitrary runtime predicates... here it is.
 
 We provide a few predefined predicates for common string constraints:
 `IsLower = Predicate(str.islower)`, `IsUpper = Predicate(str.isupper)`, and
-`IsDigit = Predicate(str.isdigit)`. Users are encouraged to use methods which
-can be given special handling, and avoid indirection like `lambda s: s.lower()`.
-
+`IsDigit = Predicate(str.isdigit)`.
 Some libraries might have special logic to handle known or understandable predicates,
 for example by checking for `str.isdigit` and using its presence to both call custom
 logic to enforce digit-only strings, and customise some generated external schema.
+Users are therefore encouraged to avoid indirection like `lambda s: s.lower()`, in
+favor of introspectable methods such as `str.lower` or `re.compile("pattern").search`.
 
 We do not specify what behaviour should be expected for predicates that raise
 an exception.  For example `Annotated[int, Predicate(str.isdigit)]` might silently
 skip invalid constraints, or statically raise an error; or it might try calling it
 and then propogate or discard the resulting
 `TypeError: descriptor 'isdigit' for 'str' objects doesn't apply to a 'int' object`
 exception.  We encourage libraries to document the behaviour they choose.
@@ -170,14 +167,16 @@
             yield Ge(self.ge)
         if self.description is not None:
             yield Description(self.description)
 ```
 
 Libraries consuming annotated-types constraints should check for `GroupedMetadata` and unpack it by iterating over the object and treating the results as if they had been "unpacked" in the `Annotated` type.  The same logic should be applied to the [PEP 646 `Unpack` type](https://peps.python.org/pep-0646/), so that `Annotated[T, Field(...)]`, `Annotated[T, Unpack[Field(...)]]` and `Annotated[T, *Field(...)]` are all treated consistently.
 
+Libraries consuming annotated-types should also ignore any metadata they do not recongize that came from unpacking a `GroupedMetadata`, just like they ignore unrecognized metadata in `Annotated` itself.
+
 Our own `annotated_types.Interval` class is a `GroupedMetadata` which unpacks itself into `Gt`, `Lt`, etc., so this is not an abstract concern.  Similarly, `annotated_types.Len` is a `GroupedMetadata` which unpacks itself into `MinLen` (optionally) and `MaxLen`.
 
 ### Consuming metadata
 
 We intend to not be perspcriptive as to _how_ the metadata and constraints are used, but as an example of how one might parse constraints from types annotations see our [implementation in `test_main.py`](https://github.com/annotated-types/annotated-types/blob/f59cf6d1b5255a0fe359b93896759a180bec30ae/tests/test_main.py#L94-L103).
 
 It is up to the implementer to determine how this metadata is used.
```

### Comparing `annotated_types-0.4.0/pyproject.toml` & `annotated_types-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 authors = [
     {name = "Samuel Colvin", email = "s@muelcolvin.com"},
     {name = "Adrian Garcia Badaracco", email = "1755071+adriangb@users.noreply.github.com"},
     {name = "Zac Hatfield-Dodds", email = "zac@zhd.dev"},
 ]
 readme = "README.md"
 repository = "https://github.com/annotated-types/annotated-types"
-license = {file = "LICENSE"}
+license-files = { paths = ['LICENSE'] }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Operating System :: Unix",
     "Operating System :: POSIX :: Linux",
     "Environment :: Console",
```

### Comparing `annotated_types-0.4.0/PKG-INFO` & `annotated_types-0.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,12 @@
 Metadata-Version: 2.1
 Name: annotated-types
-Version: 0.4.0
+Version: 0.5.0
 Summary: Reusable constraint types to use with typing.Annotated
 Author-email: Samuel Colvin <s@muelcolvin.com>, Adrian Garcia Badaracco <1755071+adriangb@users.noreply.github.com>, Zac Hatfield-Dodds <zac@zhd.dev>
-License: The MIT License (MIT)
-        
-        Copyright (c) 2022 the contributors
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
@@ -55,15 +34,15 @@
 [PEP-593](https://peps.python.org/pep-0593/) added `typing.Annotated` as a way of
 adding context-specific metadata to existing types, and specifies that
 `Annotated[T, x]` _should_ be treated as `T` by any tool or library without special
 logic for `x`.
 
 This package provides metadata objects which can be used to represent common
 constraints such as upper and lower bounds on scalar values and collection sizes,
-a `Predicate` marker for runtime checks, and [non-normative](https://developer.mozilla.org/en-US/docs/Glossary/non-normative)
+a `Predicate` marker for runtime checks, and
 descriptions of how we intend these metadata to be interpreted. In some cases,
 we also note alternative representations which do not require this package.
 
 ## Install
 
 ```bash
 pip install annotated-types
@@ -77,18 +56,16 @@
 
 class MyClass:
     age: Annotated[int, Gt(18)]                         # Valid: 19, 20, ...
                                                         # Invalid: 17, 18, "19", 19.0, ...
     factors: list[Annotated[int, Predicate(is_prime)]]  # Valid: 2, 3, 5, 7, 11, ...
                                                         # Invalid: 4, 8, -2, 5.0, "prime", ...
 
-    my_list: Annotated[list[int], 0:10]                 # Valid: [], [10, 20, 30, 40, 50]
+    my_list: Annotated[list[int], Len(0, 10)]           # Valid: [], [10, 20, 30, 40, 50]
                                                         # Invalid: (1, 2), ["abc"], [0] * 20
-    your_set: Annotated[set[int], Len(0, 10)]           # Valid: {1, 2, 3}, ...
-                                                        # Invalid: "Well, you get the idea!"
 ```
 
 ## Documentation
 
 _While `annotated-types` avoids runtime checks for performance, users should not
 construct invalid combinations such as `MultipleOf("non-numeric")` or `Annotated[int, Len(3)]`.
 Downstream implementors may choose to raise an error, emit a warning, silently ignore
@@ -97,15 +74,14 @@
 
 ### Gt, Ge, Lt, Le
 
 Express inclusive and/or exclusive bounds on orderable values - which may be numbers,
 dates, times, strings, sets, etc. Note that the boundary value need not be of the
 same type that was annotated, so long as they can be compared: `Annotated[int, Gt(1.5)]`
 is fine, for example, and implies that the value is an integer x such that `x > 1.5`.
-No interpretation is specified for special values such as `nan`.
 
 We suggest that implementors may also interpret `functools.partial(operator.le, 1.5)`
 as being equivalent to `Gt(1.5)`, for users who wish to avoid a runtime dependency on
 the `annotated-types` package.
 
 To be explicit, these types have the following meanings:
 
@@ -175,20 +151,20 @@
 
 `Predicate(func: Callable)` expresses that `func(value)` is truthy for valid values.
 Users should prefer the statically inspectable metadata above, but if you need
 the full power and flexibility of arbitrary runtime predicates... here it is.
 
 We provide a few predefined predicates for common string constraints:
 `IsLower = Predicate(str.islower)`, `IsUpper = Predicate(str.isupper)`, and
-`IsDigit = Predicate(str.isdigit)`. Users are encouraged to use methods which
-can be given special handling, and avoid indirection like `lambda s: s.lower()`.
-
+`IsDigit = Predicate(str.isdigit)`.
 Some libraries might have special logic to handle known or understandable predicates,
 for example by checking for `str.isdigit` and using its presence to both call custom
 logic to enforce digit-only strings, and customise some generated external schema.
+Users are therefore encouraged to avoid indirection like `lambda s: s.lower()`, in
+favor of introspectable methods such as `str.lower` or `re.compile("pattern").search`.
 
 We do not specify what behaviour should be expected for predicates that raise
 an exception.  For example `Annotated[int, Predicate(str.isdigit)]` might silently
 skip invalid constraints, or statically raise an error; or it might try calling it
 and then propogate or discard the resulting
 `TypeError: descriptor 'isdigit' for 'str' objects doesn't apply to a 'int' object`
 exception.  We encourage libraries to document the behaviour they choose.
@@ -217,14 +193,16 @@
             yield Ge(self.ge)
         if self.description is not None:
             yield Description(self.description)
 ```
 
 Libraries consuming annotated-types constraints should check for `GroupedMetadata` and unpack it by iterating over the object and treating the results as if they had been "unpacked" in the `Annotated` type.  The same logic should be applied to the [PEP 646 `Unpack` type](https://peps.python.org/pep-0646/), so that `Annotated[T, Field(...)]`, `Annotated[T, Unpack[Field(...)]]` and `Annotated[T, *Field(...)]` are all treated consistently.
 
+Libraries consuming annotated-types should also ignore any metadata they do not recongize that came from unpacking a `GroupedMetadata`, just like they ignore unrecognized metadata in `Annotated` itself.
+
 Our own `annotated_types.Interval` class is a `GroupedMetadata` which unpacks itself into `Gt`, `Lt`, etc., so this is not an abstract concern.  Similarly, `annotated_types.Len` is a `GroupedMetadata` which unpacks itself into `MinLen` (optionally) and `MaxLen`.
 
 ### Consuming metadata
 
 We intend to not be perspcriptive as to _how_ the metadata and constraints are used, but as an example of how one might parse constraints from types annotations see our [implementation in `test_main.py`](https://github.com/annotated-types/annotated-types/blob/f59cf6d1b5255a0fe359b93896759a180bec30ae/tests/test_main.py#L94-L103).
 
 It is up to the implementer to determine how this metadata is used.
```

