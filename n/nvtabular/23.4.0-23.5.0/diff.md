# Comparing `tmp/nvtabular-23.4.0.tar.gz` & `tmp/nvtabular-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvtabular-23.4.0.tar", last modified: Wed Apr 26 19:16:38 2023, max compression
+gzip compressed data, was "nvtabular-23.5.0.tar", last modified: Wed May 31 14:39:50 2023, max compression
```

## Comparing `nvtabular-23.4.0.tar` & `nvtabular-23.5.0.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.698010 nvtabular-23.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 19:15:49.000000 nvtabular-23.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-26 19:15:49.000000 nvtabular-23.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-04-26 19:16:38.698010 nvtabular-23.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-26 19:15:49.000000 nvtabular-23.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.678010 nvtabular-23.4.0/cpp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.682010 nvtabular-23.4.0/cpp/nvtabular/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-26 19:15:49.000000 nvtabular-23.4.0/cpp/nvtabular/__init__.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.682010 nvtabular-23.4.0/cpp/nvtabular/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-26 19:15:49.000000 nvtabular-23.4.0/cpp/nvtabular/inference/__init__.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-04-26 19:15:49.000000 nvtabular-23.4.0/cpp/nvtabular/inference/categorify.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-26 19:15:49.000000 nvtabular-23.4.0/cpp/nvtabular/inference/fill.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.678010 nvtabular-23.4.0/merlin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.682010 nvtabular-23.4.0/merlin/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-26 19:15:49.000000 nvtabular-23.4.0/merlin/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.682010 nvtabular-23.4.0/merlin/transforms/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-26 19:15:49.000000 nvtabular-23.4.0/merlin/transforms/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.698010 nvtabular-23.4.0/nvtabular/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-26 19:16:38.698010 nvtabular-23.4.0/nvtabular/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/dispatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.686010 nvtabular-23.4.0/nvtabular/framework_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.686010 nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/feature_column_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.686010 nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/layers/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/layers/outer_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/tfrecords_to_parquet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.686010 nvtabular-23.4.0/nvtabular/framework_utils/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.686010 nvtabular-23.4.0/nvtabular/framework_utils/torch/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/torch/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/torch/layers/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/torch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/framework_utils/torch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.690010 nvtabular-23.4.0/nvtabular/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.690010 nvtabular-23.4.0/nvtabular/inference/triton/
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/triton/benchmarking_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/triton/data_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25369 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/triton/ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.690010 nvtabular-23.4.0/nvtabular/inference/triton/model/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/triton/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9542 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/triton/model/model_pt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/triton/workflow_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.690010 nvtabular-23.4.0/nvtabular/inference/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/workflow/hugectr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/workflow/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/inference/workflow/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.690010 nvtabular-23.4.0/nvtabular/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/loader/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/loader/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/loader/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/loader/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.698010 nvtabular-23.4.0/nvtabular/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/add_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/bucketize.py
--rw-r--r--   0 runner    (1001) docker     (123)    61346 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/categorify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/column_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/data_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/difference_lag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/drop_low_cardinality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/dropna.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/hash_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/hashed_cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/join_external.py
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/join_groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/lambdaop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/list_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/logop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/moments.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/reduce_dtype_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/stat_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/target_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/ops/value_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.698010 nvtabular-23.4.0/nvtabular/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17101 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/tools/data_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/tools/dataset_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/tools/inspector_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.698010 nvtabular-23.4.0/nvtabular/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/workflow/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/workflow/node.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17893 2023-04-26 19:15:49.000000 nvtabular-23.4.0/nvtabular/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.686010 nvtabular-23.4.0/nvtabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-04-26 19:16:38.000000 nvtabular-23.4.0/nvtabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-26 19:16:38.000000 nvtabular-23.4.0/nvtabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:16:38.000000 nvtabular-23.4.0/nvtabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:16:38.000000 nvtabular-23.4.0/nvtabular.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-26 19:16:38.000000 nvtabular-23.4.0/nvtabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-26 19:16:38.000000 nvtabular-23.4.0/nvtabular.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-26 19:15:49.000000 nvtabular-23.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:16:38.698010 nvtabular-23.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 19:15:49.000000 nvtabular-23.4.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-26 19:15:49.000000 nvtabular-23.4.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-26 19:15:49.000000 nvtabular-23.4.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 19:15:49.000000 nvtabular-23.4.0/requirements/gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-26 19:15:49.000000 nvtabular-23.4.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-26 19:16:38.698010 nvtabular-23.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-26 19:15:49.000000 nvtabular-23.4.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81319 2023-04-26 19:15:49.000000 nvtabular-23.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.997602 nvtabular-23.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 14:39:10.000000 nvtabular-23.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-31 14:39:10.000000 nvtabular-23.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-05-31 14:39:49.997602 nvtabular-23.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-05-31 14:39:10.000000 nvtabular-23.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.985602 nvtabular-23.5.0/cpp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.985602 nvtabular-23.5.0/cpp/nvtabular/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-31 14:39:10.000000 nvtabular-23.5.0/cpp/nvtabular/__init__.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.985602 nvtabular-23.5.0/cpp/nvtabular/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-31 14:39:10.000000 nvtabular-23.5.0/cpp/nvtabular/inference/__init__.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-31 14:39:10.000000 nvtabular-23.5.0/cpp/nvtabular/inference/categorify.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-31 14:39:10.000000 nvtabular-23.5.0/cpp/nvtabular/inference/fill.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.985602 nvtabular-23.5.0/merlin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.985602 nvtabular-23.5.0/merlin/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-31 14:39:10.000000 nvtabular-23.5.0/merlin/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.985602 nvtabular-23.5.0/merlin/transforms/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-31 14:39:10.000000 nvtabular-23.5.0/merlin/transforms/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.997602 nvtabular-23.5.0/nvtabular/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-31 14:39:49.997602 nvtabular-23.5.0/nvtabular/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/dispatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular/framework_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/feature_column_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/layers/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/layers/outer_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/tfrecords_to_parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular/framework_utils/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular/framework_utils/torch/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/torch/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/torch/layers/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/torch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/torch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular/inference/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/triton/benchmarking_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/triton/data_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25369 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/triton/ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular/inference/triton/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/triton/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9542 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/triton/model/model_pt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/triton/workflow_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular/inference/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/workflow/hugectr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/workflow/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/workflow/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.993602 nvtabular-23.5.0/nvtabular/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/loader/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/loader/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/loader/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/loader/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.993602 nvtabular-23.5.0/nvtabular/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/add_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/bucketize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61346 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/categorify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10299 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/column_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/data_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/difference_lag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/drop_low_cardinality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/dropna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/hash_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/hashed_cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/join_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/join_groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/lambdaop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/list_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/logop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/reduce_dtype_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/stat_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16901 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/target_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/value_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.993602 nvtabular-23.5.0/nvtabular/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17101 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/tools/data_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/tools/dataset_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/tools/inspector_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.993602 nvtabular-23.5.0/nvtabular/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/workflow/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/workflow/node.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17893 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-05-31 14:39:49.000000 nvtabular-23.5.0/nvtabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-31 14:39:49.000000 nvtabular-23.5.0/nvtabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:39:49.000000 nvtabular-23.5.0/nvtabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:39:49.000000 nvtabular-23.5.0/nvtabular.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-31 14:39:49.000000 nvtabular-23.5.0/nvtabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 14:39:49.000000 nvtabular-23.5.0/nvtabular.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-31 14:39:10.000000 nvtabular-23.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.997602 nvtabular-23.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 14:39:10.000000 nvtabular-23.5.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-31 14:39:10.000000 nvtabular-23.5.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-31 14:39:10.000000 nvtabular-23.5.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:39:10.000000 nvtabular-23.5.0/requirements/gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-31 14:39:10.000000 nvtabular-23.5.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-31 14:39:49.997602 nvtabular-23.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-31 14:39:10.000000 nvtabular-23.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81319 2023-05-31 14:39:10.000000 nvtabular-23.5.0/versioneer.py
```

### Comparing `nvtabular-23.4.0/LICENSE` & `nvtabular-23.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/PKG-INFO` & `nvtabular-23.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvtabular
-Version: 23.4.0
+Version: 23.5.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/NVTabular
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nvtabular-23.4.0/README.md` & `nvtabular-23.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/cpp/nvtabular/__init__.cc` & `nvtabular-23.5.0/cpp/nvtabular/__init__.cc`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/cpp/nvtabular/inference/__init__.cc` & `nvtabular-23.5.0/cpp/nvtabular/inference/__init__.cc`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/cpp/nvtabular/inference/categorify.cc` & `nvtabular-23.5.0/cpp/nvtabular/inference/categorify.cc`

 * *Files 3% similar despite different names*

```diff
@@ -89,28 +89,34 @@
               insert_int_mapping<double>(values);
               return;
             }
             break;
           case 'u':
             switch (dtype.itemsize())
             {
+            case 1:
+              insert_int_mapping<uint8_t>(values);
+              return;
             case 2:
               insert_int_mapping<uint16_t>(values);
               return;
             case 4:
               insert_int_mapping<uint32_t>(values);
               return;
             case 8:
               insert_int_mapping<uint64_t>(values);
               return;
             }
             break;
           case 'i':
             switch (dtype.itemsize())
             {
+            case 1:
+              insert_int_mapping<int8_t>(values);
+              return;
             case 2:
               insert_int_mapping<int16_t>(values);
               return;
             case 4:
               insert_int_mapping<int32_t>(values);
               return;
             case 8:
@@ -200,25 +206,29 @@
             case 8:
               return transform_int<double>(input);
             }
             break;
           case 'u':
             switch (itemsize)
             {
+            case 1:
+              return transform_int<uint8_t>(input);
             case 2:
               return transform_int<uint16_t>(input);
             case 4:
               return transform_int<uint32_t>(input);
             case 8:
               return transform_int<uint64_t>(input);
             }
             break;
           case 'i':
             switch (itemsize)
             {
+            case 1:
+              return transform_int<int8_t>(input);
             case 2:
               return transform_int<int16_t>(input);
             case 4:
               return transform_int<int32_t>(input);
             case 8:
               return transform_int<int64_t>(input);
             }
```

### Comparing `nvtabular-23.4.0/cpp/nvtabular/inference/fill.cc` & `nvtabular-23.5.0/cpp/nvtabular/inference/fill.cc`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/merlin/transforms/__init__.py` & `nvtabular-23.5.0/merlin/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/merlin/transforms/ops/__init__.py` & `nvtabular-23.5.0/merlin/transforms/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/__init__.py` & `nvtabular-23.5.0/nvtabular/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/dispatch.py` & `nvtabular-23.5.0/nvtabular/dispatch.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/framework_utils/__init__.py` & `nvtabular-23.5.0/nvtabular/framework_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/__init__.py` & `nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/feature_column_utils.py` & `nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/feature_column_utils.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/layers/__init__.py` & `nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/layers/embedding.py` & `nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/layers/interaction.py` & `nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/layers/interaction.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/layers/outer_product.py` & `nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/layers/outer_product.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/framework_utils/tensorflow/tfrecords_to_parquet.py` & `nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/tfrecords_to_parquet.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/framework_utils/torch/__init__.py` & `nvtabular-23.5.0/nvtabular/framework_utils/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/framework_utils/torch/layers/__init__.py` & `nvtabular-23.5.0/nvtabular/framework_utils/torch/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/framework_utils/torch/layers/embeddings.py` & `nvtabular-23.5.0/nvtabular/framework_utils/torch/layers/embeddings.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/framework_utils/torch/models.py` & `nvtabular-23.5.0/nvtabular/framework_utils/torch/models.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/framework_utils/torch/utils.py` & `nvtabular-23.5.0/nvtabular/framework_utils/torch/utils.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/graph.py` & `nvtabular-23.5.0/nvtabular/graph.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/inference/__init__.py` & `nvtabular-23.5.0/nvtabular/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/inference/triton/__init__.py` & `nvtabular-23.5.0/nvtabular/inference/triton/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/inference/triton/benchmarking_tools.py` & `nvtabular-23.5.0/nvtabular/inference/triton/benchmarking_tools.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/inference/triton/data_conversions.py` & `nvtabular-23.5.0/nvtabular/inference/triton/data_conversions.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/inference/triton/ensemble.py` & `nvtabular-23.5.0/nvtabular/inference/triton/ensemble.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/inference/triton/model/__init__.py` & `nvtabular-23.5.0/nvtabular/inference/triton/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/inference/triton/model/model_pt.py` & `nvtabular-23.5.0/nvtabular/inference/triton/model/model_pt.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/inference/triton/workflow_model.py` & `nvtabular-23.5.0/nvtabular/inference/triton/workflow_model.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/inference/workflow/__init__.py` & `nvtabular-23.5.0/nvtabular/inference/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/inference/workflow/base.py` & `nvtabular-23.5.0/nvtabular/inference/workflow/base.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/inference/workflow/hugectr.py` & `nvtabular-23.5.0/nvtabular/inference/workflow/hugectr.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/inference/workflow/pytorch.py` & `nvtabular-23.5.0/nvtabular/inference/workflow/pytorch.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/inference/workflow/tensorflow.py` & `nvtabular-23.5.0/nvtabular/inference/workflow/tensorflow.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/io.py` & `nvtabular-23.5.0/nvtabular/io.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/loader/__init__.py` & `nvtabular-23.5.0/nvtabular/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/loader/backend.py` & `nvtabular-23.5.0/nvtabular/loader/backend.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/loader/tensorflow.py` & `nvtabular-23.5.0/nvtabular/loader/tensorflow.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/loader/tf_utils.py` & `nvtabular-23.5.0/nvtabular/loader/tf_utils.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/loader/torch.py` & `nvtabular-23.5.0/nvtabular/loader/torch.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/__init__.py` & `nvtabular-23.5.0/nvtabular/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/add_metadata.py` & `nvtabular-23.5.0/nvtabular/ops/add_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,20 +50,20 @@
     def __init__(self, properties=None):
         super().__init__(properties=properties)
 
 
 # Wrappers for common features
 class TagAsUserID(AddTags):
     def __init__(self, tags=None):
-        super().__init__(tags=[Tags.USER_ID, Tags.USER])
+        super().__init__(tags=[Tags.ID, Tags.USER])
 
 
 class TagAsItemID(AddTags):
     def __init__(self, tags=None):
-        super().__init__(tags=[Tags.ITEM_ID, Tags.ITEM])
+        super().__init__(tags=[Tags.ID, Tags.ITEM])
 
 
 class TagAsUserFeatures(AddTags):
     def __init__(self, tags=None):
         super().__init__(tags=[Tags.USER])
```

### Comparing `nvtabular-23.4.0/nvtabular/ops/bucketize.py` & `nvtabular-23.5.0/nvtabular/ops/bucketize.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/categorify.py` & `nvtabular-23.5.0/nvtabular/ops/categorify.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/clip.py` & `nvtabular-23.5.0/nvtabular/ops/clip.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/column_similarity.py` & `nvtabular-23.5.0/nvtabular/ops/column_similarity.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
     @property
     def output_tags(self):
         return [Tags.CONTINUOUS]
 
     @property
     def output_dtype(self):
-        return numpy.float
+        return float
 
 
 def row_wise_inner_product(a, a_features, b, b_features, on_device=True):
     """Computes the similarity between two columns, by computing the inner product
     along two sparse feature matrices . Both a_features and b_features are
     required to be in canonical CSR format.
```

### Comparing `nvtabular-23.4.0/nvtabular/ops/data_stats.py` & `nvtabular-23.5.0/nvtabular/ops/data_stats.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/difference_lag.py` & `nvtabular-23.5.0/nvtabular/ops/difference_lag.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/drop_low_cardinality.py` & `nvtabular-23.5.0/nvtabular/ops/drop_low_cardinality.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/dropna.py` & `nvtabular-23.5.0/nvtabular/ops/dropna.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/fill.py` & `nvtabular-23.5.0/nvtabular/ops/fill.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/filter.py` & `nvtabular-23.5.0/nvtabular/ops/filter.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/groupby.py` & `nvtabular-23.5.0/nvtabular/ops/groupby.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/hash_bucket.py` & `nvtabular-23.5.0/nvtabular/ops/hash_bucket.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/hashed_cross.py` & `nvtabular-23.5.0/nvtabular/ops/hashed_cross.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/join_external.py` & `nvtabular-23.5.0/nvtabular/ops/join_external.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/join_groupby.py` & `nvtabular-23.5.0/nvtabular/ops/join_groupby.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/lambdaop.py` & `nvtabular-23.5.0/nvtabular/ops/lambdaop.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/list_slice.py` & `nvtabular-23.5.0/nvtabular/ops/list_slice.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,24 +75,33 @@
             self.max_elements = self.end - self.start
 
     @annotate("ListSlice_op", color="darkgreen", domain="nvt_python")
     def transform(self, col_selector: ColumnSelector, df: DataFrameType) -> DataFrameType:
         on_cpu = is_cpu_object(df)
         ret = type(df)()
 
+        if on_cpu:
+            xp = np
+        else:
+            xp = cp
+
         for col in col_selector.names:
             # handle CPU via normal python slicing (not very efficient)
             if on_cpu:
                 values = [row[self.start : self.end] for row in df[col]]
 
                 # pad out to so each row has self.max_elements if asked
                 if self.pad:
                     for v in values:
                         if len(v) < self.max_elements:
-                            v.extend([self.pad_value] * (self.max_elements - len(v)))
+                            padding = [self.pad_value] * (self.max_elements - len(v))
+                            if isinstance(v, xp.ndarray):
+                                xp.append(v, padding)
+                            else:
+                                v.extend(padding)
 
                 ret[col] = values
             else:
                 # figure out the size of each row from the list offsets
                 c = df[col]._column
                 offsets = c.offsets.values
                 elements = c.elements.values
@@ -111,33 +120,43 @@
                     _calculate_row_sizes[blocks, threads](
                         self.start, self.end, offsets, new_offsets
                     )
                     new_offsets = cp.cumsum(new_offsets).astype(offsets.dtype)
 
                 # create a new array for the sliced elements
                 new_elements = cp.full(
-                    new_offsets[-1].item(), fill_value=self.pad_value, dtype=elements.dtype
+                    new_offsets[-1].item(),
+                    fill_value=self.pad_value,
+                    dtype=elements.dtype,
                 )
                 if new_elements.size:
                     _slice_rows[blocks, threads](
-                        self.start, self.end, offsets, elements, new_offsets, new_elements
+                        self.start,
+                        self.end,
+                        offsets,
+                        elements,
+                        new_offsets,
+                        new_elements,
                     )
 
                 # build up a list column with the sliced values
                 ret[col] = build_cudf_list_column(new_elements, new_offsets)
 
         return ret
 
     def _compute_dtype(self, col_schema, input_schema):
         col_schema = super()._compute_dtype(col_schema, input_schema)
         return col_schema.with_dtype(col_schema.dtype)
 
     def _compute_properties(self, col_schema, input_schema):
         col_schema = super()._compute_properties(col_schema, input_schema)
-        properties = {**col_schema.properties, **{"value_count": {"min": 0, "max": None}}}
+        properties = {
+            **col_schema.properties,
+            **{"value_count": {"min": 0, "max": None}},
+        }
         if self.max_elements != np.iinfo(np.int64).max:
             properties["value_count"]["max"] = self.max_elements
             if self.pad:
                 properties["value_count"]["min"] = self.max_elements
         return col_schema.with_properties(properties)
 
     def _compute_shape(self, col_schema, input_schema):
```

### Comparing `nvtabular-23.4.0/nvtabular/ops/logop.py` & `nvtabular-23.5.0/nvtabular/ops/logop.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/moments.py` & `nvtabular-23.5.0/nvtabular/ops/moments.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/normalize.py` & `nvtabular-23.5.0/nvtabular/ops/normalize.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/operator.py` & `nvtabular-23.5.0/nvtabular/ops/operator.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/reduce_dtype_size.py` & `nvtabular-23.5.0/nvtabular/ops/reduce_dtype_size.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/rename.py` & `nvtabular-23.5.0/nvtabular/ops/rename.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/stat_operator.py` & `nvtabular-23.5.0/nvtabular/ops/stat_operator.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/ops/target_encoding.py` & `nvtabular-23.5.0/nvtabular/ops/target_encoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
 
         return column_mapping
 
     def _compute_dtype(self, col_schema, input_schema):
         if input_schema.column_schemas:
             new_schema = super()._compute_dtype(col_schema, input_schema)
         else:
-            # fold only, setting the np.int
+            # fold only, setting the dtype to int
             new_schema = col_schema.with_dtype(np.uint8)
         return new_schema
 
     def _compute_tags(self, col_schema, input_schema):
         if input_schema.column_schemas:
             source_col_name = input_schema.column_names[0]
             return col_schema.with_tags(input_schema[source_col_name].tags + self.output_tags)
```

### Comparing `nvtabular-23.4.0/nvtabular/ops/value_counts.py` & `nvtabular-23.5.0/nvtabular/ops/value_counts.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/tools/__init__.py` & `nvtabular-23.5.0/nvtabular/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/tools/data_gen.py` & `nvtabular-23.5.0/nvtabular/tools/data_gen.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/tools/dataset_inspector.py` & `nvtabular-23.5.0/nvtabular/tools/dataset_inspector.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/tools/inspector_script.py` & `nvtabular-23.5.0/nvtabular/tools/inspector_script.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/utils.py` & `nvtabular-23.5.0/nvtabular/utils.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/worker.py` & `nvtabular-23.5.0/nvtabular/worker.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/workflow/__init__.py` & `nvtabular-23.5.0/nvtabular/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/workflow/node.py` & `nvtabular-23.5.0/nvtabular/workflow/node.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular/workflow/workflow.py` & `nvtabular-23.5.0/nvtabular/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/nvtabular.egg-info/PKG-INFO` & `nvtabular-23.5.0/nvtabular.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvtabular
-Version: 23.4.0
+Version: 23.5.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/NVTabular
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nvtabular-23.4.0/nvtabular.egg-info/SOURCES.txt` & `nvtabular-23.5.0/nvtabular.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/pyproject.toml` & `nvtabular-23.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/setup.cfg` & `nvtabular-23.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/setup.py` & `nvtabular-23.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.4.0/versioneer.py` & `nvtabular-23.5.0/versioneer.py`

 * *Files identical despite different names*

