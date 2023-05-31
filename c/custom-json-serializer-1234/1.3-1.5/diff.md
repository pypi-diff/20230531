# Comparing `tmp/custom-json-serializer-1234-1.3.tar.gz` & `tmp/custom-json-serializer-1234-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom-json-serializer-1234-1.3.tar", last modified: Wed May 31 11:05:26 2023, max compression
+gzip compressed data, was "custom-json-serializer-1234-1.5.tar", last modified: Wed May 31 13:37:37 2023, max compression
```

## Comparing `custom-json-serializer-1234-1.3.tar` & `custom-json-serializer-1234-1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 11:05:26.167487 custom-json-serializer-1234-1.3/
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      415 2023-05-31 11:05:26.167487 custom-json-serializer-1234-1.3/PKG-INFO
-drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 11:05:26.167487 custom-json-serializer-1234-1.3/core/
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      174 2023-05-29 14:08:22.000000 custom-json-serializer-1234-1.3/core/__init__.py
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      325 2023-05-30 22:15:14.000000 custom-json-serializer-1234-1.3/core/factory.py
-drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 11:05:26.167487 custom-json-serializer-1234-1.3/core/helpers/
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-30 22:46:44.000000 custom-json-serializer-1234-1.3/core/helpers/__init__.py
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     1665 2023-05-30 12:10:09.000000 custom-json-serializer-1234-1.3/core/helpers/constants.py
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     7436 2023-05-31 10:37:09.000000 custom-json-serializer-1234-1.3/core/helpers/functions.py
-drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 11:05:26.167487 custom-json-serializer-1234-1.3/core/serializers/
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-30 22:44:29.000000 custom-json-serializer-1234-1.3/core/serializers/__init__.py
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     2640 2023-05-30 22:50:19.000000 custom-json-serializer-1234-1.3/core/serializers/jsonserializer.py
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     2783 2023-05-30 22:50:50.000000 custom-json-serializer-1234-1.3/core/serializers/xmlserializer.py
-drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 11:05:26.167487 custom-json-serializer-1234-1.3/custom_json_serializer_1234.egg-info/
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      415 2023-05-31 11:05:26.000000 custom-json-serializer-1234-1.3/custom_json_serializer_1234.egg-info/PKG-INFO
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      470 2023-05-31 11:05:26.000000 custom-json-serializer-1234-1.3/custom_json_serializer_1234.egg-info/SOURCES.txt
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        1 2023-05-31 11:05:26.000000 custom-json-serializer-1234-1.3/custom_json_serializer_1234.egg-info/dependency_links.txt
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     1591 2023-05-31 11:05:26.000000 custom-json-serializer-1234-1.3/custom_json_serializer_1234.egg-info/requires.txt
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        5 2023-05-31 11:05:26.000000 custom-json-serializer-1234-1.3/custom_json_serializer_1234.egg-info/top_level.txt
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)       38 2023-05-31 11:05:26.167487 custom-json-serializer-1234-1.3/setup.cfg
--rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      602 2023-05-31 11:04:03.000000 custom-json-serializer-1234-1.3/setup.py
+drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 13:37:37.703445 custom-json-serializer-1234-1.5/
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      415 2023-05-31 13:37:37.703445 custom-json-serializer-1234-1.5/PKG-INFO
+drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 13:37:37.703445 custom-json-serializer-1234-1.5/core/
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      174 2023-05-29 14:08:22.000000 custom-json-serializer-1234-1.5/core/__init__.py
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      325 2023-05-30 22:15:14.000000 custom-json-serializer-1234-1.5/core/factory.py
+drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 13:37:37.703445 custom-json-serializer-1234-1.5/core/helpers/
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-30 22:46:44.000000 custom-json-serializer-1234-1.5/core/helpers/__init__.py
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     1517 2023-05-31 11:21:37.000000 custom-json-serializer-1234-1.5/core/helpers/constants.py
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     7185 2023-05-31 11:19:21.000000 custom-json-serializer-1234-1.5/core/helpers/functions.py
+drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 13:37:37.703445 custom-json-serializer-1234-1.5/core/serializers/
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-30 22:44:29.000000 custom-json-serializer-1234-1.5/core/serializers/__init__.py
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     2640 2023-05-30 22:50:19.000000 custom-json-serializer-1234-1.5/core/serializers/jsonserializer.py
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     2783 2023-05-30 22:50:50.000000 custom-json-serializer-1234-1.5/core/serializers/xmlserializer.py
+drwxrwxr-x   0 vdtepsnov  (1000) vdtepsnov  (1000)        0 2023-05-31 13:37:37.703445 custom-json-serializer-1234-1.5/custom_json_serializer_1234.egg-info/
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      415 2023-05-31 13:37:37.000000 custom-json-serializer-1234-1.5/custom_json_serializer_1234.egg-info/PKG-INFO
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      470 2023-05-31 13:37:37.000000 custom-json-serializer-1234-1.5/custom_json_serializer_1234.egg-info/SOURCES.txt
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        1 2023-05-31 13:37:37.000000 custom-json-serializer-1234-1.5/custom_json_serializer_1234.egg-info/dependency_links.txt
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)     1511 2023-05-31 13:37:37.000000 custom-json-serializer-1234-1.5/custom_json_serializer_1234.egg-info/requires.txt
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)        5 2023-05-31 13:37:37.000000 custom-json-serializer-1234-1.5/custom_json_serializer_1234.egg-info/top_level.txt
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)       38 2023-05-31 13:37:37.703445 custom-json-serializer-1234-1.5/setup.cfg
+-rw-rw-r--   0 vdtepsnov  (1000) vdtepsnov  (1000)      602 2023-05-31 13:34:19.000000 custom-json-serializer-1234-1.5/setup.py
```

### Comparing `custom-json-serializer-1234-1.3/core/helpers/constants.py` & `custom-json-serializer-1234-1.5/core/helpers/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-from types import LambdaType, FunctionType, MethodType, CodeType,\
+from types import LambdaType, FunctionType, MethodType, CodeType, \
     ModuleType, CellType, GeneratorType
-from typing import Final
 
-JSON_TYPE: str = r"<class '(\w\S+)'>_"
+JSON_TYPE = r"<class '(\w\S+)'>_"
 JSON = ('''{{
     "{type}_{id:x}": {{
     {items}
     }}
 }}''')
 
-
-XML_TYPE: str = r'type="(\w+)"'
+XML_TYPE = r'type="(\w+)"'
 XML = ('''
 <object type="{type}" id="{id:x}">
 {items}
 </object>
 ''')
 XML_ITEM = ('''
 <item>
@@ -24,21 +22,21 @@
     <value>
         {value}
     </value>
 </item>
 ''')
 XML_PRIMITIVE = '<primitive type="{type}">{obj}</primitive>'
 
-PRIMITIVE_TYPES: tuple = (int, float, complex, str, bool, type(None))
+PRIMITIVE_TYPES = (int, float, complex, str, bool, type(None))
 
-BOOL_TYPE: dict[bool, str] = {
-        None: 'none',
-        True: 'true',
-        False: 'false'
-    }
+BOOL_TYPE = {
+    None: 'none',
+    True: 'true',
+    False: 'false'
+}
 
 TYPE_MAPPING = {
     'int': int,
     'float': float,
     'complex': complex,
     'str': str,
     'bool': bool,
@@ -58,24 +56,23 @@
     'type': type,
     'module': ModuleType,
     'object': object,
     'property': property,
     'generator': GeneratorType
 }
 
-IGNORED_FIELDS: set[str] = {
-        '__weakref__',
-        '__subclasshook__',
-        '__dict__',
-        '__doc__'
+IGNORED_FIELDS = {
+    '__weakref__',
+    '__subclasshook__',
+    '__dict__',
+    '__doc__'
 }
-IGNORED_FIELD_TYPES: set[str] = {
+IGNORED_FIELD_TYPES = {
     'BuiltinFunctionType', 'BuiltinMethodType',
     'WrapperDescriptorType', 'MethodDescriptorType',
     'MappingProxyType', 'GetSetDescriptorType',
     'MemberDescriptorType'
 }
 
-TYPE: Final[str] = "type"
-ITERATOR_TYPE: Final[str] = "iterator"
-VALUE: Final[str] = "value"
-
+TYPE = "type"
+ITERATOR_TYPE = "iterator"
+VALUE = "value"
```

### Comparing `custom-json-serializer-1234-1.3/core/helpers/functions.py` & `custom-json-serializer-1234-1.5/core/helpers/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -214,20 +214,14 @@
             ...
 
         return obj
 
     elif issubclass(obj_type, ModuleType):
         return __import__(obj_data.get('name'))
 
-    # if obj_data[TYPE] == ITERATOR_TYPE:
-    #     return iter(create_object(obj_type, item) for item in obj_data[VALUE])
-
-    # elif issubclass(obj_type, type(iter)):
-    #     return iter(create_object(obj_type, item) for item in obj_data[VALUE])
-
     elif issubclass(obj_type, bytearray):
         return bytearray(obj_data)
     else:
         obj = object.__new__(obj_data.get('class'))
         obj.__dict__ = obj_data.get('attrs')
         return obj
```

### Comparing `custom-json-serializer-1234-1.3/core/serializers/jsonserializer.py` & `custom-json-serializer-1234-1.5/core/serializers/jsonserializer.py`

 * *Files identical despite different names*

### Comparing `custom-json-serializer-1234-1.3/core/serializers/xmlserializer.py` & `custom-json-serializer-1234-1.5/core/serializers/xmlserializer.py`

 * *Files identical despite different names*

### Comparing `custom-json-serializer-1234-1.3/custom_json_serializer_1234.egg-info/requires.txt` & `custom-json-serializer-1234-1.5/custom_json_serializer_1234.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 command-not-found==0.3
 container.py==0.0.0
 cryptography==3.4.8
 cupshelpers==1.0
 custom-json-serializer-1234==1.2
 dbus-python==1.2.18
 defer==1.0.6
-distro-info===1.1build1
 distro==1.7.0
 docker-compose==1.29.2
 docker==5.0.3
 dockerpty==0.4.1
 docopt==0.6.2
 docutils==0.20.1
 frozendict==2.3.8
@@ -55,17 +54,15 @@
 pyRFC3339==1.1
 pycairo==1.20.1
 pycodestyle==2.10.0
 pycups==2.0.1
 pymacaroons==0.13.0
 pyparsing==2.4.7
 pyrsistent==0.18.1
-python-apt==2.4.0+ubuntu1
 python-dateutil==2.8.1
-python-debian===0.1.43ubuntu1
 python-dotenv==0.19.2
 pytz==2022.1
 pyxdg==0.27
 readme-renderer==37.3
 regex==2023.5.5
 reportlab==3.6.8
 requests-toolbelt==1.0.0
```

### Comparing `custom-json-serializer-1234-1.3/setup.py` & `custom-json-serializer-1234-1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="custom-json-serializer-1234",
-    version="1.3",
+    version="1.5",
     description="serialization/deserialization package",
     url="https://github.com/donshester/PythonLabs/tree/lab3",
     author="Me",
     author_email="vlad.stepanov.2003@bk.ru",
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.10",
```

