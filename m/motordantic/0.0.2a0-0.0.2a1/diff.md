# Comparing `tmp/motordantic-0.0.2a0.tar.gz` & `tmp/motordantic-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motordantic-0.0.2a0.tar", last modified: Thu Nov 10 14:58:34 2022, max compression
+gzip compressed data, was "motordantic-0.0.2a1.tar", last modified: Wed May 31 16:19:04 2023, max compression
```

## Comparing `motordantic-0.0.2a0.tar` & `motordantic-0.0.2a1.tar`

### file list

```diff
@@ -1,41 +1,47 @@
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2022-11-10 14:58:34.982563 motordantic-0.0.2a0/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1075 2022-09-01 11:47:34.000000 motordantic-0.0.2a0/LICENCE
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     5763 2022-11-10 14:58:34.982563 motordantic-0.0.2a0/PKG-INFO
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     5463 2022-09-18 15:33:09.000000 motordantic-0.0.2a0/README.md
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2022-11-10 14:58:34.978563 motordantic-0.0.2a0/motordantic/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        0 2022-08-23 10:08:05.000000 motordantic-0.0.2a0/motordantic/__init__.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     6518 2022-11-10 14:58:18.000000 motordantic-0.0.2a0/motordantic/aggregate.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3082 2022-11-01 07:31:58.000000 motordantic-0.0.2a0/motordantic/aggregate_expressions.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4382 2022-11-10 14:58:18.000000 motordantic-0.0.2a0/motordantic/connection.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     2133 2022-11-09 14:00:58.000000 motordantic-0.0.2a0/motordantic/exceptions.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     9219 2022-11-10 14:58:18.000000 motordantic-0.0.2a0/motordantic/extra.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     5714 2022-11-01 07:31:58.000000 motordantic-0.0.2a0/motordantic/fields.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    18659 2022-11-10 14:58:18.000000 motordantic-0.0.2a0/motordantic/models.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      616 2022-11-01 07:31:58.000000 motordantic-0.0.2a0/motordantic/property.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     8609 2022-11-10 14:58:18.000000 motordantic-0.0.2a0/motordantic/query.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    48857 2022-11-10 14:58:18.000000 motordantic-0.0.2a0/motordantic/querybuilder.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4562 2022-11-09 14:02:29.000000 motordantic-0.0.2a0/motordantic/relation.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     6500 2022-11-01 07:31:58.000000 motordantic-0.0.2a0/motordantic/schema.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1565 2022-11-01 07:31:58.000000 motordantic-0.0.2a0/motordantic/session.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      272 2022-08-31 08:42:52.000000 motordantic-0.0.2a0/motordantic/singleton.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      556 2022-09-23 10:46:10.000000 motordantic-0.0.2a0/motordantic/sync.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3496 2022-11-10 14:31:35.000000 motordantic-0.0.2a0/motordantic/types.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      725 2022-11-01 07:31:58.000000 motordantic-0.0.2a0/motordantic/typing.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1978 2022-11-10 14:58:18.000000 motordantic-0.0.2a0/motordantic/validaton.py
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2022-11-10 14:58:34.978563 motordantic-0.0.2a0/motordantic.egg-info/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     5763 2022-11-10 14:58:34.000000 motordantic-0.0.2a0/motordantic.egg-info/PKG-INFO
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      882 2022-11-10 14:58:34.000000 motordantic-0.0.2a0/motordantic.egg-info/SOURCES.txt
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        1 2022-11-10 14:58:34.000000 motordantic-0.0.2a0/motordantic.egg-info/dependency_links.txt
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       43 2022-11-10 14:58:34.000000 motordantic-0.0.2a0/motordantic.egg-info/requires.txt
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       18 2022-11-10 14:58:34.000000 motordantic-0.0.2a0/motordantic.egg-info/top_level.txt
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       38 2022-11-10 14:58:34.982563 motordantic-0.0.2a0/setup.cfg
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      646 2022-11-10 14:58:18.000000 motordantic-0.0.2a0/setup.py
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2022-11-10 14:58:34.978563 motordantic-0.0.2a0/tests/
-drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2022-11-10 14:58:34.982563 motordantic-0.0.2a0/tests/queries/
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        0 2022-08-29 14:37:06.000000 motordantic-0.0.2a0/tests/queries/__init__.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    10287 2022-11-10 14:58:18.000000 motordantic-0.0.2a0/tests/queries/test_aggregation.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     7072 2022-11-10 14:58:18.000000 motordantic-0.0.2a0/tests/queries/test_basic_queries.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1607 2022-11-10 14:58:18.000000 motordantic-0.0.2a0/tests/queries/test_indexes.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     2597 2022-11-10 14:58:18.000000 motordantic-0.0.2a0/tests/queries/test_inner_qyeries.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1469 2022-11-10 14:58:18.000000 motordantic-0.0.2a0/tests/queries/test_query.py
--rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1638 2022-11-10 14:58:18.000000 motordantic-0.0.2a0/tests/queries/test_raw_queries.py
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-05-31 16:19:04.456948 motordantic-0.0.2a1/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1075 2022-09-01 11:47:34.000000 motordantic-0.0.2a1/LICENCE
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     5763 2023-05-31 16:19:04.456948 motordantic-0.0.2a1/PKG-INFO
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     5463 2022-09-18 15:33:09.000000 motordantic-0.0.2a1/README.md
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-05-31 16:19:04.452948 motordantic-0.0.2a1/motordantic/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        0 2022-08-23 10:08:05.000000 motordantic-0.0.2a1/motordantic/__init__.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     6518 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/aggregate.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3082 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/aggregate_expressions.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4382 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/connection.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     2133 2022-11-09 14:00:58.000000 motordantic-0.0.2a1/motordantic/exceptions.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     9219 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/extra.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     5714 2022-11-01 07:31:58.000000 motordantic-0.0.2a1/motordantic/fields.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    18659 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/models.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      616 2022-11-01 07:31:58.000000 motordantic-0.0.2a1/motordantic/property.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     8609 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/query.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    49044 2023-05-31 16:17:59.000000 motordantic-0.0.2a1/motordantic/querybuilder.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     4562 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/relation.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     6500 2022-11-01 07:31:58.000000 motordantic-0.0.2a1/motordantic/schema.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1565 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/session.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      272 2022-08-31 08:42:52.000000 motordantic-0.0.2a1/motordantic/singleton.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      556 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/sync.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3496 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/types.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      725 2022-11-01 07:31:58.000000 motordantic-0.0.2a1/motordantic/typing.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1978 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/motordantic/validaton.py
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-05-31 16:19:04.456948 motordantic-0.0.2a1/motordantic.egg-info/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     5763 2023-05-31 16:19:04.000000 motordantic-0.0.2a1/motordantic.egg-info/PKG-INFO
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1032 2023-05-31 16:19:04.000000 motordantic-0.0.2a1/motordantic.egg-info/SOURCES.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        1 2023-05-31 16:19:04.000000 motordantic-0.0.2a1/motordantic.egg-info/dependency_links.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       43 2023-05-31 16:19:04.000000 motordantic-0.0.2a1/motordantic.egg-info/requires.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       18 2023-05-31 16:19:04.000000 motordantic-0.0.2a1/motordantic.egg-info/top_level.txt
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)       38 2023-05-31 16:19:04.456948 motordantic-0.0.2a1/setup.cfg
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      646 2023-05-31 16:18:18.000000 motordantic-0.0.2a1/setup.py
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-05-31 16:19:04.456948 motordantic-0.0.2a1/tests/
+drwxrwxr-x   0 bzdv      (1000) bzdv      (1000)        0 2023-05-31 16:19:04.456948 motordantic-0.0.2a1/tests/queries/
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)        0 2023-03-31 20:51:37.000000 motordantic-0.0.2a1/tests/queries/__init__.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)    10287 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/tests/queries/test_aggregation.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     7072 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/tests/queries/test_basic_queries.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1607 2023-03-31 20:44:32.000000 motordantic-0.0.2a1/tests/queries/test_indexes.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     2597 2022-11-10 14:58:18.000000 motordantic-0.0.2a1/tests/queries/test_inner_qyeries.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1469 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/tests/queries/test_query.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1638 2023-03-31 20:24:13.000000 motordantic-0.0.2a1/tests/queries/test_raw_queries.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     1384 2022-11-10 14:58:18.000000 motordantic-0.0.2a1/tests/test_connection.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     2746 2023-04-12 19:32:32.000000 motordantic-0.0.2a1/tests/test_create_model.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3501 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/tests/test_extraquerymapper.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)      196 2022-09-02 10:52:13.000000 motordantic-0.0.2a1/tests/test_force_sync.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     3911 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/tests/test_relation.py
+-rw-rw-r--   0 bzdv      (1000) bzdv      (1000)     2050 2023-05-31 16:17:49.000000 motordantic-0.0.2a1/tests/test_sync.py
```

### Comparing `motordantic-0.0.2a0/LICENCE` & `motordantic-0.0.2a1/LICENCE`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/PKG-INFO` & `motordantic-0.0.2a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motordantic
-Version: 0.0.2a0
+Version: 0.0.2a1
 Summary: Mongo ODM, based on motor+pydantic
 Home-page: https://github.com/bogdanjz/motordantic
 Author: bogdanjz
 Author-email: bzdv.dn@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `motordantic-0.0.2a0/README.md` & `motordantic-0.0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/motordantic/aggregate.py` & `motordantic-0.0.2a1/motordantic/aggregate.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/motordantic/aggregate_expressions.py` & `motordantic-0.0.2a1/motordantic/aggregate_expressions.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/motordantic/connection.py` & `motordantic-0.0.2a1/motordantic/connection.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/motordantic/exceptions.py` & `motordantic-0.0.2a1/motordantic/exceptions.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/motordantic/extra.py` & `motordantic-0.0.2a1/motordantic/extra.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/motordantic/fields.py` & `motordantic-0.0.2a1/motordantic/fields.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/motordantic/models.py` & `motordantic-0.0.2a1/motordantic/models.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/motordantic/property.py` & `motordantic-0.0.2a1/motordantic/property.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/motordantic/query.py` & `motordantic-0.0.2a1/motordantic/query.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/motordantic/querybuilder.py` & `motordantic-0.0.2a1/motordantic/querybuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,21 +231,26 @@
 
     async def create_indexes(
         self,
         indexes: List[IndexModel],
         session: Optional[ClientSession] = None,
     ) -> List[str]:
         create_indexes_cursor = getattr(
-            self.mongo_model_class.collection, 'create_indexes'
-        )
-        return await create_indexes_cursor(
-            indexes,
-            session=session,
-            maxTimeMS=3600,
+            self.mongo_model_class.collection, 'create_index'
         )
+        result = []
+        for index in indexes:
+            index_value = list(index.document['key'].items())
+            res = await create_indexes_cursor(
+                index_value,
+                session=session,
+                background=True,
+            )
+            result.append(res)
+        return result
 
     async def drop_index(
         self, index_name: str, session: Optional[ClientSession] = None
     ) -> str:
         indexes = await self.list_indexes(session)
         if index_name in indexes:
             await self._make_query('drop_index', index_name, session=session)
```

### Comparing `motordantic-0.0.2a0/motordantic/relation.py` & `motordantic-0.0.2a1/motordantic/relation.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/motordantic/schema.py` & `motordantic-0.0.2a1/motordantic/schema.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/motordantic/session.py` & `motordantic-0.0.2a1/motordantic/session.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/motordantic/sync.py` & `motordantic-0.0.2a1/motordantic/sync.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/motordantic/types.py` & `motordantic-0.0.2a1/motordantic/types.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/motordantic/typing.py` & `motordantic-0.0.2a1/motordantic/typing.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/motordantic/validaton.py` & `motordantic-0.0.2a1/motordantic/validaton.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/motordantic.egg-info/PKG-INFO` & `motordantic-0.0.2a1/motordantic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motordantic
-Version: 0.0.2a0
+Version: 0.0.2a1
 Summary: Mongo ODM, based on motor+pydantic
 Home-page: https://github.com/bogdanjz/motordantic
 Author: bogdanjz
 Author-email: bzdv.dn@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `motordantic-0.0.2a0/motordantic.egg-info/SOURCES.txt` & `motordantic-0.0.2a1/motordantic.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 motordantic/typing.py
 motordantic/validaton.py
 motordantic.egg-info/PKG-INFO
 motordantic.egg-info/SOURCES.txt
 motordantic.egg-info/dependency_links.txt
 motordantic.egg-info/requires.txt
 motordantic.egg-info/top_level.txt
+tests/test_connection.py
+tests/test_create_model.py
+tests/test_extraquerymapper.py
+tests/test_force_sync.py
+tests/test_relation.py
+tests/test_sync.py
 tests/queries/__init__.py
 tests/queries/test_aggregation.py
 tests/queries/test_basic_queries.py
 tests/queries/test_indexes.py
 tests/queries/test_inner_qyeries.py
 tests/queries/test_query.py
 tests/queries/test_raw_queries.py
```

### Comparing `motordantic-0.0.2a0/setup.py` & `motordantic-0.0.2a1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read(f):
     return open(f, "r").read()
 
 
 setup(
     name="motordantic",
-    version='0.0.2a0',
+    version='0.0.2a1',
     packages=find_packages(exclude=("tests", "docs", "examples")),
     install_requires=[
         "pydantic>=1.9,<2",
         "pymongo==4.1",
         "motor==3.0.0",
     ],
     description="Mongo ODM, based on motor+pydantic",
```

### Comparing `motordantic-0.0.2a0/tests/queries/test_aggregation.py` & `motordantic-0.0.2a1/tests/queries/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/tests/queries/test_basic_queries.py` & `motordantic-0.0.2a1/tests/queries/test_basic_queries.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/tests/queries/test_indexes.py` & `motordantic-0.0.2a1/tests/queries/test_indexes.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/tests/queries/test_inner_qyeries.py` & `motordantic-0.0.2a1/tests/queries/test_inner_qyeries.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/tests/queries/test_query.py` & `motordantic-0.0.2a1/tests/queries/test_query.py`

 * *Files identical despite different names*

### Comparing `motordantic-0.0.2a0/tests/queries/test_raw_queries.py` & `motordantic-0.0.2a1/tests/queries/test_raw_queries.py`

 * *Files identical despite different names*

