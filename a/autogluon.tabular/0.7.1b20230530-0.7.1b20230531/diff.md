# Comparing `tmp/autogluon.tabular-0.7.1b20230530.tar.gz` & `tmp/autogluon.tabular-0.7.1b20230531.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.tabular-0.7.1b20230530.tar", last modified: Tue May 30 09:04:14 2023, max compression
+gzip compressed data, was "autogluon.tabular-0.7.1b20230531.tar", last modified: Wed May 31 09:04:16 2023, max compression
```

## Comparing `autogluon.tabular-0.7.1b20230530.tar` & `autogluon.tabular-0.7.1b20230531.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.025718 autogluon.tabular-0.7.1b20230530/
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-05-30 09:04:14.025718 autogluon.tabular-0.7.1b20230530/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 09:04:14.025718 autogluon.tabular-0.7.1b20230530/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.013718 autogluon.tabular-0.7.1b20230530/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.013718 autogluon.tabular-0.7.1b20230530/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.017718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.017718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/configs/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/configs/feature_generator_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/configs/hyperparameter_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.017718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47558 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/learner/abstract_learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/learner/default_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.017718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.017718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/_utils/rapids_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/_utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.017718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/automm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/automm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/automm/automm_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/automm/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.017718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/catboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/catboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/catboost/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/catboost/catboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/catboost/catboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.017718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/catboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.017718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fastainn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fastainn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fastainn/callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fastainn/fastai_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.017718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fastainn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fastainn/imports_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fastainn/quantile_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25059 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.017718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fasttext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fasttext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fasttext/fasttext_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.017718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fasttext/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.017718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/image_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/image_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/image_prediction/image_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.017718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/imodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/imodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/imodels/imodels_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.017718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/knn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/knn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/knn/_knn_loo_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/knn/knn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/knn/knn_rapids_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/knn/knn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.021718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lgb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lgb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lgb/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.021718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lgb/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    18414 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lgb/lgb_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lgb/lgb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.021718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.021718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lr/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lr/lr_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lr/lr_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.021718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/rf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/rf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.021718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/rf/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/rf/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/rf/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/rf/compilers/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/rf/rf_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36291 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/rf/rf_quantile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/rf/rf_rapids_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.021718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.021718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/pretexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.021718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.021718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/compilers/native.py
--rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.021718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.021718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33156 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.025718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35716 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.025718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/text_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/text_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.025718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/vowpalwabbit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/vowpalwabbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.025718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/xgboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/xgboost/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.025718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/xgboost/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/xgboost/xgboost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/xgboost/xgboost_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.025718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/xt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/xt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/xt/xt_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.025718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   248865 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/predictor/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.025718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.025718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/trainer/model_presets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/trainer/model_presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/trainer/model_presets/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/trainer/model_presets/presets_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/trainer/model_presets/presets_distill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.025718 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-30 09:03:44.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/tuning/feature_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-30 09:04:13.000000 autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:04:14.013718 autogluon.tabular-0.7.1b20230530/src/autogluon.tabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-05-30 09:04:13.000000 autogluon.tabular-0.7.1b20230530/src/autogluon.tabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-05-30 09:04:13.000000 autogluon.tabular-0.7.1b20230530/src/autogluon.tabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:04:13.000000 autogluon.tabular-0.7.1b20230530/src/autogluon.tabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 09:04:13.000000 autogluon.tabular-0.7.1b20230530/src/autogluon.tabular.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-30 09:04:13.000000 autogluon.tabular-0.7.1b20230530/src/autogluon.tabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 09:04:13.000000 autogluon.tabular-0.7.1b20230530/src/autogluon.tabular.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:04:13.000000 autogluon.tabular-0.7.1b20230530/src/autogluon.tabular.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.919524 autogluon.tabular-0.7.1b20230531/
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-05-31 09:04:16.919524 autogluon.tabular-0.7.1b20230531/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:04:16.919524 autogluon.tabular-0.7.1b20230531/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.903524 autogluon.tabular-0.7.1b20230531/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.903524 autogluon.tabular-0.7.1b20230531/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.903524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.903524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/configs/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/configs/feature_generator_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/configs/hyperparameter_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.907524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47558 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/learner/abstract_learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24172 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/learner/default_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.907524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.907524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/_utils/rapids_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/_utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.907524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/automm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/automm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/automm/automm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/automm/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.907524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/catboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/catboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/catboost/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/catboost/catboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/catboost/catboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.907524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/catboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/catboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.907524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fastainn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fastainn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fastainn/callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1370 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fastainn/fastai_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.907524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fastainn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fastainn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fastainn/imports_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fastainn/quantile_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25059 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.907524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fasttext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fasttext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fasttext/fasttext_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.907524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fasttext/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fasttext/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.907524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/image_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/image_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/image_prediction/image_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.907524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/imodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/imodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/imodels/imodels_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.907524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/knn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/knn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/knn/_knn_loo_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/knn/knn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/knn/knn_rapids_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/knn/knn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.907524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lgb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lgb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lgb/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.911524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lgb/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lgb/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18414 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lgb/lgb_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lgb/lgb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.911524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.911524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lr/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lr/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lr/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lr/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lr/lr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lr/lr_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.911524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/rf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/rf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.911524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/rf/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/rf/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/rf/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/rf/compilers/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/rf/rf_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36291 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/rf/rf_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/rf/rf_rapids_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.911524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.911524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/modified_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/pretexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/tab_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.911524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.911524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/compilers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.915524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.915524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33156 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.915524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35716 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.915524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/text_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/text_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.915524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/vowpalwabbit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/vowpalwabbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.915524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/xgboost/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.915524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/xgboost/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/xgboost/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/xgboost/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/xgboost/xgboost_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.915524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/xt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/xt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/xt/xt_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.915524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   251243 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/predictor/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.919524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.919524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/trainer/model_presets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/trainer/model_presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/trainer/model_presets/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/trainer/model_presets/presets_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/trainer/model_presets/presets_distill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.919524 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-31 09:03:45.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/tuning/feature_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-31 09:04:16.000000 autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:16.903524 autogluon.tabular-0.7.1b20230531/src/autogluon.tabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-05-31 09:04:16.000000 autogluon.tabular-0.7.1b20230531/src/autogluon.tabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-05-31 09:04:16.000000 autogluon.tabular-0.7.1b20230531/src/autogluon.tabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:04:16.000000 autogluon.tabular-0.7.1b20230531/src/autogluon.tabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 09:04:16.000000 autogluon.tabular-0.7.1b20230531/src/autogluon.tabular.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-31 09:04:16.000000 autogluon.tabular-0.7.1b20230531/src/autogluon.tabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 09:04:16.000000 autogluon.tabular-0.7.1b20230531/src/autogluon.tabular.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:04:16.000000 autogluon.tabular-0.7.1b20230531/src/autogluon.tabular.egg-info/zip-safe
```

### Comparing `autogluon.tabular-0.7.1b20230530/PKG-INFO` & `autogluon.tabular-0.7.1b20230531/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 0.7.1b20230530
+Version: 0.7.1b20230531
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-0.7.1b20230530/setup.py` & `autogluon.tabular-0.7.1b20230531/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/configs/config_helper.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/configs/config_helper.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/configs/feature_generator_presets.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/configs/feature_generator_presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/configs/hyperparameter_configs.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/configs/hyperparameter_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/configs/presets_configs.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/learner/abstract_learner.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/learner/default_learner.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/learner/default_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/__init__.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/_utils/rapids_utils.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/_utils/rapids_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/_utils/torch_utils.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/_utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/automm/automm_model.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/automm/automm_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/automm/ft_transformer.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/automm/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/catboost/callbacks.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/catboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/catboost/catboost_model.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/catboost/catboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/catboost/catboost_softclass_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/catboost/catboost_utils.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/catboost/catboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/catboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/catboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fastainn/callbacks.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fastainn/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fastainn/fastai_helpers.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fastainn/fastai_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fastainn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fastainn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fastainn/quantile_helpers.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fastainn/quantile_helpers.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fastainn/tabular_nn_fastai.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fasttext/fasttext_model.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fasttext/fasttext_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/fasttext/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/image_prediction/image_predictor.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/image_prediction/image_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/imodels/imodels_models.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/imodels/imodels_models.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/knn/_knn_loo_variants.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/knn/_knn_loo_variants.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/knn/knn_model.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/knn/knn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/knn/knn_rapids_model.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/knn/knn_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/knn/knn_utils.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/knn/knn_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lgb/callbacks.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lgb/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lgb/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lgb/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lgb/lgb_model.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lgb/lgb_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lgb/lgb_utils.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lgb/lgb_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lr/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lr/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lr/lr_model.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lr/lr_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lr/lr_preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/lr/lr_rapids_model.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/lr/lr_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/rf/compilers/native.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/rf/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/rf/compilers/onnx.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/rf/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/rf/rf_model.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/rf/rf_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/rf/rf_quantile.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/rf/rf_quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/rf/rf_rapids_model.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/rf/rf_rapids_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/modified_transformer.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/modified_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/pretexts.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/pretexts.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/tab_model_base.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/tab_model_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/tab_transformer.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/tab_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/tab_transformer_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tab_transformer/utils.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tab_transformer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/compilers/native.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/compilers/native.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/compilers/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/torch/tabular_nn_torch.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/torch/tabular_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/torch/torch_network_modules.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/utils/categorical_encoders.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/utils/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/tabular_nn/utils/nn_architecture_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/text_prediction/text_prediction_v1_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/vowpalwabbit/vowpalwabbit_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/xgboost/callbacks.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/xgboost/callbacks.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/xgboost/hyperparameters/parameters.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/xgboost/hyperparameters/searchspaces.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/xgboost/xgboost_model.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/xgboost/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/xgboost/xgboost_utils.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/xgboost/xgboost_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/models/xt/xt_model.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/models/xt/xt_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/predictor/predictor.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/predictor/predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import inspect
 import logging
 import math
 import os
 import pprint
 import shutil
 import time
-from typing import Union, List, Tuple
+from typing import Union, List, Tuple, Optional
 import warnings
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 
 from autogluon.common.loaders import load_json
 from autogluon.common.savers import save_json
 from autogluon.common.utils.file_utils import get_directory_size, get_directory_size_per_file
-from autogluon.common.utils.log_utils import set_logger_verbosity
+from autogluon.common.utils.log_utils import add_log_to_file, set_logger_verbosity
 from autogluon.common.utils.pandas_utils import get_approximate_df_mem_usage
 from autogluon.common.utils.utils import setup_outputdir, get_autogluon_metadata, compare_autogluon_metadata, check_saved_predictor_version
 from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, QUANTILE, AUTO_WEIGHT, BALANCE_WEIGHT, PSEUDO_MODEL_SUFFIX, PROBLEM_TYPES_CLASSIFICATION
 from autogluon.core.data.label_cleaner import LabelCleanerMulticlassToBinary
 from autogluon.core.dataset import TabularDataset
 from autogluon.core.problem_type import problem_type_info
 from autogluon.core.pseudolabeling.pseudolabeling import filter_pseudo, filter_ensemble_pseudo
@@ -97,14 +97,20 @@
         where `L` ranges from 0 to 50 (Note: higher values of `L` correspond to fewer print statements, opposite of verbosity levels).
         Verbosity levels:
             0: Only log exceptions
             1: Only log warnings + exceptions
             2: Standard logging
             3: Verbose logging (ex: log validation score every 50 iterations)
             4: Maximally verbose logging (ex: log validation score every iteration)
+    log_to_file: bool, default = True
+        Whether to save the logs into a file for later reference
+    log_file_path: str, default = "auto"
+        File path to save the logs.
+        If auto, logs will be saved under `predictor_path/logs/predictor_log.txt`.
+        Will be ignored if `log_to_file` is set to False
     sample_weight : str, default = None
         If specified, this column-name indicates which column of the data should be treated as sample weights. This column will NOT be considered as a predictive feature.
         Sample weights should be non-negative (and cannot be nan), with larger values indicating which rows are more important than others.
         If you want your usage of sample weights to match results obtained outside of this Predictor, then ensure sample weights for your training (or tuning) data sum to the number of rows in the training (or tuning) data.
         You may also specify two special strings: 'auto_weight' (automatically choose a weighting strategy based on the data) or 'balance_weight' (equally weight classes in classification, no effect in regression). If specifying your own sample_weight column, make sure its name does not match these special strings.
     weight_evaluation : bool, default = False
         Only considered when `sample_weight` column is not None. Determines whether sample weights should be taken into account when computing evaluation metrics on validation/test data.
@@ -189,22 +195,25 @@
             This indicates that the internal models will never predict those missing labels, and training rows associated with the missing labels were dropped.
     """
 
     Dataset = TabularDataset
     predictor_file_name = 'predictor.pkl'
     _predictor_version_file_name = '__version__'
     _predictor_metadata_file_name = 'metadata.json'
+    _predictor_log_file_name = 'predictor_log.txt'
 
     def __init__(
             self,
             label,
             problem_type=None,
             eval_metric=None,
             path=None,
             verbosity=2,
+            log_to_file=False,
+            log_file_path='auto',
             sample_weight=None,
             weight_evaluation=False,
             groups=None,
             **kwargs
     ):
         self.verbosity = verbosity
         set_logger_verbosity(self.verbosity)
@@ -214,14 +223,19 @@
         self.sample_weight = sample_weight
         self.weight_evaluation = weight_evaluation  # TODO: sample_weight and weight_evaluation can both be properties that link to self._learner.sample_weight, self._learner.weight_evaluation
         if self.sample_weight in [AUTO_WEIGHT, BALANCE_WEIGHT] and self.weight_evaluation:
             logger.warning(
                 f"We do not recommend specifying weight_evaluation when sample_weight='{self.sample_weight}', instead specify appropriate eval_metric.")
         self._validate_init_kwargs(kwargs)
         path = setup_outputdir(path)
+        self._setup_log_to_file(
+            path=path,
+            log_to_file=log_to_file,
+            log_file_path=log_file_path
+        )
 
         learner_type = kwargs.pop('learner_type', DefaultLearner)
         learner_kwargs = kwargs.pop('learner_kwargs', dict())
         quantile_levels = kwargs.get('quantile_levels', None)
 
         self._learner: AbstractTabularLearner = learner_type(path_context=path, label=label, feature_generator=None,
                                                              eval_metric=eval_metric, problem_type=problem_type,
@@ -3207,14 +3221,51 @@
                         f'Please ensure the versions match to avoid instability. While it is NOT recommended, '
                         f'this error can be bypassed by specifying `require_py_version_match=False`.')
 
         if predictor is None:
             predictor = cls._load(path=path)
 
         return predictor
+    
+    @classmethod
+    def load_log(cls, predictor_path: str = None, log_file_path: Optional[str] = None) -> List[str]:
+        """
+        Load log files of a predictor
+        
+        Parameters
+        ----------
+        predictor_path: Optional[str], default = None
+            Path to the predictor to load the log.
+            This can be used when the predictor was initialized with `log_file_path="auto"` to fetch the log file automatically
+        log_file_path: Optional[str], default = None
+            Path to the log file.
+            If you specified a `log_file_path` while initializing the predictor, you should use `log_file_path` to load the log file instead.
+            At least one of `predictor_path` or `log_file_path` must to be specified
+            
+        Return
+        ------
+        List[str]
+            A list containing lines of the log file
+        """
+        file_path = log_file_path
+        if file_path is None:
+            assert predictor_path is not None, "Please either provide `predictor_path` or `log_file_path` to load the log file"
+            file_path = os.path.join(predictor_path, "logs", cls._predictor_log_file_name)
+        assert os.path.isfile(file_path), f"Log file does not exist at {file_path}"
+        with open(file_path, "r") as f:
+            lines = f.readlines()
+        return lines
+    
+    def _setup_log_to_file(self, path, log_to_file, log_file_path):
+        if log_to_file:
+            if log_file_path == "auto":
+                log_file_path = os.path.join(path, "logs", self._predictor_log_file_name)
+            log_file_path = os.path.abspath(os.path.normpath(log_file_path))
+            os.makedirs(os.path.dirname(log_file_path), exist_ok=True)
+            add_log_to_file(log_file_path)
 
     @staticmethod
     def _validate_init_kwargs(kwargs):
         valid_kwargs = {
             'learner_type',
             'learner_kwargs',
             'quantile_levels',
```

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/trainer/auto_trainer.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/trainer/model_presets/presets.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/trainer/model_presets/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/trainer/model_presets/presets_custom.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/trainer/model_presets/presets_custom.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/trainer/model_presets/presets_distill.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/trainer/model_presets/presets_distill.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon/tabular/tuning/feature_pruner.py` & `autogluon.tabular-0.7.1b20230531/src/autogluon/tabular/tuning/feature_pruner.py`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon.tabular.egg-info/PKG-INFO` & `autogluon.tabular-0.7.1b20230531/src/autogluon.tabular.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.tabular
-Version: 0.7.1b20230530
+Version: 0.7.1b20230531
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon.tabular.egg-info/SOURCES.txt` & `autogluon.tabular-0.7.1b20230531/src/autogluon.tabular.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.tabular-0.7.1b20230530/src/autogluon.tabular.egg-info/requires.txt` & `autogluon.tabular-0.7.1b20230531/src/autogluon.tabular.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 numpy<1.27,>=1.21
 scipy<1.12,>=1.5.4
 pandas<1.6,>=1.4.1
 scikit-learn<1.3,>=1.0
 networkx<3.0,>=2.3
-autogluon.core==0.7.1b20230530
-autogluon.features==0.7.1b20230530
+autogluon.core==0.7.1b20230531
+autogluon.features==0.7.1b20230531
 
 [all]
-lightgbm<3.4,>=3.3
 torch<1.14,>=1.9
-catboost<1.2,>=1.1
-autogluon.core[all]==0.7.1b20230530
-xgboost<1.8,>=1.6
+autogluon.core[all]==0.7.1b20230531
 fastai<2.8,>=2.3.1
+xgboost<1.8,>=1.6
+catboost<1.2,>=1.1
+lightgbm<3.4,>=3.3
 
 [catboost]
 catboost<1.2,>=1.1
 
 [fastai]
 torch<1.14,>=1.9
 fastai<2.8,>=2.3.1
@@ -24,15 +24,15 @@
 [imodels]
 imodels<1.4.0,>=1.3.10
 
 [lightgbm]
 lightgbm<3.4,>=3.3
 
 [ray]
-autogluon.core[all]==0.7.1b20230530
+autogluon.core[all]==0.7.1b20230531
 
 [skex]
 scikit-learn-intelex<2023.1,>=2021.7
 
 [skl2onnx]
 skl2onnx<1.14.0,>=1.13.0
 onnxruntime-gpu<1.14.0,>=1.13.0
```

