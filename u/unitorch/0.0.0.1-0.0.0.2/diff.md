# Comparing `tmp/unitorch-0.0.0.1.tar.gz` & `tmp/unitorch-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unitorch-0.0.0.1.tar", last modified: Sun Feb 21 15:01:10 2021, max compression
+gzip compressed data, was "unitorch-0.0.0.2.tar", last modified: Wed May 31 15:58:31 2023, max compression
```

## Comparing `unitorch-0.0.0.1.tar` & `unitorch-0.0.0.2.tar`

### file list

```diff
@@ -1,88 +1,465 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1856 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     3407 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      129 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      182 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       46 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch/
--rw-rw-r--   0 root         (0) root         (0)     3383 2021-02-14 05:14:17.000000 unitorch-0.0.0.1/unitorch/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch/generation/
--rw-rw-r--   0 root         (0) root         (0)       97 2021-02-19 15:28:33.000000 unitorch-0.0.0.1/unitorch/generation/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    32431 2021-02-21 13:50:56.000000 unitorch-0.0.0.1/unitorch/generation/unilm.py
--rw-rw-r--   0 root         (0) root         (0)    17741 2021-02-20 16:20:37.000000 unitorch-0.0.0.1/unitorch/generation/bart.py
--rw-rw-r--   0 root         (0) root         (0)    25284 2021-02-20 16:20:38.000000 unitorch-0.0.0.1/unitorch/generation/mass.py
--rw-rw-r--   0 root         (0) root         (0)     3277 2021-02-19 02:43:18.000000 unitorch-0.0.0.1/unitorch/core.py
--rw-rw-r--   0 root         (0) root         (0)     2798 2021-02-20 16:20:37.000000 unitorch-0.0.0.1/unitorch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch/tasks/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-02-13 12:32:59.000000 unitorch-0.0.0.1/unitorch/tasks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10269 2021-02-20 16:20:38.000000 unitorch-0.0.0.1/unitorch/tasks/base.py
--rw-rw-r--   0 root         (0) root         (0)        0 2021-01-29 05:36:43.000000 unitorch-0.0.0.1/unitorch/tasks/rl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch/loss/
--rw-rw-r--   0 root         (0) root         (0)       26 2021-02-13 12:34:03.000000 unitorch-0.0.0.1/unitorch/loss/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4030 2021-02-16 13:22:24.000000 unitorch-0.0.0.1/unitorch/loss/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch/score/
--rw-rw-r--   0 root         (0) root         (0)       82 2021-02-16 12:22:46.000000 unitorch-0.0.0.1/unitorch/score/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12997 2021-02-20 16:20:38.000000 unitorch-0.0.0.1/unitorch/score/rouge.py
--rw-rw-r--   0 root         (0) root         (0)     5544 2021-02-20 16:20:37.000000 unitorch-0.0.0.1/unitorch/score/bleu.py
--rw-rw-r--   0 root         (0) root         (0)     5255 2021-02-16 12:26:10.000000 unitorch-0.0.0.1/unitorch/score/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch/ops/
--rw-rw-r--   0 root         (0) root         (0)       73 2021-02-17 07:54:05.000000 unitorch-0.0.0.1/unitorch/ops/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1895 2021-02-20 16:20:37.000000 unitorch-0.0.0.1/unitorch/ops/ngram_repeat_block.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch/classification/
--rw-rw-r--   0 root         (0) root         (0)       36 2021-02-13 04:12:17.000000 unitorch-0.0.0.1/unitorch/classification/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2021-01-21 02:48:55.000000 unitorch-0.0.0.1/unitorch/classification/roberta.py
--rw-rw-r--   0 root         (0) root         (0)     3877 2021-02-20 16:20:37.000000 unitorch-0.0.0.1/unitorch/classification/bert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch/data/
--rw-rw-r--   0 root         (0) root         (0)     3003 2021-02-20 11:53:54.000000 unitorch-0.0.0.1/unitorch/data/dataset_for_auto.py
--rw-rw-r--   0 root         (0) root         (0)       38 2021-02-13 06:38:35.000000 unitorch-0.0.0.1/unitorch/data/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4355 2021-02-16 07:29:21.000000 unitorch-0.0.0.1/unitorch/data/dataset_for_preprocess.py
--rw-rw-r--   0 root         (0) root         (0)     2115 2021-02-14 16:39:09.000000 unitorch-0.0.0.1/unitorch/data/dataset_for_raw_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch/modules/
--rw-rw-r--   0 root         (0) root         (0)    25358 2021-02-20 16:20:37.000000 unitorch-0.0.0.1/unitorch/modules/generation_mixin_v2.py
--rw-rw-r--   0 root         (0) root         (0)       44 2021-02-17 07:21:10.000000 unitorch-0.0.0.1/unitorch/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-01-19 07:11:38.000000 unitorch-0.0.0.1/unitorch/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2021-01-19 07:11:38.000000 unitorch-0.0.0.1/unitorch/utils/files.py
--rw-rw-r--   0 root         (0) root         (0)     7752 2021-02-20 16:20:38.000000 unitorch-0.0.0.1/unitorch/utils/decorators.py
--rw-rw-r--   0 root         (0) root         (0)     3379 2021-02-18 12:56:23.000000 unitorch-0.0.0.1/unitorch/utils/buffer.py
--rw-rw-r--   0 root         (0) root         (0)       68 2021-02-09 11:07:15.000000 unitorch-0.0.0.1/unitorch/utils/hf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch/clib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch/clib/cuda/
--rw-rw-r--   0 root         (0) root         (0)     2643 2021-02-17 07:54:59.000000 unitorch-0.0.0.1/unitorch/clib/cuda/ngram_repeat_block_cuda_kernel.cu
--rw-rw-r--   0 root         (0) root         (0)     1496 2021-02-17 07:54:59.000000 unitorch-0.0.0.1/unitorch/clib/cuda/ngram_repeat_block_cuda.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch/auto/
--rw-rw-r--   0 root         (0) root         (0)       73 2021-02-13 06:44:41.000000 unitorch-0.0.0.1/unitorch/auto/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6100 2021-02-14 16:39:09.000000 unitorch-0.0.0.1/unitorch/auto/supervised_task.py
--rw-rw-r--   0 root         (0) root         (0)      447 2021-02-12 16:57:21.000000 unitorch-0.0.0.1/unitorch/distributed.py
--rw-rw-r--   0 root         (0) root         (0)     1721 2021-02-20 12:37:36.000000 unitorch-0.0.0.1/unitorch/functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch/optim/
--rw-rw-r--   0 root         (0) root         (0)       27 2021-02-13 06:35:42.000000 unitorch-0.0.0.1/unitorch/optim/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      557 2021-02-13 06:35:25.000000 unitorch-0.0.0.1/unitorch/optim/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch/process/
--rw-rw-r--   0 root         (0) root         (0)     4681 2021-02-17 09:39:31.000000 unitorch-0.0.0.1/unitorch/process/label.py
--rw-rw-r--   0 root         (0) root         (0)      211 2021-02-20 16:20:37.000000 unitorch-0.0.0.1/unitorch/process/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10958 2021-02-20 16:20:37.000000 unitorch-0.0.0.1/unitorch/process/bert.py
--rw-rw-r--   0 root         (0) root         (0)    17207 2021-02-20 16:20:38.000000 unitorch-0.0.0.1/unitorch/process/unilm.py
--rw-rw-r--   0 root         (0) root         (0)     7580 2021-02-20 16:20:37.000000 unitorch-0.0.0.1/unitorch/process/bart.py
--rw-rw-r--   0 root         (0) root         (0)     2149 2021-02-19 02:48:11.000000 unitorch-0.0.0.1/unitorch/process/base.py
--rw-rw-r--   0 root         (0) root         (0)     6580 2021-02-20 16:20:37.000000 unitorch-0.0.0.1/unitorch/process/mass.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/config/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/config/core/
--rw-rw-r--   0 root         (0) root         (0)     1219 2021-02-20 11:50:40.000000 unitorch-0.0.0.1/config/core/bart_for_generation.ini
--rw-rw-r--   0 root         (0) root         (0)     1300 2021-02-20 15:54:32.000000 unitorch-0.0.0.1/config/core/mass_for_generation.ini
--rw-rw-r--   0 root         (0) root         (0)     1314 2021-02-20 16:14:41.000000 unitorch-0.0.0.1/config/core/unilm_for_generation.ini
--rw-rw-r--   0 root         (0) root         (0)     1338 2021-02-20 14:42:36.000000 unitorch-0.0.0.1/config/core/bert_for_classification.ini
--rw-rw-r--   0 root         (0) root         (0)     2214 2021-02-21 15:00:59.000000 unitorch-0.0.0.1/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3407 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1924 2021-02-21 14:47:01.000000 unitorch-0.0.0.1/readme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-21 15:01:10.000000 unitorch-0.0.0.1/unitorch_cli/
--rw-rw-r--   0 root         (0) root         (0)     3002 2021-02-17 09:45:01.000000 unitorch-0.0.0.1/unitorch_cli/auto_train.py
--rw-rw-r--   0 root         (0) root         (0)     3017 2021-02-17 09:45:11.000000 unitorch-0.0.0.1/unitorch_cli/auto_infer.py
--rw-rw-r--   0 root         (0) root         (0)        0 2021-02-20 07:46:40.000000 unitorch-0.0.0.1/unitorch_cli/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2021-02-08 07:00:52.000000 unitorch-0.0.0.1/unitorch_cli/faster_serve.py
--rw-rw-r--   0 root         (0) root         (0)        0 2021-02-08 07:00:04.000000 unitorch-0.0.0.1/unitorch_cli/faster_infer.py
--rw-rw-r--   0 root         (0) root         (0)       87 2021-02-21 14:37:39.000000 unitorch-0.0.0.1/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)      116 2021-02-20 10:05:11.000000 unitorch-0.0.0.1/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.288718 unitorch-0.0.0.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.120706 unitorch-0.0.0.2/.pytest_cache/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-05-31 15:58:14.000000 unitorch-0.0.0.2/.pytest_cache/README.md
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      131 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8981 2023-05-31 15:58:31.288718 unitorch-0.0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7952 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.124706 unitorch-0.0.0.2/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)       87 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/benchmarks/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.104704 unitorch-0.0.0.2/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.124706 unitorch-0.0.0.2/docs/search/
+-rw-r--r--   0 root         (0) root         (0)  1019191 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/docs/search/search_index.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.128706 unitorch-0.0.0.2/examples/
+-rw-r--r--   0 root         (0) root         (0)     2311 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.104704 unitorch-0.0.0.2/examples/configs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.128706 unitorch-0.0.0.2/examples/configs/caption/
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/caption/blip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.132706 unitorch-0.0.0.2/examples/configs/classification/
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/bert.ini
+-rw-r--r--   0 root         (0) root         (0)     1700 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/clip.ini
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/image_clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.132706 unitorch-0.0.0.2/examples/configs/classification/lora/
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/lora/bloom.ini
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/lora/bloom_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/lora/llama.ini
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/lora/llama_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/roberta.ini
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/swin.ini
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/classification/text_clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.136707 unitorch-0.0.0.2/examples/configs/generation/
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/bart.ini
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/bloom.ini
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/chatglm.ini
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/llama.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.140707 unitorch-0.0.0.2/examples/configs/generation/lora/
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/lora/bloom.ini
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/lora/bloom_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/lora/llama.ini
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/lora/llama_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/mbart.ini
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/mt5.ini
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/pegasus.ini
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/t5.ini
+-rw-r--r--   0 root         (0) root         (0)     1647 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/xpegasus.ini
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/generation/xprophetnet.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.140707 unitorch-0.0.0.2/examples/configs/pretrain/
+-rw-r--r--   0 root         (0) root         (0)     1266 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/pretrain/clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.104704 unitorch-0.0.0.2/examples/configs/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.140707 unitorch-0.0.0.2/examples/configs/services/zip_image/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/services/zip_image/config.ini
+-rw-r--r--   0 root         (0) root         (0)      240 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/configs/services/zip_image/config_v2.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.104704 unitorch-0.0.0.2/examples/hub/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.140707 unitorch-0.0.0.2/examples/hub/caption/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/hub/caption/blip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.140707 unitorch-0.0.0.2/examples/hub/classification/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/hub/classification/bert.ini
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/hub/classification/clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.140707 unitorch-0.0.0.2/examples/hub/generation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/hub/generation/bart.ini
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/hub/generation/llama.ini
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/examples/hub/generation/xpegasus.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.140707 unitorch-0.0.0.2/notebooks/
+-rw-r--r--   0 root         (0) root         (0)      131 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/notebooks/README.md
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      123 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 15:58:31.288718 unitorch-0.0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.104704 unitorch-0.0.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.140707 unitorch-0.0.0.2/src/unitorch/
+-rw-r--r--   0 root         (0) root         (0)     2614 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.144707 unitorch-0.0.0.2/src/unitorch/cli/
+-rw-r--r--   0 root         (0) root         (0)     6024 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.148708 unitorch-0.0.0.2/src/unitorch/cli/console/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/console/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/console/eval.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/console/infer.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/console/script.py
+-rw-r--r--   0 root         (0) root         (0)     4606 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/console/service.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/console/train.py
+-rw-r--r--   0 root         (0) root         (0)     4397 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.148708 unitorch-0.0.0.2/src/unitorch/cli/datasets/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12406 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/datasets/hf.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.148708 unitorch-0.0.0.2/src/unitorch/cli/loss/
+-rw-r--r--   0 root         (0) root         (0)     4063 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/loss/ranking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.152708 unitorch-0.0.0.2/src/unitorch/cli/models/
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.156708 unitorch-0.0.0.2/src/unitorch/cli/models/bart/
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/bart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6981 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/bart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     6140 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/bart/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.156708 unitorch-0.0.0.2/src/unitorch/cli/models/beit/
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/beit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/beit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/beit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.156708 unitorch-0.0.0.2/src/unitorch/cli/models/bert/
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/bert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/bert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     6128 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/bert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.160709 unitorch-0.0.0.2/src/unitorch/cli/models/blip/
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/blip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22703 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/blip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     7788 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/blip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.160709 unitorch-0.0.0.2/src/unitorch/cli/models/bloom/
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/bloom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13026 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/bloom/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8321 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/bloom/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.160709 unitorch-0.0.0.2/src/unitorch/cli/models/chatglm/
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/chatglm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13764 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/chatglm/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8833 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/chatglm/processing.py
+-rw-r--r--   0 root         (0) root         (0)     9143 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/classification_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.164709 unitorch-0.0.0.2/src/unitorch/cli/models/clip/
+-rw-r--r--   0 root         (0) root         (0)     2514 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/clip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16125 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/clip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/clip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.164709 unitorch-0.0.0.2/src/unitorch/cli/models/deberta/
+-rw-r--r--   0 root         (0) root         (0)     4492 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/deberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4077 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/deberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/deberta/modeling_v2.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/deberta/processing.py
+-rw-r--r--   0 root         (0) root         (0)     3434 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/deberta/processing_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2545 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/detection_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.168709 unitorch-0.0.0.2/src/unitorch/cli/models/diffusers/
+-rw-r--r--   0 root         (0) root         (0)     2807 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/diffusers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/diffusers/modeling_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/diffusers/modeling_stable.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/diffusers/processing_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/diffusers/processing_stable.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/diffusion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/generation_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5092 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/image_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/label_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.168709 unitorch-0.0.0.2/src/unitorch/cli/models/llama/
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/llama/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14017 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/llama/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8206 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/llama/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.168709 unitorch-0.0.0.2/src/unitorch/cli/models/mbart/
+-rw-r--r--   0 root         (0) root         (0)      887 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/mbart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/mbart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5826 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/mbart/processing.py
+-rw-r--r--   0 root         (0) root         (0)    15281 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/modeling_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.172709 unitorch-0.0.0.2/src/unitorch/cli/models/mt5/
+-rw-r--r--   0 root         (0) root         (0)     1381 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/mt5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7125 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/mt5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5815 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/mt5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.172709 unitorch-0.0.0.2/src/unitorch/cli/models/peft/
+-rw-r--r--   0 root         (0) root         (0)      524 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/peft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30502 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/peft/modeling_bloom.py
+-rw-r--r--   0 root         (0) root         (0)    30560 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/peft/modeling_llama.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.176710 unitorch-0.0.0.2/src/unitorch/cli/models/pegasus/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/pegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7233 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/pegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5885 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/pegasus/processing.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/processing_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.176710 unitorch-0.0.0.2/src/unitorch/cli/models/prophetnet/
+-rw-r--r--   0 root         (0) root         (0)      162 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/prophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/prophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/prophetnet/processing.py
+-rw-r--r--   0 root         (0) root         (0)      650 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/random_utils.py
+-rw-r--r--   0 root         (0) root         (0)      535 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/ranking_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.176710 unitorch-0.0.0.2/src/unitorch/cli/models/roberta/
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     3766 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/roberta/processing.py
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/segmentation_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.180710 unitorch-0.0.0.2/src/unitorch/cli/models/swin/
+-rw-r--r--   0 root         (0) root         (0)     3032 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/swin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3225 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/swin/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2564 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/swin/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.180710 unitorch-0.0.0.2/src/unitorch/cli/models/t5/
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/t5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7144 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/t5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5811 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/t5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.180710 unitorch-0.0.0.2/src/unitorch/cli/models/visualbert/
+-rw-r--r--   0 root         (0) root         (0)     1310 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/visualbert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8538 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/visualbert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     6306 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/visualbert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.184710 unitorch-0.0.0.2/src/unitorch/cli/models/vit/
+-rw-r--r--   0 root         (0) root         (0)     4602 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/vit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/vit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/vit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.184710 unitorch-0.0.0.2/src/unitorch/cli/models/xlm_roberta/
+-rw-r--r--   0 root         (0) root         (0)     2314 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/xlm_roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7533 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/xlm_roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     3408 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/xlm_roberta/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.184710 unitorch-0.0.0.2/src/unitorch/cli/models/xpegasus/
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/xpegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7238 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/xpegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5953 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/xpegasus/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.184710 unitorch-0.0.0.2/src/unitorch/cli/models/xprophetnet/
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/xprophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7811 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/xprophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5952 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/models/xprophetnet/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.188711 unitorch-0.0.0.2/src/unitorch/cli/optim/
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/optim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/optim/lion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.188711 unitorch-0.0.0.2/src/unitorch/cli/rl/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/rl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.188711 unitorch-0.0.0.2/src/unitorch/cli/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      141 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/scheduler/warmup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.188711 unitorch-0.0.0.2/src/unitorch/cli/score/
+-rw-r--r--   0 root         (0) root         (0)    13366 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/score/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.188711 unitorch-0.0.0.2/src/unitorch/cli/scripts/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/scripts/README.md
+-rw-r--r--   0 root         (0) root         (0)      213 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/scripts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.188711 unitorch-0.0.0.2/src/unitorch/cli/services/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      223 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/services/readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.192711 unitorch-0.0.0.2/src/unitorch/cli/services/zip_image/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/services/zip_image/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4866 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/services/zip_image/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.192711 unitorch-0.0.0.2/src/unitorch/cli/tasks/
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26530 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/tasks/deepspeed.py
+-rw-r--r--   0 root         (0) root         (0)    31564 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/tasks/supervised.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.192711 unitorch-0.0.0.2/src/unitorch/cli/utils/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.192711 unitorch-0.0.0.2/src/unitorch/cli/writer/
+-rw-r--r--   0 root         (0) root         (0)    10545 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/cli/writer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.192711 unitorch-0.0.0.2/src/unitorch/datasets/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6832 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/datasets/hf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.196711 unitorch-0.0.0.2/src/unitorch/loss/
+-rw-r--r--   0 root         (0) root         (0)     4712 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/loss/prophetnet.py
+-rw-r--r--   0 root         (0) root         (0)     8411 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/loss/ranking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.196711 unitorch-0.0.0.2/src/unitorch/models/
+-rw-r--r--   0 root         (0) root         (0)     7429 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.196711 unitorch-0.0.0.2/src/unitorch/models/bart/
+-rw-r--r--   0 root         (0) root         (0)      204 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/bart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13544 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/bart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/bart/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.200711 unitorch-0.0.0.2/src/unitorch/models/beit/
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/beit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/beit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/beit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.200711 unitorch-0.0.0.2/src/unitorch/models/bert/
+-rw-r--r--   0 root         (0) root         (0)      208 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/bert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/bert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8351 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/bert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.200711 unitorch-0.0.0.2/src/unitorch/models/blip/
+-rw-r--r--   0 root         (0) root         (0)      306 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/blip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30316 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/blip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     7700 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/blip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.204712 unitorch-0.0.0.2/src/unitorch/models/bloom/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/bloom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10867 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/bloom/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     9140 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/bloom/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.208712 unitorch-0.0.0.2/src/unitorch/models/chatglm/
+-rw-r--r--   0 root         (0) root         (0)      259 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/chatglm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)    11157 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/chatglm/modeling.py
+-rw-r--r--   0 root         (0) root         (0)    55823 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)    11091 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/chatglm/processing.py
+-rw-r--r--   0 root         (0) root         (0)    15625 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/chatglm/quantization.py
+-rw-r--r--   0 root         (0) root         (0)    16827 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/chatglm/tokenization_chatglm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.208712 unitorch-0.0.0.2/src/unitorch/models/clip/
+-rw-r--r--   0 root         (0) root         (0)      281 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/clip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15100 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/clip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     4393 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/clip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.212712 unitorch-0.0.0.2/src/unitorch/models/deberta/
+-rw-r--r--   0 root         (0) root         (0)      424 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/deberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4503 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/deberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/deberta/modeling_v2.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/deberta/processing.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/deberta/processing_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.212712 unitorch-0.0.0.2/src/unitorch/models/diffusers/
+-rw-r--r--   0 root         (0) root         (0)      149 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/diffusers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/diffusers/modeling_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/diffusers/modeling_stable.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/diffusers/processing_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/diffusers/processing_stable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.212712 unitorch-0.0.0.2/src/unitorch/models/llama/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/llama/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11334 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/llama/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8976 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/llama/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.216713 unitorch-0.0.0.2/src/unitorch/models/mbart/
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/mbart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13928 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/mbart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/mbart/processing.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/modeling_ema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.216713 unitorch-0.0.0.2/src/unitorch/models/mt5/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/mt5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14219 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/mt5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/mt5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.220713 unitorch-0.0.0.2/src/unitorch/models/peft/
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/peft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9891 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/peft/modeling_bloom_adalora.py
+-rw-r--r--   0 root         (0) root         (0)     9487 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/peft/modeling_bloom_lora.py
+-rw-r--r--   0 root         (0) root         (0)    10082 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/peft/modeling_llama_adalora.py
+-rw-r--r--   0 root         (0) root         (0)     9266 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/peft/modeling_llama_lora.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/peft/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.220713 unitorch-0.0.0.2/src/unitorch/models/pegasus/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/pegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13604 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/pegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/pegasus/processing.py
+-rw-r--r--   0 root         (0) root         (0)    13125 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/processing_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.220713 unitorch-0.0.0.2/src/unitorch/models/prophetnet/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/prophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7435 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/prophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/prophetnet/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.224713 unitorch-0.0.0.2/src/unitorch/models/roberta/
+-rw-r--r--   0 root         (0) root         (0)      218 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4281 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/roberta/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.224713 unitorch-0.0.0.2/src/unitorch/models/swin/
+-rw-r--r--   0 root         (0) root         (0)      193 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/swin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/swin/modeling.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/swin/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.224713 unitorch-0.0.0.2/src/unitorch/models/t5/
+-rw-r--r--   0 root         (0) root         (0)      194 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/t5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13285 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/t5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/t5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.228713 unitorch-0.0.0.2/src/unitorch/models/visualbert/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/visualbert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6710 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/visualbert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2343 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/visualbert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.228713 unitorch-0.0.0.2/src/unitorch/models/vit/
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/vit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/vit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/vit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.228713 unitorch-0.0.0.2/src/unitorch/models/xlm_roberta/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/xlm_roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7381 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/xlm_roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/xlm_roberta/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.232714 unitorch-0.0.0.2/src/unitorch/models/xpegasus/
+-rw-r--r--   0 root         (0) root         (0)      237 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/xpegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13693 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/xpegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/xpegasus/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.232714 unitorch-0.0.0.2/src/unitorch/models/xprophetnet/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/xprophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13514 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/xprophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/models/xprophetnet/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.232714 unitorch-0.0.0.2/src/unitorch/modules/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/modules/classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.236714 unitorch-0.0.0.2/src/unitorch/modules/replace/
+-rw-r--r--   0 root         (0) root         (0)      199 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/modules/replace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14643 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/modules/replace/beam_search_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/modules/replace/datasets_v2.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/modules/replace/hf_hub_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/modules/timm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.236714 unitorch-0.0.0.2/src/unitorch/ops/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/ops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16794 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/ops/dyhead.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/ops/ngram_repeat_block.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.236714 unitorch-0.0.0.2/src/unitorch/optim/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/optim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/optim/lion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.236714 unitorch-0.0.0.2/src/unitorch/rl/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/rl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.236714 unitorch-0.0.0.2/src/unitorch/rl/utils/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/rl/utils/buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.240714 unitorch-0.0.0.2/src/unitorch/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      149 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/scheduler/warmup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.240714 unitorch-0.0.0.2/src/unitorch/score/
+-rw-r--r--   0 root         (0) root         (0)     1803 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/score/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/score/bleu.py
+-rw-r--r--   0 root         (0) root         (0)     7852 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/score/map.py
+-rw-r--r--   0 root         (0) root         (0)    13291 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/score/rouge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.240714 unitorch-0.0.0.2/src/unitorch/tasks/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.244715 unitorch-0.0.0.2/src/unitorch/utils/
+-rw-r--r--   0 root         (0) root         (0)    13580 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/utils/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/utils/functional.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/utils/image_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/utils/import_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/utils/io.py
+-rw-r--r--   0 root         (0) root         (0)     5027 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/utils/palette.py
+-rw-r--r--   0 root         (0) root         (0)     3851 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/src/unitorch/utils/torch_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.144707 unitorch-0.0.0.2/src/unitorch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8981 2023-05-31 15:58:30.000000 unitorch-0.0.0.2/src/unitorch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12862 2023-05-31 15:58:31.000000 unitorch-0.0.0.2/src/unitorch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 15:58:30.000000 unitorch-0.0.0.2/src/unitorch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      287 2023-05-31 15:58:30.000000 unitorch-0.0.0.2/src/unitorch.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-31 15:58:30.000000 unitorch-0.0.0.2/src/unitorch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-31 15:58:30.000000 unitorch-0.0.0.2/src/unitorch.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.244715 unitorch-0.0.0.2/wiki/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.248715 unitorch-0.0.0.2/wiki/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/benchmarks/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.248715 unitorch-0.0.0.2/wiki/cli/
+-rw-r--r--   0 root         (0) root         (0)      504 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/ast.md
+-rw-r--r--   0 root         (0) root         (0)      173 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/csv.md
+-rw-r--r--   0 root         (0) root         (0)      414 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/datatypes.md
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/deepspeed.md
+-rw-r--r--   0 root         (0) root         (0)      181 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/jsonl.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.276717 unitorch-0.0.0.2/wiki/cli/models/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/bart.md
+-rw-r--r--   0 root         (0) root         (0)      379 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/beit.md
+-rw-r--r--   0 root         (0) root         (0)      364 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/bert.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/blip.md
+-rw-r--r--   0 root         (0) root         (0)      719 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/bloom.md
+-rw-r--r--   0 root         (0) root         (0)      761 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/chatglm.md
+-rw-r--r--   0 root         (0) root         (0)      939 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/clip.md
+-rw-r--r--   0 root         (0) root         (0)      783 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/deberta.md
+-rw-r--r--   0 root         (0) root         (0)      353 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/diffusers.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/index.md
+-rw-r--r--   0 root         (0) root         (0)      719 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/llama.md
+-rw-r--r--   0 root         (0) root         (0)      359 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/mbart.md
+-rw-r--r--   0 root         (0) root         (0)      337 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/mt5.md
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/peft.md
+-rw-r--r--   0 root         (0) root         (0)      381 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/pegasus.md
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/prophetnet.md
+-rw-r--r--   0 root         (0) root         (0)      398 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/roberta.md
+-rw-r--r--   0 root         (0) root         (0)      379 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/swin.md
+-rw-r--r--   0 root         (0) root         (0)      326 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/t5.md
+-rw-r--r--   0 root         (0) root         (0)      623 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/visualbert.md
+-rw-r--r--   0 root         (0) root         (0)      368 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/vit.md
+-rw-r--r--   0 root         (0) root         (0)      664 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/xlm_roberta.md
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/xpegasus.md
+-rw-r--r--   0 root         (0) root         (0)      425 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/models/xprophetnet.md
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/parquet.md
+-rw-r--r--   0 root         (0) root         (0)      851 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/postprocess.md
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/preprocess.md
+-rw-r--r--   0 root         (0) root         (0)      192 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/cli/supervised.md
+-rw-r--r--   0 root         (0) root         (0)     4600 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/configuration.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.116705 unitorch-0.0.0.2/wiki/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.276717 unitorch-0.0.0.2/wiki/examples/caption/
+-rw-r--r--   0 root         (0) root         (0)     4659 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/examples/caption/blip.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.276717 unitorch-0.0.0.2/wiki/examples/classification/
+-rw-r--r--   0 root         (0) root         (0)     4208 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/examples/classification/clip.md
+-rw-r--r--   0 root         (0) root         (0)     4130 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/examples/classification/roberta.md
+-rw-r--r--   0 root         (0) root         (0)     4525 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/examples/classification/swin.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.276717 unitorch-0.0.0.2/wiki/examples/diffusion/
+-rw-r--r--   0 root         (0) root         (0)       32 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/examples/diffusion/controlnet.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.276717 unitorch-0.0.0.2/wiki/examples/generation/
+-rw-r--r--   0 root         (0) root         (0)     4145 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/examples/generation/bart.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.276717 unitorch-0.0.0.2/wiki/examples/service/
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/examples/service/zip_image.md
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/index.md
+-rw-r--r--   0 root         (0) root         (0)      890 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/installation.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.276717 unitorch-0.0.0.2/wiki/labs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/labs/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:58:31.288718 unitorch-0.0.0.2/wiki/models/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/bart.md
+-rw-r--r--   0 root         (0) root         (0)      165 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/beit.md
+-rw-r--r--   0 root         (0) root         (0)      155 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/bert.md
+-rw-r--r--   0 root         (0) root         (0)      453 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/blip.md
+-rw-r--r--   0 root         (0) root         (0)      296 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/bloom.md
+-rw-r--r--   0 root         (0) root         (0)      322 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/chatglm.md
+-rw-r--r--   0 root         (0) root         (0)      383 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/clip.md
+-rw-r--r--   0 root         (0) root         (0)      402 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/deberta.md
+-rw-r--r--   0 root         (0) root         (0)      152 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/diffusers.md
+-rw-r--r--   0 root         (0) root         (0)      450 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/index.md
+-rw-r--r--   0 root         (0) root         (0)      296 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/llama.md
+-rw-r--r--   0 root         (0) root         (0)      154 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/mbart.md
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/mt5.md
+-rw-r--r--   0 root         (0) root         (0)      695 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/peft.md
+-rw-r--r--   0 root         (0) root         (0)      168 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/pegasus.md
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/prophetnet.md
+-rw-r--r--   0 root         (0) root         (0)      243 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/roberta.md
+-rw-r--r--   0 root         (0) root         (0)      165 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/swin.md
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/t5.md
+-rw-r--r--   0 root         (0) root         (0)      277 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/visualbert.md
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/vit.md
+-rw-r--r--   0 root         (0) root         (0)      375 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/xlm_roberta.md
+-rw-r--r--   0 root         (0) root         (0)      175 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/xpegasus.md
+-rw-r--r--   0 root         (0) root         (0)      196 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/models/xprophetnet.md
+-rw-r--r--   0 root         (0) root         (0)     4524 2023-05-31 15:48:32.000000 unitorch-0.0.0.2/wiki/overview.md
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `unitorch-0.0.0.1/unitorch/generation/unilm.py` & `unitorch-0.0.0.2/src/unitorch/models/blip/modeling.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,846 +1,789 @@
+# Copyright (c) FULIUCANSHENG.
+# Licensed under the MIT License.
+
 import os
-import torch
-import math
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
-from collections import OrderedDict
-from torch import Tensor, device
 import json
+import math
 import random
-from functools import partial
-import numpy as np
+import logging
+import transformers
+import torch
 import torch.nn as nn
 import torch.nn.functional as F
+import torch.distributed as dist
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
-from unitorch import add_core_pretrained_dict, register_model
-from unitorch.core import core_model_class
-from unitorch.utils.hf import hf_cached_path
-from unitorch.modules.generation_mixin_v2 import GenerationMixinV2
-from transformers import PretrainedConfig, PreTrainedModel
-from transformers.models.bert.modeling_bert import (
-    BertEmbeddings,
-    BertIntermediate,
-    BertOutput,
-    BertPooler,
-    BertPreTrainingHeads,
-    BertPreTrainedModel,
-    BertSelfOutput,
-)
-from transformers.modeling_outputs import Seq2SeqLMOutput
-from transformers.modeling_utils import apply_chunking_to_forward
-from transformers.file_utils import ModelOutput
-
-from unitorch.utils.decorators import (
-    generation_model_decorator,
-    add_default_section_for_init,
-    add_default_section_for_instance_function,
-    replace,
+from transformers.models.blip.modeling_blip import (
+    BlipConfig,
+    BlipTextModel,
+    BlipVisionModel,
+    BlipForConditionalGeneration,
 )
+from transformers.models.blip.modeling_blip_text import apply_chunking_to_forward
+from unitorch.utils.decorators import replace
+from unitorch.models import GenericModel, GenericOutputs
+from unitorch.models.clip.modeling import AllGather
 
-CONFIG_KEY = "config"
-CONFIG_NAME = "config.json"
 
-VOCABS_KEY = "vocab"
-VOCABS_NAME = "vocab.txt"
+def _contrastive_loss(logits: torch.Tensor) -> torch.Tensor:
+    return nn.functional.cross_entropy(
+        logits, torch.arange(len(logits), device=logits.device)
+    )
 
-CORE_UNILM_PRETRAINED_DICT = {
-    "default-unilm": {
-        "config": "https://huggingface.co/fuliucansheng/unilm/resolve/main/unilm-base-uncased-config.json",
-        "vocab": "https://unilm.blob.core.windows.net/ckpt/unilm1.2-base-uncased-vocab.txt",
-    },
-    "unilm-base-uncased": {
-        "config": "https://huggingface.co/fuliucansheng/unilm/resolve/main/unilm-base-uncased-config.json",
-        "vocab": "https://unilm.blob.core.windows.net/ckpt/unilm1.2-base-uncased-vocab.txt",
-        "weight": "https://unilm.blob.core.windows.net/ckpt/unilm1.2-base-uncased.bin",
-    },
-}
-
-add_core_pretrained_dict(CORE_UNILM_PRETRAINED_DICT)
-
-
-def _reorder_buffer(attn_cache, beam_idx):
-    for k, input_buffer_k in attn_cache.items():
-        if input_buffer_k is not None and "prefix_" not in k:
-            attn_cache[k] = input_buffer_k.index_select(0, beam_idx)
-    return attn_cache
-
-
-def _reorder_buffer_v2(attn_cache, batch_idx, beam_idx):
-    for k, input_buffer_k in attn_cache.items():
-        if input_buffer_k is not None:
-            if "prefix_" in k:
-                attn_cache[k] = (
-                    input_buffer_k
-                    if batch_idx is None
-                    else input_buffer_k.index_select(0, batch_idx)
-                )
-            else:
-                attn_cache[k] = (
-                    input_buffer_k
-                    if beam_idx is None
-                    else input_buffer_k.index_select(0, beam_idx)
-                )
-    return attn_cache
+
+def _blip_loss(similarity: torch.Tensor) -> torch.Tensor:
+    caption_loss = _contrastive_loss(similarity)
+    image_loss = _contrastive_loss(similarity.T)
+    return (caption_loss + image_loss) / 2.0
 
 
-class UnilmConfig(PretrainedConfig):
+@replace(transformers.models.blip.modeling_blip_text.BlipTextSelfAttention)
+class BlipTextSelfAttentionV2(
+    transformers.models.blip.modeling_blip_text.BlipTextSelfAttention
+):
     def __init__(
         self,
-        vocab_size=28996,
-        hidden_size=768,
-        num_hidden_layers=12,
-        num_attention_heads=12,
-        intermediate_size=3072,
-        hidden_act="gelu",
-        hidden_dropout_prob=0.1,
-        attention_probs_dropout_prob=0.1,
-        max_position_embeddings=512,
-        type_vocab_size=6,
-        initializer_range=0.02,
-        layer_norm_eps=1e-12,
-        source_type_id=0,
-        target_type_id=1,
-        bos_token_id=101,
-        mask_token_id=103,
-        eos_token_id=102,
-        pad_token_id=0,
-        **kwargs,
-    ):
-        super().__init__(**kwargs)
-        self.bos_token_id = bos_token_id
-        self.mask_token_id = mask_token_id
-        self.eos_token_id = eos_token_id
-        self.pad_token_id = pad_token_id
-        self.hidden_size = hidden_size
-        self.num_hidden_layers = num_hidden_layers
-        self.num_attention_heads = num_attention_heads
-        self.hidden_act = hidden_act
-        self.intermediate_size = intermediate_size
-        self.hidden_dropout_prob = hidden_dropout_prob
-        self.attention_probs_dropout_prob = attention_probs_dropout_prob
-        self.max_position_embeddings = max_position_embeddings
-        self.type_vocab_size = type_vocab_size
-        self.initializer_range = initializer_range
-        self.layer_norm_eps = layer_norm_eps
-        self.source_type_id = source_type_id
-        self.target_type_id = target_type_id
-        self.use_cache = True
-
-        if isinstance(vocab_size, str) or (
-            sys.version_info[0] == 2 and isinstance(vocab_size, unicode)
-        ):
-            with open(vocab_size, "r", encoding="utf-8") as reader:
-                json_config = json.loads(reader.read())
-                for key, value in json_config.items():
-                    self.__dict__[key] = value
-        elif isinstance(vocab_size, int):
-            self.vocab_size = vocab_size
-        else:
-            raise ValueError(
-                "First argument must be either a vocabulary size (int)"
-                " or the path to a pretrained model config file (str)"
-            )
-
-
-class BertSelfAttention(nn.Module):
-    """
-    An optimized bert self attn to unilm for faster generation
-    """
-
-    def __init__(self, config):
-        super(BertSelfAttention, self).__init__()
-        if config.hidden_size % config.num_attention_heads != 0:
-            raise ValueError(
-                "The hidden size (%d) is not a multiple of the number of attention "
-                "heads (%d)" % (config.hidden_size, config.num_attention_heads)
-            )
-        self.output_attentions = config.output_attentions
+        config,
+        is_cross_attention=False,
+    ):
+        super().__init__(
+            config=config,
+            is_cross_attention=is_cross_attention,
+        )
 
-        self.num_attention_heads = config.num_attention_heads
-        self.attention_head_size = int(config.hidden_size / config.num_attention_heads)
-        self.all_head_size = self.num_attention_heads * self.attention_head_size
+    def forward(
+        self,
+        hidden_states,
+        attention_mask: Optional[torch.Tensor] = None,
+        head_mask=None,
+        encoder_hidden_states=None,
+        encoder_attention_mask: Optional[torch.Tensor] = None,
+        past_key_value=None,
+        output_attentions=False,
+    ):
+        mixed_query_layer = self.query(hidden_states)
 
-        self.query = nn.Linear(config.hidden_size, self.all_head_size)
-        self.key = nn.Linear(config.hidden_size, self.all_head_size)
-        self.value = nn.Linear(config.hidden_size, self.all_head_size)
+        # If this is instantiated as a cross-attention module, the keys
+        # and values come from an encoder; the attention mask needs to be
+        # such that the encoder's padding tokens are not attended to.
+        is_cross_attention = encoder_hidden_states is not None
+        bsz, tgt_len, embed_dim = hidden_states.size()
+        kv_bsz = bsz
+
+        if is_cross_attention and past_key_value is not None:
+            # reuse k,v, cross_attentions
+            key_layer = past_key_value[0]
+            value_layer = past_key_value[1]
+            kv_bsz = key_layer.size(0)
+            attention_mask = encoder_attention_mask
+        elif is_cross_attention:
+            key_layer = self.transpose_for_scores(self.key(encoder_hidden_states))
+            value_layer = self.transpose_for_scores(self.value(encoder_hidden_states))
+            attention_mask = encoder_attention_mask
+        elif past_key_value is not None:
+            key_layer = self.transpose_for_scores(self.key(hidden_states))
+            value_layer = self.transpose_for_scores(self.value(hidden_states))
+            key_layer = torch.cat([past_key_value[0], key_layer], dim=2)
+            value_layer = torch.cat([past_key_value[1], value_layer], dim=2)
+        else:
+            key_layer = self.transpose_for_scores(self.key(hidden_states))
+            value_layer = self.transpose_for_scores(self.value(hidden_states))
 
-        self.dropout = nn.Dropout(config.attention_probs_dropout_prob)
+        query_layer = self.transpose_for_scores(mixed_query_layer)
 
-    def transpose_for_scores(self, x):
-        new_x_shape = x.size()[:-1] + (
-            self.num_attention_heads,
-            self.attention_head_size,
-        )
-        x = x.view(*new_x_shape)
-        return x.permute(0, 2, 1, 3)
+        past_key_value = (key_layer, value_layer)
 
-    def forward(
-        self, hidden_states, attention_mask, head_mask=None, history_states=None
-    ):
-        """
-        Args:
-            - hidden_states: last layer output or embedding output
-            - attention_mask: mask for tokens per batch
-            - history_states: a optimized cache dict for beam search inference
-        Shape:
-            - hidden_states: (N, S + L, E) for training, (N, 2, E) for cached beam search inference
-            - history_states is a optimized cache dict for beam search inference
-                - past_prefix_key_layer: (N, S, E)
-                - past_prefix_value_layer: (N, S, E)
-                - past_key_layer: (N * B, L, E)
-                - past_value_layer: (N * B, L, E)
-            Note: S is the source sequence length, L is the target sequence length, N is the batch size, E is the embedding dimension, B is the beam size
-        """
-        new_query_layer = self.query(hidden_states)
-        new_key_layer = self.key(hidden_states)
-        new_value_layer = self.value(hidden_states)
-
-        past_prefix_key_layer = history_states.get("past_prefix_key_layer")
-        past_prefix_value_layer = history_states.get("past_prefix_value_layer")
-        past_key_layer = history_states.get("past_key_layer")
-        past_value_layer = history_states.get("past_value_layer")
-
-        query_layer = self.transpose_for_scores(new_query_layer)
-        key_layer = self.transpose_for_scores(new_key_layer)
-        value_layer = self.transpose_for_scores(new_value_layer)
-        if past_prefix_key_layer is not None:
-            prefix_size = past_prefix_key_layer.size()
-            prefix_attention_scores = torch.einsum(
+        # Take the dot product between "query" and "key" to get the raw attention scores.
+        attention_scores = torch.matmul(query_layer, key_layer.transpose(-1, -2))
+        if is_cross_attention and kv_bsz != bsz:
+            attention_scores = torch.einsum(
                 "bxhtd,bhsd->bxhts",
-                query_layer.view(prefix_size[0], -1, *query_layer.size()[1:]),
-                past_prefix_key_layer,
-            )
-            prefix_attention_scores = prefix_attention_scores.reshape(
-                -1, *prefix_attention_scores.size()[2:]
-            )
-            if past_key_layer is not None:
-                key_layer = torch.cat((past_key_layer, key_layer), dim=2)
-                value_layer = torch.cat((past_value_layer, value_layer), dim=2)
-            attention_scores = torch.matmul(
-                query_layer, key_layer.transpose(-1, -2)
-            )
-            prefix_attention_scores = prefix_attention_scores / math.sqrt(
-                self.attention_head_size
-            )
-            attention_scores = attention_scores / math.sqrt(
-                self.attention_head_size
+                query_layer.view(kv_bsz, -1, self.num_heads, *query_layer.size()[1:]),
+                key_layer.view(kv_bsz, self.num_heads, *key_layer.size()[1:]),
             )
-            attention_scores = torch.cat(
-                (prefix_attention_scores, attention_scores), dim=-1
+            attention_scores = attention_scores.reshape(
+                -1, *attention_scores.size()[-2:]
             )
-            attention_scores = attention_scores + attention_mask
-            attention_probs = nn.Softmax(dim=-1)(attention_scores)
-            attention_probs = self.dropout(attention_probs)
-
-            if head_mask is not None:
-                attention_probs = attention_probs * head_mask
-            prefix_attention_probs = attention_probs[:, :, :, : prefix_size[2]]
-            attention_probs = attention_probs[:, :, :, prefix_size[2] :]
-            prefix_attention_probs = prefix_attention_probs.to(past_prefix_value_layer.dtype)
-            prefix_context_layer = torch.einsum(
-                "bxhtd,bhds->bxhts",
-                prefix_attention_probs.view(
-                    prefix_size[0], -1, *prefix_attention_probs.size()[1:]
-                ),
-                past_prefix_value_layer,
-            )
-            prefix_context_layer = prefix_context_layer.reshape(
-                -1, *prefix_context_layer.size()[2:]
-            )
-            context_layer = torch.matmul(attention_probs, value_layer)
-            context_layer = prefix_context_layer + context_layer
-
         else:
             attention_scores = torch.matmul(query_layer, key_layer.transpose(-1, -2))
-            attention_scores = attention_scores / math.sqrt(self.attention_head_size)
-            attention_scores = attention_scores + attention_mask
 
-            attention_probs = nn.Softmax(dim=-1)(attention_scores)
-            attention_probs = self.dropout(attention_probs)
-
-            if head_mask is not None:
-                attention_probs = attention_probs * head_mask
-            context_layer = torch.matmul(attention_probs, value_layer)
-
-        if history_states is None or len(history_states) == 0:
-            history_states.update(
-                dict(
-                    {
-                        "past_prefix_key_layer": key_layer,
-                        "past_prefix_value_layer": value_layer,
-                    }
+        if (
+            self.position_embedding_type == "relative_key"
+            or self.position_embedding_type == "relative_key_query"
+        ):
+            seq_length = hidden_states.size()[1]
+            position_ids_l = torch.arange(
+                seq_length, dtype=torch.long, device=hidden_states.device
+            ).view(-1, 1)
+            position_ids_r = torch.arange(
+                seq_length, dtype=torch.long, device=hidden_states.device
+            ).view(1, -1)
+            distance = position_ids_l - position_ids_r
+            positional_embedding = self.distance_embedding(
+                distance + self.max_position_embeddings - 1
+            )
+            positional_embedding = positional_embedding.to(
+                dtype=query_layer.dtype
+            )  # fp16 compatibility
+
+            if self.position_embedding_type == "relative_key":
+                relative_position_scores = torch.einsum(
+                    "bhld,lrd->bhlr", query_layer, positional_embedding
                 )
-            )
-        else:
-            history_states.update(
-                dict(
-                    {
-                        "past_prefix_key_layer": past_prefix_key_layer,
-                        "past_prefix_value_layer": past_prefix_value_layer,
-                        "past_key_layer": key_layer[:, :, :-1, :],
-                        "past_value_layer": value_layer[:, :, :-1, :],
-                    }
+                attention_scores = attention_scores + relative_position_scores
+            elif self.position_embedding_type == "relative_key_query":
+                relative_position_scores_query = torch.einsum(
+                    "bhld,lrd->bhlr", query_layer, positional_embedding
+                )
+                relative_position_scores_key = torch.einsum(
+                    "bhrd,lrd->bhlr", key_layer, positional_embedding
                 )
+                if kv_bsz != bsz:
+                    shape = relative_position_scores_query.size()
+                    relative_position_scores_key = (
+                        relative_position_scores_key.unsqueeze(1)
+                        .expand(kv_bsz, bsz // kv_bsz, *shape[1:])
+                        .contiguous()
+                        .view(bsz, *shape[1:])
+                    )
+                attention_scores = (
+                    attention_scores
+                    + relative_position_scores_query
+                    + relative_position_scores_key
+                )
+
+        attention_scores = attention_scores / math.sqrt(self.attention_head_size)
+        if attention_mask is not None:
+            # Apply the attention mask is (precomputed for all layers in BlipTextModel forward() function)
+            attention_scores = attention_scores + attention_mask.to(
+                attention_scores.device
             )
 
+        # Normalize the attention scores to probabilities.
+        attention_probs = nn.Softmax(dim=-1)(attention_scores)
+
+        # This is actually dropping out entire tokens to attend to, which might
+        # seem a bit unusual, but is taken from the original Transformer paper.
+        attention_probs_dropped = self.dropout(attention_probs)
+
+        # Mask heads if we want to
+        if head_mask is not None:
+            attention_probs_dropped = attention_probs_dropped * head_mask
+
+        if is_cross_attention and kv_bsz != bsz:
+            context_layer = torch.einsum(
+                "bxhtd,bhsd->bxhts",
+                attention_probs_dropped.view(
+                    kv_bsz, -1, self.num_heads, *query_layer.size()[1:]
+                ),
+                value_layer.view(kv_bsz, self.num_heads, *key_layer.size()[1:]),
+            )
+            context_layer = context_layer.reshape(-1, *context_layer.size()[-2:])
+        else:
+            context_layer = torch.matmul(attention_probs_dropped, value_layer)
+
         context_layer = context_layer.permute(0, 2, 1, 3).contiguous()
         new_context_layer_shape = context_layer.size()[:-2] + (self.all_head_size,)
         context_layer = context_layer.view(*new_context_layer_shape)
 
         outputs = (
-            (context_layer, attention_probs)
-            if self.output_attentions
-            else (context_layer,)
+            (context_layer, attention_probs) if output_attentions else (context_layer,)
         )
+
+        outputs = outputs + (past_key_value,)
         return outputs
 
 
-class BertAttention(nn.Module):
-    """
-    Bert Attention from Unilm offical repo
-    https://github.com/microsoft/unilm/tree/master/s2s-ft
-    """
-
-    def __init__(self, config):
-        super(BertAttention, self).__init__()
-        self.self = BertSelfAttention(config)
-        self.output = BertSelfOutput(config)
-        self.pruned_heads = set()
-
-    def prune_heads(self, heads):
-        if len(heads) == 0:
-            return
-        mask = torch.ones(self.self.num_attention_heads, self.self.attention_head_size)
-        heads = (
-            set(heads) - self.pruned_heads
-        )  # Convert to set and emove already pruned heads
-        for head in heads:
-            # Compute how many pruned heads are before the head and move the index accordingly
-            head = head - sum(1 if h < head else 0 for h in self.pruned_heads)
-            mask[head] = 0
-        mask = mask.view(-1).contiguous().eq(1)
-        index = torch.arange(len(mask))[mask].long()
-
-        # Prune linear layers
-        self.self.query = prune_linear_layer(self.self.query, index)
-        self.self.key = prune_linear_layer(self.self.key, index)
-        self.self.value = prune_linear_layer(self.self.value, index)
-        self.output.dense = prune_linear_layer(self.output.dense, index, dim=1)
-
-        # Update hyper params and store pruned heads
-        self.self.num_attention_heads = self.self.num_attention_heads - len(heads)
-        self.self.all_head_size = (
-            self.self.attention_head_size * self.self.num_attention_heads
+@replace(transformers.models.blip.modeling_blip_text.BlipTextLayer)
+class BlipTextLayerV2(transformers.models.blip.modeling_blip_text.BlipTextLayer):
+    def __init__(self, config, layer_num):
+        super().__init__(
+            config=config,
+            layer_num=layer_num,
         )
-        self.pruned_heads = self.pruned_heads.union(heads)
 
     def forward(
-        self, input_tensor, attention_mask, head_mask=None, history_states=None
+        self,
+        hidden_states,
+        attention_mask: Optional[torch.Tensor] = None,
+        head_mask=None,
+        encoder_hidden_states=None,
+        encoder_attention_mask: Optional[torch.Tensor] = None,
+        past_key_value=None,
+        output_attentions=False,
     ):
-        self_outputs = self.self(
-            input_tensor, attention_mask, head_mask, history_states=history_states
+        # decoder uni-directional self-attention cached key/values tuple is at positions 1,2
+        self_attn_past_key_value = (
+            past_key_value[:2] if past_key_value is not None else None
+        )
+        self_attention_outputs = self.attention(
+            hidden_states,
+            attention_mask,
+            head_mask,
+            output_attentions=output_attentions,
+            past_key_value=self_attn_past_key_value,
+        )
+        attention_output = self_attention_outputs[0]
+
+        outputs = self_attention_outputs[1:-1]
+        present_key_value = self_attention_outputs[-1]
+
+        if encoder_hidden_states is not None:
+            cross_attn_past_key_value = (
+                past_key_value[2:] if past_key_value is not None else None
+            )
+            cross_attention_outputs = self.crossattention(
+                attention_output,
+                attention_mask,
+                head_mask,
+                encoder_hidden_states,
+                encoder_attention_mask,
+                output_attentions=output_attentions,
+                past_key_value=cross_attn_past_key_value,
+            )
+            attention_output = cross_attention_outputs[0]
+            outputs = (
+                outputs + cross_attention_outputs[1:-1]
+            )  # add cross attentions if we output attention weights
+            present_key_value = present_key_value + cross_attention_outputs[-1]
+
+        layer_output = apply_chunking_to_forward(
+            self.feed_forward_chunk,
+            self.chunk_size_feed_forward,
+            self.seq_len_dim,
+            attention_output,
         )
-        attention_output = self.output(self_outputs[0], input_tensor)
-        outputs = (attention_output,) + self_outputs[
-            1:
-        ]  # add attentions if we output them
+        outputs = (layer_output,) + outputs
+
+        outputs = outputs + (present_key_value,)
+
         return outputs
 
 
-class BertLayer(nn.Module):
-    """
-    Bert Layer from Unilm offical repo
-    https://github.com/microsoft/unilm/tree/master/s2s-ft
-    """
-
-    def __init__(self, config):
-        super(BertLayer, self).__init__()
-        self.attention = BertAttention(config)
-        self.intermediate = BertIntermediate(config)
-        self.output = BertOutput(config)
+class BlipForPretrain(GenericModel):
+    def __init__(
+        self,
+        config_path: str,
+        projection_dim: Optional[int] = 512,
+        freeze_base_model: Optional[bool] = True,
+        gradient_checkpointing: Optional[bool] = False,
+        use_all_gather: Optional[bool] = True,
+    ):
+        """
+        Initializes the BlipForPretrain model.
+
+        Args:
+            config_path (str): Path to the configuration file.
+            projection_dim (Optional[int], optional): Dimension of the projection. Defaults to 512.
+            freeze_base_model (Optional[bool], optional): Whether to freeze the base model. Defaults to True.
+            gradient_checkpointing (Optional[bool], optional): Whether to use gradient checkpointing. Defaults to False.
+            use_all_gather (Optional[bool], optional): Whether to use all_gather operation for distributed training. Defaults to True.
+        """
+        super().__init__()
+
+        config = BlipConfig.from_json_file(config_path)
+        text_config = config.text_config
+        vision_config = config.vision_config
+        text_config.gradient_checkpointing = gradient_checkpointing
+        vision_config.gradient_checkpointing = gradient_checkpointing
+
+        self.projection_dim = projection_dim
+        self.use_all_gather = use_all_gather
+
+        self.text_embed_dim = text_config.hidden_size
+        self.vision_embed_dim = vision_config.hidden_size
+
+        self.text_model = BlipTextModel(text_config)
+        self.vision_model = BlipVisionModel(vision_config)
+
+        self.visual_projection = nn.Linear(
+            self.vision_embed_dim,
+            self.projection_dim,
+            bias=False,
+        )
+        self.text_projection = nn.Linear(
+            self.text_embed_dim,
+            self.projection_dim,
+            bias=False,
+        )
+        self.logit_scale = nn.Parameter(torch.ones([]) * config.logit_scale_init_value)
+
+        self.init_weights()
+
+        if freeze_base_model:
+            for p in self.text_model.parameters():
+                p.requires_grad = False
+
+            for p in self.vision_model.parameters():
+                p.requires_grad = False
+
+        self.text_model.encoder.gradient_checkpointing = gradient_checkpointing
+        self.vision_model.encoder.gradient_checkpointing = gradient_checkpointing
+
+    def _all_gather(self, input):
+        """
+        Applies all_gather operation for distributed training.
+
+        Args:
+            input: Input tensor to gather.
+
+        Returns:
+            output: Gathered tensor across all workers.
+        """
+        output = AllGather.apply(input)
+        output = output.view(-1, *(output.shape[2:]))
+        return output
 
     def forward(
-        self, hidden_states, attention_mask, head_mask=None, history_states=None
+        self,
+        input_ids: torch.Tensor,
+        pixel_values: torch.Tensor,
+        attention_mask: torch.Tensor,
+        position_ids: torch.Tensor,
     ):
-        attention_outputs = self.attention(
-            hidden_states, attention_mask, head_mask, history_states=history_states
-        )
-        attention_output = attention_outputs[0]
-        intermediate_output = self.intermediate(attention_output)
-        layer_output = self.output(intermediate_output, attention_output)
-        outputs = (layer_output,) + attention_outputs[
-            1:
-        ]  # add attentions if we output them
-        return outputs
+        """
+        Forward pass of the BlipForPretrain model.
 
+        Args:
+            input_ids (torch.Tensor): Input token IDs.
+            pixel_values (torch.Tensor): Pixel values of the images.
+            attention_mask (torch.Tensor): Attention mask for the input.
+            position_ids (torch.Tensor): Position IDs for the input.
 
-class BertEncoder(nn.Module):
-    """
-    Bert Encoder from Unilm offical repo
-    https://github.com/microsoft/unilm/tree/master/s2s-ft
-    """
-
-    def __init__(self, config):
-        super(BertEncoder, self).__init__()
-        self.output_attentions = config.output_attentions
-        self.output_hidden_states = config.output_hidden_states
-        self.layer = nn.ModuleList(
-            [BertLayer(config) for _ in range(config.num_hidden_layers)]
+        Returns:
+            (torch.Tensor):Output loss for the pretraining task.
+        """
+        vision_outputs = self.vision_model(
+            pixel_values=pixel_values,
         )
 
-    def forward(
-        self, hidden_states, attention_mask, head_mask=None, history_states=None
+        text_outputs = self.text_model(
+            input_ids=input_ids,
+            attention_mask=attention_mask,
+            position_ids=position_ids,
+        )
+
+        image_embeds = vision_outputs[1]
+        image_embeds = self.visual_projection(image_embeds)
+
+        text_embeds = text_outputs[1]
+        text_embeds = self.text_projection(text_embeds)
+
+        # normalized features
+        image_embeds = image_embeds / image_embeds.norm(dim=-1, keepdim=True)
+        text_embeds = text_embeds / text_embeds.norm(dim=-1, keepdim=True)
+
+        logit_scale = self.logit_scale.exp()
+        if self.use_all_gather and dist.is_initialized():
+            text_embeds = self._all_gather(text_embeds)
+            image_embeds = self._all_gather(image_embeds)
+        logits_per_text = torch.matmul(text_embeds, image_embeds.t()) * logit_scale
+        return _blip_loss(logits_per_text)
+
+
+class BlipForClassification(nn.Module):
+    def __init__(
+        self,
+        config_path: str,
+        projection_dim: Optional[int] = 512,
+        num_classes: Optional[int] = 1,
+        freeze_base_model: Optional[bool] = True,
+        gradient_checkpointing: Optional[bool] = False,
     ):
-        all_hidden_states = ()
-        all_attentions = ()
+        """
+        Initializes the BlipForClassification model.
 
-        for i, layer_module in enumerate(self.layer):
-            layer_outputs = layer_module(
-                hidden_states,
-                attention_mask,
-                head_mask[i],
-                history_states=history_states[i],
-            )
+        Args:
+            config_path (str): Path to the configuration file.
+            projection_dim (Optional[int], optional): Dimension of the projection. Defaults to 512.
+            num_classes (Optional[int], optional): Number of classes for classification. Defaults to 1.
+            freeze_base_model (Optional[bool], optional): Whether to freeze the base model. Defaults to True.
+            gradient_checkpointing (Optional[bool], optional): Whether to use gradient checkpointing. Defaults to False.
+        """
+        super().__init__()
+
+        # Load the BLIP model configuration
+        config = BlipConfig.from_json_file(config_path)
+        text_config = config.text_config
+        vision_config = config.vision_config
+
+        # Set gradient checkpointing option
+        text_config.gradient_checkpointing = gradient_checkpointing
+        vision_config.gradient_checkpointing = gradient_checkpointing
+
+        self.projection_dim = projection_dim
 
-            if self.output_hidden_states:
-                all_hidden_states = all_hidden_states + (hidden_states,)
+        self.text_embed_dim = text_config.hidden_size
+        self.vision_embed_dim = vision_config.hidden_size
 
-            hidden_states = layer_outputs[0]
-            if self.output_attentions:
-                all_attentions = all_attentions + (layer_outputs[1],)
-
-        # Add last layer
-        if self.output_hidden_states:
-            all_hidden_states = all_hidden_states + (hidden_states,)
-
-        outputs = (hidden_states,)
-        if self.output_hidden_states:
-            outputs = outputs + (all_hidden_states,)
-        if self.output_attentions:
-            outputs = outputs + (all_attentions,)
-        return outputs  # last-layer hidden state, (all hidden states), (all attentions), (all encoder layers)
-
-
-class UnilmModel(BertPreTrainedModel):
-    """
-    Unilm model structure
-    """
-
-    def __init__(self, config):
-        super().__init__(config)
-
-        self.embeddings = BertEmbeddings(config)
-        self.encoder = BertEncoder(config)
-        self.pooler = BertPooler(config)
+        # Initialize the text and vision models
+        self.text_model = BlipTextModel(text_config)
+        self.vision_model = BlipVisionModel(vision_config)
 
+        # Projection layers for text and vision embeddings
+        self.visual_projection = nn.Linear(
+            self.vision_embed_dim,
+            self.projection_dim,
+            bias=False,
+        )
+        self.text_projection = nn.Linear(
+            self.text_embed_dim,
+            self.projection_dim,
+            bias=False,
+        )
+
+        # Classifier layer
+        self.classifier = nn.Linear(self.projection_dim * 2, num_classes)
+
+        # Initialize the weights of the model
         self.init_weights()
 
-    def _resize_token_embeddings(self, new_num_tokens):
-        old_embeddings = self.embeddings.word_embeddings
-        new_embeddings = self._get_resized_embeddings(old_embeddings, new_num_tokens)
-        self.embeddings.word_embeddings = new_embeddings
-        return self.embeddings.word_embeddings
-
-    def _prune_heads(self, heads_to_prune):
-        """Prunes heads of the model.
-        heads_to_prune: dict of {layer_num: list of heads to prune in this layer}
-        See base class PreTrainedModel
-        """
-        for layer, heads in heads_to_prune.items():
-            self.encoder.layer[layer].attention.prune_heads(heads)
+        if freeze_base_model:
+            # Freeze the parameters of the base models if specified
+            for p in self.text_model.parameters():
+                p.requires_grad = False
+
+            for p in self.vision_model.parameters():
+                p.requires_grad = False
+
+        # Set gradient checkpointing option for encoders
+        self.text_model.encoder.gradient_checkpointing = gradient_checkpointing
+        self.vision_model.encoder.gradient_checkpointing = gradient_checkpointing
 
     def forward(
         self,
-        input_ids,
-        token_type_ids=None,
-        attention_mask=None,
-        position_ids=None,
-        head_mask=None,
-        history_states=None,
+        input_ids: torch.Tensor,
+        pixel_values: torch.Tensor,
+        attention_mask: torch.Tensor,
+        position_ids: torch.Tensor,
     ):
-        if attention_mask is None:
-            attention_mask = torch.ones_like(input_ids)
-        if token_type_ids is None:
-            token_type_ids = torch.zeros_like(input_ids)
-
-        # We create a 3D attention mask from a 2D tensor mask.
-        # Sizes are [batch_size, 1, 1, to_seq_length]
-        # So we can broadcast to [batch_size, num_heads, from_seq_length, to_seq_length]
-        # this attention mask is more simple than the triangular masking of causal attention
-        # used in OpenAI GPT, we just need to prepare the broadcast dimension here.
-        if attention_mask.dim() == 2:
-            extended_attention_mask = attention_mask.unsqueeze(1).unsqueeze(2)
-        elif attention_mask.dim() == 3:
-            extended_attention_mask = attention_mask.unsqueeze(1)
-        else:
-            raise NotImplementedError
+        """
+        Forward pass of the BlipForClassification model.
 
-        # Since attention_mask is 1.0 for positions we want to attend and 0.0 for
-        # masked positions, this operation will create a tensor which is 0.0 for
-        # positions we want to attend and -10000.0 for masked positions.
-        # Since we are adding it to the raw scores before the softmax, this is
-        # effectively the same as removing these entirely.
-        extended_attention_mask = extended_attention_mask.to(
-            dtype=next(self.parameters()).dtype
-        )  # fp16 compatibility
-        extended_attention_mask = (1.0 - extended_attention_mask) * -10000.0
-
-        # Prepare head mask if needed
-        # 1.0 in head_mask indicate we keep the head
-        # attention_probs has shape bsz x n_heads x N x N
-        # input head_mask has shape [num_heads] or [num_hidden_layers x num_heads]
-        # and head_mask is converted to shape [num_hidden_layers x batch x num_heads x seq_length x seq_length]
-        if head_mask is not None:
-            if head_mask.dim() == 1:
-                head_mask = (
-                    head_mask.unsqueeze(0).unsqueeze(0).unsqueeze(-1).unsqueeze(-1)
-                )
-                head_mask = head_mask.expand(
-                    self.config.num_hidden_layers, -1, -1, -1, -1
-                )
-            elif head_mask.dim() == 2:
-                head_mask = (
-                    head_mask.unsqueeze(1).unsqueeze(-1).unsqueeze(-1)
-                )  # We can specify head_mask for each layer
-            head_mask = head_mask.to(
-                dtype=next(self.parameters()).dtype
-            )  # switch to fload if need + fp16 compatibility
-        else:
-            head_mask = [None] * self.config.num_hidden_layers
+        Args:
+            input_ids (torch.Tensor): Input token IDs.
+            pixel_values (torch.Tensor): Pixel values of the images.
+            attention_mask (torch.Tensor): Attention mask for the input.
+            position_ids (torch.Tensor): Position IDs for the input.
 
-        if history_states is None:
-            history_states = [
-                dict().copy() for _ in range(self.config.num_hidden_layers)
-            ]
-        embedding_output = self.embeddings(
-            input_ids, position_ids=position_ids, token_type_ids=token_type_ids
-        )
-        encoder_outputs = self.encoder(
-            embedding_output,
-            extended_attention_mask,
-            head_mask=head_mask,
-            history_states=history_states,
+        Returns:
+            (torch.Tensor):Output logits for classification.
+        """
+        # Process the vision modality
+        vision_outputs = self.vision_model(
+            pixel_values=pixel_values,
         )
-        sequence_output = encoder_outputs[0]
-        pooled_output = self.pooler(sequence_output)
 
-        outputs = (
-            (
-                sequence_output,
-                pooled_output,
-            )
-            + encoder_outputs[1:]
-            + (history_states,)
-        )  # add hidden_states and attentions if they are here
-        return outputs  # sequence_output, pooled_output, (hidden_states), (attentions), (history_states)
+        # Process the text modality
+        text_outputs = self.text_model(
+            input_ids=input_ids,
+            attention_mask=attention_mask,
+            position_ids=position_ids,
+        )
+
+        # Project vision embeddings to the specified dimensionality
+        image_embeds = vision_outputs[1]
+        image_embeds = self.visual_projection(image_embeds)
 
+        # Project text embeddings to the specified dimensionality
+        text_embeds = text_outputs[1]
+        text_embeds = self.text_projection(text_embeds)
 
-class Unilm(core_model_class):
-    def __init__(self, config_path, **kwargs):
+        # Concatenate and classify the projected embeddings
+        return self.classifier(F.relu(torch.cat([image_embeds, text_embeds], axis=1)))
+
+
+class BlipForTextClassification(GenericModel):
+    def __init__(
+        self,
+        config_path: str,
+        projection_dim: Optional[int] = 512,
+        num_classes: Optional[int] = 1,
+        freeze_base_model: Optional[bool] = True,
+        gradient_checkpointing: Optional[bool] = False,
+    ):
+        """
+        Initializes the BlipForTextClassification model.
+
+        Args:
+            config_path (str): Path to the configuration file.
+            projection_dim (Optional[int], optional): Dimension of the projection. Defaults to 512.
+            num_classes (Optional[int], optional): Number of classes for classification. Defaults to 1.
+            freeze_base_model (Optional[bool], optional): Whether to freeze the base model. Defaults to True.
+            gradient_checkpointing (Optional[bool], optional): Whether to use gradient checkpointing. Defaults to False.
+        """
         super().__init__()
-        self.config_path = config_path
-        self.config = UnilmConfig(config_path)
 
-    @classmethod
-    def init_from_core_configure(cls, cfg, **kwargs):
-        pass
-
-    def save_checkpoint(self, ckpt_dir="./cache", **kwargs):
-        if not os.path.exists(ckpt_dir):
-            os.mkdir(ckpt_dir)
-        config_path = os.path.join(ckpt_dir, CONFIG_NAME)
-        with open(config_path, "w") as f:
-            f.write(open(self.config_path, "r").read())
-
-        super().save_checkpoint(ckpt_dir=ckpt_dir, **kwargs)
-
-    def from_checkpoint(self, ckpt_dir="./cache", **kwargs):
-        super().from_checkpoint(ckpt_dir=ckpt_dir, **kwargs)
-
-
-@register_model("core/model/unilm_for_generation", generation_model_decorator)
-class UnilmForGeneration(Unilm, GenerationMixinV2):
-    def __init__(self, config_path):
-        super().__init__(config_path)
-        self.bert = UnilmModel(self.config)
-        self.cls = BertPreTrainingHeads(self.config)
-        self.init_weights()
+        # Load the BLIP model configuration
+        config = BlipConfig.from_json_file(config_path)
+        text_config = config.text_config
+        text_config.gradient_checkpointing = gradient_checkpointing
+
+        self.projection_dim = projection_dim
+        self.text_embed_dim = text_config.hidden_size
 
-        self.hist_index = (
-            int(self.config.output_hidden_states)
-            + int(self.config.output_attentions)
-            + 2
+        # Initialize the BLIP text model
+        self.text_model = BlipTextModel(text_config)
+
+        # Project text embeddings to the desired dimension
+        self.text_projection = nn.Linear(
+            self.text_embed_dim,
+            self.projection_dim,
+            bias=False,
         )
-        self.bert.embeddings.word_embeddings.weight = (
-            self.cls.predictions.decoder.weight
+
+        # Classifier layer for classification task
+        self.classifier = nn.Linear(self.projection_dim, num_classes)
+
+        # Initialize the model weights
+        self.init_weights()
+
+        # Freeze the base model if specified
+        if freeze_base_model:
+            for p in self.text_model.parameters():
+                p.requires_grad = False
+
+        # Set gradient checkpointing for the encoder
+        self.text_model.encoder.gradient_checkpointing = gradient_checkpointing
+
+    def forward(
+        self,
+        input_ids: torch.Tensor,
+        attention_mask: torch.Tensor,
+        position_ids: torch.Tensor,
+    ):
+        """
+        Forward pass of the BlipForTextClassification model.
+
+        Args:
+            input_ids (torch.Tensor): Input token IDs.
+            attention_mask (torch.Tensor): Attention mask for the input.
+            position_ids (torch.Tensor): Position IDs for the input.
+
+        Returns:
+            (torch.Tensor):Output logits for classification.
+        """
+        # Pass the input through the BLIP text model
+        text_outputs = self.text_model(
+            input_ids=input_ids,
+            attention_mask=attention_mask,
+            position_ids=position_ids,
         )
 
-    @property
-    def device(self) -> device:
+        # Extract text embeddings and project to desired dimension
+        text_embeds = text_outputs[1]
+        text_embeds = self.text_projection(text_embeds)
+
+        # Apply ReLU activation and pass through the classifier layer
+        return self.classifier(nn.functional.relu(text_embeds))
+
+
+class BlipForImageClassification(GenericModel):
+    def __init__(
+        self,
+        config_path: str,
+        projection_dim: Optional[int] = 512,
+        num_classes: Optional[int] = 1,
+        freeze_base_model: Optional[bool] = True,
+        gradient_checkpointing: Optional[bool] = False,
+    ):
         """
-        :obj:`torch.device`: The device on which the module is (assuming that all the module parameters are on the same
-        device).
+        Initializes the BlipForImageClassification model.
+
+        Args:
+            config_path (str): Path to the configuration file.
+            projection_dim (Optional[int], optional): Dimension of the projection. Defaults to 512.
+            num_classes (Optional[int], optional): Number of classes for classification. Defaults to 1.
+            freeze_base_model (Optional[bool], optional): Whether to freeze the base model. Defaults to True.
+            gradient_checkpointing (Optional[bool], optional): Whether to use gradient checkpointing. Defaults to False.
         """
-        try:
-            return next(self.parameters()).device
-        except StopIteration:
-            # For nn.DataParallel compatibility in PyTorch 1.5
+        super().__init__()
 
-            def find_tensor_attributes(module: nn.Module) -> List[Tuple[str, Tensor]]:
-                tuples = [
-                    (k, v) for k, v in module.__dict__.items() if torch.is_tensor(v)
-                ]
-                return tuples
+        # Load the BLIP model configuration
+        config = BlipConfig.from_json_file(config_path)
+        vision_config = config.vision_config
+        vision_config.gradient_checkpointing = gradient_checkpointing
 
-            gen = self._named_members(get_members_fn=find_tensor_attributes)
-            first_tuple = next(gen)
-            return first_tuple[1].device
+        self.projection_dim = projection_dim
+        self.vision_embed_dim = vision_config.hidden_size
 
-    @classmethod
-    @add_default_section_for_init("core/model/unilm")
-    def init_from_core_configure(cls, cfg, **kwargs):
-        pretrained_name = cfg.getdefault(
-            "core/model/unilm", "pretrained_name", "default-unilm"
-        )
-        config_name_or_path = cfg.getdefault(
-            "core/model/unilm", "config_name_or_path", pretrained_name
+        self.vision_model = BlipVisionModel(vision_config)
+
+        self.visual_projection = nn.Linear(
+            self.vision_embed_dim,
+            self.projection_dim,
+            bias=False,
         )
-        config_path = (
-            CORE_UNILM_PRETRAINED_DICT[config_name_or_path][CONFIG_KEY]
-            if config_name_or_path in CORE_UNILM_PRETRAINED_DICT
-            else config_name_or_path
+
+        self.classifier = nn.Linear(self.projection_dim, num_classes)
+
+        self.init_weights()
+
+        if freeze_base_model:
+            for p in self.vision_model.parameters():
+                p.requires_grad = False
+
+        self.vision_model.encoder.gradient_checkpointing = gradient_checkpointing
+
+    def forward(
+        self,
+        pixel_values: torch.Tensor,
+    ):
+        """
+        Forward pass of the BlipForImageClassification model.
+
+        Args:
+            pixel_values (torch.Tensor): Input pixel values.
+
+        Returns:
+            (torch.Tensor):Output logits for classification.
+        """
+        vision_outputs = self.vision_model(
+            pixel_values=pixel_values,
         )
 
-        config_path = hf_cached_path(config_path)
-        inst = cls(config_path)
+        image_embeds = vision_outputs[1]
+
+        image_embeds = self.visual_projection(image_embeds)
+
+        image_embeds = F.relu(image_embeds)
+
+        return self.classifier(image_embeds)
 
-        if pretrained_name is not None:
-            inst.from_pretrained(pretrained_name)
 
-        return inst
+class BlipForImageCaption(GenericModel):
+    prefix_keys_in_state_dict = {"^(?!model\.).*": "model."}
+
+    def __init__(
+        self,
+        config_path: str,
+        gradient_checkpointing: Optional[bool] = False,
+    ):
+        """
+        Initializes the BlipForImageCaption model.
+
+        Args:
+            config_path (str): Path to the configuration file.
+            gradient_checkpointing (Optional[bool], optional): Whether to use gradient checkpointing. Defaults to False.
+        """
+        super().__init__()
+        self.config = BlipConfig.from_json_file(config_path)
+        self.config.vision_config.gradient_checkpointing = gradient_checkpointing
+        self.config.text_config.gradient_checkpointing = gradient_checkpointing
+        self.model = BlipForConditionalGeneration(self.config)
+        self.init_weights()
 
     def forward(
         self,
-        tokens_ids=None,
-        attn_mask=None,
-        seg_ids=None,
-        pos_ids=None,
-        decoder_input_ids=None,
-        decoder_pos_ids=None,
-        decoder_seg_ids=None,
-        decoder_attn_mask=None,
-        decoder_mask_ids=None,
-        past_key_values=None,
-        output_attentions=None,
-        output_hidden_states=None,
-        return_dict=None,
-    ):
-        if self.training:
-            outputs = self.bert(
-                tokens_ids,
-                seg_ids,
-                attn_mask,
-                pos_ids,
-            )
-            logits = self.cls(outputs[0], outputs[1])[0]
-            return logits
-        decoder_token = torch.cat([decoder_input_ids, decoder_mask_ids], dim=1)
-        decoder_len = decoder_token.size(1)
-        decoder_token = decoder_token[:, -2:]
-        decoder_mask = decoder_attn_mask[
-            :, decoder_len - 2 : decoder_len, : self.prefix_state["prefix_len"] + decoder_len
-        ]
-        decoder_pos = decoder_pos_ids[:, decoder_len - 2 : decoder_len]
-        outputs = self.bert(
-            decoder_token,
-            decoder_seg_ids,
-            decoder_mask,
-            decoder_pos,
-            history_states=past_key_values,
-        )
-        logits = self.cls(outputs[0], outputs[1])[0]
-        state4cache = [
-            decoder_pos_ids,
-            decoder_attn_mask,
-            decoder_mask_ids,
-            decoder_seg_ids,
-        ] + outputs[self.hist_index]
-        return Seq2SeqLMOutput(logits=logits, past_key_values=state4cache)
-
-    @staticmethod
-    def _reorder_cache(past, beam_idx):
-        """
-        For beam search in huggingface generation mixin
-        """
-        pos_ids, token_mask, decoder_mask_token, decoder_seg, history_states = (
-            past[0],
-            past[1],
-            past[2],
-            past[3],
-            past[4:],
-        )
-        reordered_past = []
-        for layer_past in history_states:
-            reordered_past.append(_reorder_buffer(layer_past, beam_idx))
-        newpast = [pos_ids, token_mask, decoder_mask_token, decoder_seg] + reordered_past
-        return newpast
-
-    @staticmethod
-    def _reorder_cache_v2(past, batch_idx, beam_idx):
-        """
-        For faster inference by optimized beam search in generation mixin v2
-        """
-        pos_ids, token_mask, decoder_mask_token, decoder_seg, history_states = (
-            past[0],
-            past[1],
-            past[2],
-            past[3],
-            past[4:],
-        )
-        reordered_past = []
-        for layer_past in history_states:
-            reordered_past.append(_reorder_buffer_v2(layer_past, batch_idx, beam_idx))
-        pos_ids = pos_ids[beam_idx]
-        token_mask = token_mask[beam_idx]
-        decoder_mask_token = decoder_mask_token[beam_idx]
-        decoder_seg = decoder_seg[beam_idx]
-        newpast = [pos_ids, token_mask, decoder_mask_token, decoder_seg] + reordered_past
-        return newpast
-
-    def prepare_inputs_for_generation(
-        self,
-        decoder_input_ids,
-        past=None,
-        **kwargs,
-    ):
-        if past is None:
-            active_batch_size, _ = decoder_input_ids.size()
-            prefix_token, prefix_seg, prefix_pos, prefix_mask = (
-                self.prefix_state["prefix_token"],
-                self.prefix_state["prefix_seg"],
-                self.prefix_state["prefix_pos"],
-                self.prefix_state["prefix_mask"],
-            )
-            prefix_len = self.prefix_state["prefix_len"]
-            outputs = self.bert(
-                prefix_token[:, :prefix_len],
-                prefix_seg[:, :prefix_len],
-                prefix_mask[:, :prefix_len, :prefix_len],
-                prefix_pos[:, :prefix_len],
-            )
-            token_pos = prefix_pos.repeat(1, self.num_beams).view(
-                active_batch_size, prefix_pos.size(1)
-            )
-            token_pos = token_pos[:, prefix_len:]
-            token_mask = (
-                prefix_mask.unsqueeze(1)
-                .repeat(1, self.num_beams, 1, 1)
-                .view(active_batch_size, prefix_mask.size(1), prefix_mask.size(1))
-            )
-            token_mask = token_mask[:, prefix_len:, :]
-            history_states = outputs[self.hist_index]
-            decoder_mask_token = (
-                torch.ones(active_batch_size, 1).to(decoder_input_ids)
-                * self.config.mask_token_id
-            )
-            decoder_seg_ids = (
-                torch.ones(active_batch_size, 2).to(decoder_input_ids)
-                * self.config.target_type_id
-            )
-        else:
-            token_pos, token_mask, decoder_mask_token, decoder_seg_ids, history_states = (
-                past[0],
-                past[1],
-                past[2],
-                past[3],
-                past[4:],
-            )
-        return {
-            "decoder_input_ids": decoder_input_ids,
-            "decoder_mask_ids": decoder_mask_token,
-            "decoder_attn_mask": token_mask,
-            "decoder_seg_ids": decoder_seg_ids,
-            "decoder_pos_ids": token_pos,
-            "past_key_values": history_states,
-        }
+        pixel_values: torch.Tensor,
+        input_ids: Optional[torch.Tensor] = None,
+        attention_mask: Optional[torch.Tensor] = None,
+    ):
+        """
+        Forward pass of the BlipForImageCaption model.
+
+        Args:
+            pixel_values (torch.Tensor): Input pixel values.
+            input_ids (Optional[torch.Tensor], optional): Input token IDs. Defaults to None.
+            attention_mask (Optional[torch.Tensor], optional): Attention mask. Defaults to None.
+
+        Returns:
+            (torch.Tensor):Logits for caption generation.
+        """
+        outputs = self.model(
+            pixel_values=pixel_values,
+            input_ids=input_ids,
+            attention_mask=attention_mask,
+            return_dict=True,
+        )
+        logits = outputs.decoder_logits
+        return logits
 
-    @add_default_section_for_instance_function("core/model/unilm")
+    @torch.no_grad()
     def generate(
         self,
-        tokens_ids,
-        num_beams=5,
-        decoder_start_token_id=101,
-        decoder_end_token_id=102,
-        num_return_sequences=1,
-        min_gen_seq_length=0,
-        max_gen_seq_length=48,
-        repetition_penalty=1.0,
-        no_repeat_ngram_size=0,
-        early_stopping=True,
-        length_penalty=1.0,
-        num_beam_groups=1,
-        diversity_penalty=0.0,
-        diverse_rate=0.0,
-    ):
-        self.num_beams = num_beams
-        prefix_token = tokens_ids
-        prefix_mask1 = tokens_ids.ne(self.config.pad_token_id).long()
-        batch_size, prefix_len = prefix_token.size()
-        total_seq_length = max_gen_seq_length + prefix_len + 1
-        prefix_mask = prefix_mask1[:, None, :].repeat(1, total_seq_length, 1)
-        new_mask = torch.zeros(batch_size, total_seq_length, max_gen_seq_length + 1).to(
-            prefix_mask
-        )
-        tri_mask = torch.ones(batch_size, total_seq_length, max_gen_seq_length + 1).to(
-            prefix_mask
-        )
-        new_mask[:, prefix_len:, :] = torch.tril(tri_mask[:, prefix_len:, :])
-        new_mask[:, :, 0] = 0
-        prefix_mask = torch.cat((prefix_mask, new_mask), dim=-1)
-        prefix_seg = torch.tensor([0] * prefix_len).to(prefix_token)
-        prefix_seg = prefix_seg[None, :].repeat(batch_size, 1)
-        prefix_pos0 = torch.ones(batch_size, max_gen_seq_length + 1).to(tokens_ids)
-        prefix_pos0[:, 0] = 0
-        prefix_pos = torch.cat((tokens_ids, prefix_pos0.to(tokens_ids)), dim=-1).ne(
-            self.config.pad_token_id
-        )
-        prefix_pos = torch.cumsum(prefix_pos, dim=-1) - 1
-        self.prefix_state = dict(
-            {
-                "prefix_len": prefix_len,
-                "prefix_token": prefix_token,
-                "prefix_seg": prefix_seg,
-                "prefix_mask": prefix_mask,
-                "prefix_pos": prefix_pos,
-            }
-        )
-        decoder_seg = torch.ones(batch_size * self.num_beams, 1).to(prefix_token)
-        decoder_seg[:, 0] = 0
-        decoder_mask_token = torch.ones(batch_size * self.num_beams, 1).to(prefix_token) * self.config.mask_token_id
-        if decoder_start_token_id is not None:
-            self.config.bos_token_id = decoder_start_token_id
-        decoder_input_ids = torch.ones(batch_size, 1).to(prefix_token) * self.config.bos_token_id
-        batch_hyp = super().generate(
-            decoder_input_ids,
-            max_length=max_gen_seq_length - 1,
+        pixel_values: torch.Tensor,
+        input_ids: Optional[torch.Tensor] = None,
+        attention_mask: Optional[torch.Tensor] = None,
+        num_beams: Optional[int] = 5,
+        decoder_start_token_id: Optional[int] = 101,
+        decoder_end_token_id: Optional[int] = 102,
+        num_return_sequences: Optional[int] = 1,
+        min_gen_seq_length: Optional[int] = 0,
+        max_gen_seq_length: Optional[int] = 48,
+        repetition_penalty: Optional[float] = 1.0,
+        no_repeat_ngram_size: Optional[int] = 0,
+        early_stopping: Optional[bool] = True,
+        length_penalty: Optional[float] = 1.0,
+        num_beam_groups: Optional[int] = 1,
+        diversity_penalty: Optional[float] = 0.0,
+        do_sample: Optional[bool] = False,
+        temperature: Optional[float] = 1.0,
+        top_k: Optional[int] = 50,
+        top_p: Optional[float] = 1.0,
+    ):
+        """
+        Generates captions for the given input images.
+
+        Args:
+            pixel_values (torch.Tensor): Input pixel values.
+            input_ids (Optional[torch.Tensor], optional): Input token IDs. Defaults to None.
+            attention_mask (Optional[torch.Tensor], optional): Attention mask. Defaults to None.
+            num_beams (Optional[int], optional): Number of beams for beam search. Defaults to 5.
+            decoder_start_token_id (Optional[int], optional): ID of the start token for decoding. Defaults to 30522.
+            decoder_end_token_id (Optional[int], optional): ID of the end token for decoding. Defaults to 2.
+            num_return_sequences (Optional[int], optional): Number of caption sequences to return. Defaults to 1.
+            min_gen_seq_length (Optional[int], optional): Minimum length of generated sequences. Defaults to 0.
+            max_gen_seq_length (Optional[int], optional): Maximum length of generated sequences. Defaults to 48.
+            repetition_penalty (Optional[float], optional): Repetition penalty value. Defaults to 1.0.
+            no_repeat_ngram_size (Optional[int], optional): Size of n-grams to avoid repetition. Defaults to 0.
+            early_stopping (Optional[bool], optional): Whether to stop generation early. Defaults to True.
+            length_penalty (Optional[float], optional): Length penalty value. Defaults to 1.0.
+            num_beam_groups (Optional[int], optional): Number of groups for diverse beam search. Defaults to 1.
+            diversity_penalty (Optional[float], optional): Diversity penalty value. Defaults to 0.0.
+            do_sample (Optional[bool], optional): Whether to use sampling for generation. Defaults to False.
+            temperature (Optional[float], optional): Temperature value for sampling. Defaults to 1.0.
+            top_k (Optional[int], optional): Value of k for top-k sampling. Defaults to 50.
+            top_p (Optional[float], optional): Value of p for top-p sampling. Defaults to 1.0.
+
+        Returns:
+            GenericOutputs: Generated caption sequences and their scores.
+        """
+        outputs = self.model.generate(
+            pixel_values=pixel_values,
+            input_ids=input_ids,
+            attention_mask=attention_mask,
+            max_length=max_gen_seq_length,
             min_length=min_gen_seq_length,
             num_beams=num_beams,
-            do_sample=False,
+            do_sample=do_sample,
             decoder_start_token_id=decoder_start_token_id,
             no_repeat_ngram_size=no_repeat_ngram_size,
             early_stopping=early_stopping,
             length_penalty=length_penalty,
             repetition_penalty=repetition_penalty,
             num_return_sequences=num_return_sequences,
             bos_token_id=decoder_start_token_id,
-            eos_token_id=decoder_end_token_id,
             num_beam_groups=num_beam_groups,
             diversity_penalty=diversity_penalty,
+            temperature=temperature,
+            top_k=top_k,
+            top_p=top_p,
+            return_dict_in_generate=True,
+            output_scores=True,
+        )
+
+        sequences = outputs.sequences.reshape(
+            -1, num_return_sequences, outputs.sequences.size(-1)
+        )
+        outputs.sequences = torch.zeros(
+            sequences.size(0), num_return_sequences, max_gen_seq_length
+        ).to(device=sequences.device)
+        outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)
+
+        if num_return_sequences == 1:
+            outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)
+
+        return GenericOutputs(
+            sequences=outputs.sequences, sequences_scores=outputs.sequences_scores
         )
-        batch_hyp = batch_hyp.reshape(-1, num_return_sequences, batch_hyp.size(-1))
-        if batch_hyp.size(-1) >= max_gen_seq_length:
-            return batch_hyp[:, :, :max_gen_seq_length].long()
-        batch_ret = torch.zeros(
-            batch_hyp.size(0), num_return_sequences, max_gen_seq_length
-        )
-        batch_ret[:, :, : batch_hyp.size(-1)].copy_(batch_hyp)
-        return batch_ret.long()
```

### Comparing `unitorch-0.0.0.1/unitorch/generation/bart.py` & `unitorch-0.0.0.2/src/unitorch/models/mbart/modeling.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,35 @@
+# Copyright (c) FULIUCANSHENG.
+# Licensed under the MIT License.
+
 import os
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
-from torch import device
+import logging
 import json
 import torch
+import logging
 import torch.nn as nn
 import torch.nn.functional as F
-from transformers import BartModel, BartConfig
-from transformers.models.bart.modeling_bart import (
-    BartAttention,
-    BartEncoder,
-    BartDecoder,
-)
-from unitorch.modules.generation_mixin_v2 import GenerationMixinV2
-from transformers.modeling_outputs import Seq2SeqLMOutput
-from unitorch import add_core_pretrained_dict, register_model
-from unitorch.utils.decorators import (
-    generation_model_decorator,
-    add_net_outputs_for_core_model,
-    add_default_section_for_init,
-    add_default_section_for_instance_function,
-    replace,
-)
-from unitorch.core import core_model_class
-from unitorch.utils.hf import hf_cached_path
-
-CONFIG_KEY = "config"
-CONFIG_NAME = "config.json"
-
-MERGES_KEY = "merge"
-MERGES_NAME = "merge.txt"
-
-VOCABS_KEY = "vocab"
-VOCABS_NAME = "vocab.json"
-
-CORE_BART_PRETRAINED_DICT = {
-    "default-bart": {
-        "config": "https://huggingface.co/facebook/bart-base/resolve/main/config.json",
-        "vocab": "https://huggingface.co/facebook/bart-base/resolve/main/vocab.json",
-        "merge": "https://huggingface.co/facebook/bart-base/resolve/main/merges.txt",
-    },
-    "bart-base": {
-        "config": "https://huggingface.co/facebook/bart-base/resolve/main/config.json",
-        "vocab": "https://huggingface.co/facebook/bart-base/resolve/main/vocab.json",
-        "merge": "https://huggingface.co/facebook/bart-base/resolve/main/merges.txt",
-        "weight": "https://huggingface.co/facebook/bart-base/resolve/main/pytorch_model.bin",
-    },
-    "bart-large": {
-        "config": "https://huggingface.co/facebook/bart-large/resolve/main/config.json",
-        "vocab": "https://huggingface.co/facebook/bart-large/resolve/main/vocab.json",
-        "merge": "https://huggingface.co/facebook/bart-large/resolve/main/merges.txt",
-        "weight": "https://huggingface.co/facebook/bart-large/resolve/main/pytorch_model.bin",
-    },
-}
-
-add_core_pretrained_dict(CORE_BART_PRETRAINED_DICT)
+import transformers
+from transformers.utils import is_remote_url
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
+from transformers import MBartConfig, MBartModel, MBartForConditionalGeneration
+from unitorch import hf_cached_path
+from unitorch.utils.decorators import replace
+from unitorch.models import GenericModel, GenericOutputs
 
 
-@replace(BartAttention)
-class BartAttentionV2(BartAttention):
+@replace(transformers.models.mbart.modeling_mbart.MBartAttention)
+class MBartAttentionV2(transformers.models.mbart.modeling_mbart.MBartAttention):
     def __init__(
         self,
         embed_dim: int,
         num_heads: int,
-        dropout: float = 0.0,
-        is_decoder: bool = False,
-        bias: bool = True,
+        dropout: Optional[float] = 0.0,
+        is_decoder: Optional[bool] = False,
+        bias: Optional[bool] = True,
     ):
         super().__init__(
             embed_dim=embed_dim,
             num_heads=num_heads,
             dropout=dropout,
             is_decoder=is_decoder,
             bias=bias,
@@ -77,15 +38,15 @@
     def forward(
         self,
         hidden_states: torch.Tensor,
         key_value_states: Optional[torch.Tensor] = None,
         past_key_value: Optional[Tuple[torch.Tensor]] = None,
         attention_mask: Optional[torch.Tensor] = None,
         layer_head_mask: Optional[torch.Tensor] = None,
-        output_attentions: bool = False,
+        output_attentions: Optional[bool] = False,
     ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
         """Input shape: Batch x Time x Channel"""
 
         # if key_value_states are provided this layer is used as a cross-attention layer
         # for the decoder
         is_cross_attention = key_value_states is not None
         bsz, tgt_len, embed_dim = hidden_states.size()
@@ -214,247 +175,151 @@
         )
 
         attn_output = self.out_proj(attn_output)
 
         return attn_output, attn_weights_reshaped, past_key_value
 
 
-class Bart(core_model_class):
-    def __init__(self, config_path, **kwargs):
-        super().__init__()
-        self.config_path = config_path
-        params = json.load(open(self.config_path, "r"))
-        self.config = BartConfig(**params)
-
-    def save_checkpoint(self, ckpt_dir="./cache", **kwargs):
-        if not os.path.exists(ckpt_dir):
-            os.mkdir(ckpt_dir)
-        config_path = os.path.join(ckpt_dir, CONFIG_NAME)
-        with open(config_path, "w") as f:
-            f.write(open(self.config_path, "r").read())
-
-        super().save_checkpoint(ckpt_dir=ckpt_dir, **kwargs)
-
-    def from_checkpoint(self, ckpt_dir="./cache", **kwargs):
-        super().from_checkpoint(ckpt_dir=ckpt_dir, **kwargs)
-
-
-@register_model("core/model/bart_for_generation", generation_model_decorator)
-class BartForGeneration(Bart, GenerationMixinV2):
-    def __init__(self, config_path):
-        super().__init__(config_path)
-        self.shared = nn.Embedding(
-            self.config.vocab_size, self.config.d_model, self.config.pad_token_id
-        )
-        self.encoder = BartEncoder(self.config, self.shared)
-        self.decoder = BartDecoder(self.config, self.shared)
-
-        self.init_weights()
-
-    def get_input_embeddings(self):
-        return self.shared
-
-    def set_input_embeddings(self, value):
-        self.shared = value
-        self.encoder.embed_tokens = self.shared
-        self.decoder.embed_tokens = self.shared
-
-    def get_encoder(self):
-        return self.encoder
+class MBartForGeneration(GenericModel):
+    prefix_keys_in_state_dict = {
+        "^(?!model\.model\.)model\.": "model.",
+        "^lm_head.": "model.",
+    }
 
-    def get_decoder(self):
-        return self.decoder
-
-    @property
-    def device(self) -> device:
-        """
-        :obj:`torch.device`: The device on which the module is (assuming that all the module parameters are on the same
-        device).
-        """
-        try:
-            return next(self.parameters()).device
-        except StopIteration:
-            # For nn.DataParallel compatibility in PyTorch 1.5
-
-            def find_tensor_attributes(module: nn.Module) -> List[Tuple[str, Tensor]]:
-                tuples = [
-                    (k, v) for k, v in module.__dict__.items() if torch.is_tensor(v)
-                ]
-                return tuples
-
-            gen = self._named_members(get_members_fn=find_tensor_attributes)
-            first_tuple = next(gen)
-            return first_tuple[1].device
-
-    @classmethod
-    @add_default_section_for_init("core/model/bart")
-    def init_from_core_configure(cls, cfg, **kwargs):
-        pretrained_name = cfg.getdefault(
-            "core/model/bart", "pretrained_name", "default-bart"
-        )
-        config_name_or_path = cfg.getdefault(
-            "core/model/bart", "config_name_or_path", pretrained_name
-        )
-        config_path = (
-            CORE_BART_PRETRAINED_DICT[config_name_or_path][CONFIG_KEY]
-            if config_name_or_path in CORE_BART_PRETRAINED_DICT
-            else config_name_or_path
-        )
-
-        config_path = hf_cached_path(config_path)
-
-        inst = cls(config_path)
-        if pretrained_name is not None:
-            inst.from_pretrained(pretrained_name)
-
-        return inst
-
-    def prepare_inputs_for_generation(
+    def __init__(
         self,
-        decoder_input_ids,
-        past=None,
-        attention_mask=None,
-        head_mask=None,
-        use_cache=None,
-        encoder_outputs=None,
-        **kwargs,
+        config_path: str,
+        freeze_input_embedding: Optional[bool] = True,
+        gradient_checkpointing: Optional[bool] = False,
     ):
-        decoder_length = decoder_input_ids.size(1)
-        if past is not None:
-            decoder_input_ids = decoder_input_ids[:, -1:]
-
-        if decoder_length == 1:
-            encoder_hidden_states = encoder_outputs.last_hidden_state
-            encoder_hidden_states = encoder_hidden_states.view(
-                -1, self.num_beams, *encoder_hidden_states.size()[1:]
-            )
-            encoder_hidden_states = encoder_hidden_states[:, 0]
-            encoder_outputs.last_hidden_state = encoder_hidden_states
-
-        return {
-            "decoder_input_ids": decoder_input_ids,
-            "attention_mask": attention_mask,
-            "encoder_outputs": encoder_outputs,
-            "decoder_length": decoder_length,
-            "past_key_values": past,
-        }
-
-    @staticmethod
-    def _reorder_cache(past, beam_idx):
-        reordered_past = ()
-        for layer_past in past:
-            # cached cross_attention states don't have to be reordered -> they are always the same
-            reordered_past += (
-                tuple(
-                    past_state.index_select(0, beam_idx)
-                    for past_state in layer_past[:2]
-                )
-                + layer_past[2:],
-            )
-        return reordered_past
+        """
+        Initializes an MBartForGeneration model with the provided configuration.
 
-    @staticmethod
-    def _reorder_cache_v2(past, batch_idx, beam_idx):
-        if batch_idx is None:
-            return _reorder_cache(past, beam_idx)
-        reordered_past = ()
-        for layer_past in past:
-            # cached cross_attention states don't have to be reordered -> they are always the same
-            past_state1 = tuple(
-                [past_state.index_select(0, beam_idx) for past_state in layer_past[:2]]
-            )
-            past_state2 = tuple(
-                [past_state.index_select(0, batch_idx) for past_state in layer_past[2:]]
-            )
-            reordered_past += (past_state1 + past_state2,)
+        Args:
+            config_path (str): The path to the model configuration file.
+            freeze_input_embedding (bool, optional): Whether to freeze the input embeddings. Defaults to True.
+            gradient_checkpointing (bool, optional): Whether to use gradient checkpointing. Defaults to False.
+        """
+        super().__init__()
+        self.config = MBartConfig.from_json_file(config_path)
+        self.config.gradient_checkpointing = gradient_checkpointing
+        self.model = MBartForConditionalGeneration(self.config)
+
+        if freeze_input_embedding:
+            for param in self.model.get_input_embeddings().parameters():
+                param.requires_grad = False
 
-        return reordered_past
+        self.init_weights()
 
     def forward(
         self,
-        tokens_ids_a=None,
-        tokens_mask_a=None,
-        tokens_ids_b=None,
-        tokens_mask_b=None,
-        decoder_input_ids=None,
-        attention_mask=None,
-        encoder_outputs=None,
-        past_key_values=None,
-        output_attentions=None,
-        output_hidden_states=None,
-        decoder_length=None,
-        return_dict=None,
+        input_ids: torch.Tensor,
+        attention_mask: torch.Tensor,
+        decoder_input_ids: torch.Tensor,
+        decoder_attention_mask: torch.Tensor,
     ):
-        if self.training:
-            encoder_outputs = self.encoder(tokens_ids_a, attention_mask=tokens_mask_a)
-            decoder_outputs = self.decoder(
-                input_ids=tokens_ids_b,
-                attention_mask=tokens_mask_b,
-                encoder_hidden_states=encoder_outputs[0],
-                encoder_attention_mask=tokens_mask_a,
-            )
-            logits = F.linear(decoder_outputs[0], self.shared.weight)
-            return logits
-        batch_size = decoder_input_ids.size(0)
-        decoder_attention_mask = torch.ones(batch_size, decoder_length).to(
-            decoder_input_ids
-        )
-        outputs = self.decoder(
-            input_ids=decoder_input_ids,
-            attention_mask=decoder_attention_mask,
-            encoder_hidden_states=encoder_outputs.last_hidden_state,
-            encoder_attention_mask=attention_mask,
-            use_cache=True,
-            past_key_values=past_key_values,
-            output_attentions=output_attentions,
-            output_hidden_states=output_hidden_states,
-            return_dict=return_dict,
+        """
+        Performs forward pass of the MBartForGeneration model.
+
+        Args:
+            input_ids (torch.Tensor): Tensor of input token IDs.
+            attention_mask (torch.Tensor): Tensor of attention mask.
+            decoder_input_ids (torch.Tensor): Tensor of decoder input token IDs.
+            decoder_attention_mask (torch.Tensor): Tensor of decoder attention mask.
+
+        Returns:
+            (torch.Tensor):The model's logits.
+        """
+        outputs = self.model(
+            input_ids=input_ids,
+            attention_mask=attention_mask,
+            decoder_input_ids=decoder_input_ids,
+            decoder_attention_mask=decoder_attention_mask,
+            return_dict=True,
         )
-        logits = F.linear(outputs[0], self.shared.weight)
-        past_key_values = outputs[1]
-        return Seq2SeqLMOutput(logits=logits, past_key_values=past_key_values)
+        logits = outputs.logits
+        return logits
 
-    @add_default_section_for_instance_function("core/model/bart")
+    @torch.no_grad()
     def generate(
         self,
-        tokens_ids,
-        tokens_mask,
-        num_beams=5,
-        decoder_start_token_id=2,
-        decoder_end_token_id=2,
-        num_return_sequences=1,
-        min_gen_seq_length=0,
-        max_gen_seq_length=48,
-        repetition_penalty=1.0,
-        no_repeat_ngram_size=0,
-        early_stopping=True,
-        length_penalty=1.0,
-        num_beam_groups=1,
-        diversity_penalty=0.0,
-        diverse_rate=0.0,
+        input_ids: torch.Tensor,
+        num_beams: Optional[int] = 5,
+        decoder_start_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[int] = 2,
+        num_return_sequences: Optional[int] = 1,
+        min_gen_seq_length: Optional[int] = 0,
+        max_gen_seq_length: Optional[int] = 48,
+        repetition_penalty: Optional[float] = 1.0,
+        no_repeat_ngram_size: Optional[int] = 0,
+        early_stopping: Optional[bool] = True,
+        length_penalty: Optional[float] = 1.0,
+        num_beam_groups: Optional[int] = 1,
+        diversity_penalty: Optional[float] = 0.0,
+        do_sample: Optional[bool] = False,
+        temperature: Optional[float] = 1.0,
+        top_k: Optional[int] = 50,
+        top_p: Optional[float] = 1.0,
     ):
-        self.num_beams = num_beams
-        batch_hyp = super().generate(
-            tokens_ids,
+        """
+        Generates sequences using the MBartForGeneration model.
+
+        Args:
+            input_ids: The input token IDs.
+            num_beams (int, optional): The number of beams for beam search. Defaults to 5.
+            decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.
+            decoder_end_token_id (int, optional): The decoder's end token ID. Defaults to 2.
+            num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.
+            min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.
+            max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.
+            repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.
+            no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.
+            early_stopping (bool, optional): Whether to stop generation early. Defaults to True.
+            length_penalty (float, optional): The length penalty. Defaults to 1.0.
+            num_beam_groups (int, optional): The number of beam groups for diverse beam search. Defaults to 1.
+            diversity_penalty (float, optional): The diversity penalty. Defaults to 0.0.
+            do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.
+            temperature (float, optional): The temperature for sampling. Defaults to 1.0.
+            top_k (int, optional): The value for top-k sampling. Defaults to 50.
+            top_p (float, optional): The value for top-p (nucleus) sampling. Defaults to 1.0.
+
+        Returns:
+            GenericOutputs: The generated sequences and their scores.
+        """
+        outputs = self.model.generate(
+            input_ids,
             max_length=max_gen_seq_length,
             min_length=min_gen_seq_length,
             num_beams=num_beams,
-            do_sample=False,
+            do_sample=do_sample,
             decoder_start_token_id=decoder_start_token_id,
             no_repeat_ngram_size=no_repeat_ngram_size,
             early_stopping=early_stopping,
             length_penalty=length_penalty,
             repetition_penalty=repetition_penalty,
             num_return_sequences=num_return_sequences,
             bos_token_id=decoder_start_token_id,
             eos_token_id=decoder_end_token_id,
             num_beam_groups=num_beam_groups,
             diversity_penalty=diversity_penalty,
+            temperature=temperature,
+            top_k=top_k,
+            top_p=top_p,
+            return_dict_in_generate=True,
+            output_scores=True,
+        )
+
+        sequences = outputs.sequences.reshape(
+            -1, num_return_sequences, outputs.sequences.size(-1)
         )
-        batch_hyp = batch_hyp.reshape(-1, num_return_sequences, batch_hyp.size(-1))
-        if batch_hyp.size(-1) >= max_gen_seq_length:
-            return batch_hyp[:, :, :max_gen_seq_length]
-        batch_ret = torch.zeros(
-            batch_hyp.size(0), num_return_sequences, max_gen_seq_length
+        outputs.sequences = torch.zeros(
+            sequences.size(0), num_return_sequences, max_gen_seq_length
+        ).to(device=sequences.device)
+        outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)
+
+        if num_return_sequences == 1:
+            outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)
+
+        return GenericOutputs(
+            sequences=outputs.sequences,
+            sequences_scores=outputs.sequences_scores,
         )
-        batch_ret[:, :, : batch_hyp.size(-1)].copy_(batch_hyp)
-        return batch_ret.long()
```

### Comparing `unitorch-0.0.0.1/unitorch/generation/mass.py` & `unitorch-0.0.0.2/src/unitorch/cli/tasks/deepspeed.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,699 +1,711 @@
+# Copyright (c) FULIUCANSHENG.
+# Licensed under the MIT License.
+
 import os
 import torch
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
-from collections import OrderedDict
-from torch import Tensor, device
+import time
 import json
-import random
-from functools import partial
+import logging
+import deepspeed
 import numpy as np
+import pandas as pd
+import torch.distributed as dist
 import torch.nn as nn
 import torch.nn.functional as F
-
-from unitorch import add_core_pretrained_dict, register_model
-from unitorch.core import core_model_class
-from unitorch.utils.hf import hf_cached_path
-from unitorch.modules.generation_mixin_v2 import GenerationMixinV2
-from transformers.modeling_outputs import Seq2SeqLMOutput
-from transformers.configuration_utils import PretrainedConfig
-from transformers.file_utils import ModelOutput
-from fairseq.modules.multihead_attention import MultiheadAttention
-from fairseq.models.transformer import TransformerEncoder, TransformerDecoder
-from fairseq.tokenizer import tokenize_line
-from fairseq.binarizer import safe_readline
-from fairseq.data import data_utils, Dictionary
-from fairseq import utils
-
-from unitorch.utils.decorators import (
-    generation_model_decorator,
+from copy import deepcopy
+from itertools import chain
+from collections.abc import Iterable
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union, Iterator
+from torch.utils.data import DataLoader, Dataset, SequentialSampler
+from torch.utils.data.distributed import DistributedSampler
+from torch.cuda.amp import autocast, GradScaler
+from torch.multiprocessing import Process, Queue
+from unitorch import set_seed, is_torch2_available
+from unitorch.models import ExponentialMovingAverage
+from unitorch.utils import get_local_rank
+from unitorch.utils import (
+    DistributedSkipSampler,
+    RandomSkipSampler,
+    SequentialSkipSampler,
+    PostProcess,
+    IOProcess,
+    GENERATE_FINISHED,
+)
+from unitorch.models import GenericOutputs
+from unitorch.utils import ActiveGPUJob
+from unitorch.cli import (
+    cached_path,
+    register_task,
+    registered_model,
+    registered_optim,
+    registered_dataset,
+    registered_loss,
+    registered_score,
+    registered_scheduler,
+    registered_writer,
+    init_registered_module,
+    init_registered_process,
     add_default_section_for_init,
-    add_default_section_for_instance_function,
-    replace,
+    add_default_section_for_function,
+)
+from unitorch.cli.models import (
+    ModelInputs,
+    ModelOutputs,
+    ModelTargets,
+    LossOutputs,
+    CombineTensorsInputs,
+    CombineTensorsTargets,
+)
+from unitorch.cli.tasks.supervised import (
+    DatasetFeature,
+    collate_fn,
+    infer,
+    monitor,
+    save_checkpoint,
 )
-
-CONFIG_KEY = "config"
-CONFIG_NAME = "config.json"
-
-VOCABS_KEY = "vocab"
-VOCABS_NAME = "vocab.txt"
-
-CORE_MASS_PRETRAINED_DICT = {
-    "default-mass": {
-        "config": "https://huggingface.co/fuliucansheng/mass/resolve/main/mass-base-uncased-config.json",
-        "vocab": "https://huggingface.co/fuliucansheng/mass/resolve/main/mass-base-uncased-vocab.txt",
-    },
-    "mass-base-uncased": {
-        "config": "https://huggingface.co/fuliucansheng/mass/resolve/main/mass-base-uncased-config.json",
-        "vocab": "https://huggingface.co/fuliucansheng/mass/resolve/main/mass-base-uncased-vocab.txt",
-        "weight": "https://huggingface.co/fuliucansheng/mass/resolve/main/mass-base-uncased-pytorch-model.bin",
-    },
-}
-
-add_core_pretrained_dict(CORE_MASS_PRETRAINED_DICT)
-
-
-def _reorder_buffer(attn_cache, new_order):
-    for k, input_buffer_k in attn_cache.items():
-        if input_buffer_k is not None:
-            attn_cache[k] = input_buffer_k.index_select(0, new_order)
-    return attn_cache
 
 
-class BertDictionary(Dictionary):
-    """A mapping from symbols to consecutive integers"""
+@register_task("core/task/deepspeed/supervised")
+class DeepspeedTask:
+    """Task class for deepspeed supervised learning."""
 
     def __init__(
         self,
-        pad="<pad>",
-        eos="</s>",
-        unk="<unk>",
-        bos="<s>",
-        extra_special_symbols=None,
+        configure,
+        model,
+        datasets,
+        local_rank: Optional[int] = -1,
+        seed: Optional[int] = 1123,
     ):
-        super().__init__(
-            pad=pad,
-            eos=eos,
-            unk=unk,
-            bos=bos,
-            extra_special_symbols=extra_special_symbols,
-        )
+        """
+        Initialize the DeepspeedTask.
+
+        Args:
+            configure: The configuration object.
+            model: The model for supervised learning.
+            datasets: The datasets for training and evaluation.
+            local_rank (optional): The local rank for distributed training. Defaults to -1.
+            seed (optional): The random seed. Defaults to 1123.
+        """
+        set_seed(seed)
+        self.n_gpu = 1 if torch.cuda.is_available() else 0
+        if dist.is_initialized():
+            self.n_gpu = dist.get_world_size()
+
+        self.config = configure
+        self.model = model
+        self.datasets = datasets
+        self.local_rank = local_rank
+
+        if self.local_rank != -1:
+            torch.cuda.set_device(self.local_rank)
+
+        if torch.cuda.is_available():
+            self.model = self.model.cuda()
+
+        self.best_score = -np.inf
 
     @classmethod
-    def load_from_file(cls, filename):
-        d = cls()
-        d.symbols = []
-        d.count = []
-        d.indices = {}
-
-        with open(filename, "r", encoding="utf-8", errors="ignore") as input_file:
-            for line in input_file:
-                k = line.strip()
-                d.add_symbol(k)
-
-        d.unk_word = "[UNK]"
-        d.pad_word = "[PAD]"
-        d.eos_word = "[SEP]"
-        d.bos_word = "[CLS]"
-
-        d.bos_index = d.add_symbol("[CLS]")
-        d.pad_index = d.add_symbol("[PAD]")
-        d.eos_index = d.add_symbol("[SEP]")
-        d.unk_index = d.add_symbol("[UNK]")
-
-        d.nspecial = 999
-        return d
-
-    def save(self, f):
-        """Stores dictionary into a text file"""
-        ex_keys, ex_vals = self._get_meta()
-        self._save(f, zip(ex_keys + self.symbols, ex_vals + self.count))
+    @add_default_section_for_init("core/task/deepspeed/supervised")
+    def from_core_configure(cls, config, **kwargs):
+        """
+        Create a DeepspeedTask instance from a core configuration.
+
+        Args:
+            config: The core configuration.
+            **kwargs: Additional keyword arguments.
 
+        Returns:
+            A DeepspeedTask instance.
+        """
+        try:
+            deepspeed.init_distributed(dist_backend="nccl", init_method="env://")
+        except:
+            logging.info("PyTorch is not in distributed mode")
 
-@replace(MultiheadAttention)
-class MultiheadAttentionV2(MultiheadAttention):
-    def __init__(
-        self,
-        embed_dim,
-        num_heads,
-        kdim=None,
-        vdim=None,
-        dropout=0.0,
-        bias=True,
-        add_bias_kv=False,
-        add_zero_attn=False,
-        self_attention=False,
-        encoder_decoder_attention=False,
-        q_noise=0.0,
-        qn_block_size=8,
-    ):
-        super().__init__(
-            embed_dim,
-            num_heads,
-            kdim,
-            vdim,
-            dropout,
-            bias,
-            add_bias_kv,
-            add_zero_attn,
-            self_attention,
-            encoder_decoder_attention,
-            q_noise,
-            qn_block_size,
+        config.set_default_section("core/task/deepspeed/supervised")
+
+        model = config.getoption("model", None)
+        dataset = config.getoption("dataset", None)
+
+        if model is not None:
+            model = init_registered_module(model, config, registered_model)
+
+        if dataset is not None:
+            dataset = init_registered_module(dataset, config, registered_dataset)
+
+        local_rank = config.getdefault(
+            "core/cli",
+            "local_rank",
+            get_local_rank(),
         )
 
-    def forward(
+        return dict(
+            configure=config,
+            model=model,
+            datasets=dataset,
+            local_rank=local_rank,
+        )
+
+    @add_default_section_for_function("core/task/deepspeed/supervised")
+    def train(
         self,
-        query,
-        key: Optional[Tensor],
-        value: Optional[Tensor],
-        key_padding_mask: Optional[Tensor] = None,
-        incremental_state: Optional[Dict[str, Dict[str, Optional[Tensor]]]] = None,
-        need_weights: bool = True,
-        static_kv: bool = False,
-        attn_mask: Optional[Tensor] = None,
-        before_softmax: bool = False,
-        need_head_weights: bool = False,
-    ) -> Tuple[Tensor, Optional[Tensor]]:
-        """Input shape: Time x Batch x Channel
+        config_path: str,
+        optim: str,
+        loss_fn: str,
+        score_fn: str,
+        monitor_fns: Optional[Union[str, List[str]]] = None,
+        from_ckpt_dir: Optional[str] = "./from_ckpt",
+        to_ckpt_dir: Optional[str] = "./to_ckpt",
+        train_batch_size: Optional[int] = 128,
+        dev_batch_size: Optional[int] = 128,
+        pin_memory: Optional[bool] = True,
+        num_workers: Optional[int] = 4,
+        save_optimizer: Optional[bool] = True,
+        save_scheduler: Optional[bool] = True,
+        log_freq: Optional[int] = 100,
+        ckpt_freq: Optional[int] = 10000,
+        grad_acc_step: Optional[int] = 1,
+        max_grad_norm: Optional[float] = 1.0,
+        learning_rate: Optional[float] = None,
+        max_warmup_learning_rate: Optional[float] = None,
+        num_warmup_steps: Optional[int] = None,
+        epochs: Optional[int] = 5,
+        use_ema: Optional[bool] = False,
+        ema_decay: Optional[float] = 0.9999,
+        ema_tau: Optional[int] = 2000,
+        gpu_mode: Optional[bool] = False,
+    ):
+        """
+        Train the model using deepspeed.
+
         Args:
-            key_padding_mask (ByteTensor, optional): mask to exclude
-                keys that are pads, of shape `(batch, src_len)`, where
-                padding elements are indicated by 1s.
-            need_weights (bool, optional): return the attention weights,
-                averaged over heads (default: False).
-            attn_mask (ByteTensor, optional): typically used to
-                implement causal attention, where the mask prevents the
-                attention from looking forward in time (default: None).
-            before_softmax (bool, optional): return the raw attention
-                weights and values before the attention softmax.
-            need_head_weights (bool, optional): return the attention
-                weights for each head. Implies *need_weights*. Default:
-                return the average attention weights over all heads.
+            config_path: The path to the deepspeed configuration file.
+            optim: The optimizer used for training.
+            loss_fn: The loss function used for training.
+            score_fn: The score function used for evaluation.
+            monitor_fns (optional): The monitoring functions for evaluation. Defaults to None.
+            from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to "./from_ckpt".
+            to_ckpt_dir (optional): The directory path to save checkpoints to. Defaults to "./to_ckpt".
+            train_batch_size (optional): The batch size for training. Defaults to 128.
+            dev_batch_size (optional): The batch size for evaluation. Defaults to 128.
+            pin_memory (optional): Whether to pin memory during data loading. Defaults to True.
+            num_workers (optional): The number of worker processes for data loading. Defaults to 4.
+            save_optimizer (optional): Whether to save the optimizer state. Defaults to True.
+            save_scheduler (optional): Whether to save the scheduler state. Defaults to True.
+            log_freq (optional): The frequency of logging. Defaults to 100.
+            ckpt_freq (optional): The frequency of saving checkpoints. Defaults to 10000.
+            grad_acc_step (optional): The number of gradient accumulation steps. Defaults to 1.
+            max_grad_norm (optional): The maximum gradient norm. Defaults to 1.0.
+            learning_rate (optional): The learning rate for the optimizer. Defaults to None.
+            max_warmup_learning_rate (optional): The maximum learning rate during warmup. Defaults to None.
+            num_warmup_steps (optional): The number of warmup steps. Defaults to None.
+            epochs (optional): The number of training epochs. Defaults to 5.
+            use_ema (optional): Whether to use exponential moving average. Defaults to False.
+            ema_decay (optional): The decay factor for exponential moving average. Defaults to 0.9999.
+            ema_tau (optional): The time constant for exponential moving average. Defaults to 2000.
+            gpu_mode (optional): Whether to make GPU active. Defaults to False.
         """
-        if need_head_weights:
-            need_weights = True
+        if not os.path.exists(to_ckpt_dir) and self.local_rank in [-1, 0]:
+            os.makedirs(to_ckpt_dir, exist_ok=True)
+
+        if loss_fn is not None:
+            loss_fn = init_registered_module(loss_fn, self.config, registered_loss)
 
-        is_tpu = query.device.type == "xla"
+        if score_fn is not None:
+            score_fn = init_registered_module(score_fn, self.config, registered_score)
 
-        tgt_len, bsz, embed_dim = query.size()
-        assert embed_dim == self.embed_dim
-        assert list(query.size()) == [tgt_len, bsz, embed_dim]
-
-        if (
-            not self.onnx_trace
-            and not is_tpu  # don't use PyTorch version on TPUs
-            and incremental_state is None
-            and not static_kv
-            # A workaround for quantization to work. Otherwise JIT compilation
-            # treats bias in linear module as method.
-            and not torch.jit.is_scripting()
-        ):
-            assert key is not None and value is not None
-            return F.multi_head_attention_forward(
-                query,
-                key,
-                value,
-                self.embed_dim,
-                self.num_heads,
-                torch.empty([0]),
-                torch.cat((self.q_proj.bias, self.k_proj.bias, self.v_proj.bias)),
-                self.bias_k,
-                self.bias_v,
-                self.add_zero_attn,
-                self.dropout_module.p,
-                self.out_proj.weight,
-                self.out_proj.bias,
-                self.training or self.dropout_module.apply_during_inference,
-                key_padding_mask,
-                need_weights,
-                attn_mask,
-                use_separate_proj_weight=True,
-                q_proj_weight=self.q_proj.weight,
-                k_proj_weight=self.k_proj.weight,
-                v_proj_weight=self.v_proj.weight,
+        if monitor_fns is not None:
+            monitor_fns = [
+                init_registered_module(monitor_fn, self.config, registered_score)
+                for monitor_fn in monitor_fns
+                if monitor_fn in registered_score
+            ]
+
+        config_file = cached_path(config_path)
+        config_dict = json.load(open(config_file, "r"))
+        config_dict["train_micro_batch_size_per_gpu"] = train_batch_size
+
+        if os.path.exists(from_ckpt_dir):
+            self.model.from_checkpoint(from_ckpt_dir)
+
+        if os.path.exists(to_ckpt_dir):
+            self.model.from_checkpoint(
+                to_ckpt_dir,
+                weight_name="pytorch_model_latest.bin",
             )
 
-        if incremental_state is not None:
-            saved_state = self._get_input_buffer(incremental_state)
-            if saved_state is not None and "prev_key" in saved_state:
-                # previous time steps are cached - no need to recompute
-                # key and value if they are static
-                if static_kv:
-                    assert self.encoder_decoder_attention and not self.self_attention
-                    key = value = None
-        else:
-            saved_state = None
+        params = self.model.parameters()
+        params = filter(lambda x: x.requires_grad, params)
+
+        assert "optimizer" in config_dict
 
-        if self.self_attention:
-            q = self.q_proj(query)
-            k = self.k_proj(query)
-            v = self.v_proj(query)
-        elif self.encoder_decoder_attention:
-            # encoder-decoder attention
-            q = self.q_proj(query)
-            if key is None:
-                assert value is None
-                k = v = None
-            else:
-                k = self.k_proj(key)
-                v = self.v_proj(key)
+        if "params" not in config_dict["optimizer"]:
+            config_dict["optimizer"]["params"] = dict()
 
+        if "scheduler" in config_dict:
+            if "params" not in config_dict["scheduler"]:
+                config_dict["scheduler"]["params"] = dict()
+
+        if learning_rate is not None:
+            config_dict["optimizer"]["params"]["lr"] = learning_rate
+            if "scheduler" in config_dict:
+                config_dict["scheduler"]["params"]["warmup_max_lr"] = learning_rate
+
+        if max_warmup_learning_rate is not None and "scheduler" in config_dict:
+            config_dict["scheduler"]["params"][
+                "warmup_max_lr"
+            ] = max_warmup_learning_rate
+
+        if num_warmup_steps is not None and "scheduler" in config_dict:
+            if "params" not in config_dict["scheduler"]:
+                config_dict["scheduler"]["params"] = dict()
+            config_dict["scheduler"]["params"]["warmup_num_steps"] = num_warmup_steps
+
+        info_path = os.path.join(to_ckpt_dir, "info.json")
+        if os.path.exists(info_path):
+            info = json.load(open(os.path.join(to_ckpt_dir, "info.json")))
         else:
-            assert key is not None and value is not None
-            q = self.q_proj(query)
-            k = self.k_proj(key)
-            v = self.v_proj(value)
-        q *= self.scaling
-
-        if self.bias_k is not None:
-            assert self.bias_v is not None
-            k = torch.cat([k, self.bias_k.repeat(1, bsz, 1)])
-            v = torch.cat([v, self.bias_v.repeat(1, bsz, 1)])
-            if attn_mask is not None:
-                attn_mask = torch.cat(
-                    [attn_mask, attn_mask.new_zeros(attn_mask.size(0), 1)], dim=1
+            info = dict()
+
+        global_epoch = info.get("global_epoch", 0)
+        global_step = info.get("global_step", 0)
+        self.best_score = info.get("best_score", self.best_score)
+
+        logging.info(f"the best score is {self.best_score}")
+
+        self.ema_model = None
+        if use_ema:
+            num_ema_steps = info.get("num_ema_steps", 0)
+            self.ema_model = ExponentialMovingAverage(
+                self.model,
+                decay=ema_decay,
+                tau=ema_tau,
+                num_steps=num_ema_steps,
+            )
+            if os.path.exists(from_ckpt_dir):
+                self.ema_model.from_checkpoint(
+                    from_ckpt_dir,
+                    weight_name="pytorch_ema_model.bin",
                 )
-            if key_padding_mask is not None:
-                key_padding_mask = torch.cat(
-                    [
-                        key_padding_mask,
-                        key_padding_mask.new_zeros(key_padding_mask.size(0), 1),
-                    ],
-                    dim=1,
+            if os.path.exists(to_ckpt_dir):
+                self.ema_model.from_checkpoint(
+                    to_ckpt_dir,
+                    weight_name="pytorch_ema_model_latest.bin",
                 )
 
-        q = (
-            q.contiguous()
-            .view(tgt_len, bsz * self.num_heads, self.head_dim)
-            .transpose(0, 1)
-        )
-        if k is not None:
-            kv_bsz = k.size(1)
-            k = (
-                k.contiguous()
-                .view(-1, kv_bsz * self.num_heads, self.head_dim)
-                .transpose(0, 1)
-            )
-        if v is not None:
-            kv_bsz = v.size(1)
-            v = (
-                v.contiguous()
-                .view(-1, kv_bsz * self.num_heads, self.head_dim)
-                .transpose(0, 1)
+        for n, p in self.model.named_parameters():
+            logging.debug(
+                f"{n}: trainable - {p.requires_grad} | tensor shape - {p.shape}"
             )
 
-        if saved_state is not None:
-            # saved states are stored with shape (bsz, num_heads, seq_len, head_dim)
-            if "prev_key" in saved_state:
-                _prev_key = saved_state["prev_key"]
-                assert _prev_key is not None
-                kv_bsz = _prev_key.size(0)
-                prev_key = _prev_key.view(kv_bsz * self.num_heads, -1, self.head_dim)
-                if static_kv:
-                    k = prev_key
-                else:
-                    assert k is not None
-                    k = torch.cat([prev_key, k], dim=1)
-            if "prev_value" in saved_state:
-                _prev_value = saved_state["prev_value"]
-                assert _prev_value is not None
-                kv_bsz == _prev_value.size(0)
-                prev_value = _prev_value.view(
-                    kv_bsz * self.num_heads, -1, self.head_dim
-                )
-                if static_kv:
-                    v = prev_value
+        self.model, optim, _, scheduler = deepspeed.initialize(
+            model=self.model,
+            config=config_dict,
+            model_parameters=params,
+        )
+
+        global_rank = -1
+        if self.n_gpu > 1:
+            global_rank = dist.get_rank()
+
+        train_sampler = DistributedSkipSampler if self.n_gpu > 1 else RandomSkipSampler
+        dev_sampler = DistributedSampler if self.n_gpu > 1 else SequentialSampler
+
+        if gpu_mode:
+            with ActiveGPUJob() as _:
+                dataset_train = self.datasets.get("train")
+                dataset_dev = self.datasets.get("dev")
+        else:
+            dataset_train = self.datasets.get("train")
+            dataset_dev = self.datasets.get("dev")
+
+        iter_train = DataLoader(
+            dataset_train,
+            sampler=train_sampler(dataset_train)
+            if not isinstance(dataset_train, Iterable)
+            else None,
+            batch_size=train_batch_size,
+            shuffle=False,
+            pin_memory=pin_memory,
+            num_workers=num_workers,
+            collate_fn=collate_fn,
+        )
+
+        iter_dev = DataLoader(
+            dataset_dev,
+            sampler=dev_sampler(dataset_dev)
+            if not isinstance(dataset_dev, Iterable)
+            else None,
+            batch_size=dev_batch_size,
+            shuffle=False,
+            pin_memory=pin_memory,
+            num_workers=num_workers,
+            collate_fn=collate_fn,
+        )
+
+        log_loss = 0
+        dev_epoch = 0
+        for e in range(0, epochs):
+            torch.cuda.empty_cache()
+            if e < global_epoch:
+                continue
+
+            if hasattr(dataset_train, "set_epoch"):
+                dataset_train.set_epoch(e)
+
+            if hasattr(dataset_train, "set_skip_step"):
+                dataset_train.set_skip_step(global_step * train_batch_size)
+
+            if hasattr(iter_train.sampler, "set_epoch"):
+                iter_train.sampler.set_epoch(e)
+
+            if hasattr(iter_train.sampler, "set_skip_step"):
+                iter_train.sampler.set_skip_step(global_step * train_batch_size)
+
+            self.model.train()
+            is_update_step = True
+            for step, (inputs, targets) in enumerate(iter_train):
+                step = step + global_step
+                is_update_step = False
+                if torch.cuda.is_available():
+                    inputs = inputs.cuda()
+                    targets = targets.cuda()
+
+                if is_torch2_available():
+                    with torch.cuda.amp.autocast(
+                        enabled=True
+                    ) as autocast, torch.backends.cuda.sdp_kernel(
+                        enable_flash=False
+                    ) as disable:
+                        outputs = self.model(**inputs.dict())
+                        if isinstance(outputs, LossOutputs):
+                            loss = outputs.loss / grad_acc_step
+                        else:
+                            loss = (
+                                loss_fn(outputs=outputs, targets=targets)
+                                / grad_acc_step
+                            )
                 else:
-                    assert v is not None
-                    v = torch.cat([prev_value, v], dim=1)
-            prev_key_padding_mask: Optional[Tensor] = None
-            if "prev_key_padding_mask" in saved_state:
-                prev_key_padding_mask = saved_state["prev_key_padding_mask"]
-            assert k is not None and v is not None
-            key_padding_mask = MultiheadAttention._append_prev_key_padding_mask(
-                key_padding_mask=key_padding_mask,
-                prev_key_padding_mask=prev_key_padding_mask,
-                batch_size=kv_bsz,
-                src_len=k.size(1),
-                static_kv=static_kv,
+                    with torch.cuda.amp.autocast(enabled=True) as autocast:
+                        outputs = self.model(**inputs.dict())
+                        if isinstance(outputs, LossOutputs):
+                            loss = outputs.loss / grad_acc_step
+                        else:
+                            loss = (
+                                loss_fn(outputs=outputs, targets=targets)
+                                / grad_acc_step
+                            )
+
+                nn.utils.clip_grad_norm_(self.model.parameters(), max_grad_norm)
+                self.model.backward(loss)
+
+                log_loss += loss.data * grad_acc_step
+                if (step + 1) % grad_acc_step == 0:
+                    is_update_step = True
+                    optim.step()
+                    if scheduler is not None:
+                        scheduler.step()
+                    optim.zero_grad()
+
+                    if use_ema and self.ema_model is not None:
+                        self.ema_model.step(
+                            self.model.module if self.n_gpu > 1 else self.model
+                        )
+
+                if (step + 1) % log_freq == 0 and global_rank in [-1, 0]:
+                    logging.info(
+                        f"epoch {e} step {step}: loss -- { log_loss / log_freq }"
+                    )
+                    log_loss = 0
+
+                if (step + 1) % ckpt_freq == 0:
+                    if hasattr(dataset_dev, "set_epoch"):
+                        dataset_dev.set_epoch(dev_epoch)
+
+                    if hasattr(iter_dev.sampler, "set_epoch"):
+                        iter_dev.sampler.set_epoch(dev_epoch)
+
+                    dev_epoch += 1
+                    self.best_score = save_checkpoint(
+                        self.model.module if self.n_gpu > 1 else self.model,
+                        to_ckpt_dir,
+                        iter_dev,
+                        score_fn,
+                        monitor_fns,
+                        optim=optim if save_optimizer else None,
+                        scheduler=scheduler if save_scheduler else None,
+                        ema_model=self.ema_ema_model if use_ema else None,
+                        best_score=self.best_score,
+                        info_path=info_path,
+                        local_rank=self.local_rank,
+                        global_epoch=e,
+                        global_step=step + 1,
+                    )
+
+            if not is_update_step:
+                optim.step()
+                if scheduler is not None:
+                    scheduler.step()
+                optim.zero_grad()
+
+                if use_ema and self.ema_model is not None:
+                    self.ema_model.step(
+                        self.model.module if self.n_gpu > 1 else self.model
+                    )
+
+            log_loss = 0
+
+            if hasattr(dataset_dev, "set_epoch"):
+                dataset_dev.set_epoch(dev_epoch)
+
+            if hasattr(iter_dev.sampler, "set_epoch"):
+                iter_dev.sampler.set_epoch(dev_epoch)
+
+            dev_epoch += 1
+
+            global_step = 0
+            self.best_score = save_checkpoint(
+                self.model.module if self.n_gpu > 1 else self.model,
+                to_ckpt_dir,
+                iter_dev,
+                score_fn,
+                monitor_fns,
+                optim=optim if save_optimizer else None,
+                scheduler=scheduler if save_scheduler else None,
+                ema_model=self.ema_ema_model if use_ema else None,
+                best_score=self.best_score,
+                info_path=info_path,
+                local_rank=self.local_rank,
+                global_epoch=e,
+                global_step=step + 1,
             )
 
-            saved_state["prev_key"] = k.view(kv_bsz, self.num_heads, -1, self.head_dim)
-            saved_state["prev_value"] = v.view(
-                kv_bsz, self.num_heads, -1, self.head_dim
-            )
-            saved_state["prev_key_padding_mask"] = key_padding_mask
-            # In this branch incremental_state is never None
-            assert incremental_state is not None
-            incremental_state = self._set_input_buffer(incremental_state, saved_state)
-        assert k is not None
-        src_len = k.size(1)
-
-        # This is part of a workaround to get around fork/join parallelism
-        # not supporting Optional types.
-        if key_padding_mask is not None and key_padding_mask.dim() == 0:
-            key_padding_mask = None
-
-        if key_padding_mask is not None:
-            assert key_padding_mask.size(0) == kv_bsz
-            assert key_padding_mask.size(1) == src_len
-
-        if self.add_zero_attn:
-            assert v is not None
-            src_len += 1
-            k = torch.cat([k, k.new_zeros((k.size(0), 1) + k.size()[2:])], dim=1)
-            v = torch.cat([v, v.new_zeros((v.size(0), 1) + v.size()[2:])], dim=1)
-            if attn_mask is not None:
-                attn_mask = torch.cat(
-                    [attn_mask, attn_mask.new_zeros(attn_mask.size(0), 1)], dim=1
-                )
-            if key_padding_mask is not None:
-                key_padding_mask = torch.cat(
-                    [
-                        key_padding_mask,
-                        torch.zeros(key_padding_mask.size(0), 1).type_as(
-                            key_padding_mask
-                        ),
-                    ],
-                    dim=1,
-                )
+    @torch.no_grad()
+    @add_default_section_for_function("core/task/deepspeed/supervised")
+    def eval(
+        self,
+        monitor_fns: Union[str, List[str]],
+        from_ckpt_dir: Optional[str] = "./from_ckpt",
+        dev_batch_size: Optional[int] = 128,
+        pin_memory: Optional[bool] = True,
+        num_workers: Optional[int] = 4,
+        gpu_mode: Optional[bool] = False,
+    ):
+        """
+        Evaluate the model.
 
-        if self.encoder_decoder_attention == True and bsz != kv_bsz:
-            attn_weights = torch.einsum(
-                "bxhtd,bhsd->bxhts",
-                q.view(kv_bsz, -1, self.num_heads, *q.size()[1:]),
-                k.view(kv_bsz, self.num_heads, *k.size()[1:]),
+        Args:
+            monitor_fns: The monitoring functions for evaluation.
+            from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to "./from_ckpt".
+            dev_batch_size (optional): The batch size for evaluation. Defaults to 128.
+            pin_memory (optional): Whether to pin memory during data loading. Defaults to True.
+            num_workers (optional): The number of worker processes for data loading. Defaults to 4.
+            gpu_mode (optional): Whether to make GPU active. Defaults to False.
+        """
+        monitor_fns = [
+            init_registered_module(monitor_fn, self.config, registered_score)
+            for monitor_fn in monitor_fns
+            if monitor_fn in registered_score
+        ]
+
+        if os.path.exists(from_ckpt_dir):
+            self.model.from_checkpoint(from_ckpt_dir)
+
+        global_rank = -1
+        if self.n_gpu > 1:
+            self.model = nn.parallel.DistributedDataParallel(
+                self.model,
+                device_ids=[self.local_rank],
+                output_device=self.local_rank,
+                find_unused_parameters=False,
+                broadcast_buffers=False,
             )
-            attn_weights = attn_weights.reshape(-1, *attn_weights.size()[-2:])
+            global_rank = dist.get_rank()
+
+        dev_sampler = DistributedSampler if self.n_gpu > 1 else SequentialSampler
+        if gpu_mode:
+            with ActiveGPUJob() as _:
+                dataset_dev = self.datasets.get("dev")
         else:
-            attn_weights = torch.bmm(q, k.transpose(1, 2))
+            dataset_dev = self.datasets.get("dev")
+        iter_dev = DataLoader(
+            dataset_dev,
+            sampler=dev_sampler(dataset_dev)
+            if not isinstance(dataset_dev, Iterable)
+            else None,
+            batch_size=dev_batch_size,
+            shuffle=False,
+            pin_memory=pin_memory,
+            num_workers=num_workers,
+            collate_fn=collate_fn,
+        )
+
+        results = infer(self.model.module if self.n_gpu > 1 else self.model, iter_dev)
+        if self.local_rank in [-1, 0]:
+            monitor(
+                outputs=results.outputs,
+                targets=results.targets,
+                monitor_fns=monitor_fns,
+            )
 
-        attn_weights = self.apply_sparse_mask(attn_weights, tgt_len, src_len, bsz)
+    @torch.no_grad()
+    @add_default_section_for_function("core/task/deepspeed/supervised")
+    def infer(
+        self,
+        postprocess_fn: str,
+        writer: str,
+        test_batch_size: Optional[int] = 128,
+        pin_memory: Optional[bool] = True,
+        num_workers: Optional[int] = 4,
+        max_size: Optional[int] = 10000,
+        from_ckpt_dir: Optional[str] = "./from_ckpt",
+        output_header: Optional[List] = None,
+        output_path: Optional[str] = "./cache/predict.txt",
+        postprocess_workers: Optional[int] = 2,
+        gpu_mode: Optional[bool] = False,
+    ):
+        """
+        Perform inference using the trained model.
 
-        assert list(attn_weights.size()) == [bsz * self.num_heads, tgt_len, src_len]
+        Args:
+            postprocess_fn: The post-processing function for inference.
+            writer: The writer for writing the results.
+            test_batch_size (optional): The batch size for inference. Defaults to 128.
+            pin_memory (optional): Whether to pin memory during data loading. Defaults to True.
+            num_workers (optional): The number of worker processes for data loading. Defaults to 4.
+            max_size (optional): The maximum size of the dataset for inference. Defaults to 10000.
+            from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to "./from_ckpt".
+            output_header (optional): The header for the output file. Defaults to None.
+            output_path (optional): The path to save the output file. Defaults to "./cache/predict.txt".
+            postprocess_workers (optional): The number of worker processes for post-processing. Defaults to 2.
+            gpu_mode (optional): Whether to make GPU active. Defaults to False.
+        """
+        assert self.n_gpu <= 1
+        assert writer is not None
 
-        if attn_mask is not None:
-            attn_mask = attn_mask.unsqueeze(0)
-            if self.onnx_trace:
-                attn_mask = attn_mask.repeat(attn_weights.size(0), 1, 1)
-            attn_weights += attn_mask
-
-        if key_padding_mask is not None:
-            # don't attend to padding symbols
-            attn_weights = attn_weights.view(bsz, self.num_heads, tgt_len, src_len)
-            attn_weights = attn_weights.view(
-                kv_bsz, -1, self.num_heads, tgt_len, src_len
+        output_dir = os.path.dirname(output_path)
+        if not os.path.exists(output_dir):
+            os.makedirs(output_dir, exist_ok=True)
+
+        if postprocess_fn is not None:
+            postprocess_fn = init_registered_process(postprocess_fn, self.config)
+
+        if writer is not None:
+            writer = init_registered_module(
+                writer,
+                self.config,
+                registered_writer,
+                output_file=output_path,
             )
 
-            if not is_tpu:
-                attn_weights = attn_weights.masked_fill(
-                    key_padding_mask.unsqueeze(1)
-                    .unsqueeze(2)
-                    .unsqueeze(3)
-                    .to(torch.bool),
-                    float("-inf"),
-                )
-            else:
-                attn_weights = attn_weights.transpose(0, 2)
-                attn_weights = attn_weights.masked_fill(key_padding_mask, float("-inf"))
-                attn_weights = attn_weights.transpose(0, 2)
-            attn_weights = attn_weights.view(bsz * self.num_heads, tgt_len, src_len)
-
-        if before_softmax:
-            return attn_weights, v
+        skip_step = writer.skip_n_samples
 
-        attn_weights_float = utils.softmax(
-            attn_weights, dim=-1, onnx_trace=self.onnx_trace
-        )
-        attn_weights = attn_weights_float.type_as(attn_weights)
-        attn_probs = self.dropout_module(attn_weights)
+        if os.path.exists(from_ckpt_dir):
+            self.model.from_checkpoint(from_ckpt_dir)
 
-        assert v is not None
-        if self.encoder_decoder_attention == True and bsz != kv_bsz:
-            attn = torch.einsum(
-                "bxhts,bhsd->bxhtd",
-                attn_probs.view(kv_bsz, -1, self.num_heads, *attn_probs.size()[1:]),
-                v.view(kv_bsz, self.num_heads, *v.size()[1:]),
-            )
-            attn = attn.reshape(-1, *attn.size()[-2:])
-        else:
-            attn = torch.bmm(attn_probs, v)
-        assert list(attn.size()) == [bsz * self.num_heads, tgt_len, self.head_dim]
-        if self.onnx_trace and attn.size(1) == 1:
-            # when ONNX tracing a single decoder step (sequence length == 1)
-            # the transpose is a no-op copy before view, thus unnecessary
-            attn = attn.contiguous().view(tgt_len, bsz, embed_dim)
+        if skip_step == 0:
+            sampler = SequentialSampler
         else:
-            attn = attn.transpose(0, 1).contiguous().view(tgt_len, bsz, embed_dim)
-        attn = self.out_proj(attn)
-        attn_weights: Optional[Tensor] = None
-        if need_weights:
-            attn_weights = attn_weights_float.view(
-                bsz, self.num_heads, tgt_len, src_len
-            ).transpose(1, 0)
-            if not need_head_weights:
-                # average attention weights over heads
-                attn_weights = attn_weights.mean(dim=0)
-
-        return attn, attn_weights
-
-
-class MassConfig(PretrainedConfig):
-    def __init__(self, params: dict):
-        super().__init__(**params)
-        self.adaptive_softmax_cutoff = None
-        self.max_source_positions = params.get("max_source_positions", 512)
-        self.max_target_positions = params.get("max_target_positions", 512)
-        self.pad_token_id = params.get("pad_token_id", 0)
-
-
-class Mass(core_model_class):
-    def __init__(self, config_path, **kwargs):
-        super().__init__()
-        self.config_path = config_path
-        self.config = MassConfig(json.load(open(self.config_path, "r")))
-
-    @classmethod
-    def init_from_core_configure(cls, cfg, **kwargs):
-        pass
+            sampler = SequentialSkipSampler
 
-    def save_checkpoint(self, ckpt_dir="./cache", **kwargs):
-        if not os.path.exists(ckpt_dir):
-            os.mkdir(ckpt_dir)
-        config_path = os.path.join(ckpt_dir, CONFIG_NAME)
-        with open(config_path, "w") as f:
-            f.write(open(self.config_path, "r").read())
-
-        super().save_checkpoint(ckpt_dir=ckpt_dir, **kwargs)
-
-    def from_checkpoint(self, ckpt_dir="./cache", **kwargs):
-        super().from_checkpoint(ckpt_dir=ckpt_dir, **kwargs)
-
-
-@register_model("core/model/mass_for_generation", generation_model_decorator)
-class MassForGeneration(Mass, GenerationMixinV2):
-    def __init__(self, config_path, vocab_path):
-        super().__init__(config_path)
-
-        self.dictionary = BertDictionary.load_from_file(vocab_path)
-        self.shared = nn.Embedding(
-            self.config.vocab_size, self.config.encoder_embed_dim, 0
-        )
+        if gpu_mode:
+            with ActiveGPUJob() as _:
+                dataset_test = self.datasets.get("test")
+        else:
+            dataset_test = self.datasets.get("test")
 
-        self.encoder = TransformerEncoder(
-            self.config, dictionary=self.dictionary, embed_tokens=self.shared
+        iter_test = DataLoader(
+            dataset_test,
+            sampler=sampler(dataset_test)
+            if not isinstance(dataset_test, Iterable)
+            else None,
+            batch_size=test_batch_size,
+            shuffle=False,
+            pin_memory=pin_memory,
+            num_workers=num_workers,
+            collate_fn=collate_fn,
         )
-        self.decoder = TransformerDecoder(
-            self.config,
-            dictionary=self.dictionary,
-            embed_tokens=self.shared,
-        )
-        self.init_weights()
-
-    def get_input_embeddings(self):
-        return self.shared
 
-    def set_input_embeddings(self, value):
-        self.shared = value
-        self.encoder.embed_tokens = self.shared
-        self.decoder.embed_tokens = self.shared
+        if skip_step > 0:
+            output_file = open(output_path, "a")
+        else:
+            output_file = open(output_path, "w")
 
-    def get_encoder(self):
-        return self.encoder
+        if skip_step > 0 and hasattr(dataset_test, "set_skip_step"):
+            dataset_test.set_skip_step(skip_step)
 
-    def get_decoder(self):
-        return self.decoder
+        if skip_step > 0 and hasattr(iter_test.sampler, "set_skip_step"):
+            iter_test.sampler.set_skip_step(skip_step)
 
-    @property
-    def device(self) -> device:
-        """
-        :obj:`torch.device`: The device on which the module is (assuming that all the module parameters are on the same
-        device).
-        """
-        try:
-            return next(self.parameters()).device
-        except StopIteration:
-            # For nn.DataParallel compatibility in PyTorch 1.5
-
-            def find_tensor_attributes(module: nn.Module) -> List[Tuple[str, Tensor]]:
-                tuples = [
-                    (k, v) for k, v in module.__dict__.items() if torch.is_tensor(v)
-                ]
-                return tuples
-
-            gen = self._named_members(get_members_fn=find_tensor_attributes)
-            first_tuple = next(gen)
-            return first_tuple[1].device
-
-    @classmethod
-    @add_default_section_for_init("core/model/mass")
-    def init_from_core_configure(cls, cfg, **kwargs):
-        pretrained_name = cfg.getdefault(
-            "core/model/mass", "pretrained_name", "default-mass"
-        )
-        config_name_or_path = cfg.getdefault(
-            "core/model/mass", "config_name_or_path", pretrained_name
-        )
-        config_path = (
-            CORE_MASS_PRETRAINED_DICT[config_name_or_path][CONFIG_KEY]
-            if config_name_or_path in CORE_MASS_PRETRAINED_DICT
-            else config_name_or_path
-        )
-
-        config_path = hf_cached_path(config_path)
+        if hasattr(dataset_test, "dataset"):
+            data_info = dataset_test.dataset
+            data_info = DatasetFeature(data_info)
+            iter_data = DataLoader(
+                deepcopy(data_info),
+                sampler=sampler(data_info)
+                if not isinstance(dataset_test, Iterable)
+                else None,
+                batch_size=test_batch_size,
+                shuffle=False,
+                pin_memory=pin_memory,
+                num_workers=num_workers,
+                collate_fn=None,
+            )
+        else:
+            iter_data = None
 
-        vocab_name_or_path = cfg.getdefault(
-            "core/model/mass", "vocab_name_or_path", pretrained_name
-        )
-        vocab_path = (
-            CORE_MASS_PRETRAINED_DICT[vocab_name_or_path][VOCABS_KEY]
-            if vocab_name_or_path in CORE_MASS_PRETRAINED_DICT
-            else vocab_name_or_path
-        )
+        if skip_step > 0 and hasattr(iter_data.sampler, "set_skip_step"):
+            iter_data.sampler.set_skip_step(skip_step)
 
-        vocab_path = hf_cached_path(vocab_path)
+        self.model.eval()
+        start = time.time()
 
-        inst = cls(config_path, vocab_path)
-        if pretrained_name is not None:
-            inst.from_pretrained(pretrained_name)
-
-        return inst
-
-    def _prepare_encoder_decoder_kwargs_for_generation(
-        self, input_ids: torch.LongTensor, model_kwargs
-    ) -> Dict[str, Any]:
-        # retrieve encoder hidden states
-        encoder = self.get_encoder()
-        encoder_kwargs = {
-            argument: value
-            for argument, value in model_kwargs.items()
-            if not argument.startswith("decoder_")
-        }
-        encoder_outputs = encoder(input_ids, src_lengths=input_ids.ne(0).sum(-1))
-        model_kwargs["encoder_outputs"] = ModelOutput(
-            dict(
-                encoder_out=encoder_outputs.encoder_out,
-                last_hidden_state=encoder_outputs.encoder_out.transpose(0, 1),
-                encoder_padding_mask=encoder_outputs.encoder_padding_mask,
+        data_queue = Queue(maxsize=max_size)
+        msg_queue = Queue(maxsize=max_size)
+        postprocess_list = []
+        for _ in range(postprocess_workers):
+            p = PostProcess(
+                postprocess_fn,
+                data_queue,
+                msg_queue,
             )
-        )
-        return model_kwargs
-
-    def prepare_inputs_for_generation(
-        self,
-        decoder_input_ids,
-        past=None,
-        attention_mask=None,
-        head_mask=None,
-        use_cache=None,
-        encoder_outputs=None,
-        **kwargs,
-    ):
-        if past is not None:
-            decoder_input_ids = decoder_input_ids[:, -1:]
-
-        if hasattr(encoder_outputs, "last_hidden_state"):
-            delattr(encoder_outputs, "last_hidden_state")
+            postprocess_list.append(p)
+            p.start()
 
-        return {
-            "decoder_input_ids": decoder_input_ids,
-            "attention_mask": attention_mask,
-            "encoder_outputs": encoder_outputs,
-            "incremental_state": past,
-        }
-
-    @staticmethod
-    def _reorder_cache(past, beam_idx):
-        reordered_past = OrderedDict()
-        for i, (key, attn_cache) in enumerate(past.items()):
-            if i % 2 == 0:
-                reordered_past[key] = _reorder_buffer(attn_cache, beam_idx)
-            else:
-                reordered_past[key] = attn_cache
-        return reordered_past
-
-    @staticmethod
-    def _reorder_cache_v2(past, batch_idx, beam_idx):
-        reordered_past = OrderedDict()
-        for i, (key, attn_cache) in enumerate(past.items()):
-            if i % 2 == 0:
-                reordered_past[key] = _reorder_buffer(attn_cache, beam_idx)
-            else:
-                reordered_past[key] = _reorder_buffer(attn_cache, batch_idx)
-        return reordered_past
+        io_process = IOProcess(msg_queue, writer=writer)
+        io_process.start()
 
-    def forward(
-        self,
-        tokens_ids_a=None,
-        tokens_ids_b=None,
-        decoder_input_ids=None,
-        encoder_outputs=None,
-        incremental_state=None,
-        decoder_length=None,
-        attention_mask=None,
-        output_attentions=None,
-        output_hidden_states=None,
-        return_dict=None,
-    ):
-        if self.training:
-            encoder_outputs = self.encoder(
-                tokens_ids_a, src_lengths=tokens_ids_a.ne(0).sum(-1)
+        if iter_data is None:
+            for step, (inputs, _) in enumerate(iter_test):
+                if torch.cuda.is_available():
+                    inputs = inputs.cuda()
+                outputs = self.model(**inputs.dict())
+                outputs = outputs.cpu()
+                data_queue.put((step, outputs))
+        else:
+            for step, ((inputs, _), _infos) in enumerate(zip(iter_test, iter_data)):
+                if torch.cuda.is_available():
+                    inputs = inputs.cuda()
+                outputs = self.model(**inputs.dict())
+                outputs = outputs.cpu()
+                if output_header is not None:
+                    _infos = {k: _infos[k] for k in output_header if k in _infos}
+                    outputs.set_base_dataframe(pd.DataFrame(_infos))
+                data_queue.put((step, outputs))
+
+        data_queue.put((-1, GENERATE_FINISHED))
+        for p in postprocess_list:
+            p.join()
+
+        msg_queue.put((-1, GENERATE_FINISHED))
+        io_process.join()
+
+        end = time.time()
+        ms = (end - start) * 1000
+        logging.info(
+            "{:.2f} ms, {:.1f} sample/s".format(
+                ms,
+                ((len(dataset_test) - skip_step) / ms * 1000),
             )
-            decoder_outputs = self.decoder(tokens_ids_b, encoder_out=encoder_outputs)
-            return decoder_outputs[0]
-        if incremental_state is None:
-            incremental_state = OrderedDict()
-
-        decoder_outputs = self.decoder(
-            decoder_input_ids,
-            encoder_out=encoder_outputs,
-            incremental_state=incremental_state,
-        )
-        return Seq2SeqLMOutput(
-            logits=decoder_outputs[0], past_key_values=incremental_state
-        )
-
-    @add_default_section_for_instance_function("core/model/mass")
-    def generate(
-        self,
-        tokens_ids,
-        num_beams=5,
-        decoder_start_token_id=101,
-        decoder_end_token_id=102,
-        num_return_sequences=1,
-        min_gen_seq_length=0,
-        max_gen_seq_length=48,
-        repetition_penalty=1.0,
-        no_repeat_ngram_size=0,
-        early_stopping=True,
-        length_penalty=1.0,
-        num_beam_groups=1,
-        diversity_penalty=0.0,
-        diverse_rate=0.0,
-    ):
-        self.num_beams = num_beams
-        batch_hyp = super().generate(
-            tokens_ids,
-            max_length=max_gen_seq_length,
-            min_length=min_gen_seq_length,
-            num_beams=num_beams,
-            do_sample=False,
-            decoder_start_token_id=decoder_start_token_id,
-            no_repeat_ngram_size=no_repeat_ngram_size,
-            early_stopping=early_stopping,
-            length_penalty=length_penalty,
-            repetition_penalty=repetition_penalty,
-            num_return_sequences=num_return_sequences,
-            bos_token_id=decoder_start_token_id,
-            eos_token_id=decoder_end_token_id,
-            num_beam_groups=num_beam_groups,
-            diversity_penalty=diversity_penalty,
-        )
-        batch_hyp = batch_hyp.reshape(-1, num_return_sequences, batch_hyp.size(-1))
-        if batch_hyp.size(-1) >= max_gen_seq_length:
-            return batch_hyp[:, :, :max_gen_seq_length]
-        batch_ret = torch.zeros(
-            batch_hyp.size(0), num_return_sequences, max_gen_seq_length
         )
-        batch_ret[:, :, : batch_hyp.size(-1)].copy_(batch_hyp)
-        return batch_ret.long()
```

### Comparing `unitorch-0.0.0.1/unitorch/score/rouge.py` & `unitorch-0.0.0.2/src/unitorch/score/rouge.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-from unitorch import register_score, core_process
-from unitorch.core import core_class
+# Copyright (c) FULIUCANSHENG.
+# Licensed under the MIT License.
+
+import torch
 import itertools
-from unitorch.utils.decorators import add_default_section_for_init
-from unitorch.functions import pop_first_non_none_value
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
+from unitorch.score import (
+    convert_tensor_to_strings,
+    remove_strings_ignore_tokens,
+)
 
 
 def _get_ngrams(n, text):
     """Calcualtes n-grams.
     Args:
       n: which n-grams to calculate
       text: An array of tokens
@@ -100,22 +105,22 @@
         else:
             return _recon(i, j - 1)
 
     recon_tuple = tuple(map(lambda x: x[0], _recon(i, j)))
     return recon_tuple
 
 
-def multi_rouge_n(sequences, scores_ids, n=2):
+def _multi_rouge_n(sequences, scores_ids, n=2):
     """
     Efficient way to compute highly repetitive scoring
     i.e. sequences are involved multiple time
     Args:
         sequences(list[str]): list of sequences (either hyp or ref)
         scores_ids(list[tuple(int)]): list of pairs (hyp_id, ref_id)
-            ie. scores[i] = rouge_n(scores_ids[i][0],
+            ie. scores[i] = _rouge_n(scores_ids[i][0],
                                     scores_ids[i][1])
     Returns:
         scores: list of length `len(scores_ids)` containing rouge `n`
                 scores as a dict with 'f', 'r', 'p'
     Raises:
         KeyError: if there's a value of i in scores_ids that is not in
                   [0, len(sequences)[
@@ -130,19 +135,19 @@
 
         reference_ngrams = ngrams[ref_id]
         reference_count = counts[ref_id]
 
         overlapping_ngrams = evaluated_ngrams.intersection(reference_ngrams)
         overlapping_count = len(overlapping_ngrams)
 
-        scores += [f_r_p_rouge_n(evaluated_count, reference_count, overlapping_count)]
+        scores += [_f_r_p_rouge_n(evaluated_count, reference_count, overlapping_count)]
     return scores
 
 
-def rouge_n(evaluated_sentences, reference_sentences, n=2):
+def _rouge_n(evaluated_sentences, reference_sentences, n=2):
     """
     Computes ROUGE-N of two text collections of sentences.
     Sourece: http://research.microsoft.com/en-us/um/people/cyl/download/
     papers/rouge-working-note-v1.3.1.pdf
     Args:
       evaluated_sentences: The sentences that have been picked by the
                            summarizer
@@ -163,18 +168,18 @@
     reference_count = len(reference_ngrams)
     evaluated_count = len(evaluated_ngrams)
 
     # Gets the overlapping ngrams between evaluated and reference
     overlapping_ngrams = evaluated_ngrams.intersection(reference_ngrams)
     overlapping_count = len(overlapping_ngrams)
 
-    return f_r_p_rouge_n(evaluated_count, reference_count, overlapping_count)
+    return _f_r_p_rouge_n(evaluated_count, reference_count, overlapping_count)
 
 
-def f_r_p_rouge_n(evaluated_count, reference_count, overlapping_count):
+def _f_r_p_rouge_n(evaluated_count, reference_count, overlapping_count):
     # Handle edge case. This isn't mathematically correct, but it's good enough
     if evaluated_count == 0:
         precision = 0.0
     else:
         precision = overlapping_count / evaluated_count
 
     if reference_count == 0:
@@ -223,15 +228,15 @@
         combined_lcs_length += len(lcs)
         lcs_union = lcs_union.union(lcs)
 
     new_lcs_count = len(lcs_union) - prev_count
     return new_lcs_count, lcs_union
 
 
-def rouge_l_summary_level(evaluated_sentences, reference_sentences):
+def _rouge_l_summary_level(evaluated_sentences, reference_sentences):
     """
     Computes ROUGE-L (summary level) of two text collections of sentences.
     http://research.microsoft.com/en-us/um/people/cyl/download/papers/
     rouge-working-note-v1.3.1.pdf
     Calculated according to:
     R_lcs = SUM(1, u)[LCS<union>(r_i,C)]/m
     P_lcs = SUM(1, u)[LCS<union>(r_i,C)]/n
@@ -267,119 +272,128 @@
         lcs_count, union = _union_lcs(evaluated_sentences, ref_s, prev_union=union)
         union_lcs_sum_across_all_references += lcs_count
 
     llcs = union_lcs_sum_across_all_references
     r_lcs = llcs / m
     p_lcs = llcs / n
     beta = p_lcs / (r_lcs + 1e-12)
-    num = (1 + (beta ** 2)) * r_lcs * p_lcs
-    denom = r_lcs + ((beta ** 2) * p_lcs)
+    num = (1 + (beta**2)) * r_lcs * p_lcs
+    denom = r_lcs + ((beta**2) * p_lcs)
     f_lcs = num / (denom + 1e-12)
     return {"f": f_lcs, "p": p_lcs, "r": r_lcs}
 
 
-class core_rouge_score(core_class):
-    def __init__(self, process_fn=None, rouge_fn=None, pad_token_id=0):
-        self.process_fn = process_fn
-        self.keys_for_label = ["tokens_ids", "next_tokens_ids"]
-        self.pad_token_id = pad_token_id
-        self.rouge_fn = rouge_fn
-
-    def default_process_fn(self, tensor):
-        if tensor.dim() == 3:
-            ret = [
-                list(
-                    [
-                        list(
-                            map(
-                                lambda x: str(int(x)),
-                                filter(lambda x: x != self.pad_token_id, t2),
-                            )
-                        )
-                        for t2 in t1
-                    ]
-                )
-                for t1 in tensor
-            ]
-        elif tensor.dim() == 2:
-            ret = [
-                [
-                    list(
-                        map(
-                            lambda x: str(int(x)),
-                            filter(lambda x: x != self.pad_token_id, t1),
-                        )
-                    )
-                ]
-                for t1 in tensor
-            ]
-        else:
-            raise f"tensor dim extracted 2-dim or 3-dim, but get size of {tensor.size()}"
-        return ret
-
-    def __call__(self, net_outputs, net_targets):
-        net_targets = pop_first_non_none_value(
-            *[net_targets.get(k) for k in self.keys_for_label]
-        )
-        # net_outputs / net_targets is 2dim or 3dim
-        if self.process_fn is not None:
-            net_outputs = self.process_fn(net_outputs)
-            net_targets = self.process_fn(net_targets)
-        else:
-            net_outputs = self.default_process_fn(net_outputs)
-            net_targets = self.default_process_fn(net_targets)
-        net_outputs = [output[0] for output in net_outputs]
-        net_targets = [target[0] for target in net_targets]
-        num = len(net_outputs)
-        pre, rec, f1 = 0, 0, 0
-        for target, output in zip(net_targets, net_outputs):
-            r = self.rouge_fn(output, target)
-            pre += r["p"]
-            rec += r["r"]
-            f1 += r["f"]
-        pre, rec, f1 = pre / num, rec / num, f1 / num
-        return f1
-
-
-@register_score("core/score/rouge1")
-class core_rouge1_score(core_rouge_score):
-    def __init__(self, process_fn=None, pad_token_id=0):
-        super().__init__(
-            process_fn=process_fn,
-            rouge_fn=lambda x, y: rouge_n(x, y, n=1),
-            pad_token_id=pad_token_id,
-        )
-
-    @classmethod
-    @add_default_section_for_init("core/score/rouge")
-    def init_from_core_configure(cls, cfg, **kwargs):
-        pass
-
-
-@register_score("core/score/rouge2")
-class core_rouge2_score(core_rouge_score):
-    def __init__(self, process_fn=None, pad_token_id=0):
-        super().__init__(
-            process_fn=process_fn,
-            rouge_fn=lambda x, y: rouge_n(x, y, n=2),
-            pad_token_id=pad_token_id,
-        )
-
-    @classmethod
-    @add_default_section_for_init("core/score/rouge")
-    def init_from_core_configure(cls, cfg, **kwargs):
-        pass
-
-
-@register_score("core/score/rougel")
-class core_rougel_score(core_rouge_score):
-    def __init__(self, process_fn=None, pad_token_id=0):
-        super().__init__(
-            process_fn=process_fn,
-            rouge_fn=rouge_l_summary_level,
-            pad_token_id=pad_token_id,
-        )
-
-    @classmethod
-    @add_default_section_for_init("core/score/rouge")
-    def init_from_core_configure(cls, cfg, **kwargs):
-        pass
+def rouge1_score(
+    y_true: List[Union[str, int, List[Union[str, int]]]],
+    y_pred: List[Union[str, int, List[Union[str, int]]]],
+    ignore_tokens: Optional[List[Union[str, int]]] = None,
+):
+    """
+    Args:
+        y_true: list of lists of int/str tokens of ground truth.
+        y_pred: list of lists of int/str tokens of generation results.
+        ignore_tokens: the token list to filtration
+    """
+
+    if isinstance(y_true, torch.Tensor):
+        if y_true.dim() == 2:
+            y_true = y_true.unsqueeze(1)
+        y_true = convert_tensor_to_strings(y_true)
+
+    if isinstance(y_pred, torch.Tensor) and y_pred.dim() == 2:
+        y_pred = convert_tensor_to_strings(y_pred)
+
+    if ignore_tokens is not None:
+        ignore_tokens = [str(t) for t in ignore_tokens]
+
+    y_true = remove_strings_ignore_tokens(y_true, ignore_tokens=ignore_tokens)
+    y_pred = remove_strings_ignore_tokens(y_pred, ignore_tokens=ignore_tokens)
+
+    y_true = [_y_true[0] for _y_true in y_true]
+
+    num = len(y_pred)
+    pre, rec, f1 = 0, 0, 0
+    for t, p in zip(y_true, y_pred):
+        r = _rouge_n(p, t, n=1)
+        pre += r["p"]
+        rec += r["r"]
+        f1 += r["f"]
+    pre, rec, f1 = pre / num, rec / num, f1 / num
+    return dict(pre=pre, rec=rec, f1=f1)
+
+
+def rouge2_score(
+    y_true: List[Union[str, int, List[Union[str, int]]]],
+    y_pred: List[Union[str, int, List[Union[str, int]]]],
+    ignore_tokens: Optional[List[Union[str, int]]] = None,
+):
+    """
+    Args:
+        y_true: list of lists of int/str tokens of ground truth.
+        y_pred: list of lists of int/str tokens of generation results.
+        ignore_tokens: the token list to filtration
+    """
+
+    if isinstance(y_true, torch.Tensor):
+        if y_true.dim() == 2:
+            y_true = y_true.unsqueeze(1)
+        y_true = convert_tensor_to_strings(y_true)
+
+    if isinstance(y_pred, torch.Tensor) and y_pred.dim() == 2:
+        y_pred = convert_tensor_to_strings(y_pred)
+
+    if ignore_tokens is not None:
+        ignore_tokens = [str(t) for t in ignore_tokens]
+
+    y_true = remove_strings_ignore_tokens(y_true, ignore_tokens=ignore_tokens)
+    y_pred = remove_strings_ignore_tokens(y_pred, ignore_tokens=ignore_tokens)
+
+    y_true = [_y_true[0] for _y_true in y_true]
+
+    num = len(y_pred)
+    pre, rec, f1 = 0, 0, 0
+    for t, p in zip(y_true, y_pred):
+        r = _rouge_n(p, t, n=2)
+        pre += r["p"]
+        rec += r["r"]
+        f1 += r["f"]
+    pre, rec, f1 = pre / num, rec / num, f1 / num
+    return dict(pre=pre, rec=rec, f1=f1)
+
+
+def rougel_score(
+    y_true: List[Union[str, int, List[Union[str, int]]]],
+    y_pred: List[Union[str, int, List[Union[str, int]]]],
+    ignore_tokens: Optional[List[Union[str, int]]] = None,
+):
+    """
+    Args:
+        y_true: list of lists of int/str tokens of ground truth.
+        y_pred: list of lists of int/str tokens of generation results.
+        ignore_tokens: the token list to filtration
+    """
+
+    if isinstance(y_true, torch.Tensor):
+        if y_true.dim() == 2:
+            y_true = y_true.unsqueeze(1)
+        y_true = convert_tensor_to_strings(y_true)
+
+    if isinstance(y_pred, torch.Tensor) and y_pred.dim() == 2:
+        y_pred = convert_tensor_to_strings(y_pred)
+
+    if ignore_tokens is not None:
+        ignore_tokens = [str(t) for t in ignore_tokens]
+
+    y_true = remove_strings_ignore_tokens(y_true, ignore_tokens=ignore_tokens)
+    y_pred = remove_strings_ignore_tokens(y_pred, ignore_tokens=ignore_tokens)
+
+    y_true = [_y_true[0] for _y_true in y_true]
+
+    num = len(y_pred)
+    pre, rec, f1 = 0, 0, 0
+    for t, p in zip(y_true, y_pred):
+        r = _rouge_l_summary_level(p, t)
+        pre += r["p"]
+        rec += r["r"]
+        f1 += r["f"]
+    pre, rec, f1 = pre / num, rec / num, f1 / num
+    return dict(pre=pre, rec=rec, f1=f1)
```

### Comparing `unitorch-0.0.0.1/unitorch/process/bert.py` & `unitorch-0.0.0.2/src/unitorch/models/processing_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,297 +1,363 @@
-import os
-import random
-from functools import partial
-from random import randint, shuffle, choice
+# Copyright (c) FULIUCANSHENG.
+# Licensed under the MIT License.
 
-import numpy as np
 import torch
-from transformers import BertTokenizer
+from PIL import Image
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
+from transformers import PreTrainedTokenizer
+from transformers.image_utils import to_numpy_array, ChannelDimension
+from transformers.image_transforms import to_channel_dimension_format
+from transformers.image_processing_utils import BaseImageProcessor
+from unitorch.models import GenericOutputs
+from unitorch.utils import pop_value, truncate_sequence_pair
+
+
+class HfTextGenerationProcessor:
+    """
+    Processor for text generation tasks.
+
+    Args:
+        tokenizer (PreTrainedTokenizer): The tokenizer to use for text generation.
+        max_seq_length (int, optional): Maximum sequence length. Defaults to 128.
+        max_gen_seq_length (int, optional): Maximum generated sequence length. Defaults to 48.
+    """
 
-from unitorch.functions import pop_first_non_none_value
-from unitorch.utils.decorators import (
-    add_default_section_for_init,
-    add_key_group_info_for_process,
-)
-from unitorch import register_process
-from unitorch.core import core_class
-from unitorch.utils.hf import hf_cached_path
-from unitorch.classification.bert import CORE_BERT_PRETRAINED_DICT, VOCABS_KEY
-
-
-def get_special_vocab(tokenizer, special_tokens):
-    extra_map = dict()
-    for i in range(len(special_tokens)):
-        extra_map["[unused{}]".format(990 - i)] = special_tokens[i]
-    for k, v in extra_map.items():
-        if k in tokenizer.vocab.keys():
-            tokenizer.vocab[v] = tokenizer.vocab[k]
-    return tokenizer, extra_map
-
-
-def get_random_word(vocab_words):
-    i = randint(0, len(vocab_words) - 1)
-    return vocab_words[i]
-
-
-def _truncate_seq_pair(tokens_a, tokens_b, max_length):
-    """Truncates a sequence pair in place to the maximum length."""
-
-    # This is a simple heuristic which will always truncate the longer sequence
-    # one token at a time. This makes more sense than truncating an equal percent
-    # of tokens from each, since if one sequence is very short then each token
-    # that's truncated likely contains more information than a longer sequence.
-    while True:
-        total_length = len(tokens_a) + len(tokens_b)
-        if total_length <= max_length:
-            break
-        if len(tokens_a) > len(tokens_b):
-            tokens_a.pop()
-        else:
-            tokens_b.pop()
+    def __init__(
+        self,
+        tokenizer: PreTrainedTokenizer,
+        max_seq_length: Optional[int] = 128,
+        max_gen_seq_length: Optional[int] = 48,
+    ):
+        self.tokenizer = tokenizer
+        self.max_seq_length = max_seq_length
+        self.max_gen_seq_length = max_gen_seq_length
+        self.pad_token = self.tokenizer.pad_token
+        self.bos_token = self.tokenizer.bos_token
+        self.eos_token = self.tokenizer.eos_token
+        self.mask_token = self.tokenizer.mask_token
+        self.pad_token_id = self.tokenizer.pad_token_id
+        self.vocab_size = len(self.tokenizer.get_vocab())
 
+    def generation_inputs(
+        self,
+        text: str,
+        max_seq_length: Optional[int] = None,
+    ):
+        """
+        Generate inputs for text generation.
 
-def get_random_mask_indexes(
-    tokens,
-    masked_lm_prob=0.15,
-    do_whole_word_mask=True,
-    max_predictions_per_seq=20,
-    special_tokens=[],
-):
-    cand_indexes = []
-    for (i, token) in enumerate(tokens):
-        if token in special_tokens:
-            continue
-        if (
-            do_whole_word_mask and len(cand_indexes) >= 1 and token.startswith("##")
-        ) and cand_indexes[-1][-1] == i - 1:
-            cand_indexes[-1].append(i)
-        else:
-            cand_indexes.append([i])
-    random.shuffle(cand_indexes)
-    num_to_predict = min(
-        max_predictions_per_seq, max(1, int(round(len(tokens) * masked_lm_prob)))
-    )
-    covered_indexes = set()
-    for index_set in cand_indexes:
-        if len(covered_indexes) >= num_to_predict:
-            break
-        if len(covered_indexes) + len(index_set) > num_to_predict or any(
-            i in covered_indexes for i in index_set
-        ):
-            continue
-        covered_indexes.update(index_set)
-    return covered_indexes
-
-
-def get_bert_tokenizer(
-    vocab_path, never_split_tokens=[], do_lower_case=True, do_basic_tokenize=True
-):
-    never_split_tokens = list(filter(lambda x: x != "", never_split_tokens))
-    assert os.path.exists(vocab_path)
-    tokenizer = BertTokenizer(
-        vocab_path,
-        do_lower_case=do_lower_case,
-        do_basic_tokenize=do_basic_tokenize,
-        never_split=never_split_tokens,
-    )
-    special_tokens_map = dict()
-    if len(never_split_tokens) > 0:
-        tokenizer, special_tokens_map = get_special_vocab(tokenizer, never_split_tokens)
-    return dict({"tokenizer": tokenizer, "special_tokens_map": special_tokens_map})
+        Args:
+            text (str): The input text.
+            max_seq_length (int, optional): Maximum sequence length. Defaults to None.
+
+        Returns:
+            GenericOutputs: The generated input tokens and attention mask.
+        """
+        max_seq_length = pop_value(max_seq_length, self.max_seq_length)
+        tokens = self.tokenizer.tokenize(str(text))
+        tokens = tokens[: max_seq_length - 2]
+        tokens = [self.bos_token] + tokens + [self.eos_token]
+        input_ids = self.tokenizer.convert_tokens_to_ids(tokens)
+        input_ids = input_ids[:max_seq_length]
+        attention_mask = [1] * len(input_ids)
 
+        padding = [0] * (max_seq_length - len(input_ids))
+        input_ids += [self.pad_token_id] * len(padding)
+        attention_mask += padding
 
-class Bert(core_class):
-    def __init__(
+        assert len(input_ids) == max_seq_length
+        assert len(attention_mask) == max_seq_length
+
+        return GenericOutputs(
+            input_ids=torch.tensor(input_ids, dtype=torch.long),
+            attention_mask=torch.tensor(attention_mask, dtype=torch.long),
+        )
+
+    def generation_labels(
         self,
-        vocab_path,
-        max_seq_length=128,
-        never_split_tokens=[],
-        do_lower_case=True,
-        do_whole_word_mask=True,
-        masked_lm_prob=0.15,
-        max_predictions_per_seq=20,
+        text: str,
+        max_gen_seq_length: Optional[int] = None,
     ):
-        self.max_seq_length = max_seq_length
-        tokenizer_and_special_token_map = get_bert_tokenizer(
-            vocab_path, never_split_tokens, do_lower_case
-        )
-        self.tokenizer = tokenizer_and_special_token_map.get("tokenizer")
-        self.special_tokens_map = tokenizer_and_special_token_map.get(
-            "special_tokens_map"
+        """
+        Generate labels for text generation.
+
+        Args:
+            text (str): The input text.
+            max_gen_seq_length (int, optional): Maximum generated sequence length. Defaults to None.
+
+        Returns:
+            GenericOutputs: The generated label tokens and attention mask.
+        """
+        max_gen_seq_length = pop_value(max_gen_seq_length, self.max_gen_seq_length)
+        tokens = self.tokenizer.tokenize(str(text))
+        tokens = tokens[: max_gen_seq_length - 2]
+        tokens = [self.bos_token] + tokens + [self.eos_token]
+        input_ids = self.tokenizer.convert_tokens_to_ids(tokens)
+        input_ids = input_ids[1:max_gen_seq_length]
+        attention_mask = [1] * len(input_ids)
+
+        padding = [0] * (max_gen_seq_length - len(input_ids))
+        input_ids += [self.pad_token_id] * len(padding)
+        attention_mask += padding
+
+        assert len(input_ids) == max_gen_seq_length
+
+        return GenericOutputs(
+            input_ids=torch.tensor(input_ids, dtype=torch.long),
+            attention_mask=torch.tensor(attention_mask, dtype=torch.long),
         )
-        self.do_whole_word_mask = do_whole_word_mask
-        self.masked_lm_prob = masked_lm_prob
-        self.max_predictions_per_seq = max_predictions_per_seq
-        self.vocab_words = list(self.tokenizer.vocab.keys())
-
-    @classmethod
-    @add_default_section_for_init("core/process/bert")
-    def init_from_core_configure(cls, cfg, **kwargs):
-        never_split_tokens = cfg.getdefault(
-            "core/process/bert", "never_split_tokens", None
+
+    def generation(
+        self,
+        text: str,
+        text_pair: str,
+        max_seq_length: Optional[int] = None,
+        max_gen_seq_length: Optional[int] = None,
+    ):
+        """
+        Generate inputs, labels, and tokens for text generation.
+
+        Args:
+            text (str): The input text.
+            text_pair (str): The paired text.
+            max_seq_length (int, optional): Maximum sequence length. Defaults to None.
+            max_gen_seq_length (int, optional): Maximum generated sequence length. Defaults to None.
+
+        Returns:
+            GenericOutputs: The generated input tokens, attention masks, label tokens, and attention masks.
+        """
+        max_seq_length = pop_value(max_seq_length, self.max_seq_length)
+        max_gen_seq_length = pop_value(max_gen_seq_length, self.max_gen_seq_length)
+
+        tokens = self.generation_inputs(text, max_seq_length)
+        tokens_pair = self.generation_inputs(text_pair, max_gen_seq_length)
+        labels = self.generation_labels(text_pair, max_gen_seq_length)
+
+        return GenericOutputs(
+            input_ids=tokens.input_ids,
+            attention_mask=tokens.attention_mask,
+            input_ids_pair=tokens_pair.input_ids,
+            attention_mask_pair=tokens_pair.attention_mask,
+            input_ids_label=labels.input_ids,
+            attention_mask_label=labels.attention_mask,
         )
-        if never_split_tokens is not None:
-            never_split_tokens = eval(never_split_tokens)
+
+    def detokenize(
+        self,
+        sequences: torch.Tensor,
+        skip_special_tokens: Optional[bool] = True,
+    ):
+        """
+        Detokenize the sequences.
+
+        Args:
+            sequences (torch.Tensor): The sequences to detokenize.
+            skip_special_tokens (bool, optional): Whether to skip special tokens. Defaults to True.
+
+        Returns:
+            list: The detokenized sequences.
+        """
+        if sequences.dim() == 3:
+            _, num_return_sequences, sequences_length = sequences.size()
+            sequences = sequences.reshape(-1, sequences_length).clamp_max(
+                self.vocab_size
+            )
+            sequences = sequences.clamp_min(0)
+            sequences[sequences == self.vocab_size] = self.pad_token_id
+            decode_tokens = self.tokenizer.batch_decode(
+                sequences,
+                skip_special_tokens=skip_special_tokens,
+            )
+            decode_tokens = [
+                decode_tokens[i : i + num_return_sequences]
+                for i in range(0, len(decode_tokens), num_return_sequences)
+            ]
+        elif sequences.dim() == 2:
+            sequences = sequences.clamp_min(0).clamp_max(self.vocab_size)
+            sequences[sequences == self.vocab_size] = self.pad_token_id
+            decode_tokens = self.tokenizer.batch_decode(
+                sequences,
+                skip_special_tokens=skip_special_tokens,
+            )
         else:
-            never_split_tokens = []
+            raise ValueError(f"Can't decode the tensor with shape {sequences.shape}")
 
-        pretrained_name = cfg.getdefault(
-            "core/process/bert", "pretrained_name", "default-bert"
-        )
-        vocab_name_or_path = cfg.getdefault(
-            "core/process/bert", "vocab_name_or_path", pretrained_name
-        )
-        vocab_path = (
-            CORE_BERT_PRETRAINED_DICT[vocab_name_or_path][VOCABS_KEY]
-            if vocab_name_or_path in CORE_BERT_PRETRAINED_DICT
-            else vocab_name_or_path
-        )
+        return decode_tokens
 
-        vocab_path = hf_cached_path(vocab_path)
 
-        return dict(
-            {
-                "vocab_path": vocab_path,
-                "never_split_tokens": never_split_tokens,
-            }
-        )
+class HfTextClassificationProcessor:
+    """
+    Processor for text classification tasks.
+
+    Args:
+        tokenizer (PreTrainedTokenizer): The tokenizer to use for text classification.
+        max_seq_length (int, optional): Maximum sequence length. Defaults to 128.
+        source_type_id (int, optional): Source type ID. Defaults to 0.
+        target_type_id (int, optional): Target type ID. Defaults to 1.
+        position_start_id (int, optional): Start position ID. Defaults to 0.
+    """
 
-    @add_key_group_info_for_process(
-        group_info=dict(
-            name="core/process/bert_for_seq",
-            net_inputs=["tokens_ids", "seg_ids", "attn_mask", "pos_ids"],
-        )
-    )
-    @register_process("core/process/bert_for_seq")
-    def for_seq(self, text, max_seq_length=None):
-        max_seq_length = int(
-            pop_first_non_none_value(max_seq_length, self.max_seq_length)
-        )
-        tokens = self.tokenizer.tokenize(text)
-        tokens = tokens[: max_seq_length - 2]
-        tokens = ["[CLS]"] + tokens + ["[SEP]"]
-        tokens_ids = self.tokenizer.convert_tokens_to_ids(tokens)
-        segment_ids = [0] * len(tokens_ids)
-        tokens_mask = [1] * len(tokens_ids)
-
-        padding = [0] * (max_seq_length - len(tokens_ids))
-        tokens_ids += padding
-        tokens_mask += padding
-        segment_ids += len(padding) * [1]
-
-        assert len(tokens_ids) == max_seq_length
-        assert len(tokens_mask) == max_seq_length
-        assert len(segment_ids) == max_seq_length
-        return dict(
-            {
-                "tokens_ids": torch.tensor(tokens_ids, dtype=torch.long),
-                "seg_ids": torch.tensor(segment_ids, dtype=torch.long),
-                "attn_mask": torch.tensor(tokens_mask, dtype=torch.long),
-                "pos_ids": torch.tensor(list(range(max_seq_length)), dtype=torch.long),
-            }
-        )
+    def __init__(
+        self,
+        tokenizer: PreTrainedTokenizer,
+        max_seq_length: Optional[int] = 128,
+        source_type_id: Optional[int] = 0,
+        target_type_id: Optional[int] = 1,
+        position_start_id: Optional[int] = 0,
+    ):
+        self.tokenizer = tokenizer
+        self.max_seq_length = max_seq_length
+        self.pad_token = self.tokenizer.pad_token
+        self.sep_token = self.tokenizer.sep_token
+        self.cls_token = self.tokenizer.cls_token
+        self.mask_token = self.tokenizer.mask_token
+        self.pad_token_id = self.tokenizer.pad_token_id
+        self.source_type_id = source_type_id
+        self.target_type_id = target_type_id
+        self.position_start_id = position_start_id
 
-    @add_key_group_info_for_process(
-        group_info=dict(
-            name="core/process/bert_for_pair",
-            net_inputs=["tokens_ids", "seg_ids", "attn_mask", "pos_ids"],
-        )
-    )
-    @register_process("core/process/bert_for_pair")
-    def for_pair(self, text_a, text_b, max_seq_length=None):
-        max_seq_length = int(
-            pop_first_non_none_value(max_seq_length, self.max_seq_length)
-        )
-        tokens_a = self.tokenizer.tokenize(text_a)
-        tokens_b = self.tokenizer.tokenize(text_b)
-        _truncate_seq_pair(tokens_a, tokens_b, max_seq_length - 3)
-        tokens = ["[CLS]"] + tokens_a + ["[SEP]"] + tokens_b + ["[SEP]"]
-        tokens_ids = self.tokenizer.convert_tokens_to_ids(tokens)
-        segment_ids = [0] + [0] * len(tokens_a) + [0] + [1] * len(tokens_b) + [1]
-        tokens_mask = [1] * len(tokens_ids)
-
-        padding = [0] * (max_seq_length - len(tokens_ids))
-        tokens_ids += padding
-        tokens_mask += padding
-        segment_ids += len(padding) * [1]
-
-        assert len(tokens_ids) == max_seq_length
-        assert len(tokens_mask) == max_seq_length
-        assert len(segment_ids) == max_seq_length
-        return dict(
-            {
-                "tokens_ids": torch.tensor(tokens_ids, dtype=torch.long),
-                "seg_ids": torch.tensor(segment_ids, dtype=torch.long),
-                "attn_mask": torch.tensor(tokens_mask, dtype=torch.long),
-                "pos_ids": torch.tensor(list(range(max_seq_length)), dtype=torch.long),
-            }
-        )
+    def classification(
+        self,
+        text: str,
+        text_pair: Optional[str] = None,
+        max_seq_length: Optional[int] = None,
+    ):
+        """
+        Generate inputs for text classification.
 
-    @add_key_group_info_for_process(
-        group_info=dict(
-            name="core/process/bert_for_pretrain",
-            net_inputs=["tokens_ids", "seg_ids", "attn_mask", "pos_ids"],
-            net_targets=["nsp_label", "mlm_label", "mlm_label_mask"],
-        )
-    )
-    @register_process("core/process/bert_for_pretrain")
-    def for_pretrain(self, text_a, text_b, nsp_label, max_seq_length=None):
-        max_seq_length = int(
-            pop_first_non_none_value(max_seq_length, self.max_seq_length)
-        )
-        tokens_a = self.tokenizer.tokenize(text_a)
-        tokens_b = self.tokenizer.tokenize(text_b)
-        _truncate_seq_pair(tokens_a, tokens_b, max_seq_length - 3)
-        tokens = ["[CLS]"] + tokens_a + ["[SEP]"] + tokens_b + ["[SEP]"]
-
-        covered_indexes = get_random_mask_indexes(
-            tokens,
-            self.masked_lm_prob,
-            do_whole_word_mask,
-            max_predictions_per_seq,
-            special_tokens=["[CLS]", "[SEP]"],
+        Args:
+            text (str): The input text.
+            text_pair (str, optional): The paired text. Defaults to None.
+            max_seq_length (int, optional): Maximum sequence length. Defaults to None.
+
+        Returns:
+            GenericOutputs: The generated input tokens, token type IDs, attention mask, and position IDs.
+        """
+        max_seq_length = pop_value(
+            max_seq_length,
+            self.max_seq_length,
+        )
+
+        tokens = self.tokenizer.tokenize(str(text))
+        if text_pair is None:
+            tokens = tokens[: max_seq_length - 2]
+            tokens = [self.cls_token] + tokens + [self.sep_token]
+            input_ids = self.tokenizer.convert_tokens_to_ids(tokens)
+            token_type_ids = [self.source_type_id] * len(input_ids)
+            attention_mask = [1] * len(input_ids)
+        else:
+            tokens_pair = self.tokenizer.tokenize(str(text_pair))
+            truncate_sequence_pair(tokens, tokens_pair, max_seq_length - 3)
+            token_type_ids = (
+                [self.source_type_id]
+                + [self.source_type_id] * len(tokens)
+                + [self.source_type_id]
+                + [self.target_type_id] * len(tokens_pair)
+                + [self.target_type_id]
+            )
+            tokens = (
+                [self.cls_token]
+                + tokens
+                + [self.sep_token]
+                + tokens_pair
+                + [self.sep_token]
+            )
+            input_ids = self.tokenizer.convert_tokens_to_ids(tokens)
+            attention_mask = [1] * len(input_ids)
+
+        padding = [0] * (max_seq_length - len(input_ids))
+        input_ids += len(padding) * [self.pad_token_id]
+        attention_mask += padding
+        token_type_ids += len(padding) * [self.target_type_id]
+
+        assert len(input_ids) == max_seq_length
+        assert len(attention_mask) == max_seq_length
+        assert len(token_type_ids) == max_seq_length
+        return GenericOutputs(
+            input_ids=torch.tensor(input_ids, dtype=torch.long),
+            token_type_ids=torch.tensor(token_type_ids, dtype=torch.long),
+            attention_mask=torch.tensor(attention_mask, dtype=torch.long),
+            position_ids=torch.tensor(
+                list(
+                    range(
+                        self.position_start_id,
+                        self.position_start_id + max_seq_length,
+                    )
+                ),
+                dtype=torch.long,
+            ),
         )
-        label = [
-            tokens[pos] if pos in covered_indexes else "[PAD]"
-            for pos in range(max_seq_length)
-        ]
-        label_mask = [
-            1 if pos in covered_indexes else 0 for pos in range(max_seq_length)
-        ]
-        label = self.tokenizer.convert_tokens_to_ids(label)
-
-        for index in covered_indexes:
-            masked_token = None
-            if random.random() < 0.8:
-                masked_token = "[MASK]"
-            else:
-                masked_token = (
-                    tokens[index]
-                    if random.random() < 0.5
-                    else get_random_word(self.vocab_words)
-                )
-            tokens[index] = masked_token
-
-        tokens_ids = self.tokenizer.convert_tokens_to_ids(tokens)
-        segment_ids = [0] + [0] * len(tokens_a) + [0] + [1] * len(tokens_b) + [1]
-        tokens_mask = [1] * len(tokens_ids)
-
-        padding = [0] * (max_seq_length - len(tokens_ids))
-        tokens_ids += padding
-        tokens_mask += padding
-        segment_ids += len(padding) * [1]
-
-        assert len(tokens_ids) == max_seq_length
-        assert len(tokens_mask) == max_seq_length
-        assert len(segment_ids) == max_seq_length
-        return dict(
-            {
-                "tokens_ids": torch.tensor(tokens_ids, dtype=torch.long),
-                "seg_ids": torch.tensor(segment_ids, dtype=torch.long),
-                "attn_mask": torch.tensor(tokens_mask, dtype=torch.long),
-                "pos_ids": torch.tensor(list(range(max_seq_length)), dtype=torch.long),
-                "nsp_label": torch.tensor(int(nsp_label), dtype=torch.long),
-                "mlm_label": torch.tensor(label, dtype=torch.long),
-                "mlm_label_mask": torch.tensor(label_mask, dtype=torch.long),
-            }
+
+
+class HfImageClassificationProcessor:
+    """
+    Processor for image classification tasks.
+    """
+
+    def __init__(
+        self,
+        vision_processor: BaseImageProcessor,
+    ):
+        """
+        Initialize the HfImageClassificationProcessor.
+
+        Args:
+            vision_processor (BaseImageProcessor): The vision processor object used for image transformations.
+        """
+        self.vision_processor = vision_processor
+
+        self.size = getattr(self.vision_processor, "size", None)
+
+        self.resample = getattr(self.vision_processor, "resample", None)
+
+        self.crop_size = getattr(self.vision_processor, "crop_size", None)
+
+        self.rescale_factor = getattr(self.vision_processor, "rescale_factor", None)
+
+        self.image_mean = getattr(self.vision_processor, "image_mean", None)
+        self.image_std = getattr(self.vision_processor, "image_std", None)
+
+    def classification(
+        self,
+        image: Image.Image,
+    ):
+        """
+        Perform image classification on the given image.
+
+        Args:
+            image (Image.Image): The input image.
+
+        Returns:
+            GenericOutputs: The output of the image classification, including pixel values.
+        """
+        if self.size is not None:
+            image = self.vision_processor.resize(
+                image=to_numpy_array(image.convert("RGB")),
+                size=self.size,
+                resample=self.resample,
+            )
+
+        if self.crop_size is not None:
+            image = self.vision_processor.center_crop(
+                image,
+                size=self.crop_size,
+            )
+
+        if self.rescale_factor is not None:
+            image = self.vision_processor.rescale(
+                image,
+                scale=self.rescale_factor,
+            )
+
+        if self.image_mean is not None and self.image_std is not None:
+            image = self.vision_processor.normalize(
+                image=image,
+                mean=self.image_mean,
+                std=self.image_std,
+            )
+
+        image = to_channel_dimension_format(image, ChannelDimension.FIRST)
+
+        return GenericOutputs(
+            pixel_values=torch.tensor(image),
         )
```

### Comparing `unitorch-0.0.0.1/unitorch/process/bart.py` & `unitorch-0.0.0.2/src/unitorch/models/llama/processing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,201 +1,257 @@
+# Copyright (c) FULIUCANSHENG.
+# Licensed under the MIT License.
+
 import os
+import random
 from functools import partial
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
+import numpy as np
 import torch
-from transformers import BartTokenizer
 
-from unitorch.functions import pop_first_non_none_value
-from unitorch.utils.decorators import (
-    add_default_section_for_init,
-    add_key_group_info_for_process,
-    add_group_prefix_suffix_for_key,
+from transformers import LlamaTokenizer
+from unitorch.utils import pop_value, truncate_sequence_pair
+from unitorch.models import (
+    HfTextClassificationProcessor,
+    HfTextGenerationProcessor,
+    GenericOutputs,
 )
-from unitorch import register_process
-from unitorch.core import core_class
-from unitorch.utils.hf import hf_cached_path
-from unitorch.generation.bart import CORE_BART_PRETRAINED_DICT, VOCABS_KEY, MERGES_KEY
 
 
-def get_bart_tokenizer(vocab_path, merge_path):
-    assert os.path.exists(vocab_path) and os.path.exists(merge_path)
-    tokenizer = BartTokenizer(vocab_path, merge_path)
-    return tokenizer
+class LlamaProcessor(HfTextClassificationProcessor, HfTextGenerationProcessor):
+    def __init__(
+        self,
+        vocab_file: str,
+        max_seq_length: Optional[int] = 128,
+        max_gen_seq_length: Optional[int] = 48,
+    ):
+        """
+        Initialize the LlamaProcessor.
+
+        Args:
+            vocab_file (str): Path to the vocabulary file.
+            max_seq_length (int, optional): Maximum sequence length for text classification. Defaults to 128.
+            max_gen_seq_length (int, optional): Maximum sequence length for text generation. Defaults to 48.
+        """
+        tokenizer = LlamaTokenizer(vocab_file=vocab_file)
+        tokenizer.cls_token = tokenizer.bos_token
+        tokenizer.sep_token = tokenizer.eos_token
+        tokenizer.pad_token = tokenizer.unk_token
+        tokenizer.cls_token_id = tokenizer.bos_token_id
+        tokenizer.sep_token_id = tokenizer.eos_token_id
+        tokenizer.pad_token_id = tokenizer.unk_token_id
+        HfTextClassificationProcessor.__init__(
+            self,
+            tokenizer=tokenizer,
+            max_seq_length=max_seq_length,
+        )
+        HfTextGenerationProcessor.__init__(
+            self,
+            tokenizer=tokenizer,
+            max_seq_length=max_seq_length,
+            max_gen_seq_length=max_gen_seq_length,
+        )
 
+    def classification(
+        self,
+        text: str,
+        text_pair: Optional[str] = None,
+        max_seq_length: Optional[int] = None,
+    ):
+        """
+        Process text for classification.
 
-class Bart(core_class):
-    def __init__(
+        Args:
+            text (str): Input text.
+            text_pair (str, optional): Input text pair. Defaults to None.
+            max_seq_length (int, optional): Maximum sequence length. Defaults to None.
+
+        Returns:
+            GenericOutputs: Processed input_ids and attention_mask tensors.
+        """
+        max_seq_length = pop_value(
+            max_seq_length,
+            self.max_seq_length,
+        )
+
+        tokens = self.tokenizer.tokenize(str(text))
+        if text_pair is None:
+            tokens = tokens[:max_seq_length]
+            input_ids = self.tokenizer.convert_tokens_to_ids(tokens)
+        else:
+            tokens_pair = self.tokenizer.tokenize(str(text_pair))
+            truncate_sequence_pair(tokens, tokens_pair, max_seq_length)
+            tokens = tokens + tokens_pair
+            input_ids = self.tokenizer.convert_tokens_to_ids(tokens)
+
+        padding = [0] * (max_seq_length - len(input_ids))
+        attention_mask = [0] * len(padding) + [1] * len(input_ids)
+        input_ids = len(padding) * [self.pad_token_id] + input_ids
+
+        assert len(input_ids) == max_seq_length
+        assert len(attention_mask) == max_seq_length
+        return GenericOutputs(
+            input_ids=torch.tensor(input_ids, dtype=torch.long),
+            attention_mask=torch.tensor(attention_mask, dtype=torch.long),
+        )
+
+    def prompt(
         self,
-        vocab_path=None,
-        merge_path=None,
-        max_seq_length=128,
-        max_gen_seq_length=48,
-    ):
-        self.tokenizer = get_bart_tokenizer(
-            vocab_path,
-            merge_path,
-        )
-        self.max_seq_length = max_seq_length
-        self.max_gen_seq_length = max_gen_seq_length
-
-    @classmethod
-    @add_default_section_for_init("core/process/bart")
-    def init_from_core_configure(cls, cfg, **kwargs):
-        pretrained_name = cfg.getdefault(
-            "core/process/bart", "pretrained_name", "default-bart"
-        )
-        vocab_name_or_path = cfg.getdefault(
-            "core/process/bart", "vocab_name_or_path", pretrained_name
-        )
-        vocab_path = (
-            CORE_BART_PRETRAINED_DICT[vocab_name_or_path][VOCABS_KEY]
-            if vocab_name_or_path in CORE_BART_PRETRAINED_DICT
-            else vocab_name_or_path
-        )
-        vocab_path = hf_cached_path(vocab_path)
-
-        merge_name_or_path = cfg.getdefault(
-            "core/process/bart", "merge_name_or_path", pretrained_name
-        )
-        merge_path = (
-            CORE_BART_PRETRAINED_DICT[merge_name_or_path][MERGES_KEY]
-            if merge_name_or_path in CORE_BART_PRETRAINED_DICT
-            else merge_name_or_path
-        )
-
-        merge_path = hf_cached_path(merge_path)
-        return dict(
-            {
-                "vocab_path": vocab_path,
-                "merge_path": merge_path,
-            }
-        )
-
-    @add_key_group_info_for_process(
-        group_info=dict(
-            name="core/process/bart_for_generation",
-            net_inputs=[
-                "tokens_ids_a",
-                "tokens_mask_a",
-                "tokens_ids_b",
-                "tokens_mask_b",
-            ],
-            net_targets=["next_tokens_ids", "next_tokens_mask"],
-        )
-    )
-    @register_process("core/process/bart_for_generation")
-    def for_generation(
-        self, text_a, text_b=None, max_seq_length=None, max_gen_seq_length=None
-    ):
-        max_seq_length = pop_first_non_none_value(max_seq_length, self.max_seq_length)
-        max_gen_seq_length = pop_first_non_none_value(
-            max_gen_seq_length, self.max_gen_seq_length
-        )
-        tokens_a = self.tokenizer.tokenize(text_a)
-        tokens_a = ["<s>"] + tokens_a[: max_seq_length - 2] + ["</s>"]
-        tokens_ids_a = self.tokenizer.convert_tokens_to_ids(tokens_a)
-
-        tokens_mask_a = [1] * len(tokens_ids_a)
-        padding_a = [0] * (max_seq_length - len(tokens_ids_a))
-        tokens_ids_a += [1] * len(padding_a)
-        tokens_mask_a += padding_a
-
-        assert len(tokens_ids_a) == max_seq_length
-        if text_b is None:
-            return dict(
-                {
-                    "tokens_ids_a": torch.tensor(tokens_ids_a, dtype=torch.long),
-                    "tokens_mask_a": torch.tensor(tokens_mask_a, dtype=torch.long),
-                }
-            )
-
-        tokens_b = self.tokenizer.tokenize(text_b)
-        tokens_b = ["</s>"] + tokens_b[: max_gen_seq_length - 2] + ["</s>"]
-        tokens_ids_b = self.tokenizer.convert_tokens_to_ids(tokens_b)
-        tokens_b_len = len(tokens_ids_b)
-
-        _tokens_ids_b = tokens_ids_b[: tokens_b_len - 1]
-        _next_tokens_ids_b = tokens_ids_b[1:tokens_b_len]
-        _next_tokens_mask_b = [1] * len(_tokens_ids_b)
-
-        padding_b = [0] * (max_gen_seq_length - len(_tokens_ids_b))
-        _tokens_ids_b += [1] * len(padding_b)
-        _tokens_mask_b = [1] * (tokens_b_len - 1) + padding_b
-        _next_tokens_ids_b += [1] * len(padding_b)
-        _next_tokens_mask_b += padding_b
-        assert len(_tokens_ids_b) == max_gen_seq_length
-        assert len(_next_tokens_ids_b) == max_gen_seq_length
-        assert len(_next_tokens_mask_b) == max_gen_seq_length
-
-        return dict(
-            {
-                "tokens_ids_a": torch.tensor(tokens_ids_a, dtype=torch.long),
-                "tokens_mask_a": torch.tensor(tokens_mask_a, dtype=torch.long),
-                "tokens_ids_b": torch.tensor(_tokens_ids_b, dtype=torch.long),
-                "tokens_mask_b": torch.tensor(_tokens_mask_b, dtype=torch.long),
-                "next_tokens_ids": torch.tensor(_next_tokens_ids_b, dtype=torch.long),
-                "next_tokens_mask": torch.tensor(_next_tokens_mask_b, dtype=torch.long),
-            }
-        )
-
-    @register_process("core/process/bart_for_tokens")
-    @add_group_prefix_suffix_for_key
-    def for_tokens(self, text, max_seq_length=None, group_for_key="net_inputs"):
-        max_seq_length = pop_first_non_none_value(max_seq_length, self.max_seq_length)
-        tokens = self.tokenizer.tokenize(text)
-        tokens = tokens[: max_seq_length - 2]
-        tokens = ["</s>"] + tokens + ["</s>"]
-        tokens_ids = self.tokenizer.convert_tokens_to_ids(tokens)
-        tokens_ids = tokens_ids[: max_seq_length - 1]
-        tokens_mask = [1] * len(tokens_ids)
-
-        padding = [0] * (max_seq_length - len(tokens_ids))
-        tokens_ids += padding
-        tokens_mask += padding
-
-        assert len(tokens_ids) == max_seq_length
-        assert len(tokens_mask) == max_seq_length
-        return dict(
-            {
-                "tokens_ids": torch.tensor(tokens_ids, dtype=torch.long),
-                "tokens_mask": torch.tensor(tokens_mask, dtype=torch.long),
-            }
-        )
-
-    @register_process("core/process/bart_for_next_tokens")
-    @add_group_prefix_suffix_for_key
-    def for_next_tokens(
-        self, text, max_gen_seq_length=None, group_for_key="net_targets"
-    ):
-        max_gen_seq_length = pop_first_non_none_value(
-            max_gen_seq_length, self.max_gen_seq_length
-        )
-        tokens = self.tokenizer.tokenize(text)
-        tokens = tokens[: max_gen_seq_length - 2]
-        tokens = ["</s>"] + tokens + ["</s>"]
-        tokens_ids = self.tokenizer.convert_tokens_to_ids(tokens)
-        tokens_ids = tokens_ids[1:max_gen_seq_length]
-        tokens_mask = [1] * len(tokens_ids)
-
-        padding = [0] * (max_gen_seq_length - len(tokens_ids))
-        tokens_ids += padding
-        tokens_mask += padding
-
-        assert len(tokens_ids) == max_gen_seq_length
-        assert len(tokens_mask) == max_gen_seq_length
-        return dict(
-            {
-                "next_tokens_ids": torch.tensor(tokens_ids, dtype=torch.long),
-                "next_tokens_mask": torch.tensor(tokens_mask, dtype=torch.long),
-            }
-        )
-
-    @register_process("core/process/bart_for_decode")
-    def for_decode(self, tensor, key="hyp"):
-        batch_size, num_return_sequences, seq_len = tensor.size()
-        tensor = tensor.reshape(-1, seq_len)
-        hyp = self.tokenizer.batch_decode(tensor)
-        hyp = [
-            hyp[i : i + num_return_sequences]
-            for i in range(0, len(hyp), num_return_sequences)
+        text: str,
+        max_seq_length: Optional[int] = None,
+    ):
+        """
+        Process text as a prompt.
+
+        Args:
+            text (str): Input text.
+            max_seq_length (int, optional): Maximum sequence length. Defaults to None.
+
+        Returns:
+            GenericOutputs: Processed input_ids tensor.
+        """
+        max_seq_length = pop_value(
+            max_seq_length,
+            self.max_seq_length,
+        )
+        tokens = [self.bos_token] + self.tokenizer.tokenize(str(text))[
+            1 - max_seq_length :
         ]
-        return dict({key: hyp})
+        padding = [self.pad_token] * (max_seq_length - len(tokens))
+        tokens = padding + tokens
+        input_ids = self.tokenizer.convert_tokens_to_ids(tokens)
+
+        assert len(input_ids) == max_seq_length
+        return GenericOutputs(
+            input_ids=torch.tensor(input_ids, dtype=torch.long),
+        )
+
+    def generation_inputs(
+        self,
+        text: str,
+        max_seq_length: Optional[int] = None,
+    ):
+        """
+        Process text for generation inputs.
+
+        Args:
+            text (str): Input text.
+            max_seq_length (int, optional): Maximum sequence length. Defaults to None.
+
+        Returns:
+            GenericOutputs: Processed input_ids tensor.
+        """
+        max_seq_length = pop_value(
+            max_seq_length,
+            self.max_seq_length,
+        )
+        tokens = [self.bos_token] + self.tokenizer.tokenize(str(text))[
+            1 - max_seq_length :
+        ]
+        padding = [self.pad_token] * (max_seq_length - len(tokens))
+        tokens = padding + tokens
+        input_ids = self.tokenizer.convert_tokens_to_ids(tokens)
+
+        assert len(input_ids) == max_seq_length
+        return GenericOutputs(
+            input_ids=torch.tensor(input_ids, dtype=torch.long),
+        )
+
+    def generation_labels(
+        self,
+        text: str,
+        max_gen_seq_length: Optional[int] = None,
+    ):
+        """
+        Process text for generation labels.
+
+        Args:
+            text (str): Input text.
+            max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to None.
+
+        Returns:
+            GenericOutputs: Processed input_ids and attention_mask tensors.
+        """
+        max_gen_seq_length = pop_value(
+            max_gen_seq_length,
+            self.max_gen_seq_length,
+        )
+        tokens = self.tokenizer.tokenize(str(text))[: max_gen_seq_length - 1] + [
+            self.eos_token
+        ]
+        padding = [self.pad_token] * (max_gen_seq_length - len(tokens))
+        input_ids = self.tokenizer.convert_tokens_to_ids(tokens)
+        attention_mask = [1] * len(input_ids)
+
+        padding = [0] * (max_gen_seq_length - len(input_ids))
+        input_ids += [self.pad_token_id] * len(padding)
+        attention_mask += padding
+
+        assert len(input_ids) == max_gen_seq_length
+        assert len(attention_mask) == max_gen_seq_length
+        return GenericOutputs(
+            input_ids=torch.tensor(input_ids, dtype=torch.long),
+            attention_mask=torch.tensor(attention_mask, dtype=torch.long),
+        )
+
+    def generation(
+        self,
+        text: str,
+        text_pair: str,
+        max_seq_length: Optional[int] = None,
+        max_gen_seq_length: Optional[int] = None,
+    ):
+        """
+        Process text for generation.
+
+        Args:
+            text (str): Input text.
+            text_pair (str): Input text pair.
+            max_seq_length (int, optional): Maximum sequence length. Defaults to None.
+            max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to None.
+
+        Returns:
+            GenericOutputs: Processed input_ids, attention_mask, input_ids_label, and attention_mask_label tensors.
+        """
+        max_seq_length = pop_value(
+            max_seq_length,
+            self.max_seq_length,
+        )
+        max_gen_seq_length = pop_value(
+            max_gen_seq_length,
+            self.max_gen_seq_length,
+        )
+        max_seq_length = max_seq_length + max_gen_seq_length
+
+        tokens = [self.bos_token] + self.tokenizer.tokenize(str(text))[
+            1 - max_seq_length :
+        ]
+        tokens_pair = self.tokenizer.tokenize(str(text_pair))[
+            : max_gen_seq_length - 1
+        ] + [self.eos_token]
+        padding_a = [self.pad_token] * (max_seq_length - len(tokens))
+        padding_b = [self.pad_token] * (max_gen_seq_length - len(tokens_pair))
+        attention_mask = (
+            [0] * len(padding_a)
+            + [1] * (len(tokens) + len(tokens_pair))
+            + [0] * len(padding_b)
+        )
+        _tokens = padding_a + tokens + tokens_pair + padding_b
+        input_ids = self.tokenizer.convert_tokens_to_ids(_tokens)
+
+        tokens_label = tokens_pair[1:max_gen_seq_length] + [self.pad_token] * (
+            max_gen_seq_length - len(tokens_pair) + 1
+        )
+        input_ids_label = self.tokenizer.convert_tokens_to_ids(tokens_label)
+        input_ids_label = [0] * max_seq_length + input_ids_label
+        attention_mask_label = [1] * len(tokens_pair[1:max_gen_seq_length]) + [0] * (
+            max_gen_seq_length - len(tokens_pair) + 1
+        )
+        attention_mask_label = [0] * max_seq_length + attention_mask_label
+
+        return GenericOutputs(
+            input_ids=torch.tensor(input_ids, dtype=torch.long),
+            attention_mask=torch.tensor(attention_mask, dtype=torch.long),
+            input_ids_label=torch.tensor(input_ids_label, dtype=torch.long),
+            attention_mask_label=torch.tensor(attention_mask_label, dtype=torch.long),
+        )
```

### Comparing `unitorch-0.0.0.1/unitorch/process/mass.py` & `unitorch-0.0.0.2/src/unitorch/cli/models/mt5/processing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,175 +1,177 @@
-import os
-import random
-from functools import partial
-
-import numpy as np
-import torch
-
-from unitorch.functions import pop_first_non_none_value
-from unitorch.utils.decorators import (
-    add_key_group_info_for_process,
-    add_group_prefix_suffix_for_key,
+# Copyright (c) FULIUCANSHENG.
+# Licensed under the MIT License.
+
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
+
+from unitorch.utils import pop_value, nested_dict_value
+from unitorch.models.mt5 import MT5Processor as _MT5Processor
+from unitorch.cli import (
+    cached_path,
     add_default_section_for_init,
+    add_default_section_for_function,
+    register_process,
+)
+from unitorch.cli import WriterOutputs
+from unitorch.cli.models import (
+    TensorsInputs,
+    GenerationOutputs,
+    GenerationTargets,
 )
-from unitorch.process.bert import _truncate_seq_pair, get_bert_tokenizer
-from unitorch import register_process
-from unitorch.core import core_class
-from unitorch.utils.hf import hf_cached_path
-from unitorch.generation.mass import CORE_MASS_PRETRAINED_DICT, VOCABS_KEY
+from unitorch.cli.models.mt5 import pretrained_mt5_infos
 
 
-class Mass(core_class):
+class MT5Processor(_MT5Processor):
+    """Processor for MT5 models."""
+
     def __init__(
         self,
-        vocab_path,
-        max_seq_length=128,
-        max_gen_seq_length=30,
-        never_split_tokens=[],
-        do_lower_case=True,
+        vocab_path: str,
+        special_input_ids: Optional[Dict] = dict(),
+        max_seq_length: Optional[int] = 128,
+        max_gen_seq_length: Optional[int] = 48,
     ):
-        self.max_seq_length = max_seq_length
-        self.max_gen_seq_length = max_gen_seq_length
-        tokenizer_and_special_token_map = get_bert_tokenizer(
-            vocab_path, never_split_tokens, do_lower_case
-        )
-        self.tokenizer = tokenizer_and_special_token_map.get("tokenizer")
-        self.special_tokens_map = tokenizer_and_special_token_map.get(
-            "special_tokens_map"
+        """
+        Initialize the MT5Processor.
+
+        Args:
+            vocab_path (str): The path to the vocabulary file.
+            special_input_ids (Dict, optional): Special input IDs. Defaults to an empty dictionary.
+            max_seq_length (int, optional): The maximum sequence length. Defaults to 128.
+            max_gen_seq_length (int, optional): The maximum generation sequence length. Defaults to 48.
+        """
+        super().__init__(
+            vocab_path=vocab_path,
+            special_input_ids=special_input_ids,
+            max_seq_length=max_seq_length,
+            max_gen_seq_length=max_gen_seq_length,
         )
 
     @classmethod
-    @add_default_section_for_init("core/process/mass")
-    def init_from_core_configure(cls, cfg, **kwargs):
-        never_split_tokens = cfg.getdefault(
-            "core/process/mass", "never_split_tokens", None
-        )
-        if never_split_tokens is not None:
-            never_split_tokens = eval(never_split_tokens)
-        else:
-            never_split_tokens = []
-
-        pretrained_name = cfg.getdefault(
-            "core/process/mass", "pretrained_name", "default-mass"
-        )
-        vocab_name_or_path = cfg.getdefault(
-            "core/process/mass", "vocab_name_or_path", pretrained_name
-        )
-        vocab_path = (
-            CORE_MASS_PRETRAINED_DICT[vocab_name_or_path][VOCABS_KEY]
-            if vocab_name_or_path in CORE_MASS_PRETRAINED_DICT
-            else vocab_name_or_path
-        )
-
-        vocab_path = hf_cached_path(vocab_path)
-
-        return dict(
-            {
-                "vocab_path": vocab_path,
-                "never_split_tokens": never_split_tokens,
-            }
-        )
-
-    @add_key_group_info_for_process(
-        group_info=dict(
-            name="core/process/mass_for_generation",
-            net_inputs=["tokens_ids_a", "tokens_ids_b"],
-            net_targets=["next_tokens_ids", "next_tokens_mask"],
-        )
-    )
-    @register_process("core/process/mass_for_generation")
-    def for_generation(
-        self, text_a, text_b, max_seq_length=None, max_gen_seq_length=None
+    @add_default_section_for_init("core/process/mt5")
+    def from_core_configure(cls, config, **kwargs):
+        """
+        Create an instance of MT5Processor from a core configuration.
+
+        Args:
+            config: The core configuration.
+            **kwargs: Additional keyword arguments.
+
+        Returns:
+            dict: A dictionary containing the arguments for initializing the MT5Processor.
+        """
+        config.set_default_section("core/process/mt5")
+        pretrained_name = config.getoption("pretrained_name", "default-mt5")
+        vocab_path = config.getoption("vocab_path", None)
+        vocab_path = pop_value(
+            vocab_path,
+            nested_dict_value(pretrained_mt5_infos, pretrained_name, "vocab"),
+        )
+        vocab_path = cached_path(vocab_path)
+
+        return {
+            "vocab_path": vocab_path,
+        }
+
+    @register_process("core/process/mt5/generation/inputs")
+    def _generation_inputs(
+        self,
+        text: str,
+        max_seq_length: Optional[int] = None,
     ):
-        max_seq_length = int(
-            pop_first_non_none_value(max_seq_length, self.max_seq_length)
+        """
+        Preprocess the input text for generation tasks.
+
+        Args:
+            text (str): The input text.
+            max_seq_length (int, optional): The maximum sequence length. Defaults to None.
+
+        Returns:
+            TensorsInputs: The processed input tensors.
+        """
+        outputs = super().generation_inputs(
+            text=text,
+            max_seq_length=max_seq_length,
         )
-        max_gen_seq_length = pop_first_non_none_value(
-            max_gen_seq_length, self.max_gen_seq_length
+        return TensorsInputs(input_ids=outputs.input_ids)
+
+    @register_process("core/process/mt5/generation/labels")
+    def _generation_labels(
+        self,
+        text: str,
+        max_gen_seq_length: Optional[int] = None,
+    ):
+        """
+        Preprocess the target text for generation tasks.
+
+        Args:
+            text (str): The target text.
+            max_gen_seq_length (int, optional): The maximum generation sequence length. Defaults to None.
+
+        Returns:
+            GenerationTargets: The processed generation targets.
+        """
+        outputs = super().generation_labels(
+            text=text,
+            max_gen_seq_length=max_gen_seq_length,
+        )
+        return GenerationTargets(
+            refs=outputs.input_ids,
+            masks=outputs.attention_mask,
+        )
+
+    @register_process("core/process/mt5/generation")
+    def _generation(
+        self,
+        text: str,
+        text_pair: Optional[str] = None,
+        max_seq_length: Optional[int] = None,
+        max_gen_seq_length: Optional[int] = None,
+    ):
+        """
+        Preprocess the input and target texts for generation tasks.
+
+        Args:
+            text (str): The input text.
+            text_pair (str, optional): The paired input text. Defaults to None.
+            max_seq_length (int, optional): The maximum sequence length. Defaults to None.
+            max_gen_seq_length (int, optional): The maximum generation sequence length. Defaults to None.
+
+        Returns:
+            Tuple[TensorsInputs, GenerationTargets]: The processed input tensors and generation targets.
+        """
+        outputs = super().generation(
+            text=text,
+            text_pair=text_pair,
+            max_seq_length=max_seq_length,
+            max_gen_seq_length=max_gen_seq_length,
+        )
+        return TensorsInputs(
+            input_ids=outputs.input_ids,
+            attention_mask=outputs.attention_mask,
+            decoder_input_ids=outputs.input_ids_pair,
+            decoder_attention_mask=outputs.attention_mask_pair,
+        ), GenerationTargets(
+            refs=outputs.input_ids_label,
+            masks=outputs.attention_mask_label,
         )
 
-        tokens_a = self.tokenizer.tokenize(text_a)
-        tokens_a = ["[CLS]"] + tokens_a[: max_seq_length - 2] + ["[SEP]"]
-        tokens_ids_a = self.tokenizer.convert_tokens_to_ids(tokens_a)
-
-        padding_a = [0] * (max_seq_length - len(tokens_ids_a))
-        tokens_ids_a += padding_a
-
-        assert len(tokens_ids_a) == max_seq_length
-
-        tokens_b = self.tokenizer.tokenize(text_b)
-        tokens_b = ["[CLS]"] + tokens_b[: max_gen_seq_length - 2] + ["[SEP]"]
-        tokens_ids_b = self.tokenizer.convert_tokens_to_ids(tokens_b)
-        tokens_b_len = len(tokens_ids_b)
-
-        _tokens_ids_b = tokens_ids_b[: tokens_b_len - 1]
-        _next_tokens_ids_b = tokens_ids_b[1:tokens_b_len]
-        _next_tokens_mask_b = [1] * len(_tokens_ids_b)
-
-        padding_b = [0] * (max_gen_seq_length - len(_tokens_ids_b))
-        _tokens_ids_b += padding_b
-        _next_tokens_ids_b += padding_b
-        _next_tokens_mask_b += padding_b
-        assert len(_tokens_ids_b) == max_gen_seq_length
-        assert len(_next_tokens_ids_b) == max_gen_seq_length
-        assert len(_next_tokens_mask_b) == max_gen_seq_length
-
-        return dict(
-            {
-                "tokens_ids_a": torch.tensor(tokens_ids_a, dtype=torch.long),
-                "tokens_ids_b": torch.tensor(_tokens_ids_b, dtype=torch.long),
-                "next_tokens_ids": torch.tensor(_next_tokens_ids_b, dtype=torch.long),
-                "next_tokens_mask": torch.tensor(_next_tokens_mask_b, dtype=torch.long),
-            }
-        )
-
-    @register_process("core/process/mass_for_tokens")
-    @add_group_prefix_suffix_for_key
-    def for_tokens(self, text, max_seq_length=None, group_for_key="net_inputs"):
-        max_seq_length = pop_first_non_none_value(max_seq_length, self.max_seq_length)
-        tokens = self.tokenizer.tokenize(text)
-        tokens = tokens[: max_seq_length - 2]
-        tokens = ["[CLS]"] + tokens + ["[SEP]"]
-        tokens_ids = self.tokenizer.convert_tokens_to_ids(tokens)
-        tokens_ids = tokens_ids[: max_seq_length - 1]
-
-        padding = [0] * (max_seq_length - len(tokens_ids))
-        tokens_ids += padding
-
-        assert len(tokens_ids) == max_seq_length
-        return dict({"tokens_ids": torch.tensor(tokens_ids, dtype=torch.long)})
-
-    @register_process("core/process/mass_for_next_tokens")
-    @add_group_prefix_suffix_for_key
-    def for_next_tokens(self, text, max_seq_length=None, group_for_key="net_targets"):
-        max_seq_length = pop_first_non_none_value(
-            max_seq_length, self.max_gen_seq_length
-        )
-        tokens = self.tokenizer.tokenize(text)
-        tokens = tokens[: max_seq_length - 2]
-        tokens = ["[CLS]"] + tokens + ["[SEP]"]
-        tokens_ids = self.tokenizer.convert_tokens_to_ids(tokens)
-        tokens_ids = tokens_ids[1:max_seq_length]
-        tokens_mask = [1] * len(tokens_ids)
-
-        padding = [0] * (max_seq_length - len(tokens_ids))
-        tokens_ids += padding
-        tokens_mask += padding
-
-        assert len(tokens_ids) == max_seq_length
-        return dict(
-            {
-                "next_tokens_ids": torch.tensor(tokens_ids, dtype=torch.long),
-                "next_tokens_mask": torch.tensor(tokens_mask, dtype=torch.long),
-            }
-        )
-
-    @register_process("core/process/mass_for_decode")
-    def for_decode(self, tensor, key="hyp"):
-        batch_size, num_return_sequences, seq_len = tensor.size()
-        tensor = tensor.reshape(-1, seq_len)
-        hyp = self.tokenizer.batch_decode(tensor, skip_special_tokens=True)
-        hyp = [
-            hyp[i : i + num_return_sequences]
-            for i in range(0, len(hyp), num_return_sequences)
-        ]
-        return dict({key: hyp})
+    @register_process("core/postprocess/mt5/detokenize")
+    def _detokenize(
+        self,
+        outputs: GenerationOutputs,
+    ):
+        """
+        Detokenize the generated sequences.
+
+        Args:
+            outputs (GenerationOutputs): The generation outputs.
+
+        Returns:
+            WriterOutputs: The detokenized writer outputs.
+        """
+        results = outputs.to_pandas()
+        assert results.shape[0] == 0 or results.shape[0] == outputs.sequences.shape[0]
+
+        decoded = super().detokenize(sequences=outputs.sequences)
+        results["decoded"] = decoded
+        return WriterOutputs(results)
```

### Comparing `unitorch-0.0.0.1/config/core/bart_for_generation.ini` & `unitorch-0.0.0.2/examples/configs/generation/mbart.ini`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,65 @@
-[core/auto]
-task_type = core/auto/supervised_task
+[core/cli]
+task_name = core/task/supervised
+from_ckpt_dir = ./cache
 cache_dir = ./cache
+train_file = ./train.tsv
+dev_file = ./dev.tsv
+test_file = ./test.tsv
 
 # model
-[core/model/bart]
-pretrained_name = bart-base
+[core/model/generation/mbart]
+pretrained_name = mbart-large-cc25
+freeze_input_embedding = True
 no_repeat_ngram_size = 3
+max_gen_seq_length = 15
 
 # dataset
-[core/dataset]
-# data columns: id, num, query, doc, label, score
-data_name = fuliucansheng/data_for_test
-
-[core/dataset/train]
-preprocess_funcs = ['core/process/bart_for_generation(query, doc)']
-
-[core/dataset/dev]
-preprocess_funcs = ['core/process/bart_for_tokens(query)', 'core/process/bart_for_next_tokens(doc)']
+[core/dataset/ast]
+names = ['encode', 'decode']
 
-[core/dataset/test]
-preprocess_funcs = ['core/process/bart_for_tokens(query)']
+[core/dataset/ast/train]
+data_files = ${core/cli:train_file}
+preprocess_functions = ['core/process/mbart/generation(encode, decode)']
+
+[core/dataset/ast/dev]
+data_files = ${core/cli:dev_file}
+preprocess_functions = ['core/process/mbart/generation/inputs(encode)', 'core/process/mbart/generation/labels(decode)']
+
+[core/dataset/ast/test]
+names = ['encode']
+data_files = ${core/cli:test_file}
+preprocess_functions = ['core/process/mbart/generation/inputs(encode)']
 
 # process
-[core/process/bart]
-pretrained_name = bart-base
+[core/process/mbart]
+pretrained_name = mbart-large-cc25
 max_seq_length = 24
 max_gen_seq_length = 15
 
+# optim
+[core/optim/adamw]
+learning_rate = 0.0001
+
+# scheduler
+[core/scheduler/linear_warmup]
+num_warmup_rate = 0.001
+
 # task
-[core/auto/supervised_task]
-model = core/model/bart_for_generation
-optim = core/optim/adam
-dataset = core/dataset/auto
+[core/task/supervised]
+model = core/model/generation/mbart
+optim = core/optim/adamw
+scheduler = core/scheduler/linear_warmup
+dataset = core/dataset/ast
 loss_fn = core/loss/lm
 score_fn = core/score/bleu
 monitor_fns = ['core/score/bleu', 'core/score/rouge1', 'core/score/rouge2', 'core/score/rougel']
-output_header = query,doc
-post_process_fn = partial(core/process/bart_for_decode)
-
-opt_fp16 = O1
-from_ckpt_dir = ${core/auto:cache_dir}
-to_ckpt_dir = ${core/auto:cache_dir}
-output_path = ${core/auto:cache_dir}/output.txt
-train_batch_size = 64
-dev_batch_size = 64
-test_batch_size = 256
+output_header = ['encode']
+postprocess_fn = core/postprocess/mbart/detokenize
+writer = core/writer/csv
+
+from_ckpt_dir = ${core/cli:from_ckpt_dir}
+to_ckpt_dir = ${core/cli:cache_dir}
+output_path = ${core/cli:cache_dir}/output.txt
+train_batch_size = 4
+dev_batch_size = 8
+test_batch_size = 8
```

### Comparing `unitorch-0.0.0.1/config/core/mass_for_generation.ini` & `unitorch-0.0.0.2/examples/configs/caption/blip.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,73 @@
-[core/auto]
-task_type = core/auto/supervised_task
+[core/cli]
+task_name = core/task/supervised
+from_ckpt_dir = ./cache
 cache_dir = ./cache
+train_file = ./train.tsv
+dev_file = ./dev.tsv
+test_file = ./test.tsv
 
 # model
-[core/model/mass]
-pretrained_name = mass-base-uncased
-num_beams = 5
-no_repeat_ngram_size = 0
+[core/model/caption/blip]
+pretrained_name = blip-image-captioning-base
+no_repeat_ngram_size = 3
 max_gen_seq_length = 15
-repetition_penalty = 1.0
 
 # dataset
-[core/dataset]
-# data columns: id, num, query, doc, label, score
-data_name = fuliucansheng/data_for_test
+[core/dataset/ast]
+names = ['caption', 'image']
 
-[core/dataset/train]
-preprocess_funcs = ['core/process/mass_for_generation(query, doc)']
-
-[core/dataset/dev]
-preprocess_funcs = ['core/process/mass_for_tokens(query)', 'core/process/mass_for_next_tokens(doc)']
-
-[core/dataset/test]
-preprocess_funcs = ['core/process/mass_for_tokens(query)']
+[core/dataset/ast/train]
+data_files = ${core/cli:train_file}
+preprocess_functions = [
+    'core/process/blip/generation(caption, core/process/image/read(image))',
+  ]
+
+[core/dataset/ast/dev]
+data_files = ${core/cli:dev_file}
+preprocess_functions = [
+    'core/process/blip/image_classification(core/process/image/read(image))',
+    'core/process/blip/generation/labels(caption)',
+  ]
+
+[core/dataset/ast/test]
+names = ['image']
+data_files = ${core/cli:test_file}
+preprocess_functions = [
+    'core/process/blip/image_classification(core/process/image/read(image))'
+  ]
 
 # process
-[core/process/mass]
-pretrained_name = mass-base-uncased
-max_seq_length = 24
+[core/process/blip]
+pretrained_name = blip-image-captioning-base
 max_gen_seq_length = 15
 
+[core/process/image]
+http_url = http://0.0.0.0:11230/?image={0}
+
+# optim
+[core/optim/adamw]
+learning_rate = 0.0001
+
+# scheduler
+[core/scheduler/linear_warmup]
+num_warmup_rate = 0.001
+
 # task
-[core/auto/supervised_task]
-model = core/model/mass_for_generation
-optim = core/optim/adam
-dataset = core/dataset/auto
+[core/task/supervised]
+model = core/model/caption/blip
+optim = core/optim/adamw
+scheduler = core/scheduler/linear_warmup
+dataset = core/dataset/ast
 loss_fn = core/loss/lm
 score_fn = core/score/bleu
 monitor_fns = ['core/score/bleu', 'core/score/rouge1', 'core/score/rouge2', 'core/score/rougel']
-output_header = query,doc
-post_process_fn = partial(core/process/mass_for_decode)
-
-opt_fp16 = O1
-from_ckpt_dir = ${core/auto:cache_dir}
-to_ckpt_dir = ${core/auto:cache_dir}
-output_path = ${core/auto:cache_dir}/output.txt
-train_batch_size = 128
-dev_batch_size = 128
-test_batch_size = 256
+output_header = ['image']
+postprocess_fn = core/postprocess/blip/detokenize
+writer = core/writer/csv
+
+from_ckpt_dir = ${core/cli:from_ckpt_dir}
+to_ckpt_dir = ${core/cli:cache_dir}
+output_path = ${core/cli:cache_dir}/output.txt
+train_batch_size = 4
+dev_batch_size = 8
+test_batch_size = 8
```

### Comparing `unitorch-0.0.0.1/config/core/unilm_for_generation.ini` & `unitorch-0.0.0.2/examples/configs/generation/pegasus.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,64 @@
-[core/auto]
-task_type = core/auto/supervised_task
+[core/cli]
+task_name = core/task/supervised
+from_ckpt_dir = ./cache
 cache_dir = ./cache
+train_file = ./train.tsv
+dev_file = ./dev.tsv
+test_file = ./test.tsv
 
 # model
-[core/model/unilm]
-pretrained_name = unilm-base-uncased
-num_beams = 5
-no_repeat_ngram_size = 0
+[core/model/generation/pegasus]
+pretrained_name = pegasus-cnn_dailymail
+no_repeat_ngram_size = 3
 max_gen_seq_length = 15
-repetition_penalty = 1.0
 
 # dataset
-[core/dataset]
-# data columns: id, num, query, doc, label, score
-data_name = fuliucansheng/data_for_test
+[core/dataset/ast]
+names = ['encode', 'decode']
 
-[core/dataset/train]
-preprocess_funcs = ['core/process/unilm_for_faster_generation(query, doc)']
-
-[core/dataset/dev]
-preprocess_funcs = ['core/process/unilm_for_tokens(query)', 'core/process/unilm_for_next_tokens(doc)']
-
-[core/dataset/test]
-preprocess_funcs = ['core/process/unilm_for_tokens(query)']
+[core/dataset/ast/train]
+data_files = ${core/cli:train_file}
+preprocess_functions = ['core/process/pegasus/generation(encode, decode)']
+
+[core/dataset/ast/dev]
+data_files = ${core/cli:dev_file}
+preprocess_functions = ['core/process/pegasus/generation/inputs(encode)', 'core/process/pegasus/generation/labels(decode)']
+
+[core/dataset/ast/test]
+names = ['encode']
+data_files = ${core/cli:test_file}
+preprocess_functions = ['core/process/pegasus/generation/inputs(encode)']
 
 # process
-[core/process/unilm]
-pretrained_name = unilm-base-uncased
+[core/process/pegasus]
+pretrained_name = pegasus-cnn_dailymail
 max_seq_length = 24
 max_gen_seq_length = 15
 
+# optim
+[core/optim/adamw]
+learning_rate = 0.0001
+
+# scheduler
+[core/scheduler/linear_warmup]
+num_warmup_rate = 0.001
+
 # task
-[core/auto/supervised_task]
-model = core/model/unilm_for_generation
-optim = core/optim/adam
-dataset = core/dataset/auto
+[core/task/supervised]
+model = core/model/generation/pegasus
+optim = core/optim/adamw
+scheduler = core/scheduler/linear_warmup
+dataset = core/dataset/ast
 loss_fn = core/loss/lm
 score_fn = core/score/bleu
 monitor_fns = ['core/score/bleu', 'core/score/rouge1', 'core/score/rouge2', 'core/score/rougel']
-output_header = query,doc
-post_process_fn = partial(core/process/unilm_for_decode)
-
-opt_fp16 = O1
-from_ckpt_dir = ${core/auto:cache_dir}
-to_ckpt_dir = ${core/auto:cache_dir}
-output_path = ${core/auto:cache_dir}/output.txt
-train_batch_size = 64
-dev_batch_size = 64
-test_batch_size = 64
+output_header = ['encode']
+postprocess_fn = core/postprocess/pegasus/detokenize
+writer = core/writer/csv
+
+from_ckpt_dir = ${core/cli:from_ckpt_dir}
+to_ckpt_dir = ${core/cli:cache_dir}
+output_path = ${core/cli:cache_dir}/output.txt
+train_batch_size = 4
+dev_batch_size = 8
+test_batch_size = 8
```

### Comparing `unitorch-0.0.0.1/config/core/bert_for_classification.ini` & `unitorch-0.0.0.2/examples/configs/generation/bloom.ini`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,67 @@
-[core/auto]
-task_type = core/auto/supervised_task
+[core/cli]
+task_name = core/task/supervised
+from_ckpt_dir = ./cache
 cache_dir = ./cache
+train_file = ./train.tsv
+dev_file = ./dev.tsv
+test_file = ./test.tsv
 
 # model
-[core/model/bert]
-pretrained_name = bert-base-uncased
-num_class = 1
+[core/model/generation/bloom]
+pretrained_name = bloom-560m
+no_repeat_ngram_size = 3
+max_gen_seq_length = 15
 
 # dataset
-[core/dataset]
-# data columns: id, num, query, doc, label, score
-data_name = fuliucansheng/data_for_test
+[core/dataset/ast]
+names = ['encode', 'decode']
 
-[core/dataset/train]
-preprocess_funcs = ['core/process/bert_for_pair(query, doc, max_seq_length=32)', 'core/process/label_for_bce(label)']
-
-[core/dataset/dev]
-preprocess_funcs = ['core/process/bert_for_pair(query, doc, max_seq_length=32)', 'core/process/label_for_bce(label)']
-
-[core/dataset/test]
-preprocess_funcs = ['core/process/bert_for_pair(query, doc, max_seq_length=32)']
+[core/dataset/ast/train]
+data_files = ${core/cli:train_file}
+preprocess_functions = ['core/process/bloom/generation(encode, decode)']
+
+[core/dataset/ast/dev]
+data_files = ${core/cli:dev_file}
+preprocess_functions = ['core/process/bloom/generation/inputs(encode)', 'core/process/bloom/generation/labels(decode)']
+
+[core/dataset/ast/test]
+names = ['encode']
+data_files = ${core/cli:test_file}
+preprocess_functions = ['core/process/bloom/generation/inputs(encode)']
 
 # process
-[core/process/bert]
-pretrained_name = bert-base-uncased
-max_seq_length = 32
-
-
-[core/process/label]
-map_dict = {'Fair': 1, 'Good': 1, 'Bad': 0, 'Excellent': 1}
-num_class = 1
+[core/process/bloom]
+pretrained_name = bloom-560m
+max_seq_length = 5
+max_gen_seq_length = 15
+
+[core/writer/csv]
+escapechar = \
+
+# optim
+[core/optim/adamw]
+learning_rate = 0.0001
+
+# scheduler
+[core/scheduler/linear_warmup]
+num_warmup_rate = 0.001
 
 # task
-[core/auto/supervised_task]
-model = core/model/bert_for_classification
-optim = core/optim/adam
-dataset = core/dataset/auto
-loss_fn = core/loss/bce
-score_fn = core/score/accuracy
-monitor_fns = ['core/score/accuracy', 'core/score/roc_auc']
-output_header = query,doc
-post_process_fn = partial(core/process/base_post_for_string, actfn=torch.sigmoid, key='bert_score')
-
-opt_fp16 = O1
-from_ckpt_dir = ${core/auto:cache_dir}
-to_ckpt_dir = ${core/auto:cache_dir}
-output_path = ${core/auto:cache_dir}/output.txt
+[core/task/supervised]
+model = core/model/generation/bloom
+optim = core/optim/adamw
+scheduler = core/scheduler/linear_warmup
+dataset = core/dataset/ast
+loss_fn = core/loss/lm
+score_fn = core/score/bleu
+monitor_fns = ['core/score/bleu', 'core/score/rouge1', 'core/score/rouge2', 'core/score/rougel']
+output_header = ['encode']
+postprocess_fn = core/postprocess/bloom/detokenize
+writer = core/writer/csv
+
+from_ckpt_dir = ${core/cli:from_ckpt_dir}
+to_ckpt_dir = ${core/cli:cache_dir}
+output_path = ${core/cli:cache_dir}/output.txt
+train_batch_size = 4
+dev_batch_size = 8
+test_batch_size = 8
```

### Comparing `unitorch-0.0.0.1/unitorch_cli/auto_train.py` & `unitorch-0.0.0.2/src/unitorch/cli/console/eval.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,94 +1,74 @@
+# Copyright (c) FULIUCANSHENG.
+# Licensed under the MIT License.
+
 import os
 import sys
+import fire
 import logging
 import importlib
-import unitorch
-from unitorch import core_configure_parser, core_task, AUTO_CONFIG_FROM_HUB_DICT
-from unitorch.utils.hf import hf_cached_path
-import fire
-
-config_files_in_repo = os.walk(os.path.join(os.path.dirname(__file__), "../config"))
-CONFIG_FROM_REPO = dict()
-for root_dir, dirs, files in config_files_in_repo:
-    for file in files:
-        if file.endswith(".ini"):
-            config_path = os.path.normpath(os.path.join(root_dir, file))
-            config_name = config_path[:-4]
-            config_name = config_name[config_name.index('config'):]
-            CONFIG_FROM_REPO[config_name] = config_path
-
-
-TEMPLATE_FROM_REPO = dict()
-TEMPLATE_DIRS = [os.path.join(os.path.dirname(__file__), "../templates")]
-for template_dir in TEMPLATE_DIRS:
-    templates = os.listdir(template_dir)
-    templates = [os.path.normpath(os.path.join(template_dir, template)) for template in templates]
-    templates = list(filter(os.path.isdir, templates))
-    for template in templates:
-        template_path = os.path.normpath(os.path.join(template_dir, template))
-        template_name = template_path[template_path.index('templates'):]
-        TEMPLATE_FROM_REPO[template_name] = template_path
-
-AUTO_CONFIG_DICT = {
-    **AUTO_CONFIG_FROM_HUB_DICT,
-    **CONFIG_FROM_REPO,
-    **TEMPLATE_FROM_REPO,
-}
+import unitorch.cli
+from transformers.utils import is_remote_url
+from unitorch.cli import CoreConfigureParser
+from unitorch.cli import (
+    import_library,
+    cached_path,
+    set_global_config,
+    registered_task,
+    registered_script,
+    init_registered_module,
+)
 
-logging.info(AUTO_CONFIG_DICT)
 
-
-def train(cfg_path_or_dir, **kwargs):
+@fire.decorators.SetParseFn(str)
+def eval(config_path_or_dir: str, **kwargs):
     config_file = kwargs.pop("config_file", "config.ini")
-    assert cfg_path_or_dir in AUTO_CONFIG_DICT or os.path.exists(cfg_path_or_dir)
-    if cfg_path_or_dir in AUTO_CONFIG_DICT:
-        cfg_path = AUTO_CONFIG_DICT[cfg_path_or_dir]
-
-    if os.path.isdir(cfg_path_or_dir):
-        cfg_path = os.path.join(cfg_path_or_dir, config_file)
-        sys.path.insert(0, cfg_path_or_dir)
-        for f in os.listdir(cfg_path_or_dir):
-            fpath = os.path.join(cfg_path_or_dir, f)
+
+    if os.path.isdir(config_path_or_dir):
+        config_path = os.path.join(config_path_or_dir, config_file)
+        sys.path.insert(0, config_path_or_dir)
+        for f in os.listdir(config_path_or_dir):
+            fpath = os.path.normpath(os.path.join(config_path_or_dir, f))
             if (
                 not f.startswith("_")
                 and not f.startswith(".")
                 and (f.endswith(".py") or os.path.isdir(fpath))
             ):
                 fname = f[:-3] if f.endswith(".py") else f
                 module = importlib.import_module(f"{fname}")
-
-    elif os.path.isfile(cfg_path_or_dir):
-        cfg_path = cfg_path_or_dir
-
-    cfg_path = hf_cached_path(cfg_path)
+    else:
+        config_path = cached_path(config_path_or_dir)
 
     params = []
     for k, v in kwargs.items():
         if k.count("@") > 0:
             k0 = k.split("@")[0]
-            k1 = k.split("@")[1]
+            k1 = "@".join(k.split("@")[1:])
         else:
-            k0 = "core/auto"
+            k0 = "core/cli"
             k1 = k
         params.append((k0, k1, v))
 
-    cfg = core_configure_parser(cfg_path, params)
+    if config_path is not None:
+        config = CoreConfigureParser(config_path, params=params)
+    else:
+        config = CoreConfigureParser(params=params)
 
-    # init core libs
-    unitorch.init_core_group(cfg)
+    set_global_config(config)
 
-    task_type = cfg.getdefault("core/auto", "task_type", None)
-    assert task_type is not None
+    task_name = config.getdefault("core/cli", "task_name", None)
+    depends_libraries = config.getdefault("core/cli", "depends_libraries", None)
 
-    if task_type in unitorch.core_task:
-        unitorch.core_task.get(task_type).train()
-    else:
-        raise f"can't find the task {task_type}"
+    if depends_libraries:
+        for library in depends_libraries:
+            import_library(library)
 
+    assert task_name is not None and task_name in registered_task
+    cli_task = init_registered_module(task_name, config, registered_task)
 
-def cli_main():
-    fire.Fire(train)
+    cli_task.eval()
+
+    os._exit(0)
 
 
-if __name__ == "__main__":
-    fire.Fire(train)
+def cli_main():
+    fire.Fire(eval)
```

### Comparing `unitorch-0.0.0.1/unitorch_cli/auto_infer.py` & `unitorch-0.0.0.2/src/unitorch/cli/console/train.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,95 +1,74 @@
+# Copyright (c) FULIUCANSHENG.
+# Licensed under the MIT License.
+
 import os
 import sys
+import fire
 import logging
 import importlib
-import unitorch
-from unitorch import core_configure_parser, core_task, AUTO_CONFIG_FROM_HUB_DICT
-from unitorch.utils.hf import hf_cached_path
-import fire
-
-config_files_in_repo = os.walk(os.path.join(os.path.dirname(__file__), "../config"))
-CONFIG_FROM_REPO = dict()
-for root_dir, dirs, files in config_files_in_repo:
-    for file in files:
-        if file.endswith(".ini"):
-            config_path = os.path.normpath(os.path.join(root_dir, file))
-            config_name = config_path[:-4]
-            config_name = config_name[config_name.index('config'):]
-            CONFIG_FROM_REPO[config_name] = config_path
-
-
-TEMPLATE_FROM_REPO = dict()
-TEMPLATE_DIRS = [os.path.join(os.path.dirname(__file__), "../templates")]
-for template_dir in TEMPLATE_DIRS:
-    templates = os.listdir(template_dir)
-    templates = [os.path.normpath(os.path.join(template_dir, template)) for template in templates]
-    templates = list(filter(os.path.isdir, templates))
-    for template in templates:
-        template_path = os.path.normpath(os.path.join(template_dir, template))
-        template_name = template_path[template_path.index('templates'):]
-        TEMPLATE_FROM_REPO[template_name] = template_path
-
-
-AUTO_CONFIG_DICT = {
-    **AUTO_CONFIG_FROM_HUB_DICT,
-    **CONFIG_FROM_REPO,
-    **TEMPLATE_FROM_REPO,
-}
+import unitorch.cli
+from transformers.utils import is_remote_url
+from unitorch.cli import CoreConfigureParser
+from unitorch.cli import (
+    import_library,
+    cached_path,
+    set_global_config,
+    registered_task,
+    registered_script,
+    init_registered_module,
+)
 
-logging.info(AUTO_CONFIG_DICT)
 
-
-def infer(cfg_path_or_dir, **kwargs):
+@fire.decorators.SetParseFn(str)
+def train(config_path_or_dir: str, **kwargs):
     config_file = kwargs.pop("config_file", "config.ini")
-    assert cfg_path_or_dir in AUTO_CONFIG_DICT or os.path.exists(cfg_path_or_dir)
-    if cfg_path_or_dir in AUTO_CONFIG_DICT:
-        cfg_path = AUTO_CONFIG_DICT[cfg_path_or_dir]
-
-    if os.path.isdir(cfg_path_or_dir):
-        cfg_path = os.path.join(cfg_path_or_dir, config_file)
-        sys.path.insert(0, cfg_path_or_dir)
-        for f in os.listdir(cfg_path_or_dir):
-            fpath = os.path.normpath(os.path.join(cfg_path_or_dir, f))
+
+    if os.path.isdir(config_path_or_dir):
+        config_path = os.path.join(config_path_or_dir, config_file)
+        sys.path.insert(0, config_path_or_dir)
+        for f in os.listdir(config_path_or_dir):
+            fpath = os.path.normpath(os.path.join(config_path_or_dir, f))
             if (
                 not f.startswith("_")
                 and not f.startswith(".")
                 and (f.endswith(".py") or os.path.isdir(fpath))
             ):
                 fname = f[:-3] if f.endswith(".py") else f
                 module = importlib.import_module(f"{fname}")
-
-    elif os.path.isfile(cfg_path_or_dir):
-        cfg_path = cfg_path_or_dir
-
-    cfg_path = hf_cached_path(cfg_path)
+    else:
+        config_path = cached_path(config_path_or_dir)
 
     params = []
     for k, v in kwargs.items():
         if k.count("@") > 0:
             k0 = k.split("@")[0]
-            k1 = k.split("@")[1]
+            k1 = "@".join(k.split("@")[1:])
         else:
-            k0 = "core/auto"
+            k0 = "core/cli"
             k1 = k
         params.append((k0, k1, v))
 
-    cfg = core_configure_parser(cfg_path, params)
+    if config_path is not None:
+        config = CoreConfigureParser(config_path, params=params)
+    else:
+        config = CoreConfigureParser(params=params)
 
-    # init core libs
-    unitorch.init_core_group(cfg)
+    set_global_config(config)
 
-    task_type = cfg.getdefault("core/auto", "task_type", None)
-    assert task_type is not None
+    task_name = config.getdefault("core/cli", "task_name", None)
+    depends_libraries = config.getdefault("core/cli", "depends_libraries", None)
 
-    if task_type in unitorch.core_task:
-        unitorch.core_task.get(task_type).infer()
-    else:
-        raise f"can't find task {task_type}"
+    if depends_libraries:
+        for library in depends_libraries:
+            import_library(library)
 
+    assert task_name is not None and task_name in registered_task
+    cli_task = init_registered_module(task_name, config, registered_task)
 
-def cli_main():
-    fire.Fire(infer)
+    cli_task.train()
+
+    os._exit(0)
 
 
-if __name__ == "__main__":
-    fire.Fire(infer)
+def cli_main():
+    fire.Fire(train)
```

