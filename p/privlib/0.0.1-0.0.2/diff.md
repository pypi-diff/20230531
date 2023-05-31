# Comparing `tmp/privlib-0.0.1.tar.gz` & `tmp/privlib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "privlib-0.0.1.tar", last modified: Mon May 29 12:15:09 2023, max compression
+gzip compressed data, was "privlib-0.0.2.tar", last modified: Wed May 31 07:50:31 2023, max compression
```

## Comparing `privlib-0.0.1.tar` & `privlib-0.0.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-29 12:15:09.903701 privlib-0.0.1/
--rw-r--r--   0 roberto    (501) staff       (20)     1295 2023-05-27 15:28:26.000000 privlib-0.0.1/LICENSE
--rw-r--r--   0 roberto    (501) staff       (20)       58 2023-05-27 15:28:26.000000 privlib-0.0.1/MANIFEST.in
--rw-r--r--   0 roberto    (501) staff       (20)     1456 2023-05-29 12:15:09.903940 privlib-0.0.1/PKG-INFO
--rw-r--r--   0 roberto    (501) staff       (20)      709 2023-05-27 18:12:15.000000 privlib-0.0.1/README.md
-drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-29 12:15:09.857694 privlib-0.0.1/privlib/
--rw-r--r--   0 roberto    (501) staff       (20)        0 2023-05-29 08:22:58.000000 privlib-0.0.1/privlib/__init__.py
-drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-29 12:15:09.859745 privlib-0.0.1/privlib/anonymization/
--rw-r--r--   0 roberto    (501) staff       (20)        0 2023-05-27 14:24:25.000000 privlib-0.0.1/privlib/anonymization/__init__.py
-drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-29 12:15:09.860086 privlib-0.0.1/privlib/anonymization/src/
--rw-r--r--   0 roberto    (501) staff       (20)        0 2022-12-16 12:26:51.000000 privlib-0.0.1/privlib/anonymization/src/__init__.py
-drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-29 12:15:09.865427 privlib-0.0.1/privlib/anonymization/src/algorithms/
--rw-r--r--   0 roberto    (501) staff       (20)        0 2022-12-16 12:26:51.000000 privlib-0.0.1/privlib/anonymization/src/algorithms/__init__.py
--rw-r--r--   0 roberto    (501) staff       (20)     2497 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/algorithms/algorithm.py
--rw-r--r--   0 roberto    (501) staff       (20)    14426 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/algorithms/anonymization_scheme.py
--rw-r--r--   0 roberto    (501) staff       (20)     5358 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/algorithms/differential_privacy.py
--rw-r--r--   0 roberto    (501) staff       (20)     3003 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/algorithms/k_anonymity.py
--rw-r--r--   0 roberto    (501) staff       (20)     3616 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/algorithms/mdav.py
--rw-r--r--   0 roberto    (501) staff       (20)     2531 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/algorithms/microaggregation.py
--rw-r--r--   0 roberto    (501) staff       (20)     6098 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/algorithms/t_closeness.py
-drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-29 12:15:09.873313 privlib-0.0.1/privlib/anonymization/src/attribute_types/
--rw-r--r--   0 roberto    (501) staff       (20)        0 2022-12-16 12:26:51.000000 privlib-0.0.1/privlib/anonymization/src/attribute_types/__init__.py
--rw-r--r--   0 roberto    (501) staff       (20)     1802 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/attribute_types/attribute_type.py
--rw-r--r--   0 roberto    (501) staff       (20)     8375 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/attribute_types/coordinate.py
--rw-r--r--   0 roberto    (501) staff       (20)     7624 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/attribute_types/date.py
--rw-r--r--   0 roberto    (501) staff       (20)     7913 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/attribute_types/datetime.py
--rw-r--r--   0 roberto    (501) staff       (20)     8130 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/attribute_types/numerical_continuous.py
--rw-r--r--   0 roberto    (501) staff       (20)     7505 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/attribute_types/numerical_discrete.py
--rw-r--r--   0 roberto    (501) staff       (20)     8663 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/attribute_types/plain_categorical.py
--rw-r--r--   0 roberto    (501) staff       (20)    11565 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/attribute_types/semantic_categorical_wordnet.py
--rw-r--r--   0 roberto    (501) staff       (20)     4174 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/attribute_types/value.py
-drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-29 12:15:09.879732 privlib-0.0.1/privlib/anonymization/src/entities/
--rw-r--r--   0 roberto    (501) staff       (20)        0 2022-12-16 12:26:51.000000 privlib-0.0.1/privlib/anonymization/src/entities/__init__.py
--rw-r--r--   0 roberto    (501) staff       (20)     1278 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/entities/attribute.py
--rw-r--r--   0 roberto    (501) staff       (20)     9347 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/entities/dataset.py
--rw-r--r--   0 roberto    (501) staff       (20)     2275 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/entities/dataset_CSV.py
--rw-r--r--   0 roberto    (501) staff       (20)     2159 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/entities/dataset_DataFrame.py
--rw-r--r--   0 roberto    (501) staff       (20)     3356 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/entities/dataset_SPF.py
--rw-r--r--   0 roberto    (501) staff       (20)     1126 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/entities/disclosure_risk_result.py
--rw-r--r--   0 roberto    (501) staff       (20)     3588 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/entities/information_loss_result.py
--rw-r--r--   0 roberto    (501) staff       (20)     5465 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/entities/record.py
-drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-29 12:15:09.882146 privlib-0.0.1/privlib/anonymization/src/utils/
--rw-r--r--   0 roberto    (501) staff       (20)        0 2022-12-16 12:26:51.000000 privlib-0.0.1/privlib/anonymization/src/utils/__init__.py
--rw-r--r--   0 roberto    (501) staff       (20)      463 2022-12-16 12:26:51.000000 privlib-0.0.1/privlib/anonymization/src/utils/constants.py
--rw-r--r--   0 roberto    (501) staff       (20)      298 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/anonymization/src/utils/sensitivity_type.py
--rw-r--r--   0 roberto    (501) staff       (20)     4587 2022-12-16 12:26:51.000000 privlib-0.0.1/privlib/anonymization/src/utils/utils.py
-drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-29 12:15:09.883029 privlib-0.0.1/privlib/antiDiscrimination/
--rw-r--r--   0 roberto    (501) staff       (20)        0 2022-12-16 12:26:51.000000 privlib-0.0.1/privlib/antiDiscrimination/__init__.py
-drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-29 12:15:09.883494 privlib-0.0.1/privlib/antiDiscrimination/src/
--rw-r--r--   0 roberto    (501) staff       (20)       86 2022-12-16 12:26:51.000000 privlib-0.0.1/privlib/antiDiscrimination/src/__init__.py
-drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-29 12:15:09.885890 privlib-0.0.1/privlib/antiDiscrimination/src/algorithms/
--rw-r--r--   0 roberto    (501) staff       (20)        0 2022-12-16 12:26:51.000000 privlib-0.0.1/privlib/antiDiscrimination/src/algorithms/__init__.py
--rw-r--r--   0 roberto    (501) staff       (20)     3510 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/antiDiscrimination/src/algorithms/anonymization_scheme.py
--rw-r--r--   0 roberto    (501) staff       (20)    38038 2023-05-28 22:42:38.000000 privlib-0.0.1/privlib/antiDiscrimination/src/algorithms/anti_discrimination.py
-drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-29 12:15:09.891632 privlib-0.0.1/privlib/antiDiscrimination/src/entities/
--rw-r--r--   0 roberto    (501) staff       (20)        0 2022-12-16 12:26:51.000000 privlib-0.0.1/privlib/antiDiscrimination/src/entities/__init__.py
--rw-r--r--   0 roberto    (501) staff       (20)     1650 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/antiDiscrimination/src/entities/anti_discrimination_metrics.py
--rw-r--r--   0 roberto    (501) staff       (20)     3477 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/antiDiscrimination/src/entities/dataset.py
--rw-r--r--   0 roberto    (501) staff       (20)     2068 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/antiDiscrimination/src/entities/dataset_CSV.py
--rw-r--r--   0 roberto    (501) staff       (20)     1905 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/antiDiscrimination/src/entities/dataset_DataFrame.py
--rw-r--r--   0 roberto    (501) staff       (20)      697 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/antiDiscrimination/src/entities/record.py
-drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-29 12:15:09.895482 privlib-0.0.1/privlib/antiDiscrimination/src/utils/
--rw-r--r--   0 roberto    (501) staff       (20)        0 2022-12-16 12:26:51.000000 privlib-0.0.1/privlib/antiDiscrimination/src/utils/__init__.py
--rw-r--r--   0 roberto    (501) staff       (20)      463 2022-12-16 12:26:51.000000 privlib-0.0.1/privlib/antiDiscrimination/src/utils/constants.py
--rw-r--r--   0 roberto    (501) staff       (20)      298 2023-05-28 22:42:36.000000 privlib-0.0.1/privlib/antiDiscrimination/src/utils/sensitivity_type.py
--rw-r--r--   0 roberto    (501) staff       (20)     4523 2022-12-16 12:26:51.000000 privlib-0.0.1/privlib/antiDiscrimination/src/utils/utils.py
-drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-29 12:15:09.896980 privlib-0.0.1/privlib/discriminationDiscovery/
--rw-r--r--   0 roberto    (501) staff       (20)        0 2023-05-28 22:15:27.000000 privlib-0.0.1/privlib/discriminationDiscovery/__init__.py
--rw-r--r--   0 roberto    (501) staff       (20)    11813 2023-05-28 22:42:37.000000 privlib-0.0.1/privlib/discriminationDiscovery/discrimination_discovery.py
-drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-29 12:15:09.903035 privlib-0.0.1/privlib/riskAssessment/
--rw-r--r--   0 roberto    (501) staff       (20)        0 2023-05-27 16:56:05.000000 privlib-0.0.1/privlib/riskAssessment/__init__.py
--rw-r--r--   0 roberto    (501) staff       (20)    20483 2023-05-28 22:42:37.000000 privlib-0.0.1/privlib/riskAssessment/attacks.py
--rw-r--r--   0 roberto    (501) staff       (20)      816 2023-05-28 22:42:37.000000 privlib-0.0.1/privlib/riskAssessment/constants.py
--rw-r--r--   0 roberto    (501) staff       (20)    22568 2023-05-28 22:42:37.000000 privlib-0.0.1/privlib/riskAssessment/riskevaluators.py
--rw-r--r--   0 roberto    (501) staff       (20)    10209 2023-05-28 22:42:37.000000 privlib-0.0.1/privlib/riskAssessment/sequentialprivacyframe.py
--rw-r--r--   0 roberto    (501) staff       (20)      927 2023-05-28 22:42:37.000000 privlib-0.0.1/privlib/riskAssessment/utils.py
-drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-29 12:15:09.859434 privlib-0.0.1/privlib.egg-info/
--rw-r--r--   0 roberto    (501) staff       (20)     1456 2023-05-29 12:15:09.000000 privlib-0.0.1/privlib.egg-info/PKG-INFO
--rw-r--r--   0 roberto    (501) staff       (20)     3117 2023-05-29 12:15:09.000000 privlib-0.0.1/privlib.egg-info/SOURCES.txt
--rw-r--r--   0 roberto    (501) staff       (20)        1 2023-05-29 12:15:09.000000 privlib-0.0.1/privlib.egg-info/dependency_links.txt
--rw-r--r--   0 roberto    (501) staff       (20)      123 2023-05-29 12:15:09.000000 privlib-0.0.1/privlib.egg-info/requires.txt
--rw-r--r--   0 roberto    (501) staff       (20)        8 2023-05-29 12:15:09.000000 privlib-0.0.1/privlib.egg-info/top_level.txt
--rw-r--r--   0 roberto    (501) staff       (20)      114 2023-05-29 07:04:15.000000 privlib-0.0.1/requirements.txt
--rw-r--r--   0 roberto    (501) staff       (20)       53 2023-05-29 12:15:09.904644 privlib-0.0.1/setup.cfg
--rw-r--r--   0 roberto    (501) staff       (20)     2053 2023-05-29 10:50:13.000000 privlib-0.0.1/setup.py
+drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-31 07:50:31.544282 privlib-0.0.2/
+-rw-r--r--   0 roberto    (501) staff       (20)     1295 2023-05-27 15:28:26.000000 privlib-0.0.2/LICENSE
+-rw-r--r--   0 roberto    (501) staff       (20)       58 2023-05-27 15:28:26.000000 privlib-0.0.2/MANIFEST.in
+-rw-r--r--   0 roberto    (501) staff       (20)     1625 2023-05-31 07:50:31.544411 privlib-0.0.2/PKG-INFO
+-rw-r--r--   0 roberto    (501) staff       (20)      869 2023-05-31 07:47:37.000000 privlib-0.0.2/README.md
+drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-31 07:50:31.507092 privlib-0.0.2/privlib/
+-rw-r--r--   0 roberto    (501) staff       (20)        0 2023-05-29 08:22:58.000000 privlib-0.0.2/privlib/__init__.py
+drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-31 07:50:31.509097 privlib-0.0.2/privlib/anonymization/
+-rw-r--r--   0 roberto    (501) staff       (20)        0 2023-05-27 14:24:25.000000 privlib-0.0.2/privlib/anonymization/__init__.py
+drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-31 07:50:31.509347 privlib-0.0.2/privlib/anonymization/src/
+-rw-r--r--   0 roberto    (501) staff       (20)        0 2022-12-16 12:26:51.000000 privlib-0.0.2/privlib/anonymization/src/__init__.py
+drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-31 07:50:31.514865 privlib-0.0.2/privlib/anonymization/src/algorithms/
+-rw-r--r--   0 roberto    (501) staff       (20)        0 2022-12-16 12:26:51.000000 privlib-0.0.2/privlib/anonymization/src/algorithms/__init__.py
+-rw-r--r--   0 roberto    (501) staff       (20)     2497 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/algorithms/algorithm.py
+-rw-r--r--   0 roberto    (501) staff       (20)    14426 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/algorithms/anonymization_scheme.py
+-rw-r--r--   0 roberto    (501) staff       (20)     5358 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/algorithms/differential_privacy.py
+-rw-r--r--   0 roberto    (501) staff       (20)     3003 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/algorithms/k_anonymity.py
+-rw-r--r--   0 roberto    (501) staff       (20)     3616 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/algorithms/mdav.py
+-rw-r--r--   0 roberto    (501) staff       (20)     2531 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/algorithms/microaggregation.py
+-rw-r--r--   0 roberto    (501) staff       (20)     6098 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/algorithms/t_closeness.py
+drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-31 07:50:31.521742 privlib-0.0.2/privlib/anonymization/src/attribute_types/
+-rw-r--r--   0 roberto    (501) staff       (20)        0 2022-12-16 12:26:51.000000 privlib-0.0.2/privlib/anonymization/src/attribute_types/__init__.py
+-rw-r--r--   0 roberto    (501) staff       (20)     1802 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/attribute_types/attribute_type.py
+-rw-r--r--   0 roberto    (501) staff       (20)     8375 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/attribute_types/coordinate.py
+-rw-r--r--   0 roberto    (501) staff       (20)     7624 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/attribute_types/date.py
+-rw-r--r--   0 roberto    (501) staff       (20)     7913 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/attribute_types/datetime.py
+-rw-r--r--   0 roberto    (501) staff       (20)     8130 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/attribute_types/numerical_continuous.py
+-rw-r--r--   0 roberto    (501) staff       (20)     7505 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/attribute_types/numerical_discrete.py
+-rw-r--r--   0 roberto    (501) staff       (20)     8663 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/attribute_types/plain_categorical.py
+-rw-r--r--   0 roberto    (501) staff       (20)    11565 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/attribute_types/semantic_categorical_wordnet.py
+-rw-r--r--   0 roberto    (501) staff       (20)     4174 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/attribute_types/value.py
+drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-31 07:50:31.526851 privlib-0.0.2/privlib/anonymization/src/entities/
+-rw-r--r--   0 roberto    (501) staff       (20)        0 2022-12-16 12:26:51.000000 privlib-0.0.2/privlib/anonymization/src/entities/__init__.py
+-rw-r--r--   0 roberto    (501) staff       (20)     1278 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/entities/attribute.py
+-rw-r--r--   0 roberto    (501) staff       (20)     9347 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/entities/dataset.py
+-rw-r--r--   0 roberto    (501) staff       (20)     2275 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/entities/dataset_CSV.py
+-rw-r--r--   0 roberto    (501) staff       (20)     2159 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/entities/dataset_DataFrame.py
+-rw-r--r--   0 roberto    (501) staff       (20)     3356 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/entities/dataset_SPF.py
+-rw-r--r--   0 roberto    (501) staff       (20)     1126 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/entities/disclosure_risk_result.py
+-rw-r--r--   0 roberto    (501) staff       (20)     3588 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/entities/information_loss_result.py
+-rw-r--r--   0 roberto    (501) staff       (20)     5465 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/entities/record.py
+drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-31 07:50:31.529044 privlib-0.0.2/privlib/anonymization/src/utils/
+-rw-r--r--   0 roberto    (501) staff       (20)        0 2022-12-16 12:26:51.000000 privlib-0.0.2/privlib/anonymization/src/utils/__init__.py
+-rw-r--r--   0 roberto    (501) staff       (20)      463 2022-12-16 12:26:51.000000 privlib-0.0.2/privlib/anonymization/src/utils/constants.py
+-rw-r--r--   0 roberto    (501) staff       (20)      298 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/anonymization/src/utils/sensitivity_type.py
+-rw-r--r--   0 roberto    (501) staff       (20)     4587 2022-12-16 12:26:51.000000 privlib-0.0.2/privlib/anonymization/src/utils/utils.py
+drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-31 07:50:31.529677 privlib-0.0.2/privlib/antiDiscrimination/
+-rw-r--r--   0 roberto    (501) staff       (20)        0 2022-12-16 12:26:51.000000 privlib-0.0.2/privlib/antiDiscrimination/__init__.py
+drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-31 07:50:31.529938 privlib-0.0.2/privlib/antiDiscrimination/src/
+-rw-r--r--   0 roberto    (501) staff       (20)       86 2022-12-16 12:26:51.000000 privlib-0.0.2/privlib/antiDiscrimination/src/__init__.py
+drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-31 07:50:31.531455 privlib-0.0.2/privlib/antiDiscrimination/src/algorithms/
+-rw-r--r--   0 roberto    (501) staff       (20)        0 2022-12-16 12:26:51.000000 privlib-0.0.2/privlib/antiDiscrimination/src/algorithms/__init__.py
+-rw-r--r--   0 roberto    (501) staff       (20)     3510 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/antiDiscrimination/src/algorithms/anonymization_scheme.py
+-rw-r--r--   0 roberto    (501) staff       (20)    38038 2023-05-28 22:42:38.000000 privlib-0.0.2/privlib/antiDiscrimination/src/algorithms/anti_discrimination.py
+drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-31 07:50:31.535914 privlib-0.0.2/privlib/antiDiscrimination/src/entities/
+-rw-r--r--   0 roberto    (501) staff       (20)        0 2022-12-16 12:26:51.000000 privlib-0.0.2/privlib/antiDiscrimination/src/entities/__init__.py
+-rw-r--r--   0 roberto    (501) staff       (20)     1650 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/antiDiscrimination/src/entities/anti_discrimination_metrics.py
+-rw-r--r--   0 roberto    (501) staff       (20)     3477 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/antiDiscrimination/src/entities/dataset.py
+-rw-r--r--   0 roberto    (501) staff       (20)     2068 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/antiDiscrimination/src/entities/dataset_CSV.py
+-rw-r--r--   0 roberto    (501) staff       (20)     1905 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/antiDiscrimination/src/entities/dataset_DataFrame.py
+-rw-r--r--   0 roberto    (501) staff       (20)      697 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/antiDiscrimination/src/entities/record.py
+drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-31 07:50:31.538092 privlib-0.0.2/privlib/antiDiscrimination/src/utils/
+-rw-r--r--   0 roberto    (501) staff       (20)        0 2022-12-16 12:26:51.000000 privlib-0.0.2/privlib/antiDiscrimination/src/utils/__init__.py
+-rw-r--r--   0 roberto    (501) staff       (20)      463 2022-12-16 12:26:51.000000 privlib-0.0.2/privlib/antiDiscrimination/src/utils/constants.py
+-rw-r--r--   0 roberto    (501) staff       (20)      298 2023-05-28 22:42:36.000000 privlib-0.0.2/privlib/antiDiscrimination/src/utils/sensitivity_type.py
+-rw-r--r--   0 roberto    (501) staff       (20)     4523 2022-12-16 12:26:51.000000 privlib-0.0.2/privlib/antiDiscrimination/src/utils/utils.py
+drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-31 07:50:31.539225 privlib-0.0.2/privlib/discriminationDiscovery/
+-rw-r--r--   0 roberto    (501) staff       (20)        0 2023-05-28 22:15:27.000000 privlib-0.0.2/privlib/discriminationDiscovery/__init__.py
+-rw-r--r--   0 roberto    (501) staff       (20)    11813 2023-05-28 22:42:37.000000 privlib-0.0.2/privlib/discriminationDiscovery/discrimination_discovery.py
+drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-31 07:50:31.543750 privlib-0.0.2/privlib/riskAssessment/
+-rw-r--r--   0 roberto    (501) staff       (20)        0 2023-05-27 16:56:05.000000 privlib-0.0.2/privlib/riskAssessment/__init__.py
+-rw-r--r--   0 roberto    (501) staff       (20)    20483 2023-05-28 22:42:37.000000 privlib-0.0.2/privlib/riskAssessment/attacks.py
+-rw-r--r--   0 roberto    (501) staff       (20)      816 2023-05-28 22:42:37.000000 privlib-0.0.2/privlib/riskAssessment/constants.py
+-rw-r--r--   0 roberto    (501) staff       (20)    22568 2023-05-28 22:42:37.000000 privlib-0.0.2/privlib/riskAssessment/riskevaluators.py
+-rw-r--r--   0 roberto    (501) staff       (20)    10209 2023-05-28 22:42:37.000000 privlib-0.0.2/privlib/riskAssessment/sequentialprivacyframe.py
+-rw-r--r--   0 roberto    (501) staff       (20)      927 2023-05-28 22:42:37.000000 privlib-0.0.2/privlib/riskAssessment/utils.py
+drwxr-xr-x   0 roberto    (501) staff       (20)        0 2023-05-31 07:50:31.508786 privlib-0.0.2/privlib.egg-info/
+-rw-r--r--   0 roberto    (501) staff       (20)     1625 2023-05-31 07:50:31.000000 privlib-0.0.2/privlib.egg-info/PKG-INFO
+-rw-r--r--   0 roberto    (501) staff       (20)     3117 2023-05-31 07:50:31.000000 privlib-0.0.2/privlib.egg-info/SOURCES.txt
+-rw-r--r--   0 roberto    (501) staff       (20)        1 2023-05-31 07:50:31.000000 privlib-0.0.2/privlib.egg-info/dependency_links.txt
+-rw-r--r--   0 roberto    (501) staff       (20)      123 2023-05-31 07:50:31.000000 privlib-0.0.2/privlib.egg-info/requires.txt
+-rw-r--r--   0 roberto    (501) staff       (20)        8 2023-05-31 07:50:31.000000 privlib-0.0.2/privlib.egg-info/top_level.txt
+-rw-r--r--   0 roberto    (501) staff       (20)      114 2023-05-29 07:04:15.000000 privlib-0.0.2/requirements.txt
+-rw-r--r--   0 roberto    (501) staff       (20)       53 2023-05-31 07:50:31.544878 privlib-0.0.2/setup.cfg
+-rw-r--r--   0 roberto    (501) staff       (20)     2083 2023-05-31 07:49:09.000000 privlib-0.0.2/setup.py
```

### Comparing `privlib-0.0.1/LICENSE` & `privlib-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/PKG-INFO` & `privlib-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: privlib
-Version: 0.0.1
+Version: 0.0.2
 Summary: Privacy library of the SoBigData research infrastructure
-Home-page: https://github.com/USERNAME/project
+Home-page: https://github.com/pellungrobe/sbdprivacylib
 Author: Roberto Pellungrini
 Author-email: roberto.pellungrini@sns.it
-License: BSD-Clause-2
+License: BSD-Clause-3
 Keywords: keyword1 keyword2 keyword3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Other
 Classifier: Operating System :: MacOS
@@ -20,15 +20,21 @@
 License-File: LICENSE
 
 # SoBigData Privacy Library
 [![SBD++](https://img.shields.io/badge/Available%20on-SoBigData%2B%2B-green)](https://sobigdata.d4science.org/group/sobigdata-gateway/explore?siteId=20371853)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## License
-This project is licensed under the terms of the BSD-2-Clause license.
+This project is licensed under the terms of the BSD-3-Clause license.
+
+## Documentation
+The full documentation is available here: [Documentation](https://pellungrobe.readthedocs.io/en/latest/)
+
+## Quickinstall
+pip install privlib
 
 ## Acknowledgements
 This repository was developed within the [SoBigData++](https://sobigdata.d4science.org/group/sobigdata-gateway/explore?siteId=20371853) H2020 project training activities (WP4) to support "Social Mining and Big Data resources Integration" (WP8).
 
 ## Contact(s)
 [Roberto Pellungrini](mailto:roberto.pellungrini@sns.it)
```

### Comparing `privlib-0.0.1/README.md` & `privlib-0.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # SoBigData Privacy Library
 [![SBD++](https://img.shields.io/badge/Available%20on-SoBigData%2B%2B-green)](https://sobigdata.d4science.org/group/sobigdata-gateway/explore?siteId=20371853)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## License
-This project is licensed under the terms of the BSD-2-Clause license.
+This project is licensed under the terms of the BSD-3-Clause license.
+
+## Documentation
+The full documentation is available here: [Documentation](https://pellungrobe.readthedocs.io/en/latest/)
+
+## Quickinstall
+pip install privlib
 
 ## Acknowledgements
 This repository was developed within the [SoBigData++](https://sobigdata.d4science.org/group/sobigdata-gateway/explore?siteId=20371853) H2020 project training activities (WP4) to support "Social Mining and Big Data resources Integration" (WP8).
 
 ## Contact(s)
 [Roberto Pellungrini](mailto:roberto.pellungrini@sns.it)
```

### Comparing `privlib-0.0.1/privlib/anonymization/src/algorithms/algorithm.py` & `privlib-0.0.2/privlib/anonymization/src/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/algorithms/anonymization_scheme.py` & `privlib-0.0.2/privlib/anonymization/src/algorithms/anonymization_scheme.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/algorithms/differential_privacy.py` & `privlib-0.0.2/privlib/anonymization/src/algorithms/differential_privacy.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/algorithms/k_anonymity.py` & `privlib-0.0.2/privlib/anonymization/src/algorithms/k_anonymity.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/algorithms/mdav.py` & `privlib-0.0.2/privlib/anonymization/src/algorithms/mdav.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/algorithms/microaggregation.py` & `privlib-0.0.2/privlib/anonymization/src/algorithms/microaggregation.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/algorithms/t_closeness.py` & `privlib-0.0.2/privlib/anonymization/src/algorithms/t_closeness.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/attribute_types/attribute_type.py` & `privlib-0.0.2/privlib/anonymization/src/attribute_types/attribute_type.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/attribute_types/coordinate.py` & `privlib-0.0.2/privlib/anonymization/src/attribute_types/coordinate.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/attribute_types/date.py` & `privlib-0.0.2/privlib/anonymization/src/attribute_types/date.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/attribute_types/datetime.py` & `privlib-0.0.2/privlib/anonymization/src/attribute_types/datetime.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/attribute_types/numerical_continuous.py` & `privlib-0.0.2/privlib/anonymization/src/attribute_types/numerical_continuous.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/attribute_types/numerical_discrete.py` & `privlib-0.0.2/privlib/anonymization/src/attribute_types/numerical_discrete.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/attribute_types/plain_categorical.py` & `privlib-0.0.2/privlib/anonymization/src/attribute_types/plain_categorical.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/attribute_types/semantic_categorical_wordnet.py` & `privlib-0.0.2/privlib/anonymization/src/attribute_types/semantic_categorical_wordnet.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/attribute_types/value.py` & `privlib-0.0.2/privlib/anonymization/src/attribute_types/value.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/entities/attribute.py` & `privlib-0.0.2/privlib/anonymization/src/entities/attribute.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/entities/dataset.py` & `privlib-0.0.2/privlib/anonymization/src/entities/dataset.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/entities/dataset_CSV.py` & `privlib-0.0.2/privlib/anonymization/src/entities/dataset_CSV.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/entities/dataset_DataFrame.py` & `privlib-0.0.2/privlib/anonymization/src/entities/dataset_DataFrame.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/entities/dataset_SPF.py` & `privlib-0.0.2/privlib/anonymization/src/entities/dataset_SPF.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/entities/disclosure_risk_result.py` & `privlib-0.0.2/privlib/anonymization/src/entities/disclosure_risk_result.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/entities/information_loss_result.py` & `privlib-0.0.2/privlib/anonymization/src/entities/information_loss_result.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/entities/record.py` & `privlib-0.0.2/privlib/anonymization/src/entities/record.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/anonymization/src/utils/utils.py` & `privlib-0.0.2/privlib/anonymization/src/utils/utils.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/antiDiscrimination/src/algorithms/anonymization_scheme.py` & `privlib-0.0.2/privlib/antiDiscrimination/src/algorithms/anonymization_scheme.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/antiDiscrimination/src/algorithms/anti_discrimination.py` & `privlib-0.0.2/privlib/antiDiscrimination/src/algorithms/anti_discrimination.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/antiDiscrimination/src/entities/anti_discrimination_metrics.py` & `privlib-0.0.2/privlib/antiDiscrimination/src/entities/anti_discrimination_metrics.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/antiDiscrimination/src/entities/dataset.py` & `privlib-0.0.2/privlib/antiDiscrimination/src/entities/dataset.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/antiDiscrimination/src/entities/dataset_CSV.py` & `privlib-0.0.2/privlib/antiDiscrimination/src/entities/dataset_CSV.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/antiDiscrimination/src/entities/dataset_DataFrame.py` & `privlib-0.0.2/privlib/antiDiscrimination/src/entities/dataset_DataFrame.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/antiDiscrimination/src/entities/record.py` & `privlib-0.0.2/privlib/antiDiscrimination/src/entities/record.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/antiDiscrimination/src/utils/utils.py` & `privlib-0.0.2/privlib/antiDiscrimination/src/utils/utils.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/discriminationDiscovery/discrimination_discovery.py` & `privlib-0.0.2/privlib/discriminationDiscovery/discrimination_discovery.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/riskAssessment/attacks.py` & `privlib-0.0.2/privlib/riskAssessment/attacks.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/riskAssessment/constants.py` & `privlib-0.0.2/privlib/riskAssessment/constants.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/riskAssessment/riskevaluators.py` & `privlib-0.0.2/privlib/riskAssessment/riskevaluators.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/riskAssessment/sequentialprivacyframe.py` & `privlib-0.0.2/privlib/riskAssessment/sequentialprivacyframe.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib/riskAssessment/utils.py` & `privlib-0.0.2/privlib/riskAssessment/utils.py`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/privlib.egg-info/PKG-INFO` & `privlib-0.0.2/privlib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: privlib
-Version: 0.0.1
+Version: 0.0.2
 Summary: Privacy library of the SoBigData research infrastructure
-Home-page: https://github.com/USERNAME/project
+Home-page: https://github.com/pellungrobe/sbdprivacylib
 Author: Roberto Pellungrini
 Author-email: roberto.pellungrini@sns.it
-License: BSD-Clause-2
+License: BSD-Clause-3
 Keywords: keyword1 keyword2 keyword3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Other
 Classifier: Operating System :: MacOS
@@ -20,15 +20,21 @@
 License-File: LICENSE
 
 # SoBigData Privacy Library
 [![SBD++](https://img.shields.io/badge/Available%20on-SoBigData%2B%2B-green)](https://sobigdata.d4science.org/group/sobigdata-gateway/explore?siteId=20371853)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## License
-This project is licensed under the terms of the BSD-2-Clause license.
+This project is licensed under the terms of the BSD-3-Clause license.
+
+## Documentation
+The full documentation is available here: [Documentation](https://pellungrobe.readthedocs.io/en/latest/)
+
+## Quickinstall
+pip install privlib
 
 ## Acknowledgements
 This repository was developed within the [SoBigData++](https://sobigdata.d4science.org/group/sobigdata-gateway/explore?siteId=20371853) H2020 project training activities (WP4) to support "Social Mining and Big Data resources Integration" (WP8).
 
 ## Contact(s)
 [Roberto Pellungrini](mailto:roberto.pellungrini@sns.it)
```

### Comparing `privlib-0.0.1/privlib.egg-info/SOURCES.txt` & `privlib-0.0.2/privlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `privlib-0.0.1/setup.py` & `privlib-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 
 with open(path.join(here, "requirements.txt"), encoding="utf-8") as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name="privlib",
-    version="0.0.1",
-    license="BSD-Clause-2",
+    version="0.0.2",
+    license="BSD-Clause-3",
     description="Privacy library of the SoBigData research infrastructure",
-    url="https://github.com/USERNAME/project",
+    url="https://github.com/pellungrobe/sbdprivacylib",
     author="Roberto Pellungrini",
     author_email="roberto.pellungrini@sns.it",
     classifiers=[
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
@@ -55,10 +55,11 @@
             "tests.*",
             "*.test.*",
             "*.tests.*",
             "test.*",
             "test",
             "privlib.test",
             "privlib.test.*",
+            "dist.*"
         ]
     ),
 )
```

