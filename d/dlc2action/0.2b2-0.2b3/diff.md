# Comparing `tmp/dlc2action-0.2b2.tar.gz` & `tmp/dlc2action-0.2b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlc2action-0.2b2.tar", last modified: Thu Nov 24 11:56:55 2022, max compression
+gzip compressed data, was "dlc2action-0.2b3.tar", last modified: Tue May 30 22:00:26 2023, max compression
```

## Comparing `dlc2action-0.2b2.tar` & `dlc2action-0.2b3.tar`

### file list

```diff
@@ -1,100 +1,121 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-24 11:56:55.704796 dlc2action-0.2b2/
--rw-r--r--   0 alex       (501) staff       (20)      345 2022-11-22 19:51:16.000000 dlc2action-0.2b2/LICENSE.yml
--rw-r--r--   0 alex       (501) staff       (20)       42 2022-11-22 19:51:16.000000 dlc2action-0.2b2/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)     2570 2022-11-22 19:51:16.000000 dlc2action-0.2b2/NOTICE.yml
--rw-r--r--   0 alex       (501) staff       (20)     3682 2022-11-24 11:56:55.704491 dlc2action-0.2b2/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     3207 2022-11-24 11:55:00.000000 dlc2action-0.2b2/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-24 11:56:55.685992 dlc2action-0.2b2/dlc2action/
--rw-r--r--   0 alex       (501) staff       (20)    17139 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-24 11:56:55.687671 dlc2action-0.2b2/dlc2action/config/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-24 11:56:55.688780 dlc2action-0.2b2/dlc2action/config/annotation/
--rw-r--r--   0 alex       (501) staff       (20)     1242 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/annotation/boris.yaml
--rw-r--r--   0 alex       (501) staff       (20)       58 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/annotation/calms21.yaml
--rw-r--r--   0 alex       (501) staff       (20)     1525 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/annotation/csv.yaml
--rw-r--r--   0 alex       (501) staff       (20)     1536 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/annotation/dlc.yaml
--rw-r--r--   0 alex       (501) staff       (20)      589 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/annotation/pku-mmd.yaml
--rw-r--r--   0 alex       (501) staff       (20)     1392 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/annotation/simba.yaml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-24 11:56:55.689119 dlc2action-0.2b2/dlc2action/config/augmentations/
--rw-r--r--   0 alex       (501) staff       (20)      208 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/augmentations/heatmap.yaml
--rw-r--r--   0 alex       (501) staff       (20)      802 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/augmentations/kinematic.yaml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-24 11:56:55.690494 dlc2action-0.2b2/dlc2action/config/data/
--rw-r--r--   0 alex       (501) staff       (20)      137 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/data/calms21.yaml
--rw-r--r--   0 alex       (501) staff       (20)      425 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/data/clip.yaml
--rw-r--r--   0 alex       (501) staff       (20)      834 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/data/dlc_track.yaml
--rw-r--r--   0 alex       (501) staff       (20)      920 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/data/dlc_tracklet.yaml
--rw-r--r--   0 alex       (501) staff       (20)      374 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/data/features.yaml
--rw-r--r--   0 alex       (501) staff       (20)      650 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/data/np_3d.yaml
--rw-r--r--   0 alex       (501) staff       (20)       52 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/data/pku-mmd.yaml
--rw-r--r--   0 alex       (501) staff       (20)     1028 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/data/simba.yaml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-24 11:56:55.690884 dlc2action-0.2b2/dlc2action/config/features/
--rw-r--r--   0 alex       (501) staff       (20)      461 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/features/heatmap.yaml
--rw-r--r--   0 alex       (501) staff       (20)     1962 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/features/kinematic.yaml
--rw-r--r--   0 alex       (501) staff       (20)     1119 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/general.yaml
--rw-r--r--   0 alex       (501) staff       (20)      260 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/losses.yaml
--rw-r--r--   0 alex       (501) staff       (20)     6533 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/metrics.yaml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-24 11:56:55.691716 dlc2action-0.2b2/dlc2action/config/model/
--rw-r--r--   0 alex       (501) staff       (20)      343 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/model/asformer.yaml
--rw-r--r--   0 alex       (501) staff       (20)      349 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/model/c2f_tcn.yaml
--rw-r--r--   0 alex       (501) staff       (20)      214 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/model/edtcn.yaml
--rw-r--r--   0 alex       (501) staff       (20)      344 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/model/mlp.yaml
--rw-r--r--   0 alex       (501) staff       (20)      284 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/model/transformer.yaml
--rw-r--r--   0 alex       (501) staff       (20)     3925 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/ssl.yaml
--rw-r--r--   0 alex       (501) staff       (20)     2840 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/config/training.yaml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-24 11:56:55.693740 dlc2action-0.2b2/dlc2action/data/
--rw-r--r--   0 alex       (501) staff       (20)     3555 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/data/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    90455 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/data/annotation_store.py
--rw-r--r--   0 alex       (501) staff       (20)    20454 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/data/base_store.py
--rw-r--r--   0 alex       (501) staff       (20)    69439 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/data/dataset.py
--rw-r--r--   0 alex       (501) staff       (20)   101462 2022-11-24 11:53:01.000000 dlc2action-0.2b2/dlc2action/data/input_store.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-24 11:56:55.694688 dlc2action-0.2b2/dlc2action/feature_extraction/
--rw-r--r--   0 alex       (501) staff       (20)    30111 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/feature_extraction/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-24 11:56:55.696616 dlc2action-0.2b2/dlc2action/loss/
--rw-r--r--   0 alex       (501) staff       (20)     1004 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/loss/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     6373 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/loss/contrastive.py
--rw-r--r--   0 alex       (501) staff       (20)     2558 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/loss/contrastive_frame.py
--rw-r--r--   0 alex       (501) staff       (20)     6934 2022-11-24 11:53:01.000000 dlc2action-0.2b2/dlc2action/loss/ms_tcn.py
--rw-r--r--   0 alex       (501) staff       (20)     1090 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/loss/mse.py
--rw-r--r--   0 alex       (501) staff       (20)    12637 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/loss/tcc.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-24 11:56:55.697197 dlc2action-0.2b2/dlc2action/metric/
--rw-r--r--   0 alex       (501) staff       (20)      356 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/metric/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2229 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/metric/base_metric.py
--rw-r--r--   0 alex       (501) staff       (20)    77572 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/metric/metrics.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-24 11:56:55.698916 dlc2action-0.2b2/dlc2action/model/
--rw-r--r--   0 alex       (501) staff       (20)      760 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/model/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    18380 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/model/asformer.py
--rw-r--r--   0 alex       (501) staff       (20)    11072 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/model/base_model.py
--rw-r--r--   0 alex       (501) staff       (20)     8419 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/model/c2f_tcn.py
--rw-r--r--   0 alex       (501) staff       (20)     5800 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/model/edtcn.py
--rw-r--r--   0 alex       (501) staff       (20)     2215 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/model/mlp.py
--rw-r--r--   0 alex       (501) staff       (20)     8697 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/model/transformer.py
--rw-r--r--   0 alex       (501) staff       (20)     9105 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/options.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-24 11:56:55.699795 dlc2action-0.2b2/dlc2action/project/
--rw-r--r--   0 alex       (501) staff       (20)     4193 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/project/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    38237 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/project/meta.py
--rw-r--r--   0 alex       (501) staff       (20)   196136 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/project/project.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-24 11:56:55.702419 dlc2action-0.2b2/dlc2action/ssl/
--rw-r--r--   0 alex       (501) staff       (20)     2221 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/ssl/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     4080 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/ssl/base_ssl.py
--rw-r--r--   0 alex       (501) staff       (20)    11358 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/ssl/contrastive.py
--rw-r--r--   0 alex       (501) staff       (20)    12879 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/ssl/masked.py
--rw-r--r--   0 alex       (501) staff       (20)     7370 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/ssl/modules.py
--rw-r--r--   0 alex       (501) staff       (20)     6599 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/ssl/segment_order.py
--rw-r--r--   0 alex       (501) staff       (20)     2810 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/ssl/tcc.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-24 11:56:55.703050 dlc2action-0.2b2/dlc2action/task/
--rw-r--r--   0 alex       (501) staff       (20)      616 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/task/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    53576 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/task/task_dispatcher.py
--rw-r--r--   0 alex       (501) staff       (20)    78258 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/task/universal_task.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-24 11:56:55.704145 dlc2action-0.2b2/dlc2action/transformer/
--rw-r--r--   0 alex       (501) staff       (20)      937 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/transformer/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    19218 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/transformer/base_transformer.py
--rw-r--r--   0 alex       (501) staff       (20)    22177 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/transformer/kinematic.py
--rw-r--r--   0 alex       (501) staff       (20)    26365 2022-11-22 19:51:16.000000 dlc2action-0.2b2/dlc2action/utils.py
--rw-r--r--   0 alex       (501) staff       (20)      303 2022-11-24 11:55:00.000000 dlc2action-0.2b2/dlc2action/version.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-24 11:56:55.686756 dlc2action-0.2b2/dlc2action.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     3682 2022-11-24 11:56:55.000000 dlc2action-0.2b2/dlc2action.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     2488 2022-11-24 11:56:55.000000 dlc2action-0.2b2/dlc2action.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2022-11-24 11:56:55.000000 dlc2action-0.2b2/dlc2action.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)      299 2022-11-24 11:56:55.000000 dlc2action-0.2b2/dlc2action.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       11 2022-11-24 11:56:55.000000 dlc2action-0.2b2/dlc2action.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2022-11-24 11:56:55.704905 dlc2action-0.2b2/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)     1357 2022-11-24 11:55:00.000000 dlc2action-0.2b2/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:26.018926 dlc2action-0.2b3/
+-rw-r--r--   0 alex       (501) staff       (20)      348 2023-01-15 18:11:41.000000 dlc2action-0.2b3/LICENSE.yml
+-rw-r--r--   0 alex       (501) staff       (20)       42 2022-11-22 19:51:16.000000 dlc2action-0.2b3/MANIFEST.in
+-rw-r--r--   0 alex       (501) staff       (20)     2588 2023-01-15 18:11:37.000000 dlc2action-0.2b3/NOTICE.yml
+-rw-r--r--   0 alex       (501) staff       (20)     3708 2023-05-30 22:00:26.018708 dlc2action-0.2b3/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     3236 2023-05-30 21:55:12.000000 dlc2action-0.2b3/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:25.995539 dlc2action-0.2b3/dlc2action/
+-rw-r--r--   0 alex       (501) staff       (20)    17142 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:25.997609 dlc2action-0.2b3/dlc2action/config/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:25.998767 dlc2action-0.2b3/dlc2action/config/annotation/
+-rw-r--r--   0 alex       (501) staff       (20)     1242 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/annotation/boris.yaml
+-rw-r--r--   0 alex       (501) staff       (20)       58 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/annotation/calms21.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     1525 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/annotation/csv.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     1536 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/annotation/dlc.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      589 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/annotation/pku-mmd.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     1392 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/annotation/simba.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:25.999099 dlc2action-0.2b3/dlc2action/config/augmentations/
+-rw-r--r--   0 alex       (501) staff       (20)      208 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/augmentations/heatmap.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      802 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/augmentations/kinematic.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:26.000673 dlc2action-0.2b3/dlc2action/config/data/
+-rw-r--r--   0 alex       (501) staff       (20)      137 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/data/calms21.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      425 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/data/clip.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      834 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/data/dlc_track.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      920 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/data/dlc_tracklet.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      374 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/data/features.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      650 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/data/np_3d.yaml
+-rw-r--r--   0 alex       (501) staff       (20)       52 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/data/pku-mmd.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     1028 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/data/simba.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:26.001053 dlc2action-0.2b3/dlc2action/config/features/
+-rw-r--r--   0 alex       (501) staff       (20)      461 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/features/heatmap.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     1962 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/features/kinematic.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     1119 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/general.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      260 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/losses.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     6533 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/metrics.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:26.002496 dlc2action-0.2b3/dlc2action/config/model/
+-rw-r--r--   0 alex       (501) staff       (20)      343 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/model/asformer.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      349 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/model/c2f_tcn.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      214 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/model/edtcn.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      344 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/model/mlp.yaml
+-rw-r--r--   0 alex       (501) staff       (20)      284 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/model/transformer.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     3925 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/ssl.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     2840 2022-11-22 19:51:16.000000 dlc2action-0.2b3/dlc2action/config/training.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:26.004872 dlc2action-0.2b3/dlc2action/data/
+-rw-r--r--   0 alex       (501) staff       (20)     3558 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/data/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    90452 2023-05-30 21:51:11.000000 dlc2action-0.2b3/dlc2action/data/annotation_store.py
+-rw-r--r--   0 alex       (501) staff       (20)    20457 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/data/base_store.py
+-rw-r--r--   0 alex       (501) staff       (20)    69442 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/data/dataset.py
+-rw-r--r--   0 alex       (501) staff       (20)   101465 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/data/input_store.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:26.005644 dlc2action-0.2b3/dlc2action/feature_extraction/
+-rw-r--r--   0 alex       (501) staff       (20)    30114 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/feature_extraction/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:26.007221 dlc2action-0.2b3/dlc2action/loss/
+-rw-r--r--   0 alex       (501) staff       (20)     1007 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/loss/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     6376 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/loss/contrastive.py
+-rw-r--r--   0 alex       (501) staff       (20)     2561 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/loss/contrastive_frame.py
+-rw-r--r--   0 alex       (501) staff       (20)     6937 2023-01-15 18:11:44.000000 dlc2action-0.2b3/dlc2action/loss/ms_tcn.py
+-rw-r--r--   0 alex       (501) staff       (20)     1093 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/loss/mse.py
+-rw-r--r--   0 alex       (501) staff       (20)    12640 2023-01-15 18:11:44.000000 dlc2action-0.2b3/dlc2action/loss/tcc.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:26.007921 dlc2action-0.2b3/dlc2action/metric/
+-rw-r--r--   0 alex       (501) staff       (20)      359 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/metric/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2232 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/metric/base_metric.py
+-rw-r--r--   0 alex       (501) staff       (20)    77575 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/metric/metrics.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:26.010155 dlc2action-0.2b3/dlc2action/model/
+-rw-r--r--   0 alex       (501) staff       (20)      763 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/model/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    18383 2023-01-15 18:11:44.000000 dlc2action-0.2b3/dlc2action/model/asformer.py
+-rw-r--r--   0 alex       (501) staff       (20)    11075 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/model/base_model.py
+-rw-r--r--   0 alex       (501) staff       (20)     8422 2023-01-15 18:11:44.000000 dlc2action-0.2b3/dlc2action/model/c2f_tcn.py
+-rw-r--r--   0 alex       (501) staff       (20)     5803 2023-01-15 18:11:44.000000 dlc2action-0.2b3/dlc2action/model/edtcn.py
+-rw-r--r--   0 alex       (501) staff       (20)     2218 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/model/mlp.py
+-rw-r--r--   0 alex       (501) staff       (20)     8700 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/model/transformer.py
+-rw-r--r--   0 alex       (501) staff       (20)     9108 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/options.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:26.010890 dlc2action-0.2b3/dlc2action/project/
+-rw-r--r--   0 alex       (501) staff       (20)     4196 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/project/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    38238 2023-05-30 21:51:11.000000 dlc2action-0.2b3/dlc2action/project/meta.py
+-rw-r--r--   0 alex       (501) staff       (20)   196092 2023-05-30 21:51:11.000000 dlc2action-0.2b3/dlc2action/project/project.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:26.012903 dlc2action-0.2b3/dlc2action/ssl/
+-rw-r--r--   0 alex       (501) staff       (20)     2224 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/ssl/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     4083 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/ssl/base_ssl.py
+-rw-r--r--   0 alex       (501) staff       (20)    11361 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/ssl/contrastive.py
+-rw-r--r--   0 alex       (501) staff       (20)    12882 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/ssl/masked.py
+-rw-r--r--   0 alex       (501) staff       (20)     7373 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/ssl/modules.py
+-rw-r--r--   0 alex       (501) staff       (20)     6602 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/ssl/segment_order.py
+-rw-r--r--   0 alex       (501) staff       (20)     2813 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/ssl/tcc.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:26.014013 dlc2action-0.2b3/dlc2action/task/
+-rw-r--r--   0 alex       (501) staff       (20)      619 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/task/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    53579 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/task/task_dispatcher.py
+-rw-r--r--   0 alex       (501) staff       (20)    78261 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/task/universal_task.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:26.014733 dlc2action-0.2b3/dlc2action/transformer/
+-rw-r--r--   0 alex       (501) staff       (20)      940 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/transformer/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    19221 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/transformer/base_transformer.py
+-rw-r--r--   0 alex       (501) staff       (20)    22180 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/transformer/kinematic.py
+-rw-r--r--   0 alex       (501) staff       (20)    26368 2023-01-15 18:11:43.000000 dlc2action-0.2b3/dlc2action/utils.py
+-rw-r--r--   0 alex       (501) staff       (20)      306 2023-05-30 21:55:12.000000 dlc2action-0.2b3/dlc2action/version.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:25.996466 dlc2action-0.2b3/dlc2action.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     3708 2023-05-30 22:00:25.000000 dlc2action-0.2b3/dlc2action.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     3027 2023-05-30 22:00:25.000000 dlc2action-0.2b3/dlc2action.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-05-30 22:00:25.000000 dlc2action-0.2b3/dlc2action.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)      299 2023-05-30 22:00:25.000000 dlc2action-0.2b3/dlc2action.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       11 2023-05-30 22:00:25.000000 dlc2action-0.2b3/dlc2action.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-05-30 22:00:26.018977 dlc2action-0.2b3/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)     1350 2023-05-30 21:56:52.000000 dlc2action-0.2b3/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-30 22:00:26.018450 dlc2action-0.2b3/tests/
+-rw-r--r--   0 alex       (501) staff       (20)     2653 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_average_evaluation.py
+-rw-r--r--   0 alex       (501) staff       (20)     5778 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_dataset_loading.py
+-rw-r--r--   0 alex       (501) staff       (20)     2485 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_delete_datasets.py
+-rw-r--r--   0 alex       (501) staff       (20)     2645 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_episodes_export.py
+-rw-r--r--   0 alex       (501) staff       (20)     5088 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_find_valleys.py
+-rw-r--r--   0 alex       (501) staff       (20)     1646 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_full_length_prediction.py
+-rw-r--r--   0 alex       (501) staff       (20)     3429 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_loading_parameters.py
+-rw-r--r--   0 alex       (501) staff       (20)     2547 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_losses.py
+-rw-r--r--   0 alex       (501) staff       (20)     3519 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_metrics.py
+-rw-r--r--   0 alex       (501) staff       (20)     1980 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_partition.py
+-rw-r--r--   0 alex       (501) staff       (20)     3102 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_prediction.py
+-rw-r--r--   0 alex       (501) staff       (20)     3930 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_project_fill.py
+-rw-r--r--   0 alex       (501) staff       (20)     2245 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_project_list.py
+-rw-r--r--   0 alex       (501) staff       (20)     1886 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_pruning.py
+-rw-r--r--   0 alex       (501) staff       (20)     1948 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_search.py
+-rw-r--r--   0 alex       (501) staff       (20)     2388 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_ssl.py
+-rw-r--r--   0 alex       (501) staff       (20)     4644 2023-05-30 21:51:11.000000 dlc2action-0.2b3/tests/test_task_creation.py
+-rw-r--r--   0 alex       (501) staff       (20)     7410 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_task_update.py
+-rw-r--r--   0 alex       (501) staff       (20)     2016 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_training.py
+-rw-r--r--   0 alex       (501) staff       (20)     1921 2023-01-15 18:11:43.000000 dlc2action-0.2b3/tests/test_valleys_intersection.py
```

### Comparing `dlc2action-0.2b2/NOTICE.yml` & `dlc2action-0.2b3/NOTICE.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 # Main repository license
 - header: |
-    Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+    Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 
     This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 
   include:
     - 'dlc2action/**/*.py'
     - 'tests/**/*.py'
     - 'examples/**/*.py'
   exclude: []
 
 # License for ASFormer code
 - header: |
-    Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+    Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 
     This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 
 
     Adapted from ASFormer by ChinaYi
     Adapted from https://github.com/ChinaYi/ASFormer
     Licensed under MIT License
   include:
     - dlc2action/model/asformer.py
 
 # License for C2F-TCN code
 - header: |
-    Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+    Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 
     This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 
 
     Adapted from C2F-TCN by dipika singhania
     Adapted from https://github.com/dipika-singhania/C2F-TCN
     Licensed under MIT License
   include:
     - dlc2action/model/c2f_tcn.py
 
 # License for EDTCN code
 - header: |
-    Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+    Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 
     This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 
 
     Adapted from ASRF by yiskw713
     Adapted from https://github.com/yiskw713/asrf/blob/main/libs/models/tcn.py
     Licensed under MIT License
   include:
     - dlc2action/model/edtcn.py
 
 # License for TCC code
 - header: |
-    Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+    Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 
     This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 
 
     Adapted from Temporal Cycle-Consistency Learning by June01
     Adapted from https://github.com/June01/tcc_Temporal_Cycle_Consistency_Loss.pytorch
     Licensed under  Apache License Version 2.0, January 2004
   include:
     - dlc2action/loss/tcc.py
 
 # License for MS-TCN code
 - header: |
-    Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+    Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 
     This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 
 
     Adapted from MS-TCN++ by yabufarha
     Adapted from https://github.com/sj-li/MS-TCN2
     Licensed under MIT License
```

### Comparing `dlc2action-0.2b2/PKG-INFO` & `dlc2action-0.2b3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dlc2action
-Version: 0.2b2
+Version: 0.2b3
 Summary: tba
-Home-page: https://github.com/amathislab/DLC2Action
+Home-page: https://github.com/AlexEMG/DLC2action
 Author: A. Mathis Lab
 Author-email: alexander@deeplabcut.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -23,15 +23,15 @@
 ## Installation
 
 ### Via the Python Package Index
 
 You can simply install DLC2Action by typing:
 
 ```
-pip install "dlc2action==0.2b2"
+pip install "dlc2action==0.2b3"
 ```
 
 ### From Github
 
 You can install DLC2Action for development by running this in your terminal.
 ```
 git clone https://github.com/AlexEMG/DLC2Action
@@ -80,18 +80,16 @@
 ## How to get more information?
 
 Check out the [examples](/examples) or [read the documentation](https://alexemg.github.io/DLC2action/html_docs/dlc2action.html) for a taste of what else you can do.
 
 
 ## Acknowledgments
 
-[Liza Kozlova](https://github.com/elkoz) from the [A. Mathis Group at EPFL](https://www.mathislab.org/) is the main developer of DLC2Action.
-
-We are grateful to many people for feedback, alpha-testing and suggestions, in particular to Andy Bonnetto, Lucas Stoffl, Margaret Lane, Marouane Jaakik, Steffen Schneider and Mackenzie Mathis.
+DLC2Action is developed by members of the [A. Mathis Group at EPFL](https://www.mathislab.org/). We are grateful to many people for feedback, alpha-testing, suggestions and contributions, in particular to Liza Kozlova, Andy Bonnetto, Lucas Stoffl, Margaret Lane, Marouane Jaakik, Steffen Schneider and Mackenzie Mathis.
 
 ## License:
 
 Note that the software is provided "as is", without warranty of any kind, express or implied. If you use the code or data, please cite us!
 
 ## Reference:
 
-Stay tuned for our first publication -- Any feedback on this beta release is welcome at this time. Thanks for using DLC2Action.
+Stay tuned for our first publication -- any feedback on this beta release is welcome at this time. Thanks for using DLC2Action. Please reach out if you want to collaborate!
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: dlc2action Version: 0.2b2 Summary: tba Home-page:
-https://github.com/amathislab/DLC2Action Author: A. Mathis Lab Author-email:
+Metadata-Version: 2.1 Name: dlc2action Version: 0.2b3 Summary: tba Home-page:
+https://github.com/AlexEMG/DLC2action Author: A. Mathis Lab Author-email:
 alexander@deeplabcut.org Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3
 (LGPLv3) Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE.yml License-File:
 NOTICE.yml [![Generic badge](https://img.shields.io/badge/Contributions-
 Welcome-brightgreen.svg)](CONTRIBUTING.md) [Code_style:_black] ![](logos/
 title.png) DLC2Action is an action segmentation package that makes running and
 tracking of machine learning experiments easy. ## Installation ### Via the
 Python Package Index You can simply install DLC2Action by typing: ``` pip
-install "dlc2action==0.2b2" ``` ### From Github You can install DLC2Action for
+install "dlc2action==0.2b3" ``` ### From Github You can install DLC2Action for
 development by running this in your terminal. ``` git clone https://github.com/
 AlexEMG/DLC2Action cd DLC2Action conda create --name DLC2Action python=3.9
 conda activate DLC2Action python -m pip install . ``` ## Features The
 functionality of DLC2Action includes: - compiling and updating project-specific
 configuration files, - filling in configuration dictionaries automatically
 whenever possible, - saving training parameters and results, - running
 predictions and hyperparameter searches, - creating active learning files, -
@@ -32,16 +32,17 @@
 (...) # run a training episode project.run_episode('episode_1') # plot the
 results project.plot_episodes(['episode_1'], metrics=['recall']) # use the
 model trained in episode_1 to make a prediction for new data
 project.run_prediction('prediction_1', episode_names=['episode_1'],
 data_path='path/to/new_data/folder') ``` ## How to get more information? Check
 out the [examples](/examples) or [read the documentation](https://
 alexemg.github.io/DLC2action/html_docs/dlc2action.html) for a taste of what
-else you can do. ## Acknowledgments [Liza Kozlova](https://github.com/elkoz)
-from the [A. Mathis Group at EPFL](https://www.mathislab.org/) is the main
-developer of DLC2Action. We are grateful to many people for feedback, alpha-
-testing and suggestions, in particular to Andy Bonnetto, Lucas Stoffl, Margaret
-Lane, Marouane Jaakik, Steffen Schneider and Mackenzie Mathis. ## License: Note
-that the software is provided "as is", without warranty of any kind, express or
+else you can do. ## Acknowledgments DLC2Action is developed by members of the
+[A. Mathis Group at EPFL](https://www.mathislab.org/). We are grateful to many
+people for feedback, alpha-testing, suggestions and contributions, in
+particular to Liza Kozlova, Andy Bonnetto, Lucas Stoffl, Margaret Lane,
+Marouane Jaakik, Steffen Schneider and Mackenzie Mathis. ## License: Note that
+the software is provided "as is", without warranty of any kind, express or
 implied. If you use the code or data, please cite us! ## Reference: Stay tuned
-for our first publication -- Any feedback on this beta release is welcome at
-this time. Thanks for using DLC2Action.
+for our first publication -- any feedback on this beta release is welcome at
+this time. Thanks for using DLC2Action. Please reach out if you want to
+collaborate!
```

### Comparing `dlc2action-0.2b2/README.md` & `dlc2action-0.2b3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ## Installation
 
 ### Via the Python Package Index
 
 You can simply install DLC2Action by typing:
 
 ```
-pip install "dlc2action==0.2b2"
+pip install "dlc2action==0.2b3"
 ```
 
 ### From Github
 
 You can install DLC2Action for development by running this in your terminal.
 ```
 git clone https://github.com/AlexEMG/DLC2Action
@@ -65,18 +65,16 @@
 ## How to get more information?
 
 Check out the [examples](/examples) or [read the documentation](https://alexemg.github.io/DLC2action/html_docs/dlc2action.html) for a taste of what else you can do.
 
 
 ## Acknowledgments
 
-[Liza Kozlova](https://github.com/elkoz) from the [A. Mathis Group at EPFL](https://www.mathislab.org/) is the main developer of DLC2Action.
-
-We are grateful to many people for feedback, alpha-testing and suggestions, in particular to Andy Bonnetto, Lucas Stoffl, Margaret Lane, Marouane Jaakik, Steffen Schneider and Mackenzie Mathis.
+DLC2Action is developed by members of the [A. Mathis Group at EPFL](https://www.mathislab.org/). We are grateful to many people for feedback, alpha-testing, suggestions and contributions, in particular to Liza Kozlova, Andy Bonnetto, Lucas Stoffl, Margaret Lane, Marouane Jaakik, Steffen Schneider and Mackenzie Mathis.
 
 ## License:
 
 Note that the software is provided "as is", without warranty of any kind, express or implied. If you use the code or data, please cite us!
 
 ## Reference:
 
-Stay tuned for our first publication -- Any feedback on this beta release is welcome at this time. Thanks for using DLC2Action.
+Stay tuned for our first publication -- any feedback on this beta release is welcome at this time. Thanks for using DLC2Action. Please reach out if you want to collaborate!
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 [![Generic badge](https://img.shields.io/badge/Contributions-Welcome-
 brightgreen.svg)](CONTRIBUTING.md) [Code_style:_black] ![](logos/title.png)
 DLC2Action is an action segmentation package that makes running and tracking of
 machine learning experiments easy. ## Installation ### Via the Python Package
 Index You can simply install DLC2Action by typing: ``` pip install
-"dlc2action==0.2b2" ``` ### From Github You can install DLC2Action for
+"dlc2action==0.2b3" ``` ### From Github You can install DLC2Action for
 development by running this in your terminal. ``` git clone https://github.com/
 AlexEMG/DLC2Action cd DLC2Action conda create --name DLC2Action python=3.9
 conda activate DLC2Action python -m pip install . ``` ## Features The
 functionality of DLC2Action includes: - compiling and updating project-specific
 configuration files, - filling in configuration dictionaries automatically
 whenever possible, - saving training parameters and results, - running
 predictions and hyperparameter searches, - creating active learning files, -
@@ -26,16 +26,17 @@
 (...) # run a training episode project.run_episode('episode_1') # plot the
 results project.plot_episodes(['episode_1'], metrics=['recall']) # use the
 model trained in episode_1 to make a prediction for new data
 project.run_prediction('prediction_1', episode_names=['episode_1'],
 data_path='path/to/new_data/folder') ``` ## How to get more information? Check
 out the [examples](/examples) or [read the documentation](https://
 alexemg.github.io/DLC2action/html_docs/dlc2action.html) for a taste of what
-else you can do. ## Acknowledgments [Liza Kozlova](https://github.com/elkoz)
-from the [A. Mathis Group at EPFL](https://www.mathislab.org/) is the main
-developer of DLC2Action. We are grateful to many people for feedback, alpha-
-testing and suggestions, in particular to Andy Bonnetto, Lucas Stoffl, Margaret
-Lane, Marouane Jaakik, Steffen Schneider and Mackenzie Mathis. ## License: Note
-that the software is provided "as is", without warranty of any kind, express or
+else you can do. ## Acknowledgments DLC2Action is developed by members of the
+[A. Mathis Group at EPFL](https://www.mathislab.org/). We are grateful to many
+people for feedback, alpha-testing, suggestions and contributions, in
+particular to Liza Kozlova, Andy Bonnetto, Lucas Stoffl, Margaret Lane,
+Marouane Jaakik, Steffen Schneider and Mackenzie Mathis. ## License: Note that
+the software is provided "as is", without warranty of any kind, express or
 implied. If you use the code or data, please cite us! ## Reference: Stay tuned
-for our first publication -- Any feedback on this beta release is welcome at
-this time. Thanks for using DLC2Action.
+for our first publication -- any feedback on this beta release is welcome at
+this time. Thanks for using DLC2Action. Please reach out if you want to
+collaborate!
```

### Comparing `dlc2action-0.2b2/dlc2action/__init__.py` & `dlc2action-0.2b3/dlc2action/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 `dlc2action` is an action segmentation package that makes running and tracking experiments easy.
 
 # Usage
```

### Comparing `dlc2action-0.2b2/dlc2action/config/annotation/boris.yaml` & `dlc2action-0.2b3/dlc2action/config/annotation/boris.yaml`

 * *Files identical despite different names*

### Comparing `dlc2action-0.2b2/dlc2action/config/annotation/csv.yaml` & `dlc2action-0.2b3/dlc2action/config/annotation/csv.yaml`

 * *Files identical despite different names*

### Comparing `dlc2action-0.2b2/dlc2action/config/annotation/dlc.yaml` & `dlc2action-0.2b3/dlc2action/config/annotation/dlc.yaml`

 * *Files identical despite different names*

### Comparing `dlc2action-0.2b2/dlc2action/config/annotation/pku-mmd.yaml` & `dlc2action-0.2b3/dlc2action/config/annotation/pku-mmd.yaml`

 * *Files identical despite different names*

### Comparing `dlc2action-0.2b2/dlc2action/config/annotation/simba.yaml` & `dlc2action-0.2b3/dlc2action/config/annotation/simba.yaml`

 * *Files identical despite different names*

### Comparing `dlc2action-0.2b2/dlc2action/config/augmentations/kinematic.yaml` & `dlc2action-0.2b3/dlc2action/config/augmentations/kinematic.yaml`

 * *Files identical despite different names*

### Comparing `dlc2action-0.2b2/dlc2action/config/data/dlc_track.yaml` & `dlc2action-0.2b3/dlc2action/config/data/dlc_track.yaml`

 * *Files identical despite different names*

### Comparing `dlc2action-0.2b2/dlc2action/config/data/dlc_tracklet.yaml` & `dlc2action-0.2b3/dlc2action/config/data/dlc_tracklet.yaml`

 * *Files identical despite different names*

### Comparing `dlc2action-0.2b2/dlc2action/config/data/np_3d.yaml` & `dlc2action-0.2b3/dlc2action/config/data/np_3d.yaml`

 * *Files identical despite different names*

### Comparing `dlc2action-0.2b2/dlc2action/config/data/simba.yaml` & `dlc2action-0.2b3/dlc2action/config/data/simba.yaml`

 * *Files identical despite different names*

### Comparing `dlc2action-0.2b2/dlc2action/config/features/kinematic.yaml` & `dlc2action-0.2b3/dlc2action/config/features/kinematic.yaml`

 * *Files identical despite different names*

### Comparing `dlc2action-0.2b2/dlc2action/config/general.yaml` & `dlc2action-0.2b3/dlc2action/config/general.yaml`

 * *Files identical despite different names*

### Comparing `dlc2action-0.2b2/dlc2action/config/metrics.yaml` & `dlc2action-0.2b3/dlc2action/config/metrics.yaml`

 * *Files identical despite different names*

### Comparing `dlc2action-0.2b2/dlc2action/config/ssl.yaml` & `dlc2action-0.2b3/dlc2action/config/ssl.yaml`

 * *Files identical despite different names*

### Comparing `dlc2action-0.2b2/dlc2action/config/training.yaml` & `dlc2action-0.2b3/dlc2action/config/training.yaml`

 * *Files identical despite different names*

### Comparing `dlc2action-0.2b2/dlc2action/data/__init__.py` & `dlc2action-0.2b3/dlc2action/data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 
 """
 ## Dataset and related objects
```

### Comparing `dlc2action-0.2b2/dlc2action/data/annotation_store.py` & `dlc2action-0.2b3/dlc2action/data/annotation_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Specific implementations of `dlc2action.data.base_store.AnnotationStore` are defined here
 """
 
@@ -885,15 +885,15 @@
                     if self.exclusive:
                         if not self.filter_background:
                             value = beh_inv.get("other", 0)
                             labels = np.ones(v_len, dtype=np.compat.long) * value
                         else:
                             labels = -100 * np.ones(v_len, dtype=np.compat.long)
                     else:
-                        labels = np.zeros((len(self.behaviors), v_len), dtype=np.float)
+                        labels = np.zeros((len(self.behaviors), v_len), dtype=float)
                     cat_new = []
                     for cat in times[ind].keys():
                         if cat.startswith("unknown"):
                             cat_new.append(cat)
                     for cat in times[ind].keys():
                         if cat.startswith("negative"):
                             cat_new.append(cat)
@@ -981,15 +981,15 @@
                 if self.exclusive:
                     annotation[
                         os.path.basename(name) + "---" + str(ind)
                     ] = -100 * np.ones(v_len, dtype=np.compat.long)
                 else:
                     annotation[
                         os.path.basename(name) + "---" + str(ind)
-                    ] = -100 * np.ones((len(self.behaviors), v_len), dtype=np.float)
+                    ] = -100 * np.ones((len(self.behaviors), v_len), dtype=float)
         return annotation
 
     def _make_trimmed_annotations(self, annotations_dict: Dict) -> torch.Tensor:
         """
         Cut a label dictionary into overlapping pieces of equal length
         """
```

### Comparing `dlc2action-0.2b2/dlc2action/data/base_store.py` & `dlc2action-0.2b3/dlc2action/data/base_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Abstract parent classes for the store objects
 """
```

### Comparing `dlc2action-0.2b2/dlc2action/data/dataset.py` & `dlc2action-0.2b3/dlc2action/data/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Behavior dataset (class that manages high-level data interactions)
 """
```

### Comparing `dlc2action-0.2b2/dlc2action/data/input_store.py` & `dlc2action-0.2b3/dlc2action/data/input_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Specific realisations of `dlc2action.data.base_store.InputStore` are defined here
 """
```

### Comparing `dlc2action-0.2b2/dlc2action/feature_extraction/__init__.py` & `dlc2action-0.2b3/dlc2action/feature_extraction/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 ## Feature extraction
 
 Feature extractors generate feature dictionaries that are then passed to SSL transformations
```

### Comparing `dlc2action-0.2b2/dlc2action/loss/__init__.py` & `dlc2action-0.2b3/dlc2action/loss/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 ## Losses
 
 There is no dedicated loss class in `dlc2action`. Instead we use regular `torch.nn.Module` instances that take
```

### Comparing `dlc2action-0.2b2/dlc2action/loss/contrastive.py` & `dlc2action-0.2b3/dlc2action/loss/contrastive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Losses used by contrastive SSL constructors (see `dlc2action.ssl.contrastive`)
 """
```

### Comparing `dlc2action-0.2b2/dlc2action/loss/contrastive_frame.py` & `dlc2action-0.2b3/dlc2action/loss/contrastive_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 from torch import nn
 import torch
```

### Comparing `dlc2action-0.2b2/dlc2action/loss/ms_tcn.py` & `dlc2action-0.2b3/dlc2action/loss/ms_tcn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 #
 # Adapted from MS-TCN++ by yabufarha
 # Adapted from https://github.com/sj-li/MS-TCN2
 # Licensed under MIT License
```

### Comparing `dlc2action-0.2b2/dlc2action/loss/mse.py` & `dlc2action-0.2b3/dlc2action/loss/mse.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 The mean squared error loss
 """
```

### Comparing `dlc2action-0.2b2/dlc2action/loss/tcc.py` & `dlc2action-0.2b3/dlc2action/loss/tcc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 #
 # Adapted from Temporal Cycle-Consistency Learning by June01
 # Adapted from https://github.com/June01/tcc_Temporal_Cycle_Consistency_Loss.pytorch
 # Licensed under  Apache License Version 2.0, January 2004
```

### Comparing `dlc2action-0.2b2/dlc2action/metric/base_metric.py` & `dlc2action-0.2b3/dlc2action/metric/base_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Abstract parent class for all metrics
 """
```

### Comparing `dlc2action-0.2b2/dlc2action/metric/metrics.py` & `dlc2action-0.2b3/dlc2action/metric/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Implementations of `dlc2action.metric.base_metric.Metric`
 """
```

### Comparing `dlc2action-0.2b2/dlc2action/model/__init__.py` & `dlc2action-0.2b3/dlc2action/model/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 ## Models
 
 The `dlc2action.model.base_model.Model` abstract class inherits from `torch.nn.Module` but additionally
```

### Comparing `dlc2action-0.2b2/dlc2action/model/asformer.py` & `dlc2action-0.2b3/dlc2action/model/asformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 #
 # Adapted from ASFormer by ChinaYi
 # Adapted from https://github.com/ChinaYi/ASFormer
 # Licensed under MIT License
```

### Comparing `dlc2action-0.2b2/dlc2action/model/base_model.py` & `dlc2action-0.2b3/dlc2action/model/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Abstract parent class for models used in `dlc2action.task.universal_task.Task`
 """
```

### Comparing `dlc2action-0.2b2/dlc2action/model/c2f_tcn.py` & `dlc2action-0.2b3/dlc2action/model/c2f_tcn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 #
 # Adapted from C2F-TCN by dipika singhania
 # Adapted from https://github.com/dipika-singhania/C2F-TCN
 # Licensed under MIT License
```

### Comparing `dlc2action-0.2b2/dlc2action/model/edtcn.py` & `dlc2action-0.2b3/dlc2action/model/edtcn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 #
 # Adapted from ASRF by yiskw713
 # Adapted from https://github.com/yiskw713/asrf/blob/main/libs/models/tcn.py
 # Licensed under MIT License
```

### Comparing `dlc2action-0.2b2/dlc2action/model/mlp.py` & `dlc2action-0.2b3/dlc2action/model/mlp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 from dlc2action.model.base_model import Model
 import torch
 from torch import nn
 from typing import List, Union
```

### Comparing `dlc2action-0.2b2/dlc2action/model/transformer.py` & `dlc2action-0.2b3/dlc2action/model/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 import torch
 from torch import nn
 from torch.nn import functional as F
 import math
```

### Comparing `dlc2action-0.2b2/dlc2action/options.py` & `dlc2action-0.2b3/dlc2action/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Here all option dictionaries are stored
 """
```

### Comparing `dlc2action-0.2b2/dlc2action/project/__init__.py` & `dlc2action-0.2b3/dlc2action/project/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 ## Project interface
 
 The most convenient way to use `dlc2action` is through the high-level project interface. It is defined in the
```

### Comparing `dlc2action-0.2b2/dlc2action/project/meta.py` & `dlc2action-0.2b3/dlc2action/project/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Handling meta (history) files
 """
 
@@ -889,15 +889,15 @@
             results[("meta", "training_time")] = training_time
         for k, v in results.items():
             self.data.loc[episode_name, k] = v
         self._save()
 
     def get_runs(self, episode_name: str) -> List:
         """
-        Get a list of runs with this episode name (episodes like `episode_name::0`)
+        Get a list of runs with this episode name (episodes like `episode_name#0`)
 
         Parameters
         ----------
         episode_name : str
             the name of the episode
 
         Returns
@@ -908,15 +908,15 @@
 
         if episode_name is None:
             return []
         index = self.data.index
         runs_list = []
         for name in index:
             if name.startswith(episode_name):
-                split = name.split("::")
+                split = name.split("#")
                 if split[0] == episode_name:
                     if len(split) > 1 and split[-1].isnumeric() or len(split) == 1:
                         runs_list.append(name)
                 elif name == episode_name:
                     runs_list.append(name)
         return runs_list
```

### Comparing `dlc2action-0.2b2/dlc2action/project/project.py` & `dlc2action-0.2b3/dlc2action/project/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Project interface
 """
 import copy
@@ -673,15 +673,15 @@
         round_to_binary : list, optional
             a list of string names of the loaded parameters that should be rounded to the nearest power of two
         load_strict : bool, default True
             if `False`, matching weights will be loaded from `load_episode` and differences in parameter name lists and
             weight shapes will be ignored; otherwise mismatches will prompt a `RuntimeError`
         n_seeds : int, default 1
             the number of runs to perform with different random seeds; if `n_seeds > 1`, the episodes will be named
-            `episode_name::seed_index`, e.g. `test_episode::0` and `test_episode::1`
+            `episode_name#seed_index`, e.g. `test_episode#0` and `test_episode#1`
         force : bool, default False
             if `True` and an episode with name `episode_name` already exists, it will be overwritten (use with caution!)
         suppress_name_check : bool, default False
             if `True`, episode names with a double colon are allowed (please don't use this option unless you understand
             why they are usually forbidden)
         remove_saved_features : bool, default False
             if `True`, the dataset will be deleted after training
@@ -704,15 +704,15 @@
         self._check_episode_validity(
             episode_name, allow_doublecolon=suppress_name_check, force=force
         )
         load_runs = self._episodes().get_runs(load_episode)
         if len(load_runs) > 1:
             task = self.run_episodes(
                 episode_names=[
-                    f'{episode_name}::{run.split("::")[-1]}' for run in load_runs
+                    f'{episode_name}#{run.split("#")[-1]}' for run in load_runs
                 ],
                 load_episodes=load_runs,
                 parameters_updates=[parameters_update for _ in load_runs],
                 load_epochs=[load_epoch for _ in load_runs],
                 load_searches=[load_search for _ in load_runs],
                 load_parameters=[load_parameters for _ in load_runs],
                 round_to_binary=[round_to_binary for _ in load_runs],
@@ -731,15 +731,15 @@
                 )
             if n_seeds > 1:
                 warnings.warn(
                     f"The n_seeds parameter is disregarded since load_episode={load_episode} has multiple runs"
                 )
         elif n_seeds > 1:
             self.run_episodes(
-                episode_names=[f"{episode_name}::{i}" for i in range(n_seeds)],
+                episode_names=[f"{episode_name}#{i}" for i in range(n_seeds)],
                 load_episodes=[load_episode for _ in range(n_seeds)],
                 parameters_updates=[parameters_update for _ in range(n_seeds)],
                 load_epochs=[load_epoch for _ in range(n_seeds)],
                 load_searches=[load_search for _ in range(n_seeds)],
                 load_parameters=[load_parameters for _ in range(n_seeds)],
                 round_to_binary=[round_to_binary for _ in range(n_seeds)],
                 load_strict=[load_strict for _ in range(n_seeds)],
@@ -929,16 +929,16 @@
         task : TaskDispatcher, optional
             a pre-existing task; if provided, the method will update the task instead of creating a new one
             (this might save time, mainly on dataset loading)
         result_average_interval : int, default 5
             the metric are averaged over the last result_average_interval to be stored in the episodes meta file
             and displayed by list_episodes() function (the full log is still always available)
         n_seeds : int, default 1
-            the number of runs to perform; if `n_seeds > 1`, the episodes will be named `episode_name::run_index`, e.g.
-            `test_episode::0` and `test_episode::1`
+            the number of runs to perform; if `n_seeds > 1`, the episodes will be named `episode_name#run_index`, e.g.
+            `test_episode#0` and `test_episode#1`
         remove_saved_features : bool, default False
             if `True`, pre-computed features will be deleted after the run
         device : str, default "cuda"
             the torch device to use
         """
 
         runs = self._episodes().get_runs(episode_name)
@@ -984,15 +984,15 @@
                 norm_stats=task.get_normalization_stats(),
             )
             self._update_episode_results(run, logs)
             print("\n")
         if len(runs) < n_seeds:
             for i in range(len(runs), n_seeds):
                 self.run_episode(
-                    f"{episode_name}::{i}",
+                    f"{episode_name}#{i}",
                     parameters_update=self._episodes().load_parameters(runs[0]),
                     task=task,
                     suppress_name_check=True,
                 )
         if remove_saved_features:
             self._remove_stores(parameters)
         return task
@@ -1850,15 +1850,15 @@
                 if isinstance(name, Iterable) and not isinstance(name, str):
                     epoch_list = defaultdict(lambda: [])
                     multi_logs = defaultdict(lambda: [])
                     for i, n in enumerate(name):
                         runs = self._episodes().get_runs(n)
                         if len(runs) > 1:
                             for run in runs:
-                                index = run.split("::")[-1]
+                                index = run.split("#")[-1]
                                 if multi_logs[index] == []:
                                     if multi_logs["null"] is None:
                                         raise RuntimeError(
                                             "The run indices are not consistent across episodes!"
                                         )
                                     else:
                                         multi_logs[index] += multi_logs["null"]
@@ -3458,17 +3458,17 @@
 
         if episode_name.startswith("_"):
             raise ValueError(
                 "Names starting with an underscore are reserved by dlc2action and cannot be used!"
             )
         elif "." in episode_name:
             raise ValueError("Names containing '.' cannot be used!")
-        if not allow_doublecolon and "::" in episode_name:
+        if not allow_doublecolon and "#" in episode_name:
             raise ValueError(
-                "Names containing '::' are reserved by dlc2action and cannot be used!"
+                "Names containing '#' are reserved by dlc2action and cannot be used!"
             )
         if force:
             self.remove_episode(episode_name)
         elif not self._episodes().check_name_validity(episode_name):
             raise ValueError(
                 f"The {episode_name} name is already taken! Set force=True to overwrite."
             )
@@ -3669,16 +3669,15 @@
         if "overlap" in pars["data"]:
             pars["data"].pop("overlap")
         split_info = {k: pars["training"][k] for k in keys}
         split_info["only_load_annotated"] = pars["general"]["only_load_annotated"]
         split_info["len_segment"] = pars["general"]["len_segment"]
         split_info["overlap"] = pars["general"]["overlap"]
         pars["training"]["log_file"] = log
-        if not os.path.exists(model_save_path):
-            os.mkdir(model_save_path)
+        os.makedirs(model_save_path, exist_ok=True)
         pars["training"]["model_save_path"] = model_save_path
         if load_experiment is not None:
             if load_experiment not in self._episodes().data.index:
                 raise ValueError(f"The {load_experiment} episode does not exist!")
             old_episode = self._episode(load_experiment)
             old_file = old_episode.split_file()
             old_info = self._split_info_from_filename(old_file)
```

### Comparing `dlc2action-0.2b2/dlc2action/ssl/__init__.py` & `dlc2action-0.2b3/dlc2action/ssl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 ## Self-supervised tasks
 
 Self-supervised learning tasks in `dlc2action` are implemented in the form of the `base_ssl.SSLConstructor`
```

### Comparing `dlc2action-0.2b2/dlc2action/ssl/base_ssl.py` & `dlc2action-0.2b3/dlc2action/ssl/base_ssl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Abstract class for defining SSL tasks
 """
```

### Comparing `dlc2action-0.2b2/dlc2action/ssl/contrastive.py` & `dlc2action-0.2b3/dlc2action/ssl/contrastive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Implementations of `dlc2action.ssl.base_ssl.SSLConstructor` of the `'contrastive'` type
 """
```

### Comparing `dlc2action-0.2b2/dlc2action/ssl/masked.py` & `dlc2action-0.2b3/dlc2action/ssl/masked.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Implementations of `dlc2action.ssl.base_ssl.SSLConstructor` that predict masked input features
 """
```

### Comparing `dlc2action-0.2b2/dlc2action/ssl/modules.py` & `dlc2action-0.2b3/dlc2action/ssl/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Network modules used by implementations of `dlc2action.ssl.base_ssl.SSLConstructor`
 """
```

### Comparing `dlc2action-0.2b2/dlc2action/ssl/segment_order.py` & `dlc2action-0.2b3/dlc2action/ssl/segment_order.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 from typing import Dict, Tuple, Union, List
 import torch
 from dlc2action.ssl.base_ssl import SSLConstructor
 from abc import ABC, abstractmethod
```

### Comparing `dlc2action-0.2b2/dlc2action/ssl/tcc.py` & `dlc2action-0.2b3/dlc2action/ssl/tcc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 from dlc2action.ssl.base_ssl import SSLConstructor
 import torch
 from dlc2action.loss.tcc import _TCCLoss
 from typing import Dict, Union, Tuple
```

### Comparing `dlc2action-0.2b2/dlc2action/task/__init__.py` & `dlc2action-0.2b3/dlc2action/task/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 ## Training and inference
 
 `dlc2action.task.universal_task.Task` is the class that performs training and inference while
```

### Comparing `dlc2action-0.2b2/dlc2action/task/task_dispatcher.py` & `dlc2action-0.2b3/dlc2action/task/task_dispatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Class that provides an interface for `dlc2action.task.universal_task.Task`
 """
```

### Comparing `dlc2action-0.2b2/dlc2action/task/universal_task.py` & `dlc2action-0.2b3/dlc2action/task/universal_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Training and inference
 """
```

### Comparing `dlc2action-0.2b2/dlc2action/transformer/__init__.py` & `dlc2action-0.2b3/dlc2action/transformer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 ## Augmentations and feature concatenation
 
 Input data in `dlc2action` is stored in feature dictionaries right up until being passed to a model.
```

### Comparing `dlc2action-0.2b2/dlc2action/transformer/base_transformer.py` & `dlc2action-0.2b3/dlc2action/transformer/base_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Abstract parent class for transformers
 """
```

### Comparing `dlc2action-0.2b2/dlc2action/transformer/kinematic.py` & `dlc2action-0.2b3/dlc2action/transformer/kinematic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 Kinematic transformer
 """
```

### Comparing `dlc2action-0.2b2/dlc2action/utils.py` & `dlc2action-0.2b3/dlc2action/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2020-2022 by A. Mathis Group and contributors. All rights reserved.
+# Copyright 2020-present by A. Mathis Group and contributors. All rights reserved.
 #
 # This project and all its files are licensed under GNU AGPLv3 or later version. A copy is included in dlc2action/LICENSE.AGPL.
 #
 """
 ## Utility functions
 
 - `TensorDict` is a convenient data structure for keeping (and indexing) lists of feature dictionaries,
```

### Comparing `dlc2action-0.2b2/dlc2action.egg-info/PKG-INFO` & `dlc2action-0.2b3/dlc2action.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dlc2action
-Version: 0.2b2
+Version: 0.2b3
 Summary: tba
-Home-page: https://github.com/amathislab/DLC2Action
+Home-page: https://github.com/AlexEMG/DLC2action
 Author: A. Mathis Lab
 Author-email: alexander@deeplabcut.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -23,15 +23,15 @@
 ## Installation
 
 ### Via the Python Package Index
 
 You can simply install DLC2Action by typing:
 
 ```
-pip install "dlc2action==0.2b2"
+pip install "dlc2action==0.2b3"
 ```
 
 ### From Github
 
 You can install DLC2Action for development by running this in your terminal.
 ```
 git clone https://github.com/AlexEMG/DLC2Action
@@ -80,18 +80,16 @@
 ## How to get more information?
 
 Check out the [examples](/examples) or [read the documentation](https://alexemg.github.io/DLC2action/html_docs/dlc2action.html) for a taste of what else you can do.
 
 
 ## Acknowledgments
 
-[Liza Kozlova](https://github.com/elkoz) from the [A. Mathis Group at EPFL](https://www.mathislab.org/) is the main developer of DLC2Action.
-
-We are grateful to many people for feedback, alpha-testing and suggestions, in particular to Andy Bonnetto, Lucas Stoffl, Margaret Lane, Marouane Jaakik, Steffen Schneider and Mackenzie Mathis.
+DLC2Action is developed by members of the [A. Mathis Group at EPFL](https://www.mathislab.org/). We are grateful to many people for feedback, alpha-testing, suggestions and contributions, in particular to Liza Kozlova, Andy Bonnetto, Lucas Stoffl, Margaret Lane, Marouane Jaakik, Steffen Schneider and Mackenzie Mathis.
 
 ## License:
 
 Note that the software is provided "as is", without warranty of any kind, express or implied. If you use the code or data, please cite us!
 
 ## Reference:
 
-Stay tuned for our first publication -- Any feedback on this beta release is welcome at this time. Thanks for using DLC2Action.
+Stay tuned for our first publication -- any feedback on this beta release is welcome at this time. Thanks for using DLC2Action. Please reach out if you want to collaborate!
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: dlc2action Version: 0.2b2 Summary: tba Home-page:
-https://github.com/amathislab/DLC2Action Author: A. Mathis Lab Author-email:
+Metadata-Version: 2.1 Name: dlc2action Version: 0.2b3 Summary: tba Home-page:
+https://github.com/AlexEMG/DLC2action Author: A. Mathis Lab Author-email:
 alexander@deeplabcut.org Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3
 (LGPLv3) Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE.yml License-File:
 NOTICE.yml [![Generic badge](https://img.shields.io/badge/Contributions-
 Welcome-brightgreen.svg)](CONTRIBUTING.md) [Code_style:_black] ![](logos/
 title.png) DLC2Action is an action segmentation package that makes running and
 tracking of machine learning experiments easy. ## Installation ### Via the
 Python Package Index You can simply install DLC2Action by typing: ``` pip
-install "dlc2action==0.2b2" ``` ### From Github You can install DLC2Action for
+install "dlc2action==0.2b3" ``` ### From Github You can install DLC2Action for
 development by running this in your terminal. ``` git clone https://github.com/
 AlexEMG/DLC2Action cd DLC2Action conda create --name DLC2Action python=3.9
 conda activate DLC2Action python -m pip install . ``` ## Features The
 functionality of DLC2Action includes: - compiling and updating project-specific
 configuration files, - filling in configuration dictionaries automatically
 whenever possible, - saving training parameters and results, - running
 predictions and hyperparameter searches, - creating active learning files, -
@@ -32,16 +32,17 @@
 (...) # run a training episode project.run_episode('episode_1') # plot the
 results project.plot_episodes(['episode_1'], metrics=['recall']) # use the
 model trained in episode_1 to make a prediction for new data
 project.run_prediction('prediction_1', episode_names=['episode_1'],
 data_path='path/to/new_data/folder') ``` ## How to get more information? Check
 out the [examples](/examples) or [read the documentation](https://
 alexemg.github.io/DLC2action/html_docs/dlc2action.html) for a taste of what
-else you can do. ## Acknowledgments [Liza Kozlova](https://github.com/elkoz)
-from the [A. Mathis Group at EPFL](https://www.mathislab.org/) is the main
-developer of DLC2Action. We are grateful to many people for feedback, alpha-
-testing and suggestions, in particular to Andy Bonnetto, Lucas Stoffl, Margaret
-Lane, Marouane Jaakik, Steffen Schneider and Mackenzie Mathis. ## License: Note
-that the software is provided "as is", without warranty of any kind, express or
+else you can do. ## Acknowledgments DLC2Action is developed by members of the
+[A. Mathis Group at EPFL](https://www.mathislab.org/). We are grateful to many
+people for feedback, alpha-testing, suggestions and contributions, in
+particular to Liza Kozlova, Andy Bonnetto, Lucas Stoffl, Margaret Lane,
+Marouane Jaakik, Steffen Schneider and Mackenzie Mathis. ## License: Note that
+the software is provided "as is", without warranty of any kind, express or
 implied. If you use the code or data, please cite us! ## Reference: Stay tuned
-for our first publication -- Any feedback on this beta release is welcome at
-this time. Thanks for using DLC2Action.
+for our first publication -- any feedback on this beta release is welcome at
+this time. Thanks for using DLC2Action. Please reach out if you want to
+collaborate!
```

### Comparing `dlc2action-0.2b2/dlc2action.egg-info/SOURCES.txt` & `dlc2action-0.2b3/dlc2action.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -73,8 +73,28 @@
 dlc2action/ssl/segment_order.py
 dlc2action/ssl/tcc.py
 dlc2action/task/__init__.py
 dlc2action/task/task_dispatcher.py
 dlc2action/task/universal_task.py
 dlc2action/transformer/__init__.py
 dlc2action/transformer/base_transformer.py
-dlc2action/transformer/kinematic.py
+dlc2action/transformer/kinematic.py
+tests/test_average_evaluation.py
+tests/test_dataset_loading.py
+tests/test_delete_datasets.py
+tests/test_episodes_export.py
+tests/test_find_valleys.py
+tests/test_full_length_prediction.py
+tests/test_loading_parameters.py
+tests/test_losses.py
+tests/test_metrics.py
+tests/test_partition.py
+tests/test_prediction.py
+tests/test_project_fill.py
+tests/test_project_list.py
+tests/test_pruning.py
+tests/test_search.py
+tests/test_ssl.py
+tests/test_task_creation.py
+tests/test_task_update.py
+tests/test_training.py
+tests/test_valleys_intersection.py
```

### Comparing `dlc2action-0.2b2/setup.py` & `dlc2action-0.2b3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dlc2action",
-    version="0.2b2",
+    version="0.2b3",
     author="A. Mathis Lab",
     author_email="alexander@deeplabcut.org",
     description="tba",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/amathislab/DLC2Action",
+    url="https://github.com/AlexEMG/DLC2action",
     install_requires=[
         "tqdm>=4.62.3",
         "torch>=1.9",
         "numpy>=1.21.2",
         "scipy>=1.7.1",
         "pandas==1.4.3",
         "matplotlib>=3.4.3",
@@ -36,15 +36,15 @@
         "pytest>=7.1.2",
         "tables>=3.7.0",
         "torchvision>=0.13.1",
         "ftfy>=6.1.1",
         "regex>=2022.8.17",
         "scikit-learn>=1.1.2",
         "jupyter",  # added for demo
-    
+
     ],
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
         "Operating System :: OS Independent",
     ],
```

