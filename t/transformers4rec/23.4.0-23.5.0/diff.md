# Comparing `tmp/transformers4rec-23.4.0.tar.gz` & `tmp/transformers4rec-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers4rec-23.4.0.tar", last modified: Wed Apr 26 21:12:08 2023, max compression
+gzip compressed data, was "transformers4rec-23.5.0.tar", last modified: Wed May 31 14:39:50 2023, max compression
```

## Comparing `transformers4rec-23.4.0.tar` & `transformers4rec-23.5.0.tar`

### file list

```diff
@@ -1,192 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/CLA.md
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/_images/
--rw-r--r--   0 runner    (1001) docker     (123)    60445 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/_images/DP_DDP_perf.png
--rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/_images/nlp_x_recsys.png
--rw-r--r--   0 runner    (1001) docker     (123)    57700 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/_images/pipeline.png
--rw-r--r--   0 runner    (1001) docker     (123)   139511 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/_images/preproc_data_example.png
--rw-r--r--   0 runner    (1001) docker     (123)    53017 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/_images/sequential_rec.png
--rw-r--r--   0 runner    (1001) docker     (123)   123737 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/_images/transformers4rec_metaarchitecture.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/merlin_standard_lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/merlin_standard_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/merlin_standard_lib/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/merlin_standard_lib/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34895 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/merlin_standard_lib/proto/schema_bp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/merlin_standard_lib/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/merlin_standard_lib/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/merlin_standard_lib/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/merlin_standard_lib/schema/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/merlin_standard_lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/merlin_standard_lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/merlin_standard_lib/utils/embedding_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/requirements/base_external.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/requirements/base_merlin.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/requirements/nvtabular.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/requirements/pytorch.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.621868 transformers4rec-23.4.0/tests/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/tests/integration/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/integration/notebooks/test_getting_started_session_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/integration/notebooks/test_notebooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/tests/unit/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.625868 transformers4rec-23.4.0/tests/unit/assets/data_schema/
--rw-r--r--   0 runner    (1001) docker     (123)    42012 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/assets/data_schema/data.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/assets/data_schema/data_schema.pbtxt
--rw-r--r--   0 runner    (1001) docker     (123)   105788 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/assets/data_schema/data_seq.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/assets/data_schema/data_seq_schema.pbtxt
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/assets/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/config/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/config/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/config/test_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/config/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/data/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/data/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/data/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/data/testing/tabular_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/data/testing/tabular_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/data/testing/tabular_data/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/data/testing/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/merlin_standard_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/merlin_standard_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/merlin_standard_lib/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/merlin_standard_lib/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/merlin_standard_lib/schema/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/_conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/torch/block/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/block/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/block/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/block/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/block/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/torch/features/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/features/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/features/test_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/features/test_sequential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/features/test_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/torch/model/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/model/test_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/model/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/torch/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/tabular/test_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/tabular/test_tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/tabular/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/test_dataloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/test_experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/test_public_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/test_ranking_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/test_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (123)    20084 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/test_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.629868 transformers4rec-23.4.0/tests/unit/torch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/utils/test_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/torch/utils/test_torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.633868 transformers4rec-23.4.0/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/utils/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tests/unit/utils/test_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/transformers4rec/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/transformers4rec/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.633868 transformers4rec-23.4.0/transformers4rec/config/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/config/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/config/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/config/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.633868 transformers4rec-23.4.0/transformers4rec/data/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.633868 transformers4rec-23.4.0/transformers4rec/data/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   105788 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/data.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.633868 transformers4rec-23.4.0/transformers4rec/data/testing/music_streaming/
--rw-r--r--   0 runner    (1001) docker     (123)   279958 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/music_streaming/data.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/music_streaming/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/music_streaming/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.633868 transformers4rec-23.4.0/transformers4rec/data/testing/tabular_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/tabular_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42012 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/tabular_data/data.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/tabular_data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/testing/tabular_data/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/data/yoochoose.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.633868 transformers4rec-23.4.0/transformers4rec/torch/
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/transformers4rec/torch/block/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/block/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/block/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/block/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/block/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/transformers4rec/torch/features/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/features/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/features/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    20993 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/features/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/features/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/features/tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/features/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    35959 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/masking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/transformers4rec/torch/model/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30310 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    27127 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/model/prediction_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/ranking_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/transformers4rec/torch/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/tabular/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/tabular/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/tabular/transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    35065 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/transformers4rec/torch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/utils/examples_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/utils/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/utils/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16202 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/torch/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.637868 transformers4rec-23.4.0/transformers4rec/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/transformers4rec/utils/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:12:08.633868 transformers4rec-23.4.0/transformers4rec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-04-26 21:12:08.000000 transformers4rec-23.4.0/transformers4rec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-26 21:12:08.000000 transformers4rec-23.4.0/transformers4rec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:12:08.000000 transformers4rec-23.4.0/transformers4rec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-26 21:12:08.000000 transformers4rec-23.4.0/transformers4rec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 21:12:08.000000 transformers4rec-23.4.0/transformers4rec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    81319 2023-04-26 21:01:39.000000 transformers4rec-23.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.492529 transformers4rec-23.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/CLA.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-05-31 14:39:50.492529 transformers4rec-23.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    60445 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/_images/DP_DDP_perf.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/_images/nlp_x_recsys.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57700 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/_images/pipeline.png
+-rw-r--r--   0 runner    (1001) docker     (123)   139511 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/_images/preproc_data_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53017 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/_images/sequential_rec.png
+-rw-r--r--   0 runner    (1001) docker     (123)   123737 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/_images/transformers4rec_metaarchitecture.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/merlin_standard_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/merlin_standard_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/merlin_standard_lib/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/merlin_standard_lib/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34895 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/merlin_standard_lib/proto/schema_bp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/merlin_standard_lib/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/merlin_standard_lib/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/merlin_standard_lib/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/merlin_standard_lib/schema/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/merlin_standard_lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/merlin_standard_lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/merlin_standard_lib/utils/embedding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/requirements/base_external.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/requirements/base_merlin.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/requirements/nvtabular.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/requirements/pytorch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-31 14:39:50.492529 transformers4rec-23.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.476529 transformers4rec-23.5.0/tests/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/integration/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/integration/notebooks/test_getting_started_session_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/integration/notebooks/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/unit/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/unit/assets/data_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    42012 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/assets/data_schema/data.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/assets/data_schema/data_schema.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (123)   105788 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/assets/data_schema/data_seq.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/assets/data_schema/data_seq_schema.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/assets/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/unit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/config/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/config/test_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/config/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/unit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/data/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/unit/data/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/data/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/unit/data/testing/tabular_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/data/testing/tabular_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/data/testing/tabular_data/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/data/testing/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/unit/merlin_standard_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/merlin_standard_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.484529 transformers4rec-23.5.0/tests/unit/merlin_standard_lib/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/merlin_standard_lib/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/merlin_standard_lib/schema/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.484529 transformers4rec-23.5.0/tests/unit/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/_conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.484529 transformers4rec-23.5.0/tests/unit/torch/block/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/block/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/block/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/block/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/block/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.484529 transformers4rec-23.5.0/tests/unit/torch/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/features/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/features/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/features/test_sequential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/features/test_tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.484529 transformers4rec-23.5.0/tests/unit/torch/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/model/test_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/model/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.484529 transformers4rec-23.5.0/tests/unit/torch/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/tabular/test_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/tabular/test_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/tabular/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_dataloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_public_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_ranking_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_torchscript_with_topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20084 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.484529 transformers4rec-23.5.0/tests/unit/torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/utils/test_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/utils/test_torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.484529 transformers4rec-23.5.0/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/utils/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/utils/test_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.492529 transformers4rec-23.5.0/transformers4rec/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-31 14:39:50.492529 transformers4rec-23.5.0/transformers4rec/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.488529 transformers4rec-23.5.0/transformers4rec/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/config/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/config/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/config/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.488529 transformers4rec-23.5.0/transformers4rec/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.488529 transformers4rec-23.5.0/transformers4rec/data/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105788 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/data.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.488529 transformers4rec-23.5.0/transformers4rec/data/testing/music_streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)   279958 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/music_streaming/data.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/music_streaming/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/music_streaming/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.488529 transformers4rec-23.5.0/transformers4rec/data/testing/tabular_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/tabular_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42012 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/tabular_data/data.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/tabular_data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/tabular_data/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/yoochoose.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.488529 transformers4rec-23.5.0/transformers4rec/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.488529 transformers4rec-23.5.0/transformers4rec/torch/block/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/block/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/block/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/block/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/block/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.488529 transformers4rec-23.5.0/transformers4rec/torch/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/features/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/features/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20993 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/features/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/features/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/features/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/features/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35959 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/masking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.492529 transformers4rec-23.5.0/transformers4rec/torch/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32200 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27439 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/model/prediction_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/ranking_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.492529 transformers4rec-23.5.0/transformers4rec/torch/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/tabular/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22373 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/tabular/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/tabular/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35389 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.492529 transformers4rec-23.5.0/transformers4rec/torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/utils/examples_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/utils/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/utils/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16202 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.492529 transformers4rec-23.5.0/transformers4rec/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/utils/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.488529 transformers4rec-23.5.0/transformers4rec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-05-31 14:39:50.000000 transformers4rec-23.5.0/transformers4rec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-31 14:39:50.000000 transformers4rec-23.5.0/transformers4rec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:39:50.000000 transformers4rec-23.5.0/transformers4rec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-31 14:39:50.000000 transformers4rec-23.5.0/transformers4rec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 14:39:50.000000 transformers4rec-23.5.0/transformers4rec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    81319 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/versioneer.py
```

### Comparing `transformers4rec-23.4.0/.pre-commit-config.yaml` & `transformers4rec-23.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/CLA.md` & `transformers4rec-23.5.0/CLA.md`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/CONTRIBUTING.md` & `transformers4rec-23.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/LICENSE` & `transformers4rec-23.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/MANIFEST.in` & `transformers4rec-23.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/PKG-INFO` & `transformers4rec-23.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers4rec
-Version: 23.4.0
+Version: 23.5.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/Transformers4Rec
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -103,14 +103,15 @@
 
 3. Construct a transformer-body and convert this into a model.
 
 The following code sample shows how to define and train an XLNet model with PyTorch for next-item prediction task:
 
 ```python
 from transformers4rec import torch as tr
+from transformers4rec.torch.ranking_metric import NDCGAt, RecallAt
 
 # Create a schema or read one from disk: tr.Schema().from_json(SCHEMA_PATH).
 schema: tr.Schema = tr.data.tabular_sequence_testing_data.schema
 
 max_sequence_length, d_model = 20, 64
 
 # Define the input module to process the tabular input features.
@@ -164,27 +165,37 @@
 You can install Transformers4Rec with the functionality to use the GPU-accelerated Merlin dataloader.
 Installation with the dataloader is highly recommended for better performance.
 Those components can be installed as optional arguments for the `pip install` command.
 
 To install Transformers4Rec using Pip, run the following command:
 
 ```shell
-pip install transformers4rec[pytorch,nvtabular,dataloader]
+pip install transformers4rec[nvtabular]
 ```
 
-> Be aware that installing Transformers4Rec with `pip` only supports the CPU version of Merlin Dataloader because `pip` does not install cuDF.
-> The GPU capabilities of the dataloader are available by using the Docker container or by installing
-> the dataloader with Conda first and then performing the `pip` installation within the Conda environment.
+-> Be aware that installing Transformers4Rec with `pip` does not automatically install RAPIDS cuDF.
+-> cuDF is required for GPU-accelerated versions of NVTabular transforms and the Merlin Dataloader.
+
+Instructions for installing cuDF with pip are available here: https://docs.rapids.ai/install#pip-install
+
+```shell
+pip install cudf-cu11 dask-cudf-cu11 --extra-index-url=https://pypi.nvidia.com
+```
 
 ### Installing Transformers4Rec Using Conda
 
-To install Transformers4Rec using Conda, run the following command:
+To install Transformers4Rec using Conda, run the following command with `conda` or `mamba` to create a new environment.
 
 ```shell
-conda install -c nvidia transformers4rec
+mamba create -n transformers4rec-23.04 -c nvidia -c rapidsai -c pytorch -c conda-forge \
+    transformers4rec=23.04 `# NVIDIA Merlin` \
+    nvtabular=23.04 `# NVIDIA Merlin - Used in example notebooks` \
+    python=3.10 `# Compatible Python environment` \
+    cudf=23.02 `# RAPIDS cuDF - GPU accelerated DataFrame` \
+    cudatoolkit=11.8 pytorch-cuda=11.8 `# NVIDIA CUDA version`
 ```
 
 ### Installing Transformers4Rec Using Docker
 
 Transformers4Rec is pre-installed in the `merlin-pytorch` container that is available from the NVIDIA GPU Cloud (NGC) catalog.
 
 Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/main/containers.html) documentation page for information about the Merlin container names, URLs to container images in the catalog, and key Merlin components.
```

### Comparing `transformers4rec-23.4.0/README.md` & `transformers4rec-23.5.0/transformers4rec.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: transformers4rec
+Version: 23.5.0
+Summary: UNKNOWN
+Home-page: https://github.com/NVIDIA-Merlin/Transformers4Rec
+Author: NVIDIA Corporation
+License: Apache 2.0
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Scientific/Engineering
+Description-Content-Type: text/markdown
+Provides-Extra: base
+Provides-Extra: pytorch
+Provides-Extra: nvtabular
+Provides-Extra: docs
+Provides-Extra: dev
+Provides-Extra: all
+License-File: LICENSE
+
 # [Transformers4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/)
 
 [![PyPI](https://img.shields.io/pypi/v/Transformers4Rec?color=orange&label=version)](https://pypi.python.org/pypi/Transformers4Rec)
 [![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/Transformers4Rec)](https://github.com/NVIDIA-Merlin/Transformers4Rec/blob/main/LICENSE)
 [![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/Transformers4Rec/main/README.html)
 
 Transformers4Rec is a flexible and efficient library for sequential and session-based recommendation and can work with PyTorch.
@@ -80,14 +103,15 @@
 
 3. Construct a transformer-body and convert this into a model.
 
 The following code sample shows how to define and train an XLNet model with PyTorch for next-item prediction task:
 
 ```python
 from transformers4rec import torch as tr
+from transformers4rec.torch.ranking_metric import NDCGAt, RecallAt
 
 # Create a schema or read one from disk: tr.Schema().from_json(SCHEMA_PATH).
 schema: tr.Schema = tr.data.tabular_sequence_testing_data.schema
 
 max_sequence_length, d_model = 20, 64
 
 # Define the input module to process the tabular input features.
@@ -141,27 +165,37 @@
 You can install Transformers4Rec with the functionality to use the GPU-accelerated Merlin dataloader.
 Installation with the dataloader is highly recommended for better performance.
 Those components can be installed as optional arguments for the `pip install` command.
 
 To install Transformers4Rec using Pip, run the following command:
 
 ```shell
-pip install transformers4rec[pytorch,nvtabular,dataloader]
+pip install transformers4rec[nvtabular]
 ```
 
-> Be aware that installing Transformers4Rec with `pip` only supports the CPU version of Merlin Dataloader because `pip` does not install cuDF.
-> The GPU capabilities of the dataloader are available by using the Docker container or by installing
-> the dataloader with Conda first and then performing the `pip` installation within the Conda environment.
+-> Be aware that installing Transformers4Rec with `pip` does not automatically install RAPIDS cuDF.
+-> cuDF is required for GPU-accelerated versions of NVTabular transforms and the Merlin Dataloader.
+
+Instructions for installing cuDF with pip are available here: https://docs.rapids.ai/install#pip-install
+
+```shell
+pip install cudf-cu11 dask-cudf-cu11 --extra-index-url=https://pypi.nvidia.com
+```
 
 ### Installing Transformers4Rec Using Conda
 
-To install Transformers4Rec using Conda, run the following command:
+To install Transformers4Rec using Conda, run the following command with `conda` or `mamba` to create a new environment.
 
 ```shell
-conda install -c nvidia transformers4rec
+mamba create -n transformers4rec-23.04 -c nvidia -c rapidsai -c pytorch -c conda-forge \
+    transformers4rec=23.04 `# NVIDIA Merlin` \
+    nvtabular=23.04 `# NVIDIA Merlin - Used in example notebooks` \
+    python=3.10 `# Compatible Python environment` \
+    cudf=23.02 `# RAPIDS cuDF - GPU accelerated DataFrame` \
+    cudatoolkit=11.8 pytorch-cuda=11.8 `# NVIDIA CUDA version`
 ```
 
 ### Installing Transformers4Rec Using Docker
 
 Transformers4Rec is pre-installed in the `merlin-pytorch` container that is available from the NVIDIA GPU Cloud (NGC) catalog.
 
 Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/main/containers.html) documentation page for information about the Merlin container names, URLs to container images in the catalog, and key Merlin components.
@@ -180,7 +214,9 @@
 
 ## Feedback and Support
 
 If you'd like to make direct contributions to Transformers4Rec, refer to [Contributing to Transformers4Rec](CONTRIBUTING.md). We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations. To further advance our Merlin roadmap, we encourage you to share all the details regarding your recommender system pipeline by going to https://developer.nvidia.com/merlin-devzone-survey.
 
 If you're interested in learning more about how Transformers4Rec works, refer to our
 [Transformers4Rec documentation](https://nvidia-merlin.github.io/Transformers4Rec/main/getting_started.html). We also have [API documentation](https://nvidia-merlin.github.io/Transformers4Rec/main/api/modules.html) that outlines the specifics of the available modules and classes within Transformers4Rec.
+
+
```

### Comparing `transformers4rec-23.4.0/_images/DP_DDP_perf.png` & `transformers4rec-23.5.0/_images/DP_DDP_perf.png`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/_images/nlp_x_recsys.png` & `transformers4rec-23.5.0/_images/nlp_x_recsys.png`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/_images/pipeline.png` & `transformers4rec-23.5.0/_images/pipeline.png`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/_images/preproc_data_example.png` & `transformers4rec-23.5.0/_images/preproc_data_example.png`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/_images/sequential_rec.png` & `transformers4rec-23.5.0/_images/sequential_rec.png`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/_images/transformers4rec_metaarchitecture.png` & `transformers4rec-23.5.0/_images/transformers4rec_metaarchitecture.png`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/merlin_standard_lib/__init__.py` & `transformers4rec-23.5.0/merlin_standard_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/merlin_standard_lib/proto/__init__.py` & `transformers4rec-23.5.0/merlin_standard_lib/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/merlin_standard_lib/proto/schema_bp.py` & `transformers4rec-23.5.0/merlin_standard_lib/proto/schema_bp.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/merlin_standard_lib/schema/__init__.py` & `transformers4rec-23.5.0/merlin_standard_lib/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/merlin_standard_lib/schema/schema.py` & `transformers4rec-23.5.0/merlin_standard_lib/schema/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,30 +306,37 @@
             to_select = [to_select]
 
         if callable(to_select):
             return self._filter_column_schemas(to_select, lambda x: False, lambda x: x.tags)
         else:
             # Schema.tags always returns a List[str] with the tag values, so if the user wants to
             # filter using the Tags Enum, we need to convert those to their string value
-            to_select = [tag.value if isinstance(tag, Tags) else tag for tag in to_select]
+            if not isinstance(to_select, (list, tuple)):
+                to_select = [to_select]
+
+            to_select = TagSet(to_select)
 
             def collection_filter_fn(column_names: List[str]):
                 return all(x in column_names for x in to_select)
 
-            return self._filter_column_schemas(to_select, collection_filter_fn, lambda x: x.tags)
+            return self._filter_column_schemas(
+                list(to_select), collection_filter_fn, lambda x: TagSet(x.tags)
+            )
 
     def remove_by_tag(self, to_remove) -> "Schema":
         if not isinstance(to_remove, (list, tuple)) and not callable(to_remove):
             to_remove = [to_remove]
 
+        to_remove = TagSet(to_remove)
+
         def collection_filter_fn(column_tags):
             return all(x in column_tags for x in to_remove)
 
         return self._filter_column_schemas(
-            to_remove, collection_filter_fn, lambda x: x.tags, negate=True
+            list(to_remove), collection_filter_fn, lambda x: TagSet(x.tags), negate=True
         )
 
     def select_by_name(self, to_select) -> "Schema":
         if not isinstance(to_select, (list, tuple)) and not callable(to_select):
             to_select = [to_select]
 
         def collection_filter_fn(column_name):
```

### Comparing `transformers4rec-23.4.0/merlin_standard_lib/schema/tag.py` & `transformers4rec-23.5.0/merlin_standard_lib/schema/tag.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/merlin_standard_lib/utils/__init__.py` & `transformers4rec-23.5.0/merlin_standard_lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/merlin_standard_lib/utils/embedding_utils.py` & `transformers4rec-23.5.0/merlin_standard_lib/utils/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/mypy.ini` & `transformers4rec-23.5.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/setup.cfg` & `transformers4rec-23.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/setup.py` & `transformers4rec-23.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/__init__.py` & `transformers4rec-23.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/conftest.py` & `transformers4rec-23.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/integration/notebooks/test_getting_started_session_based.py` & `transformers4rec-23.5.0/tests/integration/notebooks/test_getting_started_session_based.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 
 @pytest.mark.notebook
 @pytest.mark.skipif(not HAS_GPU, reason="No GPU available")
 def test_func():
     with testbook(
         REPO_ROOT / "examples" / "getting-started-session-based" / "01-ETL-with-NVTabular.ipynb",
+        timeout=180,
         execute=False,
     ) as tb1:
         tb1.inject(
             """
             import os
             os.environ["INPUT_DATA_DIR"] = "/tmp/data/"
             os.environ["NUM_ROWS"] = "10000"
@@ -31,14 +32,15 @@
         assert os.path.isdir("/tmp/data/workflow_etl")
 
     with testbook(
         REPO_ROOT
         / "examples"
         / "getting-started-session-based"
         / "02-session-based-XLNet-with-PyT.ipynb",
+        timeout=180,
         execute=False,
     ) as tb2:
         tb2.inject(
             """
             import os
             os.environ["INPUT_DATA_DIR"] = "/tmp/data/"
             os.environ["INPUT_SCHEMA_PATH"] = "/tmp/data/processed_nvt/schema.pbtxt"
@@ -64,14 +66,15 @@
         assert os.path.isdir("/tmp/data/saved_model")
 
     with testbook(
         REPO_ROOT
         / "examples"
         / "getting-started-session-based"
         / "03-serving-session-based-model-torch-backend.ipynb",
+        timeout=720,
         execute=False,
     ) as tb3:
         tb3.inject(
             """
             import os
             os.environ["INPUT_DATA_DIR"] = "/tmp/data/"
             os.environ["OUTPUT_DIR"] = "/tmp/data/sessions_by_day"
```

### Comparing `transformers4rec-23.4.0/tests/integration/notebooks/test_notebooks.py` & `transformers4rec-23.5.0/tests/integration/notebooks/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/assets/data_schema/data.parquet` & `transformers4rec-23.5.0/tests/unit/assets/data_schema/data.parquet`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/assets/data_schema/data_schema.pbtxt` & `transformers4rec-23.5.0/tests/unit/assets/data_schema/data_schema.pbtxt`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/assets/data_schema/data_seq.parquet` & `transformers4rec-23.5.0/tests/unit/assets/data_schema/data_seq.parquet`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/assets/data_schema/data_seq_schema.pbtxt` & `transformers4rec-23.5.0/tests/unit/assets/data_schema/data_seq_schema.pbtxt`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/assets/schema.pbtxt` & `transformers4rec-23.5.0/tests/unit/assets/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/config/__init__.py` & `transformers4rec-23.5.0/tests/unit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/config/test_schema.py` & `transformers4rec-23.5.0/tests/unit/config/test_schema.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/config/test_trainer.py` & `transformers4rec-23.5.0/tests/unit/config/test_trainer.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/config/test_transformer.py` & `transformers4rec-23.5.0/tests/unit/config/test_transformer.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/data/test_synthetic.py` & `transformers4rec-23.5.0/tests/unit/data/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/data/testing/tabular_data/test_dataset.py` & `transformers4rec-23.5.0/tests/unit/data/testing/tabular_data/test_dataset.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/data/testing/test_dataset.py` & `transformers4rec-23.5.0/tests/unit/data/testing/test_dataset.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/merlin_standard_lib/__init__.py` & `transformers4rec-23.5.0/tests/unit/merlin_standard_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/merlin_standard_lib/schema/__init__.py` & `transformers4rec-23.5.0/tests/unit/merlin_standard_lib/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/merlin_standard_lib/schema/test_schema.py` & `transformers4rec-23.5.0/tests/unit/merlin_standard_lib/schema/test_schema.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/__init__.py` & `transformers4rec-23.5.0/tests/unit/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/_conftest.py` & `transformers4rec-23.5.0/tests/unit/torch/_conftest.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/block/__init__.py` & `transformers4rec-23.5.0/tests/unit/torch/block/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/block/test_base.py` & `transformers4rec-23.5.0/tests/unit/torch/block/test_base.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/block/test_mlp.py` & `transformers4rec-23.5.0/tests/unit/torch/block/test_mlp.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/block/test_transformer.py` & `transformers4rec-23.5.0/tests/unit/torch/block/test_transformer.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/features/__init__.py` & `transformers4rec-23.5.0/tests/unit/torch/features/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/features/test_continuous.py` & `transformers4rec-23.5.0/tests/unit/torch/features/test_continuous.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/features/test_embedding.py` & `transformers4rec-23.5.0/tests/unit/torch/features/test_embedding.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/features/test_sequential.py` & `transformers4rec-23.5.0/tests/unit/torch/features/test_sequential.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/features/test_tabular.py` & `transformers4rec-23.5.0/tests/unit/torch/features/test_tabular.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/model/__init__.py` & `transformers4rec-23.5.0/tests/unit/torch/model/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/model/test_head.py` & `transformers4rec-23.5.0/tests/unit/torch/model/test_head.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/model/test_model.py` & `transformers4rec-23.5.0/tests/unit/torch/model/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,19 +80,19 @@
     )
     model_output = model(inference_inputs)
 
     # if the model is traced with ragged inputs it can only be called with ragged inputs
     # if the model is traced with padded inputs it can only be called with padded inputs
     traced_model = torch.jit.trace(model, inference_inputs, strict=False)
     traced_model_output = traced_model(inference_inputs)
-    assert torch.equal(model_output, traced_model_output)
+    torch.testing.assert_close(model_output, traced_model_output)
 
     model_output = model(inference_inputs_2)
     traced_model_output = traced_model(inference_inputs_2)
-    assert torch.equal(model_output, traced_model_output)
+    torch.testing.assert_close(model_output, traced_model_output)
 
 
 @pytest.mark.parametrize("task", [tr.BinaryClassificationTask, tr.RegressionTask])
 def test_sequential_prediction_model(
     torch_yoochoose_tabular_transformer_features, torch_yoochoose_like, task
 ):
     inputs = torch_yoochoose_tabular_transformer_features
```

### Comparing `transformers4rec-23.4.0/tests/unit/torch/tabular/__init__.py` & `transformers4rec-23.5.0/tests/unit/torch/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/tabular/test_aggregation.py` & `transformers4rec-23.5.0/tests/unit/torch/tabular/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/tabular/test_tabular.py` & `transformers4rec-23.5.0/tests/unit/torch/tabular/test_tabular.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/tabular/test_transformations.py` & `transformers4rec-23.5.0/tests/unit/torch/tabular/test_transformations.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,25 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+import numpy as np
 import pytest
 import torch
 from merlin.schema import Tags
 
 import transformers4rec.torch as tr
 from merlin_standard_lib import schema
 
+np.random.seed(0)
+torch.manual_seed(0)
+
 
 @pytest.mark.parametrize("replacement_prob", [0.1, 0.3, 0.5, 0.7])
 def test_stochastic_swap_noise(replacement_prob):
     NUM_SEQS = 100
     SEQ_LENGTH = 80
     PAD_TOKEN = 0
```

### Comparing `transformers4rec-23.4.0/tests/unit/torch/test_dataloader_utils.py` & `transformers4rec-23.5.0/tests/unit/torch/test_dataloader_utils.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/test_experimental.py` & `transformers4rec-23.5.0/tests/unit/torch/test_experimental.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/test_losses.py` & `transformers4rec-23.5.0/tests/unit/torch/test_losses.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/test_masking.py` & `transformers4rec-23.5.0/tests/unit/torch/test_masking.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/test_public_api.py` & `transformers4rec-23.5.0/tests/unit/torch/test_public_api.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/test_ranking_metrics.py` & `transformers4rec-23.5.0/tests/unit/torch/test_ranking_metrics.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/test_readme.py` & `transformers4rec-23.5.0/tests/unit/torch/test_readme.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/test_torchscript.py` & `transformers4rec-23.5.0/tests/unit/torch/test_torchscript.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/test_trainer.py` & `transformers4rec-23.5.0/tests/unit/torch/test_trainer.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/utils/__init__.py` & `transformers4rec-23.5.0/tests/unit/torch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/utils/test_schema_utils.py` & `transformers4rec-23.5.0/tests/unit/torch/utils/test_schema_utils.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/torch/utils/test_torch_utils.py` & `transformers4rec-23.5.0/tests/unit/torch/utils/test_torch_utils.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/utils/__init__.py` & `transformers4rec-23.5.0/tests/unit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/utils/test_data_utils.py` & `transformers4rec-23.5.0/tests/unit/utils/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tests/unit/utils/test_padding.py` & `transformers4rec-23.5.0/tests/unit/utils/test_padding.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/tox.ini` & `transformers4rec-23.5.0/tox.ini`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/__init__.py` & `transformers4rec-23.5.0/transformers4rec/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/config/__init__.py` & `transformers4rec-23.5.0/transformers4rec/config/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/config/schema.py` & `transformers4rec-23.5.0/transformers4rec/config/schema.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/config/trainer.py` & `transformers4rec-23.5.0/transformers4rec/config/trainer.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/config/transformer.py` & `transformers4rec-23.5.0/transformers4rec/config/transformer.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/data/__init__.py` & `transformers4rec-23.5.0/transformers4rec/data/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/data/dataset.py` & `transformers4rec-23.5.0/transformers4rec/data/dataset.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/data/synthetic.py` & `transformers4rec-23.5.0/transformers4rec/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/data/testing/data.parquet` & `transformers4rec-23.5.0/transformers4rec/data/testing/data.parquet`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/data/testing/dataset.py` & `transformers4rec-23.5.0/transformers4rec/data/testing/dataset.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/data/testing/music_streaming/data.parquet` & `transformers4rec-23.5.0/transformers4rec/data/testing/music_streaming/data.parquet`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/data/testing/music_streaming/schema.json` & `transformers4rec-23.5.0/transformers4rec/data/testing/music_streaming/schema.json`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/data/testing/schema.json` & `transformers4rec-23.5.0/transformers4rec/data/testing/schema.json`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/data/testing/tabular_data/data.parquet` & `transformers4rec-23.5.0/transformers4rec/data/testing/tabular_data/data.parquet`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/data/testing/tabular_data/schema.json` & `transformers4rec-23.5.0/transformers4rec/data/testing/tabular_data/schema.json`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/data/yoochoose.py` & `transformers4rec-23.5.0/transformers4rec/data/yoochoose.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/__init__.py` & `transformers4rec-23.5.0/transformers4rec/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/block/__init__.py` & `transformers4rec-23.5.0/transformers4rec/torch/block/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/block/base.py` & `transformers4rec-23.5.0/transformers4rec/torch/block/base.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/block/mlp.py` & `transformers4rec-23.5.0/transformers4rec/torch/block/mlp.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/block/transformer.py` & `transformers4rec-23.5.0/transformers4rec/torch/block/transformer.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/experimental.py` & `transformers4rec-23.5.0/transformers4rec/torch/experimental.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/features/__init__.py` & `transformers4rec-23.5.0/transformers4rec/torch/features/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/features/base.py` & `transformers4rec-23.5.0/transformers4rec/torch/features/base.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/features/continuous.py` & `transformers4rec-23.5.0/transformers4rec/torch/features/continuous.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/features/embedding.py` & `transformers4rec-23.5.0/transformers4rec/torch/features/embedding.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/features/sequence.py` & `transformers4rec-23.5.0/transformers4rec/torch/features/sequence.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/features/tabular.py` & `transformers4rec-23.5.0/transformers4rec/torch/features/tabular.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/features/text.py` & `transformers4rec-23.5.0/transformers4rec/torch/features/text.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/losses.py` & `transformers4rec-23.5.0/transformers4rec/torch/losses.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/masking.py` & `transformers4rec-23.5.0/transformers4rec/torch/masking.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/model/__init__.py` & `transformers4rec-23.5.0/transformers4rec/torch/model/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/model/base.py` & `transformers4rec-23.5.0/transformers4rec/torch/model/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,18 +367,21 @@
     def forward(
         self,
         body_outputs: Union[torch.Tensor, TabularData],
         training: bool = False,
         testing: bool = False,
         targets: Union[torch.Tensor, TabularData] = None,
         call_body: bool = False,
+        top_k: Optional[int] = None,
         **kwargs,
     ) -> Union[torch.Tensor, TabularData]:
         outputs = {}
 
+        from transformers4rec.torch.model.prediction_task import NextItemPredictionTask
+
         if call_body:
             body_outputs = self.body(body_outputs, training=training, testing=testing, **kwargs)
 
         if training or testing:
             losses = []
             labels = {}
             predictions = {}
@@ -396,17 +399,28 @@
                 predictions[name] = task_output["predictions"]
                 losses.append(task_output["loss"] * self._task_weights[name])
             loss_tensor = torch.stack(losses)
             loss = getattr(loss_tensor, self.loss_reduction)()
             outputs = {"loss": loss, "labels": labels, "predictions": predictions}
         else:
             for name, task in self.prediction_task_dict.items():
-                outputs[name] = task(
-                    body_outputs, targets=targets, training=training, testing=testing, **kwargs
-                )
+                if isinstance(task, NextItemPredictionTask):
+                    outputs[name] = task(
+                        body_outputs,
+                        targets=targets,
+                        training=training,
+                        testing=testing,
+                        top_k=top_k,
+                        **kwargs,
+                    )
+
+                else:
+                    outputs[name] = task(
+                        body_outputs, targets=targets, training=training, testing=testing, **kwargs
+                    )
 
         return outputs
 
     def calculate_metrics(  # type: ignore
         self,
         predictions: Union[torch.Tensor, TabularData],
         targets: Union[torch.Tensor, TabularData],
@@ -479,31 +493,35 @@
         self,
         *head: Head,
         head_weights: Optional[List[float]] = None,
         head_reduction: str = "mean",
         optimizer: Type[torch.optim.Optimizer] = torch.optim.Adam,
         name: str = None,
         max_sequence_length: Optional[int] = None,
+        top_k: Optional[int] = None,
     ):
         """Model class that can aggregate one or multiple heads.
         Parameters
         ----------
         head: Head
             One or more heads of the model.
         head_weights: List[float], optional
             Weight-value to use for each head.
         head_reduction: str, optional
             How to reduce the losses into a single tensor when multiple heads are used.
         optimizer: Type[torch.optim.Optimizer]
             Optimizer-class to use during fitting
         name: str, optional
             Name of the model.
-        max_sequence_length : int, optional
+        max_sequence_length: int, optional
             The maximum sequence length supported by the model.
             Used to truncate sequence inputs longer than this value.
+        top_k: int, optional
+            The number of items to return at the inference step once the model is deployed.
+            Default is None, which will return all items.
         """
         if head_weights:
             if not isinstance(head_weights, list):
                 raise ValueError("`head_weights` must be a list")
             if not len(head_weights) == len(head):
                 raise ValueError(
                     "`head_weights` needs to have the same length " "as the number of heads"
@@ -513,14 +531,15 @@
 
         self.name = name
         self.heads = torch.nn.ModuleList(head)
         self.head_weights = head_weights or [1.0] * len(head)
         self.head_reduction = head_reduction
         self.optimizer = optimizer
         self.max_sequence_length = max_sequence_length
+        self.top_k = top_k
 
     def forward(self, inputs: TabularData, targets=None, training=False, testing=False, **kwargs):
         # Convert inputs to float32 which is the default type, expected by PyTorch
         for name, val in inputs.items():
             if torch.is_floating_point(val):
                 inputs[name] = val.to(torch.float32)
 
@@ -561,14 +580,15 @@
                 outputs.update(
                     head(
                         inputs,
                         call_body=True,
                         targets=targets,
                         training=training,
                         testing=testing,
+                        top_k=self.top_k,
                         **kwargs,
                     )
                 )
             if len(outputs) == 1:
                 return list(outputs.values())[0]
 
         return outputs
@@ -752,14 +772,16 @@
                 name, dtype=dtype, tags=tags, properties=properties, dims=dims
             )
             core_schema[name] = col_schema
         return core_schema
 
     @property
     def output_schema(self):
+        from merlin.schema import Tags
+
         from .prediction_task import BinaryClassificationTask, RegressionTask
 
         # if the model has one head with one task, the output is a tensor
         # if multiple heads and/or multiple prediction task, the output is a dictionary
         output_cols = []
         for head in self.heads:
             dims = None
@@ -777,16 +799,36 @@
                 ):
                     dims = (None,)
                 else:
                     dims = (None, task.target_dim)
                 properties = {
                     "int_domain": int_domain,
                 }
-                col_schema = ColumnSchema(name, dtype=np.float32, properties=properties, dims=dims)
-                output_cols.append(col_schema)
+                # in case one sets top_k at the inference step we return two outputs
+                if self.top_k:
+                    # be sure categ item-id dtype in model.input schema and output schema matches
+                    col_name = self.input_schema.select_by_tag(Tags.ITEM_ID).column_names[0]
+                    col_dtype = (
+                        self.input_schema.select_by_tag(Tags.ITEM_ID)
+                        .column_schemas[col_name]
+                        .dtype.name
+                    )
+                    col_schema_scores = ColumnSchema(
+                        "item_id_scores", dtype=np.float32, properties=properties, dims=dims
+                    )
+                    col_schema_ids = ColumnSchema(
+                        "item_ids", dtype=np.dtype(col_dtype), properties=properties, dims=dims
+                    )
+                    output_cols.append(col_schema_scores)
+                    output_cols.append(col_schema_ids)
+                else:
+                    col_schema = ColumnSchema(
+                        name, dtype=np.float32, properties=properties, dims=dims
+                    )
+                    output_cols.append(col_schema)
 
         return Core_Schema(output_cols)
 
     @property
     def prediction_tasks(self):
         return [task for head in self.heads for task in list(head.prediction_task_dict.values())]
```

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/model/prediction_task.py` & `transformers4rec-23.5.0/transformers4rec/torch/model/prediction_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,15 +277,15 @@
             if input_size[-1] != item_dim and not task_block:
                 LOG.warning(
                     f"Projecting inputs of NextItemPredictionTask to'{item_dim}' "
                     f"As weight tying requires the input dimension '{input_size[-1]}' "
                     f"to be equal to the item-id embedding dimension '{item_dim}'"
                 )
                 # project input tensors to same dimension as item-id embeddings
-                task_block = MLPBlock([item_dim])
+                task_block = MLPBlock([item_dim], activation=None)
 
         # Retrieve the masking from the input block
         self.masking = inputs.masking
         if not self.masking:
             raise ValueError(
                 "The input block should contain a masking schema for training and evaluation"
             )
@@ -299,15 +299,23 @@
             max_n_samples=self.max_n_samples,
             min_id=self.padding_idx + 1,
         )
         super().build(
             body, input_size, device=device, inputs=inputs, task_block=task_block, pre=pre
         )
 
-    def forward(self, inputs: torch.Tensor, targets=None, training=False, testing=False, **kwargs):
+    def forward(
+        self,
+        inputs: torch.Tensor,
+        targets=None,
+        training=False,
+        testing=False,
+        top_k=None,
+        **kwargs,
+    ):
         if isinstance(inputs, (tuple, list)):
             inputs = inputs[0]
         x = inputs.float()
 
         if self.task_block:
             x = self.task_block(x)  # type: ignore
 
@@ -338,15 +346,19 @@
             else:
                 last_item_sessions = non_pad_mask.sum(dim=1) - 1
             x = x[rows_ids, last_item_sessions]
 
             # Compute predictions probs
             x, _ = self.pre(x)  # type: ignore
 
-            return x
+            if top_k is None:
+                return x
+            else:
+                preds_sorted_item_scores, preds_sorted_item_ids = torch.topk(x, k=top_k, dim=-1)
+                return preds_sorted_item_scores, preds_sorted_item_ids
 
     def remove_pad_3d(self, inp_tensor, non_pad_mask):
         # inp_tensor: (n_batch x seqlen x emb_dim)
         inp_tensor = inp_tensor.flatten(end_dim=1)
         inp_tensor_fl = torch.masked_select(
             inp_tensor, non_pad_mask.unsqueeze(1).expand_as(inp_tensor)
         )
```

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/ranking_metric.py` & `transformers4rec-23.5.0/transformers4rec/torch/ranking_metric.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/tabular/__init__.py` & `transformers4rec-23.5.0/transformers4rec/torch/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/tabular/aggregation.py` & `transformers4rec-23.5.0/transformers4rec/torch/tabular/aggregation.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/tabular/base.py` & `transformers4rec-23.5.0/transformers4rec/torch/tabular/base.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/tabular/transformations.py` & `transformers4rec-23.5.0/transformers4rec/torch/tabular/transformations.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/trainer.py` & `transformers4rec-23.5.0/transformers4rec/torch/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -525,14 +525,20 @@
                 labels = self._nested_gather(labels)
                 labels_host = (
                     labels
                     if labels_host is None
                     else nested_concat(labels_host, labels, padding_index=0)
                 )
             if preds is not None and self.args.predict_top_k > 0:
+                if self.model.top_k:
+                    raise ValueError(
+                        "you cannot set top_k argument in the model class and the, "
+                        "predict_top_k  in the trainer at the same time. Please ensure setting "
+                        "only predict_top_k"
+                    )
                 # get outputs of next-item scores
                 if isinstance(preds, dict):
                     assert any(
                         isinstance(x, NextItemPredictionTask) for x in model.prediction_tasks
                     ), "Top-k prediction is specific to NextItemPredictionTask, "
                     "Please ensure `self.args.predict_top_k == 0` "
                     pred_next_item = preds["next-item"]
```

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/typing.py` & `transformers4rec-23.5.0/transformers4rec/torch/typing.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/utils/__init__.py` & `transformers4rec-23.5.0/transformers4rec/torch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/utils/data_utils.py` & `transformers4rec-23.5.0/transformers4rec/torch/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/utils/examples_utils.py` & `transformers4rec-23.5.0/transformers4rec/torch/utils/examples_utils.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/utils/padding.py` & `transformers4rec-23.5.0/transformers4rec/torch/utils/padding.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/utils/schema_utils.py` & `transformers4rec-23.5.0/transformers4rec/torch/utils/schema_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import random
 from typing import Any, Dict, Optional
 
+import numpy as np
 import torch
 from merlin.schema.io.proto_utils import has_field
 
 from merlin_standard_lib import Schema
 
 from ..typing import TabularData
 
@@ -28,17 +29,23 @@
 def random_data_from_schema(
     schema: Schema,
     num_rows: int,
     max_session_length: Optional[int] = None,
     min_session_length: int = 5,
     device=None,
     ragged=False,
+    seed=0,
 ) -> TabularData:
     data: Dict[str, Any] = {}
 
+    random.seed(seed)
+    np.random.seed(seed)
+    if seed:
+        torch.manual_seed(seed)
+
     for i in range(num_rows):
         session_length = None
         if max_session_length:
             session_length = random.randint(min_session_length, max_session_length)
 
         for feature in schema.feature:
             is_list_feature = has_field(feature, "value_count")
```

### Comparing `transformers4rec-23.4.0/transformers4rec/torch/utils/torch_utils.py` & `transformers4rec-23.5.0/transformers4rec/torch/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/types.py` & `transformers4rec-23.5.0/transformers4rec/types.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/utils/__init__.py` & `transformers4rec-23.5.0/transformers4rec/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/utils/data_utils.py` & `transformers4rec-23.5.0/transformers4rec/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec/utils/dependencies.py` & `transformers4rec-23.5.0/transformers4rec/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.4.0/transformers4rec.egg-info/PKG-INFO` & `transformers4rec-23.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: transformers4rec
-Version: 23.4.0
-Summary: UNKNOWN
-Home-page: https://github.com/NVIDIA-Merlin/Transformers4Rec
-Author: NVIDIA Corporation
-License: Apache 2.0
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Scientific/Engineering
-Description-Content-Type: text/markdown
-Provides-Extra: base
-Provides-Extra: pytorch
-Provides-Extra: nvtabular
-Provides-Extra: docs
-Provides-Extra: dev
-Provides-Extra: all
-License-File: LICENSE
-
 # [Transformers4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/)
 
 [![PyPI](https://img.shields.io/pypi/v/Transformers4Rec?color=orange&label=version)](https://pypi.python.org/pypi/Transformers4Rec)
 [![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/Transformers4Rec)](https://github.com/NVIDIA-Merlin/Transformers4Rec/blob/main/LICENSE)
 [![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/Transformers4Rec/main/README.html)
 
 Transformers4Rec is a flexible and efficient library for sequential and session-based recommendation and can work with PyTorch.
@@ -103,14 +80,15 @@
 
 3. Construct a transformer-body and convert this into a model.
 
 The following code sample shows how to define and train an XLNet model with PyTorch for next-item prediction task:
 
 ```python
 from transformers4rec import torch as tr
+from transformers4rec.torch.ranking_metric import NDCGAt, RecallAt
 
 # Create a schema or read one from disk: tr.Schema().from_json(SCHEMA_PATH).
 schema: tr.Schema = tr.data.tabular_sequence_testing_data.schema
 
 max_sequence_length, d_model = 20, 64
 
 # Define the input module to process the tabular input features.
@@ -164,27 +142,37 @@
 You can install Transformers4Rec with the functionality to use the GPU-accelerated Merlin dataloader.
 Installation with the dataloader is highly recommended for better performance.
 Those components can be installed as optional arguments for the `pip install` command.
 
 To install Transformers4Rec using Pip, run the following command:
 
 ```shell
-pip install transformers4rec[pytorch,nvtabular,dataloader]
+pip install transformers4rec[nvtabular]
 ```
 
-> Be aware that installing Transformers4Rec with `pip` only supports the CPU version of Merlin Dataloader because `pip` does not install cuDF.
-> The GPU capabilities of the dataloader are available by using the Docker container or by installing
-> the dataloader with Conda first and then performing the `pip` installation within the Conda environment.
+-> Be aware that installing Transformers4Rec with `pip` does not automatically install RAPIDS cuDF.
+-> cuDF is required for GPU-accelerated versions of NVTabular transforms and the Merlin Dataloader.
+
+Instructions for installing cuDF with pip are available here: https://docs.rapids.ai/install#pip-install
+
+```shell
+pip install cudf-cu11 dask-cudf-cu11 --extra-index-url=https://pypi.nvidia.com
+```
 
 ### Installing Transformers4Rec Using Conda
 
-To install Transformers4Rec using Conda, run the following command:
+To install Transformers4Rec using Conda, run the following command with `conda` or `mamba` to create a new environment.
 
 ```shell
-conda install -c nvidia transformers4rec
+mamba create -n transformers4rec-23.04 -c nvidia -c rapidsai -c pytorch -c conda-forge \
+    transformers4rec=23.04 `# NVIDIA Merlin` \
+    nvtabular=23.04 `# NVIDIA Merlin - Used in example notebooks` \
+    python=3.10 `# Compatible Python environment` \
+    cudf=23.02 `# RAPIDS cuDF - GPU accelerated DataFrame` \
+    cudatoolkit=11.8 pytorch-cuda=11.8 `# NVIDIA CUDA version`
 ```
 
 ### Installing Transformers4Rec Using Docker
 
 Transformers4Rec is pre-installed in the `merlin-pytorch` container that is available from the NVIDIA GPU Cloud (NGC) catalog.
 
 Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/main/containers.html) documentation page for information about the Merlin container names, URLs to container images in the catalog, and key Merlin components.
@@ -203,9 +191,7 @@
 
 ## Feedback and Support
 
 If you'd like to make direct contributions to Transformers4Rec, refer to [Contributing to Transformers4Rec](CONTRIBUTING.md). We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations. To further advance our Merlin roadmap, we encourage you to share all the details regarding your recommender system pipeline by going to https://developer.nvidia.com/merlin-devzone-survey.
 
 If you're interested in learning more about how Transformers4Rec works, refer to our
 [Transformers4Rec documentation](https://nvidia-merlin.github.io/Transformers4Rec/main/getting_started.html). We also have [API documentation](https://nvidia-merlin.github.io/Transformers4Rec/main/api/modules.html) that outlines the specifics of the available modules and classes within Transformers4Rec.
-
-
```

### Comparing `transformers4rec-23.4.0/transformers4rec.egg-info/SOURCES.txt` & `transformers4rec-23.5.0/transformers4rec.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 tests/unit/torch/test_experimental.py
 tests/unit/torch/test_losses.py
 tests/unit/torch/test_masking.py
 tests/unit/torch/test_public_api.py
 tests/unit/torch/test_ranking_metrics.py
 tests/unit/torch/test_readme.py
 tests/unit/torch/test_torchscript.py
+tests/unit/torch/test_torchscript_with_topk.py
 tests/unit/torch/test_trainer.py
 tests/unit/torch/block/__init__.py
 tests/unit/torch/block/test_base.py
 tests/unit/torch/block/test_mlp.py
 tests/unit/torch/block/test_transformer.py
 tests/unit/torch/features/__init__.py
 tests/unit/torch/features/test_continuous.py
```

### Comparing `transformers4rec-23.4.0/transformers4rec.egg-info/requires.txt` & `transformers4rec-23.5.0/transformers4rec.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-transformers<5,>=4.12
+transformers[torch]<5,>=4.12
 tqdm>=4.27
 pyarrow>=1.0
-merlin-models>=23.4.0
+torchmetrics>=0.10.0
+merlin-models>=0.11
 
 [all]
-transformers<5,>=4.12
+transformers[torch]<5,>=4.12
 tqdm>=4.27
 pyarrow>=1.0
-merlin-models>=23.4.0
+torchmetrics>=0.10.0
+merlin-models>=0.11
 torch>=1.0
 torchmetrics>=0.10.0
 nvtabular
 Sphinx<3.6
 sphinx_rtd_theme==1.0.0
 sphinx-multiversion@ git+https://github.com/mikemckiernan/sphinx-multiversion.git
 sphinxcontrib-copydirs@ git+https://github.com/mikemckiernan/sphinxcontrib-copydirs.git
@@ -22,18 +24,19 @@
 natsort==8.0.1
 myst-nb<0.14
 linkify-it-py<1.1
 check-manifest
 bandit
 
 [base]
-transformers<5,>=4.12
+transformers[torch]<5,>=4.12
 tqdm>=4.27
 pyarrow>=1.0
-merlin-models>=23.4.0
+torchmetrics>=0.10.0
+merlin-models>=0.11
 
 [dev]
 check-manifest
 bandit
 
 [docs]
 Sphinx<3.6
```

### Comparing `transformers4rec-23.4.0/versioneer.py` & `transformers4rec-23.5.0/versioneer.py`

 * *Files identical despite different names*

