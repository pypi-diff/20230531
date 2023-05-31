# Comparing `tmp/pytorch_tabular-1.0.1.tar.gz` & `tmp/pytorch_tabular-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_tabular-1.0.1.tar", last modified: Fri Jan 20 12:08:41 2023, max compression
+gzip compressed data, was "pytorch_tabular-1.0.2.tar", last modified: Wed May 31 02:25:14 2023, max compression
```

## Comparing `pytorch_tabular-1.0.1.tar` & `pytorch_tabular-1.0.2.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.118989 pytorch_tabular-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    18468 2023-01-20 12:08:41.118989 pytorch_tabular-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11423 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.106989 pytorch_tabular-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/apidocs_common.md
--rw-r--r--   0 runner    (1001) docker     (122)      936 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/apidocs_config.md
--rw-r--r--   0 runner    (1001) docker     (122)      171 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/apidocs_coreclasses.md
--rw-r--r--   0 runner    (1001) docker     (122)      444 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/apidocs_head.md
--rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/apidocs_model.md
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/apidocs_ssl.md
--rw-r--r--   0 runner    (1001) docker     (122)      965 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/apidocs_utils.md
--rw-r--r--   0 runner    (1001) docker     (122)      399 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (122)     4002 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/data.md
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/development_manual.md
--rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/experiment_tracking.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (122)     3387 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/history.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.110988 pytorch_tabular-1.0.1/docs/imgs/
--rw-r--r--   0 runner    (1001) docker     (122)   149093 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/imgs/auto_encoder.png
--rw-r--r--   0 runner    (1001) docker     (122)   194693 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/imgs/dndt.png
--rw-r--r--   0 runner    (1001) docker     (122)    68818 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/imgs/gflu.png
--rw-r--r--   0 runner    (1001) docker     (122)    44298 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/imgs/gradient_histograms.png
--rw-r--r--   0 runner    (1001) docker     (122)    58842 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/imgs/gradient_norms.png
--rw-r--r--   0 runner    (1001) docker     (122)    11063 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/imgs/log_logits.png
--rw-r--r--   0 runner    (1001) docker     (122)    75062 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/imgs/node_arch.png
--rw-r--r--   0 runner    (1001) docker     (122)    90805 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/imgs/node_dense_arch.png
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/imgs/pytorch_tabular_logo.png
--rw-r--r--   0 runner    (1001) docker     (122)     4123 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/imgs/pytorch_tabular_logo_small_2.png
--rw-r--r--   0 runner    (1001) docker     (122)   110622 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/imgs/tabnet_architecture.png
--rw-r--r--   0 runner    (1001) docker     (122)     4365 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (122)    18387 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/models.md
--rw-r--r--   0 runner    (1001) docker     (122)     2117 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/optimizer.md
--rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/other_features.md
--rw-r--r--   0 runner    (1001) docker     (122)     8805 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/ssl_models.md
--rw-r--r--   0 runner    (1001) docker     (122)     7084 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tabular_model.md
--rw-r--r--   0 runner    (1001) docker     (122)     6534 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/training.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.102989 pytorch_tabular-1.0.1/docs/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.110988 pytorch_tabular-1.0.1/docs/tutorials/imgs/
--rw-r--r--   0 runner    (1001) docker     (122)     8783 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_eq_1.png
--rw-r--r--   0 runner    (1001) docker     (122)     7095 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_eq_2.png
--rw-r--r--   0 runner    (1001) docker     (122)    39984 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_fig_1.png
--rw-r--r--   0 runner    (1001) docker     (122)    43281 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_fig_2.png
--rw-r--r--   0 runner    (1001) docker     (122)    31733 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_fig_3.png
--rw-r--r--   0 runner    (1001) docker     (122)    21468 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_hist_1.png
--rw-r--r--   0 runner    (1001) docker     (122)    23471 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_hist_2.png
--rw-r--r--   0 runner    (1001) docker     (122)    22868 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_hist_3.png
--rw-r--r--   0 runner    (1001) docker     (122)    21969 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_hist_4.png
--rw-r--r--   0 runner    (1001) docker     (122)    50988 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_mdn_1.png
--rw-r--r--   0 runner    (1001) docker     (122)   116055 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_mdn_2.png
--rw-r--r--   0 runner    (1001) docker     (122)   100692 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_mdn_3.png
--rw-r--r--   0 runner    (1001) docker     (122)    32401 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_mixing12_3.png
--rw-r--r--   0 runner    (1001) docker     (122)   101714 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_mixing1_3.png
--rw-r--r--   0 runner    (1001) docker     (122)    86139 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_mixing2_3.png
--rw-r--r--   0 runner    (1001) docker     (122)    58362 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_non_mdn_2.png
--rw-r--r--   0 runner    (1001) docker     (122)    61311 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_non_mdn_3.png
--rw-r--r--   0 runner    (1001) docker     (122)    51641 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_pdfs_4.png
--rw-r--r--   0 runner    (1001) docker     (122)   141320 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/docs/tutorials/imgs/wandb_preview.png
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/requirements_extra.txt
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-01-20 12:08:41.118989 pytorch_tabular-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.106989 pytorch_tabular-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.114989 pytorch_tabular-1.0.1/src/pytorch_tabular/
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10093 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/categorical_encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.114989 pytorch_tabular-1.0.1/src/pytorch_tabular/config/
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    41887 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/config/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     4189 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/feature_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.114989 pytorch_tabular-1.0.1/src/pytorch_tabular/models/
--rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.114989 pytorch_tabular-1.0.1/src/pytorch_tabular/models/autoint/
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/autoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5169 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/autoint/autoint.py
--rw-r--r--   0 runner    (1001) docker     (122)    10258 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/autoint/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    22350 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.114989 pytorch_tabular-1.0.1/src/pytorch_tabular/models/category_embedding/
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/category_embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2621 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/category_embedding/category_embedding_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5234 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/category_embedding/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.114989 pytorch_tabular-1.0.1/src/pytorch_tabular/models/common/
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6989 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/common/activations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.114989 pytorch_tabular-1.0.1/src/pytorch_tabular/models/common/heads/
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/common/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6691 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/common/heads/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     7922 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/common/heads/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    23238 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/common/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)      898 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.114989 pytorch_tabular-1.0.1/src/pytorch_tabular/models/ft_transformer/
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/ft_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12865 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/ft_transformer/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6707 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/ft_transformer/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.114989 pytorch_tabular-1.0.1/src/pytorch_tabular/models/gate/
--rw-r--r--   0 runner    (1001) docker     (122)      261 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/gate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6318 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/gate/components.py
--rw-r--r--   0 runner    (1001) docker     (122)     6445 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/gate/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     8707 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/gate/gate_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.114989 pytorch_tabular-1.0.1/src/pytorch_tabular/models/mixture_density/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/mixture_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4018 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/mixture_density/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    10168 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/mixture_density/mdn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.118989 pytorch_tabular-1.0.1/src/pytorch_tabular/models/node/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2170 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/node/architecture_blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)    12528 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/node/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5232 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/node/node_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     8851 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/node/odst.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.118989 pytorch_tabular-1.0.1/src/pytorch_tabular/models/tab_transformer/
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/tab_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12435 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/tab_transformer/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5591 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/tab_transformer/tab_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.118989 pytorch_tabular-1.0.1/src/pytorch_tabular/models/tabnet/
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/tabnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5018 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/tabnet/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2878 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/models/tabnet/tabnet_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.118989 pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8200 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.118989 pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/common/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1683 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/common/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/common/heads.py
--rw-r--r--   0 runner    (1001) docker     (122)     4998 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/common/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/common/noise_generators.py
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/common/ssl_losses.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/common/ssl_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.118989 pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/dae/
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/dae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6135 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/dae/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     9334 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/dae/dae.py
--rw-r--r--   0 runner    (1001) docker     (122)    28270 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/tabular_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)    63268 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/tabular_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     7432 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/src/pytorch_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.114989 pytorch_tabular-1.0.1/src/pytorch_tabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    18468 2023-01-20 12:08:40.000000 pytorch_tabular-1.0.1/src/pytorch_tabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4917 2023-01-20 12:08:41.000000 pytorch_tabular-1.0.1/src/pytorch_tabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-20 12:08:40.000000 pytorch_tabular-1.0.1/src/pytorch_tabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-20 12:08:40.000000 pytorch_tabular-1.0.1/src/pytorch_tabular.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-01-20 12:08:40.000000 pytorch_tabular-1.0.1/src/pytorch_tabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-01-20 12:08:40.000000 pytorch_tabular-1.0.1/src/pytorch_tabular.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-20 12:08:41.118989 pytorch_tabular-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      979 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/tests/___test_augmentations.py
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     7665 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/tests/test_autoint.py
--rw-r--r--   0 runner    (1001) docker     (122)     7422 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/tests/test_categorical_embedding.py
--rw-r--r--   0 runner    (1001) docker     (122)    12458 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/tests/test_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (122)     6176 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/tests/test_ft_transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6373 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/tests/test_gate.py
--rw-r--r--   0 runner    (1001) docker     (122)     4655 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/tests/test_mdn.py
--rw-r--r--   0 runner    (1001) docker     (122)     6279 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (122)     8117 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (122)     4411 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/tests/test_tabnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     6176 2023-01-20 12:08:34.000000 pytorch_tabular-1.0.1/tests/test_tabtransformer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.651765 pytorch_tabular-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    20223 2023-05-31 02:25:14.651765 pytorch_tabular-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11626 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.639765 pytorch_tabular-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     2214 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/apidocs_common.md
+-rw-r--r--   0 runner    (1001) docker     (122)      936 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/apidocs_config.md
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/apidocs_coreclasses.md
+-rw-r--r--   0 runner    (1001) docker     (122)      444 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/apidocs_head.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/apidocs_model.md
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/apidocs_ssl.md
+-rw-r--r--   0 runner    (1001) docker     (122)      965 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/apidocs_utils.md
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (122)     4001 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/data.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/development_manual.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/experiment_tracking.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (122)     4683 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/history.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.643765 pytorch_tabular-1.0.2/docs/imgs/
+-rw-r--r--   0 runner    (1001) docker     (122)   149093 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/imgs/auto_encoder.png
+-rw-r--r--   0 runner    (1001) docker     (122)   194693 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/imgs/dndt.png
+-rw-r--r--   0 runner    (1001) docker     (122)    68818 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/imgs/gflu.png
+-rw-r--r--   0 runner    (1001) docker     (122)    44298 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/imgs/gradient_histograms.png
+-rw-r--r--   0 runner    (1001) docker     (122)    58842 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/imgs/gradient_norms.png
+-rw-r--r--   0 runner    (1001) docker     (122)    11063 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/imgs/log_logits.png
+-rw-r--r--   0 runner    (1001) docker     (122)    75062 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/imgs/node_arch.png
+-rw-r--r--   0 runner    (1001) docker     (122)    90805 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/imgs/node_dense_arch.png
+-rw-r--r--   0 runner    (1001) docker     (122)    13069 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/imgs/pytorch_tabular_logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4123 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/imgs/pytorch_tabular_logo_small_2.png
+-rw-r--r--   0 runner    (1001) docker     (122)   110622 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/imgs/tabnet_architecture.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4365 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)    18387 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/models.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2117 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/optimizer.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/other_features.md
+-rw-r--r--   0 runner    (1001) docker     (122)     8805 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/ssl_models.md
+-rw-r--r--   0 runner    (1001) docker     (122)     7084 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tabular_model.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6534 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/training.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.635765 pytorch_tabular-1.0.2/docs/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.643765 pytorch_tabular-1.0.2/docs/tutorials/imgs/
+-rw-r--r--   0 runner    (1001) docker     (122)     8783 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_eq_1.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7095 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_eq_2.png
+-rw-r--r--   0 runner    (1001) docker     (122)    39984 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_fig_1.png
+-rw-r--r--   0 runner    (1001) docker     (122)    43281 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_fig_2.png
+-rw-r--r--   0 runner    (1001) docker     (122)    31733 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_fig_3.png
+-rw-r--r--   0 runner    (1001) docker     (122)    21468 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_hist_1.png
+-rw-r--r--   0 runner    (1001) docker     (122)    23471 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_hist_2.png
+-rw-r--r--   0 runner    (1001) docker     (122)    22868 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_hist_3.png
+-rw-r--r--   0 runner    (1001) docker     (122)    21969 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_hist_4.png
+-rw-r--r--   0 runner    (1001) docker     (122)    50988 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_mdn_1.png
+-rw-r--r--   0 runner    (1001) docker     (122)   116055 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_mdn_2.png
+-rw-r--r--   0 runner    (1001) docker     (122)   100692 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_mdn_3.png
+-rw-r--r--   0 runner    (1001) docker     (122)    32401 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_mixing12_3.png
+-rw-r--r--   0 runner    (1001) docker     (122)   101714 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_mixing1_3.png
+-rw-r--r--   0 runner    (1001) docker     (122)    86139 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_mixing2_3.png
+-rw-r--r--   0 runner    (1001) docker     (122)    58362 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_non_mdn_2.png
+-rw-r--r--   0 runner    (1001) docker     (122)    61311 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_non_mdn_3.png
+-rw-r--r--   0 runner    (1001) docker     (122)    51641 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_pdfs_4.png
+-rw-r--r--   0 runner    (1001) docker     (122)   141320 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/docs/tutorials/imgs/wandb_preview.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/requirements_extra.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-05-31 02:25:14.655765 pytorch_tabular-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.635765 pytorch_tabular-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.647765 pytorch_tabular-1.0.2/src/pytorch_tabular/
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10022 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/categorical_encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.647765 pytorch_tabular-1.0.2/src/pytorch_tabular/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43762 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4208 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/feature_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.647765 pytorch_tabular-1.0.2/src/pytorch_tabular/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.647765 pytorch_tabular-1.0.2/src/pytorch_tabular/models/autoint/
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/autoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4836 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/autoint/autoint.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10737 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/autoint/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23200 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.647765 pytorch_tabular-1.0.2/src/pytorch_tabular/models/category_embedding/
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/category_embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2622 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/category_embedding/category_embedding_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5785 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/category_embedding/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.647765 pytorch_tabular-1.0.2/src/pytorch_tabular/models/common/
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6961 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/common/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.647765 pytorch_tabular-1.0.2/src/pytorch_tabular/models/common/heads/
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/common/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/common/heads/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8062 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/common/heads/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23093 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/common/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.647765 pytorch_tabular-1.0.2/src/pytorch_tabular/models/ft_transformer/
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/ft_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13671 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/ft_transformer/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6153 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/ft_transformer/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.647765 pytorch_tabular-1.0.2/src/pytorch_tabular/models/gate/
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/gate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/gate/components.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6949 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/gate/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9211 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/gate/gate_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.647765 pytorch_tabular-1.0.2/src/pytorch_tabular/models/mixture_density/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/mixture_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4509 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/mixture_density/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10193 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/mixture_density/mdn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.651765 pytorch_tabular-1.0.2/src/pytorch_tabular/models/node/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/node/architecture_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13166 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/node/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4852 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/node/node_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8846 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/node/odst.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.651765 pytorch_tabular-1.0.2/src/pytorch_tabular/models/tab_transformer/
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/tab_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13225 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/tab_transformer/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5338 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/tab_transformer/tab_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.651765 pytorch_tabular-1.0.2/src/pytorch_tabular/models/tabnet/
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/tabnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5494 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/tabnet/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/models/tabnet/tabnet_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.651765 pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8071 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.651765 pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/common/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1686 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/common/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1453 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/common/heads.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4957 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/common/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/common/noise_generators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/common/ssl_losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/common/ssl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.651765 pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/dae/
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/dae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6299 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/dae/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9334 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/dae/dae.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28398 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/tabular_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (122)    65877 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/tabular_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7514 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/src/pytorch_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.647765 pytorch_tabular-1.0.2/src/pytorch_tabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    20223 2023-05-31 02:25:14.000000 pytorch_tabular-1.0.2/src/pytorch_tabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4917 2023-05-31 02:25:14.000000 pytorch_tabular-1.0.2/src/pytorch_tabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 02:25:14.000000 pytorch_tabular-1.0.2/src/pytorch_tabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 02:25:14.000000 pytorch_tabular-1.0.2/src/pytorch_tabular.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-05-31 02:25:14.000000 pytorch_tabular-1.0.2/src/pytorch_tabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-31 02:25:14.000000 pytorch_tabular-1.0.2/src/pytorch_tabular.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 02:25:14.651765 pytorch_tabular-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      979 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/tests/___test_augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7663 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/tests/test_autoint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7523 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/tests/test_categorical_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12746 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5585 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/tests/test_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6198 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/tests/test_ft_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6389 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/tests/test_gate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4649 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/tests/test_mdn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6301 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8207 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4394 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/tests/test_tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6198 2023-05-31 02:25:00.000000 pytorch_tabular-1.0.2/tests/test_tabtransformer.py
```

### Comparing `pytorch_tabular-1.0.1/LICENSE` & `pytorch_tabular-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/PKG-INFO` & `pytorch_tabular-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch_tabular
-Version: 1.0.1
+Version: 1.0.2
 Summary: A standard framework for using Deep Learning for tabular data
 Home-page: https://github.com/manujosephv/pytorch_tabular
 Author: Manu Joseph
 Author-email: manujosephv@gmail.com
 License: MIT license
 Description: ![PyTorch Tabular](docs/imgs/pytorch_tabular_logo.png)
         
@@ -141,45 +141,45 @@
         - [PyTorch Tabular – A Framework for Deep Learning for Tabular Data](https://deep-and-shallow.com/2021/01/27/pytorch-tabular-a-framework-for-deep-learning-for-tabular-data/)
         - [Neural Oblivious Decision Ensembles(NODE) – A State-of-the-Art Deep Learning Algorithm for Tabular Data](https://deep-and-shallow.com/2021/02/25/neural-oblivious-decision-ensemblesnode-a-state-of-the-art-deep-learning-algorithm-for-tabular-data/)
         - [Mixture Density Networks: Probabilistic Regression for Uncertainty Estimation](https://deep-and-shallow.com/2021/03/20/mixture-density-networks-probabilistic-regression-for-uncertainty-estimation/)
         
         ## Future Roadmap(Contributions are Welcome)
         
         1. Integrate Optuna Hyperparameter Tuning
-        1. Integrate SHAP for interpretability
-        1. Add Variable Importance
-        1. Add ability to use custom activations in CategoryEmbeddingModel
+        1. Integrate Captum for interpretability
+        1. Have a scikit-learn compatible API
         1. Add GaussRank as Feature Transformation
-        1. ~~Add differential dropouts(layer-wise) in CategoryEmbeddingModel~~
-        1. ~~Add Fourier Encoding for cyclic time variables~~
-        1. ~~Add Text and Image Modalities for mixed modal problems~~
+        1. Enable support for multi-label classification
+        1. Migrate Datamodule to Polars or Vaex for faster data loading and to handle larger than RAM datasets.
+        1. Keep adding more architectures
         
         ## Contributors
+        
         <!-- readme: contributors -start -->
         <table>
         <tr>
             <td align="center">
                 <a href="https://github.com/manujosephv">
                     <img src="https://avatars.githubusercontent.com/u/10508493?v=4" width="100;" alt="manujosephv"/>
                     <br />
                     <sub><b>Manu Joseph</b></sub>
                 </a>
             </td>
             <td align="center">
-                <a href="https://github.com/wsad1">
-                    <img src="https://avatars.githubusercontent.com/u/13963626?v=4" width="100;" alt="wsad1"/>
+                <a href="https://github.com/Borda">
+                    <img src="https://avatars.githubusercontent.com/u/6035284?v=4" width="100;" alt="Borda"/>
                     <br />
-                    <sub><b>Jinu Sunil</b></sub>
+                    <sub><b>Jirka Borovec</b></sub>
                 </a>
             </td>
             <td align="center">
-                <a href="https://github.com/Borda">
-                    <img src="https://avatars.githubusercontent.com/u/6035284?v=4" width="100;" alt="Borda"/>
+                <a href="https://github.com/wsad1">
+                    <img src="https://avatars.githubusercontent.com/u/13963626?v=4" width="100;" alt="wsad1"/>
                     <br />
-                    <sub><b>Jirka Borovec</b></sub>
+                    <sub><b>Jinu Sunil</b></sub>
                 </a>
             </td>
             <td align="center">
                 <a href="https://github.com/fonnesbeck">
                     <img src="https://avatars.githubusercontent.com/u/81476?v=4" width="100;" alt="fonnesbeck"/>
                     <br />
                     <sub><b>Chris Fonnesbeck</b></sub>
@@ -254,30 +254,62 @@
               primaryClass={cs.LG}
         }
         ```
         
         - Zenodo Software Citation
         
         ```
-        @article{manujosephv_2021,
-            title={manujosephv/pytorch_tabular: v0.7.0-alpha},
-            DOI={10.5281/zenodo.5359010},
-            abstractNote={<p>Added a few more SOTA models - TabTransformer, FTTransformer
-                Made improvements in the model save and load capability
-                Made installation less restrictive by unfreezing some dependencies.</p>},
-            publisher={Zenodo},
-            author={manujosephv},
-            year={2021},
-            month={May}
+        @software{manu_joseph_2023_7554473,
+          author       = {Manu Joseph and
+                          Jinu Sunil and
+                          Jiri Borovec and
+                          Chris Fonnesbeck and
+                          jxtrbtk and
+                          Andreas and
+                          JulianRein and
+                          Kushashwa Ravi Shrimali and
+                          Luca Actis Grosso and
+                          Sterling G. Baird and
+                          Yinyu Nie},
+          title        = {manujosephv/pytorch\_tabular: v1.0.1},
+          month        = jan,
+          year         = 2023,
+          publisher    = {Zenodo},
+          version      = {v1.0.1},
+          doi          = {10.5281/zenodo.7554473},
+          url          = {https://doi.org/10.5281/zenodo.7554473}
         }
         ```
         
         
         # History
         
+        ## 1.0.2 (2023-05-31)
+        
+        ### New Features:
+        
+        - Added Feature Importance: The library now includes a new method in TabularModel and BaseModel for enabling feature importance. Feature Importance has been enabled for FTTransformer and GATE models. [Commit: dc2a49e]
+        ### Enhancements:
+        
+        - Enabled two more parameters in the GATE model. [Commit: 3680413]
+        - Included metric_prob_input parameter in the library configuration. This update allows for better control over metrics in the models. [Commit: 0612db5]
+        - Slight improvements to the GATE model, including changes to defaults for better performance. [Commit: c30a6c3]
+        - Minor bug fixes and improvements, including accelerator options in the configuration and progress bar enhancements. [Commit: f932230, bdd9adb, f932230]
+        ### Dependency Updates:
+        
+        - Updated dependencies, including docformatter, pyupgrade, and ruff-pre-commit. [Commits: 4aae9a8, b3df4ce, bdd9adb, 55e800c, c6c4679, c01154b, 107cd2f]
+        ### Documentation Updates:
+        
+        - Updated the library's README.md file. [Commits: db8f3b2, cab6bf1, 669faec, 1e6c400, 3097799, 7fabf6b]
+        ### Other Improvements:
+        
+        - Various code optimizations, bug fixes, and CI enhancements. [Commits: 5637020, e5171bf, 812b40f]
+        
+        For more details, you can refer to the respective commits on the library's GitHub repository.
+        
         ## 1.0.1 (2023-01-20)
         
         - Bugfix for default metric for binary classification
```

### Comparing `pytorch_tabular-1.0.1/README.md` & `pytorch_tabular-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -133,45 +133,45 @@
 - [PyTorch Tabular – A Framework for Deep Learning for Tabular Data](https://deep-and-shallow.com/2021/01/27/pytorch-tabular-a-framework-for-deep-learning-for-tabular-data/)
 - [Neural Oblivious Decision Ensembles(NODE) – A State-of-the-Art Deep Learning Algorithm for Tabular Data](https://deep-and-shallow.com/2021/02/25/neural-oblivious-decision-ensemblesnode-a-state-of-the-art-deep-learning-algorithm-for-tabular-data/)
 - [Mixture Density Networks: Probabilistic Regression for Uncertainty Estimation](https://deep-and-shallow.com/2021/03/20/mixture-density-networks-probabilistic-regression-for-uncertainty-estimation/)
 
 ## Future Roadmap(Contributions are Welcome)
 
 1. Integrate Optuna Hyperparameter Tuning
-1. Integrate SHAP for interpretability
-1. Add Variable Importance
-1. Add ability to use custom activations in CategoryEmbeddingModel
+1. Integrate Captum for interpretability
+1. Have a scikit-learn compatible API
 1. Add GaussRank as Feature Transformation
-1. ~~Add differential dropouts(layer-wise) in CategoryEmbeddingModel~~
-1. ~~Add Fourier Encoding for cyclic time variables~~
-1. ~~Add Text and Image Modalities for mixed modal problems~~
+1. Enable support for multi-label classification
+1. Migrate Datamodule to Polars or Vaex for faster data loading and to handle larger than RAM datasets.
+1. Keep adding more architectures
 
 ## Contributors
+
 <!-- readme: contributors -start -->
 <table>
 <tr>
     <td align="center">
         <a href="https://github.com/manujosephv">
             <img src="https://avatars.githubusercontent.com/u/10508493?v=4" width="100;" alt="manujosephv"/>
             <br />
             <sub><b>Manu Joseph</b></sub>
         </a>
     </td>
     <td align="center">
-        <a href="https://github.com/wsad1">
-            <img src="https://avatars.githubusercontent.com/u/13963626?v=4" width="100;" alt="wsad1"/>
+        <a href="https://github.com/Borda">
+            <img src="https://avatars.githubusercontent.com/u/6035284?v=4" width="100;" alt="Borda"/>
             <br />
-            <sub><b>Jinu Sunil</b></sub>
+            <sub><b>Jirka Borovec</b></sub>
         </a>
     </td>
     <td align="center">
-        <a href="https://github.com/Borda">
-            <img src="https://avatars.githubusercontent.com/u/6035284?v=4" width="100;" alt="Borda"/>
+        <a href="https://github.com/wsad1">
+            <img src="https://avatars.githubusercontent.com/u/13963626?v=4" width="100;" alt="wsad1"/>
             <br />
-            <sub><b>Jirka Borovec</b></sub>
+            <sub><b>Jinu Sunil</b></sub>
         </a>
     </td>
     <td align="center">
         <a href="https://github.com/fonnesbeck">
             <img src="https://avatars.githubusercontent.com/u/81476?v=4" width="100;" alt="fonnesbeck"/>
             <br />
             <sub><b>Chris Fonnesbeck</b></sub>
@@ -246,19 +246,28 @@
       primaryClass={cs.LG}
 }
 ```
 
 - Zenodo Software Citation
 
 ```
-@article{manujosephv_2021,
-    title={manujosephv/pytorch_tabular: v0.7.0-alpha},
-    DOI={10.5281/zenodo.5359010},
-    abstractNote={<p>Added a few more SOTA models - TabTransformer, FTTransformer
-        Made improvements in the model save and load capability
-        Made installation less restrictive by unfreezing some dependencies.</p>},
-    publisher={Zenodo},
-    author={manujosephv},
-    year={2021},
-    month={May}
+@software{manu_joseph_2023_7554473,
+  author       = {Manu Joseph and
+                  Jinu Sunil and
+                  Jiri Borovec and
+                  Chris Fonnesbeck and
+                  jxtrbtk and
+                  Andreas and
+                  JulianRein and
+                  Kushashwa Ravi Shrimali and
+                  Luca Actis Grosso and
+                  Sterling G. Baird and
+                  Yinyu Nie},
+  title        = {manujosephv/pytorch\_tabular: v1.0.1},
+  month        = jan,
+  year         = 2023,
+  publisher    = {Zenodo},
+  version      = {v1.0.1},
+  doi          = {10.5281/zenodo.7554473},
+  url          = {https://doi.org/10.5281/zenodo.7554473}
 }
 ```
```

### Comparing `pytorch_tabular-1.0.1/docs/apidocs_common.md` & `pytorch_tabular-1.0.2/docs/apidocs_common.md`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/apidocs_config.md` & `pytorch_tabular-1.0.2/docs/apidocs_config.md`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/apidocs_model.md` & `pytorch_tabular-1.0.2/docs/apidocs_model.md`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/apidocs_utils.md` & `pytorch_tabular-1.0.2/docs/apidocs_utils.md`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/contributing.md` & `pytorch_tabular-1.0.2/docs/contributing.md`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
       ```bash
       pytest tests/
       ```
 !!!note
 
       If you are adding a new feature, please add a test for it.
 
-* When you are done making changes and all test cases are passing, crun `pre-commit` to make sure all the linting and formatting is done correctly.
+* When you are done making changes and all test cases are passing, run `pre-commit` to make sure all the linting and formatting is done correctly.
 
       ```bash
       pre-commit run --all-files
       ```
    Accept the changes if any after reviewing. 
    
 !!!warning
```

### Comparing `pytorch_tabular-1.0.1/docs/data.md` & `pytorch_tabular-1.0.2/docs/data.md`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/development_manual.md` & `pytorch_tabular-1.0.2/docs/development_manual.md`

 * *Files 12% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ## Bump Version(Release)
 
 ```bash
 # Add new Version and changelog to History.md
 # Commit all changes and run
 bump2version --tag release
 # Check if the tag is present
-git tags
+git tag
 # Push the changes to GitHub
 git push origin <tag_name>
 
 ```
 
 - eg: 0.1.1-dev0 to 0.1.1
 - To trigger GitHub Actions to push to PyPi
```

### Comparing `pytorch_tabular-1.0.1/docs/experiment_tracking.md` & `pytorch_tabular-1.0.2/docs/experiment_tracking.md`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/history.md` & `pytorch_tabular-1.0.2/docs/history.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,32 @@
 # History
 
+## 1.0.2 (2023-05-31)
+
+### New Features:
+
+- Added Feature Importance: The library now includes a new method in TabularModel and BaseModel for enabling feature importance. Feature Importance has been enabled for FTTransformer and GATE models. [Commit: dc2a49e]
+### Enhancements:
+
+- Enabled two more parameters in the GATE model. [Commit: 3680413]
+- Included metric_prob_input parameter in the library configuration. This update allows for better control over metrics in the models. [Commit: 0612db5]
+- Slight improvements to the GATE model, including changes to defaults for better performance. [Commit: c30a6c3]
+- Minor bug fixes and improvements, including accelerator options in the configuration and progress bar enhancements. [Commit: f932230, bdd9adb, f932230]
+### Dependency Updates:
+
+- Updated dependencies, including docformatter, pyupgrade, and ruff-pre-commit. [Commits: 4aae9a8, b3df4ce, bdd9adb, 55e800c, c6c4679, c01154b, 107cd2f]
+### Documentation Updates:
+
+- Updated the library's README.md file. [Commits: db8f3b2, cab6bf1, 669faec, 1e6c400, 3097799, 7fabf6b]
+### Other Improvements:
+
+- Various code optimizations, bug fixes, and CI enhancements. [Commits: 5637020, e5171bf, 812b40f]
+
+For more details, you can refer to the respective commits on the library's GitHub repository.
+
 ## 1.0.1 (2023-01-20)
 
 - Bugfix for default metric for binary classification
```

### Comparing `pytorch_tabular-1.0.1/docs/imgs/auto_encoder.png` & `pytorch_tabular-1.0.2/docs/imgs/auto_encoder.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/imgs/dndt.png` & `pytorch_tabular-1.0.2/docs/imgs/dndt.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/imgs/gflu.png` & `pytorch_tabular-1.0.2/docs/imgs/gflu.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/imgs/gradient_histograms.png` & `pytorch_tabular-1.0.2/docs/imgs/gradient_histograms.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/imgs/gradient_norms.png` & `pytorch_tabular-1.0.2/docs/imgs/gradient_norms.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/imgs/log_logits.png` & `pytorch_tabular-1.0.2/docs/imgs/log_logits.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/imgs/node_arch.png` & `pytorch_tabular-1.0.2/docs/imgs/node_arch.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/imgs/node_dense_arch.png` & `pytorch_tabular-1.0.2/docs/imgs/node_dense_arch.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/imgs/pytorch_tabular_logo.png` & `pytorch_tabular-1.0.2/docs/imgs/pytorch_tabular_logo.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/imgs/pytorch_tabular_logo_small_2.png` & `pytorch_tabular-1.0.2/docs/imgs/pytorch_tabular_logo_small_2.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/imgs/tabnet_architecture.png` & `pytorch_tabular-1.0.2/docs/imgs/tabnet_architecture.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/index.md` & `pytorch_tabular-1.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/models.md` & `pytorch_tabular-1.0.2/docs/models.md`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/optimizer.md` & `pytorch_tabular-1.0.2/docs/optimizer.md`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/other_features.md` & `pytorch_tabular-1.0.2/docs/other_features.md`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/ssl_models.md` & `pytorch_tabular-1.0.2/docs/ssl_models.md`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tabular_model.md` & `pytorch_tabular-1.0.2/docs/tabular_model.md`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/training.md` & `pytorch_tabular-1.0.2/docs/training.md`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_eq_1.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_eq_1.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_eq_2.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_eq_2.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_fig_1.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_fig_1.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_fig_2.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_fig_2.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_fig_3.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_fig_3.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_hist_1.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_hist_1.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_hist_2.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_hist_2.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_hist_3.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_hist_3.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_hist_4.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_hist_4.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_mdn_1.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_mdn_1.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_mdn_2.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_mdn_2.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_mdn_3.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_mdn_3.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_mixing12_3.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_mixing12_3.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_mixing1_3.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_mixing1_3.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_mixing2_3.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_mixing2_3.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_non_mdn_2.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_non_mdn_2.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_non_mdn_3.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_non_mdn_3.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/prob_reg_pdfs_4.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/prob_reg_pdfs_4.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/docs/tutorials/imgs/wandb_preview.png` & `pytorch_tabular-1.0.2/docs/tutorials/imgs/wandb_preview.png`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/setup.py` & `pytorch_tabular-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,10 +57,10 @@
     name="pytorch_tabular",
     packages=find_packages(where="src", include=["pytorch_tabular", "pytorch_tabular.*"]),
     package_dir={"": "src"},
     # setup_requires=test_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/manujosephv/pytorch_tabular",
-    version="1.0.1",
+    version="1.0.2",
     zip_safe=False,
 )
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/__init__.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Pytorch Tabular."""
 
 __author__ = """Manu Joseph"""
 __email__ = "manujosephv@gmail.com"
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 from . import models, ssl_models
 from .categorical_encoders import CategoricalEmbeddingTransformer
 from .feature_extractor import DeepFeatureExtractor
 from .tabular_datamodule import TabularDatamodule
 from .tabular_model import TabularModel
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/categorical_encoders.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/categorical_encoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
 # Modified https://github.com/tcassou/mlencoders/blob/master/mlencoders/base_encoder.py to suit NN encoding
-"""Category Encoders"""
-from __future__ import absolute_import, division, print_function, unicode_literals
+"""Category Encoders."""
 
 try:
     import cPickle as pickle
 except ImportError:
     import pickle
 
 import numpy as np
@@ -17,30 +16,31 @@
 
 from pytorch_tabular.utils import get_logger
 
 logger = get_logger(__name__)
 NAN_CATEGORY = 0
 
 
-class BaseEncoder(object):
+class BaseEncoder:
     def __init__(self, cols, handle_unseen, min_samples, imputed, handle_missing):
         self.cols = cols
         self.handle_unseen = handle_unseen
         self.handle_missing = handle_missing
         self.min_samples = max(1, min_samples)
         # In case of unseen value or not enough data to learn the mapping, we use this value for imputation
         self._imputed = imputed
         # dict {str: pandas.DataFrame} column name --> mapping from category (index of df) to value (column of df)
         self._mapping = {}
 
     def transform(self, X):
         """Transform categorical data based on mapping learnt at fitting time.
+
         :param pandas.DataFrame X: DataFrame of features, shape (n_samples, n_features). Must contain columns to encode.
         :return: encoded DataFrame of shape (n_samples, n_features), initial categorical columns are dropped, and
-            replaced with encoded columns. DataFrame passed in argument is unchanged.
+                replaced with encoded columns. DataFrame passed in argument is unchanged.
         :rtype: pandas.DataFrame
         """
         if not self._mapping:
             raise ValueError("`fit` method must be called before `transform`.")
         assert all(c in X.columns for c in self.cols)
         if self.handle_missing == "error":
             assert (
@@ -50,33 +50,34 @@
         for col, mapping in self._mapping.items():
             X_encoded[col] = X_encoded[col].fillna(NAN_CATEGORY).map(mapping["value"])
 
             if self.handle_unseen == "impute":
                 X_encoded[col].fillna(self._imputed, inplace=True)
             elif self.handle_unseen == "error":
                 if np.unique(X_encoded[col]).shape[0] > mapping.shape[0]:
-                    raise ValueError("Unseen categories found in `{}` column.".format(col))
+                    raise ValueError(f"Unseen categories found in `{col}` column.")
 
         return X_encoded
 
     def fit_transform(self, X, y=None):
         """Encode given columns of X according to y, and transform X based on the learnt mapping.
+
         :param pandas.DataFrame X: DataFrame of features, shape (n_samples, n_features). Must contain columns to encode.
         :param pandas.Series y: pandas Series of target values, shape (n_samples,).
             Required only for encoders that need it: TargetEncoder, WeightOfEvidenceEncoder
         :return: encoded DataFrame of shape (n_samples, n_features), initial categorical columns are dropped, and
             replaced with encoded columns. DataFrame passed in argument is unchanged.
         :rtype: pandas.DataFrame
         """
         self.fit(X, y)
         return self.transform(X)
 
     def _input_check(self, name, value, options):
         if value not in options:
-            raise ValueError("Wrong input: {} parameter must be in {}".format(name, options))
+            raise ValueError(f"Wrong input: {name} parameter must be in {options}")
 
     def _before_fit_check(self, X, y):
         # Checking columns to encode
         if self.cols is None:
             self.cols = X.columns
         else:
             assert all(c in X.columns for c in self.cols)
@@ -92,33 +93,33 @@
 
     def load_from_object_file(self, path):
         for k, v in pickle.load(open(path, "rb")).items():
             setattr(self, k, v)
 
 
 class OrdinalEncoder(BaseEncoder):
-    """
-    Target Encoder for categorical features.
-    """
+    """Target Encoder for categorical features."""
 
     def __init__(self, cols=None, handle_unseen="impute", handle_missing="impute"):
-        """Instantiation
+        """Instantiation.
+
         :param [str] cols: list of columns to encode, or None (then all dataset columns will be encoded at fitting time)
         :param str handle_unseen:
             'error'  - raise an error if a category unseen at fitting time is found
             'ignore' - skip unseen categories
             'impute' - impute new categories to a predefined value, which is same as NAN_CATEGORY
         :return: None
         """
         self._input_check("handle_unseen", handle_unseen, ["error", "ignore", "impute"])
         self._input_check("handle_missing", handle_missing, ["error", "impute"])
-        super(OrdinalEncoder, self).__init__(cols, handle_unseen, 1, NAN_CATEGORY, handle_missing)
+        super().__init__(cols, handle_unseen, 1, NAN_CATEGORY, handle_missing)
 
     def fit(self, X, y=None):
         """Label Encode given columns of X.
+
         :param pandas.DataFrame X: DataFrame of features, shape (n_samples, n_features). Must contain columns to encode.
         :return: None
         """
         self._before_fit_check(X, y)
         if self.handle_missing == "error":
             assert (
                 not X[self.cols].isnull().any().any()
@@ -130,19 +131,18 @@
                 .rename(columns={"index": "value"})
             )
             map["value"] += 1
             self._mapping[col] = map.set_index(col)
 
 
 class CategoricalEmbeddingTransformer(BaseEstimator, TransformerMixin):
-
     NAN_CATEGORY = 0
 
     def __init__(self, tabular_model):
-        """Initializes the Transformer and extracts the neural embeddings
+        """Initializes the Transformer and extracts the neural embeddings.
 
         Args:
             tabular_model (TabularModel): The trained TabularModel object
         """
         self._categorical_encoder = tabular_model.datamodule.categorical_encoder
         self.cols = tabular_model.model.hparams.categorical_cols
         # dict {str: np.ndarray} column name --> mapping from category (index of df) to value (column of df)
@@ -151,15 +151,16 @@
         self._extract_embedding(tabular_model.model)
 
     def _extract_embedding(self, model):
         try:
             embedding_layer = model.extract_embedding()
         except ValueError as e:
             logger.error(
-                f"Extracting embedding layer from model received this error: {e}. Some models do not support this feature."
+                f"Extracting embedding layer from model received this error: {e}."
+                f" Some models do not support this feature."
             )
             embedding_layer = None
         if embedding_layer is not None:
             for i, col in enumerate(self.cols):
                 self._mapping[col] = {}
                 embedding = embedding_layer[i]
                 self._mapping[col][self.NAN_CATEGORY] = embedding.weight[0, :].detach().cpu().numpy().ravel()
@@ -171,33 +172,37 @@
                         .numpy()
                         .ravel()
                     )
         else:
             raise ValueError("Passed model doesn't support this feature.")
 
     def fit(self, X, y=None):
-        """Just for compatibility. Does not do anything"""
+        """Just for compatibility.
+
+        Does not do anything
+        """
         return self
 
     def transform(self, X: pd.DataFrame, y=None) -> pd.DataFrame:
-        """Transforms the categorical columns specified to the trained neural embedding from the model
+        """Transforms the categorical columns specified to the trained neural embedding from the model.
 
         Args:
             X (pd.DataFrame): DataFrame of features, shape (n_samples, n_features). Must contain columns to encode.
             y ([type], optional): Only for compatibility. Not used. Defaults to None.
 
         Raises:
             ValueError: [description]
 
         Returns:
             pd.DataFrame: The encoded dataframe
         """
         if not self._mapping:
             raise ValueError(
-                "Passed model should either have an attribute `embeddng_layers` or a method `extract_embedding` defined for `transform`."
+                "Passed model should either have an attribute `embeddng_layers`"
+                " or a method `extract_embedding` defined for `transform`."
             )
         assert all(c in X.columns for c in self.cols)
 
         X_encoded = X.copy(deep=True)
         for col, mapping in track(
             self._mapping.items(),
             description="Encoding the data...",
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/config/config.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/config/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""Config"""
+"""Config."""
 import os
 import re
 import warnings
 from dataclasses import dataclass, field, MISSING
 from typing import Any, Dict, Iterable, List, Optional
 
 from omegaconf import OmegaConf
@@ -32,28 +32,28 @@
         |[-+]?[0-9][0-9_]*(?::[0-5]?[0-9])+\\.[0-9_]*
         |[-+]?\\.(?:inf|Inf|INF)
         |\\.(?:nan|NaN|NAN))$""",
             re.X,
         ),
         list("-+0123456789."),
     )
-    with open(filename, "r") as file:
+    with open(filename) as file:
         config = yaml.load(file, loader)
     return config
 
 
 def _validate_choices(cls):
     for key in cls.__dataclass_fields__.keys():
         atr = cls.__dataclass_fields__[key]
-        if atr.init:
-            if "choices" in atr.metadata.keys():
-                if getattr(cls, key) not in atr.metadata.get("choices"):
-                    raise ValueError(
-                        f"{getattr(cls, key)} is not a valid choice for {key}. Please choose from on of the following: {atr.metadata['choices']}"
-                    )
+        if atr.init and "choices" in atr.metadata.keys():
+            if getattr(cls, key) not in atr.metadata.get("choices"):
+                raise ValueError(
+                    f"{getattr(cls, key)} is not a valid choice for {key}."
+                    f" Please choose from on of the following: {atr.metadata['choices']}"
+                )
 
 
 @dataclass
 class DataConfig:
     """Data configuration.
 
     Args:
@@ -95,40 +95,43 @@
         handle_missing_values (bool): Whether or not to handle missing values in categorical columns as
                 unknown
     """
 
     target: Optional[List[str]] = field(
         default=None,
         metadata={
-            "help": "A list of strings with the names of the target column(s). It is mandatory for all except SSL tasks."
+            "help": "A list of strings with the names of the target column(s)."
+            " It is mandatory for all except SSL tasks."
         },
     )
     continuous_cols: List = field(
         default_factory=list,
         metadata={"help": "Column names of the numeric fields. Defaults to []"},
     )
     categorical_cols: List = field(
         default_factory=list,
         metadata={"help": "Column names of the categorical fields to treat differently. Defaults to []"},
     )
     date_columns: List = field(
         default_factory=list,
         metadata={
-            "help": "(Column names, Freq) tuples of the date fields. For eg. a field named introduction_date and with a monthly frequency should have an entry ('intro_date','M'}"
+            "help": "(Column names, Freq) tuples of the date fields. For eg. a field named"
+            " `introduction_date` and with a monthly frequency should have an entry ('intro_date','M'}"
         },
     )
 
     encode_date_columns: bool = field(
         default=True,
         metadata={"help": "Whether or not to encode the derived variables from date"},
     )
     validation_split: Optional[float] = field(
         default=0.2,
         metadata={
-            "help": "Percentage of Training rows to keep aside as validation. Used only if Validation Data is not given separately"
+            "help": "Percentage of Training rows to keep aside as validation."
+            " Used only if Validation Data is not given separately"
         },
     )
     continuous_feature_transform: Optional[str] = field(
         default=None,
         metadata={
             "help": "Whether or not to transform the features before modelling. By default it is turned off.",
             "choices": [
@@ -143,15 +146,18 @@
     normalize_continuous_features: bool = field(
         default=True,
         metadata={"help": "Flag to normalize the input features(continuous)"},
     )
     quantile_noise: int = field(
         default=0,
         metadata={
-            "help": "NOT IMPLEMENTED. If specified fits QuantileTransformer on data with added gaussian noise with std = :quantile_noise: * data.std ; this will cause discrete values to be more separable. Please not that this transformation does NOT apply gaussian noise to the resulting data, the noise is only applied for QuantileTransformer"
+            "help": "NOT IMPLEMENTED. If specified fits QuantileTransformer on data with added gaussian noise"
+            " with std = :quantile_noise: * data.std ; this will cause discrete values to be more separable."
+            " Please not that this transformation does NOT apply gaussian noise to the resulting data,"
+            " the noise is only applied for QuantileTransformer"
         },
     )
     num_workers: Optional[int] = field(
         default=0,
         metadata={"help": "The number of workers used for data loading. For windows always set to 0"},
     )
     pin_memory: bool = field(
@@ -175,31 +181,29 @@
         if os.name == "nt" and self.num_workers != 0:
             print("Windows does not support num_workers > 0. Setting num_workers to 0")
             self.num_workers = 0
 
 
 @dataclass
 class InferredConfig:
-    """
-    Configuration inferred from the data during `fit` of the TabularDatamodule
+    """Configuration inferred from the data during `fit` of the TabularDatamodule.
 
     Args:
         categorical_dim (int): The number of categorical features
 
         continuous_dim (int): The number of continuous features
 
         output_dim (Optional[int]): The number of output targets
 
         categorical_cardinality (Optional[List[int]]): The number of unique values in categorical features
 
         embedding_dims (Optional[List]): The dimensions of the embedding for each categorical column as a
                 list of tuples (cardinality, embedding_dim).
 
         embedded_cat_dim (int): The number of features or dimensions of the embedded categorical features
-
     """
 
     categorical_dim: int = field(
         metadata={"help": "The number of categorical features"},
     )
     continuous_dim: int = field(
         metadata={"help": "The number of continuous features"},
@@ -223,28 +227,29 @@
         init=False,
         metadata={"help": "The number of features or dimensions of the embedded categorical features"},
     )
 
     def __post_init__(self):
         if self.embedding_dims is not None:
             assert all(
-                [(isinstance(t, Iterable) and len(t) == 2) for t in self.embedding_dims]
+                (isinstance(t, Iterable) and len(t) == 2) for t in self.embedding_dims
             ), "embedding_dims must be a list of tuples (cardinality, embedding_dim)"
             self.embedded_cat_dim = sum([t[1] for t in self.embedding_dims])
         else:
             self.embedded_cat_dim = 0
 
 
 @dataclass
 class TrainerConfig:
     """Trainer configuration
     Args:
         batch_size (int): Number of samples in each batch of training
 
-        data_aware_init_batch_size (int): Number of samples in each batch of training for the data-aware initialization, when applicable. Defaults to 2000
+        data_aware_init_batch_size (int): Number of samples in each batch of training for the data-aware initialization,
+            when applicable. Defaults to 2000
 
         fast_dev_run (bool): runs n if set to ``n`` (int) else 1 if set to ``True`` batch(es) of train, val
                 and test to find any bugs (ie: a sort of unit test).
 
         max_epochs (int): Maximum number of epochs to be run
 
         min_epochs (Optional[int]): Force training for at least these many epochs. 1 by default
@@ -252,15 +257,16 @@
         max_time (Optional[int]): Stop training after this amount of time has passed. Disabled by default
                 (None)
 
         gpus (Optional[int]): DEPRECATED: Number of gpus to train on (int). -1 uses all available GPUs. By
                 default uses CPU (None)
 
         accelerator (Optional[str]): The accelerator to use for training. Can be one of
-                'cpu','gpu','tpu','ipu','auto'. Defaults to 'auto'. Choices are: [`cpu`,`gpu`,`tpu`,`ipu`,`auto`].
+                'cpu','gpu','tpu','ipu', 'mps', 'auto'. Defaults to 'auto'.
+                Choices are: [`cpu`,`gpu`,`tpu`,`ipu`,'mps',`auto`].
 
         devices (Optional[int]): Number of devices to train on (int). -1 uses all available devices. By
                 default uses all available devices (-1)
 
         devices_list (Optional[List[int]]): List of devices to train on (list). If specified, takes
                 precedence over `devices` argument. Defaults to None
 
@@ -338,101 +344,116 @@
                 https://pytorch-lightning.readthedocs.io/en/latest/api/pytorch_lightning.trainer.html#pytorch_lightning.trainer.Trainer
     """
 
     batch_size: int = field(default=64, metadata={"help": "Number of samples in each batch of training"})
     data_aware_init_batch_size: int = field(
         default=2000,
         metadata={
-            "help": "Number of samples in each batch of training for the data-aware initialization, when applicable. Defaults to 2000"
+            "help": "Number of samples in each batch of training for the data-aware initialization,"
+            " when applicable. Defaults to 2000"
         },
     )
     fast_dev_run: bool = field(
         default=False,
         metadata={
-            "help": "runs n if set to ``n`` (int) else 1 if set to ``True`` batch(es) of train, val and test to find any bugs (ie: a sort of unit test)."
+            "help": "runs n if set to ``n`` (int) else 1 if set to ``True`` batch(es) of train,"
+            " val and test to find any bugs (ie: a sort of unit test)."
         },
     )
     max_epochs: int = field(default=10, metadata={"help": "Maximum number of epochs to be run"})
     min_epochs: Optional[int] = field(
         default=1,
         metadata={"help": "Force training for at least these many epochs. 1 by default"},
     )
     max_time: Optional[int] = field(
         default=None,
         metadata={"help": "Stop training after this amount of time has passed. Disabled by default (None)"},
     )
     gpus: Optional[int] = field(
         default=None,
         metadata={
-            "help": "DEPRECATED: Number of gpus to train on (int). -1 uses all available GPUs. By default uses CPU (None)"
+            "help": "DEPRECATED: Number of gpus to train on (int). -1 uses all available GPUs."
+            " By default uses CPU (None)"
         },
     )
     accelerator: Optional[str] = field(
         default="auto",
         metadata={
-            "help": "The accelerator to use for training. Can be one of 'cpu','gpu','tpu','ipu','auto'. Defaults to 'auto'",
-            "choices": ["cpu", "gpu", "tpu", "ipu", "auto"],
+            "help": "The accelerator to use for training. Can be one of 'cpu','gpu','tpu','ipu','auto'."
+            " Defaults to 'auto'",
+            "choices": ["cpu", "gpu", "tpu", "ipu", "mps", "auto"],
         },
     )
     devices: Optional[int] = field(
         default=None,
         metadata={
-            "help": "Number of devices to train on (int). -1 uses all available devices. By default uses all available devices (-1)",
+            "help": "Number of devices to train on (int). -1 uses all available devices."
+            " By default uses all available devices (-1)",
         },
     )
     devices_list: Optional[List[int]] = field(
         default=None,
         metadata={
-            "help": "List of devices to train on (list). If specified, takes precedence over `devices` argument. Defaults to None",
+            "help": "List of devices to train on (list). If specified, takes precedence over `devices` argument."
+            " Defaults to None",
         },
     )
 
     accumulate_grad_batches: int = field(
         default=1,
         metadata={
-            "help": "Accumulates grads every k batches or as set up in the dict. Trainer also calls optimizer.step() for the last indivisible step number."
+            "help": "Accumulates grads every k batches or as set up in the dict."
+            " Trainer also calls optimizer.step() for the last indivisible step number."
         },
     )
     auto_lr_find: bool = field(
         default=False,
         metadata={
-            "help": "Runs a learning rate finder algorithm (see this paper) when calling trainer.tune(), to find optimal initial learning rate."
+            "help": "Runs a learning rate finder algorithm (see this paper) when calling trainer.tune(),"
+            " to find optimal initial learning rate."
         },
     )
     auto_select_gpus: bool = field(
         default=True,
         metadata={
-            "help": "If enabled and `devices` is an integer, pick available gpus automatically. This is especially useful when GPUs are configured to be in 'exclusive mode', such that only one process at a time can access them."
+            "help": "If enabled and `devices` is an integer, pick available gpus automatically."
+            " This is especially useful when GPUs are configured to be in 'exclusive mode',"
+            " such that only one process at a time can access them."
         },
     )
     check_val_every_n_epoch: int = field(default=1, metadata={"help": "Check val every n train epochs."})
     gradient_clip_val: float = field(default=0.0, metadata={"help": "Gradient clipping value"})
     overfit_batches: float = field(
         default=0.0,
         metadata={
-            "help": "Uses this much data of the training set. If nonzero, will use the same training set for validation and testing. If the training dataloaders have shuffle=True, Lightning will automatically disable it. Useful for quickly debugging or trying to overfit on purpose."
+            "help": "Uses this much data of the training set. If nonzero, will use the same training set"
+            " for validation and testing. If the training dataloaders have shuffle=True,"
+            " Lightning will automatically disable it."
+            " Useful for quickly debugging or trying to overfit on purpose."
         },
     )
     deterministic: bool = field(
         default=False,
         metadata={
             "help": "If true enables cudnn.deterministic. Might make your system slower, but ensures reproducibility."
         },
     )
     profiler: Optional[str] = field(
         default=None,
         metadata={
-            "help": "To profile individual steps during training and assist in identifying bottlenecks. None, simple or advanced, pytorch",
+            "help": "To profile individual steps during training and assist in identifying bottlenecks."
+            " None, simple or advanced, pytorch",
             "choices": [None, "simple", "advanced", "pytorch"],
         },
     )
     early_stopping: Optional[str] = field(
         default="valid_loss",
         metadata={
-            "help": "The loss/metric that needed to be monitored for early stopping. If None, there will be no early stopping"
+            "help": "The loss/metric that needed to be monitored for early stopping."
+            " If None, there will be no early stopping"
         },
     )
     early_stopping_min_delta: float = field(
         default=0.001,
         metadata={"help": "The minimum delta in the loss/metric which qualifies as an improvement in early stopping"},
     )
     early_stopping_mode: str = field(
@@ -443,17 +464,18 @@
         },
     )
     early_stopping_patience: int = field(
         default=3,
         metadata={"help": "The number of epochs to wait until there is no further improvements in loss/metric"},
     )
     early_stopping_kwargs: Optional[Dict[str, Any]] = field(
-        default_factory=lambda: dict(),
+        default_factory=lambda: {},
         metadata={
-            "help": "Additional keyword arguments for the early stopping callback. See the documentation for the PyTorch Lightning EarlyStopping callback for more details."
+            "help": "Additional keyword arguments for the early stopping callback."
+            " See the documentation for the PyTorch Lightning EarlyStopping callback for more details."
         },
     )
     checkpoints: Optional[str] = field(
         default="valid_loss",
         metadata={
             "help": "The loss/metric that needed to be monitored for checkpoints. If None, there will be no checkpoints"
         },
@@ -465,39 +487,43 @@
     checkpoints_every_n_epochs: int = field(
         default=1,
         metadata={"help": "Number of training steps between checkpoints"},
     )
     checkpoints_name: Optional[str] = field(
         default=None,
         metadata={
-            "help": "The name under which the models will be saved. If left blank, first it will look for `run_name` in experiment_config and if that is also None then it will use a generic name like task_version."
+            "help": "The name under which the models will be saved. If left blank,"
+            " first it will look for `run_name` in experiment_config and if that is also None"
+            " then it will use a generic name like task_version."
         },
     )
     checkpoints_mode: str = field(
         default="min",
         metadata={"help": "The direction in which the loss/metric should be optimized"},
     )
     checkpoints_save_top_k: int = field(
         default=1,
         metadata={"help": "The number of best models to save"},
     )
     checkpoints_kwargs: Optional[Dict[str, Any]] = field(
-        default_factory=lambda: dict(),
+        default_factory=lambda: {},
         metadata={
-            "help": "Additional keyword arguments for the checkpoints callback. See the documentation for the PyTorch Lightning ModelCheckpoint callback for more details."
+            "help": "Additional keyword arguments for the checkpoints callback. See the documentation"
+            " for the PyTorch Lightning ModelCheckpoint callback for more details."
         },
     )
     load_best: bool = field(
         default=True,
         metadata={"help": "Flag to load the best model saved during training"},
     )
     track_grad_norm: int = field(
         default=-1,
         metadata={
-            "help": "Track and Log Gradient Norms in the logger. -1 by default means no tracking. 1 for the L1 norm, 2 for L2 norm, etc."
+            "help": "Track and Log Gradient Norms in the logger. -1 by default means no tracking. "
+            "1 for the L1 norm, 2 for L2 norm, etc."
         },
     )
     progress_bar: str = field(
         default="rich",
         metadata={"help": "Progress bar type. Can be one of: `none`, `simple`, `rich`. Defaults to `rich`."},
     )
     precision: int = field(
@@ -509,24 +535,23 @@
     )
     seed: int = field(
         default=42,
         metadata={"help": "Seed for random number generators. Defaults to 42"},
     )
     trainer_kwargs: Dict[str, Any] = field(
         default_factory=dict,
-        metadata={
-            "help": "Additional kwargs to be passed to PyTorch Lightning Trainer. See https://pytorch-lightning.readthedocs.io/en/latest/api/pytorch_lightning.trainer.html#pytorch_lightning.trainer.Trainer"
-        },
+        metadata={"help": "Additional kwargs to be passed to PyTorch Lightning Trainer."},
     )
 
     def __post_init__(self):
         _validate_choices(self)
         if self.gpus is not None:
             warnings.warn(
-                "The `gpus` argument is deprecated in favor of `accelerator` and will be removed in a future version of PyTorch Tabular. Please use `accelerator='gpu'` instead.",
+                "The `gpus` argument is deprecated in favor of `accelerator` and will be removed in a future version"
+                " of PyTorch Tabular. Please use `accelerator='gpu'` instead.",
                 DeprecationWarning,
             )
             if self.devices is None:
                 self.devices = self.gpus
             if self.accelerator is None:
                 self.accelerator = "gpu"
         else:
@@ -536,20 +561,22 @@
         if self.devices_list is not None:
             warnings.warn("Ignoring devices in favor of devices_list")
             self.devices = self.devices_list
         delattr(self, "devices_list")
         for key in self.early_stopping_kwargs.keys():
             if key in ["min_delta", "mode", "patience"]:
                 raise ValueError(
-                    f"Cannot override {key} in early_stopping_kwargs. Please use the appropriate argument in `TrainerConfig`"
+                    f"Cannot override {key} in early_stopping_kwargs."
+                    f" Please use the appropriate argument in `TrainerConfig`"
                 )
         for key in self.checkpoints_kwargs.keys():
             if key in ["dirpath", "filename", "monitor", "save_top_k", "mode", "every_n_epochs"]:
                 raise ValueError(
-                    f"Cannot override {key} in checkpoints_kwargs. Please use the appropriate argument in `TrainerConfig`"
+                    f"Cannot override {key} in checkpoints_kwargs."
+                    f" Please use the appropriate argument in `TrainerConfig`"
                 )
 
 
 @dataclass
 class ExperimentConfig:
     """Experiment configuration. Experiment Tracking with WandB and Tensorboard
     Args:
@@ -569,28 +596,32 @@
 
         exp_log_freq (int): step count between logging of gradients and parameters.
     """
 
     project_name: str = field(
         default=MISSING,
         metadata={
-            "help": "The name of the project under which all runs will be logged. For Tensorboard this defines the folder under which the logs will be saved and for W&B it defines the project name"
+            "help": "The name of the project under which all runs will be logged."
+            " For Tensorboard this defines the folder under which the logs will be saved"
+            " and for W&B it defines the project name"
         },
     )
 
     run_name: Optional[str] = field(
         default=None,
         metadata={
-            "help": "The name of the run; a specific identifier to recognize the run. If left blank, will be assigned a auto-generated name"
+            "help": "The name of the run; a specific identifier to recognize the run."
+            " If left blank, will be assigned a auto-generated name"
         },
     )
     exp_watch: Optional[str] = field(
         default=None,
         metadata={
-            "help": "The level of logging required.  Can be `gradients`, `parameters`, `all` or `None`. Defaults to None",
+            "help": "The level of logging required.  Can be `gradients`, `parameters`, `all` or `None`."
+            " Defaults to None",
             "choices": ["gradients", "parameters", "all", None],
         },
     )
 
     log_target: str = field(
         default="tensorboard",
         metadata={
@@ -639,25 +670,28 @@
         lr_scheduler_monitor_metric (Optional[str]): Used with ReduceLROnPlateau, where the plateau is
                 decided based on this metric
     """
 
     optimizer: str = field(
         default="Adam",
         metadata={
-            "help": "Any of the standard optimizers from [torch.optim](https://pytorch.org/docs/stable/optim.html#algorithms)."
+            "help": "Any of the standard optimizers from"
+            " [torch.optim](https://pytorch.org/docs/stable/optim.html#algorithms)."
         },
     )
     optimizer_params: Dict = field(
         default_factory=lambda: {},
         metadata={"help": "The parameters for the optimizer. If left blank, will use default parameters."},
     )
     lr_scheduler: Optional[str] = field(
         default=None,
         metadata={
-            "help": "The name of the LearningRateScheduler to use, if any, from [torch.optim.lr_scheduler](https://pytorch.org/docs/stable/optim.html#how-to-adjust-learning-rate). If None, will not use any scheduler. Defaults to `None`",
+            "help": "The name of the LearningRateScheduler to use, if any, from"
+            " https://pytorch.org/docs/stable/optim.html#how-to-adjust-learning-rate."
+            " If None, will not use any scheduler. Defaults to `None`",
         },
     )
     lr_scheduler_params: Optional[Dict] = field(
         default_factory=lambda: {},
         metadata={"help": "The parameters for the LearningRateScheduler. If left blank, will use default parameters."},
     )
 
@@ -676,15 +710,16 @@
 
 class ExperimentRunManager:
     def __init__(
         self,
         exp_version_manager: str = ".pt_tmp/exp_version_manager.yml",
     ) -> None:
         """The manages the versions of the experiments based on the name. It is a simple dictionary(yaml) based lookup.
-        Primary purpose is to avoid overwriting of saved models while runing the training without changing the experiment name.
+        Primary purpose is to avoid overwriting of saved models while runing the training without changing the
+        experiment name.
 
         Args:
             exp_version_manager (str, optional): The path of the yml file which acts as version control.
                 Defaults to ".pt_tmp/exp_version_manager.yml".
         """
         super().__init__()
         self._exp_version_manager = exp_version_manager
@@ -737,42 +772,52 @@
                 CrossEntropyLoss for classification. Unless you are sure what you are doing, leave it at MSELoss
                 or L1Loss for regression and CrossEntropyLoss for classification
 
         metrics (Optional[List[str]]): the list of metrics you need to track during training. The metrics
                 should be one of the functional metrics implemented in ``torchmetrics``. By default, it is
                 accuracy if classification and mean_squared_error for regression
 
-        metrics_params (Optional[List]): The parameters to be passed to the metrics function
+        metrics_prob_input (Optional[bool]): Is a mandatory parameter for classification metrics defined in
+                the config. This defines whether the input to the metric function is the probability or the class.
+                Length should be same as the number of metrics. Defaults to None.
+
+        metrics_params (Optional[List]): The parameters to be passed to the metrics function. `task` is forced to
+                be `multiclass` because the multiclass version can handle binary as well and for simplicity we are
+                only using `multiclass`.
 
         target_range (Optional[List]): The range in which we should limit the output variable. Currently
                 ignored for multi-target regression. Typically used for Regression problems. If left empty, will
                 not apply any restrictions
 
         seed (int): The seed for reproducibility. Defaults to 42
     """
 
     task: str = field(
         metadata={
-            "help": "Specify whether the problem is regression or classification. `backbone` is a task which considers the model as a backbone to generate features. Mostly used internally for SSL and related tasks.",
+            "help": "Specify whether the problem is regression or classification."
+            " `backbone` is a task which considers the model as a backbone to generate features."
+            " Mostly used internally for SSL and related tasks.",
             "choices": ["regression", "classification", "backbone"],
         }
     )
 
     head: Optional[str] = field(
         default="LinearHead",
         metadata={
-            "help": "The head to be used for the model. Should be one of the heads defined in `pytorch_tabular.models.common.heads`. Defaults to  LinearHead",
+            "help": "The head to be used for the model. Should be one of the heads defined"
+            " in `pytorch_tabular.models.common.heads`. Defaults to  LinearHead",
             "choices": [None, "LinearHead", "MixtureDensityHead"],
         },
     )
 
     head_config: Optional[Dict] = field(
         default_factory=lambda: {"layers": ""},
         metadata={
-            "help": "The config as a dict which defines the head. If left empty, will be initialized as default linear head."
+            "help": "The config as a dict which defines the head."
+            " If left empty, will be initialized as default linear head."
         },
     )
     embedding_dims: Optional[List] = field(
         default=None,
         metadata={
             "help": "The dimensions of the embedding for each categorical column as a list of tuples "
             "(cardinality, embedding_dim). If left empty, will infer using the cardinality of the "
@@ -800,21 +845,34 @@
             "leave it at MSELoss or L1Loss for regression and CrossEntropyLoss for classification"
         },
     )
     metrics: Optional[List[str]] = field(
         default=None,
         metadata={
             "help": "the list of metrics you need to track during training. The metrics should be one "
-            "of the functional metrics implemented in ``torchmetrics``. By default, "
-            "it is accuracy if classification and mean_squared_error for regression"
+            "of the functional metrics implemented in ``torchmetrics``. To use your own metric, please "
+            "use the `metric` param in the `fit` method By default, it is accuracy if classification "
+            "and mean_squared_error for regression"
+        },
+    )
+    metrics_prob_input: Optional[List[bool]] = field(
+        default=None,
+        metadata={
+            "help": "Is a mandatory parameter for classification metrics defined in the config. This defines "
+            "whether the input to the metric function is the probability or the class. Length should be same "
+            "as the number of metrics. Defaults to None."
         },
     )
     metrics_params: Optional[List] = field(
         default=None,
-        metadata={"help": "The parameters to be passed to the metrics function"},
+        metadata={
+            "help": "The parameters to be passed to the metrics function. `task` is forced to be `multiclass`` "
+            "because the multiclass version can handle binary as well and for simplicity we are only using "
+            "`multiclass`."
+        },
     )
     target_range: Optional[List] = field(
         default=None,
         metadata={
             "help": "The range in which we should limit the output variable. "
             "Currently ignored for multi-target regression. Typically used for Regression problems. "
             "If left empty, will not apply any restrictions"
@@ -828,21 +886,25 @@
     _module_src: str = field(default="models")
     _model_name: str = field(default="Model")
     _backbone_name: str = field(default="Backbone")
     _config_name: str = field(default="Config")
 
     def __post_init__(self):
         if self.task == "regression":
-            self.loss = "MSELoss" if self.loss is None else self.loss
-            self.metrics = ["mean_squared_error"] if self.metrics is None else self.metrics
+            self.loss = self.loss or "MSELoss"
+            self.metrics = self.metrics or ["mean_squared_error"]
             self.metrics_params = [{} for _ in self.metrics] if self.metrics_params is None else self.metrics_params
+            self.metrics_prob_input = [False for _ in self.metrics]  # not used in Regression. just for compatibility
         elif self.task == "classification":
-            self.loss = "CrossEntropyLoss" if self.loss is None else self.loss
-            self.metrics = ["accuracy"] if self.metrics is None else self.metrics
+            self.loss = self.loss or "CrossEntropyLoss"
+            self.metrics = self.metrics or ["accuracy"]
             self.metrics_params = [{} for _ in self.metrics] if self.metrics_params is None else self.metrics_params
+            self.metrics_prob_input = (
+                [False for _ in self.metrics] if self.metrics_prob_input is None else self.metrics_prob_input
+            )
         elif self.task == "backbone":
             self.loss = None
             self.metrics = None
             self.metrics_params = None
             if self.head is not None:
                 logger.warning("`head` is not a valid parameter for backbone task. Making `head=None`")
                 self.head = None
@@ -897,22 +959,24 @@
     """
 
     task: str = field(init=False, default="ssl")
 
     encoder_config: Optional[ModelConfig] = field(
         default=None,
         metadata={
-            "help": "The config of the encoder to be used for the model. Should be one of the model configs defined in PyTorch Tabular",
+            "help": "The config of the encoder to be used for the model."
+            " Should be one of the model configs defined in PyTorch Tabular",
         },
     )
 
     decoder_config: Optional[ModelConfig] = field(
         default=None,
         metadata={
-            "help": "The config of decoder to be used for the model. Should be one of the model configs defined in PyTorch Tabular. Defaults to nn.Identity",
+            "help": "The config of decoder to be used for the model."
+            " Should be one of the model configs defined in PyTorch Tabular. Defaults to nn.Identity",
         },
     )
 
     embedding_dims: Optional[List] = field(
         default=None,
         metadata={
             "help": "The dimensions of the embedding for each categorical column as a list of tuples "
@@ -923,15 +987,16 @@
     embedding_dropout: float = field(
         default=0.1,
         metadata={"help": "Dropout to be applied to the Categorical Embedding. Defaults to 0.1"},
     )
     batch_norm_continuous_input: bool = field(
         default=True,
         metadata={
-            "help": "If True, we will normalize the continuous layer by passing it through a BatchNorm layer. DEPRECATED - Use head and head_config instead"
+            "help": "If True, we will normalize the continuous layer by passing it through a BatchNorm layer."
+            " DEPRECATED - Use head and head_config instead"
         },
     )
     learning_rate: float = field(
         default=1e-3,
         metadata={"help": "The learning rate of the model. Defaults to 1e-3"},
     )
     seed: int = field(
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/feature_extractor.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/feature_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,34 +16,37 @@
     import pickle
 
 import torch
 
 
 class DeepFeatureExtractor(BaseEstimator, TransformerMixin):
     def __init__(self, tabular_model, extract_keys=["backbone_features"], drop_original=True):
-        """Initializes the Transformer and extracts the neural features
+        """Initializes the Transformer and extracts the neural features.
 
         Args:
             tabular_model (TabularModel): The trained TabularModel object
         """
         assert not (
             isinstance(tabular_model.model, NODEModel)
             or isinstance(tabular_model.model, TabNetModel)
             or isinstance(tabular_model.model, MDNModel)
         ), "FeatureExtractor doesn't work for Mixture Density Networks, NODE Model, & Tabnet Model"
         self.tabular_model = tabular_model
         self.extract_keys = extract_keys
         self.drop_original = drop_original
 
     def fit(self, X, y=None):
-        """Just for compatibility. Does not do anything"""
+        """Just for compatibility.
+
+        Does not do anything
+        """
         return self
 
     def transform(self, X: pd.DataFrame, y=None) -> pd.DataFrame:
-        """Transforms the categorical columns specified to the trained neural features from the model
+        """Transforms the categorical columns specified to the trained neural features from the model.
 
         Args:
             X (pd.DataFrame): DataFrame of features, shape (n_samples, n_features). Must contain columns to encode.
             y ([type], optional): Only for compatibility. Not used. Defaults to None.
 
         Raises:
             ValueError: [description]
@@ -60,15 +63,15 @@
         for batch in track(inference_dataloader, description="Generating Features..."):
             for k, v in batch.items():
                 if isinstance(v, list) and (len(v) == 0):
                     # Skipping empty list
                     continue
                 batch[k] = v.to(self.tabular_model.model.device)
             if self.tabular_model.config.task == "ssl":
-                ret_value = dict(backbone_features=self.tabular_model.model.predict(batch, ret_model_output=True))
+                ret_value = {"backbone_features": self.tabular_model.model.predict(batch, ret_model_output=True)}
             else:
                 _, ret_value = self.tabular_model.model.predict(batch, ret_model_output=True)
             for k in self.extract_keys:
                 if k in ret_value.keys():
                     logits_predictions[k].append(ret_value[k].detach().cpu())
 
         for k, v in logits_predictions.items():
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/__init__.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/autoint/autoint.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/autoint/autoint.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
 # Inspired by https://github.com/rixwew/pytorch-fm/blob/master/torchfm/model/afi.py
-"""AutomaticFeatureInteraction Model"""
+"""AutomaticFeatureInteraction Model."""
 import torch
 import torch.nn as nn
 from omegaconf import DictConfig
 
 from pytorch_tabular.models.common.layers import Embedding2dLayer
 from pytorch_tabular.utils import _initialize_layers, _linear_dropout_bn
 
@@ -119,15 +119,7 @@
     def _build_network(self):
         # Backbone
         self._backbone = AutoIntBackbone(self.hparams)
         # Embedding Layer
         self._embedding_layer = self._backbone._build_embedding_layer()
         # Head
         self._head = self._get_head_from_config()
-
-    # def extract_embedding(self):
-    #     if self.hparams.categorical_dim > 0:
-    #         return self.embedding_layer.cat_embedding_layers
-    #     else:
-    #         raise ValueError(
-    #             "Model has been trained with no categorical feature and therefore can't be used as a Categorical Encoder"
-    #         )
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/autoint/config.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/autoint/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""AutomaticFeatureInteraction Config"""
+"""AutomaticFeatureInteraction Config."""
 from dataclasses import dataclass, field
 from typing import Optional
 
 from pytorch_tabular.config import ModelConfig
 
 
 @dataclass
@@ -94,14 +94,18 @@
 
         metrics (Optional[List[str]]): the list of metrics you need to track during training. The metrics
                 should be one of the functional metrics implemented in ``torchmetrics``. By default, it is
                 accuracy if classification and mean_squared_error for regression
 
         metrics_params (Optional[List]): The parameters to be passed to the metrics function
 
+        metrics_prob_input (Optional[List]): Is a mandatory parameter for classification metrics defined in the config.
+            This defines whether the input to the metric function is the probability or the class. Length should be
+            same as the number of metrics. Defaults to None.
+
         target_range (Optional[List]): The range in which we should limit the output variable. Currently
                 ignored for multi-target regression. Typically used for Regression problems. If left empty, will
                 not apply any restrictions
 
         seed (int): The seed for reproducibility. Defaults to 42
     """
 
@@ -141,48 +145,60 @@
     embedding_bias: bool = field(
         default=True,
         metadata={"help": "Flag to turn on Embedding Bias. Defaults to True"},
     )
     share_embedding: bool = field(
         default=False,
         metadata={
-            "help": "The flag turns on shared embeddings in the input embedding process. The key idea here is to have an embedding for the feature as a whole along with embeddings of each unique values of that column. For more details refer to Appendix A of the TabTransformer paper. Defaults to False"
+            "help": "The flag turns on shared embeddings in the input embedding process."
+            " The key idea here is to have an embedding for the feature as a whole along with embeddings"
+            " of each unique values of that column."
+            " For more details refer to Appendix A of the TabTransformer paper. Defaults to False"
         },
     )
     share_embedding_strategy: Optional[str] = field(
         default="fraction",
         metadata={
-            "help": "There are two strategies in adding shared embeddings. 1. `add` - A separate embedding for the feature is added to the embedding of the unique values of the feature. 2. `fraction` - A fraction of the input embedding is reserved for the shared embedding of the feature. Defaults to fraction.",
+            "help": "There are two strategies in adding shared embeddings."
+            " 1. `add` - A separate embedding for the feature is added to the embedding"
+            " of the unique values of the feature."
+            " 2. `fraction` - A fraction of the input embedding is reserved"
+            " for the shared embedding of the feature. Defaults to fraction.",
             "choices": ["add", "fraction"],
         },
     )
     shared_embedding_fraction: float = field(
         default=0.25,
         metadata={
-            "help": "Fraction of the input_embed_dim to be reserved by the shared embedding. Should be less than one. Defaults to 0.25"
+            "help": "Fraction of the input_embed_dim to be reserved by the shared embedding."
+            " Should be less than one. Defaults to 0.25"
         },
     )
     deep_layers: bool = field(
         default=False,
         metadata={"help": "Flag to enable a deep MLP layer before the Multi-Headed Attention layer. Defaults to False"},
     )
     layers: str = field(
         default="128-64-32",
         metadata={"help": "Hyphen-separated number of layers and units in the deep MLP. Defaults to 128-64-32"},
     )
     activation: str = field(
         default="ReLU",
         metadata={
-            "help": "The activation type in the deep MLP. The default activaion in PyTorch like ReLU, TanH, LeakyReLU, etc. https://pytorch.org/docs/stable/nn.html#non-linear-activations-weighted-sum-nonlinearity. Defaults to ReLU"
+            "help": "The activation type in the deep MLP. The default activaion in PyTorch"
+            " like ReLU, TanH, LeakyReLU, etc."
+            " https://pytorch.org/docs/stable/nn.html#non-linear-activations-weighted-sum-nonlinearity."
+            " Defaults to ReLU"
         },
     )
     use_batch_norm: bool = field(
         default=False,
         metadata={
-            "help": "Flag to include a BatchNorm layer after each Linear Layer+DropOut in the deep MLP. Defaults to False"
+            "help": "Flag to include a BatchNorm layer after each Linear Layer+DropOut in the deep MLP."
+            " Defaults to False"
         },
     )
     initialization: str = field(
         default="kaiming",
         metadata={
             "help": "Initialization scheme for the linear layers in the deep MLP. Defaults to `kaiming`",
             "choices": ["kaiming", "xavier", "random"],
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/base_model.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/base_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""Base Model"""
+"""Base Model."""
 import warnings
 from abc import ABCMeta, abstractmethod
 from functools import partial
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
+import pandas as pd
 import pytorch_lightning as pl
 import torch
 import torch.nn as nn
 import torchmetrics
 from omegaconf import DictConfig, OmegaConf
 from torch import Tensor
 
@@ -43,47 +44,50 @@
         base_config: The base configuration.
         custom_config: The custom configuration.
 
     Returns:
         The merged configuration.
     """
     # using base config values if exist
-    if "embedding_dims" in config.keys() and config.embedding_dims is not None:
-        inferred_config.embedding_dims = config.embedding_dims
+    inferred_config.embedding_dims = config.get("embedding_dims") or inferred_config.embedding_dims
     merged_config = OmegaConf.merge(OmegaConf.to_container(config), OmegaConf.to_container(inferred_config))
     return merged_config
 
 
 class BaseModel(pl.LightningModule, metaclass=ABCMeta):
     def __init__(
         self,
         config: DictConfig,
         custom_loss: Optional[torch.nn.Module] = None,
         custom_metrics: Optional[List[Callable]] = None,
+        custom_metrics_prob_inputs: Optional[List[bool]] = None,
         custom_optimizer: Optional[torch.optim.Optimizer] = None,
         custom_optimizer_params: Dict = {},
         **kwargs,
     ):
-        """Base Model for PyTorch Tabular
+        """Base Model for PyTorch Tabular.
 
         Args:
             config (DictConfig): The configuration for the model.
             custom_loss (Optional[torch.nn.Module], optional): A custom loss function. Defaults to None.
             custom_metrics (Optional[List[Callable]], optional): A list of custom metrics. Defaults to None.
+            custom_metrics_prob_inputs (Optional[List[bool]], optional): A list of boolean values indicating whether the
+                metric requires probability inputs. Defaults to None.
             custom_optimizer (Optional[torch.optim.Optimizer], optional): A custom optimizer. Defaults to None.
             custom_optimizer_params (Dict, optional): A dictionary of custom optimizer parameters. Defaults to {}.
             kwargs (Dict, optional): Additional keyword arguments.
         """
         super().__init__()
         assert "inferred_config" in kwargs, "inferred_config not found in initialization arguments"
         inferred_config = kwargs["inferred_config"]
         # Merging the config and inferred config
         config = safe_merge_config(config, inferred_config)
         self.custom_loss = custom_loss
         self.custom_metrics = custom_metrics
+        self.custom_metrics_prob_inputs = custom_metrics_prob_inputs
         self.custom_optimizer = custom_optimizer
         self.custom_optimizer_params = custom_optimizer_params
         self.kwargs = kwargs
         # Updating config with custom parameters for experiment tracking
         if self.custom_loss is not None:
             config.loss = str(self.custom_loss)
         if self.custom_metrics is not None:
@@ -94,23 +98,33 @@
                 if isinstance(metric, partial):
                     # extracting func names from partial functions
                     config.metrics.append(metric.func.__name__)
                     config.metrics_params.append(metric.keywords)
                 else:
                     config.metrics.append(metric.__name__)
                     config.metrics_params.append(vars(metric))
-        else:  # Updating default metrics in config
             if config.task == "classification":
-                # Adding metric_params to config for classification task
-                for i, metric_params in enumerate(config.metrics_params):
-                    if "task" not in metric_params:
-                        # For classification task, output_dim == number of classses
-                        config.metrics_params[i]["task"] = "multiclass"
-                    if "num_classes" not in metric_params:
-                        config.metrics_params[i]["num_classes"] = inferred_config.output_dim
+                config.metrics_prob_inputs = self.custom_metrics_prob_inputs
+        # Updating default metrics in config
+        elif config.task == "classification":
+            # Adding metric_params to config for classification task
+            for i, mp in enumerate(config.metrics_params):
+                # For classification task, output_dim == number of classses
+                config.metrics_params[i]["task"] = mp.get("task", "multiclass")
+                config.metrics_params[i]["num_classes"] = mp.get("num_classes", inferred_config.output_dim)
+                if config.metrics[i] in (
+                    "accuracy",
+                    "precision",
+                    "recall",
+                    "precision_recall",
+                    "specificity",
+                    "f1_score",
+                    "fbeta_score",
+                ):
+                    config.metrics_params[i]["top_k"] = mp.get("top_k", 1)
 
         if self.custom_optimizer is not None:
             config.optimizer = str(self.custom_optimizer.__class__.__name__)
         if len(self.custom_optimizer_params) > 0:
             config.optimizer_params = self.custom_optimizer_params
         self.save_hyperparameters(config)
         # The concatenated output dim of the embedding layer
@@ -121,21 +135,23 @@
         self.do_log_logits = (
             hasattr(self.hparams, "log_logits") and self.hparams.log_logits and self.hparams.log_target == "wandb"
         )
         if not WANDB_INSTALLED:
             self.do_log_logits = False
             warnings.warn(
                 "Wandb is not installed. Please install wandb to log logits. "
-                "You can install wandb using pip install wandb or install PyTorch Tabular using pip install pytorch-tabular[all]"
+                "You can install wandb using pip install wandb or install PyTorch Tabular"
+                " using pip install pytorch-tabular[all]"
             )
         if not PLOTLY_INSTALLED:
             self.do_log_logits = False
             warnings.warn(
                 "Plotly is not installed. Please install plotly to log logits. "
-                "You can install plotly using pip install plotly or install PyTorch Tabular using pip install pytorch-tabular[all]"
+                "You can install plotly using pip install plotly or install PyTorch Tabular"
+                " using pip install pytorch-tabular[all]"
             )
 
     @abstractmethod
     def _build_network(self):
         pass
 
     @property
@@ -185,15 +201,15 @@
                         f"{metric} is not a valid functional metric defined in the torchmetrics.functional module"
                     )
                     raise e
         else:
             self.metrics = self.custom_metrics
 
     def calculate_loss(self, output: Dict, y: torch.Tensor, tag: str) -> torch.Tensor:
-        """Calculates the loss for the model
+        """Calculates the loss for the model.
 
         Args:
             output (Dict): The output dictionary from the model
             y (torch.Tensor): The target tensor
             tag (str): The tag to use for logging
 
         Returns:
@@ -202,36 +218,22 @@
         y_hat = output["logits"]
         reg_terms = [k for k, v in output.items() if "regularization" in k]
         reg_loss = 0
         for t in reg_terms:
             # Log only if non-zero
             if output[t] != 0:
                 reg_loss += output[t]
-                self.log(
-                    f"{tag}_{t}_loss",
-                    output[t],
-                    on_epoch=True,
-                    on_step=False,
-                    logger=True,
-                    prog_bar=False,
-                )
+                self.log(f"{tag}_{t}_loss", output[t], on_epoch=True, on_step=False, logger=True, prog_bar=False)
         if self.hparams.task == "regression":
             computed_loss = reg_loss
             for i in range(self.hparams.output_dim):
                 _loss = self.loss(y_hat[:, i], y[:, i])
                 computed_loss += _loss
                 if self.hparams.output_dim > 1:
-                    self.log(
-                        f"{tag}_loss_{i}",
-                        _loss,
-                        on_epoch=True,
-                        on_step=False,
-                        logger=True,
-                        prog_bar=False,
-                    )
+                    self.log(f"{tag}_loss_{i}", _loss, on_epoch=True, on_step=False, logger=True, prog_bar=False)
         else:
             # TODO loss fails with batch size of 1?
             computed_loss = self.loss(y_hat.squeeze(), y.squeeze()) + reg_loss
         self.log(
             f"{tag}_loss",
             computed_loss,
             on_epoch=(tag in ["valid", "test"]),
@@ -239,42 +241,37 @@
             # on_step=False,
             logger=True,
             prog_bar=True,
         )
         return computed_loss
 
     def calculate_metrics(self, y: torch.Tensor, y_hat: torch.Tensor, tag: str) -> List[torch.Tensor]:
-        """Calculates the metrics for the model
+        """Calculates the metrics for the model.
 
         Args:
             y (torch.Tensor): The target tensor
 
             y_hat (torch.Tensor): The predicted tensor
 
             tag (str): The tag to use for logging
 
         Returns:
             List[torch.Tensor]: The list of metric values
         """
         metrics = []
-        for metric, metric_str, metric_params in zip(self.metrics, self.hparams.metrics, self.hparams.metrics_params):
+        for metric, metric_str, prob_inp, metric_params in zip(
+            self.metrics, self.hparams.metrics, self.hparams.metrics_prob_input, self.hparams.metrics_params
+        ):
             if self.hparams.task == "regression":
                 _metrics = []
                 for i in range(self.hparams.output_dim):
-                    if isinstance(metric, partial):
-                        name = metric.func.__name__
-                    else:
-                        name = metric.__name__
+                    name = metric.func.__name__ if isinstance(metric, partial) else metric.__name__
                     if name == torchmetrics.functional.mean_squared_log_error.__name__:
                         # MSLE should only be used in strictly positive targets. It is undefined otherwise
-                        _metric = metric(
-                            torch.clamp(y_hat[:, i], min=0),
-                            torch.clamp(y[:, i], min=0),
-                            **metric_params,
-                        )
+                        _metric = metric(torch.clamp(y_hat[:, i], min=0), torch.clamp(y[:, i], min=0), **metric_params)
                     else:
                         _metric = metric(y_hat[:, i], y[:, i], **metric_params)
                     if self.hparams.output_dim > 1:
                         self.log(
                             f"{tag}_{metric_str}_{i}",
                             _metric,
                             on_epoch=True,
@@ -282,160 +279,157 @@
                             logger=True,
                             prog_bar=False,
                         )
                     _metrics.append(_metric)
                 avg_metric = torch.stack(_metrics, dim=0).sum()
             else:
                 y_hat = nn.Softmax(dim=-1)(y_hat.squeeze())
-                avg_metric = metric(y_hat, y.squeeze(), **metric_params)
+                if prob_inp:
+                    avg_metric = metric(y_hat, y.squeeze(), **metric_params)
+                else:
+                    avg_metric = metric(torch.argmax(y_hat, dim=-1), y.squeeze(), **metric_params)
             metrics.append(avg_metric)
-            self.log(
-                f"{tag}_{metric_str}",
-                avg_metric,
-                on_epoch=True,
-                on_step=False,
-                logger=True,
-                prog_bar=True,
-            )
+            self.log(f"{tag}_{metric_str}", avg_metric, on_epoch=True, on_step=False, logger=True, prog_bar=True)
         return metrics
 
     def data_aware_initialization(self, datamodule):
-        """Performs data-aware initialization of the model when defined"""
+        """Performs data-aware initialization of the model when defined."""
         pass
 
     def compute_backbone(self, x: Dict) -> torch.Tensor:
         # Returns output
         x = self.backbone(x)
         return x
 
     def embed_input(self, x: Dict) -> torch.Tensor:
         return self.embedding_layer(x)
 
     def apply_output_sigmoid_scaling(self, y_hat: torch.Tensor) -> torch.Tensor:
-        """Applies sigmoid scaling to the output of the model if the task is regression and the target range is defined
+        """Applies sigmoid scaling to the output of the model if the task is regression and the target range is defined.
 
         Args:
             y_hat (torch.Tensor): The output of the model
 
         Returns:
             torch.Tensor: The output of the model with sigmoid scaling applied
         """
         if (self.hparams.task == "regression") and (self.hparams.target_range is not None):
             for i in range(self.hparams.output_dim):
                 y_min, y_max = self.hparams.target_range[i]
                 y_hat[:, i] = y_min + nn.Sigmoid()(y_hat[:, i]) * (y_max - y_min)
         return y_hat
 
     def pack_output(self, y_hat: torch.Tensor, backbone_features: torch.tensor) -> Dict[str, Any]:
-        """Packs the output of the model
+        """Packs the output of the model.
 
         Args:
             y_hat (torch.Tensor): The output of the model
 
             backbone_features (torch.tensor): The backbone features
 
         Returns:
             The packed output of the model
         """
         # if self.head is the Identity function it means that we cannot extract backbone features,
         # because the model cannot be divide in backbone and head (i.e. TabNet)
         if type(self.head) == nn.Identity:
             return {"logits": y_hat}
-        else:
-            return {"logits": y_hat, "backbone_features": backbone_features}
+        return {"logits": y_hat, "backbone_features": backbone_features}
 
     def compute_head(self, backbone_features: Tensor) -> Dict[str, Any]:
-        """Computes the head of the model
+        """Computes the head of the model.
 
         Args:
             backbone_features (Tensor): The backbone features
 
         Returns:
             The output of the model
         """
         y_hat = self.head(backbone_features)
         y_hat = self.apply_output_sigmoid_scaling(y_hat)
         return self.pack_output(y_hat, backbone_features)
 
     def forward(self, x: Dict) -> Dict[str, Any]:
-        """The forward pass of the model
+        """The forward pass of the model.
 
         Args:
             x (Dict): The input of the model with 'continuous' and 'categorical' keys
         """
         x = self.embed_input(x)
         x = self.compute_backbone(x)
         return self.compute_head(x)
 
     def predict(self, x: Dict, ret_model_output: bool = False) -> Union[torch.Tensor, Tuple[torch.Tensor, Dict]]:
-        """
-        Predicts the output of the model
+        """Predicts the output of the model.
 
         Args:
             x (Dict): The input of the model with 'continuous' and 'categorical' keys
 
             ret_model_output (bool): If True, the method returns the output of the model
 
         Returns:
             The output of the model
         """
         assert self.hparams.task != "ssl", "It's not allowed to use the method predict in case of ssl task"
         ret_value = self.forward(x)
         if ret_model_output:
             return ret_value.get("logits"), ret_value
-        else:
-            return ret_value.get("logits")
+        return ret_value.get("logits")
 
     def forward_pass(self, batch):
         return self(batch), None
 
     def extract_embedding(self):
-        """Extracts the embedding of the model. This is used in `CategoricalEmbeddingTransformer`"""
+        """Extracts the embedding of the model.
+
+        This is used in `CategoricalEmbeddingTransformer`
+        """
         if self.hparams.categorical_dim > 0:
             if not isinstance(self.embedding_layer, PreEncoded1dLayer):
                 return self.embedding_layer.cat_embedding_layers
             else:
                 raise ValueError(
                     "Cannot extract embedding for PreEncoded1dLayer. Please use a different embedding layer."
                 )
         else:
             raise ValueError(
-                "Model has been trained with no categorical feature and therefore can't be used as a Categorical Encoder"
+                "Model has been trained with no categorical feature and therefore can't be used"
+                " as a Categorical Encoder"
             )
 
     def training_step(self, batch, batch_idx):
         output, y = self.forward_pass(batch)
         # y is not None for SSL task.Rest of the tasks target is
         # fetched from the batch
         y = batch["target"] if y is None else y
         y_hat = output["logits"]
         loss = self.calculate_loss(output, y, tag="train")
-        _ = self.calculate_metrics(y, y_hat, tag="train")
+        self.calculate_metrics(y, y_hat, tag="train")
         return loss
 
     def validation_step(self, batch, batch_idx):
         with torch.no_grad():
             output, y = self.forward_pass(batch)
             # y is not None for SSL task.Rest of the tasks target is
             # fetched from the batch
             y = batch["target"] if y is None else y
             y_hat = output["logits"]
-            _ = self.calculate_loss(output, y, tag="valid")
-            _ = self.calculate_metrics(y, y_hat, tag="valid")
+            self.calculate_loss(output, y, tag="valid")
+            self.calculate_metrics(y, y_hat, tag="valid")
         return y_hat, y
 
     def test_step(self, batch, batch_idx):
         with torch.no_grad():
             output, y = self.forward_pass(batch)
             # y is not None for SSL task.Rest of the tasks target is
             # fetched from the batch
             y = batch["target"] if y is None else y
             y_hat = output["logits"]
-            _ = self.calculate_loss(output, y, tag="test")
-            _ = self.calculate_metrics(y, y_hat, tag="test")
+            self.calculate_loss(output, y, tag="test")
+            self.calculate_metrics(y, y_hat, tag="test")
         return y_hat, y
 
     def configure_optimizers(self):
         if self.custom_optimizer is None:
             # Loading from the config
             try:
                 self._optimizer = getattr(torch.optim, self.hparams.optimizer)
@@ -457,28 +451,28 @@
                 **self.custom_optimizer_params,
             )
         if self.hparams.lr_scheduler is not None:
             try:
                 self._lr_scheduler = getattr(torch.optim.lr_scheduler, self.hparams.lr_scheduler)
             except AttributeError as e:
                 logger.error(
-                    f"{self.hparams.lr_scheduler} is not a valid learning rate sheduler defined in the torch.optim.lr_scheduler module"
+                    f"{self.hparams.lr_scheduler} is not a valid learning rate sheduler defined"
+                    f" in the torch.optim.lr_scheduler module"
                 )
                 raise e
             if isinstance(self._lr_scheduler, torch.optim.lr_scheduler._LRScheduler):
                 return {
                     "optimizer": opt,
                     "lr_scheduler": self._lr_scheduler(opt, **self.hparams.lr_scheduler_params),
                 }
-            else:
-                return {
-                    "optimizer": opt,
-                    "lr_scheduler": self._lr_scheduler(opt, **self.hparams.lr_scheduler_params),
-                    "monitor": self.hparams.lr_scheduler_monitor_metric,
-                }
+            return {
+                "optimizer": opt,
+                "lr_scheduler": self._lr_scheduler(opt, **self.hparams.lr_scheduler_params),
+                "monitor": self.hparams.lr_scheduler_monitor_metric,
+            }
         else:
             return opt
 
     def create_plotly_histogram(self, arr, name, bin_dict=None):
         fig = go.Figure()
         for i in range(arr.shape[-1]):
             fig.add_trace(
@@ -488,57 +482,68 @@
                     name=f"{name}_{i}",
                     xbins=bin_dict,  # dict(start=0.0, end=1.0, size=0.1),  # bins used for histogram
                 )
             )
         # Overlay both histograms
         fig.update_layout(
             barmode="overlay",
-            legend=dict(orientation="h", yanchor="bottom", y=1.02, xanchor="right", x=1),
+            legend={"orientation": "h", "yanchor": "bottom", "y": 1.02, "xanchor": "right", "x": 1},
         )
         # Reduce opacity to see both histograms
         fig.update_traces(opacity=0.5)
         return fig
 
     def validation_epoch_end(self, outputs) -> None:
         if self.do_log_logits:
             logits = [output[0] for output in outputs]
             logits = torch.cat(logits).detach().cpu()
             fig = self.create_plotly_histogram(logits, "logits")
             wandb.log(
-                {
-                    "valid_logits": wandb.Plotly(fig),
-                    "global_step": self.global_step,
-                },
+                {"valid_logits": wandb.Plotly(fig), "global_step": self.global_step},
                 commit=False,
             )
 
     def reset_weights(self):
         reset_all_weights(self.backbone)
         reset_all_weights(self.head)
         reset_all_weights(self.embedding_layer)
 
+    def feature_importance(self):
+        if hasattr(self.backbone, "feature_importance_"):
+            importance_df = pd.DataFrame(
+                {
+                    "Features": self.hparams.categorical_cols + self.hparams.continuous_cols,
+                    "importance": self.backbone.feature_importance_.detach().cpu().numpy(),
+                }
+            )
+            return importance_df
+        else:
+            raise ValueError("Feature Importance unavailable for this model.")
+
 
 class _GenericModel(BaseModel):
     def __init__(
         self,
         backbone: nn.Module,
         head: str,
         head_config: Dict,
         config: DictConfig,
         custom_loss: Optional[torch.nn.Module] = None,
         custom_metrics: Optional[List[Callable]] = None,
+        custom_metrics_prob_inputs: Optional[List[bool]] = None,
         custom_optimizer: Optional[torch.optim.Optimizer] = None,
         custom_optimizer_params: Dict = {},
         **kwargs,
     ):
         assert hasattr(config, "loss") or custom_loss is not None, "Loss function not defined in the config"
         super().__init__(
             config,
             custom_loss,
             custom_metrics,
+            custom_metrics_prob_inputs,
             custom_optimizer,
             custom_optimizer_params,
             head=head,
             head_config=head_config,
             backbone=backbone,
             **kwargs,
         )
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/category_embedding/category_embedding_model.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/category_embedding/category_embedding_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""Category Embedding Model"""
+"""Category Embedding Model."""
 import torch
 import torch.nn as nn
 from omegaconf import DictConfig
 
 from pytorch_tabular.models.common.layers import Embedding1dLayer
 from pytorch_tabular.utils import _initialize_layers, _linear_dropout_bn
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/category_embedding/config.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/category_embedding/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""Category Embedding Model Config"""
+"""Category Embedding Model Config."""
 from dataclasses import dataclass, field
 
 from pytorch_tabular.config import ModelConfig
 
 
 @dataclass
 class CategoryEmbeddingModelConfig(ModelConfig):
@@ -54,33 +54,43 @@
                 CrossEntropyLoss for classification. Unless you are sure what you are doing, leave it at MSELoss
                 or L1Loss for regression and CrossEntropyLoss for classification
 
         metrics (Optional[List[str]]): the list of metrics you need to track during training. The metrics
                 should be one of the functional metrics implemented in ``torchmetrics``. By default, it is
                 accuracy if classification and mean_squared_error for regression
 
-        metrics_params (Optional[List]): The parameters to be passed to the metrics function
+        metrics_params (Optional[List]): The parameters to be passed to the metrics function. `task` is forced to
+                be `multiclass` because the multiclass version can handle binary as well and for simplicity we are
+                only using `multiclass`.
+
+        metrics_prob_input (Optional[List]): Is a mandatory parameter for classification metrics defined in the config.
+            This defines whether the input to the metric function is the probability or the class. Length should be
+            same as the number of metrics. Defaults to None.
 
         target_range (Optional[List]): The range in which we should limit the output variable. Currently
                 ignored for multi-target regression. Typically used for Regression problems. If left empty, will
                 not apply any restrictions
 
         seed (int): The seed for reproducibility. Defaults to 42
     """
 
     layers: str = field(
         default="128-64-32",
         metadata={
-            "help": "Hyphen-separated number of layers and units in the classification head. eg. 32-64-32. Defaults to 128-64-32"
+            "help": "Hyphen-separated number of layers and units in the classification head. eg. 32-64-32."
+            " Defaults to 128-64-32"
         },
     )
     activation: str = field(
         default="ReLU",
         metadata={
-            "help": "The activation type in the classification head. The default activaion in PyTorch like ReLU, TanH, LeakyReLU, etc. https://pytorch.org/docs/stable/nn.html#non-linear-activations-weighted-sum-nonlinearity. Defaults to ReLU"
+            "help": "The activation type in the classification head. The default activaion in PyTorch"
+            " like ReLU, TanH, LeakyReLU, etc."
+            " https://pytorch.org/docs/stable/nn.html#non-linear-activations-weighted-sum-nonlinearity."
+            " Defaults to ReLU"
         },
     )
     use_batch_norm: bool = field(
         default=False,
         metadata={"help": "Flag to include a BatchNorm layer after each Linear Layer+DropOut. Defaults to False"},
     )
     initialization: str = field(
@@ -89,15 +99,16 @@
             "help": "Initialization scheme for the linear layers. Defaults to `kaiming`",
             "choices": ["kaiming", "xavier", "random"],
         },
     )
     dropout: float = field(
         default=0.0,
         metadata={
-            "help": "probability of an classification element to be zeroed. This is added to each linear layer. Defaults to 0.0"
+            "help": "probability of an classification element to be zeroed."
+            " This is added to each linear layer. Defaults to 0.0"
         },
     )
     _module_src: str = field(default="models.category_embedding")
     _model_name: str = field(default="CategoryEmbeddingModel")
     _backbone_name: str = field(default="CategoryEmbeddingBackbone")
     _config_name: str = field(default="CategoryEmbeddingModelConfig")
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/common/activations.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/common/activations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-# noqa W605
+# W605
 import torch
 import torch.nn.functional as F
 from torch import nn
 from torch.autograd import Function
 from torch.jit import script
 
 from pytorch_tabular.models.common.layers import PositionWiseFeedForward
 
 from .utils import _make_ix_like
 
 
 # GLU Variants Improve Transformer https://arxiv.org/pdf/2002.05202.pdf
 class GEGLU(nn.Module):
-    """
-    Gated Exponential Linear Unit (GEGLU)
-    """
+    """Gated Exponential Linear Unit (GEGLU)"""
 
     def __init__(self, d_model: int, d_ff: int, dropout: float = 0.1):
         """
         Args:
             d_model: dimension of the model
             d_ff: dimension of the feedforward layer
             dropout: dropout probability
@@ -27,17 +25,15 @@
         self.ffn = PositionWiseFeedForward(d_model, d_ff, dropout, nn.GELU(), True, False, False, False)
 
     def forward(self, x: torch.Tensor):
         return self.ffn(x)
 
 
 class ReGLU(nn.Module):
-    """
-    ReGLU
-    """
+    """ReGLU."""
 
     def __init__(self, d_model: int, d_ff: int, dropout: float = 0.1):
         """
         Args:
             d_model: dimension of the model
             d_ff: dimension of the feedforward layer
             dropout: dropout probability
@@ -61,24 +57,23 @@
         self.ffn = PositionWiseFeedForward(d_model, d_ff, dropout, nn.SiLU(), True, False, False, False)
 
     def forward(self, x: torch.Tensor):
         return self.ffn(x)
 
 
 class SparsemaxFunction(Function):
-    """
-    An implementation of sparsemax (Martins & Astudillo, 2016). See
-    :cite:`DBLP:journals/corr/MartinsA16` for detailed description.
+    """An implementation of sparsemax (Martins & Astudillo, 2016). See :cite:`DBLP:journals/corr/MartinsA16` for
+    detailed description.
 
     By Ben Peters and Vlad Niculae
     """
 
     @staticmethod
     def forward(ctx, input, dim: int = -1):
-        """sparsemax: normalizing sparse transform (a la softmax)
+        """Sparsemax: normalizing sparse transform (a la softmax)
 
         Parameters:
             input (Tensor): any shape
             dim (int): dimension along which to apply sparsemax
 
         Returns:
             output (Tensor): same shape as input
@@ -101,15 +96,15 @@
         v_hat = grad_input.sum(dim=dim) / supp_size.to(output.dtype).squeeze()
         v_hat = v_hat.unsqueeze(dim)
         grad_input = torch.where(output != 0, grad_input - v_hat, grad_input)
         return grad_input, None
 
     @staticmethod
     def _threshold_and_support(input, dim=-1):
-        """Sparsemax building block: compute the threshold
+        """Sparsemax building block: compute the threshold.
 
         Args:
             input: any dimension
             dim: dimension along which to apply the sparsemax
 
         Returns:
             the threshold value
@@ -135,16 +130,17 @@
 
 
 # sparsemax = lambda input, dim=-1: SparsemaxFunction.apply(input, dim)
 # sparsemoid = lambda input: (0.5 * input + 0.5).clamp_(0, 1)
 
 
 class Entmax15Function(Function):
-    """
-    An implementation of exact Entmax with alpha=1.5 (B. Peters, V. Niculae, A. Martins). See
+    """An implementation of exact Entmax with alpha=1.5 (B.
+
+    Peters, V. Niculae, A. Martins). See
     :cite:`https://arxiv.org/abs/1905.05702 for detailed description.
     Source: https://github.com/deep-spin/entmax
     """
 
     @staticmethod
     def forward(ctx, input, dim=-1):
         ctx.dim = dim
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/common/heads/blocks.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/common/heads/blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 from torch.distributions import Categorical
 
 from pytorch_tabular.models.common.heads import config as head_config
 from pytorch_tabular.utils import _initialize_layers, _linear_dropout_bn
 
 
 def config_link(r):
-    """
-    This is a helper function decorator to link the config to the head.
-    """
+    """This is a helper function decorator to link the config to the head."""
 
     def wrapper(f):
         f.config_template = r
         return f
 
     return wrapper
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/common/heads/config.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/common/heads/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from typing import List, Optional
 
 # from typing import Any, Dict, Iterable, List, Optional
 
 
 @dataclass
 class LinearHeadConfig:
-    """A model class for Linear Head configuration; serves as a template and documentation. The models take a dictionary as input, but if there are keys which are not present in this model class, it'll throw an exception.
+    """A model class for Linear Head configuration; serves as a template and documentation. The models take a dictionary
+    as input, but if there are keys which are not present in this model class, it'll throw an exception.
+
     Args:
         layers (str): Hyphen-separated number of layers and units in the classification/regression head.
                 eg. 32-64-32. Default is just a mapping from intput dimension to output dimension
 
         activation (str): The activation type in the classification head. The default activaion in PyTorch
                 like ReLU, TanH, LeakyReLU, etc. https://pytorch.org/docs/stable/nn.html#non-linear-activations-
                 weighted-sum-nonlinearity
@@ -22,21 +24,24 @@
         initialization (str): Initialization scheme for the linear layers. Defaults to `kaiming`. Choices
                 are: [`kaiming`,`xavier`,`random`].
     """
 
     layers: str = field(
         default="",
         metadata={
-            "help": "Hyphen-separated number of layers and units in the classification/regression head. eg. 32-64-32. Default is just a mapping from intput dimension to output dimension"
+            "help": "Hyphen-separated number of layers and units in the classification/regression head. eg. 32-64-32."
+            " Default is just a mapping from intput dimension to output dimension"
         },
     )
     activation: str = field(
         default="ReLU",
         metadata={
-            "help": "The activation type in the classification head. The default activaion in PyTorch like ReLU, TanH, LeakyReLU, etc. https://pytorch.org/docs/stable/nn.html#non-linear-activations-weighted-sum-nonlinearity"
+            "help": "The activation type in the classification head. The default activaion in PyTorch"
+            " like ReLU, TanH, LeakyReLU, etc."
+            " https://pytorch.org/docs/stable/nn.html#non-linear-activations-weighted-sum-nonlinearity"
         },
     )
     dropout: float = field(
         default=0.0,
         metadata={"help": "probability of an classification element to be zeroed."},
     )
     use_batch_norm: bool = field(
@@ -107,15 +112,17 @@
         metadata={
             "help": "Whether to have a bias term in the sigma layer. Defaults to False",
         },
     )
     mu_bias_init: Optional[List] = field(
         default=None,
         metadata={
-            "help": "To initialize the bias parameter of the mu layer to predefined cluster centers. Should be a list with the same length as number of gaussians in the mixture model. It is highly recommended to set the parameter to combat mode collapse. Defaults to None",
+            "help": "To initialize the bias parameter of the mu layer to predefined cluster centers."
+            " Should be a list with the same length as number of gaussians in the mixture model."
+            " It is highly recommended to set the parameter to combat mode collapse. Defaults to None",
         },
     )
 
     weight_regularization: Optional[int] = field(
         default=2,
         metadata={
             "help": "Whether to apply L1 or L2 Norm to the MDN layers. Defaults to L2",
@@ -140,15 +147,16 @@
         metadata={
             "help": "The regularization constant for weight regularization of mu layer. Defaults to 0",
         },
     )
     softmax_temperature: Optional[float] = field(
         default=1,
         metadata={
-            "help": "The temperature to be used in the gumbel softmax of the mixing coefficients. Values less than one leads to sharper transition between the multiple components. Defaults to 1",
+            "help": "The temperature to be used in the gumbel softmax of the mixing coefficients."
+            " Values less than one leads to sharper transition between the multiple components. Defaults to 1",
         },
     )
     n_samples: int = field(
         default=100,
         metadata={
             "help": "Number of samples to draw from the posterior to get prediction. Defaults to 100",
         },
@@ -159,27 +167,30 @@
             "help": "Which measure to use to get the point prediction. Defaults to mean",
             "choices": ["mean", "median"],
         },
     )
     speedup_training: bool = field(
         default=False,
         metadata={
-            "help": "Turning on this parameter does away with sampling during training which speeds up training, but also doesn't give you visibility on train metrics. Defaults to False",
+            "help": "Turning on this parameter does away with sampling during training which speeds up training,"
+            " but also doesn't give you visibility on train metrics. Defaults to False",
         },
     )
     log_debug_plot: bool = field(
         default=False,
         metadata={
-            "help": "Turning on this parameter plots histograms of the mu, sigma, and pi layers in addition to the logits(if log_logits is turned on in experment config). Defaults to False",
+            "help": "Turning on this parameter plots histograms of the mu, sigma, and pi layers in addition"
+            " to the logits(if log_logits is turned on in experment config). Defaults to False",
         },
     )
     input_dim: int = field(
         default=None,
         metadata={
-            "help": "The input dimensions to the head. This will be automatically filled in while initializing from the `backbone.output_dim`",
+            "help": "The input dimensions to the head. This will be automatically filled in while initializing"
+            " from the `backbone.output_dim`",
         },
     )
     _probabilistic: bool = field(default=True)
 
 
 # if __name__ == "__main__":
 #     from pytorch_tabular.utils import generate_doc_dataclass
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/common/layers.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/common/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# noqa W605
+# W605
 import math
 from functools import partial
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import torch
 from einops import rearrange
 from torch import einsum, nn
@@ -17,33 +17,33 @@
 
     def forward(self, x, **kwargs):
         return self.fn(x, **kwargs) + x
 
 
 # https://github.com/labmlai/annotated_deep_learning_paper_implementations/blob/master/labml_nn/transformers/feed_forward.py
 class PositionWiseFeedForward(nn.Module):
-    """
+    r"""
     title: Position-wise Feed-Forward Network (FFN)
     summary: Documented reusable implementation of the position wise feedforward network.
 
     # Position-wise Feed-Forward Network (FFN)
     This is a [PyTorch](https://pytorch.org)  implementation
     of position-wise feedforward network used in transformer.
     FFN consists of two fully connected layers.
     Number of dimensions in the hidden layer $d_{ff}$, is generally set to around
     four times that of the token embedding $d_{model}$.
     So it is sometime also called the expand-and-contract network.
     There is an activation at the hidden layer, which is
-    usually set to ReLU (Rectified Linear Unit) activation, $$\max(0, x)$$
+    usually set to ReLU (Rectified Linear Unit) activation, $$\\max(0, x)$$
     That is, the FFN function is,
-    $$FFN(x, W_1, W_2, b_1, b_2) = \max(0, x W_1 + b_1) W_2 + b_2$$
+    $$FFN(x, W_1, W_2, b_1, b_2) = \\max(0, x W_1 + b_1) W_2 + b_2$$
     where $W_1$, $W_2$, $b_1$ and $b_2$ are learnable parameters.
     Sometimes the
     GELU (Gaussian Error Linear Unit) activation is also used instead of ReLU.
-    $$x \Phi(x)$$ where $\Phi(x) = P(X \le x), X \sim \mathcal{N}(0,1)$
+    $$x \\Phi(x)$$ where $\\Phi(x) = P(X \\le x), X \\sim \\mathcal{N}(0,1)$
     ### Gated Linear Units
     This is a generic implementation that supports different variants including
     [Gated Linear Units](https://arxiv.org/abs/2002.05202) (GLU).
     """
 
     def __init__(
         self,
@@ -106,31 +106,30 @@
 # 3. AutoGluon - https://github.com/awslabs/autogluon
 # AutoGluon is an AuttoML library which supports Tabular data as well. it is from Amazon Research and is in MXNet
 # 4. LabML Annotated Deep Learning Papers - The position-wise FF was shamelessly copied from
 # https://github.com/labmlai/annotated_deep_learning_paper_implementations/tree/master/labml_nn/transformers
 
 
 class AddNorm(nn.Module):
-    """
-    Applies LayerNorm, Dropout and adds to input. Standard AddNorm operations in Transformers
+    """Applies LayerNorm, Dropout and adds to input.
+
+    Standard AddNorm operations in Transformers
     """
 
     def __init__(self, input_dim: int, dropout: float):
-        super(AddNorm, self).__init__()
+        super().__init__()
         self.dropout = nn.Dropout(dropout)
         self.ln = nn.LayerNorm(input_dim)
 
     def forward(self, X: torch.Tensor, Y: torch.Tensor) -> torch.Tensor:
         return self.ln(self.dropout(Y) + X)
 
 
 class MultiHeadedAttention(nn.Module):
-    """
-    Multi Headed Attention Block in Transformers
-    """
+    """Multi Headed Attention Block in Transformers."""
 
     def __init__(
         self,
         input_dim: int,
         num_heads: int = 8,
         head_dim: int = 16,
         dropout: int = 0.1,
@@ -147,40 +146,38 @@
         self.to_out = nn.Linear(inner_dim, input_dim)
 
         self.dropout = nn.Dropout(dropout)
 
     def forward(self, x):
         h = self.n_heads
         q, k, v = self.to_qkv(x).chunk(3, dim=-1)
-        q, k, v = map(lambda t: rearrange(t, "b n (h d) -> b h n d", h=h), (q, k, v))
+        q, k, v = (rearrange(t, "b n (h d) -> b h n d", h=h) for t in (q, k, v))
         sim = einsum("b h i d, b h j d -> b h i j", q, k) * self.scale
 
         attn = sim.softmax(dim=-1)
         attn = self.dropout(attn)
         if self.keep_attn:
             self.attn_weights = attn
         out = einsum("b h i j, b h j d -> b h i d", attn, v)
         out = rearrange(out, "b h n d -> b n (h d)", h=h)
         return self.to_out(out)
 
 
 # Slight adaptation from https://github.com/jrzaurin/pytorch-widedeep which in turn adapted from AutoGluon
 class SharedEmbeddings(nn.Module):
-    """
-    Enables different values in a categorical feature to share some embeddings across
-    """
+    """Enables different values in a categorical feature to share some embeddings across."""
 
     def __init__(
         self,
         num_embed: int,
         embed_dim: int,
         add_shared_embed: bool = False,
         frac_shared_embed: float = 0.25,
     ):
-        super(SharedEmbeddings, self).__init__()
+        super().__init__()
         assert frac_shared_embed < 1, "'frac_shared_embed' must be less than 1"
 
         self.add_shared_embed = add_shared_embed
         self.embed = nn.Embedding(num_embed, embed_dim, padding_idx=0)
         self.embed.weight.data.clamp_(-2, 2)
         if add_shared_embed:
             col_embed_dim = embed_dim
@@ -215,27 +212,25 @@
     elif initialization is None:
         pass
     else:
         raise NotImplementedError("initialization should be either of `kaiming_normal`, `kaiming_uniform`, `None`")
 
 
 class PreEncoded1dLayer(nn.Module):
-    """
-    Takes in pre-encoded categorical variables and just concatenates with continuous variables
-    No learnable component
-    """
+    """Takes in pre-encoded categorical variables and just concatenates with continuous variables No learnable
+    component."""
 
     def __init__(
         self,
         continuous_dim: int,
         categorical_dim: Tuple[int, int],
         embedding_dropout: float = 0.0,
         batch_norm_continuous_input: bool = False,
     ):
-        super(PreEncoded1dLayer, self).__init__()
+        super().__init__()
         self.continuous_dim = continuous_dim
         self.categorical_dim = categorical_dim
         self.batch_norm_continuous_input = batch_norm_continuous_input
 
         if embedding_dropout > 0:
             self.embd_dropout = nn.Dropout(embedding_dropout)
         else:
@@ -271,26 +266,24 @@
                 embed = torch.cat([embed, categorical_data], dim=1)
         if self.embd_dropout is not None:
             embed = self.embd_dropout(embed)
         return embed
 
 
 class Embedding1dLayer(nn.Module):
-    """
-    Enables different values in a categorical features to have different embeddings
-    """
+    """Enables different values in a categorical features to have different embeddings."""
 
     def __init__(
         self,
         continuous_dim: int,
         categorical_embedding_dims: Tuple[int, int],
         embedding_dropout: float = 0.0,
         batch_norm_continuous_input: bool = False,
     ):
-        super(Embedding1dLayer, self).__init__()
+        super().__init__()
         self.continuous_dim = continuous_dim
         self.categorical_embedding_dims = categorical_embedding_dims
         self.batch_norm_continuous_input = batch_norm_continuous_input
 
         # Embedding layers
         self.cat_embedding_layers = nn.ModuleList([nn.Embedding(x, y) for x, y in categorical_embedding_dims])
         if embedding_dropout > 0:
@@ -335,17 +328,15 @@
                 embed = torch.cat([embed, categorical_embed], dim=1)
         if self.embd_dropout is not None:
             embed = self.embd_dropout(embed)
         return embed
 
 
 class Embedding2dLayer(nn.Module):
-    """
-    Embeds categorical and continuous features into a 2D tensor
-    """
+    """Embeds categorical and continuous features into a 2D tensor."""
 
     def __init__(
         self,
         continuous_dim: int,
         categorical_cardinality: List[int],
         embedding_dim: int,
         shared_embedding_strategy: Optional[str] = None,
@@ -362,15 +353,15 @@
             embedding_dim: embedding dimension
             shared_embedding_strategy: strategy to use for shared embeddings
             frac_shared_embed: fraction of embeddings to share
             embedding_bias: whether to use bias in embedding layers
             batch_norm_continuous_input: whether to use batch norm on continuous features
             embedding_dropout: dropout to apply to embeddings
             initialization: initialization strategy to use for embedding layers"""
-        super(Embedding2dLayer, self).__init__()
+        super().__init__()
         self.continuous_dim = continuous_dim
         self.categorical_cardinality = categorical_cardinality
         self.embedding_dim = embedding_dim
         self.batch_norm_continuous_input = batch_norm_continuous_input
         self.shared_embedding_strategy = shared_embedding_strategy
         self.frac_shared_embed = frac_shared_embed
         self.embedding_bias = embedding_bias
@@ -476,15 +467,15 @@
                 embed = torch.cat([embed, categorical_embed], dim=1)
         if self.embd_dropout is not None:
             embed = self.embd_dropout(embed)
         return embed
 
 
 class TransformerEncoderBlock(nn.Module):
-    """A single Transformer Encoder Block"""
+    """A single Transformer Encoder Block."""
 
     def __init__(
         self,
         input_embed_dim: int,
         num_heads: int = 8,
         ff_hidden_multiplier: int = 4,
         ff_activation: str = "GEGLU",
@@ -535,42 +526,42 @@
         y = self.mha(x)
         x = self.attn_add_norm(x, y)
         y = self.pos_wise_ff(y)
         return self.ff_add_norm(x, y)
 
 
 class Lambda(nn.Module):
-    """A wrapper for a lambda function as a pytorch module"""
+    """A wrapper for a lambda function as a pytorch module."""
 
     def __init__(self, func: Callable):
         """Initialize lambda module
         Args:
             func: any function/callable
         """
         super().__init__()
         self.func = func
 
     def forward(self, *args, **kwargs):
         return self.func(*args, **kwargs)
 
 
 class ModuleWithInit(nn.Module):
-    """Base class for pytorch module with data-aware initializer on first batch"""
+    """Base class for pytorch module with data-aware initializer on first batch."""
 
     def __init__(self):
         super().__init__()
         self._is_initialized_tensor = nn.Parameter(torch.tensor(0, dtype=torch.uint8), requires_grad=False)
         self._is_initialized_bool = None
         # Note: this module uses a separate flag self._is_initialized so as to achieve both
         # * persistence: is_initialized is saved alongside model in state_dict
         # * speed: model doesn't need to cache
         # please DO NOT use these flags in child modules
 
     def initialize(self, *args, **kwargs):
-        """initialize module tensors using first batch of data"""
+        """Initialize module tensors using first batch of data."""
         raise NotImplementedError("Please implement ")
 
     def __call__(self, *args, **kwargs):
         if self._is_initialized_bool is None:
             self._is_initialized_bool = bool(self._is_initialized_tensor.item())
         if not self._is_initialized_bool:
             self.initialize(*args, **kwargs)
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/common/utils.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 
 
 def to_one_hot(y, depth=None):
-    r"""
-    Takes integer with n dims and converts it to 1-hot representation with n + 1 dims.
+    r"""Takes integer with n dims and converts it to 1-hot representation with n + 1 dims.
+
     The n+1'st dimension will have zeros everywhere but at y'th index, where it will be equal to 1.
     Args:
         y: input integer (IntTensor, LongTensor or Variable) of any shape
         depth (int):  the size of the one hot dimension
     """
     y_flat = y.to(torch.int64).view(-1, 1)
     depth = depth if depth is not None else int(torch.max(y_flat)) + 1
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/ft_transformer/config.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/ft_transformer/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""AutomaticFeatureInteraction Config"""
+"""AutomaticFeatureInteraction Config."""
 import warnings
 from dataclasses import dataclass, field
 from typing import Optional
 
 from pytorch_tabular.config import ModelConfig
 from pytorch_tabular.utils import ifnone
 
@@ -98,15 +98,21 @@
                 CrossEntropyLoss for classification. Unless you are sure what you are doing, leave it at MSELoss
                 or L1Loss for regression and CrossEntropyLoss for classification
 
         metrics (Optional[List[str]]): the list of metrics you need to track during training. The metrics
                 should be one of the functional metrics implemented in ``torchmetrics``. By default, it is
                 accuracy if classification and mean_squared_error for regression
 
-        metrics_params (Optional[List]): The parameters to be passed to the metrics function
+        metrics_params (Optional[List]): The parameters to be passed to the metrics function. `task` is forced to
+                be `multiclass` because the multiclass version can handle binary as well and for simplicity we are
+                only using `multiclass`.
+
+        metrics_prob_input (Optional[List]): Is a mandatory parameter for classification metrics defined in the config.
+            This defines whether the input to the metric function is the probability or the class. Length should be
+            same as the number of metrics. Defaults to None.
 
         target_range (Optional[List]): The range in which we should limit the output variable. Currently
                 ignored for multi-target regression. Typically used for Regression problems. If left empty, will
                 not apply any restrictions
 
         seed (int): The seed for reproducibility. Defaults to 42
     """
@@ -125,48 +131,58 @@
     embedding_bias: bool = field(
         default=True,
         metadata={"help": "Flag to turn on Embedding Bias. Defaults to True"},
     )
     share_embedding: bool = field(
         default=False,
         metadata={
-            "help": "The flag turns on shared embeddings in the input embedding process. The key idea here is to have an embedding for the feature as a whole along with embeddings of each unique values of that column. For more details refer to Appendix A of the TabTransformer paper. Defaults to False"
+            "help": "The flag turns on shared embeddings in the input embedding process."
+            " The key idea here is to have an embedding for the feature as a whole along with embeddings"
+            " of each unique values of that column. For more details refer"
+            " to Appendix A of the TabTransformer paper. Defaults to False"
         },
     )
     share_embedding_strategy: Optional[str] = field(
         default="fraction",
         metadata={
-            "help": "There are two strategies in adding shared embeddings. 1. `add` - A separate embedding for the feature is added to the embedding of the unique values of the feature. 2. `fraction` - A fraction of the input embedding is reserved for the shared embedding of the feature. Defaults to fraction.",
+            "help": "There are two strategies in adding shared embeddings."
+            " 1. `add` - A separate embedding for the feature is added to the embedding"
+            " of the unique values of the feature."
+            " 2. `fraction` - A fraction of the input embedding is reserved"
+            " for the shared embedding of the feature. Defaults to fraction.",
             "choices": ["add", "fraction"],
         },
     )
     shared_embedding_fraction: float = field(
         default=0.25,
         metadata={
-            "help": "Fraction of the input_embed_dim to be reserved by the shared embedding. Should be less than one. Defaults to 0.25"
+            "help": "Fraction of the input_embed_dim to be reserved by the shared embedding."
+            " Should be less than one. Defaults to 0.25"
         },
     )
     attn_feature_importance: bool = field(
         default=True,
         metadata={
-            "help": "If you are facing memory issues, you can turn off feature importance which will not save the attention weights. Defaults to True"
+            "help": "If you are facing memory issues, you can turn off feature importance"
+            " which will not save the attention weights. Defaults to True"
         },
     )
     num_heads: int = field(
         default=8,
         metadata={"help": "The number of heads in the Multi-Headed Attention layer. Defaults to 8"},
     )
     num_attn_blocks: int = field(
         default=6,
         metadata={"help": "The number of layers of stacked Multi-Headed Attention layers. Defaults to 6"},
     )
     transformer_head_dim: Optional[int] = field(
         default=None,
         metadata={
-            "help": "The number of hidden units in the Multi-Headed Attention layers. Defaults to None and will be same as input_dim."
+            "help": "The number of hidden units in the Multi-Headed Attention layers."
+            " Defaults to None and will be same as input_dim."
         },
     )
     attn_dropout: float = field(
         default=0.1,
         metadata={"help": "Dropout to be applied after Multi headed Attention. Defaults to 0.1"},
     )
     add_norm_dropout: float = field(
@@ -181,27 +197,34 @@
         default=4,
         metadata={"help": "Multiple by which the Positionwise FF layer scales the input. Defaults to 4"},
     )
 
     transformer_activation: str = field(
         default="GEGLU",
         metadata={
-            "help": "The activation type in the transformer feed forward layers. In addition to the default activation in PyTorch like ReLU, TanH, LeakyReLU, etc. https://pytorch.org/docs/stable/nn.html#non-linear-activations-weighted-sum-nonlinearity, GEGLU, ReGLU and SwiGLU are also implemented(https://arxiv.org/pdf/2002.05202.pdf). Defaults to GEGLU",
+            "help": "The activation type in the transformer feed forward layers."
+            " In addition to the default activation in PyTorch like ReLU, TanH, LeakyReLU, etc."
+            " https://pytorch.org/docs/stable/nn.html#non-linear-activations-weighted-sum-nonlinearity,"
+            " GEGLU, ReGLU and SwiGLU are also implemented (https://arxiv.org/pdf/2002.05202.pdf)."
+            " Defaults to GEGLU",
         },
     )
     out_ff_layers: Optional[str] = field(
         default=None,
         metadata={
             "help": "DEPRECATED: Hyphen-separated number of layers and units in the deep MLP. Defaults to 128-64-32"
         },
     )
     out_ff_activation: Optional[str] = field(
         default=None,
         metadata={
-            "help": "DEPRECATED: The activation type in the deep MLP. The default activaion in PyTorch like ReLU, TanH, LeakyReLU, etc. https://pytorch.org/docs/stable/nn.html#non-linear-activations-weighted-sum-nonlinearity. Defaults to ReLU"
+            "help": "DEPRECATED: The activation type in the deep MLP. The default activaion in PyTorch"
+            " like ReLU, TanH, LeakyReLU, etc."
+            " https://pytorch.org/docs/stable/nn.html#non-linear-activations-weighted-sum-nonlinearity."
+            " Defaults to ReLU"
         },
     )
     out_ff_dropout: Optional[float] = field(
         default=None,
         metadata={
             "help": "DEPRECATED: probability of an classification element to be zeroed in the deep MLP. Defaults to 0.0"
         },
@@ -223,31 +246,34 @@
             "out_ff_layers",
             "out_ff_activation",
             "out_ff_dropoout",
             "out_ff_initialization",
         ]
         if self.head_config != {"layers": ""}:  # If the user has passed a head_config
             warnings.warn(
-                "Ignoring the deprecated arguments, `out_ff_layers`, `out_ff_activation`, `out_ff_dropoout`, and `out_ff_initialization` as head_config is passed."
+                "Ignoring the deprecated arguments, `out_ff_layers`, `out_ff_activation`, `out_ff_dropoout`,"
+                " and `out_ff_initialization` as head_config is passed."
             )
         else:
-            if any([p is not None for p in deprecated_args]):
+            if any(p is not None for p in deprecated_args):
                 warnings.warn(
-                    "The `out_ff_layers`, `out_ff_activation`, `out_ff_dropoout`, and `out_ff_initialization` arguments are deprecated and will be removed next release. Please use head and head_config as an alternative.",
+                    "The `out_ff_layers`, `out_ff_activation`, `out_ff_dropoout`, and `out_ff_initialization`"
+                    " arguments are deprecated and will be removed next release."
+                    " Please use head and head_config as an alternative.",
                     DeprecationWarning,
                 )
                 # TODO: Remove this once we deprecate the old config
                 # Fill the head_config using deprecated parameters
-                self.head_config = dict(
-                    layers=ifnone(self.out_ff_layers, ""),
-                    activation=ifnone(self.out_ff_activation, "ReLU"),
-                    dropout=ifnone(self.out_ff_dropout, 0.0),
-                    use_batch_norm=False,
-                    initialization=ifnone(self.out_ff_initialization, "kaiming"),
-                )
+                self.head_config = {
+                    "layers": ifnone(self.out_ff_layers, ""),
+                    "activation": ifnone(self.out_ff_activation, "ReLU"),
+                    "dropout": ifnone(self.out_ff_dropout, 0.0),
+                    "use_batch_norm": False,
+                    "initialization": ifnone(self.out_ff_initialization, "kaiming"),
+                }
 
         return super().__post_init__()
 
 
 # if __name__ == "__main__":
 #     from pytorch_tabular.utils import generate_doc_dataclass
 #     print(generate_doc_dataclass(FTTransformerConfig))
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/ft_transformer/ft_transformer.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/ft_transformer/ft_transformer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""Feature Tokenizer Transformer Model"""
+"""Feature Tokenizer Transformer Model."""
 import math
 from collections import OrderedDict
 
-import pandas as pd
 import torch
 import torch.nn as nn
 from omegaconf import DictConfig
 
 from ..base_model import BaseModel
 from ..common.layers import Embedding2dLayer, TransformerEncoderBlock
 
@@ -43,15 +42,18 @@
 
 class FTTransformerBackbone(nn.Module):
     def __init__(self, config: DictConfig):
         super().__init__()
         assert config.share_embedding_strategy in [
             "add",
             "fraction",
-        ], f"`share_embedding_strategy` should be one of `add` or `fraction`, not {self.hparams.share_embedding_strategy}"
+        ], (
+            "`share_embedding_strategy` should be one of `add` or `fraction`,"
+            f" not {self.hparams.share_embedding_strategy}"
+        )
         self.hparams = config
         self._build_network()
 
     def _build_network(self):
         self.add_cls = AppendCLSToken(
             d_token=self.hparams.input_embed_dim,
             initialization=self.hparams.embedding_initialization,
@@ -109,15 +111,15 @@
         n, h, f, _ = self.attention_weights_[0].shape
         device = self.attention_weights_[0].device
         L = len(self.attention_weights_)
         self.local_feature_importance = torch.zeros((n, f), device=device)
         for attn_weights in self.attention_weights_:
             self.local_feature_importance += attn_weights[:, :, :, -1].sum(dim=1)
         self.local_feature_importance = (1 / (h * L)) * self.local_feature_importance[:, :-1]
-        self.feature_importance_ = self.local_feature_importance.mean(dim=0)
+        self.feature_importance_ = self.local_feature_importance.mean(dim=0).detach().cpu().numpy()
         # self.feature_importance_count_+=attn_weights.shape[0]
 
 
 class FTTransformerModel(BaseModel):
     def __init__(self, config: DictConfig, **kwargs):
         super().__init__(config, **kwargs)
 
@@ -137,26 +139,12 @@
         # Backbone
         self._backbone = FTTransformerBackbone(self.hparams)
         # Embedding Layer
         self._embedding_layer = self._backbone._build_embedding_layer()
         # Head
         self._head = self._get_head_from_config()
 
-    # def extract_embedding(self):
-    #     if self.hparams.categorical_dim > 0:
-    #         return self.embedding_layer.cat_embedding_layers
-    #     else:
-    #         raise ValueError(
-    #             "Model has been trained with no categorical feature and therefore can't be used as a Categorical Encoder"
-    #         )
-
     def feature_importance(self):
         if self.hparams.attn_feature_importance:
-            importance_df = pd.DataFrame(
-                {
-                    "Features": self.hparams.categorical_cols + self.hparams.continuous_cols,
-                    "importance": self.backbone.feature_importance_.detach().cpu().numpy(),
-                }
-            )
-            return importance_df
+            return super().feature_importance()
         else:
             raise ValueError("If you want Feature Importance, `attn_feature_weights` should be `True`.")
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/gate/components.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/gate/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         self.feature_mask_function = feature_mask_function
         self._build_network()
 
     def _build_network(self):
         for d in range(self.depth):
             for n in range(max(2 ** (d), 1)):
                 self.add_module(
-                    "decision_stump_{}_{}".format(d, n),
+                    f"decision_stump_{d}_{n}",
                     NeuralDecisionStump(
                         self.n_features + (2 ** (d) if d > 0 else 0),
                         self.binning_activation,
                         self.feature_mask_function,
                     ),
                 )
         self.dropout = nn.Dropout(self._dropout)
@@ -99,15 +99,15 @@
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         tree_input = x
         feature_masks = []
         for d in range(self.depth):
             layer_nodes = []
             layer_feature_masks = []
             for n in range(max(2 ** (d), 1)):
-                leaf_nodes, feature_mask = self._modules["decision_stump_{}_{}".format(d, n)](tree_input)
+                leaf_nodes, feature_mask = self._modules[f"decision_stump_{d}_{n}"](tree_input)
                 layer_nodes.append(leaf_nodes)
                 layer_feature_masks.append(feature_mask)
             layer_nodes = torch.cat(layer_nodes, dim=1)
             tree_input = torch.cat([x, layer_nodes], dim=1)
             feature_masks.append(layer_feature_masks)
         return self.dropout(layer_nodes), feature_masks
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/gate/config.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/gate/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""AutomaticFeatureInteraction Config"""
+"""AutomaticFeatureInteraction Config."""
 from dataclasses import dataclass, field
 
 from pytorch_tabular.config import ModelConfig
 
 
 @dataclass
 class GatedAdditiveTreeEnsembleConfig(ModelConfig):
-    """Gated Additive Tree Ensemble Config
+    """Gated Additive Tree Ensemble Config.
 
     Args:
         gflu_stages (int): Number of layers in the feature abstraction layer. Defaults to 6
 
         gflu_dropout (float): Dropout rate for the feature abstraction layer. Defaults to 0.0
 
         tree_depth (int): Depth of the tree. Defaults to 5
 
         num_trees (int): Number of trees to use in the ensemble. Defaults to 20
 
-        binning_activation (str): The binning function to use. Defaults to entmoid. Defaults to entmoid.
+        binning_activation (str): The binning function to use. Defaults to entmoid. Defaults to sparsemoid.
                 Choices are: [`entmoid`,`sparsemoid`,`sigmoid`].
 
-        feature_mask_function (str): The feature mask function to use. Defaults to entmax. Choices are:
+        feature_mask_function (str): The feature mask function to use. Defaults to sparsemax. Choices are:
                 [`entmax`,`sparsemax`,`softmax`].
 
         tree_dropout (float): probability of dropout in tree binning transformation. Defaults to 0.0
 
         chain_trees (bool): If True, we will chain the trees together. Synonymous to boosting
             (chaining trees) or bagging (parallel trees). Defaults to True
 
@@ -66,15 +66,21 @@
                 CrossEntropyLoss for classification. Unless you are sure what you are doing, leave it at MSELoss
                 or L1Loss for regression and CrossEntropyLoss for classification
 
         metrics (Optional[List[str]]): the list of metrics you need to track during training. The metrics
                 should be one of the functional metrics implemented in ``torchmetrics``. By default, it is
                 accuracy if classification and mean_squared_error for regression
 
-        metrics_params (Optional[List]): The parameters to be passed to the metrics function
+        metrics_params (Optional[List]): The parameters to be passed to the metrics function. `task` is forced to
+                be `multiclass` because the multiclass version can handle binary as well and for simplicity we are
+                only using `multiclass`.
+
+        metrics_prob_input (Optional[List]): Is a mandatory parameter for classification metrics defined in the config.
+            This defines whether the input to the metric function is the probability or the class. Length should be
+            same as the number of metrics. Defaults to None.
 
         target_range (Optional[List]): The range in which we should limit the output variable. Currently
                 ignored for multi-target regression. Typically used for Regression problems. If left empty, will
                 not apply any restrictions
 
         seed (int): The seed for reproducibility. Defaults to 42
     """
@@ -84,44 +90,45 @@
         metadata={"help": "Number of layers in the feature abstraction layer. Defaults to 6"},
     )
 
     gflu_dropout: float = field(
         default=0.0, metadata={"help": "Dropout rate for the feature abstraction layer. Defaults to 0.0"}
     )
 
-    tree_depth: int = field(default=5, metadata={"help": "Depth of the tree. Defaults to 5"})
+    tree_depth: int = field(default=4, metadata={"help": "Depth of the tree. Defaults to 5"})
 
     num_trees: int = field(
-        default=20,
+        default=10,
         metadata={"help": "Number of trees to use in the ensemble. Defaults to 20"},
     )
 
     binning_activation: str = field(
-        default="entmoid",
+        default="sparsemoid",
         metadata={
             "help": "The binning function to use. Defaults to entmoid. Defaults to entmoid",
             "choices": ["entmoid", "sparsemoid", "sigmoid"],
         },
     )
     feature_mask_function: str = field(
-        default="entmax",
+        default="sparsemax",
         metadata={
             "help": "The feature mask function to use. Defaults to entmax",
             "choices": ["entmax", "sparsemax", "softmax"],
         },
     )
 
     tree_dropout: float = field(
         default=0.0,
         metadata={"help": "probability of dropout in tree binning transformation. Defaults to 0.0"},
     )
     chain_trees: bool = field(
         default=True,
         metadata={
-            "help": "If True, we will chain the trees together. Synonymous to boosting (chaining trees) or bagging (parallel trees). Defaults to True"
+            "help": "If True, we will chain the trees together."
+            " Synonymous to boosting (chaining trees) or bagging (parallel trees). Defaults to True"
         },
     )
     tree_wise_attention: bool = field(
         default=True,
         metadata={"help": "If True, we will use tree wise attention to combine trees. Defaults to True"},
     )
     tree_wise_attention_dropout: float = field(
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/gate/gate_model.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/gate/gate_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,16 +91,17 @@
                     feature_mask_function=self.feature_mask_function,
                 )
                 for t in range(self.num_trees)
             ]
         )
         if self.tree_wise_attention:
             self.tree_attention = nn.MultiheadAttention(
-                self.output_dim,
-                1,
+                embed_dim=self.output_dim,
+                num_heads=1,
+                batch_first=False,
                 dropout=self.tree_wise_attention_dropout,
             )
 
     def _build_embedding_layer(self):
         return Embedding1dLayer(
             continuous_dim=self.n_continuous_features,
             categorical_embedding_dims=self.cat_embedding_dims,
@@ -119,20 +120,26 @@
             tree_output, feat_masks = self.trees[i](tree_input)
             tree_outputs.append(tree_output.unsqueeze(-1))
             tree_feature_masks.append(feat_masks)
             if self.chain_trees:
                 tree_input = torch.cat([tree_input, tree_output], 1)
         tree_outputs = torch.cat(tree_outputs, dim=-1)
         if self.tree_wise_attention:
-            tree_outputs, _ = self.tree_attention(tree_outputs)
+            tree_outputs = tree_outputs.permute(2, 0, 1)
+            tree_outputs, _ = self.tree_attention(tree_outputs, tree_outputs, tree_outputs)
+            tree_outputs = tree_outputs.permute(1, 2, 0)
         return tree_outputs
 
+    @property
+    def feature_importance_(self):
+        return self.gflus.feature_mask_function(self.gflus.feature_masks).sum(dim=0).detach().cpu().numpy()
+
 
 class CustomHead(nn.Module):
-    """Custom Head for GATE
+    """Custom Head for GATE.
 
     Args:
         input_dim (int): Input dimension of the head
         hparams (DictConfig): Config of the model
     """
 
     def __init__(self, input_dim: int, hparams: DictConfig):
@@ -206,14 +213,16 @@
             num_trees=self.hparams.num_trees,
             tree_depth=self.hparams.tree_depth,
             tree_dropout=self.hparams.tree_dropout,
             binning_activation=self.hparams.binning_activation,
             feature_mask_function=self.hparams.feature_mask_function,
             batch_norm_continuous_input=self.hparams.batch_norm_continuous_input,
             chain_trees=self.hparams.chain_trees,
+            tree_wise_attention=self.hparams.tree_wise_attention,
+            tree_wise_attention_dropout=self.hparams.tree_wise_attention_dropout,
         )
         # Embedding Layer
         self._embedding_layer = self._backbone._build_embedding_layer()
         # Head
         self._head = CustomHead(self.backbone.output_dim, self.hparams)
 
     def data_aware_initialization(self, datamodule):
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/mixture_density/config.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/mixture_density/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""Mixture Density Head Config"""
+"""Mixture Density Head Config."""
 from dataclasses import dataclass, field
 from typing import Dict
 
 from pytorch_tabular.config.config import ModelConfig
 
 INCOMPATIBLE_BACKBONES = ["NodeConfig", "TabNetModelConfig", "MDNConfig"]
 
@@ -43,27 +43,34 @@
                 CrossEntropyLoss for classification. Unless you are sure what you are doing, leave it at MSELoss
                 or L1Loss for regression and CrossEntropyLoss for classification
 
         metrics (Optional[List[str]]): the list of metrics you need to track during training. The metrics
                 should be one of the functional metrics implemented in ``torchmetrics``. By default, it is
                 accuracy if classification and mean_squared_error for regression
 
-        metrics_params (Optional[List]): The parameters to be passed to the metrics function
+        metrics_params (Optional[List]): The parameters to be passed to the metrics function. `task` is forced to
+                be `multiclass` because the multiclass version can handle binary as well and for simplicity we are
+                only using `multiclass`.
+
+        metrics_prob_input (Optional[List]): Is a mandatory parameter for classification metrics defined in the config.
+            This defines whether the input to the metric function is the probability or the class. Length should be
+            same as the number of metrics. Defaults to None.
 
         target_range (Optional[List]): The range in which we should limit the output variable. Currently
                 ignored for multi-target regression. Typically used for Regression problems. If left empty, will
                 not apply any restrictions
 
         seed (int): The seed for reproducibility. Defaults to 42
     """
 
     backbone_config_class: str = field(
         default=None,
         metadata={
-            "help": "The config class for defining the Backbone. The config class should be a valid module path from `models`. e.g. `FTTransformerConfig`"
+            "help": "The config class for defining the Backbone."
+            " The config class should be a valid module path from `models`. e.g. `FTTransformerConfig`"
         },
     )
     backbone_config_params: Dict = field(
         default=None,
         metadata={"help": "The dict of config parameters for defining the Backbone."},
     )
     head: str = field(init=False, default="MixtureDensityHead")
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/mixture_density/mdn.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/mixture_density/mdn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""Mixture Density Models"""
+"""Mixture Density Models."""
 import warnings
 from typing import Dict, Optional, Union
 
 import torch
 import torch.nn as nn
 from omegaconf import DictConfig, OmegaConf
 from torch import Tensor
@@ -62,15 +62,17 @@
             self.hparams.backbone_config_class,
             self.hparams.backbone_config_params,
         )
         try:
             callable = getattr(models, callable)
         except ModuleNotFoundError as e:
             logger.error(
-                "`config class` in `backbone_config` is not valid. The config class should be a valid module path from `models`. e.g. `ft_transformer.FTTransformerConfig`."
+                "`config class` in `backbone_config` is not valid."
+                " The config class should be a valid module path from `models`."
+                " e.g. `ft_transformer.FTTransformerConfig`."
             )
             raise e
         assert issubclass(callable, ModelConfig), "`config_class` should be a subclass of `ModelConfig`"
         backbone_config = callable(**config)
         backbone_callable = getattr_nested(backbone_config._module_src, backbone_config._backbone_name)
         # Merging the config and inferred config
         backbone_config = safe_merge_config(OmegaConf.structured(backbone_config), self.inferred_config)
@@ -80,16 +82,16 @@
         # Head
         self._head = self._get_head_from_config()
 
     # Redefining forward because TabTransformer flow is slightly different
     def forward(self, x: Dict):
         if isinstance(self.backbone, TabTransformerBackbone):
             if self.hparams.categorical_dim > 0:
-                x_cat = self.embed_input(dict(categorical=x["categorical"]))
-            x = self.compute_backbone(dict(categorical=x_cat, continuous=x["continuous"]))
+                x_cat = self.embed_input({"categorical": x["categorical"]})
+            x = self.compute_backbone({"categorical": x_cat, "continuous": x["continuous"]})
         else:
             x = self.embedding_layer(x)
             x = self.compute_backbone(x)
         return self.compute_head(x)
 
         # Redefining compute_backbone because TabTransformer flow flow is slightly different
 
@@ -154,31 +156,31 @@
         y = batch["target"]
         ret_value = self(batch)
         loss = self.calculate_loss(y, ret_value["pi"], ret_value["sigma"], ret_value["mu"], tag="train")
         if self.head.hparams.speedup_training:
             pass
         else:
             y_hat = self.head.generate_point_predictions(ret_value["pi"], ret_value["sigma"], ret_value["mu"])
-            _ = self.calculate_metrics(y, y_hat, tag="train")
+            self.calculate_metrics(y, y_hat, tag="train")
         return loss
 
     def validation_step(self, batch, batch_idx):
         y = batch["target"]
         ret_value = self(batch)
-        _ = self.calculate_loss(y, ret_value["pi"], ret_value["sigma"], ret_value["mu"], tag="valid")
+        self.calculate_loss(y, ret_value["pi"], ret_value["sigma"], ret_value["mu"], tag="valid")
         y_hat = self.head.generate_point_predictions(ret_value["pi"], ret_value["sigma"], ret_value["mu"])
-        _ = self.calculate_metrics(y, y_hat, tag="valid")
+        self.calculate_metrics(y, y_hat, tag="valid")
         return y_hat, y, ret_value
 
     def test_step(self, batch, batch_idx):
         y = batch["target"]
         ret_value = self(batch)
-        _ = self.calculate_loss(y, ret_value["pi"], ret_value["sigma"], ret_value["mu"], tag="test")
+        self.calculate_loss(y, ret_value["pi"], ret_value["sigma"], ret_value["mu"], tag="test")
         y_hat = self.head.generate_point_predictions(ret_value["pi"], ret_value["sigma"], ret_value["mu"])
-        _ = self.calculate_metrics(y, y_hat, tag="test")
+        self.calculate_metrics(y, y_hat, tag="test")
         return y_hat, y
 
     def validation_epoch_end(self, outputs) -> None:
         pi = [
             nn.functional.gumbel_softmax(output[2]["pi"], tau=self.head.hparams.softmax_temperature, dim=-1)
             for output in outputs
         ]
@@ -224,15 +226,15 @@
                 {
                     "valid_logits": fig,
                     "global_step": self.global_step,
                 },
                 commit=False,
             )
             if self.head.hparams.log_debug_plot:
-                fig = self.create_plotly_histogram(pi, "pi", bin_dict=dict(start=0.0, end=1.0, size=0.1))
+                fig = self.create_plotly_histogram(pi, "pi", bin_dict={"start": 0.0, "end": 1.0, "size": 0.1})
                 wandb.log(
                     {
                         "valid_pi": fig,
                         "global_step": self.global_step,
                     },
                     commit=False,
                 )
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/node/architecture_blocks.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/node/architecture_blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Neural Oblivious Decision Ensembles
 # Author: Sergey Popov, Julian Qian
 # https://github.com/Qwicen/node
 # For license information, see https://github.com/Qwicen/node/blob/master/LICENSE.md
-"""Dense ODST Block"""
+"""Dense ODST Block."""
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from .odst import ODST
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/node/config.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/node/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,21 @@
                 CrossEntropyLoss for classification. Unless you are sure what you are doing, leave it at MSELoss
                 or L1Loss for regression and CrossEntropyLoss for classification
 
         metrics (Optional[List[str]]): the list of metrics you need to track during training. The metrics
                 should be one of the functional metrics implemented in ``torchmetrics``. By default, it is
                 accuracy if classification and mean_squared_error for regression
 
-        metrics_params (Optional[List]): The parameters to be passed to the metrics function
+        metrics_params (Optional[List]): The parameters to be passed to the metrics function. `task` is forced to
+                be `multiclass` because the multiclass version can handle binary as well and for simplicity we are
+                only using `multiclass`.
+
+        metrics_prob_input (Optional[List]): Is a mandatory parameter for classification metrics defined in the config.
+            This defines whether the input to the metric function is the probability or the class. Length should be
+            same as the number of metrics. Defaults to None.
 
         target_range (Optional[List]): The range in which we should limit the output variable. Currently
                 ignored for multi-target regression. Typically used for Regression problems. If left empty, will
                 not apply any restrictions
 
         seed (int): The seed for reproducibility. Defaults to 42
     """
@@ -112,49 +118,53 @@
     num_trees: int = field(
         default=2048,
         metadata={"help": "Number of Oblivious Decision Trees in each layer"},
     )
     additional_tree_output_dim: int = field(
         default=3,
         metadata={
-            "help": "The additional output dimensions which is only used to pass through different layers of the architectures. Only the first output_dim outputs will be used for prediction"
+            "help": "The additional output dimensions which is only used to pass through different layers"
+            " of the architectures. Only the first output_dim outputs will be used for prediction"
         },
     )
     depth: int = field(
         default=6,
         metadata={"help": "The depth of the individual Oblivious Decision Trees"},
     )
     choice_function: str = field(
         default="entmax15",
         metadata={
-            "help": "Generates a sparse probability distribution to be used as feature weights(aka, soft feature selection)",
+            "help": "Generates a sparse probability distribution to be used"
+            " as feature weights(aka, soft feature selection)",
             "choices": ["entmax15", "sparsemax"],
         },
     )
     bin_function: str = field(
         default="entmoid15",
         metadata={
             "help": "Generates a sparse probability distribution to be used as tree leaf weights",
             "choices": ["entmoid15", "sparsemoid"],
         },
     )
     max_features: Optional[int] = field(
         default=None,
         metadata={
-            "help": "If not None, sets a max limit on the number of features to be carried forward from layer to layer in the Dense Architecture"
+            "help": "If not None, sets a max limit on the number of features to be carried forward"
+            " from layer to layer in the Dense Architecture"
         },
     )
     input_dropout: float = field(
         default=0.0,
         metadata={"help": "Dropout to be applied to the inputs between layers of the Dense Architecture"},
     )
     initialize_response: str = field(
         default="normal",
         metadata={
-            "help": "Initializing the response variable in the Oblivious Decision Trees. By default, it is a standard normal distribution",
+            "help": "Initializing the response variable in the Oblivious Decision Trees."
+            " By default, it is a standard normal distribution",
             "choices": ["normal", "uniform"],
         },
     )
     initialize_selection_logits: str = field(
         default="uniform",
         metadata={
             "help": "Initializing the feature selector. By default is a uniform distribution across the features",
@@ -182,49 +192,55 @@
                 Used in the Data-aware initialization of scales(used in the scaling ODTs).
                 It is initialized in such a way that all the samples in the first batch belong to the linear
                 region of the entmoid/sparsemoid(bin-selectors) and thereby have non-zero gradients
                 Threshold log-temperatures initializer, in (0, inf)
                 By default(1.0), log-temperatures are initialized in such a way that all bin selectors
                 end up in the linear region of sparse-sigmoid. The temperatures are then scaled by this parameter.
                 Setting this value > 1.0 will result in some margin between data points and sparse-sigmoid cutoff value
-                Setting this value < 1.0 will cause (1 - value) part of data points to end up in flat sparse-sigmoid region
-                For instance, threshold_init_cutoff = 0.9 will set 10% points equal to 0.0 or 1.0
+                Setting this value < 1.0 will cause (1 - value) part of data points to end up in flat sparse-sigmoid
+                region. For instance, threshold_init_cutoff = 0.9 will set 10% points equal to 0.0 or 1.0
                 Setting this value > 1.0 will result in a margin between data points and sparse-sigmoid cutoff value
                 All points will be between (0.5 - 0.5 / threshold_init_cutoff) and (0.5 + 0.5 / threshold_init_cutoff)
             """
         },
     )
     cat_embedding_dropout: float = field(
         default=0.0,
         metadata={
-            "help": "DEPRECATED: Please use `embedding_dropout` instead. probability of an embedding element to be zeroed."
+            "help": "DEPRECATED: Please use `embedding_dropout` instead."
+            " probability of an embedding element to be zeroed."
         },
     )
 
     embed_categorical: bool = field(
         default=False,
         metadata={
-            "help": "Flag to embed categorical columns using an Embedding Layer. If turned off, the categorical columns are encoded using LeaveOneOutEncoder. This is DEPRECATED and will always be `True` from next release."
+            "help": "Flag to embed categorical columns using an Embedding Layer."
+            " If turned off, the categorical columns are encoded using LeaveOneOutEncoder."
+            " This is DEPRECATED and will always be `True` from next release."
         },
     )
 
     _module_src: str = field(default="models.node")
     _model_name: str = field(default="NODEModel")
     _backbone_name: str = field(default="NODEBackbone")
     _config_name: str = field(default="NodeConfig")
 
     def __post_init__(self):
         if not self.embed_categorical:
             # raise deprecation warning
             warnings.warn(
-                "embed_categorical is set to False and will use LeaveOneOutEncoder to encode categorical features. This is deprecated and will be removed in future versions and categorical columns will be embedded by default."
+                "embed_categorical is set to False and will use LeaveOneOutEncoder to encode categorical features."
+                " This is deprecated and will be removed in future versions and categorical columns"
+                " will be embedded by default."
             )
         if self.cat_embedding_dropout > 0:
             warnings.warn(
-                "`cat_embedding_dropout` is deprecated and will be removed in the next release. Please use `embedding_dropout` instead"
+                "`cat_embedding_dropout` is deprecated and will be removed in the next release."
+                " Please use `embedding_dropout` instead"
             )
             self.embedding_dropout = self.cat_embedding_dropout
         super().__post_init__()
 
 
 # if __name__ == "__main__":
 #     from pytorch_tabular.utils import generate_doc_dataclass
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/node/node_model.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/node/node_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""Tabular Model"""
+"""Tabular Model."""
 import warnings
 
 import torch
 import torch.nn as nn
 from omegaconf import DictConfig
 
 from pytorch_tabular.models.common.layers import Embedding1dLayer, PreEncoded1dLayer
@@ -19,15 +19,16 @@
 logger = get_logger(__name__)
 
 
 class NODEBackbone(nn.Module):
     def __init__(self, config: DictConfig, **kwargs):
         super().__init__()
         self.hparams = config
-        # self.hparams.output_dim = (0 if self.hparams.output_dim is None else self.hparams.output_dim)  # For SSL cases where output_dim will be None
+        # self.hparams.output_dim = (0 if self.hparams.output_dim is None else self.hparams.output_dim)
+        # For SSL cases where output_dim will be None
         self._build_network()
 
     def _build_network(self):
         if self.hparams.embed_categorical:
             self.hparams.node_input_dim = self.hparams.continuous_dim + self.hparams.embedded_cat_dim
         else:
             self.hparams.node_input_dim = self.hparams.continuous_dim + self.hparams.categorical_dim
@@ -74,15 +75,15 @@
     def __init__(self, config: DictConfig, **kwargs):
         super().__init__(config, **kwargs)
 
     def subset(self, x):
         return x[..., : self.hparams.output_dim].mean(dim=-2)
 
     def data_aware_initialization(self, datamodule):
-        """Performs data-aware initialization for NODE"""
+        """Performs data-aware initialization for NODE."""
         logger.info("Data Aware Initialization of NODE using a forward pass with 2000 batch size....")
         # Need a big batch to initialize properly
         alt_loader = datamodule.train_dataloader(batch_size=self.hparams.data_aware_init_batch_size)
         batch = next(iter(alt_loader))
         for k, v in batch.items():
             if isinstance(v, list) and (len(v) == 0):
                 # Skipping empty list
@@ -111,16 +112,7 @@
         # Embedding Layer
         self._embedding_layer = self._backbone._build_embedding_layer()
         # average first n channels of every tree, where n is the number of output targets for regression
         # and number of classes for classification
         # Not using config head because NODE has a specific head
         warnings.warn("Ignoring head config because NODE has a specific head which subsets the tree outputs")
         self._head = Lambda(self.subset)
-
-    # def extract_embedding(self):
-    #     if self.hparams.embed_categorical:
-    #         if self.hparams.embedded_cat_dim != 0:
-    #             return self.embedding_layer.cat_embedding_layers
-    #     else:
-    #         raise ValueError(
-    #             "Model has been trained with no categorical feature and therefore can't be used as a Categorical Encoder"
-    #         )
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/node/odst.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/node/odst.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Neural Oblivious Decision Ensembles
 # Author: Sergey Popov, Julian Qian
 # https://github.com/Qwicen/node
 # For license information, see https://github.com/Qwicen/node/blob/master/LICENSE.md
-"""Dense ODST Block"""
+"""Dense ODST Block."""
 from warnings import warn
 
 import numpy as np
 import torch
 import torch.nn as nn
 
 from ..common.activations import sparsemax, sparsemoid
 from ..common.layers import ModuleWithInit
 
 
 def check_numpy(x):
-    """Makes sure x is a numpy array"""
+    """Makes sure x is a numpy array."""
     if isinstance(x, torch.Tensor):
         x = x.detach().cpu().numpy()
     x = np.asarray(x)
     assert isinstance(x, np.ndarray)
     return x
 
 
@@ -33,17 +33,17 @@
         choice_function=sparsemax,
         bin_function=sparsemoid,
         initialize_response_=nn.init.normal_,
         initialize_selection_logits_=nn.init.uniform_,
         threshold_init_beta=1.0,
         threshold_init_cutoff=1.0,
     ):
-        """
-        Oblivious Differentiable Sparsemax Trees. http://tinyurl.com/odst-readmore
-        One can drop (sic!) this module anywhere instead of nn.Linear
+        """Oblivious Differentiable Sparsemax Trees. http://tinyurl.com/odst-readmore One can drop (sic!) this module
+        anywhere instead of nn.Linear.
+
         :param in_features: number of features in the input tensor
         :param num_trees: number of trees in this layer
         :param tree_dim: number of response channels in the response of individual tree
         :param depth: number of splits in every tree
         :param flatten_output: if False, returns [..., num_trees, tree_dim],
             by default returns [..., num_trees * tree_dim]
         :param choice_function: f(tensor, dim) -> R_simplex computes feature weights s.t. f(tensor, dim).sum(dim) == 1
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/tab_transformer/config.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/tab_transformer/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""AutomaticFeatureInteraction Config"""
+"""AutomaticFeatureInteraction Config."""
 import warnings
 from dataclasses import dataclass, field
 from typing import Optional
 
 from pytorch_tabular.config import ModelConfig
 from pytorch_tabular.utils import ifnone
 
@@ -95,15 +95,21 @@
                 CrossEntropyLoss for classification. Unless you are sure what you are doing, leave it at MSELoss
                 or L1Loss for regression and CrossEntropyLoss for classification
 
         metrics (Optional[List[str]]): the list of metrics you need to track during training. The metrics
                 should be one of the functional metrics implemented in ``torchmetrics``. By default, it is
                 accuracy if classification and mean_squared_error for regression
 
-        metrics_params (Optional[List]): The parameters to be passed to the metrics function
+        metrics_params (Optional[List]): The parameters to be passed to the metrics function. `task` is forced to
+                be `multiclass` because the multiclass version can handle binary as well and for simplicity we are
+                only using `multiclass`.
+
+        metrics_prob_input (Optional[List]): Is a mandatory parameter for classification metrics defined in the config.
+            This defines whether the input to the metric function is the probability or the class. Length should be
+            same as the number of metrics. Defaults to None.
 
         target_range (Optional[List]): The range in which we should limit the output variable. Currently
                 ignored for multi-target regression. Typically used for Regression problems. If left empty, will
                 not apply any restrictions
 
         seed (int): The seed for reproducibility. Defaults to 42
     """
@@ -122,42 +128,51 @@
     embedding_bias: bool = field(
         default=False,
         metadata={"help": "Flag to turn on Embedding Bias. Defaults to False"},
     )
     share_embedding: bool = field(
         default=False,
         metadata={
-            "help": "The flag turns on shared embeddings in the input embedding process. The key idea here is to have an embedding for the feature as a whole along with embeddings of each unique values of that column. For more details refer to Appendix A of the TabTransformer paper. Defaults to False"
+            "help": "The flag turns on shared embeddings in the input embedding process."
+            " The key idea here is to have an embedding for the feature as a whole along with embeddings"
+            " of each unique values of that column. For more details refer"
+            " to Appendix A of the TabTransformer paper. Defaults to False"
         },
     )
     share_embedding_strategy: Optional[str] = field(
         default="fraction",
         metadata={
-            "help": "There are two strategies in adding shared embeddings. 1. `add` - A separate embedding for the feature is added to the embedding of the unique values of the feature. 2. `fraction` - A fraction of the input embedding is reserved for the shared embedding of the feature. Defaults to fraction.",
+            "help": "There are two strategies in adding shared embeddings."
+            " 1. `add` - A separate embedding for the feature is added to the embedding"
+            " of the unique values of the feature."
+            " 2. `fraction` - A fraction of the input embedding is reserved"
+            " for the shared embedding of the feature. Defaults to fraction.",
             "choices": ["add", "fraction"],
         },
     )
     shared_embedding_fraction: float = field(
         default=0.25,
         metadata={
-            "help": "Fraction of the input_embed_dim to be reserved by the shared embedding. Should be less than one. Defaults to 0.25"
+            "help": "Fraction of the input_embed_dim to be reserved by the shared embedding."
+            " Should be less than one. Defaults to 0.25"
         },
     )
     num_heads: int = field(
         default=8,
         metadata={"help": "The number of heads in the Multi-Headed Attention layer. Defaults to 8"},
     )
     num_attn_blocks: int = field(
         default=6,
         metadata={"help": "The number of layers of stacked Multi-Headed Attention layers. Defaults to 6"},
     )
     transformer_head_dim: Optional[int] = field(
         default=None,
         metadata={
-            "help": "The number of hidden units in the Multi-Headed Attention layers. Defaults to None and will be same as input_dim."
+            "help": "The number of hidden units in the Multi-Headed Attention layers."
+            " Defaults to None and will be same as input_dim."
         },
     )
     attn_dropout: float = field(
         default=0.1,
         metadata={"help": "Dropout to be applied after Multi headed Attention. Defaults to 0.1"},
     )
     add_norm_dropout: float = field(
@@ -171,27 +186,34 @@
     ff_hidden_multiplier: int = field(
         default=4,
         metadata={"help": "Multiple by which the Positionwise FF layer scales the input. Defaults to 4"},
     )
     transformer_activation: str = field(
         default="GEGLU",
         metadata={
-            "help": "The activation type in the transformer feed forward layers. In addition to the default activation in PyTorch like ReLU, TanH, LeakyReLU, etc. https://pytorch.org/docs/stable/nn.html#non-linear-activations-weighted-sum-nonlinearity, GEGLU, ReGLU and SwiGLU are also implemented(https://arxiv.org/pdf/2002.05202.pdf). Defaults to GEGLU",
+            "help": "The activation type in the transformer feed forward layers."
+            " In addition to the default activation in PyTorch like ReLU, TanH, LeakyReLU, etc."
+            " https://pytorch.org/docs/stable/nn.html#non-linear-activations-weighted-sum-nonlinearity,"
+            " GEGLU, ReGLU and SwiGLU are also implemented(https://arxiv.org/pdf/2002.05202.pdf)."
+            " Defaults to GEGLU",
         },
     )
     out_ff_layers: Optional[str] = field(
         default=None,
         metadata={
             "help": "DEPRECATED: Hyphen-separated number of layers and units in the deep MLP. Defaults to 128-64-32"
         },
     )
     out_ff_activation: Optional[str] = field(
         default=None,
         metadata={
-            "help": "DEPRECATED: The activation type in the deep MLP. The default activaion in PyTorch like ReLU, TanH, LeakyReLU, etc. https://pytorch.org/docs/stable/nn.html#non-linear-activations-weighted-sum-nonlinearity. Defaults to ReLU"
+            "help": "DEPRECATED: The activation type in the deep MLP. The default activaion in PyTorch"
+            " like ReLU, TanH, LeakyReLU, etc."
+            " https://pytorch.org/docs/stable/nn.html#non-linear-activations-weighted-sum-nonlinearity."
+            " Defaults to ReLU"
         },
     )
     out_ff_dropout: Optional[float] = field(
         default=None,
         metadata={
             "help": "DEPRECATED: probability of an classification element to be zeroed in the deep MLP. Defaults to 0.0"
         },
@@ -213,30 +235,33 @@
             "out_ff_layers",
             "out_ff_activation",
             "out_ff_dropoout",
             "out_ff_initialization",
         ]
         if self.head_config != {"layers": ""}:  # If the user has passed a head_config
             warnings.warn(
-                "Ignoring the deprecated arguments, `out_ff_layers`, `out_ff_activation`, `out_ff_dropoout`, and `out_ff_initialization` as head_config is passed."
+                "Ignoring the deprecated arguments, `out_ff_layers`, `out_ff_activation`, `out_ff_dropoout`,"
+                " and `out_ff_initialization` as head_config is passed."
             )
         else:
-            if any([p is not None for p in deprecated_args]):
+            if any(p is not None for p in deprecated_args):
                 warnings.warn(
-                    "The `out_ff_layers`, `out_ff_activation`, `out_ff_dropoout`, and `out_ff_initialization` arguments are deprecated and will be removed next release. Please use head and head_config as an alternative.",
+                    "The `out_ff_layers`, `out_ff_activation`, `out_ff_dropoout`, and `out_ff_initialization`"
+                    " arguments are deprecated and will be removed next release."
+                    " Please use head and head_config as an alternative.",
                     DeprecationWarning,
                 )
                 # TODO: Remove this once we deprecate the old config
                 # Fill the head_config using deprecated parameters
-                self.head_config = dict(
-                    layers=ifnone(self.out_ff_layers, ""),
-                    activation=ifnone(self.out_ff_activation, "ReLU"),
-                    dropout=ifnone(self.out_ff_dropout, 0.0),
-                    use_batch_norm=False,
-                    initialization=ifnone(self.out_ff_initialization, "kaiming"),
-                )
+                self.head_config = {
+                    "layers": ifnone(self.out_ff_layers, ""),
+                    "activation": ifnone(self.out_ff_activation, "ReLU"),
+                    "dropout": ifnone(self.out_ff_dropout, 0.0),
+                    "use_batch_norm": False,
+                    "initialization": ifnone(self.out_ff_initialization, "kaiming"),
+                }
         return super().__post_init__()
 
 
 # if __name__ == "__main__":
 #     from pytorch_tabular.utils import generate_doc_dataclass
 #     print(generate_doc_dataclass(TabTransformerConfig))
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/tab_transformer/tab_transformer.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/tab_transformer/tab_transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # 2. PyTorch Wide and Deep - https://github.com/jrzaurin/pytorch-widedeep/
 # It is another library for tabular data, which supports multi modal problems.
 # Check out the library if you haven't already.
 # 3. AutoGluon - https://github.com/awslabs/autogluon
 # AutoGluon is an AuttoML library which supports Tabular data as well. it is from Amazon Research and is in MXNet
 # 4. LabML Annotated Deep Learning Papers - The position-wise FF was shamelessly copied from
 # https://github.com/labmlai/annotated_deep_learning_paper_implementations/tree/master/labml_nn/transformers
-"""TabTransformer Model"""
+"""TabTransformer Model."""
 from collections import OrderedDict
 from typing import Dict
 
 import torch
 import torch.nn as nn
 from einops import rearrange
 from omegaconf import DictConfig
@@ -26,15 +26,18 @@
 
 class TabTransformerBackbone(nn.Module):
     def __init__(self, config: DictConfig):
         super().__init__()
         assert config.share_embedding_strategy in [
             "add",
             "fraction",
-        ], f"`share_embedding_strategy` should be one of `add` or `fraction`, not {self.hparams.share_embedding_strategy}"
+        ], (
+            f"`share_embedding_strategy` should be one of `add` or `fraction`,"
+            f" not {self.hparams.share_embedding_strategy}"
+        )
         self.hparams = config
         self._build_network()
 
     def _build_network(self):
         self.transformer_blocks = OrderedDict()
         for i in range(self.hparams.num_attn_blocks):
             self.transformer_blocks[f"mha_block_{i}"] = TransformerEncoderBlock(
@@ -107,24 +110,18 @@
         self._embedding_layer = self._backbone._build_embedding_layer()
         # Head
         self._head = self._get_head_from_config()
 
     # Redefining forward because this model flow is slightly different
     def forward(self, x: Dict):
         if self.hparams.categorical_dim > 0:
-            x_cat = self.embed_input(dict(categorical=x["categorical"]))
-        x = self.compute_backbone(dict(categorical=x_cat, continuous=x["continuous"]))
+            x_cat = self.embed_input({"categorical": x["categorical"]})
+        else:
+            x_cat = None
+        x = self.compute_backbone({"categorical": x_cat, "continuous": x["continuous"]})
         return self.compute_head(x)
 
     # Redefining compute_backbone because this model flow is slightly different
     def compute_backbone(self, x: Dict):
         # Returns output
         x = self.backbone(x["categorical"], x["continuous"])
         return x
-
-    # def extract_embedding(self):
-    #     if self.hparams.categorical_dim > 0:
-    #         return self.embedding_layer.cat_embedding_layers
-    #     else:
-    #         raise ValueError(
-    #             "Model has been trained with no categorical feature and therefore can't be used as a Categorical Encoder"
-    #         )
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/tabnet/config.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/tabnet/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""Tabnet Model Config"""
+"""Tabnet Model Config."""
 from dataclasses import dataclass, field
 
 from pytorch_tabular.config import ModelConfig
 
 
 @dataclass
 class TabNetModelConfig(ModelConfig):
@@ -55,15 +55,21 @@
                 CrossEntropyLoss for classification. Unless you are sure what you are doing, leave it at MSELoss
                 or L1Loss for regression and CrossEntropyLoss for classification
 
         metrics (Optional[List[str]]): the list of metrics you need to track during training. The metrics
                 should be one of the functional metrics implemented in ``torchmetrics``. By default, it is
                 accuracy if classification and mean_squared_error for regression
 
-        metrics_params (Optional[List]): The parameters to be passed to the metrics function
+        metrics_params (Optional[List]): The parameters to be passed to the metrics function. `task` is forced to
+                be `multiclass` because the multiclass version can handle binary as well and for simplicity we are
+                only using `multiclass`.
+
+        metrics_prob_input (Optional[List]): Is a mandatory parameter for classification metrics defined in the config.
+            This defines whether the input to the metric function is the probability or the class. Length should be
+            same as the number of metrics. Defaults to None.
 
         target_range (Optional[List]): The range in which we should limit the output variable. Currently
                 ignored for multi-target regression. Typically used for Regression problems. If left empty, will
                 not apply any restrictions
 
         seed (int): The seed for reproducibility. Defaults to 42
     """
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/models/tabnet/tabnet_model.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/models/tabnet/tabnet_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""TabNet Model"""
+"""TabNet Model."""
 from typing import Dict
 
 import torch
 import torch.nn as nn
 from omegaconf import DictConfig
 from pytorch_tabnet.tab_network import TabNet
 
@@ -22,15 +22,15 @@
         self.tabnet = TabNet(
             input_dim=self.hparams.continuous_dim + self.hparams.categorical_dim,
             output_dim=self.hparams.output_dim,
             n_d=self.hparams.n_d,
             n_a=self.hparams.n_a,
             n_steps=self.hparams.n_steps,
             gamma=self.hparams.gamma,
-            cat_idxs=[i for i in range(self.hparams.categorical_dim)],
+            cat_idxs=list(range(self.hparams.categorical_dim)),
             cat_dims=[cardinality for cardinality, _ in self.hparams.embedding_dims],
             cat_emb_dim=[embed_dim for _, embed_dim in self.hparams.embedding_dims],
             n_independent=self.hparams.n_independent,
             n_shared=self.hparams.n_shared,
             epsilon=1e-15,
             virtual_batch_size=self.hparams.virtual_batch_size,
             momentum=0.02,
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/base_model.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/base_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""SSL Base Model"""
+"""SSL Base Model."""
 import warnings
 from abc import ABCMeta, abstractmethod
 from typing import Dict, Optional
 
 import pytorch_lightning as pl
 import torch
 import torch.nn as nn
@@ -23,16 +23,15 @@
         base_config: The base configuration.
         custom_config: The custom configuration.
 
     Returns:
         The merged configuration.
     """
     # using base config values if exist
-    if "embedding_dims" in config.keys() and config.embedding_dims is not None:
-        inferred_config.embedding_dims = config.embedding_dims
+    inferred_config.embedding_dims = config.get("embedding_dims") or inferred_config.embedding_dims
     merged_config = OmegaConf.merge(OmegaConf.to_container(config), OmegaConf.to_container(inferred_config))
     return merged_config
 
 
 class SSLBaseModel(pl.LightningModule, metaclass=ABCMeta):
     def __init__(
         self,
@@ -71,15 +70,16 @@
         self._setup_loss()
         self._setup_metrics()
 
     def _setup_encoder_decoder(self, encoder, encoder_config, decoder, decoder_config, inferred_config):
         assert (encoder is not None) or (
             encoder_config is not None
         ), "Either encoder or encoder_config must be provided"
-        # assert (decoder is not None) or (decoder_config is not None), "Either decoder or decoder_config must be provided"
+        # assert (decoder is not None) or (decoder_config is not None),
+        # "Either decoder or decoder_config must be provided"
         if encoder is not None:
             self.encoder = encoder
             self._custom_decoder = True
         else:
             # Since encoder is not provided, we will use the encoder_config
             model_callable = getattr_nested(encoder_config._module_src, encoder_config._backbone_name)
             self.encoder = model_callable(
@@ -143,29 +143,29 @@
 
     def data_aware_initialization(self, datamodule):
         pass
 
     def training_step(self, batch, batch_idx):
         output = self.forward(batch)
         loss = self.calculate_loss(output, tag="train")
-        _ = self.calculate_metrics(output, tag="train")
+        self.calculate_metrics(output, tag="train")
         return loss
 
     def validation_step(self, batch, batch_idx):
         with torch.no_grad():
             output = self.forward(batch)
-            _ = self.calculate_loss(output, tag="valid")
-            _ = self.calculate_metrics(output, tag="valid")
+            self.calculate_loss(output, tag="valid")
+            self.calculate_metrics(output, tag="valid")
         return output
 
     def test_step(self, batch, batch_idx):
         with torch.no_grad():
             output = self.forward(batch)
-            _ = self.calculate_loss(output, tag="test")
-            _ = self.calculate_metrics(output, tag="test")
+            self.calculate_loss(output, tag="test")
+            self.calculate_metrics(output, tag="test")
         return output
 
     def validation_epoch_end(self, outputs) -> None:
         if hasattr(self.hparams, "log_logits") and self.hparams.log_logits:
             warnings.warn("Logging Logits is disabled for SSL tasks")
 
     def configure_optimizers(self):
@@ -181,37 +181,33 @@
             except AttributeError as e:
                 logger.error(f"{self.hparams.optimizer} is not a valid optimizer defined in the torch.optim module")
                 raise e
         else:
             # Loading from custom fit arguments
             self._optimizer = self.custom_optimizer
 
-            opt = self._optimizer(
-                self.parameters(),
-                lr=self.hparams.learning_rate,
-                **self.custom_optimizer_params,
-            )
+            opt = self._optimizer(self.parameters(), lr=self.hparams.learning_rate, **self.custom_optimizer_params)
         if self.hparams.lr_scheduler is not None:
             try:
                 self._lr_scheduler = getattr(torch.optim.lr_scheduler, self.hparams.lr_scheduler)
             except AttributeError as e:
                 logger.error(
-                    f"{self.hparams.lr_scheduler} is not a valid learning rate sheduler defined in the torch.optim.lr_scheduler module"
+                    f"{self.hparams.lr_scheduler} is not a valid learning rate sheduler defined"
+                    f" in the torch.optim.lr_scheduler module"
                 )
                 raise e
             if isinstance(self._lr_scheduler, torch.optim.lr_scheduler._LRScheduler):
                 return {
                     "optimizer": opt,
                     "lr_scheduler": self._lr_scheduler(opt, **self.hparams.lr_scheduler_params),
                 }
-            else:
-                return {
-                    "optimizer": opt,
-                    "lr_scheduler": self._lr_scheduler(opt, **self.hparams.lr_scheduler_params),
-                    "monitor": self.hparams.lr_scheduler_monitor_metric,
-                }
+            return {
+                "optimizer": opt,
+                "lr_scheduler": self._lr_scheduler(opt, **self.hparams.lr_scheduler_params),
+                "monitor": self.hparams.lr_scheduler_monitor_metric,
+            }
         else:
             return opt
 
     def reset_weights(self):
         reset_all_weights(self.featurizer)
         reset_all_weights(self.embedding_layer)
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/common/augmentations.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/common/augmentations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 from typing import Dict
 
 import numpy as np
 import torch
 
 
 def mixup(batch: Dict, lam: float = 0.5) -> Dict:
-    """It apply mixup augmentation, making a weighted average between a tensor
-    and some random element of the tensor taking random rows
+    """It apply mixup augmentation, making a weighted average between a tensor and some random element of the tensor
+    taking random rows.
 
     :param batch: Tensor on which apply the mixup augmentation
     :param lam: weight in the linear combination between the original values
         and the random permutation
     """
     result = {}
     for key, value in batch.items():
         random_index = _get_random_index(value)
         result[key] = lam * value + (1 - lam) * value[random_index, :]
         result[key] = result[key].to(dtype=value.dtype)
     return result
 
 
 def cutmix(batch: Dict, lam: float = 0.1) -> Dict:
-    """Define how apply cutmix to a tensor
+    """Define how apply cutmix to a tensor.
 
     :param batch: Tensor on which apply the cutmix augmentation
-    :param lam: probability values have 0 in a binary random mask,
-        so it means probability original values will
-    be updated
+    :param lam: probability values have 0 in a binary random mask, so it means probability original values will     be
+        updated
     """
     result = {}
     for key, value in batch.items():
         random_index = _get_random_index(value)
         x_binary_mask = torch.from_numpy(np.random.choice(2, size=value.shape, p=[lam, 1 - lam]))
         x_random = value[random_index, :]
         x_noised = value.clone().detach()
         x_noised[x_binary_mask == 0] = x_random[x_binary_mask == 0]
         result[key] = x_noised
     return result
 
 
 def _get_random_index(x: torch.Tensor) -> torch.Tensor:
-    """Given a tensor it compute random indices between 0 and the number of the first dimension
+    """Given a tensor it compute random indices between 0 and the number of the first dimension.
 
     :param x: Tensor used to get the number of rows
     """
     batch_size = x.size()[0]
     index = torch.randperm(batch_size)
     return index
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/common/heads.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/common/heads.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""SSL Heads"""
+"""SSL Heads."""
 import torch.nn as nn
 
 
 class MultiTaskHead(nn.Module):
-    """
-    Simple Linear transformation to take last hidden representation to reconstruct inputs.
+    """Simple Linear transformation to take last hidden representation to reconstruct inputs.
+
     Output is dictionary of variable type to tensor mapping.
     """
 
     def __init__(self, in_features, n_binary=0, n_categorical=0, n_numerical=0, cardinality=[]):
         super().__init__()
         assert n_categorical == len(cardinality), "require cardinalities for each categorical variable"
         assert n_binary + n_categorical + n_numerical, "need some targets"
@@ -20,15 +20,15 @@
         self.n_numerical = n_numerical
 
         self.binary_linear = nn.Linear(in_features, n_binary) if n_binary else None
         self.categorical_linears = nn.ModuleList([nn.Linear(in_features, card) for card in cardinality])
         self.numerical_linear = nn.Linear(in_features, n_numerical) if n_numerical else None
 
     def forward(self, features):
-        outputs = dict()
+        outputs = {}
 
         if self.binary_linear:
             outputs["binary"] = self.binary_linear(features)
 
         if self.categorical_linears:
             outputs["categorical"] = [linear(features) for linear in self.categorical_linears]
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/common/layers.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/common/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-# noqa W605
+# W605
 from collections import OrderedDict
 from typing import Any, Dict, Tuple
 
 import torch
 from torch import nn
 
 from pytorch_tabular.ssl_models.common.utils import OneHot
 
 
 class MixedEmbedding1dLayer(nn.Module):
-    """
-    Enables different values in a categorical features to have different embeddings
-    """
+    """Enables different values in a categorical features to have different embeddings."""
 
     def __init__(
         self,
         continuous_dim: int,
         categorical_embedding_dims: Tuple[int, int],
         max_onehot_cardinality: int = 4,
         embedding_dropout: float = 0.0,
         batch_norm_continuous_input: bool = False,
     ):
-        super(MixedEmbedding1dLayer, self).__init__()
+        super().__init__()
         self.continuous_dim = continuous_dim
         self.categorical_embedding_dims = categorical_embedding_dims
         self.categorical_dim = len(categorical_embedding_dims)
         self.batch_norm_continuous_input = batch_norm_continuous_input
 
         binary_feat_idx = []
         onehot_feat_idx = []
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/common/noise_generators.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/common/noise_generators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
 # Inspired by implementation https://github.com/ryancheunggit/tabular_dae
-"""DenoisingAutoEncoder Model"""
+"""DenoisingAutoEncoder Model."""
 import numpy as np
 import torch
 import torch.nn as nn
 
 
 class SwapNoiseCorrupter(nn.Module):
-    """
-    Apply swap noise on the input data.
+    """Apply swap noise on the input data.
+
     Each data point has specified chance be replaced by a random value from the same column.
     """
 
     def __init__(self, probas):
         super().__init__()
         self.probas = torch.from_numpy(np.array(probas))
 
     def forward(self, x):
-        should_swap = torch.bernoulli(self.probas.to(x.device) * torch.ones((x.shape)).to(x.device))
+        should_swap = torch.bernoulli(self.probas.to(x.device) * torch.ones(x.shape).to(x.device))
         corrupted_x = torch.where(should_swap == 1, x[torch.randperm(x.shape[0])], x)
         mask = (corrupted_x != x).float()
         return corrupted_x, mask
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/common/ssl_utils.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/common/ssl_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/dae/config.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/dae/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""DenoisingAutoEncoder Config"""
+"""DenoisingAutoEncoder Config."""
 from dataclasses import dataclass, field
 from typing import Dict, List, Optional
 
 from pytorch_tabular.config import SSLModelConfig
 
 
 @dataclass
 class DenoisingAutoEncoderConfig(SSLModelConfig):
-    """DeNoising AutoEncoder configuration
+    """DeNoising AutoEncoder configuration.
+
     Args:
         noise_strategy (str): Defines what kind of noise we are introducing to samples. `swap` - Swap noise
                 is when we replace values of a feature with random permutations of the same feature. `zero` - Zero
                 noise is when we replace values of a feature with zeros. Defaults to swap. Choices are:
                 [`swap`,`zero`].
 
         noise_probabilities (Dict[str, float]): Dict of individual probabilities to corrupt the input
@@ -57,45 +58,56 @@
 
         seed (int): The seed for reproducibility. Defaults to 42
     """
 
     noise_strategy: str = field(
         default="swap",
         metadata={
-            "help": "Defines what kind of noise we are introducing to samples. `swap` - Swap noise is when we replace values of a feature with random permutations of the same feature. `zero` - Zero noise is when we replace values of a feature with zeros. Defaults to swap",
+            "help": "Defines what kind of noise we are introducing to samples."
+            " `swap` - Swap noise is when we replace values of a feature with random permutations"
+            " of the same feature. `zero` - Zero noise is when we replace values of a feature with zeros."
+            " Defaults to swap",
             "choices": ["swap", "zero"],
         },
     )
     # Union not supported by omegaconf. Currently Union[float, Dict[str, float]]
     noise_probabilities: Dict[str, float] = field(
-        default_factory=lambda: dict(),
+        default_factory=lambda: {},
         metadata={
-            "help": "Dict of individual probabilities to corrupt the input features with swap/zero noise. Key should be the feature name and if any feature is missing, the default_noise_probability is used. Default is an empty dict()"
+            "help": "Dict of individual probabilities to corrupt the input features with swap/zero noise."
+            " Key should be the feature name and if any feature is missing,"
+            " the default_noise_probability is used. Default is an empty dict()"
         },
     )
     default_noise_probability: float = field(
         default=0.8,
         metadata={
-            "help": "Default probability to corrupt the input features with swap/zero noise. For features for which noise_probabilities does not define a probability. Default is 0.8"
+            "help": "Default probability to corrupt the input features with swap/zero noise."
+            " For features for which noise_probabilities does not define a probability. Default is 0.8"
         },
     )
     loss_type_weights: Optional[List[float]] = field(
         default=None,
         metadata={
-            "help": "Weights to be used for the loss function in the order [binary, categorical, numerical]. If None, will use the default weights using a formula. eg. for binary, default weight will be n_binary/n_features. Defaults to None"
+            "help": "Weights to be used for the loss function in the order [binary, categorical, numerical]."
+            " If None, will use the default weights using a formula. eg. for binary,"
+            " default weight will be n_binary/n_features. Defaults to None"
         },
     )
     mask_loss_weight: float = field(
         default=2.0,
         metadata={"help": "Weight to be used for the loss function for the masked features. Defaults to 1.0"},
     )
     max_onehot_cardinality: int = field(
         default=4,
         metadata={
-            "help": "Maximum cardinality of one-hot encoded categorical features. Any categorical feature with cardinality>max_onehot_cardinality will be embedded in a learned embedding space and others will be converted to a one hot representation. If set to 0, will use the embedding strategy for all categorical feature. Default is 4"
+            "help": "Maximum cardinality of one-hot encoded categorical features."
+            " Any categorical feature with cardinality>max_onehot_cardinality will be embedded"
+            " in a learned embedding space and others will be converted to a one hot representation."
+            " If set to 0, will use the embedding strategy for all categorical feature. Default is 4"
         },
     )
 
     _module_src: str = field(default="ssl_models.dae")
     _model_name: str = field(default="DenoisingAutoEncoderModel")
     _config_name: str = field(default="DenoisingAutoEncoderConfig")
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/ssl_models/dae/dae.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/ssl_models/dae/dae.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
 # Inspired by implementation https://github.com/ryancheunggit/tabular_dae
-"""DenoisingAutoEncoder Model"""
+"""DenoisingAutoEncoder Model."""
 from collections import namedtuple
 from typing import Dict
 
 import torch
 import torch.nn as nn
 from omegaconf import DictConfig
 
@@ -154,15 +154,15 @@
             z, mask = features.features, features.mask
             # decoder
             z_hat = self.decoder(z)
             # reconstruction
             reconstructed_in = self.reconstruction(z_hat)
             # mask reconstruction
             reconstructed_mask = self.mask_reconstruction(z_hat)
-            output_dict = dict(mask=self.output_tuple(mask, reconstructed_mask))
+            output_dict = {"mask": self.output_tuple(mask, reconstructed_mask)}
             if "continuous" in reconstructed_in.keys():
                 output_dict["continuous"] = self.output_tuple(
                     torch.cat(
                         [
                             i
                             for i in [
                                 x.get("continuous", None),
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/tabular_datamodule.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/tabular_datamodule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""Tabular Data Module"""
+"""Tabular Data Module."""
 import re
 from pathlib import Path
 from typing import Iterable, List, Optional, Tuple, Union
 
 import category_encoders as ce
 import joblib
 import numpy as np
@@ -30,61 +30,61 @@
 
 from .categorical_encoders import OrdinalEncoder
 
 logger = get_logger(__name__)
 
 
 class TabularDatamodule(pl.LightningDataModule):
-
     CONTINUOUS_TRANSFORMS = {
         "quantile_uniform": {
             "callable": QuantileTransformer,
-            "params": dict(output_distribution="uniform", random_state=None),
+            "params": {"output_distribution": "uniform", "random_state": None},
         },
         "quantile_normal": {
             "callable": QuantileTransformer,
-            "params": dict(output_distribution="normal", random_state=None),
+            "params": {"output_distribution": "normal", "random_state": None},
         },
         "box-cox": {
             "callable": PowerTransformer,
-            "params": dict(method="box-cox", standardize=False),
+            "params": {"method": "box-cox", "standardize": False},
         },
         "yeo-johnson": {
             "callable": PowerTransformer,
-            "params": dict(method="yeo-johnson", standardize=False),
+            "params": {"method": "yeo-johnson", "standardize": False},
         },
     }
 
     def __init__(
         self,
         train: pd.DataFrame,
         config: DictConfig,
         validation: pd.DataFrame = None,
         test: pd.DataFrame = None,
         target_transform: Optional[Union[TransformerMixin, Tuple]] = None,
         train_sampler: Optional[torch.utils.data.Sampler] = None,
         seed: Optional[int] = 42,
     ):
-        """The Pytorch Lightning Datamodule for Tabular Data
+        """The Pytorch Lightning Datamodule for Tabular Data.
 
         Args:
             train (pd.DataFrame): The Training Dataframe
 
             config (DictConfig): Merged configuration object from ModelConfig, DataConfig,
                 TrainerConfig, OptimizerConfig & ExperimentConfig
 
             validation (pd.DataFrame, optional): Validation Dataframe.
                 If left empty, we use the validation split from DataConfig to split a random sample as validation.
                 Defaults to None.
 
             test (pd.DataFrame, optional): Holdout DataFrame to check final performance on.
                 Defaults to None.
 
-            target_transform (Optional[Union[TransformerMixin, Tuple(Callable)]], optional): If provided, applies the transform to the target before modelling
-                and inverse the transform during prediction. The parameter can either be a sklearn Transformer which has an inverse_transform method, or
+            target_transform (Optional[Union[TransformerMixin, Tuple(Callable)]], optional):
+                If provided, applies the transform to the target before modelling and inverse the transform during
+                prediction. The parameter can either be a sklearn Transformer which has an inverse_transform method, or
                 a tuple of callables (transform_func, inverse_transform_func)
         """
         super().__init__()
         self.train = train.copy()
         self.validation = validation
         self._set_target_transform(target_transform)
         self.test = test if test is None else test.copy()
@@ -101,15 +101,15 @@
                 target_transform = FunctionTransformer(func=target_transform[0], inverse_func=target_transform[1])
             self.do_target_transform = True
         else:
             self.do_target_transform = False
         self.target_transform_template = target_transform
 
     def update_config(self, config) -> InferredConfig:
-        """Calculates and updates a few key information to the config object
+        """Calculates and updates a few key information to the config object.
 
         Args:
             config (DictConfig): The config object
 
         Returns:
             InferredConfig: The updated config object
         """
@@ -165,15 +165,16 @@
                 logger.debug("Encoding Categorical Columns using LeavOneOutEncoder")
                 self.categorical_encoder = ce.LeaveOneOutEncoder(
                     cols=self.config.categorical_cols, random_state=self.seed
                 )
                 # Multi-Target Regression uses the first target to encode the categorical columns
                 if len(self.config.target) > 1:
                     logger.warning(
-                        f"Multi-Target Regression: using the first target({self.config.target[0]}) to encode the categorical columns"
+                        f"Multi-Target Regression: using the first target({self.config.target[0]})"
+                        f" to encode the categorical columns"
                     )
                 data = self.categorical_encoder.fit_transform(data, data[self.config.target[0]])
             else:
                 logger.debug("Encoding Categorical Columns using OrdinalEncoder")
                 self.categorical_encoder = OrdinalEncoder(
                     cols=self.config.categorical_cols,
                     handle_unseen="impute" if self.config.handle_unknown_categories else "error",
@@ -219,34 +220,36 @@
                 if self.config.target[0] in data.columns:
                     data[self.config.target[0]] = self.label_encoder.transform(data[self.config.target[0]])
         return data
 
     def _target_transform(self, data: pd.DataFrame, stage: str) -> pd.DataFrame:
         if self.config.task == "regression":
             # target transform only for regression
-            if all([col in data.columns for col in self.config.target]):
+            if all(col in data.columns for col in self.config.target):
                 if self.do_target_transform:
                     if stage == "fit":
                         target_transforms = []
                         for col in self.config.target:
                             _target_transform = copy.deepcopy(self.target_transform_template)
                             data[col] = _target_transform.fit_transform(data[col].values.reshape(-1, 1))
                             target_transforms.append(_target_transform)
                         self.target_transforms = target_transforms
                     else:
                         for col, _target_transform in zip(self.config.target, self.target_transforms):
                             data[col] = _target_transform.transform(data[col].values.reshape(-1, 1))
         return data
 
     def preprocess_data(self, data: pd.DataFrame, stage: str = "inference") -> Tuple[pd.DataFrame, list]:
-        """The preprocessing, like Categorical Encoding, Normalization, etc. which any dataframe should undergo before feeding into the dataloder
+        """The preprocessing, like Categorical Encoding, Normalization, etc. which any dataframe should undergo before
+        feeding into the dataloder.
 
         Args:
             data (pd.DataFrame): A dataframe with the features and target
-            stage (str, optional): Internal parameter. Used to distinguisj between fit and inference. Defaults to "inference".
+            stage (str, optional): Internal parameter. Used to distinguisj between fit and inference.
+                Defaults to "inference".
 
         Returns:
             Returns the processed dataframe and the added features(list) as a tuple
         """
         added_features = None
         if self.config.encode_date_columns:
             data, added_features = self._encode_date_columns(data)
@@ -272,25 +275,27 @@
         # Converting target labels to a 0 indexed label
         data = self._label_encode_target(data, stage)
         # Target Transforms
         data = self._target_transform(data, stage)
         return data, added_features
 
     def setup(self, stage: Optional[str] = None) -> None:
-        """Data Operations you want to perform on all GPUs, like train-test split, transformations, etc.
-        This is called before accessing the dataloaders
+        """Data Operations you want to perform on all GPUs, like train-test split, transformations, etc. This is called
+        before accessing the dataloaders.
 
         Args:
-            stage (Optional[str], optional): Internal parameter to distinguish between fit and inference. Defaults to None.
+            stage (Optional[str], optional):
+                Internal parameter to distinguish between fit and inference. Defaults to None.
         """
         if stage == "fit" or stage is None:
             logger.info(f"Setting up the datamodule for {self.config.task} task")
             if self.validation is None:
                 logger.debug(
-                    f"No validation data provided. Using {self.config.validation_split*100}% of train data as validation"
+                    f"No validation data provided."
+                    f" Using {self.config.validation_split*100}% of train data as validation"
                 )
                 val_idx = self.train.sample(
                     int(self.config.validation_split * len(self.train)),
                     random_state=self.seed,
                 ).index
                 self.validation = self.train[self.train.index.isin(val_idx)]
                 self.train = self.train[~self.train.index.isin(val_idx)]
@@ -302,16 +307,15 @@
             if self.test is not None:
                 self.test, _ = self.preprocess_data(self.test, stage="inference")
             self._fitted = True
 
     # adapted from gluonts
     @classmethod
     def time_features_from_frequency_str(cls, freq_str: str) -> List[str]:
-        """
-        Returns a list of time features that will be appropriate for the given frequency string.
+        """Returns a list of time features that will be appropriate for the given frequency string.
 
         Args:
             freq_str (str): Frequency string of the form `[multiple][granularity]` such as "12H", "5min", "1D" etc.
 
         Returns:
             List of added features
         """
@@ -599,15 +603,15 @@
         df = self._prepare_inference_data(df)
         dataset = TabularDataset(
             task=self.config.task,
             data=df,
             categorical_cols=self.config.categorical_cols,
             continuous_cols=self.config.continuous_cols,
             embed_categorical=(not self.do_leave_one_out_encoder()),
-            target=self.target if all([col in df.columns for col in self.target]) else None,
+            target=self.target if all(col in df.columns for col in self.target) else None,
         )
         return DataLoader(
             dataset,
             batch_size if batch_size is not None else self.batch_size,
             shuffle=False,
             num_workers=self.config.num_workers,
         )
@@ -646,24 +650,27 @@
         data: pd.DataFrame,
         task: str,
         continuous_cols: List[str] = None,
         categorical_cols: List[str] = None,
         embed_categorical: bool = True,
         target: List[str] = None,
     ):
-        """Dataset to Load Tabular Data
+        """Dataset to Load Tabular Data.
 
         Args:
             data (pd.DataFrame): Pandas DataFrame to load during training
-            task (str): Whether it is a classification or regression task. If classification, it returns a LongTensor as target
+            task (str):
+                Whether it is a classification or regression task. If classification, it returns a LongTensor as target
             continuous_cols (List[str], optional): A list of names of continuous columns. Defaults to None.
             categorical_cols (List[str], optional): A list of names of categorical columns.
-            These columns must be ordinal encoded beforehand. Defaults to None.
-            embed_categorical (bool): Flag to tell the dataset whether to convert categorical columns to LongTensor or retain as float.
-            If we are going to embed categorical cols with an embedding layer, we need to convert the columns to LongTensor
+                These columns must be ordinal encoded beforehand. Defaults to None.
+            embed_categorical (bool):
+                Flag to tell the dataset whether to convert categorical columns to LongTensor or retain as float.
+                If we are going to embed categorical cols with an embedding layer,
+                we need to convert the columns to LongTensor
             target (List[str], optional): A list of strings with target column name(s). Defaults to None.
         """
 
         self.task = task
         self.n = data.shape[0]
 
         if target:
@@ -685,21 +692,17 @@
             self.categorical_X = data[categorical_cols]
             if embed_categorical:
                 self.categorical_X = self.categorical_X.astype(np.int64).values
             else:
                 self.categorical_X = self.categorical_X.astype(np.float32).values
 
     def __len__(self):
-        """
-        Denotes the total number of samples.
-        """
+        """Denotes the total number of samples."""
         return self.n
 
     def __getitem__(self, idx):
-        """
-        Generates one sample of data.
-        """
+        """Generates one sample of data."""
         return {
             "target": self.y[idx],
             "continuous": self.continuous_X[idx] if self.continuous_cols else torch.Tensor(),
             "categorical": self.categorical_X[idx] if self.categorical_cols else torch.Tensor(),
         }
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/tabular_model.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/tabular_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Pytorch Tabular
 # Author: Manu Joseph <manujoseph@gmail.com>
 # For license information, see LICENSE.TXT
-"""Tabular Model"""
+"""Tabular Model."""
 import copy
 import inspect
 import os
 import warnings
 from collections import defaultdict
 from functools import partial
 from pathlib import Path
@@ -13,17 +13,17 @@
 
 import joblib
 import numpy as np
 import pandas as pd
 import pytorch_lightning as pl
 import torch
 import torchmetrics
-from lightning_lite.utilities.seed import seed_everything
 from omegaconf import OmegaConf
 from omegaconf.dictconfig import DictConfig
+from pytorch_lightning import seed_everything
 from pytorch_lightning.callbacks import RichProgressBar
 from pytorch_lightning.callbacks.gradient_accumulation_scheduler import GradientAccumulationScheduler
 from pytorch_lightning.utilities.model_summary import summarize
 from rich.progress import track
 from sklearn.base import TransformerMixin
 from sklearn.preprocessing import LabelEncoder
 from torch import nn
@@ -58,42 +58,45 @@
     ) -> None:
         """The core model which orchestrates everything from initializing the datamodule, the model, trainer, etc.
 
         Args:
             config (Optional[Union[DictConfig, str]], optional): Single OmegaConf DictConfig object or
                 the path to the yaml file holding all the config parameters. Defaults to None.
 
-            data_config (Optional[Union[DataConfig, str]], optional): DataConfig object or path to the yaml file. Defaults to None.
+            data_config (Optional[Union[DataConfig, str]], optional):
+                DataConfig object or path to the yaml file. Defaults to None.
 
-            model_config (Optional[Union[ModelConfig, str]], optional): A subclass of ModelConfig or path to the yaml file.
+            model_config (Optional[Union[ModelConfig, str]], optional):
+                A subclass of ModelConfig or path to the yaml file.
                 Determines which model to run from the type of config. Defaults to None.
 
-            optimizer_config (Optional[Union[OptimizerConfig, str]], optional): OptimizerConfig object or path to the yaml file.
-                Defaults to None.
+            optimizer_config (Optional[Union[OptimizerConfig, str]], optional):
+                OptimizerConfig object or path to the yaml file. Defaults to None.
 
-            trainer_config (Optional[Union[TrainerConfig, str]], optional): TrainerConfig object or path to the yaml file.
-                Defaults to None.
+            trainer_config (Optional[Union[TrainerConfig, str]], optional):
+                TrainerConfig object or path to the yaml file. Defaults to None.
 
-            experiment_config (Optional[Union[ExperimentConfig, str]], optional): ExperimentConfig object or path to the yaml file.
+            experiment_config (Optional[Union[ExperimentConfig, str]], optional):
+                ExperimentConfig object or path to the yaml file.
                 If Provided configures the experiment tracking. Defaults to None.
 
-            model_callable (Optional[Callable], optional): If provided, will override the model callable that will be loaded from the config.
+            model_callable (Optional[Callable], optional):
+                If provided, will override the model callable that will be loaded from the config.
                 Typically used when providing Custom Models
 
-            model_state_dict_path (Optional[Union[str, Path]], optional): If provided, will load the state dict after initializing the model from config.
+            model_state_dict_path (Optional[Union[str, Path]], optional):
+                If provided, will load the state dict after initializing the model from config.
         """
         super().__init__()
         self.exp_manager = ExperimentRunManager()
         if config is None:
-            assert (
-                (data_config is not None)
-                or (model_config is not None)
-                or (optimizer_config is not None)
-                or (trainer_config is not None)
-            ), "If `config` is None, `data_config`, `model_config`, `trainer_config`, and `optimizer_config` cannot be None"
+            assert any(c is not None for c in (data_config, model_config, optimizer_config, trainer_config)), (
+                "If `config` is None, `data_config`, `model_config`, `trainer_config`,"
+                " and `optimizer_config` cannot be None"
+            )
             data_config = self._read_parse_config(data_config, DataConfig)
             model_config = self._read_parse_config(model_config, ModelConfig)
             trainer_config = self._read_parse_config(trainer_config, TrainerConfig)
             optimizer_config = self._read_parse_config(optimizer_config, OptimizerConfig)
             if model_config.task != "ssl":
                 assert (
                     data_config.target is not None
@@ -140,27 +143,28 @@
             self.model_callable = model_callable
             self.custom_model = True
         self.model_state_dict_path = model_state_dict_path
         self._is_config_updated_with_data = False
         self._run_validation()
 
     def _run_validation(self):
-        """Validates the Config params and throws errors if something is wrong"""
+        """Validates the Config params and throws errors if something is wrong."""
         if self.config.task == "classification":
             if len(self.config.target) > 1:
                 raise NotImplementedError("Multi-Target Classification is not implemented.")
         if self.config.task == "regression":
             if self.config.target_range is not None:
                 if (
                     (len(self.config.target_range) != len(self.config.target))
-                    or any([len(range_) != 2 for range_ in self.config.target_range])
-                    or any([range_[0] > range_[1] for range_ in self.config.target_range])
+                    or any(len(range_) != 2 for range_ in self.config.target_range)
+                    or any(range_[0] > range_[1] for range_ in self.config.target_range)
                 ):
                     raise ValueError(
-                        "Targe Range, if defined, should be list tuples of length two(min,max). The length of the list should be equal to hte length of target columns"
+                        "Targe Range, if defined, should be list tuples of length two(min,max)."
+                        " The length of the list should be equal to hte length of target columns"
                     )
         if self.config.task == "ssl":
             assert (
                 not self.config.handle_unknown_categories
             ), "SSL only supports handle_unknown_categories=False. Please set this in your DataConfig"
             assert (
                 not self.config.handle_missing_values
@@ -181,45 +185,45 @@
                 )
             else:
                 raise ValueError(f"{config} is not a valid path")
         config = OmegaConf.structured(config)
         return config
 
     def _get_run_name_uid(self) -> Tuple[str, int]:
-        """Gets the name of the experiment and increments version by 1
+        """Gets the name of the experiment and increments version by 1.
 
         Returns:
             tuple[str, int]: Returns the name and version number
         """
         if hasattr(self.config, "run_name") and self.config.run_name is not None:
             name = self.config.run_name
         elif hasattr(self.config, "checkpoints_name") and self.config.checkpoints_name is not None:
             name = self.config.checkpoints_name
         else:
             name = self.config.task
         uid = self.exp_manager.update_versions(name)
         return name, uid
 
     def _setup_experiment_tracking(self):
-        """Sets up the Experiment Tracking Framework according to the choices made in the Experimentconfig"""
+        """Sets up the Experiment Tracking Framework according to the choices made in the Experimentconfig."""
         if self.config.log_target == "tensorboard":
             self.logger = pl.loggers.TensorBoardLogger(
                 name=self.name, save_dir=self.config.project_name, version=self.uid
             )
         elif self.config.log_target == "wandb":
             self.logger = pl.loggers.WandbLogger(
                 name=f"{self.name}_{self.uid}",
                 project=self.config.project_name,
                 offline=False,
             )
         else:
             raise NotImplementedError(f"{self.config.log_target} is not implemented. Try one of [wandb, tensorboard]")
 
     def _prepare_callbacks(self, callbacks=None) -> List:
-        """Prepares the necesary callbacks to the Trainer based on the configuration
+        """Prepares the necesary callbacks to the Trainer based on the configuration.
 
         Returns:
             List: A list of callbacks
         """
         callbacks = [] if callbacks is None else callbacks
         if self.config.early_stopping is not None:
             early_stop_callback = pl.callbacks.early_stopping.EarlyStopping(
@@ -242,15 +246,15 @@
                 every_n_epochs=self.config.checkpoints_every_n_epochs,
                 **self.config.checkpoints_kwargs,
             )
             callbacks.append(model_checkpoint)
             self.config.enable_checkpointing = True
         else:
             self.config.enable_checkpointing = False
-        if self.config.progress_bar == "rich":
+        if self.config.progress_bar == "rich" and self.config.trainer_kwargs.get("enable_progress_bar", True):
             callbacks.append(RichProgressBar())
         logger.debug(f"Callbacks used: {callbacks}")
         return callbacks
 
     def _prepare_trainer(self, callbacks: List, max_epochs: int = None, min_epochs: int = None) -> pl.Trainer:
         """Prepares the Trainer object
         Args:
@@ -301,31 +305,28 @@
         self.callbacks = self._prepare_callbacks(callbacks)
         self.trainer = self._prepare_trainer(self.callbacks, max_epochs, min_epochs)
         self.model = model
         self.datamodule = datamodule
 
     @classmethod
     def _load_weights(cls, model, path: Union[str, Path]) -> None:
-        """Loads the model weights in the specified directory
+        """Loads the model weights in the specified directory.
 
         Args:
             path (str): The path to the file to load the model from
 
         Returns:
             None
         """
         ckpt = pl_load(path, map_location=lambda storage, loc: storage)
-        if "state_dict" in ckpt.keys():
-            model.load_state_dict(ckpt["state_dict"])
-        else:
-            model.load_state_dict(ckpt)
+        model.load_state_dict(ckpt.get("state_dict") or ckpt)
 
     @classmethod
     def load_model(cls, dir: str, map_location=None, strict=True):
-        """Loads a saved model from the directory
+        """Loads a saved model from the directory.
 
         Args:
             dir (str): The directory where the model wa saved, along with the checkpoints
             map_location (Union[Dict[str, str], str, device, int, Callable, None]) : If your checkpoint
                 saved a GPU model and you now load on CPUs or a different number of GPUs, use this to map
                 to the new setup. The behaviour is the same as in torch.load()
             strict (bool) : Whether to strictly enforce that the keys in checkpoint_path match the keys
@@ -368,14 +369,15 @@
         }
         custom_params = joblib.load(os.path.join(dir, "custom_params.sav"))
         if custom_params.get("custom_loss") is not None:
             model_args["loss"] = "MSELoss"  # For compatibility. Not Used
         if custom_params.get("custom_metrics") is not None:
             model_args["metrics"] = ["mean_squared_error"]  # For compatibility. Not Used
             model_args["metrics_params"] = [{}]  # For compatibility. Not Used
+            model_args["metrics_prob_inputs"] = [False]  # For compatibility. Not Used
         if custom_params.get("custom_optimizer") is not None:
             model_args["optimizer"] = "Adam"  # For compatibility. Not Used
         if custom_params.get("custom_optimizer_params") is not None:
             model_args["optimizer_params"] = {}  # For compatibility. Not Used
 
         # Initializing with default metrics, losses, and optimizers. Will revert once initialized
         model = model_callable.load_from_checkpoint(
@@ -403,15 +405,15 @@
         tabular_model.trainer = tabular_model._prepare_trainer(callbacks=callbacks)
         tabular_model.trainer.model = model
         tabular_model.logger = logger
         return tabular_model
 
     @classmethod
     def load_from_checkpoint(cls, dir: str, map_location=None, strict=True):
-        """(Deprecated: Use `load_model` instead) Loads a saved model from the directory
+        """(Deprecated: Use `load_model` instead) Loads a saved model from the directory.
 
         Args:
             dir (str): The directory where the model was saved, along with the checkpoints
             map_location (Union[Dict[str, str], str, device, int, Callable, None]) : If your checkpoint
                 saved a GPU model and you now load on CPUs or a different number of GPUs, use this to map
                 to the new setup. The behaviour is the same as in torch.load()
             strict (bool) : Whether to strictly enforce that the keys in checkpoint_path match the keys
@@ -437,34 +439,40 @@
         seed: Optional[int] = 42,
     ) -> TabularDatamodule:
         """Prepares the dataloaders for training and validation.
 
         Args:
             train (pd.DataFrame): Training Dataframe
 
-            validation (Optional[pd.DataFrame], optional): If provided, will use this dataframe as the validation while training.
-                Used in Early Stopping and Logging. If left empty, will use 20% of Train data as validation. Defaults to None.
+            validation (Optional[pd.DataFrame], optional):
+                If provided, will use this dataframe as the validation while training.
+                Used in Early Stopping and Logging. If left empty, will use 20% of Train data as validation.
+                Defaults to None.
 
             test (Optional[pd.DataFrame], optional): If provided, will use as the hold-out data,
                 which you'll be able to check performance after the model is trained. Defaults to None.
 
-            train_sampler (Optional[torch.utils.data.Sampler], optional): Custom PyTorch batch samplers which will be passed to the DataLoaders. Useful for dealing with imbalanced data and other custom batching strategies
-
-            target_transform (Optional[Union[TransformerMixin, Tuple(Callable)]], optional): If provided, applies the transform to the target before modelling
-                and inverse the transform during prediction. The parameter can either be a sklearn Transformer which has an inverse_transform method, or
+            train_sampler (Optional[torch.utils.data.Sampler], optional):
+                Custom PyTorch batch samplers which will be passed to the DataLoaders.
+                Useful for dealing with imbalanced data and other custom batching strategies
+
+            target_transform (Optional[Union[TransformerMixin, Tuple(Callable)]], optional):
+                If provided, applies the transform to the target before modelling and inverse the transform during
+                prediction. The parameter can either be a sklearn Transformer which has an inverse_transform method, or
                 a tuple of callables (transform_func, inverse_transform_func)
 
             seed (Optional[int], optional): Random seed for reproducibility. Defaults to 42.
 
         Returns:
             TabularDatamodule: The prepared datamodule
         """
         if test is not None:
             warnings.warn(
-                "Providing test data in `fit` is deprecated and will be removed in next major release. Plese use `evaluate` for evaluating on test data"
+                "Providing test data in `fit` is deprecated and will be removed in next major release."
+                " Plese use `evaluate` for evaluating on test data"
             )
         logger.info("Preparing the DataLoaders")
         target_transform = self._check_and_set_target_transform(target_transform)
 
         datamodule = TabularDatamodule(
             train=train,
             validation=validation,
@@ -479,43 +487,49 @@
         return datamodule
 
     def prepare_model(
         self,
         datamodule: TabularDatamodule,
         loss: Optional[torch.nn.Module] = None,
         metrics: Optional[List[Callable]] = None,
+        metrics_prob_inputs: Optional[List[bool]] = None,
         optimizer: Optional[torch.optim.Optimizer] = None,
         optimizer_params: Dict = {},
     ) -> BaseModel:
         """Prepares the model for training.
 
         Args:
             datamodule (TabularDatamodule): The datamodule
 
             loss (Optional[torch.nn.Module], optional): Custom Loss functions which are not in standard pytorch library
 
             metrics (Optional[List[Callable]], optional): Custom metric functions(Callable) which has the
                 signature metric_fn(y_hat, y) and works on torch tensor inputs
 
-            optimizer (Optional[torch.optim.Optimizer], optional): Custom optimizers which are a drop in replacements for standard PyToch optimizers.
+            metrics_prob_inputs (Optional[List[bool]], optional): This is a mandatory parameter for
+                classification metrics. If the metric function requires probabilities as inputs, set this to True.
+                The length of the list should be equal to the number of metrics. Defaults to None.
+
+            optimizer (Optional[torch.optim.Optimizer], optional):
+                Custom optimizers which are a drop in replacements for standard PyToch optimizers.
                 This should be the Class and not the initialized object
 
             optimizer_params (Optional[Dict], optional): The parmeters to initialize the custom optimizer.
 
         Returns:
             BaseModel: The prepared model
-
         """
         logger.info(f"Preparing the Model: {self.config._model_name}")
         # Fetching the config as some data specific configs have been added in the datamodule
         self.inferred_config = self._read_parse_config(datamodule.update_config(self.config), InferredConfig)
         model = self.model_callable(
             self.config,
             custom_loss=loss,  # Unused in SSL tasks
             custom_metrics=metrics,  # Unused in SSL tasks
+            custom_metrics_prob_inputs=metrics_prob_inputs,  # Unused in SSL tasks
             custom_optimizer=optimizer,
             custom_optimizer_params=optimizer_params,
             inferred_config=self.inferred_config,
         )
         # Data Aware Initialization(for the models that need it)
         model.data_aware_initialization(datamodule)
         if self.model_state_dict_path is not None:
@@ -535,15 +549,16 @@
         """Trains the model.
 
         Args:
             model (pl.LightningModule): The PyTorch Lightning model to be trained.
 
             datamodule (TabularDatamodule): The datamodule
 
-            callbacks (Optional[List[pl.Callback]], optional): List of callbacks to be used during training. Defaults to None.
+            callbacks (Optional[List[pl.Callback]], optional):
+                List of callbacks to be used during training. Defaults to None.
 
             max_epochs (Optional[int]): Overwrite maximum number of epochs to be run. Defaults to None.
 
             min_epochs (Optional[int]): Overwrite minimum number of epochs to be run. Defaults to None.
 
         Returns:
             pl.Trainer: The PyTorch Lightning Trainer instance
@@ -554,15 +569,16 @@
             self.datamodule.val_dataloader(),
         )
         self.model.train()
         if self.config.auto_lr_find and (not self.config.fast_dev_run):
             logger.info("Auto LR Find Started")
             result = self.trainer.tune(self.model, train_loader, val_loader)
             logger.info(
-                f"Suggested LR: {result['lr_find'].suggestion()}. For plot and detailed analysis, use `find_learning_rate` method."
+                f"Suggested LR: {result['lr_find'].suggestion()}."
+                f" For plot and detailed analysis, use `find_learning_rate` method."
             )
             # Parameters in models needs to be initialized again after LR find
             self.model.data_aware_initialization(self.datamodule)
         self.model.train()
         logger.info("Training Started")
         self.trainer.fit(self.model, train_loader, val_loader)
         logger.info("Training the model completed")
@@ -573,87 +589,108 @@
     def fit(
         self,
         train: Optional[pd.DataFrame],
         validation: Optional[pd.DataFrame] = None,
         test: Optional[pd.DataFrame] = None,  # TODO: Deprecate test in next version
         loss: Optional[torch.nn.Module] = None,
         metrics: Optional[List[Callable]] = None,
+        metrics_prob_inputs: Optional[List[bool]] = None,
         optimizer: Optional[torch.optim.Optimizer] = None,
         optimizer_params: Dict = {},
         train_sampler: Optional[torch.utils.data.Sampler] = None,
         target_transform: Optional[Union[TransformerMixin, Tuple]] = None,
         max_epochs: Optional[int] = None,
         min_epochs: Optional[int] = None,
         seed: Optional[int] = 42,
         callbacks: Optional[List[pl.Callback]] = None,
         datamodule: Optional[TabularDatamodule] = None,
     ) -> pl.Trainer:
-        """The fit method which takes in the data and triggers the training
+        """The fit method which takes in the data and triggers the training.
 
         Args:
             train (pd.DataFrame): Training Dataframe
 
-            validation (Optional[pd.DataFrame], optional): If provided, will use this dataframe as the validation while training.
-                Used in Early Stopping and Logging. If left empty, will use 20% of Train data as validation. Defaults to None.
+            validation (Optional[pd.DataFrame], optional):
+                If provided, will use this dataframe as the validation while training.
+                Used in Early Stopping and Logging. If left empty, will use 20% of Train data as validation.
+                Defaults to None.
 
             test (Optional[pd.DataFrame], optional): If provided, will use as the hold-out data,
                 which you'll be able to check performance after the model is trained. Defaults to None.
                 DEPRECATED. Will be removed in the next version.
 
             loss (Optional[torch.nn.Module], optional): Custom Loss functions which are not in standard pytorch library
 
             metrics (Optional[List[Callable]], optional): Custom metric functions(Callable) which has the
-                signature metric_fn(y_hat, y) and works on torch tensor inputs
+                signature metric_fn(y_hat, y) and works on torch tensor inputs. y_hat is expected to be of shape
+                (batch_size, num_classes) for classification and (batch_size, 1) for regression and y is expected to be
+                of shape (batch_size, 1)
+
+            metrics_prob_inputs (Optional[List[bool]], optional): This is a mandatory parameter for
+                classification metrics. If the metric function requires probabilities as inputs, set this to True.
+                The length of the list should be equal to the number of metrics. Defaults to None.
 
-            optimizer (Optional[torch.optim.Optimizer], optional): Custom optimizers which are a drop in replacements for
+            optimizer (Optional[torch.optim.Optimizer], optional):
+                Custom optimizers which are a drop in replacements for
                 standard PyToch optimizers. This should be the Class and not the initialized object
 
             optimizer_params (Optional[Dict], optional): The parmeters to initialize the custom optimizer.
 
-            train_sampler (Optional[torch.utils.data.Sampler], optional): Custom PyTorch batch samplers which will be passed
+            train_sampler (Optional[torch.utils.data.Sampler], optional):
+                Custom PyTorch batch samplers which will be passed
                 to the DataLoaders. Useful for dealing with imbalanced data and other custom batching strategies
 
-            target_transform (Optional[Union[TransformerMixin, Tuple(Callable)]], optional): If provided, applies the transform to the
-                target before modelling and inverse the transform during prediction. The parameter can either be a sklearn Transformer
+            target_transform (Optional[Union[TransformerMixin, Tuple(Callable)]], optional):
+                If provided, applies the transform to the target before modelling and inverse the transform during
+                prediction. The parameter can either be a sklearn Transformer
                 which has an inverse_transform method, or a tuple of callables (transform_func, inverse_transform_func)
 
             max_epochs (Optional[int]): Overwrite maximum number of epochs to be run. Defaults to None.
 
             min_epochs (Optional[int]): Overwrite minimum number of epochs to be run. Defaults to None.
 
             seed: (int): Random seed for reproducibility. Defaults to 42.
 
-            callbacks (Optional[List[pl.Callback]], optional): List of callbacks to be used during training. Defaults to None.
+            callbacks (Optional[List[pl.Callback]], optional):
+                List of callbacks to be used during training. Defaults to None.
 
-            datamodule (Optional[TabularDatamodule], optional): The datamodule. If provided, will ignore the rest of the parameters
-                like train, test etc and use the datamodule. Defaults to None.
+            datamodule (Optional[TabularDatamodule], optional): The datamodule.
+                If provided, will ignore the rest of the parameters like train, test etc and use the datamodule.
+                Defaults to None.
 
         Returns:
             pl.Trainer: The PyTorch Lightning Trainer instance
         """
         assert (
             self.config.task != "ssl"
         ), "`fit` is not valid for SSL task. Please use `pretrain` for semi-supervised learning"
+        if metrics is not None:
+            assert len(metrics) == len(
+                metrics_prob_inputs
+            ), "The length of `metrics` and `metrics_prob_inputs` should be equal"
         seed = seed if seed is not None else self.config.seed
         seed_everything(seed)
         if datamodule is None:
             datamodule = self.prepare_dataloader(train, validation, test, train_sampler, target_transform, seed)
         else:
             if train is not None:
                 warnings.warn(
-                    "train data is provided but datamodule is provided. Ignoring the train data and using the datamodule"
+                    "train data is provided but datamodule is provided."
+                    " Ignoring the train data and using the datamodule"
                 )
             if test is not None:
                 warnings.warn(
-                    "Providing test data in `fit` is deprecated and will be removed in next major release. Plese use `evaluate` for evaluating on test data"
+                    "Providing test data in `fit` is deprecated and will be removed in next major release."
+                    " Plese use `evaluate` for evaluating on test data"
                 )
         model = self.prepare_model(
             datamodule,
             loss,
             metrics,
+            metrics_prob_inputs,
             optimizer,
             optimizer_params,
         )
 
         return self.train(model, datamodule, callbacks, max_epochs, min_epochs)
 
     def pretrain(
@@ -665,34 +702,36 @@
         # train_sampler: Optional[torch.utils.data.Sampler] = None,
         max_epochs: Optional[int] = None,
         min_epochs: Optional[int] = None,
         seed: Optional[int] = 42,
         callbacks: Optional[List[pl.Callback]] = None,
         datamodule: Optional[TabularDatamodule] = None,
     ) -> pl.Trainer:
-        """The pretrained method which takes in the data and triggers the training
+        """The pretrained method which takes in the data and triggers the training.
 
         Args:
             train (pd.DataFrame): Training Dataframe
 
-            validation (Optional[pd.DataFrame], optional): If provided, will use this dataframe as the validation while training.
-                Used in Early Stopping and Logging. If left empty, will use 20% of Train data as validation. Defaults to None.
+            validation (Optional[pd.DataFrame], optional): If provided, will use this dataframe as the validation while
+                training. Used in Early Stopping and Logging. If left empty, will use 20% of Train data as validation.
+                Defaults to None.
 
-            optimizer (Optional[torch.optim.Optimizer], optional): Custom optimizers which are a drop in replacements for
-                standard PyToch optimizers. This should be the Class and not the initialized object
+            optimizer (Optional[torch.optim.Optimizer], optional): Custom optimizers which are a drop in replacements
+                for standard PyToch optimizers. This should be the Class and not the initialized object
 
             optimizer_params (Optional[Dict], optional): The parmeters to initialize the custom optimizer.
 
             max_epochs (Optional[int]): Overwrite maximum number of epochs to be run. Defaults to None.
 
             min_epochs (Optional[int]): Overwrite minimum number of epochs to be run. Defaults to None.
 
             seed: (int): Random seed for reproducibility. Defaults to 42.
 
-            callbacks (Optional[List[pl.Callback]], optional): List of callbacks to be used during training. Defaults to None.
+            callbacks (Optional[List[pl.Callback]], optional): List of callbacks to be used during training.
+                Defaults to None.
 
             datamodule (Optional[TabularDatamodule], optional): The datamodule. If provided, will ignore the rest of the
                 parameters like train, test etc and use the datamodule. Defaults to None.
 
         Returns:
             pl.Trainer: The PyTorch Lightning Trainer instance
         """
@@ -709,15 +748,16 @@
                 train_sampler=None,
                 target_transform=None,
                 seed=seed,
             )
         else:
             if train is not None:
                 warnings.warn(
-                    "train data is provided but datamodule is provided. Ignoring the train data and using the datamodule"
+                    "train data is provided but datamodule is provided."
+                    " Ignoring the train data and using the datamodule"
                 )
         model = self.prepare_model(
             datamodule,
             optimizer,
             optimizer_params,
         )
 
@@ -730,14 +770,15 @@
         head_config: Dict,
         target: Optional[str] = None,
         optimizer_config: Optional[OptimizerConfig] = None,
         trainer_config: Optional[TrainerConfig] = None,
         experiment_config: Optional[ExperimentConfig] = None,
         loss: Optional[torch.nn.Module] = None,
         metrics: Optional[List[Union[Callable, str]]] = None,
+        metrics_prob_input: Optional[List[bool]] = None,
         metrics_params: Optional[Dict] = None,
         optimizer: Optional[torch.optim.Optimizer] = None,
         optimizer_params: Dict = {},
         learning_rate: Optional[float] = None,
         target_range: Optional[Tuple[float, float]] = None,
     ):
         """Creates a new TabularModel model using the pretrained weights and the new task and head
@@ -750,35 +791,42 @@
 
             head_config (Dict): The config as a dict which defines the head. If left empty,
                 will be initialized as default linear head.
 
             target (Optional[str], optional): The target column name if not provided in the initial pretraining stage.
                 Defaults to None.
 
-            optimizer_config (Optional[OptimizerConfig], optional): If provided, will redefine the optimizer for fine-tuning
-                stage. Defaults to None.
+            optimizer_config (Optional[OptimizerConfig], optional):
+                If provided, will redefine the optimizer for fine-tuning stage. Defaults to None.
 
-            trainer_config (Optional[TrainerConfig], optional): If provided, will redefine the trainer for fine-tuning stage.
-                Defaults to None.
+            trainer_config (Optional[TrainerConfig], optional):
+                If provided, will redefine the trainer for fine-tuning stage. Defaults to None.
 
-            experiment_config (Optional[ExperimentConfig], optional): If provided, will redefine the experiment for fine-tuning
-                stage. Defaults to None.
+            experiment_config (Optional[ExperimentConfig], optional):
+                If provided, will redefine the experiment for fine-tuning stage. Defaults to None.
 
-            loss (Optional[torch.nn.Module], optional): If provided, will be used as the loss function for the fine-tuning.
+            loss (Optional[torch.nn.Module], optional):
+                If provided, will be used as the loss function for the fine-tuning.
                 By Default it is MSELoss for regression and CrossEntropyLoss for classification.
 
             metrics (Optional[List[Callable]], optional): List of metrics (either callables or str) to be used for the
-                fine-tuning stage. If str, it should be one of the functional metrics implemented in ``torchmetrics.functional``
-                Defaults to None.
+                fine-tuning stage. If str, it should be one of the functional metrics implemented in
+                ``torchmetrics.functional``. Defaults to None.
+
+            metrics_prob_input (Optional[List[bool]], optional): Is a mandatory parameter for classification metrics
+                This defines whether the input to the metric function is the probability or the class.
+                Length should be same as the number of metrics. Defaults to None.
 
             metrics_params (Optional[Dict], optional): The parameters for the metrics in the same order as metrics.
-                For eg. f1_score for multi-class needs a parameter `average` to fully define the metric. Defaults to None.
+                For eg. f1_score for multi-class needs a parameter `average` to fully define the metric.
+                Defaults to None.
 
-            optimizer (Optional[torch.optim.Optimizer], optional): Custom optimizers which are a drop in replacements for
-                standard PyTorch optimizers. If provided, the OptimizerConfig is ignored in favor of this. Defaults to None.
+            optimizer (Optional[torch.optim.Optimizer], optional):
+                Custom optimizers which are a drop in replacements for standard PyTorch optimizers. If provided,
+                the OptimizerConfig is ignored in favor of this. Defaults to None.
 
             optimizer_params (Dict, optional): The parameters for the optimizer. Defaults to {}.
 
             learning_rate (Optional[float], optional): The learning rate to be used. Defaults to 1e-3.
 
             target_range (Optional[Tuple[float, float]], optional): The target range for the regression task.
                 Is ignored for classification. Defaults to None.
@@ -823,53 +871,52 @@
         inferred_config = self.datamodule.update_config(config)
         inferred_config = OmegaConf.structured(inferred_config)
         # Adding dummy attributes for compatibility. Not used because custom metrics are provided
         if not hasattr(config, "metrics"):
             config.metrics = "dummy"
         if not hasattr(config, "metrics_params"):
             config.metrics_params = {}
+        if not hasattr(config, "metrics_prob_input"):
+            config.metrics_prob_input = metrics_prob_input or [False]
         if metrics is not None:
             assert len(metrics) == len(metrics_params), "Number of metrics and metrics_params should be same"
+            assert len(metrics) == len(metrics_prob_input), "Number of metrics and metrics_prob_input should be same"
             metrics = [getattr(torchmetrics.functional, m) if isinstance(m, str) else m for m in metrics]
         if task == "regression":
-            loss = loss if loss is not None else torch.nn.MSELoss()
+            loss = loss or torch.nn.MSELoss()
             if metrics is None:
                 metrics = [torchmetrics.functional.mean_squared_error]
                 metrics_params = [{}]
         elif task == "classification":
-            loss = loss if loss is not None else torch.nn.CrossEntropyLoss()
+            loss = loss or torch.nn.CrossEntropyLoss()
             if metrics is None:
                 metrics = [torchmetrics.functional.accuracy]
-                metrics_params = [
-                    {
-                        "task": "multiclass",
-                        "num_classes": inferred_config.output_dim,
-                    }
-                ]
+                metrics_params = [{"task": "multiclass", "num_classes": inferred_config.output_dim, "top_k": 1}]
+                metrics_prob_input = [False]
             else:
                 for i, mp in enumerate(metrics_params):
-                    if "task" not in mp:
-                        # For classification task, output_dim == number of classses
-                        metrics_params[i]["task"] = "multiclass"
-                    if "num_classes" not in mp:
-                        metrics_params[i]["num_classes"] = inferred_config.output_dim
+                    # For classification task, output_dim == number of classses
+                    metrics_params[i]["task"] = mp.get("task", "multiclass")
+                    metrics_params[i]["num_classes"] = mp.get("num_classes", inferred_config.output_dim)
+                    metrics_params[i]["top_k"] = mp.get("top_k", 1)
         # Forming partial callables using metrics and metric params
         metrics = [partial(m, **mp) for m, mp in zip(metrics, metrics_params)]
         self.model.mode = "finetune"
         if learning_rate is not None:
             config.learning_rate = learning_rate
         config.target_range = target_range
         model_args = {
             "backbone": self.model,
             "head": head,
             "head_config": head_config,
             "config": config,
             "inferred_config": inferred_config,
             "custom_loss": loss,
             "custom_metrics": metrics,
+            "custom_metrics_prob_inputs": metrics_prob_input,
             "custom_optimizer": optimizer,
             "custom_optimizer_params": optimizer_params,
         }
         # Initializing with default metrics, losses, and optimizers. Will revert once initialized
         model = model_callable(
             **model_args,
         )
@@ -898,28 +945,28 @@
             train (pd.DataFrame): The training data with labels
 
             validation (Optional[pd.DataFrame], optional): The validation data with labels. Defaults to None.
 
             train_sampler (Optional[torch.utils.data.Sampler], optional): If provided, will be used as a batch sampler
                 for training. Defaults to None.
 
-            target_transform (Optional[Union[TransformerMixin, Tuple]], optional): If provided, will be used to transform
-                the target before training and inverse transform the predictions.
+            target_transform (Optional[Union[TransformerMixin, Tuple]], optional): If provided, will be used
+                to transform the target before training and inverse transform the predictions.
 
             max_epochs (Optional[int], optional): The maximum number of epochs to train for. Defaults to None.
 
             min_epochs (Optional[int], optional): The minimum number of epochs to train for. Defaults to None.
 
             seed (Optional[int], optional): The seed to be used for training. Defaults to 42.
 
             callbacks (Optional[List[pl.Callback]], optional): If provided, will be added to the callbacks for Trainer.
                 Defaults to None.
 
-            datamodule (Optional[TabularDatamodule], optional): If provided, will be used as the datamodule for training.
-                Defaults to None.
+            datamodule (Optional[TabularDatamodule], optional): If provided, will be used as the datamodule
+                for training. Defaults to None.
 
             freeze_backbone (bool, optional): If True, will freeze the backbone by tirning off gradients.
                 Defaults to False, which means the pretrained weights are also further tuned during fine-tuning.
 
         Returns:
             pl.Trainer: The trainer object
         """
@@ -948,15 +995,16 @@
             else:
                 self.datamodule.validation = None
             self.datamodule.train_sampler = train_sampler
             datamodule = self.datamodule
         else:
             if train is not None:
                 warnings.warn(
-                    "train data is provided but datamodule is provided. Ignoring the train data and using the datamodule"
+                    "train data is provided but datamodule is provided."
+                    " Ignoring the train data and using the datamodule"
                 )
         if freeze_backbone:
             for param in self.model.backbone.parameters():
                 param.requires_grad = False
         return self.train(
             self.model,
             datamodule,
@@ -973,15 +1021,16 @@
         max_lr: float = 1,
         num_training: int = 100,
         mode: str = "exponential",
         early_stop_threshold: Optional[float] = 4.0,
         plot: bool = True,
         callbacks: Optional[List] = None,
     ) -> Tuple[float, pd.DataFrame]:
-        """Enables the user to do a range test of good initial learning rates, to reduce the amount of guesswork in picking a good starting learning rate.
+        """Enables the user to do a range test of good initial learning rates, to reduce the amount of guesswork in
+        picking a good starting learning rate.
 
         Args:
             model (pl.LightningModule): The PyTorch Lightning model to be trained.
 
             datamodule (TabularDatamodule): The datamodule
 
             min_lr (Optional[float], optional): minimum learning rate to investigate
@@ -1001,15 +1050,14 @@
 
             plot (bool, optional): If true, will plot using matplotlib
 
             callbacks (Optional[List], optional): If provided, will be added to the callbacks for Trainer.
 
         Returns:
             The suggested learning rate and the learning rate finder results
-
         """
         self._prepare_for_training(model, datamodule, callbacks, max_epochs=None, min_epochs=None)
         train_loader, _ = datamodule.train_dataloader(), datamodule.val_dataloader()
         lr_finder = self.trainer.tuner.lr_find(
             model=self.model,
             train_dataloaders=train_loader,
             val_dataloaders=None,
@@ -1033,42 +1081,44 @@
     def evaluate(
         self,
         test: Optional[pd.DataFrame] = None,
         test_loader: Optional[torch.utils.data.DataLoader] = None,
         ckpt_path: Optional[Union[str, Path]] = None,
         verbose: bool = True,
     ) -> Union[dict, list]:
-        """Evaluates the dataframe using the loss and metrics already set in config
+        """Evaluates the dataframe using the loss and metrics already set in config.
 
         Args:
             test (Optional[pd.DataFrame]): The dataframe to be evaluated. If not provided, will try to use the
                 test provided during fit. If that was also not provided will return an empty dictionary
 
             test_loader (Optional[torch.utils.data.DataLoader], optional): The dataloader to be used for evaluation.
                 If provided, will use the dataloader instead of the test dataframe or the test data provided during fit.
                 DEPRECATION: providing test data during fit is deprecated and will be removed in a future release.
                 Defaults to None.
 
-            ckpt_path (Optional[Union[str, Path]], optional): The path to the checkpoint to be loaded. If not provided, will try to use the
-                best checkpoint during training.
+            ckpt_path (Optional[Union[str, Path]], optional): The path to the checkpoint to be loaded. If not provided,
+                will try to use the best checkpoint during training.
 
             verbose (bool, optional): If true, will print the results. Defaults to True.
         Returns:
             The final test result dictionary.
         """
         if test_loader is None and test is None:
             warnings.warn(
-                "Providing test in fit is deprecated. Not providing `test` or `test_loader` in `evaluate` will cause an error in a future release."
+                "Providing test in fit is deprecated."
+                " Not providing `test` or `test_loader` in `evaluate` will cause an error in a future release."
             )
         if test_loader is None:
             if test is not None:
                 test_loader = self.datamodule.prepare_inference_dataloader(test)
             elif self.datamodule.test is not None:
                 warnings.warn(
-                    "Providing test in fit is deprecated. Not providing `test` or `test_loader` in `evaluate` will cause an error in a future release."
+                    "Providing test in fit is deprecated."
+                    " Not providing `test` or `test_loader` in `evaluate` will cause an error in a future release."
                 )
                 test_loader = self.datamodule.test_dataloader()
             else:
                 return {}
         result = self.trainer.test(
             model=self.model,
             dataloaders=test_loader,
@@ -1082,15 +1132,15 @@
         test: pd.DataFrame,
         quantiles: Optional[List] = [0.25, 0.5, 0.75],
         n_samples: Optional[int] = 100,
         ret_logits=False,
         include_input_features: bool = True,
         device: Optional[torch.device] = None,
     ) -> pd.DataFrame:
-        """Uses the trained model to predict on new data and return as a dataframe
+        """Uses the trained model to predict on new data and return as a dataframe.
 
         Args:
             test (pd.DataFrame): The new dataframe with the features defined during training
             quantiles (Optional[List]): For probabilistic models like Mixture Density Networks, this specifies
                 the different quantiles to be extracted apart from the `central_tendency` and added to the dataframe.
                 For other models it is ignored. Defaults to [0.25, 0.5, 0.75]
             n_samples (Optional[int]): Number of samples to draw from the posterior to estimate the quantiles.
@@ -1101,18 +1151,19 @@
                 Defaults to True
 
         Returns:
             pd.DataFrame: Returns a dataframe with predictions and features (if `include_input_features=True`).
                 If classification, it returns probabilities and final prediction
         """
         warnings.warn(
-            "Default for `include_input_features` will change from True to False in the next release. Please set it explicitly.",
+            "Default for `include_input_features` will change from True to False in the next release."
+            " Please set it explicitly.",
             DeprecationWarning,
         )
-        assert all([q <= 1 and q >= 0 for q in quantiles]), "Quantiles should be a decimal between 0 and 1"
+        assert all(q <= 1 and q >= 0 for q in quantiles), "Quantiles should be a decimal between 0 and 1"
         if device is not None:
             if isinstance(device, str):
                 device = torch.device(device)
             if self.model.device != device:
                 model = self.model.to(device)
             else:
                 model = self.model
@@ -1198,42 +1249,42 @@
                     if v.shape[-1] > 1:
                         pred_df[f"{k}_{i}"] = v[:, i]
                     else:
                         pred_df[f"{k}"] = v[:, i]
         return pred_df
 
     def load_best_model(self) -> None:
-        """Loads the best model after training is done"""
+        """Loads the best model after training is done."""
         if self.trainer.checkpoint_callback is not None:
             logger.info("Loading the best model")
             ckpt_path = self.trainer.checkpoint_callback.best_model_path
             if ckpt_path != "":
                 logger.debug(f"Model Checkpoint: {ckpt_path}")
                 ckpt = pl_load(ckpt_path, map_location=lambda storage, loc: storage)
                 self.model.load_state_dict(ckpt["state_dict"])
             else:
                 logger.warning("No best model available to load. Did you run it more than 1 epoch?...")
         else:
             logger.warning("No best model available to load. Checkpoint Callback needs to be enabled for this to work")
 
     def save_datamodule(self, dir: str) -> None:
-        """Saves the datamodule in the specified directory
+        """Saves the datamodule in the specified directory.
 
         Args:
             dir (str): The path to the directory to save the datamodule
         """
         joblib.dump(self.datamodule, os.path.join(dir, "datamodule.sav"))
 
     def save_config(self, dir: str) -> None:
-        """Saves the config in the specified directory"""
+        """Saves the config in the specified directory."""
         with open(os.path.join(dir, "config.yml"), "w") as fp:
             OmegaConf.save(self.config, fp, resolve=True)
 
     def save_model(self, dir: str) -> None:
-        """Saves the model and checkpoints in the specified directory
+        """Saves the model and checkpoints in the specified directory.
 
         Args:
             dir (str): The path to the directory to save the model
         """
         if os.path.exists(dir) and (os.listdir(dir)):
             logger.warning("Directory is not empty. Overwriting the contents.")
             for f in os.listdir(dir):
@@ -1245,44 +1296,45 @@
             joblib.dump(self.logger, os.path.join(dir, "exp_logger.sav"))
         if hasattr(self, "callbacks"):
             joblib.dump(self.callbacks, os.path.join(dir, "callbacks.sav"))
         self.trainer.save_checkpoint(os.path.join(dir, "model.ckpt"))
         custom_params = {}
         custom_params["custom_loss"] = self.model.custom_loss
         custom_params["custom_metrics"] = self.model.custom_metrics
+        custom_params["custom_metrics_prob_inputs"] = self.model.custom_metrics_prob_inputs
         custom_params["custom_optimizer"] = self.model.custom_optimizer
         custom_params["custom_optimizer_params"] = self.model.custom_optimizer_params
         joblib.dump(custom_params, os.path.join(dir, "custom_params.sav"))
         if self.custom_model:
             joblib.dump(self.model_callable, os.path.join(dir, "custom_model_callable.sav"))
 
     def save_weights(self, path: Union[str, Path]) -> None:
-        """Saves the model weights in the specified directory
+        """Saves the model weights in the specified directory.
 
         Args:
             path (str): The path to the file to save the model
         """
         torch.save(self.model.state_dict(), path)
 
     def load_weights(self, path: Union[str, Path]) -> None:
-        """Loads the model weights in the specified directory
+        """Loads the model weights in the specified directory.
 
         Args:
             path (str): The path to the file to load the model from
         """
         self._load_weights(self.model, path)
 
     # TODO Need to test ONNX export
     def save_model_for_inference(
         self,
         path: Union[str, Path],
         kind: str = "pytorch",
-        onnx_export_params: Dict = dict(opset_version=12),
+        onnx_export_params: Dict = {"opset_version": 12},
     ) -> bool:
-        """Saves the model for inference
+        """Saves the model for inference.
 
         Args:
             path (Union[str, Path]): path to save the model
             kind (str): "pytorch" or "onnx" (Experimental)
             onnx_export_params (Dict): parameters for onnx export to be
                 passed to torch.onnx.export
 
@@ -1306,24 +1358,27 @@
                 dtype=torch.int,
             )
             cont = torch.randn(
                 self.config.batch_size,
                 len(self.config.continuous_cols),
                 requires_grad=True,
             )
-            x = dict(continuous=cont, categorical=cat)
+            x = {"continuous": cont, "categorical": cat}
             torch.onnx.export(self.model, x, str(path), **onnx_export_params)
             return True
         else:
             raise ValueError("`kind` must be either pytorch or onnx")
 
     def summary(self, max_depth: int = -1) -> None:
-        """Prints a summary of the model
+        """Prints a summary of the model.
 
         Args:
             max_depth (int): The maximum depth to traverse the modules and displayed in the summary.
                 Defaults to -1, which means will display all the modules.
         """
         print(summarize(self.model, max_depth=max_depth))
 
     def __str__(self) -> str:
         return self.summary()
+
+    def feature_importance(self):
+        return self.model.feature_importance()
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular/utils.py` & `pytorch_tabular-1.0.2/src/pytorch_tabular/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,22 @@
 from pathlib import Path
 from typing import Any, Callable, Dict, IO, Optional, Union
 
 import numpy as np
 import pandas as pd
 import torch
 import torch.nn as nn
-from lightning_lite.utilities.cloud_io import get_filesystem
 from sklearn.cluster import KMeans
 from sklearn.preprocessing import LabelEncoder
 
+try:  # for 1.8
+    from pytorch_lightning.utilities.cloud_io import get_filesystem
+except ImportError:  # for 1.9
+    from pytorch_lightning.core.saving import get_filesystem
+
 import pytorch_tabular as root_module
 
 _PATH = Union[str, Path]
 _DEVICE = Union[torch.device, str, int]
 _MAP_LOCATION_TYPE = Optional[Union[_DEVICE, Callable[[_DEVICE], _DEVICE], Dict[_DEVICE, _DEVICE]]]
 
 
@@ -30,15 +34,15 @@
     return logger
 
 
 logger = logging.getLogger(__name__)
 
 
 def _make_smooth_weights_for_balanced_classes(y_train, mu=1.0):
-    labels_dict = {label: count for label, count in zip(np.unique(y_train), np.bincount(y_train))}
+    labels_dict = dict(zip(np.unique(y_train), np.bincount(y_train)))
     total = np.sum(list(labels_dict.values()))
     keys = sorted(labels_dict.keys())
     weight = []
     for i in keys:
         score = np.log(mu * total / float(labels_dict[i]))
         weight.append(score if score > 1 else 1)
     return weight
@@ -176,16 +180,15 @@
         )
     fs = get_filesystem(path_or_url)
     with fs.open(path_or_url, "rb") as f:
         return torch.load(f, map_location=map_location)
 
 
 def reset_all_weights(model: nn.Module) -> None:
-    """
-    Resets all parameters in a network.
+    """Resets all parameters in a network.
 
     Args:
         model: The model to reset the parameters of.
 
     refs:
         - https://discuss.pytorch.org/t/how-to-re-set-alll-parameters-in-a-network/20819/6
         - https://stackoverflow.com/questions/63627997/reset-parameters-of-a-neural-network-in-pytorch
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular.egg-info/PKG-INFO` & `pytorch_tabular-1.0.2/src/pytorch_tabular.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-tabular
-Version: 1.0.1
+Version: 1.0.2
 Summary: A standard framework for using Deep Learning for tabular data
 Home-page: https://github.com/manujosephv/pytorch_tabular
 Author: Manu Joseph
 Author-email: manujosephv@gmail.com
 License: MIT license
 Description: ![PyTorch Tabular](docs/imgs/pytorch_tabular_logo.png)
         
@@ -141,45 +141,45 @@
         - [PyTorch Tabular – A Framework for Deep Learning for Tabular Data](https://deep-and-shallow.com/2021/01/27/pytorch-tabular-a-framework-for-deep-learning-for-tabular-data/)
         - [Neural Oblivious Decision Ensembles(NODE) – A State-of-the-Art Deep Learning Algorithm for Tabular Data](https://deep-and-shallow.com/2021/02/25/neural-oblivious-decision-ensemblesnode-a-state-of-the-art-deep-learning-algorithm-for-tabular-data/)
         - [Mixture Density Networks: Probabilistic Regression for Uncertainty Estimation](https://deep-and-shallow.com/2021/03/20/mixture-density-networks-probabilistic-regression-for-uncertainty-estimation/)
         
         ## Future Roadmap(Contributions are Welcome)
         
         1. Integrate Optuna Hyperparameter Tuning
-        1. Integrate SHAP for interpretability
-        1. Add Variable Importance
-        1. Add ability to use custom activations in CategoryEmbeddingModel
+        1. Integrate Captum for interpretability
+        1. Have a scikit-learn compatible API
         1. Add GaussRank as Feature Transformation
-        1. ~~Add differential dropouts(layer-wise) in CategoryEmbeddingModel~~
-        1. ~~Add Fourier Encoding for cyclic time variables~~
-        1. ~~Add Text and Image Modalities for mixed modal problems~~
+        1. Enable support for multi-label classification
+        1. Migrate Datamodule to Polars or Vaex for faster data loading and to handle larger than RAM datasets.
+        1. Keep adding more architectures
         
         ## Contributors
+        
         <!-- readme: contributors -start -->
         <table>
         <tr>
             <td align="center">
                 <a href="https://github.com/manujosephv">
                     <img src="https://avatars.githubusercontent.com/u/10508493?v=4" width="100;" alt="manujosephv"/>
                     <br />
                     <sub><b>Manu Joseph</b></sub>
                 </a>
             </td>
             <td align="center">
-                <a href="https://github.com/wsad1">
-                    <img src="https://avatars.githubusercontent.com/u/13963626?v=4" width="100;" alt="wsad1"/>
+                <a href="https://github.com/Borda">
+                    <img src="https://avatars.githubusercontent.com/u/6035284?v=4" width="100;" alt="Borda"/>
                     <br />
-                    <sub><b>Jinu Sunil</b></sub>
+                    <sub><b>Jirka Borovec</b></sub>
                 </a>
             </td>
             <td align="center">
-                <a href="https://github.com/Borda">
-                    <img src="https://avatars.githubusercontent.com/u/6035284?v=4" width="100;" alt="Borda"/>
+                <a href="https://github.com/wsad1">
+                    <img src="https://avatars.githubusercontent.com/u/13963626?v=4" width="100;" alt="wsad1"/>
                     <br />
-                    <sub><b>Jirka Borovec</b></sub>
+                    <sub><b>Jinu Sunil</b></sub>
                 </a>
             </td>
             <td align="center">
                 <a href="https://github.com/fonnesbeck">
                     <img src="https://avatars.githubusercontent.com/u/81476?v=4" width="100;" alt="fonnesbeck"/>
                     <br />
                     <sub><b>Chris Fonnesbeck</b></sub>
@@ -254,30 +254,62 @@
               primaryClass={cs.LG}
         }
         ```
         
         - Zenodo Software Citation
         
         ```
-        @article{manujosephv_2021,
-            title={manujosephv/pytorch_tabular: v0.7.0-alpha},
-            DOI={10.5281/zenodo.5359010},
-            abstractNote={<p>Added a few more SOTA models - TabTransformer, FTTransformer
-                Made improvements in the model save and load capability
-                Made installation less restrictive by unfreezing some dependencies.</p>},
-            publisher={Zenodo},
-            author={manujosephv},
-            year={2021},
-            month={May}
+        @software{manu_joseph_2023_7554473,
+          author       = {Manu Joseph and
+                          Jinu Sunil and
+                          Jiri Borovec and
+                          Chris Fonnesbeck and
+                          jxtrbtk and
+                          Andreas and
+                          JulianRein and
+                          Kushashwa Ravi Shrimali and
+                          Luca Actis Grosso and
+                          Sterling G. Baird and
+                          Yinyu Nie},
+          title        = {manujosephv/pytorch\_tabular: v1.0.1},
+          month        = jan,
+          year         = 2023,
+          publisher    = {Zenodo},
+          version      = {v1.0.1},
+          doi          = {10.5281/zenodo.7554473},
+          url          = {https://doi.org/10.5281/zenodo.7554473}
         }
         ```
         
         
         # History
         
+        ## 1.0.2 (2023-05-31)
+        
+        ### New Features:
+        
+        - Added Feature Importance: The library now includes a new method in TabularModel and BaseModel for enabling feature importance. Feature Importance has been enabled for FTTransformer and GATE models. [Commit: dc2a49e]
+        ### Enhancements:
+        
+        - Enabled two more parameters in the GATE model. [Commit: 3680413]
+        - Included metric_prob_input parameter in the library configuration. This update allows for better control over metrics in the models. [Commit: 0612db5]
+        - Slight improvements to the GATE model, including changes to defaults for better performance. [Commit: c30a6c3]
+        - Minor bug fixes and improvements, including accelerator options in the configuration and progress bar enhancements. [Commit: f932230, bdd9adb, f932230]
+        ### Dependency Updates:
+        
+        - Updated dependencies, including docformatter, pyupgrade, and ruff-pre-commit. [Commits: 4aae9a8, b3df4ce, bdd9adb, 55e800c, c6c4679, c01154b, 107cd2f]
+        ### Documentation Updates:
+        
+        - Updated the library's README.md file. [Commits: db8f3b2, cab6bf1, 669faec, 1e6c400, 3097799, 7fabf6b]
+        ### Other Improvements:
+        
+        - Various code optimizations, bug fixes, and CI enhancements. [Commits: 5637020, e5171bf, 812b40f]
+        
+        For more details, you can refer to the respective commits on the library's GitHub repository.
+        
         ## 1.0.1 (2023-01-20)
         
         - Bugfix for default metric for binary classification
```

### Comparing `pytorch_tabular-1.0.1/src/pytorch_tabular.egg-info/SOURCES.txt` & `pytorch_tabular-1.0.2/src/pytorch_tabular.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/tests/___test_augmentations.py` & `pytorch_tabular-1.0.2/tests/___test_augmentations.py`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/tests/conftest.py` & `pytorch_tabular-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytorch_tabular-1.0.1/tests/test_autoint.py` & `pytorch_tabular-1.0.2/tests/test_autoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         data_config = DataConfig(
             target=target + ["MedInc"] if multi_target else target,
             continuous_cols=continuous_cols,
             categorical_cols=categorical_cols,
             continuous_feature_transform=continuous_feature_transform,
             normalize_continuous_features=normalize_continuous_features,
         )
-        model_config_params = dict(task="regression")
+        model_config_params = {"task": "regression"}
         if target_range:
             _target_range = []
             for target in data_config.target:
                 _target_range.append(
                     (
                         float(train[target].min()),
                         float(train[target].max()),
@@ -108,15 +108,15 @@
         data_config = DataConfig(
             target=target,
             continuous_cols=continuous_cols,
             categorical_cols=categorical_cols,
             continuous_feature_transform=continuous_feature_transform,
             normalize_continuous_features=normalize_continuous_features,
         )
-        model_config_params = dict(task="classification")
+        model_config_params = {"task": "classification"}
         model_config_params["deep_layers"] = deep_layers
         model_config_params["batch_norm_continuous_input"] = batch_norm_continuous_input
         model_config = AutoIntConfig(**model_config_params)
         trainer_config = TrainerConfig(
             max_epochs=3,
             checkpoints=None,
             early_stopping=None,
```

### Comparing `pytorch_tabular-1.0.1/tests/test_categorical_embedding.py` & `pytorch_tabular-1.0.2/tests/test_categorical_embedding.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,17 @@
 @pytest.mark.parametrize(
     "target_transform",
     [None, PowerTransformer(), (lambda x: np.power(x, 2), lambda x: np.sqrt(x))],
 )
 # @pytest.mark.parametrize("custom_metrics", [None, [fake_metric]])
 # @pytest.mark.parametrize("custom_loss", [None, torch.nn.L1Loss()])
 # @pytest.mark.parametrize("custom_optimizer", [None, torch.optim.Adagrad])
-@pytest.mark.parametrize("custom_args", [(None, None, None), ([fake_metric], torch.nn.L1Loss(), torch.optim.Adagrad)])
+@pytest.mark.parametrize(
+    "custom_args", [(None, None, None, None), ([fake_metric], [False], torch.nn.L1Loss(), torch.optim.Adagrad)]
+)
 @pytest.mark.parametrize("custom_head_config", [None, "", "32", "32-32"])
 def test_regression(
     regression_data,
     multi_target,
     continuous_cols,
     categorical_cols,
     continuous_feature_transform,
@@ -56,39 +58,39 @@
     # custom_metrics,
     # custom_loss,
     # custom_optimizer,
     custom_args,
     custom_head_config,
 ):
     (train, test, target) = regression_data
-    (custom_metrics, custom_loss, custom_optimizer) = custom_args
+    (custom_metrics, custom_metrics_prob_input, custom_loss, custom_optimizer) = custom_args
     if len(continuous_cols) + len(categorical_cols) == 0:
         assert True
     else:
         data_config = DataConfig(
             target=target + ["MedInc"] if multi_target else target,
             continuous_cols=continuous_cols,
             categorical_cols=categorical_cols,
             continuous_feature_transform=continuous_feature_transform,
             normalize_continuous_features=normalize_continuous_features,
         )
-        model_config_params = dict(task="regression")
+        model_config_params = {"task": "regression"}
         if target_range:
             _target_range = []
             for target in data_config.target:
                 _target_range.append(
                     (
                         float(train[target].min()),
                         float(train[target].max()),
                     )
                 )
             model_config_params["target_range"] = _target_range
         if custom_head_config is not None:
             model_config_params["head"] = "LinearHead"
-            model_config_params["head_config"] = dict(layers=custom_head_config)
+            model_config_params["head_config"] = {"layers": custom_head_config}
         model_config = CategoryEmbeddingModelConfig(**model_config_params)
         trainer_config = TrainerConfig(
             max_epochs=3,
             checkpoints=None,
             early_stopping=None,
             accelerator="cpu",
             fast_dev_run=True,
@@ -101,14 +103,15 @@
             optimizer_config=optimizer_config,
             trainer_config=trainer_config,
         )
         tabular_model.fit(
             train=train,
             test=test,
             metrics=custom_metrics,
+            metrics_prob_inputs=custom_metrics_prob_input,
             target_transform=target_transform,
             loss=custom_loss,
             optimizer=custom_optimizer,
             optimizer_params={},
         )
 
         result = tabular_model.evaluate(test)
@@ -145,15 +148,15 @@
         data_config = DataConfig(
             target=target,
             continuous_cols=continuous_cols,
             categorical_cols=categorical_cols,
             continuous_feature_transform=continuous_feature_transform,
             normalize_continuous_features=normalize_continuous_features,
         )
-        model_config_params = dict(task="classification")
+        model_config_params = {"task": "classification"}
         model_config = CategoryEmbeddingModelConfig(**model_config_params)
         trainer_config = TrainerConfig(
             max_epochs=3,
             checkpoints=None,
             early_stopping=None,
             accelerator="cpu",
             fast_dev_run=True,
@@ -185,15 +188,15 @@
             "Population",
             "AveOccup",
             "Latitude",
             "Longitude",
         ],
         categorical_cols=["HouseAgeBin"],
     )
-    model_config_params = dict(task="regression")
+    model_config_params = {"task": "regression"}
     model_config = CategoryEmbeddingModelConfig(**model_config_params)
     trainer_config = TrainerConfig(
         max_epochs=1,
         checkpoints=None,
         early_stopping=None,
         accelerator="cpu",
         fast_dev_run=True,
@@ -208,8 +211,8 @@
     )
     tabular_model.fit(train=train, test=test)
 
     transformer = CategoricalEmbeddingTransformer(tabular_model)
     train_transform = transformer.fit_transform(train)
     embed_cols = [col for col in train_transform.columns if "HouseAgeBin_embed_dim" in col]
     assert len(train["HouseAgeBin"].unique()) + 1 == len(transformer._mapping["HouseAgeBin"].keys())
-    assert all([val.shape[0] == len(embed_cols) for val in transformer._mapping["HouseAgeBin"].values()])
+    assert all(val.shape[0] == len(embed_cols) for val in transformer._mapping["HouseAgeBin"].values())
```

### Comparing `pytorch_tabular-1.0.1/tests/test_common.py` & `pytorch_tabular-1.0.2/tests/test_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 from pytorch_tabular.models import AutoIntConfig, CategoryEmbeddingModelConfig, NodeConfig, TabNetModelConfig
 from pytorch_tabular.ssl_models import DenoisingAutoEncoderConfig
 
 # import os
 
 
 MODEL_CONFIG_SAVE_TEST = [
-    (CategoryEmbeddingModelConfig, dict(layers="10-20")),
-    (AutoIntConfig, dict(num_heads=1, num_attn_blocks=1)),
-    (NodeConfig, dict(num_trees=100, depth=2)),
-    (TabNetModelConfig, dict(n_a=2, n_d=2)),
+    (CategoryEmbeddingModelConfig, {"layers": "10-20"}),
+    (AutoIntConfig, {"num_heads": 1, "num_attn_blocks": 1}),
+    (NodeConfig, {"num_trees": 100, "depth": 2}),
+    (TabNetModelConfig, {"n_a": 2, "n_d": 2}),
 ]
 
 MODEL_CONFIG_SAVE_ONNX_TEST = [
-    (CategoryEmbeddingModelConfig, dict(layers="10-20")),
+    (CategoryEmbeddingModelConfig, {"layers": "10-20"}),
     (
         AutoIntConfig,
-        dict(
-            num_heads=1,
-            num_attn_blocks=1,
-        ),
+        {
+            "num_heads": 1,
+            "num_attn_blocks": 1,
+        },
     ),
 ]
 MODEL_CONFIG_FEATURE_EXT_TEST = [
     CategoryEmbeddingModelConfig,
     AutoIntConfig,
     DenoisingAutoEncoderConfig,
 ]
@@ -85,14 +85,15 @@
         optimizer_config=optimizer_config,
         trainer_config=trainer_config,
     )
     tabular_model.fit(
         train=train,
         test=test,
         metrics=custom_metrics,
+        metrics_prob_inputs=None if custom_metrics is None else [False],
         loss=custom_loss,
         optimizer=custom_optimizer,
         optimizer_params={},
     )
 
     result_1 = tabular_model.evaluate(test)
     # sv_dir = tmpdir/"save_model"
@@ -121,15 +122,15 @@
     data_config = DataConfig(
         target=target,
         continuous_cols=continuous_cols,
         categorical_cols=categorical_cols,
         handle_missing_values=False if is_ssl else True,
         handle_unknown_categories=False if is_ssl else True,
     )
-    model_config_params = dict()
+    model_config_params = {}
     if not is_ssl:
         model_config_params["task"] = "regression"
     else:
         encoder_config = CategoryEmbeddingModelConfig(
             task="backbone",
             layers="4096-2048-512",  # Number of nodes in each layer
             activation="LeakyReLU",  # Activation between each layers
@@ -165,15 +166,15 @@
     else:
         tabular_model.fit(
             train=train,
             validation=test,
         )
     dt = DeepFeatureExtractor(tabular_model)
     enc_df = dt.fit_transform(test)
-    assert any([col for col in enc_df.columns if "backbone" in col])
+    assert any(col for col in enc_df.columns if "backbone" in col)
 
 
 @pytest.mark.parametrize("model_config_class", MODEL_CONFIG_SAVE_TEST)
 @pytest.mark.parametrize("continuous_cols", [list(DATASET_CONTINUOUS_COLUMNS)])
 @pytest.mark.parametrize("categorical_cols", [["HouseAgeBin"]])
 @pytest.mark.parametrize("custom_metrics", [None, [fake_metric]])
 @pytest.mark.parametrize("custom_loss", [None, torch.nn.L1Loss()])
@@ -212,14 +213,15 @@
         optimizer_config=optimizer_config,
         trainer_config=trainer_config,
     )
     tabular_model.fit(
         train=train,
         test=test,
         metrics=custom_metrics,
+        metrics_prob_inputs=None if custom_metrics is None else [False],
         loss=custom_loss,
         optimizer=custom_optimizer,
         optimizer_params={},
     )
 
     result_1 = tabular_model.evaluate(test)
     # sv_dir = tmpdir/"save_model"
@@ -233,14 +235,15 @@
         trainer_config=trainer_config,
         model_state_dict_path=str(sv_dir / "weights.pt"),
     )
     datamodule = new_mdl.prepare_dataloader(train, test=test)
     model = new_mdl.prepare_model(
         datamodule,
         metrics=custom_metrics,
+        metrics_prob_inputs=None if custom_metrics is None else [False],
         loss=custom_loss,
         optimizer=custom_optimizer,
         optimizer_params={},
     )
     new_mdl._prepare_for_training(model, datamodule)
     result_2 = new_mdl.evaluate(test)
     assert (
@@ -306,14 +309,15 @@
         optimizer_config=optimizer_config,
         trainer_config=trainer_config,
     )
     tabular_model.fit(
         train=train,
         test=test,
         metrics=custom_metrics,
+        metrics_prob_inputs=None if custom_metrics is None else [False],
         loss=custom_loss,
         optimizer=custom_optimizer,
         optimizer_params={},
     )
     sv_dir = tmpdir.mkdir("saved_model")
 
     tabular_model.save_model_for_inference(
@@ -337,15 +341,15 @@
     data_config = DataConfig(
         target=target,
         continuous_cols=continuous_cols,
         categorical_cols=categorical_cols,
         handle_missing_values=False if is_ssl else True,
         handle_unknown_categories=False if is_ssl else True,
     )
-    model_config_params = dict()
+    model_config_params = {}
     if not is_ssl:
         model_config_params["task"] = "regression"
     else:
         encoder_config = CategoryEmbeddingModelConfig(
             task="backbone",
             layers="4096-2048-512",  # Number of nodes in each layer
             activation="LeakyReLU",  # Activation between each layers
```

### Comparing `pytorch_tabular-1.0.1/tests/test_datamodule.py` & `pytorch_tabular-1.0.2/tests/test_datamodule.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             target=target + ["MedInc"] if multi_target else target,
             continuous_cols=continuous_cols,
             categorical_cols=categorical_cols,
             continuous_feature_transform=continuous_feature_transform,
             normalize_continuous_features=normalize_continuous_features,
             validation_split=validation_split,
         )
-        model_config_params = dict(task="regression", embedding_dims=embedding_dims)
+        model_config_params = {"task": "regression", "embedding_dims": embedding_dims}
         model_config = CategoryEmbeddingModelConfig(**model_config_params)
         trainer_config = TrainerConfig(max_epochs=1, checkpoints=None, early_stopping=None)
         optimizer_config = OptimizerConfig()
 
         tabular_model = TabularModel(
             data_config=data_config,
             model_config=model_config,
@@ -113,15 +113,15 @@
     data_config = DataConfig(
         target=target + ["Occupancy"],
         continuous_cols=["Temperature", "Humidity", "Light", "CO2", "HumidityRatio"],
         categorical_cols=[],
         date_columns=[("date", freq)],
         encode_date_columns=True,
     )
-    model_config_params = dict(task="regression")
+    model_config_params = {"task": "regression"}
     model_config = CategoryEmbeddingModelConfig(**model_config_params)
     trainer_config = TrainerConfig(max_epochs=1, checkpoints=None, early_stopping=None)
     optimizer_config = OptimizerConfig()
 
     tabular_model = TabularModel(
         data_config=data_config,
         model_config=model_config,
```

### Comparing `pytorch_tabular-1.0.1/tests/test_ft_transformer.py` & `pytorch_tabular-1.0.2/tests/test_gate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python
 """Tests for `pytorch_tabular` package."""
 import pytest
 
 from pytorch_tabular import TabularModel
-from pytorch_tabular.categorical_encoders import CategoricalEmbeddingTransformer
 from pytorch_tabular.config import DataConfig, OptimizerConfig, TrainerConfig
-from pytorch_tabular.models import FTTransformerConfig
+from pytorch_tabular.models import GatedAdditiveTreeEnsembleConfig
+
+# from pytorch_tabular.categorical_encoders import CategoricalEmbeddingTransformer
 
 
 @pytest.mark.parametrize("multi_target", [True, False])
 @pytest.mark.parametrize(
     "continuous_cols",
     [
         [
@@ -42,31 +43,31 @@
         data_config = DataConfig(
             target=target + ["MedInc"] if multi_target else target,
             continuous_cols=continuous_cols,
             categorical_cols=categorical_cols,
             continuous_feature_transform=continuous_feature_transform,
             normalize_continuous_features=normalize_continuous_features,
         )
-        model_config_params = dict(
-            task="regression",
-            input_embed_dim=8,
-            num_attn_blocks=1,
-            num_heads=2,
-        )
+        model_config_params = {
+            "task": "regression",
+            "gflu_stages": 1,
+            "tree_depth": 1,
+            "num_trees": 2,
+        }
         if target_range:
             _target_range = []
             for target in data_config.target:
                 _target_range.append(
                     (
                         float(train[target].min()),
                         float(train[target].max()),
                     )
                 )
             model_config_params["target_range"] = _target_range
-        model_config = FTTransformerConfig(**model_config_params)
+        model_config = GatedAdditiveTreeEnsembleConfig(**model_config_params)
         trainer_config = TrainerConfig(
             max_epochs=1,
             checkpoints=None,
             early_stopping=None,
             accelerator="cpu",
             fast_dev_run=True,
         )
@@ -109,21 +110,21 @@
         data_config = DataConfig(
             target=target,
             continuous_cols=continuous_cols,
             categorical_cols=categorical_cols,
             continuous_feature_transform=continuous_feature_transform,
             normalize_continuous_features=normalize_continuous_features,
         )
-        model_config_params = dict(
-            task="classification",
-            input_embed_dim=8,
-            num_attn_blocks=1,
-            num_heads=2,
-        )
-        model_config = FTTransformerConfig(**model_config_params)
+        model_config_params = {
+            "task": "classification",
+            "gflu_stages": 1,
+            "tree_depth": 1,
+            "num_trees": 2,
+        }
+        model_config = GatedAdditiveTreeEnsembleConfig(**model_config_params)
         trainer_config = TrainerConfig(
             max_epochs=1,
             checkpoints=None,
             early_stopping=None,
             accelerator="cpu",
             fast_dev_run=True,
         )
@@ -139,50 +140,59 @@
 
         result = tabular_model.evaluate(test)
         assert "test_accuracy" in result[0].keys()
         pred_df = tabular_model.predict(test)
         assert pred_df.shape[0] == test.shape[0]
 
 
-def test_embedding_transformer(regression_data):
-    (train, test, target) = regression_data
-    data_config = DataConfig(
-        target=target,
-        continuous_cols=[
-            "AveRooms",
-            "AveBedrms",
-            "Population",
-            "AveOccup",
-            "Latitude",
-            "Longitude",
-        ],
-        categorical_cols=["HouseAgeBin"],
-    )
-    model_config_params = dict(
-        task="regression",
-        input_embed_dim=8,
-        num_attn_blocks=1,
-        num_heads=2,
-    )
-    model_config = FTTransformerConfig(**model_config_params)
-    trainer_config = TrainerConfig(
-        max_epochs=1,
-        checkpoints=None,
-        early_stopping=None,
-        accelerator="cpu",
-        fast_dev_run=True,
-    )
-    optimizer_config = OptimizerConfig()
-
-    tabular_model = TabularModel(
-        data_config=data_config,
-        model_config=model_config,
-        optimizer_config=optimizer_config,
-        trainer_config=trainer_config,
-    )
-    tabular_model.fit(train=train, test=test)
-
-    transformer = CategoricalEmbeddingTransformer(tabular_model)
-    train_transform = transformer.fit_transform(train)
-    embed_cols = [col for col in train_transform.columns if "HouseAgeBin_embed_dim" in col]
-    assert len(train["HouseAgeBin"].unique()) + 1 == len(transformer._mapping["HouseAgeBin"].keys())
-    assert all([val.shape[0] == len(embed_cols) for val in transformer._mapping["HouseAgeBin"].values()])
+# def test_embedding_transformer(regression_data):
+#     (train, test, target) = regression_data
+#     data_config = DataConfig(
+#         target=target,
+#         continuous_cols=[
+#             "AveRooms",
+#             "AveBedrms",
+#             "Population",
+#             "AveOccup",
+#             "Latitude",
+#             "Longitude",
+#         ],
+#         categorical_cols=["HouseAgeBin"],
+#     )
+#     model_config_params = dict(
+#         task="regression",
+#         input_embed_dim=8,
+#         num_attn_blocks=1,
+#         num_heads=2,
+#     )
+#     model_config = FTTransformerConfig(**model_config_params)
+#     trainer_config = TrainerConfig(
+#         max_epochs=1,
+#         checkpoints=None,
+#         early_stopping=None,
+#         accelerator="cpu",
+#         fast_dev_run=True,
+#     )
+#     optimizer_config = OptimizerConfig()
+
+#     tabular_model = TabularModel(
+#         data_config=data_config,
+#         model_config=model_config,
+#         optimizer_config=optimizer_config,
+#         trainer_config=trainer_config,
+#     )
+#     tabular_model.fit(train=train, test=test)
+
+#     transformer = CategoricalEmbeddingTransformer(tabular_model)
+#     train_transform = transformer.fit_transform(train)
+#     embed_cols = [
+#         col for col in train_transform.columns if "HouseAgeBin_embed_dim" in col
+#     ]
+#     assert len(train["HouseAgeBin"].unique()) + 1 == len(
+#         transformer._mapping["HouseAgeBin"].keys()
+#     )
+#     assert all(
+#         [
+#             val.shape[0] == len(embed_cols)
+#             for val in transformer._mapping["HouseAgeBin"].values()
+#         ]
+#     )
```

### Comparing `pytorch_tabular-1.0.1/tests/test_gate.py` & `pytorch_tabular-1.0.2/tests/test_tabtransformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 #!/usr/bin/env python
 """Tests for `pytorch_tabular` package."""
 import pytest
 
 from pytorch_tabular import TabularModel
+from pytorch_tabular.categorical_encoders import CategoricalEmbeddingTransformer
 from pytorch_tabular.config import DataConfig, OptimizerConfig, TrainerConfig
-from pytorch_tabular.models import GatedAdditiveTreeEnsembleConfig
-
-# from pytorch_tabular.categorical_encoders import CategoricalEmbeddingTransformer
+from pytorch_tabular.models import TabTransformerConfig
 
 
 @pytest.mark.parametrize("multi_target", [True, False])
 @pytest.mark.parametrize(
     "continuous_cols",
     [
         [
@@ -19,15 +18,15 @@
             "Population",
             "AveOccup",
             "Latitude",
             "Longitude",
         ],
     ],
 )
-@pytest.mark.parametrize("categorical_cols", [["HouseAgeBin"], []])
+@pytest.mark.parametrize("categorical_cols", [["HouseAgeBin"]])
 @pytest.mark.parametrize("continuous_feature_transform", [None])
 @pytest.mark.parametrize("normalize_continuous_features", [True])
 @pytest.mark.parametrize("target_range", [True, False])
 def test_regression(
     regression_data,
     multi_target,
     continuous_cols,
@@ -43,31 +42,31 @@
         data_config = DataConfig(
             target=target + ["MedInc"] if multi_target else target,
             continuous_cols=continuous_cols,
             categorical_cols=categorical_cols,
             continuous_feature_transform=continuous_feature_transform,
             normalize_continuous_features=normalize_continuous_features,
         )
-        model_config_params = dict(
-            task="regression",
-            gflu_stages=1,
-            tree_depth=1,
-            num_trees=2,
-        )
+        model_config_params = {
+            "task": "regression",
+            "input_embed_dim": 8,
+            "num_attn_blocks": 1,
+            "num_heads": 2,
+        }
         if target_range:
             _target_range = []
             for target in data_config.target:
                 _target_range.append(
                     (
                         float(train[target].min()),
                         float(train[target].max()),
                     )
                 )
             model_config_params["target_range"] = _target_range
-        model_config = GatedAdditiveTreeEnsembleConfig(**model_config_params)
+        model_config = TabTransformerConfig(**model_config_params)
         trainer_config = TrainerConfig(
             max_epochs=1,
             checkpoints=None,
             early_stopping=None,
             accelerator="cpu",
             fast_dev_run=True,
         )
@@ -110,21 +109,21 @@
         data_config = DataConfig(
             target=target,
             continuous_cols=continuous_cols,
             categorical_cols=categorical_cols,
             continuous_feature_transform=continuous_feature_transform,
             normalize_continuous_features=normalize_continuous_features,
         )
-        model_config_params = dict(
-            task="classification",
-            gflu_stages=1,
-            tree_depth=1,
-            num_trees=2,
-        )
-        model_config = GatedAdditiveTreeEnsembleConfig(**model_config_params)
+        model_config_params = {
+            "task": "classification",
+            "input_embed_dim": 8,
+            "num_attn_blocks": 1,
+            "num_heads": 2,
+        }
+        model_config = TabTransformerConfig(**model_config_params)
         trainer_config = TrainerConfig(
             max_epochs=1,
             checkpoints=None,
             early_stopping=None,
             accelerator="cpu",
             fast_dev_run=True,
         )
@@ -140,59 +139,50 @@
 
         result = tabular_model.evaluate(test)
         assert "test_accuracy" in result[0].keys()
         pred_df = tabular_model.predict(test)
         assert pred_df.shape[0] == test.shape[0]
 
 
-# def test_embedding_transformer(regression_data):
-#     (train, test, target) = regression_data
-#     data_config = DataConfig(
-#         target=target,
-#         continuous_cols=[
-#             "AveRooms",
-#             "AveBedrms",
-#             "Population",
-#             "AveOccup",
-#             "Latitude",
-#             "Longitude",
-#         ],
-#         categorical_cols=["HouseAgeBin"],
-#     )
-#     model_config_params = dict(
-#         task="regression",
-#         input_embed_dim=8,
-#         num_attn_blocks=1,
-#         num_heads=2,
-#     )
-#     model_config = FTTransformerConfig(**model_config_params)
-#     trainer_config = TrainerConfig(
-#         max_epochs=1,
-#         checkpoints=None,
-#         early_stopping=None,
-#         accelerator="cpu",
-#         fast_dev_run=True,
-#     )
-#     optimizer_config = OptimizerConfig()
-
-#     tabular_model = TabularModel(
-#         data_config=data_config,
-#         model_config=model_config,
-#         optimizer_config=optimizer_config,
-#         trainer_config=trainer_config,
-#     )
-#     tabular_model.fit(train=train, test=test)
-
-#     transformer = CategoricalEmbeddingTransformer(tabular_model)
-#     train_transform = transformer.fit_transform(train)
-#     embed_cols = [
-#         col for col in train_transform.columns if "HouseAgeBin_embed_dim" in col
-#     ]
-#     assert len(train["HouseAgeBin"].unique()) + 1 == len(
-#         transformer._mapping["HouseAgeBin"].keys()
-#     )
-#     assert all(
-#         [
-#             val.shape[0] == len(embed_cols)
-#             for val in transformer._mapping["HouseAgeBin"].values()
-#         ]
-#     )
+def test_embedding_transformer(regression_data):
+    (train, test, target) = regression_data
+    data_config = DataConfig(
+        target=target,
+        continuous_cols=[
+            "AveRooms",
+            "AveBedrms",
+            "Population",
+            "AveOccup",
+            "Latitude",
+            "Longitude",
+        ],
+        categorical_cols=["HouseAgeBin"],
+    )
+    model_config_params = {
+        "task": "regression",
+        "input_embed_dim": 8,
+        "num_attn_blocks": 1,
+        "num_heads": 2,
+    }
+    model_config = TabTransformerConfig(**model_config_params)
+    trainer_config = TrainerConfig(
+        max_epochs=1,
+        checkpoints=None,
+        early_stopping=None,
+        accelerator="cpu",
+        fast_dev_run=True,
+    )
+    optimizer_config = OptimizerConfig()
+
+    tabular_model = TabularModel(
+        data_config=data_config,
+        model_config=model_config,
+        optimizer_config=optimizer_config,
+        trainer_config=trainer_config,
+    )
+    tabular_model.fit(train=train, test=test)
+
+    transformer = CategoricalEmbeddingTransformer(tabular_model)
+    train_transform = transformer.fit_transform(train)
+    embed_cols = [col for col in train_transform.columns if "HouseAgeBin_embed_dim" in col]
+    assert len(train["HouseAgeBin"].unique()) + 1 == len(transformer._mapping["HouseAgeBin"].keys())
+    assert all(val.shape[0] == len(embed_cols) for val in transformer._mapping["HouseAgeBin"].values())
```

### Comparing `pytorch_tabular-1.0.1/tests/test_mdn.py` & `pytorch_tabular-1.0.2/tests/test_mdn.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,19 +44,19 @@
         data_config = DataConfig(
             target=target + ["MedInc"] if multi_target else target,
             continuous_cols=continuous_cols,
             categorical_cols=categorical_cols,
             continuous_feature_transform=continuous_feature_transform,
             normalize_continuous_features=normalize_continuous_features,
         )
-        model_config_params = dict(task="regression")
-        mdn_config = dict(num_gaussian=num_gaussian)
+        model_config_params = {"task": "regression"}
+        mdn_config = {"num_gaussian": num_gaussian}
         model_config_params["head_config"] = mdn_config
         model_config_params["backbone_config_class"] = variant
-        model_config_params["backbone_config_params"] = dict(task="backbone")
+        model_config_params["backbone_config_params"] = {"task": "backbone"}
 
         model_config = MDNConfig(**model_config_params)
         trainer_config = TrainerConfig(
             max_epochs=3,
             checkpoints=None,
             early_stopping=None,
             accelerator="cpu",
@@ -105,19 +105,19 @@
         data_config = DataConfig(
             target=target,
             continuous_cols=continuous_cols,
             categorical_cols=categorical_cols,
             continuous_feature_transform=continuous_feature_transform,
             normalize_continuous_features=normalize_continuous_features,
         )
-        model_config_params = dict(task="classification")
-        mdn_config = dict(num_gaussian=num_gaussian)
+        model_config_params = {"task": "classification"}
+        mdn_config = {"num_gaussian": num_gaussian}
         model_config_params["head_config"] = mdn_config
         model_config_params["backbone_config_class"] = "CategoryEmbeddingMDNConfig"
-        model_config_params["backbone_config_params"] = dict(task="backbone")
+        model_config_params["backbone_config_params"] = {"task": "backbone"}
 
         model_config = MDNConfig(**model_config_params)
         trainer_config = TrainerConfig(
             max_epochs=3,
             checkpoints=None,
             early_stopping=None,
             accelerator="cpu",
```

### Comparing `pytorch_tabular-1.0.1/tests/test_node.py` & `pytorch_tabular-1.0.2/tests/test_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,20 +44,20 @@
         data_config = DataConfig(
             target=target + ["MedInc"] if multi_target else target,
             continuous_cols=continuous_cols,
             categorical_cols=categorical_cols,
             continuous_feature_transform=continuous_feature_transform,
             normalize_continuous_features=normalize_continuous_features,
         )
-        model_config_params = dict(
-            task="regression",
-            depth=2,
-            num_trees=50,
-            embed_categorical=embed_categorical,
-        )
+        model_config_params = {
+            "task": "regression",
+            "depth": 2,
+            "num_trees": 50,
+            "embed_categorical": embed_categorical,
+        }
         if target_range:
             _target_range = []
             for target in data_config.target:
                 _target_range.append(
                     (
                         float(train[target].min()),
                         float(train[target].max()),
@@ -113,20 +113,20 @@
         data_config = DataConfig(
             target=target,
             continuous_cols=continuous_cols,
             categorical_cols=categorical_cols,
             continuous_feature_transform=continuous_feature_transform,
             normalize_continuous_features=normalize_continuous_features,
         )
-        model_config_params = dict(
-            task="classification",
-            depth=2,
-            num_trees=50,
-            embed_categorical=embed_categorical,
-        )
+        model_config_params = {
+            "task": "classification",
+            "depth": 2,
+            "num_trees": 50,
+            "embed_categorical": embed_categorical,
+        }
         model_config = NodeConfig(**model_config_params)
         trainer_config = TrainerConfig(
             max_epochs=1,
             checkpoints=None,
             early_stopping=None,
             accelerator="cpu",
             fast_dev_run=True,
@@ -157,15 +157,15 @@
             "Population",
             "AveOccup",
             "Latitude",
             "Longitude",
         ],
         categorical_cols=["HouseAgeBin"],
     )
-    model_config_params = dict(task="regression", depth=2, num_trees=50, embed_categorical=True)
+    model_config_params = {"task": "regression", "depth": 2, "num_trees": 50, "embed_categorical": True}
     model_config = NodeConfig(**model_config_params)
     trainer_config = TrainerConfig(
         max_epochs=1,
         checkpoints=None,
         early_stopping=None,
         accelerator="cpu",
         fast_dev_run=True,
@@ -180,8 +180,8 @@
     )
     tabular_model.fit(train=train, test=test)
 
     transformer = CategoricalEmbeddingTransformer(tabular_model)
     train_transform = transformer.fit_transform(train)
     embed_cols = [col for col in train_transform.columns if "HouseAgeBin_embed_dim" in col]
     assert len(train["HouseAgeBin"].unique()) + 1 == len(transformer._mapping["HouseAgeBin"].keys())
-    assert all([val.shape[0] == len(embed_cols) for val in transformer._mapping["HouseAgeBin"].values()])
+    assert all(val.shape[0] == len(embed_cols) for val in transformer._mapping["HouseAgeBin"].values())
```

### Comparing `pytorch_tabular-1.0.1/tests/test_ssl.py` & `pytorch_tabular-1.0.2/tests/test_ssl.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,30 +35,30 @@
 @pytest.mark.parametrize("target_range", [False])
 @pytest.mark.parametrize(
     "target_transform",
     [None],
 )
 @pytest.mark.parametrize(
     "custom_args",
-    [(None, None, None), ([fake_metric], torch.nn.L1Loss(), torch.optim.Adagrad)],
+    [(None, None, None, None), ([fake_metric], [False], torch.nn.L1Loss(), torch.optim.Adagrad)],
 )
 def test_regression(
     regression_data,
     multi_target,
     continuous_cols,
     categorical_cols,
     continuous_feature_transform,
     normalize_continuous_features,
     freeze_backbone,
     target_range,
     target_transform,
     custom_args,
 ):
     (train, test, target) = regression_data
-    (custom_metrics, custom_loss, custom_optimizer) = custom_args
+    (custom_metrics, metrics_prob_input, custom_loss, custom_optimizer) = custom_args
     ssl, finetune = train_test_split(train, random_state=42)
     ssl_train, ssl_val = train_test_split(ssl, random_state=42)
     finetune_train, finetune_val = train_test_split(finetune, random_state=42)
     if len(continuous_cols) + len(categorical_cols) == 0:
         assert True
     else:
         data_config = DataConfig(
@@ -77,18 +77,18 @@
         )
         decoder_config = CategoryEmbeddingModelConfig(
             task="backbone",
             layers="512-2048-4096",  # Number of nodes in each layer
             activation="LeakyReLU",  # Activation between each layers
         )
 
-        model_config_params = dict(
-            encoder_config=encoder_config,
-            decoder_config=decoder_config,
-        )
+        model_config_params = {
+            "encoder_config": encoder_config,
+            "decoder_config": decoder_config,
+        }
         model_config = DenoisingAutoEncoderConfig(**model_config_params)
         trainer_config = TrainerConfig(
             max_epochs=1,
             checkpoints=None,
             early_stopping=None,
             accelerator="cpu",
             fast_dev_run=True,
@@ -122,14 +122,15 @@
             },
             trainer_config=trainer_config,
             optimizer_config=optimizer_config,
             target_range=_target_range,
             loss=custom_loss,
             metrics=custom_metrics,
             metrics_params=[{}],
+            metrics_prob_input=metrics_prob_input,
             optimizer=custom_optimizer,
         )
         finetune_model.finetune(
             train=finetune_train,
             validation=finetune_val,
             freeze_backbone=freeze_backbone,
             target_transform=target_transform,
@@ -183,18 +184,18 @@
             activation="LeakyReLU",  # Activation between each layers
         )
         decoder_config = CategoryEmbeddingModelConfig(
             task="backbone",
             layers="512-2048-4096",  # Number of nodes in each layer
             activation="LeakyReLU",  # Activation between each layers
         )
-        model_config_params = dict(
-            encoder_config=encoder_config,
-            decoder_config=decoder_config,
-        )
+        model_config_params = {
+            "encoder_config": encoder_config,
+            "decoder_config": decoder_config,
+        }
         model_config = DenoisingAutoEncoderConfig(**model_config_params)
         trainer_config = TrainerConfig(
             max_epochs=1,
             checkpoints=None,
             early_stopping=None,
             accelerator="cpu",
             fast_dev_run=True,
```

### Comparing `pytorch_tabular-1.0.1/tests/test_tabnet.py` & `pytorch_tabular-1.0.2/tests/test_tabnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         data_config = DataConfig(
             target=target + ["MedInc"] if multi_target else target,
             continuous_cols=continuous_cols,
             categorical_cols=categorical_cols,
             continuous_feature_transform=continuous_feature_transform,
             normalize_continuous_features=normalize_continuous_features,
         )
-        model_config_params = dict(task="regression")
+        model_config_params = {"task": "regression"}
         if target_range:
             _target_range = []
             for target in data_config.target:
                 _target_range.append(
                     (
                         float(train[target].min()),
                         float(train[target].max()),
@@ -78,17 +78,15 @@
         assert "test_mean_squared_error" in result[0].keys()
         pred_df = tabular_model.predict(test)
         assert pred_df.shape[0] == test.shape[0]
 
 
 @pytest.mark.parametrize(
     "continuous_cols",
-    [
-        [f"feature_{i}" for i in range(54)],
-    ],
+    [[f"feature_{i}" for i in range(54)]],
 )
 @pytest.mark.parametrize("categorical_cols", [["feature_0_cat"]])
 @pytest.mark.parametrize("continuous_feature_transform", [None])
 @pytest.mark.parametrize("normalize_continuous_features", [True])
 def test_classification(
     classification_data,
     continuous_cols,
@@ -103,15 +101,15 @@
         data_config = DataConfig(
             target=target,
             continuous_cols=continuous_cols,
             categorical_cols=categorical_cols,
             continuous_feature_transform=continuous_feature_transform,
             normalize_continuous_features=normalize_continuous_features,
         )
-        model_config_params = dict(task="classification")
+        model_config_params = {"task": "classification"}
         model_config = TabNetModelConfig(**model_config_params)
         trainer_config = TrainerConfig(
             max_epochs=1,
             checkpoints=None,
             early_stopping=None,
             accelerator="cpu",
             fast_dev_run=True,
```

### Comparing `pytorch_tabular-1.0.1/tests/test_tabtransformer.py` & `pytorch_tabular-1.0.2/tests/test_ft_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 """Tests for `pytorch_tabular` package."""
 import pytest
 
 from pytorch_tabular import TabularModel
 from pytorch_tabular.categorical_encoders import CategoricalEmbeddingTransformer
 from pytorch_tabular.config import DataConfig, OptimizerConfig, TrainerConfig
-from pytorch_tabular.models import TabTransformerConfig
+from pytorch_tabular.models import FTTransformerConfig
 
 
 @pytest.mark.parametrize("multi_target", [True, False])
 @pytest.mark.parametrize(
     "continuous_cols",
     [
         [
@@ -18,15 +18,15 @@
             "Population",
             "AveOccup",
             "Latitude",
             "Longitude",
         ],
     ],
 )
-@pytest.mark.parametrize("categorical_cols", [["HouseAgeBin"]])
+@pytest.mark.parametrize("categorical_cols", [["HouseAgeBin"], []])
 @pytest.mark.parametrize("continuous_feature_transform", [None])
 @pytest.mark.parametrize("normalize_continuous_features", [True])
 @pytest.mark.parametrize("target_range", [True, False])
 def test_regression(
     regression_data,
     multi_target,
     continuous_cols,
@@ -42,31 +42,31 @@
         data_config = DataConfig(
             target=target + ["MedInc"] if multi_target else target,
             continuous_cols=continuous_cols,
             categorical_cols=categorical_cols,
             continuous_feature_transform=continuous_feature_transform,
             normalize_continuous_features=normalize_continuous_features,
         )
-        model_config_params = dict(
-            task="regression",
-            input_embed_dim=8,
-            num_attn_blocks=1,
-            num_heads=2,
-        )
+        model_config_params = {
+            "task": "regression",
+            "input_embed_dim": 8,
+            "num_attn_blocks": 1,
+            "num_heads": 2,
+        }
         if target_range:
             _target_range = []
             for target in data_config.target:
                 _target_range.append(
                     (
                         float(train[target].min()),
                         float(train[target].max()),
                     )
                 )
             model_config_params["target_range"] = _target_range
-        model_config = TabTransformerConfig(**model_config_params)
+        model_config = FTTransformerConfig(**model_config_params)
         trainer_config = TrainerConfig(
             max_epochs=1,
             checkpoints=None,
             early_stopping=None,
             accelerator="cpu",
             fast_dev_run=True,
         )
@@ -109,21 +109,21 @@
         data_config = DataConfig(
             target=target,
             continuous_cols=continuous_cols,
             categorical_cols=categorical_cols,
             continuous_feature_transform=continuous_feature_transform,
             normalize_continuous_features=normalize_continuous_features,
         )
-        model_config_params = dict(
-            task="classification",
-            input_embed_dim=8,
-            num_attn_blocks=1,
-            num_heads=2,
-        )
-        model_config = TabTransformerConfig(**model_config_params)
+        model_config_params = {
+            "task": "classification",
+            "input_embed_dim": 8,
+            "num_attn_blocks": 1,
+            "num_heads": 2,
+        }
+        model_config = FTTransformerConfig(**model_config_params)
         trainer_config = TrainerConfig(
             max_epochs=1,
             checkpoints=None,
             early_stopping=None,
             accelerator="cpu",
             fast_dev_run=True,
         )
@@ -153,21 +153,21 @@
             "Population",
             "AveOccup",
             "Latitude",
             "Longitude",
         ],
         categorical_cols=["HouseAgeBin"],
     )
-    model_config_params = dict(
-        task="regression",
-        input_embed_dim=8,
-        num_attn_blocks=1,
-        num_heads=2,
-    )
-    model_config = TabTransformerConfig(**model_config_params)
+    model_config_params = {
+        "task": "regression",
+        "input_embed_dim": 8,
+        "num_attn_blocks": 1,
+        "num_heads": 2,
+    }
+    model_config = FTTransformerConfig(**model_config_params)
     trainer_config = TrainerConfig(
         max_epochs=1,
         checkpoints=None,
         early_stopping=None,
         accelerator="cpu",
         fast_dev_run=True,
     )
@@ -181,8 +181,8 @@
     )
     tabular_model.fit(train=train, test=test)
 
     transformer = CategoricalEmbeddingTransformer(tabular_model)
     train_transform = transformer.fit_transform(train)
     embed_cols = [col for col in train_transform.columns if "HouseAgeBin_embed_dim" in col]
     assert len(train["HouseAgeBin"].unique()) + 1 == len(transformer._mapping["HouseAgeBin"].keys())
-    assert all([val.shape[0] == len(embed_cols) for val in transformer._mapping["HouseAgeBin"].values()])
+    assert all(val.shape[0] == len(embed_cols) for val in transformer._mapping["HouseAgeBin"].values())
```

