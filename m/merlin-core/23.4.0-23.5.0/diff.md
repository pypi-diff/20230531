# Comparing `tmp/merlin-core-23.4.0.tar.gz` & `tmp/merlin-core-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merlin-core-23.4.0.tar", last modified: Wed Apr 26 16:36:00 2023, max compression
+gzip compressed data, was "merlin-core-23.5.0.tar", last modified: Wed May 31 14:39:07 2023, max compression
```

## Comparing `merlin-core-23.4.0.tar` & `merlin-core-23.5.0.tar`

### file list

```diff
@@ -1,97 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.535273 merlin-core-23.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 16:35:32.000000 merlin-core-23.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-26 16:35:32.000000 merlin-core-23.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-26 16:36:00.535273 merlin-core-23.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-26 16:35:32.000000 merlin-core-23.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.527273 merlin-core-23.4.0/merlin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.535273 merlin-core-23.4.0/merlin/core/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-26 16:36:00.535273 merlin-core-23.4.0/merlin/core/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.531273 merlin-core-23.4.0/merlin/core/compat/
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/core/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/core/compat/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/core/compat/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    25378 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/core/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/core/has_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/core/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.531273 merlin-core-23.4.0/merlin/dag/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/base_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/dictarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    15397 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    22848 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.531273 merlin-core-23.4.0/merlin/dag/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/ops/concat_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/ops/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/ops/subset_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/ops/subtraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dag/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.531273 merlin-core-23.4.0/merlin/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dispatch/lazy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.531273 merlin-core-23.4.0/merlin/dtypes/
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.531273 merlin-core-23.4.0/merlin/dtypes/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/mappings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/mappings/cudf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/mappings/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/mappings/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/mappings/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/mappings/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/mappings/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/mappings/triton.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/dtypes/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.535273 merlin-core-23.4.0/merlin/io/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/avro.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/dataframe_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/dataframe_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)    53986 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/dataset_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/fsspec_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/hugectr.py
--rw-r--r--   0 runner    (1001) docker     (123)    46920 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/io/writer_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.535273 merlin-core-23.4.0/merlin/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.535273 merlin-core-23.4.0/merlin/schema/io/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/schema/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/schema/io/proto_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36781 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/schema/io/schema_bp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/schema/io/tensorflow_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    21785 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/schema/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.535273 merlin-core-23.4.0/merlin/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/table/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/table/cupy_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/table/numpy_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/table/tensor_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/table/tensor_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/table/tensorflow_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-26 16:35:32.000000 merlin-core-23.4.0/merlin/table/torch_column.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:36:00.535273 merlin-core-23.4.0/merlin_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-26 16:36:00.000000 merlin-core-23.4.0/merlin_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-26 16:36:00.000000 merlin-core-23.4.0/merlin_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:36:00.000000 merlin-core-23.4.0/merlin_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:36:00.000000 merlin-core-23.4.0/merlin_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-26 16:36:00.000000 merlin-core-23.4.0/merlin_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 16:36:00.000000 merlin-core-23.4.0/merlin_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-26 16:35:32.000000 merlin-core-23.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-26 16:35:32.000000 merlin-core-23.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-26 16:35:32.000000 merlin-core-23.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-26 16:36:00.535273 merlin-core-23.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-26 16:35:32.000000 merlin-core-23.4.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81339 2023-04-26 16:35:32.000000 merlin-core-23.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.044466 merlin-core-23.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 14:39:00.000000 merlin-core-23.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-31 14:39:00.000000 merlin-core-23.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-31 14:39:07.044466 merlin-core-23.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-31 14:39:00.000000 merlin-core-23.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.032466 merlin-core-23.5.0/merlin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.044466 merlin-core-23.5.0/merlin/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-31 14:39:07.044466 merlin-core-23.5.0/merlin/core/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.036466 merlin-core-23.5.0/merlin/core/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/core/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/core/compat/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/core/compat/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25544 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/core/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/core/has_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/core/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.036466 merlin-core-23.5.0/merlin/dag/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/base_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21211 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22848 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.036466 merlin-core-23.5.0/merlin/dag/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/ops/concat_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/ops/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/ops/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/ops/subset_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/ops/subtraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.036466 merlin-core-23.5.0/merlin/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dispatch/lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.036466 merlin-core-23.5.0/merlin/dtypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.040466 merlin-core-23.5.0/merlin/dtypes/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mappings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mappings/cudf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mappings/merlin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mappings/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mappings/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mappings/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mappings/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mappings/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mappings/triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.040466 merlin-core-23.5.0/merlin/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/avro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/dataframe_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/dataframe_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54001 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/dataset_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/fsspec_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/hugectr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46920 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/writer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.040466 merlin-core-23.5.0/merlin/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.044466 merlin-core-23.5.0/merlin/schema/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/schema/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/schema/io/proto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36781 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/schema/io/schema_bp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/schema/io/tensorflow_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/schema/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.044466 merlin-core-23.5.0/merlin/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/table/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/table/cupy_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/table/numpy_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/table/tensor_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/table/tensor_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/table/tensorflow_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/table/torch_column.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.044466 merlin-core-23.5.0/merlin/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/testing/assert_equals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.044466 merlin-core-23.5.0/merlin_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-31 14:39:06.000000 merlin-core-23.5.0/merlin_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-31 14:39:06.000000 merlin-core-23.5.0/merlin_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:39:06.000000 merlin-core-23.5.0/merlin_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:39:06.000000 merlin-core-23.5.0/merlin_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-31 14:39:06.000000 merlin-core-23.5.0/merlin_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 14:39:06.000000 merlin-core-23.5.0/merlin_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-31 14:39:00.000000 merlin-core-23.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-31 14:39:00.000000 merlin-core-23.5.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-31 14:39:00.000000 merlin-core-23.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-31 14:39:07.044466 merlin-core-23.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-31 14:39:00.000000 merlin-core-23.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81339 2023-05-31 14:39:00.000000 merlin-core-23.5.0/versioneer.py
```

### Comparing `merlin-core-23.4.0/LICENSE` & `merlin-core-23.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/PKG-INFO` & `merlin-core-23.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-core
-Version: 23.4.0
+Version: 23.5.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/core
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -15,21 +15,21 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [Merlin Core](https://github.com/NVIDIA-Merlin/core)
 
 [![PyPI](https://img.shields.io/pypi/v/merlin-core?color=orange&label=version)](https://pypi.python.org/pypi/merlin-core/)
-[![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/core)](https://github.com/NVIDIA-Merlin/merlin-core/blob/main/LICENSE)
-[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/core/main/)
+[![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/core)](LICENSE)
+[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/core)
 
 The Merlin Core library provides the core utilities for [NVIDIA Merlin](https://github.com/NVIDIA-Merlin) libraries
 like [NVTabular](https://github.com/NVIDIA-Merlin/NVTabular), [Transformers4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec)
 and [Merlin Models](https://github.com/NVIDIA-Merlin/models).
-For example, the [merlin.io.Dataset](https://nvidia-merlin.github.io/core/main/api/merlin.io.html#merlin.io.Dataset) and [merin.schema.Schema](https://nvidia-merlin.github.io/core/main/api/merlin.schema.html#merlin.schema.Schema) classes are fundamental for working with data and building recommender systems with Merlin.
+For example, the [merlin.io.Dataset](https://nvidia-merlin.github.io/core/stable/api/merlin.io.html#merlin.io.Dataset) and [merin.schema.Schema](https://nvidia-merlin.github.io/core/stable/api/merlin.schema.html#merlin.schema.Schema) classes are fundamental for working with data and building recommender systems with Merlin.
 
 ## Installation
 
 ### Installing Merlin Core Using Pip
 
 ```shell
 pip install merlin-core
```

### Comparing `merlin-core-23.4.0/README.md` & `merlin-core-23.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # [Merlin Core](https://github.com/NVIDIA-Merlin/core)
 
 [![PyPI](https://img.shields.io/pypi/v/merlin-core?color=orange&label=version)](https://pypi.python.org/pypi/merlin-core/)
-[![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/core)](https://github.com/NVIDIA-Merlin/merlin-core/blob/main/LICENSE)
-[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/core/main/)
+[![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/core)](LICENSE)
+[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/core)
 
 The Merlin Core library provides the core utilities for [NVIDIA Merlin](https://github.com/NVIDIA-Merlin) libraries
 like [NVTabular](https://github.com/NVIDIA-Merlin/NVTabular), [Transformers4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec)
 and [Merlin Models](https://github.com/NVIDIA-Merlin/models).
-For example, the [merlin.io.Dataset](https://nvidia-merlin.github.io/core/main/api/merlin.io.html#merlin.io.Dataset) and [merin.schema.Schema](https://nvidia-merlin.github.io/core/main/api/merlin.schema.html#merlin.schema.Schema) classes are fundamental for working with data and building recommender systems with Merlin.
+For example, the [merlin.io.Dataset](https://nvidia-merlin.github.io/core/stable/api/merlin.io.html#merlin.io.Dataset) and [merin.schema.Schema](https://nvidia-merlin.github.io/core/stable/api/merlin.schema.html#merlin.schema.Schema) classes are fundamental for working with data and building recommender systems with Merlin.
 
 ## Installation
 
 ### Installing Merlin Core Using Pip
 
 ```shell
 pip install merlin-core
```

### Comparing `merlin-core-23.4.0/merlin/core/__init__.py` & `merlin-core-23.5.0/merlin/core/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/core/compat/__init__.py` & `merlin-core-23.5.0/merlin/core/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/core/compat/tensorflow.py` & `merlin-core-23.5.0/merlin/core/compat/tensorflow.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/core/compat/torch.py` & `merlin-core-23.5.0/merlin/core/compat/torch.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/core/dispatch.py` & `merlin-core-23.5.0/merlin/core/dispatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import enum
 import functools
 import itertools
-from typing import Callable, Union
+from typing import Callable, Optional, Union
 
 import dask.dataframe as dd
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 
@@ -307,35 +307,40 @@
     """Check if Series contains any null values"""
     if isinstance(s, pd.Series):
         return s.isnull().values.any()
     else:
         return s.has_nulls
 
 
-def list_val_dtype(ser: SeriesLike) -> np.dtype:
+def list_val_dtype(ser: SeriesLike) -> Optional[np.dtype]:
     """
     Return the dtype of the leaves from a list or nested list
 
     Parameters
     ----------
     ser : SeriesLike
         A series where the rows contain lists or nested lists
 
     Returns
     -------
-    np.dtype
-        The dtype of the innermost elements
+    Optional[np.dtype]
+        The dtype of the innermost elements if we find one
     """
     if is_list_dtype(ser):
         if cudf is not None and isinstance(ser, cudf.Series):
             if is_list_dtype(ser):
                 ser = ser.list.leaves
             return ser.dtype
         elif isinstance(ser, pd.Series):
-            return pd.core.dtypes.cast.infer_dtype_from(next(iter(pd.core.common.flatten(ser))))[0]
+            try:
+                return pd.core.dtypes.cast.infer_dtype_from(
+                    next(iter(pd.core.common.flatten(ser)))
+                )[0]
+            except StopIteration:
+                return None
     if isinstance(ser, np.ndarray):
         return ser.dtype
     # adds detection when in merlin column
     if hasattr(ser, "is_list"):
         return ser[0].dtype
     return None
```

### Comparing `merlin-core-23.4.0/merlin/core/has_gpu.py` & `merlin-core-23.5.0/merlin/core/has_gpu.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/core/protocols.py` & `merlin-core-23.5.0/merlin/core/protocols.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/core/utils.py` & `merlin-core-23.5.0/merlin/core/utils.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/dag/__init__.py` & `merlin-core-23.5.0/merlin/dag/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,13 +11,12 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 # flake8: noqa
-from merlin.dag.base_operator import BaseOperator, Supports
-from merlin.dag.dictarray import DictArray
+from merlin.dag.base_operator import BaseOperator, DataFormats, Supports
 from merlin.dag.graph import Graph
 from merlin.dag.node import Node, iter_nodes, postorder_iter_nodes, preorder_iter_nodes
 from merlin.dag.selector import ColumnSelector
 from merlin.dag.utils import group_values_offsets, ungroup_values_offsets
```

### Comparing `merlin-core-23.4.0/merlin/dag/base_operator.py` & `merlin-core-23.5.0/merlin/dag/base_operator.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,26 +21,43 @@
 import merlin.dag
 from merlin.core.protocols import Transformable
 from merlin.dag.selector import ColumnSelector
 from merlin.schema import ColumnSchema, Schema
 
 
 class Supports(Flag):
-    """Indicates what type of data representation this operator supports for transformations"""
+    """
+    Indicates what type of data representation this operator supports for transformations
+
+    (Deprecated)
+    """
 
     # cudf dataframe
     CPU_DATAFRAME = auto()
     # pandas dataframe
     GPU_DATAFRAME = auto()
     # dict of column name to numpy array
     CPU_DICT_ARRAY = auto()
     # dict of column name to cupy array
     GPU_DICT_ARRAY = auto()
 
 
+class DataFormats(Flag):
+    CUDF_DATAFRAME = auto()
+    PANDAS_DATAFRAME = auto()
+
+    NUMPY_TENSOR_TABLE = auto()
+    CUPY_TENSOR_TABLE = auto()
+    TF_TENSOR_TABLE = auto()
+    TORCH_TENSOR_TABLE = auto()
+
+    NUMPY_DICT_ARRAY = auto()
+    CUPY_DICT_ARRAY = auto()
+
+
 class BaseOperator:
     """
     Base class for all operator classes.
     """
 
     def compute_selector(
         self,
@@ -351,12 +368,21 @@
         return merlin.dag.Node(selector)
 
     @property
     def supports(self) -> Supports:
         """Returns what kind of data representation this operator supports"""
         return Supports.CPU_DATAFRAME | Supports.GPU_DATAFRAME
 
+    @property
+    def supported_formats(self) -> DataFormats:
+        return (
+            DataFormats.PANDAS_DATAFRAME
+            | DataFormats.CUDF_DATAFRAME
+            | DataFormats.NUMPY_TENSOR_TABLE
+            | DataFormats.CUPY_TENSOR_TABLE
+        )
+
     def _get_columns(self, df, selector):
         if isinstance(df, dict):
             return {col_name: df[col_name] for col_name in selector.names}
         else:
             return df[selector.names]
```

### Comparing `merlin-core-23.4.0/merlin/dag/graph.py` & `merlin-core-23.5.0/merlin/dag/graph.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/dag/node.py` & `merlin-core-23.5.0/merlin/dag/node.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/dag/ops/__init__.py` & `merlin-core-23.5.0/merlin/dag/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/dag/ops/concat_columns.py` & `merlin-core-23.5.0/merlin/dag/ops/concat_columns.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/dag/ops/selection.py` & `merlin-core-23.5.0/merlin/dag/ops/selection.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/dag/ops/subset_columns.py` & `merlin-core-23.5.0/merlin/dag/ops/subset_columns.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/dag/ops/subtraction.py` & `merlin-core-23.5.0/merlin/dag/ops/subtraction.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/dag/selector.py` & `merlin-core-23.5.0/merlin/dag/selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,19 @@
 
     def __init__(
         self,
         names: Union[str, List[str]] = None,
         subgroups: List["ColumnSelector"] = None,
         tags: List[Union[Tags, str]] = None,
     ):
+        self._all = False
         self._names = names if names is not None else []
         self._tags = tags if tags is not None else []
         self.subgroups = subgroups if subgroups is not None else []
 
-        self.all = isinstance(names, str) and names == "*"
         if self.all:
             self._names = []
             self._tags = []
             self.subgroups = []
 
         if isinstance(self._names, merlin.dag.Node):
             raise TypeError("ColumnSelectors can not contain Nodes")
@@ -74,14 +74,19 @@
                 self.subgroups.append(name)
             else:
                 self.subgroups.append(ColumnSelector(name))
         self._names = plain_names
         self._nested_check()
 
     @property
+    def all(self):
+        self._all = self._all or (isinstance(self._names, str) and self._names == "*")
+        return self._all
+
+    @property
     def tags(self):
         return list(dict.fromkeys(self._tags).keys())
 
     @property
     def names(self):
         names = []
         names += self._names
```

### Comparing `merlin-core-23.4.0/merlin/dag/utils.py` & `merlin-core-23.5.0/merlin/dag/utils.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/dispatch/lazy.py` & `merlin-core-23.5.0/merlin/dispatch/lazy.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/dtypes/__init__.py` & `merlin-core-23.5.0/merlin/dtypes/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 # flake8: noqa
-from merlin.dtypes import mappings
+from merlin.dtypes import aliases, mappings
 from merlin.dtypes.aliases import *
 from merlin.dtypes.base import DType
 from merlin.dtypes.registry import _dtype_registry
 from merlin.dtypes.shape import Dimension, Shape
 
 # Convenience alias for registering dtypes
 register = _dtype_registry.register
@@ -43,19 +43,30 @@
     # nothing for us to do and we can exit early
     if isinstance(external_dtype, DType):
         return external_dtype
 
     # If not, attempt to apply all the registered Merlin dtype mappings.
     # If we don't find a match with those, fall back on converting to
     # a numpy dtype and trying to match that instead.
+    base_exc = None
+    merlin_dtype = None
+
     try:
-        return _dtype_registry.to_merlin(external_dtype)
-    except TypeError as base_exc:
+        merlin_dtype = _dtype_registry.to_merlin(external_dtype)
+    except (TypeError, KeyError, AttributeError) as exc:
+        base_exc = exc
+
+    if base_exc or merlin_dtype == aliases.unknown:
         try:
-            return _dtype_registry.to_merlin_via_numpy(external_dtype)
-        except TypeError as exc:
+            merlin_dtype = _dtype_registry.to_merlin_via_numpy(external_dtype)
+        except TypeError as numpy_exc:
             # If we fail to find a match even after we try converting to
             # numpy, re-raise the original exception because it has more
             # information about the original external dtype that's causing
             # the problem. (We want to highlight that dtype, not whatever
             # numpy dtype it was converted to in the interim.)
-            raise base_exc from exc
+            if base_exc:
+                raise base_exc from numpy_exc
+            else:
+                raise numpy_exc
+
+    return merlin_dtype
```

### Comparing `merlin-core-23.4.0/merlin/dtypes/aliases.py` & `merlin-core-23.5.0/merlin/dtypes/aliases.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,8 +45,9 @@
 datetime64us = DType("datetime64[us]", ElementType.DateTime, 64, ElementUnit.Microsecond)
 datetime64ns = DType("datetime64[ns]", ElementType.DateTime, 64, ElementUnit.Nanosecond)
 
 # Miscellaneous
 string = DType("str", ElementType.String)
 boolean = DType("bool", ElementType.Bool)
 object_ = DType("object", ElementType.Object)
+struct = DType("struct", ElementType.Struct)
 unknown = DType("unknown", ElementType.Unknown)
```

### Comparing `merlin-core-23.4.0/merlin/dtypes/base.py` & `merlin-core-23.5.0/merlin/dtypes/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     Int = "int"
     UInt = "uint"
     Float = "float"
     String = "string"
     DateTime = "datetime"
     Object = "object"
     Unknown = "unknown"
+    Struct = "struct"
 
 
 class ElementUnit(Enum):
     """
     Dtype units, used only for datetime types
 
     Since a Merlin DType may describe a list, these are the either the units of
```

### Comparing `merlin-core-23.4.0/merlin/dtypes/mapping.py` & `merlin-core-23.5.0/merlin/dtypes/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,19 @@
             An external framework dtype
 
         Returns
         -------
         DType
             A Merlin DType object
         """
-        merlin_dtype = self.to_merlin_[external_dtype]
+        try:
+            merlin_dtype = self.to_merlin_[external_dtype]
+        except KeyError:
+            merlin_dtype = self.to_merlin_[type(external_dtype)]
+
         return merlin_dtype
 
     def from_merlin(self, merlin_dtype):
         """
         Translate a Merlin dtype to an external dtype
 
         Parameters
@@ -164,10 +168,10 @@
         if base_class and not isinstance(dtype, base_class):
             return False
 
         # Some external dtype objects are not hashable, so they
         # can't be used as dictionary keys. In that case, match
         # against the dtype class instead.
         try:
-            return dtype in mapping.keys()
+            return dtype in mapping.keys() or type(dtype) in mapping.keys()
         except TypeError:
             return type(dtype) in mapping.keys()
```

### Comparing `merlin-core-23.4.0/merlin/dtypes/mappings/__init__.py` & `merlin-core-23.5.0/merlin/dtypes/mappings/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 # flake8: noqa
-from merlin.dtypes.mappings import cudf, numpy, pandas, python, tf, torch, triton
+from merlin.dtypes.mappings import cudf, merlin, numpy, pandas, python, tf, torch, triton
```

### Comparing `merlin-core-23.4.0/merlin/dtypes/mappings/cudf.py` & `merlin-core-23.5.0/merlin/dtypes/mappings/cudf.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import numpy as np
 
+import merlin.dtypes.aliases as mn
 from merlin.core.compat import cudf
 from merlin.core.dispatch import is_string_dtype
 from merlin.dtypes.mapping import DTypeMapping, NumpyPreprocessor
 from merlin.dtypes.registry import _dtype_registry
 
 
 def cudf_translator(raw_dtype) -> np.dtype:
@@ -44,14 +45,17 @@
 
 if cudf:
     try:
         # We only want to register this mapping if cudf is available, even though
         # the mapping itself doesn't use cudf (yet?)
 
         cudf_dtypes = DTypeMapping(
+            {
+                mn.struct: [cudf.StructDtype],
+            },
             translator=NumpyPreprocessor("cudf", cudf_translator, attrs=["_categories"]),
         )
         _dtype_registry.register("cudf", cudf_dtypes)
     except ImportError as exc:
         from warnings import warn
 
         warn(f"cuDF dtype mappings did not load successfully due to an error: {exc.msg}")
```

### Comparing `merlin-core-23.4.0/merlin/dtypes/mappings/numpy.py` & `merlin-core-23.5.0/merlin/dtypes/mappings/numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,12 +41,12 @@
     mn.datetime64h: [np.dtype("datetime64[h]")],
     mn.datetime64m: [np.dtype("datetime64[m]")],
     mn.datetime64s: [np.dtype("datetime64[s]")],
     mn.datetime64ms: [np.dtype("datetime64[ms]")],
     mn.datetime64us: [np.dtype("datetime64[us]")],
     mn.datetime64ns: [np.dtype("datetime64[ns]")],
     # Miscellaneous
-    mn.string: [np.dtype("str"), np.str],
-    mn.object_: [np.dtype("O"), np.object],
-    mn.boolean: [np.dtype("bool"), np.bool],
+    mn.string: [np.dtype("str"), str],
+    mn.object_: [np.dtype("O"), object],
+    mn.boolean: [np.dtype("bool"), bool],
 }
 _dtype_registry.register("numpy", numpy_dtypes)
```

### Comparing `merlin-core-23.4.0/merlin/dtypes/mappings/python.py` & `merlin-core-23.5.0/merlin/dtypes/mappings/python.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,23 +9,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-import numpy as np
-
 import merlin.dtypes.aliases as mn
-from merlin.dtypes.mapping import DTypeMapping, NumpyPreprocessor
+from merlin.dtypes.mapping import DTypeMapping
 from merlin.dtypes.registry import _dtype_registry
 
 python_dtypes = DTypeMapping(
     {
         mn.boolean: bool,
         mn.int64: int,
         mn.float64: float,
         mn.string: str,
-    },
-    translator=NumpyPreprocessor("python", np.dtype, classes=[str]),
+    }
 )
 _dtype_registry.register("python", python_dtypes)
```

### Comparing `merlin-core-23.4.0/merlin/dtypes/mappings/tf.py` & `merlin-core-23.5.0/merlin/dtypes/mappings/tf.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/dtypes/mappings/torch.py` & `merlin-core-23.5.0/merlin/dtypes/mappings/torch.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/dtypes/mappings/triton.py` & `merlin-core-23.5.0/merlin/dtypes/mappings/triton.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/dtypes/registry.py` & `merlin-core-23.5.0/merlin/dtypes/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from typing import Dict, Union
 
+import merlin.dtypes.aliases as mn
 from merlin.dtypes.mapping import DTypeMapping
 
 
 class DTypeMappingRegistry:
     """
     A registry of mappings between Merlin dtypes and the dtypes of many external frameworks
     """
@@ -66,18 +67,15 @@
         TypeError
             If the Merlin dtype can't be mapped to an external dtype from the requested framework
         """
         mapping = self.mappings[mapping_name]
         if mapping.matches_merlin(merlin_dtype):
             return mapping.to_merlin(merlin_dtype)
 
-        raise TypeError(
-            f"Merlin doesn't provide a mapping from {merlin_dtype} to a {mapping_name} dtype. "
-            "If you'd like to provide one, you can use `merlin.dtype.register()`."
-        )
+        return mn.unknown
 
     def to_merlin(self, external_dtype):
         """
         Map an external dtype to a Merlin dtype
 
         Parameters
         ----------
@@ -94,19 +92,15 @@
         TypeError
             If the external dtype can't be mapped to a Merlin dtype
         """
         for framework, mapping in self.mappings.items():
             if mapping.matches_external(external_dtype):
                 return mapping.to_merlin(external_dtype)
 
-        raise TypeError(
-            f"Merlin doesn't provide a mapping from {external_dtype} ({type(external_dtype)}) "
-            "to a Merlin dtype. If you'd like to provide one, you can use "
-            "`merlin.dtype.register()`."
-        )
+        return mn.unknown
 
     def to_merlin_via_numpy(self, external_dtype):
         """
         Map an external dtype to a Merlin dtype by converting the external type to Numpy first
 
         This is sometimes useful for external framework dtypes that don't have a clear
         one-to-one mapping with a Merlin dtype, like cuDF's CategoricalDtype. We can often do
```

### Comparing `merlin-core-23.4.0/merlin/dtypes/shape.py` & `merlin-core-23.5.0/merlin/dtypes/shape.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/io/__init__.py` & `merlin-core-23.5.0/merlin/io/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/io/avro.py` & `merlin-core-23.5.0/merlin/io/avro.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/io/csv.py` & `merlin-core-23.5.0/merlin/io/csv.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/io/dask.py` & `merlin-core-23.5.0/merlin/io/dask.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/io/dataframe_engine.py` & `merlin-core-23.5.0/merlin/io/dataframe_engine.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/io/dataframe_iter.py` & `merlin-core-23.5.0/merlin/io/dataframe_iter.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/io/dataset.py` & `merlin-core-23.5.0/merlin/io/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1208,21 +1208,20 @@
             _real_meta = self.engine.sample_data(n=n)
             if self.dtypes:
                 _real_meta = _set_dtypes(_real_meta, self.dtypes)
             self._real_meta[n] = _real_meta
 
         if annotate_lists:
             _real_meta = self._real_meta[n]
-            annotated = {
-                col: {
-                    "dtype": list_val_dtype(_real_meta[col]) or _real_meta[col].dtype,
-                    "is_list": is_list_dtype(_real_meta[col]),
-                }
-                for col in _real_meta.columns
-            }
+            annotated = {}
+            for col in _real_meta.columns:
+                is_list = is_list_dtype(_real_meta[col])
+                dtype = list_val_dtype(_real_meta[col]) if is_list else _real_meta[col].dtype
+                annotated[col] = {"dtype": dtype, "is_list": is_list}
+
             return annotated
 
         return self._real_meta[n].dtypes
 
     @classmethod
     def _bind_dd_method(cls, name):
         """Bind Dask-Dataframe method to the Dataset class"""
```

### Comparing `merlin-core-23.4.0/merlin/io/dataset_engine.py` & `merlin-core-23.5.0/merlin/io/dataset_engine.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/io/fsspec_utils.py` & `merlin-core-23.5.0/merlin/io/fsspec_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/io/hugectr.py` & `merlin-core-23.5.0/merlin/io/hugectr.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/io/parquet.py` & `merlin-core-23.5.0/merlin/io/parquet.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/io/shuffle.py` & `merlin-core-23.5.0/merlin/io/shuffle.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/io/worker.py` & `merlin-core-23.5.0/merlin/io/worker.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/io/writer.py` & `merlin-core-23.5.0/merlin/io/writer.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/io/writer_factory.py` & `merlin-core-23.5.0/merlin/io/writer_factory.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/schema/__init__.py` & `merlin-core-23.5.0/merlin/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/schema/io/__init__.py` & `merlin-core-23.5.0/merlin/schema/io/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/schema/io/proto_utils.py` & `merlin-core-23.5.0/merlin/schema/io/proto_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/schema/io/schema_bp.py` & `merlin-core-23.5.0/merlin/schema/io/schema_bp.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/schema/io/tensorflow_metadata.py` & `merlin-core-23.5.0/merlin/schema/io/tensorflow_metadata.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/schema/schema.py` & `merlin-core-23.5.0/merlin/schema/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -452,39 +452,59 @@
         pred_fn = pred_fn or any
 
         if not isinstance(tags, (list, tuple)):
             tags = [tags]
 
         selected_schemas = {}
 
-        normalized_tags = [
-            Tags._value2member_map_.get(tag.lower(), tag) if isinstance(tag, str) else tag
-            for tag in tags
-        ]
+        normalized_tags = TagSet(tags)
+        if len(tags) == 1 and len(normalized_tags) > 1:
+            pred_fn = all
 
         for _, column_schema in self.column_schemas.items():
             if pred_fn(x in column_schema.tags for x in normalized_tags):
                 selected_schemas[column_schema.name] = column_schema
 
         return Schema(selected_schemas)
 
-    def excluding_by_tag(self, tags) -> "Schema":
+    def excluding_by_tag(self, tags, pred_fn=None) -> "Schema":
+        """Remove columns from the schema that match ANY of the supplied tags.
+
+        Parameters
+        ----------
+        tags : _type_
+            List of tags that describes which columns remove
+        pred_fn : `any` or `all`, optional, by default None (ANY)
+            Predicate function that decides if a column should be selected.
+            `all` can be provided to remove columns that contain ALL the tags provided
+
+        Returns
+        -------
+        Schema
+            New Schema containing only the columns that don't contain the provided tags
+        """
+        pred_fn = pred_fn or any
+
         if not isinstance(tags, (list, tuple)):
             tags = [tags]
 
         selected_schemas = {}
 
+        normalized_tags = TagSet(tags)
+        if len(tags) == 1 and len(normalized_tags) > 1:
+            pred_fn = all
+
         for column_schema in self.column_schemas.values():
-            if not any(x in column_schema.tags for x in tags):
+            if not pred_fn(x in column_schema.tags for x in normalized_tags):
                 selected_schemas[column_schema.name] = column_schema
 
         return Schema(selected_schemas)
 
-    def remove_by_tag(self, tags) -> "Schema":
-        return self.excluding_by_tag(tags)
+    def remove_by_tag(self, tags, pred_fn=None) -> "Schema":
+        return self.excluding_by_tag(tags, pred_fn=pred_fn)
 
     def select_by_name(self, names: List[str]) -> "Schema":
         """Select matching columns from this Schema object using a list of column names
 
         Parameters
         ----------
         names: List[str] :
```

### Comparing `merlin-core-23.4.0/merlin/schema/tags.py` & `merlin-core-23.5.0/merlin/schema/tags.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-import warnings
 from enum import Enum
 from typing import List, Set, Union
 
 
 class Tags(Enum):
     """Standard tags used in the Merlin ecosystem"""
 
@@ -52,16 +51,18 @@
     SESSION_ID = "session_id"
     TEXT_TOKENIZED = "text_tokenized"
     BINARY_CLASSIFICATION = "binary_classification"
     MULTI_CLASS_CLASSIFICATION = "multi_class_classification"
 
 
 TAG_COLLISIONS = {
-    Tags.CATEGORICAL: [Tags.CONTINUOUS],
-    Tags.CONTINUOUS: [Tags.CATEGORICAL],
+    Tags.CATEGORICAL: [Tags.CONTINUOUS, Tags.EMBEDDING],
+    Tags.CONTINUOUS: [Tags.CATEGORICAL, Tags.EMBEDDING, Tags.ID],
+    Tags.EMBEDDING: [Tags.CONTINUOUS, Tags.CATEGORICAL, Tags.ID],
+    Tags.ID: [Tags.CONTINUOUS, Tags.EMBEDDING],
 }
 
 COMPOUND_TAGS = {
     Tags.USER_ID: [Tags.USER, Tags.ID],
     Tags.ITEM_ID: [Tags.ITEM, Tags.ID],
     Tags.SESSION_ID: [Tags.SESSION, Tags.ID],
     Tags.TEXT_TOKENIZED: [Tags.TEXT, Tags.TOKENIZED],
@@ -73,15 +74,15 @@
 
     def __init__(self, tags: List[Union[str, Tags]] = None):
         if isinstance(tags, TagSet):
             tags = list(tags._tags)
         elif tags is None:
             tags = []
 
-        self._tags: Set[Tags] = self._normalize_tags(tags)
+        self._tags: Set[Union[str, Tags]] = self._normalize_tags(tags)
 
         collisions = self._detect_collisions(self._tags, self._tags)
         if collisions:
             raise ValueError(
                 f"Could not create a TagSet with the tags {self._tags}. "
                 f"The following tags are incompatible: {collisions}"
             )
@@ -135,27 +136,28 @@
         if not isinstance(tags, (list, set, TagSet)):
             tags = [tags]
         if not isinstance(tags, TagSet):
             tags = TagSet(tags)
 
         return tags
 
-    def _normalize_tags(self, tags) -> Set[Tags]:
-        tag_set = set(Tags[tag.upper()] if tag in Tags._value2member_map_ else tag for tag in tags)
-        atomized_tags = set()
+    def _normalize_tags(self, tags: List[Union[str, Tags]]) -> Set[Union[Tags, str]]:
+        tag_set: Set[Union[Tags, str]] = set()
+        for tag in tags:
+            if isinstance(tag, str) and tag.lower() in Tags._value2member_map_:
+                tag_set.add(Tags[tag.upper()])
+            else:
+                tag_set.add(tag)
 
+        atomized_tags: Set[Union[Tags, str]] = set()
         for tag in tag_set:
-            atomized_tags.add(tag)
-            if tag in COMPOUND_TAGS:
-                warnings.warn(
-                    f"Compound tags like {tag} have been deprecated "
-                    "and will be removed in a future version. "
-                    f"Please use the atomic versions of these tags, like {COMPOUND_TAGS[tag]}."
-                )
+            if isinstance(tag, Tags) and tag in COMPOUND_TAGS:
                 atomized_tags.update(COMPOUND_TAGS[tag])
+            else:
+                atomized_tags.add(tag)
 
         return atomized_tags
 
     def __repr__(self) -> str:
         return str(self._tags)
```

### Comparing `merlin-core-23.4.0/merlin/table/__init__.py` & `merlin-core-23.5.0/merlin/table/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/table/conversions.py` & `merlin-core-23.5.0/merlin/table/conversions.py`

 * *Files 11% similar despite different names*

```diff
@@ -161,48 +161,66 @@
     df_dict = {}
     for col_name, col_data in table.items():
         if col_data.offsets is not None:
             values = make_series(col_data.values, device=device)
             offsets = make_series(col_data.offsets, device=device)
             df_dict[col_name] = create_multihot_col(offsets, values)
         else:
-            df_dict[col_name] = make_series(col_data.values, device=device)
+            values = col_data.values
+            if len(values.shape) > 1:
+                values = values.tolist()
+            df_dict[col_name] = make_series(values, device=device)
 
     return make_df(df_dict, device=device)
 
 
 tensor_table_from_df = lazy_singledispatch("tensor_table_from_df")
 
 
 @tensor_table_from_df.register_lazy("pandas")
 def _register_tensor_table_from_pandas_df():
     import pandas as pd
 
     from merlin.table import NumpyColumn
 
     @tensor_table_from_df.register(pd.DataFrame)
-    def _tensor_table_from_pandas_df(df: pd.DataFrame):
-        return _create_table_from_df(df, NumpyColumn, device="cpu")
+    def _tensor_table_from_pandas_df(df: pd.DataFrame, schema=None):
+        return _create_table_from_df(df, NumpyColumn, device="cpu", schema=schema)
 
 
 @tensor_table_from_df.register_lazy("cudf")
 def _register_tensor_table_from_cudf_df():
     from merlin.core.compat import cudf
     from merlin.table import CupyColumn
 
     @tensor_table_from_df.register(cudf.DataFrame)
-    def _tensor_table_from_cudf_df(df: cudf.DataFrame):
-        return _create_table_from_df(df, CupyColumn)
+    def _tensor_table_from_cudf_df(df: cudf.DataFrame, schema=None):
+        return _create_table_from_df(df, CupyColumn, schema=schema)
 
 
-def _create_table_from_df(df, column_type, device=None):
+def _create_table_from_df(df, column_type, device=None, schema=None):
     from merlin.table import TensorTable
 
     array_cols = {}
     for col in df.columns:
         if is_list_dtype(df[col]):
             values_series, offsets_series = pull_apart_list(df[col], device=device)
-            array_cols[col] = column_type(values_series.values, offsets_series.values)
+            values = values_series.values
+            offsets = offsets_series.values
+            if schema and not schema[col].is_ragged:
+                row_lengths = offsets[1:] - offsets[:-1]
+                if not all(row_lengths == row_lengths[0]):
+                    raise ValueError(
+                        f"ColumnSchema for list column '{col}' describes a fixed size list. "
+                        "Found a ragged list output. If this dataframe contains a ragged list, "
+                        "Please check the 'schema' has a column shape defined to reflect this. "
+                    )
+                values_list = values.reshape(
+                    (len(row_lengths), int(row_lengths[0])) + values.shape[1:]
+                )
+                array_cols[col] = column_type(values_list)
+            else:
+                array_cols[col] = column_type(values_series.values, offsets_series.values)
         else:
             array_cols[col] = column_type(df[col].values)
 
     return TensorTable(array_cols)
```

### Comparing `merlin-core-23.4.0/merlin/table/cupy_column.py` & `merlin-core-23.5.0/merlin/table/cupy_column.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,32 +9,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import Callable, Type
+from typing import Callable, Optional, Type
 
 from merlin.core.compat import cupy as cp
 from merlin.table.conversions import _from_dlpack_gpu, _to_dlpack
 from merlin.table.tensor_column import Device, TensorColumn
 
 
 class CupyColumn(TensorColumn):
     """
     A SeriesLike column backed by CuPy arrays
     """
 
     @classmethod
-    def array_type(cls) -> Type:
+    def array_type(cls) -> Optional[Type]:
         """
         The type of the arrays backing this column
         """
-        return cp.ndarray
+        return cp.ndarray if cp else None
 
     @classmethod
     def array_constructor(cls) -> Callable:
         return cp.asarray
 
     @classmethod
     def supported_devices(cls):
```

### Comparing `merlin-core-23.4.0/merlin/table/numpy_column.py` & `merlin-core-23.5.0/merlin/table/numpy_column.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/table/tensor_column.py` & `merlin-core-23.5.0/merlin/table/tensor_column.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/merlin/table/tensor_table.py` & `merlin-core-23.5.0/merlin/table/tensor_table.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import Any, Dict
+from typing import Any, Dict, List, Type, Union
 
 from merlin.dag.utils import group_values_offsets
-from merlin.table.conversions import df_from_tensor_table, tensor_table_from_df
+from merlin.table.conversions import convert_col, df_from_tensor_table, tensor_table_from_df
 from merlin.table.cupy_column import CupyColumn
 from merlin.table.numpy_column import NumpyColumn
 from merlin.table.tensor_column import TensorColumn, create_tensor_column
 from merlin.table.tensorflow_column import TensorflowColumn
 from merlin.table.torch_column import TorchColumn
 
 TensorDict = Dict[str, Any]
@@ -29,25 +29,89 @@
 
 class TensorTable:
     """
     A DataFrameLike wrapper around a dictionary of arrays or tensors
     """
 
     @classmethod
-    def from_df(cls, df):
-        return tensor_table_from_df(df)
+    def from_df(cls, df, schema=None):
+        return tensor_table_from_df(df, schema=schema)
 
     def __init__(self, columns: TensorDict = None, _unsafe=False):
         cols_dict = self._convert_arrays_to_columns(columns, _unsafe=_unsafe)
 
         if not _unsafe:
             self._validate_columns(cols_dict)
 
         self._columns = cols_dict
 
+    def as_tensor_type(self, tensor_type: Union[Type, TensorColumn]) -> "TensorTable":
+        """Returns new TensorTable with columns cast to tensors of target framework.
+
+        Parameters
+        ----------
+        tensor_type : Union[Type, TensorColumn]
+            Tensor type or TensorColumn to convert to
+
+        Returns
+        -------
+        TensorTable
+            A new TensorTable with columns cast to framework tensors
+
+        Raises
+        ------
+        ValueError
+            If tensor type provided does not match supported types
+        """
+        framework_columns = {}
+        supported_columns = [NumpyColumn, CupyColumn, TorchColumn, TensorflowColumn]
+        for _column in supported_columns:
+            column_tensor_type = _column.array_type()
+            if column_tensor_type:
+                framework_columns[column_tensor_type] = _column
+
+        enabled_tensor_types = ", ".join(
+            f"'{_class.__module__}.{_class.__name__}'" for _class in framework_columns
+        )
+        enabled_column_types = ", ".join(
+            f"'merlin.table.{_class.__name__}'" for _class in framework_columns.values()
+        )
+
+        if not isinstance(tensor_type, type):
+            raise ValueError(
+                f"tensor_type argument must be a type. Received: {type(tensor_type)} \n"
+                f"Supported values are: {enabled_tensor_types}. \n"
+                f"Or TensorColumn Types: {enabled_column_types}"
+            )
+
+        if issubclass(tensor_type, TensorColumn):
+            target_col_type = tensor_type
+        else:
+            try:
+                target_col_type = framework_columns[tensor_type]
+            except KeyError as exc:
+                raise ValueError(
+                    f"Unsupported tensor type '{tensor_type}'. \n"
+                    f"Supported values are: {enabled_tensor_types}. \n"
+                    f"Or TensorColumn Types: {enabled_column_types}"
+                ) from exc
+
+        # if the current table already contains columns of the target type
+        # no conversion required
+        if self.column_type == target_col_type:
+            return self
+
+        # construct new table with columns cast to target framework type
+        columns = {}
+        for column_name in self.columns:
+            columns[column_name] = convert_col(self[column_name], target_col_type)
+        table = TensorTable(columns)
+
+        return table
+
     def _convert_arrays_to_columns(self, columns, _unsafe=False):
         grouped_columns = group_values_offsets(columns or {})
         cols_dict = {}
         for name, column in grouped_columns.items():
             if isinstance(column, TensorColumn):
                 cols_dict[name] = column
             elif isinstance(column, tuple):
@@ -133,22 +197,29 @@
         Create a copy of the Tensor Table, the column dictionary
 
         Exists for compatibility with the DictionaryLike protocol
         """
         return TensorTable(self._columns.copy())
 
     @property
-    def columns(self):
+    def columns(self) -> List[str]:
         """
         Return the names of the columns
 
         Exists for compatibility with the DataFrameLike protocol
         """
         return list(self.keys())
 
+    @columns.setter
+    def columns(self, col_names):
+        renamed_columns = {}
+        for col, col_name in zip(self.columns, col_names):
+            renamed_columns[col_name] = self._columns[col]
+        self._columns = renamed_columns
+
     @property
     def column_type(self):
         return type(list(self.values())[0])
 
     def dtypes(self):
         """
         Returns a list of the dtypes of all columns in the Tensor Table column
@@ -173,18 +244,34 @@
                 result[f"{col_name}__values"] = tensor_col.values
                 result[f"{col_name}__offsets"] = tensor_col.offsets
             else:
                 result[col_name] = tensor_col.values
         return result
 
     def cpu(self):
+        """
+        Move this TensorTable and its columns to CPU
+
+        Returns
+        -------
+        TensorTable
+            A new TensorTable containing the same columns but on CPU
+        """
         columns = {col_name: col_values.cpu() for col_name, col_values in self.items()}
         return TensorTable(columns)
 
     def gpu(self):
+        """
+        Move this TensorTable and its columns to GPU
+
+        Returns
+        -------
+        TensorTable
+            A new TensorTable containing the same columns but on GPU
+        """
         columns = {col_name: col_values.gpu() for col_name, col_values in self.items()}
         return TensorTable(columns)
 
     def to_df(self):
         """
         Convert to a dataframe
         """
```

### Comparing `merlin-core-23.4.0/merlin/table/tensorflow_column.py` & `merlin-core-23.5.0/merlin/table/tensorflow_column.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,19 +47,19 @@
     """
 
     @classmethod
     def _transpose(cls, values):
         return tf.transpose(values)
 
     @classmethod
-    def array_type(cls) -> Type:
+    def array_type(cls) -> Optional[Type]:
         """
         The type of the arrays backing this column
         """
-        return tf.Tensor
+        return tf.Tensor if tf else None
 
     @classmethod
     def array_constructor(cls) -> Callable:
         return tf.convert_to_tensor
 
     @classmethod
     def supported_devices(cls):
```

### Comparing `merlin-core-23.4.0/merlin/table/torch_column.py` & `merlin-core-23.5.0/merlin/table/torch_column.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,32 +9,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import Callable, Type
+from typing import Callable, Optional, Type
 
 from merlin.core.compat.torch import torch as th
 from merlin.table.conversions import _from_dlpack_cpu, _from_dlpack_gpu, _to_dlpack
 from merlin.table.tensor_column import Device, TensorColumn
 
 
 class TorchColumn(TensorColumn):
     """
     A SeriesLike column backed by Torch tensors
     """
 
+    framework_name = "torch"
+
     @classmethod
-    def array_type(cls) -> Type:
+    def array_type(cls) -> Optional[Type]:
         """
         The type of the arrays backing this column
         """
-        return th.Tensor
+        return th.Tensor if th else None
 
     @classmethod
     def array_constructor(cls) -> Callable:
         return th.tensor
 
     @classmethod
     def supported_devices(cls):
```

### Comparing `merlin-core-23.4.0/merlin_core.egg-info/PKG-INFO` & `merlin-core-23.5.0/merlin_core.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-core
-Version: 23.4.0
+Version: 23.5.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/core
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -15,21 +15,21 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # [Merlin Core](https://github.com/NVIDIA-Merlin/core)
 
 [![PyPI](https://img.shields.io/pypi/v/merlin-core?color=orange&label=version)](https://pypi.python.org/pypi/merlin-core/)
-[![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/core)](https://github.com/NVIDIA-Merlin/merlin-core/blob/main/LICENSE)
-[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/core/main/)
+[![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/core)](LICENSE)
+[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/core)
 
 The Merlin Core library provides the core utilities for [NVIDIA Merlin](https://github.com/NVIDIA-Merlin) libraries
 like [NVTabular](https://github.com/NVIDIA-Merlin/NVTabular), [Transformers4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec)
 and [Merlin Models](https://github.com/NVIDIA-Merlin/models).
-For example, the [merlin.io.Dataset](https://nvidia-merlin.github.io/core/main/api/merlin.io.html#merlin.io.Dataset) and [merin.schema.Schema](https://nvidia-merlin.github.io/core/main/api/merlin.schema.html#merlin.schema.Schema) classes are fundamental for working with data and building recommender systems with Merlin.
+For example, the [merlin.io.Dataset](https://nvidia-merlin.github.io/core/stable/api/merlin.io.html#merlin.io.Dataset) and [merin.schema.Schema](https://nvidia-merlin.github.io/core/stable/api/merlin.schema.html#merlin.schema.Schema) classes are fundamental for working with data and building recommender systems with Merlin.
 
 ## Installation
 
 ### Installing Merlin Core Using Pip
 
 ```shell
 pip install merlin-core
```

### Comparing `merlin-core-23.4.0/merlin_core.egg-info/SOURCES.txt` & `merlin-core-23.5.0/merlin_core.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,34 +14,35 @@
 merlin/core/protocols.py
 merlin/core/utils.py
 merlin/core/compat/__init__.py
 merlin/core/compat/tensorflow.py
 merlin/core/compat/torch.py
 merlin/dag/__init__.py
 merlin/dag/base_operator.py
-merlin/dag/dictarray.py
 merlin/dag/executors.py
 merlin/dag/graph.py
 merlin/dag/node.py
 merlin/dag/selector.py
 merlin/dag/utils.py
 merlin/dag/ops/__init__.py
 merlin/dag/ops/concat_columns.py
+merlin/dag/ops/rename.py
 merlin/dag/ops/selection.py
 merlin/dag/ops/subset_columns.py
 merlin/dag/ops/subtraction.py
 merlin/dispatch/lazy.py
 merlin/dtypes/__init__.py
 merlin/dtypes/aliases.py
 merlin/dtypes/base.py
 merlin/dtypes/mapping.py
 merlin/dtypes/registry.py
 merlin/dtypes/shape.py
 merlin/dtypes/mappings/__init__.py
 merlin/dtypes/mappings/cudf.py
+merlin/dtypes/mappings/merlin.py
 merlin/dtypes/mappings/numpy.py
 merlin/dtypes/mappings/pandas.py
 merlin/dtypes/mappings/python.py
 merlin/dtypes/mappings/tf.py
 merlin/dtypes/mappings/torch.py
 merlin/dtypes/mappings/triton.py
 merlin/io/__init__.py
@@ -70,13 +71,15 @@
 merlin/table/conversions.py
 merlin/table/cupy_column.py
 merlin/table/numpy_column.py
 merlin/table/tensor_column.py
 merlin/table/tensor_table.py
 merlin/table/tensorflow_column.py
 merlin/table/torch_column.py
+merlin/testing/__init__.py
+merlin/testing/assert_equals.py
 merlin_core.egg-info/PKG-INFO
 merlin_core.egg-info/SOURCES.txt
 merlin_core.egg-info/dependency_links.txt
 merlin_core.egg-info/not-zip-safe
 merlin_core.egg-info/requires.txt
 merlin_core.egg-info/top_level.txt
```

### Comparing `merlin-core-23.4.0/pyproject.toml` & `merlin-core-23.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/setup.cfg` & `merlin-core-23.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/setup.py` & `merlin-core-23.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.4.0/versioneer.py` & `merlin-core-23.5.0/versioneer.py`

 * *Files identical despite different names*

