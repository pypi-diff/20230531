# Comparing `tmp/frouros-0.2.7.tar.gz` & `tmp/frouros-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frouros-0.2.7.tar", last modified: Thu May 11 14:08:52 2023, max compression
+gzip compressed data, was "frouros-0.3.0.tar", last modified: Wed May 31 15:32:53 2023, max compression
```

## Comparing `frouros-0.2.7.tar` & `frouros-0.3.0.tar`

### file list

```diff
@@ -1,132 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.642778 frouros-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-05-11 14:08:39.000000 frouros-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-11 14:08:39.000000 frouros-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7655 2023-05-11 14:08:52.642778 frouros-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-05-11 14:08:39.000000 frouros-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.630777 frouros-0.2.7/frouros/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)      329 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2136 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/callbacks/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5287 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/batch/permutation_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/batch/reset_drift.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/callbacks/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/streaming/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/streaming/history.py
--rw-r--r--   0 runner    (1001) docker     (122)     6385 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/streaming/msprt.py
--rw-r--r--   0 runner    (1001) docker     (122)     2142 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/callbacks/streaming/warning_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/common/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5680 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/datasets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/datasets/real.py
--rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/datasets/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/detectors/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2226 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/detectors/concept_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6144 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/detectors/concept_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      567 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5351 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/
--rw-r--r--   0 runner    (1001) docker     (122)      525 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10776 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2736 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/ddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4794 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py
--rw-r--r--   0 runner    (1001) docker     (122)    12400 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/eddm.py
--rw-r--r--   0 runner    (1001) docker     (122)    23064 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/hddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9641 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/rddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7471 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/stepd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros/detectors/concept_drift/streaming/window_based/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/window_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19323 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/window_based/adwin.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/window_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/streaming/window_based/kswin.py
--rw-r--r--   0 runner    (1001) docker     (122)      506 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/concept_drift/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/detectors/data_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/detectors/data_drift/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3429 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8762 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1887 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/emd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2284 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
--rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/js.py
--rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/kl.py
--rw-r--r--   0 runner    (1001) docker     (122)     8142 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/mmd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/psi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2493 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
--rw-r--r--   0 runner    (1001) docker     (122)     2424 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/cvm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/ks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/detectors/data_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/detectors/data_drift/streaming/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/streaming/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/streaming/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3114 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/streaming/distance_based/mmd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/detectors/data_drift/streaming/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/streaming/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7320 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/detectors/data_drift/streaming/statistical_test/ks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/metrics/prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12327 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8975 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/integration/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/integration/test_concept_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)    14909 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/integration/test_data_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/integration/test_real.py
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/integration/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.638778 frouros-0.2.7/frouros/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/tests/unit/metrics/test_prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.642778 frouros-0.2.7/frouros/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21163 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     7352 2023-05-11 14:08:39.000000 frouros-0.2.7/frouros/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 14:08:52.634777 frouros-0.2.7/frouros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7655 2023-05-11 14:08:52.000000 frouros-0.2.7/frouros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-05-11 14:08:52.000000 frouros-0.2.7/frouros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 14:08:52.000000 frouros-0.2.7/frouros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 14:08:52.000000 frouros-0.2.7/frouros.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-05-11 14:08:52.000000 frouros-0.2.7/frouros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-11 14:08:52.000000 frouros-0.2.7/frouros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-05-11 14:08:39.000000 frouros-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 14:08:52.642778 frouros-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-05-11 14:08:39.000000 frouros-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-05-31 15:32:40.000000 frouros-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-31 15:32:40.000000 frouros-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    21352 2023-05-31 15:32:53.939460 frouros-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    19989 2023-05-31 15:32:40.000000 frouros-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.931460 frouros-0.3.0/frouros/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.931460 frouros-0.3.0/frouros/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)      329 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2136 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.931460 frouros-0.3.0/frouros/callbacks/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5617 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/batch/permutation_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/batch/reset_drift.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/callbacks/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/streaming/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/streaming/history.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6385 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/streaming/msprt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2142 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/callbacks/streaming/warning_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/common/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5680 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/datasets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/datasets/real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/datasets/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/detectors/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/detectors/concept_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6144 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/detectors/concept_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5351 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10783 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2752 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4810 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12416 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23079 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9657 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19323 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/adwin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5958 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/kswin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7877 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/stepd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/detectors/data_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.935460 frouros-0.3.0/frouros/detectors/data_drift/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3429 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8762 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1887 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1775 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/emd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2284 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/js.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2143 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/kl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8142 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/mmd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/psi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2493 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2424 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/cvm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/ks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/detectors/data_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/detectors/data_drift/streaming/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/streaming/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/streaming/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3114 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/streaming/distance_based/mmd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/detectors/data_drift/streaming/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/streaming/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7320 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/detectors/data_drift/streaming/statistical_test/ks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/metrics/prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12327 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9103 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/integration/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5330 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/integration/test_concept_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14909 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/integration/test_data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/integration/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/integration/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/tests/unit/metrics/test_prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.939460 frouros-0.3.0/frouros/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21163 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/utils/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7742 2023-05-31 15:32:40.000000 frouros-0.3.0/frouros/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 15:32:53.931460 frouros-0.3.0/frouros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    21352 2023-05-31 15:32:53.000000 frouros-0.3.0/frouros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4713 2023-05-31 15:32:53.000000 frouros-0.3.0/frouros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 15:32:53.000000 frouros-0.3.0/frouros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 15:32:53.000000 frouros-0.3.0/frouros.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-05-31 15:32:53.000000 frouros-0.3.0/frouros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-31 15:32:53.000000 frouros-0.3.0/frouros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-05-31 15:32:40.000000 frouros-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 15:32:53.939460 frouros-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-05-31 15:32:40.000000 frouros-0.3.0/setup.py
```

### Comparing `frouros-0.2.7/LICENSE` & `frouros-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/callbacks/base.py` & `frouros-0.3.0/frouros/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/callbacks/batch/base.py` & `frouros-0.3.0/frouros/callbacks/batch/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/callbacks/batch/permutation_test.py` & `frouros-0.3.0/frouros/callbacks/batch/permutation_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Permutation test on batch data callback module."""
 
 import multiprocessing
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import numpy as np  # type: ignore
+from scipy.stats import norm  # type: ignore
 
 from frouros.callbacks.batch.base import BatchCallback
-from frouros.utils.stats import permutation
+from frouros.utils.stats import permutation, z_score
 
 
 class PermutationTestOnBatchData(BatchCallback):
     """Permutation test on batch data callback class."""
 
     def __init__(
         self,
@@ -116,15 +117,22 @@
             statistic=statistic,
             statistical_args=statistic_args,
             num_permutations=num_permutations,
             num_jobs=num_jobs,
             random_state=random_state,
             verbose=verbose,
         )
-        p_value = (observed_statistic < permuted_statistic).mean()  # type: ignore
+        permuted_statistic = np.array(permuted_statistic)
+        # Use z-score to calculate p-value
+        observed_z_score = z_score(
+            value=observed_statistic,
+            mean=permuted_statistic.mean(),  # type: ignore
+            std=permuted_statistic.std(),  # type: ignore
+        )
+        p_value = norm.sf(np.abs(observed_z_score)) * 2
         return permuted_statistic, p_value
 
     def on_compare_end(self, **kwargs) -> None:
         """On compare end method."""
         X_ref, X_test = kwargs["X_ref"], kwargs["X_test"]  # noqa: N806
         observed_statistic = kwargs["result"][0]
         permuted_statistics, p_value = self._calculate_p_value(
```

### Comparing `frouros-0.2.7/frouros/callbacks/batch/reset_drift.py` & `frouros-0.3.0/frouros/callbacks/batch/reset_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/callbacks/streaming/base.py` & `frouros-0.3.0/frouros/callbacks/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/callbacks/streaming/history.py` & `frouros-0.3.0/frouros/callbacks/streaming/history.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/callbacks/streaming/msprt.py` & `frouros-0.3.0/frouros/callbacks/streaming/msprt.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/callbacks/streaming/warning_samples.py` & `frouros-0.3.0/frouros/callbacks/streaming/warning_samples.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/datasets/base.py` & `frouros-0.3.0/frouros/datasets/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/datasets/real.py` & `frouros-0.3.0/frouros/datasets/real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/datasets/synthetic.py` & `frouros-0.3.0/frouros/datasets/synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/base.py` & `frouros-0.3.0/frouros/detectors/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,9 +70,10 @@
         """Repr method.
 
         :return: repr value
         :rtype: str
         """
         return (
             f"{self.__class__.__name__}"
-            f"(callbacks=[{', '.join(self.callbacks)}])"  # type: ignore
+            f"(callbacks=["
+            f"{', '.join([*map(str, self.callbacks)])}])"  # type: ignore
         )
```

### Comparing `frouros-0.2.7/frouros/detectors/concept_drift/__init__.py` & `frouros-0.3.0/frouros/detectors/concept_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/concept_drift/base.py` & `frouros-0.3.0/frouros/detectors/concept_drift/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/concept_drift/streaming/__init__.py` & `frouros-0.3.0/frouros/detectors/concept_drift/streaming/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,35 +5,35 @@
     CUSUM,
     CUSUMConfig,
     GeometricMovingAverage,
     GeometricMovingAverageConfig,
     PageHinkley,
     PageHinkleyConfig,
 )
-from .ddm_based import (
+from .statistical_process_control import (
     DDM,
     DDMConfig,
     ECDDWT,
     ECDDWTConfig,
     EDDM,
     EDDMConfig,
     HDDMA,
     HDDMAConfig,
     HDDMW,
     HDDMWConfig,
     RDDM,
     RDDMConfig,
-    STEPD,
-    STEPDConfig,
 )
 from .window_based import (
     ADWIN,
     ADWINConfig,
     KSWIN,
     KSWINConfig,
+    STEPD,
+    STEPDConfig,
 )
 
 __all__ = [
     "ADWIN",
     "ADWINConfig",
     "CUSUM",
     "CUSUMConfig",
```

### Comparing `frouros-0.2.7/frouros/detectors/concept_drift/streaming/base.py` & `frouros-0.3.0/frouros/detectors/concept_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/base.py` & `frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py` & `frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py` & `frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py` & `frouros-0.3.0/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/base.py` & `frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Supervised DDM based base module."""
+"""Concept drift SPC (statistical process control) base module."""
 
 import abc
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np  # type: ignore
 
 from frouros.callbacks import Callback
@@ -10,16 +10,16 @@
     ConceptDriftStreamingBaseConfig,
     ConceptDriftStreamingBase,
 )
 from frouros.detectors.concept_drift.exceptions import InvalidAverageRunLengthError
 from frouros.utils.stats import Mean
 
 
-class DDMBaseConfig(ConceptDriftStreamingBaseConfig):
-    """Class representing a DDM based configuration class."""
+class SPCBaseConfig(ConceptDriftStreamingBaseConfig):
+    """Class representing a SPC configuration class."""
 
     def __init__(
         self,
         warning_level: float = 2.0,
         drift_level: float = 3.0,
         min_num_instances: int = 30,
     ) -> None:
@@ -78,28 +78,28 @@
         :raises ValueError: Value error exception
         """
         if value <= 0.0:
             raise ValueError("warning level must be greater than 0.0.")
         self._warning_level = value
 
 
-class DDMBased(ConceptDriftStreamingBase):
-    """Abstract class representing a DDM based estimator."""
+class SPCBase(ConceptDriftStreamingBase):
+    """Abstract class representing an SPC estimator."""
 
-    config_type = DDMBaseConfig
+    config_type = SPCBaseConfig
 
     def __init__(
         self,
-        config: Optional[DDMBaseConfig] = None,
+        config: Optional[SPCBaseConfig] = None,
         callbacks: Optional[Union[Callback, List[Callback]]] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
-        :type config: Optional[DDMBaseConfig]
+        :type config: Optional[SPCBaseConfig]
         :param callbacks: callbacks
         :type callbacks: Optional[Union[Callback, List[Callback]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
@@ -141,28 +141,28 @@
         return {**super().status, "warning": self.warning}
 
     @abc.abstractmethod
     def _update(self, value: Union[int, float], **kwargs) -> None:
         pass
 
 
-class DDMErrorBased(DDMBased):
-    """Abstract class representing a DDM error based estimator."""
+class SPCErrorBase(SPCBase):
+    """Abstract class representing a SPC error estimator."""
 
-    config_type = DDMBaseConfig
+    config_type = SPCBaseConfig
 
     def __init__(
         self,
-        config: Optional[DDMBaseConfig] = None,
+        config: Optional[SPCBaseConfig] = None,
         callbacks: Optional[Union[Callback, List[Callback]]] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
-        :type config: Optional[DDMBaseConfig]
+        :type config: Optional[SPCBaseConfig]
         :param callbacks: callbacks
         :type callbacks: Optional[Union[Callback, List[Callback]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
```

### Comparing `frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/ddm.py` & `frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """DDM (Drift detection method) module."""
 
 from contextlib import suppress
 from typing import Union
 
-from frouros.detectors.concept_drift.streaming.ddm_based.base import (
-    DDMBaseConfig,
-    DDMErrorBased,
+from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
+    SPCBaseConfig,
+    SPCErrorBase,
 )
 
 
-class DDMConfig(DDMBaseConfig):
+class DDMConfig(SPCBaseConfig):
     """DDM (Drift detection method) [gama2004learning]_ configuration.
 
     :References:
 
     .. [gama2004learning] Gama, Joao, et al.
         "Learning with drift detection."
         Advances in Artificial Intelligence–SBIA 2004: 17th Brazilian Symposium on
         Artificial Intelligence, Sao Luis, Maranhao, Brazil, September 29-Ocotber 1,
         2004. Proceedings 17. Springer Berlin Heidelberg, 2004.
     """
 
 
-class DDM(DDMErrorBased):
+class DDM(SPCErrorBase):
     """DDM (Drift detection method) [gama2004learning]_ detector.
 
     :References:
 
     .. [gama2004learning] Gama, Joao, et al.
         "Learning with drift detection."
         Advances in Artificial Intelligence–SBIA 2004: 17th Brazilian Symposium on
```

### Comparing `frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py` & `frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ECDD (EWMA for Concept Drift Detection) module."""
 
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 
 from frouros.callbacks import Callback
-from frouros.detectors.concept_drift.streaming.ddm_based.base import (
-    DDMBased,
+from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
+    SPCBase,
     ECDDBaseConfig,
 )
 from frouros.utils.stats import EWMA, Mean
 
 
 class ECDDWTConfig(ECDDBaseConfig):
     """ECDDWT (EWMA Concept Drift Detection Warning) [ross2012exponentially]_ configuration.
@@ -19,15 +19,15 @@
 
     .. [ross2012exponentially] Ross, Gordon J., et al.
         "Exponentially weighted moving average charts for detecting concept drift."
         Pattern recognition letters 33.2 (2012): 191-198.
     """
 
 
-class ECDDWT(DDMBased):
+class ECDDWT(SPCBase):
     """ECDDWT (EWMA Concept Drift Detection Warning) [ross2012exponentially]_ detector.
 
     :References:
 
     .. [ross2012exponentially] Ross, Gordon J., et al.
         "Exponentially weighted moving average charts for detecting concept drift."
         Pattern recognition letters 33.2 (2012): 191-198.
```

### Comparing `frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/eddm.py` & `frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import copy
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 
 from frouros.callbacks import Callback
-from frouros.detectors.concept_drift.streaming.ddm_based.base import (
-    DDMBaseConfig,
-    DDMBased,
+from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
+    SPCBaseConfig,
+    SPCBase,
 )
 
 
-class EDDMConfig(DDMBaseConfig):
+class EDDMConfig(SPCBaseConfig):
     """EDDM (Early drift detection method) [baena2006early]_ configuration.
 
     :References:
 
     .. [baena2006early] Baena-Garcıa, Manuel, et al. "Early drift detection method."
         Fourth international workshop on knowledge discovery from data streams.
         Vol. 6. 2006.
@@ -129,15 +129,15 @@
         if value < 0:
             raise ValueError(
                 "min_num_misclassified_instances must be greater or equal than 0."
             )
         self._min_num_misclassified_instances = value
 
 
-class EDDM(DDMBased):
+class EDDM(SPCBase):
     """EDDM (Early drift detection method) [baena2006early]_ detector.
 
     :References:
 
     .. [baena2006early] Baena-Garcıa, Manuel, et al. "Early drift detection method."
         Fourth international workshop on knowledge discovery from data streams.
         Vol. 6. 2006.
```

### Comparing `frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/hddm.py` & `frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 import copy
 from typing import List, Optional, Tuple, Union
 
 import numpy as np  # type: ignore
 
 from frouros.callbacks import Callback
-from frouros.detectors.concept_drift.streaming.ddm_based.base import (
-    DDMBaseConfig,
-    DDMBased,
+from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
+    SPCBaseConfig,
+    SPCBase,
 )
 from frouros.utils.stats import EWMA, Mean
 
 
-class HDDMBaseConfig(DDMBaseConfig):
+class HDDMBaseConfig(SPCBaseConfig):
     """HDDM (Hoeffding's drift detection method) [frias2014online]_ configuration.
 
     :References:
 
     .. [frias2014online] Frias-Blanco, Isvani, et al.
         "Online and non-parametric drift detection methods based on Hoeffding’s bounds."
         IEEE Transactions on Knowledge and Data Engineering 27.3 (2014): 810-823.
@@ -314,15 +314,15 @@
         """
         super().update_cut_point(epsilon_z=epsilon_z)
         epsilon_y = self.hoeffding_error_bound(num_values=self.y.num_values)
         if self.y.mean - epsilon_y <= self.z.mean - epsilon_z:
             self.y = copy.deepcopy(self.z)
 
 
-class HDDMA(DDMBased):
+class HDDMA(SPCBase):
     """HDDM-A (Hoeffding's drift detection method with A-Test) [frias2014online]_ detector.
 
     :References:
 
     .. [frias2014online] Frias-Blanco, Isvani, et al.
         "Online and non-parametric drift detection methods based on Hoeffding’s bounds."
         IEEE Transactions on Knowledge and Data Engineering 27.3 (2014):
@@ -610,15 +610,15 @@
             self.decrease_cut_point = ewma_minus_epsilon
             self.sample_decrease_1 = copy.deepcopy(self.total)
             self.sample_decrease_2 = SampleInfo(lambda_=self.lambda_)
         else:
             self.sample_decrease_2.update(value=value)
 
 
-class HDDMW(DDMBased):
+class HDDMW(SPCBase):
     """HDDM-W (Hoeffding's drift detection method with W-Test) [frias2014online]_ detector.
 
     :References:
 
     .. [frias2014online] Frias-Blanco, Isvani, et al.
         "Online and non-parametric drift detection methods based on Hoeffding’s bounds."
         IEEE Transactions on Knowledge and Data Engineering 27.3 (2014):
```

### Comparing `frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/rddm.py` & `frouros-0.3.0/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """RDDM (Reactive Drift detection method) module."""
 
 from typing import List, Optional, Union
 
 from frouros.callbacks import Callback
-from frouros.detectors.concept_drift.streaming.ddm_based.base import (
-    DDMBaseConfig,
-    DDMErrorBased,
+from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
+    SPCBaseConfig,
+    SPCErrorBase,
 )
 from frouros.utils.data_structures import CircularQueue
 from frouros.utils.stats import Mean
 
 
-class RDDMConfig(DDMBaseConfig):
+class RDDMConfig(SPCBaseConfig):
     """RDDM (Reactive Drift detection method) [barros2017rddm]_ configuration.
 
     :References:
 
     .. [barros2017rddm] Barros, Roberto SM, et al.
         "RDDM: Reactive drift detection method."
         Expert Systems with Applications 90 (2017): 344-355.
@@ -106,15 +106,15 @@
 
         :param value: value to be set
         :type value: int
         """
         self._max_num_instances_warning = value
 
 
-class RDDM(DDMErrorBased):
+class RDDM(SPCErrorBase):
     """RDDM (Reactive Drift detection method) [barros2017rddm]_ detector.
 
     :References:
 
     .. [barros2017rddm] Barros, Roberto SM, et al.
         "RDDM: Reactive drift detection method."
         Expert Systems with Applications 90 (2017): 344-355.
```

### Comparing `frouros-0.2.7/frouros/detectors/concept_drift/streaming/ddm_based/stepd.py` & `frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/stepd.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 from scipy.stats import norm  # type: ignore
 
 from frouros.callbacks import Callback
-from frouros.detectors.concept_drift.streaming.ddm_based.base import (
-    DDMBaseConfig,
-    DDMBased,
+from frouros.detectors.concept_drift.streaming.window_based.base import (
+    WindowBaseConfig,
+    WindowBased,
 )
 from frouros.utils.data_structures import AccuracyQueue
 
 
-class STEPDConfig(DDMBaseConfig):
+class STEPDConfig(WindowBaseConfig):
     """STEPD (Statistical test of equal proportions) [nishida2007detecting]_ configuration.
 
     :References:
 
     .. [nishida2007detecting] Nishida, Kyosuke, and Koichiro Yamauchi.
         "Detecting concept drift using statistical testing." Discovery science.
         Vol. 4755. 2007.
@@ -84,15 +84,15 @@
         if value <= 0.0:
             raise ValueError("alpha_w must be greater than 0.0.")
         if value <= self.alpha_d:
             raise ValueError("alpha_w must be greater than alpha_d.")
         self._alpha_w = value
 
 
-class STEPD(DDMBased):
+class STEPD(WindowBased):
     """STEPD (Statistical test of equal proportions) [nishida2007detecting]_ detector.
 
     :References:
 
     .. [nishida2007detecting] Nishida, Kyosuke, and Koichiro Yamauchi.
         "Detecting concept drift using statistical testing." Discovery science.
         Vol. 4755. 2007.
@@ -118,19 +118,38 @@
         )
         self.additional_vars = {
             "correct_total": 0,
             # FIXME include get method in AccuracyQueue  # pylint: disable=fixme
             "window_accuracy": AccuracyQueue(max_len=self.config.min_num_instances),
             **self.additional_vars,  # type: ignore
         }
+        self.warning = False
         self._set_additional_vars_callback()
         self._min_num_instances = 2 * self.config.min_num_instances
         self._distribution = norm()
 
     @property
+    def warning(self) -> bool:
+        """Warning property.
+
+        :return: warning
+        :rtype: bool
+        """
+        return self._warning
+
+    @warning.setter
+    def warning(self, value: bool) -> None:
+        """Warning setter.
+
+        :param value: value to be set
+        :type value: bool
+        """
+        self._warning = value
+
+    @property
     def correct_total(self) -> int:
         """Number of correct labels property.
 
         :return: accuracy scorer function
         :rtype: int
         """
         return self._additional_vars["correct_total"]
```

### Comparing `frouros-0.2.7/frouros/detectors/concept_drift/streaming/window_based/adwin.py` & `frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/adwin.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/concept_drift/streaming/window_based/base.py` & `frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/concept_drift/streaming/window_based/kswin.py` & `frouros-0.3.0/frouros/detectors/concept_drift/streaming/window_based/kswin.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/__init__.py` & `frouros-0.3.0/frouros/detectors/data_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/base.py` & `frouros-0.3.0/frouros/detectors/data_drift/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/batch/__init__.py` & `frouros-0.3.0/frouros/detectors/data_drift/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/batch/base.py` & `frouros-0.3.0/frouros/detectors/data_drift/batch/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/base.py` & `frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py` & `frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/emd.py` & `frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/emd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py` & `frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py` & `frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/js.py` & `frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/js.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/kl.py` & `frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/kl.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/mmd.py` & `frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/mmd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/batch/distance_based/psi.py` & `frouros-0.3.0/frouros/detectors/data_drift/batch/distance_based/psi.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/base.py` & `frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/chisquare.py` & `frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/chisquare.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/cvm.py` & `frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/cvm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/ks.py` & `frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/ks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py` & `frouros-0.3.0/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/streaming/base.py` & `frouros-0.3.0/frouros/detectors/data_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/streaming/distance_based/base.py` & `frouros-0.3.0/frouros/detectors/data_drift/streaming/distance_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/streaming/distance_based/mmd.py` & `frouros-0.3.0/frouros/detectors/data_drift/streaming/distance_based/mmd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/streaming/statistical_test/base.py` & `frouros-0.3.0/frouros/detectors/data_drift/streaming/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/detectors/data_drift/streaming/statistical_test/ks.py` & `frouros-0.3.0/frouros/detectors/data_drift/streaming/statistical_test/ks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/metrics/base.py` & `frouros-0.3.0/frouros/metrics/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/metrics/prequential_error.py` & `frouros-0.3.0/frouros/metrics/prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/tests/conftest.py` & `frouros-0.3.0/frouros/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/tests/integration/test_callback.py` & `frouros-0.3.0/frouros/tests/integration/test_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,17 @@
     HDDMW,
     KSWIN,
     PageHinkley,
     RDDM,
     STEPD,
 )
 from frouros.detectors.concept_drift.base import ConceptDriftBase
-from frouros.detectors.concept_drift.streaming.ddm_based.base import DDMBased
+from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
+    SPCBase,
+)
 from frouros.detectors.data_drift.batch import (
     BhattacharyyaDistance,
     CVMTest,
     EMD,
     HellingerDistance,
     HINormalizedComplement,
     JS,
@@ -48,21 +50,21 @@
 from frouros.detectors.data_drift.streaming import MMD as MMDStreaming  # noqa: N811
 
 
 @pytest.mark.parametrize(
     "detector_class, expected_distance, expected_p_value",
     [
         (BhattacharyyaDistance, 0.55516059, 0.0),
-        (EMD, 3.85346006, 0.0),
-        (HellingerDistance, 0.74509099, 0.0),
-        (HINormalizedComplement, 0.78, 0.0),
-        (JS, 0.67010107, 0.0),
-        (KL, np.inf, 0.0),
-        (MMD, 0.69509004, 0.0),
-        (PSI, 461.20379435, 0.0),
+        (EMD, 3.85346006, 9.21632493e-101),
+        (HellingerDistance, 0.74509099, 3.13808126e-50),
+        (HINormalizedComplement, 0.78, 1.31340683e-55),
+        (JS, 0.67010107, 2.30485343e-63),
+        (KL, np.inf, np.nan),
+        (MMD, 0.69509004, 2.53277069e-137),
+        (PSI, 461.20379435, 4.45088795e-238),
     ],
 )
 def test_batch_permutation_test_data_univariate_different_distribution(
     X_ref_univariate: np.ndarray,  # noqa: N803
     X_test_univariate: np.ndarray,
     detector_class: DataDriftBatchBase,
     expected_distance: float,
@@ -94,15 +96,19 @@
             )
         ]
     )
     _ = detector.fit(X=X_ref_univariate)
     distance, callback_logs = detector.compare(X=X_test_univariate)
 
     assert np.isclose(distance, expected_distance)
-    assert np.isclose(callback_logs[permutation_test_name]["p_value"], expected_p_value)
+    assert np.isclose(
+        callback_logs[permutation_test_name]["p_value"],
+        expected_p_value,
+        equal_nan=True,
+    )
 
 
 @pytest.mark.parametrize(
     "detector_class",
     [CVMTest, KSTest, WelchTTest],
 )
 def test_batch_reset_on_data_drift(
@@ -184,30 +190,29 @@
     [
         DDM,
         ECDDWT,
         EDDM,
         HDDMA,
         HDDMW,
         RDDM,
-        STEPD,
     ],  # pylint: disable=too-many-locals
 )
 def test_streaming_warning_samples_buffer_on_concept_drift(
     dataset_simple: Tuple[Tuple[np.ndarray, np.ndarray], Tuple[np.ndarray, np.ndarray]],
     model: sklearn.pipeline.Pipeline,
-    detector_class: DDMBased,
+    detector_class: SPCBase,
 ):
     """Test streaming warning samples buffer on concept drift callback.
 
     :param dataset_simple: dataset with concept drift
     :type dataset_simple: Tuple[Tuple[numpy.ndarray, numpy.ndarray],
     :param model: trained model
     :type model: sklearn.pipeline.Pipeline
     :param detector_class: concept drift detector
-    :type detector_class: DDMBased
+    :type detector_class: SPCBase
     """
     _, test = dataset_simple  # noqa: N806
 
     detector = detector_class(
         callbacks=WarningSamplesBuffer(name="samples"),  # type: ignore
     )
```

### Comparing `frouros-0.2.7/frouros/tests/integration/test_concept_drift.py` & `frouros-0.3.0/frouros/tests/integration/test_concept_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/tests/integration/test_data_drift.py` & `frouros-0.3.0/frouros/tests/integration/test_data_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/tests/integration/test_real.py` & `frouros-0.3.0/frouros/tests/integration/test_real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/tests/integration/test_synthetic.py` & `frouros-0.3.0/frouros/tests/integration/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/tests/unit/metrics/test_prequential_error.py` & `frouros-0.3.0/frouros/tests/unit/metrics/test_prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/utils/data_structures.py` & `frouros-0.3.0/frouros/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/utils/decorators.py` & `frouros-0.3.0/frouros/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `frouros-0.2.7/frouros/utils/stats.py` & `frouros-0.3.0/frouros/utils/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,7 +259,26 @@
     with Pool(processes=num_jobs) as pool:
         permuted_statistics = pool.starmap_async(
             partial(statistic, **statistical_args),
             iterable=tqdm(permuted_data) if verbose else permuted_data,
         ).get()
 
     return permuted_statistics
+
+
+def z_score(
+    value: np.ndarray,
+    mean: float,
+    std: float,
+) -> np.ndarray:
+    """Z-score method.
+
+    :param value: value to use to compute the z-score
+    :type value: np.ndarray
+    :param mean: mean value
+    :type mean: float
+    :param std: standard deviation value
+    :type std: float
+    :return: z-score
+    :rtype: np.ndarray
+    """
+    return (value - mean) / std
```

### Comparing `frouros-0.2.7/frouros.egg-info/SOURCES.txt` & `frouros-0.3.0/frouros.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -29,34 +29,33 @@
 frouros/datasets/real.py
 frouros/datasets/synthetic.py
 frouros/detectors/__init__.py
 frouros/detectors/base.py
 frouros/detectors/concept_drift/__init__.py
 frouros/detectors/concept_drift/base.py
 frouros/detectors/concept_drift/exceptions.py
-frouros/detectors/concept_drift/utils.py
 frouros/detectors/concept_drift/streaming/__init__.py
 frouros/detectors/concept_drift/streaming/base.py
 frouros/detectors/concept_drift/streaming/cusum_based/__init__.py
 frouros/detectors/concept_drift/streaming/cusum_based/base.py
 frouros/detectors/concept_drift/streaming/cusum_based/cusum.py
 frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py
 frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py
-frouros/detectors/concept_drift/streaming/ddm_based/__init__.py
-frouros/detectors/concept_drift/streaming/ddm_based/base.py
-frouros/detectors/concept_drift/streaming/ddm_based/ddm.py
-frouros/detectors/concept_drift/streaming/ddm_based/ecdd.py
-frouros/detectors/concept_drift/streaming/ddm_based/eddm.py
-frouros/detectors/concept_drift/streaming/ddm_based/hddm.py
-frouros/detectors/concept_drift/streaming/ddm_based/rddm.py
-frouros/detectors/concept_drift/streaming/ddm_based/stepd.py
+frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
+frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
+frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
+frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
+frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
+frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
+frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
 frouros/detectors/concept_drift/streaming/window_based/__init__.py
 frouros/detectors/concept_drift/streaming/window_based/adwin.py
 frouros/detectors/concept_drift/streaming/window_based/base.py
 frouros/detectors/concept_drift/streaming/window_based/kswin.py
+frouros/detectors/concept_drift/streaming/window_based/stepd.py
 frouros/detectors/data_drift/__init__.py
 frouros/detectors/data_drift/base.py
 frouros/detectors/data_drift/exceptions.py
 frouros/detectors/data_drift/batch/__init__.py
 frouros/detectors/data_drift/batch/base.py
 frouros/detectors/data_drift/batch/distance_based/__init__.py
 frouros/detectors/data_drift/batch/distance_based/base.py
```

### Comparing `frouros-0.2.7/pyproject.toml` & `frouros-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "frouros"
-version = "0.2.7"
+version = "0.3.0"
 description = "A Python library for drift detection in Machine Learning problems"
 authors = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
 maintainers = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
@@ -28,15 +28,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 requires-python = ">=3.8,<3.12"
 dependencies = [
     "matplotlib>=3.6.0,<3.7",
     "numpy>=1.24.0,<1.25",
-    "requests>=2.28.0,<2.29",
+    "requests>=2.31.0,<2.32",
     "scipy>=1.10.0,<1.11",
     "tqdm>=4.64.0,<4.65",
 ]
 
 [project.optional-dependencies]
 docs = [
     "sphinx>=5.3.0,<5.4",
```

### Comparing `frouros-0.2.7/setup.py` & `frouros-0.3.0/setup.py`

 * *Files identical despite different names*

