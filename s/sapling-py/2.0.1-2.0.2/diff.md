# Comparing `tmp/sapling-py-2.0.1.tar.gz` & `tmp/sapling-py-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapling-py-2.0.1.tar", last modified: Thu Mar 30 07:48:55 2023, max compression
+gzip compressed data, was "sapling-py-2.0.2.tar", last modified: Wed May 31 04:31:40 2023, max compression
```

## Comparing `sapling-py-2.0.1.tar` & `sapling-py-2.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 james      (502) staff       (20)        0 2023-03-30 07:48:55.119865 sapling-py-2.0.1/
--rw-r--r--   0 james      (502) staff       (20)    11357 2022-11-10 06:53:31.000000 sapling-py-2.0.1/LICENSE
--rw-r--r--   0 james      (502) staff       (20)     3321 2023-03-30 07:48:55.119743 sapling-py-2.0.1/PKG-INFO
--rw-r--r--   0 james      (502) staff       (20)     2964 2022-11-10 06:53:31.000000 sapling-py-2.0.1/README.md
-drwxr-xr-x   0 james      (502) staff       (20)        0 2023-03-30 07:48:55.118876 sapling-py-2.0.1/sapling/
--rw-r--r--   0 james      (502) staff       (20)      130 2023-03-30 07:18:05.000000 sapling-py-2.0.1/sapling/__init__.py
--rw-r--r--   0 james      (502) staff       (20)    12140 2023-03-30 07:18:06.000000 sapling-py-2.0.1/sapling/client.py
--rw-r--r--   0 james      (502) staff       (20)       22 2023-03-30 07:48:45.000000 sapling-py-2.0.1/sapling/version.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2023-03-30 07:48:55.119491 sapling-py-2.0.1/sapling_py.egg-info/
--rw-r--r--   0 james      (502) staff       (20)     3321 2023-03-30 07:48:55.000000 sapling-py-2.0.1/sapling_py.egg-info/PKG-INFO
--rw-r--r--   0 james      (502) staff       (20)      269 2023-03-30 07:48:55.000000 sapling-py-2.0.1/sapling_py.egg-info/SOURCES.txt
--rw-r--r--   0 james      (502) staff       (20)        1 2023-03-30 07:48:55.000000 sapling-py-2.0.1/sapling_py.egg-info/dependency_links.txt
--rw-r--r--   0 james      (502) staff       (20)        9 2023-03-30 07:48:55.000000 sapling-py-2.0.1/sapling_py.egg-info/requires.txt
--rw-r--r--   0 james      (502) staff       (20)       13 2023-03-30 07:48:55.000000 sapling-py-2.0.1/sapling_py.egg-info/top_level.txt
--rw-r--r--   0 james      (502) staff       (20)       38 2023-03-30 07:48:55.119918 sapling-py-2.0.1/setup.cfg
--rw-r--r--   0 james      (502) staff       (20)      948 2023-03-30 07:17:57.000000 sapling-py-2.0.1/setup.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2023-03-30 07:48:55.119608 sapling-py-2.0.1/test/
--rw-r--r--   0 james      (502) staff       (20)        0 2022-11-10 06:53:31.000000 sapling-py-2.0.1/test/__init__.py
+drwxr-xr-x   0 james      (502) staff       (20)        0 2023-05-31 04:31:40.649584 sapling-py-2.0.2/
+-rw-r--r--   0 james      (502) staff       (20)    11357 2022-11-10 06:53:31.000000 sapling-py-2.0.2/LICENSE
+-rw-r--r--   0 james      (502) staff       (20)     3321 2023-05-31 04:31:40.649453 sapling-py-2.0.2/PKG-INFO
+-rw-r--r--   0 james      (502) staff       (20)     2964 2022-11-10 06:53:31.000000 sapling-py-2.0.2/README.md
+drwxr-xr-x   0 james      (502) staff       (20)        0 2023-05-31 04:31:40.648646 sapling-py-2.0.2/sapling/
+-rw-r--r--   0 james      (502) staff       (20)      130 2023-03-30 07:18:05.000000 sapling-py-2.0.2/sapling/__init__.py
+-rw-r--r--   0 james      (502) staff       (20)    12946 2023-05-31 04:27:08.000000 sapling-py-2.0.2/sapling/client.py
+-rw-r--r--   0 james      (502) staff       (20)       22 2023-05-31 04:27:23.000000 sapling-py-2.0.2/sapling/version.py
+drwxr-xr-x   0 james      (502) staff       (20)        0 2023-05-31 04:31:40.649187 sapling-py-2.0.2/sapling_py.egg-info/
+-rw-r--r--   0 james      (502) staff       (20)     3321 2023-05-31 04:31:40.000000 sapling-py-2.0.2/sapling_py.egg-info/PKG-INFO
+-rw-r--r--   0 james      (502) staff       (20)      269 2023-05-31 04:31:40.000000 sapling-py-2.0.2/sapling_py.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (502) staff       (20)        1 2023-05-31 04:31:40.000000 sapling-py-2.0.2/sapling_py.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (502) staff       (20)        9 2023-05-31 04:31:40.000000 sapling-py-2.0.2/sapling_py.egg-info/requires.txt
+-rw-r--r--   0 james      (502) staff       (20)       13 2023-05-31 04:31:40.000000 sapling-py-2.0.2/sapling_py.egg-info/top_level.txt
+-rw-r--r--   0 james      (502) staff       (20)       38 2023-05-31 04:31:40.649622 sapling-py-2.0.2/setup.cfg
+-rw-r--r--   0 james      (502) staff       (20)      948 2023-03-30 07:17:57.000000 sapling-py-2.0.2/setup.py
+drwxr-xr-x   0 james      (502) staff       (20)        0 2023-05-31 04:31:40.649315 sapling-py-2.0.2/test/
+-rw-r--r--   0 james      (502) staff       (20)        0 2022-11-10 06:53:31.000000 sapling-py-2.0.2/test/__init__.py
```

### Comparing `sapling-py-2.0.1/LICENSE` & `sapling-py-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sapling-py-2.0.1/PKG-INFO` & `sapling-py-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapling-py
-Version: 2.0.1
+Version: 2.0.2
 Summary: Sapling Python Client
 Home-page: https://sapling.ai
 Author: Sapling Intelligence
 Author-email: info@sapling.ai
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sapling-py-2.0.1/README.md` & `sapling-py-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sapling-py-2.0.1/sapling/client.py` & `sapling-py-2.0.2/sapling/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -349,7 +349,36 @@
             url,
             json=data,
             timeout=self.timeout,
         )
         if 200 <= resp.status_code < 300:
             return
         raise Exception(f'HTTP {resp.status_code}: resp.text')
+
+    def aidetect(
+        self,
+        text,
+        sent_scores=None,
+    ):
+        '''
+        Score a piece of text on how likely it was generated by AI.
+
+        :param text: Text to
+        :type text: str
+        :param sent_scores: If true, each sentence will also be scored individually.
+        :type sent_scores: bool
+        '''
+        url = f'{self.url_endpoint}aidetect'
+        data = {
+            'key': self.api_key,
+            'text': text,
+        }
+        if sent_scores is not None:
+            data['sent_scores'] = sent_scores
+        resp = requests.post(
+            url,
+            json=data,
+            timeout=self.timeout,
+        )
+        if 200 <= resp.status_code < 300:
+            return resp.json()
+        raise Exception(f'HTTP {resp.status_code}: resp.text')
```

### Comparing `sapling-py-2.0.1/sapling_py.egg-info/PKG-INFO` & `sapling-py-2.0.2/sapling_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapling-py
-Version: 2.0.1
+Version: 2.0.2
 Summary: Sapling Python Client
 Home-page: https://sapling.ai
 Author: Sapling Intelligence
 Author-email: info@sapling.ai
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sapling-py-2.0.1/setup.py` & `sapling-py-2.0.2/setup.py`

 * *Files identical despite different names*

