# Comparing `tmp/mwsqlite-1.1.1.tar.gz` & `tmp/mwsqlite-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mwsqlite-1.1.1.tar", last modified: Sat Mar 25 19:55:58 2023, max compression
+gzip compressed data, was "dist\mwsqlite-1.2.1.tar", last modified: Wed May 31 05:59:36 2023, max compression
```

## Comparing `mwsqlite-1.1.1.tar` & `mwsqlite-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-25 19:55:58.167092 mwsqlite-1.1.1/
--rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 mwsqlite-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     3172 2023-03-25 19:55:58.168092 mwsqlite-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2075 2022-12-19 15:39:05.000000 mwsqlite-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-25 19:55:58.156089 mwsqlite-1.1.1/mwsqlite/
--rw-rw-rw-   0        0        0      186 2022-12-19 10:39:07.000000 mwsqlite-1.1.1/mwsqlite/__init__.py
--rw-rw-rw-   0        0        0     1513 2022-12-23 17:48:52.000000 mwsqlite-1.1.1/mwsqlite/_types.py
--rw-rw-rw-   0        0        0    12136 2023-03-25 19:53:26.000000 mwsqlite-1.1.1/mwsqlite/mw_sql.py
--rw-rw-rw-   0        0        0     3388 2022-12-23 15:06:08.000000 mwsqlite-1.1.1/mwsqlite/sql_compile.py
--rw-rw-rw-   0        0        0      551 2022-12-23 17:48:26.000000 mwsqlite-1.1.1/mwsqlite/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-25 19:55:58.166092 mwsqlite-1.1.1/mwsqlite.egg-info/
--rw-rw-rw-   0        0        0     3172 2023-03-25 19:55:57.000000 mwsqlite-1.1.1/mwsqlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-03-25 19:55:58.000000 mwsqlite-1.1.1/mwsqlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-25 19:55:57.000000 mwsqlite-1.1.1/mwsqlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-25 19:55:57.000000 mwsqlite-1.1.1/mwsqlite.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-03-25 19:55:57.000000 mwsqlite-1.1.1/mwsqlite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-25 19:55:58.169093 mwsqlite-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1666 2023-03-25 19:53:47.000000 mwsqlite-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:59:36.539919 mwsqlite-1.2.1/
+-rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 mwsqlite-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3172 2023-05-31 05:59:36.539919 mwsqlite-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2075 2022-12-19 15:39:05.000000 mwsqlite-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 05:59:36.526284 mwsqlite-1.2.1/mwsqlite/
+-rw-rw-rw-   0        0        0      186 2022-12-19 10:39:07.000000 mwsqlite-1.2.1/mwsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1513 2022-12-23 17:48:52.000000 mwsqlite-1.2.1/mwsqlite/_types.py
+-rw-rw-rw-   0        0        0    14614 2023-05-31 05:56:49.000000 mwsqlite-1.2.1/mwsqlite/mw_sql.py
+-rw-rw-rw-   0        0        0     3388 2022-12-23 15:06:08.000000 mwsqlite-1.2.1/mwsqlite/sql_compile.py
+-rw-rw-rw-   0        0        0      551 2022-12-23 17:48:26.000000 mwsqlite-1.2.1/mwsqlite/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:59:36.538904 mwsqlite-1.2.1/mwsqlite.egg-info/
+-rw-rw-rw-   0        0        0     3172 2023-05-31 05:59:36.000000 mwsqlite-1.2.1/mwsqlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-05-31 05:59:36.000000 mwsqlite-1.2.1/mwsqlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 05:59:36.000000 mwsqlite-1.2.1/mwsqlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-31 05:59:36.000000 mwsqlite-1.2.1/mwsqlite.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-05-31 05:59:36.000000 mwsqlite-1.2.1/mwsqlite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 05:59:36.540919 mwsqlite-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1666 2023-05-31 05:59:17.000000 mwsqlite-1.2.1/setup.py
```

### Comparing `mwsqlite-1.1.1/LICENSE` & `mwsqlite-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.1.1/PKG-INFO` & `mwsqlite-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mwsqlite
-Version: 1.1.1
+Version: 1.2.1
 Summary: Simply python library for interact with (EOSIO) WAX blockchain
 Home-page: https://github.com/makarworld/mwsqlite.git
-Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.1.1.zip
+Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.2.1.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mwsqlite-1.1.1/README.md` & `mwsqlite-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.1.1/mwsqlite/_types.py` & `mwsqlite-1.2.1/mwsqlite/_types.py`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.1.1/mwsqlite/mw_sql.py` & `mwsqlite-1.2.1/mwsqlite/mw_sql.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from __future__ import annotations
 import json
 # This Python file uses the following encoding: utf-8
 import sqlite3
 
-from ._types import Struct, Where, Order, InvalidColumnNameError, DESC, ASC, Limit
-from .utils import tuple_to_dict
-from .sql_compile import SQLCompile
+try:
+    from ._types import Struct, Where, Order, InvalidColumnNameError, DESC, ASC, Limit
+    from .utils import tuple_to_dict
+    from .sql_compile import SQLCompile
+except:
+    from _types import Struct, Where, Order, InvalidColumnNameError, DESC, ASC, Limit
+    from utils import tuple_to_dict
+    from sql_compile import SQLCompile
 
 def ensure_connection(func):
     def inner(*args, **kwargs):
         if (isinstance(args[0], MWBase) or isinstance(args[0], Table)) and func.__name__ != "__init__": # take var in self if you use class methods
             file = args[0].filename
 
         elif kwargs.get("filename"): # take var in kwargs if you use __init__ function with kwarg "filename"
@@ -91,14 +96,23 @@
     def __str__(self):
         return self.__repr__()
     
     def __repr__(self):
         return f"MWBase.{self.table}"
 
     @ensure_connection
+    def _execute(self, cmd, values, fetchall = False, cursor=None) -> None:
+        cursor.execute(cmd, values)
+        if fetchall:
+            return cursor.fetchall()
+
+    def execute(self, cmd, values = None, fetchall = False):
+        return self._execute(cmd, values, fetchall)
+
+    @ensure_connection
     def add(self, cursor=None, **kwargs) -> None:
         """
         Add new row to table.
         """
         kwargs = check_kwargs(kwargs)
 
         cmd = SQLCompile.insert(self.table, kwargs.keys())
@@ -248,15 +262,62 @@
     
     @ensure_connection
     def get_last(self, cursor=None, **kwargs) -> Row | None:
         """
         Get last row with parameters from table.
         """
         return self.get_one(default_index=-1, **kwargs)
+    @ensure_connection
+    def get_like(self, where: Where = Where(), order: Order = Order(), return_index: int = None, cursor=None, **kwargs) -> list[Row]:
+        
+        if isinstance(order, Where) and isinstance(where, Order):
+            order, where = where, order
+
+        elif isinstance(order, Where) and isinstance(where, Where): 
+            where.update(order)
+            order = Order()
+
+        elif isinstance(order, Order) and isinstance(where, Order):
+            order.update(where)
+            where = Where()
 
+        if where: kwargs.update(where)
+
+        
+        if not all([k in self.columns.keys() and v in [DESC, ASC] for k, v in order.items()]):
+            raise InvalidColumnNameError("Order keys must be in columns keys and values must be DESC or ASC")
+
+        if where:
+            kwargs.update(where)
+
+        cmd = SQLCompile.select(
+            table=self.table, 
+            where=[
+                f"{column} { ('LIKE') } ?" 
+                for column, data in kwargs.items()] if kwargs else ["NONE"], 
+            order=[
+                f'{column} {data}' 
+            for column, data in order.items()] if order else ["NONE"],
+        )
+        values = tuple(map(str, kwargs.values()))
+
+        cursor.execute(cmd, values)
+        items = cursor.fetchall()
+
+        if not items: return None
+
+        if not return_index:
+            resp = []
+            for item in items:
+                resp.append(Row(self, **tuple_to_dict(item, self.columns)))
+        else:
+            resp = tuple_to_dict(item[return_index], self.columns)
+            resp = Row(self, **resp)
+
+        return resp
 
     @ensure_connection
     def update(self, where: Where, cursor=None, **kwargs) -> None:
         """
         Update rows in table.
         """
         kwargs = check_kwargs(kwargs)
@@ -375,21 +436,28 @@
                 "first_name": str,
                 "age": int
             }
         }
     )
 
     base.users.add(first_name="John", age=20)
+    base.users.add(first_name="Jack", age=20)
+    base.users.add(first_name="Joice", age=20)
+    base.users.add(first_name="Jumba", age=20)
+    base.users.add(first_name="Jamba", age=20)
 
-    user = base.users.get_one(first_name="John")
-    user.update(first_name="Jack", age=21)
+    #user = base.users.get_one(first_name="John")
+    #user.update(first_name="Jack", age=21)
 
-    user2 = base.users.get_one(first_name="Jack")
+    #user2 = base.users.get_one(first_name="Jack")
     
-    print(user) # user and user2 are the same object
-    print(user2)
+    #print(user) # user and user2 are the same object
+    #print(user2)
+
+    users = base.users.get_like(first_name="Joh%")
+    print(users)
 
-    user.delete()
+    [user.delete() for user in users]
 
     # UPDATE test SET test1 = ?, test2 = ? WHERE test1 = ? AND test2 = ? ['name2', 'name3', 'name1', 'name3']
```

### Comparing `mwsqlite-1.1.1/mwsqlite/sql_compile.py` & `mwsqlite-1.2.1/mwsqlite/sql_compile.py`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.1.1/mwsqlite/utils.py` & `mwsqlite-1.2.1/mwsqlite/utils.py`

 * *Files identical despite different names*

### Comparing `mwsqlite-1.1.1/mwsqlite.egg-info/PKG-INFO` & `mwsqlite-1.2.1/mwsqlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mwsqlite
-Version: 1.1.1
+Version: 1.2.1
 Summary: Simply python library for interact with (EOSIO) WAX blockchain
 Home-page: https://github.com/makarworld/mwsqlite.git
-Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.1.1.zip
+Download-URL: https://github.com/makarworld/mwsqlite/archive/refs/tags/v1.2.1.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mwsqlite-1.1.1/setup.py` & `mwsqlite-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 :author: abuztrade
 :license: MIT License, see LICENSE file.
 :copyright: (c) 2022 by abuztrade.
 """
 
 
-version = '1.1.1'
+version = '1.2.1'
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="mwsqlite",
     version=version,
```

