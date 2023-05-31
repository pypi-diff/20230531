# Comparing `tmp/braincube-aws-core-alpha-0.0.28.tar.gz` & `tmp/braincube-aws-core-alpha-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-alpha-0.0.28.tar", last modified: Tue May 16 06:39:30 2023, max compression
+gzip compressed data, was "braincube-aws-core-alpha-0.0.29.tar", last modified: Wed May 31 12:26:54 2023, max compression
```

## Comparing `braincube-aws-core-alpha-0.0.28.tar` & `braincube-aws-core-alpha-0.0.29.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-16 06:39:30.063559 braincube-aws-core-alpha-0.0.28/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.28/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9091 2023-05-16 06:39:30.063844 braincube-aws-core-alpha-0.0.28/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8338 2023-05-12 07:04:00.000000 braincube-aws-core-alpha-0.0.28/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.28/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-16 06:39:30.065204 braincube-aws-core-alpha-0.0.28/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.28/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-16 06:39:30.048211 braincube-aws-core-alpha-0.0.28/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-16 06:39:30.052795 braincube-aws-core-alpha-0.0.28/src/braincube_aws_core_alpha.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9091 2023-05-16 06:39:30.000000 braincube-aws-core-alpha-0.0.28/src/braincube_aws_core_alpha.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-16 06:39:30.000000 braincube-aws-core-alpha-0.0.28/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-16 06:39:30.000000 braincube-aws-core-alpha-0.0.28/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-16 06:39:30.000000 braincube-aws-core-alpha-0.0.28/src/braincube_aws_core_alpha.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-16 06:39:30.000000 braincube-aws-core-alpha-0.0.28/src/braincube_aws_core_alpha.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-16 06:39:30.053381 braincube-aws-core-alpha-0.0.28/src/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.28/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-16 06:39:30.055855 braincube-aws-core-alpha-0.0.28/src/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.28/src/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-05-15 18:52:22.000000 braincube-aws-core-alpha-0.0.28/src/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-alpha-0.0.28/src/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4110 2023-05-15 11:28:42.000000 braincube-aws-core-alpha-0.0.28/src/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    33110 2023-05-15 18:42:36.000000 braincube-aws-core-alpha-0.0.28/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-16 06:39:30.057300 braincube-aws-core-alpha-0.0.28/src/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.28/src/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-alpha-0.0.28/src/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-alpha-0.0.28/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-16 06:39:30.059531 braincube-aws-core-alpha-0.0.28/src/core/rest/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.28/src/core/rest/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-alpha-0.0.28/src/core/rest/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3722 2023-05-11 10:52:31.000000 braincube-aws-core-alpha-0.0.28/src/core/rest/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3598 2023-05-11 17:50:46.000000 braincube-aws-core-alpha-0.0.28/src/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-16 06:39:30.062966 braincube-aws-core-alpha-0.0.28/src/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.28/src/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-alpha-0.0.28/src/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-alpha-0.0.28/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-31 12:26:54.287366 braincube-aws-core-alpha-0.0.29/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.29/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8896 2023-05-31 12:26:54.287642 braincube-aws-core-alpha-0.0.29/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8143 2023-05-23 10:50:40.000000 braincube-aws-core-alpha-0.0.29/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.29/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-31 12:26:54.290181 braincube-aws-core-alpha-0.0.29/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.29/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-31 12:26:54.271682 braincube-aws-core-alpha-0.0.29/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-31 12:26:54.276520 braincube-aws-core-alpha-0.0.29/src/braincube_aws_core_alpha.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8896 2023-05-31 12:26:54.000000 braincube-aws-core-alpha-0.0.29/src/braincube_aws_core_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-31 12:26:54.000000 braincube-aws-core-alpha-0.0.29/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-31 12:26:54.000000 braincube-aws-core-alpha-0.0.29/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-31 12:26:54.000000 braincube-aws-core-alpha-0.0.29/src/braincube_aws_core_alpha.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-31 12:26:54.000000 braincube-aws-core-alpha-0.0.29/src/braincube_aws_core_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-31 12:26:54.276889 braincube-aws-core-alpha-0.0.29/src/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.29/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-31 12:26:54.279478 braincube-aws-core-alpha-0.0.29/src/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.29/src/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-05-15 18:52:22.000000 braincube-aws-core-alpha-0.0.29/src/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-alpha-0.0.29/src/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4110 2023-05-23 08:56:40.000000 braincube-aws-core-alpha-0.0.29/src/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    33020 2023-05-31 12:25:52.000000 braincube-aws-core-alpha-0.0.29/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-31 12:26:54.281857 braincube-aws-core-alpha-0.0.29/src/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.29/src/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-alpha-0.0.29/src/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-alpha-0.0.29/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-31 12:26:54.284627 braincube-aws-core-alpha-0.0.29/src/core/rest/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.29/src/core/rest/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-alpha-0.0.29/src/core/rest/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3722 2023-05-11 10:52:31.000000 braincube-aws-core-alpha-0.0.29/src/core/rest/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3598 2023-05-11 17:50:46.000000 braincube-aws-core-alpha-0.0.29/src/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-31 12:26:54.286753 braincube-aws-core-alpha-0.0.29/src/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.29/src/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-alpha-0.0.29/src/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-alpha-0.0.29/src/core/utils/data.py
```

### Comparing `braincube-aws-core-alpha-0.0.28/LICENSE` & `braincube-aws-core-alpha-0.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.28/PKG-INFO` & `braincube-aws-core-alpha-0.0.29/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: braincube-aws-core-alpha
-Version: 0.0.28
-Summary: Microframework for python aws lambdas
-Home-page: https://bitbucket.org/braincube-common/core-aws.git
-Author: Braincube
-Author-email: v.boudis@braincube.gr
-License: MIT
-Keywords: python,amazon,aws,lambda,routing,dal,injection
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: <4,>=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # braincube-aws-core
 
 Microframework for Python AWS lambdas.
 
 [![Language](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org/)
 [![pypi](https://img.shields.io/pypi/v/braincube-aws-core-alpha.svg)](https://pypi.org/project/braincube-aws-core-alpha/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
@@ -39,46 +19,47 @@
 - [pypika](https://github.com/kayak/pypika) - Python Query Builder.
 
 ### Application Controllers Example
 
 ```python
 import asyncio
 
+from uuid import uuid4
 from http import HTTPStatus
 
 from core.rest.data import HTTPRequest, HTTPResponse
 from core.rest.app_module import AppModule
 from core.rest.app_controller import AppController
 
 from pydantic import BaseModel
 
 
 class AccountDto(BaseModel):
-    id: int
     iban: str
     bban: str
 
 
-_accounts = [
-    AccountDto(1, "EUR27100777770209299700", "EURC12345612345678"),
-    AccountDto(2, "GR27100777770209299700", "GRC12345612345678"),
-]
+data = {
+    "a0a412d9-87ef-474b-9ac8-b682ec5e0fb3": AccountDto(iban="EUR27100777770209299700", bban="EURC12345612345678"),
+    "5ebc25bd-e152-4a70-b251-d68e43be581e": AccountDto(iban="GR27100777770209299700", bban="GRC12345612345678"),
+}
 
 app = AppController("/accounts")
 
 
 @app.get("/{id}")
 async def get_account(request: HTTPRequest) -> HTTPResponse:
-    account = next((a for a in _accounts if a.id == request.path_parameters["id"]), None)
+    account = data.get(request.path_parameters["id"])
     return HTTPResponse(HTTPStatus.OK if account else HTTPStatus.NO_CONTENT, account)
 
 
 @app.post()
 async def create_account(request: HTTPRequest[AccountDto]) -> HTTPResponse:
-    return HTTPResponse(HTTPStatus.OK)
+    data[uuid4()] = request.body
+    return HTTPResponse(HTTPStatus.CREATED)
 
 
 loop = asyncio.get_event_loop()
 
 module = AppModule([app])
 
 
@@ -115,43 +96,43 @@
 from core.dal.postgres_repository import PostgresRepository
 
 # schema definition
 equities = Schema(
     table="equities",
     alias="e",
     primary_key=["id"],
-    order=[Order(type=OrderType.asc, alias="name")],
-    statement_fields=[
-        StatementField(alias="isTypeOne",
-                       statement="CASE WHEN e.type = 1 then True else False END",
-                       relations_aliases=[])
-    ],
     columns=[
         Column(name="id", updatable=False, insertable=False),
         Column(name="name"),
         Column(name="type"),
         Column(name="issuer_id", alias="issuerId"),
         Column(name="industry_sector", alias="industrySector"),
         Column(name="isin"),
         Column(name="reference"),
         Column(name="bloomberg_code", alias="bloombergCode"),
         Column(name="market_symbol", alias="marketSymbol"),
         Column(name="currency"),
         Column(name="country", ),
         Column(name="min_amount", alias="minAmount"),
     ],
+    statement_fields=[
+        StatementField(alias="isTypeOne", statement="CASE WHEN e.type = 1 then True else False END")
+    ],
+    order=[
+        Order(type=OrderType.asc, alias="name")
+    ],
     relations=[
         Relation(
             table="parties",
             alias="p",
-            join_forced=False,
             columns=[
                 SimpleColumn(name="name"),
                 SimpleColumn(name="short_name", alias="shortName"),
             ],
+            join_forced=False,
             join_type=JoinType.left,
             join_through=JoinThrough(from_column_name="issuer_id", to_column_name="id")
         )
     ]
 )
 
 
@@ -164,100 +145,90 @@
 
 # repository usage
 
 request = HTTPRequest()
 
 repo = EquitiesRepo(await get_pool())
 
-await repo.find_by_pk(key=Key(request.path_parameters["id"]), aliases=request.query_parameters.fields)
+await repo.find_by_pk(Key(request.path_parameters["id"]), request.query_parameters.fields)
 
-await repo.exists_by_pk(key=Key("9448a57b-f686-4935-b152-566baab712db"))
+await repo.exists_by_pk(Key("9448a57b-f686-4935-b152-566baab712db"))
 
 await repo.find_one(
-    aliases=request.query_parameters.fields,
+    request.query_parameters.fields,
     conditions=request.query_parameters.conditions,
     order=request.query_parameters.order)
 
 await repo.find_all(
-    aliases=request.query_parameters.fields,
+    request.query_parameters.fields,
     conditions=request.query_parameters.conditions,
     order=request.query_parameters.order)
 
-await repo.find_all_by_pk([
-    Key("9448a57b-f686-4935-b152-566baab712db"),
-    Key("43c8ec37-9a59-44eb-be90-def391ba2f02")],
+await repo.find_all_by_pk(
+    [
+        Key("9448a57b-f686-4935-b152-566baab712db"),
+        Key("43c8ec37-9a59-44eb-be90-def391ba2f02")
+    ],
     aliases=request.query_parameters.fields,
     order=request.query_parameters.order)
 
 await repo.find_many(
-    aliases=request.query_parameters.fields,
+    request.query_parameters.fields,
     conditions=request.query_parameters.conditions,
     page=request.query_parameters.page,
     order=request.query_parameters.order)
 
-await repo.insert(
-    data={
-        "name": "Bursa de Valori Bucuresti SA",
-        "type": 1,
-        "industrySector": 40,
-        "isin": "ROBVBAACNOR0",
-        "bloombergCode": "BBG000BBWMC5",
-        "marketSymbol": "BVB RO Equity",
-        "currency": "RON",
-        "country": "RO",
-    })
+await repo.insert({
+    "name": "Bursa de Valori Bucuresti SA",
+    "type": 1,
+    "industrySector": 40,
+    "isin": "ROBVBAACNOR0",
+    "bloombergCode": "BBG000BBWMC5",
+    "marketSymbol": "BVB RO Equity",
+    "currency": "RON",
+    "country": "RO",
+})
 
 await repo.insert_bulk(
     aliases=["name", "type", "industrySector", "isin", "bloombergCode", "marketSymbol", "currency", "country"],
     data=[
         ["Bursa de Valori Bucuresti SA", 1, 40, "ROBVBAACNOR0", "BBG000BBWMC5", "BVB RO Equity", "RON", "RO"],
         ["Citigroup Inc", 1, 40, "US1729674242", "BBG000FY4S11", "C US Equity", "USD", "US"],
         ["Coca-Cola HBC AG", 1, 49, "CH0198251305", "BBG004HJV2T1", "EEE GA Equity", "EUR", "GR"],
     ]
 )
 
-await repo.update(
-    data={
-        "type": 1,
-        "isin": 40,
-    },
-    conditions=request.query_parameters.conditions,
-    returning_aliases=request.query_parameters.fields)
-
-await repo.update_by_pk(
-    Key("9448a57b-f686-4935-b152-566baab712db"),
-    data={
-        "type": 1,
-        "isin": 40,
-    }, returning_aliases=[])
+await repo.update({
+    "type": 1,
+    "isin": 40,
+}, request.query_parameters.conditions, request.query_parameters.fields)
+
+await repo.update_by_pk(Key("9448a57b-f686-4935-b152-566baab712db"), {
+    "type": 1,
+    "isin": 40
+})
 
-await repo.delete(
-    conditions=request.query_parameters.conditions,
-    returning_aliases=["id", "name", "type"])
+await repo.delete(request.query_parameters.conditions, ["id", "name", "type"])
 
-await repo.delete_by_pk(
-    Key("9448a57b-f686-4935-b152-566baab712db"),
-    returning_aliases=["id", "name", "type"])
+await repo.delete_by_pk(Key("9448a57b-f686-4935-b152-566baab712db"), ["id", "name", "type"])
 
 await repo.fetch("SELECT * FROM equities WHERE type = $1 and isin = $2", [1, "TREEGYO00017"])
 
 await repo.fetch_one("SELECT * FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
 
 await repo.execute("DELETE FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
 ```
 
 ### Query params format
 
 ```
 fields=name, type, industrySector, isin, bloombergCode, parties_name, parties_shortName
-
 type=1
 isin=range(40, 49)
 id=any(9448a57b-f686-4935-b152-566baab712db, 43c8ec37-9a59-44eb-be90-def391ba2f02)
-
 page_no=1
 page_size=50
 top_size=50
 order=name, id DESC
 ```
 
 ### Local Development Requirements
```

### Comparing `braincube-aws-core-alpha-0.0.28/README.md` & `braincube-aws-core-alpha-0.0.29/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: braincube-aws-core-alpha
+Version: 0.0.29
+Summary: Microframework for python aws lambdas
+Home-page: https://bitbucket.org/braincube-common/core-aws.git
+Author: Braincube
+Author-email: v.boudis@braincube.gr
+License: MIT
+Keywords: python,amazon,aws,lambda,routing,dal,injection
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: <4,>=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # braincube-aws-core
 
 Microframework for Python AWS lambdas.
 
 [![Language](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org/)
 [![pypi](https://img.shields.io/pypi/v/braincube-aws-core-alpha.svg)](https://pypi.org/project/braincube-aws-core-alpha/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
@@ -19,46 +39,47 @@
 - [pypika](https://github.com/kayak/pypika) - Python Query Builder.
 
 ### Application Controllers Example
 
 ```python
 import asyncio
 
+from uuid import uuid4
 from http import HTTPStatus
 
 from core.rest.data import HTTPRequest, HTTPResponse
 from core.rest.app_module import AppModule
 from core.rest.app_controller import AppController
 
 from pydantic import BaseModel
 
 
 class AccountDto(BaseModel):
-    id: int
     iban: str
     bban: str
 
 
-_accounts = [
-    AccountDto(1, "EUR27100777770209299700", "EURC12345612345678"),
-    AccountDto(2, "GR27100777770209299700", "GRC12345612345678"),
-]
+data = {
+    "a0a412d9-87ef-474b-9ac8-b682ec5e0fb3": AccountDto(iban="EUR27100777770209299700", bban="EURC12345612345678"),
+    "5ebc25bd-e152-4a70-b251-d68e43be581e": AccountDto(iban="GR27100777770209299700", bban="GRC12345612345678"),
+}
 
 app = AppController("/accounts")
 
 
 @app.get("/{id}")
 async def get_account(request: HTTPRequest) -> HTTPResponse:
-    account = next((a for a in _accounts if a.id == request.path_parameters["id"]), None)
+    account = data.get(request.path_parameters["id"])
     return HTTPResponse(HTTPStatus.OK if account else HTTPStatus.NO_CONTENT, account)
 
 
 @app.post()
 async def create_account(request: HTTPRequest[AccountDto]) -> HTTPResponse:
-    return HTTPResponse(HTTPStatus.OK)
+    data[uuid4()] = request.body
+    return HTTPResponse(HTTPStatus.CREATED)
 
 
 loop = asyncio.get_event_loop()
 
 module = AppModule([app])
 
 
@@ -95,43 +116,43 @@
 from core.dal.postgres_repository import PostgresRepository
 
 # schema definition
 equities = Schema(
     table="equities",
     alias="e",
     primary_key=["id"],
-    order=[Order(type=OrderType.asc, alias="name")],
-    statement_fields=[
-        StatementField(alias="isTypeOne",
-                       statement="CASE WHEN e.type = 1 then True else False END",
-                       relations_aliases=[])
-    ],
     columns=[
         Column(name="id", updatable=False, insertable=False),
         Column(name="name"),
         Column(name="type"),
         Column(name="issuer_id", alias="issuerId"),
         Column(name="industry_sector", alias="industrySector"),
         Column(name="isin"),
         Column(name="reference"),
         Column(name="bloomberg_code", alias="bloombergCode"),
         Column(name="market_symbol", alias="marketSymbol"),
         Column(name="currency"),
         Column(name="country", ),
         Column(name="min_amount", alias="minAmount"),
     ],
+    statement_fields=[
+        StatementField(alias="isTypeOne", statement="CASE WHEN e.type = 1 then True else False END")
+    ],
+    order=[
+        Order(type=OrderType.asc, alias="name")
+    ],
     relations=[
         Relation(
             table="parties",
             alias="p",
-            join_forced=False,
             columns=[
                 SimpleColumn(name="name"),
                 SimpleColumn(name="short_name", alias="shortName"),
             ],
+            join_forced=False,
             join_type=JoinType.left,
             join_through=JoinThrough(from_column_name="issuer_id", to_column_name="id")
         )
     ]
 )
 
 
@@ -144,100 +165,90 @@
 
 # repository usage
 
 request = HTTPRequest()
 
 repo = EquitiesRepo(await get_pool())
 
-await repo.find_by_pk(key=Key(request.path_parameters["id"]), aliases=request.query_parameters.fields)
+await repo.find_by_pk(Key(request.path_parameters["id"]), request.query_parameters.fields)
 
-await repo.exists_by_pk(key=Key("9448a57b-f686-4935-b152-566baab712db"))
+await repo.exists_by_pk(Key("9448a57b-f686-4935-b152-566baab712db"))
 
 await repo.find_one(
-    aliases=request.query_parameters.fields,
+    request.query_parameters.fields,
     conditions=request.query_parameters.conditions,
     order=request.query_parameters.order)
 
 await repo.find_all(
-    aliases=request.query_parameters.fields,
+    request.query_parameters.fields,
     conditions=request.query_parameters.conditions,
     order=request.query_parameters.order)
 
-await repo.find_all_by_pk([
-    Key("9448a57b-f686-4935-b152-566baab712db"),
-    Key("43c8ec37-9a59-44eb-be90-def391ba2f02")],
+await repo.find_all_by_pk(
+    [
+        Key("9448a57b-f686-4935-b152-566baab712db"),
+        Key("43c8ec37-9a59-44eb-be90-def391ba2f02")
+    ],
     aliases=request.query_parameters.fields,
     order=request.query_parameters.order)
 
 await repo.find_many(
-    aliases=request.query_parameters.fields,
+    request.query_parameters.fields,
     conditions=request.query_parameters.conditions,
     page=request.query_parameters.page,
     order=request.query_parameters.order)
 
-await repo.insert(
-    data={
-        "name": "Bursa de Valori Bucuresti SA",
-        "type": 1,
-        "industrySector": 40,
-        "isin": "ROBVBAACNOR0",
-        "bloombergCode": "BBG000BBWMC5",
-        "marketSymbol": "BVB RO Equity",
-        "currency": "RON",
-        "country": "RO",
-    })
+await repo.insert({
+    "name": "Bursa de Valori Bucuresti SA",
+    "type": 1,
+    "industrySector": 40,
+    "isin": "ROBVBAACNOR0",
+    "bloombergCode": "BBG000BBWMC5",
+    "marketSymbol": "BVB RO Equity",
+    "currency": "RON",
+    "country": "RO",
+})
 
 await repo.insert_bulk(
     aliases=["name", "type", "industrySector", "isin", "bloombergCode", "marketSymbol", "currency", "country"],
     data=[
         ["Bursa de Valori Bucuresti SA", 1, 40, "ROBVBAACNOR0", "BBG000BBWMC5", "BVB RO Equity", "RON", "RO"],
         ["Citigroup Inc", 1, 40, "US1729674242", "BBG000FY4S11", "C US Equity", "USD", "US"],
         ["Coca-Cola HBC AG", 1, 49, "CH0198251305", "BBG004HJV2T1", "EEE GA Equity", "EUR", "GR"],
     ]
 )
 
-await repo.update(
-    data={
-        "type": 1,
-        "isin": 40,
-    },
-    conditions=request.query_parameters.conditions,
-    returning_aliases=request.query_parameters.fields)
-
-await repo.update_by_pk(
-    Key("9448a57b-f686-4935-b152-566baab712db"),
-    data={
-        "type": 1,
-        "isin": 40,
-    }, returning_aliases=[])
+await repo.update({
+    "type": 1,
+    "isin": 40,
+}, request.query_parameters.conditions, request.query_parameters.fields)
+
+await repo.update_by_pk(Key("9448a57b-f686-4935-b152-566baab712db"), {
+    "type": 1,
+    "isin": 40
+})
 
-await repo.delete(
-    conditions=request.query_parameters.conditions,
-    returning_aliases=["id", "name", "type"])
+await repo.delete(request.query_parameters.conditions, ["id", "name", "type"])
 
-await repo.delete_by_pk(
-    Key("9448a57b-f686-4935-b152-566baab712db"),
-    returning_aliases=["id", "name", "type"])
+await repo.delete_by_pk(Key("9448a57b-f686-4935-b152-566baab712db"), ["id", "name", "type"])
 
 await repo.fetch("SELECT * FROM equities WHERE type = $1 and isin = $2", [1, "TREEGYO00017"])
 
 await repo.fetch_one("SELECT * FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
 
 await repo.execute("DELETE FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
 ```
 
 ### Query params format
 
 ```
 fields=name, type, industrySector, isin, bloombergCode, parties_name, parties_shortName
-
 type=1
 isin=range(40, 49)
 id=any(9448a57b-f686-4935-b152-566baab712db, 43c8ec37-9a59-44eb-be90-def391ba2f02)
-
 page_no=1
 page_size=50
 top_size=50
 order=name, id DESC
 ```
 
 ### Local Development Requirements
```

### Comparing `braincube-aws-core-alpha-0.0.28/setup.cfg` & `braincube-aws-core-alpha-0.0.29/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core-alpha
-version = 0.0.28
+version = 0.0.29
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
```

### Comparing `braincube-aws-core-alpha-0.0.28/src/braincube_aws_core_alpha.egg-info/PKG-INFO` & `braincube-aws-core-alpha-0.0.29/src/braincube_aws_core_alpha.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.28
+Version: 0.0.29
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
@@ -39,46 +39,47 @@
 - [pypika](https://github.com/kayak/pypika) - Python Query Builder.
 
 ### Application Controllers Example
 
 ```python
 import asyncio
 
+from uuid import uuid4
 from http import HTTPStatus
 
 from core.rest.data import HTTPRequest, HTTPResponse
 from core.rest.app_module import AppModule
 from core.rest.app_controller import AppController
 
 from pydantic import BaseModel
 
 
 class AccountDto(BaseModel):
-    id: int
     iban: str
     bban: str
 
 
-_accounts = [
-    AccountDto(1, "EUR27100777770209299700", "EURC12345612345678"),
-    AccountDto(2, "GR27100777770209299700", "GRC12345612345678"),
-]
+data = {
+    "a0a412d9-87ef-474b-9ac8-b682ec5e0fb3": AccountDto(iban="EUR27100777770209299700", bban="EURC12345612345678"),
+    "5ebc25bd-e152-4a70-b251-d68e43be581e": AccountDto(iban="GR27100777770209299700", bban="GRC12345612345678"),
+}
 
 app = AppController("/accounts")
 
 
 @app.get("/{id}")
 async def get_account(request: HTTPRequest) -> HTTPResponse:
-    account = next((a for a in _accounts if a.id == request.path_parameters["id"]), None)
+    account = data.get(request.path_parameters["id"])
     return HTTPResponse(HTTPStatus.OK if account else HTTPStatus.NO_CONTENT, account)
 
 
 @app.post()
 async def create_account(request: HTTPRequest[AccountDto]) -> HTTPResponse:
-    return HTTPResponse(HTTPStatus.OK)
+    data[uuid4()] = request.body
+    return HTTPResponse(HTTPStatus.CREATED)
 
 
 loop = asyncio.get_event_loop()
 
 module = AppModule([app])
 
 
@@ -115,43 +116,43 @@
 from core.dal.postgres_repository import PostgresRepository
 
 # schema definition
 equities = Schema(
     table="equities",
     alias="e",
     primary_key=["id"],
-    order=[Order(type=OrderType.asc, alias="name")],
-    statement_fields=[
-        StatementField(alias="isTypeOne",
-                       statement="CASE WHEN e.type = 1 then True else False END",
-                       relations_aliases=[])
-    ],
     columns=[
         Column(name="id", updatable=False, insertable=False),
         Column(name="name"),
         Column(name="type"),
         Column(name="issuer_id", alias="issuerId"),
         Column(name="industry_sector", alias="industrySector"),
         Column(name="isin"),
         Column(name="reference"),
         Column(name="bloomberg_code", alias="bloombergCode"),
         Column(name="market_symbol", alias="marketSymbol"),
         Column(name="currency"),
         Column(name="country", ),
         Column(name="min_amount", alias="minAmount"),
     ],
+    statement_fields=[
+        StatementField(alias="isTypeOne", statement="CASE WHEN e.type = 1 then True else False END")
+    ],
+    order=[
+        Order(type=OrderType.asc, alias="name")
+    ],
     relations=[
         Relation(
             table="parties",
             alias="p",
-            join_forced=False,
             columns=[
                 SimpleColumn(name="name"),
                 SimpleColumn(name="short_name", alias="shortName"),
             ],
+            join_forced=False,
             join_type=JoinType.left,
             join_through=JoinThrough(from_column_name="issuer_id", to_column_name="id")
         )
     ]
 )
 
 
@@ -164,100 +165,90 @@
 
 # repository usage
 
 request = HTTPRequest()
 
 repo = EquitiesRepo(await get_pool())
 
-await repo.find_by_pk(key=Key(request.path_parameters["id"]), aliases=request.query_parameters.fields)
+await repo.find_by_pk(Key(request.path_parameters["id"]), request.query_parameters.fields)
 
-await repo.exists_by_pk(key=Key("9448a57b-f686-4935-b152-566baab712db"))
+await repo.exists_by_pk(Key("9448a57b-f686-4935-b152-566baab712db"))
 
 await repo.find_one(
-    aliases=request.query_parameters.fields,
+    request.query_parameters.fields,
     conditions=request.query_parameters.conditions,
     order=request.query_parameters.order)
 
 await repo.find_all(
-    aliases=request.query_parameters.fields,
+    request.query_parameters.fields,
     conditions=request.query_parameters.conditions,
     order=request.query_parameters.order)
 
-await repo.find_all_by_pk([
-    Key("9448a57b-f686-4935-b152-566baab712db"),
-    Key("43c8ec37-9a59-44eb-be90-def391ba2f02")],
+await repo.find_all_by_pk(
+    [
+        Key("9448a57b-f686-4935-b152-566baab712db"),
+        Key("43c8ec37-9a59-44eb-be90-def391ba2f02")
+    ],
     aliases=request.query_parameters.fields,
     order=request.query_parameters.order)
 
 await repo.find_many(
-    aliases=request.query_parameters.fields,
+    request.query_parameters.fields,
     conditions=request.query_parameters.conditions,
     page=request.query_parameters.page,
     order=request.query_parameters.order)
 
-await repo.insert(
-    data={
-        "name": "Bursa de Valori Bucuresti SA",
-        "type": 1,
-        "industrySector": 40,
-        "isin": "ROBVBAACNOR0",
-        "bloombergCode": "BBG000BBWMC5",
-        "marketSymbol": "BVB RO Equity",
-        "currency": "RON",
-        "country": "RO",
-    })
+await repo.insert({
+    "name": "Bursa de Valori Bucuresti SA",
+    "type": 1,
+    "industrySector": 40,
+    "isin": "ROBVBAACNOR0",
+    "bloombergCode": "BBG000BBWMC5",
+    "marketSymbol": "BVB RO Equity",
+    "currency": "RON",
+    "country": "RO",
+})
 
 await repo.insert_bulk(
     aliases=["name", "type", "industrySector", "isin", "bloombergCode", "marketSymbol", "currency", "country"],
     data=[
         ["Bursa de Valori Bucuresti SA", 1, 40, "ROBVBAACNOR0", "BBG000BBWMC5", "BVB RO Equity", "RON", "RO"],
         ["Citigroup Inc", 1, 40, "US1729674242", "BBG000FY4S11", "C US Equity", "USD", "US"],
         ["Coca-Cola HBC AG", 1, 49, "CH0198251305", "BBG004HJV2T1", "EEE GA Equity", "EUR", "GR"],
     ]
 )
 
-await repo.update(
-    data={
-        "type": 1,
-        "isin": 40,
-    },
-    conditions=request.query_parameters.conditions,
-    returning_aliases=request.query_parameters.fields)
-
-await repo.update_by_pk(
-    Key("9448a57b-f686-4935-b152-566baab712db"),
-    data={
-        "type": 1,
-        "isin": 40,
-    }, returning_aliases=[])
+await repo.update({
+    "type": 1,
+    "isin": 40,
+}, request.query_parameters.conditions, request.query_parameters.fields)
+
+await repo.update_by_pk(Key("9448a57b-f686-4935-b152-566baab712db"), {
+    "type": 1,
+    "isin": 40
+})
 
-await repo.delete(
-    conditions=request.query_parameters.conditions,
-    returning_aliases=["id", "name", "type"])
+await repo.delete(request.query_parameters.conditions, ["id", "name", "type"])
 
-await repo.delete_by_pk(
-    Key("9448a57b-f686-4935-b152-566baab712db"),
-    returning_aliases=["id", "name", "type"])
+await repo.delete_by_pk(Key("9448a57b-f686-4935-b152-566baab712db"), ["id", "name", "type"])
 
 await repo.fetch("SELECT * FROM equities WHERE type = $1 and isin = $2", [1, "TREEGYO00017"])
 
 await repo.fetch_one("SELECT * FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
 
 await repo.execute("DELETE FROM equities WHERE id = $1", ["2b67122a-f47e-41b1-b7f7-53be5ca381a0"])
 ```
 
 ### Query params format
 
 ```
 fields=name, type, industrySector, isin, bloombergCode, parties_name, parties_shortName
-
 type=1
 isin=range(40, 49)
 id=any(9448a57b-f686-4935-b152-566baab712db, 43c8ec37-9a59-44eb-be90-def391ba2f02)
-
 page_no=1
 page_size=50
 top_size=50
 order=name, id DESC
 ```
 
 ### Local Development Requirements
```

### Comparing `braincube-aws-core-alpha-0.0.28/src/braincube_aws_core_alpha.egg-info/SOURCES.txt` & `braincube-aws-core-alpha-0.0.29/src/braincube_aws_core_alpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.28/src/core/dal/data.py` & `braincube-aws-core-alpha-0.0.29/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.28/src/core/dal/postgres_connection.py` & `braincube-aws-core-alpha-0.0.29/src/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.28/src/core/dal/postgres_repository.py` & `braincube-aws-core-alpha-0.0.29/src/core/dal/postgres_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -444,29 +444,29 @@
         :param order: Order that will be applied to query.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Record as returning type.
         """
 
         result = await self.find_one(self.__base_model_aliases(cls), conditions, order, connection)
 
-        return cls.construct(**result) if result else None
+        return cls(**result) if result else None
 
     async def find_by_pk_data(self, key: Key,
                               cls: type[T],
                               connection: Connection = None) -> T | None:
         """Find the record from passed key.
         :param key: Record identifier.
         :param cls: Result type.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Records as returning type.
         """
 
         result = await self.find_by_pk(key, self.__base_model_aliases(cls), connection)
 
-        return cls.construct(**result) if result else None
+        return cls(**result) if result else None
 
     async def find_all_data(self, cls: type[T],
                             conditions: list[Condition] | Criterion = None,
                             order: list[Order] = None,
                             connection: Connection = None) -> list[T]:
         """Find all records from passed filters.
         :param cls: Result type.
@@ -474,15 +474,15 @@
         :param order: Order in which the records will be returned.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Records as returning type.
         """
 
         results = await self.find_all(self.__base_model_aliases(cls), conditions, order, connection)
 
-        return [cls.construct(**r) for r in results] if results else None
+        return [cls(**r) for r in results] if results else None
 
     async def find_all_by_pk_data(self, keys: list[Key],
                                   cls: type[T],
                                   order: list[Order] = None,
                                   connection: Connection = None) -> list[T]:
         """Find all records from passed keys.
         :param keys: Records identifiers.
@@ -490,15 +490,15 @@
         :param order: Order in which the records will be returned.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Records as returning type.
         """
 
         results = await self.find_all_by_pk(keys, self.__base_model_aliases(cls), order, connection)
 
-        return [cls.construct(**r) for r in results] if results else None
+        return [cls(**r) for r in results] if results else None
 
     ####################################
     # Create
     ####################################
 
     async def insert(self, data: BaseModel | dict[str, any],
                      returning_aliases: list[str] = None,
@@ -534,15 +534,15 @@
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to insert-constraints or no master column is specified.
         :return: Execution results with returning type.
         """
 
         result = await self.insert(data, self.__base_model_aliases(returning), connection)
 
-        return returning.construct(**result) if result else None
+        return returning(**result) if result else None
 
     async def insert_bulk(self, aliases: list[str],
                           data: list[list],
                           returning_aliases: list[str] = None,
                           connection: Connection = None) -> list[dict[str, any]]:
         """Insert many records at once from list.
         :param aliases: Master column aliases.
@@ -642,15 +642,15 @@
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to update-constraints or no master column is specified.
         :return: Execution results with returning type.
         """
 
         results = await self.update(data, conditions, self.__base_model_aliases(returning), connection)
 
-        return [returning.construct(**r) for r in results] if results else None
+        return [returning(**r) for r in results] if results else None
 
     async def update_data_by_pk(self, key: Key,
                                 data: BaseModel | dict[str, any],
                                 returning: type[T],
                                 connection: Connection = None) -> T | None:
         """Update record with new data according to passed key using model.
         :param key: Record identifier.
@@ -659,15 +659,15 @@
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to update-constraints or no master column is specified.
         :return: Execution result with returning type.
         """
 
         result = await self.update_by_pk(key, data, self.__base_model_aliases(returning), connection)
 
-        return returning.construct(**result) if result else None
+        return returning(**result) if result else None
 
     ####################################
     # Delete
     ####################################
 
     async def delete(self, conditions: list[Condition] | Criterion,
                      returning_aliases: list[str] = None,
@@ -719,22 +719,22 @@
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise DeleteError: When conditions are empty.
         :return: Execution results with returning type.
         """
 
         results = await self.delete(conditions, self.__base_model_aliases(returning), connection)
 
-        return [returning.construct(**r) for r in results] if results else None
+        return [returning(**r) for r in results] if results else None
 
     async def delete_data_by_pk(self, key: Key,
                                 returning: type[T],
                                 connection: Connection = None) -> T | None:
         """Delete record according to passed key.
         :param key: Record identifier.
         :param returning: Result type.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Execution result with returning type.
         """
 
         result = await self.delete_by_pk(key, self.__base_model_aliases(returning), connection)
 
-        return returning.construct(**result) if result else None
+        return returning(**result) if result else None
```

### Comparing `braincube-aws-core-alpha-0.0.28/src/core/di/data.py` & `braincube-aws-core-alpha-0.0.29/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.28/src/core/di/injector.py` & `braincube-aws-core-alpha-0.0.29/src/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.28/src/core/rest/app_controller.py` & `braincube-aws-core-alpha-0.0.29/src/core/rest/app_controller.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.28/src/core/rest/app_module.py` & `braincube-aws-core-alpha-0.0.29/src/core/rest/app_module.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.28/src/core/rest/data.py` & `braincube-aws-core-alpha-0.0.29/src/core/rest/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.28/src/core/utils/convert.py` & `braincube-aws-core-alpha-0.0.29/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.28/src/core/utils/data.py` & `braincube-aws-core-alpha-0.0.29/src/core/utils/data.py`

 * *Files identical despite different names*

