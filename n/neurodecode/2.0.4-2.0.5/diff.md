# Comparing `tmp/neurodecode-2.0.4.tar.gz` & `tmp/neurodecode-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurodecode-2.0.4.tar", last modified: Thu May 25 04:42:34 2023, max compression
+gzip compressed data, was "neurodecode-2.0.5.tar", last modified: Wed May 31 02:12:28 2023, max compression
```

## Comparing `neurodecode-2.0.4.tar` & `neurodecode-2.0.5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:42:34.375687 neurodecode-2.0.4/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     9930 2023-05-25 04:42:34.375687 neurodecode-2.0.4/PKG-INFO
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     9597 2022-11-04 09:26:38.000000 neurodecode-2.0.4/README.md
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:42:34.375687 neurodecode-2.0.4/neurodecode/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     4422 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/__init__.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:42:34.375687 neurodecode-2.0.4/neurodecode/analysis/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/analysis/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     7563 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/analysis/feature_importances_topo.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     6449 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/analysis/parse_features.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    12585 2023-05-25 04:20:23.000000 neurodecode-2.0.4/neurodecode/analysis/tfr_export.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     4889 2023-05-25 04:25:18.000000 neurodecode-2.0.4/neurodecode/analysis/tfr_export_each_file.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     4350 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/colorer.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:42:34.375687 neurodecode-2.0.4/neurodecode/decoder/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/decoder/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    29797 2023-01-20 12:47:05.000000 neurodecode-2.0.4/neurodecode/decoder/decoder.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    19602 2023-01-19 16:02:04.000000 neurodecode-2.0.4/neurodecode/decoder/features.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     3235 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/decoder/rlda.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    27572 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/decoder/trainer.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:42:34.375687 neurodecode-2.0.4/neurodecode/glass/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/glass/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     5437 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/glass/bgi_client.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:42:34.375687 neurodecode-2.0.4/neurodecode/protocols/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        1 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/protocols/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    20725 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/protocols/feedback.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    22921 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/protocols/feedback_fes.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     7022 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/protocols/viz_bars.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     9395 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/protocols/viz_images.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2958 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/pycnbi_config.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:42:34.375687 neurodecode-2.0.4/neurodecode/stream_player/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/stream_player/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     5868 2023-01-19 15:39:29.000000 neurodecode-2.0.4/neurodecode/stream_player/stream_player.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:42:34.375687 neurodecode-2.0.4/neurodecode/stream_receiver/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/stream_receiver/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    22404 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/stream_receiver/stream_receiver.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:42:34.375687 neurodecode-2.0.4/neurodecode/stream_recorder/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/stream_recorder/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     6840 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/stream_recorder/stream_recorder.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:42:34.375687 neurodecode-2.0.4/neurodecode/stream_viewer/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/stream_viewer/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     1502 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/stream_viewer/scope_settings.ini
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    40740 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/stream_viewer/stream_viewer.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    25369 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/stream_viewer/ui_mainwindow_Viewer.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:42:34.375687 neurodecode-2.0.4/neurodecode/triggers/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/triggers/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    10620 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/triggers/pyLptControl.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2156 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/triggers/trigger_def.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:42:34.375687 neurodecode-2.0.4/neurodecode/utils/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     5949 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/Motionstim8.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2472 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/ScalerMad.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        0 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/__init__.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2250 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/add_lsl_events.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     1044 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/benchmark_decoder.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     1185 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/benchmark_multitaper.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    19412 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/convert2fif.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2809 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/epochs2mat.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2370 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/epochs2txt.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     1664 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/fif2mat.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     1199 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/fif_info.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     1505 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/fif_resample.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     1455 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/fix_channel_names.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     3687 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/hdf5_to_python.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     1414 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/images2pkl.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)      684 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/list_trigger_pins.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2061 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/mat2fif.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2305 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/merge_events.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2772 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/nd_lsl.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)      853 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/parse_online_results.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     3705 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/psd_visualizer.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    24294 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/pycnbi_utils.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)    24367 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/q_common.py
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     3897 2022-11-04 09:26:38.000000 neurodecode-2.0.4/neurodecode/utils/raw2psd.py
-drwxrwxr-x   0 leeq      (1000) leeq      (1000)        0 2023-05-25 04:42:34.375687 neurodecode-2.0.4/neurodecode.egg-info/
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     9930 2023-05-25 04:42:34.000000 neurodecode-2.0.4/neurodecode.egg-info/PKG-INFO
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2245 2023-05-25 04:42:34.000000 neurodecode-2.0.4/neurodecode.egg-info/SOURCES.txt
--rw-rw-r--   0 leeq      (1000) leeq      (1000)        1 2023-05-25 04:42:34.000000 neurodecode-2.0.4/neurodecode.egg-info/dependency_links.txt
--rw-rw-r--   0 leeq      (1000) leeq      (1000)      780 2023-05-25 04:42:34.000000 neurodecode-2.0.4/neurodecode.egg-info/entry_points.txt
--rw-rw-r--   0 leeq      (1000) leeq      (1000)      299 2023-05-25 04:42:34.000000 neurodecode-2.0.4/neurodecode.egg-info/requires.txt
--rw-rw-r--   0 leeq      (1000) leeq      (1000)       12 2023-05-25 04:42:34.000000 neurodecode-2.0.4/neurodecode.egg-info/top_level.txt
--rw-rw-r--   0 leeq      (1000) leeq      (1000)       38 2023-05-25 04:42:34.375687 neurodecode-2.0.4/setup.cfg
--rw-rw-r--   0 leeq      (1000) leeq      (1000)     2350 2023-05-25 04:41:47.000000 neurodecode-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:12:28.224645 neurodecode-2.0.5/
+-rw-rw-rw-   0        0        0    10124 2023-05-31 02:12:28.224645 neurodecode-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9781 2022-11-07 14:35:59.000000 neurodecode-2.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 02:12:27.925915 neurodecode-2.0.5/neurodecode/
+-rw-rw-rw-   0        0        0     4544 2022-11-02 14:56:21.000000 neurodecode-2.0.5/neurodecode/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:12:27.954800 neurodecode-2.0.5/neurodecode/analysis/
+-rw-rw-rw-   0        0        0        0 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/analysis/__init__.py
+-rw-rw-rw-   0        0        0     7744 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/analysis/feature_importances_topo.py
+-rw-rw-rw-   0        0        0     6674 2023-05-31 02:11:38.000000 neurodecode-2.0.5/neurodecode/analysis/parse_features.py
+-rw-rw-rw-   0        0        0    12892 2023-05-31 02:11:38.000000 neurodecode-2.0.5/neurodecode/analysis/tfr_export.py
+-rw-rw-rw-   0        0        0     5036 2023-05-31 02:11:38.000000 neurodecode-2.0.5/neurodecode/analysis/tfr_export_each_file.py
+-rw-rw-rw-   0        0        0     4469 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/colorer.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:12:27.964620 neurodecode-2.0.5/neurodecode/decoder/
+-rw-rw-rw-   0        0        0        0 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/decoder/__init__.py
+-rw-rw-rw-   0        0        0    30633 2023-05-31 01:27:07.000000 neurodecode-2.0.5/neurodecode/decoder/decoder.py
+-rw-rw-rw-   0        0        0    20134 2023-05-31 01:27:07.000000 neurodecode-2.0.5/neurodecode/decoder/features.py
+-rw-rw-rw-   0        0        0     3345 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/decoder/rlda.py
+-rw-rw-rw-   0        0        0    28275 2022-11-02 14:56:21.000000 neurodecode-2.0.5/neurodecode/decoder/trainer.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:12:27.975828 neurodecode-2.0.5/neurodecode/glass/
+-rw-rw-rw-   0        0        0        0 2022-11-02 14:56:21.000000 neurodecode-2.0.5/neurodecode/glass/__init__.py
+-rw-rw-rw-   0        0        0     5624 2022-11-02 14:56:21.000000 neurodecode-2.0.5/neurodecode/glass/bgi_client.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:12:28.017266 neurodecode-2.0.5/neurodecode/protocols/
+-rw-rw-rw-   0        0        0        2 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/protocols/__init__.py
+-rw-rw-rw-   0        0        0    21168 2022-11-02 14:56:21.000000 neurodecode-2.0.5/neurodecode/protocols/feedback.py
+-rw-rw-rw-   0        0        0    23409 2022-11-02 14:56:21.000000 neurodecode-2.0.5/neurodecode/protocols/feedback_fes.py
+-rw-rw-rw-   0        0        0     7207 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/protocols/viz_bars.py
+-rw-rw-rw-   0        0        0     9643 2022-11-02 14:56:21.000000 neurodecode-2.0.5/neurodecode/protocols/viz_images.py
+-rw-rw-rw-   0        0        0     3002 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/pycnbi_config.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:12:28.019264 neurodecode-2.0.5/neurodecode/stream_player/
+-rw-rw-rw-   0        0        0        0 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/stream_player/__init__.py
+-rw-rw-rw-   0        0        0     6029 2023-01-12 16:03:23.000000 neurodecode-2.0.5/neurodecode/stream_player/stream_player.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:12:28.036414 neurodecode-2.0.5/neurodecode/stream_receiver/
+-rw-rw-rw-   0        0        0        0 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/stream_receiver/__init__.py
+-rw-rw-rw-   0        0        0    22947 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/stream_receiver/stream_receiver.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:12:28.044750 neurodecode-2.0.5/neurodecode/stream_recorder/
+-rw-rw-rw-   0        0        0        0 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/stream_recorder/__init__.py
+-rw-rw-rw-   0        0        0     7023 2022-11-02 14:56:21.000000 neurodecode-2.0.5/neurodecode/stream_recorder/stream_recorder.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:12:28.044750 neurodecode-2.0.5/neurodecode/stream_viewer/
+-rw-rw-rw-   0        0        0        0 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/stream_viewer/__init__.py
+-rw-rw-rw-   0        0        0     1533 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/stream_viewer/scope_settings.ini
+-rw-rw-rw-   0        0        0    41777 2023-05-31 02:01:39.000000 neurodecode-2.0.5/neurodecode/stream_viewer/stream_viewer.py
+-rw-rw-rw-   0        0        0    25860 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/stream_viewer/ui_mainwindow_Viewer.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:12:28.064506 neurodecode-2.0.5/neurodecode/triggers/
+-rw-rw-rw-   0        0        0        0 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/triggers/__init__.py
+-rw-rw-rw-   0        0        0    10901 2022-11-02 14:56:21.000000 neurodecode-2.0.5/neurodecode/triggers/pyLptControl.py
+-rw-rw-rw-   0        0        0     2225 2022-11-02 14:56:21.000000 neurodecode-2.0.5/neurodecode/triggers/trigger_def.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:12:28.222124 neurodecode-2.0.5/neurodecode/utils/
+-rw-rw-rw-   0        0        0     6133 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/Motionstim8.py
+-rw-rw-rw-   0        0        0     2557 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/ScalerMad.py
+-rw-rw-rw-   0        0        0        0 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/__init__.py
+-rw-rw-rw-   0        0        0     2328 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/add_lsl_events.py
+-rw-rw-rw-   0        0        0     1083 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/benchmark_decoder.py
+-rw-rw-rw-   0        0        0     1232 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/benchmark_multitaper.py
+-rw-rw-rw-   0        0        0    19968 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/convert2fif.py
+-rw-rw-rw-   0        0        0     2888 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/epochs2mat.py
+-rw-rw-rw-   0        0        0     2443 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/epochs2txt.py
+-rw-rw-rw-   0        0        0     1722 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/fif2mat.py
+-rw-rw-rw-   0        0        0     1249 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/fif_info.py
+-rw-rw-rw-   0        0        0     1561 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/fif_resample.py
+-rw-rw-rw-   0        0        0     1499 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/fix_channel_names.py
+-rw-rw-rw-   0        0        0     3780 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/hdf5_to_python.py
+-rw-rw-rw-   0        0        0     1449 2022-11-02 14:56:21.000000 neurodecode-2.0.5/neurodecode/utils/images2pkl.py
+-rw-rw-rw-   0        0        0      714 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/list_trigger_pins.py
+-rw-rw-rw-   0        0        0     2117 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/mat2fif.py
+-rw-rw-rw-   0        0        0     2376 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/merge_events.py
+-rw-rw-rw-   0        0        0     2869 2022-11-02 14:56:21.000000 neurodecode-2.0.5/neurodecode/utils/nd_lsl.py
+-rw-rw-rw-   0        0        0      886 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/parse_online_results.py
+-rw-rw-rw-   0        0        0     3821 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/psd_visualizer.py
+-rw-rw-rw-   0        0        0    24966 2022-11-02 14:56:21.000000 neurodecode-2.0.5/neurodecode/utils/pycnbi_utils.py
+-rw-rw-rw-   0        0        0    25137 2022-11-02 14:56:21.000000 neurodecode-2.0.5/neurodecode/utils/q_common.py
+-rw-rw-rw-   0        0        0     4009 2022-10-31 16:11:25.000000 neurodecode-2.0.5/neurodecode/utils/raw2psd.py
+drwxrwxrwx   0        0        0        0 2023-05-31 02:12:27.944608 neurodecode-2.0.5/neurodecode.egg-info/
+-rw-rw-rw-   0        0        0    10124 2023-05-31 02:12:27.000000 neurodecode-2.0.5/neurodecode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2245 2023-05-31 02:12:27.000000 neurodecode-2.0.5/neurodecode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 02:12:27.000000 neurodecode-2.0.5/neurodecode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      780 2023-05-31 02:12:27.000000 neurodecode-2.0.5/neurodecode.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      299 2023-05-31 02:12:27.000000 neurodecode-2.0.5/neurodecode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-31 02:12:27.000000 neurodecode-2.0.5/neurodecode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 02:12:28.224645 neurodecode-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2417 2023-05-31 02:11:47.000000 neurodecode-2.0.5/setup.py
```

### Comparing `neurodecode-2.0.4/PKG-INFO` & `neurodecode-2.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,194 +1,194 @@
-Metadata-Version: 2.1
-Name: neurodecode
-Version: 2.0.4
-Summary: Real-time brain signal decoding framework
-Home-page: https://github.com/dbdq/neurodecode/
-Author: Kyuhwa Lee, Arnaud Desvachez
-Author-email: lee.kyuh@gmail.com, arnaud.desvachez@gmail.com
-License: The GNU General Public License
-Description-Content-Type: text/markdown
-
-# Introduction
-
-Neurodecode provides a real-time brain signal decoding framework. The decoding performance was recognised at [Microsoft Brain Signal Decoding competition](https://github.com/dbdq/microsoft_decoding) with the <i>First Prize Award</i> (2016) for high decoding accuracy (2nd out of 1863 algorithms). It has been applied on a couple of online decoding projects with various electrode types including EEG, ECoG and DBS, and on several acquisition systems including AntNeuro eego, g.tec gUSBamp, BioSemi ActiveTwo, BrainProducts actiCHamp and Wearable Sensing. With modular software design, the decoding runs at approximately 15 classifications per second(cps) on a 4th-gen i7 laptop with 64-channel setup at 512 Hz sampling rate. High-speed decoding up to 200 cps was achieved using process-interleaving technique on 8 cores. It has been tested on both Linux and Windows using Python 3.7.
-
-The underlying data communication is based on Lab Streaming Layer (LSL) which provides sub-millisecond time synchronization accuracy. Any signal acquisition system supported by native LSL or OpenVibe is also supported by Neurodecode. Since the data communication is based on TCP, signals can be also transmitted wirelessly. For more information about LSL, please visit:
-[https://github.com/sccn/labstreaminglayer](https://github.com/sccn/labstreaminglayer)
-
-
-# Important modules
-
-### StreamReceiver
-The base module for acquiring signals used by other modules such as Decoder, StreamViewer and StreamRecorder.
-
-### StreamViewer
-Visualize signals in real time with spectral filtering, common average filtering options and real-time FFT.
-
-### StreamRecorder
-Record signals into fif format, a standard format mainly used in [MNE EEG analysis library](http://martinos.org/mne/).
-
-### StreamPlayer
-Replay the recorded signals in real time as if it was transmitted from a real acquisition server.
-
-### Decoder
-This folder contains decoder and trainer modules. Currently, LDA, regularized LDA, Random Forests, and Gradient Boosting Machines are supported as the classifier type. Neural Network-based decoders are currently under experiment.
-
-### Protocols
-Contains some basic protocols for training and testing. Google Glass visual feedback is supported through USB communication.
-
-### Triggers
-Triggers are used to mark event (stimulus) timings during the recording. This folder contains common trigger event definition files. 
-
-### Utils
-Contains various utilities.
-
-
-# Prerequisites
-
-Anaconda is recommended for easy installation of Python environment.
-
-Neurodecode depends on following packages:
-  - scipy
-  - numpy
-  - PyQt5
-  - scikit-learn
-  - pylsl
-  - mne 0.14 or later
-  - matplotlib 2.1.0 or later
-  - pyqtgraph
-  - opencv-python
-  - pyserial
-  - future
-  - configparser
-  - xgboost
-  - psutil
-
-Optional but strongly recommended:
-  - [OpenVibe](http://openvibe.inria.fr/downloads)
-
-OpenVibe supports a wide range of acquisition servers and all acquisition systems supported by OpenVibe are supported by Neurodecode through LSL. Make sure you tick the checkbox "LSL_EnableLSLOutput" in Preferences when you run acquisition server. This will stream the data through the LSL network from which Neurodecode receives data. 
-
-# Installation
-
-Neurodecode can be installed from PyPI.
-```
-pip install neurodecode
-```
-
-To install the latest version, clone the repository and run setup script:
-```
-git clone https://github.com/dbdq/neurodecode.git
-python setup.py develop
-```
-Add "scripts" directory to PATH environment variable for convenient access to commonly used scripts.
-
-### PyQt version problem
-The Qt API is very sensitive to version and needs to be compatible with all dependencies.
-If you experience pyqtgraph complaining incompatible PyQt version (e.g. PyQt < 5.12), try:
-```
-conda remove pyqt
-pip install -U PyQt5
-```
-This can be caused by Anaconda not having the latest PyQt version.
-
-
-### For Windows users, increase timer resolution
-The default timer resolution in some Windows versions is 16 ms, which can limit the precision of timings. It is recommended to run the following tool and set the resolution to 1 ms or lower:
-[https://vvvv.org/contribution/windows-system-timer-tool](https://vvvv.org/contribution/windows-system-timer-tool)
-
-
-### Hardware triggering without legacy parallel port
-We have also developed an Arduino-based triggering system as we wanted to send triggers to a parallel port using standard USB ports. We achieved sub-millisecond extra latency compared to physical parallel port (150 +- 25 us). Experimental results using oscilloscope can be found in "doc" folder. The package can be downloaded by:
-```
-git clone https://github.com/dbdq/arduino-trigger.git
-```
-The customized firmware should be installed on Arduino Micro and the circuit design included in the document folder should be printed to a circuit board.
-
-
-### For g.USBamp users
-The following customized acquisition server is needed instead of default LSL app to receive the trigger channel as part of signal streaming channels:
-```
-git clone https://github.com/dbdq/gUSBamp_pycnbi.git
-```
-because the default gUSBamp LSL server do not stream event channel as part of the signal stream but as a separate server. The customized version supports simultaneous signal+event channel streaming. 
-
-
-### For AntNeuro eego users
-Use the OpenVibe acquisition server and make sure to check "LSL output" in preference.  If you don't see "eego" from the device selection, it's probably because you didn't install the additional drivers when you installed OpenVibe.
-
-<br>
-<br>
-
-# Running examples
-
-To run this example, copy the /sample folder to your local folder and cd into it.
-
-### 1. Play data
-Replay a pre-recorded EEG recording sample in real-time as if acquiring signals from brain with a chunk size of 8.
-The sample data was recorded using a 24-channel EEG system from a participant doing a left and right hand motor imagery.
-The hardware events recorded during the experiment is also streamed via LSL network.
-
-```nd_stream_player mi_left_right.fif 8```
-
-Screenshot of setting up an LSL server and streaming the recorded data.
-![image](https://user-images.githubusercontent.com/6797783/199510832-c10b7df9-193b-4396-a671-15f6f8df0226.png)
-
-### 2. Record data  
-Simulate real-time decoding from the brain. We are streaming the data using nd_stream_player script above while
-the receiver is source-agnostic, allowing the full simulation of replaying and the validation of data processing.  
-This step can be skipped if you create a folder ./fif/ and copy the sample fif file into ./fif/.
-
-```
-nd_stream_recorder $PWD # for Linux
-nd_stream_recorder %CD% # for Windows
-```
-![image](https://user-images.githubusercontent.com/6797783/199511174-abb1ac03-eadc-488d-833a-6e303a93e331.png)
-
-### 3. Real-time signal visualisation (choose StreamPlayer from the list)  
-```nd_stream_viewer```
-
-Sample visualisation of streamed signals. Cursor keys allow different amplitude and time scalings.
-![image](https://user-images.githubusercontent.com/6797783/199509891-a0f30cfd-c589-4004-89f0-c71ff08b4071.png)
-
-### 4. Run an offline protocol for training
-Runs an offline training protocol. This step is just for explanation purpose and can be skipped.  
-```nd_train_mi ./config_offline.py```
-
-Snapshot of the offline protocol.  
-![image](https://user-images.githubusercontent.com/6797783/199511602-6bec54d0-50dd-485c-8d3e-6fa7621cc773.png)
-
-### 5. Train a decoder  
-Train a decoder using the fif file with defined events. In this example, it is left (event 11) vs right (event 9) hand motor imagery.  
-Events are defined in mi_left_right_events.ini file.
-
-```nd_trainer ./config_trainer.py```
-
-### 6. Run an online protocol for testing
-The provided sample is set to 60 seconds time-out without early termination so you can see
-the decoder output changes to left or right when the left (event 11) or right(event 9) is emitted 
-from the stream player terminal. Other events such as rest is undefined and will behave in random direction.
-
-```nd_test_mi config_online.py```
-
-Snapshot of the protocol showing the bar position.  
-![image](https://user-images.githubusercontent.com/6797783/199517521-de33e4f2-92bf-421f-8afc-9eee5c899a04.png)  
-
-Sample decoder output with probabilities and the corresponding bar position, which represents the accumulated probabilities.  
-![image](https://user-images.githubusercontent.com/6797783/199518166-67f8a4ea-dde9-4544-b95d-80ed5f0526aa.png)  
-
-Example of events being emitted from the stream player.  
-![image](https://user-images.githubusercontent.com/6797783/199514155-a94bbb71-c2dc-43d5-81e8-2bd4916a05e4.png)  
-
-There are still plenty of possibilities to optimize the speed in many parts of the code. Any contribution is welcome. Please contact lee.kyuh@gmail.com for any comment / feedback.
-
-
-# Copyright and license
-The codes are released under [GNU General Public License](https://www.gnu.org/licenses/gpl-3.0.en.html).
-
-
-# Citation
-This package was developed as part of the following works:
-  - Yohann Thenaisie* and Kyuhwa Lee* <i>et al.</i>, "Principles of gait encoding in the subthalamic nucleus of people with Parkinson's disease", <i>Science Translational Medicine</i>, 2022, Vol. 14, No. 661, p. eabo1800.<br>(* first authors as equal contribution)
-  - Kyuhwa Lee <i>et al.</i>, "A Brain-Controlled Exoskeleton with Cascaded Event-Related Desynchronization Classifiers", <i>Robotics and Autonomous Systems</i>, Elsevier, 2016, p. 15-23.
-   
-If some of the code here were useful or helpful for your project, I would greatly appreciate if you could cite one of the above papers.
+Metadata-Version: 2.1
+Name: neurodecode
+Version: 2.0.5
+Summary: Real-time brain signal decoding framework
+Home-page: https://github.com/dbdq/neurodecode/
+Author: Kyuhwa Lee, Arnaud Desvachez
+Author-email: lee.kyuh@gmail.com, arnaud.desvachez@gmail.com
+License: The GNU General Public License
+Description-Content-Type: text/markdown
+
+# Introduction
+
+Neurodecode provides a real-time brain signal decoding framework. The decoding performance was recognised at [Microsoft Brain Signal Decoding competition](https://github.com/dbdq/microsoft_decoding) with the <i>First Prize Award</i> (2016) for high decoding accuracy (2nd out of 1863 algorithms). It has been applied on a couple of online decoding projects with various electrode types including EEG, ECoG and DBS, and on several acquisition systems including AntNeuro eego, g.tec gUSBamp, BioSemi ActiveTwo, BrainProducts actiCHamp and Wearable Sensing. With modular software design, the decoding runs at approximately 15 classifications per second(cps) on a 4th-gen i7 laptop with 64-channel setup at 512 Hz sampling rate. High-speed decoding up to 200 cps was achieved using process-interleaving technique on 8 cores. It has been tested on both Linux and Windows using Python 3.7.
+
+The underlying data communication is based on Lab Streaming Layer (LSL) which provides sub-millisecond time synchronization accuracy. Any signal acquisition system supported by native LSL or OpenVibe is also supported by Neurodecode. Since the data communication is based on TCP, signals can be also transmitted wirelessly. For more information about LSL, please visit:
+[https://github.com/sccn/labstreaminglayer](https://github.com/sccn/labstreaminglayer)
+
+
+# Important modules
+
+### StreamReceiver
+The base module for acquiring signals used by other modules such as Decoder, StreamViewer and StreamRecorder.
+
+### StreamViewer
+Visualize signals in real time with spectral filtering, common average filtering options and real-time FFT.
+
+### StreamRecorder
+Record signals into fif format, a standard format mainly used in [MNE EEG analysis library](http://martinos.org/mne/).
+
+### StreamPlayer
+Replay the recorded signals in real time as if it was transmitted from a real acquisition server.
+
+### Decoder
+This folder contains decoder and trainer modules. Currently, LDA, regularized LDA, Random Forests, and Gradient Boosting Machines are supported as the classifier type. Neural Network-based decoders are currently under experiment.
+
+### Protocols
+Contains some basic protocols for training and testing. Google Glass visual feedback is supported through USB communication.
+
+### Triggers
+Triggers are used to mark event (stimulus) timings during the recording. This folder contains common trigger event definition files. 
+
+### Utils
+Contains various utilities.
+
+
+# Prerequisites
+
+Anaconda is recommended for easy installation of Python environment.
+
+Neurodecode depends on following packages:
+  - scipy
+  - numpy
+  - PyQt5
+  - scikit-learn
+  - pylsl
+  - mne 0.14 or later
+  - matplotlib 2.1.0 or later
+  - pyqtgraph
+  - opencv-python
+  - pyserial
+  - future
+  - configparser
+  - xgboost
+  - psutil
+
+Optional but strongly recommended:
+  - [OpenVibe](http://openvibe.inria.fr/downloads)
+
+OpenVibe supports a wide range of acquisition servers and all acquisition systems supported by OpenVibe are supported by Neurodecode through LSL. Make sure you tick the checkbox "LSL_EnableLSLOutput" in Preferences when you run acquisition server. This will stream the data through the LSL network from which Neurodecode receives data. 
+
+# Installation
+
+Neurodecode can be installed from PyPI.
+```
+pip install neurodecode
+```
+
+To install the latest version, clone the repository and run setup script:
+```
+git clone https://github.com/dbdq/neurodecode.git
+python setup.py develop
+```
+Add "scripts" directory to PATH environment variable for convenient access to commonly used scripts.
+
+### PyQt version problem
+The Qt API is very sensitive to version and needs to be compatible with all dependencies.
+If you experience pyqtgraph complaining incompatible PyQt version (e.g. PyQt < 5.12), try:
+```
+conda remove pyqt
+pip install -U PyQt5
+```
+This can be caused by Anaconda not having the latest PyQt version.
+
+
+### For Windows users, increase timer resolution
+The default timer resolution in some Windows versions is 16 ms, which can limit the precision of timings. It is recommended to run the following tool and set the resolution to 1 ms or lower:
+[https://vvvv.org/contribution/windows-system-timer-tool](https://vvvv.org/contribution/windows-system-timer-tool)
+
+
+### Hardware triggering without legacy parallel port
+We have also developed an Arduino-based triggering system as we wanted to send triggers to a parallel port using standard USB ports. We achieved sub-millisecond extra latency compared to physical parallel port (150 +- 25 us). Experimental results using oscilloscope can be found in "doc" folder. The package can be downloaded by:
+```
+git clone https://github.com/dbdq/arduino-trigger.git
+```
+The customized firmware should be installed on Arduino Micro and the circuit design included in the document folder should be printed to a circuit board.
+
+
+### For g.USBamp users
+The following customized acquisition server is needed instead of default LSL app to receive the trigger channel as part of signal streaming channels:
+```
+git clone https://github.com/dbdq/gUSBamp_pycnbi.git
+```
+because the default gUSBamp LSL server do not stream event channel as part of the signal stream but as a separate server. The customized version supports simultaneous signal+event channel streaming. 
+
+
+### For AntNeuro eego users
+Use the OpenVibe acquisition server and make sure to check "LSL output" in preference.  If you don't see "eego" from the device selection, it's probably because you didn't install the additional drivers when you installed OpenVibe.
+
+<br>
+<br>
+
+# Running examples
+
+To run this example, copy the /sample folder to your local folder and cd into it.
+
+### 1. Play data
+Replay a pre-recorded EEG recording sample in real-time as if acquiring signals from brain with a chunk size of 8.
+The sample data was recorded using a 24-channel EEG system from a participant doing a left and right hand motor imagery.
+The hardware events recorded during the experiment is also streamed via LSL network.
+
+```nd_stream_player mi_left_right.fif 8```
+
+Screenshot of setting up an LSL server and streaming the recorded data.
+![image](https://user-images.githubusercontent.com/6797783/199510832-c10b7df9-193b-4396-a671-15f6f8df0226.png)
+
+### 2. Record data  
+Simulate real-time decoding from the brain. We are streaming the data using nd_stream_player script above while
+the receiver is source-agnostic, allowing the full simulation of replaying and the validation of data processing.  
+This step can be skipped if you create a folder ./fif/ and copy the sample fif file into ./fif/.
+
+```
+nd_stream_recorder $PWD # for Linux
+nd_stream_recorder %CD% # for Windows
+```
+![image](https://user-images.githubusercontent.com/6797783/199511174-abb1ac03-eadc-488d-833a-6e303a93e331.png)
+
+### 3. Real-time signal visualisation (choose StreamPlayer from the list)  
+```nd_stream_viewer```
+
+Sample visualisation of streamed signals. Cursor keys allow different amplitude and time scalings.
+![image](https://user-images.githubusercontent.com/6797783/199509891-a0f30cfd-c589-4004-89f0-c71ff08b4071.png)
+
+### 4. Run an offline protocol for training
+Runs an offline training protocol. This step is just for explanation purpose and can be skipped.  
+```nd_train_mi ./config_offline.py```
+
+Snapshot of the offline protocol.  
+![image](https://user-images.githubusercontent.com/6797783/199511602-6bec54d0-50dd-485c-8d3e-6fa7621cc773.png)
+
+### 5. Train a decoder  
+Train a decoder using the fif file with defined events. In this example, it is left (event 11) vs right (event 9) hand motor imagery.  
+Events are defined in mi_left_right_events.ini file.
+
+```nd_trainer ./config_trainer.py```
+
+### 6. Run an online protocol for testing
+The provided sample is set to 60 seconds time-out without early termination so you can see
+the decoder output changes to left or right when the left (event 11) or right(event 9) is emitted 
+from the stream player terminal. Other events such as rest is undefined and will behave in random direction.
+
+```nd_test_mi config_online.py```
+
+Snapshot of the protocol showing the bar position.  
+![image](https://user-images.githubusercontent.com/6797783/199517521-de33e4f2-92bf-421f-8afc-9eee5c899a04.png)  
+
+Sample decoder output with probabilities and the corresponding bar position, which represents the accumulated probabilities.  
+![image](https://user-images.githubusercontent.com/6797783/199518166-67f8a4ea-dde9-4544-b95d-80ed5f0526aa.png)  
+
+Example of events being emitted from the stream player.  
+![image](https://user-images.githubusercontent.com/6797783/199514155-a94bbb71-c2dc-43d5-81e8-2bd4916a05e4.png)  
+
+There are still plenty of possibilities to optimize the speed in many parts of the code. Any contribution is welcome. Please contact lee.kyuh@gmail.com for any comment / feedback.
+
+
+# Copyright and license
+The codes are released under [GNU General Public License](https://www.gnu.org/licenses/gpl-3.0.en.html).
+
+
+# Citation
+This package was developed as part of the following works:
+  - Yohann Thenaisie* and Kyuhwa Lee* <i>et al.</i>, "Principles of gait encoding in the subthalamic nucleus of people with Parkinson's disease", <i>Science Translational Medicine</i>, 2022, Vol. 14, No. 661, p. eabo1800.<br>(* first authors as equal contribution)
+  - Kyuhwa Lee <i>et al.</i>, "A Brain-Controlled Exoskeleton with Cascaded Event-Related Desynchronization Classifiers", <i>Robotics and Autonomous Systems</i>, Elsevier, 2016, p. 15-23.
+   
+If some of the code here were useful or helpful for your project, I would greatly appreciate if you could cite one of the above papers.
```

### Comparing `neurodecode-2.0.4/README.md` & `neurodecode-2.0.5/README.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-# Introduction
-
-Neurodecode provides a real-time brain signal decoding framework. The decoding performance was recognised at [Microsoft Brain Signal Decoding competition](https://github.com/dbdq/microsoft_decoding) with the <i>First Prize Award</i> (2016) for high decoding accuracy (2nd out of 1863 algorithms). It has been applied on a couple of online decoding projects with various electrode types including EEG, ECoG and DBS, and on several acquisition systems including AntNeuro eego, g.tec gUSBamp, BioSemi ActiveTwo, BrainProducts actiCHamp and Wearable Sensing. With modular software design, the decoding runs at approximately 15 classifications per second(cps) on a 4th-gen i7 laptop with 64-channel setup at 512 Hz sampling rate. High-speed decoding up to 200 cps was achieved using process-interleaving technique on 8 cores. It has been tested on both Linux and Windows using Python 3.7.
-
-The underlying data communication is based on Lab Streaming Layer (LSL) which provides sub-millisecond time synchronization accuracy. Any signal acquisition system supported by native LSL or OpenVibe is also supported by Neurodecode. Since the data communication is based on TCP, signals can be also transmitted wirelessly. For more information about LSL, please visit:
-[https://github.com/sccn/labstreaminglayer](https://github.com/sccn/labstreaminglayer)
-
-
-# Important modules
-
-### StreamReceiver
-The base module for acquiring signals used by other modules such as Decoder, StreamViewer and StreamRecorder.
-
-### StreamViewer
-Visualize signals in real time with spectral filtering, common average filtering options and real-time FFT.
-
-### StreamRecorder
-Record signals into fif format, a standard format mainly used in [MNE EEG analysis library](http://martinos.org/mne/).
-
-### StreamPlayer
-Replay the recorded signals in real time as if it was transmitted from a real acquisition server.
-
-### Decoder
-This folder contains decoder and trainer modules. Currently, LDA, regularized LDA, Random Forests, and Gradient Boosting Machines are supported as the classifier type. Neural Network-based decoders are currently under experiment.
-
-### Protocols
-Contains some basic protocols for training and testing. Google Glass visual feedback is supported through USB communication.
-
-### Triggers
-Triggers are used to mark event (stimulus) timings during the recording. This folder contains common trigger event definition files. 
-
-### Utils
-Contains various utilities.
-
-
-# Prerequisites
-
-Anaconda is recommended for easy installation of Python environment.
-
-Neurodecode depends on following packages:
-  - scipy
-  - numpy
-  - PyQt5
-  - scikit-learn
-  - pylsl
-  - mne 0.14 or later
-  - matplotlib 2.1.0 or later
-  - pyqtgraph
-  - opencv-python
-  - pyserial
-  - future
-  - configparser
-  - xgboost
-  - psutil
-
-Optional but strongly recommended:
-  - [OpenVibe](http://openvibe.inria.fr/downloads)
-
-OpenVibe supports a wide range of acquisition servers and all acquisition systems supported by OpenVibe are supported by Neurodecode through LSL. Make sure you tick the checkbox "LSL_EnableLSLOutput" in Preferences when you run acquisition server. This will stream the data through the LSL network from which Neurodecode receives data. 
-
-# Installation
-
-Neurodecode can be installed from PyPI.
-```
-pip install neurodecode
-```
-
-To install the latest version, clone the repository and run setup script:
-```
-git clone https://github.com/dbdq/neurodecode.git
-python setup.py develop
-```
-Add "scripts" directory to PATH environment variable for convenient access to commonly used scripts.
-
-### PyQt version problem
-The Qt API is very sensitive to version and needs to be compatible with all dependencies.
-If you experience pyqtgraph complaining incompatible PyQt version (e.g. PyQt < 5.12), try:
-```
-conda remove pyqt
-pip install -U PyQt5
-```
-This can be caused by Anaconda not having the latest PyQt version.
-
-
-### For Windows users, increase timer resolution
-The default timer resolution in some Windows versions is 16 ms, which can limit the precision of timings. It is recommended to run the following tool and set the resolution to 1 ms or lower:
-[https://vvvv.org/contribution/windows-system-timer-tool](https://vvvv.org/contribution/windows-system-timer-tool)
-
-
-### Hardware triggering without legacy parallel port
-We have also developed an Arduino-based triggering system as we wanted to send triggers to a parallel port using standard USB ports. We achieved sub-millisecond extra latency compared to physical parallel port (150 +- 25 us). Experimental results using oscilloscope can be found in "doc" folder. The package can be downloaded by:
-```
-git clone https://github.com/dbdq/arduino-trigger.git
-```
-The customized firmware should be installed on Arduino Micro and the circuit design included in the document folder should be printed to a circuit board.
-
-
-### For g.USBamp users
-The following customized acquisition server is needed instead of default LSL app to receive the trigger channel as part of signal streaming channels:
-```
-git clone https://github.com/dbdq/gUSBamp_pycnbi.git
-```
-because the default gUSBamp LSL server do not stream event channel as part of the signal stream but as a separate server. The customized version supports simultaneous signal+event channel streaming. 
-
-
-### For AntNeuro eego users
-Use the OpenVibe acquisition server and make sure to check "LSL output" in preference.  If you don't see "eego" from the device selection, it's probably because you didn't install the additional drivers when you installed OpenVibe.
-
-<br>
-<br>
-
-# Running examples
-
-To run this example, copy the /sample folder to your local folder and cd into it.
-
-### 1. Play data
-Replay a pre-recorded EEG recording sample in real-time as if acquiring signals from brain with a chunk size of 8.
-The sample data was recorded using a 24-channel EEG system from a participant doing a left and right hand motor imagery.
-The hardware events recorded during the experiment is also streamed via LSL network.
-
-```nd_stream_player mi_left_right.fif 8```
-
-Screenshot of setting up an LSL server and streaming the recorded data.
-![image](https://user-images.githubusercontent.com/6797783/199510832-c10b7df9-193b-4396-a671-15f6f8df0226.png)
-
-### 2. Record data  
-Simulate real-time decoding from the brain. We are streaming the data using nd_stream_player script above while
-the receiver is source-agnostic, allowing the full simulation of replaying and the validation of data processing.  
-This step can be skipped if you create a folder ./fif/ and copy the sample fif file into ./fif/.
-
-```
-nd_stream_recorder $PWD # for Linux
-nd_stream_recorder %CD% # for Windows
-```
-![image](https://user-images.githubusercontent.com/6797783/199511174-abb1ac03-eadc-488d-833a-6e303a93e331.png)
-
-### 3. Real-time signal visualisation (choose StreamPlayer from the list)  
-```nd_stream_viewer```
-
-Sample visualisation of streamed signals. Cursor keys allow different amplitude and time scalings.
-![image](https://user-images.githubusercontent.com/6797783/199509891-a0f30cfd-c589-4004-89f0-c71ff08b4071.png)
-
-### 4. Run an offline protocol for training
-Runs an offline training protocol. This step is just for explanation purpose and can be skipped.  
-```nd_train_mi ./config_offline.py```
-
-Snapshot of the offline protocol.  
-![image](https://user-images.githubusercontent.com/6797783/199511602-6bec54d0-50dd-485c-8d3e-6fa7621cc773.png)
-
-### 5. Train a decoder  
-Train a decoder using the fif file with defined events. In this example, it is left (event 11) vs right (event 9) hand motor imagery.  
-Events are defined in mi_left_right_events.ini file.
-
-```nd_trainer ./config_trainer.py```
-
-### 6. Run an online protocol for testing
-The provided sample is set to 60 seconds time-out without early termination so you can see
-the decoder output changes to left or right when the left (event 11) or right(event 9) is emitted 
-from the stream player terminal. Other events such as rest is undefined and will behave in random direction.
-
-```nd_test_mi config_online.py```
-
-Snapshot of the protocol showing the bar position.  
-![image](https://user-images.githubusercontent.com/6797783/199517521-de33e4f2-92bf-421f-8afc-9eee5c899a04.png)  
-
-Sample decoder output with probabilities and the corresponding bar position, which represents the accumulated probabilities.  
-![image](https://user-images.githubusercontent.com/6797783/199518166-67f8a4ea-dde9-4544-b95d-80ed5f0526aa.png)  
-
-Example of events being emitted from the stream player.  
-![image](https://user-images.githubusercontent.com/6797783/199514155-a94bbb71-c2dc-43d5-81e8-2bd4916a05e4.png)  
-
-There are still plenty of possibilities to optimize the speed in many parts of the code. Any contribution is welcome. Please contact lee.kyuh@gmail.com for any comment / feedback.
-
-
-# Copyright and license
-The codes are released under [GNU General Public License](https://www.gnu.org/licenses/gpl-3.0.en.html).
-
-
-# Citation
-This package was developed as part of the following works:
-  - Yohann Thenaisie* and Kyuhwa Lee* <i>et al.</i>, "Principles of gait encoding in the subthalamic nucleus of people with Parkinson's disease", <i>Science Translational Medicine</i>, 2022, Vol. 14, No. 661, p. eabo1800.<br>(* first authors as equal contribution)
-  - Kyuhwa Lee <i>et al.</i>, "A Brain-Controlled Exoskeleton with Cascaded Event-Related Desynchronization Classifiers", <i>Robotics and Autonomous Systems</i>, Elsevier, 2016, p. 15-23.
-   
-If some of the code here were useful or helpful for your project, I would greatly appreciate if you could cite one of the above papers.
+# Introduction
+
+Neurodecode provides a real-time brain signal decoding framework. The decoding performance was recognised at [Microsoft Brain Signal Decoding competition](https://github.com/dbdq/microsoft_decoding) with the <i>First Prize Award</i> (2016) for high decoding accuracy (2nd out of 1863 algorithms). It has been applied on a couple of online decoding projects with various electrode types including EEG, ECoG and DBS, and on several acquisition systems including AntNeuro eego, g.tec gUSBamp, BioSemi ActiveTwo, BrainProducts actiCHamp and Wearable Sensing. With modular software design, the decoding runs at approximately 15 classifications per second(cps) on a 4th-gen i7 laptop with 64-channel setup at 512 Hz sampling rate. High-speed decoding up to 200 cps was achieved using process-interleaving technique on 8 cores. It has been tested on both Linux and Windows using Python 3.7.
+
+The underlying data communication is based on Lab Streaming Layer (LSL) which provides sub-millisecond time synchronization accuracy. Any signal acquisition system supported by native LSL or OpenVibe is also supported by Neurodecode. Since the data communication is based on TCP, signals can be also transmitted wirelessly. For more information about LSL, please visit:
+[https://github.com/sccn/labstreaminglayer](https://github.com/sccn/labstreaminglayer)
+
+
+# Important modules
+
+### StreamReceiver
+The base module for acquiring signals used by other modules such as Decoder, StreamViewer and StreamRecorder.
+
+### StreamViewer
+Visualize signals in real time with spectral filtering, common average filtering options and real-time FFT.
+
+### StreamRecorder
+Record signals into fif format, a standard format mainly used in [MNE EEG analysis library](http://martinos.org/mne/).
+
+### StreamPlayer
+Replay the recorded signals in real time as if it was transmitted from a real acquisition server.
+
+### Decoder
+This folder contains decoder and trainer modules. Currently, LDA, regularized LDA, Random Forests, and Gradient Boosting Machines are supported as the classifier type. Neural Network-based decoders are currently under experiment.
+
+### Protocols
+Contains some basic protocols for training and testing. Google Glass visual feedback is supported through USB communication.
+
+### Triggers
+Triggers are used to mark event (stimulus) timings during the recording. This folder contains common trigger event definition files. 
+
+### Utils
+Contains various utilities.
+
+
+# Prerequisites
+
+Anaconda is recommended for easy installation of Python environment.
+
+Neurodecode depends on following packages:
+  - scipy
+  - numpy
+  - PyQt5
+  - scikit-learn
+  - pylsl
+  - mne 0.14 or later
+  - matplotlib 2.1.0 or later
+  - pyqtgraph
+  - opencv-python
+  - pyserial
+  - future
+  - configparser
+  - xgboost
+  - psutil
+
+Optional but strongly recommended:
+  - [OpenVibe](http://openvibe.inria.fr/downloads)
+
+OpenVibe supports a wide range of acquisition servers and all acquisition systems supported by OpenVibe are supported by Neurodecode through LSL. Make sure you tick the checkbox "LSL_EnableLSLOutput" in Preferences when you run acquisition server. This will stream the data through the LSL network from which Neurodecode receives data. 
+
+# Installation
+
+Neurodecode can be installed from PyPI.
+```
+pip install neurodecode
+```
+
+To install the latest version, clone the repository and run setup script:
+```
+git clone https://github.com/dbdq/neurodecode.git
+python setup.py develop
+```
+Add "scripts" directory to PATH environment variable for convenient access to commonly used scripts.
+
+### PyQt version problem
+The Qt API is very sensitive to version and needs to be compatible with all dependencies.
+If you experience pyqtgraph complaining incompatible PyQt version (e.g. PyQt < 5.12), try:
+```
+conda remove pyqt
+pip install -U PyQt5
+```
+This can be caused by Anaconda not having the latest PyQt version.
+
+
+### For Windows users, increase timer resolution
+The default timer resolution in some Windows versions is 16 ms, which can limit the precision of timings. It is recommended to run the following tool and set the resolution to 1 ms or lower:
+[https://vvvv.org/contribution/windows-system-timer-tool](https://vvvv.org/contribution/windows-system-timer-tool)
+
+
+### Hardware triggering without legacy parallel port
+We have also developed an Arduino-based triggering system as we wanted to send triggers to a parallel port using standard USB ports. We achieved sub-millisecond extra latency compared to physical parallel port (150 +- 25 us). Experimental results using oscilloscope can be found in "doc" folder. The package can be downloaded by:
+```
+git clone https://github.com/dbdq/arduino-trigger.git
+```
+The customized firmware should be installed on Arduino Micro and the circuit design included in the document folder should be printed to a circuit board.
+
+
+### For g.USBamp users
+The following customized acquisition server is needed instead of default LSL app to receive the trigger channel as part of signal streaming channels:
+```
+git clone https://github.com/dbdq/gUSBamp_pycnbi.git
+```
+because the default gUSBamp LSL server do not stream event channel as part of the signal stream but as a separate server. The customized version supports simultaneous signal+event channel streaming. 
+
+
+### For AntNeuro eego users
+Use the OpenVibe acquisition server and make sure to check "LSL output" in preference.  If you don't see "eego" from the device selection, it's probably because you didn't install the additional drivers when you installed OpenVibe.
+
+<br>
+<br>
+
+# Running examples
+
+To run this example, copy the /sample folder to your local folder and cd into it.
+
+### 1. Play data
+Replay a pre-recorded EEG recording sample in real-time as if acquiring signals from brain with a chunk size of 8.
+The sample data was recorded using a 24-channel EEG system from a participant doing a left and right hand motor imagery.
+The hardware events recorded during the experiment is also streamed via LSL network.
+
+```nd_stream_player mi_left_right.fif 8```
+
+Screenshot of setting up an LSL server and streaming the recorded data.
+![image](https://user-images.githubusercontent.com/6797783/199510832-c10b7df9-193b-4396-a671-15f6f8df0226.png)
+
+### 2. Record data  
+Simulate real-time decoding from the brain. We are streaming the data using nd_stream_player script above while
+the receiver is source-agnostic, allowing the full simulation of replaying and the validation of data processing.  
+This step can be skipped if you create a folder ./fif/ and copy the sample fif file into ./fif/.
+
+```
+nd_stream_recorder $PWD # for Linux
+nd_stream_recorder %CD% # for Windows
+```
+![image](https://user-images.githubusercontent.com/6797783/199511174-abb1ac03-eadc-488d-833a-6e303a93e331.png)
+
+### 3. Real-time signal visualisation (choose StreamPlayer from the list)  
+```nd_stream_viewer```
+
+Sample visualisation of streamed signals. Cursor keys allow different amplitude and time scalings.
+![image](https://user-images.githubusercontent.com/6797783/199509891-a0f30cfd-c589-4004-89f0-c71ff08b4071.png)
+
+### 4. Run an offline protocol for training
+Runs an offline training protocol. This step is just for explanation purpose and can be skipped.  
+```nd_train_mi ./config_offline.py```
+
+Snapshot of the offline protocol.  
+![image](https://user-images.githubusercontent.com/6797783/199511602-6bec54d0-50dd-485c-8d3e-6fa7621cc773.png)
+
+### 5. Train a decoder  
+Train a decoder using the fif file with defined events. In this example, it is left (event 11) vs right (event 9) hand motor imagery.  
+Events are defined in mi_left_right_events.ini file.
+
+```nd_trainer ./config_trainer.py```
+
+### 6. Run an online protocol for testing
+The provided sample is set to 60 seconds time-out without early termination so you can see
+the decoder output changes to left or right when the left (event 11) or right(event 9) is emitted 
+from the stream player terminal. Other events such as rest is undefined and will behave in random direction.
+
+```nd_test_mi config_online.py```
+
+Snapshot of the protocol showing the bar position.  
+![image](https://user-images.githubusercontent.com/6797783/199517521-de33e4f2-92bf-421f-8afc-9eee5c899a04.png)  
+
+Sample decoder output with probabilities and the corresponding bar position, which represents the accumulated probabilities.  
+![image](https://user-images.githubusercontent.com/6797783/199518166-67f8a4ea-dde9-4544-b95d-80ed5f0526aa.png)  
+
+Example of events being emitted from the stream player.  
+![image](https://user-images.githubusercontent.com/6797783/199514155-a94bbb71-c2dc-43d5-81e8-2bd4916a05e4.png)  
+
+There are still plenty of possibilities to optimize the speed in many parts of the code. Any contribution is welcome. Please contact lee.kyuh@gmail.com for any comment / feedback.
+
+
+# Copyright and license
+The codes are released under [GNU General Public License](https://www.gnu.org/licenses/gpl-3.0.en.html).
+
+
+# Citation
+This package was developed as part of the following works:
+  - Yohann Thenaisie* and Kyuhwa Lee* <i>et al.</i>, "Principles of gait encoding in the subthalamic nucleus of people with Parkinson's disease", <i>Science Translational Medicine</i>, 2022, Vol. 14, No. 661, p. eabo1800.<br>(* first authors as equal contribution)
+  - Kyuhwa Lee <i>et al.</i>, "A Brain-Controlled Exoskeleton with Cascaded Event-Related Desynchronization Classifiers", <i>Robotics and Autonomous Systems</i>, Elsevier, 2016, p. 15-23.
+   
+If some of the code here were useful or helpful for your project, I would greatly appreciate if you could cite one of the above papers.
```

### Comparing `neurodecode-2.0.4/neurodecode/__init__.py` & `neurodecode-2.0.5/neurodecode/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-'''
-Initialize PyCNBI logger and other settings
-TODO: support a process-safe file logging
-Kyuhwa Lee
-Swiss Federal Institute of Technology Lausanne (EPFL)
-'''
-
-import os
-import sys
-import logging
-import neurodecode.colorer
-from neurodecode.utils import q_common as qc
-
-# log level options provided by neurodecode
-LOG_LEVELS = {
-    'DEBUG':logging.DEBUG,
-    'INFO':logging.INFO,
-    'INFO_GREEN':22,
-    'INFO_BLUE':24,
-    'INFO_YELLOW':26,
-    'WARNING':logging.WARNING,
-    'ERROR':logging.ERROR
-}
-
-class PycnbiFormatter(logging.Formatter):
-    fmt_debug = "[%(module)s:%(funcName)s:%(lineno)d] DEBUG: %(message)s (%(asctime)s)"
-    fmt_info = "[%(module)s.%(funcName)s] %(message)s"
-    fmt_warning = "[%(module)s.%(funcName)s] WARNING: %(message)s"
-    fmt_error = "[%(module)s:%(funcName)s:%(lineno)d] ERROR: %(message)s"
-
-    def __init__(self, fmt="%(levelno)s: %(message)s"):
-        logging.Formatter.__init__(self, fmt)
-
-    def format(self, record):
-        if record.levelno == LOG_LEVELS['DEBUG']:
-            self._fmt = self.fmt_debug
-        elif record.levelno == LOG_LEVELS['INFO']:
-            self._fmt = self.fmt_info
-        elif record.levelno == LOG_LEVELS['INFO_GREEN']:
-            self._fmt = self.fmt_info
-        elif record.levelno == LOG_LEVELS['INFO_BLUE']:
-            self._fmt = self.fmt_info
-        elif record.levelno == LOG_LEVELS['INFO_YELLOW']:
-            self._fmt = self.fmt_info
-        elif record.levelno == LOG_LEVELS['WARNING']:
-            self._fmt = self.fmt_warning
-        elif record.levelno >= LOG_LEVELS['ERROR']:
-            self._fmt = self.fmt_error
-        self._style = logging.PercentStyle(self._fmt)
-        return logging.Formatter.format(self, record)
-
-def init_logger(logger, verbose_console='INFO'):
-    '''
-    Add the first logger as sys.stdout. Handler will be added only once.
-
-    logger = the logger to initialize
-    verbose_console = logger verbosity
-    '''
-    if not logger.hasHandlers():
-        add_logger_handler(logger, sys.stdout, verbosity=verbose_console)
-
-    '''
-    TODO: add file handler
-    # file logger handler
-    f_handler = logging.FileHandler('neurodecode.log', mode='a')
-    f_handler.setLevel(loglevels[verbose_file])
-    f_format = logging.Formatter('%(levelname)s %(asctime)s %(funcName)s:%(lineno)d: %(message)s')
-    f_handler.setFormatter(f_format)
-    logger.addHandler(f_handler)
-    '''
-
-def add_logger_handler(logger, stream, verbosity='INFO'):
-    # add custom log levels
-    logging.addLevelName(LOG_LEVELS['INFO_GREEN'], 'INFO_GREEN')
-    def __log_info_green(self, message, *args, **kwargs):
-        if self.isEnabledFor(LOG_LEVELS['INFO_GREEN']):
-            self._log(LOG_LEVELS['INFO_GREEN'], message, args, **kwargs)
-    logging.Logger.info_green = __log_info_green
-
-    logging.addLevelName(LOG_LEVELS['INFO_BLUE'], 'INFO_BLUE')
-    def __log_info_blue(self, message, *args, **kwargs):
-        if self.isEnabledFor(LOG_LEVELS['INFO_BLUE']):
-            self._log(LOG_LEVELS['INFO_BLUE'], message, args, **kwargs)
-    logging.Logger.info_blue = __log_info_blue
-
-    logging.addLevelName(LOG_LEVELS['INFO_YELLOW'], 'INFO_YELLOW')
-    def __log_info_yellow(self, message, *args, **kwargs):
-        if self.isEnabledFor(LOG_LEVELS['INFO_YELLOW']):
-            self._log(LOG_LEVELS['INFO_YELLOW'], message, args, **kwargs)
-    logging.Logger.info_yellow = __log_info_yellow
-
-    # console logger handler
-    c_handler = logging.StreamHandler(stream)
-    c_handler.setFormatter(PycnbiFormatter())
-    logger.addHandler(c_handler)
-
-    # minimum possible level of all handlers
-    set_log_level(logger, verbosity, -1)
-    return logger
-
-def set_log_level(logger, verbosity, handler_id=0):
-    '''
-    hander ID 0 is always stdout, followed by user-defined handlers.
-    '''
-    logger.handlers[handler_id].level = LOG_LEVELS[verbosity]
-
-# init scripts
-ROOT = qc.parse_path(os.path.realpath(__file__)).dir
-for d in qc.get_dir_list(ROOT):
-    if os.path.exists('%s/__init__.py' % d):
-        exe_package = 'import neurodecode.%s' % d.replace(ROOT + '/', '')
-        exec(exe_package)
-
-# set loggers
-logging.getLogger('matplotlib').setLevel(logging.ERROR)
-logging.getLogger('sklearn').setLevel(logging.WARNING)
-logging.getLogger('PIL').setLevel(logging.WARNING)
-logging.getLogger('asyncio').setLevel(logging.WARNING)
-
-logger = logging.getLogger('neurodecode')
-logger.propagate = False
-init_logger(logger, 'INFO')
+'''
+Initialize PyCNBI logger and other settings
+TODO: support a process-safe file logging
+Kyuhwa Lee
+Swiss Federal Institute of Technology Lausanne (EPFL)
+'''
+
+import os
+import sys
+import logging
+import neurodecode.colorer
+from neurodecode.utils import q_common as qc
+
+# log level options provided by neurodecode
+LOG_LEVELS = {
+    'DEBUG':logging.DEBUG,
+    'INFO':logging.INFO,
+    'INFO_GREEN':22,
+    'INFO_BLUE':24,
+    'INFO_YELLOW':26,
+    'WARNING':logging.WARNING,
+    'ERROR':logging.ERROR
+}
+
+class PycnbiFormatter(logging.Formatter):
+    fmt_debug = "[%(module)s:%(funcName)s:%(lineno)d] DEBUG: %(message)s (%(asctime)s)"
+    fmt_info = "[%(module)s.%(funcName)s] %(message)s"
+    fmt_warning = "[%(module)s.%(funcName)s] WARNING: %(message)s"
+    fmt_error = "[%(module)s:%(funcName)s:%(lineno)d] ERROR: %(message)s"
+
+    def __init__(self, fmt="%(levelno)s: %(message)s"):
+        logging.Formatter.__init__(self, fmt)
+
+    def format(self, record):
+        if record.levelno == LOG_LEVELS['DEBUG']:
+            self._fmt = self.fmt_debug
+        elif record.levelno == LOG_LEVELS['INFO']:
+            self._fmt = self.fmt_info
+        elif record.levelno == LOG_LEVELS['INFO_GREEN']:
+            self._fmt = self.fmt_info
+        elif record.levelno == LOG_LEVELS['INFO_BLUE']:
+            self._fmt = self.fmt_info
+        elif record.levelno == LOG_LEVELS['INFO_YELLOW']:
+            self._fmt = self.fmt_info
+        elif record.levelno == LOG_LEVELS['WARNING']:
+            self._fmt = self.fmt_warning
+        elif record.levelno >= LOG_LEVELS['ERROR']:
+            self._fmt = self.fmt_error
+        self._style = logging.PercentStyle(self._fmt)
+        return logging.Formatter.format(self, record)
+
+def init_logger(logger, verbose_console='INFO'):
+    '''
+    Add the first logger as sys.stdout. Handler will be added only once.
+
+    logger = the logger to initialize
+    verbose_console = logger verbosity
+    '''
+    if not logger.hasHandlers():
+        add_logger_handler(logger, sys.stdout, verbosity=verbose_console)
+
+    '''
+    TODO: add file handler
+    # file logger handler
+    f_handler = logging.FileHandler('neurodecode.log', mode='a')
+    f_handler.setLevel(loglevels[verbose_file])
+    f_format = logging.Formatter('%(levelname)s %(asctime)s %(funcName)s:%(lineno)d: %(message)s')
+    f_handler.setFormatter(f_format)
+    logger.addHandler(f_handler)
+    '''
+
+def add_logger_handler(logger, stream, verbosity='INFO'):
+    # add custom log levels
+    logging.addLevelName(LOG_LEVELS['INFO_GREEN'], 'INFO_GREEN')
+    def __log_info_green(self, message, *args, **kwargs):
+        if self.isEnabledFor(LOG_LEVELS['INFO_GREEN']):
+            self._log(LOG_LEVELS['INFO_GREEN'], message, args, **kwargs)
+    logging.Logger.info_green = __log_info_green
+
+    logging.addLevelName(LOG_LEVELS['INFO_BLUE'], 'INFO_BLUE')
+    def __log_info_blue(self, message, *args, **kwargs):
+        if self.isEnabledFor(LOG_LEVELS['INFO_BLUE']):
+            self._log(LOG_LEVELS['INFO_BLUE'], message, args, **kwargs)
+    logging.Logger.info_blue = __log_info_blue
+
+    logging.addLevelName(LOG_LEVELS['INFO_YELLOW'], 'INFO_YELLOW')
+    def __log_info_yellow(self, message, *args, **kwargs):
+        if self.isEnabledFor(LOG_LEVELS['INFO_YELLOW']):
+            self._log(LOG_LEVELS['INFO_YELLOW'], message, args, **kwargs)
+    logging.Logger.info_yellow = __log_info_yellow
+
+    # console logger handler
+    c_handler = logging.StreamHandler(stream)
+    c_handler.setFormatter(PycnbiFormatter())
+    logger.addHandler(c_handler)
+
+    # minimum possible level of all handlers
+    set_log_level(logger, verbosity, -1)
+    return logger
+
+def set_log_level(logger, verbosity, handler_id=0):
+    '''
+    hander ID 0 is always stdout, followed by user-defined handlers.
+    '''
+    logger.handlers[handler_id].level = LOG_LEVELS[verbosity]
+
+# init scripts
+ROOT = qc.parse_path(os.path.realpath(__file__)).dir
+for d in qc.get_dir_list(ROOT):
+    if os.path.exists('%s/__init__.py' % d):
+        exe_package = 'import neurodecode.%s' % d.replace(ROOT + '/', '')
+        exec(exe_package)
+
+# set loggers
+logging.getLogger('matplotlib').setLevel(logging.ERROR)
+logging.getLogger('sklearn').setLevel(logging.WARNING)
+logging.getLogger('PIL').setLevel(logging.WARNING)
+logging.getLogger('asyncio').setLevel(logging.WARNING)
+
+logger = logging.getLogger('neurodecode')
+logger.propagate = False
+init_logger(logger, 'INFO')
```

### Comparing `neurodecode-2.0.4/neurodecode/analysis/feature_importances_topo.py` & `neurodecode-2.0.5/neurodecode/analysis/feature_importances_topo.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,181 +1,181 @@
-"""
-Export feature importance distribution using topography map
-
-TODO: merge with parse_features.py to use its API.
-
-"""
-
-import os
-import sys
-import mne
-import neurodecode
-import numpy as np
-import neurodecode.utils.pycnbi_utils as pu
-import neurodecode.utils.q_common as qc
-import matplotlib.pyplot as plt
-from neurodecode import logger
-from matplotlib.figure import Figure
-from builtins import input
-
-def export_topo(data, pos, pngfile, xlabel='', vmin=None, vmax=None, chan_vis=None, res=64, contours=0):
-    mne.viz.plot_topomap(data, pos, names=chan_vis, show_names=True, res=res, contours=contours, show=False)
-    plt.suptitle(xlabel)
-    plt.savefig(pngfile)
-    logger.info('Exported %s' % pngfile)
-
-def feature_importances_topo(featfile, topo_layout_file=None, channels=None, channel_name_show=None):
-    """
-    Compute feature importances across frequency bands and channels
-
-    @params
-    topo_laytout_file: if not None, topography map images will be generated and saved.
-    channel_name_show: list of channel names to show on topography map.
-
-    """
-    logger.info('Loading %s' % featfile)
-
-    if channels is None:
-        channel_set = set()
-        with open(featfile) as f:
-            f.readline()
-            for l in f:
-                ch = l.strip().split('\t')[1]
-                channel_set.add(ch)
-        channels = list(channel_set)
-
-    # channel index lookup table
-    ch2index = {ch:i for i, ch in enumerate(channels)}
-
-    data_delta = np.zeros(len(channels))
-    data_theta = np.zeros(len(channels))
-    data_mu = np.zeros(len(channels))
-    data_beta = np.zeros(len(channels))
-    data_beta1 = np.zeros(len(channels))
-    data_beta2 = np.zeros(len(channels))
-    data_beta3 = np.zeros(len(channels))
-    data_lgamma = np.zeros(len(channels))
-    data_hgamma = np.zeros(len(channels))
-    data_per_ch = np.zeros(len(channels))
-
-    f = open(featfile)
-    f.readline()
-    for l in f:
-        token = l.strip().split('\t')
-        importance = float(token[0])
-        ch = token[1]
-        fq = float(token[2])
-        if fq <= 3:
-            data_delta[ch2index[ch]] += importance
-        elif fq <= 7:
-            data_theta[ch2index[ch]] += importance
-        elif fq <= 12:
-            data_mu[ch2index[ch]] += importance
-        elif fq <= 30:
-            data_beta[ch2index[ch]] += importance
-        elif fq <= 70:
-            data_lgamma[ch2index[ch]] += importance
-        else:
-            data_hgamma[ch2index[ch]] += importance
-        if 12.5 <= fq <= 16:
-            data_beta1[ch2index[ch]] += importance
-        elif fq <= 20:
-            data_beta2[ch2index[ch]] += importance
-        elif fq <= 28:
-            data_beta3[ch2index[ch]] += importance
-        data_per_ch[ch2index[ch]] += importance
-
-    hlen = 18 + len(channels) * 7
-    result = '>> Feature importance distribution\n'
-    result += 'bands   ' + qc.list2string(channels, '%6s') + ' | ' + 'per band\n'
-    result += '-' * hlen + '\n'
-    result += 'delta   ' + qc.list2string(data_delta, '%6.2f') + ' | %6.2f\n' % np.sum(data_delta)
-    result += 'theta   ' + qc.list2string(data_theta, '%6.2f') + ' | %6.2f\n' % np.sum(data_theta)
-    result += 'mu      ' + qc.list2string(data_mu, '%6.2f') + ' | %6.2f\n' % np.sum(data_mu)
-    #result += 'beta    ' + qc.list2string(data_beta, '%6.2f') + ' | %6.2f\n' % np.sum(data_beta)
-    result += 'beta1   ' + qc.list2string(data_beta1, '%6.2f') + ' | %6.2f\n' % np.sum(data_beta1)
-    result += 'beta2   ' + qc.list2string(data_beta2, '%6.2f') + ' | %6.2f\n' % np.sum(data_beta2)
-    result += 'beta3   ' + qc.list2string(data_beta3, '%6.2f') + ' | %6.2f\n' % np.sum(data_beta3)
-    result += 'lgamma  ' + qc.list2string(data_lgamma, '%6.2f') + ' | %6.2f\n' % np.sum(data_lgamma)
-    result += 'hgamma  ' + qc.list2string(data_hgamma, '%6.2f') + ' | %6.2f\n' % np.sum(data_hgamma)
-    result += '-' * hlen + '\n'
-    result += 'per_ch  ' + qc.list2string(data_per_ch, '%6.2f') + ' | 100.00\n'
-    print(result)
-    p = qc.parse_path(featfile)
-    open('%s/%s_summary.txt' % (p.dir, p.name), 'w').write(result)
-
-    # export topo maps
-    if topo_layout_file is not None:
-        # default visualization setting
-        res = 64
-        contours = 6
-
-        # select channel names to show
-        if channel_name_show is None:
-            channel_name_show = channels
-        chan_vis = [''] * len(channels)
-        for ch in channel_name_show:
-            chan_vis[channels.index(ch)] = ch
-
-        # set channel locations and reverse lookup table
-        chanloc = {}
-        if not os.path.exists(topo_layout_file):
-            raise FileNotFoundError('Layout file %s not found.' % topo_layout_file)
-        logger.info('Using layout %s' % topo_layout_file)
-        for l in open(topo_layout_file):
-            token = l.strip().split('\t')
-            ch = token[5]
-            x = float(token[1])
-            y = float(token[2])
-            chanloc[ch] = [x, y]
-        pos = np.zeros((len(channels),2))
-        for i, ch in enumerate(channels):
-            pos[i] = chanloc[ch]
-
-        vmin = min(data_per_ch)
-        vmax = max(data_per_ch)
-        total = sum(data_per_ch)
-        rate_delta = sum(data_delta) * 100.0 / total
-        rate_theta = sum(data_theta) * 100.0 / total
-        rate_mu = sum(data_mu) * 100.0 / total
-        rate_beta = sum(data_beta) * 100.0 / total
-        rate_beta1 = sum(data_beta1) * 100.0 / total
-        rate_beta2 = sum(data_beta2) * 100.0 / total
-        rate_beta3 = sum(data_beta3) * 100.0 / total
-        rate_lgamma = sum(data_lgamma) * 100.0 / total
-        rate_hgamma = sum(data_hgamma) * 100.0 / total
-        export_topo(data_per_ch, pos, 'features_topo_all.png', xlabel='all bands 1-40 Hz', chan_vis=chan_vis)
-        export_topo(data_delta, pos, 'features_topo_delta.png', xlabel='delta 1-3 Hz (%.1f%%)' % rate_delta, chan_vis=chan_vis)
-        export_topo(data_theta, pos, 'features_topo_theta.png', xlabel='theta 4-7 Hz (%.1f%%)' % rate_theta, chan_vis=chan_vis)
-        export_topo(data_mu, pos, 'features_topo_mu.png', xlabel='mu 8-12 Hz (%.1f%%)' % rate_mu, chan_vis=chan_vis)
-        export_topo(data_beta, pos, 'features_topo_beta.png', xlabel='beta 13-30 Hz (%.1f%%)' % rate_beta, chan_vis=chan_vis)
-        export_topo(data_beta1, pos, 'features_topo_beta1.png', xlabel='beta 12.5-16 Hz (%.1f%%)' % rate_beta1, chan_vis=chan_vis)
-        export_topo(data_beta2, pos, 'features_topo_beta2.png', xlabel='beta 16-20 Hz (%.1f%%)' % rate_beta2, chan_vis=chan_vis)
-        export_topo(data_beta3, pos, 'features_topo_beta3.png', xlabel='beta 20-28 Hz (%.1f%%)' % rate_beta3, chan_vis=chan_vis)
-        export_topo(data_lgamma, pos, 'features_topo_lowgamma.png', xlabel='low gamma 31-40 Hz (%.1f%%)' % rate_lgamma, chan_vis=chan_vis)
-
-def config_run(featfile=None, topo_layout_file=None):
-    if featfile is None or len(featfile.strip()) == 0:
-        if os.path.exists('good_features.txt'):
-            featfile = os.path.realpath('good_features.txt').replace('\\', '/')
-            logger.info('Found %s in the current folder.' % featfile)
-        else:
-            featfile = input('Feature file path? ')
-
-    if topo_layout_file is None or len(topo_layout_file.strip()) == 0:
-        topo_layout_file = 'antneuro_64ch.lay'
-
-    feature_importances_topo(featfile, topo_layout_file)
-
-def main():
-    """
-    Invoked from the console
-    """
-    if len(sys.argv) > 2:
-        config_run(sys.argv[1], sys.argv[2])
-    elif len(sys.argv) > 1:
-        config_run(sys.argv[1])
-    else:
-        config_run()
-
-if __name__ == '__main__':
-    main()
+"""
+Export feature importance distribution using topography map
+
+TODO: merge with parse_features.py to use its API.
+
+"""
+
+import os
+import sys
+import mne
+import neurodecode
+import numpy as np
+import neurodecode.utils.pycnbi_utils as pu
+import neurodecode.utils.q_common as qc
+import matplotlib.pyplot as plt
+from neurodecode import logger
+from matplotlib.figure import Figure
+from builtins import input
+
+def export_topo(data, pos, pngfile, xlabel='', vmin=None, vmax=None, chan_vis=None, res=64, contours=0):
+    mne.viz.plot_topomap(data, pos, names=chan_vis, show_names=True, res=res, contours=contours, show=False)
+    plt.suptitle(xlabel)
+    plt.savefig(pngfile)
+    logger.info('Exported %s' % pngfile)
+
+def feature_importances_topo(featfile, topo_layout_file=None, channels=None, channel_name_show=None):
+    """
+    Compute feature importances across frequency bands and channels
+
+    @params
+    topo_laytout_file: if not None, topography map images will be generated and saved.
+    channel_name_show: list of channel names to show on topography map.
+
+    """
+    logger.info('Loading %s' % featfile)
+
+    if channels is None:
+        channel_set = set()
+        with open(featfile) as f:
+            f.readline()
+            for l in f:
+                ch = l.strip().split('\t')[1]
+                channel_set.add(ch)
+        channels = list(channel_set)
+
+    # channel index lookup table
+    ch2index = {ch:i for i, ch in enumerate(channels)}
+
+    data_delta = np.zeros(len(channels))
+    data_theta = np.zeros(len(channels))
+    data_mu = np.zeros(len(channels))
+    data_beta = np.zeros(len(channels))
+    data_beta1 = np.zeros(len(channels))
+    data_beta2 = np.zeros(len(channels))
+    data_beta3 = np.zeros(len(channels))
+    data_lgamma = np.zeros(len(channels))
+    data_hgamma = np.zeros(len(channels))
+    data_per_ch = np.zeros(len(channels))
+
+    f = open(featfile)
+    f.readline()
+    for l in f:
+        token = l.strip().split('\t')
+        importance = float(token[0])
+        ch = token[1]
+        fq = float(token[2])
+        if fq <= 3:
+            data_delta[ch2index[ch]] += importance
+        elif fq <= 7:
+            data_theta[ch2index[ch]] += importance
+        elif fq <= 12:
+            data_mu[ch2index[ch]] += importance
+        elif fq <= 30:
+            data_beta[ch2index[ch]] += importance
+        elif fq <= 70:
+            data_lgamma[ch2index[ch]] += importance
+        else:
+            data_hgamma[ch2index[ch]] += importance
+        if 12.5 <= fq <= 16:
+            data_beta1[ch2index[ch]] += importance
+        elif fq <= 20:
+            data_beta2[ch2index[ch]] += importance
+        elif fq <= 28:
+            data_beta3[ch2index[ch]] += importance
+        data_per_ch[ch2index[ch]] += importance
+
+    hlen = 18 + len(channels) * 7
+    result = '>> Feature importance distribution\n'
+    result += 'bands   ' + qc.list2string(channels, '%6s') + ' | ' + 'per band\n'
+    result += '-' * hlen + '\n'
+    result += 'delta   ' + qc.list2string(data_delta, '%6.2f') + ' | %6.2f\n' % np.sum(data_delta)
+    result += 'theta   ' + qc.list2string(data_theta, '%6.2f') + ' | %6.2f\n' % np.sum(data_theta)
+    result += 'mu      ' + qc.list2string(data_mu, '%6.2f') + ' | %6.2f\n' % np.sum(data_mu)
+    #result += 'beta    ' + qc.list2string(data_beta, '%6.2f') + ' | %6.2f\n' % np.sum(data_beta)
+    result += 'beta1   ' + qc.list2string(data_beta1, '%6.2f') + ' | %6.2f\n' % np.sum(data_beta1)
+    result += 'beta2   ' + qc.list2string(data_beta2, '%6.2f') + ' | %6.2f\n' % np.sum(data_beta2)
+    result += 'beta3   ' + qc.list2string(data_beta3, '%6.2f') + ' | %6.2f\n' % np.sum(data_beta3)
+    result += 'lgamma  ' + qc.list2string(data_lgamma, '%6.2f') + ' | %6.2f\n' % np.sum(data_lgamma)
+    result += 'hgamma  ' + qc.list2string(data_hgamma, '%6.2f') + ' | %6.2f\n' % np.sum(data_hgamma)
+    result += '-' * hlen + '\n'
+    result += 'per_ch  ' + qc.list2string(data_per_ch, '%6.2f') + ' | 100.00\n'
+    print(result)
+    p = qc.parse_path(featfile)
+    open('%s/%s_summary.txt' % (p.dir, p.name), 'w').write(result)
+
+    # export topo maps
+    if topo_layout_file is not None:
+        # default visualization setting
+        res = 64
+        contours = 6
+
+        # select channel names to show
+        if channel_name_show is None:
+            channel_name_show = channels
+        chan_vis = [''] * len(channels)
+        for ch in channel_name_show:
+            chan_vis[channels.index(ch)] = ch
+
+        # set channel locations and reverse lookup table
+        chanloc = {}
+        if not os.path.exists(topo_layout_file):
+            raise FileNotFoundError('Layout file %s not found.' % topo_layout_file)
+        logger.info('Using layout %s' % topo_layout_file)
+        for l in open(topo_layout_file):
+            token = l.strip().split('\t')
+            ch = token[5]
+            x = float(token[1])
+            y = float(token[2])
+            chanloc[ch] = [x, y]
+        pos = np.zeros((len(channels),2))
+        for i, ch in enumerate(channels):
+            pos[i] = chanloc[ch]
+
+        vmin = min(data_per_ch)
+        vmax = max(data_per_ch)
+        total = sum(data_per_ch)
+        rate_delta = sum(data_delta) * 100.0 / total
+        rate_theta = sum(data_theta) * 100.0 / total
+        rate_mu = sum(data_mu) * 100.0 / total
+        rate_beta = sum(data_beta) * 100.0 / total
+        rate_beta1 = sum(data_beta1) * 100.0 / total
+        rate_beta2 = sum(data_beta2) * 100.0 / total
+        rate_beta3 = sum(data_beta3) * 100.0 / total
+        rate_lgamma = sum(data_lgamma) * 100.0 / total
+        rate_hgamma = sum(data_hgamma) * 100.0 / total
+        export_topo(data_per_ch, pos, 'features_topo_all.png', xlabel='all bands 1-40 Hz', chan_vis=chan_vis)
+        export_topo(data_delta, pos, 'features_topo_delta.png', xlabel='delta 1-3 Hz (%.1f%%)' % rate_delta, chan_vis=chan_vis)
+        export_topo(data_theta, pos, 'features_topo_theta.png', xlabel='theta 4-7 Hz (%.1f%%)' % rate_theta, chan_vis=chan_vis)
+        export_topo(data_mu, pos, 'features_topo_mu.png', xlabel='mu 8-12 Hz (%.1f%%)' % rate_mu, chan_vis=chan_vis)
+        export_topo(data_beta, pos, 'features_topo_beta.png', xlabel='beta 13-30 Hz (%.1f%%)' % rate_beta, chan_vis=chan_vis)
+        export_topo(data_beta1, pos, 'features_topo_beta1.png', xlabel='beta 12.5-16 Hz (%.1f%%)' % rate_beta1, chan_vis=chan_vis)
+        export_topo(data_beta2, pos, 'features_topo_beta2.png', xlabel='beta 16-20 Hz (%.1f%%)' % rate_beta2, chan_vis=chan_vis)
+        export_topo(data_beta3, pos, 'features_topo_beta3.png', xlabel='beta 20-28 Hz (%.1f%%)' % rate_beta3, chan_vis=chan_vis)
+        export_topo(data_lgamma, pos, 'features_topo_lowgamma.png', xlabel='low gamma 31-40 Hz (%.1f%%)' % rate_lgamma, chan_vis=chan_vis)
+
+def config_run(featfile=None, topo_layout_file=None):
+    if featfile is None or len(featfile.strip()) == 0:
+        if os.path.exists('good_features.txt'):
+            featfile = os.path.realpath('good_features.txt').replace('\\', '/')
+            logger.info('Found %s in the current folder.' % featfile)
+        else:
+            featfile = input('Feature file path? ')
+
+    if topo_layout_file is None or len(topo_layout_file.strip()) == 0:
+        topo_layout_file = 'antneuro_64ch.lay'
+
+    feature_importances_topo(featfile, topo_layout_file)
+
+def main():
+    """
+    Invoked from the console
+    """
+    if len(sys.argv) > 2:
+        config_run(sys.argv[1], sys.argv[2])
+    elif len(sys.argv) > 1:
+        config_run(sys.argv[1])
+    else:
+        config_run()
+
+if __name__ == '__main__':
+    main()
```

### Comparing `neurodecode-2.0.4/neurodecode/analysis/parse_features.py` & `neurodecode-2.0.5/neurodecode/analysis/parse_features.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,193 +1,194 @@
-# -*- coding: utf-8 -*-
-from __future__ import print_function, division, unicode_literals
-
-"""
-Parse features generated by Random Forest classifier and
-compute feature importance distribution.
-
-@author: Kyuhwa Lee
-Swiss Federal Institute of Technology Lausanne (EPFL)
-
-"""
-
-import os
-import sys
-import neurodecode
-import scipy.io
-import numpy as np
-from neurodecode import logger
-from neurodecode.utils import q_common as qc
-
-def get_feature_scores(featfile, channels=None, freq_ranges=None, matfile=None):
-    """
-    Parse feature importance scores generated by decoder.trainer.run_trainer() and
-    compute feature importance distribution. The raw scores are importance ratio
-    per feature to all features.
-
-    Input
-    -----
-    featfile: Feature importance distribution file computed by Random Forests.
-              Each line contains 3 columns separated by tab: Score Channel Frequency
-              e.g. 66.6\tCz\t18
-    channels: List of channel names. If None, all channels in featfile will be used.
-    freq_ranges: Per-band frequency range. dict:{band_name:[fq_low, fq_high]}
-                 fq_high is inclusive in the range.
-                 if None, predefined bands will be used.
-
-    Output
-    ------
-    data: Feature importance score. {band_name:percentage}
-          'channel' field contains the sum of all scores per channel.
-          'raw' field contains raw scores of all channels and frequency bins
-    """
-
-    # default ranges
-    if freq_ranges is None:
-        freq_ranges = dict(
-            delta=[1, 4],
-            theta=[4, 8],
-            alpha=[8, 13],
-            beta1=[13, 18],
-            beta2=[18, 24],
-            beta3=[24, 30],
-            gamma=[31, 49])
-
-    # find all channels first if needed
-    if channels is None:
-        channels = []
-        with open(featfile) as f:
-            f.readline()
-            for l in f:
-                ch = l.strip().split('\t')[1]
-                if ch not in channels:
-                    channels.append(ch)
-        channels.sort()
-
-    # build channel index lookup table
-    ch2index = {ch:i for i, ch in enumerate(channels)}
-
-    # initialise data structure
-    data = {'channel':np.zeros(len(channels)), 'ch_names':channels,
-        'raw':{ch:{} for ch in channels}, 'freq_ranges':freq_ranges}
-#        'norm':{ch:{} for ch in channels}}
-    for band in freq_ranges:
-        data[band] = np.zeros(len(channels))
-
-    # start parsing
-    f = open(featfile)
-    f.readline()
-    for l in f:
-        token = l.strip().split('\t')
-        importance = float(token[0])
-        ch = token[1]
-        if ch not in channels:
-            continue
-        fq = float(token[2])
-        data['raw'][ch][fq] = importance
-        for band in freq_ranges:
-            if freq_ranges[band][0] <= fq <= freq_ranges[band][1]:
-                data[band][ch2index[ch]] += importance
-        data['channel'][ch2index[ch]] += importance
-
-    # MATLAB export
-    if matfile is not None:
-        # matvar = [fq] x [ch]
-        matvar = np.zeros([len(data['raw'][channels[0]]), len(channels)])
-        fqlist = sorted(list(data['raw'][channels[0]].keys()))
-        fq2index = {fq:i for i, fq in enumerate(fqlist)}
-        for ch in channels:
-            for fq in fqlist:
-                try:
-                    matvar[fq2index[fq]][ch2index[ch]] = data['raw'][ch][fq]
-                except KeyError:
-                    matvar[fq2index[fq]][ch2index[ch]] = 0
-        scipy.io.savemat(matfile, {'scores':matvar, 'channels':channels, 'frequencies':fqlist})
-        logger.info('Data exported to %s\n' % matfile)
-
-    return data
-
-def print_feature_scores(data, num_cols=8):
-    """
-    print features with number of channels per line set by num_cols (default=8)
-
-    """
-    print('-- Feature importance distribution --')
-    channels = data['ch_names']
-    channels_split = []
-    for i in range(len(channels)):
-        if i % num_cols == 0:
-            channels_split.append([])
-        channels_split[-1].append(i)
-    for i, chs in enumerate(channels_split):
-        channels_subset = ['%6s' % channels[ch] for ch in chs]
-        txt = 'bands   | ' + ' '.join(channels_subset)
-        if i == (len(channels_split) - 1):
-            txt += ' | per band'
-        rowlen = len(txt)
-        print('=' * rowlen)
-        print(txt)
-        print('-' * rowlen)
-        for band in data:
-            if band in ['channel', 'raw', 'freq_ranges', 'ch_names']:
-                continue
-            band_name = '%d-%d' % (data['freq_ranges'][band][0], data['freq_ranges'][band][1])
-            band_scores = []
-            for ch_i in chs:
-                band_scores.append('%6.2f' % data[band][ch_i])
-            txt = '%-7s | %s' % (band_name, ' '.join(band_scores))
-            if i == (len(channels_split) - 1):
-                txt += ' | %6.2f' % np.sum(data[band])
-            print(txt)
-        txt = []
-        for ch_i in chs:
-            txt.append('%6.2f' % data['channel'][ch_i])
-        if i == (len(channels_split) - 1):
-            txt.append('| %6.2f' % sum(data['channel']))
-        print('-' * rowlen)
-        print('per chan| %s' % ' '.join(txt))
-
-def feature_info(featfile, channels=None, freq_ranges=None, matfile=None):
-    """
-    Wrapper function to get feature importance and print statistics
-    """
-    data = get_feature_scores(featfile, channels, freq_ranges, matfile)
-    print_feature_scores(data)
-
-
-def config_run(featfile=None):
-    if featfile is None or len(featfile.strip()) == 0:
-        if os.path.exists('good_features.txt'):
-            featfile = os.path.realpath('good_features.txt').replace('\\', '/')
-            logger.info('Found %s in the current folder.' % featfile)
-        else:
-            featfile = input('Feature file path? ')
-    feature_info(featfile)
-
-
-# sample code
-def sample_code():
-    FEATFILE = r'D:\data\MI\z2\LR\classifier\good_features.txt'
-    CHANNELS = ['C3', 'C4', 'Cz']
-    FREQ_RANGES = dict(
-        delta=[1, 4],
-        theta=[4, 8],
-        alpha=[8, 13],
-        beta=[13, 30],
-        lgamma=[30, 49])
-    #MATFILE = '%s/good_features.mat' % qc.parse_path(FEATFILE).dir
-    MATFILE = None
-    feature_info(FEATFILE, CHANNELS, FREQ_RANGES, MATFILE)
-
-def main():
-    """
-    Invoked from console
-    """
-    if len(sys.argv) < 2:
-        print('Usage: %s feature_file' % os.path.basename(__file__))
-        return
-
-    featfile = sys.argv[1]
-    config_run(featfile)
-
-if __name__ == '__main__':
-    main()
+# -*- coding: utf-8 -*-
+from __future__ import print_function, division, unicode_literals
+
+"""
+Parse features generated by Random Forest classifier and
+compute feature importance distribution.
+
+@author: Kyuhwa Lee
+Swiss Federal Institute of Technology Lausanne (EPFL)
+
+"""
+
+import os
+import sys
+import neurodecode
+import scipy.io
+import numpy as np
+from neurodecode import logger
+from neurodecode.utils import q_common as qc
+
+def get_feature_scores(featfile, channels=None, freq_ranges=None, matfile=None):
+    """
+    Parse feature importance scores generated by decoder.trainer.run_trainer() and
+    compute feature importance distribution. The raw scores are importance ratio
+    per feature to all features.
+
+    Input
+    -----
+    featfile: Feature importance distribution file computed by Random Forests.
+              Each line contains 3 columns separated by tab: Score Channel Frequency
+              e.g. 66.6\tCz\t18
+    channels: List of channel names. If None, all channels in featfile will be used.
+    freq_ranges: Per-band frequency range. dict:{band_name:[fq_low, fq_high]}
+                 fq_high is inclusive in the range.
+                 if None, predefined bands will be used.
+
+    Output
+    ------
+    data: Feature importance score. {band_name:percentage}
+          'channel' field contains the sum of all scores per channel.
+          'raw' field contains raw scores of all channels and frequency bins
+    """
+
+    # default ranges
+    if freq_ranges is None:
+        freq_ranges = dict(
+            delta=[1, 4],
+            theta=[4, 8],
+            alpha=[8, 13],
+            beta1=[13, 18],
+            beta2=[18, 24],
+            beta3=[24, 30],
+            gamma1=[31, 49],
+            gamma2=[50, 140])
+
+    # find all channels first if needed
+    if channels is None:
+        channels = []
+        with open(featfile) as f:
+            f.readline()
+            for l in f:
+                ch = l.strip().split('\t')[1]
+                if ch not in channels:
+                    channels.append(ch)
+        channels.sort()
+
+    # build channel index lookup table
+    ch2index = {ch:i for i, ch in enumerate(channels)}
+
+    # initialise data structure
+    data = {'channel':np.zeros(len(channels)), 'ch_names':channels,
+        'raw':{ch:{} for ch in channels}, 'freq_ranges':freq_ranges}
+#        'norm':{ch:{} for ch in channels}}
+    for band in freq_ranges:
+        data[band] = np.zeros(len(channels))
+
+    # start parsing
+    f = open(featfile)
+    f.readline()
+    for l in f:
+        token = l.strip().split('\t')
+        importance = float(token[0])
+        ch = token[1]
+        if ch not in channels:
+            continue
+        fq = float(token[2])
+        data['raw'][ch][fq] = importance
+        for band in freq_ranges:
+            if freq_ranges[band][0] <= fq <= freq_ranges[band][1]:
+                data[band][ch2index[ch]] += importance
+        data['channel'][ch2index[ch]] += importance
+
+    # MATLAB export
+    if matfile is not None:
+        # matvar = [fq] x [ch]
+        matvar = np.zeros([len(data['raw'][channels[0]]), len(channels)])
+        fqlist = sorted(list(data['raw'][channels[0]].keys()))
+        fq2index = {fq:i for i, fq in enumerate(fqlist)}
+        for ch in channels:
+            for fq in fqlist:
+                try:
+                    matvar[fq2index[fq]][ch2index[ch]] = data['raw'][ch][fq]
+                except KeyError:
+                    matvar[fq2index[fq]][ch2index[ch]] = 0
+        scipy.io.savemat(matfile, {'scores':matvar, 'channels':channels, 'frequencies':fqlist})
+        logger.info('Data exported to %s\n' % matfile)
+
+    return data
+
+def print_feature_scores(data, num_cols=8):
+    """
+    print features with number of channels per line set by num_cols (default=8)
+
+    """
+    print('-- Feature importance distribution --')
+    channels = data['ch_names']
+    channels_split = []
+    for i in range(len(channels)):
+        if i % num_cols == 0:
+            channels_split.append([])
+        channels_split[-1].append(i)
+    for i, chs in enumerate(channels_split):
+        channels_subset = ['%6s' % channels[ch] for ch in chs]
+        txt = 'bands   | ' + ' '.join(channels_subset)
+        if i == (len(channels_split) - 1):
+            txt += ' | per band'
+        rowlen = len(txt)
+        print('=' * rowlen)
+        print(txt)
+        print('-' * rowlen)
+        for band in data:
+            if band in ['channel', 'raw', 'freq_ranges', 'ch_names']:
+                continue
+            band_name = '%d-%d' % (data['freq_ranges'][band][0], data['freq_ranges'][band][1])
+            band_scores = []
+            for ch_i in chs:
+                band_scores.append('%6.2f' % data[band][ch_i])
+            txt = '%-7s | %s' % (band_name, ' '.join(band_scores))
+            if i == (len(channels_split) - 1):
+                txt += ' | %6.2f' % np.sum(data[band])
+            print(txt)
+        txt = []
+        for ch_i in chs:
+            txt.append('%6.2f' % data['channel'][ch_i])
+        if i == (len(channels_split) - 1):
+            txt.append('| %6.2f' % sum(data['channel']))
+        print('-' * rowlen)
+        print('per chan| %s' % ' '.join(txt))
+
+def feature_info(featfile, channels=None, freq_ranges=None, matfile=None):
+    """
+    Wrapper function to get feature importance and print statistics
+    """
+    data = get_feature_scores(featfile, channels, freq_ranges, matfile)
+    print_feature_scores(data)
+
+
+def config_run(featfile=None):
+    if featfile is None or len(featfile.strip()) == 0:
+        if os.path.exists('good_features.txt'):
+            featfile = os.path.realpath('good_features.txt').replace('\\', '/')
+            logger.info('Found %s in the current folder.' % featfile)
+        else:
+            featfile = input('Feature file path? ')
+    feature_info(featfile)
+
+
+# sample code
+def sample_code():
+    FEATFILE = r'D:\data\MI\z2\LR\classifier\good_features.txt'
+    CHANNELS = ['C3', 'C4', 'Cz']
+    FREQ_RANGES = dict(
+        delta=[1, 4],
+        theta=[4, 8],
+        alpha=[8, 13],
+        beta=[13, 30],
+        lgamma=[30, 49])
+    #MATFILE = '%s/good_features.mat' % qc.parse_path(FEATFILE).dir
+    MATFILE = None
+    feature_info(FEATFILE, CHANNELS, FREQ_RANGES, MATFILE)
+
+def main():
+    """
+    Invoked from console
+    """
+    if len(sys.argv) < 2:
+        print('Usage: %s feature_file' % os.path.basename(__file__))
+        return
+
+    featfile = sys.argv[1]
+    config_run(featfile)
+
+if __name__ == '__main__':
+    main()
```

### Comparing `neurodecode-2.0.4/neurodecode/analysis/tfr_export.py` & `neurodecode-2.0.5/neurodecode/analysis/tfr_export.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,307 +1,307 @@
-from __future__ import print_function, division
-
-"""
-Time-frequency analysis using Morlet wavelets or multitapers
-
-Kyuhwa Lee
-EPFL, 2019
-
-"""
-
-import sys
-import os
-import mne
-import imp
-import pdb
-import scipy
-import traceback
-import numpy as np
-import multiprocessing as mp
-import mne.time_frequency
-import matplotlib.pyplot as plt
-import neurodecode.utils.pycnbi_utils as pu
-import neurodecode.utils.q_common as qc
-from neurodecode.triggers.trigger_def import trigger_def
-from neurodecode import logger
-from builtins import input
-from scipy.signal import lfilter
-from scipy.signal import butter
-from scipy.signal import hilbert
-
-def check_config(cfg):
-    if not hasattr(cfg, 'TFR_TYPE'):
-        cfg.TFR_TYPE = 'multitaper'
-    if not hasattr(cfg, 'N_JOBS'):
-        cfg.N_JOBS = None
-    if not hasattr(cfg, 'T_BUFFER'):
-        cfg.T_BUFFER = 1
-    if not hasattr(cfg, 'BS_MODE'):
-        cfg.BS_MODE = 'logratio'
-    if not hasattr(cfg, 'BS_TIMES'):
-        cfg.BS_TIMES = (None, 0)
-    if not hasattr(cfg, 'EXPORT_PNG'):
-        cfg.EXPORT_PNG = False
-    if not hasattr(cfg, 'EXPORT_MATLAB'):
-        cfg.MATLAB = False
-    if not hasattr(cfg, 'EXPORT_PATH'):
-        cfg.EXPORT_PATH = None
-    return cfg
-
-def butter_bandpass(lowcut, highcut, fs, order=5):
-    nyq = fs / 2.0
-    low = lowcut / nyq
-    high = highcut / nyq
-    b, a = butter(order, [low, high], btype='band')
-    return b, a
-
-def get_tfr(cfg, recursive=False, n_jobs=1):
-    '''
-    @params:
-    tfr_type: 'multitaper' or 'morlet'
-    recursive: if True, load raw files in sub-dirs recursively
-    export_path: path to save plots
-    n_jobs: number of cores to run in parallel
-    '''
-
-    cfg = check_config(cfg)
-    tfr_type = cfg.TFR_TYPE
-    export_path = cfg.EXPORT_PATH
-    t_buffer = cfg.T_BUFFER
-    if tfr_type == 'multitaper':
-        tfr = mne.time_frequency.tfr_multitaper
-    elif tfr_type == 'morlet':
-        tfr = mne.time_frequency.tfr_morlet
-    elif tfr_type == 'butter':
-        butter_order = 4 # TODO: parameterize
-        tfr = lfilter
-    elif tfr_type == 'fir':
-        raise NotImplementedError
-    else:
-        raise ValueError('Wrong TFR type %s' % tfr_type)
-    if cfg.DECIM_FACTOR is None:
-        decim = 1
-    else:
-        decim = int(cfg.DECIM_FACTOR)
-    n_jobs = cfg.N_JOBS
-    if n_jobs is None:
-        n_jobs = mp.cpu_count()
-
-    if hasattr(cfg, 'DATA_PATHS'):
-        if export_path is None:
-            raise ValueError('For multiple directories, cfg.EXPORT_PATH cannot be None')
-        else:
-            outpath = export_path
-        # custom event file
-        if hasattr(cfg, 'EVENT_FILE') and cfg.EVENT_FILE is not None:
-            events = mne.read_events(cfg.EVENT_FILE)
-        file_prefix = 'grandavg'
-
-        # load and merge files from all directories
-        flist = []
-        for ddir in cfg.DATA_PATHS:
-            ddir = ddir.replace('\\', '/')
-            if ddir[-1] != '/': ddir += '/'
-            for f in qc.get_file_list(ddir, fullpath=True, recursive=recursive):
-                if qc.parse_path(f).ext in ['fif', 'bdf', 'gdf']:
-                    flist.append(f)
-        raw, events = pu.load_multi(flist)
-    elif hasattr(cfg, 'DATA_FILE'):
-        logger.info('Loading %s' % cfg.DATA_FILE)
-        raw, events = pu.load_raw(cfg.DATA_FILE)
-
-        # custom events
-        if hasattr(cfg, 'EVENT_FILE') and cfg.EVENT_FILE is not None:
-            events = mne.read_events(cfg.EVENT_FILE)
-
-        if export_path is None:
-            [outpath, file_prefix, _] = qc.parse_path_list(cfg.DATA_FILE)
-        else:
-            file_prefix = qc.parse_path(cfg.DATA_FILE).name
-            outpath = export_path
-            file_prefix = qc.parse_path(cfg.DATA_FILE).name
-    else:
-        logger.error('Either DATA_PATHS or DATA_FILE is required in config file')
-        raise ValueError
-
-    # re-referencing
-    if cfg.REREFERENCE is not None:
-        pu.rereference(raw, cfg.REREFERENCE[1], cfg.REREFERENCE[0])
-        assert cfg.REREFERENCE[0] in raw.ch_names
-
-    sfreq = raw.info['sfreq']
-
-    # set channels of interest
-    picks = pu.channel_names_to_index(raw, cfg.CHANNEL_PICKS)
-
-    if max(picks) > len(raw.info['ch_names']):
-        msg = 'ERROR: "picks" has a channel index %d while there are only %d channels.' %\
-              (max(picks), len(raw.info['ch_names']))
-        raise RuntimeError(msg)
-
-    # Apply filters
-    raw = pu.preprocess(raw, spatial=cfg.SP_FILTER, spatial_ch=picks, spectral=cfg.TP_FILTER,
-                  spectral_ch=picks, notch=cfg.NOTCH_FILTER, notch_ch=picks,
-                  multiplier=cfg.MULTIPLIER, n_jobs=n_jobs, decim=decim)
-    sfreq /= decim
-    events[:,0] //= decim
-
-    # Read epochs
-    classes = {}
-    event_set = set(events[:, -1])
-    for t_name in cfg.TRIGGER_DEF:
-        if cfg.TRIGGER_FILE is not None:
-            tdef = trigger_def(cfg.TRIGGER_FILE)
-            t_value = tdef.by_name[t_name]
-            if t_value in event_set:
-                classes[t_name] = t_value
-        else:
-            classes[str(t_name)] = t_name
-    if len(classes) == 0:
-        raise ValueError('No desired event was found from the data.')
-
-    try:
-        tmin = cfg.EPOCH[0]
-        tmin_buffer = tmin - t_buffer
-        raw_tmax = raw._data.shape[1] / sfreq - 0.1
-        if cfg.EPOCH[1] is None:
-            if cfg.POWER_AVERAGED:
-                raise ValueError('EPOCH value cannot have None for grand averaged TFR')
-            else:
-                if len(cfg.TRIGGERS) > 1:
-                    raise ValueError('If the end time of EPOCH is None, only a single event can be defined.')
-                t_ref = events[np.where(events[:,2] == list(cfg.TRIGGERS)[0])[0][0], 0] / sfreq
-                tmax = raw_tmax - t_ref - t_buffer
-        else:
-            tmax = cfg.EPOCH[1]
-        tmax_buffer = tmax + t_buffer
-        if tmax_buffer > raw_tmax:
-            raise ValueError('Epoch length with buffer (%.3f) is larger than signal length (%.3f)' % (tmax_buffer, raw_tmax))
-        epochs_all = mne.Epochs(raw, events, classes, tmin=tmin_buffer, tmax=tmax_buffer,
-                                proj=False, picks=picks, baseline=None, preload=True)
-        if epochs_all.drop_log_stats() > 0:
-            logger.error('\n** Bad epochs found. Dropping into a Python shell.')
-            logger.error(epochs_all.drop_log)
-            logger.error('tmin = %.1f, tmax = %.1f, tmin_buffer = %.1f, tmax_buffer = %.1f, raw length = %.1f' % \
-                (tmin, tmax, tmin_buffer, tmax_buffer, raw._data.shape[1] / sfreq))
-            logger.error('\nType exit to continue.\n')
-            pdb.set_trace()
-    except:
-        logger.critical('\n*** (tfr_export) Unknown error occurred while epoching ***')
-        logger.critical('tmin = %.1f, tmax = %.1f, tmin_buffer = %.1f, tmax_buffer = %.1f, raw length = %.1f' % \
-            (tmin, tmax, tmin_buffer, tmax_buffer, raw._data.shape[1] / sfreq))
-        pdb.set_trace()
-
-    power = {}
-    for evname in classes:
-        export_dir = outpath
-        qc.make_dirs(export_dir)
-        logger.info('>> Processing %s' % evname)
-        freqs = cfg.FREQ_RANGE  # define frequencies of interest
-        n_cycles = freqs / 2.  # different number of cycle per frequency
-        if cfg.POWER_AVERAGED:
-            # grand-average TFR
-            epochs = epochs_all[evname][:]
-            if len(epochs) == 0:
-                logger.WARNING('No %s epochs. Skipping.' % evname)
-                continue
-
-            if tfr_type == 'butter':
-                b, a = butter_bandpass(cfg.FREQ_RANGE[0], cfg.FREQ_RANGE[-1], sfreq, order=butter_order)
-                tfr_filtered = lfilter(b, a, epochs, axis=2)
-                tfr_hilbert = hilbert(tfr_filtered)
-                tfr_power = abs(tfr_hilbert)
-                tfr_data = np.mean(tfr_power, axis=0)
-            elif tfr_type == 'fir':
-                raise NotImplementedError
-            else:
-                power[evname] = tfr(epochs, freqs=freqs, n_cycles=n_cycles, use_fft=False,
-                    return_itc=False, n_jobs=n_jobs)
-                power[evname] = power[evname].crop(tmin=tmin, tmax=tmax)
-                tfr_data = power[evname].data
-
-            if cfg.EXPORT_MATLAB is True:
-                # export all channels to MATLAB
-                mout = '%s/%s-%s-%s.mat' % (export_dir, file_prefix, cfg.SP_FILTER, evname)
-                scipy.io.savemat(mout, {'tfr':tfr_data, 'chs':epochs.ch_names,
-                    'events':events, 'sfreq':sfreq, 'tmin':tmin, 'tmax':tmax, 'epochs':cfg.EPOCH, 'freqs':cfg.FREQ_RANGE})
-                logger.info('Exported %s' % mout)
-            if cfg.EXPORT_PNG is True:
-                # Inspect power for each channel
-                for ch in np.arange(len(picks)):
-                    chname = raw.ch_names[picks[ch]]
-                    title = 'Peri-event %s - Channel %s' % (evname, chname)
-
-                    # mode= None | 'logratio' | 'ratio' | 'zscore' | 'mean' | 'percent'
-                    fig = power[evname].plot([ch], baseline=cfg.BS_TIMES, mode=cfg.BS_MODE, show=False,
-                        colorbar=True, title=title, vmin=cfg.VMIN, vmax=cfg.VMAX, dB=False)[0]
-                    fout = '%s/%s-%s-%s-%s.png' % (export_dir, file_prefix, cfg.SP_FILTER, evname, chname)
-                    fig.savefig(fout)
-                    plt.close()
-                    logger.info('Exported to %s' % fout)
-        else:
-            # TFR per event
-            for ep in range(len(epochs_all[evname])):
-                epochs = epochs_all[evname][ep]
-                if len(epochs) == 0:
-                    logger.WARNING('No %s epochs. Skipping.' % evname)
-                    continue
-                power[evname] = tfr(epochs, freqs=freqs, n_cycles=n_cycles, use_fft=False,
-                    return_itc=False, n_jobs=n_jobs)
-                power[evname] = power[evname].crop(tmin=tmin, tmax=tmax)
-                if cfg.EXPORT_MATLAB is True:
-                    # export all channels to MATLAB
-                    mout = '%s/%s-%s-%s-ep%02d.mat' % (export_dir, file_prefix, cfg.SP_FILTER, evname, ep + 1)
-                    scipy.io.savemat(mout, {'tfr':power[evname].data, 'chs':power[evname].ch_names,
-                        'events':events, 'sfreq':sfreq, 'tmin':tmin, 'tmax':tmax, 'epochs':cfg.EPOCH, 'freqs':cfg.FREQ_RANGE})
-                    logger.info('Exported %s' % mout)
-                if cfg.EXPORT_PNG is True:
-                    # Inspect power for each channel
-                    for ch in np.arange(len(picks)):
-                        chname = raw.ch_names[picks[ch]]
-                        title = 'Peri-event %s - Channel %s, Trial %d' % (evname, chname, ep + 1)
-                        # mode= None | 'logratio' | 'ratio' | 'zscore' | 'mean' | 'percent'
-                        fig = power[evname].plot([ch], baseline=cfg.BS_TIMES, mode=cfg.BS_MODE, show=False,
-                            colorbar=True, title=title, vmin=cfg.VMIN, vmax=cfg.VMAX, dB=False)[0]
-                        fout = '%s/%s-%s-%s-%s-ep%02d.png' % (export_dir, file_prefix, cfg.SP_FILTER, evname, chname, ep + 1)
-                        fig.savefig(fout)
-                        plt.close()
-                        logger.info('Exported %s' % fout)
-
-    if hasattr(cfg, 'POWER_DIFF'):
-        export_dir = '%s/diff' % outpath
-        qc.make_dirs(export_dir)
-        labels = classes.keys()
-        df = power[labels[0]] - power[labels[1]]
-        df.data = np.log(np.abs(df.data))
-        # Inspect power diff for each channel
-        for ch in np.arange(len(picks)):
-            chname = raw.ch_names[picks[ch]]
-            title = 'Peri-event %s-%s - Channel %s' % (labels[0], labels[1], chname)
-
-            # mode= None | 'logratio' | 'ratio' | 'zscore' | 'mean' | 'percent'
-            fig = df.plot([ch], baseline=cfg.BS_TIMES, mode=cfg.BS_MODE, show=False,
-                colorbar=True, title=title, vmin=3.0, vmax=-3.0, dB=False)[0] # this code needs testing
-            fout = '%s/%s-%s-diff-%s-%s-%s.jpg' % (export_dir, file_prefix, cfg.SP_FILTER, labels[0], labels[1], chname)
-            logger.info('Exporting to %s' % fout)
-            fig.savefig(fout)
-            plt.close()
-    logger.info('Finished !')
-
-def batch_run(cfg_module):
-    cfg = pu.load_config(cfg_module)
-    cfg = check_config(cfg)
-    get_tfr(cfg)
-
-def main():
-    """
-    Invoked from console
-    """
-    if len(sys.argv) == 1:
-        print('Usage: %s config_module' % os.path.basename(__file__))
-        return
-
-    cfg_module = sys.argv[1]
-    batch_run(cfg_module)
-
-if __name__ == '__main__':
-    main()
+from __future__ import print_function, division
+
+"""
+Time-frequency analysis using Morlet wavelets or multitapers
+
+Kyuhwa Lee
+EPFL, 2019
+
+"""
+
+import sys
+import os
+import mne
+import imp
+import pdb
+import scipy
+import traceback
+import numpy as np
+import multiprocessing as mp
+import mne.time_frequency
+import matplotlib.pyplot as plt
+import neurodecode.utils.pycnbi_utils as pu
+import neurodecode.utils.q_common as qc
+from neurodecode.triggers.trigger_def import trigger_def
+from neurodecode import logger
+from builtins import input
+from scipy.signal import lfilter
+from scipy.signal import butter
+from scipy.signal import hilbert
+
+def check_config(cfg):
+    if not hasattr(cfg, 'TFR_TYPE'):
+        cfg.TFR_TYPE = 'multitaper'
+    if not hasattr(cfg, 'N_JOBS'):
+        cfg.N_JOBS = None
+    if not hasattr(cfg, 'T_BUFFER'):
+        cfg.T_BUFFER = 1
+    if not hasattr(cfg, 'BS_MODE'):
+        cfg.BS_MODE = 'logratio'
+    if not hasattr(cfg, 'BS_TIMES'):
+        cfg.BS_TIMES = (None, 0)
+    if not hasattr(cfg, 'EXPORT_PNG'):
+        cfg.EXPORT_PNG = False
+    if not hasattr(cfg, 'EXPORT_MATLAB'):
+        cfg.MATLAB = False
+    if not hasattr(cfg, 'EXPORT_PATH'):
+        cfg.EXPORT_PATH = None
+    return cfg
+
+def butter_bandpass(lowcut, highcut, fs, order=5):
+    nyq = fs / 2.0
+    low = lowcut / nyq
+    high = highcut / nyq
+    b, a = butter(order, [low, high], btype='band')
+    return b, a
+
+def get_tfr(cfg, recursive=False, n_jobs=1):
+    '''
+    @params:
+    tfr_type: 'multitaper' or 'morlet'
+    recursive: if True, load raw files in sub-dirs recursively
+    export_path: path to save plots
+    n_jobs: number of cores to run in parallel
+    '''
+
+    cfg = check_config(cfg)
+    tfr_type = cfg.TFR_TYPE
+    export_path = cfg.EXPORT_PATH
+    t_buffer = cfg.T_BUFFER
+    if tfr_type == 'multitaper':
+        tfr = mne.time_frequency.tfr_multitaper
+    elif tfr_type == 'morlet':
+        tfr = mne.time_frequency.tfr_morlet
+    elif tfr_type == 'butter':
+        butter_order = 4 # TODO: parameterize
+        tfr = lfilter
+    elif tfr_type == 'fir':
+        raise NotImplementedError
+    else:
+        raise ValueError('Wrong TFR type %s' % tfr_type)
+    if cfg.DECIM_FACTOR is None:
+        decim = 1
+    else:
+        decim = int(cfg.DECIM_FACTOR)
+    n_jobs = cfg.N_JOBS
+    if n_jobs is None:
+        n_jobs = mp.cpu_count()
+
+    if hasattr(cfg, 'DATA_PATHS'):
+        if export_path is None:
+            raise ValueError('For multiple directories, cfg.EXPORT_PATH cannot be None')
+        else:
+            outpath = export_path
+        # custom event file
+        if hasattr(cfg, 'EVENT_FILE') and cfg.EVENT_FILE is not None:
+            events = mne.read_events(cfg.EVENT_FILE)
+        file_prefix = 'grandavg'
+
+        # load and merge files from all directories
+        flist = []
+        for ddir in cfg.DATA_PATHS:
+            ddir = ddir.replace('\\', '/')
+            if ddir[-1] != '/': ddir += '/'
+            for f in qc.get_file_list(ddir, fullpath=True, recursive=recursive):
+                if qc.parse_path(f).ext in ['fif', 'bdf', 'gdf']:
+                    flist.append(f)
+        raw, events = pu.load_multi(flist)
+    elif hasattr(cfg, 'DATA_FILE'):
+        logger.info('Loading %s' % cfg.DATA_FILE)
+        raw, events = pu.load_raw(cfg.DATA_FILE)
+
+        # custom events
+        if hasattr(cfg, 'EVENT_FILE') and cfg.EVENT_FILE is not None:
+            events = mne.read_events(cfg.EVENT_FILE)
+
+        if export_path is None:
+            [outpath, file_prefix, _] = qc.parse_path_list(cfg.DATA_FILE)
+        else:
+            file_prefix = qc.parse_path(cfg.DATA_FILE).name
+            outpath = export_path
+            file_prefix = qc.parse_path(cfg.DATA_FILE).name
+    else:
+        logger.error('Either DATA_PATHS or DATA_FILE is required in config file')
+        raise ValueError
+
+    # re-referencing
+    if cfg.REREFERENCE is not None:
+        pu.rereference(raw, cfg.REREFERENCE[1], cfg.REREFERENCE[0])
+        assert cfg.REREFERENCE[0] in raw.ch_names
+
+    sfreq = raw.info['sfreq']
+
+    # set channels of interest
+    picks = pu.channel_names_to_index(raw, cfg.CHANNEL_PICKS)
+
+    if max(picks) > len(raw.info['ch_names']):
+        msg = 'ERROR: "picks" has a channel index %d while there are only %d channels.' %\
+              (max(picks), len(raw.info['ch_names']))
+        raise RuntimeError(msg)
+
+    # Apply filters
+    raw = pu.preprocess(raw, spatial=cfg.SP_FILTER, spatial_ch=picks, spectral=cfg.TP_FILTER,
+                  spectral_ch=picks, notch=cfg.NOTCH_FILTER, notch_ch=picks,
+                  multiplier=cfg.MULTIPLIER, n_jobs=n_jobs, decim=decim)
+    sfreq /= decim
+    events[:,0] //= decim
+
+    # Read epochs
+    classes = {}
+    event_set = set(events[:, -1])
+    for t_name in cfg.TRIGGER_DEF:
+        if cfg.TRIGGER_FILE is not None:
+            tdef = trigger_def(cfg.TRIGGER_FILE)
+            t_value = tdef.by_name[t_name]
+            if t_value in event_set:
+                classes[t_name] = t_value
+        else:
+            classes[str(t_name)] = t_name
+    if len(classes) == 0:
+        raise ValueError('No desired event was found from the data.')
+
+    try:
+        tmin = cfg.EPOCH[0]
+        tmin_buffer = tmin - t_buffer
+        raw_tmax = raw._data.shape[1] / sfreq - 0.1
+        if cfg.EPOCH[1] is None:
+            if cfg.POWER_AVERAGED:
+                raise ValueError('EPOCH value cannot have None for grand averaged TFR')
+            else:
+                if len(cfg.TRIGGERS) > 1:
+                    raise ValueError('If the end time of EPOCH is None, only a single event can be defined.')
+                t_ref = events[np.where(events[:,2] == list(cfg.TRIGGERS)[0])[0][0], 0] / sfreq
+                tmax = raw_tmax - t_ref - t_buffer
+        else:
+            tmax = cfg.EPOCH[1]
+        tmax_buffer = tmax + t_buffer
+        if tmax_buffer > raw_tmax:
+            raise ValueError('Epoch length with buffer (%.3f) is larger than signal length (%.3f)' % (tmax_buffer, raw_tmax))
+        epochs_all = mne.Epochs(raw, events, classes, tmin=tmin_buffer, tmax=tmax_buffer,
+                                proj=False, picks=picks, baseline=None, preload=True)
+        if epochs_all.drop_log_stats() > 0:
+            logger.error('\n** Bad epochs found. Dropping into a Python shell.')
+            logger.error(epochs_all.drop_log)
+            logger.error('tmin = %.1f, tmax = %.1f, tmin_buffer = %.1f, tmax_buffer = %.1f, raw length = %.1f' % \
+                (tmin, tmax, tmin_buffer, tmax_buffer, raw._data.shape[1] / sfreq))
+            logger.error('\nType exit to continue.\n')
+            pdb.set_trace()
+    except:
+        logger.critical('\n*** (tfr_export) Unknown error occurred while epoching ***')
+        logger.critical('tmin = %.1f, tmax = %.1f, tmin_buffer = %.1f, tmax_buffer = %.1f, raw length = %.1f' % \
+            (tmin, tmax, tmin_buffer, tmax_buffer, raw._data.shape[1] / sfreq))
+        pdb.set_trace()
+
+    power = {}
+    for evname in classes:
+        export_dir = outpath
+        qc.make_dirs(export_dir)
+        logger.info('>> Processing %s' % evname)
+        freqs = cfg.FREQ_RANGE  # define frequencies of interest
+        n_cycles = freqs / 2.  # different number of cycle per frequency
+        if cfg.POWER_AVERAGED:
+            # grand-average TFR
+            epochs = epochs_all[evname][:]
+            if len(epochs) == 0:
+                logger.WARNING('No %s epochs. Skipping.' % evname)
+                continue
+
+            if tfr_type == 'butter':
+                b, a = butter_bandpass(cfg.FREQ_RANGE[0], cfg.FREQ_RANGE[-1], sfreq, order=butter_order)
+                tfr_filtered = lfilter(b, a, epochs, axis=2)
+                tfr_hilbert = hilbert(tfr_filtered)
+                tfr_power = abs(tfr_hilbert)
+                tfr_data = np.mean(tfr_power, axis=0)
+            elif tfr_type == 'fir':
+                raise NotImplementedError
+            else:
+                power[evname] = tfr(epochs, freqs=freqs, n_cycles=n_cycles, use_fft=False,
+                    return_itc=False, n_jobs=n_jobs)
+                power[evname] = power[evname].crop(tmin=tmin, tmax=tmax)
+                tfr_data = power[evname].data
+
+            if cfg.EXPORT_MATLAB is True:
+                # export all channels to MATLAB
+                mout = '%s/%s-%s-%s.mat' % (export_dir, file_prefix, cfg.SP_FILTER, evname)
+                scipy.io.savemat(mout, {'tfr':tfr_data, 'chs':epochs.ch_names,
+                    'events':events, 'sfreq':sfreq, 'tmin':tmin, 'tmax':tmax, 'epochs':cfg.EPOCH, 'freqs':cfg.FREQ_RANGE})
+                logger.info('Exported %s' % mout)
+            if cfg.EXPORT_PNG is True:
+                # Inspect power for each channel
+                for ch in np.arange(len(picks)):
+                    chname = raw.ch_names[picks[ch]]
+                    title = 'Peri-event %s - Channel %s' % (evname, chname)
+
+                    # mode= None | 'logratio' | 'ratio' | 'zscore' | 'mean' | 'percent'
+                    fig = power[evname].plot([ch], baseline=cfg.BS_TIMES, mode=cfg.BS_MODE, show=False,
+                        colorbar=True, title=title, vmin=cfg.VMIN, vmax=cfg.VMAX, dB=False)[0]
+                    fout = '%s/%s-%s-%s-%s.png' % (export_dir, file_prefix, cfg.SP_FILTER, evname, chname)
+                    fig.savefig(fout)
+                    plt.close()
+                    logger.info('Exported to %s' % fout)
+        else:
+            # TFR per event
+            for ep in range(len(epochs_all[evname])):
+                epochs = epochs_all[evname][ep]
+                if len(epochs) == 0:
+                    logger.WARNING('No %s epochs. Skipping.' % evname)
+                    continue
+                power[evname] = tfr(epochs, freqs=freqs, n_cycles=n_cycles, use_fft=False,
+                    return_itc=False, n_jobs=n_jobs)
+                power[evname] = power[evname].crop(tmin=tmin, tmax=tmax)
+                if cfg.EXPORT_MATLAB is True:
+                    # export all channels to MATLAB
+                    mout = '%s/%s-%s-%s-ep%02d.mat' % (export_dir, file_prefix, cfg.SP_FILTER, evname, ep + 1)
+                    scipy.io.savemat(mout, {'tfr':power[evname].data, 'chs':power[evname].ch_names,
+                        'events':events, 'sfreq':sfreq, 'tmin':tmin, 'tmax':tmax, 'epochs':cfg.EPOCH, 'freqs':cfg.FREQ_RANGE})
+                    logger.info('Exported %s' % mout)
+                if cfg.EXPORT_PNG is True:
+                    # Inspect power for each channel
+                    for ch in np.arange(len(picks)):
+                        chname = raw.ch_names[picks[ch]]
+                        title = 'Peri-event %s - Channel %s, Trial %d' % (evname, chname, ep + 1)
+                        # mode= None | 'logratio' | 'ratio' | 'zscore' | 'mean' | 'percent'
+                        fig = power[evname].plot([ch], baseline=cfg.BS_TIMES, mode=cfg.BS_MODE, show=False,
+                            colorbar=True, title=title, vmin=cfg.VMIN, vmax=cfg.VMAX, dB=False)[0]
+                        fout = '%s/%s-%s-%s-%s-ep%02d.png' % (export_dir, file_prefix, cfg.SP_FILTER, evname, chname, ep + 1)
+                        fig.savefig(fout)
+                        plt.close()
+                        logger.info('Exported %s' % fout)
+
+    if hasattr(cfg, 'POWER_DIFF'):
+        export_dir = '%s/diff' % outpath
+        qc.make_dirs(export_dir)
+        labels = classes.keys()
+        df = power[labels[0]] - power[labels[1]]
+        df.data = np.log(np.abs(df.data))
+        # Inspect power diff for each channel
+        for ch in np.arange(len(picks)):
+            chname = raw.ch_names[picks[ch]]
+            title = 'Peri-event %s-%s - Channel %s' % (labels[0], labels[1], chname)
+
+            # mode= None | 'logratio' | 'ratio' | 'zscore' | 'mean' | 'percent'
+            fig = df.plot([ch], baseline=cfg.BS_TIMES, mode=cfg.BS_MODE, show=False,
+                colorbar=True, title=title, vmin=3.0, vmax=-3.0, dB=False)[0] # this code needs testing
+            fout = '%s/%s-%s-diff-%s-%s-%s.jpg' % (export_dir, file_prefix, cfg.SP_FILTER, labels[0], labels[1], chname)
+            logger.info('Exporting to %s' % fout)
+            fig.savefig(fout)
+            plt.close()
+    logger.info('Finished !')
+
+def batch_run(cfg_module):
+    cfg = pu.load_config(cfg_module)
+    cfg = check_config(cfg)
+    get_tfr(cfg)
+
+def main():
+    """
+    Invoked from console
+    """
+    if len(sys.argv) == 1:
+        print('Usage: %s config_module' % os.path.basename(__file__))
+        return
+
+    cfg_module = sys.argv[1]
+    batch_run(cfg_module)
+
+if __name__ == '__main__':
+    main()
```

### Comparing `neurodecode-2.0.4/neurodecode/analysis/tfr_export_each_file.py` & `neurodecode-2.0.5/neurodecode/analysis/tfr_export_each_file.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-from __future__ import print_function, division
-
-"""
-Time-frequency analysis using Morlet wavelets or multitapers
-TFRs are computed on each the whole fif file, from the beginning until the end.
-
-Kyuhwa Lee, 2018
-
-"""
-
-import sys
-import os
-import imp
-import mne
-import scipy
-import numpy as np
-import mne.time_frequency
-import multiprocessing as mp
-import neurodecode.utils.pycnbi_utils as pu
-import neurodecode.utils.q_common as qc
-from neurodecode import logger
-from builtins import input
-
-def check_cfg(cfg):
-    if not hasattr(cfg, 'N_JOBS'):
-        cfg.N_JOBS = None
-    if not hasattr(cfg, 'T_BUFFER'):
-        cfg.T_BUFFER = 1
-    if not hasattr(cfg, 'BS_MODE'):
-        cfg.BS_MODE = 'logratio'
-    if not hasattr(cfg, 'BS_TIMES'):
-        cfg.BS_TIMES = (None, 0)
-    if not hasattr(cfg, 'EXPORT_PNG'):
-        cfg.EXPORT_PNG = False
-    if not hasattr(cfg, 'EXPORT_MATLAB'):
-        cfg.MATLAB = False
-    if not hasattr(cfg, 'EVENT_START'):
-        cfg.EVENT_START = None
-    return cfg
-
-def get_tfr_each_file(cfg, tfr_type='multitaper', recursive=False, export_path=None, n_jobs=1):
-    '''
-    @params:
-    tfr_type: 'multitaper' or 'morlet'
-    recursive: if True, load raw files in sub-dirs recursively
-    export_path: path to save plots
-    n_jobs: number of cores to run in parallel
-    '''
-
-    cfg = check_cfg(cfg)
-    if cfg.N_JOBS is None:
-        n_jobs = mp.cpu_count()
-    else:
-        n_jobs = cfg.N_JOBS
-
-    t_buffer = cfg.T_BUFFER
-    if tfr_type == 'multitaper':
-        tfr = mne.time_frequency.tfr_multitaper
-    elif tfr_type == 'morlet':
-        tfr = mne.time_frequency.tfr_morlet
-    else:
-        raise ValueError('Wrong TFR type %s' % tfr_type)
-
-    for fifdir in cfg.DATA_PATHS:
-        for f in qc.get_file_list(fifdir, fullpath=True, recursive=recursive):
-            [fdir, fname, fext] = qc.parse_path_list(f)
-            if fext in ['fif', 'bdf', 'gdf']:
-                get_tfr(f, cfg, tfr, n_jobs)
-
-def get_tfr(fif_file, cfg, tfr, n_jobs=1):
-    raw, events = pu.load_raw(fif_file)
-    p = qc.parse_path(fif_file)
-    fname = p.name
-    outpath = p.dir
-
-    export_dir = '%s/plot_%s' % (outpath, fname)
-    qc.make_dirs(export_dir)
-
-    # set channels of interest
-    picks = pu.channel_names_to_index(raw, cfg.CHANNEL_PICKS)
-
-    if max(picks) > len(raw.info['ch_names']):
-        msg = 'ERROR: "picks" has a channel index %d while there are only %d channels.' %\
-              (max(picks), len(raw.info['ch_names']))
-        raise RuntimeError(msg)
-
-    # Apply filters
-    raw = pu.preprocess(raw, spatial=cfg.SP_FILTER, spatial_ch=picks, spectral=cfg.TP_FILTER,
-                  spectral_ch=picks, notch=cfg.NOTCH_FILTER, notch_ch=picks,
-                  multiplier=cfg.MULTIPLIER, n_jobs=n_jobs)
-
-    # MNE TFR functions do not support Raw instances yet, so convert to Epoch
-    if cfg.EVENT_START is None:
-        raw._data[0][0] = 1
-        events = np.array([[0, 0, 1]])
-        classes = None
-    else:
-        classes = {'START':cfg.EVENT_START}
-    tmax = (raw._data.shape[1] - 1) / raw.info['sfreq']
-    epochs_all = mne.Epochs(raw, events, classes, tmin=0, tmax=tmax,
-                    picks=picks, baseline=None, preload=True)
-    logger.info('\n>> Processing %s' % fif_file)
-    freqs = cfg.FREQ_RANGE  # define frequencies of interest
-    n_cycles = freqs / 2.  # different number of cycle per frequency
-    power = tfr(epochs_all, freqs=freqs, n_cycles=n_cycles, use_fft=False,
-        return_itc=False, decim=1, n_jobs=n_jobs)
-
-    if cfg.EXPORT_MATLAB is True:
-        # export all channels to MATLAB
-        mout = '%s/%s-%s.mat' % (export_dir, fname, cfg.SP_FILTER)
-        scipy.io.savemat(mout, {'tfr':power.data, 'chs':power.ch_names, 'events':events,
-            'sfreq':raw.info['sfreq'], 'freqs':cfg.FREQ_RANGE})
-
-    if cfg.EXPORT_PNG is True:
-        # Plot power of each channel
-        for ch in np.arange(len(picks)):
-            ch_name = raw.ch_names[picks[ch]]
-            title = 'Channel %s' % (ch_name)
-            # mode= None | 'logratio' | 'ratio' | 'zscore' | 'mean' | 'percent'
-            fig = power.plot([ch], baseline=cfg.BS_TIMES, mode=cfg.BS_MODE, show=False,
-                colorbar=True, title=title, vmin=cfg.VMIN, vmax=cfg.VMAX, dB=False)[0]
-            fout = '%s/%s-%s-%s.png' % (export_dir, fname, cfg.SP_FILTER, ch_name)
-            fig.savefig(fout)
-            logger.info('Exported %s' % fout)
-
-    logger.info('Finished !')
-
-def config_run(cfg_module):
-    cfg = pu.load_config(cfg_module)
-
-    if not hasattr(cfg, 'TFR_TYPE'):
-        cfg.TFR_TYPE = 'multitaper'
-    get_tfr_each_file(cfg, tfr_type=cfg.TFR_TYPE)
-
-def main():
-    """
-    Invoked from console
-    """
-    if len(sys.argv) == 1:
-        print('Usage: %s config_module' % os.path.basename(__file__))
-        return
-
-    cfg_module = sys.argv[1]
-    config_run(cfg_module)
-
-if __name__ == '__main__':
-    main()
+from __future__ import print_function, division
+
+"""
+Time-frequency analysis using Morlet wavelets or multitapers
+TFRs are computed on each the whole fif file, from the beginning until the end.
+
+Kyuhwa Lee, 2018
+
+"""
+
+import sys
+import os
+import imp
+import mne
+import scipy
+import numpy as np
+import mne.time_frequency
+import multiprocessing as mp
+import neurodecode.utils.pycnbi_utils as pu
+import neurodecode.utils.q_common as qc
+from neurodecode import logger
+from builtins import input
+
+def check_cfg(cfg):
+    if not hasattr(cfg, 'N_JOBS'):
+        cfg.N_JOBS = None
+    if not hasattr(cfg, 'T_BUFFER'):
+        cfg.T_BUFFER = 1
+    if not hasattr(cfg, 'BS_MODE'):
+        cfg.BS_MODE = 'logratio'
+    if not hasattr(cfg, 'BS_TIMES'):
+        cfg.BS_TIMES = (None, 0)
+    if not hasattr(cfg, 'EXPORT_PNG'):
+        cfg.EXPORT_PNG = False
+    if not hasattr(cfg, 'EXPORT_MATLAB'):
+        cfg.MATLAB = False
+    if not hasattr(cfg, 'EVENT_START'):
+        cfg.EVENT_START = None
+    return cfg
+
+def get_tfr_each_file(cfg, tfr_type='multitaper', recursive=False, export_path=None, n_jobs=1):
+    '''
+    @params:
+    tfr_type: 'multitaper' or 'morlet'
+    recursive: if True, load raw files in sub-dirs recursively
+    export_path: path to save plots
+    n_jobs: number of cores to run in parallel
+    '''
+
+    cfg = check_cfg(cfg)
+    if cfg.N_JOBS is None:
+        n_jobs = mp.cpu_count()
+    else:
+        n_jobs = cfg.N_JOBS
+
+    t_buffer = cfg.T_BUFFER
+    if tfr_type == 'multitaper':
+        tfr = mne.time_frequency.tfr_multitaper
+    elif tfr_type == 'morlet':
+        tfr = mne.time_frequency.tfr_morlet
+    else:
+        raise ValueError('Wrong TFR type %s' % tfr_type)
+
+    for fifdir in cfg.DATA_PATHS:
+        for f in qc.get_file_list(fifdir, fullpath=True, recursive=recursive):
+            [fdir, fname, fext] = qc.parse_path_list(f)
+            if fext in ['fif', 'bdf', 'gdf']:
+                get_tfr(f, cfg, tfr, n_jobs)
+
+def get_tfr(fif_file, cfg, tfr, n_jobs=1):
+    raw, events = pu.load_raw(fif_file)
+    p = qc.parse_path(fif_file)
+    fname = p.name
+    outpath = p.dir
+
+    export_dir = '%s/plot_%s' % (outpath, fname)
+    qc.make_dirs(export_dir)
+
+    # set channels of interest
+    picks = pu.channel_names_to_index(raw, cfg.CHANNEL_PICKS)
+
+    if max(picks) > len(raw.info['ch_names']):
+        msg = 'ERROR: "picks" has a channel index %d while there are only %d channels.' %\
+              (max(picks), len(raw.info['ch_names']))
+        raise RuntimeError(msg)
+
+    # Apply filters
+    raw = pu.preprocess(raw, spatial=cfg.SP_FILTER, spatial_ch=picks, spectral=cfg.TP_FILTER,
+                  spectral_ch=picks, notch=cfg.NOTCH_FILTER, notch_ch=picks,
+                  multiplier=cfg.MULTIPLIER, n_jobs=n_jobs)
+
+    # MNE TFR functions do not support Raw instances yet, so convert to Epoch
+    if cfg.EVENT_START is None:
+        raw._data[0][0] = 1
+        events = np.array([[0, 0, 1]])
+        classes = None
+    else:
+        classes = {'START':cfg.EVENT_START}
+    tmax = (raw._data.shape[1] - 1) / raw.info['sfreq']
+    epochs_all = mne.Epochs(raw, events, classes, tmin=0, tmax=tmax,
+                    picks=picks, baseline=None, preload=True)
+    logger.info('\n>> Processing %s' % fif_file)
+    freqs = cfg.FREQ_RANGE  # define frequencies of interest
+    n_cycles = freqs / 2.  # different number of cycle per frequency
+    power = tfr(epochs_all, freqs=freqs, n_cycles=n_cycles, use_fft=False,
+        return_itc=False, decim=1, n_jobs=n_jobs)
+
+    if cfg.EXPORT_MATLAB is True:
+        # export all channels to MATLAB
+        mout = '%s/%s-%s.mat' % (export_dir, fname, cfg.SP_FILTER)
+        scipy.io.savemat(mout, {'tfr':power.data, 'chs':power.ch_names, 'events':events,
+            'sfreq':raw.info['sfreq'], 'freqs':cfg.FREQ_RANGE})
+
+    if cfg.EXPORT_PNG is True:
+        # Plot power of each channel
+        for ch in np.arange(len(picks)):
+            ch_name = raw.ch_names[picks[ch]]
+            title = 'Channel %s' % (ch_name)
+            # mode= None | 'logratio' | 'ratio' | 'zscore' | 'mean' | 'percent'
+            fig = power.plot([ch], baseline=cfg.BS_TIMES, mode=cfg.BS_MODE, show=False,
+                colorbar=True, title=title, vmin=cfg.VMIN, vmax=cfg.VMAX, dB=False)[0]
+            fout = '%s/%s-%s-%s.png' % (export_dir, fname, cfg.SP_FILTER, ch_name)
+            fig.savefig(fout)
+            logger.info('Exported %s' % fout)
+
+    logger.info('Finished !')
+
+def config_run(cfg_module):
+    cfg = pu.load_config(cfg_module)
+
+    if not hasattr(cfg, 'TFR_TYPE'):
+        cfg.TFR_TYPE = 'multitaper'
+    get_tfr_each_file(cfg, tfr_type=cfg.TFR_TYPE)
+
+def main():
+    """
+    Invoked from console
+    """
+    if len(sys.argv) == 1:
+        print('Usage: %s config_module' % os.path.basename(__file__))
+        return
+
+    cfg_module = sys.argv[1]
+    config_run(cfg_module)
+
+if __name__ == '__main__':
+    main()
```

### Comparing `neurodecode-2.0.4/neurodecode/colorer.py` & `neurodecode-2.0.5/neurodecode/colorer.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-'''
-Colorize logger messages depending on the log level.
-Usage: just import this module.
-
-This code was stolen and modified from:
-https://stackoverflow.com/questions/384076/how-can-i-color-python-logging-output
-'''
-
-#!/usr/bin/env python
-# encoding: utf-8
-import logging
-# now we patch Python code to add color support to logging.StreamHandler
-def add_coloring_to_emit_windows(fn):
-        # add methods we need to the class
-    def _out_handle(self):
-        import ctypes
-        return ctypes.windll.kernel32.GetStdHandle(self.STD_OUTPUT_HANDLE)
-    out_handle = property(_out_handle)
-
-    def _set_color(self, code):
-        import ctypes
-        # Constants from the Windows API
-        self.STD_OUTPUT_HANDLE = -11
-        hdl = ctypes.windll.kernel32.GetStdHandle(self.STD_OUTPUT_HANDLE)
-        ctypes.windll.kernel32.SetConsoleTextAttribute(hdl, code)
-
-    setattr(logging.StreamHandler, '_set_color', _set_color)
-
-    def new(*args):
-        FOREGROUND_BLUE      = 0x0001 # text color contains blue.
-        FOREGROUND_GREEN     = 0x0002 # text color contains green.
-        FOREGROUND_RED       = 0x0004 # text color contains red.
-        FOREGROUND_INTENSITY = 0x0008 # text color is intensified.
-        FOREGROUND_WHITE     = FOREGROUND_BLUE|FOREGROUND_GREEN |FOREGROUND_RED
-    # winbase.h
-        STD_INPUT_HANDLE = -10
-        STD_OUTPUT_HANDLE = -11
-        STD_ERROR_HANDLE = -12
-
-        # wincon.h
-        FOREGROUND_BLACK     = 0x0000
-        FOREGROUND_BLUE      = 0x0001
-        FOREGROUND_GREEN     = 0x0002
-        FOREGROUND_CYAN      = 0x0003
-        FOREGROUND_RED       = 0x0004
-        FOREGROUND_MAGENTA   = 0x0005
-        FOREGROUND_YELLOW    = 0x0006
-        FOREGROUND_GREY      = 0x0007
-        FOREGROUND_INTENSITY = 0x0008 # foreground color is intensified.
-
-        BACKGROUND_BLACK     = 0x0000
-        BACKGROUND_BLUE      = 0x0010
-        BACKGROUND_GREEN     = 0x0020
-        BACKGROUND_CYAN      = 0x0030
-        BACKGROUND_RED       = 0x0040
-        BACKGROUND_MAGENTA   = 0x0050
-        BACKGROUND_YELLOW    = 0x0060
-        BACKGROUND_GREY      = 0x0070
-        BACKGROUND_INTENSITY = 0x0080 # background color is intensified.
-
-        levelno = args[1].levelno
-        if(levelno>=50):
-            color = BACKGROUND_YELLOW | FOREGROUND_RED | FOREGROUND_INTENSITY | BACKGROUND_INTENSITY
-        elif(levelno>=40):
-            color = FOREGROUND_RED | FOREGROUND_INTENSITY
-        elif(levelno>=30):
-            color = FOREGROUND_YELLOW | FOREGROUND_INTENSITY
-        elif(levelno==26):
-            color = FOREGROUND_YELLOW | FOREGROUND_INTENSITY
-        elif(levelno==24):
-            color = FOREGROUND_BLUE | FOREGROUND_INTENSITY
-        elif(levelno==22):
-            color = FOREGROUND_GREEN | FOREGROUND_INTENSITY
-        elif(levelno>=20):
-            color = FOREGROUND_WHITE | FOREGROUND_INTENSITY
-        elif(levelno>=10):
-            color = FOREGROUND_GREEN | FOREGROUND_INTENSITY
-        else:
-            color =  FOREGROUND_WHITE
-        args[0]._set_color(color)
-
-        ret = fn(*args)
-        # reset to normal text color
-        args[0]._set_color( FOREGROUND_WHITE )
-        return ret
-    return new
-
-def add_coloring_to_emit_ansi(fn):
-    # add methods we need to the class
-    def new(*args):
-        levelno = args[1].levelno
-        if(levelno>=50):
-            color = '\x1b[31m' # red
-        elif(levelno>=40):
-            color = '\x1b[31m' # red
-        elif(levelno>=30):
-            color = '\x1b[33m' # yellow
-        elif(levelno>=20):
-            color = '\x1b[32m' # green
-        elif(levelno>=10):
-            color = '\x1b[35m' # pink
-        else:
-            color = '\x1b[0m' # normal
-        args[1].msg = color + args[1].msg +  '\x1b[0m'  # normal
-        #print "after"
-        return fn(*args)
-    return new
-
-import platform
-if platform.system()=='Windows':
-    # Windows does not support ANSI escapes and we are using API calls to set the console color
-    logging.StreamHandler.emit = add_coloring_to_emit_windows(logging.StreamHandler.emit)
-else:
-    # all non-Windows platforms are supporting ANSI escapes so we use them
-    logging.StreamHandler.emit = add_coloring_to_emit_ansi(logging.StreamHandler.emit)
-    #log = logging.getLogger()
-    #log.addFilter(log_filter())
-    #//hdlr = logging.StreamHandler()
-    #//hdlr.setFormatter(formatter())
+'''
+Colorize logger messages depending on the log level.
+Usage: just import this module.
+
+This code was stolen and modified from:
+https://stackoverflow.com/questions/384076/how-can-i-color-python-logging-output
+'''
+
+#!/usr/bin/env python
+# encoding: utf-8
+import logging
+# now we patch Python code to add color support to logging.StreamHandler
+def add_coloring_to_emit_windows(fn):
+        # add methods we need to the class
+    def _out_handle(self):
+        import ctypes
+        return ctypes.windll.kernel32.GetStdHandle(self.STD_OUTPUT_HANDLE)
+    out_handle = property(_out_handle)
+
+    def _set_color(self, code):
+        import ctypes
+        # Constants from the Windows API
+        self.STD_OUTPUT_HANDLE = -11
+        hdl = ctypes.windll.kernel32.GetStdHandle(self.STD_OUTPUT_HANDLE)
+        ctypes.windll.kernel32.SetConsoleTextAttribute(hdl, code)
+
+    setattr(logging.StreamHandler, '_set_color', _set_color)
+
+    def new(*args):
+        FOREGROUND_BLUE      = 0x0001 # text color contains blue.
+        FOREGROUND_GREEN     = 0x0002 # text color contains green.
+        FOREGROUND_RED       = 0x0004 # text color contains red.
+        FOREGROUND_INTENSITY = 0x0008 # text color is intensified.
+        FOREGROUND_WHITE     = FOREGROUND_BLUE|FOREGROUND_GREEN |FOREGROUND_RED
+    # winbase.h
+        STD_INPUT_HANDLE = -10
+        STD_OUTPUT_HANDLE = -11
+        STD_ERROR_HANDLE = -12
+
+        # wincon.h
+        FOREGROUND_BLACK     = 0x0000
+        FOREGROUND_BLUE      = 0x0001
+        FOREGROUND_GREEN     = 0x0002
+        FOREGROUND_CYAN      = 0x0003
+        FOREGROUND_RED       = 0x0004
+        FOREGROUND_MAGENTA   = 0x0005
+        FOREGROUND_YELLOW    = 0x0006
+        FOREGROUND_GREY      = 0x0007
+        FOREGROUND_INTENSITY = 0x0008 # foreground color is intensified.
+
+        BACKGROUND_BLACK     = 0x0000
+        BACKGROUND_BLUE      = 0x0010
+        BACKGROUND_GREEN     = 0x0020
+        BACKGROUND_CYAN      = 0x0030
+        BACKGROUND_RED       = 0x0040
+        BACKGROUND_MAGENTA   = 0x0050
+        BACKGROUND_YELLOW    = 0x0060
+        BACKGROUND_GREY      = 0x0070
+        BACKGROUND_INTENSITY = 0x0080 # background color is intensified.
+
+        levelno = args[1].levelno
+        if(levelno>=50):
+            color = BACKGROUND_YELLOW | FOREGROUND_RED | FOREGROUND_INTENSITY | BACKGROUND_INTENSITY
+        elif(levelno>=40):
+            color = FOREGROUND_RED | FOREGROUND_INTENSITY
+        elif(levelno>=30):
+            color = FOREGROUND_YELLOW | FOREGROUND_INTENSITY
+        elif(levelno==26):
+            color = FOREGROUND_YELLOW | FOREGROUND_INTENSITY
+        elif(levelno==24):
+            color = FOREGROUND_BLUE | FOREGROUND_INTENSITY
+        elif(levelno==22):
+            color = FOREGROUND_GREEN | FOREGROUND_INTENSITY
+        elif(levelno>=20):
+            color = FOREGROUND_WHITE | FOREGROUND_INTENSITY
+        elif(levelno>=10):
+            color = FOREGROUND_GREEN | FOREGROUND_INTENSITY
+        else:
+            color =  FOREGROUND_WHITE
+        args[0]._set_color(color)
+
+        ret = fn(*args)
+        # reset to normal text color
+        args[0]._set_color( FOREGROUND_WHITE )
+        return ret
+    return new
+
+def add_coloring_to_emit_ansi(fn):
+    # add methods we need to the class
+    def new(*args):
+        levelno = args[1].levelno
+        if(levelno>=50):
+            color = '\x1b[31m' # red
+        elif(levelno>=40):
+            color = '\x1b[31m' # red
+        elif(levelno>=30):
+            color = '\x1b[33m' # yellow
+        elif(levelno>=20):
+            color = '\x1b[32m' # green
+        elif(levelno>=10):
+            color = '\x1b[35m' # pink
+        else:
+            color = '\x1b[0m' # normal
+        args[1].msg = color + args[1].msg +  '\x1b[0m'  # normal
+        #print "after"
+        return fn(*args)
+    return new
+
+import platform
+if platform.system()=='Windows':
+    # Windows does not support ANSI escapes and we are using API calls to set the console color
+    logging.StreamHandler.emit = add_coloring_to_emit_windows(logging.StreamHandler.emit)
+else:
+    # all non-Windows platforms are supporting ANSI escapes so we use them
+    logging.StreamHandler.emit = add_coloring_to_emit_ansi(logging.StreamHandler.emit)
+    #log = logging.getLogger()
+    #log.addFilter(log_filter())
+    #//hdlr = logging.StreamHandler()
+    #//hdlr.setFormatter(formatter())
```

### Comparing `neurodecode-2.0.4/neurodecode/decoder/features.py` & `neurodecode-2.0.5/neurodecode/decoder/features.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,532 +1,532 @@
-from __future__ import print_function, division
-
-"""
-features.py
-
-Feature computation module.
-
-
-Kyuhwa Lee, 2019
-Swiss Federal Institute of Technology Lausanne (EPFL)
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""
-
-import os
-import mne
-import mne.io
-import numpy as np
-import multiprocessing as mp
-import neurodecode.utils.q_common as qc
-import neurodecode.utils.pycnbi_utils as pu
-from mne import Epochs, pick_types
-from neurodecode import logger
-
-
-def slice_win(epochs_data, w_starts, w_length, psde, picks=None, title=None, flatten=True, preprocess=None, verbose=False):
-    '''
-    Compute PSD values of a sliding window
-
-    Params
-        epochs_data ([channels]x[samples]): raw epoch data
-        w_starts (list): starting indices of sample segments
-        w_length (int): window length in number of samples
-        psde: MNE PSDEstimator object
-        picks (list): subset of channels within epochs_data
-        title (string): print out the title associated with PID
-        flatten (boolean): generate concatenated feature vectors
-            If True: X = [windows] x [channels x freqs]
-            If False: X = [windows] x [channels] x [freqs]
-        preprocess (dict): None or parameters for pycnbi_utils.preprocess() with the following keys:
-            sfreq, spatial, spatial_ch, spectral, spectral_ch, notch, notch_ch,
-            multiplier, ch_names, rereference, decim, n_jobs
-    Returns:
-        [windows] x [channels*freqs] or [windows] x [channels] x [freqs]
-    '''
-
-    # raise error for wrong indexing
-    def WrongIndexError(Exception):
-        logger.error('%s' % Exception)
-
-    if type(w_length) is not int:
-        logger.warning('w_length type is %s. Converting to int.' % type(w_length))
-        w_length = int(w_length)
-    if title is None:
-        title = '[PID %d] Frames %d-%d' % (os.getpid(), w_starts[0], w_starts[-1]+w_length-1)
-    else:
-        title = '[PID %d] %s' % (os.getpid(), title)
-    if preprocess is not None and preprocess['decim'] != 1:
-        title += ' (decim factor %d)' % preprocess['decim']
-    logger.info(title)
-
-    X = None
-    for n in w_starts:
-        n = int(round(n))
-        if n >= epochs_data.shape[1]:
-            logger.error('w_starts has an out-of-bounds index %d for epoch length %d.' % (n, epochs_data.shape[1]))
-            raise WrongIndexError
-        window = epochs_data[:, n:(n + w_length)]
-
-        if preprocess is not None:
-            window = pu.preprocess(window,
-                sfreq=preprocess['sfreq'],
-                spatial=preprocess['spatial'],
-                spatial_ch=preprocess['spatial_ch'],
-                spectral=preprocess['spectral'],
-                spectral_ch=preprocess['spectral_ch'],
-                notch=preprocess['notch'],
-                notch_ch=preprocess['notch_ch'],
-                multiplier=preprocess['multiplier'],
-                ch_names=preprocess['ch_names'],
-                rereference=preprocess['rereference'],
-                decim=preprocess['decim'],
-                n_jobs=preprocess['n_jobs'])
-
-        # dimension: psde.transform( [epochs x channels x times] )
-        psd = psde.transform(window.reshape((1, window.shape[0], window.shape[1])))
-        psd = psd.reshape((psd.shape[0], psd.shape[1] * psd.shape[2]))
-        if picks:
-            psd = psd[0][picks]
-            psd = psd.reshape((1, len(psd)))
-
-        if X is None:
-            X = psd
-        else:
-            X = np.concatenate((X, psd), axis=0)
-
-        if verbose == True:
-            logger.info('[PID %d] processing frame %d / %d' % (os.getpid(), n, w_starts[-1]))
-
-    return X
-
-
-def get_psd(epochs, psde, wlen, wstep, picks=None, flatten=True, preprocess=None, decim=1, n_jobs=1):
-    """
-    Compute multi-taper PSDs over a sliding window
-
-    Input
-    =====
-    epochs: MNE Epochs object
-    psde: MNE PSDEstimator object
-    wlen: window length in frames
-    wstep: window step in frames
-    picks: channels to be used; use all if None
-    flatten: boolean, see Returns section
-    n_jobs: nubmer of cores to use, None = use all cores
-
-    Output
-    ======
-    if flatten==True:
-        X_data: [epochs] x [windows] x [channels*freqs]
-    else:
-        X_data: [epochs] x [windows] x [channels] x [freqs]
-    y_data: [epochs] x [windows]
-
-    TODO:
-        Accept input as numpy array as well, in addition to Epochs object
-    """
-
-    tm = qc.Timer()
-
-    if n_jobs is None:
-        n_jobs = mp.cpu_count()
-    if n_jobs > 1:
-        logger.info('Opening a pool of %d workers' % n_jobs)
-        pool = mp.Pool(n_jobs)
-
-    # compute PSD from sliding windows of each epoch
-    labels = epochs.events[:, -1]
-    epochs_data = epochs.get_data()
-    w_starts = np.arange(0, epochs_data.shape[2] - wlen, wstep)
-    X_data = None
-    y_data = None
-    results = []
-    for ep in np.arange(len(labels)):
-        title = 'Epoch %d / %d, Frames %d-%d' % (ep+1, len(labels), w_starts[0], w_starts[-1] + wlen - 1)
-        if n_jobs == 1:
-            # no multiprocessing
-            results.append(slice_win(epochs_data[ep], w_starts, wlen, psde, picks, title, True, preprocess))
-        else:
-            # parallel psd computation
-            results.append(pool.apply_async(slice_win, [epochs_data[ep], w_starts, wlen, psde, picks, title, True, preprocess]))
-
-    for ep in range(len(results)):
-        if n_jobs == 1:
-            r = results[ep]
-        else:
-            r = results[ep].get()  # windows x features
-        X = r.reshape((1, r.shape[0], r.shape[1]))  # 1 x windows x features
-        if X_data is None:
-            X_data = X
-        else:
-            X_data = np.concatenate((X_data, X), axis=0)
-
-        # speed comparison: http://stackoverflow.com/questions/5891410/numpy-array-initialization-fill-with-identical-values
-        y = np.empty((1, r.shape[0]))  # 1 x windows
-        y.fill(labels[ep])
-        if y_data is None:
-            y_data = y
-        else:
-            y_data = np.concatenate((y_data, y), axis=0)
-
-    # close pool
-    if n_jobs > 1:
-        pool.close()
-        pool.join()
-
-    logger.info('Feature computation took %d seconds.' % tm.sec())
-
-    if flatten:
-        return X_data, y_data.astype(np.int)
-    else:
-        xs = X_data.shape
-        nch = len(epochs.ch_names)
-        return X_data.reshape(xs[0], xs[1], nch, int(xs[2] / nch)), y_data.astype(np.int)
-
-
-def get_psd_feature(epochs_train, window, psdparam, picks=None, preprocess=None, n_jobs=1):
-    """
-    Wrapper for get_psd() adding meta information.
-
-    Input
-    =====
-    epochs_train: mne.Epochs object or list of mne.Epochs object.
-    window: [t_start, t_end]. Time window range for computing PSD.
-    psdparam: {fmin:float, fmax:float, wlen:float, wstep:int, decim:int}.
-              fmin, fmax in Hz, wlen in seconds, wstep in number of samples.
-    picks: Channels to compute features from.
-
-    Output
-    ======
-    dict object containing computed features.
-    """
-
-    if type(window[0]) is list:
-        sfreq = epochs_train[0].info['sfreq']
-        wlen = []
-        w_frames = []
-        # multiple PSD estimators, defined for each epoch
-        if type(psdparam) is list:
-            '''
-            TODO: implement multi-window PSD for each epoch
-            assert len(psdparam) == len(window)
-            for i, p in enumerate(psdparam):
-                if p['wlen'] is None:
-                    wl = window[i][1] - window[i][0]
-                else:
-                    wl = p['wlen']
-                wlen.append(wl)
-                w_frames.append(int(sfreq * wl))
-            '''
-            logger.error('Multiple psd function not implemented yet.')
-            raise NotImplementedError
-        # same PSD estimator for all epochs
-        else:
-            for i, e in enumerate(window):
-                if psdparam['wlen'] is None:
-                    wl = window[i][1] - window[i][0]
-                else:
-                    wl = psdparam['wlen']
-                assert wl > 0
-                wlen.append(wl)
-                w_frames.append(int(round(sfreq * wl)))
-    else:
-        sfreq = epochs_train.info['sfreq']
-        wlen = window[1] - window[0]
-        if psdparam['wlen'] is None:
-            psdparam['wlen'] = wlen
-        w_frames = int(round(sfreq * psdparam['wlen']))  # window length in number of samples(frames)
-    if 'decim' not in psdparam or psdparam['decim'] is None:
-        psdparam['decim'] = 1
-
-    psde_sfreq = sfreq / psdparam['decim']
-    psde = mne.decoding.PSDEstimator(sfreq=psde_sfreq, fmin=psdparam['fmin'], fmax=psdparam['fmax'],
-        bandwidth=None, adaptive=False, low_bias=True, n_jobs=1, normalization='length', verbose='WARNING')
-
-    logger.info_green('PSD computation')
-    if type(epochs_train) is list:
-        X_all = []
-        for i, ep in enumerate(epochs_train):
-            X, Y_data = get_psd(ep, psde, w_frames[i], psdparam['wstep'], picks, n_jobs=n_jobs, preprocess=preprocess, decim=psdparam['decim'])
-            X_all.append(X)
-        # concatenate along the feature dimension
-        # feature index order: window block x channel block x frequency block
-        # feature vector = [window1, window2, ...]
-        # where windowX = [channel1, channel2, ...]
-        # where channelX = [freq1, freq2, ...]
-        X_data = np.concatenate(X_all, axis=2)
-    else:
-        # feature index order: channel block x frequency block
-        # feature vector = [channel1, channel2, ...]
-        # where channelX = [freq1, freq2, ...]
-        X_data, Y_data = get_psd(epochs_train, psde, w_frames, psdparam['wstep'], picks, n_jobs=n_jobs, preprocess=preprocess, decim=psdparam['decim'])
-
-    # assign relative timestamps for each feature. time reference is the leading edge of a window.
-    w_starts = np.arange(0, epochs_train.get_data().shape[2] - w_frames, psdparam['wstep'])
-    t_features = w_starts / sfreq + psdparam['wlen'] + window[0]
-    return dict(X_data=X_data, Y_data=Y_data, wlen=wlen, w_frames=w_frames, psde=psde, times=t_features, decim=psdparam['decim'])
-
-
-def get_timelags(epochs, wlen, wstep, downsample=1, picks=None):
-    """
-    (DEPRECATED FUNCTION)
-    Get concatenated timelag features
-
-    TODO: Unit test.
-
-    Input
-    =====
-    epochs: input signals
-    wlen: window length (# time points) in downsampled data
-    wstep: window step in downsampled data
-    downsample: downsample signal to be 1/downsample length
-    picks: ignored for now
-
-    Output
-    ======
-    X: [epochs] x [windows] x [channels*freqs]
-    y: [epochs] x [labels]
-    """
-
-    '''
-    wlen = int(wlen)
-    wstep = int(wstep)
-    downsample = int(downsample)
-    X_data = None
-    y_data = None
-    labels = epochs.events[:, -1]  # every epoch must have event id
-    epochs_data = epochs.get_data()
-    n_channels = epochs_data.shape[1]
-    # trim to the nearest divisible length
-    epoch_ds_len = int(epochs_data.shape[2] / downsample)
-    epoch_len = downsample * epoch_ds_len
-    range_epochs = np.arange(epochs_data.shape[0])
-    range_channels = np.arange(epochs_data.shape[1])
-    range_windows = np.arange(epoch_ds_len - wlen, 0, -wstep)
-    X_data = np.zeros((len(range_epochs), len(range_windows), wlen * n_channels))
-
-    # for each epoch
-    for ep in range_epochs:
-        epoch = epochs_data[ep, :, :epoch_len]
-        ds = qc.average_every_n(epoch.reshape(-1), downsample)  # flatten to 1-D, then downsample
-        epoch_ds = ds.reshape(n_channels, -1)  # recover structure to channel x samples
-        # for each window over all channels
-        for i in range(len(range_windows)):
-            w = range_windows[i]
-            X = epoch_ds[:, w:w + wlen].reshape(1, -1)  # our feature vector
-            X_data[ep, i, :] = X
-
-        # fill labels
-        y = np.empty((1, len(range_windows)))  # 1 x windows
-        y.fill(labels[ep])
-        if y_data is None:
-            y_data = y
-        else:
-            y_data = np.concatenate((y_data, y), axis=0)
-
-    return X_data, y_data
-    '''
-    logger.error('This function is deprecated.')
-    raise NotImplementedError
-
-def feature2chz(x, fqlist, ch_names):
-    """
-    Label channel, frequency pair for PSD feature indices
-
-    Input
-    =====
-    x: feature index
-    fqlist: list of frequency bands
-    ch_names: list of complete channel names
-
-    Output
-    ======
-    (channel, frequency)
-
-    """
-
-    x = np.array(x).astype('int64').reshape(-1)
-    fqlist = np.array(fqlist).astype('float64')
-    ch_names = np.array(ch_names)
-
-    n_fq = len(fqlist)
-    hz = fqlist[x % n_fq]
-    ch = (x / n_fq).astype('int64')  # 0-based indexing
-
-    return ch_names[ch], hz
-
-
-def cva_features(datadir):
-    """
-    (DEPRECATED FUNCTION)
-    """
-    for fin in qc.get_file_list(datadir, fullpath=True):
-        if fin[-4:] != '.gdf': continue
-        fout = fin + '.cva'
-        if os.path.exists(fout):
-            logger.info('Skipping', fout)
-            continue
-        logger.info("cva_features('%s')" % fin)
-        qc.matlab("cva_features('%s')" % fin)
-
-
-def compute_features(cfg):
-    '''
-    Compute features using config specification.
-
-    Performs preprocessing, epcoching and feature computation.
-
-    Input
-    =====
-    Config file object
-
-    Output
-    ======
-    Feature data in dictionary
-    - X_data: feature vectors
-    - Y_data: feature labels
-    - wlen: window length in seconds
-    - w_frames: window length in frames
-    - psde: MNE PSD estimator object
-    - ch_names: selected channel names
-    - picks: original channel indices of the input fif
-    - sfreq: input sampling frequency
-    - sfreq_features: feature sampling frequency
-    - times: feature timestamp (leading edge of a window)
-    '''
-    # Preprocessing, epoching and PSD computation
-    ftrain = []
-    if hasattr(cfg, 'DATA_FILES'):
-        ftrain = cfg.DATA_FILES
-        logger.info('Using file list defined in cfg.DATA_FILES.')
-    else:
-        for f in qc.get_file_list(cfg.DATA_PATH, fullpath=True):
-            if f[-4:] in ['.fif', '.fiff']:
-                ftrain.append(f)
-        if len(ftrain) > 1 and cfg.PICKED_CHANNELS is not None and type(cfg.PICKED_CHANNELS[0]) == int:
-            logger.error('When loading multiple EEG files, PICKED_CHANNELS must be list of string, not integers because they may have different channel order.')
-            raise RuntimeError
-    raw, events = pu.load_multi(ftrain)
-
-    reref = cfg.REREFERENCE[cfg.REREFERENCE['selected']]
-    if reref is not None:
-        pu.rereference(raw, reref['New'], reref['Old'])
-
-    if cfg.LOAD_EVENTS[cfg.LOAD_EVENTS['selected']] is not None:
-        events = mne.read_events(cfg.LOAD_EVENTS[cfg.LOAD_EVENTS['selected']])
-
-    trigger_def_int = set()
-    for a in cfg.TRIGGER_DEF:
-        trigger_def_int.add(getattr(cfg.tdef, a))
-    triggers = {cfg.tdef.by_value[c]:c for c in trigger_def_int}
-
-    # Pick channels
-    if cfg.PICKED_CHANNELS is None or len(cfg.PICKED_CHANNELS) == 0:
-        picks = [int(x) for x in pick_types(raw.info, stim=False, eeg=True)]
-        chlist = [raw.ch_names[x] for x in picks]
-    else:
-        chlist = cfg.PICKED_CHANNELS
-        picks = []
-        for c in chlist:
-            if type(c) == int:
-                picks.append(c)
-            elif type(c) == str:
-                picks.append(raw.ch_names.index(c))
-            else:
-                logger.error('PICKED_CHANNELS has a value of unknown type %s.\nPICKED_CHANNELS=%s' % (type(c), cfg.PICKED_CHANNELS))
-                raise RuntimeError
-
-    if cfg.EXCLUDED_CHANNELS is not None and len(cfg.EXCLUDED_CHANNELS) > 0:
-        if len(set(cfg.EXCLUDED_CHANNELS) & set(cfg.PICKED_CHANNELS)) > 0:
-            logger.error('in config, EXCLUDED_CHANNELS and PICKED_CHANNELS must not contain the same channel')
-            raise ValueError
-        for c in cfg.EXCLUDED_CHANNELS:
-            if type(c) == str:
-                if c not in raw.ch_names:
-                    logger.warning('Exclusion channel %s does not exist. Ignored.' % c)
-                    continue
-                c_int = raw.ch_names.index(c)
-            elif type(c) == int:
-                c_int = c
-            else:
-                logger.error('EXCLUDED_CHANNELS has a value of unknown type %s.\nEXCLUDED_CHANNELS=%s' % (type(c), cfg.EXCLUDED_CHANNELS))
-                raise RuntimeError
-            if c_int in picks:
-                del picks[picks.index(c_int)]
-    if max(picks) > len(raw.ch_names):
-        logger.error('"picks" has a channel index %d while there are only %d channels.' % (max(picks), len(raw.ch_names)))
-        raise ValueError
-
-    if 'decim' not in cfg.FEATURES['PSD']:
-        cfg.FEATURES['PSD']['decim'] = 1
-        logger.warning('PSD["decim"] undefined. Set to 1.')
-
-    # Read epochs
-    try:
-        # Experimental: multiple epoch ranges
-        if type(cfg.EPOCH[0]) is list:
-            epochs_train = []
-            for ep in cfg.EPOCH:
-                epoch = Epochs(raw, events, triggers, tmin=ep[0], tmax=ep[1],
-                    proj=False, picks=picks, baseline=None, preload=True,
-                    verbose=False, detrend=None)
-                epochs_train.append(epoch)
-        else:
-            # Usual method: single epoch range
-            epochs_train = Epochs(raw, events, triggers, tmin=cfg.EPOCH[0], tmax=cfg.EPOCH[1], proj=False,
-                picks=picks, baseline=None, preload=True, verbose=False, detrend=None, on_missing='warn')
-    except:
-        logger.exception('Problem while epoching.')
-        raise RuntimeError
-
-    # Compute features
-    if cfg.FEATURES['selected'] == 'PSD':
-        preprocess = dict(sfreq=epochs_train.info['sfreq'],
-            spatial=cfg.SP_FILTER,
-            spatial_ch=None,
-            spectral=cfg.TP_FILTER[cfg.TP_FILTER['selected']],
-            spectral_ch=None,
-            notch=cfg.NOTCH_FILTER[cfg.NOTCH_FILTER['selected']],
-            notch_ch=None,
-            multiplier=cfg.MULTIPLIER,
-            ch_names=None,
-            rereference=None,
-            decim=cfg.FEATURES['PSD']['decim'],
-            n_jobs=cfg.N_JOBS
-        )
-        featdata = get_psd_feature(epochs_train, cfg.EPOCH, cfg.FEATURES['PSD'], picks=None, preprocess=preprocess, n_jobs=cfg.N_JOBS)
-    elif cfg.FEATURES == 'TIMELAG':
-        '''
-        TODO: Implement multiple epochs for timelag feature
-        '''
-        logger.error('MULTIPLE EPOCHS NOT IMPLEMENTED YET FOR TIMELAG FEATURE.')
-        raise NotImplementedError
-    elif cfg.FEATURES == 'WAVELET':
-        '''
-        TODO: Implement multiple epochs for wavelet feature
-        '''
-        logger.error('MULTIPLE EPOCHS NOT IMPLEMENTED YET FOR WAVELET FEATURE.')
-        raise NotImplementedError
-    else:
-        logger.error('%s feature type is not supported.' % cfg.FEATURES)
-        raise NotImplementedError
-
-    featdata['picks'] = picks
-    featdata['sfreq'] = raw.info['sfreq']
-    featdata['sfreq_features'] = raw.info['sfreq'] / cfg.FEATURES['PSD']['wstep']
-    featdata['wlen'] = cfg.FEATURES['PSD']['wlen']
-    featdata['ch_names'] = [raw.ch_names[i] for i in picks]
-    featdata['ch_names_raw'] = raw.ch_names
-    return featdata
+from __future__ import print_function, division
+
+"""
+features.py
+
+Feature computation module.
+
+
+Kyuhwa Lee, 2019
+Swiss Federal Institute of Technology Lausanne (EPFL)
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+"""
+
+import os
+import mne
+import mne.io
+import numpy as np
+import multiprocessing as mp
+import neurodecode.utils.q_common as qc
+import neurodecode.utils.pycnbi_utils as pu
+from mne import Epochs, pick_types
+from neurodecode import logger
+
+
+def slice_win(epochs_data, w_starts, w_length, psde, picks=None, title=None, flatten=True, preprocess=None, verbose=False):
+    '''
+    Compute PSD values of a sliding window
+
+    Params
+        epochs_data ([channels]x[samples]): raw epoch data
+        w_starts (list): starting indices of sample segments
+        w_length (int): window length in number of samples
+        psde: MNE PSDEstimator object
+        picks (list): subset of channels within epochs_data
+        title (string): print out the title associated with PID
+        flatten (boolean): generate concatenated feature vectors
+            If True: X = [windows] x [channels x freqs]
+            If False: X = [windows] x [channels] x [freqs]
+        preprocess (dict): None or parameters for pycnbi_utils.preprocess() with the following keys:
+            sfreq, spatial, spatial_ch, spectral, spectral_ch, notch, notch_ch,
+            multiplier, ch_names, rereference, decim, n_jobs
+    Returns:
+        [windows] x [channels*freqs] or [windows] x [channels] x [freqs]
+    '''
+
+    # raise error for wrong indexing
+    def WrongIndexError(Exception):
+        logger.error('%s' % Exception)
+
+    if type(w_length) is not int:
+        logger.warning('w_length type is %s. Converting to int.' % type(w_length))
+        w_length = int(w_length)
+    if title is None:
+        title = '[PID %d] Frames %d-%d' % (os.getpid(), w_starts[0], w_starts[-1]+w_length-1)
+    else:
+        title = '[PID %d] %s' % (os.getpid(), title)
+    if preprocess is not None and preprocess['decim'] != 1:
+        title += ' (decim factor %d)' % preprocess['decim']
+    logger.info(title)
+
+    X = None
+    for n in w_starts:
+        n = int(round(n))
+        if n >= epochs_data.shape[1]:
+            logger.error('w_starts has an out-of-bounds index %d for epoch length %d.' % (n, epochs_data.shape[1]))
+            raise WrongIndexError
+        window = epochs_data[:, n:(n + w_length)]
+
+        if preprocess is not None:
+            window = pu.preprocess(window,
+                sfreq=preprocess['sfreq'],
+                spatial=preprocess['spatial'],
+                spatial_ch=preprocess['spatial_ch'],
+                spectral=preprocess['spectral'],
+                spectral_ch=preprocess['spectral_ch'],
+                notch=preprocess['notch'],
+                notch_ch=preprocess['notch_ch'],
+                multiplier=preprocess['multiplier'],
+                ch_names=preprocess['ch_names'],
+                rereference=preprocess['rereference'],
+                decim=preprocess['decim'],
+                n_jobs=preprocess['n_jobs'])
+
+        # dimension: psde.transform( [epochs x channels x times] )
+        psd = psde.transform(window.reshape((1, window.shape[0], window.shape[1])))
+        psd = psd.reshape((psd.shape[0], psd.shape[1] * psd.shape[2]))
+        if picks:
+            psd = psd[0][picks]
+            psd = psd.reshape((1, len(psd)))
+
+        if X is None:
+            X = psd
+        else:
+            X = np.concatenate((X, psd), axis=0)
+
+        if verbose == True:
+            logger.info('[PID %d] processing frame %d / %d' % (os.getpid(), n, w_starts[-1]))
+
+    return X
+
+
+def get_psd(epochs, psde, wlen, wstep, picks=None, flatten=True, preprocess=None, decim=1, n_jobs=1):
+    """
+    Compute multi-taper PSDs over a sliding window
+
+    Input
+    =====
+    epochs: MNE Epochs object
+    psde: MNE PSDEstimator object
+    wlen: window length in frames
+    wstep: window step in frames
+    picks: channels to be used; use all if None
+    flatten: boolean, see Returns section
+    n_jobs: nubmer of cores to use, None = use all cores
+
+    Output
+    ======
+    if flatten==True:
+        X_data: [epochs] x [windows] x [channels*freqs]
+    else:
+        X_data: [epochs] x [windows] x [channels] x [freqs]
+    y_data: [epochs] x [windows]
+
+    TODO:
+        Accept input as numpy array as well, in addition to Epochs object
+    """
+
+    tm = qc.Timer()
+
+    if n_jobs is None:
+        n_jobs = mp.cpu_count()
+    if n_jobs > 1:
+        logger.info('Opening a pool of %d workers' % n_jobs)
+        pool = mp.Pool(n_jobs)
+
+    # compute PSD from sliding windows of each epoch
+    labels = epochs.events[:, -1]
+    epochs_data = epochs.get_data()
+    w_starts = np.arange(0, epochs_data.shape[2] - wlen, wstep)
+    X_data = None
+    y_data = None
+    results = []
+    for ep in np.arange(len(labels)):
+        title = 'Epoch %d / %d, Frames %d-%d' % (ep+1, len(labels), w_starts[0], w_starts[-1] + wlen - 1)
+        if n_jobs == 1:
+            # no multiprocessing
+            results.append(slice_win(epochs_data[ep], w_starts, wlen, psde, picks, title, True, preprocess))
+        else:
+            # parallel psd computation
+            results.append(pool.apply_async(slice_win, [epochs_data[ep], w_starts, wlen, psde, picks, title, True, preprocess]))
+
+    for ep in range(len(results)):
+        if n_jobs == 1:
+            r = results[ep]
+        else:
+            r = results[ep].get()  # windows x features
+        X = r.reshape((1, r.shape[0], r.shape[1]))  # 1 x windows x features
+        if X_data is None:
+            X_data = X
+        else:
+            X_data = np.concatenate((X_data, X), axis=0)
+
+        # speed comparison: http://stackoverflow.com/questions/5891410/numpy-array-initialization-fill-with-identical-values
+        y = np.empty((1, r.shape[0]))  # 1 x windows
+        y.fill(labels[ep])
+        if y_data is None:
+            y_data = y
+        else:
+            y_data = np.concatenate((y_data, y), axis=0)
+
+    # close pool
+    if n_jobs > 1:
+        pool.close()
+        pool.join()
+
+    logger.info('Feature computation took %d seconds.' % tm.sec())
+
+    if flatten:
+        return X_data, y_data.astype(np.int)
+    else:
+        xs = X_data.shape
+        nch = len(epochs.ch_names)
+        return X_data.reshape(xs[0], xs[1], nch, int(xs[2] / nch)), y_data.astype(np.int)
+
+
+def get_psd_feature(epochs_train, window, psdparam, picks=None, preprocess=None, n_jobs=1):
+    """
+    Wrapper for get_psd() adding meta information.
+
+    Input
+    =====
+    epochs_train: mne.Epochs object or list of mne.Epochs object.
+    window: [t_start, t_end]. Time window range for computing PSD.
+    psdparam: {fmin:float, fmax:float, wlen:float, wstep:int, decim:int}.
+              fmin, fmax in Hz, wlen in seconds, wstep in number of samples.
+    picks: Channels to compute features from.
+
+    Output
+    ======
+    dict object containing computed features.
+    """
+
+    if type(window[0]) is list:
+        sfreq = epochs_train[0].info['sfreq']
+        wlen = []
+        w_frames = []
+        # multiple PSD estimators, defined for each epoch
+        if type(psdparam) is list:
+            '''
+            TODO: implement multi-window PSD for each epoch
+            assert len(psdparam) == len(window)
+            for i, p in enumerate(psdparam):
+                if p['wlen'] is None:
+                    wl = window[i][1] - window[i][0]
+                else:
+                    wl = p['wlen']
+                wlen.append(wl)
+                w_frames.append(int(sfreq * wl))
+            '''
+            logger.error('Multiple psd function not implemented yet.')
+            raise NotImplementedError
+        # same PSD estimator for all epochs
+        else:
+            for i, e in enumerate(window):
+                if psdparam['wlen'] is None:
+                    wl = window[i][1] - window[i][0]
+                else:
+                    wl = psdparam['wlen']
+                assert wl > 0
+                wlen.append(wl)
+                w_frames.append(int(round(sfreq * wl)))
+    else:
+        sfreq = epochs_train.info['sfreq']
+        wlen = window[1] - window[0]
+        if psdparam['wlen'] is None:
+            psdparam['wlen'] = wlen
+        w_frames = int(round(sfreq * psdparam['wlen']))  # window length in number of samples(frames)
+    if 'decim' not in psdparam or psdparam['decim'] is None:
+        psdparam['decim'] = 1
+
+    psde_sfreq = sfreq / psdparam['decim']
+    psde = mne.decoding.PSDEstimator(sfreq=psde_sfreq, fmin=psdparam['fmin'], fmax=psdparam['fmax'],
+        bandwidth=None, adaptive=False, low_bias=True, n_jobs=1, normalization='length', verbose='WARNING')
+
+    logger.info_green('PSD computation')
+    if type(epochs_train) is list:
+        X_all = []
+        for i, ep in enumerate(epochs_train):
+            X, Y_data = get_psd(ep, psde, w_frames[i], psdparam['wstep'], picks, n_jobs=n_jobs, preprocess=preprocess, decim=psdparam['decim'])
+            X_all.append(X)
+        # concatenate along the feature dimension
+        # feature index order: window block x channel block x frequency block
+        # feature vector = [window1, window2, ...]
+        # where windowX = [channel1, channel2, ...]
+        # where channelX = [freq1, freq2, ...]
+        X_data = np.concatenate(X_all, axis=2)
+    else:
+        # feature index order: channel block x frequency block
+        # feature vector = [channel1, channel2, ...]
+        # where channelX = [freq1, freq2, ...]
+        X_data, Y_data = get_psd(epochs_train, psde, w_frames, psdparam['wstep'], picks, n_jobs=n_jobs, preprocess=preprocess, decim=psdparam['decim'])
+
+    # assign relative timestamps for each feature. time reference is the leading edge of a window.
+    w_starts = np.arange(0, epochs_train.get_data().shape[2] - w_frames, psdparam['wstep'])
+    t_features = w_starts / sfreq + psdparam['wlen'] + window[0]
+    return dict(X_data=X_data, Y_data=Y_data, wlen=wlen, w_frames=w_frames, psde=psde, times=t_features, decim=psdparam['decim'])
+
+
+def get_timelags(epochs, wlen, wstep, downsample=1, picks=None):
+    """
+    (DEPRECATED FUNCTION)
+    Get concatenated timelag features
+
+    TODO: Unit test.
+
+    Input
+    =====
+    epochs: input signals
+    wlen: window length (# time points) in downsampled data
+    wstep: window step in downsampled data
+    downsample: downsample signal to be 1/downsample length
+    picks: ignored for now
+
+    Output
+    ======
+    X: [epochs] x [windows] x [channels*freqs]
+    y: [epochs] x [labels]
+    """
+
+    '''
+    wlen = int(wlen)
+    wstep = int(wstep)
+    downsample = int(downsample)
+    X_data = None
+    y_data = None
+    labels = epochs.events[:, -1]  # every epoch must have event id
+    epochs_data = epochs.get_data()
+    n_channels = epochs_data.shape[1]
+    # trim to the nearest divisible length
+    epoch_ds_len = int(epochs_data.shape[2] / downsample)
+    epoch_len = downsample * epoch_ds_len
+    range_epochs = np.arange(epochs_data.shape[0])
+    range_channels = np.arange(epochs_data.shape[1])
+    range_windows = np.arange(epoch_ds_len - wlen, 0, -wstep)
+    X_data = np.zeros((len(range_epochs), len(range_windows), wlen * n_channels))
+
+    # for each epoch
+    for ep in range_epochs:
+        epoch = epochs_data[ep, :, :epoch_len]
+        ds = qc.average_every_n(epoch.reshape(-1), downsample)  # flatten to 1-D, then downsample
+        epoch_ds = ds.reshape(n_channels, -1)  # recover structure to channel x samples
+        # for each window over all channels
+        for i in range(len(range_windows)):
+            w = range_windows[i]
+            X = epoch_ds[:, w:w + wlen].reshape(1, -1)  # our feature vector
+            X_data[ep, i, :] = X
+
+        # fill labels
+        y = np.empty((1, len(range_windows)))  # 1 x windows
+        y.fill(labels[ep])
+        if y_data is None:
+            y_data = y
+        else:
+            y_data = np.concatenate((y_data, y), axis=0)
+
+    return X_data, y_data
+    '''
+    logger.error('This function is deprecated.')
+    raise NotImplementedError
+
+def feature2chz(x, fqlist, ch_names):
+    """
+    Label channel, frequency pair for PSD feature indices
+
+    Input
+    =====
+    x: feature index
+    fqlist: list of frequency bands
+    ch_names: list of complete channel names
+
+    Output
+    ======
+    (channel, frequency)
+
+    """
+
+    x = np.array(x).astype('int64').reshape(-1)
+    fqlist = np.array(fqlist).astype('float64')
+    ch_names = np.array(ch_names)
+
+    n_fq = len(fqlist)
+    hz = fqlist[x % n_fq]
+    ch = (x / n_fq).astype('int64')  # 0-based indexing
+
+    return ch_names[ch], hz
+
+
+def cva_features(datadir):
+    """
+    (DEPRECATED FUNCTION)
+    """
+    for fin in qc.get_file_list(datadir, fullpath=True):
+        if fin[-4:] != '.gdf': continue
+        fout = fin + '.cva'
+        if os.path.exists(fout):
+            logger.info('Skipping', fout)
+            continue
+        logger.info("cva_features('%s')" % fin)
+        qc.matlab("cva_features('%s')" % fin)
+
+
+def compute_features(cfg):
+    '''
+    Compute features using config specification.
+
+    Performs preprocessing, epcoching and feature computation.
+
+    Input
+    =====
+    Config file object
+
+    Output
+    ======
+    Feature data in dictionary
+    - X_data: feature vectors
+    - Y_data: feature labels
+    - wlen: window length in seconds
+    - w_frames: window length in frames
+    - psde: MNE PSD estimator object
+    - ch_names: selected channel names
+    - picks: original channel indices of the input fif
+    - sfreq: input sampling frequency
+    - sfreq_features: feature sampling frequency
+    - times: feature timestamp (leading edge of a window)
+    '''
+    # Preprocessing, epoching and PSD computation
+    ftrain = []
+    if hasattr(cfg, 'DATA_FILES'):
+        ftrain = cfg.DATA_FILES
+        logger.info('Using file list defined in cfg.DATA_FILES.')
+    else:
+        for f in qc.get_file_list(cfg.DATA_PATH, fullpath=True):
+            if f[-4:] in ['.fif', '.fiff']:
+                ftrain.append(f)
+        if len(ftrain) > 1 and cfg.PICKED_CHANNELS is not None and type(cfg.PICKED_CHANNELS[0]) == int:
+            logger.error('When loading multiple EEG files, PICKED_CHANNELS must be list of string, not integers because they may have different channel order.')
+            raise RuntimeError
+    raw, events = pu.load_multi(ftrain)
+
+    reref = cfg.REREFERENCE[cfg.REREFERENCE['selected']]
+    if reref is not None:
+        pu.rereference(raw, reref['New'], reref['Old'])
+
+    if cfg.LOAD_EVENTS[cfg.LOAD_EVENTS['selected']] is not None:
+        events = mne.read_events(cfg.LOAD_EVENTS[cfg.LOAD_EVENTS['selected']])
+
+    trigger_def_int = set()
+    for a in cfg.TRIGGER_DEF:
+        trigger_def_int.add(getattr(cfg.tdef, a))
+    triggers = {cfg.tdef.by_value[c]:c for c in trigger_def_int}
+
+    # Pick channels
+    if cfg.PICKED_CHANNELS is None or len(cfg.PICKED_CHANNELS) == 0:
+        picks = [int(x) for x in pick_types(raw.info, stim=False, eeg=True)]
+        chlist = [raw.ch_names[x] for x in picks]
+    else:
+        chlist = cfg.PICKED_CHANNELS
+        picks = []
+        for c in chlist:
+            if type(c) == int:
+                picks.append(c)
+            elif type(c) == str:
+                picks.append(raw.ch_names.index(c))
+            else:
+                logger.error('PICKED_CHANNELS has a value of unknown type %s.\nPICKED_CHANNELS=%s' % (type(c), cfg.PICKED_CHANNELS))
+                raise RuntimeError
+
+    if cfg.EXCLUDED_CHANNELS is not None and len(cfg.EXCLUDED_CHANNELS) > 0:
+        if len(set(cfg.EXCLUDED_CHANNELS) & set(cfg.PICKED_CHANNELS)) > 0:
+            logger.error('in config, EXCLUDED_CHANNELS and PICKED_CHANNELS must not contain the same channel')
+            raise ValueError
+        for c in cfg.EXCLUDED_CHANNELS:
+            if type(c) == str:
+                if c not in raw.ch_names:
+                    logger.warning('Exclusion channel %s does not exist. Ignored.' % c)
+                    continue
+                c_int = raw.ch_names.index(c)
+            elif type(c) == int:
+                c_int = c
+            else:
+                logger.error('EXCLUDED_CHANNELS has a value of unknown type %s.\nEXCLUDED_CHANNELS=%s' % (type(c), cfg.EXCLUDED_CHANNELS))
+                raise RuntimeError
+            if c_int in picks:
+                del picks[picks.index(c_int)]
+    if max(picks) > len(raw.ch_names):
+        logger.error('"picks" has a channel index %d while there are only %d channels.' % (max(picks), len(raw.ch_names)))
+        raise ValueError
+
+    if 'decim' not in cfg.FEATURES['PSD']:
+        cfg.FEATURES['PSD']['decim'] = 1
+        logger.warning('PSD["decim"] undefined. Set to 1.')
+
+    # Read epochs
+    try:
+        # Experimental: multiple epoch ranges
+        if type(cfg.EPOCH[0]) is list:
+            epochs_train = []
+            for ep in cfg.EPOCH:
+                epoch = Epochs(raw, events, triggers, tmin=ep[0], tmax=ep[1],
+                    proj=False, picks=picks, baseline=None, preload=True,
+                    verbose=False, detrend=None)
+                epochs_train.append(epoch)
+        else:
+            # Usual method: single epoch range
+            epochs_train = Epochs(raw, events, triggers, tmin=cfg.EPOCH[0], tmax=cfg.EPOCH[1], proj=False,
+                picks=picks, baseline=None, preload=True, verbose=False, detrend=None, on_missing='warn')
+    except:
+        logger.exception('Problem while epoching.')
+        raise RuntimeError
+
+    # Compute features
+    if cfg.FEATURES['selected'] == 'PSD':
+        preprocess = dict(sfreq=epochs_train.info['sfreq'],
+            spatial=cfg.SP_FILTER,
+            spatial_ch=None,
+            spectral=cfg.TP_FILTER[cfg.TP_FILTER['selected']],
+            spectral_ch=None,
+            notch=cfg.NOTCH_FILTER[cfg.NOTCH_FILTER['selected']],
+            notch_ch=None,
+            multiplier=cfg.MULTIPLIER,
+            ch_names=None,
+            rereference=None,
+            decim=cfg.FEATURES['PSD']['decim'],
+            n_jobs=cfg.N_JOBS
+        )
+        featdata = get_psd_feature(epochs_train, cfg.EPOCH, cfg.FEATURES['PSD'], picks=None, preprocess=preprocess, n_jobs=cfg.N_JOBS)
+    elif cfg.FEATURES == 'TIMELAG':
+        '''
+        TODO: Implement multiple epochs for timelag feature
+        '''
+        logger.error('MULTIPLE EPOCHS NOT IMPLEMENTED YET FOR TIMELAG FEATURE.')
+        raise NotImplementedError
+    elif cfg.FEATURES == 'WAVELET':
+        '''
+        TODO: Implement multiple epochs for wavelet feature
+        '''
+        logger.error('MULTIPLE EPOCHS NOT IMPLEMENTED YET FOR WAVELET FEATURE.')
+        raise NotImplementedError
+    else:
+        logger.error('%s feature type is not supported.' % cfg.FEATURES)
+        raise NotImplementedError
+
+    featdata['picks'] = picks
+    featdata['sfreq'] = raw.info['sfreq']
+    featdata['sfreq_features'] = raw.info['sfreq'] / cfg.FEATURES['PSD']['wstep']
+    featdata['wlen'] = cfg.FEATURES['PSD']['wlen']
+    featdata['ch_names'] = [raw.ch_names[i] for i in picks]
+    featdata['ch_names_raw'] = raw.ch_names
+    return featdata
```

### Comparing `neurodecode-2.0.4/neurodecode/decoder/rlda.py` & `neurodecode-2.0.5/neurodecode/decoder/rlda.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-from __future__ import print_function, division
-
-"""
-Regularized LDA
-
-The code was implemented based on the following paper:
-Dornhege et al., "General Signal Processing and Machine Learning Tools for
-BCI Analysis Toward Brain-Computer Interfacing", MIT Press, 2007, page 218.
-
-Kyuhwa Lee
-Swiss Federal Institute of Technology Lausanne (EPFL)
-
-"""
-
-import sys
-import math
-import numpy as np
-from neurodecode import logger
-
-class rLDA(object):
-    def __init__(self, reg_cov=None):
-        if reg_cov > 1:
-            raise RuntimeError('reg_cov > 1')
-        self.lambdaStar = reg_cov
-
-    def fit(self, X, Y):
-        """
-        Train rLDA
-
-        Input
-        -----
-        X(Data): 2-D numpy array. [ samples x features ]
-        Y(Label): 1-D numpy array.
-
-        Output
-        ------
-        w: weight vector. [ samples ]
-        b: bias scalar.
-
-        Note that the rLDA object itself is also updated with w and b, i.e.,
-        the return values can be safely ignored.
-
-        """
-        labels = np.unique(Y)
-        if X.ndim != 2:
-            raise RuntimeError('X must be 2 dimensional.')
-        if len(labels) != 2 or labels[0] == labels[1]:
-            raise RuntimeError('Exactly two different labels required.')
-
-        index1 = np.where(Y == labels[0])[0]
-        index2 = np.where(Y == labels[1])[0]
-        cov = np.matrix(np.cov(X.T))
-        mu1 = np.matrix(np.mean(X[index1], axis=0).T).T
-        mu2 = np.matrix(np.mean(X[index2], axis=0).T).T
-        mu = (mu1 + mu2) / 2;
-        numFeatures = X.shape[1]
-
-        if self.lambdaStar is not None and numFeatures > 1:
-            cov = (1 - self.lambdaStar) * cov + (self.lambdaStar / numFeatures) * np.trace(cov) * np.eye(cov.shape[0])
-
-        w = np.linalg.pinv(cov) * (mu2 - mu1)
-        b = -(w.T) * mu
-
-        for wi in w:
-            assert not math.isnan(wi)
-        assert not math.isnan(b)
-
-        self.w = np.array(w).reshape(-1)  # vector
-        self.b = np.array(b).reshape(-1)  # scalar
-        self.labels = labels
-
-        return self.w, self.b
-
-    def predict(self, X, proba=False):
-        """
-        Returns the predicted class labels optionally with likelihoods
-        """
-        probs = []
-        predicted = []
-        for row in X:
-            probability = float(self.w.T * np.matrix(row).T + self.b.T)
-            if probability >= 0:
-                predicted.append(self.labels[1])
-            else:
-                predicted.append(self.labels[0])
-
-            # rescale from 0 to 1, similar to scikit-learn's way
-            prob_norm = 1.0 / (np.exp(-probability / 10.0) + 1.0)
-            # values are in the same order as that of self.labels
-            probs.append([1 - prob_norm, prob_norm])
-
-        if proba:
-            return np.array(probs)
-        else:
-            return predicted
-
-    def predict_proba(self, X):
-        """
-        Returns the predicted class labels and likelihoods
-        """
-        return self.predict(X, proba=True)
-
-    def get_labels(self):
-        """
-        Returns labels in the same order as you get when you call predict()
-        """
-        return self.labels
-
-    def score(self, X, true_labels):
-        raise RuntimeError('SORRY: FUNCTION IS NOT IMPLEMENTED YET.')
+from __future__ import print_function, division
+
+"""
+Regularized LDA
+
+The code was implemented based on the following paper:
+Dornhege et al., "General Signal Processing and Machine Learning Tools for
+BCI Analysis Toward Brain-Computer Interfacing", MIT Press, 2007, page 218.
+
+Kyuhwa Lee
+Swiss Federal Institute of Technology Lausanne (EPFL)
+
+"""
+
+import sys
+import math
+import numpy as np
+from neurodecode import logger
+
+class rLDA(object):
+    def __init__(self, reg_cov=None):
+        if reg_cov > 1:
+            raise RuntimeError('reg_cov > 1')
+        self.lambdaStar = reg_cov
+
+    def fit(self, X, Y):
+        """
+        Train rLDA
+
+        Input
+        -----
+        X(Data): 2-D numpy array. [ samples x features ]
+        Y(Label): 1-D numpy array.
+
+        Output
+        ------
+        w: weight vector. [ samples ]
+        b: bias scalar.
+
+        Note that the rLDA object itself is also updated with w and b, i.e.,
+        the return values can be safely ignored.
+
+        """
+        labels = np.unique(Y)
+        if X.ndim != 2:
+            raise RuntimeError('X must be 2 dimensional.')
+        if len(labels) != 2 or labels[0] == labels[1]:
+            raise RuntimeError('Exactly two different labels required.')
+
+        index1 = np.where(Y == labels[0])[0]
+        index2 = np.where(Y == labels[1])[0]
+        cov = np.matrix(np.cov(X.T))
+        mu1 = np.matrix(np.mean(X[index1], axis=0).T).T
+        mu2 = np.matrix(np.mean(X[index2], axis=0).T).T
+        mu = (mu1 + mu2) / 2;
+        numFeatures = X.shape[1]
+
+        if self.lambdaStar is not None and numFeatures > 1:
+            cov = (1 - self.lambdaStar) * cov + (self.lambdaStar / numFeatures) * np.trace(cov) * np.eye(cov.shape[0])
+
+        w = np.linalg.pinv(cov) * (mu2 - mu1)
+        b = -(w.T) * mu
+
+        for wi in w:
+            assert not math.isnan(wi)
+        assert not math.isnan(b)
+
+        self.w = np.array(w).reshape(-1)  # vector
+        self.b = np.array(b).reshape(-1)  # scalar
+        self.labels = labels
+
+        return self.w, self.b
+
+    def predict(self, X, proba=False):
+        """
+        Returns the predicted class labels optionally with likelihoods
+        """
+        probs = []
+        predicted = []
+        for row in X:
+            probability = float(self.w.T * np.matrix(row).T + self.b.T)
+            if probability >= 0:
+                predicted.append(self.labels[1])
+            else:
+                predicted.append(self.labels[0])
+
+            # rescale from 0 to 1, similar to scikit-learn's way
+            prob_norm = 1.0 / (np.exp(-probability / 10.0) + 1.0)
+            # values are in the same order as that of self.labels
+            probs.append([1 - prob_norm, prob_norm])
+
+        if proba:
+            return np.array(probs)
+        else:
+            return predicted
+
+    def predict_proba(self, X):
+        """
+        Returns the predicted class labels and likelihoods
+        """
+        return self.predict(X, proba=True)
+
+    def get_labels(self):
+        """
+        Returns labels in the same order as you get when you call predict()
+        """
+        return self.labels
+
+    def score(self, X, true_labels):
+        raise RuntimeError('SORRY: FUNCTION IS NOT IMPLEMENTED YET.')
```

### Comparing `neurodecode-2.0.4/neurodecode/decoder/trainer.py` & `neurodecode-2.0.5/neurodecode/decoder/trainer.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,703 +1,703 @@
-from __future__ import print_function, division
-
-"""
-trainer.py
-
-Perform cross-validation and train a classifier.
-See run() to see the overall flow.
-
-When you add more classifiers, modify "CLASSIFIERS" variable to include your classifier.
-
-Kyuhwa Lee, 2018
-Swiss Federal Institute of Technology Lausanne (EPFL)
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""
-
-import os
-import sys
-import imp
-import mne
-import mne.io
-import platform
-import numpy as np
-import multiprocessing as mp
-import sklearn.metrics as skmetrics
-import neurodecode.utils.q_common as qc
-import neurodecode.utils.pycnbi_utils as pu
-import neurodecode.decoder.features as features
-from builtins import input
-from sklearn.ensemble import RandomForestClassifier
-from sklearn.ensemble import GradientBoostingClassifier
-from xgboost import XGBClassifier
-from lightgbm import LGBMClassifier
-from sklearn.discriminant_analysis import LinearDiscriminantAnalysis as LDA
-from neurodecode.decoder.rlda import rLDA
-from neurodecode import logger
-from neurodecode.triggers.trigger_def import trigger_def
-
-# supported classifiers: add this part as you add more classifiers
-CLASSIFIERS = {'RF':RandomForestClassifier, 'GB':GradientBoostingClassifier, 'XGB':XGBClassifier,
-    'LGB':LGBMClassifier, 'LDA':LDA, 'rLDA':rLDA}
-
-# scikit-learn old version compatibility
-try:
-    from sklearn.model_selection import StratifiedShuffleSplit, LeaveOneOut
-    SKLEARN_OLD = False
-except ImportError:
-    from sklearn.cross_validation import StratifiedShuffleSplit, LeaveOneOut
-    SKLEARN_OLD = True
-mne.set_log_level('ERROR')
-os.environ['OMP_NUM_THREADS'] = '1' # actually improves performance for multitaper
-
-def check_config(cfg):
-    critical_vars = {
-        'COMMON': ['TRIGGER_FILE',
-                    'TRIGGER_DEF',
-                    'EPOCH',
-                    'DATA_PATH',
-                    'PICKED_CHANNELS',
-                    'SP_FILTER',
-                    'TP_FILTER',
-                    'NOTCH_FILTER',
-                    'FEATURES',
-                    'CLASSIFIER',
-                    'CV_PERFORM'],
-                    'RF': ['n_estimators'],
-                    'GB': ['n_estimators', 'learning_rate'],
-                    'XGB': ['n_estimators', 'learning_rate'],
-                    'LGB': ['n_estimators', 'learning_rate'],
-                    'LDA': [],
-                    'rLDA': ['reg_cov'],
-                    'StratifiedShuffleSplit': ['test_ratio', 'folds', 'seed', 'export_result'],
-                    'LeaveOneOut': ['export_result']
-    }
-
-    # optional variables with default values
-    optional_vars = {
-        'MULTIPLIER': 1,
-        'EXPORT_GOOD_FEATURES': False,
-        'FEAT_TOPN': 10,
-        'EXPORT_CLS': False,
-        'REREFERENCE': None,
-        'N_JOBS': None,
-        'EXCLUDED_CHANNELS': None,
-        'LOAD_EVENTS': None,
-        'CV': {'IGNORE_THRES': None, 'DECISION_THRES': None, 'BALANCE_SAMPLES': False},
-    }
-
-    for v in critical_vars['COMMON']:
-        if not hasattr(cfg, v):
-            logger.error('%s not defined in config.' % v)
-            raise KeyError
-
-    for key in optional_vars:
-        if not hasattr(cfg, key):
-            setattr(cfg, key, optional_vars[key])
-            logger.warning('Setting undefined parameter %s=%s' % (key, getattr(cfg, key)))
-
-    if 'decim' not in cfg.FEATURES['PSD']:
-        cfg.FEATURES['PSD']['decim'] = 1
-
-    # classifier parameters check
-    selected_classifier = cfg.CLASSIFIER['selected']
-    if selected_classifier not in cfg.CLASSIFIER:
-        logger.error('"%s" not defined in your config.' % selected_classifier)
-        raise KeyError
-    for v in critical_vars[selected_classifier]:
-        if v not in cfg.CLASSIFIER[selected_classifier]:
-            logger.error('parameter %s must be defined for %s classifier.' % (v, selected_classifier))
-            raise KeyError
-
-    cv_selected = cfg.CV_PERFORM['selected']
-    if cfg.CV_PERFORM[cv_selected] is not None:
-        if cv_selected not in cfg.CV_PERFORM:
-            logger.error('"%s" not defined in config.' % cv_selected)
-            raise KeyError
-        for v in critical_vars[cv_selected]:
-            if v not in cfg.CV_PERFORM[cv_selected]:
-                logger.error('parameter %s must be defined for %s.' % (v, cv_selected))
-                raise KeyError
-    if cfg.N_JOBS is None:
-        cfg.N_JOBS = mp.cpu_count()
-
-    return cfg
-
-
-def balance_samples(X, Y, balance_type, verbose=False):
-    if balance_type == 'OVER':
-        """
-        Oversample from classes that lack samples
-        """
-        label_set = np.unique(Y)
-        max_set = []
-        X_balanced = np.array(X)
-        Y_balanced = np.array(Y)
-
-        # find a class with maximum number of samples
-        for c in label_set:
-            yl = np.where(Y == c)[0]
-            if len(max_set) == 0 or len(yl) > max_set[1]:
-                max_set = [c, len(yl)]
-        for c in label_set:
-            if c == max_set[0]: continue
-            yl = np.where(Y == c)[0]
-            extra_samples = max_set[1] - len(yl)
-            extra_idx = np.random.choice(yl, extra_samples)
-            X_balanced = np.append(X_balanced, X[extra_idx], axis=0)
-            Y_balanced = np.append(Y_balanced, Y[extra_idx], axis=0)
-    elif balance_type == 'UNDER':
-        """
-        Undersample from classes that are excessive
-        """
-        label_set = np.unique(Y)
-        min_set = []
-
-        # find a class with minimum number of samples
-        for c in label_set:
-            yl = np.where(Y == c)[0]
-            if len(min_set) == 0 or len(yl) < min_set[1]:
-                min_set = [c, len(yl)]
-        yl = np.where(Y == min_set[0])[0]
-        X_balanced = np.array(X[yl])
-        Y_balanced = np.array(Y[yl])
-        for c in label_set:
-            if c == min_set[0]: continue
-            yl = np.where(Y == c)[0]
-            reduced_idx = np.random.choice(yl, min_set[1])
-            X_balanced = np.append(X_balanced, X[reduced_idx], axis=0)
-            Y_balanced = np.append(Y_balanced, Y[reduced_idx], axis=0)
-    elif balance_type is None or balance_type is False:
-        return X, Y
-    else:
-        logger.error('Unknown balancing type %s' % balance_type)
-        raise ValueError
-
-    logger.info_green('\nNumber of samples after %ssampling' % balance_type.lower())
-    for c in label_set:
-        logger.info('%s: %d -> %d' % (c, len(np.where(Y == c)[0]), len(np.where(Y_balanced == c)[0])))
-
-    return X_balanced, Y_balanced
-
-
-def crossval_epochs(cv, epochs_data, labels, cls, label_names=None, do_balance=None, n_jobs=None, ignore_thres=None, decision_thres=None):
-    """
-    Epoch-based cross-validation used by cross_validate().
-
-    Params
-    ======
-    cv: scikit-learn cross-validation object
-    epochs_data: np.array of shape [epochs x samples x features]
-    labels: np.array of shape [epochs x samples]
-    cls: classifier
-    label_names: associated label names {0:'Left', 1:'Right', ...}
-    do_balance: oversample or undersample to match the number of samples among classes
-
-    """
-
-    scores = []
-    f1s = []
-    cnum = 1
-    cm_sum = 0
-    label_set = np.unique(labels)
-    num_labels = len(label_set)
-    if label_names is None:
-        label_names = {l:'%s' % l for l in label_set}
-
-    if n_jobs is None:
-        n_jobs = mp.cpu_count()
-
-    if n_jobs > 1:
-        logger.info('crossval_epochs(): Using %d cores' % n_jobs)
-        pool = mp.Pool(n_jobs)
-        results = []
-
-    # for classifier itself, single core is usually faster
-    cls.n_jobs = 1
-
-    if SKLEARN_OLD:
-        splits = cv
-    else:
-        splits = cv.split(epochs_data, labels[:, 0])
-    for train, test in splits:
-        X_train = np.concatenate(epochs_data[train])
-        X_test = np.concatenate(epochs_data[test])
-        Y_train = np.concatenate(labels[train])
-        Y_test = np.concatenate(labels[test])
-        if do_balance:
-            X_train, Y_train = balance_samples(X_train, Y_train, do_balance)
-            X_test, Y_test = balance_samples(X_test, Y_test, do_balance)
-
-        if n_jobs > 1:
-            results.append(pool.apply_async(fit_predict_thres,
-                                            [cls, X_train, Y_train, X_test, Y_test, cnum, label_set, ignore_thres, decision_thres]))
-        else:
-            score, cm, f1 = fit_predict_thres(cls, X_train, Y_train, X_test, Y_test, cnum, label_set, ignore_thres, decision_thres)
-            scores.append(score)
-            f1s.append(f1)
-            cm_sum += cm
-        cnum += 1
-
-    if n_jobs > 1:
-        pool.close()
-        pool.join()
-
-        for r in results:
-            score, cm, f1 = r.get()
-            scores.append(score)
-            f1s.append(f1)
-            cm_sum += cm
-
-    # confusion matrix
-    cm_sum = cm_sum.astype('float')
-    if cm_sum.shape[0] != cm_sum.shape[1]:
-        # we have decision thresholding condition
-        assert cm_sum.shape[0] < cm_sum.shape[1]
-        cm_sum_all = cm_sum
-        cm_sum = cm_sum[:, :cm_sum.shape[0]]
-        underthres = np.array([r[-1] / sum(r) for r in cm_sum_all])
-    else:
-        underthres = None
-
-    cm_rate = np.zeros(cm_sum.shape)
-    for r_in, r_out in zip(cm_sum, cm_rate):
-        rs = sum(r_in)
-        if rs > 0:
-            r_out[:] = r_in / rs
-        else:
-            assert min(r) == max(r) == 0
-    if underthres is not None:
-        cm_rate = np.concatenate((cm_rate, underthres[:, np.newaxis]), axis=1)
-
-    cm_txt = 'Y: ground-truth, X: predicted\n'
-    max_chars = 12
-    tpl_str = '%%-%ds ' % max_chars
-    tpl_float = '%%-%d.2f ' % max_chars
-    for l in label_set:
-        cm_txt += tpl_str % label_names[l][:max_chars]
-    if underthres is not None:
-        cm_txt += tpl_str % 'Ignored'
-    cm_txt += '\n'
-    for r in cm_rate:
-        for c in r:
-            cm_txt += tpl_float % c
-        cm_txt += '\n'
-    cm_txt += 'Average accuracy: %.2f\n' % np.mean(scores)
-    cm_txt += 'Average F1 score: %.2f\n' % np.mean(f1s)
-
-    return np.array(scores), cm_txt
-
-
-def balance_tpr(cfg, featdata):
-    """
-    Find the threshold of class index 0 that yields equal number of true positive samples of each class.
-    Currently only available for binary classes.
-
-    Params
-    ======
-    cfg: config module
-    feetdata: feature data computed using compute_features()
-    """
-
-    n_jobs = cfg.N_JOBS
-    if n_jobs is None:
-        n_jobs = mp.cpu_count()
-    if n_jobs > 1:
-        logger.info('balance_tpr(): Using %d cores' % n_jobs)
-        pool = mp.Pool(n_jobs)
-        results = []
-
-    # Init a classifier
-    selected_classifier = cfg.CLASSIFIER[cfg.CLASSIFIER['selected']]
-    if selected_classifier not in CLASSIFIERS:
-        logger.error('Unsupported classifier %s' % selected_classifier)
-        raise ValueError
-    params = cfg.CLASSIFIER[selected_classifier]
-    cls = CLASSIFIERS[selected_classifier](**params)
-
-    # Setup features
-    X_data = featdata['X_data']
-    Y_data = featdata['Y_data']
-    wlen = featdata['wlen']
-    if cfg.CLASSIFIER['PSD']['wlen'] is None:
-        cfg.CLASSIFIER['PSD']['wlen'] = wlen
-
-    # Choose CV type
-    ntrials, nsamples, fsize = X_data.shape
-    selected_CV = cfg.CV_PERFORM[cfg.CV_PERFORM['selected']]
-    if cselected_CV == 'LeaveOneOut':
-        logger.info_green('\n%d-fold leave-one-out cross-validation' % ntrials)
-        if SKLEARN_OLD:
-            cv = LeaveOneOut(len(Y_data))
-        else:
-            cv = LeaveOneOut()
-    elif selected_CV == 'StratifiedShuffleSplit':
-        logger.info_green('\n%d-fold stratified cross-validation with test set ratio %.2f' % (cfg.CV_PERFORM[selected_CV]['folds'], cfg.CV_PERFORM[selected_CV]['test_ratio']))
-        if SKLEARN_OLD:
-            cv = StratifiedShuffleSplit(Y_data[:, 0], cfg.CV_PERFORM[selected_CV]['folds'], test_size=cfg.CV_PERFORM[selected_CV]['test_ratio'], random_state=cfg.CV_PERFORM[selected_CV]['random_seed'])
-        else:
-            cv = StratifiedShuffleSplit(n_splits=cfg.CV_PERFORM[selected_CV]['folds'], test_size=cfg.CV_PERFORM[selected_CV]['test_ratio'], random_state=cfg.CV_PERFORM[selected_CV]['random_seed'])
-    else:
-        logger.error('%s is not supported yet. Sorry.' % selected_CV)
-        raise NotImplementedError
-    logger.info('%d trials, %d samples per trial, %d feature dimension' % (ntrials, nsamples, fsize))
-
-    # For classifier itself, single core is usually faster
-    cls.n_jobs = 1
-    Y_preds = []
-
-    if SKLEARN_OLD:
-        splits = cv
-    else:
-        splits = cv.split(X_data, Y_data[:, 0])
-    for cnum, (train, test) in enumerate(splits):
-        X_train = np.concatenate(X_data[train])
-        X_test = np.concatenate(X_data[test])
-        Y_train = np.concatenate(Y_data[train])
-        Y_test = np.concatenate(Y_data[test])
-        if n_jobs > 1:
-            results.append(pool.apply_async(get_predict_proba, [cls, X_train, Y_train, X_test, Y_test, cnum+1]))
-        else:
-            Y_preds.append(get_predict_proba(cls, X_train, Y_train, X_test, Y_test, cnum+1))
-        cnum += 1
-
-    # Aggregate predictions
-    if n_jobs > 1:
-        pool.close()
-        pool.join()
-        for r in results:
-            Y_preds.append(r.get())
-    Y_preds = np.concatenate(Y_preds, axis=0)
-
-    # Find threshold for class index 0
-    Y_preds = sorted(Y_preds)
-    mid_idx = int(len(Y_preds) / 2)
-    if len(Y_preds) == 1:
-        return 0.5 # should not reach here in normal conditions
-    elif len(Y_preds) % 2 == 0:
-        thres = Y_preds[mid_idx-1] + (Y_preds[mid_idx] - Y_preds[mid_idx-1]) / 2
-    else:
-        thres = Y_preds[mid_idx]
-    return thres
-
-
-def cva_features(datadir):
-    """
-    (DEPRECATED FUNCTION)
-    """
-    for fin in qc.get_file_list(datadir, fullpath=True):
-        if fin[-4:] != '.gdf': continue
-        fout = fin + '.cva'
-        if os.path.exists(fout):
-            logger.info('Skipping', fout)
-            continue
-        logger.info("cva_features('%s')" % fin)
-        qc.matlab("cva_features('%s')" % fin)
-
-
-def get_predict_proba(cls, X_train, Y_train, X_test, Y_test, cnum):
-    """
-    All likelihoods will be collected from every fold of a cross-validaiton. Based on these likelihoods,
-    a threshold will be computed that will balance the true positive rate of each class.
-    Available with binary classification scenario only.
-    """
-    timer = qc.Timer()
-    cls.fit(X_train, Y_train)
-    Y_pred = cls.predict_proba(X_test)
-    logger.info('Cross-validation %d (%d tests) - %.1f sec' % (cnum, Y_pred.shape[0], timer.sec()))
-    return Y_pred[:,0]
-
-
-def fit_predict_thres(cls, X_train, Y_train, X_test, Y_test, cnum, label_list, ignore_thres=None, decision_thres=None):
-    """
-    Any likelihood lower than a threshold is not counted as classification score
-    Confusion matrix, accuracy and F1 score (macro average) are computed.
-
-    Params
-    ======
-    ignore_thres:
-    if not None or larger than 0, likelihood values lower than ignore_thres will be ignored
-    while computing confusion matrix.
-
-    """
-    timer = qc.Timer()
-    cls.fit(X_train, Y_train)
-    assert ignore_thres is None or ignore_thres >= 0
-    if ignore_thres is None or ignore_thres == 0:
-        Y_pred = cls.predict(X_test)
-        score = skmetrics.accuracy_score(Y_test, Y_pred)
-        cm = skmetrics.confusion_matrix(Y_test, Y_pred, labels=label_list)
-        f1 = skmetrics.f1_score(Y_test, Y_pred, average='macro')
-    else:
-        if decision_thres is not None:
-            logger.error('decision threshold and ignore_thres cannot be set at the same time.')
-            raise ValueError
-        Y_pred = cls.predict_proba(X_test)
-        Y_pred_labels = np.argmax(Y_pred, axis=1)
-        Y_pred_maxes = np.array([x[i] for i, x in zip(Y_pred_labels, Y_pred)])
-        Y_index_overthres = np.where(Y_pred_maxes >= ignore_thres)[0]
-        Y_index_underthres = np.where(Y_pred_maxes < ignore_thres)[0]
-        Y_pred_overthres = np.array([cls.classes_[x] for x in Y_pred_labels[Y_index_overthres]])
-        Y_pred_underthres = np.array([cls.classes_[x] for x in Y_pred_labels[Y_index_underthres]])
-        Y_pred_underthres_count = np.array([np.count_nonzero(Y_pred_underthres == c) for c in label_list])
-        Y_test_overthres = Y_test[Y_index_overthres]
-        score = skmetrics.accuracy_score(Y_test_overthres, Y_pred_overthres)
-        cm = skmetrics.confusion_matrix(Y_test_overthres, Y_pred_overthres, labels=label_list)
-        cm = np.concatenate((cm, Y_pred_underthres_count[:, np.newaxis]), axis=1)
-        f1 = skmetrics.f1_score(Y_test_overthres, Y_pred_overthres, average='macro')
-
-    logger.info('Cross-validation %d (%.3f) - %.1f sec' % (cnum, score, timer.sec()))
-    return score, cm, f1
-
-
-def cross_validate(cfg, featdata, cv_file=None):
-    """
-    Perform cross validation
-    """
-    # Init a classifier
-    selected_classifier = cfg.CLASSIFIER['selected']
-    if selected_classifier not in CLASSIFIERS:
-        logger.error('Unsupported classifier %s' % selected_classifier)
-        raise ValueError
-    params = cfg.CLASSIFIER[selected_classifier]
-    cls = CLASSIFIERS[selected_classifier](**params)
-
-    # Setup features
-    X_data = featdata['X_data']
-    Y_data = featdata['Y_data']
-    wlen = featdata['wlen']
-
-    # Choose CV type
-    ntrials, nsamples, fsize = X_data.shape
-    selected_cv =  cfg.CV_PERFORM['selected']
-    if selected_cv == 'LeaveOneOut':
-        logger.info_green('%d-fold leave-one-out cross-validation' % ntrials)
-        if SKLEARN_OLD:
-            cv = LeaveOneOut(len(Y_data))
-        else:
-            cv = LeaveOneOut()
-    elif selected_cv == 'StratifiedShuffleSplit':
-        logger.info_green('%d-fold stratified cross-validation with test set ratio %.2f' % (cfg.CV_PERFORM[selected_cv]['folds'], cfg.CV_PERFORM[selected_cv]['test_ratio']))
-        if SKLEARN_OLD:
-            cv = StratifiedShuffleSplit(Y_data[:, 0], cfg.CV_PERFORM[selected_cv]['folds'], test_size=cfg.CV_PERFORM[selected_cv]['test_ratio'], random_state=cfg.CV_PERFORM[selected_cv]['seed'])
-        else:
-            cv = StratifiedShuffleSplit(n_splits=cfg.CV_PERFORM[selected_cv]['folds'], test_size=cfg.CV_PERFORM[selected_cv]['test_ratio'], random_state=cfg.CV_PERFORM[selected_cv]['seed'])
-    else:
-        logger.error('%s is not supported yet. Sorry.' % cfg.CV_PERFORM[cfg.CV_PERFORM['selected']])
-        raise NotImplementedError
-    logger.info('%d trials, %d samples per trial, %d feature dimension' % (ntrials, nsamples, fsize))
-
-    # Do it!
-    timer_cv = qc.Timer()
-    scores, cm_txt = crossval_epochs(cv, X_data, Y_data, cls, cfg.tdef.by_value, cfg.CV['BALANCE_SAMPLES'], n_jobs=cfg.N_JOBS,
-                                     ignore_thres=cfg.CV['IGNORE_THRES'], decision_thres=cfg.CV['DECISION_THRES'])
-    t_cv = timer_cv.sec()
-
-    # Export results
-    txt = 'Cross validation took %d seconds.\n' % t_cv
-    txt += '\n- Class information\n'
-    txt += '%d epochs, %d samples per epoch, %d feature dimension (total %d samples)\n' %\
-        (ntrials, nsamples, fsize, ntrials * nsamples)
-    for ev in np.unique(Y_data):
-        txt += '%s: %d trials\n' % (cfg.tdef.by_value[ev], len(np.where(Y_data[:, 0] == ev)[0]))
-    if cfg.CV['BALANCE_SAMPLES']:
-        txt += 'The number of samples was balanced using %ssampling.\n' % cfg.BALANCE_SAMPLES.lower()
-    txt += '\n- Experiment condition\n'
-    txt += 'Sampling frequency: %.3f Hz\n' % featdata['sfreq']
-    txt += 'Spatial filter: %s\n' % cfg.SP_FILTER
-    txt += 'Spectral filter: %s\n' % cfg.TP_FILTER[cfg.TP_FILTER['selected']]
-    txt += 'Notch filter: %s\n' % cfg.NOTCH_FILTER[cfg.NOTCH_FILTER['selected']]
-    #txt += 'Channels: ' + ','.join([str(featdata['ch_names'][p]) for p in featdata['picks']]) + '\n'
-    txt += 'Channels: %s\n' % featdata['ch_names']
-    txt += 'PSD range: %.1f - %.1f Hz\n' % (cfg.FEATURES['PSD']['fmin'], cfg.FEATURES['PSD']['fmax'])
-    txt += 'Window step: %.2f msec\n' % (1000.0 * cfg.FEATURES['PSD']['wstep'] / featdata['sfreq'])
-    if type(wlen) is list:
-        for i, w in enumerate(wlen):
-            txt += 'Window size: %.1f msec\n' % (w * 1000.0)
-            txt += 'Epoch range: %s sec\n' % (cfg.EPOCH[i])
-    else:
-        txt += 'Window size: %.1f msec\n' % (cfg.FEATURES['PSD']['wlen'] * 1000.0)
-        txt += 'Epoch range: %s sec\n' % (cfg.EPOCH)
-    txt += 'Decimation factor: %d\n' % cfg.FEATURES['PSD']['decim']
-
-    # Compute stats
-    cv_mean, cv_std = np.mean(scores), np.std(scores)
-    txt += '\n- Average CV accuracy over %d epochs (random seed=%s)\n' % (ntrials, cfg.CV_PERFORM[cfg.CV_PERFORM['selected']]['seed'])
-    if cfg.CV_PERFORM[cfg.CV_PERFORM['selected']] in ['LeaveOneOut', 'StratifiedShuffleSplit']:
-        txt += "mean %.3f, std: %.3f\n" % (cv_mean, cv_std)
-    txt += 'Classifier: %s, ' % selected_classifier
-    txt += ', '.join(['%s=%s' % (k, params[k]) for k in params]) + '\n'
-    if cfg.CV['IGNORE_THRES'] is not None:
-        txt += 'Decision threshold: %.2f\n' % cfg.CV['IGNORE_THRES']
-    txt += '\n- Confusion Matrix\n' + cm_txt
-    logger.info(txt)
-
-    # Export to a file
-    if 'export_result' in cfg.CV_PERFORM[selected_cv] and cfg.CV_PERFORM[selected_cv]['export_result'] is True:
-        if cv_file is None:
-            if cfg.EXPORT_CLS is True:
-                qc.make_dirs('%s/classifier' % cfg.DATA_PATH)
-                fout = open('%s/classifier/cv_result.txt' % cfg.DATA_PATH, 'w')
-            else:
-                fout = open('%s/cv_result.txt' % cfg.DATA_PATH, 'w')
-        else:
-            fout = open(cv_file, 'w')
-        fout.write(txt)
-        fout.close()
-
-
-def train_decoder(cfg, featdata, feat_file=None):
-    """
-    Train the final decoder using all data
-    """
-    # Init a classifier
-    selected_classifier = cfg.CLASSIFIER['selected']
-    if selected_classifier not in CLASSIFIERS:
-        logger.error('Unsupported classifier %s' % selected_classifier)
-        raise ValueError
-    params = cfg.CLASSIFIER[selected_classifier]
-    cls = CLASSIFIERS[selected_classifier](**params)
-
-    # Setup features
-    X_data = featdata['X_data']
-    Y_data = featdata['Y_data']
-    wlen = featdata['wlen']
-    if cfg.FEATURES['PSD']['wlen'] is None:
-        cfg.FEATURES['PSD']['wlen'] = wlen
-    w_frames = featdata['w_frames']
-    ch_names = featdata['ch_names']
-    ch_names_raw = featdata['ch_names_raw']
-    X_data_merged = np.concatenate(X_data)
-    Y_data_merged = np.concatenate(Y_data)
-    if cfg.CV['BALANCE_SAMPLES']:
-        X_data_merged, Y_data_merged = balance_samples(X_data_merged, Y_data_merged, cfg.CV['BALANCE_SAMPLES'], verbose=True)
-
-    # Start training the decoder
-    logger.info_green('Training the decoder')
-    timer = qc.Timer()
-    cls.n_jobs = cfg.N_JOBS
-    cls.fit(X_data_merged, Y_data_merged)
-    logger.info('Trained %d samples x %d dimension in %.1f sec' %\
-          (X_data_merged.shape[0], X_data_merged.shape[1], timer.sec()))
-    cls.n_jobs = 1 # always set n_jobs=1 for testing
-
-    # Export the decoder
-    classes = {c:cfg.tdef.by_value[c] for c in np.unique(Y_data)}
-    if cfg.FEATURES['selected'] == 'PSD':
-        data = dict(cls=cls, ch_names=ch_names, ch_names_raw=ch_names_raw, psde=featdata['psde'], sfreq=featdata['sfreq'],
-            picks=featdata['picks'], classes=classes, epochs=cfg.EPOCH, w_frames=w_frames,
-            w_seconds=cfg.FEATURES['PSD']['wlen'], wstep=cfg.FEATURES['PSD']['wstep'], spatial=cfg.SP_FILTER,
-            spatial_ch=featdata['picks'], spectral=cfg.TP_FILTER[cfg.TP_FILTER['selected']], spectral_ch=featdata['picks'],
-            notch=cfg.NOTCH_FILTER[cfg.NOTCH_FILTER['selected']], notch_ch=featdata['picks'], multiplier=cfg.MULTIPLIER,
-            ref_ch=cfg.REREFERENCE[cfg.REREFERENCE['selected']], decim=cfg.FEATURES['PSD']['decim'])
-    clsfile = '%s/classifier/classifier-%s.pkl' % (cfg.DATA_PATH, platform.architecture()[0])
-    qc.make_dirs('%s/classifier' % cfg.DATA_PATH)
-    qc.save_obj(clsfile, data)
-    logger.info('Decoder saved to %s' % clsfile)
-
-    # Reverse-lookup frequency from FFT
-    fq = 0
-    if type(cfg.FEATURES['PSD']['wlen']) == list:
-        fq_res = 1.0 / cfg.FEATURES['PSD']['wlen'][0]
-    else:
-        fq_res = 1.0 / cfg.FEATURES['PSD']['wlen']
-    fqlist = []
-    while fq <= cfg.FEATURES['PSD']['fmax']:
-        if fq >= cfg.FEATURES['PSD']['fmin']:
-            fqlist.append(fq)
-        fq += fq_res
-
-    # Show top distinctive features
-    if cfg.FEATURES['selected'] == 'PSD':
-        logger.info_green('Good features ordered by importance')
-        if selected_classifier in ['RF', 'GB', 'XGB', 'LGB']:
-            keys, values = qc.sort_by_value(list(cls.feature_importances_), rev=True)
-        elif selected_classifier in ['LDA', 'rLDA']:
-            keys, values = qc.sort_by_value(cls.w, rev=True)
-        keys = np.array(keys)
-        values = np.array(values)
-
-        if cfg.EXPORT_GOOD_FEATURES:
-            if feat_file is None:
-                gfout = open('%s/classifier/good_features.txt' % cfg.DATA_PATH, 'w')
-            else:
-                gfout = open(feat_file, 'w')
-
-        if type(wlen) is list:
-            ch_names = []
-            for w in range(len(wlen)):
-                for c in featdata['picks']:
-                    ch_names.append('w%d-%s' % (w, ch_names_raw[c]))
-
-        chlist, hzlist = features.feature2chz(keys, fqlist, ch_names=ch_names)
-        valnorm = values.copy()
-        valsum = np.sum(valnorm)
-        if valsum > 0:
-            valnorm = valnorm / valsum * 100.0
-
-        # show top-N features
-        for i, (ch, hz) in enumerate(zip(chlist, hzlist)):
-            if i >= cfg.FEAT_TOPN:
-                break
-            txt = '%-3s %5.1f Hz  normalized importance %-6s  raw importance %-6s  feature %-5d' %\
-                  (ch, hz, '%.2f%%' % valnorm[i], '%.2f' % values[i], keys[i])
-            logger.info(txt)
-
-        if cfg.EXPORT_GOOD_FEATURES:
-            gfout.write('Importance(%) Channel Frequency Index\n')
-            for i, (ch, hz) in enumerate(zip(chlist, hzlist)):
-                gfout.write('%.3f\t%s\t%s\t%d\n' % (valnorm[i], ch, hz, keys[i]))
-            gfout.close()
-
-
-# for batch scripts
-def batch_run(cfg_module):
-    cfg = pu.load_config(cfg_module)
-    cfg = check_config(cfg)
-    run(cfg, interactive=True)
-
-def run(cfg, interactive=False, cv_file=None, feat_file=None, logger=logger):
-    # add tdef object
-    cfg.tdef = trigger_def(cfg.TRIGGER_FILE)
-
-    # Extract features
-    featdata = features.compute_features(cfg)
-
-    # Find optimal threshold for TPR balancing
-    #balance_tpr(cfg, featdata)
-
-    # Perform cross validation
-    if cfg.CV_PERFORM[cfg.CV_PERFORM['selected']] is not None:
-        cross_validate(cfg, featdata, cv_file=cv_file)
-
-    # Train a decoder
-    if cfg.EXPORT_CLS is True:
-        train_decoder(cfg, featdata, feat_file=feat_file)
-
-def main():
-    """
-    Invoked from console
-    """
-    # Load parameters
-    if len(sys.argv) == 1:
-        print('Usage: %s config_module' % os.path.basename(__file__))
-        return
-
-    cfg_module = sys.argv[1]
-    batch_run(cfg_module)
-    logger.info('Finished.')
-
-if __name__ == '__main__':
-    main()
+from __future__ import print_function, division
+
+"""
+trainer.py
+
+Perform cross-validation and train a classifier.
+See run() to see the overall flow.
+
+When you add more classifiers, modify "CLASSIFIERS" variable to include your classifier.
+
+Kyuhwa Lee, 2018
+Swiss Federal Institute of Technology Lausanne (EPFL)
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+"""
+
+import os
+import sys
+import imp
+import mne
+import mne.io
+import platform
+import numpy as np
+import multiprocessing as mp
+import sklearn.metrics as skmetrics
+import neurodecode.utils.q_common as qc
+import neurodecode.utils.pycnbi_utils as pu
+import neurodecode.decoder.features as features
+from builtins import input
+from sklearn.ensemble import RandomForestClassifier
+from sklearn.ensemble import GradientBoostingClassifier
+from xgboost import XGBClassifier
+from lightgbm import LGBMClassifier
+from sklearn.discriminant_analysis import LinearDiscriminantAnalysis as LDA
+from neurodecode.decoder.rlda import rLDA
+from neurodecode import logger
+from neurodecode.triggers.trigger_def import trigger_def
+
+# supported classifiers: add this part as you add more classifiers
+CLASSIFIERS = {'RF':RandomForestClassifier, 'GB':GradientBoostingClassifier, 'XGB':XGBClassifier,
+    'LGB':LGBMClassifier, 'LDA':LDA, 'rLDA':rLDA}
+
+# scikit-learn old version compatibility
+try:
+    from sklearn.model_selection import StratifiedShuffleSplit, LeaveOneOut
+    SKLEARN_OLD = False
+except ImportError:
+    from sklearn.cross_validation import StratifiedShuffleSplit, LeaveOneOut
+    SKLEARN_OLD = True
+mne.set_log_level('ERROR')
+os.environ['OMP_NUM_THREADS'] = '1' # actually improves performance for multitaper
+
+def check_config(cfg):
+    critical_vars = {
+        'COMMON': ['TRIGGER_FILE',
+                    'TRIGGER_DEF',
+                    'EPOCH',
+                    'DATA_PATH',
+                    'PICKED_CHANNELS',
+                    'SP_FILTER',
+                    'TP_FILTER',
+                    'NOTCH_FILTER',
+                    'FEATURES',
+                    'CLASSIFIER',
+                    'CV_PERFORM'],
+                    'RF': ['n_estimators'],
+                    'GB': ['n_estimators', 'learning_rate'],
+                    'XGB': ['n_estimators', 'learning_rate'],
+                    'LGB': ['n_estimators', 'learning_rate'],
+                    'LDA': [],
+                    'rLDA': ['reg_cov'],
+                    'StratifiedShuffleSplit': ['test_ratio', 'folds', 'seed', 'export_result'],
+                    'LeaveOneOut': ['export_result']
+    }
+
+    # optional variables with default values
+    optional_vars = {
+        'MULTIPLIER': 1,
+        'EXPORT_GOOD_FEATURES': False,
+        'FEAT_TOPN': 10,
+        'EXPORT_CLS': False,
+        'REREFERENCE': None,
+        'N_JOBS': None,
+        'EXCLUDED_CHANNELS': None,
+        'LOAD_EVENTS': None,
+        'CV': {'IGNORE_THRES': None, 'DECISION_THRES': None, 'BALANCE_SAMPLES': False},
+    }
+
+    for v in critical_vars['COMMON']:
+        if not hasattr(cfg, v):
+            logger.error('%s not defined in config.' % v)
+            raise KeyError
+
+    for key in optional_vars:
+        if not hasattr(cfg, key):
+            setattr(cfg, key, optional_vars[key])
+            logger.warning('Setting undefined parameter %s=%s' % (key, getattr(cfg, key)))
+
+    if 'decim' not in cfg.FEATURES['PSD']:
+        cfg.FEATURES['PSD']['decim'] = 1
+
+    # classifier parameters check
+    selected_classifier = cfg.CLASSIFIER['selected']
+    if selected_classifier not in cfg.CLASSIFIER:
+        logger.error('"%s" not defined in your config.' % selected_classifier)
+        raise KeyError
+    for v in critical_vars[selected_classifier]:
+        if v not in cfg.CLASSIFIER[selected_classifier]:
+            logger.error('parameter %s must be defined for %s classifier.' % (v, selected_classifier))
+            raise KeyError
+
+    cv_selected = cfg.CV_PERFORM['selected']
+    if cfg.CV_PERFORM[cv_selected] is not None:
+        if cv_selected not in cfg.CV_PERFORM:
+            logger.error('"%s" not defined in config.' % cv_selected)
+            raise KeyError
+        for v in critical_vars[cv_selected]:
+            if v not in cfg.CV_PERFORM[cv_selected]:
+                logger.error('parameter %s must be defined for %s.' % (v, cv_selected))
+                raise KeyError
+    if cfg.N_JOBS is None:
+        cfg.N_JOBS = mp.cpu_count()
+
+    return cfg
+
+
+def balance_samples(X, Y, balance_type, verbose=False):
+    if balance_type == 'OVER':
+        """
+        Oversample from classes that lack samples
+        """
+        label_set = np.unique(Y)
+        max_set = []
+        X_balanced = np.array(X)
+        Y_balanced = np.array(Y)
+
+        # find a class with maximum number of samples
+        for c in label_set:
+            yl = np.where(Y == c)[0]
+            if len(max_set) == 0 or len(yl) > max_set[1]:
+                max_set = [c, len(yl)]
+        for c in label_set:
+            if c == max_set[0]: continue
+            yl = np.where(Y == c)[0]
+            extra_samples = max_set[1] - len(yl)
+            extra_idx = np.random.choice(yl, extra_samples)
+            X_balanced = np.append(X_balanced, X[extra_idx], axis=0)
+            Y_balanced = np.append(Y_balanced, Y[extra_idx], axis=0)
+    elif balance_type == 'UNDER':
+        """
+        Undersample from classes that are excessive
+        """
+        label_set = np.unique(Y)
+        min_set = []
+
+        # find a class with minimum number of samples
+        for c in label_set:
+            yl = np.where(Y == c)[0]
+            if len(min_set) == 0 or len(yl) < min_set[1]:
+                min_set = [c, len(yl)]
+        yl = np.where(Y == min_set[0])[0]
+        X_balanced = np.array(X[yl])
+        Y_balanced = np.array(Y[yl])
+        for c in label_set:
+            if c == min_set[0]: continue
+            yl = np.where(Y == c)[0]
+            reduced_idx = np.random.choice(yl, min_set[1])
+            X_balanced = np.append(X_balanced, X[reduced_idx], axis=0)
+            Y_balanced = np.append(Y_balanced, Y[reduced_idx], axis=0)
+    elif balance_type is None or balance_type is False:
+        return X, Y
+    else:
+        logger.error('Unknown balancing type %s' % balance_type)
+        raise ValueError
+
+    logger.info_green('\nNumber of samples after %ssampling' % balance_type.lower())
+    for c in label_set:
+        logger.info('%s: %d -> %d' % (c, len(np.where(Y == c)[0]), len(np.where(Y_balanced == c)[0])))
+
+    return X_balanced, Y_balanced
+
+
+def crossval_epochs(cv, epochs_data, labels, cls, label_names=None, do_balance=None, n_jobs=None, ignore_thres=None, decision_thres=None):
+    """
+    Epoch-based cross-validation used by cross_validate().
+
+    Params
+    ======
+    cv: scikit-learn cross-validation object
+    epochs_data: np.array of shape [epochs x samples x features]
+    labels: np.array of shape [epochs x samples]
+    cls: classifier
+    label_names: associated label names {0:'Left', 1:'Right', ...}
+    do_balance: oversample or undersample to match the number of samples among classes
+
+    """
+
+    scores = []
+    f1s = []
+    cnum = 1
+    cm_sum = 0
+    label_set = np.unique(labels)
+    num_labels = len(label_set)
+    if label_names is None:
+        label_names = {l:'%s' % l for l in label_set}
+
+    if n_jobs is None:
+        n_jobs = mp.cpu_count()
+
+    if n_jobs > 1:
+        logger.info('crossval_epochs(): Using %d cores' % n_jobs)
+        pool = mp.Pool(n_jobs)
+        results = []
+
+    # for classifier itself, single core is usually faster
+    cls.n_jobs = 1
+
+    if SKLEARN_OLD:
+        splits = cv
+    else:
+        splits = cv.split(epochs_data, labels[:, 0])
+    for train, test in splits:
+        X_train = np.concatenate(epochs_data[train])
+        X_test = np.concatenate(epochs_data[test])
+        Y_train = np.concatenate(labels[train])
+        Y_test = np.concatenate(labels[test])
+        if do_balance:
+            X_train, Y_train = balance_samples(X_train, Y_train, do_balance)
+            X_test, Y_test = balance_samples(X_test, Y_test, do_balance)
+
+        if n_jobs > 1:
+            results.append(pool.apply_async(fit_predict_thres,
+                                            [cls, X_train, Y_train, X_test, Y_test, cnum, label_set, ignore_thres, decision_thres]))
+        else:
+            score, cm, f1 = fit_predict_thres(cls, X_train, Y_train, X_test, Y_test, cnum, label_set, ignore_thres, decision_thres)
+            scores.append(score)
+            f1s.append(f1)
+            cm_sum += cm
+        cnum += 1
+
+    if n_jobs > 1:
+        pool.close()
+        pool.join()
+
+        for r in results:
+            score, cm, f1 = r.get()
+            scores.append(score)
+            f1s.append(f1)
+            cm_sum += cm
+
+    # confusion matrix
+    cm_sum = cm_sum.astype('float')
+    if cm_sum.shape[0] != cm_sum.shape[1]:
+        # we have decision thresholding condition
+        assert cm_sum.shape[0] < cm_sum.shape[1]
+        cm_sum_all = cm_sum
+        cm_sum = cm_sum[:, :cm_sum.shape[0]]
+        underthres = np.array([r[-1] / sum(r) for r in cm_sum_all])
+    else:
+        underthres = None
+
+    cm_rate = np.zeros(cm_sum.shape)
+    for r_in, r_out in zip(cm_sum, cm_rate):
+        rs = sum(r_in)
+        if rs > 0:
+            r_out[:] = r_in / rs
+        else:
+            assert min(r) == max(r) == 0
+    if underthres is not None:
+        cm_rate = np.concatenate((cm_rate, underthres[:, np.newaxis]), axis=1)
+
+    cm_txt = 'Y: ground-truth, X: predicted\n'
+    max_chars = 12
+    tpl_str = '%%-%ds ' % max_chars
+    tpl_float = '%%-%d.2f ' % max_chars
+    for l in label_set:
+        cm_txt += tpl_str % label_names[l][:max_chars]
+    if underthres is not None:
+        cm_txt += tpl_str % 'Ignored'
+    cm_txt += '\n'
+    for r in cm_rate:
+        for c in r:
+            cm_txt += tpl_float % c
+        cm_txt += '\n'
+    cm_txt += 'Average accuracy: %.2f\n' % np.mean(scores)
+    cm_txt += 'Average F1 score: %.2f\n' % np.mean(f1s)
+
+    return np.array(scores), cm_txt
+
+
+def balance_tpr(cfg, featdata):
+    """
+    Find the threshold of class index 0 that yields equal number of true positive samples of each class.
+    Currently only available for binary classes.
+
+    Params
+    ======
+    cfg: config module
+    feetdata: feature data computed using compute_features()
+    """
+
+    n_jobs = cfg.N_JOBS
+    if n_jobs is None:
+        n_jobs = mp.cpu_count()
+    if n_jobs > 1:
+        logger.info('balance_tpr(): Using %d cores' % n_jobs)
+        pool = mp.Pool(n_jobs)
+        results = []
+
+    # Init a classifier
+    selected_classifier = cfg.CLASSIFIER[cfg.CLASSIFIER['selected']]
+    if selected_classifier not in CLASSIFIERS:
+        logger.error('Unsupported classifier %s' % selected_classifier)
+        raise ValueError
+    params = cfg.CLASSIFIER[selected_classifier]
+    cls = CLASSIFIERS[selected_classifier](**params)
+
+    # Setup features
+    X_data = featdata['X_data']
+    Y_data = featdata['Y_data']
+    wlen = featdata['wlen']
+    if cfg.CLASSIFIER['PSD']['wlen'] is None:
+        cfg.CLASSIFIER['PSD']['wlen'] = wlen
+
+    # Choose CV type
+    ntrials, nsamples, fsize = X_data.shape
+    selected_CV = cfg.CV_PERFORM[cfg.CV_PERFORM['selected']]
+    if cselected_CV == 'LeaveOneOut':
+        logger.info_green('\n%d-fold leave-one-out cross-validation' % ntrials)
+        if SKLEARN_OLD:
+            cv = LeaveOneOut(len(Y_data))
+        else:
+            cv = LeaveOneOut()
+    elif selected_CV == 'StratifiedShuffleSplit':
+        logger.info_green('\n%d-fold stratified cross-validation with test set ratio %.2f' % (cfg.CV_PERFORM[selected_CV]['folds'], cfg.CV_PERFORM[selected_CV]['test_ratio']))
+        if SKLEARN_OLD:
+            cv = StratifiedShuffleSplit(Y_data[:, 0], cfg.CV_PERFORM[selected_CV]['folds'], test_size=cfg.CV_PERFORM[selected_CV]['test_ratio'], random_state=cfg.CV_PERFORM[selected_CV]['random_seed'])
+        else:
+            cv = StratifiedShuffleSplit(n_splits=cfg.CV_PERFORM[selected_CV]['folds'], test_size=cfg.CV_PERFORM[selected_CV]['test_ratio'], random_state=cfg.CV_PERFORM[selected_CV]['random_seed'])
+    else:
+        logger.error('%s is not supported yet. Sorry.' % selected_CV)
+        raise NotImplementedError
+    logger.info('%d trials, %d samples per trial, %d feature dimension' % (ntrials, nsamples, fsize))
+
+    # For classifier itself, single core is usually faster
+    cls.n_jobs = 1
+    Y_preds = []
+
+    if SKLEARN_OLD:
+        splits = cv
+    else:
+        splits = cv.split(X_data, Y_data[:, 0])
+    for cnum, (train, test) in enumerate(splits):
+        X_train = np.concatenate(X_data[train])
+        X_test = np.concatenate(X_data[test])
+        Y_train = np.concatenate(Y_data[train])
+        Y_test = np.concatenate(Y_data[test])
+        if n_jobs > 1:
+            results.append(pool.apply_async(get_predict_proba, [cls, X_train, Y_train, X_test, Y_test, cnum+1]))
+        else:
+            Y_preds.append(get_predict_proba(cls, X_train, Y_train, X_test, Y_test, cnum+1))
+        cnum += 1
+
+    # Aggregate predictions
+    if n_jobs > 1:
+        pool.close()
+        pool.join()
+        for r in results:
+            Y_preds.append(r.get())
+    Y_preds = np.concatenate(Y_preds, axis=0)
+
+    # Find threshold for class index 0
+    Y_preds = sorted(Y_preds)
+    mid_idx = int(len(Y_preds) / 2)
+    if len(Y_preds) == 1:
+        return 0.5 # should not reach here in normal conditions
+    elif len(Y_preds) % 2 == 0:
+        thres = Y_preds[mid_idx-1] + (Y_preds[mid_idx] - Y_preds[mid_idx-1]) / 2
+    else:
+        thres = Y_preds[mid_idx]
+    return thres
+
+
+def cva_features(datadir):
+    """
+    (DEPRECATED FUNCTION)
+    """
+    for fin in qc.get_file_list(datadir, fullpath=True):
+        if fin[-4:] != '.gdf': continue
+        fout = fin + '.cva'
+        if os.path.exists(fout):
+            logger.info('Skipping', fout)
+            continue
+        logger.info("cva_features('%s')" % fin)
+        qc.matlab("cva_features('%s')" % fin)
+
+
+def get_predict_proba(cls, X_train, Y_train, X_test, Y_test, cnum):
+    """
+    All likelihoods will be collected from every fold of a cross-validaiton. Based on these likelihoods,
+    a threshold will be computed that will balance the true positive rate of each class.
+    Available with binary classification scenario only.
+    """
+    timer = qc.Timer()
+    cls.fit(X_train, Y_train)
+    Y_pred = cls.predict_proba(X_test)
+    logger.info('Cross-validation %d (%d tests) - %.1f sec' % (cnum, Y_pred.shape[0], timer.sec()))
+    return Y_pred[:,0]
+
+
+def fit_predict_thres(cls, X_train, Y_train, X_test, Y_test, cnum, label_list, ignore_thres=None, decision_thres=None):
+    """
+    Any likelihood lower than a threshold is not counted as classification score
+    Confusion matrix, accuracy and F1 score (macro average) are computed.
+
+    Params
+    ======
+    ignore_thres:
+    if not None or larger than 0, likelihood values lower than ignore_thres will be ignored
+    while computing confusion matrix.
+
+    """
+    timer = qc.Timer()
+    cls.fit(X_train, Y_train)
+    assert ignore_thres is None or ignore_thres >= 0
+    if ignore_thres is None or ignore_thres == 0:
+        Y_pred = cls.predict(X_test)
+        score = skmetrics.accuracy_score(Y_test, Y_pred)
+        cm = skmetrics.confusion_matrix(Y_test, Y_pred, labels=label_list)
+        f1 = skmetrics.f1_score(Y_test, Y_pred, average='macro')
+    else:
+        if decision_thres is not None:
+            logger.error('decision threshold and ignore_thres cannot be set at the same time.')
+            raise ValueError
+        Y_pred = cls.predict_proba(X_test)
+        Y_pred_labels = np.argmax(Y_pred, axis=1)
+        Y_pred_maxes = np.array([x[i] for i, x in zip(Y_pred_labels, Y_pred)])
+        Y_index_overthres = np.where(Y_pred_maxes >= ignore_thres)[0]
+        Y_index_underthres = np.where(Y_pred_maxes < ignore_thres)[0]
+        Y_pred_overthres = np.array([cls.classes_[x] for x in Y_pred_labels[Y_index_overthres]])
+        Y_pred_underthres = np.array([cls.classes_[x] for x in Y_pred_labels[Y_index_underthres]])
+        Y_pred_underthres_count = np.array([np.count_nonzero(Y_pred_underthres == c) for c in label_list])
+        Y_test_overthres = Y_test[Y_index_overthres]
+        score = skmetrics.accuracy_score(Y_test_overthres, Y_pred_overthres)
+        cm = skmetrics.confusion_matrix(Y_test_overthres, Y_pred_overthres, labels=label_list)
+        cm = np.concatenate((cm, Y_pred_underthres_count[:, np.newaxis]), axis=1)
+        f1 = skmetrics.f1_score(Y_test_overthres, Y_pred_overthres, average='macro')
+
+    logger.info('Cross-validation %d (%.3f) - %.1f sec' % (cnum, score, timer.sec()))
+    return score, cm, f1
+
+
+def cross_validate(cfg, featdata, cv_file=None):
+    """
+    Perform cross validation
+    """
+    # Init a classifier
+    selected_classifier = cfg.CLASSIFIER['selected']
+    if selected_classifier not in CLASSIFIERS:
+        logger.error('Unsupported classifier %s' % selected_classifier)
+        raise ValueError
+    params = cfg.CLASSIFIER[selected_classifier]
+    cls = CLASSIFIERS[selected_classifier](**params)
+
+    # Setup features
+    X_data = featdata['X_data']
+    Y_data = featdata['Y_data']
+    wlen = featdata['wlen']
+
+    # Choose CV type
+    ntrials, nsamples, fsize = X_data.shape
+    selected_cv =  cfg.CV_PERFORM['selected']
+    if selected_cv == 'LeaveOneOut':
+        logger.info_green('%d-fold leave-one-out cross-validation' % ntrials)
+        if SKLEARN_OLD:
+            cv = LeaveOneOut(len(Y_data))
+        else:
+            cv = LeaveOneOut()
+    elif selected_cv == 'StratifiedShuffleSplit':
+        logger.info_green('%d-fold stratified cross-validation with test set ratio %.2f' % (cfg.CV_PERFORM[selected_cv]['folds'], cfg.CV_PERFORM[selected_cv]['test_ratio']))
+        if SKLEARN_OLD:
+            cv = StratifiedShuffleSplit(Y_data[:, 0], cfg.CV_PERFORM[selected_cv]['folds'], test_size=cfg.CV_PERFORM[selected_cv]['test_ratio'], random_state=cfg.CV_PERFORM[selected_cv]['seed'])
+        else:
+            cv = StratifiedShuffleSplit(n_splits=cfg.CV_PERFORM[selected_cv]['folds'], test_size=cfg.CV_PERFORM[selected_cv]['test_ratio'], random_state=cfg.CV_PERFORM[selected_cv]['seed'])
+    else:
+        logger.error('%s is not supported yet. Sorry.' % cfg.CV_PERFORM[cfg.CV_PERFORM['selected']])
+        raise NotImplementedError
+    logger.info('%d trials, %d samples per trial, %d feature dimension' % (ntrials, nsamples, fsize))
+
+    # Do it!
+    timer_cv = qc.Timer()
+    scores, cm_txt = crossval_epochs(cv, X_data, Y_data, cls, cfg.tdef.by_value, cfg.CV['BALANCE_SAMPLES'], n_jobs=cfg.N_JOBS,
+                                     ignore_thres=cfg.CV['IGNORE_THRES'], decision_thres=cfg.CV['DECISION_THRES'])
+    t_cv = timer_cv.sec()
+
+    # Export results
+    txt = 'Cross validation took %d seconds.\n' % t_cv
+    txt += '\n- Class information\n'
+    txt += '%d epochs, %d samples per epoch, %d feature dimension (total %d samples)\n' %\
+        (ntrials, nsamples, fsize, ntrials * nsamples)
+    for ev in np.unique(Y_data):
+        txt += '%s: %d trials\n' % (cfg.tdef.by_value[ev], len(np.where(Y_data[:, 0] == ev)[0]))
+    if cfg.CV['BALANCE_SAMPLES']:
+        txt += 'The number of samples was balanced using %ssampling.\n' % cfg.BALANCE_SAMPLES.lower()
+    txt += '\n- Experiment condition\n'
+    txt += 'Sampling frequency: %.3f Hz\n' % featdata['sfreq']
+    txt += 'Spatial filter: %s\n' % cfg.SP_FILTER
+    txt += 'Spectral filter: %s\n' % cfg.TP_FILTER[cfg.TP_FILTER['selected']]
+    txt += 'Notch filter: %s\n' % cfg.NOTCH_FILTER[cfg.NOTCH_FILTER['selected']]
+    #txt += 'Channels: ' + ','.join([str(featdata['ch_names'][p]) for p in featdata['picks']]) + '\n'
+    txt += 'Channels: %s\n' % featdata['ch_names']
+    txt += 'PSD range: %.1f - %.1f Hz\n' % (cfg.FEATURES['PSD']['fmin'], cfg.FEATURES['PSD']['fmax'])
+    txt += 'Window step: %.2f msec\n' % (1000.0 * cfg.FEATURES['PSD']['wstep'] / featdata['sfreq'])
+    if type(wlen) is list:
+        for i, w in enumerate(wlen):
+            txt += 'Window size: %.1f msec\n' % (w * 1000.0)
+            txt += 'Epoch range: %s sec\n' % (cfg.EPOCH[i])
+    else:
+        txt += 'Window size: %.1f msec\n' % (cfg.FEATURES['PSD']['wlen'] * 1000.0)
+        txt += 'Epoch range: %s sec\n' % (cfg.EPOCH)
+    txt += 'Decimation factor: %d\n' % cfg.FEATURES['PSD']['decim']
+
+    # Compute stats
+    cv_mean, cv_std = np.mean(scores), np.std(scores)
+    txt += '\n- Average CV accuracy over %d epochs (random seed=%s)\n' % (ntrials, cfg.CV_PERFORM[cfg.CV_PERFORM['selected']]['seed'])
+    if cfg.CV_PERFORM[cfg.CV_PERFORM['selected']] in ['LeaveOneOut', 'StratifiedShuffleSplit']:
+        txt += "mean %.3f, std: %.3f\n" % (cv_mean, cv_std)
+    txt += 'Classifier: %s, ' % selected_classifier
+    txt += ', '.join(['%s=%s' % (k, params[k]) for k in params]) + '\n'
+    if cfg.CV['IGNORE_THRES'] is not None:
+        txt += 'Decision threshold: %.2f\n' % cfg.CV['IGNORE_THRES']
+    txt += '\n- Confusion Matrix\n' + cm_txt
+    logger.info(txt)
+
+    # Export to a file
+    if 'export_result' in cfg.CV_PERFORM[selected_cv] and cfg.CV_PERFORM[selected_cv]['export_result'] is True:
+        if cv_file is None:
+            if cfg.EXPORT_CLS is True:
+                qc.make_dirs('%s/classifier' % cfg.DATA_PATH)
+                fout = open('%s/classifier/cv_result.txt' % cfg.DATA_PATH, 'w')
+            else:
+                fout = open('%s/cv_result.txt' % cfg.DATA_PATH, 'w')
+        else:
+            fout = open(cv_file, 'w')
+        fout.write(txt)
+        fout.close()
+
+
+def train_decoder(cfg, featdata, feat_file=None):
+    """
+    Train the final decoder using all data
+    """
+    # Init a classifier
+    selected_classifier = cfg.CLASSIFIER['selected']
+    if selected_classifier not in CLASSIFIERS:
+        logger.error('Unsupported classifier %s' % selected_classifier)
+        raise ValueError
+    params = cfg.CLASSIFIER[selected_classifier]
+    cls = CLASSIFIERS[selected_classifier](**params)
+
+    # Setup features
+    X_data = featdata['X_data']
+    Y_data = featdata['Y_data']
+    wlen = featdata['wlen']
+    if cfg.FEATURES['PSD']['wlen'] is None:
+        cfg.FEATURES['PSD']['wlen'] = wlen
+    w_frames = featdata['w_frames']
+    ch_names = featdata['ch_names']
+    ch_names_raw = featdata['ch_names_raw']
+    X_data_merged = np.concatenate(X_data)
+    Y_data_merged = np.concatenate(Y_data)
+    if cfg.CV['BALANCE_SAMPLES']:
+        X_data_merged, Y_data_merged = balance_samples(X_data_merged, Y_data_merged, cfg.CV['BALANCE_SAMPLES'], verbose=True)
+
+    # Start training the decoder
+    logger.info_green('Training the decoder')
+    timer = qc.Timer()
+    cls.n_jobs = cfg.N_JOBS
+    cls.fit(X_data_merged, Y_data_merged)
+    logger.info('Trained %d samples x %d dimension in %.1f sec' %\
+          (X_data_merged.shape[0], X_data_merged.shape[1], timer.sec()))
+    cls.n_jobs = 1 # always set n_jobs=1 for testing
+
+    # Export the decoder
+    classes = {c:cfg.tdef.by_value[c] for c in np.unique(Y_data)}
+    if cfg.FEATURES['selected'] == 'PSD':
+        data = dict(cls=cls, ch_names=ch_names, ch_names_raw=ch_names_raw, psde=featdata['psde'], sfreq=featdata['sfreq'],
+            picks=featdata['picks'], classes=classes, epochs=cfg.EPOCH, w_frames=w_frames,
+            w_seconds=cfg.FEATURES['PSD']['wlen'], wstep=cfg.FEATURES['PSD']['wstep'], spatial=cfg.SP_FILTER,
+            spatial_ch=featdata['picks'], spectral=cfg.TP_FILTER[cfg.TP_FILTER['selected']], spectral_ch=featdata['picks'],
+            notch=cfg.NOTCH_FILTER[cfg.NOTCH_FILTER['selected']], notch_ch=featdata['picks'], multiplier=cfg.MULTIPLIER,
+            ref_ch=cfg.REREFERENCE[cfg.REREFERENCE['selected']], decim=cfg.FEATURES['PSD']['decim'])
+    clsfile = '%s/classifier/classifier-%s.pkl' % (cfg.DATA_PATH, platform.architecture()[0])
+    qc.make_dirs('%s/classifier' % cfg.DATA_PATH)
+    qc.save_obj(clsfile, data)
+    logger.info('Decoder saved to %s' % clsfile)
+
+    # Reverse-lookup frequency from FFT
+    fq = 0
+    if type(cfg.FEATURES['PSD']['wlen']) == list:
+        fq_res = 1.0 / cfg.FEATURES['PSD']['wlen'][0]
+    else:
+        fq_res = 1.0 / cfg.FEATURES['PSD']['wlen']
+    fqlist = []
+    while fq <= cfg.FEATURES['PSD']['fmax']:
+        if fq >= cfg.FEATURES['PSD']['fmin']:
+            fqlist.append(fq)
+        fq += fq_res
+
+    # Show top distinctive features
+    if cfg.FEATURES['selected'] == 'PSD':
+        logger.info_green('Good features ordered by importance')
+        if selected_classifier in ['RF', 'GB', 'XGB', 'LGB']:
+            keys, values = qc.sort_by_value(list(cls.feature_importances_), rev=True)
+        elif selected_classifier in ['LDA', 'rLDA']:
+            keys, values = qc.sort_by_value(cls.w, rev=True)
+        keys = np.array(keys)
+        values = np.array(values)
+
+        if cfg.EXPORT_GOOD_FEATURES:
+            if feat_file is None:
+                gfout = open('%s/classifier/good_features.txt' % cfg.DATA_PATH, 'w')
+            else:
+                gfout = open(feat_file, 'w')
+
+        if type(wlen) is list:
+            ch_names = []
+            for w in range(len(wlen)):
+                for c in featdata['picks']:
+                    ch_names.append('w%d-%s' % (w, ch_names_raw[c]))
+
+        chlist, hzlist = features.feature2chz(keys, fqlist, ch_names=ch_names)
+        valnorm = values.copy()
+        valsum = np.sum(valnorm)
+        if valsum > 0:
+            valnorm = valnorm / valsum * 100.0
+
+        # show top-N features
+        for i, (ch, hz) in enumerate(zip(chlist, hzlist)):
+            if i >= cfg.FEAT_TOPN:
+                break
+            txt = '%-3s %5.1f Hz  normalized importance %-6s  raw importance %-6s  feature %-5d' %\
+                  (ch, hz, '%.2f%%' % valnorm[i], '%.2f' % values[i], keys[i])
+            logger.info(txt)
+
+        if cfg.EXPORT_GOOD_FEATURES:
+            gfout.write('Importance(%) Channel Frequency Index\n')
+            for i, (ch, hz) in enumerate(zip(chlist, hzlist)):
+                gfout.write('%.3f\t%s\t%s\t%d\n' % (valnorm[i], ch, hz, keys[i]))
+            gfout.close()
+
+
+# for batch scripts
+def batch_run(cfg_module):
+    cfg = pu.load_config(cfg_module)
+    cfg = check_config(cfg)
+    run(cfg, interactive=True)
+
+def run(cfg, interactive=False, cv_file=None, feat_file=None, logger=logger):
+    # add tdef object
+    cfg.tdef = trigger_def(cfg.TRIGGER_FILE)
+
+    # Extract features
+    featdata = features.compute_features(cfg)
+
+    # Find optimal threshold for TPR balancing
+    #balance_tpr(cfg, featdata)
+
+    # Perform cross validation
+    if cfg.CV_PERFORM[cfg.CV_PERFORM['selected']] is not None:
+        cross_validate(cfg, featdata, cv_file=cv_file)
+
+    # Train a decoder
+    if cfg.EXPORT_CLS is True:
+        train_decoder(cfg, featdata, feat_file=feat_file)
+
+def main():
+    """
+    Invoked from console
+    """
+    # Load parameters
+    if len(sys.argv) == 1:
+        print('Usage: %s config_module' % os.path.basename(__file__))
+        return
+
+    cfg_module = sys.argv[1]
+    batch_run(cfg_module)
+    logger.info('Finished.')
+
+if __name__ == '__main__':
+    main()
```

### Comparing `neurodecode-2.0.4/neurodecode/glass/bgi_client.py` & `neurodecode-2.0.5/neurodecode/glass/bgi_client.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-from __future__ import print_function, division
-
-"""
-Brain-Glass Interface
-
-Controls the visual feedback on Google Glass.
-When connected with USB cable, connect to the local loopback network (127.0.0.1).
-adb executable must be in the system's PATH environment variable.
-
-
-Kyuhwa Lee, 2018
-Swiss Federal Institute of Technology (EPFL)
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""
-
-import socket
-import time
-import os
-import sys
-import neurodecode.utils.q_common as qc
-
-
-class GlassControl(object):
-    """
-    Controls Glass UI
-
-    Constructor:
-        mock: set to False if you don't have a Glass.
-
-    """
-
-    def __init__(self, mock=False):
-        self.BUFFER_SIZE = 1024
-        self.last_dir = 'L'
-        self.timer = qc.Timer(autoreset=True)
-        self.mock = mock
-        if self.mock:
-            self.print('Using a fake, mock Glass control object.')
-
-    def print(self, *args):
-        if len(args) > 0: print('[GlassControl] ', end='')
-        print(*args)
-
-    def connect(self, ip, port):
-        if self.mock: return
-        self.ip = ip
-        self.port = port
-
-        # Networking via USB if IP=127.0.0.1
-        if ip == '127.0.0.1':
-            exe = 'adb forward tcp:%d tcp:%d' % (port, port)
-            self.print(exe)
-            os.system(exe)
-            time.sleep(0.2)
-        self.print('Connecting to %s:%d' % (ip, port))
-        try:
-            self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            self.socket.connect((self.ip, self.port))
-        except:
-            self.print('* ERROR connecting to Glass. The error was:')
-            self.print(sys.exc_info()[0], sys.exc_info()[1])
-            sys.exit(-1)
-
-    def disconnect(self):
-        if self.mock: return
-        self.print('Disconnecting from Glass')
-        self.socket.close()
-
-    def send_byte(self, msg):
-        if sys.version_info.major >= 3:
-            self.socket.sendall(bytes(msg + '\n', "UTF-8"))
-        else:
-            self.socket.sendall(bytes(unicode(msg + '\n')))
-
-    def send_msg(self, msg, wait=True):
-        """
-        Send a message to the Glass
-
-        Glass requires some delay after when the last command was sent.
-        This function will be blocked until minimum this delay is satisfied.
-        Set wait=False to force sending message, but the msg is likely to be ignored.
-
-        """
-        if wait:
-            # Wait only if the time hasn't passed enough
-            self.timer.sleep_atleast(0.033)  # 30 Hz
-        if self.mock:
-            return
-        try:
-            self.send_byte(msg)
-        except Exception as e:
-            self.print('* ERROR: Glass communication failed! Attempting to reconnect again.')
-            self.disconnect()
-            time.sleep(2)
-            # Let's try again
-            self.connect(self.ip, self.port)
-            try:
-                self.send_byte(msg)
-            except Exception as e:
-                self.print('Sorry, cannot fix the problem. I give up.')
-                raise Exception(e)
-
-    # Show empty bars
-    def clear(self):
-        if self.mock: return
-        self.send_msg('C')
-
-    # Show empty bars
-    def draw_cross(self):
-        if self.mock: return
-        self.clear()
-
-    # Only one direction at a time
-    def move_bar(self, new_dir, amount, overlay=False):
-        if self.mock: return
-        if overlay is False and self.last_dir != new_dir:
-            self.send_msg('%s0' % self.last_dir)
-        self.send_msg('%s%d' % (new_dir, amount))
-        self.last_dir = new_dir
-
-    # Fill screen with a solid color (None, 'R','G','B')
-    def fill(self, color=None):
-        if self.mock: return
-        if color is None:
-            self.send_msg('F0')
-        elif color == 'R':
-            self.send_msg('F1')
-        elif color == 'G':
-            self.send_msg('F2')
-        elif color == 'B':
-            self.send_msg('F3')
-        elif color == 'K':
-            self.send_msg('F4')
-
-    def fullbar_color(self, color):
-        if color not in ['R', 'G', 'B', 'Y']:
-            print('**** UNSUPPORTED GLASS BAR COLOR ****')
-        else:
-            msg = 'B' + color[0]
-            # print('*** GLASS SENDING', msg)
-            self.send_msg(msg)
-
-
-# Test code
-if __name__ == '__main__':
-    step = 5
-
-    ui = GlassControl()
-    ui.connect('127.0.0.1', 59900)
-    ui.clear()
-
-    for x in range(10):
-        print('L move')
-        for x in range(0, 101, step):
-            ui.move_bar('L', x)
-        time.sleep(0.2)
-
-        print('R move')
-        for x in range(0, 101, step):
-            ui.move_bar('R', x)
-        time.sleep(0.2)
-
-        print('U move')
-        for x in range(0, 101, step):
-            ui.move_bar('U', x)
-        time.sleep(0.2)
-
-        print('D move')
-        for x in range(0, 101, step):
-            ui.move_bar('D', x)
-        time.sleep(0.2)
-
-    ui.clear()
-    ui.disconnect()
+from __future__ import print_function, division
+
+"""
+Brain-Glass Interface
+
+Controls the visual feedback on Google Glass.
+When connected with USB cable, connect to the local loopback network (127.0.0.1).
+adb executable must be in the system's PATH environment variable.
+
+
+Kyuhwa Lee, 2018
+Swiss Federal Institute of Technology (EPFL)
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+"""
+
+import socket
+import time
+import os
+import sys
+import neurodecode.utils.q_common as qc
+
+
+class GlassControl(object):
+    """
+    Controls Glass UI
+
+    Constructor:
+        mock: set to False if you don't have a Glass.
+
+    """
+
+    def __init__(self, mock=False):
+        self.BUFFER_SIZE = 1024
+        self.last_dir = 'L'
+        self.timer = qc.Timer(autoreset=True)
+        self.mock = mock
+        if self.mock:
+            self.print('Using a fake, mock Glass control object.')
+
+    def print(self, *args):
+        if len(args) > 0: print('[GlassControl] ', end='')
+        print(*args)
+
+    def connect(self, ip, port):
+        if self.mock: return
+        self.ip = ip
+        self.port = port
+
+        # Networking via USB if IP=127.0.0.1
+        if ip == '127.0.0.1':
+            exe = 'adb forward tcp:%d tcp:%d' % (port, port)
+            self.print(exe)
+            os.system(exe)
+            time.sleep(0.2)
+        self.print('Connecting to %s:%d' % (ip, port))
+        try:
+            self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            self.socket.connect((self.ip, self.port))
+        except:
+            self.print('* ERROR connecting to Glass. The error was:')
+            self.print(sys.exc_info()[0], sys.exc_info()[1])
+            sys.exit(-1)
+
+    def disconnect(self):
+        if self.mock: return
+        self.print('Disconnecting from Glass')
+        self.socket.close()
+
+    def send_byte(self, msg):
+        if sys.version_info.major >= 3:
+            self.socket.sendall(bytes(msg + '\n', "UTF-8"))
+        else:
+            self.socket.sendall(bytes(unicode(msg + '\n')))
+
+    def send_msg(self, msg, wait=True):
+        """
+        Send a message to the Glass
+
+        Glass requires some delay after when the last command was sent.
+        This function will be blocked until minimum this delay is satisfied.
+        Set wait=False to force sending message, but the msg is likely to be ignored.
+
+        """
+        if wait:
+            # Wait only if the time hasn't passed enough
+            self.timer.sleep_atleast(0.033)  # 30 Hz
+        if self.mock:
+            return
+        try:
+            self.send_byte(msg)
+        except Exception as e:
+            self.print('* ERROR: Glass communication failed! Attempting to reconnect again.')
+            self.disconnect()
+            time.sleep(2)
+            # Let's try again
+            self.connect(self.ip, self.port)
+            try:
+                self.send_byte(msg)
+            except Exception as e:
+                self.print('Sorry, cannot fix the problem. I give up.')
+                raise Exception(e)
+
+    # Show empty bars
+    def clear(self):
+        if self.mock: return
+        self.send_msg('C')
+
+    # Show empty bars
+    def draw_cross(self):
+        if self.mock: return
+        self.clear()
+
+    # Only one direction at a time
+    def move_bar(self, new_dir, amount, overlay=False):
+        if self.mock: return
+        if overlay is False and self.last_dir != new_dir:
+            self.send_msg('%s0' % self.last_dir)
+        self.send_msg('%s%d' % (new_dir, amount))
+        self.last_dir = new_dir
+
+    # Fill screen with a solid color (None, 'R','G','B')
+    def fill(self, color=None):
+        if self.mock: return
+        if color is None:
+            self.send_msg('F0')
+        elif color == 'R':
+            self.send_msg('F1')
+        elif color == 'G':
+            self.send_msg('F2')
+        elif color == 'B':
+            self.send_msg('F3')
+        elif color == 'K':
+            self.send_msg('F4')
+
+    def fullbar_color(self, color):
+        if color not in ['R', 'G', 'B', 'Y']:
+            print('**** UNSUPPORTED GLASS BAR COLOR ****')
+        else:
+            msg = 'B' + color[0]
+            # print('*** GLASS SENDING', msg)
+            self.send_msg(msg)
+
+
+# Test code
+if __name__ == '__main__':
+    step = 5
+
+    ui = GlassControl()
+    ui.connect('127.0.0.1', 59900)
+    ui.clear()
+
+    for x in range(10):
+        print('L move')
+        for x in range(0, 101, step):
+            ui.move_bar('L', x)
+        time.sleep(0.2)
+
+        print('R move')
+        for x in range(0, 101, step):
+            ui.move_bar('R', x)
+        time.sleep(0.2)
+
+        print('U move')
+        for x in range(0, 101, step):
+            ui.move_bar('U', x)
+        time.sleep(0.2)
+
+        print('D move')
+        for x in range(0, 101, step):
+            ui.move_bar('D', x)
+        time.sleep(0.2)
+
+    ui.clear()
+    ui.disconnect()
```

### Comparing `neurodecode-2.0.4/neurodecode/protocols/feedback.py` & `neurodecode-2.0.5/neurodecode/protocols/feedback.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,443 +1,443 @@
-from __future__ import print_function, division
-
-"""
-Visual feedback with online decoding
-
-Kyuhwa Lee
-Swiss Federal Institute of Technology Lausanne (EPFL)
-
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""
-
-import neurodecode
-import cv2
-import os
-import neurodecode.utils.q_common as qc
-import numpy as np
-import time
-import serial
-import serial.tools.list_ports
-from neurodecode import logger
-
-# global constants
-KEYS = {'right':2555904, 'up':2490368, 'left':2424832, 'down':2621440, 'pgup':85, 'pgdn':86, 'home':80, 'end':87, 'space':32, 'esc':27}
-ARROW_KEYS = {KEYS['left']:'L', KEYS['right']:'R', KEYS['up']:'U', KEYS['down']:'D'}
-COLORS = dict(G=(20, 140, 0), B=(210, 0, 0), R=(0, 50, 200), Y=(0, 215, 235), K=(0, 0, 0), W=(255, 255, 255), w=(200, 200, 200))
-DIRS = {'L':'LEFT', 'R':'RIGHT', 'U':'UP', 'D':'DOWN', 'B':'BOTH'}
-BIAS_INCREMENT = 0.025
-
-class Feedback:
-    """
-    Perform a classification with visual feedback
-    """
-
-    def __init__(self, cfg, viz, tdef, trigger, logfile=None):
-        self.cfg = cfg
-        self.tdef = tdef
-        self.trigger = trigger
-        self.viz = viz
-        self.viz.fill()
-        self.refresh_delay = 1.0 / self.cfg.REFRESH_RATE
-        self.bar_step_left = self.cfg.BAR_STEP['left']
-        self.bar_step_right = self.cfg.BAR_STEP['right']
-        self.bar_step_up = self.cfg.BAR_STEP['up']
-        self.bar_step_down = self.cfg.BAR_STEP['down']
-        self.bar_step_both = self.cfg.BAR_STEP['both']
-
-        if type(self.cfg.BAR_BIAS) is tuple:
-            self.bar_bias = list(self.cfg.BAR_BIAS)
-        else:
-            self.bar_bias = self.cfg.BAR_BIAS
-
-        # New decoder: already smoothed by the decoder so bias after.
-        #self.alpha_old = self.cfg.PROB_ACC_ALPHA
-        #self.alpha_new = 1.0 - self.cfg.PROB_ACC_ALPHA
-
-        if hasattr(self.cfg, 'BAR_REACH_FINISH') and self.cfg.BAR_REACH_FINISH == True:
-            self.premature_end = True
-        else:
-            self.premature_end = False
-
-        self.tm_trigger = qc.Timer()
-        self.tm_display = qc.Timer()
-        self.tm_watchdog = qc.Timer()
-        if logfile is not None:
-            self.logf = open(logfile, 'w')
-        else:
-            self.logf = None
-
-        # STIMO only
-        if self.cfg.WITH_STIMO is True:
-            if self.cfg.STIMO_COMPORT is None:
-                atens = [x for x in serial.tools.list_ports.grep('ATEN')]
-                if len(atens) == 0:
-                    raise RuntimeError('No ATEN device found. Stop.')
-                try:
-                    self.stimo_port = atens[0].device
-                except AttributeError: # depends on Python distribution
-                    self.stimo_port = atens[0][0]
-            else:
-                self.stimo_port = self.cfg.STIMO_COMPORT
-            self.ser = serial.Serial(self.stimo_port, self.cfg.STIMO_BAUDRATE)
-            logger.info('STIMO serial port %s is_open = %s' % (self.stimo_port, self.ser.is_open))
-
-    def __del__(self):
-        # STIMO only
-        if self.cfg.WITH_STIMO is True:
-            self.ser.close()
-            logger.info('Closed STIMO serial port %s' % self.stimo_port)
-
-    def classify(self, decoder, true_label, title_text, bar_dirs, state='start', prob_history=None):
-        """
-        Run a single trial
-        """
-        true_label_index = bar_dirs.index(true_label)
-        self.tm_trigger.reset()
-        if self.bar_bias is not None:
-            bias_idx = bar_dirs.index(self.bar_bias[0])
-
-        if self.logf is not None:
-            self.logf.write('True label: %s\n' % true_label)
-
-        tm_classify = qc.Timer(autoreset=True)
-        self.stimo_timer = qc.Timer()
-        while True:
-            self.tm_display.sleep_atleast(self.refresh_delay)
-            self.tm_display.reset()
-            if state == 'start' and self.tm_trigger.sec() > self.cfg.TIMINGS['INIT']:
-                state = 'gap_s'
-                if self.cfg.TRIALS_PAUSE:
-                    self.viz.put_text('Press any key')
-                    self.viz.update()
-                    key = cv2.waitKeyEx()
-                    if key == KEYS['esc']:
-                        return
-                self.viz.fill()
-                self.tm_trigger.reset()
-                self.trigger.signal(self.tdef.INIT)
-
-            elif state == 'gap_s':
-                if self.cfg.TIMINGS['GAP'] > 0:
-                    self.viz.put_text(title_text)
-                state = 'gap'
-                self.tm_trigger.reset()
-
-            elif state == 'gap' and self.tm_trigger.sec() > self.cfg.TIMINGS['GAP']:
-                state = 'cue'
-                self.viz.fill()
-                self.viz.draw_cue()
-                self.viz.glass_draw_cue()
-                self.trigger.signal(self.tdef.CUE)
-                self.tm_trigger.reset()
-
-            elif state == 'cue' and self.tm_trigger.sec() > self.cfg.TIMINGS['READY']:
-                state = 'dir_r'
-
-                if self.cfg.SHOW_CUE is True:
-                    if self.cfg.FEEDBACK_TYPE == 'BAR':
-                        self.viz.move(true_label, 100, overlay=False, barcolor='G')
-                    elif self.cfg.FEEDBACK_TYPE == 'IMAGE':
-                        self.viz.put_text(DIRS[true_label], 'R')
-                    if true_label == 'L':  # left
-                        self.trigger.signal(self.tdef.LEFT_READY)
-                    elif true_label == 'R':  # right
-                        self.trigger.signal(self.tdef.RIGHT_READY)
-                    elif true_label == 'U':  # up
-                        self.trigger.signal(self.tdef.UP_READY)
-                    elif true_label == 'D':  # down
-                        self.trigger.signal(self.tdef.DOWN_READY)
-                    elif true_label == 'B':  # both hands
-                        self.trigger.signal(self.tdef.BOTH_READY)
-                    else:
-                        raise RuntimeError('Unknown direction %s' % true_label)
-                self.tm_trigger.reset()
-                '''
-                if self.cfg.FEEDBACK_TYPE == 'IMAGE':
-                    self.viz.set_pc_feedback(False)
-                self.viz.move(true_label, 100, overlay=False, barcolor='G')
-
-                if self.cfg.FEEDBACK_TYPE == 'IMAGE':
-                    self.viz.set_pc_feedback(True)
-                    if self.cfg.SHOW_CUE is True:
-                        self.viz.put_text(dirs[true_label], 'R')
-
-                if true_label == 'L':  # left
-                    self.trigger.signal(self.tdef.LEFREADY)
-                elif true_label == 'R':  # right
-                    self.trigger.signal(self.tdef.RIGHT_READY)
-                elif true_label == 'U':  # up
-                    self.trigger.signal(self.tdef.UP_READY)
-                elif true_label == 'D':  # down
-                    self.trigger.signal(self.tdef.DOWN_READY)
-                elif true_label == 'B':  # both hands
-                    self.trigger.signal(self.tdef.BOTH_READY)
-                else:
-                    raise RuntimeError('Unknown direction %s' % true_label)
-                self.tm_trigger.reset()
-                '''
-            elif state == 'dir_r' and self.tm_trigger.sec() > self.cfg.TIMINGS['DIR_CUE']:
-                self.viz.fill()
-                self.viz.draw_cue()
-                self.viz.glass_draw_cue()
-                state = 'dir'
-
-                # initialize bar scores
-                bar_label = bar_dirs[0]
-                bar_score = 0
-                probs = [1.0 / len(bar_dirs)] * len(bar_dirs)
-                self.viz.move(bar_label, bar_score, overlay=False)
-                probs_acc = np.zeros(len(probs))
-
-                if true_label == 'L':  # left
-                    self.trigger.signal(self.tdef.LEFT_GO)
-                elif true_label == 'R':  # right
-                    self.trigger.signal(self.tdef.RIGHT_GO)
-                elif true_label == 'U':  # up
-                    self.trigger.signal(self.tdef.UP_GO)
-                elif true_label == 'D':  # down
-                    self.trigger.signal(self.tdef.DOWN_GO)
-                elif true_label == 'B':  # both
-                    self.trigger.signal(self.tdef.BOTH_GO)
-                else:
-                    raise RuntimeError('Unknown truedirection %s' % true_label)
-
-                self.tm_watchdog.reset()
-                self.tm_trigger.reset()
-
-            elif state == 'dir':
-                if self.tm_trigger.sec() > self.cfg.TIMINGS['CLASSIFY'] or (self.premature_end and bar_score >= 100):
-                    if not hasattr(self.cfg, 'SHOW_RESULT') or self.cfg.SHOW_RESULT is True:
-                        # show classfication result
-                        if self.cfg.WITH_STIMO is True:
-                            if self.cfg.STIMO_FULLGAIT_CYCLE is not None and bar_label == 'U':
-                                res_color = 'G'
-                            elif self.cfg.TRIALS_RETRY is False or bar_label == true_label:
-                                res_color = 'G'
-                            else:
-                                res_color = 'Y'
-                        else:
-                            res_color = 'Y'
-                        if self.cfg.FEEDBACK_TYPE == 'IMAGE':
-                            self.viz.move(bar_label, bar_score, overlay=False, barcolor=res_color, caption=DIRS[bar_label], caption_color=res_color)
-                        else:
-                            self.viz.move(bar_label, 100, overlay=False, barcolor=res_color)
-                    else:
-                        res_color = 'Y'
-                        if self.cfg.FEEDBACK_TYPE == 'IMAGE':
-                            self.viz.move(bar_label, bar_score, overlay=False, barcolor=res_color, caption='TRIAL END', caption_color=res_color)
-                        else:
-                            self.viz.move(bar_label, 0, overlay=False, barcolor=res_color)
-                    self.trigger.signal(self.tdef.FEEDBACK)
-
-                    # STIMO
-                    if self.cfg.WITH_STIMO is True and self.cfg.STIMO_CONTINUOUS is False:
-                        if self.cfg.STIMO_FULLGAIT_CYCLE is not None:
-                            if bar_label == 'U':
-                                self.ser.write(self.cfg.STIMO_FULLGAIT_PATTERN[0])
-                                logger.info('STIMO: Sent 1')
-                                time.sleep(self.cfg.STIMO_FULLGAIT_CYCLE)
-                                self.ser.write(self.cfg.STIMO_FULLGAIT_PATTERN[1])
-                                logger.info('STIMO: Sent 2')
-                                time.sleep(self.cfg.STIMO_FULLGAIT_CYCLE)
-                        elif self.cfg.TRIALS_RETRY is False or bar_label == true_label:
-                            if bar_label == 'L':
-                                self.ser.write(b'1')
-                                logger.info('STIMO: Sent 1')
-                            elif bar_label == 'R':
-                                self.ser.write(b'2')
-                                logger.info('STIMO: Sent 2')
-
-                    if self.cfg.DEBUG_PROBS:
-                        msg = 'DEBUG: Accumulated probabilities = %s' % qc.list2string(probs_acc, '%.3f')
-                        logger.info(msg)
-                        if self.logf is not None:
-                            self.logf.write(msg + '\n')
-                    if self.logf is not None:
-                        self.logf.write('%s detected as %s (%d)\n\n' % (true_label, bar_label, bar_score))
-                        self.logf.flush()
-
-                    # end of trial
-                    state = 'feedback'
-                    self.tm_trigger.reset()
-                else:
-                    # classify
-                    probs_new = decoder.get_prob_smooth_unread()
-                    if probs_new is None:
-                        if self.tm_watchdog.sec() > 3:
-                            logger.warning('No classification being done. Are you receiving data streams?')
-                            self.tm_watchdog.reset()
-                    else:
-                        self.tm_watchdog.reset()
-
-                        if prob_history is not None:
-                            prob_history[true_label].append(probs_new[true_label_index])
-
-                        probs_acc += np.array(probs_new)
-
-                        '''
-                        New decoder: already smoothed by the decoder so bias after.
-                        '''
-                        probs = list(probs_new)
-                        if self.bar_bias is not None:
-                            probs[bias_idx] += self.bar_bias[1]
-                            newsum = sum(probs)
-                            probs = [p / newsum for p in probs]
-
-                        '''
-                        # Method 2: bias and smoothen
-                        if self.bar_bias is not None:
-                            # print('BEFORE: %.3f %.3f'% (probs_new[0], probs_new[1]) )
-                            probs_new[bias_idx] += self.bar_bias[1]
-                            newsum = sum(probs_new)
-                            probs_new = [p / newsum for p in probs_new]
-                        # print('AFTER: %.3f %.3f'% (probs_new[0], probs_new[1]) )
-                        for i in range(len(probs_new)):
-                            probs[i] = probs[i] * self.alpha_old + probs_new[i] * self.alpha_new
-                        '''
-
-                        ''' Original method
-                        # Method 1: smoothen and bias
-                        for i in range( len(probs_new) ):
-                            probs[i] = probs[i] * self.alpha_old + probs_new[i] * self.alpha_new
-                        # bias bar
-                        if self.bar_bias is not None:
-                            probs[bias_idx] += self.bar_bias[1]
-                            newsum = sum(probs)
-                            probs = [p/newsum for p in probs]
-                        '''
-
-                        # determine the direction
-                        # TODO: np.argmax(probs)
-                        max_pidx = qc.get_index_max(probs)
-                        max_label = bar_dirs[max_pidx]
-
-                        if self.cfg.POSITIVE_FEEDBACK is False or \
-                                (self.cfg.POSITIVE_FEEDBACK and true_label == max_label):
-                            dx = probs[max_pidx]
-                            if max_label == 'R':
-                                dx *= self.bar_step_right
-                            elif max_label == 'L':
-                                dx *= self.bar_step_left
-                            elif max_label == 'U':
-                                dx *= self.bar_step_up
-                            elif max_label == 'D':
-                                dx *= self.bar_step_down
-                            elif max_label == 'B':
-                                dx *= self.bar_step_both
-                            else:
-                                logger.debug('Direction %s using bar step %d' % (max_label, self.bar_step_left))
-                                dx *= self.bar_step_left
-
-                            # slow start
-                            selected = self.cfg.BAR_SLOW_START['selected']
-                            if self.cfg.BAR_SLOW_START[selected] and self.tm_trigger.sec() < self.cfg.BAR_SLOW_START[selected]:
-                                dx *= self.tm_trigger.sec() / self.cfg.BAR_SLOW_START[selected][0]
-
-                            # add likelihoods
-                            if max_label == bar_label:
-                                bar_score += dx
-                            else:
-                                bar_score -= dx
-                                # change of direction
-                                if bar_score < 0:
-                                    bar_score = -bar_score
-                                    bar_label = max_label
-                            bar_score = int(bar_score)
-                            if bar_score > 100:
-                                bar_score = 100
-                            if self.cfg.FEEDBACK_TYPE == 'IMAGE':
-                                if self.cfg.SHOW_CUE:
-                                    self.viz.move(bar_label, bar_score, overlay=False, caption=DIRS[true_label], caption_color='G')
-                                else:
-                                    self.viz.move(bar_label, bar_score, overlay=False)
-                            else:
-                                self.viz.move(bar_label, bar_score, overlay=False)
-
-                            # send the confidence value continuously
-                            if self.cfg.WITH_STIMO and self.cfg.STIMO_CONTINUOUS:
-                                if self.stimo_timer.sec() >= self.cfg.STIMO_COOLOFF:
-                                    if bar_label == 'U':
-                                        stimo_code = bar_score
-                                    else:
-                                        stimo_code = 0
-                                    self.ser.write(bytes([stimo_code]))
-                                    logger.info('Sent STIMO code %d' % stimo_code)
-                                    self.stimo_timer.reset()
-
-                        if self.cfg.DEBUG_PROBS:
-                            if self.bar_bias is not None:
-                                biastxt = '[Bias=%s%.3f]  ' % (self.bar_bias[0], self.bar_bias[1])
-                            else:
-                                biastxt = ''
-                            msg = '%s%s  prob %s   acc %s   bar %s%d  (%.1f ms)' % \
-                                  (biastxt, bar_dirs, qc.list2string(probs_new, '%.2f'), qc.list2string(probs, '%.2f'),
-                                   bar_label, bar_score, tm_classify.msec())
-                            logger.info(msg)
-                            if self.logf is not None:
-                                self.logf.write(msg + '\n')
-
-            elif state == 'feedback' and self.tm_trigger.sec() > self.cfg.TIMINGS['FEEDBACK']:
-                self.trigger.signal(self.tdef.BLANK)
-                if self.cfg.FEEDBACK_TYPE == 'IMAGE':
-                    state = 'return'
-                    self.tm_trigger.reset()
-                else:
-                    state = 'gap_s'
-                    self.viz.fill()
-                    self.viz.update()
-                    return bar_label
-
-            elif state == 'return':
-                self.viz.set_glass_feedback(False)
-                if self.cfg.WITH_STIMO:
-                    self.viz.move(bar_label, bar_score, overlay=False, barcolor='B')
-                else:
-                    self.viz.move(bar_label, bar_score, overlay=False, barcolor='Y')
-                self.viz.set_glass_feedback(True)
-                bar_score -= 5
-                if bar_score <= 0:
-                    state = 'gap_s'
-                    self.viz.fill()
-                    self.viz.update()
-                    return bar_label
-
-            self.viz.update()
-            key = cv2.waitKeyEx(1)
-            if key == KEYS['esc']:
-                return
-            elif key == KEYS['space']:
-                dx = 0
-                bar_score = 0
-                probs = [1.0 / len(bar_dirs)] * len(bar_dirs)
-                self.viz.move(bar_dirs[0], bar_score, overlay=False)
-                self.viz.update()
-                logger.info('probs and dx reset.')
-                self.tm_trigger.reset()
-            elif key in ARROW_KEYS and ARROW_KEYS[key] in bar_dirs:
-                # change bias on the fly
-                if self.bar_bias is None:
-                    self.bar_bias = [ARROW_KEYS[key], BIAS_INCREMENT]
-                else:
-                    if ARROW_KEYS[key] == self.bar_bias[0]:
-                        self.bar_bias[1] += BIAS_INCREMENT
-                    elif self.bar_bias[1] >= BIAS_INCREMENT:
-                        self.bar_bias[1] -= BIAS_INCREMENT
-                    else:
-                        self.bar_bias = [ARROW_KEYS[key], BIAS_INCREMENT]
-                if self.bar_bias[1] == 0:
-                    self.bar_bias = None
-                else:
-                    bias_idx = bar_dirs.index(self.bar_bias[0])
+from __future__ import print_function, division
+
+"""
+Visual feedback with online decoding
+
+Kyuhwa Lee
+Swiss Federal Institute of Technology Lausanne (EPFL)
+
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+"""
+
+import neurodecode
+import cv2
+import os
+import neurodecode.utils.q_common as qc
+import numpy as np
+import time
+import serial
+import serial.tools.list_ports
+from neurodecode import logger
+
+# global constants
+KEYS = {'right':2555904, 'up':2490368, 'left':2424832, 'down':2621440, 'pgup':85, 'pgdn':86, 'home':80, 'end':87, 'space':32, 'esc':27}
+ARROW_KEYS = {KEYS['left']:'L', KEYS['right']:'R', KEYS['up']:'U', KEYS['down']:'D'}
+COLORS = dict(G=(20, 140, 0), B=(210, 0, 0), R=(0, 50, 200), Y=(0, 215, 235), K=(0, 0, 0), W=(255, 255, 255), w=(200, 200, 200))
+DIRS = {'L':'LEFT', 'R':'RIGHT', 'U':'UP', 'D':'DOWN', 'B':'BOTH'}
+BIAS_INCREMENT = 0.025
+
+class Feedback:
+    """
+    Perform a classification with visual feedback
+    """
+
+    def __init__(self, cfg, viz, tdef, trigger, logfile=None):
+        self.cfg = cfg
+        self.tdef = tdef
+        self.trigger = trigger
+        self.viz = viz
+        self.viz.fill()
+        self.refresh_delay = 1.0 / self.cfg.REFRESH_RATE
+        self.bar_step_left = self.cfg.BAR_STEP['left']
+        self.bar_step_right = self.cfg.BAR_STEP['right']
+        self.bar_step_up = self.cfg.BAR_STEP['up']
+        self.bar_step_down = self.cfg.BAR_STEP['down']
+        self.bar_step_both = self.cfg.BAR_STEP['both']
+
+        if type(self.cfg.BAR_BIAS) is tuple:
+            self.bar_bias = list(self.cfg.BAR_BIAS)
+        else:
+            self.bar_bias = self.cfg.BAR_BIAS
+
+        # New decoder: already smoothed by the decoder so bias after.
+        #self.alpha_old = self.cfg.PROB_ACC_ALPHA
+        #self.alpha_new = 1.0 - self.cfg.PROB_ACC_ALPHA
+
+        if hasattr(self.cfg, 'BAR_REACH_FINISH') and self.cfg.BAR_REACH_FINISH == True:
+            self.premature_end = True
+        else:
+            self.premature_end = False
+
+        self.tm_trigger = qc.Timer()
+        self.tm_display = qc.Timer()
+        self.tm_watchdog = qc.Timer()
+        if logfile is not None:
+            self.logf = open(logfile, 'w')
+        else:
+            self.logf = None
+
+        # STIMO only
+        if self.cfg.WITH_STIMO is True:
+            if self.cfg.STIMO_COMPORT is None:
+                atens = [x for x in serial.tools.list_ports.grep('ATEN')]
+                if len(atens) == 0:
+                    raise RuntimeError('No ATEN device found. Stop.')
+                try:
+                    self.stimo_port = atens[0].device
+                except AttributeError: # depends on Python distribution
+                    self.stimo_port = atens[0][0]
+            else:
+                self.stimo_port = self.cfg.STIMO_COMPORT
+            self.ser = serial.Serial(self.stimo_port, self.cfg.STIMO_BAUDRATE)
+            logger.info('STIMO serial port %s is_open = %s' % (self.stimo_port, self.ser.is_open))
+
+    def __del__(self):
+        # STIMO only
+        if self.cfg.WITH_STIMO is True:
+            self.ser.close()
+            logger.info('Closed STIMO serial port %s' % self.stimo_port)
+
+    def classify(self, decoder, true_label, title_text, bar_dirs, state='start', prob_history=None):
+        """
+        Run a single trial
+        """
+        true_label_index = bar_dirs.index(true_label)
+        self.tm_trigger.reset()
+        if self.bar_bias is not None:
+            bias_idx = bar_dirs.index(self.bar_bias[0])
+
+        if self.logf is not None:
+            self.logf.write('True label: %s\n' % true_label)
+
+        tm_classify = qc.Timer(autoreset=True)
+        self.stimo_timer = qc.Timer()
+        while True:
+            self.tm_display.sleep_atleast(self.refresh_delay)
+            self.tm_display.reset()
+            if state == 'start' and self.tm_trigger.sec() > self.cfg.TIMINGS['INIT']:
+                state = 'gap_s'
+                if self.cfg.TRIALS_PAUSE:
+                    self.viz.put_text('Press any key')
+                    self.viz.update()
+                    key = cv2.waitKeyEx()
+                    if key == KEYS['esc']:
+                        return
+                self.viz.fill()
+                self.tm_trigger.reset()
+                self.trigger.signal(self.tdef.INIT)
+
+            elif state == 'gap_s':
+                if self.cfg.TIMINGS['GAP'] > 0:
+                    self.viz.put_text(title_text)
+                state = 'gap'
+                self.tm_trigger.reset()
+
+            elif state == 'gap' and self.tm_trigger.sec() > self.cfg.TIMINGS['GAP']:
+                state = 'cue'
+                self.viz.fill()
+                self.viz.draw_cue()
+                self.viz.glass_draw_cue()
+                self.trigger.signal(self.tdef.CUE)
+                self.tm_trigger.reset()
+
+            elif state == 'cue' and self.tm_trigger.sec() > self.cfg.TIMINGS['READY']:
+                state = 'dir_r'
+
+                if self.cfg.SHOW_CUE is True:
+                    if self.cfg.FEEDBACK_TYPE == 'BAR':
+                        self.viz.move(true_label, 100, overlay=False, barcolor='G')
+                    elif self.cfg.FEEDBACK_TYPE == 'IMAGE':
+                        self.viz.put_text(DIRS[true_label], 'R')
+                    if true_label == 'L':  # left
+                        self.trigger.signal(self.tdef.LEFT_READY)
+                    elif true_label == 'R':  # right
+                        self.trigger.signal(self.tdef.RIGHT_READY)
+                    elif true_label == 'U':  # up
+                        self.trigger.signal(self.tdef.UP_READY)
+                    elif true_label == 'D':  # down
+                        self.trigger.signal(self.tdef.DOWN_READY)
+                    elif true_label == 'B':  # both hands
+                        self.trigger.signal(self.tdef.BOTH_READY)
+                    else:
+                        raise RuntimeError('Unknown direction %s' % true_label)
+                self.tm_trigger.reset()
+                '''
+                if self.cfg.FEEDBACK_TYPE == 'IMAGE':
+                    self.viz.set_pc_feedback(False)
+                self.viz.move(true_label, 100, overlay=False, barcolor='G')
+
+                if self.cfg.FEEDBACK_TYPE == 'IMAGE':
+                    self.viz.set_pc_feedback(True)
+                    if self.cfg.SHOW_CUE is True:
+                        self.viz.put_text(dirs[true_label], 'R')
+
+                if true_label == 'L':  # left
+                    self.trigger.signal(self.tdef.LEFREADY)
+                elif true_label == 'R':  # right
+                    self.trigger.signal(self.tdef.RIGHT_READY)
+                elif true_label == 'U':  # up
+                    self.trigger.signal(self.tdef.UP_READY)
+                elif true_label == 'D':  # down
+                    self.trigger.signal(self.tdef.DOWN_READY)
+                elif true_label == 'B':  # both hands
+                    self.trigger.signal(self.tdef.BOTH_READY)
+                else:
+                    raise RuntimeError('Unknown direction %s' % true_label)
+                self.tm_trigger.reset()
+                '''
+            elif state == 'dir_r' and self.tm_trigger.sec() > self.cfg.TIMINGS['DIR_CUE']:
+                self.viz.fill()
+                self.viz.draw_cue()
+                self.viz.glass_draw_cue()
+                state = 'dir'
+
+                # initialize bar scores
+                bar_label = bar_dirs[0]
+                bar_score = 0
+                probs = [1.0 / len(bar_dirs)] * len(bar_dirs)
+                self.viz.move(bar_label, bar_score, overlay=False)
+                probs_acc = np.zeros(len(probs))
+
+                if true_label == 'L':  # left
+                    self.trigger.signal(self.tdef.LEFT_GO)
+                elif true_label == 'R':  # right
+                    self.trigger.signal(self.tdef.RIGHT_GO)
+                elif true_label == 'U':  # up
+                    self.trigger.signal(self.tdef.UP_GO)
+                elif true_label == 'D':  # down
+                    self.trigger.signal(self.tdef.DOWN_GO)
+                elif true_label == 'B':  # both
+                    self.trigger.signal(self.tdef.BOTH_GO)
+                else:
+                    raise RuntimeError('Unknown truedirection %s' % true_label)
+
+                self.tm_watchdog.reset()
+                self.tm_trigger.reset()
+
+            elif state == 'dir':
+                if self.tm_trigger.sec() > self.cfg.TIMINGS['CLASSIFY'] or (self.premature_end and bar_score >= 100):
+                    if not hasattr(self.cfg, 'SHOW_RESULT') or self.cfg.SHOW_RESULT is True:
+                        # show classfication result
+                        if self.cfg.WITH_STIMO is True:
+                            if self.cfg.STIMO_FULLGAIT_CYCLE is not None and bar_label == 'U':
+                                res_color = 'G'
+                            elif self.cfg.TRIALS_RETRY is False or bar_label == true_label:
+                                res_color = 'G'
+                            else:
+                                res_color = 'Y'
+                        else:
+                            res_color = 'Y'
+                        if self.cfg.FEEDBACK_TYPE == 'IMAGE':
+                            self.viz.move(bar_label, bar_score, overlay=False, barcolor=res_color, caption=DIRS[bar_label], caption_color=res_color)
+                        else:
+                            self.viz.move(bar_label, 100, overlay=False, barcolor=res_color)
+                    else:
+                        res_color = 'Y'
+                        if self.cfg.FEEDBACK_TYPE == 'IMAGE':
+                            self.viz.move(bar_label, bar_score, overlay=False, barcolor=res_color, caption='TRIAL END', caption_color=res_color)
+                        else:
+                            self.viz.move(bar_label, 0, overlay=False, barcolor=res_color)
+                    self.trigger.signal(self.tdef.FEEDBACK)
+
+                    # STIMO
+                    if self.cfg.WITH_STIMO is True and self.cfg.STIMO_CONTINUOUS is False:
+                        if self.cfg.STIMO_FULLGAIT_CYCLE is not None:
+                            if bar_label == 'U':
+                                self.ser.write(self.cfg.STIMO_FULLGAIT_PATTERN[0])
+                                logger.info('STIMO: Sent 1')
+                                time.sleep(self.cfg.STIMO_FULLGAIT_CYCLE)
+                                self.ser.write(self.cfg.STIMO_FULLGAIT_PATTERN[1])
+                                logger.info('STIMO: Sent 2')
+                                time.sleep(self.cfg.STIMO_FULLGAIT_CYCLE)
+                        elif self.cfg.TRIALS_RETRY is False or bar_label == true_label:
+                            if bar_label == 'L':
+                                self.ser.write(b'1')
+                                logger.info('STIMO: Sent 1')
+                            elif bar_label == 'R':
+                                self.ser.write(b'2')
+                                logger.info('STIMO: Sent 2')
+
+                    if self.cfg.DEBUG_PROBS:
+                        msg = 'DEBUG: Accumulated probabilities = %s' % qc.list2string(probs_acc, '%.3f')
+                        logger.info(msg)
+                        if self.logf is not None:
+                            self.logf.write(msg + '\n')
+                    if self.logf is not None:
+                        self.logf.write('%s detected as %s (%d)\n\n' % (true_label, bar_label, bar_score))
+                        self.logf.flush()
+
+                    # end of trial
+                    state = 'feedback'
+                    self.tm_trigger.reset()
+                else:
+                    # classify
+                    probs_new = decoder.get_prob_smooth_unread()
+                    if probs_new is None:
+                        if self.tm_watchdog.sec() > 3:
+                            logger.warning('No classification being done. Are you receiving data streams?')
+                            self.tm_watchdog.reset()
+                    else:
+                        self.tm_watchdog.reset()
+
+                        if prob_history is not None:
+                            prob_history[true_label].append(probs_new[true_label_index])
+
+                        probs_acc += np.array(probs_new)
+
+                        '''
+                        New decoder: already smoothed by the decoder so bias after.
+                        '''
+                        probs = list(probs_new)
+                        if self.bar_bias is not None:
+                            probs[bias_idx] += self.bar_bias[1]
+                            newsum = sum(probs)
+                            probs = [p / newsum for p in probs]
+
+                        '''
+                        # Method 2: bias and smoothen
+                        if self.bar_bias is not None:
+                            # print('BEFORE: %.3f %.3f'% (probs_new[0], probs_new[1]) )
+                            probs_new[bias_idx] += self.bar_bias[1]
+                            newsum = sum(probs_new)
+                            probs_new = [p / newsum for p in probs_new]
+                        # print('AFTER: %.3f %.3f'% (probs_new[0], probs_new[1]) )
+                        for i in range(len(probs_new)):
+                            probs[i] = probs[i] * self.alpha_old + probs_new[i] * self.alpha_new
+                        '''
+
+                        ''' Original method
+                        # Method 1: smoothen and bias
+                        for i in range( len(probs_new) ):
+                            probs[i] = probs[i] * self.alpha_old + probs_new[i] * self.alpha_new
+                        # bias bar
+                        if self.bar_bias is not None:
+                            probs[bias_idx] += self.bar_bias[1]
+                            newsum = sum(probs)
+                            probs = [p/newsum for p in probs]
+                        '''
+
+                        # determine the direction
+                        # TODO: np.argmax(probs)
+                        max_pidx = qc.get_index_max(probs)
+                        max_label = bar_dirs[max_pidx]
+
+                        if self.cfg.POSITIVE_FEEDBACK is False or \
+                                (self.cfg.POSITIVE_FEEDBACK and true_label == max_label):
+                            dx = probs[max_pidx]
+                            if max_label == 'R':
+                                dx *= self.bar_step_right
+                            elif max_label == 'L':
+                                dx *= self.bar_step_left
+                            elif max_label == 'U':
+                                dx *= self.bar_step_up
+                            elif max_label == 'D':
+                                dx *= self.bar_step_down
+                            elif max_label == 'B':
+                                dx *= self.bar_step_both
+                            else:
+                                logger.debug('Direction %s using bar step %d' % (max_label, self.bar_step_left))
+                                dx *= self.bar_step_left
+
+                            # slow start
+                            selected = self.cfg.BAR_SLOW_START['selected']
+                            if self.cfg.BAR_SLOW_START[selected] and self.tm_trigger.sec() < self.cfg.BAR_SLOW_START[selected]:
+                                dx *= self.tm_trigger.sec() / self.cfg.BAR_SLOW_START[selected][0]
+
+                            # add likelihoods
+                            if max_label == bar_label:
+                                bar_score += dx
+                            else:
+                                bar_score -= dx
+                                # change of direction
+                                if bar_score < 0:
+                                    bar_score = -bar_score
+                                    bar_label = max_label
+                            bar_score = int(bar_score)
+                            if bar_score > 100:
+                                bar_score = 100
+                            if self.cfg.FEEDBACK_TYPE == 'IMAGE':
+                                if self.cfg.SHOW_CUE:
+                                    self.viz.move(bar_label, bar_score, overlay=False, caption=DIRS[true_label], caption_color='G')
+                                else:
+                                    self.viz.move(bar_label, bar_score, overlay=False)
+                            else:
+                                self.viz.move(bar_label, bar_score, overlay=False)
+
+                            # send the confidence value continuously
+                            if self.cfg.WITH_STIMO and self.cfg.STIMO_CONTINUOUS:
+                                if self.stimo_timer.sec() >= self.cfg.STIMO_COOLOFF:
+                                    if bar_label == 'U':
+                                        stimo_code = bar_score
+                                    else:
+                                        stimo_code = 0
+                                    self.ser.write(bytes([stimo_code]))
+                                    logger.info('Sent STIMO code %d' % stimo_code)
+                                    self.stimo_timer.reset()
+
+                        if self.cfg.DEBUG_PROBS:
+                            if self.bar_bias is not None:
+                                biastxt = '[Bias=%s%.3f]  ' % (self.bar_bias[0], self.bar_bias[1])
+                            else:
+                                biastxt = ''
+                            msg = '%s%s  prob %s   acc %s   bar %s%d  (%.1f ms)' % \
+                                  (biastxt, bar_dirs, qc.list2string(probs_new, '%.2f'), qc.list2string(probs, '%.2f'),
+                                   bar_label, bar_score, tm_classify.msec())
+                            logger.info(msg)
+                            if self.logf is not None:
+                                self.logf.write(msg + '\n')
+
+            elif state == 'feedback' and self.tm_trigger.sec() > self.cfg.TIMINGS['FEEDBACK']:
+                self.trigger.signal(self.tdef.BLANK)
+                if self.cfg.FEEDBACK_TYPE == 'IMAGE':
+                    state = 'return'
+                    self.tm_trigger.reset()
+                else:
+                    state = 'gap_s'
+                    self.viz.fill()
+                    self.viz.update()
+                    return bar_label
+
+            elif state == 'return':
+                self.viz.set_glass_feedback(False)
+                if self.cfg.WITH_STIMO:
+                    self.viz.move(bar_label, bar_score, overlay=False, barcolor='B')
+                else:
+                    self.viz.move(bar_label, bar_score, overlay=False, barcolor='Y')
+                self.viz.set_glass_feedback(True)
+                bar_score -= 5
+                if bar_score <= 0:
+                    state = 'gap_s'
+                    self.viz.fill()
+                    self.viz.update()
+                    return bar_label
+
+            self.viz.update()
+            key = cv2.waitKeyEx(1)
+            if key == KEYS['esc']:
+                return
+            elif key == KEYS['space']:
+                dx = 0
+                bar_score = 0
+                probs = [1.0 / len(bar_dirs)] * len(bar_dirs)
+                self.viz.move(bar_dirs[0], bar_score, overlay=False)
+                self.viz.update()
+                logger.info('probs and dx reset.')
+                self.tm_trigger.reset()
+            elif key in ARROW_KEYS and ARROW_KEYS[key] in bar_dirs:
+                # change bias on the fly
+                if self.bar_bias is None:
+                    self.bar_bias = [ARROW_KEYS[key], BIAS_INCREMENT]
+                else:
+                    if ARROW_KEYS[key] == self.bar_bias[0]:
+                        self.bar_bias[1] += BIAS_INCREMENT
+                    elif self.bar_bias[1] >= BIAS_INCREMENT:
+                        self.bar_bias[1] -= BIAS_INCREMENT
+                    else:
+                        self.bar_bias = [ARROW_KEYS[key], BIAS_INCREMENT]
+                if self.bar_bias[1] == 0:
+                    self.bar_bias = None
+                else:
+                    bias_idx = bar_dirs.index(self.bar_bias[0])
```

### Comparing `neurodecode-2.0.4/neurodecode/protocols/feedback_fes.py` & `neurodecode-2.0.5/neurodecode/protocols/feedback_fes.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,488 +1,488 @@
-from __future__ import print_function, division
-
-"""
-FES feedback with online decoding
-
-Kyuhwa Lee
-Swiss Federal Institute of Technology Lausanne (EPFL)
-
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""
-
-import neurodecode
-import cv2
-import os
-import neurodecode.utils.q_common as qc
-import numpy as np
-import time
-import serial
-import serial.tools.list_ports
-from neurodecode import logger
-import neurodecode.utils.Motionstim8 as fes
-
-
-# global constants
-KEYS = {'right':2555904, 'up':2490368, 'left':2424832, 'down':2621440, 'pgup':85, 'pgdn':86, 'home':80, 'end':87, 'space':32, 'esc':27}
-ARROW_KEYS = {KEYS['left']:'L', KEYS['right']:'R', KEYS['up']:'U', KEYS['down']:'D'}
-COLORS = dict(G=(20, 140, 0), B=(210, 0, 0), R=(0, 50, 200), Y=(0, 215, 235), K=(0, 0, 0), W=(255, 255, 255), w=(200, 200, 200))
-DIRS = {'L':'LEFT', 'R':'RIGHT', 'U':'UP', 'D':'DOWN', 'B':'BOTH'}
-BIAS_INCREMENT = 0.025
-
-class Feedback:
-    """
-    Perform a classification with visual feedback
-    """
-
-    def __init__(self, cfg, viz, tdef, trigger, logfile=None):
-        self.cfg = cfg
-        self.tdef = tdef
-        self.trigger = trigger
-        self.viz = viz
-        self.viz.fill()
-        self.refresh_delay = 1.0 / self.cfg.REFRESH_RATE
-        self.bar_step_left = self.cfg.BAR_STEP['left']
-        self.bar_step_right = self.cfg.BAR_STEP['right']
-        self.bar_step_up = self.cfg.BAR_STEP['up']
-        self.bar_step_down = self.cfg.BAR_STEP['down']
-        self.bar_step_both = self.cfg.BAR_STEP['both']
-
-        if type(self.cfg.BAR_BIAS) is tuple:
-            self.bar_bias = list(self.cfg.BAR_BIAS)
-        else:
-            self.bar_bias = self.cfg.BAR_BIAS
-
-        # New decoder: already smoothed by the decoder so bias after.
-        #self.alpha_old = self.cfg.PROB_ACC_ALPHA
-        #self.alpha_new = 1.0 - self.cfg.PROB_ACC_ALPHA
-
-        if hasattr(self.cfg, 'BAR_REACH_FINISH') and self.cfg.BAR_REACH_FINISH == True:
-            self.premature_end = True
-        else:
-            self.premature_end = False
-
-        self.tm_trigger = qc.Timer()
-        self.tm_display = qc.Timer()
-        self.tm_watchdog = qc.Timer()
-        if logfile is not None:
-            self.logf = open(logfile, 'w')
-        else:
-            self.logf = None
-
-        # STIMO only
-        if self.cfg.WITH_STIMO is True:
-            if self.cfg.STIMO_COMPORT is None:
-                atens = [x for x in serial.tools.list_ports.grep('ATEN')]
-                if len(atens) == 0:
-                    raise RuntimeError('No ATEN device found. Stop.')
-                try:
-                    self.stimo_port = atens[0].device
-                except AttributeError: # depends on Python distribution
-                    self.stimo_port = atens[0][0]
-            else:
-                self.stimo_port = self.cfg.STIMO_COMPORT
-            self.ser = serial.Serial(self.stimo_port, self.cfg.STIMO_BAUDRATE)
-            logger.info('STIMO serial port %s is_open = %s' % (self.stimo_port, self.ser.is_open))
-
-        # FES only
-        if self.cfg.WITH_FES is True:
-            self.stim = fes.Motionstim8()
-            self.stim.OpenSerialPort(self.cfg.FES_COMPORT)
-            self.stim.InitializeChannelListMode()
-            logger.info('Opened FES serial port')
-
-
-    def __del__(self):
-        # STIMO only
-        if self.cfg.WITH_STIMO is True:
-            self.ser.close()
-            logger.info('Closed STIMO serial port %s' % self.stimo_port)
-        # FES only
-        if self.cfg.WITH_FES is True:
-            stim_code = [0, 0, 0, 0, 0, 0, 0, 0]
-            self.stim.UpdateChannelSettings(stim_code)
-            self.stim.CloseSerialPort()
-            logger.info('Closed FES serial port')
-
-    def classify(self, decoder, true_label, title_text, bar_dirs, state='start', prob_history=None):
-        """
-        Run a single trial
-        """
-        true_label_index = bar_dirs.index(true_label)
-        self.tm_trigger.reset()
-        if self.bar_bias is not None:
-            bias_idx = bar_dirs.index(self.bar_bias[0])
-
-        if self.logf is not None:
-            self.logf.write('True label: %s\n' % true_label)
-
-        tm_classify = qc.Timer(autoreset=True)
-        self.stimo_timer = qc.Timer()
-        while True:
-            self.tm_display.sleep_atleast(self.refresh_delay)
-            self.tm_display.reset()
-            if state == 'start' and self.tm_trigger.sec() > self.cfg.TIMINGS['INIT']:
-                state = 'gap_s'
-                if self.cfg.TRIALS_PAUSE:
-                    self.viz.put_text('Press any key')
-                    self.viz.update()
-                    key = cv2.waitKeyEx()
-                    if key == KEYS['esc']:
-                        return
-                self.viz.fill()
-                self.tm_trigger.reset()
-                self.trigger.signal(self.tdef.INIT)
-
-            elif state == 'gap_s':
-                if self.cfg.TIMINGS['GAP'] > 0:
-                    self.viz.put_text(title_text)
-                state = 'gap'
-                self.tm_trigger.reset()
-
-            elif state == 'gap' and self.tm_trigger.sec() > self.cfg.TIMINGS['GAP']:
-                state = 'cue'
-                self.viz.fill()
-                self.viz.draw_cue()
-                self.viz.glass_draw_cue()
-                self.trigger.signal(self.tdef.CUE)
-                self.tm_trigger.reset()
-
-            elif state == 'cue' and self.tm_trigger.sec() > self.cfg.TIMINGS['READY']:
-                state = 'dir_r'
-
-                if self.cfg.SHOW_CUE is True:
-                    if self.cfg.FEEDBACK_TYPE == 'BAR':
-                        self.viz.move(true_label, 100, overlay=False, barcolor='G')
-                    elif self.cfg.FEEDBACK_TYPE == 'IMAGE':
-                        self.viz.put_text(DIRS[true_label], 'R')
-                    if true_label == 'L':  # left
-                        self.trigger.signal(self.tdef.LEFT_READY)
-                    elif true_label == 'R':  # right
-                        self.trigger.signal(self.tdef.RIGHT_READY)
-                    elif true_label == 'U':  # up
-                        self.trigger.signal(self.tdef.UP_READY)
-                    elif true_label == 'D':  # down
-                        self.trigger.signal(self.tdef.DOWN_READY)
-                    elif true_label == 'B':  # both hands
-                        self.trigger.signal(self.tdef.BOTH_READY)
-                    else:
-                        raise RuntimeError('Unknown direction %s' % true_label)
-                self.tm_trigger.reset()
-                '''
-                if self.cfg.FEEDBACK_TYPE == 'IMAGE':
-                    self.viz.set_pc_feedback(False)
-                self.viz.move(true_label, 100, overlay=False, barcolor='G')
-
-                if self.cfg.FEEDBACK_TYPE == 'IMAGE':
-                    self.viz.set_pc_feedback(True)
-                    if self.cfg.SHOW_CUE is True:
-                        self.viz.put_text(dirs[true_label], 'R')
-
-                if true_label == 'L':  # left
-                    self.trigger.signal(self.tdef.LEFREADY)
-                elif true_label == 'R':  # right
-                    self.trigger.signal(self.tdef.RIGHT_READY)
-                elif true_label == 'U':  # up
-                    self.trigger.signal(self.tdef.UP_READY)
-                elif true_label == 'D':  # down
-                    self.trigger.signal(self.tdef.DOWN_READY)
-                elif true_label == 'B':  # both hands
-                    self.trigger.signal(self.tdef.BOTH_READY)
-                else:
-                    raise RuntimeError('Unknown direction %s' % true_label)
-                self.tm_trigger.reset()
-                '''
-            elif state == 'dir_r' and self.tm_trigger.sec() > self.cfg.TIMINGS['DIR_CUE']:
-                self.viz.fill()
-                self.viz.draw_cue()
-                self.viz.glass_draw_cue()
-                state = 'dir'
-
-                # initialize bar scores
-                bar_label = bar_dirs[0]
-                bar_score = 0
-                probs = [1.0 / len(bar_dirs)] * len(bar_dirs)
-                self.viz.move(bar_label, bar_score, overlay=False)
-                probs_acc = np.zeros(len(probs))
-
-                if true_label == 'L':  # left
-                    self.trigger.signal(self.tdef.LEFT_GO)
-                elif true_label == 'R':  # right
-                    self.trigger.signal(self.tdef.RIGHT_GO)
-                elif true_label == 'U':  # up
-                    self.trigger.signal(self.tdef.UP_GO)
-                elif true_label == 'D':  # down
-                    self.trigger.signal(self.tdef.DOWN_GO)
-                elif true_label == 'B':  # both
-                    self.trigger.signal(self.tdef.BOTH_GO)
-                else:
-                    raise RuntimeError('Unknown truedirection %s' % true_label)
-
-                self.tm_watchdog.reset()
-                self.tm_trigger.reset()
-
-            elif state == 'dir':
-                if self.tm_trigger.sec() > self.cfg.TIMINGS['CLASSIFY'] or (self.premature_end and bar_score >= 100):
-                    if not hasattr(self.cfg, 'SHOW_RESULT') or self.cfg.SHOW_RESULT is True:
-                        # show classfication result
-                        if self.cfg.WITH_STIMO is True:
-                            if self.cfg.STIMO_FULLGAIT_CYCLE is not None and bar_label == 'U':
-                                res_color = 'G'
-                            elif self.cfg.TRIALS_RETRY is False or bar_label == true_label:
-                                res_color = 'G'
-                            else:
-                                res_color = 'Y'
-                        else:
-                            res_color = 'Y'
-                        if self.cfg.FEEDBACK_TYPE == 'IMAGE':
-                            self.viz.move(bar_label, bar_score, overlay=False, barcolor=res_color, caption=DIRS[bar_label], caption_color=res_color)
-                        else:
-                            self.viz.move(bar_label, 100, overlay=False, barcolor=res_color)
-                    else:
-                        if self.cfg.FEEDBACK_TYPE == 'IMAGE':
-                            self.viz.move(bar_label, bar_score, overlay=False, barcolor=res_color, caption='TRIAL END', caption_color=res_color)
-                        else:
-                            self.viz.move(bar_label, 0, overlay=False, barcolor=res_color)
-                    self.trigger.signal(self.tdef.FEEDBACK)
-
-                    # STIMO
-                    if self.cfg.WITH_STIMO is True and self.cfg.STIMO_CONTINUOUS is False:
-                        if self.cfg.STIMO_FULLGAIT_CYCLE is not None:
-                            if bar_label == 'U':
-                                self.ser.write(self.cfg.STIMO_FULLGAIT_PATTERN[0])
-                                logger.info('STIMO: Sent 1')
-                                time.sleep(self.cfg.STIMO_FULLGAIT_CYCLE)
-                                self.ser.write(self.cfg.STIMO_FULLGAIT_PATTERN[1])
-                                logger.info('STIMO: Sent 2')
-                                time.sleep(self.cfg.STIMO_FULLGAIT_CYCLE)
-                        elif self.cfg.TRIALS_RETRY is False or bar_label == true_label:
-                            if bar_label == 'L':
-                                self.ser.write(b'1')
-                                logger.info('STIMO: Sent 1')
-                            elif bar_label == 'R':
-                                self.ser.write(b'2')
-                                logger.info('STIMO: Sent 2')
-
-
-                    # FES event mode mode
-                    if self.cfg.WITH_FES is True and self.cfg.FES_CONTINUOUS is False:
-                        if bar_label == 'L':
-                            stim_code = [0, 30, 0, 0, 0, 0, 0, 0]
-                            self.stim.UpdateChannelSettings(stim_code)
-                            logger.info('FES: Sent Left')
-                            time.sleep(0.5)
-                            stim_code = [0, 0, 0, 0, 0, 0, 0, 0]
-                            self.stim.UpdateChannelSettings(stim_code)
-
-                        elif bar_label == 'R':
-                            stim_code = [30, 0, 0, 0, 0, 0, 0, 0]
-                            self.stim.UpdateChannelSettings(stim_code)
-                            time.sleep(0.5)
-                            logger.info('FES: Sent Right')
-                            stim_code = [0, 0, 0, 0, 0, 0, 0, 0]
-                            self.stim.UpdateChannelSettings(stim_code)
-
-
-                    if self.cfg.DEBUG_PROBS:
-                        msg = 'DEBUG: Accumulated probabilities = %s' % qc.list2string(probs_acc, '%.3f')
-                        logger.info(msg)
-                        if self.logf is not None:
-                            self.logf.write(msg + '\n')
-                    if self.logf is not None:
-                        self.logf.write('%s detected as %s (%d)\n\n' % (true_label, bar_label, bar_score))
-                        self.logf.flush()
-
-                    # end of trial
-                    state = 'feedback'
-                    self.tm_trigger.reset()
-                else:
-                    # classify
-                    probs_new = decoder.get_prob_smooth_unread()
-                    if probs_new is None:
-                        if self.tm_watchdog.sec() > 3:
-                            logger.warning('No classification being done. Are you receiving data streams?')
-                            self.tm_watchdog.reset()
-                    else:
-                        self.tm_watchdog.reset()
-
-                        if prob_history is not None:
-                            prob_history[true_label].append(probs_new[true_label_index])
-
-                        probs_acc += np.array(probs_new)
-
-                        '''
-                        New decoder: already smoothed by the decoder so bias after.
-                        '''
-                        probs = list(probs_new)
-                        if self.bar_bias is not None:
-                            probs[bias_idx] += self.bar_bias[1]
-                            newsum = sum(probs)
-                            probs = [p / newsum for p in probs]
-
-                        '''
-                        # Method 2: bias and smoothen
-                        if self.bar_bias is not None:
-                            # print('BEFORE: %.3f %.3f'% (probs_new[0], probs_new[1]) )
-                            probs_new[bias_idx] += self.bar_bias[1]
-                            newsum = sum(probs_new)
-                            probs_new = [p / newsum for p in probs_new]
-                        # print('AFTER: %.3f %.3f'% (probs_new[0], probs_new[1]) )
-                        for i in range(len(probs_new)):
-                            probs[i] = probs[i] * self.alpha_old + probs_new[i] * self.alpha_new
-                        '''
-
-                        ''' Original method
-                        # Method 1: smoothen and bias
-                        for i in range( len(probs_new) ):
-                            probs[i] = probs[i] * self.alpha_old + probs_new[i] * self.alpha_new
-                        # bias bar
-                        if self.bar_bias is not None:
-                            probs[bias_idx] += self.bar_bias[1]
-                            newsum = sum(probs)
-                            probs = [p/newsum for p in probs]
-                        '''
-
-                        # determine the direction
-                        # TODO: np.argmax(probs)
-                        max_pidx = qc.get_index_max(probs)
-                        max_label = bar_dirs[max_pidx]
-
-                        if self.cfg.POSITIVE_FEEDBACK is False or \
-                                (self.cfg.POSITIVE_FEEDBACK and true_label == max_label):
-                            dx = probs[max_pidx]
-                            if max_label == 'R':
-                                dx *= self.bar_step_right
-                            elif max_label == 'L':
-                                dx *= self.bar_step_left
-                            elif max_label == 'U':
-                                dx *= self.bar_step_up
-                            elif max_label == 'D':
-                                dx *= self.bar_step_down
-                            elif max_label == 'B':
-                                dx *= self.bar_step_both
-                            else:
-                                logger.debug('Direction %s using bar step %d' % (max_label, self.bar_step_left))
-                                dx *= self.bar_step_left
-
-                            # slow start
-                            selected = self.cfg.BAR_SLOW_START['selected']
-                            if self.cfg.BAR_SLOW_START[selected] and self.tm_trigger.sec() < self.cfg.BAR_SLOW_START[selected]:
-                                dx *= self.tm_trigger.sec() / self.cfg.BAR_SLOW_START[selected][0]
-
-                            # add likelihoods
-                            if max_label == bar_label:
-                                bar_score += dx
-                            else:
-                                bar_score -= dx
-                                # change of direction
-                                if bar_score < 0:
-                                    bar_score = -bar_score
-                                    bar_label = max_label
-                            bar_score = int(bar_score)
-                            if bar_score > 100:
-                                bar_score = 100
-                            if self.cfg.FEEDBACK_TYPE == 'IMAGE':
-                                if self.cfg.SHOW_CUE:
-                                    self.viz.move(bar_label, bar_score, overlay=False, caption=DIRS[true_label], caption_color='G')
-                                else:
-                                    self.viz.move(bar_label, bar_score, overlay=False)
-                            else:
-                                self.viz.move(bar_label, bar_score, overlay=False)
-
-                            # send the confidence value continuously
-                            if self.cfg.WITH_STIMO and self.cfg.STIMO_CONTINUOUS:
-                                if self.stimo_timer.sec() >= self.cfg.STIMO_COOLOFF:
-                                    if bar_label == 'U':
-                                        stimo_code = bar_score
-                                    else:
-                                        stimo_code = 0
-                                    self.ser.write(bytes([stimo_code]))
-                                    logger.info('Sent STIMO code %d' % stimo_code)
-                                    self.stimo_timer.reset()
-                            # with FES
-                            if self.cfg.WITH_FES is True and self.cfg.FES_CONTINUOUS is True:
-                                if self.stimo_timer.sec() >= self.cfg.STIMO_COOLOFF:
-                                    if bar_label == 'L':
-                                        stim_code = [bar_score, 0, 0, 0, 0, 0, 0, 0]
-                                    else:
-                                        stim_code = [0, bar_score, 0, 0, 0, 0, 0, 0]
-                                    self.stim.UpdateChannelSettings(stim_code)
-                                    logger.info('Sent FES code %d' % bar_score)
-                                    self.stimo_timer.reset()
-
-                        if self.cfg.DEBUG_PROBS:
-                            if self.bar_bias is not None:
-                                biastxt = '[Bias=%s%.3f]  ' % (self.bar_bias[0], self.bar_bias[1])
-                            else:
-                                biastxt = ''
-                            msg = '%s%s  prob %s   acc %s   bar %s%d  (%.1f ms)' % \
-                                  (biastxt, bar_dirs, qc.list2string(probs_new, '%.2f'), qc.list2string(probs, '%.2f'),
-                                   bar_label, bar_score, tm_classify.msec())
-                            logger.info(msg)
-                            if self.logf is not None:
-                                self.logf.write(msg + '\n')
-
-            elif state == 'feedback' and self.tm_trigger.sec() > self.cfg.TIMINGS['FEEDBACK']:
-                self.trigger.signal(self.tdef.BLANK)
-                if self.cfg.FEEDBACK_TYPE == 'IMAGE':
-                    state = 'return'
-                    self.tm_trigger.reset()
-                else:
-                    state = 'gap_s'
-                    self.viz.fill()
-                    self.viz.update()
-                    return bar_label
-
-            elif state == 'return':
-                self.viz.set_glass_feedback(False)
-                if self.cfg.WITH_STIMO:
-                    self.viz.move(bar_label, bar_score, overlay=False, barcolor='B')
-                else:
-                    self.viz.move(bar_label, bar_score, overlay=False, barcolor='Y')
-                self.viz.set_glass_feedback(True)
-                bar_score -= 5
-                if bar_score <= 0:
-                    state = 'gap_s'
-                    self.viz.fill()
-                    self.viz.update()
-                    return bar_label
-
-            self.viz.update()
-            key = cv2.waitKeyEx(1)
-            if key == KEYS['esc']:
-                return
-            elif key == KEYS['space']:
-                dx = 0
-                bar_score = 0
-                probs = [1.0 / len(bar_dirs)] * len(bar_dirs)
-                self.viz.move(bar_dirs[0], bar_score, overlay=False)
-                self.viz.update()
-                logger.info('probs and dx reset.')
-                self.tm_trigger.reset()
-            elif key in ARROW_KEYS and ARROW_KEYS[key] in bar_dirs:
-                # change bias on the fly
-                if self.bar_bias is None:
-                    self.bar_bias = [ARROW_KEYS[key], BIAS_INCREMENT]
-                else:
-                    if ARROW_KEYS[key] == self.bar_bias[0]:
-                        self.bar_bias[1] += BIAS_INCREMENT
-                    elif self.bar_bias[1] >= BIAS_INCREMENT:
-                        self.bar_bias[1] -= BIAS_INCREMENT
-                    else:
-                        self.bar_bias = [ARROW_KEYS[key], BIAS_INCREMENT]
-                if self.bar_bias[1] == 0:
-                    self.bar_bias = None
-                else:
-                    bias_idx = bar_dirs.index(self.bar_bias[0])
+from __future__ import print_function, division
+
+"""
+FES feedback with online decoding
+
+Kyuhwa Lee
+Swiss Federal Institute of Technology Lausanne (EPFL)
+
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+"""
+
+import neurodecode
+import cv2
+import os
+import neurodecode.utils.q_common as qc
+import numpy as np
+import time
+import serial
+import serial.tools.list_ports
+from neurodecode import logger
+import neurodecode.utils.Motionstim8 as fes
+
+
+# global constants
+KEYS = {'right':2555904, 'up':2490368, 'left':2424832, 'down':2621440, 'pgup':85, 'pgdn':86, 'home':80, 'end':87, 'space':32, 'esc':27}
+ARROW_KEYS = {KEYS['left']:'L', KEYS['right']:'R', KEYS['up']:'U', KEYS['down']:'D'}
+COLORS = dict(G=(20, 140, 0), B=(210, 0, 0), R=(0, 50, 200), Y=(0, 215, 235), K=(0, 0, 0), W=(255, 255, 255), w=(200, 200, 200))
+DIRS = {'L':'LEFT', 'R':'RIGHT', 'U':'UP', 'D':'DOWN', 'B':'BOTH'}
+BIAS_INCREMENT = 0.025
+
+class Feedback:
+    """
+    Perform a classification with visual feedback
+    """
+
+    def __init__(self, cfg, viz, tdef, trigger, logfile=None):
+        self.cfg = cfg
+        self.tdef = tdef
+        self.trigger = trigger
+        self.viz = viz
+        self.viz.fill()
+        self.refresh_delay = 1.0 / self.cfg.REFRESH_RATE
+        self.bar_step_left = self.cfg.BAR_STEP['left']
+        self.bar_step_right = self.cfg.BAR_STEP['right']
+        self.bar_step_up = self.cfg.BAR_STEP['up']
+        self.bar_step_down = self.cfg.BAR_STEP['down']
+        self.bar_step_both = self.cfg.BAR_STEP['both']
+
+        if type(self.cfg.BAR_BIAS) is tuple:
+            self.bar_bias = list(self.cfg.BAR_BIAS)
+        else:
+            self.bar_bias = self.cfg.BAR_BIAS
+
+        # New decoder: already smoothed by the decoder so bias after.
+        #self.alpha_old = self.cfg.PROB_ACC_ALPHA
+        #self.alpha_new = 1.0 - self.cfg.PROB_ACC_ALPHA
+
+        if hasattr(self.cfg, 'BAR_REACH_FINISH') and self.cfg.BAR_REACH_FINISH == True:
+            self.premature_end = True
+        else:
+            self.premature_end = False
+
+        self.tm_trigger = qc.Timer()
+        self.tm_display = qc.Timer()
+        self.tm_watchdog = qc.Timer()
+        if logfile is not None:
+            self.logf = open(logfile, 'w')
+        else:
+            self.logf = None
+
+        # STIMO only
+        if self.cfg.WITH_STIMO is True:
+            if self.cfg.STIMO_COMPORT is None:
+                atens = [x for x in serial.tools.list_ports.grep('ATEN')]
+                if len(atens) == 0:
+                    raise RuntimeError('No ATEN device found. Stop.')
+                try:
+                    self.stimo_port = atens[0].device
+                except AttributeError: # depends on Python distribution
+                    self.stimo_port = atens[0][0]
+            else:
+                self.stimo_port = self.cfg.STIMO_COMPORT
+            self.ser = serial.Serial(self.stimo_port, self.cfg.STIMO_BAUDRATE)
+            logger.info('STIMO serial port %s is_open = %s' % (self.stimo_port, self.ser.is_open))
+
+        # FES only
+        if self.cfg.WITH_FES is True:
+            self.stim = fes.Motionstim8()
+            self.stim.OpenSerialPort(self.cfg.FES_COMPORT)
+            self.stim.InitializeChannelListMode()
+            logger.info('Opened FES serial port')
+
+
+    def __del__(self):
+        # STIMO only
+        if self.cfg.WITH_STIMO is True:
+            self.ser.close()
+            logger.info('Closed STIMO serial port %s' % self.stimo_port)
+        # FES only
+        if self.cfg.WITH_FES is True:
+            stim_code = [0, 0, 0, 0, 0, 0, 0, 0]
+            self.stim.UpdateChannelSettings(stim_code)
+            self.stim.CloseSerialPort()
+            logger.info('Closed FES serial port')
+
+    def classify(self, decoder, true_label, title_text, bar_dirs, state='start', prob_history=None):
+        """
+        Run a single trial
+        """
+        true_label_index = bar_dirs.index(true_label)
+        self.tm_trigger.reset()
+        if self.bar_bias is not None:
+            bias_idx = bar_dirs.index(self.bar_bias[0])
+
+        if self.logf is not None:
+            self.logf.write('True label: %s\n' % true_label)
+
+        tm_classify = qc.Timer(autoreset=True)
+        self.stimo_timer = qc.Timer()
+        while True:
+            self.tm_display.sleep_atleast(self.refresh_delay)
+            self.tm_display.reset()
+            if state == 'start' and self.tm_trigger.sec() > self.cfg.TIMINGS['INIT']:
+                state = 'gap_s'
+                if self.cfg.TRIALS_PAUSE:
+                    self.viz.put_text('Press any key')
+                    self.viz.update()
+                    key = cv2.waitKeyEx()
+                    if key == KEYS['esc']:
+                        return
+                self.viz.fill()
+                self.tm_trigger.reset()
+                self.trigger.signal(self.tdef.INIT)
+
+            elif state == 'gap_s':
+                if self.cfg.TIMINGS['GAP'] > 0:
+                    self.viz.put_text(title_text)
+                state = 'gap'
+                self.tm_trigger.reset()
+
+            elif state == 'gap' and self.tm_trigger.sec() > self.cfg.TIMINGS['GAP']:
+                state = 'cue'
+                self.viz.fill()
+                self.viz.draw_cue()
+                self.viz.glass_draw_cue()
+                self.trigger.signal(self.tdef.CUE)
+                self.tm_trigger.reset()
+
+            elif state == 'cue' and self.tm_trigger.sec() > self.cfg.TIMINGS['READY']:
+                state = 'dir_r'
+
+                if self.cfg.SHOW_CUE is True:
+                    if self.cfg.FEEDBACK_TYPE == 'BAR':
+                        self.viz.move(true_label, 100, overlay=False, barcolor='G')
+                    elif self.cfg.FEEDBACK_TYPE == 'IMAGE':
+                        self.viz.put_text(DIRS[true_label], 'R')
+                    if true_label == 'L':  # left
+                        self.trigger.signal(self.tdef.LEFT_READY)
+                    elif true_label == 'R':  # right
+                        self.trigger.signal(self.tdef.RIGHT_READY)
+                    elif true_label == 'U':  # up
+                        self.trigger.signal(self.tdef.UP_READY)
+                    elif true_label == 'D':  # down
+                        self.trigger.signal(self.tdef.DOWN_READY)
+                    elif true_label == 'B':  # both hands
+                        self.trigger.signal(self.tdef.BOTH_READY)
+                    else:
+                        raise RuntimeError('Unknown direction %s' % true_label)
+                self.tm_trigger.reset()
+                '''
+                if self.cfg.FEEDBACK_TYPE == 'IMAGE':
+                    self.viz.set_pc_feedback(False)
+                self.viz.move(true_label, 100, overlay=False, barcolor='G')
+
+                if self.cfg.FEEDBACK_TYPE == 'IMAGE':
+                    self.viz.set_pc_feedback(True)
+                    if self.cfg.SHOW_CUE is True:
+                        self.viz.put_text(dirs[true_label], 'R')
+
+                if true_label == 'L':  # left
+                    self.trigger.signal(self.tdef.LEFREADY)
+                elif true_label == 'R':  # right
+                    self.trigger.signal(self.tdef.RIGHT_READY)
+                elif true_label == 'U':  # up
+                    self.trigger.signal(self.tdef.UP_READY)
+                elif true_label == 'D':  # down
+                    self.trigger.signal(self.tdef.DOWN_READY)
+                elif true_label == 'B':  # both hands
+                    self.trigger.signal(self.tdef.BOTH_READY)
+                else:
+                    raise RuntimeError('Unknown direction %s' % true_label)
+                self.tm_trigger.reset()
+                '''
+            elif state == 'dir_r' and self.tm_trigger.sec() > self.cfg.TIMINGS['DIR_CUE']:
+                self.viz.fill()
+                self.viz.draw_cue()
+                self.viz.glass_draw_cue()
+                state = 'dir'
+
+                # initialize bar scores
+                bar_label = bar_dirs[0]
+                bar_score = 0
+                probs = [1.0 / len(bar_dirs)] * len(bar_dirs)
+                self.viz.move(bar_label, bar_score, overlay=False)
+                probs_acc = np.zeros(len(probs))
+
+                if true_label == 'L':  # left
+                    self.trigger.signal(self.tdef.LEFT_GO)
+                elif true_label == 'R':  # right
+                    self.trigger.signal(self.tdef.RIGHT_GO)
+                elif true_label == 'U':  # up
+                    self.trigger.signal(self.tdef.UP_GO)
+                elif true_label == 'D':  # down
+                    self.trigger.signal(self.tdef.DOWN_GO)
+                elif true_label == 'B':  # both
+                    self.trigger.signal(self.tdef.BOTH_GO)
+                else:
+                    raise RuntimeError('Unknown truedirection %s' % true_label)
+
+                self.tm_watchdog.reset()
+                self.tm_trigger.reset()
+
+            elif state == 'dir':
+                if self.tm_trigger.sec() > self.cfg.TIMINGS['CLASSIFY'] or (self.premature_end and bar_score >= 100):
+                    if not hasattr(self.cfg, 'SHOW_RESULT') or self.cfg.SHOW_RESULT is True:
+                        # show classfication result
+                        if self.cfg.WITH_STIMO is True:
+                            if self.cfg.STIMO_FULLGAIT_CYCLE is not None and bar_label == 'U':
+                                res_color = 'G'
+                            elif self.cfg.TRIALS_RETRY is False or bar_label == true_label:
+                                res_color = 'G'
+                            else:
+                                res_color = 'Y'
+                        else:
+                            res_color = 'Y'
+                        if self.cfg.FEEDBACK_TYPE == 'IMAGE':
+                            self.viz.move(bar_label, bar_score, overlay=False, barcolor=res_color, caption=DIRS[bar_label], caption_color=res_color)
+                        else:
+                            self.viz.move(bar_label, 100, overlay=False, barcolor=res_color)
+                    else:
+                        if self.cfg.FEEDBACK_TYPE == 'IMAGE':
+                            self.viz.move(bar_label, bar_score, overlay=False, barcolor=res_color, caption='TRIAL END', caption_color=res_color)
+                        else:
+                            self.viz.move(bar_label, 0, overlay=False, barcolor=res_color)
+                    self.trigger.signal(self.tdef.FEEDBACK)
+
+                    # STIMO
+                    if self.cfg.WITH_STIMO is True and self.cfg.STIMO_CONTINUOUS is False:
+                        if self.cfg.STIMO_FULLGAIT_CYCLE is not None:
+                            if bar_label == 'U':
+                                self.ser.write(self.cfg.STIMO_FULLGAIT_PATTERN[0])
+                                logger.info('STIMO: Sent 1')
+                                time.sleep(self.cfg.STIMO_FULLGAIT_CYCLE)
+                                self.ser.write(self.cfg.STIMO_FULLGAIT_PATTERN[1])
+                                logger.info('STIMO: Sent 2')
+                                time.sleep(self.cfg.STIMO_FULLGAIT_CYCLE)
+                        elif self.cfg.TRIALS_RETRY is False or bar_label == true_label:
+                            if bar_label == 'L':
+                                self.ser.write(b'1')
+                                logger.info('STIMO: Sent 1')
+                            elif bar_label == 'R':
+                                self.ser.write(b'2')
+                                logger.info('STIMO: Sent 2')
+
+
+                    # FES event mode mode
+                    if self.cfg.WITH_FES is True and self.cfg.FES_CONTINUOUS is False:
+                        if bar_label == 'L':
+                            stim_code = [0, 30, 0, 0, 0, 0, 0, 0]
+                            self.stim.UpdateChannelSettings(stim_code)
+                            logger.info('FES: Sent Left')
+                            time.sleep(0.5)
+                            stim_code = [0, 0, 0, 0, 0, 0, 0, 0]
+                            self.stim.UpdateChannelSettings(stim_code)
+
+                        elif bar_label == 'R':
+                            stim_code = [30, 0, 0, 0, 0, 0, 0, 0]
+                            self.stim.UpdateChannelSettings(stim_code)
+                            time.sleep(0.5)
+                            logger.info('FES: Sent Right')
+                            stim_code = [0, 0, 0, 0, 0, 0, 0, 0]
+                            self.stim.UpdateChannelSettings(stim_code)
+
+
+                    if self.cfg.DEBUG_PROBS:
+                        msg = 'DEBUG: Accumulated probabilities = %s' % qc.list2string(probs_acc, '%.3f')
+                        logger.info(msg)
+                        if self.logf is not None:
+                            self.logf.write(msg + '\n')
+                    if self.logf is not None:
+                        self.logf.write('%s detected as %s (%d)\n\n' % (true_label, bar_label, bar_score))
+                        self.logf.flush()
+
+                    # end of trial
+                    state = 'feedback'
+                    self.tm_trigger.reset()
+                else:
+                    # classify
+                    probs_new = decoder.get_prob_smooth_unread()
+                    if probs_new is None:
+                        if self.tm_watchdog.sec() > 3:
+                            logger.warning('No classification being done. Are you receiving data streams?')
+                            self.tm_watchdog.reset()
+                    else:
+                        self.tm_watchdog.reset()
+
+                        if prob_history is not None:
+                            prob_history[true_label].append(probs_new[true_label_index])
+
+                        probs_acc += np.array(probs_new)
+
+                        '''
+                        New decoder: already smoothed by the decoder so bias after.
+                        '''
+                        probs = list(probs_new)
+                        if self.bar_bias is not None:
+                            probs[bias_idx] += self.bar_bias[1]
+                            newsum = sum(probs)
+                            probs = [p / newsum for p in probs]
+
+                        '''
+                        # Method 2: bias and smoothen
+                        if self.bar_bias is not None:
+                            # print('BEFORE: %.3f %.3f'% (probs_new[0], probs_new[1]) )
+                            probs_new[bias_idx] += self.bar_bias[1]
+                            newsum = sum(probs_new)
+                            probs_new = [p / newsum for p in probs_new]
+                        # print('AFTER: %.3f %.3f'% (probs_new[0], probs_new[1]) )
+                        for i in range(len(probs_new)):
+                            probs[i] = probs[i] * self.alpha_old + probs_new[i] * self.alpha_new
+                        '''
+
+                        ''' Original method
+                        # Method 1: smoothen and bias
+                        for i in range( len(probs_new) ):
+                            probs[i] = probs[i] * self.alpha_old + probs_new[i] * self.alpha_new
+                        # bias bar
+                        if self.bar_bias is not None:
+                            probs[bias_idx] += self.bar_bias[1]
+                            newsum = sum(probs)
+                            probs = [p/newsum for p in probs]
+                        '''
+
+                        # determine the direction
+                        # TODO: np.argmax(probs)
+                        max_pidx = qc.get_index_max(probs)
+                        max_label = bar_dirs[max_pidx]
+
+                        if self.cfg.POSITIVE_FEEDBACK is False or \
+                                (self.cfg.POSITIVE_FEEDBACK and true_label == max_label):
+                            dx = probs[max_pidx]
+                            if max_label == 'R':
+                                dx *= self.bar_step_right
+                            elif max_label == 'L':
+                                dx *= self.bar_step_left
+                            elif max_label == 'U':
+                                dx *= self.bar_step_up
+                            elif max_label == 'D':
+                                dx *= self.bar_step_down
+                            elif max_label == 'B':
+                                dx *= self.bar_step_both
+                            else:
+                                logger.debug('Direction %s using bar step %d' % (max_label, self.bar_step_left))
+                                dx *= self.bar_step_left
+
+                            # slow start
+                            selected = self.cfg.BAR_SLOW_START['selected']
+                            if self.cfg.BAR_SLOW_START[selected] and self.tm_trigger.sec() < self.cfg.BAR_SLOW_START[selected]:
+                                dx *= self.tm_trigger.sec() / self.cfg.BAR_SLOW_START[selected][0]
+
+                            # add likelihoods
+                            if max_label == bar_label:
+                                bar_score += dx
+                            else:
+                                bar_score -= dx
+                                # change of direction
+                                if bar_score < 0:
+                                    bar_score = -bar_score
+                                    bar_label = max_label
+                            bar_score = int(bar_score)
+                            if bar_score > 100:
+                                bar_score = 100
+                            if self.cfg.FEEDBACK_TYPE == 'IMAGE':
+                                if self.cfg.SHOW_CUE:
+                                    self.viz.move(bar_label, bar_score, overlay=False, caption=DIRS[true_label], caption_color='G')
+                                else:
+                                    self.viz.move(bar_label, bar_score, overlay=False)
+                            else:
+                                self.viz.move(bar_label, bar_score, overlay=False)
+
+                            # send the confidence value continuously
+                            if self.cfg.WITH_STIMO and self.cfg.STIMO_CONTINUOUS:
+                                if self.stimo_timer.sec() >= self.cfg.STIMO_COOLOFF:
+                                    if bar_label == 'U':
+                                        stimo_code = bar_score
+                                    else:
+                                        stimo_code = 0
+                                    self.ser.write(bytes([stimo_code]))
+                                    logger.info('Sent STIMO code %d' % stimo_code)
+                                    self.stimo_timer.reset()
+                            # with FES
+                            if self.cfg.WITH_FES is True and self.cfg.FES_CONTINUOUS is True:
+                                if self.stimo_timer.sec() >= self.cfg.STIMO_COOLOFF:
+                                    if bar_label == 'L':
+                                        stim_code = [bar_score, 0, 0, 0, 0, 0, 0, 0]
+                                    else:
+                                        stim_code = [0, bar_score, 0, 0, 0, 0, 0, 0]
+                                    self.stim.UpdateChannelSettings(stim_code)
+                                    logger.info('Sent FES code %d' % bar_score)
+                                    self.stimo_timer.reset()
+
+                        if self.cfg.DEBUG_PROBS:
+                            if self.bar_bias is not None:
+                                biastxt = '[Bias=%s%.3f]  ' % (self.bar_bias[0], self.bar_bias[1])
+                            else:
+                                biastxt = ''
+                            msg = '%s%s  prob %s   acc %s   bar %s%d  (%.1f ms)' % \
+                                  (biastxt, bar_dirs, qc.list2string(probs_new, '%.2f'), qc.list2string(probs, '%.2f'),
+                                   bar_label, bar_score, tm_classify.msec())
+                            logger.info(msg)
+                            if self.logf is not None:
+                                self.logf.write(msg + '\n')
+
+            elif state == 'feedback' and self.tm_trigger.sec() > self.cfg.TIMINGS['FEEDBACK']:
+                self.trigger.signal(self.tdef.BLANK)
+                if self.cfg.FEEDBACK_TYPE == 'IMAGE':
+                    state = 'return'
+                    self.tm_trigger.reset()
+                else:
+                    state = 'gap_s'
+                    self.viz.fill()
+                    self.viz.update()
+                    return bar_label
+
+            elif state == 'return':
+                self.viz.set_glass_feedback(False)
+                if self.cfg.WITH_STIMO:
+                    self.viz.move(bar_label, bar_score, overlay=False, barcolor='B')
+                else:
+                    self.viz.move(bar_label, bar_score, overlay=False, barcolor='Y')
+                self.viz.set_glass_feedback(True)
+                bar_score -= 5
+                if bar_score <= 0:
+                    state = 'gap_s'
+                    self.viz.fill()
+                    self.viz.update()
+                    return bar_label
+
+            self.viz.update()
+            key = cv2.waitKeyEx(1)
+            if key == KEYS['esc']:
+                return
+            elif key == KEYS['space']:
+                dx = 0
+                bar_score = 0
+                probs = [1.0 / len(bar_dirs)] * len(bar_dirs)
+                self.viz.move(bar_dirs[0], bar_score, overlay=False)
+                self.viz.update()
+                logger.info('probs and dx reset.')
+                self.tm_trigger.reset()
+            elif key in ARROW_KEYS and ARROW_KEYS[key] in bar_dirs:
+                # change bias on the fly
+                if self.bar_bias is None:
+                    self.bar_bias = [ARROW_KEYS[key], BIAS_INCREMENT]
+                else:
+                    if ARROW_KEYS[key] == self.bar_bias[0]:
+                        self.bar_bias[1] += BIAS_INCREMENT
+                    elif self.bar_bias[1] >= BIAS_INCREMENT:
+                        self.bar_bias[1] -= BIAS_INCREMENT
+                    else:
+                        self.bar_bias = [ARROW_KEYS[key], BIAS_INCREMENT]
+                if self.bar_bias[1] == 0:
+                    self.bar_bias = None
+                else:
+                    bias_idx = bar_dirs.index(self.bar_bias[0])
```

### Comparing `neurodecode-2.0.4/neurodecode/protocols/viz_bars.py` & `neurodecode-2.0.5/neurodecode/protocols/viz_bars.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-from __future__ import print_function, division
-
-"""
-Bar visual feedback class
-
-
-Kyuhwa Lee, 2015
-Swiss Federal Institute of Technology (EPFL)
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""
-
-import sys
-import numpy as np
-import time
-import cv2
-import neurodecode
-import neurodecode.glass.bgi_client as bgi_client
-import neurodecode.utils.q_common as qc
-from neurodecode import logger
-
-
-class BarVisual(object):
-    # Default setting
-    color = dict(G=(20, 140, 0), B=(210, 0, 0), R=(0, 50, 200),
-        Y=(0, 215, 235), K=(0, 0, 0), W=(255, 255, 255), w=(200, 200, 200))
-    barwidth = 100
-    textlimit = 20  # maximum number of characters to show
-
-    def __init__(self, use_glass=False, glass_feedback=True, pc_feedback=True, screen_pos=None, screen_size=None):
-        """
-        Input:
-            use_glass: if False, mock Glass will be used
-            glass_feedback: show feedback to the user?
-            pc_feedback: show feedback on the pc screen?
-            screen_pos: screen position in (x,y)
-            screen_size: screen size in (x,y)
-        """
-        # screen size and message setting
-        if screen_size is None:
-            if sys.platform.startswith('win'):
-                from win32api import GetSystemMetrics
-                screen_width = GetSystemMetrics(0)
-                screen_height = GetSystemMetrics(1)
-            else:
-                screen_width = 1024
-                screen_height = 768
-        else:
-            screen_width, screen_height = screen_size
-
-        if screen_pos is None:
-            screen_x, screen_y = (0, 0)
-        else:
-            screen_x, screen_y = screen_pos
-
-        self.text_x = int(screen_width / 4)
-        self.text_y = int(screen_height / 2)
-        self.text_size = 2
-        cv2.namedWindow("img", cv2.WINDOW_AUTOSIZE)
-        cv2.moveWindow("img", screen_x, screen_y)
-        cv2.setWindowProperty("img", cv2.WND_PROP_FULLSCREEN, cv2.WINDOW_FULLSCREEN);
-
-        self.img = np.zeros((screen_height, screen_width, 3), np.uint8)
-        self.glass = bgi_client.GlassControl(mock=not use_glass)
-        self.glass.connect('127.0.0.1', 59900)
-        self.set_glass_feedback(glass_feedback)
-        self.set_pc_feedback(pc_feedback)
-        self.set_cue_color(boxcol='B', crosscol='W')
-        self.width = self.img.shape[1]
-        self.height = self.img.shape[0]
-        hw = int(self.barwidth / 2)
-        self.cx = int(self.width / 2)
-        self.cy = int(self.height / 2)
-        self.xl1 = self.cx - hw  # 200
-        self.xl2 = self.xl1 - self.barwidth  # 100
-        self.xr1 = self.cx + hw  # 300
-        self.xr2 = self.xr1 + self.barwidth  # 400
-        self.yl1 = self.cy - hw
-        self.yl2 = self.yl1 - self.barwidth
-        self.yr1 = self.cy + hw
-        self.yr2 = self.yr1 + self.barwidth
-
-    def finish(self):
-        cv2.destroyAllWindows()
-        self.glass.disconnect()
-
-    def set_glass_feedback(self, fb):
-        self.glass_feedback = fb
-
-    def set_pc_feedback(self, fb):
-        self.pc_feedback = fb
-
-    def set_cue_color(self, boxcol='B', crosscol='W'):
-        self.boxcol = self.color[boxcol]
-        self.crosscol = self.color[crosscol]
-
-    def fill(self, fillcolor='K'):
-        self.glass.fill(fillcolor)
-        cv2.rectangle(self.img, (0, 0), (self.width, self.height), self.color[fillcolor], -1)
-
-    # draw cue with custom colors
-    def draw_cue(self):
-        cv2.rectangle(self.img, (self.xl2, self.yl1), (self.xr2, self.yr1), self.color['w'], -1)
-        cv2.rectangle(self.img, (self.xl1, self.yl2), (self.xr1, self.yr2), self.color['w'], -1)
-        cv2.rectangle(self.img, (self.xl1, self.yl1), (self.xr1, self.yr1), self.boxcol, -1)
-
-        # cross fixation point
-        #cv2.rectangle( self.img, (self.cx-3,self.cy), (self.cx+3,self.cy), self.crosscol, -1 )
-        #cv2.rectangle( self.img, (self.cx,self.cy-3), (self.cx,self.cy+3), self.crosscol, -1 )
-
-        # circle fixation point
-        cv2.circle(self.img, (self.cx, self.cy), 3, self.color['W'], -1)
-
-    # paints the new bar on top of the current image
-    def move(self, dir, dx, overlay=False, barcolor=None, caption='', caption_color='W'):
-        if not overlay:
-            self.draw_cue()
-
-        if barcolor is None:
-            if dx == self.xl2:
-                c = 'G'
-            else:
-                c = 'R'
-        else:
-            c = barcolor
-
-        self.glass.fullbar_color(c)
-        color = self.color[c]
-
-        if dir == 'L':
-            if self.pc_feedback:
-                cv2.rectangle(self.img, (self.xl1 - dx, self.yl1), (self.xl1, self.yr1), color, -1)
-            if self.glass_feedback:
-                self.glass.move_bar(dir, dx, overlay)
-        elif dir == 'U':
-            if self.pc_feedback:
-                cv2.rectangle(self.img, (self.xl1, self.yl1 - dx), (self.xr1, self.yl1), color, -1)
-            if self.glass_feedback:
-                self.glass.move_bar(dir, dx, overlay)
-        elif dir == 'R':
-            if self.pc_feedback:
-                cv2.rectangle(self.img, (self.xr1, self.yl1), (self.xr1 + dx, self.yr1), color, -1)
-            if self.glass_feedback:
-                self.glass.move_bar(dir, dx, overlay)
-        elif dir == 'D':
-            if self.pc_feedback:
-                cv2.rectangle(self.img, (self.xl1, self.yr1), (self.xr1, self.yr1 + dx), color, -1)
-            if self.glass_feedback:
-                self.glass.move_bar(dir, dx, overlay)
-        elif dir == 'B':
-            if self.pc_feedback:
-                cv2.rectangle(self.img, (self.xl1 - dx, self.yl1), (self.xl1, self.yr1), color, -1)
-                cv2.rectangle(self.img, (self.xr1, self.yl1), (self.xr1 + dx, self.yr1), color, -1)
-            if self.glass_feedback:
-                self.glass.move_bar('S', dx, overlay)
-        else:
-            logger.error('Unknown direction %s' % dir)
-        self.put_text(caption, caption_color)
-
-    def put_text(self, txt, color='W'):
-        cv2.putText(self.img, txt[:self.textlimit].center(self.textlimit, ' '), (self.text_x, self.text_y),\
-                    cv2.FONT_HERSHEY_DUPLEX, self.text_size, self.color[color], 2, cv2.LINE_AA)
-
-    def update(self):
-        cv2.imshow("img", self.img)
-        #time.sleep(0.0005) # needed for CV to update window -> seems ok without this line
-
-    # Glass functions
-    def glass_draw_cue(self):
-        self.glass.draw_cross()
-
-    def glass_fullbarcolor(self, color):
-        self.glass.set_fullbar_color(color)
+from __future__ import print_function, division
+
+"""
+Bar visual feedback class
+
+
+Kyuhwa Lee, 2015
+Swiss Federal Institute of Technology (EPFL)
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+"""
+
+import sys
+import numpy as np
+import time
+import cv2
+import neurodecode
+import neurodecode.glass.bgi_client as bgi_client
+import neurodecode.utils.q_common as qc
+from neurodecode import logger
+
+
+class BarVisual(object):
+    # Default setting
+    color = dict(G=(20, 140, 0), B=(210, 0, 0), R=(0, 50, 200),
+        Y=(0, 215, 235), K=(0, 0, 0), W=(255, 255, 255), w=(200, 200, 200))
+    barwidth = 100
+    textlimit = 20  # maximum number of characters to show
+
+    def __init__(self, use_glass=False, glass_feedback=True, pc_feedback=True, screen_pos=None, screen_size=None):
+        """
+        Input:
+            use_glass: if False, mock Glass will be used
+            glass_feedback: show feedback to the user?
+            pc_feedback: show feedback on the pc screen?
+            screen_pos: screen position in (x,y)
+            screen_size: screen size in (x,y)
+        """
+        # screen size and message setting
+        if screen_size is None:
+            if sys.platform.startswith('win'):
+                from win32api import GetSystemMetrics
+                screen_width = GetSystemMetrics(0)
+                screen_height = GetSystemMetrics(1)
+            else:
+                screen_width = 1024
+                screen_height = 768
+        else:
+            screen_width, screen_height = screen_size
+
+        if screen_pos is None:
+            screen_x, screen_y = (0, 0)
+        else:
+            screen_x, screen_y = screen_pos
+
+        self.text_x = int(screen_width / 4)
+        self.text_y = int(screen_height / 2)
+        self.text_size = 2
+        cv2.namedWindow("img", cv2.WINDOW_AUTOSIZE)
+        cv2.moveWindow("img", screen_x, screen_y)
+        cv2.setWindowProperty("img", cv2.WND_PROP_FULLSCREEN, cv2.WINDOW_FULLSCREEN);
+
+        self.img = np.zeros((screen_height, screen_width, 3), np.uint8)
+        self.glass = bgi_client.GlassControl(mock=not use_glass)
+        self.glass.connect('127.0.0.1', 59900)
+        self.set_glass_feedback(glass_feedback)
+        self.set_pc_feedback(pc_feedback)
+        self.set_cue_color(boxcol='B', crosscol='W')
+        self.width = self.img.shape[1]
+        self.height = self.img.shape[0]
+        hw = int(self.barwidth / 2)
+        self.cx = int(self.width / 2)
+        self.cy = int(self.height / 2)
+        self.xl1 = self.cx - hw  # 200
+        self.xl2 = self.xl1 - self.barwidth  # 100
+        self.xr1 = self.cx + hw  # 300
+        self.xr2 = self.xr1 + self.barwidth  # 400
+        self.yl1 = self.cy - hw
+        self.yl2 = self.yl1 - self.barwidth
+        self.yr1 = self.cy + hw
+        self.yr2 = self.yr1 + self.barwidth
+
+    def finish(self):
+        cv2.destroyAllWindows()
+        self.glass.disconnect()
+
+    def set_glass_feedback(self, fb):
+        self.glass_feedback = fb
+
+    def set_pc_feedback(self, fb):
+        self.pc_feedback = fb
+
+    def set_cue_color(self, boxcol='B', crosscol='W'):
+        self.boxcol = self.color[boxcol]
+        self.crosscol = self.color[crosscol]
+
+    def fill(self, fillcolor='K'):
+        self.glass.fill(fillcolor)
+        cv2.rectangle(self.img, (0, 0), (self.width, self.height), self.color[fillcolor], -1)
+
+    # draw cue with custom colors
+    def draw_cue(self):
+        cv2.rectangle(self.img, (self.xl2, self.yl1), (self.xr2, self.yr1), self.color['w'], -1)
+        cv2.rectangle(self.img, (self.xl1, self.yl2), (self.xr1, self.yr2), self.color['w'], -1)
+        cv2.rectangle(self.img, (self.xl1, self.yl1), (self.xr1, self.yr1), self.boxcol, -1)
+
+        # cross fixation point
+        #cv2.rectangle( self.img, (self.cx-3,self.cy), (self.cx+3,self.cy), self.crosscol, -1 )
+        #cv2.rectangle( self.img, (self.cx,self.cy-3), (self.cx,self.cy+3), self.crosscol, -1 )
+
+        # circle fixation point
+        cv2.circle(self.img, (self.cx, self.cy), 3, self.color['W'], -1)
+
+    # paints the new bar on top of the current image
+    def move(self, dir, dx, overlay=False, barcolor=None, caption='', caption_color='W'):
+        if not overlay:
+            self.draw_cue()
+
+        if barcolor is None:
+            if dx == self.xl2:
+                c = 'G'
+            else:
+                c = 'R'
+        else:
+            c = barcolor
+
+        self.glass.fullbar_color(c)
+        color = self.color[c]
+
+        if dir == 'L':
+            if self.pc_feedback:
+                cv2.rectangle(self.img, (self.xl1 - dx, self.yl1), (self.xl1, self.yr1), color, -1)
+            if self.glass_feedback:
+                self.glass.move_bar(dir, dx, overlay)
+        elif dir == 'U':
+            if self.pc_feedback:
+                cv2.rectangle(self.img, (self.xl1, self.yl1 - dx), (self.xr1, self.yl1), color, -1)
+            if self.glass_feedback:
+                self.glass.move_bar(dir, dx, overlay)
+        elif dir == 'R':
+            if self.pc_feedback:
+                cv2.rectangle(self.img, (self.xr1, self.yl1), (self.xr1 + dx, self.yr1), color, -1)
+            if self.glass_feedback:
+                self.glass.move_bar(dir, dx, overlay)
+        elif dir == 'D':
+            if self.pc_feedback:
+                cv2.rectangle(self.img, (self.xl1, self.yr1), (self.xr1, self.yr1 + dx), color, -1)
+            if self.glass_feedback:
+                self.glass.move_bar(dir, dx, overlay)
+        elif dir == 'B':
+            if self.pc_feedback:
+                cv2.rectangle(self.img, (self.xl1 - dx, self.yl1), (self.xl1, self.yr1), color, -1)
+                cv2.rectangle(self.img, (self.xr1, self.yl1), (self.xr1 + dx, self.yr1), color, -1)
+            if self.glass_feedback:
+                self.glass.move_bar('S', dx, overlay)
+        else:
+            logger.error('Unknown direction %s' % dir)
+        self.put_text(caption, caption_color)
+
+    def put_text(self, txt, color='W'):
+        cv2.putText(self.img, txt[:self.textlimit].center(self.textlimit, ' '), (self.text_x, self.text_y),\
+                    cv2.FONT_HERSHEY_DUPLEX, self.text_size, self.color[color], 2, cv2.LINE_AA)
+
+    def update(self):
+        cv2.imshow("img", self.img)
+        #time.sleep(0.0005) # needed for CV to update window -> seems ok without this line
+
+    # Glass functions
+    def glass_draw_cue(self):
+        self.glass.draw_cross()
+
+    def glass_fullbarcolor(self, color):
+        self.glass.set_fullbar_color(color)
```

### Comparing `neurodecode-2.0.4/neurodecode/protocols/viz_images.py` & `neurodecode-2.0.5/neurodecode/protocols/viz_images.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,248 +1,248 @@
-from __future__ import print_function, division
-
-"""
-Bar visual feedback class
-
-
-Kyuhwa Lee, 2015
-Swiss Federal Institute of Technology (EPFL)
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""
-
-import sys
-import os
-import gzip
-import time
-import cv2
-import numpy as np
-import neurodecode
-import neurodecode.glass.bgi_client as bgi_client
-import neurodecode.utils.q_common as qc
-from neurodecode import logger
-from builtins import input
-try:
-    import cPickle as pickle  # Python 2 (cPickle = C version of pickle)
-except ImportError:
-    import pickle  # Python 3 (C version is the default)
-
-
-def read_images(img_path, screen_size=None):
-    pnglist = []
-    for f in qc.get_file_list(img_path):
-        if f[-4:] != '.png':
-            continue
-
-        img = cv2.imread(f)
-        # fit to screen size if image is larger
-        if screen_size is not None:
-            screen_width, screen_height = screen_size
-            rx = img.shape[1] / screen_width
-            ry = img.shape[0] / screen_height
-            if max(rx, ry) > 1:
-                if rx > ry:
-                    target_w = screen_width
-                    target_h = int(img.shape[0] / rx)
-                elif rx < ry:
-                    target_w = int(img.shape[1] / ry)
-                    target_h = screen_height
-                else:
-                    target_w = screen_width
-                    target_h = screen_height
-            else:
-                target_w = img.shape[1]
-                target_h = img.shape[0]
-            dsize = (int(target_w), int(target_h))
-            img_res = cv2.resize(img, dsize, interpolation=cv2.INTER_LANCZOS4)
-            img_out = np.zeros((screen_height, screen_width, img.shape[2]), dtype=img.dtype)
-            ox = int((screen_width - target_w) / 2)
-            oy = int((screen_height - target_h) / 2)
-            img_out[oy:oy+target_h, ox:ox+target_w, :] = img_res
-        else:
-            img_out = img
-        pnglist.append(img_out)
-        print('.', end='')
-    logger.info('Done loading images.')
-    return pnglist
-
-
-class ImageVisual(object):
-    # Default setting
-    color = dict(G=(20, 140, 0), B=(255, 90, 0), R=(0, 50, 200), Y=(0, 215, 235), K=(0, 0, 0),\
-                 W=(255, 255, 255), w=(200, 200, 200))
-    barwidth = 100
-    textlimit = 25  # maximum number of characters to show
-
-    def __init__(self, image_path, use_glass=False, glass_feedback=True, pc_feedback=True, screen_pos=None, screen_size=None):
-        """
-        Input:
-            use_glass: if False, mock Glass will be used
-            glass_feedback: show feedback to the user?
-            pc_feedback: show feedback on the pc screen?
-            screen_pos: screen position in (x,y)
-            screen_size: screen size in (x,y)
-        """
-        # screen size and message setting
-        if screen_size is None:
-            if sys.platform.startswith('win'):
-                from win32api import GetSystemMetrics
-                screen_width = GetSystemMetrics(0)
-                screen_height = GetSystemMetrics(1)
-            else:
-                screen_width = 1024
-                screen_height = 768
-            screen_size = (screen_width, screen_height)
-        else:
-            screen_width, screen_height = screen_size
-        if screen_pos is None:
-            screen_x, screen_y = (0, 0)
-        else:
-            screen_x, screen_y = screen_pos
-
-        self.text_size = 2
-        self.img = np.zeros((screen_height, screen_width, 3), np.uint8)
-        self.glass = bgi_client.GlassControl(mock=not use_glass)
-        self.glass.connect('127.0.0.1', 59900)
-        self.set_glass_feedback(glass_feedback)
-        self.set_pc_feedback(pc_feedback)
-        self.set_cue_color(boxcol='B', crosscol='W')
-        self.width = self.img.shape[1]
-        self.height = self.img.shape[0]
-        hw = int(self.barwidth / 2)
-        self.cx = int(self.width / 2)
-        self.cy = int(self.height / 2)
-        self.xl1 = self.cx - hw
-        self.xl2 = self.xl1 - self.barwidth
-        self.xr1 = self.cx + hw
-        self.xr2 = self.xr1 + self.barwidth
-        self.yl1 = self.cy - hw
-        self.yl2 = self.yl1 - self.barwidth
-        self.yr1 = self.cy + hw
-        self.yr2 = self.yr1 + self.barwidth
-
-        if os.path.isdir(image_path):
-            # load images
-            left_image_path = '%s/left' % image_path
-            right_image_path = '%s/right' % image_path
-            tm = qc.Timer()
-            logger.info('Reading images from %s' % left_image_path )
-            self.left_images = read_images(left_image_path, screen_size)
-            logger.info('Reading images from %s' % right_image_path)
-            self.right_images = read_images(right_image_path, screen_size)
-            logger.info('Took %.1f s' % tm.sec())
-        else:
-            # load pickled images
-            # note: this is painfully slow in Pytohn 2 even with cPickle (3s vs 27s)
-            assert image_path[-4:] == '.pkl', 'The file must be of .pkl format'
-            logger.info('Loading image binary file %s ...' % image_path)
-            tm = qc.Timer()
-            with gzip.open(image_path, 'rb') as fp:
-                image_data = pickle.load(fp)
-            self.left_images = image_data['left_images']
-            self.right_images = image_data['right_images']
-            feedback_w = self.left_images[0].shape[1] / 2
-            feedback_h = self.left_images[0].shape[0] / 2
-            loc_x = [int(self.cx - feedback_w), int(self.cx + feedback_w)]
-            loc_y = [int(self.cy - feedback_h), int(self.cy + feedback_h)]
-            img_fit = np.zeros((screen_height, screen_width, 3), np.uint8)
-
-            # adjust to the current screen size
-            logger.info('Fitting images into the current screen size')
-            for i, img in enumerate(self.left_images):
-                img_fit = np.zeros((screen_height, screen_width, 3), np.uint8)
-                img_fit[loc_y[0]:loc_y[1], loc_x[0]:loc_x[1]] = img
-                self.left_images[i] = img_fit
-            for i, img in enumerate(self.right_images):
-                img_fit = np.zeros((screen_height, screen_width, 3), np.uint8)
-                img_fit[loc_y[0]:loc_y[1], loc_x[0]:loc_x[1]] = img
-                self.right_images[i] = img_fit
-
-            logger.info('Took %.1f s' % tm.sec())
-            logger.info('Done.')
-        cv2.namedWindow("Protocol", cv2.WND_PROP_FULLSCREEN)
-        cv2.moveWindow("Protocol", screen_x, screen_y)
-        cv2.setWindowProperty("Protocol", cv2.WND_PROP_FULLSCREEN, cv2.WINDOW_FULLSCREEN);
-
-    def finish(self):
-        cv2.destroyAllWindows()
-        self.glass.disconnect()
-
-    def set_glass_feedback(self, fb):
-        self.glass_feedback = fb
-
-    def set_pc_feedback(self, fb):
-        self.pc_feedback = fb
-
-    def set_cue_color(self, boxcol='B', crosscol='W'):
-        self.boxcol = self.color[boxcol]
-        self.crosscol = self.color[crosscol]
-
-    def fill(self, fillcolor='K'):
-        self.glass.fill(fillcolor)
-        self.img = self.left_images[0]
-        self.update()
-
-    # draw cue with custom colors
-    def draw_cue(self):
-        self.img = self.left_images[0]
-        self.update()
-
-    # paints the new bar on top of the current image
-    def move(self, dir, dx, overlay=False, barcolor=None, caption='', caption_color='W'):
-        if barcolor is None:
-            if dx == self.xl2:
-                c = 'G'
-            else:
-                c = 'R'
-        else:
-            c = barcolor
-
-        self.glass.fullbar_color(c)
-        color = self.color[c]
-
-        if dir == 'L':
-            if self.pc_feedback:
-                self.img = self.left_images[dx]
-            if self.glass_feedback:
-                self.glass.move_bar(dir, dx, overlay)
-        elif dir == 'R':
-            if self.pc_feedback:
-                self.img = self.right_images[dx]
-            if self.glass_feedback:
-                self.glass.move_bar(dir, dx, overlay)
-        else:
-            logger.error('Unknown direction %s' % dir)
-        self.put_text(caption, caption_color)
-        self.update()
-
-    def put_text(self, txt, color='W'):
-        self.img = self.img.copy()
-        size_wh, baseline = cv2.getTextSize(txt, cv2.FONT_HERSHEY_DUPLEX, self.text_size, 2)
-        pos = (int(self.cx - size_wh[0] / 2), int(self.cy - size_wh[1] / 2))
-        cv2.putText(self.img, txt[:self.textlimit], pos,
-                    cv2.FONT_HERSHEY_DUPLEX, self.text_size, self.color[color], 2, cv2.LINE_AA)
-        self.update()
-
-    def update(self):
-        cv2.imshow("Protocol", self.img)
-        #cv2.waitKey(1)  # at least 1 ms needed for CV to update window
-        time.sleep(0.0005)
-
-    # Glass functions
-    def glass_draw_cue(self):
-        self.glass.draw_cross()
-
-    def glass_fullbarcolor(self, color):
-        self.glass.set_fullbar_color(color)
+from __future__ import print_function, division
+
+"""
+Bar visual feedback class
+
+
+Kyuhwa Lee, 2015
+Swiss Federal Institute of Technology (EPFL)
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+"""
+
+import sys
+import os
+import gzip
+import time
+import cv2
+import numpy as np
+import neurodecode
+import neurodecode.glass.bgi_client as bgi_client
+import neurodecode.utils.q_common as qc
+from neurodecode import logger
+from builtins import input
+try:
+    import cPickle as pickle  # Python 2 (cPickle = C version of pickle)
+except ImportError:
+    import pickle  # Python 3 (C version is the default)
+
+
+def read_images(img_path, screen_size=None):
+    pnglist = []
+    for f in qc.get_file_list(img_path):
+        if f[-4:] != '.png':
+            continue
+
+        img = cv2.imread(f)
+        # fit to screen size if image is larger
+        if screen_size is not None:
+            screen_width, screen_height = screen_size
+            rx = img.shape[1] / screen_width
+            ry = img.shape[0] / screen_height
+            if max(rx, ry) > 1:
+                if rx > ry:
+                    target_w = screen_width
+                    target_h = int(img.shape[0] / rx)
+                elif rx < ry:
+                    target_w = int(img.shape[1] / ry)
+                    target_h = screen_height
+                else:
+                    target_w = screen_width
+                    target_h = screen_height
+            else:
+                target_w = img.shape[1]
+                target_h = img.shape[0]
+            dsize = (int(target_w), int(target_h))
+            img_res = cv2.resize(img, dsize, interpolation=cv2.INTER_LANCZOS4)
+            img_out = np.zeros((screen_height, screen_width, img.shape[2]), dtype=img.dtype)
+            ox = int((screen_width - target_w) / 2)
+            oy = int((screen_height - target_h) / 2)
+            img_out[oy:oy+target_h, ox:ox+target_w, :] = img_res
+        else:
+            img_out = img
+        pnglist.append(img_out)
+        print('.', end='')
+    logger.info('Done loading images.')
+    return pnglist
+
+
+class ImageVisual(object):
+    # Default setting
+    color = dict(G=(20, 140, 0), B=(255, 90, 0), R=(0, 50, 200), Y=(0, 215, 235), K=(0, 0, 0),\
+                 W=(255, 255, 255), w=(200, 200, 200))
+    barwidth = 100
+    textlimit = 25  # maximum number of characters to show
+
+    def __init__(self, image_path, use_glass=False, glass_feedback=True, pc_feedback=True, screen_pos=None, screen_size=None):
+        """
+        Input:
+            use_glass: if False, mock Glass will be used
+            glass_feedback: show feedback to the user?
+            pc_feedback: show feedback on the pc screen?
+            screen_pos: screen position in (x,y)
+            screen_size: screen size in (x,y)
+        """
+        # screen size and message setting
+        if screen_size is None:
+            if sys.platform.startswith('win'):
+                from win32api import GetSystemMetrics
+                screen_width = GetSystemMetrics(0)
+                screen_height = GetSystemMetrics(1)
+            else:
+                screen_width = 1024
+                screen_height = 768
+            screen_size = (screen_width, screen_height)
+        else:
+            screen_width, screen_height = screen_size
+        if screen_pos is None:
+            screen_x, screen_y = (0, 0)
+        else:
+            screen_x, screen_y = screen_pos
+
+        self.text_size = 2
+        self.img = np.zeros((screen_height, screen_width, 3), np.uint8)
+        self.glass = bgi_client.GlassControl(mock=not use_glass)
+        self.glass.connect('127.0.0.1', 59900)
+        self.set_glass_feedback(glass_feedback)
+        self.set_pc_feedback(pc_feedback)
+        self.set_cue_color(boxcol='B', crosscol='W')
+        self.width = self.img.shape[1]
+        self.height = self.img.shape[0]
+        hw = int(self.barwidth / 2)
+        self.cx = int(self.width / 2)
+        self.cy = int(self.height / 2)
+        self.xl1 = self.cx - hw
+        self.xl2 = self.xl1 - self.barwidth
+        self.xr1 = self.cx + hw
+        self.xr2 = self.xr1 + self.barwidth
+        self.yl1 = self.cy - hw
+        self.yl2 = self.yl1 - self.barwidth
+        self.yr1 = self.cy + hw
+        self.yr2 = self.yr1 + self.barwidth
+
+        if os.path.isdir(image_path):
+            # load images
+            left_image_path = '%s/left' % image_path
+            right_image_path = '%s/right' % image_path
+            tm = qc.Timer()
+            logger.info('Reading images from %s' % left_image_path )
+            self.left_images = read_images(left_image_path, screen_size)
+            logger.info('Reading images from %s' % right_image_path)
+            self.right_images = read_images(right_image_path, screen_size)
+            logger.info('Took %.1f s' % tm.sec())
+        else:
+            # load pickled images
+            # note: this is painfully slow in Pytohn 2 even with cPickle (3s vs 27s)
+            assert image_path[-4:] == '.pkl', 'The file must be of .pkl format'
+            logger.info('Loading image binary file %s ...' % image_path)
+            tm = qc.Timer()
+            with gzip.open(image_path, 'rb') as fp:
+                image_data = pickle.load(fp)
+            self.left_images = image_data['left_images']
+            self.right_images = image_data['right_images']
+            feedback_w = self.left_images[0].shape[1] / 2
+            feedback_h = self.left_images[0].shape[0] / 2
+            loc_x = [int(self.cx - feedback_w), int(self.cx + feedback_w)]
+            loc_y = [int(self.cy - feedback_h), int(self.cy + feedback_h)]
+            img_fit = np.zeros((screen_height, screen_width, 3), np.uint8)
+
+            # adjust to the current screen size
+            logger.info('Fitting images into the current screen size')
+            for i, img in enumerate(self.left_images):
+                img_fit = np.zeros((screen_height, screen_width, 3), np.uint8)
+                img_fit[loc_y[0]:loc_y[1], loc_x[0]:loc_x[1]] = img
+                self.left_images[i] = img_fit
+            for i, img in enumerate(self.right_images):
+                img_fit = np.zeros((screen_height, screen_width, 3), np.uint8)
+                img_fit[loc_y[0]:loc_y[1], loc_x[0]:loc_x[1]] = img
+                self.right_images[i] = img_fit
+
+            logger.info('Took %.1f s' % tm.sec())
+            logger.info('Done.')
+        cv2.namedWindow("Protocol", cv2.WND_PROP_FULLSCREEN)
+        cv2.moveWindow("Protocol", screen_x, screen_y)
+        cv2.setWindowProperty("Protocol", cv2.WND_PROP_FULLSCREEN, cv2.WINDOW_FULLSCREEN);
+
+    def finish(self):
+        cv2.destroyAllWindows()
+        self.glass.disconnect()
+
+    def set_glass_feedback(self, fb):
+        self.glass_feedback = fb
+
+    def set_pc_feedback(self, fb):
+        self.pc_feedback = fb
+
+    def set_cue_color(self, boxcol='B', crosscol='W'):
+        self.boxcol = self.color[boxcol]
+        self.crosscol = self.color[crosscol]
+
+    def fill(self, fillcolor='K'):
+        self.glass.fill(fillcolor)
+        self.img = self.left_images[0]
+        self.update()
+
+    # draw cue with custom colors
+    def draw_cue(self):
+        self.img = self.left_images[0]
+        self.update()
+
+    # paints the new bar on top of the current image
+    def move(self, dir, dx, overlay=False, barcolor=None, caption='', caption_color='W'):
+        if barcolor is None:
+            if dx == self.xl2:
+                c = 'G'
+            else:
+                c = 'R'
+        else:
+            c = barcolor
+
+        self.glass.fullbar_color(c)
+        color = self.color[c]
+
+        if dir == 'L':
+            if self.pc_feedback:
+                self.img = self.left_images[dx]
+            if self.glass_feedback:
+                self.glass.move_bar(dir, dx, overlay)
+        elif dir == 'R':
+            if self.pc_feedback:
+                self.img = self.right_images[dx]
+            if self.glass_feedback:
+                self.glass.move_bar(dir, dx, overlay)
+        else:
+            logger.error('Unknown direction %s' % dir)
+        self.put_text(caption, caption_color)
+        self.update()
+
+    def put_text(self, txt, color='W'):
+        self.img = self.img.copy()
+        size_wh, baseline = cv2.getTextSize(txt, cv2.FONT_HERSHEY_DUPLEX, self.text_size, 2)
+        pos = (int(self.cx - size_wh[0] / 2), int(self.cy - size_wh[1] / 2))
+        cv2.putText(self.img, txt[:self.textlimit], pos,
+                    cv2.FONT_HERSHEY_DUPLEX, self.text_size, self.color[color], 2, cv2.LINE_AA)
+        self.update()
+
+    def update(self):
+        cv2.imshow("Protocol", self.img)
+        #cv2.waitKey(1)  # at least 1 ms needed for CV to update window
+        time.sleep(0.0005)
+
+    # Glass functions
+    def glass_draw_cue(self):
+        self.glass.draw_cross()
+
+    def glass_fullbarcolor(self, color):
+        self.glass.set_fullbar_color(color)
```

### Comparing `neurodecode-2.0.4/neurodecode/pycnbi_config.py` & `neurodecode-2.0.5/neurodecode/pycnbi_config.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-"""
-Neurodeocde global configurations
-
-Kyuhwa Lee, 2014
-
-"""
-
-import os
-
-# channel names (trigger channel is index 0 so that eeg channels start from index 1)
-CAP = {
-    'GTEC_16': ['TRIGGER', 'Fz', 'FC3', 'FC1', 'FCz', 'FC2', 'FC4',
-               'C3', 'C1', 'Cz', 'C2', 'C4', 'CP3', 'CP1', 'CPz', 'CP2', 'CP4'],
-    'GTEC_16_INFO': ['stim'] + ['eeg'] * 16,
-    'BIOSEMI_64': ['TRIGGER', 'Fp1', 'AF7', 'AF3', 'F1', 'F3', 'F5', 'F7', 'FT7',
-                  'FC5', 'FC3', 'FC1', 'C1', 'C3', 'C5', 'T7', 'TP7', 'CP5', 'CP3',
-                  'CP1', 'P1', 'P3', 'P5', 'P7', 'P9', 'PO7', 'PO3', 'O1', 'Iz',
-                  'Oz', 'POz', 'Pz', 'CPz', 'Fpz', 'Fp2', 'AF8', 'AF4', 'AFz', 'Fz',
-                  'F2', 'F4', 'F6', 'F8', 'FT8', 'FC6', 'FC4', 'FC2', 'FCz', 'Cz',
-                  'C2', 'C4', 'C6', 'T8', 'TP8', 'CP6', 'CP4', 'CP2', 'P2', 'P4',
-                  'P6', 'P8', 'P10', 'PO8', 'PO4', 'O2', 'EXG1', 'EXG2', 'EXG3',
-                  'EXG4', 'EXG5', 'EXG6', 'EXG7', 'EXG8'],
-    'BIOSEMI_64_INFO': ['stim'] + ['eeg'] * 64 + ['misc'] * 8,
-    'SMARTBCI_24': ['TRIGGER',
-                   'CH1', 'CH2', 'CH3', 'CH4', 'CH5', 'CH6', 'CH7', 'CH8', 'CH9', 'CH10',
-                   'CH11', 'CH12', 'CH13', 'CH14', 'CH15', 'CH16', 'CH17', 'CH18', 'CH19', 'CH20',
-                   'CH21', 'CH22', 'CH23'],
-    # 'SMARTBCI_24_INFO': ['stim'] + ['eeg']*8 + ['misc'] + ['eeg']*6 + ['misc'] + ['eeg']*7 #+ ['misc']
-    'SMARTBCI_24_INFO': ['stim'] + ['eeg'] * 23,  # CHANGE TO 24
-    'ANTNEURO_MI15': ['TRIGGER'] + ['Fz', 'FC1', 'FC2', 'C3', 'Cz', 'C4', 'CP1', 'CP2', 'FC3',
-                                   'FCz', 'FC4', 'C1', 'C2', 'CP3', 'CP4'],
-    'ANTNEURO_MI15_INFO': ['stim'] + ['eeg'] * 15,
-    'ANTNEURO_64': ['Fp1', 'Fpz', 'Fp2', 'F7', 'F3', 'Fz', 'F4', 'F8', 'FC5', 'FC1', 'FC2', 'FC6', 'T7', 'C3', 'Cz', 'C4', 'T8', 'CP5', 'CP1', 'CP2', 'CP6', 'P7', 'P3', 'Pz', 'P4', 'P8', 'POz', 'O1', 'O2', 'AF7', 'AF3', 'AF4', 'AF8', 'F5', 'F1', 'F2', 'F6', 'FC3', 'FCz', 'FC4', 'C5', 'C1', 'C2', 'C6', 'CP3', 'CP4', 'P5', 'P1', 'P2', 'P6', 'PO5', 'PO3', 'PO4', 'PO6', 'FT7', 'FT8', 'TP7', 'TP8', 'PO7', 'PO8', 'Oz'],
-    'ANTNEURO_64_NO_PERIPHERAL': ['F3', 'Fz', 'F4', 'FC5', 'FC1', 'FC2', 'FC6', 'C3', 'Cz', 'C4', 'CP5', 'CP1', 'CP2', 'CP6', 'P3', 'Pz', 'P4', 'POz', 'AF3', 'AF4', 'F5', 'F1', 'F2', 'F6', 'FC3', 'FCz', 'FC4', 'C5', 'C1', 'C2', 'C6', 'CP3', 'CP4', 'P5', 'P1', 'P2', 'P6', 'PO5', 'PO3', 'PO4', 'PO6'],
-    'DSI_24': ['Fp1', 'Fp2', 'Fz', 'F3', 'F4', 'F7', 'F8', 'Cz', 'C3', 'C4', 'T3', 'T4', 'T5', 'T6', 'Pz', 'P3', 'P4', 'O1', 'O2', 'A1', 'A2', 'X1', 'X2', 'X3']
-}
-
-# spatial laplacian channel definitions
-# TODO: Add BioSemi 64 channels
-LAPLACIAN = {
-    'GTEC_16':{1:[4], 2:[3, 7], 3:[2, 4, 8], 4:[3, 5, 9], 5:[4, 6, 10], 6:[5, 11],
-               7:[2, 8, 12], 8:[3, 7, 9, 13], 9:[4, 8, 10, 14], 10:[5, 9, 11, 15], 11:[6, 10, 16],
-               12:[7, 13], 13:[8, 12, 14], 14:[9, 13, 15], 15:[10, 14, 16], 16:[11, 15]}
-}
+"""
+Neurodeocde global configurations
+
+Kyuhwa Lee, 2014
+
+"""
+
+import os
+
+# channel names (trigger channel is index 0 so that eeg channels start from index 1)
+CAP = {
+    'GTEC_16': ['TRIGGER', 'Fz', 'FC3', 'FC1', 'FCz', 'FC2', 'FC4',
+               'C3', 'C1', 'Cz', 'C2', 'C4', 'CP3', 'CP1', 'CPz', 'CP2', 'CP4'],
+    'GTEC_16_INFO': ['stim'] + ['eeg'] * 16,
+    'BIOSEMI_64': ['TRIGGER', 'Fp1', 'AF7', 'AF3', 'F1', 'F3', 'F5', 'F7', 'FT7',
+                  'FC5', 'FC3', 'FC1', 'C1', 'C3', 'C5', 'T7', 'TP7', 'CP5', 'CP3',
+                  'CP1', 'P1', 'P3', 'P5', 'P7', 'P9', 'PO7', 'PO3', 'O1', 'Iz',
+                  'Oz', 'POz', 'Pz', 'CPz', 'Fpz', 'Fp2', 'AF8', 'AF4', 'AFz', 'Fz',
+                  'F2', 'F4', 'F6', 'F8', 'FT8', 'FC6', 'FC4', 'FC2', 'FCz', 'Cz',
+                  'C2', 'C4', 'C6', 'T8', 'TP8', 'CP6', 'CP4', 'CP2', 'P2', 'P4',
+                  'P6', 'P8', 'P10', 'PO8', 'PO4', 'O2', 'EXG1', 'EXG2', 'EXG3',
+                  'EXG4', 'EXG5', 'EXG6', 'EXG7', 'EXG8'],
+    'BIOSEMI_64_INFO': ['stim'] + ['eeg'] * 64 + ['misc'] * 8,
+    'SMARTBCI_24': ['TRIGGER',
+                   'CH1', 'CH2', 'CH3', 'CH4', 'CH5', 'CH6', 'CH7', 'CH8', 'CH9', 'CH10',
+                   'CH11', 'CH12', 'CH13', 'CH14', 'CH15', 'CH16', 'CH17', 'CH18', 'CH19', 'CH20',
+                   'CH21', 'CH22', 'CH23'],
+    # 'SMARTBCI_24_INFO': ['stim'] + ['eeg']*8 + ['misc'] + ['eeg']*6 + ['misc'] + ['eeg']*7 #+ ['misc']
+    'SMARTBCI_24_INFO': ['stim'] + ['eeg'] * 23,  # CHANGE TO 24
+    'ANTNEURO_MI15': ['TRIGGER'] + ['Fz', 'FC1', 'FC2', 'C3', 'Cz', 'C4', 'CP1', 'CP2', 'FC3',
+                                   'FCz', 'FC4', 'C1', 'C2', 'CP3', 'CP4'],
+    'ANTNEURO_MI15_INFO': ['stim'] + ['eeg'] * 15,
+    'ANTNEURO_64': ['Fp1', 'Fpz', 'Fp2', 'F7', 'F3', 'Fz', 'F4', 'F8', 'FC5', 'FC1', 'FC2', 'FC6', 'T7', 'C3', 'Cz', 'C4', 'T8', 'CP5', 'CP1', 'CP2', 'CP6', 'P7', 'P3', 'Pz', 'P4', 'P8', 'POz', 'O1', 'O2', 'AF7', 'AF3', 'AF4', 'AF8', 'F5', 'F1', 'F2', 'F6', 'FC3', 'FCz', 'FC4', 'C5', 'C1', 'C2', 'C6', 'CP3', 'CP4', 'P5', 'P1', 'P2', 'P6', 'PO5', 'PO3', 'PO4', 'PO6', 'FT7', 'FT8', 'TP7', 'TP8', 'PO7', 'PO8', 'Oz'],
+    'ANTNEURO_64_NO_PERIPHERAL': ['F3', 'Fz', 'F4', 'FC5', 'FC1', 'FC2', 'FC6', 'C3', 'Cz', 'C4', 'CP5', 'CP1', 'CP2', 'CP6', 'P3', 'Pz', 'P4', 'POz', 'AF3', 'AF4', 'F5', 'F1', 'F2', 'F6', 'FC3', 'FCz', 'FC4', 'C5', 'C1', 'C2', 'C6', 'CP3', 'CP4', 'P5', 'P1', 'P2', 'P6', 'PO5', 'PO3', 'PO4', 'PO6'],
+    'DSI_24': ['Fp1', 'Fp2', 'Fz', 'F3', 'F4', 'F7', 'F8', 'Cz', 'C3', 'C4', 'T3', 'T4', 'T5', 'T6', 'Pz', 'P3', 'P4', 'O1', 'O2', 'A1', 'A2', 'X1', 'X2', 'X3']
+}
+
+# spatial laplacian channel definitions
+# TODO: Add BioSemi 64 channels
+LAPLACIAN = {
+    'GTEC_16':{1:[4], 2:[3, 7], 3:[2, 4, 8], 4:[3, 5, 9], 5:[4, 6, 10], 6:[5, 11],
+               7:[2, 8, 12], 8:[3, 7, 9, 13], 9:[4, 8, 10, 14], 10:[5, 9, 11, 15], 11:[6, 10, 16],
+               12:[7, 13], 13:[8, 12, 14], 14:[9, 13, 15], 15:[10, 14, 16], 16:[11, 15]}
+}
```

### Comparing `neurodecode-2.0.4/neurodecode/stream_player/stream_player.py` & `neurodecode-2.0.5/neurodecode/stream_player/stream_player.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-from __future__ import print_function, division
-
-"""
-Stream Player
-
-Stream signals from a recorded file on LSL network.
-
-For Windows users, make sure to use the provided time resolution
-tweak tool to set to 500us time resolution of the OS.
-
-Kyuhwa Lee, 2015
-
-"""
-
-import os
-import sys
-import time
-import pylsl
-import numpy as np
-import neurodecode.utils.q_common as qc
-import neurodecode.utils.pycnbi_utils as pu
-from neurodecode.triggers.trigger_def import trigger_def
-from neurodecode import logger
-from builtins import input
-
-def stream_player(server_name, fif_file, chunk_size, auto_restart=True, wait_start=True, repeat=float('inf'), high_resolution=False, trigger_file=None):
-    """
-    Input
-    =====
-    server_name: LSL server name.
-    fif_file: fif file to replay.
-    chunk_size: number of samples to send at once (usually 16-32 is good enough).
-    auto_restart: play from beginning again after reaching the end.
-    wait_start: wait for user to start in the beginning.
-    repeat: number of loops to play.
-    high_resolution: use perf_counter() instead of sleep() for higher time resolution
-                     but uses much more cpu due to polling.
-    trigger_file: used to convert event numbers into event strings for readability.
-
-    Note: Run neurodecode.set_log_level('DEBUG') to print out the relative time stamps since started.
-
-    """
-    raw, events = pu.load_raw(fif_file)
-    sfreq = raw.info['sfreq']  # sampling frequency
-    n_channels = len(raw.ch_names)  # number of channels
-    if trigger_file is not None:
-        tdef = trigger_def(trigger_file)
-    try:
-        event_ch = raw.ch_names.index('TRIGGER')
-    except ValueError:
-        event_ch = None
-    if raw is not None:
-        logger.info_green('Successfully loaded %s' % fif_file)
-        logger.info('Server name: %s' % server_name)
-        logger.info('Sampling frequency %.3f Hz' % sfreq)
-        logger.info('Number of channels : %d' % n_channels)
-        logger.info('Chunk size : %d' % chunk_size)
-        for i, ch in enumerate(raw.ch_names):
-            logger.info('%d %s' % (i, ch))
-        logger.info('Trigger channel : %s' % event_ch)
-    else:
-        raise RuntimeError('Error while loading %s' % fif_file)
-
-    # set server information
-    sinfo = pylsl.StreamInfo(server_name, channel_count=n_channels, channel_format='float32', nominal_srate=sfreq, type='EEG', source_id=server_name)
-    desc = sinfo.desc()
-    channel_desc = desc.append_child("channels")
-    for ch in raw.ch_names:
-        channel_desc.append_child('channel').append_child_value('label', str(ch))\
-            .append_child_value('type','EEG').append_child_value('unit','microvolts')
-    desc.append_child('amplifier').append_child('settings').append_child_value('is_slave', 'false')
-    desc.append_child('acquisition').append_child_value('manufacturer', 'PyCNBI').append_child_value('serial_number', 'N/A')
-    outlet = pylsl.StreamOutlet(sinfo, chunk_size=chunk_size)
-
-    if wait_start:
-        input('Press Enter to start streaming.')
-    logger.info('Streaming started')
-
-    idx_chunk = 0
-    t_chunk = chunk_size / sfreq
-    finished = False
-    if high_resolution:
-        t_start = time.perf_counter()
-    else:
-        t_start = time.time()
-
-    # start streaming
-    played = 1
-    while played < repeat:
-        idx_current = idx_chunk * chunk_size
-        chunk = raw._data[:, idx_current:idx_current + chunk_size]
-        data = chunk.transpose().tolist()
-        if idx_current >= raw._data.shape[1] - chunk_size:
-            finished = True
-        if high_resolution:
-            # if a resolution over 2 KHz is needed
-            t_sleep_until = t_start + idx_chunk * t_chunk
-            while time.perf_counter() < t_sleep_until:
-                pass
-        else:
-            # time.sleep() can have 500 us resolution using the tweak tool provided.
-            t_wait = t_start + idx_chunk * t_chunk - time.time()
-            if t_wait > 0.001:
-                time.sleep(t_wait)
-
-        outlet.push_chunk(data)
-        logger.debug('[%8.3fs] sent %d samples (LSL %8.3f)' % (time.perf_counter(), len(data), pylsl.local_clock()))
-        if event_ch is not None:
-            event_values = set(chunk[event_ch]) - set([0])
-            if len(event_values) > 0:
-                if trigger_file is None:
-                    logger.info('Events: %s' % event_values)
-                else:
-                    for event in event_values:
-                        if event in tdef.by_value:
-                            logger.info('Events: %s (%s)' % (event, tdef.by_value[event]))
-                        else:
-                            logger.info('Events: %s (Undefined event)' % event)
-        idx_chunk += 1
-
-        if finished:
-            if auto_restart:
-                if wait_start:
-                    input('Reached the end of data. Press Enter to restart or Ctrl+C to stop.')
-                idx_chunk = 0
-                finished = False
-                if high_resolution:
-                    t_start = time.perf_counter()
-                else:
-                    t_start = time.time()
-                played += 1
-            else:
-                logger.info('Reached the end of data.')
-                break
-
-
-def main():
-    """
-    Invoked from console
-    """
-    if len(sys.argv) < 3:
-        print('Usage: %s fif_file chunk_size [server_name=StreamPlayer]' % os.path.basename(__file__))
-        return
-
-    fif_file = sys.argv[1]
-    chunk_size = int(sys.argv[2])
-    if len(sys.argv) > 3:
-        server_name = sys.argv[3]
-    else:
-        server_name = 'StreamPlayer'
-    stream_player(server_name, fif_file, chunk_size)
-
-def sample_code():
-    server_name = 'StreamPlayer'
-    chunk_size = 8
-    fif_file = '../../mi_left_right.fif'
-    stream_player(server_name, fif_file, chunk_size)
-
-# sample code
-if __name__ == '__main__':
-    main()
+from __future__ import print_function, division
+
+"""
+Stream Player
+
+Stream signals from a recorded file on LSL network.
+
+For Windows users, make sure to use the provided time resolution
+tweak tool to set to 500us time resolution of the OS.
+
+Kyuhwa Lee, 2015
+
+"""
+
+import os
+import sys
+import time
+import pylsl
+import numpy as np
+import neurodecode.utils.q_common as qc
+import neurodecode.utils.pycnbi_utils as pu
+from neurodecode.triggers.trigger_def import trigger_def
+from neurodecode import logger
+from builtins import input
+
+def stream_player(server_name, fif_file, chunk_size, auto_restart=True, wait_start=True, repeat=float('inf'), high_resolution=False, trigger_file=None):
+    """
+    Input
+    =====
+    server_name: LSL server name.
+    fif_file: fif file to replay.
+    chunk_size: number of samples to send at once (usually 16-32 is good enough).
+    auto_restart: play from beginning again after reaching the end.
+    wait_start: wait for user to start in the beginning.
+    repeat: number of loops to play.
+    high_resolution: use perf_counter() instead of sleep() for higher time resolution
+                     but uses much more cpu due to polling.
+    trigger_file: used to convert event numbers into event strings for readability.
+
+    Note: Run neurodecode.set_log_level('DEBUG') to print out the relative time stamps since started.
+
+    """
+    raw, events = pu.load_raw(fif_file)
+    sfreq = raw.info['sfreq']  # sampling frequency
+    n_channels = len(raw.ch_names)  # number of channels
+    if trigger_file is not None:
+        tdef = trigger_def(trigger_file)
+    try:
+        event_ch = raw.ch_names.index('TRIGGER')
+    except ValueError:
+        event_ch = None
+    if raw is not None:
+        logger.info_green('Successfully loaded %s' % fif_file)
+        logger.info('Server name: %s' % server_name)
+        logger.info('Sampling frequency %.3f Hz' % sfreq)
+        logger.info('Number of channels : %d' % n_channels)
+        logger.info('Chunk size : %d' % chunk_size)
+        for i, ch in enumerate(raw.ch_names):
+            logger.info('%d %s' % (i, ch))
+        logger.info('Trigger channel : %s' % event_ch)
+    else:
+        raise RuntimeError('Error while loading %s' % fif_file)
+
+    # set server information
+    sinfo = pylsl.StreamInfo(server_name, channel_count=n_channels, channel_format='float32', nominal_srate=sfreq, type='EEG', source_id=server_name)
+    desc = sinfo.desc()
+    channel_desc = desc.append_child("channels")
+    for ch in raw.ch_names:
+        channel_desc.append_child('channel').append_child_value('label', str(ch))\
+            .append_child_value('type','EEG').append_child_value('unit','microvolts')
+    desc.append_child('amplifier').append_child('settings').append_child_value('is_slave', 'false')
+    desc.append_child('acquisition').append_child_value('manufacturer', 'PyCNBI').append_child_value('serial_number', 'N/A')
+    outlet = pylsl.StreamOutlet(sinfo, chunk_size=chunk_size)
+
+    if wait_start:
+        input('Press Enter to start streaming.')
+    logger.info('Streaming started')
+
+    idx_chunk = 0
+    t_chunk = chunk_size / sfreq
+    finished = False
+    if high_resolution:
+        t_start = time.perf_counter()
+    else:
+        t_start = time.time()
+
+    # start streaming
+    played = 1
+    while played < repeat:
+        idx_current = idx_chunk * chunk_size
+        chunk = raw._data[:, idx_current:idx_current + chunk_size]
+        data = chunk.transpose().tolist()
+        if idx_current >= raw._data.shape[1] - chunk_size:
+            finished = True
+        if high_resolution:
+            # if a resolution over 2 KHz is needed
+            t_sleep_until = t_start + idx_chunk * t_chunk
+            while time.perf_counter() < t_sleep_until:
+                pass
+        else:
+            # time.sleep() can have 500 us resolution using the tweak tool provided.
+            t_wait = t_start + idx_chunk * t_chunk - time.time()
+            if t_wait > 0.001:
+                time.sleep(t_wait)
+
+        outlet.push_chunk(data)
+        logger.debug('[%8.3fs] sent %d samples (LSL %8.3f)' % (time.perf_counter(), len(data), pylsl.local_clock()))
+        if event_ch is not None:
+            event_values = set(chunk[event_ch]) - set([0])
+            if len(event_values) > 0:
+                if trigger_file is None:
+                    logger.info('Events: %s' % event_values)
+                else:
+                    for event in event_values:
+                        if event in tdef.by_value:
+                            logger.info('Events: %s (%s)' % (event, tdef.by_value[event]))
+                        else:
+                            logger.info('Events: %s (Undefined event)' % event)
+        idx_chunk += 1
+
+        if finished:
+            if auto_restart:
+                if wait_start:
+                    input('Reached the end of data. Press Enter to restart or Ctrl+C to stop.')
+                idx_chunk = 0
+                finished = False
+                if high_resolution:
+                    t_start = time.perf_counter()
+                else:
+                    t_start = time.time()
+                played += 1
+            else:
+                logger.info('Reached the end of data.')
+                break
+
+
+def main():
+    """
+    Invoked from console
+    """
+    if len(sys.argv) < 3:
+        print('Usage: %s fif_file chunk_size [server_name=StreamPlayer]' % os.path.basename(__file__))
+        return
+
+    fif_file = sys.argv[1]
+    chunk_size = int(sys.argv[2])
+    if len(sys.argv) > 3:
+        server_name = sys.argv[3]
+    else:
+        server_name = 'StreamPlayer'
+    stream_player(server_name, fif_file, chunk_size)
+
+def sample_code():
+    server_name = 'StreamPlayer'
+    chunk_size = 8
+    fif_file = '../../mi_left_right.fif'
+    stream_player(server_name, fif_file, chunk_size)
+
+# sample code
+if __name__ == '__main__':
+    main()
```

### Comparing `neurodecode-2.0.4/neurodecode/stream_receiver/stream_receiver.py` & `neurodecode-2.0.5/neurodecode/stream_receiver/stream_receiver.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,543 +1,543 @@
-from __future__ import print_function, division
-
-"""
-stream_receiver.py
-
-Acquires signals from LSL server and save into buffer.
-
-Note:
-- Trigger channel is always 0 and EEG channels start from 1. When there is no
-  known trigger channel, channel 0 is added with zero values for consistency.
-
-- BioSemi's Trigger values (Ch.0) should be taken with care because all
-  trigger pins are pulled to 1 and the data is written with 32 bits. Since
-  the usual parallel port supports only 8 bits, remove the highest 24 bits
-  by masking to 0 and subtract 1. A quick and dirty way is to subtract the
-  most commonly occurring value, which usually corresponds to zero value.
-  It only works when 0's are majority.
-
-- Some LSL servers, especially OpenVibe-based servers, send wrong LSL timestamps.
-  Most of the time, it does not matter but when you use software trigger, you will
-  need this offset to synchronize the event timings.
-
-TODO:
-   Restrict buffer size.
-
-Kyuhwa Lee, 2019
-Swiss Federal Institute of Technology Lausanne (EPFL)
-
-"""
-
-import sys
-import pdb
-import math
-import time
-import pylsl
-import numpy as np
-import neurodecode.utils.pycnbi_utils as pu
-import neurodecode.utils.q_common as qc
-from neurodecode.utils.pycnbi_utils import find_event_channel
-from neurodecode import logger
-
-class StreamReceiver:
-    def __init__(self, window_size=1, buffer_size=1, amp_serial=None, eeg_only=False, amp_name=None):
-        """
-        Params:
-            window_size (in seconds): keep the latest window_size seconds of the buffer.
-            buffer_size (in seconds): 1-day is the maximum size. Large buffer may lead to a delay if not pulled frequently.
-            amp_name: connect to a server named 'amp_name'. None: no constraint.
-            amp_serial: connect to a server with serial number 'amp_serial'. None: no constraint.
-            eeg_only: ignore non-EEG servers
-        """
-        _MAX_BUFFER_SIZE = 86400 # max buffer size allowed by StreamReceiver (24 hours)
-        _MAX_PYLSL_STREAM_BUFSIZE = 360 # max buffer size for pylsl.StreamInlet
-
-        if window_size <= 0:
-            logger.error('Wrong window_size %d.' % window_size)
-            raise ValueError()
-        self.winsec = window_size
-        if buffer_size == 0:
-            buffer_size = _MAX_BUFFER_SIZE
-        elif buffer_size < 0 or buffer_size > _MAX_BUFFER_SIZE:
-            logger.error('Improper buffer size %.1f. Setting to %d.' % (buffer_size, _MAX_BUFFER_SIZE))
-            buffer_size = _MAX_BUFFER_SIZE
-        elif buffer_size < self.winsec:
-            logger.error('Buffer size %.1f is smaller than window size. Setting to %.1f.' % (buffer_size, self.winsec))
-            buffer_size = self.winsec
-        self.bufsec = buffer_size
-        self.bufsize = 0 # to be calculated using sampling rate
-        self.stream_bufsec = int(math.ceil(min(_MAX_PYLSL_STREAM_BUFSIZE, self.bufsec)))
-        self.stream_bufsize = 0 # to be calculated using sampling rate
-        self.amp_serial = amp_serial
-        self.eeg_only = eeg_only
-        self.amp_name = amp_name
-        self.tr_channel = None  # trigger indx used by StreamReceiver class
-        self.eeg_channels = []  # signal indx used by StreamReceiver class
-        self._lsl_tr_channel = None  # raw trigger indx in pylsl.pull_chunk()
-        self._lsl_eeg_channels = []  # raw signal indx in pylsl.pull_chunk()
-        self.ready = False  # False until the buffer is filled for the first time
-        self.connected = False
-        self.buffers = []
-        self.timestamps = []
-        self.watchdog = qc.Timer()
-        self.multiplier = 1  # 10**6 for uV unit (automatically updated for openvibe servers)
-
-        self.connect()
-
-    def connect(self, find_any=True):
-        """
-        Run in child process
-        """
-        server_found = False
-        amps = []
-        channels = 0
-        while server_found == False:
-            if self.amp_name is None and self.amp_serial is None:
-                logger.info("Looking for a streaming server...")
-            else:
-                logger.info("Looking for %s (Serial %s) ..." % (self.amp_name, self.amp_serial))
-            streamInfos = pylsl.resolve_streams()
-            if len(streamInfos) > 0:
-                # For now, only 1 amp is supported by a single StreamReceiver object.
-                for si in streamInfos:
-                    # is_slave= ('true'==pylsl.StreamInlet(si).info().desc().child('amplifier').child('settings').child('is_slave').first_child().value() )
-                    inlet = pylsl.StreamInlet(si)
-                    # LSL XML parser has a bug which crashes so do not use for now
-                    #amp_serial = inlet.info().desc().child('acquisition').child_value('serial_number')
-                    amp_serial = 'N/A'
-                    amp_name = si.name()
-
-                    # connect to a specific amp only?
-                    if self.amp_serial is not None and self.amp_serial != amp_serial:
-                        continue
-
-                    # connect to a specific amp only?
-                    if self.amp_name is not None and self.amp_name != amp_name:
-                        continue
-
-                    # EEG streaming server only?
-                    if self.eeg_only and si.type() != 'EEG':
-                        continue
-
-                    if 'USBamp' in amp_name:
-                        logger.info('Found USBamp streaming server %s (type %s, amp_serial %s) @ %s.' % (amp_name, si.type(), amp_serial, si.hostname()))
-                        self._lsl_tr_channel = 16
-                        channels += si.channel_count()
-                        ch_list = pu.lsl_channel_list(inlet)
-                        amps.append(si)
-                        server_found = True
-                        break
-                    elif 'BioSemi' in amp_name:
-                        logger.info('Found BioSemi streaming server %s (type %s, amp_serial %s) @ %s.' % (amp_name, si.type(), amp_serial, si.hostname()))
-                        self._lsl_tr_channel = 0  # or subtract -6684927? (value when trigger==0)
-                        channels += si.channel_count()
-                        ch_list = pu.lsl_channel_list(inlet)
-                        amps.append(si)
-                        server_found = True
-                        break
-                    elif 'SmartBCI' in amp_name:
-                        logger.info('Found SmartBCI streaming server %s (type %s, amp_serial %s) @ %s.' % (amp_name, si.type(), amp_serial, si.hostname()))
-                        self._lsl_tr_channel = 23
-                        channels += si.channel_count()
-                        ch_list = pu.lsl_channel_list(inlet)
-                        amps.append(si)
-                        server_found = True
-                        break
-                    elif 'StreamPlayer' in amp_name:
-                        logger.info('Found StreamPlayer streaming server %s (type %s, amp_serial %s) @ %s.' % (amp_name, si.type(), amp_serial, si.hostname()))
-                        self._lsl_tr_channel = 0
-                        channels += si.channel_count()
-                        ch_list = pu.lsl_channel_list(inlet)
-                        amps.append(si)
-                        server_found = True
-                        break
-                    elif 'openvibeSignal' in amp_name:
-                        logger.info('Found an Openvibe signal streaming server %s (type %s, amp_serial %s) @ %s.' % (amp_name, si.type(), amp_serial, si.hostname()))
-                        ch_list = pu.lsl_channel_list(inlet)
-                        self._lsl_tr_channel = find_event_channel(ch_names=ch_list)
-                        channels += si.channel_count()
-                        amps.append(si)
-                        server_found = True
-                        # OpenVibe standard unit is Volts, which is not ideal for some numerical computations
-                        self.multiplier = 10**6 # change V -> uV unit for OpenVibe sources
-                        break
-                    elif 'openvibeMarkers' in amp_name:
-                        logger.info('Found an Openvibe markers server %s (type %s, amp_serial %s) @ %s.' % (amp_name, si.type(), amp_serial, si.hostname()))
-                        ch_list = pu.lsl_channel_list(inlet)
-                        self._lsl_tr_channel = find_event_channel(ch_names=ch_list)
-                        channels += si.channel_count()
-                        amps.append(si)
-                        server_found = True
-                        break
-                    elif find_any:
-                        logger.info('Found a streaming server %s (type %s, amp_serial %s) @ %s.' % (amp_name, si.type(), amp_serial, si.hostname()))
-                        ch_list = pu.lsl_channel_list(inlet)
-                        self._lsl_tr_channel = find_event_channel(ch_names=ch_list)
-                        channels += si.channel_count()
-                        amps.append(si)
-                        server_found = True
-                        break
-            time.sleep(1)
-
-        self.amp_name = amp_name
-
-        # define EEG channel indices
-        self._lsl_eeg_channels = list(range(channels))
-        if self._lsl_tr_channel is None:
-            logger.warning('Trigger channel not fonud. Adding an empty channel 0.')
-        else:
-            if self._lsl_tr_channel != 0:
-                logger.info('Trigger channel found at index %d. Moving to index 0.' % self._lsl_tr_channel)
-            self._lsl_eeg_channels.pop(self._lsl_tr_channel)
-        self._lsl_eeg_channels = np.array(self._lsl_eeg_channels)
-        self.tr_channel = 0  # trigger channel is always set to 0.
-        self.eeg_channels = np.arange(1, channels)  # signal channels start from 1.
-
-        # create new inlets to read from the stream
-        inlets_master = []
-        inlets_slaves = []
-        for amp in amps:
-            # data type of the 2nd argument (max_buflen) is int according to LSL C++ specification!
-            inlet = pylsl.StreamInlet(amp, max_buflen=self.stream_bufsec)
-            inlets_master.append(inlet)
-            self.buffers.append([])
-            self.timestamps.append([])
-
-        inlets = inlets_master + inlets_slaves
-        sample_rate = amps[0].nominal_srate()
-        logger.info('Channels: %d' % channels)
-        logger.info('LSL Protocol version: %s' % amps[0].version())
-        logger.info('Source sampling rate: %.1f' % sample_rate)
-        logger.info('Unit multiplier: %.1f' % self.multiplier)
-
-        #self.winsize = int(self.winsec * sample_rate)
-        #self.bufsize = int(self.bufsec * sample_rate)
-        self.winsize = int(round(self.winsec * sample_rate))
-        self.bufsize = int(round(self.bufsec * sample_rate))
-        self.stream_bufsize = int(round(self.stream_bufsec * sample_rate))
-        self.sample_rate = sample_rate
-        self.connected = True
-        self.ch_list = ch_list
-        self.inlets = inlets  # Note: not picklable!
-
-        # TODO: check if there's any problem with multiple inlets
-        if len(self.inlets) > 1:
-            logger.warning('Merging of multiple acquisition servers is not supported yet. Only %s will be used.' % amps[0].name())
-            '''
-            for i in range(1, len(self.inlets)):
-                chunk, tslist = self.inlets[i].pull_chunk(max_samples=self.stream_bufsize)
-                self.buffers[i].extend(chunk)
-                self.timestamps[i].extend(tslist)
-                if self.bufsize > 0 and len(self.buffers[i]) > self.bufsize:
-                    self.buffers[i] = self.buffers[i][-self.bufsize:]
-            '''
-
-        # create channel info
-        if self._lsl_tr_channel is None:
-            self.ch_list = ['TRIGGER'] + self.ch_list
-        else:
-            for i, chn in enumerate(self.ch_list):
-                if chn == 'TRIGGER' or chn == 'TRG' or 'STI ' in chn:
-                    self.ch_list.pop(i)
-                    self.ch_list = ['TRIGGER'] + self.ch_list
-                    break
-        logger.info('self.ch_list %s' % self.ch_list)
-
-        # fill in initial buffer
-        logger.info('Waiting to fill initial buffer of length %d' % (self.winsize))
-        while len(self.timestamps[0]) < self.winsize:
-            self.acquire()
-            time.sleep(0.1)
-        self.ready = True
-        logger.info('Start receiving stream data.')
-
-    def acquire(self, blocking=True):
-        """
-        Reads data into buffer. It is a blocking function as default.
-
-        Fills the buffer and return the current chunk of data and timestamps.
-
-        Returns:
-            data [samples x channels], timestamps [samples]
-        """
-        timestamp_offset = False
-        if len(self.timestamps[0]) == 0:
-            timestamp_offset = True
-
-        self.watchdog.reset()
-        tslist = []
-        received = False
-        chunk = None
-        while not received:
-            while self.watchdog.sec() < 5:
-                # chunk = [frames]x[ch], tslist = [frames]
-                if len(tslist) == 0:
-                    chunk, tslist = self.inlets[0].pull_chunk(max_samples=self.stream_bufsize)
-                    if blocking == False and len(tslist) == 0:
-                        return np.empty((0, len(self.ch_list))), []
-                if len(tslist) > 0:
-                    if timestamp_offset is True:
-                        lsl_clock = pylsl.local_clock()
-                    received = True
-                    break
-                time.sleep(0.0005)
-            else:
-                logger.warning('Timeout occurred while acquiring data. Amp driver bug?')
-                # give up and return empty values to avoid deadlock
-                return np.empty((0, len(self.ch_list))), []
-        data = np.array(chunk)
-
-        # BioSemi has pull-up resistor instead of pull-down
-        if self.amp_name == 'BioSemi' and self._lsl_tr_channel is not None:
-            datatype = data.dtype
-            data[:, self._lsl_tr_channel] = (np.bitwise_and(255, data[:, self._lsl_tr_channel].astype(int)) - 1).astype(datatype)
-
-        # multiply values (to change unit)
-        if self.multiplier != 1:
-            data[:, self._lsl_eeg_channels] *= self.multiplier
-
-        if self._lsl_tr_channel is not None:
-            # move trigger channel to 0 and add back to the buffer
-            data = np.concatenate((data[:, self._lsl_tr_channel].reshape(-1, 1),
-                                   data[:, self._lsl_eeg_channels]), axis=1)
-        else:
-            # add an empty channel with zeros to channel 0
-            data = np.concatenate((np.zeros((data.shape[0],1)),
-                                   data[:, self._lsl_eeg_channels]), axis=1)
-
-        # add data to buffer
-        chunk = data.tolist()
-        self.buffers[0].extend(chunk)
-        self.timestamps[0].extend(tslist)
-        if self.bufsize > 0 and len(self.timestamps[0]) > self.bufsize:
-            self.buffers[0] = self.buffers[0][-self.bufsize:]
-            self.timestamps[0] = self.timestamps[0][-self.bufsize:]
-
-        if timestamp_offset is True:
-            timestamp_offset = False
-            logger.info('LSL timestamp = %s' % lsl_clock)
-            logger.info('Server timestamp = %s' % self.timestamps[-1][-1])
-            self.lsl_time_offset = self.timestamps[-1][-1] - lsl_clock
-            logger.info('Offset = %.3f ' % (self.lsl_time_offset))
-            if abs(self.lsl_time_offset) > 0.1:
-                logger.warning('LSL server has a high timestamp offset.')
-            else:
-                logger.info_green('LSL time server synchronized')
-
-        ''' TODO: test the merging of multiple streams
-        # if we have multiple synchronized amps
-        if len(self.inlets) > 1:
-            for i in range(1, len(self.inlets)):
-                chunk, tslist = self.inlets[i].pull_chunk(max_samples=len(tslist))  # [frames][channels]
-                self.buffers[i].extend(chunk)
-                self.timestamps[i].extend(tslist)
-                if self.bufsize > 0 and len(self.buffers[i]) > self.bufsize:
-                    self.buffers[i] = self.buffers[i][-self.bufsize:]
-        '''
-
-        # data= array[samples, channels], tslist=[samples]
-        return (data, tslist)
-
-    def check_connect(self):
-        """
-        Check connection and automatically connect if not connected
-        """
-        while not self.connected:
-            logger.error('LSL server not connected yet. Trying to connect automatically.')
-            self.connect()
-            time.sleep(1)
-
-    def set_window_size(self, window_size):
-        """
-        Set window size (in seconds)
-        """
-        self.check_connect()
-        #self.winsize = int(window_size * self.sample_rate) + 1
-        self.winsize = int(round(window_size * self.sample_rate)) + 1
-
-    def get_channel_names(self):
-        """
-        Get a list of channels
-        """
-        return self.ch_list
-
-    def get_window_list(self):
-        """
-        Get the latest window
-        IT ONLY RETURNS list[amps][samples][channels]
-        """
-        self.check_connect()
-        window = self.buffers[0][-self.winsize:]
-        timestamps = self.timestamps[0][-self.winsize:]
-        return window, timestamps
-
-    def get_window(self, decim=1):
-        """
-        Get the latest window and timestamps in numpy format
-
-        input
-        -----
-        decim (int): decimation factor
-
-        output
-        ------
-        [samples x channels], [samples]
-        """
-        self.check_connect()
-        window, timestamps = self.get_window_list()
-
-        if len(timestamps) > 0:
-            # window = array[[samples_ch1],[samples_ch2]...]
-            return np.array(window), np.array(timestamps)
-        else:
-            return np.array([]), np.array([])
-
-    def get_buffer_list(self):
-        """
-        Get entire buffer
-        Returns the raw list: amps x samples x channels
-        """
-        self.check_connect()
-        return self.buffers, self.timestamps
-
-    def get_buffer(self):
-        """
-        Returns the entire buffer: samples x channels
-
-        If multiple amps, signals are concatenated along the channel axis.
-        """
-        self.check_connect()
-        try:
-            if len(self.timestamps[0]) > 0:
-                w = np.concatenate(self.buffers, axis=1) # samples x channels
-                t = np.array(self.timestamps).reshape(-1, 1) # samples x 1
-                return w, t
-            else:
-                return np.array([]), np.array([])
-        except:
-            logger.exception('Sorry! Unexpected error occurred in get_buffer(). Dropping into a shell for debugging.')
-            pdb.pm()
-
-    def get_buflen(self):
-        """
-        Return buffer length in seconds
-        """
-        return (len(self.timestamps[0]) / self.sample_rate)
-
-    def get_sample_rate(self):
-        """
-        Sampling rate
-        """
-        return self.sample_rate
-
-    def get_num_channels(self):
-        """
-        Total number of channels includingi trigger channel
-        """
-        return len(self.ch_list)
-
-    def get_eeg_channels(self):
-        """
-        Returns indices of eeg channels excluding trigger channel
-        """
-        return self.eeg_channels
-
-    def get_trigger_channel(self):
-        """
-        Return trigger channel (0-based index)
-        """
-        return self.tr_channel
-
-    def get_lsl_offset(self):
-        """
-        Return time difference of acquisition server's time and LSL time
-
-        OpenVibe servers often have a bug of sending its own running time instead of LSL time.
-        """
-        return self.lsl_time_offset
-
-    def reset_buffer(self):
-        """
-        Clear buffers
-        """
-        self.buffers = []
-
-    def is_ready(self):
-        """
-        Returns True if the buffer is not empty.
-        """
-        return self.ready
-
-
-"""
-Example code for printing out raw values
-"""
-def test_receiver():
-    import mne
-    import os
-
-    CH_INDEX = [1] # channel to monitor
-    TIME_INDEX = None # integer or None. None = average of raw values of the current window
-    SHOW_PSD = False
-    mne.set_log_level('ERROR')
-    os.environ['OMP_NUM_THREADS'] = '1' # actually improves performance for multitaper
-
-    # connect to LSL server
-    amp_name, amp_serial = pu.search_lsl()
-    sr = StreamReceiver(window_size=1, buffer_size=1, amp_serial=amp_serial, eeg_only=False, amp_name=amp_name)
-    sfreq = sr.get_sample_rate()
-    trg_ch = sr.get_trigger_channel()
-    logger.info('Trigger channel = %d' % trg_ch)
-
-    # PSD init
-    if SHOW_PSD:
-        psde = mne.decoding.PSDEstimator(sfreq=sfreq, fmin=1, fmax=50, bandwidth=None, \
-            adaptive=False, low_bias=True, n_jobs=1, normalization='length', verbose=None)
-
-    watchdog = qc.Timer()
-    tm = qc.Timer(autoreset=True)
-    last_ts = 0
-    while True:
-        sr.acquire()
-        window, tslist = sr.get_window() # window = [samples x channels]
-        window = window.T # chanel x samples
-
-        qc.print_c('LSL Diff = %.3f' % (pylsl.local_clock() - tslist[-1]), 'G')
-
-        # print event values
-        tsnew = np.where(np.array(tslist) > last_ts)[0]
-        if len(tsnew) == 0:
-            logger.warning('There seems to be delay in receiving data.')
-            time.sleep(1)
-            continue
-        trigger = np.unique(window[trg_ch, tsnew[0]:])
-
-        # for Biosemi
-        # if sr.amp_name=='BioSemi':
-        #    trigger= set( [255 & int(x-1) for x in trigger ] )
-
-        if len(trigger) > 0:
-            logger.info('Triggers: %s' % np.array(trigger))
-
-        logger.info('[%.1f] Receiving data...' % watchdog.sec())
-
-        if TIME_INDEX is None:
-            datatxt = qc.list2string(np.mean(window[CH_INDEX, :], axis=1), '%-15.6f')
-            print('[%.3f : %.3f]' % (tslist[0], tslist[-1]) + ' data: %s' % datatxt)
-        else:
-            datatxt = qc.list2string(window[CH_INDEX, TIME_INDEX], '%-15.6f')
-            print('[%.3f]' % tslist[TIME_INDEX] + ' data: %s' % datatxt)
-
-        # show PSD
-        if SHOW_PSD:
-            psd = psde.transform(window.reshape((1, window.shape[0], window.shape[1])))
-            psd = psd.reshape((psd.shape[1], psd.shape[2]))
-            psdmean = np.mean(psd, axis=1)
-            for p in psdmean:
-                print('%.1f' % p, end=' ')
-
-        last_ts = tslist[-1]
-        tm.sleep_atleast(0.05)
-
-if __name__ == '__main__':
-    test_receiver()
+from __future__ import print_function, division
+
+"""
+stream_receiver.py
+
+Acquires signals from LSL server and save into buffer.
+
+Note:
+- Trigger channel is always 0 and EEG channels start from 1. When there is no
+  known trigger channel, channel 0 is added with zero values for consistency.
+
+- BioSemi's Trigger values (Ch.0) should be taken with care because all
+  trigger pins are pulled to 1 and the data is written with 32 bits. Since
+  the usual parallel port supports only 8 bits, remove the highest 24 bits
+  by masking to 0 and subtract 1. A quick and dirty way is to subtract the
+  most commonly occurring value, which usually corresponds to zero value.
+  It only works when 0's are majority.
+
+- Some LSL servers, especially OpenVibe-based servers, send wrong LSL timestamps.
+  Most of the time, it does not matter but when you use software trigger, you will
+  need this offset to synchronize the event timings.
+
+TODO:
+   Restrict buffer size.
+
+Kyuhwa Lee, 2019
+Swiss Federal Institute of Technology Lausanne (EPFL)
+
+"""
+
+import sys
+import pdb
+import math
+import time
+import pylsl
+import numpy as np
+import neurodecode.utils.pycnbi_utils as pu
+import neurodecode.utils.q_common as qc
+from neurodecode.utils.pycnbi_utils import find_event_channel
+from neurodecode import logger
+
+class StreamReceiver:
+    def __init__(self, window_size=1, buffer_size=1, amp_serial=None, eeg_only=False, amp_name=None):
+        """
+        Params:
+            window_size (in seconds): keep the latest window_size seconds of the buffer.
+            buffer_size (in seconds): 1-day is the maximum size. Large buffer may lead to a delay if not pulled frequently.
+            amp_name: connect to a server named 'amp_name'. None: no constraint.
+            amp_serial: connect to a server with serial number 'amp_serial'. None: no constraint.
+            eeg_only: ignore non-EEG servers
+        """
+        _MAX_BUFFER_SIZE = 86400 # max buffer size allowed by StreamReceiver (24 hours)
+        _MAX_PYLSL_STREAM_BUFSIZE = 360 # max buffer size for pylsl.StreamInlet
+
+        if window_size <= 0:
+            logger.error('Wrong window_size %d.' % window_size)
+            raise ValueError()
+        self.winsec = window_size
+        if buffer_size == 0:
+            buffer_size = _MAX_BUFFER_SIZE
+        elif buffer_size < 0 or buffer_size > _MAX_BUFFER_SIZE:
+            logger.error('Improper buffer size %.1f. Setting to %d.' % (buffer_size, _MAX_BUFFER_SIZE))
+            buffer_size = _MAX_BUFFER_SIZE
+        elif buffer_size < self.winsec:
+            logger.error('Buffer size %.1f is smaller than window size. Setting to %.1f.' % (buffer_size, self.winsec))
+            buffer_size = self.winsec
+        self.bufsec = buffer_size
+        self.bufsize = 0 # to be calculated using sampling rate
+        self.stream_bufsec = int(math.ceil(min(_MAX_PYLSL_STREAM_BUFSIZE, self.bufsec)))
+        self.stream_bufsize = 0 # to be calculated using sampling rate
+        self.amp_serial = amp_serial
+        self.eeg_only = eeg_only
+        self.amp_name = amp_name
+        self.tr_channel = None  # trigger indx used by StreamReceiver class
+        self.eeg_channels = []  # signal indx used by StreamReceiver class
+        self._lsl_tr_channel = None  # raw trigger indx in pylsl.pull_chunk()
+        self._lsl_eeg_channels = []  # raw signal indx in pylsl.pull_chunk()
+        self.ready = False  # False until the buffer is filled for the first time
+        self.connected = False
+        self.buffers = []
+        self.timestamps = []
+        self.watchdog = qc.Timer()
+        self.multiplier = 1  # 10**6 for uV unit (automatically updated for openvibe servers)
+
+        self.connect()
+
+    def connect(self, find_any=True):
+        """
+        Run in child process
+        """
+        server_found = False
+        amps = []
+        channels = 0
+        while server_found == False:
+            if self.amp_name is None and self.amp_serial is None:
+                logger.info("Looking for a streaming server...")
+            else:
+                logger.info("Looking for %s (Serial %s) ..." % (self.amp_name, self.amp_serial))
+            streamInfos = pylsl.resolve_streams()
+            if len(streamInfos) > 0:
+                # For now, only 1 amp is supported by a single StreamReceiver object.
+                for si in streamInfos:
+                    # is_slave= ('true'==pylsl.StreamInlet(si).info().desc().child('amplifier').child('settings').child('is_slave').first_child().value() )
+                    inlet = pylsl.StreamInlet(si)
+                    # LSL XML parser has a bug which crashes so do not use for now
+                    #amp_serial = inlet.info().desc().child('acquisition').child_value('serial_number')
+                    amp_serial = 'N/A'
+                    amp_name = si.name()
+
+                    # connect to a specific amp only?
+                    if self.amp_serial is not None and self.amp_serial != amp_serial:
+                        continue
+
+                    # connect to a specific amp only?
+                    if self.amp_name is not None and self.amp_name != amp_name:
+                        continue
+
+                    # EEG streaming server only?
+                    if self.eeg_only and si.type() != 'EEG':
+                        continue
+
+                    if 'USBamp' in amp_name:
+                        logger.info('Found USBamp streaming server %s (type %s, amp_serial %s) @ %s.' % (amp_name, si.type(), amp_serial, si.hostname()))
+                        self._lsl_tr_channel = 16
+                        channels += si.channel_count()
+                        ch_list = pu.lsl_channel_list(inlet)
+                        amps.append(si)
+                        server_found = True
+                        break
+                    elif 'BioSemi' in amp_name:
+                        logger.info('Found BioSemi streaming server %s (type %s, amp_serial %s) @ %s.' % (amp_name, si.type(), amp_serial, si.hostname()))
+                        self._lsl_tr_channel = 0  # or subtract -6684927? (value when trigger==0)
+                        channels += si.channel_count()
+                        ch_list = pu.lsl_channel_list(inlet)
+                        amps.append(si)
+                        server_found = True
+                        break
+                    elif 'SmartBCI' in amp_name:
+                        logger.info('Found SmartBCI streaming server %s (type %s, amp_serial %s) @ %s.' % (amp_name, si.type(), amp_serial, si.hostname()))
+                        self._lsl_tr_channel = 23
+                        channels += si.channel_count()
+                        ch_list = pu.lsl_channel_list(inlet)
+                        amps.append(si)
+                        server_found = True
+                        break
+                    elif 'StreamPlayer' in amp_name:
+                        logger.info('Found StreamPlayer streaming server %s (type %s, amp_serial %s) @ %s.' % (amp_name, si.type(), amp_serial, si.hostname()))
+                        self._lsl_tr_channel = 0
+                        channels += si.channel_count()
+                        ch_list = pu.lsl_channel_list(inlet)
+                        amps.append(si)
+                        server_found = True
+                        break
+                    elif 'openvibeSignal' in amp_name:
+                        logger.info('Found an Openvibe signal streaming server %s (type %s, amp_serial %s) @ %s.' % (amp_name, si.type(), amp_serial, si.hostname()))
+                        ch_list = pu.lsl_channel_list(inlet)
+                        self._lsl_tr_channel = find_event_channel(ch_names=ch_list)
+                        channels += si.channel_count()
+                        amps.append(si)
+                        server_found = True
+                        # OpenVibe standard unit is Volts, which is not ideal for some numerical computations
+                        self.multiplier = 10**6 # change V -> uV unit for OpenVibe sources
+                        break
+                    elif 'openvibeMarkers' in amp_name:
+                        logger.info('Found an Openvibe markers server %s (type %s, amp_serial %s) @ %s.' % (amp_name, si.type(), amp_serial, si.hostname()))
+                        ch_list = pu.lsl_channel_list(inlet)
+                        self._lsl_tr_channel = find_event_channel(ch_names=ch_list)
+                        channels += si.channel_count()
+                        amps.append(si)
+                        server_found = True
+                        break
+                    elif find_any:
+                        logger.info('Found a streaming server %s (type %s, amp_serial %s) @ %s.' % (amp_name, si.type(), amp_serial, si.hostname()))
+                        ch_list = pu.lsl_channel_list(inlet)
+                        self._lsl_tr_channel = find_event_channel(ch_names=ch_list)
+                        channels += si.channel_count()
+                        amps.append(si)
+                        server_found = True
+                        break
+            time.sleep(1)
+
+        self.amp_name = amp_name
+
+        # define EEG channel indices
+        self._lsl_eeg_channels = list(range(channels))
+        if self._lsl_tr_channel is None:
+            logger.warning('Trigger channel not fonud. Adding an empty channel 0.')
+        else:
+            if self._lsl_tr_channel != 0:
+                logger.info('Trigger channel found at index %d. Moving to index 0.' % self._lsl_tr_channel)
+            self._lsl_eeg_channels.pop(self._lsl_tr_channel)
+        self._lsl_eeg_channels = np.array(self._lsl_eeg_channels)
+        self.tr_channel = 0  # trigger channel is always set to 0.
+        self.eeg_channels = np.arange(1, channels)  # signal channels start from 1.
+
+        # create new inlets to read from the stream
+        inlets_master = []
+        inlets_slaves = []
+        for amp in amps:
+            # data type of the 2nd argument (max_buflen) is int according to LSL C++ specification!
+            inlet = pylsl.StreamInlet(amp, max_buflen=self.stream_bufsec)
+            inlets_master.append(inlet)
+            self.buffers.append([])
+            self.timestamps.append([])
+
+        inlets = inlets_master + inlets_slaves
+        sample_rate = amps[0].nominal_srate()
+        logger.info('Channels: %d' % channels)
+        logger.info('LSL Protocol version: %s' % amps[0].version())
+        logger.info('Source sampling rate: %.1f' % sample_rate)
+        logger.info('Unit multiplier: %.1f' % self.multiplier)
+
+        #self.winsize = int(self.winsec * sample_rate)
+        #self.bufsize = int(self.bufsec * sample_rate)
+        self.winsize = int(round(self.winsec * sample_rate))
+        self.bufsize = int(round(self.bufsec * sample_rate))
+        self.stream_bufsize = int(round(self.stream_bufsec * sample_rate))
+        self.sample_rate = sample_rate
+        self.connected = True
+        self.ch_list = ch_list
+        self.inlets = inlets  # Note: not picklable!
+
+        # TODO: check if there's any problem with multiple inlets
+        if len(self.inlets) > 1:
+            logger.warning('Merging of multiple acquisition servers is not supported yet. Only %s will be used.' % amps[0].name())
+            '''
+            for i in range(1, len(self.inlets)):
+                chunk, tslist = self.inlets[i].pull_chunk(max_samples=self.stream_bufsize)
+                self.buffers[i].extend(chunk)
+                self.timestamps[i].extend(tslist)
+                if self.bufsize > 0 and len(self.buffers[i]) > self.bufsize:
+                    self.buffers[i] = self.buffers[i][-self.bufsize:]
+            '''
+
+        # create channel info
+        if self._lsl_tr_channel is None:
+            self.ch_list = ['TRIGGER'] + self.ch_list
+        else:
+            for i, chn in enumerate(self.ch_list):
+                if chn == 'TRIGGER' or chn == 'TRG' or 'STI ' in chn:
+                    self.ch_list.pop(i)
+                    self.ch_list = ['TRIGGER'] + self.ch_list
+                    break
+        logger.info('self.ch_list %s' % self.ch_list)
+
+        # fill in initial buffer
+        logger.info('Waiting to fill initial buffer of length %d' % (self.winsize))
+        while len(self.timestamps[0]) < self.winsize:
+            self.acquire()
+            time.sleep(0.1)
+        self.ready = True
+        logger.info('Start receiving stream data.')
+
+    def acquire(self, blocking=True):
+        """
+        Reads data into buffer. It is a blocking function as default.
+
+        Fills the buffer and return the current chunk of data and timestamps.
+
+        Returns:
+            data [samples x channels], timestamps [samples]
+        """
+        timestamp_offset = False
+        if len(self.timestamps[0]) == 0:
+            timestamp_offset = True
+
+        self.watchdog.reset()
+        tslist = []
+        received = False
+        chunk = None
+        while not received:
+            while self.watchdog.sec() < 5:
+                # chunk = [frames]x[ch], tslist = [frames]
+                if len(tslist) == 0:
+                    chunk, tslist = self.inlets[0].pull_chunk(max_samples=self.stream_bufsize)
+                    if blocking == False and len(tslist) == 0:
+                        return np.empty((0, len(self.ch_list))), []
+                if len(tslist) > 0:
+                    if timestamp_offset is True:
+                        lsl_clock = pylsl.local_clock()
+                    received = True
+                    break
+                time.sleep(0.0005)
+            else:
+                logger.warning('Timeout occurred while acquiring data. Amp driver bug?')
+                # give up and return empty values to avoid deadlock
+                return np.empty((0, len(self.ch_list))), []
+        data = np.array(chunk)
+
+        # BioSemi has pull-up resistor instead of pull-down
+        if self.amp_name == 'BioSemi' and self._lsl_tr_channel is not None:
+            datatype = data.dtype
+            data[:, self._lsl_tr_channel] = (np.bitwise_and(255, data[:, self._lsl_tr_channel].astype(int)) - 1).astype(datatype)
+
+        # multiply values (to change unit)
+        if self.multiplier != 1:
+            data[:, self._lsl_eeg_channels] *= self.multiplier
+
+        if self._lsl_tr_channel is not None:
+            # move trigger channel to 0 and add back to the buffer
+            data = np.concatenate((data[:, self._lsl_tr_channel].reshape(-1, 1),
+                                   data[:, self._lsl_eeg_channels]), axis=1)
+        else:
+            # add an empty channel with zeros to channel 0
+            data = np.concatenate((np.zeros((data.shape[0],1)),
+                                   data[:, self._lsl_eeg_channels]), axis=1)
+
+        # add data to buffer
+        chunk = data.tolist()
+        self.buffers[0].extend(chunk)
+        self.timestamps[0].extend(tslist)
+        if self.bufsize > 0 and len(self.timestamps[0]) > self.bufsize:
+            self.buffers[0] = self.buffers[0][-self.bufsize:]
+            self.timestamps[0] = self.timestamps[0][-self.bufsize:]
+
+        if timestamp_offset is True:
+            timestamp_offset = False
+            logger.info('LSL timestamp = %s' % lsl_clock)
+            logger.info('Server timestamp = %s' % self.timestamps[-1][-1])
+            self.lsl_time_offset = self.timestamps[-1][-1] - lsl_clock
+            logger.info('Offset = %.3f ' % (self.lsl_time_offset))
+            if abs(self.lsl_time_offset) > 0.1:
+                logger.warning('LSL server has a high timestamp offset.')
+            else:
+                logger.info_green('LSL time server synchronized')
+
+        ''' TODO: test the merging of multiple streams
+        # if we have multiple synchronized amps
+        if len(self.inlets) > 1:
+            for i in range(1, len(self.inlets)):
+                chunk, tslist = self.inlets[i].pull_chunk(max_samples=len(tslist))  # [frames][channels]
+                self.buffers[i].extend(chunk)
+                self.timestamps[i].extend(tslist)
+                if self.bufsize > 0 and len(self.buffers[i]) > self.bufsize:
+                    self.buffers[i] = self.buffers[i][-self.bufsize:]
+        '''
+
+        # data= array[samples, channels], tslist=[samples]
+        return (data, tslist)
+
+    def check_connect(self):
+        """
+        Check connection and automatically connect if not connected
+        """
+        while not self.connected:
+            logger.error('LSL server not connected yet. Trying to connect automatically.')
+            self.connect()
+            time.sleep(1)
+
+    def set_window_size(self, window_size):
+        """
+        Set window size (in seconds)
+        """
+        self.check_connect()
+        #self.winsize = int(window_size * self.sample_rate) + 1
+        self.winsize = int(round(window_size * self.sample_rate)) + 1
+
+    def get_channel_names(self):
+        """
+        Get a list of channels
+        """
+        return self.ch_list
+
+    def get_window_list(self):
+        """
+        Get the latest window
+        IT ONLY RETURNS list[amps][samples][channels]
+        """
+        self.check_connect()
+        window = self.buffers[0][-self.winsize:]
+        timestamps = self.timestamps[0][-self.winsize:]
+        return window, timestamps
+
+    def get_window(self, decim=1):
+        """
+        Get the latest window and timestamps in numpy format
+
+        input
+        -----
+        decim (int): decimation factor
+
+        output
+        ------
+        [samples x channels], [samples]
+        """
+        self.check_connect()
+        window, timestamps = self.get_window_list()
+
+        if len(timestamps) > 0:
+            # window = array[[samples_ch1],[samples_ch2]...]
+            return np.array(window), np.array(timestamps)
+        else:
+            return np.array([]), np.array([])
+
+    def get_buffer_list(self):
+        """
+        Get entire buffer
+        Returns the raw list: amps x samples x channels
+        """
+        self.check_connect()
+        return self.buffers, self.timestamps
+
+    def get_buffer(self):
+        """
+        Returns the entire buffer: samples x channels
+
+        If multiple amps, signals are concatenated along the channel axis.
+        """
+        self.check_connect()
+        try:
+            if len(self.timestamps[0]) > 0:
+                w = np.concatenate(self.buffers, axis=1) # samples x channels
+                t = np.array(self.timestamps).reshape(-1, 1) # samples x 1
+                return w, t
+            else:
+                return np.array([]), np.array([])
+        except:
+            logger.exception('Sorry! Unexpected error occurred in get_buffer(). Dropping into a shell for debugging.')
+            pdb.pm()
+
+    def get_buflen(self):
+        """
+        Return buffer length in seconds
+        """
+        return (len(self.timestamps[0]) / self.sample_rate)
+
+    def get_sample_rate(self):
+        """
+        Sampling rate
+        """
+        return self.sample_rate
+
+    def get_num_channels(self):
+        """
+        Total number of channels includingi trigger channel
+        """
+        return len(self.ch_list)
+
+    def get_eeg_channels(self):
+        """
+        Returns indices of eeg channels excluding trigger channel
+        """
+        return self.eeg_channels
+
+    def get_trigger_channel(self):
+        """
+        Return trigger channel (0-based index)
+        """
+        return self.tr_channel
+
+    def get_lsl_offset(self):
+        """
+        Return time difference of acquisition server's time and LSL time
+
+        OpenVibe servers often have a bug of sending its own running time instead of LSL time.
+        """
+        return self.lsl_time_offset
+
+    def reset_buffer(self):
+        """
+        Clear buffers
+        """
+        self.buffers = []
+
+    def is_ready(self):
+        """
+        Returns True if the buffer is not empty.
+        """
+        return self.ready
+
+
+"""
+Example code for printing out raw values
+"""
+def test_receiver():
+    import mne
+    import os
+
+    CH_INDEX = [1] # channel to monitor
+    TIME_INDEX = None # integer or None. None = average of raw values of the current window
+    SHOW_PSD = False
+    mne.set_log_level('ERROR')
+    os.environ['OMP_NUM_THREADS'] = '1' # actually improves performance for multitaper
+
+    # connect to LSL server
+    amp_name, amp_serial = pu.search_lsl()
+    sr = StreamReceiver(window_size=1, buffer_size=1, amp_serial=amp_serial, eeg_only=False, amp_name=amp_name)
+    sfreq = sr.get_sample_rate()
+    trg_ch = sr.get_trigger_channel()
+    logger.info('Trigger channel = %d' % trg_ch)
+
+    # PSD init
+    if SHOW_PSD:
+        psde = mne.decoding.PSDEstimator(sfreq=sfreq, fmin=1, fmax=50, bandwidth=None, \
+            adaptive=False, low_bias=True, n_jobs=1, normalization='length', verbose=None)
+
+    watchdog = qc.Timer()
+    tm = qc.Timer(autoreset=True)
+    last_ts = 0
+    while True:
+        sr.acquire()
+        window, tslist = sr.get_window() # window = [samples x channels]
+        window = window.T # chanel x samples
+
+        qc.print_c('LSL Diff = %.3f' % (pylsl.local_clock() - tslist[-1]), 'G')
+
+        # print event values
+        tsnew = np.where(np.array(tslist) > last_ts)[0]
+        if len(tsnew) == 0:
+            logger.warning('There seems to be delay in receiving data.')
+            time.sleep(1)
+            continue
+        trigger = np.unique(window[trg_ch, tsnew[0]:])
+
+        # for Biosemi
+        # if sr.amp_name=='BioSemi':
+        #    trigger= set( [255 & int(x-1) for x in trigger ] )
+
+        if len(trigger) > 0:
+            logger.info('Triggers: %s' % np.array(trigger))
+
+        logger.info('[%.1f] Receiving data...' % watchdog.sec())
+
+        if TIME_INDEX is None:
+            datatxt = qc.list2string(np.mean(window[CH_INDEX, :], axis=1), '%-15.6f')
+            print('[%.3f : %.3f]' % (tslist[0], tslist[-1]) + ' data: %s' % datatxt)
+        else:
+            datatxt = qc.list2string(window[CH_INDEX, TIME_INDEX], '%-15.6f')
+            print('[%.3f]' % tslist[TIME_INDEX] + ' data: %s' % datatxt)
+
+        # show PSD
+        if SHOW_PSD:
+            psd = psde.transform(window.reshape((1, window.shape[0], window.shape[1])))
+            psd = psd.reshape((psd.shape[1], psd.shape[2]))
+            psdmean = np.mean(psd, axis=1)
+            for p in psdmean:
+                print('%.1f' % p, end=' ')
+
+        last_ts = tslist[-1]
+        tm.sleep_atleast(0.05)
+
+if __name__ == '__main__':
+    test_receiver()
```

### Comparing `neurodecode-2.0.4/neurodecode/stream_recorder/stream_recorder.py` & `neurodecode-2.0.5/neurodecode/stream_recorder/stream_recorder.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-from __future__ import print_function, division
-
-"""
-stream_receiver.py
-Acquires signals from LSL server and save into buffer.
-Command-line arguments:
-  #1: AMP_NAME
-  #2: AMP_SERIAL (can be omitted if no serial number available)
-  If no argument is supplied, you will be prompted to select one
-  from a list of available LSL servers.
-Example:
-  python stream_recorder.py openvibeSignals
-TODO:
-- Support HDF output.
-- Write simulatenously while receivng data.
-- Support multiple amps.
-Kyuhwa Lee, 2014
-Swiss Federal Institute of Technology Lausanne (EPFL)
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import os
-import sys
-import time
-import datetime
-import numpy as np
-import multiprocessing as mp
-import neurodecode.utils.add_lsl_events
-import neurodecode.utils.q_common as qc
-import neurodecode.utils.pycnbi_utils as pu
-from neurodecode.utils.convert2fif import pcl2fif
-from neurodecode.utils.nd_lsl import start_server
-from neurodecode.stream_receiver.stream_receiver import StreamReceiver
-from neurodecode import logger
-from builtins import input
-
-
-def record(record_state, amp_name, amp_serial, record_dir, eeg_only, recordLogger=logger):
-    # set data file name
-    timestamp = time.strftime('%Y%m%d-%H%M%S', time.localtime())
-    pcl_file = "%s/%s-raw.pcl" % (record_dir, timestamp)
-    eve_file = '%s/%s-eve.txt' % (record_dir, timestamp)
-    recordLogger.info('>> Output file: %s' % (pcl_file))
-
-    # test writability
-    try:
-        qc.make_dirs(record_dir)
-        open(pcl_file, 'w').write('The data will written when the recording is finished.')
-    except:
-        raise RuntimeError('Problem writing to %s. Check permission.' % pcl_file)
-
-    # start a server for sending out data pcl_file when software trigger is used
-    outlet = start_server('StreamRecorderInfo', channel_format='string',\
-        source_id=eve_file, stype='Markers')
-
-    # connect to EEG stream server
-    sr = StreamReceiver(buffer_size=0, amp_name=amp_name, amp_serial=amp_serial, eeg_only=eeg_only)
-
-    # start recording
-    recordLogger.info('\n>> Recording started (PID %d).' % os.getpid())
-    qc.print_c('\n>> Press Enter to stop recording', 'G')
-    tm = qc.Timer(autoreset=True)
-    next_sec = 1
-    while record_state.value == 1:
-        sr.acquire()
-        if sr.get_buflen() > next_sec:
-            duration = str(datetime.timedelta(seconds=int(sr.get_buflen())))
-            recordLogger.info('RECORDING %s' % duration)
-            next_sec += 1
-        tm.sleep_atleast(0.001)
-
-    # record stop
-    recordLogger.info('>> Stop requested. Copying buffer')
-    buffers, times = sr.get_buffer()
-    signals = buffers
-    events = None
-
-    # channels = total channels from amp, including trigger channel
-    data = {'signals':signals, 'timestamps':times, 'events':events,
-            'sample_rate':sr.get_sample_rate(), 'channels':sr.get_num_channels(),
-            'ch_names':sr.get_channel_names(), 'lsl_time_offset':sr.lsl_time_offset}
-    recordLogger.info('Saving raw data ...')
-    qc.save_obj(pcl_file, data)
-    recordLogger.info('Saved to %s\n' % pcl_file)
-
-    # automatically convert to fif and use event file if it exists (software trigger)
-    if os.path.exists(eve_file):
-        recordLogger.info('Found matching event file, adding events.')
-    else:
-        eve_file = None
-    recordLogger.info('Converting raw file into fif.')
-    pcl2fif(pcl_file, external_event=eve_file)
-
-def run(record_dir, amp_name, amp_serial, eeg_only=False):
-    recordLogger = logger
-    recordLogger.info('\nOutput directory: %s' % (record_dir))
-
-    # spawn the recorder as a child process
-    recordLogger.info('\n>> Press Enter to start recording.')
-    key = input()
-    record_state = mp.Value('i', 1)
-    proc = mp.Process(target=record, args=[record_state, amp_name, amp_serial, record_dir, eeg_only])
-    proc.start()
-
-    # clean up
-    time.sleep(1) # required on some Python distribution
-    input()
-    record_state.value = 0
-    recordLogger.info('(main) Waiting for recorder process to finish.')
-    proc.join(10)
-    if proc.is_alive():
-        recordLogger.error('Recorder process not finishing. Are you running from Spyder?')
-        recordLogger.error('Dropping into a shell')
-        qc.shell()
-    sys.stdout.flush()
-    recordLogger.info('Recording finished.')
-
-# for batch script
-def batch_run(record_dir=None, amp_name=None, amp_serial=None):
-    # configure LSL server name and device serial if available
-    if not record_dir:
-        record_dir = '%s/records' % os.path.expanduser('~')
-    if not amp_name:
-        amp_name, amp_serial = pu.search_lsl(ignore_markers=True)
-    run(record_dir, amp_name=amp_name, amp_serial=amp_serial)
-
-# backup: for invoking from GUI
-def run_gui(record_state, protocolState, record_dir, recordLogger=logger, amp_name=None, amp_serial=None, eeg_only=False):
-    # configure LSL server name and device serial if available
-    if not amp_name:
-        amp_name, amp_serial = pu.search_lsl(record_state, recordLogger, ignore_markers=True)
-
-    recordLogger.info('\nOutput directory: %s' % (record_dir))
-
-    # spawn the recorder as a child process
-    recordLogger.info('\n>> Recording started.')
-    proc = mp.Process(target=record, args=[record_state, amp_name, amp_serial, record_dir, eeg_only, recordLogger])
-    proc.start()
-
-    # Launching the protocol (shared variable)
-    with protocolState.get_lock():
-        protocolState.value = 1
-
-    # Continue recording until the shared variable changes to 0.
-    while record_state.value:
-        time.sleep(1)
-
-    recordLogger.info('(main) Waiting for recorder process to finish.')
-    proc.join(10)
-    if proc.is_alive():
-        recordLogger.error('Recorder process not finishing. Are you running from Spyder?')
-        recordLogger.error('Dropping into a shell')
-        qc.shell()
-    sys.stdout.flush()
-    recordLogger.info('Recording finished.')
-
-def main():
-    """
-    Invoked from console
-    """
-    record_dir = None
-    amp_name = None
-    amp_serial = None
-    if len(sys.argv) > 3:
-        amp_serial = sys.argv[3]
-    if len(sys.argv) > 2:
-        amp_name = sys.argv[2]
-    if len(sys.argv) > 1:
-        record_dir = sys.argv[1]
-    batch_run(record_dir, amp_name, amp_serial)
-
-# default sample recorder
-if __name__ == '__main__':
-    main()
+from __future__ import print_function, division
+
+"""
+stream_receiver.py
+Acquires signals from LSL server and save into buffer.
+Command-line arguments:
+  #1: AMP_NAME
+  #2: AMP_SERIAL (can be omitted if no serial number available)
+  If no argument is supplied, you will be prompted to select one
+  from a list of available LSL servers.
+Example:
+  python stream_recorder.py openvibeSignals
+TODO:
+- Support HDF output.
+- Write simulatenously while receivng data.
+- Support multiple amps.
+Kyuhwa Lee, 2014
+Swiss Federal Institute of Technology Lausanne (EPFL)
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import os
+import sys
+import time
+import datetime
+import numpy as np
+import multiprocessing as mp
+import neurodecode.utils.add_lsl_events
+import neurodecode.utils.q_common as qc
+import neurodecode.utils.pycnbi_utils as pu
+from neurodecode.utils.convert2fif import pcl2fif
+from neurodecode.utils.nd_lsl import start_server
+from neurodecode.stream_receiver.stream_receiver import StreamReceiver
+from neurodecode import logger
+from builtins import input
+
+
+def record(record_state, amp_name, amp_serial, record_dir, eeg_only, recordLogger=logger):
+    # set data file name
+    timestamp = time.strftime('%Y%m%d-%H%M%S', time.localtime())
+    pcl_file = "%s/%s-raw.pcl" % (record_dir, timestamp)
+    eve_file = '%s/%s-eve.txt' % (record_dir, timestamp)
+    recordLogger.info('>> Output file: %s' % (pcl_file))
+
+    # test writability
+    try:
+        qc.make_dirs(record_dir)
+        open(pcl_file, 'w').write('The data will written when the recording is finished.')
+    except:
+        raise RuntimeError('Problem writing to %s. Check permission.' % pcl_file)
+
+    # start a server for sending out data pcl_file when software trigger is used
+    outlet = start_server('StreamRecorderInfo', channel_format='string',\
+        source_id=eve_file, stype='Markers')
+
+    # connect to EEG stream server
+    sr = StreamReceiver(buffer_size=0, amp_name=amp_name, amp_serial=amp_serial, eeg_only=eeg_only)
+
+    # start recording
+    recordLogger.info('\n>> Recording started (PID %d).' % os.getpid())
+    qc.print_c('\n>> Press Enter to stop recording', 'G')
+    tm = qc.Timer(autoreset=True)
+    next_sec = 1
+    while record_state.value == 1:
+        sr.acquire()
+        if sr.get_buflen() > next_sec:
+            duration = str(datetime.timedelta(seconds=int(sr.get_buflen())))
+            recordLogger.info('RECORDING %s' % duration)
+            next_sec += 1
+        tm.sleep_atleast(0.001)
+
+    # record stop
+    recordLogger.info('>> Stop requested. Copying buffer')
+    buffers, times = sr.get_buffer()
+    signals = buffers
+    events = None
+
+    # channels = total channels from amp, including trigger channel
+    data = {'signals':signals, 'timestamps':times, 'events':events,
+            'sample_rate':sr.get_sample_rate(), 'channels':sr.get_num_channels(),
+            'ch_names':sr.get_channel_names(), 'lsl_time_offset':sr.lsl_time_offset}
+    recordLogger.info('Saving raw data ...')
+    qc.save_obj(pcl_file, data)
+    recordLogger.info('Saved to %s\n' % pcl_file)
+
+    # automatically convert to fif and use event file if it exists (software trigger)
+    if os.path.exists(eve_file):
+        recordLogger.info('Found matching event file, adding events.')
+    else:
+        eve_file = None
+    recordLogger.info('Converting raw file into fif.')
+    pcl2fif(pcl_file, external_event=eve_file)
+
+def run(record_dir, amp_name, amp_serial, eeg_only=False):
+    recordLogger = logger
+    recordLogger.info('\nOutput directory: %s' % (record_dir))
+
+    # spawn the recorder as a child process
+    recordLogger.info('\n>> Press Enter to start recording.')
+    key = input()
+    record_state = mp.Value('i', 1)
+    proc = mp.Process(target=record, args=[record_state, amp_name, amp_serial, record_dir, eeg_only])
+    proc.start()
+
+    # clean up
+    time.sleep(1) # required on some Python distribution
+    input()
+    record_state.value = 0
+    recordLogger.info('(main) Waiting for recorder process to finish.')
+    proc.join(10)
+    if proc.is_alive():
+        recordLogger.error('Recorder process not finishing. Are you running from Spyder?')
+        recordLogger.error('Dropping into a shell')
+        qc.shell()
+    sys.stdout.flush()
+    recordLogger.info('Recording finished.')
+
+# for batch script
+def batch_run(record_dir=None, amp_name=None, amp_serial=None):
+    # configure LSL server name and device serial if available
+    if not record_dir:
+        record_dir = '%s/records' % os.path.expanduser('~')
+    if not amp_name:
+        amp_name, amp_serial = pu.search_lsl(ignore_markers=True)
+    run(record_dir, amp_name=amp_name, amp_serial=amp_serial)
+
+# backup: for invoking from GUI
+def run_gui(record_state, protocolState, record_dir, recordLogger=logger, amp_name=None, amp_serial=None, eeg_only=False):
+    # configure LSL server name and device serial if available
+    if not amp_name:
+        amp_name, amp_serial = pu.search_lsl(record_state, recordLogger, ignore_markers=True)
+
+    recordLogger.info('\nOutput directory: %s' % (record_dir))
+
+    # spawn the recorder as a child process
+    recordLogger.info('\n>> Recording started.')
+    proc = mp.Process(target=record, args=[record_state, amp_name, amp_serial, record_dir, eeg_only, recordLogger])
+    proc.start()
+
+    # Launching the protocol (shared variable)
+    with protocolState.get_lock():
+        protocolState.value = 1
+
+    # Continue recording until the shared variable changes to 0.
+    while record_state.value:
+        time.sleep(1)
+
+    recordLogger.info('(main) Waiting for recorder process to finish.')
+    proc.join(10)
+    if proc.is_alive():
+        recordLogger.error('Recorder process not finishing. Are you running from Spyder?')
+        recordLogger.error('Dropping into a shell')
+        qc.shell()
+    sys.stdout.flush()
+    recordLogger.info('Recording finished.')
+
+def main():
+    """
+    Invoked from console
+    """
+    record_dir = None
+    amp_name = None
+    amp_serial = None
+    if len(sys.argv) > 3:
+        amp_serial = sys.argv[3]
+    if len(sys.argv) > 2:
+        amp_name = sys.argv[2]
+    if len(sys.argv) > 1:
+        record_dir = sys.argv[1]
+    batch_run(record_dir, amp_name, amp_serial)
+
+# default sample recorder
+if __name__ == '__main__':
+    main()
```

### Comparing `neurodecode-2.0.4/neurodecode/stream_viewer/scope_settings.ini` & `neurodecode-2.0.5/neurodecode/stream_viewer/scope_settings.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,96 @@
-00000000: 5b70 6c6f 745d 0a23 2053 6361 6c65 2028  [plot].# Scale (
-00000010: 7556 290a 7363 616c 655f 706c 6f74 203d  uV).scale_plot =
-00000020: 2033 300a 2320 5469 6d65 2028 7329 0a74   30.# Time (s).t
-00000030: 696d 655f 706c 6f74 203d 2031 300a 2320  ime_plot = 10.# 
-00000040: 5368 6f77 2054 6944 2065 7665 6e74 733f  Show TiD events?
-00000050: 0a73 686f 775f 5449 445f 6576 656e 7473  .show_TID_events
-00000060: 203d 2030 0a23 2053 686f 7720 4c50 5420   = 0.# Show LPT 
-00000070: 6576 656e 7473 3f0a 7368 6f77 5f4c 5054  events?.show_LPT
-00000080: 5f65 7665 6e74 7320 3d20 310a 2320 5368  _events = 1.# Sh
-00000090: 6f77 2028 616e 6420 7265 636f 7264 2920  ow (and record) 
-000000a0: 4b65 7920 6576 656e 7473 3f0a 7368 6f77  Key events?.show
-000000b0: 5f4b 4559 5f65 7665 6e74 7320 3d20 310a  _KEY_events = 1.
-000000c0: 0a5b 6669 6c74 6572 696e 675d 0a61 7070  .[filtering].app
-000000d0: 6c79 5f63 6172 5f66 696c 7465 7220 3d20  ly_car_filter = 
-000000e0: 310a 6170 706c 795f 6261 6e64 7061 7373  1.apply_bandpass
-000000f0: 5f66 696c 7465 7220 3d20 310a 2320 5b68  _filter = 1.# [h
-00000100: 6920 6c6f 5d20 666f 726d 6174 2e20 4361  i lo] format. Ca
-00000110: 6e20 6265 2066 6c6f 6174 730a 6261 6e64  n be floats.band
-00000120: 7061 7373 5f63 7574 6f66 665f 6672 6571  pass_cutoff_freq
-00000130: 7565 6e63 7920 3d20 3120 3430 0a0a 0a5b  uency = 1 40...[
-00000140: 696e 7465 726e 616c 5d0a 2320 5061 7468  internal].# Path
-00000150: 2074 6f20 7069 7065 0a70 6174 685f 7069   to pipe.path_pi
-00000160: 7065 203d 202f 746d 702f 636c 2e70 6970  pe = /tmp/cl.pip
-00000170: 652e 6e64 662e 3130 0a23 2053 686f 7720  e.ndf.10.# Show 
-00000180: 6368 616e 6e65 6c20 6e61 6d65 7320 696e  channel names in
-00000190: 7374 6561 6420 6f66 206e 756d 6265 7273  stead of numbers
-000001a0: 3f0a 7368 6f77 5f63 6861 6e6e 656c 5f6e  ?.show_channel_n
-000001b0: 616d 6573 203d 2031 0a23 2043 6861 6e6e  ames = 1.# Chann
-000001c0: 656c 206e 616d 6573 2066 6f72 2065 6163  el names for eac
-000001d0: 6820 616d 706c 6966 6965 722e 2053 686f  h amplifier. Sho
-000001e0: 756c 6420 6265 2073 6570 6172 6174 6564  uld be separated
-000001f0: 2062 7920 7468 6520 7374 7269 6e67 2022   by the string "
-00000200: 2c20 220a 6368 616e 6e65 6c5f 6e61 6d65  , ".channel_name
-00000210: 735f 6774 6563 3136 203d 2046 7a2c 2046  s_gtec16 = Fz, F
-00000220: 4333 2c20 4643 312c 2046 437a 2c20 4643  C3, FC1, FCz, FC
-00000230: 322c 2046 4334 2c20 4333 2c20 4331 2c20  2, FC4, C3, C1, 
-00000240: 437a 2c20 4332 2c20 4334 2c20 4350 332c  Cz, C2, C4, CP3,
-00000250: 2043 5031 2c20 4350 7a2c 2043 5032 2c20   CP1, CPz, CP2, 
-00000260: 4350 340a 6368 616e 6e65 6c5f 6e61 6d65  CP4.channel_name
-00000270: 735f 6774 6563 3332 203d 2046 7a2c 2046  s_gtec32 = Fz, F
-00000280: 4333 2c20 4643 312c 2046 437a 2c20 4643  C3, FC1, FCz, FC
-00000290: 322c 2046 4334 2c20 4333 2c20 4331 2c20  2, FC4, C3, C1, 
-000002a0: 437a 2c20 4332 2c20 4334 2c20 4350 332c  Cz, C2, C4, CP3,
-000002b0: 2043 5031 2c20 4350 7a2c 2043 5032 2c20   CP1, CPz, CP2, 
-000002c0: 4350 342c 2031 372c 2031 382c 2031 392c  CP4, 17, 18, 19,
-000002d0: 2032 302c 2032 312c 2032 322c 2032 332c   20, 21, 22, 23,
-000002e0: 2032 342c 2032 352c 2032 362c 2032 372c   24, 25, 26, 27,
-000002f0: 2032 382c 2032 392c 2033 302c 2033 312c   28, 29, 30, 31,
-00000300: 2033 320a 6368 616e 6e65 6c5f 6e61 6d65   32.channel_name
-00000310: 735f 6269 6f73 656d 6936 3420 3d20 4670  s_biosemi64 = Fp
-00000320: 312c 2041 4637 2c20 4146 332c 2046 312c  1, AF7, AF3, F1,
-00000330: 2046 332c 2046 352c 2046 372c 2046 5437   F3, F5, F7, FT7
-00000340: 2c20 4643 352c 2046 4333 2c20 4643 312c  , FC5, FC3, FC1,
-00000350: 2043 312c 2043 332c 2043 352c 2054 372c   C1, C3, C5, T7,
-00000360: 2054 5037 2c20 4350 352c 2043 5033 2c20   TP7, CP5, CP3, 
-00000370: 4350 312c 2050 312c 2050 332c 2050 352c  CP1, P1, P3, P5,
-00000380: 2050 372c 2050 392c 2050 4f37 2c20 504f   P7, P9, PO7, PO
-00000390: 332c 204f 312c 2049 7a2c 204f 7a2c 2050  3, O1, Iz, Oz, P
-000003a0: 4f7a 2c20 507a 2c20 4350 7a2c 2046 707a  Oz, Pz, CPz, Fpz
-000003b0: 2c20 4670 322c 2041 4638 2c20 4146 342c  , Fp2, AF8, AF4,
-000003c0: 2041 467a 2c20 467a 2c20 4632 2c20 4634   AFz, Fz, F2, F4
-000003d0: 2c20 4636 2c20 4638 2c20 4654 382c 2046  , F6, F8, FT8, F
-000003e0: 4336 2c20 4643 342c 2046 4332 2c20 4643  C6, FC4, FC2, FC
-000003f0: 7a2c 2043 7a2c 2043 322c 2043 342c 2043  z, Cz, C2, C4, C
-00000400: 362c 2054 382c 2054 5038 2c20 4350 362c  6, T8, TP8, CP6,
-00000410: 2043 5034 2c20 4350 322c 2050 322c 2050   CP4, CP2, P2, P
-00000420: 342c 2050 362c 2050 382c 2050 3130 2c20  4, P6, P8, P10, 
-00000430: 504f 382c 2050 4f34 2c20 4f32 0a63 6861  PO8, PO4, O2.cha
-00000440: 6e6e 656c 5f6e 616d 6573 5f68 6961 6d70  nnel_names_hiamp
-00000450: 3634 203d 2046 7031 2c20 4146 372c 2041  64 = Fp1, AF7, A
-00000460: 4633 2c20 4631 2c20 4633 2c20 4635 2c20  F3, F1, F3, F5, 
-00000470: 4637 2c20 4654 372c 2046 4335 2c20 4643  F7, FT7, FC5, FC
-00000480: 332c 2046 4331 2c20 4331 2c20 4333 2c20  3, FC1, C1, C3, 
-00000490: 4335 2c20 5437 2c20 5450 372c 2043 5035  C5, T7, TP7, CP5
-000004a0: 2c20 4350 332c 2043 5031 2c20 5031 2c20  , CP3, CP1, P1, 
-000004b0: 5033 2c20 5035 2c20 5037 2c20 5039 2c20  P3, P5, P7, P9, 
-000004c0: 504f 372c 2050 4f33 2c20 4f31 2c20 497a  PO7, PO3, O1, Iz
-000004d0: 2c20 4f7a 2c20 504f 7a2c 2050 7a2c 2043  , Oz, POz, Pz, C
-000004e0: 507a 2c20 4670 7a2c 2046 7032 2c20 4146  Pz, Fpz, Fp2, AF
-000004f0: 382c 2041 4634 2c20 4146 7a2c 2046 7a2c  8, AF4, AFz, Fz,
-00000500: 2046 322c 2046 342c 2046 362c 2046 382c   F2, F4, F6, F8,
-00000510: 2046 5438 2c20 4643 362c 2046 4334 2c20   FT8, FC6, FC4, 
-00000520: 4643 322c 2046 437a 2c20 437a 2c20 4332  FC2, FCz, Cz, C2
-00000530: 2c20 4334 2c20 4336 2c20 5438 2c20 5450  , C4, C6, T8, TP
-00000540: 382c 2043 5036 2c20 4350 342c 2043 5032  8, CP6, CP4, CP2
-00000550: 2c20 5032 2c20 5034 2c20 5036 2c20 5038  , P2, P4, P6, P8
-00000560: 2c20 5031 302c 2050 4f38 2c20 504f 342c  , P10, PO8, PO4,
-00000570: 204f 320a 0a63 6861 6e6e 656c 5f6e 616d   O2..channel_nam
-00000580: 6573 5f67 7465 6331 3720 3d20 467a 2c20  es_gtec17 = Fz, 
-00000590: 4643 332c 2046 4331 2c20 4643 7a2c 2046  FC3, FC1, FCz, F
-000005a0: 4332 2c20 4643 342c 2043 332c 2043 312c  C2, FC4, C3, C1,
-000005b0: 2043 7a2c 2043 322c 2043 342c 2043 5033   Cz, C2, C4, CP3
-000005c0: 2c20 4350 312c 2043 507a 2c20 4350 322c  , CP1, CPz, CP2,
-000005d0: 2043 5034 2c20 5452 4947 4745 520a        CP4, TRIGGER.
+00000000: 5b70 6c6f 745d 0d0a 2320 5363 616c 6520  [plot]..# Scale 
+00000010: 2875 5629 0d0a 7363 616c 655f 706c 6f74  (uV)..scale_plot
+00000020: 203d 2033 300d 0a23 2054 696d 6520 2873   = 30..# Time (s
+00000030: 290d 0a74 696d 655f 706c 6f74 203d 2031  )..time_plot = 1
+00000040: 300d 0a23 2053 686f 7720 5469 4420 6576  0..# Show TiD ev
+00000050: 656e 7473 3f0d 0a73 686f 775f 5449 445f  ents?..show_TID_
+00000060: 6576 656e 7473 203d 2030 0d0a 2320 5368  events = 0..# Sh
+00000070: 6f77 204c 5054 2065 7665 6e74 733f 0d0a  ow LPT events?..
+00000080: 7368 6f77 5f4c 5054 5f65 7665 6e74 7320  show_LPT_events 
+00000090: 3d20 310d 0a23 2053 686f 7720 2861 6e64  = 1..# Show (and
+000000a0: 2072 6563 6f72 6429 204b 6579 2065 7665   record) Key eve
+000000b0: 6e74 733f 0d0a 7368 6f77 5f4b 4559 5f65  nts?..show_KEY_e
+000000c0: 7665 6e74 7320 3d20 310d 0a0d 0a5b 6669  vents = 1....[fi
+000000d0: 6c74 6572 696e 675d 0d0a 6170 706c 795f  ltering]..apply_
+000000e0: 6361 725f 6669 6c74 6572 203d 2031 0d0a  car_filter = 1..
+000000f0: 6170 706c 795f 6261 6e64 7061 7373 5f66  apply_bandpass_f
+00000100: 696c 7465 7220 3d20 310d 0a23 205b 6869  ilter = 1..# [hi
+00000110: 206c 6f5d 2066 6f72 6d61 742e 2043 616e   lo] format. Can
+00000120: 2062 6520 666c 6f61 7473 0d0a 6261 6e64   be floats..band
+00000130: 7061 7373 5f63 7574 6f66 665f 6672 6571  pass_cutoff_freq
+00000140: 7565 6e63 7920 3d20 3120 3430 0d0a 0d0a  uency = 1 40....
+00000150: 0d0a 5b69 6e74 6572 6e61 6c5d 0d0a 2320  ..[internal]..# 
+00000160: 5061 7468 2074 6f20 7069 7065 0d0a 7061  Path to pipe..pa
+00000170: 7468 5f70 6970 6520 3d20 2f74 6d70 2f63  th_pipe = /tmp/c
+00000180: 6c2e 7069 7065 2e6e 6466 2e31 300d 0a23  l.pipe.ndf.10..#
+00000190: 2053 686f 7720 6368 616e 6e65 6c20 6e61   Show channel na
+000001a0: 6d65 7320 696e 7374 6561 6420 6f66 206e  mes instead of n
+000001b0: 756d 6265 7273 3f0d 0a73 686f 775f 6368  umbers?..show_ch
+000001c0: 616e 6e65 6c5f 6e61 6d65 7320 3d20 310d  annel_names = 1.
+000001d0: 0a23 2043 6861 6e6e 656c 206e 616d 6573  .# Channel names
+000001e0: 2066 6f72 2065 6163 6820 616d 706c 6966   for each amplif
+000001f0: 6965 722e 2053 686f 756c 6420 6265 2073  ier. Should be s
+00000200: 6570 6172 6174 6564 2062 7920 7468 6520  eparated by the 
+00000210: 7374 7269 6e67 2022 2c20 220d 0a63 6861  string ", "..cha
+00000220: 6e6e 656c 5f6e 616d 6573 5f67 7465 6331  nnel_names_gtec1
+00000230: 3620 3d20 467a 2c20 4643 332c 2046 4331  6 = Fz, FC3, FC1
+00000240: 2c20 4643 7a2c 2046 4332 2c20 4643 342c  , FCz, FC2, FC4,
+00000250: 2043 332c 2043 312c 2043 7a2c 2043 322c   C3, C1, Cz, C2,
+00000260: 2043 342c 2043 5033 2c20 4350 312c 2043   C4, CP3, CP1, C
+00000270: 507a 2c20 4350 322c 2043 5034 0d0a 6368  Pz, CP2, CP4..ch
+00000280: 616e 6e65 6c5f 6e61 6d65 735f 6774 6563  annel_names_gtec
+00000290: 3332 203d 2046 7a2c 2046 4333 2c20 4643  32 = Fz, FC3, FC
+000002a0: 312c 2046 437a 2c20 4643 322c 2046 4334  1, FCz, FC2, FC4
+000002b0: 2c20 4333 2c20 4331 2c20 437a 2c20 4332  , C3, C1, Cz, C2
+000002c0: 2c20 4334 2c20 4350 332c 2043 5031 2c20  , C4, CP3, CP1, 
+000002d0: 4350 7a2c 2043 5032 2c20 4350 342c 2031  CPz, CP2, CP4, 1
+000002e0: 372c 2031 382c 2031 392c 2032 302c 2032  7, 18, 19, 20, 2
+000002f0: 312c 2032 322c 2032 332c 2032 342c 2032  1, 22, 23, 24, 2
+00000300: 352c 2032 362c 2032 372c 2032 382c 2032  5, 26, 27, 28, 2
+00000310: 392c 2033 302c 2033 312c 2033 320d 0a63  9, 30, 31, 32..c
+00000320: 6861 6e6e 656c 5f6e 616d 6573 5f62 696f  hannel_names_bio
+00000330: 7365 6d69 3634 203d 2046 7031 2c20 4146  semi64 = Fp1, AF
+00000340: 372c 2041 4633 2c20 4631 2c20 4633 2c20  7, AF3, F1, F3, 
+00000350: 4635 2c20 4637 2c20 4654 372c 2046 4335  F5, F7, FT7, FC5
+00000360: 2c20 4643 332c 2046 4331 2c20 4331 2c20  , FC3, FC1, C1, 
+00000370: 4333 2c20 4335 2c20 5437 2c20 5450 372c  C3, C5, T7, TP7,
+00000380: 2043 5035 2c20 4350 332c 2043 5031 2c20   CP5, CP3, CP1, 
+00000390: 5031 2c20 5033 2c20 5035 2c20 5037 2c20  P1, P3, P5, P7, 
+000003a0: 5039 2c20 504f 372c 2050 4f33 2c20 4f31  P9, PO7, PO3, O1
+000003b0: 2c20 497a 2c20 4f7a 2c20 504f 7a2c 2050  , Iz, Oz, POz, P
+000003c0: 7a2c 2043 507a 2c20 4670 7a2c 2046 7032  z, CPz, Fpz, Fp2
+000003d0: 2c20 4146 382c 2041 4634 2c20 4146 7a2c  , AF8, AF4, AFz,
+000003e0: 2046 7a2c 2046 322c 2046 342c 2046 362c   Fz, F2, F4, F6,
+000003f0: 2046 382c 2046 5438 2c20 4643 362c 2046   F8, FT8, FC6, F
+00000400: 4334 2c20 4643 322c 2046 437a 2c20 437a  C4, FC2, FCz, Cz
+00000410: 2c20 4332 2c20 4334 2c20 4336 2c20 5438  , C2, C4, C6, T8
+00000420: 2c20 5450 382c 2043 5036 2c20 4350 342c  , TP8, CP6, CP4,
+00000430: 2043 5032 2c20 5032 2c20 5034 2c20 5036   CP2, P2, P4, P6
+00000440: 2c20 5038 2c20 5031 302c 2050 4f38 2c20  , P8, P10, PO8, 
+00000450: 504f 342c 204f 320d 0a63 6861 6e6e 656c  PO4, O2..channel
+00000460: 5f6e 616d 6573 5f68 6961 6d70 3634 203d  _names_hiamp64 =
+00000470: 2046 7031 2c20 4146 372c 2041 4633 2c20   Fp1, AF7, AF3, 
+00000480: 4631 2c20 4633 2c20 4635 2c20 4637 2c20  F1, F3, F5, F7, 
+00000490: 4654 372c 2046 4335 2c20 4643 332c 2046  FT7, FC5, FC3, F
+000004a0: 4331 2c20 4331 2c20 4333 2c20 4335 2c20  C1, C1, C3, C5, 
+000004b0: 5437 2c20 5450 372c 2043 5035 2c20 4350  T7, TP7, CP5, CP
+000004c0: 332c 2043 5031 2c20 5031 2c20 5033 2c20  3, CP1, P1, P3, 
+000004d0: 5035 2c20 5037 2c20 5039 2c20 504f 372c  P5, P7, P9, PO7,
+000004e0: 2050 4f33 2c20 4f31 2c20 497a 2c20 4f7a   PO3, O1, Iz, Oz
+000004f0: 2c20 504f 7a2c 2050 7a2c 2043 507a 2c20  , POz, Pz, CPz, 
+00000500: 4670 7a2c 2046 7032 2c20 4146 382c 2041  Fpz, Fp2, AF8, A
+00000510: 4634 2c20 4146 7a2c 2046 7a2c 2046 322c  F4, AFz, Fz, F2,
+00000520: 2046 342c 2046 362c 2046 382c 2046 5438   F4, F6, F8, FT8
+00000530: 2c20 4643 362c 2046 4334 2c20 4643 322c  , FC6, FC4, FC2,
+00000540: 2046 437a 2c20 437a 2c20 4332 2c20 4334   FCz, Cz, C2, C4
+00000550: 2c20 4336 2c20 5438 2c20 5450 382c 2043  , C6, T8, TP8, C
+00000560: 5036 2c20 4350 342c 2043 5032 2c20 5032  P6, CP4, CP2, P2
+00000570: 2c20 5034 2c20 5036 2c20 5038 2c20 5031  , P4, P6, P8, P1
+00000580: 302c 2050 4f38 2c20 504f 342c 204f 320d  0, PO8, PO4, O2.
+00000590: 0a0d 0a63 6861 6e6e 656c 5f6e 616d 6573  ...channel_names
+000005a0: 5f67 7465 6331 3720 3d20 467a 2c20 4643  _gtec17 = Fz, FC
+000005b0: 332c 2046 4331 2c20 4643 7a2c 2046 4332  3, FC1, FCz, FC2
+000005c0: 2c20 4643 342c 2043 332c 2043 312c 2043  , FC4, C3, C1, C
+000005d0: 7a2c 2043 322c 2043 342c 2043 5033 2c20  z, C2, C4, CP3, 
+000005e0: 4350 312c 2043 507a 2c20 4350 322c 2043  CP1, CPz, CP2, C
+000005f0: 5034 2c20 5452 4947 4745 520d 0a         P4, TRIGGER..
```

### Comparing `neurodecode-2.0.4/neurodecode/stream_viewer/stream_viewer.py` & `neurodecode-2.0.5/neurodecode/stream_viewer/stream_viewer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,985 +1,986 @@
-# -*- coding: utf-8 -*-
-from __future__ import print_function, division, unicode_literals
-
-"""
- EEG Scope
- Iñaki Iturrate, Kyuhwa Lee
- 2017
-
- V1.0
- TODO
-	- Should move to VisPY: http://vispy.org/plot.html#module-vispy.plot but still under development
-	- The scope should be a class itself
-	- Scope of EXG signals
-	- Events should stored in a class.
-
-"""
-
-DEBUG_TRIGGER = False # TODO: parameterize
-NUM_X_CHANNELS = 16 # TODO: parameterize
-
-import os
-import sys
-import pdb
-import time
-import math
-import struct
-import traceback
-import subprocess
-import numpy as np
-import pyqtgraph as pg
-import neurodecode
-import neurodecode.utils.q_common as qc
-import neurodecode.utils.pycnbi_utils as pu
-import multiprocessing as mp
-from PyQt5.QtWidgets import QMainWindow,QApplication, QTableWidgetItem
-from PyQt5 import QtCore
-from PyQt5.QtGui import QPainter
-from pathlib import Path
-from importlib.resources import files
-from scipy.signal import butter, lfilter, lfiltic, buttord
-from neurodecode.stream_receiver.stream_receiver import StreamReceiver
-from neurodecode import logger
-from configparser import RawConfigParser
-from neurodecode.stream_viewer.ui_mainwindow_Viewer import Ui_MainWindow
-
-class Scope(QMainWindow):
-    def __init__(self, amp_name, amp_serial):
-        super(Scope, self).__init__()
-        self.ui = Ui_MainWindow()
-        self.ui.setupUi(self)
-        self.amp_name = amp_name
-        self.amp_serial = amp_serial
-        self.init_scope()
-        logger.info('Viewer launched')
-
-    #
-    # 	Main init function
-    #
-    def init_scope(self):
-
-        # pg.setConfigOption('background', 'w')
-        # pg.setConfigOption('foreground', 'k')
-
-        self.init_config_file()
-        self.init_loop()
-        self.init_panel_GUI()
-        self.init_scope_GUI()
-        self.init_timer()
-
-    #
-    #	Initializes config file
-    #
-    def init_config_file(self):
-        self.scope_settings = RawConfigParser(allow_no_value=True, inline_comment_prefixes=('#', ';'))
-        if (len(sys.argv) == 1):
-            self.show_channel_names = 0
-            self.device_name = ""
-        else:
-            if (sys.argv[1].find("gtec") > -1):
-                self.device_name = "gtec"
-                self.show_channel_names = 1
-            elif (sys.argv[1].find("biosemi") > -1):
-                self.device_name = "biosemi"
-                self.show_channel_names = 1
-            elif (sys.argv[1].find("hiamp") > -1):
-                self.device_name = "hiamp"
-                self.show_channel_names = 1
-            else:
-                self.device_name = ""
-                self.show_channel_names = 0
-
-        scope_setting_file = files('neurodecode.stream_viewer').joinpath('scope_settings.ini')
-        read_ok = self.scope_settings.read(scope_setting_file)
-        if len(read_ok) == 0:
-            logger.error('Cannot read scope setting file')
-            raise FileNotFoundError(scope_setting_file)
-
-    #
-    # 	Initialize control panel parameter
-    #
-    def init_panel_GUI(self):
-
-        self.show_TID_events = False
-        self.show_LPT_events = False
-        self.show_Key_events = False
-
-        # Event handler
-        self.ui.comboBox_scale.activated.connect(self.onActivated_combobox_scale)
-        self.ui.spinBox_time.valueChanged.connect(self.onValueChanged_spinbox_time)
-        self.ui.checkBox_car.stateChanged.connect(self.onActivated_checkbox_car)
-        self.ui.checkBox_bandpass.stateChanged.connect(
-            self.onActivated_checkbox_bandpass)
-        self.ui.checkBox_showTID.stateChanged.connect(
-            self.onActivated_checkbox_TID)
-        self.ui.checkBox_showLPT.stateChanged.connect(
-            self.onActivated_checkbox_LPT)
-        self.ui.checkBox_showKey.stateChanged.connect(
-            self.onActivated_checkbox_Key)
-        self.ui.pushButton_bp.clicked.connect(self.onClicked_button_bp)
-        self.ui.pushButton_rec.clicked.connect(self.onClicked_button_rec)
-        self.ui.pushButton_stoprec.clicked.connect(self.onClicked_button_stoprec)
-
-        self.ui.pushButton_stoprec.setEnabled(False)
-        self.ui.comboBox_scale.setCurrentIndex(4)
-        self.ui.checkBox_car.setChecked(
-            int(self.scope_settings.get("filtering", "apply_car_filter")))
-        self.ui.checkBox_bandpass.setChecked(
-            int(self.scope_settings.get("filtering", "apply_bandpass_filter")))
-        self.ui.checkBox_showTID.setChecked(
-            int(self.scope_settings.get("plot", "show_TID_events")))
-        self.ui.checkBox_showLPT.setChecked(
-            int(self.scope_settings.get("plot", "show_LPT_events")))
-        self.ui.checkBox_showKey.setChecked(
-            int(self.scope_settings.get("plot", "show_KEY_events")))
-        self.ui.statusBar.showMessage("[Not recording]")
-
-        self.channels_to_show_idx = []
-        idx = 0
-        for y in range(0, 4):
-            for x in range(0, NUM_X_CHANNELS):
-                if (idx < self.config['eeg_channels']):
-                    # self.table_channels.item(x,y).setTextAlignment(QtCore.Qt.AlignCenter)
-                    self.ui.table_channels.item(x, y).setSelected(True) # Qt5
-                    #self.table_channels.setItemSelected(self.table_channels.item(x, y), True) # Qt4 only
-                    self.channels_to_show_idx.append(idx)
-                else:
-                    self.ui.table_channels.setItem(x, y,
-                        QTableWidgetItem("N/A"))
-                    self.ui.table_channels.item(x, y).setFlags(
-                        QtCore.Qt.NoItemFlags)
-                    self.ui.table_channels.item(x, y).setTextAlignment(
-                        QtCore.Qt.AlignCenter)
-                idx += 1
-
-        self.ui.table_channels.verticalHeader().setStretchLastSection(True)
-        self.ui.table_channels.horizontalHeader().setStretchLastSection(True)
-        self.ui.table_channels.itemSelectionChanged.connect(
-            self.onSelectionChanged_table)
-
-        self.screen_width = 522
-        self.screen_height = 160
-        # self.setGeometry(100,100, self.screen_width, self.screen_height)
-        # self.setFixedSize(self.screen_width, self.screen_height)
-        self.setWindowTitle('EEG Scope Panel')
-        self.setFocusPolicy(QtCore.Qt.ClickFocus)
-        self.setFocus()
-        self.show()
-
-    #
-    #	Initialize scope parameters
-    #
-    def init_scope_GUI(self):
-
-        self.bool_parser = {True:'1', False:'0'}
-
-        # PyQTGraph plot initialization
-        self.win = pg.GraphicsLayoutWidget()
-        self.win.setWindowTitle('EEG Scope')
-        self.win.setWindowFlags(QtCore.Qt.WindowMinimizeButtonHint)
-        self.win.keyPressEvent = self.keyPressEvent
-        self.win.show()
-        self.main_plot_handler = self.win.addPlot()
-        self.win.resize(1280, 800)
-
-        # Scales available in the GUI. If you change the options in the GUI
-        # you should change them here as well
-        self.scales_range = [1, 10, 25, 50, 100, 250, 500, 1000, 2500, 100000]
-
-        # Scale in uV
-        self.scale = int(self.scope_settings.get("plot", "scale_plot"))
-        # Time window to show in seconds
-        self.seconds_to_show = int(self.scope_settings.get("plot", "time_plot"))
-
-        # Y Tick labels. Use values from the config file.
-        self.channel_labels = []
-        values = []
-
-        ''' For non-LSL systems having no channel names
-        for x in range(0, self.config['eeg_channels']):
-            if (self.show_channel_names):
-                self.channel_labels.append("(" + str(x + 1) + ") " +
-                    self.scope_settings.get("internal",
-                    "channel_names_" + self.device_name + str(
-                    self.config['eeg_channels'])).split(', ')[x])
-            else:
-                self.channel_labels.append('CH ' + str(x + 1))
-        '''
-        ch_names = np.array( self.sr.get_channel_names() )
-        self.channel_labels = ch_names[ self.sr.get_eeg_channels() ]
-        for x in range(0, len(self.channels_to_show_idx)):
-            values.append((-x * self.scale,
-                self.channel_labels[self.channels_to_show_idx[x]]))
-
-        values_axis = []
-        values_axis.append(values)
-        values_axis.append([])
-
-        # Update table labels with current names
-        idx = 0
-        for y in range(0, 4):
-            for x in range(0, NUM_X_CHANNELS):
-                if (idx < self.config['eeg_channels']):
-                    self.ui.table_channels.item(x, y).setText(
-                        self.channel_labels[idx])
-                idx += 1
-
-        # Plot initialization
-        self.main_plot_handler.getAxis('left').setTicks(values_axis)
-        self.main_plot_handler.setRange(xRange=[0, self.seconds_to_show],
-            yRange=[+1.5 * self.scale,
-                -0.5 * self.scale - self.scale * self.config['eeg_channels']])
-        self.main_plot_handler.disableAutoRange()
-        self.main_plot_handler.showGrid(y=True)
-        self.main_plot_handler.setLabel(axis='left',
-            text='Scale (uV): ' + str(self.scale))
-        self.main_plot_handler.setLabel(axis='bottom', text='Time (s)')
-
-        # X axis
-        self.x_ticks = np.zeros(self.config['sf'] * self.seconds_to_show);
-        for x in range(0, self.config['sf'] * self.seconds_to_show):
-            self.x_ticks[x] = (x * 1) / float(self.config['sf'])
-
-        # Plotting colors. If channels > 16, colors will roll back to the beginning
-        self.colors = np.array(
-            [[255, 0, 0], [0, 255, 0], [0, 0, 255], [255, 255, 0],
-            [0, 255, 255], [255, 0, 255], [128, 100, 100], [0, 128, 0],
-            [0, 128, 128], [128, 128, 0], [255, 128, 128], [128, 0, 128],
-            [128, 255, 0], [255, 128, 0], [0, 255, 128], [128, 0, 255]])
-
-        # We want a lightweight scope, so we downsample the plotting to 64 Hz
-        self.subsampling_value = self.config['sf'] / 64
-
-        # EEG data for plotting
-        self.data_plot = np.zeros((self.config['sf'] * self.seconds_to_show,
-        self.config['eeg_channels']))
-        self.curve_eeg = []
-        for x in range(0, len(self.channels_to_show_idx)):
-            self.curve_eeg.append(self.main_plot_handler.plot(x=self.x_ticks,
-                y=self.data_plot[:, self.channels_to_show_idx[x]],
-                pen=pg.mkColor(
-                    self.colors[self.channels_to_show_idx[x] % 16, :])))
-        # self.curve_eeg[-1].setDownsampling(ds=self.subsampling_value, auto=False, method="mean")
-
-
-        # Events data
-        self.events_detected = []
-        self.events_curves = []
-        self.events_text = []
-
-        # CAR initialization
-        self.apply_car = int(
-            self.scope_settings.get("filtering", "apply_car_filter"))
-        self.matrix_car = np.zeros(
-            (self.config['eeg_channels'], self.config['eeg_channels']),
-            dtype=float)
-        self.matrix_car[:, :] = -1 / float(self.config['eeg_channels'])
-        np.fill_diagonal(self.matrix_car,
-            1 - (1 / float(self.config['eeg_channels'])))
-
-        # Laplacian initalization. TO BE DONE
-        self.matrix_lap = np.zeros(
-            (self.config['eeg_channels'], self.config['eeg_channels']),
-            dtype=float)
-        np.fill_diagonal(self.matrix_lap, 1)
-        '''
-        self.matrix_lap[2, 0] = -1
-        self.matrix_lap[0, 2] = -0.25
-        self.matrix_lap[0, 2] = -0.25
-        '''
-
-        # BP initialization
-        self.apply_bandpass = int(
-            self.scope_settings.get("filtering", "apply_bandpass_filter"))
-        if (self.apply_bandpass):
-            self.ui.doubleSpinBox_hp.setValue(float(
-                self.scope_settings.get("filtering",
-                    "bandpass_cutoff_frequency").split(' ')[0]))
-            self.ui.doubleSpinBox_lp.setValue(float(
-                self.scope_settings.get("filtering",
-                    "bandpass_cutoff_frequency").split(' ')[1]))
-            self.ui.doubleSpinBox_lp.setMinimum(0.1)
-            self.ui.doubleSpinBox_lp.setMaximum(self.sr.sample_rate/2 - 0.1)
-            self.ui.doubleSpinBox_lp.setDecimals(1)
-            self.ui.doubleSpinBox_lp.setSingleStep(1)
-            self.ui.doubleSpinBox_hp.setMinimum(0.1)
-            self.ui.doubleSpinBox_hp.setMaximum(self.sr.sample_rate/2 - 0.1)
-            self.ui.doubleSpinBox_hp.setDecimals(1)
-            self.ui.doubleSpinBox_hp.setSingleStep(1)
-            self.ui.pushButton_bp.click()
-
-        self.ui.checkBox_bandpass.setChecked(self.apply_car)
-        self.ui.checkBox_bandpass.setChecked(self.apply_bandpass)
-
-        self.update_title_scope()
-
-        # Help variables
-        self.show_help = 0
-        self.help = pg.TextItem(
-            "CNBI EEG Scope v0.3 \n" + "----------------------------------------------------------------------------------\n" + "C: De/activate CAR Filter\n" + "B: De/activate Bandpass Filter (with current settings)\n" + "T: Show/hide TiD events\n" + "L: Show/hide LPT events\n" + "K: Show/hide Key events. If not shown, they are NOT recorded!\n" + "0-9: Add a user-specific Key event. Do not forget to write down why you marked it.\n" + "Up, down arrow keys: Increase/decrease the scale, steps of 10 uV\n" + "Left, right arrow keys: Increase/decrease the time to show, steps of 1 s\n" + "Spacebar: Stop the scope plotting, whereas data acquisition keeps running (EXPERIMENTAL)\n" + "Esc: Exits the scope",
-            anchor=(0, 0), border=(70, 70, 70),
-            fill=pg.mkColor(20, 20, 20, 200), color=(255, 255, 255))
-
-        # Stop plot functionality
-        self.stop_plot = 0
-
-        # Force repaint even when we shouldn't repaint.
-        self.force_repaint = 0
-
-    # For some strange reason when the width is > 1 px the scope runs slow.
-    # self.pen_plot = []
-    # for x in range(0, self.config['eeg_channels']):
-    # 	self.pen_plot.append(pg.mkPen(self.colors[x%16,:], width=3))
-
-    #
-    # 	Initializes the BCI loop parameters
-    #
-    def init_loop_cnbiloop(self):
-
-        self.fin = open(self.scope_settings.get("internal", "path_pipe"), 'r')
-
-        # 12 unsigned ints (4 bytes)
-        data = struct.unpack("<12I", self.fin.read(4 * 12))
-
-        self.config = {'id':data[0], 'sf':data[1], 'labels':data[2],
-            'samples':data[3], 'eeg_channels':data[4], 'exg_channels':data[5],
-            'tri_channels':data[6], 'eeg_type':data[8], 'exg_type':data[9],
-            'tri_type':data[10], 'lbl_type':data[11], 'tim_size':1,
-            'idx_size':1}
-
-        self.tri = np.zeros(self.config['samples'])
-        self.eeg = np.zeros(
-            (self.config['samples'], self.config['eeg_channels']),
-            dtype=float)
-        self.exg = np.zeros(
-            (self.config['samples'], self.config['exg_channels']),
-            dtype=float)
-
-        # TID initialization
-        self.bci = BCI.BciInterface()
-
-    #
-    # 	Initializes the BCI loop parameters
-    #
-    def init_loop(self):
-
-        self.updating = False
-
-        self.sr = StreamReceiver(window_size=1, buffer_size=10,
-            amp_serial=self.amp_serial, amp_name=self.amp_name)
-        srate = int(self.sr.sample_rate)
-        # n_channels= self.sr.channels
-
-        # 12 unsigned ints (4 bytes)
-        ########## TODO: assumkng 32 samples chunk => make it read from LSL header
-        data = ['EEG', srate, ['L', 'R'], 32, len(self.sr.get_eeg_channels()),
-            0, self.sr.get_trigger_channel(), None, None, None, None, None]
-        logger.info('Trigger channel is %d' % self.sr.get_trigger_channel())
-
-        self.config = {'id':data[0], 'sf':data[1], 'labels':data[2],
-            'samples':data[3], 'eeg_channels':data[4], 'exg_channels':data[5],
-            'tri_channels':data[6], 'eeg_type':data[8], 'exg_type':data[9],
-            'tri_type':data[10], 'lbl_type':data[11], 'tim_size':1,
-            'idx_size':1}
-
-        self.tri = np.zeros(self.config['samples'])
-        self.last_tri = 0
-        self.eeg = np.zeros(
-            (self.config['samples'], self.config['eeg_channels']),
-            dtype=float)
-        self.exg = np.zeros(
-            (self.config['samples'], self.config['exg_channels']),
-            dtype=float)
-        self.ts_list = []
-        self.ts_list_tri = []
-
-    #
-    # 	Initializes the QT timer, which will call the update function every 20 ms
-    #
-    def init_timer(self):
-
-        self.tm = qc.Timer()  # leeq
-
-        QtCore.QCoreApplication.processEvents()
-        QtCore.QCoreApplication.flush()
-        self.timer = QtCore.QTimer(self)
-        self.timer.timeout.connect(self.update_loop)
-        self.timer.start(20);
-
-    # QtCore.QTimer.singleShot( 20, self.update_loop )
-
-
-    #
-    #	Main update function (connected to the timer)
-    #
-    def update_loop(self):
-        try:
-            # assert self.updating==False, 'thread destroyed?'
-            # self.updating= True
-            # self.handle_tobiid_input()	# Read TiDs
-            self.read_eeg()  # Read new chunk
-            if len(self.ts_list) > 0:
-                self.filter_signal()  # Filter acquired data
-                self.update_ringbuffers()  # Update the plotting infor
-                if (not self.stop_plot):
-                    self.repaint()  # Call paint event
-        except:
-            logger.exception('Exception. Dropping into a shell.')
-            pdb.set_trace()
-        finally:
-            # self.updating= False
-            # using singleShot instead
-            # QtCore.QTimer.singleShot( 20, self.update_loop )
-            pass
-
-    #
-    #	Read EEG
-    #
-    def read_eeg(self):
-
-        # if self.updating==True: print( '##### ERROR: thread destroyed ? ######' )
-        # self.updating= True
-
-        try:
-            # data, self.ts_list= self.sr.inlets[0].pull_chunk(max_samples=self.config['sf']) # [frames][channels]
-            data, self.ts_list = self.sr.acquire(blocking=False)
-
-            # TODO: check and change to these two lines
-            #self.sr.acquire(blocking=False, decim=DECIM)
-            #data, self.ts_list = self.sr.get_window()
-
-            if len(self.ts_list) == 0:
-                # self.eeg= None
-                # self.tri= None
-                return
-
-            n = self.config['eeg_channels']
-            '''
-            x= np.array( data )
-            trg_ch= self.config['tri_channels']
-            if trg_ch is not None:
-                self.tri= np.reshape( x[:,trg_ch], (-1,1) ) # samples x 1
-            self.eeg= np.reshape( x[:,self.sr.eeg_channels], (-1,n) ) # samples x channels
-            '''
-            trg_ch = self.config['tri_channels']
-            if trg_ch is not None:
-                self.tri = np.reshape(data[:, trg_ch], (-1, 1))  # samples x 1
-            self.eeg = np.reshape(data[:, self.sr.eeg_channels],
-                (-1, n))  # samples x channels
-
-            if DEBUG_TRIGGER:
-                # show trigger value
-                try:
-                    trg_value = max(self.tri)
-                    if trg_value > 0:
-                        logger.info('Received trigger %s' % trg_value)
-                except:
-                    logger.exception('Error! self.tri = %s' % self.tri)
-
-                    # Read exg. self.config.samples*self.config.exg_ch, type float
-                    # bexg = np.random.rand( 1, self.config['samples'] * self.config['exg_channels'] )
-                    # self.exg = np.reshape(list(bexg), (self.config['samples'],self.config['exg_channels']))
-        except WindowsError:
-            # print('**** Access violation in read_eeg():\n%s\n%s'% (sys.exc_info()[0], sys.exc_info()[1]))
-            pass
-        except:
-            logger.exception()
-            pdb.set_trace()
-
-    #
-    #	Read EEG
-    #
-    def read_eeg_cnbiloop(self):
-
-        # Reading in python is blocking, so it will wait until having the amount of data needed
-        # Read timestamp. 1 value, type double
-        timestamp = struct.unpack("<d", self.fin.read(8 * 1))
-        # Read index. 1 value, type uint64
-        index = struct.unpack("<Q", self.fin.read(8 * 1))
-        # Read labels. self.config.labels, type double
-        labels = struct.unpack("<" + str(self.config['labels']) + "I",
-            self.fin.read(4 * self.config['labels']))
-        # Read eeg. self.config.samples*self.config.eeg_ch, type float
-        beeg = struct.unpack("<" + str(
-            self.config['samples'] * self.config['eeg_channels']) + "f",
-            self.fin.read(
-                4 * self.config['samples'] * self.config['eeg_channels']))
-        self.eeg = np.reshape(list(beeg),
-            (self.config['samples'], self.config['eeg_channels']))
-        # Read exg. self.config.samples*self.config.exg_ch, type float
-        bexg = struct.unpack("<" + str(
-            self.config['samples'] * self.config['exg_channels']) + "f",
-            self.fin.read(
-                4 * self.config['samples'] * self.config['exg_channels']))
-        self.exg = np.reshape(list(bexg),
-            (self.config['samples'], self.config['exg_channels']))
-        # Read tri. self.config.samples*self.config.tri_ch, type float
-        self.tri = struct.unpack("<" + str(
-            self.config['samples'] * self.config['tri_channels']) + "i",
-            self.fin.read(
-                4 * self.config['samples'] * self.config['tri_channels']))
-
-    #
-    #	Bandpas + CAR filtering
-    #
-    def filter_signal(self):
-
-        if (self.apply_bandpass):
-            for x in range(0, self.eeg.shape[1]):
-                self.eeg[:, x], self.zi[:, x] = lfilter(self.b, self.a,
-                    self.eeg[:, x], -1, self.zi[:, x])
-
-        # We only apply CAR if selected AND there are at least 2 channels. Otherwise it makes no sense
-        if (self.apply_car) and (len(self.channels_to_show_idx) > 1):
-            self.eeg = np.dot(self.matrix_car, np.transpose(self.eeg))
-            self.eeg = np.transpose(self.eeg)
-
-    #
-    #	Update ringbuffers and events for plotting
-    #
-    def update_ringbuffers(self):
-        # leeq
-        self.data_plot = np.roll(self.data_plot, -len(self.ts_list), 0)
-        self.data_plot[-len(self.ts_list):, :] = self.eeg
-
-        # We have to remove those indexes that reached time = 0
-        delete_indices_e = []
-        delete_indices_c = []
-        for x in range(0, len(self.events_detected), 2):
-            xh = int(x / 2)
-            self.events_detected[x] -= len(self.ts_list)  # leeq
-            if (self.events_detected[x] < 0) and (not self.stop_plot):
-                delete_indices_e.append(x)
-                delete_indices_e.append(x + 1)
-                delete_indices_c.append(xh)
-                self.events_curves[xh].clear()
-                self.main_plot_handler.removeItem(self.events_text[xh])
-
-        self.events_detected = [i for j, i in enumerate(self.events_detected) if
-            j not in delete_indices_e]
-        self.events_curves = [i for j, i in enumerate(self.events_curves) if
-            j not in delete_indices_c]
-        self.events_text = [i for j, i in enumerate(self.events_text) if
-            j not in delete_indices_c]
-
-        # Find LPT events and add them
-        if (self.show_LPT_events) and (not self.stop_plot):
-            for x in range(len(self.tri)):
-                tri = int(self.tri[x])
-                if tri != 0 and (tri > self.last_tri):
-                    self.addEventPlot("LPT", tri)
-                    logger.info('Trigger %d received' % tri)
-                self.last_tri = tri
-
-    #
-    #	Called by repaint()
-    #
-    def paintEvent(self, e):
-        # Distinguish between paint events from timer and event QT widget resizing, clicking etc (sender is None)
-        # We should only paint when the timer triggered the event.
-        # Just in case, there's a flag to force a repaint even when we shouldn't repaint
-        sender = self.sender()
-        if 'force_repaint' not in self.__dict__.keys():
-            logger.warning('force_repaint is not set! Is it a Qt bug?')
-            self.force_repaint = 0
-        if (sender is None) and (not self.force_repaint):
-            pass
-        else:
-            self.force_repaint = 0
-            qp = QPainter()
-            qp.begin(self)
-            # Update the interface
-            self.paintInterface(qp)
-            qp.end()
-
-    #
-    #	Update stuff on the interface. Only graphical updates should be added here
-    #
-    def paintInterface(self, qp):
-
-        # Update EEG channels
-        for x in range(0, len(self.channels_to_show_idx)):
-            self.curve_eeg[x].setData(x=self.x_ticks, y=self.data_plot[:,self.channels_to_show_idx[x]] - x * self.scale)
-
-        # Update events
-        for x in range(0, len(self.events_detected), 2):
-            xh = int(x / 2)
-            self.events_curves[xh].setData(x=np.array(
-                [self.x_ticks[self.events_detected[x]],
-                    self.x_ticks[self.events_detected[x]]]), y=np.array(
-                [+1.5 * self.scale,
-                    -0.5 * self.scale - self.scale * self.config[
-                        'eeg_channels']]))
-            self.events_text[xh].setPos(self.x_ticks[self.events_detected[x]],
-                self.scale)
-
-    #
-    #	Do necessary stuff when scale has changed
-    #
-    def update_plot_scale(self, new_scale):
-
-        if (new_scale < 1):
-            new_scale = 1
-        # commented out by dbdq.
-        # else:
-        #	new_scale = new_scale - new_scale%10
-
-        self.scale = new_scale
-
-        # Y Tick labels
-        values = []
-        for x in range(0, len(self.channels_to_show_idx)):
-            values.append((-x * self.scale,
-            self.channel_labels[self.channels_to_show_idx[x]]))
-
-        values_axis = []
-        values_axis.append(values)
-        values_axis.append([])
-
-        self.main_plot_handler.getAxis('left').setTicks(values_axis)
-        self.main_plot_handler.setRange(
-            yRange=[+self.scale, -self.scale * len(self.channels_to_show_idx)])
-        self.main_plot_handler.setLabel(axis='left',
-            text='Scale (uV): ' + str(self.scale))
-        self.trigger_help()
-
-        # We force an immediate repaint to avoid "shakiness".
-        if (not self.stop_plot):
-            self.force_repaint = 1
-            self.repaint()
-
-    #
-    #	Do necessary stuff when seconds to show have changed
-    #
-    def update_plot_seconds(self, new_seconds):
-
-        # Do nothing unless...
-        if (new_seconds != self.seconds_to_show) and (new_seconds > 0) and (
-                new_seconds < 100):
-            self.ui.spinBox_time.setValue(new_seconds)
-            self.main_plot_handler.setRange(xRange=[0, new_seconds])
-            self.x_ticks = np.zeros(self.config['sf'] * new_seconds);
-            for x in range(0, self.config['sf'] * new_seconds):
-                self.x_ticks[x] = (x * 1) / float(self.config['sf'])
-
-            if (new_seconds > self.seconds_to_show):
-                padded_signal = np.zeros((self.config['sf'] * new_seconds,
-                self.config['eeg_channels']))
-                padded_signal[padded_signal.shape[0] - self.data_plot.shape[0]:,
-                :] = self.data_plot
-                for x in range(0, len(self.events_detected), 2):
-                    self.events_detected[x] += padded_signal.shape[0] - \
-                                               self.data_plot.shape[0]
-                self.data_plot = padded_signal
-
-            else:
-                for x in range(0, len(self.events_detected), 2):
-                    self.events_detected[x] -= self.data_plot.shape[0] - \
-                                               self.config['sf'] * new_seconds
-                self.data_plot = self.data_plot[
-                self.data_plot.shape[0] - self.config['sf'] * new_seconds:, :]
-
-            self.seconds_to_show = new_seconds
-            self.trigger_help()
-
-            # We force an immediate repaint to avoid "shakiness".
-            if (not self.stop_plot):
-                self.force_repaint = 1
-                self.repaint()
-
-    #
-    # Handle TOBI iD events
-    #
-    def handle_tobiid_input(self):
-
-        data = None
-        try:
-            data = self.bci.iDsock_bus.recv(512)
-            self.bci.idStreamer_bus.Append(data)
-        except:
-            self.nS = False
-            self.dec = 0
-            pass
-
-        # deserialize ID message
-        if data:
-            if self.bci.idStreamer_bus.Has("<tobiid", "/>"):
-                msg = self.bci.idStreamer_bus.Extract("<tobiid", "/>")
-                self.bci.id_serializer_bus.Deserialize(msg)
-                self.bci.idStreamer_bus.Clear()
-                tmpmsg = int(self.bci.id_msg_bus.GetEvent())
-                if (self.show_TID_events) and (not self.stop_plot):
-                    self.addEventPlot("TID", tmpmsg)
-
-            elif self.bci.idStreamer_bus.Has("<tcstatus", "/>"):
-                MsgNum = self.bci.idStreamer_bus.Count("<tcstatus")
-                for i in range(1, MsgNum - 1):
-                    # Extract most of these messages and trash them
-                    msg_useless = self.bci.idStreamer_bus.Extract("<tcstatus",
-                        "/>")
-
-    #
-    # 	Add an event to the scope
-    #
-    def addEventPlot(self, event_name, event_id):
-        if (event_name == "TID"):
-            color = pg.mkColor(0, 0, 255)
-        elif (event_name == "KEY"):
-            color = pg.mkColor(255, 0, 0)
-        elif (event_name == "LPT"):
-            color = pg.mkColor(0, 255, 0)
-        else:
-            color = pg.mkColor(255, 255, 255)
-
-        self.events_detected.append(self.data_plot.shape[0] - 1)
-        self.events_detected.append(event_id)
-        self.events_curves.append(self.main_plot_handler.plot(pen=color,
-            x=np.array([self.x_ticks[-1], self.x_ticks[-1]]), y=np.array(
-                [+1.5 * self.scale,
-                    -1.5 * self.scale * self.config['eeg_channels']])))
-        # text = pg.TextItem(event_name + "(" + str(self.events_detected[-1]) + ")", anchor=(1.1,0), fill=(0,0,0), color=color)
-        text = pg.TextItem(str(self.events_detected[-1]), anchor=(1.1, 0),
-            fill=(0, 0, 0), color=color)
-        text.setPos(self.x_ticks[-1], self.scale)
-        self.events_text.append(text)
-        self.main_plot_handler.addItem(self.events_text[-1])
-
-    #
-    #	Calculation of bandpass coefficients.
-    #	Order is computed automatically.
-    #	Note that if filter is unstable this function crashes (TODO handle problems)
-    #
-    def butter_bandpass(self, highcut, lowcut, fs, num_ch):
-        low = lowcut / (0.5 * fs)
-        high = highcut / (0.5 * fs)
-        # get the order. TO BE DONE: Sometimes it fails
-        #ord = buttord(high, low, 2, 40)
-        #b, a = butter(ord[0], [high, low], btype='band')
-        b, a = butter(2, [high, low], btype='band')
-        zi = np.zeros([a.shape[0] - 1, num_ch])
-        return b, a, zi
-
-    #
-    #	Updates the title shown in the scope
-    #
-    def update_title_scope(self):
-        if (hasattr(self, 'main_plot_handler')):
-            self.main_plot_handler.setTitle(
-                title='TLK: ' + self.bool_parser[self.show_TID_events] +
-                      self.bool_parser[self.show_LPT_events] + self.bool_parser[
-                          self.show_Key_events] + ', CAR: ' + self.bool_parser[
-                          self.apply_car] + ', BP: ' + self.bool_parser[
-                          self.apply_bandpass] + ' [' + str(
-                    self.ui.doubleSpinBox_hp.value()) + '-' + str(
-                    self.ui.doubleSpinBox_lp.value()) + '] Hz')
-            # ', BP: ' + self.bool_parser[self.apply_bandpass] + (' [' + str(self.doubleSpinBox_hp.value()) + '-' + str(self.doubleSpinBox_lp.value()) + '] Hz' if self.apply_bandpass else ''))
-
-    #
-    #	Shows / hide help in the scope window
-    #
-    def trigger_help(self):
-        if self.show_help:
-            self.help.setPos(0, self.scale)
-            self.main_plot_handler.addItem(self.help)
-            self.help.setZValue(1)
-        else:
-            self.main_plot_handler.removeItem(self.help)
-
-    # ----------------------------------------------------------------------------------------------------
-    # 			EVENT HANDLERS
-    # ----------------------------------------------------------------------------------------------------
-    def onClicked_button_rec(self):
-        # Simply call cl_rpc for this.
-        if (len(self.lineEdit_recFilename.text()) > 0):
-            if ".gdf" in self.lineEdit_recFilename.text():
-                self.ui.pushButton_stoprec.setEnabled(True)
-                self.ui.pushButton_rec.setEnabled(False)
-                # Popen is more efficient than os.open, since it is non-blocking
-                subprocess.Popen(
-                    ["cl_rpc", "openxdf", str(self.ui.lineEdit_recFilename.text()),
-                        "dummy_log", "dummy_log"], close_fds=True)
-                self.statusBar.showMessage(
-                    "Recording file " + str(self.ui.lineEdit_recFilename.text()))
-            elif ".bdf" in self.ui.lineEdit_recFilename.text():
-                self.ui.pushButton_stoprec.setEnabled(True)
-                self.ui.pushButton_rec.setEnabled(False)
-                subprocess.Popen(
-                    ["cl_rpc", "openxdf", str(self.ui.lineEdit_recFilename.text()),
-                        "dummy_log", "dummy_log"], close_fds=True)
-                self.statusBar.showMessage(
-                    "Recording file " + str(self.ui.lineEdit_recFilename.text()))
-            else:
-                pass
-
-    def onClicked_button_stoprec(self):
-        subprocess.Popen(["cl_rpc", "closexdf"], close_fds=True)
-        self.ui.pushButton_rec.setEnabled(True)
-        self.ui.pushButton_stoprec.setEnabled(False)
-        self.ui.statusBar.showMessage("Not recording")
-
-    def onActivated_checkbox_bandpass(self):
-        self.apply_bandpass = False
-        self.ui.pushButton_bp.setEnabled(self.ui.checkBox_bandpass.isChecked())
-        self.ui.doubleSpinBox_hp.setEnabled(self.ui.checkBox_bandpass.isChecked())
-        self.ui.doubleSpinBox_lp.setEnabled(self.ui.checkBox_bandpass.isChecked())
-        self.update_title_scope()
-
-    def onActivated_checkbox_car(self):
-        self.apply_car = self.ui.checkBox_car.isChecked()
-        self.update_title_scope()
-
-    def onActivated_checkbox_TID(self):
-        self.show_TID_events = self.ui.checkBox_showTID.isChecked()
-        self.update_title_scope()
-
-    def onActivated_checkbox_LPT(self):
-        self.show_LPT_events = self.ui.checkBox_showLPT.isChecked()
-        self.update_title_scope()
-
-    def onActivated_checkbox_Key(self):
-        self.show_Key_events = self.ui.checkBox_showKey.isChecked()
-        self.update_title_scope()
-
-    def onValueChanged_spinbox_time(self):
-        self.update_plot_seconds(self.ui.spinBox_time.value())
-
-    def onActivated_combobox_scale(self):
-        self.update_plot_scale(
-            self.scales_range[self.ui.comboBox_scale.currentIndex()])
-
-    def onClicked_button_bp(self):
-        if (self.ui.doubleSpinBox_lp.value() > self.ui.doubleSpinBox_hp.value()):
-            self.apply_bandpass = True
-            self.b, self.a, self.zi = self.butter_bandpass(
-                self.ui.doubleSpinBox_hp.value(), self.ui.doubleSpinBox_lp.value(),
-                self.config['sf'], self.config['eeg_channels'])
-        self.update_title_scope()
-
-    def onSelectionChanged_table(self):
-
-        # Remove current plot
-        for x in range(0, len(self.channels_to_show_idx)):
-            self.main_plot_handler.removeItem(self.curve_eeg[x])
-
-        # Which channels should I plot?
-        self.channels_to_show_idx = []
-        self.channels_to_hide_idx = []
-        idx = 0
-        for y in range(0, 4):
-            for x in range(0, NUM_X_CHANNELS):
-                if (idx < self.config['eeg_channels']):
-                    #if (self.table_channels.isItemSelected( # Qt4 only
-                    if (QTableWidgetItem.isSelected( # Qt5
-                        self.ui.table_channels.item(x, y))):
-                        self.channels_to_show_idx.append(idx)
-                    else:
-                        self.channels_to_hide_idx.append(idx)
-                    idx += 1
-
-        # Add new plots
-        self.curve_eeg = []
-        for x in range(0, len(self.channels_to_show_idx)):
-            self.curve_eeg.append(self.main_plot_handler.plot(x=self.x_ticks,
-                y=self.data_plot[:, self.channels_to_show_idx[x]],
-                pen=self.colors[self.channels_to_show_idx[x] % NUM_X_CHANNELS, :]))
-            self.curve_eeg[-1].setDownsampling(ds=self.subsampling_value,
-                auto=False, method="mean")
-
-        # Update CAR so it's computed based only on the shown channels
-        if (len(self.channels_to_show_idx) > 1):
-            self.matrix_car = np.zeros(
-                (self.config['eeg_channels'], self.config['eeg_channels']),
-                dtype=float)
-            self.matrix_car[:, :] = -1 / float(len(self.channels_to_show_idx))
-            np.fill_diagonal(self.matrix_car,
-                1 - (1 / float(len(self.channels_to_show_idx))))
-            for x in range(0, len(self.channels_to_hide_idx)):
-                self.matrix_car[self.channels_to_hide_idx[x], :] = 0
-                self.matrix_car[:, self.channels_to_hide_idx[x]] = 0
-
-        # Refresh the plot
-        self.update_plot_scale(self.scale)
-
-    def keyPressEvent(self, event):
-        key = event.key()
-        if (key == QtCore.Qt.Key_Escape):
-            self.closeEvent(None)
-        if (key == QtCore.Qt.Key_H):
-            self.show_help = not self.show_help
-            self.trigger_help()
-        if (key == QtCore.Qt.Key_Up):
-            # Python's log(x, 10) has a rounding bug. Use log10(x) instead.
-            new_scale = self.scale + max(1, 10 ** int(math.log10(self.scale)))
-            self.update_plot_scale(new_scale)
-        if (key == QtCore.Qt.Key_Space):
-            self.stop_plot = not self.stop_plot
-        if (key == QtCore.Qt.Key_Down):
-            if self.scale >= 2:
-                # Python's log(x, 10) has a rounding bug. Use log10(x) instead.
-                new_scale = self.scale - max(1,
-                    10 ** int(math.log10(self.scale - 1)))
-                self.update_plot_scale(new_scale)
-        if (key == QtCore.Qt.Key_Left):
-            self.update_plot_seconds(self.seconds_to_show - 1)
-        if (key == QtCore.Qt.Key_Right):
-            self.update_plot_seconds(self.seconds_to_show + 1)
-        if (key == QtCore.Qt.Key_L):
-            self.ui.checkBox_showLPT.setChecked(
-                not self.ui.checkBox_showLPT.isChecked())
-        if (key == QtCore.Qt.Key_T):
-            self.ui.checkBox_showTID.setChecked(
-                not self.ui.checkBox_showTID.isChecked())
-        if (key == QtCore.Qt.Key_K):
-            self.ui.checkBox_showKey.setChecked(
-                not self.ui.checkBox_showKey.isChecked())
-        if (key == QtCore.Qt.Key_C):
-            self.ui.checkBox_car.setChecked(not self.ui.checkBox_car.isChecked())
-        if (key == QtCore.Qt.Key_B):
-            self.ui.checkBox_bandpass.setChecked(
-                not self.ui.checkBox_bandpass.isChecked())
-            if self.ui.checkBox_bandpass.isChecked():
-                self.ui.pushButton_bp.click()
-        if ((key >= QtCore.Qt.Key_0) and (key <= QtCore.Qt.Key_9)):
-            if (self.show_Key_events) and (not self.stop_plot):
-                self.addEventPlot("KEY", 990 + key - QtCore.Qt.Key_0)
-
-    #
-    #	Function called when a closing event was triggered.
-    #
-    def closeEvent(self, event):
-        '''
-        reply = QtGui.QMessageBox.question(self, "Quit", "Are you sure you want to quit?", QtGui.QMessageBox.Yes | QtGui.QMessageBox.No, QtGui.QMessageBox.Yes)
-        if (reply == QtGui.QMessageBox.Yes):
-            if (self.pushButton_stoprec.isEnabled()):
-                subprocess.Popen(["cl_rpc", "closexdf"], close_fds=True)
-            self.fin.close()
-            exit()
-        '''
-
-        # leeq
-        if (self.ui.pushButton_stoprec.isEnabled()):
-            subprocess.Popen(["cl_rpc", "closexdf"], close_fds=True)
-
-        # ----------------------------------------------------------------------------------------------------
-        # 		END OF EVENT HANDLERS
-        # ----------------------------------------------------------------------------------------------------
-
-
-def main():
-    """
-    Invoked from console
-    """
-    if len(sys.argv) == 1:
-        amp_name, amp_serial = pu.search_lsl()
-    elif len(sys.argv) == 2:
-        amp_name, amp_serial = sys.argv[1], None
-    else:
-        amp_name, amp_serial = sys.argv[1:3]
-    logger.info('Connecting to a server %s (Serial %s).' % (amp_name, amp_serial))
-
-    app = QApplication(sys.argv)
-    Scope(amp_name, amp_serial)
-    sys.exit(app.exec_())
-
-if __name__ == '__main__':
-    main()
+# -*- coding: utf-8 -*-
+from __future__ import print_function, division, unicode_literals
+
+"""
+ EEG Scope
+ Iñaki Iturrate, Kyuhwa Lee
+ 2017
+
+ V1.0
+ TODO
+	- Should move to VisPY: http://vispy.org/plot.html#module-vispy.plot but still under development
+	- The scope should be a class itself
+	- Scope of EXG signals
+	- Events should stored in a class.
+
+"""
+
+DEBUG_TRIGGER = False # TODO: parameterize
+NUM_X_CHANNELS = 16 # TODO: parameterize
+
+import os
+import sys
+import pdb
+import time
+import math
+import struct
+import traceback
+import subprocess
+import numpy as np
+import pyqtgraph as pg
+import neurodecode
+import neurodecode.utils.q_common as qc
+import neurodecode.utils.pycnbi_utils as pu
+import multiprocessing as mp
+from PyQt5.QtWidgets import QMainWindow, QApplication, QTableWidgetItem
+from PyQt5 import QtCore
+from PyQt5.QtGui import QPainter
+from pathlib import Path
+from importlib.resources import files
+from scipy.signal import butter, lfilter, lfiltic, buttord
+from neurodecode.stream_receiver.stream_receiver import StreamReceiver
+from neurodecode import logger
+from configparser import RawConfigParser
+from neurodecode.stream_viewer.ui_mainwindow_Viewer import Ui_MainWindow
+
+class Scope(QMainWindow):
+    def __init__(self, amp_name, amp_serial):
+        super(Scope, self).__init__()
+        self.ui = Ui_MainWindow()
+        self.ui.setupUi(self)
+        self.amp_name = amp_name
+        self.amp_serial = amp_serial
+        self.init_scope()
+        logger.info('Viewer launched')
+
+    #
+    # 	Main init function
+    #
+    def init_scope(self):
+
+        # pg.setConfigOption('background', 'w')
+        # pg.setConfigOption('foreground', 'k')
+
+        self.init_config_file()
+        self.init_loop()
+        self.init_panel_GUI()
+        self.init_scope_GUI()
+        self.init_timer()
+
+    #
+    #	Initializes config file
+    #
+    def init_config_file(self):
+        self.scope_settings = RawConfigParser(allow_no_value=True, inline_comment_prefixes=('#', ';'))
+        if (len(sys.argv) == 1):
+            self.show_channel_names = 0
+            self.device_name = ""
+        else:
+            if (sys.argv[1].find("gtec") > -1):
+                self.device_name = "gtec"
+                self.show_channel_names = 1
+            elif (sys.argv[1].find("biosemi") > -1):
+                self.device_name = "biosemi"
+                self.show_channel_names = 1
+            elif (sys.argv[1].find("hiamp") > -1):
+                self.device_name = "hiamp"
+                self.show_channel_names = 1
+            else:
+                self.device_name = ""
+                self.show_channel_names = 0
+
+        scope_setting_file = files('neurodecode.stream_viewer').joinpath('scope_settings.ini')
+        read_ok = self.scope_settings.read(scope_setting_file)
+        if len(read_ok) == 0:
+            logger.error('Cannot read scope setting file')
+            raise FileNotFoundError(scope_setting_file)
+
+    #
+    # 	Initialize control panel parameter
+    #
+    def init_panel_GUI(self):
+
+        self.show_TID_events = False
+        self.show_LPT_events = False
+        self.show_Key_events = False
+
+        # Event handler
+        self.ui.comboBox_scale.activated.connect(self.onActivated_combobox_scale)
+        self.ui.spinBox_time.valueChanged.connect(self.onValueChanged_spinbox_time)
+        self.ui.checkBox_car.stateChanged.connect(self.onActivated_checkbox_car)
+        self.ui.checkBox_bandpass.stateChanged.connect(
+            self.onActivated_checkbox_bandpass)
+        self.ui.checkBox_showTID.stateChanged.connect(
+            self.onActivated_checkbox_TID)
+        self.ui.checkBox_showLPT.stateChanged.connect(
+            self.onActivated_checkbox_LPT)
+        self.ui.checkBox_showKey.stateChanged.connect(
+            self.onActivated_checkbox_Key)
+        self.ui.pushButton_bp.clicked.connect(self.onClicked_button_bp)
+        self.ui.pushButton_rec.clicked.connect(self.onClicked_button_rec)
+        self.ui.pushButton_stoprec.clicked.connect(self.onClicked_button_stoprec)
+
+        self.ui.pushButton_stoprec.setEnabled(False)
+        self.ui.comboBox_scale.setCurrentIndex(4)
+        self.ui.checkBox_car.setChecked(
+            int(self.scope_settings.get("filtering", "apply_car_filter")))
+        self.ui.checkBox_bandpass.setChecked(
+            int(self.scope_settings.get("filtering", "apply_bandpass_filter")))
+        self.ui.checkBox_showTID.setChecked(
+            int(self.scope_settings.get("plot", "show_TID_events")))
+        self.ui.checkBox_showLPT.setChecked(
+            int(self.scope_settings.get("plot", "show_LPT_events")))
+        self.ui.checkBox_showKey.setChecked(
+            int(self.scope_settings.get("plot", "show_KEY_events")))
+        self.ui.statusBar.showMessage("[Not recording]")
+
+        self.channels_to_show_idx = []
+        idx = 0
+        for y in range(0, 4):
+            for x in range(0, NUM_X_CHANNELS):
+                if (idx < self.config['eeg_channels']):
+                    # self.table_channels.item(x,y).setTextAlignment(QtCore.Qt.AlignCenter)
+                    self.ui.table_channels.item(x, y).setSelected(True) # Qt5
+                    #self.table_channels.setItemSelected(self.table_channels.item(x, y), True) # Qt4 only
+                    self.channels_to_show_idx.append(idx)
+                else:
+                    self.ui.table_channels.setItem(x, y,
+                        QTableWidgetItem("N/A"))
+                    self.ui.table_channels.item(x, y).setFlags(
+                        QtCore.Qt.NoItemFlags)
+                    self.ui.table_channels.item(x, y).setTextAlignment(
+                        QtCore.Qt.AlignCenter)
+                idx += 1
+
+        self.ui.table_channels.verticalHeader().setStretchLastSection(True)
+        self.ui.table_channels.horizontalHeader().setStretchLastSection(True)
+        self.ui.table_channels.itemSelectionChanged.connect(
+            self.onSelectionChanged_table)
+
+        self.screen_width = 522
+        self.screen_height = 160
+        # self.setGeometry(100,100, self.screen_width, self.screen_height)
+        # self.setFixedSize(self.screen_width, self.screen_height)
+        self.setWindowTitle('EEG Scope Panel')
+        self.setFocusPolicy(QtCore.Qt.ClickFocus)
+        self.setFocus()
+        self.show()
+
+    #
+    #	Initialize scope parameters
+    #
+    def init_scope_GUI(self):
+
+        self.bool_parser = {True:'1', False:'0'}
+
+        # PyQTGraph plot initialization
+        self.win = pg.GraphicsLayoutWidget()
+        self.win.setWindowTitle('EEG Scope')
+        self.win.setWindowFlags(QtCore.Qt.WindowMinimizeButtonHint)
+        self.win.keyPressEvent = self.keyPressEvent
+        self.win.show()
+        self.main_plot_handler = self.win.addPlot()
+        self.win.resize(1280, 800)
+
+        # Scales available in the GUI. If you change the options in the GUI
+        # you should change them here as well
+        self.scales_range = [1, 10, 25, 50, 100, 250, 500, 1000, 2500, 100000]
+
+        # Scale in uV
+        self.scale = int(self.scope_settings.get("plot", "scale_plot"))
+        # Time window to show in seconds
+        self.seconds_to_show = int(self.scope_settings.get("plot", "time_plot"))
+
+        # Y Tick labels. Use values from the config file.
+        self.channel_labels = []
+        values = []
+
+        ''' For non-LSL systems having no channel names
+        for x in range(0, self.config['eeg_channels']):
+            if (self.show_channel_names):
+                self.channel_labels.append("(" + str(x + 1) + ") " +
+                    self.scope_settings.get("internal",
+                    "channel_names_" + self.device_name + str(
+                    self.config['eeg_channels'])).split(', ')[x])
+            else:
+                self.channel_labels.append('CH ' + str(x + 1))
+        '''
+        ch_names = np.array( self.sr.get_channel_names() )
+        self.channel_labels = ch_names[ self.sr.get_eeg_channels() ]
+        for x in range(0, len(self.channels_to_show_idx)):
+            values.append((-x * self.scale,
+                self.channel_labels[self.channels_to_show_idx[x]]))
+
+        values_axis = []
+        values_axis.append(values)
+        values_axis.append([])
+
+        # Update table labels with current names
+        idx = 0
+        for y in range(0, 4):
+            for x in range(0, NUM_X_CHANNELS):
+                if (idx < self.config['eeg_channels']):
+                    self.ui.table_channels.item(x, y).setText(
+                        self.channel_labels[idx])
+                idx += 1
+
+        # Plot initialization
+        self.main_plot_handler.getAxis('left').setTicks(values_axis)
+        self.main_plot_handler.setRange(xRange=[0, self.seconds_to_show],
+            yRange=[+1.5 * self.scale,
+                -0.5 * self.scale - self.scale * self.config['eeg_channels']])
+        self.main_plot_handler.disableAutoRange()
+        self.main_plot_handler.showGrid(y=True)
+        self.main_plot_handler.setLabel(axis='left',
+            text='Scale (uV): ' + str(self.scale))
+        self.main_plot_handler.setLabel(axis='bottom', text='Time (s)')
+
+        # X axis
+        self.x_ticks = np.zeros(self.config['sf'] * self.seconds_to_show);
+        for x in range(0, self.config['sf'] * self.seconds_to_show):
+            self.x_ticks[x] = (x * 1) / float(self.config['sf'])
+
+        # Plotting colors. If channels > 16, colors will roll back to the beginning
+        self.colors = np.array(
+            [[255, 0, 0], [0, 255, 0], [0, 0, 255], [255, 255, 0],
+            [0, 255, 255], [255, 0, 255], [128, 100, 100], [0, 128, 0],
+            [0, 128, 128], [128, 128, 0], [255, 128, 128], [128, 0, 128],
+            [128, 255, 0], [255, 128, 0], [0, 255, 128], [128, 0, 255]])
+
+        # We want a lightweight scope, so we downsample the plotting to 64 Hz
+        self.subsampling_value = self.config['sf'] / 64
+
+        # EEG data for plotting
+        self.data_plot = np.zeros((self.config['sf'] * self.seconds_to_show,
+        self.config['eeg_channels']))
+        self.curve_eeg = []
+        for x in range(0, len(self.channels_to_show_idx)):
+            self.curve_eeg.append(self.main_plot_handler.plot(x=self.x_ticks,
+                y=self.data_plot[:, self.channels_to_show_idx[x]],
+                pen=pg.mkColor(
+                    self.colors[self.channels_to_show_idx[x] % 16, :])))
+        # self.curve_eeg[-1].setDownsampling(ds=self.subsampling_value, auto=False, method="mean")
+
+
+        # Events data
+        self.events_detected = []
+        self.events_curves = []
+        self.events_text = []
+
+        # CAR initialization
+        self.apply_car = int(
+            self.scope_settings.get("filtering", "apply_car_filter"))
+        self.matrix_car = np.zeros(
+            (self.config['eeg_channels'], self.config['eeg_channels']),
+            dtype=float)
+        self.matrix_car[:, :] = -1 / float(self.config['eeg_channels'])
+        np.fill_diagonal(self.matrix_car,
+            1 - (1 / float(self.config['eeg_channels'])))
+
+        # Laplacian initalization. TO BE DONE
+        self.matrix_lap = np.zeros(
+            (self.config['eeg_channels'], self.config['eeg_channels']),
+            dtype=float)
+        np.fill_diagonal(self.matrix_lap, 1)
+        '''
+        self.matrix_lap[2, 0] = -1
+        self.matrix_lap[0, 2] = -0.25
+        self.matrix_lap[0, 2] = -0.25
+        '''
+
+        # BP initialization
+        self.apply_bandpass = int(
+            self.scope_settings.get("filtering", "apply_bandpass_filter"))
+        if (self.apply_bandpass):
+            self.ui.doubleSpinBox_hp.setValue(float(
+                self.scope_settings.get("filtering",
+                    "bandpass_cutoff_frequency").split(' ')[0]))
+            self.ui.doubleSpinBox_lp.setValue(float(
+                self.scope_settings.get("filtering",
+                    "bandpass_cutoff_frequency").split(' ')[1]))
+            self.ui.doubleSpinBox_lp.setMinimum(0.1)
+            self.ui.doubleSpinBox_lp.setMaximum(self.sr.sample_rate/2 - 0.1)
+            self.ui.doubleSpinBox_lp.setDecimals(1)
+            self.ui.doubleSpinBox_lp.setSingleStep(1)
+            self.ui.doubleSpinBox_hp.setMinimum(0.1)
+            self.ui.doubleSpinBox_hp.setMaximum(self.sr.sample_rate/2 - 0.1)
+            self.ui.doubleSpinBox_hp.setDecimals(1)
+            self.ui.doubleSpinBox_hp.setSingleStep(1)
+            self.ui.pushButton_bp.click()
+
+        self.ui.checkBox_bandpass.setChecked(self.apply_car)
+        self.ui.checkBox_bandpass.setChecked(self.apply_bandpass)
+
+        self.update_title_scope()
+
+        # Help variables
+        self.show_help = 0
+        self.help = pg.TextItem(
+            "CNBI EEG Scope v0.3 \n" + "----------------------------------------------------------------------------------\n" + "C: De/activate CAR Filter\n" + "B: De/activate Bandpass Filter (with current settings)\n" + "T: Show/hide TiD events\n" + "L: Show/hide LPT events\n" + "K: Show/hide Key events. If not shown, they are NOT recorded!\n" + "0-9: Add a user-specific Key event. Do not forget to write down why you marked it.\n" + "Up, down arrow keys: Increase/decrease the scale, steps of 10 uV\n" + "Left, right arrow keys: Increase/decrease the time to show, steps of 1 s\n" + "Spacebar: Stop the scope plotting, whereas data acquisition keeps running (EXPERIMENTAL)\n" + "Esc: Exits the scope",
+            anchor=(0, 0), border=(70, 70, 70),
+            fill=pg.mkColor(20, 20, 20, 200), color=(255, 255, 255))
+
+        # Stop plot functionality
+        self.stop_plot = 0
+
+        # Force repaint even when we shouldn't repaint.
+        self.force_repaint = 0
+
+    # For some strange reason when the width is > 1 px the scope runs slow.
+    # self.pen_plot = []
+    # for x in range(0, self.config['eeg_channels']):
+    # 	self.pen_plot.append(pg.mkPen(self.colors[x%16,:], width=3))
+
+    #
+    # 	Initializes the BCI loop parameters
+    #
+    def init_loop_cnbiloop(self):
+
+        self.fin = open(self.scope_settings.get("internal", "path_pipe"), 'r')
+
+        # 12 unsigned ints (4 bytes)
+        data = struct.unpack("<12I", self.fin.read(4 * 12))
+
+        self.config = {'id':data[0], 'sf':data[1], 'labels':data[2],
+            'samples':data[3], 'eeg_channels':data[4], 'exg_channels':data[5],
+            'tri_channels':data[6], 'eeg_type':data[8], 'exg_type':data[9],
+            'tri_type':data[10], 'lbl_type':data[11], 'tim_size':1,
+            'idx_size':1}
+
+        self.tri = np.zeros(self.config['samples'])
+        self.eeg = np.zeros(
+            (self.config['samples'], self.config['eeg_channels']),
+            dtype=float)
+        self.exg = np.zeros(
+            (self.config['samples'], self.config['exg_channels']),
+            dtype=float)
+
+        # TID initialization
+        self.bci = BCI.BciInterface()
+
+    #
+    # 	Initializes the BCI loop parameters
+    #
+    def init_loop(self):
+
+        self.updating = False
+
+        self.sr = StreamReceiver(window_size=1, buffer_size=10,
+            amp_serial=self.amp_serial, amp_name=self.amp_name)
+        srate = int(self.sr.sample_rate)
+        # n_channels= self.sr.channels
+
+        # 12 unsigned ints (4 bytes)
+        ########## TODO: assumkng 32 samples chunk => make it read from LSL header
+        data = ['EEG', srate, ['L', 'R'], 32, len(self.sr.get_eeg_channels()),
+            0, self.sr.get_trigger_channel(), None, None, None, None, None]
+        logger.info('Trigger channel is %d' % self.sr.get_trigger_channel())
+
+        self.config = {'id':data[0], 'sf':data[1], 'labels':data[2],
+            'samples':data[3], 'eeg_channels':data[4], 'exg_channels':data[5],
+            'tri_channels':data[6], 'eeg_type':data[8], 'exg_type':data[9],
+            'tri_type':data[10], 'lbl_type':data[11], 'tim_size':1,
+            'idx_size':1}
+
+        self.tri = np.zeros(self.config['samples'])
+        self.last_tri = 0
+        self.eeg = np.zeros(
+            (self.config['samples'], self.config['eeg_channels']),
+            dtype=float)
+        self.exg = np.zeros(
+            (self.config['samples'], self.config['exg_channels']),
+            dtype=float)
+        self.ts_list = []
+        self.ts_list_tri = []
+
+    #
+    # 	Initializes the QT timer, which will call the update function every 20 ms
+    #
+    def init_timer(self):
+
+        self.tm = qc.Timer()  # leeq
+
+        QtCore.QCoreApplication.processEvents()
+        QtCore.QCoreApplication.flush()
+        self.timer = QtCore.QTimer(self)
+        self.timer.timeout.connect(self.update_loop)
+        self.timer.start(20);
+
+    # QtCore.QTimer.singleShot( 20, self.update_loop )
+
+
+    #
+    #	Main update function (connected to the timer)
+    #
+    def update_loop(self):
+        try:
+            # assert self.updating==False, 'thread destroyed?'
+            # self.updating= True
+            # self.handle_tobiid_input()	# Read TiDs
+            self.read_eeg()  # Read new chunk
+            if len(self.ts_list) > 0:
+                self.filter_signal()  # Filter acquired data
+                self.update_ringbuffers()  # Update the plotting infor
+                if (not self.stop_plot):
+                    self.repaint()  # Call paint event
+        except:
+            logger.exception('Exception. Dropping into a shell.')
+            pdb.set_trace()
+        finally:
+            # self.updating= False
+            # using singleShot instead
+            # QtCore.QTimer.singleShot( 20, self.update_loop )
+            pass
+
+    #
+    #	Read EEG
+    #
+    def read_eeg(self):
+
+        # if self.updating==True: print( '##### ERROR: thread destroyed ? ######' )
+        # self.updating= True
+
+        try:
+            # data, self.ts_list= self.sr.inlets[0].pull_chunk(max_samples=self.config['sf']) # [frames][channels]
+            data, self.ts_list = self.sr.acquire(blocking=False)
+
+            # TODO: check and change to these two lines
+            #self.sr.acquire(blocking=False, decim=DECIM)
+            #data, self.ts_list = self.sr.get_window()
+
+            if len(self.ts_list) == 0:
+                # self.eeg= None
+                # self.tri= None
+                return
+
+            n = self.config['eeg_channels']
+            '''
+            x= np.array( data )
+            trg_ch= self.config['tri_channels']
+            if trg_ch is not None:
+                self.tri= np.reshape( x[:,trg_ch], (-1,1) ) # samples x 1
+            self.eeg= np.reshape( x[:,self.sr.eeg_channels], (-1,n) ) # samples x channels
+            '''
+            trg_ch = self.config['tri_channels']
+            if trg_ch is not None:
+                self.tri = np.reshape(data[:, trg_ch], (-1, 1))  # samples x 1
+            self.eeg = np.reshape(data[:, self.sr.eeg_channels],
+                (-1, n))  # samples x channels
+
+            if DEBUG_TRIGGER:
+                # show trigger value
+                try:
+                    trg_value = max(self.tri)
+                    if trg_value > 0:
+                        logger.info('Received trigger %s' % trg_value)
+                except:
+                    logger.exception('Error! self.tri = %s' % self.tri)
+
+                    # Read exg. self.config.samples*self.config.exg_ch, type float
+                    # bexg = np.random.rand( 1, self.config['samples'] * self.config['exg_channels'] )
+                    # self.exg = np.reshape(list(bexg), (self.config['samples'],self.config['exg_channels']))
+        except WindowsError:
+            # print('**** Access violation in read_eeg():\n%s\n%s'% (sys.exc_info()[0], sys.exc_info()[1]))
+            pass
+        except:
+            logger.exception()
+            pdb.set_trace()
+
+    #
+    #	Read EEG
+    #
+    def read_eeg_cnbiloop(self):
+
+        # Reading in python is blocking, so it will wait until having the amount of data needed
+        # Read timestamp. 1 value, type double
+        timestamp = struct.unpack("<d", self.fin.read(8 * 1))
+        # Read index. 1 value, type uint64
+        index = struct.unpack("<Q", self.fin.read(8 * 1))
+        # Read labels. self.config.labels, type double
+        labels = struct.unpack("<" + str(self.config['labels']) + "I",
+            self.fin.read(4 * self.config['labels']))
+        # Read eeg. self.config.samples*self.config.eeg_ch, type float
+        beeg = struct.unpack("<" + str(
+            self.config['samples'] * self.config['eeg_channels']) + "f",
+            self.fin.read(
+                4 * self.config['samples'] * self.config['eeg_channels']))
+        self.eeg = np.reshape(list(beeg),
+            (self.config['samples'], self.config['eeg_channels']))
+        # Read exg. self.config.samples*self.config.exg_ch, type float
+        bexg = struct.unpack("<" + str(
+            self.config['samples'] * self.config['exg_channels']) + "f",
+            self.fin.read(
+                4 * self.config['samples'] * self.config['exg_channels']))
+        self.exg = np.reshape(list(bexg),
+            (self.config['samples'], self.config['exg_channels']))
+        # Read tri. self.config.samples*self.config.tri_ch, type float
+        self.tri = struct.unpack("<" + str(
+            self.config['samples'] * self.config['tri_channels']) + "i",
+            self.fin.read(
+                4 * self.config['samples'] * self.config['tri_channels']))
+
+    #
+    #	Bandpas + CAR filtering
+    #
+    def filter_signal(self):
+
+        if (self.apply_bandpass):
+            for x in range(0, self.eeg.shape[1]):
+                self.eeg[:, x], self.zi[:, x] = lfilter(self.b, self.a,
+                    self.eeg[:, x], -1, self.zi[:, x])
+
+        # We only apply CAR if selected AND there are at least 2 channels. Otherwise it makes no sense
+        if (self.apply_car) and (len(self.channels_to_show_idx) > 1):
+            self.eeg = np.dot(self.matrix_car, np.transpose(self.eeg))
+            self.eeg = np.transpose(self.eeg)
+
+    #
+    #	Update ringbuffers and events for plotting
+    #
+    def update_ringbuffers(self):
+        # leeq
+        self.data_plot = np.roll(self.data_plot, -len(self.ts_list), 0)
+        self.data_plot[-len(self.ts_list):, :] = self.eeg
+
+        # We have to remove those indexes that reached time = 0
+        delete_indices_e = []
+        delete_indices_c = []
+        for x in range(0, len(self.events_detected), 2):
+            xh = int(x / 2)
+            self.events_detected[x] -= len(self.ts_list)  # leeq
+            if (self.events_detected[x] < 0) and (not self.stop_plot):
+                delete_indices_e.append(x)
+                delete_indices_e.append(x + 1)
+                delete_indices_c.append(xh)
+                self.events_curves[xh].clear()
+                self.main_plot_handler.removeItem(self.events_text[xh])
+
+        self.events_detected = [i for j, i in enumerate(self.events_detected) if
+            j not in delete_indices_e]
+        self.events_curves = [i for j, i in enumerate(self.events_curves) if
+            j not in delete_indices_c]
+        self.events_text = [i for j, i in enumerate(self.events_text) if
+            j not in delete_indices_c]
+
+        # Find LPT events and add them
+        if (self.show_LPT_events) and (not self.stop_plot):
+            for x in range(len(self.tri)):
+                tri = int(self.tri[x])
+                if tri != 0 and (tri > self.last_tri):
+                    self.addEventPlot("LPT", tri)
+                    logger.info('Trigger %d received' % tri)
+                self.last_tri = tri
+
+    #
+    #	Called by repaint()
+    #
+    def paintEvent(self, e):
+        # Distinguish between paint events from timer and event QT widget resizing, clicking etc (sender is None)
+        # We should only paint when the timer triggered the event.
+        # Just in case, there's a flag to force a repaint even when we shouldn't repaint
+        sender = self.sender()
+        if 'force_repaint' not in self.__dict__.keys():
+            logger.warning('force_repaint is not set! Is it a Qt bug?')
+            self.force_repaint = 0
+        if (sender is None) and (not self.force_repaint):
+            pass
+        else:
+            self.force_repaint = 0
+            qp = QPainter()
+            qp.begin(self)
+            # Update the interface
+            self.paintInterface(qp)
+            qp.end()
+
+    #
+    #	Update stuff on the interface. Only graphical updates should be added here
+    #
+    def paintInterface(self, qp):
+
+        # Update EEG channels
+        for x in range(0, len(self.channels_to_show_idx)):
+            self.curve_eeg[x].setData(x=self.x_ticks, y=self.data_plot[:,self.channels_to_show_idx[x]] - x * self.scale)
+
+        # Update events
+        for x in range(0, len(self.events_detected), 2):
+            xh = int(x / 2)
+            self.events_curves[xh].setData(x=np.array(
+                [self.x_ticks[self.events_detected[x]],
+                    self.x_ticks[self.events_detected[x]]]), y=np.array(
+                [+1.5 * self.scale,
+                    -0.5 * self.scale - self.scale * self.config[
+                        'eeg_channels']]))
+            self.events_text[xh].setPos(self.x_ticks[self.events_detected[x]],
+                self.scale)
+
+    #
+    #	Do necessary stuff when scale has changed
+    #
+    def update_plot_scale(self, new_scale):
+
+        if (new_scale < 1):
+            new_scale = 1
+        # commented out by dbdq.
+        # else:
+        #	new_scale = new_scale - new_scale%10
+
+        self.scale = new_scale
+
+        # Y Tick labels
+        values = []
+        for x in range(0, len(self.channels_to_show_idx)):
+            values.append((-x * self.scale,
+            self.channel_labels[self.channels_to_show_idx[x]]))
+
+        values_axis = []
+        values_axis.append(values)
+        values_axis.append([])
+
+        self.main_plot_handler.getAxis('left').setTicks(values_axis)
+        self.main_plot_handler.setRange(
+            yRange=[+self.scale, -self.scale * len(self.channels_to_show_idx)])
+        self.main_plot_handler.setLabel(axis='left',
+            text='Scale (uV): ' + str(self.scale))
+        self.trigger_help()
+
+        # We force an immediate repaint to avoid "shakiness".
+        if (not self.stop_plot):
+            self.force_repaint = 1
+            self.repaint()
+
+    #
+    #	Do necessary stuff when seconds to show have changed
+    #
+    def update_plot_seconds(self, new_seconds):
+
+        # Do nothing unless...
+        if (new_seconds != self.seconds_to_show) and (new_seconds > 0) and (
+                new_seconds < 100):
+            self.ui.spinBox_time.setValue(new_seconds)
+            self.main_plot_handler.setRange(xRange=[0, new_seconds])
+            self.x_ticks = np.zeros(self.config['sf'] * new_seconds);
+            for x in range(0, self.config['sf'] * new_seconds):
+                self.x_ticks[x] = (x * 1) / float(self.config['sf'])
+
+            if (new_seconds > self.seconds_to_show):
+                padded_signal = np.zeros((self.config['sf'] * new_seconds,
+                self.config['eeg_channels']))
+                padded_signal[padded_signal.shape[0] - self.data_plot.shape[0]:,
+                :] = self.data_plot
+                for x in range(0, len(self.events_detected), 2):
+                    self.events_detected[x] += padded_signal.shape[0] - \
+                                               self.data_plot.shape[0]
+                self.data_plot = padded_signal
+
+            else:
+                for x in range(0, len(self.events_detected), 2):
+                    self.events_detected[x] -= self.data_plot.shape[0] - \
+                                               self.config['sf'] * new_seconds
+                self.data_plot = self.data_plot[
+                self.data_plot.shape[0] - self.config['sf'] * new_seconds:, :]
+
+            self.seconds_to_show = new_seconds
+            self.trigger_help()
+
+            # We force an immediate repaint to avoid "shakiness".
+            if (not self.stop_plot):
+                self.force_repaint = 1
+                self.repaint()
+
+    #
+    # Handle TOBI iD events
+    #
+    def handle_tobiid_input(self):
+
+        data = None
+        try:
+            data = self.bci.iDsock_bus.recv(512)
+            self.bci.idStreamer_bus.Append(data)
+        except:
+            self.nS = False
+            self.dec = 0
+            pass
+
+        # deserialize ID message
+        if data:
+            if self.bci.idStreamer_bus.Has("<tobiid", "/>"):
+                msg = self.bci.idStreamer_bus.Extract("<tobiid", "/>")
+                self.bci.id_serializer_bus.Deserialize(msg)
+                self.bci.idStreamer_bus.Clear()
+                tmpmsg = int(self.bci.id_msg_bus.GetEvent())
+                if (self.show_TID_events) and (not self.stop_plot):
+                    self.addEventPlot("TID", tmpmsg)
+
+            elif self.bci.idStreamer_bus.Has("<tcstatus", "/>"):
+                MsgNum = self.bci.idStreamer_bus.Count("<tcstatus")
+                for i in range(1, MsgNum - 1):
+                    # Extract most of these messages and trash them
+                    msg_useless = self.bci.idStreamer_bus.Extract("<tcstatus",
+                        "/>")
+
+    #
+    # 	Add an event to the scope
+    #
+    def addEventPlot(self, event_name, event_id):
+        if (event_name == "TID"):
+            color = pg.mkColor(0, 0, 255)
+        elif (event_name == "KEY"):
+            color = pg.mkColor(255, 0, 0)
+        elif (event_name == "LPT"):
+            color = pg.mkColor(0, 255, 0)
+        else:
+            color = pg.mkColor(255, 255, 255)
+
+        self.events_detected.append(self.data_plot.shape[0] - 1)
+        self.events_detected.append(event_id)
+        self.events_curves.append(self.main_plot_handler.plot(pen=color,
+            x=np.array([self.x_ticks[-1], self.x_ticks[-1]]), y=np.array(
+                [+1.5 * self.scale,
+                    -1.5 * self.scale * self.config['eeg_channels']])))
+        # text = pg.TextItem(event_name + "(" + str(self.events_detected[-1]) + ")", anchor=(1.1,0), fill=(0,0,0), color=color)
+        text = pg.TextItem(str(self.events_detected[-1]), anchor=(1.1, 0),
+            fill=(0, 0, 0), color=color)
+        text.setPos(self.x_ticks[-1], self.scale)
+        self.events_text.append(text)
+        self.main_plot_handler.addItem(self.events_text[-1])
+
+    #
+    #	Calculation of bandpass coefficients.
+    #	Order is computed automatically.
+    #	Note that if filter is unstable this function crashes (TODO handle problems)
+    #
+    def butter_bandpass(self, highcut, lowcut, fs, num_ch):
+        low = lowcut / (0.5 * fs)
+        high = highcut / (0.5 * fs)
+        # get the order. TO BE DONE: Sometimes it fails
+        #ord = buttord(high, low, 2, 40)
+        #b, a = butter(ord[0], [high, low], btype='band')
+        b, a = butter(2, [high, low], btype='band')
+        zi = np.zeros([a.shape[0] - 1, num_ch])
+        return b, a, zi
+
+    #
+    #	Updates the title shown in the scope
+    #
+    def update_title_scope(self):
+        if (hasattr(self, 'main_plot_handler')):
+            self.main_plot_handler.setTitle(
+                title='TLK: ' + self.bool_parser[self.show_TID_events] +
+                      self.bool_parser[self.show_LPT_events] + self.bool_parser[
+                          self.show_Key_events] + ', CAR: ' + self.bool_parser[
+                          self.apply_car] + ', BP: ' + self.bool_parser[
+                          self.apply_bandpass] + ' [' + str(
+                    self.ui.doubleSpinBox_hp.value()) + '-' + str(
+                    self.ui.doubleSpinBox_lp.value()) + '] Hz')
+            # ', BP: ' + self.bool_parser[self.apply_bandpass] + (' [' + str(self.doubleSpinBox_hp.value()) + '-' + str(self.doubleSpinBox_lp.value()) + '] Hz' if self.apply_bandpass else ''))
+
+    #
+    #	Shows / hide help in the scope window
+    #
+    def trigger_help(self):
+        if self.show_help:
+            self.help.setPos(0, self.scale)
+            self.main_plot_handler.addItem(self.help)
+            self.help.setZValue(1)
+        else:
+            self.main_plot_handler.removeItem(self.help)
+
+    # ----------------------------------------------------------------------------------------------------
+    # 			EVENT HANDLERS
+    # ----------------------------------------------------------------------------------------------------
+    def onClicked_button_rec(self):
+        # Simply call cl_rpc for this.
+        if (len(self.lineEdit_recFilename.text()) > 0):
+            if ".gdf" in self.lineEdit_recFilename.text():
+                self.ui.pushButton_stoprec.setEnabled(True)
+                self.ui.pushButton_rec.setEnabled(False)
+                # Popen is more efficient than os.open, since it is non-blocking
+                subprocess.Popen(
+                    ["cl_rpc", "openxdf", str(self.ui.lineEdit_recFilename.text()),
+                        "dummy_log", "dummy_log"], close_fds=True)
+                self.statusBar.showMessage(
+                    "Recording file " + str(self.ui.lineEdit_recFilename.text()))
+            elif ".bdf" in self.ui.lineEdit_recFilename.text():
+                self.ui.pushButton_stoprec.setEnabled(True)
+                self.ui.pushButton_rec.setEnabled(False)
+                subprocess.Popen(
+                    ["cl_rpc", "openxdf", str(self.ui.lineEdit_recFilename.text()),
+                        "dummy_log", "dummy_log"], close_fds=True)
+                self.statusBar.showMessage(
+                    "Recording file " + str(self.ui.lineEdit_recFilename.text()))
+            else:
+                pass
+
+    def onClicked_button_stoprec(self):
+        subprocess.Popen(["cl_rpc", "closexdf"], close_fds=True)
+        self.ui.pushButton_rec.setEnabled(True)
+        self.ui.pushButton_stoprec.setEnabled(False)
+        self.ui.statusBar.showMessage("Not recording")
+
+    def onActivated_checkbox_bandpass(self):
+        self.apply_bandpass = False
+        self.ui.pushButton_bp.setEnabled(self.ui.checkBox_bandpass.isChecked())
+        self.ui.doubleSpinBox_hp.setEnabled(self.ui.checkBox_bandpass.isChecked())
+        self.ui.doubleSpinBox_lp.setEnabled(self.ui.checkBox_bandpass.isChecked())
+        self.update_title_scope()
+
+    def onActivated_checkbox_car(self):
+        self.apply_car = self.ui.checkBox_car.isChecked()
+        self.update_title_scope()
+
+    def onActivated_checkbox_TID(self):
+        self.show_TID_events = self.ui.checkBox_showTID.isChecked()
+        self.update_title_scope()
+
+    def onActivated_checkbox_LPT(self):
+        self.show_LPT_events = self.ui.checkBox_showLPT.isChecked()
+        self.update_title_scope()
+
+    def onActivated_checkbox_Key(self):
+        self.show_Key_events = self.ui.checkBox_showKey.isChecked()
+        self.update_title_scope()
+
+    def onValueChanged_spinbox_time(self):
+        self.update_plot_seconds(self.ui.spinBox_time.value())
+
+    def onActivated_combobox_scale(self):
+        self.update_plot_scale(
+            self.scales_range[self.ui.comboBox_scale.currentIndex()])
+
+    def onClicked_button_bp(self):
+        if (self.ui.doubleSpinBox_lp.value() > self.ui.doubleSpinBox_hp.value()):
+            self.apply_bandpass = True
+            self.b, self.a, self.zi = self.butter_bandpass(
+                self.ui.doubleSpinBox_hp.value(), self.ui.doubleSpinBox_lp.value(),
+                self.config['sf'], self.config['eeg_channels'])
+        self.update_title_scope()
+
+    def onSelectionChanged_table(self):
+
+        # Remove current plot
+        for x in range(0, len(self.channels_to_show_idx)):
+            self.main_plot_handler.removeItem(self.curve_eeg[x])
+
+        # Which channels should I plot?
+        self.channels_to_show_idx = []
+        self.channels_to_hide_idx = []
+        idx = 0
+        for y in range(0, 4):
+            for x in range(0, NUM_X_CHANNELS):
+                if (idx < self.config['eeg_channels']):
+                    #if (self.table_channels.isItemSelected( # Qt4 only
+                    if (QTableWidgetItem.isSelected( # Qt5
+                        self.ui.table_channels.item(x, y))):
+                        self.channels_to_show_idx.append(idx)
+                    else:
+                        self.channels_to_hide_idx.append(idx)
+                    idx += 1
+
+        # Add new plots
+        self.curve_eeg = []
+        for x in range(0, len(self.channels_to_show_idx)):
+            self.curve_eeg.append(self.main_plot_handler.plot(x=self.x_ticks,
+                y=self.data_plot[:, self.channels_to_show_idx[x]],
+                pen=self.colors[self.channels_to_show_idx[x] % NUM_X_CHANNELS, :]))
+            self.curve_eeg[-1].setDownsampling(ds=self.subsampling_value,
+                auto=False, method="mean")
+
+        # Update CAR so it's computed based only on the shown channels
+        if (len(self.channels_to_show_idx) > 1):
+            self.matrix_car = np.zeros(
+                (self.config['eeg_channels'], self.config['eeg_channels']),
+                dtype=float)
+            self.matrix_car[:, :] = -1 / float(len(self.channels_to_show_idx))
+            np.fill_diagonal(self.matrix_car,
+                1 - (1 / float(len(self.channels_to_show_idx))))
+            for x in range(0, len(self.channels_to_hide_idx)):
+                self.matrix_car[self.channels_to_hide_idx[x], :] = 0
+                self.matrix_car[:, self.channels_to_hide_idx[x]] = 0
+
+        # Refresh the plot
+        self.update_plot_scale(self.scale)
+
+    def keyPressEvent(self, event):
+        key = event.key()
+        if (key == QtCore.Qt.Key_Escape):
+            self.closeEvent(None)
+        if (key == QtCore.Qt.Key_H):
+            self.show_help = not self.show_help
+            self.trigger_help()
+        if (key == QtCore.Qt.Key_Up):
+            # Python's log(x, 10) has a rounding bug. Use log10(x) instead.
+            new_scale = self.scale + max(1, 10 ** int(math.log10(self.scale)))
+            self.update_plot_scale(new_scale)
+        if (key == QtCore.Qt.Key_Space):
+            self.stop_plot = not self.stop_plot
+        if (key == QtCore.Qt.Key_Down):
+            if self.scale >= 2:
+                # Python's log(x, 10) has a rounding bug. Use log10(x) instead.
+                new_scale = self.scale - max(1,
+                    10 ** int(math.log10(self.scale - 1)))
+                self.update_plot_scale(new_scale)
+        if (key == QtCore.Qt.Key_Left):
+            self.update_plot_seconds(self.seconds_to_show - 1)
+        if (key == QtCore.Qt.Key_Right):
+            self.update_plot_seconds(self.seconds_to_show + 1)
+        if (key == QtCore.Qt.Key_L):
+            self.ui.checkBox_showLPT.setChecked(
+                not self.ui.checkBox_showLPT.isChecked())
+        if (key == QtCore.Qt.Key_T):
+            self.ui.checkBox_showTID.setChecked(
+                not self.ui.checkBox_showTID.isChecked())
+        if (key == QtCore.Qt.Key_K):
+            self.ui.checkBox_showKey.setChecked(
+                not self.ui.checkBox_showKey.isChecked())
+        if (key == QtCore.Qt.Key_C):
+            self.ui.checkBox_car.setChecked(not self.ui.checkBox_car.isChecked())
+        if (key == QtCore.Qt.Key_B):
+            self.ui.checkBox_bandpass.setChecked(
+                not self.ui.checkBox_bandpass.isChecked())
+            if self.ui.checkBox_bandpass.isChecked():
+                self.ui.pushButton_bp.click()
+        if ((key >= QtCore.Qt.Key_0) and (key <= QtCore.Qt.Key_9)):
+            if (self.show_Key_events) and (not self.stop_plot):
+                self.addEventPlot("KEY", 990 + key - QtCore.Qt.Key_0)
+
+    #
+    #	Function called when a closing event was triggered.
+    #
+    def closeEvent(self, event):
+        '''
+        reply = QtGui.QMessageBox.question(self, "Quit", "Are you sure you want to quit?", QtGui.QMessageBox.Yes | QtGui.QMessageBox.No, QtGui.QMessageBox.Yes)
+        if (reply == QtGui.QMessageBox.Yes):
+            if (self.pushButton_stoprec.isEnabled()):
+                subprocess.Popen(["cl_rpc", "closexdf"], close_fds=True)
+            self.fin.close()
+            exit()
+        '''
+
+        # leeq
+        if (self.ui.pushButton_stoprec.isEnabled()):
+            subprocess.Popen(["cl_rpc", "closexdf"], close_fds=True)
+
+        QApplication.instance().closeAllWindows()
+        # ----------------------------------------------------------------------------------------------------
+        # 		END OF EVENT HANDLERS
+        # ----------------------------------------------------------------------------------------------------
+
+
+def main():
+    """
+    Invoked from console
+    """
+    if len(sys.argv) == 1:
+        amp_name, amp_serial = pu.search_lsl()
+    elif len(sys.argv) == 2:
+        amp_name, amp_serial = sys.argv[1], None
+    else:
+        amp_name, amp_serial = sys.argv[1:3]
+    logger.info('Connecting to a server %s (Serial %s).' % (amp_name, amp_serial))
+
+    app = QApplication(sys.argv)
+    Scope(amp_name, amp_serial)
+    sys.exit(app.exec_())
+
+if __name__ == '__main__':
+    main()
```

### Comparing `neurodecode-2.0.4/neurodecode/stream_viewer/ui_mainwindow_Viewer.py` & `neurodecode-2.0.5/neurodecode/stream_viewer/ui_mainwindow_Viewer.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,491 +1,491 @@
-# -*- coding: utf-8 -*-
-
-# Form implementation generated from reading ui file 'mainwindow.ui'
-#
-# Created by: PyQt5 UI code generator 5.12.1
-#
-# WARNING! All changes made in this file will be lost!
-
-from PyQt5 import QtCore, QtGui, QtWidgets
-
-
-class Ui_MainWindow(object):
-    def setupUi(self, MainWindow):
-        MainWindow.setObjectName("MainWindow")
-        MainWindow.resize(533, 688)
-        self.centralWidget = QtWidgets.QWidget(MainWindow)
-        self.centralWidget.setObjectName("centralWidget")
-        self.comboBox_scale = QtWidgets.QComboBox(self.centralWidget)
-        self.comboBox_scale.setGeometry(QtCore.QRect(10, 20, 85, 27))
-        self.comboBox_scale.setObjectName("comboBox_scale")
-        self.comboBox_scale.addItem("")
-        self.comboBox_scale.addItem("")
-        self.comboBox_scale.addItem("")
-        self.comboBox_scale.addItem("")
-        self.comboBox_scale.addItem("")
-        self.comboBox_scale.addItem("")
-        self.comboBox_scale.addItem("")
-        self.comboBox_scale.addItem("")
-        self.comboBox_scale.addItem("")
-        self.comboBox_scale.addItem("")
-        self.checkBox_car = QtWidgets.QCheckBox(self.centralWidget)
-        self.checkBox_car.setGeometry(QtCore.QRect(120, 0, 97, 22))
-        self.checkBox_car.setObjectName("checkBox_car")
-        self.label_2 = QtWidgets.QLabel(self.centralWidget)
-        self.label_2.setGeometry(QtCore.QRect(10, 60, 67, 17))
-        self.label_2.setObjectName("label_2")
-        self.label_3 = QtWidgets.QLabel(self.centralWidget)
-        self.label_3.setGeometry(QtCore.QRect(10, 0, 67, 17))
-        self.label_3.setObjectName("label_3")
-        self.checkBox_bandpass = QtWidgets.QCheckBox(self.centralWidget)
-        self.checkBox_bandpass.setGeometry(QtCore.QRect(120, 20, 141, 22))
-        self.checkBox_bandpass.setObjectName("checkBox_bandpass")
-        self.pushButton_bp = QtWidgets.QPushButton(self.centralWidget)
-        self.pushButton_bp.setGeometry(QtCore.QRect(410, 20, 99, 27))
-        self.pushButton_bp.setObjectName("pushButton_bp")
-        self.spinBox_time = QtWidgets.QSpinBox(self.centralWidget)
-        self.spinBox_time.setGeometry(QtCore.QRect(10, 80, 85, 27))
-        self.spinBox_time.setMinimum(1)
-        self.spinBox_time.setProperty("value", 5)
-        self.spinBox_time.setObjectName("spinBox_time")
-        self.doubleSpinBox_hp = QtWidgets.QDoubleSpinBox(self.centralWidget)
-        self.doubleSpinBox_hp.setGeometry(QtCore.QRect(260, 20, 69, 27))
-        self.doubleSpinBox_hp.setMinimum(0.1)
-        self.doubleSpinBox_hp.setSingleStep(0.1)
-        self.doubleSpinBox_hp.setProperty("value", 1.0)
-        self.doubleSpinBox_hp.setObjectName("doubleSpinBox_hp")
-        self.doubleSpinBox_lp = QtWidgets.QDoubleSpinBox(self.centralWidget)
-        self.doubleSpinBox_lp.setGeometry(QtCore.QRect(340, 20, 69, 27))
-        self.doubleSpinBox_lp.setMinimum(1.0)
-        self.doubleSpinBox_lp.setSingleStep(0.1)
-        self.doubleSpinBox_lp.setProperty("value", 50.0)
-        self.doubleSpinBox_lp.setObjectName("doubleSpinBox_lp")
-        self.checkBox_showTID = QtWidgets.QCheckBox(self.centralWidget)
-        self.checkBox_showTID.setGeometry(QtCore.QRect(120, 60, 161, 22))
-        self.checkBox_showTID.setObjectName("checkBox_showTID")
-        self.checkBox_showLPT = QtWidgets.QCheckBox(self.centralWidget)
-        self.checkBox_showLPT.setGeometry(QtCore.QRect(120, 80, 151, 22))
-        self.checkBox_showLPT.setObjectName("checkBox_showLPT")
-        self.checkBox_showKey = QtWidgets.QCheckBox(self.centralWidget)
-        self.checkBox_showKey.setGeometry(QtCore.QRect(120, 100, 151, 22))
-        self.checkBox_showKey.setObjectName("checkBox_showKey")
-        self.line = QtWidgets.QFrame(self.centralWidget)
-        self.line.setGeometry(QtCore.QRect(100, 0, 21, 121))
-        self.line.setFrameShape(QtWidgets.QFrame.VLine)
-        self.line.setFrameShadow(QtWidgets.QFrame.Sunken)
-        self.line.setObjectName("line")
-        self.line_2 = QtWidgets.QFrame(self.centralWidget)
-        self.line_2.setGeometry(QtCore.QRect(110, 45, 431, 21))
-        self.line_2.setFrameShape(QtWidgets.QFrame.HLine)
-        self.line_2.setFrameShadow(QtWidgets.QFrame.Sunken)
-        self.line_2.setObjectName("line_2")
-        self.line_3 = QtWidgets.QFrame(self.centralWidget)
-        self.line_3.setGeometry(QtCore.QRect(290, 60, 21, 61))
-        self.line_3.setFrameShape(QtWidgets.QFrame.VLine)
-        self.line_3.setFrameShadow(QtWidgets.QFrame.Sunken)
-        self.line_3.setObjectName("line_3")
-        self.pushButton_stoprec = QtWidgets.QPushButton(self.centralWidget)
-        self.pushButton_stoprec.setGeometry(QtCore.QRect(310, 90, 201, 27))
-        self.pushButton_stoprec.setObjectName("pushButton_stoprec")
-        self.pushButton_rec = QtWidgets.QPushButton(self.centralWidget)
-        self.pushButton_rec.setGeometry(QtCore.QRect(460, 60, 51, 27))
-        self.pushButton_rec.setObjectName("pushButton_rec")
-        self.lineEdit_recFilename = QtWidgets.QLineEdit(self.centralWidget)
-        self.lineEdit_recFilename.setGeometry(QtCore.QRect(310, 60, 141, 27))
-        self.lineEdit_recFilename.setObjectName("lineEdit_recFilename")
-        self.table_channels = QtWidgets.QTableWidget(self.centralWidget)
-        self.table_channels.setGeometry(QtCore.QRect(60, 140, 411, 491))
-        self.table_channels.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
-        self.table_channels.setTextElideMode(QtCore.Qt.ElideMiddle)
-        self.table_channels.setShowGrid(False)
-        self.table_channels.setObjectName("table_channels")
-        self.table_channels.setColumnCount(4)
-        self.table_channels.setRowCount(16)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setVerticalHeaderItem(0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setVerticalHeaderItem(1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setVerticalHeaderItem(2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setVerticalHeaderItem(3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setVerticalHeaderItem(4, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setVerticalHeaderItem(5, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setVerticalHeaderItem(6, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setVerticalHeaderItem(7, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setVerticalHeaderItem(8, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setVerticalHeaderItem(9, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setVerticalHeaderItem(10, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setVerticalHeaderItem(11, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setVerticalHeaderItem(12, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setVerticalHeaderItem(13, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setVerticalHeaderItem(14, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setVerticalHeaderItem(15, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setHorizontalHeaderItem(0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setHorizontalHeaderItem(1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setHorizontalHeaderItem(2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setHorizontalHeaderItem(3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(0, 0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(0, 1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(0, 2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(0, 3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(1, 0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(1, 1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(1, 2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(1, 3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(2, 0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(2, 1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(2, 2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(2, 3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(3, 0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(3, 1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(3, 2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(3, 3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(4, 0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(4, 1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(4, 2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(4, 3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(5, 0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(5, 1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(5, 2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(5, 3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(6, 0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(6, 1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(6, 2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(6, 3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(7, 0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(7, 1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(7, 2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(7, 3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(8, 0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(8, 1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(8, 2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(8, 3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(9, 0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(9, 1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(9, 2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(9, 3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(10, 0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(10, 1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(10, 2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(10, 3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(11, 0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(11, 1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(11, 2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(11, 3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(12, 0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(12, 1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(12, 2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(12, 3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(13, 0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(13, 1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(13, 2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(13, 3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(14, 0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(14, 1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(14, 2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(14, 3, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(15, 0, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(15, 1, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(15, 2, item)
-        item = QtWidgets.QTableWidgetItem()
-        self.table_channels.setItem(15, 3, item)
-        self.table_channels.horizontalHeader().setVisible(False)
-        self.table_channels.horizontalHeader().setHighlightSections(False)
-        self.table_channels.verticalHeader().setVisible(False)
-        self.table_channels.verticalHeader().setHighlightSections(False)
-        self.line_4 = QtWidgets.QFrame(self.centralWidget)
-        self.line_4.setGeometry(QtCore.QRect(0, 120, 531, 21))
-        self.line_4.setFrameShape(QtWidgets.QFrame.HLine)
-        self.line_4.setFrameShadow(QtWidgets.QFrame.Sunken)
-        self.line_4.setObjectName("line_4")
-        MainWindow.setCentralWidget(self.centralWidget)
-        self.menuBar = QtWidgets.QMenuBar(MainWindow)
-        self.menuBar.setGeometry(QtCore.QRect(0, 0, 533, 25))
-        self.menuBar.setObjectName("menuBar")
-        MainWindow.setMenuBar(self.menuBar)
-        self.mainToolBar = QtWidgets.QToolBar(MainWindow)
-        self.mainToolBar.setObjectName("mainToolBar")
-        MainWindow.addToolBar(QtCore.Qt.TopToolBarArea, self.mainToolBar)
-        self.statusBar = QtWidgets.QStatusBar(MainWindow)
-        self.statusBar.setObjectName("statusBar")
-        MainWindow.setStatusBar(self.statusBar)
-
-        self.retranslateUi(MainWindow)
-        QtCore.QMetaObject.connectSlotsByName(MainWindow)
-
-    def retranslateUi(self, MainWindow):
-        _translate = QtCore.QCoreApplication.translate
-        MainWindow.setWindowTitle(_translate("MainWindow", "MainWindow"))
-        self.comboBox_scale.setItemText(0, _translate("MainWindow", "1uV"))
-        self.comboBox_scale.setItemText(1, _translate("MainWindow", "10uV"))
-        self.comboBox_scale.setItemText(2, _translate("MainWindow", "25uV"))
-        self.comboBox_scale.setItemText(3, _translate("MainWindow", "50uV"))
-        self.comboBox_scale.setItemText(4, _translate("MainWindow", "100uV"))
-        self.comboBox_scale.setItemText(5, _translate("MainWindow", "250uV"))
-        self.comboBox_scale.setItemText(6, _translate("MainWindow", "500uV"))
-        self.comboBox_scale.setItemText(7, _translate("MainWindow", "1mV"))
-        self.comboBox_scale.setItemText(8, _translate("MainWindow", "2.5mV"))
-        self.comboBox_scale.setItemText(9, _translate("MainWindow", "100mV"))
-        self.checkBox_car.setText(_translate("MainWindow", "CAR Filter"))
-        self.label_2.setText(_translate("MainWindow", "Time (s)"))
-        self.label_3.setText(_translate("MainWindow", "Scale"))
-        self.checkBox_bandpass.setText(_translate("MainWindow", "Bandpass Filter"))
-        self.pushButton_bp.setText(_translate("MainWindow", "Apply BP"))
-        self.checkBox_showTID.setText(_translate("MainWindow", "Show TID events"))
-        self.checkBox_showLPT.setText(_translate("MainWindow", "Show LPT events"))
-        self.checkBox_showKey.setText(_translate("MainWindow", "Show Key events"))
-        self.pushButton_stoprec.setText(_translate("MainWindow", "Stop REC"))
-        self.pushButton_rec.setText(_translate("MainWindow", "REC"))
-        item = self.table_channels.verticalHeaderItem(0)
-        item.setText(_translate("MainWindow", "1"))
-        item = self.table_channels.verticalHeaderItem(1)
-        item.setText(_translate("MainWindow", "2"))
-        item = self.table_channels.verticalHeaderItem(2)
-        item.setText(_translate("MainWindow", "3"))
-        item = self.table_channels.verticalHeaderItem(3)
-        item.setText(_translate("MainWindow", "4"))
-        item = self.table_channels.verticalHeaderItem(4)
-        item.setText(_translate("MainWindow", "5"))
-        item = self.table_channels.verticalHeaderItem(5)
-        item.setText(_translate("MainWindow", "6"))
-        item = self.table_channels.verticalHeaderItem(6)
-        item.setText(_translate("MainWindow", "7"))
-        item = self.table_channels.verticalHeaderItem(7)
-        item.setText(_translate("MainWindow", "8"))
-        item = self.table_channels.verticalHeaderItem(8)
-        item.setText(_translate("MainWindow", "9"))
-        item = self.table_channels.verticalHeaderItem(9)
-        item.setText(_translate("MainWindow", "10"))
-        item = self.table_channels.verticalHeaderItem(10)
-        item.setText(_translate("MainWindow", "11"))
-        item = self.table_channels.verticalHeaderItem(11)
-        item.setText(_translate("MainWindow", "12"))
-        item = self.table_channels.verticalHeaderItem(12)
-        item.setText(_translate("MainWindow", "13"))
-        item = self.table_channels.verticalHeaderItem(13)
-        item.setText(_translate("MainWindow", "14"))
-        item = self.table_channels.verticalHeaderItem(14)
-        item.setText(_translate("MainWindow", "15"))
-        item = self.table_channels.verticalHeaderItem(15)
-        item.setText(_translate("MainWindow", "16"))
-        item = self.table_channels.horizontalHeaderItem(0)
-        item.setText(_translate("MainWindow", "1"))
-        item = self.table_channels.horizontalHeaderItem(1)
-        item.setText(_translate("MainWindow", "2"))
-        item = self.table_channels.horizontalHeaderItem(2)
-        item.setText(_translate("MainWindow", "3"))
-        item = self.table_channels.horizontalHeaderItem(3)
-        item.setText(_translate("MainWindow", "4"))
-        __sortingEnabled = self.table_channels.isSortingEnabled()
-        self.table_channels.setSortingEnabled(False)
-        item = self.table_channels.item(0, 0)
-        item.setText(_translate("MainWindow", "1"))
-        item = self.table_channels.item(0, 1)
-        item.setText(_translate("MainWindow", "17"))
-        item = self.table_channels.item(0, 2)
-        item.setText(_translate("MainWindow", "33"))
-        item = self.table_channels.item(0, 3)
-        item.setText(_translate("MainWindow", "49"))
-        item = self.table_channels.item(1, 0)
-        item.setText(_translate("MainWindow", "2"))
-        item = self.table_channels.item(1, 1)
-        item.setText(_translate("MainWindow", "18"))
-        item = self.table_channels.item(1, 2)
-        item.setText(_translate("MainWindow", "34"))
-        item = self.table_channels.item(1, 3)
-        item.setText(_translate("MainWindow", "50"))
-        item = self.table_channels.item(2, 0)
-        item.setText(_translate("MainWindow", "3"))
-        item = self.table_channels.item(2, 1)
-        item.setText(_translate("MainWindow", "19"))
-        item = self.table_channels.item(2, 2)
-        item.setText(_translate("MainWindow", "35"))
-        item = self.table_channels.item(2, 3)
-        item.setText(_translate("MainWindow", "51"))
-        item = self.table_channels.item(3, 0)
-        item.setText(_translate("MainWindow", "4"))
-        item = self.table_channels.item(3, 1)
-        item.setText(_translate("MainWindow", "20"))
-        item = self.table_channels.item(3, 2)
-        item.setText(_translate("MainWindow", "36"))
-        item = self.table_channels.item(3, 3)
-        item.setText(_translate("MainWindow", "52"))
-        item = self.table_channels.item(4, 0)
-        item.setText(_translate("MainWindow", "5"))
-        item = self.table_channels.item(4, 1)
-        item.setText(_translate("MainWindow", "21"))
-        item = self.table_channels.item(4, 2)
-        item.setText(_translate("MainWindow", "37"))
-        item = self.table_channels.item(4, 3)
-        item.setText(_translate("MainWindow", "53"))
-        item = self.table_channels.item(5, 0)
-        item.setText(_translate("MainWindow", "6"))
-        item = self.table_channels.item(5, 1)
-        item.setText(_translate("MainWindow", "22"))
-        item = self.table_channels.item(5, 2)
-        item.setText(_translate("MainWindow", "38"))
-        item = self.table_channels.item(5, 3)
-        item.setText(_translate("MainWindow", "54"))
-        item = self.table_channels.item(6, 0)
-        item.setText(_translate("MainWindow", "7"))
-        item = self.table_channels.item(6, 1)
-        item.setText(_translate("MainWindow", "23"))
-        item = self.table_channels.item(6, 2)
-        item.setText(_translate("MainWindow", "39"))
-        item = self.table_channels.item(6, 3)
-        item.setText(_translate("MainWindow", "55"))
-        item = self.table_channels.item(7, 0)
-        item.setText(_translate("MainWindow", "8"))
-        item = self.table_channels.item(7, 1)
-        item.setText(_translate("MainWindow", "24"))
-        item = self.table_channels.item(7, 2)
-        item.setText(_translate("MainWindow", "40"))
-        item = self.table_channels.item(7, 3)
-        item.setText(_translate("MainWindow", "56"))
-        item = self.table_channels.item(8, 0)
-        item.setText(_translate("MainWindow", "9"))
-        item = self.table_channels.item(8, 1)
-        item.setText(_translate("MainWindow", "25"))
-        item = self.table_channels.item(8, 2)
-        item.setText(_translate("MainWindow", "41"))
-        item = self.table_channels.item(8, 3)
-        item.setText(_translate("MainWindow", "57"))
-        item = self.table_channels.item(9, 0)
-        item.setText(_translate("MainWindow", "10"))
-        item = self.table_channels.item(9, 1)
-        item.setText(_translate("MainWindow", "26"))
-        item = self.table_channels.item(9, 2)
-        item.setText(_translate("MainWindow", "42"))
-        item = self.table_channels.item(9, 3)
-        item.setText(_translate("MainWindow", "58"))
-        item = self.table_channels.item(10, 0)
-        item.setText(_translate("MainWindow", "11"))
-        item = self.table_channels.item(10, 1)
-        item.setText(_translate("MainWindow", "27"))
-        item = self.table_channels.item(10, 2)
-        item.setText(_translate("MainWindow", "43"))
-        item = self.table_channels.item(10, 3)
-        item.setText(_translate("MainWindow", "59"))
-        item = self.table_channels.item(11, 0)
-        item.setText(_translate("MainWindow", "12"))
-        item = self.table_channels.item(11, 1)
-        item.setText(_translate("MainWindow", "28"))
-        item = self.table_channels.item(11, 2)
-        item.setText(_translate("MainWindow", "44"))
-        item = self.table_channels.item(11, 3)
-        item.setText(_translate("MainWindow", "60"))
-        item = self.table_channels.item(12, 0)
-        item.setText(_translate("MainWindow", "13"))
-        item = self.table_channels.item(12, 1)
-        item.setText(_translate("MainWindow", "29"))
-        item = self.table_channels.item(12, 2)
-        item.setText(_translate("MainWindow", "45"))
-        item = self.table_channels.item(12, 3)
-        item.setText(_translate("MainWindow", "61"))
-        item = self.table_channels.item(13, 0)
-        item.setText(_translate("MainWindow", "14"))
-        item = self.table_channels.item(13, 1)
-        item.setText(_translate("MainWindow", "30"))
-        item = self.table_channels.item(13, 2)
-        item.setText(_translate("MainWindow", "46"))
-        item = self.table_channels.item(13, 3)
-        item.setText(_translate("MainWindow", "62"))
-        item = self.table_channels.item(14, 0)
-        item.setText(_translate("MainWindow", "15"))
-        item = self.table_channels.item(14, 1)
-        item.setText(_translate("MainWindow", "31"))
-        item = self.table_channels.item(14, 2)
-        item.setText(_translate("MainWindow", "47"))
-        item = self.table_channels.item(14, 3)
-        item.setText(_translate("MainWindow", "63"))
-        item = self.table_channels.item(15, 0)
-        item.setText(_translate("MainWindow", "16"))
-        item = self.table_channels.item(15, 1)
-        item.setText(_translate("MainWindow", "32"))
-        item = self.table_channels.item(15, 2)
-        item.setText(_translate("MainWindow", "48"))
-        item = self.table_channels.item(15, 3)
-        item.setText(_translate("MainWindow", "64"))
-        self.table_channels.setSortingEnabled(__sortingEnabled)
-
-
+# -*- coding: utf-8 -*-
+
+# Form implementation generated from reading ui file 'mainwindow.ui'
+#
+# Created by: PyQt5 UI code generator 5.12.1
+#
+# WARNING! All changes made in this file will be lost!
+
+from PyQt5 import QtCore, QtGui, QtWidgets
+
+
+class Ui_MainWindow(object):
+    def setupUi(self, MainWindow):
+        MainWindow.setObjectName("MainWindow")
+        MainWindow.resize(533, 688)
+        self.centralWidget = QtWidgets.QWidget(MainWindow)
+        self.centralWidget.setObjectName("centralWidget")
+        self.comboBox_scale = QtWidgets.QComboBox(self.centralWidget)
+        self.comboBox_scale.setGeometry(QtCore.QRect(10, 20, 85, 27))
+        self.comboBox_scale.setObjectName("comboBox_scale")
+        self.comboBox_scale.addItem("")
+        self.comboBox_scale.addItem("")
+        self.comboBox_scale.addItem("")
+        self.comboBox_scale.addItem("")
+        self.comboBox_scale.addItem("")
+        self.comboBox_scale.addItem("")
+        self.comboBox_scale.addItem("")
+        self.comboBox_scale.addItem("")
+        self.comboBox_scale.addItem("")
+        self.comboBox_scale.addItem("")
+        self.checkBox_car = QtWidgets.QCheckBox(self.centralWidget)
+        self.checkBox_car.setGeometry(QtCore.QRect(120, 0, 97, 22))
+        self.checkBox_car.setObjectName("checkBox_car")
+        self.label_2 = QtWidgets.QLabel(self.centralWidget)
+        self.label_2.setGeometry(QtCore.QRect(10, 60, 67, 17))
+        self.label_2.setObjectName("label_2")
+        self.label_3 = QtWidgets.QLabel(self.centralWidget)
+        self.label_3.setGeometry(QtCore.QRect(10, 0, 67, 17))
+        self.label_3.setObjectName("label_3")
+        self.checkBox_bandpass = QtWidgets.QCheckBox(self.centralWidget)
+        self.checkBox_bandpass.setGeometry(QtCore.QRect(120, 20, 141, 22))
+        self.checkBox_bandpass.setObjectName("checkBox_bandpass")
+        self.pushButton_bp = QtWidgets.QPushButton(self.centralWidget)
+        self.pushButton_bp.setGeometry(QtCore.QRect(410, 20, 99, 27))
+        self.pushButton_bp.setObjectName("pushButton_bp")
+        self.spinBox_time = QtWidgets.QSpinBox(self.centralWidget)
+        self.spinBox_time.setGeometry(QtCore.QRect(10, 80, 85, 27))
+        self.spinBox_time.setMinimum(1)
+        self.spinBox_time.setProperty("value", 5)
+        self.spinBox_time.setObjectName("spinBox_time")
+        self.doubleSpinBox_hp = QtWidgets.QDoubleSpinBox(self.centralWidget)
+        self.doubleSpinBox_hp.setGeometry(QtCore.QRect(260, 20, 69, 27))
+        self.doubleSpinBox_hp.setMinimum(0.1)
+        self.doubleSpinBox_hp.setSingleStep(0.1)
+        self.doubleSpinBox_hp.setProperty("value", 1.0)
+        self.doubleSpinBox_hp.setObjectName("doubleSpinBox_hp")
+        self.doubleSpinBox_lp = QtWidgets.QDoubleSpinBox(self.centralWidget)
+        self.doubleSpinBox_lp.setGeometry(QtCore.QRect(340, 20, 69, 27))
+        self.doubleSpinBox_lp.setMinimum(1.0)
+        self.doubleSpinBox_lp.setSingleStep(0.1)
+        self.doubleSpinBox_lp.setProperty("value", 50.0)
+        self.doubleSpinBox_lp.setObjectName("doubleSpinBox_lp")
+        self.checkBox_showTID = QtWidgets.QCheckBox(self.centralWidget)
+        self.checkBox_showTID.setGeometry(QtCore.QRect(120, 60, 161, 22))
+        self.checkBox_showTID.setObjectName("checkBox_showTID")
+        self.checkBox_showLPT = QtWidgets.QCheckBox(self.centralWidget)
+        self.checkBox_showLPT.setGeometry(QtCore.QRect(120, 80, 151, 22))
+        self.checkBox_showLPT.setObjectName("checkBox_showLPT")
+        self.checkBox_showKey = QtWidgets.QCheckBox(self.centralWidget)
+        self.checkBox_showKey.setGeometry(QtCore.QRect(120, 100, 151, 22))
+        self.checkBox_showKey.setObjectName("checkBox_showKey")
+        self.line = QtWidgets.QFrame(self.centralWidget)
+        self.line.setGeometry(QtCore.QRect(100, 0, 21, 121))
+        self.line.setFrameShape(QtWidgets.QFrame.VLine)
+        self.line.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.line.setObjectName("line")
+        self.line_2 = QtWidgets.QFrame(self.centralWidget)
+        self.line_2.setGeometry(QtCore.QRect(110, 45, 431, 21))
+        self.line_2.setFrameShape(QtWidgets.QFrame.HLine)
+        self.line_2.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.line_2.setObjectName("line_2")
+        self.line_3 = QtWidgets.QFrame(self.centralWidget)
+        self.line_3.setGeometry(QtCore.QRect(290, 60, 21, 61))
+        self.line_3.setFrameShape(QtWidgets.QFrame.VLine)
+        self.line_3.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.line_3.setObjectName("line_3")
+        self.pushButton_stoprec = QtWidgets.QPushButton(self.centralWidget)
+        self.pushButton_stoprec.setGeometry(QtCore.QRect(310, 90, 201, 27))
+        self.pushButton_stoprec.setObjectName("pushButton_stoprec")
+        self.pushButton_rec = QtWidgets.QPushButton(self.centralWidget)
+        self.pushButton_rec.setGeometry(QtCore.QRect(460, 60, 51, 27))
+        self.pushButton_rec.setObjectName("pushButton_rec")
+        self.lineEdit_recFilename = QtWidgets.QLineEdit(self.centralWidget)
+        self.lineEdit_recFilename.setGeometry(QtCore.QRect(310, 60, 141, 27))
+        self.lineEdit_recFilename.setObjectName("lineEdit_recFilename")
+        self.table_channels = QtWidgets.QTableWidget(self.centralWidget)
+        self.table_channels.setGeometry(QtCore.QRect(60, 140, 411, 491))
+        self.table_channels.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
+        self.table_channels.setTextElideMode(QtCore.Qt.ElideMiddle)
+        self.table_channels.setShowGrid(False)
+        self.table_channels.setObjectName("table_channels")
+        self.table_channels.setColumnCount(4)
+        self.table_channels.setRowCount(16)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setVerticalHeaderItem(0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setVerticalHeaderItem(1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setVerticalHeaderItem(2, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setVerticalHeaderItem(3, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setVerticalHeaderItem(4, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setVerticalHeaderItem(5, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setVerticalHeaderItem(6, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setVerticalHeaderItem(7, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setVerticalHeaderItem(8, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setVerticalHeaderItem(9, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setVerticalHeaderItem(10, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setVerticalHeaderItem(11, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setVerticalHeaderItem(12, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setVerticalHeaderItem(13, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setVerticalHeaderItem(14, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setVerticalHeaderItem(15, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setHorizontalHeaderItem(0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setHorizontalHeaderItem(1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setHorizontalHeaderItem(2, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setHorizontalHeaderItem(3, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(0, 0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(0, 1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(0, 2, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(0, 3, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(1, 0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(1, 1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(1, 2, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(1, 3, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(2, 0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(2, 1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(2, 2, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(2, 3, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(3, 0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(3, 1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(3, 2, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(3, 3, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(4, 0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(4, 1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(4, 2, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(4, 3, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(5, 0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(5, 1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(5, 2, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(5, 3, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(6, 0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(6, 1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(6, 2, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(6, 3, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(7, 0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(7, 1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(7, 2, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(7, 3, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(8, 0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(8, 1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(8, 2, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(8, 3, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(9, 0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(9, 1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(9, 2, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(9, 3, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(10, 0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(10, 1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(10, 2, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(10, 3, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(11, 0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(11, 1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(11, 2, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(11, 3, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(12, 0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(12, 1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(12, 2, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(12, 3, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(13, 0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(13, 1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(13, 2, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(13, 3, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(14, 0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(14, 1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(14, 2, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(14, 3, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(15, 0, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(15, 1, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(15, 2, item)
+        item = QtWidgets.QTableWidgetItem()
+        self.table_channels.setItem(15, 3, item)
+        self.table_channels.horizontalHeader().setVisible(False)
+        self.table_channels.horizontalHeader().setHighlightSections(False)
+        self.table_channels.verticalHeader().setVisible(False)
+        self.table_channels.verticalHeader().setHighlightSections(False)
+        self.line_4 = QtWidgets.QFrame(self.centralWidget)
+        self.line_4.setGeometry(QtCore.QRect(0, 120, 531, 21))
+        self.line_4.setFrameShape(QtWidgets.QFrame.HLine)
+        self.line_4.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.line_4.setObjectName("line_4")
+        MainWindow.setCentralWidget(self.centralWidget)
+        self.menuBar = QtWidgets.QMenuBar(MainWindow)
+        self.menuBar.setGeometry(QtCore.QRect(0, 0, 533, 25))
+        self.menuBar.setObjectName("menuBar")
+        MainWindow.setMenuBar(self.menuBar)
+        self.mainToolBar = QtWidgets.QToolBar(MainWindow)
+        self.mainToolBar.setObjectName("mainToolBar")
+        MainWindow.addToolBar(QtCore.Qt.TopToolBarArea, self.mainToolBar)
+        self.statusBar = QtWidgets.QStatusBar(MainWindow)
+        self.statusBar.setObjectName("statusBar")
+        MainWindow.setStatusBar(self.statusBar)
+
+        self.retranslateUi(MainWindow)
+        QtCore.QMetaObject.connectSlotsByName(MainWindow)
+
+    def retranslateUi(self, MainWindow):
+        _translate = QtCore.QCoreApplication.translate
+        MainWindow.setWindowTitle(_translate("MainWindow", "MainWindow"))
+        self.comboBox_scale.setItemText(0, _translate("MainWindow", "1uV"))
+        self.comboBox_scale.setItemText(1, _translate("MainWindow", "10uV"))
+        self.comboBox_scale.setItemText(2, _translate("MainWindow", "25uV"))
+        self.comboBox_scale.setItemText(3, _translate("MainWindow", "50uV"))
+        self.comboBox_scale.setItemText(4, _translate("MainWindow", "100uV"))
+        self.comboBox_scale.setItemText(5, _translate("MainWindow", "250uV"))
+        self.comboBox_scale.setItemText(6, _translate("MainWindow", "500uV"))
+        self.comboBox_scale.setItemText(7, _translate("MainWindow", "1mV"))
+        self.comboBox_scale.setItemText(8, _translate("MainWindow", "2.5mV"))
+        self.comboBox_scale.setItemText(9, _translate("MainWindow", "100mV"))
+        self.checkBox_car.setText(_translate("MainWindow", "CAR Filter"))
+        self.label_2.setText(_translate("MainWindow", "Time (s)"))
+        self.label_3.setText(_translate("MainWindow", "Scale"))
+        self.checkBox_bandpass.setText(_translate("MainWindow", "Bandpass Filter"))
+        self.pushButton_bp.setText(_translate("MainWindow", "Apply BP"))
+        self.checkBox_showTID.setText(_translate("MainWindow", "Show TID events"))
+        self.checkBox_showLPT.setText(_translate("MainWindow", "Show LPT events"))
+        self.checkBox_showKey.setText(_translate("MainWindow", "Show Key events"))
+        self.pushButton_stoprec.setText(_translate("MainWindow", "Stop REC"))
+        self.pushButton_rec.setText(_translate("MainWindow", "REC"))
+        item = self.table_channels.verticalHeaderItem(0)
+        item.setText(_translate("MainWindow", "1"))
+        item = self.table_channels.verticalHeaderItem(1)
+        item.setText(_translate("MainWindow", "2"))
+        item = self.table_channels.verticalHeaderItem(2)
+        item.setText(_translate("MainWindow", "3"))
+        item = self.table_channels.verticalHeaderItem(3)
+        item.setText(_translate("MainWindow", "4"))
+        item = self.table_channels.verticalHeaderItem(4)
+        item.setText(_translate("MainWindow", "5"))
+        item = self.table_channels.verticalHeaderItem(5)
+        item.setText(_translate("MainWindow", "6"))
+        item = self.table_channels.verticalHeaderItem(6)
+        item.setText(_translate("MainWindow", "7"))
+        item = self.table_channels.verticalHeaderItem(7)
+        item.setText(_translate("MainWindow", "8"))
+        item = self.table_channels.verticalHeaderItem(8)
+        item.setText(_translate("MainWindow", "9"))
+        item = self.table_channels.verticalHeaderItem(9)
+        item.setText(_translate("MainWindow", "10"))
+        item = self.table_channels.verticalHeaderItem(10)
+        item.setText(_translate("MainWindow", "11"))
+        item = self.table_channels.verticalHeaderItem(11)
+        item.setText(_translate("MainWindow", "12"))
+        item = self.table_channels.verticalHeaderItem(12)
+        item.setText(_translate("MainWindow", "13"))
+        item = self.table_channels.verticalHeaderItem(13)
+        item.setText(_translate("MainWindow", "14"))
+        item = self.table_channels.verticalHeaderItem(14)
+        item.setText(_translate("MainWindow", "15"))
+        item = self.table_channels.verticalHeaderItem(15)
+        item.setText(_translate("MainWindow", "16"))
+        item = self.table_channels.horizontalHeaderItem(0)
+        item.setText(_translate("MainWindow", "1"))
+        item = self.table_channels.horizontalHeaderItem(1)
+        item.setText(_translate("MainWindow", "2"))
+        item = self.table_channels.horizontalHeaderItem(2)
+        item.setText(_translate("MainWindow", "3"))
+        item = self.table_channels.horizontalHeaderItem(3)
+        item.setText(_translate("MainWindow", "4"))
+        __sortingEnabled = self.table_channels.isSortingEnabled()
+        self.table_channels.setSortingEnabled(False)
+        item = self.table_channels.item(0, 0)
+        item.setText(_translate("MainWindow", "1"))
+        item = self.table_channels.item(0, 1)
+        item.setText(_translate("MainWindow", "17"))
+        item = self.table_channels.item(0, 2)
+        item.setText(_translate("MainWindow", "33"))
+        item = self.table_channels.item(0, 3)
+        item.setText(_translate("MainWindow", "49"))
+        item = self.table_channels.item(1, 0)
+        item.setText(_translate("MainWindow", "2"))
+        item = self.table_channels.item(1, 1)
+        item.setText(_translate("MainWindow", "18"))
+        item = self.table_channels.item(1, 2)
+        item.setText(_translate("MainWindow", "34"))
+        item = self.table_channels.item(1, 3)
+        item.setText(_translate("MainWindow", "50"))
+        item = self.table_channels.item(2, 0)
+        item.setText(_translate("MainWindow", "3"))
+        item = self.table_channels.item(2, 1)
+        item.setText(_translate("MainWindow", "19"))
+        item = self.table_channels.item(2, 2)
+        item.setText(_translate("MainWindow", "35"))
+        item = self.table_channels.item(2, 3)
+        item.setText(_translate("MainWindow", "51"))
+        item = self.table_channels.item(3, 0)
+        item.setText(_translate("MainWindow", "4"))
+        item = self.table_channels.item(3, 1)
+        item.setText(_translate("MainWindow", "20"))
+        item = self.table_channels.item(3, 2)
+        item.setText(_translate("MainWindow", "36"))
+        item = self.table_channels.item(3, 3)
+        item.setText(_translate("MainWindow", "52"))
+        item = self.table_channels.item(4, 0)
+        item.setText(_translate("MainWindow", "5"))
+        item = self.table_channels.item(4, 1)
+        item.setText(_translate("MainWindow", "21"))
+        item = self.table_channels.item(4, 2)
+        item.setText(_translate("MainWindow", "37"))
+        item = self.table_channels.item(4, 3)
+        item.setText(_translate("MainWindow", "53"))
+        item = self.table_channels.item(5, 0)
+        item.setText(_translate("MainWindow", "6"))
+        item = self.table_channels.item(5, 1)
+        item.setText(_translate("MainWindow", "22"))
+        item = self.table_channels.item(5, 2)
+        item.setText(_translate("MainWindow", "38"))
+        item = self.table_channels.item(5, 3)
+        item.setText(_translate("MainWindow", "54"))
+        item = self.table_channels.item(6, 0)
+        item.setText(_translate("MainWindow", "7"))
+        item = self.table_channels.item(6, 1)
+        item.setText(_translate("MainWindow", "23"))
+        item = self.table_channels.item(6, 2)
+        item.setText(_translate("MainWindow", "39"))
+        item = self.table_channels.item(6, 3)
+        item.setText(_translate("MainWindow", "55"))
+        item = self.table_channels.item(7, 0)
+        item.setText(_translate("MainWindow", "8"))
+        item = self.table_channels.item(7, 1)
+        item.setText(_translate("MainWindow", "24"))
+        item = self.table_channels.item(7, 2)
+        item.setText(_translate("MainWindow", "40"))
+        item = self.table_channels.item(7, 3)
+        item.setText(_translate("MainWindow", "56"))
+        item = self.table_channels.item(8, 0)
+        item.setText(_translate("MainWindow", "9"))
+        item = self.table_channels.item(8, 1)
+        item.setText(_translate("MainWindow", "25"))
+        item = self.table_channels.item(8, 2)
+        item.setText(_translate("MainWindow", "41"))
+        item = self.table_channels.item(8, 3)
+        item.setText(_translate("MainWindow", "57"))
+        item = self.table_channels.item(9, 0)
+        item.setText(_translate("MainWindow", "10"))
+        item = self.table_channels.item(9, 1)
+        item.setText(_translate("MainWindow", "26"))
+        item = self.table_channels.item(9, 2)
+        item.setText(_translate("MainWindow", "42"))
+        item = self.table_channels.item(9, 3)
+        item.setText(_translate("MainWindow", "58"))
+        item = self.table_channels.item(10, 0)
+        item.setText(_translate("MainWindow", "11"))
+        item = self.table_channels.item(10, 1)
+        item.setText(_translate("MainWindow", "27"))
+        item = self.table_channels.item(10, 2)
+        item.setText(_translate("MainWindow", "43"))
+        item = self.table_channels.item(10, 3)
+        item.setText(_translate("MainWindow", "59"))
+        item = self.table_channels.item(11, 0)
+        item.setText(_translate("MainWindow", "12"))
+        item = self.table_channels.item(11, 1)
+        item.setText(_translate("MainWindow", "28"))
+        item = self.table_channels.item(11, 2)
+        item.setText(_translate("MainWindow", "44"))
+        item = self.table_channels.item(11, 3)
+        item.setText(_translate("MainWindow", "60"))
+        item = self.table_channels.item(12, 0)
+        item.setText(_translate("MainWindow", "13"))
+        item = self.table_channels.item(12, 1)
+        item.setText(_translate("MainWindow", "29"))
+        item = self.table_channels.item(12, 2)
+        item.setText(_translate("MainWindow", "45"))
+        item = self.table_channels.item(12, 3)
+        item.setText(_translate("MainWindow", "61"))
+        item = self.table_channels.item(13, 0)
+        item.setText(_translate("MainWindow", "14"))
+        item = self.table_channels.item(13, 1)
+        item.setText(_translate("MainWindow", "30"))
+        item = self.table_channels.item(13, 2)
+        item.setText(_translate("MainWindow", "46"))
+        item = self.table_channels.item(13, 3)
+        item.setText(_translate("MainWindow", "62"))
+        item = self.table_channels.item(14, 0)
+        item.setText(_translate("MainWindow", "15"))
+        item = self.table_channels.item(14, 1)
+        item.setText(_translate("MainWindow", "31"))
+        item = self.table_channels.item(14, 2)
+        item.setText(_translate("MainWindow", "47"))
+        item = self.table_channels.item(14, 3)
+        item.setText(_translate("MainWindow", "63"))
+        item = self.table_channels.item(15, 0)
+        item.setText(_translate("MainWindow", "16"))
+        item = self.table_channels.item(15, 1)
+        item.setText(_translate("MainWindow", "32"))
+        item = self.table_channels.item(15, 2)
+        item.setText(_translate("MainWindow", "48"))
+        item = self.table_channels.item(15, 3)
+        item.setText(_translate("MainWindow", "64"))
+        self.table_channels.setSortingEnabled(__sortingEnabled)
+
+
```

### Comparing `neurodecode-2.0.4/neurodecode/triggers/pyLptControl.py` & `neurodecode-2.0.5/neurodecode/triggers/pyLptControl.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,281 +1,281 @@
-from __future__ import print_function, division
-
-"""
-Send trigger events to parallel port.
-
-See sample code at the end.
-
-Kyuhwa Lee, 2014
-Swiss Federal Institute of Technology Lausanne (EPFL)
-
-"""
-
-import os
-import sys
-import time
-import pylsl
-import ctypes
-import threading
-import multiprocessing as mp
-import neurodecode.utils.q_common as qc
-import neurodecode.utils.nd_lsl as nd_lsl
-import neurodecode.utils.pycnbi_utils as pu
-from neurodecode import logger
-from builtins import input, bytes
-
-class Trigger(object):
-    """
-    Supported device types:
-     'Arduino': CNBI Arduino trigger
-     'USB2LPT': Commercial USB2LPT adapter
-     'DESKTOP': Desktop native LPT
-     'SOFTWARE': Software trigger (StreamRecorderInfo LSL server required)
-     'MOCK': Mock trigger device for testing
-
-    When using USB2LPT, the port number (e.g. 0x378) can be searched automatically.
-    When using Desktop's LPT, the port number must be specified during initialization.
-
-    Software trigger writes event information into a text file with LSL timestamps in the
-    same folder where StreamRecorder writes data, to be added later to the fif file.
-    This file will be automatically saved and closed when Ctrl+C is pressed or
-    terminal window is closed (or killed for whatever reason).
-
-    The asynchronous function signal(x) sends 1-byte integer value x and returns immediately.
-    It schedules to send the value 0 at the end of the signal length.
-
-    To use with USB2LPT, download the driver from:
-    https://www-user.tu-chemnitz.de/~heha/bastelecke/Rund%20um%20den%20PC/USB2LPT/index.en.htm
-
-    I've made a C++ library to send commands to LPTx using standard Windows API.
-    Use LptControl64.dll for 64 bit Python and LptControl32.dll for 32 bit Python.
-
-    state = multiprocessing.value 1: acquire, 0:stop
-
-    Some important functions:
-    int init(duration)
-        Returns False if error, True if success.
-        Duration unit: msec
-
-    void signal(value)
-        Sends the value to the parallel port and sets to 0 after a set period.
-        The value shuold be an integer in the range of 0-255.
-    """
-    def __init__(self, lpttype='USB2LPT', portaddr=None, verbose=True, check_lsl_offset=True, state=mp.Value('i', 1)):
-        self.evefile = None
-        self.lpttype = lpttype
-        self.verbose = verbose
-
-        if self.lpttype in ['USB2LPT', 'DESKTOP']:
-            if self.lpttype == 'USB2LPT':
-                if ctypes.sizeof(ctypes.c_voidp) == 4:
-                    dllname = 'LptControl_USB2LPT32.dll'  # 32 bit
-                else:
-                    dllname = 'LptControl_USB2LPT64.dll'  # 64 bit
-                if portaddr not in [0x278, 0x378]:
-                    logger.warning('LPT port address %d is unusual.' % portaddr)
-
-            elif self.lpttype == 'DESKTOP':
-                if ctypes.sizeof(ctypes.c_voidp) == 4:
-                    dllname = 'LptControl_Desktop32.dll'  # 32 bit
-                else:
-                    dllname = 'LptControl_Desktop64.dll'  # 64 bit
-                if portaddr not in [0x278, 0x378]:
-                    logger.warning('LPT port address %d is unusual.' % portaddr)
-
-            self.portaddr = portaddr
-            search = []
-            search.append(os.path.dirname(__file__) + '/' + dllname)
-            search.append(os.path.dirname(__file__) + '/libs/' + dllname)
-            search.append(os.getcwd() + '/' + dllname)
-            search.append(os.getcwd() + '/libs/' + dllname)
-            for f in search:
-                if os.path.exists(f):
-                    dllpath = f
-                    break
-            else:
-                logger.error('Cannot find the required library %s' % dllname)
-                raise RuntimeError
-
-            logger.info('Loading %s' % dllpath)
-            self.lpt = ctypes.cdll.LoadLibrary(dllpath)
-
-        elif self.lpttype == 'ARDUINO':
-            import serial, serial.tools.list_ports
-            BAUD_RATE = 115200
-
-            # portaddr should be None or in the form of 'COM1', 'COM2', etc.
-            if portaddr is None:
-                arduinos = [x for x in serial.tools.list_ports.grep('Arduino')]
-                if len(arduinos) == 0:
-                    logger.error('No Arduino found. Stop.')
-                    sys.exit()
-
-                for i, a in enumerate(arduinos):
-                    logger.info('Found %s' % a[0])
-                try:
-                    com_port = arduinos[0].device
-                except AttributeError: # depends on Python distribution
-                    com_port = arduinos[0][0]
-            else:
-                com_port = portaddr
-
-            self.ser = serial.Serial(com_port, BAUD_RATE)
-            time.sleep(1)  # doesn't work without this delay. why?
-            logger.info('Connected to %s.' % com_port)
-
-        elif self.lpttype == 'SOFTWARE':
-            from neurodecode.stream_receiver.stream_receiver import StreamReceiver
-            logger.info('Using software trigger')
-
-            # get data file location
-            LSL_SERVER = 'StreamRecorderInfo'
-            inlet = nd_lsl.start_client(LSL_SERVER)
-            evefile = inlet.info().source_id()
-            eveoffset_file = evefile[:-4] + '-offset.txt'
-            logger.info('Event file is: %s' % evefile)
-            self.evefile = open(evefile, 'a')
-
-            if check_lsl_offset:
-                # check server LSL time server integrity
-                qc.print_c('>> Please choose amplifier server to check the timestamp offset:', 'G')
-                amp_name, amp_serial = pu.search_lsl()
-                sr = StreamReceiver(window_size=1, buffer_size=1, amp_serial=amp_serial, eeg_only=False, amp_name=amp_name)
-                local_time = pylsl.local_clock()
-                server_time = sr.get_window_list()[1][-1]
-                lsl_time_offset = server_time - local_time
-                with open(eveoffset_file, 'a') as f:
-                    f.write('Offset: %.6f\n' % lsl_time_offset)
-                    f.write('Server time: %.6f\n' % server_time)
-                    f.write('Local time: %.6f\n' % local_time)
-                logger.info('LSL timestamp offset (%.3f) saved to %s' % (lsl_time_offset, eveoffset_file))
-
-        elif self.lpttype == 'MOCK' or self.lpttype is None or self.lpttype is False:
-            logger.warning('Using a fake trigger.')
-            self.lpttype = 'MOCK'
-            self.lpt = None
-
-        else:
-            logger.error('Unrecognized lpttype device name %s' % lpttype)
-            sys.exit(-1)
-
-    def __del__(self):
-        if self.evefile is not None and not self.evefile.closed:
-            self.evefile.close()
-
-    def init(self, duration):
-        if self.lpttype == 'SOFTWARE':
-            logger.info('Ignoring delay parameter for software trigger.')
-            return True
-        elif self.lpttype == 'MOCK':
-            return True
-        else:
-            self.delay = duration / 1000.0
-
-            if self.lpttype in ['DESKTOP', 'USB2LPT']:
-                if self.lpt.init() == -1:
-                    logger.error('Connecting to LPT port failed. Check the driver status.')
-                    self.lpt = None
-                    return False
-
-            self.action = False
-            self.offtimer = threading.Timer(self.delay, self.signal_off)
-            return True
-
-    # write to software trigger
-    def write_event(self, value):
-        assert self.lpttype == 'SOFTWARE'
-        self.evefile.write('%.6f\t0\t%d\n' % (pylsl.local_clock(), value))
-        return True
-
-    # set data
-    def set_data(self, value):
-        if self.lpttype == 'SOFTWARE':
-            logger.error('set_data() not supported for software trigger.')
-            return False
-        elif self.lpttype == 'MOCK':
-            logger.info('MOCK trigger value %s' % value)
-            return True
-        else:
-            if self.lpttype == 'USB2LPT':
-                self.lpt.setdata(value)
-            elif self.lpttype == 'DESKTOP':
-                self.lpt.setdata(self.portaddr, value)
-            elif self.lpttype == 'ARDUINO':
-                self.ser.write(bytes([value]))
-            else:
-                raise RuntimeError('Wrong trigger device')
-
-    # sends data and turn off after delay
-    def signal(self, value):
-        if self.lpttype == 'SOFTWARE':
-            if self.verbose is True:
-                logger.info('Sending software trigger %s' % value)
-            return self.write_event(value)
-        elif self.lpttype == 'MOCK':
-            logger.info('Sending MOCK trigger signal %s' % value)
-            return True
-        else:
-            if self.offtimer.is_alive():
-                logger.warning('You are sending a new signal before the end of the last signal. Signal ignored.')
-                logger.warning('self.delay=%.1f' % self.delay)
-                return False
-            self.set_data(value)
-            if self.verbose is True:
-                logger.info('Sending %s' % value)
-            self.offtimer.start()
-            return True
-
-    # set data to zero (all bits off)
-    def signal_off(self):
-        if self.lpttype == 'SOFTWARE':
-            return self.write_event(0)
-        elif self.lpttype == 'MOCK':
-            logger.info('MOCK trigger off')
-            return True
-        else:
-            self.set_data(0)
-            self.offtimer = threading.Timer(self.delay, self.signal_off)
-
-    # set pin
-    def set_pin(self, pin):
-        if self.lpttype == 'SOFTWARE':
-            logger.error('set_pin() not supported for software trigger.')
-            return False
-        elif self.lpttype == 'MOCK':
-            logger.info('MOCK trigger pin %s' % pin)
-            return True
-        else:
-            self.set_data(2 ** (pin - 1))
-
-
-# set 1 to each bit and rotate from bit 0 to bit 7
-def test_all_bits(trigger):
-    for x in range(8):
-        val = 2 ** x
-        trigger.signal(val)
-        logger.info(val)
-        time.sleep(1)
-
-# sample test code
-if __name__ == '__main__':
-    trigger = Trigger('ARDUINO') # Arduino trigger
-    #trigger = Trigger('SOFTWARE')
-    if not trigger.init(500):
-        print('LPT port cannot be opened. Using a mock trigger.')
-        trigger = Trigger('MOCK')
-
-    # Christmas tree mode (set 1 bit-by-bit)
-    #test_all_bits(trigger)
-
-    print('Type quit or Ctrl+C to finish.')
-    while True:
-        val = input('Trigger value? ')
-        if val.strip() == '':
-            continue
-        if val == 'quit':
-            break
-        if 0 <= int(val) <= 255:
-            trigger.signal(int(val))
-            print('Sent %d' % int(val))
-        else:
-            print('Ignored %s' % val)
+from __future__ import print_function, division
+
+"""
+Send trigger events to parallel port.
+
+See sample code at the end.
+
+Kyuhwa Lee, 2014
+Swiss Federal Institute of Technology Lausanne (EPFL)
+
+"""
+
+import os
+import sys
+import time
+import pylsl
+import ctypes
+import threading
+import multiprocessing as mp
+import neurodecode.utils.q_common as qc
+import neurodecode.utils.nd_lsl as nd_lsl
+import neurodecode.utils.pycnbi_utils as pu
+from neurodecode import logger
+from builtins import input, bytes
+
+class Trigger(object):
+    """
+    Supported device types:
+     'Arduino': CNBI Arduino trigger
+     'USB2LPT': Commercial USB2LPT adapter
+     'DESKTOP': Desktop native LPT
+     'SOFTWARE': Software trigger (StreamRecorderInfo LSL server required)
+     'MOCK': Mock trigger device for testing
+
+    When using USB2LPT, the port number (e.g. 0x378) can be searched automatically.
+    When using Desktop's LPT, the port number must be specified during initialization.
+
+    Software trigger writes event information into a text file with LSL timestamps in the
+    same folder where StreamRecorder writes data, to be added later to the fif file.
+    This file will be automatically saved and closed when Ctrl+C is pressed or
+    terminal window is closed (or killed for whatever reason).
+
+    The asynchronous function signal(x) sends 1-byte integer value x and returns immediately.
+    It schedules to send the value 0 at the end of the signal length.
+
+    To use with USB2LPT, download the driver from:
+    https://www-user.tu-chemnitz.de/~heha/bastelecke/Rund%20um%20den%20PC/USB2LPT/index.en.htm
+
+    I've made a C++ library to send commands to LPTx using standard Windows API.
+    Use LptControl64.dll for 64 bit Python and LptControl32.dll for 32 bit Python.
+
+    state = multiprocessing.value 1: acquire, 0:stop
+
+    Some important functions:
+    int init(duration)
+        Returns False if error, True if success.
+        Duration unit: msec
+
+    void signal(value)
+        Sends the value to the parallel port and sets to 0 after a set period.
+        The value shuold be an integer in the range of 0-255.
+    """
+    def __init__(self, lpttype='USB2LPT', portaddr=None, verbose=True, check_lsl_offset=True, state=mp.Value('i', 1)):
+        self.evefile = None
+        self.lpttype = lpttype
+        self.verbose = verbose
+
+        if self.lpttype in ['USB2LPT', 'DESKTOP']:
+            if self.lpttype == 'USB2LPT':
+                if ctypes.sizeof(ctypes.c_voidp) == 4:
+                    dllname = 'LptControl_USB2LPT32.dll'  # 32 bit
+                else:
+                    dllname = 'LptControl_USB2LPT64.dll'  # 64 bit
+                if portaddr not in [0x278, 0x378]:
+                    logger.warning('LPT port address %d is unusual.' % portaddr)
+
+            elif self.lpttype == 'DESKTOP':
+                if ctypes.sizeof(ctypes.c_voidp) == 4:
+                    dllname = 'LptControl_Desktop32.dll'  # 32 bit
+                else:
+                    dllname = 'LptControl_Desktop64.dll'  # 64 bit
+                if portaddr not in [0x278, 0x378]:
+                    logger.warning('LPT port address %d is unusual.' % portaddr)
+
+            self.portaddr = portaddr
+            search = []
+            search.append(os.path.dirname(__file__) + '/' + dllname)
+            search.append(os.path.dirname(__file__) + '/libs/' + dllname)
+            search.append(os.getcwd() + '/' + dllname)
+            search.append(os.getcwd() + '/libs/' + dllname)
+            for f in search:
+                if os.path.exists(f):
+                    dllpath = f
+                    break
+            else:
+                logger.error('Cannot find the required library %s' % dllname)
+                raise RuntimeError
+
+            logger.info('Loading %s' % dllpath)
+            self.lpt = ctypes.cdll.LoadLibrary(dllpath)
+
+        elif self.lpttype == 'ARDUINO':
+            import serial, serial.tools.list_ports
+            BAUD_RATE = 115200
+
+            # portaddr should be None or in the form of 'COM1', 'COM2', etc.
+            if portaddr is None:
+                arduinos = [x for x in serial.tools.list_ports.grep('Arduino')]
+                if len(arduinos) == 0:
+                    logger.error('No Arduino found. Stop.')
+                    sys.exit()
+
+                for i, a in enumerate(arduinos):
+                    logger.info('Found %s' % a[0])
+                try:
+                    com_port = arduinos[0].device
+                except AttributeError: # depends on Python distribution
+                    com_port = arduinos[0][0]
+            else:
+                com_port = portaddr
+
+            self.ser = serial.Serial(com_port, BAUD_RATE)
+            time.sleep(1)  # doesn't work without this delay. why?
+            logger.info('Connected to %s.' % com_port)
+
+        elif self.lpttype == 'SOFTWARE':
+            from neurodecode.stream_receiver.stream_receiver import StreamReceiver
+            logger.info('Using software trigger')
+
+            # get data file location
+            LSL_SERVER = 'StreamRecorderInfo'
+            inlet = nd_lsl.start_client(LSL_SERVER)
+            evefile = inlet.info().source_id()
+            eveoffset_file = evefile[:-4] + '-offset.txt'
+            logger.info('Event file is: %s' % evefile)
+            self.evefile = open(evefile, 'a')
+
+            if check_lsl_offset:
+                # check server LSL time server integrity
+                qc.print_c('>> Please choose amplifier server to check the timestamp offset:', 'G')
+                amp_name, amp_serial = pu.search_lsl()
+                sr = StreamReceiver(window_size=1, buffer_size=1, amp_serial=amp_serial, eeg_only=False, amp_name=amp_name)
+                local_time = pylsl.local_clock()
+                server_time = sr.get_window_list()[1][-1]
+                lsl_time_offset = server_time - local_time
+                with open(eveoffset_file, 'a') as f:
+                    f.write('Offset: %.6f\n' % lsl_time_offset)
+                    f.write('Server time: %.6f\n' % server_time)
+                    f.write('Local time: %.6f\n' % local_time)
+                logger.info('LSL timestamp offset (%.3f) saved to %s' % (lsl_time_offset, eveoffset_file))
+
+        elif self.lpttype == 'MOCK' or self.lpttype is None or self.lpttype is False:
+            logger.warning('Using a fake trigger.')
+            self.lpttype = 'MOCK'
+            self.lpt = None
+
+        else:
+            logger.error('Unrecognized lpttype device name %s' % lpttype)
+            sys.exit(-1)
+
+    def __del__(self):
+        if self.evefile is not None and not self.evefile.closed:
+            self.evefile.close()
+
+    def init(self, duration):
+        if self.lpttype == 'SOFTWARE':
+            logger.info('Ignoring delay parameter for software trigger.')
+            return True
+        elif self.lpttype == 'MOCK':
+            return True
+        else:
+            self.delay = duration / 1000.0
+
+            if self.lpttype in ['DESKTOP', 'USB2LPT']:
+                if self.lpt.init() == -1:
+                    logger.error('Connecting to LPT port failed. Check the driver status.')
+                    self.lpt = None
+                    return False
+
+            self.action = False
+            self.offtimer = threading.Timer(self.delay, self.signal_off)
+            return True
+
+    # write to software trigger
+    def write_event(self, value):
+        assert self.lpttype == 'SOFTWARE'
+        self.evefile.write('%.6f\t0\t%d\n' % (pylsl.local_clock(), value))
+        return True
+
+    # set data
+    def set_data(self, value):
+        if self.lpttype == 'SOFTWARE':
+            logger.error('set_data() not supported for software trigger.')
+            return False
+        elif self.lpttype == 'MOCK':
+            logger.info('MOCK trigger value %s' % value)
+            return True
+        else:
+            if self.lpttype == 'USB2LPT':
+                self.lpt.setdata(value)
+            elif self.lpttype == 'DESKTOP':
+                self.lpt.setdata(self.portaddr, value)
+            elif self.lpttype == 'ARDUINO':
+                self.ser.write(bytes([value]))
+            else:
+                raise RuntimeError('Wrong trigger device')
+
+    # sends data and turn off after delay
+    def signal(self, value):
+        if self.lpttype == 'SOFTWARE':
+            if self.verbose is True:
+                logger.info('Sending software trigger %s' % value)
+            return self.write_event(value)
+        elif self.lpttype == 'MOCK':
+            logger.info('Sending MOCK trigger signal %s' % value)
+            return True
+        else:
+            if self.offtimer.is_alive():
+                logger.warning('You are sending a new signal before the end of the last signal. Signal ignored.')
+                logger.warning('self.delay=%.1f' % self.delay)
+                return False
+            self.set_data(value)
+            if self.verbose is True:
+                logger.info('Sending %s' % value)
+            self.offtimer.start()
+            return True
+
+    # set data to zero (all bits off)
+    def signal_off(self):
+        if self.lpttype == 'SOFTWARE':
+            return self.write_event(0)
+        elif self.lpttype == 'MOCK':
+            logger.info('MOCK trigger off')
+            return True
+        else:
+            self.set_data(0)
+            self.offtimer = threading.Timer(self.delay, self.signal_off)
+
+    # set pin
+    def set_pin(self, pin):
+        if self.lpttype == 'SOFTWARE':
+            logger.error('set_pin() not supported for software trigger.')
+            return False
+        elif self.lpttype == 'MOCK':
+            logger.info('MOCK trigger pin %s' % pin)
+            return True
+        else:
+            self.set_data(2 ** (pin - 1))
+
+
+# set 1 to each bit and rotate from bit 0 to bit 7
+def test_all_bits(trigger):
+    for x in range(8):
+        val = 2 ** x
+        trigger.signal(val)
+        logger.info(val)
+        time.sleep(1)
+
+# sample test code
+if __name__ == '__main__':
+    trigger = Trigger('ARDUINO') # Arduino trigger
+    #trigger = Trigger('SOFTWARE')
+    if not trigger.init(500):
+        print('LPT port cannot be opened. Using a mock trigger.')
+        trigger = Trigger('MOCK')
+
+    # Christmas tree mode (set 1 bit-by-bit)
+    #test_all_bits(trigger)
+
+    print('Type quit or Ctrl+C to finish.')
+    while True:
+        val = input('Trigger value? ')
+        if val.strip() == '':
+            continue
+        if val == 'quit':
+            break
+        if 0 <= int(val) <= 255:
+            trigger.signal(int(val))
+            print('Sent %d' % int(val))
+        else:
+            print('Ignored %s' % val)
```

### Comparing `neurodecode-2.0.4/neurodecode/triggers/trigger_def.py` & `neurodecode-2.0.5/neurodecode/triggers/trigger_def.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from __future__ import print_function, division
-
-"""
-Reads trigger info and creates a class object with the follwing attributes:
-- self.event_id = event_value
-- self.by_name() = {key:value, ...}
-- self.by_value() = {value:key, ...}
-
-"""
-
-import sys
-import os
-import neurodecode.utils.q_common as qc
-from configparser import ConfigParser
-from neurodecode import logger
-
-def trigger_def(ini_file, verbose=False):
-    class TriggerDef(object):
-        def __init__(self, items):
-            self.by_name = {}
-            self.by_value = {}
-            for key, value in items:
-                value = int(value)
-                setattr(self, key, value)
-                self.by_name[key] = value
-                self.by_value[value] = key
-
-        # show all possible trigger values
-        def check_data(self):
-            print('Attributes of the final class')
-            for attr in dir(self):
-                if not callable(getattr(self, attr)) and not attr.startswith("__"):
-                    print(attr, getattr(self, attr))
-
-    if not os.path.exists(ini_file):
-        if os.path.exists(ini_file):
-            logger.info('Found trigger definition file %s' % ini_file)
-        else:
-            raise FileNotFoundError('Trigger event definition file %s not found' % ini_file)
-    config = ConfigParser(inline_comment_prefixes=('#', ';'))
-    config.optionxform = str
-    config.read(ini_file)
-    return TriggerDef(config.items('events'))
-
-# example
-if __name__ == '__main__':
-    ini_file = 'triggerdef_16.ini'
-    tdef = trigger_def(ini_file)
-
-    # accessing a trigger value as a member variable
-    print('INIT =', tdef.INIT)
-
-    # check whether the trigger name is defined
-    print('\nINIT in tdef.by_name?')
-    print('INIT' in tdef.by_name)
-
-    # check whether the trigger value is defined
-    print('\n255 in tdef.by_value?')
-    print(255 in tdef.by_value)
-    print('\n1 in tdef.by_value?')
-    print(1 in tdef.by_value)
-
-    # print all trigger names and associated values
-    print('\ntdef.by_name')
-    print(tdef.by_name)
-
-    # print all trigger values and associated names
-    print('\ntdef.by_value')
-    print(tdef.by_value)
+from __future__ import print_function, division
+
+"""
+Reads trigger info and creates a class object with the follwing attributes:
+- self.event_id = event_value
+- self.by_name() = {key:value, ...}
+- self.by_value() = {value:key, ...}
+
+"""
+
+import sys
+import os
+import neurodecode.utils.q_common as qc
+from configparser import ConfigParser
+from neurodecode import logger
+
+def trigger_def(ini_file, verbose=False):
+    class TriggerDef(object):
+        def __init__(self, items):
+            self.by_name = {}
+            self.by_value = {}
+            for key, value in items:
+                value = int(value)
+                setattr(self, key, value)
+                self.by_name[key] = value
+                self.by_value[value] = key
+
+        # show all possible trigger values
+        def check_data(self):
+            print('Attributes of the final class')
+            for attr in dir(self):
+                if not callable(getattr(self, attr)) and not attr.startswith("__"):
+                    print(attr, getattr(self, attr))
+
+    if not os.path.exists(ini_file):
+        if os.path.exists(ini_file):
+            logger.info('Found trigger definition file %s' % ini_file)
+        else:
+            raise FileNotFoundError('Trigger event definition file %s not found' % ini_file)
+    config = ConfigParser(inline_comment_prefixes=('#', ';'))
+    config.optionxform = str
+    config.read(ini_file)
+    return TriggerDef(config.items('events'))
+
+# example
+if __name__ == '__main__':
+    ini_file = 'triggerdef_16.ini'
+    tdef = trigger_def(ini_file)
+
+    # accessing a trigger value as a member variable
+    print('INIT =', tdef.INIT)
+
+    # check whether the trigger name is defined
+    print('\nINIT in tdef.by_name?')
+    print('INIT' in tdef.by_name)
+
+    # check whether the trigger value is defined
+    print('\n255 in tdef.by_value?')
+    print(255 in tdef.by_value)
+    print('\n1 in tdef.by_value?')
+    print(1 in tdef.by_value)
+
+    # print all trigger names and associated values
+    print('\ntdef.by_name')
+    print(tdef.by_name)
+
+    # print all trigger values and associated names
+    print('\ntdef.by_value')
+    print(tdef.by_value)
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/Motionstim8.py` & `neurodecode-2.0.5/neurodecode/utils/Motionstim8.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-# -*- coding: utf-8 -*-
-import serial
-import numpy as np
-
-class Motionstim8:
-
-
-
-    def __init__(self):
-
-        # The Motionstim8 device has a serial port
-        self.serialPort = serial.Serial()
-
-        # The default main stimulation frequency being used is 20 Hz
-        self.stimulationFrequency = 50
-
-        # The default group stimulation frequency being used is 50 Hz
-        self.groupStimulationFrequency = 50
-
-        # Set the N factor (0 by default)
-        self.nFactor = 0
-
-        # The number of channels in the FES device
-        self.nChannels = 8
-
-        # The device channel modes (singlets)
-        self.pulseModes = [0] * self.nChannels
-
-        # The device pulse widths
-        self.pulseWidths = [300] * self.nChannels
-
-        # The device amplitudes
-        self.amplitudes = [0] * self.nChannels
-
-
-
-
-    def OpenSerialPort(self, comPortName):
-
-        # configure the serial connections (the parameters differs on the device you are connecting to)
-        self.serialPort.port = comPortName
-        self.serialPort.baudrate = 115200
-        self.serialPort.parity = serial.PARITY_NONE
-        self.serialPort.stopbits = serial.STOPBITS_ONE
-        self.serialPort.bytesize = serial.EIGHTBITS
-        self.serialPort.timeout = 500
-        self.serialPort.write_timeout = 500
-        self.serialPort.xonxoff  = False
-        self.serialPort.rtscts = False
-        self.dsrdtr = False
-
-        # Open the port if not already opened
-        if not self.serialPort.is_open:
-            self.serialPort.open()
-
-
-
-
-    def CloseSerialPort(self):
-
-        # Close the serial port if it is open
-        if self.serialPort.is_open:
-            self.serialPort.close()
-
-
-
-    def WriteFES(self, bitString):
-
-        # Write a bitstring through the open serial port
-        if self.serialPort.is_open:
-
-            # Convert the bit string in to a bytes object
-            byteString = int(bitString, 2).to_bytes(len(bitString) // 8, byteorder='big')
-            bytesWritten = self.serialPort.write(byteString)
-            self.serialPort.flush()
-
-        else:
-            print("Error writing to FES device: serial port not opened")
-
-
-
-    # A method to initialize the device into Channel List Mode
-    def InitializeChannelListMode(self):
-
-        # Set ts1 and ts2
-        ts1 = 1000  / self.stimulationFrequency
-        ts2 = 1000 / self.groupStimulationFrequency
-
-        # Compute the group and main times
-        mainTime = int((ts1 - 1.0) / 0.5)
-        groupTime = int((ts2 - 1.5) / 0.5)
-
-        # Set the active channels according to the input
-        activeChannelsString = "11111111"
-
-        # Specify which channels apply the scaler to get lower frequencies (none by default)
-        lowFrequencyChannelsString = "00000000"
-
-        # Compute checksum
-        checksum = (self.nFactor + int(activeChannelsString) + int(lowFrequencyChannelsString) + groupTime + mainTime) % 8
-
-        # Convert each parameter to its correct binary representation
-        mainTimeBinary = "{0:011b}".format(mainTime)                              # binary, 11 bit width, 0 padding
-        nFactorBinary = "{0:03b}".format(self.nFactor)                                 # binary, 3 bit width, 0 padding
-        groupTimeBinary = "{0:05b}".format(groupTime)                             # binary, 5 bit width, 0 padding
-        checksumBinary = "{0:03b}".format(checksum)                               # binary, 3 bit width, 0 padding
-
-        # Compose the complete bistring
-        bitString = "100"\
-                    + checksumBinary\
-                    + nFactorBinary[0:2]\
-                    + "0"\
-                    + nFactorBinary[2:3]\
-                    + activeChannelsString[0:6]\
-                    + "0"\
-                    + activeChannelsString[6:8]\
-                    + lowFrequencyChannelsString[0:5]\
-                    + "0"\
-                    + lowFrequencyChannelsString[5:8]\
-                    + "00"\
-                    + groupTimeBinary[0:2]\
-                    + "0"\
-                    + groupTimeBinary[2:5]\
-                    + mainTimeBinary[0:4]\
-                    + "0"\
-                    + mainTimeBinary[4:11]
-
-        # Write the bit string
-        self.WriteFES(bitString)
-
-
-
-    def UpdateChannelSettings(self, newAmplitudes):
-
-        # Ensure that the device amplitudes are capped between the safety bounds 0 - 50 mA
-        for index, amplitude in enumerate(newAmplitudes):
-
-            if amplitude > 50:
-
-                self.amplitudes[index] = 50
-
-            elif amplitude < 0:
-
-                self.amplitudes[index] = 0
-
-            else:
-
-                self.amplitudes[index] = newAmplitudes[index]
-
-        # Compute checksum
-        checksum = (np.sum(self.pulseModes) + np.sum(self.pulseWidths) + np.sum(self.amplitudes)) % 32
-
-        # Construct the channel settings string
-        checksumBinary = "{0:05b}".format(checksum)
-
-        channelSettingsBinary = ""
-        for amplitude, pulseWidth, pulseMode in zip(self.amplitudes, self.pulseWidths, self.pulseModes):
-
-            pulseWidthBinary = "{0:09b}".format(pulseWidth)
-            channelSettingBinary = "0"\
-                                   + "{0:02b}".format(pulseMode)\
-                                   + "000"\
-                                   + pulseWidthBinary[0:2]\
-                                   + "0"\
-                                   + pulseWidthBinary[2:9]\
-                                   + "0"\
-                                   + "{0:07b}".format(amplitude)
-
-            channelSettingsBinary += channelSettingBinary
-
-        # Compose the final bitstring
-        bitString = "101" + checksumBinary + channelSettingsBinary
-
-        # Write the bit string
-        self.WriteFES(bitString)
-
-
-    def StopDevice(self):
-
-        # Compose the stop command
-        stopCommandBinary = "11000000"
-
-        # Write the bit string
-        self.WriteFES(stopCommandBinary)
+# -*- coding: utf-8 -*-
+import serial
+import numpy as np
+
+class Motionstim8:
+
+
+
+    def __init__(self):
+
+        # The Motionstim8 device has a serial port
+        self.serialPort = serial.Serial()
+
+        # The default main stimulation frequency being used is 20 Hz
+        self.stimulationFrequency = 50
+
+        # The default group stimulation frequency being used is 50 Hz
+        self.groupStimulationFrequency = 50
+
+        # Set the N factor (0 by default)
+        self.nFactor = 0
+
+        # The number of channels in the FES device
+        self.nChannels = 8
+
+        # The device channel modes (singlets)
+        self.pulseModes = [0] * self.nChannels
+
+        # The device pulse widths
+        self.pulseWidths = [300] * self.nChannels
+
+        # The device amplitudes
+        self.amplitudes = [0] * self.nChannels
+
+
+
+
+    def OpenSerialPort(self, comPortName):
+
+        # configure the serial connections (the parameters differs on the device you are connecting to)
+        self.serialPort.port = comPortName
+        self.serialPort.baudrate = 115200
+        self.serialPort.parity = serial.PARITY_NONE
+        self.serialPort.stopbits = serial.STOPBITS_ONE
+        self.serialPort.bytesize = serial.EIGHTBITS
+        self.serialPort.timeout = 500
+        self.serialPort.write_timeout = 500
+        self.serialPort.xonxoff  = False
+        self.serialPort.rtscts = False
+        self.dsrdtr = False
+
+        # Open the port if not already opened
+        if not self.serialPort.is_open:
+            self.serialPort.open()
+
+
+
+
+    def CloseSerialPort(self):
+
+        # Close the serial port if it is open
+        if self.serialPort.is_open:
+            self.serialPort.close()
+
+
+
+    def WriteFES(self, bitString):
+
+        # Write a bitstring through the open serial port
+        if self.serialPort.is_open:
+
+            # Convert the bit string in to a bytes object
+            byteString = int(bitString, 2).to_bytes(len(bitString) // 8, byteorder='big')
+            bytesWritten = self.serialPort.write(byteString)
+            self.serialPort.flush()
+
+        else:
+            print("Error writing to FES device: serial port not opened")
+
+
+
+    # A method to initialize the device into Channel List Mode
+    def InitializeChannelListMode(self):
+
+        # Set ts1 and ts2
+        ts1 = 1000  / self.stimulationFrequency
+        ts2 = 1000 / self.groupStimulationFrequency
+
+        # Compute the group and main times
+        mainTime = int((ts1 - 1.0) / 0.5)
+        groupTime = int((ts2 - 1.5) / 0.5)
+
+        # Set the active channels according to the input
+        activeChannelsString = "11111111"
+
+        # Specify which channels apply the scaler to get lower frequencies (none by default)
+        lowFrequencyChannelsString = "00000000"
+
+        # Compute checksum
+        checksum = (self.nFactor + int(activeChannelsString) + int(lowFrequencyChannelsString) + groupTime + mainTime) % 8
+
+        # Convert each parameter to its correct binary representation
+        mainTimeBinary = "{0:011b}".format(mainTime)                              # binary, 11 bit width, 0 padding
+        nFactorBinary = "{0:03b}".format(self.nFactor)                                 # binary, 3 bit width, 0 padding
+        groupTimeBinary = "{0:05b}".format(groupTime)                             # binary, 5 bit width, 0 padding
+        checksumBinary = "{0:03b}".format(checksum)                               # binary, 3 bit width, 0 padding
+
+        # Compose the complete bistring
+        bitString = "100"\
+                    + checksumBinary\
+                    + nFactorBinary[0:2]\
+                    + "0"\
+                    + nFactorBinary[2:3]\
+                    + activeChannelsString[0:6]\
+                    + "0"\
+                    + activeChannelsString[6:8]\
+                    + lowFrequencyChannelsString[0:5]\
+                    + "0"\
+                    + lowFrequencyChannelsString[5:8]\
+                    + "00"\
+                    + groupTimeBinary[0:2]\
+                    + "0"\
+                    + groupTimeBinary[2:5]\
+                    + mainTimeBinary[0:4]\
+                    + "0"\
+                    + mainTimeBinary[4:11]
+
+        # Write the bit string
+        self.WriteFES(bitString)
+
+
+
+    def UpdateChannelSettings(self, newAmplitudes):
+
+        # Ensure that the device amplitudes are capped between the safety bounds 0 - 50 mA
+        for index, amplitude in enumerate(newAmplitudes):
+
+            if amplitude > 50:
+
+                self.amplitudes[index] = 50
+
+            elif amplitude < 0:
+
+                self.amplitudes[index] = 0
+
+            else:
+
+                self.amplitudes[index] = newAmplitudes[index]
+
+        # Compute checksum
+        checksum = (np.sum(self.pulseModes) + np.sum(self.pulseWidths) + np.sum(self.amplitudes)) % 32
+
+        # Construct the channel settings string
+        checksumBinary = "{0:05b}".format(checksum)
+
+        channelSettingsBinary = ""
+        for amplitude, pulseWidth, pulseMode in zip(self.amplitudes, self.pulseWidths, self.pulseModes):
+
+            pulseWidthBinary = "{0:09b}".format(pulseWidth)
+            channelSettingBinary = "0"\
+                                   + "{0:02b}".format(pulseMode)\
+                                   + "000"\
+                                   + pulseWidthBinary[0:2]\
+                                   + "0"\
+                                   + pulseWidthBinary[2:9]\
+                                   + "0"\
+                                   + "{0:07b}".format(amplitude)
+
+            channelSettingsBinary += channelSettingBinary
+
+        # Compose the final bitstring
+        bitString = "101" + checksumBinary + channelSettingsBinary
+
+        # Write the bit string
+        self.WriteFES(bitString)
+
+
+    def StopDevice(self):
+
+        # Compose the stop command
+        stopCommandBinary = "11000000"
+
+        # Write the bit string
+        self.WriteFES(stopCommandBinary)
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/benchmark_multitaper.py` & `neurodecode-2.0.5/neurodecode/utils/benchmark_multitaper.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-# -*- coding: utf-8 -*-
-from __future__ import print_function, division
-
-"""
-Measure multitaper computation speed.
-
-i7-8700K: 9.9 ms (101.0 Hz)
-
-@author: leeq
-"""
-
-import os
-import mne
-import numpy as np
-import neurodecode.utils.q_common as qc
-from neurodecode import logger
-
-os.environ['OMP_NUM_THREADS'] = '1' # actually improves performance for multitaper
-
-
-def main():
-    fmin = 1
-    fmax = 40
-    channels = 64
-    wlen = 0.5 # window length in seconds
-    sfreq = 512
-    num_iterations = 500
-
-    signal = np.random.rand(channels, int(np.round(sfreq * wlen)))
-    psde = mne.decoding.PSDEstimator(sfreq=sfreq, fmin=fmin,\
-        fmax=fmax, bandwidth=None, adaptive=False, low_bias=True,\
-        n_jobs=1, normalization='length', verbose=None)
-
-    tm = qc.Timer()
-    times = []
-    for i in range(num_iterations):
-        tm.reset()
-        psd = psde.transform(signal.reshape((1, signal.shape[0], signal.shape[1])))
-        times.append(tm.msec())
-        if i % 100 == 0:
-            logger.info('%d / %d' % (i, num_iterations))
-    ms = np.mean(times)
-    fps = 1000 / ms
-    logger.info('Average = %.1f ms (%.1f Hz)' % (ms, fps))
-
-if __name__ == '__main__':
-    main()
+# -*- coding: utf-8 -*-
+from __future__ import print_function, division
+
+"""
+Measure multitaper computation speed.
+
+i7-8700K: 9.9 ms (101.0 Hz)
+
+@author: leeq
+"""
+
+import os
+import mne
+import numpy as np
+import neurodecode.utils.q_common as qc
+from neurodecode import logger
+
+os.environ['OMP_NUM_THREADS'] = '1' # actually improves performance for multitaper
+
+
+def main():
+    fmin = 1
+    fmax = 40
+    channels = 64
+    wlen = 0.5 # window length in seconds
+    sfreq = 512
+    num_iterations = 500
+
+    signal = np.random.rand(channels, int(np.round(sfreq * wlen)))
+    psde = mne.decoding.PSDEstimator(sfreq=sfreq, fmin=fmin,\
+        fmax=fmax, bandwidth=None, adaptive=False, low_bias=True,\
+        n_jobs=1, normalization='length', verbose=None)
+
+    tm = qc.Timer()
+    times = []
+    for i in range(num_iterations):
+        tm.reset()
+        psd = psde.transform(signal.reshape((1, signal.shape[0], signal.shape[1])))
+        times.append(tm.msec())
+        if i % 100 == 0:
+            logger.info('%d / %d' % (i, num_iterations))
+    ms = np.mean(times)
+    fps = 1000 / ms
+    logger.info('Average = %.1f ms (%.1f Hz)' % (ms, fps))
+
+if __name__ == '__main__':
+    main()
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/convert2fif.py` & `neurodecode-2.0.5/neurodecode/utils/convert2fif.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,556 +1,556 @@
-from __future__ import print_function, division, unicode_literals
-
-"""
-Convert known file format to FIF.
-
-
-Kyuhwa Lee, 2014
-Swiss Federal Institute of Technology Lausanne (EPFL)
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""
-
-import os
-import sys
-import mne
-import pdb
-import scipy.io
-import numpy as np
-import neurodecode.utils.q_common as qc
-import neurodecode.utils.pycnbi_utils as pu
-from neurodecode.pycnbi_config import CAP, LAPLACIAN
-from neurodecode import logger
-from builtins import input
-from pathlib import Path
-
-mne.set_log_level('ERROR')
-
-
-def event_timestamps_to_indices(sigfile, eventfile, offset=0):
-    """
-    Convert LSL timestamps to sample indices for separetely recorded events.
-
-    Parameters:
-    sigfile: raw signal file (Python Pickle) recorded with stream_recorder.py.
-    eventfile: event file where events are indexed with LSL timestamps.
-    offset: if the LSL server's timestamp is shifted, correct with offset value in seconds.
-
-    Returns:
-    events list, which can be used as an input to mne.io.RawArray.add_events().
-    """
-
-    raw = qc.load_obj(sigfile)
-    ts = raw['timestamps'].reshape(-1)
-    ts_min = min(ts)
-    ts_max = max(ts)
-    events = []
-
-    with open(eventfile) as f:
-        for l in f:
-            data = l.strip().split('\t')
-            event_ts = float(data[0]) + offset
-            event_value = int(data[2])
-            # find the first index not smaller than ts
-            next_index = np.searchsorted(ts, event_ts)
-            if next_index >= len(ts):
-                logger.warning('Event %d at time %.3f is out of time range (%.3f - %.3f).' % (event_value, event_ts, ts_min, ts_max))
-            else:
-                events.append([next_index, 0, event_value])
-    return events
-
-
-def convert2mat(filename, matfile):
-    """
-    Convert to mat using MATLAB BioSig sload().
-    """
-    basename = '.'.join(filename.split('.')[:-1])
-    # extension= filename.split('.')[-1]
-    matfile = basename + '.mat'
-    if not os.path.exists(matfile):
-        logger.info('Converting input to mat file')
-        run = "[sig,header]=sload('%s'); save('%s.mat','sig','header');" % (filename, basename)
-        qc.matlab(run)
-        if not os.path.exists(matfile):
-            logger.error('mat file convertion error.')
-            sys.exit()
-
-
-def pcl2fif(filename, interactive=False, outdir=None, external_event=None, offset=0, overwrite=False, precision='single'):
-    """
-    PyCNBI Python pickle file
-
-    Params
-    --------
-    outdir: If None, it will be the subdirectory of the fif file.
-    external_event: Event file in text format. Each row should be: "SAMPLE_INDEX 0 EVENT_TYPE"
-    precision: Data matrix format. 'single' improves backward compatability.
-    """
-    fdir, fname, fext = qc.parse_path_list(filename)
-    if outdir is None:
-        outdir = fdir + 'fif/'
-    elif outdir[-1] != '/':
-        outdir += '/'
-
-    data = qc.load_obj(filename)
-
-    if type(data['signals']) == list:
-        signals_raw = np.array(data['signals'][0]).T  # to channels x samples
-    else:
-        signals_raw = data['signals'].T  # to channels x samples
-    sample_rate = data['sample_rate']
-
-    if 'ch_names' not in data:
-        ch_names = ['CH%d' % (x + 1) for x in range(signals_raw.shape[0])]
-    else:
-        ch_names = data['ch_names']
-
-    # search for event channel
-    trig_ch = pu.find_event_channel(signals_raw, ch_names)
-
-    ''' TODO: REMOVE
-    # exception
-    if trig_ch is None:
-        logger.warning('Inferred event channel is None.')
-        if interactive:
-            logger.warning('If you are sure everything is alright, press Enter.')
-            input()
-
-    # fix wrong event channel
-    elif trig_ch_guess != trig_ch:
-        logger.warning('Specified event channel (%d) != inferred event channel (%d).' % (trig_ch, trig_ch_guess))
-        if interactive: input('Press Enter to fix. Event channel will be set to %d.' % trig_ch_guess)
-        ch_names.insert(trig_ch_guess, ch_names.pop(trig_ch))
-        trig_ch = trig_ch_guess
-        logger.info('New channel list:')
-        for c in ch_names:
-            logger.info('%s' % c)
-        logger.info('Event channel is now set to %d' % trig_ch)
-    '''
-
-    # move trigger channel to index 0
-    if trig_ch is None:
-        # assuming no event channel exists, add a event channel to index 0 for consistency.
-        logger.warning('No event channel was not found. Adding a blank event channel to index 0.')
-        eventch = np.zeros([1, signals_raw.shape[1]])
-        signals = np.concatenate((eventch, signals_raw), axis=0)
-        num_eeg_channels = signals_raw.shape[0] # data['channels'] is not reliable any more
-        trig_ch = 0
-        ch_names = ['TRIGGER'] + ['CH%d' % (x + 1) for x in range(num_eeg_channels)]
-    elif trig_ch == 0:
-        signals = signals_raw
-        num_eeg_channels = data['channels'] - 1
-    else:
-        # move event channel to 0
-        logger.info('Moving event channel %d to 0.' % trig_ch)
-        signals = np.concatenate((signals_raw[[trig_ch]], signals_raw[:trig_ch], signals_raw[trig_ch + 1:]), axis=0)
-        assert signals_raw.shape == signals.shape
-        num_eeg_channels = data['channels'] - 1
-        ch_names.pop(trig_ch)
-        trig_ch = 0
-        ch_names.insert(trig_ch, 'TRIGGER')
-        logger.info('New channel list:')
-        for c in ch_names:
-            logger.info('%s' % c)
-
-    ch_info = ['stim'] + ['eeg'] * num_eeg_channels
-    info = mne.create_info(ch_names, sample_rate, ch_info)
-
-    # create Raw object
-    raw = mne.io.RawArray(signals, info)
-    raw._times = data['timestamps'] # seems to have no effect
-
-    if external_event is not None:
-        raw._data[0] = 0  # erase current events
-        events_index = event_timestamps_to_indices(filename, external_event, offset)
-        if len(events_index) == 0:
-            logger.warning('No events were found in the event file')
-        else:
-            logger.info('Found %d events' % len(events_index))
-            raw.add_events(events_index, stim_channel='TRIGGER')
-
-    qc.make_dirs(outdir)
-    fiffile = outdir + fname + '.fif'
-
-    raw.save(fiffile, verbose=False, overwrite=overwrite, fmt=precision)
-    logger.info('Saved to %s' % fiffile)
-
-    saveChannels2txt(outdir, ch_names)
-
-    return True
-
-
-def eeg2fif(filename, interactive=False, outdir=None):
-    """
-    Brain Products EEG format
-    """
-    fdir, fname, fext = qc.parse_path_list(filename)
-    if outdir is None:
-        outdir = fdir
-    elif outdir[-1] != '/':
-        outdir += '/'
-
-    eegfile = fdir + fname + '.eeg'
-    matfile = fdir + fname + '.mat'
-    markerfile = fdir + fname + '.vmrk'
-    fiffile = outdir + fname + '.fif'
-
-    # convert to mat using MATLAB
-    if not os.path.exists(matfile):
-        logger.info('Converting input to mat file')
-        run = "[sig,header]=sload('%s'); save('%s','sig','header');" % (eegfile, matfile)
-        qc.matlab(run)
-        if not os.path.exists(matfile):
-            logger.error('mat file convertion error.')
-            sys.exit()
-    else:
-        logger.warning('MAT file already exists. Skipping conversion.')
-
-    # extract events
-    events = []
-    for l in open(markerfile):
-        if 'Stimulus,S' in l:
-            # event, sample_index= l.split('  ')[-1].split(',')[:2]
-            data = l.split(',')[1:3]
-            event = int(data[0][1:])  # ignore 'S'
-            sample_index = int(data[1])
-            events.append([sample_index, 0, event])
-
-    # load data and create fif header
-    mat = scipy.io.loadmat(matfile)
-    # headers= mat['header']
-    sample_rate = int(mat['header']['SampleRate'])
-    signals = mat['sig'].T  # channels x samples
-    nch, t_len = signals.shape
-    ch_names = ['TRIGGER'] + ['CH%d' % (x + 1) for x in range(nch)]
-    ch_info = ['stim'] + ['eeg'] * (nch)
-    info = mne.create_info(ch_names, sample_rate, ch_info, montage='standard_1005')
-
-    # add event channel
-    eventch = np.zeros([1, signals.shape[1]])
-    signals = np.concatenate((eventch, signals), axis=0)
-
-    # create Raw object
-    raw = mne.io.RawArray(signals, info)
-
-    # add events
-    raw.add_events(events, 'TRIGGER')
-
-    # save and close
-    raw.save(fiffile, verbose=False, overwrite=True, fmt='double')
-    logger.info('Saved to %s' % fiffile)
-
-    saveChannels2txt(outdir, ch_names)
-
-
-def gdf2fif(filename, interactive=False, outdir=None, channel_file=None):
-    """
-    g.Tec gdf format
-
-    Assumes the last channel is event channel.
-    """
-    fdir, fname, fext = qc.parse_path_list(filename)
-    if outdir is None:
-        outdir = fdir
-    elif outdir[-1] != '/':
-        outdir += '/'
-
-    fiffile = outdir + fname + '.fif'
-    matfile = fdir + fname + '.mat'
-
-    convert2mat(fdir + fname + '.gdf', matfile)
-    mat = scipy.io.loadmat(matfile)
-    os.remove(matfile)
-    sample_rate = int(mat['header']['SampleRate'])
-    nch = mat['sig'].shape[1]
-
-    # read events from header
-    evtype = mat['header']['EVENT'][0][0][0]['TYP'][0]
-    evpos = mat['header']['EVENT'][0][0][0]['POS'][0]
-    events = []
-    for e in range(evtype.shape[0]):
-        label = int(evtype[e])
-        events.append([int(evpos[e][0]), 0, label])
-
-    signals_raw = mat['sig'].T  # -> channels x samples
-
-    ''' it seems they fixed the bug now
-    # Note: Biosig's sload() sometimes returns bogus event values so we use the following for events
-    raw= mne.io.read_raw_edf(filename, preload=True)
-    events= mne.find_events(raw, stim_channel='TRIGGER', shortest_event=1, consecutive=True)
-    #signals_raw[-1][:]= raw._data[-1][:] # overwrite with the correct event values
-    '''
-
-    # Move the event channel to 0 (for consistency)
-    signals = np.concatenate((signals_raw[-1, :].reshape(1, -1), signals_raw[:-1, :]))
-    signals[0] *= 0  # init the event channel
-
-    # Note: gdf might have a software event channel
-    if channel_file is None:
-        ch_names = ['TRIGGER'] + ['CH%d' % x for x in range(1, nch)]
-    else:
-        ch_names_raw = []
-        for l in open(channel_file):
-            ch_names_raw.append(l.strip())
-        if ch_names_raw[-1] != 'TRIGGER':
-            input(
-                'Warning: Trigger channel is assumed to be the last channel. Press Ctrl+C if this is not the case.')
-        ch_names = ['TRIGGER'] + ch_names_raw[:-1]
-    ch_info = ['stim'] + ['eeg'] * (nch - 1)
-    info = mne.create_info(ch_names, sample_rate, ch_info)
-
-    # create Raw object
-    raw = mne.io.RawArray(signals, info)
-
-    # add events
-    raw.add_events(events, 'TRIGGER')
-
-    # save and close
-    raw.save(fiffile, verbose=False, overwrite=True, fmt='double')
-    logger.info('Saved to %s' % fiffile)
-
-    saveChannels2txt(outdir, ch_names)
-
-
-def bdf2fif(filename, interactive=False, outdir=None):
-    """
-    EDF or BioSemi BDF format
-    """
-    # convert to mat using MATLAB (MNE's edf reader has an offset bug)
-    fdir, fname, fext = qc.parse_path_list(filename)
-    if outdir is None:
-        outdir = fdir
-    elif outdir[-1] != '/':
-        outdir += '/'
-
-    fiffile = outdir + fname + '.fif'
-    raw = mne.io.read_raw_edf(filename, preload=True)
-
-    # process event channel
-    if raw.info['chs'][-1]['ch_name'] != 'STI 014':
-        logger.error("The last channel (%s) doesn't seem to be an event channel. Entering debugging mode." % raw.info['chs'][-1]['ch_name'])
-        pdb.set_trace()
-    raw.info['chs'][-1]['ch_name'] = 'TRIGGER'
-    events = mne.find_events(raw, stim_channel='TRIGGER', shortest_event=1, uint_cast=True, consecutive=True)
-    events[:, 2] -= events[:, 1]  # set offset to 0
-    events[:, 1] = 0
-    # move the event channel to index 0 (for consistency)
-    raw._data = np.concatenate((raw._data[-1, :].reshape(1, -1), raw._data[:-1, :]))
-    raw._data[0] *= 0  # init the event channel
-    raw.info['chs'] = [raw.info['chs'][-1]] + raw.info['chs'][:-1]
-
-    # add events
-    raw.add_events(events, 'TRIGGER')
-
-    # save and close
-    raw.save(fiffile, verbose=False, overwrite=True, fmt='double')
-    logger.info('Saved to %s' % fiffile)
-
-    saveChannels2txt(outdir, ch_names)
-
-
-def bdf2fif_matlab(filename, interactive=False, outdir=None):
-    """
-    BioSemi bdf reader using BioSig toolbox of MATLAB.
-    """
-    # convert to mat using MATLAB (MNE's edf reader has an offset bug)
-    fdir, fname, fext = qc.parse_path_list(filename)
-    if outdir is None:
-        outdir = fdir
-    elif outdir[-1] != '/':
-        outdir += '/'
-
-    fiffile = outdir + fname + '.fif'
-    matfile = outdir + fname + '.mat'
-
-    if not os.path.exists(matfile):
-        logger.info('Converting input to mat file')
-        run = "[sig,header]=sload('%s'); save('%s','sig','header');" % (filename, matfile)
-        qc.matlab(run)
-        if not os.path.exists(matfile):
-            logger.error('mat file convertion error.')
-            sys.exit()
-
-    mat = scipy.io.loadmat(matfile)
-    os.remove(matfile)
-    sample_rate = int(mat['header']['SampleRate'])
-    nch = mat['sig'].shape[1]
-
-    # assume Biosemi always has the same number of channels
-    if nch == 73:
-        ch_names = CAP['BIOSEMI_64']
-        extra_ch = nch - len(CAP['BIOSEMI_64_INFO'])
-        extra_names = []
-        for ch in range(extra_ch):
-            extra_names.append('EXTRA%d' % ch)
-        ch_names = ch_names + extra_names
-        ch_info = CAP['BIOSEMI_64_INFO'] + ['misc'] * extra_ch
-    else:
-        logger.warning('Unrecognized number of channels (%d)' % nch)
-        logger.warning('The last channel will be assumed to be trigger. Press Enter to continue, or Ctrl+C to break.')
-        if interactive:
-            input()
-
-        # Set the trigger to be channel 0 because later we will move it to channel 0.
-        ch_names = ['TRIGGER'] + ['CH%d' % (x + 1) for x in range(nch - 1)]
-        ch_info = ['stim'] + ['eeg'] * (nch - 1)
-
-    signals_raw = mat['sig'].T  # -> channels x samples
-
-    # Note: Biosig's sload() sometimes returns bogus event values so we use the following for events
-    bdf = mne.io.read_raw_edf(filename, preload=True)
-    events = mne.find_events(bdf, stim_channel='TRIGGER', shortest_event=1, consecutive=True)
-    # signals_raw[-1][:]= bdf._data[-1][:] # overwrite with the correct event values
-
-    # Move the event channel to 0 (for consistency)
-    signals = np.concatenate((signals_raw[-1, :].reshape(1, -1), signals_raw[:-1, :]))
-    signals[0] *= 0  # init the event channel
-
-    info = mne.create_info(ch_names, sample_rate, ch_info, montage='standard_1005')
-
-    # create Raw object
-    raw = mne.io.RawArray(signals, info)
-
-    # add events
-    raw.add_events(events, 'TRIGGER')
-
-    # save and close
-    raw.save(fiffile, verbose=False, overwrite=True, fmt='double')
-    logger.info('Saved to %s' % fiffile)
-
-    saveChannels2txt(outdir, ch_names)
-
-
-def xdf2fif(filename, interactive=False, outdir=None):
-    """
-    Convert XDF format
-    """
-    from pyxdf import pyxdf
-    pyxdf.logger.setLevel('WARNING')
-
-    fdir, fname, fext = qc.parse_path_list(filename)
-    if outdir is None:
-        outdir = fdir
-    elif outdir[-1] != '/':
-        outdir += '/'
-
-    fiffile = outdir + fname + '.fif'
-
-    # channel x times
-    data = pyxdf.load_xdf(filename)
-    raw_data = data[0][0]['time_series'].T
-    if np.max(raw_data[:-1]) < 1:
-        logger.info('Assuming the signal unit is volate (V). Converting to uV')
-        raw_data[:-1] *= 10**6
-
-    signals = np.concatenate((raw_data[-1, :].reshape(1, -1), raw_data[:-1, :]))
-
-    sample_rate = int(data[0][0]['info']['nominal_srate'][0])
-    # TODO: check the event channel index and move to the 0-th index
-    # in LSL, usually the name is TRIG or STI 014.
-    ch_names = []
-    for ch in data[0][0]['info']['desc'][0]['channels'][0]['channel']:
-        ch_names.append(ch['label'][0])
-    trig_ch_guess = pu.find_event_channel(signals, ch_names)
-    if trig_ch_guess is None:
-        trig_ch_guess = 0
-    ch_names =['TRIGGER'] + ch_names[:trig_ch_guess] + ch_names[trig_ch_guess+1:]
-    ch_info = ['stim'] + ['eeg'] * (len(ch_names)-1)
-
-    # fif header creation
-    info = mne.create_info(ch_names, sample_rate, ch_info)
-    raw = mne.io.RawArray(signals, info)
-    #raw.add_events(events_index, stim_channel='TRIGGER')
-
-    # save and close
-    raw.save(fiffile, verbose=False, overwrite=True, fmt='double')
-    logger.info('Saved to %s' % fiffile)
-
-    saveChannels2txt(outdir, ch_names)
-
-
-
-def any2fif(filename, interactive=False, outdir=None, channel_file=None):
-    """
-    Generic file format converter
-    """
-    p = qc.parse_path(filename)
-    if outdir is not None:
-        qc.make_dirs(outdir)
-
-    if p.ext == 'pcl':
-        eve_file = '%s/%s.txt' % (p.dir, p.name.replace('raw', 'eve'))
-        if os.path.exists(eve_file):
-            logger.info('Adding events from %s' % eve_file)
-            eveoffset_file = qc.parse_path(eve_file).name + '-offset.txt'
-            if os.path.exists(eveoffset_file):
-                offset = float(open(eveoffset_file).readline().split('Offset: ')[-1].strip())
-                logger.info('Adding event offset %.1f from %s' % (offset, eve_file))
-        else:
-            eve_file = None
-        pcl2fif(filename, interactive=interactive, outdir=outdir, external_event=eve_file, offset=offset)
-    elif p.ext == 'eeg':
-        eeg2fif(filename, interactive=interactive, outdir=outdir)
-    elif p.ext in ['edf', 'bdf']:
-        bdf2fif(filename, interactive=interactive, outdir=outdir)
-    elif p.ext == 'gdf':
-        gdf2fif(filename, interactive=interactive, outdir=outdir, channel_file=channel_file)
-    elif p.ext == 'xdf':
-        xdf2fif(filename, interactive=interactive, outdir=outdir)
-    else:  # unknown format
-        logger.error('Ignored unrecognized file extension %s. It should be [.pcl | .eeg | .gdf | .bdf]' % p.ext)
-
-
-def saveChannels2txt(outdir, ch_names):
-    """
-    Save the channels list to a txt file for the GUI
-    """
-
-    filename = outdir + "channelsList.txt"
-    config = Path(filename)
-
-    if config.is_file() is False:
-        file = open(filename, "w")
-        for x in range(len(ch_names)):
-            file.write(ch_names[x] + "\n")
-        file.close()
-
-
-def main():
-    """
-    Invoked from the console
-    """
-    if len(sys.argv) == 1:
-        print('Usage: %s data_dir [channel_file]' % os.path.basename(__file__))
-        return
-
-    input_dir = sys.argv[1]
-    if len(sys.argv) > 2:
-        channel_file = sys.argv[2]
-    else:
-        channel_file = None
-
-    count = 0
-    for f in qc.get_file_list(input_dir, fullpath=True, recursive=True):
-        p = qc.parse_path(f)
-        outdir = p.dir + '/fif/'
-        if p.ext in ['pcl', 'bdf', 'edf', 'gdf', 'eeg', 'xdf']:
-            logger.info('Converting %s' % f)
-            any2fif(f, interactive=True, outdir=outdir, channel_file=channel_file)
-            count += 1
-
-    logger.info('%d files converted.' % count)
-
-if __name__ == '__main__':
-    main()
+from __future__ import print_function, division, unicode_literals
+
+"""
+Convert known file format to FIF.
+
+
+Kyuhwa Lee, 2014
+Swiss Federal Institute of Technology Lausanne (EPFL)
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+"""
+
+import os
+import sys
+import mne
+import pdb
+import scipy.io
+import numpy as np
+import neurodecode.utils.q_common as qc
+import neurodecode.utils.pycnbi_utils as pu
+from neurodecode.pycnbi_config import CAP, LAPLACIAN
+from neurodecode import logger
+from builtins import input
+from pathlib import Path
+
+mne.set_log_level('ERROR')
+
+
+def event_timestamps_to_indices(sigfile, eventfile, offset=0):
+    """
+    Convert LSL timestamps to sample indices for separetely recorded events.
+
+    Parameters:
+    sigfile: raw signal file (Python Pickle) recorded with stream_recorder.py.
+    eventfile: event file where events are indexed with LSL timestamps.
+    offset: if the LSL server's timestamp is shifted, correct with offset value in seconds.
+
+    Returns:
+    events list, which can be used as an input to mne.io.RawArray.add_events().
+    """
+
+    raw = qc.load_obj(sigfile)
+    ts = raw['timestamps'].reshape(-1)
+    ts_min = min(ts)
+    ts_max = max(ts)
+    events = []
+
+    with open(eventfile) as f:
+        for l in f:
+            data = l.strip().split('\t')
+            event_ts = float(data[0]) + offset
+            event_value = int(data[2])
+            # find the first index not smaller than ts
+            next_index = np.searchsorted(ts, event_ts)
+            if next_index >= len(ts):
+                logger.warning('Event %d at time %.3f is out of time range (%.3f - %.3f).' % (event_value, event_ts, ts_min, ts_max))
+            else:
+                events.append([next_index, 0, event_value])
+    return events
+
+
+def convert2mat(filename, matfile):
+    """
+    Convert to mat using MATLAB BioSig sload().
+    """
+    basename = '.'.join(filename.split('.')[:-1])
+    # extension= filename.split('.')[-1]
+    matfile = basename + '.mat'
+    if not os.path.exists(matfile):
+        logger.info('Converting input to mat file')
+        run = "[sig,header]=sload('%s'); save('%s.mat','sig','header');" % (filename, basename)
+        qc.matlab(run)
+        if not os.path.exists(matfile):
+            logger.error('mat file convertion error.')
+            sys.exit()
+
+
+def pcl2fif(filename, interactive=False, outdir=None, external_event=None, offset=0, overwrite=False, precision='single'):
+    """
+    PyCNBI Python pickle file
+
+    Params
+    --------
+    outdir: If None, it will be the subdirectory of the fif file.
+    external_event: Event file in text format. Each row should be: "SAMPLE_INDEX 0 EVENT_TYPE"
+    precision: Data matrix format. 'single' improves backward compatability.
+    """
+    fdir, fname, fext = qc.parse_path_list(filename)
+    if outdir is None:
+        outdir = fdir + 'fif/'
+    elif outdir[-1] != '/':
+        outdir += '/'
+
+    data = qc.load_obj(filename)
+
+    if type(data['signals']) == list:
+        signals_raw = np.array(data['signals'][0]).T  # to channels x samples
+    else:
+        signals_raw = data['signals'].T  # to channels x samples
+    sample_rate = data['sample_rate']
+
+    if 'ch_names' not in data:
+        ch_names = ['CH%d' % (x + 1) for x in range(signals_raw.shape[0])]
+    else:
+        ch_names = data['ch_names']
+
+    # search for event channel
+    trig_ch = pu.find_event_channel(signals_raw, ch_names)
+
+    ''' TODO: REMOVE
+    # exception
+    if trig_ch is None:
+        logger.warning('Inferred event channel is None.')
+        if interactive:
+            logger.warning('If you are sure everything is alright, press Enter.')
+            input()
+
+    # fix wrong event channel
+    elif trig_ch_guess != trig_ch:
+        logger.warning('Specified event channel (%d) != inferred event channel (%d).' % (trig_ch, trig_ch_guess))
+        if interactive: input('Press Enter to fix. Event channel will be set to %d.' % trig_ch_guess)
+        ch_names.insert(trig_ch_guess, ch_names.pop(trig_ch))
+        trig_ch = trig_ch_guess
+        logger.info('New channel list:')
+        for c in ch_names:
+            logger.info('%s' % c)
+        logger.info('Event channel is now set to %d' % trig_ch)
+    '''
+
+    # move trigger channel to index 0
+    if trig_ch is None:
+        # assuming no event channel exists, add a event channel to index 0 for consistency.
+        logger.warning('No event channel was not found. Adding a blank event channel to index 0.')
+        eventch = np.zeros([1, signals_raw.shape[1]])
+        signals = np.concatenate((eventch, signals_raw), axis=0)
+        num_eeg_channels = signals_raw.shape[0] # data['channels'] is not reliable any more
+        trig_ch = 0
+        ch_names = ['TRIGGER'] + ['CH%d' % (x + 1) for x in range(num_eeg_channels)]
+    elif trig_ch == 0:
+        signals = signals_raw
+        num_eeg_channels = data['channels'] - 1
+    else:
+        # move event channel to 0
+        logger.info('Moving event channel %d to 0.' % trig_ch)
+        signals = np.concatenate((signals_raw[[trig_ch]], signals_raw[:trig_ch], signals_raw[trig_ch + 1:]), axis=0)
+        assert signals_raw.shape == signals.shape
+        num_eeg_channels = data['channels'] - 1
+        ch_names.pop(trig_ch)
+        trig_ch = 0
+        ch_names.insert(trig_ch, 'TRIGGER')
+        logger.info('New channel list:')
+        for c in ch_names:
+            logger.info('%s' % c)
+
+    ch_info = ['stim'] + ['eeg'] * num_eeg_channels
+    info = mne.create_info(ch_names, sample_rate, ch_info)
+
+    # create Raw object
+    raw = mne.io.RawArray(signals, info)
+    raw._times = data['timestamps'] # seems to have no effect
+
+    if external_event is not None:
+        raw._data[0] = 0  # erase current events
+        events_index = event_timestamps_to_indices(filename, external_event, offset)
+        if len(events_index) == 0:
+            logger.warning('No events were found in the event file')
+        else:
+            logger.info('Found %d events' % len(events_index))
+            raw.add_events(events_index, stim_channel='TRIGGER')
+
+    qc.make_dirs(outdir)
+    fiffile = outdir + fname + '.fif'
+
+    raw.save(fiffile, verbose=False, overwrite=overwrite, fmt=precision)
+    logger.info('Saved to %s' % fiffile)
+
+    saveChannels2txt(outdir, ch_names)
+
+    return True
+
+
+def eeg2fif(filename, interactive=False, outdir=None):
+    """
+    Brain Products EEG format
+    """
+    fdir, fname, fext = qc.parse_path_list(filename)
+    if outdir is None:
+        outdir = fdir
+    elif outdir[-1] != '/':
+        outdir += '/'
+
+    eegfile = fdir + fname + '.eeg'
+    matfile = fdir + fname + '.mat'
+    markerfile = fdir + fname + '.vmrk'
+    fiffile = outdir + fname + '.fif'
+
+    # convert to mat using MATLAB
+    if not os.path.exists(matfile):
+        logger.info('Converting input to mat file')
+        run = "[sig,header]=sload('%s'); save('%s','sig','header');" % (eegfile, matfile)
+        qc.matlab(run)
+        if not os.path.exists(matfile):
+            logger.error('mat file convertion error.')
+            sys.exit()
+    else:
+        logger.warning('MAT file already exists. Skipping conversion.')
+
+    # extract events
+    events = []
+    for l in open(markerfile):
+        if 'Stimulus,S' in l:
+            # event, sample_index= l.split('  ')[-1].split(',')[:2]
+            data = l.split(',')[1:3]
+            event = int(data[0][1:])  # ignore 'S'
+            sample_index = int(data[1])
+            events.append([sample_index, 0, event])
+
+    # load data and create fif header
+    mat = scipy.io.loadmat(matfile)
+    # headers= mat['header']
+    sample_rate = int(mat['header']['SampleRate'])
+    signals = mat['sig'].T  # channels x samples
+    nch, t_len = signals.shape
+    ch_names = ['TRIGGER'] + ['CH%d' % (x + 1) for x in range(nch)]
+    ch_info = ['stim'] + ['eeg'] * (nch)
+    info = mne.create_info(ch_names, sample_rate, ch_info, montage='standard_1005')
+
+    # add event channel
+    eventch = np.zeros([1, signals.shape[1]])
+    signals = np.concatenate((eventch, signals), axis=0)
+
+    # create Raw object
+    raw = mne.io.RawArray(signals, info)
+
+    # add events
+    raw.add_events(events, 'TRIGGER')
+
+    # save and close
+    raw.save(fiffile, verbose=False, overwrite=True, fmt='double')
+    logger.info('Saved to %s' % fiffile)
+
+    saveChannels2txt(outdir, ch_names)
+
+
+def gdf2fif(filename, interactive=False, outdir=None, channel_file=None):
+    """
+    g.Tec gdf format
+
+    Assumes the last channel is event channel.
+    """
+    fdir, fname, fext = qc.parse_path_list(filename)
+    if outdir is None:
+        outdir = fdir
+    elif outdir[-1] != '/':
+        outdir += '/'
+
+    fiffile = outdir + fname + '.fif'
+    matfile = fdir + fname + '.mat'
+
+    convert2mat(fdir + fname + '.gdf', matfile)
+    mat = scipy.io.loadmat(matfile)
+    os.remove(matfile)
+    sample_rate = int(mat['header']['SampleRate'])
+    nch = mat['sig'].shape[1]
+
+    # read events from header
+    evtype = mat['header']['EVENT'][0][0][0]['TYP'][0]
+    evpos = mat['header']['EVENT'][0][0][0]['POS'][0]
+    events = []
+    for e in range(evtype.shape[0]):
+        label = int(evtype[e])
+        events.append([int(evpos[e][0]), 0, label])
+
+    signals_raw = mat['sig'].T  # -> channels x samples
+
+    ''' it seems they fixed the bug now
+    # Note: Biosig's sload() sometimes returns bogus event values so we use the following for events
+    raw= mne.io.read_raw_edf(filename, preload=True)
+    events= mne.find_events(raw, stim_channel='TRIGGER', shortest_event=1, consecutive=True)
+    #signals_raw[-1][:]= raw._data[-1][:] # overwrite with the correct event values
+    '''
+
+    # Move the event channel to 0 (for consistency)
+    signals = np.concatenate((signals_raw[-1, :].reshape(1, -1), signals_raw[:-1, :]))
+    signals[0] *= 0  # init the event channel
+
+    # Note: gdf might have a software event channel
+    if channel_file is None:
+        ch_names = ['TRIGGER'] + ['CH%d' % x for x in range(1, nch)]
+    else:
+        ch_names_raw = []
+        for l in open(channel_file):
+            ch_names_raw.append(l.strip())
+        if ch_names_raw[-1] != 'TRIGGER':
+            input(
+                'Warning: Trigger channel is assumed to be the last channel. Press Ctrl+C if this is not the case.')
+        ch_names = ['TRIGGER'] + ch_names_raw[:-1]
+    ch_info = ['stim'] + ['eeg'] * (nch - 1)
+    info = mne.create_info(ch_names, sample_rate, ch_info)
+
+    # create Raw object
+    raw = mne.io.RawArray(signals, info)
+
+    # add events
+    raw.add_events(events, 'TRIGGER')
+
+    # save and close
+    raw.save(fiffile, verbose=False, overwrite=True, fmt='double')
+    logger.info('Saved to %s' % fiffile)
+
+    saveChannels2txt(outdir, ch_names)
+
+
+def bdf2fif(filename, interactive=False, outdir=None):
+    """
+    EDF or BioSemi BDF format
+    """
+    # convert to mat using MATLAB (MNE's edf reader has an offset bug)
+    fdir, fname, fext = qc.parse_path_list(filename)
+    if outdir is None:
+        outdir = fdir
+    elif outdir[-1] != '/':
+        outdir += '/'
+
+    fiffile = outdir + fname + '.fif'
+    raw = mne.io.read_raw_edf(filename, preload=True)
+
+    # process event channel
+    if raw.info['chs'][-1]['ch_name'] != 'STI 014':
+        logger.error("The last channel (%s) doesn't seem to be an event channel. Entering debugging mode." % raw.info['chs'][-1]['ch_name'])
+        pdb.set_trace()
+    raw.info['chs'][-1]['ch_name'] = 'TRIGGER'
+    events = mne.find_events(raw, stim_channel='TRIGGER', shortest_event=1, uint_cast=True, consecutive=True)
+    events[:, 2] -= events[:, 1]  # set offset to 0
+    events[:, 1] = 0
+    # move the event channel to index 0 (for consistency)
+    raw._data = np.concatenate((raw._data[-1, :].reshape(1, -1), raw._data[:-1, :]))
+    raw._data[0] *= 0  # init the event channel
+    raw.info['chs'] = [raw.info['chs'][-1]] + raw.info['chs'][:-1]
+
+    # add events
+    raw.add_events(events, 'TRIGGER')
+
+    # save and close
+    raw.save(fiffile, verbose=False, overwrite=True, fmt='double')
+    logger.info('Saved to %s' % fiffile)
+
+    saveChannels2txt(outdir, ch_names)
+
+
+def bdf2fif_matlab(filename, interactive=False, outdir=None):
+    """
+    BioSemi bdf reader using BioSig toolbox of MATLAB.
+    """
+    # convert to mat using MATLAB (MNE's edf reader has an offset bug)
+    fdir, fname, fext = qc.parse_path_list(filename)
+    if outdir is None:
+        outdir = fdir
+    elif outdir[-1] != '/':
+        outdir += '/'
+
+    fiffile = outdir + fname + '.fif'
+    matfile = outdir + fname + '.mat'
+
+    if not os.path.exists(matfile):
+        logger.info('Converting input to mat file')
+        run = "[sig,header]=sload('%s'); save('%s','sig','header');" % (filename, matfile)
+        qc.matlab(run)
+        if not os.path.exists(matfile):
+            logger.error('mat file convertion error.')
+            sys.exit()
+
+    mat = scipy.io.loadmat(matfile)
+    os.remove(matfile)
+    sample_rate = int(mat['header']['SampleRate'])
+    nch = mat['sig'].shape[1]
+
+    # assume Biosemi always has the same number of channels
+    if nch == 73:
+        ch_names = CAP['BIOSEMI_64']
+        extra_ch = nch - len(CAP['BIOSEMI_64_INFO'])
+        extra_names = []
+        for ch in range(extra_ch):
+            extra_names.append('EXTRA%d' % ch)
+        ch_names = ch_names + extra_names
+        ch_info = CAP['BIOSEMI_64_INFO'] + ['misc'] * extra_ch
+    else:
+        logger.warning('Unrecognized number of channels (%d)' % nch)
+        logger.warning('The last channel will be assumed to be trigger. Press Enter to continue, or Ctrl+C to break.')
+        if interactive:
+            input()
+
+        # Set the trigger to be channel 0 because later we will move it to channel 0.
+        ch_names = ['TRIGGER'] + ['CH%d' % (x + 1) for x in range(nch - 1)]
+        ch_info = ['stim'] + ['eeg'] * (nch - 1)
+
+    signals_raw = mat['sig'].T  # -> channels x samples
+
+    # Note: Biosig's sload() sometimes returns bogus event values so we use the following for events
+    bdf = mne.io.read_raw_edf(filename, preload=True)
+    events = mne.find_events(bdf, stim_channel='TRIGGER', shortest_event=1, consecutive=True)
+    # signals_raw[-1][:]= bdf._data[-1][:] # overwrite with the correct event values
+
+    # Move the event channel to 0 (for consistency)
+    signals = np.concatenate((signals_raw[-1, :].reshape(1, -1), signals_raw[:-1, :]))
+    signals[0] *= 0  # init the event channel
+
+    info = mne.create_info(ch_names, sample_rate, ch_info, montage='standard_1005')
+
+    # create Raw object
+    raw = mne.io.RawArray(signals, info)
+
+    # add events
+    raw.add_events(events, 'TRIGGER')
+
+    # save and close
+    raw.save(fiffile, verbose=False, overwrite=True, fmt='double')
+    logger.info('Saved to %s' % fiffile)
+
+    saveChannels2txt(outdir, ch_names)
+
+
+def xdf2fif(filename, interactive=False, outdir=None):
+    """
+    Convert XDF format
+    """
+    from pyxdf import pyxdf
+    pyxdf.logger.setLevel('WARNING')
+
+    fdir, fname, fext = qc.parse_path_list(filename)
+    if outdir is None:
+        outdir = fdir
+    elif outdir[-1] != '/':
+        outdir += '/'
+
+    fiffile = outdir + fname + '.fif'
+
+    # channel x times
+    data = pyxdf.load_xdf(filename)
+    raw_data = data[0][0]['time_series'].T
+    if np.max(raw_data[:-1]) < 1:
+        logger.info('Assuming the signal unit is volate (V). Converting to uV')
+        raw_data[:-1] *= 10**6
+
+    signals = np.concatenate((raw_data[-1, :].reshape(1, -1), raw_data[:-1, :]))
+
+    sample_rate = int(data[0][0]['info']['nominal_srate'][0])
+    # TODO: check the event channel index and move to the 0-th index
+    # in LSL, usually the name is TRIG or STI 014.
+    ch_names = []
+    for ch in data[0][0]['info']['desc'][0]['channels'][0]['channel']:
+        ch_names.append(ch['label'][0])
+    trig_ch_guess = pu.find_event_channel(signals, ch_names)
+    if trig_ch_guess is None:
+        trig_ch_guess = 0
+    ch_names =['TRIGGER'] + ch_names[:trig_ch_guess] + ch_names[trig_ch_guess+1:]
+    ch_info = ['stim'] + ['eeg'] * (len(ch_names)-1)
+
+    # fif header creation
+    info = mne.create_info(ch_names, sample_rate, ch_info)
+    raw = mne.io.RawArray(signals, info)
+    #raw.add_events(events_index, stim_channel='TRIGGER')
+
+    # save and close
+    raw.save(fiffile, verbose=False, overwrite=True, fmt='double')
+    logger.info('Saved to %s' % fiffile)
+
+    saveChannels2txt(outdir, ch_names)
+
+
+
+def any2fif(filename, interactive=False, outdir=None, channel_file=None):
+    """
+    Generic file format converter
+    """
+    p = qc.parse_path(filename)
+    if outdir is not None:
+        qc.make_dirs(outdir)
+
+    if p.ext == 'pcl':
+        eve_file = '%s/%s.txt' % (p.dir, p.name.replace('raw', 'eve'))
+        if os.path.exists(eve_file):
+            logger.info('Adding events from %s' % eve_file)
+            eveoffset_file = qc.parse_path(eve_file).name + '-offset.txt'
+            if os.path.exists(eveoffset_file):
+                offset = float(open(eveoffset_file).readline().split('Offset: ')[-1].strip())
+                logger.info('Adding event offset %.1f from %s' % (offset, eve_file))
+        else:
+            eve_file = None
+        pcl2fif(filename, interactive=interactive, outdir=outdir, external_event=eve_file, offset=offset)
+    elif p.ext == 'eeg':
+        eeg2fif(filename, interactive=interactive, outdir=outdir)
+    elif p.ext in ['edf', 'bdf']:
+        bdf2fif(filename, interactive=interactive, outdir=outdir)
+    elif p.ext == 'gdf':
+        gdf2fif(filename, interactive=interactive, outdir=outdir, channel_file=channel_file)
+    elif p.ext == 'xdf':
+        xdf2fif(filename, interactive=interactive, outdir=outdir)
+    else:  # unknown format
+        logger.error('Ignored unrecognized file extension %s. It should be [.pcl | .eeg | .gdf | .bdf]' % p.ext)
+
+
+def saveChannels2txt(outdir, ch_names):
+    """
+    Save the channels list to a txt file for the GUI
+    """
+
+    filename = outdir + "channelsList.txt"
+    config = Path(filename)
+
+    if config.is_file() is False:
+        file = open(filename, "w")
+        for x in range(len(ch_names)):
+            file.write(ch_names[x] + "\n")
+        file.close()
+
+
+def main():
+    """
+    Invoked from the console
+    """
+    if len(sys.argv) == 1:
+        print('Usage: %s data_dir [channel_file]' % os.path.basename(__file__))
+        return
+
+    input_dir = sys.argv[1]
+    if len(sys.argv) > 2:
+        channel_file = sys.argv[2]
+    else:
+        channel_file = None
+
+    count = 0
+    for f in qc.get_file_list(input_dir, fullpath=True, recursive=True):
+        p = qc.parse_path(f)
+        outdir = p.dir + '/fif/'
+        if p.ext in ['pcl', 'bdf', 'edf', 'gdf', 'eeg', 'xdf']:
+            logger.info('Converting %s' % f)
+            any2fif(f, interactive=True, outdir=outdir, channel_file=channel_file)
+            count += 1
+
+    logger.info('%d files converted.' % count)
+
+if __name__ == '__main__':
+    main()
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/epochs2mat.py` & `neurodecode-2.0.5/neurodecode/utils/epochs2mat.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-from __future__ import print_function, division
-
-"""
-Export epochs from fif files to mat files
-
-if MERGE_EPOCHS is True, merge epochs from all raw files and export to a
-single mat file. Otherwise, export epochs of each raw file individually.
-
-Author: Kyuhwa Lee
-Swiss Federal Institute of Technology (EPFL)
-
-"""
-
-import mne
-import scipy.io
-import numpy as np
-import neurodecode.utils.pycnbi_utils as pu
-import neurodecode.utils.q_common as qc
-from neurodecode import logger
-
-mne.set_log_level('ERROR')
-
-def save_mat(raw, events, picks, event_id, tmin, tmax, matfile):
-    sfreq = raw.info['sfreq']
-
-    # pick channels
-    if picks is None:
-        picks = mne.pick_types(raw.info, meg=False, eeg=True, stim=False,
-            eog=False, exclude='bads')
-    elif type(picks[0]) == str:
-        picks = [raw.ch_names.index(c) for c in picks]
-    else:
-        assert type(picks[0]) is int
-        picks = picks
-
-    # epoching
-    epochs = mne.Epochs(raw, events, event_id, tmin=tmin, tmax=tmax, proj=False,
-        picks=picks, baseline=(tmin, tmax), preload=True)
-
-    # save into mat format
-    data = dict(tmin=tmin, tmax=tmax, sfreq=epochs.info['sfreq'],
-        labels = list(event_id.keys()), ch_names = [raw.ch_names[ch] for ch in picks])
-    for eve in event_id:
-        data['epochs_%s' % eve] = epochs[eve].get_data()
-    scipy.io.savemat(matfile, data)
-
-def epochs2mat(data_dir, channel_picks, event_id, tmin, tmax, merge_epochs=False, spfilter=None, spchannels=None):
-    if merge_epochs:
-        # load all raw files in the directory and merge epochs
-        fiflist = []
-        for data_file in qc.get_file_list(data_dir, fullpath=True):
-            if data_file[-4:] != '.fif':
-                continue
-            fiflist.append(data_file)
-        raw, events = pu.load_multi(fiflist, spfilter=spfilter, spchannels=spchannels)
-        matfile = data_dir + '/epochs_all.mat'
-        save_mat(raw, events, channel_picks, event_id, tmin, tmax, matfile)
-    else:
-        # process individual raw file separately
-        for data_file in qc.get_file_list(data_dir, fullpath=True):
-            if data_file[-4:] != '.fif':
-                continue
-            [base, fname, fext] = qc.parse_path_list(data_file)
-            matfile = '%s/%s-epochs.mat' % (base, fname)
-            raw, events = pu.load_raw(data_file)
-            save_mat(raw, events, channel_picks, event_id, tmin, tmax, matfile)
-
-    logger.info('Exported to %s' % matfile)
-
-# sample code
-if __name__ == '__main__':
-    data_dir = r'd:\data\mi\z2\lr'
-    channel_picks = ['F3','F4','C3','Cz','C4','P3','Pz','P4']
-    event_id = {'LEFT_GO':11, 'RIGHT_GO':9}
-    tmin = -1.0
-    tmax = 3.0
-    merge_epochs = True
-    spfilter = 'car'
-    epochs2mat(data_dir, channel_picks, event_id, tmin, tmax, merge_epochs, spfilter=spfilter)
+from __future__ import print_function, division
+
+"""
+Export epochs from fif files to mat files
+
+if MERGE_EPOCHS is True, merge epochs from all raw files and export to a
+single mat file. Otherwise, export epochs of each raw file individually.
+
+Author: Kyuhwa Lee
+Swiss Federal Institute of Technology (EPFL)
+
+"""
+
+import mne
+import scipy.io
+import numpy as np
+import neurodecode.utils.pycnbi_utils as pu
+import neurodecode.utils.q_common as qc
+from neurodecode import logger
+
+mne.set_log_level('ERROR')
+
+def save_mat(raw, events, picks, event_id, tmin, tmax, matfile):
+    sfreq = raw.info['sfreq']
+
+    # pick channels
+    if picks is None:
+        picks = mne.pick_types(raw.info, meg=False, eeg=True, stim=False,
+            eog=False, exclude='bads')
+    elif type(picks[0]) == str:
+        picks = [raw.ch_names.index(c) for c in picks]
+    else:
+        assert type(picks[0]) is int
+        picks = picks
+
+    # epoching
+    epochs = mne.Epochs(raw, events, event_id, tmin=tmin, tmax=tmax, proj=False,
+        picks=picks, baseline=(tmin, tmax), preload=True)
+
+    # save into mat format
+    data = dict(tmin=tmin, tmax=tmax, sfreq=epochs.info['sfreq'],
+        labels = list(event_id.keys()), ch_names = [raw.ch_names[ch] for ch in picks])
+    for eve in event_id:
+        data['epochs_%s' % eve] = epochs[eve].get_data()
+    scipy.io.savemat(matfile, data)
+
+def epochs2mat(data_dir, channel_picks, event_id, tmin, tmax, merge_epochs=False, spfilter=None, spchannels=None):
+    if merge_epochs:
+        # load all raw files in the directory and merge epochs
+        fiflist = []
+        for data_file in qc.get_file_list(data_dir, fullpath=True):
+            if data_file[-4:] != '.fif':
+                continue
+            fiflist.append(data_file)
+        raw, events = pu.load_multi(fiflist, spfilter=spfilter, spchannels=spchannels)
+        matfile = data_dir + '/epochs_all.mat'
+        save_mat(raw, events, channel_picks, event_id, tmin, tmax, matfile)
+    else:
+        # process individual raw file separately
+        for data_file in qc.get_file_list(data_dir, fullpath=True):
+            if data_file[-4:] != '.fif':
+                continue
+            [base, fname, fext] = qc.parse_path_list(data_file)
+            matfile = '%s/%s-epochs.mat' % (base, fname)
+            raw, events = pu.load_raw(data_file)
+            save_mat(raw, events, channel_picks, event_id, tmin, tmax, matfile)
+
+    logger.info('Exported to %s' % matfile)
+
+# sample code
+if __name__ == '__main__':
+    data_dir = r'd:\data\mi\z2\lr'
+    channel_picks = ['F3','F4','C3','Cz','C4','P3','Pz','P4']
+    event_id = {'LEFT_GO':11, 'RIGHT_GO':9}
+    tmin = -1.0
+    tmax = 3.0
+    merge_epochs = True
+    spfilter = 'car'
+    epochs2mat(data_dir, channel_picks, event_id, tmin, tmax, merge_epochs, spfilter=spfilter)
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/epochs2txt.py` & `neurodecode-2.0.5/neurodecode/utils/epochs2txt.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-from __future__ import print_function, division
-
-"""
-Export epochs to one text file per epoch
-File name  : EVENT-N.txt (N=0,1,2,...)
-Data format: times x channels, space-separated floats
-
-Kyuhwa Lee
-Swiss Federal Institute of Technology (EPFL)
-
-"""
-
-DATA_PATH = r'D:\data\BCI_COURSE\raw_corrected\Session2\rx7'
-EXCLUDES = ['M1', 'M2', 'EOG']
-REF_CH_OLD = None  # original channel used as a reference
-REF_CH_NEW = None  # re-reference to the average of these channels
-CHANNEL_PICKS = None # list of integers or list of strings
-MULTIPLIER = 1 # unit multiplier
-EPOCHS = {'stand':240, 'sit':238}
-TMIN = 0.0
-TMAX = 2.0
-
-
-import neurodecode.utils.pycnbi_utils as pu
-import neurodecode.utils.q_common as qc
-import scipy.io
-import mne
-import numpy as np
-import trainer
-from multiprocessing import cpu_count
-from neurodecode import logger
-
-mne.set_log_level('ERROR')
-
-if __name__ == '__main__':
-    rawlist = []
-    for f in qc.get_file_list(DATA_PATH, fullpath=True):
-        if f[-4:] == '.fif':
-            rawlist.append(f)
-    if len(rawlist) == 0:
-        raise RuntimeError('No fif files found in the path.')
-
-    # make output directory
-    out_path = DATA_PATH + '/epochs'
-    qc.make_dirs(out_path)
-
-    # load data
-    raw, events = pu.load_multi(rawlist, multiplier=MULTIPLIER)
-    raw.pick_types(meg=False, eeg=True, stim=False)
-    sfreq = raw.info['sfreq']
-    if REF_CH_NEW is not None:
-        pu.rereference(raw, REF_CH_NEW, REF_CH_OLD)
-
-    # pick channels
-    if CHANNEL_PICKS is None:
-        picks = [raw.ch_names.index(c) for c in raw.ch_names if c not in EXCLUDES]
-    elif type(CHANNEL_PICKS[0]) == str:
-        picks = [raw.ch_names.index(c) for c in CHANNEL_PICKS]
-    else:
-        assert type(CHANNEL_PICKS[0]) is int
-        picks = CHANNEL_PICKS
-
-    # do epoching
-    for epname, epval in EPOCHS.items():
-        epochs = mne.Epochs(raw, events, dict(epname=epval), tmin=TMIN, tmax=TMAX,
-                            proj=False, picks=picks, baseline=None, preload=True)
-        data = epochs.get_data()  # epochs x channels x times
-        for i, ep_data in enumerate(data):
-            fout = '%s/%s-%d.txt' % (out_path, epname, i + 1)
-            with open(fout, 'w') as f:
-                for t in range(ep_data.shape[1]):
-                    f.write(qc.list2string(ep_data[:, t], '%.6f') + '\n')
-            logger.info('Exported %s' % fout)
+from __future__ import print_function, division
+
+"""
+Export epochs to one text file per epoch
+File name  : EVENT-N.txt (N=0,1,2,...)
+Data format: times x channels, space-separated floats
+
+Kyuhwa Lee
+Swiss Federal Institute of Technology (EPFL)
+
+"""
+
+DATA_PATH = r'D:\data\BCI_COURSE\raw_corrected\Session2\rx7'
+EXCLUDES = ['M1', 'M2', 'EOG']
+REF_CH_OLD = None  # original channel used as a reference
+REF_CH_NEW = None  # re-reference to the average of these channels
+CHANNEL_PICKS = None # list of integers or list of strings
+MULTIPLIER = 1 # unit multiplier
+EPOCHS = {'stand':240, 'sit':238}
+TMIN = 0.0
+TMAX = 2.0
+
+
+import neurodecode.utils.pycnbi_utils as pu
+import neurodecode.utils.q_common as qc
+import scipy.io
+import mne
+import numpy as np
+import trainer
+from multiprocessing import cpu_count
+from neurodecode import logger
+
+mne.set_log_level('ERROR')
+
+if __name__ == '__main__':
+    rawlist = []
+    for f in qc.get_file_list(DATA_PATH, fullpath=True):
+        if f[-4:] == '.fif':
+            rawlist.append(f)
+    if len(rawlist) == 0:
+        raise RuntimeError('No fif files found in the path.')
+
+    # make output directory
+    out_path = DATA_PATH + '/epochs'
+    qc.make_dirs(out_path)
+
+    # load data
+    raw, events = pu.load_multi(rawlist, multiplier=MULTIPLIER)
+    raw.pick_types(meg=False, eeg=True, stim=False)
+    sfreq = raw.info['sfreq']
+    if REF_CH_NEW is not None:
+        pu.rereference(raw, REF_CH_NEW, REF_CH_OLD)
+
+    # pick channels
+    if CHANNEL_PICKS is None:
+        picks = [raw.ch_names.index(c) for c in raw.ch_names if c not in EXCLUDES]
+    elif type(CHANNEL_PICKS[0]) == str:
+        picks = [raw.ch_names.index(c) for c in CHANNEL_PICKS]
+    else:
+        assert type(CHANNEL_PICKS[0]) is int
+        picks = CHANNEL_PICKS
+
+    # do epoching
+    for epname, epval in EPOCHS.items():
+        epochs = mne.Epochs(raw, events, dict(epname=epval), tmin=TMIN, tmax=TMAX,
+                            proj=False, picks=picks, baseline=None, preload=True)
+        data = epochs.get_data()  # epochs x channels x times
+        for i, ep_data in enumerate(data):
+            fout = '%s/%s-%d.txt' % (out_path, epname, i + 1)
+            with open(fout, 'w') as f:
+                for t in range(ep_data.shape[1]):
+                    f.write(qc.list2string(ep_data[:, t], '%.6f') + '\n')
+            logger.info('Exported %s' % fout)
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/fif2mat.py` & `neurodecode-2.0.5/neurodecode/utils/fif2mat.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from __future__ import print_function, division
-
-"""
-Export fif data into mat files.
-
-"""
-
-import os
-import sys
-import mne
-import scipy.io
-import neurodecode.utils.q_common as qc
-import neurodecode.utils.pycnbi_utils as pu
-from neurodecode import logger
-
-def fif2mat_file(fif_file, out_dir='./'):
-    raw, events = pu.load_raw(fif_file)
-    events[:,0] += 1 # MATLAB uses 1-based indexing
-    sfreq = raw.info['sfreq']
-    data = dict(signals=raw._data, events=events, sfreq=sfreq, ch_names=raw.ch_names)
-    fname = qc.parse_path(fif_file).name
-    matfile = '%s/%s.mat' % (out_dir, fname)
-    scipy.io.savemat(matfile, data)
-    logger.info('Exported to %s' % matfile)
-
-def fif2mat(input_path):
-    if os.path.isdir(input_path):
-        out_dir = '%s/mat_files' % input_path
-        qc.make_dirs(out_dir)
-        num_processed = 0
-        for rawfile in qc.get_file_list(input_path, fullpath=True):
-            if rawfile[-4:] != '.fif':
-                continue
-            fif2mat_file(rawfile, out_dir)
-            num_processed += 1
-        if num_processed == 0:
-            logger.warning('No fif files found in the path.')
-    elif os.path.isfile(input_path):
-        out_dir = '%s/mat_files' % qc.parse_path(input_path).dir
-        qc.make_dirs(out_dir)
-        fif2mat_file(input_path, out_dir)
-    else:
-        raise ValueError('Neither directory nor file: %s' % input_path)
-    logger.info('Finished.')
-
-def main():
-    """
-    Invoked from console
-    """
-    if len(sys.argv) == 1:
-        print('Usage: %s fif_dir' % os.path.basename(__file__))
-        return
-
-    fif_dir = sys.argv[1]
-    fif2mat(fif_dir)
-
-if __name__ == '__main__':
-    main()
+from __future__ import print_function, division
+
+"""
+Export fif data into mat files.
+
+"""
+
+import os
+import sys
+import mne
+import scipy.io
+import neurodecode.utils.q_common as qc
+import neurodecode.utils.pycnbi_utils as pu
+from neurodecode import logger
+
+def fif2mat_file(fif_file, out_dir='./'):
+    raw, events = pu.load_raw(fif_file)
+    events[:,0] += 1 # MATLAB uses 1-based indexing
+    sfreq = raw.info['sfreq']
+    data = dict(signals=raw._data, events=events, sfreq=sfreq, ch_names=raw.ch_names)
+    fname = qc.parse_path(fif_file).name
+    matfile = '%s/%s.mat' % (out_dir, fname)
+    scipy.io.savemat(matfile, data)
+    logger.info('Exported to %s' % matfile)
+
+def fif2mat(input_path):
+    if os.path.isdir(input_path):
+        out_dir = '%s/mat_files' % input_path
+        qc.make_dirs(out_dir)
+        num_processed = 0
+        for rawfile in qc.get_file_list(input_path, fullpath=True):
+            if rawfile[-4:] != '.fif':
+                continue
+            fif2mat_file(rawfile, out_dir)
+            num_processed += 1
+        if num_processed == 0:
+            logger.warning('No fif files found in the path.')
+    elif os.path.isfile(input_path):
+        out_dir = '%s/mat_files' % qc.parse_path(input_path).dir
+        qc.make_dirs(out_dir)
+        fif2mat_file(input_path, out_dir)
+    else:
+        raise ValueError('Neither directory nor file: %s' % input_path)
+    logger.info('Finished.')
+
+def main():
+    """
+    Invoked from console
+    """
+    if len(sys.argv) == 1:
+        print('Usage: %s fif_dir' % os.path.basename(__file__))
+        return
+
+    fif_dir = sys.argv[1]
+    fif2mat(fif_dir)
+
+if __name__ == '__main__':
+    main()
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/fif_resample.py` & `neurodecode-2.0.5/neurodecode/utils/fif_resample.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from __future__ import print_function, division
-
-"""
-Change the sampling frequency of fif files.
-Appropriate low-pass filter is applied before resampling.
-
-Kyuhwa Lee
-Swiss Federal Institute of Technology (EPFL)
-
-"""
-
-import os
-import sys
-import neurodecode.utils.q_common as qc
-import neurodecode.utils.pycnbi_utils as pu
-from builtins import input
-from neurodecode import logger
-
-def fif_resample(fif_dir, sfreq_target):
-    out_dir = fif_dir + '/fif_resample%d' % sfreq_target
-    qc.make_dirs(out_dir)
-    for f in qc.get_file_list(fif_dir):
-        pp = qc.parse_path(f)
-        if pp.ext != 'fif':
-            continue
-        logger.info('Resampling %s' % f)
-        raw, events = pu.load_raw(f)
-        raw.resample(sfreq_target)
-        fif_out = '%s/%s.fif' % (out_dir, pp.name)
-        raw.save(fif_out)
-        logger.info('Exported to %s' % fif_out)
-
-# for batch scripts
-def batch_run(fif_dir=None, sfreq_target=None):
-    if not fif_dir:
-        fif_dir = input('Data file path? ')
-    if not sfreq_target:
-        sfreq_target = input('Target sampling frequency? ')
-    sfreq_target = float(sfreq_target)
-    fif_resample(fif_dir, sfreq_target)
-
-def main():
-    """
-    Invoked from console
-    """
-    if len(sys.argv) < 3:
-        print('Usage: %s fif_dir target_sfreq' % os.path.basename(__file__))
-        return
-
-    fif_dir = sys.argv[1]
-    sfreq_target = float(sys.argv[2])
-    fif_resample(fif_dir, sfreq_target)
-    logger.info('Finished.')
-
-if __name__ == '__main__':
-    main()
+from __future__ import print_function, division
+
+"""
+Change the sampling frequency of fif files.
+Appropriate low-pass filter is applied before resampling.
+
+Kyuhwa Lee
+Swiss Federal Institute of Technology (EPFL)
+
+"""
+
+import os
+import sys
+import neurodecode.utils.q_common as qc
+import neurodecode.utils.pycnbi_utils as pu
+from builtins import input
+from neurodecode import logger
+
+def fif_resample(fif_dir, sfreq_target):
+    out_dir = fif_dir + '/fif_resample%d' % sfreq_target
+    qc.make_dirs(out_dir)
+    for f in qc.get_file_list(fif_dir):
+        pp = qc.parse_path(f)
+        if pp.ext != 'fif':
+            continue
+        logger.info('Resampling %s' % f)
+        raw, events = pu.load_raw(f)
+        raw.resample(sfreq_target)
+        fif_out = '%s/%s.fif' % (out_dir, pp.name)
+        raw.save(fif_out)
+        logger.info('Exported to %s' % fif_out)
+
+# for batch scripts
+def batch_run(fif_dir=None, sfreq_target=None):
+    if not fif_dir:
+        fif_dir = input('Data file path? ')
+    if not sfreq_target:
+        sfreq_target = input('Target sampling frequency? ')
+    sfreq_target = float(sfreq_target)
+    fif_resample(fif_dir, sfreq_target)
+
+def main():
+    """
+    Invoked from console
+    """
+    if len(sys.argv) < 3:
+        print('Usage: %s fif_dir target_sfreq' % os.path.basename(__file__))
+        return
+
+    fif_dir = sys.argv[1]
+    sfreq_target = float(sys.argv[2])
+    fif_resample(fif_dir, sfreq_target)
+    logger.info('Finished.')
+
+if __name__ == '__main__':
+    main()
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/fix_channel_names.py` & `neurodecode-2.0.5/neurodecode/utils/fix_channel_names.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from __future__ import print_function, division
-
-import neurodecode.utils.pycnbi_utils as pu
-import neurodecode.utils.q_common as qc
-from neurodecode import logger
-
-def fix_channel_names(fif_dir, new_channel_names):
-    '''
-    Change channel names of fif files in a given directory.
-
-    Input
-    -----
-    @fif_dir: path to fif files
-    @new_channel_names: list of new channel names
-
-    Output
-    ------
-    Modified fif files are saved in fif_dir/corrected/
-
-    Kyuhwa Lee, 2019.
-    '''
-
-    flist = []
-    for f in qc.get_file_list(fif_dir):
-        if qc.parse_path(f).ext == 'fif':
-            flist.append(f)
-
-    if len(flist) > 0:
-        qc.make_dirs('%s/corrected' % fif_dir)
-        for f in qc.get_file_list(fif_dir):
-            logger.info('\nLoading %s' % f)
-            p = qc.parse_path(f)
-            if p.ext == 'fif':
-                raw, eve = pu.load_raw(f)
-                if len(raw.ch_names) != len(new_channel_names):
-                    raise RuntimeError('The number of new channels do not matach that of fif file.')
-                raw.info['ch_names'] = new_channel_names
-                for ch, new_ch in zip(raw.info['chs'], new_channel_names):
-                    ch['ch_name'] = new_ch
-                out_fif = '%s/corrected/%s.fif' % (p.dir, p.name)
-                logger.info('Exporting to %s' % out_fif)
-                raw.save(out_fif)
-    else:
-        logger.warning('No fif files found in %s' % fif_dir)
+from __future__ import print_function, division
+
+import neurodecode.utils.pycnbi_utils as pu
+import neurodecode.utils.q_common as qc
+from neurodecode import logger
+
+def fix_channel_names(fif_dir, new_channel_names):
+    '''
+    Change channel names of fif files in a given directory.
+
+    Input
+    -----
+    @fif_dir: path to fif files
+    @new_channel_names: list of new channel names
+
+    Output
+    ------
+    Modified fif files are saved in fif_dir/corrected/
+
+    Kyuhwa Lee, 2019.
+    '''
+
+    flist = []
+    for f in qc.get_file_list(fif_dir):
+        if qc.parse_path(f).ext == 'fif':
+            flist.append(f)
+
+    if len(flist) > 0:
+        qc.make_dirs('%s/corrected' % fif_dir)
+        for f in qc.get_file_list(fif_dir):
+            logger.info('\nLoading %s' % f)
+            p = qc.parse_path(f)
+            if p.ext == 'fif':
+                raw, eve = pu.load_raw(f)
+                if len(raw.ch_names) != len(new_channel_names):
+                    raise RuntimeError('The number of new channels do not matach that of fif file.')
+                raw.info['ch_names'] = new_channel_names
+                for ch, new_ch in zip(raw.info['chs'], new_channel_names):
+                    ch['ch_name'] = new_ch
+                out_fif = '%s/corrected/%s.fif' % (p.dir, p.name)
+                logger.info('Exporting to %s' % out_fif)
+                raw.save(out_fif)
+    else:
+        logger.warning('No fif files found in %s' % fif_dir)
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/hdf5_to_python.py` & `neurodecode-2.0.5/neurodecode/utils/hdf5_to_python.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-from __future__ import print_function, division
-
-"""
-HDF5 to Python
-
-Convert HDF5 to usable python numpy arrays
-
-Created on Mon Oct 05 10:02:22 2015
-
-@author: Hoang Pham, hoang.pham@epfl.ch
-"""
-
-import h5py
-import scipy.io
-import numpy as np
-import neurodecode.utils.q_common as qc
-import neurodecode.utils.pycnbi_utils as pu
-import xml.etree.ElementTree as XET  # xml parser
-from neurodecode import logger
-
-def hdf5_to_python(data_dir):
-    for rawfile in qc.get_file_list(data_dir, fullpath=True):
-        # rawfile = 'D:/Hoang/My Documents/Python/artifact_data/arm_move2015.09.30_18.48.16.hdf5'
-        # rawfile= 'D:/data/Artifact/eyeroll2015.09.30_18.38.23.hdf5'
-        if rawfile.split('.')[-1] != 'hdf5': continue
-
-        f = h5py.File(rawfile)
-
-        # Reading xml properties
-        """
-        The HDF5 file is structured as folloging
-        - AsynchronData
-        |- AsynchronSignalType: XML
-        |- Time: time index of the trigger data
-        |- TypeID: corresponding trigger data, in a shifted 8-bit pattern (see below for explanation)
-        |- Value: No idea !
-
-        -RawData
-        |- AcquisitionTaskDescription: XML, one node per channel
-        |- DAQDeviceCapabilities: XML, one node per channel
-        |- DAQDeviceDescription: XML, mostly useless
-        |- Sample: Array of channel x time indexes
-        |- SessionDescription: XML, mostly useless
-        |- SubjectDescription: XML, mostly useless
-
-        -SavedFeatures
-        |- NumberOfFeatures: empty ?
-
-        -Version
-        |- Float, useless.
-        """
-        # Read properties from XML
-        tree = XET.fromstring(f['RawData']['AcquisitionTaskDescription'][0])
-        samplingFreq = int(tree.findall('SamplingFrequency')[0].text)  # todo: typecheck ?
-
-        # Decode the trigger channel
-        triggerDataRaw = f['AsynchronData']['TypeID'].value.ravel()  # Get the bit trigger data, flatten it
-        bitoffset = min(triggerDataRaw)  # we're looking for the smallest value
-        triggerDataExp = np.ravel(triggerDataRaw - bitoffset)
-
-        timestamps = f['AsynchronData']['Time'].value.ravel()  # timestamps
-
-        # We're looking at the indexes where there's a change
-        timestampsOffset = np.insert(timestamps, 0, 0)  # offset by one
-        timestamps = np.append(timestamps, 0)  # set to the same length
-        diff_idx = np.ravel(np.nonzero(
-            timestamps - timestampsOffset))  # non-zero element of this are the one we seek,[0] because it's stupid to have a nparray inside a tuple
-
-        # Iterate each bit indexes and convert the 8-bits to decimal values
-        triggerData = np.array([])
-        for index, current in enumerate(diff_idx):
-            tmp = 0
-            if index < len(diff_idx) - 1:  # most elements
-                for i in range(diff_idx[index], diff_idx[index + 1]):
-                    tmp = tmp + 2 ** triggerDataExp[i]
-                triggerData = np.append(triggerData, tmp)
-
-        # Get the index, remove the last element to match the size of triggerData
-        triggerIndexes = timestamps[diff_idx]
-        triggerIndexes = np.delete(triggerIndexes, len(triggerIndexes) - 1)
-
-        # triggerData and triggerIndexes are ready to be inputted to mne.create_event
-
-        logger.info('%s\n%d events found. Event types: %s' % (rawfile, len(triggerIndexes), set(triggerData)))
-        merged = np.vstack((triggerIndexes, triggerData)).T
-        matfile = rawfile.replace('.hdf5', '.mat')
-        matdata = dict(events=merged)
-        scipy.io.savemat(matfile, matdata)
-        logger.info('Data exported to %s' % matfile)
-
-if __name__ == '__main__':
-    data_dir = r'D:\data\TriggerTest'
-    hdf5_to_python(data_dir)
+from __future__ import print_function, division
+
+"""
+HDF5 to Python
+
+Convert HDF5 to usable python numpy arrays
+
+Created on Mon Oct 05 10:02:22 2015
+
+@author: Hoang Pham, hoang.pham@epfl.ch
+"""
+
+import h5py
+import scipy.io
+import numpy as np
+import neurodecode.utils.q_common as qc
+import neurodecode.utils.pycnbi_utils as pu
+import xml.etree.ElementTree as XET  # xml parser
+from neurodecode import logger
+
+def hdf5_to_python(data_dir):
+    for rawfile in qc.get_file_list(data_dir, fullpath=True):
+        # rawfile = 'D:/Hoang/My Documents/Python/artifact_data/arm_move2015.09.30_18.48.16.hdf5'
+        # rawfile= 'D:/data/Artifact/eyeroll2015.09.30_18.38.23.hdf5'
+        if rawfile.split('.')[-1] != 'hdf5': continue
+
+        f = h5py.File(rawfile)
+
+        # Reading xml properties
+        """
+        The HDF5 file is structured as folloging
+        - AsynchronData
+        |- AsynchronSignalType: XML
+        |- Time: time index of the trigger data
+        |- TypeID: corresponding trigger data, in a shifted 8-bit pattern (see below for explanation)
+        |- Value: No idea !
+
+        -RawData
+        |- AcquisitionTaskDescription: XML, one node per channel
+        |- DAQDeviceCapabilities: XML, one node per channel
+        |- DAQDeviceDescription: XML, mostly useless
+        |- Sample: Array of channel x time indexes
+        |- SessionDescription: XML, mostly useless
+        |- SubjectDescription: XML, mostly useless
+
+        -SavedFeatures
+        |- NumberOfFeatures: empty ?
+
+        -Version
+        |- Float, useless.
+        """
+        # Read properties from XML
+        tree = XET.fromstring(f['RawData']['AcquisitionTaskDescription'][0])
+        samplingFreq = int(tree.findall('SamplingFrequency')[0].text)  # todo: typecheck ?
+
+        # Decode the trigger channel
+        triggerDataRaw = f['AsynchronData']['TypeID'].value.ravel()  # Get the bit trigger data, flatten it
+        bitoffset = min(triggerDataRaw)  # we're looking for the smallest value
+        triggerDataExp = np.ravel(triggerDataRaw - bitoffset)
+
+        timestamps = f['AsynchronData']['Time'].value.ravel()  # timestamps
+
+        # We're looking at the indexes where there's a change
+        timestampsOffset = np.insert(timestamps, 0, 0)  # offset by one
+        timestamps = np.append(timestamps, 0)  # set to the same length
+        diff_idx = np.ravel(np.nonzero(
+            timestamps - timestampsOffset))  # non-zero element of this are the one we seek,[0] because it's stupid to have a nparray inside a tuple
+
+        # Iterate each bit indexes and convert the 8-bits to decimal values
+        triggerData = np.array([])
+        for index, current in enumerate(diff_idx):
+            tmp = 0
+            if index < len(diff_idx) - 1:  # most elements
+                for i in range(diff_idx[index], diff_idx[index + 1]):
+                    tmp = tmp + 2 ** triggerDataExp[i]
+                triggerData = np.append(triggerData, tmp)
+
+        # Get the index, remove the last element to match the size of triggerData
+        triggerIndexes = timestamps[diff_idx]
+        triggerIndexes = np.delete(triggerIndexes, len(triggerIndexes) - 1)
+
+        # triggerData and triggerIndexes are ready to be inputted to mne.create_event
+
+        logger.info('%s\n%d events found. Event types: %s' % (rawfile, len(triggerIndexes), set(triggerData)))
+        merged = np.vstack((triggerIndexes, triggerData)).T
+        matfile = rawfile.replace('.hdf5', '.mat')
+        matdata = dict(events=merged)
+        scipy.io.savemat(matfile, matdata)
+        logger.info('Data exported to %s' % matfile)
+
+if __name__ == '__main__':
+    data_dir = r'D:\data\TriggerTest'
+    hdf5_to_python(data_dir)
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/images2pkl.py` & `neurodecode-2.0.5/neurodecode/utils/images2pkl.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from __future__ import print_function, division
-
-"""
-Compress feedback images into a single pickle object.
-
-"""
-
-import gzip
-import neurodecode.utils.q_common as qc
-from neurodecode.protocols.viz_images import read_images
-from neurodecode import logger
-try:
-    import cPickle as pickle  # Python 2 (cPickle = C version of pickle)
-except ImportError:
-    import pickle  # Python 3 (C version is the default)
-
-if __name__ == '__main__':
-    LEFT_IMAGE_DIR = r'D:\work\pycnbi_protocols\BodyFeedback\left_behind'
-    RIGHT_IMAGE_DIR = r'D:\work\pycnbi_protocols\BodyFeedback\right_behind'
-    EXPORT_IMAGE_DIR = r'D:\work\pycnbi_protocols\BodyFeedback'
-
-    if pickle.HIGHEST_PROTOCOL >= 4:
-        outfile = '%s/ImageVisuals.pkl' % EXPORT_IMAGE_DIR
-        tm = qc.Timer()
-        logger.info('Reading images from %s' % LEFT_IMAGE_DIR )
-        left_images = read_images(LEFT_IMAGE_DIR)
-        logger.info('Reading images from %s' % RIGHT_IMAGE_DIR)
-        right_images = read_images(RIGHT_IMAGE_DIR)
-        logger.info('Took %.1f s. Start exporting ...' % tm.sec())
-        img_data = {'left_images':left_images, 'right_images':right_images}
-        with gzip.open(outfile, 'wb') as fp:
-            pickle.dump(img_data, fp)
-        logger.info('Exported to %s' % outfile)
-    else:
-        logger.warning('Your Python pickle protocol version is less than 4, which will be slower with loading a pickle object.')
+from __future__ import print_function, division
+
+"""
+Compress feedback images into a single pickle object.
+
+"""
+
+import gzip
+import neurodecode.utils.q_common as qc
+from neurodecode.protocols.viz_images import read_images
+from neurodecode import logger
+try:
+    import cPickle as pickle  # Python 2 (cPickle = C version of pickle)
+except ImportError:
+    import pickle  # Python 3 (C version is the default)
+
+if __name__ == '__main__':
+    LEFT_IMAGE_DIR = r'D:\work\pycnbi_protocols\BodyFeedback\left_behind'
+    RIGHT_IMAGE_DIR = r'D:\work\pycnbi_protocols\BodyFeedback\right_behind'
+    EXPORT_IMAGE_DIR = r'D:\work\pycnbi_protocols\BodyFeedback'
+
+    if pickle.HIGHEST_PROTOCOL >= 4:
+        outfile = '%s/ImageVisuals.pkl' % EXPORT_IMAGE_DIR
+        tm = qc.Timer()
+        logger.info('Reading images from %s' % LEFT_IMAGE_DIR )
+        left_images = read_images(LEFT_IMAGE_DIR)
+        logger.info('Reading images from %s' % RIGHT_IMAGE_DIR)
+        right_images = read_images(RIGHT_IMAGE_DIR)
+        logger.info('Took %.1f s. Start exporting ...' % tm.sec())
+        img_data = {'left_images':left_images, 'right_images':right_images}
+        with gzip.open(outfile, 'wb') as fp:
+            pickle.dump(img_data, fp)
+        logger.info('Exported to %s' % outfile)
+    else:
+        logger.warning('Your Python pickle protocol version is less than 4, which will be slower with loading a pickle object.')
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/list_trigger_pins.py` & `neurodecode-2.0.5/neurodecode/utils/list_trigger_pins.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from __future__ import print_function, division
-
-"""
-List possible trigger values assuming some pins are dead.
-
-For example, current cascading cable for AntNeuro has dead pins of 2,4,7.
-
-Kyuhwa Lee, 2015.
-
-"""
-
-# Set dead bits (bit 0 is the LSB)
-DEAD_BITS = [2, 4, 7]
-BIT_LENGTH = 8
-
-import numpy as np
-
-assert max(DEAD_BITS) < BIT_LENGTH
-x = ['1'] * BIT_LENGTH
-for i in DEAD_BITS:
-    x[-1 - i] = '0'
-
-dead = int(''.join(x), 2)  # e.g. 01101011 = 107
-triggers = set()
-for t in range(2 ** BIT_LENGTH):
-    triggers.add(t & dead)
-
-print('Total %d trigger values are possible.' % len(triggers))
-for t in sorted(triggers):
-    print('%s (%d)' % (np.binary_repr(t, width=BIT_LENGTH), t))
+from __future__ import print_function, division
+
+"""
+List possible trigger values assuming some pins are dead.
+
+For example, current cascading cable for AntNeuro has dead pins of 2,4,7.
+
+Kyuhwa Lee, 2015.
+
+"""
+
+# Set dead bits (bit 0 is the LSB)
+DEAD_BITS = [2, 4, 7]
+BIT_LENGTH = 8
+
+import numpy as np
+
+assert max(DEAD_BITS) < BIT_LENGTH
+x = ['1'] * BIT_LENGTH
+for i in DEAD_BITS:
+    x[-1 - i] = '0'
+
+dead = int(''.join(x), 2)  # e.g. 01101011 = 107
+triggers = set()
+for t in range(2 ** BIT_LENGTH):
+    triggers.add(t & dead)
+
+print('Total %d trigger values are possible.' % len(triggers))
+for t in sorted(triggers):
+    print('%s (%d)' % (np.binary_repr(t, width=BIT_LENGTH), t))
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/mat2fif.py` & `neurodecode-2.0.5/neurodecode/utils/mat2fif.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from __future__ import print_function, division, unicode_literals
-
-"""
-Convert Matlab signal data into fif format.
-
-Kyuhwa Lee, 2017
-Swiss Federal Institute of Technology Lausanne (EPFL)
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""
-import scipy.io
-import numpy as np
-import neurodecode.utils.q_common as qc
-from neurodecode import logger
-import mne
-
-def mat2fif(mat_file, sample_rate, data_field, event_field):
-    """
-    mat_file: Input Matlab file
-    sample_rate: Hz
-    data_field: Name of signal
-    event_field: Name of event
-    """
-    data = scipy.io.loadmat(MAT_FILE)
-    eeg_data = data[DATA_FIELD]
-    event_data = data[EVENT_FIELD]
-    num_eeg_channels = eeg_data.shape[0]
-    signals = np.concatenate( (event_data, eeg_data), axis=0 )
-    assert event_data.shape[1] == eeg_data.shape[1]
-    ch_names = ['TRIGGER'] + ['CH%d' % ch for ch in range(num_eeg_channels)]
-    ch_info = ['stim'] + ['eeg'] * num_eeg_channels
-    info = mne.create_info(ch_names, SAMPLE_RATE, ch_info)
-    raw = mne.io.RawArray(signals, info)
-    [basedir, fname, fext] = qc.parse_path_list(MAT_FILE)
-    fifname = '%s/%s.fif' % (basedir, fname)
-    raw.save(fifname, verbose=False, overwrite=True)
-    logger.info('Saved to %s.' % fifname)
-
-if __name__ == '__main__':
-    MAT_FILE = r'D:\data\Phoneme\data.mat'
-    SAMPLE_RATE = 1000.0
-    DATA_FIELD = 'ecog' # data containing signals
-    EVENT_FIELD = 'phoneme' # data containing events
-    mat2fif(MAT_FILE, SAMPLE_RATE, DATA_FIELD, EVENT_FIELD)
+from __future__ import print_function, division, unicode_literals
+
+"""
+Convert Matlab signal data into fif format.
+
+Kyuhwa Lee, 2017
+Swiss Federal Institute of Technology Lausanne (EPFL)
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+"""
+import scipy.io
+import numpy as np
+import neurodecode.utils.q_common as qc
+from neurodecode import logger
+import mne
+
+def mat2fif(mat_file, sample_rate, data_field, event_field):
+    """
+    mat_file: Input Matlab file
+    sample_rate: Hz
+    data_field: Name of signal
+    event_field: Name of event
+    """
+    data = scipy.io.loadmat(MAT_FILE)
+    eeg_data = data[DATA_FIELD]
+    event_data = data[EVENT_FIELD]
+    num_eeg_channels = eeg_data.shape[0]
+    signals = np.concatenate( (event_data, eeg_data), axis=0 )
+    assert event_data.shape[1] == eeg_data.shape[1]
+    ch_names = ['TRIGGER'] + ['CH%d' % ch for ch in range(num_eeg_channels)]
+    ch_info = ['stim'] + ['eeg'] * num_eeg_channels
+    info = mne.create_info(ch_names, SAMPLE_RATE, ch_info)
+    raw = mne.io.RawArray(signals, info)
+    [basedir, fname, fext] = qc.parse_path_list(MAT_FILE)
+    fifname = '%s/%s.fif' % (basedir, fname)
+    raw.save(fifname, verbose=False, overwrite=True)
+    logger.info('Saved to %s.' % fifname)
+
+if __name__ == '__main__':
+    MAT_FILE = r'D:\data\Phoneme\data.mat'
+    SAMPLE_RATE = 1000.0
+    DATA_FIELD = 'ecog' # data containing signals
+    EVENT_FIELD = 'phoneme' # data containing events
+    mat2fif(MAT_FILE, SAMPLE_RATE, DATA_FIELD, EVENT_FIELD)
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/merge_events.py` & `neurodecode-2.0.5/neurodecode/utils/merge_events.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-from __future__ import print_function, division
-
-"""
-Merge different events. Can be also used to simply change event values.
-
-EVENTS = dict(LABEL_MERGED:[LABEL1, LABEL2, ...])
-
-Kyuhwa Lee, 2015
-
-"""
-
-import numpy as np
-import neurodecode.utils.q_common as qc
-import neurodecode.utils.pycnbi_utils as pu
-from neurodecode.triggers.trigger_def import trigger_def
-from neurodecode import logger
-
-def merge_events(trigger_file, events, rawfile_in, rawfile_out):
-    tdef = trigger_def(trigger_file)
-    raw, eve = pu.load_raw(rawfile_in)
-
-    logger.info('=== Before merging ===')
-    notfounds = []
-    for key in np.unique(eve[:, 2]):
-        if key in tdef.by_value:
-            logger.info('%s: %d events' % (tdef.by_value[key], len(np.where(eve[:, 2] == key)[0])))
-        else:
-            logger.info('%d: %d events' % (key, len(np.where(eve[:, 2] == key)[0])))
-            notfounds.append(key)
-    if notfounds:
-        for key in notfounds:
-            logger.warning('Key %d was not found in the definition file.' % key)
-
-    for key in events:
-        ev_src = events[key]
-        ev_out = tdef.by_name[key]
-        x = []
-        for e in ev_src:
-            x.append(np.where(eve[:, 2] == tdef.by_name[e])[0])
-        eve[np.concatenate(x), 2] = ev_out
-
-    # sanity check
-    dups = np.where(0 == np.diff(eve[:, 0]))[0]
-    assert len(dups) == 0
-
-    # reset trigger channel
-    raw._data[0] *= 0
-    raw.add_events(eve, 'TRIGGER')
-    raw.save(rawfile_out, overwrite=True)
-
-    logger.info('=== After merging ===')
-    for key in np.unique(eve[:, 2]):
-        if key in tdef.by_value:
-            logger.info('%s: %d events' % (tdef.by_value[key], len(np.where(eve[:, 2] == key)[0])))
-        else:
-            logger.info('%s: %d events' % (key, len(np.where(eve[:, 2] == key)[0])))
-
-# sample code
-if __name__ == '__main__':
-    fif_dir = r'D:\data\STIMO\GO004\offline\all'
-    trigger_file = 'triggerdef_gait_chuv.ini'
-    events = {'BOTH_GO':['LEFT_GO', 'RIGHT_GO']}
-
-    out_dir = fif_dir + '/merged'
-    qc.make_dirs(out_dir)
-    for rawfile_in in qc.get_file_list(fif_dir):
-        p = qc.parse_path(rawfile_in)
-        if p.ext != 'fif':
-            continue
-        rawfile_out = '%s/%s.%s' % (out_dir, p.name, p.ext)
-        merge_events(trigger_file, events, rawfile_in, rawfile_out)
+from __future__ import print_function, division
+
+"""
+Merge different events. Can be also used to simply change event values.
+
+EVENTS = dict(LABEL_MERGED:[LABEL1, LABEL2, ...])
+
+Kyuhwa Lee, 2015
+
+"""
+
+import numpy as np
+import neurodecode.utils.q_common as qc
+import neurodecode.utils.pycnbi_utils as pu
+from neurodecode.triggers.trigger_def import trigger_def
+from neurodecode import logger
+
+def merge_events(trigger_file, events, rawfile_in, rawfile_out):
+    tdef = trigger_def(trigger_file)
+    raw, eve = pu.load_raw(rawfile_in)
+
+    logger.info('=== Before merging ===')
+    notfounds = []
+    for key in np.unique(eve[:, 2]):
+        if key in tdef.by_value:
+            logger.info('%s: %d events' % (tdef.by_value[key], len(np.where(eve[:, 2] == key)[0])))
+        else:
+            logger.info('%d: %d events' % (key, len(np.where(eve[:, 2] == key)[0])))
+            notfounds.append(key)
+    if notfounds:
+        for key in notfounds:
+            logger.warning('Key %d was not found in the definition file.' % key)
+
+    for key in events:
+        ev_src = events[key]
+        ev_out = tdef.by_name[key]
+        x = []
+        for e in ev_src:
+            x.append(np.where(eve[:, 2] == tdef.by_name[e])[0])
+        eve[np.concatenate(x), 2] = ev_out
+
+    # sanity check
+    dups = np.where(0 == np.diff(eve[:, 0]))[0]
+    assert len(dups) == 0
+
+    # reset trigger channel
+    raw._data[0] *= 0
+    raw.add_events(eve, 'TRIGGER')
+    raw.save(rawfile_out, overwrite=True)
+
+    logger.info('=== After merging ===')
+    for key in np.unique(eve[:, 2]):
+        if key in tdef.by_value:
+            logger.info('%s: %d events' % (tdef.by_value[key], len(np.where(eve[:, 2] == key)[0])))
+        else:
+            logger.info('%s: %d events' % (key, len(np.where(eve[:, 2] == key)[0])))
+
+# sample code
+if __name__ == '__main__':
+    fif_dir = r'D:\data\STIMO\GO004\offline\all'
+    trigger_file = 'triggerdef_gait_chuv.ini'
+    events = {'BOTH_GO':['LEFT_GO', 'RIGHT_GO']}
+
+    out_dir = fif_dir + '/merged'
+    qc.make_dirs(out_dir)
+    for rawfile_in in qc.get_file_list(fif_dir):
+        p = qc.parse_path(rawfile_in)
+        if p.ext != 'fif':
+            continue
+        rawfile_out = '%s/%s.%s' % (out_dir, p.name, p.ext)
+        merge_events(trigger_file, events, rawfile_in, rawfile_out)
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/nd_lsl.py` & `neurodecode-2.0.5/neurodecode/utils/nd_lsl.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-from __future__ import print_function, division
-
-"""
-LSL wrapper functions for creating a server and a client
-
-Kyuhwa Lee, 2014
-Swiss Federal Institute of Technology Lausanne (EPFL)
-
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-"""
-import sys
-import time
-import pylsl
-import multiprocessing as mp
-from neurodecode import logger
-
-
-def start_server(server_name, n_channels=1, channel_format='string', nominal_srate=pylsl.IRREGULAR_RATE, stype='EEG',
-                 source_id=None):
-    """
-    Start a new LSL server
-
-    Params
-    ------
-    server_name:
-        Name of the server
-    n_channels:
-        Number of channels
-    channel_format:
-        pylsl.cf_string (or 'string')
-        pylsl.cf_float32 (or 'float32')
-        pylsl.cf_double64 (or 'double64')
-        pylsl.cf_int8 (or 'int8')
-        pylsl.cf_int16 (or 'int16')
-        pylsl.cf_int32 (or 'int32')
-        pylsl.cf_int64 (or 'int64')
-    nominal_srate:
-        Sampling rate in Hz. Defaults to irregular sampling rate.
-    stype:
-        Signal type in string format
-    source_id:
-        If None, set to server name
-
-    Returns
-    -------
-    outlet: LSL server object
-
-    """
-    if source_id is None:
-        source_id = server_name
-    sinfo = pylsl.StreamInfo(server_name, channel_count=n_channels, channel_format=channel_format,\
-                           nominal_srate=nominal_srate, type=stype, source_id=source_id)
-    return pylsl.StreamOutlet(sinfo)
-
-
-def start_client(server_name):
-    """
-    Search and connect to an LSL server
-
-    Params
-    ------
-    server_name:
-        Name of the server to search
-
-    Returns
-    -------
-    inlet:
-        LSL client object
-
-    """
-    while True:
-        logger.info('Searching for LSL server %s ...' % server_name)
-        streamInfos = pylsl.resolve_byprop("name", server_name, timeout=1)
-        if not streamInfos:
-            continue
-        for sinfo in streamInfos:
-            logger.info('Found %s' % sinfo.name())
-        if len(streamInfos) == 0:
-            logger.info('No desired LSL server found. Keep searching...')
-            time.sleep(1.0)
-        else:
-            sinfo = streamInfos[0]
-            break
-    return pylsl.StreamInlet(sinfo)
+from __future__ import print_function, division
+
+"""
+LSL wrapper functions for creating a server and a client
+
+Kyuhwa Lee, 2014
+Swiss Federal Institute of Technology Lausanne (EPFL)
+
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+"""
+import sys
+import time
+import pylsl
+import multiprocessing as mp
+from neurodecode import logger
+
+
+def start_server(server_name, n_channels=1, channel_format='string', nominal_srate=pylsl.IRREGULAR_RATE, stype='EEG',
+                 source_id=None):
+    """
+    Start a new LSL server
+
+    Params
+    ------
+    server_name:
+        Name of the server
+    n_channels:
+        Number of channels
+    channel_format:
+        pylsl.cf_string (or 'string')
+        pylsl.cf_float32 (or 'float32')
+        pylsl.cf_double64 (or 'double64')
+        pylsl.cf_int8 (or 'int8')
+        pylsl.cf_int16 (or 'int16')
+        pylsl.cf_int32 (or 'int32')
+        pylsl.cf_int64 (or 'int64')
+    nominal_srate:
+        Sampling rate in Hz. Defaults to irregular sampling rate.
+    stype:
+        Signal type in string format
+    source_id:
+        If None, set to server name
+
+    Returns
+    -------
+    outlet: LSL server object
+
+    """
+    if source_id is None:
+        source_id = server_name
+    sinfo = pylsl.StreamInfo(server_name, channel_count=n_channels, channel_format=channel_format,\
+                           nominal_srate=nominal_srate, type=stype, source_id=source_id)
+    return pylsl.StreamOutlet(sinfo)
+
+
+def start_client(server_name):
+    """
+    Search and connect to an LSL server
+
+    Params
+    ------
+    server_name:
+        Name of the server to search
+
+    Returns
+    -------
+    inlet:
+        LSL client object
+
+    """
+    while True:
+        logger.info('Searching for LSL server %s ...' % server_name)
+        streamInfos = pylsl.resolve_byprop("name", server_name, timeout=1)
+        if not streamInfos:
+            continue
+        for sinfo in streamInfos:
+            logger.info('Found %s' % sinfo.name())
+        if len(streamInfos) == 0:
+            logger.info('No desired LSL server found. Keep searching...')
+            time.sleep(1.0)
+        else:
+            sinfo = streamInfos[0]
+            break
+    return pylsl.StreamInlet(sinfo)
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/parse_online_results.py` & `neurodecode-2.0.5/neurodecode/utils/parse_online_results.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from __future__ import print_function, division
-
-"""
-Compute confusion matrix and accuracy from online result logs.
-
-Kyuhwa Lee (kyu.lee@epfl.ch)
-Swiss Federal Institute of Technology of Lausanne (EPFL)
-"""
-
-LOG_DIR = r'D:\data\MI\rx1\classifier\gait-ULR-250ms'
-
-import neurodecode
-import neurodecode.utils.q_common as qc
-
-dtlist = []
-gtlist = []
-for f in qc.get_file_list(LOG_DIR):
-    [basedir, fname, fext] = qc.parse_path_list(f)
-    if 'online' not in fname or fext != 'txt':
-        continue
-    print(f)
-
-    for l in open(f):
-        if len(l.strip()) == 0: break
-        gt, dt = l.strip().split(',')
-        gtlist.append(gt)
-        dtlist.append(dt)
-
-print('Ground-truth: %s' % ''.join(gtlist))
-print('Detected as : %s' % ''.join(dtlist))
-cfmat, acc = qc.confusion_matrix(gtlist, dtlist)
-print('\nAverage accuracy: %.3f' % acc)
-print(cfmat)
+from __future__ import print_function, division
+
+"""
+Compute confusion matrix and accuracy from online result logs.
+
+Kyuhwa Lee (kyu.lee@epfl.ch)
+Swiss Federal Institute of Technology of Lausanne (EPFL)
+"""
+
+LOG_DIR = r'D:\data\MI\rx1\classifier\gait-ULR-250ms'
+
+import neurodecode
+import neurodecode.utils.q_common as qc
+
+dtlist = []
+gtlist = []
+for f in qc.get_file_list(LOG_DIR):
+    [basedir, fname, fext] = qc.parse_path_list(f)
+    if 'online' not in fname or fext != 'txt':
+        continue
+    print(f)
+
+    for l in open(f):
+        if len(l.strip()) == 0: break
+        gt, dt = l.strip().split(',')
+        gtlist.append(gt)
+        dtlist.append(dt)
+
+print('Ground-truth: %s' % ''.join(gtlist))
+print('Detected as : %s' % ''.join(dtlist))
+cfmat, acc = qc.confusion_matrix(gtlist, dtlist)
+print('\nAverage accuracy: %.3f' % acc)
+print(cfmat)
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/psd_visualizer.py` & `neurodecode-2.0.5/neurodecode/utils/psd_visualizer.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-"""
-Real-time PSD visualization script
-
-TODO: make it a function or a class
-
-Author:
-Kyuhwa Lee
-
-"""
-
-amp_name = 'openvibeSignal'
-amp_serial = None
-
-# screen
-screen_offset_x = 100
-screen_offset_y = 100
-
-# channels
-channel_picks = ['L1', 'L2', 'L3', 'R1', 'R2', 'R3']
-
-# PSD
-w_seconds = 0.5
-fmin = 71
-fmax = 200
-
-# filters
-spatial = None #'car'
-spatial_ch = None
-spectral = None
-spectral_ch = None
-notch = None
-notch_ch = None
-multiplier = 1
-
-
-# code begins
-from mne.decoding import PSDEstimator
-from neurodecode.stream_receiver.stream_receiver import StreamReceiver
-import neurodecode.utils.pycnbi_utils as pu
-import numpy as np
-import cv2
-import mne
-import os
-mne.set_log_level('ERROR')
-os.environ['OMP_NUM_THREADS'] = '1' # actually improves performance for multitaper
-
-
-def get_psd(sr, psde, picks):
-    sr.acquire()
-    w, ts = sr.get_window()  # w = times x channels
-    w = w.T  # -> channels x times
-
-    # apply filters. Important: maintain the original channel order at this point.
-    w = pu.preprocess(w, sfreq=sfreq, spatial=spatial, spatial_ch=spatial_ch,
-                      spectral=spectral, spectral_ch=spectral_ch, notch=notch,
-                              notch_ch=notch_ch, multiplier=multiplier)
-
-    # select the same channels used for training
-    w = w[picks]
-
-    # debug: show max - min
-    # c=1; print( '### %d: %.1f - %.1f = %.1f'% ( picks[c], max(w[c]), min(w[c]), max(w[c])-min(w[c]) ) )
-
-    # psde.transform = [channels x freqs]
-    psd = psde.transform(w)
-
-    return psd
-
-if __name__ == '__main__':
-    sr = StreamReceiver(window_size=w_seconds, amp_name=amp_name, amp_serial=amp_serial)
-    sfreq = sr.sample_rate
-    psde = PSDEstimator(sfreq=sfreq, fmin=fmin, fmax=fmax, bandwidth=None, adaptive=False,
-                                     low_bias=True, n_jobs=1, normalization='length', verbose=None)
-    ch_names = sr.get_channel_names()
-    fq_res = 1 / w_seconds
-    hz_list = []
-    f = fmin
-    while f <= fmax:
-        hz_list.append(f)
-        f += fq_res
-    picks = [ch_names.index(ch) for ch in channel_picks]
-    psd = get_psd(sr, psde, picks).T # freq x ch
-    assert len(hz_list) == psd.shape[0], (len(hz_list), psd.shape[0])
-    cv2.namedWindow("img", cv2.WINDOW_AUTOSIZE)
-    cv2.moveWindow("img", screen_offset_x, screen_offset_y)
-    #cv2.setWindowProperty("img", cv2.WND_PROP_FULLSCREEN, cv2.WINDOW_FULLSCREEN);
-    mul_x = 50
-    mul_y = 20
-    fq_width = 55
-    ch_height = 30
-    img_x = psd.shape[1] * mul_x
-    img_y = psd.shape[0] * mul_y
-    img = np.zeros((img_y + ch_height, img_x + fq_width), np.uint8)
-    # channels
-    for x in range(psd.shape[1]):
-        cv2.putText(img, '%s' % ch_names[picks[x]], (x * mul_x + fq_width + 13, img_y + ch_height - 10),
-                    cv2.FONT_HERSHEY_DUPLEX, 0.5, [255,255,255], 1, cv2.LINE_AA)
-    # frequencies
-    for y in range(psd.shape[0]):
-        cv2.putText(img, '%5.0f' % hz_list[y], (1, y * mul_y + 15), cv2.FONT_HERSHEY_DUPLEX,
-                    0.5, [255,255,255], 1, cv2.LINE_AA)
-    cv2.putText(img, 'Hz/Ch', (1, img_y + ch_height - 10), cv2.FONT_HERSHEY_DUPLEX, 0.5, [255,255,255], 1, cv2.LINE_AA)
-
-    key = 0
-    while key != 27:
-        psd = get_psd(sr, psde, picks)
-        psd_r = np.true_divide(psd, np.mean(psd, axis=0))
-        psd_r = psd_r - np.min(psd_r, axis=0)
-        psd_r = np.true_divide(psd_r, np.max(psd_r, axis=0))
-        psd_n = np.round(psd_r * 255) # freq x ch
-
-        psd_img = cv2.resize(psd_n.T, (img_x, img_y), interpolation=0)
-        img[:-ch_height, fq_width:] = psd_img
-        #cv2.imshow("img", cv2.cvtColor(cv2.cvtColor(img, code=cv2.COLOR_GRAY2BGR), code=cv2.COLOR_BGR2HSV))
-        cv2.imshow("img", img)
-        key = cv2.waitKey(1)
+"""
+Real-time PSD visualization script
+
+TODO: make it a function or a class
+
+Author:
+Kyuhwa Lee
+
+"""
+
+amp_name = 'openvibeSignal'
+amp_serial = None
+
+# screen
+screen_offset_x = 100
+screen_offset_y = 100
+
+# channels
+channel_picks = ['L1', 'L2', 'L3', 'R1', 'R2', 'R3']
+
+# PSD
+w_seconds = 0.5
+fmin = 71
+fmax = 200
+
+# filters
+spatial = None #'car'
+spatial_ch = None
+spectral = None
+spectral_ch = None
+notch = None
+notch_ch = None
+multiplier = 1
+
+
+# code begins
+from mne.decoding import PSDEstimator
+from neurodecode.stream_receiver.stream_receiver import StreamReceiver
+import neurodecode.utils.pycnbi_utils as pu
+import numpy as np
+import cv2
+import mne
+import os
+mne.set_log_level('ERROR')
+os.environ['OMP_NUM_THREADS'] = '1' # actually improves performance for multitaper
+
+
+def get_psd(sr, psde, picks):
+    sr.acquire()
+    w, ts = sr.get_window()  # w = times x channels
+    w = w.T  # -> channels x times
+
+    # apply filters. Important: maintain the original channel order at this point.
+    w = pu.preprocess(w, sfreq=sfreq, spatial=spatial, spatial_ch=spatial_ch,
+                      spectral=spectral, spectral_ch=spectral_ch, notch=notch,
+                              notch_ch=notch_ch, multiplier=multiplier)
+
+    # select the same channels used for training
+    w = w[picks]
+
+    # debug: show max - min
+    # c=1; print( '### %d: %.1f - %.1f = %.1f'% ( picks[c], max(w[c]), min(w[c]), max(w[c])-min(w[c]) ) )
+
+    # psde.transform = [channels x freqs]
+    psd = psde.transform(w)
+
+    return psd
+
+if __name__ == '__main__':
+    sr = StreamReceiver(window_size=w_seconds, amp_name=amp_name, amp_serial=amp_serial)
+    sfreq = sr.sample_rate
+    psde = PSDEstimator(sfreq=sfreq, fmin=fmin, fmax=fmax, bandwidth=None, adaptive=False,
+                                     low_bias=True, n_jobs=1, normalization='length', verbose=None)
+    ch_names = sr.get_channel_names()
+    fq_res = 1 / w_seconds
+    hz_list = []
+    f = fmin
+    while f <= fmax:
+        hz_list.append(f)
+        f += fq_res
+    picks = [ch_names.index(ch) for ch in channel_picks]
+    psd = get_psd(sr, psde, picks).T # freq x ch
+    assert len(hz_list) == psd.shape[0], (len(hz_list), psd.shape[0])
+    cv2.namedWindow("img", cv2.WINDOW_AUTOSIZE)
+    cv2.moveWindow("img", screen_offset_x, screen_offset_y)
+    #cv2.setWindowProperty("img", cv2.WND_PROP_FULLSCREEN, cv2.WINDOW_FULLSCREEN);
+    mul_x = 50
+    mul_y = 20
+    fq_width = 55
+    ch_height = 30
+    img_x = psd.shape[1] * mul_x
+    img_y = psd.shape[0] * mul_y
+    img = np.zeros((img_y + ch_height, img_x + fq_width), np.uint8)
+    # channels
+    for x in range(psd.shape[1]):
+        cv2.putText(img, '%s' % ch_names[picks[x]], (x * mul_x + fq_width + 13, img_y + ch_height - 10),
+                    cv2.FONT_HERSHEY_DUPLEX, 0.5, [255,255,255], 1, cv2.LINE_AA)
+    # frequencies
+    for y in range(psd.shape[0]):
+        cv2.putText(img, '%5.0f' % hz_list[y], (1, y * mul_y + 15), cv2.FONT_HERSHEY_DUPLEX,
+                    0.5, [255,255,255], 1, cv2.LINE_AA)
+    cv2.putText(img, 'Hz/Ch', (1, img_y + ch_height - 10), cv2.FONT_HERSHEY_DUPLEX, 0.5, [255,255,255], 1, cv2.LINE_AA)
+
+    key = 0
+    while key != 27:
+        psd = get_psd(sr, psde, picks)
+        psd_r = np.true_divide(psd, np.mean(psd, axis=0))
+        psd_r = psd_r - np.min(psd_r, axis=0)
+        psd_r = np.true_divide(psd_r, np.max(psd_r, axis=0))
+        psd_n = np.round(psd_r * 255) # freq x ch
+
+        psd_img = cv2.resize(psd_n.T, (img_x, img_y), interpolation=0)
+        img[:-ch_height, fq_width:] = psd_img
+        #cv2.imshow("img", cv2.cvtColor(cv2.cvtColor(img, code=cv2.COLOR_GRAY2BGR), code=cv2.COLOR_BGR2HSV))
+        cv2.imshow("img", img)
+        key = cv2.waitKey(1)
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/pycnbi_utils.py` & `neurodecode-2.0.5/neurodecode/utils/pycnbi_utils.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,672 +1,672 @@
-from __future__ import print_function, division
-
-"""
-PyCNBI utility functions
-
-Note:
-When exporting to Panda Dataframes format, raw.as_data_frame() silently
-scales data to the Volts unit by default, which is the convention in MNE.
-Try raw.as_data_frame(scalings=dict(eeg=1.0, misc=1.0))
-
-Kyuhwa Lee, 2014
-Swiss Federal Institute of Technology Lausanne (EPFL)
-
-"""
-
-import os
-import sys
-import mne
-import pylsl
-import scipy.io
-import importlib
-import numpy as np
-import multiprocessing as mp
-import xml.etree.ElementTree as ET
-import neurodecode.utils.q_common as qc
-from scipy.signal import butter, lfilter, lfiltic, buttord
-from neurodecode.pycnbi_config import CAP, LAPLACIAN
-from neurodecode import logger
-from builtins import input
-
-mne.set_log_level('ERROR')
-os.environ['OMP_NUM_THREADS'] = '1' # actually improves performance for multitaper
-
-
-# note that MNE already has find_events function
-def find_events(events_raw):
-    """
-    Find trigger values, rising from zero to non-zero
-    """
-    events = []  # triggered event values other than zero
-
-    # set epochs (frame start, frame end)
-    ev_last = 0
-    for et in range(len(events_raw)):
-        ev = events_raw[et]
-        if ev != ev_last:
-            if ev > 0:
-                events.append([et, 0, ev])
-            ev_last = ev
-
-    return events
-
-
-def find_event_channel(raw=None, ch_names=None):
-    """
-    Find event channel using heuristics for pcl files.
-
-    Disclaimer: Not 100% guaranteed to find.
-
-    Input:
-        raw: mne.io.RawArray-like object or numpy array (n_channels x n_samples)
-        if raw is None, ch_names must be given.
-
-    Output:
-        channel index or None if not found.
-    """
-
-    if type(raw) == np.ndarray:
-        if ch_names is not None:
-            for ch_name in ch_names:
-                if 'TRIGGER' in ch_name or 'STI ' in ch_name or 'TRG' in ch_name or 'CH_Event' in ch_name:
-                    return ch_names.index(ch_name)
-
-        # data range between 0 and 255 and all integers?
-        for ch in range(raw.shape[0]):
-            if (raw[ch].astype(int) == raw[ch]).all()\
-                    and max(raw[ch]) < 256 and min(raw[ch]) == 0:
-                return ch
-    elif hasattr(raw, 'ch_names'):
-        for ch_name in raw.ch_names:
-            if 'TRIGGER' in ch_name or 'STI ' in ch_name or 'TRG' in ch_name or 'CH_Event' in ch_name:
-                return raw.ch_names.index(ch_name)
-    else:
-        if ch_names is None:
-            raise ValueError('ch_names cannot be None when raw is None.')
-        for ch_name in ch_names:
-            if 'TRIGGER' in ch_name or 'STI ' in ch_name or 'TRG' in ch_name or 'CH_Event' in ch_name:
-                return ch_names.index(ch_name)
-    return None
-
-
-def raw2mat(infile, outfile):
-    '''
-    Convert raw data file to MATLAB file
-    '''
-    raw, events = load_raw(infile)
-    header = dict(bads=raw.info['bads'], ch_names=raw.info['ch_names'],\
-                  sfreq=raw.info['sfreq'], events=events)
-    scipy.io.savemat(outfile, dict(signals=raw._data, header=header))
-    logger.info('Exported to %s' % outfile)
-
-
-def add_events_raw(rawfile, outfile, eventfile, overwrite=True):
-    """
-    Add events from a file and save
-
-    Note: If the event values already exists in raw file, the new event values
-        will be added to the previous value instead of replacing them.
-    """
-
-    raw = mne.io.Raw(rawfile, preload=True, proj=False)
-    events = mne.read_events(eventfile)
-    raw.add_events(events, stim_channel='TRIGGER')
-    raw.save(outfile, overwrite=overwrite)
-
-
-def export_morlet(epochs, filename):
-    """
-    Export wavelet tranformation decomposition into Matlab format
-    """
-    freqs = np.array(DWT['freqs'])  # define frequencies of interest
-    n_cycles = freqs / 2.  # different number of cycle per frequency
-    power, itc = mne.time_frequency.tfr_morlet(epochs, freqs=freqs,
-        n_cycles=n_cycles, use_fft=False, return_itc=True, n_jobs=mp.cpu_count())
-    scipy.io.savemat(filename, dict(power=power.data, itc=itc.data, freqs=freqs,
-        channels=epochs.ch_names, sfreq=epochs.info['sfreq'], onset=-epochs.tmin))
-
-
-def event_timestamps_to_indices(sigfile, eventfile):
-    """
-    Convert LSL timestamps to sample indices for separetely recorded events.
-
-    Parameters:
-    sigfile: raw signal file (Python Pickle) recorded with stream_recorder.py.
-    eventfile: event file where events are indexed with LSL timestamps.
-
-    Returns:
-    events list, which can be used as an input to mne.io.RawArray.add_events().
-    """
-
-    raw = qc.load_obj(sigfile)
-    ts = raw['timestamps'].reshape(-1)
-    ts_min = min(ts)
-    ts_max = max(ts)
-    events = []
-
-    with open(eventfile) as f:
-        for l in f:
-            data = l.strip().split('\t')
-            event_ts = float(data[0])
-            event_value = int(data[2])
-            # find the first index not smaller than ts
-            next_index = np.searchsorted(ts, event_ts)
-            if next_index >= len(ts):
-                logger.warning('Event %d at time %.3f is out of time range (%.3f - %.3f).' % (event_value, event_ts, ts_min, ts_max))
-            else:
-                events.append([next_index, 0, event_value])
-    return events
-
-
-def rereference(raw, ref_new, ref_old=None):
-    """
-    Reference to new channels. raw object is modified in-place for efficiency.
-
-    raw: mne.io.RawArray
-
-    ref_new: None | list of str (RawArray) | list of int (numpy array)
-        Channel(s) to re-reference, e.g. M1, M2.
-        Average of these channel values are substracted from all channel values.
-
-    ref_old: None | str
-        Channel to recover, assuming this channel was originally used as a reference.
-    """
-
-    # Re-reference and recover the original reference channel values if possible
-    if type(raw) == np.ndarray:
-        if raw_ch_old is not None:
-            logger.error('Recovering original reference channel is not yet supported for numpy arrays.')
-            raise NotImplementedError
-        if type(raw_ch_new[0]) is not int:
-            logger.error('Channels must be integer values for numpy arrays')
-            raise ValueError
-        raw -= np.mean(raw[ref_new], axis=0)
-    else:
-        if ref_old is not None:
-            # Add a blank (zero-valued) channel
-            mne.io.add_reference_channels(raw, ref_old, copy=False)
-        # Re-reference
-        mne.io.set_eeg_reference(raw, ref_new, copy=False)
-
-    return True
-
-
-def preprocess(raw, sfreq=None, spatial=None, spatial_ch=None, spectral=None, spectral_ch=None,
-               notch=None, notch_ch=None, multiplier=1, ch_names=None, rereference=None, decim=None, n_jobs=1):
-    """
-    Apply spatial, spectral, notch filters and convert unit.
-    raw is modified in-place.
-
-    Input
-    ------
-    raw: mne.io.Raw | mne.io.RawArray | mne.Epochs | numpy.array (n_channels x n_samples)
-         numpy.array type assumes the data has only pure EEG channnels without event channels
-
-    sfreq: required only if raw is numpy array.
-
-    spatial: None | 'car' | 'laplacian'
-        Spatial filter type.
-
-    spatial_ch: None | list (for CAR) | dict (for LAPLACIAN)
-        Reference channels for spatial filtering. May contain channel names.
-        'car': channel indices used for CAR filtering. If None, use all channels except
-               the trigger channel (index 0).
-        'laplacian': {channel:[neighbor1, neighbor2, ...], ...}
-        (Note) since Neurodecode puts trigger channel as index 0, data channel starts from index 1.
-
-    spectral: None | [l_freq, h_freq]
-        Spectral filter.
-        if l_freq is None: lowpass filter is applied.
-        if h_freq is None: highpass filter is applied.
-        if l_freq < h_freq: bandpass filter is applied.
-        if l_freq > h_freq: band-stop filter is applied.
-
-    spectral_ch: None | list
-        Channel picks for spectra filtering. May contain channel names.
-
-    notch: None | float | list of frequency in floats
-        Notch filter.
-
-    notch_ch: None | list
-        Channel picks for notch filtering. May contain channel names.
-
-    multiplier: float
-        If not 1, multiply data values excluding trigger values.
-
-    ch_names: None | list
-        If raw is numpy array and channel picks are list of strings, ch_names will
-        be used as a look-up table to convert channel picks to channel numbers.
-
-    rereference: Not supported yet.
-
-    decim: None | int
-        Apply low-pass filter and decimate (downsample). sfreq must be given. Ignored if 1.
-
-    Output
-    ------
-    Same input data structure.
-
-    Note: To save computation time, input data may be modified in-place.
-    TODO: Add an option to disable in-place modification.
-    """
-
-    # Check datatype
-    if type(raw) == np.ndarray:
-        # Numpy array: assume we don't have event channel
-        data = raw
-        assert sfreq is not None and sfreq > 0, 'Wrong sfreq value.'
-        assert 2 <= len(data.shape) <= 3, 'Unknown data shape. The dimension must be 2 or 3.'
-        if len(data.shape) == 3:
-            n_channels = data.shape[1]
-        elif len(data.shape) == 2:
-            n_channels = data.shape[0]
-        eeg_channels = list(range(n_channels))
-        if decim is not None and decim != 1:
-            if sfreq is None:
-                logger.error('Decimation cannot be applied if sfreq is None.')
-                raise ValueError
-    else:
-        # MNE Raw object: exclude event channel
-        ch_names = raw.ch_names
-        data = raw._data
-        sfreq = raw.info['sfreq']
-        assert 2 <= len(data.shape) <= 3, 'Unknown data shape. The dimension must be 2 or 3.'
-        if len(data.shape) == 3:
-            # assert type(raw) is mne.epochs.Epochs
-            n_channels = data.shape[1]
-        elif len(data.shape) == 2:
-            n_channels = data.shape[0]
-        eeg_channels = list(range(n_channels))
-        tch = find_event_channel(raw)
-        if tch is None:
-            logger.warning('No trigger channel found. Using all channels.')
-        else:
-            tch_name = ch_names[tch]
-            eeg_channels.pop(tch)
-
-    # Re-reference channels
-    if rereference is not None:
-        logger.error('re-referencing not implemented yet. Sorry.')
-        raise NotImplementedError
-
-    # Do unit conversion
-    if multiplier != 1:
-        data[eeg_channels] *= multiplier
-
-    # Apply spatial filter
-    if spatial is None:
-        pass
-    elif spatial == 'car':
-        if spatial_ch is None:
-            spatial_ch = eeg_channels
-
-        if type(spatial_ch[0]) == str:
-            assert ch_names is not None, 'preprocess(): ch_names must not be None'
-            spatial_ch_i = [ch_names.index(c) for c in spatial_ch]
-        else:
-            spatial_ch_i = spatial_ch
-
-        if len(spatial_ch_i) > 1:
-            if len(data.shape) == 2:
-                data[spatial_ch_i] -= np.mean(data[spatial_ch_i], axis=0)
-            elif len(data.shape) == 3:
-                means = np.mean(data[:, spatial_ch_i, :], axis=1)
-                data[:, spatial_ch_i, :] -= means[:, np.newaxis, :]
-            else:
-                logger.error('Unknown data shape %s' % str(data.shape))
-                raise ValueError
-    elif spatial == 'laplacian':
-        if type(spatial_ch) is not dict:
-            logger.error('preprocess(): For Lapcacian, spatial_ch must be of form {CHANNEL:[NEIGHBORS], ...}')
-            raise TypeError
-        if type(spatial_ch.keys()[0]) == str:
-            spatial_ch_i = {}
-            for c in spatial_ch:
-                ref_ch = ch_names.index(c)
-                spatial_ch_i[ref_ch] = [ch_names.index(n) for n in spatial_ch[c]]
-        else:
-            spatial_ch_i = spatial_ch
-
-        if len(spatial_ch_i) > 1:
-            rawcopy = data.copy()
-            for src in spatial_ch:
-                nei = spatial_ch[src]
-                if len(data.shape) == 2:
-                    data[src] = rawcopy[src] - np.mean(rawcopy[nei], axis=0)
-                elif len(data.shape) == 3:
-                    data[:, src, :] = rawcopy[:, src, :] - np.mean(rawcopy[:, nei, :], axis=1)
-                else:
-                    logger.error('preprocess(): Unknown data shape %s' % str(data.shape))
-                    raise ValueError
-    else:
-        logger.error('preprocess(): Unknown spatial filter %s' % spatial)
-        raise ValueError
-
-    # Downsample
-    if decim is not None and decim != 1:
-        if type(raw) == np.ndarray:
-            data = mne.filter.resample(data, down=decim, npad='auto', window='boxcar', n_jobs=1)
-        else:
-            # resample() of Raw* and Epochs object internally calls mne.filter.resample()
-            raw = raw.resample(raw.info['sfreq'] / decim, npad='auto', window='boxcar', n_jobs=1)
-            data = raw._data
-        sfreq /= decim
-
-    # Apply spectral filter
-    if spectral is not None:
-        if spectral_ch is None:
-            spectral_ch = eeg_channels
-
-        if type(spectral_ch[0]) == str:
-            assert ch_names is not None, 'preprocess(): ch_names must not be None'
-            spectral_ch_i = [ch_names.index(c) for c in spectral_ch]
-        else:
-            spectral_ch_i = spectral_ch
-
-        # fir_design='firwin' is especially important for ICA analysis. See:
-        # http://martinos.org/mne/dev/generated/mne.preprocessing.ICA.html?highlight=score_sources#mne.preprocessing.ICA.score_sources
-        mne.filter.filter_data(data, sfreq, spectral[0], spectral[1], picks=spectral_ch_i,
-            filter_length='auto', l_trans_bandwidth='auto',
-            h_trans_bandwidth='auto', n_jobs=n_jobs, method='fir',
-            iir_params=None, copy=False, phase='zero',
-            fir_window='hamming', fir_design='firwin', verbose='ERROR')
-
-    # Apply notch filter
-    if notch is not None:
-        if notch_ch is None:
-            notch_ch = eeg_channels
-
-        if type(notch_ch[0]) == str:
-            assert ch_names is not None, 'preprocess(): ch_names must not be None'
-            notch_ch_i = [ch_names.index(c) for c in notch_ch]
-        else:
-            notch_ch_i = notch_ch
-
-        mne.filter.notch_filter(data, Fs=sfreq, freqs=notch, notch_widths=5,
-                                picks=notch_ch_i, method='fft', n_jobs=n_jobs, copy=False)
-
-    if type(raw) == np.ndarray:
-        raw = data
-    return raw
-
-
-def load_raw(rawfile, spfilter=None, spchannels=None, events_ext=None, multiplier=1, verbose='ERROR'):
-    """
-    Loads data from a fif-format file.
-    You can convert non-fif files (.eeg, .bdf, .gdf, .pcl) to fif format.
-
-    Parameters:
-    rawfile: (absolute) data file path
-    spfilter: 'car' | 'laplacian' | None
-    spchannels: None | list (for CAR) | dict (for LAPLACIAN)
-        'car': channel indices used for CAR filtering. If None, use all channels except
-               the trigger channel (index 0).
-        'laplacian': {channel:[neighbor1, neighbor2, ...], ...}
-        *** Note ***
-        Since PyCNBI puts trigger channel as index 0, data channel starts from index 1.
-    events_ext: Add externally recorded events.
-                [ [sample_index1, 0, event_value1],... ]
-    multiplier: Multiply all values except triggers (to convert unit).
-
-    Returns:
-    raw: mne.io.RawArray object. First channel (index 0) is always trigger channel.
-    events: mne-compatible events numpy array object (N x [frame, 0, type])
-    spfilter= {None | 'car' | 'laplacian'}
-
-    """
-
-    if not os.path.exists(rawfile):
-        logger.error('File %s not found' % rawfile)
-        raise IOError
-    if not os.path.isfile(rawfile):
-        logger.error('%s is not a file' % rawfile)
-        raise IOError
-
-    extension = qc.parse_path(rawfile).ext
-    assert extension in ['fif', 'fiff'], 'only fif format is supported'
-    raw = mne.io.Raw(rawfile, preload=True, verbose=verbose)
-    if spfilter is not None or multiplier != 1:
-        preprocess(raw, spatial=spfilter, spatial_ch=spchannels, multiplier=multiplier)
-    if events_ext is not None:
-        events = mne.read_events(events_ext)
-    else:
-        tch = find_event_channel(raw)
-        if tch is not None:
-            events = mne.find_events(raw, stim_channel=raw.ch_names[tch], shortest_event=1,
-                uint_cast=True, consecutive='increasing', output='onset', initial_event=True)
-            # some of MNE's functions do not correctly update first_samp, especially Raw.crop() function
-            events[:, 0] -= raw.first_samp
-        else:
-            events = np.array([], dtype=np.int64)
-
-    return raw, events
-
-
-def load_multi(src, spfilter=None, spchannels=None, multiplier=1):
-    """
-    Load multiple data files and concatenate them into a single series
-
-    - Assumes all files have the same sampling rate and channel order.
-    - Event locations are updated accordingly with new offset.
-
-    @params:
-        src: directory or list of files.
-        spfilter: apply spatial filter while loading.
-        spchannels: list of channel names to apply spatial filter.
-        multiplier: to change units for better numerical stability.
-
-    See load_raw() for more low-level details.
-
-    """
-
-    if type(src) == str:
-        if not os.path.isdir(src):
-            logger.error('%s is not a directory or does not exist.' % src)
-            raise IOError
-        flist = []
-        for f in qc.get_file_list(src):
-            if qc.parse_path_list(f)[2] == 'fif':
-                flist.append(f)
-    elif type(src) in [list, tuple]:
-        flist = src
-    else:
-        logger.error('Unknown input type %s' % type(src))
-        raise TypeError
-
-    if len(flist) == 0:
-        logger.error('load_multi(): No fif files found in %s.' % src)
-        raise RuntimeError
-    elif len(flist) == 1:
-        return load_raw(flist[0], spfilter=spfilter, spchannels=spchannels, multiplier=multiplier)
-
-    # load raw files
-    rawlist = []
-    for f in flist:
-        logger.info('Loading %s' % f)
-        raw, _ = load_raw(f, spfilter=spfilter, spchannels=spchannels, multiplier=multiplier)
-        rawlist.append(raw)
-
-    # concatenate signals
-    signals = None
-    for raw in rawlist:
-        if signals is None:
-            signals = raw._data
-        else:
-            signals = np.concatenate((signals, raw._data), axis=1) # append samples
-
-    # create a concatenated raw object and update channel names
-    raw = rawlist[0]
-    trigch = find_event_channel(raw)
-    ch_types = ['eeg'] * len(raw.ch_names)
-    if trigch is not None:
-        ch_types[trigch] = 'stim'
-    info = mne.create_info(raw.ch_names, raw.info['sfreq'], ch_types)
-    raw_merged = mne.io.RawArray(signals, info)
-
-    # re-calculate event positions
-    events = mne.find_events(raw_merged, stim_channel='TRIGGER', shortest_event=1,
-        uint_cast=True, consecutive='increasing', output='onset', initial_event=True)
-
-    return raw_merged, events
-
-
-def butter_bandpass(highcut, lowcut, fs, num_ch):
-    """
-    Calculation of bandpass coefficients.
-    Order is computed automatically.
-    Note that if filter is unstable this function crashes.
-
-    TODO: handle exceptions
-    """
-
-    low = lowcut / (0.5 * fs)
-    high = highcut / (0.5 * fs)
-    ord = buttord(high, low, 2, 40)
-    b, a = butter(2, [low, high], btype='band')
-    zi = np.zeros([a.shape[0] - 1, num_ch])
-    return b, a, zi
-
-
-def list_lsl_streams(logger=logger, ignore_markers=False):
-    """
-    List available LSL streams found on network
-    """
-    import time
-
-    # look for LSL servers
-    amp_list = []
-    amp_list_backup = []
-
-    while True:
-        streamInfos = pylsl.resolve_streams()
-        if len(streamInfos) > 0:
-            for index, si in enumerate(streamInfos):
-                # LSL XML parser has a bug which crashes so do not use for now
-                #desc = pylsl.StreamInlet(si).info().desc()
-                #amp_serial = desc.child('acquisition').child_value('serial_number').strip()
-                amp_serial = 'N/A' # serial number not supported yet
-                amp_name = si.name()
-                if 'Markers' in amp_name:
-                    amp_list_backup.append((index, amp_name, amp_serial))
-                else:
-                    amp_list.append((index, amp_name, amp_serial))
-            break
-        logger.info('No server available yet on the network...')
-        time.sleep(1)
-
-    if ignore_markers is False:
-        amp_list += amp_list_backup
-
-    logger.info('-- List of servers --')
-    for i, (index, amp_name, amp_serial) in enumerate(amp_list):
-        if amp_serial == '':
-            amp_ser = 'N/A'
-        else:
-            amp_ser = amp_serial
-        logger.info('%d: %s (Serial %s)' % (i, amp_name, amp_ser))
-
-    return amp_list, streamInfos
-
-
-
-def search_lsl(logger=logger, ignore_markers=False):
-    #  Find avaiable LSL streams
-    amp_list, streamInfos = list_lsl_streams(logger, ignore_markers)
-
-    if len(amp_list) == 1:
-        index = 0
-    else:
-        index = input('Amp index? Hit enter without index to select the first server.\n>> ')
-        if index.strip() == '':
-            index = 0
-        else:
-            index = int(index.strip())
-    amp_index, amp_name, amp_serial = amp_list[index]
-    si = streamInfos[amp_index]
-    assert amp_name == si.name()
-    # LSL XML parser has a bug which crashes so do not use for now
-    #assert amp_serial == pylsl.StreamInlet(si).info().desc().child('acquisition').child_value('serial_number').strip()
-    logger.info('Selected %s (Serial: %s)' % (amp_name, amp_serial))
-
-    return amp_name, amp_serial
-
-def lsl_channel_list(inlet):
-    """
-    Reads XML description of LSL header and returns channel list
-
-    Input:
-        pylsl.StreamInlet object
-    Returns:
-        ch_list: [ name1, name2, ... ]
-    """
-    if not type(inlet) is pylsl.StreamInlet:
-        logger.error('lsl_channel_list(): wrong input type %s' % type(inlet))
-        raise TypeError
-    root = ET.fromstring(inlet.info().as_xml())
-    desc = root.find('desc')
-    ch_list = []
-    for ch in list(desc.find('channels')):
-        ch_name = ch.find('label').text
-        ch_list.append(ch_name)
-
-    ''' This code may throw access violation error due to bug in pylsl.XMLElement
-    # for some reason type(inlet) returns 'instance' type in Python 2.
-    ch = inlet.info().desc().child('channels').first_child()
-    ch_list = []
-    for k in range(inlet.info().channel_count()):
-        ch_name = ch.child_value('label')
-        ch_list.append(ch_name)
-        ch = ch.next_sibling()
-    '''
-    return ch_list
-
-
-def channel_names_to_index(raw, channel_names=None):
-    """
-    Return channel indicies among EEG channels
-    """
-    if channel_names is None:
-        picks = mne.pick_types(raw.info, meg=False, eeg=True, stim=False, eog=False, exclude='bads')
-    else:
-        picks = []
-        for c in channel_names:
-            if type(c) == int:
-                picks.append(c)
-            elif type(c) == str:
-                if c not in raw.ch_names:
-                    raise IndexError('Channel %s not found in raw.ch_names' % c)
-                picks.append(raw.ch_names.index(c))
-            else:
-                raise TypeError('channel_names is unknown format.\nchannel_names=%s' % channel_names)
-
-    return picks
-
-
-def raw_crop(raw, tmin, tmax):
-    """
-    Perform a real cropping of a Raw object
-
-    mne.Raw.crop() updates a very confusing variable "first_samp", which reuslts
-    in the mismatch of real event indices when run with mne.find_events().
-    """
-    trigch = find_event_channel(raw)
-    ch_types = ['eeg'] * len(raw.ch_names)
-    if trigch is not None:
-        ch_types[trigch] = 'stim'
-    info = mne.create_info(raw.ch_names, raw.info['sfreq'], ch_types)
-    tmin_index = int(round(raw.info['sfreq'] * tmin))
-    tmax_index = int(round(raw.info['sfreq'] * tmax))
-    return mne.io.RawArray(raw._data[:, tmin_index:tmax_index], info)
-
-
-def load_config(cfg_module):
-    cfg_module = cfg_module.replace('\\', '/')
-    if '/' in cfg_module:
-        spec = importlib.util.spec_from_file_location(qc.parse_path(cfg_module).name, cfg_module)
-        cfg = importlib.util.module_from_spec(spec)
-        spec.loader.exec_module(cfg)
-    else:
-        cfg = importlib.import_module(cfg_module)
-        importlib.reload(cfg) # in case cfg_module was dynamically changed
-    logger.info('Loaded config %s' % cfg_module)
-    return cfg
+from __future__ import print_function, division
+
+"""
+PyCNBI utility functions
+
+Note:
+When exporting to Panda Dataframes format, raw.as_data_frame() silently
+scales data to the Volts unit by default, which is the convention in MNE.
+Try raw.as_data_frame(scalings=dict(eeg=1.0, misc=1.0))
+
+Kyuhwa Lee, 2014
+Swiss Federal Institute of Technology Lausanne (EPFL)
+
+"""
+
+import os
+import sys
+import mne
+import pylsl
+import scipy.io
+import importlib
+import numpy as np
+import multiprocessing as mp
+import xml.etree.ElementTree as ET
+import neurodecode.utils.q_common as qc
+from scipy.signal import butter, lfilter, lfiltic, buttord
+from neurodecode.pycnbi_config import CAP, LAPLACIAN
+from neurodecode import logger
+from builtins import input
+
+mne.set_log_level('ERROR')
+os.environ['OMP_NUM_THREADS'] = '1' # actually improves performance for multitaper
+
+
+# note that MNE already has find_events function
+def find_events(events_raw):
+    """
+    Find trigger values, rising from zero to non-zero
+    """
+    events = []  # triggered event values other than zero
+
+    # set epochs (frame start, frame end)
+    ev_last = 0
+    for et in range(len(events_raw)):
+        ev = events_raw[et]
+        if ev != ev_last:
+            if ev > 0:
+                events.append([et, 0, ev])
+            ev_last = ev
+
+    return events
+
+
+def find_event_channel(raw=None, ch_names=None):
+    """
+    Find event channel using heuristics for pcl files.
+
+    Disclaimer: Not 100% guaranteed to find.
+
+    Input:
+        raw: mne.io.RawArray-like object or numpy array (n_channels x n_samples)
+        if raw is None, ch_names must be given.
+
+    Output:
+        channel index or None if not found.
+    """
+
+    if type(raw) == np.ndarray:
+        if ch_names is not None:
+            for ch_name in ch_names:
+                if 'TRIGGER' in ch_name or 'STI ' in ch_name or 'TRG' in ch_name or 'CH_Event' in ch_name:
+                    return ch_names.index(ch_name)
+
+        # data range between 0 and 255 and all integers?
+        for ch in range(raw.shape[0]):
+            if (raw[ch].astype(int) == raw[ch]).all()\
+                    and max(raw[ch]) < 256 and min(raw[ch]) == 0:
+                return ch
+    elif hasattr(raw, 'ch_names'):
+        for ch_name in raw.ch_names:
+            if 'TRIGGER' in ch_name or 'STI ' in ch_name or 'TRG' in ch_name or 'CH_Event' in ch_name:
+                return raw.ch_names.index(ch_name)
+    else:
+        if ch_names is None:
+            raise ValueError('ch_names cannot be None when raw is None.')
+        for ch_name in ch_names:
+            if 'TRIGGER' in ch_name or 'STI ' in ch_name or 'TRG' in ch_name or 'CH_Event' in ch_name:
+                return ch_names.index(ch_name)
+    return None
+
+
+def raw2mat(infile, outfile):
+    '''
+    Convert raw data file to MATLAB file
+    '''
+    raw, events = load_raw(infile)
+    header = dict(bads=raw.info['bads'], ch_names=raw.info['ch_names'],\
+                  sfreq=raw.info['sfreq'], events=events)
+    scipy.io.savemat(outfile, dict(signals=raw._data, header=header))
+    logger.info('Exported to %s' % outfile)
+
+
+def add_events_raw(rawfile, outfile, eventfile, overwrite=True):
+    """
+    Add events from a file and save
+
+    Note: If the event values already exists in raw file, the new event values
+        will be added to the previous value instead of replacing them.
+    """
+
+    raw = mne.io.Raw(rawfile, preload=True, proj=False)
+    events = mne.read_events(eventfile)
+    raw.add_events(events, stim_channel='TRIGGER')
+    raw.save(outfile, overwrite=overwrite)
+
+
+def export_morlet(epochs, filename):
+    """
+    Export wavelet tranformation decomposition into Matlab format
+    """
+    freqs = np.array(DWT['freqs'])  # define frequencies of interest
+    n_cycles = freqs / 2.  # different number of cycle per frequency
+    power, itc = mne.time_frequency.tfr_morlet(epochs, freqs=freqs,
+        n_cycles=n_cycles, use_fft=False, return_itc=True, n_jobs=mp.cpu_count())
+    scipy.io.savemat(filename, dict(power=power.data, itc=itc.data, freqs=freqs,
+        channels=epochs.ch_names, sfreq=epochs.info['sfreq'], onset=-epochs.tmin))
+
+
+def event_timestamps_to_indices(sigfile, eventfile):
+    """
+    Convert LSL timestamps to sample indices for separetely recorded events.
+
+    Parameters:
+    sigfile: raw signal file (Python Pickle) recorded with stream_recorder.py.
+    eventfile: event file where events are indexed with LSL timestamps.
+
+    Returns:
+    events list, which can be used as an input to mne.io.RawArray.add_events().
+    """
+
+    raw = qc.load_obj(sigfile)
+    ts = raw['timestamps'].reshape(-1)
+    ts_min = min(ts)
+    ts_max = max(ts)
+    events = []
+
+    with open(eventfile) as f:
+        for l in f:
+            data = l.strip().split('\t')
+            event_ts = float(data[0])
+            event_value = int(data[2])
+            # find the first index not smaller than ts
+            next_index = np.searchsorted(ts, event_ts)
+            if next_index >= len(ts):
+                logger.warning('Event %d at time %.3f is out of time range (%.3f - %.3f).' % (event_value, event_ts, ts_min, ts_max))
+            else:
+                events.append([next_index, 0, event_value])
+    return events
+
+
+def rereference(raw, ref_new, ref_old=None):
+    """
+    Reference to new channels. raw object is modified in-place for efficiency.
+
+    raw: mne.io.RawArray
+
+    ref_new: None | list of str (RawArray) | list of int (numpy array)
+        Channel(s) to re-reference, e.g. M1, M2.
+        Average of these channel values are substracted from all channel values.
+
+    ref_old: None | str
+        Channel to recover, assuming this channel was originally used as a reference.
+    """
+
+    # Re-reference and recover the original reference channel values if possible
+    if type(raw) == np.ndarray:
+        if raw_ch_old is not None:
+            logger.error('Recovering original reference channel is not yet supported for numpy arrays.')
+            raise NotImplementedError
+        if type(raw_ch_new[0]) is not int:
+            logger.error('Channels must be integer values for numpy arrays')
+            raise ValueError
+        raw -= np.mean(raw[ref_new], axis=0)
+    else:
+        if ref_old is not None:
+            # Add a blank (zero-valued) channel
+            mne.io.add_reference_channels(raw, ref_old, copy=False)
+        # Re-reference
+        mne.io.set_eeg_reference(raw, ref_new, copy=False)
+
+    return True
+
+
+def preprocess(raw, sfreq=None, spatial=None, spatial_ch=None, spectral=None, spectral_ch=None,
+               notch=None, notch_ch=None, multiplier=1, ch_names=None, rereference=None, decim=None, n_jobs=1):
+    """
+    Apply spatial, spectral, notch filters and convert unit.
+    raw is modified in-place.
+
+    Input
+    ------
+    raw: mne.io.Raw | mne.io.RawArray | mne.Epochs | numpy.array (n_channels x n_samples)
+         numpy.array type assumes the data has only pure EEG channnels without event channels
+
+    sfreq: required only if raw is numpy array.
+
+    spatial: None | 'car' | 'laplacian'
+        Spatial filter type.
+
+    spatial_ch: None | list (for CAR) | dict (for LAPLACIAN)
+        Reference channels for spatial filtering. May contain channel names.
+        'car': channel indices used for CAR filtering. If None, use all channels except
+               the trigger channel (index 0).
+        'laplacian': {channel:[neighbor1, neighbor2, ...], ...}
+        (Note) since Neurodecode puts trigger channel as index 0, data channel starts from index 1.
+
+    spectral: None | [l_freq, h_freq]
+        Spectral filter.
+        if l_freq is None: lowpass filter is applied.
+        if h_freq is None: highpass filter is applied.
+        if l_freq < h_freq: bandpass filter is applied.
+        if l_freq > h_freq: band-stop filter is applied.
+
+    spectral_ch: None | list
+        Channel picks for spectra filtering. May contain channel names.
+
+    notch: None | float | list of frequency in floats
+        Notch filter.
+
+    notch_ch: None | list
+        Channel picks for notch filtering. May contain channel names.
+
+    multiplier: float
+        If not 1, multiply data values excluding trigger values.
+
+    ch_names: None | list
+        If raw is numpy array and channel picks are list of strings, ch_names will
+        be used as a look-up table to convert channel picks to channel numbers.
+
+    rereference: Not supported yet.
+
+    decim: None | int
+        Apply low-pass filter and decimate (downsample). sfreq must be given. Ignored if 1.
+
+    Output
+    ------
+    Same input data structure.
+
+    Note: To save computation time, input data may be modified in-place.
+    TODO: Add an option to disable in-place modification.
+    """
+
+    # Check datatype
+    if type(raw) == np.ndarray:
+        # Numpy array: assume we don't have event channel
+        data = raw
+        assert sfreq is not None and sfreq > 0, 'Wrong sfreq value.'
+        assert 2 <= len(data.shape) <= 3, 'Unknown data shape. The dimension must be 2 or 3.'
+        if len(data.shape) == 3:
+            n_channels = data.shape[1]
+        elif len(data.shape) == 2:
+            n_channels = data.shape[0]
+        eeg_channels = list(range(n_channels))
+        if decim is not None and decim != 1:
+            if sfreq is None:
+                logger.error('Decimation cannot be applied if sfreq is None.')
+                raise ValueError
+    else:
+        # MNE Raw object: exclude event channel
+        ch_names = raw.ch_names
+        data = raw._data
+        sfreq = raw.info['sfreq']
+        assert 2 <= len(data.shape) <= 3, 'Unknown data shape. The dimension must be 2 or 3.'
+        if len(data.shape) == 3:
+            # assert type(raw) is mne.epochs.Epochs
+            n_channels = data.shape[1]
+        elif len(data.shape) == 2:
+            n_channels = data.shape[0]
+        eeg_channels = list(range(n_channels))
+        tch = find_event_channel(raw)
+        if tch is None:
+            logger.warning('No trigger channel found. Using all channels.')
+        else:
+            tch_name = ch_names[tch]
+            eeg_channels.pop(tch)
+
+    # Re-reference channels
+    if rereference is not None:
+        logger.error('re-referencing not implemented yet. Sorry.')
+        raise NotImplementedError
+
+    # Do unit conversion
+    if multiplier != 1:
+        data[eeg_channels] *= multiplier
+
+    # Apply spatial filter
+    if spatial is None:
+        pass
+    elif spatial == 'car':
+        if spatial_ch is None:
+            spatial_ch = eeg_channels
+
+        if type(spatial_ch[0]) == str:
+            assert ch_names is not None, 'preprocess(): ch_names must not be None'
+            spatial_ch_i = [ch_names.index(c) for c in spatial_ch]
+        else:
+            spatial_ch_i = spatial_ch
+
+        if len(spatial_ch_i) > 1:
+            if len(data.shape) == 2:
+                data[spatial_ch_i] -= np.mean(data[spatial_ch_i], axis=0)
+            elif len(data.shape) == 3:
+                means = np.mean(data[:, spatial_ch_i, :], axis=1)
+                data[:, spatial_ch_i, :] -= means[:, np.newaxis, :]
+            else:
+                logger.error('Unknown data shape %s' % str(data.shape))
+                raise ValueError
+    elif spatial == 'laplacian':
+        if type(spatial_ch) is not dict:
+            logger.error('preprocess(): For Lapcacian, spatial_ch must be of form {CHANNEL:[NEIGHBORS], ...}')
+            raise TypeError
+        if type(spatial_ch.keys()[0]) == str:
+            spatial_ch_i = {}
+            for c in spatial_ch:
+                ref_ch = ch_names.index(c)
+                spatial_ch_i[ref_ch] = [ch_names.index(n) for n in spatial_ch[c]]
+        else:
+            spatial_ch_i = spatial_ch
+
+        if len(spatial_ch_i) > 1:
+            rawcopy = data.copy()
+            for src in spatial_ch:
+                nei = spatial_ch[src]
+                if len(data.shape) == 2:
+                    data[src] = rawcopy[src] - np.mean(rawcopy[nei], axis=0)
+                elif len(data.shape) == 3:
+                    data[:, src, :] = rawcopy[:, src, :] - np.mean(rawcopy[:, nei, :], axis=1)
+                else:
+                    logger.error('preprocess(): Unknown data shape %s' % str(data.shape))
+                    raise ValueError
+    else:
+        logger.error('preprocess(): Unknown spatial filter %s' % spatial)
+        raise ValueError
+
+    # Downsample
+    if decim is not None and decim != 1:
+        if type(raw) == np.ndarray:
+            data = mne.filter.resample(data, down=decim, npad='auto', window='boxcar', n_jobs=1)
+        else:
+            # resample() of Raw* and Epochs object internally calls mne.filter.resample()
+            raw = raw.resample(raw.info['sfreq'] / decim, npad='auto', window='boxcar', n_jobs=1)
+            data = raw._data
+        sfreq /= decim
+
+    # Apply spectral filter
+    if spectral is not None:
+        if spectral_ch is None:
+            spectral_ch = eeg_channels
+
+        if type(spectral_ch[0]) == str:
+            assert ch_names is not None, 'preprocess(): ch_names must not be None'
+            spectral_ch_i = [ch_names.index(c) for c in spectral_ch]
+        else:
+            spectral_ch_i = spectral_ch
+
+        # fir_design='firwin' is especially important for ICA analysis. See:
+        # http://martinos.org/mne/dev/generated/mne.preprocessing.ICA.html?highlight=score_sources#mne.preprocessing.ICA.score_sources
+        mne.filter.filter_data(data, sfreq, spectral[0], spectral[1], picks=spectral_ch_i,
+            filter_length='auto', l_trans_bandwidth='auto',
+            h_trans_bandwidth='auto', n_jobs=n_jobs, method='fir',
+            iir_params=None, copy=False, phase='zero',
+            fir_window='hamming', fir_design='firwin', verbose='ERROR')
+
+    # Apply notch filter
+    if notch is not None:
+        if notch_ch is None:
+            notch_ch = eeg_channels
+
+        if type(notch_ch[0]) == str:
+            assert ch_names is not None, 'preprocess(): ch_names must not be None'
+            notch_ch_i = [ch_names.index(c) for c in notch_ch]
+        else:
+            notch_ch_i = notch_ch
+
+        mne.filter.notch_filter(data, Fs=sfreq, freqs=notch, notch_widths=5,
+                                picks=notch_ch_i, method='fft', n_jobs=n_jobs, copy=False)
+
+    if type(raw) == np.ndarray:
+        raw = data
+    return raw
+
+
+def load_raw(rawfile, spfilter=None, spchannels=None, events_ext=None, multiplier=1, verbose='ERROR'):
+    """
+    Loads data from a fif-format file.
+    You can convert non-fif files (.eeg, .bdf, .gdf, .pcl) to fif format.
+
+    Parameters:
+    rawfile: (absolute) data file path
+    spfilter: 'car' | 'laplacian' | None
+    spchannels: None | list (for CAR) | dict (for LAPLACIAN)
+        'car': channel indices used for CAR filtering. If None, use all channels except
+               the trigger channel (index 0).
+        'laplacian': {channel:[neighbor1, neighbor2, ...], ...}
+        *** Note ***
+        Since PyCNBI puts trigger channel as index 0, data channel starts from index 1.
+    events_ext: Add externally recorded events.
+                [ [sample_index1, 0, event_value1],... ]
+    multiplier: Multiply all values except triggers (to convert unit).
+
+    Returns:
+    raw: mne.io.RawArray object. First channel (index 0) is always trigger channel.
+    events: mne-compatible events numpy array object (N x [frame, 0, type])
+    spfilter= {None | 'car' | 'laplacian'}
+
+    """
+
+    if not os.path.exists(rawfile):
+        logger.error('File %s not found' % rawfile)
+        raise IOError
+    if not os.path.isfile(rawfile):
+        logger.error('%s is not a file' % rawfile)
+        raise IOError
+
+    extension = qc.parse_path(rawfile).ext
+    assert extension in ['fif', 'fiff'], 'only fif format is supported'
+    raw = mne.io.Raw(rawfile, preload=True, verbose=verbose)
+    if spfilter is not None or multiplier != 1:
+        preprocess(raw, spatial=spfilter, spatial_ch=spchannels, multiplier=multiplier)
+    if events_ext is not None:
+        events = mne.read_events(events_ext)
+    else:
+        tch = find_event_channel(raw)
+        if tch is not None:
+            events = mne.find_events(raw, stim_channel=raw.ch_names[tch], shortest_event=1,
+                uint_cast=True, consecutive='increasing', output='onset', initial_event=True)
+            # some of MNE's functions do not correctly update first_samp, especially Raw.crop() function
+            events[:, 0] -= raw.first_samp
+        else:
+            events = np.array([], dtype=np.int64)
+
+    return raw, events
+
+
+def load_multi(src, spfilter=None, spchannels=None, multiplier=1):
+    """
+    Load multiple data files and concatenate them into a single series
+
+    - Assumes all files have the same sampling rate and channel order.
+    - Event locations are updated accordingly with new offset.
+
+    @params:
+        src: directory or list of files.
+        spfilter: apply spatial filter while loading.
+        spchannels: list of channel names to apply spatial filter.
+        multiplier: to change units for better numerical stability.
+
+    See load_raw() for more low-level details.
+
+    """
+
+    if type(src) == str:
+        if not os.path.isdir(src):
+            logger.error('%s is not a directory or does not exist.' % src)
+            raise IOError
+        flist = []
+        for f in qc.get_file_list(src):
+            if qc.parse_path_list(f)[2] == 'fif':
+                flist.append(f)
+    elif type(src) in [list, tuple]:
+        flist = src
+    else:
+        logger.error('Unknown input type %s' % type(src))
+        raise TypeError
+
+    if len(flist) == 0:
+        logger.error('load_multi(): No fif files found in %s.' % src)
+        raise RuntimeError
+    elif len(flist) == 1:
+        return load_raw(flist[0], spfilter=spfilter, spchannels=spchannels, multiplier=multiplier)
+
+    # load raw files
+    rawlist = []
+    for f in flist:
+        logger.info('Loading %s' % f)
+        raw, _ = load_raw(f, spfilter=spfilter, spchannels=spchannels, multiplier=multiplier)
+        rawlist.append(raw)
+
+    # concatenate signals
+    signals = None
+    for raw in rawlist:
+        if signals is None:
+            signals = raw._data
+        else:
+            signals = np.concatenate((signals, raw._data), axis=1) # append samples
+
+    # create a concatenated raw object and update channel names
+    raw = rawlist[0]
+    trigch = find_event_channel(raw)
+    ch_types = ['eeg'] * len(raw.ch_names)
+    if trigch is not None:
+        ch_types[trigch] = 'stim'
+    info = mne.create_info(raw.ch_names, raw.info['sfreq'], ch_types)
+    raw_merged = mne.io.RawArray(signals, info)
+
+    # re-calculate event positions
+    events = mne.find_events(raw_merged, stim_channel='TRIGGER', shortest_event=1,
+        uint_cast=True, consecutive='increasing', output='onset', initial_event=True)
+
+    return raw_merged, events
+
+
+def butter_bandpass(highcut, lowcut, fs, num_ch):
+    """
+    Calculation of bandpass coefficients.
+    Order is computed automatically.
+    Note that if filter is unstable this function crashes.
+
+    TODO: handle exceptions
+    """
+
+    low = lowcut / (0.5 * fs)
+    high = highcut / (0.5 * fs)
+    ord = buttord(high, low, 2, 40)
+    b, a = butter(2, [low, high], btype='band')
+    zi = np.zeros([a.shape[0] - 1, num_ch])
+    return b, a, zi
+
+
+def list_lsl_streams(logger=logger, ignore_markers=False):
+    """
+    List available LSL streams found on network
+    """
+    import time
+
+    # look for LSL servers
+    amp_list = []
+    amp_list_backup = []
+
+    while True:
+        streamInfos = pylsl.resolve_streams()
+        if len(streamInfos) > 0:
+            for index, si in enumerate(streamInfos):
+                # LSL XML parser has a bug which crashes so do not use for now
+                #desc = pylsl.StreamInlet(si).info().desc()
+                #amp_serial = desc.child('acquisition').child_value('serial_number').strip()
+                amp_serial = 'N/A' # serial number not supported yet
+                amp_name = si.name()
+                if 'Markers' in amp_name:
+                    amp_list_backup.append((index, amp_name, amp_serial))
+                else:
+                    amp_list.append((index, amp_name, amp_serial))
+            break
+        logger.info('No server available yet on the network...')
+        time.sleep(1)
+
+    if ignore_markers is False:
+        amp_list += amp_list_backup
+
+    logger.info('-- List of servers --')
+    for i, (index, amp_name, amp_serial) in enumerate(amp_list):
+        if amp_serial == '':
+            amp_ser = 'N/A'
+        else:
+            amp_ser = amp_serial
+        logger.info('%d: %s (Serial %s)' % (i, amp_name, amp_ser))
+
+    return amp_list, streamInfos
+
+
+
+def search_lsl(logger=logger, ignore_markers=False):
+    #  Find avaiable LSL streams
+    amp_list, streamInfos = list_lsl_streams(logger, ignore_markers)
+
+    if len(amp_list) == 1:
+        index = 0
+    else:
+        index = input('Amp index? Hit enter without index to select the first server.\n>> ')
+        if index.strip() == '':
+            index = 0
+        else:
+            index = int(index.strip())
+    amp_index, amp_name, amp_serial = amp_list[index]
+    si = streamInfos[amp_index]
+    assert amp_name == si.name()
+    # LSL XML parser has a bug which crashes so do not use for now
+    #assert amp_serial == pylsl.StreamInlet(si).info().desc().child('acquisition').child_value('serial_number').strip()
+    logger.info('Selected %s (Serial: %s)' % (amp_name, amp_serial))
+
+    return amp_name, amp_serial
+
+def lsl_channel_list(inlet):
+    """
+    Reads XML description of LSL header and returns channel list
+
+    Input:
+        pylsl.StreamInlet object
+    Returns:
+        ch_list: [ name1, name2, ... ]
+    """
+    if not type(inlet) is pylsl.StreamInlet:
+        logger.error('lsl_channel_list(): wrong input type %s' % type(inlet))
+        raise TypeError
+    root = ET.fromstring(inlet.info().as_xml())
+    desc = root.find('desc')
+    ch_list = []
+    for ch in list(desc.find('channels')):
+        ch_name = ch.find('label').text
+        ch_list.append(ch_name)
+
+    ''' This code may throw access violation error due to bug in pylsl.XMLElement
+    # for some reason type(inlet) returns 'instance' type in Python 2.
+    ch = inlet.info().desc().child('channels').first_child()
+    ch_list = []
+    for k in range(inlet.info().channel_count()):
+        ch_name = ch.child_value('label')
+        ch_list.append(ch_name)
+        ch = ch.next_sibling()
+    '''
+    return ch_list
+
+
+def channel_names_to_index(raw, channel_names=None):
+    """
+    Return channel indicies among EEG channels
+    """
+    if channel_names is None:
+        picks = mne.pick_types(raw.info, meg=False, eeg=True, stim=False, eog=False, exclude='bads')
+    else:
+        picks = []
+        for c in channel_names:
+            if type(c) == int:
+                picks.append(c)
+            elif type(c) == str:
+                if c not in raw.ch_names:
+                    raise IndexError('Channel %s not found in raw.ch_names' % c)
+                picks.append(raw.ch_names.index(c))
+            else:
+                raise TypeError('channel_names is unknown format.\nchannel_names=%s' % channel_names)
+
+    return picks
+
+
+def raw_crop(raw, tmin, tmax):
+    """
+    Perform a real cropping of a Raw object
+
+    mne.Raw.crop() updates a very confusing variable "first_samp", which reuslts
+    in the mismatch of real event indices when run with mne.find_events().
+    """
+    trigch = find_event_channel(raw)
+    ch_types = ['eeg'] * len(raw.ch_names)
+    if trigch is not None:
+        ch_types[trigch] = 'stim'
+    info = mne.create_info(raw.ch_names, raw.info['sfreq'], ch_types)
+    tmin_index = int(round(raw.info['sfreq'] * tmin))
+    tmax_index = int(round(raw.info['sfreq'] * tmax))
+    return mne.io.RawArray(raw._data[:, tmin_index:tmax_index], info)
+
+
+def load_config(cfg_module):
+    cfg_module = cfg_module.replace('\\', '/')
+    if '/' in cfg_module:
+        spec = importlib.util.spec_from_file_location(qc.parse_path(cfg_module).name, cfg_module)
+        cfg = importlib.util.module_from_spec(spec)
+        spec.loader.exec_module(cfg)
+    else:
+        cfg = importlib.import_module(cfg_module)
+        importlib.reload(cfg) # in case cfg_module was dynamically changed
+    logger.info('Loaded config %s' % cfg_module)
+    return cfg
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/q_common.py` & `neurodecode-2.0.5/neurodecode/utils/q_common.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,770 +1,770 @@
-from __future__ import print_function, division
-
-"""
-Useful Python utilities
-
-Author: Kyuhwa Lee
-Imperial College of Science, Technology and Medicine
-
-"""
-
-# set Q_VERBOSE= 0 to make it silent. 1:verbose, 2:extra verbose
-Q_VERBOSE = 0
-
-
-import os
-import sys
-import pdb
-import code
-import time
-import math
-import mat73
-import scipy.io
-import shutil
-import logging
-import inspect
-import traceback
-import itertools
-import numpy as np
-import sklearn.metrics
-import matplotlib.pyplot as plt
-
-# logger
-try:
-    from neurodecode import logger
-except ImportError:
-    logging.basicConfig(format='%(msg)s', level='INFO')
-    logger = logging.getLogger(__name__)
-    logger.propagate = False
-
-# pickle
-try:
-    import cPickle as pickle  # Python 2 (cPickle = C version of pickle)
-except ImportError:
-    import pickle  # Python 3 (C version is the default)
-
-
-'''"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
- Math
-"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""'''
-
-def sigmoid(x):
-    return 1 / (1 + math.exp(-x))
-
-def sigmoid_array(x):
-    return 1 / (1 + np.exp(-x))
-
-def dirichlet(n):
-    """
-    Uniform Dirichlet distribution with sigma(alpha)=1.0
-    """
-    alpha = 1.0 / n
-    return 1 / beta(alpha, n) * ((1 / n) ** (alpha - 1)) ** n
-
-def beta(alpha, n):
-    """
-    Multinomial Beta function with uniform alpha values
-
-    n: number of rule probabilities
-    """
-    return math.gamma(alpha) ** n / math.gamma(n * alpha)
-
-def poisson(mean, k):
-    """
-    Poisson distribution. We use k-1 since the minimum length is 1, not 0.
-    """
-    return (mean ** (k - 1) * math.exp(-mean)) / math.factorial(k - 1)
-
-def average_every_n(arr, n):
-    """
-    Average every n elements of a numpy array
-
-    if not len(arr) % n == 0, it will be trimmed to the closest divisible length
-    """
-    end = n * int(len(arr) / n)
-    return np.mean(arr[:end].reshape(-1, n), 1)
-
-def zscore_mod(X, axis=0):
-    """
-    Modified z-score for multidimensional arrays
-
-    MAD = median(abs(X-median(X)))
-    MeanAD = mean(abs(X-mean(X)))
-    If MAD does equal 0 (if at least 50% of samples have the same value)
-      Subtract the median from the score and divide by 1.253314*MeanAD.
-      1.253314*MeanAD approximately equals the standard deviation.
-    If MAD does not equal 0
-      Subtract the median from the score and divide by 1.486*MAD.
-      1.486*MAD approximately equals the standard deviation.
-
-    Reference:
-    https://www.ibm.com/docs/en/cognos-analytics/11.1.0?topic=terms-modified-z-score
-    """
-    # medians are computed for each trial for each feature
-    X_med = np.median(X, axis=axis)
-    # expand dimension for broadcasting
-    X_med_diff = X - np.expand_dims(X_med, axis=axis)
-    # compute MAD
-    X_mad = np.median(np.abs(X_med_diff), axis=axis)
-
-    if X_mad.all():
-        # if all MADs are non-zero
-        X_norm = X_med_diff / (1.486 * np.expand_dims(X_mad, axis))
-    else:
-        # compute MeanAD
-        X_mean = np.mean(X, axis=axis)
-        X_mean_ad = np.mean(abs(X - np.expand_dims(X_mean, axis=axis)), axis=axis)
-        X_mad_corrected = X_mad * 1.486
-        # replace 0 in MAD with the corresponding meanAD value
-        for zero_loc in np.array(np.where(X_mad==0)).T:
-            zero_loc = tuple(zero_loc) # every index containing 0 in MAD
-            X_mad_corrected[zero_loc] = 1.253314 * X_mean_ad[zero_loc]
-        X_norm = X_med_diff / np.expand_dims(X_mad_corrected, axis)
-    return X_norm
-
-
-'''"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
- List/Dict related
-"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""'''
-
-def list2string(vec, fmt, sep=' '):
-    """
-    Convert a list to string with formatting, separated by sep (default is space).
-    Example: fmt= '%.32e', '%.6f', etc.
-    """
-    return sep.join((fmt % x for x in vec))
-
-def flatten_list(l):
-    return list(itertools.chain.from_iterable(l))
-
-def get_index_min(seq):
-    """
-    Get the index of the minimum item in a list or dict
-    """
-    if type(seq) == list:
-        return min(range(len(seq)), key=seq.__getitem__)
-    elif type(seq) == dict:
-        return min(seq, key=seq.__getitem__)
-    else:
-        logger.error('Unsupported input %s' % type(seq))
-        return None
-
-def get_index_max(seq):
-    """
-    Get the index of the maximum item in a list or dict
-    """
-    if type(seq) == list:
-        return max(range(len(seq)), key=seq.__getitem__)
-    elif type(seq) == dict:
-        return max(seq, key=seq.__getitem__)
-    else:
-        logger.error('Unsupported input %s' % type(seq))
-        return None
-
-def sort_by_value(s, rev=False):
-    """
-    Sort dictionary or list by value and return a sorted list of keys and values.
-    Values must be hashable and unique.
-    """
-    assert type(s) == dict or type(s) == list, 'Input must be a dictionary or list.'
-    if type(s) == list:
-        s = dict(enumerate(s))
-    s_rev = dict((v, k) for k, v in s.items())
-    if Q_VERBOSE > 0 and not len(s_rev) == len(s):
-        logger.warning('sort_by_value(): %d identical values' % (len(s.values()) - len(set(s.values())) + 1))
-    values = sorted(s_rev, reverse=rev)
-    keys = [s_rev[x] for x in values]
-    return keys, values
-
-
-'''"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
- File I/O
-"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""'''
-
-def get_file_list(path, fullpath=True, recursive=False):
-    """
-    Get files with or without full path.
-    """
-    path = path.replace('\\', '/')
-    if not path[-1] == '/': path += '/'
-
-    if recursive == False:
-        if fullpath == True:
-            filelist = [path + f for f in os.listdir(path) if os.path.isfile(path + '/' + f) and f[0] != '.']
-        else:
-            filelist = [f for f in os.listdir(path) if os.path.isfile(path + '/' + f) and f[0] != '.']
-    else:
-        filelist = []
-        for root, dirs, files in os.walk(path):
-            root = root.replace('\\', '/')
-            if fullpath == True:
-                [filelist.append(root + '/' + f) for f in files]
-            else:
-                [filelist.append(f) for f in files]
-    return sorted(filelist)
-
-def get_dir_list(path, recursive=False, no_child=False):
-    """
-    Get directory list relative to path.
-
-    Input:
-        recusrive: search recursively if True.
-        no_child: search directories having no child directory (leaf nodes)
-    """
-    path = path.replace('\\', '/')
-    if not path[-1] == '/': path += '/'
-
-    if recursive == True:
-        pathlist = []
-        for root, dirs, files in os.walk(path):
-            root = root.replace('\\', '/')
-            [pathlist.append(root + '/' + d) for d in dirs]
-
-            if no_child:
-                for p in pathlist:
-                    if len(get_dir_list(p)) > 0:
-                        pathlist.remove(p)
-
-    else:
-        pathlist = [path + f for f in os.listdir(path) if os.path.isdir(path + '/' + f)]
-        if no_child:
-            for p in pathlist:
-                if len(get_dir_list(p)) > 0:
-                    pathlist.remove(p)
-
-    return sorted(pathlist)
-
-def make_dirs(dirname, delete=False):
-    """
-    Recusively create directories.
-    if delete=true, directory will be deleted first if exists.
-    """
-    if os.path.exists(dirname) and delete == True:
-        try:
-            shutil.rmtree(dirname)
-        except OSError:
-            logger.error('Directory was not completely removed. (Perhaps a Dropbox folder?). Continuing.')
-    if not os.path.exists(dirname):
-        os.makedirs(dirname)
-
-def save_obj(fname, obj, protocol=4):
-    """
-    Save python object into a file
-    Set protocol=2 for Python 2 compatibility
-    """
-    with open(fname, 'wb') as fout:
-        pickle.dump(obj, fout, protocol)
-
-def load_obj(fname):
-    """
-    Read python object from a file
-    """
-    try:
-        with open(fname, 'rb') as f:
-            return pickle.load(f)
-    except UnicodeDecodeError:
-        # usually happens when trying to load Python 2 pickle object from Python 3
-        with open(fname, 'rb') as f:
-            return pickle.load(f, encoding='latin1')
-    except:
-        msg = 'load_obj(): Cannot load pickled object file "%s". The error was:\n%s\n%s' %\
-              (fname, sys.exc_info()[0], sys.exc_info()[1])
-        raise IOError(msg)
-
-def loadtxt_fast(filename, delimiter=',', skiprows=0, dtype=float):
-    """
-    Much faster matrix loading than numpy's loadtxt
-    http://stackoverflow.com/a/8964779
-    """
-    def iter_func():
-        with open(filename, 'r') as infile:
-            for _ in range(skiprows):
-                next(infile)
-            for line in infile:
-                line = line.rstrip().split(delimiter)
-                for item in line:
-                    yield dtype(item)
-        loadtxt_fast.rowlength = len(line)
-
-    data = np.fromiter(iter_func(), dtype=dtype)
-    data = data.reshape((-1, loadtxt_fast.rowlength))
-    return data
-
-def parse_path(file_path):
-    """
-    Input:
-        full path
-
-    Returns:
-        self.dir = base directory of the file
-        self.name = file name without extension
-        self.ext = file extension
-    """
-    class path_info:
-        def __init__(self, path):
-            path_abs = os.path.realpath(path).replace('\\', '/')
-            s = path_abs.split('/')
-            f = s[-1].split('.')
-            basedir = '/'.join(s[:-1])
-            if len(f) == 1:
-                name, ext = f[-1], ''
-            else:
-                name, ext = '.'.join(f[:-1]), f[-1]
-            self.dir = basedir
-            self.name = name
-            self.ext = ext
-            self.txt = 'self.dir=%s\nself.name=%s\nself.ext=%s\n' % (self.dir, self.name, self.ext)
-        def __repr__(self):
-            return self.txt
-        def __str__(self):
-            return self.txt
-
-    return path_info(file_path)
-
-def parse_path_list(path):
-    """
-    Input:
-        full path
-
-    Returns:
-        base dir, file(or dir) name, extension (if file)
-    """
-
-    path_abs = os.path.realpath(path).replace('\\', '/')
-    s = path_abs.split('/')
-    f = s[-1].split('.')
-    basedir = '/'.join(s[:-1]) + '/'
-    if len(f) == 1:
-        name, ext = f[-1], ''
-    else:
-        name, ext = '.'.join(f[:-1]), f[-1]
-
-    return basedir, name, ext
-
-def forward_slashify(txt):
-    return txt.replace('\\\\', '/').replace('\\', '/')
-
-
-'''"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
- Timer class
-"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""'''
-
-class Timer(object):
-    """
-    Timer class
-
-    if autoreset=True, timer is reset after any member function call
-    """
-    def __init__(self, autoreset=False):
-        self.autoreset = autoreset
-        self.reset()
-
-    def sec(self):
-        read = time.time() - self.ref
-        if self.autoreset: self.reset()
-        return read
-
-    def msec(self):
-        return self.sec() * 1000.0
-
-    def reset(self):
-        self.ref = time.time()
-
-    def sleep_atleast(self, sec):
-        """
-        Sleep up to sec seconds
-        It's more convenient if autoreset=True
-        """
-        timer_sec = self.sec()
-        if timer_sec < sec:
-            time.sleep(sec - timer_sec)
-            if self.autoreset: self.reset()
-
-
-'''"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
- Debugging
-"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""'''
-
-def auto_debug():
-    """
-    Triggers debugging mode automatically when AssertionError is raised
-
-    Snippet from:
-      stackoverflow.com/questions/242485/starting-python-debugger-automatically-on-error
-    """
-    def debug_info(type, value, tb):
-        if hasattr(sys, 'ps1') or not sys.stderr.isatty() or type == KeyboardInterrupt:
-            # interactive mode or no tty-like device
-            sys.__excepthook__(type, value, tb)
-        else:
-            # non-interactive mode
-            logger.exception()
-            pdb.pm()
-    sys.excepthook = debug_info
-
-# enter interactive shell within the caller's scope
-def shell():
-    """
-    Enter interactive shell within the caller's scope
-    """
-    logger.info('*** Entering interactive shell. Ctrl+D to return. ***')
-    stack = inspect.stack()
-    try:  # globals are first loaded, then overwritten by locals
-        globals_ = {}
-        globals_.update({key:value for key, value in stack[1][0].f_globals.items()})
-        globals_.update({key:value for key, value in stack[1][0].f_locals.items()})
-    finally:
-        del stack
-    code.InteractiveConsole(globals_).interact()
-
-def run_multi(cmd_list, cores=0, quiet=False):
-    """
-    Input
-    -----
-    cmd_list: list of commands just like when you type on bash
-    cores: number of cores to use (use all cores if 0)
-    Logging tip: "command args > log.txt 2>&1"
-    """
-    if cores == 0: cores = mp.cpu_count()
-    pool = mp.Pool(cores)
-    processes = []
-    for c in cmd_list:
-        if not quiet:
-            logger.info(cmd)
-        processes.append(pool.apply_async(os.system, [cmd]))
-    for proc in processes:
-        proc.get()
-    pool.close()
-    pool.join()
-
-# print_c definition: print texts in color
-try:
-    import colorama
-    colorama.init()
-
-    def print_c(msg, color=None, end='\n'):
-        """
-        Colored print using colorama.
-
-        Fullset:
-            https://pypi.python.org/pypi/colorama
-            Fore: BLACK, RED, GREEN, YELLOW, BLUE, MAGENTA, CYAN, WHITE, RESET.
-            Back: BLACK, RED, GREEN, YELLOW, BLUE, MAGENTA, CYAN, WHITE, RESET.
-            Style: DIM, NORMAL, BRIGHT, RESET_ALL
-
-        TODO:
-            Make it using *args and **kwargs to support fully featured print().
-
-        """
-        if color is None:
-            print(str(msg), end=end)
-            return
-        color = str(color)
-        if len(color) != 1:
-            raise ValueError('Color parameter must be a single color code, not %s' % type(color))
-        if color.upper() == 'B':
-            c = colorama.Fore.BLUE
-        elif color.upper() == 'R':
-            c = colorama.Fore.RED
-        elif color.upper() == 'G':
-            c = colorama.Fore.GREEN
-        elif color.upper() == 'Y':
-            c = colorama.Fore.YELLOW
-        elif color.upper() == 'W':
-            c = colorama.Fore.WHITE
-        elif color.upper() == 'C':
-            c = colorama.Fore.CYAN
-        else:
-            logger.error('print_c(): Unknown color code %s' % color)
-            raise ValueError
-        print(colorama.Style.BRIGHT + c + str(msg) + colorama.Style.RESET_ALL, end=end)
-
-except ImportError:
-    logger.warning('colorama module not found. print_c() will ignore color codes.')
-    def print_c(msg, color, end='\n'):
-        print(msg, end=end)
-
-
-'''"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
- MATLAB
-"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""'''
-
-def matlab(codes):
-    """ Execute Matlab snippets """
-    exe = 'matlab -nojvm -nodisplay -nosplash -wait -automation -r \"cd %s; %s; exit;\"' % (os.getcwd(), codes)
-    # exe= 'matlab -nojvm -nodisplay -nosplash -wait -automation -r \"%s; exit;\"'% codes
-    os.system(exe)
-
-def loadmat(filename):
-    '''
-    Proper mat file loading perserving the correct structure
-    https://stackoverflow.com/review/suggested-edits/21667510
-
-    this function should be called instead of direct scipy.io.loadmat
-    as it cures the problem of not properly recovering python dictionaries
-    from mat files. It calls the function check keys to cure all entries
-    which are still mat-objects
-    '''
-    def _check_keys(d):
-        '''
-        checks if entries in dictionary are mat-objects. If yes
-        todict is called to change them to nested dictionaries
-        '''
-        for key in d:
-            if isinstance(d[key], scipy.io.matlab.mio5_params.mat_struct):
-                d[key] = _todict(d[key])
-        return d
-
-    def _has_struct(elem):
-        """Determine if elem is an array and if any array item is a struct"""
-        return isinstance(elem, np.ndarray) and any(isinstance(
-                    e, scipy.io.matlab.mio5_params.mat_struct) for e in elem)
-
-    def _todict(matobj):
-        '''
-        A recursive function which constructs from matobjects nested dictionaries
-        '''
-        d = {}
-        for strg in matobj._fieldnames:
-            elem = matobj.__dict__[strg]
-            if isinstance(elem, scipy.io.matlab.mio5_params.mat_struct):
-                d[strg] = _todict(elem)
-            elif _has_struct(elem):
-                d[strg] = _tolist(elem)
-            else:
-                d[strg] = elem
-        return d
-
-    def _tolist(ndarray):
-        '''
-        A recursive function which constructs lists from cellarrays
-        (which are loaded as numpy ndarrays), recursing into the elements
-        if they contain matobjects.
-        '''
-        elem_list = []
-        for sub_elem in ndarray:
-            if isinstance(sub_elem, scipy.io.matlab.mio5_params.mat_struct):
-                elem_list.append(_todict(sub_elem))
-            elif _has_struct(sub_elem):
-                elem_list.append(_tolist(sub_elem))
-            else:
-                elem_list.append(sub_elem)
-        return elem_list
-    try:
-        # old Matlab format
-        data = scipy.io.loadmat(filename, struct_as_record=False, squeeze_me=True)
-        return _check_keys(data)
-    except NotImplementedError:
-        # Matlab 7.3 and higher (HDF)
-        return mat73.loadmat(filename)
-
-
-'''"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
- Scikit-learn
-"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""'''
-
-def confusion_matrix(Y_true, Y_pred, label_len=6):
-    """
-    Generate confusion matrix in a string format
-
-    Input
-    -----
-        Y_true: true labels
-        Y_pred: test labels
-        label_len: maximum label text length (minimum length: 6)
-
-    Output
-    ------
-        (cfmat, acc)
-        cfmat: confusion matrix (string)
-            X-axis: prediction
-            Y-axis: ground truth
-        acc: accuracy (float)
-    """
-
-    # find labels
-    if type(Y_true) == np.ndarray:
-        Y_labels = np.unique(Y_true)
-    else:
-        Y_labels = [x for x in set(Y_true)]
-    if label_len < 6:
-        label_len = 6
-        logger.warning('label_len < 6. Setting to 6.')
-    label_tpl = '%' + '-%ds' % label_len
-    col_tpl = '%' + '-%d.2f' % label_len
-
-    # sanity check
-    if len(Y_pred) > len(Y_true):
-        raise RuntimeError('Y_pred has more items than Y_true')
-    elif len(Y_pred) < len(Y_true):
-        Y_true = Y_true[:len(Y_pred)]
-
-    cm = sklearn.metrics.confusion_matrix(Y_true, Y_pred, labels=Y_labels)
-
-    # compute confusion matrix
-    cm_rate = cm.copy().astype('float')
-    # cm_rate= cm.astype('float') / cm.sum(axis=1)[:, np.newaxis] # this can have NaN
-    cm_sum = np.sum(cm, axis=1)
-
-    for r, s in zip(cm_rate, cm_sum):
-        if s > 0:
-            r /= s
-    cm_txt = label_tpl % 'gt\dt'
-    for l in Y_labels:
-        cm_txt += label_tpl % l[:label_len]
-    cm_txt += '\n'
-    for l, r in zip(Y_labels, cm_rate):
-        cm_txt += label_tpl % l[:label_len]
-        for c in r:
-            cm_txt += col_tpl % c
-        cm_txt += '\n'
-
-    # compute accuracy
-    correct = 0.0
-    for c in range(cm.shape[0]):
-        correct += cm[c][c]
-    cm_sum = cm.sum()
-    if cm_sum > 0:
-        acc = correct / cm.sum()
-    else:
-        acc = 0.0
-
-    return cm_txt, acc
-
-
-'''"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
- Matplotlib
-"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""'''
-
-def plot_imagesc(img, x=None, y=None, title='', colorbar=True, **kwargs):
-    """
-    Plot 2-D array as image with autoscaling with a color range [med-std, med+std]
-    """
-    # sanity check
-    if (x is not None and y is not None) and (len(x) != img.shape[1] or len(y) != img.shape[0]):
-        raise ValueError('yicks (%d) and xticks (%d) do not correspond to image shape %s' % (len(x), len(y), img.shape))
-
-    plt.imshow(img, aspect='auto', interpolation='none', origin='lower', **kwargs)
-    if colorbar:
-        plt.colorbar()
-    std = np.std(img, axis=None)
-    med = np.median(img, axis=None)
-    plt.clim([med-std, med+std])
-    if x is not None:
-        if len(x) <= 10:
-            xstep = 1
-        else:
-            xstep = len(x) // 10
-        if type(x[0]) in [str, np.str_]:
-            xticklabels = x[::xstep]
-        else:
-            xticklabels = x.round(6)[::xstep]
-        plt.xticks(range(0, img.shape[1], xstep), xticklabels)
-    if y is not None:
-        if len(y) <= 10:
-            ystep = 1
-        else:
-            ystep = len(y) // 10
-        if type(y[0]) in [str, np.str_]:
-            yticklabels = y[::ystep]
-        else:
-            yticklabels = y.round(6)[::ystep]
-        plt.yticks(range(0, img.shape[0], ystep), yticklabels)
-    plt.title(title)
-    plt.show(block=False)
-
-def plot_cm(Y_pred, Y_test, labels, title_prefix='', print_console=True):
-    """
-    Plot confusion matrix
-    """
-    N = len(Y_pred)
-    cm_norm = 'true' #'true', None
-    cm = sklearn.metrics.confusion_matrix(Y_test, Y_pred, normalize=cm_norm, labels=labels)
-    cm_raw = sklearn.metrics.confusion_matrix(Y_test, Y_pred, normalize=None, labels=labels)
-    img = sklearn.metrics.ConfusionMatrixDisplay(cm, display_labels=labels)
-    img.plot(cmap=plt.cm.Blues)
-    accuracy = sklearn.metrics.accuracy_score(Y_test, Y_pred)
-    f1_score = sklearn.metrics.f1_score(Y_test, Y_pred, average='macro')
-    plt.title('%s Confusion matrix (f1=%.2f, acc=%.2f, N=%d)' % (title_prefix, f1_score, accuracy, N))
-    if print_console:
-        print(sklearn.metrics.classification_report(Y_test, Y_pred, labels=labels))
-        print('%s Confusion matrix (raw values)' % title_prefix)
-        print(cm_raw)
-    plt.show(block=False)
-    plt.ioff()
-    plt.pause(0.05)
-
-def plot_cm_le(Y_pred, Y_test, le, title_prefix='', print_console=True):
-    """
-    Plot confusion matrix using label encoder
-    """
-    N = len(Y_pred)
-    cm_norm = 'true' #'true', None
-    cm = sklearn.metrics.confusion_matrix(Y_test, Y_pred, normalize=cm_norm)
-    img = sklearn.metrics.ConfusionMatrixDisplay(cm, display_labels=le.classes_)
-    img.plot(cmap=plt.cm.Blues)
-    accuracy = sklearn.metrics.accuracy_score(Y_test, Y_pred)
-    f1_score = sklearn.metrics.f1_score(Y_test, Y_pred, average='macro')
-    plt.title('%s Confusion matrix (f1=%.2f, acc=%.2f, N=%d)' % (title_prefix, f1_score, accuracy, N))
-    if print_console:
-        print(sklearn.metrics.classification_report(Y_test, Y_pred, target_names=le.classes_))
-        print(sklearn.metrics.confusion_matrix(Y_test, Y_pred, normalize=None))
-        print('%s Confusion matrix (raw values)' % title_prefix)
-    plt.show(block=False)
-    plt.ioff()
-    plt.pause(0.05)
-
-def plot_errorbar(data, method='std', ticks=None, title=None, **kwargs):
-    """
-    Plot horizontal errorbar from an array of samples
-
-    data: Numpy array of dimension [samples] x [variables]
-    method:
-      sem: standard error of means
-      std: standard deviation
-    ticks: bar tick labels
-    """
-    if type(data) == list:
-        data = np.array(data)
-    elif type(data) != np.ndarray:
-        raise ValueError('Unsupported data type %s' % type(data))
-    if len(data.shape) != 2:
-        raise ValueError('Input must be of 2 dimensions')
-    if method == 'std':
-        n = 1
-    elif method == 'sem':
-        n = len(data)
-    else:
-        raise ValueError('Unsupported method: %s' % method)
-    if ticks is None:
-        ticks = ['%d'%x for x in range(data.shape[1])]
-    if title is None:
-        title = ''
-    mean = np.mean(data, axis=0)
-    std = np.std(data, axis=0)
-    plt.bar(x=ticks, height=mean, yerr=std/n, **kwargs)
-    plt.title(title)
-
-def pvalue2txt(pvalue, max_precision=3):
-    if pvalue >= 10**(-max_precision):
-        txt = ('p=%%.%df' % max_precision) % pvalue
-    elif pvalue == 0:
-        txt = 'p<10^-32'
-    else:
-        txt = 'p<=10^%d' % math.ceil(math.log10(pvalue))
-    return txt
-
-'''"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
- ETC
-"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""'''
-
-def int2bits(num, nbits=8):
-    """ Convert an integer into bits representation. default=8 bits (0-255) """
-    return [int(num) >> x & 1 for x in range(nbits - 1, -1, -1)]
-
-def bits2int(bitlist):
-    """ Convert a list of bits into an integer """
-    out = 0
-    for bit in bitlist:
-        out = (out << 1) | bit
-    return out
+from __future__ import print_function, division
+
+"""
+Useful Python utilities
+
+Author: Kyuhwa Lee
+Imperial College of Science, Technology and Medicine
+
+"""
+
+# set Q_VERBOSE= 0 to make it silent. 1:verbose, 2:extra verbose
+Q_VERBOSE = 0
+
+
+import os
+import sys
+import pdb
+import code
+import time
+import math
+import mat73
+import scipy.io
+import shutil
+import logging
+import inspect
+import traceback
+import itertools
+import numpy as np
+import sklearn.metrics
+import matplotlib.pyplot as plt
+
+# logger
+try:
+    from neurodecode import logger
+except ImportError:
+    logging.basicConfig(format='%(msg)s', level='INFO')
+    logger = logging.getLogger(__name__)
+    logger.propagate = False
+
+# pickle
+try:
+    import cPickle as pickle  # Python 2 (cPickle = C version of pickle)
+except ImportError:
+    import pickle  # Python 3 (C version is the default)
+
+
+'''"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
+ Math
+"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""'''
+
+def sigmoid(x):
+    return 1 / (1 + math.exp(-x))
+
+def sigmoid_array(x):
+    return 1 / (1 + np.exp(-x))
+
+def dirichlet(n):
+    """
+    Uniform Dirichlet distribution with sigma(alpha)=1.0
+    """
+    alpha = 1.0 / n
+    return 1 / beta(alpha, n) * ((1 / n) ** (alpha - 1)) ** n
+
+def beta(alpha, n):
+    """
+    Multinomial Beta function with uniform alpha values
+
+    n: number of rule probabilities
+    """
+    return math.gamma(alpha) ** n / math.gamma(n * alpha)
+
+def poisson(mean, k):
+    """
+    Poisson distribution. We use k-1 since the minimum length is 1, not 0.
+    """
+    return (mean ** (k - 1) * math.exp(-mean)) / math.factorial(k - 1)
+
+def average_every_n(arr, n):
+    """
+    Average every n elements of a numpy array
+
+    if not len(arr) % n == 0, it will be trimmed to the closest divisible length
+    """
+    end = n * int(len(arr) / n)
+    return np.mean(arr[:end].reshape(-1, n), 1)
+
+def zscore_mod(X, axis=0):
+    """
+    Modified z-score for multidimensional arrays
+
+    MAD = median(abs(X-median(X)))
+    MeanAD = mean(abs(X-mean(X)))
+    If MAD does equal 0 (if at least 50% of samples have the same value)
+      Subtract the median from the score and divide by 1.253314*MeanAD.
+      1.253314*MeanAD approximately equals the standard deviation.
+    If MAD does not equal 0
+      Subtract the median from the score and divide by 1.486*MAD.
+      1.486*MAD approximately equals the standard deviation.
+
+    Reference:
+    https://www.ibm.com/docs/en/cognos-analytics/11.1.0?topic=terms-modified-z-score
+    """
+    # medians are computed for each trial for each feature
+    X_med = np.median(X, axis=axis)
+    # expand dimension for broadcasting
+    X_med_diff = X - np.expand_dims(X_med, axis=axis)
+    # compute MAD
+    X_mad = np.median(np.abs(X_med_diff), axis=axis)
+
+    if X_mad.all():
+        # if all MADs are non-zero
+        X_norm = X_med_diff / (1.486 * np.expand_dims(X_mad, axis))
+    else:
+        # compute MeanAD
+        X_mean = np.mean(X, axis=axis)
+        X_mean_ad = np.mean(abs(X - np.expand_dims(X_mean, axis=axis)), axis=axis)
+        X_mad_corrected = X_mad * 1.486
+        # replace 0 in MAD with the corresponding meanAD value
+        for zero_loc in np.array(np.where(X_mad==0)).T:
+            zero_loc = tuple(zero_loc) # every index containing 0 in MAD
+            X_mad_corrected[zero_loc] = 1.253314 * X_mean_ad[zero_loc]
+        X_norm = X_med_diff / np.expand_dims(X_mad_corrected, axis)
+    return X_norm
+
+
+'''"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
+ List/Dict related
+"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""'''
+
+def list2string(vec, fmt, sep=' '):
+    """
+    Convert a list to string with formatting, separated by sep (default is space).
+    Example: fmt= '%.32e', '%.6f', etc.
+    """
+    return sep.join((fmt % x for x in vec))
+
+def flatten_list(l):
+    return list(itertools.chain.from_iterable(l))
+
+def get_index_min(seq):
+    """
+    Get the index of the minimum item in a list or dict
+    """
+    if type(seq) == list:
+        return min(range(len(seq)), key=seq.__getitem__)
+    elif type(seq) == dict:
+        return min(seq, key=seq.__getitem__)
+    else:
+        logger.error('Unsupported input %s' % type(seq))
+        return None
+
+def get_index_max(seq):
+    """
+    Get the index of the maximum item in a list or dict
+    """
+    if type(seq) == list:
+        return max(range(len(seq)), key=seq.__getitem__)
+    elif type(seq) == dict:
+        return max(seq, key=seq.__getitem__)
+    else:
+        logger.error('Unsupported input %s' % type(seq))
+        return None
+
+def sort_by_value(s, rev=False):
+    """
+    Sort dictionary or list by value and return a sorted list of keys and values.
+    Values must be hashable and unique.
+    """
+    assert type(s) == dict or type(s) == list, 'Input must be a dictionary or list.'
+    if type(s) == list:
+        s = dict(enumerate(s))
+    s_rev = dict((v, k) for k, v in s.items())
+    if Q_VERBOSE > 0 and not len(s_rev) == len(s):
+        logger.warning('sort_by_value(): %d identical values' % (len(s.values()) - len(set(s.values())) + 1))
+    values = sorted(s_rev, reverse=rev)
+    keys = [s_rev[x] for x in values]
+    return keys, values
+
+
+'''"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
+ File I/O
+"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""'''
+
+def get_file_list(path, fullpath=True, recursive=False):
+    """
+    Get files with or without full path.
+    """
+    path = path.replace('\\', '/')
+    if not path[-1] == '/': path += '/'
+
+    if recursive == False:
+        if fullpath == True:
+            filelist = [path + f for f in os.listdir(path) if os.path.isfile(path + '/' + f) and f[0] != '.']
+        else:
+            filelist = [f for f in os.listdir(path) if os.path.isfile(path + '/' + f) and f[0] != '.']
+    else:
+        filelist = []
+        for root, dirs, files in os.walk(path):
+            root = root.replace('\\', '/')
+            if fullpath == True:
+                [filelist.append(root + '/' + f) for f in files]
+            else:
+                [filelist.append(f) for f in files]
+    return sorted(filelist)
+
+def get_dir_list(path, recursive=False, no_child=False):
+    """
+    Get directory list relative to path.
+
+    Input:
+        recusrive: search recursively if True.
+        no_child: search directories having no child directory (leaf nodes)
+    """
+    path = path.replace('\\', '/')
+    if not path[-1] == '/': path += '/'
+
+    if recursive == True:
+        pathlist = []
+        for root, dirs, files in os.walk(path):
+            root = root.replace('\\', '/')
+            [pathlist.append(root + '/' + d) for d in dirs]
+
+            if no_child:
+                for p in pathlist:
+                    if len(get_dir_list(p)) > 0:
+                        pathlist.remove(p)
+
+    else:
+        pathlist = [path + f for f in os.listdir(path) if os.path.isdir(path + '/' + f)]
+        if no_child:
+            for p in pathlist:
+                if len(get_dir_list(p)) > 0:
+                    pathlist.remove(p)
+
+    return sorted(pathlist)
+
+def make_dirs(dirname, delete=False):
+    """
+    Recusively create directories.
+    if delete=true, directory will be deleted first if exists.
+    """
+    if os.path.exists(dirname) and delete == True:
+        try:
+            shutil.rmtree(dirname)
+        except OSError:
+            logger.error('Directory was not completely removed. (Perhaps a Dropbox folder?). Continuing.')
+    if not os.path.exists(dirname):
+        os.makedirs(dirname)
+
+def save_obj(fname, obj, protocol=4):
+    """
+    Save python object into a file
+    Set protocol=2 for Python 2 compatibility
+    """
+    with open(fname, 'wb') as fout:
+        pickle.dump(obj, fout, protocol)
+
+def load_obj(fname):
+    """
+    Read python object from a file
+    """
+    try:
+        with open(fname, 'rb') as f:
+            return pickle.load(f)
+    except UnicodeDecodeError:
+        # usually happens when trying to load Python 2 pickle object from Python 3
+        with open(fname, 'rb') as f:
+            return pickle.load(f, encoding='latin1')
+    except:
+        msg = 'load_obj(): Cannot load pickled object file "%s". The error was:\n%s\n%s' %\
+              (fname, sys.exc_info()[0], sys.exc_info()[1])
+        raise IOError(msg)
+
+def loadtxt_fast(filename, delimiter=',', skiprows=0, dtype=float):
+    """
+    Much faster matrix loading than numpy's loadtxt
+    http://stackoverflow.com/a/8964779
+    """
+    def iter_func():
+        with open(filename, 'r') as infile:
+            for _ in range(skiprows):
+                next(infile)
+            for line in infile:
+                line = line.rstrip().split(delimiter)
+                for item in line:
+                    yield dtype(item)
+        loadtxt_fast.rowlength = len(line)
+
+    data = np.fromiter(iter_func(), dtype=dtype)
+    data = data.reshape((-1, loadtxt_fast.rowlength))
+    return data
+
+def parse_path(file_path):
+    """
+    Input:
+        full path
+
+    Returns:
+        self.dir = base directory of the file
+        self.name = file name without extension
+        self.ext = file extension
+    """
+    class path_info:
+        def __init__(self, path):
+            path_abs = os.path.realpath(path).replace('\\', '/')
+            s = path_abs.split('/')
+            f = s[-1].split('.')
+            basedir = '/'.join(s[:-1])
+            if len(f) == 1:
+                name, ext = f[-1], ''
+            else:
+                name, ext = '.'.join(f[:-1]), f[-1]
+            self.dir = basedir
+            self.name = name
+            self.ext = ext
+            self.txt = 'self.dir=%s\nself.name=%s\nself.ext=%s\n' % (self.dir, self.name, self.ext)
+        def __repr__(self):
+            return self.txt
+        def __str__(self):
+            return self.txt
+
+    return path_info(file_path)
+
+def parse_path_list(path):
+    """
+    Input:
+        full path
+
+    Returns:
+        base dir, file(or dir) name, extension (if file)
+    """
+
+    path_abs = os.path.realpath(path).replace('\\', '/')
+    s = path_abs.split('/')
+    f = s[-1].split('.')
+    basedir = '/'.join(s[:-1]) + '/'
+    if len(f) == 1:
+        name, ext = f[-1], ''
+    else:
+        name, ext = '.'.join(f[:-1]), f[-1]
+
+    return basedir, name, ext
+
+def forward_slashify(txt):
+    return txt.replace('\\\\', '/').replace('\\', '/')
+
+
+'''"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
+ Timer class
+"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""'''
+
+class Timer(object):
+    """
+    Timer class
+
+    if autoreset=True, timer is reset after any member function call
+    """
+    def __init__(self, autoreset=False):
+        self.autoreset = autoreset
+        self.reset()
+
+    def sec(self):
+        read = time.time() - self.ref
+        if self.autoreset: self.reset()
+        return read
+
+    def msec(self):
+        return self.sec() * 1000.0
+
+    def reset(self):
+        self.ref = time.time()
+
+    def sleep_atleast(self, sec):
+        """
+        Sleep up to sec seconds
+        It's more convenient if autoreset=True
+        """
+        timer_sec = self.sec()
+        if timer_sec < sec:
+            time.sleep(sec - timer_sec)
+            if self.autoreset: self.reset()
+
+
+'''"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
+ Debugging
+"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""'''
+
+def auto_debug():
+    """
+    Triggers debugging mode automatically when AssertionError is raised
+
+    Snippet from:
+      stackoverflow.com/questions/242485/starting-python-debugger-automatically-on-error
+    """
+    def debug_info(type, value, tb):
+        if hasattr(sys, 'ps1') or not sys.stderr.isatty() or type == KeyboardInterrupt:
+            # interactive mode or no tty-like device
+            sys.__excepthook__(type, value, tb)
+        else:
+            # non-interactive mode
+            logger.exception()
+            pdb.pm()
+    sys.excepthook = debug_info
+
+# enter interactive shell within the caller's scope
+def shell():
+    """
+    Enter interactive shell within the caller's scope
+    """
+    logger.info('*** Entering interactive shell. Ctrl+D to return. ***')
+    stack = inspect.stack()
+    try:  # globals are first loaded, then overwritten by locals
+        globals_ = {}
+        globals_.update({key:value for key, value in stack[1][0].f_globals.items()})
+        globals_.update({key:value for key, value in stack[1][0].f_locals.items()})
+    finally:
+        del stack
+    code.InteractiveConsole(globals_).interact()
+
+def run_multi(cmd_list, cores=0, quiet=False):
+    """
+    Input
+    -----
+    cmd_list: list of commands just like when you type on bash
+    cores: number of cores to use (use all cores if 0)
+    Logging tip: "command args > log.txt 2>&1"
+    """
+    if cores == 0: cores = mp.cpu_count()
+    pool = mp.Pool(cores)
+    processes = []
+    for c in cmd_list:
+        if not quiet:
+            logger.info(cmd)
+        processes.append(pool.apply_async(os.system, [cmd]))
+    for proc in processes:
+        proc.get()
+    pool.close()
+    pool.join()
+
+# print_c definition: print texts in color
+try:
+    import colorama
+    colorama.init()
+
+    def print_c(msg, color=None, end='\n'):
+        """
+        Colored print using colorama.
+
+        Fullset:
+            https://pypi.python.org/pypi/colorama
+            Fore: BLACK, RED, GREEN, YELLOW, BLUE, MAGENTA, CYAN, WHITE, RESET.
+            Back: BLACK, RED, GREEN, YELLOW, BLUE, MAGENTA, CYAN, WHITE, RESET.
+            Style: DIM, NORMAL, BRIGHT, RESET_ALL
+
+        TODO:
+            Make it using *args and **kwargs to support fully featured print().
+
+        """
+        if color is None:
+            print(str(msg), end=end)
+            return
+        color = str(color)
+        if len(color) != 1:
+            raise ValueError('Color parameter must be a single color code, not %s' % type(color))
+        if color.upper() == 'B':
+            c = colorama.Fore.BLUE
+        elif color.upper() == 'R':
+            c = colorama.Fore.RED
+        elif color.upper() == 'G':
+            c = colorama.Fore.GREEN
+        elif color.upper() == 'Y':
+            c = colorama.Fore.YELLOW
+        elif color.upper() == 'W':
+            c = colorama.Fore.WHITE
+        elif color.upper() == 'C':
+            c = colorama.Fore.CYAN
+        else:
+            logger.error('print_c(): Unknown color code %s' % color)
+            raise ValueError
+        print(colorama.Style.BRIGHT + c + str(msg) + colorama.Style.RESET_ALL, end=end)
+
+except ImportError:
+    logger.warning('colorama module not found. print_c() will ignore color codes.')
+    def print_c(msg, color, end='\n'):
+        print(msg, end=end)
+
+
+'''"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
+ MATLAB
+"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""'''
+
+def matlab(codes):
+    """ Execute Matlab snippets """
+    exe = 'matlab -nojvm -nodisplay -nosplash -wait -automation -r \"cd %s; %s; exit;\"' % (os.getcwd(), codes)
+    # exe= 'matlab -nojvm -nodisplay -nosplash -wait -automation -r \"%s; exit;\"'% codes
+    os.system(exe)
+
+def loadmat(filename):
+    '''
+    Proper mat file loading perserving the correct structure
+    https://stackoverflow.com/review/suggested-edits/21667510
+
+    this function should be called instead of direct scipy.io.loadmat
+    as it cures the problem of not properly recovering python dictionaries
+    from mat files. It calls the function check keys to cure all entries
+    which are still mat-objects
+    '''
+    def _check_keys(d):
+        '''
+        checks if entries in dictionary are mat-objects. If yes
+        todict is called to change them to nested dictionaries
+        '''
+        for key in d:
+            if isinstance(d[key], scipy.io.matlab.mio5_params.mat_struct):
+                d[key] = _todict(d[key])
+        return d
+
+    def _has_struct(elem):
+        """Determine if elem is an array and if any array item is a struct"""
+        return isinstance(elem, np.ndarray) and any(isinstance(
+                    e, scipy.io.matlab.mio5_params.mat_struct) for e in elem)
+
+    def _todict(matobj):
+        '''
+        A recursive function which constructs from matobjects nested dictionaries
+        '''
+        d = {}
+        for strg in matobj._fieldnames:
+            elem = matobj.__dict__[strg]
+            if isinstance(elem, scipy.io.matlab.mio5_params.mat_struct):
+                d[strg] = _todict(elem)
+            elif _has_struct(elem):
+                d[strg] = _tolist(elem)
+            else:
+                d[strg] = elem
+        return d
+
+    def _tolist(ndarray):
+        '''
+        A recursive function which constructs lists from cellarrays
+        (which are loaded as numpy ndarrays), recursing into the elements
+        if they contain matobjects.
+        '''
+        elem_list = []
+        for sub_elem in ndarray:
+            if isinstance(sub_elem, scipy.io.matlab.mio5_params.mat_struct):
+                elem_list.append(_todict(sub_elem))
+            elif _has_struct(sub_elem):
+                elem_list.append(_tolist(sub_elem))
+            else:
+                elem_list.append(sub_elem)
+        return elem_list
+    try:
+        # old Matlab format
+        data = scipy.io.loadmat(filename, struct_as_record=False, squeeze_me=True)
+        return _check_keys(data)
+    except NotImplementedError:
+        # Matlab 7.3 and higher (HDF)
+        return mat73.loadmat(filename)
+
+
+'''"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
+ Scikit-learn
+"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""'''
+
+def confusion_matrix(Y_true, Y_pred, label_len=6):
+    """
+    Generate confusion matrix in a string format
+
+    Input
+    -----
+        Y_true: true labels
+        Y_pred: test labels
+        label_len: maximum label text length (minimum length: 6)
+
+    Output
+    ------
+        (cfmat, acc)
+        cfmat: confusion matrix (string)
+            X-axis: prediction
+            Y-axis: ground truth
+        acc: accuracy (float)
+    """
+
+    # find labels
+    if type(Y_true) == np.ndarray:
+        Y_labels = np.unique(Y_true)
+    else:
+        Y_labels = [x for x in set(Y_true)]
+    if label_len < 6:
+        label_len = 6
+        logger.warning('label_len < 6. Setting to 6.')
+    label_tpl = '%' + '-%ds' % label_len
+    col_tpl = '%' + '-%d.2f' % label_len
+
+    # sanity check
+    if len(Y_pred) > len(Y_true):
+        raise RuntimeError('Y_pred has more items than Y_true')
+    elif len(Y_pred) < len(Y_true):
+        Y_true = Y_true[:len(Y_pred)]
+
+    cm = sklearn.metrics.confusion_matrix(Y_true, Y_pred, labels=Y_labels)
+
+    # compute confusion matrix
+    cm_rate = cm.copy().astype('float')
+    # cm_rate= cm.astype('float') / cm.sum(axis=1)[:, np.newaxis] # this can have NaN
+    cm_sum = np.sum(cm, axis=1)
+
+    for r, s in zip(cm_rate, cm_sum):
+        if s > 0:
+            r /= s
+    cm_txt = label_tpl % 'gt\dt'
+    for l in Y_labels:
+        cm_txt += label_tpl % l[:label_len]
+    cm_txt += '\n'
+    for l, r in zip(Y_labels, cm_rate):
+        cm_txt += label_tpl % l[:label_len]
+        for c in r:
+            cm_txt += col_tpl % c
+        cm_txt += '\n'
+
+    # compute accuracy
+    correct = 0.0
+    for c in range(cm.shape[0]):
+        correct += cm[c][c]
+    cm_sum = cm.sum()
+    if cm_sum > 0:
+        acc = correct / cm.sum()
+    else:
+        acc = 0.0
+
+    return cm_txt, acc
+
+
+'''"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
+ Matplotlib
+"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""'''
+
+def plot_imagesc(img, x=None, y=None, title='', colorbar=True, **kwargs):
+    """
+    Plot 2-D array as image with autoscaling with a color range [med-std, med+std]
+    """
+    # sanity check
+    if (x is not None and y is not None) and (len(x) != img.shape[1] or len(y) != img.shape[0]):
+        raise ValueError('yicks (%d) and xticks (%d) do not correspond to image shape %s' % (len(x), len(y), img.shape))
+
+    plt.imshow(img, aspect='auto', interpolation='none', origin='lower', **kwargs)
+    if colorbar:
+        plt.colorbar()
+    std = np.std(img, axis=None)
+    med = np.median(img, axis=None)
+    plt.clim([med-std, med+std])
+    if x is not None:
+        if len(x) <= 10:
+            xstep = 1
+        else:
+            xstep = len(x) // 10
+        if type(x[0]) in [str, np.str_]:
+            xticklabels = x[::xstep]
+        else:
+            xticklabels = x.round(6)[::xstep]
+        plt.xticks(range(0, img.shape[1], xstep), xticklabels)
+    if y is not None:
+        if len(y) <= 10:
+            ystep = 1
+        else:
+            ystep = len(y) // 10
+        if type(y[0]) in [str, np.str_]:
+            yticklabels = y[::ystep]
+        else:
+            yticklabels = y.round(6)[::ystep]
+        plt.yticks(range(0, img.shape[0], ystep), yticklabels)
+    plt.title(title)
+    plt.show(block=False)
+
+def plot_cm(Y_pred, Y_test, labels, title_prefix='', print_console=True):
+    """
+    Plot confusion matrix
+    """
+    N = len(Y_pred)
+    cm_norm = 'true' #'true', None
+    cm = sklearn.metrics.confusion_matrix(Y_test, Y_pred, normalize=cm_norm, labels=labels)
+    cm_raw = sklearn.metrics.confusion_matrix(Y_test, Y_pred, normalize=None, labels=labels)
+    img = sklearn.metrics.ConfusionMatrixDisplay(cm, display_labels=labels)
+    img.plot(cmap=plt.cm.Blues)
+    accuracy = sklearn.metrics.accuracy_score(Y_test, Y_pred)
+    f1_score = sklearn.metrics.f1_score(Y_test, Y_pred, average='macro')
+    plt.title('%s Confusion matrix (f1=%.2f, acc=%.2f, N=%d)' % (title_prefix, f1_score, accuracy, N))
+    if print_console:
+        print(sklearn.metrics.classification_report(Y_test, Y_pred, labels=labels))
+        print('%s Confusion matrix (raw values)' % title_prefix)
+        print(cm_raw)
+    plt.show(block=False)
+    plt.ioff()
+    plt.pause(0.05)
+
+def plot_cm_le(Y_pred, Y_test, le, title_prefix='', print_console=True):
+    """
+    Plot confusion matrix using label encoder
+    """
+    N = len(Y_pred)
+    cm_norm = 'true' #'true', None
+    cm = sklearn.metrics.confusion_matrix(Y_test, Y_pred, normalize=cm_norm)
+    img = sklearn.metrics.ConfusionMatrixDisplay(cm, display_labels=le.classes_)
+    img.plot(cmap=plt.cm.Blues)
+    accuracy = sklearn.metrics.accuracy_score(Y_test, Y_pred)
+    f1_score = sklearn.metrics.f1_score(Y_test, Y_pred, average='macro')
+    plt.title('%s Confusion matrix (f1=%.2f, acc=%.2f, N=%d)' % (title_prefix, f1_score, accuracy, N))
+    if print_console:
+        print(sklearn.metrics.classification_report(Y_test, Y_pred, target_names=le.classes_))
+        print(sklearn.metrics.confusion_matrix(Y_test, Y_pred, normalize=None))
+        print('%s Confusion matrix (raw values)' % title_prefix)
+    plt.show(block=False)
+    plt.ioff()
+    plt.pause(0.05)
+
+def plot_errorbar(data, method='std', ticks=None, title=None, **kwargs):
+    """
+    Plot horizontal errorbar from an array of samples
+
+    data: Numpy array of dimension [samples] x [variables]
+    method:
+      sem: standard error of means
+      std: standard deviation
+    ticks: bar tick labels
+    """
+    if type(data) == list:
+        data = np.array(data)
+    elif type(data) != np.ndarray:
+        raise ValueError('Unsupported data type %s' % type(data))
+    if len(data.shape) != 2:
+        raise ValueError('Input must be of 2 dimensions')
+    if method == 'std':
+        n = 1
+    elif method == 'sem':
+        n = len(data)
+    else:
+        raise ValueError('Unsupported method: %s' % method)
+    if ticks is None:
+        ticks = ['%d'%x for x in range(data.shape[1])]
+    if title is None:
+        title = ''
+    mean = np.mean(data, axis=0)
+    std = np.std(data, axis=0)
+    plt.bar(x=ticks, height=mean, yerr=std/n, **kwargs)
+    plt.title(title)
+
+def pvalue2txt(pvalue, max_precision=3):
+    if pvalue >= 10**(-max_precision):
+        txt = ('p=%%.%df' % max_precision) % pvalue
+    elif pvalue == 0:
+        txt = 'p<10^-32'
+    else:
+        txt = 'p<=10^%d' % math.ceil(math.log10(pvalue))
+    return txt
+
+'''"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
+ ETC
+"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""'''
+
+def int2bits(num, nbits=8):
+    """ Convert an integer into bits representation. default=8 bits (0-255) """
+    return [int(num) >> x & 1 for x in range(nbits - 1, -1, -1)]
+
+def bits2int(bitlist):
+    """ Convert a list of bits into an integer """
+    out = 0
+    for bit in bitlist:
+        out = (out << 1) | bit
+    return out
```

### Comparing `neurodecode-2.0.4/neurodecode/utils/raw2psd.py` & `neurodecode-2.0.5/neurodecode/utils/raw2psd.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-
-from __future__ import print_function, division
-
-"""
-Compute PSD features over a sliding window on the entire raw file
-
-Kyuhwa Lee
-Swiss Federal Institute of Technology (EPFL)
-
-"""
-
-# start
-import os
-import mne
-import numpy as np
-import neurodecode.utils.pycnbi_utils as pu
-import neurodecode.utils.q_common as qc
-from neurodecode import logger
-from IPython import embed
-
-mne.set_log_level('ERROR')
-os.environ['OMP_NUM_THREADS'] = '1' # actually improves performance for multitaper
-
-
-def raw2psd(rawfile=None, fmin=1, fmax=40, wlen=0.5, wstep=1, tmin=0.0, tmax=None,
-            channel_picks=None, excludes=[], n_jobs=1):
-    """
-    Compute PSD features over a sliding window on the entire raw file.
-    Leading edge of the window is the time reference, i.e. do not use future data.
-
-    Input
-    =====
-    rawfile: fif file.
-    channel_picks: None or list of channel names
-    tmin (sec): start time of the PSD window relative to the event onset.
-    tmax (sec): end time of the PSD window relative to the event onset. None = until the end.
-    fmin (Hz): minimum PSD frequency
-    fmax (Hz): maximum PSD frequency
-    wlen (sec): sliding window length for computing PSD (sec)
-    wstep (int): sliding window step (time samples)
-    excludes (list): list of channels to exclude
-    """
-
-    raw, eve = pu.load_raw(rawfile)
-    sfreq = raw.info['sfreq']
-    wframes = int(round(sfreq * wlen))
-    raw_eeg = raw.pick_types(meg=False, eeg=True, stim=False, exclude=excludes)
-    if channel_picks is None:
-        rawdata = raw_eeg._data
-        chlist = raw.ch_names
-    else:
-        chlist = []
-        for ch in channel_picks:
-            chlist.append(raw.ch_names.index(ch))
-        rawdata = raw_eeg._data[np.array(chlist)]
-
-    if tmax is None:
-        t_end = rawdata.shape[1]
-    else:
-        t_end = int(round(tmax * sfreq))
-    t_start = int(round(tmin * sfreq)) + wframes
-    psde = mne.decoding.PSDEstimator(sfreq, fmin=fmin, fmax=fmax, n_jobs=1,\
-        bandwidth=None, low_bias=True, adaptive=False, normalization='length',
-        verbose=None)
-    print('[PID %d] %s' % (os.getpid(), rawfile))
-    psd_all = []
-    evelist = []
-    times = []
-    t_len = t_end - t_start
-    last_eve = 0
-    y_i = 0
-    t_last = t_start
-    tm = qc.Timer()
-    for t in range(t_start, t_end, wstep):
-        # compute PSD
-        window = rawdata[:, t - wframes: t]
-        psd = psde.transform(window.reshape((1, window.shape[0], window.shape[1])))
-        psd = psd.reshape(psd.shape[1], psd.shape[2])
-        psd_all.append(psd)
-        times.append(t)
-
-        # matching events at the current window
-        if y_i < eve.shape[0] and t >= eve[y_i][0]:
-            last_eve = eve[y_i][2]
-            y_i += 1
-        evelist.append(last_eve)
-
-        if tm.sec() >= 1:
-            perc = (t - t_start) / t_len
-            fps = (t - t_last) / wstep
-            est = (t_end - t) / wstep / fps
-            logger.info('[PID %d] %.1f%% (%.1f FPS, %ds left)' % (os.getpid(), perc * 100.0, fps, est))
-            t_last = t
-            tm.reset()
-    logger.info('Finished.')
-
-    # export data
-    try:
-        chnames = [raw.ch_names[ch] for ch in chlist]
-        psd_all = np.array(psd_all)
-        [basedir, fname, fext] = qc.parse_path_list(rawfile)
-        fout_header = '%s/psd-%s-header.pkl' % (basedir, fname)
-        fout_psd = '%s/psd-%s-data.npy' % (basedir, fname)
-        header = {'psdfile':fout_psd, 'times':np.array(times), 'sfreq':sfreq,
-                  'channels':chnames, 'wframes':wframes, 'events':evelist}
-        qc.save_obj(fout_header, header)
-        np.save(fout_psd, psd_all)
-        logger.info('Exported to:\n(header) %s\n(numpy array) %s' % (fout_header, fout_psd))
-    except:
-        logger.exception('(%s) Unexpected error occurred while exporting data. Dropping you into a shell for recovery.' %\
-            os.path.basename(__file__))
-        embed()
+
+from __future__ import print_function, division
+
+"""
+Compute PSD features over a sliding window on the entire raw file
+
+Kyuhwa Lee
+Swiss Federal Institute of Technology (EPFL)
+
+"""
+
+# start
+import os
+import mne
+import numpy as np
+import neurodecode.utils.pycnbi_utils as pu
+import neurodecode.utils.q_common as qc
+from neurodecode import logger
+from IPython import embed
+
+mne.set_log_level('ERROR')
+os.environ['OMP_NUM_THREADS'] = '1' # actually improves performance for multitaper
+
+
+def raw2psd(rawfile=None, fmin=1, fmax=40, wlen=0.5, wstep=1, tmin=0.0, tmax=None,
+            channel_picks=None, excludes=[], n_jobs=1):
+    """
+    Compute PSD features over a sliding window on the entire raw file.
+    Leading edge of the window is the time reference, i.e. do not use future data.
+
+    Input
+    =====
+    rawfile: fif file.
+    channel_picks: None or list of channel names
+    tmin (sec): start time of the PSD window relative to the event onset.
+    tmax (sec): end time of the PSD window relative to the event onset. None = until the end.
+    fmin (Hz): minimum PSD frequency
+    fmax (Hz): maximum PSD frequency
+    wlen (sec): sliding window length for computing PSD (sec)
+    wstep (int): sliding window step (time samples)
+    excludes (list): list of channels to exclude
+    """
+
+    raw, eve = pu.load_raw(rawfile)
+    sfreq = raw.info['sfreq']
+    wframes = int(round(sfreq * wlen))
+    raw_eeg = raw.pick_types(meg=False, eeg=True, stim=False, exclude=excludes)
+    if channel_picks is None:
+        rawdata = raw_eeg._data
+        chlist = raw.ch_names
+    else:
+        chlist = []
+        for ch in channel_picks:
+            chlist.append(raw.ch_names.index(ch))
+        rawdata = raw_eeg._data[np.array(chlist)]
+
+    if tmax is None:
+        t_end = rawdata.shape[1]
+    else:
+        t_end = int(round(tmax * sfreq))
+    t_start = int(round(tmin * sfreq)) + wframes
+    psde = mne.decoding.PSDEstimator(sfreq, fmin=fmin, fmax=fmax, n_jobs=1,\
+        bandwidth=None, low_bias=True, adaptive=False, normalization='length',
+        verbose=None)
+    print('[PID %d] %s' % (os.getpid(), rawfile))
+    psd_all = []
+    evelist = []
+    times = []
+    t_len = t_end - t_start
+    last_eve = 0
+    y_i = 0
+    t_last = t_start
+    tm = qc.Timer()
+    for t in range(t_start, t_end, wstep):
+        # compute PSD
+        window = rawdata[:, t - wframes: t]
+        psd = psde.transform(window.reshape((1, window.shape[0], window.shape[1])))
+        psd = psd.reshape(psd.shape[1], psd.shape[2])
+        psd_all.append(psd)
+        times.append(t)
+
+        # matching events at the current window
+        if y_i < eve.shape[0] and t >= eve[y_i][0]:
+            last_eve = eve[y_i][2]
+            y_i += 1
+        evelist.append(last_eve)
+
+        if tm.sec() >= 1:
+            perc = (t - t_start) / t_len
+            fps = (t - t_last) / wstep
+            est = (t_end - t) / wstep / fps
+            logger.info('[PID %d] %.1f%% (%.1f FPS, %ds left)' % (os.getpid(), perc * 100.0, fps, est))
+            t_last = t
+            tm.reset()
+    logger.info('Finished.')
+
+    # export data
+    try:
+        chnames = [raw.ch_names[ch] for ch in chlist]
+        psd_all = np.array(psd_all)
+        [basedir, fname, fext] = qc.parse_path_list(rawfile)
+        fout_header = '%s/psd-%s-header.pkl' % (basedir, fname)
+        fout_psd = '%s/psd-%s-data.npy' % (basedir, fname)
+        header = {'psdfile':fout_psd, 'times':np.array(times), 'sfreq':sfreq,
+                  'channels':chnames, 'wframes':wframes, 'events':evelist}
+        qc.save_obj(fout_header, header)
+        np.save(fout_psd, psd_all)
+        logger.info('Exported to:\n(header) %s\n(numpy array) %s' % (fout_header, fout_psd))
+    except:
+        logger.exception('(%s) Unexpected error occurred while exporting data. Dropping you into a shell for recovery.' %\
+            os.path.basename(__file__))
+        embed()
```

### Comparing `neurodecode-2.0.4/neurodecode.egg-info/PKG-INFO` & `neurodecode-2.0.5/neurodecode.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,194 +1,194 @@
-Metadata-Version: 2.1
-Name: neurodecode
-Version: 2.0.4
-Summary: Real-time brain signal decoding framework
-Home-page: https://github.com/dbdq/neurodecode/
-Author: Kyuhwa Lee, Arnaud Desvachez
-Author-email: lee.kyuh@gmail.com, arnaud.desvachez@gmail.com
-License: The GNU General Public License
-Description-Content-Type: text/markdown
-
-# Introduction
-
-Neurodecode provides a real-time brain signal decoding framework. The decoding performance was recognised at [Microsoft Brain Signal Decoding competition](https://github.com/dbdq/microsoft_decoding) with the <i>First Prize Award</i> (2016) for high decoding accuracy (2nd out of 1863 algorithms). It has been applied on a couple of online decoding projects with various electrode types including EEG, ECoG and DBS, and on several acquisition systems including AntNeuro eego, g.tec gUSBamp, BioSemi ActiveTwo, BrainProducts actiCHamp and Wearable Sensing. With modular software design, the decoding runs at approximately 15 classifications per second(cps) on a 4th-gen i7 laptop with 64-channel setup at 512 Hz sampling rate. High-speed decoding up to 200 cps was achieved using process-interleaving technique on 8 cores. It has been tested on both Linux and Windows using Python 3.7.
-
-The underlying data communication is based on Lab Streaming Layer (LSL) which provides sub-millisecond time synchronization accuracy. Any signal acquisition system supported by native LSL or OpenVibe is also supported by Neurodecode. Since the data communication is based on TCP, signals can be also transmitted wirelessly. For more information about LSL, please visit:
-[https://github.com/sccn/labstreaminglayer](https://github.com/sccn/labstreaminglayer)
-
-
-# Important modules
-
-### StreamReceiver
-The base module for acquiring signals used by other modules such as Decoder, StreamViewer and StreamRecorder.
-
-### StreamViewer
-Visualize signals in real time with spectral filtering, common average filtering options and real-time FFT.
-
-### StreamRecorder
-Record signals into fif format, a standard format mainly used in [MNE EEG analysis library](http://martinos.org/mne/).
-
-### StreamPlayer
-Replay the recorded signals in real time as if it was transmitted from a real acquisition server.
-
-### Decoder
-This folder contains decoder and trainer modules. Currently, LDA, regularized LDA, Random Forests, and Gradient Boosting Machines are supported as the classifier type. Neural Network-based decoders are currently under experiment.
-
-### Protocols
-Contains some basic protocols for training and testing. Google Glass visual feedback is supported through USB communication.
-
-### Triggers
-Triggers are used to mark event (stimulus) timings during the recording. This folder contains common trigger event definition files. 
-
-### Utils
-Contains various utilities.
-
-
-# Prerequisites
-
-Anaconda is recommended for easy installation of Python environment.
-
-Neurodecode depends on following packages:
-  - scipy
-  - numpy
-  - PyQt5
-  - scikit-learn
-  - pylsl
-  - mne 0.14 or later
-  - matplotlib 2.1.0 or later
-  - pyqtgraph
-  - opencv-python
-  - pyserial
-  - future
-  - configparser
-  - xgboost
-  - psutil
-
-Optional but strongly recommended:
-  - [OpenVibe](http://openvibe.inria.fr/downloads)
-
-OpenVibe supports a wide range of acquisition servers and all acquisition systems supported by OpenVibe are supported by Neurodecode through LSL. Make sure you tick the checkbox "LSL_EnableLSLOutput" in Preferences when you run acquisition server. This will stream the data through the LSL network from which Neurodecode receives data. 
-
-# Installation
-
-Neurodecode can be installed from PyPI.
-```
-pip install neurodecode
-```
-
-To install the latest version, clone the repository and run setup script:
-```
-git clone https://github.com/dbdq/neurodecode.git
-python setup.py develop
-```
-Add "scripts" directory to PATH environment variable for convenient access to commonly used scripts.
-
-### PyQt version problem
-The Qt API is very sensitive to version and needs to be compatible with all dependencies.
-If you experience pyqtgraph complaining incompatible PyQt version (e.g. PyQt < 5.12), try:
-```
-conda remove pyqt
-pip install -U PyQt5
-```
-This can be caused by Anaconda not having the latest PyQt version.
-
-
-### For Windows users, increase timer resolution
-The default timer resolution in some Windows versions is 16 ms, which can limit the precision of timings. It is recommended to run the following tool and set the resolution to 1 ms or lower:
-[https://vvvv.org/contribution/windows-system-timer-tool](https://vvvv.org/contribution/windows-system-timer-tool)
-
-
-### Hardware triggering without legacy parallel port
-We have also developed an Arduino-based triggering system as we wanted to send triggers to a parallel port using standard USB ports. We achieved sub-millisecond extra latency compared to physical parallel port (150 +- 25 us). Experimental results using oscilloscope can be found in "doc" folder. The package can be downloaded by:
-```
-git clone https://github.com/dbdq/arduino-trigger.git
-```
-The customized firmware should be installed on Arduino Micro and the circuit design included in the document folder should be printed to a circuit board.
-
-
-### For g.USBamp users
-The following customized acquisition server is needed instead of default LSL app to receive the trigger channel as part of signal streaming channels:
-```
-git clone https://github.com/dbdq/gUSBamp_pycnbi.git
-```
-because the default gUSBamp LSL server do not stream event channel as part of the signal stream but as a separate server. The customized version supports simultaneous signal+event channel streaming. 
-
-
-### For AntNeuro eego users
-Use the OpenVibe acquisition server and make sure to check "LSL output" in preference.  If you don't see "eego" from the device selection, it's probably because you didn't install the additional drivers when you installed OpenVibe.
-
-<br>
-<br>
-
-# Running examples
-
-To run this example, copy the /sample folder to your local folder and cd into it.
-
-### 1. Play data
-Replay a pre-recorded EEG recording sample in real-time as if acquiring signals from brain with a chunk size of 8.
-The sample data was recorded using a 24-channel EEG system from a participant doing a left and right hand motor imagery.
-The hardware events recorded during the experiment is also streamed via LSL network.
-
-```nd_stream_player mi_left_right.fif 8```
-
-Screenshot of setting up an LSL server and streaming the recorded data.
-![image](https://user-images.githubusercontent.com/6797783/199510832-c10b7df9-193b-4396-a671-15f6f8df0226.png)
-
-### 2. Record data  
-Simulate real-time decoding from the brain. We are streaming the data using nd_stream_player script above while
-the receiver is source-agnostic, allowing the full simulation of replaying and the validation of data processing.  
-This step can be skipped if you create a folder ./fif/ and copy the sample fif file into ./fif/.
-
-```
-nd_stream_recorder $PWD # for Linux
-nd_stream_recorder %CD% # for Windows
-```
-![image](https://user-images.githubusercontent.com/6797783/199511174-abb1ac03-eadc-488d-833a-6e303a93e331.png)
-
-### 3. Real-time signal visualisation (choose StreamPlayer from the list)  
-```nd_stream_viewer```
-
-Sample visualisation of streamed signals. Cursor keys allow different amplitude and time scalings.
-![image](https://user-images.githubusercontent.com/6797783/199509891-a0f30cfd-c589-4004-89f0-c71ff08b4071.png)
-
-### 4. Run an offline protocol for training
-Runs an offline training protocol. This step is just for explanation purpose and can be skipped.  
-```nd_train_mi ./config_offline.py```
-
-Snapshot of the offline protocol.  
-![image](https://user-images.githubusercontent.com/6797783/199511602-6bec54d0-50dd-485c-8d3e-6fa7621cc773.png)
-
-### 5. Train a decoder  
-Train a decoder using the fif file with defined events. In this example, it is left (event 11) vs right (event 9) hand motor imagery.  
-Events are defined in mi_left_right_events.ini file.
-
-```nd_trainer ./config_trainer.py```
-
-### 6. Run an online protocol for testing
-The provided sample is set to 60 seconds time-out without early termination so you can see
-the decoder output changes to left or right when the left (event 11) or right(event 9) is emitted 
-from the stream player terminal. Other events such as rest is undefined and will behave in random direction.
-
-```nd_test_mi config_online.py```
-
-Snapshot of the protocol showing the bar position.  
-![image](https://user-images.githubusercontent.com/6797783/199517521-de33e4f2-92bf-421f-8afc-9eee5c899a04.png)  
-
-Sample decoder output with probabilities and the corresponding bar position, which represents the accumulated probabilities.  
-![image](https://user-images.githubusercontent.com/6797783/199518166-67f8a4ea-dde9-4544-b95d-80ed5f0526aa.png)  
-
-Example of events being emitted from the stream player.  
-![image](https://user-images.githubusercontent.com/6797783/199514155-a94bbb71-c2dc-43d5-81e8-2bd4916a05e4.png)  
-
-There are still plenty of possibilities to optimize the speed in many parts of the code. Any contribution is welcome. Please contact lee.kyuh@gmail.com for any comment / feedback.
-
-
-# Copyright and license
-The codes are released under [GNU General Public License](https://www.gnu.org/licenses/gpl-3.0.en.html).
-
-
-# Citation
-This package was developed as part of the following works:
-  - Yohann Thenaisie* and Kyuhwa Lee* <i>et al.</i>, "Principles of gait encoding in the subthalamic nucleus of people with Parkinson's disease", <i>Science Translational Medicine</i>, 2022, Vol. 14, No. 661, p. eabo1800.<br>(* first authors as equal contribution)
-  - Kyuhwa Lee <i>et al.</i>, "A Brain-Controlled Exoskeleton with Cascaded Event-Related Desynchronization Classifiers", <i>Robotics and Autonomous Systems</i>, Elsevier, 2016, p. 15-23.
-   
-If some of the code here were useful or helpful for your project, I would greatly appreciate if you could cite one of the above papers.
+Metadata-Version: 2.1
+Name: neurodecode
+Version: 2.0.5
+Summary: Real-time brain signal decoding framework
+Home-page: https://github.com/dbdq/neurodecode/
+Author: Kyuhwa Lee, Arnaud Desvachez
+Author-email: lee.kyuh@gmail.com, arnaud.desvachez@gmail.com
+License: The GNU General Public License
+Description-Content-Type: text/markdown
+
+# Introduction
+
+Neurodecode provides a real-time brain signal decoding framework. The decoding performance was recognised at [Microsoft Brain Signal Decoding competition](https://github.com/dbdq/microsoft_decoding) with the <i>First Prize Award</i> (2016) for high decoding accuracy (2nd out of 1863 algorithms). It has been applied on a couple of online decoding projects with various electrode types including EEG, ECoG and DBS, and on several acquisition systems including AntNeuro eego, g.tec gUSBamp, BioSemi ActiveTwo, BrainProducts actiCHamp and Wearable Sensing. With modular software design, the decoding runs at approximately 15 classifications per second(cps) on a 4th-gen i7 laptop with 64-channel setup at 512 Hz sampling rate. High-speed decoding up to 200 cps was achieved using process-interleaving technique on 8 cores. It has been tested on both Linux and Windows using Python 3.7.
+
+The underlying data communication is based on Lab Streaming Layer (LSL) which provides sub-millisecond time synchronization accuracy. Any signal acquisition system supported by native LSL or OpenVibe is also supported by Neurodecode. Since the data communication is based on TCP, signals can be also transmitted wirelessly. For more information about LSL, please visit:
+[https://github.com/sccn/labstreaminglayer](https://github.com/sccn/labstreaminglayer)
+
+
+# Important modules
+
+### StreamReceiver
+The base module for acquiring signals used by other modules such as Decoder, StreamViewer and StreamRecorder.
+
+### StreamViewer
+Visualize signals in real time with spectral filtering, common average filtering options and real-time FFT.
+
+### StreamRecorder
+Record signals into fif format, a standard format mainly used in [MNE EEG analysis library](http://martinos.org/mne/).
+
+### StreamPlayer
+Replay the recorded signals in real time as if it was transmitted from a real acquisition server.
+
+### Decoder
+This folder contains decoder and trainer modules. Currently, LDA, regularized LDA, Random Forests, and Gradient Boosting Machines are supported as the classifier type. Neural Network-based decoders are currently under experiment.
+
+### Protocols
+Contains some basic protocols for training and testing. Google Glass visual feedback is supported through USB communication.
+
+### Triggers
+Triggers are used to mark event (stimulus) timings during the recording. This folder contains common trigger event definition files. 
+
+### Utils
+Contains various utilities.
+
+
+# Prerequisites
+
+Anaconda is recommended for easy installation of Python environment.
+
+Neurodecode depends on following packages:
+  - scipy
+  - numpy
+  - PyQt5
+  - scikit-learn
+  - pylsl
+  - mne 0.14 or later
+  - matplotlib 2.1.0 or later
+  - pyqtgraph
+  - opencv-python
+  - pyserial
+  - future
+  - configparser
+  - xgboost
+  - psutil
+
+Optional but strongly recommended:
+  - [OpenVibe](http://openvibe.inria.fr/downloads)
+
+OpenVibe supports a wide range of acquisition servers and all acquisition systems supported by OpenVibe are supported by Neurodecode through LSL. Make sure you tick the checkbox "LSL_EnableLSLOutput" in Preferences when you run acquisition server. This will stream the data through the LSL network from which Neurodecode receives data. 
+
+# Installation
+
+Neurodecode can be installed from PyPI.
+```
+pip install neurodecode
+```
+
+To install the latest version, clone the repository and run setup script:
+```
+git clone https://github.com/dbdq/neurodecode.git
+python setup.py develop
+```
+Add "scripts" directory to PATH environment variable for convenient access to commonly used scripts.
+
+### PyQt version problem
+The Qt API is very sensitive to version and needs to be compatible with all dependencies.
+If you experience pyqtgraph complaining incompatible PyQt version (e.g. PyQt < 5.12), try:
+```
+conda remove pyqt
+pip install -U PyQt5
+```
+This can be caused by Anaconda not having the latest PyQt version.
+
+
+### For Windows users, increase timer resolution
+The default timer resolution in some Windows versions is 16 ms, which can limit the precision of timings. It is recommended to run the following tool and set the resolution to 1 ms or lower:
+[https://vvvv.org/contribution/windows-system-timer-tool](https://vvvv.org/contribution/windows-system-timer-tool)
+
+
+### Hardware triggering without legacy parallel port
+We have also developed an Arduino-based triggering system as we wanted to send triggers to a parallel port using standard USB ports. We achieved sub-millisecond extra latency compared to physical parallel port (150 +- 25 us). Experimental results using oscilloscope can be found in "doc" folder. The package can be downloaded by:
+```
+git clone https://github.com/dbdq/arduino-trigger.git
+```
+The customized firmware should be installed on Arduino Micro and the circuit design included in the document folder should be printed to a circuit board.
+
+
+### For g.USBamp users
+The following customized acquisition server is needed instead of default LSL app to receive the trigger channel as part of signal streaming channels:
+```
+git clone https://github.com/dbdq/gUSBamp_pycnbi.git
+```
+because the default gUSBamp LSL server do not stream event channel as part of the signal stream but as a separate server. The customized version supports simultaneous signal+event channel streaming. 
+
+
+### For AntNeuro eego users
+Use the OpenVibe acquisition server and make sure to check "LSL output" in preference.  If you don't see "eego" from the device selection, it's probably because you didn't install the additional drivers when you installed OpenVibe.
+
+<br>
+<br>
+
+# Running examples
+
+To run this example, copy the /sample folder to your local folder and cd into it.
+
+### 1. Play data
+Replay a pre-recorded EEG recording sample in real-time as if acquiring signals from brain with a chunk size of 8.
+The sample data was recorded using a 24-channel EEG system from a participant doing a left and right hand motor imagery.
+The hardware events recorded during the experiment is also streamed via LSL network.
+
+```nd_stream_player mi_left_right.fif 8```
+
+Screenshot of setting up an LSL server and streaming the recorded data.
+![image](https://user-images.githubusercontent.com/6797783/199510832-c10b7df9-193b-4396-a671-15f6f8df0226.png)
+
+### 2. Record data  
+Simulate real-time decoding from the brain. We are streaming the data using nd_stream_player script above while
+the receiver is source-agnostic, allowing the full simulation of replaying and the validation of data processing.  
+This step can be skipped if you create a folder ./fif/ and copy the sample fif file into ./fif/.
+
+```
+nd_stream_recorder $PWD # for Linux
+nd_stream_recorder %CD% # for Windows
+```
+![image](https://user-images.githubusercontent.com/6797783/199511174-abb1ac03-eadc-488d-833a-6e303a93e331.png)
+
+### 3. Real-time signal visualisation (choose StreamPlayer from the list)  
+```nd_stream_viewer```
+
+Sample visualisation of streamed signals. Cursor keys allow different amplitude and time scalings.
+![image](https://user-images.githubusercontent.com/6797783/199509891-a0f30cfd-c589-4004-89f0-c71ff08b4071.png)
+
+### 4. Run an offline protocol for training
+Runs an offline training protocol. This step is just for explanation purpose and can be skipped.  
+```nd_train_mi ./config_offline.py```
+
+Snapshot of the offline protocol.  
+![image](https://user-images.githubusercontent.com/6797783/199511602-6bec54d0-50dd-485c-8d3e-6fa7621cc773.png)
+
+### 5. Train a decoder  
+Train a decoder using the fif file with defined events. In this example, it is left (event 11) vs right (event 9) hand motor imagery.  
+Events are defined in mi_left_right_events.ini file.
+
+```nd_trainer ./config_trainer.py```
+
+### 6. Run an online protocol for testing
+The provided sample is set to 60 seconds time-out without early termination so you can see
+the decoder output changes to left or right when the left (event 11) or right(event 9) is emitted 
+from the stream player terminal. Other events such as rest is undefined and will behave in random direction.
+
+```nd_test_mi config_online.py```
+
+Snapshot of the protocol showing the bar position.  
+![image](https://user-images.githubusercontent.com/6797783/199517521-de33e4f2-92bf-421f-8afc-9eee5c899a04.png)  
+
+Sample decoder output with probabilities and the corresponding bar position, which represents the accumulated probabilities.  
+![image](https://user-images.githubusercontent.com/6797783/199518166-67f8a4ea-dde9-4544-b95d-80ed5f0526aa.png)  
+
+Example of events being emitted from the stream player.  
+![image](https://user-images.githubusercontent.com/6797783/199514155-a94bbb71-c2dc-43d5-81e8-2bd4916a05e4.png)  
+
+There are still plenty of possibilities to optimize the speed in many parts of the code. Any contribution is welcome. Please contact lee.kyuh@gmail.com for any comment / feedback.
+
+
+# Copyright and license
+The codes are released under [GNU General Public License](https://www.gnu.org/licenses/gpl-3.0.en.html).
+
+
+# Citation
+This package was developed as part of the following works:
+  - Yohann Thenaisie* and Kyuhwa Lee* <i>et al.</i>, "Principles of gait encoding in the subthalamic nucleus of people with Parkinson's disease", <i>Science Translational Medicine</i>, 2022, Vol. 14, No. 661, p. eabo1800.<br>(* first authors as equal contribution)
+  - Kyuhwa Lee <i>et al.</i>, "A Brain-Controlled Exoskeleton with Cascaded Event-Related Desynchronization Classifiers", <i>Robotics and Autonomous Systems</i>, Elsevier, 2016, p. 15-23.
+   
+If some of the code here were useful or helpful for your project, I would greatly appreciate if you could cite one of the above papers.
```

### Comparing `neurodecode-2.0.4/neurodecode.egg-info/SOURCES.txt` & `neurodecode-2.0.5/neurodecode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.4/neurodecode.egg-info/entry_points.txt` & `neurodecode-2.0.5/neurodecode.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `neurodecode-2.0.4/setup.py` & `neurodecode-2.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from setuptools import find_packages, setup
-
-# backward compatibility for old pycnbi users
-'''
-# symlink pycnbi to neurodecode
-import os
-import sys
-if not os.path.exists('./pycnbi'):
-    if sys.platform.startswith('win'):
-        os.system('mklink pycnbi neurodecode /J')
-    else:
-        os.symlink('./neurodecode', './pycnbi', True)
-'''
-
-setup(
-    name='neurodecode',
-    version='2.0.4',
-    author='Kyuhwa Lee, Arnaud Desvachez',
-    author_email='lee.kyuh@gmail.com, arnaud.desvachez@gmail.com',
-    license='The GNU General Public License',
-    url='https://github.com/dbdq/neurodecode/',
-    description='Real-time brain signal decoding framework',
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
-    packages=find_packages(),
-    package_data={'neurodecode.stream_viewer':['*.ini']},
-    install_requires=[
-        'h5py>=2.7',
-        'opencv_python>=3.4',
-        'numpy>=1.16',
-        'scipy>=1.2',
-        'colorama>=0.3.9',
-        'xgboost>=0.81',
-        'matplotlib>=3.0.2',
-        'mne>=0.16',
-        'psutil>=5.4.8',
-        'setuptools>=39.0.1',
-        'pyqtgraph>=0.13',
-        'pylsl>=1.12.2',
-        'ipython>=6',
-        'PyQt5>=5',
-        'pyxdf>=1.15.2',
-        'pyserial>=3.4',
-        'simplejson>=3.16.0',
-        'scikit_learn>=0.21',
-        'future',
-        'configparser',
-        'lightgbm>=2.3',
-        'mat73'
-    ],
-    entry_points = {'console_scripts':[
-        'nd_stream_viewer=neurodecode.stream_viewer.stream_viewer:main',
-        'nd_fif_info=neurodecode.utils.fif_info:main',
-        'nd_fif_resample=neurodecode.utils.fif_resample:main',
-        'nd_fif2mat=neurodecode.utils.fif2mat:main',
-        'nd_add_lsl_events=neurodecode.utils.add_lsl_events:main',
-        'nd_parse_features=neurodecode.analysis.parse_features:main',
-        'nd_convert2fif=neurodecode.utils.convert2fif:main',
-        'nd_train_mi=neurodecode.protocols.mi.train_mi:main',
-        'nd_test_mi=neurodecode.protocols.mi.test_mi:main',
-        'nd_stream_player=neurodecode.stream_player.stream_player:main',
-        'nd_stream_recorder=neurodecode.stream_recorder.stream_recorder:main',
-        'nd_tfr_export=neurodecode.analysis.tfr_export:main',
-        'nd_trainer=neurodecode.decoder.trainer:main',
-        'nd_decoder=neurodecode.decoder.decoder:main'
-    ]}
-)
+from setuptools import find_packages, setup
+
+# backward compatibility for old pycnbi users
+'''
+# symlink pycnbi to neurodecode
+import os
+import sys
+if not os.path.exists('./pycnbi'):
+    if sys.platform.startswith('win'):
+        os.system('mklink pycnbi neurodecode /J')
+    else:
+        os.symlink('./neurodecode', './pycnbi', True)
+'''
+
+setup(
+    name='neurodecode',
+    version='2.0.5',
+    author='Kyuhwa Lee, Arnaud Desvachez',
+    author_email='lee.kyuh@gmail.com, arnaud.desvachez@gmail.com',
+    license='The GNU General Public License',
+    url='https://github.com/dbdq/neurodecode/',
+    description='Real-time brain signal decoding framework',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
+    packages=find_packages(),
+    package_data={'neurodecode.stream_viewer':['*.ini']},
+    install_requires=[
+        'h5py>=2.7',
+        'opencv_python>=3.4',
+        'numpy>=1.16',
+        'scipy>=1.2',
+        'colorama>=0.3.9',
+        'xgboost>=0.81',
+        'matplotlib>=3.0.2',
+        'mne>=0.16',
+        'psutil>=5.4.8',
+        'setuptools>=39.0.1',
+        'pyqtgraph>=0.13',
+        'pylsl>=1.12.2',
+        'ipython>=6',
+        'PyQt5>=5',
+        'pyxdf>=1.15.2',
+        'pyserial>=3.4',
+        'simplejson>=3.16.0',
+        'scikit_learn>=0.21',
+        'future',
+        'configparser',
+        'lightgbm>=2.3',
+        'mat73'
+    ],
+    entry_points = {'console_scripts':[
+        'nd_stream_viewer=neurodecode.stream_viewer.stream_viewer:main',
+        'nd_fif_info=neurodecode.utils.fif_info:main',
+        'nd_fif_resample=neurodecode.utils.fif_resample:main',
+        'nd_fif2mat=neurodecode.utils.fif2mat:main',
+        'nd_add_lsl_events=neurodecode.utils.add_lsl_events:main',
+        'nd_parse_features=neurodecode.analysis.parse_features:main',
+        'nd_convert2fif=neurodecode.utils.convert2fif:main',
+        'nd_train_mi=neurodecode.protocols.mi.train_mi:main',
+        'nd_test_mi=neurodecode.protocols.mi.test_mi:main',
+        'nd_stream_player=neurodecode.stream_player.stream_player:main',
+        'nd_stream_recorder=neurodecode.stream_recorder.stream_recorder:main',
+        'nd_tfr_export=neurodecode.analysis.tfr_export:main',
+        'nd_trainer=neurodecode.decoder.trainer:main',
+        'nd_decoder=neurodecode.decoder.decoder:main'
+    ]}
+)
```

