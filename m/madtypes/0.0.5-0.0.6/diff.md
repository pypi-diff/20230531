# Comparing `tmp/madtypes-0.0.5.tar.gz` & `tmp/madtypes-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madtypes-0.0.5.tar", last modified: Tue May 30 13:31:24 2023, max compression
+gzip compressed data, was "madtypes-0.0.6.tar", last modified: Wed May 31 12:15:56 2023, max compression
```

## Comparing `madtypes-0.0.5.tar` & `madtypes-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:31:24.101182 madtypes-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-30 13:31:24.101182 madtypes-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-30 13:31:05.000000 madtypes-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:31:24.097182 madtypes-0.0.5/madtypes/
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-05-30 13:31:05.000000 madtypes-0.0.5/madtypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:31:24.097182 madtypes-0.0.5/madtypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-30 13:31:24.000000 madtypes-0.0.5/madtypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-30 13:31:24.000000 madtypes-0.0.5/madtypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:31:24.000000 madtypes-0.0.5/madtypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 13:31:24.000000 madtypes-0.0.5/madtypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:31:24.101182 madtypes-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-30 13:31:05.000000 madtypes-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:31:24.097182 madtypes-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-30 13:31:05.000000 madtypes-0.0.5/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:15:56.367192 madtypes-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-05-31 12:15:56.367192 madtypes-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-05-31 12:15:45.000000 madtypes-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:15:56.367192 madtypes-0.0.6/madtypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-05-31 12:15:45.000000 madtypes-0.0.6/madtypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:15:56.367192 madtypes-0.0.6/madtypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-05-31 12:15:56.000000 madtypes-0.0.6/madtypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-31 12:15:56.000000 madtypes-0.0.6/madtypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:15:56.000000 madtypes-0.0.6/madtypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 12:15:56.000000 madtypes-0.0.6/madtypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 12:15:56.367192 madtypes-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-31 12:15:45.000000 madtypes-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:15:56.367192 madtypes-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-05-31 12:15:45.000000 madtypes-0.0.6/tests/test_schema.py
```

### Comparing `madtypes-0.0.5/madtypes/__init__.py` & `madtypes-0.0.6/madtypes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import get_args, get_origin, Union, Type
+from enum import Enum
 import inspect
 import re
 
 TYPE_TO_STRING: dict[type, str] = {
     str: "string",
     int: "integer",
     list: "array",
@@ -94,15 +95,23 @@
 
     def is_valid(self, **__kwargs__) -> bool:
         """Validation at Object scope, for validation based on multiple fields."""
         return True
 
     @classmethod
     def get_fields(cls):
-        return list(cls.__annotations__.items())
+        fields = list(cls.__annotations__.items())
+
+        # Check if the class inherits from another Schema
+        for base in cls.__bases__:
+            if issubclass(base, Schema):
+                # Retrieve the fields from the parent class
+                fields.extend(base.get_fields())
+
+        return fields
 
     def __getattr__(self, name):
         if name in self:
             return self[name]
         # I don't know how to trigger the next line, it's more of an `in-case'
         return super().__getattribute__(name)  # pragma: no cover
 
@@ -113,15 +122,15 @@
             raise TypeError(f"{value} is not an instance of {annotation}")
         self[name] = value
 
     @classmethod
     def required_fields(cls) -> list[str]:
         return [
             name
-            for name, field in cls.__annotations__.items()
+            for name, field in cls.get_fields()
             if not is_optional_type(field)
         ]
 
 
 class Immutable(Schema):
     def __setattr__(self, __name__, __value__):
         raise TypeError("'Immutable' object does not support item assignment")
@@ -136,21 +145,33 @@
 ) -> dict:
     result = kwargs
     origin = get_origin(annotation)
     origin = annotation if not origin else origin
     args = get_args(annotation)
     if origin in TYPE_TO_STRING:
         result.update({"type": TYPE_TO_STRING[origin]})
-    if origin == list:
-        result.update({"items": json_schema(args[0])})
+    if origin == list or origin == set:
+        result.update({"type": "array", "items": json_schema(args[0])})
+    if origin == set:
+        result.update({"uniqueItems": True})
     if origin == tuple:
         result.update({"items": [json_schema(arg) for arg in args]})
     if isinstance(origin, str):
         raise SyntaxError("A typing annotation has been written as Literal")
     if inspect.isclass(origin):
+        if issubclass(origin, Enum):
+            first_enum_member = next(iter(origin))
+            enum_type = TYPE_TO_STRING[type(first_enum_member.value)]
+            result.update(
+                {
+                    "type": enum_type,
+                    "enum": [enu.value for enu in iter(origin)],
+                }
+            )
+
         if issubclass(origin, Schema):
             result.update(
                 {
                     "type": "object",
                     "properties": {
                         name: json_schema(field)
                         for name, field in origin.get_fields()
```

### Comparing `madtypes-0.0.5/setup.py` & `madtypes-0.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="madtypes",
-    version="0.0.5",
+    version="0.0.6",
     author="6r17",
     author_email="patrick.borowy@proton.me",
     description="Python typing that raise TypeError at runtime",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/6r17/madtypes",
     packages=find_packages(include=["madtypes"]),
     keywords=["typing", "json", "json-schema"],
-    python_requires=">=3.9",
+    python_requires=">=3.10",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
 )
```

### Comparing `madtypes-0.0.5/tests/test_schema.py` & `madtypes-0.0.6/tests/test_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from enum import Enum
 from typing import Optional
 from madtypes import json_schema, Schema, Annotation, Immutable, type_check
 import pytest
 import json
 
 
 class Gender(Schema):
@@ -570,7 +571,90 @@
                 "pattern": "^\\d{3}-\\d{3}-\\d{4}$",
                 "description": "A phone number in the format XXX-XXX-XXXX",
                 "type": "string",
             }
         },
         "required": ["phone"],
     }
+
+
+def test_multiple_inheritance_json_schema():
+    class Foo(Schema):
+        foo: str
+
+    class Bar(Schema):
+        bar: str
+
+    class FooBar(Foo, Bar):
+        pass
+
+    assert len(FooBar.get_fields()) == 2
+    schema = json_schema(FooBar)
+    print(schema)
+    assert schema == {
+        "type": "object",
+        "properties": {"foo": {"type": "string"}, "bar": {"type": "string"}},
+        "required": ["foo", "bar"],
+    }
+
+
+def test_list_json_schema():
+    class Foo(Schema):
+        my_set: list[int]
+
+    schema = json_schema(Foo)
+    print(schema)
+    assert schema == {
+        "type": "object",
+        "properties": {
+            "my_set": {
+                "type": "array",
+                "items": {"type": "integer"},
+            }
+        },
+        "required": ["my_set"],
+    }
+
+
+def test_set_json_schema():
+    class Foo(Schema):
+        my_set: set[int]
+
+    schema = json_schema(Foo)
+    print(json.dumps(schema, indent=4))
+    assert schema == {
+        "type": "object",
+        "properties": {
+            "my_set": {
+                "type": "array",
+                "items": {"type": "integer"},
+                "uniqueItems": True,
+            }
+        },
+        "required": ["my_set"],
+    }
+    with pytest.raises(TypeError):
+        Foo(my_set=[1, 2, 3])
+    Foo(my_set={1, 2, 3})
+
+
+def test_enum():
+    class SomeEnum(Enum):
+        FOO = "Foo"
+        BAR = "Bar"
+        BAZ = "Baz"
+
+    class Item(Schema):
+        key: SomeEnum
+
+    schema = json_schema(Item)
+    print(schema)
+    assert schema == {
+        "type": "object",
+        "properties": {
+            "key": {"type": "string", "enum": ["Foo", "Bar", "Baz"]}
+        },
+        "required": ["key"],
+    }
+    Item(key=SomeEnum.FOO)
+    with pytest.raises(TypeError):
+        Item(key="Foo")
```

