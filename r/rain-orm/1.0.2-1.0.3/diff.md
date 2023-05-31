# Comparing `tmp/rain_orm-1.0.2.tar.gz` & `tmp/rain_orm-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rain_orm-1.0.2.tar", last modified: Wed May 31 04:15:05 2023, max compression
+gzip compressed data, was "rain_orm-1.0.3.tar", last modified: Wed May 31 18:11:26 2023, max compression
```

## Comparing `rain_orm-1.0.2.tar` & `rain_orm-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 04:15:05.643228 rain_orm-1.0.2/
--rw-rw-rw-   0        0        0    11555 2023-05-28 17:49:39.000000 rain_orm-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2951 2023-05-31 04:15:05.643228 rain_orm-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2696 2023-05-31 03:53:53.000000 rain_orm-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 04:15:05.623705 rain_orm-1.0.2/rain_orm/
--rw-rw-rw-   0        0        0      137 2023-05-31 02:13:13.000000 rain_orm-1.0.2/rain_orm/__init__.py
--rw-rw-rw-   0        0        0      311 2023-05-29 18:48:08.000000 rain_orm-1.0.2/rain_orm/common.py
--rw-rw-rw-   0        0        0      781 2023-05-30 18:06:06.000000 rain_orm-1.0.2/rain_orm/db.py
-drwxrwxrwx   0        0        0        0 2023-05-31 04:15:05.633312 rain_orm-1.0.2/rain_orm/error/
--rw-rw-rw-   0        0        0      153 2023-05-30 17:55:36.000000 rain_orm-1.0.2/rain_orm/error/__init__.py
--rw-rw-rw-   0        0        0      283 2023-05-30 16:40:48.000000 rain_orm-1.0.2/rain_orm/error/error.py
-drwxrwxrwx   0        0        0        0 2023-05-31 04:15:05.637732 rain_orm-1.0.2/rain_orm/sql_builder/
--rw-rw-rw-   0        0        0      178 2023-05-30 17:56:14.000000 rain_orm-1.0.2/rain_orm/sql_builder/__init__.py
--rw-rw-rw-   0        0        0       29 2023-05-30 17:52:43.000000 rain_orm-1.0.2/rain_orm/sql_builder/ddl_builder.py
--rw-rw-rw-   0        0        0     5961 2023-05-30 17:43:33.000000 rain_orm-1.0.2/rain_orm/sql_builder/dmldql_builder.py
--rw-rw-rw-   0        0        0     6030 2023-05-31 04:08:56.000000 rain_orm-1.0.2/rain_orm/table.py
-drwxrwxrwx   0        0        0        0 2023-05-31 04:15:05.631015 rain_orm-1.0.2/rain_orm.egg-info/
--rw-rw-rw-   0        0        0     2951 2023-05-31 04:15:05.000000 rain_orm-1.0.2/rain_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-05-31 04:15:05.000000 rain_orm-1.0.2/rain_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 04:15:05.000000 rain_orm-1.0.2/rain_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-31 04:15:05.000000 rain_orm-1.0.2/rain_orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-31 04:15:05.000000 rain_orm-1.0.2/rain_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-31 04:15:05.644621 rain_orm-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      441 2023-05-31 03:58:42.000000 rain_orm-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 04:15:05.641925 rain_orm-1.0.2/tests/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:46:43.000000 rain_orm-1.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0       19 2023-05-31 01:50:35.000000 rain_orm-1.0.2/tests/test_db.py
+drwxrwxrwx   0        0        0        0 2023-05-31 18:11:26.511297 rain_orm-1.0.3/
+-rw-rw-rw-   0        0        0    11555 2023-05-28 17:49:39.000000 rain_orm-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3049 2023-05-31 18:11:26.512316 rain_orm-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2768 2023-05-31 18:03:33.000000 rain_orm-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 18:11:26.494241 rain_orm-1.0.3/rain_orm/
+-rw-rw-rw-   0        0        0      139 2023-05-31 18:07:58.000000 rain_orm-1.0.3/rain_orm/__init__.py
+-rw-rw-rw-   0        0        0      311 2023-05-29 18:48:08.000000 rain_orm-1.0.3/rain_orm/common.py
+-rw-rw-rw-   0        0        0      781 2023-05-30 18:06:06.000000 rain_orm-1.0.3/rain_orm/db.py
+drwxrwxrwx   0        0        0        0 2023-05-31 18:11:26.505288 rain_orm-1.0.3/rain_orm/error/
+-rw-rw-rw-   0        0        0      153 2023-05-30 17:55:36.000000 rain_orm-1.0.3/rain_orm/error/__init__.py
+-rw-rw-rw-   0        0        0      283 2023-05-30 16:40:48.000000 rain_orm-1.0.3/rain_orm/error/error.py
+drwxrwxrwx   0        0        0        0 2023-05-31 18:11:26.509286 rain_orm-1.0.3/rain_orm/sql_builder/
+-rw-rw-rw-   0        0        0      178 2023-05-30 17:56:14.000000 rain_orm-1.0.3/rain_orm/sql_builder/__init__.py
+-rw-rw-rw-   0        0        0       29 2023-05-30 17:52:43.000000 rain_orm-1.0.3/rain_orm/sql_builder/ddl_builder.py
+-rw-rw-rw-   0        0        0     5961 2023-05-30 17:43:33.000000 rain_orm-1.0.3/rain_orm/sql_builder/dmldql_builder.py
+-rw-rw-rw-   0        0        0     5918 2023-05-31 18:02:57.000000 rain_orm-1.0.3/rain_orm/table.py
+drwxrwxrwx   0        0        0        0 2023-05-31 18:11:26.501280 rain_orm-1.0.3/rain_orm.egg-info/
+-rw-rw-rw-   0        0        0     3049 2023-05-31 18:11:26.000000 rain_orm-1.0.3/rain_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2023-05-31 18:11:26.000000 rain_orm-1.0.3/rain_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 18:11:26.000000 rain_orm-1.0.3/rain_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-31 18:11:26.000000 rain_orm-1.0.3/rain_orm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-31 18:11:26.000000 rain_orm-1.0.3/rain_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-31 18:11:26.513287 rain_orm-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      474 2023-05-31 18:07:58.000000 rain_orm-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 18:11:26.510292 rain_orm-1.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:46:43.000000 rain_orm-1.0.3/tests/__init__.py
```

### Comparing `rain_orm-1.0.2/LICENSE` & `rain_orm-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.2/PKG-INFO` & `rain_orm-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: rain_orm
-Version: 1.0.2
+Version: 1.0.3
 Summary: a tiny orm frame
-Home-page: UNKNOWN
+Home-page: https://github.com/cgynb/rain-orm
 Author: rain
 Author-email: 948628463@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -36,28 +36,32 @@
 import rain_orm
 
 rain_orm.connect(host="you host", port=3306, user="root", password="your password", database="student_management")
 
 
 class StudentModel(rain_orm.Table):
     __table__ = "students"
-    __instance__ = {
+    __fields__ = {
         "id": None,
         "name": None,
         "password": None,
         "class_id": None
     }
 
 if __name__ == "__main__":
     stu = StudentModel().where("id=?", 1).one()
+    print("id: ", stu.id)
+    print("name: ", stu.name)
     print(stu)
 ```
 result
 
 ```cmd
+id: 1
+name: cgy
 <<StudentModel 2109293369984
     .table = students
     .instance = {
         id: 1,
         name: cgy,
         password: None,
         class_id: 1,
@@ -68,15 +72,15 @@
 # Basic Usage
 
 it's easy to use rain-orm
 
 1. import rain_orm
 2. connect to database
 3. define model class that inherits class rain_orm.Table
-4. define two attribute "\_\_table__" and "\_\_instance__"
+4. define two attribute "\_\_table__" and "\_\_fields__"
 5. use rain-orm API
 
 ## Import
 ```python
 import rain_orm
 ```
```

### Comparing `rain_orm-1.0.2/README.md` & `rain_orm-1.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,28 +24,32 @@
 import rain_orm
 
 rain_orm.connect(host="you host", port=3306, user="root", password="your password", database="student_management")
 
 
 class StudentModel(rain_orm.Table):
     __table__ = "students"
-    __instance__ = {
+    __fields__ = {
         "id": None,
         "name": None,
         "password": None,
         "class_id": None
     }
 
 if __name__ == "__main__":
     stu = StudentModel().where("id=?", 1).one()
+    print("id: ", stu.id)
+    print("name: ", stu.name)
     print(stu)
 ```
 result
 
 ```cmd
+id: 1
+name: cgy
 <<StudentModel 2109293369984
     .table = students
     .instance = {
         id: 1,
         name: cgy,
         password: None,
         class_id: 1,
@@ -56,15 +60,15 @@
 # Basic Usage
 
 it's easy to use rain-orm
 
 1. import rain_orm
 2. connect to database
 3. define model class that inherits class rain_orm.Table
-4. define two attribute "\_\_table__" and "\_\_instance__"
+4. define two attribute "\_\_table__" and "\_\_fields__"
 5. use rain-orm API
 
 ## Import
 ```python
 import rain_orm
 ```
```

### Comparing `rain_orm-1.0.2/rain_orm/db.py` & `rain_orm-1.0.3/rain_orm/db.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.2/rain_orm/sql_builder/dmldql_builder.py` & `rain_orm-1.0.3/rain_orm/sql_builder/dmldql_builder.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.2/rain_orm/table.py` & `rain_orm-1.0.3/rain_orm/table.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,31 +25,29 @@
     #     # TODO: DDL
     #     print(cls.__subclasses__())
 
     def __init__(self, **kwargs):
         if not isinstance(self.__table__, str):
             raise DefineError(f"type(__table__) should be str, but is {type(self.__table__)}")
         if not isinstance(self.__fields__, dict):
-            raise DefineError(f"type(__instance__) should be dict, but is {type(self.__instance__)}")
+            raise DefineError(f"type(__fields__) should be dict, but is {type(self.__fields__)}")
 
         self.instance = copy.deepcopy(self.__fields__)
         self.__dmldql_builder = DMLDQLBuilder(self.__table__)
         for k, v in kwargs.items():
             self.instance[k] = v
 
     def __str__(self):
         table = self.__table__
-        fields = list(self.__fields__.keys())
         instance = "{\n"
         for k, v in self.instance.items():
             instance += f"\t\t{k}: {v},\n"
         instance += "\t}"
         return f"\033[0;36m<< {self.__class__.__name__} {id(self)}\033[0m\n" \
                f"\t\033[0;32m.table\033[0m = {table}\n" \
-               f"\t\033[0;32m.fields\033[0m = {fields}\n" \
                f"\t\033[0;32m.instance\033[0m = {instance}\n" \
                f"\033[0;36m>>\033[0m\n"
 
     def __repr__(self):
         return str(self)
 
     def __getattr__(self, key):
```

### Comparing `rain_orm-1.0.2/rain_orm.egg-info/PKG-INFO` & `rain_orm-1.0.3/rain_orm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: rain-orm
-Version: 1.0.2
+Version: 1.0.3
 Summary: a tiny orm frame
-Home-page: UNKNOWN
+Home-page: https://github.com/cgynb/rain-orm
 Author: rain
 Author-email: 948628463@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -36,28 +36,32 @@
 import rain_orm
 
 rain_orm.connect(host="you host", port=3306, user="root", password="your password", database="student_management")
 
 
 class StudentModel(rain_orm.Table):
     __table__ = "students"
-    __instance__ = {
+    __fields__ = {
         "id": None,
         "name": None,
         "password": None,
         "class_id": None
     }
 
 if __name__ == "__main__":
     stu = StudentModel().where("id=?", 1).one()
+    print("id: ", stu.id)
+    print("name: ", stu.name)
     print(stu)
 ```
 result
 
 ```cmd
+id: 1
+name: cgy
 <<StudentModel 2109293369984
     .table = students
     .instance = {
         id: 1,
         name: cgy,
         password: None,
         class_id: 1,
@@ -68,15 +72,15 @@
 # Basic Usage
 
 it's easy to use rain-orm
 
 1. import rain_orm
 2. connect to database
 3. define model class that inherits class rain_orm.Table
-4. define two attribute "\_\_table__" and "\_\_instance__"
+4. define two attribute "\_\_table__" and "\_\_fields__"
 5. use rain-orm API
 
 ## Import
 ```python
 import rain_orm
 ```
```

