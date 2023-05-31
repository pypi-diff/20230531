# Comparing `tmp/weighted_tqdm-0.8.tar.gz` & `tmp/weighted_tqdm-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weighted_tqdm-0.8.tar", last modified: Tue May 30 15:46:16 2023, max compression
+gzip compressed data, was "weighted_tqdm-0.9.tar", last modified: Wed May 31 17:54:11 2023, max compression
```

## Comparing `weighted_tqdm-0.8.tar` & `weighted_tqdm-0.9.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 15:46:16.890186 weighted_tqdm-0.8/
--rw-rw-rw-   0        0        0     1096 2023-05-30 15:42:25.000000 weighted_tqdm-0.8/LICENSE
--rw-rw-rw-   0        0        0     3110 2023-05-30 15:46:16.891187 weighted_tqdm-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2589 2023-05-30 15:45:46.000000 weighted_tqdm-0.8/README.md
--rw-rw-rw-   0        0        0      516 2023-05-30 15:46:16.894183 weighted_tqdm-0.8/setup.cfg
--rw-rw-rw-   0        0        0      867 2023-05-30 15:42:25.000000 weighted_tqdm-0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:46:16.851792 weighted_tqdm-0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-30 15:46:16.862962 weighted_tqdm-0.8/src/weighted_tqdm/
--rw-rw-rw-   0        0        0       68 2023-04-26 13:34:55.000000 weighted_tqdm-0.8/src/weighted_tqdm/__init__.py
--rw-rw-rw-   0        0        0    18996 2023-05-30 15:29:27.000000 weighted_tqdm-0.8/src/weighted_tqdm/weighted_tqdm.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:46:16.888021 weighted_tqdm-0.8/src/weighted_tqdm.egg-info/
--rw-rw-rw-   0        0        0     3110 2023-05-30 15:46:16.000000 weighted_tqdm-0.8/src/weighted_tqdm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-05-30 15:46:16.000000 weighted_tqdm-0.8/src/weighted_tqdm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 15:46:16.000000 weighted_tqdm-0.8/src/weighted_tqdm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-30 15:46:16.000000 weighted_tqdm-0.8/src/weighted_tqdm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-30 15:46:16.000000 weighted_tqdm-0.8/src/weighted_tqdm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 17:54:11.535296 weighted_tqdm-0.9/
+-rw-rw-rw-   0        0        0     1096 2023-05-31 17:53:51.000000 weighted_tqdm-0.9/LICENSE
+-rw-rw-rw-   0        0        0     3110 2023-05-31 17:54:11.536295 weighted_tqdm-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2589 2023-05-31 17:53:51.000000 weighted_tqdm-0.9/README.md
+-rw-rw-rw-   0        0        0      516 2023-05-31 17:54:11.541855 weighted_tqdm-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      868 2023-05-31 17:53:51.000000 weighted_tqdm-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 17:54:11.415046 weighted_tqdm-0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 17:54:11.437134 weighted_tqdm-0.9/src/weighted_tqdm/
+-rw-rw-rw-   0        0        0       68 2023-04-26 13:34:55.000000 weighted_tqdm-0.9/src/weighted_tqdm/__init__.py
+-rw-rw-rw-   0        0        0    17904 2023-05-31 17:49:16.000000 weighted_tqdm-0.9/src/weighted_tqdm/weighted_tqdm.py
+drwxrwxrwx   0        0        0        0 2023-05-31 17:54:11.527716 weighted_tqdm-0.9/src/weighted_tqdm.egg-info/
+-rw-rw-rw-   0        0        0     3110 2023-05-31 17:54:10.000000 weighted_tqdm-0.9/src/weighted_tqdm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-05-31 17:54:11.000000 weighted_tqdm-0.9/src/weighted_tqdm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 17:54:10.000000 weighted_tqdm-0.9/src/weighted_tqdm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-31 17:54:10.000000 weighted_tqdm-0.9/src/weighted_tqdm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-31 17:54:10.000000 weighted_tqdm-0.9/src/weighted_tqdm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 17:54:11.533295 weighted_tqdm-0.9/test/
+-rw-rw-rw-   0        0        0      452 2023-05-31 17:24:42.000000 weighted_tqdm-0.9/test/test_kronbinations_tqdm.py
```

### Comparing `weighted_tqdm-0.8/LICENSE` & `weighted_tqdm-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `weighted_tqdm-0.8/PKG-INFO` & `weighted_tqdm-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: weighted_tqdm
-Version: 0.8
+Version: 0.9
 Summary: weighted_tqdm allows for weighted iterations in tqdm progress bars.
-Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.8.tar.gz
+Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.9.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `weighted_tqdm-0.8/README.md` & `weighted_tqdm-0.9/README.md`

 * *Files identical despite different names*

### Comparing `weighted_tqdm-0.8/setup.cfg` & `weighted_tqdm-0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206b 726f 6e62 696e 6174 696f 6e73   = kronbinations
-00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 380d  ..version = 0.8.
+00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 390d  ..version = 0.9.
 00000030: 0a61 7574 686f 7220 3d20 4d69 6368 6165  .author = Michae
 00000040: 6c20 5363 6869 6c6c 696e 670d 0a61 7574  l Schilling..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6d69 6368  hor_email = mich
 00000060: 6165 6c40 6e74 726f 7069 632e 6465 0d0a  ael@ntropic.de..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 7765  description = we
 00000080: 6967 6874 6564 5f74 7164 6d20 616c 6c6f  ighted_tqdm allo
 00000090: 7773 2066 6f72 2077 6569 6768 7465 6420  ws for weighted 
@@ -15,15 +15,15 @@
 000000e0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
 000000f0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
 00000100: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
 00000110: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
 00000120: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4e  s://github.com/N
 00000130: 7472 6f70 6963 2f77 6569 6768 7465 645f  tropic/weighted_
 00000140: 7471 646d 2f61 7263 6869 7665 2f72 6566  tqdm/archive/ref
-00000150: 732f 7461 6773 2f76 302e 382e 7461 722e  s/tags/v0.8.tar.
+00000150: 732f 7461 6773 2f76 302e 392e 7461 722e  s/tags/v0.9.tar.
 00000160: 677a 0d0a 5072 6f67 7261 6d6d 696e 6720  gz..Programming 
 00000170: 4c61 6e67 7561 6765 203d 203a 2050 7974  Language = : Pyt
 00000180: 686f 6e20 3a3a 2033 0d0a 094c 6963 656e  hon :: 3...Licen
 00000190: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
 000001a0: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
 000001b0: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
 000001c0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
```

### Comparing `weighted_tqdm-0.8/setup.py` & `weighted_tqdm-0.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "weighted_tqdm",
-    version        = "0.8",
+    version         = "0.9",
     author = "Michael Schilling",
     author_email = "michael@ntropic.de",
     description  = "weighted_tqdm allows for weighted iterations in tqdm progress bars.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.8.tar.gz",
+    url = "https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.9.tar.gz",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
```

### Comparing `weighted_tqdm-0.8/src/weighted_tqdm/weighted_tqdm.py` & `weighted_tqdm-0.9/src/weighted_tqdm/weighted_tqdm.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,23 @@
 def make_weight_list(iterable, total, weights=None):
     # determine the sum of the weights if weights is specified otherwise assume weights are all 1
     if weights is not None:
         if hasattr(weights, '__iter__'): #isinstance(weights, (list, tuple, np.ndarray)):
             min_weight = min(weights)
             weights = [int(i/min_weight) for i in weights]
             weight_sum = sum(weights)
-        else:
+        # if callable
+        elif callable(weights):
             weight_vals = [weights(i) for i in iterable]
             min_weight = min(weight_vals)
             weights = [int(i/min_weight) for i in weight_vals]
             weight_sum = sum(weights)
+        else: # constant
+            weight_sum = weights*total
+            weights = [weights]*total
     else:
         weight_sum = total
         weights = [1]*total
     return weights, weight_sum
 
 def weighted_tqdm(iterable, weights=None, name='', print_val=False, bar_format='{l_bar}{bar}| {elapsed}<{remaining}', max_rate=30, **kwargs):
     total = determine_length_of_iterable(iterable, weights, **kwargs)
@@ -251,37 +255,34 @@
       
 #p = progress(total=1000)
 #for i in p.weighted_tqdm(range(5), weights=lambda i: (i+1), name='outer'):
 #    for j in p.tqdm((1,2,3,4,5), name='inner'):
 #        time.sleep(0.1*(i+1))      
 
 class weighted_kronbinations_tqdm:
-    def __init__(self, list_of_iterators, list_of_weights, total=1000, bar_format='{l_bar}{bar}| {elapsed}<{remaining}', max_rate=30, **kwargs):
+    def __init__(self, list_of_iterators, list_of_weights, total=1000, bar_format='{l_bar}{bar}| {elapsed}<{remaining}', **kwargs):
         # this function takes a list of iterators and weights and returns a generator that iterates through the kronecker product of the iterators
         # Prepare data
         lengths = []
         weights = []
         for i, w in zip(list_of_iterators, list_of_weights):
             lengths.append(determine_length_of_iterable(i, w, **kwargs))
             weights_var, sum_weights = make_weight_list(i, lengths[-1], w)
             weights.append([j/sum_weights for j in weights_var])
         self.lengths = lengths
-        self.total_length = np.prod(lengths)
         self.weights = weights
         self.total = total
         # Variables for subincrements 
         # similar to progress class but lowest level is kronbinations level and 
         # treated differently
         self.levels = 0
         self.weight_by_level = []
         self.ind_by_level = []
         self.names = []
         self.bar_format = bar_format
-        self.last_update_time = time.time()
-        self.min_t = 1/max_rate
         
     def init(self, indexes, **kwargs):
         # indexes is a 2d array of indexes, where each row is an index and each column is an iterator
         # Construct a pbar object, and find the total weight  of all indexes to renormalize for the pbar
         # find sum_of_weights = sum([weight of every index]), with weight of an index being the product of the weights of the iterators that make up that index
         weights = []
         for ind in indexes:
@@ -295,36 +296,14 @@
         self.indexes = indexes
         self.len_indexes = len(indexes)
         self.curr_ind = 0 # tracks the current indexes index in indexes
         self.cumm_weight = 0.0
         self.curr_pbar_index = 0
         self.pbar = tqdm(total=self.total, bar_format=self.bar_format)
         
-                
-    def _parallel(self, function, *iterables, num_cpus=None, **kwargs):
-        # Modified version of p_tqdm works with weighted_tqdm generators
-
-        # Determine num_cpus
-        if num_cpus is None:
-            num_cpus = cpu_count()
-        elif type(num_cpus) == float:
-            num_cpus = int(round(num_cpus * cpu_count()))
-
-        # Create parallel generator
-        pool = Pool(num_cpus)
-        for item in self.sub_tqdm(pool.imap(function, *iterables), **kwargs):
-            yield item
-        pool.clear()
-        
-    def p_tqdm(self, function, *iterables, num_cpus=None, **kwargs):
-        """Performs a parallel ordered map with a progress bar."""
-        generator = self._parallel(function, *iterables, num_cpus=num_cpus, **kwargs)
-        result = list(generator)
-        return result
-        
     def sub_tqdm(self, iterable, weights=None, name='', **kwargs):
         how_many = determine_length_of_iterable(iterable, weights, **kwargs)
         self.levels += 1
         my_level = self.levels
         if len(name):
             name += ': '
         self.names.append(name)
@@ -337,14 +316,15 @@
         weight_factor = weight_factor/weight_sum
         weight_vals = [w*weight_factor for w in weight_vals]
         self.weight_by_level.append(weight_vals)
         ind = 0
         self.pbar.set_description(self.names[-1]+' (' +str(ind) + '/' + str(how_many) + ')')
         iterator = iter(iterable)
         yield next(iterator) 
+        destroyed_subcall_last = 0
         for i in range(1, how_many):
             elem = next(iterator)
             if my_level == self.levels: # no sub-call -> update pbar
                 self.cumm_weight += self.weight_by_level[-1][ind]
                 ind += 1
                 new_count = round(self.cumm_weight)
                 diff_count = new_count - self.curr_pbar_index
@@ -373,32 +353,27 @@
         else:
             self.pbar.set_description(self.names[-1]+'(' +str(ind+1) + '/' + str(how_many) + ')')
                 
     def increment(self):
         # increment 
         curr_weight = self.curr_weights[self.curr_ind]
         self.curr_ind += 1
-        new_time = time.time()
-        if new_time - self.last_update_time > self.min_t:
-            self.pbar.set_description('(' +str(self.curr_ind) + '/' + str(self.total_length) + ')')
-            self.last_update_time = new_time
+        #self.pbar.set_description('(' +str(i) + '/' + str(self.len_indexes) + ')')
         if self.levels == 0:
             self.cumm_weight += curr_weight 
             new_index = round(self.cumm_weight)
             diff = new_index - self.curr_pbar_index
             self.curr_pbar_index = new_index
             self.pbar.update(diff)
         else: # reset sublevels
             self.levels = 0
             self.weight_by_level = []
             self.ind_by_level = []
             self.names = []
             
     def close(self):
-        self.pbar.set_description('(' +str(self.curr_ind) + '/' + str(self.total_length) + ')')
-        self.pbar.update(0)
         self.pbar.close()
         
     def all_indexes(self):
         list_of_indexes = [list(np.arange(0, len(l))) for l in list_of_iterators]
         return np.array(list(itertools.product(*list_of_indexes)))
```

### Comparing `weighted_tqdm-0.8/src/weighted_tqdm.egg-info/PKG-INFO` & `weighted_tqdm-0.9/src/weighted_tqdm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: weighted-tqdm
-Version: 0.8
+Version: 0.9
 Summary: weighted_tqdm allows for weighted iterations in tqdm progress bars.
-Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.8.tar.gz
+Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.9.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

