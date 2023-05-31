# Comparing `tmp/pywencai-0.8.7.tar.gz` & `tmp/pywencai-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywencai-0.8.7.tar", max compression
+gzip compressed data, was "pywencai-0.8.8.tar", max compression
```

## Comparing `pywencai-0.8.7.tar` & `pywencai-0.8.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-05-30 16:15:26.783706 pywencai-0.8.7/LICENSE
--rw-r--r--   0        0        0     3043 2023-05-30 16:15:26.783706 pywencai-0.8.7/README.md
--rw-r--r--   0        0        0      612 2023-05-30 16:15:26.787706 pywencai-0.8.7/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-30 16:15:26.787706 pywencai-0.8.7/pywencai/__init__.py
--rw-r--r--   0        0        0     4816 2023-05-30 16:15:26.787706 pywencai-0.8.7/pywencai/convert.py
--rw-r--r--   0        0        0      433 2023-05-30 16:15:26.787706 pywencai-0.8.7/pywencai/headers.py
--rw-r--r--   0        0        0    39677 2023-05-30 16:15:26.787706 pywencai-0.8.7/pywencai/hexin-v.js
--rw-r--r--   0        0        0     4303 2023-05-30 16:15:26.787706 pywencai-0.8.7/pywencai/wencai.py
--rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 pywencai-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-31 15:55:01.769338 pywencai-0.8.8/LICENSE
+-rw-r--r--   0        0        0     3043 2023-05-31 15:55:01.769338 pywencai-0.8.8/README.md
+-rw-r--r--   0        0        0      612 2023-05-31 15:55:01.769338 pywencai-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-31 15:55:01.769338 pywencai-0.8.8/pywencai/__init__.py
+-rw-r--r--   0        0        0     5294 2023-05-31 15:55:01.769338 pywencai-0.8.8/pywencai/convert.py
+-rw-r--r--   0        0        0      433 2023-05-31 15:55:01.769338 pywencai-0.8.8/pywencai/headers.py
+-rw-r--r--   0        0        0    39677 2023-05-31 15:55:01.769338 pywencai-0.8.8/pywencai/hexin-v.js
+-rw-r--r--   0        0        0     4303 2023-05-31 15:55:01.769338 pywencai-0.8.8/pywencai/wencai.py
+-rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 pywencai-0.8.8/PKG-INFO
```

### Comparing `pywencai-0.8.7/LICENSE` & `pywencai-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.7/README.md` & `pywencai-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.7/pyproject.toml` & `pywencai-0.8.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pywencai"
-version = "0.8.7"
+version = "0.8.8"
 description = ""
 authors = ["pluto <mayuanchi1029@gmail.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
```

### Comparing `pywencai-0.8.7/pywencai/convert.py` & `pywencai-0.8.8/pywencai/convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 import pandas as pd
 import json
 import pydash as _
 import requests as rq
 from pywencai.headers import headers
 
+def get_url(url):
+    res = rq.request(
+        method='GET',
+        url=f'http://www.iwencai.com{url}',
+        headers=headers()
+    )
+    result = json.loads(res.text)
+    return result.get('data')
+
 def xuangu_tableV1_handler(comp, comps):
     '''xuangu_tableV1类型'''
     return {
         'condition': _.get(comp, 'data.meta.extra.condition'),
         'comp_id': comp['cid'],
         'uuid': comp['puuid']
     }
 
 def common_handler(comp, comps):
     '''common类型'''
     datas = _.get(comp, 'data.datas')
     if isinstance(datas, list):
         return pd.DataFrame.from_dict(datas)
     else:
-        return None
+        return _.get(comp, 'data')
 
 def container_handler(comp, comps):
     '''container类型'''
     result = {}
     for uuid in _.get(comp, 'config.children', []):
         child = _.find(comps, lambda c: c.get('uuid') == uuid)
         key = _.get(child, 'show_type')
         if key is not None and key != '':
             result[key] = show_type_handler(child, comps)
     return result
 
-def txt1_handler(comp, comps):
-    '''txt1类型'''
+def txt_handler(comp, comps):
+    '''txt类型'''
     content = _.get(comp, 'data.content')
     return content
 
 def tab4_handler(comp, comps):
     '''tab4类型'''
     result = {}
     for tab in comp.get('tab_list'):
@@ -74,50 +83,52 @@
     if detail is not None:
         result['detail'] = {
             'buy': pd.DataFrame.from_dict(_.get(detail[0], 'buy.datas')),
             'sell': pd.DataFrame.from_dict(_.get(detail[0], 'sell.datas'))
         }
     return result
 
-def table2_handler(comp, comps):
-    data = _.get(comp, 'data')
-    return pd.DataFrame.from_dict(data)
-
-def textblocklinkone_handler(comp, comps):
-    data = _.get(comp, 'data.result.data')
-    return pd.DataFrame.from_dict(data)
-
 def wiki1_handler(comp, comps):
     url = _.get(comp, 'data.url')
     if url is not None:
-        res = rq.request(
-            method='GET',
-            url=f'http://www.iwencai.com{url}',
-            headers=headers()
-        )
-        result = json.loads(res.text)
-        wcomp = result.get('data')
+        wcomp = get_url(url)
         if wcomp is not None:
             return show_type_handler(wcomp, comps)
         else:
-            return {}
-    return {}
+            return None
+    return None
+
+def textblocklinkone_handler(comp, comps):
+    data = _.get(comp, 'data.result.data')
+    return pd.DataFrame.from_dict(data)
+
+def nestedblocks_handler(comp, comps):
+    '''股东户数分析'''
+    subBlocks = _.get(comp, 'data.result.subBlocks.0.subBlocks')
+    result = []
+    for sub in subBlocks:
+        url = sub.get('url')
+        sub_comp = get_url(url)
+        if sub_comp is not None:
+            result.append(show_type_handler(sub_comp, comps))
+    return result
+
 
 
 
 show_type_handler_dict = {
-    'xuangu_tableV1': xuangu_tableV1_handler,
     'container': container_handler,
-    'txt1': txt1_handler,
+    'txt1': txt_handler,
+    'txt2': txt_handler,
     'tab4': tab4_handler,
     'dragon_tiger_stock': dragon_tiger_stock_handler,
-    'table2': table2_handler,
     'tab1': tab1_handler,
     'wiki1': wiki1_handler,
-    'textblocklinkone': textblocklinkone_handler
+    'textblocklinkone': textblocklinkone_handler,
+    'nestedblocks': nestedblocks_handler
 }
 
 def show_type_handler(comp, comps):
     '''处理每种不同的show_type类型'''
     show_type = comp.get('show_type')
     handler = show_type_handler_dict.get(show_type)
     if handler is not None:
@@ -148,15 +159,21 @@
     content = _.get(result, 'data.answer.0.txt.0.content')
     if type(content) == str:
         content = json.loads(content)
     components = content['components'] 
     params = {}
     if len(components) == 1:
         components0 = components[0]
-        params = {
-            'data': show_type_handler(components0, components)
-        } 
+        if (components0.get('show_type') == 'xuangu_tableV1'):
+            params = {
+                'data': xuangu_tableV1_handler(components0, components)
+            }
+        else:
+            params = {
+                'data': show_type_handler(components0, components)
+            }
+        
     else:
         params = {
             'data': multi_show_type_handler(components)
         }
     return params
```

### Comparing `pywencai-0.8.7/pywencai/hexin-v.js` & `pywencai-0.8.8/pywencai/hexin-v.js`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.7/pywencai/wencai.py` & `pywencai-0.8.8/pywencai/wencai.py`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.7/PKG-INFO` & `pywencai-0.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywencai
-Version: 0.8.7
+Version: 0.8.8
 Summary: 
 Author: pluto
 Author-email: mayuanchi1029@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

