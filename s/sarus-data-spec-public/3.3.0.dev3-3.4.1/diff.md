# Comparing `tmp/sarus_data_spec_public-3.3.0.dev3.tar.gz` & `tmp/sarus_data_spec_public-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus_data_spec_public-3.3.0.dev3.tar", last modified: Thu May 25 08:51:02 2023, max compression
+gzip compressed data, was "sarus_data_spec_public-3.4.1.tar", last modified: Wed May 31 10:28:36 2023, max compression
```

## Comparing `sarus_data_spec_public-3.3.0.dev3.tar` & `sarus_data_spec_public-3.4.1.tar`

### file list

```diff
@@ -1,201 +1,202 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.682494 sarus_data_spec_public-3.3.0.dev3/
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      436 2023-05-25 08:51:02.682494 sarus_data_spec_public-3.3.0.dev3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.655493 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/
--rwxrwxrwx   0 root         (0) root         (0)      830 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.656493 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/arrow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6445 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/arrow/admin_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/arrow/array.py
--rw-rw-rw-   0 root         (0) root         (0)     3172 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/arrow/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     2101 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/arrow/pandas_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6260 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/arrow/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    10408 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/arrow/type.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/attribute.py
--rw-rw-rw-   0 root         (0) root         (0)     4618 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.657493 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/config/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/config/privacy_properties.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3718 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.657493 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/context/
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/context/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/context/public.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/context/state.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/context/typing.py
--rw-rw-rw-   0 root         (0) root         (0)    18762 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.658493 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_rewriter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_rewriter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_rewriter/base.py
--rw-rw-rw-   0 root         (0) root         (0)    13030 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_rewriter/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_rewriter/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.659493 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_validator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_validator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11237 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_validator/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3882 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_validator/parameter_kind.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_validator/privacy_limit.py
--rw-rw-rw-   0 root         (0) root         (0)    20331 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_validator/signature.py
--rw-rw-rw-   0 root         (0) root         (0)     3012 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_validator/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     4492 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_validator/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     8849 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8679 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/json_serialisation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.660493 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7230 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/async_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    29039 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.660493 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/computations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/computations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8793 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/computations/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.661493 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/computations/local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/computations/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/computations/local/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2311 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/computations/local/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.661493 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/computations/remote/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/computations/remote/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3302 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/computations/remote/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.662493 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3640 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.662493 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.664493 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11571 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/external_op.py
--rw-rw-rw-   0 root         (0) root         (0)     3047 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/imblearn.py
--rw-rw-rw-   0 root         (0) root         (0)     7943 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.664493 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/pandas/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    75666 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
--rw-rw-rw-   0 root         (0) root         (0)    26307 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
--rw-rw-rw-   0 root         (0) root         (0)     2819 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.667493 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21085 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
--rw-rw-rw-   0 root         (0) root         (0)     1914 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
--rw-rw-rw-   0 root         (0) root         (0)    38717 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
--rw-rw-rw-   0 root         (0) root         (0)     2096 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
--rw-rw-rw-   0 root         (0) root         (0)     7004 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
--rw-rw-rw-   0 root         (0) root         (0)    12822 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     6057 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     4382 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
--rw-rw-rw-   0 root         (0) root         (0)     2896 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/skopt.py
--rw-rw-rw-   0 root         (0) root         (0)    18437 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/std.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6106 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/xgboost.py
--rw-rw-rw-   0 root         (0) root         (0)    10560 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.669493 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14040 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/extract.py
--rw-rw-rw-   0 root         (0) root         (0)    11996 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/filter.py
--rw-rw-rw-   0 root         (0) root         (0)    11180 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/get_item.py
--rw-rw-rw-   0 root         (0) root         (0)    11214 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/project.py
--rw-rw-rw-   0 root         (0) root         (0)     6820 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/sample.py
--rw-rw-rw-   0 root         (0) root         (0)     4290 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/select_sql.py
--rw-rw-rw-   0 root         (0) root         (0)     2480 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/shuffle.py
--rw-rw-rw-   0 root         (0) root         (0)    10337 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/standard_op.py
--rw-rw-rw-   0 root         (0) root         (0)    11292 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/synthetic.py
--rw-rw-rw-   0 root         (0) root         (0)    27153 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.670493 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/source/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/source/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/source/privacy_params.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/source/random_seed.py
--rw-rw-rw-   0 root         (0) root         (0)     2596 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/source/routing.py
--rw-rw-rw-   0 root         (0) root         (0)    10235 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/marginals.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/multiplicity.py
--rw-rw-rw-   0 root         (0) root         (0)     3578 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/path.py
--rw-rw-rw-   0 root         (0) root         (0)     3004 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/predicate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.680493 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/attribute.proto
--rw-r--r--   0 root         (0) root         (0)     5552 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/attribute_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/bounds.proto
--rw-r--r--   0 root         (0) root         (0)     6306 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/bounds_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/bounds_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/constraint.proto
--rw-r--r--   0 root         (0) root         (0)     8070 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/constraint_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/constraint_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1233 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/dataset.proto
--rw-r--r--   0 root         (0) root         (0)    24833 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/dataset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8880 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/dataset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/links.proto
--rw-r--r--   0 root         (0) root         (0)    11282 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/links_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4193 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/links_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/manager.proto
--rw-r--r--   0 root         (0) root         (0)     4572 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/manager_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/marginals.proto
--rw-r--r--   0 root         (0) root         (0)     6408 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/marginals_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2177 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/marginals_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/multiplicity.proto
--rw-r--r--   0 root         (0) root         (0)     6521 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/multiplicity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/multiplicity_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/path.proto
--rw-r--r--   0 root         (0) root         (0)     4998 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/path_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/path_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/predicate.proto
--rw-r--r--   0 root         (0) root         (0)    13369 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/predicate_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4859 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/predicate_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/proto_container.proto
--rw-r--r--   0 root         (0) root         (0)     5086 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/proto_container_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/proto_container_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/relation.proto
--rw-r--r--   0 root         (0) root         (0)     5982 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/relation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/relation_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3044 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/scalar.proto
--rw-r--r--   0 root         (0) root         (0)    32882 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/scalar_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14459 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/scalar_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/schema.proto
--rw-r--r--   0 root         (0) root         (0)    12546 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/schema_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/schema_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/size.proto
--rw-r--r--   0 root         (0) root         (0)     6233 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/size_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2162 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/size_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3909 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/statistics.proto
--rw-r--r--   0 root         (0) root         (0)    91981 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/statistics_pb2.py
--rw-r--r--   0 root         (0) root         (0)    32903 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/statistics_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/status.proto
--rw-r--r--   0 root         (0) root         (0)    18816 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     5640 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/transform.proto
--rw-r--r--   0 root         (0) root         (0)   107770 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/transform_pb2.py
--rw-r--r--   0 root         (0) root         (0)    38135 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/transform_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4567 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/type.proto
--rw-r--r--   0 root         (0) root         (0)    74241 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/type_pb2.py
--rw-r--r--   0 root         (0) root         (0)    29134 2023-05-25 08:50:54.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/type_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3914 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/utilities.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    10599 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/scalar.py
--rw-rw-rw-   0 root         (0) root         (0)     4640 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/size.py
--rw-rw-rw-   0 root         (0) root         (0)    43603 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)    16850 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.681494 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11812 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/storage/local.py
--rw-rw-rw-   0 root         (0) root         (0)     5153 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/storage/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3078 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/storage/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    31102 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/transform.py
--rw-rw-rw-   0 root         (0) root         (0)   137071 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/type.py
--rw-rw-rw-   0 root         (0) root         (0)    35885 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     4107 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/variant_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 08:51:02.682494 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec_public.egg-info/
--rw-r--r--   0 root         (0) root         (0)      436 2023-05-25 08:51:02.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec_public.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7837 2023-05-25 08:51:02.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec_public.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 08:51:02.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec_public.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 08:51:02.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec_public.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      109 2023-05-25 08:51:02.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec_public.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-25 08:51:02.000000 sarus_data_spec_public-3.3.0.dev3/sarus_data_spec_public.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     5776 2023-05-25 08:51:02.683493 sarus_data_spec_public-3.3.0.dev3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1191 2023-05-25 08:50:45.000000 sarus_data_spec_public-3.3.0.dev3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.544371 sarus_data_spec_public-3.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)      167 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      431 2023-05-31 10:28:36.544371 sarus_data_spec_public-3.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.518372 sarus_data_spec_public-3.4.1/sarus_data_spec/
+-rwxrwxrwx   0 root         (0) root         (0)      825 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.519372 sarus_data_spec_public-3.4.1/sarus_data_spec/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/arrow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6445 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/arrow/admin_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/arrow/array.py
+-rw-rw-rw-   0 root         (0) root         (0)     3172 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/arrow/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     2101 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/arrow/pandas_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6260 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/arrow/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    10408 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/arrow/type.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)     4618 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.519372 sarus_data_spec_public-3.4.1/sarus_data_spec/config/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/config/privacy_properties.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3718 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.520372 sarus_data_spec_public-3.4.1/sarus_data_spec/context/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/context/public.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/context/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/context/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    18762 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.521372 sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_rewriter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_rewriter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_rewriter/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    13030 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_rewriter/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_rewriter/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.522372 sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_validator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_validator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11823 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_validator/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3882 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_validator/parameter_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_validator/privacy_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)    20331 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_validator/signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     3012 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_validator/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4492 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_validator/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8849 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8679 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/json_serialisation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.522372 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7230 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/async_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    29039 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.523372 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/computations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/computations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8793 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/computations/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.523372 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/computations/local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/computations/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/computations/local/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2311 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/computations/local/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.524372 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/computations/remote/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/computations/remote/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/computations/remote/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.524372 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.524372 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.526372 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11570 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/external_op.py
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/imblearn.py
+-rw-rw-rw-   0 root         (0) root         (0)     7943 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.527372 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8034 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py
+-rw-rw-rw-   0 root         (0) root         (0)    72652 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)    34252 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2819 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.529372 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21085 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
+-rw-rw-rw-   0 root         (0) root         (0)     1914 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
+-rw-rw-rw-   0 root         (0) root         (0)    38717 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2096 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
+-rw-rw-rw-   0 root         (0) root         (0)     7004 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    12822 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     6057 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4382 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2896 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/skopt.py
+-rw-rw-rw-   0 root         (0) root         (0)    18437 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/std.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6106 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/xgboost.py
+-rw-rw-rw-   0 root         (0) root         (0)    10560 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.531372 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14040 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)    11996 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11180 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/get_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    11214 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     6820 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     4290 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/select_sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/shuffle.py
+-rw-rw-rw-   0 root         (0) root         (0)    10337 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/standard_op.py
+-rw-rw-rw-   0 root         (0) root         (0)    11292 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/synthetic.py
+-rw-rw-rw-   0 root         (0) root         (0)    27153 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.532372 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/source/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/source/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/source/privacy_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/source/random_seed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2596 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/source/routing.py
+-rw-rw-rw-   0 root         (0) root         (0)    10235 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/manager/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/marginals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/multiplicity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3578 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/predicate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.542372 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/attribute.proto
+-rw-r--r--   0 root         (0) root         (0)     5552 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/attribute_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/bounds.proto
+-rw-r--r--   0 root         (0) root         (0)     6306 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/bounds_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/bounds_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/constraint.proto
+-rw-r--r--   0 root         (0) root         (0)     8070 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/constraint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/constraint_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/dataset.proto
+-rw-r--r--   0 root         (0) root         (0)    24833 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/dataset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8880 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/dataset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/links.proto
+-rw-r--r--   0 root         (0) root         (0)    11282 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/links_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4193 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/links_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/manager.proto
+-rw-r--r--   0 root         (0) root         (0)     4572 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/manager_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/manager_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/marginals.proto
+-rw-r--r--   0 root         (0) root         (0)     6408 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/marginals_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2177 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/marginals_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/multiplicity.proto
+-rw-r--r--   0 root         (0) root         (0)     6521 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/multiplicity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/multiplicity_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/path.proto
+-rw-r--r--   0 root         (0) root         (0)     4998 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/path_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/path_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/predicate.proto
+-rw-r--r--   0 root         (0) root         (0)    13369 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/predicate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/predicate_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/proto_container.proto
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/proto_container_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/proto_container_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/relation.proto
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/relation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/relation_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3044 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/scalar.proto
+-rw-r--r--   0 root         (0) root         (0)    32882 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/scalar_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14459 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/scalar_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/schema.proto
+-rw-r--r--   0 root         (0) root         (0)    12546 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/schema_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/schema_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/size.proto
+-rw-r--r--   0 root         (0) root         (0)     6233 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/size_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/size_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/statistics.proto
+-rw-r--r--   0 root         (0) root         (0)    91981 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/statistics_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    32903 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/statistics_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/status.proto
+-rw-r--r--   0 root         (0) root         (0)    18816 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     5640 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/transform.proto
+-rw-r--r--   0 root         (0) root         (0)   107770 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/transform_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    38135 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/transform_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4567 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/type.proto
+-rw-r--r--   0 root         (0) root         (0)    74241 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/type_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    29134 2023-05-31 10:28:28.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/type_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3914 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/utilities.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    10599 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/scalar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4640 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/size.py
+-rw-rw-rw-   0 root         (0) root         (0)    43603 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)    16850 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.543372 sarus_data_spec_public-3.4.1/sarus_data_spec/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11812 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/storage/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     5153 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/storage/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3078 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/storage/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    31102 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)   137075 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/type.py
+-rw-rw-rw-   0 root         (0) root         (0)    35885 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4107 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/sarus_data_spec/variant_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 10:28:36.544371 sarus_data_spec_public-3.4.1/sarus_data_spec_public.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      431 2023-05-31 10:28:36.000000 sarus_data_spec_public-3.4.1/sarus_data_spec_public.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7902 2023-05-31 10:28:36.000000 sarus_data_spec_public-3.4.1/sarus_data_spec_public.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 10:28:36.000000 sarus_data_spec_public-3.4.1/sarus_data_spec_public.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 10:28:36.000000 sarus_data_spec_public-3.4.1/sarus_data_spec_public.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      110 2023-05-31 10:28:36.000000 sarus_data_spec_public-3.4.1/sarus_data_spec_public.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-31 10:28:36.000000 sarus_data_spec_public-3.4.1/sarus_data_spec_public.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5840 2023-05-31 10:28:36.545372 sarus_data_spec_public-3.4.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1186 2023-05-31 10:28:20.000000 sarus_data_spec_public-3.4.1/setup.py
```

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/__init__.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sarus_data_spec.transform import Transform
 from sarus_data_spec.variant_constraint import VariantConstraint
 
 """A library to manage Sarus datasets"""
 # pylint: disable=unused-variable
 
 PACKAGE_NAME: Final[str] = 'sarus_data_spec'
-VERSION: Final[str] = '3.3.0.dev3'
+VERSION: Final[str] = '3.4.1'
 
 try:
     import sarus_data_spec.context.worker as sw
 
     push_global_context(sw.WorkerContext())
 except ModuleNotFoundError as exception:
     if exception.name == 'sarus_data_spec.context.worker':
```

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/arrow/admin_utils.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/arrow/admin_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/arrow/array.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/arrow/array.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/arrow/conversion.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/arrow/conversion.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/arrow/pandas_utils.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/arrow/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/arrow/schema.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/arrow/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/arrow/type.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/arrow/type.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/attribute.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/attribute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/base.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/bounds.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/bounds.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/config/privacy_properties.yaml` & `sarus_data_spec_public-3.4.1/sarus_data_spec/config/privacy_properties.yaml`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/constants.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/constants.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/context/public.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/context/public.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/context/typing.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/context/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataset.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_rewriter/base.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_rewriter/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_rewriter/simple_rules.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_rewriter/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_rewriter/typing.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_rewriter/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_validator/base.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_validator/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from sarus_data_spec.attribute import attach_properties
 from sarus_data_spec.constants import (
     IS_PUBLIC,
     NO_TOKEN,
     PEP_TOKEN,
     PRIVATE_QUERY,
+    PUBLIC,
 )
 from sarus_data_spec.dataspec_validator.privacy_limit import DeltaEpsilonLimit
 from sarus_data_spec.manager.async_utils import sync
 from sarus_data_spec.manager.ops.processor import routing
 from sarus_data_spec.protobuf.utilities import dejson
 from sarus_data_spec.protobuf.utilities import json as proto_to_json
 from sarus_data_spec.storage.typing import Storage
@@ -172,19 +173,33 @@
         for constraint in self.verified_constraints(dataspec):
             if self.verifies(constraint, kind, public_context, privacy_limit):
                 return constraint.properties()[IS_PUBLIC] == str(True)
 
         # Determine is the Dataspec is public
         if dataspec.is_transformed():
             # Returns true if the DataSpec derives only from public
-            args_parents, kwargs_parents = dataspec.parents()
-            is_public = all(
-                [self.is_public(ds) for ds in args_parents]
-                + [self.is_public(ds) for ds in kwargs_parents.values()]
-            )
+            if (
+                dataspec.transform().is_external()
+                or dataspec.prototype() == sp.Scalar
+            ):
+                args_parents, kwargs_parents = dataspec.parents()
+                is_public = all(
+                    [self.is_public(ds) for ds in args_parents]
+                    + [self.is_public(ds) for ds in kwargs_parents.values()]
+                )
+            else:
+                assert dataspec.prototype() == sp.Dataset
+                # For a standard transform, all tables must be
+                # public in the schema to have a public dataset
+                dataset = cast(st.Dataset, dataspec)
+                schema = dataset.schema()
+                is_public = schema.data_type().properties()[PUBLIC] == str(
+                    True
+                )
+
         elif dataspec.prototype() == sp.Scalar:
             scalar = cast(st.Scalar, dataspec)
             assert (
                 scalar.is_random_seed()
                 or scalar.is_privacy_params()
                 or scalar.is_synthetic_model()
             )
```

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_validator/parameter_kind.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_validator/parameter_kind.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_validator/privacy_limit.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_validator/privacy_limit.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_validator/signature.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_validator/signature.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_validator/simple_rules.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_validator/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/dataspec_validator/typing.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/dataspec_validator/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/deprecation.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/deprecation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/factory.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/factory.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/json_serialisation.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/json_serialisation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/async_utils.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/async_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/base.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/computations/base.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/computations/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/computations/local/base.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/computations/local/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/computations/local/schema.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/computations/local/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/computations/remote/base.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/computations/remote/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/base.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/__init__.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/external_op.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/external_op.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         """
         transform = self.dataspec.transform()
         implementation = external_implementation(transform)
         dp_implementation = implementation.dp_equivalent()
         bound_signature = implementation.signature().bind_dataspec(
             self.dataspec
         )
-
         if dp_implementation is None or not dp_implementation.is_dp(
             bound_signature
         ):
             return False
 
         return bound_signature.pep_token() is not None
```

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/imblearn.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/imblearn.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/numpy.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/numpy.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,27 +154,33 @@
     )
 
     async def call(self, signature: SarusBoundSignature) -> pd.DataFrame:
         (this, key) = await signature.collect_args()
         return this.loc[key]
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
-        """PEP in all cases.
-        Preserves the alignment if the key is a tuple or a slice that
-        selects all the rows (e.g. loc[:, "col"], loc[:])."""
+        """Token preserving if the key is a tuple or a slice that
+        selects all the rows (e.g. loc[:, "col"], loc[:]).
+        Not PEP if the key is a single int.
+        PEP in the other cases.
+        """
         key_arg = signature["key"]
         if STATIC.isin(key_arg.parameter_kind()):
             key_value = key_arg.static_value()
             if isinstance(key_value, tuple) and len(key_value) == 2:
                 row_key, _ = key_value
                 if row_key == slice(None, None, None):
                     return PEPKind.TOKEN_PRESERVING
             elif isinstance(key_value, slice):
                 if key_value == slice(None, None, None):
                     return PEPKind.TOKEN_PRESERVING
+            elif isinstance(key_value, int):
+                # a int changes the index, we are not able to compute
+                # the output PE
+                return PEPKind.NOT_PEP
 
         return PEPKind.PEP
 
 
 class pd_set_loc(ExternalOpImplementation):
     _transform_id = "pandas.PD_SET_LOC"
     _signature = SarusSignature(
@@ -216,23 +222,29 @@
     )
 
     async def call(self, signature: SarusBoundSignature) -> pd.DataFrame:
         (this, key) = await signature.collect_args()
         return this.iloc[key]
 
     def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
-        """PEP in all cases.
-        Preserves the alignment if the key is a slice that
-        selects all the rows (e.g. iloc[:])."""
+        """Token preserving the alignment if the key is a slice that
+        selects all the rows (e.g. iloc[:]).
+        Not PEP if the key is a single int.
+        PEP in the other cases.
+        """
         key_arg = signature["key"]
         if STATIC.isin(key_arg.parameter_kind()):
             key_value = key_arg.static_value()
             if isinstance(key_value, slice):
                 if key_value == slice(None, None, None):
                     return PEPKind.TOKEN_PRESERVING
+            elif isinstance(key_value, int):
+                # a int changes the index, we are not able to compute
+                # the output PE
+                return PEPKind.NOT_PEP
 
         return PEPKind.PEP
 
 
 class pd_set_iloc(ExternalOpImplementation):
     _transform_id = "pandas.PD_SET_ILOC"
     _signature = SarusSignature(
@@ -1394,14 +1406,15 @@
             if kwargs[name] is None:
                 del kwargs[name]
         return this.reindex(**kwargs)
 
 
 class pd_count(ExternalOpImplementation):
     _transform_id = "pandas.PD_COUNT"
+    _dp_equivalent_id = "pandas.PD_COUNT_DP"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Union[pd.Series, pd.DataFrame],
             condition=DATASPEC,
         ),
         SarusParameter(
@@ -1442,14 +1455,15 @@
     async def call(self, signature: SarusBoundSignature) -> Any:
         this, kwargs = await signature.collect_kwargs_method()
         return this.transpose(**kwargs)
 
 
 class pd_value_counts(ExternalOpImplementation):
     _transform_id = "pandas.PD_VALUE_COUNTS"
+    _dp_equivalent_id = "pandas.PD_VALUE_COUNTS_DP"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Union[pd.Series, pd.DataFrame],
             condition=DATASPEC,
         ),
         SarusParameter(
@@ -2538,136 +2552,7 @@
             default=None,
         ),
     )
 
     async def call(self, signature: SarusBoundSignature) -> Any:
         this, kwargs = await signature.collect_kwargs_method()
         return this.union(**kwargs)
-
-
-# ------ GROUPBY METHODS ----------
-class pd_groups(ExternalOpImplementation):
-    _transform_id = "pandas.PD_GROUPS"
-    _signature = SarusSignature(
-        SarusParameter(
-            name="this",
-            annotation=Union[
-                pd.core.groupby.DataFrameGroupBy, pd.core.groupby.SeriesGroupBy
-            ],
-            condition=DATASPEC,
-        ),
-    )
-
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        (this,) = await signature.collect_args()
-        return this.groups
-
-
-class pd_sum_groupby(ExternalOpImplementation):
-    _transform_id = "pandas.PD_SUM_GROUPBY"
-    _signature = SarusSignature(
-        SarusParameter(
-            name="this",
-            annotation=pd.core.groupby.GroupBy,
-            condition=DATASPEC,
-        ),
-        SarusParameter(
-            name="numeric_only",
-            annotation=bool,
-            default=False,
-        ),
-        SarusParameter(
-            name="min_count",
-            annotation=int,
-            default=0,
-        ),
-    )
-
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
-        return this.sum(**kwargs)
-
-
-class pd_std_groupby(ExternalOpImplementation):
-    _transform_id = "pandas.PD_STD_GROUPBY"
-    _signature = SarusSignature(
-        SarusParameter(
-            name="this",
-            annotation=pd.core.groupby.GroupBy,
-            condition=DATASPEC,
-        ),
-        SarusParameter(
-            name="ddof",
-            annotation=int,
-            default=1,
-        ),
-        # > 1.3.5
-        # SarusParameter(
-        #     name="engine",
-        #     annotation=Optional[str],
-        #     default=None,
-        # ),
-        # SarusParameter(
-        #     name="engine_kwargs",
-        #     annotation=Optional[Dict[str, bool]],
-        #     default=None,
-        # ),
-        # SarusParameter(
-        #     name="numeric_only",
-        #     annotation=bool,
-        #     default=False,
-        # ),
-    )
-
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
-        return this.std(**kwargs)
-
-
-class pd_mean_groupby(ExternalOpImplementation):
-    _transform_id = "pandas.PD_MEAN_GROUPBY"
-    _signature = SarusSignature(
-        SarusParameter(
-            name="this",
-            annotation=pd.core.groupby.GroupBy,
-            condition=DATASPEC,
-        ),
-        SarusParameter(
-            name="numeric_only",
-            annotation=bool,
-            default=False,
-        ),
-        # SarusParameter(
-        #     name="engine",
-        #     annotation=str,
-        #     default="cython",
-        # ),
-        # SarusParameter(
-        #     name="engine_kwargs",
-        #     annotation=Optional[Dict[str, bool]],
-        #     default=None,
-        # ),
-    )
-
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
-        return this.mean(**kwargs)
-
-
-class pd_median_groupby(ExternalOpImplementation):
-    _transform_id = "pandas.PD_MEDIAN_GROUPBY"
-    _signature = SarusSignature(
-        SarusParameter(
-            name="this",
-            annotation=pd.core.groupby.GroupBy,
-            condition=DATASPEC,
-        ),
-        SarusParameter(
-            name="numeric_only",
-            annotation=bool,
-            default=False,
-        ),
-    )
-
-    async def call(self, signature: SarusBoundSignature) -> Any:
-        this, kwargs = await signature.collect_kwargs_method()
-        return this.median(**kwargs)
```

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from ..external_op import ExternalOpImplementation
 
 logger = logging.getLogger(__name__)
 
 try:
     from sarus_statistics.ops.bounds.op import BoundOp
-    from sarus_statistics.ops.histograms.op import CountOp
+    from sarus_statistics.ops.histograms.op import CountOp, HistogramOp
     from sarus_statistics.ops.max_multiplicity.op import MaxMultiplicityOp
     from sarus_statistics.ops.mean.op import MeanOp
     from sarus_statistics.ops.median.op import MedianOp
     from sarus_statistics.ops.std.op import StdOp
     from sarus_statistics.ops.sum.op import SumOp
     from sarus_statistics.protobuf.multiplicity_pb2 import (
         MultiplicityParameters,
@@ -120,15 +120,15 @@
         """Implementation of DP shape.
 
         A DP implementation receives additional arguments compared to a
         standard external implementation:
             - `budget`: a list of sp.Scalar.PrivacyParams.Point
                 object containing each an epsilon and a delta values
             - `seed`: an integer used to parametrize random number generators
-            - `pe`: theprotected entity used by `sarus_statistics` primitives
+            - `pe`: the protected entity used by `sarus_statistics` primitives
         """
         # Evaluate arguments
         parent_ds = signature.static_kwargs()["this"]
         (dataframe, budget, seed) = await signature.collect_args()
 
         # Get QB task parametrization
         _, tasks = await self.private_queries_and_task(signature)
@@ -149,19 +149,17 @@
             max_mult_task.noise_multiplicity,
             max_mult_task.max_max_multiplicity,
         ).value(random_generator)
 
         n_rows = CountOp(
             parent_ds,
             noise=shape_task.parameters['noise'],
-        ).value(max_mul, random_generator)
+        ).value(None, max_mul, random_generator)
 
         dp_shape = (n_rows, n_cols)
-
-        # Compute private query
         return dp_shape
 
 
 class pd_sum_dp(ExternalOpImplementation):
     _transform_id = "pandas.PD_SUM_DP"
     _non_dp_equivalent_id = "pandas.PD_SUM"
 
@@ -611,15 +609,15 @@
         column_bounds_std_builder: OptimizableQueryBuilder = (
             simple_composed_builder(
                 parent_ds,
                 [
                     simple_bounds_builder(
                         parent_ds, Query(bounds=Query.Bounds())
                     ),
-                    std_builder(parent_ds, Query(median=Query.Median())),
+                    std_builder(parent_ds, Query(std=Query.Std())),
                 ],
             )
         )
 
         builder = simple_composed_builder(
             parent_ds,
             [max_mult_builder] + n_cols * [column_bounds_std_builder],
@@ -694,7 +692,205 @@
 
         if signature["this"].python_type() == str(pd.DataFrame):
             std_dp = pd.Series(std_dp_dict)
         else:
             std_dp = list(std_dp_dict.values()).pop()
 
         return std_dp
+
+
+class pd_count_dp(ExternalOpImplementation):
+    _transform_id = "pandas.PD_COUNT_DP"
+    _non_dp_equivalent_id = "pandas.PD_COUNT"
+
+    def is_dp(self, signature: SarusBoundSignature) -> bool:
+        """`axis = 0` and `numeric_only` is `True`"""
+        axis = signature["axis"].static_value()
+        return bool(axis == 0)
+
+    async def private_queries_and_task(
+        self, signature: SarusBoundSignature
+    ) -> t.Tuple[t.List[st.PrivateQuery], st.Task]:
+        parent_ds = signature["this"].static_value()
+        budget = await signature["budget"].collect()
+        if len(budget) != 1:
+            raise NotImplementedError(
+                "The PrivacyParams contains more than 1 point in the privacy "
+                "profile."
+            )
+
+        parent_schema = await parent_ds.manager().async_schema(parent_ds)
+        max_max_mult = int(
+            parent_schema.properties().get(MAX_MAX_MULT, DEFAULT_MAX_MAX_MULT)
+        )
+
+        epsilon = budget[0].epsilon
+        delta = budget[0].delta
+        if epsilon == 0.0:
+            raise ValueError("`epsilon` should be greater than 0.")
+        n_cols = len(parent_schema.data_type().children())
+
+        max_mult_builder: OptimizableQueryBuilder = (
+            simple_max_multiplicity_builder(
+                parent_ds,
+                Query(
+                    max_multiplicity=Query.MaxMultiplicity(
+                        max_max_multiplicity=max_max_mult
+                    )
+                ),
+            )
+        )
+        column_counts_builder = laplace_builder(
+            parent_ds, Query(laplace_mechanism=Query.LaplaceMechanism())
+        )
+        builders_list: t.List[OptimizableQueryBuilder] = [max_mult_builder]
+        builders_list.extend(n_cols * [column_counts_builder])
+        builder = simple_composed_builder(parent_ds, builders_list)
+        tasks = builder.build_query(
+            builder.target([(epsilon, delta)], (0, epsilon))
+        )
+        query = builder.private_query(tasks)
+        composed_query = t.cast(ComposedPrivateQuery, query)
+        return list(composed_query.all_subqueries()), tasks
+
+    async def call(self, signature: SarusBoundSignature) -> t.Any:
+        # Evaluate arguments
+        parent_ds: st.Dataset = signature["this"].static_value()
+        dataframe: pd.DataFrame = await parent_ds.async_to(pd.DataFrame)
+        budget_value = await signature["budget"].collect()
+        seed_value = await signature["seed"].collect()
+
+        _, tasks = await self.private_queries_and_task(signature)
+        tasks = [unwrap(subtask) for subtask in tasks.subtasks]
+        max_mult_task, shape_task = tasks[0], tasks[1:]
+
+        epsilon = budget_value[0].epsilon
+        random_generator = np.random.default_rng(abs(seed_value))
+
+        # Compute DP value
+        max_mul = MaxMultiplicityOp(
+            parent_ds,
+            epsilon,  # parameter for quantiles
+            max_mult_task.noise_user_count,
+            max_mult_task.noise_multiplicity,
+            max_mult_task.max_max_multiplicity,
+        ).value(random_generator)
+
+        count_dp_dict = {}
+        for index, column_name in enumerate(dataframe.columns):
+            count_parameters = shape_task[index]
+            count_dp_dict[column_name] = CountOp(
+                parent_ds,
+                count_parameters.parameters['noise'],
+            ).value(column_name, max_mul, random_generator)
+
+        if signature["this"].python_type() == str(pd.DataFrame):
+            count_dp = pd.Series(count_dp_dict)
+        else:
+            count_dp = list(count_dp_dict.values()).pop()
+        return count_dp
+
+
+class pd_value_counts_dp(ExternalOpImplementation):
+    _transform_id: str = "pandas.PD_VALUE_COUNTS_DP"
+    _non_dp_equivalent_id = "pandas.PD_VALUE_COUNTS"
+
+    def is_dp(self, signature: SarusBoundSignature) -> bool:
+        return signature["this"].python_type() == str(pd.Series)
+
+    async def private_queries_and_task(
+        self, signature: SarusBoundSignature
+    ) -> t.Tuple[t.List[st.PrivateQuery], st.Task]:
+        """Return the PrivateQueries summarizing DP characteristics."""
+        parent_ds = signature["this"].static_value()
+        budget = await signature["budget"].collect()
+        if len(budget) != 1:
+            raise NotImplementedError(
+                "The PrivacyParams contains more than 1 point in the privacy "
+                "profile."
+            )
+
+        parent_schema = await parent_ds.manager().async_schema(parent_ds)
+        max_max_mult = int(
+            parent_schema.properties().get(MAX_MAX_MULT, DEFAULT_MAX_MAX_MULT)
+        )
+
+        epsilon = budget[0].epsilon
+        delta = budget[0].delta
+        if epsilon == 0.0:
+            raise ValueError("`epsilon` should be greater than 0.")
+        n_cols = len(parent_schema.data_type().children())
+
+        max_mult_builder: OptimizableQueryBuilder = (
+            simple_max_multiplicity_builder(
+                parent_ds,
+                Query(
+                    max_multiplicity=Query.MaxMultiplicity(
+                        max_max_multiplicity=max_max_mult
+                    )
+                ),
+            )
+        )
+        column_counts_builder = laplace_builder(
+            parent_ds, Query(laplace_mechanism=Query.LaplaceMechanism())
+        )
+        builders_list: t.List[OptimizableQueryBuilder] = [max_mult_builder]
+        builders_list.extend(n_cols * [column_counts_builder])
+        builder = simple_composed_builder(parent_ds, builders_list)
+        tasks = builder.build_query(
+            builder.target([(epsilon, delta)], (0, epsilon))
+        )
+        query = builder.private_query(tasks)
+        composed_query = t.cast(ComposedPrivateQuery, query)
+        return list(composed_query.all_subqueries()), tasks
+
+    async def call(self, signature: SarusBoundSignature) -> t.Any:
+        """Implementation of DP shape.
+
+        A DP implementation receives additional arguments compared to a
+        standard external implementation:
+            - `budget`: a list of sp.Scalar.PrivacyParams.Point
+                object containing each an epsilon and a delta values
+            - `seed`: an integer used to parametrize random number generators
+            - `pe`: the protected entity used by `sarus_statistics` primitives
+        """
+        parent_ds: st.Dataset = signature["this"].static_value()
+        dataframe: pd.DataFrame = await parent_ds.async_to(pd.DataFrame)
+        budget_value = await signature["budget"].collect()
+        seed_value = await signature["seed"].collect()
+        sort = await signature["sort"].collect()
+        ascending = await signature["ascending"].collect()
+        normalize = await signature["normalize"].collect()
+        dropna = await signature["dropna"].collect()
+
+        _, tasks = await self.private_queries_and_task(signature)
+        tasks = [unwrap(subtask) for subtask in tasks.subtasks]
+        max_mult_task, shape_task = tasks[0], tasks[1:]
+
+        epsilon = budget_value[0].epsilon
+        random_generator = np.random.default_rng(abs(seed_value))
+
+        # Compute DP value
+        max_mul = MaxMultiplicityOp(
+            parent_ds,
+            epsilon,  # parameter for quantiles
+            max_mult_task.noise_user_count,
+            max_mult_task.noise_multiplicity,
+            max_mult_task.max_max_multiplicity,
+        ).value(random_generator)
+
+        count_dp_dict = {}
+        for index, column_name in enumerate(dataframe.columns):
+            count_parameters = shape_task[index]
+
+            count_dp_dict[column_name] = HistogramOp(
+                parent_ds,
+                noise=count_parameters.parameters['noise'],
+                sort=sort,
+                ascending=ascending,
+                normalize=normalize,
+                dropna=dropna,
+            ).value(column_name, max_mul, random_generator)
+
+        # for now only on series
+        count_dp = pd.Series(list(count_dp_dict.values())[0])
+        return count_dp
```

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/skopt.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/skopt.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/std.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/std.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/typing.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/utils.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/external/xgboost.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/external/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/routing.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/extract.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/extract.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/filter.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/filter.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/get_item.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/get_item.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/project.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/project.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/sample.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/select_sql.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/select_sql.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/shuffle.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/shuffle.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/standard_op.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/standard_op.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/synthetic.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/synthetic.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/ops/source/routing.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/ops/source/routing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/manager/typing.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/marginals.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/marginals.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/multiplicity.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/multiplicity.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/path.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/path.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/predicate.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/predicate.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/__init__.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/attribute_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/attribute_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/attribute_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/attribute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/bounds_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/bounds_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/bounds_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/bounds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/constraint_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/constraint_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/constraint_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/constraint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/dataset.proto` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/dataset.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/dataset_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/dataset_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/links_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/links_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/links_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/manager_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/manager_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/marginals_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/marginals_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/marginals_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/marginals_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/multiplicity_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/multiplicity_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/multiplicity_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/multiplicity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/path_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/path_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/path_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/path_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/predicate.proto` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/predicate.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/predicate_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/predicate_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/predicate_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/predicate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/proto_container_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/proto_container_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/proto_container_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/proto_container_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/relation.proto` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/relation.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/relation_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/relation_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/relation_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/relation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/scalar.proto` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/scalar.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/scalar_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/scalar_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/scalar_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/scalar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/schema.proto` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/schema.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/schema_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/schema_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/size_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/size_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/size_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/size_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/statistics.proto` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/statistics.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/statistics_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/statistics_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/statistics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/status.proto` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/status.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/status_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/status_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/status_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/transform.proto` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/transform.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/transform_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/transform_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/transform_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/transform_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/type.proto` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/type_pb2.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/type_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/type_pb2.pyi` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/typing.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/protobuf/utilities.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/protobuf/utilities.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/scalar.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/scalar.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/schema.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/size.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/size.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/statistics.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/statistics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/status.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/status.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/storage/local.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/storage/local.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/storage/typing.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/storage/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/storage/utils.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/storage/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/transform.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/transform.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/type.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/type.py`

 * *Files 0% similar despite different names*

```diff
@@ -3383,15 +3383,15 @@
                     ("%S", "s"),
                     ("%f", "us"),
                 ]:
                     if unit not in format:
                         break
                     elif unit in ["%m", "%Y"]:
                         # months and years have variable length
-                        as_unit = np.datetime64(bound, np_unit)
+                        as_unit = np.datetime64(int_bound, np_unit)
                         aliasing = np.timedelta64(1, np_unit)
                         aliasing = as_unit + aliasing - as_unit
                         aliasing = aliasing.astype("timedelta64[ns]")
                     else:
                         aliasing = np.timedelta64(1, np_unit)
             elif i == 1:
                 int_bound = iint64.max
```

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/typing.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec/variant_constraint.py` & `sarus_data_spec_public-3.4.1/sarus_data_spec/variant_constraint.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.3.0.dev3/sarus_data_spec_public.egg-info/SOURCES.txt` & `sarus_data_spec_public-3.4.1/sarus_data_spec_public.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
 sarus_data_spec/manager/ops/processor/external/skopt.py
 sarus_data_spec/manager/ops/processor/external/std.py
 sarus_data_spec/manager/ops/processor/external/typing.py
 sarus_data_spec/manager/ops/processor/external/utils.py
 sarus_data_spec/manager/ops/processor/external/xgboost.py
 sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
+sarus_data_spec/manager/ops/processor/external/pandas/groupby.py
 sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
 sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
 sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
 sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
 sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
 sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
 sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
```

### Comparing `sarus_data_spec_public-3.3.0.dev3/setup.cfg` & `sarus_data_spec_public-3.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 	sarus_data_spec.manager.ops.processor.standard.select_sql
 	sarus_data_spec.manager.ops.processor.standard.extract
 	sarus_data_spec.manager.ops.processor.standard.shuffle
 	sarus_data_spec.manager.ops.processor.standard.synthetic
 	sarus_data_spec.manager.ops.processor.external.external_op
 	sarus_data_spec.manager.ops.processor.external.imblearn
 	sarus_data_spec.manager.ops.processor.external.numpy
+	sarus_data_spec.manager.ops.processor.external.pandas.groupby
 	sarus_data_spec.manager.ops.processor.external.pandas.pandas
 	sarus_data_spec.manager.ops.processor.external.pandas.pandas_dp
 	sarus_data_spec.manager.ops.processor.external.pandas_profiling
 	sarus_data_spec.manager.ops.processor.external.sklearn
 	sarus_data_spec.manager.ops.processor.external.sklearn.cluster
 	sarus_data_spec.manager.ops.processor.external.sklearn.compose
 	sarus_data_spec.manager.ops.processor.external.sklearn.decomposition
@@ -131,15 +132,15 @@
 	sarus_data_spec.protobuf.statistics_pb2
 	sarus_data_spec.protobuf.status_pb2
 	sarus_data_spec.protobuf.transform_pb2
 	sarus_data_spec.protobuf.type_pb2
 install_requires = 
 	protobuf >= 3.0, < 4.0
 	numpy>=1.20.0
-	pyarrow >= 5.0
+	pyarrow ~= 11.0
 	fsspec[http,gcs] >= 2021.0 # Generic FS support (e.g. in apache arrow)
 	tqdm >= 4.0
 	pandas~=1.3.0
 	pyyaml >= 5.4.1
 
 [options.packages.find]
 exclude = tests
```

### Comparing `sarus_data_spec_public-3.3.0.dev3/setup.py` & `sarus_data_spec_public-3.4.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
     def run(self):
         generate_proto_code()
         build_py.run(self)
 
 
 if __name__ == '__main__':
-    setup(version='3.3.0.dev3')
+    setup(version='3.4.1')
```

