# Comparing `tmp/ditty-0.3.1.tar.gz` & `tmp/ditty-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ditty-0.3.1.tar", last modified: Mon May 29 11:54:13 2023, max compression
+gzip compressed data, was "ditty-0.4.0.tar", last modified: Tue May 30 22:17:13 2023, max compression
```

## Comparing `ditty-0.3.1.tar` & `ditty-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-29 11:54:13.110935 ditty-0.3.1/
--rw-rw-r--   0 crow      (1000) crow      (1000)    11357 2023-05-20 22:13:26.000000 ditty-0.3.1/LICENSE
--rw-rw-r--   0 crow      (1000) crow      (1000)     3435 2023-05-29 11:54:13.110935 ditty-0.3.1/PKG-INFO
--rw-rw-r--   0 crow      (1000) crow      (1000)     3138 2023-05-29 11:53:59.000000 ditty-0.3.1/README.md
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-29 11:54:13.110935 ditty-0.3.1/lib/
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-29 11:54:13.110935 ditty-0.3.1/lib/ditty/
--rw-rw-r--   0 crow      (1000) crow      (1000)        0 2023-05-21 15:10:10.000000 ditty-0.3.1/lib/ditty/__init__.py
--rw-rw-r--   0 crow      (1000) crow      (1000)     5251 2023-05-26 05:12:23.000000 ditty-0.3.1/lib/ditty/data.py
--rw-rw-r--   0 crow      (1000) crow      (1000)     7288 2023-05-29 11:53:59.000000 ditty-0.3.1/lib/ditty/pipeline.py
--rw-rw-r--   0 crow      (1000) crow      (1000)     6597 2023-05-27 06:36:39.000000 ditty-0.3.1/lib/ditty/trainer.py
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-29 11:54:13.110935 ditty-0.3.1/lib/ditty.egg-info/
--rw-rw-r--   0 crow      (1000) crow      (1000)     3435 2023-05-29 11:54:13.000000 ditty-0.3.1/lib/ditty.egg-info/PKG-INFO
--rw-rw-r--   0 crow      (1000) crow      (1000)      283 2023-05-29 11:54:13.000000 ditty-0.3.1/lib/ditty.egg-info/SOURCES.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)        1 2023-05-29 11:54:13.000000 ditty-0.3.1/lib/ditty.egg-info/dependency_links.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)       56 2023-05-29 11:54:13.000000 ditty-0.3.1/lib/ditty.egg-info/requires.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)        6 2023-05-29 11:54:13.000000 ditty-0.3.1/lib/ditty.egg-info/top_level.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)      103 2023-05-29 11:54:13.110935 ditty-0.3.1/setup.cfg
--rw-rw-r--   0 crow      (1000) crow      (1000)      639 2023-05-29 11:53:59.000000 ditty-0.3.1/setup.py
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-30 22:17:13.466307 ditty-0.4.0/
+-rw-rw-r--   0 crow      (1000) crow      (1000)    11357 2023-05-20 22:13:26.000000 ditty-0.4.0/LICENSE
+-rw-rw-r--   0 crow      (1000) crow      (1000)     3435 2023-05-30 22:17:13.466307 ditty-0.4.0/PKG-INFO
+-rw-rw-r--   0 crow      (1000) crow      (1000)     3138 2023-05-29 11:53:59.000000 ditty-0.4.0/README.md
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-30 22:17:13.462308 ditty-0.4.0/lib/
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-30 22:17:13.466307 ditty-0.4.0/lib/ditty/
+-rw-rw-r--   0 crow      (1000) crow      (1000)        0 2023-05-21 15:10:10.000000 ditty-0.4.0/lib/ditty/__init__.py
+-rw-rw-r--   0 crow      (1000) crow      (1000)     5251 2023-05-26 05:12:23.000000 ditty-0.4.0/lib/ditty/data.py
+-rw-rw-r--   0 crow      (1000) crow      (1000)     7408 2023-05-30 22:14:56.000000 ditty-0.4.0/lib/ditty/pipeline.py
+-rw-rw-r--   0 crow      (1000) crow      (1000)     8324 2023-05-30 22:14:56.000000 ditty-0.4.0/lib/ditty/trainer.py
+-rw-rw-r--   0 crow      (1000) crow      (1000)      311 2023-05-30 22:14:56.000000 ditty-0.4.0/lib/ditty/utils.py
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-30 22:17:13.466307 ditty-0.4.0/lib/ditty.egg-info/
+-rw-rw-r--   0 crow      (1000) crow      (1000)     3435 2023-05-30 22:17:13.000000 ditty-0.4.0/lib/ditty.egg-info/PKG-INFO
+-rw-rw-r--   0 crow      (1000) crow      (1000)      302 2023-05-30 22:17:13.000000 ditty-0.4.0/lib/ditty.egg-info/SOURCES.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)        1 2023-05-30 22:17:13.000000 ditty-0.4.0/lib/ditty.egg-info/dependency_links.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)       56 2023-05-30 22:17:13.000000 ditty-0.4.0/lib/ditty.egg-info/requires.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)        6 2023-05-30 22:17:13.000000 ditty-0.4.0/lib/ditty.egg-info/top_level.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)      103 2023-05-30 22:17:13.466307 ditty-0.4.0/setup.cfg
+-rw-rw-r--   0 crow      (1000) crow      (1000)      639 2023-05-30 22:16:23.000000 ditty-0.4.0/setup.py
```

### Comparing `ditty-0.3.1/LICENSE` & `ditty-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ditty-0.3.1/PKG-INFO` & `ditty-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ditty
-Version: 0.3.1
+Version: 0.4.0
 Home-page: https://github.com/iantbutler01/ditty
 Author: Ian T Butler (KinglyCrow)
 Author-email: iantbutler01@gmail.com
 License: Apache V2
 Keywords: finetuning,llm,nlp,machine learning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ditty-0.3.1/README.md` & `ditty-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ditty-0.3.1/lib/ditty/data.py` & `ditty-0.4.0/lib/ditty/data.py`

 * *Files identical despite different names*

### Comparing `ditty-0.3.1/lib/ditty/pipeline.py` & `ditty-0.4.0/lib/ditty/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         fp32_cpu_offload=False,
         load_checkpoint=True,
         checkpoint_every=1000,
         gradient_checkpointing=True,
         experimental=False,
         block_size=2048,
         use_bfloat16=False,
+        model_load_kwargs={},
     ):
         self.output_dir = output_dir
         self.dataset_name = dataset_name
         self.dataset_language = dataset_language
         self.model_name_or_path = model_name_or_path
         self.hf_hub_token = hf_hub_token
         self.hf_hub_model_id = hf_hub_model_id
@@ -57,14 +58,15 @@
         self.l4bit = l4bit
         self.push_to_hub = push_to_hub
         self.batch_size = batch_size
         self.grad_accum = grad_accum
         self.block_size = block_size
         self.fp32_cpu_offload = fp32_cpu_offload
         self.use_bfloat16 = use_bfloat16
+        self.model_load_kwargs = model_load_kwargs
 
         if self.l8bit and self.l4bit:
             raise ValueError("Cannot set both l8bit and l4bit to True.")
 
         if self.l4bit and experimental:
             self.bnb_config = BitsAndBytesConfig(
                 load_in_4bit=True,
@@ -133,15 +135,16 @@
             self.tokenizer.pad_token_id = self.tokenizer.eos_token_id
 
         data = self.dataset()
 
         self.model = AutoModelForCausalLM.from_pretrained(
             self.model_name_or_path,
             device_map="auto",
-            quantization_config=self.bnb_config
+            quantization_config=self.bnb_config,
+            **self.model_load_kwargs,
         )
 
         target_modules = None
 
         print(self.model)
 
         if "gpt-neox" in self.model_name_or_path:
```

### Comparing `ditty-0.3.1/lib/ditty/trainer.py` & `ditty-0.4.0/lib/ditty/trainer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from dataclasses import dataclass, field
+import time
+from .utils import convert_seconds_to_string_time
 import torch
 import torch.nn as nn
 from torch.utils.data import DataLoader
 from accelerate import Accelerator
 from accelerate.utils import set_seed, ProjectConfiguration
 from transformers.trainer_pt_utils import (
     get_model_param_count,
 )
 import atexit
 
+
 import numpy as np
 import random
 import contextlib
 
 from peft import PeftModelForCausalLM
 from logging import getLogger
 from typing import Optional
@@ -119,25 +122,38 @@
         context_manager =  contextlib.nullcontext()
 
         if self.fp16:
             context_manager = torch.cuda.amp.autocast(cache_enabled=False, dtype=self.f16_dtype)
 
 
         self.model.train()
-
+        total_batches = len(self.dataset) * epochs
+        start_time = time.time()
+        
+        
+       
         if self.load_checkpoint:
             try:
-                last_cp = sorted(os.listdir(f"{self.output_dir}/checkpoints/"))[-1]
-                logger.info(f"Trying to load checkpoint: {last_cp}....")
-                self.accelerator.load_state(f"{self.output_dir}/checkpoints/{last_cp}")
-
-                # Update the iteration number so that the next checkpoint name is increased by 1
-                last_cp_num = last_cp.split("_")[-1]
-                self.accelerator.project_configuration.iteration = int(last_cp_num) + 1
-                logger.info("Checkpoint loaded.")
+                checkpoints_dir = f"{self.output_dir}/checkpoints/"
+                
+                if os.path.exists(checkpoints_dir) and os.listdir(checkpoints_dir):
+                    last_cp = sorted(os.listdir(checkpoints_dir))[-1]
+                    logger.info(f"Trying to load checkpoint: {last_cp}....")
+                    last_cp = sorted(os.listdir(f"{self.output_dir}/checkpoints/"))[-1]
+                    logger.info(f"Trying to load checkpoint: {last_cp}....")
+                    self.accelerator.load_state(f"{self.output_dir}/checkpoints/{last_cp}")
+
+                    # Update the iteration number so that the next checkpoint name is increased by 1
+                    last_cp_num = last_cp.split("_")[-1]
+                    self.accelerator.project_configuration.iteration = int(last_cp_num) + 1
+                    logger.info("Checkpoint loaded.")
+                else:
+                    logger.warning("No checkpoint found, starting from scratch.")
+                    self._save(no_dist=True)
+                    
             except FileNotFoundError as e:
                 logger.warning(e)
                 logger.warning("No checkpoint found, starting from scratch.")
                 self._save(no_dist=True)
         else:
             self._save(no_dist=True)
 
@@ -159,15 +175,30 @@
                     self.optimizer.step()
                     if self.use_scheduler:
                         self.scheduler.step()
                     self.optimizer.zero_grad()
 
                     batch_loss = loss.item() / self.grad_accum
 
-                    print(f"Epoch {ep} | Batch {batch_idx} | Loss {batch_loss}")
+                    # calculate current epoch as decimal
+                    total_batches_done = ep * len(self.dataset) + batch_idx
+                    current_epoch_decimal = total_batches_done / total_batches
+
+                    # calculate time elapsed and estimate remaining time
+                    time_elapsed = time.time() - start_time
+                    batches_remaining = total_batches - total_batches_done
+                    estimated_time_remaining = (time_elapsed / total_batches_done) * batches_remaining if total_batches_done > 0 else 0
+
+                    # convert estimated_time_remaining to format: dd days, hh hours, mm minutes, ss seconds
+                    estimated_time_remaining_ddhhmmss = convert_seconds_to_string_time(estimated_time_remaining)
+
+                    # calculate percentage done
+                    percent_done = (total_batches_done / total_batches) * 100
+
+                    print(f"Epoch {current_epoch_decimal:.2f} | Batch {batch_idx}/{len(self.dataset)} | Loss {batch_loss} | {percent_done:.2f}% done | Estimated time remaining: {estimated_time_remaining_ddhhmmss}")
 
                     self.state.global_loss += batch_loss
 
                 self.state.steps += 1
                 if max_steps is not None and batch_idx >= max_steps:
                     break
```

### Comparing `ditty-0.3.1/lib/ditty.egg-info/PKG-INFO` & `ditty-0.4.0/lib/ditty.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ditty
-Version: 0.3.1
+Version: 0.4.0
 Home-page: https://github.com/iantbutler01/ditty
 Author: Ian T Butler (KinglyCrow)
 Author-email: iantbutler01@gmail.com
 License: Apache V2
 Keywords: finetuning,llm,nlp,machine learning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ditty-0.3.1/setup.py` & `ditty-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='ditty',
-    version='0.3.1',
+    version='0.4.0',
     license='Apache V2',
     author="Ian T Butler (KinglyCrow)",
     author_email='iantbutler01@gmail.com',
     packages=find_packages('lib'),
     package_dir={'': 'lib'},
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

