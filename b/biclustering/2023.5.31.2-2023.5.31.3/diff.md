# Comparing `tmp/biclustering-2023.5.31.2.tar.gz` & `tmp/biclustering-2023.5.31.3.tar.gz`

## Comparing `biclustering-2023.5.31.2.tar` & `biclustering-2023.5.31.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 biclustering-2023.5.31.2/biclustering/Pattern.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 biclustering-2023.5.31.2/biclustering/__init__.py
--rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 biclustering-2023.5.31.2/biclustering/association_rules.py
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 biclustering-2023.5.31.2/biclustering/bicluster.py
--rw-r--r--   0        0        0     8039 2020-02-02 00:00:00.000000 biclustering-2023.5.31.2/biclustering/fist.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 biclustering-2023.5.31.2/biclustering/frequent_patterns.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 biclustering-2023.5.31.2/biclustering/generators.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 biclustering-2023.5.31.2/biclustering/printing_util.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 biclustering-2023.5.31.2/biclustering/suffix_tree.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 biclustering-2023.5.31.2/LICENSE
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 biclustering-2023.5.31.2/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 biclustering-2023.5.31.2/pyproject.toml
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 biclustering-2023.5.31.2/PKG-INFO
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 biclustering-2023.5.31.3/biclustering/Pattern.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 biclustering-2023.5.31.3/biclustering/__init__.py
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 biclustering-2023.5.31.3/biclustering/association_rules.py
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 biclustering-2023.5.31.3/biclustering/bicluster.py
+-rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 biclustering-2023.5.31.3/biclustering/fist.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 biclustering-2023.5.31.3/biclustering/frequent_patterns.py
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 biclustering-2023.5.31.3/biclustering/generators.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 biclustering-2023.5.31.3/biclustering/printing_util.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 biclustering-2023.5.31.3/biclustering/suffix_tree.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 biclustering-2023.5.31.3/LICENSE
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 biclustering-2023.5.31.3/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 biclustering-2023.5.31.3/pyproject.toml
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 biclustering-2023.5.31.3/PKG-INFO
```

### Comparing `biclustering-2023.5.31.2/biclustering/Pattern.py` & `biclustering-2023.5.31.3/biclustering/Pattern.py`

 * *Files identical despite different names*

### Comparing `biclustering-2023.5.31.2/biclustering/association_rules.py` & `biclustering-2023.5.31.3/biclustering/association_rules.py`

 * *Files identical despite different names*

### Comparing `biclustering-2023.5.31.2/biclustering/bicluster.py` & `biclustering-2023.5.31.3/biclustering/bicluster.py`

 * *Files identical despite different names*

### Comparing `biclustering-2023.5.31.2/biclustering/fist.py` & `biclustering-2023.5.31.3/biclustering/fist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import pandas as pd
 import math
 import csv
-from biclustering.suffix_tree import build_sufix_tree, generate_tree_image,generate_tree_JSON
+from biclustering.suffix_tree import build_sufix_tree, generate_tree_as_image,generate_tree_JSON
 from biclustering.frequent_patterns import get_FCPs, convert_fcp_to_csv, convert_fcp_to_JSON
 from biclustering.generators import get_generators, write_generators_to_csv, write_generators_toJSON
 from biclustering.association_rules import Rule
 from biclustering.bicluster import generate_biclusters
 
 class FIST:
     def __init__(self):
@@ -117,15 +117,15 @@
         return self.sfd            
     
     def build_tree(self, produce_suffix_tree_image = False):
         self.h_tree = build_sufix_tree(self.sfd)
         tree_path = f'{self.output_directory_path}/suffixTree.dataset={self.dataset_name}.minSupport={self.min_sup_percent}%.'
         generate_tree_JSON(self.h_tree,tree_path+"json")
         if(produce_suffix_tree_image):
-            generate_tree_image(self.h_tree,tree_path+"png")
+            generate_tree_as_image(self.h_tree,tree_path+"png")
         
         return self.h_tree
 
     def extract_fcp_list(self, min_support_count, generate_fcp_file=True):
         self.fcp_list = get_FCPs(self.h_tree, min_support_count)
         if(generate_fcp_file):
             fcp_path = f'{self.output_directory_path}/FCP.dataset={self.dataset_name}.minSupport={self.min_sup_percent}%.'
```

### Comparing `biclustering-2023.5.31.2/biclustering/frequent_patterns.py` & `biclustering-2023.5.31.3/biclustering/frequent_patterns.py`

 * *Files identical despite different names*

### Comparing `biclustering-2023.5.31.2/biclustering/generators.py` & `biclustering-2023.5.31.3/biclustering/generators.py`

 * *Files identical despite different names*

### Comparing `biclustering-2023.5.31.2/biclustering/printing_util.py` & `biclustering-2023.5.31.3/biclustering/printing_util.py`

 * *Files identical despite different names*

### Comparing `biclustering-2023.5.31.2/biclustering/suffix_tree.py` & `biclustering-2023.5.31.3/biclustering/suffix_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     while idx < len(arr):
         suffix.append(arr[idx])
         idx += 1
 
     suffix.append(leaf_obj)
     return suffix
 
-def generate_tree_image(tree,tree_path):
+def generate_tree_as_image(tree,tree_path):
     # output-3 : Tree Image
     generate_tree_image(tree, tree_path )
     print("\nImage of the suffix tree is generated in file : ",tree_path)
 
 
 def generate_tree_JSON(tree,tree_path):
```

### Comparing `biclustering-2023.5.31.2/LICENSE` & `biclustering-2023.5.31.3/LICENSE`

 * *Files identical despite different names*

### Comparing `biclustering-2023.5.31.2/README.md` & `biclustering-2023.5.31.3/README.md`

 * *Files identical despite different names*

### Comparing `biclustering-2023.5.31.2/pyproject.toml` & `biclustering-2023.5.31.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "biclustering"
-version = "2023.05.31.2"
+version = "2023.05.31.3"
 authors = [
   { name="Mijanur Rahaman Mallick", email="mijanur08@gmail.com" }
 ]
 description = "Biclustering and association rule mining using Suffix Tree and Frequent Closed Itemset based algorithm."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `biclustering-2023.5.31.2/PKG-INFO` & `biclustering-2023.5.31.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biclustering
-Version: 2023.5.31.2
+Version: 2023.5.31.3
 Summary: Biclustering and association rule mining using Suffix Tree and Frequent Closed Itemset based algorithm.
 Project-URL: Homepage, https://github.com/Mijanur08/biclusturing-using-suffixTree
 Project-URL: Bug Tracker, https://github.com/Mijanur08/biclusturing-using-suffixTree/issues
 Author-email: Mijanur Rahaman Mallick <mijanur08@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

