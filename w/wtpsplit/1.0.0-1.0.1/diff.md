# Comparing `tmp/wtpsplit-1.0.0.tar.gz` & `tmp/wtpsplit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/benjamin_cohere_com/nnsplit/dist/.tmp-zok0ai0c/wtpsplit-1.0.0.tar", last modified: Wed May 31 10:52:16 2023, max compression
+gzip compressed data, was "/home/benjamin_cohere_com/nnsplit/dist/.tmp-lfgwvf1a/wtpsplit-1.0.1.tar", last modified: Wed May 31 11:17:38 2023, max compression
```

## Comparing `wtpsplit-1.0.0.tar` & `wtpsplit-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-05-31 10:52:16.196569 wtpsplit-1.0.0/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      246 2023-05-31 10:52:16.196569 wtpsplit-1.0.0/PKG-INFO
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    10223 2023-05-31 10:50:58.000000 wtpsplit-1.0.0/README.md
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)       73 2023-05-31 08:05:00.000000 wtpsplit-1.0.0/pyproject.toml
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)       97 2023-05-31 10:52:16.196569 wtpsplit-1.0.0/setup.cfg
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      493 2023-05-31 10:51:22.000000 wtpsplit-1.0.0/setup.py
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-05-31 10:52:16.196569 wtpsplit-1.0.0/wtpsplit/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    13429 2023-05-31 10:39:24.000000 wtpsplit-1.0.0/wtpsplit/__init__.py
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-05-31 10:52:16.196569 wtpsplit-1.0.0/wtpsplit/data/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     3434 2023-05-31 08:05:00.000000 wtpsplit-1.0.0/wtpsplit/data/language_info.csv
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    38208 2023-05-31 08:05:00.000000 wtpsplit-1.0.0/wtpsplit/data/punctuation.json
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      408 2023-05-31 08:05:00.000000 wtpsplit-1.0.0/wtpsplit/data/punctuation.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     7560 2023-05-31 10:39:32.000000 wtpsplit-1.0.0/wtpsplit/extract.py
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    40289 2023-05-31 08:05:00.000000 wtpsplit-1.0.0/wtpsplit/models.py
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     5814 2023-05-31 08:05:00.000000 wtpsplit-1.0.0/wtpsplit/utils.py
-drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-05-31 10:52:16.196569 wtpsplit-1.0.0/wtpsplit.egg-info/
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      246 2023-05-31 10:52:16.000000 wtpsplit-1.0.0/wtpsplit.egg-info/PKG-INFO
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      373 2023-05-31 10:52:16.000000 wtpsplit-1.0.0/wtpsplit.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        1 2023-05-31 10:52:16.000000 wtpsplit-1.0.0/wtpsplit.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)       49 2023-05-31 10:52:16.000000 wtpsplit-1.0.0/wtpsplit.egg-info/requires.txt
--rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        9 2023-05-31 10:52:16.000000 wtpsplit-1.0.0/wtpsplit.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-05-31 11:17:38.847082 wtpsplit-1.0.1/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      246 2023-05-31 11:17:38.847082 wtpsplit-1.0.1/PKG-INFO
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    10223 2023-05-31 11:16:52.000000 wtpsplit-1.0.1/README.md
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)       73 2023-05-31 11:16:52.000000 wtpsplit-1.0.1/pyproject.toml
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)       97 2023-05-31 11:17:38.847082 wtpsplit-1.0.1/setup.cfg
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      494 2023-05-31 11:17:06.000000 wtpsplit-1.0.1/setup.py
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-05-31 11:17:38.843082 wtpsplit-1.0.1/wtpsplit/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    13654 2023-05-31 11:16:57.000000 wtpsplit-1.0.1/wtpsplit/__init__.py
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-05-31 11:17:38.847082 wtpsplit-1.0.1/wtpsplit/data/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     3434 2023-05-31 11:16:52.000000 wtpsplit-1.0.1/wtpsplit/data/language_info.csv
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    38208 2023-05-31 11:16:52.000000 wtpsplit-1.0.1/wtpsplit/data/punctuation.json
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      408 2023-05-31 11:16:52.000000 wtpsplit-1.0.1/wtpsplit/data/punctuation.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     7560 2023-05-31 11:16:52.000000 wtpsplit-1.0.1/wtpsplit/extract.py
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)    40289 2023-05-31 11:16:52.000000 wtpsplit-1.0.1/wtpsplit/models.py
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)     5814 2023-05-31 11:16:52.000000 wtpsplit-1.0.1/wtpsplit/utils.py
+drwxr-xr-x   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        0 2023-05-31 11:17:38.843082 wtpsplit-1.0.1/wtpsplit.egg-info/
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      246 2023-05-31 11:17:38.000000 wtpsplit-1.0.1/wtpsplit.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)      373 2023-05-31 11:17:38.000000 wtpsplit-1.0.1/wtpsplit.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        1 2023-05-31 11:17:38.000000 wtpsplit-1.0.1/wtpsplit.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)       49 2023-05-31 11:17:38.000000 wtpsplit-1.0.1/wtpsplit.egg-info/requires.txt
+-rw-r--r--   0 benjamin_cohere_com (271073365) benjamin_cohere_com (271073365)        9 2023-05-31 11:17:38.000000 wtpsplit-1.0.1/wtpsplit.egg-info/top_level.txt
```

### Comparing `wtpsplit-1.0.0/README.md` & `wtpsplit-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.0.0/wtpsplit/__init__.py` & `wtpsplit-1.0.1/wtpsplit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 from transformers import AutoModelForTokenClassification
 from transformers.utils.hub import cached_file
 import skops.io as sio
 
 from wtpsplit.extract import extract
 from wtpsplit.utils import Constants, encode, indices_to_sentences
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
+
 
 class ORTWrapper:
     def __init__(self, model, ort_session):
         self.model = model
         self.ort_session = ort_session
 
     @property
@@ -43,15 +44,23 @@
             },
         )[0]
 
         return {"logits": torch.from_numpy(logits).to(self.model.device)}
 
 
 class WtP:
-    def __init__(self, model_name_or_model, ort_providers=None, ort_kwargs=None, mixtures=None, hub_prefix="benjamin"):
+    def __init__(
+        self,
+        model_name_or_model,
+        from_pretrained_kwargs=None,
+        ort_providers=None,
+        ort_kwargs=None,
+        mixtures=None,
+        hub_prefix="benjamin",
+    ):
         self.model_name_or_model = model_name_or_model
         self.ort_providers = ort_providers
         self.ort_kwargs = ort_kwargs
 
         mixture_path = None
 
         if isinstance(model_name_or_model, (str, Path)):
@@ -59,30 +68,32 @@
             is_local = os.path.isdir(model_name_or_model)
 
             if not is_local and hub_prefix is not None:
                 model_name_to_fetch = f"{hub_prefix}/{model_name_or_model}"
             else:
                 model_name_to_fetch = model_name_or_model
 
-            model = AutoModelForTokenClassification.from_pretrained(model_name_to_fetch)
+            model = AutoModelForTokenClassification.from_pretrained(
+                model_name_to_fetch, **(from_pretrained_kwargs or {})
+            )
 
             if is_local:
                 model_path = Path(model_name_or_model)
                 mixture_path = model_path / "mixture.skops"
                 if not mixture_path.exists():
                     mixture_path = None
                 onnx_path = model_path / "model.onnx"
                 if not onnx_path.exists():
                     onnx_path = None
             else:
-                mixture_path = cached_file(model_name_to_fetch, "mixtures.skops")
+                mixture_path = cached_file(model_name_to_fetch, "mixtures.skops", **(from_pretrained_kwargs or {}))
 
                 # no need to load if no ort_providers set
                 if ort_providers is not None:
-                    onnx_path = cached_file(model_name_to_fetch, "model.onnx")
+                    onnx_path = cached_file(model_name_to_fetch, "model.onnx", **(from_pretrained_kwargs or {}))
                 else:
                     onnx_path = None
 
             if ort_providers is not None:
                 if onnx_path is None:
                     raise ValueError(
                         "Could not find an ONNX model in the model directory. Try `use_ort=False` to run with PyTorch."
```

### Comparing `wtpsplit-1.0.0/wtpsplit/data/language_info.csv` & `wtpsplit-1.0.1/wtpsplit/data/language_info.csv`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.0.0/wtpsplit/data/punctuation.json` & `wtpsplit-1.0.1/wtpsplit/data/punctuation.json`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.0.0/wtpsplit/extract.py` & `wtpsplit-1.0.1/wtpsplit/extract.py`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.0.0/wtpsplit/models.py` & `wtpsplit-1.0.1/wtpsplit/models.py`

 * *Files identical despite different names*

### Comparing `wtpsplit-1.0.0/wtpsplit/utils.py` & `wtpsplit-1.0.1/wtpsplit/utils.py`

 * *Files identical despite different names*

