# Comparing `tmp/MEGABYTE-pytorch-0.1.2.tar.gz` & `tmp/MEGABYTE-pytorch-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MEGABYTE-pytorch-0.1.2.tar", last modified: Mon May 29 17:43:05 2023, max compression
+gzip compressed data, was "MEGABYTE-pytorch-0.1.4.tar", last modified: Wed May 31 01:02:21 2023, max compression
```

## Comparing `MEGABYTE-pytorch-0.1.2.tar` & `MEGABYTE-pytorch-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:43:05.468703 MEGABYTE-pytorch-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 17:42:51.000000 MEGABYTE-pytorch-0.1.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:43:05.468703 MEGABYTE-pytorch-0.1.2/MEGABYTE_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 17:42:51.000000 MEGABYTE-pytorch-0.1.2/MEGABYTE_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-29 17:42:51.000000 MEGABYTE-pytorch-0.1.2/MEGABYTE_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    13608 2023-05-29 17:42:51.000000 MEGABYTE-pytorch-0.1.2/MEGABYTE_pytorch/megabyte.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:43:05.468703 MEGABYTE-pytorch-0.1.2/MEGABYTE_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-29 17:43:05.000000 MEGABYTE-pytorch-0.1.2/MEGABYTE_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-29 17:43:05.000000 MEGABYTE-pytorch-0.1.2/MEGABYTE_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:43:05.000000 MEGABYTE-pytorch-0.1.2/MEGABYTE_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-29 17:43:05.000000 MEGABYTE-pytorch-0.1.2/MEGABYTE_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-29 17:43:05.000000 MEGABYTE-pytorch-0.1.2/MEGABYTE_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-29 17:43:05.468703 MEGABYTE-pytorch-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-29 17:42:51.000000 MEGABYTE-pytorch-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:43:05.468703 MEGABYTE-pytorch-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-29 17:42:51.000000 MEGABYTE-pytorch-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:02:21.510444 MEGABYTE-pytorch-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 01:02:10.000000 MEGABYTE-pytorch-0.1.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:02:21.510444 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 01:02:10.000000 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-31 01:02:10.000000 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-05-31 01:02:10.000000 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch/megabyte.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:02:21.510444 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-31 01:02:21.000000 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-31 01:02:21.000000 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 01:02:21.000000 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 01:02:21.000000 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 01:02:21.000000 MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-31 01:02:21.510444 MEGABYTE-pytorch-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-31 01:02:10.000000 MEGABYTE-pytorch-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 01:02:21.510444 MEGABYTE-pytorch-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-31 01:02:10.000000 MEGABYTE-pytorch-0.1.4/setup.py
```

### Comparing `MEGABYTE-pytorch-0.1.2/LICENSE` & `MEGABYTE-pytorch-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.1.2/MEGABYTE_pytorch/attend.py` & `MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.1.2/MEGABYTE_pytorch/megabyte.py` & `MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch/megabyte.py`

 * *Files 2% similar despite different names*

```diff
@@ -393,15 +393,18 @@
 
             prev_stage_tokens_repr = proj(attended[..., :-1, :])
 
         # project to logits
 
         logits = self.to_logits(attended)
 
-        start_tokens, logits = logits[:, 0, :1, :], logits[..., 1:, :]
+        start_tokens = logits[(slice(None), *((0,) * (logits.ndim - 2)), slice(None))]
+        start_tokens = rearrange(start_tokens, 'b d -> b 1 d')
+
+        logits = logits[..., 1:, :]
 
         if not return_loss:
 
             if flattened_dims:
                 logits = rearrange(logits, 'b ... c -> b (...) c')
                 logits = logits[:, :seq_len]
```

### Comparing `MEGABYTE-pytorch-0.1.2/MEGABYTE_pytorch.egg-info/PKG-INFO` & `MEGABYTE-pytorch-0.1.4/MEGABYTE_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.1.2
+Version: 0.1.4
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.1.2/PKG-INFO` & `MEGABYTE-pytorch-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.1.2
+Version: 0.1.4
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.1.2/README.md` & `MEGABYTE-pytorch-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.1.2/setup.py` & `MEGABYTE-pytorch-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'MEGABYTE-pytorch',
   packages = find_packages(),
-  version = '0.1.2',
+  version = '0.1.4',
   license='MIT',
   description = 'MEGABYTE - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/MEGABYTE-pytorch',
   keywords = [
```

