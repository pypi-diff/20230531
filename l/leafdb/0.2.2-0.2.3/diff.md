# Comparing `tmp/leafdb-0.2.2.tar.gz` & `tmp/leafdb-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leafdb-0.2.2.tar", last modified: Fri May 20 14:05:17 2022, max compression
+gzip compressed data, was "leafdb-0.2.3.tar", last modified: Wed May 31 03:17:30 2023, max compression
```

## Comparing `leafdb-0.2.2.tar` & `leafdb-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 yhq        (501) staff       (20)        0 2022-05-20 14:05:17.756588 leafdb-0.2.2/
--rw-r--r--   0 yhq        (501) staff       (20)      283 2022-05-20 14:05:17.756460 leafdb-0.2.2/PKG-INFO
-drwxr-xr-x   0 yhq        (501) staff       (20)        0 2022-05-20 14:05:17.756308 leafdb-0.2.2/leafdb.egg-info/
--rw-r--r--   0 yhq        (501) staff       (20)      283 2022-05-20 14:05:17.000000 leafdb-0.2.2/leafdb.egg-info/PKG-INFO
--rw-r--r--   0 yhq        (501) staff       (20)      167 2022-05-20 14:05:17.000000 leafdb-0.2.2/leafdb.egg-info/SOURCES.txt
--rw-r--r--   0 yhq        (501) staff       (20)        1 2022-05-20 14:05:17.000000 leafdb-0.2.2/leafdb.egg-info/dependency_links.txt
--rw-r--r--   0 yhq        (501) staff       (20)       19 2022-05-20 14:05:17.000000 leafdb-0.2.2/leafdb.egg-info/requires.txt
--rw-r--r--   0 yhq        (501) staff       (20)        7 2022-05-20 14:05:17.000000 leafdb-0.2.2/leafdb.egg-info/top_level.txt
--rw-r--r--   0 yhq        (501) staff       (20)    29448 2022-05-20 14:03:38.000000 leafdb-0.2.2/leafdb.py
--rw-r--r--   0 yhq        (501) staff       (20)       38 2022-05-20 14:05:17.756624 leafdb-0.2.2/setup.cfg
--rwxrwxrwx   0 yhq        (501) staff       (20)      482 2022-05-20 14:03:24.000000 leafdb-0.2.2/setup.py
+drwxr-xr-x   0 yhq        (501) staff       (20)        0 2023-05-31 03:17:30.388420 leafdb-0.2.3/
+-rw-r--r--   0 yhq        (501) staff       (20)      283 2023-05-31 03:17:30.388322 leafdb-0.2.3/PKG-INFO
+drwxr-xr-x   0 yhq        (501) staff       (20)        0 2023-05-31 03:17:30.388197 leafdb-0.2.3/leafdb.egg-info/
+-rw-r--r--   0 yhq        (501) staff       (20)      283 2023-05-31 03:17:30.000000 leafdb-0.2.3/leafdb.egg-info/PKG-INFO
+-rw-r--r--   0 yhq        (501) staff       (20)      167 2023-05-31 03:17:30.000000 leafdb-0.2.3/leafdb.egg-info/SOURCES.txt
+-rw-r--r--   0 yhq        (501) staff       (20)        1 2023-05-31 03:17:30.000000 leafdb-0.2.3/leafdb.egg-info/dependency_links.txt
+-rw-r--r--   0 yhq        (501) staff       (20)       26 2023-05-31 03:17:30.000000 leafdb-0.2.3/leafdb.egg-info/requires.txt
+-rw-r--r--   0 yhq        (501) staff       (20)        7 2023-05-31 03:17:30.000000 leafdb-0.2.3/leafdb.egg-info/top_level.txt
+-rw-r--r--   0 yhq        (501) staff       (20)    29458 2023-05-31 03:11:31.000000 leafdb-0.2.3/leafdb.py
+-rw-r--r--   0 yhq        (501) staff       (20)       38 2023-05-31 03:17:30.388458 leafdb-0.2.3/setup.cfg
+-rwxrwxrwx   0 yhq        (501) staff       (20)      489 2023-05-31 03:14:40.000000 leafdb-0.2.3/setup.py
```

### Comparing `leafdb-0.2.2/leafdb.py` & `leafdb-0.2.3/leafdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 
 __all__ = ["DbDialect", "database", "SQLConn", "SQLRow", "SQLRowCollection", "SQLParser", "Connection", "BaseDbs",
            "MultipleBaseDbs"]
 
 import os
 import re
 from collections import OrderedDict
@@ -317,15 +317,15 @@
 
     def __repr__(self):
         return '<Connection open={}>'.format(self.open)
 
     def query(self, query, fetchall=False, **params):
         cursor = self._conn.execute(text(query), **params)
         if not cursor.keys():  # Skip insert,update has none return values error
-        	return None
+            return None
         row_gen = (SQLRow(cursor.keys(), row) for row in cursor)
         results = SQLRowCollection(row_gen)
         if fetchall:
             results.list()
         return results
 
     def bulk_query(self, query, *multiparams):
@@ -881,23 +881,26 @@
             if hasattr(db, name):
                 return getattr(db, name)
 
         raise KeyError("not find database: %s in DB Config" % name)
 
     def _gen_conn(self, name):
         if name in self._dbs:
-            return self._dbs.get(name)
-        else:
-            _dbc = self._dbc.get(name)
-            _lpt = _dbc.pop("printing", False)
-            printing = any([_lpt, _dbc.get("PRINTING")])
-            _dbc.update(dict(PRINTING=printing))
-            if _dbc:
-                _db = database(**_dbc)
-                self._dbs[name] = _db
+            _db = self._dbs.get(name)
+            if _db.open:
                 return _db
+
+        _dbc = self._dbc.get(name)
+        _lpt = _dbc.pop("printing", False)
+        printing = any([_lpt, _dbc.get("PRINTING")])
+        _dbc.update(dict(PRINTING=printing))
+        if _dbc:
+            _db = database(**_dbc)
+            self._dbs[name] = _db
+            return _db
+
         return None
 
     def close(self):
         for v in self._dbs.values():
             v.close()
         self._dbs.clear()
```

