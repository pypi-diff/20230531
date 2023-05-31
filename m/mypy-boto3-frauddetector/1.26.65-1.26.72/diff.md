# Comparing `tmp/mypy-boto3-frauddetector-1.26.65.tar.gz` & `tmp/mypy-boto3-frauddetector-1.26.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-frauddetector-1.26.65.tar", last modified: Mon Feb  6 20:47:28 2023, max compression
+gzip compressed data, was "mypy-boto3-frauddetector-1.26.72.tar", last modified: Wed Feb 15 22:27:56 2023, max compression
```

## Comparing `mypy-boto3-frauddetector-1.26.65.tar` & `mypy-boto3-frauddetector-1.26.72.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:28.165984 mypy-boto3-frauddetector-1.26.65/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-06 20:47:07.000000 mypy-boto3-frauddetector-1.26.65/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18545 2023-02-06 20:47:28.153984 mypy-boto3-frauddetector-1.26.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-02-06 20:47:07.000000 mypy-boto3-frauddetector-1.26.65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:28.153984 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-02-06 20:47:07.000000 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-06 20:47:07.000000 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-02-06 20:47:07.000000 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43452 2023-02-06 20:47:07.000000 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43377 2023-02-06 20:47:07.000000 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-02-06 20:47:07.000000 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-02-06 20:47:07.000000 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:07.000000 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55926 2023-02-06 20:47:09.000000 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55867 2023-02-06 20:47:08.000000 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-06 20:47:07.000000 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:28.153984 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18545 2023-02-06 20:47:28.000000 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-06 20:47:28.000000 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 20:47:28.000000 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 20:47:28.000000 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-06 20:47:28.000000 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-06 20:47:28.000000 mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 20:47:28.165984 mypy-boto3-frauddetector-1.26.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-02-06 20:47:07.000000 mypy-boto3-frauddetector-1.26.65/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.846127 mypy-boto3-frauddetector-1.26.72/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-15 22:27:07.000000 mypy-boto3-frauddetector-1.26.72/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18860 2023-02-15 22:27:56.846127 mypy-boto3-frauddetector-1.26.72/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-02-15 22:27:07.000000 mypy-boto3-frauddetector-1.26.72/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.846127 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-02-15 22:27:07.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-15 22:27:07.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-02-15 22:27:07.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46244 2023-02-15 22:27:08.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46164 2023-02-15 22:27:07.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-02-15 22:27:08.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-02-15 22:27:08.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:07.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59063 2023-02-15 22:27:10.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58996 2023-02-15 22:27:09.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-15 22:27:07.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.846127 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18860 2023-02-15 22:27:56.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-15 22:27:56.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:27:56.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:27:56.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-15 22:27:56.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-15 22:27:56.000000 mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 22:27:56.846127 mypy-boto3-frauddetector-1.26.72/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-02-15 22:27:07.000000 mypy-boto3-frauddetector-1.26.72/setup.py
```

### Comparing `mypy-boto3-frauddetector-1.26.65/LICENSE` & `mypy-boto3-frauddetector-1.26.72/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.26.65/PKG-INFO` & `mypy-boto3-frauddetector-1.26.72/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-frauddetector
-Version: 1.26.65
-Summary: Type annotations for boto3.FraudDetector 1.26.65 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.72
+Summary: Type annotations for boto3.FraudDetector 1.26.72 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-frauddetector?color=blue)](https://pypistats.org/packages/mypy-boto3-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FraudDetector 1.26.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[boto3.FraudDetector 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -282,14 +282,15 @@
 from mypy_boto3_frauddetector.literals import (
     AsyncJobStatusType,
     DataSourceType,
     DataTypeType,
     DetectorVersionStatusType,
     EventIngestionType,
     LanguageType,
+    ListUpdateModeType,
     ModelEndpointStatusType,
     ModelInputDataFormatType,
     ModelOutputDataFormatType,
     ModelSourceType,
     ModelTypeEnumType,
     ModelVersionStatusType,
     RuleExecutionModeType,
@@ -315,14 +316,15 @@
 
 ```python
 from mypy_boto3_frauddetector.type_defs import (
     ATIMetricDataPointTypeDef,
     ATIModelPerformanceTypeDef,
     AggregatedLogOddsMetricTypeDef,
     AggregatedVariablesImpactExplanationTypeDef,
+    AllowDenyListTypeDef,
     BatchCreateVariableErrorTypeDef,
     TagTypeDef,
     VariableEntryTypeDef,
     ResponseMetadataTypeDef,
     BatchGetVariableErrorTypeDef,
     BatchGetVariableRequestRequestTypeDef,
     VariableTypeDef,
@@ -341,14 +343,15 @@
     DeleteDetectorVersionRequestRequestTypeDef,
     DeleteEntityTypeRequestRequestTypeDef,
     DeleteEventRequestRequestTypeDef,
     DeleteEventTypeRequestRequestTypeDef,
     DeleteEventsByEventTypeRequestRequestTypeDef,
     DeleteExternalModelRequestRequestTypeDef,
     DeleteLabelRequestRequestTypeDef,
+    DeleteListRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
     DeleteModelVersionRequestRequestTypeDef,
     DeleteOutcomeRequestRequestTypeDef,
     DeleteVariableRequestRequestTypeDef,
     DescribeDetectorRequestRequestTypeDef,
     DetectorVersionSummaryTypeDef,
     DescribeModelVersionsRequestRequestTypeDef,
@@ -375,14 +378,16 @@
     RuleResultTypeDef,
     GetEventRequestRequestTypeDef,
     GetEventTypesRequestRequestTypeDef,
     GetExternalModelsRequestRequestTypeDef,
     KMSKeyTypeDef,
     GetLabelsRequestRequestTypeDef,
     LabelTypeDef,
+    GetListElementsRequestRequestTypeDef,
+    GetListsMetadataRequestRequestTypeDef,
     GetModelVersionRequestRequestTypeDef,
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetOutcomesRequestRequestTypeDef,
     OutcomeTypeDef,
     GetRulesRequestRequestTypeDef,
     RuleDetailTypeDef,
@@ -398,21 +403,23 @@
     VariableImpactExplanationTypeDef,
     PutKMSEncryptionKeyRequestRequestTypeDef,
     TFIMetricDataPointTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDetectorVersionMetadataRequestRequestTypeDef,
     UpdateDetectorVersionStatusRequestRequestTypeDef,
     UpdateEventLabelRequestRequestTypeDef,
+    UpdateListRequestRequestTypeDef,
     UpdateModelRequestRequestTypeDef,
     UpdateModelVersionStatusRequestRequestTypeDef,
     UpdateVariableRequestRequestTypeDef,
     ATITrainingMetricsValueTypeDef,
     AggregatedVariablesImportanceMetricsTypeDef,
     CreateBatchImportJobRequestRequestTypeDef,
     CreateBatchPredictionJobRequestRequestTypeDef,
+    CreateListRequestRequestTypeDef,
     CreateModelRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateVariableRequestRequestTypeDef,
     PutDetectorRequestRequestTypeDef,
     PutEntityTypeRequestRequestTypeDef,
     PutEventTypeRequestRequestTypeDef,
     PutLabelRequestRequestTypeDef,
@@ -420,14 +427,16 @@
     TagResourceRequestRequestTypeDef,
     BatchCreateVariableRequestRequestTypeDef,
     BatchCreateVariableResultTypeDef,
     CreateDetectorVersionResultTypeDef,
     CreateModelVersionResultTypeDef,
     DeleteEventsByEventTypeResultTypeDef,
     GetDeleteEventsByEventTypeStatusResultTypeDef,
+    GetListElementsResultTypeDef,
+    GetListsMetadataResultTypeDef,
     ListTagsForResourceResultTypeDef,
     UpdateModelVersionResultTypeDef,
     BatchGetVariableResultTypeDef,
     GetVariablesResultTypeDef,
     GetBatchImportJobsResultTypeDef,
     GetBatchPredictionJobsResultTypeDef,
     ModelScoresTypeDef,
```

### Comparing `mypy-boto3-frauddetector-1.26.65/README.md` & `mypy-boto3-frauddetector-1.26.72/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-frauddetector?color=blue)](https://pypistats.org/packages/mypy-boto3-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FraudDetector 1.26.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[boto3.FraudDetector 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -250,14 +250,15 @@
 from mypy_boto3_frauddetector.literals import (
     AsyncJobStatusType,
     DataSourceType,
     DataTypeType,
     DetectorVersionStatusType,
     EventIngestionType,
     LanguageType,
+    ListUpdateModeType,
     ModelEndpointStatusType,
     ModelInputDataFormatType,
     ModelOutputDataFormatType,
     ModelSourceType,
     ModelTypeEnumType,
     ModelVersionStatusType,
     RuleExecutionModeType,
@@ -283,14 +284,15 @@
 
 ```python
 from mypy_boto3_frauddetector.type_defs import (
     ATIMetricDataPointTypeDef,
     ATIModelPerformanceTypeDef,
     AggregatedLogOddsMetricTypeDef,
     AggregatedVariablesImpactExplanationTypeDef,
+    AllowDenyListTypeDef,
     BatchCreateVariableErrorTypeDef,
     TagTypeDef,
     VariableEntryTypeDef,
     ResponseMetadataTypeDef,
     BatchGetVariableErrorTypeDef,
     BatchGetVariableRequestRequestTypeDef,
     VariableTypeDef,
@@ -309,14 +311,15 @@
     DeleteDetectorVersionRequestRequestTypeDef,
     DeleteEntityTypeRequestRequestTypeDef,
     DeleteEventRequestRequestTypeDef,
     DeleteEventTypeRequestRequestTypeDef,
     DeleteEventsByEventTypeRequestRequestTypeDef,
     DeleteExternalModelRequestRequestTypeDef,
     DeleteLabelRequestRequestTypeDef,
+    DeleteListRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
     DeleteModelVersionRequestRequestTypeDef,
     DeleteOutcomeRequestRequestTypeDef,
     DeleteVariableRequestRequestTypeDef,
     DescribeDetectorRequestRequestTypeDef,
     DetectorVersionSummaryTypeDef,
     DescribeModelVersionsRequestRequestTypeDef,
@@ -343,14 +346,16 @@
     RuleResultTypeDef,
     GetEventRequestRequestTypeDef,
     GetEventTypesRequestRequestTypeDef,
     GetExternalModelsRequestRequestTypeDef,
     KMSKeyTypeDef,
     GetLabelsRequestRequestTypeDef,
     LabelTypeDef,
+    GetListElementsRequestRequestTypeDef,
+    GetListsMetadataRequestRequestTypeDef,
     GetModelVersionRequestRequestTypeDef,
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetOutcomesRequestRequestTypeDef,
     OutcomeTypeDef,
     GetRulesRequestRequestTypeDef,
     RuleDetailTypeDef,
@@ -366,21 +371,23 @@
     VariableImpactExplanationTypeDef,
     PutKMSEncryptionKeyRequestRequestTypeDef,
     TFIMetricDataPointTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDetectorVersionMetadataRequestRequestTypeDef,
     UpdateDetectorVersionStatusRequestRequestTypeDef,
     UpdateEventLabelRequestRequestTypeDef,
+    UpdateListRequestRequestTypeDef,
     UpdateModelRequestRequestTypeDef,
     UpdateModelVersionStatusRequestRequestTypeDef,
     UpdateVariableRequestRequestTypeDef,
     ATITrainingMetricsValueTypeDef,
     AggregatedVariablesImportanceMetricsTypeDef,
     CreateBatchImportJobRequestRequestTypeDef,
     CreateBatchPredictionJobRequestRequestTypeDef,
+    CreateListRequestRequestTypeDef,
     CreateModelRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateVariableRequestRequestTypeDef,
     PutDetectorRequestRequestTypeDef,
     PutEntityTypeRequestRequestTypeDef,
     PutEventTypeRequestRequestTypeDef,
     PutLabelRequestRequestTypeDef,
@@ -388,14 +395,16 @@
     TagResourceRequestRequestTypeDef,
     BatchCreateVariableRequestRequestTypeDef,
     BatchCreateVariableResultTypeDef,
     CreateDetectorVersionResultTypeDef,
     CreateModelVersionResultTypeDef,
     DeleteEventsByEventTypeResultTypeDef,
     GetDeleteEventsByEventTypeStatusResultTypeDef,
+    GetListElementsResultTypeDef,
+    GetListsMetadataResultTypeDef,
     ListTagsForResourceResultTypeDef,
     UpdateModelVersionResultTypeDef,
     BatchGetVariableResultTypeDef,
     GetVariablesResultTypeDef,
     GetBatchImportJobsResultTypeDef,
     GetBatchPredictionJobsResultTypeDef,
     ModelScoresTypeDef,
```

### Comparing `mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/__main__.py` & `mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FraudDetector 1.26.65\nVersion:         1.26.65\nBuilder"
+        "Type annotations for boto3.FraudDetector 1.26.72\nVersion:         1.26.72\nBuilder"
         " version: 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.65")
+    print("1.26.72")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/client.py` & `mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DataSourceType,
     DataTypeType,
     DetectorVersionStatusType,
     EventIngestionType,
+    ListUpdateModeType,
     ModelEndpointStatusType,
     ModelTypeEnumType,
     ModelVersionStatusType,
     RuleExecutionModeType,
     TrainingDataSourceEnumType,
 )
 from .type_defs import (
@@ -50,14 +51,16 @@
     GetEventPredictionMetadataResultTypeDef,
     GetEventPredictionResultTypeDef,
     GetEventResultTypeDef,
     GetEventTypesResultTypeDef,
     GetExternalModelsResultTypeDef,
     GetKMSEncryptionKeyResultTypeDef,
     GetLabelsResultTypeDef,
+    GetListElementsResultTypeDef,
+    GetListsMetadataResultTypeDef,
     GetModelsResultTypeDef,
     GetModelVersionResultTypeDef,
     GetOutcomesResultTypeDef,
     GetRulesResultTypeDef,
     GetVariablesResultTypeDef,
     IngestedEventsDetailTypeDef,
     ListEventPredictionsResultTypeDef,
@@ -220,14 +223,30 @@
         """
         Creates a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_detector_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_detector_version)
         """
 
+    def create_list(
+        self,
+        *,
+        name: str,
+        elements: Sequence[str] = ...,
+        variableType: str = ...,
+        description: str = ...,
+        tags: Sequence[TagTypeDef] = ...
+    ) -> Dict[str, Any]:
+        """
+        Creates a list.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_list)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_list)
+        """
+
     def create_model(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         eventTypeName: str,
         description: str = ...,
@@ -374,14 +393,22 @@
         """
         Deletes a label.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_label)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_label)
         """
 
+    def delete_list(self, *, name: str) -> Dict[str, Any]:
+        """
+        Deletes the list, provided it is not used in a rule.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_list)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_list)
+        """
+
     def delete_model(self, *, modelId: str, modelType: ModelTypeEnumType) -> Dict[str, Any]:
         """
         Deletes a model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_model)
         """
@@ -602,14 +629,35 @@
         """
         Gets all labels or a specific label if name is provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_labels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_labels)
         """
 
+    def get_list_elements(
+        self, *, name: str, nextToken: str = ..., maxResults: int = ...
+    ) -> GetListElementsResultTypeDef:
+        """
+        Gets all the elements in the specified list.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_list_elements)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_list_elements)
+        """
+
+    def get_lists_metadata(
+        self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
+    ) -> GetListsMetadataResultTypeDef:
+        """
+        Gets the metadata of either all the lists under the account or the specified
+        list.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_lists_metadata)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_lists_metadata)
+        """
+
     def get_model_version(
         self, *, modelId: str, modelType: ModelTypeEnumType, modelVersionNumber: str
     ) -> GetModelVersionResultTypeDef:
         """
         Gets the details of the specified model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_model_version)
@@ -864,14 +912,30 @@
         """
         Updates the specified event with a new label.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_event_label)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_event_label)
         """
 
+    def update_list(
+        self,
+        *,
+        name: str,
+        elements: Sequence[str] = ...,
+        description: str = ...,
+        updateMode: ListUpdateModeType = ...,
+        variableType: str = ...
+    ) -> Dict[str, Any]:
+        """
+        Updates a list.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_list)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_list)
+        """
+
     def update_model(
         self, *, modelId: str, modelType: ModelTypeEnumType, description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates model description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_model)
```

### Comparing `mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/client.pyi` & `mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DataSourceType,
     DataTypeType,
     DetectorVersionStatusType,
     EventIngestionType,
+    ListUpdateModeType,
     ModelEndpointStatusType,
     ModelTypeEnumType,
     ModelVersionStatusType,
     RuleExecutionModeType,
     TrainingDataSourceEnumType,
 )
 from .type_defs import (
@@ -50,14 +51,16 @@
     GetEventPredictionMetadataResultTypeDef,
     GetEventPredictionResultTypeDef,
     GetEventResultTypeDef,
     GetEventTypesResultTypeDef,
     GetExternalModelsResultTypeDef,
     GetKMSEncryptionKeyResultTypeDef,
     GetLabelsResultTypeDef,
+    GetListElementsResultTypeDef,
+    GetListsMetadataResultTypeDef,
     GetModelsResultTypeDef,
     GetModelVersionResultTypeDef,
     GetOutcomesResultTypeDef,
     GetRulesResultTypeDef,
     GetVariablesResultTypeDef,
     IngestedEventsDetailTypeDef,
     ListEventPredictionsResultTypeDef,
@@ -206,14 +209,29 @@
     ) -> CreateDetectorVersionResultTypeDef:
         """
         Creates a detector version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_detector_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_detector_version)
         """
+    def create_list(
+        self,
+        *,
+        name: str,
+        elements: Sequence[str] = ...,
+        variableType: str = ...,
+        description: str = ...,
+        tags: Sequence[TagTypeDef] = ...
+    ) -> Dict[str, Any]:
+        """
+        Creates a list.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.create_list)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#create_list)
+        """
     def create_model(
         self,
         *,
         modelId: str,
         modelType: ModelTypeEnumType,
         eventTypeName: str,
         description: str = ...,
@@ -346,14 +364,21 @@
     def delete_label(self, *, name: str) -> Dict[str, Any]:
         """
         Deletes a label.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_label)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_label)
         """
+    def delete_list(self, *, name: str) -> Dict[str, Any]:
+        """
+        Deletes the list, provided it is not used in a rule.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_list)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_list)
+        """
     def delete_model(self, *, modelId: str, modelType: ModelTypeEnumType) -> Dict[str, Any]:
         """
         Deletes a model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.delete_model)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#delete_model)
         """
@@ -553,14 +578,33 @@
     ) -> GetLabelsResultTypeDef:
         """
         Gets all labels or a specific label if name is provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_labels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_labels)
         """
+    def get_list_elements(
+        self, *, name: str, nextToken: str = ..., maxResults: int = ...
+    ) -> GetListElementsResultTypeDef:
+        """
+        Gets all the elements in the specified list.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_list_elements)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_list_elements)
+        """
+    def get_lists_metadata(
+        self, *, name: str = ..., nextToken: str = ..., maxResults: int = ...
+    ) -> GetListsMetadataResultTypeDef:
+        """
+        Gets the metadata of either all the lists under the account or the specified
+        list.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_lists_metadata)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#get_lists_metadata)
+        """
     def get_model_version(
         self, *, modelId: str, modelType: ModelTypeEnumType, modelVersionNumber: str
     ) -> GetModelVersionResultTypeDef:
         """
         Gets the details of the specified model version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.get_model_version)
@@ -794,14 +838,29 @@
     ) -> Dict[str, Any]:
         """
         Updates the specified event with a new label.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_event_label)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_event_label)
         """
+    def update_list(
+        self,
+        *,
+        name: str,
+        elements: Sequence[str] = ...,
+        description: str = ...,
+        updateMode: ListUpdateModeType = ...,
+        variableType: str = ...
+    ) -> Dict[str, Any]:
+        """
+        Updates a list.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_list)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/client/#update_list)
+        """
     def update_model(
         self, *, modelId: str, modelType: ModelTypeEnumType, description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates model description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector.Client.update_model)
```

### Comparing `mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/literals.py` & `mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 __all__ = (
     "AsyncJobStatusType",
     "DataSourceType",
     "DataTypeType",
     "DetectorVersionStatusType",
     "EventIngestionType",
     "LanguageType",
+    "ListUpdateModeType",
     "ModelEndpointStatusType",
     "ModelInputDataFormatType",
     "ModelOutputDataFormatType",
     "ModelSourceType",
     "ModelTypeEnumType",
     "ModelVersionStatusType",
     "RuleExecutionModeType",
@@ -51,14 +52,15 @@
     "IN_PROGRESS_INITIALIZING",
 ]
 DataSourceType = Literal["EVENT", "EXTERNAL_MODEL_SCORE", "MODEL_SCORE"]
 DataTypeType = Literal["BOOLEAN", "FLOAT", "INTEGER", "STRING"]
 DetectorVersionStatusType = Literal["ACTIVE", "DRAFT", "INACTIVE"]
 EventIngestionType = Literal["DISABLED", "ENABLED"]
 LanguageType = Literal["DETECTORPL"]
+ListUpdateModeType = Literal["APPEND", "REMOVE", "REPLACE"]
 ModelEndpointStatusType = Literal["ASSOCIATED", "DISSOCIATED"]
 ModelInputDataFormatType = Literal["APPLICATION_JSON", "TEXT_CSV"]
 ModelOutputDataFormatType = Literal["APPLICATION_JSONLINES", "TEXT_CSV"]
 ModelSourceType = Literal["SAGEMAKER"]
 ModelTypeEnumType = Literal[
     "ACCOUNT_TAKEOVER_INSIGHTS", "ONLINE_FRAUD_INSIGHTS", "TRANSACTION_FRAUD_INSIGHTS"
 ]
```

### Comparing `mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/literals.pyi` & `mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 __all__ = (
     "AsyncJobStatusType",
     "DataSourceType",
     "DataTypeType",
     "DetectorVersionStatusType",
     "EventIngestionType",
     "LanguageType",
+    "ListUpdateModeType",
     "ModelEndpointStatusType",
     "ModelInputDataFormatType",
     "ModelOutputDataFormatType",
     "ModelSourceType",
     "ModelTypeEnumType",
     "ModelVersionStatusType",
     "RuleExecutionModeType",
@@ -49,14 +50,15 @@
     "IN_PROGRESS_INITIALIZING",
 ]
 DataSourceType = Literal["EVENT", "EXTERNAL_MODEL_SCORE", "MODEL_SCORE"]
 DataTypeType = Literal["BOOLEAN", "FLOAT", "INTEGER", "STRING"]
 DetectorVersionStatusType = Literal["ACTIVE", "DRAFT", "INACTIVE"]
 EventIngestionType = Literal["DISABLED", "ENABLED"]
 LanguageType = Literal["DETECTORPL"]
+ListUpdateModeType = Literal["APPEND", "REMOVE", "REPLACE"]
 ModelEndpointStatusType = Literal["ASSOCIATED", "DISSOCIATED"]
 ModelInputDataFormatType = Literal["APPLICATION_JSON", "TEXT_CSV"]
 ModelOutputDataFormatType = Literal["APPLICATION_JSONLINES", "TEXT_CSV"]
 ModelSourceType = Literal["SAGEMAKER"]
 ModelTypeEnumType = Literal[
     "ACCOUNT_TAKEOVER_INSIGHTS", "ONLINE_FRAUD_INSIGHTS", "TRANSACTION_FRAUD_INSIGHTS"
 ]
```

### Comparing `mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/type_defs.py` & `mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from .literals import (
     AsyncJobStatusType,
     DataSourceType,
     DataTypeType,
     DetectorVersionStatusType,
     EventIngestionType,
+    ListUpdateModeType,
     ModelEndpointStatusType,
     ModelInputDataFormatType,
     ModelOutputDataFormatType,
     ModelTypeEnumType,
     ModelVersionStatusType,
     RuleExecutionModeType,
     TrainingDataSourceEnumType,
@@ -37,20 +38,20 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ATIMetricDataPointTypeDef",
     "ATIModelPerformanceTypeDef",
     "AggregatedLogOddsMetricTypeDef",
     "AggregatedVariablesImpactExplanationTypeDef",
+    "AllowDenyListTypeDef",
     "BatchCreateVariableErrorTypeDef",
     "TagTypeDef",
     "VariableEntryTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetVariableErrorTypeDef",
     "BatchGetVariableRequestRequestTypeDef",
     "VariableTypeDef",
@@ -69,14 +70,15 @@
     "DeleteDetectorVersionRequestRequestTypeDef",
     "DeleteEntityTypeRequestRequestTypeDef",
     "DeleteEventRequestRequestTypeDef",
     "DeleteEventTypeRequestRequestTypeDef",
     "DeleteEventsByEventTypeRequestRequestTypeDef",
     "DeleteExternalModelRequestRequestTypeDef",
     "DeleteLabelRequestRequestTypeDef",
+    "DeleteListRequestRequestTypeDef",
     "DeleteModelRequestRequestTypeDef",
     "DeleteModelVersionRequestRequestTypeDef",
     "DeleteOutcomeRequestRequestTypeDef",
     "DeleteVariableRequestRequestTypeDef",
     "DescribeDetectorRequestRequestTypeDef",
     "DetectorVersionSummaryTypeDef",
     "DescribeModelVersionsRequestRequestTypeDef",
@@ -103,14 +105,16 @@
     "RuleResultTypeDef",
     "GetEventRequestRequestTypeDef",
     "GetEventTypesRequestRequestTypeDef",
     "GetExternalModelsRequestRequestTypeDef",
     "KMSKeyTypeDef",
     "GetLabelsRequestRequestTypeDef",
     "LabelTypeDef",
+    "GetListElementsRequestRequestTypeDef",
+    "GetListsMetadataRequestRequestTypeDef",
     "GetModelVersionRequestRequestTypeDef",
     "GetModelsRequestRequestTypeDef",
     "ModelTypeDef",
     "GetOutcomesRequestRequestTypeDef",
     "OutcomeTypeDef",
     "GetRulesRequestRequestTypeDef",
     "RuleDetailTypeDef",
@@ -126,21 +130,23 @@
     "VariableImpactExplanationTypeDef",
     "PutKMSEncryptionKeyRequestRequestTypeDef",
     "TFIMetricDataPointTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDetectorVersionMetadataRequestRequestTypeDef",
     "UpdateDetectorVersionStatusRequestRequestTypeDef",
     "UpdateEventLabelRequestRequestTypeDef",
+    "UpdateListRequestRequestTypeDef",
     "UpdateModelRequestRequestTypeDef",
     "UpdateModelVersionStatusRequestRequestTypeDef",
     "UpdateVariableRequestRequestTypeDef",
     "ATITrainingMetricsValueTypeDef",
     "AggregatedVariablesImportanceMetricsTypeDef",
     "CreateBatchImportJobRequestRequestTypeDef",
     "CreateBatchPredictionJobRequestRequestTypeDef",
+    "CreateListRequestRequestTypeDef",
     "CreateModelRequestRequestTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "CreateVariableRequestRequestTypeDef",
     "PutDetectorRequestRequestTypeDef",
     "PutEntityTypeRequestRequestTypeDef",
     "PutEventTypeRequestRequestTypeDef",
     "PutLabelRequestRequestTypeDef",
@@ -148,14 +154,16 @@
     "TagResourceRequestRequestTypeDef",
     "BatchCreateVariableRequestRequestTypeDef",
     "BatchCreateVariableResultTypeDef",
     "CreateDetectorVersionResultTypeDef",
     "CreateModelVersionResultTypeDef",
     "DeleteEventsByEventTypeResultTypeDef",
     "GetDeleteEventsByEventTypeStatusResultTypeDef",
+    "GetListElementsResultTypeDef",
+    "GetListsMetadataResultTypeDef",
     "ListTagsForResourceResultTypeDef",
     "UpdateModelVersionResultTypeDef",
     "BatchGetVariableResultTypeDef",
     "GetVariablesResultTypeDef",
     "GetBatchImportJobsResultTypeDef",
     "GetBatchPredictionJobsResultTypeDef",
     "ModelScoresTypeDef",
@@ -244,14 +252,35 @@
         "eventVariableNames": List[str],
         "relativeImpact": str,
         "logOddsImpact": float,
     },
     total=False,
 )
 
+_RequiredAllowDenyListTypeDef = TypedDict(
+    "_RequiredAllowDenyListTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalAllowDenyListTypeDef = TypedDict(
+    "_OptionalAllowDenyListTypeDef",
+    {
+        "description": str,
+        "variableType": str,
+        "createdTime": str,
+        "updatedTime": str,
+        "arn": str,
+    },
+    total=False,
+)
+
+class AllowDenyListTypeDef(_RequiredAllowDenyListTypeDef, _OptionalAllowDenyListTypeDef):
+    pass
+
 BatchCreateVariableErrorTypeDef = TypedDict(
     "BatchCreateVariableErrorTypeDef",
     {
         "name": str,
         "code": int,
         "message": str,
     },
@@ -391,19 +420,17 @@
     "_OptionalModelVersionTypeDef",
     {
         "arn": str,
     },
     total=False,
 )
 
-
 class ModelVersionTypeDef(_RequiredModelVersionTypeDef, _OptionalModelVersionTypeDef):
     pass
 
-
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "detectorId": str,
         "ruleId": str,
         "ruleVersion": str,
     },
@@ -486,21 +513,19 @@
     "_OptionalDeleteEventRequestRequestTypeDef",
     {
         "deleteAuditHistory": bool,
     },
     total=False,
 )
 
-
 class DeleteEventRequestRequestTypeDef(
     _RequiredDeleteEventRequestRequestTypeDef, _OptionalDeleteEventRequestRequestTypeDef
 ):
     pass
 
-
 DeleteEventTypeRequestRequestTypeDef = TypedDict(
     "DeleteEventTypeRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -521,14 +546,21 @@
 DeleteLabelRequestRequestTypeDef = TypedDict(
     "DeleteLabelRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
+DeleteListRequestRequestTypeDef = TypedDict(
+    "DeleteListRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+
 DeleteModelRequestRequestTypeDef = TypedDict(
     "DeleteModelRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
     },
 )
@@ -567,21 +599,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class DescribeDetectorRequestRequestTypeDef(
     _RequiredDescribeDetectorRequestRequestTypeDef, _OptionalDescribeDetectorRequestRequestTypeDef
 ):
     pass
 
-
 DetectorVersionSummaryTypeDef = TypedDict(
     "DetectorVersionSummaryTypeDef",
     {
         "detectorVersionId": str,
         "status": DetectorVersionStatusType,
         "description": str,
         "lastUpdatedTime": str,
@@ -716,21 +746,19 @@
         "format": ModelInputDataFormatType,
         "jsonInputTemplate": str,
         "csvInputTemplate": str,
     },
     total=False,
 )
 
-
 class ModelInputConfigurationTypeDef(
     _RequiredModelInputConfigurationTypeDef, _OptionalModelInputConfigurationTypeDef
 ):
     pass
 
-
 _RequiredModelOutputConfigurationTypeDef = TypedDict(
     "_RequiredModelOutputConfigurationTypeDef",
     {
         "format": ModelOutputDataFormatType,
     },
 )
 _OptionalModelOutputConfigurationTypeDef = TypedDict(
@@ -738,21 +766,19 @@
     {
         "jsonKeyToVariableMap": Dict[str, str],
         "csvIndexToVariableMap": Dict[str, str],
     },
     total=False,
 )
 
-
 class ModelOutputConfigurationTypeDef(
     _RequiredModelOutputConfigurationTypeDef, _OptionalModelOutputConfigurationTypeDef
 ):
     pass
 
-
 FilterConditionTypeDef = TypedDict(
     "FilterConditionTypeDef",
     {
         "value": str,
     },
     total=False,
 )
@@ -895,14 +921,44 @@
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
     },
     total=False,
 )
 
+_RequiredGetListElementsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetListElementsRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalGetListElementsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetListElementsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class GetListElementsRequestRequestTypeDef(
+    _RequiredGetListElementsRequestRequestTypeDef, _OptionalGetListElementsRequestRequestTypeDef
+):
+    pass
+
+GetListsMetadataRequestRequestTypeDef = TypedDict(
+    "GetListsMetadataRequestRequestTypeDef",
+    {
+        "name": str,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
 GetModelVersionRequestRequestTypeDef = TypedDict(
     "GetModelVersionRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
     },
@@ -968,21 +1024,19 @@
         "ruleVersion": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetRulesRequestRequestTypeDef(
     _RequiredGetRulesRequestRequestTypeDef, _OptionalGetRulesRequestRequestTypeDef
 ):
     pass
 
-
 RuleDetailTypeDef = TypedDict(
     "RuleDetailTypeDef",
     {
         "ruleId": str,
         "description": str,
         "detectorId": str,
         "ruleVersion": str,
@@ -1042,22 +1096,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
 LogOddsMetricTypeDef = TypedDict(
     "LogOddsMetricTypeDef",
     {
         "variableName": str,
         "variableType": str,
         "variableImportance": float,
     },
@@ -1153,14 +1205,36 @@
         "eventId": str,
         "eventTypeName": str,
         "assignedLabel": str,
         "labelTimestamp": str,
     },
 )
 
+_RequiredUpdateListRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateListRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalUpdateListRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateListRequestRequestTypeDef",
+    {
+        "elements": Sequence[str],
+        "description": str,
+        "updateMode": ListUpdateModeType,
+        "variableType": str,
+    },
+    total=False,
+)
+
+class UpdateListRequestRequestTypeDef(
+    _RequiredUpdateListRequestRequestTypeDef, _OptionalUpdateListRequestRequestTypeDef
+):
+    pass
+
 _RequiredUpdateModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
     },
 )
@@ -1168,21 +1242,19 @@
     "_OptionalUpdateModelRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class UpdateModelRequestRequestTypeDef(
     _RequiredUpdateModelRequestRequestTypeDef, _OptionalUpdateModelRequestRequestTypeDef
 ):
     pass
 
-
 UpdateModelVersionStatusRequestRequestTypeDef = TypedDict(
     "UpdateModelVersionStatusRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
         "status": ModelVersionStatusType,
@@ -1201,21 +1273,19 @@
         "defaultValue": str,
         "description": str,
         "variableType": str,
     },
     total=False,
 )
 
-
 class UpdateVariableRequestRequestTypeDef(
     _RequiredUpdateVariableRequestRequestTypeDef, _OptionalUpdateVariableRequestRequestTypeDef
 ):
     pass
 
-
 ATITrainingMetricsValueTypeDef = TypedDict(
     "ATITrainingMetricsValueTypeDef",
     {
         "metricDataPoints": List[ATIMetricDataPointTypeDef],
         "modelPerformance": ATIModelPerformanceTypeDef,
     },
     total=False,
@@ -1243,22 +1313,20 @@
     "_OptionalCreateBatchImportJobRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateBatchImportJobRequestRequestTypeDef(
     _RequiredCreateBatchImportJobRequestRequestTypeDef,
     _OptionalCreateBatchImportJobRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateBatchPredictionJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchPredictionJobRequestRequestTypeDef",
     {
         "jobId": str,
         "inputPath": str,
         "outputPath": str,
         "eventTypeName": str,
@@ -1271,21 +1339,41 @@
     {
         "detectorVersion": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateBatchPredictionJobRequestRequestTypeDef(
     _RequiredCreateBatchPredictionJobRequestRequestTypeDef,
     _OptionalCreateBatchPredictionJobRequestRequestTypeDef,
 ):
     pass
 
+_RequiredCreateListRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateListRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateListRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateListRequestRequestTypeDef",
+    {
+        "elements": Sequence[str],
+        "variableType": str,
+        "description": str,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateListRequestRequestTypeDef(
+    _RequiredCreateListRequestRequestTypeDef, _OptionalCreateListRequestRequestTypeDef
+):
+    pass
 
 _RequiredCreateModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "eventTypeName": str,
@@ -1296,21 +1384,19 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateModelRequestRequestTypeDef(
     _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleRequestRequestTypeDef",
     {
         "ruleId": str,
         "detectorId": str,
         "expression": str,
         "language": Literal["DETECTORPL"],
@@ -1322,21 +1408,19 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateRuleRequestRequestTypeDef(
     _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateVariableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVariableRequestRequestTypeDef",
     {
         "name": str,
         "dataType": DataTypeType,
         "dataSource": DataSourceType,
         "defaultValue": str,
@@ -1348,21 +1432,19 @@
         "description": str,
         "variableType": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateVariableRequestRequestTypeDef(
     _RequiredCreateVariableRequestRequestTypeDef, _OptionalCreateVariableRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredPutDetectorRequestRequestTypeDef",
     {
         "detectorId": str,
         "eventTypeName": str,
     },
 )
@@ -1371,21 +1453,19 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutDetectorRequestRequestTypeDef(
     _RequiredPutDetectorRequestRequestTypeDef, _OptionalPutDetectorRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutEntityTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutEntityTypeRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutEntityTypeRequestRequestTypeDef = TypedDict(
@@ -1393,21 +1473,19 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutEntityTypeRequestRequestTypeDef(
     _RequiredPutEntityTypeRequestRequestTypeDef, _OptionalPutEntityTypeRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutEventTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutEventTypeRequestRequestTypeDef",
     {
         "name": str,
         "eventVariables": Sequence[str],
         "entityTypes": Sequence[str],
     },
@@ -1419,21 +1497,19 @@
         "labels": Sequence[str],
         "eventIngestion": EventIngestionType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutEventTypeRequestRequestTypeDef(
     _RequiredPutEventTypeRequestRequestTypeDef, _OptionalPutEventTypeRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutLabelRequestRequestTypeDef = TypedDict(
     "_RequiredPutLabelRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutLabelRequestRequestTypeDef = TypedDict(
@@ -1441,21 +1517,19 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutLabelRequestRequestTypeDef(
     _RequiredPutLabelRequestRequestTypeDef, _OptionalPutLabelRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutOutcomeRequestRequestTypeDef = TypedDict(
     "_RequiredPutOutcomeRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutOutcomeRequestRequestTypeDef = TypedDict(
@@ -1463,21 +1537,19 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutOutcomeRequestRequestTypeDef(
     _RequiredPutOutcomeRequestRequestTypeDef, _OptionalPutOutcomeRequestRequestTypeDef
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1492,22 +1564,20 @@
     "_OptionalBatchCreateVariableRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class BatchCreateVariableRequestRequestTypeDef(
     _RequiredBatchCreateVariableRequestRequestTypeDef,
     _OptionalBatchCreateVariableRequestRequestTypeDef,
 ):
     pass
 
-
 BatchCreateVariableResultTypeDef = TypedDict(
     "BatchCreateVariableResultTypeDef",
     {
         "errors": List[BatchCreateVariableErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1547,14 +1617,32 @@
     {
         "eventTypeName": str,
         "eventsDeletionStatus": AsyncJobStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetListElementsResultTypeDef = TypedDict(
+    "GetListElementsResultTypeDef",
+    {
+        "elements": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetListsMetadataResultTypeDef = TypedDict(
+    "GetListsMetadataResultTypeDef",
+    {
+        "lists": List[AllowDenyListTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
         "tags": List[TagTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1631,22 +1719,20 @@
         "modelVersions": Sequence[ModelVersionTypeDef],
         "ruleExecutionMode": RuleExecutionModeType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDetectorVersionRequestRequestTypeDef(
     _RequiredCreateDetectorVersionRequestRequestTypeDef,
     _OptionalCreateDetectorVersionRequestRequestTypeDef,
 ):
     pass
 
-
 CreateRuleResultTypeDef = TypedDict(
     "CreateRuleResultTypeDef",
     {
         "rule": RuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1691,22 +1777,20 @@
         "description": str,
         "modelVersions": Sequence[ModelVersionTypeDef],
         "ruleExecutionMode": RuleExecutionModeType,
     },
     total=False,
 )
 
-
 class UpdateDetectorVersionRequestRequestTypeDef(
     _RequiredUpdateDetectorVersionRequestRequestTypeDef,
     _OptionalUpdateDetectorVersionRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateRuleMetadataRequestRequestTypeDef = TypedDict(
     "UpdateRuleMetadataRequestRequestTypeDef",
     {
         "rule": RuleTypeDef,
         "description": str,
     },
 )
@@ -1725,21 +1809,19 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class UpdateRuleVersionRequestRequestTypeDef(
     _RequiredUpdateRuleVersionRequestRequestTypeDef, _OptionalUpdateRuleVersionRequestRequestTypeDef
 ):
     pass
 
-
 UpdateRuleVersionResultTypeDef = TypedDict(
     "UpdateRuleVersionResultTypeDef",
     {
         "rule": RuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1802,21 +1884,19 @@
     {
         "assignedLabel": str,
         "labelTimestamp": str,
     },
     total=False,
 )
 
-
 class SendEventRequestRequestTypeDef(
     _RequiredSendEventRequestRequestTypeDef, _OptionalSendEventRequestRequestTypeDef
 ):
     pass
 
-
 GetEntityTypesResultTypeDef = TypedDict(
     "GetEntityTypesResultTypeDef",
     {
         "entityTypes": List[EntityTypeTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1888,21 +1968,19 @@
     "_OptionalPutExternalModelRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutExternalModelRequestRequestTypeDef(
     _RequiredPutExternalModelRequestRequestTypeDef, _OptionalPutExternalModelRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetEventPredictionRequestRequestTypeDef = TypedDict(
     "_RequiredGetEventPredictionRequestRequestTypeDef",
     {
         "detectorId": str,
         "eventId": str,
         "eventTypeName": str,
         "entities": Sequence[EntityTypeDef],
@@ -1915,22 +1993,20 @@
     {
         "detectorVersionId": str,
         "externalModelEndpointDataBlobs": Mapping[str, ModelEndpointDataBlobTypeDef],
     },
     total=False,
 )
 
-
 class GetEventPredictionRequestRequestTypeDef(
     _RequiredGetEventPredictionRequestRequestTypeDef,
     _OptionalGetEventPredictionRequestRequestTypeDef,
 ):
     pass
 
-
 GetKMSEncryptionKeyResultTypeDef = TypedDict(
     "GetKMSEncryptionKeyResultTypeDef",
     {
         "kmsKey": KMSKeyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1988,21 +2064,19 @@
     "_OptionalTrainingDataSchemaTypeDef",
     {
         "labelSchema": LabelSchemaTypeDef,
     },
     total=False,
 )
 
-
 class TrainingDataSchemaTypeDef(
     _RequiredTrainingDataSchemaTypeDef, _OptionalTrainingDataSchemaTypeDef
 ):
     pass
 
-
 ListEventPredictionsRequestRequestTypeDef = TypedDict(
     "ListEventPredictionsRequestRequestTypeDef",
     {
         "eventId": FilterConditionTypeDef,
         "eventType": FilterConditionTypeDef,
         "detectorId": FilterConditionTypeDef,
         "detectorVersionId": FilterConditionTypeDef,
@@ -2107,22 +2181,20 @@
         "externalEventsDetail": ExternalEventsDetailTypeDef,
         "ingestedEventsDetail": IngestedEventsDetailTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class UpdateModelVersionRequestRequestTypeDef(
     _RequiredUpdateModelVersionRequestRequestTypeDef,
     _OptionalUpdateModelVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateModelVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelVersionRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "trainingDataSource": TrainingDataSourceEnumType,
         "trainingDataSchema": TrainingDataSchemaTypeDef,
@@ -2134,22 +2206,20 @@
         "externalEventsDetail": ExternalEventsDetailTypeDef,
         "ingestedEventsDetail": IngestedEventsDetailTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateModelVersionRequestRequestTypeDef(
     _RequiredCreateModelVersionRequestRequestTypeDef,
     _OptionalCreateModelVersionRequestRequestTypeDef,
 ):
     pass
 
-
 GetModelVersionResultTypeDef = TypedDict(
     "GetModelVersionResultTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
         "trainingDataSource": TrainingDataSourceEnumType,
```

### Comparing `mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector/type_defs.pyi` & `mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from .literals import (
     AsyncJobStatusType,
     DataSourceType,
     DataTypeType,
     DetectorVersionStatusType,
     EventIngestionType,
+    ListUpdateModeType,
     ModelEndpointStatusType,
     ModelInputDataFormatType,
     ModelOutputDataFormatType,
     ModelTypeEnumType,
     ModelVersionStatusType,
     RuleExecutionModeType,
     TrainingDataSourceEnumType,
@@ -37,19 +38,21 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ATIMetricDataPointTypeDef",
     "ATIModelPerformanceTypeDef",
     "AggregatedLogOddsMetricTypeDef",
     "AggregatedVariablesImpactExplanationTypeDef",
+    "AllowDenyListTypeDef",
     "BatchCreateVariableErrorTypeDef",
     "TagTypeDef",
     "VariableEntryTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetVariableErrorTypeDef",
     "BatchGetVariableRequestRequestTypeDef",
     "VariableTypeDef",
@@ -68,14 +71,15 @@
     "DeleteDetectorVersionRequestRequestTypeDef",
     "DeleteEntityTypeRequestRequestTypeDef",
     "DeleteEventRequestRequestTypeDef",
     "DeleteEventTypeRequestRequestTypeDef",
     "DeleteEventsByEventTypeRequestRequestTypeDef",
     "DeleteExternalModelRequestRequestTypeDef",
     "DeleteLabelRequestRequestTypeDef",
+    "DeleteListRequestRequestTypeDef",
     "DeleteModelRequestRequestTypeDef",
     "DeleteModelVersionRequestRequestTypeDef",
     "DeleteOutcomeRequestRequestTypeDef",
     "DeleteVariableRequestRequestTypeDef",
     "DescribeDetectorRequestRequestTypeDef",
     "DetectorVersionSummaryTypeDef",
     "DescribeModelVersionsRequestRequestTypeDef",
@@ -102,14 +106,16 @@
     "RuleResultTypeDef",
     "GetEventRequestRequestTypeDef",
     "GetEventTypesRequestRequestTypeDef",
     "GetExternalModelsRequestRequestTypeDef",
     "KMSKeyTypeDef",
     "GetLabelsRequestRequestTypeDef",
     "LabelTypeDef",
+    "GetListElementsRequestRequestTypeDef",
+    "GetListsMetadataRequestRequestTypeDef",
     "GetModelVersionRequestRequestTypeDef",
     "GetModelsRequestRequestTypeDef",
     "ModelTypeDef",
     "GetOutcomesRequestRequestTypeDef",
     "OutcomeTypeDef",
     "GetRulesRequestRequestTypeDef",
     "RuleDetailTypeDef",
@@ -125,21 +131,23 @@
     "VariableImpactExplanationTypeDef",
     "PutKMSEncryptionKeyRequestRequestTypeDef",
     "TFIMetricDataPointTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDetectorVersionMetadataRequestRequestTypeDef",
     "UpdateDetectorVersionStatusRequestRequestTypeDef",
     "UpdateEventLabelRequestRequestTypeDef",
+    "UpdateListRequestRequestTypeDef",
     "UpdateModelRequestRequestTypeDef",
     "UpdateModelVersionStatusRequestRequestTypeDef",
     "UpdateVariableRequestRequestTypeDef",
     "ATITrainingMetricsValueTypeDef",
     "AggregatedVariablesImportanceMetricsTypeDef",
     "CreateBatchImportJobRequestRequestTypeDef",
     "CreateBatchPredictionJobRequestRequestTypeDef",
+    "CreateListRequestRequestTypeDef",
     "CreateModelRequestRequestTypeDef",
     "CreateRuleRequestRequestTypeDef",
     "CreateVariableRequestRequestTypeDef",
     "PutDetectorRequestRequestTypeDef",
     "PutEntityTypeRequestRequestTypeDef",
     "PutEventTypeRequestRequestTypeDef",
     "PutLabelRequestRequestTypeDef",
@@ -147,14 +155,16 @@
     "TagResourceRequestRequestTypeDef",
     "BatchCreateVariableRequestRequestTypeDef",
     "BatchCreateVariableResultTypeDef",
     "CreateDetectorVersionResultTypeDef",
     "CreateModelVersionResultTypeDef",
     "DeleteEventsByEventTypeResultTypeDef",
     "GetDeleteEventsByEventTypeStatusResultTypeDef",
+    "GetListElementsResultTypeDef",
+    "GetListsMetadataResultTypeDef",
     "ListTagsForResourceResultTypeDef",
     "UpdateModelVersionResultTypeDef",
     "BatchGetVariableResultTypeDef",
     "GetVariablesResultTypeDef",
     "GetBatchImportJobsResultTypeDef",
     "GetBatchPredictionJobsResultTypeDef",
     "ModelScoresTypeDef",
@@ -243,14 +253,37 @@
         "eventVariableNames": List[str],
         "relativeImpact": str,
         "logOddsImpact": float,
     },
     total=False,
 )
 
+_RequiredAllowDenyListTypeDef = TypedDict(
+    "_RequiredAllowDenyListTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalAllowDenyListTypeDef = TypedDict(
+    "_OptionalAllowDenyListTypeDef",
+    {
+        "description": str,
+        "variableType": str,
+        "createdTime": str,
+        "updatedTime": str,
+        "arn": str,
+    },
+    total=False,
+)
+
+
+class AllowDenyListTypeDef(_RequiredAllowDenyListTypeDef, _OptionalAllowDenyListTypeDef):
+    pass
+
+
 BatchCreateVariableErrorTypeDef = TypedDict(
     "BatchCreateVariableErrorTypeDef",
     {
         "name": str,
         "code": int,
         "message": str,
     },
@@ -390,17 +423,19 @@
     "_OptionalModelVersionTypeDef",
     {
         "arn": str,
     },
     total=False,
 )
 
+
 class ModelVersionTypeDef(_RequiredModelVersionTypeDef, _OptionalModelVersionTypeDef):
     pass
 
+
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "detectorId": str,
         "ruleId": str,
         "ruleVersion": str,
     },
@@ -483,19 +518,21 @@
     "_OptionalDeleteEventRequestRequestTypeDef",
     {
         "deleteAuditHistory": bool,
     },
     total=False,
 )
 
+
 class DeleteEventRequestRequestTypeDef(
     _RequiredDeleteEventRequestRequestTypeDef, _OptionalDeleteEventRequestRequestTypeDef
 ):
     pass
 
+
 DeleteEventTypeRequestRequestTypeDef = TypedDict(
     "DeleteEventTypeRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
@@ -516,14 +553,21 @@
 DeleteLabelRequestRequestTypeDef = TypedDict(
     "DeleteLabelRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
+DeleteListRequestRequestTypeDef = TypedDict(
+    "DeleteListRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+
 DeleteModelRequestRequestTypeDef = TypedDict(
     "DeleteModelRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
     },
 )
@@ -562,19 +606,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class DescribeDetectorRequestRequestTypeDef(
     _RequiredDescribeDetectorRequestRequestTypeDef, _OptionalDescribeDetectorRequestRequestTypeDef
 ):
     pass
 
+
 DetectorVersionSummaryTypeDef = TypedDict(
     "DetectorVersionSummaryTypeDef",
     {
         "detectorVersionId": str,
         "status": DetectorVersionStatusType,
         "description": str,
         "lastUpdatedTime": str,
@@ -709,19 +755,21 @@
         "format": ModelInputDataFormatType,
         "jsonInputTemplate": str,
         "csvInputTemplate": str,
     },
     total=False,
 )
 
+
 class ModelInputConfigurationTypeDef(
     _RequiredModelInputConfigurationTypeDef, _OptionalModelInputConfigurationTypeDef
 ):
     pass
 
+
 _RequiredModelOutputConfigurationTypeDef = TypedDict(
     "_RequiredModelOutputConfigurationTypeDef",
     {
         "format": ModelOutputDataFormatType,
     },
 )
 _OptionalModelOutputConfigurationTypeDef = TypedDict(
@@ -729,19 +777,21 @@
     {
         "jsonKeyToVariableMap": Dict[str, str],
         "csvIndexToVariableMap": Dict[str, str],
     },
     total=False,
 )
 
+
 class ModelOutputConfigurationTypeDef(
     _RequiredModelOutputConfigurationTypeDef, _OptionalModelOutputConfigurationTypeDef
 ):
     pass
 
+
 FilterConditionTypeDef = TypedDict(
     "FilterConditionTypeDef",
     {
         "value": str,
     },
     total=False,
 )
@@ -884,14 +934,46 @@
         "lastUpdatedTime": str,
         "createdTime": str,
         "arn": str,
     },
     total=False,
 )
 
+_RequiredGetListElementsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetListElementsRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalGetListElementsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetListElementsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class GetListElementsRequestRequestTypeDef(
+    _RequiredGetListElementsRequestRequestTypeDef, _OptionalGetListElementsRequestRequestTypeDef
+):
+    pass
+
+
+GetListsMetadataRequestRequestTypeDef = TypedDict(
+    "GetListsMetadataRequestRequestTypeDef",
+    {
+        "name": str,
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
 GetModelVersionRequestRequestTypeDef = TypedDict(
     "GetModelVersionRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
     },
@@ -957,19 +1039,21 @@
         "ruleVersion": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetRulesRequestRequestTypeDef(
     _RequiredGetRulesRequestRequestTypeDef, _OptionalGetRulesRequestRequestTypeDef
 ):
     pass
 
+
 RuleDetailTypeDef = TypedDict(
     "RuleDetailTypeDef",
     {
         "ruleId": str,
         "description": str,
         "detectorId": str,
         "ruleVersion": str,
@@ -1029,20 +1113,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
 LogOddsMetricTypeDef = TypedDict(
     "LogOddsMetricTypeDef",
     {
         "variableName": str,
         "variableType": str,
         "variableImportance": float,
     },
@@ -1138,14 +1224,38 @@
         "eventId": str,
         "eventTypeName": str,
         "assignedLabel": str,
         "labelTimestamp": str,
     },
 )
 
+_RequiredUpdateListRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateListRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalUpdateListRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateListRequestRequestTypeDef",
+    {
+        "elements": Sequence[str],
+        "description": str,
+        "updateMode": ListUpdateModeType,
+        "variableType": str,
+    },
+    total=False,
+)
+
+
+class UpdateListRequestRequestTypeDef(
+    _RequiredUpdateListRequestRequestTypeDef, _OptionalUpdateListRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredUpdateModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
     },
 )
@@ -1153,19 +1263,21 @@
     "_OptionalUpdateModelRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class UpdateModelRequestRequestTypeDef(
     _RequiredUpdateModelRequestRequestTypeDef, _OptionalUpdateModelRequestRequestTypeDef
 ):
     pass
 
+
 UpdateModelVersionStatusRequestRequestTypeDef = TypedDict(
     "UpdateModelVersionStatusRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
         "status": ModelVersionStatusType,
@@ -1184,19 +1296,21 @@
         "defaultValue": str,
         "description": str,
         "variableType": str,
     },
     total=False,
 )
 
+
 class UpdateVariableRequestRequestTypeDef(
     _RequiredUpdateVariableRequestRequestTypeDef, _OptionalUpdateVariableRequestRequestTypeDef
 ):
     pass
 
+
 ATITrainingMetricsValueTypeDef = TypedDict(
     "ATITrainingMetricsValueTypeDef",
     {
         "metricDataPoints": List[ATIMetricDataPointTypeDef],
         "modelPerformance": ATIModelPerformanceTypeDef,
     },
     total=False,
@@ -1224,20 +1338,22 @@
     "_OptionalCreateBatchImportJobRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateBatchImportJobRequestRequestTypeDef(
     _RequiredCreateBatchImportJobRequestRequestTypeDef,
     _OptionalCreateBatchImportJobRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateBatchPredictionJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBatchPredictionJobRequestRequestTypeDef",
     {
         "jobId": str,
         "inputPath": str,
         "outputPath": str,
         "eventTypeName": str,
@@ -1250,20 +1366,46 @@
     {
         "detectorVersion": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateBatchPredictionJobRequestRequestTypeDef(
     _RequiredCreateBatchPredictionJobRequestRequestTypeDef,
     _OptionalCreateBatchPredictionJobRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredCreateListRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateListRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateListRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateListRequestRequestTypeDef",
+    {
+        "elements": Sequence[str],
+        "variableType": str,
+        "description": str,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateListRequestRequestTypeDef(
+    _RequiredCreateListRequestRequestTypeDef, _OptionalCreateListRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredCreateModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "eventTypeName": str,
     },
@@ -1273,19 +1415,21 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateModelRequestRequestTypeDef(
     _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRuleRequestRequestTypeDef",
     {
         "ruleId": str,
         "detectorId": str,
         "expression": str,
         "language": Literal["DETECTORPL"],
@@ -1297,19 +1441,21 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateRuleRequestRequestTypeDef(
     _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateVariableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVariableRequestRequestTypeDef",
     {
         "name": str,
         "dataType": DataTypeType,
         "dataSource": DataSourceType,
         "defaultValue": str,
@@ -1321,19 +1467,21 @@
         "description": str,
         "variableType": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateVariableRequestRequestTypeDef(
     _RequiredCreateVariableRequestRequestTypeDef, _OptionalCreateVariableRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredPutDetectorRequestRequestTypeDef",
     {
         "detectorId": str,
         "eventTypeName": str,
     },
 )
@@ -1342,19 +1490,21 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutDetectorRequestRequestTypeDef(
     _RequiredPutDetectorRequestRequestTypeDef, _OptionalPutDetectorRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutEntityTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutEntityTypeRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutEntityTypeRequestRequestTypeDef = TypedDict(
@@ -1362,19 +1512,21 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutEntityTypeRequestRequestTypeDef(
     _RequiredPutEntityTypeRequestRequestTypeDef, _OptionalPutEntityTypeRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutEventTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutEventTypeRequestRequestTypeDef",
     {
         "name": str,
         "eventVariables": Sequence[str],
         "entityTypes": Sequence[str],
     },
@@ -1386,19 +1538,21 @@
         "labels": Sequence[str],
         "eventIngestion": EventIngestionType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutEventTypeRequestRequestTypeDef(
     _RequiredPutEventTypeRequestRequestTypeDef, _OptionalPutEventTypeRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutLabelRequestRequestTypeDef = TypedDict(
     "_RequiredPutLabelRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutLabelRequestRequestTypeDef = TypedDict(
@@ -1406,19 +1560,21 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutLabelRequestRequestTypeDef(
     _RequiredPutLabelRequestRequestTypeDef, _OptionalPutLabelRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutOutcomeRequestRequestTypeDef = TypedDict(
     "_RequiredPutOutcomeRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalPutOutcomeRequestRequestTypeDef = TypedDict(
@@ -1426,19 +1582,21 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutOutcomeRequestRequestTypeDef(
     _RequiredPutOutcomeRequestRequestTypeDef, _OptionalPutOutcomeRequestRequestTypeDef
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1453,20 +1611,22 @@
     "_OptionalBatchCreateVariableRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class BatchCreateVariableRequestRequestTypeDef(
     _RequiredBatchCreateVariableRequestRequestTypeDef,
     _OptionalBatchCreateVariableRequestRequestTypeDef,
 ):
     pass
 
+
 BatchCreateVariableResultTypeDef = TypedDict(
     "BatchCreateVariableResultTypeDef",
     {
         "errors": List[BatchCreateVariableErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1506,14 +1666,32 @@
     {
         "eventTypeName": str,
         "eventsDeletionStatus": AsyncJobStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetListElementsResultTypeDef = TypedDict(
+    "GetListElementsResultTypeDef",
+    {
+        "elements": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetListsMetadataResultTypeDef = TypedDict(
+    "GetListsMetadataResultTypeDef",
+    {
+        "lists": List[AllowDenyListTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
         "tags": List[TagTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1590,20 +1768,22 @@
         "modelVersions": Sequence[ModelVersionTypeDef],
         "ruleExecutionMode": RuleExecutionModeType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDetectorVersionRequestRequestTypeDef(
     _RequiredCreateDetectorVersionRequestRequestTypeDef,
     _OptionalCreateDetectorVersionRequestRequestTypeDef,
 ):
     pass
 
+
 CreateRuleResultTypeDef = TypedDict(
     "CreateRuleResultTypeDef",
     {
         "rule": RuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1648,20 +1828,22 @@
         "description": str,
         "modelVersions": Sequence[ModelVersionTypeDef],
         "ruleExecutionMode": RuleExecutionModeType,
     },
     total=False,
 )
 
+
 class UpdateDetectorVersionRequestRequestTypeDef(
     _RequiredUpdateDetectorVersionRequestRequestTypeDef,
     _OptionalUpdateDetectorVersionRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateRuleMetadataRequestRequestTypeDef = TypedDict(
     "UpdateRuleMetadataRequestRequestTypeDef",
     {
         "rule": RuleTypeDef,
         "description": str,
     },
 )
@@ -1680,19 +1862,21 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class UpdateRuleVersionRequestRequestTypeDef(
     _RequiredUpdateRuleVersionRequestRequestTypeDef, _OptionalUpdateRuleVersionRequestRequestTypeDef
 ):
     pass
 
+
 UpdateRuleVersionResultTypeDef = TypedDict(
     "UpdateRuleVersionResultTypeDef",
     {
         "rule": RuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1755,19 +1939,21 @@
     {
         "assignedLabel": str,
         "labelTimestamp": str,
     },
     total=False,
 )
 
+
 class SendEventRequestRequestTypeDef(
     _RequiredSendEventRequestRequestTypeDef, _OptionalSendEventRequestRequestTypeDef
 ):
     pass
 
+
 GetEntityTypesResultTypeDef = TypedDict(
     "GetEntityTypesResultTypeDef",
     {
         "entityTypes": List[EntityTypeTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1839,19 +2025,21 @@
     "_OptionalPutExternalModelRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutExternalModelRequestRequestTypeDef(
     _RequiredPutExternalModelRequestRequestTypeDef, _OptionalPutExternalModelRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetEventPredictionRequestRequestTypeDef = TypedDict(
     "_RequiredGetEventPredictionRequestRequestTypeDef",
     {
         "detectorId": str,
         "eventId": str,
         "eventTypeName": str,
         "entities": Sequence[EntityTypeDef],
@@ -1864,20 +2052,22 @@
     {
         "detectorVersionId": str,
         "externalModelEndpointDataBlobs": Mapping[str, ModelEndpointDataBlobTypeDef],
     },
     total=False,
 )
 
+
 class GetEventPredictionRequestRequestTypeDef(
     _RequiredGetEventPredictionRequestRequestTypeDef,
     _OptionalGetEventPredictionRequestRequestTypeDef,
 ):
     pass
 
+
 GetKMSEncryptionKeyResultTypeDef = TypedDict(
     "GetKMSEncryptionKeyResultTypeDef",
     {
         "kmsKey": KMSKeyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1935,19 +2125,21 @@
     "_OptionalTrainingDataSchemaTypeDef",
     {
         "labelSchema": LabelSchemaTypeDef,
     },
     total=False,
 )
 
+
 class TrainingDataSchemaTypeDef(
     _RequiredTrainingDataSchemaTypeDef, _OptionalTrainingDataSchemaTypeDef
 ):
     pass
 
+
 ListEventPredictionsRequestRequestTypeDef = TypedDict(
     "ListEventPredictionsRequestRequestTypeDef",
     {
         "eventId": FilterConditionTypeDef,
         "eventType": FilterConditionTypeDef,
         "detectorId": FilterConditionTypeDef,
         "detectorVersionId": FilterConditionTypeDef,
@@ -2052,20 +2244,22 @@
         "externalEventsDetail": ExternalEventsDetailTypeDef,
         "ingestedEventsDetail": IngestedEventsDetailTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class UpdateModelVersionRequestRequestTypeDef(
     _RequiredUpdateModelVersionRequestRequestTypeDef,
     _OptionalUpdateModelVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateModelVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelVersionRequestRequestTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "trainingDataSource": TrainingDataSourceEnumType,
         "trainingDataSchema": TrainingDataSchemaTypeDef,
@@ -2077,20 +2271,22 @@
         "externalEventsDetail": ExternalEventsDetailTypeDef,
         "ingestedEventsDetail": IngestedEventsDetailTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateModelVersionRequestRequestTypeDef(
     _RequiredCreateModelVersionRequestRequestTypeDef,
     _OptionalCreateModelVersionRequestRequestTypeDef,
 ):
     pass
 
+
 GetModelVersionResultTypeDef = TypedDict(
     "GetModelVersionResultTypeDef",
     {
         "modelId": str,
         "modelType": ModelTypeEnumType,
         "modelVersionNumber": str,
         "trainingDataSource": TrainingDataSourceEnumType,
```

### Comparing `mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector.egg-info/PKG-INFO` & `mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-frauddetector
-Version: 1.26.65
-Summary: Type annotations for boto3.FraudDetector 1.26.65 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.72
+Summary: Type annotations for boto3.FraudDetector 1.26.72 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_frauddetector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-frauddetector.svg?color=blue)](https://pypi.org/project/mypy-boto3-frauddetector)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-frauddetector?color=blue)](https://pypistats.org/packages/mypy-boto3-frauddetector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FraudDetector 1.26.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
+[boto3.FraudDetector 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -282,14 +282,15 @@
 from mypy_boto3_frauddetector.literals import (
     AsyncJobStatusType,
     DataSourceType,
     DataTypeType,
     DetectorVersionStatusType,
     EventIngestionType,
     LanguageType,
+    ListUpdateModeType,
     ModelEndpointStatusType,
     ModelInputDataFormatType,
     ModelOutputDataFormatType,
     ModelSourceType,
     ModelTypeEnumType,
     ModelVersionStatusType,
     RuleExecutionModeType,
@@ -315,14 +316,15 @@
 
 ```python
 from mypy_boto3_frauddetector.type_defs import (
     ATIMetricDataPointTypeDef,
     ATIModelPerformanceTypeDef,
     AggregatedLogOddsMetricTypeDef,
     AggregatedVariablesImpactExplanationTypeDef,
+    AllowDenyListTypeDef,
     BatchCreateVariableErrorTypeDef,
     TagTypeDef,
     VariableEntryTypeDef,
     ResponseMetadataTypeDef,
     BatchGetVariableErrorTypeDef,
     BatchGetVariableRequestRequestTypeDef,
     VariableTypeDef,
@@ -341,14 +343,15 @@
     DeleteDetectorVersionRequestRequestTypeDef,
     DeleteEntityTypeRequestRequestTypeDef,
     DeleteEventRequestRequestTypeDef,
     DeleteEventTypeRequestRequestTypeDef,
     DeleteEventsByEventTypeRequestRequestTypeDef,
     DeleteExternalModelRequestRequestTypeDef,
     DeleteLabelRequestRequestTypeDef,
+    DeleteListRequestRequestTypeDef,
     DeleteModelRequestRequestTypeDef,
     DeleteModelVersionRequestRequestTypeDef,
     DeleteOutcomeRequestRequestTypeDef,
     DeleteVariableRequestRequestTypeDef,
     DescribeDetectorRequestRequestTypeDef,
     DetectorVersionSummaryTypeDef,
     DescribeModelVersionsRequestRequestTypeDef,
@@ -375,14 +378,16 @@
     RuleResultTypeDef,
     GetEventRequestRequestTypeDef,
     GetEventTypesRequestRequestTypeDef,
     GetExternalModelsRequestRequestTypeDef,
     KMSKeyTypeDef,
     GetLabelsRequestRequestTypeDef,
     LabelTypeDef,
+    GetListElementsRequestRequestTypeDef,
+    GetListsMetadataRequestRequestTypeDef,
     GetModelVersionRequestRequestTypeDef,
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetOutcomesRequestRequestTypeDef,
     OutcomeTypeDef,
     GetRulesRequestRequestTypeDef,
     RuleDetailTypeDef,
@@ -398,21 +403,23 @@
     VariableImpactExplanationTypeDef,
     PutKMSEncryptionKeyRequestRequestTypeDef,
     TFIMetricDataPointTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDetectorVersionMetadataRequestRequestTypeDef,
     UpdateDetectorVersionStatusRequestRequestTypeDef,
     UpdateEventLabelRequestRequestTypeDef,
+    UpdateListRequestRequestTypeDef,
     UpdateModelRequestRequestTypeDef,
     UpdateModelVersionStatusRequestRequestTypeDef,
     UpdateVariableRequestRequestTypeDef,
     ATITrainingMetricsValueTypeDef,
     AggregatedVariablesImportanceMetricsTypeDef,
     CreateBatchImportJobRequestRequestTypeDef,
     CreateBatchPredictionJobRequestRequestTypeDef,
+    CreateListRequestRequestTypeDef,
     CreateModelRequestRequestTypeDef,
     CreateRuleRequestRequestTypeDef,
     CreateVariableRequestRequestTypeDef,
     PutDetectorRequestRequestTypeDef,
     PutEntityTypeRequestRequestTypeDef,
     PutEventTypeRequestRequestTypeDef,
     PutLabelRequestRequestTypeDef,
@@ -420,14 +427,16 @@
     TagResourceRequestRequestTypeDef,
     BatchCreateVariableRequestRequestTypeDef,
     BatchCreateVariableResultTypeDef,
     CreateDetectorVersionResultTypeDef,
     CreateModelVersionResultTypeDef,
     DeleteEventsByEventTypeResultTypeDef,
     GetDeleteEventsByEventTypeStatusResultTypeDef,
+    GetListElementsResultTypeDef,
+    GetListsMetadataResultTypeDef,
     ListTagsForResourceResultTypeDef,
     UpdateModelVersionResultTypeDef,
     BatchGetVariableResultTypeDef,
     GetVariablesResultTypeDef,
     GetBatchImportJobsResultTypeDef,
     GetBatchPredictionJobsResultTypeDef,
     ModelScoresTypeDef,
```

### Comparing `mypy-boto3-frauddetector-1.26.65/mypy_boto3_frauddetector.egg-info/SOURCES.txt` & `mypy-boto3-frauddetector-1.26.72/mypy_boto3_frauddetector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-frauddetector-1.26.65/setup.py` & `mypy-boto3-frauddetector-1.26.72/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-frauddetector",
-    version="1.26.65",
+    version="1.26.72",
     packages=["mypy_boto3_frauddetector"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FraudDetector 1.26.65 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.FraudDetector 1.26.72 service generated with mypy-boto3-builder"
         " 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

