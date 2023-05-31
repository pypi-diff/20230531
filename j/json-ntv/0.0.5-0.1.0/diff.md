# Comparing `tmp/json_ntv-0.0.5.tar.gz` & `tmp/json_ntv-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_ntv-0.0.5.tar", last modified: Thu Apr  6 07:47:46 2023, max compression
+gzip compressed data, was "json_ntv-0.1.0.tar", last modified: Wed May 31 14:38:36 2023, max compression
```

## Comparing `json_ntv-0.0.5.tar` & `json_ntv-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 07:47:46.624723 json_ntv-0.0.5/
--rw-rw-rw-   0        0        0     4785 2023-04-06 07:47:46.624723 json_ntv-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4157 2023-04-03 22:02:10.000000 json_ntv-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 07:47:46.604310 json_ntv-0.0.5/json_ntv/
--rw-rw-rw-   0        0        0     3874 2023-04-03 13:54:52.000000 json_ntv-0.0.5/json_ntv/__init__.py
--rw-rw-rw-   0        0        0    20211 2023-04-05 14:57:12.000000 json_ntv-0.0.5/json_ntv/namespace.py
--rw-rw-rw-   0        0        0    30330 2023-04-05 14:57:12.000000 json_ntv-0.0.5/json_ntv/ntv.py
--rw-rw-rw-   0        0        0     5098 2023-04-02 20:40:09.000000 json_ntv-0.0.5/json_ntv/ntv_connector.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:47:46.621736 json_ntv-0.0.5/json_ntv.egg-info/
--rw-rw-rw-   0        0        0     4785 2023-04-06 07:47:46.000000 json_ntv-0.0.5/json_ntv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-04-06 07:47:46.000000 json_ntv-0.0.5/json_ntv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 07:47:46.000000 json_ntv-0.0.5/json_ntv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-06 07:47:46.000000 json_ntv-0.0.5/json_ntv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-06 07:47:46.000000 json_ntv-0.0.5/json_ntv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-04-06 07:47:46.633685 json_ntv-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1137 2023-04-06 07:47:07.000000 json_ntv-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:47:46.623727 json_ntv-0.0.5/tests/
--rw-rw-rw-   0        0        0     2959 2023-04-04 12:21:26.000000 json_ntv-0.0.5/tests/tests_namespace.py
--rw-rw-rw-   0        0        0    14252 2023-04-06 07:32:08.000000 json_ntv-0.0.5/tests/tests_ntv.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:38:36.217201 json_ntv-0.1.0/
+-rw-rw-rw-   0        0        0     4765 2023-05-31 14:38:36.217698 json_ntv-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4137 2023-05-08 21:25:08.000000 json_ntv-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 14:38:36.150567 json_ntv-0.1.0/json_ntv/
+-rw-rw-rw-   0        0        0     4138 2023-05-31 09:23:04.000000 json_ntv-0.1.0/json_ntv/__init__.py
+-rw-rw-rw-   0        0        0     2770 2023-05-24 21:47:42.000000 json_ntv-0.1.0/json_ntv/json_mermaid.py
+-rw-rw-rw-   0        0        0    20675 2023-05-11 13:01:46.000000 json_ntv-0.1.0/json_ntv/namespace.py
+-rw-rw-rw-   0        0        0    39554 2023-05-31 14:30:06.000000 json_ntv-0.1.0/json_ntv/ntv.py
+-rw-rw-rw-   0        0        0     9958 2023-05-31 09:23:04.000000 json_ntv-0.1.0/json_ntv/ntv_connector.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:38:36.177632 json_ntv-0.1.0/json_ntv.egg-info/
+-rw-rw-rw-   0        0        0     4765 2023-05-31 14:38:36.000000 json_ntv-0.1.0/json_ntv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-05-31 14:38:36.000000 json_ntv-0.1.0/json_ntv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 14:38:36.000000 json_ntv-0.1.0/json_ntv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-31 14:38:36.000000 json_ntv-0.1.0/json_ntv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-31 14:38:36.000000 json_ntv-0.1.0/json_ntv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-31 14:38:36.222806 json_ntv-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1137 2023-05-31 14:36:39.000000 json_ntv-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 14:38:36.214711 json_ntv-0.1.0/tests/
+-rw-rw-rw-   0        0        0     3989 2023-05-01 21:49:44.000000 json_ntv-0.1.0/tests/test_mongo.py
+-rw-rw-rw-   0        0        0     1265 2023-04-25 21:48:53.000000 json_ntv-0.1.0/tests/test_ntvstruct.py
+-rw-rw-rw-   0        0        0     3077 2023-05-01 21:49:44.000000 json_ntv-0.1.0/tests/tests_namespace.py
+-rw-rw-rw-   0        0        0    17085 2023-05-31 14:30:06.000000 json_ntv-0.1.0/tests/tests_ntv.py
```

### Comparing `json_ntv-0.0.5/PKG-INFO` & `json_ntv-0.1.0/json_ntv.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: json_ntv
-Version: 0.0.5
+Name: json-ntv
+Version: 0.1.0
 Summary: JSON-NTV a semantic format for interoperability
 Home-page: https://github.com/loco-philippe/NTV/blob/main/README.md
 Author: Philippe Thomy
 Author-email: philippe@loco-labs.io
 Keywords: JSON-NTV,semantic JSON,development,environmental data
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -36,30 +36,30 @@
 The constructed entities (called NTV for *named typed value*) are therefore a triplet with one mandatory element (the value in JSON format) and two optional elements (name, type).
 >
 > *For example, the location of Paris can be represented by:*
 > - *a name: "Paris",*
 > - *a type: the coordinates of a point according to the GeoJSON format,*
 > - *a value: [ 2.3522, 48.8566]*
 
-The easiest way to add this information is to use a JSON-object with a single member using the syntax [JSON-ND](https://github.com/glenkleidon/JSON-ND) for the first term of the member and the JSON-value for the second term of the member.
+The easiest way to add this information into a JSON-value is to use a JSON-object with a single member using the syntax [JSON-ND](https://github.com/glenkleidon/JSON-ND) for the first term of the member and the JSON-value for the second term of the member.
 >
 > *For the example above, the JSON representation is:*    
 > *```{ "paris:point" : [2.3522, 48.8566] }```*
 
-With this approach, three NTV entities are defined:
+With this approach, two NTV entities are defined:
 - a primitive entity which is not composed of any other entity (NTV-single),
-- two structured entities: an unordered collection of NTV entities (NTV-set) and an ordered sequence of NTV entities (NTV-list).
+- a structured entity which is an ordered sequence of NTV entities (Ntv-list).
       
 as well as two JSON formats:
 - simple format when the name and the type are not present (this is the usual case of CSV data),
 - named format when the name or type is present (see example above for an NTV-single entity and below for a structured entity).
 >
 > *Example of an entity composed of two other entities:*
-> - *```{ "cities::point": [[2.3522, 48.8566], [4.8357, 45.7640]] }``` for an NTV-list entity*
-> - *```{ "cities::point": { "paris":[2.3522, 48.8566], "lyon":[4.8357, 45.7640] } }``` for an NTV-set entity*
+> - *```{ "cities::point": [[2.3522, 48.8566], [4.8357, 45.7640]] }``` for an unnamed NTV-list entity*
+> - *```{ "cities::point": { "paris":[2.3522, 48.8566], "lyon":[4.8357, 45.7640] } }``` for a named NTV-list entity*
 >
 > *Note: This syntax can also be used for CSV file headers*
 
 The type incorporates a notion of `namespaces` that can be nested.
 > *For example, the type: "ns1.ns2.type" means that:*
 > - *ns1. is a namespace defined in the global namespace,*
 > - *ns2. is a namespace defined in the ns1 namespace.,*
```

### Comparing `json_ntv-0.0.5/README.md` & `json_ntv-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 The constructed entities (called NTV for *named typed value*) are therefore a triplet with one mandatory element (the value in JSON format) and two optional elements (name, type).
 >
 > *For example, the location of Paris can be represented by:*
 > - *a name: "Paris",*
 > - *a type: the coordinates of a point according to the GeoJSON format,*
 > - *a value: [ 2.3522, 48.8566]*
 
-The easiest way to add this information is to use a JSON-object with a single member using the syntax [JSON-ND](https://github.com/glenkleidon/JSON-ND) for the first term of the member and the JSON-value for the second term of the member.
+The easiest way to add this information into a JSON-value is to use a JSON-object with a single member using the syntax [JSON-ND](https://github.com/glenkleidon/JSON-ND) for the first term of the member and the JSON-value for the second term of the member.
 >
 > *For the example above, the JSON representation is:*    
 > *```{ "paris:point" : [2.3522, 48.8566] }```*
 
-With this approach, three NTV entities are defined:
+With this approach, two NTV entities are defined:
 - a primitive entity which is not composed of any other entity (NTV-single),
-- two structured entities: an unordered collection of NTV entities (NTV-set) and an ordered sequence of NTV entities (NTV-list).
+- a structured entity which is an ordered sequence of NTV entities (Ntv-list).
       
 as well as two JSON formats:
 - simple format when the name and the type are not present (this is the usual case of CSV data),
 - named format when the name or type is present (see example above for an NTV-single entity and below for a structured entity).
 >
 > *Example of an entity composed of two other entities:*
-> - *```{ "cities::point": [[2.3522, 48.8566], [4.8357, 45.7640]] }``` for an NTV-list entity*
-> - *```{ "cities::point": { "paris":[2.3522, 48.8566], "lyon":[4.8357, 45.7640] } }``` for an NTV-set entity*
+> - *```{ "cities::point": [[2.3522, 48.8566], [4.8357, 45.7640]] }``` for an unnamed NTV-list entity*
+> - *```{ "cities::point": { "paris":[2.3522, 48.8566], "lyon":[4.8357, 45.7640] } }``` for a named NTV-list entity*
 >
 > *Note: This syntax can also be used for CSV file headers*
 
 The type incorporates a notion of `namespaces` that can be nested.
 > *For example, the type: "ns1.ns2.type" means that:*
 > - *ns1. is a namespace defined in the global namespace,*
 > - *ns2. is a namespace defined in the ns1 namespace.,*
```

### Comparing `json_ntv-0.0.5/json_ntv/__init__.py` & `json_ntv-0.1.0/json_ntv/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,24 +14,29 @@
     - `NTV.json_ntv.namespace.NtvType`
             
          
 - `NTV.json_ntv.ntv` :
 
     - `NTV.json_ntv.ntv.NtvSingle`
     - `NTV.json_ntv.ntv.NtvList`
-    - `NTV.json_ntv.ntv.NtvSet`
+    - `NTV.json_ntv.ntv.NtvTree`
     - `NTV.json_ntv.ntv.Ntv` (abstract class)
     - `NTV.json_ntv.ntv.NtvConnector` (abstract class)    
           
           
 - `NTV.json_ntv.ntv_connector` :
     
     - `NTV.json_ntv.ntv_connector.DataFrameConnec`
     - `NTV.json_ntv.ntv_connector.SeriesConnec`
-    
+    - `NTV.json_ntv.ntv_connector.IlistConnec`
+    - `NTV.json_ntv.ntv_connector.IindexConnec`
+     
+The functions to convert a json object to Mermaid code are in the 
+`NTV.json_ntv.json_mermaid` submodule.    
+       
 # 0 - Abstract
 
 Today, the semantic level of shared data remains low. It is very often limited 
 to the type of data defined in the exchange formats (strings for CSV formats; 
 numbers, strings, arrays and objects for JSON formats).
 
 The proposed consists of adding a type and a name to the data exchanged (see also the 
@@ -85,10 +90,11 @@
 This structuring of type makes it possible to reference any type of data that has
  a JSON representation and to consolidate all the shared data structures within the
  same tree of types.
 
 
 """
 from json_ntv.namespace import Namespace, NtvType, str_type, relative_type, agreg_type
-from json_ntv.ntv import Ntv, NtvSingle, NtvList, NtvSet, NtvConnector, NtvError
+from json_ntv.ntv import Ntv, NtvSingle, NtvList, NtvConnector, NtvError, NtvTree
 from json_ntv.ntv_connector import DataFrameConnec, SeriesConnec, from_csv, to_csv
+from json_ntv.json_mermaid import diagram
 #print('package :', __package__)
```

### Comparing `json_ntv-0.0.5/json_ntv/namespace.py` & `json_ntv-0.1.0/json_ntv/namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,37 +321,47 @@
     def __init__(self, name, nspace=None):
         '''NtvType constructor.
 
         *Parameters*
 
         - **name** : string - name of the Type
         - **nspace** : Namespace (default None) - namespace associated'''
+        if isinstance(name, NtvType):
+            self.name = name.name
+            self.nspace = name.nspace
+            self.custom = name.custom
+            return
         if not name or not isinstance(name, str):
             raise NtvTypeError('null name is not allowed')
         if not name and not nspace:
             name = 'json'
         if not nspace:
             nspace = Namespace._namespaces_['']
         if name[0] != '$' and not nspace.custom and not name in nspace.content['type']:
             raise NtvTypeError(name + ' is not defined in ' + nspace.long_name)
         self.name = name
         self.nspace = nspace
         self.custom = nspace.custom or name[0] == '$'
         self._types_[self.long_name] = self
+        return
 
     def __eq__(self, other):
         ''' equal if name and nspace are equal'''
         if self is None and other is None:
             return True
         if self is None or other is None:
             return False
-        if self.__class__ != other.__class__:
+        if self.__class__.__name__ != other.__class__.__name__:
             return False
         return self.name == other.name and self.nspace == other.nspace
 
+    def __hash__(self):
+        '''return hash(name) + hash(nspace)'''
+        return hash(self.name) + hash(self.nspace)
+
     def __str__(self):
         '''return string format'''
         return self.long_name
 
     def __repr__(self):
         '''return classname and long name'''
         return self.__class__.__name__ + '(' + self.long_name + ')'
@@ -386,15 +396,14 @@
     The methods defined in this class are :
 
     *classmethods*
     - `namespaces`
     - `add`
 
     *dynamic values (@property)*
-    - `file`
     - `long_name`
     - `content`
 
     *instance methods*
     - `is_child`
     - `is_parent`
     '''
@@ -447,18 +456,22 @@
 
     def __eq__(self, other):
         ''' equal if name and parent are equal'''
         if self is None and other is None:
             return True
         if self is None or other is None:
             return False
-        if self.__class__ != other.__class__:
+        if self.__class__.__name__ != other.__class__.__name__:
             return False
         return self.name == other.name and self.parent == other.parent
 
+    def __hash__(self):
+        '''return hash(name) + hash(parent)'''
+        return hash(self.name) + hash(self.parent)
+
     def __str__(self):
         '''return string format'''
         return self.long_name
 
     def __repr__(self):
         '''return classname and long name'''
         return self.__class__.__name__ + '(' + self.long_name + ')'
```

### Comparing `json_ntv-0.0.5/json_ntv/ntv.py` & `json_ntv-0.1.0/json_ntv/ntv.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,108 +3,122 @@
 Created on Feb 27 2023
 
 @author: Philippe@loco-labs.io
 
 The `ntv` module is part of the `NTV.json_ntv` package ([specification document](
 https://github.com/loco-philippe/NTV/blob/main/documentation/JSON-NTV-standard.pdf)).
 
-It contains the classes `NtvSingle`, `NtvSet`, `NtvList`, `Ntv`(abstract),
-`NtvConnector` and `NtvError` for NTV entities.
+It contains the classes `NtvSingle`, `NtvList`, `Ntv`(abstract),
+`NtvConnector`, `NtvTree` and `NtvError` for NTV entities.
 
 # 1 - JSON-NTV structure
 
 The NTV triplet (name, type, value) is represented using a JSON-NTV format inspired
 by the RFC [JSON-ND](https://github.com/glenkleidon/JSON-ND) project :
 - **```value```** (if name and type are not documented)
 - **```{ "name" : value }```** (if name is documented but not type)
 - **```{ ":type" : value }```** for primitive entities and **```{ "::type" : value }```**
  for structured entities (if type is documented but not name)
 - **```{ "name:type" : value }```** for primitive entities and **```{
  "name::type" : value }```** for structured entities (if type and name are documented).
 
 For an NTV-single, the value is the JSON-value of the entity.
-For an NTV-list, value is a JSON-array where JSON-elements are the JSON-NTV formats
- of included NTV entities.
-For an NTV-set, value is a JSON-object where JSON-members are the JSON-members of
-the JSON-NTV formats of included NTV entities.
+For an NTV-list, value is a JSON-array (JSON-object) where JSON-elements (JSON-members)
+are the JSON-NTV formats of included NTV entities.
 
 This JSON-NTV format allows full compatibility with existing JSON structures:
 - a JSON-number, JSON-string or JSON-boolean is the representation of an NTV-single entity,
 - a JSON-object with a single member is the representation of an NTV-single entity
-- a JSON-array is the representation of an NTV-list entity
-- a JSON-object without a single member is the representation of an NTV-set entity
+- a JSON-array or JSON-object is the representation of an NTV-list entity
 
 # 2 - Examples of JSON-NTV representations
 - NTV-single, simple format :
    - ```"lyon"```
    - ```52.5```
 - NTV-single, named format :
    - ```{ "paris:point" : [2.3522, 48.8566] }```
    - ```{ ":point" : [4.8357, 45.7640] }```
    - ```{ "city" : "paris" }```
-- NTV-list, simple format :
+- NTV-list, simple format (whithout names):
    - ```[ [2.3522, 48.8566], {"lyon" : [4.8357, 45.7640]} ]```
    - ```[ { ":point" : [2.3522, 48.8566]}, {":point" : [4.8357, 45.7640]} ]```
    - ```[ 4, 45 ]```
    - ```[ "paris" ]```
    - ```[ ]```
-- NTV-list, named format :
+- NTV-list, named format (whithout names):
    - ```{ "cities::point" : [ [2.3522, 48.8566], [4.8357, 45.7640] ] }```
    - ```{ "::point" : [ [2.3522, 48.8566], {"lyon" : [4.8357, 45.7640]} ] }```
    - ```{ "simple list" : [ 4, 45.7 ] }```
    - ```{ "generic date::dat" : [ "2022-01-28T18-23-54Z", "2022-01-28", 1234.78 ] }```
-- NTV-set, simple format :
+- NTV-list, simple format (with names):
    - ```{ "nom”: "white", "prenom": "walter", "surnom": "heisenberg" }```
    - ```{ "paris:point" : [2.3522, 48.8566] , "lyon" : "france" }```
    - ```{ "paris" : [2.3522, 48.8566], "" : [4.8357, 45.7640] }```
    - ```{ }```
-- NTV-set, named format :
+- NTV-list, named format (with names):
    - ```{ "cities::point": { "paris": [2.352, 48.856], "lyon": [4.835, 45.764]}}```
    - ```{ "cities" :     { "paris:point" : [2.3522, 48.8566] , "lyon" : "france"} }```
    - ```{ "city" : { "paris" : [2.3522, 48.8566] } }```
 
 """
 from abc import ABC
 import datetime
 import json
 from json import JSONDecodeError
+from base64 import b64encode
 
 import cbor2
 from shapely import geometry
-from observation import Ilist
+#from observation import Ilist
+from IPython.display import Image, display
 
 from json_ntv.namespace import NtvType, Namespace, str_type, relative_type, agreg_type
 
 
 class Ntv(ABC):
     ''' The Ntv class is an abstract class used for all NTV entities.
 
     *Attributes :*
 
     - **ntv_name** : String - name of the NTV entity
     - **ntv_type**: NtvType - type of the entity
     - **ntv_value**:  value of the entity
+    - **parent**:  parent NtvList entity
+    - **_row**:  row in the parent NtvList
 
     *dynamic values (@property)*
+    - `address`
+    - `address_name`
+    - `json_array`
     - `type_str`
     - `code_ntv`
+    - `max_len`
+    - `val`
 
     The methods defined in this class are :
 
-    *Ntv constructor*
-    - `obj` *(classmethod)*
-    - `from_obj` *(staticmethod)*
-    - `from_att` *(staticmethod)*
+    *Ntv constructor (staticmethod)*
+    - `obj`
+    - `from_obj`
+    - `from_att`
 
     *instance methods*
+    - `alike`
+    - `from_value`
+    - `json_name`
     - `set_name`
     - `set_type`
     - `set_value`
     - `to_obj`
     - `to_repr`
+    - `to_mermaid`
+    - `to_tuple`
+
+    *utility methods*
+    - `from_obj_name` *(staticmethod)*
     '''
 
     def __init__(self, ntv_value, ntv_name, ntv_type):
         '''Ntv constructor.
 
         *Parameters*
 
@@ -120,192 +134,334 @@
             self.ntv_type = Namespace.add(ntv_type)
         else:
             self.ntv_type = None
         if not isinstance(ntv_name, str):
             ntv_name = ''
         self.ntv_name = ntv_name
         self.ntv_value = ntv_value
+        self.parent = None
+        self._row = None
 
-    @classmethod
-    def obj(cls, data):
+    @staticmethod
+    def obj(data, no_typ=False, decode_str=False):
         ''' return an Ntv entity from data.
-        Data can be :
+        **Data** can be :
         - a tuple with value, name, typ and cat (see `from_att` method)
-        - a value to decode (see `from_obj`method)'''
+        - a value to decode (see `from_obj`method)
+        - **no_typ** : boolean (default None) - if True, NtvList is with 'json' type
+        - **decode_str**: boolean (default False) - if True, string are loaded in json data'''
         if isinstance(data, tuple):
-            return cls.from_att(*data)
-        return cls.from_obj(data)
+            return Ntv.from_att(*data, decode_str=decode_str)
+        return Ntv.from_obj(data, no_typ=no_typ, decode_str=decode_str)
 
     @staticmethod
-    def from_att(value, name, typ, cat):
+    def from_att(value, name, typ, cat, decode_str=False):
         ''' return an Ntv entity.
 
         *Parameters*
 
         - **value**: Ntv entity or value to convert in an Ntv entity
         - **name** : string - name of the Ntv entity
         - **typ** : string or NtvType - type of the NTV entity
-        - **cat**: string - NTV category ('single', 'list' or 'set')'''
-        value = Ntv._from_value(value)
-        if value.__class__.__name__ in ['NtvSingle', 'NtvList', 'NtvSet']:
+        - **cat**: string - NTV category ('single', 'list')
+        - **decode_str**: boolean (default False) - if True, string are loaded in json data'''
+        value = Ntv._from_value(value, decode_str)
+        if value.__class__.__name__ in ['NtvSingle', 'NtvList']:
             return value
         if isinstance(value, list) and cat == 'list':
             return NtvList(value, name, typ)
-        if isinstance(value, list) and cat == 'set':
-            return NtvSet(value, name, typ)
         if cat == 'single':
             return NtvSingle(value, name, typ)
         return Ntv.from_obj(value, def_type=typ)
-    
+
     @staticmethod
-    def from_obj(value, def_type=None, def_sep=None):
+    def from_obj(value, def_type=None, def_sep=None, no_typ=False, decode_str=False):
         ''' return an Ntv entity from an object value.
 
         *Parameters*
 
         - **value**: Ntv value to convert in an Ntv entity
-        - **def_type** : NtvType or Namespace (default None) - default type of the NTV entity
-        - **def_sep**: ':', '::' or None (default None) - default separator of the Ntv entity'''
-        value = Ntv._from_value(value)
-        if value.__class__.__name__ in ['NtvSingle', 'NtvList', 'NtvSet']:
+        - **no_typ** : boolean (default None) - if True, NtvList is with 'json' type
+        - **def_type** : NtvType or Namespace (default None) - default type of the value
+        - **def_sep**: ':', '::' or None (default None) - default separator of the value
+        - **decode_str**: boolean (default False) - if True, string are loaded in json data'''
+        value = Ntv._from_value(value, decode_str)
+        if value.__class__.__name__ in ['NtvSingle', 'NtvList']:
             return value
         ntv_name, str_typ, ntv_value, sep = Ntv._decode(value)
-        if not sep:
-            sep = def_sep
+        sep = def_sep if not sep else sep
         if isinstance(ntv_value, list) and sep in (None, '::'):
             def_type = agreg_type(str_typ, def_type, False)
-            if sep and not def_type:
-                sep = None
-            if sep:
-                sep = ':'
+            sep = None if sep and not def_type else sep
+            sep = ':' if sep else sep
             ntv_list = [Ntv.from_obj(val, def_type, sep) for val in ntv_value]
             if not def_type and ntv_list:
                 def_type = ntv_list[0].ntv_type
+            def_type = 'json' if no_typ else def_type
             return NtvList(ntv_list, ntv_name, def_type)
-        if sep == ':':
+        if sep == ':' or (sep is None and isinstance(ntv_value, dict) and
+                          len(ntv_value) == 1):
             ntv_type = agreg_type(str_typ, def_type, False)
-            return NtvSingle(ntv_value, ntv_name, ntv_type,)
+            return NtvSingle(ntv_value, ntv_name, ntv_type)
         if sep is None and not isinstance(ntv_value, dict):
             is_json = isinstance(value, (int, str, float, bool))
             ntv_type = agreg_type(str_typ, def_type, is_json)
             return NtvSingle(ntv_value, ntv_name, ntv_type)
         if isinstance(ntv_value, dict) and (sep == '::' or len(ntv_value) != 1 and
                                             sep is None):
             keys = list(ntv_value.keys())
             values = list(ntv_value.values())
             def_type = agreg_type(str_typ, def_type, False)
-            if sep and not def_type:
-                sep = None
-            if sep:
-                sep = ':'
+            sep = None if sep and not def_type else sep
+            sep = ':' if sep else sep
             ntv_list = [Ntv.from_obj({key: val}, def_type, sep)
                         for key, val in zip(keys, values)]
             if not def_type and ntv_list:
                 def_type = ntv_list[0].ntv_type
-            return NtvSet(ntv_list, ntv_name, def_type,)
+            def_type = 'json' if no_typ else def_type
+            return NtvList(ntv_list, ntv_name, def_type)
         raise NtvError('separator ":" is not compatible with value')
 
-    @staticmethod
-    def _from_value(value):
-        '''return a decoded value'''
-        if isinstance(value, str) and value.lstrip() and value.lstrip()[0] in '"-{[0123456789':
-            try:
-                value = json.loads(value)
-            except JSONDecodeError:
-                pass
-        string = isinstance(value, str)
-        if value is None or (string and value == 'null'):
-            return NtvSingle(None)
-        if string and value == 'true':
-            return NtvSingle(True)
-        if string and value == 'false':
-            return NtvSingle(False)
-        return value
-
     def __len__(self):
         ''' len of ntv_value'''
-        if isinstance(self.ntv_value, (list, set)):
+        if isinstance(self.ntv_value, list):
             return len(self.ntv_value)
         return 1
 
     def __str__(self):
         '''return string format'''
         return self.to_obj(encoded=True)
 
     def __repr__(self):
         '''return classname and code'''
         return json.dumps(self.to_repr(False, False, False, 10))
 
     def __contains__(self, item):
         ''' item of Ntv entities'''
-        return item in self.ntv_value
-
-    def __getitem__(self, ind):
-        ''' return ntv_value item (value conversion)'''
-        if isinstance(ind, tuple):
-            return [self.ntv_value[i] for i in ind]
-        return self.ntv_value[ind]
+        if isinstance(self.val, list):
+            return item in self.ntv_value
+        return item == self.ntv_value
+
+    def __iter__(self):
+        ''' iterator for Ntv entities'''
+        if isinstance(self, NtvSingle):
+            return iter([self.val])
+        return iter(self.val)
+
+    def __getitem__(self, selector):
+        ''' return ntv_value item '''
+        if isinstance(self, NtvSingle) and selector == 0:
+            return self.ntv_value
+        if isinstance(self, NtvSingle) and selector != 0:
+            raise NtvError('item not present')
+        if isinstance(selector, tuple):
+            return [self.ntv_value[i] for i in selector]
+        if isinstance(selector, str) and isinstance(self, NtvList):
+            ind = [ntv.ntv_name for ntv in self.ntv_value].index(selector)
+            return self.ntv_value[ind]
+        return self.ntv_value[selector]
 
     def __setitem__(self, ind, value):
         ''' modify ntv_value item'''
         if ind < 0 or ind >= len(self):
             raise NtvError("out of bounds")
         self.ntv_value[ind] = value
 
     def __delitem__(self, ind):
         '''remove a ntv_value item'''
         self.ntv_value.pop(ind)
 
+    def __lt__(self, other):
+        ''' return a comparison between hash value'''
+        return hash(self) < hash(other)
+
     @property
-    def type_str(self):
-        '''return a string with the value of the NtvType of the entity'''
-        if not self.ntv_type:
-            return None
-        return self.ntv_type.long_name
+    def address(self):
+        '''return a list of parent row from root'''
+        if not self.parent:
+            return [0]
+        return self.parent.address + [self._row]
+
+    @property
+    def address_name(self):
+        '''return a string of address'''
+        name = ''
+        for ind in self.address:
+            name += str(ind) + '.'
+        return name[:-1]
 
     @property
     def code_ntv(self):
         '''return a string with the NTV code composed with :
-        - 'l' (for NtvList), 's' (for NtvSet) or 'v' (for NtvSingle)
+        - 'l' (for NtvList) or 's' (for NtvSingle)
         - 'N' if ntv_name is present
         - 'T' if ntv_type is present'''
-        dic = {'NtvList': 'l', 'NtvSet': 's', 'NtvSingle': 'v'}
+        dic = {'NtvList': 'l', 'NtvSingle': 's'}
         code = dic[self.__class__.__name__]
         if self.ntv_name:
             code += 'N'
         if self.ntv_type and self.ntv_type.long_name != 'json':
             code += 'T'
         return code
 
+    @property
+    def max_len(self):
+        '''return the highest len of Ntv entity included'''
+        maxi = len(self)
+        if isinstance(self.ntv_value, (list, set)):
+            maxi = max(maxi, max(ntv.max_len for ntv in self.ntv_value))
+        return maxi
+
+    @property
+    def name(self):
+        '''return the ntv_name of the entity'''
+        return self.ntv_name
+
+    @property
+    def type_str(self):
+        '''return a string with the value of the NtvType of the entity'''
+        if not self.ntv_type:
+            return None
+        return self.ntv_type.long_name
+
+    @property
+    def val(self):
+        '''return the ntv_value of the entity'''
+        return self.ntv_value
+
+    @staticmethod
+    def from_obj_name(string):
+        '''return a tuple with name, type and separator from string'''
+        if not isinstance(string, str):
+            raise NtvError('a json-name have to be str')
+        if string == '':
+            return (None, None, None)
+        sep = None
+        if '::' in string:
+            sep = '::'
+        elif ':' in string:
+            sep = ':'
+        if sep is None:
+            return (string, None, None)
+        split = string.rsplit(sep, 2)
+        if len(split) == 1:
+            return (string, None, sep)
+        if split[0] == '':
+            return (None, split[1], sep)
+        if split[1] == '':
+            return (split[0], None, sep)
+        return (split[0], split[1], sep)
+
+    def alike(self, ntv_value):
+        ''' return a Ntv entity with same name and type.
+
+        *Parameters*
+
+        - **ntv_value**: list of ntv values'''
+        return self.__class__(ntv_value, self.ntv_name, self.ntv_type)
+
+    def from_value(self):
+        '''return a Ntv entity from ntv_value'''
+        if isinstance(self.ntv_value, list):
+            return NtvList(self.ntv_value)
+        return Ntv.obj(self.ntv_value)
+
+    def json_name(self, def_type=None, string=False, explicit=False):
+        '''return the JSON name of the NTV entity (json-ntv format)
+
+        *Parameters*
+
+        - **def_typ** : NtvType or Namespace (default None) - type of the parent entity
+        - **string** : boolean (default False) - If True, return a string else a tuple
+        - **explicit** : boolean (default False) - If True, type is always included'''
+        if def_type is None:
+            def_type = ''
+        elif isinstance(def_type, (NtvType, Namespace)):
+            def_type = def_type.long_name
+        json_name = ''
+        if self.ntv_name:
+            json_name = self.ntv_name
+        json_type = ''
+        if self.ntv_type:
+            json_type = relative_type(def_type, self.ntv_type.long_name)
+        if json_type == 'json' and (not def_type or def_type == 'json') and not explicit:
+            json_type = ''
+        json_sep = self._obj_sep(json_type, def_type)
+        if string:
+            return json_name + json_sep + json_type
+        return [json_name, json_sep, json_type]
+
     def set_name(self, name):
         '''set a new name to the entity'''
         if name and not isinstance(name, str):
             raise NtvError('the name is not a string')
         if not name:
             name = ''
         self.ntv_name = name
 
     def set_type(self, typ=None):
-        '''set a new type to the entity (available only for NtvSingle)'''
+        '''set a new type to the entity (default None)'''
         if typ and not isinstance(typ, (str, NtvType, Namespace)):
             raise NtvError('the type is not a valid type')
-        if self.__class__.__name__ != 'NtvSingle':
-            raise NtvError('set_type is available only for NtvSingle class')
+        # if self.__class__.__name__ != 'NtvSingle':
+        #    raise NtvError('set_type is available only for NtvSingle class')
         self.ntv_type = str_type(typ, True)
 
+    def set_value(self, value):
+        '''set new ntv_value of 'Ntv Single' entities included
+
+        *Parameters*
+
+        - **value**: list / NtvList or value / NtvSingle'''
+        if isinstance(self, NtvSingle):
+            self.ntv_value = value.val if isinstance(
+                value, NtvSingle) else value
+        for val, ntv in zip(Ntv.obj(value), NtvTree(self).leaf_nodes):
+            ntv.ntv_value = val.val
+
+    def to_mermaid(self, title='', disp=False, row=False, leaves=False):
+        '''return a mermaid flowchart.
+
+        *Parameters*
+
+        - **title**: String (default '') - title of the flowchart
+        - **disp**: Boolean (default False) - if true, return a display else return
+        - **row**: Boolean (default False) - if True, add the node row
+        - **leaves**: Boolean (default False) - if True, add the leaf row
+        a mermaid text diagram
+        '''
+        from json_ntv.json_mermaid import diagram
+
+        ntv = Ntv.obj(self)
+        node_link = {'nodes': [], 'links': []}
+        dic_node = {}
+        if leaves:
+            nodes = [node for node in NtvTree(
+                ntv) if not isinstance(node.val, list)]
+            dic_node = {node: row for row, node in enumerate(nodes)}
+        Ntv._mermaid_link(ntv, None, node_link, row, dic_node)
+        mermaid_json = {title + ':$flowchart': {
+            'orientation': 'top-down',
+            'node::': {node[0]: node[1] for node in node_link['nodes']},
+            'link::': node_link['links']}}
+        if disp:
+            return display(Image(url="https://mermaid.ink/img/" +
+                                 b64encode(diagram(mermaid_json).encode("ascii")).decode("ascii")))
+        return diagram(mermaid_json)
+
     def to_repr(self, nam=True, typ=True, val=True, maxi=10):
         '''return a simple json representation of the Ntv entity.
 
         *Parameters*
 
         - **nam**: Boolean (default True) : if true, the names are included
         - **typ**: Boolean (default True) : if true, the types are included
         - **val**: Boolean (default True) : if true, the values are included
         - **maxi**: Integer (default 10) : number of values to included for NtvList
-        or NtvSet entities. If maxi < 1 all the values are included.
+        entities. If maxi < 1 all the values are included.
         '''
         ntv = self.code_ntv
         if nam and typ:
             ntv = ntv[0]
         if self.ntv_name and nam:
             ntv += '-' + self.ntv_name
         if self.ntv_type and typ:
@@ -314,48 +470,58 @@
             if val:
                 if ntv:
                     ntv += '-'
                 ntv += json.dumps(self.ntv_value)
             return ntv
         if isinstance(self, NtvSingle) and isinstance(self.ntv_value, NtvSingle):
             return {ntv:  self.ntv_value.to_repr(nam, typ, val)}
-        if isinstance(self, (NtvList, NtvSet)):
+        if isinstance(self, NtvList):
             if maxi < 1:
                 maxi = len(self.ntv_value)
             return {ntv:  [ntvi.to_repr(nam, typ, val) for ntvi in self.ntv_value[:maxi]]}
         raise NtvError('the ntv entity is not consistent')
 
+    def to_name(self, default=''):
+        '''return the name of the NTV entity'''
+        if self.ntv_name == '':
+            return default
+        return self.ntv_name
+
     def to_obj(self, def_type=None, **kwargs):
         '''return the JSON representation of the NTV entity (json-ntv format).
 
         *Parameters*
 
         - **def_type** : NtvType or Namespace (default None) - default type to apply
         to the NTV entity
         - **encoded** : boolean (default False) - choice for return format
         (string/bytes if True, dict/list/tuple else)
         - **encode_format**  : string (default 'json')- choice for return format
         (json, cbor, obj)
         - **simpleval** : boolean (default False) - if True, only value (without
         name and type) is included
+        - **name** : boolean (default true) - if False, name is not included
+        - **json_array** : boolean (default false) - if True, Json-object is not used for NtvList
         '''
         option = {'encoded': False, 'encode_format': 'json',
-                  'simpleval': False} | kwargs
-        value = self._obj_value(def_type=def_type, **option)
-        obj_name = self.obj_name(def_type)
+                  'simpleval': False, 'name': True, 'json_array': False} | kwargs
+        if option['simpleval'] and isinstance(self, NtvList) and not self.json_array:
+            value = NtvList(self).obj_value(def_type=def_type, **option)
+        else:
+            value = self.obj_value(def_type=def_type, **option)
+        obj_name = self.json_name(def_type)
+        if not option['name']:
+            obj_name[0] = ''
         if option['simpleval']:
             name = ''
         elif option['encode_format'] in ('cbor', 'obj') and not Ntv._is_json_ntv(value):
             name = obj_name[0]
         else:
             name = obj_name[0] + obj_name[1] + obj_name[2]
-        if not name:
-            json_obj = value
-        else:
-            json_obj = {name: value}
+        json_obj = {name: value} if name else value
         if option['encoded'] and option['encode_format'] == 'json':
             return json.dumps(json_obj)
         if option['encoded'] and option['encode_format'] == 'cbor':
             return cbor2.dumps(json_obj, datetime_as_timestamp=True,
                                timezone=datetime.timezone.utc, canonical=True,
                                date_as_datetime=True)
         return json_obj
@@ -380,166 +546,183 @@
         typ = None
         if self.ntv_type:
             typ = self.ntv_type.long_name
         if isinstance(self, NtvSingle) and not isinstance(val, NtvSingle):
             return (clas, name, typ, val)
         if isinstance(self, NtvSingle) and isinstance(val, NtvSingle):
             return (clas, name, typ, val.to_tuple(maxi=maxi))
-        if isinstance(self, (NtvList, NtvSet)):
+        if isinstance(self, NtvList):
             if maxi < 1:
                 maxi = len(val)
             return (clas, name, typ, [ntv.to_tuple(maxi=maxi) for ntv in val[:maxi]])
         raise NtvError('the ntv entity is not consistent')
 
-    def _obj_value(self):
+    def obj_value(self):
+        '''abstract method'''
         return ''
 
-    def _obj_sep(self, json_type, def_type=None):
-        return ''
-
-    def obj_name(self, def_type=None, string=False):
-        '''return the JSON name of the NTV entity (json-ntv format)
+    @property
+    def json_array(self):
+        '''abstract method'''
+        return False
 
-        *Parameters*
+    def _obj_sep(self, json_type, def_type):
+        '''abstract method'''
+        return ''
 
-        - **def_typ** : NtvType or Namespace (default None) - type of the parent entity
-        - **string** : boolean (default False) - If True, return a string else a tuple'''
-        if def_type is None:
-            def_type = ''
-        elif isinstance(def_type, (NtvType, Namespace)):
-            def_type = def_type.long_name
-        json_name = ''
-        if self.ntv_name:
-            json_name = self.ntv_name
-        json_type = ''
-        if self.ntv_type:
-            json_type = relative_type(def_type, self.ntv_type.long_name)
-        if json_type == 'json' and (not def_type or def_type == 'json'):
-            json_type = ''
-        json_sep = self._obj_sep(json_type, def_type)
-        if string:
-            return json_name + json_sep + json_type
-        return (json_name, json_sep, json_type)
+    @staticmethod
+    def _from_value(value, decode_str):
+        '''return a decoded value'''
+        if isinstance(value, bytes):
+            value = cbor2.loads(value)
+        elif decode_str and isinstance(value, str) and value.lstrip() and value.lstrip()[0] in '"-{[0123456789':
+            try:
+                value = json.loads(value)
+            except JSONDecodeError:
+                pass
+        string = isinstance(value, str)
+        if value is None or (string and value == 'null'):
+            return NtvSingle(None)
+        if string and value == 'true':
+            return NtvSingle(True)
+        if string and value == 'false':
+            return NtvSingle(False)
+        return value
 
     @staticmethod
     def _decode(json_value):
         '''return (name, type, value, separator) of the json value'''
         if json_value is None:
             return (None, None, None, None)
+        # if isinstance(json_value, tuple):
+        #    return (None, None, list(json_value), None)
+        # if isinstance(json_value, (int, str, float, bool)):
         if isinstance(json_value, (list, int, str, float, bool)):
             return (None, None, json_value, None)
         if isinstance(json_value, dict) and len(json_value) != 1:
             return (None, None, json_value, None)
         if isinstance(json_value, dict) and len(json_value) == 1:
             json_name = list(json_value.keys())[0]
             val = json_value[json_name]
             nam, typ, sep = Ntv.from_obj_name(json_name)
             return (nam, typ, val, sep)
         return(*Ntv._cast(json_value), ':')
 
     @staticmethod
     def _cast(data):
-        '''return (name, type, value) of the data'''
+        '''return (name, type, json_value) of the data'''
         dic_geo_cl = {'Point': 'point', 'MultiPoint': 'multipoint', 'LineString': 'line',
                       'MultiLineString': 'multiline', 'Polygon': 'polygon',
                       'MultiPolygon': 'multipolygon'}
         dic_connec = NtvConnector.dic_connec()
         clas = data.__class__.__name__
         match clas:
+            case 'tuple':
+                return (None, 'array', list(data))
             case 'date' | 'time' | 'datetime':
                 return (None, clas, data.isoformat())
             case 'Point' | 'MultiPoint' | 'LineString' | 'MultiLineString' | \
                     'Polygon' | 'MultiPolygon':
                 return (None, dic_geo_cl[data.__class__.__name__],
                         Ntv._listed(data.__geo_interface__['coordinates']))
             case 'NtvSingle' | 'NtvSet' | 'NtvList':
                 return (None, 'ntv', data.to_obj())
-            case 'Ilist':
-                return (None, 'tab', data.to_obj())
             case _:
                 connec = None
                 if clas in dic_connec and dic_connec[clas] in NtvConnector.connector():
                     connec = NtvConnector.connector()[dic_connec[clas]]
                 if connec:
                     return connec.to_ntv(data)
-                raise NtvError('connector is not defined to NTV entity')
+                raise NtvError(
+                    'connector is not defined for NTV entity of class : ', clas)
         return (None, None, None)
 
     def _uncast(self, **option):
         '''return object from ntv_value'''
         dic_fct = {'date': datetime.date.fromisoformat, 'time': datetime.time.fromisoformat,
-                   'datetime': datetime.datetime.fromisoformat}
+                   'datetime': datetime.datetime.fromisoformat, 'array': tuple}
         dic_geo = {'point': 'point', 'multipoint': 'multipoint', 'line': 'linestring',
                    'multiline': 'multilinestring', 'polygon': 'polygon',
                    'multipolygon': 'multipolygon'}
         dic_cbor = {'point': False, 'multipoint': False, 'line': False,
                     'multiline': False, 'polygon': False, 'multipolygon': False,
                     'date': True, 'time': False, 'datetime': True}
-        dic_obj = {'tab': 'Ilist', 'other': None}
+        dic_obj = {'tab': 'IlistConnec',
+                   'field': 'IindexConnec', 'other': None}
         type_n = self.ntv_type.name
         if 'dicobj' in option:
             dic_obj |= option['dicobj']
         obj = not option['encode_format'] == 'cbor' or \
             (self.ntv_type and type_n in dic_cbor and dic_cbor[type_n])
         if self.ntv_type is None or not obj:
             return self.ntv_value
         if type_n in dic_fct:
             return dic_fct[type_n](self.ntv_value)
         if type_n == 'ntv':
             return Ntv.obj(self.ntv_value)
         if type_n in dic_geo:
             return geometry.shape({"type": dic_geo[type_n],
                                    "coordinates": self.ntv_value})
-        if type_n == 'tab' and dic_obj[type_n] == 'Ilist':
-            if isinstance(self.ntv_value, list):
-                return Ilist.obj(self.ntv_value)
-            return Ilist.dic(self.ntv_value)
         connec = None
         if type_n in dic_obj and \
                 dic_obj[type_n] in NtvConnector.connector():
             connec = NtvConnector.connector()[dic_obj[type_n]]
         elif dic_obj['other'] in NtvConnector.connector():
             connec = NtvConnector.connector()['other']
         if connec:
-            return connec.from_ntv(self.ntv_value)
+            return connec.from_ntv(self.ntv_value, **option)
         return self.ntv_value
 
     @staticmethod
-    def from_obj_name(string):
-        '''return a tuple with name, type and separator from string'''
-        if not isinstance(string, str):
-            raise NtvError('a json-name have to be str')
-        if string == '':
-            return (None, None, None)
-        sep = None
-        if '::' in string:
-            sep = '::'
-        elif ':' in string:
-            sep = ':'
-        if sep is None:
-            return (string, None, None)
-        split = string.rsplit(sep, 2)
-        if len(split) == 1:
-            return (string, None, sep)
-        if split[0] == '':
-            return (None, split[1], sep)
-        if split[1] == '':
-            return (split[0], None, sep)
-        return (split[0], split[1], sep)
-
-    @staticmethod
     def _is_json_ntv(val):
         ''' return True if val is a json type'''
+        # return val is None or isinstance(val, (list, int, str, float, bool, dict))
         return val is None or isinstance(val, (list, int, str, float, bool, dict))
 
     @staticmethod
     def _listed(idx):
         '''transform a tuple of tuple in a list of list'''
         return [val if not isinstance(val, tuple) else Ntv._listed(val) for val in idx]
 
+    @staticmethod
+    def _mermaid_node(ntv, def_typ_str, num, dic_node):
+        '''create and return a node'''
+        j_name, j_sep, j_type = ntv.json_name(def_typ_str)
+        name = ''
+        if j_name:
+            name += '<b>' + j_name + '</b>\n'
+        if j_type:
+            name += j_type + '\n'
+        if ntv in dic_node:
+            num += ' ' + str(dic_node[ntv])
+        if num:
+            name += '<i>' + num + '</i>\n'
+        elif isinstance(ntv, NtvSingle):
+            if isinstance(ntv.val, str):
+                name += '<i>' + ntv.val + '</i>\n'
+            else:
+                name += '<i>' + json.dumps(ntv.val) + '</i>\n'
+            return [ntv.address_name, ['rectangle', name[:-1]]]
+        if not name:
+            name = '<b>::</b>\n'
+        return [ntv.address_name, ['roundedge', name[:-1]]]
+
+    @staticmethod
+    def _mermaid_link(ntv, def_typ_str, node_link, row, dic_node):
+        '''add nodes and links from ntv in node_list and link_list '''
+        num = str(len(node_link['nodes'])) if row else ''
+        node_link['nodes'].append(Ntv._mermaid_node(
+            ntv, def_typ_str, num, dic_node))
+        if isinstance(ntv, NtvList):
+            for ntv_val in ntv:
+                Ntv._mermaid_link(ntv_val, ntv.type_str,
+                                  node_link, row, dic_node)
+                node_link['links'].append(
+                    [ntv.address_name, 'normalarrow', ntv_val.address_name])
+
 
 class NtvSingle(Ntv):
     ''' An NTV-single entity is a Ntv entity not composed with other entities.
 
     *Attributes :*
 
     - **ntv_name** : String - name of the NTV entity
@@ -561,205 +744,263 @@
     - `set_name`
     - `set_type`
     - `set_value`
     - `to_obj`
     - `to_repr`
     '''
 
-    def __init__(self, value, ntv_name=None, ntv_type=None):
+    def __init__(self, value, ntv_name=None, ntv_type=None, fast=False):
         '''NtvSingle constructor.
 
         *Parameters*
 
         - **ntv_name** : String (default None) - name of the NTV entity
         - **ntv_type**: String (default None) - type of the entity
         - **value**: value of the entity
         '''
-        is_json_ntv = Ntv._is_json_ntv(
-            value)  # or isinstance(value, NtvSingle)
-        if not ntv_type and is_json_ntv:
-            ntv_type = 'json'
-        if not ntv_type and not is_json_ntv:
-            name, ntv_type, value = Ntv._cast(value)
-            if not ntv_name:
-                ntv_name = name
-        elif ntv_type and not is_json_ntv:
-            raise NtvError('ntv_value is not compatible with ntv_type')
-        if ntv_type and isinstance(ntv_type, str) and ntv_type[-1] == '.':
-            raise NtvError('the ntv_type is not valid')
+        if not fast:
+            # or isinstance(value, NtvSingle)
+            is_json_ntv = Ntv._is_json_ntv(value)
+
+            if not is_json_ntv:
+                name, typ, value = Ntv._cast(value)
+            if not ntv_type:
+                if is_json_ntv:
+                    ntv_type = 'json'
+                else:
+                    ntv_type = typ
+                    if not ntv_name:
+                        ntv_name = name
+            else:
+                if not is_json_ntv and NtvType(ntv_type) != NtvType(typ):
+                    raise NtvError('ntv_value is not compatible with ntv_type')
+            if ntv_type and isinstance(ntv_type, str) and ntv_type[-1] == '.':
+                raise NtvError('the ntv_type is not valid')
         super().__init__(value, ntv_name, ntv_type)
 
     def __eq__(self, other):
         ''' equal if name type and value are equal'''
         return self.__class__.__name__ == other.__class__.__name__ and\
             self.ntv_name == other.ntv_name and self.ntv_type == other.ntv_type and\
             self.ntv_value == other.ntv_value
 
+    def __hash__(self):
+        '''return hash(name) + hash(type) + hash(value)'''
+        return hash(self.ntv_name) + hash(self.ntv_type) + hash(json.dumps(self.ntv_value))
+
     def _obj_sep(self, json_type, def_type=None):
         ''' return separator to include in json_name'''
         if json_type or not def_type and \
             (isinstance(self.ntv_value, list) or
              isinstance(self.ntv_value, dict) and len(self.ntv_value) != 1):
             return ':'
         return ''
 
-    def _obj_value(self, def_type=None, **kwargs):
-        '''return the Json format of the ntv_value'''
+    @property
+    def json_array(self):
+        ''' return the json_array dynamic attribute'''
+        return False
+
+    def obj_value(self, def_type=None, **kwargs):
+        '''return the ntv_value with different formats defined by kwargs'''
         option = {'encoded': False, 'encode_format': 'json',
                   'simpleval': False} | kwargs
         if option['encode_format'] in ('json', 'tuple'):
             return self.ntv_value
+        if option['encode_format'] == 'obj' and self.ntv_value == 'null':
+            return None
         return Ntv._uncast(self, **option)
 
 
 class NtvList(Ntv):
     '''An NTV-list entity is a Ntv entity where:
 
     - ntv_value is a list of NTV entities,
     - ntv_type is a default type available for included NTV entities
 
     *Attributes :*
 
     - **ntv_name** : String - name of the NTV entity
     - **ntv_type**: NtvType - type of the entity
     - **ntv_value**:  value of the entity
+    - **json_array**: Boolean - False if all the entity names are present and different
+    (dynamic value)
 
     The methods defined in this class are :
 
     *Ntv constructor*
     - `obj`
     - `from_obj`
     - `from_att`
 
     *dynamic values (@property)*
     - `type_str`
     - `code_ntv`
+    - `json_array`
 
     *instance methods*
     - `set_name`
     - `set_type`
     - `set_value`
     - `to_obj`
     - `to_repr`
     '''
 
-    def __init__(self, list_ntv, ntv_name=None, ntv_type=None):
+    def __init__(self, list_ntv, ntv_name=None, ntv_type=None, fast=False):
         '''NtvList constructor.
 
         *Parameters*
 
         - **ntv_name** : String (default None) - name of the NTV entity
         - **ntv_type**: String (default None) - default type or namespace of the included entities
         - **list_ntv**: list - list of Ntv objects or obj_value of Ntv objectd
         '''
-        if isinstance(list_ntv, (NtvList, NtvSet)):
+        if isinstance(list_ntv, NtvList):
             ntv_value = list_ntv.ntv_value
             ntv_type = list_ntv.ntv_type
             ntv_name = list_ntv.ntv_name
-        elif isinstance(list_ntv, list):
+        elif fast and isinstance(list_ntv, list):
+            ntv_value = [NtvSingle(val, ntv_type=ntv_type, fast=True)
+                         for val in list_ntv]
+        elif not fast and isinstance(list_ntv, list):
             ntv_value = [Ntv.from_obj(ntv, ntv_type, ':') for ntv in list_ntv]
         else:
             raise NtvError('ntv_value is not a list')
-        if not ntv_type and len(ntv_value) > 0 and ntv_value[0].ntv_type:  # and \
-            #    ntv_value[0].ntv_type.long_name != 'json':
+        if not ntv_type and len(ntv_value) > 0 and ntv_value[0].ntv_type:
             ntv_type = ntv_value[0].ntv_type
         super().__init__(ntv_value, ntv_name, ntv_type)
+        for row, ntv in enumerate(self):
+            ntv.parent = self
+            ntv._row = row
+
+    @property
+    def json_array(self):
+        ''' return the json_array dynamic attribute'''
+        set_name = {ntv.ntv_name for ntv in self}
+        return '' in set_name or len(set_name) != len(self)
 
     def __eq__(self, other):
         ''' equal if name and value are equal'''
         return self.__class__.__name__ == other.__class__.__name__ and\
             self.ntv_name == other.ntv_name and self.ntv_value == other.ntv_value
 
+    def __hash__(self):
+        '''return hash(name) + hash(value)'''
+        return hash(self.ntv_name) + hash(tuple(self.ntv_value))
+
     def _obj_sep(self, json_type, def_type=None):
         ''' return separator to include in json_name'''
-        if json_type:
+        if json_type or (len(self.ntv_value) == 1 and not self.json_array):
             return '::'
         return ''
 
-    def _obj_value(self, def_type=None, **kwargs):
-        '''return the Json format of the ntv_value'''
+    def obj_value(self, def_type=None, **kwargs):
+        '''return the ntv_value with different formats defined by kwargs'''
         option = {'encoded': False, 'encode_format': 'json',
-                  'simpleval': False} | kwargs
-        option2 = option | {'encoded': False}
+                  'simpleval': False, 'json_array': False} | kwargs
+        opt2 = option | {'encoded': False}
         if self.ntv_type:
             def_type = self.ntv_type.long_name
-        return [ntv.to_obj(def_type=def_type, **option2) for ntv in self.ntv_value]
+        if self.json_array or option['simpleval'] or option['json_array']:
+            return [ntv.to_obj(def_type=def_type, **opt2) for ntv in self.ntv_value]
+        values = [ntv.to_obj(def_type=def_type, **opt2)
+                  for ntv in self.ntv_value]
+        return {list(val.items())[0][0]: list(val.items())[0][1] for val in values}
 
 
-class NtvSet(Ntv):
-    '''An NTV-set entity is a Ntv entity where:
-
-    - ntv_value is a list of NTV entities,
-    - ntv_type is a default type available for included NTV entities
+class NtvTree:
+    ''' The NtvTree class is an iterator class used to traverse a NTV tree structure.
+    Some other methods give tree indicators and data.
 
     *Attributes :*
 
-    - **ntv_name** : String - name of the NTV entity
-    - **ntv_type**: NtvType - type of the entity
-    - **ntv_value**:  value of the entity
-
-    The methods defined in this class are :
-
-    *Ntv constructor*
-    - `obj`
-    - `from_obj`
-    - `from_att`
+    - **ntv** : Ntv entity
+    - **_node**:  Ntv entity - node pointer
 
     *dynamic values (@property)*
-    - `type_str`
-    - `code_ntv`
-
-    *instance methods*
-    - `set_name`
-    - `set_type`
-    - `set_value`
-    - `to_obj`
-    - `to_repr`
+    - `breadth`
+    - `size`
+    - `height`
+    - `adjacency_list`
+    - `nodes`
+    - `leaf_nodes`
+    - `inner_nodes`
     '''
 
-    def __init__(self, list_ntv, ntv_name=None, ntv_type=None):
-        '''NtvSet constructor.
+    def __init__(self, ntv):
+        ''' the parameter of the constructor is the Ntv entity'''
+        self.ntv = ntv
+        self._node = None
+
+    def __iter__(self):
+        ''' iterator without initialization'''
+        return self
+
+    def __next__(self):
+        ''' return next node in the tree'''
+        if not self._node:
+            self._node = self.ntv
+        elif isinstance(self._node.val, list):
+            self._next_down()
+        else:
+            self._next_up()
+        return self._node
 
-        *Parameters*
+    @property
+    def breadth(self):
+        ''' return the number of leaves'''
+        return len(self.leaf_nodes)
 
-        - **ntv_name** : String (default None) - name of the NTV entity
-        - **ntv_type**: String (default None) - default type or namespace of the included entities
-        - **list_ntv**: list - list of Ntv objects or obj_value
-        '''
-        if isinstance(list_ntv, (NtvList, NtvSet)):
-            ntv_value = list_ntv.ntv_value
-            ntv_type = list_ntv.ntv_type
-            ntv_name = list_ntv.ntv_name
-        elif isinstance(list_ntv, list):
-            ntv_value = [Ntv.from_obj(ntv, ntv_type, ':') for ntv in list_ntv]
-        else:
-            raise NtvError('ntv_value is not a list')
-        super().__init__(ntv_value, ntv_name, ntv_type)
+    @property
+    def size(self):
+        ''' return the number of nodes'''
+        return len(self.nodes)
 
-    def __eq__(self, other):
-        ''' equal if name and value are equal'''
-        return self.__class__.__name__ == other.__class__.__name__ and\
-            self.ntv_name == other.ntv_name and self.ntv_value == other.ntv_value
+    @property
+    def height(self):
+        ''' return the height of the tree'''
+        return max(len(node.address) for node in self.__class__(self.ntv)) - 1
 
-    def _obj_sep(self, json_type, def_type=None):
-        ''' return separator to include in json_name'''
-        if json_type or len(self.ntv_value) == 1:
-            return '::'
-        return ''
+    @property
+    def adjacency_list(self):
+        ''' return a dict with the list of child nodes for each parent node'''
+        return {node: node.val for node in self.inner_nodes}
 
-    def _obj_value(self, def_type=None, **kwargs):
-        '''return the Json format of the ntv_value'''
-        option = {'encoded': False, 'encode_format': 'json',
-                  'simpleval': False} | kwargs
-        option2 = option | {'encoded': False}
-        if self.ntv_type:
-            def_type = self.ntv_type.long_name
-        return {list(ntv.to_obj(def_type=def_type, **option2).items())[0][0]:
-                list(ntv.to_obj(def_type=def_type, **option2).items())[0][1]
-                for ntv in self.ntv_value}
+    @property
+    def nodes(self):
+        ''' return the list of nodes'''
+        return list(self.__class__(self.ntv))
+
+    @property
+    def leaf_nodes(self):
+        ''' return the list of leaf nodes'''
+        return [node for node in self.__class__(self.ntv) if not isinstance(node.val, list)]
+
+    @property
+    def inner_nodes(self):
+        ''' return the list of inner nodes'''
+        return [node for node in self.__class__(self.ntv) if isinstance(node.val, list)]
+
+    def _next_down(self):
+        ''' find the next subchild node'''
+        self._node = self._node[0]
+
+    def _next_up(self):
+        ''' find the next sibling or ancestor node'''
+        parent = self._node.parent
+        if not parent:
+            raise StopIteration
+        ind = parent.val.index(self._node)
+        if ind < len(parent) - 1:  # if ind is not the last
+            self._node = parent[ind + 1]
+        else:
+            if parent == self.ntv:
+                raise StopIteration
+            self._node = parent
+            self._next_up()
 
 
 class NtvConnector(ABC):
     ''' The NtvConnector class is an abstract class used for all NTV connectors.
     A NTV connector has two methods for conversion between NTV data and an object'''
 
     @classmethod
```

### Comparing `json_ntv-0.0.5/json_ntv.egg-info/PKG-INFO` & `json_ntv-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: json-ntv
-Version: 0.0.5
+Name: json_ntv
+Version: 0.1.0
 Summary: JSON-NTV a semantic format for interoperability
 Home-page: https://github.com/loco-philippe/NTV/blob/main/README.md
 Author: Philippe Thomy
 Author-email: philippe@loco-labs.io
 Keywords: JSON-NTV,semantic JSON,development,environmental data
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -36,30 +36,30 @@
 The constructed entities (called NTV for *named typed value*) are therefore a triplet with one mandatory element (the value in JSON format) and two optional elements (name, type).
 >
 > *For example, the location of Paris can be represented by:*
 > - *a name: "Paris",*
 > - *a type: the coordinates of a point according to the GeoJSON format,*
 > - *a value: [ 2.3522, 48.8566]*
 
-The easiest way to add this information is to use a JSON-object with a single member using the syntax [JSON-ND](https://github.com/glenkleidon/JSON-ND) for the first term of the member and the JSON-value for the second term of the member.
+The easiest way to add this information into a JSON-value is to use a JSON-object with a single member using the syntax [JSON-ND](https://github.com/glenkleidon/JSON-ND) for the first term of the member and the JSON-value for the second term of the member.
 >
 > *For the example above, the JSON representation is:*    
 > *```{ "paris:point" : [2.3522, 48.8566] }```*
 
-With this approach, three NTV entities are defined:
+With this approach, two NTV entities are defined:
 - a primitive entity which is not composed of any other entity (NTV-single),
-- two structured entities: an unordered collection of NTV entities (NTV-set) and an ordered sequence of NTV entities (NTV-list).
+- a structured entity which is an ordered sequence of NTV entities (Ntv-list).
       
 as well as two JSON formats:
 - simple format when the name and the type are not present (this is the usual case of CSV data),
 - named format when the name or type is present (see example above for an NTV-single entity and below for a structured entity).
 >
 > *Example of an entity composed of two other entities:*
-> - *```{ "cities::point": [[2.3522, 48.8566], [4.8357, 45.7640]] }``` for an NTV-list entity*
-> - *```{ "cities::point": { "paris":[2.3522, 48.8566], "lyon":[4.8357, 45.7640] } }``` for an NTV-set entity*
+> - *```{ "cities::point": [[2.3522, 48.8566], [4.8357, 45.7640]] }``` for an unnamed NTV-list entity*
+> - *```{ "cities::point": { "paris":[2.3522, 48.8566], "lyon":[4.8357, 45.7640] } }``` for a named NTV-list entity*
 >
 > *Note: This syntax can also be used for CSV file headers*
 
 The type incorporates a notion of `namespaces` that can be nested.
 > *For example, the type: "ns1.ns2.type" means that:*
 > - *ns1. is a namespace defined in the global namespace,*
 > - *ns2. is a namespace defined in the ns1 namespace.,*
```

### Comparing `json_ntv-0.0.5/setup.py` & `json_ntv-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="json_ntv",
-    version="0.0.5",
+    version="0.1.0",
     description="JSON-NTV a semantic format for interoperability",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/loco-philippe/NTV/blob/main/README.md",
     author="Philippe Thomy",
     author_email="philippe@loco-labs.io",
     classifiers=[
```

### Comparing `json_ntv-0.0.5/tests/tests_namespace.py` & `json_ntv-0.1.0/tests/tests_namespace.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,17 @@
         liststr = ['fr.$IRVE.', '$a.', '$b.$c.', '$a.$c.', '$a.c.c.', 'fr.$a.b.']
         for nstr in liststr:
             self.assertEqual(Namespace.add(nstr).file, None)        
             self.assertEqual(Namespace.add(nstr).content, {'type': {}, 'namespace': {}})        
 
 class Test_NtvType(unittest.TestCase):
     
+    def test_self_init(self):
+        self.assertEqual(NtvType(NtvType('datetime')), NtvType('datetime'))
+        
     def test_add(self):
         liststr = ['fr.BAN.lon', 'fr.BAN.$lon', 'year', 'fr.reg', 'fr.BAN.numero',
                    'fr.reg', 'fr.$IRVE.$a', '$a.$c', 'fr.$c', '$a.c.c.d', 'fr.$a.b.d']
         for tstr in liststr:
             self.assertEqual(NtvType.add(tstr).long_name, tstr)
     
     def test_add_ko(self):
```

### Comparing `json_ntv-0.0.5/tests/tests_ntv.py` & `json_ntv-0.1.0/tests/tests_ntv.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,20 +7,17 @@
 The `NTV.test_ntv` module contains the unit tests (class unittest) for the
 `NtvSingle`, `NtvList` and `NtvSet` classes.
 """
 import unittest
 import datetime
 import csv
 
-from json_ntv import NtvSingle, NtvList, NtvSet, Ntv, NtvError, NtvType, from_csv, to_csv, agreg_type
+from json_ntv import NtvSingle, NtvList, Ntv, NtvError, from_csv, to_csv, agreg_type, NtvTree
 from shapely import geometry
 
-from ntv_connector import to_csv, from_csv
-from observation import Ilist
-
 
 class Test_Ntv_creation(unittest.TestCase):
 
     def test_single_obj_name(self):
         list_obj = [['json', 4, ('', '', '')],
                     ['fr.', 4, ('', ':', 'json')],
                     ['point', 4, ('', ':', 'json')],
@@ -37,19 +34,20 @@
                     ['', {"::point": [1, 2]}, ('', '::', 'point')],
                     ['fr.', {"::fr.reg": [1, 2]}, ('', '::', 'reg')],
                     #['', {"::json": [1, 2]}, ('', '::', 'json')],
                     ['', {"::json": [1, 2]}, ('', '', '')],
                     ['json', {"::json": [1, 2]}, ('', '', '')],
                     #['json', {"::": [1, 2]}, ('', '::', 'json')],
                     ['json', {"::": [1, 2]}, ('', '', '')],
+                    ['array', {":array": [1, 2]}, ('', '', '')],
                     ]
         for data in list_obj:
             ntv = Ntv.obj(data[1])
-            #print(ntv)
-            self.assertEqual(ntv.obj_name(data[0]), data[2])
+            # print(ntv)
+            self.assertEqual(ntv.json_name(data[0]), list(data[2]))
 
     def test_agreg_type(self):
         list_type = [[[None, None, True], 'json'],
                      [['point', None, True], 'point'],
                      [[None, 'fr.', True], 'json'],
                      [['json', None, True], 'json'],
                      [['point', 'date', True], 'point'],
@@ -69,37 +67,48 @@
             if typ[0] == [None, None, False]:
                 self.assertEqual(agreg_type(
                     typ[0][0], typ[0][1], typ[0][2]), typ[1])
             else:
                 self.assertEqual(agreg_type(
                     typ[0][0], typ[0][1], typ[0][2]).long_name, typ[1])
 
+    def test_address(self):
+        a = Ntv.obj({'test': {'t1': 1, 't2': 2, 't3': [3, 4]}})
+        self.assertTrue(a.parent is None)
+        self.assertEqual(a.address, [0])
+        self.assertEqual(a.address_name, '0')
+        self.assertEqual(a['t3'].address, [0, 2])
+        self.assertEqual(a['t3'].address_name, '0.2')
+        self.assertEqual(a['t3'][0].parent.parent, a)
+        self.assertEqual(a['t3'][0].address, [0, 2, 0])
+        self.assertEqual(a['t3'][0].address_name, '0.2.0')
+
     def test_from_obj_repr(self):
-        list_repr = [[1, '"v"'],
-                     [{"truc":  1}, '"vN"'],
-                     [{":point": 1}, '"vT"'],
-                     [{"truc:":  1}, '"vN"'],
-                     [{":": 1}, '"v"'],
-                     [[1, 2], '{"l": ["v", "v"]}'],
-                     [{"truc": [1, 2]}, '{"lN": ["v", "v"]}'],
-                     [{":point": [1, 2]}, '"vT"'],
-                     [{"truc:":  [1, 2]}, '"vN"'],
-                     [{":": [1, 2]}, '"v"'],
-                     [{"::": [1, 2]}, '{"l": ["v", "v"]}'],
-                     [{"::": {"a": 2}}, '{"s": ["vN"]}'],
+        list_repr = [[1, '"s"'],
+                     [{"truc":  1}, '"sN"'],
+                     [{":point": 1}, '"sT"'],
+                     [{"truc:":  1}, '"sN"'],
+                     [{":": 1}, '"s"'],
+                     [[1, 2], '{"l": ["s", "s"]}'],
+                     [{"truc": [1, 2]}, '{"lN": ["s", "s"]}'],
+                     [{":point": [1, 2]}, '"sT"'],
+                     [{"truc:":  [1, 2]}, '"sN"'],
+                     [{":": [1, 2]}, '"s"'],
+                     [{"::": [1, 2]}, '{"l": ["s", "s"]}'],
+                     [{"::": {"a": 2}}, '{"l": ["sN"]}'],
                      [{"::": [[1, 2], [3, 4]]},
-                         '{"l": [{"l": ["v", "v"]}, {"l": ["v", "v"]}]}'],
-                     [{"::point": [[1, 2], [3, 4]]}, '{"lT": ["vT", "vT"]}'],
-                     [{"a": 2}, '"vN"'],
-                     #[{"truc": {"a": 2}}, '{"vN": "vN"}'],
-                     [{":point": {"a": 2}}, '"vT"'],
-                     [{"truc:": {"a": 2}}, '"vN"'],
-                     [{":": {"a": 2}}, '"v"']]
+                         '{"l": [{"l": ["s", "s"]}, {"l": ["s", "s"]}]}'],
+                     [{"::point": [[1, 2], [3, 4]]}, '{"lT": ["sT", "sT"]}'],
+                     [{"a": 2}, '"sN"'],
+                     #[{"truc": {"a": 2}}, '{"sN": "sN"}'],
+                     [{":point": {"a": 2}}, '"sT"'],
+                     [{"truc:": {"a": 2}}, '"sN"'],
+                     [{":": {"a": 2}}, '"s"']]
         for test in list_repr:
-            #print(test)
+            # print(test)
             self.assertEqual(repr(Ntv.from_obj(test[0])), test[1])
 
     def test_from_obj_ko(self):
         liststr = [{"::": 1}]
         for nstr in liststr:
             with self.assertRaises(NtvError):
                 Ntv.from_obj(nstr)
@@ -123,161 +132,211 @@
         for obj in list_obj:
             self.assertEqual(Ntv.from_obj(
                 NtvSingle(obj).to_obj()), NtvSingle(obj))
             self.assertEqual(NtvSingle(obj).to_obj(encode_format='obj'), obj)
 
     def test_from_att(self):
         self.assertEqual(
-            repr(Ntv.obj(([[1, 2], [3, 4]], None, 'point', 'single'))), '"vT"')
+            repr(Ntv.obj(([[1, 2], [3, 4]], None, 'point', 'single'))), '"sT"')
         self.assertEqual(
-            repr(Ntv.obj(([[1, 2], [3, 4]], None, 'point', 'list'))), '{"lT": ["vT", "vT"]}')
+            repr(Ntv.obj(([[1, 2], [3, 4]], None, 'point', 'list'))), '{"lT": ["sT", "sT"]}')
 
     def test_from_obj(self):
-        dictstr = {'0NtvSingle': None,
-                   'oNtvSingle': {'none': None},
-                   '1NtvSingle': 1,
-                   '2NtvSingle': 'test',
-                   '3NtvSingle': {'single': 1},
-                   '4NtvSingle': {'ntv1:ntv': {'ntv2': 2}},
-                   '5NtvSingle': {'ntv1:fr.reg': {'ntv2:fr.BAN.lon': 2}},
-                   '6NtvSingle': {'ntv1': True},
-                   '7NtvSingle': True,
-                   '8NtvSingle': {'ntv1:dat': [1, 2]},
-                   '9NtvSingle': {'ntv1': datetime.date(2021, 2, 1)},
-                   'dNtvSingle': datetime.date(2021, 2, 1),
-                   'aNtvSingle': '{ner',
-                   'bNtvSingle': {':$point': {'a': [1, 2], 'b': [3, 4]}},
-                   'cNtvSingle': {':': [{'paris': [2.1, 40.3]}, {'lyon': [2.1, 40.3]}]},
-                   'eNtvSingle': {':': NtvSingle(1,'test')},
-                   'hNtvSingle': {'set:': NtvSet([{'l1':21}, {'l2': [2,3]}])},
-                   'fNtvSingle': {'set:': NtvSet([{'l1':21}, {'l2': datetime.date(2021, 2, 1)}])},
-                   'gNtvSingle': {'lis:': NtvList([{'l1':21}, {'l2': datetime.date(2021, 2, 1)}])},
-                   'iNtvSingle': {'lis:': NtvList([1,2,3])},
-                   '1NtvList': [],
-                   '2NtvList': [[4, [5, 6]], {'heure': [21, 22]}],
-                   '3NtvList': [[4, 5], {'heure': 21}],
-                   '4NtvList': [[4, 5], 21],
-                   '5NtvList': [[4, 5], [1, 2, 3]],
-                   '6NtvList': {'ntv1::fr.reg': [[4, [5, 6]], {'heure': [21, 22]}]},
-                   '7NtvList': {'ntv1::fr.reg': [4]},
-                   '8NtvList': {'ntv1::fr.': [4]},
-                   '9NtvList': [[4, [5, 6]], {'heure': [datetime.time(10, 25, 10), 22]}],
-                   'aNtvList': [[4, [5, 6]], {'heure': [datetime.time(10, 25, 10),
+        dictstr = [['NtvSingle', None],
+                   ['NtvSingle', {'none': None}],
+                   ['NtvSingle', 1],
+                   ['NtvSingle', 'test'],
+                   ['NtvSingle', {'Single': 1}],
+                   ['NtvSingle', {'Ntv1:ntv': {'Ntv2': 2}}],
+                   ['NtvSingle', {'Ntv1': {'Ntv2': 2}}],
+                   ['NtvSingle', {'Ntv1:fr.reg': {'Ntv2:fr.BAN.lon': 2}}],
+                   ['NtvSingle', {'Ntv1': True}],
+                   ['NtvSingle', True],
+                   ['NtvSingle', {'Ntv1:array': [1, 2]}],
+                   ['NtvSingle', {'Ntv1:dat': [1, 2]}],
+                   ['NtvSingle', '{ner'],
+                   ['NtvSingle', {':$point': {'a': [1, 2], 'b': [3, 4]}}],
+                   ['NtvSingle', {
+                       ':': [{'paris': [2.1, 40.3]}, {'lyon': [2.1, 40.3]}]}],
+                   ['NtvList', [[4, [5, 6]], {'heure': [21, 22]}]],
+                   ['NtvList', [[4, 5], {'heure': 21}]],
+                   ['NtvList', [[4, 5], 21]],
+                   ['NtvList', [[4, 5], [1, 2, 3]]],
+                   ['NtvList', {'Ntv1::fr.reg': [
+                       [4, [5, 6]], {'heure': [21, 22]}]}],
+                   ['NtvList', {'Ntv1::fr.reg': [4]}],
+                   ['NtvList', {'Ntv1::fr.': [4]}],
+                   ['NtvList', {'cities::point': [[2.1, 40.3], [2.1, 40.3]]}],
+                   ['NtvList', {}],
+                   ['NtvList', {'Ntv1': 1, 'Ntv2': '2'}],
+                   ['NtvList', {'Ntv3': {'Ntv1': 1, 'Ntv2': '2'}}],
+                   ['NtvList', {"::": {" a": 2}}],
+                   ['NtvList', {"test::": {"a": 2}}]]
+        dictstr2 = [
+                   ['NtvSingle', {':': NtvSingle(1, 'test')}, {
+                       ':ntv': {'test': 1}}],
+                   ['NtvSingle', {'set': NtvList([{'l1': 21}, {'l2': [2, 3]}])},
+                    {'set:ntv': {'l1': 21, 'l2': [2, 3]}}],
+                   ['NtvSingle', {'lis:': NtvList([1, 2, 3])}, {
+                       'lis:ntv': [1, 2, 3]}],
+                   ['NtvSingle', {'Ntv1': datetime.date(2021, 2, 1)},
+                    {'Ntv1:date': '2021-02-01'}],
+                   ['NtvSingle', {'Ntv1:date': datetime.date(2021, 2, 1)},
+                    {'Ntv1:date': '2021-02-01'}],
+                   ['NtvSingle', datetime.date(2021, 2, 1), {
+                       ':date': '2021-02-01'}],
+                   ['NtvSingle', {'set:': NtvList([{'l1': 21}, {'l2': datetime.date(2021, 2, 1)}])},
+                    {'set:ntv': {'l1': 21, 'l2:date': '2021-02-01'}}],
+                   ['NtvList', [[4, [5, 6]], {'heure': [datetime.time(10, 25, 10), 22]}],
+                    [[4, [5, 6]], {'heure::time': ['10:25:10', {':json': 22}]}]],
+                   ['NtvList', [[4, [5, 6]], {'heure': [datetime.time(10, 25, 10),
                                                         geometry.point.Point((3, 4))]}],
-                   'bNtvList': {'::': [{'paris': [2.1, 40.3]}, {'lyon': [2.1, 40.3]}]},
-                   'cNtvList': {'cities::point': [[2.1, 40.3], [2.1, 40.3]]},
-                   '1NtvSet': {},
-                   '2NtvSet': {'ntv1': 1, 'ntv2': '2'},
-                   '3NtvSet': {'ntv3': {'ntv1': 1, 'ntv2': '2'}},
-                   '4NtvSet': {'ntv3::fr.reg': {'ntv1': 1, 'ntv2:fr.reg': '2'}},
-                   '5NtvSet': {'ntv3::fr.reg': {'ntv1': [1, 2], 'ntv2:fr.reg': '2'}},
-                   '6NtvSet': {"::": {" a": 2}},
-                   '7NtvSet': {"test::": {"a": 2}}
-                   }
-        liststr = list(dictstr.values())
-        listtyp = list(dictstr.keys())
+                    [[4, [5, 6]], {'heure::time': ['10:25:10', {':point': [3, 4]}]}]],
+                   ['NtvList', [], {}],
+                   ['NtvList', {'::': [{'paris': [2.1, 40.3]}, {'lyon': [2.1, 40.3]}]},
+                    {'paris': [2.1, 40.3], 'lyon': [2.1, 40.3]}],
+                   ['NtvList', {'Ntv3::fr.reg': {'Ntv1': 1, 'Ntv2:fr.reg': '2'}},
+                    {'Ntv3::fr.reg': {'Ntv1': 1, 'Ntv2': '2'}}],
+                   ['NtvList', {'Ntv3::fr.reg': {'Ntv1': [1, 2], 'Ntv2:fr.reg': '2'}},
+                    {'Ntv3::fr.reg': {'Ntv1': [1, 2], 'Ntv2': '2'}}],
+        ]
+        lis = list(zip(*dictstr))
+        liststr = list(lis[1])
+        listtyp = list(lis[0])
         for nstr, typ in zip(liststr, listtyp):
             #print('av', nstr, typ)
             ntv = Ntv.from_obj(nstr)
             ntv2 = Ntv.obj(nstr)
             self.assertEqual(ntv, ntv2)
             #print('ap', nstr, typ)
-            if not typ in ['9NtvList', 'aNtvList', 'bNtvList', '9NtvSingle', 'eNtvSingle',
-                           'dNtvSingle', 'fNtvSingle', 'gNtvSingle', 'hNtvSingle',
-                           'iNtvSingle', '4NtvSet', '5NtvSet']:
-                self.assertEqual(nstr, ntv.to_obj())
-            if typ == 'bNtvList':
-                self.assertEqual(nstr['::'], ntv.to_obj())
-            if typ == '4NtvSet':
-                self.assertEqual(
-                    {'ntv3::fr.reg': {'ntv1': 1, 'ntv2': '2'}}, ntv.to_obj())
-            if typ == '5NtvSet':
-                self.assertEqual(
-                    {'ntv3::fr.reg': {'ntv1': [1, 2], 'ntv2': '2'}}, ntv.to_obj())
+            self.assertEqual(nstr, ntv.to_obj())
+            self.assertTrue(ntv.__class__.__name__ == typ)
             self.assertEqual(ntv, Ntv.from_obj(Ntv.to_obj(ntv)))
-            # self.assertEqual(ntv, Ntv.from_obj(
-            #    Ntv.to_obj(ntv, encode_format='cbor')))
-            if not typ in ['9NtvList', 'aNtvList']:
-                self.assertEqual(ntv, Ntv.from_obj(
-                    Ntv.to_obj(ntv, encoded=True)))
-            self.assertTrue(ntv.__class__.__name__ == typ[1:])
+
+        lis = list(zip(*dictstr2))
+        listres = list(lis[2])
+        liststr = list(lis[1])
+        listtyp = list(lis[0])
+        for nstr, typ, nres in zip(liststr, listtyp, listres):
+            #print('av', nstr, typ)
+            ntv = Ntv.from_obj(nstr)
+            ntv2 = Ntv.obj(nstr)
+            self.assertEqual(ntv, ntv2)
+            #print('ap', nstr, typ)
+            self.assertTrue(ntv.__class__.__name__ == typ)
+            self.assertEqual(ntv, Ntv.from_obj(Ntv.to_obj(ntv)))
+            self.assertEqual(nres, ntv.to_obj())
 
     def test_default_type(self):
         list_test = [[('', ':', 'fr.BAN.lon'), {'ntv1::fr.BAN.': [{':BAN.lon': 4}, 5, 6]}],
                      [('', ':', 'fr.BAN.lon'), {
                          'ntv1::fr.BAN.': [{':lon': 4}, 5, 6]}],
                      [('', ':', 'fr.reg'), {'ntv1::fr.': [{':reg': 4}, 5, 6]}],
                      [('', ':', 'fr.reg'), {
                          'ntv1::fr.': [{':fr.reg': 4}, 5, 6]}],
                      [('', ':', 'fr.reg'), {
-                          'ntv1::fr.reg': [{':fr.reg': 4}, 5, 6]}],
+                         'ntv1::fr.reg': [{':fr.reg': 4}, 5, 6]}],
                      [('', ':', 'fr.reg'), {'ntv1::fr.reg': [4, 5, 6]}],
                      [('', ':', 'fr.reg'), {
                          'ntv1::fr.BAN.lon': [{':fr.reg': 4}, 5, 6]}],
                      [('', ':', 'fr.reg'), {'ntv1::fr.BAN.': [{':fr.reg': 4}, 5, 6]}]]
         for test in list_test:
             # print(test[1])
             self.assertEqual(Ntv.from_obj(
-                test[1]).ntv_value[0].obj_name(), test[0])
+                test[1]).ntv_value[0].json_name(), list(test[0]))
             self.assertEqual(
-                Ntv.obj(test[1]).ntv_value[0].obj_name(), test[0])
+                Ntv.obj(test[1]).ntv_value[0].json_name(), list(test[0]))
 
-    def test_defaukt_list(self):
-        unic = NtvSingle({'un':1, 'deux':2}, 'param')
-        lis1 = NtvList([1,2,3,4], 'lis1', 'int')
-        lis2 = NtvList([10,2.5,30,40], 'lis2')
+    def test_default_list(self):
+        unic = NtvSingle({'un': 1, 'deux': 2}, 'param')
+        lis1 = NtvList([1, 2, 3, 4], 'lis1', 'int')
+        lis2 = NtvList([10, 2.5, 30, 40], 'lis2')
         il_lis1 = NtvList([lis1, lis2, unic], 'ilis1')
         il_lis2 = NtvList([lis2, lis1, unic], 'ilis2')
-        self.assertEqual(il_lis2[0].ntv_type, il_lis1[0].ntv_type)
-        self.assertEqual(il_lis2[1].ntv_type, il_lis1[1].ntv_type)
+        self.assertEqual(il_lis2[0].ntv_type, il_lis1[1].ntv_type)
+        self.assertEqual(il_lis2[1].ntv_type, il_lis1[0].ntv_type)
         self.assertNotEqual(il_lis2.ntv_type, il_lis1.ntv_type)
-        
+
     def test_to_obj(self):
         nstr = {'cities': [{'paris': [2.1, 40.3]}, {'lyon': [2.1, 40.3]}]}
-        self.assertEqual(Ntv.from_obj(nstr).to_obj(
-            simpleval=True), [[2.1, 40.3], [2.1, 40.3]])
+        nstr2 = {'cities':  {'paris': [2.1, 40.3],   'lyon': [2.1, 40.3]}}
+        nstr3 = {'cities': [[2.1, 40.3],           [2.1, 40.3]]}
+        self.assertTrue(Ntv.from_obj(nstr).to_obj(simpleval=True) ==
+                        Ntv.from_obj(nstr2).to_obj(simpleval=True) ==
+                        Ntv.from_obj(nstr3).to_obj(simpleval=True) ==
+                        [[2.1, 40.3], [2.1, 40.3]])
+        self.assertEqual(Ntv.obj(nstr), Ntv.obj(nstr2))
+        self.assertEqual(Ntv.obj(nstr).to_obj(json_array=True), nstr)
+        self.assertEqual(Ntv.obj(nstr).to_obj(json_array=False), nstr2)
+        self.assertEqual(Ntv.obj({'paris:point': 'null'}).to_obj(encode_format='obj'),
+                         {'paris:point': None})
+
+    def test_tab(self):
+        tab = Ntv.obj({'index':           [1, 2, 3],
+                       'dates::datetime': ['1964-01-01', '1985-02-05', '2022-01-21'],
+                       'value':           [10, 20, 30],
+                       'value32::int32':  [10, 20, 30],
+                       'res':             {'res1': 10, 'res2': 20, 'res3': 30},
+                       'coord::point':    [[1, 2], [3, 4], [5, 6]],
+                       'names::string':   ['john', 'eric', 'judith']})
+        self.assertEqual(tab[1][2], tab['dates'][2],
+                         Ntv.obj({":datetime": "2022-01-21"}))
+        self.assertEqual(tab[4][2], tab['res']['res3'], Ntv.obj(30))
+
+    def test_tab_field_pandas_ilist_Iindex(self):
+        field = Ntv.obj({':field':
+                         {'dates::datetime': ['1964-01-01', '1985-02-05', '2022-01-21']}})
+        tab = Ntv.obj({':tab':
+                       {'index':           [1, 2, 3],
+                        'dates::datetime': ['1964-01-01', '1985-02-05', '2022-01-21'],
+                        'value':           [10, 20, 30],
+                        'value32::int32':  [10, 20, 30],
+                        'res':             {'res1': 10, 'res2': 20, 'res3': 30},
+                        'coord::point':    [[1, 2], [3, 4], [5, 6]],
+                        'names::string':   ['john', 'eric', 'judith']}})
+        sr = field.to_obj(encode_format='obj', dicobj={
+                          'field': 'SeriesConnec'})
+        df = tab.to_obj(encode_format='obj', dicobj={'tab': 'DataFrameConnec'})
+        #il  = tab.to_obj  (encode_format='obj')
+        #idx = field.to_obj(encode_format='obj')
+        #self.assertEqual(idx, Ntv.obj(idx).to_obj(encode_format='obj'))
+        #self.assertEqual(il, Ntv.obj(il).to_obj(encode_format='obj'))
+        self.assertTrue(df.equals(Ntv.obj(df).to_obj(
+            encode_format='obj', dicobj={'tab': 'DataFrameConnec'})))
+        self.assertTrue(sr.equals(Ntv.obj(sr).to_obj(
+            encode_format='obj', dicobj={'field': 'SeriesConnec'})))
 
-    def test_pandas(self):
-        field = Ntv.obj({':field': 
-                     {'dates::datetime': ['1964-01-01', '1985-02-05', '2022-01-21']}})
-        tab   = Ntv.obj({':tab'  :
-                     {'index':           [1, 2, 3],
-                      'dates::datetime': ['1964-01-01', '1985-02-05', '2022-01-21'], 
-                      'value':           [10, 20, 30],
-                      'value32::int32':  [10, 20, 30],
-                      'coord::point':    [[1,2], [3,4], [5,6]],
-                      'names::string':   ['john', 'eric', 'judith']}})
-        sr = field.to_obj(encode_format='obj', dicobj={'field': 'SeriesConnec'})
-        df = tab.to_obj  (encode_format='obj', dicobj={'tab': 'DataFrameConnec'})
-        self.assertTrue(df.equals(Ntv.obj(df).to_obj(encode_format='obj', dicobj={'tab': 'DataFrameConnec'})))
-        self.assertTrue(sr.equals(Ntv.obj(sr).to_obj(encode_format='obj', dicobj={'field': 'SeriesConnec'})))
-
-    def test_observation(self):
-        field = Ntv.obj({':field': 
-                     {'dates::datetime': ['1964-01-01', '1985-02-05', '2022-01-21']}})
-        tab = { 'index':           [1, 2, 3],
-                'dates::datetime': ['1964-01-01', '1985-02-05', '2022-01-21'], 
-                'value':           [10, 20, 30],
-                'value32::int32':  [10, 20, 30],
-                'coord::point':    [[1,2], [3,4], [5,6]],
-                'names::string':   ['john', 'eric', 'judith']}
-        il   = Ilist.dic(tab)
-        ntv = Ntv.obj( il)
-        self.assertEqual(il, ntv.to_obj(encode_format='obj'))
-        tab_ntv = Ntv.obj({':tab'  : tab})
-        il = tab_ntv.to_obj  (encode_format='obj')
-        self.assertEqual(il, Ntv.obj(il).to_obj(encode_format='obj'))
-
-                          
     def test_csv(self):
-        tab   = Ntv.obj({':tab'  :
-                     {'index':           [1, 2, 3],
-                      'dates::datetime': ['1964-01-01', '1985-02-05', '2022-01-21'], 
-                      'value':           [10, 20, 30],
-                      'value32::int32':  [10, 20, 30],
-                      'coord::point':    [[1,2], [3,4], [5,6]],
-                      'names::string':   ['john', 'eric', 'judith']}})        
+        tab = Ntv.obj({':tab':
+                       {'index':           [1, 2, 3],
+                        'dates::datetime': ['1964-01-01', '1985-02-05', '2022-01-21'],
+                        'value':           [10, 20, 30],
+                        'value32::int32':  [10, 20, 30],
+                        'coord::point':    [[1, 2], [3, 4], [5, 6]],
+                        'names::string':   ['john', 'eric', 'judith']}})
         self.assertEqual(tab, from_csv(to_csv('test.csv', tab)))
-        self.assertEqual(tab, from_csv(to_csv('test.csv', tab, quoting=csv.QUOTE_ALL)))
-        
+        self.assertEqual(tab, from_csv(
+            to_csv('test.csv', tab, quoting=csv.QUOTE_ALL)))
+
+    def test_NtvTree(self):
+        ntv = Ntv.obj({'a': [1, [2, 3, 4], [5, 6]], 'b': 'ert'})
+        tree = NtvTree(ntv)
+        self.assertEqual(tree.nodes[0], tree.ntv)
+        self.assertEqual(
+            [node.address_name for node in tree.leaf_nodes][6], '0.1')
+        self.assertEqual(tree.adjacency_list[ntv][0], ntv[0])
+        self.assertEqual(tree.height, 3)
+        self.assertEqual(tree.size, 11)
+        self.assertEqual(tree.breadth, 7)
+        self.assertEqual(len(tree.inner_nodes), 4)
+
+    def test_iter(self):
+        ntv = Ntv.obj(0)
+        for int, val in enumerate(ntv):
+            self.assertEqual(val, int)
+        ntv = Ntv.obj([0, 1, 2, 3])
+        for int, val in enumerate(ntv):
+            self.assertEqual(val.val, int)
+
+
 if __name__ == '__main__':
     unittest.main(verbosity=2)
```

