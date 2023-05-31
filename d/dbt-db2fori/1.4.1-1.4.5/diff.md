# Comparing `tmp/dbt_db2fori-1.4.1.tar.gz` & `tmp/dbt_db2fori-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_db2fori-1.4.1.tar", max compression
+gzip compressed data, was "dbt_db2fori-1.4.5.tar", max compression
```

## Comparing `dbt_db2fori-1.4.1.tar` & `dbt_db2fori-1.4.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1063 2021-10-17 19:23:28.613106 dbt_db2fori-1.4.1/LICENSE
--rw-r--r--   0        0        0     1280 2021-10-22 01:03:55.829895 dbt_db2fori-1.4.1/README.md
--rw-r--r--   0        0        0       22 2023-02-01 03:53:39.139502 dbt_db2fori-1.4.1/dbt/__init__.py
--rw-r--r--   0        0        0      356 2023-02-01 02:39:07.983395 dbt_db2fori-1.4.1/dbt/adapters/db2_for_i/__init__.py
--rw-r--r--   0        0        0       17 2023-02-01 03:53:45.886978 dbt_db2fori-1.4.1/dbt/adapters/db2_for_i/__version__.py
--rw-r--r--   0        0        0     5764 2023-02-01 03:52:27.823841 dbt_db2fori-1.4.1/dbt/adapters/db2_for_i/connections.py
--rw-r--r--   0        0        0     4167 2023-02-01 03:21:09.060777 dbt_db2fori-1.4.1/dbt/adapters/db2_for_i/impl.py
--rw-r--r--   0        0        0      654 2021-10-20 08:42:12.055845 dbt_db2fori-1.4.1/dbt/adapters/db2_for_i/relation.py
--rw-r--r--   0        0        0       51 2021-10-20 08:48:28.010000 dbt_db2fori-1.4.1/dbt/include/db2_for_i/__init__.py
--rw-r--r--   0        0        0      140 2021-10-20 09:31:24.618814 dbt_db2fori-1.4.1/dbt/include/db2_for_i/dbt_project.yml
--rw-r--r--   0        0        0    11746 2023-01-15 23:08:34.553060 dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/adapters.sql
--rw-r--r--   0        0        0     4050 2021-10-20 08:57:53.402901 dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/catalog.sql
--rw-r--r--   0        0        0     5501 2023-01-15 23:08:34.553851 dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/materializations/incremental/incremental.sql
--rw-r--r--   0        0        0     4578 2023-01-15 23:08:34.554699 dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/materializations/incremental/merge.sql
--rw-r--r--   0        0        0     6053 2023-01-15 23:08:34.555800 dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/materializations/seed/seed.sql
--rw-r--r--   0        0        0     8852 2021-10-20 09:12:37.134945 dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0        0        0      914 2021-10-20 09:13:33.996765 dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0        0        0     2543 2021-10-20 09:17:52.225120 dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/materializations/snapshot/strategies.sql
--rw-r--r--   0        0        0      589 2023-01-15 23:08:34.556422 dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/materializations/tests/helpers.sql
--rw-r--r--   0        0        0      493 2023-01-15 23:08:34.557021 dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/materializations/tests/where_subquery.sql
--rw-r--r--   0        0        0      599 2023-02-01 03:53:58.431252 dbt_db2fori-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     2336 1970-01-01 00:00:00.000000 dbt_db2fori-1.4.1/setup.py
--rw-r--r--   0        0        0     2064 1970-01-01 00:00:00.000000 dbt_db2fori-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2021-10-17 19:23:28.613106 dbt_db2fori-1.4.5/LICENSE
+-rw-r--r--   0        0        0     1280 2021-10-22 01:03:55.829895 dbt_db2fori-1.4.5/README.md
+-rw-r--r--   0        0        0       22 2023-02-01 03:53:39.139502 dbt_db2fori-1.4.5/dbt/__init__.py
+-rw-r--r--   0        0        0      356 2023-03-02 06:41:54.087569 dbt_db2fori-1.4.5/dbt/adapters/db2_for_i/__init__.py
+-rw-r--r--   0        0        0       17 2023-05-31 06:40:33.026887 dbt_db2fori-1.4.5/dbt/adapters/db2_for_i/__version__.py
+-rw-r--r--   0        0        0     5764 2023-02-01 03:52:27.823841 dbt_db2fori-1.4.5/dbt/adapters/db2_for_i/connections.py
+-rw-r--r--   0        0        0     4167 2023-02-01 03:21:09.060777 dbt_db2fori-1.4.5/dbt/adapters/db2_for_i/impl.py
+-rw-r--r--   0        0        0      701 2023-05-31 06:34:29.604677 dbt_db2fori-1.4.5/dbt/adapters/db2_for_i/relation.py
+-rw-r--r--   0        0        0       51 2021-10-20 08:48:28.010000 dbt_db2fori-1.4.5/dbt/include/db2_for_i/__init__.py
+-rw-r--r--   0        0        0      140 2021-10-20 09:31:24.618814 dbt_db2fori-1.4.5/dbt/include/db2_for_i/dbt_project.yml
+-rw-r--r--   0        0        0    11746 2023-01-15 23:08:34.553060 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/adapters.sql
+-rw-r--r--   0        0        0     4050 2021-10-20 08:57:53.402901 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/catalog.sql
+-rw-r--r--   0        0        0     5501 2023-01-15 23:08:34.553851 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0        0        0     4578 2023-01-15 23:08:34.554699 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/incremental/merge.sql
+-rw-r--r--   0        0        0     6053 2023-01-15 23:08:34.555800 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/seed/seed.sql
+-rw-r--r--   0        0        0     8852 2021-10-20 09:12:37.134945 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0        0        0      914 2021-10-20 09:13:33.996765 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0        0        0     2543 2021-10-20 09:17:52.225120 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/snapshot/strategies.sql
+-rw-r--r--   0        0        0      589 2023-01-15 23:08:34.556422 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/tests/helpers.sql
+-rw-r--r--   0        0        0      493 2023-01-15 23:08:34.557021 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/tests/where_subquery.sql
+-rw-r--r--   0        0        0      598 2023-05-31 06:35:35.448664 dbt_db2fori-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0     2329 1970-01-01 00:00:00.000000 dbt_db2fori-1.4.5/setup.py
+-rw-r--r--   0        0        0     2057 1970-01-01 00:00:00.000000 dbt_db2fori-1.4.5/PKG-INFO
```

### Comparing `dbt_db2fori-1.4.1/LICENSE` & `dbt_db2fori-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.1/README.md` & `dbt_db2fori-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.1/dbt/adapters/db2_for_i/connections.py` & `dbt_db2fori-1.4.5/dbt/adapters/db2_for_i/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.1/dbt/adapters/db2_for_i/impl.py` & `dbt_db2fori-1.4.5/dbt/adapters/db2_for_i/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.1/dbt/adapters/db2_for_i/relation.py` & `dbt_db2fori-1.4.5/dbt/adapters/db2_for_i/relation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from dbt.adapters.base.relation import BaseRelation, Policy
 
 @dataclass
 class DB2ForIQuotePolicy(Policy):
     database: bool = False
     schema: bool = False
     identifier: bool = False
@@ -13,13 +13,13 @@
     database: bool = False
     schema: bool = True
     identifier: bool = True
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class DB2ForIRelation(BaseRelation):
-    quote_policy: DB2ForIQuotePolicy = DB2ForIQuotePolicy()
-    include_policy: DB2ForIIncludePolicy = DB2ForIIncludePolicy()
+    quote_policy: Policy = field(default_factory = lambda: DB2ForIQuotePolicy())
+    include_policy: Policy = field(default_factory = lambda: DB2ForIIncludePolicy())
 
     @staticmethod
     def add_ephemeral_prefix(name: str):
         return f'DBT_CTE__{name}'
```

### Comparing `dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/adapters.sql` & `dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/catalog.sql` & `dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/materializations/incremental/incremental.sql` & `dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/materializations/incremental/merge.sql` & `dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/materializations/seed/seed.sql` & `dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/seed/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot.sql` & `dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot_merge.sql` & `dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/materializations/snapshot/strategies.sql` & `dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/snapshot/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.1/dbt/include/db2_for_i/macros/materializations/tests/helpers.sql` & `dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.1/setup.py` & `dbt_db2fori-1.4.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,19 @@
  'dbt.include.db2_for_i': ['macros/*',
                            'macros/materializations/incremental/*',
                            'macros/materializations/seed/*',
                            'macros/materializations/snapshot/*',
                            'macros/materializations/tests/*']}
 
 install_requires = \
-['dbt-core>=1.3.2,<2.0.0', 'pyodbc>=4.0.35,<5.0.0']
+['dbt-core==1.4.5', 'pyodbc>=4.0.39,<5.0.0']
 
 setup_kwargs = {
     'name': 'dbt-db2fori',
-    'version': '1.4.1',
+    'version': '1.4.5',
     'description': 'dbt adapter for IBM db2 for i',
     'long_description': "# dbt-db2fori\n\nA [dbt](https://www.getdbt.com/) adapter for IBM's DB2 for i v7.2+. The connection to the warehouse is through `ODBC` and requires that `pyodbc` is installed. All credits to [dbt-sqlserver adapter](https://github.com/dbt-msft/dbt-sqlserver) and [dbt-ibmdb2](https://github.com/aurany/dbt-ibmdb2) projects that heavily inspired this adapter.\n\n## Why this adapter?\nA similar adapter [dbt-ibmdb2](https://github.com/aurany/dbt-ibmdb2) exists, however, [dbt-ibmdb2](https://github.com/aurany/dbt-ibmdb2) uses the `ibm_db` Python package to connect to IBM DB2. This adapter connects to the warehouse using `pyodbc`\n\n## Features\nThe following materializations are supported:\n\n- Incremental\n- Snapshot\n- View\n- Table\n\nEphemeral models have not been tested yet. \n\n\n## Installation\nUse pip to install:\n```bash\npip install dbt-db2fori\n```\nAn example `profiles.yml` is:\n```bash\ndefault:\n    outputs:\n        dev:\n            type: db2_for_i\n            threads: 4\n            driver: IBM i Access ODBC Driver\n            system: system\n            username: username\n            password: password\n            database: db\n            schema: schema\n\n    target: dev\n```\n\nTo report a bug or request a feature, open an [issue](https://github.com/kaysef/dbt-db2fori/issues/new)\n",
     'author': 'Seth O',
     'author_email': 'sdowusu@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kaysef/dbt-db2fori',
```

### Comparing `dbt_db2fori-1.4.1/PKG-INFO` & `dbt_db2fori-1.4.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dbt-db2fori
-Version: 1.4.1
+Version: 1.4.5
 Summary: dbt adapter for IBM db2 for i
 Home-page: https://github.com/kaysef/dbt-db2fori
 License: MIT
 Author: Seth O
 Author-email: sdowusu@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dbt-core (>=1.3.2,<2.0.0)
-Requires-Dist: pyodbc (>=4.0.35,<5.0.0)
+Requires-Dist: dbt-core (==1.4.5)
+Requires-Dist: pyodbc (>=4.0.39,<5.0.0)
 Project-URL: Documentation, https://github.com/kaysef/dbt-db2fori
 Project-URL: Repository, https://github.com/kaysef/dbt-db2fori
 Description-Content-Type: text/markdown
 
 # dbt-db2fori
 
 A [dbt](https://www.getdbt.com/) adapter for IBM's DB2 for i v7.2+. The connection to the warehouse is through `ODBC` and requires that `pyodbc` is installed. All credits to [dbt-sqlserver adapter](https://github.com/dbt-msft/dbt-sqlserver) and [dbt-ibmdb2](https://github.com/aurany/dbt-ibmdb2) projects that heavily inspired this adapter.
```

