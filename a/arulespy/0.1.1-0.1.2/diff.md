# Comparing `tmp/arulespy-0.1.1.tar.gz` & `tmp/arulespy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arulespy-0.1.1.tar", last modified: Mon May 22 18:09:37 2023, max compression
+gzip compressed data, was "arulespy-0.1.2.tar", last modified: Wed May 31 16:19:17 2023, max compression
```

## Comparing `arulespy-0.1.1.tar` & `arulespy-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:09:37.122646 arulespy-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-22 18:09:24.000000 arulespy-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 18:09:24.000000 arulespy-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-05-22 18:09:37.122646 arulespy-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-22 18:09:24.000000 arulespy-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 18:09:24.000000 arulespy-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-22 18:09:37.122646 arulespy-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-22 18:09:24.000000 arulespy-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:09:37.122646 arulespy-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:09:37.122646 arulespy-0.1.1/src/arulespy/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-22 18:09:24.000000 arulespy-0.1.1/src/arulespy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-05-22 18:09:24.000000 arulespy-0.1.1/src/arulespy/arules.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-22 18:09:24.000000 arulespy-0.1.1/src/arulespy/arulesViz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:09:37.122646 arulespy-0.1.1/src/arulespy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-05-22 18:09:37.000000 arulespy-0.1.1/src/arulespy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-22 18:09:37.000000 arulespy-0.1.1/src/arulespy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:09:37.000000 arulespy-0.1.1/src/arulespy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 18:09:37.000000 arulespy-0.1.1/src/arulespy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 18:09:37.000000 arulespy-0.1.1/src/arulespy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:09:37.122646 arulespy-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-22 18:09:24.000000 arulespy-0.1.1/tests/test_arules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:19:17.344966 arulespy-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-31 16:19:07.000000 arulespy-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-31 16:19:07.000000 arulespy-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-31 16:19:17.344966 arulespy-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-05-31 16:19:07.000000 arulespy-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-31 16:19:07.000000 arulespy-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-31 16:19:17.344966 arulespy-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-31 16:19:07.000000 arulespy-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:19:17.344966 arulespy-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:19:17.344966 arulespy-0.1.2/src/arulespy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-31 16:19:07.000000 arulespy-0.1.2/src/arulespy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-05-31 16:19:07.000000 arulespy-0.1.2/src/arulespy/arules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-31 16:19:07.000000 arulespy-0.1.2/src/arulespy/arulesViz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:19:17.344966 arulespy-0.1.2/src/arulespy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-31 16:19:17.000000 arulespy-0.1.2/src/arulespy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-31 16:19:17.000000 arulespy-0.1.2/src/arulespy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 16:19:17.000000 arulespy-0.1.2/src/arulespy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-31 16:19:17.000000 arulespy-0.1.2/src/arulespy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 16:19:17.000000 arulespy-0.1.2/src/arulespy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:19:17.344966 arulespy-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-31 16:19:07.000000 arulespy-0.1.2/tests/test_arules.py
```

### Comparing `arulespy-0.1.1/LICENSE` & `arulespy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arulespy-0.1.1/PKG-INFO` & `arulespy-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arulespy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python interface to the R package arules
 Home-page: https://github.com/mhahsler/arulespy
 Author: Michael Hahsler
 Author-email: mhahsler@lyle.smu.edu
 Project-URL: Documentation, https://github.com/mhahsler/arulespy
 Project-URL: Bug Reports, https://github.com/mhahsler/arulespy/issues
 Project-URL: Source Code, https://github.com/mhahsler/arulespy
@@ -14,15 +14,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: R
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Python interface to the R package arules
 
 [![PyPI
@@ -141,14 +141,16 @@
 Complete examples:
   * [Using arules](https://mhahsler.github.io/arulespy/examples/arules.html)
   * [Using arulesViz](https://mhahsler.github.io/arulespy/examples/arulesViz.html)
 
 
 ## References
 
+- Michael Hahsler. [ARULESPY: Exploring association rules and frequent itemsets in 
+  Python.](http://dx.doi.org/10.48550/arXiv.2305.15263) arXiv:2305.15263 [cs.DB], May 2023. 
 - Michael Hahsler, Sudheer Chelluboina, Kurt Hornik, and Christian
   Buchta. [The arules R-package ecosystem: Analyzing interesting
   patterns from large transaction
   datasets.](https://jmlr.csail.mit.edu/papers/v12/hahsler11a.html)
   *Journal of Machine Learning Research,* 12:1977-1981, 2011.
 - Michael Hahsler, Bettina Grün and Kurt Hornik. [arules - A
   Computational Environment for Mining Association Rules and Frequent
```

### Comparing `arulespy-0.1.1/README.md` & `arulespy-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,16 @@
 Complete examples:
   * [Using arules](https://mhahsler.github.io/arulespy/examples/arules.html)
   * [Using arulesViz](https://mhahsler.github.io/arulespy/examples/arulesViz.html)
 
 
 ## References
 
+- Michael Hahsler. [ARULESPY: Exploring association rules and frequent itemsets in 
+  Python.](http://dx.doi.org/10.48550/arXiv.2305.15263) arXiv:2305.15263 [cs.DB], May 2023. 
 - Michael Hahsler, Sudheer Chelluboina, Kurt Hornik, and Christian
   Buchta. [The arules R-package ecosystem: Analyzing interesting
   patterns from large transaction
   datasets.](https://jmlr.csail.mit.edu/papers/v12/hahsler11a.html)
   *Journal of Machine Learning Research,* 12:1977-1981, 2011.
 - Michael Hahsler, Bettina Grün and Kurt Hornik. [arules - A
   Computational Environment for Mining Association Rules and Frequent
```

### Comparing `arulespy-0.1.1/setup.py` & `arulespy-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,18 @@
 
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
 
         'Operating System :: OS Independent',
 
         'Topic :: Scientific/Engineering :: Information Analysis'
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=['pandas',
+                      'numpy',
+                      'scipy',
                       'rpy2'                   
                       ],
     # install_requires=['Pillow'],
     extras_require={
         'dev': ['check-manifest'],
         # 'test': ['coverage'],
     },
```

### Comparing `arulespy-0.1.1/src/arulespy/__init__.py` & `arulespy-0.1.2/src/arulespy/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 
 import rpy2.robjects as ro
 import rpy2.robjects.packages as packages
 import os
 
 os.makedirs(ro.r('Sys.getenv("R_LIBS_USER")')[0], exist_ok=True)
 ro.r('.libPaths(c(Sys.getenv("R_LIBS_USER"), .libPaths()))')
```

### Comparing `arulespy-0.1.1/src/arulespy/arules.py` & `arulespy-0.1.2/src/arulespy/arules.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """The arules module provides an interface to R's arules package."""
 
 import pandas as pd
 import numpy as np
+from scipy.sparse import csc_matrix
 
 import rpy2.robjects as ro
 import rpy2.robjects.packages as packages
 from rpy2.robjects import pandas2ri
 
 ### activate automatic conversion of pandas dataframes to R dataframes
 #pandas2ri.activate()
@@ -14,55 +15,122 @@
 # we try to create the directory so install.packages does not ask
 
 ### import the R arules package
 R = packages.importr('arules')
 methods = packages.importr('methods')
 base = packages.importr('base')
 
+### Sparse matrix helper
+def ngC_to_csc_matrix(m):
+    """convert a ngCMatrix to a scipy csc_matrix"""
+    indices = np.array(m.slots['i'])
+    indptr  = np.array(m.slots['p'])
+    ## all ones for ngCMatrix
+    data = np.array([1]*len(indices))
+    return csc_matrix((data, indices, indptr), tuple(m.slots['Dim']))    
+
+### Conversion functions
+def a2py(x):
+    """convert arules S4 object to python object
+    
+    Conversion rules:
+    - rules: Python Rules object
+    - itemsets: Python Itemsets object
+    - transactions: Python Transactions object
+    - itemMatrix: Python ItemMatrix object
+    - data.frame: pandas dataframe
+    - character: string list
+    - integer: int list
+    - numeric: float list
+    - matrix: numpy matrix
+    """
+
+    if x.rclass[0] == "rules":
+        return Rules(x)
+    elif x.rclass[0] == "itemsets":
+        return Itemsets(x)
+    elif x.rclass[0] == "transactions":
+        return Transactions(x)
+    elif x.rclass[0] == "itemMatrix":
+        return ItemMatrix(x)
+    elif x.rclass[0] == "data.frame":
+        colnames = list(x.colnames)
+        with (ro.default_converter + ro.pandas2ri.converter).context():
+            pd_df = ro.conversion.get_conversion().rpy2py(x)
+
+        if type(pd_df) != pd.core.frame.DataFrame:
+            pd_df = pd.DataFrame(pd_df, columns= colnames)   ### set column name!
+        return pd_df   
+    elif x.rclass[0] in ["character", "integer", "numeric", "logical"]:
+        return list(x)
+    elif x.rclass[0] == "matrix":
+        return np.array(x)
+
+    else:
+        return x
+
+def a2py_decor(function):
+    """decorator to convert arules S4 objects to python objects"""
+
+    def wrapper(*args, **kwargs):
+        return a2py(function(*args, **kwargs))
+    return wrapper
+
+
 ### arules interface code 
 
 def parameters(x):
     """define parameters for apriori and eclat"""
 
     return ro.ListVector(x)
 
 
 class ItemMatrix(ro.RS4):
     """Class for arules itemMatrix object"""
     
     @staticmethod
     def from_list(items, itemLabels):
+        """convert list of lists into an arules itemMatrix object"""
         items = [ro.StrVector(x) for x in items]
         return ItemMatrix(R.encode(items, itemLabels))
 
     def as_df(self):
         """convert to pandas dataframe"""
         if type(self) != ro.vectors.DataFrame:
             self  = R.DATAFRAME(self)
         with (ro.default_converter + pandas2ri.converter).context():
             pd_df = ro.conversion.get_conversion().rpy2py(self)
         return pd_df
     
     def as_matrix(self):
-        """convert to numpy matrix
-        """
+        """convert to numpy matrix"""
 
         return np.array(ro.r('function(x) as(x, "matrix")')(self))
 
+    def as_csc_matrix(self):
+        """convert to scipy sparse matrix"""
+
+        return ngC_to_csc_matrix(self.slots['data'])
+
     def as_dict(self):
-        """convert to dictionary
-        """
+        """convert to dictionary"""
 
         l = ro.r('function(x) as(x, "list")')(self)
         l.names = [*range(0, len(l))]
         return dict(zip(l.names, map(list,list(l))))
       
     def as_list(self):
         """convert to list"""
         return list(self.as_dict().values())  
+    
+    def as_int_list(self):
+        """convert to int list"""
+
+        l = ro.r('function(x) LIST(x, decode = FALSE)')(self)
+        return [list(x) for x in l]
 
     def __getitem__(self, key):
         # prepare subset selection
         if isinstance(key, slice):
             key = list(range(key.stop)[key])  
         
         key = np.array(key)
@@ -119,44 +187,59 @@
     
     def itemFrequency(self, type = "absolute"):
         """return item frequency
         
         Args:
             type: "absolute" or "relative"
         """
-        return np.array(a2py(ro.r('function(x, type) itemFrequency(x, type)')(self, type)))
+        return a2py(ro.r('function(x, type) itemFrequency(x, type)')(self, type))
     
     def itemInfo(self):
         """return item info as dataframe"""
         return a2py(ro.r('function(x) itemInfo(x)')(self))
     
     def labels(self):
         """returns a list of labels for the sets"""
         return a2py(ro.r('function(x) labels(x)')(self))
     
-    def is_subset(self, x, sparse = False):
+    def itemLabels(self):
+        """returns a list of labels for the sets"""
+        return a2py(ro.r('function(x) itemLabels(x)')(self))
+    
+    def is_subset(self, x, proper = False, sparse = True):
         """check if x is a subset of self
         
         Args:
             x: the other set
-            sparse: return sparse matrix representation?
+            proper: proper subset?
+            sparse: return sparse matrix representation as a scipy.sparse.csc_matrix?
         """    
-        sparse = ro.vectors.BoolVector([sparse])
-        return ro.r('function(x, y, sparse) is.subset(x, y, sparse)')(self, x, sparse)
+        m = ro.r('function(x, y, proper, sparse) is.subset(x, y, proper, sparse)')(self, x, 
+                        ro.vectors.BoolVector([proper]), ro.vectors.BoolVector([sparse]))
+
+        if sparse:
+            return ngC_to_csc_matrix(m)
+        else:
+            return np.array(m)  
     
-    def is_superset(self, x, sparse = False):
+    def is_superset(self, x, proper = False, sparse = True):
         """check if x is a superset of self
         
         Args:
             x: the other set
-            sparse: return sparse matrix representation?
+            proper: proper superset?
+            sparse: return sparse matrix representation as a scipy.sparse.csc_matrix?
         """
-        sparse = ro.vectors.BoolVector([sparse])
-        return ro.r('function(x, y, sparse) is.superset(x, y, sparse)')(self, x, sparse)
-            
+        m = ro.r('function(x, y, proper, sparse) is.superset(x, y, proper, sparse)')(self, x, 
+                        ro.vectors.BoolVector([proper]), ro.vectors.BoolVector([sparse]))
+
+        if sparse:
+            return ngC_to_csc_matrix(m)
+        else:
+            return np.array(m)     
 
 class Associations(ItemMatrix):
     """Superclass for arules associations (rules/itemsets)"""
 
     def quality(self):
         """return quality measures as dataframe"""
         return a2py(ro.r('function(x) quality(x)')(self))
@@ -230,15 +313,15 @@
 class Itemsets(Associations):
     """Class for arules itemsets object"""
     
     @staticmethod
     def new(items, quality = None):
 
         if quality == None:
-             return a2py(methods.new("itemsets", items))
+            return a2py(methods.new("itemsets", items))
         else:
             return a2py(methods.new("itemsets", items, quality))
     
     def items(self):
         """return items as an itemMatrix"""
         return ItemMatrix(ro.r('function(x) lhs(x)')(self))
 
@@ -258,63 +341,14 @@
             x_r = ro.conversion.get_conversion().py2rpy(x)
     
         if itemLabels == None:
             return Transactions(R.transactions(x_r))
         else:
             return Transactions(R.transactions(x_r, itemLabels))
 
-### Conversion functions
-
-def a2py(x):
-    """convert arules S4 object to python object
-    
-    Conversion rules:
-    - rules: Python Rules object
-    - itemsets: Python Itemsets object
-    - transactions: Python Transactions object
-    - itemMatrix: Python ItemMatrix object
-    - data.frame: pandas dataframe
-    - character: string list
-    - integer: int list
-    - numeric: float list
-    - matrix: numpy matrix
-    """
-
-    if x.rclass[0] == "rules":
-        return Rules(x)
-    elif x.rclass[0] == "itemsets":
-        return Itemsets(x)
-    elif x.rclass[0] == "transactions":
-        return Transactions(x)
-    elif x.rclass[0] == "itemMatrix":
-        return ItemMatrix(x)
-    elif x.rclass[0] == "data.frame":
-        colnames = list(x.colnames)
-        with (ro.default_converter + ro.pandas2ri.converter).context():
-            pd_df = ro.conversion.get_conversion().rpy2py(x)
-
-        if type(pd_df) != pd.core.frame.DataFrame:
-            pd_df = pd.DataFrame(pd_df, columns= colnames)   ### set column name!
-        return pd_df   
-    elif x.rclass[0] == "character" or x.rclass[0] == "integer" or x.rclass[0] == "numeric":
-        return list(x)
-    elif x.rclass[0] == "matrix":
-        return np.array(x)
-
-    else:
-        return x
-
-
-def a2py_decor(function):
-    """decorator to convert arules S4 objects to python objects"""
-
-    def wrapper(*args, **kwargs):
-        return a2py(function(*args, **kwargs))
-    return wrapper
-
 
 # package functions
 discretizeDF = a2py_decor(R.discretizeDF)
 discretizeDF.__doc__ = R.discretizeDF.__doc__   
 
 
 apriori = a2py_decor(R.apriori)
```

### Comparing `arulespy-0.1.1/src/arulespy.egg-info/PKG-INFO` & `arulespy-0.1.2/src/arulespy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arulespy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python interface to the R package arules
 Home-page: https://github.com/mhahsler/arulespy
 Author: Michael Hahsler
 Author-email: mhahsler@lyle.smu.edu
 Project-URL: Documentation, https://github.com/mhahsler/arulespy
 Project-URL: Bug Reports, https://github.com/mhahsler/arulespy/issues
 Project-URL: Source Code, https://github.com/mhahsler/arulespy
@@ -14,15 +14,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: R
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Python interface to the R package arules
 
 [![PyPI
@@ -141,14 +141,16 @@
 Complete examples:
   * [Using arules](https://mhahsler.github.io/arulespy/examples/arules.html)
   * [Using arulesViz](https://mhahsler.github.io/arulespy/examples/arulesViz.html)
 
 
 ## References
 
+- Michael Hahsler. [ARULESPY: Exploring association rules and frequent itemsets in 
+  Python.](http://dx.doi.org/10.48550/arXiv.2305.15263) arXiv:2305.15263 [cs.DB], May 2023. 
 - Michael Hahsler, Sudheer Chelluboina, Kurt Hornik, and Christian
   Buchta. [The arules R-package ecosystem: Analyzing interesting
   patterns from large transaction
   datasets.](https://jmlr.csail.mit.edu/papers/v12/hahsler11a.html)
   *Journal of Machine Learning Research,* 12:1977-1981, 2011.
 - Michael Hahsler, Bettina Grün and Kurt Hornik. [arules - A
   Computational Environment for Mining Association Rules and Frequent
```

### Comparing `arulespy-0.1.1/tests/test_arules.py` & `arulespy-0.1.2/tests/test_arules.py`

 * *Files identical despite different names*

