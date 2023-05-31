# Comparing `tmp/tensorflow_similarity-0.16.9.tar.gz` & `tmp/tensorflow_similarity-0.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorflow_similarity-0.16.9.tar", last modified: Fri Dec  2 02:22:55 2022, max compression
+gzip compressed data, was "tensorflow_similarity-0.17.1.tar", last modified: Wed May 31 05:10:51 2023, max compression
```

## Comparing `tensorflow_similarity-0.16.9.tar` & `tensorflow_similarity-0.17.1.tar`

### file list

```diff
@@ -1,170 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.612414 tensorflow_similarity-0.16.9/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11426 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8888 2022-12-02 02:22:55.612414 tensorflow_similarity-0.16.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-02 02:22:55.612414 tensorflow_similarity-0.16.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.604414 tensorflow_similarity-0.16.9/tensorflow_similarity/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/algebra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.604414 tensorflow_similarity-0.16.9/tensorflow_similarity/api/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.604414 tensorflow_similarity-0.16.9/tensorflow_similarity/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/architectures/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/architectures/resnet18.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/architectures/resnet50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/architectures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.604414 tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.604414 tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/augmentation_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/augmentation_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/augmentation_utils/blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/augmentation_utils/color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8558 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/augmentation_utils/cropping.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/augmentation_utils/flip.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/augmentation_utils/random_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/augmentation_utils/solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/barlow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/simclr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13518 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.604414 tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/binary_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/classification_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/f1_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/false_positive_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/negative_predictive_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/recall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11612 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/distances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.604414 tensorflow_similarity-0.16.9/tensorflow_similarity/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/evaluators/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16200 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/evaluators/memory_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    30064 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.608414 tensorflow_similarity-0.16.9/tensorflow_similarity/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/losses/barlow.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/losses/circle_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/losses/metric_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9338 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/losses/multisim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/losses/pn_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/losses/simclr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/losses/simsiam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/losses/softnn_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/losses/triplet_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/losses/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/losses/vicreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/losses/xbm_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.608414 tensorflow_similarity-0.16.9/tensorflow_similarity/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/matchers/classification_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/matchers/match_majority_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/matchers/match_nearest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/matchers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.608414 tensorflow_similarity-0.16.9/tensorflow_similarity/models/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40548 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/models/contrastive_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31328 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/models/similarity_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.608414 tensorflow_similarity-0.16.9/tensorflow_similarity/retrieval_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/retrieval_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/retrieval_metrics/bndcg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/retrieval_metrics/map_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/retrieval_metrics/precision_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/retrieval_metrics/recall_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/retrieval_metrics/retrieval_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/retrieval_metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.608414 tensorflow_similarity-0.16.9/tensorflow_similarity/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14019 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/samplers/memory_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/samplers/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/samplers/tfdataset_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/samplers/tfrecords_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/samplers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/schedules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.608414 tensorflow_similarity-0.16.9/tensorflow_similarity/search/
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/search/nmslib_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/search/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.608414 tensorflow_similarity-0.16.9/tensorflow_similarity/stores/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/stores/memory_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/stores/store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.608414 tensorflow_similarity-0.16.9/tensorflow_similarity/training_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/training_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/training_metrics/distance_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/training_metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.608414 tensorflow_similarity-0.16.9/tensorflow_similarity/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/visualization/confusion_matrix_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/visualization/neighbors_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/visualization/projector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tensorflow_similarity/visualization/vizualize_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.604414 tensorflow_similarity-0.16.9/tensorflow_similarity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8888 2022-12-02 02:22:55.000000 tensorflow_similarity-0.16.9/tensorflow_similarity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2022-12-02 02:22:55.000000 tensorflow_similarity-0.16.9/tensorflow_similarity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-02 02:22:55.000000 tensorflow_similarity-0.16.9/tensorflow_similarity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      399 2022-12-02 02:22:55.000000 tensorflow_similarity-0.16.9/tensorflow_similarity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-02 02:22:55.000000 tensorflow_similarity-0.16.9/tensorflow_similarity.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.612414 tensorflow_similarity-0.16.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.612414 tensorflow_similarity-0.16.9/tests/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/architectures/test_efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/architectures/test_resnet18.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/architectures/test_resnet50.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.612414 tensorflow_similarity-0.16.9/tests/classification_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/classification_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/classification_metrics/test_classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.612414 tensorflow_similarity-0.16.9/tests/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/evaluators/test_memory_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.612414 tensorflow_similarity-0.16.9/tests/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/matchers/test_classification_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/matchers/test_majority_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/matchers/test_match_nearest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.612414 tensorflow_similarity-0.16.9/tests/retrieval_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/retrieval_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/retrieval_metrics/test_bndcg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/retrieval_metrics/test_map_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/retrieval_metrics/test_precision_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/retrieval_metrics/test_recall_at_k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/retrieval_metrics/test_retrieval_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.612414 tensorflow_similarity-0.16.9/tests/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/samplers/test_memory_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/samplers/test_tfdataset_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/samplers/test_tfrecord_samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.612414 tensorflow_similarity-0.16.9/tests/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/search/test_nmslib_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.612414 tensorflow_similarity-0.16.9/tests/stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/stores/test_memory_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/test_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)    10981 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/test_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/test_indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/test_schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.612414 tensorflow_similarity-0.16.9/tests/training_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/training_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/training_metrics/test_distance_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 02:22:55.612414 tensorflow_similarity-0.16.9/tests/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/visualization/test_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2022-12-02 02:21:24.000000 tensorflow_similarity-0.16.9/tests/visualization/test_neighbors_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.480757 tensorflow_similarity-0.17.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11426 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-05-31 05:10:51.480757 tensorflow_similarity-0.17.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 05:10:51.480757 tensorflow_similarity-0.17.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.448756 tensorflow_similarity-0.17.1/tensorflow_similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/algebra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.448756 tensorflow_similarity-0.17.1/tensorflow_similarity/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.452757 tensorflow_similarity-0.17.1/tensorflow_similarity/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/architectures/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/architectures/resnet18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/architectures/resnet50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/architectures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.452757 tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.452757 tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/augmentation_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/augmentation_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/augmentation_utils/blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/augmentation_utils/color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/augmentation_utils/cropping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/augmentation_utils/flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/augmentation_utils/random_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/augmentation_utils/solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/barlow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/simclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12238 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.456756 tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/binary_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/classification_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/f1_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/false_positive_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/negative_predictive_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/recall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12881 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/distances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.456756 tensorflow_similarity-0.17.1/tensorflow_similarity/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/evaluators/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16195 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/evaluators/memory_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30633 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.460757 tensorflow_similarity-0.17.1/tensorflow_similarity/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/losses/barlow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/losses/circle_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/losses/metric_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/losses/multinegrank_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/losses/multisim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/losses/pn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/losses/simclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/losses/simsiam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/losses/softnn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/losses/triplet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/losses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/losses/vicreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/losses/xbm_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.460757 tensorflow_similarity-0.17.1/tensorflow_similarity/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/matchers/classification_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/matchers/match_majority_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/matchers/match_nearest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/matchers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.460757 tensorflow_similarity-0.17.1/tensorflow_similarity/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39080 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/models/contrastive_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31807 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/models/similarity_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.464757 tensorflow_similarity-0.17.1/tensorflow_similarity/retrieval_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/retrieval_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/retrieval_metrics/bndcg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/retrieval_metrics/map_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/retrieval_metrics/precision_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/retrieval_metrics/recall_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/retrieval_metrics/retrieval_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/retrieval_metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.464757 tensorflow_similarity-0.17.1/tensorflow_similarity/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/samplers/file_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/samplers/memory_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/samplers/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/samplers/tfdata_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/samplers/tfdataset_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/samplers/tfrecords_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/samplers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/schedules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.464757 tensorflow_similarity-0.17.1/tensorflow_similarity/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/search/nmslib_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/search/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.468757 tensorflow_similarity-0.17.1/tensorflow_similarity/stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/stores/memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/stores/store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.468757 tensorflow_similarity-0.17.1/tensorflow_similarity/training_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/training_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/training_metrics/distance_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/training_metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.468757 tensorflow_similarity-0.17.1/tensorflow_similarity/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/visualization/confusion_matrix_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/visualization/neighbors_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/visualization/projector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tensorflow_similarity/visualization/vizualize_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.448756 tensorflow_similarity-0.17.1/tensorflow_similarity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-05-31 05:10:51.000000 tensorflow_similarity-0.17.1/tensorflow_similarity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-05-31 05:10:51.000000 tensorflow_similarity-0.17.1/tensorflow_similarity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 05:10:51.000000 tensorflow_similarity-0.17.1/tensorflow_similarity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-31 05:10:51.000000 tensorflow_similarity-0.17.1/tensorflow_similarity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 05:10:51.000000 tensorflow_similarity-0.17.1/tensorflow_similarity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.472757 tensorflow_similarity-0.17.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.472757 tensorflow_similarity-0.17.1/tests/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/architectures/test_efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/architectures/test_resnet18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/architectures/test_resnet50.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.472757 tensorflow_similarity-0.17.1/tests/classification_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/classification_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/classification_metrics/test_classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.472757 tensorflow_similarity-0.17.1/tests/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/evaluators/test_memory_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.472757 tensorflow_similarity-0.17.1/tests/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/losses/test_pn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/losses/test_softnn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/losses/test_triplet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/losses/test_xbm_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.476757 tensorflow_similarity-0.17.1/tests/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/matchers/test_classification_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/matchers/test_majority_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/matchers/test_match_nearest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.476757 tensorflow_similarity-0.17.1/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/models/test_contrastive_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/models/test_similarity_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.476757 tensorflow_similarity-0.17.1/tests/retrieval_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/retrieval_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/retrieval_metrics/test_bndcg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/retrieval_metrics/test_map_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/retrieval_metrics/test_precision_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/retrieval_metrics/test_recall_at_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/retrieval_metrics/test_retrieval_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.476757 tensorflow_similarity-0.17.1/tests/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/samplers/test_file_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/samplers/test_memory_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/samplers/test_tfdata_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/samplers/test_tfdataset_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/samplers/test_tfrecord_samplers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.476757 tensorflow_similarity-0.17.1/tests/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/search/test_nmslib_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.480757 tensorflow_similarity-0.17.1/tests/stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/stores/test_memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/test_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/test_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/test_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/test_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.480757 tensorflow_similarity-0.17.1/tests/training_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/training_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/training_metrics/test_distance_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 05:10:51.480757 tensorflow_similarity-0.17.1/tests/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/visualization/test_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-31 05:09:01.000000 tensorflow_similarity-0.17.1/tests/visualization/test_neighbors_viz.py
```

### Comparing `tensorflow_similarity-0.16.9/LICENSE` & `tensorflow_similarity-0.17.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/PKG-INFO` & `tensorflow_similarity-0.17.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow_similarity
-Version: 0.16.9
+Version: 0.17.1
 Summary: Metric Learning for Humans
 Home-page: https://github.com/tensorflow/similarity
 Author: Tensorflow Similarity authors
 Author-email: tf-similarity@google.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,27 +34,21 @@
 
 1. **Self-supervised models**: Used to learn general data representations on unlabeled data to boost the accuracy of downstream tasks where you have few labels. For example, you can pre-train a model on a large number of unlabled images using one of the supported contrastive methods supported by TensorFlow Similarity, and then fine-tune it on a small labeled dataset to achieve higher accuracy. To get started training your own self-supervised model see this [notebook](examples/unsupervised_hello_world.ipynb).
 
 2. **Similarity models**: Output embeddings that allow you to find and cluster similar examples such as images representing the same object within a large corpus of examples. For instance, as visible above, you can train a similarity model to find and cluster similar looking, unseen cat and dog images from the [Oxford IIIT Pet Dataset](https://www.tensorflow.org/datasets/catalog/oxford_iiit_pet) while only training on a few of the dataset classes. To get started training your own similarity model see this [notebook](examples/supervised/visualization.ipynb).
 
 ## What's new
 
-- [May 2022]: 0.16 major optimization release
-    * Cross-batch memory (XBM) loss added thank to @chjort
-    * Many self-supervised related improvement thanks to @dewball345
-    * Major layers and callback refactoring to make them faster and more flexible. E.g `EvalCallback()` now support splited validation.
-     For full changes see [the changelog](./releases.md)
-
-- [Jan 2022]: 0.15 self-supervised release
-    * Added support for self-supervised contrastive learning. Including SimCLR, SimSiam, and Barlow Twins. Checkout the in-depth [hello world notebook](examples/unsupervised_hello_world.ipynb) to get started.
-    * Soft Nearest Neighbor Loss added thanks to [Abhishar Sinha](https://github.com/abhisharsinha)
-    * Added GenerlizedMeanPooling2D support that improves similarity matching accuracy over GlobalMeanPooling2D.
-    * Numerous speed optimizations and general bug fixes.
+- [Mar 2032]: 0.17 more losses and metric and massive refactoring 
+   * Added VicReg Loss to contrastive losses.
+   * Added metrics used in retrieval papers such as Precision@K
+   * Native support for distributed training e.g SimClr now works correctly with distributed training.
+   * Multi-modal embedding initial support (CLIP)
 
-For previous changes and more details - see [the changelog](./releases.md)
+For more details and previous releases informaiton - see [the changelog](./releases.md)
 
 ## Getting Started
 
 ### Installation
 
 Use pip to install the library.
```

### Comparing `tensorflow_similarity-0.16.9/README.md` & `tensorflow_similarity-0.17.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,27 +12,21 @@
 
 1. **Self-supervised models**: Used to learn general data representations on unlabeled data to boost the accuracy of downstream tasks where you have few labels. For example, you can pre-train a model on a large number of unlabled images using one of the supported contrastive methods supported by TensorFlow Similarity, and then fine-tune it on a small labeled dataset to achieve higher accuracy. To get started training your own self-supervised model see this [notebook](examples/unsupervised_hello_world.ipynb).
 
 2. **Similarity models**: Output embeddings that allow you to find and cluster similar examples such as images representing the same object within a large corpus of examples. For instance, as visible above, you can train a similarity model to find and cluster similar looking, unseen cat and dog images from the [Oxford IIIT Pet Dataset](https://www.tensorflow.org/datasets/catalog/oxford_iiit_pet) while only training on a few of the dataset classes. To get started training your own similarity model see this [notebook](examples/supervised/visualization.ipynb).
 
 ## What's new
 
-- [May 2022]: 0.16 major optimization release
-    * Cross-batch memory (XBM) loss added thank to @chjort
-    * Many self-supervised related improvement thanks to @dewball345
-    * Major layers and callback refactoring to make them faster and more flexible. E.g `EvalCallback()` now support splited validation.
-     For full changes see [the changelog](./releases.md)
-
-- [Jan 2022]: 0.15 self-supervised release
-    * Added support for self-supervised contrastive learning. Including SimCLR, SimSiam, and Barlow Twins. Checkout the in-depth [hello world notebook](examples/unsupervised_hello_world.ipynb) to get started.
-    * Soft Nearest Neighbor Loss added thanks to [Abhishar Sinha](https://github.com/abhisharsinha)
-    * Added GenerlizedMeanPooling2D support that improves similarity matching accuracy over GlobalMeanPooling2D.
-    * Numerous speed optimizations and general bug fixes.
+- [Mar 2032]: 0.17 more losses and metric and massive refactoring 
+   * Added VicReg Loss to contrastive losses.
+   * Added metrics used in retrieval papers such as Precision@K
+   * Native support for distributed training e.g SimClr now works correctly with distributed training.
+   * Multi-modal embedding initial support (CLIP)
 
-For previous changes and more details - see [the changelog](./releases.md)
+For more details and previous releases informaiton - see [the changelog](./releases.md)
 
 ## Getting Started
 
 ### Installation
 
 Use pip to install the library.
```

### Comparing `tensorflow_similarity-0.16.9/setup.py` & `tensorflow_similarity-0.17.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -83,17 +83,17 @@
             "pytype",
             "setuptools",
             "types-termcolor",
             "twine",
             "types-tabulate",
             "wheel",
         ],
-        "tensorflow": ["tensorflow>=2.4,<=2.9"],
-        "tensorflow-gpu": ["tensorflow-gpu>=2.4,<=2.9"],
-        "tensorflow-cpu": ["tensorflow-cpu>=2.4,<=2.9"],
+        "tensorflow": ["tensorflow>=2.7,<=2.11"],
+        "tensorflow-gpu": ["tensorflow-gpu>=2.7,<=2.11"],
+        "tensorflow-cpu": ["tensorflow-cpu>=2.7,<=2.11"],
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "License :: OSI Approved :: Apache Software License",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/__init__.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.16.9"
+__version__ = "0.17.1"
 
 
 from . import algebra  # noqa
 from . import architectures  # noqa
 from . import augmenters  # noqa
 from . import callbacks  # noqa
 from . import classification_metrics  # noqa
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/algebra.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/algebra.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,74 +7,75 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 "Set of useful algebraic functions used through the package"
-from typing import Tuple
+from __future__ import annotations
 
 import tensorflow as tf
 
 from .types import BoolTensor, FloatTensor, IntTensor
 
 
-def masked_max(distances: FloatTensor, mask: BoolTensor, dim: int = 1) -> Tuple[FloatTensor, FloatTensor]:
+def masked_max(distances: FloatTensor, mask: BoolTensor, dim: int = 1) -> tuple[FloatTensor, FloatTensor]:
     """Computes the maximum values over masked pairwise distances.
 
     We need to use this formula to make sure all values are >=0.
 
     Args:
       distances: 2-D float `Tensor` of [n, n] pairwise distances
       mask: 2-D Boolean `Tensor` of [n, n] valid distance size.
       dim: The dimension over which to compute the maximum. Defaults to 1.
 
     Returns:
       A Tuple of Tensors containing the maximum distance value and the arg_max
       for each example.
     """
     # Convert to dbl to avoid precision error in offset
+    distance_dtype = distances.dtype
     distances = tf.cast(distances, dtype=tf.float64)
     mask = tf.cast(mask, dtype=tf.float64)
 
     axis_min = tf.math.reduce_min(distances, dim, keepdims=True) - 1e-6
     masked_max = tf.math.multiply(distances - axis_min, mask)
     arg_max = tf.math.argmax(masked_max, dim)
     masked_max = tf.math.reduce_max(masked_max, dim, keepdims=True) + axis_min
-    return tf.cast(masked_max, dtype=tf.float32), arg_max
+    return tf.cast(masked_max, dtype=distance_dtype), arg_max
 
 
-def masked_min(distances: FloatTensor, mask: BoolTensor, dim: int = 1) -> Tuple[FloatTensor, FloatTensor]:
+def masked_min(distances: FloatTensor, mask: BoolTensor, dim: int = 1) -> tuple[FloatTensor, FloatTensor]:
     """Computes the minimal values over masked pairwise distances.
 
     Args:
       distances: 2-D float `Tensor` of [n, n] pairwise distances
       mask: 2-D Boolean `Tensor` of [n, n] valid distance size.
       dim: The dimension over which to compute the minimum. Defaults to 1.
 
     Returns:
       A Tuple of Tensors containing the minimal distance value and the arg_min
       for each example.
     """
     # Convert to dbl to avoid precision error in offset
+    distance_dtype = distances.dtype
     distances = tf.cast(distances, dtype=tf.float64)
     mask = tf.cast(mask, dtype=tf.float64)
 
     axis_max = tf.math.reduce_max(distances, dim, keepdims=True) + 1e-6
     masked_min = tf.math.multiply(distances - axis_max, mask)
     arg_min = tf.math.argmin(masked_min, dim)
     masked_min = tf.math.reduce_min(masked_min, dim, keepdims=True) + axis_max
-    return tf.cast(masked_min, dtype=tf.float32), arg_min
+    return tf.cast(masked_min, dtype=distance_dtype), arg_min
 
 
 def build_masks(
     query_labels: IntTensor, key_labels: IntTensor, batch_size: int, remove_diagonal: bool = True
-) -> Tuple[BoolTensor, BoolTensor]:
+) -> tuple[BoolTensor, BoolTensor]:
     """Build masks that allows to select only the positive or negatives
     embeddings.
     Args:
         query_labels: 1D int `Tensor` that contains the query class ids.
         key_labels: 1D int `Tensor` that contains the key class ids.
         batch_size: size of the batch.
         remove_diagonal: Bool. If True, will set diagonal to False in positive pair mask
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/api/__init__.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/architectures/__init__.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/architectures/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/architectures/efficientnet.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/architectures/efficientnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 "EfficientNet backbone for similarity learning"
+from __future__ import annotations
+
 import re
-from typing import Tuple
 
 import tensorflow as tf
 from tensorflow.keras import layers
 from tensorflow.keras.applications import efficientnet
 
 from tensorflow_similarity.layers import GeneralizedMeanPooling2D, MetricEmbedding
 from tensorflow_similarity.models import SimilarityModel
@@ -45,23 +45,23 @@
     "B5": efficientnet.EfficientNetB5,
     "B6": efficientnet.EfficientNetB6,
     "B7": efficientnet.EfficientNetB7,
 }
 
 
 def EfficientNetSim(
-    input_shape: Tuple[int, int, int],
+    input_shape: tuple[int, int, int],
     embedding_size: int = 128,
     variant: str = "B0",
     weights: str = "imagenet",
     trainable: str = "frozen",
     l2_norm: bool = True,
     include_top: bool = True,
     pooling: str = "gem",
-    gem_p=3.0,
+    gem_p: float = 3.0,
 ) -> SimilarityModel:
     """Build an EfficientNet Model backbone for similarity learning
 
     [EfficientNet: Rethinking Model Scaling for Convolutional Neural Networks](https://arxiv.org/abs/1905.11946)
 
     Args:
         input_shape: Size of the input image. Must match size of EfficientNet version you use.
@@ -141,15 +141,15 @@
             outputs = layers.Dense(embedding_size)(x)
     else:
         outputs = x
 
     return SimilarityModel(inputs, outputs)
 
 
-def build_effnet(variant: str, weights: str = None, trainable: str = "full") -> tf.keras.Model:
+def build_effnet(variant: str, weights: str | None = None, trainable: str = "full") -> tf.keras.Model:
     """Build the requested efficient net.
 
     Args:
 
         variant: Which Variant of the EfficientNet to use.
 
         weights: Use pre-trained weights - the only available currently being
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/architectures/resnet18.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/architectures/resnet18.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,33 +7,32 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-"ResNet50 backbone for similarity learning"
-from typing import Tuple
+"ResNet18 backbone for similarity learning"
+from __future__ import annotations
 
 import tensorflow as tf
 from tensorflow.keras import layers
 
 from tensorflow_similarity.layers import GeneralizedMeanPooling2D, MetricEmbedding
 from tensorflow_similarity.models import SimilarityModel
 
 
 # Create an image augmentation pipeline.
 def ResNet18Sim(
-    input_shape: Tuple[int, int, int],
+    input_shape: tuple[int, int, int],
     embedding_size: int = 128,
     l2_norm: bool = True,
     include_top: bool = True,
     pooling: str = "gem",
-    gem_p=3.0,
+    gem_p: float = 3.0,
 ) -> SimilarityModel:
     """Build an ResNet18 Model backbone for similarity learning
 
     Architecture from [Deep Residual Learning for Image Recognition](https://arxiv.org/abs/1512.03385)
 
     Args:
         input_shape: Expected to be betweeen 32 and 224 and in the (H, W, C)
@@ -87,15 +86,15 @@
             outputs = layers.Dense(embedding_size)(x)
     else:
         outputs = x
 
     return SimilarityModel(inputs, outputs, name="resnet18sim")
 
 
-def build_resnet(input_shape: Tuple[int, int, int]) -> layers.Layer:
+def build_resnet(input_shape: tuple[int, int, int]) -> layers.Layer:
     """Build the requested ResNet.
 
     Args:
         x: The input layer to the ResNet.
 
         input_shape: Expected to be betweeen 32 and 224 and in the (H, W, C)
         data_format.
@@ -123,67 +122,67 @@
 
     return model
 
 
 def block0(
     x,
     filters,
-    kernel_size=3,
-    stride=1,
-    conv_shortcut=True,
-    name=None,
+    kernel_size: int = 3,
+    stride: int = 1,
+    conv_shortcut: bool = True,
+    name: str = "",
 ):
     if conv_shortcut:
         shortcut = tf.keras.layers.Conv2D(
             filters,
             1,
             strides=stride,
             use_bias=False,
             kernel_initializer=tf.keras.initializers.LecunUniform(),
-            name=name + "_0_conv",
+            name=f"{name}_0_conv",
         )(x)
-        shortcut = tf.keras.layers.experimental.SyncBatchNormalization(epsilon=1.001e-5, name=name + "_0_bn")(shortcut)
+        shortcut = tf.keras.layers.experimental.SyncBatchNormalization(epsilon=1.001e-5, name=f"{name}_0_bn")(shortcut)
     else:
         shortcut = x
 
     x = tf.keras.layers.Conv2D(
         filters,
         kernel_size,
         strides=stride,
         padding="SAME",
         use_bias=False,
         kernel_initializer=tf.keras.initializers.LecunUniform(),
-        name=name + "_1_conv",
+        name=f"{name}_1_conv",
     )(x)
-    x = tf.keras.layers.experimental.SyncBatchNormalization(epsilon=1.001e-5, name=name + "_1_bn")(x)
-    x = tf.keras.layers.Activation("relu", name=name + "_1_relu")(x)
+    x = tf.keras.layers.experimental.SyncBatchNormalization(epsilon=1.001e-5, name=f"{name}_1_bn")(x)
+    x = tf.keras.layers.Activation("relu", name=f"{name}_1_relu")(x)
 
     x = tf.keras.layers.Conv2D(
         filters,
         kernel_size,
         padding="SAME",
         use_bias=False,
         kernel_initializer=tf.keras.initializers.LecunUniform(),
-        name=name + "_2_conv",
+        name=f"{name}_2_conv",
     )(x)
-    x = tf.keras.layers.experimental.SyncBatchNormalization(epsilon=1.001e-5, name=name + "_2_bn")(x)
+    x = tf.keras.layers.experimental.SyncBatchNormalization(epsilon=1.001e-5, name=f"{name}_2_bn")(x)
 
-    x = tf.keras.layers.Add(name=name + "_add")([shortcut, x])
-    x = tf.keras.layers.Activation("relu", name=name + "_out")(x)
+    x = tf.keras.layers.Add(name=f"{name}_add")([shortcut, x])
+    x = tf.keras.layers.Activation("relu", name=f"{name}_out")(x)
     return x
 
 
-def stack0(x, filters, blocks, stride1=2, name=None):
-    x = block0(x, filters, stride=stride1, name=name + "_block1")
+def stack0(x, filters, blocks, stride1: int = 2, name: str = ""):
+    x = block0(x, filters, stride=stride1, name=f"{name}_block1")
     for i in range(2, blocks + 1):
         x = block0(
             x,
             filters,
             conv_shortcut=False,
-            name=name + "_block" + str(i),
+            name=f"{name}_block" + str(i),
         )
     return x
 
 
 def stack_fn(x):
     x = stack0(x, 64, 2, stride1=1, name="conv2")
     x = stack0(x, 128, 2, name="conv3")
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/architectures/resnet50.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/architectures/resnet50.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,39 +7,39 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 "ResNet50 backbone for similarity learning"
+from __future__ import annotations
+
 import re
-from typing import Tuple
 
 import tensorflow as tf
 from tensorflow.keras import layers
 from tensorflow.keras.applications import resnet50
 
 from tensorflow_similarity.layers import GeneralizedMeanPooling2D, MetricEmbedding
 from tensorflow_similarity.models import SimilarityModel
 
 from .utils import convert_sync_batchnorm
 
 
 # Create an image augmentation pipeline.
 def ResNet50Sim(
-    input_shape: Tuple[int],
+    input_shape: tuple[int, int, int],
     embedding_size: int = 128,
     weights: str = "imagenet",
     trainable: str = "frozen",
     l2_norm: bool = True,
     include_top: bool = True,
     pooling: str = "gem",
-    gem_p=3.0,
+    gem_p: float = 3.0,
 ) -> SimilarityModel:
     """Build an ResNet50 Model backbone for similarity learning
 
     Architecture from [Deep Residual Learning for Image Recognition](https://arxiv.org/abs/1512.03385)
 
     Args:
         input_shape: Size of the image input prior to augmentation,
@@ -103,15 +103,15 @@
             outputs = layers.Dense(embedding_size)(x)
     else:
         outputs = x
 
     return SimilarityModel(inputs, outputs)
 
 
-def build_resnet(weights: str = None, trainable: str = "full") -> tf.keras.Model:
+def build_resnet(weights: str | None = None, trainable: str = "full") -> tf.keras.Model:
     """Build the requested ResNet.
 
     Args:
         weights: Use pre-trained weights - the only available currently being
         imagenet.
 
         trainable: Make the ResNet backbone fully trainable or partially
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/augmentation_utils/color_jitter.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/augmentation_utils/color_jitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,40 @@
+# Copyright 2020 The TensorFlow Authors. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
+from __future__ import annotations
+
 import functools
 
 import tensorflow as tf
 
 from tensorflow_similarity.augmenters.augmentation_utils.random_apply import (
     random_apply,
 )
 from tensorflow_similarity.types import Tensor
 
 
 def color_jitter(
     image: Tensor,
     strength: float = 1.0,
-    brightness_multiplier=0.8,
-    contrast_multiplier=0.8,
-    saturation_multiplier=0.8,
-    hue_multiplier=0.2,
+    brightness_multiplier: float = 0.8,
+    contrast_multiplier: float = 0.8,
+    saturation_multiplier: float = 0.8,
+    hue_multiplier: float = 0.2,
     random_order: bool = True,
     impl: str = "multiplicative",
 ) -> Tensor:
     """Distorts the color of the image.
 
     Args:
       image: The input image tensor.
@@ -39,18 +55,18 @@
         return color_jitter_rand(image, brightness, contrast, saturation, hue, impl=impl)
     else:
         return color_jitter_nonrand(image, brightness, contrast, saturation, hue, impl=impl)
 
 
 def color_jitter_nonrand(
     image: Tensor,
-    brightness: float = 0,
-    contrast: float = 0,
-    saturation: float = 0,
-    hue: float = 0,
+    brightness: float = 0.0,
+    contrast: float = 0.0,
+    saturation: float = 0.0,
+    hue: float = 0.0,
     impl: str = "multiplicative",
 ) -> Tensor:
     """Distorts the color of the image (jittering order is fixed).
 
     Args:
       image: The input image tensor.
       brightness: A float, specifying the brightness for color jitter.
@@ -88,18 +104,18 @@
             image = apply_transform(i, image, brightness, contrast, saturation, hue)
             image = tf.clip_by_value(image, 0.0, 1.0)
         return image
 
 
 def color_jitter_rand(
     image: Tensor,
-    brightness: float = 0,
-    contrast: float = 0,
-    saturation: float = 0,
-    hue: float = 0,
+    brightness: float = 0.0,
+    contrast: float = 0.0,
+    saturation: float = 0.0,
+    hue: float = 0.0,
     impl: str = "multiplicative",
 ) -> Tensor:
     """Distorts the color of the image (jittering order is random).
 
     Args:
       image: The input image tensor.
       brightness: A float, specifying the brightness for color jitter.
@@ -183,20 +199,20 @@
     else:
         raise ValueError("Unknown impl {} for random brightness.".format(impl))
     return image
 
 
 def random_color_jitter(
     image: Tensor,
-    p_execute=1.0,
+    p_execute: float = 1.0,
     p_jitter: float = 0.8,
-    brightness_multiplier=0.8,
-    contrast_multiplier=0.8,
-    saturation_multiplier=0.8,
-    hue_multiplier=0.2,
+    brightness_multiplier: float = 0.8,
+    contrast_multiplier: float = 0.8,
+    saturation_multiplier: float = 0.8,
+    hue_multiplier: float = 0.2,
     p_grey: float = 0.2,
     strength: float = 1.0,
     impl: str = "multiplicative",
 ) -> Tensor:
     def _transform(image: Tensor) -> Tensor:
         color_jitter_t = functools.partial(
             color_jitter,
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/augmentation_utils/cropping.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/augmentation_utils/cropping.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,36 @@
-from typing import Tuple
+# Copyright 2021 The TensorFlow Authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+from __future__ import annotations
 
 import tensorflow as tf
 
 from tensorflow_similarity.augmenters.augmentation_utils.random_apply import (
     random_apply,
 )
 from tensorflow_similarity.types import Tensor
 
 
 def _compute_crop_shape(
     image_height: int,
     image_width: int,
     aspect_ratio: float,
     crop_proportion: float,
-) -> Tuple[int, int]:
+) -> tuple[int, int]:
     """Compute aspect ratio-preserving shape for central crop.
 
     The resulting shape retains `crop_proportion` along one side and a
     proportion less than or equal to `crop_proportion` along the other side.
 
     Args:
       image_height: Height of image to be cropped.
@@ -83,18 +96,18 @@
     return image
 
 
 def distorted_bounding_box_crop(
     image: Tensor,
     bbox: Tensor,
     min_object_covered: float = 0.1,
-    aspect_ratio_range: Tuple[float, float] = (0.75, 1.33),
-    area_range: Tuple[float, float] = (0.05, 1.0),
+    aspect_ratio_range: tuple[float, float] = (0.75, 1.33),
+    area_range: tuple[float, float] = (0.05, 1.0),
     max_attempts: int = 100,
-    scope: bool = None,
+    scope: bool | None = None,
 ) -> Tensor:
     """Generates cropped_image using one of the bboxes randomly distorted.
 
     See `tf.image.sample_distorted_bounding_box` for more documentation.
 
     Args:
       image: `Tensor` of image data.
@@ -137,15 +150,15 @@
         return image
 
 
 def crop_and_resize(
     image: Tensor,
     height: int,
     width: int,
-    area_range: Tuple[float, float] = (0.08, 1.0),
+    area_range: tuple[float, float] = (0.08, 1.0),
 ) -> Tensor:
     """Make a random crop and resize it to height `height` and width `width`.
 
     Args:
       image: Tensor representing the image.
       height: Desired image height.
       width: Desired image width.
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/augmenter.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/augmenter.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,36 +7,33 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+from __future__ import annotations
 
 import abc
 
-# from tensorflow import Tensor
-from typing import List
-
 from tensorflow_similarity.types import Tensor
 
 
 class Augmenter(abc.ABC):
     @abc.abstractmethod
     def augment(
         self,
         x: Tensor,
         y: Tensor,
         num_augmentations_per_example: int,
         is_warmup: bool,
-    ) -> List[Tensor]:
+    ) -> list[Tensor]:
         pass
 
     def __call__(
         self,
         x: Tensor,
         y: Tensor,
         num_augmentations_per_example: int,
         is_warmup: bool,
-    ) -> List[Tensor]:
+    ) -> list[Tensor]:
         return self.augment(x, y, num_augmentations_per_example, is_warmup)
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/barlow.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/barlow.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,26 @@
+# Copyright 2020 The TensorFlow Authors. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
+from __future__ import annotations
+
 import os
 from functools import partial
-from typing import Any, List, Optional
+from typing import Any
 
 import tensorflow as tf
 
 from tensorflow_similarity.augmenters import Augmenter
 from tensorflow_similarity.types import Tensor
 
 from .augmentation_utils.blur import random_blur
@@ -83,15 +99,15 @@
         blur_probability=0.2,
         blur_min_sigma=0,
         blur_max_sigma=1,
         solarize_probability=0.2,
         solarize_pixel_min=0,
         solarize_pixel_max=255,
         solarize_thresh=10,
-        num_cpu: Optional[int] = os.cpu_count(),
+        num_cpu: int | None = os.cpu_count(),
     ):
         super().__init__()
         self.num_cpu = num_cpu
         self.width = width
         self.height = height
         self.flip_probability = flip_probability
         self.brightness_multiplier = brightness_multiplier
@@ -111,15 +127,15 @@
     @tf.function
     def augment(
         self,
         x: Any,
         y: Any = None,
         num_augmentations_per_example: int = 2,
         is_warmup: bool = True,
-    ) -> List[Any]:
+    ) -> list[Any]:
 
         with tf.device("/cpu:0"):
             if y is None:
                 y = tf.constant([0])
             inputs = tf.stack(x)
             inputs = tf.cast(inputs, dtype="float32")
 
@@ -157,9 +173,9 @@
 
     def __call__(
         self,
         x: Any,
         y: Any = None,
         num_augmentations_per_example: int = 2,
         is_warmup: bool = True,
-    ) -> List[Any]:
+    ) -> list[Any]:
         return list(self.augment(x, y))
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/contrastive.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/contrastive.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,30 +7,31 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 import os
-from typing import Callable, List, Optional
+from collections.abc import Callable
 
 import tensorflow as tf
 
 from tensorflow_similarity.augmenters import Augmenter
 from tensorflow_similarity.types import Tensor
 
 
 class ContrastiveAugmenter(Augmenter):
-    def __init__(self, process: Callable, num_cpu: Optional[int] = os.cpu_count()):
+    def __init__(self, process: Callable, num_cpu: int | None = os.cpu_count()):
         self.process = process
         self.num_cpu = num_cpu
 
-    def augment(self, x: Tensor, y: Tensor, num_views: int, is_warmup: bool) -> List[Tensor]:
+    def augment(self, x: Tensor, y: Tensor, num_views: int, is_warmup: bool) -> list[Tensor]:
         with tf.device("/cpu:0"):
             inputs = tf.stack(x)
 
             views = []
             for _ in range(num_views):
                 # multi-cor augementations
                 view = tf.map_fn(self.process, inputs, parallel_iterations=self.num_cpu)
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/augmenters/simclr.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/augmenters/simclr.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific simclr governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Data preprocessing and augmentation."""
+from __future__ import annotations
 
 import os
-from typing import List, Optional
 
 import tensorflow as tf
 
 from tensorflow_similarity.augmenters import Augmenter
 from tensorflow_similarity.types import Tensor
 
 from .augmentation_utils.color_jitter import random_color_jitter
@@ -102,15 +102,15 @@
         is_training: bool = True,
         color_distort: bool = True,
         jitter_stength: float = 1.0,
         crop: bool = True,
         eval_crop_proportion: float = 0.875,  # imagenet standard
         flip: bool = True,
         version: str = "v2",
-        num_cpu: Optional[int] = os.cpu_count(),
+        num_cpu: int | None = os.cpu_count(),
     ):
 
         self.width = width
         self.height = height
         self.is_training = is_training
         self.color_distort = color_distort
         self.jitter_stength = jitter_stength
@@ -127,15 +127,15 @@
 
         if self.is_training:
             self.augment_img = self._train_augment_img
         else:
             self.augment_img = self._eval_augment_img
 
     @tf.function
-    def augment(self, x: Tensor, y: Tensor, num_views: int, is_warmup: bool) -> List[Tensor]:
+    def augment(self, x: Tensor, y: Tensor, num_views: int, is_warmup: bool) -> list[Tensor]:
 
         with tf.device("/cpu:0"):
             inputs = tf.stack(x)
             inputs = tf.cast(inputs, dtype="float32") / 255.0
             views = []
 
             for _ in range(num_views):
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/callbacks.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/callbacks.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Specialized callbacks that track similarity metrics during training"""
+from __future__ import annotations
+
 import math
+from collections.abc import MutableMapping, Sequence
 from pathlib import Path
-from typing import Dict, List, Optional, Sequence, Union
 
 import numpy as np
 import tensorflow as tf
 from tensorflow.keras.callbacks import Callback
 
-from .classification_metrics import make_classification_metric  # noqa
-from .classification_metrics import ClassificationMetric
+from .classification_metrics import ClassificationMetric, make_classification_metric
 from .evaluators import Evaluator, MemoryEvaluator
 from .matchers import ClassificationMatch
 from .models import SimilarityModel
+from .retrieval_metrics import RetrievalMetric
 from .types import FloatTensor, IntTensor, Tensor
 from .utils import unpack_lookup_distances, unpack_lookup_labels, unpack_results
 
 
 class EvalCallback(Callback):
     """Epoch end evaluation callback that build a test index and evaluate
     model performance on it.
@@ -41,23 +43,21 @@
     def __init__(
         self,
         queries: Tensor,
         query_labels: Sequence[int],
         targets: Tensor,
         target_labels: Sequence[int],
         distance: str = "cosine",
-        metrics: Sequence[Union[str, ClassificationMetric]] = [
-            "binary_accuracy",
-            "f1score",
-        ],  # noqa
-        tb_logdir: str = None,
+        metrics: Sequence[str | ClassificationMetric] = ["binary_accuracy"],
+        tb_logdir: str | None = None,
         k: int = 1,
-        matcher: Union[str, ClassificationMatch] = "match_nearest",
-        distance_thresholds: Optional[FloatTensor] = None,
-        known_classes: Optional[IntTensor] = None,
+        matcher: str | ClassificationMatch = "match_nearest",
+        distance_thresholds: FloatTensor | None = None,
+        known_classes: IntTensor | None = None,
+        retrieval_metrics: Sequence[RetrievalMetric] | None = None,
     ):
         """Evaluate model matching quality against a validation dataset at
         epoch end.
 
         Args:
             queries: Test examples that will be tested against the built index.
 
@@ -102,15 +102,16 @@
         # Ensure all label tensors have the same dtype.
         self.target_labels = tf.cast(self.target_labels, dtype=t_query_labels.dtype)
 
         self.targets = targets
         self.distance = distance
         self.evaluator = MemoryEvaluator()
         # typing requires this weird formulation of creating a new list
-        self.metrics: List[ClassificationMetric] = [make_classification_metric(m) for m in metrics]
+        self.classification_metrics: list[ClassificationMetric] = [make_classification_metric(m) for m in metrics]
+        self.retrieval_metrics = retrieval_metrics if retrieval_metrics is not None else []
         self.k = k
         self.matcher = matcher
 
         if distance_thresholds is not None:
             self.distance_thresholds = distance_thresholds
         else:
             self.distance_thresholds = tf.constant([math.inf])
@@ -159,15 +160,15 @@
                     self.query_labels_unknown = tf.expand_dims(self.query_labels_unknown, axis=0)
             else:
                 self.queries_known = queries
                 self.query_labels_known = t_query_labels
                 self.queries_unknown = None
                 self.query_labels_unknown = None
 
-    def on_epoch_end(self, epoch: int, logs: dict = None):
+    def on_epoch_end(self, epoch: int, logs: MutableMapping | None = None):
         """Computes the eval metrics at the end of each epoch.
 
         NOTE: This method resets the index and batch adds the target embeddings
         to the index using the new embeddings generated by the current version
         of the model.
         """
         _ = epoch
@@ -176,138 +177,84 @@
 
         # reset the index
         self.model.reset_index()
 
         # rebuild the index
         self.model.index(self.targets, self.target_labels, verbose=0)
 
-        known_results = _compute_classification_metrics(
+        known_results = _compute_metrics(
             queries=self.queries_known,
             query_labels=self.query_labels_known,
             model=self.model,
             evaluator=self.evaluator,
-            metrics=self.metrics,
+            classification_metrics=self.classification_metrics,
+            retrieval_metrics=self.retrieval_metrics,
             k=self.k,
             matcher=self.matcher,
             distance_thresholds=self.distance_thresholds,
         )
 
+        mstr = []
+
         if self.split_validation:
-            unknown_results = _compute_classification_metrics(
+            unknown_results = _compute_metrics(
                 queries=self.queries_unknown,
                 query_labels=self.query_labels_unknown,
                 model=self.model,
                 evaluator=self.evaluator,
-                metrics=self.metrics,
+                classification_metrics=self.classification_metrics,
+                retrieval_metrics=self.retrieval_metrics,
                 k=self.k,
                 matcher=self.matcher,
                 distance_thresholds=self.distance_thresholds,
             )
 
-            mstr = unpack_results(
-                known_results,
-                epoch=epoch,
-                logs=logs,
-                tb_writer=self.tb_writer,
-                name_suffix="_known_classes",
-            )
-            mstr.extend(
-                unpack_results(
-                    unknown_results,
-                    epoch=epoch,
-                    logs=logs,
-                    tb_writer=self.tb_writer,
-                    name_suffix="_unknown_classes",
+            for a, b in zip(known_results, unknown_results):
+                mstr.extend(
+                    unpack_results(
+                        a,
+                        epoch=epoch,
+                        logs=logs,
+                        tb_writer=self.tb_writer,
+                        name_suffix="_known_classes",
+                    )
+                )
+                mstr.extend(
+                    unpack_results(
+                        b,
+                        epoch=epoch,
+                        logs=logs,
+                        tb_writer=self.tb_writer,
+                        name_suffix="_unknown_classes",
+                    )
                 )
-            )
         else:
-            mstr = unpack_results(known_results, epoch=epoch, logs=logs, tb_writer=self.tb_writer)
+            for a in known_results:
+                mstr.extend(
+                    unpack_results(
+                        a,
+                        epoch=epoch,
+                        logs=logs,
+                        tb_writer=self.tb_writer,
+                    )
+                )
         self.model.reset_index()
-        print(" - ".join(mstr))
 
 
-def SplitValidationLoss(
-    queries: Tensor,
-    query_labels: Sequence[int],
-    targets: Tensor,
-    target_labels: Sequence[int],
-    known_classes: IntTensor,
-    distance: str = "cosine",
-    metrics: Sequence[Union[str, ClassificationMetric]] = [
-        "binary_accuracy",
-        "f1score",
-    ],  # noqa
-    tb_logdir: str = None,
-    k: int = 1,
-    matcher: Union[str, ClassificationMatch] = "match_nearest",
-    distance_thresholds: Optional[FloatTensor] = None,
-):
-    """Creates the validation callbacks.
-
-    Args:
-        queries: Test examples that will be tested against the built index.
-
-        query_labels: Queries nearest neighbors expected labels.
-
-        targets: Examples that are indexed.
-
-        target_labels: Target examples labels.
-
-        known_classes: The set of classes seen during training.
-
-        distance: Distance function used to compute pairwise distance
-        between examples embeddings.
-
-        metrics: List of
-        'tf.similarity.classification_metrics.ClassificationMetric()` to
-        compute during the evaluation. Defaults to ['binary_accuracy',
-        'f1score'].
-
-        tb_logdir: Where to write TensorBoard logs. Defaults to None.
-
-        k: The number of nearest neighbors to return for each query.
-        The lookups are consumed by the Matching Strategy and used to
-        derive the matching label and distance.
-
-        matcher: {'match_nearest', 'match_majority_vote'} or
-        ClassificationMatch object. Defines the classification matching,
-        e.g., match_nearest will count a True Positive if the query_label
-        is equal to the label of the nearest neighbor and the distance is
-        less than or equal to the distance threshold.
-
-        distance_thresholds: A 1D tensor denoting the distances points at
-        which we compute the metrics. If None, distance_thresholds is set
-        to tf.constant([math.inf])
-    """
-    print("WARNING: SplitValidationLoss is deprecated. Please use EvalCallback.")
-    return EvalCallback(
-        queries=queries,
-        query_labels=query_labels,
-        targets=targets,
-        target_labels=target_labels,
-        distance=distance,
-        metrics=metrics,
-        tb_logdir=tb_logdir,
-        k=k,
-        matcher=matcher,
-        distance_thresholds=distance_thresholds,
-        known_classes=known_classes,
-    )
-
-
-def _compute_classification_metrics(
+def _compute_metrics(
     queries: Tensor,
     query_labels: IntTensor,
     model: SimilarityModel,
     evaluator: Evaluator,
-    metrics: Sequence[ClassificationMetric],
+    classification_metrics: Sequence[ClassificationMetric],
+    retrieval_metrics: Sequence[RetrievalMetric],
     k: int,
-    matcher: Union[str, ClassificationMatch],
+    matcher: str | ClassificationMatch,
     distance_thresholds: FloatTensor,
-) -> Dict[str, np.ndarray]:
+) -> tuple[dict[str, np.ndarray], dict[str, np.ndarray]]:
     """Compute the classification metrics.
 
     Args:
         queries: A Tensor of embeddings representing the queries.
 
         query_labels: An IntTensor representing the class ids associated with
             the queries.
@@ -332,23 +279,32 @@
     Returns:
         A Python dict mapping the metric name to the copmuted value.
     """
     lookups = model.lookup(queries, k=k, verbose=0)
     lookup_distances = unpack_lookup_distances(lookups, model.dtype)
     lookup_labels = unpack_lookup_labels(lookups, query_labels.dtype)
 
-    # TODO(ovallis): Support passing other matchers. Currently we are using
-    # match_nearest.
-    results = evaluator.evaluate_classification(
-        query_labels=query_labels,
-        lookup_labels=lookup_labels,
-        lookup_distances=lookup_distances,
-        distance_thresholds=distance_thresholds,
-        metrics=metrics,
-        matcher=matcher,
-        verbose=0,
-    )
-
-    # The callbacks don't set a distance theshold so we remove it here.
-    results.pop("distance")
+    if classification_metrics:
+        classification_results = evaluator.evaluate_classification(
+            query_labels=query_labels,
+            lookup_labels=lookup_labels,
+            lookup_distances=lookup_distances,
+            distance_thresholds=distance_thresholds,
+            metrics=classification_metrics,
+            matcher=matcher,
+            verbose=0,
+        )
+        # The callbacks don't set a distance theshold so we remove it here.
+        classification_results.pop("distance")
+    else:
+        classification_results = {}
+
+    if retrieval_metrics:
+        retrieval_results = evaluator.evaluate_retrieval(
+            target_labels=query_labels,
+            lookups=lookups,
+            retrieval_metrics=retrieval_metrics,
+        )
+    else:
+        retrieval_results = {}
 
-    return results
+    return classification_results, retrieval_results
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/__init__.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/binary_accuracy.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/binary_accuracy.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 import tensorflow as tf
 
 from tensorflow_similarity.types import FloatTensor
 
 from .classification_metric import ClassificationMetric
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/classification_metric.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/classification_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 from abc import ABC, abstractmethod
 
 from tensorflow_similarity.types import FloatTensor
 
 
 class ClassificationMetric(ABC):
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/f1_score.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/f1_score.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 import tensorflow as tf
 
 from tensorflow_similarity.types import FloatTensor
 
 from .classification_metric import ClassificationMetric
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/false_positive_rate.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/false_positive_rate.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 import tensorflow as tf
 
 from tensorflow_similarity.types import FloatTensor
 
 from .classification_metric import ClassificationMetric
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/negative_predictive_value.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/negative_predictive_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 import tensorflow as tf
 
 from tensorflow_similarity.types import FloatTensor
 
 from .classification_metric import ClassificationMetric
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/precision.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/precision.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 import tensorflow as tf
 
 from tensorflow_similarity.types import FloatTensor
 
 from .classification_metric import ClassificationMetric
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/recall.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/recall.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 import tensorflow as tf
 
 from tensorflow_similarity.types import FloatTensor
 
 from .classification_metric import ClassificationMetric
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/classification_metrics/utils.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/classification_metrics/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,40 +7,41 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
-from typing import Dict, Type, Union
+from typing import Type
 
 from .binary_accuracy import BinaryAccuracy  # noqa
 from .classification_metric import ClassificationMetric  # noqa
 from .f1_score import F1Score  # noqa
 from .false_positive_rate import FalsePositiveRate  # noqa
 from .negative_predictive_value import NegativePredictiveValue  # noqa
 from .precision import Precision  # noqa
 from .recall import Recall  # noqa
 
 
-def make_classification_metric(metric: Union[str, ClassificationMetric], name: str = "") -> ClassificationMetric:
+def make_classification_metric(metric: str | ClassificationMetric, name: str = "") -> ClassificationMetric:
     """Convert classification metric from str name to object if needed.
 
     Args:
         metric: ClassificationMetric() or metric name.
 
     Raises:
         ValueError: Unknown metric name: {metric}, typo?
 
     Returns:
         ClassificationMetric: Instantiated metric if needed.
     """
     # ! Metrics must be non-instantiated.
-    METRICS_ALIASES: Dict[str, Type[ClassificationMetric]] = {
+    METRICS_ALIASES: dict[str, Type[ClassificationMetric]] = {
         "recall": Recall,
         "precision": Precision,
         "f1": F1Score,
         "f1score": F1Score,
         "f1_score": F1Score,
         "binary_accuracy": BinaryAccuracy,
         "npv": NegativePredictiveValue,
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/distances.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/distances.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,32 +8,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Vectorized embedding pairwise distances computation functions"""
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
-from typing import List, Union
+from collections.abc import Sequence
 
 import tensorflow as tf
 
 from .types import FloatTensor
 
 
 class Distance(ABC):
     """
     Note: don't forget to add your distance to the DISTANCES list
     and add alias names in it.
 
     """
 
-    def __init__(self, name: str, aliases: List[str] = []):
-        self.name = name
-        self.aliases = aliases
+    def __init__(self, name: str, aliases: Sequence[str]):
+        self.name = name if name is not None else "distance"
+        self.aliases = aliases if aliases is not None else None
 
     @abstractmethod
     def call(self, query_embeddings: FloatTensor, key_embeddings: FloatTensor) -> FloatTensor:
         """Compute pairwise distances for a given batch.
 
         Args:
             query_embeddings: Embeddings to compute the pairwise one.
@@ -46,15 +48,15 @@
     def __call__(self, query_embeddings: FloatTensor, key_embeddings: FloatTensor):
         return self.call(query_embeddings, key_embeddings)
 
     def __str__(self) -> str:
         return self.name
 
     def get_config(self):
-        return {}
+        return {"name": self.name, "aliases": self.aliases}
 
 
 @tf.keras.utils.register_keras_serializable(package="Similarity")
 class InnerProductSimilarity(Distance):
     """Compute the pairwise inner product between embeddings.
 
     The [Inner product](https://en.wikipedia.org/wiki/Inner_product_space) is
@@ -63,17 +65,19 @@
 
     NOTE! This is not a distance and is likely not what you want to use with
     the built in losses. At the very least this will flip the sign on the
     margin in many of the losses. This is likely meant to be used with custom
     loss functions that expect a similarity instead of a distance.
     """
 
-    def __init__(self):
+    def __init__(self, name: str | None = None, aliases: Sequence[str] | None = None):
         "Init Inner product similarity"
-        super().__init__("inner_product", ["ip"])
+        name = name if name is not None else "inner_product"
+        aliases = aliases if aliases is not None else ["ip"]
+        super().__init__(name, aliases)
 
     @tf.function
     def call(self, query_embeddings: FloatTensor, key_embeddings: FloatTensor) -> FloatTensor:
         """Compute pairwise similarities for a given batch of embeddings.
 
         Args:
             query_embeddings: Embeddings to compute the pairwise one.
@@ -91,17 +95,19 @@
 class CosineDistance(Distance):
     """Compute pairwise cosine distances between embeddings.
 
     The [Cosine Distance](https://en.wikipedia.org/wiki/Cosine_similarity) is
     an angular distance that varies from 0 (similar) to 1 (dissimilar).
     """
 
-    def __init__(self):
+    def __init__(self, name: str | None = None, aliases: Sequence[str] | None = None):
         "Init Cosine distance"
-        super().__init__("cosine")
+        name = name if name is not None else "cosine"
+        aliases = aliases if aliases is not None else []
+        super().__init__(name, aliases)
 
     @tf.function
     def call(self, query_embeddings: FloatTensor, key_embeddings: FloatTensor) -> FloatTensor:
         """Compute pairwise distances for a given batch of embeddings.
 
         Args:
             query_embeddings: Embeddings to compute the pairwise one. The embeddings
@@ -125,17 +131,19 @@
     is the standard distance to measure the line segment between two embeddings
     in the Cartesian point. The larger the distance the more dissimilar
     the embeddings are.
 
     **Alias**: L2 Norm, Pythagorean
     """
 
-    def __init__(self):
+    def __init__(self, name: str | None = None, aliases: Sequence[str] | None = None):
         "Init Euclidean distance"
-        super().__init__("euclidean", ["l2", "pythagorean"])
+        name = name if name is not None else "euclidean"
+        aliases = aliases if aliases is not None else ["l2", "pythagorean"]
+        super().__init__(name, aliases)
 
     @tf.function
     def call(self, query_embeddings: FloatTensor, key_embeddings: FloatTensor) -> FloatTensor:
         """Compute pairwise distances for a given batch of embeddings.
 
         Args:
             query_embeddings: Embeddings to compute the pairwise one.
@@ -168,16 +176,19 @@
 class SquaredEuclideanDistance(Distance):
     """Compute pairwise squared Euclidean distance.
 
     The [Squared Euclidean Distance](https://en.wikipedia.org/wiki/Euclidean_distance#Squared_Euclidean_distance) is
     a distance that varies from 0 (similar) to infinity (dissimilar).
     """
 
-    def __init__(self):
-        super().__init__("squared_euclidean", ["sql2", "sqeuclidean"])
+    def __init__(self, name: str | None = None, aliases: Sequence[str] | None = None):
+        "Init Squared Euclidean distance"
+        name = name if name is not None else "squared_euclidean"
+        aliases = aliases if aliases is not None else ["sql2", "sqeuclidean"]
+        super().__init__(name, aliases)
 
     @tf.function
     def call(self, query_embeddings: FloatTensor, key_embeddings: FloatTensor) -> FloatTensor:
         """Compute pairwise distances for a given batch of embeddings.
 
         Args:
             query_embeddings: Embeddings to compute the pairwise one.
@@ -205,17 +216,19 @@
 
     The [Manhattan Distance](https://en.wikipedia.org/wiki/Euclidean_distance)
     is the sum of the lengths of the projections of the line segment between
     two embeddings onto the Cartesian axes. The larger the distance the more
     dissimilar the embeddings are.
     """
 
-    def __init__(self):
+    def __init__(self, name: str | None = None, aliases: Sequence[str] | None = None):
         "Init Manhattan distance"
-        super().__init__("manhattan", ["l1", "taxicab"])
+        name = name if name is not None else "manhattan"
+        aliases = aliases if aliases is not None else ["l1", "taxicab"]
+        super().__init__(name, aliases)
 
     @tf.function
     def call(self, query_embeddings: FloatTensor, key_embeddings: FloatTensor) -> FloatTensor:
         """Compute pairwise distances for a given batch of embeddings.
 
         Args:
             query_embeddings: Embeddings to compute the pairwise one.
@@ -236,17 +249,19 @@
     """
     Computes pairwise SNR distances between embeddings.
 
     The [Signal-to-Noise Ratio distance](https://arxiv.org/abs/1904.02616)
     is the ratio of noise variance to the feature variance.
     """
 
-    def __init__(self):
+    def __init__(self, name: str | None = None, aliases: Sequence[str] | None = None):
         "Init SNR distance"
-        super().__init__("snr")
+        name = name if name is not None else "snr"
+        aliases = aliases if aliases is not None else ["signal-to-noise-ratio"]
+        super().__init__(name, aliases)
 
     @tf.function
     def call(self, query_embeddings: FloatTensor, key_embeddings: FloatTensor) -> FloatTensor:
         """Compute pairwise snr distances for a given batch of embeddings.
         SNR(i, j): anchor i and compared feature j
         SNR(i,j) may not be equal to SNR(j, i)
 
@@ -277,15 +292,15 @@
     SquaredEuclideanDistance(),
     ManhattanDistance(),
     CosineDistance(),
     SNRDistance(),
 ]
 
 
-def distance_canonicalizer(user_distance: Union[Distance, str]) -> Distance:
+def distance_canonicalizer(user_distance: Distance | str) -> Distance:
     """Normalize user requested distance to its matching Distance object.
 
     Args:
         user_distance: Requested distance either by name or by object
 
     Returns:
         Distance: Requested object name.
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/evaluators/__init__.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/evaluators/evaluator.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/evaluators/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Dict, MutableMapping, Sequence, Union
+from collections.abc import MutableMapping, Sequence
 
 import numpy as np
 
 from tensorflow_similarity.classification_metrics import ClassificationMetric
 from tensorflow_similarity.matchers import ClassificationMatch
 from tensorflow_similarity.retrieval_metrics import RetrievalMetric
 from tensorflow_similarity.types import (
@@ -40,15 +41,15 @@
     @abstractmethod
     def evaluate_retrieval(
         self,
         target_labels: Sequence[int],
         lookups: Sequence[Sequence[Lookup]],
         retrieval_metrics: Sequence[RetrievalMetric],
         distance_rounding: int = 8,
-    ) -> Dict[str, np.ndarray]:
+    ) -> dict[str, np.ndarray]:
         """Evaluates lookup performances against a supplied set of metrics
 
         Args:
             target_labels: Sequence of the expected labels to match.
 
             lookups: Sequence of lookup results as produced by the
             `Index().batch_lookup()` method.
@@ -68,18 +69,18 @@
     def evaluate_classification(
         self,
         query_labels: IntTensor,
         lookup_labels: IntTensor,
         lookup_distances: FloatTensor,
         distance_thresholds: FloatTensor,
         metrics: Sequence[ClassificationMetric],
-        matcher: Union[str, ClassificationMatch],
+        matcher: str | ClassificationMatch,
         distance_rounding: int = 8,
         verbose: int = 1,
-    ) -> Dict[str, np.ndarray]:
+    ) -> dict[str, np.ndarray]:
         """Evaluate the classification performance.
 
         Compute the classification metrics given a set of queries, lookups, and
         distance thresholds.
 
         Args:
             query_labels: Sequence of expected labels for the lookups.
@@ -113,15 +114,15 @@
     @abstractmethod
     def calibrate(
         self,
         target_labels: Sequence[int],
         lookups: Sequence[Sequence[Lookup]],
         thresholds_targets: MutableMapping[str, float],
         calibration_metric: ClassificationMetric,
-        matcher: Union[str, ClassificationMatch],
+        matcher: str | ClassificationMatch,
         extra_metrics: Sequence[ClassificationMetric] = [],
         distance_rounding: int = 8,
         metric_rounding: int = 6,
         verbose: int = 1,
     ) -> CalibrationResults:
         """Computes the distances thresholds that the classification must match to
         meet a fixed target.
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/evaluators/memory_evaluator.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/evaluators/memory_evaluator.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
-from typing import Dict, MutableMapping, Sequence, Union
+from collections.abc import MutableMapping, Sequence
 
 import numpy as np
 import tensorflow as tf
 from tqdm.auto import tqdm
 
 from tensorflow_similarity.classification_metrics import ClassificationMetric
 from tensorflow_similarity.matchers import (
@@ -41,15 +42,15 @@
 
     def evaluate_retrieval(
         self,
         target_labels: Sequence[int],
         lookups: Sequence[Sequence[Lookup]],
         retrieval_metrics: Sequence[RetrievalMetric],
         distance_rounding: int = 8,
-    ) -> Dict[str, np.ndarray]:
+    ) -> dict[str, np.ndarray]:
         """Evaluates lookup performances against a supplied set of metrics
 
         Args:
             target_labels: Sequence of the expected labels to match.
 
             lookups: Sequence of lookup results as produced by the
             `Index().batch_lookup()` method.
@@ -102,18 +103,18 @@
     def evaluate_classification(
         self,
         query_labels: IntTensor,
         lookup_labels: IntTensor,
         lookup_distances: FloatTensor,
         distance_thresholds: FloatTensor,
         metrics: Sequence[ClassificationMetric],
-        matcher: Union[str, ClassificationMatch],
+        matcher: str | ClassificationMatch,
         distance_rounding: int = 8,
         verbose: int = 1,
-    ) -> Dict[str, np.ndarray]:
+    ) -> dict[str, np.ndarray]:
         """Evaluate the classification performance.
 
         Compute the classification metrics given a set of queries, lookups, and
         distance thresholds.
 
         Args:
             query_labels: Sequence of expected labels for the lookups.
@@ -155,15 +156,15 @@
         )
 
         # evaluating performance as distance value increase
         if verbose:
             pb = tqdm(total=len(metrics), desc="Evaluating")
 
         # evaluating performance as distance value increase
-        results: Dict[str, np.ndarray] = {"distance": distance_thresholds.numpy()}
+        results: dict[str, np.ndarray] = {"distance": distance_thresholds.numpy()}
         for m in metrics:
             res = m.compute(
                 tp=matcher.tp,
                 fp=matcher.fp,
                 tn=matcher.tn,
                 fn=matcher.fn,
                 count=matcher.count,
@@ -180,15 +181,15 @@
 
     def calibrate(
         self,
         target_labels: Sequence[int],
         lookups: Sequence[Sequence[Lookup]],
         thresholds_targets: MutableMapping[str, float],
         calibration_metric: ClassificationMetric,
-        matcher: Union[str, ClassificationMatch],
+        matcher: str | ClassificationMatch,
         extra_metrics: Sequence[ClassificationMetric] = [],
         distance_rounding: int = 8,
         metric_rounding: int = 6,
         verbose: int = 1,
     ) -> CalibrationResults:
         """Computes the distances thresholds that the classification must match to
         meet a fixed target.
@@ -257,15 +258,15 @@
             distance_thresholds=distance_thresholds,
             metrics=combined_metrics,
             matcher=matcher,
             distance_rounding=distance_rounding,
             verbose=verbose,
         )
 
-        cutpoints: Dict[str, Dict[str, Union[str, float]]] = {}
+        cutpoints: dict[str, dict[str, str | float]] = {}
 
         cutpoints["optimal"] = self._optimal_cutpoint(results, calibration_metric)
 
         for name, value in thresholds_targets.items():
             target_cp = self._target_cutpoints(results, calibration_metric, name, value)
             if target_cp:
                 cutpoints[name] = target_cp
@@ -273,17 +274,17 @@
         # Add the calibration metric as 'value' in the thresholds dict.
         results["value"] = results[calibration_metric.name]
 
         return CalibrationResults(cutpoints=cutpoints, thresholds=results)
 
     def _optimal_cutpoint(
         self,
-        metrics: Dict[str, np.ndarray],
+        metrics: dict[str, np.ndarray],
         calibration_metric: ClassificationMetric,
-    ) -> Dict[str, Union[str, float]]:
+    ) -> dict[str, str | float]:
         """Compute the optimal distance threshold for the calibration metric.
 
         Args:
             metrics: A mapping from metric name to a list of metric values
               computed for each unique distance observed in the calibration
               dataset. This dict should also include a distance key mapping
               to the list of observed distances. We expect the distances to be
@@ -319,19 +320,19 @@
 
             optimal_cp[metric_name] = metrics[metric_name][idx].item()
 
         return optimal_cp
 
     def _target_cutpoints(
         self,
-        metrics: Dict[str, np.ndarray],
+        metrics: dict[str, np.ndarray],
         calibration_metric: ClassificationMetric,
         target_name: str,
         target_value: float,
-    ) -> Dict[str, Union[str, float]]:
+    ) -> dict[str, str | float]:
         """Compute the distance at the target metric for the calibration metric.
 
         Args:
             metrics: A mapping from metric name to a list of metric values
               computed for each unique distance observed in the calibration
               dataset. This dict should also include a distance key mapping
               to the list of observed distances. We expect the distances to be
@@ -355,15 +356,15 @@
                   'distance': 0.1,    # Calibrated distance.
                   'precision': 0.901, # Here, we calibrated using precision.
                   'f1': 0.4,          # We also computed F1 at this point.
               }
               ```
         """
         indicators = np.where(metrics[calibration_metric.name] >= target_value)[0]
-        target_cp: Dict[str, Union[str, float]] = {}
+        target_cp: dict[str, str | float] = {}
 
         if indicators.size > 0:
             if calibration_metric.increasing:
                 # Take the first index above the target if the metric is increasing
                 idx = indicators[0]
             else:
                 # Take the last index above the target if the metric is decreasing
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/indexer.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/indexer.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,30 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Index the embeddings infered by the model to allow distance based
 sub-linear search"""
+from __future__ import annotations
 
 import json
 from collections import defaultdict, deque
+from collections.abc import Mapping, MutableMapping, Sequence
 from pathlib import Path
 from time import time
-from typing import (
-    DefaultDict,
-    Deque,
-    Dict,
-    List,
-    Mapping,
-    MutableMapping,
-    Optional,
-    Sequence,
-    Union,
-)
 
 import numpy as np
 import tensorflow as tf
 from tabulate import tabulate
 from tqdm.auto import tqdm
 
 from .classification_metrics import (
@@ -43,15 +34,15 @@
 )
 
 # internal
 from .distances import Distance, distance_canonicalizer
 from .evaluators import Evaluator, MemoryEvaluator
 from .matchers import ClassificationMatch, make_classification_matcher
 from .retrieval_metrics import RetrievalMetric
-from .search import NMSLibSearch, Search
+from .search import NMSLibSearch, Search, make_search
 from .stores import MemoryStore, Store
 from .types import CalibrationResults, FloatTensor, Lookup, PandasDataFrame, Tensor
 from .utils import unpack_lookup_distances, unpack_lookup_labels
 
 
 class Indexer:
     """Indexing system that allows to efficiently find nearest embeddings
@@ -72,19 +63,19 @@
     LABELS = 2
     DATA = 3
     RANKS = 4
 
     def __init__(
         self,
         embedding_size: int,
-        distance: Union[Distance, str] = "cosine",
-        search: Union[Search, str] = "nmslib",
-        kv_store: Union[Store, str] = "memory",
-        evaluator: Union[Evaluator, str] = "memory",
-        embedding_output: int = None,
+        distance: Distance | str = "cosine",
+        search: Search | str = "nmslib",
+        kv_store: Store | str = "memory",
+        evaluator: Evaluator | str = "memory",
+        embedding_output: int | None = None,
         stat_buffer_size: int = 1000,
     ) -> None:
         """Index embeddings to make them searchable via KNN
 
         Args:
             embedding_size: Size of the embeddings that will be stored.
             It is usually equivalent to the size of the output layer.
@@ -126,53 +117,59 @@
 
         # stats configuration
         self.stat_buffer_size = stat_buffer_size
 
         # calibration
         self.is_calibrated = False
         self.calibration_metric: ClassificationMetric = F1Score()
-        self.cutpoints: Mapping[str, Mapping[str, Union[float, str]]] = {}
+        self.cutpoints: Mapping[str, Mapping[str, float | str]] = {}
         self.calibration_thresholds: Mapping[str, np.ndarray] = {}
 
         # initialize internal structures
         self._init_structures()
 
     def reset(self) -> None:
         "Reinitialize the indexer"
         self._init_structures()
 
     def _init_structures(self) -> None:
         "(re)initialize internal storage structure"
 
         if self.search_type == "nmslib":
-            self.search: Search = NMSLibSearch(distance=self.distance, dims=self.embedding_size)
+            self.search: Search = NMSLibSearch(distance=self.distance, dim=self.embedding_size)
         elif isinstance(self.search_type, Search):
-            self.search = self.search_type
+            # TODO: Temporary fix to support resetting custom objects. Currently only supports NMSLibSearch.
+            #       Search class should provide a reset method instead.
+            if type(self.search_type).__name__ != "NMSLibSearch":
+                raise ValueError("Currently NMSLibSearch is the only supported Search object.")
+            search = make_search(self.search_type.get_config())
+            self.search = search
         else:
             raise ValueError("You need to either supply a known search " "framework name or a Search() object")
 
         # mapper from id to record data
         if self.kv_store_type == "memory":
             self.kv_store: Store = MemoryStore()
         elif isinstance(self.kv_store_type, Store):
+            print("WARNING: custom store objects are not currently supported and will not be reset.")
             self.kv_store = self.kv_store_type
         else:
             raise ValueError("You need to either supply a know key value " "store name or a Store() object")
 
         # code used to evaluate indexer performance
         if self.evaluator_type == "memory":
             self.evaluator: Evaluator = MemoryEvaluator()
         elif isinstance(self.evaluator_type, Evaluator):
             self.evaluator = self.evaluator_type
         else:
             raise ValueError("You need to either supply a know evaluator name " "or an Evaluator() object")
 
         # stats
-        self._stats: DefaultDict[str, int] = defaultdict(int)
-        self._lookup_timings_buffer: Deque = deque([], maxlen=self.stat_buffer_size)
+        self._stats: defaultdict[str, int] = defaultdict(int)
+        self._lookup_timings_buffer: deque[float] = deque([], maxlen=self.stat_buffer_size)
 
         # calibration data
         self.is_calibrated = False
         self.calibration_metric = F1Score()
         self.cutpoints = {}
         self.calibration_thresholds = {}
 
@@ -212,23 +209,23 @@
         if isinstance(self.embedding_output, int):
             embeddings: FloatTensor = predictions[self.embedding_output]
         else:
             # needed for typing
             embeddings = predictions
         return embeddings
 
-    def _cast_label(self, label: Optional[int]) -> Optional[int]:
+    def _cast_label(self, label: int | None) -> int | None:
         if label is not None:
             label = int(label)
         return label
 
     def add(
         self,
         prediction: FloatTensor,
-        label: Optional[int] = None,
+        label: int | None = None,
         data: Tensor = None,
         build: bool = True,
         verbose: int = 1,
     ):
         """Add a single embedding to the indexer
 
         Args:
@@ -257,16 +254,16 @@
 
         # add index to the embedding
         self.search.add(embedding, idx, build=build, verbose=verbose)
 
     def batch_add(
         self,
         predictions: FloatTensor,
-        labels: Optional[Sequence[int]] = None,
-        data: Optional[Tensor] = None,
+        labels: Sequence[int] | None = None,
+        data: Tensor | None = None,
         build: bool = True,
         verbose: int = 1,
     ):
         """Add a batch of embeddings to the indexer
 
         Args:
             predictions: TF similarity model predictions, may be a multi-headed
@@ -288,25 +285,25 @@
 
         # store points
         if verbose:
             print("|-Storing data points in key value store")
         idxs = self.kv_store.batch_add(embeddings, labels, data)
         self.search.batch_add(embeddings, idxs, build=build, verbose=verbose)
 
-    def single_lookup(self, prediction: FloatTensor, k: int = 5) -> List[Lookup]:
+    def single_lookup(self, prediction: FloatTensor, k: int = 5) -> list[Lookup]:
         """Find the k closest matches of a given embedding
 
         Args:
             prediction: TF similarity model prediction, may be a multi-headed
             output.
 
             k: Number of nearest neighbors to lookup. Defaults to 5.
         Returns
             list of the k nearest neighbors info:
-            List[Lookup]
+            list[Lookup]
         """
 
         embedding = self._get_embedding(prediction)
         start = time()
         idxs, distances = self.search.lookup(embedding, k=k)
         nn_embeddings, labels, data = self.kv_store.batch_get(idxs)
 
@@ -323,29 +320,29 @@
                     data=data[i],
                 )
             )
         self._lookup_timings_buffer.append(lookup_time)
         self._stats["num_lookups"] += 1
         return lookups
 
-    def batch_lookup(self, predictions: FloatTensor, k: int = 5, verbose: int = 1) -> List[List[Lookup]]:
+    def batch_lookup(self, predictions: FloatTensor, k: int = 5, verbose: int = 1) -> list[list[Lookup]]:
 
         """Find the k closest matches for a set of embeddings
 
         Args:
             predictions: TF similarity model predictions, may be a multi-headed
             output.
 
             k: Number of nearest neighbors to lookup. Defaults to 5.
 
             verbose: Be verbose. Defaults to 1.
 
         Returns
             list of list of k nearest neighbors:
-            List[List[Lookup]]
+            list[list[Lookup]]
         """
 
         embeddings = self._get_embeddings(predictions)
         num_embeddings = len(embeddings)
         start = time()
         batch_lookups = []
 
@@ -392,25 +389,25 @@
     # evaluation related functions
     def evaluate_retrieval(
         self,
         predictions: FloatTensor,
         target_labels: Sequence[int],
         retrieval_metrics: Sequence[RetrievalMetric],
         verbose: int = 1,
-    ) -> Dict[str, np.ndarray]:
+    ) -> dict[str, np.ndarray]:
         """Evaluate the quality of the index against a test dataset.
 
         Args:
             predictions: TF similarity model predictions, may be a multi-headed
             output.
 
             target_labels: Sequence of the expected labels associated with the
             embedded queries.
 
-            retrieval_metrics: List of
+            retrieval_metrics: list of
             [RetrievalMetric()](retrieval_metrics/overview.md) to compute.
 
             verbose (int, optional): Display results if set to 1 otherwise
             results are returned silently. Defaults to 1.
 
         Returns:
             Dictionary of metric results where keys are the metric names and
@@ -426,34 +423,38 @@
                     "is not a valid RetrivalMetric(). The "
                     "RetrivialMetric() must be instantiated with "
                     "a valid K.",
                 )
             if m.k > k:
                 k = m.k
 
+        # Add one more K to handle the case where we drop the closest lookup.
+        # This ensures that we always have enough lookups in the result set.
+        k += 1
+
         # Find NN
         lookups = self.batch_lookup(predictions, k=k, verbose=verbose)
 
         # Evaluate them
         return self.evaluator.evaluate_retrieval(
             retrieval_metrics=retrieval_metrics,
             target_labels=target_labels,
             lookups=lookups,
         )
 
     def evaluate_classification(
         self,
         predictions: FloatTensor,
         target_labels: Sequence[int],
-        distance_thresholds: Union[Sequence[float], FloatTensor],
-        metrics: Sequence[Union[str, ClassificationMetric]] = ["f1"],
-        matcher: Union[str, ClassificationMatch] = "match_nearest",
+        distance_thresholds: Sequence[float] | FloatTensor,
+        metrics: Sequence[str | ClassificationMetric] = ["f1"],
+        matcher: str | ClassificationMatch = "match_nearest",
         k: int = 1,
         verbose: int = 1,
-    ) -> Dict[str, np.ndarray]:
+    ) -> dict[str, np.ndarray]:
         """Evaluate the classification performance.
 
         Compute the classification metrics given a set of queries, lookups, and
         distance thresholds.
 
         Args:
             predictions: TF similarity model predictions, may be a multi-headed
@@ -476,28 +477,27 @@
             decide if the distance changed. Defaults to 8.
 
             verbose: Be verbose. Defaults to 1.
         Returns:
             A Mapping from metric name to the list of values computed for each
             distance threshold.
         """
-        combined_metrics: List[ClassificationMetric] = [make_classification_metric(m) for m in metrics]
+        combined_metrics: list[ClassificationMetric] = [make_classification_metric(m) for m in metrics]
 
         lookups = self.batch_lookup(predictions, k=k, verbose=verbose)
 
         # we also convert to np.ndarray first to avoid a slow down if
-        # convert_to_tensor is called on a List.
+        # convert_to_tensor is called on a list.
         query_labels = tf.convert_to_tensor(np.array(target_labels))
 
-        # TODO(ovallis): The float type should be derived from the model.
-        lookup_distances = unpack_lookup_distances(lookups, dtype="float32")
+        lookup_distances = unpack_lookup_distances(lookups, dtype=tf.keras.backend.floatx())
         lookup_labels = unpack_lookup_labels(lookups, dtype=query_labels.dtype)
         thresholds: FloatTensor = tf.cast(
             tf.convert_to_tensor(distance_thresholds),
-            dtype=lookup_distances.dtype,
+            dtype=tf.keras.backend.floatx(),
         )
 
         results = self.evaluator.evaluate_classification(
             query_labels=query_labels,
             lookup_labels=lookup_labels,
             lookup_distances=lookup_distances,
             distance_thresholds=thresholds,
@@ -509,18 +509,18 @@
         return results
 
     def calibrate(
         self,
         predictions: FloatTensor,
         target_labels: Sequence[int],
         thresholds_targets: MutableMapping[str, float],
-        calibration_metric: Union[str, ClassificationMetric] = "f1_score",  # noqa
+        calibration_metric: str | ClassificationMetric = "f1_score",  # noqa
         k: int = 1,
-        matcher: Union[str, ClassificationMatch] = "match_nearest",
-        extra_metrics: Sequence[Union[str, ClassificationMetric]] = [
+        matcher: str | ClassificationMatch = "match_nearest",
+        extra_metrics: Sequence[str | ClassificationMetric] = [
             "precision",
             "recall",
         ],  # noqa
         rounding: int = 2,
         verbose: int = 1,
     ) -> CalibrationResults:
         """Calibrate model thresholds using a test dataset.
@@ -546,15 +546,15 @@
             matcher: {'match_nearest', 'match_majority_vote'} or
             ClassificationMatch object. Defines the classification matching,
             e.g., match_nearest will count a True Positive if the query_label
             is equal to the label of the nearest neighbor and the distance is
             less than or equal to the distance threshold.
             Defaults to 'match_nearest'.
 
-            extra_metrics: List of additional
+            extra_metrics: list of additional
             `tf.similarity.classification_metrics.ClassificationMetric()` to
             compute and report. Defaults to ['precision', 'recall'].
 
             rounding: Metric rounding. Default to 2 digits.
 
             verbose: Be verbose and display calibration results. Defaults to 1.
 
@@ -564,15 +564,15 @@
 
         # find NN
         lookups = self.batch_lookup(predictions, k=k, verbose=verbose)
 
         # making sure our metrics are all ClassificationMetric objects
         calibration_metric = make_classification_metric(calibration_metric)
 
-        combined_metrics: List[ClassificationMetric] = [make_classification_metric(m) for m in extra_metrics]
+        combined_metrics: list[ClassificationMetric] = [make_classification_metric(m) for m in extra_metrics]
 
         # running calibration
         calibration_results = self.evaluator.calibrate(
             target_labels=target_labels,
             lookups=lookups,
             thresholds_targets=thresholds_targets,
             calibration_metric=calibration_metric,
@@ -606,17 +606,17 @@
         return calibration_results
 
     def match(
         self,
         predictions: FloatTensor,
         no_match_label: int = -1,
         k=1,
-        matcher: Union[str, ClassificationMatch] = "match_nearest",
+        matcher: str | ClassificationMatch = "match_nearest",
         verbose: int = 1,
-    ) -> Dict[str, List[int]]:
+    ) -> dict[str, list[int]]:
         """Match embeddings against the various cutpoints thresholds
 
         Args:
             predictions: TF similarity model predictions, may be a multi-headed
             output.
 
             no_match_label: What label value to assign when there is no match.
@@ -648,25 +648,25 @@
         Returns:
             Dict of cutpoint names mapped to lists of matches.
         """
         matcher = make_classification_matcher(matcher)
 
         lookups = self.batch_lookup(predictions, k=k, verbose=verbose)
 
-        lookup_distances = unpack_lookup_distances(lookups, dtype=predictions.dtype)
+        lookup_distances = unpack_lookup_distances(lookups, dtype=tf.keras.backend.floatx())
         # TODO(ovallis): The int type should be derived from the model.
         lookup_labels = unpack_lookup_labels(lookups, dtype="int32")
 
         if verbose:
             pb = tqdm(
                 total=len(lookup_distances) * len(self.cutpoints),
                 desc="matching embeddings",
             )
 
-        matches: DefaultDict[str, List[int]] = defaultdict(list)
+        matches: defaultdict[str, list[int]] = defaultdict(list)
         for cp_name, cp_data in self.cutpoints.items():
             distance_threshold = float(cp_data["distance"])
 
             pred_labels, pred_dist = matcher.derive_match(
                 lookup_labels=lookup_labels, lookup_distances=lookup_distances
             )
 
@@ -700,15 +700,15 @@
             "size": self.size(),
             "compression": compression,
             "distance": self.distance.name,
             "embedding_output": self.embedding_output,
             "embedding_size": self.embedding_size,
             "kv_store": self.kv_store_type,
             "evaluator": self.evaluator_type,
-            "search": self.search_type,
+            "search_config": self.search.get_config(),
             "stat_buffer_size": self.stat_buffer_size,
             "is_calibrated": self.is_calibrated,
             "calibration_metric_config": self.calibration_metric.get_config(),
             "cutpoints": self.cutpoints,
             # convert np.arrays to list before serialization
             "calibration_thresholds": {k: v.tolist() for k, v in self.calibration_thresholds.items()},
         }
@@ -716,15 +716,15 @@
         metadata_fname = self.__make_metadata_fname(path)
         tf.io.write_file(metadata_fname, json.dumps(metadata))
 
         self.kv_store.save(path, compression=compression)
         self.search.save(path)
 
     @staticmethod
-    def load(path: Union[str, Path], verbose: int = 1):
+    def load(path: str | Path, verbose: int = 1):
         """Load Index data from a checkpoint and initialize underlying
         structure with the reloaded data.
 
         Args:
             path: Directory where the checkpoint is located.
             verbose: Be verbose. Defaults to 1.
 
@@ -733,21 +733,22 @@
         """
         path = str(path)
         # recreate the index from metadata
         metadata_fname = Indexer.__make_metadata_fname(path)
         metadata = tf.io.read_file(metadata_fname)
         metadata = tf.keras.backend.eval(metadata)
         md = json.loads(metadata)
+        search = make_search(md["search_config"])
         index = Indexer(
             distance=md["distance"],
             embedding_size=md["embedding_size"],
             embedding_output=md["embedding_output"],
             kv_store=md["kv_store"],
             evaluator=md["evaluator"],
-            search=md["search"],
+            search=search,
             stat_buffer_size=md["stat_buffer_size"],
         )
 
         # reload the key value store
         if verbose:
             print("Loading index data")
         index.kv_store.load(path)
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/layers.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Specialized Similarity `keras.layers`"""
+from __future__ import annotations
+
 import math
-from typing import Any, Dict, Optional
+from typing import Any
 
 import tensorflow as tf
 from tensorflow.keras import layers
 from tensorflow.python.keras.utils import conv_utils
 
 from .types import FloatTensor, IntTensor
 
@@ -33,15 +35,15 @@
     def call(self, inputs: FloatTensor) -> FloatTensor:
         x = super().call(inputs)
         normed_x: FloatTensor = tf.math.l2_normalize(x, axis=1)
         return normed_x
 
 
 class GeneralizedMeanPooling(layers.Layer):
-    def __init__(self, p: float = 3.0, data_format: Optional[str] = None, keepdims: bool = False, **kwargs) -> None:
+    def __init__(self, p: float = 3.0, data_format: str | None = None, keepdims: bool = False, **kwargs) -> None:
         super().__init__(**kwargs)
 
         self.p = p
         self.data_format = conv_utils.normalize_data_format(data_format)
         self.keepdims = keepdims
 
         if tf.math.abs(self.p) < 0.00001:
@@ -72,15 +74,15 @@
 
     def _pos_inf(self, x):
         raise NotImplementedError
 
     def _neg_inf(self, x):
         return self._pos_inf(x * -1) * -1
 
-    def get_config(self) -> Dict[str, Any]:
+    def get_config(self) -> dict[str, Any]:
         config = {
             "p": self.p,
             "data_format": self.data_format,
             "keepdims": self.keepdims,
         }
         base_config = super().get_config()
         return {**base_config, **config}
@@ -137,15 +139,15 @@
       - If `keepdims`=True:
         - If `data_format='channels_last'`:
           3D tensor with shape `(batch_size, 1, features)`
         - If `data_format='channels_first'`:
           3D tensor with shape `(batch_size, features, 1)`
     """
 
-    def __init__(self, p: float = 3.0, data_format: Optional[str] = None, keepdims: bool = False, **kwargs) -> None:
+    def __init__(self, p: float = 3.0, data_format: str | None = None, keepdims: bool = False, **kwargs) -> None:
         super().__init__(p=p, data_format=data_format, keepdims=keepdims, **kwargs)
 
         self.input_spec = layers.InputSpec(ndim=3)
         self.gap = layers.GlobalAveragePooling1D(data_format=data_format, keepdims=keepdims, **kwargs)
         self.step_axis = 1 if self.data_format == "channels_last" else 2
 
     def call(self, inputs: FloatTensor) -> FloatTensor:
@@ -223,15 +225,15 @@
       - If `keepdims`=True:
         - If `data_format='channels_last'`:
           3D tensor with shape `(batch_size, 1, features)`
         - If `data_format='channels_first'`:
           3D tensor with shape `(batch_size, features, 1)`
     """
 
-    def __init__(self, p: float = 3.0, data_format: Optional[str] = None, keepdims: bool = False, **kwargs) -> None:
+    def __init__(self, p: float = 3.0, data_format: str | None = None, keepdims: bool = False, **kwargs) -> None:
         super().__init__(p=p, data_format=data_format, keepdims=keepdims, **kwargs)
 
         self.input_spec = layers.InputSpec(ndim=4)
         self.gap = layers.GlobalAveragePooling2D(data_format=data_format, keepdims=keepdims, **kwargs)
 
     def call(self, inputs: FloatTensor) -> FloatTensor:
         x = inputs
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/losses/__init__.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/losses/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 """
 Contrastive learning specialized losses.
 """
 from .barlow import Barlow  # noqa
 from .circle_loss import CircleLoss  # noqa
 from .metric_loss import MetricLoss  # noqa
+from .multinegrank_loss import MultiNegativesRankLoss  # noqa
 from .multisim_loss import MultiSimilarityLoss  # noqa
 from .pn_loss import PNLoss  # noqa
 from .simclr import SimCLRLoss  # noqa
 from .simsiam import SimSiamLoss  # noqa
 from .softnn_loss import SoftNearestNeighborLoss  # noqa
 from .triplet_loss import TripletLoss  # noqa
 from .vicreg import VicReg  # noqa
+from .xbm_loss import XBM  # noqa
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/losses/barlow.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/losses/barlow.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Barlow Loss.
     Barlow Twins: Self-Supervised Learning via Redundancy Reduction
     https://arxiv.org/abs/2103.03230
 """
-from typing import Any, Callable, Dict, Optional
+from __future__ import annotations
+
+from collections.abc import Callable
+from typing import Any
 
 import tensorflow as tf
 
 from tensorflow_similarity.types import FloatTensor
 
 
 @tf.keras.utils.register_keras_serializable(package="Similarity")
@@ -48,16 +51,16 @@
     """
 
     def __init__(
         self,
         lambda_: float = 5e-3,
         margin: float = 1e-12,
         reduction: Callable = tf.keras.losses.Reduction.AUTO,
-        name: Optional[str] = None,
-        **kwargs
+        name: str | None = None,
+        **kwargs,
     ):
         super().__init__(reduction=reduction, name=name, **kwargs)
         self.lambda_ = lambda_
         self.margin = margin
 
     def call(self, za: FloatTensor, zb: FloatTensor) -> FloatTensor:
         """Compute the lost.
@@ -73,30 +76,30 @@
         batch_size = tf.shape(za)[0]
 
         za = self.standardize_columns(za)
         zb = self.standardize_columns(zb)
 
         # compute pairwise
         c = tf.matmul(za, zb, transpose_a=True)
-        c = c / tf.cast(batch_size, dtype="float32")
+        c = c / tf.cast(batch_size, dtype=c.dtype)
 
         on_diag = 1.0 - tf.linalg.diag_part(c)
         on_diag = tf.math.pow(on_diag, 2)
         on_diag = tf.math.reduce_sum(on_diag)
 
         off_diag = self.off_diagonal(c)
         off_diag = tf.math.pow(off_diag, 2)
         off_diag = tf.math.reduce_sum(off_diag)
 
         # 1D Tensor
         loss: FloatTensor = off_diag * self.lambda_ + on_diag + self.margin
 
         return loss
 
-    def get_config(self) -> Dict[str, Any]:
+    def get_config(self) -> dict[str, Any]:
         config = {
             "lambda_": self.lambda_,
             "margin": self.margin,
         }
         base_config = super().get_config()
         return {**base_config, **config}
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/losses/circle_loss.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/losses/circle_loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Circle Loss.
     [Circle Loss: A Unified Perspective of Pair Similarity Optimization](https://arxiv.org/abs/2002.10857)
 """
-from typing import Any, Callable, Union
+from __future__ import annotations
+
+from typing import Any
 
 import tensorflow as tf
 
 from tensorflow_similarity.algebra import build_masks
 from tensorflow_similarity.distances import Distance, distance_canonicalizer
 from tensorflow_similarity.types import FloatTensor, IntTensor
 
@@ -28,15 +30,15 @@
 
 
 def circle_loss(
     query_labels: IntTensor,
     query_embeddings: FloatTensor,
     key_labels: IntTensor,
     key_embeddings: FloatTensor,
-    distance: Callable,
+    distance: Distance,
     remove_diagonal: bool = True,
     gamma: float = 80,
     margin: float = 0.4,
 ) -> Any:
     """Circle loss computations.
 
     The original paper used cosine similarity while this loss has been modified
@@ -153,19 +155,19 @@
     you can use the layer `tensorflow_similarity.layers.L2Embedding()` as the
     last layer of your model to ensure your model output is properly
     normalized.
     """
 
     def __init__(
         self,
-        distance: Union[Distance, str] = "cosine",
+        distance: Distance | str = "cosine",
         gamma: float = 80.0,
         margin: float = 0.40,
         name: str = "CircleLoss",
-        **kwargs
+        **kwargs,
     ):
         """Initializes a CircleLoss
 
         Args:
             distance: Which distance function to use to compute the pairwise
             distances between embeddings. The distance is expected to be
             between [0, 2]. Defaults to 'cosine'.
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/losses/metric_loss.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/losses/metric_loss.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,28 +9,30 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Metric losses  base class."""
+from __future__ import annotations
 
-from typing import Any, Callable, Dict, Optional
+from collections.abc import Callable
+from typing import Any
 
 import tensorflow as tf
 
 from tensorflow_similarity.types import FloatTensor
 from tensorflow_similarity.utils import is_tensor_or_variable
 
 
 class MetricLoss(tf.keras.losses.Loss):
     """Wraps a loss function in the `Loss` class."""
 
     def __init__(
-        self, fn: Callable, reduction: Callable = tf.keras.losses.Reduction.AUTO, name: Optional[str] = None, **kwargs
+        self, fn: Callable, reduction: Callable = tf.keras.losses.Reduction.AUTO, name: str | None = None, **kwargs
     ):
         """Initializes `LossFunctionWrapper` class.
         Args:
           fn: The loss function to wrap, with signature `fn(y_true, y_pred,
             **kwargs)`.
           reduction: (Optional) Type of `tf.keras.losses.Reduction` to apply to
             loss. Default value is `AUTO`.
@@ -48,15 +50,15 @@
           y_pred: The predicted values.
         Returns:
           Loss values per sample.
         """
         loss: FloatTensor = self.fn(y_true, y_pred, y_true, y_pred, **self._fn_kwargs)
         return loss
 
-    def get_config(self) -> Dict[str, Any]:
+    def get_config(self) -> dict[str, Any]:
         """Contains the loss configuration.
 
         Returns:
             A Python dict containing the configuration of the loss.
         """
         config = {}
         for k, v in iter(self._fn_kwargs.items()):
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/losses/multisim_loss.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/losses/multisim_loss.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Multi Similarity Loss.
     Multi-Similarity Loss with General Pair Weighting for Deep Metric Learning
     https://arxiv.org/abs/1904.06627
 """
-from typing import Any, Callable, Union
+from __future__ import annotations
+
+from typing import Any
 
 import tensorflow as tf
 
 from tensorflow_similarity.algebra import build_masks, masked_max, masked_min
 from tensorflow_similarity.distances import Distance, distance_canonicalizer
 from tensorflow_similarity.types import FloatTensor, IntTensor
 
@@ -29,63 +31,53 @@
 
 
 def multisimilarity_loss(
     query_labels: IntTensor,
     query_embeddings: FloatTensor,
     key_labels: IntTensor,
     key_embeddings: FloatTensor,
-    distance: Callable,
+    distance: Distance,
     remove_diagonal: bool = True,
     alpha: float = 2.0,
     beta: float = 40,
     epsilon: float = 0.1,
     lmda: float = 0.5,
     center: float = 1.0,
 ) -> Any:
     """Multi Similarity loss computations.
 
     Args:
         query_labels: labels associated with the query embed.
-
         query_embeddings: Embedded query examples.
-
         key_labels: labels associated with the key embed.
-
         key_embeddings: Embedded key examples.
-
         distance: Which distance function to use to compute the pairwise.
-
-        remove_diagonal: Bool. If True, will set diagonal to False in positive pair mask
-
+        remove_diagonal: Bool. If True, will set diagonal to False in positive
+            pair mask
         alpha: The exponential weight for the positive pairs. Increasing alpha
-        makes the logsumexp softmax closer to the max positive pair distance,
-        while decreasing it makes it closer to max(P) + log(batch_size).
-
+            makes the logsumexp softmax closer to the max positive pair distance,
+            while decreasing it makes it closer to max(P) + log(batch_size).
         beta: The exponential weight for the negative pairs. Increasing beta
-        makes the logsumexp softmax closer to the max negative pair distance,
-        while decreasing it makes the softmax closer to
-        max(N) + log(batch_size).
-
+            makes the logsumexp softmax closer to the max negative pair distance,
+            while decreasing it makes the softmax closer to
+            max(N) + log(batch_size).
         epsilon: Used to remove easy positive and negative pairs. We only keep
-        positives that we greater than the (smallest negative pair - epsilon)
-        and we only keep negatives that are less than the
-        (largest positive pair + epsilon).
-
+            positives that we greater than the (smallest negative pair - epsilon)
+            and we only keep negatives that are less than the
+            (largest positive pair + epsilon).
         lmda: Used to weight the distance. Below this distance, negatives are
-        up weighted and positives are down weighted. Similarly, above this
-        distance negatives are down weighted and positive are up weighted.
-
+            up weighted and positives are down weighted. Similarly, above this
+            distance negatives are down weighted and positive are up weighted.
         center: This represents the expected distance value and will be used
-        to center the values in the pairwise distance matrix. This is used
-        when weighting the positive and negative examples, with the hardest
-        examples receiving an up weight and the easiest examples receiving a
-        down weight. This should 1 for cosine distances which we expect to
-        be between [0,2]. The value will depend on the data for L2 and L1
-        distances.
-
+            to center the values in the pairwise distance matrix. This is used
+            when weighting the positive and negative examples, with the hardest
+            examples receiving an up weight and the easiest examples receiving a
+            down weight. This should 1 for cosine distances which we expect to
+            be between [0,2]. The value will depend on the data for L2 and L1
+            distances.
 
     Returns:
         Loss: The loss value for the current batch.
     """
     # [Label]
     # ! Weirdness to be investigated
     # do not remove this code. It is actually needed for specific situation
@@ -122,33 +114,31 @@
     # Mark all pairs where we have both valid negative and positive pairs.
     valid_anchors = tf.math.logical_and(
         tf.math.reduce_any(pos_sim_p_mask, axis=1),
         tf.math.reduce_any(neg_sim_p_mask, axis=1),
     )
 
     # Cast masks as floats to support multiply
-    valid_anchors = tf.cast(valid_anchors, dtype="float32")
-    pos_sim_p_mask_f32 = tf.cast(pos_sim_p_mask, dtype="float32")
-    neg_sim_p_mask_f32 = tf.cast(neg_sim_p_mask, dtype="float32")
+    valid_anchors = tf.cast(valid_anchors, dtype=pairwise_distances.dtype)
+    pos_sim_p_mask = tf.cast(pos_sim_p_mask, dtype=pairwise_distances.dtype)
+    neg_sim_p_mask = tf.cast(neg_sim_p_mask, dtype=pairwise_distances.dtype)
 
     # [Weight the remaining pairs using Similarity-S and Similarity-N]
     shifted_distances = pairwise_distances + lmda - center
     pos_dists = alpha * shifted_distances
     neg_dists = -1 * beta * shifted_distances
 
     # [compute loss]
 
     # Positive pairs with a distance above 0 will be up weighted.
-    p_loss = logsumexp(pos_dists, pos_sim_p_mask_f32)
-    # p_loss = tf.math.log1p(tf.math.reduce_sum(tf.exp(pos_dists)*pos_sim_p_mask_f32, axis=1))
+    p_loss = logsumexp(pos_dists, pos_sim_p_mask)
     p_loss = p_loss / alpha
 
     # Negative pairs with a distance below 0 will be up weighted.
-    n_loss = logsumexp(neg_dists, neg_sim_p_mask_f32)
-    # n_loss = tf.math.log1p(tf.math.reduce_sum(tf.exp(neg_dists)*neg_sim_p_mask_f32, axis=1))
+    n_loss = logsumexp(neg_dists, neg_sim_p_mask)
     n_loss = n_loss / beta
 
     # Remove any anchors that have empty neg or pos pairs.
     # NOTE: reshape is required here because valid_anchors is [m] and
     #       p_loss + n_loss is [m, 1].
     multisim_loss = tf.math.multiply(p_loss + n_loss, tf.reshape(valid_anchors, (-1, 1)))
 
@@ -167,58 +157,58 @@
     you can use the layer `tensorflow_similarity.layers.L2Embedding()` as the
     last layer of your model to ensure your model output is properly
     normalized.
     """
 
     def __init__(
         self,
-        distance: Union[Distance, str] = "cosine",
+        distance: Distance | str = "cosine",
         alpha: float = 2.0,
         beta: float = 40.0,
         epsilon: float = 0.1,
         lmda: float = 0.5,
         center: float = 1.0,
         name: str = "MultiSimilarityLoss",
-        **kwargs
+        **kwargs,
     ):
         """Initializes the Multi Similarity Loss.
 
         Args:
             distance: Which distance function to use to compute the pairwise
-            distances between embeddings. Defaults to 'cosine'.
+                distances between embeddings. Defaults to 'cosine'.
 
             alpha: The exponential weight for the positive pairs. Increasing
-            alpha makes the logsumexp softmax closer to the max positive pair
-            distance, while decreasing it makes it closer to
-            max(P) + log(batch_size).
+                alpha makes the logsumexp softmax closer to the max positive
+                pair distance, while decreasing it makes it closer to
+                max(P) + log(batch_size).
 
             beta: The exponential weight for the negative pairs. Increasing
-            beta makes the logsumexp softmax closer to the max negative pair
-            distance, while decreasing it makes the softmax closer to
-            max(N) + log(batch_size).
+                beta makes the logsumexp softmax closer to the max negative
+                pair distance, while decreasing it makes the softmax closer
+                to max(N) + log(batch_size).
 
             epsilon: Used to remove easy positive and negative pairs. We only
-            keep positives that we greater than the (smallest negative pair -
-            epsilon) and we only keep negatives that are less than the
-            (largest positive pair + epsilon).
+                keep positives that we greater than the (smallest negative
+                pair - epsilon) and we only keep negatives that are less than
+                the (largest positive pair + epsilon).
 
             lmda: Used to weight the distance. Below this distance, negatives
-            are up weighted and positives are down weighted. Similarly, above
-            this distance negatives are down weighted and positive are up
-            weighted.
+                are up weighted and positives are down weighted. Similarly,
+                above this distance negatives are down weighted and positive
+                are up weighted.
 
             center: This represents the expected distance value and will be used
-            to center the values in the pairwise distance matrix. This is used
-            when weighting the positive and negative examples, with the hardest
-            examples receiving an up weight and the easiest examples receiving a
-            down weight. This should 1 for cosine distances which we expect to
-            be between [0,2]. The value will depend on the data for L2 and L1
-            distances.
+                to center the values in the pairwise distance matrix. This is
+                used when weighting the positive and negative examples, with the
+                hardest examples receiving an up weight and the easiest examples
+                receiving a down weight. This should 1 for cosine distances which
+                we expect to be between [0,2]. The value will depend on the data
+                for L2 and L1 distances.
 
-            name: Loss name. Defaults to MultiSimilarityLoss.
+            name: Loss name. Defaults to 'MultiSimilarityLoss'.
         """
 
         # distance canonicalization
         distance = distance_canonicalizer(distance)
         self.distance = distance
 
         super().__init__(
@@ -226,9 +216,9 @@
             name=name,
             distance=distance,
             alpha=alpha,
             beta=beta,
             epsilon=epsilon,
             lmda=lmda,
             center=center,
-            **kwargs
+            **kwargs,
         )
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/losses/pn_loss.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/losses/triplet_loss.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,73 +8,64 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""PN Loss foudn in Ivis.
-    Szubert, B., Cole, J.E., Monaco, C. et al.
-    Structure-preserving visualisation of high dimensional single-cell dataset
-    Sci Rep 9, 8914 (2019). https://doi.org/10.1038/s41598-019-45301-0
+"""Triplet Loss.
+    FaceNet: A Unified Embedding for Face Recognition and Clustering
+    https://arxiv.org/abs/1503.03832
 """
-from typing import Any, Callable, Union
+from __future__ import annotations
+
+from typing import Any
 
 import tensorflow as tf
 
 from tensorflow_similarity.algebra import build_masks
 from tensorflow_similarity.distances import Distance, distance_canonicalizer
 from tensorflow_similarity.types import FloatTensor, IntTensor
 
 from .metric_loss import MetricLoss
 from .utils import compute_loss, negative_distances, positive_distances
 
 
-def pn_loss(
+def triplet_loss(
     query_labels: IntTensor,
     query_embeddings: FloatTensor,
     key_labels: IntTensor,
     key_embeddings: FloatTensor,
-    distance: Callable,
+    distance: Distance,
     remove_diagonal: bool = True,
     positive_mining_strategy: str = "hard",
     negative_mining_strategy: str = "semi-hard",
-    soft_margin: bool = False,
-    margin: float = 1.0,
+    margin: float | None = None,
 ) -> Any:
-    """Positive Negative loss computations.
-
-    Based on the pn loss used in IVIS.
+    """Triplet loss computations.
 
     Args:
         query_labels: labels associated with the query embed.
-
         query_embeddings: Embedded query examples.
-
         key_labels: labels associated with the key embed.
-
         key_embeddings: Embedded key examples.
-
         distance: Which distance function to use to compute the pairwise
-        distances between embeddings. Defaults to 'cosine'.
-
-        remove_diagonal: Bool. If True, will set diagonal to False in positive pair mask
-
+            distances between embeddings.
+        remove_diagonal: If True, set the diagonal to False in positive pair
+            mask.
         positive_mining_strategy: What mining strategy to use to select
-        embedding from the same class. Defaults to 'hard'.
-        Available: {'easy', 'hard'}
-
+            embedding from the same class. {'easy', 'hard'}
         negative_mining_strategy: What mining strategy to use for select the
-        embedding from the different class. Defaults to 'semi-hard'.
-        Available: {'hard', 'semi-hard', 'easy'}
-
-        soft_margin: [description]. Defaults to True. Use a soft margin
-        instead of an explicit one.
-
-        margin: Use an explicit value for the margin term. Defaults to 1.0.
+            embedding from the different class. {'hard', 'semi-hard', 'easy'}
+        margin: Defines the target margin between positive and negative pairs,
+            e.g., a margin of 1.0 means that the positive and negative
+            distances should be 1.0 apart. If None, then a soft margin is used.
+            A soft margin can be beneficial to pull together samples from the
+            same class as much as possible. See the paper for more details
+            https://arxiv.org/pdf/1703.07737.pdf. Defaults to None.
 
     Returns:
         Loss: The loss value for the current batch.
     """
 
     # [Label]
     # ! Weirdness to be investigated
@@ -105,116 +96,86 @@
     neg_distances, neg_idxs = negative_distances(
         negative_mining_strategy,
         pairwise_distances,
         negative_mask,
         positive_mask,
     )
 
-    # Compute the distance between the pairs of positive and negative examples.
-    # Then take the min(pos_neg_dist, anchor_neg_dist) as the neg_distances.
-    # This encourages both the anchor and the positives to be far from the
-    # negative.
-    pn_pairs = tf.stack([pos_idxs, neg_idxs], axis=1)
-    pn_distances = tf.gather_nd(pairwise_distances, pn_pairs)
-    pn_distances = tf.reshape(pn_distances, [-1, 1])
-    neg_distances = tf.math.minimum(pn_distances, neg_distances)
+    # [Triplet loss computation]
+    triplet_loss = compute_loss(pos_distances, neg_distances, margin)
 
-    # [PN loss computation]
-    pn_loss = compute_loss(pos_distances, neg_distances, soft_margin, margin)
-
-    return pn_loss
+    return triplet_loss
 
 
 @tf.keras.utils.register_keras_serializable(package="Similarity")
-class PNLoss(MetricLoss):
-    """Computes the PN loss in an online fashion.
+class TripletLoss(MetricLoss):
+    """Computes the triplet loss in an online fashion.
 
     This loss encourages the positive distances between a pair of embeddings
     with the same labels to be smaller than the minimum negative distances
-    between pair of embeddings of different labels. Additionally, both the
-    anchor and the positive embeddings are encouraged to be far from the
-    negative embeddings. This is accomplished by taking the
-    min(pos_neg_dist, anchor_neg_dist) and using that as the negative distance
-    in the triplet loss.
-
-    See PN Loss Ivis:
-    Szubert, B., Cole, J.E., Monaco, C. et al.
-    Structure-preserving visualisation of high dimensional single-cell dataset
-    Sci Rep 9, 8914 (2019). https://doi.org/10.1038/s41598-019-45301-0
+    between pair of embeddings of different labels.
+    See: https://arxiv.org/abs/1503.03832 for the original paper.
+
 
     `y_true` must be  a 1-D integer `Tensor` of shape (batch_size,).
     It's values represent the classes associated with the examples as
     **integer  values**.
 
     `y_pred` must be 2-D float `Tensor`  of L2 normalized embedding vectors.
     you can use the layer `tensorflow_similarity.layers.L2Embedding()` as the
     last layer of your model to ensure your model output is properly
     normalized.
     """
 
     def __init__(
         self,
-        distance: Union[Distance, str] = "cosine",
+        distance: Distance | str = "cosine",
         positive_mining_strategy: str = "hard",
         negative_mining_strategy: str = "semi-hard",
-        soft_margin: bool = False,
-        margin: float = 1.0,
-        name: str = "PNLoss",
-        **kwargs
+        margin: float | None = None,
+        name: str = "TripletLoss",
+        **kwargs,
     ):
-        """Initializes the PN Loss.
+        """Initializes the TripletLoss.
 
         Args:
-            distance: Which distance function to use to compute
-            the pairwise distances between embeddings. Defaults to 'cosine'.
-
-            positive_mining_strategy: What mining strategy to
-            use to select embedding from the same class. Defaults to 'hard'.
-            available: {'easy', 'hard'}
-
-            negative_mining_strategy: What mining strategy to
-            use for select the embedding from the different class.
-            Defaults to 'semi-hard'. Available: {'hard', 'semi-hard', 'easy'}
-
-            soft_margin: [description]. Defaults to True.
-            Use a soft margin instead of an explicit one.
-
-            margin: Use an explicit value for the margin
-            term. Defaults to 1.0.
-
-            name: Loss name. Defaults to PNLoss.
+            distance: Which distance function to use to compute the pairwise
+                distances between embeddings.
+            remove_diagonal: If True, set the diagonal to False in positive pair
+                mask.
+            positive_mining_strategy: What mining strategy to use to select
+                embedding from the same class. {'easy', 'hard'}
+            negative_mining_strategy: What mining strategy to use for select the
+                embedding from the different class. {'hard', 'semi-hard', 'easy'}
+            margin: Defines the target margin between positive and negative pairs,
+                e.g., a margin of 1.0 means that the positive and negative
+                distances should be 1.0 apart. If None, then a soft margin is used.
+                A soft margin can be beneficial to pull together samples from the
+                same class as much as possible. See the paper for more details
+                https://arxiv.org/pdf/1703.07737.pdf. Defaults to None.
+            name: Loss name. Defaults to "TripletLoss".
 
         Raises:
             ValueError: Invalid positive mining strategy.
             ValueError: Invalid negative mining strategy.
-            ValueError: Margin value is not used when soft_margin is set
-                        to True.
         """
 
         # distance canonicalization
         distance = distance_canonicalizer(distance)
         self.distance = distance
-        # sanity checks
 
+        # sanity checks
         if positive_mining_strategy not in ["easy", "hard"]:
-            raise ValueError("Invalid positive mining strategy.")
+            raise ValueError("Invalid positive mining strategy")
 
         if negative_mining_strategy not in ["easy", "hard", "semi-hard"]:
-            raise ValueError("Invalid negative mining strategy.")
-
-        # Ensure users knows its one or the other
-        if margin != 1.0 and soft_margin:
-            raise ValueError(
-                "Margin value is not used when soft_margin is\
-                              set to True"
-            )
+            raise ValueError("Invalid negative mining strategy")
 
         super().__init__(
-            pn_loss,
+            triplet_loss,
             name=name,
             distance=distance,
             positive_mining_strategy=positive_mining_strategy,
             negative_mining_strategy=negative_mining_strategy,
-            soft_margin=soft_margin,
             margin=margin,
-            **kwargs
+            **kwargs,
         )
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/losses/simclr.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/losses/simclr.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """SimCLR Loss.
     A Simple Framework for Contrastive Learning of Visual Representations
     https://arxiv.org/abs/2002.05709
 """
-from typing import Any, Dict
+from __future__ import annotations
+
+from typing import Any
 
 import tensorflow as tf
 
 from tensorflow_similarity.types import FloatTensor
 
 
 @tf.keras.utils.register_keras_serializable(package="Similarity")
@@ -125,13 +127,13 @@
             ext_tensor = replica_context.all_reduce(tf.distribute.ReduceOp.SUM, ext_tensor)
 
             # Flatten the replica dimension.
             # The first dimension size will be: tensor.shape[0] * num_replicas
             # Using [-1] trick to support also scalar input.
             return tf.reshape(ext_tensor, [-1] + ext_tensor.shape.as_list()[2:])
 
-    def get_config(self) -> Dict[str, Any]:
+    def get_config(self) -> dict[str, Any]:
         config = {
             "temperature": self.temperature,
         }
         base_config = super().get_config()
         return {**base_config, **config}
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/losses/simsiam.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/losses/simsiam.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,29 +12,32 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """SimSiam Loss.
     Exploring Simple Siamese Representation Learning
     https://bit.ly/3LxsWdj
 """
+from __future__ import annotations
+
 import math
-from typing import Any, Callable, Dict, Optional
+from collections.abc import Callable
+from typing import Any
 
 import tensorflow as tf
 
 from tensorflow_similarity.types import FloatTensor
 
 
 def negative_cosine_sim(sim: FloatTensor) -> FloatTensor:
-    loss: FloatTensor = tf.constant([-1.0]) * sim
+    loss: FloatTensor = tf.math.multiply(tf.constant(-1.0, dtype=sim.dtype), sim)
     return loss
 
 
 def cosine_distance(sim: FloatTensor) -> FloatTensor:
-    loss: FloatTensor = tf.constant([1.0]) - sim
+    loss: FloatTensor = tf.math.subtract(tf.constant(1.0, dtype=sim.dtype), sim)
     return loss
 
 
 def angular_distance(sim: FloatTensor) -> FloatTensor:
     loss: FloatTensor = tf.math.acos(sim) / tf.constant(math.pi)
     return loss
 
@@ -47,15 +50,15 @@
     """
 
     def __init__(
         self,
         projection_type: str = "negative_cosine_sim",
         margin: float = 0.001,
         reduction: Callable = tf.keras.losses.Reduction.AUTO,
-        name: Optional[str] = None,
+        name: str | None = None,
         **kwargs,
     ):
         """Create the SimSiam Loss.
 
         Args:
           projection_type: Projects results into a metric space to allow KNN
           search.
@@ -106,14 +109,14 @@
         per_example_projection = self._projection(cosine_simlarity)
 
         # 1D tensor
         loss: FloatTensor = tf.math.multiply(per_example_projection, 0.5) + self.margin
 
         return loss
 
-    def get_config(self) -> Dict[str, Any]:
+    def get_config(self) -> dict[str, Any]:
         config = {
             "projection_type": self.projection_type,
             "margin": self.margin,
         }
         base_config = super().get_config()
         return {**base_config, **config}
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/losses/softnn_loss.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/losses/softnn_loss.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Soft Nearest Neighbors Loss.
     FaceNet: A Unified Embedding for Face Recognition and Clustering
     https://arxiv.org/abs/1902.01889
 """
-from typing import Any, Callable, Union
+from __future__ import annotations
+
+from typing import Any
 
 import tensorflow as tf
 
 from tensorflow_similarity.algebra import build_masks
 from tensorflow_similarity.distances import Distance, distance_canonicalizer
 from tensorflow_similarity.types import FloatTensor, IntTensor
 
@@ -28,64 +30,63 @@
 
 
 def soft_nn_loss(
     query_labels: IntTensor,
     query_embeddings: FloatTensor,
     key_labels: IntTensor,
     key_embeddings: FloatTensor,
-    distance: Callable,
+    distance: Distance,
     temperature: float,
     remove_diagonal: bool = True,
 ) -> Any:
     """Computes the soft nearest neighbors loss.
 
     Args:
         query_labels: labels associated with the query embed.
         query_embeddings: Embedded query examples.
         key_labels: labels associated with the key embed.
         key_embeddings: Embedded key examples.
         distance: Which distance function to use to compute the pairwise.
-        temperature: Controls relative importance given
-                        to the pair of points.
+        temperature: Controls relative importance given to the pair of points.
         remove_diagonal: Bool. If True, will set diagonal to False in positive pair mask
 
     Returns:
         loss: loss value for the current batch.
     """
 
     batch_size = tf.size(query_labels)
-    eps = 1e-9
+    eps = tf.cast(1e-9, dtype=query_embeddings.dtype)
 
     pairwise_dist = distance(query_embeddings, key_embeddings)
     pairwise_dist = pairwise_dist / temperature
     negexpd = tf.math.exp(-pairwise_dist)
 
     # Mask out diagonal entries
     diag = tf.linalg.diag(tf.ones(batch_size, dtype=tf.bool))
-    diag_mask = tf.cast(tf.logical_not(diag), dtype=tf.float32)
+    diag_mask = tf.cast(tf.logical_not(diag), dtype=query_embeddings.dtype)
     negexpd = tf.math.multiply(negexpd, diag_mask)
 
     # creating mask to sample same class neighboorhood
     pos_mask, _ = build_masks(
         query_labels,
         key_labels,
         batch_size=batch_size,
         remove_diagonal=remove_diagonal,
     )
-    pos_mask = tf.cast(pos_mask, dtype=tf.float32)
+    pos_mask = tf.cast(pos_mask, dtype=query_embeddings.dtype)
 
     # all class neighborhood
     alcn = tf.reduce_sum(negexpd, axis=1)
 
     # same class neighborhood
     sacn = tf.reduce_sum(tf.math.multiply(negexpd, pos_mask), axis=1)
 
     # exclude examples with unique class from loss calculation
     excl = tf.math.not_equal(tf.reduce_sum(pos_mask, axis=1), tf.zeros(batch_size))
-    excl = tf.cast(excl, tf.float32)
+    excl = tf.cast(excl, dtype=query_embeddings.dtype)
 
     loss = tf.math.divide(sacn, alcn)
     loss = -tf.multiply(tf.math.log(eps + loss), excl)
 
     return loss
 
 
@@ -103,18 +104,18 @@
     **integer  values**.
 
     `embeddings` must be 2-D float `Tensor` of embedding vectors.
     """
 
     def __init__(
         self,
-        distance: Union[Distance, str] = "sql2",
+        distance: Distance | str = "sql2",
         temperature: float = 1,
         name: str = "SoftNearestNeighborLoss",
-        **kwargs
+        **kwargs,
     ):
         """Initializes the SoftNearestNeighborLoss Loss
 
         Args:
             `distance`: Which distance function to use to compute
                         the pairwise distances between embeddings.
                         Defaults to 'sql2'.
@@ -125,8 +126,14 @@
             `name`: Loss name. Defaults to SoftNearestNeighborLoss.
         """
         # distance canonicalization
         distance = distance_canonicalizer(distance)
         self.distance = distance
         self.temperature = temperature
 
-        super().__init__(fn=soft_nn_loss, name=name, distance=distance, temperature=temperature, **kwargs)
+        super().__init__(
+            fn=soft_nn_loss,
+            name=name,
+            distance=distance,
+            temperature=temperature,
+            **kwargs,
+        )
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/losses/triplet_loss.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/losses/pn_loss.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,70 +8,67 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Triplet Loss.
-    FaceNet: A Unified Embedding for Face Recognition and Clustering
-    https://arxiv.org/abs/1503.03832
+"""PN Loss foudn in Ivis.
+    Szubert, B., Cole, J.E., Monaco, C. et al.
+    Structure-preserving visualisation of high dimensional single-cell dataset
+    Sci Rep 9, 8914 (2019). https://doi.org/10.1038/s41598-019-45301-0
 """
-from typing import Any, Callable, Union
+from __future__ import annotations
+
+from typing import Any
 
 import tensorflow as tf
 
 from tensorflow_similarity.algebra import build_masks
 from tensorflow_similarity.distances import Distance, distance_canonicalizer
 from tensorflow_similarity.types import FloatTensor, IntTensor
 
 from .metric_loss import MetricLoss
 from .utils import compute_loss, negative_distances, positive_distances
 
 
-def triplet_loss(
+def pn_loss(
     query_labels: IntTensor,
     query_embeddings: FloatTensor,
     key_labels: IntTensor,
     key_embeddings: FloatTensor,
-    distance: Callable,
+    distance: Distance,
     remove_diagonal: bool = True,
     positive_mining_strategy: str = "hard",
     negative_mining_strategy: str = "semi-hard",
-    soft_margin: bool = False,
-    margin: float = 1.0,
+    margin: float | None = None,
 ) -> Any:
-    """Triplet loss computations.
+    """Positive Negative loss computations.
+
+    Based on the pn loss used in IVIS.
 
     Args:
         query_labels: labels associated with the query embed.
-
         query_embeddings: Embedded query examples.
-
         key_labels: labels associated with the key embed.
-
         key_embeddings: Embedded key examples.
-
-        distance: Which distance function to use to compute the pairwise
-        distances between embeddings. Defaults to 'cosine'.
-
-        remove_diagonal: Bool. If True, will set diagonal to False in positive pair mask
-
+        distance: The distance function to use to compute the pairwise distances
+            between embeddings.
+        remove_diagonal: If True, set the diagonal to False in the positive pair
+            mask
         positive_mining_strategy: What mining strategy to use to select
-        embedding from the same class. Defaults to 'hard'.
-        Available: {'easy', 'hard'}
-
+            embedding from the same class. {'easy', 'hard'}
         negative_mining_strategy: What mining strategy to use for select the
-        embedding from the different class. Defaults to 'semi-hard'.
-        Available: {'hard', 'semi-hard', 'easy'}
-
-        soft_margin: [description]. Defaults to True. Use a soft margin
-        instead of an explicit one.
-
-        margin: Use an explicit value for the margin term. Defaults to 1.0.
+            embedding from the different class. {'hard', 'semi-hard', 'easy'}
+        margin: Defines the target margin between positive and negative pairs,
+            e.g., a margin of 1.0 means that the positive and negative
+            distances should be 1.0 apart. If None, then a soft margin is used.
+            A soft margin can be beneficial to pull together samples from the
+            same class as much as possible. See the paper for more details
+            https://arxiv.org/pdf/1703.07737.pdf. Defaults to None.
 
     Returns:
         Loss: The loss value for the current batch.
     """
 
     # [Label]
     # ! Weirdness to be investigated
@@ -102,100 +99,100 @@
     neg_distances, neg_idxs = negative_distances(
         negative_mining_strategy,
         pairwise_distances,
         negative_mask,
         positive_mask,
     )
 
-    # [Triplet loss computation]
-    triplet_loss = compute_loss(pos_distances, neg_distances, soft_margin, margin)
+    # Compute the distance between the pairs of positive and negative examples.
+    # Then take the min(pos_neg_dist, anchor_neg_dist) as the neg_distances.
+    # This encourages both the anchor and the positives to be far from the
+    # negative.
+    pn_pairs = tf.stack([pos_idxs, neg_idxs], axis=1)
+    pn_distances = tf.gather_nd(pairwise_distances, pn_pairs)
+    pn_distances = tf.reshape(pn_distances, [-1, 1])
+    neg_distances = tf.math.minimum(pn_distances, neg_distances)
 
-    return triplet_loss
+    # [PN loss computation]
+    pn_loss = compute_loss(pos_distances, neg_distances, margin)
+
+    return pn_loss
 
 
 @tf.keras.utils.register_keras_serializable(package="Similarity")
-class TripletLoss(MetricLoss):
-    """Computes the triplet loss in an online fashion.
+class PNLoss(MetricLoss):
+    """Computes the PN loss in an online fashion.
 
     This loss encourages the positive distances between a pair of embeddings
     with the same labels to be smaller than the minimum negative distances
-    between pair of embeddings of different labels.
-    See: https://arxiv.org/abs/1503.03832 for the original paper.
-
+    between pair of embeddings of different labels. Additionally, both the
+    anchor and the positive embeddings are encouraged to be far from the
+    negative embeddings. This is accomplished by taking the
+    min(pos_neg_dist, anchor_neg_dist) and using that as the negative distance
+    in the triplet loss.
+
+    See PN Loss Ivis:
+    Szubert, B., Cole, J.E., Monaco, C. et al.
+    Structure-preserving visualisation of high dimensional single-cell dataset
+    Sci Rep 9, 8914 (2019). https://doi.org/10.1038/s41598-019-45301-0
 
     `y_true` must be  a 1-D integer `Tensor` of shape (batch_size,).
     It's values represent the classes associated with the examples as
     **integer  values**.
 
     `y_pred` must be 2-D float `Tensor`  of L2 normalized embedding vectors.
     you can use the layer `tensorflow_similarity.layers.L2Embedding()` as the
     last layer of your model to ensure your model output is properly
     normalized.
     """
 
     def __init__(
         self,
-        distance: Union[Distance, str] = "cosine",
+        distance: Distance | str = "cosine",
         positive_mining_strategy: str = "hard",
         negative_mining_strategy: str = "semi-hard",
-        soft_margin: bool = False,
-        margin: float = 1.0,
-        name: str = "TripletLoss",
-        **kwargs
+        margin: float | None = None,
+        name: str = "PNLoss",
+        **kwargs,
     ):
-        """Initializes the TripletLoss.
+        """Initializes the PN Loss.
 
         Args:
-            distance: Which distance function to use to compute
-            the pairwise distances between embeddings. Defaults to 'cosine'.
-
-            positive_mining_strategy: What mining strategy to
-            use to select embedding from the same class. Defaults to 'hard'.
-            available: {'easy', 'hard'}
-
-            negative_mining_strategy: What mining strategy to
-            use for select the embedding from the different class.
-            Defaults to 'semi-hard'. Available: {'hard', 'semi-hard', 'easy'}
-
-            soft_margin: [description]. Defaults to True.
-            Use a soft margin instead of an explicit one.
-
-            margin: Use an explicit value for the margin
-            term. Defaults to 1.0.
-
-            name: Loss name. Defaults to TripletLoss.
+            distance: The distance function to use to compute the pairwise
+                distances between embeddings.
+            positive_mining_strategy: What mining strategy to use to select
+                embedding from the same class. {'easy', 'hard'}
+            negative_mining_strategy: What mining strategy to use for select the
+                embedding from the different class. {'hard', 'semi-hard', 'easy'}
+            margin: Defines the target margin between positive and negative pairs,
+                e.g., a margin of 1.0 means that the positive and negative
+                distances should be 1.0 apart. If None, then a soft margin is used.
+                A soft margin can be beneficial to pull together samples from the
+                same class as much as possible. See the paper for more details
+                https://arxiv.org/pdf/1703.07737.pdf. Defaults to None.
+            name: Loss name. Defaults to "PNLoss".
 
         Raises:
             ValueError: Invalid positive mining strategy.
             ValueError: Invalid negative mining strategy.
-            ValueError: Margin value is not used when soft_margin is set
-                        to True.
         """
 
         # distance canonicalization
         distance = distance_canonicalizer(distance)
         self.distance = distance
-        # sanity checks
 
+        # sanity checks
         if positive_mining_strategy not in ["easy", "hard"]:
-            raise ValueError("Invalid positive mining strategy")
+            raise ValueError("Invalid positive mining strategy.")
 
         if negative_mining_strategy not in ["easy", "hard", "semi-hard"]:
-            raise ValueError("Invalid negative mining strategy")
-
-        # Ensure users knows its one or the other
-        if margin != 1.0 and soft_margin:
-            raise ValueError(
-                "Margin value is not used when soft_margin is\
-                              set to True"
-            )
+            raise ValueError("Invalid negative mining strategy.")
 
         super().__init__(
-            triplet_loss,
+            pn_loss,
             name=name,
             distance=distance,
             positive_mining_strategy=positive_mining_strategy,
             negative_mining_strategy=negative_mining_strategy,
-            soft_margin=soft_margin,
             margin=margin,
-            **kwargs
+            **kwargs,
         )
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/losses/utils.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/losses/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Utility functions for computing the metric loss."""
-from typing import Any, Tuple
+from __future__ import annotations
+
+from typing import Any
 
 import tensorflow as tf
 
 from tensorflow_similarity.algebra import masked_max, masked_min
-from tensorflow_similarity.types import BoolTensor, FloatTensor
+from tensorflow_similarity.types import BoolTensor, FloatTensor, IntTensor
 
 
 def positive_distances(
     positive_mining_strategy: str,
     distances: FloatTensor,
     positive_mask: BoolTensor,
-) -> Tuple[FloatTensor, FloatTensor]:
+) -> tuple[FloatTensor, FloatTensor]:
     """Positive distance computation.
 
     Args:
         positive_mining_strategy (str, optional): [description].
         distances: 2-D float `Tensor` of [n, n] pairwise distances.
         positive_mask: 2-D Boolean `Tensor` of [n, n] valid distance size.
 
@@ -50,15 +52,15 @@
 
 
 def negative_distances(
     negative_mining_strategy: str,
     distances: FloatTensor,
     negative_mask: BoolTensor,
     positive_mask: BoolTensor,
-) -> Tuple[FloatTensor, FloatTensor]:
+) -> tuple[FloatTensor, FloatTensor]:
     """Negative distance computation.
 
     Args:
         negative_mining_strategy: What mining strategy to use for select the
         embedding from the different class.
         Available: {'hard', 'semi-hard', 'easy'}
 
@@ -77,64 +79,92 @@
       A Tuple of Tensors containing the negative distance values
       and the index for each example.
     """
     if negative_mining_strategy == "hard":
         # find the *non-zero* minimal distance between negative labels
         negative_distances, neg_idxs = masked_min(distances, negative_mask)
     elif negative_mining_strategy == "semi-hard":
-        # find the minimal distance between negative label gt than max distance
-        # between positive labels
+        # Find the negative label with the minimal distance that is greater
+        # than the maximal positive distance. If no such negative exists,
+        # i.e., max(d(a,n)) < max(d(a,p)), then use the maximal negative
+        # distance, as in the easy case.
+
         # find max value of positive distance
         max_positive, _ = masked_max(distances, positive_mask)
 
         # select distance that are above the max positive distance
         greater_distances = tf.math.greater(distances, max_positive)
 
-        # combine with negative mask: keep negative value if greater,
-        # zero otherwise
-        empty = tf.zeros_like(greater_distances, dtype=tf.bool)
-        semi_hard_mask = tf.where(greater_distances, negative_mask, empty)
+        # combine greater_distances with negative mask: keep negative
+        # value if greater, otherwise set to value from easy mask.
+        _, max_neg_idxs = masked_max(distances, negative_mask)
+        easy_mask = semi_hard_easy_mask(distances, max_neg_idxs)
+        semi_hard_mask = tf.where(greater_distances, negative_mask, easy_mask)
 
         # find the  minimal distance between negative labels above threshold
         negative_distances, neg_idxs = masked_min(distances, semi_hard_mask)
 
     elif negative_mining_strategy == "easy":
         # find the maximal distance between negative labels
         negative_distances, neg_idxs = masked_max(distances, negative_mask)
     else:
         raise ValueError("Invalid negative mining strategy")
 
     return negative_distances, neg_idxs
 
 
+def semi_hard_easy_mask(
+    distances: FloatTensor,
+    max_neg_idxs: IntTensor,
+) -> BoolTensor:
+    """Compute the fallback easy mask for semi-hard mining.
+
+    Find the negative label with the maximal distance that is less than or
+    equal to the maximal positive distance. This is used in the semi-hard
+    mining for the case when no negative label is found that is greater
+    than the maximal positive distance.
+    """
+    empty = tf.zeros_like(distances, dtype=tf.bool)
+    updates = tf.ones(tf.shape(max_neg_idxs)[0], dtype=tf.bool)
+    # tf.tensor_scatter_nd_update requires both the row and col idxs.
+    # here we use a range for the row idxs and take the max_neg_idxs as the cols.
+    row_idxs = tf.range(tf.shape(max_neg_idxs)[0])
+    col_idxs = tf.cast(max_neg_idxs, dtype=row_idxs.dtype)
+    indicies = tf.concat(
+        (tf.expand_dims(row_idxs, axis=-1), tf.expand_dims(col_idxs, axis=-1)),
+        axis=1,
+    )
+
+    # easy mask is a boolean tensor because we cast empty and updates to bool.
+    easy_mask: BoolTensor = tf.tensor_scatter_nd_update(empty, indicies, updates)
+
+    return easy_mask
+
+
 def compute_loss(
     positive_distances: FloatTensor,
     negative_distances: FloatTensor,
-    soft_margin: bool,
-    margin: float,
+    margin: float | None,
 ) -> Any:
     """Compute the final loss.
 
     Args:
         positive_distances: An [n,1] FloatTensor of positive distances.
 
         negative_distances: An [n,1] FloatTensor of negative distances.
 
-        soft_margin: [description]. Defaults to False.
-
-        margin: [description]. Defaults to 1.0.
+        margin: [description]. Use soft margin if None otherwise use explicit margin.
 
     Returns:
         An [n,1] FloatTensor containing the loss for each example.
     """
-
     loss = tf.math.subtract(positive_distances, negative_distances)
 
-    if soft_margin:
-        loss = tf.reduce_logsumexp(loss)
+    if margin is None:
+        loss = logsumexp(loss, tf.ones_like(loss))
     else:
         loss = tf.math.add(loss, margin)
         loss = tf.maximum(loss, 0.0)  # numeric stability
 
     return loss
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/losses/vicreg.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/losses/vicreg.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """VicReg Loss.
     VICReg: Variance-Invariance-Covariance Regularization for Self-Supervised Learning
     https://arxiv.org/abs/2105.04906
 """
-from typing import Any, Callable, Dict, Optional
+from __future__ import annotations
+
+from collections.abc import Callable
+from typing import Any
 
 import tensorflow as tf
 
 from tensorflow_similarity.types import FloatTensor
 
 
 @tf.keras.utils.register_keras_serializable(package="Similarity")
@@ -32,16 +35,16 @@
     def __init__(
         self,
         std_const: float = 1e-4,
         lambda_: float = 25,
         mu: float = 25,
         nu: float = 1,
         reduction: Callable = tf.keras.losses.Reduction.NONE,
-        name: Optional[str] = None,
-        **kwargs
+        name: str | None = None,
+        **kwargs,
     ):
         super().__init__(reduction=reduction, name=name, **kwargs)
         self.lambda_ = lambda_
         self.mu = mu
         self.nu = nu
         self.std_const = std_const
         self.reduction = reduction
@@ -79,15 +82,15 @@
         # covariance loss(1d tensor) for redundancy reduction
         cov_loss = off_diag_ca + off_diag_cb
 
         loss: FloatTensor = self.lambda_ * sim_loss + self.mu * std_loss + self.nu * cov_loss
 
         return loss
 
-    def get_config(self) -> Dict[str, Any]:
+    def get_config(self) -> dict[str, Any]:
         config = {
             "std_const": self.std_const,
             "lambda_": self.lambda_,
             "mu": self.mu,
             "nu": self.nu,
         }
         base_config = super().get_config()
@@ -99,22 +102,22 @@
         off_diagonals = tf.reshape(flattened, (n - 1, n + 1))[:, 1:]
         off_diag: FloatTensor = tf.reshape(off_diagonals, [-1])
         return off_diag
 
     def cov_loss_each(self, z, batch_size):
         # cross-correlation matrix axa
         c = tf.matmul(z, z, transpose_a=True)
-        c = c / tf.cast(batch_size - 1, dtype="float32")
+        c = c / tf.cast(batch_size - 1, dtype=c.dtype)
 
         num_features = tf.shape(c)[0]
 
         off_diag_c = self.off_diagonal(c)
         off_diag_c = tf.math.pow(off_diag_c, 2)
 
-        off_diag_c = tf.math.reduce_sum(off_diag_c) / tf.cast(num_features, tf.float32)
+        off_diag_c = tf.math.reduce_sum(off_diag_c) / tf.cast(num_features, dtype=c.dtype)
 
         return off_diag_c
 
     def mean_center_columns(self, x: FloatTensor) -> FloatTensor:
         col_mean = tf.math.reduce_mean(x, axis=0)
 
         norm_col: FloatTensor = x - col_mean
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/losses/xbm_loss.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/losses/xbm_loss.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/matchers/__init__.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/matchers/classification_match.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/matchers/classification_match.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 import math
 from abc import ABC, abstractmethod
-from typing import Optional, Tuple
 
 import tensorflow as tf
 
 from tensorflow_similarity.types import BoolTensor, FloatTensor, IntTensor
 
 
 class ClassificationMatch(ABC):
@@ -49,29 +49,29 @@
     def get_config(self):
         return {
             "name": str(self.name),
             "canonical_name": str(self.canonical_name),
             "distance_thresholds": self.distance_thresholds,
         }
 
-    def compile(self, distance_thresholds: Optional[FloatTensor] = None):
+    def compile(self, distance_thresholds: FloatTensor | None = None):
         """Configures the distance thresholds used during matching.
 
         Args:
             distance_thresholds: The max distance below which a nearest neighbor
             is considered a valid match. A threshold of math.inf is used if None
             is passed.
         """
         if distance_thresholds is None:
-            distance_thresholds = tf.constant([math.inf])
+            distance_thresholds = tf.constant([math.inf], dtype=tf.keras.backend.floatx())
 
-        self.distance_thresholds = tf.sort(tf.cast(distance_thresholds, dtype="float32"))
+        self.distance_thresholds = tf.sort(distance_thresholds)
 
     @abstractmethod
-    def derive_match(self, lookup_labels: IntTensor, lookup_distances: FloatTensor) -> Tuple[IntTensor, FloatTensor]:
+    def derive_match(self, lookup_labels: IntTensor, lookup_distances: FloatTensor) -> tuple[IntTensor, FloatTensor]:
         """Derive a match label and distance from a set of K neighbors.
 
         For each query, derive a single match label and distance given the
         associated set of lookup labels and distances.
 
         Args:
             lookup_labels: A 2D array where the jth row is the labels
@@ -89,15 +89,15 @@
                 derived_distances: A FloatTensor of shape
                 [len(lookup_labels), 1] where the jth row contains the distance
                 associated with the jth derived label.
         """
 
     def _compute_match_indicators(
         self, query_labels: IntTensor, lookup_labels: IntTensor, lookup_distances: FloatTensor
-    ) -> Tuple[BoolTensor, BoolTensor]:
+    ) -> tuple[BoolTensor, BoolTensor]:
         """Compute the match indicator tensor.
 
         Compute the match indicator tensor given a set of query labels and a
         set of associated lookup labels and distances.
 
         The method first calls `derive_match()` on the lookup labels and
         distances and then compares the query labels (y_true) against the
@@ -136,15 +136,15 @@
         if tf.rank(d_dist) == 1:
             d_dist = tf.expand_dims(d_dist, axis=-1)
 
         # A 1D BoolTensor [len(query_labels), 1]
         match_mask = tf.math.equal(d_labels, query_labels)
 
         # A 2D BoolTensor [len(lookup_distance), len(self.distance_thresholds)]
-        distance_mask = tf.math.less_equal(d_dist, self.distance_thresholds)
+        distance_mask = tf.math.less_equal(d_dist, tf.cast(self.distance_thresholds, dtype=d_dist.dtype))
 
         return match_mask, distance_mask
 
     def compute_count(self, query_labels: IntTensor, lookup_labels: IntTensor, lookup_distances: FloatTensor) -> None:
         """Computes the match counts at each of the distance thresholds.
 
         This method computes the following at each distance threshold.
@@ -179,27 +179,27 @@
         )
 
         self._compute_count(match_mask, distance_mask)
 
     def _compute_count(self, label_match: BoolTensor, dist_mask: BoolTensor) -> None:
         _tp = tf.math.logical_and(label_match, dist_mask)
         _tp = tf.math.count_nonzero(_tp, axis=0)
-        self._tp: FloatTensor = tf.cast(_tp, dtype="float")
+        self._tp: FloatTensor = tf.cast(_tp, dtype=tf.keras.backend.floatx())
 
         _fn = tf.math.logical_and(label_match, tf.math.logical_not(dist_mask))
         _fn = tf.math.count_nonzero(_fn, axis=0)
-        self._fn: FloatTensor = tf.cast(_fn, dtype="float")
+        self._fn: FloatTensor = tf.cast(_fn, dtype=tf.keras.backend.floatx())
 
         _fp = tf.math.logical_and(tf.math.logical_not(label_match), dist_mask)
         _fp = tf.math.count_nonzero(_fp, axis=0)
-        self._fp: FloatTensor = tf.cast(_fp, dtype="float")
+        self._fp: FloatTensor = tf.cast(_fp, dtype=tf.keras.backend.floatx())
 
         _tn = tf.math.logical_and(tf.math.logical_not(label_match), tf.math.logical_not(dist_mask))
         _tn = tf.math.count_nonzero(_tn, axis=0)
-        self._tn: FloatTensor = tf.cast(_tn, dtype="float")
+        self._tn: FloatTensor = tf.cast(_tn, dtype=tf.keras.backend.floatx())
 
         self._count = len(label_match)
 
     @property
     def tp(self) -> FloatTensor:
         """The count of True positive matches.
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/matchers/match_majority_vote.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/matchers/match_majority_vote.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from typing import Tuple
+from __future__ import annotations
 
 import tensorflow as tf
 
 from tensorflow_similarity.types import FloatTensor, IntTensor
 
 from .classification_match import ClassificationMatch
 
@@ -27,15 +26,15 @@
     def __init__(self, name: str = "majority_vote", **kwargs) -> None:
 
         if "canonical_name" not in kwargs:
             kwargs["canonical_name"] = "match_majority_vote"
 
         super().__init__(name=name, **kwargs)
 
-    def derive_match(self, lookup_labels: IntTensor, lookup_distances: FloatTensor) -> Tuple[IntTensor, FloatTensor]:
+    def derive_match(self, lookup_labels: IntTensor, lookup_distances: FloatTensor) -> tuple[IntTensor, FloatTensor]:
         """Derive a match label and distance from a set of K neighbors.
 
         For each query, derive a single match label and distance given the
         associated set of lookup labels and distances.
 
         Args:
             lookup_labels: A 2D array where the jth row is the labels
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/matchers/match_nearest.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/matchers/match_nearest.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from typing import Tuple
+from __future__ import annotations
 
 from tensorflow_similarity.types import FloatTensor, IntTensor
 
 from .classification_match import ClassificationMatch
 
 
 class MatchNearest(ClassificationMatch):
@@ -25,15 +24,15 @@
     def __init__(self, name: str = "nearest", **kwargs) -> None:
 
         if "canonical_name" not in kwargs:
             kwargs["canonical_name"] = "match_nearest"
 
         super().__init__(name=name, **kwargs)
 
-    def derive_match(self, lookup_labels: IntTensor, lookup_distances: FloatTensor) -> Tuple[IntTensor, FloatTensor]:
+    def derive_match(self, lookup_labels: IntTensor, lookup_distances: FloatTensor) -> tuple[IntTensor, FloatTensor]:
         """Derive a match label and distance from a set of K neighbors.
 
         For each query, derive a single match label and distance given the
         associated set of lookup labels and distances.
 
         Args:
             lookup_labels: A 2D array where the jth row is the labels
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/matchers/utils.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/matchers/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
-from typing import Dict, Type, Union
+from typing import Type
 
 from .classification_match import ClassificationMatch
 from .match_majority_vote import MatchMajorityVote
 from .match_nearest import MatchNearest
 
 
-def make_classification_matcher(matcher: Union[str, ClassificationMatch]) -> ClassificationMatch:
+def make_classification_matcher(matcher: str | ClassificationMatch) -> ClassificationMatch:
     """Convert classification matcher from str name to object if needed.
 
     Args:
         matcher: {'match_nearest', 'match_majority_vote'} or
         ClassificationMatch object. Defines the classification matching,
         e.g., match_nearest will count a True Positive if the query_label
         is equal to the label of the nearest neighbor and the distance is
@@ -32,15 +33,15 @@
     Raises:
         ValueError: matcher name is invalid.
 
     Returns:
         ClassificationMatch: Instantiated matcher if needed.
     """
     # ! Matcher must be non-instantiated.
-    MATCHER_ALIASES: Dict[str, Type[ClassificationMatch]] = {
+    MATCHER_ALIASES: dict[str, Type[ClassificationMatch]] = {
         "match_nearest": MatchNearest,
         "match_majority_vote": MatchMajorityVote,
     }
 
     if isinstance(matcher, str):
         if matcher.lower() in MATCHER_ALIASES:
             matcher = MATCHER_ALIASES[matcher.lower()]()
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/models/__init__.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/retrieval_metrics/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,13 +7,16 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Specialized `keras.model.Model` subclasses that offers additional
-functionalities to make training and serving similarity models quick and easy.
+"""Retrieval metrics measure the quality of the embedding space given a
+set query examples and a set of indexed examples. Informally it can be thought
+of as how well the space is clustered among other things.
 """
-
-from .contrastive_model import ContrastiveModel  # noqa
-from .similarity_model import SimilarityModel  # noqa
+from .bndcg import BNDCG  # noqa
+from .map_at_k import MapAtK  # noqa
+from .precision_at_k import PrecisionAtK  # noqa
+from .recall_at_k import RecallAtK  # noqa
+from .retrieval_metric import RetrievalMetric  # noqa
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/models/contrastive_model.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/models/contrastive_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-import itertools
-import json
-import os
+# Copyright 2021 The TensorFlow Authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+from __future__ import annotations
+
 from collections import defaultdict
+from collections.abc import Callable, Mapping, MutableMapping, MutableSequence, Sequence
 from copy import copy
 from pathlib import Path
-from typing import (
-    Callable,
-    DefaultDict,
-    Dict,
-    List,
-    Mapping,
-    MutableMapping,
-    MutableSequence,
-    Optional,
-    Sequence,
-    Tuple,
-    Union,
-)
+from typing import Any
 
 import numpy as np
 import tensorflow as tf
 from tabulate import tabulate
 from tensorflow.keras.losses import Loss
 from tensorflow.keras.metrics import Metric
 from tensorflow.keras.optimizers import Optimizer
@@ -30,14 +31,15 @@
 from tensorflow_similarity.classification_metrics import (  # noqa
     ClassificationMetric,
     make_classification_metric,
 )
 from tensorflow_similarity.distances import Distance, distance_canonicalizer
 from tensorflow_similarity.evaluators.evaluator import Evaluator
 from tensorflow_similarity.indexer import Indexer
+from tensorflow_similarity.layers import ActivationStdLoggingLayer
 from tensorflow_similarity.losses import MetricLoss
 from tensorflow_similarity.matchers import ClassificationMatch
 from tensorflow_similarity.retrieval_metrics import RetrievalMetric
 from tensorflow_similarity.search import Search
 from tensorflow_similarity.stores import Store
 from tensorflow_similarity.training_metrics import DistanceMetric
 from tensorflow_similarity.types import (
@@ -45,124 +47,156 @@
     FloatTensor,
     IntTensor,
     Lookup,
     PandasDataFrame,
     Tensor,
 )
 
+# Value based on implementation from original papers.
+BN_EPSILON = 1.001e-5
 
-class NumpyFloatValuesEncoder(json.JSONEncoder):
-    def default(self, obj):
-        if isinstance(obj, np.float32):
-            return float(obj)
-        return json.JSONEncoder.default(self, obj)
-
-
-def load_model(filepath):
-    spath = Path(filepath)
-    backbone_path = spath / "backbone"
-    proj_path = spath / "projector"
-    pred_path = spath / "predictor"
-    optw_path = spath / "opt_weights.npy"
-    config_path = spath / "config.json"
 
-    backbone = tf.keras.models.load_model(backbone_path)
-    projector = tf.keras.models.load_model(proj_path)
-
-    if os.path.isdir(pred_path):
-        predictor = tf.keras.models.load_model(pred_path)
+def get_projector(input_dim, dim=512, activation="relu", num_layers: int = 3):
+    inputs = tf.keras.layers.Input((input_dim,), name="projector_input")
+    x = inputs
+
+    for i in range(num_layers - 1):
+        x = tf.keras.layers.Dense(
+            dim,
+            use_bias=False,
+            kernel_initializer=tf.keras.initializers.LecunUniform(),
+            name=f"projector_layer_{i}",
+        )(x)
+        x = tf.keras.layers.BatchNormalization(epsilon=BN_EPSILON, name=f"batch_normalization_{i}")(x)
+        x = tf.keras.layers.Activation(activation, name=f"{activation}_activation_{i}")(x)
+    x = tf.keras.layers.Dense(
+        dim,
+        use_bias=False,
+        kernel_initializer=tf.keras.initializers.LecunUniform(),
+        name="projector_output",
+    )(x)
+    x = tf.keras.layers.BatchNormalization(
+        epsilon=BN_EPSILON,
+        center=False,  # Page:5, Paragraph:2 of SimSiam paper
+        scale=False,  # Page:5, Paragraph:2 of SimSiam paper
+        name="batch_normalization_ouput",
+    )(x)
+    # Metric Logging layer. Monitors the std of the layer activations.
+    # Degnerate solutions colapse to 0 while valid solutions will move
+    # towards something like 0.0220. The actual number will depend on the layer size.
+    outputs = ActivationStdLoggingLayer(name="proj_std")(x)
+    projector = tf.keras.Model(inputs, outputs, name="projector")
+    return projector
+
+
+def get_predictor(input_dim, hidden_dim=512, activation="relu"):
+    inputs = tf.keras.layers.Input(shape=(input_dim,), name="predictor_input")
+    x = inputs
+
+    x = tf.keras.layers.Dense(
+        hidden_dim,
+        use_bias=False,
+        kernel_initializer=tf.keras.initializers.LecunUniform(),
+        name="predictor_layer_0",
+    )(x)
+    x = tf.keras.layers.BatchNormalization(epsilon=BN_EPSILON, name="batch_normalization_0")(x)
+    x = tf.keras.layers.Activation(activation, name=f"{activation}_activation_0")(x)
+
+    x = tf.keras.layers.Dense(
+        input_dim,
+        kernel_initializer=tf.keras.initializers.LecunUniform(),
+        name="predictor_output",
+    )(x)
+    # Metric Logging layer. Monitors the std of the layer activations.
+    # Degnerate solutions colapse to 0 while valid solutions will move
+    # towards something like 0.0220. The actual number will depend on the layer size.
+    outputs = ActivationStdLoggingLayer(name="pred_std")(x)
+    predictor = tf.keras.Model(inputs, outputs, name="predictor")
+    return predictor
+
+
+def create_contrastive_model(
+    *args,
+    backbone: tf.keras.Model,
+    projector: tf.keras.Model | None = None,
+    predictor: tf.keras.Model | None = None,
+    algorithm: str = "simsiam",
+    **kwargs,
+) -> ContrastiveModel:
+    """Create a contrastive model."""
+    if projector is None:
+        projector = get_projector(input_dim=backbone.output_shape[-1], num_layers=2)
+
+    input_shape = backbone.input_shape[1:]
+    inputs = tf.keras.layers.Input(shape=input_shape, name="main_model_input")
+    projector_features = projector(backbone(inputs))
+    if algorithm == "simsiam":
+        if predictor is None:
+            predictor = get_predictor(input_dim=projector.output_shape[-1])
+        predictor_features = predictor(projector_features)
     else:
-        predictor = None
+        predictor_features = None
 
-    with open(config_path, "r") as f:
-        config = json.load(f)
-        metadata = json.loads(config)
-
-    optimizer = tf.keras.optimizers.deserialize(metadata["optimizer"])
-    opt_weights = np.load(optw_path, allow_pickle=True)
-    loss = tf.keras.losses.deserialize(metadata["loss"])
-    metrics = [tf.keras.metrics.deserialize(m) for m in metadata["metrics"]]
-    algorithm = metadata["algorithm"]
+    outputs = [projector_features]
+    if predictor_features is not None:
+        outputs.append(predictor_features)
 
-    model = ContrastiveModel(
+    return ContrastiveModel(
+        *args,
         backbone=backbone,
         projector=projector,
         predictor=predictor,
         algorithm=algorithm,
+        inputs=inputs,
+        outputs=outputs,
+        **kwargs,
     )
 
-    model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
-
-    def load_optim_weights():
-        # collect train variables from both the backbone, projector, and projector
-        tvars = model.backbone.trainable_variables
-        tvars = tvars + model.projector.trainable_variables
-        if model.predictor is not None:
-            tvars = tvars + model.predictor.trainable_variables
-
-        # dummy zero gradients
-        zero_grads = [tf.zeros_like(w) for w in tvars]
-        # save current state of variables
-        saved_vars = [tf.identity(w) for w in tvars]
-
-        model.optimizer.apply_gradients(zip(zero_grads, tvars))
-
-        # Reload variables
-        [x.assign(y) for x, y in zip(tvars, saved_vars)]
-
-        model.optimizer.set_weights(opt_weights)
-
-    strategy = tf.distribute.get_strategy()
-    strategy.run(load_optim_weights)
-    return model
-
 
 @tf.keras.utils.register_keras_serializable(package="Similarity")
 class ContrastiveModel(tf.keras.Model):
     def __init__(
         self,
+        *args,
         backbone: tf.keras.Model,
         projector: tf.keras.Model,
-        predictor: Optional[tf.keras.Model] = None,
+        predictor: tf.keras.Model | None = None,
         algorithm: str = "simsiam",
         **kwargs,
     ) -> None:
-        super().__init__(**kwargs)
+        super().__init__(*args, **kwargs)
         self.backbone = backbone
         self.projector = projector
         self.predictor = predictor
 
-        self.outputs = [self.backbone.output]
-        self.output_names = ["backbone_output"]
         self.algorithm = algorithm
 
         self._create_loss_trackers()
 
-        self.supported_algorithms = ("simsiam", "simclr", "barlow")
+        self.supported_algorithms = ("simsiam", "simclr", "barlow", "vicreg")
 
         if self.algorithm not in self.supported_algorithms:
             raise ValueError(
                 f"{self.algorithm} is not a supported algorithm."
                 f"Supported algorithms are {self.supported_algorithms}."
             )
 
     def compile(
         self,
-        optimizer: Union[Optimizer, str, Dict, List] = "rmsprop",
-        loss: Optional[Union[Loss, MetricLoss, str, Dict, List]] = None,
-        metrics: Optional[Union[Metric, DistanceMetric, str, Dict, List]] = None,  # noqa
-        loss_weights: Optional[Union[List, Dict]] = None,
-        weighted_metrics: Optional[Union[Metric, DistanceMetric, str, Dict, List]] = None,  # noqa
+        optimizer: Optimizer | str | Mapping | Sequence = "rmsprop",
+        loss: Loss | MetricLoss | str | Mapping | Sequence | None = None,
+        metrics: Metric | DistanceMetric | str | Mapping | Sequence | None = None,  # noqa
+        loss_weights: Mapping | Sequence | None = None,
+        weighted_metrics: Metric | DistanceMetric | str | Mapping | Sequence | None = None,  # noqa
         run_eagerly: bool = False,
         steps_per_execution: int = 1,
-        distance: Union[Distance, str] = "cosine",
-        embedding_output: Optional[int] = None,
-        kv_store: Union[Store, str] = "memory",
-        search: Union[Search, str] = "nmslib",
-        evaluator: Union[Evaluator, str] = "memory",
+        distance: Distance | str = "cosine",
+        kv_store: Store | str = "memory",
+        search: Search | str = "nmslib",
+        evaluator: Evaluator | str = "memory",
         stat_buffer_size: int = 1000,
         **kwargs,
     ):
         """Configures the model for training.
 
         Args:
             optimizer: String (name of optimizer) or optimizer instance. See
@@ -188,23 +222,14 @@
               For technical and performance reasons, indexing data at each
               training batch to compute those is impractical so those metrics are
               computed at epoch end via the [EvalCallback](../callbacks.md)
 
               See [Evaluation Metrics](../eval_metrics.md) for a list of available
               metrics.
 
-              For multi-output models you can specify different metrics for
-              different outputs by passing a dictionary, such as
-              `metrics={'similarity': 'min_neg_gap', 'other': ['accuracy',
-              'mse']}`.  You can also pass a list (len = len(outputs)) of lists of
-              metrics such as `metrics=[['min_neg_gap'], ['accuracy', 'mse']]` or
-              `metrics=['min_neg_gap', ['accuracy', 'mse']]`. For outputs which
-              are not related to metrics learning, you can use any of the standard
-              `tf.keras.metrics`.
-
             loss_weights: Optional list or dictionary specifying scalar
               coefficients (Python floats) to weight the loss contributions of
               different model outputs. The loss value that will be minimized by
               the model will then be the *weighted sum* of all individual losses,
               weighted by the `loss_weights` coefficients.  If a list, it is
               expected to have a 1:1 mapping to the model's outputs. If a dict, it
               is expected to map output names (strings) to scalar coefficients.
@@ -235,20 +260,14 @@
 
             search: Which `Search()` framework to use to perform KNN search.
               Defaults to 'nmslib'.
 
             evaluator: What type of `Evaluator()` to use to evaluate index
               performance. Defaults to in-memory one.
 
-            embedding_output: Which model output head predicts the embeddings
-            that should be indexed. Defaults to None which is for single output
-            model. For multi-head model, the callee, usually the
-            `SimilarityModel()` class is responsible for passing the correct
-            one.
-
             stat_buffer_size: Size of the sliding windows buffer used to compute
               index performance. Defaults to 1000.
 
         Raises:
             ValueError: In case of invalid arguments for
                 `optimizer`, `loss` or `metrics`.
         """
@@ -256,15 +275,14 @@
 
         # init index
         self.create_index(
             distance=distance_obj,
             search=search,
             kv_store=kv_store,
             evaluator=evaluator,
-            embedding_output=embedding_output,
             stat_buffer_size=stat_buffer_size,
         )
 
         # call underlying keras method
         super().compile(
             optimizer=optimizer,
             loss=loss,
@@ -289,16 +307,17 @@
             self.loss_trackers["regularization_loss"] = tf.keras.metrics.Mean(name="regularization_loss")
 
     @property
     def metrics(self):
         # We remove the compiled loss metric because we want to manually track
         # the loss in train_step and test_step.
         base_metrics = [m for m in super().metrics if m.name != "loss"]
-        loss_trackers = self.loss_trackers.values()
-        return itertools.chain(loss_trackers, base_metrics)
+        loss_trackers = list(self.loss_trackers.values())
+        loss_trackers.extend(base_metrics)
+        return loss_trackers
 
     def train_step(self, data):
         view1, view2 = self._parse_views(data)
 
         # Forward pass through the backbone, projector, and predictor
         with tf.GradientTape() as tape:
             contrastive_loss, pred1, pred2, z1, z2 = self._forward_pass(view1, view2, training=True)
@@ -385,156 +404,49 @@
         if self.algorithm == "simsiam":
             p1 = self.predictor(z1, training=training)
             p2 = self.predictor(z2, training=training)
             l1 = self.compiled_loss(tf.stop_gradient(z1), p2)
             l2 = self.compiled_loss(tf.stop_gradient(z2), p1)
             loss = l1 + l2
             pred1, pred2 = p1, p2
-        elif self.algorithm in ["simclr", "barlow"]:
+        elif self.algorithm in ("simclr", "barlow", "vicreg"):
             loss = self.compiled_loss(z1, z2)
             pred1, pred2 = z1, z2
 
         return loss, pred1, pred2, z1, z2
 
-    def _parse_views(self, data: Sequence[FloatTensor]) -> Tuple[FloatTensor, FloatTensor]:
+    def _parse_views(self, data: Sequence[FloatTensor]) -> tuple[FloatTensor, FloatTensor]:
         if len(data) == 2:
-            view1 = data[0]
-            view2 = data[1]
+            view1, view2 = data
         else:
-            view1 = data[0]
-            view2 = data[0]
+            view1 = view2 = data[0]
 
         return view1, view2
 
     # fix TF 2.x < 2.7 bugs when using generator
-    def call(self, inputs):
+    # todo(ovallis): link to original issue.
+    def call(self, inputs, training=None, mask=None):
         return inputs
 
     def summary(self):
         cprint("[Backbone]", "green")
         self.backbone.summary()
         cprint("\n[Projector]", "magenta")
         self.projector.summary()
         if self.predictor is not None:
             cprint("\n[Predictor]", "magenta")
             self.projector.summary()
 
-    def save(
-        self,
-        filepath: Union[str, Path],
-        save_index: bool = True,
-        compression: bool = True,
-        overwrite: bool = True,
-        include_optimizer: bool = True,
-        save_format: Optional[str] = None,
-        signatures: Optional[Union[Callable, Mapping[str, Callable]]] = None,
-        options: Optional[tf.saved_model.SaveOptions] = None,
-        save_traces: bool = True,
-    ) -> None:
-        """Save Constrative model backbone, projector, and predictor
-
-        Args:
-            filepath: where to save the model.
-            save_index: Save the index content. Defaults to True.
-            compression: Compress index data. Defaults to True.
-            overwrite: Overwrite previous model. Defaults to True.
-            include_optimizer: Save optimizer state. Defaults to True.
-            save_format: Either 'tf' or 'h5', indicating whether to save the
-              model to Tensorflow SavedModel or HDF5. Defaults to 'tf' in
-              TF 2.X, and 'h5' in TF 1.X.
-            signatures: Signatures to save with the SavedModel. Applicable to
-              the 'tf' format only. Please see the signatures argument in
-              tf.saved_model.save for details.
-            options: A `tf.saved_model.SaveOptions` to save with the model.
-              Defaults to None.
-            save_traces (optional): When enabled, the SavedModel will store the
-              function traces for each layer. This can be disabled, so that only
-              the configs of each layer are stored.  Defaults to True. Disabling
-              this will decrease serialization time and reduce file size, but it
-              requires that all custom layers/models implement a get_config()
-              method.
-        """
-        spath = Path(filepath)
-        backbone_path = spath / "backbone"
-        proj_path = spath / "projector"
-        pred_path = spath / "predictor"
-        optw_path = spath / "opt_weights.npy"
-        config_path = spath / "config.json"
-
-        cprint("[Saving backbone model]", "blue")
-        cprint("|-path:%s" % backbone_path, "green")
-        self.backbone.save(
-            backbone_path,
-            overwrite=overwrite,
-            include_optimizer=include_optimizer,
-            save_format=save_format,
-            signatures=signatures,
-            options=options,
-            save_traces=save_traces,
-        )
-
-        cprint("[Saving projector model]", "blue")
-        cprint("|-path:%s" % proj_path, "green")
-        self.projector.save(
-            proj_path,
-            overwrite=overwrite,
-            include_optimizer=include_optimizer,
-            save_format=save_format,
-            signatures=signatures,
-            options=options,
-            save_traces=save_traces,
-        )
-
-        if self.predictor is not None:
-            cprint("[Saving predictor model]", "blue")
-            cprint("|-path:%s" % pred_path, "green")
-            self.predictor.save(
-                pred_path,
-                overwrite=overwrite,
-                include_optimizer=include_optimizer,
-                save_format=save_format,
-                signatures=signatures,
-                options=options,
-                save_traces=save_traces,
-            )
-
-        metadata = {}
-        base_metrics = [m for m in super().metrics if m.name != "loss"]
-        metadata["metrics"] = [tf.keras.metrics.serialize(m) for m in base_metrics]
-        metadata["loss"] = tf.keras.losses.serialize(self.loss)
-        metadata["optimizer"] = tf.keras.optimizers.serialize(self.optimizer)
-        np.save(optw_path, self.optimizer.get_weights())
-
-        with open(config_path, "w") as f:
-            base_config = self.get_config()
-            config = json.dumps({**metadata, **base_config}, cls=NumpyFloatValuesEncoder)
-            json.dump(config, f)
-
-        if hasattr(self, "_index") and self._index and save_index:
-            self.save_index(filepath, compression=compression)
-        else:
-            print("Index not saved as save_index=False")
-
-    def get_config(self):
-        config = {
-            "algorithm": self.algorithm,
-        }
-        return config
-
-    # TODO(ovallis): Overwrite load
-
-    # TODO(ovallis): Overwrite summary to show the whole model.
-
     def predict(
         self,
         x: FloatTensor,
-        batch_size: Optional[int] = None,
+        batch_size: int | None = None,
         verbose: int = 0,
-        steps: Optional[int] = None,
-        callbacks: Optional[tf.keras.callbacks.Callback] = None,
+        steps: int | None = None,
+        callbacks: tf.keras.callbacks.Callback | None = None,
         max_queue_size: int = 10,
         workers: int = 1,
         use_multiprocessing: bool = False,
     ) -> FloatTensor:
         """Generates output predictions for the input samples.
 
         The predict returns the L2 normalized output of the projector.
@@ -548,15 +460,14 @@
             verbose,
             steps,
             callbacks,
             max_queue_size,
             workers,
             use_multiprocessing,
         )
-
         x = self.projector.predict(
             x,
             batch_size,
             verbose,
             steps,
             callbacks,
             max_queue_size,
@@ -564,23 +475,20 @@
             use_multiprocessing,
         )
 
         output: FloatTensor = tf.math.l2_normalize(x, axis=1)
 
         return output
 
-    # TODO (ovallis): Refactor the following indexing code into a MixIn.
-
     def create_index(
         self,
-        distance: Union[Distance, str] = "cosine",
-        search: Union[Search, str] = "nmslib",
-        kv_store: Union[Store, str] = "memory",
-        evaluator: Union[Evaluator, str] = "memory",
-        embedding_output: Optional[int] = None,
+        distance: Distance | str = "cosine",
+        search: Search | str = "nmslib",
+        kv_store: Store | str = "memory",
+        evaluator: Evaluator | str = "memory",
         stat_buffer_size: int = 1000,
     ) -> None:
         """Create the model index to make embeddings searchable via KNN.
 
         This method is normally called as part of `SimilarityModel.compile()`.
         However, this method is provided if users want to define a custom index
         outside of the `compile()` method.
@@ -596,59 +504,35 @@
 
             search: Which `Search()` framework to use to perform KNN search.
             Defaults to 'nmslib'.
 
             evaluator: What type of `Evaluator()` to use to evaluate index
             performance. Defaults to in-memory one.
 
-            embedding_output: Which model output head predicts the embeddings
-            that should be indexed. Defaults to None which is for single output
-            model. For multi-head model, the callee, usually the
-            `SimilarityModel()` class is responsible for passing the correct
-            one.
-
             stat_buffer_size: Size of the sliding windows buffer used to compute
             index performance. Defaults to 1000.
 
         Raises:
             ValueError: Invalid search framework or key value store.
         """
-        # check if we we need to set the embedding head
-        num_outputs = len(self.output_names)
-        if embedding_output is not None and embedding_output > num_outputs:
-            raise ValueError("Embedding_output value exceed number of model outputs")
-
-        if embedding_output is None and num_outputs > 1:
-            print(
-                "Embedding output set to be model output 0. ",
-                "Use the embedding_output arg to override this.",
-            )
-            embedding_output = 0
-
-        # fetch embedding size as some ANN libs requires it for init
-        if num_outputs > 1 and embedding_output is not None:
-            self.embedding_size = self.outputs[embedding_output].shape[1]
-        else:
-            self.embedding_size = self.outputs[0].shape[1]
-
         self._index = Indexer(
-            embedding_size=self.embedding_size,
+            embedding_size=self.projector.output_shape[-1],
             distance=distance,
             search=search,
             kv_store=kv_store,
             evaluator=evaluator,
-            embedding_output=embedding_output,
+            embedding_output=None,
             stat_buffer_size=stat_buffer_size,
         )
 
     def index(
         self,
         x: Tensor,
-        y: IntTensor = None,
-        data: Optional[Tensor] = None,
+        y: IntTensor | None = None,
+        data: Tensor | None = None,
         build: bool = True,
         verbose: int = 1,
     ):
         """Index data.
 
         Args:
             x: Samples to index.
@@ -680,16 +564,16 @@
             build=build,
             verbose=verbose,
         )
 
     def index_single(
         self,
         x: Tensor,
-        y: IntTensor = None,
-        data: Optional[Tensor] = None,
+        y: IntTensor | None = None,
+        data: Tensor | None = None,
         build: bool = True,
         verbose: int = 1,
     ):
         """Index data.
 
         Args:
             x: Sample to index.
@@ -719,42 +603,42 @@
             prediction=prediction,
             label=y,
             data=data,
             build=build,
             verbose=verbose,
         )
 
-    def lookup(self, x: Tensor, k: int = 5, verbose: int = 1) -> List[List[Lookup]]:
+    def lookup(self, x: Tensor, k: int = 5, verbose: int = 1) -> list[list[Lookup]]:
         """Find the k closest matches in the index for a set of samples.
 
         Args:
             x: Samples to match.
 
             k: Number of nearest neighboors to lookup. Defaults to 5.
 
             verbose: display progress. Default to 1.
 
         Returns
             list of list of k nearest neighboors:
-            List[List[Lookup]]
+            list[list[Lookup]]
         """
         predictions = self.predict(x)
         return self._index.batch_lookup(predictions=predictions, k=k, verbose=verbose)
 
-    def single_lookup(self, x: Tensor, k: int = 5) -> List[Lookup]:
+    def single_lookup(self, x: Tensor, k: int = 5) -> list[Lookup]:
         """Find the k closest matches in the index for a given sample.
 
         Args:
             x: Sample to match.
 
             k: Number of nearest neighboors to lookup. Defaults to 5.
 
         Returns
             list of the k nearest neigboors info:
-            List[Lookup]
+            list[Lookup]
         """
         x = tf.expand_dims(x, axis=0)
         prediction = self.predict(x)
         return self._index.single_lookup(prediction=prediction, k=k)
 
     def index_summary(self):
         "Display index info summary."
@@ -762,17 +646,17 @@
 
     def calibrate(
         self,
         x: FloatTensor,
         y: IntTensor,
         thresholds_targets: MutableMapping[str, float] = {},
         k: int = 1,
-        calibration_metric: Union[str, ClassificationMetric] = "f1",
-        matcher: Union[str, ClassificationMatch] = "match_nearest",
-        extra_metrics: MutableSequence[Union[str, ClassificationMetric]] = [
+        calibration_metric: str | ClassificationMetric = "f1",
+        matcher: str | ClassificationMatch = "match_nearest",
+        extra_metrics: MutableSequence[str | ClassificationMetric] = [
             "precision",
             "recall",
         ],  # noqa
         rounding: int = 2,
         verbose: int = 1,
     ) -> CalibrationResults:
         """Calibrate model thresholds using a test dataset.
@@ -834,15 +718,15 @@
 
     def match(
         self,
         x: FloatTensor,
         cutpoint="optimal",
         no_match_label=-1,
         k=1,
-        matcher: Union[str, ClassificationMatch] = "match_nearest",
+        matcher: str | ClassificationMatch = "match_nearest",
         verbose=0,
     ):
         """Match a set of examples against the calibrated index
 
         For the match function to work, the index must be calibrated using
         calibrate().
 
@@ -900,15 +784,15 @@
 
     def evaluate_retrieval(
         self,
         x: Tensor,
         y: IntTensor,
         retrieval_metrics: Sequence[RetrievalMetric],  # noqa
         verbose: int = 1,
-    ) -> Dict[str, np.ndarray]:
+    ) -> dict[str, np.ndarray]:
         """Evaluate the quality of the index against a test dataset.
 
         Args:
             x: Examples to be matched against the index.
 
             y: Label associated with the examples supplied.
 
@@ -952,21 +836,21 @@
         return results
 
     def evaluate_classification(
         self,
         x: Tensor,
         y: IntTensor,
         k: int = 1,
-        extra_metrics: MutableSequence[Union[str, ClassificationMetric]] = [
+        extra_metrics: MutableSequence[str | ClassificationMetric] = [
             "precision",
             "recall",
         ],  # noqa
-        matcher: Union[str, ClassificationMatch] = "match_nearest",
+        matcher: str | ClassificationMatch = "match_nearest",
         verbose: int = 1,
-    ) -> DefaultDict[str, Dict[str, Union[str, np.ndarray]]]:
+    ) -> defaultdict[str, dict[str, str | np.ndarray]]:
         """Evaluate model classification matching on a given evaluation dataset.
 
         Args:
             x: Examples to be matched against the index.
 
             y: Label associated with the examples supplied.
 
@@ -1004,27 +888,27 @@
         cal_metric = self._index.get_calibration_metric()
 
         # get embeddings
         if verbose:
             print("|-Computing embeddings")
         predictions = self.predict(x)
 
-        results: DefaultDict[str, Dict[str, Union[str, np.ndarray]]] = defaultdict(dict)
+        results: defaultdict[str, dict[str, str | np.ndarray]] = defaultdict(dict)
 
         if verbose:
             pb = tqdm(total=len(self._index.cutpoints), desc="Evaluating cutpoints")
 
         for cp_name, cp_data in self._index.cutpoints.items():
             # create a metric that match at the requested k and threshold
             distance_threshold = float(cp_data["distance"])
             metric = make_classification_metric(cal_metric.name)
             metrics = copy(extra_metrics)
             metrics.append(metric)
 
-            res: Dict[str, Union[str, np.ndarray]] = {}
+            res: dict[str, str | np.ndarray] = {}
             res.update(
                 self._index.evaluate_classification(
                     predictions,
                     y,
                     [distance_threshold],
                     metrics=metrics,
                     matcher=matcher,
@@ -1079,25 +963,99 @@
         Args:
             path: directory where to save the index
             compression: Store index data compressed. Defaults to True.
         """
         index_path = Path(filepath) / "index"
         self._index.save(index_path, compression=compression)
 
+    def save(
+        self,
+        filepath: str | Path,
+        save_index: bool = True,
+        compression: bool = True,
+        overwrite: bool = True,
+        include_optimizer: bool = True,
+        save_format: str | None = None,
+        signatures: Callable | Mapping[str, Callable] | None = None,
+        options: tf.saved_model.SaveOptions | None = None,
+        save_traces: bool = True,
+    ) -> None:
+        """Save Constrative model backbone, projector, and predictor
+
+        Args:
+            filepath: where to save the model.
+            save_index: Save the index content. Defaults to True.
+            compression: Compress index data. Defaults to True.
+            overwrite: Overwrite previous model. Defaults to True.
+            include_optimizer: Save optimizer state. Defaults to True.
+            save_format: Either 'tf' or 'h5', indicating whether to save the
+              model to Tensorflow SavedModel or HDF5. Defaults to 'tf' in
+              TF 2.X, and 'h5' in TF 1.X.
+            signatures: Signatures to save with the SavedModel. Applicable to
+              the 'tf' format only. Please see the signatures argument in
+              tf.saved_model.save for details.
+            options: A `tf.saved_model.SaveOptions` to save with the model.
+              Defaults to None.
+            save_traces (optional): When enabled, the SavedModel will store the
+              function traces for each layer. This can be disabled, so that only
+              the configs of each layer are stored.  Defaults to True. Disabling
+              this will decrease serialization time and reduce file size, but it
+              requires that all custom layers/models implement a get_config()
+              method.
+        """
+        super().save(
+            filepath,
+            overwrite=overwrite,
+            include_optimizer=include_optimizer,
+            save_format=save_format,
+            signatures=signatures,
+            options=options,
+            save_traces=save_traces,
+        )
+
+        if hasattr(self, "_index") and self._index and save_index:
+            self.save_index(filepath, compression=compression)
+        else:
+            msg = "The index was not saved with the model."
+            if not hasattr(self, "_index"):
+                msg = msg + (
+                    "The model does not currently have an index. To use indexing "
+                    "you must call either model.compile() or model.create_index() "
+                    "and set a valid Distance."
+                )
+
+            if not save_index:
+                msg = msg + " The save_index param is set to False."
+
+            print(msg)
+
     def to_data_frame(self, num_items: int = 0) -> PandasDataFrame:
         """Export data as pandas dataframe
 
         Args:
             num_items (int, optional): Num items to export to the dataframe.
             Defaults to 0 (unlimited).
 
         Returns:
             pd.DataFrame: a pandas dataframe.
         """
         return self._index.to_data_frame(num_items=num_items)
 
-    # We don't need from_config as the index is reloaded separatly.
-    # this is kept as a reminder that it was looked into and decided to split
-    # the index reloading instead of overloading this method.
-    # @classmethod
-    # def from_config(cls, config):
-    #     return super().from_config(**config)
+    def get_config(self) -> dict[str, Any]:
+        config = {
+            "backbone": self.backbone,
+            "projector": self.projector,
+            "predictor": self.predictor,
+            "algorithm": self.algorithm,
+        }
+        base_config = super().get_config()
+        return {**base_config, **config}
+
+    @classmethod
+    def from_config(cls, config):
+        if "layers" in config:
+            del config["layers"]
+        if "input_layers" in config:
+            del config["input_layers"]
+        if "output_layers" in config:
+            del config["output_layers"]
+        return create_contrastive_model(**config)
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/models/similarity_model.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/models/similarity_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,27 +34,20 @@
 
 model = SimilarityModel(inputs, outputs)
 model.compile(optimizer=Adam(LR), loss=similarity_loss)
 
 history = model.fit(train_ds)
 ```
 """
+from __future__ import annotations
+
 from collections import defaultdict
+from collections.abc import Mapping, MutableMapping, MutableSequence, Sequence
 from copy import copy
 from pathlib import Path
-from typing import (
-    DefaultDict,
-    Dict,
-    List,
-    MutableMapping,
-    MutableSequence,
-    Optional,
-    Sequence,
-    Union,
-)
 
 import numpy as np
 import tensorflow as tf
 from tabulate import tabulate
 from tensorflow.keras.losses import Loss
 from tensorflow.keras.metrics import Metric
 from tensorflow.keras.optimizers import Optimizer
@@ -94,26 +87,26 @@
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def compile(
         self,
-        optimizer: Union[Optimizer, str, Dict, List] = "rmsprop",
-        loss: Optional[Union[Loss, MetricLoss, str, Dict, List]] = None,
-        metrics: Optional[Union[Metric, DistanceMetric, str, Dict, List]] = None,  # noqa
-        loss_weights: Optional[Union[List, Dict]] = None,
-        weighted_metrics: Optional[Union[Metric, DistanceMetric, str, Dict, List]] = None,  # noqa
+        optimizer: Optimizer | str | Mapping | Sequence = "rmsprop",
+        loss: Loss | MetricLoss | str | Mapping | Sequence | None = None,
+        metrics: Metric | DistanceMetric | str | Mapping | Sequence | None = None,  # noqa
+        loss_weights: Mapping | Sequence | None = None,
+        weighted_metrics: Metric | DistanceMetric | str | Mapping | Sequence | None = None,  # noqa
         run_eagerly: bool = False,
         steps_per_execution: int = 1,
-        distance: Union[Distance, str] = "auto",
-        embedding_output: Optional[int] = None,
-        kv_store: Union[Store, str] = "memory",
-        search: Union[Search, str] = "nmslib",
-        evaluator: Union[Evaluator, str] = "memory",
+        distance: Distance | str = "auto",
+        embedding_output: int | None = None,
+        kv_store: Store | str = "memory",
+        search: Search | str = "nmslib",
+        evaluator: Evaluator | str = "memory",
         stat_buffer_size: int = 1000,
         **kwargs,
     ):
         """Configures the model for training.
 
         Args:
             optimizer: String (name of optimizer) or optimizer instance. See
@@ -201,52 +194,63 @@
 
         Raises:
             ValueError: In case of invalid arguments for
                 `optimizer`, `loss` or `metrics`.
         """
         # Fetching the distance used from the first loss if auto
         if distance == "auto":
-            if isinstance(loss, list):
-                metric_loss = loss[0]
+            if loss is None:
+                distance = distance_canonicalizer("cosine")
             else:
-                metric_loss = loss
+                metric_loss = loss[0] if isinstance(loss, list) else loss
 
-            try:
-                distance = metric_loss.distance
-            except AttributeError:
-                msg = "distance='auto' only works if the first loss is a " "metric loss"
+                try:
+                    distance = metric_loss.distance
+                except AttributeError:
+                    msg = "distance='auto' only works if the first loss is a " "metric loss"
+                    raise ValueError(msg)
 
-                raise ValueError(msg)
-            print(
-                f"Distance metric automatically set to {distance} use the " "distance arg to override.",
-            )
+            print(f"Distance metric automatically set to {distance} use the " "distance arg to override.")
         else:
             distance = distance_canonicalizer(distance)
 
         # init index
         self.create_index(
             distance=distance,
             search=search,
             kv_store=kv_store,
             evaluator=evaluator,
             embedding_output=embedding_output,
             stat_buffer_size=stat_buffer_size,
         )
 
         # call underlying keras method
-        super().compile(
-            optimizer=optimizer,
-            loss=loss,
-            metrics=metrics,
-            loss_weights=loss_weights,
-            weighted_metrics=weighted_metrics,
-            run_eagerly=run_eagerly,
-            steps_per_execution=steps_per_execution,
-            **kwargs,
-        )
+        if tf.executing_eagerly():
+            super().compile(
+                optimizer=optimizer,
+                loss=loss,
+                metrics=metrics,
+                loss_weights=loss_weights,
+                weighted_metrics=weighted_metrics,
+                run_eagerly=run_eagerly,
+                steps_per_execution=steps_per_execution,
+                **kwargs,
+            )
+        else:
+            # apprently keras calls training_v1.py in graph mode which does not
+            # support the steps_per_execution arg.
+            super().compile(
+                optimizer=optimizer,
+                loss=loss,
+                metrics=metrics,
+                loss_weights=loss_weights,
+                weighted_metrics=weighted_metrics,
+                run_eagerly=run_eagerly,
+                **kwargs,
+            )
 
     @property
     def _index(self) -> Indexer:
         if not hasattr(self, "_ix") and self._ix:
             raise AttributeError(
                 "The model does not currently have an index. To create an "
                 "index you must call either model.compile() or "
@@ -257,19 +261,19 @@
 
     @_index.setter
     def _index(self, index: Indexer) -> None:
         self._ix = index
 
     def create_index(
         self,
-        distance: Union[Distance, str] = "cosine",
-        search: Union[Search, str] = "nmslib",
-        kv_store: Union[Store, str] = "memory",
-        evaluator: Union[Evaluator, str] = "memory",
-        embedding_output: int = None,
+        distance: Distance | str = "cosine",
+        search: Search | str = "nmslib",
+        kv_store: Store | str = "memory",
+        evaluator: Evaluator | str = "memory",
+        embedding_output: int | None = None,
         stat_buffer_size: int = 1000,
     ) -> None:
         """Create the model index to make embeddings searchable via KNN.
 
         This method is normally called as part of `SimilarityModel.compile()`.
         However, this method is provided if users want to define a custom index
         outside of the `compile()` method.
@@ -328,16 +332,16 @@
             embedding_output=embedding_output,
             stat_buffer_size=stat_buffer_size,
         )
 
     def index(
         self,
         x: Tensor,
-        y: IntTensor = None,
-        data: Optional[Tensor] = None,
+        y: IntTensor | None = None,
+        data: Tensor | None = None,
         build: bool = True,
         verbose: int = 1,
     ):
         """Index data.
 
         Args:
             x: Samples to index.
@@ -352,31 +356,32 @@
             when calling indexing repeatidly without the need to search between
             the indexing requests. Defaults to True.
 
             verbose: Output indexing progress info. Defaults to 1.
         """
 
         if verbose:
-            print("[Indexing %d points]" % len(x))
+            print(f"[Indexing {len(x)} points]")
             print("|-Computing embeddings")
+
         predictions = self.predict(x)
 
         self._index.batch_add(
             predictions=predictions,
             labels=y,
             data=data,
             build=build,
             verbose=verbose,
         )
 
     def index_single(
         self,
         x: Tensor,
-        y: IntTensor = None,
-        data: Optional[Tensor] = None,
+        y: IntTensor | None = None,
+        data: Tensor | None = None,
         build: bool = True,
         verbose: int = 1,
     ):
         """Index data.
 
         Args:
             x: Sample to index.
@@ -396,68 +401,71 @@
 
         if verbose:
             print("[Indexing 1 point]")
             print("|-Computing embeddings")
 
         x = tf.expand_dims(x, axis=0)
         prediction = self.predict(x)
+
         self._index.add(
             prediction=prediction,
             label=y,
             data=data,
             build=build,
             verbose=verbose,
         )
 
-    def lookup(self, x: Tensor, k: int = 5, verbose: int = 1) -> List[List[Lookup]]:
+    def lookup(self, x: Tensor, k: int = 5, verbose: int = 1) -> list[list[Lookup]]:
         """Find the k closest matches in the index for a set of samples.
 
         Args:
             x: Samples to match.
 
             k: Number of nearest neighboors to lookup. Defaults to 5.
 
             verbose: display progress. Default to 1.
 
         Returns
             list of list of k nearest neighboors:
-            List[List[Lookup]]
+            list[list[Lookup]]
         """
         predictions = self.predict(x)
+
         return self._index.batch_lookup(predictions=predictions, k=k, verbose=verbose)
 
-    def single_lookup(self, x: Tensor, k: int = 5) -> List[Lookup]:
+    def single_lookup(self, x: Tensor, k: int = 5) -> list[Lookup]:
         """Find the k closest matches in the index for a given sample.
 
         Args:
             x: Sample to match.
 
             k: Number of nearest neighboors to lookup. Defaults to 5.
 
         Returns
             list of the k nearest neigboors info:
-            List[Lookup]
+            list[Lookup]
         """
         x = tf.expand_dims(x, axis=0)
         prediction = self.predict(x)
+
         return self._index.single_lookup(prediction=prediction, k=k)
 
     def index_summary(self):
         "Display index info summary."
         self._index.print_stats()
 
     def calibrate(
         self,
         x: FloatTensor,
         y: IntTensor,
-        thresholds_targets: Optional[MutableMapping[str, float]] = None,
+        thresholds_targets: MutableMapping[str, float] | None = None,
         k: int = 1,
-        calibration_metric: Union[str, ClassificationMetric] = "f1",
-        matcher: Union[str, ClassificationMatch] = "match_nearest",
-        extra_metrics: MutableSequence[Union[str, ClassificationMetric]] = [
+        calibration_metric: str | ClassificationMetric = "f1",
+        matcher: str | ClassificationMatch = "match_nearest",
+        extra_metrics: MutableSequence[str | ClassificationMetric] = [
             "precision",
             "recall",
         ],  # noqa
         rounding: int = 2,
         verbose: int = 1,
     ) -> CalibrationResults:
         """Calibrate model thresholds using a test dataset.
@@ -521,15 +529,15 @@
 
     def match(
         self,
         x: FloatTensor,
         cutpoint="optimal",
         no_match_label=-1,
         k=1,
-        matcher: Union[str, ClassificationMatch] = "match_nearest",
+        matcher: str | ClassificationMatch = "match_nearest",
         verbose=0,
     ):
         """Match a set of examples against the calibrated index
 
         For the match function to work, the index must be calibrated using
         calibrate().
 
@@ -587,15 +595,15 @@
 
     def evaluate_retrieval(
         self,
         x: Tensor,
         y: IntTensor,
         retrieval_metrics: Sequence[RetrievalMetric],  # noqa
         verbose: int = 1,
-    ) -> Dict[str, np.ndarray]:
+    ) -> dict[str, np.ndarray]:
         """Evaluate the quality of the index against a test dataset.
 
         Args:
             x: Examples to be matched against the index.
 
             y: Label associated with the examples supplied.
 
@@ -639,21 +647,21 @@
         return results
 
     def evaluate_classification(
         self,
         x: Tensor,
         y: IntTensor,
         k: int = 1,
-        extra_metrics: MutableSequence[Union[str, ClassificationMetric]] = [
+        extra_metrics: MutableSequence[str | ClassificationMetric] = [
             "precision",
             "recall",
         ],  # noqa
-        matcher: Union[str, ClassificationMatch] = "match_nearest",
+        matcher: str | ClassificationMatch = "match_nearest",
         verbose: int = 1,
-    ) -> DefaultDict[str, Dict[str, Union[str, np.ndarray]]]:
+    ) -> defaultdict[str, dict[str, str | np.ndarray]]:
         """Evaluate model classification matching on a given evaluation dataset.
 
         Args:
             x: Examples to be matched against the index.
 
             y: Label associated with the examples supplied.
 
@@ -693,38 +701,38 @@
         cal_metric = self._index.get_calibration_metric()
 
         # get embeddings
         if verbose:
             print("|-Computing embeddings")
         predictions = self.predict(x)
 
-        results: DefaultDict[str, Dict[str, Union[str, np.ndarray]]] = defaultdict(dict)
+        results: defaultdict[str, dict[str, str | np.ndarray]] = defaultdict(dict)
 
         if verbose:
             pb = tqdm(total=len(self._index.cutpoints), desc="Evaluating cutpoints")
 
         for cp_name, cp_data in self._index.cutpoints.items():
             # create a metric that match at the requested k and threshold
             distance_threshold = float(cp_data["distance"])
             metric = make_classification_metric(cal_metric.name)
             metrics = copy(extra_metrics)
             metrics.append(metric)
 
-            res: Dict[str, Union[str, np.ndarray]] = {}
+            res: dict[str, str | np.ndarray] = {}
             res.update(
                 self._index.evaluate_classification(
                     predictions,
                     y,
                     [distance_threshold],
                     metrics=metrics,
                     matcher=matcher,
                     k=k,
                 )
             )
-            res["distance"] = tf.constant([distance_threshold])
+            res["distance"] = tf.constant([distance_threshold], dtype=tf.keras.backend.floatx())
             res["name"] = cp_name
             results[cp_name] = res
             if verbose:
                 pb.update()
 
         if verbose:
             pb.close()
@@ -775,15 +783,15 @@
     def save(
         self,
         filepath: str,
         save_index: bool = True,
         compression: bool = True,
         overwrite: bool = True,
         include_optimizer: bool = True,
-        save_format: Optional[str] = None,
+        save_format: str | None = None,
         signatures=None,
         options=None,
         save_traces: bool = True,
     ):
         """Save the model and the index.
 
         Args:
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/retrieval_metrics/__init__.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/visualization/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,16 +7,12 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Retrieval metrics measure the quality of the embedding space given a
-set query examples and a set of indexed examples. Informally it can be thought
-of as how well the space is clustered among other things.
-"""
-from .bndcg import BNDCG  # noqa
-from .map_at_k import MapAtK  # noqa
-from .precision_at_k import PrecisionAtK  # noqa
-from .recall_at_k import RecallAtK  # noqa
-from .retrieval_metric import RetrievalMetric  # noqa
+"Collection of specialized notebook vizualization tools"
+from .confusion_matrix_viz import confusion_matrix  # noqa
+from .neighbors_viz import viz_neigbors_imgs  # noqa
+from .projector import projector  # noqa
+from .vizualize_views import visualize_views  # noqa
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/retrieval_metrics/bndcg.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/retrieval_metrics/bndcg.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import math
+from __future__ import annotations
 
 import tensorflow as tf
 
 from tensorflow_similarity.types import BoolTensor, FloatTensor, IntTensor
 
 from .retrieval_metric import RetrievalMetric
 
@@ -58,34 +58,34 @@
         e.g., precision@K
 
         k: The number of nearest neighbors over which the metric is computed.
 
         distance_threshold: The max distance below which a nearest neighbor is
         considered a valid match.
 
-        average: {'micro', 'macro'} Determines the type of averaging performed
-        on the data.
-
-        * 'micro': Calculates metrics globally over all data.
+        average: {'micro'} Determines the type of averaging performed over the
+        queries.
 
+        * 'micro': Calculates metrics globally over all queries.
         * 'macro': Calculates metrics for each label and takes the unweighted
-                   mean.
+        mean.
+
+        drop_closest_lookup: If True, remove the closest lookup before computing
+        the metrics. This is used when the query set == indexed set.
     """
 
     def __init__(
         self,
         name: str = "ndcg",
-        k: int = 5,
-        distance_threshold: float = math.inf,
         **kwargs,
     ) -> None:
         if "canonical_name" not in kwargs:
             kwargs["canonical_name"] = "ndcg@k"
 
-        super().__init__(name=name, k=k, distance_threshold=distance_threshold, **kwargs)
+        super().__init__(name=name, **kwargs)
 
     def compute(
         self,
         *,  # keyword only arguments see PEP-570
         query_labels: IntTensor,
         lookup_distances: FloatTensor,
         match_mask: BoolTensor,
@@ -117,20 +117,21 @@
                 "of query labels. Number of lookup distance rows is "
                 f"{tf.shape(lookup_distances)[0]} but the number of query "
                 f"labels is {tf.shape(query_labels)[0]}."
             )
 
         dist_mask = tf.math.less_equal(lookup_distances, self.distance_threshold)
 
+        start_idx = 1 if self.drop_closest_lookup else 0
         k_slice = tf.math.multiply(
-            tf.cast(match_mask, dtype="float"),
-            tf.cast(dist_mask, dtype="float"),
-        )[:, : self.k]
+            tf.cast(match_mask, dtype=lookup_distances.dtype),
+            tf.cast(dist_mask, dtype=lookup_distances.dtype),
+        )[:, start_idx : start_idx + self.k]
 
-        rank = tf.range(1, self.k + 1, dtype="float")
+        rank = tf.range(1, self.k + 1, dtype=lookup_distances.dtype)
         rank_weights = tf.math.divide(tf.math.log1p(rank), tf.math.log(2.0))
 
         # the numerator is simplier here because we are using binary weights
         dcg = tf.math.reduce_sum(k_slice / rank_weights, axis=1)
 
         # generate the "ideal ordering".
         ideal_ordering = tf.sort(k_slice, direction="DESCENDING", axis=1)
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/retrieval_metrics/map_at_k.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/retrieval_metrics/map_at_k.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,25 +7,24 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
-from typing import Mapping
+from collections.abc import Mapping
 
 import tensorflow as tf
 
-from tensorflow_similarity.types import BoolTensor, FloatTensor, IntTensor
+from .precision_at_k import PrecisionAtK
 
-from .retrieval_metric import RetrievalMetric
 
-
-class MapAtK(RetrievalMetric):
+class MapAtK(PrecisionAtK):
     r"""Mean Average precision - mAP@K is computed as.
 
     $$
     mAP_i@K = \frac{\sum_{j = 1}^{K} {rel_i_j}\times{P_i@j}}{R}
     $$
 
     Where: K is the number of neighbors in the i_th query result set.
@@ -50,97 +49,59 @@
     are relevant to the query; however, it requires that we pass a mapping from
     the class id to the number of indexed examples for that class.
 
     Args:
         r: A mapping from class id to the number of examples in the index,
         e.g., r[4] = 10 represents 10 indexed examples from class 4.
 
+        clip_at_r: If True, set precision at K values to 0.0 for all values
+        with rank greater than the count defined in the r mapping, e.g., a
+        result set of 10 values, for a query label with 7 indexed examples,
+        will have the last 3 precision at K values set to 0.0. Use this to
+        compute MAP@R. See section 3.2 of https://arxiv.org/pdf/2003.08505.pdf
+
         name: Name associated with the metric object, e.g., avg_precision@5
 
         canonical_name: The canonical name associated with metric, e.g.,
         avg_precision@K
 
         k: The number of nearest neighbors over which the metric is computed.
 
         distance_threshold: The max distance below which a nearest neighbor is
         considered a valid match.
 
         average: {'micro'} Determines the type of averaging performed over the
         queries.
 
         * 'micro': Calculates metrics globally over all queries.
+
+        drop_closest_lookup: If True, remove the closest lookup before computing
+        the metrics. This is used when the query set == indexed set.
     """
 
     def __init__(
         self,
-        r: Mapping[int, int],
+        r: Mapping[int, int] | None = None,
+        clip_at_r: bool = False,
         name: str = "map",
-        k: int = 5,
-        average: str = "micro",
         **kwargs,
     ) -> None:
-        if average == "macro":
+        if kwargs.get("average") == "macro":
             raise ValueError("Mean Average Precision only supports micro averaging.")
 
         if "canonical_name" not in kwargs:
             kwargs["canonical_name"] = "map@k"
 
-        super().__init__(name=name, k=k, average=average, **kwargs)
-        self.r = r
-
-    def get_config(self):
-        config = {
-            "r": self.r,
-        }
-        base_config = super().get_config()
-        return {**base_config, **config}
-
-    def compute(
-        self,
-        *,  # keyword only arguments see PEP-570
-        query_labels: IntTensor,
-        match_mask: BoolTensor,
-        **kwargs,
-    ) -> FloatTensor:
-        """Compute the metric
-
-        Args:
-            query_labels: A 1D array of the labels associated with the
-            embedding queries.
-
-            match_mask: A 2D mask where a 1 indicates a match between the
-            jth query and the kth neighbor and a 0 indicates a mismatch.
-
-            **kwargs: Additional compute args
-
-        Returns:
-            A rank 0 tensor containing the metric.
-        """
-        self._check_shape(query_labels, match_mask)
-
-        k_slice = tf.cast(match_mask[:, : self.k], dtype="float")
-        tp = tf.math.cumsum(k_slice, axis=1)
-        p_at_k = tf.math.divide(tp, tf.range(1, self.k + 1, dtype="float"))
-        p_at_k = tf.math.multiply(k_slice, p_at_k)
-
-        if self.average == "micro":
-            table = tf.lookup.StaticHashTable(
-                tf.lookup.KeyValueTensorInitializer(
-                    list(self.r.keys()),
-                    list(self.r.values()),
-                    key_dtype=tf.int32,
-                    value_dtype=tf.int32,
-                ),
-                default_value=-1,
-            )
-            class_counts = table.lookup(query_labels)
-            avg_p_at_k = tf.math.divide(
-                tf.math.reduce_sum(p_at_k, axis=1),
-                tf.cast(class_counts, dtype="float"),
-            )
-
-            avg_p_at_k = tf.math.reduce_mean(avg_p_at_k)
-        else:
-            raise ValueError(f"{self.average} is not a supported average option")
+        super().__init__(r=r, clip_at_r=clip_at_r, name=name, **kwargs)
 
-        result: FloatTensor = avg_p_at_k
-        return result
+    @property
+    def name(self) -> str:
+        if self.clip_at_r:
+            return f"{self._name}"
+
+        return super().name
+
+    def _get_matches(self, x):
+        tp = tf.math.cumsum(x, axis=1)
+        p_at_k = tf.math.divide_no_nan(tp, tf.range(1, x.shape[1] + 1, dtype=tp.dtype))
+        p_at_k = tf.math.multiply(x, p_at_k)
+        return p_at_k
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/retrieval_metrics/precision_at_k.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/retrieval_metrics/recall_at_k.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,99 +7,94 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 import tensorflow as tf
 
 from tensorflow_similarity.types import BoolTensor, FloatTensor, IntTensor
 
 from .retrieval_metric import RetrievalMetric
 
 
-class PrecisionAtK(RetrievalMetric):
-    r"""Precision@K is computed as.
+class RecallAtK(RetrievalMetric):
+    """The metric learning version of Recall@K.
 
-    $$
-    P_i@k = \frac{TP_i}{TP_i+FP_i} = \frac{\sum_{j = 1}^{k} {rel_i_j}}{K}
-    $$
-
-    Where: K is the number of neighbors in the i_th query result set.
-           rel is the relevance mask (indicator function) for the i_th query.
-           i represents the i_th query.
-           j represents the j_th ranked query result.
-
-    P@K is unordered and does not take into account the rank of the TP results.
-
-    This metric is useful when we are interested in evaluating the embedding
-    within the context of a kNN classifier or as part of a clustering method.
+    A query is counted as a positive when ANY lookup in top K match the query
+    class, 0 otherwise.
 
     Args:
-        name: Name associated with the metric object, e.g., precision@5
+        name: Name associated with the metric object, e.g., recall@5
 
         canonical_name: The canonical name associated with metric,
-        e.g., precision@K
+        e.g., recall@K
 
         k: The number of nearest neighbors over which the metric is computed.
 
         distance_threshold: The max distance below which a nearest neighbor is
         considered a valid match.
 
-        average: {'micro', 'macro'} Determines the type of averaging performed
-        on the data.
-
-        * 'micro': Calculates metrics globally over all data.
+        average: {'micro'} Determines the type of averaging performed over the
+        queries.
 
+        * 'micro': Calculates metrics globally over all queries.
         * 'macro': Calculates metrics for each label and takes the unweighted
-                   mean.
+        mean.
+
+        drop_closest_lookup: If True, remove the closest lookup before computing
+        the metrics. This is used when the query set == indexed set.
     """
 
-    def __init__(self, name: str = "precision", k: int = 5, **kwargs) -> None:
+    def __init__(self, name: str = "recall", **kwargs) -> None:
         if "canonical_name" not in kwargs:
-            kwargs["canonical_name"] = "precision@k"
+            kwargs["canonical_name"] = "recall@k"
 
-        super().__init__(name=name, k=k, **kwargs)
+        super().__init__(name=name, **kwargs)
 
     def compute(
         self,
         *,  # keyword only arguments see PEP-570
         query_labels: IntTensor,
         match_mask: BoolTensor,
         **kwargs,
     ) -> FloatTensor:
         """Compute the metric
 
         Args:
-            query_labels: A 1D array of the labels associated with the
+            query_labels: A 1D tensor of the labels associated with the
             embedding queries.
 
             match_mask: A 2D mask where a 1 indicates a match between the
             jth query and the kth neighbor and a 0 indicates a mismatch.
-
+            k
             **kwargs: Additional compute args.
 
         Returns:
             A rank 0 tensor containing the metric.
         """
         self._check_shape(query_labels, match_mask)
 
-        k_slice = tf.cast(match_mask[:, : self.k], dtype="float")
-        tp = tf.math.reduce_sum(k_slice, axis=1)
-        per_example_p = tf.math.divide(tp, self.k)
+        start_k = 1 if self.drop_closest_lookup else 0
+        k_slice = match_mask[:, start_k : start_k + self.k]
+
+        match_indicator = tf.math.reduce_any(k_slice, axis=1)
+        match_indicator = tf.cast(match_indicator, dtype=tf.keras.backend.floatx())
 
         if self.average == "micro":
-            p_at_k = tf.math.reduce_mean(per_example_p)
+            recall_at_k = tf.math.reduce_mean(match_indicator)
         elif self.average == "macro":
             per_class_metrics = 0
             class_labels = tf.unique(tf.reshape(query_labels, (-1)))[0]
+            # TODO(ovallis): potential slowness.
             for label in class_labels:
                 idxs = tf.where(query_labels == label)
-                c_slice = tf.gather(per_example_p, indices=idxs)
+                c_slice = tf.gather(match_indicator, indices=idxs)
                 per_class_metrics += tf.math.reduce_mean(c_slice)
-            p_at_k = tf.math.divide(per_class_metrics, len(class_labels))
+            recall_at_k = tf.math.divide(per_class_metrics, len(class_labels))
         else:
             raise ValueError(f"{self.average} is not a supported average " "option")
-        result: FloatTensor = p_at_k
+        result: FloatTensor = recall_at_k
         return result
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/retrieval_metrics/retrieval_metric.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/retrieval_metrics/retrieval_metric.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 import math
 from abc import ABC, abstractmethod
 
 import tensorflow as tf
 
 from tensorflow_similarity.types import BoolTensor, FloatTensor, IntTensor
@@ -37,36 +38,41 @@
         average: {'micro'} Determines the type of averaging performed over the
         queries.
 
         * 'micro': Calculates metrics globally over all queries.
         * 'macro': Calculates metrics for each label and takes the unweighted
         mean.
 
+        drop_closest_lookup: If True, remove the closest lookup before computing
+        the metrics. This is used when the query set == indexed set.
+
     `RetrievalMetric` measure the retrieval quality given a query label and the
     labels from the set of lookup results.
     """
 
     def __init__(
         self,
         name: str = "",
         canonical_name: str = "",
         k: int = 5,
         distance_threshold: float = math.inf,
         average: str = "micro",
+        drop_closest_lookup: bool = False,
     ) -> None:
         self._name = name
         self.canonical_name = canonical_name
         self.k = k
         self.distance_threshold = distance_threshold
         self.average = average
+        self.drop_closest_lookup = drop_closest_lookup
 
     @property
     def name(self) -> str:
         if self.distance_threshold and self.distance_threshold != math.inf:
-            return f"{self._name}@{self.k} : " f"distance_threshold@{self.distance_threshold}"
+            return f"{self._name}@{self.k} : distance_threshold@{self.distance_threshold}"
         else:
             return f"{self._name}@{self.k}"
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/retrieval_metrics/utils.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/retrieval_metrics/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
+
 import tensorflow as tf
 
 from tensorflow_similarity.types import BoolTensor, IntTensor
 
 
 def compute_match_mask(query_labels: IntTensor, lookup_labels: IntTensor) -> BoolTensor:
     """Compute a boolean mask (indicator function) marking the TPs in the results.
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/samplers/__init__.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/samplers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,12 +25,13 @@
 To address this need, TensorFlow Similarity provides data samplers for
 various types of datasets that:
 - Ensure that batches contain at least N examples of each class present in
 the batch.
 - Support restricting the batches to a subset of the classes present in
 the dataset.
 """
+from .file_samplers import MultiShotFileSampler  # noqa
 from .memory_samplers import MultiShotMemorySampler  # noqa
 from .memory_samplers import SingleShotMemorySampler  # noqa
 from .tfdataset_samplers import TFDatasetMultiShotMemorySampler  # noqa
 from .tfrecords_samplers import TFRecordDatasetSampler  # noqa
 from .utils import select_examples  # noqa
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/samplers/memory_samplers.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/samplers/memory_samplers.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,42 +7,42 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 import random
 from collections import defaultdict
-from typing import Optional, Sequence, Set, Tuple, TypeVar
+from collections.abc import Callable, Sequence
 
 import numpy as np
 import tensorflow as tf
 from tqdm.auto import tqdm
 
 from tensorflow_similarity.types import FloatTensor, IntTensor
 
 from .samplers import Augmenter, Sampler
 from .utils import select_examples
 
-T = TypeVar("T", FloatTensor, IntTensor)
-
 
 class MultiShotMemorySampler(Sampler):
     def __init__(
         self,
         x,
         y,
+        load_example_fn: Callable = lambda q: q,
         classes_per_batch: int = 2,
         examples_per_class_per_batch: int = 2,
         steps_per_epoch: int = 1000,
-        class_list: Sequence[int] = None,
-        total_examples_per_class: int = None,
-        augmenter: Optional[Augmenter] = None,
+        class_list: Sequence[int] | None = None,
+        total_examples_per_class: int | None = None,
+        augmenter: Augmenter | None = None,
         warmup: int = -1,
     ):
         """Create a Multishot in memory sampler that ensures that each batch is
         well balanced. That is, each batch aims to contain
         `examples_per_class_per_batch` examples of `classes_per_batch` classes.
 
         The `batch_size` used during training will be equal to:
@@ -59,17 +59,23 @@
 
         Memory samplers are good for datasets that fit in memory. If you have
         larger ones that needs to sample from disk then use the
         [TFRecordDatasetSampler()](tfdataset_sampler.md)
 
 
         Args:
-            x: examples.
-
-            y: labels.
+            x: Examples. It can be anything, like a numpy array or a list
+            of file paths. In order to determine the real examples, each
+            element of `x` is passed through `load_example_fn`.
+
+            y: Labels.
+
+            load_example_fn: A function for loading real examples from `x`.
+            It is useful for loading images from their corresponding file path
+            provided in `x` or similar situations. Defaults to `lambda q: q`.
 
             classes_per_batch: Numbers of distinct class to include in a
             single batch
 
             examples_per_class_per_batch: How many example of each class
             to use per batch. Defaults to 2.
 
@@ -96,53 +102,51 @@
             classes_per_batch,
             examples_per_class_per_batch=examples_per_class_per_batch,
             steps_per_epoch=steps_per_epoch,
             augmenter=augmenter,
             warmup=warmup,
         )
 
+        self.load_example_fn = load_example_fn
+
         # precompute information we need
         if not class_list:
             self.class_list = list(set([int(e) for e in y]))
         else:
             # dedup in case user mess up and cast in case its a tensor
             self.class_list = list(set([int(c) for c in class_list]))
 
         if classes_per_batch > len(self.class_list):
             raise ValueError(
                 "the value of classes_per_batch must be <= to the " "number of existing classes in the dataset"
             )
 
         # We only want to warn users once per class if we are sampling with
         # replacement
-        self._small_classes: Set[int] = set()
+        self._small_classes: set[int] = set()
 
         # filter
-        x, y = select_examples(
+        self._x, self._y = select_examples(
             x,
             y,
             class_list=self.class_list,
             num_examples_per_class=total_examples_per_class,
         )
 
-        # assign after potential selection
-        self._x = x
-        self._y = y
-
         # we need to reindex here  as the numbers of samples might have
         # changed due to the filtering
         # In this sampler, contrary to file based one, the pool of examples
         # wont' change so we can optimize by doing this step in the constructor
         self.index_per_class = defaultdict(list)
-        cls = [int(c) for c in y]  # need to cast as  tensor lookup are slowww
-        for idx in tqdm(range(len(x)), desc="indexing classes"):
+        cls = [int(c) for c in self._y]  # need to cast as  tensor lookup are slowww
+        for idx in tqdm(range(len(self._x)), desc="indexing classes"):
             cl = cls[idx]
             self.index_per_class[cl].append(idx)
 
-    def _get_examples(self, batch_id: int, num_classes: int, examples_per_class: int) -> Tuple[FloatTensor, IntTensor]:
+    def _get_examples(self, batch_id: int, num_classes: int, examples_per_class: int) -> tuple[FloatTensor, IntTensor]:
         """Get the set of examples that would be used to create a single batch.
 
         Notes:
          - before passing the batch data to TF, the sampler will call the
            augmenter function (if any) on the returned example.
 
          - A batch_size = num_classes * examples_per_class
@@ -181,23 +185,23 @@
             else:
                 idxs.extend(random.sample(class_idxs, k=examples_per_class))
 
         batch_x = []
         batch_y = []
         # strip examples if needed. This might happen due to rounding
         for idx in idxs[: self.batch_size]:
-            batch_x.append(self._x[idx])
+            batch_x.append(self.load_example_fn(self._x[idx]))
             batch_y.append(self._y[idx])
 
         return (
             tf.convert_to_tensor(np.array(batch_x)),
             tf.convert_to_tensor(np.array(batch_y)),
         )
 
-    def get_slice(self, begin: int = 0, size: int = -1) -> Tuple[FloatTensor, IntTensor]:
+    def get_slice(self, begin: int = 0, size: int = -1) -> tuple[FloatTensor, IntTensor]:
         """Extracts a slice over both the x and y tensors.
 
         This method extracts a slice of size `size` over the first dimension of
         both the x and y tensors starting at the index specified by `begin`.
 
         The value of `begin + size` must be less than `self.num_examples`.
 
@@ -205,35 +209,26 @@
             begin: The starting index.
 
             size: The size of the slice.
 
         Returns:
             A Tuple of FloatTensor and IntTensor
         """
-        slice_x: FloatTensor = self._get_slice(self._x, begin, size)
-        slice_y: IntTensor = self._get_slice(self._y, begin, size)
+        slice_x = [self.load_example_fn(q) for q in self._x[begin : begin + size]]
+        slice_y = self._y[begin : begin + size]
 
-        return slice_x, slice_y
-
-    def _get_slice(self, input_: T, begin: int, size: int) -> T:
-        b = [0] * len(tf.shape(input_))
-        b[0] = begin
-        s = [-1] * len(tf.shape(input_))
-        s[0] = size
-
-        slice_: T = tf.slice(input_, b, s)
-        return slice_
+        return tf.convert_to_tensor(slice_x), tf.convert_to_tensor(slice_y)
 
     @property
     def num_examples(self) -> int:
         return len(self._x)
 
     @property
     def example_shape(self):
-        return self._x[0].shape
+        return self.load_example_fn(self._x[0]).shape
 
 
 class SingleShotMemorySampler(Sampler):
     def __init__(
         self,
         x,
         augmenter: Augmenter,
@@ -290,15 +285,15 @@
             steps_per_epoch=steps_per_epoch,
             augmenter=augmenter,
             warmup=warmup,
         )
         self._x = x
         self._y = tf.range(0, self.num_examples, dtype="int32")
 
-    def _get_examples(self, batch_id: int, num_classes: int, examples_per_class: int) -> Tuple[FloatTensor, IntTensor]:
+    def _get_examples(self, batch_id: int, num_classes: int, examples_per_class: int) -> tuple[FloatTensor, IntTensor]:
         """Get the set of examples that would be used to create a single batch.
 
         Notes:
          - before passing the batch data to TF, the sampler will call the
            augmenter function (if any) on the returned example.
 
          - A batch_size = num_classes * examples_per_class
@@ -328,15 +323,15 @@
         # strip examples if needed. This might happen due to rounding
         if len(x) > self.batch_size:
             x = x[: self.batch_size]
             y = y[: self.batch_size]
 
         return x, y
 
-    def get_slice(self, begin: int = 0, size: int = -1) -> Tuple[FloatTensor, IntTensor]:
+    def get_slice(self, begin: int = 0, size: int = -1) -> tuple[FloatTensor, IntTensor]:
         """Extracts an augmented slice over both the x and y tensors.
 
         This method extracts a slice of size `size` over the first dimension of
         both the x and y tensors starting at the index specified by `begin`.
 
         The value of `begin + size` must be less than `self.num_examples`.
 
@@ -344,35 +339,26 @@
             begin: The starting index.
 
             size: The size of the slice.
 
         Returns:
             A Tuple of FloatTensor and IntTensor
         """
-        slice_x: FloatTensor = self._get_slice(self._x, begin, size)
-        slice_y: IntTensor = self._get_slice(self._y, begin, size)
+        slice_x = tf.convert_to_tensor(self._x[begin : begin + size])
+        slice_y = tf.convert_to_tensor(self._y[begin : begin + size])
         if self.augmenter is not None:
             slice_x, slice_y = self.augmenter(
                 slice_x,
                 slice_y,
                 self.num_augmentations_per_example,
                 self.is_warmup,
             )
 
         return slice_x, slice_y
 
-    def _get_slice(self, input_: T, begin: int, size: int) -> T:
-        b = [0] * len(tf.shape(input_))
-        b[0] = begin
-        s = [-1] * len(tf.shape(input_))
-        s[0] = size
-
-        slice_: T = tf.slice(input_, b, s)
-        return slice_
-
     @property
     def num_examples(self) -> int:
         return len(self._x)
 
     @property
     def example_shape(self):
         return self._x[0].shape
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/samplers/samplers.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/samplers/samplers.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,41 +7,43 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 import abc
-from typing import Any, Callable, List, Mapping, Optional, Tuple, Union
+from typing import Any, Callable, List, Mapping, Union
 
 import numpy as np
 from tensorflow import Tensor
-from tensorflow.keras.utils import Sequence
+from tensorflow.keras.utils import Sequence as KerasSequence
 
 from tensorflow_similarity.augmenters import Augmenter
 
 # Not currently used. Might be useful to allows gradual call of augmenter
 Scheduler = Callable[[Any], Any]
 
 # All basic types accepted by tf.keras.Model.fit(). This doesn't include tf.data
 # datasets or keras generators.
+# TODO(ovallis): Replace Union with pep585 typing '|' once numpy arrays support it.
 Batch = Union[np.ndarray, List[np.ndarray], Tensor, List[Tensor], Mapping[str, Union[np.ndarray, Tensor]]]
 
 
-class Sampler(Sequence, metaclass=abc.ABCMeta):
+class Sampler(KerasSequence, metaclass=abc.ABCMeta):
     def __init__(
         self,
         classes_per_batch: int,
         examples_per_class_per_batch: int = 2,
-        num_augmentations_per_example: int = 0,
+        num_augmentations_per_example: int = 1,
         steps_per_epoch: int = 1000,
-        augmenter: Optional[Augmenter] = None,
-        # scheduler: Optional[Scheduler] = None,
+        augmenter: Augmenter | None = None,
+        # scheduler: Scheduler | None = None,
         warmup: int = 0,
     ) -> None:
         """Create a dataset sampler that ensure that each batch contains at
         least `examples_per_class_per_batch` examples of `classes_per_batch`
         classes. Sampling is needed as contrastive loss requires at least two
         examples of the same class present in a batch. The batch_size used
         during training will be equal to: `classes_per_batch` *
@@ -53,15 +55,15 @@
         Args:
             classes_per_batch: Numbers of classes to include in a single batch
 
             examples_per_class_per_batch: how many examples of each class to
             use per batch. Defaults to 2.
 
             num_augmentations_per_example: how many augmented versions of an
-            example will be produced by the augmenter. Defaults to 0.
+            example will be produced by the augmenter. Defaults to 1.
 
             steps_per_epoch: How many steps/batches per epoch. Defaults to
             1000.
 
             augmenter: A function that takes a batch in and returns a batch
             out. Can alter the number of examples returned, which in turn can
             change the batch_size used. Defaults to None.
@@ -83,19 +85,19 @@
 
         # Tell the users what to expect as they might be unsure what the batch
         # size will be
         print(
             f"\nThe initial batch size is {self.batch_size} "
             f"({self.classes_per_batch} classes * "
             f"{self.examples_per_class_per_batch} examples per class) with "
-            f"{self.num_augmentations_per_example} augmenters"
+            f"{0 if self.augmenter is None else self.num_augmentations_per_example} augmentations"
         )
 
     @abc.abstractmethod
-    def _get_examples(self, batch_id: int, num_classes: int, examples_per_class: int) -> Tuple[Batch, Batch]:
+    def _get_examples(self, batch_id: int, num_classes: int, examples_per_class: int) -> tuple[Batch, Batch]:
         """Get the set of examples that would be used to create a single batch.
 
         Notes:
          - before passing the batch data to TF, the sampler will call the
            augmenter function (if any) on the returned example.
 
          - A batch_size = num_classes * examples_per_class
@@ -126,18 +128,18 @@
         #     self.scheduler(self.epoch)
 
         self.epoch += 1
         if self.is_warmup and (self.epoch >= self.warmup):
             print("Warmup complete")
             self.is_warmup = False
 
-    def __getitem__(self, batch_id: int) -> Tuple[Batch, Batch]:
+    def __getitem__(self, batch_id: int) -> tuple[Batch, Batch]:
         return self.generate_batch(batch_id)
 
-    def generate_batch(self, batch_id: int) -> Tuple[Batch, Batch]:
+    def generate_batch(self, batch_id: int) -> tuple[Batch, Batch]:
         """Generate a batch of data.
 
 
         Args:
             batch_id ([type]): [description]
 
         Returns:
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/samplers/tfdataset_samplers.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/samplers/tfdataset_samplers.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
-from typing import Callable, Optional, Sequence, Tuple, TypeVar, Union
+from collections.abc import Sequence
+from typing import Callable, Tuple, TypeVar
 
 import tensorflow_datasets as tfds
 from tqdm.auto import tqdm
 
 from tensorflow_similarity.types import FloatTensor, IntTensor
 
 from .memory_samplers import MultiShotMemorySampler
@@ -30,21 +32,21 @@
 class TFDatasetMultiShotMemorySampler(MultiShotMemorySampler):
     def __init__(
         self,
         dataset_name: str,
         classes_per_batch: int,
         x_key: str = "image",
         y_key: str = "label",
-        splits: Union[str, Sequence[str]] = ["train", "test"],
+        splits: str | Sequence[str] = ["train", "test"],
         examples_per_class_per_batch: int = 2,
         steps_per_epoch: int = 1000,
-        class_list: Sequence[int] = None,
-        total_examples_per_class: int = None,
-        preprocess_fn: Optional[PreProcessFn] = None,
-        augmenter: Optional[Augmenter] = None,
+        class_list: Sequence[int] | None = None,
+        total_examples_per_class: int | None = None,
+        preprocess_fn: PreProcessFn | None = None,
+        augmenter: Augmenter | None = None,
         warmup: int = -1,
     ):
         """Create a Multishot in memory sampler from a dataset downloaded from
         the [TensorFlow datasets catalogue](https://www.tensorflow.org/datasets/catalog/)
 
         The sampler ensures that each batch is well balanced by ensure that
         each batch aims to contains `example_per_class` examples of
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/samplers/tfrecords_samplers.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/samplers/tfrecords_samplers.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,32 +7,33 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 import os
-from typing import Callable, Optional
+from collections.abc import Callable
 
 import tensorflow as tf
 from absl import logging
 
 
 def TFRecordDatasetSampler(
     shard_path: str,
     deserialization_fn: Callable,
     example_per_class: int = 2,
     batch_size: int = 32,
-    shards_per_cycle: int = None,
-    compression: Optional[str] = None,
+    shards_per_cycle: int | None = None,
+    compression: str | None = None,
     parallelism: int = tf.data.AUTOTUNE,
     async_cycle: bool = False,
-    prefetch_size: Optional[int] = None,
+    prefetch_size: int | None = None,
     shard_suffix: str = "*.tfrec",
     num_repeat: int = -1,
 ) -> tf.data.Dataset:
     """Create a [TFRecordDataset](https://www.tensorflow.org/api_docs/python/tf/data/TFRecordDataset) based sampler.
 
     This sampler should be used when using a TFDataset or have a large
     dataset that needs to be stored on file.
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/samplers/utils.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/samplers/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,31 +7,32 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 import random
 from collections import defaultdict
-from typing import Sequence, Tuple
+from collections.abc import Sequence
 
 import numpy as np
 from tqdm.auto import tqdm
 
 from tensorflow_similarity.types import FloatTensor, IntTensor
 
 
 def select_examples(
     x: FloatTensor,
     y: IntTensor,
-    class_list: Sequence[int] = None,
-    num_examples_per_class: int = None,
-) -> Tuple[np.ndarray, np.ndarray]:
+    class_list: Sequence[int] | None = None,
+    num_examples_per_class: int | None = None,
+) -> tuple[np.ndarray, np.ndarray]:
     """Randomly select at most N examples per class
 
     Args:
         x: A 2-D Tensor containing the data.
 
         y: A 1-D Tensor containing the labels.
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/search/__init__.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/search/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,9 +28,15 @@
 pass it to the `compile()` method of your [SimilarityModel].
 
 Adding your search backend as a built-in choice invlolves
 modifiying the [Indexer](../indexer.md) and sending a PR. In general, unless
 the backend is of general use, its better to not include it as
 a built-in option as it must be supported moving forward.
 """
+import logging
+
+# Disable the INFO logging from NMSLIB
+logging.getLogger("nmslib").setLevel(logging.WARNING)
+
 from .nmslib_search import NMSLibSearch  # noqa
 from .search import Search  # noqa
+from .utils import make_search  # noqa
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/search/search.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/search/search.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,35 +7,47 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import List, Sequence, Tuple, Union
+from collections.abc import Sequence
+from typing import Any
 
-from tensorflow_similarity.distances import Distance
+from tensorflow_similarity.distances import Distance, distance_canonicalizer
 from tensorflow_similarity.types import FloatTensor
 
 
 class Search(ABC):
-    @abstractmethod
-    def __init__(self, distance: Union[Distance, str], dim: int, verbose: bool, **kwargs):
+    def __init__(
+        self,
+        distance: Distance | str,
+        dim: int,
+        verbose: int = 0,
+        name: str | None = None,
+        **kwargs,
+    ):
         """Initializes a nearest neigboors search index.
 
         Args:
             distance: the distance used to compute the distance between
             embeddings.
 
             dim: the size of the embeddings.
 
             verbose: be verbose.
         """
+        self.distance: Distance = distance_canonicalizer(distance)
+        self.dim = dim
+        self.verbose = verbose
+        self.name = name if name is not None else self.__class__.__name__
 
     @abstractmethod
     def add(self, embedding: FloatTensor, idx: int, verbose: int = 1, **kwargs):
         """Add a single embedding to the search index.
 
         Args:
             embedding: The embedding to index as computed by
@@ -58,24 +70,24 @@
             the embeddings to allow to lookup the data associated
             with the returned embeddings.
 
             verbose: Be verbose. Defaults to 1.
         """
 
     @abstractmethod
-    def lookup(self, embedding: FloatTensor, k: int = 5) -> Tuple[List[int], List[float]]:
+    def lookup(self, embedding: FloatTensor, k: int = 5) -> tuple[list[int], list[float]]:
         """Find embedding K nearest neighboors embeddings.
 
         Args:
             embedding: Query embedding as predicted by the model.
             k: Number of nearest neighboors embedding to lookup. Defaults to 5.
         """
 
     @abstractmethod
-    def batch_lookup(self, embeddings: FloatTensor, k: int = 5) -> Tuple[List[List[int]], List[List[float]]]:
+    def batch_lookup(self, embeddings: FloatTensor, k: int = 5) -> tuple[list[list[int]], list[list[float]]]:
         """Find embeddings K nearest neighboors embeddings.
 
         Args:
             embedding: Batch of query embeddings as predicted by the model.
             k: Number of nearest neighboors embedding to lookup. Defaults to 5.
         """
 
@@ -90,7 +102,23 @@
     @abstractmethod
     def load(self, path: str):
         """load index on disk
 
         Args:
             path: where to store the data
         """
+
+    def get_config(self) -> dict[str, Any]:
+        """Contains the search configuration.
+
+        Returns:
+            A Python dict containing the configuration of the search obj.
+        """
+        config = {
+            "distance": self.distance.name,
+            "dim": self.dim,
+            "verbose": self.verbose,
+            "name": self.name,
+            "canonical_name": self.__class__.__name__,
+        }
+
+        return config
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/stores/__init__.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/stores/memory_store.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/stores/memory_store.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 import io
+from collections.abc import Sequence
 from pathlib import Path
-from typing import List, Optional, Sequence, Tuple
 
 import numpy as np
 import pandas as pd
 import tensorflow as tf
 
 from tensorflow_similarity.types import FloatTensor, PandasDataFrame, Tensor
 
@@ -27,25 +28,25 @@
 
 class MemoryStore(Store):
     """Efficient in-memory dataset store"""
 
     def __init__(self) -> None:
         # We are using a native python array in memory for its row speed.
         # Serialization / export relies on Arrow.
-        self.labels: List[Optional[int]] = []
-        self.embeddings: List[FloatTensor] = []
-        self.data: List[Optional[Tensor]] = []
+        self.labels: list[int | None] = []
+        self.embeddings: list[FloatTensor] = []
+        self.data: list[Tensor | None] = []
         self.num_items: int = 0
         pass
 
     def add(
         self,
         embedding: FloatTensor,
-        label: Optional[int] = None,
-        data: Optional[Tensor] = None,
+        label: int | None = None,
+        data: Tensor | None = None,
     ) -> int:
         """Add an Embedding record to the key value store.
 
         Args:
             embedding: Embedding predicted by the model.
 
             label: Class numerical id. Defaults to None.
@@ -61,17 +62,17 @@
         self.data.append(data)
         self.num_items += 1
         return idx
 
     def batch_add(
         self,
         embeddings: Sequence[FloatTensor],
-        labels: Optional[Sequence[int]] = None,
-        data: Optional[Sequence[Tensor]] = None,
-    ) -> List[int]:
+        labels: Sequence[int] | None = None,
+        data: Sequence[Tensor] | None = None,
+    ) -> list[int]:
         """Add a set of embedding records to the key value store.
 
         Args:
             embeddings: Embeddings predicted by the model.
 
             labels: Class numerical ids. Defaults to None.
 
@@ -79,34 +80,34 @@
 
         See:
             add() for what a record contains.
 
         Returns:
             List of associated record id.
         """
-        idxs: List[int] = []
+        idxs: list[int] = []
         for idx, embedding in enumerate(embeddings):
             label = None if labels is None else labels[idx]
             rec_data = None if data is None else data[idx]
             idxs.append(self.add(embedding, label, rec_data))
         return idxs
 
-    def get(self, idx: int) -> Tuple[FloatTensor, Optional[int], Optional[Tensor]]:
+    def get(self, idx: int) -> tuple[FloatTensor, int | None, Tensor | None]:
         """Get an embedding record from the key value store.
 
         Args:
             idx: Id of the record to fetch.
 
         Returns:
             record associated with the requested id.
         """
 
         return self.embeddings[idx], self.labels[idx], self.data[idx]
 
-    def batch_get(self, idxs: Sequence[int]) -> Tuple[List[FloatTensor], List[Optional[int]], List[Optional[Tensor]]]:
+    def batch_get(self, idxs: Sequence[int]) -> tuple[list[FloatTensor], list[int | None], list[Tensor | None]]:
         """Get embedding records from the key value store.
 
         Args:
             idxs: ids of the records to fetch.
 
         Returns:
             List of records associated with the requested ids.
@@ -196,13 +197,13 @@
 
         if not num_records:
             num_records = self.num_items
 
         data = {
             "embeddings": self.embeddings[:num_records],
             "data": self.data[:num_records],
-            "lables": self.labels[:num_records],
+            "labels": self.labels[:num_records],
         }
 
         # forcing type from Any to PandasFrame
         df: PandasDataFrame = pd.DataFrame.from_dict(data)
         return df
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/stores/store.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/stores/store.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import List, Optional, Sequence, Tuple
+from collections.abc import Sequence
 
 from tensorflow_similarity.types import FloatTensor, PandasDataFrame, Tensor
 
 
 class Store(ABC):
     @abstractmethod
-    def add(self, embedding: FloatTensor, label: Optional[int] = None, data: Optional[Tensor] = None) -> int:
+    def add(self, embedding: FloatTensor, label: int | None = None, data: Tensor | None = None) -> int:
         """Add an Embedding record to the key value store.
 
         Args:
             embedding: Embedding predicted by the model.
 
             label: Class numerical id. Defaults to None.
 
@@ -34,17 +35,17 @@
             Associated record id.
         """
 
     @abstractmethod
     def batch_add(
         self,
         embeddings: Sequence[FloatTensor],
-        labels: Optional[Sequence[int]] = None,
-        data: Optional[Sequence[Tensor]] = None,
-    ) -> List[int]:
+        labels: Sequence[int] | None = None,
+        data: Sequence[Tensor] | None = None,
+    ) -> list[int]:
         """Add a set of embedding records to the key value store.
 
         Args:
             embeddings: Embeddings predicted by the model.
 
             labels: Class numerical ids. Defaults to None.
 
@@ -54,26 +55,26 @@
             add() for what a record contains.
 
         Returns:
             List of associated record id.
         """
 
     @abstractmethod
-    def get(self, idx: int) -> Tuple[FloatTensor, Optional[int], Optional[Tensor]]:
+    def get(self, idx: int) -> tuple[FloatTensor, int | None, Tensor | None]:
         """Get an embedding record from the key value store.
 
         Args:
             idx: Id of the record to fetch.
 
         Returns:
             record associated with the requested id.
         """
 
     @abstractmethod
-    def batch_get(self, idxs: Sequence[int]) -> Tuple[List[FloatTensor], List[Optional[int]], List[Optional[Tensor]]]:
+    def batch_get(self, idxs: Sequence[int]) -> tuple[list[FloatTensor], list[int | None], list[Tensor | None]]:
         """Get embedding records from the key value store.
 
         Args:
             idxs: ids of the records to fetch.
 
         Returns:
             List of records associated with the requested ids.
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/training_metrics/__init__.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/training_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/training_metrics/distance_metrics.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/training_metrics/distance_metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,34 +7,38 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 "Metrics computed over embeddings"
+from __future__ import annotations
+
+from typing import Any
+
 import tensorflow as tf
 from tensorflow.keras.metrics import Metric
 
 from tensorflow_similarity.algebra import build_masks, masked_max, masked_min
-from tensorflow_similarity.distances import distance_canonicalizer
+from tensorflow_similarity.distances import Distance, distance_canonicalizer
+from tensorflow_similarity.types import FloatTensor, IntTensor
 
 
 @tf.keras.utils.register_keras_serializable(package="Similarity")
 class DistanceMetric(Metric):
     def __init__(
         self,
-        distance,
-        aggregate="mean",
-        anchor="positive",
-        name=None,
-        positive_mining_strategy="hard",
-        negative_mining_strategy="hard",
-        **kwargs
+        distance: Distance | str,
+        aggregate: str = "mean",
+        anchor: str = "positive",
+        name: str | None = None,
+        positive_mining_strategy: str = "hard",
+        negative_mining_strategy: str = "hard",
+        **kwargs,
     ):
 
         if not name:
             name = "%s_%s" % (aggregate, anchor[:3])
         super().__init__(name=name, **kwargs)
 
         self.distance = distance_canonicalizer(distance)
@@ -52,17 +56,17 @@
         self.negative_mining_strategy = negative_mining_strategy
 
         if aggregate not in ["mean", "max", "avg", "min", "sum"]:
             raise ValueError("Invalid reduction")
         self.aggregate = aggregate
 
         # result variable
-        self.aggregated_distances = tf.Variable(0, dtype="float32")
+        self.aggregated_distances = tf.Variable(0, dtype=tf.keras.backend.floatx())
 
-    def update_state(self, labels, embeddings, sample_weight):
+    def update_state(self, labels: IntTensor, embeddings: FloatTensor, sample_weight: FloatTensor) -> None:
 
         # [distances]
         pairwise_distances = self.distance(embeddings, embeddings)
 
         # [mask]
         batch_size = tf.size(labels)
         positive_mask, negative_mask = build_masks(labels, labels, batch_size)
@@ -86,99 +90,99 @@
         elif self.aggregate == "min":
             aggregated_distances = tf.reduce_min(distances)
         elif self.aggregate == "sum":
             aggregated_distances = tf.reduce_sum(distances)
 
         self.aggregated_distances = aggregated_distances
 
-    def reset_state(self):
-        self.aggregated_distances = tf.Variable(0, dtype="float32")
+    def reset_state(self) -> None:
+        self.aggregated_distances = tf.Variable(0, dtype=tf.keras.backend.floatx())
 
-    def result(self):
+    def result(self) -> tf.Variable:
         return self.aggregated_distances
 
-    def get_config(self):
+    def get_config(self) -> dict[str, Any]:
         config = {
             "distance": self.distance.name,
             "aggregate": self.aggregate,
             "anchor": self.anchor,
             "positive_mining_strategy": self.positive_mining_strategy,
             "negative_mining_strategy": self.negative_mining_strategy,
         }
         base_config = super().get_config()
         return {**base_config, **config}
 
 
 @tf.keras.utils.register_keras_serializable(package="Similarity")
 class DistanceGapMetric(Metric):
-    def __init__(self, distance, name=None, **kwargs):
+    def __init__(self, distance: Distance | str, name: str | None = None, **kwargs):
         name = name if name else "dist_gap"
         super().__init__(name=name, **kwargs)
         self.distance = distance
         self.max_pos_fn = DistanceMetric(distance, aggregate="max")
         self.min_neg_fn = DistanceMetric(distance, aggregate="min", anchor="negative")
-        self.gap = tf.Variable(0, dtype="float32")
+        self.gap = tf.Variable(0, dtype=tf.keras.backend.floatx())
 
-    def update_state(self, labels, embeddings, sample_weight):
+    def update_state(self, labels: IntTensor, embeddings: FloatTensor, sample_weight: FloatTensor):
         max_pos = self.max_pos_fn(labels, embeddings, sample_weight)
         min_neg = self.min_neg_fn(labels, embeddings, sample_weight)
-        self.gap.assign(tf.abs(min_neg - max_pos))
+        self.gap.assign(tf.cast(tf.abs(min_neg - max_pos), tf.keras.backend.floatx()))
 
-    def result(self):
+    def result(self) -> tf.Variable:
         return self.gap
 
-    def get_config(self):
+    def get_config(self) -> dict[str, Any]:
         config = {
             "distance": self.distance,
         }
         base_config = super().get_config()
         return {**base_config, **config}
 
 
 # aliases
 @tf.keras.utils.register_keras_serializable(package="Similarity")
-def dist_gap(distance):
+def dist_gap(distance: Distance | str) -> DistanceGapMetric:
     return DistanceGapMetric(distance)
 
 
 # max
 @tf.keras.utils.register_keras_serializable(package="Similarity")
-def max_pos(distance):
+def max_pos(distance: Distance | str) -> DistanceMetric:
     return DistanceMetric(distance, aggregate="max")
 
 
 @tf.keras.utils.register_keras_serializable(package="Similarity")
-def max_neg(distance):
+def max_neg(distance: Distance | str) -> DistanceMetric:
     return DistanceMetric(distance, aggregate="max", anchor="negative")
 
 
 # avg
 @tf.keras.utils.register_keras_serializable(package="Similarity")
-def avg_pos(distance):
+def avg_pos(distance: Distance | str) -> DistanceGapMetric:
     return DistanceMetric(distance, aggregate="mean")
 
 
 @tf.keras.utils.register_keras_serializable(package="Similarity")
-def avg_neg(distance):
+def avg_neg(distance: Distance | str) -> DistanceMetric:
     return DistanceMetric(distance, aggregate="mean", anchor="negative")
 
 
 # min
 @tf.keras.utils.register_keras_serializable(package="Similarity")
-def min_pos(distance):
+def min_pos(distance: Distance | str) -> DistanceMetric:
     return DistanceMetric(distance, aggregate="min")
 
 
 @tf.keras.utils.register_keras_serializable(package="Similarity")
-def min_neg(distance):
+def min_neg(distance: Distance | str) -> DistanceMetric:
     return DistanceMetric(distance, aggregate="min", anchor="negative")
 
 
 # sum
 @tf.keras.utils.register_keras_serializable(package="Similarity")
-def sum_pos(distance):
+def sum_pos(distance: Distance | str) -> DistanceMetric:
     return DistanceMetric(distance, aggregate="sum")
 
 
 @tf.keras.utils.register_keras_serializable(package="Similarity")
-def sum_neg(distance):
+def sum_neg(distance: Distance | str) -> DistanceMetric:
     return DistanceMetric(distance, aggregate="sum", anchor="negative")
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/types.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Core TensorFlow types."""
+from __future__ import annotations
 
 import dataclasses
-from typing import Any, Callable, Mapping, Optional, Union
+from collections.abc import Mapping
+from typing import Any, Callable
 
 import numpy as np
 import tensorflow as tf
 from tensorflow import Tensor
 
 
 class PandasDataFrame(object):
@@ -106,17 +108,17 @@
 
         data: The original Tensor representation of the match result.
         Default None.
     """
 
     rank: int
     distance: float
-    label: Optional[int] = dataclasses.field(default=None)
-    embedding: Optional[np.ndarray] = dataclasses.field(default=None)
-    data: Optional[Tensor] = dataclasses.field(default=None)
+    label: int | None = dataclasses.field(default=None)
+    embedding: np.ndarray | None = dataclasses.field(default=None)
+    data: Tensor | None = dataclasses.field(default=None)
 
     def __eq__(self, other) -> bool:
         if other.__class__ is not self.__class__:
             return False
         if self.rank != other.rank:
             return False
         if self.distance != other.distance:
@@ -141,9 +143,9 @@
         threshold, e.g., 'optimal' : {'acc': 0.90, 'f1': 0.92}.
 
         thresholds: A Dict mapping ClassificationMetric names to a list
         containing the metric's value computed at each of the distance
         thresholds, e.g., {'f1': [0.99, 0.80], 'distance': [0.0, 1.0]}.
     """
 
-    cutpoints: Mapping[str, Mapping[str, Union[str, float]]]
+    cutpoints: Mapping[str, Mapping[str, str | float]]
     thresholds: Mapping[str, np.ndarray]
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/utils.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 "Various utilities functions for improved quality of life."
+from __future__ import annotations
+
 import math
-from typing import Dict, List, Optional, Sequence, Union
+from collections.abc import Mapping, MutableMapping, Sequence
+from typing import Any
 
 import numpy as np
 import tensorflow as tf
 
 from tensorflow_similarity.types import BoolTensor, FloatTensor, IntTensor, Lookup
 
 
@@ -35,15 +38,15 @@
             try:
                 tf.config.experimental.set_memory_growth(gpu, True)
             except RuntimeError as e:
                 # Memory growth must be set before GPUs have been initialized
                 print(e)
 
 
-def unpack_lookup_labels(lookups: Sequence[Sequence[Lookup]], dtype: Union[str, tf.DType]) -> IntTensor:
+def unpack_lookup_labels(lookups: Sequence[Sequence[Lookup]], dtype: str | tf.DType) -> IntTensor:
     # Using list comprehension as it is faster
     all_values = [[n.label for n in lu] for lu in lookups]
     # Lookup sets are not guaranteed to all be the same size. Therefore we load
     # the list of lists as a ragged tensor and convert to an int tensor with a
     # default class label value set to the max value for int.
     base_type = tf.dtypes.as_dtype(dtype).base_dtype
     ragged_labels = tf.ragged.constant(all_values, dtype=base_type)
@@ -57,15 +60,15 @@
 
     result: IntTensor = ragged_labels.to_tensor(default_value=0x7FFFFFFF)
 
     return result
 
 
 def unpack_lookup_distances(
-    lookups: Sequence[Sequence[Lookup]], dtype: Union[str, tf.DType], distance_rounding: Optional[int] = None
+    lookups: Sequence[Sequence[Lookup]], dtype: str | tf.DType, distance_rounding: int | None = None
 ) -> FloatTensor:
     # using list comprehension as it is faster
     all_values = [[n.distance for n in lu] for lu in lookups]
     # Lookup sets are not guaranteed to all be the same size. Therefore we load
     # the list of lists as a ragged tensor and convert to an flat32 tensor with a
     # default dist value set to math.inf.
     base_type = tf.dtypes.as_dtype(dtype).base_dtype
@@ -84,25 +87,25 @@
 
     dists: FloatTensor = ragged_dists.to_tensor(default_value=math.inf)
 
     return dists
 
 
 def unpack_results(
-    results: Dict[str, np.ndarray],
+    results: Mapping[str, np.ndarray],
     epoch: int,
-    logs: dict,
+    logs: MutableMapping[str, Any],
     tb_writer: tf.summary.SummaryWriter,
-    name_suffix: Optional[str] = "",
-) -> List[str]:
+    name_suffix: str | None = "",
+) -> list[str]:
     """Updates logs, writes summary, and returns list of strings of
     evaluation metric"""
     mstr = []
     for metric_name, vals in results.items():
-        float_val = vals[0]
+        float_val = vals[0] if isinstance(vals, np.ndarray) else vals
         full_metric_name = f"{metric_name}{name_suffix}"
         logs[full_metric_name] = float_val
         mstr.append(f"{full_metric_name}: {float_val:.4f}")
         if tb_writer:
             with tb_writer.as_default():
                 tf.summary.scalar(full_metric_name, float_val, step=epoch)
     return mstr
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/visualization/confusion_matrix_viz.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/visualization/confusion_matrix_viz.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,34 +7,36 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""Visualization utilities for TensorFlow Similarity."""
+from __future__ import annotations
 
 import itertools
-from typing import Any, Tuple
+from typing import Any
 
 import numpy as np
 import tensorflow as tf
 from matplotlib import pyplot as plt
 
 from tensorflow_similarity.types import FloatTensor, IntTensor
 
 
 def confusion_matrix(
     y_pred: IntTensor,
     y_true: IntTensor,
     normalize: bool = True,
-    labels: IntTensor = None,
+    labels: IntTensor | None = None,
     title: str = "Confusion matrix",
     cmap: str = "Blues",
     show: bool = True,
-) -> Tuple[Any, FloatTensor]:
+) -> tuple[Any, FloatTensor]:
     """Plot confusion matrix
 
     Args:
         y_pred: Model prediction returned by `model.match()`
 
         y_true: Expected class_id.
 
@@ -60,15 +62,15 @@
             y_pred = tf.convert_to_tensor(np.array(y_pred))
         y_pred = tf.cast(y_pred, dtype="int32")
         if not tf.is_tensor(y_true):
             y_true = tf.convert_to_tensor(np.array(y_true))
         y_true = tf.cast(y_true, dtype="int32")
 
         cm = tf.math.confusion_matrix(y_true, y_pred)
-        cm = tf.cast(cm, dtype="float")
+        cm = tf.cast(cm, dtype=tf.keras.backend.floatx())
         accuracy = tf.linalg.trace(cm) / tf.math.reduce_sum(cm)
         misclass = 1 - accuracy
 
         if normalize:
             cm = tf.math.divide_no_nan(cm, tf.math.reduce_sum(cm, axis=1)[:, np.newaxis])
 
         f, ax = plt.subplots(figsize=(8, 6))
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/visualization/neighbors_viz.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/visualization/neighbors_viz.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
-from typing import Mapping, Optional, Sequence, Tuple
+from collections.abc import Mapping, Sequence
 
 from matplotlib import pyplot as plt
 
 from tensorflow_similarity.types import Lookup, Tensor
 
 
 def viz_neigbors_imgs(
     example: Tensor,
     example_class: int,
     neighbors: Sequence[Lookup],
-    class_mapping: Optional[Mapping[int, str]] = None,
-    fig_size: Tuple[int, int] = (24, 4),
+    class_mapping: Mapping[int, str] | None = None,
+    fig_size: tuple[int, int] = (24, 4),
     cmap: str = "viridis",
     show: bool = True,
 ):
     """Display images nearest neighboors
 
     Args:
         example: The data used as query input.
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/visualization/projector.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/visualization/projector.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,30 +7,33 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
 import base64
 import io
-from typing import Any, List, Mapping, Optional, Sequence
+from collections.abc import Mapping, Sequence
+from typing import Any
 
 import numpy as np
 import PIL
 import umap
+from bokeh import __version__
 from bokeh.plotting import ColumnDataSource, figure, output_notebook, show
 from distinctipy import distinctipy
 from tqdm.auto import tqdm
 
 from tensorflow_similarity.types import FloatTensor, Tensor
 
 
-def tensor2images(tensor: Tensor, size: Optional[int] = 64) -> List[str]:
+def tensor2images(tensor: Tensor, size: int = 64) -> list[str]:
     """Convert tensor images back to in memory images
     encoded in base 64.
 
     Args:
         tensor: 4D tensor that represent an image list.
         size: Image size to output in pixels. Defaults to 64.
 
@@ -65,19 +68,19 @@
         imgs_b64.append(img64)
 
     return imgs_b64
 
 
 def projector(
     embeddings: FloatTensor,
-    labels: Optional[Sequence[Any]] = None,
-    class_mapping: Optional[Sequence[int]] = None,
-    images: Optional[Tensor] = None,
+    labels: Sequence[Any] | None = None,
+    class_mapping: Sequence[int] | None = None,
+    images: Tensor | None = None,
     image_size: int = 64,
-    tooltips_info: Optional[Mapping[str, Sequence[str]]] = None,
+    tooltips_info: Mapping[str, Sequence[str]] | None = None,
     pt_size: int = 3,
     colorize: bool = True,
     pastel_factor: float = 0.1,
     plot_size: int = 600,
     active_drag: str = "box_zoom",
     densmap: bool = True,
 ):
@@ -179,21 +182,31 @@
             tooltips += "%s:@%s <br>" % (k, k)
 
     tooltips += "Class:@labels_txt <br>ID:@id </div>"
 
     # to bokeh format
     source = ColumnDataSource(data=data)
     output_notebook()
-    fig = figure(
-        tooltips=tooltips,
-        plot_width=plot_size,
-        plot_height=plot_size,
-        active_drag=active_drag,
-        active_scroll="wheel_zoom",
-    )
+    # Bokeh backward compatibility
+    if int(__version__.split(".")[0]) >= 3:
+        fig = figure(
+            tooltips=tooltips,
+            width=plot_size,
+            height=plot_size,
+            active_drag=active_drag,
+            active_scroll="wheel_zoom",
+        )
+    else:
+        fig = figure(
+            tooltips=tooltips,
+            plot_width=plot_size,
+            plot_height=plot_size,
+            active_drag=active_drag,
+            active_scroll="wheel_zoom",
+        )
 
     # remove grid and axis
     fig.xaxis.visible = False
     fig.yaxis.visible = False
     fig.xgrid.visible = False
     fig.ygrid.visible = False
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity/visualization/vizualize_views.py` & `tensorflow_similarity-0.17.1/tensorflow_similarity/visualization/vizualize_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Tuple
+from __future__ import annotations
 
 import tensorflow as tf
 from matplotlib import pyplot as plt
 from tensorflow import Tensor
 
 
 def visualize_views(
     views: Tensor,
     labels: Tensor = None,
     predictions: Tensor = None,
-    num_imgs: int = None,
+    num_imgs: int | None = None,
     views_per_col: int = 4,
-    fig_size: Tuple[int, int] = (24, 4),
+    fig_size: tuple[int, int] = (24, 4),
     max_pixel_value: float = 1.0,
     min_pixel_value: float = 0.0,
 ):
     """Display side by side different image views with labels, and predictions
 
     Args:
         views: Aray of views
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity.egg-info/PKG-INFO` & `tensorflow_similarity-0.17.1/tensorflow_similarity.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow-similarity
-Version: 0.16.9
+Version: 0.17.1
 Summary: Metric Learning for Humans
 Home-page: https://github.com/tensorflow/similarity
 Author: Tensorflow Similarity authors
 Author-email: tf-similarity@google.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,27 +34,21 @@
 
 1. **Self-supervised models**: Used to learn general data representations on unlabeled data to boost the accuracy of downstream tasks where you have few labels. For example, you can pre-train a model on a large number of unlabled images using one of the supported contrastive methods supported by TensorFlow Similarity, and then fine-tune it on a small labeled dataset to achieve higher accuracy. To get started training your own self-supervised model see this [notebook](examples/unsupervised_hello_world.ipynb).
 
 2. **Similarity models**: Output embeddings that allow you to find and cluster similar examples such as images representing the same object within a large corpus of examples. For instance, as visible above, you can train a similarity model to find and cluster similar looking, unseen cat and dog images from the [Oxford IIIT Pet Dataset](https://www.tensorflow.org/datasets/catalog/oxford_iiit_pet) while only training on a few of the dataset classes. To get started training your own similarity model see this [notebook](examples/supervised/visualization.ipynb).
 
 ## What's new
 
-- [May 2022]: 0.16 major optimization release
-    * Cross-batch memory (XBM) loss added thank to @chjort
-    * Many self-supervised related improvement thanks to @dewball345
-    * Major layers and callback refactoring to make them faster and more flexible. E.g `EvalCallback()` now support splited validation.
-     For full changes see [the changelog](./releases.md)
-
-- [Jan 2022]: 0.15 self-supervised release
-    * Added support for self-supervised contrastive learning. Including SimCLR, SimSiam, and Barlow Twins. Checkout the in-depth [hello world notebook](examples/unsupervised_hello_world.ipynb) to get started.
-    * Soft Nearest Neighbor Loss added thanks to [Abhishar Sinha](https://github.com/abhisharsinha)
-    * Added GenerlizedMeanPooling2D support that improves similarity matching accuracy over GlobalMeanPooling2D.
-    * Numerous speed optimizations and general bug fixes.
+- [Mar 2032]: 0.17 more losses and metric and massive refactoring 
+   * Added VicReg Loss to contrastive losses.
+   * Added metrics used in retrieval papers such as Precision@K
+   * Native support for distributed training e.g SimClr now works correctly with distributed training.
+   * Multi-modal embedding initial support (CLIP)
 
-For previous changes and more details - see [the changelog](./releases.md)
+For more details and previous releases informaiton - see [the changelog](./releases.md)
 
 ## Getting Started
 
 ### Installation
 
 Use pip to install the library.
```

### Comparing `tensorflow_similarity-0.16.9/tensorflow_similarity.egg-info/SOURCES.txt` & `tensorflow_similarity-0.17.1/tensorflow_similarity.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 tensorflow_similarity/evaluators/__init__.py
 tensorflow_similarity/evaluators/evaluator.py
 tensorflow_similarity/evaluators/memory_evaluator.py
 tensorflow_similarity/losses/__init__.py
 tensorflow_similarity/losses/barlow.py
 tensorflow_similarity/losses/circle_loss.py
 tensorflow_similarity/losses/metric_loss.py
+tensorflow_similarity/losses/multinegrank_loss.py
 tensorflow_similarity/losses/multisim_loss.py
 tensorflow_similarity/losses/pn_loss.py
 tensorflow_similarity/losses/simclr.py
 tensorflow_similarity/losses/simsiam.py
 tensorflow_similarity/losses/softnn_loss.py
 tensorflow_similarity/losses/triplet_loss.py
 tensorflow_similarity/losses/utils.py
@@ -71,22 +72,25 @@
 tensorflow_similarity/retrieval_metrics/bndcg.py
 tensorflow_similarity/retrieval_metrics/map_at_k.py
 tensorflow_similarity/retrieval_metrics/precision_at_k.py
 tensorflow_similarity/retrieval_metrics/recall_at_k.py
 tensorflow_similarity/retrieval_metrics/retrieval_metric.py
 tensorflow_similarity/retrieval_metrics/utils.py
 tensorflow_similarity/samplers/__init__.py
+tensorflow_similarity/samplers/file_samplers.py
 tensorflow_similarity/samplers/memory_samplers.py
 tensorflow_similarity/samplers/samplers.py
+tensorflow_similarity/samplers/tfdata_sampler.py
 tensorflow_similarity/samplers/tfdataset_samplers.py
 tensorflow_similarity/samplers/tfrecords_samplers.py
 tensorflow_similarity/samplers/utils.py
 tensorflow_similarity/search/__init__.py
 tensorflow_similarity/search/nmslib_search.py
 tensorflow_similarity/search/search.py
+tensorflow_similarity/search/utils.py
 tensorflow_similarity/stores/__init__.py
 tensorflow_similarity/stores/memory_store.py
 tensorflow_similarity/stores/store.py
 tensorflow_similarity/training_metrics/__init__.py
 tensorflow_similarity/training_metrics/distance_metrics.py
 tensorflow_similarity/training_metrics/utils.py
 tensorflow_similarity/visualization/__init__.py
@@ -97,39 +101,48 @@
 tests/__init__.py
 tests/conftest.py
 tests/test_algebra.py
 tests/test_callbacks.py
 tests/test_distances.py
 tests/test_indexer.py
 tests/test_layers.py
-tests/test_losses.py
-tests/test_model.py
 tests/test_schedules.py
 tests/test_types.py
 tests/test_utils.py
 tests/architectures/__init__.py
 tests/architectures/test_efficientnet.py
 tests/architectures/test_resnet18.py
 tests/architectures/test_resnet50.py
 tests/classification_metrics/__init__.py
 tests/classification_metrics/test_classification_metrics.py
 tests/evaluators/__init__.py
 tests/evaluators/test_memory_evaluator.py
+tests/losses/__init__.py
+tests/losses/test_pn_loss.py
+tests/losses/test_softnn_loss.py
+tests/losses/test_triplet_loss.py
+tests/losses/test_xbm_loss.py
+tests/losses/utils.py
 tests/matchers/__init__.py
 tests/matchers/test_classification_match.py
 tests/matchers/test_majority_vote.py
 tests/matchers/test_match_nearest.py
+tests/models/__init__.py
+tests/models/test_contrastive_model.py
+tests/models/test_similarity_model.py
 tests/retrieval_metrics/__init__.py
 tests/retrieval_metrics/test_bndcg.py
 tests/retrieval_metrics/test_map_at_k.py
 tests/retrieval_metrics/test_precision_at_k.py
 tests/retrieval_metrics/test_recall_at_k.py
 tests/retrieval_metrics/test_retrieval_metric.py
 tests/samplers/__init__.py
+tests/samplers/test_file_samplers.py
 tests/samplers/test_memory_samplers.py
+tests/samplers/test_tfdata_sampler.py
 tests/samplers/test_tfdataset_samplers.py
 tests/samplers/test_tfrecord_samplers.py
 tests/search/__init__.py
 tests/search/test_nmslib_search.py
 tests/stores/__init__.py
 tests/stores/test_memory_store.py
 tests/training_metrics/__init__.py
```

### Comparing `tensorflow_similarity-0.16.9/tests/architectures/test_efficientnet.py` & `tensorflow_similarity-0.17.1/tests/architectures/test_efficientnet.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/architectures/test_resnet18.py` & `tensorflow_similarity-0.17.1/tests/architectures/test_resnet18.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/architectures/test_resnet50.py` & `tensorflow_similarity-0.17.1/tests/architectures/test_resnet50.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/classification_metrics/test_classification_metrics.py` & `tensorflow_similarity-0.17.1/tests/classification_metrics/test_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/evaluators/test_memory_evaluator.py` & `tensorflow_similarity-0.17.1/tests/evaluators/test_memory_evaluator.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/matchers/test_classification_match.py` & `tensorflow_similarity-0.17.1/tests/matchers/test_classification_match.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,22 +26,21 @@
         )
 
 
 def test_compile():
     cm = ConcreteClassificationMatch(name="foo", canonical_name="bar")
 
     # Pass distance_thresholds as a 1D tensor.
-    distance_thresholds = tf.constant([1, 2, 3, 4, 5, 6, 7])
+    distance_thresholds = tf.constant([1, 2, 3, 4, 5, 6, 7], dtype=tf.float32)
     cm.compile(distance_thresholds=distance_thresholds)
 
-    expected_dt = tf.cast(distance_thresholds, dtype="float32")
     assert cm.name == "foo"
     assert cm.canonical_name == "bar"
-    assert tf.math.reduce_all(tf.shape(cm.distance_thresholds) == tf.shape(expected_dt))
-    assert tf.math.reduce_all(tf.math.equal(cm.distance_thresholds, expected_dt))
+    assert tf.math.reduce_all(tf.shape(cm.distance_thresholds) == tf.shape(distance_thresholds))
+    assert tf.math.reduce_all(tf.math.equal(cm.distance_thresholds, distance_thresholds))
 
 
 def test_compute_match_indicators():
     cm = ConcreteClassificationMatch(name="foo", canonical_name="bar")
 
     # Pass distance_thresholds as a 1D tensor.
     distance_thresholds = tf.constant([1.0, 2.0])
```

### Comparing `tensorflow_similarity-0.16.9/tests/matchers/test_majority_vote.py` & `tensorflow_similarity-0.17.1/tests/matchers/test_majority_vote.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/matchers/test_match_nearest.py` & `tensorflow_similarity-0.17.1/tests/matchers/test_match_nearest.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/retrieval_metrics/test_bndcg.py` & `tensorflow_similarity-0.17.1/tests/retrieval_metrics/test_bndcg.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/retrieval_metrics/test_map_at_k.py` & `tensorflow_similarity-0.17.1/tests/retrieval_metrics/test_map_at_k.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     assert rm.distance_threshold == 0.1
     assert rm.average == "micro"
 
     expected_config = {
         "r": {1: 4, 0: 4},
         "name": "map@5 : distance_threshold@0.1",
         "canonical_name": "map@k",
+        "clip_at_r": False,
         "k": 5,
         "distance_threshold": 0.1,
     }
     assert rm.get_config() == expected_config
 
 
 def test_compute():
@@ -47,7 +48,32 @@
     #     (1.0*True+1.0*True+0.66*False)/3 = 0.66667
     # class 0 has 1 result set that is F,F,T
     #     (0.0*False+0.0*False+0.33*True)/10 = 0.03332
     # mapk = (0.667*3 + 0.0332)/4
     expected = tf.constant(0.50833333332)
 
     np.testing.assert_allclose(mapk, expected)
+
+
+def test_clip_at_r():
+    query_labels = tf.constant([0, 1])
+    match_mask = tf.constant(
+        [
+            [False, False, False, True],
+            [False, False, False, True],
+        ],
+        dtype=bool,
+    )
+    rm = MapAtK(r={0: 4, 1: 3}, k=4, clip_at_r=True)
+
+    mapk = rm.compute(query_labels=query_labels, match_mask=match_mask)
+
+    # mapk should be sum(precision@k*Relevancy_Mask)/R
+    # but here we clip the result set at the r associate with the query label.
+    # class 0 has 1 result set of F,F,F,T with R == 4
+    #     (0.0*False+0.0*False+0.0*False)/3 = 0.0
+    # class 1 has 1 result set of F,F,F,T with R == 3
+    #     (0.0*False+0.0*False+0.0*False+0.25*True)/4 = 0.0625
+    # mapk = (0.0 + 0.0625)/2
+    expected = tf.constant(0.03125)
+
+    np.testing.assert_allclose(mapk, expected)
```

### Comparing `tensorflow_similarity-0.16.9/tests/retrieval_metrics/test_precision_at_k.py` & `tensorflow_similarity-0.17.1/tests/retrieval_metrics/test_precision_at_k.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/retrieval_metrics/test_recall_at_k.py` & `tensorflow_similarity-0.17.1/tests/retrieval_metrics/test_recall_at_k.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/retrieval_metrics/test_retrieval_metric.py` & `tensorflow_similarity-0.17.1/tests/retrieval_metrics/test_retrieval_metric.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/samplers/test_memory_samplers.py` & `tensorflow_similarity-0.17.1/tests/samplers/test_memory_samplers.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/samplers/test_tfdataset_samplers.py` & `tensorflow_similarity-0.17.1/tests/samplers/test_tfdataset_samplers.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/samplers/test_tfrecord_samplers.py` & `tensorflow_similarity-0.17.1/tests/samplers/test_tfrecord_samplers.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/search/test_nmslib_search.py` & `tensorflow_similarity-0.17.1/tests/search/test_nmslib_search.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/stores/test_memory_store.py` & `tensorflow_similarity-0.17.1/tests/stores/test_memory_store.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/test_algebra.py` & `tensorflow_similarity-0.17.1/tests/test_algebra.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/test_callbacks.py` & `tensorflow_similarity-0.17.1/tests/test_callbacks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 
 import numpy as np
 import tensorflow as tf
 
-from tensorflow_similarity.callbacks import EvalCallback, SplitValidationLoss
+from tensorflow_similarity.callbacks import EvalCallback
 from tensorflow_similarity.classification_metrics import Recall
 from tensorflow_similarity.evaluators import MemoryEvaluator
 from tensorflow_similarity.models import SimilarityModel
 
 
 def test_eval_init_defaults():
     queries = tf.constant([[1.0, 2.0], [3.0, 4.0]])
@@ -24,15 +24,15 @@
 
     assert tf.math.reduce_all(callback.queries_known == queries)
     assert tf.math.reduce_all(callback.query_labels_known == query_labels)
     assert tf.math.reduce_all(callback.targets == targets)
     assert tf.math.reduce_all(callback.target_labels == target_labels)
     assert callback.distance == "cosine"
     assert isinstance(callback.evaluator, MemoryEvaluator)
-    assert {"binary_accuracy", "f1score"} == set([m.name for m in callback.metrics])
+    assert {"binary_accuracy"} == set([m.name for m in callback.classification_metrics])
     assert callback.k == 1
     assert tf.math.reduce_all(callback.distance_thresholds == tf.constant([math.inf]))
     assert callback.matcher == "match_nearest"
     assert callback.tb_writer is None
 
 
 def test_eval_init(tmp_path):
@@ -65,15 +65,15 @@
 
     assert tf.math.reduce_all(callback.queries_known == queries)
     assert tf.math.reduce_all(callback.query_labels_known == query_labels)
     assert tf.math.reduce_all(callback.targets == targets)
     assert tf.math.reduce_all(callback.target_labels == target_labels)
     assert callback.distance == "l2"
     assert isinstance(callback.evaluator, MemoryEvaluator)
-    assert {"recall"} == set([m.name for m in callback.metrics])
+    assert {"recall"} == set([m.name for m in callback.classification_metrics])
     assert callback.k == 11
     assert tf.math.reduce_all(callback.distance_thresholds == distance_thresholds)
     assert callback.matcher == "majority_vote"
     assert isinstance(callback.tb_writer, tf.summary.SummaryWriter)
 
 
 def test_eval_callback(tmp_path):
@@ -88,14 +88,15 @@
 
     callback = EvalCallback(
         queries=queries,
         query_labels=query_labels,
         targets=targets,
         target_labels=target_labels,
         tb_logdir=str(log_dir),
+        metrics=["binary_accuracy", "f1score"],
     )
 
     # manually set model ^^
     tf.keras.backend.clear_session()
     inputs = tf.keras.layers.Input(shape=(2,))
     outputs = tf.keras.layers.Dense(2)(inputs)
     model = SimilarityModel(inputs, outputs)
@@ -118,27 +119,27 @@
     target_labels = tf.constant([1, 2])
     known_classes = tf.constant([1])
     q_known = tf.constant([[1.0, 2.0]])
     q_label_known = tf.constant([1], dtype="int32")
     q_unknown = tf.constant([[3.0, 4.0]])
     q_label_unknown = tf.constant([2], dtype="int32")
 
-    callback = SplitValidationLoss(
+    callback = EvalCallback(
         queries=queries,
         query_labels=query_labels,
         targets=targets,
         target_labels=target_labels,
         known_classes=known_classes,
     )
 
     assert tf.math.reduce_all(callback.targets == targets)
     assert tf.math.reduce_all(callback.target_labels == target_labels)
     assert callback.distance == "cosine"
     assert isinstance(callback.evaluator, MemoryEvaluator)
-    assert {"binary_accuracy", "f1score"} == set([m.name for m in callback.metrics])
+    assert {"binary_accuracy"} == set([m.name for m in callback.classification_metrics])
     assert callback.k == 1
     assert tf.math.reduce_all(callback.distance_thresholds == tf.constant([math.inf]))
     assert callback.matcher == "match_nearest"
     assert callback.tb_writer is None
 
     assert tf.math.reduce_all(callback.queries_known == q_known)
     assert tf.math.reduce_all(callback.query_labels_known == q_label_known)
@@ -162,15 +163,15 @@
     q_unknown = tf.constant([[3.0, 4.0]])
     q_label_unknown = tf.constant([2], dtype="int32")
 
     log_dir = tmp_path / "sec/"
     if not log_dir.exists():
         log_dir.mkdir(parents=True)
 
-    callback = SplitValidationLoss(
+    callback = EvalCallback(
         queries=queries,
         query_labels=query_labels,
         targets=targets,
         target_labels=target_labels,
         known_classes=known_classes,
         distance=distance,
         metrics=metrics,
@@ -180,15 +181,15 @@
         tb_logdir=log_dir,
     )
 
     assert tf.math.reduce_all(callback.targets == targets)
     assert tf.math.reduce_all(callback.target_labels == target_labels)
     assert callback.distance == "l2"
     assert isinstance(callback.evaluator, MemoryEvaluator)
-    assert {"recall"} == set([m.name for m in callback.metrics])
+    assert {"recall"} == set([m.name for m in callback.classification_metrics])
     assert callback.k == 11
     assert tf.math.reduce_all(callback.distance_thresholds == distance_thresholds)
     assert callback.matcher == "majority_vote"
     assert isinstance(callback.tb_writer, tf.summary.SummaryWriter)
 
     assert tf.math.reduce_all(callback.queries_known == q_known)
     assert tf.math.reduce_all(callback.query_labels_known == q_label_known)
@@ -203,15 +204,15 @@
     target_labels = tf.constant([1, 2])
     known_classes = tf.constant([1])
 
     log_dir = tmp_path / "sec/"
     if not log_dir.exists():
         log_dir.mkdir(parents=True)
 
-    callback = SplitValidationLoss(
+    callback = EvalCallback(
         queries=queries,
         query_labels=query_labels,
         targets=targets,
         target_labels=target_labels,
         known_classes=known_classes,
         tb_logdir=str(log_dir),
     )
@@ -262,15 +263,15 @@
         tb_logdir=log_dir,
     )
 
     assert tf.math.reduce_all(callback.targets == targets)
     assert tf.math.reduce_all(callback.target_labels == target_labels)
     assert callback.distance == "l2"
     assert isinstance(callback.evaluator, MemoryEvaluator)
-    assert {"recall"} == set([m.name for m in callback.metrics])
+    assert {"recall"} == set([m.name for m in callback.classification_metrics])
     assert callback.k == 11
     assert tf.math.reduce_all(callback.distance_thresholds == distance_thresholds)
     assert callback.matcher == "majority_vote"
     assert isinstance(callback.tb_writer, tf.summary.SummaryWriter)
 
     assert tf.math.reduce_all(callback.queries_known == q_known)
     assert tf.math.reduce_all(callback.query_labels_known == q_label_known)
```

### Comparing `tensorflow_similarity-0.16.9/tests/test_distances.py` & `tensorflow_similarity-0.17.1/tests/test_distances.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/test_indexer.py` & `tensorflow_similarity-0.17.1/tests/test_indexer.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/test_layers.py` & `tensorflow_similarity-0.17.1/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/test_types.py` & `tensorflow_similarity-0.17.1/tests/test_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,11 @@
-import random
-
-import numpy as np
 import tensorflow as tf
 
 from tensorflow_similarity import types
 
-random.seed(303)
-np.random.seed(606)
-tf.random.set_seed(808)
-
 
 def basic_lookup(rank=1, distance=0.1):
     return types.Lookup(rank=rank, distance=distance)
 
 
 def label_lookup(label=10):
     return types.Lookup(rank=1, distance=0.1, label=label)
@@ -60,27 +53,27 @@
     def test_optional_label_lookup_not_eq(self):
         l1 = label_lookup()
         l2 = label_lookup(label=None)
 
         self.assertNotEqual(l1, l2)
 
     def test_embedding_lookup_eq(self):
-        l1 = embedding_lookup(embedding=np.ones((1, 512)))
-        l2 = embedding_lookup(embedding=np.ones((1, 512)))
+        l1 = embedding_lookup(embedding=tf.ones((1, 512)))
+        l2 = embedding_lookup(embedding=tf.ones((1, 512)))
 
         self.assertEqual(l1, l2)
 
     def test_embedding_lookup_not_eq(self):
-        l1 = embedding_lookup(embedding=np.ones((1, 512)))
-        l2 = embedding_lookup(embedding=np.ones((1, 512)) + 1)
+        l1 = embedding_lookup(embedding=tf.ones((1, 512)))
+        l2 = embedding_lookup(embedding=tf.ones((1, 512)) + 1)
 
         self.assertNotEqual(l1, l2)
 
     def test_optional_embedding_lookup_not_eq(self):
-        l1 = embedding_lookup(embedding=np.ones((1, 512)))
+        l1 = embedding_lookup(embedding=tf.ones((1, 512)))
         l2 = embedding_lookup(embedding=None)
 
         self.assertNotEqual(l1, l2)
 
     def test_data_lookup_eq(self):
         l1 = data_lookup(data=tf.constant("foo"))
         l2 = data_lookup(data=tf.constant("foo"))
```

### Comparing `tensorflow_similarity-0.16.9/tests/test_utils.py` & `tensorflow_similarity-0.17.1/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,23 @@
         lookups.append(lookup_set)
 
     return lookups
 
 
 class UtilsTest(tf.test.TestCase):
     def setUp(self):
+        super().setUp()
+        # the lookups collection may be modified by the tests, so it must be
+        # created in setUp before each test.
         self.lookups = create_lookups()
 
+    def tearDown(self):
+        super().tearDown()
+        del self.lookups
+
     def test_tf_cap_memory_gpu_exists(self):
         tf.config.experimental.list_physical_devices = MagicMock(return_value=["foo"])
         tf.config.experimental.set_memory_growth = MagicMock()
 
         utils.tf_cap_memory()
         tf.config.experimental.set_memory_growth.assert_called_with("foo", True)
```

### Comparing `tensorflow_similarity-0.16.9/tests/training_metrics/test_distance_metrics.py` & `tensorflow_similarity-0.17.1/tests/training_metrics/test_distance_metrics.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/visualization/test_confusion_matrix.py` & `tensorflow_similarity-0.17.1/tests/visualization/test_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `tensorflow_similarity-0.16.9/tests/visualization/test_neighbors_viz.py` & `tensorflow_similarity-0.17.1/tests/visualization/test_neighbors_viz.py`

 * *Files identical despite different names*

