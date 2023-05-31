# Comparing `tmp/fideslang-1.3.4.tar.gz` & `tmp/fideslang-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fideslang-1.3.4.tar", last modified: Tue Apr 18 13:29:41 2023, max compression
+gzip compressed data, was "fideslang-1.4.tar", last modified: Wed May 31 15:23:42 2023, max compression
```

## Comparing `fideslang-1.3.4.tar` & `fideslang-1.4.tar`

### file list

```diff
@@ -1,30 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:29:41.948316 fideslang-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-04-18 13:29:36.000000 fideslang-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-18 13:29:36.000000 fideslang-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-18 13:29:41.948316 fideslang-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-18 13:29:36.000000 fideslang-1.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-18 13:29:36.000000 fideslang-1.3.4/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-18 13:29:36.000000 fideslang-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-18 13:29:36.000000 fideslang-1.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-18 13:29:41.952316 fideslang-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-18 13:29:36.000000 fideslang-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:29:41.948316 fideslang-1.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:29:41.952316 fideslang-1.3.4/src/fideslang/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 13:29:41.952316 fideslang-1.3.4/src/fideslang/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/default_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    32851 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/default_taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/manifests.py
--rw-r--r--   0 runner    (1001) docker     (123)    35611 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:29:41.948316 fideslang-1.3.4/src/fideslang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-18 13:29:41.000000 fideslang-1.3.4/src/fideslang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-18 13:29:41.000000 fideslang-1.3.4/src/fideslang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:29:41.000000 fideslang-1.3.4/src/fideslang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-18 13:29:41.000000 fideslang-1.3.4/src/fideslang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 13:29:41.000000 fideslang-1.3.4/src/fideslang.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    57971 2023-04-18 13:29:36.000000 fideslang-1.3.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:23:42.411170 fideslang-1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-05-31 15:23:37.000000 fideslang-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-31 15:23:37.000000 fideslang-1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-31 15:23:42.411170 fideslang-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-31 15:23:37.000000 fideslang-1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-31 15:23:37.000000 fideslang-1.4/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-31 15:23:37.000000 fideslang-1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-31 15:23:37.000000 fideslang-1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-31 15:23:42.411170 fideslang-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-31 15:23:37.000000 fideslang-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:23:42.407170 fideslang-1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:23:42.411170 fideslang-1.4/src/fideslang/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-31 15:23:42.411170 fideslang-1.4/src/fideslang/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/default_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:23:42.411170 fideslang-1.4/src/fideslang/default_taxonomy/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/default_taxonomy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15437 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/default_taxonomy/data_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/default_taxonomy/data_qualifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/default_taxonomy/data_subjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/default_taxonomy/data_uses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/default_taxonomy/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/manifests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35055 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:23:42.407170 fideslang-1.4/src/fideslang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-31 15:23:42.000000 fideslang-1.4/src/fideslang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-31 15:23:42.000000 fideslang-1.4/src/fideslang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:23:42.000000 fideslang-1.4/src/fideslang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-31 15:23:42.000000 fideslang-1.4/src/fideslang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 15:23:42.000000 fideslang-1.4/src/fideslang.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    57971 2023-05-31 15:23:37.000000 fideslang-1.4/versioneer.py
```

### Comparing `fideslang-1.3.4/LICENSE` & `fideslang-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.4/PKG-INFO` & `fideslang-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fideslang
-Version: 1.3.4
+Version: 1.4
 Summary: Fides Taxonomy Language
 Home-page: https://github.com/ethyca/fideslang
 Author: Ethyca, Inc.
 Author-email: fidesteam@ethyca.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fideslang-1.3.4/README.md` & `fideslang-1.4/README.md`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.4/pyproject.toml` & `fideslang-1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.4/setup.cfg` & `fideslang-1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.4/setup.py` & `fideslang-1.4/setup.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.4/src/fideslang/__init__.py` & `fideslang-1.4/src/fideslang/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
 Exports various fideslang objects for easier use elsewhere.
 """
 
 from typing import Dict, Type, Union
 
-from .default_fixtures import COUNTRY_CODES
-from .default_taxonomy import DEFAULT_TAXONOMY
+from fideslang.default_fixtures import COUNTRY_CODES
+from fideslang.default_taxonomy import DEFAULT_TAXONOMY
 
 # Export the Models
 from .models import (
     DataCategory,
     DataFlow,
     DataQualifier,
     Dataset,
     DatasetField,
     DatasetFieldBase,
     DataSubject,
     DataUse,
     Evaluation,
+    FidesCollectionKey,
+    FidesDatasetReference,
     FidesMeta,
     FidesModel,
-    FidesDatasetReference,
-    FidesCollectionKey,
     Organization,
     Policy,
     PolicyRule,
     PrivacyDeclaration,
     PrivacyRule,
     Registry,
     System,
```

### Comparing `fideslang-1.3.4/src/fideslang/default_fixtures.py` & `fideslang-1.4/src/fideslang/default_fixtures.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.4/src/fideslang/manifests.py` & `fideslang-1.4/src/fideslang/manifests.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,23 @@
     Write a dict representation of a resource out to a file.
     """
     if isinstance(manifest, dict):
         manifest = {resource_type: [manifest]}
     else:
         manifest = {resource_type: manifest}
 
-    with open(file_name, "w") as manifest_file:
+    with open(file_name, "w", encoding="utf-8") as manifest_file:
         yaml.dump(manifest, manifest_file, sort_keys=False, indent=2)
 
 
 def load_yaml_into_dict(file_path: str) -> Dict:
     """
     This loads yaml files into a dictionary to be used in API calls.
     """
-    with open(file_path, "r") as yaml_file:
+    with open(file_path, "r", encoding="utf-8") as yaml_file:
         loaded = yaml.safe_load(yaml_file)
         if isinstance(loaded, dict):
             return loaded
 
     print(f"Failed to parse invalid manifest: {file_path.split('/')[-1]}. Skipping.")
     return {}
```

### Comparing `fideslang-1.3.4/src/fideslang/models.py` & `fideslang-1.4/src/fideslang/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 
 """
 Contains all of the Fides resources modeled as Pydantic models.
 """
 from __future__ import annotations
 
 from enum import Enum
-from typing import Any, Dict, List, Literal, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 from warnings import warn
 
 from pydantic import (
     AnyUrl,
     BaseModel,
     ConstrainedStr,
     Field,
     HttpUrl,
     PositiveInt,
     root_validator,
     validator,
 )
 
+# import `Literal` from typing_extensions to work around https://github.com/pydantic/pydantic/issues/5821
+from typing_extensions import Literal
+
 from fideslang.validation import (
     FidesKey,
     check_valid_country_code,
     matching_parent_key,
     no_self_reference,
     parse_data_type_string,
     sort_list_objects_by_name,
@@ -59,15 +62,15 @@
     fides_key: FidesKey = Field(
         description="A unique key used to identify this resource."
     )
     organization_fides_key: FidesKey = Field(
         default="default_organization",
         description="Defines the Organization that this resource belongs to.",
     )
-    tags: Optional[List[str]]
+    tags: Optional[List[str]] = None
     name: Optional[str] = name_field
     description: Optional[str] = description_field
 
     class Config:
         "Config for the FidesModel"
         extra = "ignore"
         orm_mode = True
@@ -213,29 +216,33 @@
     )
     is_default: bool = is_default_field
 
 
 class DataUse(FidesModel):
     """The DataUse resource model."""
 
-    parent_key: Optional[FidesKey]
+    parent_key: Optional[FidesKey] = None
     legal_basis: Optional[LegalBasisEnum] = Field(
+        default=None,
         description="The legal basis category of which the data use falls under. This field is used as part of the creation of an exportable data map.",
     )
     special_category: Optional[SpecialCategoriesEnum] = Field(
+        default=None,
         description="The special category for processing of which the data use falls under. This field is used as part of the creation of an exportable data map.",
     )
     recipients: Optional[List[str]] = Field(
+        default=None,
         description="An array of recipients when sharing personal data outside of your organization.",
     )
     legitimate_interest: bool = Field(
         default=False,
         description="A boolean representation of if the legal basis used is `Legitimate Interest`. Validated at run time and looks for a `legitimate_interest_impact_assessment` to exist if true.",
     )
     legitimate_interest_impact_assessment: Optional[AnyUrl] = Field(
+        default=None,
         description="A url pointing to the legitimate interest impact assessment. Required if the legal bases used is legitimate interest.",
     )
     is_default: bool = is_default_field
 
     _matching_parent_key: classmethod = matching_parent_key_validator
     _no_self_reference: classmethod = no_self_reference_validator
 
@@ -933,17 +940,14 @@
     )
     ingress: Optional[List[DataFlow]] = Field(
         description="The resources from which the System receives data."
     )
     privacy_declarations: List[PrivacyDeclaration] = Field(
         description=PrivacyDeclaration.__doc__,
     )
-    system_dependencies: Optional[List[FidesKey]] = Field(
-        description="A list of fides keys to model dependencies."
-    )
     joint_controller: Optional[ContactDetails] = Field(
         description=ContactDetails.__doc__,
     )
     third_country_transfers: Optional[List[str]] = Field(
         description="An optional array to identify any third countries where data is transited to. For consistency purposes, these fields are required to follow the Alpha-3 code set in ISO 3166-1.",
     )
     administrating_department: Optional[str] = Field(
@@ -955,18 +959,14 @@
         description=DataProtectionImpactAssessment.__doc__,
     )
 
     _sort_privacy_declarations: classmethod = validator(
         "privacy_declarations", allow_reuse=True
     )(sort_list_objects_by_name)
 
-    _no_self_reference: classmethod = validator(
-        "system_dependencies", allow_reuse=True, each_item=True
-    )(no_self_reference)
-
     _check_valid_country_code: classmethod = country_code_validator
 
     @validator("privacy_declarations", each_item=True)
     @classmethod
     def privacy_declarations_reference_data_flows(
         cls,
         value: PrivacyDeclaration,
@@ -989,29 +989,14 @@
                 for fides_key in fides_keys:
                     assert fides_key in [
                         data_flow.fides_key for data_flow in data_flows
                     ], f"PrivacyDeclaration '{value.name}' defines {direction} with '{fides_key}' and is applied to the System '{system}', which does not itself define {direction} with that resource."
 
         return value
 
-    @validator("system_dependencies")
-    @classmethod
-    def deprecate_system_dependencies(cls, value: List[FidesKey]) -> List[FidesKey]:
-        """
-        Warn that the `system_dependencies` field is deprecated, if set.
-        """
-
-        if value is not None:
-            warn(
-                "The system_dependencies field is deprecated, and will be removed in a future version of fideslang. Use the 'egress' and 'ingress` fields instead.",
-                DeprecationWarning,
-            )
-
-        return value
-
     class Config:
         """Class for the System config"""
 
         use_enum_values = True
 
 
 # Taxonomy
```

### Comparing `fideslang-1.3.4/src/fideslang/parse.py` & `fideslang-1.4/src/fideslang/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This module handles everything related to parsing resources into Pydantic models,
 either from local files or the server.
 """
-from typing import List, Dict
+from typing import Dict, List
 
-from fideslang import model_map, FidesModel, Taxonomy
+from fideslang import FidesModel, Taxonomy, model_map
 
 
 def parse_dict(
     resource_type: str, resource: Dict, from_server: bool = False
 ) -> FidesModel:
     """
     Parse an individual resource into its Python model.
```

### Comparing `fideslang-1.3.4/src/fideslang/relationships.py` & `fideslang-1.4/src/fideslang/relationships.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,15 @@
 by each other and building a dependency graph of relationships.
 """
 
 import inspect
 from functools import reduce
 from typing import List, Set
 
-
-from fideslang.models import (
-    FidesKey,
-    Taxonomy,
-    BaseModel,
-)
+from fideslang.models import BaseModel, FidesKey, Taxonomy
 from fideslang.utils import get_resource_by_fides_key
 
 
 def find_nested_keys_in_list(parameter_value: List[BaseModel]) -> List[str]:
     """
     Iterates a nested object list and returns any keys nested fides keys
     """
```

### Comparing `fideslang-1.3.4/src/fideslang/utils.py` & `fideslang-1.4/src/fideslang/utils.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.4/src/fideslang/validation.py` & `fideslang-1.4/src/fideslang/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 def no_self_reference(value: FidesKey, values: Dict) -> FidesKey:
     """
     Check to make sure that the fides_key doesn't match other fides_key
     references within an object.
 
     i.e. DataCategory.parent_key != DataCategory.fides_key
     """
-
     fides_key = FidesKey.validate(values.get("fides_key", ""))
     if value == fides_key:
         raise FidesValidationError("FidesKey can not self-reference!")
     return value
 
 
 def matching_parent_key(value: FidesKey, values: Dict) -> FidesKey:
```

### Comparing `fideslang-1.3.4/src/fideslang.egg-info/PKG-INFO` & `fideslang-1.4/src/fideslang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fideslang
-Version: 1.3.4
+Version: 1.4
 Summary: Fides Taxonomy Language
 Home-page: https://github.com/ethyca/fideslang
 Author: Ethyca, Inc.
 Author-email: fidesteam@ethyca.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fideslang-1.3.4/src/fideslang.egg-info/SOURCES.txt` & `fideslang-1.4/src/fideslang.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,20 +6,25 @@
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 src/fideslang/__init__.py
 src/fideslang/_version.py
 src/fideslang/default_fixtures.py
-src/fideslang/default_taxonomy.py
 src/fideslang/manifests.py
 src/fideslang/models.py
 src/fideslang/parse.py
 src/fideslang/py.typed
 src/fideslang/relationships.py
 src/fideslang/utils.py
 src/fideslang/validation.py
 src/fideslang.egg-info/PKG-INFO
 src/fideslang.egg-info/SOURCES.txt
 src/fideslang.egg-info/dependency_links.txt
 src/fideslang.egg-info/requires.txt
-src/fideslang.egg-info/top_level.txt
+src/fideslang.egg-info/top_level.txt
+src/fideslang/default_taxonomy/__init__.py
+src/fideslang/default_taxonomy/data_categories.py
+src/fideslang/default_taxonomy/data_qualifiers.py
+src/fideslang/default_taxonomy/data_subjects.py
+src/fideslang/default_taxonomy/data_uses.py
+src/fideslang/default_taxonomy/organizations.py
```

### Comparing `fideslang-1.3.4/versioneer.py` & `fideslang-1.4/versioneer.py`

 * *Files identical despite different names*

