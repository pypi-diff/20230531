# Comparing `tmp/numpyro-0.9.1.tar.gz` & `tmp/numpyro-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpyro-0.9.1.tar", last modified: Mon Feb 28 14:03:59 2022, max compression
+gzip compressed data, was "numpyro-0.9.2.tar", last modified: Thu Apr 14 00:09:47 2022, max compression
```

## Comparing `numpyro-0.9.1.tar` & `numpyro-0.9.2.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-02-28 14:03:59.200101 numpyro-0.9.1/
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    11358 2021-08-04 16:19:08.000000 numpyro-0.9.1/LICENSE.md
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    26602 2022-02-28 14:03:59.200268 numpyro-0.9.1/PKG-INFO
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    25637 2022-02-03 01:44:41.000000 numpyro-0.9.1/README.md
-drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-02-28 14:03:59.147270 numpyro-0.9.1/numpyro/
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     1353 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/__init__.py
-drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-02-28 14:03:59.153467 numpyro-0.9.1/numpyro/compat/
--rw-r--r--   0 phandu   (884847) primarygroup (89939)        0 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/compat/__init__.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)      141 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/compat/distributions.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)      136 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/compat/handlers.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     5148 2022-02-28 14:03:00.000000 numpyro-0.9.1/numpyro/compat/infer.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     1207 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/compat/ops.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)      756 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/compat/optim.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     1269 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/compat/pyro.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)      358 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/compat/util.py
-drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-02-28 14:03:59.155819 numpyro-0.9.1/numpyro/contrib/
--rw-r--r--   0 phandu   (884847) primarygroup (89939)        0 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/contrib/__init__.py
-drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-02-28 14:03:59.163378 numpyro-0.9.1/numpyro/contrib/control_flow/
--rw-r--r--   0 phandu   (884847) primarygroup (89939)      215 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/contrib/control_flow/__init__.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     5757 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/contrib/control_flow/cond.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    18705 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/contrib/control_flow/scan.py
-drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-02-28 14:03:59.166109 numpyro-0.9.1/numpyro/contrib/einstein/
--rw-r--r--   0 phandu   (884847) primarygroup (89939)      561 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/contrib/einstein/__init__.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    16605 2022-02-05 06:34:54.000000 numpyro-0.9.1/numpyro/contrib/einstein/kernels.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    18388 2022-02-28 14:03:00.000000 numpyro-0.9.1/numpyro/contrib/einstein/steinvi.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     3482 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/contrib/einstein/util.py
-drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-02-28 14:03:59.168243 numpyro-0.9.1/numpyro/contrib/funsor/
--rw-r--r--   0 phandu   (884847) primarygroup (89939)      991 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/contrib/funsor/__init__.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     6848 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/contrib/funsor/discrete.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    25507 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/contrib/funsor/enum_messenger.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     9920 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/contrib/funsor/infer_util.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    18111 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/contrib/module.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    13104 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/contrib/nested_sampling.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    10740 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/contrib/render.py
-drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-02-28 14:03:59.169772 numpyro-0.9.1/numpyro/contrib/tfp/
--rw-r--r--   0 phandu   (884847) primarygroup (89939)      363 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/contrib/tfp/__init__.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    10853 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/contrib/tfp/distributions.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     9698 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/contrib/tfp/mcmc.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    11225 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/diagnostics.py
-drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-02-28 14:03:59.178096 numpyro-0.9.1/numpyro/distributions/
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     3967 2022-02-28 14:03:00.000000 numpyro-0.9.1/numpyro/distributions/__init__.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    10705 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/distributions/conjugate.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    16660 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/distributions/constraints.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    71711 2022-02-28 14:03:00.000000 numpyro-0.9.1/numpyro/distributions/continuous.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    25292 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/distributions/directional.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    31202 2022-02-28 14:03:00.000000 numpyro-0.9.1/numpyro/distributions/discrete.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    43574 2022-02-28 14:03:00.000000 numpyro-0.9.1/numpyro/distributions/distribution.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     4597 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/distributions/flows.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    12932 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/distributions/gof.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     7096 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/distributions/kl.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     8387 2021-09-10 15:52:28.000000 numpyro-0.9.1/numpyro/distributions/mixtures.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    38303 2022-02-28 14:03:00.000000 numpyro-0.9.1/numpyro/distributions/transforms.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    16340 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/distributions/truncated.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    21027 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/distributions/util.py
-drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-02-28 14:03:59.179229 numpyro-0.9.1/numpyro/examples/
--rw-r--r--   0 phandu   (884847) primarygroup (89939)        0 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/examples/__init__.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    11293 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/examples/datasets.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    31395 2022-02-28 14:03:00.000000 numpyro-0.9.1/numpyro/handlers.py
-drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-02-28 14:03:59.187709 numpyro-0.9.1/numpyro/infer/
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     1184 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/infer/__init__.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    50079 2022-02-28 14:03:00.000000 numpyro-0.9.1/numpyro/infer/autoguide.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    10814 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/infer/barker.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    25693 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/infer/elbo.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    40234 2022-02-05 06:34:54.000000 numpyro-0.9.1/numpyro/infer/hmc.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    39633 2022-02-28 14:03:00.000000 numpyro-0.9.1/numpyro/infer/hmc_gibbs.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    50036 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/infer/hmc_util.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     3769 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/infer/initialization.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     9482 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/infer/inspect.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    29282 2022-02-28 14:03:00.000000 numpyro-0.9.1/numpyro/infer/mcmc.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    13401 2021-11-10 15:03:49.000000 numpyro-0.9.1/numpyro/infer/mixed_hmc.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    11889 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/infer/reparam.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    15870 2022-02-05 06:34:54.000000 numpyro-0.9.1/numpyro/infer/sa.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    15991 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/infer/svi.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    43600 2022-02-28 14:03:00.000000 numpyro-0.9.1/numpyro/infer/util.py
-drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-02-28 14:03:59.190531 numpyro-0.9.1/numpyro/nn/
--rw-r--r--   0 phandu   (884847) primarygroup (89939)      346 2021-08-04 16:19:08.000000 numpyro-0.9.1/numpyro/nn/__init__.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     7217 2021-12-08 21:15:17.000000 numpyro-0.9.1/numpyro/nn/auto_reg_nn.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     6926 2021-12-08 21:15:17.000000 numpyro-0.9.1/numpyro/nn/block_neural_arn.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     1457 2021-12-08 21:15:17.000000 numpyro-0.9.1/numpyro/nn/masked_dense.py
-drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-02-28 14:03:59.192031 numpyro-0.9.1/numpyro/ops/
--rw-r--r--   0 phandu   (884847) primarygroup (89939)        0 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/ops/__init__.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     5446 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/ops/indexing.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     4683 2022-02-05 06:34:54.000000 numpyro-0.9.1/numpyro/ops/provenance.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     2206 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/ops/pytree.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    11123 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/optim.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)      622 2021-12-09 02:17:52.000000 numpyro-0.9.1/numpyro/patch.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    24940 2022-02-28 14:03:00.000000 numpyro-0.9.1/numpyro/primitives.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    25969 2022-02-03 01:44:41.000000 numpyro-0.9.1/numpyro/util.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)      107 2022-02-28 14:03:00.000000 numpyro-0.9.1/numpyro/version.py
-drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-02-28 14:03:59.149121 numpyro-0.9.1/numpyro.egg-info/
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    26602 2022-02-28 14:03:59.000000 numpyro-0.9.1/numpyro.egg-info/PKG-INFO
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     2605 2022-02-28 14:03:59.000000 numpyro-0.9.1/numpyro.egg-info/SOURCES.txt
--rw-r--r--   0 phandu   (884847) primarygroup (89939)        1 2022-02-28 14:03:59.000000 numpyro-0.9.1/numpyro.egg-info/dependency_links.txt
--rw-r--r--   0 phandu   (884847) primarygroup (89939)      501 2022-02-28 14:03:59.000000 numpyro-0.9.1/numpyro.egg-info/requires.txt
--rw-r--r--   0 phandu   (884847) primarygroup (89939)        8 2022-02-28 14:03:59.000000 numpyro-0.9.1/numpyro.egg-info/top_level.txt
--rw-r--r--   0 phandu   (884847) primarygroup (89939)      966 2022-02-28 14:03:59.200930 numpyro-0.9.1/setup.cfg
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     3168 2022-02-05 06:34:54.000000 numpyro-0.9.1/setup.py
-drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-02-28 14:03:59.199783 numpyro-0.9.1/test/
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     2259 2021-11-10 15:03:49.000000 numpyro-0.9.1/test/test_compile.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     2765 2021-12-09 02:35:01.000000 numpyro-0.9.1/test/test_diagnostics.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    90427 2022-02-28 14:03:00.000000 numpyro-0.9.1/test/test_distributions.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     5107 2021-09-10 15:52:28.000000 numpyro-0.9.1/test/test_distributions_mixture.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     5679 2022-02-03 01:44:41.000000 numpyro-0.9.1/test/test_distributions_util.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     1440 2021-08-04 16:19:08.000000 numpyro-0.9.1/test/test_example_utils.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     3398 2022-02-28 14:03:00.000000 numpyro-0.9.1/test/test_examples.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     3411 2021-12-08 21:15:17.000000 numpyro-0.9.1/test/test_flows.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)    27277 2022-02-03 01:44:41.000000 numpyro-0.9.1/test/test_handlers.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     4282 2022-02-03 01:44:41.000000 numpyro-0.9.1/test/test_model_rendering.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     6456 2021-12-08 21:15:17.000000 numpyro-0.9.1/test/test_nn.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     3197 2022-02-03 01:44:41.000000 numpyro-0.9.1/test/test_optimizers.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     2776 2021-11-10 15:03:49.000000 numpyro-0.9.1/test/test_pickle.py
--rw-r--r--   0 phandu   (884847) primarygroup (89939)     8638 2022-02-03 01:44:41.000000 numpyro-0.9.1/test/test_util.py
+drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-04-14 00:09:47.472130 numpyro-0.9.2/
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    11358 2021-08-04 16:19:08.000000 numpyro-0.9.2/LICENSE.md
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    26602 2022-04-14 00:09:47.472339 numpyro-0.9.2/PKG-INFO
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    25637 2022-02-03 01:44:41.000000 numpyro-0.9.2/README.md
+drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-04-14 00:09:47.417335 numpyro-0.9.2/numpyro/
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     1353 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/__init__.py
+drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-04-14 00:09:47.423129 numpyro-0.9.2/numpyro/compat/
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)        0 2021-08-04 16:19:08.000000 numpyro-0.9.2/numpyro/compat/__init__.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)      141 2021-08-04 16:19:08.000000 numpyro-0.9.2/numpyro/compat/distributions.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)      136 2021-08-04 16:19:08.000000 numpyro-0.9.2/numpyro/compat/handlers.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     5148 2022-02-28 14:03:00.000000 numpyro-0.9.2/numpyro/compat/infer.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     1207 2021-08-04 16:19:08.000000 numpyro-0.9.2/numpyro/compat/ops.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)      756 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/compat/optim.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     1269 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/compat/pyro.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)      358 2021-08-04 16:19:08.000000 numpyro-0.9.2/numpyro/compat/util.py
+drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-04-14 00:09:47.425456 numpyro-0.9.2/numpyro/contrib/
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)        0 2021-08-04 16:19:08.000000 numpyro-0.9.2/numpyro/contrib/__init__.py
+drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-04-14 00:09:47.427103 numpyro-0.9.2/numpyro/contrib/control_flow/
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)      215 2021-08-04 16:19:08.000000 numpyro-0.9.2/numpyro/contrib/control_flow/__init__.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     5757 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/contrib/control_flow/cond.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    18684 2022-04-13 23:59:53.000000 numpyro-0.9.2/numpyro/contrib/control_flow/scan.py
+drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-04-14 00:09:47.429678 numpyro-0.9.2/numpyro/contrib/einstein/
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)      561 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/contrib/einstein/__init__.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    16605 2022-02-05 06:34:54.000000 numpyro-0.9.2/numpyro/contrib/einstein/kernels.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    18375 2022-04-10 00:36:28.000000 numpyro-0.9.2/numpyro/contrib/einstein/steinvi.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     3462 2022-04-10 00:36:28.000000 numpyro-0.9.2/numpyro/contrib/einstein/util.py
+drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-04-14 00:09:47.431928 numpyro-0.9.2/numpyro/contrib/funsor/
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)      991 2021-08-04 16:19:08.000000 numpyro-0.9.2/numpyro/contrib/funsor/__init__.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     6848 2021-08-04 16:19:08.000000 numpyro-0.9.2/numpyro/contrib/funsor/discrete.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    25507 2021-08-04 16:19:08.000000 numpyro-0.9.2/numpyro/contrib/funsor/enum_messenger.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     9920 2021-08-04 16:19:08.000000 numpyro-0.9.2/numpyro/contrib/funsor/infer_util.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    18111 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/contrib/module.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    12388 2022-04-13 10:41:24.000000 numpyro-0.9.2/numpyro/contrib/nested_sampling.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    13169 2022-04-10 00:34:48.000000 numpyro-0.9.2/numpyro/contrib/render.py
+drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-04-14 00:09:47.435626 numpyro-0.9.2/numpyro/contrib/tfp/
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)      363 2021-08-04 16:19:08.000000 numpyro-0.9.2/numpyro/contrib/tfp/__init__.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    10853 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/contrib/tfp/distributions.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     9698 2021-08-04 16:19:08.000000 numpyro-0.9.2/numpyro/contrib/tfp/mcmc.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    11225 2021-08-04 16:19:08.000000 numpyro-0.9.2/numpyro/diagnostics.py
+drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-04-14 00:09:47.445774 numpyro-0.9.2/numpyro/distributions/
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     3967 2022-03-14 01:40:38.000000 numpyro-0.9.2/numpyro/distributions/__init__.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    10726 2022-03-14 01:40:50.000000 numpyro-0.9.2/numpyro/distributions/conjugate.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    18095 2022-04-13 10:32:37.000000 numpyro-0.9.2/numpyro/distributions/constraints.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    70992 2022-04-10 00:36:28.000000 numpyro-0.9.2/numpyro/distributions/continuous.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    25882 2022-04-10 00:34:48.000000 numpyro-0.9.2/numpyro/distributions/directional.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    31286 2022-04-13 10:41:24.000000 numpyro-0.9.2/numpyro/distributions/discrete.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    43706 2022-04-13 10:41:24.000000 numpyro-0.9.2/numpyro/distributions/distribution.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     4597 2021-08-04 16:19:08.000000 numpyro-0.9.2/numpyro/distributions/flows.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    12932 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/distributions/gof.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     7096 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/distributions/kl.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     8404 2022-03-14 01:40:50.000000 numpyro-0.9.2/numpyro/distributions/mixtures.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    38303 2022-03-14 01:40:38.000000 numpyro-0.9.2/numpyro/distributions/transforms.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    16355 2022-03-14 01:40:50.000000 numpyro-0.9.2/numpyro/distributions/truncated.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    21027 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/distributions/util.py
+drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-04-14 00:09:47.447105 numpyro-0.9.2/numpyro/examples/
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)        0 2021-08-04 16:19:08.000000 numpyro-0.9.2/numpyro/examples/__init__.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    12519 2022-04-13 10:41:24.000000 numpyro-0.9.2/numpyro/examples/datasets.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    31633 2022-04-13 23:59:53.000000 numpyro-0.9.2/numpyro/handlers.py
+drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-04-14 00:09:47.457342 numpyro-0.9.2/numpyro/infer/
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     1184 2021-08-04 16:19:08.000000 numpyro-0.9.2/numpyro/infer/__init__.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    50079 2022-03-14 01:40:38.000000 numpyro-0.9.2/numpyro/infer/autoguide.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    10814 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/infer/barker.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    25693 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/infer/elbo.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    40727 2022-04-10 00:34:48.000000 numpyro-0.9.2/numpyro/infer/hmc.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    39633 2022-03-14 01:40:38.000000 numpyro-0.9.2/numpyro/infer/hmc_gibbs.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    49991 2022-04-10 00:36:28.000000 numpyro-0.9.2/numpyro/infer/hmc_util.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     3769 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/infer/initialization.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     9482 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/infer/inspect.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    29069 2022-04-10 00:36:28.000000 numpyro-0.9.2/numpyro/infer/mcmc.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    13401 2021-11-10 15:03:49.000000 numpyro-0.9.2/numpyro/infer/mixed_hmc.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    12470 2022-04-13 23:59:53.000000 numpyro-0.9.2/numpyro/infer/reparam.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    15870 2022-02-05 06:34:54.000000 numpyro-0.9.2/numpyro/infer/sa.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    15991 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/infer/svi.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    43600 2022-02-28 14:03:00.000000 numpyro-0.9.2/numpyro/infer/util.py
+drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-04-14 00:09:47.460437 numpyro-0.9.2/numpyro/nn/
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)      346 2021-08-04 16:19:08.000000 numpyro-0.9.2/numpyro/nn/__init__.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     7217 2021-12-08 21:15:17.000000 numpyro-0.9.2/numpyro/nn/auto_reg_nn.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     6926 2021-12-08 21:15:17.000000 numpyro-0.9.2/numpyro/nn/block_neural_arn.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     1457 2021-12-08 21:15:17.000000 numpyro-0.9.2/numpyro/nn/masked_dense.py
+drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-04-14 00:09:47.462168 numpyro-0.9.2/numpyro/ops/
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)        0 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/ops/__init__.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     5446 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/ops/indexing.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     4723 2022-04-10 00:34:48.000000 numpyro-0.9.2/numpyro/ops/provenance.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     2215 2022-04-10 00:34:48.000000 numpyro-0.9.2/numpyro/ops/pytree.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    11123 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/optim.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)      622 2021-12-09 02:17:52.000000 numpyro-0.9.2/numpyro/patch.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    24970 2022-03-14 01:40:50.000000 numpyro-0.9.2/numpyro/primitives.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    25969 2022-02-03 01:44:41.000000 numpyro-0.9.2/numpyro/util.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)      107 2022-04-13 23:59:53.000000 numpyro-0.9.2/numpyro/version.py
+drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-04-14 00:09:47.418925 numpyro-0.9.2/numpyro.egg-info/
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    26602 2022-04-14 00:09:47.000000 numpyro-0.9.2/numpyro.egg-info/PKG-INFO
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     2605 2022-04-14 00:09:47.000000 numpyro-0.9.2/numpyro.egg-info/SOURCES.txt
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)        1 2022-04-14 00:09:47.000000 numpyro-0.9.2/numpyro.egg-info/dependency_links.txt
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)      501 2022-04-14 00:09:47.000000 numpyro-0.9.2/numpyro.egg-info/requires.txt
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)        8 2022-04-14 00:09:47.000000 numpyro-0.9.2/numpyro.egg-info/top_level.txt
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)      966 2022-04-14 00:09:47.472914 numpyro-0.9.2/setup.cfg
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     3168 2022-04-13 10:41:24.000000 numpyro-0.9.2/setup.py
+drwxr-xr-x   0 phandu   (884847) primarygroup (89939)        0 2022-04-14 00:09:47.471542 numpyro-0.9.2/test/
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     2259 2021-11-10 15:03:49.000000 numpyro-0.9.2/test/test_compile.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     2765 2021-12-09 02:35:01.000000 numpyro-0.9.2/test/test_diagnostics.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    91029 2022-04-10 00:36:42.000000 numpyro-0.9.2/test/test_distributions.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     5107 2021-09-10 15:52:28.000000 numpyro-0.9.2/test/test_distributions_mixture.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     5679 2022-02-03 01:44:41.000000 numpyro-0.9.2/test/test_distributions_util.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     1440 2021-08-04 16:19:08.000000 numpyro-0.9.2/test/test_example_utils.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     3466 2022-04-13 10:41:24.000000 numpyro-0.9.2/test/test_examples.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     3411 2021-12-08 21:15:17.000000 numpyro-0.9.2/test/test_flows.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)    27352 2022-04-13 23:59:53.000000 numpyro-0.9.2/test/test_handlers.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     4282 2022-02-03 01:44:41.000000 numpyro-0.9.2/test/test_model_rendering.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     6456 2021-12-08 21:15:17.000000 numpyro-0.9.2/test/test_nn.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     3333 2022-04-10 00:36:28.000000 numpyro-0.9.2/test/test_optimizers.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     2776 2021-11-10 15:03:49.000000 numpyro-0.9.2/test/test_pickle.py
+-rw-r--r--   0 phandu   (884847) primarygroup (89939)     8623 2022-04-10 00:36:28.000000 numpyro-0.9.2/test/test_util.py
```

### Comparing `numpyro-0.9.1/LICENSE.md` & `numpyro-0.9.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/PKG-INFO` & `numpyro-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numpyro
-Version: 0.9.1
+Version: 0.9.2
 Summary: Pyro PPL on NumPy
 Home-page: https://github.com/pyro-ppl/numpyro
 Author: Uber AI Labs
 License: Apache License 2.0
 Keywords: probabilistic machine learning bayesian statistics
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `numpyro-0.9.1/README.md` & `numpyro-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/__init__.py` & `numpyro-0.9.2/numpyro/__init__.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/compat/infer.py` & `numpyro-0.9.2/numpyro/compat/infer.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/compat/ops.py` & `numpyro-0.9.2/numpyro/compat/ops.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/compat/optim.py` & `numpyro-0.9.2/numpyro/compat/optim.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/compat/pyro.py` & `numpyro-0.9.2/numpyro/compat/pyro.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/contrib/control_flow/cond.py` & `numpyro-0.9.2/numpyro/contrib/control_flow/cond.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/contrib/control_flow/scan.py` & `numpyro-0.9.2/numpyro/contrib/control_flow/scan.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 # Copyright Contributors to the Pyro project.
 # SPDX-License-Identifier: Apache-2.0
 
 from collections import OrderedDict
 from functools import partial
 
-from jax import (
-    device_put,
-    lax,
-    random,
-    tree_flatten,
-    tree_map,
-    tree_multimap,
-    tree_unflatten,
-)
+from jax import device_put, lax, random, tree_flatten, tree_map, tree_unflatten
 import jax.numpy as jnp
 
 from numpyro import handlers
 from numpyro.ops.pytree import PytreeTrace
 from numpyro.primitives import _PYRO_STACK, Messenger, apply_stack
 from numpyro.util import not_jax_tracer
 
@@ -149,15 +141,17 @@
             if subs_type == "condition":
                 seeded_fn = handlers.condition(seeded_fn, condition_fn=subs_fn)
             elif subs_type == "substitute":
                 seeded_fn = handlers.substitute(seeded_fn, substitute_fn=subs_fn)
 
         if init:
             # handler the name to match the pattern of sakkar_bilmes product
-            with handlers.scope(prefix="_PREV_" * (unroll_steps - i), divider=""):
+            with handlers.scope(
+                prefix="_PREV_" * (unroll_steps - i), divider="", hide_types=["plate"]
+            ):
                 new_carry, y = config_enumerate(seeded_fn)(carry, x)
                 trace = {}
         else:
             # Like scan_wrapper, we collect the trace of scan's transition function
             # `seeded_fn` here. To put time dimension to the correct position, we need to
             # promote shapes to make `fn` and `value`
             # at each site have the same batch dims (e.g. if `fn.batch_shape = (2, 3)`,
@@ -170,15 +164,15 @@
                 new_carry, y = config_enumerate(seeded_fn)(carry, x)
 
             # store shape of new_carry at a global variable
             if len(carry_shapes) < (history + 1):
                 carry_shapes.append([jnp.shape(x) for x in tree_flatten(new_carry)[0]])
             # make new_carry have the same shape as carry
             # FIXME: is this rigorous?
-            new_carry = tree_multimap(
+            new_carry = tree_map(
                 lambda a, b: jnp.reshape(a, jnp.shape(b)), new_carry, carry
             )
         return (i + 1, rng_key, new_carry), (PytreeTrace(trace), y)
 
     with handlers.block(
         hide_fn=lambda site: not site["name"].startswith("_PREV_")
     ), enum(first_available_dim=first_available_dim):
@@ -188,27 +182,27 @@
         for i in markov(range(unroll_steps + 1), history=history):
             if i < unroll_steps:
                 wrapped_carry, (_, y0) = body_fn(
                     wrapped_carry, tree_map(lambda z: z[i], x0)
                 )
                 if i > 0:
                     # reshape y1, y2,... to have the same shape as y0
-                    y0 = tree_multimap(
+                    y0 = tree_map(
                         lambda z0, z: jnp.reshape(z, jnp.shape(z0)), y0s[0], y0
                     )
                 y0s.append(y0)
                 # shapes of the first `history - 1` steps are not useful to interpret the last carry
                 # shape so we don't need to record them here
                 if (i >= history - 1) and (len(carry_shapes) < history + 1):
                     carry_shapes.append(
                         jnp.shape(x) for x in tree_flatten(wrapped_carry[-1])[0]
                     )
             else:
                 # this is the last rolling step
-                y0s = tree_multimap(lambda *z: jnp.stack(z, axis=0), *y0s)
+                y0s = tree_map(lambda *z: jnp.stack(z, axis=0), *y0s)
                 # return early if length = unroll_steps
                 if length == unroll_steps:
                     return wrapped_carry, (PytreeTrace({}), y0s)
                 wrapped_carry = device_put(wrapped_carry)
                 wrapped_carry, (pytree_trace, ys) = lax.scan(
                     body_fn, wrapped_carry, xs_, length - unroll_steps, reverse
                 )
@@ -230,19 +224,19 @@
         # we don't record 1-size dimensions in this field
         time_dim = -min(
             len(site["fn"].batch_shape), jnp.ndim(site["value"]) - site["fn"].event_dim
         )
         site["infer"]["dim_to_name"][time_dim] = "_time_{}".format(first_var)
 
     # similar to carry, we need to reshape due to shape alternating in markov
-    ys = tree_multimap(
+    ys = tree_map(
         lambda z0, z: jnp.reshape(z, z.shape[:1] + jnp.shape(z0)[1:]), y0s, ys
     )
     # then join with y0s
-    ys = tree_multimap(lambda z0, z: jnp.concatenate([z0, z], axis=0), y0s, ys)
+    ys = tree_map(lambda z0, z: jnp.concatenate([z0, z], axis=0), y0s, ys)
     # we also need to reshape `carry` to match sequential behavior
     i = (length + 1) % (history + 1)
     t, rng_key, carry = wrapped_carry
     carry_shape = carry_shapes[i]
     flatten_carry, treedef = tree_flatten(carry)
     flatten_carry = [
         jnp.reshape(x, t1_shape) for x, t1_shape in zip(flatten_carry, carry_shape)
```

### Comparing `numpyro-0.9.1/numpyro/contrib/einstein/__init__.py` & `numpyro-0.9.2/numpyro/contrib/einstein/__init__.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/contrib/einstein/kernels.py` & `numpyro-0.9.2/numpyro/contrib/einstein/kernels.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/contrib/einstein/steinvi.py` & `numpyro-0.9.2/numpyro/contrib/einstein/steinvi.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,18 +268,18 @@
                 if jac is not None:
                     force = force @ jac.reshape(
                         (_numel(jac.shape[: len(jac.shape) // 2]), -1)
                     )
                 return force.reshape(attr_force.shape)
 
             reparam_jac = {
-                name: jax.tree_map(lambda var: _nontrivial_jac(name, var), variables)
+                name: tree_map(lambda var: _nontrivial_jac(name, var), variables)
                 for name, variables in unravel_pytree(particle).items()
             }
-            jac_params = jax.tree_multimap(
+            jac_params = tree_map(
                 _update_force,
                 unravel_pytree(attr_forces),
                 unravel_pytree(rep_forces),
                 reparam_jac,
             )
             jac_particle, _ = ravel_pytree(jac_params)
             return jac_particle
```

### Comparing `numpyro-0.9.1/numpyro/contrib/einstein/util.py` & `numpyro-0.9.2/numpyro/contrib/einstein/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright Contributors to the Pyro project.
 # SPDX-License-Identifier: Apache-2.0
 
 from jax import numpy as jnp, vmap
 from jax.flatten_util import ravel_pytree
-from jax.tree_util import tree_map, tree_multimap
+from jax.tree_util import tree_map
 
 from numpyro.distributions import biject_to
 from numpyro.distributions.constraints import real
 from numpyro.distributions.transforms import ComposeTransform, IdentityTransform
 
 
 def posdef(m):
@@ -78,11 +78,11 @@
     shapes = tree_map(lambda x: x.shape, pytree)
     flat_pytree = tree_map(lambda x: x.reshape(*x.shape[:-nbatch_dims], -1), pytree)
     flat = vmap(lambda x: ravel_pytree(x)[0])(flat_pytree)
     unravel_fn = ravel_pytree(tree_map(lambda x: x[0], flat_pytree))[1]
     return (
         flat,
         unravel_fn,
-        lambda _flat: tree_multimap(
+        lambda _flat: tree_map(
             lambda x, shape: x.reshape(shape), vmap(unravel_fn)(_flat), shapes
         ),
     )
```

### Comparing `numpyro-0.9.1/numpyro/contrib/funsor/__init__.py` & `numpyro-0.9.2/numpyro/contrib/funsor/__init__.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/contrib/funsor/discrete.py` & `numpyro-0.9.2/numpyro/contrib/funsor/discrete.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/contrib/funsor/enum_messenger.py` & `numpyro-0.9.2/numpyro/contrib/funsor/enum_messenger.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/contrib/funsor/infer_util.py` & `numpyro-0.9.2/numpyro/contrib/funsor/infer_util.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/contrib/module.py` & `numpyro-0.9.2/numpyro/contrib/module.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/contrib/nested_sampling.py` & `numpyro-0.9.2/numpyro/contrib/nested_sampling.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 # Copyright Contributors to the Pyro project.
 # SPDX-License-Identifier: Apache-2.0
 
 from functools import singledispatch
-import warnings
 
-from jax import config, nn, random, tree_util
+from jax import nn, random, tree_util
 import jax.numpy as jnp
 
 try:
-    # jaxns changes the default precision to double precision
-    # so here we undo that action
-    use_x64 = config.jax_enable_x64
-
-    from jaxns.nested_sampling import NestedSampler as OrigNestedSampler
-    from jaxns.plotting import plot_cornerplot, plot_diagnostics
-    from jaxns.prior_transforms.common import ContinuousPrior
-    from jaxns.prior_transforms.prior_chain import PriorChain, UniformBase
-    from jaxns.utils import summary
-
-    config.update("jax_enable_x64", use_x64)
+    from jaxns import (
+        NestedSampler as OrigNestedSampler,
+        plot_cornerplot,
+        plot_diagnostics,
+        summary,
+    )
+    from jaxns.prior_transforms import ContinuousPrior, PriorChain
+    from jaxns.prior_transforms.prior import UniformBase
 except ImportError as e:
     raise ImportError(
         "To use this module, please install `jaxns` package. It can be"
         " installed with `pip install jaxns`"
     ) from e
 
 import numpyro
@@ -118,14 +114,16 @@
             "{}_base".format(name),
             dist.Uniform(tiny, 1).expand(shape).to_event(event_dim).mask(False),
         )
         # Simulate a numpyro.deterministic() site.
         return None, transform(x)
 
 
+# TODO: Consider deprecating this wrapper. It might be better to only provide some
+# utilities to help converting a NumPyro model to a Jaxns loglikelihood function.
 class NestedSampler:
     """
     (EXPERIMENTAL) A wrapper for `jaxns <https://github.com/Joshuaalbert/jaxns>`_ ,
     a nested sampling package based on JAX.
 
     See reference [1] for details on the meaning of each parameter.
     Please consider citing this reference if you use the nested sampler in your research.
@@ -138,24 +136,18 @@
 
     **References**
 
     1. *JAXNS: a high-performance nested sampling package based on JAX*,
        Joshua G. Albert (https://arxiv.org/abs/2012.15286)
 
     :param callable model: a call with NumPyro primitives
-    :param int num_live_points: the number of live points. As a rule-of-thumb, we should
-        allocate around 50 live points per possible mode.
-    :param int max_samples: the maximum number of iterations and samples
-    :param str sampler_name: either "slice" (default value) or "multi_ellipsoid"
-    :param int depth: an integer which determines the maximum number of ellipsoids to
-        construct via hierarchical splitting (typical range: 3 - 9, default to 5)
-    :param int num_slices: the number of slice sampling proposals at each sampling step
-        (typical range: 1 - 5, default to 5)
-    :param float termination_frac: termination condition (typical range: 0.001 - 0.01)
-        (default to 0.01).
+    :param dict constructor_kwargs: additional keyword arguments to construct an upstream
+        :class:`jaxns.NestedSampler` instance.
+    :param dict termination_kwargs: keyword arguments to terminate the sampler. Please
+        refer to the upstream :meth:`jaxns.NestedSampler.__call__` method.
 
     **Example**
 
     .. doctest::
 
         >>> from jax import random
         >>> import jax.numpy as jnp
@@ -181,28 +173,24 @@
         [0.93661342 1.95034876 2.86123884]
     """
 
     def __init__(
         self,
         model,
         *,
-        num_live_points=1000,
-        max_samples=100000,
-        sampler_name="slice",
-        depth=5,
-        num_slices=5,
-        termination_frac=0.01
+        constructor_kwargs=None,
+        termination_kwargs=None,
     ):
         self.model = model
-        self.num_live_points = num_live_points
-        self.max_samples = max_samples
-        self.termination_frac = termination_frac
-        self.sampler_name = sampler_name
-        self.depth = depth
-        self.num_slices = num_slices
+        self.constructor_kwargs = (
+            constructor_kwargs if constructor_kwargs is not None else {}
+        )
+        self.termination_kwargs = (
+            termination_kwargs if termination_kwargs is not None else {}
+        )
         self._samples = None
         self._log_weights = None
         self._results = None
 
     def run(self, rng_key, *args, **kwargs):
         """
         Run the nested samplers and collect weighted samples.
@@ -241,45 +229,44 @@
 
             max_plate_nesting = _guess_max_plate_nesting(prototype_trace)
             _validate_model(prototype_trace)
             reparam_model = enum(reparam_model, -max_plate_nesting - 1)
         else:
             log_density_ = log_density
 
-        def loglik_fn(**params):
-            return log_density_(reparam_model, args, kwargs, params)[0]
+        # Jaxns requires loglikelihood function to have explicit signatures.
+        local_dict = {}
+        loglik_fn_def = """def loglik_fn({}):\n
+        \tparams = dict({})\n
+        \treturn log_density_(reparam_model, args, kwargs, params)[0]
+        """.format(
+            ", ".join([f"{name}_base" for name in param_names]),
+            ", ".join([f"{name}_base={name}_base" for name in param_names]),
+        )
+        exec(loglik_fn_def, locals(), local_dict)
+        loglik_fn = local_dict["loglik_fn"]
 
         # use NestedSampler with identity prior chain
         prior_chain = PriorChain()
         for name in param_names:
             prior = UniformPrior(name + "_base", prototype_trace[name]["fn"].shape())
             prior_chain.push(prior)
         # XXX: the `marginalised` keyword in jaxns can be used to get expectation of some
         # quantity over posterior samples; it can be helpful to expose it in this wrapper
         ns = OrigNestedSampler(
             loglik_fn,
             prior_chain,
-            sampler_name=self.sampler_name,
-            sampler_kwargs={"depth": self.depth, "num_slices": self.num_slices},
-            max_samples=self.max_samples,
-            num_live_points=self.num_live_points,
-            collect_samples=True,
+            **self.constructor_kwargs,
         )
-        # some places of jaxns uses float64 and raises some warnings if the default dtype is
-        # float32, so we suppress them here to avoid confusion
-        with warnings.catch_warnings():
-            warnings.filterwarnings(
-                "ignore", message=".*will be truncated to dtype float32.*"
-            )
-            results = ns(rng_sampling, termination_frac=self.termination_frac)
+        results = ns(rng_sampling, **self.termination_kwargs)
         # transform base samples back to original domains
         # Here we only transform the first valid num_samples samples
         # NB: the number of weighted samples obtained from jaxns is results.num_samples
         # and only the first num_samples values of results.samples are valid.
-        num_samples = results.num_samples
+        num_samples = results.total_num_samples
         samples = tree_util.tree_map(lambda x: x[:num_samples], results.samples)
         predictive = Predictive(
             reparam_model, samples, return_sites=param_names + deterministics
         )
         samples = predictive(rng_predictive, *args, **kwargs)
         # replace base samples in jaxns results by transformed samples
         self._results = results._replace(samples=samples)
@@ -307,16 +294,16 @@
         Gets weighted samples and their corresponding log weights.
         """
         if self._results is None:
             raise RuntimeError(
                 "NestedSampler.run(...) method should be called first to obtain results."
             )
 
-        num_samples = self._results.num_samples
-        return self._results.samples, self._results.log_p[:num_samples]
+        num_samples = self._results.total_num_samples
+        return self._results.samples, self._results.log_dp_mean[:num_samples]
 
     def print_summary(self):
         """
         Print summary of the result. This is a wrapper of :func:`jaxns.utils.summary`.
         """
         if self._results is None:
             raise RuntimeError(
```

### Comparing `numpyro-0.9.1/numpyro/contrib/render.py` & `numpyro-0.9.2/numpyro/contrib/render.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,16 +18,20 @@
     Infer relations of RVs and plates from given model and optionally data.
     See https://github.com/pyro-ppl/numpyro/issues/949 for more details.
 
     This returns a dictionary with keys:
 
     -  "sample_sample" map each downstream sample site to a list of the upstream
        sample sites on which it depend;
+    -  "sample_param" map each downstream sample site to a list of the upstream
+       param sites on which it depend;
     -  "sample_dist" maps each sample site to the name of the distribution at
        that site;
+    -  "param_constraint" maps each param site to the name of the constraints at
+       that site;
     -  "plate_sample" maps each plate name to a lists of the sample sites
        within that plate; and
     -  "observe" is a list of observed sample sites.
 
     For example for the model::
 
         def model(data):
@@ -125,50 +129,95 @@
             for name, site in tr.items()
             if site["type"] == "sample"
         }
 
     samples = {
         name: ProvenanceArray(site["value"], frozenset({name}))
         for name, site in trace.items()
-        if site["type"] == "sample" and not site["is_observed"]
+        if (site["type"] == "sample" and not site["is_observed"])
+    }
+
+    params = {
+        name: jax.tree_util.tree_map(
+            lambda x: ProvenanceArray(x, frozenset({name})), site["value"]
+        )
+        for name, site in trace.items()
+        if site["type"] == "param"
     }
-    sample_deps = get_provenance(eval_provenance(get_log_probs, samples))
+
+    sample_and_params = {**samples, **params}
+    sample_params_deps = get_provenance(
+        eval_provenance(get_log_probs, sample_and_params)
+    )
+
     sample_sample = {}
+    sample_param = {}
     for name in sample_dist:
         sample_sample[name] = [
-            var for var in sample_dist if var in sample_deps[name] and var != name
+            var
+            for var in sample_dist
+            if var in sample_params_deps[name] and var != name
         ]
+        sample_param[name] = [var for var in sample_params_deps[name] if var in params]
+
+    param_constraint = {}
+    for param in params:
+        if "constraint" in trace[param]["kwargs"]:
+            param_constraint[param] = str(trace[param]["kwargs"]["constraint"])
+        else:
+            param_constraint[param] = ""
+
     return {
         "sample_sample": sample_sample,
+        "sample_param": sample_param,
         "sample_dist": sample_dist,
+        "param_constraint": param_constraint,
         "plate_sample": plate_samples,
         "observed": obs_sites,
     }
 
 
-def generate_graph_specification(model_relations):
+def generate_graph_specification(model_relations, render_params=False):
     """
     Convert model relations into data structure which can be readily
     converted into a network.
+
+    :param bool render_params: Whether to add nodes of params.
     """
     # group nodes by plate
     plate_groups = dict(model_relations["plate_sample"])
     plate_rvs = {rv for rvs in plate_groups.values() for rv in rvs}
     plate_groups[None] = [
         rv for rv in model_relations["sample_sample"] if rv not in plate_rvs
     ]  # RVs which are in no plate
 
+    # get set of params
+    params = set()
+    if render_params:
+        for rv, params_list in model_relations["sample_param"].items():
+            for param in params_list:
+                params.add(param)
+        plate_groups[None].extend(params)
+
     # retain node metadata
     node_data = {}
     for rv in model_relations["sample_sample"]:
         node_data[rv] = {
             "is_observed": rv in model_relations["observed"],
             "distribution": model_relations["sample_dist"][rv],
         }
 
+    if render_params:
+        for param, constraint in model_relations["param_constraint"].items():
+            node_data[param] = {
+                "is_observed": False,
+                "constraint": constraint,
+                "distribution": None,
+            }
+
     # infer plate structure
     # (when the order of plates cannot be determined from subset relations,
     # it follows the order in which plates appear in trace)
     plate_data = {}
     for plate1, plate2 in list(itertools.combinations(plate_groups, 2)):
         if plate1 is None or plate2 is None:
             continue
@@ -186,14 +235,18 @@
             plate_data[plate] = {"parent": None}
 
     # infer RV edges
     edge_list = []
     for target, source_list in model_relations["sample_sample"].items():
         edge_list.extend([(source, target) for source in source_list])
 
+    if render_params:
+        for target, source_list in model_relations["sample_param"].items():
+            edge_list.extend([(source, target) for source in source_list])
+
     return {
         "plate_groups": plate_groups,
         "plate_data": plate_data,
         "node_data": node_data,
         "edge_list": edge_list,
     }
 
@@ -234,16 +287,29 @@
 
     # add nodes
     for plate, rv_list in plate_groups.items():
         cur_graph = plate_graph_dict[plate]
 
         for rv in rv_list:
             color = "grey" if node_data[rv]["is_observed"] else "white"
+
+            # For sample_nodes - ellipse
+            if node_data[rv]["distribution"]:
+                shape = "ellipse"
+                rv_label = rv
+
+            # For param_nodes - No shape
+            else:
+                shape = "plain"
+                rv_label = rv.replace(
+                    "$params", ""
+                )  # incase of neural network parameters
+
             cur_graph.node(
-                rv, label=rv, shape="ellipse", style="filled", fillcolor=color
+                rv, label=rv_label, shape=shape, style="filled", fillcolor=color
             )
 
     # add leaf nodes first
     while len(plate_data) >= 1:
         for plate, data in plate_data.items():
             parent_plate = data["parent"]
             is_leaf = True
@@ -258,54 +324,60 @@
                 plate_data.pop(plate)
                 break
 
     # add edges
     for source, target in edge_list:
         graph.edge(source, target)
 
-    # render distributions if requested
+    # render distributions and constraints if requested
     if render_distributions:
         dist_label = ""
         for rv, data in node_data.items():
             rv_dist = data["distribution"]
-            dist_label += rf"{rv} ~ {rv_dist}\l"
+            if rv_dist:
+                dist_label += rf"{rv} ~ {rv_dist}\l"
+
+            if "constraint" in data and data["constraint"]:
+                dist_label += rf"{rv} ∈ {data['constraint']}\l"
 
         graph.node("distribution_description_node", label=dist_label, shape="plaintext")
 
     # return whole graph
     return graph
 
 
 def render_model(
     model,
     model_args=None,
     model_kwargs=None,
     filename=None,
     render_distributions=False,
+    render_params=False,
 ):
     """
     Wrap all functions needed to automatically render a model.
 
     .. warning:: This utility does not support the
         :func:`~numpyro.contrib.control_flow.scan` primitive.
         If you want to render a time-series model, you can try
         to rewrite the code using Python for loop.
 
     :param model: Model to render.
     :param model_args: Positional arguments to pass to the model.
     :param model_kwargs: Keyword arguments to pass to the model.
     :param str filename: File to save rendered model in.
     :param bool render_distributions: Whether to include RV distribution annotations in the plot.
+    :param bool render_params: Whether to show params in the plot.
     """
     relations = get_model_relations(
         model,
         model_args=model_args,
         model_kwargs=model_kwargs,
     )
-    graph_spec = generate_graph_specification(relations)
+    graph_spec = generate_graph_specification(relations, render_params=render_params)
     graph = render_graph(graph_spec, render_distributions=render_distributions)
 
     if filename is not None:
         filename = Path(filename)
         graph.render(
             filename.stem, view=False, cleanup=True, format=filename.suffix[1:]
         )  # remove leading period from suffix
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `numpyro-0.9.1/numpyro/contrib/tfp/distributions.py` & `numpyro-0.9.2/numpyro/contrib/tfp/distributions.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/contrib/tfp/mcmc.py` & `numpyro-0.9.2/numpyro/contrib/tfp/mcmc.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/diagnostics.py` & `numpyro-0.9.2/numpyro/diagnostics.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/distributions/__init__.py` & `numpyro-0.9.2/numpyro/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/distributions/conjugate.py` & `numpyro-0.9.2/numpyro/distributions/conjugate.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         "concentration0": constraints.positive,
         "total_count": constraints.nonnegative_integer,
     }
     has_enumerate_support = True
     enumerate_support = BinomialProbs.enumerate_support
 
     def __init__(
-        self, concentration1, concentration0, total_count=1, validate_args=None
+        self, concentration1, concentration0, total_count=1, *, validate_args=None
     ):
         self.concentration1, self.concentration0, self.total_count = promote_shapes(
             concentration1, concentration0, total_count
         )
         batch_shape = lax.broadcast_shapes(
             jnp.shape(concentration1), jnp.shape(concentration0), jnp.shape(total_count)
         )
@@ -106,15 +106,15 @@
     :param numpy.ndarray total_count: number of Categorical trials.
     """
     arg_constraints = {
         "concentration": constraints.independent(constraints.positive, 1),
         "total_count": constraints.nonnegative_integer,
     }
 
-    def __init__(self, concentration, total_count=1, validate_args=None):
+    def __init__(self, concentration, total_count=1, *, validate_args=None):
         if jnp.ndim(concentration) < 1:
             raise ValueError(
                 "`concentration` parameter must be at least one-dimensional."
             )
 
         batch_shape = lax.broadcast_shapes(
             jnp.shape(concentration)[:-1], jnp.shape(total_count)
@@ -180,15 +180,15 @@
     """
     arg_constraints = {
         "concentration": constraints.positive,
         "rate": constraints.positive,
     }
     support = constraints.nonnegative_integer
 
-    def __init__(self, concentration, rate=1.0, validate_args=None):
+    def __init__(self, concentration, rate=1.0, *, validate_args=None):
         self.concentration, self.rate = promote_shapes(concentration, rate)
         self._gamma = Gamma(concentration, rate)
         super(GammaPoisson, self).__init__(
             self._gamma.batch_shape, validate_args=validate_args
         )
 
     def sample(self, key, sample_shape=()):
@@ -216,15 +216,15 @@
         return self.concentration / jnp.square(self.rate) * (1 + self.rate)
 
     def cdf(self, value):
         bt = betainc(self.concentration, value + 1.0, self.rate / (self.rate + 1.0))
         return bt
 
 
-def NegativeBinomial(total_count, probs=None, logits=None, validate_args=None):
+def NegativeBinomial(total_count, probs=None, logits=None, *, validate_args=None):
     if probs is not None:
         return NegativeBinomialProbs(total_count, probs, validate_args=validate_args)
     elif logits is not None:
         return NegativeBinomialLogits(total_count, logits, validate_args=validate_args)
     else:
         raise ValueError("One of `probs` or `logits` must be specified.")
 
@@ -232,29 +232,29 @@
 class NegativeBinomialProbs(GammaPoisson):
     arg_constraints = {
         "total_count": constraints.positive,
         "probs": constraints.unit_interval,
     }
     support = constraints.nonnegative_integer
 
-    def __init__(self, total_count, probs, validate_args=None):
+    def __init__(self, total_count, probs, *, validate_args=None):
         self.total_count, self.probs = promote_shapes(total_count, probs)
         concentration = total_count
         rate = 1.0 / probs - 1.0
         super().__init__(concentration, rate, validate_args=validate_args)
 
 
 class NegativeBinomialLogits(GammaPoisson):
     arg_constraints = {
         "total_count": constraints.positive,
         "logits": constraints.real,
     }
     support = constraints.nonnegative_integer
 
-    def __init__(self, total_count, logits, validate_args=None):
+    def __init__(self, total_count, logits, *, validate_args=None):
         self.total_count, self.logits = promote_shapes(total_count, logits)
         concentration = total_count
         rate = jnp.exp(-logits)
         super().__init__(concentration, rate, validate_args=validate_args)
 
     @validate_sample
     def log_prob(self, value):
@@ -272,15 +272,15 @@
 
     arg_constraints = {
         "mean": constraints.positive,
         "concentration": constraints.positive,
     }
     support = constraints.nonnegative_integer
 
-    def __init__(self, mean, concentration, validate_args=None):
+    def __init__(self, mean, concentration, *, validate_args=None):
         rate = concentration / mean
         super().__init__(concentration, rate, validate_args=validate_args)
 
 
 def ZeroInflatedNegativeBinomial2(
     mean, concentration, *, gate=None, gate_logits=None, validate_args=None
 ):
```

### Comparing `numpyro-0.9.1/numpyro/distributions/constraints.py` & `numpyro-0.9.2/numpyro/distributions/constraints.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,14 +73,17 @@
 
     is_discrete = False
     event_dim = 0
 
     def __call__(self, x):
         raise NotImplementedError
 
+    def __repr__(self):
+        return self.__class__.__name__[1:] + "()"
+
     def check(self, value):
         """
         Returns a byte tensor of `sample_shape + batch_shape` indicating
         whether each event in value satisfies this constraint.
         """
         return self(value)
 
@@ -213,14 +216,19 @@
 class _GreaterThan(Constraint):
     def __init__(self, lower_bound):
         self.lower_bound = lower_bound
 
     def __call__(self, x):
         return x > self.lower_bound
 
+    def __repr__(self):
+        fmt_string = self.__class__.__name__[1:]
+        fmt_string += "(lower_bound={})".format(self.lower_bound)
+        return fmt_string
+
     def feasible_like(self, prototype):
         return jax.numpy.broadcast_to(self.lower_bound + 1, jax.numpy.shape(prototype))
 
 
 class _IndependentConstraint(Constraint):
     """
     Wraps a constraint by aggregating over ``reinterpreted_batch_ndims``-many
@@ -259,64 +267,95 @@
                 : jax.numpy.ndim(result) - self.reinterpreted_batch_ndims
             ]
             + (-1,)
         )
         result = result.all(-1)
         return result
 
+    def __repr__(self):
+        return "{}({}, {})".format(
+            self.__class__.__name__[1:],
+            repr(self.base_constraint),
+            self.reinterpreted_batch_ndims,
+        )
+
     def feasible_like(self, prototype):
         return self.base_constraint.feasible_like(prototype)
 
 
 class _LessThan(Constraint):
     def __init__(self, upper_bound):
         self.upper_bound = upper_bound
 
     def __call__(self, x):
         return x < self.upper_bound
 
+    def __repr__(self):
+        fmt_string = self.__class__.__name__[1:]
+        fmt_string += "(upper_bound={})".format(self.upper_bound)
+        return fmt_string
+
     def feasible_like(self, prototype):
         return jax.numpy.broadcast_to(self.upper_bound - 1, jax.numpy.shape(prototype))
 
 
 class _IntegerInterval(Constraint):
     is_discrete = True
 
     def __init__(self, lower_bound, upper_bound):
         self.lower_bound = lower_bound
         self.upper_bound = upper_bound
 
     def __call__(self, x):
         return (x >= self.lower_bound) & (x <= self.upper_bound) & (x % 1 == 0)
 
+    def __repr__(self):
+        fmt_string = self.__class__.__name__[1:]
+        fmt_string += "(lower_bound={}, upper_bound={})".format(
+            self.lower_bound, self.upper_bound
+        )
+        return fmt_string
+
     def feasible_like(self, prototype):
         return jax.numpy.broadcast_to(self.lower_bound, jax.numpy.shape(prototype))
 
 
 class _IntegerGreaterThan(Constraint):
     is_discrete = True
 
     def __init__(self, lower_bound):
         self.lower_bound = lower_bound
 
     def __call__(self, x):
         return (x % 1 == 0) & (x >= self.lower_bound)
 
+    def __repr__(self):
+        fmt_string = self.__class__.__name__[1:]
+        fmt_string += "(lower_bound={})".format(self.lower_bound)
+        return fmt_string
+
     def feasible_like(self, prototype):
         return jax.numpy.broadcast_to(self.lower_bound, jax.numpy.shape(prototype))
 
 
 class _Interval(Constraint):
     def __init__(self, lower_bound, upper_bound):
         self.lower_bound = lower_bound
         self.upper_bound = upper_bound
 
     def __call__(self, x):
         return (x >= self.lower_bound) & (x <= self.upper_bound)
 
+    def __repr__(self):
+        fmt_string = self.__class__.__name__[1:]
+        fmt_string += "(lower_bound={}, upper_bound={})".format(
+            self.lower_bound, self.upper_bound
+        )
+        return fmt_string
+
     def feasible_like(self, prototype):
         return jax.numpy.broadcast_to(
             (self.lower_bound + self.upper_bound) / 2, jax.numpy.shape(prototype)
         )
 
     def __eq__(self, other):
         return (
@@ -326,14 +365,21 @@
         )
 
 
 class _OpenInterval(_Interval):
     def __call__(self, x):
         return (x > self.lower_bound) & (x < self.upper_bound)
 
+    def __repr__(self):
+        fmt_string = self.__class__.__name__[1:]
+        fmt_string += "(lower_bound={}, upper_bound={})".format(
+            self.lower_bound, self.upper_bound
+        )
+        return fmt_string
+
 
 class _LowerCholesky(Constraint):
     event_dim = 2
 
     def __call__(self, x):
         jnp = np if isinstance(x, (np.ndarray, np.generic)) else jax.numpy
         tril = jnp.tril(x)
```

### Comparing `numpyro-0.9.1/numpyro/distributions/continuous.py` & `numpyro-0.9.2/numpyro/distributions/continuous.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         "loc": constraints.real,
         "scale": constraints.positive,
         "asymmetry": constraints.positive,
     }
     reparametrized_params = ["loc", "scale", "asymmetry"]
     support = constraints.real
 
-    def __init__(self, loc=0.0, scale=1.0, asymmetry=1.0, validate_args=None):
+    def __init__(self, loc=0.0, scale=1.0, asymmetry=1.0, *, validate_args=None):
         batch_shape = lax.broadcast_shapes(
             jnp.shape(loc), jnp.shape(scale), jnp.shape(asymmetry)
         )
         self.loc, self.scale, self.asymmetry = promote_shapes(
             loc, scale, asymmetry, shape=batch_shape
         )
         super(AsymmetricLaplace, self).__init__(
@@ -146,15 +146,15 @@
     arg_constraints = {
         "concentration1": constraints.positive,
         "concentration0": constraints.positive,
     }
     reparametrized_params = ["concentration1", "concentration0"]
     support = constraints.unit_interval
 
-    def __init__(self, concentration1, concentration0, validate_args=None):
+    def __init__(self, concentration1, concentration0, *, validate_args=None):
         self.concentration1, self.concentration0 = promote_shapes(
             concentration1, concentration0
         )
         batch_shape = lax.broadcast_shapes(
             jnp.shape(concentration1), jnp.shape(concentration0)
         )
         concentration1 = jnp.broadcast_to(concentration1, batch_shape)
@@ -186,15 +186,15 @@
 
 
 class Cauchy(Distribution):
     arg_constraints = {"loc": constraints.real, "scale": constraints.positive}
     support = constraints.real
     reparametrized_params = ["loc", "scale"]
 
-    def __init__(self, loc=0.0, scale=1.0, validate_args=None):
+    def __init__(self, loc=0.0, scale=1.0, *, validate_args=None):
         self.loc, self.scale = promote_shapes(loc, scale)
         batch_shape = lax.broadcast_shapes(jnp.shape(loc), jnp.shape(scale))
         super(Cauchy, self).__init__(
             batch_shape=batch_shape, validate_args=validate_args
         )
 
     def sample(self, key, sample_shape=()):
@@ -229,43 +229,31 @@
 class Dirichlet(Distribution):
     arg_constraints = {
         "concentration": constraints.independent(constraints.positive, 1)
     }
     reparametrized_params = ["concentration"]
     support = constraints.simplex
 
-    def __init__(self, concentration, validate_args=None):
+    def __init__(self, concentration, *, validate_args=None):
         if jnp.ndim(concentration) < 1:
             raise ValueError(
                 "`concentration` parameter must be at least one-dimensional."
             )
         self.concentration = concentration
         batch_shape, event_shape = concentration.shape[:-1], concentration.shape[-1:]
         super(Dirichlet, self).__init__(
             batch_shape=batch_shape,
             event_shape=event_shape,
             validate_args=validate_args,
         )
 
     def sample(self, key, sample_shape=()):
         assert is_prng_key(key)
-        shape = sample_shape + self.batch_shape + self.event_shape
-        key_gamma, key_expon = random.split(key)
-        # To improve precision for the cases concentration << 1,
-        # we boost concentration to concentration + 1 and get gamma samples according to
-        #   Gamma(concentration) ~ Gamma(concentration+1) * Uniform()^(1 / concentration)
-        # When concentration << 1, u^(1 / concentration) is very near 0 and lost precision, so
-        # we will convert the samples to log space
-        #   log(Gamma(concentration)) ~ log(Gamma(concentration + 1)) - Expon() / concentration
-        # and apply softmax to get a dirichlet sample
-        gamma_samples = random.gamma(key_gamma, self.concentration + 1, shape=shape)
-        expon_samples = random.exponential(key_expon, shape=shape)
-        samples = nn.softmax(
-            jnp.log(gamma_samples) - expon_samples / self.concentration, -1
-        )
+        shape = sample_shape + self.batch_shape
+        samples = random.dirichlet(key, self.concentration, shape=shape)
         return jnp.clip(
             samples, a_min=jnp.finfo(samples).tiny, a_max=1 - jnp.finfo(samples).eps
         )
 
     @validate_sample
     def log_prob(self, value):
         normalize_term = jnp.sum(gammaln(self.concentration), axis=-1) - gammaln(
@@ -295,15 +283,15 @@
 
 
 class Exponential(Distribution):
     reparametrized_params = ["rate"]
     arg_constraints = {"rate": constraints.positive}
     support = constraints.positive
 
-    def __init__(self, rate=1.0, validate_args=None):
+    def __init__(self, rate=1.0, *, validate_args=None):
         self.rate = rate
         super(Exponential, self).__init__(
             batch_shape=jnp.shape(rate), validate_args=validate_args
         )
 
     def sample(self, key, sample_shape=()):
         assert is_prng_key(key)
@@ -334,15 +322,15 @@
     arg_constraints = {
         "concentration": constraints.positive,
         "rate": constraints.positive,
     }
     support = constraints.positive
     reparametrized_params = ["concentration", "rate"]
 
-    def __init__(self, concentration, rate=1.0, validate_args=None):
+    def __init__(self, concentration, rate=1.0, *, validate_args=None):
         self.concentration, self.rate = promote_shapes(concentration, rate)
         batch_shape = lax.broadcast_shapes(jnp.shape(concentration), jnp.shape(rate))
         super(Gamma, self).__init__(
             batch_shape=batch_shape, validate_args=validate_args
         )
 
     def sample(self, key, sample_shape=()):
@@ -373,25 +361,25 @@
         return gammainc(self.concentration, self.rate * x)
 
 
 class Chi2(Gamma):
     arg_constraints = {"df": constraints.positive}
     reparametrized_params = ["df"]
 
-    def __init__(self, df, validate_args=None):
+    def __init__(self, df, *, validate_args=None):
         self.df = df
         super(Chi2, self).__init__(0.5 * df, 0.5, validate_args=validate_args)
 
 
 class GaussianRandomWalk(Distribution):
     arg_constraints = {"scale": constraints.positive}
     support = constraints.real_vector
     reparametrized_params = ["scale"]
 
-    def __init__(self, scale=1.0, num_steps=1, validate_args=None):
+    def __init__(self, scale=1.0, num_steps=1, *, validate_args=None):
         assert (
             isinstance(num_steps, int) and num_steps > 0
         ), "`num_steps` argument should be an positive integer."
         self.scale = scale
         self.num_steps = num_steps
         batch_shape, event_shape = jnp.shape(scale), (num_steps,)
         super(GaussianRandomWalk, self).__init__(
@@ -431,15 +419,15 @@
 
 
 class HalfCauchy(Distribution):
     reparametrized_params = ["scale"]
     support = constraints.positive
     arg_constraints = {"scale": constraints.positive}
 
-    def __init__(self, scale=1.0, validate_args=None):
+    def __init__(self, scale=1.0, *, validate_args=None):
         self._cauchy = Cauchy(0.0, scale)
         self.scale = scale
         super(HalfCauchy, self).__init__(
             batch_shape=jnp.shape(scale), validate_args=validate_args
         )
 
     def sample(self, key, sample_shape=()):
@@ -466,15 +454,15 @@
 
 
 class HalfNormal(Distribution):
     reparametrized_params = ["scale"]
     support = constraints.positive
     arg_constraints = {"scale": constraints.positive}
 
-    def __init__(self, scale=1.0, validate_args=None):
+    def __init__(self, scale=1.0, *, validate_args=None):
         self._normal = Normal(0.0, scale)
         self.scale = scale
         super(HalfNormal, self).__init__(
             batch_shape=jnp.shape(scale), validate_args=validate_args
         )
 
     def sample(self, key, sample_shape=()):
@@ -510,15 +498,15 @@
     arg_constraints = {
         "concentration": constraints.positive,
         "rate": constraints.positive,
     }
     reparametrized_params = ["concentration", "rate"]
     support = constraints.positive
 
-    def __init__(self, concentration, rate=1.0, validate_args=None):
+    def __init__(self, concentration, rate=1.0, *, validate_args=None):
         base_dist = Gamma(concentration, rate)
         self.concentration = base_dist.concentration
         self.rate = base_dist.rate
         super(InverseGamma, self).__init__(
             base_dist, PowerTransform(-1.0), validate_args=validate_args
         )
 
@@ -542,15 +530,15 @@
 
 
 class Gumbel(Distribution):
     arg_constraints = {"loc": constraints.real, "scale": constraints.positive}
     support = constraints.real
     reparametrized_params = ["loc", "scale"]
 
-    def __init__(self, loc=0.0, scale=1.0, validate_args=None):
+    def __init__(self, loc=0.0, scale=1.0, *, validate_args=None):
         self.loc, self.scale = promote_shapes(loc, scale)
         batch_shape = lax.broadcast_shapes(jnp.shape(loc), jnp.shape(scale))
 
         super(Gumbel, self).__init__(
             batch_shape=batch_shape, validate_args=validate_args
         )
 
@@ -593,15 +581,15 @@
     # XXX: This flag is used to approximate the Taylor expansion
     # of KL(Kumaraswamy||Beta) following
     # https://arxiv.org/abs/1605.06197 Formula (12)
     # We follow the paper and set this to 10 but to get more precise KL,
     # we can set this flag to 1000.
     KL_KUMARASWAMY_BETA_TAYLOR_ORDER = 10
 
-    def __init__(self, concentration1, concentration0, validate_args=None):
+    def __init__(self, concentration1, concentration0, *, validate_args=None):
         self.concentration1, self.concentration0 = promote_shapes(
             concentration1, concentration0
         )
         batch_shape = lax.broadcast_shapes(
             jnp.shape(concentration1), jnp.shape(concentration0)
         )
         base_dist = Uniform(0, 1).expand(batch_shape)
@@ -644,15 +632,15 @@
 
 
 class Laplace(Distribution):
     arg_constraints = {"loc": constraints.real, "scale": constraints.positive}
     support = constraints.real
     reparametrized_params = ["loc", "scale"]
 
-    def __init__(self, loc=0.0, scale=1.0, validate_args=None):
+    def __init__(self, loc=0.0, scale=1.0, *, validate_args=None):
         self.loc, self.scale = promote_shapes(loc, scale)
         batch_shape = lax.broadcast_shapes(jnp.shape(loc), jnp.shape(scale))
         super(Laplace, self).__init__(
             batch_shape=batch_shape, validate_args=validate_args
         )
 
     def sample(self, key, sample_shape=()):
@@ -732,15 +720,15 @@
     Daniel Lewandowski, Dorota Kurowicka, Harry Joe
     """
     arg_constraints = {"concentration": constraints.positive}
     reparametrized_params = ["concentration"]
     support = constraints.corr_matrix
 
     def __init__(
-        self, dimension, concentration=1.0, sample_method="onion", validate_args=None
+        self, dimension, concentration=1.0, sample_method="onion", *, validate_args=None
     ):
         base_dist = LKJCholesky(dimension, concentration, sample_method)
         self.dimension, self.concentration = (
             base_dist.dimension,
             base_dist.concentration,
         )
         self.sample_method = sample_method
@@ -815,15 +803,15 @@
     Daniel Lewandowski, Dorota Kurowicka, Harry Joe
     """
     arg_constraints = {"concentration": constraints.positive}
     reparametrized_params = ["concentration"]
     support = constraints.corr_cholesky
 
     def __init__(
-        self, dimension, concentration=1.0, sample_method="onion", validate_args=None
+        self, dimension, concentration=1.0, sample_method="onion", *, validate_args=None
     ):
         if dimension < 2:
             raise ValueError("Dimension must be greater than or equal to 2.")
         self.dimension = dimension
         self.concentration = concentration
         batch_shape = jnp.shape(concentration)
         event_shape = (dimension, dimension)
@@ -976,15 +964,15 @@
 
 
 class LogNormal(TransformedDistribution):
     arg_constraints = {"loc": constraints.real, "scale": constraints.positive}
     support = constraints.positive
     reparametrized_params = ["loc", "scale"]
 
-    def __init__(self, loc=0.0, scale=1.0, validate_args=None):
+    def __init__(self, loc=0.0, scale=1.0, *, validate_args=None):
         base_dist = Normal(loc, scale)
         self.loc, self.scale = base_dist.loc, base_dist.scale
         super(LogNormal, self).__init__(
             base_dist, ExpTransform(), validate_args=validate_args
         )
 
     @property
@@ -1003,15 +991,15 @@
 
 
 class Logistic(Distribution):
     arg_constraints = {"loc": constraints.real, "scale": constraints.positive}
     support = constraints.real
     reparametrized_params = ["loc", "scale"]
 
-    def __init__(self, loc=0.0, scale=1.0, validate_args=None):
+    def __init__(self, loc=0.0, scale=1.0, *, validate_args=None):
         self.loc, self.scale = promote_shapes(loc, scale)
         batch_shape = lax.broadcast_shapes(jnp.shape(loc), jnp.shape(scale))
         super(Logistic, self).__init__(batch_shape, validate_args=validate_args)
 
     def sample(self, key, sample_shape=()):
         assert is_prng_key(key)
         z = random.logistic(
@@ -1350,15 +1338,15 @@
         "loc": constraints.real_vector,
         "cov_factor": constraints.independent(constraints.real, 2),
         "cov_diag": constraints.independent(constraints.positive, 1),
     }
     support = constraints.real_vector
     reparametrized_params = ["loc", "cov_factor", "cov_diag"]
 
-    def __init__(self, loc, cov_factor, cov_diag, validate_args=None):
+    def __init__(self, loc, cov_factor, cov_diag, *, validate_args=None):
         if jnp.ndim(loc) < 1:
             raise ValueError("`loc` must be at least one-dimensional.")
         event_shape = jnp.shape(loc)[-1:]
         if jnp.ndim(cov_factor) < 2:
             raise ValueError(
                 "`cov_factor` must be at least two-dimensional, "
                 "with optional leading batch dimensions"
@@ -1481,15 +1469,15 @@
 
 
 class Normal(Distribution):
     arg_constraints = {"loc": constraints.real, "scale": constraints.positive}
     support = constraints.real
     reparametrized_params = ["loc", "scale"]
 
-    def __init__(self, loc=0.0, scale=1.0, validate_args=None):
+    def __init__(self, loc=0.0, scale=1.0, *, validate_args=None):
         self.loc, self.scale = promote_shapes(loc, scale)
         batch_shape = lax.broadcast_shapes(jnp.shape(loc), jnp.shape(scale))
         super(Normal, self).__init__(
             batch_shape=batch_shape, validate_args=validate_args
         )
 
     def sample(self, key, sample_shape=()):
@@ -1521,15 +1509,15 @@
         return jnp.broadcast_to(self.scale**2, self.batch_shape)
 
 
 class Pareto(TransformedDistribution):
     arg_constraints = {"scale": constraints.positive, "alpha": constraints.positive}
     reparametrized_params = ["scale", "alpha"]
 
-    def __init__(self, scale, alpha, validate_args=None):
+    def __init__(self, scale, alpha, *, validate_args=None):
         self.scale, self.alpha = promote_shapes(scale, alpha)
         batch_shape = lax.broadcast_shapes(jnp.shape(scale), jnp.shape(alpha))
         scale, alpha = jnp.broadcast_to(scale, batch_shape), jnp.broadcast_to(
             alpha, batch_shape
         )
         base_dist = Exponential(alpha)
         transforms = [ExpTransform(), AffineTransform(loc=0, scale=scale)]
@@ -1564,25 +1552,25 @@
         return super(TransformedDistribution, self).tree_flatten()
 
 
 class RelaxedBernoulliLogits(TransformedDistribution):
     arg_constraints = {"temperature": constraints.positive, "logits": constraints.real}
     support = constraints.unit_interval
 
-    def __init__(self, temperature, logits, validate_args=None):
+    def __init__(self, temperature, logits, *, validate_args=None):
         self.temperature, self.logits = promote_shapes(temperature, logits)
         base_dist = Logistic(logits / temperature, 1 / temperature)
         transforms = [SigmoidTransform()]
         super().__init__(base_dist, transforms, validate_args=validate_args)
 
     def tree_flatten(self):
         return super(TransformedDistribution, self).tree_flatten()
 
 
-def RelaxedBernoulli(temperature, probs=None, logits=None, validate_args=None):
+def RelaxedBernoulli(temperature, probs=None, logits=None, *, validate_args=None):
     if probs is None and logits is None:
         raise ValueError("One of `probs` or `logits` must be specified.")
     if probs is not None:
         logits = _to_logits_bernoulli(probs)
     return RelaxedBernoulliLogits(temperature, logits, validate_args=validate_args)
 
 
@@ -1648,15 +1636,15 @@
         "df": constraints.positive,
         "loc": constraints.real,
         "scale": constraints.positive,
     }
     support = constraints.real
     reparametrized_params = ["df", "loc", "scale"]
 
-    def __init__(self, df, loc=0.0, scale=1.0, validate_args=None):
+    def __init__(self, df, loc=0.0, scale=1.0, *, validate_args=None):
         batch_shape = lax.broadcast_shapes(
             jnp.shape(df), jnp.shape(loc), jnp.shape(scale)
         )
         self.df, self.loc, self.scale = promote_shapes(
             df, loc, scale, shape=batch_shape
         )
         df = jnp.broadcast_to(df, batch_shape)
@@ -1719,15 +1707,15 @@
         raise NotImplementedError
 
 
 class Uniform(Distribution):
     arg_constraints = {"low": constraints.dependent, "high": constraints.dependent}
     reparametrized_params = ["low", "high"]
 
-    def __init__(self, low=0.0, high=1.0, validate_args=None):
+    def __init__(self, low=0.0, high=1.0, *, validate_args=None):
         self.low, self.high = promote_shapes(low, high)
         batch_shape = lax.broadcast_shapes(jnp.shape(low), jnp.shape(high))
         self._support = constraints.interval(low, high)
         super().__init__(batch_shape, validate_args=validate_args)
 
     @constraints.dependent_property(is_discrete=False, event_dim=0)
     def support(self):
@@ -1784,15 +1772,15 @@
     arg_constraints = {
         "scale": constraints.positive,
         "concentration": constraints.positive,
     }
     support = constraints.positive
     reparametrized_params = ["scale", "concentration"]
 
-    def __init__(self, scale, concentration, validate_args=None):
+    def __init__(self, scale, concentration, *, validate_args=None):
         self.concentration, self.scale = promote_shapes(concentration, scale)
         batch_shape = lax.broadcast_shapes(jnp.shape(concentration), jnp.shape(scale))
         super().__init__(batch_shape=batch_shape, validate_args=validate_args)
 
     def sample(self, key, sample_shape=()):
         assert is_prng_key(key)
         return random.weibull_min(
@@ -1839,15 +1827,15 @@
     arg_constraints = {
         "mean": constraints.open_interval(0.0, 1.0),
         "concentration": constraints.positive,
     }
     reparametrized_params = ["mean", "concentration"]
     support = constraints.unit_interval
 
-    def __init__(self, mean, concentration, validate_args=None):
+    def __init__(self, mean, concentration, *, validate_args=None):
         self.concentration = jnp.broadcast_to(
             concentration, lax.broadcast_shapes(jnp.shape(concentration))
         )
         super().__init__(
             mean * concentration,
             (1.0 - mean) * concentration,
             validate_args=validate_args,
@@ -1874,15 +1862,15 @@
         "loc": constraints.real,
         "scale": constraints.positive,
         "quantile": constraints.open_interval(0.0, 1.0),
     }
     reparametrized_params = ["loc", "scale", "quantile"]
     support = constraints.real
 
-    def __init__(self, loc=0.0, scale=1.0, quantile=0.5, validate_args=None):
+    def __init__(self, loc=0.0, scale=1.0, quantile=0.5, *, validate_args=None):
         batch_shape = lax.broadcast_shapes(
             jnp.shape(loc), jnp.shape(scale), jnp.shape(quantile)
         )
         self.loc, self.scale, self.quantile = promote_shapes(
             loc, scale, quantile, shape=batch_shape
         )
         super(AsymmetricLaplaceQuantile, self).__init__(
```

### Comparing `numpyro-0.9.1/numpyro/distributions/directional.py` & `numpyro-0.9.2/numpyro/distributions/directional.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             ...
     """
 
     arg_constraints = {"loc": constraints.real, "concentration": constraints.positive}
     reparametrized_params = ["loc"]
     support = constraints.circular
 
-    def __init__(self, loc, concentration, validate_args=None):
+    def __init__(self, loc, concentration, *, validate_args=None):
         """von Mises distribution for sampling directions.
 
         :param loc: center of distribution
         :param concentration: concentration of distribution
         """
         self.loc, self.concentration = promote_shapes(loc, concentration)
 
@@ -213,15 +213,15 @@
     :param jax.numpy.array skewness: skewness of the distribution.
     """
 
     arg_constraints = {"skewness": constraints.l1_ball}
 
     support = constraints.independent(constraints.circular, 1)
 
-    def __init__(self, base_dist: Distribution, skewness, validate_args=None):
+    def __init__(self, base_dist: Distribution, skewness, *, validate_args=None):
         assert (
             base_dist.event_shape == skewness.shape[-1:]
         ), "Sine Skewing is only valid with a skewness parameter for each dimension of `base_dist.event_shape`."
 
         batch_shape = jnp.broadcast_shapes(base_dist.batch_shape, skewness.shape[:-1])
         event_shape = skewness.shape[-1:]
         self.skewness = jnp.broadcast_to(skewness, batch_shape + event_shape)
@@ -353,31 +353,43 @@
 
         if weighted_correlation is not None:
             correlation = (
                 weighted_correlation * jnp.sqrt(phi_concentration * psi_concentration)
                 + 1e-8
             )
 
+        batch_shape = lax.broadcast_shapes(
+            jnp.shape(phi_loc),
+            jnp.shape(psi_loc),
+            jnp.shape(phi_concentration),
+            jnp.shape(psi_concentration),
+            jnp.shape(correlation),
+        )
         (
             self.phi_loc,
             self.psi_loc,
             self.phi_concentration,
             self.psi_concentration,
             self.correlation,
         ) = promote_shapes(
-            phi_loc, psi_loc, phi_concentration, psi_concentration, correlation
-        )
-        batch_shape = lax.broadcast_shapes(
-            jnp.shape(phi_loc),
-            jnp.shape(psi_loc),
-            jnp.shape(phi_concentration),
-            jnp.shape(psi_concentration),
-            jnp.shape(correlation),
+            phi_loc,
+            psi_loc,
+            phi_concentration,
+            psi_concentration,
+            correlation,
+            shape=batch_shape,
         )
-        super().__init__(batch_shape, (2,), validate_args)
+
+        super().__init__(batch_shape, (2,), validate_args=validate_args)
+
+        self.phi_loc = jnp.broadcast_to(self.phi_loc, batch_shape)
+        self.psi_loc = jnp.broadcast_to(self.psi_loc, batch_shape)
+        self.phi_concentration = jnp.broadcast_to(self.phi_concentration, batch_shape)
+        self.psi_concentration = jnp.broadcast_to(self.psi_concentration, batch_shape)
+        self.correlation = jnp.broadcast_to(self.correlation, batch_shape)
 
     @lazy_property
     def norm_const(self):
         corr = jnp.reshape(self.correlation, (1, -1)) + 1e-8
         conc = jnp.stack(
             (self.phi_concentration, self.psi_concentration), axis=-1
         ).reshape(-1, 2)
@@ -439,25 +451,27 @@
             jnp.reshape(b0, (batch_size,)),
             jnp.reshape(eigmin, (batch_size,)),
             jnp.reshape(phi_den, (batch_size,)),
         )
 
         phi = jnp.arctan2(phi_state.phi[:, 1:], phi_state.phi[:, :1])
 
-        alpha = jnp.sqrt(conc[1] ** 2 + (corr * jnp.sin(phi)) ** 2)
-        beta = jnp.arctan(corr / conc[1] * jnp.sin(phi))
+        alpha = jnp.sqrt(
+            conc[1].reshape(-1) ** 2 + (corr.reshape(-1) * jnp.sin(phi)) ** 2
+        )
+        beta = jnp.arctan(corr.reshape(-1) / conc[1].reshape(-1) * jnp.sin(phi))
 
         psi = VonMises(beta, alpha).sample(psi_key)
 
         phi_psi = jnp.concatenate(
             (
-                (phi + self.phi_loc + pi) % (2 * pi) - pi,
-                (psi + self.psi_loc + pi) % (2 * pi) - pi,
+                (phi + jnp.reshape(self.phi_loc, -1) + pi) % (2 * pi) - pi,
+                (psi + jnp.reshape(self.psi_loc, -1) + pi) % (2 * pi) - pi,
             ),
-            axis=1,
+            axis=-1,
         )
         phi_psi = jnp.transpose(phi_psi, (0, 2, 1))
         return phi_psi.reshape(*sample_shape, *self.batch_shape, *self.event_shape)
 
     @staticmethod
     def _phi_marginal(shape, rng_key, conc, corr, eig, b0, eigmin, phi_den):
         conc = jnp.broadcast_to(conc, shape)
```

### Comparing `numpyro-0.9.1/numpyro/distributions/discrete.py` & `numpyro-0.9.2/numpyro/distributions/discrete.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 
 class BernoulliProbs(Distribution):
     arg_constraints = {"probs": constraints.unit_interval}
     support = constraints.boolean
     has_enumerate_support = True
 
-    def __init__(self, probs, validate_args=None):
+    def __init__(self, probs, *, validate_args=None):
         self.probs = probs
         super(BernoulliProbs, self).__init__(
             batch_shape=jnp.shape(self.probs), validate_args=validate_args
         )
 
     def sample(self, key, sample_shape=()):
         assert is_prng_key(key)
@@ -111,15 +111,15 @@
 
 
 class BernoulliLogits(Distribution):
     arg_constraints = {"logits": constraints.real}
     support = constraints.boolean
     has_enumerate_support = True
 
-    def __init__(self, logits=None, validate_args=None):
+    def __init__(self, logits=None, *, validate_args=None):
         self.logits = logits
         super(BernoulliLogits, self).__init__(
             batch_shape=jnp.shape(self.logits), validate_args=validate_args
         )
 
     def sample(self, key, sample_shape=()):
         assert is_prng_key(key)
@@ -147,15 +147,15 @@
     def enumerate_support(self, expand=True):
         values = jnp.arange(2).reshape((-1,) + (1,) * len(self.batch_shape))
         if expand:
             values = jnp.broadcast_to(values, values.shape[:1] + self.batch_shape)
         return values
 
 
-def Bernoulli(probs=None, logits=None, validate_args=None):
+def Bernoulli(probs=None, logits=None, *, validate_args=None):
     if probs is not None:
         return BernoulliProbs(probs, validate_args=validate_args)
     elif logits is not None:
         return BernoulliLogits(logits, validate_args=validate_args)
     else:
         raise ValueError("One of `probs` or `logits` must be specified.")
 
@@ -163,15 +163,15 @@
 class BinomialProbs(Distribution):
     arg_constraints = {
         "probs": constraints.unit_interval,
         "total_count": constraints.nonnegative_integer,
     }
     has_enumerate_support = True
 
-    def __init__(self, probs, total_count=1, validate_args=None):
+    def __init__(self, probs, total_count=1, *, validate_args=None):
         self.probs, self.total_count = promote_shapes(probs, total_count)
         batch_shape = lax.broadcast_shapes(jnp.shape(probs), jnp.shape(total_count))
         super(BinomialProbs, self).__init__(
             batch_shape=batch_shape, validate_args=validate_args
         )
 
     def sample(self, key, sample_shape=()):
@@ -181,20 +181,21 @@
         )
 
     @validate_sample
     def log_prob(self, value):
         log_factorial_n = gammaln(self.total_count + 1)
         log_factorial_k = gammaln(value + 1)
         log_factorial_nmk = gammaln(self.total_count - value + 1)
+        probs = clamp_probs(self.probs)
         return (
             log_factorial_n
             - log_factorial_k
             - log_factorial_nmk
-            + xlogy(value, self.probs)
-            + xlog1py(self.total_count - value, -self.probs)
+            + xlogy(value, probs)
+            + xlog1py(self.total_count - value, -probs)
         )
 
     @lazy_property
     def logits(self):
         return _to_logits_bernoulli(self.probs)
 
     @property
@@ -233,15 +234,15 @@
     arg_constraints = {
         "logits": constraints.real,
         "total_count": constraints.nonnegative_integer,
     }
     has_enumerate_support = True
     enumerate_support = BinomialProbs.enumerate_support
 
-    def __init__(self, logits, total_count=1, validate_args=None):
+    def __init__(self, logits, total_count=1, *, validate_args=None):
         self.logits, self.total_count = promote_shapes(logits, total_count)
         batch_shape = lax.broadcast_shapes(jnp.shape(logits), jnp.shape(total_count))
         super(BinomialLogits, self).__init__(
             batch_shape=batch_shape, validate_args=validate_args
         )
 
     def sample(self, key, sample_shape=()):
@@ -279,28 +280,28 @@
         )
 
     @constraints.dependent_property(is_discrete=True, event_dim=0)
     def support(self):
         return constraints.integer_interval(0, self.total_count)
 
 
-def Binomial(total_count=1, probs=None, logits=None, validate_args=None):
+def Binomial(total_count=1, probs=None, logits=None, *, validate_args=None):
     if probs is not None:
         return BinomialProbs(probs, total_count, validate_args=validate_args)
     elif logits is not None:
         return BinomialLogits(logits, total_count, validate_args=validate_args)
     else:
         raise ValueError("One of `probs` or `logits` must be specified.")
 
 
 class CategoricalProbs(Distribution):
     arg_constraints = {"probs": constraints.simplex}
     has_enumerate_support = True
 
-    def __init__(self, probs, validate_args=None):
+    def __init__(self, probs, *, validate_args=None):
         if jnp.ndim(probs) < 1:
             raise ValueError("`probs` parameter must be at least one-dimensional.")
         self.probs = probs
         super(CategoricalProbs, self).__init__(
             batch_shape=jnp.shape(self.probs)[:-1], validate_args=validate_args
         )
 
@@ -342,15 +343,15 @@
         return values
 
 
 class CategoricalLogits(Distribution):
     arg_constraints = {"logits": constraints.real_vector}
     has_enumerate_support = True
 
-    def __init__(self, logits, validate_args=None):
+    def __init__(self, logits, *, validate_args=None):
         if jnp.ndim(logits) < 1:
             raise ValueError("`logits` parameter must be at least one-dimensional.")
         self.logits = logits
         super(CategoricalLogits, self).__init__(
             batch_shape=jnp.shape(logits)[:-1], validate_args=validate_args
         )
 
@@ -390,28 +391,28 @@
             (-1,) + (1,) * len(self.batch_shape)
         )
         if expand:
             values = jnp.broadcast_to(values, values.shape[:1] + self.batch_shape)
         return values
 
 
-def Categorical(probs=None, logits=None, validate_args=None):
+def Categorical(probs=None, logits=None, *, validate_args=None):
     if probs is not None:
         return CategoricalProbs(probs, validate_args=validate_args)
     elif logits is not None:
         return CategoricalLogits(logits, validate_args=validate_args)
     else:
         raise ValueError("One of `probs` or `logits` must be specified.")
 
 
 class DiscreteUniform(Distribution):
     arg_constraints = {"low": constraints.dependent, "high": constraints.dependent}
     has_enumerate_support = True
 
-    def __init__(self, low=0, high=1, validate_args=None):
+    def __init__(self, low=0, high=1, *, validate_args=None):
         self.low, self.high = promote_shapes(low, high)
         batch_shape = lax.broadcast_shapes(jnp.shape(low), jnp.shape(high))
         self._support = constraints.integer_interval(low, high)
         super().__init__(batch_shape, validate_args=validate_args)
 
     @constraints.dependent_property(is_discrete=True, event_dim=0)
     def support(self):
@@ -477,15 +478,15 @@
     """
 
     arg_constraints = {
         "predictor": constraints.real,
         "cutpoints": constraints.ordered_vector,
     }
 
-    def __init__(self, predictor, cutpoints, validate_args=None):
+    def __init__(self, predictor, cutpoints, *, validate_args=None):
         if jnp.ndim(predictor) == 0:
             (predictor,) = promote_shapes(predictor, shape=(1,))
         else:
             predictor = predictor[..., None]
         predictor, self.cutpoints = promote_shapes(predictor, cutpoints)
         self.predictor = predictor[..., 0]
         probs = transforms.SimplexToOrderedTransform(self.predictor).inv(self.cutpoints)
@@ -500,15 +501,15 @@
 
 class MultinomialProbs(Distribution):
     arg_constraints = {
         "probs": constraints.simplex,
         "total_count": constraints.nonnegative_integer,
     }
 
-    def __init__(self, probs, total_count=1, validate_args=None):
+    def __init__(self, probs, total_count=1, *, validate_args=None):
         if jnp.ndim(probs) < 1:
             raise ValueError("`probs` parameter must be at least one-dimensional.")
         batch_shape, event_shape = self.infer_shapes(
             jnp.shape(probs), jnp.shape(total_count)
         )
         self.probs = promote_shapes(probs, shape=batch_shape + jnp.shape(probs)[-1:])[0]
         self.total_count = promote_shapes(total_count, shape=batch_shape)[0]
@@ -557,15 +558,15 @@
 
 class MultinomialLogits(Distribution):
     arg_constraints = {
         "logits": constraints.real_vector,
         "total_count": constraints.nonnegative_integer,
     }
 
-    def __init__(self, logits, total_count=1, validate_args=None):
+    def __init__(self, logits, total_count=1, *, validate_args=None):
         if jnp.ndim(logits) < 1:
             raise ValueError("`logits` parameter must be at least one-dimensional.")
         batch_shape, event_shape = self.infer_shapes(
             jnp.shape(logits), jnp.shape(total_count)
         )
         self.logits = promote_shapes(
             logits, shape=batch_shape + jnp.shape(logits)[-1:]
@@ -613,15 +614,15 @@
     @staticmethod
     def infer_shapes(logits, total_count):
         batch_shape = lax.broadcast_shapes(logits[:-1], total_count)
         event_shape = logits[-1:]
         return batch_shape, event_shape
 
 
-def Multinomial(total_count=1, probs=None, logits=None, validate_args=None):
+def Multinomial(total_count=1, probs=None, logits=None, *, validate_args=None):
     if probs is not None:
         return MultinomialProbs(probs, total_count, validate_args=validate_args)
     elif logits is not None:
         return MultinomialLogits(logits, total_count, validate_args=validate_args)
     else:
         raise ValueError("One of `probs` or `logits` must be specified.")
 
@@ -791,24 +792,24 @@
     """
 
     arg_constraints = {"gate": constraints.unit_interval, "rate": constraints.positive}
     support = constraints.nonnegative_integer
 
     # TODO: resolve inconsistent parameter order w.r.t. Pyro
     # and support `gate_logits` argument
-    def __init__(self, gate, rate=1.0, validate_args=None):
+    def __init__(self, gate, rate=1.0, *, validate_args=None):
         _, self.rate = promote_shapes(gate, rate)
         super().__init__(Poisson(self.rate), gate, validate_args=validate_args)
 
 
 class GeometricProbs(Distribution):
     arg_constraints = {"probs": constraints.unit_interval}
     support = constraints.nonnegative_integer
 
-    def __init__(self, probs, validate_args=None):
+    def __init__(self, probs, *, validate_args=None):
         self.probs = probs
         super(GeometricProbs, self).__init__(
             batch_shape=jnp.shape(self.probs), validate_args=validate_args
         )
 
     def sample(self, key, sample_shape=()):
         assert is_prng_key(key)
@@ -836,15 +837,15 @@
         return (1.0 / self.probs - 1.0) / self.probs
 
 
 class GeometricLogits(Distribution):
     arg_constraints = {"logits": constraints.real}
     support = constraints.nonnegative_integer
 
-    def __init__(self, logits, validate_args=None):
+    def __init__(self, logits, *, validate_args=None):
         self.logits = logits
         super(GeometricLogits, self).__init__(
             batch_shape=jnp.shape(self.logits), validate_args=validate_args
         )
 
     @lazy_property
     def probs(self):
@@ -867,14 +868,14 @@
         return 1.0 / self.probs - 1.0
 
     @property
     def variance(self):
         return (1.0 / self.probs - 1.0) / self.probs
 
 
-def Geometric(probs=None, logits=None, validate_args=None):
+def Geometric(probs=None, logits=None, *, validate_args=None):
     if probs is not None:
         return GeometricProbs(probs, validate_args=validate_args)
     elif logits is not None:
         return GeometricLogits(logits, validate_args=validate_args)
     else:
         raise ValueError("One of `probs` or `logits` must be specified.")
```

### Comparing `numpyro-0.9.1/numpyro/distributions/distribution.py` & `numpyro-0.9.2/numpyro/distributions/distribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,25 +82,26 @@
         enable_validation(distribution_validation_status)
 
 
 COERCIONS = []
 
 
 class DistributionMeta(type):
+    def __init__(cls, *args, **kwargs):
+        signature = inspect.signature(functools.partial(cls.__init__, None))
+        cls.__signature__ = signature
+        return super().__init__(*args, **kwargs)
+
     def __call__(cls, *args, **kwargs):
         for coerce_ in COERCIONS:
             result = coerce_(cls, args, kwargs)
             if result is not None:
                 return result
         return super().__call__(*args, **kwargs)
 
-    @property
-    def __wrapped__(cls):
-        return functools.partial(cls.__init__, None)
-
 
 class Distribution(metaclass=DistributionMeta):
     """
     Base class for probability distributions in NumPyro. The design largely
     follows from :mod:`torch.distributions`.
 
     :param batch_shape: The batch shape for the distribution. This designates
@@ -153,15 +154,15 @@
 
     @staticmethod
     def set_default_validate_args(value):
         if value not in [True, False]:
             raise ValueError
         Distribution._validate_args = value
 
-    def __init__(self, batch_shape=(), event_shape=(), validate_args=None):
+    def __init__(self, batch_shape=(), event_shape=(), *, validate_args=None):
         self._batch_shape = batch_shape
         self._event_shape = event_shape
         if validate_args is not None:
             self._validate_args = validate_args
         if self._validate_args:
             for param, constraint in self.arg_constraints.items():
                 if param not in self.__dict__ and isinstance(
@@ -675,15 +676,15 @@
         set `batch_shape=()`.
     :param tuple event_shape: event shape of this distribution.
     """
 
     arg_constraints = {}
     support = constraints.dependent
 
-    def __init__(self, support, batch_shape, event_shape, validate_args=None):
+    def __init__(self, support, batch_shape, event_shape, *, validate_args=None):
         self.support = constraints.independent(
             support, len(event_shape) - support.event_dim
         )
         super().__init__(batch_shape, event_shape, validate_args=validate_args)
 
     @validate_sample
     def log_prob(self, value):
@@ -729,15 +730,15 @@
 
     :param numpyro.distribution.Distribution base_distribution: a distribution instance.
     :param int reinterpreted_batch_ndims: the number of batch dims to reinterpret as event dims.
     """
 
     arg_constraints = {}
 
-    def __init__(self, base_dist, reinterpreted_batch_ndims, validate_args=None):
+    def __init__(self, base_dist, reinterpreted_batch_ndims, *, validate_args=None):
         if reinterpreted_batch_ndims > len(base_dist.batch_shape):
             raise ValueError(
                 "Expected reinterpreted_batch_ndims <= len(base_distribution.batch_shape), "
                 "actual {} vs {}".format(
                     reinterpreted_batch_ndims, len(base_dist.batch_shape)
                 )
             )
@@ -917,15 +918,15 @@
     :param transforms: a single transform or a list of transforms.
     :param validate_args: Whether to enable validation of distribution
         parameters and arguments to `.log_prob` method.
     """
 
     arg_constraints = {}
 
-    def __init__(self, base_distribution, transforms, validate_args=None):
+    def __init__(self, base_distribution, transforms, *, validate_args=None):
         if isinstance(transforms, Transform):
             transforms = [transforms]
         elif isinstance(transforms, list):
             if not all(isinstance(t, Transform) for t in transforms):
                 raise ValueError(
                     "transforms must be a Transform or a list of Transforms"
                 )
@@ -1059,15 +1060,15 @@
     but additionally supports :meth:`log_prob` .
 
     :param Distribution base_dist: A univariate distribution to reflect.
     """
 
     support = constraints.positive
 
-    def __init__(self, base_dist, validate_args=None):
+    def __init__(self, base_dist, *, validate_args=None):
         if base_dist.event_shape:
             raise ValueError("Only univariate distributions can be folded.")
         super().__init__(base_dist, AbsTransform(), validate_args=validate_args)
 
     @validate_sample
     def log_prob(self, value):
         dim = max(len(self.batch_shape), jnp.ndim(value))
@@ -1088,15 +1089,15 @@
 class Delta(Distribution):
     arg_constraints = {
         "v": constraints.dependent(is_discrete=False),
         "log_density": constraints.real,
     }
     reparametrized_params = ["v", "log_density"]
 
-    def __init__(self, v=0.0, log_density=0.0, event_dim=0, validate_args=None):
+    def __init__(self, v=0.0, log_density=0.0, event_dim=0, *, validate_args=None):
         if event_dim > jnp.ndim(v):
             raise ValueError(
                 "Expected event_dim <= v.dim(), actual {} vs {}".format(
                     event_dim, jnp.ndim(v)
                 )
             )
         batch_dim = jnp.ndim(v) - event_dim
@@ -1147,15 +1148,15 @@
 
     This is used for :func:`numpyro.factor` statements.
     """
 
     arg_constraints = {"log_factor": constraints.real}
     support = constraints.real
 
-    def __init__(self, log_factor, validate_args=None):
+    def __init__(self, log_factor, *, validate_args=None):
         batch_shape = jnp.shape(log_factor)
         event_shape = (0,)  # This satisfies .size == 0.
         self.log_factor = log_factor
         super(Unit, self).__init__(
             batch_shape, event_shape, validate_args=validate_args
         )
```

### Comparing `numpyro-0.9.1/numpyro/distributions/flows.py` & `numpyro-0.9.2/numpyro/distributions/flows.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/distributions/gof.py` & `numpyro-0.9.2/numpyro/distributions/gof.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/distributions/kl.py` & `numpyro-0.9.2/numpyro/distributions/kl.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/distributions/mixtures.py` & `numpyro-0.9.2/numpyro/distributions/mixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,17 @@
        >>> mixing_dist = dist.Categorical(probs=jnp.ones(3) / 3.)
        >>> component_dist = dist.Normal(loc=jnp.zeros(3), scale=jnp.ones(3))
        >>> mixture = dist.MixtureSameFamily(mixing_dist, component_dist)
        >>> mixture.sample(jax.random.PRNGKey(42)).shape
        ()
     """
 
-    def __init__(self, mixing_distribution, component_distribution, validate_args=None):
+    def __init__(
+        self, mixing_distribution, component_distribution, *, validate_args=None
+    ):
         # Check arguments
         if not isinstance(mixing_distribution, (CategoricalLogits, CategoricalProbs)):
             raise ValueError(
                 "The mixing distribution need to be a numpyro.distributions.Categorical. "
                 f"However, it is of type {type(mixing_distribution)}"
             )
         mixture_size = mixing_distribution.probs.shape[-1]
```

### Comparing `numpyro-0.9.1/numpyro/distributions/transforms.py` & `numpyro-0.9.2/numpyro/distributions/transforms.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/distributions/truncated.py` & `numpyro-0.9.2/numpyro/distributions/truncated.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 class LeftTruncatedDistribution(Distribution):
     arg_constraints = {"low": constraints.real}
     reparametrized_params = ["low"]
     supported_types = (Cauchy, Laplace, Logistic, Normal, SoftLaplace, StudentT)
 
-    def __init__(self, base_dist, low=0.0, validate_args=None):
+    def __init__(self, base_dist, low=0.0, *, validate_args=None):
         assert isinstance(base_dist, self.supported_types)
         assert (
             base_dist.support is constraints.real
         ), "The base distribution should be univariate and have real support."
         batch_shape = lax.broadcast_shapes(base_dist.batch_shape, jnp.shape(low))
         self.base_dist = tree_map(
             lambda p: promote_shapes(p, shape=batch_shape)[0], base_dist
@@ -126,15 +126,15 @@
 
 
 class RightTruncatedDistribution(Distribution):
     arg_constraints = {"high": constraints.real}
     reparametrized_params = ["high"]
     supported_types = (Cauchy, Laplace, Logistic, Normal, SoftLaplace, StudentT)
 
-    def __init__(self, base_dist, high=0.0, validate_args=None):
+    def __init__(self, base_dist, high=0.0, *, validate_args=None):
         assert isinstance(base_dist, self.supported_types)
         assert (
             base_dist.support is constraints.real
         ), "The base distribution should be univariate and have real support."
         batch_shape = lax.broadcast_shapes(base_dist.batch_shape, jnp.shape(high))
         self.base_dist = tree_map(
             lambda p: promote_shapes(p, shape=batch_shape)[0], base_dist
@@ -211,15 +211,15 @@
 
 
 class TwoSidedTruncatedDistribution(Distribution):
     arg_constraints = {"low": constraints.dependent, "high": constraints.dependent}
     reparametrized_params = ["low", "high"]
     supported_types = (Cauchy, Laplace, Logistic, Normal, SoftLaplace, StudentT)
 
-    def __init__(self, base_dist, low=0.0, high=1.0, validate_args=None):
+    def __init__(self, base_dist, low=0.0, high=1.0, *, validate_args=None):
         assert isinstance(base_dist, self.supported_types)
         assert (
             base_dist.support is constraints.real
         ), "The base distribution should be univariate and have real support."
         batch_shape = lax.broadcast_shapes(
             base_dist.batch_shape, jnp.shape(low), jnp.shape(high)
         )
@@ -332,15 +332,15 @@
             )
         elif isinstance(self.base_dist, Cauchy):
             return jnp.full(self.batch_shape, jnp.nan)
         else:
             return NotImplementedError("var only available for Normal and Cauchy")
 
 
-def TruncatedDistribution(base_dist, low=None, high=None, validate_args=None):
+def TruncatedDistribution(base_dist, low=None, high=None, *, validate_args=None):
     """
     A function to generate a truncated distribution.
 
     :param base_dist: The base distribution to be truncated. This should be a univariate
         distribution. Currently, only the following distributions are supported:
         Cauchy, Laplace, Logistic, Normal, and StudentT.
     :param low: the value which is used to truncate the base distribution from below.
@@ -382,15 +382,15 @@
     num_log_prob_terms = 7
     num_gamma_variates = 8
     assert num_log_prob_terms % 2 == 1
 
     arg_constraints = {}
     support = constraints.interval(0.0, truncation_point)
 
-    def __init__(self, batch_shape=(), validate_args=None):
+    def __init__(self, batch_shape=(), *, validate_args=None):
         super(TruncatedPolyaGamma, self).__init__(
             batch_shape, validate_args=validate_args
         )
 
     def sample(self, key, sample_shape=()):
         assert is_prng_key(key)
         denom = jnp.square(jnp.arange(0.5, self.num_gamma_variates))
```

### Comparing `numpyro-0.9.1/numpyro/distributions/util.py` & `numpyro-0.9.2/numpyro/distributions/util.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/examples/datasets.py` & `numpyro-0.9.2/numpyro/examples/datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,14 +76,21 @@
 )
 
 NINE_MERS = dset(
     "9mers",
     ["https://github.com/pyro-ppl/datasets/blob/master/9mers_data.pkl?raw=true"],
 )
 
+MORTALITY = dset(
+    "mortality",
+    [
+        "https://github.com/pyro-ppl/datasets/blob/master/simulated_mortality.csv?raw=true"
+    ],
+)
+
 
 def _download(dset):
     for url in dset.urls:
         file = os.path.basename(urlparse(url).path)
         out_path = os.path.join(DATA_DIR, file)
         if not os.path.exists(out_path):
             print("Downloading - {}.".format(url))
@@ -300,14 +307,53 @@
 
 def _load_9mers():
     _download(NINE_MERS)
     file_path = os.path.join(DATA_DIR, "9mers_data.pkl")
     return pickle.load(open(file_path, "rb"))
 
 
+def _load_mortality():
+    _download(MORTALITY)
+
+    a, s1, s2, t, deaths, population = [], [], [], [], [], []
+    with open(os.path.join(DATA_DIR, "simulated_mortality.csv")) as f:
+        csv_reader = csv.DictReader(
+            f,
+            fieldnames=[
+                "age_group",
+                "year",
+                "a",
+                "s1",
+                "s2",
+                "t",
+                "deaths",
+                "population",
+            ],
+        )
+        next(csv_reader)  # skip the first row
+        for row in csv_reader:
+            a.append(int(row["a"]))
+            s1.append(int(row["s1"]))
+            s2.append(int(row["s2"]))
+            t.append(int(row["t"]))
+            deaths.append(int(row["deaths"]))
+            population.append(int(row["population"]))
+
+    return {
+        "train": (
+            np.stack(a),
+            np.stack(s1),
+            np.stack(s2),
+            np.stack(t),
+            np.stack(deaths),
+            np.stack(population),
+        )
+    }
+
+
 def _load(dset, num_datapoints=-1):
     if dset == BASEBALL:
         return _load_baseball()
     elif dset == BOSTON_HOUSING:
         return _load_boston_housing()
     elif dset == COVTYPE:
         return _load_covtype()
@@ -323,14 +369,16 @@
         return _load_lynxhare()
     elif dset == JSB_CHORALES:
         return _load_jsb_chorales()
     elif dset == HIGGS:
         return _load_higgs(num_datapoints)
     elif dset == NINE_MERS:
         return _load_9mers()
+    elif dset == MORTALITY:
+        return _load_mortality()
     raise ValueError("Dataset - {} not found.".format(dset.name))
 
 
 def iter_dataset(dset, batch_size=None, split="train", shuffle=True):
     arrays = _load(dset)[split]
     num_records = len(arrays[0])
     idxs = np.arange(num_records)
```

### Comparing `numpyro-0.9.1/numpyro/handlers.py` & `numpyro-0.9.2/numpyro/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -626,26 +626,28 @@
         ...             return numpyro.sample("x", dist.Bernoulli(0.5))
         ...
         >>> assert "a/b.x" in trace(seed(model, 0)).get_trace()
 
     :param fn: Python callable with NumPyro primitives.
     :param str prefix: a string to prepend to sample names
     :param str divider: a string to join the prefix and sample name; default to `'/'`
+    :param list hide_types: an optional list of side types to skip renaming.
     """
 
-    def __init__(self, fn=None, prefix="", divider="/"):
+    def __init__(self, fn=None, prefix="", divider="/", *, hide_types=None):
         self.prefix = prefix
         self.divider = divider
+        self.hide_types = [] if hide_types is None else hide_types
         super().__init__(fn)
 
     def process_message(self, msg):
-        if msg.get("name"):
+        if msg.get("name") and msg["type"] not in self.hide_types:
             msg["name"] = f"{self.prefix}{self.divider}{msg['name']}"
 
-        if msg.get("cond_indep_stack"):
+        if msg.get("cond_indep_stack") and "plate" not in self.hide_types:
             msg["cond_indep_stack"] = [
                 CondIndepStackFrame(
                     f"{self.prefix}{self.divider}{i.name}", i.dim, i.size
                 )
                 for i in msg["cond_indep_stack"]
             ]
```

### Comparing `numpyro-0.9.1/numpyro/infer/__init__.py` & `numpyro-0.9.2/numpyro/infer/__init__.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/infer/autoguide.py` & `numpyro-0.9.2/numpyro/infer/autoguide.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/infer/barker.py` & `numpyro-0.9.2/numpyro/infer/barker.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/infer/elbo.py` & `numpyro-0.9.2/numpyro/infer/elbo.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/infer/hmc.py` & `numpyro-0.9.2/numpyro/infer/hmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,27 +175,29 @@
         kinetic_fn = euclidean_kinetic_energy
     vv_update = None
     max_treedepth = None
     wa_update = None
     wa_steps = None
     forward_mode_ad = False
     max_delta_energy = 1000.0
+    fixed_num_steps = None
     if algo not in {"HMC", "NUTS"}:
         raise ValueError("`algo` must be one of `HMC` or `NUTS`.")
 
     def init_kernel(
         init_params,
         num_warmup,
-        *,
         step_size=1.0,
         inverse_mass_matrix=None,
         adapt_step_size=True,
         adapt_mass_matrix=True,
         dense_mass=False,
         target_accept_prob=0.8,
+        *,
+        num_steps=None,
         trajectory_length=2 * math.pi,
         max_tree_depth=10,
         find_heuristic_step_size=False,
         forward_mode_differentiation=False,
         regularize_mass_matrix=True,
         model_args=(),
         model_kwargs=None,
@@ -243,14 +245,15 @@
                 + dense_mass=[("x",), ("y",), ("z")]: use dense mass matrices for
                   each of x, y, and z (i.e. block-diagonal with 3 blocks)
 
         :type dense_mass: bool or list
         :param float target_accept_prob: Target acceptance probability for step size
             adaptation using Dual Averaging. Increasing this value will lead to a smaller
             step size, hence the sampling will be slower but more robust. Defaults to 0.8.
+        :param int num_steps: if different than None, fix the number of steps allowed for each iteration.
         :param float trajectory_length: Length of a MCMC trajectory for HMC. Default
             value is :math:`2\\pi`.
         :param int max_tree_depth: Max depth of the binary tree created during the doubling
             scheme of NUTS sampler. Defaults to 10. This argument also accepts a tuple of
             integers `(d1, d2)`, where `d1` is the max tree depth during warmup phase and
             `d2` is the max tree depth during post warmup phase.
         :param bool find_heuristic_step_size: whether to a heuristic function to adjust the
@@ -266,22 +269,23 @@
         """
         rng_key = random.PRNGKey(0) if rng_key is None else rng_key
         step_size = lax.convert_element_type(step_size, jnp.result_type(float))
         if trajectory_length is not None:
             trajectory_length = lax.convert_element_type(
                 trajectory_length, jnp.result_type(float)
             )
-        nonlocal wa_update, max_treedepth, vv_update, wa_steps, forward_mode_ad
+        nonlocal wa_update, max_treedepth, vv_update, wa_steps, forward_mode_ad, fixed_num_steps
         forward_mode_ad = forward_mode_differentiation
         wa_steps = num_warmup
         max_treedepth = (
             max_tree_depth
             if isinstance(max_tree_depth, tuple)
             else (max_tree_depth, max_tree_depth)
         )
+        fixed_num_steps = num_steps
         if isinstance(init_params, ParamInfo):
             z, pe, z_grad = init_params
         else:
             z, pe, z_grad = init_params, None, None
         pe_fn = potential_fn
         if potential_fn_gen:
             if pe_fn is not None:
@@ -347,16 +351,18 @@
         trajectory_length,
     ):
         if potential_fn_gen:
             nonlocal vv_update, forward_mode_ad
             pe_fn = potential_fn_gen(*model_args, **model_kwargs)
             _, vv_update = velocity_verlet(pe_fn, kinetic_fn, forward_mode_ad)
 
+        if fixed_num_steps is not None:
+            num_steps = fixed_num_steps
         # no need to spend too many steps if the state z has 0 size (i.e. z is empty)
-        if len(inverse_mass_matrix) == 0:
+        elif len(inverse_mass_matrix) == 0:
             num_steps = 1
         else:
             num_steps = _get_num_steps(step_size, trajectory_length)
         # makes sure trajectory length is constant, rather than step_size * num_steps
         step_size = trajectory_length / num_steps
         vv_state_new = fori_loop(
             0,
@@ -568,14 +574,15 @@
             + dense_mass=[("x",), ("y",), ("z")]: use dense mass matrices for
               each of x, y, and z (i.e. block-diagonal with 3 blocks)
 
     :type dense_mass: bool or list
     :param float target_accept_prob: Target acceptance probability for step size
         adaptation using Dual Averaging. Increasing this value will lead to a smaller
         step size, hence the sampling will be slower but more robust. Defaults to 0.8.
+    :param int num_steps: if different than None, fix the number of steps allowed for each iteration.
     :param float trajectory_length: Length of a MCMC trajectory for HMC. Default
         value is :math:`2\\pi`.
     :param callable init_strategy: a per-site initialization function.
         See :ref:`init_strategy` section for available functions.
     :param bool find_heuristic_step_size: whether or not to use a heuristic function
         to adjust the step size at the beginning of each adaptation window. Defaults
         to False.
@@ -598,27 +605,29 @@
         kinetic_fn=None,
         step_size=1.0,
         inverse_mass_matrix=None,
         adapt_step_size=True,
         adapt_mass_matrix=True,
         dense_mass=False,
         target_accept_prob=0.8,
+        num_steps=None,
         trajectory_length=2 * math.pi,
         init_strategy=init_to_uniform,
         find_heuristic_step_size=False,
         forward_mode_differentiation=False,
         regularize_mass_matrix=True,
     ):
         if not (model is None) ^ (potential_fn is None):
             raise ValueError("Only one of `model` or `potential_fn` must be specified.")
         self._model = model
         self._potential_fn = potential_fn
         self._kinetic_fn = (
             kinetic_fn if kinetic_fn is not None else euclidean_kinetic_energy
         )
+        self._num_steps = num_steps
         self._step_size = float(step_size) if isinstance(step_size, int) else step_size
         self._inverse_mass_matrix = inverse_mass_matrix
         self._adapt_step_size = adapt_step_size
         self._adapt_mass_matrix = adapt_mass_matrix
         self._dense_mass = dense_mass
         self._target_accept_prob = target_accept_prob
         self._trajectory_length = (
@@ -714,14 +723,15 @@
                 dense_mass = [tuple(sorted(z))] if dense_mass else []
             assert isinstance(dense_mass, list)
 
         hmc_init_fn = lambda init_params, rng_key: self._init_fn(  # noqa: E731
             init_params,
             num_warmup=num_warmup,
             step_size=self._step_size,
+            num_steps=self._num_steps,
             inverse_mass_matrix=inverse_mass_matrix,
             adapt_step_size=self._adapt_step_size,
             adapt_mass_matrix=self._adapt_mass_matrix,
             dense_mass=dense_mass,
             target_accept_prob=self._target_accept_prob,
             trajectory_length=self._trajectory_length,
             max_tree_depth=self._max_tree_depth,
```

### Comparing `numpyro-0.9.1/numpyro/infer/hmc_gibbs.py` & `numpyro-0.9.2/numpyro/infer/hmc_gibbs.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/infer/hmc_util.py` & `numpyro-0.9.2/numpyro/infer/hmc_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from collections import OrderedDict, namedtuple
 
 from jax import grad, jacfwd, random, value_and_grad, vmap
 from jax.flatten_util import ravel_pytree
 import jax.numpy as jnp
 from jax.scipy.linalg import solve_triangular
 from jax.scipy.special import expit
-from jax.tree_util import tree_flatten, tree_map, tree_multimap
+from jax.tree_util import tree_flatten, tree_map
 
 import numpyro.distributions as dist
 from numpyro.util import cond, identity, while_loop
 
 AdaptWindow = namedtuple("AdaptWindow", ["start", "end"])
 # XXX: we need to store rng_key here in case we use find_reasonable_step_size functionality
 HMCAdaptState = namedtuple(
@@ -285,23 +285,23 @@
         :param float step_size: Size of a single step.
         :param inverse_mass_matrix: Inverse of mass matrix, which is used to
             calculate kinetic energy.
         :param state: Current state of the integrator.
         :return: new state for the integrator.
         """
         z, r, _, z_grad = state
-        r = tree_multimap(
+        r = tree_map(
             lambda r, z_grad: r - 0.5 * step_size * z_grad, r, z_grad
         )  # r(n+1/2)
         r_grad = _kinetic_grad(kinetic_fn, inverse_mass_matrix, r)
-        z = tree_multimap(lambda z, r_grad: z + step_size * r_grad, z, r_grad)  # z(n+1)
+        z = tree_map(lambda z, r_grad: z + step_size * r_grad, z, r_grad)  # z(n+1)
         potential_energy, z_grad = _value_and_grad(
             potential_fn, z, forward_mode_differentiation
         )
-        r = tree_multimap(
+        r = tree_map(
             lambda r, z_grad: r - 0.5 * step_size * z_grad, r, z_grad
         )  # r(n+1)
         return IntegratorState(z, r, potential_energy, z_grad)
 
     return init_fn, update_fn
 
 
@@ -780,15 +780,15 @@
             trees[0].r_left,
             trees[0].z_left_grad,
             trees[1].z_right,
             trees[1].r_right,
             trees[1].z_right_grad,
         ),
     )
-    r_sum = tree_multimap(jnp.add, current_tree.r_sum, new_tree.r_sum)
+    r_sum = tree_map(jnp.add, current_tree.r_sum, new_tree.r_sum)
 
     if biased_transition:
         transition_prob = _biased_transition_kernel(current_tree, new_tree)
         turning = new_tree.turning | _is_turning(
             inverse_mass_matrix, r_left, r_right, r_sum
         )
     else:
@@ -1236,15 +1236,15 @@
     :param bool diagonal: whether to compute weights using variance or covariance, defaults to
         `False` (using covariance).
     :param jax.random.PRNGKey rng_key: source of the randomness, defaults to `jax.random.PRNGKey(0)`.
     :return: if `num_draws` is None, merges subposteriors without resampling; otherwise, returns
         a collection of `num_draws` samples with the same data structure as each subposterior.
     """
     # stack subposteriors
-    joined_subposteriors = tree_multimap(lambda *args: jnp.stack(args), *subposteriors)
+    joined_subposteriors = tree_map(lambda *args: jnp.stack(args), *subposteriors)
     # shape of joined_subposteriors: n_subs x n_samples x sample_shape
     joined_subposteriors = vmap(vmap(lambda sample: ravel_pytree(sample)[0]))(
         joined_subposteriors
     )
 
     if num_draws is not None:
         rng_key = random.PRNGKey(0) if rng_key is None else rng_key
@@ -1291,15 +1291,15 @@
        Willie Neiswanger, Chong Wang, Eric Xing
 
     :param list subposteriors: a list in which each element is a collection of samples.
     :param bool diagonal: whether to compute weights using variance or covariance, defaults to
         `False` (using covariance).
     :return: the estimated mean and variance/covariance parameters of the joined posterior
     """
-    joined_subposteriors = tree_multimap(lambda *args: jnp.stack(args), *subposteriors)
+    joined_subposteriors = tree_map(lambda *args: jnp.stack(args), *subposteriors)
     joined_subposteriors = vmap(vmap(lambda sample: ravel_pytree(sample)[0]))(
         joined_subposteriors
     )
 
     submeans = jnp.mean(joined_subposteriors, axis=1)
     if diagonal:
         weights = vmap(lambda x: 1 / jnp.var(x, ddof=1, axis=0))(joined_subposteriors)
```

### Comparing `numpyro-0.9.1/numpyro/infer/initialization.py` & `numpyro-0.9.2/numpyro/infer/initialization.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/infer/inspect.py` & `numpyro-0.9.2/numpyro/infer/inspect.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/infer/mcmc.py` & `numpyro-0.9.2/numpyro/infer/mcmc.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 from operator import attrgetter
 import os
 import warnings
 
 import numpy as np
 
 from jax import jit, lax, local_device_count, pmap, random, vmap
-from jax.core import Tracer
-from jax.interpreters.xla import DeviceArray
 import jax.numpy as jnp
-from jax.tree_util import tree_flatten, tree_map, tree_multimap
+from jax.tree_util import tree_flatten, tree_map
 
 from numpyro.diagnostics import print_summary
 from numpyro.util import cached_by, find_stack_level, fori_collect, identity
 
 __all__ = [
     "MCMCKernel",
     "MCMC",
@@ -157,15 +155,15 @@
     n = tree_flatten(xs)[0][0].shape[0]
 
     ys = []
     for i in range(n):
         x = jit(_get_value_from_index)(xs, i)
         ys.append(f(x))
 
-    return tree_multimap(lambda *args: jnp.stack(args), *ys)
+    return tree_map(lambda *args: jnp.stack(args), *ys)
 
 
 def _sample_fn_jit_args(state, sampler):
     hmc_state, args, kwargs = state
     return sampler.sample(hmc_state, args, kwargs), args, kwargs
 
 
@@ -183,21 +181,17 @@
             return x[0]
 
     return collect
 
 
 # XXX: Is there a better hash key that we can use?
 def _hashable(x):
-    # When the arguments are JITed, ShapedArray is hashable.
-    if isinstance(x, Tracer):
-        return x
-    elif isinstance(x, DeviceArray):
-        return x.copy().tobytes()
-    elif isinstance(x, (np.ndarray, jnp.ndarray)):
-        return x.tobytes()
+    # NOTE: When the arguments are JITed, ShapedArray is hashable.
+    if isinstance(x, (np.ndarray, jnp.ndarray)):
+        return id(x)
     return x
 
 
 class MCMC(object):
     """
     Provides access to Markov Chain Monte Carlo inference algorithms in NumPyro.
```

### Comparing `numpyro-0.9.1/numpyro/infer/mixed_hmc.py` & `numpyro-0.9.2/numpyro/infer/mixed_hmc.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/infer/reparam.py` & `numpyro-0.9.2/numpyro/infer/reparam.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # Copyright Contributors to the Pyro project.
 # SPDX-License-Identifier: Apache-2.0
 
 from abc import ABC, abstractmethod
 import math
 
+import numpy as np
+
+import jax
 import jax.numpy as jnp
 
 import numpyro
 import numpyro.distributions as dist
 from numpyro.distributions import biject_to, constraints
 from numpyro.distributions.util import is_identically_one, safe_normalize, sum_rightmost
 from numpyro.infer.autoguide import AutoContinuous
+from numpyro.util import not_jax_tracer
 
 
 class Reparam(ABC):
     """
     Base class for reparameterizers.
     """
 
@@ -74,19 +78,27 @@
         unchanged.
     :param shape_params: list of additional parameter names to copy unchanged from
         the centered to decentered distribution.
     :type shape_params: tuple or list
     """
 
     def __init__(self, centered=None, shape_params=()):
-        assert centered is None or isinstance(centered, (int, float))
+        assert centered is None or isinstance(
+            centered, (int, float, np.generic, np.ndarray, jnp.ndarray, jax.core.Tracer)
+        )
         assert isinstance(shape_params, (tuple, list))
         assert all(isinstance(name, str) for name in shape_params)
-        if isinstance(centered, (int, float)):
-            assert 0 <= centered and centered <= 1
+        if centered is not None:
+            is_valid = constraints.unit_interval.check(centered)
+            if not_jax_tracer(is_valid):
+                if not np.all(is_valid):
+                    raise ValueError(
+                        "`centered` argument does not satisfy `0 <= centered <= 1`."
+                    )
+
         self.centered = centered
         self.shape_params = shape_params
 
     def __call__(self, name, fn, obs):
         assert obs is None, "LocScaleReparam does not support observe statements"
         centered = self.centered
         if is_identically_one(centered):
@@ -98,16 +110,20 @@
         params = {key: getattr(fn, key) for key in self.shape_params}
         if self.centered is None:
             centered = numpyro.param(
                 "{}_centered".format(name),
                 jnp.full(event_shape, 0.5),
                 constraint=constraints.unit_interval,
             )
-        params["loc"] = fn.loc * centered
-        params["scale"] = fn.scale**centered
+        if isinstance(centered, (int, float, np.generic)) and centered == 0.0:
+            params["loc"] = jnp.zeros_like(fn.loc)
+            params["scale"] = jnp.ones_like(fn.scale)
+        else:
+            params["loc"] = fn.loc * centered
+            params["scale"] = fn.scale**centered
         decentered_fn = self._wrap(type(fn)(**params), expand_shape, event_dim)
 
         # Draw decentered noise.
         decentered_value = numpyro.sample("{}_decentered".format(name), decentered_fn)
 
         # Differentiably transform.
         delta = decentered_value - centered * fn.loc
```

### Comparing `numpyro-0.9.1/numpyro/infer/sa.py` & `numpyro-0.9.2/numpyro/infer/sa.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/infer/svi.py` & `numpyro-0.9.2/numpyro/infer/svi.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/infer/util.py` & `numpyro-0.9.2/numpyro/infer/util.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/nn/auto_reg_nn.py` & `numpyro-0.9.2/numpyro/nn/auto_reg_nn.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/nn/block_neural_arn.py` & `numpyro-0.9.2/numpyro/nn/block_neural_arn.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/nn/masked_dense.py` & `numpyro-0.9.2/numpyro/nn/masked_dense.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/ops/indexing.py` & `numpyro-0.9.2/numpyro/ops/indexing.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/ops/provenance.py` & `numpyro-0.9.2/numpyro/ops/provenance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright Contributors to the Pyro project.
 # SPDX-License-Identifier: Apache-2.0
 
 import jax
 from jax.interpreters import partial_eval
 from jax.linear_util import wrap_init
+import jax.numpy as jnp
 
 
 class _ProvenanceJaxprTrace(partial_eval.DynamicJaxprTrace):
     """A JAX class to control the behavior of primitives on tracers."""
 
     def process_primitive(self, primitive, tracers, params):
         # remove "_provenance" dimension in arguments before executing the function
@@ -64,16 +65,16 @@
 
     :param data: An initial data to start tracking. The data needs
         to have attributes `shape` and `dtype`.
     :param frozenset provenance: An initial provenance set.
     """
 
     def __init__(self, data, provenance=frozenset()):
-        self.shape = data.shape
-        self.dtype = data.dtype
+        self.shape = jnp.shape(data)
+        self.dtype = jnp.result_type(data)
         self.named_shape = {"_provenance": provenance}
 
 
 def get_provenance(data):
     """
     Reads the provenance of a recursive datastructure possibly containing ndarray.
```

### Comparing `numpyro-0.9.1/numpyro/ops/pytree.py` & `numpyro-0.9.2/numpyro/ops/pytree.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class PytreeTrace:
     def __init__(self, trace):
         self.trace = trace
 
     def tree_flatten(self):
         trace, aux_trace = {}, {}
         for name, site in self.trace.items():
-            if site["type"] in ["sample", "deterministic", "plate"]:
+            if site["type"] in ["sample", "deterministic", "plate", "param"]:
                 trace[name], aux_trace[name] = {}, {"_control_flow_done": True}
                 for key in site:
                     if key == "fn":
                         if site["type"] == "sample":
                             trace[name][key] = site[key]
                         elif site["type"] == "plate":
                             aux_trace[name][key] = site[key]
```

### Comparing `numpyro-0.9.1/numpyro/optim.py` & `numpyro-0.9.2/numpyro/optim.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/patch.py` & `numpyro-0.9.2/numpyro/patch.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro/primitives.py` & `numpyro-0.9.2/numpyro/primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,15 +597,15 @@
     probabilistic model.
 
     :param str name: Name of the trivial sample.
     :param numpy.ndarray log_factor: A possibly batched log probability factor.
     """
     unit_dist = numpyro.distributions.distribution.Unit(log_factor)
     unit_value = unit_dist.sample(None)
-    sample(name, unit_dist, obs=unit_value)
+    sample(name, unit_dist, obs=unit_value, infer={"is_auxiliary": True})
 
 
 def prng_key():
     """
     A statement to draw a pseudo-random number generator key
     :func:`~jax.random.PRNGKey` under :class:`~numpyro.handlers.seed` handler.
```

### Comparing `numpyro-0.9.1/numpyro/util.py` & `numpyro-0.9.2/numpyro/util.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/numpyro.egg-info/PKG-INFO` & `numpyro-0.9.2/numpyro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numpyro
-Version: 0.9.1
+Version: 0.9.2
 Summary: Pyro PPL on NumPy
 Home-page: https://github.com/pyro-ppl/numpyro
 Author: Uber AI Labs
 License: Apache License 2.0
 Keywords: probabilistic machine learning bayesian statistics
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `numpyro-0.9.1/numpyro.egg-info/SOURCES.txt` & `numpyro-0.9.2/numpyro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/setup.cfg` & `numpyro-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/setup.py` & `numpyro-0.9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             "scipy>=1.6,<1.7",
         ],
         "dev": [
             "dm-haiku",
             "flax",
             "funsor>=0.4.1",
             "graphviz",
-            "jaxns==0.0.7",
+            "jaxns==1.0.0",
             "optax>=0.0.6",
             "tensorflow_probability>=0.15.0",
         ],
         "examples": [
             "arviz",
             "jupyter",
             "matplotlib",
```

### Comparing `numpyro-0.9.1/test/test_compile.py` & `numpyro-0.9.2/test/test_compile.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/test/test_diagnostics.py` & `numpyro-0.9.2/test/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/test/test_distributions.py` & `numpyro-0.9.2/test/test_distributions.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,21 +10,26 @@
 import numpy as np
 from numpy.testing import assert_allclose, assert_array_equal
 import pytest
 import scipy
 import scipy.stats as osp
 
 import jax
-from jax import grad, lax, vmap
+from jax import grad, lax, tree_map, vmap
 import jax.numpy as jnp
 import jax.random as random
 from jax.scipy.special import expit, logsumexp
 
 import numpyro.distributions as dist
-from numpyro.distributions import constraints, kl_divergence, transforms
+from numpyro.distributions import (
+    SineBivariateVonMises,
+    constraints,
+    kl_divergence,
+    transforms,
+)
 from numpyro.distributions.discrete import _to_probs_bernoulli, _to_probs_multinom
 from numpyro.distributions.flows import InverseAutoregressiveTransform
 from numpyro.distributions.gof import InvalidTest, auto_goodness_of_fit
 from numpyro.distributions.transforms import (
     LowerCholeskyAffine,
     PermuteTransform,
     PowerTransform,
@@ -771,15 +776,15 @@
 )
 @pytest.mark.parametrize("prepend_shape", [(), (2,), (2, 3)])
 def test_dist_shape(jax_dist, sp_dist, params, prepend_shape):
     jax_dist = jax_dist(*params)
     rng_key = random.PRNGKey(0)
     expected_shape = prepend_shape + jax_dist.batch_shape + jax_dist.event_shape
     samples = jax_dist.sample(key=rng_key, sample_shape=prepend_shape)
-    assert isinstance(samples, jax.interpreters.xla.DeviceArray)
+    assert isinstance(samples, jnp.ndarray)
     assert jnp.shape(samples) == expected_shape
     if (
         sp_dist
         and not _is_batched_multivariate(jax_dist)
         and not isinstance(jax_dist, dist.MultivariateStudentT)
     ):
         sp_dist = sp_dist(*params)
@@ -870,14 +875,15 @@
 
 @pytest.mark.parametrize("jax_dist, sp_dist, params", CONTINUOUS)
 def test_sample_gradient(jax_dist, sp_dist, params):
     # we have pathwise gradient for gamma sampler
     gamma_derived_params = {
         "Gamma": ["concentration"],
         "Beta": ["concentration1", "concentration0"],
+        "BetaProportion": ["mean", "concentration"],
         "Chi2": ["df"],
         "Dirichlet": ["concentration"],
         "InverseGamma": ["concentration"],
         "LKJ": ["concentration"],
         "LKJCholesky": ["concentration"],
         "StudentT": ["df"],
     }.get(jax_dist.__name__, [])
@@ -1037,15 +1043,15 @@
     try:
         expected = sp_dist.logpdf(samples)
     except AttributeError:
         expected = sp_dist.logpmf(samples)
     except ValueError as e:
         # precision issue: jnp.sum(x / jnp.sum(x)) = 0.99999994 != 1
         if "The input vector 'x' must lie within the normal simplex." in str(e):
-            samples = samples.copy().astype("float64")
+            samples = jax.device_get(samples).astype("float64")
             samples = samples / samples.sum(axis=-1, keepdims=True)
             expected = sp_dist.logpdf(samples)
         else:
             raise e
     assert_allclose(jit_fn(jax_dist.log_prob)(samples), expected, atol=1e-5)
 
 
@@ -1812,15 +1818,15 @@
 
     # test codomain
     batch_shape = shape if event_dim == 0 else shape[:-1]
     assert_array_equal(transform.codomain(y), jnp.ones(batch_shape, dtype=jnp.bool_))
 
     # test inv
     z = transform.inv(y)
-    assert_allclose(x, z, atol=1e-6, rtol=1e-6)
+    assert_allclose(x, z, atol=1e-5, rtol=1e-5)
 
     # test domain, currently all is constraints.real or constraints.real_vector
     assert_array_equal(transform.domain(z), jnp.ones(batch_shape))
 
     # test log_abs_det_jacobian
     actual = transform.log_abs_det_jacobian(x, y)
     assert jnp.shape(actual) == batch_shape
@@ -1877,16 +1883,16 @@
 
             expected = np.linalg.slogdet(jax.jacobian(vec_transform)(x))[1]
             inv_expected = np.linalg.slogdet(jax.jacobian(inv_vec_transform)(y_tril))[1]
         else:
             expected = jnp.log(jnp.abs(grad(transform)(x)))
             inv_expected = jnp.log(jnp.abs(grad(transform.inv)(y)))
 
-        assert_allclose(actual, expected, atol=1e-6, rtol=1e-6)
-        assert_allclose(actual, -inv_expected, atol=1e-6, rtol=1e-6)
+        assert_allclose(actual, expected, atol=1e-5, rtol=1e-5)
+        assert_allclose(actual, -inv_expected, atol=1e-5, rtol=1e-5)
 
 
 # NB: skip transforms which are tested in `test_biject_to`
 @pytest.mark.parametrize(
     "transform, event_shape",
     [
         (PermuteTransform(np.array([3, 0, 4, 1, 2])), (5,)),
@@ -2200,14 +2206,29 @@
     base_dist = dist.Normal(loc, 0.1).to_event(event_dim)
     expanded_dist = base_dist.expand(expand_shape[: len(expand_shape) - event_dim])
     samples = expanded_dist.sample(random.PRNGKey(1), sample_shape)
     expected_mean = jnp.broadcast_to(loc, sample_shape[1:] + expanded_dist.shape())
     assert_allclose(samples.mean(0), expected_mean, atol=0.1)
 
 
+@pytest.mark.parametrize("batch_shape", [(), (4,), (10, 3)])
+def test_sine_bivariate_von_mises_batch_shape(batch_shape):
+    phi_loc = jnp.broadcast_to(jnp.array(0.0), batch_shape)
+    psi_loc = jnp.array(0.0)
+    phi_conc = jnp.array(1.0)
+    psi_conc = jnp.array(1.0)
+    corr = jnp.array(0.1)
+
+    sine = SineBivariateVonMises(phi_loc, psi_loc, phi_conc, psi_conc, corr)
+    assert sine.batch_shape == batch_shape
+
+    samples = sine.sample(random.PRNGKey(0))
+    assert samples.shape == (*batch_shape, 2)
+
+
 @pytest.mark.parametrize("batch_shape", [(), (4,)])
 def test_polya_gamma(batch_shape, num_points=20000):
     d = dist.TruncatedPolyaGamma(batch_shape=batch_shape)
     rng_key = random.PRNGKey(0)
 
     # test density approximately normalized
     x = jnp.linspace(1.0e-6, d.truncation_point, num_points)
@@ -2311,15 +2332,15 @@
 
 
 def test_expand_pytree():
     def g(x):
         return dist.Normal(x, 1).expand([10, 3])
 
     assert lax.map(g, jnp.ones((5, 3))).batch_shape == (5, 10, 3)
-    assert jax.tree_map(lambda x: x[None], g(0)).batch_shape == (1, 10, 3)
+    assert tree_map(lambda x: x[None], g(0)).batch_shape == (1, 10, 3)
 
 
 @pytest.mark.parametrize("batch_shape", [(), (4,), (2, 3)], ids=str)
 def test_kl_delta_normal_shape(batch_shape):
     v = np.random.normal(size=batch_shape)
     loc = np.random.normal(size=batch_shape)
     scale = np.exp(np.random.normal(size=batch_shape))
```

### Comparing `numpyro-0.9.1/test/test_distributions_mixture.py` & `numpyro-0.9.2/test/test_distributions_mixture.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/test/test_distributions_util.py` & `numpyro-0.9.2/test/test_distributions_util.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/test/test_example_utils.py` & `numpyro-0.9.2/test/test_example_utils.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/test/test_examples.py` & `numpyro-0.9.2/test/test_examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     "hmm_enum.py -m 3 -t 3 -d 3 --num-warmup 1 -n 4",
     "hmm_enum.py -m 3 -t 3 -d 4 --num-warmup 1 -n 4",
     "hmm_enum.py -m 4 -t 3 -d 4 --num-warmup 1 -n 4",
     "hmm_enum.py -m 6 -t 4 -d 3 --num-warmup 1 -n 4",
     "horseshoe_regression.py --num-samples 10 --num-warmup 10 --num-data 5",
     "hsgp.py --num-samples 10 --num-warmup 10 --num-chains 2",
     "minipyro.py",
+    "mortality.py --num-samples 10 --num-warmup 10 --num-chains 2",
     "neutra.py --num-samples 100 --num-warmup 100",
     "ode.py --num-samples 100 --num-warmup 100 --num-chains 1",
     pytest.param(
         "prodlda.py --num-steps 10 --hidden 10 --nn-framework flax",
         marks=pytest.mark.skipif(
             "CI" in os.environ, reason="This example requires a lot of memory."
         ),
```

### Comparing `numpyro-0.9.1/test/test_flows.py` & `numpyro-0.9.2/test/test_flows.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/test/test_handlers.py` & `numpyro-0.9.2/test/test_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright Contributors to the Pyro project.
 # SPDX-License-Identifier: Apache-2.0
 
 import numpy as np
 from numpy.testing import assert_allclose, assert_raises
 import pytest
 
-from jax import jit, random, tree_multimap, value_and_grad, vmap
+import jax
+from jax import jit, random, tree_map, value_and_grad, vmap
 import jax.numpy as jnp
 
 import numpyro
 from numpyro import handlers
 import numpyro.distributions as dist
 from numpyro.distributions import constraints
 from numpyro.infer import MCMC, NUTS, SVI, Trace_ELBO
@@ -430,15 +431,15 @@
         )(params)
         subsample = jnp.array([1])
         loss2, grads2 = value_and_grad(
             lambda x: svi.loss.loss(
                 svi_state.rng_key, svi.constrain_fn(x), svi.model, svi.guide, subsample
             )
         )(params)
-        grads = tree_multimap(lambda *vals: vals[0] + vals[1], grads1, grads2)
+        grads = tree_map(lambda *vals: vals[0] + vals[1], grads1, grads2)
         loss = loss1 + loss2
     else:
         subsample = jnp.array([0, 1])
         loss, grads = value_and_grad(
             lambda x: svi.loss.loss(
                 svi_state.rng_key, svi.constrain_fn(x), svi.model, svi.guide, subsample
             )
@@ -573,26 +574,26 @@
             with handlers.seed(rng_seed=0):
                 numpyro.sample("x", dist.Normal())
     assert "x" not in trace
 
 
 def test_scope():
     def fn():
-        return numpyro.sample("x", dist.Normal())
+        with numpyro.plate("N", 10):
+            return numpyro.sample("x", dist.Normal())
 
     with handlers.trace() as trace:
         with handlers.seed(rng_seed=1):
             with handlers.scope(prefix="a"):
                 fn()
             with handlers.scope(prefix="b"):
-                with handlers.scope(prefix="a"):
+                with handlers.scope(prefix="a", hide_types=["plate"]):
                     fn()
 
-    assert "a/x" in trace
-    assert "b/a/x" in trace
+    assert set(trace) == {"a/x", "b/a/x", "a/N", "b/N"}
 
 
 def test_scope_frames():
     def model(y):
         mu = numpyro.sample("mu", dist.Normal())
         sigma = numpyro.sample("sigma", dist.HalfNormal())
 
@@ -773,15 +774,15 @@
         assert_allclose(
             jnp.mean(subsamples == i, axis=0),
             jnp.full(subsample_size, 1 / size),
             atol=1e-3,
         )
 
         # test that values are not duplicated
-        assert len(set(subsamples[k].copy())) == subsample_size
+        assert len(set(jax.device_get(subsamples[k]))) == subsample_size
 
 
 def test_sites_have_unique_names():
     def model():
         alpha = numpyro.sample("alpha", dist.Normal())
         numpyro.deterministic("alpha", alpha * 2)
```

### Comparing `numpyro-0.9.1/test/test_model_rendering.py` & `numpyro-0.9.2/test/test_model_rendering.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/test/test_nn.py` & `numpyro-0.9.2/test/test_nn.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/test/test_optimizers.py` & `numpyro-0.9.2/test/test_optimizers.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         (optim.Momentum, (1e-2, 0.5), {}),
         (optim.RMSProp, (1e-2, 0.95), {}),
         (optim.RMSPropMomentum, (1e-4,), {}),
         (optim.SGD, (1e-2,), {}),
     ]
     + optax_optimizers,
 )
+@pytest.mark.filterwarnings("ignore:.*tree_multimap:FutureWarning")
 def test_optim_multi_params(optim_class, args, kwargs):
     params = {"x": jnp.array([1.0, 1.0, 1.0]), "y": jnp.array([-1, -1.0, -1.0])}
     opt = optim_class(*args, **kwargs)
     if not isinstance(opt, optim._NumPyroOptim):
         opt = optim.optax_to_numpyro(opt)
     opt_state = opt.init(params)
     for i in range(2000):
@@ -80,14 +81,15 @@
         (optim.Momentum, (1e-2, 0.5), {}),
         (optim.RMSProp, (1e-2, 0.95), {}),
         (optim.RMSPropMomentum, (1e-4,), {}),
         (optim.SGD, (1e-2,), {}),
     ]
     + optax_optimizers,
 )
+@pytest.mark.filterwarnings("ignore:.*tree_multimap:FutureWarning")
 def test_numpyrooptim_no_double_jit(optim_class, args, kwargs):
 
     opt = optim_class(*args, **kwargs)
     if not isinstance(opt, optim._NumPyroOptim):
         opt = optim.optax_to_numpyro(opt)
     state = opt.init(jnp.zeros(10))
```

### Comparing `numpyro-0.9.1/test/test_pickle.py` & `numpyro-0.9.2/test/test_pickle.py`

 * *Files identical despite different names*

### Comparing `numpyro-0.9.1/test/test_util.py` & `numpyro-0.9.2/test/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from numpy.testing import assert_allclose
 import pytest
 
 from jax import random
 from jax.flatten_util import ravel_pytree
 import jax.numpy as jnp
 from jax.test_util import check_eq
-from jax.tree_util import tree_flatten, tree_multimap
+from jax.tree_util import tree_flatten, tree_map
 
 import numpyro
 import numpyro.distributions as dist
 from numpyro.util import check_model_guide_match, fori_collect, format_shapes, soft_vmap
 
 
 def test_fori_collect_thinning():
@@ -78,18 +78,18 @@
         {"a": False, "b": np.array([[1.0, 2.0], [3.0, 4.0]])},
         [False, True, 0.0, np.array([[1.0, 2.0], [3.0, 4.0]])],
     ],
 )
 def test_ravel_pytree(pytree):
     flat, unravel_fn = ravel_pytree(pytree)
     unravel = unravel_fn(flat)
-    tree_flatten(tree_multimap(lambda x, y: assert_allclose(x, y), unravel, pytree))
+    tree_flatten(tree_map(lambda x, y: assert_allclose(x, y), unravel, pytree))
     assert all(
         tree_flatten(
-            tree_multimap(
+            tree_map(
                 lambda x, y: jnp.result_type(x) == jnp.result_type(y), unravel, pytree
             )
         )[0]
     )
 
 
 @pytest.mark.parametrize("batch_shape", [(), (1,), (10,), (3, 4)])
```

