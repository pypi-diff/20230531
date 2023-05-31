# Comparing `tmp/fbgemm_gpu_nightly_cpu-2023.5.29-cp39-cp39-manylinux1_x86_64.whl.zip` & `tmp/fbgemm_gpu_nightly_cpu-2023.5.30-cp39-cp39-manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,42 +1,42 @@
-Zip file size: 3505099 bytes, number of entries: 40
--rw-r--r--  2.0 unx      567 b- defN 23-May-29 13:01 fbgemm_gpu/__init__.py
--rw-r--r--  2.0 unx    14920 b- defN 23-May-29 13:01 fbgemm_gpu/_fbgemm_gpu_docs.py
--rw-r--r--  2.0 unx     2747 b- defN 23-May-29 13:01 fbgemm_gpu/batched_unary_embeddings_ops.py
--rw-r--r--  2.0 unx      818 b- defN 23-May-29 13:01 fbgemm_gpu/enums.py
--rwxr-xr-x  2.0 unx 11491080 b- defN 23-May-29 13:01 fbgemm_gpu/fbgemm_gpu_py.so
--rw-r--r--  2.0 unx     5648 b- defN 23-May-29 13:01 fbgemm_gpu/metrics.py
--rw-r--r--  2.0 unx     2339 b- defN 23-May-29 13:01 fbgemm_gpu/permute_pooled_embedding_modules.py
--rw-r--r--  2.0 unx     2477 b- defN 23-May-29 13:01 fbgemm_gpu/permute_pooled_embedding_modules_split.py
--rw-r--r--  2.0 unx     7682 b- defN 23-May-29 13:01 fbgemm_gpu/quantize_comm.py
--rw-r--r--  2.0 unx     4005 b- defN 23-May-29 13:01 fbgemm_gpu/quantize_utils.py
--rw-r--r--  2.0 unx     5727 b- defN 23-May-29 13:01 fbgemm_gpu/split_embedding_configs.py
--rw-r--r--  2.0 unx     8697 b- defN 23-May-29 13:01 fbgemm_gpu/split_embedding_inference_converter.py
--rw-r--r--  2.0 unx    20516 b- defN 23-May-29 13:01 fbgemm_gpu/split_embedding_utils.py
--rw-r--r--  2.0 unx     2170 b- defN 23-May-29 13:01 fbgemm_gpu/split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx     3433 b- defN 23-May-29 13:01 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
--rw-r--r--  2.0 unx    59005 b- defN 23-May-29 13:01 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
--rw-r--r--  2.0 unx    74102 b- defN 23-May-29 13:01 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
--rw-r--r--  2.0 unx    39171 b- defN 23-May-29 13:01 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx      910 b- defN 23-May-29 13:01 fbgemm_gpu/uvm.py
--rw-r--r--  2.0 unx     1912 b- defN 23-May-29 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
--rw-r--r--  2.0 unx     4163 b- defN 23-May-29 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
--rw-r--r--  2.0 unx     4932 b- defN 23-May-29 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
--rw-r--r--  2.0 unx     4465 b- defN 23-May-29 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad.py
--rw-r--r--  2.0 unx     6474 b- defN 23-May-29 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     2558 b- defN 23-May-29 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     3710 b- defN 23-May-29 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_sgd.py
--rw-r--r--  2.0 unx     1533 b- defN 23-May-29 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
--rw-r--r--  2.0 unx     4932 b- defN 23-May-29 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
--rw-r--r--  2.0 unx     4401 b- defN 23-May-29 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
--rw-r--r--  2.0 unx     4964 b- defN 23-May-29 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
--rw-r--r--  2.0 unx     4964 b- defN 23-May-29 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
--rw-r--r--  2.0 unx     4451 b- defN 23-May-29 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
--rw-r--r--  2.0 unx     6460 b- defN 23-May-29 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     2551 b- defN 23-May-29 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     4407 b- defN 23-May-29 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
--rw-r--r--  2.0 unx     3696 b- defN 23-May-29 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
--rw-r--r--  2.0 unx     2934 b- defN 23-May-29 13:01 fbgemm_gpu_nightly_cpu-2023.5.29.dist-info/METADATA
--rw-r--r--  2.0 unx      102 b- defN 23-May-29 13:01 fbgemm_gpu_nightly_cpu-2023.5.29.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-29 13:01 fbgemm_gpu_nightly_cpu-2023.5.29.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4470 b- defN 23-May-29 13:01 fbgemm_gpu_nightly_cpu-2023.5.29.dist-info/RECORD
-40 files, 11824104 bytes uncompressed, 3497555 bytes compressed:  70.4%
+Zip file size: 3505097 bytes, number of entries: 40
+-rw-r--r--  2.0 unx      567 b- defN 23-May-30 12:59 fbgemm_gpu/__init__.py
+-rw-r--r--  2.0 unx    14920 b- defN 23-May-30 12:59 fbgemm_gpu/_fbgemm_gpu_docs.py
+-rw-r--r--  2.0 unx     2747 b- defN 23-May-30 12:59 fbgemm_gpu/batched_unary_embeddings_ops.py
+-rw-r--r--  2.0 unx      818 b- defN 23-May-30 12:59 fbgemm_gpu/enums.py
+-rwxr-xr-x  2.0 unx 11491080 b- defN 23-May-30 12:59 fbgemm_gpu/fbgemm_gpu_py.so
+-rw-r--r--  2.0 unx     5648 b- defN 23-May-30 12:59 fbgemm_gpu/metrics.py
+-rw-r--r--  2.0 unx     2339 b- defN 23-May-30 12:59 fbgemm_gpu/permute_pooled_embedding_modules.py
+-rw-r--r--  2.0 unx     2477 b- defN 23-May-30 12:59 fbgemm_gpu/permute_pooled_embedding_modules_split.py
+-rw-r--r--  2.0 unx     7682 b- defN 23-May-30 12:59 fbgemm_gpu/quantize_comm.py
+-rw-r--r--  2.0 unx     4005 b- defN 23-May-30 12:59 fbgemm_gpu/quantize_utils.py
+-rw-r--r--  2.0 unx     5727 b- defN 23-May-30 12:59 fbgemm_gpu/split_embedding_configs.py
+-rw-r--r--  2.0 unx     8697 b- defN 23-May-30 12:59 fbgemm_gpu/split_embedding_inference_converter.py
+-rw-r--r--  2.0 unx    20516 b- defN 23-May-30 12:59 fbgemm_gpu/split_embedding_utils.py
+-rw-r--r--  2.0 unx     2170 b- defN 23-May-30 12:59 fbgemm_gpu/split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx     3433 b- defN 23-May-30 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
+-rw-r--r--  2.0 unx    59005 b- defN 23-May-30 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
+-rw-r--r--  2.0 unx    74102 b- defN 23-May-30 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
+-rw-r--r--  2.0 unx    39171 b- defN 23-May-30 12:59 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx      910 b- defN 23-May-30 12:59 fbgemm_gpu/uvm.py
+-rw-r--r--  2.0 unx     1912 b- defN 23-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
+-rw-r--r--  2.0 unx     4163 b- defN 23-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
+-rw-r--r--  2.0 unx     4932 b- defN 23-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
+-rw-r--r--  2.0 unx     4465 b- defN 23-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     6474 b- defN 23-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     2558 b- defN 23-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     3710 b- defN 23-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_sgd.py
+-rw-r--r--  2.0 unx     1533 b- defN 23-May-30 12:53 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
+-rw-r--r--  2.0 unx     4932 b- defN 23-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
+-rw-r--r--  2.0 unx     4401 b- defN 23-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
+-rw-r--r--  2.0 unx     4964 b- defN 23-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
+-rw-r--r--  2.0 unx     4964 b- defN 23-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
+-rw-r--r--  2.0 unx     4451 b- defN 23-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     6460 b- defN 23-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     2551 b- defN 23-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     4407 b- defN 23-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
+-rw-r--r--  2.0 unx     3696 b- defN 23-May-30 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
+-rw-r--r--  2.0 unx     2934 b- defN 23-May-30 12:59 fbgemm_gpu_nightly_cpu-2023.5.30.dist-info/METADATA
+-rw-r--r--  2.0 unx      102 b- defN 23-May-30 12:59 fbgemm_gpu_nightly_cpu-2023.5.30.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-30 12:59 fbgemm_gpu_nightly_cpu-2023.5.30.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4470 b- defN 23-May-30 12:59 fbgemm_gpu_nightly_cpu-2023.5.30.dist-info/RECORD
+40 files, 11824104 bytes uncompressed, 3497553 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -102,20 +102,20 @@
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.5.29.dist-info/METADATA
+Filename: fbgemm_gpu_nightly_cpu-2023.5.30.dist-info/METADATA
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.5.29.dist-info/WHEEL
+Filename: fbgemm_gpu_nightly_cpu-2023.5.30.dist-info/WHEEL
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.5.29.dist-info/top_level.txt
+Filename: fbgemm_gpu_nightly_cpu-2023.5.30.dist-info/top_level.txt
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.5.29.dist-info/RECORD
+Filename: fbgemm_gpu_nightly_cpu-2023.5.30.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.5.29.dist-info/METADATA` & `fbgemm_gpu_nightly_cpu-2023.5.30.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbgemm-gpu-nightly-cpu
-Version: 2023.5.29
+Version: 2023.5.30
 Home-page: https://github.com/pytorch/fbgemm
 Author: FBGEMM Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: PyTorch,Recommendation Models,High Performance Computing,GPU,CUDA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.5.29.dist-info/RECORD` & `fbgemm_gpu_nightly_cpu-2023.5.30.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -30,11 +30,11 @@
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py,sha256=fBw0hDYHVaob9Pc2IC_XnpQ0jRStbG9R-IZqBnMywRM,4964
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py,sha256=z_INEdVlMxPi-rrq4W7oma6YnJF6EqHFIJeD1VdJNh0,4964
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py,sha256=YO8izH_FCVjxnhlf-Rx3uwTYrKJeERYEGki-QwnWmag,4451
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py,sha256=5NeEd5Vx-cEpJMLTXFbJqlUtbKptFtx6lFpTSrd6xKA,6460
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py,sha256=U8LroH3QA8U16dylYQ4UGTjEihOaZFbrZYqnqPfsuss,2551
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py,sha256=qOeMzSHbEm74uOWD4W5r5UPZ1NpBqZefvYZS41_9kbE,4407
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=IjeKrN7_9l5SZppuc2WbOR8sv6JtRew5geHKKRIRexY,3696
-fbgemm_gpu_nightly_cpu-2023.5.29.dist-info/METADATA,sha256=niz3EGKxlI7FAdpgaGrBvYb6_VSb931bJ3C6QqwR51M,2934
-fbgemm_gpu_nightly_cpu-2023.5.29.dist-info/WHEEL,sha256=7fnRuWrgVZ-We1c67_7QZCYn_AQfJ-Z7mCmVro0eJMM,102
-fbgemm_gpu_nightly_cpu-2023.5.29.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
-fbgemm_gpu_nightly_cpu-2023.5.29.dist-info/RECORD,,
+fbgemm_gpu_nightly_cpu-2023.5.30.dist-info/METADATA,sha256=UAnLlFcEqwRpQXlut9JGhkMmcGwVpBBHNyUNX5ZuXRQ,2934
+fbgemm_gpu_nightly_cpu-2023.5.30.dist-info/WHEEL,sha256=7fnRuWrgVZ-We1c67_7QZCYn_AQfJ-Z7mCmVro0eJMM,102
+fbgemm_gpu_nightly_cpu-2023.5.30.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
+fbgemm_gpu_nightly_cpu-2023.5.30.dist-info/RECORD,,
```

