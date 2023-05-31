# Comparing `tmp/vadvergasov_serialization-1.0.0.tar.gz` & `tmp/vadvergasov_serialization-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vadvergasov_serialization-1.0.0.tar", last modified: Tue May 30 21:20:45 2023, max compression
+gzip compressed data, was "vadvergasov_serialization-1.1.0.tar", last modified: Wed May 31 13:16:29 2023, max compression
```

## Comparing `vadvergasov_serialization-1.0.0.tar` & `vadvergasov_serialization-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 21:20:45.347238 vadvergasov_serialization-1.0.0/
--rw-rw-rw-   0        0        0    35820 2023-04-29 17:53:07.000000 vadvergasov_serialization-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      475 2023-05-30 21:20:45.346239 vadvergasov_serialization-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-30 21:20:45.316234 vadvergasov_serialization-1.0.0/serializer/
--rw-rw-rw-   0        0        0       63 2023-05-30 21:07:38.000000 vadvergasov_serialization-1.0.0/serializer/__init__.py
--rw-rw-rw-   0        0        0     1820 2023-05-30 16:48:50.000000 vadvergasov_serialization-1.0.0/serializer/__main__.py
--rw-rw-rw-   0        0        0     1852 2023-05-30 21:15:43.000000 vadvergasov_serialization-1.0.0/serializer/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-30 21:20:45.319240 vadvergasov_serialization-1.0.0/serializer/factory/
--rw-rw-rw-   0        0        0      110 2023-05-30 21:05:59.000000 vadvergasov_serialization-1.0.0/serializer/factory/__init__.py
--rw-rw-rw-   0        0        0      488 2023-05-28 17:18:22.000000 vadvergasov_serialization-1.0.0/serializer/factory/factory.py
-drwxrwxrwx   0        0        0        0 2023-05-30 21:20:45.323242 vadvergasov_serialization-1.0.0/serializer/factory/parsers/
--rw-rw-rw-   0        0        0      218 2023-05-30 17:11:14.000000 vadvergasov_serialization-1.0.0/serializer/factory/parsers/__init__.py
--rw-rw-rw-   0        0        0       87 2023-05-28 17:17:04.000000 vadvergasov_serialization-1.0.0/serializer/factory/parsers/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-30 21:20:45.326240 vadvergasov_serialization-1.0.0/serializer/factory/parsers/json/
--rw-rw-rw-   0        0        0       95 2023-05-30 17:11:26.000000 vadvergasov_serialization-1.0.0/serializer/factory/parsers/json/__init__.py
--rw-rw-rw-   0        0        0     3176 2023-05-30 21:11:56.000000 vadvergasov_serialization-1.0.0/serializer/factory/parsers/json/parser.py
--rw-rw-rw-   0        0        0      735 2023-05-30 20:54:38.000000 vadvergasov_serialization-1.0.0/serializer/factory/parsers/parser.py
-drwxrwxrwx   0        0        0        0 2023-05-30 21:20:45.330243 vadvergasov_serialization-1.0.0/serializer/factory/parsers/xml/
--rw-rw-rw-   0        0        0       92 2023-05-30 17:11:37.000000 vadvergasov_serialization-1.0.0/serializer/factory/parsers/xml/__init__.py
--rw-rw-rw-   0        0        0     3800 2023-05-30 21:03:53.000000 vadvergasov_serialization-1.0.0/serializer/factory/parsers/xml/parser.py
-drwxrwxrwx   0        0        0        0 2023-05-30 21:20:45.335237 vadvergasov_serialization-1.0.0/serializer/serializer/
--rw-rw-rw-   0        0        0      118 2023-05-30 21:00:49.000000 vadvergasov_serialization-1.0.0/serializer/serializer/__init__.py
--rw-rw-rw-   0        0        0     4148 2023-05-30 20:44:41.000000 vadvergasov_serialization-1.0.0/serializer/serializer/deserializer.py
--rw-rw-rw-   0        0        0     5470 2023-05-30 20:39:27.000000 vadvergasov_serialization-1.0.0/serializer/serializer/serializer.py
--rw-rw-rw-   0        0        0       42 2023-05-30 21:20:45.347238 vadvergasov_serialization-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      648 2023-05-30 21:20:25.000000 vadvergasov_serialization-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 21:20:45.336246 vadvergasov_serialization-1.0.0/tests/
--rw-rw-rw-   0        0        0     5406 2023-05-29 16:53:14.000000 vadvergasov_serialization-1.0.0/tests/test_serialization.py
-drwxrwxrwx   0        0        0        0 2023-05-30 21:20:45.345236 vadvergasov_serialization-1.0.0/vadvergasov_serialization.egg-info/
--rw-rw-rw-   0        0        0      475 2023-05-30 21:20:45.000000 vadvergasov_serialization-1.0.0/vadvergasov_serialization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2023-05-30 21:20:45.000000 vadvergasov_serialization-1.0.0/vadvergasov_serialization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 21:20:45.000000 vadvergasov_serialization-1.0.0/vadvergasov_serialization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-30 21:20:45.000000 vadvergasov_serialization-1.0.0/vadvergasov_serialization.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-30 21:20:45.000000 vadvergasov_serialization-1.0.0/vadvergasov_serialization.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 13:16:29.118052 vadvergasov_serialization-1.1.0/
+-rw-rw-rw-   0        0        0    35820 2023-05-30 12:44:21.000000 vadvergasov_serialization-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      500 2023-05-31 13:16:29.114075 vadvergasov_serialization-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-31 13:16:28.976055 vadvergasov_serialization-1.1.0/serializer/
+-rw-rw-rw-   0        0        0       63 2023-05-31 12:54:05.000000 vadvergasov_serialization-1.1.0/serializer/__init__.py
+-rw-rw-rw-   0        0        0     1820 2023-05-31 12:54:05.000000 vadvergasov_serialization-1.1.0/serializer/__main__.py
+-rw-rw-rw-   0        0        0     1898 2023-05-31 13:04:59.000000 vadvergasov_serialization-1.1.0/serializer/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-31 13:16:28.987054 vadvergasov_serialization-1.1.0/serializer/factory/
+-rw-rw-rw-   0        0        0      110 2023-05-31 12:54:05.000000 vadvergasov_serialization-1.1.0/serializer/factory/__init__.py
+-rw-rw-rw-   0        0        0      488 2023-05-30 12:44:21.000000 vadvergasov_serialization-1.1.0/serializer/factory/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-31 13:16:29.003056 vadvergasov_serialization-1.1.0/serializer/factory/parsers/
+-rw-rw-rw-   0        0        0      218 2023-05-31 12:54:05.000000 vadvergasov_serialization-1.1.0/serializer/factory/parsers/__init__.py
+-rw-rw-rw-   0        0        0       87 2023-05-30 12:44:21.000000 vadvergasov_serialization-1.1.0/serializer/factory/parsers/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-31 13:16:29.026056 vadvergasov_serialization-1.1.0/serializer/factory/parsers/json/
+-rw-rw-rw-   0        0        0       95 2023-05-31 12:54:05.000000 vadvergasov_serialization-1.1.0/serializer/factory/parsers/json/__init__.py
+-rw-rw-rw-   0        0        0     3176 2023-05-31 12:54:05.000000 vadvergasov_serialization-1.1.0/serializer/factory/parsers/json/parser.py
+-rw-rw-rw-   0        0        0      735 2023-05-31 12:54:05.000000 vadvergasov_serialization-1.1.0/serializer/factory/parsers/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-31 13:16:29.040057 vadvergasov_serialization-1.1.0/serializer/factory/parsers/xml/
+-rw-rw-rw-   0        0        0       92 2023-05-31 12:54:05.000000 vadvergasov_serialization-1.1.0/serializer/factory/parsers/xml/__init__.py
+-rw-rw-rw-   0        0        0     3800 2023-05-31 12:54:05.000000 vadvergasov_serialization-1.1.0/serializer/factory/parsers/xml/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-31 13:16:29.054055 vadvergasov_serialization-1.1.0/serializer/serializer/
+-rw-rw-rw-   0        0        0      118 2023-05-31 12:54:05.000000 vadvergasov_serialization-1.1.0/serializer/serializer/__init__.py
+-rw-rw-rw-   0        0        0     4148 2023-05-31 12:54:05.000000 vadvergasov_serialization-1.1.0/serializer/serializer/deserializer.py
+-rw-rw-rw-   0        0        0     5470 2023-05-31 12:54:05.000000 vadvergasov_serialization-1.1.0/serializer/serializer/serializer.py
+-rw-rw-rw-   0        0        0       42 2023-05-31 13:16:29.119054 vadvergasov_serialization-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      679 2023-05-31 13:14:51.000000 vadvergasov_serialization-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 13:16:29.058054 vadvergasov_serialization-1.1.0/tests/
+-rw-rw-rw-   0        0        0     5732 2023-05-31 13:09:16.000000 vadvergasov_serialization-1.1.0/tests/test_serialization.py
+drwxrwxrwx   0        0        0        0 2023-05-31 13:16:29.110053 vadvergasov_serialization-1.1.0/vadvergasov_serialization.egg-info/
+-rw-rw-rw-   0        0        0      500 2023-05-31 13:16:28.000000 vadvergasov_serialization-1.1.0/vadvergasov_serialization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2023-05-31 13:16:28.000000 vadvergasov_serialization-1.1.0/vadvergasov_serialization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 13:16:28.000000 vadvergasov_serialization-1.1.0/vadvergasov_serialization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-31 13:16:28.000000 vadvergasov_serialization-1.1.0/vadvergasov_serialization.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-31 13:16:28.000000 vadvergasov_serialization-1.1.0/vadvergasov_serialization.egg-info/top_level.txt
```

### Comparing `vadvergasov_serialization-1.0.0/LICENSE` & `vadvergasov_serialization-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vadvergasov_serialization-1.0.0/serializer/__main__.py` & `vadvergasov_serialization-1.1.0/serializer/__main__.py`

 * *Files identical despite different names*

### Comparing `vadvergasov_serialization-1.0.0/serializer/constants.py` & `vadvergasov_serialization-1.1.0/serializer/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,18 @@
     "co_flags",
     "co_code",
     "co_consts",
     "co_names",
     "co_varnames",
     "co_filename",
     "co_name",
+    "co_qualname",
     "co_firstlineno",
     "co_lnotab",
+    "co_exceptiontable",
     "co_freevars",
     "co_cellvars",
 )
 
 IGNORED_CLASS_ATTRIBUTES = ("__name__", "__base__", "__basicsize__", "__dictoffset__", "__class__")
 
 IGNORED_TYPES = (
```

### Comparing `vadvergasov_serialization-1.0.0/serializer/factory/parsers/json/parser.py` & `vadvergasov_serialization-1.1.0/serializer/factory/parsers/json/parser.py`

 * *Files identical despite different names*

### Comparing `vadvergasov_serialization-1.0.0/serializer/factory/parsers/parser.py` & `vadvergasov_serialization-1.1.0/serializer/factory/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `vadvergasov_serialization-1.0.0/serializer/factory/parsers/xml/parser.py` & `vadvergasov_serialization-1.1.0/serializer/factory/parsers/xml/parser.py`

 * *Files identical despite different names*

### Comparing `vadvergasov_serialization-1.0.0/serializer/serializer/deserializer.py` & `vadvergasov_serialization-1.1.0/serializer/serializer/deserializer.py`

 * *Files identical despite different names*

### Comparing `vadvergasov_serialization-1.0.0/serializer/serializer/serializer.py` & `vadvergasov_serialization-1.1.0/serializer/serializer/serializer.py`

 * *Files identical despite different names*

### Comparing `vadvergasov_serialization-1.0.0/setup.py` & `vadvergasov_serialization-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="vadvergasov_serialization",
-    version="1.0.0",
+    version="1.1.0",
     description="Serialization library",
     url="https://github.com/VadVergasov/SCCS",
     author="VadVergasov",
     author_email="vadim.vergasov2003@gmail.com",
     license="GNU GPLv3",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(),
     include_package_data=True,
     install_requires=["regex"],
+     python_requires="==3.11"
 )
```

### Comparing `vadvergasov_serialization-1.0.0/tests/test_serialization.py` & `vadvergasov_serialization-1.1.0/tests/test_serialization.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,224 +1,234 @@
 from constants import *
-from serializer.serializer.serializer import Serializer
+from serializer.serializer import Serializer, Deserializer
 
 
 def test_primitive_1():
-    assert a == Serializer.deserialize(Serializer.serialize(a))
+    assert a == Deserializer.deserialize(Serializer.serialize(a))
 
 
 def test_primitive_2():
-    assert aa == Serializer.deserialize(Serializer.serialize(aa))
+    assert aa == Deserializer.deserialize(Serializer.serialize(aa))
 
 
 def test_primitive_3():
-    assert b == Serializer.deserialize(Serializer.serialize(b))
+    assert b == Deserializer.deserialize(Serializer.serialize(b))
 
 
 def test_primitive_4():
-    assert bb == Serializer.deserialize(Serializer.serialize(bb))
+    assert bb == Deserializer.deserialize(Serializer.serialize(bb))
 
 
 def test_primitive_5():
-    assert c == Serializer.deserialize(Serializer.serialize(c))
+    assert c == Deserializer.deserialize(Serializer.serialize(c))
 
 
 def test_primitive_6():
-    assert cc == Serializer.deserialize(Serializer.serialize(cc))
+    assert cc == Deserializer.deserialize(Serializer.serialize(cc))
 
 
 def test_primitive_7():
-    assert d == Serializer.deserialize(Serializer.serialize(d))
+    assert d == Deserializer.deserialize(Serializer.serialize(d))
 
 
 def test_primitive_8():
-    assert dd == Serializer.deserialize(Serializer.serialize(dd))
+    assert dd == Deserializer.deserialize(Serializer.serialize(dd))
 
 
 def test_primitive_9():
-    assert e == Serializer.deserialize(Serializer.serialize(e))
+    assert e == Deserializer.deserialize(Serializer.serialize(e))
 
 
 def test_primitive_10():
-    assert f == Serializer.deserialize(Serializer.serialize(f))
+    assert f == Deserializer.deserialize(Serializer.serialize(f))
 
 
 def test_collection_1():
-    assert list1 == Serializer.deserialize(Serializer.serialize(list1))
+    assert list1 == Deserializer.deserialize(Serializer.serialize(list1))
 
 
 def test_collection_2():
-    assert list2 == Serializer.deserialize(Serializer.serialize(list2))
+    assert list2 == Deserializer.deserialize(Serializer.serialize(list2))
 
 
 def test_collection_3():
-    assert list3 == Serializer.deserialize(Serializer.serialize(list3))
+    assert list3 == Deserializer.deserialize(Serializer.serialize(list3))
 
 
 def test_collection_4():
-    assert tuple1 == Serializer.deserialize(Serializer.serialize(tuple1))
+    assert tuple1 == Deserializer.deserialize(Serializer.serialize(tuple1))
 
 
 def test_collection_4():
-    assert tuple2 == Serializer.deserialize(Serializer.serialize(tuple2))
+    assert tuple2 == Deserializer.deserialize(Serializer.serialize(tuple2))
 
 
 def test_collection_6():
-    assert tuple3 == Serializer.deserialize(Serializer.serialize(tuple3))
+    assert tuple3 == Deserializer.deserialize(Serializer.serialize(tuple3))
 
 
 def test_collection_7():
-    assert bytes1 == Serializer.deserialize(Serializer.serialize(bytes1))
+    assert bytes1 == Deserializer.deserialize(Serializer.serialize(bytes1))
 
 
 def test_collection_8():
-    assert dict1 == Serializer.deserialize(Serializer.serialize(dict1))
+    assert dict1 == Deserializer.deserialize(Serializer.serialize(dict1))
 
 
 def test_collection_9():
-    assert dict2 == Serializer.deserialize(Serializer.serialize(dict2))
+    assert dict2 == Deserializer.deserialize(Serializer.serialize(dict2))
 
 
 def test_collection_10():
-    assert dict3 == Serializer.deserialize(Serializer.serialize(dict3))
+    assert dict3 == Deserializer.deserialize(Serializer.serialize(dict3))
 
 
 def test_collection_11():
-    assert dict4 == Serializer.deserialize(Serializer.serialize(dict4))
+    assert dict4 == Deserializer.deserialize(Serializer.serialize(dict4))
 
 
 def test_collection_12():
-    assert dict5 == Serializer.deserialize(Serializer.serialize(dict5))
+    assert dict5 == Deserializer.deserialize(Serializer.serialize(dict5))
 
 
 def test_func_1():
-    assert func1() == Serializer.deserialize(Serializer.serialize(func1))()
+    assert func1() == Deserializer.deserialize(Serializer.serialize(func1))()
 
 
 def test_func_2():
-    assert func2(12) == Serializer.deserialize(Serializer.serialize(func2))(12)
+    assert func2(12) == Deserializer.deserialize(Serializer.serialize(func2))(12)
 
 
 def test_func_3():
-    assert func3(12) == Serializer.deserialize(Serializer.serialize(func3))(12)
+    assert func3(12) == Deserializer.deserialize(Serializer.serialize(func3))(12)
 
 
 def test_func_4():
-    assert func3(12, 12, 12, 12, 12) == Serializer.deserialize(Serializer.serialize(func3))(12, 12, 12, 12, 12)
+    assert func3(12, 12, 12, 12, 12) == Deserializer.deserialize(Serializer.serialize(func3))(12, 12, 12, 12, 12)
 
 
 def test_func_5():
-    assert func4(0.5) == Serializer.deserialize(Serializer.serialize(func4))(0.5)
+    assert func4(0.5) == Deserializer.deserialize(Serializer.serialize(func4))(0.5)
 
 
 def test_func_6():
-    assert func5([4, 3, 2, 1]) == Serializer.deserialize(Serializer.serialize(func5))([4, 3, 2, 1])
+    assert func5([4, 3, 2, 1]) == Deserializer.deserialize(Serializer.serialize(func5))([4, 3, 2, 1])
 
 
 def test_func_7():
-    assert func6(5) == Serializer.deserialize(Serializer.serialize(func6))(5)
+    assert func6(5) == Deserializer.deserialize(Serializer.serialize(func6))(5)
 
 
 def test_func_8():
-    assert func7(5) == Serializer.deserialize(Serializer.serialize(func7))(5)
+    assert func7(5) == Deserializer.deserialize(Serializer.serialize(func7))(5)
 
 
 def test_func_9():
-    tmp = Serializer.deserialize(Serializer.serialize(lambda1))
+    tmp = Deserializer.deserialize(Serializer.serialize(lambda1))
 
     assert tmp(5) == lambda1(5)
 
 
 def test_func_10():
-    tmp = Serializer.deserialize(Serializer.serialize(lambda2))
+    tmp = Deserializer.deserialize(Serializer.serialize(lambda2))
 
     assert tmp(1, 2, 3) == lambda2(3, 2, 1)
 
 
 def test_class_1():
-    tmp = Serializer.deserialize(Serializer.serialize(A))
+    tmp = Deserializer.deserialize(Serializer.serialize(A))
     tmp = tmp()
     a = A()
 
     assert a.a == tmp.a
     assert a.qwe(2) == tmp.qwe(2)
 
 
 def test_class_2():
-    tmp = Serializer.deserialize(Serializer.serialize(B))
+    tmp = Deserializer.deserialize(Serializer.serialize(B))
     tmp = tmp(2)
     b = B(2)
 
     assert tmp.a == b.a
     assert tmp.func() == b.func()
     assert tmp.qwe(4) == b.qwe(4)
 
 
 def test_class_3():
-    tmp = Serializer.deserialize(Serializer.serialize(EEEE))
+    tmp = Deserializer.deserialize(Serializer.serialize(EEEE))
     tmp = tmp()
     eeee = EEEE()
 
     assert tmp.e == eeee.e
     assert tmp.ee == eeee.ee
     assert tmp.eee == eeee.eee
     assert tmp.eeee == eeee.eeee
 
 
 def test_class_4():
-    tmp = Serializer.deserialize(Serializer.serialize(first))
+    tmp = Deserializer.deserialize(Serializer.serialize(first))
     f = tmp()
 
-    tmp = Serializer.deserialize(Serializer.serialize(second))
+    tmp = Deserializer.deserialize(Serializer.serialize(second))
     s = tmp()
     so = second()
 
     assert s.func(4) == so.func(4)
     assert f.func(4) ** 4 == s.func(4)
 
 
 def test_class_object_1():
     a = A()
-    tmp = Serializer.deserialize(Serializer.serialize(a))
+    tmp = Deserializer.deserialize(Serializer.serialize(a))
 
     assert tmp.a == a.a
     assert tmp.qwe(4) == a.qwe(4)
 
 
 def test_class_5():
-    tmp = Serializer.deserialize(Serializer.serialize(st))
+    tmp = Deserializer.deserialize(Serializer.serialize(st))
 
     assert tmp.qwe() == st.qwe()
 
 
 def test_class_6():
-    tmp = Serializer.deserialize(Serializer.serialize(HardClass))
+    tmp = Deserializer.deserialize(Serializer.serialize(HardClass))
 
     h = HardClass()
     tmp = tmp()
 
     assert tmp.a == h.a
     assert tmp.s == h.s
     assert tmp.func(1, 2) == h.func(1, 2)
 
     assert tmp.c == h.c
     assert tmp.func1(1, 2, 3, 4) == h.func1(1, 2, 3, 4)
     assert tmp.func2(5) == h.func2(5)
 
 
 def test_multiple_inheritance():
-    tmp = Serializer.deserialize(Serializer.serialize(CCCC))
+    tmp = Deserializer.deserialize(Serializer.serialize(CCCC))
     c = CCCC()
     tmp = tmp()
 
     assert c.a == tmp.a
     assert c.b == tmp.b
     assert c.c == tmp.c
 
 
 def test_decorator():
-    tmp = Serializer.deserialize(Serializer.serialize(raise_if_to_many_args))
+    tmp = Deserializer.deserialize(Serializer.serialize(raise_if_to_many_args))
     tmp = tmp(sum_func)
 
     f = raise_if_to_many_args(sum_func)
 
     assert f(1, 2, 3) == tmp(1, 2, 3)
+
+def test_recursion():
+    tmp = Deserializer.deserialize(Serializer.serialize(fact))
+
+    assert 24 == tmp(4)
+
+def test_lambda():
+    tmp = Deserializer.deserialize(Serializer.serialize(lambda x: x**3))
+
+    assert 27 == tmp(3)
```

### Comparing `vadvergasov_serialization-1.0.0/vadvergasov_serialization.egg-info/SOURCES.txt` & `vadvergasov_serialization-1.1.0/vadvergasov_serialization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

