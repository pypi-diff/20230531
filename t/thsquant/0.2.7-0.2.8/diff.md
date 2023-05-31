# Comparing `tmp/thsquant-0.2.7.tar.gz` & `tmp/thsquant-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thsquant-0.2.7.tar", last modified: Wed May 31 03:18:12 2023, max compression
+gzip compressed data, was "thsquant-0.2.8.tar", last modified: Wed May 31 10:06:21 2023, max compression
```

## Comparing `thsquant-0.2.7.tar` & `thsquant-0.2.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 03:18:12.537835 thsquant-0.2.7/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    11357 2023-05-30 02:01:43.000000 thsquant-0.2.7/LICENSE.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      747 2023-05-31 03:18:12.537835 thsquant-0.2.7/PKG-INFO
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       18 2023-05-30 02:01:43.000000 thsquant-0.2.7/README.md
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       38 2023-05-31 03:18:12.537835 thsquant-0.2.7/setup.cfg
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     1357 2023-05-31 03:17:21.000000 thsquant-0.2.7/setup.py
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 03:18:12.533835 thsquant-0.2.7/thsquant/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        0 2023-05-30 02:01:43.000000 thsquant-0.2.7/thsquant/__init__.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     1112 2023-05-30 02:02:36.000000 thsquant-0.2.7/thsquant/convert_llama_weights_to_hf.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     7713 2023-05-31 02:44:02.000000 thsquant-0.2.7/thsquant/gptq.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    19650 2023-05-31 02:46:41.000000 thsquant-0.2.7/thsquant/llama.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     4661 2023-05-31 03:15:05.000000 thsquant-0.2.7/thsquant/llama_inference.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    13161 2023-05-30 02:02:36.000000 thsquant-0.2.7/thsquant/llama_inference_offload.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    15967 2023-05-30 02:02:36.000000 thsquant-0.2.7/thsquant/neox.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    17497 2023-05-30 02:02:36.000000 thsquant-0.2.7/thsquant/opt.py
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 03:18:12.537835 thsquant-0.2.7/thsquant/quant/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      317 2023-05-30 02:02:36.000000 thsquant-0.2.7/thsquant/quant/__init__.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     8775 2023-05-30 02:02:36.000000 thsquant-0.2.7/thsquant/quant/custom_autotune.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     8799 2023-05-30 02:02:36.000000 thsquant-0.2.7/thsquant/quant/fused_attn.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    12139 2023-05-30 02:02:36.000000 thsquant-0.2.7/thsquant/quant/fused_mlp.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    18730 2023-05-30 02:02:36.000000 thsquant-0.2.7/thsquant/quant/quant_linear.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     4263 2023-05-30 02:02:36.000000 thsquant-0.2.7/thsquant/quant/quantizer.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     3120 2023-05-30 02:02:36.000000 thsquant-0.2.7/thsquant/quant/triton_norm.py
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 03:18:12.537835 thsquant-0.2.7/thsquant/utils/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      215 2023-05-30 02:02:36.000000 thsquant-0.2.7/thsquant/utils/__init__.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     6712 2023-05-30 02:02:36.000000 thsquant-0.2.7/thsquant/utils/datautils.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     1019 2023-05-30 02:02:36.000000 thsquant-0.2.7/thsquant/utils/export.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     2563 2023-05-30 02:02:36.000000 thsquant-0.2.7/thsquant/utils/modelutils.py
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 03:18:12.533835 thsquant-0.2.7/thsquant.egg-info/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      747 2023-05-31 03:18:12.000000 thsquant-0.2.7/thsquant.egg-info/PKG-INFO
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      733 2023-05-31 03:18:12.000000 thsquant-0.2.7/thsquant.egg-info/SOURCES.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       69 2023-05-31 03:18:12.000000 thsquant-0.2.7/thsquant.egg-info/dependency_links.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       62 2023-05-31 03:18:12.000000 thsquant-0.2.7/thsquant.egg-info/entry_points.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      126 2023-05-31 03:18:12.000000 thsquant-0.2.7/thsquant.egg-info/requires.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        9 2023-05-31 03:18:12.000000 thsquant-0.2.7/thsquant.egg-info/top_level.txt
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 10:06:21.240664 thsquant-0.2.8/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    11357 2023-05-30 02:01:43.000000 thsquant-0.2.8/LICENSE.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      747 2023-05-31 10:06:21.240664 thsquant-0.2.8/PKG-INFO
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       18 2023-05-30 02:01:43.000000 thsquant-0.2.8/README.md
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       38 2023-05-31 10:06:21.240664 thsquant-0.2.8/setup.cfg
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     1357 2023-05-31 10:06:07.000000 thsquant-0.2.8/setup.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 10:06:21.240664 thsquant-0.2.8/thsquant/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        0 2023-05-30 02:01:43.000000 thsquant-0.2.8/thsquant/__init__.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     1112 2023-05-30 02:02:36.000000 thsquant-0.2.8/thsquant/convert_llama_weights_to_hf.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     7713 2023-05-31 02:44:02.000000 thsquant-0.2.8/thsquant/gptq.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    19674 2023-05-31 10:05:44.000000 thsquant-0.2.8/thsquant/llama.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     4825 2023-05-31 03:36:05.000000 thsquant-0.2.8/thsquant/llama_inference.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    13161 2023-05-30 02:02:36.000000 thsquant-0.2.8/thsquant/llama_inference_offload.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    15967 2023-05-30 02:02:36.000000 thsquant-0.2.8/thsquant/neox.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    17497 2023-05-30 02:02:36.000000 thsquant-0.2.8/thsquant/opt.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 10:06:21.240664 thsquant-0.2.8/thsquant/quant/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      317 2023-05-30 02:02:36.000000 thsquant-0.2.8/thsquant/quant/__init__.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     8775 2023-05-30 02:02:36.000000 thsquant-0.2.8/thsquant/quant/custom_autotune.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     8799 2023-05-30 02:02:36.000000 thsquant-0.2.8/thsquant/quant/fused_attn.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    12139 2023-05-30 02:02:36.000000 thsquant-0.2.8/thsquant/quant/fused_mlp.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    18730 2023-05-30 02:02:36.000000 thsquant-0.2.8/thsquant/quant/quant_linear.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     4263 2023-05-30 02:02:36.000000 thsquant-0.2.8/thsquant/quant/quantizer.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     3120 2023-05-30 02:02:36.000000 thsquant-0.2.8/thsquant/quant/triton_norm.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 10:06:21.240664 thsquant-0.2.8/thsquant/utils/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      215 2023-05-30 02:02:36.000000 thsquant-0.2.8/thsquant/utils/__init__.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     6712 2023-05-30 02:02:36.000000 thsquant-0.2.8/thsquant/utils/datautils.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     1019 2023-05-30 02:02:36.000000 thsquant-0.2.8/thsquant/utils/export.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     2563 2023-05-30 02:02:36.000000 thsquant-0.2.8/thsquant/utils/modelutils.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-31 10:06:21.240664 thsquant-0.2.8/thsquant.egg-info/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      747 2023-05-31 10:06:20.000000 thsquant-0.2.8/thsquant.egg-info/PKG-INFO
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      733 2023-05-31 10:06:21.000000 thsquant-0.2.8/thsquant.egg-info/SOURCES.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       69 2023-05-31 10:06:20.000000 thsquant-0.2.8/thsquant.egg-info/dependency_links.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       62 2023-05-31 10:06:21.000000 thsquant-0.2.8/thsquant.egg-info/entry_points.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      126 2023-05-31 10:06:21.000000 thsquant-0.2.8/thsquant.egg-info/requires.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        9 2023-05-31 10:06:21.000000 thsquant-0.2.8/thsquant.egg-info/top_level.txt
```

### Comparing `thsquant-0.2.7/LICENSE.txt` & `thsquant-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.7/PKG-INFO` & `thsquant-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thsquant
-Version: 0.2.7
+Version: 0.2.8
 Summary: A short description of your awesome package
 Home-page: https://github.com/qinbo23/ths-quant
 Author: qinbo
 Author-email: qinbo@myhexin.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `thsquant-0.2.7/setup.py` & `thsquant-0.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="thsquant",
-    version="0.2.7",
+    version="0.2.8",
     packages=find_packages(),
     install_requires=[
         'safetensors==0.3.0',
         'datasets==2.10.1',
         'sentencepiece',
         'accelerate==0.17.1',
         'triton==2.0.0',
```

### Comparing `thsquant-0.2.7/thsquant/convert_llama_weights_to_hf.py` & `thsquant-0.2.8/thsquant/convert_llama_weights_to_hf.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.7/thsquant/gptq.py` & `thsquant-0.2.8/thsquant/gptq.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.7/thsquant/llama.py` & `thsquant-0.2.8/thsquant/llama.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     from transformers import LlamaForCausalLM
     model = LlamaForCausalLM.from_pretrained(model, torch_dtype=torch.float16)
     model.seqlen = 2048
     return model
 
 
 @torch.no_grad()
-def llama_sequential(model, dataloader, dev):
+def llama_sequential(model, dataloader, dev, args):
     print('Starting ...')
 
     use_cache = model.config.use_cache
     model.config.use_cache = False
     layers = model.model.layers
 
     model.model.embed_tokens = model.model.embed_tokens.to(dev)
@@ -167,15 +167,15 @@
 
     model.config.use_cache = use_cache
 
     return quantizers
 
 
 @torch.no_grad()
-def llama_eval(model, testenc, dev):
+def llama_eval(model, testenc, dev, args):
     print('Evaluating ...')
 
     testenc = testenc.input_ids
     nsamples = testenc.numel() // model.seqlen
 
     use_cache = model.config.use_cache
     model.config.use_cache = False
@@ -474,15 +474,15 @@
         model = get_llama(args.model)
         model.eval()
 
     dataloader, testloader = get_loaders(args.dataset, nsamples=args.nsamples, seed=args.seed, model=args.model, seqlen=model.seqlen)
 
     if not args.load and args.wbits < 16 and not args.nearest:
         tick = time.time()
-        quantizers = llama_sequential(model, dataloader, DEV)
+        quantizers = llama_sequential(model, dataloader, DEV, args)
         print(time.time() - tick)
 
     if args.benchmark:
         gpus = [torch.device('cuda:%d' % i) for i in range(torch.cuda.device_count())]
         if len(gpus) > 1:
             llama_multigpu(model, gpus, gpu_dist)
         else:
@@ -494,15 +494,15 @@
     if args.eval:
         datasets = ['wikitext2', 'ptb', 'c4']
         if args.new_eval:
             datasets = ['wikitext2', 'ptb-new', 'c4-new']
         for dataset in datasets:
             dataloader, testloader = get_loaders(dataset, seed=args.seed, model=args.model, seqlen=model.seqlen)
             print(dataset)
-            llama_eval(model, testloader, DEV)
+            llama_eval(model, testloader, DEV, args)
 
     if args.quant_directory is not None:
         export_quant_table(quantizers, args.quant_directory)
 
     if not args.observe and args.save:
         llama_pack(model, quantizers, args.wbits, args.groupsize)
         torch.save(model.state_dict(), args.save)
```

### Comparing `thsquant-0.2.7/thsquant/llama_inference.py` & `thsquant-0.2.8/thsquant/llama_inference.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,17 @@
     from transformers import LlamaForCausalLM
     model = LlamaForCausalLM.from_pretrained(model, torch_dtype='auto')
     model.seqlen = 2048
     return model
 
 
 def load_quant(model, checkpoint='', wbits=16, groupsize=-1, fused_mlp=True, eval=True, warmup_autotune=True):
+    print("model: ", model)
+    print("checkpoint: ", checkpoint)
+    print("wbits: ", wbits)
     from transformers import LlamaConfig, LlamaForCausalLM
     config = LlamaConfig.from_pretrained(model)
 
     def noop(*args, **kwargs):
         pass
 
     torch.nn.init.kaiming_uniform_ = noop
@@ -48,19 +51,21 @@
             del layers[name]
     quant.make_quant_linear(model, layers, wbits, groupsize)
 
     del layers
 
     print('Loading model ...')
     if checkpoint.endswith('.safetensors'):
+        print("there")
         from safetensors.torch import load_file as safe_load
         model.load_state_dict(safe_load(checkpoint), strict=False)
     else:
+        print("here")
         model.load_state_dict(torch.load(checkpoint), strict=False)
-
+    print("finish check")
     if eval:
         quant.make_quant_attn(model)
         quant.make_quant_norm(model)
         if fused_mlp:
             quant.make_fused_mlp(model)
     if warmup_autotune:
         quant.autotune_warmup_linear(model, transpose=not (eval))
```

### Comparing `thsquant-0.2.7/thsquant/llama_inference_offload.py` & `thsquant-0.2.8/thsquant/llama_inference_offload.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.7/thsquant/neox.py` & `thsquant-0.2.8/thsquant/neox.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.7/thsquant/opt.py` & `thsquant-0.2.8/thsquant/opt.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.7/thsquant/quant/custom_autotune.py` & `thsquant-0.2.8/thsquant/quant/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.7/thsquant/quant/fused_attn.py` & `thsquant-0.2.8/thsquant/quant/fused_attn.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.7/thsquant/quant/fused_mlp.py` & `thsquant-0.2.8/thsquant/quant/fused_mlp.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.7/thsquant/quant/quant_linear.py` & `thsquant-0.2.8/thsquant/quant/quant_linear.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.7/thsquant/quant/quantizer.py` & `thsquant-0.2.8/thsquant/quant/quantizer.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.7/thsquant/quant/triton_norm.py` & `thsquant-0.2.8/thsquant/quant/triton_norm.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.7/thsquant/utils/datautils.py` & `thsquant-0.2.8/thsquant/utils/datautils.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.7/thsquant/utils/export.py` & `thsquant-0.2.8/thsquant/utils/export.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.7/thsquant/utils/modelutils.py` & `thsquant-0.2.8/thsquant/utils/modelutils.py`

 * *Files identical despite different names*

### Comparing `thsquant-0.2.7/thsquant.egg-info/PKG-INFO` & `thsquant-0.2.8/thsquant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thsquant
-Version: 0.2.7
+Version: 0.2.8
 Summary: A short description of your awesome package
 Home-page: https://github.com/qinbo23/ths-quant
 Author: qinbo
 Author-email: qinbo@myhexin.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `thsquant-0.2.7/thsquant.egg-info/SOURCES.txt` & `thsquant-0.2.8/thsquant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

