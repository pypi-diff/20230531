# Comparing `tmp/mypy-boto3-m2-1.26.31.tar.gz` & `tmp/mypy-boto3-m2-1.26.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-m2-1.26.31.tar", last modified: Thu Dec 15 20:33:07 2022, max compression
+gzip compressed data, was "mypy-boto3-m2-1.26.57.tar", last modified: Wed Jan 25 20:48:07 2023, max compression
```

## Comparing `mypy-boto3-m2-1.26.31.tar` & `mypy-boto3-m2-1.26.57.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 20:33:07.308147 mypy-boto3-m2-1.26.31/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-15 20:32:26.000000 mypy-boto3-m2-1.26.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18394 2022-12-15 20:33:07.308147 mypy-boto3-m2-1.26.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2022-12-15 20:32:26.000000 mypy-boto3-m2-1.26.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 20:33:07.292147 mypy-boto3-m2-1.26.31/mypy_boto3_m2/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2022-12-15 20:32:26.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2022-12-15 20:32:26.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2022-12-15 20:32:26.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27335 2022-12-15 20:32:26.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27287 2022-12-15 20:32:26.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9922 2022-12-15 20:32:26.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2022-12-15 20:32:26.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11364 2022-12-15 20:32:26.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2022-12-15 20:32:26.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-15 20:32:26.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40722 2022-12-15 20:32:27.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40658 2022-12-15 20:32:27.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-15 20:32:26.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 20:33:07.308147 mypy-boto3-m2-1.26.31/mypy_boto3_m2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18394 2022-12-15 20:33:07.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2022-12-15 20:33:07.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 20:33:07.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 20:33:07.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-15 20:33:07.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-15 20:33:07.000000 mypy-boto3-m2-1.26.31/mypy_boto3_m2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-15 20:33:07.308147 mypy-boto3-m2-1.26.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2022-12-15 20:32:26.000000 mypy-boto3-m2-1.26.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:48:07.692256 mypy-boto3-m2-1.26.57/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-25 20:47:28.000000 mypy-boto3-m2-1.26.57/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18394 2023-01-25 20:48:07.676256 mypy-boto3-m2-1.26.57/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-01-25 20:47:28.000000 mypy-boto3-m2-1.26.57/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:48:07.676256 mypy-boto3-m2-1.26.57/mypy_boto3_m2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-01-25 20:47:28.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-01-25 20:47:28.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-25 20:47:28.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27335 2023-01-25 20:47:29.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27287 2023-01-25 20:47:28.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-01-25 20:47:29.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-01-25 20:47:29.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-01-25 20:47:29.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-01-25 20:47:29.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 20:47:28.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40890 2023-01-25 20:47:29.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40826 2023-01-25 20:47:29.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-25 20:47:28.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 20:48:07.676256 mypy-boto3-m2-1.26.57/mypy_boto3_m2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18394 2023-01-25 20:48:07.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-01-25 20:48:07.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 20:48:07.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 20:48:07.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-25 20:48:07.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-25 20:48:07.000000 mypy-boto3-m2-1.26.57/mypy_boto3_m2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 20:48:07.692256 mypy-boto3-m2-1.26.57/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-01-25 20:47:28.000000 mypy-boto3-m2-1.26.57/setup.py
```

### Comparing `mypy-boto3-m2-1.26.31/LICENSE` & `mypy-boto3-m2-1.26.57/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.26.31/PKG-INFO` & `mypy-boto3-m2-1.26.57/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-m2
-Version: 1.26.31
-Summary: Type annotations for boto3.MainframeModernization 1.26.31 service generated with mypy-boto3-builder 7.12.0
+Version: 1.26.57
+Summary: Type annotations for boto3.MainframeModernization 1.26.57 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-m2?color=blue)](https://pypistats.org/packages/mypy-boto3-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MainframeModernization 1.26.31](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[boto3.MainframeModernization 1.26.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-m2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -367,15 +367,14 @@
 ```python
 from mypy_boto3_m2.type_defs import (
     AlternateKeyTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
     FileBatchJobDefinitionTypeDef,
     ScriptBatchJobDefinitionTypeDef,
-    BatchJobExecutionSummaryTypeDef,
     FileBatchJobIdentifierTypeDef,
     ScriptBatchJobIdentifierTypeDef,
     CancelBatchJobExecutionRequestRequestTypeDef,
     DefinitionTypeDef,
     ResponseMetadataTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     HighAvailabilityConfigTypeDef,
@@ -425,19 +424,17 @@
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     CreateDataSetImportTaskResponseTypeDef,
     CreateDeploymentResponseTypeDef,
     CreateEnvironmentResponseTypeDef,
     GetApplicationVersionResponseTypeDef,
-    GetBatchJobExecutionResponseTypeDef,
     GetDeploymentResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    ListBatchJobExecutionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartBatchJobResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
     DataSetImportTaskTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     ListDataSetsResponseTypeDef,
@@ -455,20 +452,23 @@
     ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
     ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     PendingMaintenanceTypeDef,
     VsamAttributesTypeDef,
     VsamDetailAttributesTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
+    BatchJobExecutionSummaryTypeDef,
+    GetBatchJobExecutionResponseTypeDef,
     StartBatchJobRequestRequestTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     GetEnvironmentResponseTypeDef,
     DatasetOrgAttributesTypeDef,
     DatasetDetailOrgAttributesTypeDef,
+    ListBatchJobExecutionsResponseTypeDef,
     DataSetTypeDef,
     GetDataSetDetailsResponseTypeDef,
     DataSetImportItemTypeDef,
     DataSetImportConfigTypeDef,
     CreateDataSetImportTaskRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-m2-1.26.31/README.md` & `mypy-boto3-m2-1.26.57/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-m2?color=blue)](https://pypistats.org/packages/mypy-boto3-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MainframeModernization 1.26.31](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[boto3.MainframeModernization 1.26.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-m2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -335,15 +335,14 @@
 ```python
 from mypy_boto3_m2.type_defs import (
     AlternateKeyTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
     FileBatchJobDefinitionTypeDef,
     ScriptBatchJobDefinitionTypeDef,
-    BatchJobExecutionSummaryTypeDef,
     FileBatchJobIdentifierTypeDef,
     ScriptBatchJobIdentifierTypeDef,
     CancelBatchJobExecutionRequestRequestTypeDef,
     DefinitionTypeDef,
     ResponseMetadataTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     HighAvailabilityConfigTypeDef,
@@ -393,19 +392,17 @@
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     CreateDataSetImportTaskResponseTypeDef,
     CreateDeploymentResponseTypeDef,
     CreateEnvironmentResponseTypeDef,
     GetApplicationVersionResponseTypeDef,
-    GetBatchJobExecutionResponseTypeDef,
     GetDeploymentResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    ListBatchJobExecutionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartBatchJobResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
     DataSetImportTaskTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     ListDataSetsResponseTypeDef,
@@ -423,20 +420,23 @@
     ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
     ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     PendingMaintenanceTypeDef,
     VsamAttributesTypeDef,
     VsamDetailAttributesTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
+    BatchJobExecutionSummaryTypeDef,
+    GetBatchJobExecutionResponseTypeDef,
     StartBatchJobRequestRequestTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     GetEnvironmentResponseTypeDef,
     DatasetOrgAttributesTypeDef,
     DatasetDetailOrgAttributesTypeDef,
+    ListBatchJobExecutionsResponseTypeDef,
     DataSetTypeDef,
     GetDataSetDetailsResponseTypeDef,
     DataSetImportItemTypeDef,
     DataSetImportConfigTypeDef,
     CreateDataSetImportTaskRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-m2-1.26.31/mypy_boto3_m2/__init__.py` & `mypy-boto3-m2-1.26.57/mypy_boto3_m2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.26.31/mypy_boto3_m2/__init__.pyi` & `mypy-boto3-m2-1.26.57/mypy_boto3_m2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.26.31/mypy_boto3_m2/__main__.py` & `mypy-boto3-m2-1.26.57/mypy_boto3_m2/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MainframeModernization 1.26.31\nVersion:        "
-        " 1.26.31\nBuilder version: 7.12.0\nDocs:           "
+        "Type annotations for boto3.MainframeModernization 1.26.57\nVersion:        "
+        " 1.26.57\nBuilder version: 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.31")
+    print("1.26.57")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-m2-1.26.31/mypy_boto3_m2/client.py` & `mypy-boto3-m2-1.26.57/mypy_boto3_m2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.26.31/mypy_boto3_m2/client.pyi` & `mypy-boto3-m2-1.26.57/mypy_boto3_m2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.26.31/mypy_boto3_m2/literals.py` & `mypy-boto3-m2-1.26.57/mypy_boto3_m2/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ApplicationDeploymentLifecycleType",
     "ApplicationLifecycleType",
     "ApplicationVersionLifecycleType",
     "BatchJobExecutionStatusType",
     "BatchJobTypeType",
     "DataSetTaskLifecycleType",
@@ -41,15 +40,14 @@
     "MainframeModernizationServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApplicationDeploymentLifecycleType = Literal["Deployed", "Deploying"]
 ApplicationLifecycleType = Literal[
     "Available",
     "Created",
     "Creating",
     "Deleting",
     "Deleting From Environment",
@@ -126,14 +124,15 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
@@ -251,30 +250,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
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
@@ -444,19 +446,22 @@
     "list_data_sets",
     "list_deployments",
     "list_engine_versions",
     "list_environments",
 ]
 RegionName = Literal[
     "ap-northeast-1",
+    "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "sa-east-1",
     "us-east-1",
+    "us-east-2",
+    "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-m2-1.26.31/mypy_boto3_m2/literals.pyi` & `mypy-boto3-m2-1.26.57/mypy_boto3_m2/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ApplicationDeploymentLifecycleType",
     "ApplicationLifecycleType",
     "ApplicationVersionLifecycleType",
     "BatchJobExecutionStatusType",
     "BatchJobTypeType",
     "DataSetTaskLifecycleType",
@@ -40,14 +41,15 @@
     "MainframeModernizationServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ApplicationDeploymentLifecycleType = Literal["Deployed", "Deploying"]
 ApplicationLifecycleType = Literal[
     "Available",
     "Created",
     "Creating",
     "Deleting",
     "Deleting From Environment",
@@ -124,14 +126,15 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
@@ -249,30 +252,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
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
@@ -442,19 +448,22 @@
     "list_data_sets",
     "list_deployments",
     "list_engine_versions",
     "list_environments",
 ]
 RegionName = Literal[
     "ap-northeast-1",
+    "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "sa-east-1",
     "us-east-1",
+    "us-east-2",
+    "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-m2-1.26.31/mypy_boto3_m2/paginator.py` & `mypy-boto3-m2-1.26.57/mypy_boto3_m2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.26.31/mypy_boto3_m2/paginator.pyi` & `mypy-boto3-m2-1.26.57/mypy_boto3_m2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.26.31/mypy_boto3_m2/type_defs.py` & `mypy-boto3-m2-1.26.57/mypy_boto3_m2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
 __all__ = (
     "AlternateKeyTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationVersionSummaryTypeDef",
     "FileBatchJobDefinitionTypeDef",
     "ScriptBatchJobDefinitionTypeDef",
-    "BatchJobExecutionSummaryTypeDef",
     "FileBatchJobIdentifierTypeDef",
     "ScriptBatchJobIdentifierTypeDef",
     "CancelBatchJobExecutionRequestRequestTypeDef",
     "DefinitionTypeDef",
     "ResponseMetadataTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "HighAvailabilityConfigTypeDef",
@@ -93,19 +92,17 @@
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "CreateDataSetImportTaskResponseTypeDef",
     "CreateDeploymentResponseTypeDef",
     "CreateEnvironmentResponseTypeDef",
     "GetApplicationVersionResponseTypeDef",
-    "GetBatchJobExecutionResponseTypeDef",
     "GetDeploymentResponseTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "ListBatchJobExecutionsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartBatchJobResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "DataSetImportTaskTypeDef",
     "GetDataSetImportTaskResponseTypeDef",
     "ListDataSetsResponseTypeDef",
@@ -123,20 +120,23 @@
     "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
     "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "PendingMaintenanceTypeDef",
     "VsamAttributesTypeDef",
     "VsamDetailAttributesTypeDef",
     "ListBatchJobDefinitionsResponseTypeDef",
+    "BatchJobExecutionSummaryTypeDef",
+    "GetBatchJobExecutionResponseTypeDef",
     "StartBatchJobRequestRequestTypeDef",
     "ListDataSetImportHistoryResponseTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
     "GetEnvironmentResponseTypeDef",
     "DatasetOrgAttributesTypeDef",
     "DatasetDetailOrgAttributesTypeDef",
+    "ListBatchJobExecutionsResponseTypeDef",
     "DataSetTypeDef",
     "GetDataSetDetailsResponseTypeDef",
     "DataSetImportItemTypeDef",
     "DataSetImportConfigTypeDef",
     "CreateDataSetImportTaskRequestRequestTypeDef",
 )
 
@@ -239,41 +239,14 @@
 ScriptBatchJobDefinitionTypeDef = TypedDict(
     "ScriptBatchJobDefinitionTypeDef",
     {
         "scriptName": str,
     },
 )
 
-_RequiredBatchJobExecutionSummaryTypeDef = TypedDict(
-    "_RequiredBatchJobExecutionSummaryTypeDef",
-    {
-        "applicationId": str,
-        "executionId": str,
-        "startTime": datetime,
-        "status": BatchJobExecutionStatusType,
-    },
-)
-_OptionalBatchJobExecutionSummaryTypeDef = TypedDict(
-    "_OptionalBatchJobExecutionSummaryTypeDef",
-    {
-        "endTime": datetime,
-        "jobId": str,
-        "jobName": str,
-        "jobType": BatchJobTypeType,
-    },
-    total=False,
-)
-
-
-class BatchJobExecutionSummaryTypeDef(
-    _RequiredBatchJobExecutionSummaryTypeDef, _OptionalBatchJobExecutionSummaryTypeDef
-):
-    pass
-
-
 _RequiredFileBatchJobIdentifierTypeDef = TypedDict(
     "_RequiredFileBatchJobIdentifierTypeDef",
     {
         "fileName": str,
     },
 )
 _OptionalFileBatchJobIdentifierTypeDef = TypedDict(
@@ -995,31 +968,14 @@
         "name": str,
         "status": ApplicationVersionLifecycleType,
         "statusReason": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetBatchJobExecutionResponseTypeDef = TypedDict(
-    "GetBatchJobExecutionResponseTypeDef",
-    {
-        "applicationId": str,
-        "endTime": datetime,
-        "executionId": str,
-        "jobId": str,
-        "jobName": str,
-        "jobType": BatchJobTypeType,
-        "jobUser": str,
-        "startTime": datetime,
-        "status": BatchJobExecutionStatusType,
-        "statusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetDeploymentResponseTypeDef = TypedDict(
     "GetDeploymentResponseTypeDef",
     {
         "applicationId": str,
         "applicationVersion": int,
         "creationTime": datetime,
         "deploymentId": str,
@@ -1044,23 +1000,14 @@
     {
         "applications": List[ApplicationSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListBatchJobExecutionsResponseTypeDef = TypedDict(
-    "ListBatchJobExecutionsResponseTypeDef",
-    {
-        "batchJobExecutions": List[BatchJobExecutionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1396,14 +1343,62 @@
     {
         "batchJobDefinitions": List[BatchJobDefinitionTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredBatchJobExecutionSummaryTypeDef = TypedDict(
+    "_RequiredBatchJobExecutionSummaryTypeDef",
+    {
+        "applicationId": str,
+        "executionId": str,
+        "startTime": datetime,
+        "status": BatchJobExecutionStatusType,
+    },
+)
+_OptionalBatchJobExecutionSummaryTypeDef = TypedDict(
+    "_OptionalBatchJobExecutionSummaryTypeDef",
+    {
+        "batchJobIdentifier": BatchJobIdentifierTypeDef,
+        "endTime": datetime,
+        "jobId": str,
+        "jobName": str,
+        "jobType": BatchJobTypeType,
+        "returnCode": str,
+    },
+    total=False,
+)
+
+
+class BatchJobExecutionSummaryTypeDef(
+    _RequiredBatchJobExecutionSummaryTypeDef, _OptionalBatchJobExecutionSummaryTypeDef
+):
+    pass
+
+
+GetBatchJobExecutionResponseTypeDef = TypedDict(
+    "GetBatchJobExecutionResponseTypeDef",
+    {
+        "applicationId": str,
+        "batchJobIdentifier": BatchJobIdentifierTypeDef,
+        "endTime": datetime,
+        "executionId": str,
+        "jobId": str,
+        "jobName": str,
+        "jobType": BatchJobTypeType,
+        "jobUser": str,
+        "returnCode": str,
+        "startTime": datetime,
+        "status": BatchJobExecutionStatusType,
+        "statusReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredStartBatchJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartBatchJobRequestRequestTypeDef",
     {
         "applicationId": str,
         "batchJobIdentifier": BatchJobIdentifierTypeDef,
     },
 )
@@ -1507,14 +1502,23 @@
     {
         "gdg": GdgDetailAttributesTypeDef,
         "vsam": VsamDetailAttributesTypeDef,
     },
     total=False,
 )
 
+ListBatchJobExecutionsResponseTypeDef = TypedDict(
+    "ListBatchJobExecutionsResponseTypeDef",
+    {
+        "batchJobExecutions": List[BatchJobExecutionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredDataSetTypeDef = TypedDict(
     "_RequiredDataSetTypeDef",
     {
         "datasetName": str,
         "datasetOrg": DatasetOrgAttributesTypeDef,
         "recordLength": RecordLengthTypeDef,
     },
```

### Comparing `mypy-boto3-m2-1.26.31/mypy_boto3_m2/type_defs.pyi` & `mypy-boto3-m2-1.26.57/mypy_boto3_m2/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
 __all__ = (
     "AlternateKeyTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationVersionSummaryTypeDef",
     "FileBatchJobDefinitionTypeDef",
     "ScriptBatchJobDefinitionTypeDef",
-    "BatchJobExecutionSummaryTypeDef",
     "FileBatchJobIdentifierTypeDef",
     "ScriptBatchJobIdentifierTypeDef",
     "CancelBatchJobExecutionRequestRequestTypeDef",
     "DefinitionTypeDef",
     "ResponseMetadataTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "HighAvailabilityConfigTypeDef",
@@ -92,19 +91,17 @@
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "CreateDataSetImportTaskResponseTypeDef",
     "CreateDeploymentResponseTypeDef",
     "CreateEnvironmentResponseTypeDef",
     "GetApplicationVersionResponseTypeDef",
-    "GetBatchJobExecutionResponseTypeDef",
     "GetDeploymentResponseTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "ListBatchJobExecutionsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartBatchJobResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "DataSetImportTaskTypeDef",
     "GetDataSetImportTaskResponseTypeDef",
     "ListDataSetsResponseTypeDef",
@@ -122,20 +119,23 @@
     "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
     "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "PendingMaintenanceTypeDef",
     "VsamAttributesTypeDef",
     "VsamDetailAttributesTypeDef",
     "ListBatchJobDefinitionsResponseTypeDef",
+    "BatchJobExecutionSummaryTypeDef",
+    "GetBatchJobExecutionResponseTypeDef",
     "StartBatchJobRequestRequestTypeDef",
     "ListDataSetImportHistoryResponseTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
     "GetEnvironmentResponseTypeDef",
     "DatasetOrgAttributesTypeDef",
     "DatasetDetailOrgAttributesTypeDef",
+    "ListBatchJobExecutionsResponseTypeDef",
     "DataSetTypeDef",
     "GetDataSetDetailsResponseTypeDef",
     "DataSetImportItemTypeDef",
     "DataSetImportConfigTypeDef",
     "CreateDataSetImportTaskRequestRequestTypeDef",
 )
 
@@ -230,39 +230,14 @@
 ScriptBatchJobDefinitionTypeDef = TypedDict(
     "ScriptBatchJobDefinitionTypeDef",
     {
         "scriptName": str,
     },
 )
 
-_RequiredBatchJobExecutionSummaryTypeDef = TypedDict(
-    "_RequiredBatchJobExecutionSummaryTypeDef",
-    {
-        "applicationId": str,
-        "executionId": str,
-        "startTime": datetime,
-        "status": BatchJobExecutionStatusType,
-    },
-)
-_OptionalBatchJobExecutionSummaryTypeDef = TypedDict(
-    "_OptionalBatchJobExecutionSummaryTypeDef",
-    {
-        "endTime": datetime,
-        "jobId": str,
-        "jobName": str,
-        "jobType": BatchJobTypeType,
-    },
-    total=False,
-)
-
-class BatchJobExecutionSummaryTypeDef(
-    _RequiredBatchJobExecutionSummaryTypeDef, _OptionalBatchJobExecutionSummaryTypeDef
-):
-    pass
-
 _RequiredFileBatchJobIdentifierTypeDef = TypedDict(
     "_RequiredFileBatchJobIdentifierTypeDef",
     {
         "fileName": str,
     },
 )
 _OptionalFileBatchJobIdentifierTypeDef = TypedDict(
@@ -952,31 +927,14 @@
         "name": str,
         "status": ApplicationVersionLifecycleType,
         "statusReason": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetBatchJobExecutionResponseTypeDef = TypedDict(
-    "GetBatchJobExecutionResponseTypeDef",
-    {
-        "applicationId": str,
-        "endTime": datetime,
-        "executionId": str,
-        "jobId": str,
-        "jobName": str,
-        "jobType": BatchJobTypeType,
-        "jobUser": str,
-        "startTime": datetime,
-        "status": BatchJobExecutionStatusType,
-        "statusReason": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetDeploymentResponseTypeDef = TypedDict(
     "GetDeploymentResponseTypeDef",
     {
         "applicationId": str,
         "applicationVersion": int,
         "creationTime": datetime,
         "deploymentId": str,
@@ -1001,23 +959,14 @@
     {
         "applications": List[ApplicationSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListBatchJobExecutionsResponseTypeDef = TypedDict(
-    "ListBatchJobExecutionsResponseTypeDef",
-    {
-        "batchJobExecutions": List[BatchJobExecutionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1339,14 +1288,60 @@
     {
         "batchJobDefinitions": List[BatchJobDefinitionTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredBatchJobExecutionSummaryTypeDef = TypedDict(
+    "_RequiredBatchJobExecutionSummaryTypeDef",
+    {
+        "applicationId": str,
+        "executionId": str,
+        "startTime": datetime,
+        "status": BatchJobExecutionStatusType,
+    },
+)
+_OptionalBatchJobExecutionSummaryTypeDef = TypedDict(
+    "_OptionalBatchJobExecutionSummaryTypeDef",
+    {
+        "batchJobIdentifier": BatchJobIdentifierTypeDef,
+        "endTime": datetime,
+        "jobId": str,
+        "jobName": str,
+        "jobType": BatchJobTypeType,
+        "returnCode": str,
+    },
+    total=False,
+)
+
+class BatchJobExecutionSummaryTypeDef(
+    _RequiredBatchJobExecutionSummaryTypeDef, _OptionalBatchJobExecutionSummaryTypeDef
+):
+    pass
+
+GetBatchJobExecutionResponseTypeDef = TypedDict(
+    "GetBatchJobExecutionResponseTypeDef",
+    {
+        "applicationId": str,
+        "batchJobIdentifier": BatchJobIdentifierTypeDef,
+        "endTime": datetime,
+        "executionId": str,
+        "jobId": str,
+        "jobName": str,
+        "jobType": BatchJobTypeType,
+        "jobUser": str,
+        "returnCode": str,
+        "startTime": datetime,
+        "status": BatchJobExecutionStatusType,
+        "statusReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredStartBatchJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartBatchJobRequestRequestTypeDef",
     {
         "applicationId": str,
         "batchJobIdentifier": BatchJobIdentifierTypeDef,
     },
 )
@@ -1446,14 +1441,23 @@
     {
         "gdg": GdgDetailAttributesTypeDef,
         "vsam": VsamDetailAttributesTypeDef,
     },
     total=False,
 )
 
+ListBatchJobExecutionsResponseTypeDef = TypedDict(
+    "ListBatchJobExecutionsResponseTypeDef",
+    {
+        "batchJobExecutions": List[BatchJobExecutionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredDataSetTypeDef = TypedDict(
     "_RequiredDataSetTypeDef",
     {
         "datasetName": str,
         "datasetOrg": DatasetOrgAttributesTypeDef,
         "recordLength": RecordLengthTypeDef,
     },
```

### Comparing `mypy-boto3-m2-1.26.31/mypy_boto3_m2.egg-info/PKG-INFO` & `mypy-boto3-m2-1.26.57/mypy_boto3_m2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-m2
-Version: 1.26.31
-Summary: Type annotations for boto3.MainframeModernization 1.26.31 service generated with mypy-boto3-builder 7.12.0
+Version: 1.26.57
+Summary: Type annotations for boto3.MainframeModernization 1.26.57 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-m2.svg?color=blue)](https://pypi.org/project/mypy-boto3-m2)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-m2?color=blue)](https://pypistats.org/packages/mypy-boto3-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MainframeModernization 1.26.31](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
+[boto3.MainframeModernization 1.26.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-m2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_m2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -367,15 +367,14 @@
 ```python
 from mypy_boto3_m2.type_defs import (
     AlternateKeyTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
     FileBatchJobDefinitionTypeDef,
     ScriptBatchJobDefinitionTypeDef,
-    BatchJobExecutionSummaryTypeDef,
     FileBatchJobIdentifierTypeDef,
     ScriptBatchJobIdentifierTypeDef,
     CancelBatchJobExecutionRequestRequestTypeDef,
     DefinitionTypeDef,
     ResponseMetadataTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     HighAvailabilityConfigTypeDef,
@@ -425,19 +424,17 @@
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     CreateDataSetImportTaskResponseTypeDef,
     CreateDeploymentResponseTypeDef,
     CreateEnvironmentResponseTypeDef,
     GetApplicationVersionResponseTypeDef,
-    GetBatchJobExecutionResponseTypeDef,
     GetDeploymentResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    ListBatchJobExecutionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartBatchJobResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
     DataSetImportTaskTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     ListDataSetsResponseTypeDef,
@@ -455,20 +452,23 @@
     ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
     ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     PendingMaintenanceTypeDef,
     VsamAttributesTypeDef,
     VsamDetailAttributesTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
+    BatchJobExecutionSummaryTypeDef,
+    GetBatchJobExecutionResponseTypeDef,
     StartBatchJobRequestRequestTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
     GetEnvironmentResponseTypeDef,
     DatasetOrgAttributesTypeDef,
     DatasetDetailOrgAttributesTypeDef,
+    ListBatchJobExecutionsResponseTypeDef,
     DataSetTypeDef,
     GetDataSetDetailsResponseTypeDef,
     DataSetImportItemTypeDef,
     DataSetImportConfigTypeDef,
     CreateDataSetImportTaskRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-m2-1.26.31/mypy_boto3_m2.egg-info/SOURCES.txt` & `mypy-boto3-m2-1.26.57/mypy_boto3_m2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-m2-1.26.31/setup.py` & `mypy-boto3-m2-1.26.57/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-m2",
-    version="1.26.31",
+    version="1.26.57",
     packages=["mypy_boto3_m2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MainframeModernization 1.26.31 service generated with"
-        " mypy-boto3-builder 7.12.0"
+        "Type annotations for boto3.MainframeModernization 1.26.57 service generated with"
+        " mypy-boto3-builder 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

