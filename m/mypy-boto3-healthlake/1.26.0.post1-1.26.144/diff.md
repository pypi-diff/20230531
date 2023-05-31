# Comparing `tmp/mypy-boto3-healthlake-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-healthlake-1.26.144.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-healthlake-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:30 2022, max compression
+gzip compressed data, was "mypy-boto3-healthlake-1.26.144.tar", last modified: Wed May 31 19:48:12 2023, max compression
```

## Comparing `mypy-boto3-healthlake-1.26.0.post1.tar` & `mypy-boto3-healthlake-1.26.144.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:30.680826 mypy-boto3-healthlake-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:35:33.000000 mypy-boto3-healthlake-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13393 2022-11-01 21:43:30.672826 mypy-boto3-healthlake-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11940 2022-11-01 21:35:33.000000 mypy-boto3-healthlake-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:30.672826 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake/
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-01 21:35:33.000000 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-11-01 21:35:33.000000 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-11-01 21:35:33.000000 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12027 2022-11-01 21:35:33.000000 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    12007 2022-11-01 21:35:33.000000 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7338 2022-11-01 21:35:34.000000 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7336 2022-11-01 21:35:34.000000 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:35:33.000000 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    13373 2022-11-01 21:35:34.000000 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    13354 2022-11-01 21:35:34.000000 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:35:33.000000 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:30.672826 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13393 2022-11-01 21:43:30.000000 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-11-01 21:43:30.000000 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:30.000000 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:30.000000 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:30.000000 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-01 21:43:30.000000 mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:30.680826 mypy-boto3-healthlake-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-11-01 21:35:33.000000 mypy-boto3-healthlake-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:48:12.452929 mypy-boto3-healthlake-1.26.144/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-05-31 19:48:12.452929 mypy-boto3-healthlake-1.26.144/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12022 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:48:12.432929 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-05-31 19:47:31.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-05-31 19:47:31.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:48:12.452929 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-05-31 19:48:12.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-31 19:48:12.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:48:12.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:48:12.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 19:48:12.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 19:48:12.000000 mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:48:12.452929 mypy-boto3-healthlake-1.26.144/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-31 19:47:30.000000 mypy-boto3-healthlake-1.26.144/setup.py
```

### Comparing `mypy-boto3-healthlake-1.26.0.post1/LICENSE` & `mypy-boto3-healthlake-1.26.144/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-healthlake-1.26.0.post1/PKG-INFO` & `mypy-boto3-healthlake-1.26.144/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-healthlake
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.HealthLake 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.144
+Summary: Type annotations for boto3.HealthLake 1.26.144 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-healthlake"></a>
 
 # mypy-boto3-healthlake
 
 [![PyPI - mypy-boto3-healthlake](https://img.shields.io/pypi/v/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-healthlake?color=blue)](https://pypistats.org/packages/mypy-boto3-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthLake 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[boto3.HealthLake 1.26.144](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-healthlake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -274,39 +275,41 @@
 ### Literals
 
 `mypy_boto3_healthlake.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_healthlake.literals import (
+    AuthorizationStrategyType,
     CmkTypeType,
     DatastoreStatusType,
     FHIRVersionType,
     JobStatusType,
     PreloadDataTypeType,
     HealthLakeServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
-def check_value(value: CmkTypeType) -> bool:
+def check_value(value: AuthorizationStrategyType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_healthlake.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_healthlake.type_defs import (
+    IdentityProviderConfigurationTypeDef,
     PreloadDataConfigTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     DatastoreFilterTypeDef,
     DeleteFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRExportJobRequestRequestTypeDef,
@@ -338,53 +341,53 @@
     DescribeFHIRExportJobResponseTypeDef,
     ListFHIRExportJobsResponseTypeDef,
     DescribeFHIRImportJobResponseTypeDef,
     ListFHIRImportJobsResponseTypeDef,
 )
 
 
-def get_structure() -> PreloadDataConfigTypeDef:
+def get_structure() -> IdentityProviderConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-healthlake-1.26.0.post1/README.md` & `mypy-boto3-healthlake-1.26.144/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-healthlake"></a>
 
 # mypy-boto3-healthlake
 
 [![PyPI - mypy-boto3-healthlake](https://img.shields.io/pypi/v/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-healthlake?color=blue)](https://pypistats.org/packages/mypy-boto3-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthLake 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[boto3.HealthLake 1.26.144](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-healthlake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -243,39 +243,41 @@
 ### Literals
 
 `mypy_boto3_healthlake.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_healthlake.literals import (
+    AuthorizationStrategyType,
     CmkTypeType,
     DatastoreStatusType,
     FHIRVersionType,
     JobStatusType,
     PreloadDataTypeType,
     HealthLakeServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
-def check_value(value: CmkTypeType) -> bool:
+def check_value(value: AuthorizationStrategyType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_healthlake.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_healthlake.type_defs import (
+    IdentityProviderConfigurationTypeDef,
     PreloadDataConfigTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     DatastoreFilterTypeDef,
     DeleteFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRExportJobRequestRequestTypeDef,
@@ -307,53 +309,53 @@
     DescribeFHIRExportJobResponseTypeDef,
     ListFHIRExportJobsResponseTypeDef,
     DescribeFHIRImportJobResponseTypeDef,
     ListFHIRImportJobsResponseTypeDef,
 )
 
 
-def get_structure() -> PreloadDataConfigTypeDef:
+def get_structure() -> IdentityProviderConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake/client.py` & `mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from .type_defs import (
     CreateFHIRDatastoreResponseTypeDef,
     DatastoreFilterTypeDef,
     DeleteFHIRDatastoreResponseTypeDef,
     DescribeFHIRDatastoreResponseTypeDef,
     DescribeFHIRExportJobResponseTypeDef,
     DescribeFHIRImportJobResponseTypeDef,
+    IdentityProviderConfigurationTypeDef,
     InputDataConfigTypeDef,
     ListFHIRDatastoresResponseTypeDef,
     ListFHIRExportJobsResponseTypeDef,
     ListFHIRImportJobsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     OutputDataConfigTypeDef,
     PreloadDataConfigTypeDef,
@@ -104,36 +105,33 @@
         self,
         *,
         DatastoreTypeVersion: Literal["R4"],
         DatastoreName: str = ...,
         SseConfiguration: SseConfigurationTypeDef = ...,
         PreloadDataConfig: PreloadDataConfigTypeDef = ...,
         ClientToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
+        IdentityProviderConfiguration: IdentityProviderConfigurationTypeDef = ...
     ) -> CreateFHIRDatastoreResponseTypeDef:
         """
         Creates a Data Store that can ingest and export FHIR formatted data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.create_fhir_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#create_fhir_datastore)
         """
 
-    def delete_fhir_datastore(
-        self, *, DatastoreId: str = ...
-    ) -> DeleteFHIRDatastoreResponseTypeDef:
+    def delete_fhir_datastore(self, *, DatastoreId: str) -> DeleteFHIRDatastoreResponseTypeDef:
         """
         Deletes a Data Store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.delete_fhir_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#delete_fhir_datastore)
         """
 
-    def describe_fhir_datastore(
-        self, *, DatastoreId: str = ...
-    ) -> DescribeFHIRDatastoreResponseTypeDef:
+    def describe_fhir_datastore(self, *, DatastoreId: str) -> DescribeFHIRDatastoreResponseTypeDef:
         """
         Gets the properties associated with the FHIR Data Store, including the Data
         Store ID, Data Store ARN, Data Store name, Data Store status, created at, Data
         Store type version, and Data Store endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.describe_fhir_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#describe_fhir_datastore)
@@ -261,15 +259,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.start_fhir_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#start_fhir_import_job)
         """
 
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
-        Adds a user specifed key and value tag to a Data Store.
+        Adds a user specified key and value tag to a Data Store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#tag_resource)
         """
 
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
```

### Comparing `mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake/client.pyi` & `mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from .type_defs import (
     CreateFHIRDatastoreResponseTypeDef,
     DatastoreFilterTypeDef,
     DeleteFHIRDatastoreResponseTypeDef,
     DescribeFHIRDatastoreResponseTypeDef,
     DescribeFHIRExportJobResponseTypeDef,
     DescribeFHIRImportJobResponseTypeDef,
+    IdentityProviderConfigurationTypeDef,
     InputDataConfigTypeDef,
     ListFHIRDatastoresResponseTypeDef,
     ListFHIRExportJobsResponseTypeDef,
     ListFHIRImportJobsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     OutputDataConfigTypeDef,
     PreloadDataConfigTypeDef,
@@ -97,34 +98,31 @@
         self,
         *,
         DatastoreTypeVersion: Literal["R4"],
         DatastoreName: str = ...,
         SseConfiguration: SseConfigurationTypeDef = ...,
         PreloadDataConfig: PreloadDataConfigTypeDef = ...,
         ClientToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
+        IdentityProviderConfiguration: IdentityProviderConfigurationTypeDef = ...
     ) -> CreateFHIRDatastoreResponseTypeDef:
         """
         Creates a Data Store that can ingest and export FHIR formatted data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.create_fhir_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#create_fhir_datastore)
         """
-    def delete_fhir_datastore(
-        self, *, DatastoreId: str = ...
-    ) -> DeleteFHIRDatastoreResponseTypeDef:
+    def delete_fhir_datastore(self, *, DatastoreId: str) -> DeleteFHIRDatastoreResponseTypeDef:
         """
         Deletes a Data Store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.delete_fhir_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#delete_fhir_datastore)
         """
-    def describe_fhir_datastore(
-        self, *, DatastoreId: str = ...
-    ) -> DescribeFHIRDatastoreResponseTypeDef:
+    def describe_fhir_datastore(self, *, DatastoreId: str) -> DescribeFHIRDatastoreResponseTypeDef:
         """
         Gets the properties associated with the FHIR Data Store, including the Data
         Store ID, Data Store ARN, Data Store name, Data Store status, created at, Data
         Store type version, and Data Store endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.describe_fhir_datastore)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#describe_fhir_datastore)
@@ -242,15 +240,15 @@
         Begins a FHIR Import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.start_fhir_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#start_fhir_import_job)
         """
     def tag_resource(self, *, ResourceARN: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
-        Adds a user specifed key and value tag to a Data Store.
+        Adds a user specified key and value tag to a Data Store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/client/#tag_resource)
         """
     def untag_resource(self, *, ResourceARN: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from a Data Store.
```

### Comparing `mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake/literals.py` & `mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/literals.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,44 +2,54 @@
 Type annotations for healthlake service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_healthlake.literals import CmkTypeType
+    from mypy_boto3_healthlake.literals import AuthorizationStrategyType
 
-    data: CmkTypeType = "AWS_OWNED_KMS_KEY"
+    data: AuthorizationStrategyType = "AWS_AUTH"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
+    "AuthorizationStrategyType",
     "CmkTypeType",
     "DatastoreStatusType",
     "FHIRVersionType",
     "JobStatusType",
     "PreloadDataTypeType",
     "HealthLakeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
+AuthorizationStrategyType = Literal["AWS_AUTH", "SMART_ON_FHIR_V1"]
 CmkTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_MANAGED_KMS_KEY"]
 DatastoreStatusType = Literal["ACTIVE", "CREATING", "DELETED", "DELETING"]
 FHIRVersionType = Literal["R4"]
-JobStatusType = Literal["COMPLETED", "COMPLETED_WITH_ERRORS", "FAILED", "IN_PROGRESS", "SUBMITTED"]
+JobStatusType = Literal[
+    "CANCEL_COMPLETED",
+    "CANCEL_FAILED",
+    "CANCEL_IN_PROGRESS",
+    "CANCEL_SUBMITTED",
+    "COMPLETED",
+    "COMPLETED_WITH_ERRORS",
+    "FAILED",
+    "IN_PROGRESS",
+    "SUBMITTED",
+]
 PreloadDataTypeType = Literal["SYNTHEA"]
 HealthLakeServiceName = Literal["healthlake"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -58,14 +68,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -75,27 +86,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -124,14 +139,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -176,51 +192,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -233,14 +255,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -252,28 +275,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -282,14 +310,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -300,55 +329,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -366,8 +403,8 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-RegionName = Literal["us-east-1", "us-east-2", "us-west-2"]
+RegionName = Literal["ap-south-1", "us-east-1", "us-east-2", "us-west-2"]
```

### Comparing `mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake/literals.pyi` & `mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/literals.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,42 +2,56 @@
 Type annotations for healthlake service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_healthlake.literals import CmkTypeType
+    from mypy_boto3_healthlake.literals import AuthorizationStrategyType
 
-    data: CmkTypeType = "AWS_OWNED_KMS_KEY"
+    data: AuthorizationStrategyType = "AWS_AUTH"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
+    "AuthorizationStrategyType",
     "CmkTypeType",
     "DatastoreStatusType",
     "FHIRVersionType",
     "JobStatusType",
     "PreloadDataTypeType",
     "HealthLakeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
+AuthorizationStrategyType = Literal["AWS_AUTH", "SMART_ON_FHIR_V1"]
 CmkTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_MANAGED_KMS_KEY"]
 DatastoreStatusType = Literal["ACTIVE", "CREATING", "DELETED", "DELETING"]
 FHIRVersionType = Literal["R4"]
-JobStatusType = Literal["COMPLETED", "COMPLETED_WITH_ERRORS", "FAILED", "IN_PROGRESS", "SUBMITTED"]
+JobStatusType = Literal[
+    "CANCEL_COMPLETED",
+    "CANCEL_FAILED",
+    "CANCEL_IN_PROGRESS",
+    "CANCEL_SUBMITTED",
+    "COMPLETED",
+    "COMPLETED_WITH_ERRORS",
+    "FAILED",
+    "IN_PROGRESS",
+    "SUBMITTED",
+]
 PreloadDataTypeType = Literal["SYNTHEA"]
 HealthLakeServiceName = Literal["healthlake"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -56,14 +70,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -73,27 +88,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -122,14 +141,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -174,51 +194,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -231,14 +257,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -250,28 +277,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -280,14 +312,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -298,55 +331,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -364,8 +405,8 @@
     "glacier",
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
-RegionName = Literal["us-east-1", "us-east-2", "us-west-2"]
+RegionName = Literal["ap-south-1", "us-east-1", "us-east-2", "us-west-2"]
```

### Comparing `mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake/type_defs.py` & `mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,36 +2,37 @@
 Type annotations for healthlake service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_healthlake.type_defs import PreloadDataConfigTypeDef
+    from mypy_boto3_healthlake.type_defs import IdentityProviderConfigurationTypeDef
 
-    data: PreloadDataConfigTypeDef = {...}
+    data: IdentityProviderConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
-from .literals import CmkTypeType, DatastoreStatusType, JobStatusType
+from .literals import AuthorizationStrategyType, CmkTypeType, DatastoreStatusType, JobStatusType
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "IdentityProviderConfigurationTypeDef",
     "PreloadDataConfigTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DatastoreFilterTypeDef",
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRExportJobRequestRequestTypeDef",
@@ -62,14 +63,37 @@
     "ListFHIRDatastoresResponseTypeDef",
     "DescribeFHIRExportJobResponseTypeDef",
     "ListFHIRExportJobsResponseTypeDef",
     "DescribeFHIRImportJobResponseTypeDef",
     "ListFHIRImportJobsResponseTypeDef",
 )
 
+_RequiredIdentityProviderConfigurationTypeDef = TypedDict(
+    "_RequiredIdentityProviderConfigurationTypeDef",
+    {
+        "AuthorizationStrategy": AuthorizationStrategyType,
+    },
+)
+_OptionalIdentityProviderConfigurationTypeDef = TypedDict(
+    "_OptionalIdentityProviderConfigurationTypeDef",
+    {
+        "FineGrainedAuthorizationEnabled": bool,
+        "Metadata": str,
+        "IdpLambdaArn": str,
+    },
+    total=False,
+)
+
+
+class IdentityProviderConfigurationTypeDef(
+    _RequiredIdentityProviderConfigurationTypeDef, _OptionalIdentityProviderConfigurationTypeDef
+):
+    pass
+
+
 PreloadDataConfigTypeDef = TypedDict(
     "PreloadDataConfigTypeDef",
     {
         "PreloadDataType": Literal["SYNTHEA"],
     },
 )
 
@@ -104,23 +128,21 @@
 )
 
 DeleteFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
-    total=False,
 )
 
 DescribeFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
-    total=False,
 )
 
 DescribeFHIRExportJobRequestRequestTypeDef = TypedDict(
     "DescribeFHIRExportJobRequestRequestTypeDef",
     {
         "DatastoreId": str,
         "JobId": str,
@@ -334,14 +356,15 @@
     "_OptionalCreateFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreName": str,
         "SseConfiguration": SseConfigurationTypeDef,
         "PreloadDataConfig": PreloadDataConfigTypeDef,
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
+        "IdentityProviderConfiguration": IdentityProviderConfigurationTypeDef,
     },
     total=False,
 )
 
 
 class CreateFHIRDatastoreRequestRequestTypeDef(
     _RequiredCreateFHIRDatastoreRequestRequestTypeDef,
@@ -363,14 +386,15 @@
 _OptionalDatastorePropertiesTypeDef = TypedDict(
     "_OptionalDatastorePropertiesTypeDef",
     {
         "DatastoreName": str,
         "CreatedAt": datetime,
         "SseConfiguration": SseConfigurationTypeDef,
         "PreloadDataConfig": PreloadDataConfigTypeDef,
+        "IdentityProviderConfiguration": IdentityProviderConfigurationTypeDef,
     },
     total=False,
 )
 
 
 class DatastorePropertiesTypeDef(
     _RequiredDatastorePropertiesTypeDef, _OptionalDatastorePropertiesTypeDef
```

### Comparing `mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake/type_defs.pyi` & `mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -2,35 +2,36 @@
 Type annotations for healthlake service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_healthlake.type_defs import PreloadDataConfigTypeDef
+    from mypy_boto3_healthlake.type_defs import IdentityProviderConfigurationTypeDef
 
-    data: PreloadDataConfigTypeDef = {...}
+    data: IdentityProviderConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
-from .literals import CmkTypeType, DatastoreStatusType, JobStatusType
+from .literals import AuthorizationStrategyType, CmkTypeType, DatastoreStatusType, JobStatusType
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "IdentityProviderConfigurationTypeDef",
     "PreloadDataConfigTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DatastoreFilterTypeDef",
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRExportJobRequestRequestTypeDef",
@@ -61,14 +62,35 @@
     "ListFHIRDatastoresResponseTypeDef",
     "DescribeFHIRExportJobResponseTypeDef",
     "ListFHIRExportJobsResponseTypeDef",
     "DescribeFHIRImportJobResponseTypeDef",
     "ListFHIRImportJobsResponseTypeDef",
 )
 
+_RequiredIdentityProviderConfigurationTypeDef = TypedDict(
+    "_RequiredIdentityProviderConfigurationTypeDef",
+    {
+        "AuthorizationStrategy": AuthorizationStrategyType,
+    },
+)
+_OptionalIdentityProviderConfigurationTypeDef = TypedDict(
+    "_OptionalIdentityProviderConfigurationTypeDef",
+    {
+        "FineGrainedAuthorizationEnabled": bool,
+        "Metadata": str,
+        "IdpLambdaArn": str,
+    },
+    total=False,
+)
+
+class IdentityProviderConfigurationTypeDef(
+    _RequiredIdentityProviderConfigurationTypeDef, _OptionalIdentityProviderConfigurationTypeDef
+):
+    pass
+
 PreloadDataConfigTypeDef = TypedDict(
     "PreloadDataConfigTypeDef",
     {
         "PreloadDataType": Literal["SYNTHEA"],
     },
 )
 
@@ -103,23 +125,21 @@
 )
 
 DeleteFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
-    total=False,
 )
 
 DescribeFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
-    total=False,
 )
 
 DescribeFHIRExportJobRequestRequestTypeDef = TypedDict(
     "DescribeFHIRExportJobRequestRequestTypeDef",
     {
         "DatastoreId": str,
         "JobId": str,
@@ -327,14 +347,15 @@
     "_OptionalCreateFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreName": str,
         "SseConfiguration": SseConfigurationTypeDef,
         "PreloadDataConfig": PreloadDataConfigTypeDef,
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
+        "IdentityProviderConfiguration": IdentityProviderConfigurationTypeDef,
     },
     total=False,
 )
 
 class CreateFHIRDatastoreRequestRequestTypeDef(
     _RequiredCreateFHIRDatastoreRequestRequestTypeDef,
     _OptionalCreateFHIRDatastoreRequestRequestTypeDef,
@@ -354,14 +375,15 @@
 _OptionalDatastorePropertiesTypeDef = TypedDict(
     "_OptionalDatastorePropertiesTypeDef",
     {
         "DatastoreName": str,
         "CreatedAt": datetime,
         "SseConfiguration": SseConfigurationTypeDef,
         "PreloadDataConfig": PreloadDataConfigTypeDef,
+        "IdentityProviderConfiguration": IdentityProviderConfigurationTypeDef,
     },
     total=False,
 )
 
 class DatastorePropertiesTypeDef(
     _RequiredDatastorePropertiesTypeDef, _OptionalDatastorePropertiesTypeDef
 ):
```

### Comparing `mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake.egg-info/PKG-INFO` & `mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-healthlake
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.HealthLake 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.144
+Summary: Type annotations for boto3.HealthLake 1.26.144 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-healthlake"></a>
 
 # mypy-boto3-healthlake
 
 [![PyPI - mypy-boto3-healthlake](https://img.shields.io/pypi/v/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-healthlake?color=blue)](https://pypistats.org/packages/mypy-boto3-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthLake 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[boto3.HealthLake 1.26.144](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-healthlake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -274,39 +275,41 @@
 ### Literals
 
 `mypy_boto3_healthlake.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
 ```python
 from mypy_boto3_healthlake.literals import (
+    AuthorizationStrategyType,
     CmkTypeType,
     DatastoreStatusType,
     FHIRVersionType,
     JobStatusType,
     PreloadDataTypeType,
     HealthLakeServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
-def check_value(value: CmkTypeType) -> bool:
+def check_value(value: AuthorizationStrategyType) -> bool:
     ...
 ```
 
 <a id="typed-dictionaries"></a>
 
 ### Typed dictionaries
 
 `mypy_boto3_healthlake.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_healthlake.type_defs import (
+    IdentityProviderConfigurationTypeDef,
     PreloadDataConfigTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     DatastoreFilterTypeDef,
     DeleteFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRExportJobRequestRequestTypeDef,
@@ -338,53 +341,53 @@
     DescribeFHIRExportJobResponseTypeDef,
     ListFHIRExportJobsResponseTypeDef,
     DescribeFHIRImportJobResponseTypeDef,
     ListFHIRImportJobsResponseTypeDef,
 )
 
 
-def get_structure() -> PreloadDataConfigTypeDef:
+def get_structure() -> IdentityProviderConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-healthlake-1.26.0.post1/mypy_boto3_healthlake.egg-info/SOURCES.txt` & `mypy-boto3-healthlake-1.26.144/mypy_boto3_healthlake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.26.0.post1/setup.py` & `mypy-boto3-healthlake-1.26.144/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-healthlake.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-healthlake",
-    version="1.26.0.post1",
+    version="1.26.144",
     packages=["mypy_boto3_healthlake"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.HealthLake 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.HealthLake 1.26.144 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 healthlake type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_healthlake": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_healthlake": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

