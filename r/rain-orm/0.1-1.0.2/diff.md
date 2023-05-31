# Comparing `tmp/rain_orm-0.1.tar.gz` & `tmp/rain_orm-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rain_orm-0.1.tar", last modified: Sun May 28 18:05:47 2023, max compression
+gzip compressed data, was "rain_orm-1.0.2.tar", last modified: Wed May 31 04:15:05 2023, max compression
```

## Comparing `rain_orm-0.1.tar` & `rain_orm-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 18:05:47.273089 rain_orm-0.1/
--rw-rw-rw-   0        0        0    11555 2023-05-28 17:49:39.000000 rain_orm-0.1/LICENSE
--rw-rw-rw-   0        0        0      260 2023-05-28 18:05:47.273089 rain_orm-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-28 17:49:56.000000 rain_orm-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 18:05:47.266095 rain_orm-0.1/rain_orm/
--rw-rw-rw-   0        0        0       67 2023-05-28 17:47:06.000000 rain_orm-0.1/rain_orm/__init__.py
--rw-rw-rw-   0        0        0      771 2023-05-27 18:18:51.000000 rain_orm-0.1/rain_orm/db.py
--rw-rw-rw-   0        0        0      443 2023-05-27 12:49:37.000000 rain_orm-0.1/rain_orm/error.py
--rw-rw-rw-   0        0        0     4305 2023-05-28 17:47:06.000000 rain_orm-0.1/rain_orm/orm.py
--rw-rw-rw-   0        0        0     5592 2023-05-28 17:45:08.000000 rain_orm-0.1/rain_orm/sql_builder.py
-drwxrwxrwx   0        0        0        0 2023-05-28 18:05:47.272092 rain_orm-0.1/rain_orm.egg-info/
--rw-rw-rw-   0        0        0      260 2023-05-28 18:05:47.000000 rain_orm-0.1/rain_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-05-28 18:05:47.000000 rain_orm-0.1/rain_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 18:05:47.000000 rain_orm-0.1/rain_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-28 18:05:47.000000 rain_orm-0.1/rain_orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-28 18:05:47.000000 rain_orm-0.1/rain_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-28 18:05:47.274089 rain_orm-0.1/setup.cfg
--rw-rw-rw-   0        0        0      439 2023-05-28 18:04:44.000000 rain_orm-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:15:05.643228 rain_orm-1.0.2/
+-rw-rw-rw-   0        0        0    11555 2023-05-28 17:49:39.000000 rain_orm-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2951 2023-05-31 04:15:05.643228 rain_orm-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2696 2023-05-31 03:53:53.000000 rain_orm-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 04:15:05.623705 rain_orm-1.0.2/rain_orm/
+-rw-rw-rw-   0        0        0      137 2023-05-31 02:13:13.000000 rain_orm-1.0.2/rain_orm/__init__.py
+-rw-rw-rw-   0        0        0      311 2023-05-29 18:48:08.000000 rain_orm-1.0.2/rain_orm/common.py
+-rw-rw-rw-   0        0        0      781 2023-05-30 18:06:06.000000 rain_orm-1.0.2/rain_orm/db.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:15:05.633312 rain_orm-1.0.2/rain_orm/error/
+-rw-rw-rw-   0        0        0      153 2023-05-30 17:55:36.000000 rain_orm-1.0.2/rain_orm/error/__init__.py
+-rw-rw-rw-   0        0        0      283 2023-05-30 16:40:48.000000 rain_orm-1.0.2/rain_orm/error/error.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:15:05.637732 rain_orm-1.0.2/rain_orm/sql_builder/
+-rw-rw-rw-   0        0        0      178 2023-05-30 17:56:14.000000 rain_orm-1.0.2/rain_orm/sql_builder/__init__.py
+-rw-rw-rw-   0        0        0       29 2023-05-30 17:52:43.000000 rain_orm-1.0.2/rain_orm/sql_builder/ddl_builder.py
+-rw-rw-rw-   0        0        0     5961 2023-05-30 17:43:33.000000 rain_orm-1.0.2/rain_orm/sql_builder/dmldql_builder.py
+-rw-rw-rw-   0        0        0     6030 2023-05-31 04:08:56.000000 rain_orm-1.0.2/rain_orm/table.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:15:05.631015 rain_orm-1.0.2/rain_orm.egg-info/
+-rw-rw-rw-   0        0        0     2951 2023-05-31 04:15:05.000000 rain_orm-1.0.2/rain_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2023-05-31 04:15:05.000000 rain_orm-1.0.2/rain_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 04:15:05.000000 rain_orm-1.0.2/rain_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-31 04:15:05.000000 rain_orm-1.0.2/rain_orm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-31 04:15:05.000000 rain_orm-1.0.2/rain_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-31 04:15:05.644621 rain_orm-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      441 2023-05-31 03:58:42.000000 rain_orm-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:15:05.641925 rain_orm-1.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:46:43.000000 rain_orm-1.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0       19 2023-05-31 01:50:35.000000 rain_orm-1.0.2/tests/test_db.py
```

### Comparing `rain_orm-0.1/LICENSE` & `rain_orm-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rain_orm-0.1/rain_orm/sql_builder.py` & `rain_orm-1.0.2/rain_orm/sql_builder/dmldql_builder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,147 +1,184 @@
-try:
-    from rain_orm.error import SqlBuildError
-except ImportError:
-    from error import SqlBuildError
+from rain_orm.error import SqlBuildError
 
 
-class SqlBuilder:
+class DMLDQLBuilder:
     operations = ["select", "insert", "update", "delete"]
 
     def __init__(self, table, op=None):
-        self.sql_str = ""
+        self.__sql_str = None
         self.table = table
         self.op = op
-        self.target = []
-        self.condition = []
-        self.fields_values = {}
-        self.limit_num = None
-        self.offset_num = None
-        self.order = []
+        self.__select_items = list()
+        self.__conditions = list()
+        self.__set_fields_values = dict()
+        self.__orders = list()
+        self.__limit_num = None
+        self.__offset_num = None
 
     def __str__(self):
-        return self.sql_str
+        if self.__sql_str is None:
+            return self.sql
+        else:
+            return self.__sql_str
 
     def __repr__(self):
-        return self.sql_str
+        return str(self)
 
     def set_operation(self, op):
         self.op = op
 
     def select(self, *args):
         for t in args:
             if not isinstance(t, str):
                 raise SqlBuildError("args should be str")
         for t in args:
-            self.target.append(t)
+            self.__select_items.append(t)
         return self
 
     def where(self, condition, value=None):
         if isinstance(value, str):
             value = f"'{value}'"
         cond_str = condition.replace("?", str(value))
-        self.condition.append(cond_str)
+        self.__conditions.append(cond_str)
         return self
 
+    def clear_where(self):
+        self.__conditions.clear()
+
     def set(self, **kwargs):
-        self.fields_values = kwargs
+        self.__set_fields_values = kwargs
         return self
 
+    def clear_set(self):
+        self.__set_fields_values.clear()
+
     def limit(self, num=None):
         if isinstance(num, int):
-            self.limit_num = num
+            self.__limit_num = num
         elif num is not None:
             raise SqlBuildError("limit num should be int or None")
         return self
 
     def offset(self, num=None):
         if isinstance(num, int):
-            self.offset_num = num
+            self.__offset_num = num
         elif num is not None:
             raise SqlBuildError("limit num should be int or None")
         return self
 
     def order_by(self, by=None, asc=True):
         if isinstance(by, str) and isinstance(asc, bool):
-            self.order.append({
+            self.__orders.append({
                 "by": by,
                 "asc": asc
             })
         elif by is not None:
             raise SqlBuildError("by should be str or None")
         return self
 
-    def generate_sql(self):
+    @property
+    def sql(self):
         if self.op not in self.operations:
             raise SqlBuildError("operation should be in ['select', 'insert', 'update', 'delete']")
-        table = self.table
-        if self.op == "select":
-            self.target.sort()
-            target_str = "*" if len(self.target) == 0 else f"{', '.join(self.target)}"
-            condition_str = "" if len(self.condition) == 0 else f"where {' and '.join(self.condition)}"
-            order_str = "" if len(self.order) == 0 else "order by " + ' ,'.join(
-                [f"{item['by']} {'asc' if item['asc'] else 'desc'}" for item in self.order])
-            limit_str = "" if self.limit_num is None else f"limit {self.limit_num}"
-            offset_str = "" if self.limit_num is None or self.offset_num is None else f"offset {self.offset_num}"
-            self.sql_str = f"select {target_str} from {table} {condition_str} {order_str} {limit_str} {offset_str};"
-        elif self.op == "insert":
-            if len(self.fields_values) == 0:
-                raise SqlBuildError("insert operation should take fields and values, but there are not defined")
-            fields = ', '.join([item for item in self.fields_values.keys() if self.fields_values.get(item) is not None])
-            values = ', '.join(list(
-                map(
-                    lambda item: f"'{item}'" if isinstance(item, str) else str(item),
-                    [item for item in self.fields_values.values() if item is not None]
-                )))
-            self.sql_str = f"insert into {table} ({fields}) values ({values});"
-        elif self.op == "update":
-            if len(self.fields_values) != 1:
-                raise SqlBuildError("update operation should only set 1 field")
-            condition_str = "" if len(self.condition) == 0 else f"where {' and '.join(self.condition)}"
-            field = list(self.fields_values.keys())[0]
-            value = list(self.fields_values.values())[0]
-            if isinstance(value, str):
-                value = f"'{value}'"
-            self.sql_str = f"update {table} set {field}={value} {condition_str}"
-        elif self.op == "delete":
-            if len(self.condition) == 0:
-                raise SqlBuildError("delete operation should take at least 1 condition")
-            condition_str = f"where {' and '.join(self.condition)}"
-            self.sql_str = f"delete from {table} {condition_str}"
-        return self.sql_str
+        else:
+            if self.op == "select":
+                self.__sql_str = self.select_sql
+            elif self.op == "insert":
+                self.__sql_str = self.insert_sql
+            elif self.op == "update":
+                self.__sql_str = self.update_sql
+            elif self.op == "delete":
+                self.__sql_str = self.delete_sql
+        return self.__sql_str
+
+    @property
+    def select_sql(self):
+        return f"select {self.__select_str} from {self.table} {self.__condition_str} {self.__order_str} {self.__limit_str} {self.__offset_str};"
+
+    @property
+    def insert_sql(self):
+        if len(self.__set_fields_values) == 0:
+            raise SqlBuildError("insert operation should take fields and values, but there are not defined")
+        return f"insert into {self.table} ({self.__field_str}) values ({self.__value_str});"
+
+    @property
+    def update_sql(self):
+        if len(self.__set_fields_values) != 1:
+            raise SqlBuildError("update operation should only set 1 field")
+        return f"update {self.table} set {self.__field_str} = {self.__value_str} {self.__condition_str}"
+
+    @property
+    def delete_sql(self):
+        if len(self.__conditions) == 0:
+            raise SqlBuildError("delete operation should take at least 1 condition")
+        return f"delete from {self.table} {self.__condition_str}"
+
+    @property
+    def __select_str(self):
+        if len(self.__select_items) == 0:
+            return "*"
+        else:
+            self.__select_items.sort()
+            return f"{', '.join(self.__select_items)}"
+
+    @property
+    def __condition_str(self):
+        if len(self.__conditions) == 0:
+            return ""
+        else:
+            return f"where {' and '.join(self.__conditions)}"
+
+    @property
+    def __order_str(self):
+        if len(self.__orders) == 0:
+            return ""
+        else:
+            return "order by " + ' ,'.join([f"{item['by']} {'asc' if item['asc'] else 'desc'}" for item in self.__orders])
+
+    @property
+    def __limit_str(self):
+        if self.__limit_num is None:
+            return ""
+        else:
+            return f"limit {self.__limit_num}"
+
+    @property
+    def __offset_str(self):
+        if self.__limit_num is None or self.__offset_num is None:
+            return ""
+        else:
+            return f"offset {self.__offset_num}"
+
+    @property
+    def __field_str(self):
+        return ', '.join([item for item in self.__set_fields_values.keys() if self.__set_fields_values.get(item) is not None])
+
+    @property
+    def __value_str(self):
+        return ', '.join(list(
+                            map(
+                                lambda item: f"'{item}'" if isinstance(item, str) else str(item),
+                                [item for item in self.__set_fields_values.values() if item is not None]
+                            )))
+
+    @property
+    def select_items(self):
+        return self.__select_items
 
 
 if __name__ == "__main__":
-    S1 = SqlBuilder("table", "select")
-    S2 = SqlBuilder("table", "select")
-    S1.where("id = ?", 1).where("name='cgy'").select("name").select("id").generate_sql()
-    S2.generate_sql()
-
-    S3 = SqlBuilder("table", "insert")
-    S4 = SqlBuilder("table", "insert")
-    S3.set(name="cgy", gender="male").generate_sql()
-    # S4.generate_sql()
-
-    S5 = SqlBuilder("table", "delete")
-    S6 = SqlBuilder("table", "delete")
-    S5.where("id = ?", 1).generate_sql()
-    # S6.generate_sql()
-
-    S7 = SqlBuilder("table", "update")
-    S8 = SqlBuilder("table", "update")
-    S9 = SqlBuilder("table", "update")
-    S7.set(name="cgy").where("id = ?", 1).generate_sql()
-    # S8.set(name="cgy", age=18).generate_sql()
-    S9.set(gender="female").generate_sql()
-
-    # print(S1)
-    # print(S2)
-    # print(S3)
-    # # print(S4)
-    # print(S5)
-    # # print(S6)
-    # print(S7)
-    # print(S8)
-    # print(S9)
-    s = SqlBuilder("table", "select")
-    s.select("id", "name", "age").where("id < 5").order_by("id", False).limit(2).offset(1).generate_sql()
-    print(s)
+    s_select = SqlBuilder(table="table")
+    s_select.select("id", "name").where("id < 500").order_by("id", asc=False).limit(2).offset(9)
+    print(s_select.select_sql)
+
+    s_insert = SqlBuilder(table="table")
+    s_insert.set(id=1, age=18)
+    print(s_insert.insert_sql)
+
+    s_update = SqlBuilder(table="table")
+    s_update.where("id = ?", 1).set(age=19)
+    print(s_update.update_sql)
+
+    s_delete = SqlBuilder(table="table")
+    s_delete.where("age < ?", 18)
+    print(s_delete.delete_sql)
```

