# Comparing `tmp/thsquant-0.2.4.tar.gz` & `tmp/thsquant-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thsquant-0.2.4.tar", last modified: Wed May 31 02:42:25 2023, max compression
+gzip compressed data, was "thsquant-0.2.5.tar", last modified: Wed May 31 02:44:54 2023, max compression
```

## Comparing `thsquant-0.2.4.tar` & `thsquant-0.2.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 02:42:25.615874 thsquant-0.2.4/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    11357 2023-05-30 02:01:43.000000 thsquant-0.2.4/LICENSE.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      747 2023-05-31 02:42:25.615874 thsquant-0.2.4/PKG-INFO
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       18 2023-05-30 02:01:43.000000 thsquant-0.2.4/README.md
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       38 2023-05-31 02:42:25.615874 thsquant-0.2.4/setup.cfg
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     1357 2023-05-31 02:42:00.000000 thsquant-0.2.4/setup.py
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 02:42:25.615874 thsquant-0.2.4/thsquant/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        0 2023-05-30 02:01:43.000000 thsquant-0.2.4/thsquant/__init__.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     1112 2023-05-30 02:02:36.000000 thsquant-0.2.4/thsquant/convert_llama_weights_to_hf.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     7704 2023-05-31 02:41:51.000000 thsquant-0.2.4/thsquant/gptq.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    19641 2023-05-31 02:24:25.000000 thsquant-0.2.4/thsquant/llama.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     4629 2023-05-30 02:27:44.000000 thsquant-0.2.4/thsquant/llama_inference.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    13161 2023-05-30 02:02:36.000000 thsquant-0.2.4/thsquant/llama_inference_offload.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    15967 2023-05-30 02:02:36.000000 thsquant-0.2.4/thsquant/neox.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    17497 2023-05-30 02:02:36.000000 thsquant-0.2.4/thsquant/opt.py
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 02:42:25.615874 thsquant-0.2.4/thsquant/quant/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      317 2023-05-30 02:02:36.000000 thsquant-0.2.4/thsquant/quant/__init__.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     8775 2023-05-30 02:02:36.000000 thsquant-0.2.4/thsquant/quant/custom_autotune.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     8799 2023-05-30 02:02:36.000000 thsquant-0.2.4/thsquant/quant/fused_attn.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    12139 2023-05-30 02:02:36.000000 thsquant-0.2.4/thsquant/quant/fused_mlp.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    18730 2023-05-30 02:02:36.000000 thsquant-0.2.4/thsquant/quant/quant_linear.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     4263 2023-05-30 02:02:36.000000 thsquant-0.2.4/thsquant/quant/quantizer.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     3120 2023-05-30 02:02:36.000000 thsquant-0.2.4/thsquant/quant/triton_norm.py
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 02:42:25.615874 thsquant-0.2.4/thsquant/utils/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      215 2023-05-30 02:02:36.000000 thsquant-0.2.4/thsquant/utils/__init__.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     6712 2023-05-30 02:02:36.000000 thsquant-0.2.4/thsquant/utils/datautils.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     1019 2023-05-30 02:02:36.000000 thsquant-0.2.4/thsquant/utils/export.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     2563 2023-05-30 02:02:36.000000 thsquant-0.2.4/thsquant/utils/modelutils.py
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 02:42:25.615874 thsquant-0.2.4/thsquant.egg-info/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      747 2023-05-31 02:42:25.000000 thsquant-0.2.4/thsquant.egg-info/PKG-INFO
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      733 2023-05-31 02:42:25.000000 thsquant-0.2.4/thsquant.egg-info/SOURCES.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       69 2023-05-31 02:42:25.000000 thsquant-0.2.4/thsquant.egg-info/dependency_links.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       62 2023-05-31 02:42:25.000000 thsquant-0.2.4/thsquant.egg-info/entry_points.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      126 2023-05-31 02:42:25.000000 thsquant-0.2.4/thsquant.egg-info/requires.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        9 2023-05-31 02:42:25.000000 thsquant-0.2.4/thsquant.egg-info/top_level.txt
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 02:44:54.315732 thsquant-0.2.5/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    11357 2023-05-30 02:01:43.000000 thsquant-0.2.5/LICENSE.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      747 2023-05-31 02:44:54.315732 thsquant-0.2.5/PKG-INFO
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       18 2023-05-30 02:01:43.000000 thsquant-0.2.5/README.md
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       38 2023-05-31 02:44:54.315732 thsquant-0.2.5/setup.cfg
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     1357 2023-05-31 02:44:43.000000 thsquant-0.2.5/setup.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 02:44:54.315732 thsquant-0.2.5/thsquant/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        0 2023-05-30 02:01:43.000000 thsquant-0.2.5/thsquant/__init__.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     1112 2023-05-30 02:02:36.000000 thsquant-0.2.5/thsquant/convert_llama_weights_to_hf.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     7713 2023-05-31 02:44:02.000000 thsquant-0.2.5/thsquant/gptq.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    19641 2023-05-31 02:24:25.000000 thsquant-0.2.5/thsquant/llama.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     4629 2023-05-30 02:27:44.000000 thsquant-0.2.5/thsquant/llama_inference.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    13161 2023-05-30 02:02:36.000000 thsquant-0.2.5/thsquant/llama_inference_offload.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    15967 2023-05-30 02:02:36.000000 thsquant-0.2.5/thsquant/neox.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    17497 2023-05-30 02:02:36.000000 thsquant-0.2.5/thsquant/opt.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 02:44:54.315732 thsquant-0.2.5/thsquant/quant/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      317 2023-05-30 02:02:36.000000 thsquant-0.2.5/thsquant/quant/__init__.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     8775 2023-05-30 02:02:36.000000 thsquant-0.2.5/thsquant/quant/custom_autotune.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     8799 2023-05-30 02:02:36.000000 thsquant-0.2.5/thsquant/quant/fused_attn.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    12139 2023-05-30 02:02:36.000000 thsquant-0.2.5/thsquant/quant/fused_mlp.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    18730 2023-05-30 02:02:36.000000 thsquant-0.2.5/thsquant/quant/quant_linear.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     4263 2023-05-30 02:02:36.000000 thsquant-0.2.5/thsquant/quant/quantizer.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     3120 2023-05-30 02:02:36.000000 thsquant-0.2.5/thsquant/quant/triton_norm.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 02:44:54.315732 thsquant-0.2.5/thsquant/utils/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      215 2023-05-30 02:02:36.000000 thsquant-0.2.5/thsquant/utils/__init__.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     6712 2023-05-30 02:02:36.000000 thsquant-0.2.5/thsquant/utils/datautils.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     1019 2023-05-30 02:02:36.000000 thsquant-0.2.5/thsquant/utils/export.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     2563 2023-05-30 02:02:36.000000 thsquant-0.2.5/thsquant/utils/modelutils.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 02:44:54.315732 thsquant-0.2.5/thsquant.egg-info/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      747 2023-05-31 02:44:53.000000 thsquant-0.2.5/thsquant.egg-info/PKG-INFO
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      733 2023-05-31 02:44:54.000000 thsquant-0.2.5/thsquant.egg-info/SOURCES.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       69 2023-05-31 02:44:53.000000 thsquant-0.2.5/thsquant.egg-info/dependency_links.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       62 2023-05-31 02:44:54.000000 thsquant-0.2.5/thsquant.egg-info/entry_points.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      126 2023-05-31 02:44:54.000000 thsquant-0.2.5/thsquant.egg-info/requires.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        9 2023-05-31 02:44:54.000000 thsquant-0.2.5/thsquant.egg-info/top_level.txt
```

### Comparing `thsquant-0.2.4/LICENSE.txt` & `thsquant-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.4/PKG-INFO` & `thsquant-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thsquant
-Version: 0.2.4
+Version: 0.2.5
 Summary: A short description of your awesome package
 Home-page: https://github.com/qinbo23/ths-quant
 Author: qinbo
 Author-email: qinbo@myhexin.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `thsquant-0.2.4/setup.py` & `thsquant-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="thsquant",
-    version="0.2.4",
+    version="0.2.5",
     packages=find_packages(),
     install_requires=[
         'safetensors==0.3.0',
         'datasets==2.10.1',
         'sentencepiece',
         'accelerate==0.17.1',
         'triton==2.0.0',
```

### Comparing `thsquant-0.2.4/thsquant/convert_llama_weights_to_hf.py` & `thsquant-0.2.5/thsquant/convert_llama_weights_to_hf.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.4/thsquant/gptq.py` & `thsquant-0.2.5/thsquant/gptq.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 
 import torch
 import torch.nn as nn
 import transformers
 import thsquant.quant
 from texttable import Texttable
-from utils import torch_snr_error
+from thsquant.utils import torch_snr_error
 
 torch.backends.cuda.matmul.allow_tf32 = False
 torch.backends.cudnn.allow_tf32 = False
 
 
 class Observer:
```

### Comparing `thsquant-0.2.4/thsquant/llama.py` & `thsquant-0.2.5/thsquant/llama.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.4/thsquant/llama_inference.py` & `thsquant-0.2.5/thsquant/llama_inference.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.4/thsquant/llama_inference_offload.py` & `thsquant-0.2.5/thsquant/llama_inference_offload.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.4/thsquant/neox.py` & `thsquant-0.2.5/thsquant/neox.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.4/thsquant/opt.py` & `thsquant-0.2.5/thsquant/opt.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.4/thsquant/quant/custom_autotune.py` & `thsquant-0.2.5/thsquant/quant/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.4/thsquant/quant/fused_attn.py` & `thsquant-0.2.5/thsquant/quant/fused_attn.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.4/thsquant/quant/fused_mlp.py` & `thsquant-0.2.5/thsquant/quant/fused_mlp.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.4/thsquant/quant/quant_linear.py` & `thsquant-0.2.5/thsquant/quant/quant_linear.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.4/thsquant/quant/quantizer.py` & `thsquant-0.2.5/thsquant/quant/quantizer.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.4/thsquant/quant/triton_norm.py` & `thsquant-0.2.5/thsquant/quant/triton_norm.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.4/thsquant/utils/datautils.py` & `thsquant-0.2.5/thsquant/utils/datautils.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.4/thsquant/utils/export.py` & `thsquant-0.2.5/thsquant/utils/export.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.4/thsquant/utils/modelutils.py` & `thsquant-0.2.5/thsquant/utils/modelutils.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.4/thsquant.egg-info/PKG-INFO` & `thsquant-0.2.5/thsquant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thsquant
-Version: 0.2.4
+Version: 0.2.5
 Summary: A short description of your awesome package
 Home-page: https://github.com/qinbo23/ths-quant
 Author: qinbo
 Author-email: qinbo@myhexin.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `thsquant-0.2.4/thsquant.egg-info/SOURCES.txt` & `thsquant-0.2.5/thsquant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

