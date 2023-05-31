# Comparing `tmp/beansp-1.0.1.tar.gz` & `tmp/beansp-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beansp-1.0.1.tar", last modified: Thu May 18 13:05:25 2023, max compression
+gzip compressed data, was "beansp-1.4.3.tar", last modified: Wed May 31 15:06:38 2023, max compression
```

## Comparing `beansp-1.0.1.tar` & `beansp-1.4.3.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-18 13:05:25.644700 beansp-1.0.1/
--rw-rw-r--   0 duncan     (504) staff       (20)     3622 2020-07-28 03:51:27.000000 beansp-1.0.1/CONTRIBUTING.rst
--rw-rw-r--   0 duncan     (504) staff       (20)       89 2020-07-28 03:51:27.000000 beansp-1.0.1/HISTORY.rst
--rw-rw-r--   0 duncan     (504) staff       (20)     1073 2020-07-28 03:51:27.000000 beansp-1.0.1/LICENSE
--rw-rw-r--   0 duncan     (504) staff       (20)      284 2023-03-30 03:04:22.000000 beansp-1.0.1/MANIFEST.in
--rw-rw-r--   0 duncan     (504) staff       (20)     3093 2023-05-18 13:05:25.644793 beansp-1.0.1/PKG-INFO
--rw-rw-r--   0 duncan     (504) staff       (20)     2270 2023-04-09 12:34:34.000000 beansp-1.0.1/README.rst
-drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-18 13:05:25.611422 beansp-1.0.1/beansp/
--rw-rw-r--   0 duncan     (504) staff       (20)      418 2023-05-18 10:07:21.000000 beansp-1.0.1/beansp/__init__.py
--rw-rw-r--   0 duncan     (504) staff       (20)     2152 2023-03-30 03:04:22.000000 beansp-1.0.1/beansp/analyse.py
--rw-rw-r--   0 duncan     (504) staff       (20)    53892 2023-05-18 09:33:33.000000 beansp-1.0.1/beansp/beans.py
--rw-rw-r--   0 duncan     (504) staff       (20)    18244 2023-03-30 03:04:22.000000 beansp-1.0.1/beansp/burstrain.py
-drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-18 13:05:25.615822 beansp-1.0.1/beansp/data/
--rw-rw-r--   0 duncan     (504) staff       (20)      903 2023-03-30 03:04:22.000000 beansp-1.0.1/beansp/data/1731_bursts_avg.txt
--rw-rw-r--   0 duncan     (504) staff       (20)     1285 2023-03-30 03:04:22.000000 beansp-1.0.1/beansp/data/17498_bursts.txt
-drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-18 13:05:25.627524 beansp-1.0.1/beansp/data/17498_data/
--rw-rw-r--   0 duncan     (504) staff       (20)      302 2023-03-30 03:04:22.000000 beansp-1.0.1/beansp/data/17498_data/17498_bursts_new.txt
--rw-rw-r--   0 duncan     (504) staff       (20)     6190 2023-03-30 03:04:22.000000 beansp-1.0.1/beansp/data/17498_data/17498_gti.txt
--rw-rw-r--   0 duncan     (504) staff       (20)     3338 2023-03-30 03:04:22.000000 beansp-1.0.1/beansp/data/17498_data/17498_obs_new.txt
--rw-rw-r--   0 duncan     (504) staff       (20)      776 2023-03-30 03:04:22.000000 beansp-1.0.1/beansp/data/17498_data/run_17498.py
--rw-rw-r--   0 duncan     (504) staff       (20)     3016 2023-03-30 03:04:22.000000 beansp-1.0.1/beansp/data/17498_obs.txt
-drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-18 13:05:25.627927 beansp-1.0.1/beansp/data/17511/
--rw-rw-r--   0 duncan     (504) staff       (20)     1230 2023-03-30 03:04:22.000000 beansp-1.0.1/beansp/data/17511/test2_parameterconstraints_pred.txt
--rw-rw-r--   0 duncan     (504) staff       (20)     1230 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/17511/test3_parameterconstraints_pred.txt
--rw-rw-r--   0 duncan     (504) staff       (20)     1401 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/17511_bursts.txt
--rw-rw-r--   0 duncan     (504) staff       (20)     9378 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/17511_gti.dat
--rw-rw-r--   0 duncan     (504) staff       (20)     2699 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/17511_obs.txt
-drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-18 13:05:25.629649 beansp-1.0.1/beansp/data/1808/
--rw-rw-r--   0 duncan     (504) staff       (20)     1096 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/1808/test1_parameterconstraints_pred.txt
--rw-rw-r--   0 duncan     (504) staff       (20)     1096 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/1808/test2_parameterconstraints_pred.txt
--rw-rw-r--   0 duncan     (504) staff       (20)     1096 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/1808/test4_parameterconstraints_pred.txt
--rw-rw-r--   0 duncan     (504) staff       (20)      978 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/1808/test5_parameterconstraints_pred.txt
--rw-rw-r--   0 duncan     (504) staff       (20)     1230 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/1808/test6_parameterconstraints_pred.txt
--rw-rw-r--   0 duncan     (504) staff       (20)     1230 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/1808/test7_parameterconstraints_pred.txt
--rw-rw-r--   0 duncan     (504) staff       (20)      100 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/1808/test_acceptancefraction.txt
--rw-rw-r--   0 duncan     (504) staff       (20)     1098 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/1808_bursts.txt
--rw-rw-r--   0 duncan     (504) staff       (20)   382126 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/1808_example_burstsfromminbar.png
--rw-rw-r--   0 duncan     (504) staff       (20)     3588 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/1808_gti.txt
--rw-rw-r--   0 duncan     (504) staff       (20)     1647 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/1808_obs.txt
--rw-rw-r--   0 duncan     (504) staff       (20)      999 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/1826_bursts.txt
--rw-rw-r--   0 duncan     (504) staff       (20)      281 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/beans.ini
--rw-rw-r--   0 duncan     (504) staff       (20)   342452 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/example_1808_pfluxfromminbar.png
--rw-rw-r--   0 duncan     (504) staff       (20)     4862 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/data/mr_prior_fit.txt
--rw-rw-r--   0 duncan     (504) staff       (20)     1046 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/get_alphas.py
--rw-rw-r--   0 duncan     (504) staff       (20)     8243 2023-05-18 09:33:33.000000 beansp-1.0.1/beansp/get_data.py
--rw-rw-r--   0 duncan     (504) staff       (20)     2662 2023-05-18 09:33:33.000000 beansp-1.0.1/beansp/initialise.py
--rw-rw-r--   0 duncan     (504) staff       (20)     1004 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/mrprior.py
--rw-rw-r--   0 duncan     (504) staff       (20)     5943 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/run_emcee.py
--rw-rw-r--   0 duncan     (504) staff       (20)     9174 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/run_model.py
--rw-rw-r--   0 duncan     (504) staff       (20)      682 2023-03-30 03:04:23.000000 beansp-1.0.1/beansp/settle.py
-drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-18 13:05:25.612493 beansp-1.0.1/beansp.egg-info/
--rw-rw-r--   0 duncan     (504) staff       (20)     3093 2023-05-18 13:05:25.000000 beansp-1.0.1/beansp.egg-info/PKG-INFO
--rw-rw-r--   0 duncan     (504) staff       (20)     2033 2023-05-18 13:05:25.000000 beansp-1.0.1/beansp.egg-info/SOURCES.txt
--rw-rw-r--   0 duncan     (504) staff       (20)        1 2023-05-18 13:05:25.000000 beansp-1.0.1/beansp.egg-info/dependency_links.txt
--rw-rw-r--   0 duncan     (504) staff       (20)        1 2023-03-30 03:06:21.000000 beansp-1.0.1/beansp.egg-info/not-zip-safe
--rw-rw-r--   0 duncan     (504) staff       (20)       98 2023-05-18 13:05:25.000000 beansp-1.0.1/beansp.egg-info/requires.txt
--rw-rw-r--   0 duncan     (504) staff       (20)        7 2023-05-18 13:05:25.000000 beansp-1.0.1/beansp.egg-info/top_level.txt
-drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-18 13:05:25.631484 beansp-1.0.1/docs/
--rwxrwxr-x   0 duncan     (504) staff       (20)     5333 2020-07-28 03:51:27.000000 beansp-1.0.1/docs/conf.py
--rw-rw-r--   0 duncan     (504) staff       (20)       33 2020-07-28 03:51:27.000000 beansp-1.0.1/docs/contributing.rst
--rw-rw-r--   0 duncan     (504) staff       (20)        1 2020-07-28 03:51:27.000000 beansp-1.0.1/docs/history.rst
--rw-rw-r--   0 duncan     (504) staff       (20)      770 2020-07-28 03:51:27.000000 beansp-1.0.1/docs/index.rst
--rw-rw-r--   0 duncan     (504) staff       (20)     2454 2022-05-10 01:28:21.000000 beansp-1.0.1/docs/installation.rst
--rw-rw-r--   0 duncan     (504) staff       (20)       27 2020-07-28 03:51:27.000000 beansp-1.0.1/docs/readme.rst
--rw-rw-r--   0 duncan     (504) staff       (20)    10694 2020-07-28 03:53:36.000000 beansp-1.0.1/docs/usage.rst
--rw-rw-r--   0 duncan     (504) staff       (20)      117 2023-05-18 13:05:25.645073 beansp-1.0.1/setup.cfg
--rw-rw-r--   0 duncan     (504) staff       (20)     2144 2023-05-18 09:33:15.000000 beansp-1.0.1/setup.py
-drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-18 13:05:25.634107 beansp-1.0.1/tests/
--rw-rw-r--   0 duncan     (504) staff       (20)     1141 2023-03-30 03:04:23.000000 beansp-1.0.1/tests/README.rst
--rw-rw-r--   0 duncan     (504) staff       (20)       60 2020-07-28 03:51:27.000000 beansp-1.0.1/tests/__init__.py
-drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-18 13:05:25.643835 beansp-1.0.1/tests/data/
-drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-18 13:05:25.644384 beansp-1.0.1/tests/data/benchmark/
--rw-rw-r--   0 duncan     (504) staff       (20)     3716 2023-03-30 03:04:23.000000 beansp-1.0.1/tests/data/benchmark/settle_expected_result.ecsv
--rw-rw-r--   0 duncan     (504) staff       (20)     7499 2023-03-30 03:04:23.000000 beansp-1.0.1/tests/data/benchmark/table1.mrt
--rw-rw-r--   0 duncan     (504) staff       (20)   639200 2023-03-30 03:19:20.000000 beansp-1.0.1/tests/data/dummy.h5
--rw-rw-r--   0 duncan     (504) staff       (20)      482 2023-03-30 03:18:52.000000 beansp-1.0.1/tests/data/dummy.ini
--rw-rw-r--   0 duncan     (504) staff       (20)     3741 2023-05-18 10:20:25.000000 beansp-1.0.1/tests/data/multiprocessing.ecsv
--rw-rw-r--   0 duncan     (504) staff       (20)     3741 2023-05-18 10:20:06.000000 beansp-1.0.1/tests/data/serial.ecsv
--rw-rw-r--   0 duncan     (504) staff       (20)      603 2020-07-28 03:51:27.000000 beansp-1.0.1/tests/test_beans.py
--rw-rw-r--   0 duncan     (504) staff       (20)    10918 2023-04-09 12:34:34.000000 beansp-1.0.1/tests/test_benchmark_settle.py
--rw-rw-r--   0 duncan     (504) staff       (20)      169 2020-07-28 03:51:27.000000 beansp-1.0.1/tests/test_burstrain.py
--rw-rw-r--   0 duncan     (504) staff       (20)     1272 2023-05-18 10:18:29.000000 beansp-1.0.1/tests/test_get_data.py
--rw-rw-r--   0 duncan     (504) staff       (20)      435 2023-04-09 12:34:34.000000 beansp-1.0.1/tests/test_likelihood.py
--rw-rw-r--   0 duncan     (504) staff       (20)     2150 2023-05-18 10:19:59.000000 beansp-1.0.1/tests/test_runmodel.py
--rw-rw-r--   0 duncan     (504) staff       (20)      603 2023-03-30 03:04:23.000000 beansp-1.0.1/tests/test_settle.py
--rwxrwxr-x   0 duncan     (504) staff       (20)     1351 2023-05-18 09:33:15.000000 beansp-1.0.1/tests/test_sft_beans.py
+drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-31 15:06:38.221928 beansp-1.4.3/
+-rw-rw-r--   0 duncan     (504) staff       (20)     3622 2020-07-28 03:51:27.000000 beansp-1.4.3/CONTRIBUTING.rst
+-rw-rw-r--   0 duncan     (504) staff       (20)       89 2020-07-28 03:51:27.000000 beansp-1.4.3/HISTORY.rst
+-rw-rw-r--   0 duncan     (504) staff       (20)     1073 2020-07-28 03:51:27.000000 beansp-1.4.3/LICENSE
+-rw-rw-r--   0 duncan     (504) staff       (20)      284 2023-03-30 03:04:22.000000 beansp-1.4.3/MANIFEST.in
+-rw-rw-r--   0 duncan     (504) staff       (20)     3073 2023-05-31 15:06:38.222020 beansp-1.4.3/PKG-INFO
+-rw-rw-r--   0 duncan     (504) staff       (20)     2250 2023-05-29 06:54:34.000000 beansp-1.4.3/README.rst
+drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-31 15:06:38.155228 beansp-1.4.3/beansp/
+-rw-rw-r--   0 duncan     (504) staff       (20)      418 2023-05-31 14:16:49.000000 beansp-1.4.3/beansp/__init__.py
+-rw-rw-r--   0 duncan     (504) staff       (20)     2537 2023-05-24 15:46:49.000000 beansp-1.4.3/beansp/analyse.py
+-rw-rw-r--   0 duncan     (504) staff       (20)    58645 2023-05-31 14:15:25.000000 beansp-1.4.3/beansp/beans.py
+-rw-rw-r--   0 duncan     (504) staff       (20)    18670 2023-05-25 12:59:26.000000 beansp-1.4.3/beansp/burstrain.py
+drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-31 15:06:38.170926 beansp-1.4.3/beansp/data/
+-rw-rw-r--   0 duncan     (504) staff       (20)      903 2023-03-30 03:04:22.000000 beansp-1.4.3/beansp/data/1731_bursts_avg.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)     1285 2023-03-30 03:04:22.000000 beansp-1.4.3/beansp/data/17498_bursts.txt
+drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-31 15:06:38.171712 beansp-1.4.3/beansp/data/17498_data/
+-rw-rw-r--   0 duncan     (504) staff       (20)      302 2023-03-30 03:04:22.000000 beansp-1.4.3/beansp/data/17498_data/17498_bursts_new.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)     6190 2023-03-30 03:04:22.000000 beansp-1.4.3/beansp/data/17498_data/17498_gti.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)     3338 2023-03-30 03:04:22.000000 beansp-1.4.3/beansp/data/17498_data/17498_obs_new.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)      776 2023-03-30 03:04:22.000000 beansp-1.4.3/beansp/data/17498_data/run_17498.py
+-rw-rw-r--   0 duncan     (504) staff       (20)     3016 2023-03-30 03:04:22.000000 beansp-1.4.3/beansp/data/17498_obs.txt
+drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-31 15:06:38.172100 beansp-1.4.3/beansp/data/17511/
+-rw-rw-r--   0 duncan     (504) staff       (20)     1230 2023-03-30 03:04:22.000000 beansp-1.4.3/beansp/data/17511/test2_parameterconstraints_pred.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)     1230 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/17511/test3_parameterconstraints_pred.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)     1401 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/17511_bursts.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)     9378 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/17511_gti.dat
+-rw-rw-r--   0 duncan     (504) staff       (20)     2699 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/17511_obs.txt
+drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-31 15:06:38.173344 beansp-1.4.3/beansp/data/1808/
+-rw-rw-r--   0 duncan     (504) staff       (20)     1096 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/1808/test1_parameterconstraints_pred.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)     1096 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/1808/test2_parameterconstraints_pred.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)     1096 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/1808/test4_parameterconstraints_pred.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)      978 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/1808/test5_parameterconstraints_pred.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)     1230 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/1808/test6_parameterconstraints_pred.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)     1230 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/1808/test7_parameterconstraints_pred.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)      100 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/1808/test_acceptancefraction.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)     1098 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/1808_bursts.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)   382126 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/1808_example_burstsfromminbar.png
+-rw-rw-r--   0 duncan     (504) staff       (20)     3588 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/1808_gti.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)     1647 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/1808_obs.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)      999 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/1826_bursts.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)      281 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/beans.ini
+-rw-rw-r--   0 duncan     (504) staff       (20)   342452 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/example_1808_pfluxfromminbar.png
+-rw-rw-r--   0 duncan     (504) staff       (20)     4862 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/data/mr_prior_fit.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)     1046 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/get_alphas.py
+-rw-rw-r--   0 duncan     (504) staff       (20)     8756 2023-05-22 17:16:24.000000 beansp-1.4.3/beansp/get_data.py
+-rw-rw-r--   0 duncan     (504) staff       (20)     1004 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/mrprior.py
+-rw-rw-r--   0 duncan     (504) staff       (20)     6590 2023-05-25 12:59:26.000000 beansp-1.4.3/beansp/run_emcee.py
+-rw-rw-r--   0 duncan     (504) staff       (20)     9174 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/run_model.py
+-rw-rw-r--   0 duncan     (504) staff       (20)      682 2023-03-30 03:04:23.000000 beansp-1.4.3/beansp/settle.py
+drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-31 15:06:38.156505 beansp-1.4.3/beansp.egg-info/
+-rw-rw-r--   0 duncan     (504) staff       (20)     3073 2023-05-31 15:06:38.000000 beansp-1.4.3/beansp.egg-info/PKG-INFO
+-rw-rw-r--   0 duncan     (504) staff       (20)     2026 2023-05-31 15:06:38.000000 beansp-1.4.3/beansp.egg-info/SOURCES.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)        1 2023-05-31 15:06:38.000000 beansp-1.4.3/beansp.egg-info/dependency_links.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)        1 2023-03-30 03:06:21.000000 beansp-1.4.3/beansp.egg-info/not-zip-safe
+-rw-rw-r--   0 duncan     (504) staff       (20)       98 2023-05-31 15:06:38.000000 beansp-1.4.3/beansp.egg-info/requires.txt
+-rw-rw-r--   0 duncan     (504) staff       (20)        7 2023-05-31 15:06:38.000000 beansp-1.4.3/beansp.egg-info/top_level.txt
+drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-31 15:06:38.212250 beansp-1.4.3/docs/
+-rwxrwxr-x   0 duncan     (504) staff       (20)     5336 2023-05-29 06:54:34.000000 beansp-1.4.3/docs/conf.py
+-rw-rw-r--   0 duncan     (504) staff       (20)       33 2020-07-28 03:51:27.000000 beansp-1.4.3/docs/contributing.rst
+-rw-rw-r--   0 duncan     (504) staff       (20)     2026 2023-05-29 06:54:34.000000 beansp-1.4.3/docs/data.rst
+-rw-rw-r--   0 duncan     (504) staff       (20)        1 2020-07-28 03:51:27.000000 beansp-1.4.3/docs/history.rst
+-rw-rw-r--   0 duncan     (504) staff       (20)     1183 2023-05-29 06:54:34.000000 beansp-1.4.3/docs/index.rst
+-rw-rw-r--   0 duncan     (504) staff       (20)     1435 2023-05-29 06:54:34.000000 beansp-1.4.3/docs/installation.rst
+-rw-rw-r--   0 duncan     (504) staff       (20)       27 2020-07-28 03:51:27.000000 beansp-1.4.3/docs/readme.rst
+-rw-rw-r--   0 duncan     (504) staff       (20)    11113 2023-05-29 06:54:34.000000 beansp-1.4.3/docs/usage.rst
+-rw-rw-r--   0 duncan     (504) staff       (20)      117 2023-05-31 15:06:38.222307 beansp-1.4.3/setup.cfg
+-rw-rw-r--   0 duncan     (504) staff       (20)     2144 2023-05-18 09:33:15.000000 beansp-1.4.3/setup.py
+drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-31 15:06:38.214788 beansp-1.4.3/tests/
+-rw-rw-r--   0 duncan     (504) staff       (20)     1141 2023-03-30 03:04:23.000000 beansp-1.4.3/tests/README.rst
+-rw-rw-r--   0 duncan     (504) staff       (20)       60 2020-07-28 03:51:27.000000 beansp-1.4.3/tests/__init__.py
+drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-31 15:06:38.221077 beansp-1.4.3/tests/data/
+drwxrwxr-x   0 duncan     (504) staff       (20)        0 2023-05-31 15:06:38.221623 beansp-1.4.3/tests/data/benchmark/
+-rw-rw-r--   0 duncan     (504) staff       (20)     3724 2023-05-31 14:10:56.000000 beansp-1.4.3/tests/data/benchmark/settle_expected_result.ecsv
+-rw-rw-r--   0 duncan     (504) staff       (20)     7499 2023-03-30 03:04:23.000000 beansp-1.4.3/tests/data/benchmark/table1.mrt
+-rw-rw-r--   0 duncan     (504) staff       (20)   639200 2023-03-30 03:19:20.000000 beansp-1.4.3/tests/data/dummy.h5
+-rw-rw-r--   0 duncan     (504) staff       (20)      482 2023-03-30 03:18:52.000000 beansp-1.4.3/tests/data/dummy.ini
+-rw-rw-r--   0 duncan     (504) staff       (20)     3724 2023-05-31 14:11:27.000000 beansp-1.4.3/tests/data/multiprocessing.ecsv
+-rw-rw-r--   0 duncan     (504) staff       (20)     3724 2023-05-31 14:11:10.000000 beansp-1.4.3/tests/data/serial.ecsv
+-rw-rw-r--   0 duncan     (504) staff       (20)      603 2020-07-28 03:51:27.000000 beansp-1.4.3/tests/test_beans.py
+-rw-rw-r--   0 duncan     (504) staff       (20)    10918 2023-04-09 12:34:34.000000 beansp-1.4.3/tests/test_benchmark_settle.py
+-rw-rw-r--   0 duncan     (504) staff       (20)      169 2020-07-28 03:51:27.000000 beansp-1.4.3/tests/test_burstrain.py
+-rw-rw-r--   0 duncan     (504) staff       (20)     1558 2023-05-22 17:16:24.000000 beansp-1.4.3/tests/test_get_data.py
+-rw-rw-r--   0 duncan     (504) staff       (20)      435 2023-04-09 12:34:34.000000 beansp-1.4.3/tests/test_likelihood.py
+-rw-rw-r--   0 duncan     (504) staff       (20)     2704 2023-05-31 14:07:00.000000 beansp-1.4.3/tests/test_runmodel.py
+-rw-rw-r--   0 duncan     (504) staff       (20)      765 2023-05-31 14:02:30.000000 beansp-1.4.3/tests/test_settle.py
+-rwxrwxr-x   0 duncan     (504) staff       (20)     1351 2023-05-18 09:33:15.000000 beansp-1.4.3/tests/test_sft_beans.py
```

### Comparing `beansp-1.0.1/CONTRIBUTING.rst` & `beansp-1.4.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/LICENSE` & `beansp-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/PKG-INFO` & `beansp-1.4.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beansp
-Version: 1.0.1
+Version: 1.4.3
 Summary: Bayesian Estimation of Accreting Neutron Stars parameters
 Home-page: https://github.com/adellej/beans
 Author: 
 Author-email: adelle.goodwin@curtin.edu.au
 License: MIT license
 Keywords: beans
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -43,22 +43,24 @@
 * Documentation: https://beans-7.readthedocs.io/en/latest/
 * Repo: https://github.com/adellej/beans
 
 
 Features
 --------
 
-This software uses a Markov Chain Monte Carlo approach to match observations of an accreting neutron star in outburst with a simple ignition model to predict unobservable parameters such as neutron star mass, radius, surface gravity, distance and inclination of the source, and accreted fuel composition. The code is all written in Python 3, except for settle which is a c++ code with a python wrapper. It makes use of Dan Foreman-Mackey's python implementation of MCMC, emcee, available here - https://github.com/dfm/emcee.
+This software uses a Markov Chain Monte Carlo approach to match observations of an accreting neutron star in outburst with a simple ignition model to constrain parameters including the neutron star mass, radius, surface gravity, distance and system inclination, and accreted fuel composition. 
+
+The code is written in Python 3, except for settle which is a C++ code with a python wrapper. It makes use of Dan Foreman-Mackey's python implementation of MCMC, emcee, available at https://github.com/dfm/emcee.
 
 Credits
 -------
 
-Software written by Adelle Goodwin. See Goodwin et al. (2019) - https://arxiv.org/pdf/1907.00996.
+Software written by Adelle Goodwin; for a full description see Goodwin et al. (2019, https://doi.org/10.1093/mnras/stz2638 or preprint at https://arxiv.org/pdf/1907.00996).
 
-This softwate (BEANSp) was based on code written by Duncan Galloway, and uses Dan Foreman-Mackey's python implementation of MCMC, emcee. It depends on pySettle (https://github.com/adellej/pysettle), which was forked from the original settle written by Andrew Cumming.
+The algorithm is based on code written by Duncan Galloway, and depends on pySettle (https://github.com/adellej/pysettle), which was forked from the original settle written by Andrew Cumming.
 
 Package installation and usage
 ------------------------------
 BEANSp is on pyPI (https://pypi.org/project/beansp/) so installation is easy - either straight or in virtual environment:
 
    .. code-block::
```

### Comparing `beansp-1.0.1/README.rst` & `beansp-1.4.3/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -22,22 +22,24 @@
 * Documentation: https://beans-7.readthedocs.io/en/latest/
 * Repo: https://github.com/adellej/beans
 
 
 Features
 --------
 
-This software uses a Markov Chain Monte Carlo approach to match observations of an accreting neutron star in outburst with a simple ignition model to predict unobservable parameters such as neutron star mass, radius, surface gravity, distance and inclination of the source, and accreted fuel composition. The code is all written in Python 3, except for settle which is a c++ code with a python wrapper. It makes use of Dan Foreman-Mackey's python implementation of MCMC, emcee, available here - https://github.com/dfm/emcee.
+This software uses a Markov Chain Monte Carlo approach to match observations of an accreting neutron star in outburst with a simple ignition model to constrain parameters including the neutron star mass, radius, surface gravity, distance and system inclination, and accreted fuel composition. 
+
+The code is written in Python 3, except for settle which is a C++ code with a python wrapper. It makes use of Dan Foreman-Mackey's python implementation of MCMC, emcee, available at https://github.com/dfm/emcee.
 
 Credits
 -------
 
-Software written by Adelle Goodwin. See Goodwin et al. (2019) - https://arxiv.org/pdf/1907.00996.
+Software written by Adelle Goodwin; for a full description see Goodwin et al. (2019, https://doi.org/10.1093/mnras/stz2638 or preprint at https://arxiv.org/pdf/1907.00996).
 
-This softwate (BEANSp) was based on code written by Duncan Galloway, and uses Dan Foreman-Mackey's python implementation of MCMC, emcee. It depends on pySettle (https://github.com/adellej/pysettle), which was forked from the original settle written by Andrew Cumming.
+The algorithm is based on code written by Duncan Galloway, and depends on pySettle (https://github.com/adellej/pysettle), which was forked from the original settle written by Andrew Cumming.
 
 Package installation and usage
 ------------------------------
 BEANSp is on pyPI (https://pypi.org/project/beansp/) so installation is easy - either straight or in virtual environment:
 
    .. code-block::
```

### Comparing `beansp-1.0.1/beansp/analyse.py` & `beansp-1.4.3/beansp/analyse.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import random
 import math
 import subprocess
 from astropy.io import ascii
 import pickle
 from matplotlib.ticker import MaxNLocator
 import sys
-from scipy.stats.kde import gaussian_kde
+from scipy.stats import gaussian_kde
 import scipy.stats as stats
 import matplotlib.mlab as mlab
 import tables
 from scipy.interpolate import interp1d
 from chainconsumer import ChainConsumer
 from multiprocessing import Pool
 import os
@@ -31,40 +31,55 @@
 from .run_model import runmodel
 from .get_data import get_obs
 from .mrprior import mr_prior
 from .get_data import *
 from .run_emcee import runemcee
 
 
-# def get_param_uncert_obs1(param_array, numburstssim):
-#     # Get uncertainties on individual parameters:
-#     p1, p2, p3, p4 ,p5, p6, p7 = map(lambda v: (v[1], v[2]-v[1], v[1]-v[0]), zip(*np.percentile(param_array, [16, 50, 84], axis=0)))
-#     # this will return 
-#     return p1, p2, p3, p4, p5, p6, p7
+def get_param_uncert_obs(param_array, numburstssim, percentile=[16,50,84]):
+    '''
+    Get uncertainties on predicted parameters. This routine accepts a
+    list-of-lists with (for example) the start times of bursts for each
+    walker and each timestep:
+      [ [ t1, t2, t3, t4... tn ], 
+        [ t1, t2, t3, t4... tn ],
+            .
+            .
+            .
+    and calculates the 50th percentile value and +/- 1-sigma confidence
+    limits for each of the t1, t2, t3, returning a list-of-tuples for each
+    parameter, with the 50th percentile and the upper & lower uncertainties 
+    for each parameter in each tuple.
+
+    :param param_array: array listing the predicted values
+    :param numburstssim: number of events per instance (2nd dimension of
+      param_array)
+
+    :return: list of tuples giving parameter centroid and limits
+    '''
 
-def get_param_uncert_obs(param_array, numburstssim):
-    # Get uncertainties on individual parameters:
     plist = list()
     for i in range(0,numburstssim):
-        plist = map(lambda v: (v[1], v[2]-v[1], v[1]-v[0]), zip(*np.percentile(param_array, [16, 50, 84], axis=0)))
+        plist = map(lambda v: (v[1], v[2]-v[1], v[1]-v[0]),
+            zip(*np.percentile(param_array, percentile, axis=0)))
     plist2 = list()
     plist3 = list(plist)
     for i in range(0,numburstssim):
         plist2.append(plist3[i])
+
     return plist2
 
+
 def get_param_uncert(param_array, percentile=[16,50,84]):
     '''
-    Calculate uncertainties on individual parameterss.
-    This routine only works on unitless quantities
+    Calculate uncertainties on individual (scalar) parameters.
 
     :param param_array: array of parameter values to calculate percentiles
     :param percentile: percentiles to calculate, normally 1-sigma
     :return: array of percentile values; by default, the 50th percentile,
       upper error and lower error
     '''
 
-    p = map(lambda v: (v[1], v[2]-v[1], v[1]-v[0]), 
-        zip(*np.percentile(param_array, percentile, axis=0)))
+    v = np.percentile(param_array, percentile, axis=0)
 
-    return p
+    return np.array([v[1], v[2]-v[1], v[1]-v[0]])
```

### Comparing `beansp-1.0.1/beansp/beans.py` & `beansp-1.4.3/beansp/beans.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 """Main module. This has functions that do the sampling, save the chains, and analyse the results."""
 ## Python packages required:
 import matplotlib.pyplot as plt
+from matplotlib.colors import LogNorm
 import numpy as np
 import emcee
 import corner
 import random
 import math
 import subprocess
 from astropy.io import ascii
 import astropy.units as u
 import astropy.constants as const
 import pickle
 from matplotlib.ticker import MaxNLocator
 import sys
-from scipy.stats.kde import gaussian_kde
-import scipy.stats as stats
+from scipy.stats import gaussian_kde
+# import scipy.stats as stats
 import matplotlib.mlab as mlab
 import tables
 from scipy.interpolate import interp1d
 from chainconsumer import ChainConsumer
 from multiprocessing import Pool
 import os
 import time
 from configparser import ConfigParser
 
 import pkg_resources  # part of setuptools
 try:
     # this will fail if the package is not pip-installed
-    __version__ = pkg_resources.require("beans")[0].version
+    __version__ = pkg_resources.require("beansp")[0].version
 except:
     # in which case just record the path
     __version__ = os.getcwd()
 
-try:
-    # Required for the distance_limit method
-    import concord as cd
-except:
-    pass
+# Some constants
+
+BSTART_ERR = 10*u.min # Default uncertainty for burst start times
 
 # -------------------------------------------------------------------------#
 ## load local  modules
 from .settle import settle
 from .burstrain import generate_burst_train, next_burst, get_a_b, mean_flux, burstensemble
 from .run_model import runmodel
 from .get_data import get_obs
 from .mrprior import mr_prior
 from .run_emcee import runemcee
 from .analyse import get_param_uncert_obs, get_param_uncert
-from .initialise import init
 
 # -------------------------------------------------------------------------#
 
 
 __all__ = (
     "Beans"
 )
@@ -116,37 +114,89 @@
     """
 
     X, Z, Q_b, f_a, f_E, r1, r2, r3, mass, radius = theta_in
 
     # upper bound and lower bounds of each parameter defined here. Bounds were
     # found by considering an estimated value for each parameter then giving
     # reasonable limits.
-    if (0.00001 < X < 0.76) and \
+    if (0.00001 < X < 0.76) and (Z > 0.00001) and\
         (0.000001 <= Q_b < 5.0) and (1 <= f_a < 100) and (1 <= f_E < 100) and \
         (0.005 < r1 < 1.0) and (0.005 < r2 < 3.0) and \
         (0 < r3 * 1e3 < 1000) \
         and (1.15 < mass < 2.5) and (9 < radius < 17):
 
         return 0.0 + lnZprior(Z) + mr_prior(mass, radius) 
     else:
         return -np.inf
 
 
+def calc_dist_anisotropy(r1, r2, r3):
+    '''
+    Calculate distance and inclincation from scaling factors.  These
+    functions are taken (more or less) from Goodwin et al. 2019, eq.  18-20, 
+    but there seem to be some slight differences
+
+    TODO also infer the inclination, which will depend on the model
+    adopted for the anisotropy; because the burst and persistent emission
+    anisotropy are free to vary independently, there is no guarantee there
+    would be an inclination value consistent with every pair of values for
+    a given model
+
+    :param r1: ratio of mdot to bolometric (isotropic) fluence (eq. 12)
+    :param r2: ratio of observed to predicted alpha (eq. 13)
+    :param r3: ratio of fluence to isotropic burst energy (eq. 14)
+
+    :return: distance, xi_b, xi_p
+    '''
+
+    xi_p = np.power( (r1*r2*r3*1e3)/(63.23*0.74816), 0.5)
+    xi_b = (0.74816*xi_p)/r2
+    distance = 10*np.power((r1/xi_p), 0.5) #kpc
+
+    return distance, xi_b, xi_p
+
+
+def model_str(model):
+    """
+    Prints a compressed string representation of the model dict, with
+    reduced precision to reduce the size of the record saved to the .h5
+    file
+
+    :param model: model dictionary as returned by runmodel
+
+    :return: string representation of the model dict
+    """
+
+    return ("{'time': ["+','.join(['{:.4f}'.format(x) for x in model['time']]) \
+        +"], 'mdot': ["+','.join(['{:.5f}'.format(x) for x in model['mdot']]) \
+        +"], 'alpha': ["+','.join(['{:.3f}'.format(x) for x in model['alpha']]) \
+        +"], 'e_b': ["+','.join(['{:.4f}'.format(x) for x in model['e_b']]) \
+        +"]}").replace(' ','')
+
+
 class Beans:
     """
     The main object class that includes the basic functionality required for
     beans. The code will read in burst (and observation) data and attempt to
     simulate bursts to match the observed burst properties. There are two
     principle modes; the original function generates a "train" of individual
     bursts, observed (for example) during a transient outburst, as for the 
     original application to the 2002 outburst of SAX J1808.4-3658, observed
     with RXTE/PCA. The alternative is to match to a set of non-contiguous
     bursts ("ensemble" mode)
     """
 
+    HAS_CONCORD = False
+    try:
+        # Required for the distance_limit method
+        import concord as cd
+        HAS_CONCORD = True
+    except:
+        pass
+
     def __init__(self, config_file=None, nwalkers=200, nsteps=100,
                  run_id="test", obsname=None, burstname=None, gtiname=None,
                  theta= (0.44, 0.01, 0.18, 2.1, 3.5, 0.108, 0.90, 0.5, 1.4, 11.2),
                  numburstssim=3, bc=2.21, ref_ind=1, prior=prior_func,
                  threads = 4, test_model=True, restart=False, **kwargs):
         """
         Initialise a Beans object
@@ -209,65 +259,76 @@
 
         if run_id is None:
             run_id = os.path.join(data_path, '1808/test1')
 
         if burstname is None:
             burstname = os.path.join(data_path, '1808_bursts.txt')
 
+        self.lnprior = prior
+
         # Set up initial conditions:
 
         if config_file is not None:
             if not os.path.exists(config_file):
                 print ('** ERROR ** config file not found, applying keywords')
             print ('Reading run params from {} ...'.format(config_file))
             self.read_config(config_file)
             print ("...done")
         else:
             # apply the keyword values or defaults
             self.nwalkers = nwalkers
             self.nsteps = nsteps
             self.run_id = run_id
+            self.obsname = obsname
+            self.burstname = burstname
+            self.gtiname = gtiname
             self.theta = theta
+            self.bc = bc
+            self.ref_ind = ref_ind
             self.threads = threads
             self.numburstssim = numburstssim
             # number of bursts observed (redundant; set below after reading the data)
             # self.numburstsobs = numburstsobs
-            self.ref_ind = ref_ind
-            self.obsname = obsname
-            self.burstname = burstname
-            self.gtiname = gtiname
-            self.bc = bc
 
-        self.lnprior = prior
+        if self.lnprior(self.theta) == -np.inf:
+            print ('** ERROR ** supplied parameter vector is excluded by the prior')
+            return
+
+        # below set the parameters which are not part of the config
+        # file
+
         self.restart = restart
 
         # number of dimensions for the parameter array
-        # self.ndim = ndim
-        self.ndim = len(theta)
 
-        # self.gti_checking = gti_checking
-        self.gti_checking = gtiname is not None
+        self.ndim = len(self.theta)
+
+        self.gti_checking = self.gtiname is not None
 
 	# determines whether will run as a train of bursts or non-contiguous
 	# bursts ("ensemble" mode); previously numerical, default is 1 (True),
 	# which means a burst train will be generated; set obsname=None for
 	# non-contiguous (ensemble mode) run
 
-        self.train = (obsname is not None)
+        self.train = (self.obsname is not None)
+
+        self.bstart_err = BSTART_ERR.to('d').value
 
         # Read in all the measurements and set up all the parameters
+        # This function now operates on the Beans object directly, and the
+        # required attributes:
+        # x, y, yerr, tref, bstart, pflux, pfluxe, tobs, fluen, fluen_err, 
+        #     st, et
+        # are set in that routine
+        # bypasses the earlier init function, and instead calls get_obs
+        # directly
 
-        self.x, self.y, self.yerr, self.tref, self.bstart, self.pflux, \
-            self.pfluxe, self.tobs, self.fluen, self.fluen_err, \
-            self.st, self.et = init(
-            self.ref_ind, self.gti_checking, self.obsname, self.burstname,
-            self.gtiname, self.bc)
-        self.numburstsobs = len(self.fluen)
-        print(self.st, self.et)
+        get_obs(self)
 
+        self.numburstsobs = len(self.fluen)
 
         # # -------------------------------------------------------------------------#
         # # TEST THE MODEL WORKS
         # # -------------------------------------------------------------------------#
         print("# -------------------------------------------------------------------------#")
         print("Doing Initialisation..")
 
@@ -324,23 +385,26 @@
 
         :param theta: the model parameter tuple
         :param indent: number of characters to indent the string from the left
         """
 
         X, Z, Q_b, f_a, f_E, r1, r2, r3, mass, radius = theta
 
-        return """#X = {} \ hydrogen mass fraction
-#Z = {} \ CNO mass fraction
-#Q_b = {} \ base flux [MeV/nucleon]
-#M_NS = {} M_sun \ neutron star mass
-#R_NS = {} km \ neutron star radius
-#f_a, f_E = {}, {} \ systematic error terms for alpha, fluence
-#r_1, r_2, r_3 = {}, {}, {} \ scaling factors to convert predictions""".format(
-            X, Z, Q_b, mass, radius, f_a, f_E, r1, r2, r3).replace(
-            '#',' '*indent)
+        dist, xi_b, xi_p = calc_dist_anisotropy(r1, r2, r3)
+
+        return """#X = {} \\ hydrogen mass fraction
+#Z = {} \\ CNO mass fraction
+#Q_b = {} \\ base flux [MeV/nucleon]
+#M_NS = {} M_sun \\ neutron star mass
+#R_NS = {} km \\ neutron star radius
+#f_a, f_E = {}, {} \\ systematic error terms for alpha, fluence
+#r_1, r_2, r_3 = {}, {}, {} \\ scaling factors to convert predictions
+#  (equivalent to d = {:.2f} kpc, xi_b = {:.3f}, xi_p = {:.3f})""".format(
+    X, Z, Q_b, mass, radius, f_a, f_E, r1, r2, r3, dist, xi_b, xi_p).replace(
+    '#',' '*indent)
 
 
     def save_config(self, file=None, clobber=True):
         """
         Routine to write all the configuration parameters to a file, as a
         record of the run; but also to more easily replicate or continue
         a run
@@ -370,15 +434,15 @@
            Config.set("data", "ref_ind", str(self.ref_ind))
            Config.set("data", "gtiname", str(self.gtiname))
            Config.set("data", "bc", str(self.bc))
 
            Config.add_section("emcee")
            Config.set("emcee", "theta", str(self.theta))
            Config.set("emcee", "numburstssim", str(self.numburstssim))
-           # Config.set("emcee", "prior", str(self.lnprior))
+           Config.set("emcee", "prior", str(self.lnprior))
            Config.set("emcee", "nwalkers", str(self.nwalkers))
            Config.set("emcee", "nsteps", str(self.nsteps))
            Config.set("emcee", "threads", str(self.threads))
 
            Config.write(cfgfile)
            cfgfile.close()
 
@@ -413,14 +477,21 @@
                 #     "x %s:::%s:::%s"
                 #     % (option, config.get(section, option), str(type(option))))
                 if option == 'theta':
                     setattr(self, option, 
                         tuple(map(float, config.get(section, option)[1:-1].split(', '))))
                 elif option == 'bc':
                     setattr(self, option, config.getfloat(section, option))
+                elif option =='prior':
+                    function_name = config.get(section, option).split(' ')[1]
+                    if function_name != str(self.lnprior).split(' ')[1]:
+                        print ('''
+** WARNING ** config file lists prior function as {}, but supplied prior is {}
+              To fully replicate the previous run you need to specify the same prior using the prior flag on init
+'''.format(function_name, self.lnprior))
                 elif option in int_params:
                     setattr(self, option, config.getint(section, option))
                 else:
                     # string options (including "None")
                     _value = config.get(section, option)
                     if _value == 'None':
                         setattr(self, option, None)
@@ -442,48 +513,21 @@
           r2, r3, mass & radius
         :param x: the "independent" variable, passed to lnlike
         :param y: the "dependent" variable (i.e. measurements), passed to lnlike
         :param yerr: erorr estimates on y
         :return: likelihood, model result array
         """
 
-        # define y = "data" parameters
-        # I think these "globals" are not used; the only other reference I 
-        # can see is in run_model, which is commented out. So I think
-        # TODO these siz for loops can be deleted - dkg
-
-        for x,i in zip([ x for x in range(0, len(self.bstart)-1) if x != self.ref_ind], [i for i in range(0, len(self.bstart)-1) if i != self.ref_ind]):
-            globals()['t%s' % i] = self.y[x]
-        for x,i in zip(range(len(self.bstart)-1, len(self.fluen)+len(self.bstart)-1),range(0,len(self.bstart))):
-            globals()['Eb%s' % i] = self.y[x]
-        for x,i in zip(range(len(self.fluen)+len(self.bstart)-1, len(self.y)),range(0, len(self.bstart-1))):
-            globals()['a%s' % i] = self.y[x]
-
-    # define yerr as variance terms (errors) for our data parameters (listed in same order as for y)
-    # *note that we have to enter three time errors for the code to work however in reality the error should be the same for all of them (st0, st2 and st3 are really dummy parameters)
-
-        for x,i in zip([ x for x in range(0, len(self.bstart)-1) if x != self.ref_ind], [i for i in range(0, len(self.bstart)-1) if i != self.ref_ind]):
-            globals()['st%s' % i] = self.yerr[x]
-        for x,i in zip(range(len(self.bstart)-1, len(self.fluen)+len(self.bstart)-1),range(0,len(self.bstart))):
-            globals()['sEb%s' % i] = self.yerr[x]
-        for x,i in zip(range(len(self.fluen)+len(self.bstart)-1, len(self.y)),range(0, len(self.bstart-1))):
-            globals()['sa%s' % i] = self.yerr[x]
-
-
         # define theta = model parameters, which we define priors for
 
         X, Z, Q_b, f_a, f_E, r1, r2, r3, mass, radius = theta_in
 
-        # Instead of treating s_t as a parameter, we just hardwire it here
-
-        s_t = 10.0 / 1440.0
-
-	      # call model (function runmodel, in run_model.py) to generate the burst
-	      # train, or the set of bursts (for "ensemble" mode. In earlier versions
-	      # the corresponding IDL function was defined as
+	# call model (function runmodel, in run_model.py) to generate the burst
+	# train, or the set of bursts (for "ensemble" mode. In earlier versions
+	# the corresponding IDL function was defined as
         # modeldata(base, z, x, r1, r2 ,r3)
 
         model, valid, model2 = runmodel(
             theta_in, y, self.tref, self.bstart, self.pflux, self.pfluxe, self.tobs,self.numburstssim,self.numburstsobs, self.ref_ind, self.gti_checking,self.train,
              self.st, self.et
         )
         if not valid:
@@ -493,47 +537,32 @@
         # indices for the fluence and the alphas are shifted by one
         # if we're doing a "train" run, hence the int(self.train) (=1 if
         # self.train == True
 
         ato = int(self.train) # array "train" offset
         # special to trap "unhashable type" error
         # print (model, ato, len(self.bstart), len(self.fluen))
-        model[len(self.bstart)-ato:len(self.fluen)+len(self.bstart)-ato] *= r3
-        model[len(self.fluen)+len(self.bstart)-ato:] *= r2
+        model[self.numburstsobs-ato:len(self.fluen)+self.numburstsobs-ato] *= r3
+        model[len(self.fluen)+self.numburstsobs-ato:] *= r2
 
 	# To simplify final likelihood expression we define inv_sigma2 for each
 	# data parameter that describe the error.  The variance (eg sEb0) is
 	# underestimated by some fractional amount, f, for each set of
 	# parameters.
-        # TODO: assembling inv_sigma2 can probably all be done in one line
 
-        sEb = yerr[len(self.bstart)-ato:len(self.fluen)+len(self.bstart)-ato]
-        sa = yerr[len(self.fluen)+len(self.bstart)-ato:]
-
-        inv_sigma2 = []
-        if self.train:
-            for i in range (0,len(self.bstart)-1):
-                inv_sigma2.append(1.0/(s_t**2))
-        else:
-            for i in range (0,len(self.bstart)):
-                inv_sigma2.append(1.0/(yerr[i]**2))
-        for i in range(0,len(self.bstart)):
-            inv_sigma2.append(1.0/((sEb[i]*f_E)**2))
-        for i in range(0,len(self.bstart)-ato):
-            inv_sigma2.append(1.0/((sa[i]*f_a)**2))
+        err_fac = np.concatenate(( np.full(self.numburstsobs-ato,1.),
+            np.full(self.numburstsobs,f_E), np.full(self.numburstsobs-ato,f_a)))
+        inv_sigma2 = 1./(yerr*err_fac)**2
 
         # Final likelihood expression
         cpts = (self.y - (model)) ** 2 * inv_sigma2 - (np.log(inv_sigma2))
 
         # Test if the result string is defined here. It is, so we return the selected elements of result
         # instead of the downselection in model
 
-        model2 = str(model2).encode('ASCII')
-
-
         # Now also return the model
         return -0.5 * np.sum(cpts), model2
 
 
     def lnprob(self, theta_in, x, y, yerr):
         """
         The full log-probability function incorporating the priors (via 
@@ -557,22 +586,26 @@
         # Now also returns the model, to accumulate along with the likelihoods
 
         like, model = self.lnlike(theta_in, x, y, yerr)
 
         if (not np.isfinite(like)):
             return -np.inf, -np.inf, model
 
-        # we return the logprobability as well as the theta parameters at this point so we can extract results later
-        return lp + like, lp, model
+        # encoding below is so we have a suitable object for including in
+        # the blobs (see the dtype specification in runemcee)
+
+        return lp + like, lp, model_str(model).encode('ASCII')
+
 
 
     def plot_model(self, model=None, mdot=True):
         """
-        Display a plot of the model results, for a burst train calculated with generate_burst_train
-        Adapted from the example at https://matplotlib.org/gallery/api/two_scales.html
+	Display a plot of the model results, for a burst train calculated
+	with generate_burst_train Adapted from the example at
+        https://matplotlib.org/gallery/api/two_scales.html
 
         :param model: array of packed model prediction, OR dict giving full
           model results
         :param mdot: flag to show mdot rather than flux (only possible if
           you're passing the full model)
         """
         tobs = self.bstart
@@ -780,16 +813,16 @@
 
         print("# -------------------------------------------------------------------------#")
         print (self)
         print("# -------------------------------------------------------------------------#")
         # Testing the various functions. Each of these will display the likelihood value, followed by the model-results "blob"
         print("Testing the prior and likelihood functions..")
         print("lnprior:", self.lnprior(self.theta))
-        print("lnlike:", self.lnlike(self.theta, self.x, self.y, self.yerr))
-        print("lnprob:", self.lnprob(self.theta, self.x, self.y, self.yerr))
+        print("lnlike:", self.lnlike(self.theta, None, self.y, self.yerr))
+        print("lnprob:", self.lnprob(self.theta, None, self.y, self.yerr))
         print("# -------------------------------------------------------------------------#")
         # print(f"The theta parameters will begin at: {self.theta}")
         # print("# -------------------------------------------------------------------------#")
         if plot:
             print("plotting the initial guess.. (you want the predicted bursts to match approximately the observed bursts here)")
             # make plot of observed burst comparison with predicted bursts:
             # TODO: this section can presumably be replaced by the plot_model
@@ -821,20 +854,19 @@
             #plt.errorbar(tobs, ebobs, fmt='.',color='black')
             plt.xlabel("Time (days after start of outburst)")
             plt.ylabel("Fluence (1e-9 erg/cm$^2$)")
             plt.title("Initial guess of parameters")
             plt.legend(loc=2)
             plt.show()
 
-        print("# -------------------------------------------------------------------------#")
-        print("Beginning sampling...")
         _start = time.time()
 
         # run the chains and save the output as a h5 file
-        sampler = runemcee(self.nwalkers, self.nsteps, self.theta, self.lnprob, self.x, self.y, self.yerr, self.run_id, self.restart, self.threads)
+        sampler = runemcee(self.nwalkers, self.nsteps, self.theta, self.lnprob, self.lnprior, 
+            None, self.y, self.yerr, self.run_id, self.restart, self.threads)
         print(f"...sampling complete!")
 
         _end = time.time()
         print ("Sampling took {0:.1f} seconds".format(_end-_start))
 
         if analyse:
             self.do_analysis(burnin=burnin)
@@ -995,15 +1027,17 @@
         G = const.G.to('cm3 g-1 s-2')
 
         # list of available analyses
 
         analyses = {'autocor': 'autocorrelation times as a function of timestep',
                     'chain': 'first 300 iterations of the chains',
                     'posteriors': 'raw posteriors and the input values',
-                    'mrcorner': 'M, R, g and 1+z corner plot',
+                    'mrcorner': 'corner plot with M, R, g and 1+z',
+                    'fig6': 'corner plot with xi_b, xi_p, d, Q_b, Z',
+                    'fig8': 'xi_b vs. xi_p and models for comparison',
                     'comparison': 'observed and predicted burst times, fluences' }
 
         # check the chosen option is one of those implemented
 
         for option in options:
             if option not in analyses.keys():
                 print ('** ERROR ** {} is not an available analysis option; choose from'.format(option))
@@ -1030,27 +1064,33 @@
 
         # moved burnin to be a parameter, so we can pass that from do_run
 
         if burnin >= self.nsteps_completed*0.9:
             print ('** WARNING ** discarding burnin {} will leave too few steps ({} total), ignoring'.format(burnin, self.nsteps_completed))
             burnin = 0
 
+        # print ("Reading in flattened samples to show posteriors...")
+        # samples = self.reader.get_chain(flat=True, discard=burnin)
+        self.samples = self.sampler[burnin:,:,:].reshape((-1,10))
+
+        # ---------------------------------------------------------------------#
         if 'autocor' in options:
 
             # plot autocorrelation times
 
             if savefig:
                 self.plot_autocorr(self.reader, savefile='{}_autocorrelationtimes.pdf'.format(self.run_id))
             else:
                 self.plot_autocorr(self.reader, savefile=None)
                 print ('Skipping autocorrelation plot save')
             print ("...done")
 
         #sampler = emcee.EnsembleSampler(self.nwalkers, self.ndim, self.lnprob, args=(self.x, self.y, self.yerr), backend=reader)
 
+        # ---------------------------------------------------------------------#
         if 'chain' in options:
 
             # plot the chains:
 
             print ("Plotting the chains...")
             labels = ["$X$","$Z$","$Q_b$","$f_a$","$f_E$","$r1$","$r2$","$r3$", "$M$", "$R$"]
             # plt.clf()
@@ -1068,66 +1108,77 @@
                 plt.savefig(self.run_id+'chain-plot.pdf')
             else:
                 print ('Skipping chain plot save')
 
             plt.show()
             print ("...done")
 
+        # ---------------------------------------------------------------------#
         if 'posteriors' in options:
 
             # Also read in the "flattened" chain, for the posteriors
 
-            # I think I can get samples from the previously-read in
-            # sampler object, just need to flatten the array
-
-            # print ("Reading in flattened samples to show posteriors...")
-            # samples = self.reader.get_chain(flat=True, discard=burnin)
-            samples = self.sampler[burnin:,:,:].reshape((-1,10))
-
             # make plot of posterior distributions of your parameters:
             cc = ChainConsumer()
-            cc.add_chain(samples, parameters=["X", "Z", "Qb", "fa", "fE", "r1", "r2", "r3", "M", "R"])
+            cc.add_chain(self.samples, parameters=["X", "Z", "Qb", "fa", "fE", "r1", "r2", "r3", "M", "R"])
             if savefig:
                 cc.plotter.plot(filename=self.run_id+"_posteriors.pdf",
-                    figsize="column", truth=list(self.theta))
+                    figsize="page", truth=list(self.theta))
             else:
-                # this one doesn't appear on the Mac, not sure why
-                cc.plotter.plot(figsize="column", truth=list(self.theta))
+                fig = cc.plotter.plot(figsize="page", truth=list(self.theta))
+                fig.show()
             print ("...done")
 
-        if ('mrcorner' in options) or ('comparison' in options):
+        # ---------------------------------------------------------------------#
+        if (('mrcorner' in options) or ('comparison' in options) \
+            or ('fig6' in options) or ('fig8' in options)):
+            # maybe can try to record that we've already read these
+            # parameters in, like so
+            # and (self.burnin_excluded != burnin):
 
             # and finally read in the model realisations
             # This loop can take a LOOOOOONG time for long runs
             # TODO save this to the Beans object so we only need to read
             # it in once; need to rationalise what arrays are kept etc.
 
-            print ("Reading in and processing blobs...")
+            print ("Reading in and processing blobs, ignoring first {}...".format(burnin))
             blobs = self.reader.get_blobs(flat=True)
 
-            data = []
-            for i in range(len(blobs["model"])):
-                data.append(eval(blobs["model"][i].decode('ASCII', 'replace')))
-            print ("...done")
+            # Get predictions for each model run from the blobs structure:
 
-            # Get parameters for each model run from the blobs structure:
+            time, e_b, alpha, mdot = [], [], [], []
+            # X = [] # just for testing; won't be included in future blobs
+            for i in range(burnin*self.nwalkers, len(blobs["model"])):
+                _model = eval(blobs["model"][i].decode('ASCII', 'replace'))
+                time.append(_model['time'])
+                e_b.append(_model['e_b'])
+                alpha.append(_model['alpha'])
+                mdot.append(_model['mdot'])
+                # X.append(_model['x_0'][0])
+            print ("...done")
 
-            # get each individual parameter:
-            time = [data[i]['time'] for i in range(len(data))]
-            e_b = [data[i]['e_b'] for i in range(len(data))]
-            alpha = [data[i]['alpha'] for i in range(len(data))]
-            X = [data[i]['x_0'] for i in range(len(data))]
-            Z = [data[i]['z'] for i in range(len(data))]
-            base = [data[i]['base'] for i in range(len(data))]
-            mdot = [data[i]['mdot'] for i in range(len(data))]
-            r1 = np.array([data[i]['r1'] for i in range(len(data))])
-            r2 = np.array([data[i]['r2'] for i in range(len(data))])
-            r3 = np.array([data[i]['r3'] for i in range(len(data))])
-            mass = np.array([data[i]['mass'] for i in range(len(data))])
-            radius = np.array([data[i]['radius'] for i in range(len(data))])
+            # we don't include these in the blobs anymore, to save space
+            # (and they're redundant, as also included in the samples)
+            # X = [data[i]['x_0'][0] for i in range(len(data))]
+            # Z = [data[i]['z'][0] for i in range(len(data))]
+            # base = [data[i]['base'][0] for i in range(len(data))]
+            # r1 = np.array([data[i]['r1'][0] for i in range(len(data))])
+            # r2 = np.array([data[i]['r2'][0] for i in range(len(data))])
+            # r3 = np.array([data[i]['r3'][0] for i in range(len(data))])
+            # mass = np.array([data[i]['mass'][0] for i in range(len(data))])
+            # radius = np.array([data[i]['radius'][0] for i in range(len(data))])
+            # assert np.allclose(X, self.samples[:,0])
+            X = self.samples[:,0]
+            Z = self.samples[:,1]
+            base = self.samples[:,2]
+            r1 = self.samples[:,5]
+            r2 = self.samples[:,6]
+            r3 = self.samples[:,7]
+            mass = self.samples[:,8]
+            radius = self.samples[:,9]
 
             # calculate redshift and gravity from mass and radius:
 	    # keep the parameters that we're going to calculate limits on
 	    # below, dimensionless
 
             R = np.array(radius)*1e5*u.cm #cgs
             M = np.array(mass)*const.M_sun.to('g') #cgs
@@ -1135,25 +1186,20 @@
 	    # ChainConsumer's plot method can't handle Quantity objects,
 	    # so we need to convert gravity and redshift back to numpy
 	    # arrays here
             redshift = np.power((1 - (2*G*M/(R*c**2))), -0.5).value
             gravity = (M*redshift*G/R**2 / (u.cm/u.s**2)).value #cgs
 
             # calculate distance and inclincation from scaling factors:
-            r1 = np.array(r1)
-            r2 = np.array(r2)
-            r3 = np.array(r3)
-
-            xip = np.power( (r1*r2*r3*1e3)/(63.23*0.74816), 0.5)
-            xib = (0.74816*xip)/r2
-            distance = 10*np.power((r1/xip), 0.5) #kpc
+
+            distance, xib, xip = calc_dist_anisotropy(r1, r2, r3)
+
             cosi_2 = 1/(2*xip)
             cosi = 0.5/(2*(xip/xib)-1)
 
-
 	    # to get the parameter middle values and uncertainty use the
 	    # functions get_param_uncert_obs and get_param_uncert_pred,
 	    # e.g.
 
             if self.train:
                 times = get_param_uncert_obs(time, self.numburstssim*2+1)
             else:
@@ -1169,28 +1215,29 @@
             ebpred = [x[0] for x in ebs]
             ebpred_errup = [x[1] for x in ebs]
             ebpred_errlow = [x[2] for x in ebs]
             if self.train:
                 alphas = get_param_uncert_obs(alpha, self.numburstssim*2)
             else:
                 alphas = get_param_uncert_obs(alpha, self.numburstssim)
-            Xpred = np.array(list(get_param_uncert(X))[0])
-            Zpred = np.array(list(get_param_uncert(Z))[0])
-            basepred = np.array(list(get_param_uncert(base))[0])
-            dpred = np.array(list(get_param_uncert(distance))[0])
-            cosipred = np.array(list(get_param_uncert(cosi))[0])
-            xippred = np.array(list(get_param_uncert(xip))[0])
-            xibpred = np.array(list(get_param_uncert(xib))[0])
-            masspred = np.array(list(get_param_uncert(mass))[0])
-            radiuspred = np.array(list(get_param_uncert(radius))[0])
-            gravitypred = np.array(list(get_param_uncert(gravity))[0])
-            redshiftpred = np.array(list(get_param_uncert(redshift))[0])
-            r1pred = np.array(list(get_param_uncert(r1))[0])
-            r2pred = np.array(list(get_param_uncert(r2))[0])
-            r3pred = np.array(list(get_param_uncert(r3))[0])
+
+            Xpred = get_param_uncert(X)
+            Zpred = get_param_uncert(Z)
+            basepred = get_param_uncert(base)
+            dpred = get_param_uncert(distance)
+            cosipred = get_param_uncert(cosi)
+            xippred = get_param_uncert(xip)
+            xibpred = get_param_uncert(xib)
+            masspred = get_param_uncert(mass)
+            radiuspred = get_param_uncert(radius)
+            gravitypred = get_param_uncert(gravity)
+            redshiftpred = get_param_uncert(redshift)
+            r1pred = get_param_uncert(r1)
+            r2pred = get_param_uncert(r2)
+            r3pred = get_param_uncert(r3)
 
             # scale fluences by scaling factor:
             ebpred = np.array(ebpred)*np.array(r3pred[0])
             ebpred_errup = np.array(ebpred_errup)*np.array(r3pred[0])
             ebpred_errlow = np.array(ebpred_errlow)*np.array(r3pred[0])
 
             # save to text file with columns: paramname, value, upper uncertainty, lower uncertainty
@@ -1200,34 +1247,127 @@
 	    # make plot of posterior distributions of the mass, radius,
 	    # surface gravity, and redshift: stack data for input to
 	    # chainconsumer:
             mass = mass.ravel()
             radius = radius.ravel()
             gravity = np.array(gravity).ravel()
             redshift = redshift.ravel()
-            mrgr = np.column_stack((mass, radius, gravity, redshift))
 
+        # ---------------------------------------------------------------------#
         if 'mrcorner' in options:
 
+            mrgr = np.column_stack((mass, radius, gravity, redshift))
+
             # plot with chainconsumer:
             cc = ChainConsumer()
             cc.add_chain(mrgr, parameters=["M", "R", "g", "1+z"])
             if savefig:
-                cc.plotter.plot(filename=self.run_id+"_massradius.pdf",figsize="column")
+                cc.plotter.plot(filename=self.run_id+"_massradius.pdf",figsize="page")
+            else:
+                fig = cc.plotter.plot(figsize="page")
+                fig.show()
+
+        # ---------------------------------------------------------------------#
+        if 'fig6' in options:
+
+            # fig6data = np.column_stack((xip, xib, distance, base, Z, X))
+            fig6data = np.column_stack((X, Z, base, distance, xib, xip))
+
+            # plot with chainconsumer:
+
+            cc = ChainConsumer()
+
+            # configure params below copied from Adelle's jupyter notebook
+            cc.add_chain(fig6data, parameters=["X", "$Z$", "$Q_b$ (MeV)",
+                "$d$ (kpc)", "$\\xi_b$", "$\\xi_p$"])\
+                .configure(flip=False, bins=0.7, summary=False, \
+                diagonal_tick_labels=False, max_ticks=3, shade=True, \
+                shade_alpha=1.0 ,bar_shade=True, tick_font_size='xx-large', \
+                label_font_size='xx-large',smooth=True, \
+                sigmas=np.linspace(0, 3, 4))
+            if savefig:
+                cc.plotter.plot(filename=self.run_id+"_fig6.pdf",figsize="page")
             else:
-                cc.plotter.plot(figsize="column")
+                fig = cc.plotter.plot(figsize="page")
+                fig.show()
 
+        # ---------------------------------------------------------------------#
+        if 'fig8' in options:
+
+            # here we read in data from the anisotropy models. There's
+            # probably a better way to do this, via concord (if it's
+            # available)
+
+            counts, ybins, xbins, image = plt.hist2d(np.array(xip), 
+                np.array(xib), bins=500, norm=LogNorm(), cmap='OrRd')
+
+            xi_p_model2 = np.arange(0, 2.5, 0.01)
+            xi_b_model2 = np.empty(len(xi_p_model2))
+
+            for i in range(0,250):
+    
+                xi_b_model2[i] = 1./((1./(2*xi_p_model2[i])) + 0.5)
+    
+            # overplot the various models
+
+            plt.plot(xi_p_model2, xi_b_model2, color = 'black',ls='-', label = 'Fujimoto (1988)')  
+
+            if Beans.HAS_CONCORD:
+                # setup dict with list of models, legend labels and linestyles
+                he16_models = {'he16_a': ('He & Keek (2016) model A', '--'),
+                               'he16_b': ('model B', '-.'),
+                               'he16_c': ('model C', (0, (3, 5, 1, 5))), 
+                               'he16_d': ('model D', (0, (1, 5))) }
+
+                for model in he16_models.keys():
+
+                    _model = self.cd.diskmodel.load_he16(model)
+
+                    model_theta = _model['col1']
+                    model_xid = _model['col2']
+                    model_xir = _model['col3']
+                    model_xip1 = _model['col4']
+                    model_xib1 = model_xid + model_xir
+
+                    model_xib = 1./model_xib1
+                    model_xip = 1./model_xip1
+
+                    #modela:
+                    plt.plot(model_xip, model_xib, color='darkblue', 
+                        ls=he16_models[model][1], label=he16_models[model][0])
+
+            else:
+                print ('''
+** WARNING ** install concord if you want to overplot model curves
+              See https://github.com/outs1der/concord''')
+
+            plt.xlabel(r'$\xi_{\mathrm{p}}$',fontsize='xx-large')
+            plt.ylabel(r'$\xi_{\mathrm{b}}$',fontsize='xx-large')
+
+            plt.legend(loc='best',fontsize='large')
+
+            plt.axis([0.,2.1,0.,2.1])
+
+            plt.xticks(fontsize=14)
+            plt.yticks(fontsize=14)
+
+            if savefig:
+                plt.savefig('{}_xipvsxib_models_contourlines.pdf'.format(self.run_id))
+            else:
+                plt.show()
+
+        # ---------------------------------------------------------------------#
         if 'comparison' in options:
 
             # make plot of observed burst comparison with predicted bursts:
 
             plt.figure(figsize=(10,7))
 
             # plt.scatter(self.bstart, self.fluen, color = 'black', marker = '.', label='Observed', s =200)
-            plt.errorbar(self.bstart, self.fluen, yerr=self.fluen_err, 
+            plt.errorbar(self.bstart, self.fluen, yerr=self.fluene, 
                 color='black', linestyle='', marker='.', ms=13, label='Observed')
             #plt.scatter(time_pred_35, e_b_pred_35, marker = '*',color='cyan',s = 200, label = '2 M$_{\odot}$, R = 11.2 km')
             if self.train:
                 # plt.scatter(timepred[1:], ebpred, marker='*', color='darkgrey', s=100, label='Predicted')
                 plt.errorbar(timepred[1:], ebpred, 
                     yerr=[ebpred_errup, ebpred_errlow],
                     xerr=[timepred_errup[1:], timepred_errlow[1:]],
```

### Comparing `beansp-1.0.1/beansp/burstrain.py` & `beansp-1.4.3/beansp/burstrain.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,15 +265,16 @@
 
 # -------------------------------------------------------------------------#
 
 # -------------------------------------------------------------------------#
 
 
 def generate_burst_train( base, z, x_0, r1, r2, r3, mass, radius,
-    bstart, pflux, pfluxe, tobs, numburstssim, ref_ind, debug=False):
+    bstart, pflux, pfluxe, tobs, numburstssim, ref_ind, full_model=False, 
+    debug=False):
     """
     This routine generates a simulated burst train based on the model
     input parameters, and the mdot history inferred from the persistent
     flux measurements (tobs, pflux, pfluxe)
 
     :param base: base flux [MeV/nucleon]
     :param z: accreted CNO metallicity
@@ -286,14 +287,16 @@
     # Now all the parameters below can be passed from a Beans object
     :param bstart: burst start times
     :param pflux: persistent flux measurements
     :param pfluxe: uncertainty on persistent flux
     :param tobs: times for the persistent flux measurements
     :param numburstssim: number of bursts to simulate (in each direction)
     :param ref_ind: index of reference burst
+    :param full_model: if set to True, include all the parameters in the
+      dict that is returned
     :param debug: set to True to show additional debugging information
 
     :return: a dictionary with the following keys:
     ['base', 'z', 'x_0', 'r1', 'r2', 'r3', 'time', 'mdot_max', 'mdot',
     'iref', 'alpha', 'e_b', 'mass', 'radius', 'forward', 'backward']
     We have one more element of the time array than the other arrays, because
     we can't determine the properties for that burst, as we don't have
@@ -429,53 +432,49 @@
 
     if (mdot_max == -1) & (len(stime) > 0):
 
         mdot_max = max(smdot)
 
     result = dict()
 
-    result["base"] = [base]
-    result["z"] = [z]
-    result["x_0"] = [x_0]
-    result["r1"] = [r1]
-    result["r2"] = [r2]
-    result["r3"] = [r3]
+    if full_model:
+        # model parameters are redundant for the model returned
+        result["base"] = [base]
+        result["z"] = [z]
+        result["x_0"] = [x_0]
+        result["r1"] = [r1]
+        result["r2"] = [r2]
+        result["r3"] = [r3]
+
+        result["mdot_max"] = [mdot_max]
+
+        result["mass"] = [mass]
+        result["radius"] =  [radius]
+
+        result["forward"] = forward     # to keep track of the outcome of each direction
+        result["backward"] = backward
+
+    # now the actual predictions
+
     result["time"] = stime
-    result["mdot_max"] = [mdot_max]
     if len(stime) > 0:
         # The simulation might fail to generate any bursts, so only add the arrays if they exist
         result["mdot"] = smdot
-        result["iref"] = iref
+        # this is redundant, can be worked out from the times
+        # result["iref"] = iref
         result["alpha"] = salpha
         result["e_b"] = se_b
         #print(f"In burstrain fluence is {se_b}")
 
-    # result["qnuc"] = sqnuc
-    # result["xbar"] = sxbar
-    result["mass"] = [mass]
-    result["radius"] =  [radius]
-    result["forward"] = forward     # to keep track of the outcome of each direction
-    result["backward"] = backward
 
     return result
 
 
-def burstensemble(
-    base,
-    x_0,
-    z,
-    r1,
-    r2,
-    r3,
-    mass,
-    radius,
-    bstart,
-    pflux,
-    numburstsobs,
-):
+def burstensemble( base, x_0, z, r1, r2, r3, mass, radius, bstart, pflux,
+    numburstsobs, full_model=False ):
     """
     This routine generates as many burst predictions as there are burst
     measurements.
     Written initially by Luke Waterson, 2021
     """
 
     minmdot = 0.0
@@ -515,28 +514,33 @@
         smdot.append(_mdot)
         # stime.append(bstart[i])
         stime.append(tmp.tdel[0])
         mdot_max = max(smdot)
 
     result = dict()
 
-    result["base"] = [base]
-    result["z"] = [z]
-    result["x_0"] = [x_0]
-    result["r1"] = [r1]
-    result["r2"] = [r2]
-    result["r3"] = [r3]
-    result["mdot"] = smdot
-    result["mdot_max"] = [mdot_max]
+    if full_model:
+        # model parameters are redundant for the model returned
+        result["base"] = [base]
+        result["z"] = [z]
+        result["x_0"] = [x_0]
+        result["r1"] = [r1]
+        result["r2"] = [r2]
+        result["r3"] = [r3]
+
+        result["mdot_max"] = [mdot_max]
+
+        result["mass"] = [mass]
+        result["radius"] = [radius]
+
+    # now the actual predictions
+
     result["time"] = stime
+    result["mdot"] = smdot
     result["alpha"] = salpha
     result["e_b"] = se_b
 
-    result["mass"] = [mass]
-    result["radius"] = [radius]
-
     # omit the printing for now, as it prevents assessing the progress
     # print('ensemble')
     # print(f"In burstrain fluence is {se_b}")
 
-
     return result
```

### Comparing `beansp-1.0.1/beansp/data/1731_bursts_avg.txt` & `beansp-1.4.3/beansp/data/1731_bursts_avg.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/17498_bursts.txt` & `beansp-1.4.3/beansp/data/17498_bursts.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/17498_data/17498_gti.txt` & `beansp-1.4.3/beansp/data/17498_data/17498_gti.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/17498_data/17498_obs_new.txt` & `beansp-1.4.3/beansp/data/17498_data/17498_obs_new.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/17498_data/run_17498.py` & `beansp-1.4.3/beansp/data/17498_data/run_17498.py`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/17498_obs.txt` & `beansp-1.4.3/beansp/data/17498_obs.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/17511/test2_parameterconstraints_pred.txt` & `beansp-1.4.3/beansp/data/17511/test2_parameterconstraints_pred.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/17511/test3_parameterconstraints_pred.txt` & `beansp-1.4.3/beansp/data/17511/test3_parameterconstraints_pred.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/17511_bursts.txt` & `beansp-1.4.3/beansp/data/17511_bursts.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/17511_gti.dat` & `beansp-1.4.3/beansp/data/17511_gti.dat`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/17511_obs.txt` & `beansp-1.4.3/beansp/data/17511_obs.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/1808/test1_parameterconstraints_pred.txt` & `beansp-1.4.3/beansp/data/1808/test1_parameterconstraints_pred.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/1808/test2_parameterconstraints_pred.txt` & `beansp-1.4.3/beansp/data/1808/test2_parameterconstraints_pred.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/1808/test4_parameterconstraints_pred.txt` & `beansp-1.4.3/beansp/data/1808/test4_parameterconstraints_pred.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/1808/test5_parameterconstraints_pred.txt` & `beansp-1.4.3/beansp/data/1808/test5_parameterconstraints_pred.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/1808/test6_parameterconstraints_pred.txt` & `beansp-1.4.3/beansp/data/1808/test6_parameterconstraints_pred.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/1808/test7_parameterconstraints_pred.txt` & `beansp-1.4.3/beansp/data/1808/test7_parameterconstraints_pred.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/1808_bursts.txt` & `beansp-1.4.3/beansp/data/1808_bursts.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/1808_example_burstsfromminbar.png` & `beansp-1.4.3/beansp/data/1808_example_burstsfromminbar.png`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/1808_gti.txt` & `beansp-1.4.3/beansp/data/1808_gti.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/1808_obs.txt` & `beansp-1.4.3/beansp/data/1808_obs.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/1826_bursts.txt` & `beansp-1.4.3/beansp/data/1826_bursts.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/example_1808_pfluxfromminbar.png` & `beansp-1.4.3/beansp/data/example_1808_pfluxfromminbar.png`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/data/mr_prior_fit.txt` & `beansp-1.4.3/beansp/data/mr_prior_fit.txt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/get_alphas.py` & `beansp-1.4.3/beansp/get_alphas.py`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/mrprior.py` & `beansp-1.4.3/beansp/mrprior.py`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/run_emcee.py` & `beansp-1.4.3/beansp/run_emcee.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,25 +2,55 @@
 import emcee
 import sys
 import pickle
 from multiprocessing import Pool
 import time
 import h5py
 
-def runemcee(nwalkers, nsteps, theta, lnprob, x, y, yerr, run_id, restart, threads):
+def set_initial_positions(theta, nwalkers, prior, scale=1e-4):
+    '''
+    Distribute the initial positions for the walkers around the supplied theta value, 
+    making sure they're consistent with the prior
+
+    :param theta: desired centroid for walker parameters
+    :param nwalkers: number of initial positions to generate
+    :param prior: prior function adopted
+    :param scale: Gaussian spread of the values in each dimension
+
+    :return: list of nwalkers positions
+    '''
+    
+    ndim = len(theta)
+    pos = np.array([theta + scale*np.random.randn(ndim) for i in range(nwalkers)])
+    
+    valid = np.array([prior(pos[i]) != -np.inf for i in range(nwalkers)])
+    
+    print ('Initial walker positions within {} of supplied parameter vector, checking for consistency with prior...'.format(scale))
+
+    # print (len(np.where(~valid)[0]))
+    while (len(np.where(~valid)[0])) > 0:
+        pos[~valid] = [theta + scale*np.random.randn(ndim) for i in range(len(np.where(~valid)[0]))]
+        valid = np.array([prior(pos[i]) != -np.inf for i in range(nwalkers)])
+        # print (len(np.where(~valid)[0]))                                                                     
+
+    return list(pos)
+
+
+def runemcee(nwalkers, nsteps, theta, lnprob, prior, x, y, yerr, run_id, restart, threads):
     """
     Function to initilise and run emcee.
     Removed the redundant parameter ndim, which can be determined from the
     theta parameter array
 
     :param nwalkers: number of walkers for the emcee run
     :param nsteps: number of MCMC steps to run
     :param theta: model parameter tuple, with X, Z, Q_b, f_a, f_E, r1, r2, r3,
       mass & radius
     :param lnprob: log-probability function to use with emcee
+    :param prior: prior function to use with emcee, used to check the initial walker positions
     :param x: the "independent" variable, passed to lnlike
     :param y: the "dependent" variable (i.e. measurements), passed to lnlike
     :param yerr: erorr estimates on y
     :param run_id: string identifier for the run, used to label all the
       result files, and where you want output to be saved
     :param restart: set to True to continue a previously interrupted run
     :param threads: number of threads for emcee to use (e.g. number of
@@ -30,30 +60,33 @@
     ndim = len(theta)
 
     # This section now defines the initial walker positions and next defines the chain and runs emcee.
 
     print("# -------------------------------------------------------------------------#")
 
     # define the dtype of the blobs
-    #dtype = [("lnprob", float), ("model", "S1000")]
-    dtype = [("lnprob", float), ("model", h5py.string_dtype(encoding='ascii'))]
+    # this refers to the 2nd and subsequent parameters returned by lnprob;
+    # in our case the prior probability and the full model result, encoded
+    # as ASCII
+
+    dtype = [("lnprior", float), ("model", h5py.string_dtype(encoding='ascii'))]
 
     # use emcee backend to save as a HD5 file
     # see https://emcee.readthedocs.io/en/stable/user/backends
     reader = emcee.backends.HDFBackend(filename=run_id + ".h5")
 
     if restart == True:
-        # don't know why the pos are identical to the restart=False case below;
-        # perhaps they're ignored
         steps_so_far = np.shape(reader.get_chain())[0]
         print('Restarting',run_id,'with',nwalkers,'walkers after',steps_so_far,'steps done')
     else:
         reader.reset(nwalkers, ndim)
         # set the intial position of the walkers
-        pos = [theta + 1e-4*np.random.randn(ndim) for i in range(nwalkers)]
+        # pos = [theta + 1e-4*np.random.randn(ndim) for i in range(nwalkers)]
+        pos = set_initial_positions(theta,  nwalkers, prior)
+
         print('Ready to run',run_id,'with',nwalkers,'walkers')
             
     print("Beginning sampling..")
    
     # try the multiprocessing (again) following the simple example here:
     # https://emcee.readthedocs.io/en/stable/tutorials/parallel
     with Pool(processes=threads) as pool:
@@ -112,29 +145,11 @@
                 converged = np.all(tau * 100 < sampler.iteration)
                 converged &= np.all(np.abs(old_tau - tau) / tau < 0.01)
                 if converged:
                     print('Complete! Chains are converged')
                     break
                 old_tau = tau
 
-
-        #tau = sampler.get_autocorr_time()
         print('Complete! WARNING max number of steps reached but chains may or may not be converged.')
-        
-    #     print('Samples complete. Took {0:.1f} seconds'.format(multi_time))
-
-    # with Pool() as pool:
-    #     print("Beginning sampling..")
-    #     # use emcee backend to save as a HD5 file
-    #     reader = emcee.backends.HDFBackend(f"chains_{run_id}.h5")
-    #     reader.reset(nwalkers, ndim)
-    #     sampler = emcee.EnsembleSampler(nwalkers, ndim, lnprob, args=(x, y, yerr), pool=pool, backend=reader, blobs_dtype=dtype)
-    #     start = time.time()
-    #     sampler.run_mcmc(pos, nsteps, progress=True, store=True)
-    #     end = time.time()
-    #     multi_time = end-start
-
-    #     print('Samples complete. Took {0:.1f} seconds'.format(multi_time))
-
 
     return sampler
```

### Comparing `beansp-1.0.1/beansp/run_model.py` & `beansp-1.4.3/beansp/run_model.py`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp/settle.py` & `beansp-1.4.3/beansp/settle.py`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/beansp.egg-info/PKG-INFO` & `beansp-1.4.3/beansp.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beansp
-Version: 1.0.1
+Version: 1.4.3
 Summary: Bayesian Estimation of Accreting Neutron Stars parameters
 Home-page: https://github.com/adellej/beans
 Author: 
 Author-email: adelle.goodwin@curtin.edu.au
 License: MIT license
 Keywords: beans
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -43,22 +43,24 @@
 * Documentation: https://beans-7.readthedocs.io/en/latest/
 * Repo: https://github.com/adellej/beans
 
 
 Features
 --------
 
-This software uses a Markov Chain Monte Carlo approach to match observations of an accreting neutron star in outburst with a simple ignition model to predict unobservable parameters such as neutron star mass, radius, surface gravity, distance and inclination of the source, and accreted fuel composition. The code is all written in Python 3, except for settle which is a c++ code with a python wrapper. It makes use of Dan Foreman-Mackey's python implementation of MCMC, emcee, available here - https://github.com/dfm/emcee.
+This software uses a Markov Chain Monte Carlo approach to match observations of an accreting neutron star in outburst with a simple ignition model to constrain parameters including the neutron star mass, radius, surface gravity, distance and system inclination, and accreted fuel composition. 
+
+The code is written in Python 3, except for settle which is a C++ code with a python wrapper. It makes use of Dan Foreman-Mackey's python implementation of MCMC, emcee, available at https://github.com/dfm/emcee.
 
 Credits
 -------
 
-Software written by Adelle Goodwin. See Goodwin et al. (2019) - https://arxiv.org/pdf/1907.00996.
+Software written by Adelle Goodwin; for a full description see Goodwin et al. (2019, https://doi.org/10.1093/mnras/stz2638 or preprint at https://arxiv.org/pdf/1907.00996).
 
-This softwate (BEANSp) was based on code written by Duncan Galloway, and uses Dan Foreman-Mackey's python implementation of MCMC, emcee. It depends on pySettle (https://github.com/adellej/pysettle), which was forked from the original settle written by Andrew Cumming.
+The algorithm is based on code written by Duncan Galloway, and depends on pySettle (https://github.com/adellej/pysettle), which was forked from the original settle written by Andrew Cumming.
 
 Package installation and usage
 ------------------------------
 BEANSp is on pyPI (https://pypi.org/project/beansp/) so installation is easy - either straight or in virtual environment:
 
    .. code-block::
```

### Comparing `beansp-1.0.1/beansp.egg-info/SOURCES.txt` & `beansp-1.4.3/beansp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 setup.py
 beansp/__init__.py
 beansp/analyse.py
 beansp/beans.py
 beansp/burstrain.py
 beansp/get_alphas.py
 beansp/get_data.py
-beansp/initialise.py
 beansp/mrprior.py
 beansp/run_emcee.py
 beansp/run_model.py
 beansp/settle.py
 beansp.egg-info/PKG-INFO
 beansp.egg-info/SOURCES.txt
 beansp.egg-info/dependency_links.txt
@@ -47,14 +46,15 @@
 beansp/data/1808/test4_parameterconstraints_pred.txt
 beansp/data/1808/test5_parameterconstraints_pred.txt
 beansp/data/1808/test6_parameterconstraints_pred.txt
 beansp/data/1808/test7_parameterconstraints_pred.txt
 beansp/data/1808/test_acceptancefraction.txt
 docs/conf.py
 docs/contributing.rst
+docs/data.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/readme.rst
 docs/usage.rst
 tests/README.rst
 tests/__init__.py
```

### Comparing `beansp-1.0.1/docs/conf.py` & `beansp-1.4.3/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # absolute, like shown here.
 #
 import os
 import sys
 
 sys.path.insert(0, os.path.abspath('..'))
 
-import beans
+import beansp
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
@@ -58,17 +58,17 @@
 author = u"Adelle Goodwin"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
-version = beans.__version__
+version = beansp.__version__
 # The full version, including alpha/beta/rc tags.
-release = beans.__version__
+release = beansp.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `beansp-1.0.1/setup.py` & `beansp-1.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/tests/README.rst` & `beansp-1.4.3/tests/README.rst`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/tests/data/benchmark/table1.mrt` & `beansp-1.4.3/tests/data/benchmark/table1.mrt`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/tests/data/dummy.h5` & `beansp-1.4.3/tests/data/dummy.h5`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/tests/data/multiprocessing.ecsv` & `beansp-1.4.3/tests/data/benchmark/settle_expected_result.ecsv`

 * *Files 24% similar despite different names*

```diff
@@ -3,67 +3,67 @@
 # datatype:
 # - {name: run, datatype: int64, description: '[1/63] Run ID'}
 # - {name: col1, datatype: float64}
 # - {name: col2, datatype: float64}
 # - {name: col3, datatype: float64}
 # schema: astropy-2.0
 run col1 col2 col3
-1 0.9750249492497147 2.7633298129722212 125.36400406768861
-2 1.1834082259963283 3.5327331387728154 101.17854126804022
-3 1.4326140761813766 4.3939919170268835 85.10718611872517
-4 1.719805957611559 5.301930544118799 73.58923044466951
-5 2.0469420989926155 6.287932602974589 64.98446815863171
-6 2.4258230141618933 7.354141930015495 58.32854138662956
-7 2.8588579557401066 8.501210280139192 53.04184999414501
-8 1.5102597228074401 4.559994887552733 117.67308643642023
-9 1.8776596318436733 5.964356407677315 95.19594110335086
-10 2.311364392458959 7.530909791666819 80.02335510530598
-11 2.8260967039201 9.278069455484495 69.10321173161746
-12 3.4489433715663083 11.305624194014182 60.898052953455974
-13 4.216517223746999 13.674246027671073 54.52610815589443
-14 1.5102597228074401 4.559994887552733 117.67308643642023
-15 0.7885802984224203 1.6586997051654009 168.91491474715858
-16 0.8896576668237084 1.934638967550629 139.36852597116444
-17 1.0317923236535316 2.296717566775029 117.39701262985879
-18 1.1844554735818604 2.6727421750224716 100.88058014486178
-19 1.3476471166086947 3.0430527657358657 88.60437263193684
-20 1.5213672527340338 3.400964082519242 79.27980850482301
-21 0.7885802984224203 1.6586997051654009 168.91491474715858
-22 1.4918200501025023 2.6567727257184246 132.8495656098967
-23 1.7607095916948963 3.3258800853828046 106.59934760307227
-24 2.1108492155855054 4.09874350827555 89.6213499886908
-25 2.5062508862404558 4.896111057299534 77.50886196714266
-26 2.94445144277334 5.723437296241542 68.46491879271578
-27 3.4348395828527045 6.585943938821317 61.48245235183508
-28 0.7885802984224203 1.6586997051654009 168.91491474715858
-29 2.3838309624305425 4.685735374487517 120.36377525684507
-31 3.5685077336848847 7.581381372173076 81.81686269757651
-32 4.315617038888946 9.253725983651432 70.6976281886428
-33 5.1991964734313845 11.086198162482747 62.340993251868966
-34 6.245633811490399 13.177599396995465 55.87312588843211
-35 1.4918200501025023 2.6567727257184246 132.8495656098967
-36 1.9350777065062008 2.3699755486859844 193.39851771375967
-37 1.668708694166463 2.017174155520817 166.57527471213413
-38 1.6154360852097813 2.0030404031074545 140.34762741719726
-39 1.7766832103727905 2.2002774040186486 122.54263062532519
-40 2.0214706749130418 2.4513232026938514 109.99275040419089
-41 2.2820508791010505 2.6973613709456536 99.95982892695585
-42 0.7885802984224203 1.6586997051654009 168.91491474715858
-43 4.393366424563562 3.007273941835494 172.62037106394376
-44 3.569971715679648 2.8055911184090077 128.11022813169654
-45 4.074902008743686 3.343743658600808 105.7933171777798
-46 4.641565794199872 3.879764737288232 90.57476186650587
-47 5.283441396823477 4.4182594082925055 79.57127517536188
-48 6.030891653462239 4.981030071018491 71.44890983430918
-49 1.4918200501025023 2.6567727257184246 132.8495656098967
-50 5.042639507538074 4.610389226927514 129.3863428982813
-51 5.9962343318105775 5.806570734582028 104.08850494076826
-52 7.174363864962495 7.131135166576885 87.43780746932785
-53 8.519642837080193 8.533393220694506 75.587104886647
-54 10.034104870601007 10.005856066420177 66.72906177421763
-55 11.739049696314249 11.555790281205187 59.877829103992006
-56 2.3838309624305425 4.685735374487517 120.36377525684507
-57 16.044749363313866 8.963943890801213 211.98368930291923
-58 11.591808648001928 5.671911783005604 206.2367940969244
-59 9.981316636421273 4.390137116144868 197.8266455256759
-60 9.44377273636636 3.8047477797525464 188.13441263782937
-63 1.9350777065062008 2.3699755486859844 193.39851771375967
+1 0.9750249492497107 2.7633298129722115 94.31579709642531
+2 1.1834082259963619 3.532733138772906 76.12021361088897
+3 1.4326140761813766 4.3939919170268835 64.02916177667193
+4 1.719805957611559 5.301930544118799 55.36379424634554
+5 2.046942098992633 6.287932602974636 48.89012566924173
+6 2.425823014161883 7.35414193001547 43.88263533271835
+7 2.8588579557401066 8.501210280139192 39.90526945011807
+8 1.510259722807471 4.559994887552824 88.52964634134607
+9 1.8776596318436733 5.964356407677315 71.61929081859167
+10 2.311364392458959 7.530909791666819 60.20441496916515
+11 2.8260967039201 9.278069455484495 51.98880288532826
+12 3.4489433715663083 11.305624194014182 45.815770233569715
+13 4.216517223746999 13.674246027671073 41.02192963230789
+14 1.510259722807471 4.559994887552824 88.52964634134607
+15 0.7885802984224203 1.6586997051654009 127.08069548617065
+16 0.8896576668237084 1.934638967550629 104.85189680146907
+17 1.0317923236535316 2.296717566775029 88.32194620192458
+18 1.1844554735818604 2.6727421750224716 75.89604686505676
+19 1.3476471166086947 3.0430527657358657 66.6602195196133
+20 1.5213672527340338 3.400964082519242 59.64501842767448
+21 0.7885802984224203 1.6586997051654009 127.08069548617065
+22 1.4918200501025023 2.6567727257184246 99.94745116505659
+23 1.7607095916949038 3.3258800853828157 80.19847893270993
+24 2.1108492155855054 4.09874350827555 67.42532773982839
+25 2.5062508862404558 4.896111057299534 58.312672388166256
+26 2.94445144277334 5.723437296241542 51.50859241533539
+27 3.4348395828527045 6.585943938821317 46.25543467704933
+28 0.7885802984224203 1.6586997051654009 127.08069548617065
+29 2.3838309624305425 4.685735374487517 90.55394719807188
+31 3.5685077336847826 7.581381372172873 61.55373449211321
+32 4.315617038888946 9.253725983651432 53.188339069309805
+33 5.1991964734313845 11.086198162482747 46.9013455182734
+34 6.245633811490399 13.177599396995465 42.035338960544685
+35 1.4918200501025023 2.6567727257184246 99.94745116505659
+36 1.9350777065062008 2.3699755486859844 145.50058041853586
+37 1.668708694166463 2.017174155520817 125.32050111089453
+38 1.6154360852097813 2.0030404031074545 105.58850962751589
+39 1.7766832103727905 2.2002774040186486 92.19317755262462
+40 2.0214706749130418 2.4513232026938514 82.75145649941187
+41 2.2820508791010505 2.6973613709456536 75.20333299004832
+42 0.7885802984224203 1.6586997051654009 127.08069548617065
+43 4.393366424563562 3.007273941835494 129.86844200657438
+44 3.569971715679648 2.8055911184090077 96.38187909124136
+45 4.074902008743885 3.3437436586009097 79.59207358844377
+46 4.641565794199872 3.879764737288232 68.14261339041097
+47 5.283441396823001 4.418259408292253 59.86429916589838
+48 6.030891653462239 4.981030071018491 53.753554960281825
+49 1.4918200501025023 2.6567727257184246 99.94745116505659
+50 5.042639507537971 4.610389226927433 97.3419455975085
+51 5.9962343318105775 5.806570734582028 78.3094827344786
+52 7.174363864962495 7.131135166576885 65.78257107503283
+53 8.519642837080193 8.533393220694506 56.866866215807704
+54 10.034104870601007 10.005856066420177 50.2026454685812
+55 11.739049696314249 11.555790281205187 45.0482195614723
+56 2.3838309624305425 4.685735374487517 90.55394719807188
+57 16.044749363313866 8.963943890801213 159.4828657295489
+58 11.591808648001928 5.671911783005604 155.15927215726344
+59 9.981316636421273 4.390137116144868 148.83201839653972
+60 9.44377273636636 3.8047477797525464 141.54020702484914
+63 1.9350777065062008 2.3699755486859844 145.50058041853586
```

### Comparing `beansp-1.0.1/tests/data/serial.ecsv` & `beansp-1.4.3/tests/data/multiprocessing.ecsv`

 * *Files 24% similar despite different names*

```diff
@@ -3,67 +3,67 @@
 # datatype:
 # - {name: run, datatype: int64, description: '[1/63] Run ID'}
 # - {name: col1, datatype: float64}
 # - {name: col2, datatype: float64}
 # - {name: col3, datatype: float64}
 # schema: astropy-2.0
 run col1 col2 col3
-1 0.9750249492497147 2.7633298129722212 125.36400406768861
-2 1.1834082259963283 3.5327331387728154 101.17854126804022
-3 1.4326140761813766 4.3939919170268835 85.10718611872517
-4 1.719805957611559 5.301930544118799 73.58923044466951
-5 2.0469420989926155 6.287932602974589 64.98446815863171
-6 2.4258230141618933 7.354141930015495 58.32854138662956
-7 2.8588579557401066 8.501210280139192 53.04184999414501
-8 1.5102597228074401 4.559994887552733 117.67308643642023
-9 1.8776596318436733 5.964356407677315 95.19594110335086
-10 2.311364392458959 7.530909791666819 80.02335510530598
-11 2.8260967039201 9.278069455484495 69.10321173161746
-12 3.4489433715663083 11.305624194014182 60.898052953455974
-13 4.216517223746999 13.674246027671073 54.52610815589443
-14 1.5102597228074401 4.559994887552733 117.67308643642023
-15 0.7885802984224203 1.6586997051654009 168.91491474715858
-16 0.8896576668237084 1.934638967550629 139.36852597116444
-17 1.0317923236535316 2.296717566775029 117.39701262985879
-18 1.1844554735818604 2.6727421750224716 100.88058014486178
-19 1.3476471166086947 3.0430527657358657 88.60437263193684
-20 1.5213672527340338 3.400964082519242 79.27980850482301
-21 0.7885802984224203 1.6586997051654009 168.91491474715858
-22 1.4918200501025023 2.6567727257184246 132.8495656098967
-23 1.7607095916948963 3.3258800853828046 106.59934760307227
-24 2.1108492155855054 4.09874350827555 89.6213499886908
-25 2.5062508862404558 4.896111057299534 77.50886196714266
-26 2.94445144277334 5.723437296241542 68.46491879271578
-27 3.4348395828527045 6.585943938821317 61.48245235183508
-28 0.7885802984224203 1.6586997051654009 168.91491474715858
-29 2.3838309624305425 4.685735374487517 120.36377525684507
-31 3.5685077336848847 7.581381372173076 81.81686269757651
-32 4.315617038888946 9.253725983651432 70.6976281886428
-33 5.1991964734313845 11.086198162482747 62.340993251868966
-34 6.245633811490399 13.177599396995465 55.87312588843211
-35 1.4918200501025023 2.6567727257184246 132.8495656098967
-36 1.9350777065062008 2.3699755486859844 193.39851771375967
-37 1.668708694166463 2.017174155520817 166.57527471213413
-38 1.6154360852097813 2.0030404031074545 140.34762741719726
-39 1.7766832103727905 2.2002774040186486 122.54263062532519
-40 2.0214706749130418 2.4513232026938514 109.99275040419089
-41 2.2820508791010505 2.6973613709456536 99.95982892695585
-42 0.7885802984224203 1.6586997051654009 168.91491474715858
-43 4.393366424563562 3.007273941835494 172.62037106394376
-44 3.569971715679648 2.8055911184090077 128.11022813169654
-45 4.074902008743686 3.343743658600808 105.7933171777798
-46 4.641565794199872 3.879764737288232 90.57476186650587
-47 5.283441396823477 4.4182594082925055 79.57127517536188
-48 6.030891653462239 4.981030071018491 71.44890983430918
-49 1.4918200501025023 2.6567727257184246 132.8495656098967
-50 5.042639507538074 4.610389226927514 129.3863428982813
-51 5.9962343318105775 5.806570734582028 104.08850494076826
-52 7.174363864962495 7.131135166576885 87.43780746932785
-53 8.519642837080193 8.533393220694506 75.587104886647
-54 10.034104870601007 10.005856066420177 66.72906177421763
-55 11.739049696314249 11.555790281205187 59.877829103992006
-56 2.3838309624305425 4.685735374487517 120.36377525684507
-57 16.044749363313866 8.963943890801213 211.98368930291923
-58 11.591808648001928 5.671911783005604 206.2367940969244
-59 9.981316636421273 4.390137116144868 197.8266455256759
-60 9.44377273636636 3.8047477797525464 188.13441263782937
-63 1.9350777065062008 2.3699755486859844 193.39851771375967
+1 0.9750249492497107 2.7633298129722115 94.31579709642531
+2 1.1834082259963619 3.532733138772906 76.12021361088897
+3 1.4326140761813766 4.3939919170268835 64.02916177667193
+4 1.719805957611559 5.301930544118799 55.36379424634554
+5 2.046942098992633 6.287932602974636 48.89012566924173
+6 2.425823014161883 7.35414193001547 43.88263533271835
+7 2.8588579557401066 8.501210280139192 39.90526945011807
+8 1.510259722807471 4.559994887552824 88.52964634134607
+9 1.8776596318436733 5.964356407677315 71.61929081859167
+10 2.311364392458959 7.530909791666819 60.20441496916515
+11 2.8260967039201 9.278069455484495 51.98880288532826
+12 3.4489433715663083 11.305624194014182 45.815770233569715
+13 4.216517223746999 13.674246027671073 41.02192963230789
+14 1.510259722807471 4.559994887552824 88.52964634134607
+15 0.7885802984224203 1.6586997051654009 127.08069548617065
+16 0.8896576668237084 1.934638967550629 104.85189680146907
+17 1.0317923236535316 2.296717566775029 88.32194620192458
+18 1.1844554735818604 2.6727421750224716 75.89604686505676
+19 1.3476471166086947 3.0430527657358657 66.6602195196133
+20 1.5213672527340338 3.400964082519242 59.64501842767448
+21 0.7885802984224203 1.6586997051654009 127.08069548617065
+22 1.4918200501025023 2.6567727257184246 99.94745116505659
+23 1.7607095916949038 3.3258800853828157 80.19847893270993
+24 2.1108492155855054 4.09874350827555 67.42532773982839
+25 2.5062508862404558 4.896111057299534 58.312672388166256
+26 2.94445144277334 5.723437296241542 51.50859241533539
+27 3.4348395828527045 6.585943938821317 46.25543467704933
+28 0.7885802984224203 1.6586997051654009 127.08069548617065
+29 2.3838309624305425 4.685735374487517 90.55394719807188
+31 3.5685077336847826 7.581381372172873 61.55373449211321
+32 4.315617038888946 9.253725983651432 53.188339069309805
+33 5.1991964734313845 11.086198162482747 46.9013455182734
+34 6.245633811490399 13.177599396995465 42.035338960544685
+35 1.4918200501025023 2.6567727257184246 99.94745116505659
+36 1.9350777065062008 2.3699755486859844 145.50058041853586
+37 1.668708694166463 2.017174155520817 125.32050111089453
+38 1.6154360852097813 2.0030404031074545 105.58850962751589
+39 1.7766832103727905 2.2002774040186486 92.19317755262462
+40 2.0214706749130418 2.4513232026938514 82.75145649941187
+41 2.2820508791010505 2.6973613709456536 75.20333299004832
+42 0.7885802984224203 1.6586997051654009 127.08069548617065
+43 4.393366424563562 3.007273941835494 129.86844200657438
+44 3.569971715679648 2.8055911184090077 96.38187909124136
+45 4.074902008743885 3.3437436586009097 79.59207358844377
+46 4.641565794199872 3.879764737288232 68.14261339041097
+47 5.283441396823001 4.418259408292253 59.86429916589838
+48 6.030891653462239 4.981030071018491 53.753554960281825
+49 1.4918200501025023 2.6567727257184246 99.94745116505659
+50 5.042639507537971 4.610389226927433 97.3419455975085
+51 5.9962343318105775 5.806570734582028 78.3094827344786
+52 7.174363864962495 7.131135166576885 65.78257107503283
+53 8.519642837080193 8.533393220694506 56.866866215807704
+54 10.034104870601007 10.005856066420177 50.2026454685812
+55 11.739049696314249 11.555790281205187 45.0482195614723
+56 2.3838309624305425 4.685735374487517 90.55394719807188
+57 16.044749363313866 8.963943890801213 159.4828657295489
+58 11.591808648001928 5.671911783005604 155.15927215726344
+59 9.981316636421273 4.390137116144868 148.83201839653972
+60 9.44377273636636 3.8047477797525464 141.54020702484914
+63 1.9350777065062008 2.3699755486859844 145.50058041853586
```

### Comparing `beansp-1.0.1/tests/test_beans.py` & `beansp-1.4.3/tests/test_beans.py`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/tests/test_benchmark_settle.py` & `beansp-1.4.3/tests/test_benchmark_settle.py`

 * *Files identical despite different names*

### Comparing `beansp-1.0.1/tests/test_get_data.py` & `beansp-1.4.3/tests/test_get_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Tests the data reading in routine """
 import numpy as np
+from beansp import Beans
 from beansp.get_data import get_obs
 import pathlib
 
 def test_get_obs():
 
     path_to_data_file_obs = (
             pathlib.Path(__file__).resolve().parent.parent / "beansp/data" / "1808_obs.txt"
@@ -14,22 +15,27 @@
         )
 
     path_to_data_file_gti = (
             pathlib.Path(__file__).resolve().parent.parent / "beansp/data" / "1808_gti.txt"
         )
 
 
-    bstart0, bstart, fluen, fluene, obs, obs_err, pflux, pfluxe, tobs, st, et = get_obs(ref_ind=1, bc=2.21, obsname=path_to_data_file_obs, burstname=path_to_data_file_bursts, gtiname=path_to_data_file_gti)
+    # bstart0, bstart, fluen, fluene, obs, obs_err, pflux, pfluxe, tobs, st, et = get_obs(ref_ind=1, bc=2.21, obsname=path_to_data_file_obs, burstname=path_to_data_file_bursts, gtiname=path_to_data_file_gti)
+    B = Beans(obsname=path_to_data_file_obs, burstname=path_to_data_file_bursts, gtiname=path_to_data_file_gti)
+    get_obs(B)
+
+    bstart_err = B.bstart_err
 
     obsexp = [0.0, 2.770649999998568, 4.013149999998859, 2.6196, 2.6486, 2.9904, 3.4599, 107.0, 105.7, 121.1] 
-    obserrexp = [0.0069, 0.0069, 0.0069, 0.0207, 0.0178, 0.0173, 0.0221, 2.0, 1.9, 2.3]
+    # obserrexp = [0.0069, 0.0069, 0.0069, 0.0207, 0.0178, 0.0173, 0.0221, 2.0, 1.9, 2.3]
+    obserrexp = [bstart_err, bstart_err, bstart_err, 0.0207, 0.0178, 0.0173, 0.0221, 2.0, 1.9, 2.3]
 
-    result = np.allclose(obsexp, obs)
+    result = np.allclose(obsexp, B.y)
     assert result
-    result = np.allclose(obserrexp, obs_err)
+    result = np.allclose(obserrexp, B.yerr)
     assert result
 
     return
 
 
 if __name__ == "__main__":
     # introspect and run all the functions starting with 'test'
```

### Comparing `beansp-1.0.1/tests/test_runmodel.py` & `beansp-1.4.3/tests/test_runmodel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ test to see if runmodel functions as expected """
 import sys, os
 myPath = os.path.dirname(os.path.abspath(__file__))
 sys.path.insert(0, myPath + '../beans')
 from beansp.burstrain import *
 from beansp.run_model import runmodel
 import numpy as np
+from beansp import Beans
 from beansp.get_data import get_obs
 import pathlib
 
 
 def test_run_model():
 
     numburstssim = 3 # this needs to be an integer value of half the number of bursts you want to simulate. I.e. simulate this many from the reference burst in either direction. Don't forget to account for missed bursts!
@@ -25,30 +26,41 @@
         )
 
     path_to_data_file_gti = (
             pathlib.Path(__file__).resolve().parent.parent / "beansp/data" / "1808_gti.txt"
         )
 
 
-    bstart0, bstart, fluen, fluene, obs, obs_err, pflux, pfluxe, tobs, st, et = get_obs(ref_ind=1, bc=2.21, obsname=path_to_data_file_obs, burstname=path_to_data_file_bursts, gtiname=path_to_data_file_gti)
+    # bstart0, bstart, fluen, fluene, obs, obs_err, pflux, pfluxe, tobs, st, et = get_obs(ref_ind=1, bc=2.21, obsname=path_to_data_file_obs, burstname=path_to_data_file_bursts, gtiname=path_to_data_file_gti)
+    B = Beans(ref_ind=1, bc=2.21, obsname=path_to_data_file_obs, burstname=path_to_data_file_bursts)#, gtiname=path_to_data_file_gti)
 
     ref_ind = 1
-    tref = bstart[ref_ind]
+    # tref = bstart[ref_ind]
+    tref = B.tref
     gti_checking =0
     # this is for emcee:
-    y = obs
-    yerr = obs_err
+    y = B.y
+    yerr = B.yerr
+    # y = obs
+    # yerr = obs_err
     x = 0 # in our case, we do not require x (independent variables), however for input into MCMC we need to define a x
 
     # updated call to include the train, numburstsobs parameter, and add the
     # full model which is now also output
-    test, valid, full_model = runmodel(theta,y,tref,bstart,pflux, pfluxe, tobs,numburstssim,len(bstart),ref_ind,gti_checking, 1, st, et)
+    # test, valid, full_model = runmodel(theta,y,tref,bstart,pflux, pfluxe, tobs,numburstssim,len(bstart),ref_ind,gti_checking, 1, st, et)
+    test, valid, full_model = runmodel(theta,B.y,B.tref,B.bstart,B.pflux, B.pfluxe, B.tobs, B.numburstssim,
+        len(B.bstart), B.ref_ind, gti_checking, 1, B.st, B.et)
 
     #exp = [  0.37596756  , 2.57382977 ,  3.6951732  ,  5.22042564 ,  5.49339669, 5.76917402  , 7.5398804  ,129.9739876,  139.81100404 ,155.46956035]
 
     
-    exp = [0.36955303, 2.56867184, 3.51029901, 5.24244931, 5.39297104, 5.67404108, 6.33264429, 130.38129617, 140.42569944, 155.456677] 
+    # updated here with the new (corrected) alpha calculation, for
+    # v0.1.3 and later
+    exp = [0.36955303, 2.56867184, 3.51029901, 5.24244931, 5.39297104, 5.67404108, 6.33264429, 
+        # 130.38129617, 140.42569944, 155.456677] 
+        86.19418202, 92.83446824, 102.77134457]
     result = np.allclose(test, exp)
+    print (test)
 
     assert result
 
     return
```

### Comparing `beansp-1.0.1/tests/test_sft_beans.py` & `beansp-1.4.3/tests/test_sft_beans.py`

 * *Files identical despite different names*

