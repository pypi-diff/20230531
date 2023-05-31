# Comparing `tmp/encord-0.1.78.tar.gz` & `tmp/encord-0.1.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord-0.1.78.tar", max compression
+gzip compressed data, was "encord-0.1.79.tar", max compression
```

## Comparing `encord-0.1.78.tar` & `encord-0.1.79.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0    11330 2023-05-30 13:19:21.437542 encord-0.1.78/LICENSE
--rw-r--r--   0        0        0     2037 2023-05-30 13:19:21.437542 encord-0.1.78/README.md
--rw-r--r--   0        0        0       84 2023-05-30 13:19:21.437542 encord-0.1.78/cord/__init__.py
--rw-r--r--   0        0        0      158 2023-05-30 13:19:21.453542 encord-0.1.78/encord/__init__.py
--rw-r--r--   0        0        0      214 2023-05-30 13:19:21.453542 encord-0.1.78/encord/_version.py
--rw-r--r--   0        0        0    49096 2023-05-30 13:19:21.453542 encord-0.1.78/encord/client.py
--rw-r--r--   0        0        0    10843 2023-05-30 13:19:21.453542 encord-0.1.78/encord/configs.py
--rw-r--r--   0        0        0        0 2023-05-30 13:19:21.453542 encord-0.1.78/encord/constants/__init__.py
--rw-r--r--   0        0        0      810 2023-05-30 13:19:21.453542 encord-0.1.78/encord/constants/enums.py
--rw-r--r--   0        0        0     3293 2023-05-30 13:19:21.453542 encord-0.1.78/encord/constants/model.py
--rw-r--r--   0        0        0     6068 2023-05-30 13:19:21.453542 encord-0.1.78/encord/constants/model_weights.py
--rw-r--r--   0        0        0     1119 2023-05-30 13:19:21.453542 encord-0.1.78/encord/constants/string_constants.py
--rw-r--r--   0        0        0        0 2023-05-30 13:19:21.453542 encord-0.1.78/encord/constants/test/__init__.py
--rw-r--r--   0        0        0      634 2023-05-30 13:19:21.453542 encord-0.1.78/encord/constants/test/test_enums.py
--rw-r--r--   0        0        0    16035 2023-05-30 13:19:21.453542 encord-0.1.78/encord/dataset.py
--rw-r--r--   0        0        0     6351 2023-05-30 13:19:21.453542 encord-0.1.78/encord/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-30 13:19:21.453542 encord-0.1.78/encord/http/__init__.py
--rw-r--r--   0        0        0     5315 2023-05-30 13:19:21.453542 encord-0.1.78/encord/http/bundle.py
--rw-r--r--   0        0        0      535 2023-05-30 13:19:21.453542 encord-0.1.78/encord/http/constants.py
--rw-r--r--   0        0        0     7234 2023-05-30 13:19:21.453542 encord-0.1.78/encord/http/error_utils.py
--rw-r--r--   0        0        0      103 2023-05-30 13:19:21.453542 encord-0.1.78/encord/http/limits.py
--rw-r--r--   0        0        0     7916 2023-05-30 13:19:21.453542 encord-0.1.78/encord/http/querier.py
--rw-r--r--   0        0        0      697 2023-05-30 13:19:21.453542 encord-0.1.78/encord/http/query_methods.py
--rw-r--r--   0        0        0     1719 2023-05-30 13:19:21.453542 encord-0.1.78/encord/http/request.py
--rw-r--r--   0        0        0     6182 2023-05-30 13:19:21.453542 encord-0.1.78/encord/http/utils.py
--rw-r--r--   0        0        0      340 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/__init__.py
--rw-r--r--   0        0        0      182 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/classification.py
--rw-r--r--   0        0        0    29750 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/common.py
--rw-r--r--   0        0        0      149 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/constants.py
--rw-r--r--   0        0        0     5631 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/coordinates.py
--rw-r--r--   0        0        0     3419 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/frames.py
--rw-r--r--   0        0        0    21407 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/internal_helpers.py
--rw-r--r--   0        0        0   140605 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/ontology_labels_impl.py
--rw-r--r--   0        0        0      174 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/ontology_object.py
--rw-r--r--   0        0        0      185 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/ontology_structure.py
--rw-r--r--   0        0        0      549 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/project.py
--rw-r--r--   0        0        0     1240 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/utils.py
--rw-r--r--   0        0        0     3430 2023-05-30 13:19:21.453542 encord-0.1.78/encord/ontology.py
--rw-r--r--   0        0        0        0 2023-05-30 13:19:21.453542 encord-0.1.78/encord/orm/__init__.py
--rw-r--r--   0        0        0      982 2023-05-30 13:19:21.453542 encord-0.1.78/encord/orm/api_key.py
--rw-r--r--   0        0        0     5335 2023-05-30 13:19:21.453542 encord-0.1.78/encord/orm/base_orm.py
--rw-r--r--   0        0        0      111 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/cloud_integration.py
--rw-r--r--   0        0        0    32204 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/dataset.py
--rw-r--r--   0        0        0      828 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/dataset_with_user_role.py
--rw-r--r--   0        0        0      175 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/formatter.py
--rw-r--r--   0        0        0     1146 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/label_log.py
--rw-r--r--   0        0        0    11869 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/label_row.py
--rw-r--r--   0        0        0     1577 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/labeling_algorithm.py
--rw-r--r--   0        0        0     6687 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/model.py
--rw-r--r--   0        0        0      823 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/ontology.py
--rw-r--r--   0        0        0     8885 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/project.py
--rw-r--r--   0        0        0      625 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/project_api_key.py
--rw-r--r--   0        0        0      828 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/project_with_user_role.py
--rw-r--r--   0        0        0        0 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/test/__init__.py
--rw-r--r--   0        0        0      570 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/test/test_dataset.py
--rw-r--r--   0        0        0    39203 2023-05-30 13:19:21.457542 encord-0.1.78/encord/project.py
--rw-r--r--   0        0        0        0 2023-05-30 13:19:21.457542 encord-0.1.78/encord/project_ontology/__init__.py
--rw-r--r--   0        0        0     1316 2023-05-30 13:19:21.457542 encord-0.1.78/encord/project_ontology/classification_attribute.py
--rw-r--r--   0        0        0      525 2023-05-30 13:19:21.457542 encord-0.1.78/encord/project_ontology/classification_option.py
--rw-r--r--   0        0        0      357 2023-05-30 13:19:21.457542 encord-0.1.78/encord/project_ontology/classification_type.py
--rw-r--r--   0        0        0      237 2023-05-30 13:19:21.457542 encord-0.1.78/encord/project_ontology/object_type.py
--rw-r--r--   0        0        0     9676 2023-05-30 13:19:21.457542 encord-0.1.78/encord/project_ontology/ontology.py
--rw-r--r--   0        0        0      630 2023-05-30 13:19:21.457542 encord-0.1.78/encord/project_ontology/ontology_classification.py
--rw-r--r--   0        0        0      683 2023-05-30 13:19:21.457542 encord-0.1.78/encord/project_ontology/ontology_object.py
--rw-r--r--   0        0        0    27854 2023-05-30 13:19:21.457542 encord-0.1.78/encord/user_client.py
--rw-r--r--   0        0        0        0 2023-05-30 13:19:21.457542 encord-0.1.78/encord/utilities/__init__.py
--rw-r--r--   0        0        0     4282 2023-05-30 13:19:21.457542 encord-0.1.78/encord/utilities/client_utilities.py
--rw-r--r--   0        0        0      253 2023-05-30 13:19:21.457542 encord-0.1.78/encord/utilities/common.py
--rw-r--r--   0        0        0     3270 2023-05-30 13:19:21.457542 encord-0.1.78/encord/utilities/label_utilities.py
--rw-r--r--   0        0        0      343 2023-05-30 13:19:21.457542 encord-0.1.78/encord/utilities/ontology_user.py
--rw-r--r--   0        0        0      578 2023-05-30 13:19:21.457542 encord-0.1.78/encord/utilities/project_user.py
--rw-r--r--   0        0        0      467 2023-05-30 13:19:21.457542 encord-0.1.78/encord/utilities/project_utilities.py
--rw-r--r--   0        0        0     1944 2023-05-30 13:19:21.457542 encord-0.1.78/pyproject.toml
--rw-r--r--   0        0        0     3220 1970-01-01 00:00:00.000000 encord-0.1.78/PKG-INFO
+-rw-r--r--   0        0        0    11330 2023-05-31 16:24:21.757835 encord-0.1.79/LICENSE
+-rw-r--r--   0        0        0     2037 2023-05-31 16:24:21.757835 encord-0.1.79/README.md
+-rw-r--r--   0        0        0       84 2023-05-31 16:24:21.757835 encord-0.1.79/cord/__init__.py
+-rw-r--r--   0        0        0      158 2023-05-31 16:24:21.777835 encord-0.1.79/encord/__init__.py
+-rw-r--r--   0        0        0      214 2023-05-31 16:24:21.777835 encord-0.1.79/encord/_version.py
+-rw-r--r--   0        0        0    49096 2023-05-31 16:24:21.777835 encord-0.1.79/encord/client.py
+-rw-r--r--   0        0        0    10843 2023-05-31 16:24:21.777835 encord-0.1.79/encord/configs.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:24:21.777835 encord-0.1.79/encord/constants/__init__.py
+-rw-r--r--   0        0        0      810 2023-05-31 16:24:21.777835 encord-0.1.79/encord/constants/enums.py
+-rw-r--r--   0        0        0     3293 2023-05-31 16:24:21.777835 encord-0.1.79/encord/constants/model.py
+-rw-r--r--   0        0        0     6068 2023-05-31 16:24:21.777835 encord-0.1.79/encord/constants/model_weights.py
+-rw-r--r--   0        0        0     1119 2023-05-31 16:24:21.777835 encord-0.1.79/encord/constants/string_constants.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:24:21.777835 encord-0.1.79/encord/constants/test/__init__.py
+-rw-r--r--   0        0        0      634 2023-05-31 16:24:21.777835 encord-0.1.79/encord/constants/test/test_enums.py
+-rw-r--r--   0        0        0    16035 2023-05-31 16:24:21.777835 encord-0.1.79/encord/dataset.py
+-rw-r--r--   0        0        0     6351 2023-05-31 16:24:21.777835 encord-0.1.79/encord/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:24:21.777835 encord-0.1.79/encord/http/__init__.py
+-rw-r--r--   0        0        0     5315 2023-05-31 16:24:21.777835 encord-0.1.79/encord/http/bundle.py
+-rw-r--r--   0        0        0      535 2023-05-31 16:24:21.777835 encord-0.1.79/encord/http/constants.py
+-rw-r--r--   0        0        0     7234 2023-05-31 16:24:21.777835 encord-0.1.79/encord/http/error_utils.py
+-rw-r--r--   0        0        0      103 2023-05-31 16:24:21.777835 encord-0.1.79/encord/http/limits.py
+-rw-r--r--   0        0        0     7928 2023-05-31 16:24:21.777835 encord-0.1.79/encord/http/querier.py
+-rw-r--r--   0        0        0      697 2023-05-31 16:24:21.777835 encord-0.1.79/encord/http/query_methods.py
+-rw-r--r--   0        0        0     1719 2023-05-31 16:24:21.777835 encord-0.1.79/encord/http/request.py
+-rw-r--r--   0        0        0     6182 2023-05-31 16:24:21.777835 encord-0.1.79/encord/http/utils.py
+-rw-r--r--   0        0        0      340 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/classification.py
+-rw-r--r--   0        0        0    30906 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/common.py
+-rw-r--r--   0        0        0      149 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/constants.py
+-rw-r--r--   0        0        0     5631 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/coordinates.py
+-rw-r--r--   0        0        0     3419 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/frames.py
+-rw-r--r--   0        0        0    21407 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/internal_helpers.py
+-rw-r--r--   0        0        0   140605 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/ontology_labels_impl.py
+-rw-r--r--   0        0        0      174 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/ontology_object.py
+-rw-r--r--   0        0        0      185 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/ontology_structure.py
+-rw-r--r--   0        0        0      549 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/project.py
+-rw-r--r--   0        0        0     1240 2023-05-31 16:24:21.777835 encord-0.1.79/encord/objects/utils.py
+-rw-r--r--   0        0        0     3430 2023-05-31 16:24:21.777835 encord-0.1.79/encord/ontology.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/__init__.py
+-rw-r--r--   0        0        0      982 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/api_key.py
+-rw-r--r--   0        0        0     5335 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/base_orm.py
+-rw-r--r--   0        0        0      111 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/cloud_integration.py
+-rw-r--r--   0        0        0    32204 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/dataset.py
+-rw-r--r--   0        0        0      828 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/dataset_with_user_role.py
+-rw-r--r--   0        0        0      175 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/formatter.py
+-rw-r--r--   0        0        0     1146 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/label_log.py
+-rw-r--r--   0        0        0    11869 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/label_row.py
+-rw-r--r--   0        0        0     1577 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/labeling_algorithm.py
+-rw-r--r--   0        0        0     6687 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/model.py
+-rw-r--r--   0        0        0      823 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/ontology.py
+-rw-r--r--   0        0        0     8885 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/project.py
+-rw-r--r--   0        0        0      625 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/project_api_key.py
+-rw-r--r--   0        0        0      828 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/project_with_user_role.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/test/__init__.py
+-rw-r--r--   0        0        0      570 2023-05-31 16:24:21.777835 encord-0.1.79/encord/orm/test/test_dataset.py
+-rw-r--r--   0        0        0    39203 2023-05-31 16:24:21.777835 encord-0.1.79/encord/project.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:24:21.777835 encord-0.1.79/encord/project_ontology/__init__.py
+-rw-r--r--   0        0        0     1316 2023-05-31 16:24:21.777835 encord-0.1.79/encord/project_ontology/classification_attribute.py
+-rw-r--r--   0        0        0      525 2023-05-31 16:24:21.777835 encord-0.1.79/encord/project_ontology/classification_option.py
+-rw-r--r--   0        0        0      357 2023-05-31 16:24:21.777835 encord-0.1.79/encord/project_ontology/classification_type.py
+-rw-r--r--   0        0        0      237 2023-05-31 16:24:21.777835 encord-0.1.79/encord/project_ontology/object_type.py
+-rw-r--r--   0        0        0     9676 2023-05-31 16:24:21.777835 encord-0.1.79/encord/project_ontology/ontology.py
+-rw-r--r--   0        0        0      630 2023-05-31 16:24:21.777835 encord-0.1.79/encord/project_ontology/ontology_classification.py
+-rw-r--r--   0        0        0      683 2023-05-31 16:24:21.777835 encord-0.1.79/encord/project_ontology/ontology_object.py
+-rw-r--r--   0        0        0    28739 2023-05-31 16:24:21.777835 encord-0.1.79/encord/user_client.py
+-rw-r--r--   0        0        0        0 2023-05-31 16:24:21.777835 encord-0.1.79/encord/utilities/__init__.py
+-rw-r--r--   0        0        0     4282 2023-05-31 16:24:21.777835 encord-0.1.79/encord/utilities/client_utilities.py
+-rw-r--r--   0        0        0      253 2023-05-31 16:24:21.777835 encord-0.1.79/encord/utilities/common.py
+-rw-r--r--   0        0        0     3270 2023-05-31 16:24:21.781835 encord-0.1.79/encord/utilities/label_utilities.py
+-rw-r--r--   0        0        0      343 2023-05-31 16:24:21.781835 encord-0.1.79/encord/utilities/ontology_user.py
+-rw-r--r--   0        0        0      578 2023-05-31 16:24:21.781835 encord-0.1.79/encord/utilities/project_user.py
+-rw-r--r--   0        0        0      467 2023-05-31 16:24:21.781835 encord-0.1.79/encord/utilities/project_utilities.py
+-rw-r--r--   0        0        0     1944 2023-05-31 16:24:21.781835 encord-0.1.79/pyproject.toml
+-rw-r--r--   0        0        0     3220 1970-01-01 00:00:00.000000 encord-0.1.79/PKG-INFO
```

### Comparing `encord-0.1.78/LICENSE` & `encord-0.1.79/LICENSE`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/README.md` & `encord-0.1.79/README.md`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/client.py` & `encord-0.1.79/encord/client.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/configs.py` & `encord-0.1.79/encord/configs.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/constants/enums.py` & `encord-0.1.79/encord/constants/enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/constants/model.py` & `encord-0.1.79/encord/constants/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/constants/model_weights.py` & `encord-0.1.79/encord/constants/model_weights.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/constants/string_constants.py` & `encord-0.1.79/encord/constants/string_constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/constants/test/test_enums.py` & `encord-0.1.79/encord/constants/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/dataset.py` & `encord-0.1.79/encord/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/exceptions.py` & `encord-0.1.79/encord/exceptions.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/http/bundle.py` & `encord-0.1.79/encord/http/bundle.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/http/constants.py` & `encord-0.1.79/encord/http/constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/http/error_utils.py` & `encord-0.1.79/encord/http/error_utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/http/querier.py` & `encord-0.1.79/encord/http/querier.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             uid,
             self._config.write_timeout,
             payload=payload,
         )
 
         res, context = self._execute(request)
 
-        if res:
+        if res is not None:
             return res
         else:
             raise RequestException(f"Setting {db_object_type} with uid {uid} failed.", context=context)
 
     def basic_put(self, db_object_type, uid, payload, enable_logging=True):
         """Single DB object put request."""
         request = self._request(
```

### Comparing `encord-0.1.78/encord/http/query_methods.py` & `encord-0.1.79/encord/http/query_methods.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/http/request.py` & `encord-0.1.79/encord/http/request.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/http/utils.py` & `encord-0.1.79/encord/http/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/objects/common.py` & `encord-0.1.79/encord/objects/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -799,7 +799,52 @@
     Type[ChecklistAttribute],
     Type[TextAttribute],
     Type[Attribute],
 ]
 AttributeClasses = Union[RadioAttribute, ChecklistAttribute, TextAttribute, Attribute]
 OptionTypes = Union[Type[FlatOption], Type[NestableOption], Type[Option]]
 OptionClasses = Union[FlatOption, NestableOption, Option]
+
+
+class DeidentifyRedactTextMode(Enum):
+    REDACT_ALL_TEXT = "REDACT_ALL_TEXT"
+    REDACT_NO_TEXT = "REDACT_NO_TEXT"
+    REDACT_SENSITIVE_TEXT = "REDACT_SENSITIVE_TEXT"
+
+
+class SaveDeidentifiedDicomConditionType(Enum):
+    NOT_SUBSTR = "NOT_SUBSTR"
+    IN = "IN"
+
+
+@dataclass
+class SaveDeidentifiedDicomConditionIn:
+    value: List[str]
+    dicom_tag: str
+    condition_type: SaveDeidentifiedDicomConditionType = SaveDeidentifiedDicomConditionType.IN
+
+    def to_dict(self) -> dict:
+        return {
+            "value": self.value,
+            "dicom_tag": self.dicom_tag,
+            "condition_type": self.condition_type.value,
+        }
+
+
+@dataclass
+class SaveDeidentifiedDicomConditionNotSubstr:
+    value: str
+    dicom_tag: str
+    condition_type: SaveDeidentifiedDicomConditionType = SaveDeidentifiedDicomConditionType.NOT_SUBSTR
+
+    def to_dict(self) -> dict:
+        return {
+            "value": self.value,
+            "dicom_tag": self.dicom_tag,
+            "condition_type": self.condition_type.value,
+        }
+
+
+SaveDeidentifiedDicomCondition = Union[
+    SaveDeidentifiedDicomConditionNotSubstr,
+    SaveDeidentifiedDicomConditionIn,
+]
```

### Comparing `encord-0.1.78/encord/objects/coordinates.py` & `encord-0.1.79/encord/objects/coordinates.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/objects/frames.py` & `encord-0.1.79/encord/objects/frames.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/objects/internal_helpers.py` & `encord-0.1.79/encord/objects/internal_helpers.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/objects/ontology_labels_impl.py` & `encord-0.1.79/encord/objects/ontology_labels_impl.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/objects/project.py` & `encord-0.1.79/encord/objects/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/objects/utils.py` & `encord-0.1.79/encord/objects/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/ontology.py` & `encord-0.1.79/encord/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/orm/api_key.py` & `encord-0.1.79/encord/orm/api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/orm/base_orm.py` & `encord-0.1.79/encord/orm/base_orm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/orm/dataset.py` & `encord-0.1.79/encord/orm/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/orm/dataset_with_user_role.py` & `encord-0.1.79/encord/orm/dataset_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/orm/label_log.py` & `encord-0.1.79/encord/orm/label_log.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/orm/label_row.py` & `encord-0.1.79/encord/orm/label_row.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/orm/labeling_algorithm.py` & `encord-0.1.79/encord/orm/labeling_algorithm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/orm/model.py` & `encord-0.1.79/encord/orm/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/orm/ontology.py` & `encord-0.1.79/encord/orm/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/orm/project.py` & `encord-0.1.79/encord/orm/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/orm/project_api_key.py` & `encord-0.1.79/encord/orm/project_api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/orm/project_with_user_role.py` & `encord-0.1.79/encord/orm/project_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/orm/test/test_dataset.py` & `encord-0.1.79/encord/orm/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/project.py` & `encord-0.1.79/encord/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/project_ontology/classification_attribute.py` & `encord-0.1.79/encord/project_ontology/classification_attribute.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/project_ontology/classification_option.py` & `encord-0.1.79/encord/project_ontology/classification_option.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/project_ontology/ontology.py` & `encord-0.1.79/encord/project_ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/project_ontology/ontology_classification.py` & `encord-0.1.79/encord/project_ontology/ontology_classification.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/project_ontology/ontology_object.py` & `encord-0.1.79/encord/project_ontology/ontology_object.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/user_client.py` & `encord-0.1.79/encord/user_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 from encord.http.constants import DEFAULT_REQUESTS_SETTINGS, RequestsSettings
 from encord.http.querier import Querier
 from encord.http.utils import (
     CloudUploadSettings,
     upload_images_to_encord,
     upload_to_signed_url_list,
 )
+from encord.objects.common import (
+    DeidentifyRedactTextMode,
+    SaveDeidentifiedDicomCondition,
+)
 from encord.objects.ontology_labels_impl import Ontology as OrmOntology
 from encord.objects.ontology_labels_impl import OntologyStructure
 from encord.ontology import Ontology
 from encord.orm.cloud_integration import CloudIntegration
 from encord.orm.dataset import DEFAULT_DATASET_ACCESS_SETTINGS, CreateDatasetResponse
 from encord.orm.dataset import Dataset as OrmDataset
 from encord.orm.dataset import (
@@ -616,14 +620,17 @@
 
         return ret
 
     def deidentify_dicom_files(
         self,
         dicom_urls: List[str],
         integration_hash: str,
+        redact_dicom_tags: bool = True,
+        redact_pixels_mode: DeidentifyRedactTextMode = DeidentifyRedactTextMode.REDACT_NO_TEXT,
+        save_conditions: Optional[List[SaveDeidentifiedDicomCondition]] = None,
     ) -> List[str]:
         """
         Deidentify DICOM files in external storage.
         Given links to DICOM files pointing to AWS, GCP, AZURE or OTC, for example:
         [ "https://s3.region-code.amazonaws.com/bucket-name/dicom-file-input.dcm" ]
         Function executes deidentification on those files, it removes all
         DICOM tags (https://dicom.nema.org/medical/Dicom/2017e/output/chtml/part06/chapter_6.html)
@@ -644,28 +651,37 @@
 
         Args:
             self: Encord client object.
             dicom_urls: a list of urls to DICOM files, e.g.
                 `[ "https://s3.region-code.amazonaws.com/bucket-name/dicom-file-input.dcm" ]`
             integration_hash:
                 integration_hash parameter of Encord platform external storage integration
+            redact_dicom_tags:
+                Specifies if DICOM tags redaction should be enabled.
+            redact_pixels_mode:
+                Specifies which text redaction policy should be applied to pixel data.
+            save_conditions:
+                Specifies a list of conditions which all have to be true for DICOM deidentified file to be saved.
         Returns:
             Function returns list of links pointing to deidentified DICOM files,
             those will be saved to the same bucket and the same directory
             as original files with prefix ( deid_{timestamp}_ ).
             Example output:
             `[ "https://s3.region-code.amazonaws.com/bucket-name/deid_167294769118005312_dicom-file-input.dcm" ]`
 
         """
 
         return self.querier.basic_setter(
             DicomDeidentifyTask,
             uid=integration_hash,
             payload={
                 "dicom_urls": dicom_urls,
+                "redact_dicom_tags": redact_dicom_tags,
+                "redact_pixels_mode": redact_pixels_mode.value,
+                "save_conditions": [x.to_dict() for x in (save_conditions or [])],
             },
         )
 
 
 class ListingFilter(Enum):
     """
     Available properties_filter keys for get_projects() and get_datasets().
```

### Comparing `encord-0.1.78/encord/utilities/client_utilities.py` & `encord-0.1.79/encord/utilities/client_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/utilities/label_utilities.py` & `encord-0.1.79/encord/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/encord/utilities/project_user.py` & `encord-0.1.79/encord/utilities/project_user.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.78/pyproject.toml` & `encord-0.1.79/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encord"
-version = "0.1.78"
+version = "0.1.79"
 description = "Encord Python SDK Client"
 authors = ["Cord Technologies Limited <hello@encord.com>"]
 license = "Apache Software License"
 keywords = ["cord", "encord"]
 packages = [
     { include = "cord"},
     { include = "encord"},
```

### Comparing `encord-0.1.78/PKG-INFO` & `encord-0.1.79/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encord
-Version: 0.1.78
+Version: 0.1.79
 Summary: Encord Python SDK Client
 Home-page: https://github.com/encord-team/encord-client-python
 License: Apache Software License
 Keywords: cord,encord
 Author: Cord Technologies Limited
 Author-email: hello@encord.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: encord Version: 0.1.78 Summary: Encord Python SDK
+Metadata-Version: 2.1 Name: encord Version: 0.1.79 Summary: Encord Python SDK
 Client Home-page: https://github.com/encord-team/encord-client-python License:
 Apache Software License Keywords: cord,encord Author: Cord Technologies Limited
 Author-email: hello@encord.com Requires-Python: >=3.7,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

