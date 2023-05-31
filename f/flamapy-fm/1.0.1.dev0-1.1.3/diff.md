# Comparing `tmp/flamapy-fm-1.0.1.dev0.tar.gz` & `tmp/flamapy-fm-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamapy-fm-1.0.1.dev0.tar", last modified: Sat Aug 13 17:00:04 2022, max compression
+gzip compressed data, was "flamapy-fm-1.1.3.tar", last modified: Wed May 31 20:58:26 2023, max compression
```

## Comparing `flamapy-fm-1.0.1.dev0.tar` & `flamapy-fm-1.1.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:04.377230 flamapy-fm-1.0.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-08-13 17:00:04.377230 flamapy-fm-1.0.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:04.373229 flamapy-fm-1.0.1.dev0/flamapy/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:04.373229 flamapy-fm-1.0.1.dev0/flamapy/metamodels/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:04.373229 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:04.373229 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/models/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13273 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/models/feature_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:04.373229 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/
--rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1317 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/fm_atomic_sets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/fm_average_branching_factor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2587 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/fm_core_features.py
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/fm_count_leafs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1760 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/fm_estimated_products_number.py
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/fm_feature_ancestors.py
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/fm_leaf_features.py
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/fm_max_depth_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:04.373229 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8469 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/afm_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     4220 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/afm_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/attributes_csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     5974 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/featureide_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     5533 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/glencoe_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3525 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/glencoe_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/json_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2633 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/splot_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)    13821 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/uvl_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3549 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/uvl_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4742 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/xml_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-13 17:00:04.377230 flamapy-fm-1.0.1.dev0/flamapy_fm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-08-13 17:00:04.000000 flamapy-fm-1.0.1.dev0/flamapy_fm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1692 2022-08-13 17:00:04.000000 flamapy-fm-1.0.1.dev0/flamapy_fm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-08-13 17:00:04.000000 flamapy-fm-1.0.1.dev0/flamapy_fm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-13 17:00:04.000000 flamapy-fm-1.0.1.dev0/flamapy_fm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-13 17:00:04.000000 flamapy-fm-1.0.1.dev0/flamapy_fm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-13 17:00:04.377230 flamapy-fm-1.0.1.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-08-13 16:59:52.000000 flamapy-fm-1.0.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:58:26.989568 flamapy-fm-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-31 20:58:26.989568 flamapy-fm-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:58:26.985568 flamapy-fm-1.1.3/flamapy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:58:26.985568 flamapy-fm-1.1.3/flamapy/metamodels/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:58:26.985568 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:58:26.985568 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13335 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/models/feature_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:58:26.985568 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/fm_atomic_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/fm_average_branching_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/fm_core_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/fm_count_leafs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/fm_estimated_products_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/fm_feature_ancestors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/fm_leaf_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/fm_max_depth_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:58:26.989568 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/afm_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/afm_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/attributes_csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/featureide_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/glencoe_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/glencoe_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/json_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/splot_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/uvl_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/uvl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/xml_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:58:26.989568 flamapy-fm-1.1.3/flamapy_fm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-31 20:58:26.000000 flamapy-fm-1.1.3/flamapy_fm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-31 20:58:26.000000 flamapy-fm-1.1.3/flamapy_fm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 20:58:26.000000 flamapy-fm-1.1.3/flamapy_fm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-31 20:58:26.000000 flamapy-fm-1.1.3/flamapy_fm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 20:58:26.000000 flamapy-fm-1.1.3/flamapy_fm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 20:58:26.989568 flamapy-fm-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-31 20:58:10.000000 flamapy-fm-1.1.3/setup.py
```

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/models/feature_model.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/models/feature_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,24 +55,26 @@
     def __str__(self) -> str:
         parent_name = self.parent.name if self.parent else ''
         res = f'{parent_name}[{self.card_min},{self.card_max}]'
         for _child in self.children:
             res += _child.name + ' '
         if self.is_alternative():
             relation_type = 'alternative'
-        if self.is_or():
+        elif self.is_or():
             relation_type = 'or'
-        if self.is_mandatory():
+        elif self.is_mandatory():
             relation_type = 'mandatory'
-        if self.is_optional():
+        elif self.is_optional():
             relation_type = 'optional'
-        if self.is_mutex():
+        elif self.is_mutex():
             relation_type = 'mutex'
-        if self.is_cardinal():
+        elif self.is_cardinal():
             relation_type = 'cardinality'
+        else: 
+            relation_type = 'Other'
         res = f'({relation_type}) ' + res
         return res
 
     def __hash__(self) -> int:
         return hash((self.parent, frozenset(self.children), self.card_min, self.card_max))
 
     def __eq__(self, other: Any) -> bool:
@@ -190,16 +192,16 @@
     def ast(self) -> AST:
         return self._ast
 
     @ast.setter
     def ast(self, ast: AST) -> None:
         self._ast = ast
 
-    def get_features(self) -> list['Feature']:
-        """List of features involved in the constraint."""
+    def get_features(self) -> list[str]:
+        """List of features' names involved in the constraint."""
         features = set()
         stack = [self.ast.root]
         while stack:
             node = stack.pop()
             if node.is_unique_term():
                 features.add(node.data)
             elif node.is_unary_op():
```

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/__init__.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/fm_atomic_sets.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/fm_atomic_sets.py`

 * *Files identical despite different names*

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/fm_average_branching_factor.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/fm_average_branching_factor.py`

 * *Files identical despite different names*

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/fm_core_features.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/fm_core_features.py`

 * *Files identical despite different names*

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/fm_count_leafs.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/fm_count_leafs.py`

 * *Files identical despite different names*

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/fm_estimated_products_number.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/fm_estimated_products_number.py`

 * *Files identical despite different names*

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/fm_feature_ancestors.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/fm_feature_ancestors.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,20 @@
 
 class FMFeatureAncestors(Operation):
     """
     This operation returns the list of ancestors of a given feature
     (i.e., all parents recursively up to the root feature).
     """
 
-    def __init__(self, feature: Feature):
+    def __init__(self):
         self.result = []  # type: list[Feature]
-        self.feature = feature
+        self.feature = None  # type: Feature
+
+    def set_feature(self, feature: Feature) -> None:
+        self.feature = feature  
 
     def get_result(self) -> list[Feature]:
         return self.result
 
     def execute(self, model: FeatureModel) -> 'FMFeatureAncestors':
         self.result = get_feature_ancestors(self.feature)
         return self
```

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/fm_leaf_features.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/fm_leaf_features.py`

 * *Files identical despite different names*

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/operations/fm_max_depth_tree.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/operations/fm_max_depth_tree.py`

 * *Files identical despite different names*

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/__init__.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/afm_reader.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/afm_reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 
 from typing import Optional
 
 from afmparser import AFMParser
 from afmparser import get_tree
 
+from flamapy.core.exceptions import FlamaException
 from flamapy.core.transformations import TextToModel
 from flamapy.core.models.ast import AST, Node, ASTOperation
 from flamapy.metamodels.fm_metamodel.models import (
     Constraint,
     Domain,
     Feature,
     FeatureModel,
@@ -95,16 +96,17 @@
                 children.append(feature)
 
             relation = Relation(parent_feature, children, card_min, card_max)
             parent_feature.add_relation(relation)
 
     def set_attributes(self) -> None:
         attributes_block = self.parse_tree.attributes_block()
-        for attribute_spec in attributes_block.attribute_spec():
-            self.read_attribute(attribute_spec)
+        if attributes_block is not None:
+            for attribute_spec in attributes_block.attribute_spec():
+                self.read_attribute(attribute_spec)
 
     def read_attribute(self, attribute_spec: AFMParser.Attribute_specContext) -> None:
         attribute_name_node = attribute_spec.attribute_name()
         attribute_name = attribute_name_node.LOWERCASE().getText()
 
         if self.model is None:
             raise TypeError('self.model is None, expected FeatureModel type')
@@ -134,27 +136,27 @@
         attribute = Attribute(attribute_name, domain,
                               default_value, null_value)
         attribute.set_parent(attribute_feature)
         attribute_feature.add_attribute(attribute)
 
     def set_constraints(self) -> None:
         constraints_block = self.parse_tree.constraints_block()
+        if constraints_block is not None:
+            for constraint_spec in constraints_block.constraint_spec():
 
-        for constraint_spec in constraints_block.constraint_spec():
-
-            simple_spec = constraint_spec.simple_spec()
-            if simple_spec is not None:
-                prefix = ""
-                self.read_expression(simple_spec.expression(), prefix)
-
-            brackets_spec = constraint_spec.brackets_spec()
-            if brackets_spec is not None:
-                prefix = brackets_spec.WORD().getText() + "."
-                for spec in brackets_spec.simple_spec():
-                    self.read_expression(spec.expression(), prefix)
+                simple_spec = constraint_spec.simple_spec()
+                if simple_spec is not None:
+                    prefix = ""
+                    self.read_expression(simple_spec.expression(), prefix)
+
+                brackets_spec = constraint_spec.brackets_spec()
+                if brackets_spec is not None:
+                    prefix = brackets_spec.WORD().getText() + "."
+                    for spec in brackets_spec.simple_spec():
+                        self.read_expression(spec.expression(), prefix)
 
     def read_expression(self, expression: AFMParser.ExpressionContext, prefix: str) -> None:
 
         root_node = self.build_ast_node(expression, prefix)
         ast = AST(root_node)
         cst = Constraint(expression.getText(), ast)
 
@@ -184,23 +186,25 @@
 
         if expression.__class__ in binary_operation_types:
             binary_operation = expression.getChild(1).getText()
             ast_operation = binary_operations_map.get(binary_operation)
 
             # TODO: provide support for arithmetic and relational operations.
             if ast_operation is None:
-                raise Exception(f'Constraints not supported in AFM Reader: {binary_operation}.')
+                raise FlamaException(
+                    f'Constraints not supported in AFM Reader: {binary_operation}.')
             result = Node(ast_operation)
             result.left = self.build_ast_node(expression.expression()[0], prefix)
             result.right = self.build_ast_node(expression.expression()[1], prefix)
 
         if isinstance(expression, AFMParser.NotExpContext):
             result = Node(ASTOperation.NOT)
             result.right = self.build_ast_node(expression.expression(), prefix)
 
         if isinstance(expression, AFMParser.ParenthesisExpContext):
             result = self.build_ast_node(expression.expression(), prefix)
 
         if result is None:
-            raise Exception(f'Constraint not support in AFM Reader: {expression}, {prefix}')
+            raise FlamaException(
+                f'Constraint not support in AFM Reader: {expression}, {prefix}')
 
         return result
```

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/afm_writer.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/afm_writer.py`

 * *Files identical despite different names*

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/attributes_csv_reader.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/attributes_csv_reader.py`

 * *Files identical despite different names*

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/featureide_reader.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/featureide_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from xml.etree import ElementTree
 from xml.etree.ElementTree import Element
 
+from flamapy.core.exceptions import FlamaException
 from flamapy.core.models.ast import AST, Node, ASTOperation
 from flamapy.core.transformations import TextToModel
 from flamapy.metamodels.fm_metamodel.models import (
     Constraint,
     Feature,
     FeatureModel,
     Relation,
@@ -113,15 +114,15 @@
                 index += 1
             rule = ctc[index]
             ast = self._parse_rule(rule)
             if ast:
                 ctc = Constraint(str(number), ast)
                 constraints.append(ctc)
             else:
-                raise Exception()
+                raise FlamaException()
             number += 1
         return constraints
 
     def _parse_rule(self, rule: Element) -> AST:
         """Return the representation of the constraint (rule) in the AST syntax."""
         if rule.tag == FeatureIDEReader.TAG_VAR:
             node = Node(rule.text)
@@ -153,8 +154,8 @@
         elif rule.tag == FeatureIDEReader.TAG_CONJ:
             if len(rule) > 1:
                 node = Node(ASTOperation.AND)
                 node.left = self._parse_rule(rule[0]).root
                 node.right = self._parse_rule(rule[1]).root
             else:
                 node = self._parse_rule(rule[0]).root
-        return AST(node)
+        return AST(node)
```

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/glencoe_reader.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/glencoe_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import functools
 import json
 from typing import Any
 
+from flamapy.core.exceptions import FlamaException
 from flamapy.core.models.ast import AST, Node, ASTOperation
 from flamapy.core.transformations import TextToModel
 
 from flamapy.metamodels.fm_metamodel.models import FeatureModel, Feature, Relation, Constraint
 
 
 class GlencoeReader(TextToModel):
@@ -23,15 +24,15 @@
             features_info = data['features']
             root_node = data['tree']
             constraints_info = data['constraints']
             root_feature = self._parse_tree(None, root_node, features_info)
             constraints = self._parse_constraints(constraints_info, features_info)
             return FeatureModel(root_feature, constraints)
 
-    def _parse_tree(self, parent: Feature, feature_node: dict[str, Any],
+    def _parse_tree(self, parent: Feature, feature_node: dict[str, Any], 
                     features_info: dict[str, Any]) -> Feature:
         """Parse the tree structure and returns the root feature."""
         feature_id = feature_node['id']
         feature_type = features_info[feature_id]['type']
         feature = Feature(name=features_info[feature_id]['name'], parent=parent)
 
         if 'children' in feature_node:
@@ -46,15 +47,15 @@
                 elif not optional:
                     # Additional relation because Glencoe supports mandatory features in groups
                     relation = Relation(feature, [child_feature], 1, 1)
                     feature.add_relation(relation)
                     children.append(child_feature)
                 else:
                     children.append(child_feature)
-            if relation != 'FEATURE':  # group
+            if feature_type != 'FEATURE':  # group
                 if feature_type == 'XOR':
                     relation = Relation(feature, children, 1, 1)
                 elif feature_type == 'OR':
                     relation = Relation(feature, children, 1, len(children))
                 elif feature_type == 'GENOR':  # Group Cardinality
                     card_min = features_info[feature_id]['min']
                     card_max = features_info[feature_id]['max']
@@ -62,25 +63,25 @@
                 feature.add_relation(relation)
         # Create an attribute for the 'note' parameter
         # note = features_info[feature_id]['note']
         # if note:
         #     pass
         return feature
 
-    def _parse_constraints(self, ctcs_info: dict[str, Any],
+    def _parse_constraints(self, ctcs_info: dict[str, Any], 
                            features_info: dict[str, Any]) -> list[Constraint]:
         constraints = []
         print(ctcs_info)
         for i, ctc_info in enumerate(ctcs_info.values(), 1):
             ctc_node = self._parse_ast_constraint(ctc_info, features_info)
             ctc = Constraint(f'CTC{i}', AST(ctc_node))
             constraints.append(ctc)
         return constraints
 
-    def _parse_ast_constraint(self, ctc_info: dict[str, Any],
+    def _parse_ast_constraint(self, ctc_info: dict[str, Any], 
                               features_info: dict[str, Any]) -> Node:
         ctc_type = ctc_info['type']
         ctc_operands = ctc_info['operands']
         node = None
         if ctc_type == 'FeatureTerm':
             feature_id = ctc_info['operands'][0]
             feature_name = features_info[feature_id]['name']
@@ -98,17 +99,17 @@
             node = Node(ASTOperation.EXCLUDES, left, right)
         elif ctc_type == 'EquivalentTerm':
             left = self._parse_ast_constraint(ctc_operands[0], features_info)
             right = self._parse_ast_constraint(ctc_operands[1], features_info)
             node = Node(ASTOperation.EQUIVALENCE, left, right)
         elif ctc_type == 'AndTerm':
             op_list = [self._parse_ast_constraint(op, features_info) for op in ctc_operands]
-            node = functools.reduce(lambda l, r: Node(ASTOperation.AND, l, r), op_list)
+            node = functools.reduce(lambda lamb, r: Node(ASTOperation.AND, lamb, r), op_list)
         elif ctc_type == 'OrTerm':
             op_list = [self._parse_ast_constraint(op, features_info) for op in ctc_operands]
-            node = functools.reduce(lambda l, r: Node(ASTOperation.OR, l, r), op_list)
+            node = functools.reduce(lambda lamb, r: Node(ASTOperation.OR, lamb, r), op_list)
         elif ctc_type == 'XorTerm':
             op_list = [self._parse_ast_constraint(op, features_info) for op in ctc_operands]
-            node = functools.reduce(lambda l, r: Node(ASTOperation.XOR, l, r), op_list)
+            node = functools.reduce(lambda lamb, r: Node(ASTOperation.XOR, lamb, r), op_list)
         else:
-            raise Exception(f'Invalid constraint: {ctc_info}')
-        return node
+            raise FlamaException(f'Invalid constraint: {ctc_info}')
+        return node
```

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/glencoe_writer.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/glencoe_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 
     def __init__(self, path: str, source_model: FeatureModel) -> None:
         self.path = path
         self.source_model = source_model
 
     def transform(self) -> str:
         json_object = _to_json(self.source_model)
-        with open(self.path, 'w', encoding='utf8') as file:
-            json.dump(json_object, file, indent=4)
+        if self.path is not None:
+            with open(self.path, 'w', encoding='utf8') as file:
+                json.dump(json_object, file, indent=4)
         return json.dumps(json_object, indent=4)
 
 
 def _to_json(feature_model: FeatureModel) -> dict[str, Any]:
     result: dict[str, Any] = {}
     result['id'] = f'FM_{feature_model.root.name}'
     result['name'] = f'FM_{feature_model.root.name}'
@@ -57,15 +58,15 @@
             'name': feature.name,
             'optional': not feature.is_mandatory(),
             'type': feature_type,
             'note': ''  # ToDo: add 'note' attribute information
         }
 
         if feature_type == 'GENOR':
-            relation = next(r.is_cardinal() for r in feature.get_relations())
+            relation = next(r for r in feature.get_relations() if r.is_cardinal())
             features_info[feature.name]['min'] = relation.card_min
             features_info[feature.name]['max'] = relation.card_max
     return features_info
 
 
 def _get_tree_info(feature: Feature) -> dict[str, Any]:
     feature_info = {}
```

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/json_writer.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/json_writer.py`

 * *Files identical despite different names*

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/splot_writer.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/splot_writer.py`

 * *Files identical despite different names*

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/uvl_reader.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/uvl_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from typing import Any
 
 from uvlparser import get_tree
 from uvlparser.UVLParser import UVLParser
 
+from flamapy.core.exceptions import FlamaException
 from flamapy.core.transformations import TextToModel
 from flamapy.core.models.ast import AST, ASTOperation, Node
 from flamapy.metamodels.fm_metamodel.models import (
     Constraint,
     Feature,
     FeatureModel,
     Relation,
@@ -281,19 +282,19 @@
         if isinstance(expression, UVLParser.LogicalExpContext):
             logic_op_type = {UVLParser.EquivExpContext: ASTOperation.EQUIVALENCE,
                              UVLParser.ImpliesExpContext: ASTOperation.IMPLIES,
                              UVLParser.RequiresExpContext: ASTOperation.REQUIRES,
                              UVLParser.ExcludesExpContext: ASTOperation.EXCLUDES}
             logic_op = logic_op_type.get(type(expression.logical_operator()))
             if logic_op is None:
-                raise Exception(f'Constraint expression not supported by UVL reader: '
-                                f'{expression.logical_operator().getText()}')
+                raise FlamaException(f'Constraint expression not supported by UVL reader: '
+                                     f'{expression.logical_operator().getText()}')
             return Node(logic_op, left, right)
-        raise Exception(f'Constraint expression not supported by UVL reader: '
-                        f'{expression.getText()}')
+        raise FlamaException(f'Constraint expression not supported by UVL reader: '
+                             f'{expression.getText()}')
 
     def _clear_invalid_constraints(self) -> None:
         """Remove duplicate constraints and constraints that involve features not present 
         in the feature model.
 
         This can occur due to the 'imports' statement that allows importing partial sub-trees
         in the feature model, and therefore only constraints involving existing features should
```

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/uvl_writer.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/uvl_writer.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,54 +16,49 @@
     def get_destination_extension() -> str:
         return 'uvl'
 
     def __init__(self, source_model: FeatureModel, path: str):
         self.path = path
         self.model = source_model
 
-    def transform(self) -> FeatureModel:
+    def transform(self) -> str:
         model = self.model
         root = model.root
 
         serialized_model = self.read_features(
             root, "features", 0) + "\n" + self.read_constraints()
 
-        with open(self.path, 'w', encoding='utf8') as file:
-            file.write(serialized_model)
+        if self.path is not None:
+            with open(self.path, 'w', encoding='utf8') as file:
+                file.write(serialized_model)
+        return serialized_model
 
     def read_features(self, feature: Feature, result: str, tab_count: int) -> str:
         tab_count = tab_count + 1
         result = result + "\n" + tab_count * "\t" + \
-            feature.name + self.read_attributes(feature)
+            feature.name + " " + self.read_attributes(feature)
         tab_count = tab_count + 1
         for relation in feature.relations:
             relation_name = self.serialize_relation(relation)
             result = result + "\n" + tab_count * "\t" + relation_name
             for feature_node in relation.children:
                 result = self.read_features(feature_node, result, tab_count)
         return result
 
     @classmethod
     def read_attributes(cls, feature: Feature) -> str:
-        attributes = feature.get_attributes()
-        result = ""
-
-        if len(attributes) > 0:
-            result = "{"
-            first = True
-            for attribute in attributes:
-                if not first:
-                    result += ", "
-                result += attribute.name
-                if attribute.default_value is not None:
-                    result += ' "' + attribute.default_value + '"'
-                first = False
-            result += "}"
-
-        return result
+        attributes = []
+        if feature.is_abstract:
+            attributes.append('abstract')
+        for attribute in feature.get_attributes():
+            attribute_str = attribute.name
+            if attribute.default_value is not None:
+                attribute_str += f' "{attribute.default_value}"'
+            attributes.append(attribute_str)
+        return f'{{{", ".join(attributes)}}}' if attributes else ''
 
     @staticmethod
     def serialize_relation(rel: Relation) -> str:
         result = ""
 
         if rel.is_alternative():
             result = "alternative"
```

### Comparing `flamapy-fm-1.0.1.dev0/flamapy/metamodels/fm_metamodel/transformations/xml_reader.py` & `flamapy-fm-1.1.3/flamapy/metamodels/fm_metamodel/transformations/xml_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from typing import Optional
 from xml.etree import ElementTree
 
 from flamapy.core.transformations import TextToModel
 from flamapy.core.models.ast import AST, ASTOperation
-from flamapy.core.exceptions import DuplicatedFeature
+from flamapy.core.exceptions import DuplicatedFeature, FlamaException
 from flamapy.metamodels.fm_metamodel.models import (
     Constraint,
     Feature,
     FeatureModel,
     Relation,
 )
 
@@ -61,15 +61,15 @@
             destination = self.name_feature[el_exclude]
             operator_type = ASTOperation.EXCLUDES
         elif ctc_type == 'requires' and el_require in self.name_feature:
             destination = self.name_feature[el_require]
             operator_type = ASTOperation.REQUIRES
 
         if origin is None or destination is None:
-            raise Exception('origin or destination not found')
+            raise FlamaException('origin or destination not found')
 
         return Constraint(
             name,
             AST.create_simple_binary_operation(operator_type, origin.name, destination.name)
         )
 
     def parse_feature(self, element: ElementTree.Element, parent: Feature) -> Feature:
```

### Comparing `flamapy-fm-1.0.1.dev0/flamapy_fm.egg-info/SOURCES.txt` & `flamapy-fm-1.1.3/flamapy_fm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flamapy-fm-1.0.1.dev0/setup.py` & `flamapy-fm-1.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="flamapy-fm",
-    version="1.0.1.dev0",
+    version="1.1.3",
     author="Flamapy",
     author_email="flamapy@us.es",
     description="flamapy-fm is a plugin to Flamapy module",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/flamapy/fm_metamodel",
     packages=setuptools.find_namespace_packages(include=['flamapy.*']),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.9',
     install_requires=[
-        'flamapy~=1.0.1.dev0',
-        'uvlparser~=1.0.0',
+        'flamapy~=1.1.3',
+        'uvlparser~=1.0.2',
         'afmparser~=1.0.0',
     ],
     extras_require={
         'dev': [
             'pytest',
             'pytest-mock',
             'prospector',
             'mypy',
             'coverage',
         ]
     },
     dependency_links=[
-        'flamapy~=1.0.1.dev0'
+        'flamapy~=1.1.3'
     ],
 )
```

