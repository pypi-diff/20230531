# Comparing `tmp/triclustering-2023.5.31.0.tar.gz` & `tmp/triclustering-2023.5.31.1.tar.gz`

## Comparing `triclustering-2023.5.31.0.tar` & `triclustering-2023.5.31.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 triclustering-2023.5.31.0/triclustering/Pattern.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 triclustering-2023.5.31.0/triclustering/__init__.py
--rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 triclustering-2023.5.31.0/triclustering/association_rules.py
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 triclustering-2023.5.31.0/triclustering/frequent_patterns.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 triclustering-2023.5.31.0/triclustering/generators.py
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 triclustering-2023.5.31.0/triclustering/printing_util.py
--rw-r--r--   0        0        0    10116 2020-02-02 00:00:00.000000 triclustering-2023.5.31.0/triclustering/processor.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 triclustering-2023.5.31.0/triclustering/suffix_forest.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 triclustering-2023.5.31.0/triclustering/tricluster.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 triclustering-2023.5.31.0/triclustering/util.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 triclustering-2023.5.31.0/LICENSE
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 triclustering-2023.5.31.0/README.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 triclustering-2023.5.31.0/pyproject.toml
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 triclustering-2023.5.31.0/PKG-INFO
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 triclustering-2023.5.31.1/triclustering/Pattern.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 triclustering-2023.5.31.1/triclustering/__init__.py
+-rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 triclustering-2023.5.31.1/triclustering/association_rules.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 triclustering-2023.5.31.1/triclustering/frequent_patterns.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 triclustering-2023.5.31.1/triclustering/generators.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 triclustering-2023.5.31.1/triclustering/printing_util.py
+-rw-r--r--   0        0        0    10186 2020-02-02 00:00:00.000000 triclustering-2023.5.31.1/triclustering/processor.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 triclustering-2023.5.31.1/triclustering/suffix_forest.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 triclustering-2023.5.31.1/triclustering/tricluster.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 triclustering-2023.5.31.1/triclustering/util.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 triclustering-2023.5.31.1/LICENSE
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 triclustering-2023.5.31.1/README.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 triclustering-2023.5.31.1/pyproject.toml
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 triclustering-2023.5.31.1/PKG-INFO
```

### Comparing `triclustering-2023.5.31.0/triclustering/Pattern.py` & `triclustering-2023.5.31.1/triclustering/Pattern.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from triclustering.util import get_support_count
 import copy
-from util import get_support_count
 
 class Pattern:
     def __init__(self, itemset: set, object: dict):
         self.itemset = set(itemset)
         self.object = copy.deepcopy(object)
     
     def __eq__(self, __o) -> bool:
```

### Comparing `triclustering-2023.5.31.0/triclustering/association_rules.py` & `triclustering-2023.5.31.1/triclustering/association_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from util import get_support_count
+from triclustering.util import get_support_count
 import pandas as pd
 import copy
 import json
 
 
 def find_support_count(itemset: set, FCPs: list) -> int:
     max_count = 0
```

### Comparing `triclustering-2023.5.31.0/triclustering/frequent_patterns.py` & `triclustering-2023.5.31.1/triclustering/frequent_patterns.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import copy
-from Pattern import Pattern
+from triclustering.Pattern import Pattern
 
 
 def get_FCPs(h_tree, min_support_count = 1):
     """Returns all the Frequent Closed Patterns from the suffix forest h_tree"""
     all_patterns = get_all_Patterns(h_tree)
     FCP = [pattern for pattern in all_patterns if pattern.is_closed(all_patterns)]
```

### Comparing `triclustering-2023.5.31.0/triclustering/generators.py` & `triclustering-2023.5.31.1/triclustering/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import itertools
-from Pattern import Pattern
-from util import get_support_count
+from triclustering.Pattern import Pattern
+from triclustering.util import get_support_count
 import pandas as pd
+import itertools
 
 def get_generators(FCP: list):
     """Returns the list of generators from the FCP list"""
     FCP.sort(key = comparator)
     GEN = []
     
     for i in range(len(FCP)):
```

### Comparing `triclustering-2023.5.31.0/triclustering/printing_util.py` & `triclustering-2023.5.31.1/triclustering/printing_util.py`

 * *Files identical despite different names*

### Comparing `triclustering-2023.5.31.0/triclustering/processor.py` & `triclustering-2023.5.31.1/triclustering/processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+from triclustering.suffix_forest import build_sufix_forest, produce_forest_json
+from triclustering.frequent_patterns import get_FCPs
+from triclustering.generators import get_generators, write_generators_to_csv
+from triclustering.association_rules import Rule
+from triclustering.tricluster import write_triclusters_to_csv, write_triclusters_to_json
 import pandas as pd
 import math
-from suffix_forest import build_sufix_forest, produce_forest_json
-from frequent_patterns import get_FCPs
-from generators import get_generators, write_generators_to_csv
-from association_rules import Rule
-from tricluster import write_triclusters_to_csv, write_triclusters_to_json
 import os
 
 class Processor:
     def __init__(self):
         self.h_tree = None
         self.df = None
         self.OID_ATTR = 'OID'
```

### Comparing `triclustering-2023.5.31.0/triclustering/suffix_forest.py` & `triclustering-2023.5.31.1/triclustering/suffix_forest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from triclustering.printing_util import generate_forest_image
 import copy
-from printing_util import generate_forest_image
 import json
 
 def get_all_suffix(arr, leaf_obj):
     all_suffix = []
 
     for i in range(len(arr)):
         all_suffix.append(get_suffix(arr, i, copy.deepcopy(leaf_obj)))
```

### Comparing `triclustering-2023.5.31.0/triclustering/tricluster.py` & `triclustering-2023.5.31.1/triclustering/tricluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import pandas as pd
 import json
 
 def get_clusters(FCP: list, min_support_count = 1) ->list:
     """Returns a list of tri-clusters from the given list of FCPs"""
     
     return [fcp.toJSON(include_object=True)
```

### Comparing `triclustering-2023.5.31.0/LICENSE` & `triclustering-2023.5.31.1/LICENSE`

 * *Files identical despite different names*

### Comparing `triclustering-2023.5.31.0/README.md` & `triclustering-2023.5.31.1/README.md`

 * *Files identical despite different names*

### Comparing `triclustering-2023.5.31.0/pyproject.toml` & `triclustering-2023.5.31.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "triclustering"
-version = "2023.05.31.0"
+version = "2023.05.31.1"
 authors = [
   { name="Dhiraj Bag", email="dhirajbag.db@gmail.com" }
 ]
 description = "Triclustering and association rule mining Suffix Forest and Frequent Closed Itemset based algorithm."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `triclustering-2023.5.31.0/PKG-INFO` & `triclustering-2023.5.31.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triclustering
-Version: 2023.5.31.0
+Version: 2023.5.31.1
 Summary: Triclustering and association rule mining Suffix Forest and Frequent Closed Itemset based algorithm.
 Project-URL: Homepage, https://github.com/dhirajbag/triclustering-using-suffix_forest
 Project-URL: Bug Tracker, https://github.com/dhirajbag/triclustering-using-suffix_forest/issues
 Author-email: Dhiraj Bag <dhirajbag.db@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

