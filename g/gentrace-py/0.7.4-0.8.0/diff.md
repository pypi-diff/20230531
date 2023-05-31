# Comparing `tmp/gentrace_py-0.7.4.tar.gz` & `tmp/gentrace_py-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentrace_py-0.7.4.tar", max compression
+gzip compressed data, was "gentrace_py-0.8.0.tar", max compression
```

## Comparing `gentrace_py-0.7.4.tar` & `gentrace_py-0.8.0.tar`

### file list

```diff
@@ -1,39 +1,54 @@
--rw-r--r--   0        0        0     1058 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/__init__.py
--rw-r--r--   0        0        0    59420 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/api_client.py
--rw-r--r--   0        0        0      215 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/apis/__init__.py
--rw-r--r--   0        0        0      325 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/apis/path_to_api.py
--rw-r--r--   0        0        0      235 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/apis/paths/__init__.py
--rw-r--r--   0        0        0      105 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/apis/paths/pipeline_run.py
--rw-r--r--   0        0        0      459 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/apis/tag_to_api.py
--rw-r--r--   0        0        0      335 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/apis/tags/__init__.py
--rw-r--r--   0        0        0      485 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/apis/tags/ingestion_api.py
--rw-r--r--   0        0        0    15476 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/configuration.py
--rw-r--r--   0        0        0     4444 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/exceptions.py
--rw-r--r--   0        0        0      342 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/model/__init__.py
--rw-r--r--   0        0        0     5209 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/model/feedback_request.py
--rw-r--r--   0        0        0     4998 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/model/feedback_request.pyi
--rw-r--r--   0        0        0     2144 2023-05-19 19:19:11.229895 gentrace_py-0.7.4/gentrace/model/feedback_response.py
--rw-r--r--   0        0        0     2121 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/model/feedback_response.pyi
--rw-r--r--   0        0        0    33338 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/model/pipeline_run_request.py
--rw-r--r--   0        0        0    32730 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/model/pipeline_run_request.pyi
--rw-r--r--   0        0        0     2779 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/model/pipeline_run_response.py
--rw-r--r--   0        0        0     2739 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/model/pipeline_run_response.pyi
--rw-r--r--   0        0        0      640 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/models/__init__.py
--rw-r--r--   0        0        0      318 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/paths/__init__.py
--rw-r--r--   0        0        0      299 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/paths/pipeline_run/__init__.py
--rw-r--r--   0        0        0    12578 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/paths/pipeline_run/post.py
--rw-r--r--   0        0        0    12355 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/paths/pipeline_run/post.pyi
--rw-r--r--   0        0        0      229 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/__init__.py
--rw-r--r--   0        0        0     1134 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/getters.py
--rw-r--r--   0        0        0      182 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/llms/__init__.py
--rw-r--r--   0        0        0    27820 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/llms/openai.py
--rw-r--r--   0        0        0     3042 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/pipeline.py
--rw-r--r--   0        0        0     6400 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/pipeline_run.py
--rw-r--r--   0        0        0      531 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/step_run.py
--rw-r--r--   0        0        0     3706 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/utils.py
--rw-r--r--   0        0        0      219 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/vectorstores/__init__.py
--rw-r--r--   0        0        0    12262 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/providers/vectorstores/pinecone.py
--rw-r--r--   0        0        0    10398 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/rest.py
--rw-r--r--   0        0        0   103185 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/gentrace/schemas.py
--rw-r--r--   0        0        0     1571 2023-05-19 19:19:11.233895 gentrace_py-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1026 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/__init__.py
+-rw-r--r--   0        0        0    58467 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/api_client.py
+-rw-r--r--   0        0        0      214 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/apis/__init__.py
+-rw-r--r--   0        0        0      576 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/apis/path_to_api.py
+-rw-r--r--   0        0        0      235 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/apis/paths/__init__.py
+-rw-r--r--   0        0        0      105 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/apis/paths/pipeline_run.py
+-rw-r--r--   0        0        0       96 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/apis/paths/test_case.py
+-rw-r--r--   0        0        0      162 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/apis/paths/test_run.py
+-rw-r--r--   0        0        0      428 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/apis/tag_to_api.py
+-rw-r--r--   0        0        0      325 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/apis/tags/__init__.py
+-rw-r--r--   0        0        0      687 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/apis/tags/core_api.py
+-rw-r--r--   0        0        0    15451 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/configuration.py
+-rw-r--r--   0        0        0     4505 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/exceptions.py
+-rw-r--r--   0        0        0      342 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/model/__init__.py
+-rw-r--r--   0        0        0     4839 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/model/feedback_request.py
+-rw-r--r--   0        0        0     4680 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/model/feedback_request.pyi
+-rw-r--r--   0        0        0     2071 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/model/feedback_response.py
+-rw-r--r--   0        0        0     2070 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/model/feedback_response.pyi
+-rw-r--r--   0        0        0    22463 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/model/pipeline_run_request.py
+-rw-r--r--   0        0        0    22462 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/model/pipeline_run_request.pyi
+-rw-r--r--   0        0        0     2508 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/model/pipeline_run_response.py
+-rw-r--r--   0        0        0     2507 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/model/pipeline_run_response.pyi
+-rw-r--r--   0        0        0     5025 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/model/test_case.py
+-rw-r--r--   0        0        0     5024 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/model/test_case.pyi
+-rw-r--r--   0        0        0     4468 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/model/test_run.py
+-rw-r--r--   0        0        0     4467 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/model/test_run.pyi
+-rw-r--r--   0        0        0      730 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/models/__init__.py
+-rw-r--r--   0        0        0      372 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/paths/__init__.py
+-rw-r--r--   0        0        0      298 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/paths/pipeline_run/__init__.py
+-rw-r--r--   0        0        0    12466 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/paths/pipeline_run/post.py
+-rw-r--r--   0        0        0    12295 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/paths/pipeline_run/post.pyi
+-rw-r--r--   0        0        0      292 2023-05-31 21:57:00.709270 gentrace_py-0.8.0/gentrace/paths/test_case/__init__.py
+-rw-r--r--   0        0        0    15925 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/paths/test_case/get.py
+-rw-r--r--   0        0        0    15754 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/paths/test_case/get.pyi
+-rw-r--r--   0        0        0      290 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/paths/test_run/__init__.py
+-rw-r--r--   0        0        0    23021 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/paths/test_run/get.py
+-rw-r--r--   0        0        0    22910 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/paths/test_run/get.pyi
+-rw-r--r--   0        0        0    24323 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/paths/test_run/post.py
+-rw-r--r--   0        0        0    24103 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/paths/test_run/post.pyi
+-rw-r--r--   0        0        0      229 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/providers/__init__.py
+-rw-r--r--   0        0        0     1146 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/providers/evaluation.py
+-rw-r--r--   0        0        0     1134 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/providers/getters.py
+-rw-r--r--   0        0        0      182 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/providers/llms/__init__.py
+-rw-r--r--   0        0        0    27820 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/providers/llms/openai.py
+-rw-r--r--   0        0        0     3042 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/providers/pipeline.py
+-rw-r--r--   0        0        0     6355 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/providers/pipeline_run.py
+-rw-r--r--   0        0        0      531 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/providers/step_run.py
+-rw-r--r--   0        0        0     3691 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/providers/utils.py
+-rw-r--r--   0        0        0      219 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/providers/vectorstores/__init__.py
+-rw-r--r--   0        0        0    12262 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/providers/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    10526 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/rest.py
+-rw-r--r--   0        0        0    97629 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/gentrace/schemas.py
+-rw-r--r--   0        0        0     1591 2023-05-31 21:57:00.713271 gentrace_py-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 gentrace_py-0.8.0/PKG-INFO
```

### Comparing `gentrace_py-0.7.4/gentrace/__init__.py` & `gentrace_py-0.8.0/gentrace/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # coding: utf-8
 
 # flake8: noqa
 
-""" Gentrace API
+"""
+    Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.8
+    The version of the OpenAPI document: 0.4.13
     Generated by: https://openapi-generator.tech
 """
 
 __version__ = "1.0.0"
 
 # import ApiClient
 from gentrace.api_client import ApiClient
@@ -22,23 +23,17 @@
 from gentrace.exceptions import OpenApiException
 from gentrace.exceptions import ApiAttributeError
 from gentrace.exceptions import ApiTypeError
 from gentrace.exceptions import ApiValueError
 from gentrace.exceptions import ApiKeyError
 from gentrace.exceptions import ApiException
 
+from gentrace.providers.evaluation import Evaluation
 from gentrace.providers.pipeline import Pipeline
 from gentrace.providers.pipeline_run import PipelineRun, flush
 from gentrace.providers.step_run import StepRun
-from gentrace.providers.utils import (
-    to_date_string,
-    log_debug,
-    log_info,
-    log_warn,
-    log_exception,
-)
+from gentrace.providers.utils import to_date_string
 
 from gentrace.providers.getters import *
 
 api_key = ""
 host = ""
-log_level = "warn"
```

### Comparing `gentrace_py-0.7.4/gentrace/api_client.py` & `gentrace_py-0.8.0/gentrace/api_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.8
+    The version of the OpenAPI document: 0.4.13
     Generated by: https://openapi-generator.tech
 """
 
 import atexit
 import email
 import enum
 import io
@@ -49,15 +49,15 @@
     def __eq__(self, other):
         if not isinstance(other, RequestField):
             return False
         return self.__dict__ == other.__dict__
 
 
 class JSONEncoder(json.JSONEncoder):
-    compact_separators = (",", ":")
+    compact_separators = (',', ':')
 
     def default(self, obj):
         if isinstance(obj, str):
             return str(obj)
         elif isinstance(obj, float):
             return float(obj)
         elif isinstance(obj, int):
@@ -70,47 +70,45 @@
             return None
         elif isinstance(obj, BoolClass):
             return bool(obj)
         elif isinstance(obj, (dict, frozendict.frozendict)):
             return {key: self.default(val) for key, val in obj.items()}
         elif isinstance(obj, (list, tuple)):
             return [self.default(item) for item in obj]
-        raise ApiValueError(
-            "Unable to prepare type {} for serialization".format(obj.__class__.__name__)
-        )
+        raise ApiValueError('Unable to prepare type {} for serialization'.format(obj.__class__.__name__))
 
 
 class ParameterInType(enum.Enum):
-    QUERY = "query"
-    HEADER = "header"
-    PATH = "path"
-    COOKIE = "cookie"
+    QUERY = 'query'
+    HEADER = 'header'
+    PATH = 'path'
+    COOKIE = 'cookie'
 
 
 class ParameterStyle(enum.Enum):
-    MATRIX = "matrix"
-    LABEL = "label"
-    FORM = "form"
-    SIMPLE = "simple"
-    SPACE_DELIMITED = "spaceDelimited"
-    PIPE_DELIMITED = "pipeDelimited"
-    DEEP_OBJECT = "deepObject"
+    MATRIX = 'matrix'
+    LABEL = 'label'
+    FORM = 'form'
+    SIMPLE = 'simple'
+    SPACE_DELIMITED = 'spaceDelimited'
+    PIPE_DELIMITED = 'pipeDelimited'
+    DEEP_OBJECT = 'deepObject'
 
 
 class PrefixSeparatorIterator:
     # A class to store prefixes and separators for rfc6570 expansions
 
     def __init__(self, prefix: str, separator: str):
         self.prefix = prefix
         self.separator = separator
         self.first = True
-        if separator in {".", "|", "%20"}:
+        if separator in {'.', '|', '%20'}:
             item_separator = separator
         else:
-            item_separator = ","
+            item_separator = ','
         self.item_separator = item_separator
 
     def __iter__(self):
         return self
 
     def __next__(self):
         if self.first:
@@ -144,69 +142,60 @@
             return None
         elif isinstance(in_data, list) and not in_data:
             # ignored by the expansion process https://datatracker.ietf.org/doc/html/rfc6570#section-3.2.1
             return None
         elif isinstance(in_data, dict) and not in_data:
             # ignored by the expansion process https://datatracker.ietf.org/doc/html/rfc6570#section-3.2.1
             return None
-        raise ApiValueError(
-            "Unable to generate a ref6570 item representation of {}".format(in_data)
-        )
+        raise ApiValueError('Unable to generate a ref6570 item representation of {}'.format(in_data))
 
     @staticmethod
     def _to_dict(name: str, value: str):
         return {name: value}
 
     @classmethod
     def __ref6570_str_float_int_expansion(
         cls,
         variable_name: str,
         in_data: typing.Any,
         explode: bool,
         percent_encode: bool,
         prefix_separator_iterator: PrefixSeparatorIterator,
         var_name_piece: str,
-        named_parameter_expansion: bool,
+        named_parameter_expansion: bool
     ) -> str:
         item_value = cls.__ref6570_item_value(in_data, percent_encode)
-        if item_value is None or (
-            item_value == "" and prefix_separator_iterator.separator == ";"
-        ):
+        if item_value is None or (item_value == '' and prefix_separator_iterator.separator == ';'):
             return next(prefix_separator_iterator) + var_name_piece
-        value_pair_equals = "=" if named_parameter_expansion else ""
-        return (
-            next(prefix_separator_iterator)
-            + var_name_piece
-            + value_pair_equals
-            + item_value
-        )
+        value_pair_equals = '=' if named_parameter_expansion else ''
+        return next(prefix_separator_iterator) + var_name_piece + value_pair_equals + item_value
 
     @classmethod
     def __ref6570_list_expansion(
         cls,
         variable_name: str,
         in_data: typing.Any,
         explode: bool,
         percent_encode: bool,
         prefix_separator_iterator: PrefixSeparatorIterator,
         var_name_piece: str,
-        named_parameter_expansion: bool,
+        named_parameter_expansion: bool
     ) -> str:
         item_values = [cls.__ref6570_item_value(v, percent_encode) for v in in_data]
         item_values = [v for v in item_values if v is not None]
         if not item_values:
             # ignored by the expansion process https://datatracker.ietf.org/doc/html/rfc6570#section-3.2.1
             return ""
-        value_pair_equals = "=" if named_parameter_expansion else ""
+        value_pair_equals = '=' if named_parameter_expansion else ''
         if not explode:
             return (
-                next(prefix_separator_iterator)
-                + var_name_piece
-                + value_pair_equals
-                + prefix_separator_iterator.item_separator.join(item_values)
+                next(prefix_separator_iterator) +
+                var_name_piece +
+                value_pair_equals +
+                prefix_separator_iterator.item_separator.join(item_values)
             )
         # exploded
         return next(prefix_separator_iterator) + next(prefix_separator_iterator).join(
             [var_name_piece + value_pair_equals + val for val in item_values]
         )
 
     @classmethod
@@ -214,93 +203,86 @@
         cls,
         variable_name: str,
         in_data: typing.Any,
         explode: bool,
         percent_encode: bool,
         prefix_separator_iterator: PrefixSeparatorIterator,
         var_name_piece: str,
-        named_parameter_expansion: bool,
+        named_parameter_expansion: bool
     ) -> str:
-        in_data_transformed = {
-            key: cls.__ref6570_item_value(val, percent_encode)
-            for key, val in in_data.items()
-        }
-        in_data_transformed = {
-            key: val for key, val in in_data_transformed.items() if val is not None
-        }
+        in_data_transformed = {key: cls.__ref6570_item_value(val, percent_encode) for key, val in in_data.items()}
+        in_data_transformed = {key: val for key, val in in_data_transformed.items() if val is not None}
         if not in_data_transformed:
             # ignored by the expansion process https://datatracker.ietf.org/doc/html/rfc6570#section-3.2.1
             return ""
-        value_pair_equals = "=" if named_parameter_expansion else ""
+        value_pair_equals = '=' if named_parameter_expansion else ''
         if not explode:
             return (
-                next(prefix_separator_iterator)
-                + var_name_piece
-                + value_pair_equals
-                + prefix_separator_iterator.item_separator.join(
-                    prefix_separator_iterator.item_separator.join(item_pair)
-                    for item_pair in in_data_transformed.items()
+                next(prefix_separator_iterator) +
+                var_name_piece + value_pair_equals +
+                prefix_separator_iterator.item_separator.join(
+                    prefix_separator_iterator.item_separator.join(
+                        item_pair
+                    ) for item_pair in in_data_transformed.items()
                 )
             )
         # exploded
         return next(prefix_separator_iterator) + next(prefix_separator_iterator).join(
-            [key + "=" + val for key, val in in_data_transformed.items()]
+            [key + '=' + val for key, val in in_data_transformed.items()]
         )
 
     @classmethod
     def _ref6570_expansion(
         cls,
         variable_name: str,
         in_data: typing.Any,
         explode: bool,
         percent_encode: bool,
-        prefix_separator_iterator: PrefixSeparatorIterator,
+        prefix_separator_iterator: PrefixSeparatorIterator
     ) -> str:
         """
         Separator is for separate variables like dict with explode true, not for array item separation
         """
-        named_parameter_expansion = prefix_separator_iterator.separator in {"&", ";"}
-        var_name_piece = variable_name if named_parameter_expansion else ""
+        named_parameter_expansion = prefix_separator_iterator.separator in {'&', ';'}
+        var_name_piece = variable_name if named_parameter_expansion else ''
         if type(in_data) in {str, float, int}:
             return cls.__ref6570_str_float_int_expansion(
                 variable_name,
                 in_data,
                 explode,
                 percent_encode,
                 prefix_separator_iterator,
                 var_name_piece,
-                named_parameter_expansion,
+                named_parameter_expansion
             )
         elif isinstance(in_data, none_type):
             # ignored by the expansion process https://datatracker.ietf.org/doc/html/rfc6570#section-3.2.1
             return ""
         elif isinstance(in_data, list):
             return cls.__ref6570_list_expansion(
                 variable_name,
                 in_data,
                 explode,
                 percent_encode,
                 prefix_separator_iterator,
                 var_name_piece,
-                named_parameter_expansion,
+                named_parameter_expansion
             )
         elif isinstance(in_data, dict):
             return cls.__ref6570_dict_expansion(
                 variable_name,
                 in_data,
                 explode,
                 percent_encode,
                 prefix_separator_iterator,
                 var_name_piece,
-                named_parameter_expansion,
+                named_parameter_expansion
             )
         # bool, bytes, etc
-        raise ApiValueError(
-            "Unable to generate a ref6570 representation of {}".format(in_data)
-        )
+        raise ApiValueError('Unable to generate a ref6570 representation of {}'.format(in_data))
 
 
 class StyleFormSerializer(ParameterSerializerBase):
     @classmethod
     def _get_default_explode(cls, style: ParameterStyle) -> bool:
         if style is ParameterStyle.FORM:
             return True
@@ -308,54 +290,54 @@
 
     def _serialize_form(
         self,
         in_data: typing.Union[None, int, float, str, bool, dict, list],
         name: str,
         explode: bool,
         percent_encode: bool,
-        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator] = None,
+        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator] = None
     ) -> str:
         if prefix_separator_iterator is None:
-            prefix_separator_iterator = PrefixSeparatorIterator("", "&")
+            prefix_separator_iterator = PrefixSeparatorIterator('', '&')
         return self._ref6570_expansion(
             variable_name=name,
             in_data=in_data,
             explode=explode,
             percent_encode=percent_encode,
-            prefix_separator_iterator=prefix_separator_iterator,
+            prefix_separator_iterator=prefix_separator_iterator
         )
 
 
 class StyleSimpleSerializer(ParameterSerializerBase):
+
     def _serialize_simple(
         self,
         in_data: typing.Union[None, int, float, str, bool, dict, list],
         name: str,
         explode: bool,
-        percent_encode: bool,
+        percent_encode: bool
     ) -> str:
-        prefix_separator_iterator = PrefixSeparatorIterator("", ",")
+        prefix_separator_iterator = PrefixSeparatorIterator('', ',')
         return self._ref6570_expansion(
             variable_name=name,
             in_data=in_data,
             explode=explode,
             percent_encode=percent_encode,
-            prefix_separator_iterator=prefix_separator_iterator,
+            prefix_separator_iterator=prefix_separator_iterator
         )
 
 
 class JSONDetector:
     """
     Works for:
     application/json
     application/json; charset=UTF-8
     application/json-patch+json
     application/geo+json
     """
-
     __json_content_type_pattern = re.compile("application/[^+]*[+]?(json);?.*")
 
     @classmethod
     def _content_type_is_json(cls, content_type: str) -> bool:
         if cls.__json_content_type_pattern.match(content_type):
             return True
         return False
@@ -383,156 +365,137 @@
     }
     __in_type_to_default_style = {
         ParameterInType.QUERY: ParameterStyle.FORM,
         ParameterInType.PATH: ParameterStyle.SIMPLE,
         ParameterInType.HEADER: ParameterStyle.SIMPLE,
         ParameterInType.COOKIE: ParameterStyle.FORM,
     }
-    __disallowed_header_names = {"Accept", "Content-Type", "Authorization"}
+    __disallowed_header_names = {'Accept', 'Content-Type', 'Authorization'}
     _json_encoder = JSONEncoder()
 
     @classmethod
-    def __verify_style_to_in_type(
-        cls, style: typing.Optional[ParameterStyle], in_type: ParameterInType
-    ):
+    def __verify_style_to_in_type(cls, style: typing.Optional[ParameterStyle], in_type: ParameterInType):
         if style is None:
             return
         in_type_set = cls.__style_to_in_type[style]
         if in_type not in in_type_set:
             raise ValueError(
-                "Invalid style and in_type combination. For style={} only in_type={} are allowed".format(
+                'Invalid style and in_type combination. For style={} only in_type={} are allowed'.format(
                     style, in_type_set
                 )
             )
 
     def __init__(
         self,
         name: str,
         in_type: ParameterInType,
         required: bool = False,
         style: typing.Optional[ParameterStyle] = None,
         explode: bool = False,
         allow_reserved: typing.Optional[bool] = None,
         schema: typing.Optional[typing.Type[Schema]] = None,
-        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None,
+        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None
     ):
         if schema is None and content is None:
-            raise ValueError("Value missing; Pass in either schema or content")
+            raise ValueError('Value missing; Pass in either schema or content')
         if schema and content:
-            raise ValueError(
-                "Too many values provided. Both schema and content were provided. Only one may be input"
-            )
+            raise ValueError('Too many values provided. Both schema and content were provided. Only one may be input')
         if name in self.__disallowed_header_names and in_type is ParameterInType.HEADER:
-            raise ValueError(
-                "Invalid name, name may not be one of {}".format(
-                    self.__disallowed_header_names
-                )
-            )
+            raise ValueError('Invalid name, name may not be one of {}'.format(self.__disallowed_header_names))
         self.__verify_style_to_in_type(style, in_type)
         if content is None and style is None:
             style = self.__in_type_to_default_style[in_type]
-        if (
-            content is not None
-            and in_type in self.__in_type_to_default_style
-            and len(content) != 1
-        ):
-            raise ValueError("Invalid content length, content length must equal 1")
+        if content is not None and in_type in self.__in_type_to_default_style and len(content) != 1:
+            raise ValueError('Invalid content length, content length must equal 1')
         self.in_type = in_type
         self.name = name
         self.required = required
         self.style = style
         self.explode = explode
         self.allow_reserved = allow_reserved
         self.schema = schema
         self.content = content
 
     def _serialize_json(
         self,
         in_data: typing.Union[None, int, float, str, bool, dict, list],
-        eliminate_whitespace: bool = False,
+        eliminate_whitespace: bool = False
     ) -> str:
         if eliminate_whitespace:
             return json.dumps(in_data, separators=self._json_encoder.compact_separators)
         return json.dumps(in_data)
 
 
 class PathParameter(ParameterBase, StyleSimpleSerializer):
+
     def __init__(
         self,
         name: str,
         required: bool = False,
         style: typing.Optional[ParameterStyle] = None,
         explode: bool = False,
         allow_reserved: typing.Optional[bool] = None,
         schema: typing.Optional[typing.Type[Schema]] = None,
-        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None,
+        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None
     ):
         super().__init__(
             name,
             in_type=ParameterInType.PATH,
             required=required,
             style=style,
             explode=explode,
             allow_reserved=allow_reserved,
             schema=schema,
-            content=content,
+            content=content
         )
 
     def __serialize_label(
-        self, in_data: typing.Union[None, int, float, str, bool, dict, list]
+        self,
+        in_data: typing.Union[None, int, float, str, bool, dict, list]
     ) -> typing.Dict[str, str]:
-        prefix_separator_iterator = PrefixSeparatorIterator(".", ".")
+        prefix_separator_iterator = PrefixSeparatorIterator('.', '.')
         value = self._ref6570_expansion(
             variable_name=self.name,
             in_data=in_data,
             explode=self.explode,
             percent_encode=True,
-            prefix_separator_iterator=prefix_separator_iterator,
+            prefix_separator_iterator=prefix_separator_iterator
         )
         return self._to_dict(self.name, value)
 
     def __serialize_matrix(
-        self, in_data: typing.Union[None, int, float, str, bool, dict, list]
+        self,
+        in_data: typing.Union[None, int, float, str, bool, dict, list]
     ) -> typing.Dict[str, str]:
-        prefix_separator_iterator = PrefixSeparatorIterator(";", ";")
+        prefix_separator_iterator = PrefixSeparatorIterator(';', ';')
         value = self._ref6570_expansion(
             variable_name=self.name,
             in_data=in_data,
             explode=self.explode,
             percent_encode=True,
-            prefix_separator_iterator=prefix_separator_iterator,
+            prefix_separator_iterator=prefix_separator_iterator
         )
         return self._to_dict(self.name, value)
 
     def __serialize_simple(
         self,
         in_data: typing.Union[None, int, float, str, bool, dict, list],
     ) -> typing.Dict[str, str]:
         value = self._serialize_simple(
-            in_data=in_data, name=self.name, explode=self.explode, percent_encode=True
+            in_data=in_data,
+            name=self.name,
+            explode=self.explode,
+            percent_encode=True
         )
         return self._to_dict(self.name, value)
 
     def serialize(
         self,
         in_data: typing.Union[
-            Schema,
-            Decimal,
-            int,
-            float,
-            str,
-            date,
-            datetime,
-            None,
-            bool,
-            list,
-            tuple,
-            dict,
-            frozendict.frozendict,
-        ],
+            Schema, Decimal, int, float, str, date, datetime, None, bool, list, tuple, dict, frozendict.frozendict]
     ) -> typing.Dict[str, str]:
         if self.schema:
             cast_in_data = self.schema(in_data)
             cast_in_data = self._json_encoder.default(cast_in_data)
             """
             simple -> path
                 path:
@@ -552,120 +515,104 @@
         # self.content will be length one
         for content_type, schema in self.content.items():
             cast_in_data = schema(in_data)
             cast_in_data = self._json_encoder.default(cast_in_data)
             if self._content_type_is_json(content_type):
                 value = self._serialize_json(cast_in_data)
                 return self._to_dict(self.name, value)
-            raise NotImplementedError(
-                "Serialization of {} has not yet been implemented".format(content_type)
-            )
+            raise NotImplementedError('Serialization of {} has not yet been implemented'.format(content_type))
 
 
 class QueryParameter(ParameterBase, StyleFormSerializer):
+
     def __init__(
         self,
         name: str,
         required: bool = False,
         style: typing.Optional[ParameterStyle] = None,
         explode: typing.Optional[bool] = None,
         allow_reserved: typing.Optional[bool] = None,
         schema: typing.Optional[typing.Type[Schema]] = None,
-        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None,
+        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None
     ):
         used_style = ParameterStyle.FORM if style is None else style
-        used_explode = (
-            self._get_default_explode(used_style) if explode is None else explode
-        )
+        used_explode = self._get_default_explode(used_style) if explode is None else explode
 
         super().__init__(
             name,
             in_type=ParameterInType.QUERY,
             required=required,
             style=used_style,
             explode=used_explode,
             allow_reserved=allow_reserved,
             schema=schema,
-            content=content,
+            content=content
         )
 
     def __serialize_space_delimited(
         self,
         in_data: typing.Union[None, int, float, str, bool, dict, list],
-        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator],
+        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator]
     ) -> typing.Dict[str, str]:
         if prefix_separator_iterator is None:
             prefix_separator_iterator = self.get_prefix_separator_iterator()
         value = self._ref6570_expansion(
             variable_name=self.name,
             in_data=in_data,
             explode=self.explode,
             percent_encode=True,
-            prefix_separator_iterator=prefix_separator_iterator,
+            prefix_separator_iterator=prefix_separator_iterator
         )
         return self._to_dict(self.name, value)
 
     def __serialize_pipe_delimited(
         self,
         in_data: typing.Union[None, int, float, str, bool, dict, list],
-        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator],
+        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator]
     ) -> typing.Dict[str, str]:
         if prefix_separator_iterator is None:
             prefix_separator_iterator = self.get_prefix_separator_iterator()
         value = self._ref6570_expansion(
             variable_name=self.name,
             in_data=in_data,
             explode=self.explode,
             percent_encode=True,
-            prefix_separator_iterator=prefix_separator_iterator,
+            prefix_separator_iterator=prefix_separator_iterator
         )
         return self._to_dict(self.name, value)
 
     def __serialize_form(
         self,
         in_data: typing.Union[None, int, float, str, bool, dict, list],
-        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator],
+        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator]
     ) -> typing.Dict[str, str]:
         if prefix_separator_iterator is None:
             prefix_separator_iterator = self.get_prefix_separator_iterator()
         value = self._serialize_form(
             in_data,
             name=self.name,
             explode=self.explode,
             percent_encode=True,
-            prefix_separator_iterator=prefix_separator_iterator,
+            prefix_separator_iterator=prefix_separator_iterator
         )
         return self._to_dict(self.name, value)
 
     def get_prefix_separator_iterator(self) -> typing.Optional[PrefixSeparatorIterator]:
         if self.style is ParameterStyle.FORM:
-            return PrefixSeparatorIterator("?", "&")
+            return PrefixSeparatorIterator('?', '&')
         elif self.style is ParameterStyle.SPACE_DELIMITED:
-            return PrefixSeparatorIterator("", "%20")
+            return PrefixSeparatorIterator('', '%20')
         elif self.style is ParameterStyle.PIPE_DELIMITED:
-            return PrefixSeparatorIterator("", "|")
+            return PrefixSeparatorIterator('', '|')
 
     def serialize(
         self,
         in_data: typing.Union[
-            Schema,
-            Decimal,
-            int,
-            float,
-            str,
-            date,
-            datetime,
-            None,
-            bool,
-            list,
-            tuple,
-            dict,
-            frozendict.frozendict,
-        ],
-        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator] = None,
+            Schema, Decimal, int, float, str, date, datetime, None, bool, list, tuple, dict, frozendict.frozendict],
+        prefix_separator_iterator: typing.Optional[PrefixSeparatorIterator] = None
     ) -> typing.Dict[str, str]:
         if self.schema:
             cast_in_data = self.schema(in_data)
             cast_in_data = self._json_encoder.default(cast_in_data)
             """
             form -> query
                 query:
@@ -678,90 +625,64 @@
                 returns fields
             deepObject -> query, https://github.com/OAI/OpenAPI-Specification/issues/1706
                 returns fields
             """
             if self.style:
                 # TODO update query ones to omit setting values when [] {} or None is input
                 if self.style is ParameterStyle.FORM:
-                    return self.__serialize_form(
-                        cast_in_data, prefix_separator_iterator
-                    )
+                    return self.__serialize_form(cast_in_data, prefix_separator_iterator)
                 elif self.style is ParameterStyle.SPACE_DELIMITED:
-                    return self.__serialize_space_delimited(
-                        cast_in_data, prefix_separator_iterator
-                    )
+                    return self.__serialize_space_delimited(cast_in_data, prefix_separator_iterator)
                 elif self.style is ParameterStyle.PIPE_DELIMITED:
-                    return self.__serialize_pipe_delimited(
-                        cast_in_data, prefix_separator_iterator
-                    )
+                    return self.__serialize_pipe_delimited(cast_in_data, prefix_separator_iterator)
         # self.content will be length one
         if prefix_separator_iterator is None:
             prefix_separator_iterator = self.get_prefix_separator_iterator()
         for content_type, schema in self.content.items():
             cast_in_data = schema(in_data)
             cast_in_data = self._json_encoder.default(cast_in_data)
             if self._content_type_is_json(content_type):
                 value = self._serialize_json(cast_in_data, eliminate_whitespace=True)
                 return self._to_dict(
                     self.name,
-                    next(prefix_separator_iterator) + self.name + "=" + quote(value),
+                    next(prefix_separator_iterator) + self.name + '=' + quote(value)
                 )
-            raise NotImplementedError(
-                "Serialization of {} has not yet been implemented".format(content_type)
-            )
+            raise NotImplementedError('Serialization of {} has not yet been implemented'.format(content_type))
 
 
 class CookieParameter(ParameterBase, StyleFormSerializer):
+
     def __init__(
         self,
         name: str,
         required: bool = False,
         style: typing.Optional[ParameterStyle] = None,
         explode: typing.Optional[bool] = None,
         allow_reserved: typing.Optional[bool] = None,
         schema: typing.Optional[typing.Type[Schema]] = None,
-        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None,
+        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None
     ):
-        used_style = (
-            ParameterStyle.FORM
-            if style is None and content is None and schema
-            else style
-        )
-        used_explode = (
-            self._get_default_explode(used_style) if explode is None else explode
-        )
+        used_style = ParameterStyle.FORM if style is None and content is None and schema else style
+        used_explode = self._get_default_explode(used_style) if explode is None else explode
 
         super().__init__(
             name,
             in_type=ParameterInType.COOKIE,
             required=required,
             style=used_style,
             explode=used_explode,
             allow_reserved=allow_reserved,
             schema=schema,
-            content=content,
+            content=content
         )
 
     def serialize(
         self,
         in_data: typing.Union[
-            Schema,
-            Decimal,
-            int,
-            float,
-            str,
-            date,
-            datetime,
-            None,
-            bool,
-            list,
-            tuple,
-            dict,
-            frozendict.frozendict,
-        ],
+            Schema, Decimal, int, float, str, date, datetime, None, bool, list, tuple, dict, frozendict.frozendict]
     ) -> typing.Dict[str, str]:
         if self.schema:
             cast_in_data = self.schema(in_data)
             cast_in_data = self._json_encoder.default(cast_in_data)
             """
             form -> cookie
                 returns fields: tuple
@@ -772,103 +693,82 @@
                 or turn encoding on
                 """
                 value = self._serialize_form(
                     cast_in_data,
                     explode=self.explode,
                     name=self.name,
                     percent_encode=False,
-                    prefix_separator_iterator=PrefixSeparatorIterator("", "&"),
+                    prefix_separator_iterator=PrefixSeparatorIterator('', '&')
                 )
                 return self._to_dict(self.name, value)
         # self.content will be length one
         for content_type, schema in self.content.items():
             cast_in_data = schema(in_data)
             cast_in_data = self._json_encoder.default(cast_in_data)
             if self._content_type_is_json(content_type):
                 value = self._serialize_json(cast_in_data)
                 return self._to_dict(self.name, value)
-            raise NotImplementedError(
-                "Serialization of {} has not yet been implemented".format(content_type)
-            )
+            raise NotImplementedError('Serialization of {} has not yet been implemented'.format(content_type))
 
 
 class HeaderParameter(ParameterBase, StyleSimpleSerializer):
     def __init__(
         self,
         name: str,
         required: bool = False,
         style: typing.Optional[ParameterStyle] = None,
         explode: bool = False,
         allow_reserved: typing.Optional[bool] = None,
         schema: typing.Optional[typing.Type[Schema]] = None,
-        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None,
+        content: typing.Optional[typing.Dict[str, typing.Type[Schema]]] = None
     ):
         super().__init__(
             name,
             in_type=ParameterInType.HEADER,
             required=required,
             style=style,
             explode=explode,
             allow_reserved=allow_reserved,
             schema=schema,
-            content=content,
+            content=content
         )
 
     @staticmethod
-    def __to_headers(
-        in_data: typing.Tuple[typing.Tuple[str, str], ...]
-    ) -> HTTPHeaderDict:
+    def __to_headers(in_data: typing.Tuple[typing.Tuple[str, str], ...]) -> HTTPHeaderDict:
         data = tuple(t for t in in_data if t)
         headers = HTTPHeaderDict()
         if not data:
             return headers
         headers.extend(data)
         return headers
 
     def serialize(
         self,
         in_data: typing.Union[
-            Schema,
-            Decimal,
-            int,
-            float,
-            str,
-            date,
-            datetime,
-            None,
-            bool,
-            list,
-            tuple,
-            dict,
-            frozendict.frozendict,
-        ],
+            Schema, Decimal, int, float, str, date, datetime, None, bool, list, tuple, dict, frozendict.frozendict]
     ) -> HTTPHeaderDict:
         if self.schema:
             cast_in_data = self.schema(in_data)
             cast_in_data = self._json_encoder.default(cast_in_data)
             """
             simple -> header
                 headers: PoolManager needs a mapping, tuple is close
                     returns headers: dict
             """
             if self.style:
-                value = self._serialize_simple(
-                    cast_in_data, self.name, self.explode, False
-                )
+                value = self._serialize_simple(cast_in_data, self.name, self.explode, False)
                 return self.__to_headers(((self.name, value),))
         # self.content will be length one
         for content_type, schema in self.content.items():
             cast_in_data = schema(in_data)
             cast_in_data = self._json_encoder.default(cast_in_data)
             if self._content_type_is_json(content_type):
                 value = self._serialize_json(cast_in_data)
                 return self.__to_headers(((self.name, value),))
-            raise NotImplementedError(
-                "Serialization of {} has not yet been implemented".format(content_type)
-            )
+            raise NotImplementedError('Serialization of {} has not yet been implemented'.format(content_type))
 
 
 class Encoding:
     def __init__(
         self,
         content_type: str,
         headers: typing.Optional[typing.Dict[str, HeaderParameter]] = None,
@@ -889,30 +789,29 @@
     Used to store request and response body schema information
     encoding:
         A map between a property name and its encoding information.
         The key, being the property name, MUST exist in the schema as a property.
         The encoding object SHALL only apply to requestBody objects when the media type is
         multipart or application/x-www-form-urlencoded.
     """
-
     schema: typing.Optional[typing.Type[Schema]] = None
     encoding: typing.Optional[typing.Dict[str, Encoding]] = None
 
 
 @dataclass
 class ApiResponse:
     response: urllib3.HTTPResponse
     body: typing.Union[Unset, Schema] = unset
     headers: typing.Union[Unset, typing.Dict[str, Schema]] = unset
 
     def __init__(
         self,
         response: urllib3.HTTPResponse,
         body: typing.Union[Unset, Schema] = unset,
-        headers: typing.Union[Unset, typing.Dict[str, Schema]] = unset,
+        headers: typing.Union[Unset, typing.Dict[str, Schema]] = unset
     ):
         """
         pycharm needs this to prevent 'Unexpected argument' warnings
         """
         self.response = response
         self.body = body
         self.headers = headers
@@ -932,44 +831,38 @@
         self,
         response_cls: typing.Type[ApiResponse] = ApiResponse,
         content: typing.Optional[typing.Dict[str, MediaType]] = None,
         headers: typing.Optional[typing.List[HeaderParameter]] = None,
     ):
         self.headers = headers
         if content is not None and len(content) == 0:
-            raise ValueError(
-                "Invalid value for content, the content dict must have >= 1 entry"
-            )
+            raise ValueError('Invalid value for content, the content dict must have >= 1 entry')
         self.content = content
         self.response_cls = response_cls
 
     @staticmethod
     def __deserialize_json(response: urllib3.HTTPResponse) -> typing.Any:
         # python must be >= 3.9 so we can pass in bytes into json.loads
         return json.loads(response.data)
 
     @staticmethod
-    def __file_name_from_response_url(
-        response_url: typing.Optional[str],
-    ) -> typing.Optional[str]:
+    def __file_name_from_response_url(response_url: typing.Optional[str]) -> typing.Optional[str]:
         if response_url is None:
             return None
         url_path = urlparse(response_url).path
         if url_path:
             path_basename = os.path.basename(url_path)
             if path_basename:
                 _filename, ext = os.path.splitext(path_basename)
                 if ext:
                     return path_basename
         return None
 
     @classmethod
-    def __file_name_from_content_disposition(
-        cls, content_disposition: typing.Optional[str]
-    ) -> typing.Optional[str]:
+    def __file_name_from_content_disposition(cls, content_disposition: typing.Optional[str]) -> typing.Optional[str]:
         if content_disposition is None:
             return None
         match = cls.__filename_content_disposition_pattern.search(content_disposition)
         if not match:
             return None
         return match.group(1)
 
@@ -979,55 +872,54 @@
         """
         urllib3 use cases:
         1. when preload_content=True (stream=False) then supports_chunked_reads is False and bytes are returned
         2. when preload_content=False (stream=True) then supports_chunked_reads is True and
             a file will be written and returned
         """
         if response.supports_chunked_reads():
-            file_name = self.__file_name_from_content_disposition(
-                response.headers.get("content-disposition")
-            ) or self.__file_name_from_response_url(response.geturl())
+            file_name = (
+                self.__file_name_from_content_disposition(response.headers.get('content-disposition'))
+                or self.__file_name_from_response_url(response.geturl())
+            )
 
             if file_name is None:
                 _fd, path = tempfile.mkstemp()
             else:
                 path = os.path.join(tempfile.gettempdir(), file_name)
 
-            with open(path, "wb") as new_file:
+            with open(path, 'wb') as new_file:
                 chunk_size = 1024
                 while True:
                     data = response.read(chunk_size)
                     if not data:
                         break
                     new_file.write(data)
             # release_conn is needed for streaming connections only
             response.release_conn()
-            new_file = open(path, "rb")
+            new_file = open(path, 'rb')
             return new_file
         else:
             return response.data
 
     @staticmethod
     def __deserialize_multipart_form_data(
-        response: urllib3.HTTPResponse,
+        response: urllib3.HTTPResponse
     ) -> typing.Dict[str, typing.Any]:
         msg = email.message_from_bytes(response.data)
         return {
             part.get_param("name", header="Content-Disposition"): part.get_payload(
                 decode=True
             ).decode(part.get_content_charset())
             if part.get_content_charset()
             else part.get_payload()
             for part in msg.get_payload()
         }
 
-    def deserialize(
-        self, response: urllib3.HTTPResponse, configuration: Configuration
-    ) -> ApiResponse:
-        content_type = response.getheader("content-type")
+    def deserialize(self, response: urllib3.HTTPResponse, configuration: Configuration) -> ApiResponse:
+        content_type = response.getheader('content-type')
         deserialized_body = unset
         streamed = response.supports_chunked_reads()
 
         deserialized_headers = unset
         if self.headers is not None:
             # TODO add header deserialiation here
             pass
@@ -1038,38 +930,37 @@
                     f"Invalid content_type returned. Content_type='{content_type}' was returned "
                     f"when only {str(set(self.content))} are defined for status_code={str(response.status)}"
                 )
             body_schema = self.content[content_type].schema
             if body_schema is None:
                 # some specs do not define response content media type schemas
                 return self.response_cls(
-                    response=response, headers=deserialized_headers, body=unset
+                    response=response,
+                    headers=deserialized_headers,
+                    body=unset
                 )
 
             if self._content_type_is_json(content_type):
                 body_data = self.__deserialize_json(response)
-            elif content_type == "application/octet-stream":
+            elif content_type == 'application/octet-stream':
                 body_data = self.__deserialize_application_octet_stream(response)
-            elif content_type.startswith("multipart/form-data"):
+            elif content_type.startswith('multipart/form-data'):
                 body_data = self.__deserialize_multipart_form_data(response)
-                content_type = "multipart/form-data"
+                content_type = 'multipart/form-data'
             else:
-                raise NotImplementedError(
-                    "Deserialization of {} has not yet been implemented".format(
-                        content_type
-                    )
-                )
+                raise NotImplementedError('Deserialization of {} has not yet been implemented'.format(content_type))
             deserialized_body = body_schema.from_openapi_data_oapg(
-                body_data, _configuration=configuration
-            )
+                body_data, _configuration=configuration)
         elif streamed:
             response.release_conn()
 
         return self.response_cls(
-            response=response, headers=deserialized_headers, body=deserialized_body
+            response=response,
+            headers=deserialized_headers,
+            body=deserialized_body
         )
 
 
 class ApiClient:
     """Generic API client for OpenAPI client library builds.
 
     OpenAPI generic API client. This client handles the client-
@@ -1095,61 +986,61 @@
 
     def __init__(
         self,
         configuration: typing.Optional[Configuration] = None,
         header_name: typing.Optional[str] = None,
         header_value: typing.Optional[str] = None,
         cookie: typing.Optional[str] = None,
-        pool_threads: int = 1,
+        pool_threads: int = 1
     ):
         if configuration is None:
             configuration = Configuration()
         self.configuration = configuration
         self.pool_threads = pool_threads
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = "OpenAPI-Generator/1.0.0/python"
+        self.user_agent = 'OpenAPI-Generator/1.0.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
     def close(self):
         if self._pool:
             self._pool.close()
             self._pool.join()
             self._pool = None
-            if hasattr(atexit, "unregister"):
+            if hasattr(atexit, 'unregister'):
                 atexit.unregister(self.close)
 
     @property
     def pool(self):
         """Create thread pool on first request
-        avoids instantiating unused threadpool for blocking clients.
+         avoids instantiating unused threadpool for blocking clients.
         """
         if self._pool is None:
             atexit.register(self.close)
             self._pool = ThreadPool(self.pool_threads)
         return self._pool
 
     @property
     def user_agent(self):
         """User agent for this API client"""
-        return self.default_headers["User-Agent"]
+        return self.default_headers['User-Agent']
 
     @user_agent.setter
     def user_agent(self, value):
-        self.default_headers["User-Agent"] = value
+        self.default_headers['User-Agent'] = value
 
     def set_default_header(self, header_name, header_value):
         self.default_headers[header_name] = header_value
 
     def __call_api(
         self,
         resource_path: str,
@@ -1158,23 +1049,23 @@
         body: typing.Optional[typing.Union[str, bytes]] = None,
         fields: typing.Optional[typing.Tuple[typing.Tuple[str, str], ...]] = None,
         auth_settings: typing.Optional[typing.List[str]] = None,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         host: typing.Optional[str] = None,
     ) -> urllib3.HTTPResponse:
+
         # header parameters
         used_headers = HTTPHeaderDict(self.default_headers)
         if self.cookie:
-            headers["Cookie"] = self.cookie
+            headers['Cookie'] = self.cookie
 
         # auth setting
-        self.update_params_for_auth(
-            used_headers, auth_settings, resource_path, method, body
-        )
+        self.update_params_for_auth(used_headers,
+                                    auth_settings, resource_path, method, body)
 
         # must happen after cookie setting and auth setting in case user is overriding those
         if headers:
             used_headers.update(headers)
 
         # request url
         if host is None:
@@ -1264,85 +1155,80 @@
                 body,
                 json,
                 fields,
                 auth_settings,
                 stream,
                 timeout,
                 host,
-            ),
+            )
         )
 
     def request(
         self,
         method: str,
         url: str,
         headers: typing.Optional[HTTPHeaderDict] = None,
         fields: typing.Optional[typing.Tuple[typing.Tuple[str, str], ...]] = None,
         body: typing.Optional[typing.Union[str, bytes]] = None,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> urllib3.HTTPResponse:
         """Makes the HTTP request using RESTClient."""
         if method == "GET":
-            return self.rest_client.GET(
-                url, stream=stream, timeout=timeout, headers=headers
-            )
+            return self.rest_client.GET(url,
+                                        stream=stream,
+                                        timeout=timeout,
+                                        headers=headers)
         elif method == "HEAD":
-            return self.rest_client.HEAD(
-                url, stream=stream, timeout=timeout, headers=headers
-            )
+            return self.rest_client.HEAD(url,
+                                         stream=stream,
+                                         timeout=timeout,
+                                         headers=headers)
         elif method == "OPTIONS":
-            return self.rest_client.OPTIONS(
-                url,
-                headers=headers,
-                fields=fields,
-                stream=stream,
-                timeout=timeout,
-                body=body,
-            )
+            return self.rest_client.OPTIONS(url,
+                                            headers=headers,
+                                            fields=fields,
+                                            stream=stream,
+                                            timeout=timeout,
+                                            body=body)
         elif method == "POST":
-            return self.rest_client.POST(
-                url,
-                headers=headers,
-                fields=fields,
-                stream=stream,
-                timeout=timeout,
-                body=body,
-            )
+            return self.rest_client.POST(url,
+                                         headers=headers,
+                                         fields=fields,
+                                         stream=stream,
+                                         timeout=timeout,
+                                         body=body)
         elif method == "PUT":
-            return self.rest_client.PUT(
-                url,
-                headers=headers,
-                fields=fields,
-                stream=stream,
-                timeout=timeout,
-                body=body,
-            )
+            return self.rest_client.PUT(url,
+                                        headers=headers,
+                                        fields=fields,
+                                        stream=stream,
+                                        timeout=timeout,
+                                        body=body)
         elif method == "PATCH":
-            return self.rest_client.PATCH(
-                url,
-                headers=headers,
-                fields=fields,
-                stream=stream,
-                timeout=timeout,
-                body=body,
-            )
+            return self.rest_client.PATCH(url,
+                                          headers=headers,
+                                          fields=fields,
+                                          stream=stream,
+                                          timeout=timeout,
+                                          body=body)
         elif method == "DELETE":
-            return self.rest_client.DELETE(
-                url, headers=headers, stream=stream, timeout=timeout, body=body
-            )
+            return self.rest_client.DELETE(url,
+                                           headers=headers,
+                                           stream=stream,
+                                           timeout=timeout,
+                                           body=body)
         else:
             raise ApiValueError(
                 "http method must be `GET`, `HEAD`, `OPTIONS`,"
                 " `POST`, `PATCH`, `PUT` or `DELETE`."
             )
 
-    def update_params_for_auth(
-        self, headers, auth_settings, resource_path, method, body
-    ):
+    def update_params_for_auth(self, headers, auth_settings,
+                               resource_path, method, body):
         """Updates header and query params based on authentication setting.
 
         :param headers: Header parameters dict to be updated.
         :param auth_settings: Authentication setting identifiers list.
         :param resource_path: A string representation of the HTTP request resource path.
         :param method: A string representation of the HTTP request method.
         :param body: A object representing the body of the HTTP request.
@@ -1351,28 +1237,28 @@
         if not auth_settings:
             return
 
         for auth in auth_settings:
             auth_setting = self.configuration.auth_settings().get(auth)
             if not auth_setting:
                 continue
-            if auth_setting["in"] == "cookie":
-                headers.add("Cookie", auth_setting["value"])
-            elif auth_setting["in"] == "header":
-                if auth_setting["type"] != "http-signature":
-                    headers.add(auth_setting["key"], auth_setting["value"])
-            elif auth_setting["in"] == "query":
-                """TODO implement auth in query
+            if auth_setting['in'] == 'cookie':
+                headers.add('Cookie', auth_setting['value'])
+            elif auth_setting['in'] == 'header':
+                if auth_setting['type'] != 'http-signature':
+                    headers.add(auth_setting['key'], auth_setting['value'])
+            elif auth_setting['in'] == 'query':
+                """ TODO implement auth in query
                 need to pass in prefix_separator_iterator
                 and need to output resource_path with query params added
                 """
                 raise ApiValueError("Auth in query not yet implemented")
             else:
                 raise ApiValueError(
-                    "Authentication token must be in `query` or `header`"
+                    'Authentication token must be in `query` or `header`'
                 )
 
 
 class Api:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
@@ -1381,18 +1267,15 @@
 
     def __init__(self, api_client: typing.Optional[ApiClient] = None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     @staticmethod
-    def _verify_typed_dict_inputs_oapg(
-        cls: typing.Type[typing_extensions.TypedDict],
-        data: typing.Dict[str, typing.Any],
-    ):
+    def _verify_typed_dict_inputs_oapg(cls: typing.Type[typing_extensions.TypedDict], data: typing.Dict[str, typing.Any]):
         """
         Ensures that:
         - required keys are present
         - additional properties are not input
         - value stored under required keys do not have the value unset
         Note: detailed value checking is done in schema classes
         """
@@ -1403,46 +1286,42 @@
                 missing_required_keys.append(required_key)
                 continue
             value = data[required_key]
             if value is unset:
                 required_keys_with_unset_values.append(required_key)
         if missing_required_keys:
             raise ApiTypeError(
-                "{} missing {} required arguments: {}".format(
+                '{} missing {} required arguments: {}'.format(
                     cls.__name__, len(missing_required_keys), missing_required_keys
-                )
-            )
+                 )
+             )
         if required_keys_with_unset_values:
             raise ApiValueError(
-                "{} contains invalid unset values for {} required keys: {}".format(
-                    cls.__name__,
-                    len(required_keys_with_unset_values),
-                    required_keys_with_unset_values,
+                '{} contains invalid unset values for {} required keys: {}'.format(
+                    cls.__name__, len(required_keys_with_unset_values), required_keys_with_unset_values
                 )
             )
 
         disallowed_additional_keys = []
         for key in data:
             if key in cls.__required_keys__ or key in cls.__optional_keys__:
                 continue
             disallowed_additional_keys.append(key)
         if disallowed_additional_keys:
             raise ApiTypeError(
-                "{} got {} unexpected keyword arguments: {}".format(
-                    cls.__name__,
-                    len(disallowed_additional_keys),
-                    disallowed_additional_keys,
+                '{} got {} unexpected keyword arguments: {}'.format(
+                    cls.__name__, len(disallowed_additional_keys), disallowed_additional_keys
                 )
             )
 
     def _get_host_oapg(
         self,
         operation_id: str,
         servers: typing.Tuple[typing.Dict[str, str], ...] = tuple(),
-        host_index: typing.Optional[int] = None,
+        host_index: typing.Optional[int] = None
     ) -> typing.Optional[str]:
         configuration = self.api_client.configuration
         try:
             if host_index is None:
                 index = configuration.server_operation_index.get(
                     operation_id, configuration.server_index
                 )
@@ -1453,15 +1332,16 @@
             )
             host = configuration.get_host_from_settings(
                 index, variables=server_variables, servers=servers
             )
         except IndexError:
             if servers:
                 raise ApiValueError(
-                    "Invalid host index. Must be 0 <= index < %s" % len(servers)
+                    "Invalid host index. Must be 0 <= index < %s" %
+                    len(servers)
                 )
             host = None
         return host
 
 
 class SerializedRequestBody(typing_extensions.TypedDict, total=False):
     body: typing.Union[str, bytes]
@@ -1469,80 +1349,74 @@
 
 
 class RequestBody(StyleFormSerializer, JSONDetector):
     """
     A request body parameter
     content: content_type to MediaType Schema info
     """
-
     __json_encoder = JSONEncoder()
 
     def __init__(
         self,
         content: typing.Dict[str, MediaType],
         required: bool = False,
     ):
         self.required = required
         if len(content) == 0:
-            raise ValueError(
-                "Invalid value for content, the content dict must have >= 1 entry"
-            )
+            raise ValueError('Invalid value for content, the content dict must have >= 1 entry')
         self.content = content
 
-    def __serialize_json(self, in_data: typing.Any) -> typing.Dict[str, bytes]:
+    def __serialize_json(
+        self,
+        in_data: typing.Any
+    ) -> typing.Dict[str, bytes]:
         in_data = self.__json_encoder.default(in_data)
-        json_str = json.dumps(
-            in_data, separators=(",", ":"), ensure_ascii=False
-        ).encode("utf-8")
+        json_str = json.dumps(in_data, separators=(",", ":"), ensure_ascii=False).encode(
+            "utf-8"
+        )
         return dict(body=json_str)
 
     @staticmethod
     def __serialize_text_plain(in_data: typing.Any) -> typing.Dict[str, str]:
         if isinstance(in_data, frozendict.frozendict):
-            raise ValueError(
-                "Unable to serialize type frozendict.frozendict to text/plain"
-            )
+            raise ValueError('Unable to serialize type frozendict.frozendict to text/plain')
         elif isinstance(in_data, tuple):
-            raise ValueError("Unable to serialize type tuple to text/plain")
+            raise ValueError('Unable to serialize type tuple to text/plain')
         elif isinstance(in_data, NoneClass):
-            raise ValueError("Unable to serialize type NoneClass to text/plain")
+            raise ValueError('Unable to serialize type NoneClass to text/plain')
         elif isinstance(in_data, BoolClass):
-            raise ValueError("Unable to serialize type BoolClass to text/plain")
+            raise ValueError('Unable to serialize type BoolClass to text/plain')
         return dict(body=str(in_data))
 
     def __multipart_json_item(self, key: str, value: Schema) -> RequestField:
         json_value = self.__json_encoder.default(value)
         request_field = RequestField(name=key, data=json.dumps(json_value))
-        request_field.make_multipart(content_type="application/json")
+        request_field.make_multipart(content_type='application/json')
         return request_field
 
     def __multipart_form_item(self, key: str, value: Schema) -> RequestField:
         if isinstance(value, str):
             request_field = RequestField(name=key, data=str(value))
-            request_field.make_multipart(content_type="text/plain")
+            request_field.make_multipart(content_type='text/plain')
         elif isinstance(value, bytes):
             request_field = RequestField(name=key, data=value)
-            request_field.make_multipart(content_type="application/octet-stream")
+            request_field.make_multipart(content_type='application/octet-stream')
         elif isinstance(value, FileIO):
             # TODO use content.encoding to limit allowed content types if they are present
-            request_field = RequestField.from_tuples(
-                key, (os.path.basename(value.name), value.read())
-            )
+            request_field = RequestField.from_tuples(key, (os.path.basename(value.name), value.read()))
             value.close()
         else:
             request_field = self.__multipart_json_item(key=key, value=value)
         return request_field
 
     def __serialize_multipart_form_data(
         self, in_data: Schema
     ) -> typing.Dict[str, typing.Tuple[RequestField, ...]]:
         if not isinstance(in_data, frozendict.frozendict):
-            raise ValueError(
-                f"Unable to serialize {in_data} to multipart/form-data because it is not a dict of data"
-            )
+            raise ValueError(f'Unable to serialize {in_data} to multipart/form-data because it is not a dict of data')
         """
         In a multipart/form-data request body, each schema property, or each element of a schema array property,
         takes a section in the payload with an internal header as defined by RFC7578. The serialization strategy
         for each property of a multipart/form-data request body can be specified in an associated Encoding Object.
 
         When passing in multipart types, boundaries MAY be used to separate sections of the content being
         transferred – thus, the following default Content-Types are defined for multipart:
@@ -1566,17 +1440,15 @@
                     fields.append(request_field)
             else:
                 request_field = self.__multipart_form_item(key=key, value=value)
                 fields.append(request_field)
 
         return dict(fields=tuple(fields))
 
-    def __serialize_application_octet_stream(
-        self, in_data: BinarySchema
-    ) -> typing.Dict[str, bytes]:
+    def __serialize_application_octet_stream(self, in_data: BinarySchema) -> typing.Dict[str, bytes]:
         if isinstance(in_data, bytes):
             return dict(body=in_data)
         # FileIO type
         result = dict(body=in_data.read())
         in_data.close()
         return result
 
@@ -1584,20 +1456,17 @@
         self, in_data: typing.Any
     ) -> SerializedRequestBody:
         """
         POST submission of form data in body
         """
         if not isinstance(in_data, frozendict.frozendict):
             raise ValueError(
-                f"Unable to serialize {in_data} to application/x-www-form-urlencoded because it is not a dict of data"
-            )
+                f'Unable to serialize {in_data} to application/x-www-form-urlencoded because it is not a dict of data')
         cast_in_data = self.__json_encoder.default(in_data)
-        value = self._serialize_form(
-            cast_in_data, name="", explode=True, percent_encode=True
-        )
+        value = self._serialize_form(cast_in_data, name='', explode=True, percent_encode=True)
         return dict(body=value)
 
     def serialize(
         self, in_data: typing.Any, content_type: str
     ) -> SerializedRequestBody:
         """
         If a str is returned then the result will be assigned to data when making the request
@@ -1615,18 +1484,16 @@
             cast_in_data = media_type.schema(**in_data)
         else:
             cast_in_data = media_type.schema(in_data)
         # TODO check for and use encoding if it exists
         # and content_type is multipart or application/x-www-form-urlencoded
         if self._content_type_is_json(content_type):
             return self.__serialize_json(cast_in_data)
-        elif content_type == "text/plain":
+        elif content_type == 'text/plain':
             return self.__serialize_text_plain(cast_in_data)
-        elif content_type == "multipart/form-data":
+        elif content_type == 'multipart/form-data':
             return self.__serialize_multipart_form_data(cast_in_data)
-        elif content_type == "application/x-www-form-urlencoded":
+        elif content_type == 'application/x-www-form-urlencoded':
             return self.__serialize_application_x_www_form_data(cast_in_data)
-        elif content_type == "application/octet-stream":
+        elif content_type == 'application/octet-stream':
             return self.__serialize_application_octet_stream(cast_in_data)
-        raise NotImplementedError(
-            "Serialization has not yet been implemented for {}".format(content_type)
-        )
+        raise NotImplementedError('Serialization has not yet been implemented for {}'.format(content_type))
```

### Comparing `gentrace_py-0.7.4/gentrace/configuration.py` & `gentrace_py-0.8.0/gentrace/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,35 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.8
+    The version of the OpenAPI document: 0.4.13
     Generated by: https://openapi-generator.tech
 """
 
 import copy
 import logging
 import multiprocessing
 import sys
 from http import client as http_client
 
 import urllib3
 
 from gentrace.exceptions import ApiValueError
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
-    "multipleOf",
-    "maximum",
-    "exclusiveMaximum",
-    "minimum",
-    "exclusiveMinimum",
-    "maxLength",
-    "minLength",
-    "pattern",
-    "maxItems",
-    "minItems",
-    "uniqueItems",
-    "maxProperties",
-    "minProperties",
+    'multipleOf', 'maximum', 'exclusiveMaximum',
+    'minimum', 'exclusiveMinimum', 'maxLength',
+    'minLength', 'pattern', 'maxItems', 'minItems',
+    'uniqueItems', 'maxProperties', 'minProperties',
 }
 
-
 class Configuration(object):
     """NOTE: This class is auto generated by OpenAPI Generator
 
     Ref: https://openapi-generator.tech
     Do not edit the class manually.
 
     :param host: Base url
@@ -97,15 +87,16 @@
         discard_unknown_keys=False,
         disabled_client_side_validations="",
         server_index=None,
         server_variables=None,
         server_operation_index=None,
         server_operation_variables=None,
     ):
-        """Constructor"""
+        """Constructor
+        """
         self._base_path = "https://gentrace.ai/api/v1" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
         """Default server index
         """
@@ -119,15 +110,15 @@
         # Authentication Settings
         self.disabled_client_side_validations = disabled_client_side_validations
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("gentrace")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
-        self.logger_format = "%(asctime)s %(levelname)s %(message)s"
+        self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
         self.logger_file_handler = None
         """Log file handler
@@ -167,15 +158,15 @@
 
         self.proxy = None
         """Proxy URL
         """
         self.proxy_headers = None
         """Proxy headers
         """
-        self.safe_chars_for_path_param = ""
+        self.safe_chars_for_path_param = ''
         """Safe chars for path_param
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
         # Enable client side validation
         self.client_side_validation = True
@@ -184,30 +175,31 @@
         self.socket_options = None
 
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
-            if k not in ("logger", "logger_file_handler"):
+            if k not in ('logger', 'logger_file_handler'):
                 setattr(result, k, copy.deepcopy(v, memo))
         # shallow copy of loggers
         result.logger = copy.copy(self.logger)
         # use setters to configure loggers
         result.logger_file = self.logger_file
         result.debug = self.debug
         return result
 
     def __setattr__(self, name, value):
         object.__setattr__(self, name, value)
-        if name == "disabled_client_side_validations":
-            s = set(filter(None, value.split(",")))
+        if name == 'disabled_client_side_validations':
+            s = set(filter(None, value.split(',')))
             for v in s:
                 if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
-                    raise ApiValueError("Invalid keyword: '{0}''".format(v))
+                    raise ApiValueError(
+                        "Invalid keyword: '{0}''".format(v))
             self._disabled_client_side_validations = s
 
     @classmethod
     def set_default(cls, default):
         """Set default instance of configuration.
 
         It stores default configuration, which can be
@@ -321,17 +313,15 @@
 
         :param identifier: The identifier of apiKey.
         :param alias: The alternative identifier of apiKey.
         :return: The token for api key authentication.
         """
         if self.refresh_api_key_hook is not None:
             self.refresh_api_key_hook(self)
-        key = self.api_key.get(
-            identifier, self.api_key.get(alias) if alias is not None else None
-        )
+        key = self.api_key.get(identifier, self.api_key.get(alias) if alias is not None else None)
         if key:
             prefix = self.api_key_prefix.get(identifier)
             if prefix:
                 return "%s %s" % (prefix, key)
             else:
                 return key
 
@@ -342,55 +332,54 @@
         """
         username = ""
         if self.username is not None:
             username = self.username
         password = ""
         if self.password is not None:
             password = self.password
-        return urllib3.util.make_headers(basic_auth=username + ":" + password).get(
-            "authorization"
-        )
+        return urllib3.util.make_headers(
+            basic_auth=username + ':' + password
+        ).get('authorization')
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         auth = {}
         if self.access_token is not None:
-            auth["bearerAuth"] = {
-                "type": "bearer",
-                "in": "header",
-                "key": "Authorization",
-                "value": "Bearer " + self.access_token,
+            auth['bearerAuth'] = {
+                'type': 'bearer',
+                'in': 'header',
+                'key': 'Authorization',
+                'value': 'Bearer ' + self.access_token
             }
         return auth
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
-        return (
-            "Python SDK Debug Report:\n"
-            "OS: {env}\n"
-            "Python Version: {pyversion}\n"
-            "Version of the API: 0.4.8\n"
-            "SDK Package Version: 1.0.0".format(env=sys.platform, pyversion=sys.version)
-        )
+        return "Python SDK Debug Report:\n"\
+               "OS: {env}\n"\
+               "Python Version: {pyversion}\n"\
+               "Version of the API: 0.4.13\n"\
+               "SDK Package Version: 1.0.0".\
+               format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
-                "url": "https://gentrace.ai/api/v1",
-                "description": "No description provided",
+                'url': "https://gentrace.ai/api/v1",
+                'description': "No description provided",
             }
         ]
 
     def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
         :param variables: hash of variable and the corresponding value
@@ -404,40 +393,38 @@
         servers = self.get_host_settings() if servers is None else servers
 
         try:
             server = servers[index]
         except IndexError:
             raise ValueError(
                 "Invalid index {0} when selecting the host settings. "
-                "Must be less than {1}".format(index, len(servers))
-            )
+                "Must be less than {1}".format(index, len(servers)))
 
-        url = server["url"]
+        url = server['url']
 
         # go through variables and replace placeholders
-        for variable_name, variable in server.get("variables", {}).items():
-            used_value = variables.get(variable_name, variable["default_value"])
+        for variable_name, variable in server.get('variables', {}).items():
+            used_value = variables.get(
+                variable_name, variable['default_value'])
 
-            if "enum_values" in variable and used_value not in variable["enum_values"]:
+            if 'enum_values' in variable \
+                    and used_value not in variable['enum_values']:
                 raise ValueError(
                     "The variable `{0}` in the host URL has invalid value "
                     "{1}. Must be {2}.".format(
-                        variable_name, variables[variable_name], variable["enum_values"]
-                    )
-                )
+                        variable_name, variables[variable_name],
+                        variable['enum_values']))
 
             url = url.replace("{" + variable_name + "}", used_value)
 
         return url
 
     @property
     def host(self):
         """Return generated host."""
-        return self.get_host_from_settings(
-            self.server_index, variables=self.server_variables
-        )
+        return self.get_host_from_settings(self.server_index, variables=self.server_variables)
 
     @host.setter
     def host(self, value):
         """Fix base path."""
         self._base_path = value
         self.server_index = None
```

### Comparing `gentrace_py-0.7.4/gentrace/exceptions.py` & `gentrace_py-0.8.0/gentrace/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.8
+    The version of the OpenAPI document: 0.4.13
     Generated by: https://openapi-generator.tech
 """
 import dataclasses
 import typing
 
 from urllib3._collections import HTTPHeaderDict
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
 
 class ApiTypeError(OpenApiException, TypeError):
-    def __init__(self, msg, path_to_item=None, valid_classes=None, key_type=None):
-        """Raises an exception for TypeErrors
+    def __init__(self, msg, path_to_item=None, valid_classes=None,
+                 key_type=None):
+        """ Raises an exception for TypeErrors
 
         Args:
             msg (str): the exception message
 
         Keyword Args:
             path_to_item (list): a list of keys an indices to get to the
                                  current_item
@@ -119,17 +120,19 @@
     def headers(self) -> typing.Optional[HTTPHeaderDict]:
         if not self.api_response:
             return None
         return self.api_response.response.getheaders()
 
     def __str__(self):
         """Custom error messages for exception"""
-        error_message = "({0})\n" "Reason: {1}\n".format(self.status, self.reason)
+        error_message = "({0})\n"\
+                        "Reason: {1}\n".format(self.status, self.reason)
         if self.headers:
-            error_message += "HTTP response headers: {0}\n".format(self.headers)
+            error_message += "HTTP response headers: {0}\n".format(
+                self.headers)
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
```

### Comparing `gentrace_py-0.7.4/gentrace/model/feedback_request.py` & `gentrace_py-0.8.0/gentrace/model/feedback_request.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.8
+    The version of the OpenAPI document: 0.4.13
     Generated by: https://openapi-generator.tech
 """
 
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
@@ -18,168 +18,112 @@
 from datetime import date, datetime  # noqa: F401
 
 import frozendict  # noqa: F401
 import typing_extensions  # noqa: F401
 
 from gentrace import schemas  # noqa: F401
 
-
-class FeedbackRequest(schemas.DictSchema):
+class FeedbackRequest(
+    schemas.DictSchema
+):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
+
     class MetaOapg:
         required = {
             "score",
             "pipelineRunId",
             "recordedTime",
         }
-
+        
         class properties:
             pipelineRunId = schemas.UUIDSchema
-
-            class score(schemas.Float32Schema):
-                class MetaOapg:
-                    format = "float"
-                    inclusive_maximum = 1
-                    inclusive_minimum = 0
-
+            
+            
+            class score(
+                schemas.Float32Schema
+            ):
+                pass
             recordedTime = schemas.DateTimeSchema
-
+            
+            
             class details(
-                schemas.StrBase, schemas.NoneBase, schemas.Schema, schemas.NoneStrMixin
+                schemas.StrBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneStrMixin
             ):
+            
+            
                 def __new__(
                     cls,
-                    *_args: typing.Union[
-                        None,
-                        str,
-                    ],
+                    *_args: typing.Union[None, str, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> "details":
+                ) -> 'details':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                     )
-
             __annotations__ = {
                 "pipelineRunId": pipelineRunId,
                 "score": score,
                 "recordedTime": recordedTime,
                 "details": details,
             }
-
         additional_properties = schemas.NotAnyTypeSchema
-
+    
     score: MetaOapg.properties.score
     pipelineRunId: MetaOapg.properties.pipelineRunId
     recordedTime: MetaOapg.properties.recordedTime
-
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["score"]) -> MetaOapg.properties.score: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["pipelineRunId"]) -> MetaOapg.properties.pipelineRunId: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["recordedTime"]) -> MetaOapg.properties.recordedTime: ...
+    
     @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["score"]
-    ) -> MetaOapg.properties.score:
-        ...
-
-    @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["pipelineRunId"]
-    ) -> MetaOapg.properties.pipelineRunId:
-        ...
-
-    @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["recordedTime"]
-    ) -> MetaOapg.properties.recordedTime:
-        ...
-
-    @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["details"]
-    ) -> MetaOapg.properties.details:
-        ...
-
-    def __getitem__(
-        self,
-        name: typing.Union[
-            typing_extensions.Literal["score"],
-            typing_extensions.Literal["pipelineRunId"],
-            typing_extensions.Literal["recordedTime"],
-            typing_extensions.Literal["details"],
-        ],
-    ):
+    def __getitem__(self, name: typing_extensions.Literal["details"]) -> MetaOapg.properties.details: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["score"], typing_extensions.Literal["pipelineRunId"], typing_extensions.Literal["recordedTime"], typing_extensions.Literal["details"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
-
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["score"]) -> MetaOapg.properties.score: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["pipelineRunId"]) -> MetaOapg.properties.pipelineRunId: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["recordedTime"]) -> MetaOapg.properties.recordedTime: ...
+    
     @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["score"]
-    ) -> MetaOapg.properties.score:
-        ...
-
-    @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["pipelineRunId"]
-    ) -> MetaOapg.properties.pipelineRunId:
-        ...
-
-    @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["recordedTime"]
-    ) -> MetaOapg.properties.recordedTime:
-        ...
-
-    @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["details"]
-    ) -> typing.Union[MetaOapg.properties.details, schemas.Unset]:
-        ...
-
-    def get_item_oapg(
-        self,
-        name: typing.Union[
-            typing_extensions.Literal["score"],
-            typing_extensions.Literal["pipelineRunId"],
-            typing_extensions.Literal["recordedTime"],
-            typing_extensions.Literal["details"],
-        ],
-    ):
+    def get_item_oapg(self, name: typing_extensions.Literal["details"]) -> typing.Union[MetaOapg.properties.details, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["score"], typing_extensions.Literal["pipelineRunId"], typing_extensions.Literal["recordedTime"], typing_extensions.Literal["details"], ]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
-        *_args: typing.Union[
-            dict,
-            frozendict.frozendict,
-        ],
-        score: typing.Union[
-            MetaOapg.properties.score,
-            decimal.Decimal,
-            int,
-            float,
-        ],
-        pipelineRunId: typing.Union[
-            MetaOapg.properties.pipelineRunId,
-            str,
-            uuid.UUID,
-        ],
-        recordedTime: typing.Union[
-            MetaOapg.properties.recordedTime,
-            str,
-            datetime,
-        ],
-        details: typing.Union[
-            MetaOapg.properties.details, None, str, schemas.Unset
-        ] = schemas.unset,
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        score: typing.Union[MetaOapg.properties.score, decimal.Decimal, int, float, ],
+        pipelineRunId: typing.Union[MetaOapg.properties.pipelineRunId, str, uuid.UUID, ],
+        recordedTime: typing.Union[MetaOapg.properties.recordedTime, str, datetime, ],
+        details: typing.Union[MetaOapg.properties.details, None, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> "FeedbackRequest":
+    ) -> 'FeedbackRequest':
         return super().__new__(
             cls,
             *_args,
             score=score,
             pipelineRunId=pipelineRunId,
             recordedTime=recordedTime,
             details=details,
```

### Comparing `gentrace_py-0.7.4/gentrace/model/feedback_request.pyi` & `gentrace_py-0.8.0/gentrace/model/feedback_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.8
+    The version of the OpenAPI document: 0.4.13
     Generated by: https://openapi-generator.tech
 """
 
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
@@ -18,142 +18,118 @@
 from datetime import date, datetime  # noqa: F401
 
 import frozendict  # noqa: F401
 import typing_extensions  # noqa: F401
 
 from gentrace import schemas  # noqa: F401
 
-class FeedbackRequest(schemas.DictSchema):
+
+class FeedbackRequest(
+    schemas.DictSchema
+):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
+
     class MetaOapg:
         required = {
             "score",
             "pipelineRunId",
             "recordedTime",
         }
-
+        
         class properties:
             pipelineRunId = schemas.UUIDSchema
-
-            class score(schemas.Float32Schema):
-                pass
+            
+            
+            class score(
+                schemas.Float32Schema
+            ):
+            
+            
+                class MetaOapg:
+                    format = 'float'
+                    inclusive_maximum = 1
+                    inclusive_minimum = 0
             recordedTime = schemas.DateTimeSchema
-
+            
+            
             class details(
-                schemas.StrBase, schemas.NoneBase, schemas.Schema, schemas.NoneStrMixin
+                schemas.StrBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneStrMixin
             ):
+            
+            
                 def __new__(
                     cls,
-                    *_args: typing.Union[
-                        None,
-                        str,
-                    ],
+                    *_args: typing.Union[None, str, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> "details":
+                ) -> 'details':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                     )
             __annotations__ = {
                 "pipelineRunId": pipelineRunId,
                 "score": score,
                 "recordedTime": recordedTime,
                 "details": details,
             }
         additional_properties = schemas.NotAnyTypeSchema
+    
     score: MetaOapg.properties.score
     pipelineRunId: MetaOapg.properties.pipelineRunId
     recordedTime: MetaOapg.properties.recordedTime
-
+    
     @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["score"]
-    ) -> MetaOapg.properties.score: ...
-    @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["pipelineRunId"]
-    ) -> MetaOapg.properties.pipelineRunId: ...
-    @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["recordedTime"]
-    ) -> MetaOapg.properties.recordedTime: ...
-    @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["details"]
-    ) -> MetaOapg.properties.details: ...
-    def __getitem__(
-        self,
-        name: typing.Union[
-            typing_extensions.Literal["score"],
-            typing_extensions.Literal["pipelineRunId"],
-            typing_extensions.Literal["recordedTime"],
-            typing_extensions.Literal["details"],
-        ],
-    ):
+    def __getitem__(self, name: typing_extensions.Literal["score"]) -> MetaOapg.properties.score: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["pipelineRunId"]) -> MetaOapg.properties.pipelineRunId: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["recordedTime"]) -> MetaOapg.properties.recordedTime: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["details"]) -> MetaOapg.properties.details: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["score"], typing_extensions.Literal["pipelineRunId"], typing_extensions.Literal["recordedTime"], typing_extensions.Literal["details"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["score"]) -> MetaOapg.properties.score: ...
+    
     @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["score"]
-    ) -> MetaOapg.properties.score: ...
-    @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["pipelineRunId"]
-    ) -> MetaOapg.properties.pipelineRunId: ...
-    @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["recordedTime"]
-    ) -> MetaOapg.properties.recordedTime: ...
-    @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["details"]
-    ) -> typing.Union[MetaOapg.properties.details, schemas.Unset]: ...
-    def get_item_oapg(
-        self,
-        name: typing.Union[
-            typing_extensions.Literal["score"],
-            typing_extensions.Literal["pipelineRunId"],
-            typing_extensions.Literal["recordedTime"],
-            typing_extensions.Literal["details"],
-        ],
-    ):
+    def get_item_oapg(self, name: typing_extensions.Literal["pipelineRunId"]) -> MetaOapg.properties.pipelineRunId: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["recordedTime"]) -> MetaOapg.properties.recordedTime: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["details"]) -> typing.Union[MetaOapg.properties.details, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["score"], typing_extensions.Literal["pipelineRunId"], typing_extensions.Literal["recordedTime"], typing_extensions.Literal["details"], ]):
         return super().get_item_oapg(name)
+
     def __new__(
         cls,
-        *_args: typing.Union[
-            dict,
-            frozendict.frozendict,
-        ],
-        score: typing.Union[
-            MetaOapg.properties.score,
-            decimal.Decimal,
-            int,
-            float,
-        ],
-        pipelineRunId: typing.Union[
-            MetaOapg.properties.pipelineRunId,
-            str,
-            uuid.UUID,
-        ],
-        recordedTime: typing.Union[
-            MetaOapg.properties.recordedTime,
-            str,
-            datetime,
-        ],
-        details: typing.Union[
-            MetaOapg.properties.details, None, str, schemas.Unset
-        ] = schemas.unset,
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        score: typing.Union[MetaOapg.properties.score, decimal.Decimal, int, float, ],
+        pipelineRunId: typing.Union[MetaOapg.properties.pipelineRunId, str, uuid.UUID, ],
+        recordedTime: typing.Union[MetaOapg.properties.recordedTime, str, datetime, ],
+        details: typing.Union[MetaOapg.properties.details, None, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> "FeedbackRequest":
+    ) -> 'FeedbackRequest':
         return super().__new__(
             cls,
             *_args,
             score=score,
             pipelineRunId=pipelineRunId,
             recordedTime=recordedTime,
             details=details,
```

### Comparing `gentrace_py-0.7.4/gentrace/model/feedback_response.py` & `gentrace_py-0.8.0/gentrace/model/feedback_response.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.8
+    The version of the OpenAPI document: 0.4.13
     Generated by: https://openapi-generator.tech
 """
 
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
@@ -18,67 +18,56 @@
 from datetime import date, datetime  # noqa: F401
 
 import frozendict  # noqa: F401
 import typing_extensions  # noqa: F401
 
 from gentrace import schemas  # noqa: F401
 
-
-class FeedbackResponse(schemas.DictSchema):
+class FeedbackResponse(
+    schemas.DictSchema
+):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
+
     class MetaOapg:
         required = {
             "message",
         }
-
+        
         class properties:
             message = schemas.StrSchema
             __annotations__ = {
                 "message": message,
             }
-
         additional_properties = schemas.NotAnyTypeSchema
-
+    
     message: MetaOapg.properties.message
-
+    
     @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["message"]
-    ) -> MetaOapg.properties.message:
-        ...
-
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["message"],]):
+    def __getitem__(self, name: typing_extensions.Literal["message"]) -> MetaOapg.properties.message: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["message"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
-
+    
     @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["message"]
-    ) -> MetaOapg.properties.message:
-        ...
-
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["message"],]):
+    def get_item_oapg(self, name: typing_extensions.Literal["message"]) -> MetaOapg.properties.message: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["message"], ]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
-        *_args: typing.Union[
-            dict,
-            frozendict.frozendict,
-        ],
-        message: typing.Union[
-            MetaOapg.properties.message,
-            str,
-        ],
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        message: typing.Union[MetaOapg.properties.message, str, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> "FeedbackResponse":
+    ) -> 'FeedbackResponse':
         return super().__new__(
             cls,
             *_args,
             message=message,
             _configuration=_configuration,
         )
```

### Comparing `gentrace_py-0.7.4/gentrace/model/feedback_response.pyi` & `gentrace_py-0.8.0/gentrace/model/feedback_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.8
+    The version of the OpenAPI document: 0.4.13
     Generated by: https://openapi-generator.tech
 """
 
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
@@ -18,58 +18,57 @@
 from datetime import date, datetime  # noqa: F401
 
 import frozendict  # noqa: F401
 import typing_extensions  # noqa: F401
 
 from gentrace import schemas  # noqa: F401
 
-class FeedbackResponse(schemas.DictSchema):
+
+class FeedbackResponse(
+    schemas.DictSchema
+):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
+
     class MetaOapg:
         required = {
             "message",
         }
-
+        
         class properties:
             message = schemas.StrSchema
             __annotations__ = {
                 "message": message,
             }
         additional_properties = schemas.NotAnyTypeSchema
+    
     message: MetaOapg.properties.message
-
+    
     @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["message"]
-    ) -> MetaOapg.properties.message: ...
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["message"],]):
+    def __getitem__(self, name: typing_extensions.Literal["message"]) -> MetaOapg.properties.message: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["message"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
+    
     @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["message"]
-    ) -> MetaOapg.properties.message: ...
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["message"],]):
+    def get_item_oapg(self, name: typing_extensions.Literal["message"]) -> MetaOapg.properties.message: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["message"], ]):
         return super().get_item_oapg(name)
+
     def __new__(
         cls,
-        *_args: typing.Union[
-            dict,
-            frozendict.frozendict,
-        ],
-        message: typing.Union[
-            MetaOapg.properties.message,
-            str,
-        ],
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        message: typing.Union[MetaOapg.properties.message, str, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> "FeedbackResponse":
+    ) -> 'FeedbackResponse':
         return super().__new__(
             cls,
             *_args,
             message=message,
             _configuration=_configuration,
         )
```

### Comparing `gentrace_py-0.7.4/gentrace/model/pipeline_run_request.py` & `gentrace_py-0.8.0/gentrace/paths/test_run/post.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,723 +1,624 @@
 # coding: utf-8
 
 """
-    Gentrace API
 
-    These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.8
     Generated by: https://openapi-generator.tech
 """
 
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
 import typing  # noqa: F401
 import uuid  # noqa: F401
+from dataclasses import dataclass
 from datetime import date, datetime  # noqa: F401
 
 import frozendict  # noqa: F401
 import typing_extensions  # noqa: F401
+import urllib3
+from urllib3._collections import HTTPHeaderDict
 
-from gentrace import schemas  # noqa: F401
+from gentrace import (
+    api_client,
+    exceptions,
+    schemas,  # noqa: F401
+)
 
+# body param
 
-class PipelineRunRequest(schemas.DictSchema):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
-    """
+class SchemaForRequestBodyApplicationJson(
+    schemas.DictSchema
+):
+
 
     class MetaOapg:
         required = {
-            "stepRuns",
-            "name",
-            "id",
+            "testResults",
+            "setId",
+            "source",
         }
-
+        
         class properties:
-            id = schemas.UUIDSchema
-            name = schemas.StrSchema
-
-            class stepRuns(schemas.ListSchema):
+            setId = schemas.UUIDSchema
+            
+            
+            class source(
+                schemas.StrSchema
+            ):
+                pass
+            
+            
+            class testResults(
+                schemas.ListSchema
+            ):
+            
+            
                 class MetaOapg:
-                    class items(schemas.DictSchema):
+                    
+                    
+                    class items(
+                        schemas.DictSchema
+                    ):
+                    
+                    
                         class MetaOapg:
+                            required = {
+                                "output",
+                                "inputs",
+                                "caseId",
+                            }
+                            
                             class properties:
-                                class provider(schemas.DictSchema):
-                                    class MetaOapg:
-                                        class properties:
-                                            name = schemas.StrSchema
-                                            invocation = schemas.StrSchema
-
-                                            class modelParams(schemas.DictSchema):
-                                                class MetaOapg:
-                                                    additional_properties = (
-                                                        schemas.AnyTypeSchema
-                                                    )
-
-                                                def __getitem__(
-                                                    self, name: typing.Union[str,]
-                                                ) -> MetaOapg.additional_properties:
-                                                    # dict_instance[name] accessor
-                                                    return super().__getitem__(name)
-
-                                                def get_item_oapg(
-                                                    self, name: typing.Union[str,]
-                                                ) -> MetaOapg.additional_properties:
-                                                    return super().get_item_oapg(name)
-
-                                                def __new__(
-                                                    cls,
-                                                    *_args: typing.Union[
-                                                        dict,
-                                                        frozendict.frozendict,
-                                                    ],
-                                                    _configuration: typing.Optional[
-                                                        schemas.Configuration
-                                                    ] = None,
-                                                    **kwargs: typing.Union[
-                                                        MetaOapg.additional_properties,
-                                                        dict,
-                                                        frozendict.frozendict,
-                                                        str,
-                                                        date,
-                                                        datetime,
-                                                        uuid.UUID,
-                                                        int,
-                                                        float,
-                                                        decimal.Decimal,
-                                                        bool,
-                                                        None,
-                                                        list,
-                                                        tuple,
-                                                        bytes,
-                                                        io.FileIO,
-                                                        io.BufferedReader,
-                                                    ],
-                                                ) -> "modelParams":
-                                                    return super().__new__(
-                                                        cls,
-                                                        *_args,
-                                                        _configuration=_configuration,
-                                                        **kwargs,
-                                                    )
-
-                                            class inputs(schemas.DictSchema):
-                                                class MetaOapg:
-                                                    additional_properties = (
-                                                        schemas.AnyTypeSchema
-                                                    )
-
-                                                def __getitem__(
-                                                    self, name: typing.Union[str,]
-                                                ) -> MetaOapg.additional_properties:
-                                                    # dict_instance[name] accessor
-                                                    return super().__getitem__(name)
-
-                                                def get_item_oapg(
-                                                    self, name: typing.Union[str,]
-                                                ) -> MetaOapg.additional_properties:
-                                                    return super().get_item_oapg(name)
-
-                                                def __new__(
-                                                    cls,
-                                                    *_args: typing.Union[
-                                                        dict,
-                                                        frozendict.frozendict,
-                                                    ],
-                                                    _configuration: typing.Optional[
-                                                        schemas.Configuration
-                                                    ] = None,
-                                                    **kwargs: typing.Union[
-                                                        MetaOapg.additional_properties,
-                                                        dict,
-                                                        frozendict.frozendict,
-                                                        str,
-                                                        date,
-                                                        datetime,
-                                                        uuid.UUID,
-                                                        int,
-                                                        float,
-                                                        decimal.Decimal,
-                                                        bool,
-                                                        None,
-                                                        list,
-                                                        tuple,
-                                                        bytes,
-                                                        io.FileIO,
-                                                        io.BufferedReader,
-                                                    ],
-                                                ) -> "inputs":
-                                                    return super().__new__(
-                                                        cls,
-                                                        *_args,
-                                                        _configuration=_configuration,
-                                                        **kwargs,
-                                                    )
-
-                                            class outputs(schemas.DictSchema):
-                                                class MetaOapg:
-                                                    additional_properties = (
-                                                        schemas.AnyTypeSchema
-                                                    )
-
-                                                def __getitem__(
-                                                    self, name: typing.Union[str,]
-                                                ) -> MetaOapg.additional_properties:
-                                                    # dict_instance[name] accessor
-                                                    return super().__getitem__(name)
-
-                                                def get_item_oapg(
-                                                    self, name: typing.Union[str,]
-                                                ) -> MetaOapg.additional_properties:
-                                                    return super().get_item_oapg(name)
-
-                                                def __new__(
-                                                    cls,
-                                                    *_args: typing.Union[
-                                                        dict,
-                                                        frozendict.frozendict,
-                                                    ],
-                                                    _configuration: typing.Optional[
-                                                        schemas.Configuration
-                                                    ] = None,
-                                                    **kwargs: typing.Union[
-                                                        MetaOapg.additional_properties,
-                                                        dict,
-                                                        frozendict.frozendict,
-                                                        str,
-                                                        date,
-                                                        datetime,
-                                                        uuid.UUID,
-                                                        int,
-                                                        float,
-                                                        decimal.Decimal,
-                                                        bool,
-                                                        None,
-                                                        list,
-                                                        tuple,
-                                                        bytes,
-                                                        io.FileIO,
-                                                        io.BufferedReader,
-                                                    ],
-                                                ) -> "outputs":
-                                                    return super().__new__(
-                                                        cls,
-                                                        *_args,
-                                                        _configuration=_configuration,
-                                                        **kwargs,
-                                                    )
-
-                                            __annotations__ = {
-                                                "name": name,
-                                                "invocation": invocation,
-                                                "modelParams": modelParams,
-                                                "inputs": inputs,
-                                                "outputs": outputs,
-                                            }
-
-                                    @typing.overload
-                                    def __getitem__(
-                                        self, name: typing_extensions.Literal["name"]
-                                    ) -> MetaOapg.properties.name:
-                                        ...
-
-                                    @typing.overload
-                                    def __getitem__(
-                                        self,
-                                        name: typing_extensions.Literal["invocation"],
-                                    ) -> MetaOapg.properties.invocation:
-                                        ...
-
-                                    @typing.overload
-                                    def __getitem__(
-                                        self,
-                                        name: typing_extensions.Literal["modelParams"],
-                                    ) -> MetaOapg.properties.modelParams:
-                                        ...
-
-                                    @typing.overload
-                                    def __getitem__(
-                                        self, name: typing_extensions.Literal["inputs"]
-                                    ) -> MetaOapg.properties.inputs:
-                                        ...
-
-                                    @typing.overload
-                                    def __getitem__(
-                                        self, name: typing_extensions.Literal["outputs"]
-                                    ) -> MetaOapg.properties.outputs:
-                                        ...
-
-                                    @typing.overload
-                                    def __getitem__(
-                                        self, name: str
-                                    ) -> schemas.UnsetAnyTypeSchema:
-                                        ...
-
-                                    def __getitem__(
-                                        self,
-                                        name: typing.Union[
-                                            typing_extensions.Literal[
-                                                "name",
-                                                "invocation",
-                                                "modelParams",
-                                                "inputs",
-                                                "outputs",
-                                            ],
-                                            str,
-                                        ],
-                                    ):
-                                        # dict_instance[name] accessor
-                                        return super().__getitem__(name)
-
-                                    @typing.overload
-                                    def get_item_oapg(
-                                        self, name: typing_extensions.Literal["name"]
-                                    ) -> typing.Union[
-                                        MetaOapg.properties.name, schemas.Unset
-                                    ]:
-                                        ...
-
-                                    @typing.overload
-                                    def get_item_oapg(
-                                        self,
-                                        name: typing_extensions.Literal["invocation"],
-                                    ) -> typing.Union[
-                                        MetaOapg.properties.invocation, schemas.Unset
-                                    ]:
-                                        ...
-
-                                    @typing.overload
-                                    def get_item_oapg(
-                                        self,
-                                        name: typing_extensions.Literal["modelParams"],
-                                    ) -> typing.Union[
-                                        MetaOapg.properties.modelParams, schemas.Unset
-                                    ]:
-                                        ...
-
-                                    @typing.overload
-                                    def get_item_oapg(
-                                        self, name: typing_extensions.Literal["inputs"]
-                                    ) -> typing.Union[
-                                        MetaOapg.properties.inputs, schemas.Unset
-                                    ]:
-                                        ...
-
-                                    @typing.overload
-                                    def get_item_oapg(
-                                        self, name: typing_extensions.Literal["outputs"]
-                                    ) -> typing.Union[
-                                        MetaOapg.properties.outputs, schemas.Unset
-                                    ]:
-                                        ...
-
-                                    @typing.overload
-                                    def get_item_oapg(
-                                        self, name: str
-                                    ) -> typing.Union[
-                                        schemas.UnsetAnyTypeSchema, schemas.Unset
-                                    ]:
-                                        ...
-
-                                    def get_item_oapg(
-                                        self,
-                                        name: typing.Union[
-                                            typing_extensions.Literal[
-                                                "name",
-                                                "invocation",
-                                                "modelParams",
-                                                "inputs",
-                                                "outputs",
-                                            ],
-                                            str,
-                                        ],
-                                    ):
-                                        return super().get_item_oapg(name)
-
-                                    def __new__(
-                                        cls,
-                                        *_args: typing.Union[
-                                            dict,
-                                            frozendict.frozendict,
-                                        ],
-                                        name: typing.Union[
-                                            MetaOapg.properties.name, str, schemas.Unset
-                                        ] = schemas.unset,
-                                        invocation: typing.Union[
-                                            MetaOapg.properties.invocation,
-                                            str,
-                                            schemas.Unset,
-                                        ] = schemas.unset,
-                                        modelParams: typing.Union[
-                                            MetaOapg.properties.modelParams,
-                                            dict,
-                                            frozendict.frozendict,
-                                            schemas.Unset,
-                                        ] = schemas.unset,
-                                        inputs: typing.Union[
-                                            MetaOapg.properties.inputs,
-                                            dict,
-                                            frozendict.frozendict,
-                                            schemas.Unset,
-                                        ] = schemas.unset,
-                                        outputs: typing.Union[
-                                            MetaOapg.properties.outputs,
-                                            dict,
-                                            frozendict.frozendict,
-                                            schemas.Unset,
-                                        ] = schemas.unset,
-                                        _configuration: typing.Optional[
-                                            schemas.Configuration
-                                        ] = None,
-                                        **kwargs: typing.Union[
-                                            schemas.AnyTypeSchema,
-                                            dict,
-                                            frozendict.frozendict,
-                                            str,
-                                            date,
-                                            datetime,
-                                            uuid.UUID,
-                                            int,
-                                            float,
-                                            decimal.Decimal,
-                                            None,
-                                            list,
-                                            tuple,
-                                            bytes,
-                                        ],
-                                    ) -> "provider":
-                                        return super().__new__(
-                                            cls,
-                                            *_args,
-                                            name=name,
-                                            invocation=invocation,
-                                            modelParams=modelParams,
-                                            inputs=inputs,
-                                            outputs=outputs,
-                                            _configuration=_configuration,
-                                            **kwargs,
-                                        )
-
-                                elapsedTime = schemas.IntSchema
-                                startTime = schemas.DateTimeSchema
-                                endTime = schemas.DateTimeSchema
+                                id = schemas.UUIDSchema
+                                caseId = schemas.UUIDSchema
+                                inputs = schemas.DictSchema
+                                output = schemas.StrSchema
                                 __annotations__ = {
-                                    "provider": provider,
-                                    "elapsedTime": elapsedTime,
-                                    "startTime": startTime,
-                                    "endTime": endTime,
+                                    "id": id,
+                                    "caseId": caseId,
+                                    "inputs": inputs,
+                                    "output": output,
                                 }
-
+                        
+                        output: MetaOapg.properties.output
+                        inputs: MetaOapg.properties.inputs
+                        caseId: MetaOapg.properties.caseId
+                        
                         @typing.overload
-                        def __getitem__(
-                            self, name: typing_extensions.Literal["provider"]
-                        ) -> MetaOapg.properties.provider:
-                            ...
-
+                        def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+                        
                         @typing.overload
-                        def __getitem__(
-                            self, name: typing_extensions.Literal["elapsedTime"]
-                        ) -> MetaOapg.properties.elapsedTime:
-                            ...
-
+                        def __getitem__(self, name: typing_extensions.Literal["caseId"]) -> MetaOapg.properties.caseId: ...
+                        
                         @typing.overload
-                        def __getitem__(
-                            self, name: typing_extensions.Literal["startTime"]
-                        ) -> MetaOapg.properties.startTime:
-                            ...
-
+                        def __getitem__(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
+                        
                         @typing.overload
-                        def __getitem__(
-                            self, name: typing_extensions.Literal["endTime"]
-                        ) -> MetaOapg.properties.endTime:
-                            ...
-
+                        def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
+                        
                         @typing.overload
-                        def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
-                            ...
-
-                        def __getitem__(
-                            self,
-                            name: typing.Union[
-                                typing_extensions.Literal[
-                                    "provider",
-                                    "elapsedTime",
-                                    "startTime",
-                                    "endTime",
-                                ],
-                                str,
-                            ],
-                        ):
+                        def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+                        
+                        def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "caseId", "inputs", "output", ], str]):
                             # dict_instance[name] accessor
                             return super().__getitem__(name)
-
+                        
+                        
                         @typing.overload
-                        def get_item_oapg(
-                            self, name: typing_extensions.Literal["provider"]
-                        ) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]:
-                            ...
-
+                        def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
+                        
                         @typing.overload
-                        def get_item_oapg(
-                            self, name: typing_extensions.Literal["elapsedTime"]
-                        ) -> typing.Union[
-                            MetaOapg.properties.elapsedTime, schemas.Unset
-                        ]:
-                            ...
-
+                        def get_item_oapg(self, name: typing_extensions.Literal["caseId"]) -> MetaOapg.properties.caseId: ...
+                        
                         @typing.overload
-                        def get_item_oapg(
-                            self, name: typing_extensions.Literal["startTime"]
-                        ) -> typing.Union[MetaOapg.properties.startTime, schemas.Unset]:
-                            ...
-
+                        def get_item_oapg(self, name: typing_extensions.Literal["inputs"]) -> MetaOapg.properties.inputs: ...
+                        
                         @typing.overload
-                        def get_item_oapg(
-                            self, name: typing_extensions.Literal["endTime"]
-                        ) -> typing.Union[MetaOapg.properties.endTime, schemas.Unset]:
-                            ...
-
+                        def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
+                        
                         @typing.overload
-                        def get_item_oapg(
-                            self, name: str
-                        ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
-                            ...
-
-                        def get_item_oapg(
-                            self,
-                            name: typing.Union[
-                                typing_extensions.Literal[
-                                    "provider",
-                                    "elapsedTime",
-                                    "startTime",
-                                    "endTime",
-                                ],
-                                str,
-                            ],
-                        ):
+                        def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+                        
+                        def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "caseId", "inputs", "output", ], str]):
                             return super().get_item_oapg(name)
-
+                        
+                    
                         def __new__(
                             cls,
-                            *_args: typing.Union[
-                                dict,
-                                frozendict.frozendict,
-                            ],
-                            provider: typing.Union[
-                                MetaOapg.properties.provider,
-                                dict,
-                                frozendict.frozendict,
-                                schemas.Unset,
-                            ] = schemas.unset,
-                            elapsedTime: typing.Union[
-                                MetaOapg.properties.elapsedTime,
-                                decimal.Decimal,
-                                int,
-                                schemas.Unset,
-                            ] = schemas.unset,
-                            startTime: typing.Union[
-                                MetaOapg.properties.startTime,
-                                str,
-                                datetime,
-                                schemas.Unset,
-                            ] = schemas.unset,
-                            endTime: typing.Union[
-                                MetaOapg.properties.endTime,
-                                str,
-                                datetime,
-                                schemas.Unset,
-                            ] = schemas.unset,
-                            _configuration: typing.Optional[
-                                schemas.Configuration
-                            ] = None,
-                            **kwargs: typing.Union[
-                                schemas.AnyTypeSchema,
-                                dict,
-                                frozendict.frozendict,
-                                str,
-                                date,
-                                datetime,
-                                uuid.UUID,
-                                int,
-                                float,
-                                decimal.Decimal,
-                                None,
-                                list,
-                                tuple,
-                                bytes,
-                            ],
-                        ) -> "items":
+                            *_args: typing.Union[dict, frozendict.frozendict, ],
+                            output: typing.Union[MetaOapg.properties.output, str, ],
+                            inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, ],
+                            caseId: typing.Union[MetaOapg.properties.caseId, str, uuid.UUID, ],
+                            id: typing.Union[MetaOapg.properties.id, str, uuid.UUID, schemas.Unset] = schemas.unset,
+                            _configuration: typing.Optional[schemas.Configuration] = None,
+                            **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                        ) -> 'items':
                             return super().__new__(
                                 cls,
                                 *_args,
-                                provider=provider,
-                                elapsedTime=elapsedTime,
-                                startTime=startTime,
-                                endTime=endTime,
+                                output=output,
+                                inputs=inputs,
+                                caseId=caseId,
+                                id=id,
                                 _configuration=_configuration,
                                 **kwargs,
                             )
-
+            
                 def __new__(
                     cls,
-                    _arg: typing.Union[
-                        typing.Tuple[
-                            typing.Union[
-                                MetaOapg.items,
-                                dict,
-                                frozendict.frozendict,
-                            ]
-                        ],
-                        typing.List[
-                            typing.Union[
-                                MetaOapg.items,
-                                dict,
-                                frozendict.frozendict,
-                            ]
-                        ],
-                    ],
+                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, dict, frozendict.frozendict, ]], typing.List[typing.Union[MetaOapg.items, dict, frozendict.frozendict, ]]],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> "stepRuns":
+                ) -> 'testResults':
                     return super().__new__(
                         cls,
                         _arg,
                         _configuration=_configuration,
                     )
-
+            
                 def __getitem__(self, i: int) -> MetaOapg.items:
                     return super().__getitem__(i)
-
             __annotations__ = {
-                "id": id,
-                "name": name,
-                "stepRuns": stepRuns,
+                "setId": setId,
+                "source": source,
+                "testResults": testResults,
             }
+    
+    testResults: MetaOapg.properties.testResults
+    setId: MetaOapg.properties.setId
+    source: MetaOapg.properties.source
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["setId"]) -> MetaOapg.properties.setId: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["testResults"]) -> MetaOapg.properties.testResults: ...
+    
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["setId", "source", "testResults", ], str]):
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+    
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["setId"]) -> MetaOapg.properties.setId: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["testResults"]) -> MetaOapg.properties.testResults: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["setId", "source", "testResults", ], str]):
+        return super().get_item_oapg(name)
+    
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        testResults: typing.Union[MetaOapg.properties.testResults, list, tuple, ],
+        setId: typing.Union[MetaOapg.properties.setId, str, uuid.UUID, ],
+        source: typing.Union[MetaOapg.properties.source, str, ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'SchemaForRequestBodyApplicationJson':
+        return super().__new__(
+            cls,
+            *_args,
+            testResults=testResults,
+            setId=setId,
+            source=source,
+            _configuration=_configuration,
+            **kwargs,
+        )
 
-    stepRuns: MetaOapg.properties.stepRuns
-    name: MetaOapg.properties.name
-    id: MetaOapg.properties.id
 
-    @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["id"]
-    ) -> MetaOapg.properties.id:
-        ...
+request_body_any_type = api_client.RequestBody(
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaForRequestBodyApplicationJson),
+    },
+    required=True,
+)
 
-    @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["name"]
-    ) -> MetaOapg.properties.name:
-        ...
 
-    @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["stepRuns"]
-    ) -> MetaOapg.properties.stepRuns:
-        ...
+class SchemaFor200ResponseBodyApplicationJson(
+    schemas.DictSchema
+):
 
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
-        ...
 
-    def __getitem__(
-        self,
-        name: typing.Union[
-            typing_extensions.Literal[
-                "id",
-                "name",
-                "stepRuns",
-            ],
-            str,
-        ],
-    ):
+    class MetaOapg:
+        
+        class properties:
+            runId = schemas.UUIDSchema
+            __annotations__ = {
+                "runId": runId,
+            }
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["runId"]) -> MetaOapg.properties.runId: ...
+    
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["runId", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
+    
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["runId"]) -> typing.Union[MetaOapg.properties.runId, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["runId", ], str]):
+        return super().get_item_oapg(name)
+    
 
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        runId: typing.Union[MetaOapg.properties.runId, str, uuid.UUID, schemas.Unset] = schemas.unset,
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'SchemaFor200ResponseBodyApplicationJson':
+        return super().__new__(
+            cls,
+            *_args,
+            runId=runId,
+            _configuration=_configuration,
+            **kwargs,
+        )
+
+
+class SchemaFor200ResponseBodyApplicationJsonCharsetutf8(
+    schemas.DictSchema
+):
+
+
+    class MetaOapg:
+        
+        class properties:
+            runId = schemas.UUIDSchema
+            __annotations__ = {
+                "runId": runId,
+            }
+    
     @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["id"]
-    ) -> MetaOapg.properties.id:
-        ...
-
-    @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["name"]
-    ) -> MetaOapg.properties.name:
-        ...
-
-    @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["stepRuns"]
-    ) -> MetaOapg.properties.stepRuns:
-        ...
-
-    @typing.overload
-    def get_item_oapg(
-        self, name: str
-    ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
-        ...
-
-    def get_item_oapg(
-        self,
-        name: typing.Union[
-            typing_extensions.Literal[
-                "id",
-                "name",
-                "stepRuns",
-            ],
-            str,
-        ],
-    ):
+    def __getitem__(self, name: typing_extensions.Literal["runId"]) -> MetaOapg.properties.runId: ...
+    
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["runId", ], str]):
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+    
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["runId"]) -> typing.Union[MetaOapg.properties.runId, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["runId", ], str]):
         return super().get_item_oapg(name)
+    
 
     def __new__(
         cls,
-        *_args: typing.Union[
-            dict,
-            frozendict.frozendict,
-        ],
-        stepRuns: typing.Union[
-            MetaOapg.properties.stepRuns,
-            list,
-            tuple,
-        ],
-        name: typing.Union[
-            MetaOapg.properties.name,
-            str,
-        ],
-        id: typing.Union[
-            MetaOapg.properties.id,
-            str,
-            uuid.UUID,
-        ],
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        runId: typing.Union[MetaOapg.properties.runId, str, uuid.UUID, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[
-            schemas.AnyTypeSchema,
-            dict,
-            frozendict.frozendict,
-            str,
-            date,
-            datetime,
-            uuid.UUID,
-            int,
-            float,
-            decimal.Decimal,
-            None,
-            list,
-            tuple,
-            bytes,
-        ],
-    ) -> "PipelineRunRequest":
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'SchemaFor200ResponseBodyApplicationJsonCharsetutf8':
         return super().__new__(
             cls,
             *_args,
-            stepRuns=stepRuns,
-            name=name,
-            id=id,
+            runId=runId,
             _configuration=_configuration,
             **kwargs,
         )
+
+
+@dataclass
+class ApiResponseFor200(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJsonCharsetutf8,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor200ResponseBodyApplicationJson),
+        'application/json; charset=utf-8': api_client.MediaType(
+            schema=SchemaFor200ResponseBodyApplicationJsonCharsetutf8),
+    },
+)
+_all_accept_content_types = (
+    'application/json',
+    'application/json; charset=utf-8',
+)
+
+
+class BaseApi(api_client.Api):
+    @typing.overload
+    def _test_run_post_oapg(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,dict, frozendict.frozendict, ],
+        content_type: typing_extensions.Literal["application/json"] = ...,
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+    @typing.overload
+    def _test_run_post_oapg(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,dict, frozendict.frozendict, ],
+        content_type: str = ...,
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+
+    @typing.overload
+    def _test_run_post_oapg(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,dict, frozendict.frozendict, ],
+        skip_deserialization: typing_extensions.Literal[True],
+        content_type: str = ...,
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+    ) -> api_client.ApiResponseWithoutDeserialization: ...
+
+    @typing.overload
+    def _test_run_post_oapg(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,dict, frozendict.frozendict, ],
+        content_type: str = ...,
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: bool = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+        api_client.ApiResponseWithoutDeserialization,
+    ]: ...
+
+    def _test_run_post_oapg(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,dict, frozendict.frozendict, ],
+        content_type: str = 'application/json',
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: bool = False,
+    ):
+        """
+        Create a new test run from test results
+        :param skip_deserialization: If true then api_response.response will be set but
+            api_response.body and api_response.headers will not be deserialized into schema
+            class instances
+        """
+        used_path = path.value
+
+        _headers = HTTPHeaderDict()
+        # TODO add cookie handling
+        if accept_content_types:
+            for accept_content_type in accept_content_types:
+                _headers.add('Accept', accept_content_type)
+
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_any_type.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']
+        response = self.api_client.call_api(
+            resource_path=used_path,
+            method='post'.upper(),
+            headers=_headers,
+            fields=_fields,
+            body=_body,
+            auth_settings=_auth,
+            stream=stream,
+            timeout=timeout,
+        )
+
+        if skip_deserialization:
+            api_response = api_client.ApiResponseWithoutDeserialization(response=response)
+        else:
+            response_for_status = _status_code_to_response.get(str(response.status))
+            if response_for_status:
+                api_response = response_for_status.deserialize(response, self.api_client.configuration)
+            else:
+                api_response = api_client.ApiResponseWithoutDeserialization(response=response)
+
+        if not 200 <= response.status <= 299:
+            raise exceptions.ApiException(
+                status=response.status,
+                reason=response.reason,
+                api_response=api_response
+            )
+
+        return api_response
+
+
+class TestRunPost(BaseApi):
+    # this class is used by api classes that refer to endpoints with operationId fn names
+
+    @typing.overload
+    def test_run_post(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,dict, frozendict.frozendict, ],
+        content_type: typing_extensions.Literal["application/json"] = ...,
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+    @typing.overload
+    def test_run_post(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,dict, frozendict.frozendict, ],
+        content_type: str = ...,
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+
+    @typing.overload
+    def test_run_post(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,dict, frozendict.frozendict, ],
+        skip_deserialization: typing_extensions.Literal[True],
+        content_type: str = ...,
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+    ) -> api_client.ApiResponseWithoutDeserialization: ...
+
+    @typing.overload
+    def test_run_post(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,dict, frozendict.frozendict, ],
+        content_type: str = ...,
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: bool = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+        api_client.ApiResponseWithoutDeserialization,
+    ]: ...
+
+    def test_run_post(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,dict, frozendict.frozendict, ],
+        content_type: str = 'application/json',
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: bool = False,
+    ):
+        return self._test_run_post_oapg(
+            body=body,
+            content_type=content_type,
+            accept_content_types=accept_content_types,
+            stream=stream,
+            timeout=timeout,
+            skip_deserialization=skip_deserialization
+        )
+
+
+class ApiForpost(BaseApi):
+    # this class is used by api classes that refer to endpoints by path and http method names
+
+    @typing.overload
+    def post(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,dict, frozendict.frozendict, ],
+        content_type: typing_extensions.Literal["application/json"] = ...,
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+    @typing.overload
+    def post(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,dict, frozendict.frozendict, ],
+        content_type: str = ...,
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+
+    @typing.overload
+    def post(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,dict, frozendict.frozendict, ],
+        skip_deserialization: typing_extensions.Literal[True],
+        content_type: str = ...,
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+    ) -> api_client.ApiResponseWithoutDeserialization: ...
+
+    @typing.overload
+    def post(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,dict, frozendict.frozendict, ],
+        content_type: str = ...,
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: bool = ...,
+    ) -> typing.Union[
+        ApiResponseFor200,
+        api_client.ApiResponseWithoutDeserialization,
+    ]: ...
+
+    def post(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationJson,dict, frozendict.frozendict, ],
+        content_type: str = 'application/json',
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: bool = False,
+    ):
+        return self._test_run_post_oapg(
+            body=body,
+            content_type=content_type,
+            accept_content_types=accept_content_types,
+            stream=stream,
+            timeout=timeout,
+            skip_deserialization=skip_deserialization
+        )
+
+
```

### Comparing `gentrace_py-0.7.4/gentrace/model/pipeline_run_response.py` & `gentrace_py-0.8.0/gentrace/model/pipeline_run_response.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.8
+    The version of the OpenAPI document: 0.4.13
     Generated by: https://openapi-generator.tech
 """
 
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
@@ -18,89 +18,60 @@
 from datetime import date, datetime  # noqa: F401
 
 import frozendict  # noqa: F401
 import typing_extensions  # noqa: F401
 
 from gentrace import schemas  # noqa: F401
 
-
-class PipelineRunResponse(schemas.DictSchema):
+class PipelineRunResponse(
+    schemas.DictSchema
+):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
+
     class MetaOapg:
+        
         class properties:
-            pipelineRunId = schemas.StrSchema
+            pipelineRunId = schemas.UUIDSchema
             __annotations__ = {
                 "pipelineRunId": pipelineRunId,
             }
-
+    
     @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["pipelineRunId"]
-    ) -> MetaOapg.properties.pipelineRunId:
-        ...
-
+    def __getitem__(self, name: typing_extensions.Literal["pipelineRunId"]) -> MetaOapg.properties.pipelineRunId: ...
+    
     @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
-        ...
-
-    def __getitem__(
-        self, name: typing.Union[typing_extensions.Literal["pipelineRunId",], str]
-    ):
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["pipelineRunId", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
-
+    
+    
     @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["pipelineRunId"]
-    ) -> typing.Union[MetaOapg.properties.pipelineRunId, schemas.Unset]:
-        ...
-
+    def get_item_oapg(self, name: typing_extensions.Literal["pipelineRunId"]) -> typing.Union[MetaOapg.properties.pipelineRunId, schemas.Unset]: ...
+    
     @typing.overload
-    def get_item_oapg(
-        self, name: str
-    ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
-        ...
-
-    def get_item_oapg(
-        self, name: typing.Union[typing_extensions.Literal["pipelineRunId",], str]
-    ):
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["pipelineRunId", ], str]):
         return super().get_item_oapg(name)
+    
 
     def __new__(
         cls,
-        *_args: typing.Union[
-            dict,
-            frozendict.frozendict,
-        ],
-        pipelineRunId: typing.Union[
-            MetaOapg.properties.pipelineRunId, str, schemas.Unset
-        ] = schemas.unset,
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        pipelineRunId: typing.Union[MetaOapg.properties.pipelineRunId, str, uuid.UUID, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[
-            schemas.AnyTypeSchema,
-            dict,
-            frozendict.frozendict,
-            str,
-            date,
-            datetime,
-            uuid.UUID,
-            int,
-            float,
-            decimal.Decimal,
-            None,
-            list,
-            tuple,
-            bytes,
-        ],
-    ) -> "PipelineRunResponse":
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'PipelineRunResponse':
         return super().__new__(
             cls,
             *_args,
             pipelineRunId=pipelineRunId,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `gentrace_py-0.7.4/gentrace/model/pipeline_run_response.pyi` & `gentrace_py-0.8.0/gentrace/model/pipeline_run_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.8
+    The version of the OpenAPI document: 0.4.13
     Generated by: https://openapi-generator.tech
 """
 
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
@@ -18,77 +18,61 @@
 from datetime import date, datetime  # noqa: F401
 
 import frozendict  # noqa: F401
 import typing_extensions  # noqa: F401
 
 from gentrace import schemas  # noqa: F401
 
-class PipelineRunResponse(schemas.DictSchema):
+
+class PipelineRunResponse(
+    schemas.DictSchema
+):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
+
     class MetaOapg:
+        
         class properties:
-            pipelineRunId = schemas.StrSchema
+            pipelineRunId = schemas.UUIDSchema
             __annotations__ = {
                 "pipelineRunId": pipelineRunId,
             }
+    
     @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["pipelineRunId"]
-    ) -> MetaOapg.properties.pipelineRunId: ...
+    def __getitem__(self, name: typing_extensions.Literal["pipelineRunId"]) -> MetaOapg.properties.pipelineRunId: ...
+    
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    def __getitem__(
-        self, name: typing.Union[typing_extensions.Literal["pipelineRunId",], str]
-    ):
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["pipelineRunId", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
+    
+    
     @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["pipelineRunId"]
-    ) -> typing.Union[MetaOapg.properties.pipelineRunId, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["pipelineRunId"]) -> typing.Union[MetaOapg.properties.pipelineRunId, schemas.Unset]: ...
+    
     @typing.overload
-    def get_item_oapg(
-        self, name: str
-    ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    def get_item_oapg(
-        self, name: typing.Union[typing_extensions.Literal["pipelineRunId",], str]
-    ):
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["pipelineRunId", ], str]):
         return super().get_item_oapg(name)
+    
+
     def __new__(
         cls,
-        *_args: typing.Union[
-            dict,
-            frozendict.frozendict,
-        ],
-        pipelineRunId: typing.Union[
-            MetaOapg.properties.pipelineRunId, str, schemas.Unset
-        ] = schemas.unset,
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        pipelineRunId: typing.Union[MetaOapg.properties.pipelineRunId, str, uuid.UUID, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[
-            schemas.AnyTypeSchema,
-            dict,
-            frozendict.frozendict,
-            str,
-            date,
-            datetime,
-            uuid.UUID,
-            int,
-            float,
-            decimal.Decimal,
-            None,
-            list,
-            tuple,
-            bytes,
-        ],
-    ) -> "PipelineRunResponse":
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'PipelineRunResponse':
         return super().__new__(
             cls,
             *_args,
             pipelineRunId=pipelineRunId,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `gentrace_py-0.7.4/gentrace/models/__init__.py` & `gentrace_py-0.8.0/gentrace/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,7 +11,9 @@
 # import sys
 # sys.setrecursionlimit(n)
 
 from gentrace.model.feedback_request import FeedbackRequest
 from gentrace.model.feedback_response import FeedbackResponse
 from gentrace.model.pipeline_run_request import PipelineRunRequest
 from gentrace.model.pipeline_run_response import PipelineRunResponse
+from gentrace.model.test_case import TestCase
+from gentrace.model.test_run import TestRun
```

### Comparing `gentrace_py-0.7.4/gentrace/paths/pipeline_run/post.py` & `gentrace_py-0.8.0/gentrace/paths/pipeline_run/post.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,22 +32,21 @@
 
 # body param
 SchemaForRequestBodyApplicationJson = PipelineRunRequest
 
 
 request_body_pipeline_run_request = api_client.RequestBody(
     content={
-        "application/json": api_client.MediaType(
-            schema=SchemaForRequestBodyApplicationJson
-        ),
+        'application/json': api_client.MediaType(
+            schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
-    "bearerAuth",
+    'bearerAuth',
 ]
 SchemaFor200ResponseBodyApplicationJsonCharsetutf8 = PipelineRunResponse
 SchemaFor200ResponseBodyApplicationJson = PipelineRunResponse
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
@@ -58,20 +57,18 @@
     ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
-        "application/json; charset=utf-8": api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJsonCharsetutf8
-        ),
-        "application/json": api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson
-        ),
+        'application/json; charset=utf-8': api_client.MediaType(
+            schema=SchemaFor200ResponseBodyApplicationJsonCharsetutf8),
+        'application/json': api_client.MediaType(
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -91,77 +88,81 @@
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_500 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor500,
 )
 _status_code_to_response = {
-    "200": _response_for_200,
-    "400": _response_for_400,
-    "500": _response_for_500,
+    '200': _response_for_200,
+    '400': _response_for_400,
+    '500': _response_for_500,
 }
 _all_accept_content_types = (
-    "application/json; charset=utf-8",
-    "application/json",
+    'application/json; charset=utf-8',
+    'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
     def _pipeline_run_post_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: typing_extensions.Literal["application/json"] = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
-        ...
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
 
     @typing.overload
     def _pipeline_run_post_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
-        ...
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
 
     @typing.overload
     def _pipeline_run_post_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization:
-        ...
+    ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
     def _pipeline_run_post_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor200, api_client.ApiResponseWithoutDeserialization,]:
-        ...
+    ) -> typing.Union[
+        ApiResponseFor200,
+        api_client.ApiResponseWithoutDeserialization,
+    ]: ...
 
     def _pipeline_run_post_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = "application/json",
+        content_type: str = 'application/json',
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
         Create a pipeline run
@@ -171,61 +172,52 @@
         """
         used_path = path.value
 
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
-                _headers.add("Accept", accept_content_type)
+                _headers.add('Accept', accept_content_type)
 
         if body is schemas.unset:
             raise exceptions.ApiValueError(
-                "The required body parameter has an invalid value of: unset. Set a valid value instead"
-            )
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
-        serialized_data = request_body_pipeline_run_request.serialize(
-            body, content_type
-        )
-        _headers.add("Content-Type", content_type)
-        if "fields" in serialized_data:
-            _fields = serialized_data["fields"]
-        elif "body" in serialized_data:
-            _body = serialized_data["body"]
+        serialized_data = request_body_pipeline_run_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']
         response = self.api_client.call_api(
             resource_path=used_path,
-            method="post".upper(),
+            method='post'.upper(),
             headers=_headers,
             fields=_fields,
             body=_body,
             auth_settings=_auth,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
-            api_response = api_client.ApiResponseWithoutDeserialization(
-                response=response
-            )
+            api_response = api_client.ApiResponseWithoutDeserialization(response=response)
         else:
             response_for_status = _status_code_to_response.get(str(response.status))
             if response_for_status:
-                api_response = response_for_status.deserialize(
-                    response, self.api_client.configuration
-                )
+                api_response = response_for_status.deserialize(response, self.api_client.configuration)
             else:
-                api_response = api_client.ApiResponseWithoutDeserialization(
-                    response=response
-                )
+                api_response = api_client.ApiResponseWithoutDeserialization(response=response)
 
         if not 200 <= response.status <= 299:
             raise exceptions.ApiException(
                 status=response.status,
                 reason=response.reason,
-                api_response=api_response,
+                api_response=api_response
             )
 
         return api_response
 
 
 class PipelineRunPost(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
@@ -235,69 +227,73 @@
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: typing_extensions.Literal["application/json"] = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
-        ...
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
 
     @typing.overload
     def pipeline_run_post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
-        ...
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
 
     @typing.overload
     def pipeline_run_post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization:
-        ...
+    ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
     def pipeline_run_post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor200, api_client.ApiResponseWithoutDeserialization,]:
-        ...
+    ) -> typing.Union[
+        ApiResponseFor200,
+        api_client.ApiResponseWithoutDeserialization,
+    ]: ...
 
     def pipeline_run_post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = "application/json",
+        content_type: str = 'application/json',
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         return self._pipeline_run_post_oapg(
             body=body,
             content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
-            skip_deserialization=skip_deserialization,
+            skip_deserialization=skip_deserialization
         )
 
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
@@ -305,63 +301,69 @@
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: typing_extensions.Literal["application/json"] = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
-        ...
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
 
     @typing.overload
     def post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]:
-        ...
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
 
     @typing.overload
     def post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization:
-        ...
+    ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
     def post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
-    ) -> typing.Union[ApiResponseFor200, api_client.ApiResponseWithoutDeserialization,]:
-        ...
+    ) -> typing.Union[
+        ApiResponseFor200,
+        api_client.ApiResponseWithoutDeserialization,
+    ]: ...
 
     def post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = "application/json",
+        content_type: str = 'application/json',
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         return self._pipeline_run_post_oapg(
             body=body,
             content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
-            skip_deserialization=skip_deserialization,
+            skip_deserialization=skip_deserialization
         )
+
+
```

### Comparing `gentrace_py-0.7.4/gentrace/paths/pipeline_run/post.pyi` & `gentrace_py-0.8.0/gentrace/paths/pipeline_run/post.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -27,118 +27,132 @@
 )
 from gentrace.model.pipeline_run_request import PipelineRunRequest
 from gentrace.model.pipeline_run_response import PipelineRunResponse
 
 # body param
 SchemaForRequestBodyApplicationJson = PipelineRunRequest
 
+
 request_body_pipeline_run_request = api_client.RequestBody(
     content={
-        "application/json": api_client.MediaType(
-            schema=SchemaForRequestBodyApplicationJson
-        ),
+        'application/json': api_client.MediaType(
+            schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 SchemaFor200ResponseBodyApplicationJsonCharsetutf8 = PipelineRunResponse
 SchemaFor200ResponseBodyApplicationJson = PipelineRunResponse
 
+
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJsonCharsetutf8,
         SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
+
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
-        "application/json; charset=utf-8": api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJsonCharsetutf8
-        ),
-        "application/json": api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson
-        ),
+        'application/json; charset=utf-8': api_client.MediaType(
+            schema=SchemaFor200ResponseBodyApplicationJsonCharsetutf8),
+        'application/json': api_client.MediaType(
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 
+
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
+
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
 )
 
+
 @dataclass
 class ApiResponseFor500(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
+
 _response_for_500 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor500,
 )
 _all_accept_content_types = (
-    "application/json; charset=utf-8",
-    "application/json",
+    'application/json; charset=utf-8',
+    'application/json',
 )
 
+
 class BaseApi(api_client.Api):
     @typing.overload
     def _pipeline_run_post_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: typing_extensions.Literal["application/json"] = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]: ...
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
     @typing.overload
     def _pipeline_run_post_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]: ...
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+
     @typing.overload
     def _pipeline_run_post_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
+
     @typing.overload
     def _pipeline_run_post_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
+
     def _pipeline_run_post_oapg(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = "application/json",
+        content_type: str = 'application/json',
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
         Create a pipeline run
@@ -148,185 +162,198 @@
         """
         used_path = path.value
 
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
-                _headers.add("Accept", accept_content_type)
+                _headers.add('Accept', accept_content_type)
 
         if body is schemas.unset:
             raise exceptions.ApiValueError(
-                "The required body parameter has an invalid value of: unset. Set a valid value instead"
-            )
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
-        serialized_data = request_body_pipeline_run_request.serialize(
-            body, content_type
-        )
-        _headers.add("Content-Type", content_type)
-        if "fields" in serialized_data:
-            _fields = serialized_data["fields"]
-        elif "body" in serialized_data:
-            _body = serialized_data["body"]
+        serialized_data = request_body_pipeline_run_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']
         response = self.api_client.call_api(
             resource_path=used_path,
-            method="post".upper(),
+            method='post'.upper(),
             headers=_headers,
             fields=_fields,
             body=_body,
             auth_settings=_auth,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
-            api_response = api_client.ApiResponseWithoutDeserialization(
-                response=response
-            )
+            api_response = api_client.ApiResponseWithoutDeserialization(response=response)
         else:
             response_for_status = _status_code_to_response.get(str(response.status))
             if response_for_status:
-                api_response = response_for_status.deserialize(
-                    response, self.api_client.configuration
-                )
+                api_response = response_for_status.deserialize(response, self.api_client.configuration)
             else:
-                api_response = api_client.ApiResponseWithoutDeserialization(
-                    response=response
-                )
+                api_response = api_client.ApiResponseWithoutDeserialization(response=response)
 
         if not 200 <= response.status <= 299:
             raise exceptions.ApiException(
                 status=response.status,
                 reason=response.reason,
-                api_response=api_response,
+                api_response=api_response
             )
 
         return api_response
 
+
 class PipelineRunPost(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
     def pipeline_run_post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: typing_extensions.Literal["application/json"] = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]: ...
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
     @typing.overload
     def pipeline_run_post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]: ...
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+
     @typing.overload
     def pipeline_run_post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
+
     @typing.overload
     def pipeline_run_post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
+
     def pipeline_run_post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = "application/json",
+        content_type: str = 'application/json',
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         return self._pipeline_run_post_oapg(
             body=body,
             content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
-            skip_deserialization=skip_deserialization,
+            skip_deserialization=skip_deserialization
         )
 
+
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
     def post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: typing_extensions.Literal["application/json"] = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]: ...
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
     @typing.overload
     def post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[ApiResponseFor200,]: ...
+    ) -> typing.Union[
+        ApiResponseFor200,
+    ]: ...
+
+
     @typing.overload
     def post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> api_client.ApiResponseWithoutDeserialization: ...
+
     @typing.overload
     def post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
         content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]: ...
+
     def post(
         self,
         body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = "application/json",
+        content_type: str = 'application/json',
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         return self._pipeline_run_post_oapg(
             body=body,
             content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
-            skip_deserialization=skip_deserialization,
+            skip_deserialization=skip_deserialization
         )
+
+
```

### Comparing `gentrace_py-0.7.4/gentrace/providers/getters.py` & `gentrace_py-0.8.0/gentrace/providers/getters.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.4/gentrace/providers/llms/openai.py` & `gentrace_py-0.8.0/gentrace/providers/llms/openai.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.4/gentrace/providers/pipeline.py` & `gentrace_py-0.8.0/gentrace/providers/pipeline.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.4/gentrace/providers/pipeline_run.py` & `gentrace_py-0.8.0/gentrace/providers/pipeline_run.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import copy
 import inspect
 import threading
 import uuid
 from typing import Dict, List, Optional, cast
 
 from gentrace.api_client import ApiClient
-from gentrace.apis.tags.ingestion_api import IngestionApi
+from gentrace.apis.tags.core_api import CoreApi
 from gentrace.configuration import Configuration
 from gentrace.providers.pipeline import Pipeline
 from gentrace.providers.step_run import StepRun
 from gentrace.providers.utils import pipeline_run_post_background
 
 _pipeline_run_loop = None
 _pipeline_tasks = []
@@ -84,15 +84,15 @@
     def add_step_run(self, step_run: StepRun):
         self.step_runs.append(step_run)
 
     async def asubmit(self) -> Dict:
         configuration = Configuration(host=self.pipeline.config.get("host"))
         configuration.access_token = self.pipeline.config.get("api_key")
         api_client = ApiClient(configuration=configuration)
-        ingestion_api = IngestionApi(api_client=api_client)
+        core_api = CoreApi(api_client=api_client)
 
         step_runs_data = [
             {
                 "provider": {
                     "name": step_run.provider,
                     "invocation": step_run.invocation,
                     "modelParams": step_run.model_params,
@@ -106,15 +106,15 @@
             for step_run in self.step_runs
         ]
 
         pipeline_run_id = str(uuid.uuid4())
 
         try:
             pipeline_post_response = await pipeline_run_post_background(
-                ingestion_api,
+                core_api,
                 {
                     "id": pipeline_run_id,
                     "name": self.pipeline.id,
                     "stepRuns": step_runs_data,
                 },
             )
             return {
@@ -127,15 +127,15 @@
             return {"pipelineRunId": None}
 
     def submit(self, wait_for_server=False) -> Dict:
         configuration = Configuration(host=self.pipeline.config.get("host"))
         configuration.access_token = self.pipeline.config.get("api_key")
 
         api_client = ApiClient(configuration=configuration)
-        ingestion_api = IngestionApi(api_client=api_client)
+        core_api = CoreApi(api_client=api_client)
 
         step_runs_data = [
             {
                 "provider": {
                     "name": step_run.provider,
                     "invocation": step_run.invocation,
                     "modelParams": step_run.model_params,
@@ -151,28 +151,28 @@
 
         if len(step_runs_data) == 0:
             return {"pipelineRunId": None}
 
         if not wait_for_server:
             fire_and_forget(
                 pipeline_run_post_background(
-                    ingestion_api,
+                    core_api,
                     {
                         "id": self.pipeline_run_id,
                         "name": self.pipeline.id,
                         "stepRuns": step_runs_data,
                     },
                 )
             )
 
             return {"pipelineRunId": self.pipeline_run_id}
 
         if wait_for_server:
             try:
-                pipeline_post_response = ingestion_api.pipeline_run_post(
+                pipeline_post_response = core_api.pipeline_run_post(
                     {
                         "id": self.pipeline_run_id,
                         "name": self.pipeline.id,
                         "stepRuns": step_runs_data,
                     }
                 )
                 return {
```

### Comparing `gentrace_py-0.7.4/gentrace/providers/step_run.py` & `gentrace_py-0.8.0/gentrace/providers/step_run.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.4/gentrace/providers/utils.py` & `gentrace_py-0.8.0/gentrace/providers/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import logging
 import re
 import sys
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
 
-from gentrace.apis.tags.ingestion_api import IngestionApi
+from gentrace.apis.tags.core_api import CoreApi
 from gentrace.models import PipelineRunRequest
 
 __all__ = [
     "to_date_string",
     "pipeline_run_post_background",
     "log_debug",
     "log_info",
@@ -114,15 +114,15 @@
             key = repr(key)
         return "{key}={val}".format(key=key, val=val)
 
     return " ".join([fmt(key, val) for key, val in sorted(props.items())])
 
 
 async def pipeline_run_post_background(
-    api_instance: IngestionApi, pipeline_run_data: PipelineRunRequest
+    api_instance: CoreApi, pipeline_run_data: PipelineRunRequest
 ):
     def wrapped_api_invocation():
         try:
             log_info("Submitting PipelineRun to Gentrace")
             result = api_instance.pipeline_run_post(pipeline_run_data)
             log_info("Successfully submitted PipelineRun to Gentrace")
             return result
```

### Comparing `gentrace_py-0.7.4/gentrace/providers/vectorstores/pinecone.py` & `gentrace_py-0.8.0/gentrace/providers/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gentrace_py-0.7.4/gentrace/rest.py` & `gentrace_py-0.8.0/gentrace/rest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.8
+    The version of the OpenAPI document: 0.4.13
     Generated by: https://openapi-generator.tech
 """
 
 import logging
 import ssl
 import typing
 from urllib.parse import urlencode
@@ -20,14 +20,15 @@
 
 from gentrace.exceptions import ApiException, ApiValueError
 
 logger = logging.getLogger(__name__)
 
 
 class RESTClientObject(object):
+
     def __init__(self, configuration, pools_size=4, maxsize=None):
         # urllib3.PoolManager will pass all kw parameters to connectionpool
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/connectionpool.py#L680  # noqa: E501
         # maxsize is the number of requests to host that are allowed in parallel  # noqa: E501
         # Custom SSL certificates and client certificates: http://urllib3.readthedocs.io/en/latest/advanced-usage.html  # noqa: E501
 
@@ -42,23 +43,21 @@
             ca_certs = configuration.ssl_ca_cert
         else:
             # if not set certificate file, use Mozilla's root certificates.
             ca_certs = certifi.where()
 
         addition_pool_args = {}
         if configuration.assert_hostname is not None:
-            addition_pool_args[
-                "assert_hostname"
-            ] = configuration.assert_hostname  # noqa: E501
+            addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
 
         if configuration.retries is not None:
-            addition_pool_args["retries"] = configuration.retries
+            addition_pool_args['retries'] = configuration.retries
 
         if configuration.socket_options is not None:
-            addition_pool_args["socket_options"] = configuration.socket_options
+            addition_pool_args['socket_options'] = configuration.socket_options
 
         if maxsize is None:
             if configuration.connection_pool_maxsize is not None:
                 maxsize = configuration.connection_pool_maxsize
             else:
                 maxsize = 4
 
@@ -87,17 +86,15 @@
             )
 
     def request(
         self,
         method: str,
         url: str,
         headers: typing.Optional[HTTPHeaderDict] = None,
-        fields: typing.Optional[
-            typing.Tuple[typing.Tuple[str, typing.Any], ...]
-        ] = None,
+        fields: typing.Optional[typing.Tuple[typing.Tuple[str, typing.Any], ...]] = None,
         body: typing.Optional[typing.Union[str, bytes]] = None,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
     ) -> urllib3.HTTPResponse:
         """Perform requests.
 
         :param method: http request method
@@ -112,175 +109,145 @@
                                 data. Default is False.
         :param timeout: timeout setting for this request. If one
                                 number provided, it will be total request
                                 timeout. It can also be a pair (tuple) of
                                 (connection, read) timeouts.
         """
         method = method.upper()
-        assert method in ["GET", "HEAD", "DELETE", "POST", "PUT", "PATCH", "OPTIONS"]
+        assert method in ['GET', 'HEAD', 'DELETE', 'POST', 'PUT',
+                          'PATCH', 'OPTIONS']
 
         if fields and body:
-            raise ApiValueError("body parameter cannot be used with fields parameter.")
+            raise ApiValueError(
+                "body parameter cannot be used with fields parameter."
+            )
 
         fields = fields or {}
         headers = headers or {}
 
         if timeout:
             if isinstance(timeout, (int, float)):  # noqa: E501,F821
                 timeout = urllib3.Timeout(total=timeout)
-            elif isinstance(timeout, tuple) and len(timeout) == 2:
+            elif (isinstance(timeout, tuple) and
+                  len(timeout) == 2):
                 timeout = urllib3.Timeout(connect=timeout[0], read=timeout[1])
 
         try:
             # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
-            if method in ["POST", "PUT", "PATCH", "OPTIONS", "DELETE"]:
-                if "Content-Type" not in headers and body is None:
+            if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
+                if 'Content-Type' not in headers and body is None:
                     r = self.pool_manager.request(
                         method,
                         url,
                         preload_content=not stream,
                         timeout=timeout,
-                        headers=headers,
+                        headers=headers
                     )
-                elif (
-                    headers["Content-Type"] == "application/x-www-form-urlencoded"
-                ):  # noqa: E501
+                elif headers['Content-Type'] == 'application/x-www-form-urlencoded':  # noqa: E501
                     r = self.pool_manager.request(
-                        method,
-                        url,
+                        method, url,
                         body=body,
                         fields=fields,
                         encode_multipart=False,
                         preload_content=not stream,
                         timeout=timeout,
-                        headers=headers,
-                    )
-                elif headers["Content-Type"] == "multipart/form-data":
+                        headers=headers)
+                elif headers['Content-Type'] == 'multipart/form-data':
                     # must del headers['Content-Type'], or the correct
                     # Content-Type which generated by urllib3 will be
                     # overwritten.
-                    del headers["Content-Type"]
+                    del headers['Content-Type']
                     r = self.pool_manager.request(
-                        method,
-                        url,
+                        method, url,
                         fields=fields,
                         encode_multipart=True,
                         preload_content=not stream,
                         timeout=timeout,
-                        headers=headers,
-                    )
+                        headers=headers)
                 # Pass a `string` parameter directly in the body to support
                 # other content types than Json when `body` argument is
                 # provided in serialized form
                 elif isinstance(body, str) or isinstance(body, bytes):
                     request_body = body
                     r = self.pool_manager.request(
-                        method,
-                        url,
+                        method, url,
                         body=request_body,
                         preload_content=not stream,
                         timeout=timeout,
-                        headers=headers,
-                    )
+                        headers=headers)
                 else:
                     # Cannot generate the request from given parameters
                     msg = """Cannot prepare a request message for provided
                              arguments. Please check that your arguments match
                              declared content type."""
                     raise ApiException(status=0, reason=msg)
             # For `GET`, `HEAD`
             else:
-                r = self.pool_manager.request(
-                    method,
-                    url,
-                    preload_content=not stream,
-                    timeout=timeout,
-                    headers=headers,
-                )
+                r = self.pool_manager.request(method, url,
+                                              preload_content=not stream,
+                                              timeout=timeout,
+                                              headers=headers)
         except urllib3.exceptions.SSLError as e:
             msg = "{0}\n{1}".format(type(e).__name__, str(e))
             raise ApiException(status=0, reason=msg)
 
         if not stream:
             # log response body
             logger.debug("response body: %s", r.data)
 
         return r
 
-    def GET(
-        self, url, headers=None, stream=False, timeout=None, fields=None
-    ) -> urllib3.HTTPResponse:
-        return self.request(
-            "GET", url, headers=headers, stream=stream, timeout=timeout, fields=fields
-        )
-
-    def HEAD(
-        self, url, headers=None, stream=False, timeout=None, fields=None
-    ) -> urllib3.HTTPResponse:
-        return self.request(
-            "HEAD", url, headers=headers, stream=stream, timeout=timeout, fields=fields
-        )
-
-    def OPTIONS(
-        self, url, headers=None, body=None, stream=False, timeout=None, fields=None
-    ) -> urllib3.HTTPResponse:
-        return self.request(
-            "OPTIONS",
-            url,
-            headers=headers,
-            stream=stream,
-            timeout=timeout,
-            body=body,
-            fields=fields,
-        )
-
-    def DELETE(
-        self, url, headers=None, body=None, stream=False, timeout=None, fields=None
-    ) -> urllib3.HTTPResponse:
-        return self.request(
-            "DELETE",
-            url,
-            headers=headers,
-            stream=stream,
-            timeout=timeout,
-            body=body,
-            fields=fields,
-        )
-
-    def POST(
-        self, url, headers=None, body=None, stream=False, timeout=None, fields=None
-    ) -> urllib3.HTTPResponse:
-        return self.request(
-            "POST",
-            url,
-            headers=headers,
-            stream=stream,
-            timeout=timeout,
-            body=body,
-            fields=fields,
-        )
-
-    def PUT(
-        self, url, headers=None, body=None, stream=False, timeout=None, fields=None
-    ) -> urllib3.HTTPResponse:
-        return self.request(
-            "PUT",
-            url,
-            headers=headers,
-            stream=stream,
-            timeout=timeout,
-            body=body,
-            fields=fields,
-        )
-
-    def PATCH(
-        self, url, headers=None, body=None, stream=False, timeout=None, fields=None
-    ) -> urllib3.HTTPResponse:
-        return self.request(
-            "PATCH",
-            url,
-            headers=headers,
-            stream=stream,
-            timeout=timeout,
-            body=body,
-            fields=fields,
-        )
+    def GET(self, url, headers=None, stream=False,
+            timeout=None, fields=None) -> urllib3.HTTPResponse:
+        return self.request("GET", url,
+                            headers=headers,
+                            stream=stream,
+                            timeout=timeout,
+                            fields=fields)
+
+    def HEAD(self, url, headers=None, stream=False,
+             timeout=None, fields=None) -> urllib3.HTTPResponse:
+        return self.request("HEAD", url,
+                            headers=headers,
+                            stream=stream,
+                            timeout=timeout,
+                            fields=fields)
+
+    def OPTIONS(self, url, headers=None,
+                body=None, stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
+        return self.request("OPTIONS", url,
+                            headers=headers,
+                            stream=stream,
+                            timeout=timeout,
+                            body=body, fields=fields)
+
+    def DELETE(self, url, headers=None, body=None,
+               stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
+        return self.request("DELETE", url,
+                            headers=headers,
+                            stream=stream,
+                            timeout=timeout,
+                            body=body, fields=fields)
+
+    def POST(self, url, headers=None,
+             body=None, stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
+        return self.request("POST", url,
+                            headers=headers,
+                            stream=stream,
+                            timeout=timeout,
+                            body=body, fields=fields)
+
+    def PUT(self, url, headers=None,
+            body=None, stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
+        return self.request("PUT", url,
+                            headers=headers,
+                            stream=stream,
+                            timeout=timeout,
+                            body=body, fields=fields)
+
+    def PATCH(self, url, headers=None,
+              body=None, stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
+        return self.request("PATCH", url,
+                            headers=headers,
+                            stream=stream,
+                            timeout=timeout,
+                            body=body, fields=fields)
```

### Comparing `gentrace_py-0.7.4/gentrace/schemas.py` & `gentrace_py-0.8.0/gentrace/schemas.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gentrace API
 
     These API routes are designed to ingest events from clients.  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.8
+    The version of the OpenAPI document: 0.4.13
     Generated by: https://openapi-generator.tech
 """
 
 import decimal
 import functools
 import io
 import re
@@ -32,18 +32,16 @@
 
 
 class Unset(object):
     """
     An instance of this class is set as the default value for object type(dict) properties that are optional
     When a property has an unset value, that property will not be assigned in the dict
     """
-
     pass
 
-
 unset = Unset()
 
 none_type = type(None)
 file_type = io.IOBase
 
 
 class FileIO(io.FileIO):
@@ -51,22 +49,20 @@
     A class for storing files
     Note: this class is not immutable
     """
 
     def __new__(cls, _arg: typing.Union[io.FileIO, io.BufferedReader]):
         if isinstance(_arg, (io.FileIO, io.BufferedReader)):
             if _arg.closed:
-                raise ApiValueError(
-                    "Invalid file state; file is closed and must be open"
-                )
+                raise ApiValueError('Invalid file state; file is closed and must be open')
             _arg.close()
             inst = super(FileIO, cls).__new__(cls, _arg.name)
             super(FileIO, inst).__init__(_arg.name)
             return inst
-        raise ApiValueError("FileIO must be passed _arg which contains the open file")
+        raise ApiValueError('FileIO must be passed _arg which contains the open file')
 
     def __init__(self, _arg: typing.Union[io.FileIO, io.BufferedReader]):
         pass
 
 
 def update(d: dict, u: dict):
     """
@@ -82,24 +78,21 @@
             d[k] = d[k] | v
 
 
 class ValidationMetadata(frozendict.frozendict):
     """
     A class storing metadata that is needed to validate OpenApi Schema payloads
     """
-
     def __new__(
         cls,
-        path_to_item: typing.Tuple[typing.Union[str, int], ...] = tuple(["args[0]"]),
+        path_to_item: typing.Tuple[typing.Union[str, int], ...] = tuple(['args[0]']),
         from_server: bool = False,
         configuration: typing.Optional[Configuration] = None,
         seen_classes: typing.FrozenSet[typing.Type] = frozenset(),
-        validated_path_to_schemas: typing.Dict[
-            typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Type]
-        ] = frozendict.frozendict(),
+        validated_path_to_schemas: typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Type]] = frozendict.frozendict()
     ):
         """
         Args:
             path_to_item: the path to the current data being instantiated.
                 For {'a': [1]} if the code is handling, 1, then the path is ('args[0]', 'a', 0)
                 This changes from location to location
             from_server: whether or not this data came form the server
@@ -118,74 +111,65 @@
         """
         return super().__new__(
             cls,
             path_to_item=path_to_item,
             from_server=from_server,
             configuration=configuration,
             seen_classes=seen_classes,
-            validated_path_to_schemas=validated_path_to_schemas,
+            validated_path_to_schemas=validated_path_to_schemas
         )
 
     def validation_ran_earlier(self, cls: type) -> bool:
         validated_schemas = self.validated_path_to_schemas.get(self.path_to_item, set())
         validation_ran_earlier = validated_schemas and cls in validated_schemas
         if validation_ran_earlier:
             return True
         if cls in self.seen_classes:
             return True
         return False
 
     @property
     def path_to_item(self) -> typing.Tuple[typing.Union[str, int], ...]:
-        return self.get("path_to_item")
+        return self.get('path_to_item')
 
     @property
     def from_server(self) -> bool:
-        return self.get("from_server")
+        return self.get('from_server')
 
     @property
     def configuration(self) -> typing.Optional[Configuration]:
-        return self.get("configuration")
+        return self.get('configuration')
 
     @property
     def seen_classes(self) -> typing.FrozenSet[typing.Type]:
-        return self.get("seen_classes")
+        return self.get('seen_classes')
 
     @property
-    def validated_path_to_schemas(
-        self,
-    ) -> typing.Dict[
-        typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Type]
-    ]:
-        return self.get("validated_path_to_schemas")
+    def validated_path_to_schemas(self) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Type]]:
+        return self.get('validated_path_to_schemas')
 
 
-def add_deeper_validated_schemas(
-    validation_metadata: ValidationMetadata, path_to_schemas: dict
-):
+def add_deeper_validated_schemas(validation_metadata: ValidationMetadata, path_to_schemas: dict):
     # this is called if validation_ran_earlier and current and deeper locations need to be added
     current_path_to_item = validation_metadata.path_to_item
     other_path_to_schemas = {}
     for path_to_item, schemas in validation_metadata.validated_path_to_schemas.items():
         if len(path_to_item) < len(current_path_to_item):
             continue
-        path_begins_with_current_path = (
-            path_to_item[: len(current_path_to_item)] == current_path_to_item
-        )
+        path_begins_with_current_path = path_to_item[:len(current_path_to_item)] == current_path_to_item
         if path_begins_with_current_path:
             other_path_to_schemas[path_to_item] = schemas
     update(path_to_schemas, other_path_to_schemas)
 
 
 class Singleton:
     """
     Enums and singletons are the same
     The same instance is returned for a given key of (cls, _arg)
     """
-
     _instances = {}
 
     def __new__(cls, _arg: typing.Any, **kwargs):
         """
         cls base classes: BoolClass, NoneClass, str, decimal.Decimal
         The 3rd key is used in the tuple below for a corner case where an enum contains integer 1
         However 1.0  can also be ingested into that enum schema because 1.0 == 1 and
@@ -201,23 +185,24 @@
                 cls._instances[key] = inst
             else:
                 cls._instances[key] = super().__new__(cls, _arg)
         return cls._instances[key]
 
     def __repr__(self):
         if isinstance(self, NoneClass):
-            return f"<{self.__class__.__name__}: None>"
+            return f'<{self.__class__.__name__}: None>'
         elif isinstance(self, BoolClass):
             if bool(self):
-                return f"<{self.__class__.__name__}: True>"
-            return f"<{self.__class__.__name__}: False>"
-        return f"<{self.__class__.__name__}: {super().__repr__()}>"
+                return f'<{self.__class__.__name__}: True>'
+            return f'<{self.__class__.__name__}: False>'
+        return f'<{self.__class__.__name__}: {super().__repr__()}>'
 
 
 class classproperty:
+
     def __init__(self, fget):
         self.fget = fget
 
     def __get__(self, owner_self, owner_cls):
         return self.fget(owner_cls)
 
 
@@ -240,74 +225,63 @@
         return cls(False)
 
     @functools.lru_cache()
     def __bool__(self) -> bool:
         for key, instance in self._instances.items():
             if self is instance:
                 return bool(key[1])
-        raise ValueError("Unable to find the boolean value of this instance")
+        raise ValueError('Unable to find the boolean value of this instance')
 
 
 class MetaOapgTyped:
     exclusive_maximum: typing.Union[int, float]
     inclusive_maximum: typing.Union[int, float]
     exclusive_minimum: typing.Union[int, float]
     inclusive_minimum: typing.Union[int, float]
     max_items: int
     min_items: int
-    discriminator: typing.Dict[str, typing.Dict[str, typing.Type["Schema"]]]
+    discriminator: typing.Dict[str, typing.Dict[str, typing.Type['Schema']]]
+
 
     class properties:
         # to hold object properties
         pass
 
-    additional_properties: typing.Optional[typing.Type["Schema"]]
+    additional_properties: typing.Optional[typing.Type['Schema']]
     max_properties: int
     min_properties: int
-    all_of: typing.List[typing.Type["Schema"]]
-    one_of: typing.List[typing.Type["Schema"]]
-    any_of: typing.List[typing.Type["Schema"]]
-    not_schema: typing.Type["Schema"]
+    all_of: typing.List[typing.Type['Schema']]
+    one_of: typing.List[typing.Type['Schema']]
+    any_of: typing.List[typing.Type['Schema']]
+    not_schema: typing.Type['Schema']
     max_length: int
     min_length: int
-    items: typing.Type["Schema"]
+    items: typing.Type['Schema']
 
 
 class Schema:
     """
     the base class of all swagger/openapi schemas/models
     """
-
-    __inheritable_primitive_types_set = {
-        decimal.Decimal,
-        str,
-        tuple,
-        frozendict.frozendict,
-        FileIO,
-        bytes,
-        BoolClass,
-        NoneClass,
-    }
+    __inheritable_primitive_types_set = {decimal.Decimal, str, tuple, frozendict.frozendict, FileIO, bytes, BoolClass, NoneClass}
     _types: typing.Set[typing.Type]
     MetaOapg = MetaOapgTyped
 
     @staticmethod
     def __get_valid_classes_phrase(input_classes):
         """Returns a string phrase describing what types are allowed"""
         all_classes = list(input_classes)
         all_classes = sorted(all_classes, key=lambda cls: cls.__name__)
         all_class_names = [cls.__name__ for cls in all_classes]
         if len(all_class_names) == 1:
             return "is {0}".format(all_class_names[0])
         return "is one of [{0}]".format(", ".join(all_class_names))
 
     @staticmethod
-    def _get_class_oapg(
-        item_cls: typing.Union[types.FunctionType, staticmethod, typing.Type["Schema"]]
-    ) -> typing.Type["Schema"]:
+    def _get_class_oapg(item_cls: typing.Union[types.FunctionType, staticmethod, typing.Type['Schema']]) -> typing.Type['Schema']:
         if isinstance(item_cls, types.FunctionType):
             # referenced schema
             return item_cls()
         elif isinstance(item_cls, staticmethod):
             # referenced schema
             return item_cls.__func__()
         return item_cls
@@ -354,28 +328,15 @@
         )
 
     @classmethod
     def _validate_oapg(
         cls,
         arg,
         validation_metadata: ValidationMetadata,
-    ) -> typing.Dict[
-        typing.Tuple[typing.Union[str, int], ...],
-        typing.Set[
-            typing.Union[
-                "Schema",
-                str,
-                decimal.Decimal,
-                BoolClass,
-                NoneClass,
-                frozendict.frozendict,
-                tuple,
-            ]
-        ],
-    ]:
+    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]]:
         """
         Schema _validate_oapg
         All keyword validation except for type checking was done in calling stack frames
         If those validations passed, the validated classes are collected in path_to_schemas
 
         Returns:
             path_to_schemas: a map of path to schemas
@@ -396,25 +357,15 @@
         path_to_schemas = {validation_metadata.path_to_item: set()}
         path_to_schemas[validation_metadata.path_to_item].add(cls)
         path_to_schemas[validation_metadata.path_to_item].add(base_class)
         return path_to_schemas
 
     @staticmethod
     def _process_schema_classes_oapg(
-        schema_classes: typing.Set[
-            typing.Union[
-                "Schema",
-                str,
-                decimal.Decimal,
-                BoolClass,
-                NoneClass,
-                frozendict.frozendict,
-                tuple,
-            ]
-        ]
+        schema_classes: typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]
     ):
         """
         Processes and mutates schema_classes
         If a SomeSchema is a subclass of DictSchema then remove DictSchema because it is already included
         """
         if len(schema_classes) < 2:
             return
@@ -426,16 +377,18 @@
         x_schema = x_schema.pop()
         if any(c is not x_schema and issubclass(c, x_schema) for c in schema_classes):
             # needed to not have a mro error in get_new_class
             schema_classes.remove(x_schema)
 
     @classmethod
     def __get_new_cls(
-        cls, arg, validation_metadata: ValidationMetadata
-    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Type["Schema"]]:
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata
+    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Type['Schema']]:
         """
         Make a new dynamic class and return an instance of that class
         We are making an instance of cls, but instead of making cls
         make a new class, new_cls
         which includes dynamic bases including cls
         return an instance of that new class
 
@@ -451,17 +404,15 @@
             and in list/dict _get_items_oapg,_get_properties_oapg the value will be directly assigned
             because value is of the correct type, and validation was run earlier when the instance was created
         """
         _path_to_schemas = {}
         if validation_metadata.validation_ran_earlier(cls):
             add_deeper_validated_schemas(validation_metadata, _path_to_schemas)
         else:
-            other_path_to_schemas = cls._validate_oapg(
-                arg, validation_metadata=validation_metadata
-            )
+            other_path_to_schemas = cls._validate_oapg(arg, validation_metadata=validation_metadata)
             update(_path_to_schemas, other_path_to_schemas)
         # loop through it make a new class for each entry
         # do not modify the returned result because it is cached and we would be modifying the cached value
         path_to_schemas = {}
         for path, schema_classes in _path_to_schemas.items():
             """
             Use cases
@@ -469,41 +420,33 @@
                 needs Singleton added
             2. N number of schema classes + enum + type == bool/None, classes in path_to_schemas: BoolClass/NoneClass
                 Singleton already added
             3. N number of schema classes, classes in path_to_schemas: BoolClass/NoneClass/tuple/frozendict.frozendict/str/Decimal/bytes/FileIo
             """
             cls._process_schema_classes_oapg(schema_classes)
             enum_schema = any(
-                issubclass(this_cls, EnumBase) for this_cls in schema_classes
-            )
-            inheritable_primitive_type = schema_classes.intersection(
-                cls.__inheritable_primitive_types_set
-            )
+                issubclass(this_cls, EnumBase) for this_cls in schema_classes)
+            inheritable_primitive_type = schema_classes.intersection(cls.__inheritable_primitive_types_set)
             chosen_schema_classes = schema_classes - inheritable_primitive_type
             suffix = tuple(inheritable_primitive_type)
             if enum_schema and suffix[0] not in {NoneClass, BoolClass}:
                 suffix = (Singleton,) + suffix
 
-            used_classes = (
-                tuple(sorted(chosen_schema_classes, key=lambda a_cls: a_cls.__name__))
-                + suffix
-            )
-            mfg_cls = get_new_class(class_name="DynamicSchema", bases=used_classes)
+            used_classes = tuple(sorted(chosen_schema_classes, key=lambda a_cls: a_cls.__name__)) + suffix
+            mfg_cls = get_new_class(class_name='DynamicSchema', bases=used_classes)
             path_to_schemas[path] = mfg_cls
 
         return path_to_schemas
 
     @classmethod
     def _get_new_instance_without_conversion_oapg(
         cls,
         arg: typing.Any,
         path_to_item: typing.Tuple[typing.Union[str, int], ...],
-        path_to_schemas: typing.Dict[
-            typing.Tuple[typing.Union[str, int], ...], typing.Type["Schema"]
-        ],
+        path_to_schemas: typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Type['Schema']]
     ):
         # We have a Dynamic class and we are making an instance of it
         if issubclass(cls, frozendict.frozendict) and issubclass(cls, DictBase):
             properties = cls._get_properties_oapg(arg, path_to_item, path_to_schemas)
             return super(Schema, cls).__new__(cls, properties)
         elif issubclass(cls, tuple) and issubclass(cls, ListBase):
             items = cls._get_items_oapg(arg, path_to_item, path_to_schemas)
@@ -524,40 +467,39 @@
             date,
             datetime,
             int,
             float,
             decimal.Decimal,
             bool,
             None,
-            "Schema",
+            'Schema',
             dict,
             frozendict.frozendict,
             tuple,
             list,
             io.FileIO,
             io.BufferedReader,
-            bytes,
+            bytes
         ],
-        _configuration: typing.Optional[Configuration],
+        _configuration: typing.Optional[Configuration]
     ):
         """
         Schema from_openapi_data_oapg
         """
         from_server = True
         validated_path_to_schemas = {}
         arg = cast_to_allowed_types(arg, from_server, validated_path_to_schemas)
         validation_metadata = ValidationMetadata(
-            from_server=from_server,
-            configuration=_configuration,
-            validated_path_to_schemas=validated_path_to_schemas,
-        )
+            from_server=from_server, configuration=_configuration, validated_path_to_schemas=validated_path_to_schemas)
         path_to_schemas = cls.__get_new_cls(arg, validation_metadata)
         new_cls = path_to_schemas[validation_metadata.path_to_item]
         new_inst = new_cls._get_new_instance_without_conversion_oapg(
-            arg, validation_metadata.path_to_item, path_to_schemas
+            arg,
+            validation_metadata.path_to_item,
+            path_to_schemas
         )
         return new_inst
 
     @staticmethod
     def __get_input_dict(*args, **kwargs) -> frozendict.frozendict:
         input_dict = {}
         if args and isinstance(args[0], (dict, frozendict.frozendict)):
@@ -566,126 +508,67 @@
             input_dict.update(kwargs)
         return frozendict.frozendict(input_dict)
 
     @staticmethod
     def __remove_unsets(kwargs):
         return {key: val for key, val in kwargs.items() if val is not unset}
 
-    def __new__(
-        cls,
-        *_args: typing.Union[
-            dict,
-            frozendict.frozendict,
-            list,
-            tuple,
-            decimal.Decimal,
-            float,
-            int,
-            str,
-            date,
-            datetime,
-            bool,
-            None,
-            "Schema",
-        ],
-        _configuration: typing.Optional[Configuration] = None,
-        **kwargs: typing.Union[
-            dict,
-            frozendict.frozendict,
-            list,
-            tuple,
-            decimal.Decimal,
-            float,
-            int,
-            str,
-            date,
-            datetime,
-            bool,
-            None,
-            "Schema",
-            Unset,
-        ],
-    ):
+    def __new__(cls, *_args: typing.Union[dict, frozendict.frozendict, list, tuple, decimal.Decimal, float, int, str, date, datetime, bool, None, 'Schema'], _configuration: typing.Optional[Configuration] = None, **kwargs: typing.Union[dict, frozendict.frozendict, list, tuple, decimal.Decimal, float, int, str, date, datetime, bool, None, 'Schema', Unset]):
         """
         Schema __new__
 
         Args:
             _args (int/float/decimal.Decimal/str/list/tuple/dict/frozendict.frozendict/bool/None): the value
             kwargs (str, int/float/decimal.Decimal/str/list/tuple/dict/frozendict.frozendict/bool/None): dict values
             _configuration: contains the Configuration that enables json schema validation keywords
                 like minItems, minLength etc
 
         Note: double underscores are used here because pycharm thinks that these variables
         are instance properties if they are named normally :(
         """
         __kwargs = cls.__remove_unsets(kwargs)
         if not _args and not __kwargs:
-            raise TypeError("No input given. args or kwargs must be given.")
+            raise TypeError(
+                'No input given. args or kwargs must be given.'
+            )
         if not __kwargs and _args and not isinstance(_args[0], dict):
             __arg = _args[0]
         else:
             __arg = cls.__get_input_dict(*_args, **__kwargs)
         __from_server = False
         __validated_path_to_schemas = {}
-        __arg = cast_to_allowed_types(__arg, __from_server, __validated_path_to_schemas)
+        __arg = cast_to_allowed_types(
+            __arg, __from_server, __validated_path_to_schemas)
         __validation_metadata = ValidationMetadata(
-            configuration=_configuration,
-            from_server=__from_server,
-            validated_path_to_schemas=__validated_path_to_schemas,
-        )
+            configuration=_configuration, from_server=__from_server, validated_path_to_schemas=__validated_path_to_schemas)
         __path_to_schemas = cls.__get_new_cls(__arg, __validation_metadata)
         __new_cls = __path_to_schemas[__validation_metadata.path_to_item]
         return __new_cls._get_new_instance_without_conversion_oapg(
-            __arg, __validation_metadata.path_to_item, __path_to_schemas
+            __arg,
+            __validation_metadata.path_to_item,
+            __path_to_schemas
         )
 
     def __init__(
         self,
         *_args: typing.Union[
-            dict,
-            frozendict.frozendict,
-            list,
-            tuple,
-            decimal.Decimal,
-            float,
-            int,
-            str,
-            date,
-            datetime,
-            bool,
-            None,
-            "Schema",
-        ],
+            dict, frozendict.frozendict, list, tuple, decimal.Decimal, float, int, str, date, datetime, bool, None, 'Schema'],
         _configuration: typing.Optional[Configuration] = None,
         **kwargs: typing.Union[
-            dict,
-            frozendict.frozendict,
-            list,
-            tuple,
-            decimal.Decimal,
-            float,
-            int,
-            str,
-            date,
-            datetime,
-            bool,
-            None,
-            "Schema",
-            Unset,
-        ],
+            dict, frozendict.frozendict, list, tuple, decimal.Decimal, float, int, str, date, datetime, bool, None, 'Schema', Unset
+        ]
     ):
         """
         this is needed to fix 'Unexpected argument' warning in pycharm
         this code does nothing because all Schema instances are immutable
         this means that all input data is passed into and used in new, and after the new instance is made
         no new attributes are assigned and init is not used
         """
         pass
 
-
 """
 import itertools
 data_types = ('None', 'FrozenDict', 'Tuple', 'Str', 'Decimal', 'Bool')
 type_to_cls = {
     'None': 'NoneClass',
     'FrozenDict': 'frozendict.frozendict',
     'Tuple': 'tuple',
@@ -707,459 +590,280 @@
     FrozenDictMixin = frozendict.frozendict
     TupleMixin = tuple
     StrMixin = str
     DecimalMixin = decimal.Decimal
     BoolMixin = BoolClass
     BytesMixin = bytes
     FileMixin = FileIO
-
     # qty 2
     class BinaryMixin(bytes, FileIO):
         pass
-
     class NoneFrozenDictMixin(NoneClass, frozendict.frozendict):
         pass
-
     class NoneTupleMixin(NoneClass, tuple):
         pass
-
     class NoneStrMixin(NoneClass, str):
         pass
-
     class NoneDecimalMixin(NoneClass, decimal.Decimal):
         pass
-
     class NoneBoolMixin(NoneClass, BoolClass):
         pass
-
     class FrozenDictTupleMixin(frozendict.frozendict, tuple):
         pass
-
     class FrozenDictStrMixin(frozendict.frozendict, str):
         pass
-
     class FrozenDictDecimalMixin(frozendict.frozendict, decimal.Decimal):
         pass
-
     class FrozenDictBoolMixin(frozendict.frozendict, BoolClass):
         pass
-
     class TupleStrMixin(tuple, str):
         pass
-
     class TupleDecimalMixin(tuple, decimal.Decimal):
         pass
-
     class TupleBoolMixin(tuple, BoolClass):
         pass
-
     class StrDecimalMixin(str, decimal.Decimal):
         pass
-
     class StrBoolMixin(str, BoolClass):
         pass
-
     class DecimalBoolMixin(decimal.Decimal, BoolClass):
         pass
-
     # qty 3
     class NoneFrozenDictTupleMixin(NoneClass, frozendict.frozendict, tuple):
         pass
-
     class NoneFrozenDictStrMixin(NoneClass, frozendict.frozendict, str):
         pass
-
     class NoneFrozenDictDecimalMixin(NoneClass, frozendict.frozendict, decimal.Decimal):
         pass
-
     class NoneFrozenDictBoolMixin(NoneClass, frozendict.frozendict, BoolClass):
         pass
-
     class NoneTupleStrMixin(NoneClass, tuple, str):
         pass
-
     class NoneTupleDecimalMixin(NoneClass, tuple, decimal.Decimal):
         pass
-
     class NoneTupleBoolMixin(NoneClass, tuple, BoolClass):
         pass
-
     class NoneStrDecimalMixin(NoneClass, str, decimal.Decimal):
         pass
-
     class NoneStrBoolMixin(NoneClass, str, BoolClass):
         pass
-
     class NoneDecimalBoolMixin(NoneClass, decimal.Decimal, BoolClass):
         pass
-
     class FrozenDictTupleStrMixin(frozendict.frozendict, tuple, str):
         pass
-
     class FrozenDictTupleDecimalMixin(frozendict.frozendict, tuple, decimal.Decimal):
         pass
-
     class FrozenDictTupleBoolMixin(frozendict.frozendict, tuple, BoolClass):
         pass
-
     class FrozenDictStrDecimalMixin(frozendict.frozendict, str, decimal.Decimal):
         pass
-
     class FrozenDictStrBoolMixin(frozendict.frozendict, str, BoolClass):
         pass
-
     class FrozenDictDecimalBoolMixin(frozendict.frozendict, decimal.Decimal, BoolClass):
         pass
-
     class TupleStrDecimalMixin(tuple, str, decimal.Decimal):
         pass
-
     class TupleStrBoolMixin(tuple, str, BoolClass):
         pass
-
     class TupleDecimalBoolMixin(tuple, decimal.Decimal, BoolClass):
         pass
-
     class StrDecimalBoolMixin(str, decimal.Decimal, BoolClass):
         pass
-
     # qty 4
     class NoneFrozenDictTupleStrMixin(NoneClass, frozendict.frozendict, tuple, str):
         pass
-
-    class NoneFrozenDictTupleDecimalMixin(
-        NoneClass, frozendict.frozendict, tuple, decimal.Decimal
-    ):
+    class NoneFrozenDictTupleDecimalMixin(NoneClass, frozendict.frozendict, tuple, decimal.Decimal):
         pass
-
-    class NoneFrozenDictTupleBoolMixin(
-        NoneClass, frozendict.frozendict, tuple, BoolClass
-    ):
+    class NoneFrozenDictTupleBoolMixin(NoneClass, frozendict.frozendict, tuple, BoolClass):
         pass
-
-    class NoneFrozenDictStrDecimalMixin(
-        NoneClass, frozendict.frozendict, str, decimal.Decimal
-    ):
+    class NoneFrozenDictStrDecimalMixin(NoneClass, frozendict.frozendict, str, decimal.Decimal):
         pass
-
     class NoneFrozenDictStrBoolMixin(NoneClass, frozendict.frozendict, str, BoolClass):
         pass
-
-    class NoneFrozenDictDecimalBoolMixin(
-        NoneClass, frozendict.frozendict, decimal.Decimal, BoolClass
-    ):
+    class NoneFrozenDictDecimalBoolMixin(NoneClass, frozendict.frozendict, decimal.Decimal, BoolClass):
         pass
-
     class NoneTupleStrDecimalMixin(NoneClass, tuple, str, decimal.Decimal):
         pass
-
     class NoneTupleStrBoolMixin(NoneClass, tuple, str, BoolClass):
         pass
-
     class NoneTupleDecimalBoolMixin(NoneClass, tuple, decimal.Decimal, BoolClass):
         pass
-
     class NoneStrDecimalBoolMixin(NoneClass, str, decimal.Decimal, BoolClass):
         pass
-
-    class FrozenDictTupleStrDecimalMixin(
-        frozendict.frozendict, tuple, str, decimal.Decimal
-    ):
+    class FrozenDictTupleStrDecimalMixin(frozendict.frozendict, tuple, str, decimal.Decimal):
         pass
-
     class FrozenDictTupleStrBoolMixin(frozendict.frozendict, tuple, str, BoolClass):
         pass
-
-    class FrozenDictTupleDecimalBoolMixin(
-        frozendict.frozendict, tuple, decimal.Decimal, BoolClass
-    ):
+    class FrozenDictTupleDecimalBoolMixin(frozendict.frozendict, tuple, decimal.Decimal, BoolClass):
         pass
-
-    class FrozenDictStrDecimalBoolMixin(
-        frozendict.frozendict, str, decimal.Decimal, BoolClass
-    ):
+    class FrozenDictStrDecimalBoolMixin(frozendict.frozendict, str, decimal.Decimal, BoolClass):
         pass
-
     class TupleStrDecimalBoolMixin(tuple, str, decimal.Decimal, BoolClass):
         pass
-
     # qty 5
-    class NoneFrozenDictTupleStrDecimalMixin(
-        NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal
-    ):
+    class NoneFrozenDictTupleStrDecimalMixin(NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal):
         pass
-
-    class NoneFrozenDictTupleStrBoolMixin(
-        NoneClass, frozendict.frozendict, tuple, str, BoolClass
-    ):
+    class NoneFrozenDictTupleStrBoolMixin(NoneClass, frozendict.frozendict, tuple, str, BoolClass):
         pass
-
-    class NoneFrozenDictTupleDecimalBoolMixin(
-        NoneClass, frozendict.frozendict, tuple, decimal.Decimal, BoolClass
-    ):
+    class NoneFrozenDictTupleDecimalBoolMixin(NoneClass, frozendict.frozendict, tuple, decimal.Decimal, BoolClass):
         pass
-
-    class NoneFrozenDictStrDecimalBoolMixin(
-        NoneClass, frozendict.frozendict, str, decimal.Decimal, BoolClass
-    ):
+    class NoneFrozenDictStrDecimalBoolMixin(NoneClass, frozendict.frozendict, str, decimal.Decimal, BoolClass):
         pass
-
-    class NoneTupleStrDecimalBoolMixin(
-        NoneClass, tuple, str, decimal.Decimal, BoolClass
-    ):
+    class NoneTupleStrDecimalBoolMixin(NoneClass, tuple, str, decimal.Decimal, BoolClass):
         pass
-
-    class FrozenDictTupleStrDecimalBoolMixin(
-        frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass
-    ):
+    class FrozenDictTupleStrDecimalBoolMixin(frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass):
         pass
-
     # qty 6
-    class NoneFrozenDictTupleStrDecimalBoolMixin(
-        NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass
-    ):
+    class NoneFrozenDictTupleStrDecimalBoolMixin(NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass):
         pass
-
     # qty 8
-    class NoneFrozenDictTupleStrDecimalBoolFileBytesMixin(
-        NoneClass,
-        frozendict.frozendict,
-        tuple,
-        str,
-        decimal.Decimal,
-        BoolClass,
-        FileIO,
-        bytes,
-    ):
+    class NoneFrozenDictTupleStrDecimalBoolFileBytesMixin(NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass, FileIO, bytes):
         pass
-
 else:
     # qty 1
     class NoneMixin:
         _types = {NoneClass}
-
     class FrozenDictMixin:
         _types = {frozendict.frozendict}
-
     class TupleMixin:
         _types = {tuple}
-
     class StrMixin:
         _types = {str}
-
     class DecimalMixin:
         _types = {decimal.Decimal}
-
     class BoolMixin:
         _types = {BoolClass}
-
     class BytesMixin:
         _types = {bytes}
-
     class FileMixin:
         _types = {FileIO}
-
     # qty 2
     class BinaryMixin:
         _types = {bytes, FileIO}
-
     class NoneFrozenDictMixin:
         _types = {NoneClass, frozendict.frozendict}
-
     class NoneTupleMixin:
         _types = {NoneClass, tuple}
-
     class NoneStrMixin:
         _types = {NoneClass, str}
-
     class NoneDecimalMixin:
         _types = {NoneClass, decimal.Decimal}
-
     class NoneBoolMixin:
         _types = {NoneClass, BoolClass}
-
     class FrozenDictTupleMixin:
         _types = {frozendict.frozendict, tuple}
-
     class FrozenDictStrMixin:
         _types = {frozendict.frozendict, str}
-
     class FrozenDictDecimalMixin:
         _types = {frozendict.frozendict, decimal.Decimal}
-
     class FrozenDictBoolMixin:
         _types = {frozendict.frozendict, BoolClass}
-
     class TupleStrMixin:
         _types = {tuple, str}
-
     class TupleDecimalMixin:
         _types = {tuple, decimal.Decimal}
-
     class TupleBoolMixin:
         _types = {tuple, BoolClass}
-
     class StrDecimalMixin:
         _types = {str, decimal.Decimal}
-
     class StrBoolMixin:
         _types = {str, BoolClass}
-
     class DecimalBoolMixin:
         _types = {decimal.Decimal, BoolClass}
-
     # qty 3
     class NoneFrozenDictTupleMixin:
         _types = {NoneClass, frozendict.frozendict, tuple}
-
     class NoneFrozenDictStrMixin:
         _types = {NoneClass, frozendict.frozendict, str}
-
     class NoneFrozenDictDecimalMixin:
         _types = {NoneClass, frozendict.frozendict, decimal.Decimal}
-
     class NoneFrozenDictBoolMixin:
         _types = {NoneClass, frozendict.frozendict, BoolClass}
-
     class NoneTupleStrMixin:
         _types = {NoneClass, tuple, str}
-
     class NoneTupleDecimalMixin:
         _types = {NoneClass, tuple, decimal.Decimal}
-
     class NoneTupleBoolMixin:
         _types = {NoneClass, tuple, BoolClass}
-
     class NoneStrDecimalMixin:
         _types = {NoneClass, str, decimal.Decimal}
-
     class NoneStrBoolMixin:
         _types = {NoneClass, str, BoolClass}
-
     class NoneDecimalBoolMixin:
         _types = {NoneClass, decimal.Decimal, BoolClass}
-
     class FrozenDictTupleStrMixin:
         _types = {frozendict.frozendict, tuple, str}
-
     class FrozenDictTupleDecimalMixin:
         _types = {frozendict.frozendict, tuple, decimal.Decimal}
-
     class FrozenDictTupleBoolMixin:
         _types = {frozendict.frozendict, tuple, BoolClass}
-
     class FrozenDictStrDecimalMixin:
         _types = {frozendict.frozendict, str, decimal.Decimal}
-
     class FrozenDictStrBoolMixin:
         _types = {frozendict.frozendict, str, BoolClass}
-
     class FrozenDictDecimalBoolMixin:
         _types = {frozendict.frozendict, decimal.Decimal, BoolClass}
-
     class TupleStrDecimalMixin:
         _types = {tuple, str, decimal.Decimal}
-
     class TupleStrBoolMixin:
         _types = {tuple, str, BoolClass}
-
     class TupleDecimalBoolMixin:
         _types = {tuple, decimal.Decimal, BoolClass}
-
     class StrDecimalBoolMixin:
         _types = {str, decimal.Decimal, BoolClass}
-
     # qty 4
     class NoneFrozenDictTupleStrMixin:
         _types = {NoneClass, frozendict.frozendict, tuple, str}
-
     class NoneFrozenDictTupleDecimalMixin:
         _types = {NoneClass, frozendict.frozendict, tuple, decimal.Decimal}
-
     class NoneFrozenDictTupleBoolMixin:
         _types = {NoneClass, frozendict.frozendict, tuple, BoolClass}
-
     class NoneFrozenDictStrDecimalMixin:
         _types = {NoneClass, frozendict.frozendict, str, decimal.Decimal}
-
     class NoneFrozenDictStrBoolMixin:
         _types = {NoneClass, frozendict.frozendict, str, BoolClass}
-
     class NoneFrozenDictDecimalBoolMixin:
         _types = {NoneClass, frozendict.frozendict, decimal.Decimal, BoolClass}
-
     class NoneTupleStrDecimalMixin:
         _types = {NoneClass, tuple, str, decimal.Decimal}
-
     class NoneTupleStrBoolMixin:
         _types = {NoneClass, tuple, str, BoolClass}
-
     class NoneTupleDecimalBoolMixin:
         _types = {NoneClass, tuple, decimal.Decimal, BoolClass}
-
     class NoneStrDecimalBoolMixin:
         _types = {NoneClass, str, decimal.Decimal, BoolClass}
-
     class FrozenDictTupleStrDecimalMixin:
         _types = {frozendict.frozendict, tuple, str, decimal.Decimal}
-
     class FrozenDictTupleStrBoolMixin:
         _types = {frozendict.frozendict, tuple, str, BoolClass}
-
     class FrozenDictTupleDecimalBoolMixin:
         _types = {frozendict.frozendict, tuple, decimal.Decimal, BoolClass}
-
     class FrozenDictStrDecimalBoolMixin:
         _types = {frozendict.frozendict, str, decimal.Decimal, BoolClass}
-
     class TupleStrDecimalBoolMixin:
         _types = {tuple, str, decimal.Decimal, BoolClass}
-
     # qty 5
     class NoneFrozenDictTupleStrDecimalMixin:
         _types = {NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal}
-
     class NoneFrozenDictTupleStrBoolMixin:
         _types = {NoneClass, frozendict.frozendict, tuple, str, BoolClass}
-
     class NoneFrozenDictTupleDecimalBoolMixin:
         _types = {NoneClass, frozendict.frozendict, tuple, decimal.Decimal, BoolClass}
-
     class NoneFrozenDictStrDecimalBoolMixin:
         _types = {NoneClass, frozendict.frozendict, str, decimal.Decimal, BoolClass}
-
     class NoneTupleStrDecimalBoolMixin:
         _types = {NoneClass, tuple, str, decimal.Decimal, BoolClass}
-
     class FrozenDictTupleStrDecimalBoolMixin:
         _types = {frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass}
-
     # qty 6
     class NoneFrozenDictTupleStrDecimalBoolMixin:
-        _types = {
-            NoneClass,
-            frozendict.frozendict,
-            tuple,
-            str,
-            decimal.Decimal,
-            BoolClass,
-        }
-
+        _types = {NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass}
     # qty 8
     class NoneFrozenDictTupleStrDecimalBoolFileBytesMixin:
-        _types = {
-            NoneClass,
-            frozendict.frozendict,
-            tuple,
-            str,
-            decimal.Decimal,
-            BoolClass,
-            FileIO,
-            bytes,
-        }
+        _types = {NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass, FileIO, bytes}
 
 
 class ValidatorBase:
     @staticmethod
     def _is_json_validation_enabled_oapg(schema_keyword, configuration=None):
         """Returns true if JSON schema validation is enabled for the specified
         validation keyword. This can be used to skip JSON schema structural validation
@@ -1168,24 +872,20 @@
         it has been added to prevent collisions with other methods and properties
 
         Args:
             schema_keyword (string): the name of a JSON schema validation keyword.
             configuration (Configuration): the configuration class.
         """
 
-        return (
-            configuration is None
-            or not hasattr(configuration, "_disabled_client_side_validations")
-            or schema_keyword not in configuration._disabled_client_side_validations
-        )
+        return (configuration is None or
+            not hasattr(configuration, '_disabled_client_side_validations') or
+            schema_keyword not in configuration._disabled_client_side_validations)
 
     @staticmethod
-    def _raise_validation_error_message_oapg(
-        value, constraint_msg, constraint_value, path_to_item, additional_txt=""
-    ):
+    def _raise_validation_error_message_oapg(value, constraint_msg, constraint_value, path_to_item, additional_txt=""):
         raise ApiValueError(
             "Invalid value `{value}`, {constraint_msg} `{constraint_value}`{additional_txt} at {path_to_item}".format(
                 value=value,
                 constraint_msg=constraint_msg,
                 constraint_value=constraint_value,
                 additional_txt=additional_txt,
                 path_to_item=path_to_item,
@@ -1195,40 +895,23 @@
 
 class EnumBase:
     @classmethod
     def _validate_oapg(
         cls,
         arg,
         validation_metadata: ValidationMetadata,
-    ) -> typing.Dict[
-        typing.Tuple[typing.Union[str, int], ...],
-        typing.Set[
-            typing.Union[
-                "Schema",
-                str,
-                decimal.Decimal,
-                BoolClass,
-                NoneClass,
-                frozendict.frozendict,
-                tuple,
-            ]
-        ],
-    ]:
+    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]]:
         """
         EnumBase _validate_oapg
         Validates that arg is in the enum's allowed values
         """
         try:
             cls.MetaOapg.enum_value_to_name[arg]
         except KeyError:
-            raise ApiValueError(
-                "Invalid value {} passed in to {}, allowed_values={}".format(
-                    arg, cls, cls.MetaOapg.enum_value_to_name.keys()
-                )
-            )
+            raise ApiValueError("Invalid value {} passed in to {}, allowed_values={}".format(arg, cls, cls.MetaOapg.enum_value_to_name.keys()))
         return super()._validate_oapg(arg, validation_metadata=validation_metadata)
 
 
 class BoolBase:
     def is_true_oapg(self) -> bool:
         """
         A replacement for x is True
@@ -1264,102 +947,84 @@
 
     @property
     def as_str_oapg(self) -> str:
         return self
 
     @property
     def as_date_oapg(self) -> date:
-        raise Exception("not implemented")
+        raise Exception('not implemented')
 
     @property
     def as_datetime_oapg(self) -> datetime:
-        raise Exception("not implemented")
+        raise Exception('not implemented')
 
     @property
     def as_decimal_oapg(self) -> decimal.Decimal:
-        raise Exception("not implemented")
+        raise Exception('not implemented')
 
     @property
     def as_uuid_oapg(self) -> uuid.UUID:
-        raise Exception("not implemented")
+        raise Exception('not implemented')
 
     @classmethod
-    def __check_str_validations(cls, arg: str, validation_metadata: ValidationMetadata):
-        if not hasattr(cls, "MetaOapg"):
+    def __check_str_validations(
+        cls,
+        arg: str,
+        validation_metadata: ValidationMetadata
+    ):
+        if not hasattr(cls, 'MetaOapg'):
             return
-        if (
-            cls._is_json_validation_enabled_oapg(
-                "maxLength", validation_metadata.configuration
-            )
-            and hasattr(cls.MetaOapg, "max_length")
-            and len(arg) > cls.MetaOapg.max_length
-        ):
+        if (cls._is_json_validation_enabled_oapg('maxLength', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'max_length') and
+                len(arg) > cls.MetaOapg.max_length):
             cls._raise_validation_error_message_oapg(
                 value=arg,
                 constraint_msg="length must be less than or equal to",
                 constraint_value=cls.MetaOapg.max_length,
-                path_to_item=validation_metadata.path_to_item,
+                path_to_item=validation_metadata.path_to_item
             )
 
-        if (
-            cls._is_json_validation_enabled_oapg(
-                "minLength", validation_metadata.configuration
-            )
-            and hasattr(cls.MetaOapg, "min_length")
-            and len(arg) < cls.MetaOapg.min_length
-        ):
+        if (cls._is_json_validation_enabled_oapg('minLength', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'min_length') and
+                len(arg) < cls.MetaOapg.min_length):
             cls._raise_validation_error_message_oapg(
                 value=arg,
                 constraint_msg="length must be greater than or equal to",
                 constraint_value=cls.MetaOapg.min_length,
-                path_to_item=validation_metadata.path_to_item,
+                path_to_item=validation_metadata.path_to_item
             )
 
-        if cls._is_json_validation_enabled_oapg(
-            "pattern", validation_metadata.configuration
-        ) and hasattr(cls.MetaOapg, "regex"):
+        if (cls._is_json_validation_enabled_oapg('pattern', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'regex')):
             for regex_dict in cls.MetaOapg.regex:
-                flags = regex_dict.get("flags", 0)
-                if not re.search(regex_dict["pattern"], arg, flags=flags):
+                flags = regex_dict.get('flags', 0)
+                if not re.search(regex_dict['pattern'], arg, flags=flags):
                     if flags != 0:
                         # Don't print the regex flags if the flags are not
                         # specified in the OAS document.
                         cls._raise_validation_error_message_oapg(
                             value=arg,
                             constraint_msg="must match regular expression",
-                            constraint_value=regex_dict["pattern"],
+                            constraint_value=regex_dict['pattern'],
                             path_to_item=validation_metadata.path_to_item,
-                            additional_txt=" with flags=`{}`".format(flags),
+                            additional_txt=" with flags=`{}`".format(flags)
                         )
                     cls._raise_validation_error_message_oapg(
                         value=arg,
                         constraint_msg="must match regular expression",
-                        constraint_value=regex_dict["pattern"],
-                        path_to_item=validation_metadata.path_to_item,
+                        constraint_value=regex_dict['pattern'],
+                        path_to_item=validation_metadata.path_to_item
                     )
 
     @classmethod
     def _validate_oapg(
         cls,
         arg,
         validation_metadata: ValidationMetadata,
-    ) -> typing.Dict[
-        typing.Tuple[typing.Union[str, int], ...],
-        typing.Set[
-            typing.Union[
-                "Schema",
-                str,
-                decimal.Decimal,
-                BoolClass,
-                NoneClass,
-                frozendict.frozendict,
-                tuple,
-            ]
-        ],
-    ]:
+    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]]:
         """
         StrBase _validate_oapg
         Validates that validations pass
         """
         if isinstance(arg, str):
             cls.__check_str_validations(arg, validation_metadata)
         return super()._validate_oapg(arg, validation_metadata=validation_metadata)
@@ -1368,26 +1033,22 @@
 class UUIDBase:
     @property
     @functools.lru_cache()
     def as_uuid_oapg(self) -> uuid.UUID:
         return uuid.UUID(self)
 
     @classmethod
-    def __validate_format(
-        cls, arg: typing.Optional[str], validation_metadata: ValidationMetadata
-    ):
+    def __validate_format(cls, arg: typing.Optional[str], validation_metadata: ValidationMetadata):
         if isinstance(arg, str):
             try:
                 uuid.UUID(arg)
                 return True
             except ValueError:
                 raise ApiValueError(
-                    "Invalid value '{}' for type UUID at {}".format(
-                        arg, validation_metadata.path_to_item
-                    )
+                    "Invalid value '{}' for type UUID at {}".format(arg, validation_metadata.path_to_item)
                 )
 
     @classmethod
     def _validate_oapg(
         cls,
         arg,
         validation_metadata: typing.Optional[ValidationMetadata] = None,
@@ -1396,68 +1057,65 @@
         UUIDBase _validate_oapg
         """
         cls.__validate_format(arg, validation_metadata=validation_metadata)
         return super()._validate_oapg(arg, validation_metadata=validation_metadata)
 
 
 class CustomIsoparser(isoparser):
+
     @_takes_ascii
     def parse_isodatetime(self, dt_str):
         components, pos = self._parse_isodate(dt_str)
         if len(dt_str) > pos:
-            if self._sep is None or dt_str[pos : pos + 1] == self._sep:
-                components += self._parse_isotime(dt_str[pos + 1 :])
+            if self._sep is None or dt_str[pos:pos + 1] == self._sep:
+                components += self._parse_isotime(dt_str[pos + 1:])
             else:
-                raise ValueError("String contains unknown ISO components")
+                raise ValueError('String contains unknown ISO components')
 
         if len(components) > 3 and components[3] == 24:
             components[3] = 0
             return datetime(*components) + timedelta(days=1)
 
         if len(components) <= 3:
-            raise ValueError("Value is not a datetime")
+            raise ValueError('Value is not a datetime')
 
         return datetime(*components)
 
     @_takes_ascii
     def parse_isodate(self, datestr):
         components, pos = self._parse_isodate(datestr)
 
         if len(datestr) > pos:
-            raise ValueError("String contains invalid time components")
+            raise ValueError('String contains invalid time components')
 
         if len(components) > 3:
-            raise ValueError("String contains invalid time components")
+            raise ValueError('String contains invalid time components')
 
         return date(*components)
 
 
 DEFAULT_ISOPARSER = CustomIsoparser()
 
 
 class DateBase:
     @property
     @functools.lru_cache()
     def as_date_oapg(self) -> date:
         return DEFAULT_ISOPARSER.parse_isodate(self)
 
     @classmethod
-    def __validate_format(
-        cls, arg: typing.Optional[str], validation_metadata: ValidationMetadata
-    ):
+    def __validate_format(cls, arg: typing.Optional[str], validation_metadata: ValidationMetadata):
         if isinstance(arg, str):
             try:
                 DEFAULT_ISOPARSER.parse_isodate(arg)
                 return True
             except ValueError:
                 raise ApiValueError(
                     "Value does not conform to the required ISO-8601 date format. "
-                    "Invalid value '{}' for type date at {}".format(
-                        arg, validation_metadata.path_to_item
-                    )
+                    "Invalid value '{}' for type date at {}".format(arg, validation_metadata.path_to_item)
                 )
 
     @classmethod
     def _validate_oapg(
         cls,
         arg,
         validation_metadata: typing.Optional[ValidationMetadata] = None,
@@ -1472,27 +1130,23 @@
 class DateTimeBase:
     @property
     @functools.lru_cache()
     def as_datetime_oapg(self) -> datetime:
         return DEFAULT_ISOPARSER.parse_isodatetime(self)
 
     @classmethod
-    def __validate_format(
-        cls, arg: typing.Optional[str], validation_metadata: ValidationMetadata
-    ):
+    def __validate_format(cls, arg: typing.Optional[str], validation_metadata: ValidationMetadata):
         if isinstance(arg, str):
             try:
                 DEFAULT_ISOPARSER.parse_isodatetime(arg)
                 return True
             except ValueError:
                 raise ApiValueError(
                     "Value does not conform to the required ISO-8601 datetime format. "
-                    "Invalid value '{}' for type datetime at {}".format(
-                        arg, validation_metadata.path_to_item
-                    )
+                    "Invalid value '{}' for type datetime at {}".format(arg, validation_metadata.path_to_item)
                 )
 
     @classmethod
     def _validate_oapg(
         cls,
         arg,
         validation_metadata: ValidationMetadata,
@@ -1513,27 +1167,23 @@
 
     @property
     @functools.lru_cache()
     def as_decimal_oapg(self) -> decimal.Decimal:
         return decimal.Decimal(self)
 
     @classmethod
-    def __validate_format(
-        cls, arg: typing.Optional[str], validation_metadata: ValidationMetadata
-    ):
+    def __validate_format(cls, arg: typing.Optional[str], validation_metadata: ValidationMetadata):
         if isinstance(arg, str):
             try:
                 decimal.Decimal(arg)
                 return True
             except decimal.InvalidOperation:
                 raise ApiValueError(
                     "Value cannot be converted to a decimal. "
-                    "Invalid value '{}' for type decimal at {}".format(
-                        arg, validation_metadata.path_to_item
-                    )
+                    "Invalid value '{}' for type decimal at {}".format(arg, validation_metadata.path_to_item)
                 )
 
     @classmethod
     def _validate_oapg(
         cls,
         arg,
         validation_metadata: ValidationMetadata,
@@ -1560,132 +1210,105 @@
             DecimalTuple(sign=0, digits=(9, 0), exponent=-1)
             so we can tell that the value came from a float and convert it back to a float
             during later serialization
             """
             if self.as_tuple().exponent < 0:
                 # this could be represented as an integer but should be represented as a float
                 # because that's what it was serialized from
-                raise ApiValueError(f"{self} is not an integer")
+                raise ApiValueError(f'{self} is not an integer')
             self._as_int = int(self)
             return self._as_int
 
     @property
     def as_float_oapg(self) -> float:
         try:
             return self._as_float
         except AttributeError:
             if self.as_tuple().exponent >= 0:
-                raise ApiValueError(f"{self} is not a float")
+                raise ApiValueError(f'{self} is not a float')
             self._as_float = float(self)
             return self._as_float
 
     @classmethod
-    def __check_numeric_validations(cls, arg, validation_metadata: ValidationMetadata):
-        if not hasattr(cls, "MetaOapg"):
+    def __check_numeric_validations(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata
+    ):
+        if not hasattr(cls, 'MetaOapg'):
             return
-        if cls._is_json_validation_enabled_oapg(
-            "multipleOf", validation_metadata.configuration
-        ) and hasattr(cls.MetaOapg, "multiple_of"):
+        if cls._is_json_validation_enabled_oapg('multipleOf',
+                                      validation_metadata.configuration) and hasattr(cls.MetaOapg, 'multiple_of'):
             multiple_of_value = cls.MetaOapg.multiple_of
-            if not (float(arg) / multiple_of_value).is_integer():
+            if (not (float(arg) / multiple_of_value).is_integer()):
                 # Note 'multipleOf' will be as good as the floating point arithmetic.
                 cls._raise_validation_error_message_oapg(
                     value=arg,
                     constraint_msg="value must be a multiple of",
                     constraint_value=multiple_of_value,
-                    path_to_item=validation_metadata.path_to_item,
+                    path_to_item=validation_metadata.path_to_item
                 )
 
         checking_max_or_min_values = any(
-            hasattr(cls.MetaOapg, validation_key)
-            for validation_key in {
-                "exclusive_maximum",
-                "inclusive_maximum",
-                "exclusive_minimum",
-                "inclusive_minimum",
+            hasattr(cls.MetaOapg, validation_key) for validation_key in {
+                'exclusive_maximum',
+                'inclusive_maximum',
+                'exclusive_minimum',
+                'inclusive_minimum',
             }
         )
         if not checking_max_or_min_values:
             return
 
-        if (
-            cls._is_json_validation_enabled_oapg(
-                "exclusiveMaximum", validation_metadata.configuration
-            )
-            and hasattr(cls.MetaOapg, "exclusive_maximum")
-            and arg >= cls.MetaOapg.exclusive_maximum
-        ):
+        if (cls._is_json_validation_enabled_oapg('exclusiveMaximum', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'exclusive_maximum') and
+                arg >= cls.MetaOapg.exclusive_maximum):
             cls._raise_validation_error_message_oapg(
                 value=arg,
                 constraint_msg="must be a value less than",
                 constraint_value=cls.MetaOapg.exclusive_maximum,
-                path_to_item=validation_metadata.path_to_item,
+                path_to_item=validation_metadata.path_to_item
             )
 
-        if (
-            cls._is_json_validation_enabled_oapg(
-                "maximum", validation_metadata.configuration
-            )
-            and hasattr(cls.MetaOapg, "inclusive_maximum")
-            and arg > cls.MetaOapg.inclusive_maximum
-        ):
+        if (cls._is_json_validation_enabled_oapg('maximum', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'inclusive_maximum') and
+                arg > cls.MetaOapg.inclusive_maximum):
             cls._raise_validation_error_message_oapg(
                 value=arg,
                 constraint_msg="must be a value less than or equal to",
                 constraint_value=cls.MetaOapg.inclusive_maximum,
-                path_to_item=validation_metadata.path_to_item,
+                path_to_item=validation_metadata.path_to_item
             )
 
-        if (
-            cls._is_json_validation_enabled_oapg(
-                "exclusiveMinimum", validation_metadata.configuration
-            )
-            and hasattr(cls.MetaOapg, "exclusive_minimum")
-            and arg <= cls.MetaOapg.exclusive_minimum
-        ):
+        if (cls._is_json_validation_enabled_oapg('exclusiveMinimum', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'exclusive_minimum') and
+                arg <= cls.MetaOapg.exclusive_minimum):
             cls._raise_validation_error_message_oapg(
                 value=arg,
                 constraint_msg="must be a value greater than",
                 constraint_value=cls.MetaOapg.exclusive_maximum,
-                path_to_item=validation_metadata.path_to_item,
+                path_to_item=validation_metadata.path_to_item
             )
 
-        if (
-            cls._is_json_validation_enabled_oapg(
-                "minimum", validation_metadata.configuration
-            )
-            and hasattr(cls.MetaOapg, "inclusive_minimum")
-            and arg < cls.MetaOapg.inclusive_minimum
-        ):
+        if (cls._is_json_validation_enabled_oapg('minimum', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'inclusive_minimum') and
+                arg < cls.MetaOapg.inclusive_minimum):
             cls._raise_validation_error_message_oapg(
                 value=arg,
                 constraint_msg="must be a value greater than or equal to",
                 constraint_value=cls.MetaOapg.inclusive_minimum,
-                path_to_item=validation_metadata.path_to_item,
+                path_to_item=validation_metadata.path_to_item
             )
 
     @classmethod
     def _validate_oapg(
         cls,
         arg,
         validation_metadata: ValidationMetadata,
-    ) -> typing.Dict[
-        typing.Tuple[typing.Union[str, int], ...],
-        typing.Set[
-            typing.Union[
-                "Schema",
-                str,
-                decimal.Decimal,
-                BoolClass,
-                NoneClass,
-                frozendict.frozendict,
-                tuple,
-            ]
-        ],
-    ]:
+    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]]:
         """
         NumberBase _validate_oapg
         Validates that validations pass
         """
         if isinstance(arg, decimal.Decimal):
             cls.__check_numeric_validations(arg, validation_metadata)
         return super()._validate_oapg(arg, validation_metadata=validation_metadata)
@@ -1707,80 +1330,67 @@
 
         Raises:
             ApiTypeError - for missing required arguments, or for invalid properties
         """
 
         # if we have definitions for an items schema, use it
         # otherwise accept anything
-        item_cls = getattr(cls.MetaOapg, "items", UnsetAnyTypeSchema)
+        item_cls = getattr(cls.MetaOapg, 'items', UnsetAnyTypeSchema)
         item_cls = cls._get_class_oapg(item_cls)
         path_to_schemas = {}
         for i, value in enumerate(list_items):
             item_validation_metadata = ValidationMetadata(
                 from_server=validation_metadata.from_server,
                 configuration=validation_metadata.configuration,
-                path_to_item=validation_metadata.path_to_item + (i,),
-                validated_path_to_schemas=validation_metadata.validated_path_to_schemas,
+                path_to_item=validation_metadata.path_to_item+(i,),
+                validated_path_to_schemas=validation_metadata.validated_path_to_schemas
             )
             if item_validation_metadata.validation_ran_earlier(item_cls):
                 add_deeper_validated_schemas(item_validation_metadata, path_to_schemas)
                 continue
             other_path_to_schemas = item_cls._validate_oapg(
-                value, validation_metadata=item_validation_metadata
-            )
+                value, validation_metadata=item_validation_metadata)
             update(path_to_schemas, other_path_to_schemas)
         return path_to_schemas
 
     @classmethod
-    def __check_tuple_validations(cls, arg, validation_metadata: ValidationMetadata):
-        if not hasattr(cls, "MetaOapg"):
+    def __check_tuple_validations(
+            cls, arg,
+            validation_metadata: ValidationMetadata):
+        if not hasattr(cls, 'MetaOapg'):
             return
-        if (
-            cls._is_json_validation_enabled_oapg(
-                "maxItems", validation_metadata.configuration
-            )
-            and hasattr(cls.MetaOapg, "max_items")
-            and len(arg) > cls.MetaOapg.max_items
-        ):
+        if (cls._is_json_validation_enabled_oapg('maxItems', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'max_items') and
+                len(arg) > cls.MetaOapg.max_items):
             cls._raise_validation_error_message_oapg(
                 value=arg,
                 constraint_msg="number of items must be less than or equal to",
                 constraint_value=cls.MetaOapg.max_items,
-                path_to_item=validation_metadata.path_to_item,
+                path_to_item=validation_metadata.path_to_item
             )
 
-        if (
-            cls._is_json_validation_enabled_oapg(
-                "minItems", validation_metadata.configuration
-            )
-            and hasattr(cls.MetaOapg, "min_items")
-            and len(arg) < cls.MetaOapg.min_items
-        ):
+        if (cls._is_json_validation_enabled_oapg('minItems', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'min_items') and
+                len(arg) < cls.MetaOapg.min_items):
             cls._raise_validation_error_message_oapg(
                 value=arg,
                 constraint_msg="number of items must be greater than or equal to",
                 constraint_value=cls.MetaOapg.min_items,
-                path_to_item=validation_metadata.path_to_item,
+                path_to_item=validation_metadata.path_to_item
             )
 
-        if (
-            cls._is_json_validation_enabled_oapg(
-                "uniqueItems", validation_metadata.configuration
-            )
-            and hasattr(cls.MetaOapg, "unique_items")
-            and cls.MetaOapg.unique_items
-            and arg
-        ):
+        if (cls._is_json_validation_enabled_oapg('uniqueItems', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'unique_items') and cls.MetaOapg.unique_items and arg):
             unique_items = set(arg)
             if len(arg) > len(unique_items):
                 cls._raise_validation_error_message_oapg(
                     value=arg,
                     constraint_msg="duplicate items were found, and the tuple must not contain duplicates because",
-                    constraint_value="unique_items==True",
-                    path_to_item=validation_metadata.path_to_item,
+                    constraint_value='unique_items==True',
+                    path_to_item=validation_metadata.path_to_item
                 )
 
     @classmethod
     def _validate_oapg(
         cls,
         arg,
         validation_metadata: ValidationMetadata,
@@ -1798,125 +1408,110 @@
 
         Raises:
             ApiValueError: when a string can't be converted into a date or datetime and it must be one of those classes
             ApiTypeError: when the input type is not in the list of allowed spec types
         """
         if isinstance(arg, tuple):
             cls.__check_tuple_validations(arg, validation_metadata)
-        _path_to_schemas = super()._validate_oapg(
-            arg, validation_metadata=validation_metadata
-        )
+        _path_to_schemas = super()._validate_oapg(arg, validation_metadata=validation_metadata)
         if not isinstance(arg, tuple):
             return _path_to_schemas
         updated_vm = ValidationMetadata(
             configuration=validation_metadata.configuration,
             from_server=validation_metadata.from_server,
             path_to_item=validation_metadata.path_to_item,
             seen_classes=validation_metadata.seen_classes | frozenset({cls}),
-            validated_path_to_schemas=validation_metadata.validated_path_to_schemas,
-        )
-        other_path_to_schemas = cls.__validate_items(
-            arg, validation_metadata=updated_vm
+            validated_path_to_schemas=validation_metadata.validated_path_to_schemas
         )
+        other_path_to_schemas = cls.__validate_items(arg, validation_metadata=updated_vm)
         update(_path_to_schemas, other_path_to_schemas)
         return _path_to_schemas
 
     @classmethod
     def _get_items_oapg(
-        cls: "Schema",
+        cls: 'Schema',
         arg: typing.List[typing.Any],
         path_to_item: typing.Tuple[typing.Union[str, int], ...],
-        path_to_schemas: typing.Dict[
-            typing.Tuple[typing.Union[str, int], ...], typing.Type["Schema"]
-        ],
+        path_to_schemas: typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Type['Schema']]
     ):
-        """
+        '''
         ListBase _get_items_oapg
-        """
+        '''
         cast_items = []
 
         for i, value in enumerate(arg):
             item_path_to_item = path_to_item + (i,)
             item_cls = path_to_schemas[item_path_to_item]
             new_value = item_cls._get_new_instance_without_conversion_oapg(
-                value, item_path_to_item, path_to_schemas
+                value,
+                item_path_to_item,
+                path_to_schemas
             )
             cast_items.append(new_value)
 
         return cast_items
 
 
 class Discriminable:
     MetaOapg: MetaOapgTyped
 
     @classmethod
-    def _ensure_discriminator_value_present_oapg(
-        cls, disc_property_name: str, validation_metadata: ValidationMetadata, *args
-    ):
+    def _ensure_discriminator_value_present_oapg(cls, disc_property_name: str, validation_metadata: ValidationMetadata, *args):
         if not args or args and disc_property_name not in args[0]:
             # The input data does not contain the discriminator property
             raise ApiValueError(
                 "Cannot deserialize input data due to missing discriminator. "
-                "The discriminator property '{}' is missing at path: {}".format(
-                    disc_property_name, validation_metadata.path_to_item
-                )
+                "The discriminator property '{}' is missing at path: {}".format(disc_property_name, validation_metadata.path_to_item)
             )
 
     @classmethod
-    def get_discriminated_class_oapg(
-        cls, disc_property_name: str, disc_payload_value: str
-    ):
+    def get_discriminated_class_oapg(cls, disc_property_name: str, disc_payload_value: str):
         """
         Used in schemas with discriminators
         """
-        if not hasattr(cls.MetaOapg, "discriminator"):
+        if not hasattr(cls.MetaOapg, 'discriminator'):
             return None
         disc = cls.MetaOapg.discriminator()
         if disc_property_name not in disc:
             return None
         discriminated_cls = disc[disc_property_name].get(disc_payload_value)
         if discriminated_cls is not None:
             return discriminated_cls
-        if not hasattr(cls, "MetaOapg"):
+        if not hasattr(cls, 'MetaOapg'):
             return None
         elif not (
-            hasattr(cls.MetaOapg, "all_of")
-            or hasattr(cls.MetaOapg, "one_of")
-            or hasattr(cls.MetaOapg, "any_of")
+            hasattr(cls.MetaOapg, 'all_of') or
+            hasattr(cls.MetaOapg, 'one_of') or
+            hasattr(cls.MetaOapg, 'any_of')
         ):
             return None
         # TODO stop traveling if a cycle is hit
-        if hasattr(cls.MetaOapg, "all_of"):
+        if hasattr(cls.MetaOapg, 'all_of'):
             for allof_cls in cls.MetaOapg.all_of():
                 discriminated_cls = allof_cls.get_discriminated_class_oapg(
-                    disc_property_name=disc_property_name,
-                    disc_payload_value=disc_payload_value,
-                )
+                    disc_property_name=disc_property_name, disc_payload_value=disc_payload_value)
                 if discriminated_cls is not None:
                     return discriminated_cls
-        if hasattr(cls.MetaOapg, "one_of"):
+        if hasattr(cls.MetaOapg, 'one_of'):
             for oneof_cls in cls.MetaOapg.one_of():
                 discriminated_cls = oneof_cls.get_discriminated_class_oapg(
-                    disc_property_name=disc_property_name,
-                    disc_payload_value=disc_payload_value,
-                )
+                    disc_property_name=disc_property_name, disc_payload_value=disc_payload_value)
                 if discriminated_cls is not None:
                     return discriminated_cls
-        if hasattr(cls.MetaOapg, "any_of"):
+        if hasattr(cls.MetaOapg, 'any_of'):
             for anyof_cls in cls.MetaOapg.any_of():
                 discriminated_cls = anyof_cls.get_discriminated_class_oapg(
-                    disc_property_name=disc_property_name,
-                    disc_payload_value=disc_payload_value,
-                )
+                    disc_property_name=disc_property_name, disc_payload_value=disc_payload_value)
                 if discriminated_cls is not None:
                     return discriminated_cls
         return None
 
 
 class DictBase(Discriminable, ValidatorBase):
+
     @classmethod
     def __validate_arg_presence(cls, arg):
         """
         Ensures that:
         - all required arguments are passed in
         - the input variable names are valid
             - present in properties or
@@ -1931,50 +1526,46 @@
             arg: the input dict
 
         Raises:
             ApiTypeError - for missing required arguments, or for invalid properties
         """
         seen_required_properties = set()
         invalid_arguments = []
-        required_property_names = getattr(cls.MetaOapg, "required", set())
-        additional_properties = getattr(
-            cls.MetaOapg, "additional_properties", UnsetAnyTypeSchema
-        )
-        properties = getattr(cls.MetaOapg, "properties", {})
-        property_annotations = getattr(properties, "__annotations__", {})
+        required_property_names = getattr(cls.MetaOapg, 'required', set())
+        additional_properties = getattr(cls.MetaOapg, 'additional_properties', UnsetAnyTypeSchema)
+        properties = getattr(cls.MetaOapg, 'properties', {})
+        property_annotations = getattr(properties, '__annotations__', {})
         for property_name in arg:
             if property_name in required_property_names:
                 seen_required_properties.add(property_name)
             elif property_name in property_annotations:
                 continue
             elif additional_properties is not NotAnyTypeSchema:
                 continue
             else:
                 invalid_arguments.append(property_name)
-        missing_required_arguments = list(
-            required_property_names - seen_required_properties
-        )
+        missing_required_arguments = list(required_property_names - seen_required_properties)
         if missing_required_arguments:
             missing_required_arguments.sort()
             raise ApiTypeError(
                 "{} is missing {} required argument{}: {}".format(
                     cls.__name__,
                     len(missing_required_arguments),
                     "s" if len(missing_required_arguments) > 1 else "",
-                    missing_required_arguments,
+                    missing_required_arguments
                 )
             )
         if invalid_arguments:
             invalid_arguments.sort()
             raise ApiTypeError(
                 "{} was passed {} invalid argument{}: {}".format(
                     cls.__name__,
                     len(invalid_arguments),
                     "s" if len(invalid_arguments) > 1 else "",
-                    invalid_arguments,
+                    invalid_arguments
                 )
             )
 
     @classmethod
     def __validate_args(cls, arg, validation_metadata: ValidationMetadata):
         """
         Ensures that:
@@ -1985,85 +1576,75 @@
         Args:
             arg: the input dict
 
         Raises:
             ApiTypeError - for missing required arguments, or for invalid properties
         """
         path_to_schemas = {}
-        additional_properties = getattr(
-            cls.MetaOapg, "additional_properties", UnsetAnyTypeSchema
-        )
-        properties = getattr(cls.MetaOapg, "properties", {})
-        property_annotations = getattr(properties, "__annotations__", {})
+        additional_properties = getattr(cls.MetaOapg, 'additional_properties', UnsetAnyTypeSchema)
+        properties = getattr(cls.MetaOapg, 'properties', {})
+        property_annotations = getattr(properties, '__annotations__', {})
         for property_name, value in arg.items():
-            path_to_item = validation_metadata.path_to_item + (property_name,)
+            path_to_item = validation_metadata.path_to_item+(property_name,)
             if property_name in property_annotations:
                 schema = property_annotations[property_name]
             elif additional_properties is not NotAnyTypeSchema:
                 if additional_properties is UnsetAnyTypeSchema:
                     """
                     If additionalProperties is unset and this path_to_item does not yet have
                     any validations on it, validate it.
                     If it already has validations on it, skip this validation.
                     """
                     if path_to_item in path_to_schemas:
                         continue
                 schema = additional_properties
             else:
-                raise ApiTypeError(
-                    "Unable to find schema for value={} in class={} at path_to_item={}".format(
-                        value, cls, validation_metadata.path_to_item + (property_name,)
-                    )
-                )
+                raise ApiTypeError('Unable to find schema for value={} in class={} at path_to_item={}'.format(
+                    value, cls, validation_metadata.path_to_item+(property_name,)
+                ))
             schema = cls._get_class_oapg(schema)
             arg_validation_metadata = ValidationMetadata(
                 from_server=validation_metadata.from_server,
                 configuration=validation_metadata.configuration,
                 path_to_item=path_to_item,
-                validated_path_to_schemas=validation_metadata.validated_path_to_schemas,
+                validated_path_to_schemas=validation_metadata.validated_path_to_schemas
             )
             if arg_validation_metadata.validation_ran_earlier(schema):
                 add_deeper_validated_schemas(arg_validation_metadata, path_to_schemas)
                 continue
-            other_path_to_schemas = schema._validate_oapg(
-                value, validation_metadata=arg_validation_metadata
-            )
+            other_path_to_schemas = schema._validate_oapg(value, validation_metadata=arg_validation_metadata)
             update(path_to_schemas, other_path_to_schemas)
         return path_to_schemas
 
     @classmethod
-    def __check_dict_validations(cls, arg, validation_metadata: ValidationMetadata):
-        if not hasattr(cls, "MetaOapg"):
+    def __check_dict_validations(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata
+    ):
+        if not hasattr(cls, 'MetaOapg'):
             return
-        if (
-            cls._is_json_validation_enabled_oapg(
-                "maxProperties", validation_metadata.configuration
-            )
-            and hasattr(cls.MetaOapg, "max_properties")
-            and len(arg) > cls.MetaOapg.max_properties
-        ):
+        if (cls._is_json_validation_enabled_oapg('maxProperties', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'max_properties') and
+                len(arg) > cls.MetaOapg.max_properties):
             cls._raise_validation_error_message_oapg(
                 value=arg,
                 constraint_msg="number of properties must be less than or equal to",
                 constraint_value=cls.MetaOapg.max_properties,
-                path_to_item=validation_metadata.path_to_item,
+                path_to_item=validation_metadata.path_to_item
             )
 
-        if (
-            cls._is_json_validation_enabled_oapg(
-                "minProperties", validation_metadata.configuration
-            )
-            and hasattr(cls.MetaOapg, "min_properties")
-            and len(arg) < cls.MetaOapg.min_properties
-        ):
+        if (cls._is_json_validation_enabled_oapg('minProperties', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'min_properties') and
+                len(arg) < cls.MetaOapg.min_properties):
             cls._raise_validation_error_message_oapg(
                 value=arg,
                 constraint_msg="number of properties must be greater than or equal to",
                 constraint_value=cls.MetaOapg.min_properties,
-                path_to_item=validation_metadata.path_to_item,
+                path_to_item=validation_metadata.path_to_item
             )
 
     @classmethod
     def _validate_oapg(
         cls,
         arg,
         validation_metadata: ValidationMetadata,
@@ -2081,91 +1662,80 @@
 
         Raises:
             ApiValueError: when a string can't be converted into a date or datetime and it must be one of those classes
             ApiTypeError: when the input type is not in the list of allowed spec types
         """
         if isinstance(arg, frozendict.frozendict):
             cls.__check_dict_validations(arg, validation_metadata)
-        _path_to_schemas = super()._validate_oapg(
-            arg, validation_metadata=validation_metadata
-        )
+        _path_to_schemas = super()._validate_oapg(arg, validation_metadata=validation_metadata)
         if not isinstance(arg, frozendict.frozendict):
             return _path_to_schemas
         cls.__validate_arg_presence(arg)
-        other_path_to_schemas = cls.__validate_args(
-            arg, validation_metadata=validation_metadata
-        )
+        other_path_to_schemas = cls.__validate_args(arg, validation_metadata=validation_metadata)
         update(_path_to_schemas, other_path_to_schemas)
         try:
             discriminator = cls.MetaOapg.discriminator()
         except AttributeError:
             return _path_to_schemas
         # discriminator exists
         disc_prop_name = list(discriminator.keys())[0]
-        cls._ensure_discriminator_value_present_oapg(
-            disc_prop_name, validation_metadata, arg
-        )
+        cls._ensure_discriminator_value_present_oapg(disc_prop_name, validation_metadata, arg)
         discriminated_cls = cls.get_discriminated_class_oapg(
-            disc_property_name=disc_prop_name, disc_payload_value=arg[disc_prop_name]
-        )
+            disc_property_name=disc_prop_name, disc_payload_value=arg[disc_prop_name])
         if discriminated_cls is None:
             raise ApiValueError(
                 "Invalid discriminator value was passed in to {}.{} Only the values {} are allowed at {}".format(
                     cls.__name__,
                     disc_prop_name,
                     list(discriminator[disc_prop_name].keys()),
-                    validation_metadata.path_to_item + (disc_prop_name,),
+                    validation_metadata.path_to_item + (disc_prop_name,)
                 )
             )
         updated_vm = ValidationMetadata(
             configuration=validation_metadata.configuration,
             from_server=validation_metadata.from_server,
             path_to_item=validation_metadata.path_to_item,
             seen_classes=validation_metadata.seen_classes | frozenset({cls}),
-            validated_path_to_schemas=validation_metadata.validated_path_to_schemas,
+            validated_path_to_schemas=validation_metadata.validated_path_to_schemas
         )
         if updated_vm.validation_ran_earlier(discriminated_cls):
             add_deeper_validated_schemas(updated_vm, _path_to_schemas)
             return _path_to_schemas
-        other_path_to_schemas = discriminated_cls._validate_oapg(
-            arg, validation_metadata=updated_vm
-        )
+        other_path_to_schemas = discriminated_cls._validate_oapg(arg, validation_metadata=updated_vm)
         update(_path_to_schemas, other_path_to_schemas)
         return _path_to_schemas
 
     @classmethod
     def _get_properties_oapg(
         cls,
         arg: typing.Dict[str, typing.Any],
         path_to_item: typing.Tuple[typing.Union[str, int], ...],
-        path_to_schemas: typing.Dict[
-            typing.Tuple[typing.Union[str, int], ...], typing.Type["Schema"]
-        ],
+        path_to_schemas: typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Type['Schema']]
     ):
         """
         DictBase _get_properties_oapg, this is how properties are set
         These values already passed validation
         """
         dict_items = {}
 
         for property_name_js, value in arg.items():
             property_path_to_item = path_to_item + (property_name_js,)
             property_cls = path_to_schemas[property_path_to_item]
             new_value = property_cls._get_new_instance_without_conversion_oapg(
-                value, property_path_to_item, path_to_schemas
+                value,
+                property_path_to_item,
+                path_to_schemas
             )
             dict_items[property_name_js] = new_value
 
         return dict_items
 
     def __setattr__(self, name: str, value: typing.Any):
         if not isinstance(self, FileIO):
-            raise AttributeError(
-                "property setting not supported on immutable instances"
-            )
+            raise AttributeError('property setting not supported on immutable instances')
 
     def __getattr__(self, name: str):
         """
         for instance.name access
         Properties are only type hinted for required properties
         so that hasattr(instance, 'optionalProp') is False when that key is not present
         """
@@ -2184,69 +1754,30 @@
         dict_instance[name] accessor
         key errors thrown
         """
         if not isinstance(self, frozendict.frozendict):
             return super().__getattr__(name)
         return super().__getitem__(name)
 
-    def get_item_oapg(self, name: str) -> typing.Union["AnyTypeSchema", Unset]:
+    def get_item_oapg(self, name: str) -> typing.Union['AnyTypeSchema', Unset]:
         # dict_instance[name] accessor
         if not isinstance(self, frozendict.frozendict):
             raise NotImplementedError()
         try:
             return super().__getitem__(name)
         except KeyError:
             return unset
 
 
 def cast_to_allowed_types(
-    arg: typing.Union[
-        str,
-        date,
-        datetime,
-        uuid.UUID,
-        decimal.Decimal,
-        int,
-        float,
-        None,
-        dict,
-        frozendict.frozendict,
-        list,
-        tuple,
-        bytes,
-        Schema,
-        io.FileIO,
-        io.BufferedReader,
-    ],
+    arg: typing.Union[str, date, datetime, uuid.UUID, decimal.Decimal, int, float, None, dict, frozendict.frozendict, list, tuple, bytes, Schema, io.FileIO, io.BufferedReader],
     from_server: bool,
-    validated_path_to_schemas: typing.Dict[
-        typing.Tuple[typing.Union[str, int], ...],
-        typing.Set[
-            typing.Union[
-                "Schema",
-                str,
-                decimal.Decimal,
-                BoolClass,
-                NoneClass,
-                frozendict.frozendict,
-                tuple,
-            ]
-        ],
-    ],
-    path_to_item: typing.Tuple[typing.Union[str, int], ...] = tuple(["args[0]"]),
-) -> typing.Union[
-    frozendict.frozendict,
-    tuple,
-    decimal.Decimal,
-    str,
-    bytes,
-    BoolClass,
-    NoneClass,
-    FileIO,
-]:
+    validated_path_to_schemas: typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]],
+    path_to_item: typing.Tuple[typing.Union[str, int], ...] = tuple(['args[0]']),
+) -> typing.Union[frozendict.frozendict, tuple, decimal.Decimal, str, bytes, BoolClass, NoneClass, FileIO]:
     """
     Casts the input payload arg into the allowed types
     The input validated_path_to_schemas is mutated by running this function
 
     When from_server is False then
     - date/datetime is cast to str
     - int/float is cast to Decimal
@@ -2269,28 +1800,19 @@
         for cls in arg.__class__.__bases__:
             if cls is Singleton:
                 # Skip Singleton
                 continue
             schema_classes.add(cls)
         validated_path_to_schemas[path_to_item] = schema_classes
 
-    type_error = ApiTypeError(
-        f"Invalid type. Required value type is str and passed type was {type(arg)} at {path_to_item}"
-    )
+    type_error = ApiTypeError(f"Invalid type. Required value type is str and passed type was {type(arg)} at {path_to_item}")
     if isinstance(arg, str):
         return str(arg)
     elif isinstance(arg, (dict, frozendict.frozendict)):
-        return frozendict.frozendict(
-            {
-                key: cast_to_allowed_types(
-                    val, from_server, validated_path_to_schemas, path_to_item + (key,)
-                )
-                for key, val in arg.items()
-            }
-        )
+        return frozendict.frozendict({key: cast_to_allowed_types(val, from_server, validated_path_to_schemas, path_to_item + (key,)) for key, val in arg.items()})
     elif isinstance(arg, (bool, BoolClass)):
         """
         this check must come before isinstance(arg, (int, float))
         because isinstance(True, int) is True
         """
         if arg:
             return BoolClass.TRUE
@@ -2298,25 +1820,18 @@
     elif isinstance(arg, int):
         return decimal.Decimal(arg)
     elif isinstance(arg, float):
         decimal_from_float = decimal.Decimal(arg)
         if decimal_from_float.as_integer_ratio()[1] == 1:
             # 9.0 -> Decimal('9.0')
             # 3.4028234663852886e+38 -> Decimal('340282346638528859811704183484516925440.0')
-            return decimal.Decimal(str(decimal_from_float) + ".0")
+            return decimal.Decimal(str(decimal_from_float)+'.0')
         return decimal_from_float
     elif isinstance(arg, (tuple, list)):
-        return tuple(
-            [
-                cast_to_allowed_types(
-                    item, from_server, validated_path_to_schemas, path_to_item + (i,)
-                )
-                for i, item in enumerate(arg)
-            ]
-        )
+        return tuple([cast_to_allowed_types(item, from_server, validated_path_to_schemas, path_to_item + (i,)) for i, item in enumerate(arg)])
     elif isinstance(arg, (none_type, NoneClass)):
         return NoneClass.NONE
     elif isinstance(arg, (date, datetime)):
         if not from_server:
             return arg.isoformat()
         raise type_error
     elif isinstance(arg, uuid.UUID):
@@ -2325,30 +1840,27 @@
         raise type_error
     elif isinstance(arg, decimal.Decimal):
         return decimal.Decimal(arg)
     elif isinstance(arg, bytes):
         return bytes(arg)
     elif isinstance(arg, (io.FileIO, io.BufferedReader)):
         return FileIO(arg)
-    raise ValueError(
-        "Invalid type passed in got input={} type={}".format(arg, type(arg))
-    )
+    raise ValueError('Invalid type passed in got input={} type={}'.format(arg, type(arg)))
 
 
 class ComposedBase(Discriminable):
+
     @classmethod
     def __get_allof_classes(cls, arg, validation_metadata: ValidationMetadata):
         path_to_schemas = defaultdict(set)
         for allof_cls in cls.MetaOapg.all_of():
             if validation_metadata.validation_ran_earlier(allof_cls):
                 add_deeper_validated_schemas(validation_metadata, path_to_schemas)
                 continue
-            other_path_to_schemas = allof_cls._validate_oapg(
-                arg, validation_metadata=validation_metadata
-            )
+            other_path_to_schemas = allof_cls._validate_oapg(arg, validation_metadata=validation_metadata)
             update(path_to_schemas, other_path_to_schemas)
         return path_to_schemas
 
     @classmethod
     def __get_oneof_class(
         cls,
         arg,
@@ -2362,53 +1874,50 @@
                 oneof_classes.append(oneof_cls)
                 continue
             if validation_metadata.validation_ran_earlier(oneof_cls):
                 oneof_classes.append(oneof_cls)
                 add_deeper_validated_schemas(validation_metadata, path_to_schemas)
                 continue
             try:
-                path_to_schemas = oneof_cls._validate_oapg(
-                    arg, validation_metadata=validation_metadata
-                )
+                path_to_schemas = oneof_cls._validate_oapg(arg, validation_metadata=validation_metadata)
             except (ApiValueError, ApiTypeError) as ex:
                 if discriminated_cls is not None and oneof_cls is discriminated_cls:
                     raise ex
                 continue
             oneof_classes.append(oneof_cls)
         if not oneof_classes:
             raise ApiValueError(
                 "Invalid inputs given to generate an instance of {}. None "
                 "of the oneOf schemas matched the input data.".format(cls)
             )
         elif len(oneof_classes) > 1:
             raise ApiValueError(
                 "Invalid inputs given to generate an instance of {}. Multiple "
-                "oneOf schemas {} matched the inputs, but a max of one is allowed.".format(
-                    cls, oneof_classes
-                )
+                "oneOf schemas {} matched the inputs, but a max of one is allowed.".format(cls, oneof_classes)
             )
         # exactly one class matches
         return path_to_schemas
 
     @classmethod
     def __get_anyof_classes(
-        cls, arg, discriminated_cls, validation_metadata: ValidationMetadata
+        cls,
+        arg,
+        discriminated_cls,
+        validation_metadata: ValidationMetadata
     ):
         anyof_classes = []
         path_to_schemas = defaultdict(set)
         for anyof_cls in cls.MetaOapg.any_of():
             if validation_metadata.validation_ran_earlier(anyof_cls):
                 anyof_classes.append(anyof_cls)
                 add_deeper_validated_schemas(validation_metadata, path_to_schemas)
                 continue
 
             try:
-                other_path_to_schemas = anyof_cls._validate_oapg(
-                    arg, validation_metadata=validation_metadata
-                )
+                other_path_to_schemas = anyof_cls._validate_oapg(arg, validation_metadata=validation_metadata)
             except (ApiValueError, ApiTypeError) as ex:
                 if discriminated_cls is not None and anyof_cls is discriminated_cls:
                     raise ex
                 continue
             anyof_classes.append(anyof_cls)
             update(path_to_schemas, other_path_to_schemas)
         if not anyof_classes:
@@ -2419,28 +1928,15 @@
         return path_to_schemas
 
     @classmethod
     def _validate_oapg(
         cls,
         arg,
         validation_metadata: ValidationMetadata,
-    ) -> typing.Dict[
-        typing.Tuple[typing.Union[str, int], ...],
-        typing.Set[
-            typing.Union[
-                "Schema",
-                str,
-                decimal.Decimal,
-                BoolClass,
-                NoneClass,
-                frozendict.frozendict,
-                tuple,
-            ]
-        ],
-    ]:
+    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]]:
         """
         ComposedBase _validate_oapg
         We return dynamic classes of different bases depending upon the inputs
         This makes it so:
         - the returned instance is always a subclass of our defining schema
             - this allows us to check type based on whether an instance is a subclass of a schema
         - the returned instance is a serializable type (except for None, True, and False) which are enums
@@ -2449,69 +1945,65 @@
             new_cls (type): the new class
 
         Raises:
             ApiValueError: when a string can't be converted into a date or datetime and it must be one of those classes
             ApiTypeError: when the input type is not in the list of allowed spec types
         """
         # validation checking on types, validations, and enums
-        path_to_schemas = super()._validate_oapg(
-            arg, validation_metadata=validation_metadata
-        )
+        path_to_schemas = super()._validate_oapg(arg, validation_metadata=validation_metadata)
 
         updated_vm = ValidationMetadata(
             configuration=validation_metadata.configuration,
             from_server=validation_metadata.from_server,
             path_to_item=validation_metadata.path_to_item,
             seen_classes=validation_metadata.seen_classes | frozenset({cls}),
-            validated_path_to_schemas=validation_metadata.validated_path_to_schemas,
+            validated_path_to_schemas=validation_metadata.validated_path_to_schemas
         )
 
         # process composed schema
         discriminator = None
-        if hasattr(cls, "MetaOapg") and hasattr(cls.MetaOapg, "discriminator"):
+        if hasattr(cls, 'MetaOapg') and hasattr(cls.MetaOapg, 'discriminator'):
             discriminator = cls.MetaOapg.discriminator()
         discriminated_cls = None
         if discriminator and arg and isinstance(arg, frozendict.frozendict):
             disc_property_name = list(discriminator.keys())[0]
-            cls._ensure_discriminator_value_present_oapg(
-                disc_property_name, updated_vm, arg
-            )
+            cls._ensure_discriminator_value_present_oapg(disc_property_name, updated_vm, arg)
             # get discriminated_cls by looking at the dict in the current class
             discriminated_cls = cls.get_discriminated_class_oapg(
-                disc_property_name=disc_property_name,
-                disc_payload_value=arg[disc_property_name],
-            )
+                disc_property_name=disc_property_name, disc_payload_value=arg[disc_property_name])
             if discriminated_cls is None:
                 raise ApiValueError(
                     "Invalid discriminator value '{}' was passed in to {}.{} Only the values {} are allowed at {}".format(
                         arg[disc_property_name],
                         cls.__name__,
                         disc_property_name,
                         list(discriminator[disc_property_name].keys()),
-                        updated_vm.path_to_item + (disc_property_name,),
+                        updated_vm.path_to_item + (disc_property_name,)
                     )
                 )
 
-        if hasattr(cls, "MetaOapg") and hasattr(cls.MetaOapg, "all_of"):
-            other_path_to_schemas = cls.__get_allof_classes(
-                arg, validation_metadata=updated_vm
-            )
+        if hasattr(cls, 'MetaOapg') and hasattr(cls.MetaOapg, 'all_of'):
+            other_path_to_schemas = cls.__get_allof_classes(arg, validation_metadata=updated_vm)
             update(path_to_schemas, other_path_to_schemas)
-        if hasattr(cls, "MetaOapg") and hasattr(cls.MetaOapg, "one_of"):
+        if hasattr(cls, 'MetaOapg') and hasattr(cls.MetaOapg, 'one_of'):
             other_path_to_schemas = cls.__get_oneof_class(
-                arg, discriminated_cls=discriminated_cls, validation_metadata=updated_vm
+                arg,
+                discriminated_cls=discriminated_cls,
+                validation_metadata=updated_vm
             )
             update(path_to_schemas, other_path_to_schemas)
-        if hasattr(cls, "MetaOapg") and hasattr(cls.MetaOapg, "any_of"):
+        if hasattr(cls, 'MetaOapg') and hasattr(cls.MetaOapg, 'any_of'):
             other_path_to_schemas = cls.__get_anyof_classes(
-                arg, discriminated_cls=discriminated_cls, validation_metadata=updated_vm
+                arg,
+                discriminated_cls=discriminated_cls,
+                validation_metadata=updated_vm
             )
             update(path_to_schemas, other_path_to_schemas)
         not_cls = None
-        if hasattr(cls, "MetaOapg") and hasattr(cls.MetaOapg, "not_schema"):
+        if hasattr(cls, 'MetaOapg') and hasattr(cls.MetaOapg, 'not_schema'):
             not_cls = cls.MetaOapg.not_schema
             not_cls = cls._get_class_oapg(not_cls)
         if not_cls:
             other_path_to_schemas = None
             not_exception = ApiValueError(
                 "Invalid value '{}' was passed in to {}. Value is invalid because it is disallowed by {}".format(
                     arg,
@@ -2519,25 +2011,21 @@
                     not_cls.__name__,
                 )
             )
             if updated_vm.validation_ran_earlier(not_cls):
                 raise not_exception
 
             try:
-                other_path_to_schemas = not_cls._validate_oapg(
-                    arg, validation_metadata=updated_vm
-                )
+                other_path_to_schemas = not_cls._validate_oapg(arg, validation_metadata=updated_vm)
             except (ApiValueError, ApiTypeError):
                 pass
             if other_path_to_schemas:
                 raise not_exception
 
-        if discriminated_cls is not None and not updated_vm.validation_ran_earlier(
-            discriminated_cls
-        ):
+        if discriminated_cls is not None and not updated_vm.validation_ran_earlier(discriminated_cls):
             # TODO use an exception from this package here
             add_deeper_validated_schemas(updated_vm, path_to_schemas)
             assert discriminated_cls in path_to_schemas[updated_vm.path_to_item]
         return path_to_schemas
 
 
 # DictBase, ListBase, NumberBase, StrBase, BoolBase, NoneBase
@@ -2546,104 +2034,88 @@
     DictBase,
     ListBase,
     NumberBase,
     StrBase,
     BoolBase,
     NoneBase,
     Schema,
-    NoneFrozenDictTupleStrDecimalBoolMixin,
+    NoneFrozenDictTupleStrDecimalBoolMixin
 ):
     @classmethod
-    def from_openapi_data_oapg(
-        cls,
-        *args: typing.Any,
-        _configuration: typing.Optional[Configuration] = None,
-        **kwargs,
-    ):
+    def from_openapi_data_oapg(cls, *args: typing.Any, _configuration: typing.Optional[Configuration] = None, **kwargs):
         if not args:
             if not kwargs:
-                raise ApiTypeError(
-                    "{} is missing required input data in args or kwargs".format(
-                        cls.__name__
-                    )
-                )
-            args = (kwargs,)
+                raise ApiTypeError('{} is missing required input data in args or kwargs'.format(cls.__name__))
+            args = (kwargs, )
         return super().from_openapi_data_oapg(args[0], _configuration=_configuration)
 
 
-class ListSchema(ListBase, Schema, TupleMixin):
+class ListSchema(
+    ListBase,
+    Schema,
+    TupleMixin
+):
+
     @classmethod
-    def from_openapi_data_oapg(
-        cls,
-        arg: typing.List[typing.Any],
-        _configuration: typing.Optional[Configuration] = None,
-    ):
+    def from_openapi_data_oapg(cls, arg: typing.List[typing.Any], _configuration: typing.Optional[Configuration] = None):
         return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
-    def __new__(
-        cls,
-        _arg: typing.Union[typing.List[typing.Any], typing.Tuple[typing.Any]],
-        **kwargs: Configuration,
-    ):
+    def __new__(cls, _arg: typing.Union[typing.List[typing.Any], typing.Tuple[typing.Any]], **kwargs: Configuration):
         return super().__new__(cls, _arg, **kwargs)
 
 
-class NoneSchema(NoneBase, Schema, NoneMixin):
+class NoneSchema(
+    NoneBase,
+    Schema,
+    NoneMixin
+):
+
     @classmethod
-    def from_openapi_data_oapg(
-        cls, arg: None, _configuration: typing.Optional[Configuration] = None
-    ):
+    def from_openapi_data_oapg(cls, arg: None, _configuration: typing.Optional[Configuration] = None):
         return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
     def __new__(cls, _arg: None, **kwargs: Configuration):
         return super().__new__(cls, _arg, **kwargs)
 
 
-class NumberSchema(NumberBase, Schema, DecimalMixin):
+class NumberSchema(
+    NumberBase,
+    Schema,
+    DecimalMixin
+):
     """
     This is used for type: number with no format
     Both integers AND floats are accepted
     """
 
     @classmethod
-    def from_openapi_data_oapg(
-        cls,
-        arg: typing.Union[int, float],
-        _configuration: typing.Optional[Configuration] = None,
-    ):
+    def from_openapi_data_oapg(cls, arg: typing.Union[int, float], _configuration: typing.Optional[Configuration] = None):
         return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
-    def __new__(
-        cls, _arg: typing.Union[decimal.Decimal, int, float], **kwargs: Configuration
-    ):
+    def __new__(cls, _arg: typing.Union[decimal.Decimal, int, float], **kwargs: Configuration):
         return super().__new__(cls, _arg, **kwargs)
 
 
 class IntBase:
     @property
     def as_int_oapg(self) -> int:
         try:
             return self._as_int
         except AttributeError:
             self._as_int = int(self)
             return self._as_int
 
     @classmethod
-    def __validate_format(
-        cls,
-        arg: typing.Optional[decimal.Decimal],
-        validation_metadata: ValidationMetadata,
-    ):
+    def __validate_format(cls, arg: typing.Optional[decimal.Decimal], validation_metadata: ValidationMetadata):
         if isinstance(arg, decimal.Decimal):
+
             denominator = arg.as_integer_ratio()[-1]
             if denominator != 1:
                 raise ApiValueError(
-                    "Invalid value '{}' for type integer at {}".format(
-                        arg, validation_metadata.path_to_item
-                    )
+                    "Invalid value '{}' for type integer at {}".format(arg, validation_metadata.path_to_item)
                 )
 
     @classmethod
     def _validate_oapg(
         cls,
         arg,
         validation_metadata: ValidationMetadata,
@@ -2653,40 +2125,33 @@
         TODO what about types = (int, number) -> IntBase, NumberBase? We could drop int and keep number only
         """
         cls.__validate_format(arg, validation_metadata=validation_metadata)
         return super()._validate_oapg(arg, validation_metadata=validation_metadata)
 
 
 class IntSchema(IntBase, NumberSchema):
+
     @classmethod
-    def from_openapi_data_oapg(
-        cls, arg: int, _configuration: typing.Optional[Configuration] = None
-    ):
+    def from_openapi_data_oapg(cls, arg: int, _configuration: typing.Optional[Configuration] = None):
         return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
     def __new__(cls, _arg: typing.Union[decimal.Decimal, int], **kwargs: Configuration):
         return super().__new__(cls, _arg, **kwargs)
 
 
 class Int32Base:
     __inclusive_minimum = decimal.Decimal(-2147483648)
     __inclusive_maximum = decimal.Decimal(2147483647)
 
     @classmethod
-    def __validate_format(
-        cls,
-        arg: typing.Optional[decimal.Decimal],
-        validation_metadata: ValidationMetadata,
-    ):
+    def __validate_format(cls, arg: typing.Optional[decimal.Decimal], validation_metadata: ValidationMetadata):
         if isinstance(arg, decimal.Decimal) and arg.as_tuple().exponent == 0:
             if not cls.__inclusive_minimum <= arg <= cls.__inclusive_maximum:
                 raise ApiValueError(
-                    "Invalid value '{}' for type int32 at {}".format(
-                        arg, validation_metadata.path_to_item
-                    )
+                    "Invalid value '{}' for type int32 at {}".format(arg, validation_metadata.path_to_item)
                 )
 
     @classmethod
     def _validate_oapg(
         cls,
         arg,
         validation_metadata: ValidationMetadata,
@@ -2694,34 +2159,31 @@
         """
         Int32Base _validate_oapg
         """
         cls.__validate_format(arg, validation_metadata=validation_metadata)
         return super()._validate_oapg(arg, validation_metadata=validation_metadata)
 
 
-class Int32Schema(Int32Base, IntSchema):
+class Int32Schema(
+    Int32Base,
+    IntSchema
+):
     pass
 
 
 class Int64Base:
     __inclusive_minimum = decimal.Decimal(-9223372036854775808)
     __inclusive_maximum = decimal.Decimal(9223372036854775807)
 
     @classmethod
-    def __validate_format(
-        cls,
-        arg: typing.Optional[decimal.Decimal],
-        validation_metadata: ValidationMetadata,
-    ):
+    def __validate_format(cls, arg: typing.Optional[decimal.Decimal], validation_metadata: ValidationMetadata):
         if isinstance(arg, decimal.Decimal) and arg.as_tuple().exponent == 0:
             if not cls.__inclusive_minimum <= arg <= cls.__inclusive_maximum:
                 raise ApiValueError(
-                    "Invalid value '{}' for type int64 at {}".format(
-                        arg, validation_metadata.path_to_item
-                    )
+                    "Invalid value '{}' for type int64 at {}".format(arg, validation_metadata.path_to_item)
                 )
 
     @classmethod
     def _validate_oapg(
         cls,
         arg,
         validation_metadata: ValidationMetadata,
@@ -2729,34 +2191,31 @@
         """
         Int64Base _validate_oapg
         """
         cls.__validate_format(arg, validation_metadata=validation_metadata)
         return super()._validate_oapg(arg, validation_metadata=validation_metadata)
 
 
-class Int64Schema(Int64Base, IntSchema):
+class Int64Schema(
+    Int64Base,
+    IntSchema
+):
     pass
 
 
 class Float32Base:
-    __inclusive_minimum = decimal.Decimal(-3.4028234663852886e38)
-    __inclusive_maximum = decimal.Decimal(3.4028234663852886e38)
+    __inclusive_minimum = decimal.Decimal(-3.4028234663852886e+38)
+    __inclusive_maximum = decimal.Decimal(3.4028234663852886e+38)
 
     @classmethod
-    def __validate_format(
-        cls,
-        arg: typing.Optional[decimal.Decimal],
-        validation_metadata: ValidationMetadata,
-    ):
+    def __validate_format(cls, arg: typing.Optional[decimal.Decimal], validation_metadata: ValidationMetadata):
         if isinstance(arg, decimal.Decimal):
             if not cls.__inclusive_minimum <= arg <= cls.__inclusive_maximum:
                 raise ApiValueError(
-                    "Invalid value '{}' for type float at {}".format(
-                        arg, validation_metadata.path_to_item
-                    )
+                    "Invalid value '{}' for type float at {}".format(arg, validation_metadata.path_to_item)
                 )
 
     @classmethod
     def _validate_oapg(
         cls,
         arg,
         validation_metadata: ValidationMetadata,
@@ -2764,120 +2223,126 @@
         """
         Float32Base _validate_oapg
         """
         cls.__validate_format(arg, validation_metadata=validation_metadata)
         return super()._validate_oapg(arg, validation_metadata=validation_metadata)
 
 
-class Float32Schema(Float32Base, NumberSchema):
+class Float32Schema(
+    Float32Base,
+    NumberSchema
+):
+
     @classmethod
-    def from_openapi_data_oapg(
-        cls, arg: float, _configuration: typing.Optional[Configuration] = None
-    ):
+    def from_openapi_data_oapg(cls, arg: float, _configuration: typing.Optional[Configuration] = None):
         return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
 
 class Float64Base:
-    __inclusive_minimum = decimal.Decimal(-1.7976931348623157e308)
-    __inclusive_maximum = decimal.Decimal(1.7976931348623157e308)
+    __inclusive_minimum = decimal.Decimal(-1.7976931348623157E+308)
+    __inclusive_maximum = decimal.Decimal(1.7976931348623157E+308)
 
     @classmethod
-    def __validate_format(
-        cls,
-        arg: typing.Optional[decimal.Decimal],
-        validation_metadata: ValidationMetadata,
-    ):
+    def __validate_format(cls, arg: typing.Optional[decimal.Decimal], validation_metadata: ValidationMetadata):
         if isinstance(arg, decimal.Decimal):
             if not cls.__inclusive_minimum <= arg <= cls.__inclusive_maximum:
                 raise ApiValueError(
-                    "Invalid value '{}' for type double at {}".format(
-                        arg, validation_metadata.path_to_item
-                    )
+                    "Invalid value '{}' for type double at {}".format(arg, validation_metadata.path_to_item)
                 )
 
     @classmethod
     def _validate_oapg(
         cls,
         arg,
         validation_metadata: ValidationMetadata,
     ):
         """
         Float64Base _validate_oapg
         """
         cls.__validate_format(arg, validation_metadata=validation_metadata)
         return super()._validate_oapg(arg, validation_metadata=validation_metadata)
 
+class Float64Schema(
+    Float64Base,
+    NumberSchema
+):
 
-class Float64Schema(Float64Base, NumberSchema):
     @classmethod
-    def from_openapi_data_oapg(
-        cls, arg: float, _configuration: typing.Optional[Configuration] = None
-    ):
+    def from_openapi_data_oapg(cls, arg: float, _configuration: typing.Optional[Configuration] = None):
         # todo check format
         return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
 
-class StrSchema(StrBase, Schema, StrMixin):
+class StrSchema(
+    StrBase,
+    Schema,
+    StrMixin
+):
     """
     date + datetime string types must inherit from this class
     That is because one can validate a str payload as both:
     - type: string (format unset)
     - type: string, format: date
     """
 
     @classmethod
-    def from_openapi_data_oapg(
-        cls, arg: str, _configuration: typing.Optional[Configuration] = None
-    ) -> "StrSchema":
+    def from_openapi_data_oapg(cls, arg: str, _configuration: typing.Optional[Configuration] = None) -> 'StrSchema':
         return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
-    def __new__(
-        cls, _arg: typing.Union[str, date, datetime, uuid.UUID], **kwargs: Configuration
-    ):
+    def __new__(cls, _arg: typing.Union[str, date, datetime, uuid.UUID], **kwargs: Configuration):
         return super().__new__(cls, _arg, **kwargs)
 
 
 class UUIDSchema(UUIDBase, StrSchema):
+
     def __new__(cls, _arg: typing.Union[str, uuid.UUID], **kwargs: Configuration):
         return super().__new__(cls, _arg, **kwargs)
 
 
 class DateSchema(DateBase, StrSchema):
+
     def __new__(cls, _arg: typing.Union[str, date], **kwargs: Configuration):
         return super().__new__(cls, _arg, **kwargs)
 
 
 class DateTimeSchema(DateTimeBase, StrSchema):
+
     def __new__(cls, _arg: typing.Union[str, datetime], **kwargs: Configuration):
         return super().__new__(cls, _arg, **kwargs)
 
 
 class DecimalSchema(DecimalBase, StrSchema):
+
     def __new__(cls, _arg: str, **kwargs: Configuration):
         """
         Note: Decimals may not be passed in because cast_to_allowed_types is only invoked once for payloads
         which can be simple (str) or complex (dicts or lists with nested values)
         Because casting is only done once and recursively casts all values prior to validation then for a potential
         client side Decimal input if Decimal was accepted as an input in DecimalSchema then one would not know
         if one was using it for a StrSchema (where it should be cast to str) or one is using it for NumberSchema
         where it should stay as Decimal.
         """
         return super().__new__(cls, _arg, **kwargs)
 
 
-class BytesSchema(Schema, BytesMixin):
+class BytesSchema(
+    Schema,
+    BytesMixin
+):
     """
     this class will subclass bytes and is immutable
     """
-
     def __new__(cls, _arg: bytes, **kwargs: Configuration):
         return super(Schema, cls).__new__(cls, _arg)
 
 
-class FileSchema(Schema, FileMixin):
+class FileSchema(
+    Schema,
+    FileMixin
+):
     """
     This class is NOT immutable
     Dynamic classes are built using it for example when AnyType allows in binary data
     Al other schema classes ARE immutable
     If one wanted to make this immutable one could make this a DictSchema with required properties:
     - data = BytesSchema (which would be an immutable bytes based schema)
     - file_name = StrSchema
@@ -2887,61 +2352,63 @@
     The developer is responsible for closing this file and deleting it
 
     This class was kept as mutable:
     - to allow file reading and writing to disk
     - to be able to preserve file name info
     """
 
-    def __new__(
-        cls, _arg: typing.Union[io.FileIO, io.BufferedReader], **kwargs: Configuration
-    ):
+    def __new__(cls, _arg: typing.Union[io.FileIO, io.BufferedReader], **kwargs: Configuration):
         return super(Schema, cls).__new__(cls, _arg)
 
 
 class BinaryBase:
     pass
 
 
-class BinarySchema(ComposedBase, BinaryBase, Schema, BinaryMixin):
+class BinarySchema(
+    ComposedBase,
+    BinaryBase,
+    Schema,
+    BinaryMixin
+):
     class MetaOapg:
         @staticmethod
         def one_of():
             return [
                 BytesSchema,
                 FileSchema,
             ]
 
-    def __new__(
-        cls,
-        _arg: typing.Union[io.FileIO, io.BufferedReader, bytes],
-        **kwargs: Configuration,
-    ):
+    def __new__(cls, _arg: typing.Union[io.FileIO, io.BufferedReader, bytes], **kwargs: Configuration):
         return super().__new__(cls, _arg)
 
 
-class BoolSchema(BoolBase, Schema, BoolMixin):
+class BoolSchema(
+    BoolBase,
+    Schema,
+    BoolMixin
+):
+
     @classmethod
-    def from_openapi_data_oapg(
-        cls, arg: bool, _configuration: typing.Optional[Configuration] = None
-    ):
+    def from_openapi_data_oapg(cls, arg: bool, _configuration: typing.Optional[Configuration] = None):
         return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
     def __new__(cls, _arg: bool, **kwargs: ValidationMetadata):
         return super().__new__(cls, _arg, **kwargs)
 
 
 class AnyTypeSchema(
     DictBase,
     ListBase,
     NumberBase,
     StrBase,
     BoolBase,
     NoneBase,
     Schema,
-    NoneFrozenDictTupleStrDecimalBoolFileBytesMixin,
+    NoneFrozenDictTupleStrDecimalBoolFileBytesMixin
 ):
     # Python representation of a schema defined as true or {}
     pass
 
 
 class UnsetAnyTypeSchema(AnyTypeSchema):
     # Used when additionalProperties/items was not explicitly defined and a defining schema is needed
@@ -2960,78 +2427,49 @@
     class MetaOapg:
         not_schema = AnyTypeSchema
 
     def __new__(
         cls,
         *_args,
         _configuration: typing.Optional[Configuration] = None,
-    ) -> "NotAnyTypeSchema":
+    ) -> 'NotAnyTypeSchema':
         return super().__new__(
             cls,
             *_args,
             _configuration=_configuration,
         )
 
 
-class DictSchema(DictBase, Schema, FrozenDictMixin):
+class DictSchema(
+    DictBase,
+    Schema,
+    FrozenDictMixin
+):
     @classmethod
-    def from_openapi_data_oapg(
-        cls,
-        arg: typing.Dict[str, typing.Any],
-        _configuration: typing.Optional[Configuration] = None,
-    ):
+    def from_openapi_data_oapg(cls, arg: typing.Dict[str, typing.Any], _configuration: typing.Optional[Configuration] = None):
         return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict],
-        **kwargs: typing.Union[
-            dict,
-            frozendict.frozendict,
-            list,
-            tuple,
-            decimal.Decimal,
-            float,
-            int,
-            str,
-            date,
-            datetime,
-            bool,
-            None,
-            bytes,
-            Schema,
-            Unset,
-            ValidationMetadata,
-        ],
-    ):
+    def __new__(cls, *_args: typing.Union[dict, frozendict.frozendict], **kwargs: typing.Union[dict, frozendict.frozendict, list, tuple, decimal.Decimal, float, int, str, date, datetime, bool, None, bytes, Schema, Unset, ValidationMetadata]):
         return super().__new__(cls, *_args, **kwargs)
 
 
-schema_type_classes = {
-    NoneSchema,
-    DictSchema,
-    ListSchema,
-    NumberSchema,
-    StrSchema,
-    BoolSchema,
-    AnyTypeSchema,
-}
+schema_type_classes = {NoneSchema, DictSchema, ListSchema, NumberSchema, StrSchema, BoolSchema, AnyTypeSchema}
 
 
 @functools.lru_cache()
 def get_new_class(
     class_name: str,
-    bases: typing.Tuple[typing.Type[typing.Union[Schema, typing.Any]], ...],
+    bases: typing.Tuple[typing.Type[typing.Union[Schema, typing.Any]], ...]
 ) -> typing.Type[Schema]:
     """
     Returns a new class that is made with the subclass bases
     """
     new_cls: typing.Type[Schema] = type(class_name, bases, {})
     return new_cls
 
 
 LOG_CACHE_USAGE = False
 
 
 def log_cache_usage(cache_fn):
     if LOG_CACHE_USAGE:
-        print(cache_fn.__name__, cache_fn.cache_info())
+        print(cache_fn.__name__, cache_fn.cache_info())
```

### Comparing `gentrace_py-0.7.4/pyproject.toml` & `gentrace_py-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Python SDK for the Gentrace API"
 license = "MIT"
 name = "gentrace-py"
 packages = [
   {include = "gentrace"},
 ]
 repository = "https://github.com/gentrace/gentrace-python"
-version = "0.7.4"
+version = "0.8.0"
 
 [tool.poetry.dependencies]
 aenum = ">=3.1.11"
 frozendict = "^2.3.7"
 openai = {version = "^0.27.4", optional = true}
 pinecone-client = {version = "^2.2.1", optional = true}
 pydantic = ">=1.10.2"
@@ -36,16 +36,16 @@
 
 [tool.poetry.group.test.dependencies]
 aioresponses = "^0.7.4"
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.10.0"
 pytest-responses = "^0.5.1"
-responses = "^0.23.1"
 python-dotenv = "^1.0.0"
+responses = "^0.23.1"
 
 [tool.poetry.extras]
 all = [
   "openai",
   "pinecone-client",
 ]
 llms = ["openai"]
@@ -60,14 +60,16 @@
 [tool.ruff]
 exclude = [".venv"]
 # TODO: Figure out how to solve these by changing Mustache templates.
 ignore = [
   "F401",
   "E501",
   "F841",
+  "F821",
+  "F523",
 ]
 select = [
   "E", # pycodestyle
   "F", # pyflakes
   "I", # isort
 ]
```

### Comparing `gentrace_py-0.7.4/PKG-INFO` & `gentrace_py-0.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentrace-py
-Version: 0.7.4
+Version: 0.8.0
 Summary: Python SDK for the Gentrace API
 Home-page: https://github.com/gentrace/gentrace-python
 License: MIT
 Author: Gentrace
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

