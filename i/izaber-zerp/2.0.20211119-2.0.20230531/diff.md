# Comparing `tmp/izaber-zerp-2.0.20211119.tar.gz` & `tmp/izaber_zerp-2.0.20230531.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izaber-zerp-2.0.20211119.tar", last modified: Sat Nov 20 00:52:40 2021, max compression
+gzip compressed data, was "izaber_zerp-2.0.20230531.tar", max compression
```

## Comparing `izaber-zerp-2.0.20211119.tar` & `izaber_zerp-2.0.20230531.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    30566 2021-11-20 00:33:15.291070 izaber-zerp-2.0.20211119/izaber_zerp/__init__.py
--rw-r--r--   0        0        0    12978 2021-11-20 00:33:15.291070 izaber-zerp-2.0.20211119/izaber_zerp/crm.py
--rw-r--r--   0        0        0     2872 2021-11-20 00:33:15.291070 izaber-zerp-2.0.20211119/izaber_zerp/gui.py
--rw-r--r--   0        0        0     2919 2021-11-20 00:33:15.291070 izaber-zerp-2.0.20211119/izaber_zerp/product.py
--rw-r--r--   0        0        0    24758 2021-11-20 00:33:15.291070 izaber-zerp-2.0.20211119/izaber_zerp/timesheet.py
--rw-r--r--   0        0        0      477 2021-11-20 00:52:22.147604 izaber-zerp-2.0.20211119/pyproject.toml
--rw-r--r--   0        0        0      640 2021-11-20 00:52:40.528361 izaber-zerp-2.0.20211119/setup.py
--rw-r--r--   0        0        0      499 2021-11-20 00:52:40.528678 izaber-zerp-2.0.20211119/PKG-INFO
+-rw-r--r--   0        0        0    30570 2023-05-31 18:50:52.624235 izaber_zerp-2.0.20230531/izaber_zerp/__init__.py
+-rw-r--r--   0        0        0    12979 2023-05-31 19:09:18.529761 izaber_zerp-2.0.20230531/izaber_zerp/crm.py
+-rw-r--r--   0        0        0     2873 2023-05-31 19:09:48.557769 izaber_zerp-2.0.20230531/izaber_zerp/gui.py
+-rw-r--r--   0        0        0     2914 2023-05-31 19:04:37.162002 izaber_zerp-2.0.20230531/izaber_zerp/product.py
+-rw-r--r--   0        0        0    24758 2022-04-26 19:22:18.819068 izaber_zerp-2.0.20230531/izaber_zerp/timesheet.py
+-rw-r--r--   0        0        0      477 2023-05-31 19:48:05.503266 izaber_zerp-2.0.20230531/pyproject.toml
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 izaber_zerp-2.0.20230531/setup.py
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 izaber_zerp-2.0.20230531/PKG-INFO
```

### Comparing `izaber-zerp-2.0.20211119/izaber_zerp/__init__.py` & `izaber_zerp-2.0.20230531/izaber_zerp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             date objects, they get turned into the string format
             Zerp expects
         """
         filtered_constraints = []
         for constraint in constraints:
             try:
                 key, op, value = constraint
-                if isinstance(value, collections.Iterable):
+                if isinstance(value, collections.abc.Iterable):
                     if not isinstance(value, str):
                         value = [self.data_normalize(v) for v in value]
                 else:
                     value = self.data_normalize(value)
                 filtered_constraints.append((key, op, value))
             except ValueError:
                 # catch elements of constraint list that are boolean
```

### Comparing `izaber-zerp-2.0.20211119/izaber_zerp/crm.py` & `izaber_zerp-2.0.20230531/izaber_zerp/crm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import absolute_import
 from __future__ import print_function
-from zaber.zerp import *
+from izaber.zerp import *
 import operator
 import sys
 import six
 from six.moves import range
 
 
 try:
```

### Comparing `izaber-zerp-2.0.20211119/izaber_zerp/gui.py` & `izaber_zerp-2.0.20230531/izaber_zerp/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import absolute_import
-from zaber.zerp import *
+from izaber.zerp import *
 
 class ZerpMenuItem(ZerpRecord):
   def execute(self,*args,**kwargs):
     """ Attempt to execute this menu item
     """
     try:
       action = self.action
```

### Comparing `izaber-zerp-2.0.20211119/izaber_zerp/product.py` & `izaber_zerp-2.0.20230531/izaber_zerp/product.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import absolute_import
 import pickle 
 
-from zaber.zerp import *
+from izaber.zerp import *
 import six
 
 STATE_PREFERENCES = {
     'sellable': 1,
     'end': 2,
     'draft': 3,
     'obsolete': 4,
 }
 
-def product_sort(a,b):
-    result = cmp(STATE_PREFERENCES[a['state']], STATE_PREFERENCES[b['state']])
-    if result: return result
-    return cmp(a['revision'], b['revision'])
+def product_sort(item):
+    state_preference = STATE_PREFERENCES.get(item['state']) or 4
+    revision = item.get('revision') or 0
+    return (state_preference, revision)
 
 class ZerpProducts(Zerp):
 
     def __init__(self,*args,**kwargs):
         self._product_name_cache = {}
         super(ZerpProducts,self).__init__(*args,**kwargs)
 
@@ -46,15 +46,15 @@
                 new_product_name_cache.setdefault(partnumber,[]).append({
                     'product_id': prod.id,
                     'state': prod.state,
                     'revision': prod.revision
                   })
 
             for partnumber, parts in six.iteritems(new_product_name_cache.copy()):
-                parts.sort(cmp=product_sort)
+                parts.sort(key=product_sort)
                 new_product_name_cache[partnumber] = parts[0]['product_id']
             self._product_name_cache[state_filter_key] = new_product_name_cache
 
         # Then we try our best to match the partnumber to the subproducts
         # FIXME: Does this algo handle partials?
         segs = product_name.split('-')
         result = []
```

### Comparing `izaber-zerp-2.0.20211119/izaber_zerp/timesheet.py` & `izaber_zerp-2.0.20230531/izaber_zerp/timesheet.py`

 * *Files identical despite different names*

### Comparing `izaber-zerp-2.0.20211119/setup.py` & `izaber_zerp-2.0.20230531/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['izaber>=2.20210919', 'pytz>=2014.4']
 
 setup_kwargs = {
     'name': 'izaber-zerp',
-    'version': '2.0.20211119',
+    'version': '2.0.20230531',
     'description': 'Old style izaber.zerp connectivity',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'Aki Mimoto',
     'author_email': 'aki@zaber.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.6.0,<4.0',
+    'python_requires': '>=3.7.0,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

