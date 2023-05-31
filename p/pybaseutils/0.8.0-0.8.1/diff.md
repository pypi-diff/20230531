# Comparing `tmp/pybaseutils-0.8.0.tar.gz` & `tmp/pybaseutils-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pybaseutils-0.8.0.tar", last modified: Wed Apr 19 09:08:10 2023, max compression
+gzip compressed data, was "dist/pybaseutils-0.8.1.tar", last modified: Wed May 31 02:57:58 2023, max compression
```

## Comparing `pybaseutils-0.8.0.tar` & `pybaseutils-0.8.1.tar`

### file list

```diff
@@ -1,119 +1,135 @@
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-0.8.0/LICENCE
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3952 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/PKG-INFO
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/base64_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2155 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/batch_utils.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils/cluster/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/cluster/kmean.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/cluster/maxmin_distance.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/cluster/similarity.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/cluster/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-0.8.0/pybaseutils/color_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-0.8.0/pybaseutils/config_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    10076 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/coords_utils.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils/cvutils/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7528 2022-11-25 09:29:09.000000 pybaseutils-0.8.0/pybaseutils/cvutils/corner_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/cvutils/mouse_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7784 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/cvutils/video_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-0.8.0/pybaseutils/cvutils/__init__.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils/dataloader/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7363 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/dataloader/dataset.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    12136 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/dataloader/parser_labelme.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    11897 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/dataloader/parser_textdata.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    19470 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/dataloader/parser_voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/dataloader/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    32583 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/file_utils.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils/font_style/
--rwxrwxrwx   0 dm        (1000) dm        (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/font_style/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/font_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    13053 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/geometry_tools.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5306 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/heatmap_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    95465 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/image_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4255 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/json_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/log.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-0.8.0/pybaseutils/logger.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils/maker/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4645 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/maker/convert_labelme2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4366 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/maker/convert_voc2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     6204 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/maker/convert_voc2yolo.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3508 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/maker/convert_yolo2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1651 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/maker/maker_labelme.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    17365 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/maker/maker_voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/maker/__init__.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils/metrics/
--rwxrwxrwx   0 dm        (1000) dm        (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/metrics/accuracy.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/metrics/average_meter.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/metrics/class_report.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/metrics/plot_pr.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/metrics/plot_roc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/metrics/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    19288 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/numpy_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2090 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/pandas_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7522 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/plot_utils.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils/pycpp/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-0.8.0/pybaseutils/pycpp/demo.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/pycpp/main.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-0.8.0/pybaseutils/pycpp/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-0.8.0/pybaseutils/setup_config.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7283 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/thread_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/time_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/tracemalloc_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-0.8.0/pybaseutils/tracemalloc_utils2.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils/transforms/
--rwxrwxrwx   0 dm        (1000) dm        (1000)    24116 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/transforms/affine_transform.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/transforms/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)    13621 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/pybaseutils/word_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4095 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/pybaseutils/worker.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-0.8.0/pybaseutils/yaml_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      137 2023-04-19 09:08:03.000000 pybaseutils-0.8.0/pybaseutils/__init__.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils.egg-info/
--rwxrwxrwx   0 dm        (1000) dm        (1000)        1 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dm        (1000) dm        (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-0.8.0/pybaseutils.egg-info/not-zip-safe
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3952 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils.egg-info/PKG-INFO
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3054 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dm        (1000) dm        (1000)       20 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/pybaseutils.egg-info/top_level.txt
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3374 2023-03-01 06:33:08.000000 pybaseutils-0.8.0/README.md
--rwxrwxrwx   0 dm        (1000) dm        (1000)       38 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/setup.cfg
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2213 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/setup.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/test_py/
--rwxrwxrwx   0 dm        (1000) dm        (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-0.8.0/test_py/class_names.py
-drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-04-19 09:08:10.000000 pybaseutils-0.8.0/test_py/converter/
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-0.8.0/test_py/converter/AffectNet.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3472 2023-03-11 01:43:26.000000 pybaseutils-0.8.0/test_py/converter/AsianMovie.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3693 2022-12-13 08:38:36.000000 pybaseutils-0.8.0/test_py/converter/BITVehicle2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4577 2022-12-13 08:38:36.000000 pybaseutils-0.8.0/test_py/converter/BSTLD2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5580 2023-01-18 07:11:31.000000 pybaseutils-0.8.0/test_py/converter/CCPD.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7024 2023-01-18 07:11:16.000000 pybaseutils-0.8.0/test_py/converter/CCPD2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4942 2023-03-14 10:27:29.000000 pybaseutils-0.8.0/test_py/converter/detect_face_person.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1203 2023-04-12 08:06:30.000000 pybaseutils-0.8.0/test_py/converter/insects_for_aichallenger.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2568 2023-04-10 08:35:17.000000 pybaseutils-0.8.0/test_py/converter/TT100K.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-0.8.0/test_py/converter/tt100k_utils.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7592 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/test_py/converter/ua_detrac2voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/test_py/converter/__init__.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      830 2023-04-12 02:15:23.000000 pybaseutils-0.8.0/test_py/demo1.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1111 2023-03-31 03:30:19.000000 pybaseutils-0.8.0/test_py/demo2.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     4533 2023-04-15 03:49:32.000000 pybaseutils-0.8.0/test_py/demo_copy_files.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2132 2023-02-27 02:15:50.000000 pybaseutils-0.8.0/test_py/demo_copy_files_for_voc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-0.8.0/test_py/demo_correction_v1.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     5657 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/test_py/demo_correction_v2.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/test_py/demo_correction_v3.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-0.8.0/test_py/demo_for_trt.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2877 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/test_py/demo_get_file_list.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      667 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/test_py/demo_gif.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/test_py/demo_metrics.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/test_py/demo_mouse.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2085 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/test_py/demo_pandas.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-0.8.0/test_py/demo_plot.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-0.8.0/test_py/demo_standard_image .py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      861 2023-03-21 08:22:16.000000 pybaseutils-0.8.0/test_py/demo_standard_video .py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/test_py/demo_taichi.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1891 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/test_py/demo_video.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3267 2023-04-19 06:55:52.000000 pybaseutils-0.8.0/test_py/demo_voc_crop.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2374 2023-04-18 03:49:38.000000 pybaseutils-0.8.0/test_py/demo_voc_vis.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-0.8.0/test_py/demo_word_similar.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/test_py/demo_worker1.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-0.8.0/test_py/demo_worker2.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-0.8.0/test_py/men_tracemalloc.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-0.8.0/test_py/performance.py
--rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.0/test_py/__init__.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-0.8.1/LICENCE
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3952 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/PKG-INFO
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/base64_utils.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/base_audio/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4792 2023-05-16 07:29:26.000000 pybaseutils-0.8.1/pybaseutils/base_audio/audio_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-0.8.1/pybaseutils/base_audio/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2155 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/batch_utils.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/cluster/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/cluster/kmean.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/cluster/maxmin_distance.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/cluster/similarity.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/cluster/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-0.8.1/pybaseutils/color_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-0.8.1/pybaseutils/config_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    10076 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/coords_utils.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/cvutils/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7528 2022-11-25 09:29:09.000000 pybaseutils-0.8.1/pybaseutils/cvutils/corner_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/cvutils/mouse_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7804 2023-05-24 02:10:31.000000 pybaseutils-0.8.1/pybaseutils/cvutils/video_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-0.8.1/pybaseutils/cvutils/__init__.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/dataloader/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7363 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/dataloader/dataset.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    12136 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/dataloader/parser_labelme.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    11897 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/dataloader/parser_textdata.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    19470 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/dataloader/parser_voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/dataloader/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    32583 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/file_utils.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/font_style/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/font_style/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/font_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    13053 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/geometry_tools.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5306 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/heatmap_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    97144 2023-05-30 10:28:33.000000 pybaseutils-0.8.1/pybaseutils/image_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4255 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/json_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/log.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-0.8.1/pybaseutils/logger.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/maker/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4645 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/maker/convert_labelme2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4366 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/maker/convert_voc2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     6204 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/maker/convert_voc2yolo.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3508 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/maker/convert_yolo2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1651 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/maker/maker_labelme.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    17365 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/maker/maker_voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/maker/__init__.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/metrics/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/metrics/accuracy.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/metrics/average_meter.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/metrics/class_report.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/metrics/plot_pr.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/metrics/plot_roc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/metrics/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    19288 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/numpy_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2090 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/pandas_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-0.8.1/pybaseutils/plot_utils.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/pycpp/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-0.8.1/pybaseutils/pycpp/demo.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/pycpp/main.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-0.8.1/pybaseutils/pycpp/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-0.8.1/pybaseutils/setup_config.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7283 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/thread_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/time_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/tracemalloc_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-0.8.1/pybaseutils/tracemalloc_utils2.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils/transforms/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    24116 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/pybaseutils/transforms/affine_transform.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/pybaseutils/transforms/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-0.8.1/pybaseutils/word_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-0.8.1/pybaseutils/worker.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-0.8.1/pybaseutils/yaml_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      137 2023-05-31 02:57:56.000000 pybaseutils-0.8.1/pybaseutils/__init__.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils.egg-info/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)        1 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dm        (1000) dm        (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-0.8.1/pybaseutils.egg-info/not-zip-safe
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3952 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3460 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dm        (1000) dm        (1000)       20 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/pybaseutils.egg-info/top_level.txt
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3374 2023-03-01 06:33:08.000000 pybaseutils-0.8.1/README.md
+-rwxrwxrwx   0 dm        (1000) dm        (1000)       38 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/setup.cfg
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2213 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/setup.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/test_py/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-0.8.1/test_py/class_names.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/test_py/converter/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-0.8.1/test_py/converter/AffectNet.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3472 2023-03-11 01:43:26.000000 pybaseutils-0.8.1/test_py/converter/AsianMovie.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3693 2022-12-13 08:38:36.000000 pybaseutils-0.8.1/test_py/converter/BITVehicle2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4577 2022-12-13 08:38:36.000000 pybaseutils-0.8.1/test_py/converter/BSTLD2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5580 2023-01-18 07:11:31.000000 pybaseutils-0.8.1/test_py/converter/CCPD.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7024 2023-01-18 07:11:16.000000 pybaseutils-0.8.1/test_py/converter/CCPD2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1203 2023-04-12 08:06:30.000000 pybaseutils-0.8.1/test_py/converter/insects_for_aichallenger.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2568 2023-04-10 08:35:17.000000 pybaseutils-0.8.1/test_py/converter/TT100K.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-0.8.1/test_py/converter/tt100k_utils.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7592 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/test_py/converter/ua_detrac2voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/test_py/converter/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1733 2023-05-11 03:26:39.000000 pybaseutils-0.8.1/test_py/demo1.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1189 2023-05-30 10:27:09.000000 pybaseutils-0.8.1/test_py/demo2.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-0.8.1/test_py/demo_async_await1.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1194 2023-05-25 05:49:48.000000 pybaseutils-0.8.1/test_py/demo_async_await2.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     4533 2023-04-15 03:49:32.000000 pybaseutils-0.8.1/test_py/demo_copy_files.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2132 2023-02-27 02:15:50.000000 pybaseutils-0.8.1/test_py/demo_copy_files_for_voc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1342 2023-05-16 02:22:22.000000 pybaseutils-0.8.1/test_py/demo_ffmpy.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-0.8.1/test_py/demo_for_trt.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2877 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/test_py/demo_get_file_list.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      667 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/test_py/demo_gif.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1745 2023-05-24 03:16:30.000000 pybaseutils-0.8.1/test_py/demo_gif_video.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/test_py/demo_metrics.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/test_py/demo_mouse.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2085 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/test_py/demo_pandas.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-0.8.1/test_py/demo_plot.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-0.8.1/test_py/demo_standard_image .py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      863 2023-04-19 10:05:09.000000 pybaseutils-0.8.1/test_py/demo_standard_video .py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/test_py/demo_taichi.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      669 2023-04-23 09:10:41.000000 pybaseutils-0.8.1/test_py/demo_video.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3267 2023-04-19 06:55:52.000000 pybaseutils-0.8.1/test_py/demo_voc_crop.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2374 2023-04-18 03:49:38.000000 pybaseutils-0.8.1/test_py/demo_voc_vis.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-0.8.1/test_py/demo_word_similar.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/test_py/demo_worker1.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/test_py/demo_worker2.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/test_py/detector/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     6671 2023-05-04 08:11:18.000000 pybaseutils-0.8.1/test_py/detector/detect_face_person.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-0.8.1/test_py/detector/__init__.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/test_py/flask_demo/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-0.8.1/test_py/flask_demo/func.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-0.8.1/test_py/flask_demo/server.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-0.8.1/test_py/flask_demo/__init__.py
+drwxrwxrwx   0 dm        (1000) dm        (1000)        0 2023-05-31 02:57:58.000000 pybaseutils-0.8.1/test_py/image_correction/
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-0.8.1/test_py/image_correction/demo_correction_v1.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     5657 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/test_py/image_correction/demo_correction_v2.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-0.8.1/test_py/image_correction/demo_correction_v3.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-0.8.1/test_py/image_correction/__init__.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-0.8.1/test_py/kafka_worker.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-0.8.1/test_py/men_tracemalloc.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-0.8.1/test_py/performance.py
+-rwxrwxrwx   0 dm        (1000) dm        (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-0.8.1/test_py/__init__.py
```

### Comparing `pybaseutils-0.8.0/LICENCE` & `pybaseutils-0.8.1/LICENCE`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/PKG-INFO` & `pybaseutils-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 0.8.0
+Version: 0.8.1
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENCE
```

### Comparing `pybaseutils-0.8.0/pybaseutils/base64_utils.py` & `pybaseutils-0.8.1/pybaseutils/base64_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/batch_utils.py` & `pybaseutils-0.8.1/pybaseutils/batch_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/cluster/kmean.py` & `pybaseutils-0.8.1/pybaseutils/cluster/kmean.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/cluster/maxmin_distance.py` & `pybaseutils-0.8.1/pybaseutils/cluster/maxmin_distance.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/cluster/similarity.py` & `pybaseutils-0.8.1/pybaseutils/cluster/similarity.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/color_utils.py` & `pybaseutils-0.8.1/pybaseutils/color_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/config_utils.py` & `pybaseutils-0.8.1/pybaseutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/coords_utils.py` & `pybaseutils-0.8.1/pybaseutils/coords_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/cvutils/corner_utils.py` & `pybaseutils-0.8.1/pybaseutils/cvutils/corner_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/cvutils/mouse_utils.py` & `pybaseutils-0.8.1/pybaseutils/cvutils/mouse_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/cvutils/video_utils.py` & `pybaseutils-0.8.1/pybaseutils/cvutils/video_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,15 @@
     count = 0
     frames = []
     while True:
         if count % interval == 0 and count >= 0:
             # 设置抽帧的位置
             video_cap.set(cv2.CAP_PROP_POS_FRAMES, count)
             isSuccess, frame = video_cap.read()
-            if not isSuccess:
-                break
+            if not isSuccess or count > num_frames: break
             if func:
                 frame = func(frame)
             if vis:
                 image_utils.cv_show_image("frame", frame, use_rgb=False, delay=30)
             frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
             frames.append(frame)
         count += 1
@@ -72,15 +71,15 @@
     """
     name = os.path.basename(video_file).split(".")[0]
     if not out_dir:  out_dir = os.path.join(os.path.dirname(video_file), name)
     video_cap = get_video_capture(video_file)
     width, height, num_frames, fps = get_video_info(video_cap)
     if not os.path.exists(out_dir): os.makedirs(out_dir)
     count = 0
-    while True:
+    while count < num_frames:
         if count % interval == 0:
             # 设置抽帧的位置
             video_cap.set(cv2.CAP_PROP_POS_FRAMES, count)
             isSuccess, frame = video_cap.read()
             if not isSuccess:
                 break
             if func:
```

### Comparing `pybaseutils-0.8.0/pybaseutils/dataloader/dataset.py` & `pybaseutils-0.8.1/pybaseutils/dataloader/dataset.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/dataloader/parser_labelme.py` & `pybaseutils-0.8.1/pybaseutils/dataloader/parser_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/dataloader/parser_textdata.py` & `pybaseutils-0.8.1/pybaseutils/dataloader/parser_textdata.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/dataloader/parser_voc.py` & `pybaseutils-0.8.1/pybaseutils/dataloader/parser_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/file_utils.py` & `pybaseutils-0.8.1/pybaseutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/font_style/__init__.py` & `pybaseutils-0.8.1/pybaseutils/font_style/__init__.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/font_utils.py` & `pybaseutils-0.8.1/pybaseutils/font_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/geometry_tools.py` & `pybaseutils-0.8.1/pybaseutils/geometry_tools.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/heatmap_utils.py` & `pybaseutils-0.8.1/pybaseutils/heatmap_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/image_utils.py` & `pybaseutils-0.8.1/pybaseutils/image_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,22 +21,31 @@
 from typing import List, Dict, Tuple
 from PIL import ImageDraw, ImageFont
 from math import cos, sin
 from pybaseutils import file_utils
 from pybaseutils.coords_utils import *
 from pybaseutils.transforms import affine_transform
 
-color_map = [(0, 0, 0), (0, 0, 255), (0, 255, 0), (255, 0, 0),
-             (128, 0, 0), (0, 128, 0), (128, 128, 0),
-             (0, 0, 128), (128, 0, 128), (0, 128, 128), (128, 128, 128),
-             (64, 0, 0), (192, 0, 0), (64, 128, 0), (192, 128, 0),
-             (64, 0, 128), (192, 0, 128), (64, 128, 128), (192, 128, 128),
-             (0, 64, 0), (128, 64, 0), (0, 192, 0), (128, 192, 0), (0, 64, 128)] * 100
-
-ROOT = os.path.dirname(__file__)
+color_map2 = [(0, 0, 0), (0, 0, 255), (0, 255, 0), (255, 0, 0),
+              (128, 0, 0), (0, 128, 0), (128, 128, 0),
+              (0, 0, 128), (128, 0, 128), (0, 128, 128), (128, 128, 128),
+              (64, 0, 0), (192, 0, 0), (64, 128, 0), (192, 128, 0),
+              (64, 0, 128), (192, 0, 128), (64, 128, 128), (192, 128, 128),
+              (0, 64, 0), (128, 64, 0), (0, 192, 0), (128, 192, 0), (0, 64, 128)] * 100
+
+color_map = [(0, 0, 0), (56, 56, 255), (151, 157, 255), (31, 112, 255), (29, 178, 255), (49, 210, 207),
+             (10, 249, 72), (23, 204, 146), (134, 219, 61), (52, 147, 26), (187, 212, 0),
+             (168, 153, 44), (255, 194, 0), (147, 69, 52), (255, 115, 100),
+             (236, 24, 0), (255, 56, 132), (133, 0, 82), (255, 56, 203), (200, 149, 255), (199, 55, 255)] * 100
+
+root = os.path.dirname(__file__)
+coco_skeleton = [[1, 3], [1, 0], [2, 4], [2, 0], [0, 5], [0, 6], [5, 7], [7, 9], [6, 8],
+                 [8, 10], [5, 11], [6, 12], [11, 12], [11, 13], [13, 15], [12, 14], [14, 16]]
+mpii_skeleton = [[0, 1], [1, 2], [3, 4], [4, 5], [2, 6], [6, 3], [12, 11], [7, 12],
+                 [11, 10], [13, 14], [14, 15], [8, 9], [8, 7], [6, 7], [7, 13]]
 
 
 def get_font_type(size, font=""):
     """
     Windows字体路径      : /usr/share/fonts/楷体.ttf
     Linux(Ubuntu)字体路径：/usr/share/fonts/楷体.ttf
      >> fc-list             查看所有的字体
@@ -50,15 +59,15 @@
         font = ImageFont.truetype(font, size, encoding="utf-8")
     elif platform.system().lower() == 'windows':
         font = ImageFont.truetype("simhei.ttf", size, encoding="utf-8")  # simsun.ttc 宋体
     elif platform.system().lower() == 'linux':
         # font = ImageFont.truetype("uming.ttc", size, encoding="utf-8")
         font = ImageFont.truetype("NotoSansCJK-Regular.ttc", size, encoding="utf-8")
     else:
-        font = ImageFont.truetype(os.path.join(ROOT, "font_style/simhei.ttf"), size, encoding="utf-8")
+        font = ImageFont.truetype(os.path.join(root, "font_style/simhei.ttf"), size, encoding="utf-8")
     return font
 
 
 def create_image(shape, color=(255, 255, 255), dtype=np.uint8, use_rgb=False):
     """
     生成一张图片
     :param shape:
@@ -1188,75 +1197,82 @@
     :param drawType:
     :param top:
     :return:
     """
     thickness, fontScale = get_linesize(max(image.shape), thickness=thickness, fontScale=fontScale)
     if not name: drawType = "simple"
     if drawType == "chinese":
-        cv2.rectangle(image, (bbox[0], bbox[1]), (bbox[2], bbox[3]), color, thickness, 8, 0)
+        cv2.rectangle(image, (bbox[0], bbox[1]), (bbox[2], bbox[3]), color, thickness)
         cv2_putText(image, str(name), (bbox[0], bbox[1]), color=color, fontScale=fontScale, thickness=thickness)
     elif drawType == "simple":
         cv2.rectangle(image, (bbox[0], bbox[1]), (bbox[2], bbox[3]), color, thickness, 8, 0)
         cv2.putText(image, str(name), (bbox[0], bbox[1]), cv2.FONT_HERSHEY_SIMPLEX, fontScale, color, thickness)
     elif drawType == "custom":
         cv2.rectangle(image, (bbox[0], bbox[1]), (bbox[2], bbox[3]), color, thickness)
-        # draw score roi
-        # fontScale = 0.4
         text_size, baseline = cv2.getTextSize(str(name), cv2.FONT_HERSHEY_SIMPLEX, fontScale, thickness)
         if top:
             text_loc = (bbox[0], bbox[1] - text_size[1])
         else:
-            # text_loc = (bbox[0], bbox[3])
-            # text_loc = (bbox[2], bbox[3] - text_size[1])
-            text_loc = (bbox[2], bbox[1] + text_size[1])
-
+            # text_loc = (bbox[0], bbox[1])
+            text_loc = (bbox[0], bbox[3])
+            # text_loc = (bbox[2], bbox[1] + text_size[1])
         cv2.rectangle(image, (text_loc[0] - 2 // 2, text_loc[1] - 2 - baseline),
                       (text_loc[0] + text_size[0], text_loc[1] + text_size[1]), color, -1)
         # draw score value
         cv2.putText(image, str(name), (text_loc[0], text_loc[1] + baseline), cv2.FONT_HERSHEY_SIMPLEX, fontScale,
                     (255, 255, 255), thickness)
     return image
 
 
-def draw_landmark(image, landmarks_list, radius=1, thickness=2, color=(0, 0, 255), vis_id=False):
+def draw_landmark(image, landmarks, radius=2, fontScale=1.0, color=(0, 0, 255), vis_id=False):
+    """
+    :param image:
+    :param landmarks:
+    :param radius:
+    :param thickness:
+    :param fontScale:
+    :param color:
+    :param vis_id:
+    :return:
+    """
     image = copy.copy(image)
-    for landmarks in landmarks_list:
-        for i, landmark in enumerate(landmarks):
+    for lm in landmarks:
+        for i, landmark in enumerate(lm):
             # 要画的点的坐标
             point = (int(landmark[0]), int(landmark[1]))
-            cv2.circle(image, point, radius, color, thickness)
+            cv2.circle(image, point, radius, color, thickness=-1)
             if vis_id:
-                image = draw_points_text(image, [point], texts=[str(i)],
-                                         color=color, thickness=thickness, drawType="simple")
+                image = draw_points_text(image, [point], texts=[str(i)], color=color, thickness=radius,
+                                         fontScale=fontScale, drawType="simple")
     return image
 
 
-def show_landmark_boxes(title, image, landmarks_list, boxes):
+def show_landmark_boxes(title, image, landmarks, boxes):
     """
     显示landmark和boxex
     :param title:
     :param image:
-    :param landmarks_list: [[x1, y1], [x2, y2]]
+    :param landmarks: [[x1, y1], [x2, y2]]
     :param boxes:     [[ x1, y1, x2, y2],[ x1, y1, x2, y2]]
     :return:
     """
-    image = draw_landmark(image, landmarks_list)
+    image = draw_landmark(image, landmarks)
     image = show_image_boxes(title, image, boxes)
     return image
 
 
-def show_landmark(title, image, landmarks_list, vis_id=False, delay=0):
+def show_landmark(title, image, landmarks, vis_id=False, delay=0):
     """
     显示landmark和boxex
     :param title:
     :param image:
-    :param landmarks_list: [[x1, y1], [x2, y2]]
+    :param landmarks: [[x1, y1], [x2, y2]]
     :return:
     """
-    image = draw_landmark(image, landmarks_list, vis_id=vis_id)
+    image = draw_landmark(image, landmarks, vis_id=vis_id)
     cv_show_image(title, image, delay=delay)
     return image
 
 
 def draw_points_text(image, points, texts=None, color=(255, 0, 0), thickness=-1, fontScale=-1.0, drawType="simple"):
     """
     :param image:
@@ -1268,15 +1284,15 @@
     """
     thickness, fontScale = get_linesize(max(image.shape), thickness=thickness, fontScale=fontScale)
     if texts is None:
         texts = [""] * len(points)
     for point, text in zip(points, texts):
         if not check_point(point): continue
         point = (int(point[0]), int(point[1]))
-        cv2.circle(image, point, thickness * 2, color, -1)
+        cv2.circle(image, point, thickness * 3, color, -1)
         draw_text(image, point, text, color=color, fontScale=fontScale, thickness=thickness, drawType=drawType)
     return image
 
 
 def draw_texts(image, points, texts, color=(255, 0, 0), fontScale=-1.0, thickness=-1, drawType="simple"):
     for point, text in zip(points, texts):
         image = draw_text(image, point, text, color=color, fontScale=fontScale, thickness=thickness, drawType=drawType)
@@ -1340,15 +1356,15 @@
     :param size:
     :param color_color:
     :return:
     """
     pilimg = Image.fromarray(image)  # Image.fromarray()将数组类型转成图片格式，与np.array()相反
     draw = ImageDraw.Draw(pilimg)  # PIL图片上打印汉字
     # 参数1：字体文件路径，参数2：字体大小；Windows系统“simhei.ttf”默认存储在路径：
-    font = ImageFont.truetype(os.path.join(ROOT, "font_style/simhei.ttf"), size, encoding="utf-8")
+    font = ImageFont.truetype(os.path.join(root, "font_style/simhei.ttf"), size, encoding="utf-8")
     draw.text(point, text, color_color, font)
     image = cv2.cvtColor(np.array(pilimg), cv2.COLOR_RGB2BGR)  # 将图片转成cv2.imshow()可以显示的数组格式
     return image
 
 
 def cv2_putText(img, text, point, fontFace=None, fontScale=0.8, color=(255, 0, 0), thickness=None):
     # cv2.putText(img, str(text), point, fontFace, fontScale, color=color, thickness=thickness)
@@ -1357,55 +1373,44 @@
     size = int(fontScale * 10 * thickness)
     point = (point[0], point[1] - int(size * 1.3))
     font = get_font_type(size=size)
     draw.text(point, text, color, font)
     img[:] = np.asarray(pilimg)
 
 
-def draw_key_point_in_image(image,
-                            key_points,
-                            pointline=[],
-                            vis_id=False,
-                            circle_color=(0, 255, 0),
-                            line_color=(0, 0, 255),
-                            thickness=2):
+def draw_key_point_in_image(image, key_points, pointline=[], boxes=[], vis_id=False, thickness=2):
     """
     :param key_points: list(ndarray(19,2)) or ndarray(n_person,19,2)
     :param image:
     :param pointline: `auto`->pointline = circle_line(len(points), iscircle=True)
     :return:
     """
-    image = copy.deepcopy(image)
-    for person_id, points in enumerate(key_points):
-        if points is None:
-            continue
-        if vis_id:
-            text = None
-        else:
-            text = [""] * len(points)
-        image = draw_image_points_lines(image, points, pointline,
-                                        circle_color=circle_color,
-                                        line_color=line_color,
-                                        texts=text,
-                                        thickness=thickness)
+    nums = max(len(key_points), len(boxes))
+    for p in range(nums):
+        color = color_map[p + 1]
+        if len(key_points) > 0:
+            points = key_points[p]
+            if points is None or len(points) == 0: continue
+            text = list(range(len(points))) if vis_id else [""] * len(points)
+            image = draw_image_points_lines(image, points, pointline, circle_color=color, line_color=color,
+                                            texts=text, thickness=thickness)
+        if len(boxes) > 0:
+            image = draw_image_boxes(image, boxes=[boxes[p]], color=color, thickness=thickness)
     return image
 
 
 def draw_key_point_arrowed_in_image(image, key_points, pointline=[], color=None):
     """
     :param key_points: list(ndarray(19,2)) or ndarray(n_person,19,2)
     :param image:
     :param pointline:[[start-->end]]
     :return:
     """
-    image = copy.deepcopy(image)
-    person_nums = len(key_points)
     for person_id, points in enumerate(key_points):
-        if points is None:
-            continue
+        if points is None or len(points) == 0: continue
         image = draw_image_points_arrowed_lines(image, points, pointline)
     return image
 
 
 def draw_image_points_lines(image,
                             points,
                             pointline=[],
@@ -1658,54 +1663,67 @@
 
 
 def file2base64(file):
     image_base64 = base64.b64encode(open(file, 'rb').read()).decode()
     return image_base64
 
 
-def bgr_image2image_base64(bgr_image):
+def image2base64(image: np.ndarray, prefix="", use_rgb=False) -> str:
     """
-    image = cv2.imencode('.jpeg', bgr_image)[1]
-    image_base64 = base64.b64encode(image).decode()
-    image_base64 = str(base64.b64encode(image), encoding='utf-8')
-    """
-    from io import BytesIO
-    if len(bgr_image.shape) == 3:
-        bgr_image = cv2.cvtColor(bgr_image, cv2.COLOR_BGR2RGB)
-    image = Image.fromarray(bgr_image)
-    buff = BytesIO()
-    image.save(buff, format="PNG")
-    image_base64 = base64.b64encode(buff.getvalue()).decode("utf-8")
-    return image_base64
+    将图像编码为二进制字符串
+    ``` python
+        from io import BytesIO
+        bgr_img = Image.fromarray(image)
+        buff = BytesIO()
+        mg.save(buff, format="PNG")
+        image_base64 = base64.b64encode(buff.getvalue()).decode("utf-8")
+        image_base64 = str(base64.b64encode(image), encoding='utf-8')
+    ```
+    :param image: 图像
+    :param prefix: base64字符串前缀,用于表识字符串的类型
+    :param use_rgb: True:输入image是RGB的图像, False:输入image是BGR格式的图像
+    :return: 返回图像
+    """
+    # image = cv2.imencode('.jpeg', bgr_image)[1]
+    # image_base64 = base64.b64encode(image).decode()
+    # image_base64 = str(base64.b64encode(image), encoding='utf-8')
+    img = image.copy()
+    if len(img.shape) == 3 and use_rgb:
+        img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)
+    ext = prefix.split("/")
+    ext = "." + ext[1] if len(ext) == 2 else ".png"
+    img = cv2.imencode(ext, img)[1]
+    bs64 = prefix + base64.b64encode(img).decode()
+    return bs64
 
 
-def image_base642rgb_image(image_base64, use_rgb=False) -> np.ndarray:
+def base642image(image_bs64, use_rgb=False) -> np.ndarray:
     """
     將二进制字符串图像image_base64解码为正常形式
-    :param image_base64: 二进制字符串图像
+    :param image_bs64: 二进制字符串图像
     :param use_rgb: True:返回RGB的图像, False:返回BGR格式的图像
     :return: 返回图像矩阵
     """
-    image_base64 = bytes(image_base64, 'utf-8')
-    image = base64.b64decode(image_base64)
+    image_bs64 = bytes(image_bs64, 'utf-8')
+    image = base64.b64decode(image_bs64)
     image = np.fromstring(image, np.uint8)
     image = cv2.imdecode(image, cv2.IMREAD_COLOR)
     if use_rgb:
         image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
     return image
 
 
-def read_image_base64(image_path, size=None):
+def read_image_base64(image_file, size=None):
     if not size:
-        with open(image_path, 'rb') as f_in:
+        with open(image_file, 'rb') as f_in:
             image_base64 = base64.b64encode(f_in.read())
             image_base64 = str(image_base64, encoding='utf-8')
     else:
-        bgr_image = read_image(image_path, size=size, use_rgb=False)
-        image_base64 = bgr_image2image_base64(bgr_image)
+        bgr_image = read_image(image_file, size=size, use_rgb=False)
+        image_base64 = image2base64(bgr_image)
     return image_base64
 
 
 def bin2image(bin_data, size, norm=False, use_rgb=True):
     data = np.asarray(bytearray(bin_data), dtype="uint8")
     image = cv2.imdecode(data, cv2.IMREAD_COLOR)
     if use_rgb:
@@ -2147,14 +2165,32 @@
     if inv:
         ret, mask = cv2.threshold(image, 0, 255, cv2.THRESH_BINARY_INV | cv2.THRESH_OTSU)
     else:
         ret, mask = cv2.threshold(image, 0, 255, cv2.THRESH_BINARY | cv2.THRESH_OTSU)
     return mask
 
 
+def get_mask_erode_dilate(mask, ksize, binarize=False):
+    """
+    获得膨胀和腐蚀的mask
+    :param mask:
+    :param ksize:
+    :param binarize:
+    :return:
+    """
+    if binarize: mask = get_image_mask(mask, inv=False)
+    if ksize > 0:
+        k = np.ones((5, 5), np.uint8)  # 设置kenenel大小
+        mask = cv2.erode(mask, k)  # 腐蚀去除白点
+    if ksize < 0:
+        k = np.ones((5, 5), np.uint8)  # 设置kenenel大小
+        mask = cv2.dilate(mask, k)  # 膨胀增大白点
+    return mask
+
+
 def get_scale_image(image, scale=0.85, offset=(0, 0), color=(0, 0, 0), interpolation=cv2.INTER_NEAREST):
     """
     同比居中缩小image，以便居中显示
     :param image: mask
     :param scale: 缩放比例
     :param offset: 偏移量(x,y)
     :return: 返回缩放的轮廓Mask
```

### Comparing `pybaseutils-0.8.0/pybaseutils/json_utils.py` & `pybaseutils-0.8.1/pybaseutils/json_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/log.py` & `pybaseutils-0.8.1/pybaseutils/log.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/logger.py` & `pybaseutils-0.8.1/pybaseutils/logger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/maker/convert_labelme2voc.py` & `pybaseutils-0.8.1/pybaseutils/maker/convert_labelme2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/maker/convert_voc2voc.py` & `pybaseutils-0.8.1/pybaseutils/maker/convert_voc2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/maker/convert_voc2yolo.py` & `pybaseutils-0.8.1/pybaseutils/maker/convert_voc2yolo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/maker/convert_yolo2voc.py` & `pybaseutils-0.8.1/pybaseutils/maker/convert_yolo2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/maker/maker_labelme.py` & `pybaseutils-0.8.1/pybaseutils/maker/maker_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/maker/maker_voc.py` & `pybaseutils-0.8.1/pybaseutils/maker/maker_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/metrics/accuracy.py` & `pybaseutils-0.8.1/pybaseutils/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/metrics/average_meter.py` & `pybaseutils-0.8.1/pybaseutils/metrics/average_meter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/metrics/class_report.py` & `pybaseutils-0.8.1/pybaseutils/metrics/class_report.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/metrics/plot_pr.py` & `pybaseutils-0.8.1/pybaseutils/metrics/plot_pr.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/metrics/plot_roc.py` & `pybaseutils-0.8.1/pybaseutils/metrics/plot_roc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/numpy_utils.py` & `pybaseutils-0.8.1/pybaseutils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/pandas_utils.py` & `pybaseutils-0.8.1/pybaseutils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/plot_utils.py` & `pybaseutils-0.8.1/pybaseutils/plot_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         font = FontProperties(fname="simhei.ttf", size=size)
     elif platform.system().lower() == 'linux':
         # font = ImageFont.truetype("uming.ttc", size, encoding="utf-8")
         # font = ImageFont.truetype("NotoSansCJK-Regular.ttc", size, encoding="utf-8")
         # font = FontProperties(fname="NotoSansCJK-Regular.ttc", size=size)
         font = FontProperties(fname=os.path.join(ROOT, "font_style/simhei.ttf"), size=size)
     else:
-        # font = ImageFont.truetype(os.path.join(ROOT, "font_style/simhei.ttf"), size, encoding="utf-8")
+        # font = ImageFont.truetype(os.path.join(root, "font_style/simhei.ttf"), size, encoding="utf-8")
         font = FontProperties(fname=os.path.join(ROOT, "font_style/simhei.ttf"), size=size)
     return font
 
 
 def count_bin(x, bin_ranges, num_bin=10, norm=True):
     """
     统计x在范围bin_ranges出现的频率
```

### Comparing `pybaseutils-0.8.0/pybaseutils/pycpp/demo.py` & `pybaseutils-0.8.1/pybaseutils/pycpp/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/pycpp/main.py` & `pybaseutils-0.8.1/pybaseutils/pycpp/main.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/setup_config.py` & `pybaseutils-0.8.1/pybaseutils/setup_config.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/thread_utils.py` & `pybaseutils-0.8.1/pybaseutils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/time_utils.py` & `pybaseutils-0.8.1/pybaseutils/time_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/tracemalloc_utils.py` & `pybaseutils-0.8.1/pybaseutils/tracemalloc_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/tracemalloc_utils2.py` & `pybaseutils-0.8.1/pybaseutils/tracemalloc_utils2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/transforms/affine_transform.py` & `pybaseutils-0.8.1/pybaseutils/transforms/affine_transform.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils/word_utils.py` & `pybaseutils-0.8.1/pybaseutils/word_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,14 +127,15 @@
             out_packers[i].update(packers[p][i])
     return out_packers
 
 
 def word_packer(unpacker: Dict, keys):
     packer = []
     for key in keys:
+        if key not in unpacker: continue
         if not packer:
             packer = [{key: v} for v in unpacker[key]]
         else:
             for i in range(len(unpacker[key])):
                 packer[i][key] = unpacker[key][i]
     return packer
```

### Comparing `pybaseutils-0.8.0/pybaseutils/worker.py` & `pybaseutils-0.8.1/pybaseutils/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
                 self.task_list.append(task)
             except Exception as e:
                 pass
             finally:
                 index = []
                 for i, task in enumerate(self.task_list):
                     if task.done():
-                        self.output.put(task.result(), block=True, timeout=None)
+                        self.output.put(task.r(), block=True, timeout=None)
                     else:
                         index.append(i)
                 self.task_list = [self.task_list[i] for i in index]
 
     def target(self):
         return self._target_v2()
         # return self._target_v1()
```

### Comparing `pybaseutils-0.8.0/pybaseutils/yaml_utils.py` & `pybaseutils-0.8.1/pybaseutils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/pybaseutils.egg-info/PKG-INFO` & `pybaseutils-0.8.1/pybaseutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 0.8.0
+Version: 0.8.1
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENCE
```

### Comparing `pybaseutils-0.8.0/pybaseutils.egg-info/SOURCES.txt` & `pybaseutils-0.8.1/pybaseutils.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 pybaseutils/worker.py
 pybaseutils/yaml_utils.py
 pybaseutils.egg-info/PKG-INFO
 pybaseutils.egg-info/SOURCES.txt
 pybaseutils.egg-info/dependency_links.txt
 pybaseutils.egg-info/not-zip-safe
 pybaseutils.egg-info/top_level.txt
+pybaseutils/base_audio/__init__.py
+pybaseutils/base_audio/audio_utils.py
 pybaseutils/cluster/__init__.py
 pybaseutils/cluster/kmean.py
 pybaseutils/cluster/maxmin_distance.py
 pybaseutils/cluster/similarity.py
 pybaseutils/cvutils/__init__.py
 pybaseutils/cvutils/corner_utils.py
 pybaseutils/cvutils/mouse_utils.py
@@ -63,42 +65,52 @@
 pybaseutils/pycpp/main.py
 pybaseutils/transforms/__init__.py
 pybaseutils/transforms/affine_transform.py
 test_py/__init__.py
 test_py/class_names.py
 test_py/demo1.py
 test_py/demo2.py
+test_py/demo_async_await1.py
+test_py/demo_async_await2.py
 test_py/demo_copy_files.py
 test_py/demo_copy_files_for_voc.py
-test_py/demo_correction_v1.py
-test_py/demo_correction_v2.py
-test_py/demo_correction_v3.py
+test_py/demo_ffmpy.py
 test_py/demo_for_trt.py
 test_py/demo_get_file_list.py
 test_py/demo_gif.py
+test_py/demo_gif_video.py
 test_py/demo_metrics.py
 test_py/demo_mouse.py
 test_py/demo_pandas.py
 test_py/demo_plot.py
 test_py/demo_standard_image .py
 test_py/demo_standard_video .py
 test_py/demo_taichi.py
 test_py/demo_video.py
 test_py/demo_voc_crop.py
 test_py/demo_voc_vis.py
 test_py/demo_word_similar.py
 test_py/demo_worker1.py
 test_py/demo_worker2.py
+test_py/kafka_worker.py
 test_py/men_tracemalloc.py
 test_py/performance.py
 test_py/converter/AffectNet.py
 test_py/converter/AsianMovie.py
 test_py/converter/BITVehicle2voc.py
 test_py/converter/BSTLD2voc.py
 test_py/converter/CCPD.py
 test_py/converter/CCPD2voc.py
 test_py/converter/TT100K.py
 test_py/converter/__init__.py
-test_py/converter/detect_face_person.py
 test_py/converter/insects_for_aichallenger.py
 test_py/converter/tt100k_utils.py
-test_py/converter/ua_detrac2voc.py
+test_py/converter/ua_detrac2voc.py
+test_py/detector/__init__.py
+test_py/detector/detect_face_person.py
+test_py/flask_demo/__init__.py
+test_py/flask_demo/func.py
+test_py/flask_demo/server.py
+test_py/image_correction/__init__.py
+test_py/image_correction/demo_correction_v1.py
+test_py/image_correction/demo_correction_v2.py
+test_py/image_correction/demo_correction_v3.py
```

### Comparing `pybaseutils-0.8.0/README.md` & `pybaseutils-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/setup.py` & `pybaseutils-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/class_names.py` & `pybaseutils-0.8.1/test_py/class_names.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/converter/AffectNet.py` & `pybaseutils-0.8.1/test_py/converter/AffectNet.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/converter/AsianMovie.py` & `pybaseutils-0.8.1/test_py/converter/AsianMovie.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/converter/BITVehicle2voc.py` & `pybaseutils-0.8.1/test_py/converter/BITVehicle2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/converter/BSTLD2voc.py` & `pybaseutils-0.8.1/test_py/converter/BSTLD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/converter/CCPD.py` & `pybaseutils-0.8.1/test_py/converter/CCPD.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/converter/CCPD2voc.py` & `pybaseutils-0.8.1/test_py/converter/CCPD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/converter/detect_face_person.py` & `pybaseutils-0.8.1/test_py/detector/detect_face_person.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,39 +7,28 @@
 import random
 import cv2
 import numpy as np
 from tqdm import tqdm
 from pybaseutils import file_utils, image_utils, pandas_utils
 from libs.detector.detector import Detector
 
-class_name = {0: "neutral",
-              1: "happy",
-              2: "excited",
-              3: "surprised",
-              4: "sad",
-              5: "disgust",
-              6: "fear",
-              7: "confused",
-              8: "tired",
-              9: "angry",
-              10: "serious"
-              }
-
 
 class ParseDataset(object):
-    def __init__(self, prb_thresh=0.9, iou_thresh=0.3):
+    def __init__(self, prb_thresh=0.5, iou_thresh=0.3):
         """
         :param file:
         :param image_dir:
         :param is_detect:
         :param image_sub:
         :param shuffle:
         """
         # self.detector = Detector(prb_thresh=prb_thresh, iou_thresh=iou_thresh, detect_type="mtcnn")
-        self.detector = Detector(prb_thresh=prb_thresh, iou_thresh=iou_thresh, detect_type="dfsd")
+        # self.detector = Detector(prb_thresh=prb_thresh, iou_thresh=iou_thresh, detect_type="dfsd")
+        self.detector = Detector(prb_thresh=prb_thresh, iou_thresh=iou_thresh, detect_type="yolov5_person")
+        self.names = self.detector.class_names
 
     def get_item_list_class(self, image_dir, shuffle=True):
         """
         数据格式：
         image_dir
            ├── A
            │ ├── 0001.jpg
@@ -56,16 +45,16 @@
         item_list = [[path, os.path.dirname(path)] for path in images]
         if shuffle:
             random.seed(200)
             random.shuffle(item_list)
         print("have dataset:{}".format(len(item_list)))
         return item_list
 
-    def parse_data(self, image_dir, out_dir="", flag="20220200", square=True,
-                   extend=[2.0, 2.0], max_num=None, shuffle=True, vis=True):
+    def parse_data(self, image_dir, out_dir="", scale=[], square=False, padding=False, flag="20220200", max_num=None,
+                   shuffle=True, vis=True):
         """
         数据格式：
         image_dir
            ├── A
            │ ├── 0001.jpg
            │ └── 0002.jpg
            └── B
@@ -77,59 +66,103 @@
         :param max_num:
         :param shuffle:
         :param vis:
         :return:
         """
         item_list = self.get_item_list_class(image_dir=image_dir, shuffle=shuffle)
         nums_sample = len(item_list)
-        if max_num:
-            nums_sample = min(max_num, nums_sample)
-        dst_item_list = []
+        if max_num: nums_sample = min(max_num, nums_sample)
         for i in tqdm(range(nums_sample)):
             image_file, label = item_list[i]
             image_path = os.path.join(image_dir, image_file)
             if not os.path.exists(image_path):
                 print("no path:{}".format(image_path))
                 continue
             image = image_utils.read_image(image_path)
             if image is None:
                 print("empty file:{}".format(image_path))
                 continue
             h, w = image.shape[:2]
             rgb = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
-            dets, _ = self.detector.detect(rgb, vis=False)
-            if len(dets) == 0: continue
-            boxes = dets[:, 0:4]
-            if square: boxes = image_utils.get_square_bboxes(boxes, use_max=True)
-            if extend: boxes = image_utils.extend_xyxy(boxes, scale=extend)
-            xmin, ymin, xmax, ymax = np.asarray(boxes, dtype=np.int32)[0]
-            sub, name = image_file.split("/")
-            name = "{}_{:0=6d}.jpg".format(flag, i)
-            # item = [os.path.join(label, name), xmin, ymin, xmax, ymax]
-            item = [image_file, label, xmin, ymin, xmax, ymax]
-            box = [xmin, ymin, xmax, ymax]
-            dst_item_list.append(item)
+            bbox_score, labels = self.detector.detect(rgb, vis=False)
+            if len(bbox_score) == 0: continue
+            dets = np.hstack((bbox_score, labels.reshape(-1, 1)))
+            image_id = "{}_{:0=6d}".format(flag, i) if flag else os.path.basename(image_file).split(".")[0]
+            self.save_crops(image, dets, image_id, scale=scale, square=square, padding=padding, out_dir=out_dir,
+                            vis=vis)
+
+    def faceboxes2bodyup(self, xyxy, shift=(0, 0.5), scale=(1.0, 1.0)):
+        """通过人脸框获得上半身"""
+        if not isinstance(xyxy, np.ndarray): xyxy = np.asarray(xyxy)
+        cxcywh = image_utils.xyxy2cxcywh(xyxy)
+        dcxcywh = cxcywh.copy()
+        dcxcywh[:, 0] = dcxcywh[:, 0] + dcxcywh[:, 2] * shift[0]
+        dcxcywh[:, 1] = dcxcywh[:, 1] + dcxcywh[:, 3] * shift[1]
+        dxyxy = image_utils.cxcywh2xyxy(dcxcywh)
+        dxyxy = image_utils.extend_xyxy(dxyxy, scale=scale)
+        return dxyxy
+
+    def get_boxes_up(self, xyxy, scale=(), cut=0.3):
+        """获得boxes上半部分"""
+        dxyxy = []
+        for i in range(len(xyxy)):
+            xmin, ymin, xmax, ymax = xyxy[i]
+            w, h = (xmax - xmin), (ymax - ymin)
+            ymax = max(ymin + h * cut, ymin + w)
+            dxyxy.append([xmin, ymin, xmax, ymax])
+        dxyxy = np.asarray(dxyxy)
+        if scale: dxyxy = image_utils.extend_xyxy(dxyxy, scale=scale)
+        return dxyxy
+
+    def save_crops(self, image, dets, image_id, scale=[], square=False, padding=False, out_dir=None, vis=False):
+        boxes = dets[:, 0:4]
+        conf = dets[:, 4:5]
+        labels = dets[:, 5]
+        if square:
+            boxes = image_utils.get_square_bboxes(boxes, use_max=True, baseline=-1)
+        if scale:
+            # boxes = image_utils.extend_xyxy(boxes, scale=scale)
+            # boxes = self.faceboxes2bodyup(boxes, scale=scale)
+            boxes = self.get_boxes_up(boxes, scale=scale)
+        if padding:
+            crops = image_utils.get_bboxes_crop_padding(image, boxes)
+        else:
+            crops = image_utils.get_bboxes_crop(image, boxes)
+        if vis:
+            m = image_utils.draw_image_detection_bboxes(image.copy(), boxes, conf, labels, class_name=self.names)
+            image_utils.cv_show_image("image", m, use_rgb=False, delay=10)
+        for i, img in enumerate(crops):
+            name = self.names[int(labels[i])] if self.names else labels[i]
             if out_dir:
-                # orig_file = file_utils.create_dir(os.path.join(out_dir, "origin"), label, name)
-                # file_utils.copy_file(image_path, orig_file)
-                crop_file = file_utils.create_dir(os.path.join(out_dir, "crops"), label, name)
-                crop = image_utils.get_bbox_crop(image, box)
-                cv2.imwrite(crop_file, crop)
-            if vis:
-                image = image_utils.draw_image_boxes(image, [box])
-                image = image_utils.draw_texts(image, [[xmin + 5, ymin + 10]], texts=[label])
-                image_utils.cv_show_image("image", image)
-        if not out_dir: out_dir = image_dir
-        filename = file_utils.create_dir(out_dir, None, "label.txt")
-        file_utils.write_data(filename, dst_item_list, split=",")
-        return dst_item_list
-
-
-def main():
-    image_dir = "/home/dm/nasdata/dataset/csdn/smoking/smokingVSnotsmoking/training_data"
-    out_dir = "/home/dm/nasdata/dataset/csdn/smoking/dataset1"
+                # img_file = file_utils.create_dir(out_dir, name, "{}_{:0=3d}.jpg".format(image_id, i))
+                img_file = file_utils.create_dir(out_dir, None, "{}_{:0=3d}.jpg".format(image_id, i))
+                cv2.imwrite(img_file, img)
+            if vis: image_utils.cv_show_image("crop", img, use_rgb=False, delay=0)
+
+
+def demo_for_image_dir(image_dir="", out_dir=""):
+    # image_dir = "/home/dm/nasdata/release/tmp/PyTorch-Classification-Trainer/data/test_image"
+    # out_dir = image_dir + "-crops"
     dataset = ParseDataset()
-    data_info = dataset.parse_data(image_dir=image_dir, out_dir=out_dir, flag="202200000", shuffle=False, vis=False)
+    scale = [1.1, 1.1]
+    square = False
+    padding = False
+    flag = file_utils.get_time("s").replace("2023", "2018")
+    # flag = ""
+    data_info = dataset.parse_data(image_dir=image_dir, out_dir=out_dir, scale=scale, square=square,
+                                   padding=padding, flag=flag, shuffle=False, vis=False)
+
+
+
+def demo_for_image_root():
+    root = "/home/dm/nasdata/dataset/tmp/smoking-calling/train"
+    out_root = "/home/dm/nasdata/dataset/tmp/smoking/smoking-person/dataset-v4/train"
+    subs = file_utils.get_sub_paths(root)
+    for sub in subs:
+        image_dir = os.path.join(root, sub)
+        out_dir = os.path.join(out_root, sub)
+        demo_for_image_dir(image_dir, out_dir)
 
 
 if __name__ == '__main__':
-    main()
+    demo_for_image_root()
+    # demo_for_image_dir()
```

### Comparing `pybaseutils-0.8.0/test_py/converter/insects_for_aichallenger.py` & `pybaseutils-0.8.1/test_py/converter/insects_for_aichallenger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/converter/TT100K.py` & `pybaseutils-0.8.1/test_py/converter/TT100K.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/converter/tt100k_utils.py` & `pybaseutils-0.8.1/test_py/converter/tt100k_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/converter/ua_detrac2voc.py` & `pybaseutils-0.8.1/test_py/converter/ua_detrac2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/demo2.py` & `pybaseutils-0.8.1/test_py/demo_standard_image .py`

 * *Files 26% similar despite different names*

```diff
@@ -3,38 +3,34 @@
     @Author : PKing
     @E-mail : 390737991@qq.com
     @Date   : 2022-12-31 11:37:30
     @Brief  :
 """
 import os
 import cv2
-import time
-from tqdm import tqdm
-from multiprocessing import Pool
 import numpy as np
-from pybaseutils import file_utils, image_utils, base64_utils, time_utils
+from pybaseutils import file_utils, image_utils
 
 
-def image_dir_mask(image_dir, info_file):
-    names = file_utils.read_json_data(info_file)
-    sub_list = file_utils.get_sub_paths(image_dir)
-    others = []
-    class_dict = names.copy()
-    for sub in sub_list:
-        old = sub.strip().lower()
-        if old in names:
-            new = names[old]["name"]
-            old = os.path.join(image_dir, old)
-            new = os.path.join(image_dir, new)
-            if os.path.exists(old):
-                os.rename(old, new)
-        else:
-            # class_dict[old] = {"name": ""}
-            others.append(old)
-    print(others)
-
+def image_clip_demo(image_dir, out_dir):
+    """
+    显示图片大小
+    pip install pybaseutils==0.7.3
+    :param image_dir: 输入图片文件夹
+    :param out_dir:保存图片文件夹
+    :return:
+    """
+    image_list = file_utils.get_images_list(image_dir)
+    for image_file in image_list:
+        image = cv2.imread(image_file)
+        # 限制图像最大分辨率,不超过1920
+        out_image = image_utils.resize_image_clip(image, clip_max=1920)
+        print(image.shape, out_image.shape)
+        if out_dir:
+            out_file = file_utils.create_dir(out_dir, None, os.path.basename(image_file))
+            cv2.imwrite(out_file, out_image)
 
 
 if __name__ == "__main__":
-    image_dir = "/home/dm/nasdata/dataset/tmp/Medicine/dataset/train"
-    info_file = "/home/dm/nasdata/dataset/tmp/Medicine/dataset/file.json"
-    image_dir_mask(image_dir, info_file)
+    image_dir = "/home/dm/nasdata/dataset-dmai/handwriting/word-det/word-v6/zip/test1"
+    out_dir = "/home/dm/nasdata/dataset-dmai/handwriting/word-det/word-v6/zip/test"
+    image_clip_demo(image_dir, out_dir)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pybaseutils-0.8.0/test_py/demo_copy_files.py` & `pybaseutils-0.8.1/test_py/demo_copy_files.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/demo_copy_files_for_voc.py` & `pybaseutils-0.8.1/test_py/demo_copy_files_for_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/demo_correction_v1.py` & `pybaseutils-0.8.1/test_py/image_correction/demo_correction_v1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/demo_correction_v2.py` & `pybaseutils-0.8.1/test_py/image_correction/demo_correction_v2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/demo_correction_v3.py` & `pybaseutils-0.8.1/test_py/image_correction/demo_correction_v3.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/demo_get_file_list.py` & `pybaseutils-0.8.1/test_py/demo_get_file_list.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/demo_gif.py` & `pybaseutils-0.8.1/test_py/demo_gif.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/demo_metrics.py` & `pybaseutils-0.8.1/test_py/demo_metrics.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/demo_mouse.py` & `pybaseutils-0.8.1/test_py/demo_mouse.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/demo_pandas.py` & `pybaseutils-0.8.1/test_py/demo_pandas.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/demo_plot.py` & `pybaseutils-0.8.1/test_py/demo_plot.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/demo_standard_video .py` & `pybaseutils-0.8.1/test_py/demo_standard_video .py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 import os
 import cv2
 import numpy as np
 from pybaseutils import file_utils, image_utils
 from pybaseutils.cvutils import video_utils
 
 
-def video_conerter(root, out):
+def video_converter(root, out):
     files = file_utils.get_files_list(root, postfix=["*.avi"])
     for video_file in files:
         save_video = file_utils.create_dir(out, None, os.path.basename(video_file))
         save_video = save_video.replace(".avi", ".mp4")
         video_utils.video2video(video_file, save_video, interval=1, vis=False)
 
 
 if __name__ == "__main__":
     root = "/media/dm/新加卷/SDK/project/Camera-Calibration-Reconstruct-Cpp/data/lenacv-video"
     out = "/media/dm/新加卷/SDK/project/Camera-Calibration-Reconstruct-Cpp/data/lenacv-video1"
-    video_conerter(root, out)
+    video_converter(root, out)
```

### Comparing `pybaseutils-0.8.0/test_py/demo_taichi.py` & `pybaseutils-0.8.1/test_py/demo_taichi.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/demo_video.py` & `pybaseutils-0.8.1/test_py/demo_gif_video.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,36 +20,35 @@
     h, w = frame.shape[:2]
     frame = image_utils.resize_image(frame, size=(None, 580))  # android-video
     return frame
 
 
 def resize_fun(frame):
     h, w = frame.shape[:2]
-    frame = image_utils.resize_image(frame, size=(360, None))
+    frame = image_utils.resize_image(frame, size=(416, None))
     # frame = image_utils.resize_image(frame, size=(None, 640))  # android-video
     return frame
 
 
 def android_gif():
     # video_file = "/media/dm/新加卷/SDK/CSDN/双目测距/demo/image-nouse-wls.mp4"
-    video_file = "/media/dm/新加卷/SDK/CSDN/双目测距/demo/image-use-wls.mp4"
-    video_utils.video2gif(video_file, interval=6, func=resize_android, fps=3, use_pil=False, vis=True)
+    video_file = "/home/dm/nasdata/dataset/tmp/Face-Recognition/demo/android-demo/android-人脸识别视频demo2.mp4"
+    video_utils.video2gif(video_file, interval=12, func=resize_android, fps=4, use_pil=False, vis=True)
 
 
 def python_gif():
-    video_file = "/home/dm/nasdata/dataset/csdn/emotion/demo/emotion-python.avi"
-    video_utils.video2gif(video_file, interval=5, func=resize_fun, fps=6, use_pil=False, vis=True)
+    video_file = "/media/dm/新加卷/SDK/face-recognition/Face-Recognition/Face-Recognition-Python/docs/result2.avi"
+    video_utils.video2gif(video_file, interval=7, func=resize_fun, fps=6, use_pil=False, vis=True)
 
 
-def other_gif(video_file):
-    video_utils.video2frames(video_file, interval=2, func=None, vis=True)
-    # video_utils.video2gif(video_file, interval=3, func=resize_fun, fps=7, use_pil=False, vis=True)
-    # video_utils.video2gif(video_file, interval=4, func=None, fps=5, use_pil=True, vis=True)
-    # video2video(video_file, dst_file, vis=True)
-    # image_dir = "/home/dm/视频/Kazam_screencast_00000"
-    # video_utils.frames2video(image_dir,interval=1, fps=1)
-    # image_utils.image_dir2gif(image_dir, size=(None, 600), interval=6, fps=2, loop=0, padding=False, use_pil=False)
+def image_gif():
+    image_dir = "/home/dm/nasdata/dataset/tmp/Face-Recognition/demo/Cpp-demo/cpp-fr-demo"
+    gif_file = image_dir + ".gif"
+    frames = file_utils.get_images_list(image_dir)
+    image_utils.image_file2gif(frames, size=(416, 416), padding=True, interval=1, gif_file=gif_file, fps=1,
+                               use_pil=False)
 
 
 if __name__ == "__main__":
+    # image_gif()
     android_gif()
     # python_gif()
```

### Comparing `pybaseutils-0.8.0/test_py/demo_voc_crop.py` & `pybaseutils-0.8.1/test_py/demo_voc_crop.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/demo_voc_vis.py` & `pybaseutils-0.8.1/test_py/demo_voc_vis.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/demo_word_similar.py` & `pybaseutils-0.8.1/test_py/demo_word_similar.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/demo_worker1.py` & `pybaseutils-0.8.1/test_py/demo_worker1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/demo_worker2.py` & `pybaseutils-0.8.1/test_py/demo_worker2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/men_tracemalloc.py` & `pybaseutils-0.8.1/test_py/men_tracemalloc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-0.8.0/test_py/performance.py` & `pybaseutils-0.8.1/test_py/performance.py`

 * *Files identical despite different names*

