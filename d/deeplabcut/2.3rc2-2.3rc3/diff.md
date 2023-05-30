# Comparing `tmp/deeplabcut-2.3rc2.tar.gz` & `tmp/deeplabcut-2.3rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deeplabcut-2.3rc2.tar", last modified: Fri Nov  4 17:39:23 2022, max compression
+gzip compressed data, was "deeplabcut-2.3rc3.tar", last modified: Wed Nov 23 10:44:34 2022, max compression
```

## Comparing `deeplabcut-2.3rc2.tar` & `deeplabcut-2.3rc3.tar`

### file list

```diff
@@ -1,219 +1,220 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/
--rw-r--r--   0 alex       (501) staff       (20)     4016 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/AUTHORS
--rw-r--r--   0 alex       (501) staff       (20)     7652 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)    26272 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)    25639 2022-11-04 17:28:45.000000 deeplabcut-2.3rc2/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/
--rw-r--r--   0 alex       (501) staff       (20)     3359 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      715 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/__main__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/benchmark/
--rw-r--r--   0 alex       (501) staff       (20)     3965 2022-11-04 17:28:45.000000 deeplabcut-2.3rc2/deeplabcut/benchmark/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      345 2022-11-04 17:28:45.000000 deeplabcut-2.3rc2/deeplabcut/benchmark/__main__.py
--rw-r--r--   0 alex       (501) staff       (20)     7461 2022-11-04 17:28:45.000000 deeplabcut-2.3rc2/deeplabcut/benchmark/base.py
--rw-r--r--   0 alex       (501) staff       (20)     8574 2022-11-04 17:28:45.000000 deeplabcut-2.3rc2/deeplabcut/benchmark/benchmarks.py
--rw-r--r--   0 alex       (501) staff       (20)     1262 2022-11-04 17:28:45.000000 deeplabcut-2.3rc2/deeplabcut/benchmark/cli.py
--rw-r--r--   0 alex       (501) staff       (20)     8248 2022-11-04 17:28:45.000000 deeplabcut-2.3rc2/deeplabcut/benchmark/metrics.py
--rw-r--r--   0 alex       (501) staff       (20)     2194 2022-11-04 17:28:45.000000 deeplabcut-2.3rc2/deeplabcut/benchmark/utils.py
--rw-r--r--   0 alex       (501) staff       (20)    23955 2022-10-04 20:28:48.000000 deeplabcut-2.3rc2/deeplabcut/cli.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/create_project/
--rw-r--r--   0 alex       (501) staff       (20)      367 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/deeplabcut/create_project/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     5314 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/create_project/add.py
--rw-r--r--   0 alex       (501) staff       (20)     2061 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/create_project/demo_data.py
--rw-r--r--   0 alex       (501) staff       (20)    11378 2022-08-22 16:31:54.000000 deeplabcut-2.3rc2/deeplabcut/create_project/modelzoo.py
--rw-r--r--   0 alex       (501) staff       (20)    10930 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/create_project/new.py
--rw-r--r--   0 alex       (501) staff       (20)     4825 2022-08-22 16:31:54.000000 deeplabcut-2.3rc2/deeplabcut/create_project/new_3d.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/generate_training_dataset/
--rw-r--r--   0 alex       (501) staff       (20)      504 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/deeplabcut/generate_training_dataset/__init__.py
--rwxr-xr-x   0 alex       (501) staff       (20)    22756 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/generate_training_dataset/frame_extraction.py
--rwxr-xr-x   0 alex       (501) staff       (20)    23036 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/generate_training_dataset/multiple_individuals_trainingsetmanipulation.py
--rwxr-xr-x   0 alex       (501) staff       (20)    46615 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/generate_training_dataset/trainingsetmanipulation.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/gui/
--rw-r--r--   0 alex       (501) staff       (20)      419 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/gui/assets/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/gui/assets/icons/
--rw-r--r--   0 alex       (501) staff       (20)     4738 2022-10-09 01:25:35.000000 deeplabcut-2.3rc2/deeplabcut/gui/assets/icons/help.png
--rw-r--r--   0 alex       (501) staff       (20)     5061 2022-10-09 01:25:35.000000 deeplabcut-2.3rc2/deeplabcut/gui/assets/icons/help2.png
--rw-r--r--   0 alex       (501) staff       (20)    15880 2022-10-09 01:25:35.000000 deeplabcut-2.3rc2/deeplabcut/gui/assets/icons/new_project.png
--rw-r--r--   0 alex       (501) staff       (20)    17049 2022-10-09 01:25:35.000000 deeplabcut-2.3rc2/deeplabcut/gui/assets/icons/new_project2.png
--rw-r--r--   0 alex       (501) staff       (20)     6313 2022-10-09 01:25:35.000000 deeplabcut-2.3rc2/deeplabcut/gui/assets/icons/open.png
--rw-r--r--   0 alex       (501) staff       (20)     3242 2022-10-09 01:25:35.000000 deeplabcut-2.3rc2/deeplabcut/gui/assets/icons/open2.png
--rw-r--r--   0 alex       (501) staff       (20)   162713 2022-10-09 01:25:35.000000 deeplabcut-2.3rc2/deeplabcut/gui/assets/logo.png
--rw-r--r--   0 alex       (501) staff       (20)   130352 2022-10-09 01:25:35.000000 deeplabcut-2.3rc2/deeplabcut/gui/assets/logo_transparent.png
--rw-r--r--   0 alex       (501) staff       (20)   160086 2022-10-09 01:25:35.000000 deeplabcut-2.3rc2/deeplabcut/gui/assets/welcome.png
--rw-r--r--   0 alex       (501) staff       (20)     9052 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/components.py
--rw-r--r--   0 alex       (501) staff       (20)      647 2022-10-09 01:25:35.000000 deeplabcut-2.3rc2/deeplabcut/gui/dlc_params.py
--rw-r--r--   0 alex       (501) staff       (20)     1902 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/launch_script.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/gui/media/
--rw-r--r--   0 alex       (501) staff       (20)        0 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/deeplabcut/gui/media/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    61371 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/deeplabcut/gui/media/dlc_1-01.png
--rw-r--r--   0 alex       (501) staff       (20)     2370 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/deeplabcut/gui/media/logo.png
--rw-r--r--   0 alex       (501) staff       (20)      309 2022-10-09 01:25:35.000000 deeplabcut-2.3rc2/deeplabcut/gui/style.qss
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/gui/tabs/
--rw-r--r--   0 alex       (501) staff       (20)      898 2022-10-09 01:25:35.000000 deeplabcut-2.3rc2/deeplabcut/gui/tabs/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    13604 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/tabs/analyze_videos.py
--rw-r--r--   0 alex       (501) staff       (20)     7438 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/tabs/create_project.py
--rw-r--r--   0 alex       (501) staff       (20)     5512 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/tabs/create_training_dataset.py
--rw-r--r--   0 alex       (501) staff       (20)     9177 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/tabs/create_videos.py
--rw-r--r--   0 alex       (501) staff       (20)     6439 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/tabs/evaluate_network.py
--rw-r--r--   0 alex       (501) staff       (20)     7724 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/tabs/extract_frames.py
--rw-r--r--   0 alex       (501) staff       (20)     5998 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/tabs/extract_outlier_frames.py
--rw-r--r--   0 alex       (501) staff       (20)     1463 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/tabs/label_frames.py
--rw-r--r--   0 alex       (501) staff       (20)     2156 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/tabs/manage_project.py
--rw-r--r--   0 alex       (501) staff       (20)     2796 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/tabs/open_project.py
--rw-r--r--   0 alex       (501) staff       (20)    10027 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/tabs/refine_tracklets.py
--rw-r--r--   0 alex       (501) staff       (20)     5817 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/tabs/train_network.py
--rw-r--r--   0 alex       (501) staff       (20)     4269 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/tabs/unsupervised_id_tracking.py
--rw-r--r--   0 alex       (501) staff       (20)     6461 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/tabs/video_editor.py
--rw-r--r--   0 alex       (501) staff       (20)    35580 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/tracklet_toolbox.py
--rw-r--r--   0 alex       (501) staff       (20)      920 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/utils.py
--rw-r--r--   0 alex       (501) staff       (20)    23966 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/widgets.py
--rw-r--r--   0 alex       (501) staff       (20)    18783 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/gui/window.py
--rw-r--r--   0 alex       (501) staff       (20)     1419 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/deeplabcut/inference_cfg.yaml
--rw-r--r--   0 alex       (501) staff       (20)     6882 2022-07-19 14:21:41.000000 deeplabcut-2.3rc2/deeplabcut/pose_cfg.yaml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_3d/
--rw-r--r--   0 alex       (501) staff       (20)      176 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_3d/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    19369 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_3d/camera_calibration.py
--rw-r--r--   0 alex       (501) staff       (20)    15511 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_3d/plotting3D.py
--rw-r--r--   0 alex       (501) staff       (20)    24567 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_3d/triangulation.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/
--rw-r--r--   0 alex       (501) staff       (20)     1081 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/backbones/
--rw-r--r--   0 alex       (501) staff       (20)        0 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/backbones/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    11213 2022-04-07 19:49:51.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/backbones/efficientnet_builder.py
--rw-r--r--   0 alex       (501) staff       (20)    20889 2022-01-06 23:12:13.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/backbones/efficientnet_model.py
--rw-r--r--   0 alex       (501) staff       (20)    17305 2022-04-07 19:49:51.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/backbones/mobilenet.py
--rw-r--r--   0 alex       (501) staff       (20)     8120 2022-04-07 19:49:51.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/backbones/mobilenet_v2.py
--rw-r--r--   0 alex       (501) staff       (20)     1744 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/config.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/
--rw-r--r--   0 alex       (501) staff       (20)        0 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    41903 2022-08-22 16:31:54.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/evaluate.py
--rw-r--r--   0 alex       (501) staff       (20)    29133 2022-08-22 16:31:54.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/evaluate_multianimal.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/openvino/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-04-07 19:49:51.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/openvino/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/openvino/mo_extensions/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-04-07 19:49:51.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/openvino/mo_extensions/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/openvino/mo_extensions/front/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-04-07 19:49:51.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/openvino/mo_extensions/front/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/openvino/mo_extensions/front/tf/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-04-07 19:49:51.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/openvino/mo_extensions/front/tf/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1892 2022-04-10 22:15:38.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/openvino/mo_extensions/front/tf/unravel_index.py
--rw-r--r--   0 alex       (501) staff       (20)     4430 2022-04-10 22:15:38.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/openvino/session.py
--rw-r--r--   0 alex       (501) staff       (20)     8533 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/predict.py
--rw-r--r--   0 alex       (501) staff       (20)    10129 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/predict_multianimal.py
--rw-r--r--   0 alex       (501) staff       (20)     2682 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/test.py
--rw-r--r--   0 alex       (501) staff       (20)    10788 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/train.py
--rw-r--r--   0 alex       (501) staff       (20)     7822 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/train_multianimal.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/
--rw-r--r--   0 alex       (501) staff       (20)      782 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     4882 2022-07-19 14:21:41.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/augmentation.py
--rw-r--r--   0 alex       (501) staff       (20)      964 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/factory.py
--rw-r--r--   0 alex       (501) staff       (20)      991 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/pose_base.py
--rw-r--r--   0 alex       (501) staff       (20)    10491 2022-10-04 20:06:36.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/pose_deterministic.py
--rw-r--r--   0 alex       (501) staff       (20)    21595 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/pose_imgaug.py
--rw-r--r--   0 alex       (501) staff       (20)    28835 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/pose_multianimal_imgaug.py
--rw-r--r--   0 alex       (501) staff       (20)     1583 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/pose_scalecrop.py
--rw-r--r--   0 alex       (501) staff       (20)    17946 2022-10-04 20:06:36.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/pose_tensorpack.py
--rw-r--r--   0 alex       (501) staff       (20)     1623 2022-01-06 23:12:13.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/utils.py
--rw-r--r--   0 alex       (501) staff       (20)     1560 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/default_config.py
--rw-r--r--   0 alex       (501) staff       (20)    12014 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/export.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/lib/
--rw-r--r--   0 alex       (501) staff       (20)      322 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/lib/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    15306 2022-08-22 16:31:54.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/lib/crossvalutils.py
--rw-r--r--   0 alex       (501) staff       (20)    39067 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/lib/inferenceutils.py
--rw-r--r--   0 alex       (501) staff       (20)    28953 2022-10-04 20:29:05.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/lib/trackingutils.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/models/
--rw-r--r--   0 alex       (501) staff       (20)        0 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/models/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/models/pretrained/
--rw-r--r--   0 alex       (501) staff       (20)        0 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/models/pretrained/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      274 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/models/pretrained/download.sh
--rw-r--r--   0 alex       (501) staff       (20)     1828 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/models/pretrained/pretrained_model_urls.yaml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/
--rw-r--r--   0 alex       (501) staff       (20)      666 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     8515 2022-04-10 22:15:38.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/base.py
--rw-r--r--   0 alex       (501) staff       (20)    13787 2022-04-07 19:49:51.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/conv_blocks.py
--rw-r--r--   0 alex       (501) staff       (20)     2037 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/efficientnet.py
--rw-r--r--   0 alex       (501) staff       (20)      895 2021-12-11 11:48:15.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/factory.py
--rw-r--r--   0 alex       (501) staff       (20)     2020 2022-04-10 22:15:38.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/layers.py
--rw-r--r--   0 alex       (501) staff       (20)     2846 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/mobilenet.py
--rw-r--r--   0 alex       (501) staff       (20)    16991 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/multi.py
--rw-r--r--   0 alex       (501) staff       (20)     2328 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/resnet.py
--rw-r--r--   0 alex       (501) staff       (20)     8898 2021-12-11 11:48:15.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/utils.py
--rw-r--r--   0 alex       (501) staff       (20)    15372 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/predict_multianimal.py
--rw-r--r--   0 alex       (501) staff       (20)    74142 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/predict_videos.py
--rw-r--r--   0 alex       (501) staff       (20)     8500 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/training.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/util/
--rw-r--r--   0 alex       (501) staff       (20)      161 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/util/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      487 2021-08-06 13:06:27.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/util/logging.py
--rw-r--r--   0 alex       (501) staff       (20)     2928 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/util/visualize.py
--rw-r--r--   0 alex       (501) staff       (20)     2211 2021-07-07 16:42:37.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/vis_dataset.py
--rw-r--r--   0 alex       (501) staff       (20)    19847 2022-08-22 16:31:54.000000 deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/visualizemaps.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/
--rw-r--r--   0 alex       (501) staff       (20)      432 2022-04-10 22:15:38.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     4366 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/apis.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/config/
--rw-r--r--   0 alex       (501) staff       (20)      510 2022-04-10 22:15:38.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/config/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     3372 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/create_dataset.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/datasets/
--rw-r--r--   0 alex       (501) staff       (20)      313 2022-04-10 22:15:38.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/datasets/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1308 2022-04-10 22:15:38.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/datasets/dlc_vec.py
--rw-r--r--   0 alex       (501) staff       (20)      664 2022-04-10 22:15:38.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/datasets/make_dataloader.py
--rw-r--r--   0 alex       (501) staff       (20)     2618 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/inference.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/loss/
--rw-r--r--   0 alex       (501) staff       (20)       41 2022-04-09 07:43:39.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/loss/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      227 2022-04-09 07:43:39.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/loss/make_loss.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/model/
--rw-r--r--   0 alex       (501) staff       (20)      326 2022-04-10 22:15:38.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/model/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/model/backbones/
--rw-r--r--   0 alex       (501) staff       (20)       48 2022-04-09 07:43:39.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/model/backbones/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    14893 2022-08-22 16:31:54.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/model/backbones/vit_pytorch.py
--rw-r--r--   0 alex       (501) staff       (20)     1740 2022-04-10 22:15:38.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/model/make_model.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/processor/
--rw-r--r--   0 alex       (501) staff       (20)      357 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/processor/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     9003 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/processor/processor.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/solver/
--rw-r--r--   0 alex       (501) staff       (20)       48 2022-04-09 07:43:39.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/solver/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     4094 2022-04-08 15:55:47.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/solver/cosine_lr.py
--rw-r--r--   0 alex       (501) staff       (20)     1091 2022-04-08 16:38:25.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/solver/make_optimizer.py
--rw-r--r--   0 alex       (501) staff       (20)     4926 2022-04-08 15:55:47.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/solver/scheduler.py
--rw-r--r--   0 alex       (501) staff       (20)      746 2022-04-08 15:55:47.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/solver/scheduler_factory.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/tracking_utils/
--rw-r--r--   0 alex       (501) staff       (20)      153 2022-04-08 15:55:47.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/tracking_utils/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      456 2022-04-08 15:55:47.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/tracking_utils/meter.py
--rw-r--r--   0 alex       (501) staff       (20)     4682 2022-04-08 15:55:47.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/tracking_utils/metrics.py
--rw-r--r--   0 alex       (501) staff       (20)     1523 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/tracking_utils/preprocessing.py
--rw-r--r--   0 alex       (501) staff       (20)     4446 2022-04-10 22:15:38.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/tracking_utils/reranking.py
--rw-r--r--   0 alex       (501) staff       (20)     3313 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/train_dlctransreid.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/post_processing/
--rw-r--r--   0 alex       (501) staff       (20)      388 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/post_processing/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    10417 2022-08-22 16:31:54.000000 deeplabcut-2.3rc2/deeplabcut/post_processing/analyze_skeleton.py
--rw-r--r--   0 alex       (501) staff       (20)    10525 2022-08-22 16:31:54.000000 deeplabcut-2.3rc2/deeplabcut/post_processing/filtering.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/refine_training_dataset/
--rw-r--r--   0 alex       (501) staff       (20)      389 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/refine_training_dataset/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    39235 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/refine_training_dataset/outlier_frames.py
--rw-r--r--   0 alex       (501) staff       (20)    46449 2022-10-29 17:19:05.000000 deeplabcut-2.3rc2/deeplabcut/refine_training_dataset/stitch.py
--rw-r--r--   0 alex       (501) staff       (20)    16360 2021-08-06 13:06:27.000000 deeplabcut-2.3rc2/deeplabcut/refine_training_dataset/tracklets.py
--rw-r--r--   0 alex       (501) staff       (20)      922 2022-04-08 15:55:47.000000 deeplabcut-2.3rc2/deeplabcut/reid_cfg.yaml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut/utils/
--rw-r--r--   0 alex       (501) staff       (20)      379 2022-11-04 17:28:45.000000 deeplabcut-2.3rc2/deeplabcut/utils/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     6420 2022-11-04 17:28:45.000000 deeplabcut-2.3rc2/deeplabcut/utils/auxfun_models.py
--rw-r--r--   0 alex       (501) staff       (20)    22851 2022-11-04 17:28:45.000000 deeplabcut-2.3rc2/deeplabcut/utils/auxfun_multianimal.py
--rw-r--r--   0 alex       (501) staff       (20)    19436 2022-11-04 17:28:45.000000 deeplabcut-2.3rc2/deeplabcut/utils/auxfun_videos.py
--rw-r--r--   0 alex       (501) staff       (20)    28114 2022-11-04 17:28:45.000000 deeplabcut-2.3rc2/deeplabcut/utils/auxiliaryfunctions.py
--rw-r--r--   0 alex       (501) staff       (20)    11744 2022-11-04 17:28:45.000000 deeplabcut-2.3rc2/deeplabcut/utils/auxiliaryfunctions_3d.py
--rw-r--r--   0 alex       (501) staff       (20)     9725 2022-11-04 17:28:45.000000 deeplabcut-2.3rc2/deeplabcut/utils/conversioncode.py
--rw-r--r--   0 alex       (501) staff       (20)    16249 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/utils/frameselectiontools.py
--rw-r--r--   0 alex       (501) staff       (20)    38111 2022-11-04 17:28:45.000000 deeplabcut-2.3rc2/deeplabcut/utils/make_labeled_video.py
--rw-r--r--   0 alex       (501) staff       (20)    15418 2022-11-04 17:28:45.000000 deeplabcut-2.3rc2/deeplabcut/utils/plotting.py
--rw-r--r--   0 alex       (501) staff       (20)     6496 2022-06-21 10:33:29.000000 deeplabcut-2.3rc2/deeplabcut/utils/skeleton.py
--rw-r--r--   0 alex       (501) staff       (20)     3799 2021-12-11 11:48:15.000000 deeplabcut-2.3rc2/deeplabcut/utils/video_processor.py
--rw-r--r--   0 alex       (501) staff       (20)    12006 2021-12-11 11:48:15.000000 deeplabcut-2.3rc2/deeplabcut/utils/visualization.py
--rw-r--r--   0 alex       (501) staff       (20)      314 2022-11-04 17:35:49.000000 deeplabcut-2.3rc2/deeplabcut/version.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)    26272 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     8416 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       33 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut.egg-info/entry_points.txt
--rw-r--r--   0 alex       (501) staff       (20)      430 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       11 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/deeplabcut.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2022-11-04 17:39:23.000000 deeplabcut-2.3rc2/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)     3128 2022-11-04 17:39:06.000000 deeplabcut-2.3rc2/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.534149 deeplabcut-2.3rc3/
+-rw-r--r--   0 alex       (501) staff       (20)     4016 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/AUTHORS
+-rw-r--r--   0 alex       (501) staff       (20)     7652 2021-07-07 16:42:37.000000 deeplabcut-2.3rc3/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)     4853 2022-11-22 22:21:25.000000 deeplabcut-2.3rc3/NOTICE.yml
+-rw-r--r--   0 alex       (501) staff       (20)    26553 2022-11-23 10:44:34.533979 deeplabcut-2.3rc3/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)    25870 2022-11-22 22:21:25.000000 deeplabcut-2.3rc3/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.513339 deeplabcut-2.3rc3/deeplabcut/
+-rw-r--r--   0 alex       (501) staff       (20)     3359 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      715 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/__main__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.515038 deeplabcut-2.3rc3/deeplabcut/benchmark/
+-rw-r--r--   0 alex       (501) staff       (20)     3965 2022-11-04 17:28:45.000000 deeplabcut-2.3rc3/deeplabcut/benchmark/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      345 2022-11-04 17:28:45.000000 deeplabcut-2.3rc3/deeplabcut/benchmark/__main__.py
+-rw-r--r--   0 alex       (501) staff       (20)     7461 2022-11-04 17:28:45.000000 deeplabcut-2.3rc3/deeplabcut/benchmark/base.py
+-rw-r--r--   0 alex       (501) staff       (20)     8574 2022-11-04 17:28:45.000000 deeplabcut-2.3rc3/deeplabcut/benchmark/benchmarks.py
+-rw-r--r--   0 alex       (501) staff       (20)     1262 2022-11-04 17:28:45.000000 deeplabcut-2.3rc3/deeplabcut/benchmark/cli.py
+-rw-r--r--   0 alex       (501) staff       (20)     8248 2022-11-04 17:28:45.000000 deeplabcut-2.3rc3/deeplabcut/benchmark/metrics.py
+-rw-r--r--   0 alex       (501) staff       (20)     2194 2022-11-04 17:28:45.000000 deeplabcut-2.3rc3/deeplabcut/benchmark/utils.py
+-rw-r--r--   0 alex       (501) staff       (20)    23955 2022-10-04 20:28:48.000000 deeplabcut-2.3rc3/deeplabcut/cli.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.515758 deeplabcut-2.3rc3/deeplabcut/create_project/
+-rw-r--r--   0 alex       (501) staff       (20)      367 2021-07-07 16:42:37.000000 deeplabcut-2.3rc3/deeplabcut/create_project/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     5314 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/create_project/add.py
+-rw-r--r--   0 alex       (501) staff       (20)     2061 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/create_project/demo_data.py
+-rw-r--r--   0 alex       (501) staff       (20)    11676 2022-11-23 10:23:30.000000 deeplabcut-2.3rc3/deeplabcut/create_project/modelzoo.py
+-rw-r--r--   0 alex       (501) staff       (20)    10930 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/create_project/new.py
+-rw-r--r--   0 alex       (501) staff       (20)     4825 2022-08-22 16:31:54.000000 deeplabcut-2.3rc3/deeplabcut/create_project/new_3d.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.516248 deeplabcut-2.3rc3/deeplabcut/generate_training_dataset/
+-rw-r--r--   0 alex       (501) staff       (20)      504 2021-07-07 16:42:37.000000 deeplabcut-2.3rc3/deeplabcut/generate_training_dataset/__init__.py
+-rwxr-xr-x   0 alex       (501) staff       (20)    22244 2022-11-22 22:21:25.000000 deeplabcut-2.3rc3/deeplabcut/generate_training_dataset/frame_extraction.py
+-rwxr-xr-x   0 alex       (501) staff       (20)    23036 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/generate_training_dataset/multiple_individuals_trainingsetmanipulation.py
+-rwxr-xr-x   0 alex       (501) staff       (20)    46615 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/generate_training_dataset/trainingsetmanipulation.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.517289 deeplabcut-2.3rc3/deeplabcut/gui/
+-rw-r--r--   0 alex       (501) staff       (20)      419 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.517836 deeplabcut-2.3rc3/deeplabcut/gui/assets/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.518580 deeplabcut-2.3rc3/deeplabcut/gui/assets/icons/
+-rw-r--r--   0 alex       (501) staff       (20)     4738 2022-10-09 01:25:35.000000 deeplabcut-2.3rc3/deeplabcut/gui/assets/icons/help.png
+-rw-r--r--   0 alex       (501) staff       (20)     5061 2022-10-09 01:25:35.000000 deeplabcut-2.3rc3/deeplabcut/gui/assets/icons/help2.png
+-rw-r--r--   0 alex       (501) staff       (20)    15880 2022-10-09 01:25:35.000000 deeplabcut-2.3rc3/deeplabcut/gui/assets/icons/new_project.png
+-rw-r--r--   0 alex       (501) staff       (20)    17049 2022-10-09 01:25:35.000000 deeplabcut-2.3rc3/deeplabcut/gui/assets/icons/new_project2.png
+-rw-r--r--   0 alex       (501) staff       (20)     6313 2022-10-09 01:25:35.000000 deeplabcut-2.3rc3/deeplabcut/gui/assets/icons/open.png
+-rw-r--r--   0 alex       (501) staff       (20)     3242 2022-10-09 01:25:35.000000 deeplabcut-2.3rc3/deeplabcut/gui/assets/icons/open2.png
+-rw-r--r--   0 alex       (501) staff       (20)   162713 2022-10-09 01:25:35.000000 deeplabcut-2.3rc3/deeplabcut/gui/assets/logo.png
+-rw-r--r--   0 alex       (501) staff       (20)   130352 2022-10-09 01:25:35.000000 deeplabcut-2.3rc3/deeplabcut/gui/assets/logo_transparent.png
+-rw-r--r--   0 alex       (501) staff       (20)   160086 2022-10-09 01:25:35.000000 deeplabcut-2.3rc3/deeplabcut/gui/assets/welcome.png
+-rw-r--r--   0 alex       (501) staff       (20)     9050 2022-11-22 22:21:25.000000 deeplabcut-2.3rc3/deeplabcut/gui/components.py
+-rw-r--r--   0 alex       (501) staff       (20)      647 2022-10-09 01:25:35.000000 deeplabcut-2.3rc3/deeplabcut/gui/dlc_params.py
+-rw-r--r--   0 alex       (501) staff       (20)     1902 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/launch_script.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.518935 deeplabcut-2.3rc3/deeplabcut/gui/media/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2021-07-07 16:42:37.000000 deeplabcut-2.3rc3/deeplabcut/gui/media/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    61371 2021-07-07 16:42:37.000000 deeplabcut-2.3rc3/deeplabcut/gui/media/dlc_1-01.png
+-rw-r--r--   0 alex       (501) staff       (20)     2370 2021-07-07 16:42:37.000000 deeplabcut-2.3rc3/deeplabcut/gui/media/logo.png
+-rw-r--r--   0 alex       (501) staff       (20)      309 2022-10-09 01:25:35.000000 deeplabcut-2.3rc3/deeplabcut/gui/style.qss
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.520586 deeplabcut-2.3rc3/deeplabcut/gui/tabs/
+-rw-r--r--   0 alex       (501) staff       (20)      898 2022-10-09 01:25:35.000000 deeplabcut-2.3rc3/deeplabcut/gui/tabs/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    13604 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/tabs/analyze_videos.py
+-rw-r--r--   0 alex       (501) staff       (20)     7438 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/tabs/create_project.py
+-rw-r--r--   0 alex       (501) staff       (20)     5512 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/tabs/create_training_dataset.py
+-rw-r--r--   0 alex       (501) staff       (20)     9177 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/tabs/create_videos.py
+-rw-r--r--   0 alex       (501) staff       (20)     6439 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/tabs/evaluate_network.py
+-rw-r--r--   0 alex       (501) staff       (20)     7724 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/tabs/extract_frames.py
+-rw-r--r--   0 alex       (501) staff       (20)     5998 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/tabs/extract_outlier_frames.py
+-rw-r--r--   0 alex       (501) staff       (20)     1463 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/tabs/label_frames.py
+-rw-r--r--   0 alex       (501) staff       (20)     2156 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/tabs/manage_project.py
+-rw-r--r--   0 alex       (501) staff       (20)     2796 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/tabs/open_project.py
+-rw-r--r--   0 alex       (501) staff       (20)    10027 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/tabs/refine_tracklets.py
+-rw-r--r--   0 alex       (501) staff       (20)     5817 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/tabs/train_network.py
+-rw-r--r--   0 alex       (501) staff       (20)     4269 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/tabs/unsupervised_id_tracking.py
+-rw-r--r--   0 alex       (501) staff       (20)     6461 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/tabs/video_editor.py
+-rw-r--r--   0 alex       (501) staff       (20)    35580 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/tracklet_toolbox.py
+-rw-r--r--   0 alex       (501) staff       (20)      920 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/utils.py
+-rw-r--r--   0 alex       (501) staff       (20)    23966 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/gui/widgets.py
+-rw-r--r--   0 alex       (501) staff       (20)    18785 2022-11-22 22:21:25.000000 deeplabcut-2.3rc3/deeplabcut/gui/window.py
+-rw-r--r--   0 alex       (501) staff       (20)     1419 2021-07-07 16:42:37.000000 deeplabcut-2.3rc3/deeplabcut/inference_cfg.yaml
+-rw-r--r--   0 alex       (501) staff       (20)     6882 2022-07-19 14:21:41.000000 deeplabcut-2.3rc3/deeplabcut/pose_cfg.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.521042 deeplabcut-2.3rc3/deeplabcut/pose_estimation_3d/
+-rw-r--r--   0 alex       (501) staff       (20)      176 2021-07-07 16:42:37.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_3d/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    19369 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_3d/camera_calibration.py
+-rw-r--r--   0 alex       (501) staff       (20)    15511 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_3d/plotting3D.py
+-rw-r--r--   0 alex       (501) staff       (20)    24567 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_3d/triangulation.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.522103 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/
+-rw-r--r--   0 alex       (501) staff       (20)     1081 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.522686 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/backbones/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2021-07-07 16:42:37.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/backbones/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    11213 2022-04-07 19:49:51.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/backbones/efficientnet_builder.py
+-rw-r--r--   0 alex       (501) staff       (20)    20889 2022-01-06 23:12:13.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/backbones/efficientnet_model.py
+-rw-r--r--   0 alex       (501) staff       (20)    17305 2022-04-07 19:49:51.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/backbones/mobilenet.py
+-rw-r--r--   0 alex       (501) staff       (20)     8120 2022-04-07 19:49:51.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/backbones/mobilenet_v2.py
+-rw-r--r--   0 alex       (501) staff       (20)     1744 2021-07-07 16:42:37.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/config.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.523593 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2021-07-07 16:42:37.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    41903 2022-08-22 16:31:54.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/evaluate.py
+-rw-r--r--   0 alex       (501) staff       (20)    29133 2022-08-22 16:31:54.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/evaluate_multianimal.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.523787 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/openvino/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-04-07 19:49:51.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/openvino/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.523895 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/openvino/mo_extensions/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-04-07 19:49:51.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/openvino/mo_extensions/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.523983 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/openvino/mo_extensions/front/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-04-07 19:49:51.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/openvino/mo_extensions/front/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.524178 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/openvino/mo_extensions/front/tf/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-04-07 19:49:51.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/openvino/mo_extensions/front/tf/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1892 2022-04-10 22:15:38.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/openvino/mo_extensions/front/tf/unravel_index.py
+-rw-r--r--   0 alex       (501) staff       (20)     4430 2022-04-10 22:15:38.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/openvino/session.py
+-rw-r--r--   0 alex       (501) staff       (20)     8533 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/predict.py
+-rw-r--r--   0 alex       (501) staff       (20)    10129 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/predict_multianimal.py
+-rw-r--r--   0 alex       (501) staff       (20)     2682 2021-07-07 16:42:37.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/test.py
+-rw-r--r--   0 alex       (501) staff       (20)    10788 2022-11-04 17:35:49.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/train.py
+-rw-r--r--   0 alex       (501) staff       (20)     7822 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/train_multianimal.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.525323 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/
+-rw-r--r--   0 alex       (501) staff       (20)      782 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     4939 2022-11-22 22:21:25.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/augmentation.py
+-rw-r--r--   0 alex       (501) staff       (20)      964 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/factory.py
+-rw-r--r--   0 alex       (501) staff       (20)      991 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/pose_base.py
+-rw-r--r--   0 alex       (501) staff       (20)    10491 2022-10-04 20:06:36.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/pose_deterministic.py
+-rw-r--r--   0 alex       (501) staff       (20)    21595 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/pose_imgaug.py
+-rw-r--r--   0 alex       (501) staff       (20)    28835 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/pose_multianimal_imgaug.py
+-rw-r--r--   0 alex       (501) staff       (20)     1583 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/pose_scalecrop.py
+-rw-r--r--   0 alex       (501) staff       (20)    17946 2022-10-04 20:06:36.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/pose_tensorpack.py
+-rw-r--r--   0 alex       (501) staff       (20)     1623 2022-01-06 23:12:13.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/utils.py
+-rw-r--r--   0 alex       (501) staff       (20)     1560 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/default_config.py
+-rw-r--r--   0 alex       (501) staff       (20)    12014 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/export.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.525778 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/lib/
+-rw-r--r--   0 alex       (501) staff       (20)      322 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/lib/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    15306 2022-08-22 16:31:54.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/lib/crossvalutils.py
+-rw-r--r--   0 alex       (501) staff       (20)    39067 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/lib/inferenceutils.py
+-rw-r--r--   0 alex       (501) staff       (20)    28953 2022-10-04 20:29:05.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/lib/trackingutils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.525907 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/models/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2021-07-07 16:42:37.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/models/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.526195 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/models/pretrained/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2021-07-07 16:42:37.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/models/pretrained/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      274 2022-11-23 01:27:59.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/models/pretrained/download.sh
+-rw-r--r--   0 alex       (501) staff       (20)     2987 2022-11-23 10:35:01.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/models/pretrained/pretrained_model_urls.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.527298 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/
+-rw-r--r--   0 alex       (501) staff       (20)      666 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     8515 2022-04-10 22:15:38.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/base.py
+-rw-r--r--   0 alex       (501) staff       (20)    13787 2022-04-07 19:49:51.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/conv_blocks.py
+-rw-r--r--   0 alex       (501) staff       (20)     2037 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/efficientnet.py
+-rw-r--r--   0 alex       (501) staff       (20)      895 2021-12-11 11:48:15.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/factory.py
+-rw-r--r--   0 alex       (501) staff       (20)     2020 2022-04-10 22:15:38.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/layers.py
+-rw-r--r--   0 alex       (501) staff       (20)     2846 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/mobilenet.py
+-rw-r--r--   0 alex       (501) staff       (20)    16991 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/multi.py
+-rw-r--r--   0 alex       (501) staff       (20)     2328 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/resnet.py
+-rw-r--r--   0 alex       (501) staff       (20)     8898 2021-12-11 11:48:15.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/utils.py
+-rw-r--r--   0 alex       (501) staff       (20)    15372 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/predict_multianimal.py
+-rw-r--r--   0 alex       (501) staff       (20)    73496 2022-11-22 22:21:25.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/predict_videos.py
+-rw-r--r--   0 alex       (501) staff       (20)     8500 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/training.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.527618 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/util/
+-rw-r--r--   0 alex       (501) staff       (20)      161 2021-07-07 16:42:37.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/util/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      487 2021-08-06 13:06:27.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/util/logging.py
+-rw-r--r--   0 alex       (501) staff       (20)     2928 2021-07-07 16:42:37.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/util/visualize.py
+-rw-r--r--   0 alex       (501) staff       (20)     2211 2021-07-07 16:42:37.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/vis_dataset.py
+-rw-r--r--   0 alex       (501) staff       (20)    19847 2022-08-22 16:31:54.000000 deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/visualizemaps.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.528141 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/
+-rw-r--r--   0 alex       (501) staff       (20)      432 2022-04-10 22:15:38.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     4366 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/apis.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.528256 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/config/
+-rw-r--r--   0 alex       (501) staff       (20)      510 2022-04-10 22:15:38.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/config/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     3372 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/create_dataset.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.528579 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/datasets/
+-rw-r--r--   0 alex       (501) staff       (20)      313 2022-04-10 22:15:38.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/datasets/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1308 2022-04-10 22:15:38.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/datasets/dlc_vec.py
+-rw-r--r--   0 alex       (501) staff       (20)      664 2022-04-10 22:15:38.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/datasets/make_dataloader.py
+-rw-r--r--   0 alex       (501) staff       (20)     2618 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/inference.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.528797 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/loss/
+-rw-r--r--   0 alex       (501) staff       (20)       41 2022-04-09 07:43:39.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/loss/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      227 2022-04-09 07:43:39.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/loss/make_loss.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.529010 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/model/
+-rw-r--r--   0 alex       (501) staff       (20)      326 2022-04-10 22:15:38.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/model/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.529259 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/model/backbones/
+-rw-r--r--   0 alex       (501) staff       (20)       48 2022-04-09 07:43:39.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/model/backbones/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    14893 2022-08-22 16:31:54.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/model/backbones/vit_pytorch.py
+-rw-r--r--   0 alex       (501) staff       (20)     1740 2022-04-10 22:15:38.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/model/make_model.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.529703 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/processor/
+-rw-r--r--   0 alex       (501) staff       (20)      357 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/processor/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     9003 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/processor/processor.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.530496 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/solver/
+-rw-r--r--   0 alex       (501) staff       (20)       48 2022-04-09 07:43:39.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/solver/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     4094 2022-04-08 15:55:47.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/solver/cosine_lr.py
+-rw-r--r--   0 alex       (501) staff       (20)     1091 2022-04-08 16:38:25.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/solver/make_optimizer.py
+-rw-r--r--   0 alex       (501) staff       (20)     4926 2022-04-08 15:55:47.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/solver/scheduler.py
+-rw-r--r--   0 alex       (501) staff       (20)      746 2022-04-08 15:55:47.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/solver/scheduler_factory.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.531133 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/tracking_utils/
+-rw-r--r--   0 alex       (501) staff       (20)      153 2022-04-08 15:55:47.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/tracking_utils/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      456 2022-04-08 15:55:47.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/tracking_utils/meter.py
+-rw-r--r--   0 alex       (501) staff       (20)     4682 2022-04-08 15:55:47.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/tracking_utils/metrics.py
+-rw-r--r--   0 alex       (501) staff       (20)     1523 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/tracking_utils/preprocessing.py
+-rw-r--r--   0 alex       (501) staff       (20)     4446 2022-04-10 22:15:38.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/tracking_utils/reranking.py
+-rw-r--r--   0 alex       (501) staff       (20)     3313 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/train_dlctransreid.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.531511 deeplabcut-2.3rc3/deeplabcut/post_processing/
+-rw-r--r--   0 alex       (501) staff       (20)      388 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/post_processing/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    10417 2022-08-22 16:31:54.000000 deeplabcut-2.3rc3/deeplabcut/post_processing/analyze_skeleton.py
+-rw-r--r--   0 alex       (501) staff       (20)    10525 2022-08-22 16:31:54.000000 deeplabcut-2.3rc3/deeplabcut/post_processing/filtering.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.532170 deeplabcut-2.3rc3/deeplabcut/refine_training_dataset/
+-rw-r--r--   0 alex       (501) staff       (20)      389 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/refine_training_dataset/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    39170 2022-11-22 22:21:25.000000 deeplabcut-2.3rc3/deeplabcut/refine_training_dataset/outlier_frames.py
+-rw-r--r--   0 alex       (501) staff       (20)    46449 2022-10-29 17:19:05.000000 deeplabcut-2.3rc3/deeplabcut/refine_training_dataset/stitch.py
+-rw-r--r--   0 alex       (501) staff       (20)    16360 2021-08-06 13:06:27.000000 deeplabcut-2.3rc3/deeplabcut/refine_training_dataset/tracklets.py
+-rw-r--r--   0 alex       (501) staff       (20)      922 2022-04-08 15:55:47.000000 deeplabcut-2.3rc3/deeplabcut/reid_cfg.yaml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.533759 deeplabcut-2.3rc3/deeplabcut/utils/
+-rw-r--r--   0 alex       (501) staff       (20)      379 2022-11-04 17:28:45.000000 deeplabcut-2.3rc3/deeplabcut/utils/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     8552 2022-11-23 10:16:08.000000 deeplabcut-2.3rc3/deeplabcut/utils/auxfun_models.py
+-rw-r--r--   0 alex       (501) staff       (20)    22851 2022-11-04 17:28:45.000000 deeplabcut-2.3rc3/deeplabcut/utils/auxfun_multianimal.py
+-rw-r--r--   0 alex       (501) staff       (20)    19436 2022-11-04 17:28:45.000000 deeplabcut-2.3rc3/deeplabcut/utils/auxfun_videos.py
+-rw-r--r--   0 alex       (501) staff       (20)    28114 2022-11-04 17:28:45.000000 deeplabcut-2.3rc3/deeplabcut/utils/auxiliaryfunctions.py
+-rw-r--r--   0 alex       (501) staff       (20)    11744 2022-11-04 17:28:45.000000 deeplabcut-2.3rc3/deeplabcut/utils/auxiliaryfunctions_3d.py
+-rw-r--r--   0 alex       (501) staff       (20)     9725 2022-11-04 17:28:45.000000 deeplabcut-2.3rc3/deeplabcut/utils/conversioncode.py
+-rw-r--r--   0 alex       (501) staff       (20)    14697 2022-11-22 22:21:25.000000 deeplabcut-2.3rc3/deeplabcut/utils/frameselectiontools.py
+-rw-r--r--   0 alex       (501) staff       (20)    38111 2022-11-04 17:28:45.000000 deeplabcut-2.3rc3/deeplabcut/utils/make_labeled_video.py
+-rw-r--r--   0 alex       (501) staff       (20)    15418 2022-11-04 17:28:45.000000 deeplabcut-2.3rc3/deeplabcut/utils/plotting.py
+-rw-r--r--   0 alex       (501) staff       (20)     6496 2022-06-21 10:33:29.000000 deeplabcut-2.3rc3/deeplabcut/utils/skeleton.py
+-rw-r--r--   0 alex       (501) staff       (20)     3799 2021-12-11 11:48:15.000000 deeplabcut-2.3rc3/deeplabcut/utils/video_processor.py
+-rw-r--r--   0 alex       (501) staff       (20)    12006 2021-12-11 11:48:15.000000 deeplabcut-2.3rc3/deeplabcut/utils/visualization.py
+-rw-r--r--   0 alex       (501) staff       (20)      314 2022-11-23 10:16:35.000000 deeplabcut-2.3rc3/deeplabcut/version.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-23 10:44:34.514196 deeplabcut-2.3rc3/deeplabcut.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)    26553 2022-11-23 10:44:34.000000 deeplabcut-2.3rc3/deeplabcut.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     8427 2022-11-23 10:44:34.000000 deeplabcut-2.3rc3/deeplabcut.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2022-11-23 10:44:34.000000 deeplabcut-2.3rc3/deeplabcut.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       33 2022-11-23 10:44:34.000000 deeplabcut-2.3rc3/deeplabcut.egg-info/entry_points.txt
+-rw-r--r--   0 alex       (501) staff       (20)      458 2022-11-23 10:44:34.000000 deeplabcut-2.3rc3/deeplabcut.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       11 2022-11-23 10:44:34.000000 deeplabcut-2.3rc3/deeplabcut.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)       38 2022-11-23 10:44:34.534195 deeplabcut-2.3rc3/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)     3169 2022-11-23 10:16:35.000000 deeplabcut-2.3rc3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `deeplabcut-2.3rc2/AUTHORS` & `deeplabcut-2.3rc3/AUTHORS`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/LICENSE` & `deeplabcut-2.3rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/PKG-INFO` & `deeplabcut-2.3rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: deeplabcut
-Version: 2.3rc2
+Version: 2.3rc3
 Summary: Markerless pose-estimation of user-defined features with deep learning
 Home-page: https://github.com/DeepLabCut/DeepLabCut
 Author: A. & M. Mathis Labs
 Author-email: alexander@deeplabcut.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: gui
 Provides-Extra: openvino
 Provides-Extra: docs
 Provides-Extra: tf
 Provides-Extra: apple_mchips
+Provides-Extra: modelzoo
 License-File: LICENSE
+License-File: NOTICE.yml
 License-File: AUTHORS
 
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 ![Python package](https://github.com/DeepLabCut/DeepLabCut/workflows/Python%20package/badge.svg)
 [![PyPI version](https://badge.fury.io/py/deeplabcut.svg)](https://badge.fury.io/py/deeplabcut)
 [![Downloads](https://pepy.tech/badge/deeplabcut)](https://pepy.tech/project/deeplabcut)
 [![Downloads](https://pepy.tech/badge/deeplabcut/month)](https://pepy.tech/project/deeplabcut)
@@ -47,25 +49,27 @@
 <img src="https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/1619609897110-TKSTWKEM6HTGXID9D489/ke17ZwdGBToddI8pDm48kAvjv6tW_eojYQmNU0ncbllZw-zPPgdn4jUwVcJE1ZvWEtT5uBSRWt4vQZAgTJucoTqqXjS3CfNDSuuf31e0tVHBSTXHtjUKlhRtWJ1Vo6l1B2bxJtByvWSjL6Vz3amc5yb8BodarTVrzIWCp72ioWw/triMouseDLC.gif?format=300w" height="150">
 
 <img src="https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/5c3fbd0c898583417a040dfc/1547681053201/rat-grasp.gif?format=300w" height="150">
 </p>
 
 DeepLabCut is a toolbox for markerless pose estimation of animals performing various tasks. [Read a short development and application summary below](https://github.com/DeepLabCut/DeepLabCut#why-use-deeplabcut). As long as you can see (label) what you want to track, you can use this toolbox, as it is animal and object agnostic.
 
+**Quick start** read the docs: https://deeplabcut.github.io/DeepLabCut
+
 **Latest updates:**
 
 :purple_heart: **DeepLabCut supports multi-animal pose estimation!** maDLC is out of beta/rc mode and beta is deprecated, thanks to the testers out there for feedback! Your labeled data will be backwards compatible, but not all other steps. Please see the [new `2.2+` releases](https://github.com/DeepLabCut/DeepLabCut/releases) for what's new & how to install it, please see our new [paper, Lauer et al 2022](https://www.nature.com/articles/s41592-022-01443-0), and the [new docs]( https://deeplabcut.github.io/DeepLabCut) on how to use it!
 
 :purple_heart: We support multi-animal re-identification, see [Lauer et al 2022](https://www.nature.com/articles/s41592-022-01443-0).
 
 :purple_heart: We have a **real-time** package available! http://DLClive.deeplabcut.org
 
 # [Installation: how to install DeepLabCut](https://deeplabcut.github.io/DeepLabCut/docs/installation.html)
 
-Very quick start: `pip install "deeplabcut[gui]"` that includes all GUI functions, or `pip install deeplabcut` (headless version).
+Very quick start: `pip install "deeplabcut[gui,tf]"` that includes all functions plus GUIs, or `pip install deeplabcut[tf]` (headless version with PyTorch and TensorFlow).
 * We recommend using our conda file, see [here](https://github.com/DeepLabCut/DeepLabCut/blob/master/conda-environments/README.md) or the new [`deeplabcut-docker` package](https://github.com/DeepLabCut/DeepLabCut/tree/master/docker).
 
 # [Documentation: The DeepLabCut Process](https://deeplabcut.github.io/DeepLabCut)
 
 Our docs walk you through using DeepLabCut, and key API points. For an overview of the toolbox and workflow for project management, see our step-by-step at [Nature Protocols paper](https://doi.org/10.1038/s41596-019-0176-0).
 
 For a deeper understanding and more resources for you to get started with Python and DeepLabCut, please check out our free online course! http://DLCcourse.deeplabcut.org
@@ -76,15 +80,15 @@
 
 # [DEMO the code](/examples)
 
 We provide data and several Jupyter Notebooks: one that walks you through a demo dataset to test your installation, and another Notebook to run DeepLabCut from the beginning on your own data. We also show you how to use the code in Docker, and on Google Colab.
 
 # Why use DeepLabCut?
 
-In 2018, we demonstrated the capabilities for [trail tracking](https://vnmurthylab.org/), [reaching in mice](http://www.mousemotorlab.org/) and various Drosophila behaviors during egg-laying (see [Mathis et al.](https://www.nature.com/articles/s41593-018-0209-y) for details). There is, however, nothing specific that makes the toolbox only applicable to these tasks and/or species. The toolbox has already been successfully applied (by us and others) to [rats](http://www.mousemotorlab.org/deeplabcut), humans, various fish species, bacteria, leeches, various robots, cheetahs, [mouse whiskers](http://www.mousemotorlab.org/deeplabcut) and [race horses](http://www.mousemotorlab.org/deeplabcut). DeepLabCut utilized the feature detectors (ResNets + readout layers) of one of the state-of-the-art algorithms for human pose estimation by Insafutdinov et al., called DeeperCut, which inspired the name for our toolbox (see references below). Since this time, the package has changed substantially.  The code has been re-tooled and re-factored since 2.1+: We have added faster and higher performance variants with MobileNetV2s, EfficientNets, and our own DLCRNet backbones (see [Pretraining boosts out-of-domain robustness for pose estimation](https://arxiv.org/abs/1909.11229) and [Lauer et al 2021](https://www.biorxiv.org/content/10.1101/2021.04.30.442096v1)). Additionally, we have improved the inference speed and provided both additional and novel augmentation methods, added real-time, and multi-animal support. We currently provide state-of-the-art performance for animal pose estimation.
+In 2018, we demonstrated the capabilities for [trail tracking](https://vnmurthylab.org/), [reaching in mice](http://www.mousemotorlab.org/) and various Drosophila behaviors during egg-laying (see [Mathis et al.](https://www.nature.com/articles/s41593-018-0209-y) for details). There is, however, nothing specific that makes the toolbox only applicable to these tasks and/or species. The toolbox has already been successfully applied (by us and others) to [rats](http://www.mousemotorlab.org/deeplabcut), humans, various fish species, bacteria, leeches, various robots, cheetahs, [mouse whiskers](http://www.mousemotorlab.org/deeplabcut) and [race horses](http://www.mousemotorlab.org/deeplabcut). DeepLabCut utilized the feature detectors (ResNets + readout layers) of one of the state-of-the-art algorithms for human pose estimation by Insafutdinov et al., called DeeperCut, which inspired the name for our toolbox (see references below). Since this time, the package has changed substantially.  The code has been re-tooled and re-factored since 2.1+: We have added faster and higher performance variants with MobileNetV2s, EfficientNets, and our own DLCRNet backbones (see [Pretraining boosts out-of-domain robustness for pose estimation](https://arxiv.org/abs/1909.11229) and [Lauer et al 2022](https://www.nature.com/articles/s41592-022-01443-0)). Additionally, we have improved the inference speed and provided both additional and novel augmentation methods, added real-time, and multi-animal support. We currently provide state-of-the-art performance for animal pose estimation.
 
 <p align="center">
 <img src="https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/5c3e47258a922d548c483247/1547585339819/ErrorvsTrainingsetSize.png?format=750w" height="160">
 <img src="https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/5c3e469d8a922d548c4828fa/1547585194560/compressionrobustness.png?format=750w" height="160">
 <img src="https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/5c3fbed74fa51acecd63deeb/1547681534736/MouseLocomotion_warren.gif?format=500w" height="160">  
 <img src="https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/5c3fc1c6758d46950ce7eec7/1547682383595/cheetah.png?format=750w" height="160">
 </p>
@@ -95,15 +99,15 @@
 
 <p align="center">
 <img src="https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/1588292233203-FD1DVKAQYNV2TU91CO7R/ke17ZwdGBToddI8pDm48kIX24IsDPzy6M4KUaihfICJZw-zPPgdn4jUwVcJE1ZvWQUxwkmyExglNqGp0IvTJZamWLI2zvYWH8K3-s_4yszcp2ryTI0HqTOaaUohrI8PIxtGUdkzp028KVNnpOijF3PweOM5su6FUQHO6Wkh72Nw/dlc_eco.gif?format=1000w" width="80%">
 </p>
 
 ## Code contributors:
 
-DLC code was originally developed by [Alexander Mathis](https://github.com/AlexEMG) & [Mackenzie Mathis](https://github.com/MMathisLab), and was extended in 2.0 with [Tanmay Nath](http://www.mousemotorlab.org/team), and currently (2.1+) actively developed with our CZI DLC Fellow, [Jessy Lauer](https://github.com/jeylau). DeepLabCut is an open-source tool and has benefited from suggestions and edits by many individuals including  Mert Yuksekgonul, Tom Biasi, Richard Warren, Ronny Eichler, Hao Wu, Federico Claudi, Gary Kane and Jonny Saunders as well as the [contributors](https://github.com/DeepLabCut/DeepLabCut/graphs/contributors). Please see [AUTHORS](https://github.com/DeepLabCut/DeepLabCut/blob/master/AUTHORS) for more details!
+DLC code was originally developed by [Alexander Mathis](https://github.com/AlexEMG) & [Mackenzie Mathis](https://github.com/MMathisLab), and was extended in 2.0 with [Tanmay Nath](http://www.mousemotorlab.org/team), and currently (2.1+) actively developed with [Jessy Lauer](https://github.com/jeylau). DeepLabCut is an open-source tool and has benefited from suggestions and edits by many individuals including  Mert Yuksekgonul, Tom Biasi, Richard Warren, Ronny Eichler, Hao Wu, Federico Claudi, Gary Kane and Jonny Saunders as well as the [contributors](https://github.com/DeepLabCut/DeepLabCut/graphs/contributors). Please see [AUTHORS](https://github.com/DeepLabCut/DeepLabCut/blob/master/AUTHORS) for more details!
 
 This is an actively developed package and we welcome community development and involvement.
 
 ## Be part of the DLC Community✨:
 
 | 🚉 Platform                                                 | 🎯 Goal                                                                      | ⏱️ Estimated Response Time | 📢 Support Squad                        |
 |------------------------------------------------------------|-----------------------------------------------------------------------------|---------------------------|----------------------------------------|
@@ -114,20 +118,21 @@
 | 🚧 GitHub DeepLabCut/[Roadmap](https://github.com/DeepLabCut/DeepLabCut/blob/master/docs/roadmap.md)                             | To learn more about our journey✈️                                            | N/A                       | N/A                                    |
 | [![Twitter Follow](https://img.shields.io/twitter/follow/DeepLabCut.svg?label=DeepLabCut&style=social)](https://twitter.com/DeepLabCut)                                                   | To keep up with our latest news and updates 📢                               | Daily                     | DLC Team                               |
 | The DeepLabCut [AI Residency Program](https://www.deeplabcutairesidency.org/)                        | To come and work with us next summer👏                                       | Annually                  | DLC Team                               |
 
 
 ## References:
 
-If you use this code or data we kindly as that you please [cite Mathis et al, 2018](https://www.nature.com/articles/s41593-018-0209-y) and, if you use the Python package (DeepLabCut2.x) please also cite [Nath, Mathis et al, 2019](https://doi.org/10.1038/s41596-019-0176-0). If you utilize the MobileNetV2s or EfficientNets please cite [Mathis, Biasi et al. 2021](https://openaccess.thecvf.com/content/WACV2021/papers/Mathis_Pretraining_Boosts_Out-of-Domain_Robustness_for_Pose_Estimation_WACV_2021_paper.pdf). If you use multi-animal in beta mode, please contact us; if you use the 2.2rc1+, please cite [Lauer et al. 2021](https://www.biorxiv.org/content/10.1101/2021.04.30.442096v1).
+If you use this code or data we kindly as that you please [cite Mathis et al, 2018](https://www.nature.com/articles/s41593-018-0209-y) and, if you use the Python package (DeepLabCut2.x) please also cite [Nath, Mathis et al, 2019](https://doi.org/10.1038/s41596-019-0176-0). If you utilize the MobileNetV2s or EfficientNets please cite [Mathis, Biasi et al. 2021](https://openaccess.thecvf.com/content/WACV2021/papers/Mathis_Pretraining_Boosts_Out-of-Domain_Robustness_for_Pose_Estimation_WACV_2021_paper.pdf). If you use versions 2.2beta+ or 2.2rc1+, please cite [Lauer et al. 2022](https://www.nature.com/articles/s41592-022-01443-0).
 
 DOIs (#ProTip, for helping you find citations for software, check out [CiteAs.org](http://citeas.org/)!):
 
 - Mathis et al 2018: [10.1038/s41593-018-0209-y](https://doi.org/10.1038/s41593-018-0209-y)
 - Nath, Mathis et al 2019: [10.1038/s41596-019-0176-0](https://doi.org/10.1038/s41596-019-0176-0)
+- Lauer et al 2022: [10.1038/s41592-022-01443-0](https://doi.org/10.1038/s41592-022-01443-0)
 
 
 Please check out the following references for more details:
 
     @article{Mathisetal2018,
         title = {DeepLabCut: markerless pose estimation of user-defined body parts with deep learning},
         author = {Alexander Mathis and Pranav Mamidanna and Kevin M. Cury and Taiga Abe  and Venkatesh N. Murthy and Mackenzie W. Mathis and Matthias Bethge},
@@ -160,15 +165,15 @@
 
     @article{insafutdinov2016eccv,
         title = {DeeperCut: A Deeper, Stronger, and Faster Multi-Person Pose Estimation Model},
         author = {Eldar Insafutdinov and Leonid Pishchulin and Bjoern Andres and Mykhaylo Andriluka and Bernt Schiele},
         booktitle = {ECCV'16},
         url = {http://arxiv.org/abs/1605.03170}}
         
-Review articles:
+Review & Educational articles:
 
     @article{Mathis2020DeepLT,
         title={Deep learning tools for the measurement of animal behavior in neuroscience},
         author={Mackenzie W. Mathis and Alexander Mathis},
         journal={Current Opinion in Neurobiology},
         year={2020},
         volume={60},
@@ -192,27 +197,29 @@
         publisher = {Cold Spring Harbor Laboratory},
         URL = {https://www.biorxiv.org/content/early/2018/10/30/457242},
         eprint = {https://www.biorxiv.org/content/early/2018/10/30/457242.full.pdf},
         journal = {bioRxiv}}
 
 ## License:
 
-This project is licensed under the GNU Lesser General Public License v3.0. Note that the software is provided "as is", without warranty of any kind, express or implied. If you use the code or data, please cite us! Note, artwork (DeepLabCut logo) and images are copyrighted; please do not take or use these images without written permission.
+This project is primarily licensed under the GNU Lesser General Public License v3.0. Note that the software is provided "as is", without warranty of any kind, express or implied. If you use the code or data, please cite us! Note, artwork (DeepLabCut logo) and images are copyrighted; please do not take or use these images without written permission.
 
 ## Versions:
 
-VERSION 2.2: Multi-animal pose estimation and tracking with DeepLabCut is supported (as well as single-animal projects).
+VERSION 2.2: Multi-animal pose estimation, identification, and tracking with DeepLabCut is supported (as well as single-animal projects).
 
-VERSION 2.0-2.1: This is the **Python package** of [DeepLabCut](https://www.nature.com/articles/s41593-018-0209-y) that was originally released with our [Nature Protocols](https://doi.org/10.1038/s41596-019-0176-0) paper (preprint [here](https://www.biorxiv.org/content/10.1101/476531v1)).
+VERSION 2.0-2.1: This is the **Python package** of [DeepLabCut](https://www.nature.com/articles/s41593-018-0209-y) that was originally released in Oct 2018 with our [Nature Protocols](https://doi.org/10.1038/s41596-019-0176-0) paper (preprint [here](https://www.biorxiv.org/content/10.1101/476531v1)).
 This package includes graphical user interfaces to label your data, and take you from data set creation to automatic behavioral analysis. It also introduces an active learning framework to efficiently use DeepLabCut on large experimental projects, and data augmentation tools that improve network performance, especially in challenging cases (see [panel b](https://camo.githubusercontent.com/77c92f6b89d44ca758d815bdd7e801247437060b/68747470733a2f2f737461746963312e73717561726573706163652e636f6d2f7374617469632f3537663664353163396637343536366635356563663237312f742f3563336663316336373538643436393530636537656563372f313534373638323338333539352f636865657461682e706e673f666f726d61743d37353077)).
 
 VERSION 1.0: The initial, Nature Neuroscience version of [DeepLabCut](https://www.nature.com/articles/s41593-018-0209-y) can be found in the history of git, or here: https://github.com/DeepLabCut/DeepLabCut/releases/tag/1.11
 
 ## News (and in the news):
 
+- August 2022: DeepLabCut hit 400,000 downloads!
+
 - August 2021: 2.2 becomes the new stable release for DeepLabCut.
 
 - July 2021: Docs are now at https://deeplabcut.github.io/DeepLabCut and we now include TensorFlow 2 support!
 
 - May 2021: DeepLabCut hit 200,000 downloads! Also, Our preprint on 2.2, multi-animal DeepLabCut is released!
 
 - Jan 2021: [Pretraining boosts out-of-domain robustness for pose estimation](https://openaccess.thecvf.com/content/WACV2021/html/Mathis_Pretraining_Boosts_Out-of-Domain_Robustness_for_Pose_Estimation_WACV_2021_paper.html) published in the IEEE Winter Conference on Applications of Computer Vision. We also added EfficientNet backbones to DeepLabCut, those are best trained with cosine decay (see paper). To use them, just pass "`efficientnet-b0`" to "`efficientnet-b6`" when creating the trainingset!
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: deeplabcut Version: 2.3rc2 Summary: Markerless
+Metadata-Version: 2.1 Name: deeplabcut Version: 2.3rc3 Summary: Markerless
 pose-estimation of user-defined features with deep learning Home-page: https://
 github.com/DeepLabCut/DeepLabCut Author: A. & M. Mathis Labs Author-email:
 alexander@deeplabcut.org Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3
 (LGPLv3) Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown Provides-Extra: gui Provides-Extra: openvino Provides-
-Extra: docs Provides-Extra: tf Provides-Extra: apple_mchips License-File:
-LICENSE License-File: AUTHORS [Code_style:_black] ![Python package](https://
-github.com/DeepLabCut/DeepLabCut/workflows/Python%20package/badge.svg) [![PyPI
-version](https://badge.fury.io/py/deeplabcut.svg)](https://badge.fury.io/py/
-deeplabcut) [![Downloads](https://pepy.tech/badge/deeplabcut)](https://
-pepy.tech/project/deeplabcut) [![Downloads](https://pepy.tech/badge/deeplabcut/
-month)](https://pepy.tech/project/deeplabcut) [![GitHub stars](https://
-img.shields.io/github/stars/DeepLabCut/DeepLabCut.svg?style=social&label=Star)]
-(https://github.com/DeepLabCut/DeepLabCut) [![Generic badge](https://
-img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](CONTRIBUTING.md)
-[![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)]
-(https://www.gnu.org/licenses/lgpl-3.0) [![Image.sc forum](https://
-img.shields.io/badge/dynamic/
+Extra: docs Provides-Extra: tf Provides-Extra: apple_mchips Provides-Extra:
+modelzoo License-File: LICENSE License-File: NOTICE.yml License-File: AUTHORS
+[Code_style:_black] ![Python package](https://github.com/DeepLabCut/DeepLabCut/
+workflows/Python%20package/badge.svg) [![PyPI version](https://badge.fury.io/
+py/deeplabcut.svg)](https://badge.fury.io/py/deeplabcut) [![Downloads](https://
+pepy.tech/badge/deeplabcut)](https://pepy.tech/project/deeplabcut) [!
+[Downloads](https://pepy.tech/badge/deeplabcut/month)](https://pepy.tech/
+project/deeplabcut) [![GitHub stars](https://img.shields.io/github/stars/
+DeepLabCut/DeepLabCut.svg?style=social&label=Star)](https://github.com/
+DeepLabCut/DeepLabCut) [![Generic badge](https://img.shields.io/badge/
+Contributions-Welcome-brightgreen.svg)](CONTRIBUTING.md) [![License: LGPL v3]
+(https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/
+licenses/lgpl-3.0) [![Image.sc forum](https://img.shields.io/badge/dynamic/
 json.svg?label=forum&url=https%3A%2F%2Fforum.image.sc%2Ftag%2Fdeeplabcut.json&query=%24.topic_list.tags.0.topic_count&colorB=brightgreen&&suffix=%20topics&logo=data:
 image/
 png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+/
 /
 17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/
 cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://
 forum.image.sc/tag/deeplabcut) [![Gitter](https://badges.gitter.im/DeepLabCut/
@@ -51,38 +51,39 @@
      triMouseDLC.gif?format=300w] [https://static1.squarespace.com/static/
     57f6d51c9f74566f55ecf271/t/5c3fbd0c898583417a040dfc/1547681053201/rat-
                             grasp.gif?format=300w]
 DeepLabCut is a toolbox for markerless pose estimation of animals performing
 various tasks. [Read a short development and application summary below](https:/
 /github.com/DeepLabCut/DeepLabCut#why-use-deeplabcut). As long as you can see
 (label) what you want to track, you can use this toolbox, as it is animal and
-object agnostic. **Latest updates:** :purple_heart: **DeepLabCut supports
-multi-animal pose estimation!** maDLC is out of beta/rc mode and beta is
-deprecated, thanks to the testers out there for feedback! Your labeled data
-will be backwards compatible, but not all other steps. Please see the [new
-`2.2+` releases](https://github.com/DeepLabCut/DeepLabCut/releases) for what's
-new & how to install it, please see our new [paper, Lauer et al 2022](https://
+object agnostic. **Quick start** read the docs: https://deeplabcut.github.io/
+DeepLabCut **Latest updates:** :purple_heart: **DeepLabCut supports multi-
+animal pose estimation!** maDLC is out of beta/rc mode and beta is deprecated,
+thanks to the testers out there for feedback! Your labeled data will be
+backwards compatible, but not all other steps. Please see the [new `2.2+`
+releases](https://github.com/DeepLabCut/DeepLabCut/releases) for what's new &
+how to install it, please see our new [paper, Lauer et al 2022](https://
 www.nature.com/articles/s41592-022-01443-0), and the [new docs]( https://
 deeplabcut.github.io/DeepLabCut) on how to use it! :purple_heart: We support
 multi-animal re-identification, see [Lauer et al 2022](https://www.nature.com/
 articles/s41592-022-01443-0). :purple_heart: We have a **real-time** package
 available! http://DLClive.deeplabcut.org # [Installation: how to install
 DeepLabCut](https://deeplabcut.github.io/DeepLabCut/docs/installation.html)
-Very quick start: `pip install "deeplabcut[gui]"` that includes all GUI
-functions, or `pip install deeplabcut` (headless version). * We recommend using
-our conda file, see [here](https://github.com/DeepLabCut/DeepLabCut/blob/
-master/conda-environments/README.md) or the new [`deeplabcut-docker` package]
-(https://github.com/DeepLabCut/DeepLabCut/tree/master/docker). #
-[Documentation: The DeepLabCut Process](https://deeplabcut.github.io/
-DeepLabCut) Our docs walk you through using DeepLabCut, and key API points. For
-an overview of the toolbox and workflow for project management, see our step-
-by-step at [Nature Protocols paper](https://doi.org/10.1038/s41596-019-0176-0).
-For a deeper understanding and more resources for you to get started with
-Python and DeepLabCut, please check out our free online course! http://
-DLCcourse.deeplabcut.org
+Very quick start: `pip install "deeplabcut[gui,tf]"` that includes all
+functions plus GUIs, or `pip install deeplabcut[tf]` (headless version with
+PyTorch and TensorFlow). * We recommend using our conda file, see [here](https:
+//github.com/DeepLabCut/DeepLabCut/blob/master/conda-environments/README.md) or
+the new [`deeplabcut-docker` package](https://github.com/DeepLabCut/DeepLabCut/
+tree/master/docker). # [Documentation: The DeepLabCut Process](https://
+deeplabcut.github.io/DeepLabCut) Our docs walk you through using DeepLabCut,
+and key API points. For an overview of the toolbox and workflow for project
+management, see our step-by-step at [Nature Protocols paper](https://doi.org/
+10.1038/s41596-019-0176-0). For a deeper understanding and more resources for
+you to get started with Python and DeepLabCut, please check out our free online
+course! http://DLCcourse.deeplabcut.org
    [https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/
                       1609244903687-US1SN063QIFJS4BP4IJD/
 ke17ZwdGBToddI8pDm48kFG9xAYub2PPnmh56PTVg7gUqsxRUqqbr1mOJYKfIPR7LoDQ9mXPOjoJoqy81S2I8N_N4V1vUb5AoIIIbLZhVYxCRW4BPu10St3TBAUQYVKcAju5e7u9RZJEVbVQPZRu9xb_m-
                     kUO2M3I1IeDqD4l8YcGqu2nZPx1UhKV8wc1ELN/
                   dlc_overview_whitebkgrnd.png?format=2500w]
 # [DEMO the code](/examples) We provide data and several Jupyter Notebooks: one
 that walks you through a demo dataset to test your installation, and another
@@ -101,19 +102,18 @@
 (ResNets + readout layers) of one of the state-of-the-art algorithms for human
 pose estimation by Insafutdinov et al., called DeeperCut, which inspired the
 name for our toolbox (see references below). Since this time, the package has
 changed substantially. The code has been re-tooled and re-factored since 2.1+:
 We have added faster and higher performance variants with MobileNetV2s,
 EfficientNets, and our own DLCRNet backbones (see [Pretraining boosts out-of-
 domain robustness for pose estimation](https://arxiv.org/abs/1909.11229) and
-[Lauer et al 2021](https://www.biorxiv.org/content/10.1101/
-2021.04.30.442096v1)). Additionally, we have improved the inference speed and
-provided both additional and novel augmentation methods, added real-time, and
-multi-animal support. We currently provide state-of-the-art performance for
-animal pose estimation.
+[Lauer et al 2022](https://www.nature.com/articles/s41592-022-01443-0)).
+Additionally, we have improved the inference speed and provided both additional
+and novel augmentation methods, added real-time, and multi-animal support. We
+currently provide state-of-the-art performance for animal pose estimation.
       [https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/
 5c3e47258a922d548c483247/1547585339819/ErrorvsTrainingsetSize.png?format=750w]
       [https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/
 5c3e469d8a922d548c4828fa/1547585194560/compressionrobustness.png?format=750w]
       [https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/
 5c3fbed74fa51acecd63deeb/1547681534736/MouseLocomotion_warren.gif?format=500w]
       [https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/
@@ -137,28 +137,28 @@
                 ke17ZwdGBToddI8pDm48kIX24IsDPzy6M4KUaihfICJZw-
             zPPgdn4jUwVcJE1ZvWQUxwkmyExglNqGp0IvTJZamWLI2zvYWH8K3-
    s_4yszcp2ryTI0HqTOaaUohrI8PIxtGUdkzp028KVNnpOijF3PweOM5su6FUQHO6Wkh72Nw/
                            dlc_eco.gif?format=1000w]
 ## Code contributors: DLC code was originally developed by [Alexander Mathis]
 (https://github.com/AlexEMG) & [Mackenzie Mathis](https://github.com/
 MMathisLab), and was extended in 2.0 with [Tanmay Nath](http://
-www.mousemotorlab.org/team), and currently (2.1+) actively developed with our
-CZI DLC Fellow, [Jessy Lauer](https://github.com/jeylau). DeepLabCut is an
-open-source tool and has benefited from suggestions and edits by many
-individuals including Mert Yuksekgonul, Tom Biasi, Richard Warren, Ronny
-Eichler, Hao Wu, Federico Claudi, Gary Kane and Jonny Saunders as well as the
-[contributors](https://github.com/DeepLabCut/DeepLabCut/graphs/contributors).
-Please see [AUTHORS](https://github.com/DeepLabCut/DeepLabCut/blob/master/
-AUTHORS) for more details! This is an actively developed package and we welcome
-community development and involvement. ## Be part of the DLC Communityâ¨: |
-ð Platform | ð¯ Goal | â±ï¸ Estimated Response Time | ð¢ Support Squad
-| |------------------------------------------------------------|---------------
---------------------------------------------------------------|----------------
------------|----------------------------------------| | [![Image.sc forum]
-(https://img.shields.io/badge/dynamic/
+www.mousemotorlab.org/team), and currently (2.1+) actively developed with
+[Jessy Lauer](https://github.com/jeylau). DeepLabCut is an open-source tool and
+has benefited from suggestions and edits by many individuals including Mert
+Yuksekgonul, Tom Biasi, Richard Warren, Ronny Eichler, Hao Wu, Federico Claudi,
+Gary Kane and Jonny Saunders as well as the [contributors](https://github.com/
+DeepLabCut/DeepLabCut/graphs/contributors). Please see [AUTHORS](https://
+github.com/DeepLabCut/DeepLabCut/blob/master/AUTHORS) for more details! This is
+an actively developed package and we welcome community development and
+involvement. ## Be part of the DLC Communityâ¨: | ð Platform | ð¯ Goal |
+â±ï¸ Estimated Response Time | ð¢ Support Squad | |------------------------
+------------------------------------|------------------------------------------
+-----------------------------------|---------------------------|---------------
+-------------------------| | [![Image.sc forum](https://img.shields.io/badge/
+dynamic/
 json.svg?label=forum&url=https%3A%2F%2Fforum.image.sc%2Ftag%2Fdeeplabcut.json&query=%24.topic_list.tags.0.topic_count&colorB=brightgreen&&suffix=%20topics&logo=data:
 image/
 png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+/
 /
 17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/
 cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://
 forum.image.sc/tag/deeplabcut)
@@ -181,88 +181,88 @@
 come and work with us next summerð | Annually | DLC Team | ## References: If
 you use this code or data we kindly as that you please [cite Mathis et al,
 2018](https://www.nature.com/articles/s41593-018-0209-y) and, if you use the
 Python package (DeepLabCut2.x) please also cite [Nath, Mathis et al, 2019]
 (https://doi.org/10.1038/s41596-019-0176-0). If you utilize the MobileNetV2s or
 EfficientNets please cite [Mathis, Biasi et al. 2021](https://
 openaccess.thecvf.com/content/WACV2021/papers/Mathis_Pretraining_Boosts_Out-of-
-Domain_Robustness_for_Pose_Estimation_WACV_2021_paper.pdf). If you use multi-
-animal in beta mode, please contact us; if you use the 2.2rc1+, please cite
-[Lauer et al. 2021](https://www.biorxiv.org/content/10.1101/
-2021.04.30.442096v1). DOIs (#ProTip, for helping you find citations for
+Domain_Robustness_for_Pose_Estimation_WACV_2021_paper.pdf). If you use versions
+2.2beta+ or 2.2rc1+, please cite [Lauer et al. 2022](https://www.nature.com/
+articles/s41592-022-01443-0). DOIs (#ProTip, for helping you find citations for
 software, check out [CiteAs.org](http://citeas.org/)!): - Mathis et al 2018:
 [10.1038/s41593-018-0209-y](https://doi.org/10.1038/s41593-018-0209-y) - Nath,
 Mathis et al 2019: [10.1038/s41596-019-0176-0](https://doi.org/10.1038/s41596-
-019-0176-0) Please check out the following references for more details:
-@article{Mathisetal2018, title = {DeepLabCut: markerless pose estimation of
-user-defined body parts with deep learning}, author = {Alexander Mathis and
-Pranav Mamidanna and Kevin M. Cury and Taiga Abe and Venkatesh N. Murthy and
-Mackenzie W. Mathis and Matthias Bethge}, journal = {Nature Neuroscience}, year
-= {2018}, url = {https://www.nature.com/articles/s41593-018-0209-y}} @article
-{NathMathisetal2019, title = {Using DeepLabCut for 3D markerless pose
-estimation across species and behaviors}, author = {Nath*, Tanmay and Mathis*,
-Alexander and Chen, An Chi and Patel, Amir and Bethge, Matthias and Mathis,
-Mackenzie W}, journal = {Nature Protocols}, year = {2019}, url = {https://
-doi.org/10.1038/s41596-019-0176-0}} @InProceedings{Mathis_2021_WACV, author =
-{Mathis, Alexander and Biasi, Thomas and Schneider, Steffen and Yuksekgonul,
-Mert and Rogers, Byron and Bethge, Matthias and Mathis, Mackenzie W.}, title =
-{Pretraining Boosts Out-of-Domain Robustness for Pose Estimation}, booktitle =
-{Proceedings of the IEEE/CVF Winter Conference on Applications of Computer
-Vision (WACV)}, month = {January}, year = {2021}, pages = {1859-1868}} @article
-{Lauer2022MultianimalPE, title={Multi-animal pose estimation, identification
-and tracking with DeepLabCut}, author={Jessy Lauer and Mu Zhou and Shaokai Ye
-and William Menegas and Steffen Schneider and Tanmay Nath and Mohammed
-Mostafizur Rahman and Valentina Di Santo and Daniel Soberanes and Guoping Feng
-and Venkatesh N. Murthy and George Lauder and Catherine Dulac and M. Mathis and
-Alexander Mathis}, journal={Nature Methods}, year={2022}, volume={19}, pages=
-{496 - 504}} @article{insafutdinov2016eccv, title = {DeeperCut: A Deeper,
-Stronger, and Faster Multi-Person Pose Estimation Model}, author = {Eldar
-Insafutdinov and Leonid Pishchulin and Bjoern Andres and Mykhaylo Andriluka and
-Bernt Schiele}, booktitle = {ECCV'16}, url = {http://arxiv.org/abs/1605.03170}}
-Review articles: @article{Mathis2020DeepLT, title={Deep learning tools for the
-measurement of animal behavior in neuroscience}, author={Mackenzie W. Mathis
-and Alexander Mathis}, journal={Current Opinion in Neurobiology}, year={2020},
-volume={60}, pages={1-11}} @article{Mathis2020Primer, title={A Primer on Motion
-Capture with Deep Learning: Principles, Pitfalls, and Perspectives}, author=
-{Alexander Mathis and Steffen Schneider and Jessy Lauer and Mackenzie W.
-Mathis}, journal={Neuron}, year={2020}, volume={108}, pages={44-65}} Other
-open-access pre-prints related to our work on DeepLabCut: @article
-{MathisWarren2018speed, author = {Mathis, Alexander and Warren, Richard A.},
-title = {On the inference speed and video-compression robustness of
-DeepLabCut}, year = {2018}, doi = {10.1101/457242}, publisher = {Cold Spring
-Harbor Laboratory}, URL = {https://www.biorxiv.org/content/early/2018/10/30/
-457242}, eprint = {https://www.biorxiv.org/content/early/2018/10/30/
-457242.full.pdf}, journal = {bioRxiv}} ## License: This project is licensed
-under the GNU Lesser General Public License v3.0. Note that the software is
-provided "as is", without warranty of any kind, express or implied. If you use
-the code or data, please cite us! Note, artwork (DeepLabCut logo) and images
-are copyrighted; please do not take or use these images without written
-permission. ## Versions: VERSION 2.2: Multi-animal pose estimation and tracking
-with DeepLabCut is supported (as well as single-animal projects). VERSION 2.0-
-2.1: This is the **Python package** of [DeepLabCut](https://www.nature.com/
-articles/s41593-018-0209-y) that was originally released with our [Nature
-Protocols](https://doi.org/10.1038/s41596-019-0176-0) paper (preprint [here]
-(https://www.biorxiv.org/content/10.1101/476531v1)). This package includes
-graphical user interfaces to label your data, and take you from data set
-creation to automatic behavioral analysis. It also introduces an active
-learning framework to efficiently use DeepLabCut on large experimental
-projects, and data augmentation tools that improve network performance,
-especially in challenging cases (see [panel b](https://
-camo.githubusercontent.com/77c92f6b89d44ca758d815bdd7e801247437060b/
+019-0176-0) - Lauer et al 2022: [10.1038/s41592-022-01443-0](https://doi.org/
+10.1038/s41592-022-01443-0) Please check out the following references for more
+details: @article{Mathisetal2018, title = {DeepLabCut: markerless pose
+estimation of user-defined body parts with deep learning}, author = {Alexander
+Mathis and Pranav Mamidanna and Kevin M. Cury and Taiga Abe and Venkatesh N.
+Murthy and Mackenzie W. Mathis and Matthias Bethge}, journal = {Nature
+Neuroscience}, year = {2018}, url = {https://www.nature.com/articles/s41593-
+018-0209-y}} @article{NathMathisetal2019, title = {Using DeepLabCut for 3D
+markerless pose estimation across species and behaviors}, author = {Nath*,
+Tanmay and Mathis*, Alexander and Chen, An Chi and Patel, Amir and Bethge,
+Matthias and Mathis, Mackenzie W}, journal = {Nature Protocols}, year = {2019},
+url = {https://doi.org/10.1038/s41596-019-0176-0}} @InProceedings
+{Mathis_2021_WACV, author = {Mathis, Alexander and Biasi, Thomas and Schneider,
+Steffen and Yuksekgonul, Mert and Rogers, Byron and Bethge, Matthias and
+Mathis, Mackenzie W.}, title = {Pretraining Boosts Out-of-Domain Robustness for
+Pose Estimation}, booktitle = {Proceedings of the IEEE/CVF Winter Conference on
+Applications of Computer Vision (WACV)}, month = {January}, year = {2021},
+pages = {1859-1868}} @article{Lauer2022MultianimalPE, title={Multi-animal pose
+estimation, identification and tracking with DeepLabCut}, author={Jessy Lauer
+and Mu Zhou and Shaokai Ye and William Menegas and Steffen Schneider and Tanmay
+Nath and Mohammed Mostafizur Rahman and Valentina Di Santo and Daniel Soberanes
+and Guoping Feng and Venkatesh N. Murthy and George Lauder and Catherine Dulac
+and M. Mathis and Alexander Mathis}, journal={Nature Methods}, year={2022},
+volume={19}, pages={496 - 504}} @article{insafutdinov2016eccv, title =
+{DeeperCut: A Deeper, Stronger, and Faster Multi-Person Pose Estimation Model},
+author = {Eldar Insafutdinov and Leonid Pishchulin and Bjoern Andres and
+Mykhaylo Andriluka and Bernt Schiele}, booktitle = {ECCV'16}, url = {http://
+arxiv.org/abs/1605.03170}} Review & Educational articles: @article
+{Mathis2020DeepLT, title={Deep learning tools for the measurement of animal
+behavior in neuroscience}, author={Mackenzie W. Mathis and Alexander Mathis},
+journal={Current Opinion in Neurobiology}, year={2020}, volume={60}, pages={1-
+11}} @article{Mathis2020Primer, title={A Primer on Motion Capture with Deep
+Learning: Principles, Pitfalls, and Perspectives}, author={Alexander Mathis and
+Steffen Schneider and Jessy Lauer and Mackenzie W. Mathis}, journal={Neuron},
+year={2020}, volume={108}, pages={44-65}} Other open-access pre-prints related
+to our work on DeepLabCut: @article{MathisWarren2018speed, author = {Mathis,
+Alexander and Warren, Richard A.}, title = {On the inference speed and video-
+compression robustness of DeepLabCut}, year = {2018}, doi = {10.1101/457242},
+publisher = {Cold Spring Harbor Laboratory}, URL = {https://www.biorxiv.org/
+content/early/2018/10/30/457242}, eprint = {https://www.biorxiv.org/content/
+early/2018/10/30/457242.full.pdf}, journal = {bioRxiv}} ## License: This
+project is primarily licensed under the GNU Lesser General Public License v3.0.
+Note that the software is provided "as is", without warranty of any kind,
+express or implied. If you use the code or data, please cite us! Note, artwork
+(DeepLabCut logo) and images are copyrighted; please do not take or use these
+images without written permission. ## Versions: VERSION 2.2: Multi-animal pose
+estimation, identification, and tracking with DeepLabCut is supported (as well
+as single-animal projects). VERSION 2.0-2.1: This is the **Python package** of
+[DeepLabCut](https://www.nature.com/articles/s41593-018-0209-y) that was
+originally released in Oct 2018 with our [Nature Protocols](https://doi.org/
+10.1038/s41596-019-0176-0) paper (preprint [here](https://www.biorxiv.org/
+content/10.1101/476531v1)). This package includes graphical user interfaces to
+label your data, and take you from data set creation to automatic behavioral
+analysis. It also introduces an active learning framework to efficiently use
+DeepLabCut on large experimental projects, and data augmentation tools that
+improve network performance, especially in challenging cases (see [panel b]
+(https://camo.githubusercontent.com/77c92f6b89d44ca758d815bdd7e801247437060b/
 68747470733a2f2f737461746963312e73717561726573706163652e636f6d2f7374617469632f3537663664353163396637343536366635356563663237312f742f3563336663316336373538643436393530636537656563372f313534373638323338333539352f636865657461682e706e673f666f726d61743d37353077)).
 VERSION 1.0: The initial, Nature Neuroscience version of [DeepLabCut](https://
 www.nature.com/articles/s41593-018-0209-y) can be found in the history of git,
 or here: https://github.com/DeepLabCut/DeepLabCut/releases/tag/1.11 ## News
-(and in the news): - August 2021: 2.2 becomes the new stable release for
-DeepLabCut. - July 2021: Docs are now at https://deeplabcut.github.io/
-DeepLabCut and we now include TensorFlow 2 support! - May 2021: DeepLabCut hit
-200,000 downloads! Also, Our preprint on 2.2, multi-animal DeepLabCut is
-released! - Jan 2021: [Pretraining boosts out-of-domain robustness for pose
-estimation](https://openaccess.thecvf.com/content/WACV2021/html/
-Mathis_Pretraining_Boosts_Out-of-
+(and in the news): - August 2022: DeepLabCut hit 400,000 downloads! - August
+2021: 2.2 becomes the new stable release for DeepLabCut. - July 2021: Docs are
+now at https://deeplabcut.github.io/DeepLabCut and we now include TensorFlow 2
+support! - May 2021: DeepLabCut hit 200,000 downloads! Also, Our preprint on
+2.2, multi-animal DeepLabCut is released! - Jan 2021: [Pretraining boosts out-
+of-domain robustness for pose estimation](https://openaccess.thecvf.com/
+content/WACV2021/html/Mathis_Pretraining_Boosts_Out-of-
 Domain_Robustness_for_Pose_Estimation_WACV_2021_paper.html) published in the
 IEEE Winter Conference on Applications of Computer Vision. We also added
 EfficientNet backbones to DeepLabCut, those are best trained with cosine decay
 (see paper). To use them, just pass "`efficientnet-b0`" to "`efficientnet-b6`"
 when creating the trainingset! - Dec 2020: We released a real-time package that
 allows for online pose estimation and real-time feedback. See
 [DLClive.deeplabcut.org](http://DLClive.deeplabcut.org). - 5/22 2020: We
```

### Comparing `deeplabcut-2.3rc2/README.md` & `deeplabcut-2.3rc3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,27 @@
 <img src="https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/1619609897110-TKSTWKEM6HTGXID9D489/ke17ZwdGBToddI8pDm48kAvjv6tW_eojYQmNU0ncbllZw-zPPgdn4jUwVcJE1ZvWEtT5uBSRWt4vQZAgTJucoTqqXjS3CfNDSuuf31e0tVHBSTXHtjUKlhRtWJ1Vo6l1B2bxJtByvWSjL6Vz3amc5yb8BodarTVrzIWCp72ioWw/triMouseDLC.gif?format=300w" height="150">
 
 <img src="https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/5c3fbd0c898583417a040dfc/1547681053201/rat-grasp.gif?format=300w" height="150">
 </p>
 
 DeepLabCut is a toolbox for markerless pose estimation of animals performing various tasks. [Read a short development and application summary below](https://github.com/DeepLabCut/DeepLabCut#why-use-deeplabcut). As long as you can see (label) what you want to track, you can use this toolbox, as it is animal and object agnostic.
 
+**Quick start** read the docs: https://deeplabcut.github.io/DeepLabCut
+
 **Latest updates:**
 
 :purple_heart: **DeepLabCut supports multi-animal pose estimation!** maDLC is out of beta/rc mode and beta is deprecated, thanks to the testers out there for feedback! Your labeled data will be backwards compatible, but not all other steps. Please see the [new `2.2+` releases](https://github.com/DeepLabCut/DeepLabCut/releases) for what's new & how to install it, please see our new [paper, Lauer et al 2022](https://www.nature.com/articles/s41592-022-01443-0), and the [new docs]( https://deeplabcut.github.io/DeepLabCut) on how to use it!
 
 :purple_heart: We support multi-animal re-identification, see [Lauer et al 2022](https://www.nature.com/articles/s41592-022-01443-0).
 
 :purple_heart: We have a **real-time** package available! http://DLClive.deeplabcut.org
 
 # [Installation: how to install DeepLabCut](https://deeplabcut.github.io/DeepLabCut/docs/installation.html)
 
-Very quick start: `pip install "deeplabcut[gui]"` that includes all GUI functions, or `pip install deeplabcut` (headless version).
+Very quick start: `pip install "deeplabcut[gui,tf]"` that includes all functions plus GUIs, or `pip install deeplabcut[tf]` (headless version with PyTorch and TensorFlow).
 * We recommend using our conda file, see [here](https://github.com/DeepLabCut/DeepLabCut/blob/master/conda-environments/README.md) or the new [`deeplabcut-docker` package](https://github.com/DeepLabCut/DeepLabCut/tree/master/docker).
 
 # [Documentation: The DeepLabCut Process](https://deeplabcut.github.io/DeepLabCut)
 
 Our docs walk you through using DeepLabCut, and key API points. For an overview of the toolbox and workflow for project management, see our step-by-step at [Nature Protocols paper](https://doi.org/10.1038/s41596-019-0176-0).
 
 For a deeper understanding and more resources for you to get started with Python and DeepLabCut, please check out our free online course! http://DLCcourse.deeplabcut.org
@@ -57,15 +59,15 @@
 
 # [DEMO the code](/examples)
 
 We provide data and several Jupyter Notebooks: one that walks you through a demo dataset to test your installation, and another Notebook to run DeepLabCut from the beginning on your own data. We also show you how to use the code in Docker, and on Google Colab.
 
 # Why use DeepLabCut?
 
-In 2018, we demonstrated the capabilities for [trail tracking](https://vnmurthylab.org/), [reaching in mice](http://www.mousemotorlab.org/) and various Drosophila behaviors during egg-laying (see [Mathis et al.](https://www.nature.com/articles/s41593-018-0209-y) for details). There is, however, nothing specific that makes the toolbox only applicable to these tasks and/or species. The toolbox has already been successfully applied (by us and others) to [rats](http://www.mousemotorlab.org/deeplabcut), humans, various fish species, bacteria, leeches, various robots, cheetahs, [mouse whiskers](http://www.mousemotorlab.org/deeplabcut) and [race horses](http://www.mousemotorlab.org/deeplabcut). DeepLabCut utilized the feature detectors (ResNets + readout layers) of one of the state-of-the-art algorithms for human pose estimation by Insafutdinov et al., called DeeperCut, which inspired the name for our toolbox (see references below). Since this time, the package has changed substantially.  The code has been re-tooled and re-factored since 2.1+: We have added faster and higher performance variants with MobileNetV2s, EfficientNets, and our own DLCRNet backbones (see [Pretraining boosts out-of-domain robustness for pose estimation](https://arxiv.org/abs/1909.11229) and [Lauer et al 2021](https://www.biorxiv.org/content/10.1101/2021.04.30.442096v1)). Additionally, we have improved the inference speed and provided both additional and novel augmentation methods, added real-time, and multi-animal support. We currently provide state-of-the-art performance for animal pose estimation.
+In 2018, we demonstrated the capabilities for [trail tracking](https://vnmurthylab.org/), [reaching in mice](http://www.mousemotorlab.org/) and various Drosophila behaviors during egg-laying (see [Mathis et al.](https://www.nature.com/articles/s41593-018-0209-y) for details). There is, however, nothing specific that makes the toolbox only applicable to these tasks and/or species. The toolbox has already been successfully applied (by us and others) to [rats](http://www.mousemotorlab.org/deeplabcut), humans, various fish species, bacteria, leeches, various robots, cheetahs, [mouse whiskers](http://www.mousemotorlab.org/deeplabcut) and [race horses](http://www.mousemotorlab.org/deeplabcut). DeepLabCut utilized the feature detectors (ResNets + readout layers) of one of the state-of-the-art algorithms for human pose estimation by Insafutdinov et al., called DeeperCut, which inspired the name for our toolbox (see references below). Since this time, the package has changed substantially.  The code has been re-tooled and re-factored since 2.1+: We have added faster and higher performance variants with MobileNetV2s, EfficientNets, and our own DLCRNet backbones (see [Pretraining boosts out-of-domain robustness for pose estimation](https://arxiv.org/abs/1909.11229) and [Lauer et al 2022](https://www.nature.com/articles/s41592-022-01443-0)). Additionally, we have improved the inference speed and provided both additional and novel augmentation methods, added real-time, and multi-animal support. We currently provide state-of-the-art performance for animal pose estimation.
 
 <p align="center">
 <img src="https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/5c3e47258a922d548c483247/1547585339819/ErrorvsTrainingsetSize.png?format=750w" height="160">
 <img src="https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/5c3e469d8a922d548c4828fa/1547585194560/compressionrobustness.png?format=750w" height="160">
 <img src="https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/5c3fbed74fa51acecd63deeb/1547681534736/MouseLocomotion_warren.gif?format=500w" height="160">  
 <img src="https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/5c3fc1c6758d46950ce7eec7/1547682383595/cheetah.png?format=750w" height="160">
 </p>
@@ -76,15 +78,15 @@
 
 <p align="center">
 <img src="https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/1588292233203-FD1DVKAQYNV2TU91CO7R/ke17ZwdGBToddI8pDm48kIX24IsDPzy6M4KUaihfICJZw-zPPgdn4jUwVcJE1ZvWQUxwkmyExglNqGp0IvTJZamWLI2zvYWH8K3-s_4yszcp2ryTI0HqTOaaUohrI8PIxtGUdkzp028KVNnpOijF3PweOM5su6FUQHO6Wkh72Nw/dlc_eco.gif?format=1000w" width="80%">
 </p>
 
 ## Code contributors:
 
-DLC code was originally developed by [Alexander Mathis](https://github.com/AlexEMG) & [Mackenzie Mathis](https://github.com/MMathisLab), and was extended in 2.0 with [Tanmay Nath](http://www.mousemotorlab.org/team), and currently (2.1+) actively developed with our CZI DLC Fellow, [Jessy Lauer](https://github.com/jeylau). DeepLabCut is an open-source tool and has benefited from suggestions and edits by many individuals including  Mert Yuksekgonul, Tom Biasi, Richard Warren, Ronny Eichler, Hao Wu, Federico Claudi, Gary Kane and Jonny Saunders as well as the [contributors](https://github.com/DeepLabCut/DeepLabCut/graphs/contributors). Please see [AUTHORS](https://github.com/DeepLabCut/DeepLabCut/blob/master/AUTHORS) for more details!
+DLC code was originally developed by [Alexander Mathis](https://github.com/AlexEMG) & [Mackenzie Mathis](https://github.com/MMathisLab), and was extended in 2.0 with [Tanmay Nath](http://www.mousemotorlab.org/team), and currently (2.1+) actively developed with [Jessy Lauer](https://github.com/jeylau). DeepLabCut is an open-source tool and has benefited from suggestions and edits by many individuals including  Mert Yuksekgonul, Tom Biasi, Richard Warren, Ronny Eichler, Hao Wu, Federico Claudi, Gary Kane and Jonny Saunders as well as the [contributors](https://github.com/DeepLabCut/DeepLabCut/graphs/contributors). Please see [AUTHORS](https://github.com/DeepLabCut/DeepLabCut/blob/master/AUTHORS) for more details!
 
 This is an actively developed package and we welcome community development and involvement.
 
 ## Be part of the DLC Community✨:
 
 | 🚉 Platform                                                 | 🎯 Goal                                                                      | ⏱️ Estimated Response Time | 📢 Support Squad                        |
 |------------------------------------------------------------|-----------------------------------------------------------------------------|---------------------------|----------------------------------------|
@@ -95,20 +97,21 @@
 | 🚧 GitHub DeepLabCut/[Roadmap](https://github.com/DeepLabCut/DeepLabCut/blob/master/docs/roadmap.md)                             | To learn more about our journey✈️                                            | N/A                       | N/A                                    |
 | [![Twitter Follow](https://img.shields.io/twitter/follow/DeepLabCut.svg?label=DeepLabCut&style=social)](https://twitter.com/DeepLabCut)                                                   | To keep up with our latest news and updates 📢                               | Daily                     | DLC Team                               |
 | The DeepLabCut [AI Residency Program](https://www.deeplabcutairesidency.org/)                        | To come and work with us next summer👏                                       | Annually                  | DLC Team                               |
 
 
 ## References:
 
-If you use this code or data we kindly as that you please [cite Mathis et al, 2018](https://www.nature.com/articles/s41593-018-0209-y) and, if you use the Python package (DeepLabCut2.x) please also cite [Nath, Mathis et al, 2019](https://doi.org/10.1038/s41596-019-0176-0). If you utilize the MobileNetV2s or EfficientNets please cite [Mathis, Biasi et al. 2021](https://openaccess.thecvf.com/content/WACV2021/papers/Mathis_Pretraining_Boosts_Out-of-Domain_Robustness_for_Pose_Estimation_WACV_2021_paper.pdf). If you use multi-animal in beta mode, please contact us; if you use the 2.2rc1+, please cite [Lauer et al. 2021](https://www.biorxiv.org/content/10.1101/2021.04.30.442096v1).
+If you use this code or data we kindly as that you please [cite Mathis et al, 2018](https://www.nature.com/articles/s41593-018-0209-y) and, if you use the Python package (DeepLabCut2.x) please also cite [Nath, Mathis et al, 2019](https://doi.org/10.1038/s41596-019-0176-0). If you utilize the MobileNetV2s or EfficientNets please cite [Mathis, Biasi et al. 2021](https://openaccess.thecvf.com/content/WACV2021/papers/Mathis_Pretraining_Boosts_Out-of-Domain_Robustness_for_Pose_Estimation_WACV_2021_paper.pdf). If you use versions 2.2beta+ or 2.2rc1+, please cite [Lauer et al. 2022](https://www.nature.com/articles/s41592-022-01443-0).
 
 DOIs (#ProTip, for helping you find citations for software, check out [CiteAs.org](http://citeas.org/)!):
 
 - Mathis et al 2018: [10.1038/s41593-018-0209-y](https://doi.org/10.1038/s41593-018-0209-y)
 - Nath, Mathis et al 2019: [10.1038/s41596-019-0176-0](https://doi.org/10.1038/s41596-019-0176-0)
+- Lauer et al 2022: [10.1038/s41592-022-01443-0](https://doi.org/10.1038/s41592-022-01443-0)
 
 
 Please check out the following references for more details:
 
     @article{Mathisetal2018,
         title = {DeepLabCut: markerless pose estimation of user-defined body parts with deep learning},
         author = {Alexander Mathis and Pranav Mamidanna and Kevin M. Cury and Taiga Abe  and Venkatesh N. Murthy and Mackenzie W. Mathis and Matthias Bethge},
@@ -141,15 +144,15 @@
 
     @article{insafutdinov2016eccv,
         title = {DeeperCut: A Deeper, Stronger, and Faster Multi-Person Pose Estimation Model},
         author = {Eldar Insafutdinov and Leonid Pishchulin and Bjoern Andres and Mykhaylo Andriluka and Bernt Schiele},
         booktitle = {ECCV'16},
         url = {http://arxiv.org/abs/1605.03170}}
         
-Review articles:
+Review & Educational articles:
 
     @article{Mathis2020DeepLT,
         title={Deep learning tools for the measurement of animal behavior in neuroscience},
         author={Mackenzie W. Mathis and Alexander Mathis},
         journal={Current Opinion in Neurobiology},
         year={2020},
         volume={60},
@@ -173,27 +176,29 @@
         publisher = {Cold Spring Harbor Laboratory},
         URL = {https://www.biorxiv.org/content/early/2018/10/30/457242},
         eprint = {https://www.biorxiv.org/content/early/2018/10/30/457242.full.pdf},
         journal = {bioRxiv}}
 
 ## License:
 
-This project is licensed under the GNU Lesser General Public License v3.0. Note that the software is provided "as is", without warranty of any kind, express or implied. If you use the code or data, please cite us! Note, artwork (DeepLabCut logo) and images are copyrighted; please do not take or use these images without written permission.
+This project is primarily licensed under the GNU Lesser General Public License v3.0. Note that the software is provided "as is", without warranty of any kind, express or implied. If you use the code or data, please cite us! Note, artwork (DeepLabCut logo) and images are copyrighted; please do not take or use these images without written permission.
 
 ## Versions:
 
-VERSION 2.2: Multi-animal pose estimation and tracking with DeepLabCut is supported (as well as single-animal projects).
+VERSION 2.2: Multi-animal pose estimation, identification, and tracking with DeepLabCut is supported (as well as single-animal projects).
 
-VERSION 2.0-2.1: This is the **Python package** of [DeepLabCut](https://www.nature.com/articles/s41593-018-0209-y) that was originally released with our [Nature Protocols](https://doi.org/10.1038/s41596-019-0176-0) paper (preprint [here](https://www.biorxiv.org/content/10.1101/476531v1)).
+VERSION 2.0-2.1: This is the **Python package** of [DeepLabCut](https://www.nature.com/articles/s41593-018-0209-y) that was originally released in Oct 2018 with our [Nature Protocols](https://doi.org/10.1038/s41596-019-0176-0) paper (preprint [here](https://www.biorxiv.org/content/10.1101/476531v1)).
 This package includes graphical user interfaces to label your data, and take you from data set creation to automatic behavioral analysis. It also introduces an active learning framework to efficiently use DeepLabCut on large experimental projects, and data augmentation tools that improve network performance, especially in challenging cases (see [panel b](https://camo.githubusercontent.com/77c92f6b89d44ca758d815bdd7e801247437060b/68747470733a2f2f737461746963312e73717561726573706163652e636f6d2f7374617469632f3537663664353163396637343536366635356563663237312f742f3563336663316336373538643436393530636537656563372f313534373638323338333539352f636865657461682e706e673f666f726d61743d37353077)).
 
 VERSION 1.0: The initial, Nature Neuroscience version of [DeepLabCut](https://www.nature.com/articles/s41593-018-0209-y) can be found in the history of git, or here: https://github.com/DeepLabCut/DeepLabCut/releases/tag/1.11
 
 ## News (and in the news):
 
+- August 2022: DeepLabCut hit 400,000 downloads!
+
 - August 2021: 2.2 becomes the new stable release for DeepLabCut.
 
 - July 2021: Docs are now at https://deeplabcut.github.io/DeepLabCut and we now include TensorFlow 2 support!
 
 - May 2021: DeepLabCut hit 200,000 downloads! Also, Our preprint on 2.2, multi-animal DeepLabCut is released!
 
 - Jan 2021: [Pretraining boosts out-of-domain robustness for pose estimation](https://openaccess.thecvf.com/content/WACV2021/html/Mathis_Pretraining_Boosts_Out-of-Domain_Robustness_for_Pose_Estimation_WACV_2021_paper.html) published in the IEEE Winter Conference on Applications of Computer Vision. We also added EfficientNet backbones to DeepLabCut, those are best trained with cosine decay (see paper). To use them, just pass "`efficientnet-b0`" to "`efficientnet-b6`" when creating the trainingset!
```

#### html2text {}

```diff
@@ -42,38 +42,39 @@
      triMouseDLC.gif?format=300w] [https://static1.squarespace.com/static/
     57f6d51c9f74566f55ecf271/t/5c3fbd0c898583417a040dfc/1547681053201/rat-
                             grasp.gif?format=300w]
 DeepLabCut is a toolbox for markerless pose estimation of animals performing
 various tasks. [Read a short development and application summary below](https:/
 /github.com/DeepLabCut/DeepLabCut#why-use-deeplabcut). As long as you can see
 (label) what you want to track, you can use this toolbox, as it is animal and
-object agnostic. **Latest updates:** :purple_heart: **DeepLabCut supports
-multi-animal pose estimation!** maDLC is out of beta/rc mode and beta is
-deprecated, thanks to the testers out there for feedback! Your labeled data
-will be backwards compatible, but not all other steps. Please see the [new
-`2.2+` releases](https://github.com/DeepLabCut/DeepLabCut/releases) for what's
-new & how to install it, please see our new [paper, Lauer et al 2022](https://
+object agnostic. **Quick start** read the docs: https://deeplabcut.github.io/
+DeepLabCut **Latest updates:** :purple_heart: **DeepLabCut supports multi-
+animal pose estimation!** maDLC is out of beta/rc mode and beta is deprecated,
+thanks to the testers out there for feedback! Your labeled data will be
+backwards compatible, but not all other steps. Please see the [new `2.2+`
+releases](https://github.com/DeepLabCut/DeepLabCut/releases) for what's new &
+how to install it, please see our new [paper, Lauer et al 2022](https://
 www.nature.com/articles/s41592-022-01443-0), and the [new docs]( https://
 deeplabcut.github.io/DeepLabCut) on how to use it! :purple_heart: We support
 multi-animal re-identification, see [Lauer et al 2022](https://www.nature.com/
 articles/s41592-022-01443-0). :purple_heart: We have a **real-time** package
 available! http://DLClive.deeplabcut.org # [Installation: how to install
 DeepLabCut](https://deeplabcut.github.io/DeepLabCut/docs/installation.html)
-Very quick start: `pip install "deeplabcut[gui]"` that includes all GUI
-functions, or `pip install deeplabcut` (headless version). * We recommend using
-our conda file, see [here](https://github.com/DeepLabCut/DeepLabCut/blob/
-master/conda-environments/README.md) or the new [`deeplabcut-docker` package]
-(https://github.com/DeepLabCut/DeepLabCut/tree/master/docker). #
-[Documentation: The DeepLabCut Process](https://deeplabcut.github.io/
-DeepLabCut) Our docs walk you through using DeepLabCut, and key API points. For
-an overview of the toolbox and workflow for project management, see our step-
-by-step at [Nature Protocols paper](https://doi.org/10.1038/s41596-019-0176-0).
-For a deeper understanding and more resources for you to get started with
-Python and DeepLabCut, please check out our free online course! http://
-DLCcourse.deeplabcut.org
+Very quick start: `pip install "deeplabcut[gui,tf]"` that includes all
+functions plus GUIs, or `pip install deeplabcut[tf]` (headless version with
+PyTorch and TensorFlow). * We recommend using our conda file, see [here](https:
+//github.com/DeepLabCut/DeepLabCut/blob/master/conda-environments/README.md) or
+the new [`deeplabcut-docker` package](https://github.com/DeepLabCut/DeepLabCut/
+tree/master/docker). # [Documentation: The DeepLabCut Process](https://
+deeplabcut.github.io/DeepLabCut) Our docs walk you through using DeepLabCut,
+and key API points. For an overview of the toolbox and workflow for project
+management, see our step-by-step at [Nature Protocols paper](https://doi.org/
+10.1038/s41596-019-0176-0). For a deeper understanding and more resources for
+you to get started with Python and DeepLabCut, please check out our free online
+course! http://DLCcourse.deeplabcut.org
    [https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/
                       1609244903687-US1SN063QIFJS4BP4IJD/
 ke17ZwdGBToddI8pDm48kFG9xAYub2PPnmh56PTVg7gUqsxRUqqbr1mOJYKfIPR7LoDQ9mXPOjoJoqy81S2I8N_N4V1vUb5AoIIIbLZhVYxCRW4BPu10St3TBAUQYVKcAju5e7u9RZJEVbVQPZRu9xb_m-
                     kUO2M3I1IeDqD4l8YcGqu2nZPx1UhKV8wc1ELN/
                   dlc_overview_whitebkgrnd.png?format=2500w]
 # [DEMO the code](/examples) We provide data and several Jupyter Notebooks: one
 that walks you through a demo dataset to test your installation, and another
@@ -92,19 +93,18 @@
 (ResNets + readout layers) of one of the state-of-the-art algorithms for human
 pose estimation by Insafutdinov et al., called DeeperCut, which inspired the
 name for our toolbox (see references below). Since this time, the package has
 changed substantially. The code has been re-tooled and re-factored since 2.1+:
 We have added faster and higher performance variants with MobileNetV2s,
 EfficientNets, and our own DLCRNet backbones (see [Pretraining boosts out-of-
 domain robustness for pose estimation](https://arxiv.org/abs/1909.11229) and
-[Lauer et al 2021](https://www.biorxiv.org/content/10.1101/
-2021.04.30.442096v1)). Additionally, we have improved the inference speed and
-provided both additional and novel augmentation methods, added real-time, and
-multi-animal support. We currently provide state-of-the-art performance for
-animal pose estimation.
+[Lauer et al 2022](https://www.nature.com/articles/s41592-022-01443-0)).
+Additionally, we have improved the inference speed and provided both additional
+and novel augmentation methods, added real-time, and multi-animal support. We
+currently provide state-of-the-art performance for animal pose estimation.
       [https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/
 5c3e47258a922d548c483247/1547585339819/ErrorvsTrainingsetSize.png?format=750w]
       [https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/
 5c3e469d8a922d548c4828fa/1547585194560/compressionrobustness.png?format=750w]
       [https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/
 5c3fbed74fa51acecd63deeb/1547681534736/MouseLocomotion_warren.gif?format=500w]
       [https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/
@@ -128,28 +128,28 @@
                 ke17ZwdGBToddI8pDm48kIX24IsDPzy6M4KUaihfICJZw-
             zPPgdn4jUwVcJE1ZvWQUxwkmyExglNqGp0IvTJZamWLI2zvYWH8K3-
    s_4yszcp2ryTI0HqTOaaUohrI8PIxtGUdkzp028KVNnpOijF3PweOM5su6FUQHO6Wkh72Nw/
                            dlc_eco.gif?format=1000w]
 ## Code contributors: DLC code was originally developed by [Alexander Mathis]
 (https://github.com/AlexEMG) & [Mackenzie Mathis](https://github.com/
 MMathisLab), and was extended in 2.0 with [Tanmay Nath](http://
-www.mousemotorlab.org/team), and currently (2.1+) actively developed with our
-CZI DLC Fellow, [Jessy Lauer](https://github.com/jeylau). DeepLabCut is an
-open-source tool and has benefited from suggestions and edits by many
-individuals including Mert Yuksekgonul, Tom Biasi, Richard Warren, Ronny
-Eichler, Hao Wu, Federico Claudi, Gary Kane and Jonny Saunders as well as the
-[contributors](https://github.com/DeepLabCut/DeepLabCut/graphs/contributors).
-Please see [AUTHORS](https://github.com/DeepLabCut/DeepLabCut/blob/master/
-AUTHORS) for more details! This is an actively developed package and we welcome
-community development and involvement. ## Be part of the DLC Communityâ¨: |
-ð Platform | ð¯ Goal | â±ï¸ Estimated Response Time | ð¢ Support Squad
-| |------------------------------------------------------------|---------------
---------------------------------------------------------------|----------------
------------|----------------------------------------| | [![Image.sc forum]
-(https://img.shields.io/badge/dynamic/
+www.mousemotorlab.org/team), and currently (2.1+) actively developed with
+[Jessy Lauer](https://github.com/jeylau). DeepLabCut is an open-source tool and
+has benefited from suggestions and edits by many individuals including Mert
+Yuksekgonul, Tom Biasi, Richard Warren, Ronny Eichler, Hao Wu, Federico Claudi,
+Gary Kane and Jonny Saunders as well as the [contributors](https://github.com/
+DeepLabCut/DeepLabCut/graphs/contributors). Please see [AUTHORS](https://
+github.com/DeepLabCut/DeepLabCut/blob/master/AUTHORS) for more details! This is
+an actively developed package and we welcome community development and
+involvement. ## Be part of the DLC Communityâ¨: | ð Platform | ð¯ Goal |
+â±ï¸ Estimated Response Time | ð¢ Support Squad | |------------------------
+------------------------------------|------------------------------------------
+-----------------------------------|---------------------------|---------------
+-------------------------| | [![Image.sc forum](https://img.shields.io/badge/
+dynamic/
 json.svg?label=forum&url=https%3A%2F%2Fforum.image.sc%2Ftag%2Fdeeplabcut.json&query=%24.topic_list.tags.0.topic_count&colorB=brightgreen&&suffix=%20topics&logo=data:
 image/
 png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+/
 /
 17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/
 cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://
 forum.image.sc/tag/deeplabcut)
@@ -172,88 +172,88 @@
 come and work with us next summerð | Annually | DLC Team | ## References: If
 you use this code or data we kindly as that you please [cite Mathis et al,
 2018](https://www.nature.com/articles/s41593-018-0209-y) and, if you use the
 Python package (DeepLabCut2.x) please also cite [Nath, Mathis et al, 2019]
 (https://doi.org/10.1038/s41596-019-0176-0). If you utilize the MobileNetV2s or
 EfficientNets please cite [Mathis, Biasi et al. 2021](https://
 openaccess.thecvf.com/content/WACV2021/papers/Mathis_Pretraining_Boosts_Out-of-
-Domain_Robustness_for_Pose_Estimation_WACV_2021_paper.pdf). If you use multi-
-animal in beta mode, please contact us; if you use the 2.2rc1+, please cite
-[Lauer et al. 2021](https://www.biorxiv.org/content/10.1101/
-2021.04.30.442096v1). DOIs (#ProTip, for helping you find citations for
+Domain_Robustness_for_Pose_Estimation_WACV_2021_paper.pdf). If you use versions
+2.2beta+ or 2.2rc1+, please cite [Lauer et al. 2022](https://www.nature.com/
+articles/s41592-022-01443-0). DOIs (#ProTip, for helping you find citations for
 software, check out [CiteAs.org](http://citeas.org/)!): - Mathis et al 2018:
 [10.1038/s41593-018-0209-y](https://doi.org/10.1038/s41593-018-0209-y) - Nath,
 Mathis et al 2019: [10.1038/s41596-019-0176-0](https://doi.org/10.1038/s41596-
-019-0176-0) Please check out the following references for more details:
-@article{Mathisetal2018, title = {DeepLabCut: markerless pose estimation of
-user-defined body parts with deep learning}, author = {Alexander Mathis and
-Pranav Mamidanna and Kevin M. Cury and Taiga Abe and Venkatesh N. Murthy and
-Mackenzie W. Mathis and Matthias Bethge}, journal = {Nature Neuroscience}, year
-= {2018}, url = {https://www.nature.com/articles/s41593-018-0209-y}} @article
-{NathMathisetal2019, title = {Using DeepLabCut for 3D markerless pose
-estimation across species and behaviors}, author = {Nath*, Tanmay and Mathis*,
-Alexander and Chen, An Chi and Patel, Amir and Bethge, Matthias and Mathis,
-Mackenzie W}, journal = {Nature Protocols}, year = {2019}, url = {https://
-doi.org/10.1038/s41596-019-0176-0}} @InProceedings{Mathis_2021_WACV, author =
-{Mathis, Alexander and Biasi, Thomas and Schneider, Steffen and Yuksekgonul,
-Mert and Rogers, Byron and Bethge, Matthias and Mathis, Mackenzie W.}, title =
-{Pretraining Boosts Out-of-Domain Robustness for Pose Estimation}, booktitle =
-{Proceedings of the IEEE/CVF Winter Conference on Applications of Computer
-Vision (WACV)}, month = {January}, year = {2021}, pages = {1859-1868}} @article
-{Lauer2022MultianimalPE, title={Multi-animal pose estimation, identification
-and tracking with DeepLabCut}, author={Jessy Lauer and Mu Zhou and Shaokai Ye
-and William Menegas and Steffen Schneider and Tanmay Nath and Mohammed
-Mostafizur Rahman and Valentina Di Santo and Daniel Soberanes and Guoping Feng
-and Venkatesh N. Murthy and George Lauder and Catherine Dulac and M. Mathis and
-Alexander Mathis}, journal={Nature Methods}, year={2022}, volume={19}, pages=
-{496 - 504}} @article{insafutdinov2016eccv, title = {DeeperCut: A Deeper,
-Stronger, and Faster Multi-Person Pose Estimation Model}, author = {Eldar
-Insafutdinov and Leonid Pishchulin and Bjoern Andres and Mykhaylo Andriluka and
-Bernt Schiele}, booktitle = {ECCV'16}, url = {http://arxiv.org/abs/1605.03170}}
-Review articles: @article{Mathis2020DeepLT, title={Deep learning tools for the
-measurement of animal behavior in neuroscience}, author={Mackenzie W. Mathis
-and Alexander Mathis}, journal={Current Opinion in Neurobiology}, year={2020},
-volume={60}, pages={1-11}} @article{Mathis2020Primer, title={A Primer on Motion
-Capture with Deep Learning: Principles, Pitfalls, and Perspectives}, author=
-{Alexander Mathis and Steffen Schneider and Jessy Lauer and Mackenzie W.
-Mathis}, journal={Neuron}, year={2020}, volume={108}, pages={44-65}} Other
-open-access pre-prints related to our work on DeepLabCut: @article
-{MathisWarren2018speed, author = {Mathis, Alexander and Warren, Richard A.},
-title = {On the inference speed and video-compression robustness of
-DeepLabCut}, year = {2018}, doi = {10.1101/457242}, publisher = {Cold Spring
-Harbor Laboratory}, URL = {https://www.biorxiv.org/content/early/2018/10/30/
-457242}, eprint = {https://www.biorxiv.org/content/early/2018/10/30/
-457242.full.pdf}, journal = {bioRxiv}} ## License: This project is licensed
-under the GNU Lesser General Public License v3.0. Note that the software is
-provided "as is", without warranty of any kind, express or implied. If you use
-the code or data, please cite us! Note, artwork (DeepLabCut logo) and images
-are copyrighted; please do not take or use these images without written
-permission. ## Versions: VERSION 2.2: Multi-animal pose estimation and tracking
-with DeepLabCut is supported (as well as single-animal projects). VERSION 2.0-
-2.1: This is the **Python package** of [DeepLabCut](https://www.nature.com/
-articles/s41593-018-0209-y) that was originally released with our [Nature
-Protocols](https://doi.org/10.1038/s41596-019-0176-0) paper (preprint [here]
-(https://www.biorxiv.org/content/10.1101/476531v1)). This package includes
-graphical user interfaces to label your data, and take you from data set
-creation to automatic behavioral analysis. It also introduces an active
-learning framework to efficiently use DeepLabCut on large experimental
-projects, and data augmentation tools that improve network performance,
-especially in challenging cases (see [panel b](https://
-camo.githubusercontent.com/77c92f6b89d44ca758d815bdd7e801247437060b/
+019-0176-0) - Lauer et al 2022: [10.1038/s41592-022-01443-0](https://doi.org/
+10.1038/s41592-022-01443-0) Please check out the following references for more
+details: @article{Mathisetal2018, title = {DeepLabCut: markerless pose
+estimation of user-defined body parts with deep learning}, author = {Alexander
+Mathis and Pranav Mamidanna and Kevin M. Cury and Taiga Abe and Venkatesh N.
+Murthy and Mackenzie W. Mathis and Matthias Bethge}, journal = {Nature
+Neuroscience}, year = {2018}, url = {https://www.nature.com/articles/s41593-
+018-0209-y}} @article{NathMathisetal2019, title = {Using DeepLabCut for 3D
+markerless pose estimation across species and behaviors}, author = {Nath*,
+Tanmay and Mathis*, Alexander and Chen, An Chi and Patel, Amir and Bethge,
+Matthias and Mathis, Mackenzie W}, journal = {Nature Protocols}, year = {2019},
+url = {https://doi.org/10.1038/s41596-019-0176-0}} @InProceedings
+{Mathis_2021_WACV, author = {Mathis, Alexander and Biasi, Thomas and Schneider,
+Steffen and Yuksekgonul, Mert and Rogers, Byron and Bethge, Matthias and
+Mathis, Mackenzie W.}, title = {Pretraining Boosts Out-of-Domain Robustness for
+Pose Estimation}, booktitle = {Proceedings of the IEEE/CVF Winter Conference on
+Applications of Computer Vision (WACV)}, month = {January}, year = {2021},
+pages = {1859-1868}} @article{Lauer2022MultianimalPE, title={Multi-animal pose
+estimation, identification and tracking with DeepLabCut}, author={Jessy Lauer
+and Mu Zhou and Shaokai Ye and William Menegas and Steffen Schneider and Tanmay
+Nath and Mohammed Mostafizur Rahman and Valentina Di Santo and Daniel Soberanes
+and Guoping Feng and Venkatesh N. Murthy and George Lauder and Catherine Dulac
+and M. Mathis and Alexander Mathis}, journal={Nature Methods}, year={2022},
+volume={19}, pages={496 - 504}} @article{insafutdinov2016eccv, title =
+{DeeperCut: A Deeper, Stronger, and Faster Multi-Person Pose Estimation Model},
+author = {Eldar Insafutdinov and Leonid Pishchulin and Bjoern Andres and
+Mykhaylo Andriluka and Bernt Schiele}, booktitle = {ECCV'16}, url = {http://
+arxiv.org/abs/1605.03170}} Review & Educational articles: @article
+{Mathis2020DeepLT, title={Deep learning tools for the measurement of animal
+behavior in neuroscience}, author={Mackenzie W. Mathis and Alexander Mathis},
+journal={Current Opinion in Neurobiology}, year={2020}, volume={60}, pages={1-
+11}} @article{Mathis2020Primer, title={A Primer on Motion Capture with Deep
+Learning: Principles, Pitfalls, and Perspectives}, author={Alexander Mathis and
+Steffen Schneider and Jessy Lauer and Mackenzie W. Mathis}, journal={Neuron},
+year={2020}, volume={108}, pages={44-65}} Other open-access pre-prints related
+to our work on DeepLabCut: @article{MathisWarren2018speed, author = {Mathis,
+Alexander and Warren, Richard A.}, title = {On the inference speed and video-
+compression robustness of DeepLabCut}, year = {2018}, doi = {10.1101/457242},
+publisher = {Cold Spring Harbor Laboratory}, URL = {https://www.biorxiv.org/
+content/early/2018/10/30/457242}, eprint = {https://www.biorxiv.org/content/
+early/2018/10/30/457242.full.pdf}, journal = {bioRxiv}} ## License: This
+project is primarily licensed under the GNU Lesser General Public License v3.0.
+Note that the software is provided "as is", without warranty of any kind,
+express or implied. If you use the code or data, please cite us! Note, artwork
+(DeepLabCut logo) and images are copyrighted; please do not take or use these
+images without written permission. ## Versions: VERSION 2.2: Multi-animal pose
+estimation, identification, and tracking with DeepLabCut is supported (as well
+as single-animal projects). VERSION 2.0-2.1: This is the **Python package** of
+[DeepLabCut](https://www.nature.com/articles/s41593-018-0209-y) that was
+originally released in Oct 2018 with our [Nature Protocols](https://doi.org/
+10.1038/s41596-019-0176-0) paper (preprint [here](https://www.biorxiv.org/
+content/10.1101/476531v1)). This package includes graphical user interfaces to
+label your data, and take you from data set creation to automatic behavioral
+analysis. It also introduces an active learning framework to efficiently use
+DeepLabCut on large experimental projects, and data augmentation tools that
+improve network performance, especially in challenging cases (see [panel b]
+(https://camo.githubusercontent.com/77c92f6b89d44ca758d815bdd7e801247437060b/
 68747470733a2f2f737461746963312e73717561726573706163652e636f6d2f7374617469632f3537663664353163396637343536366635356563663237312f742f3563336663316336373538643436393530636537656563372f313534373638323338333539352f636865657461682e706e673f666f726d61743d37353077)).
 VERSION 1.0: The initial, Nature Neuroscience version of [DeepLabCut](https://
 www.nature.com/articles/s41593-018-0209-y) can be found in the history of git,
 or here: https://github.com/DeepLabCut/DeepLabCut/releases/tag/1.11 ## News
-(and in the news): - August 2021: 2.2 becomes the new stable release for
-DeepLabCut. - July 2021: Docs are now at https://deeplabcut.github.io/
-DeepLabCut and we now include TensorFlow 2 support! - May 2021: DeepLabCut hit
-200,000 downloads! Also, Our preprint on 2.2, multi-animal DeepLabCut is
-released! - Jan 2021: [Pretraining boosts out-of-domain robustness for pose
-estimation](https://openaccess.thecvf.com/content/WACV2021/html/
-Mathis_Pretraining_Boosts_Out-of-
+(and in the news): - August 2022: DeepLabCut hit 400,000 downloads! - August
+2021: 2.2 becomes the new stable release for DeepLabCut. - July 2021: Docs are
+now at https://deeplabcut.github.io/DeepLabCut and we now include TensorFlow 2
+support! - May 2021: DeepLabCut hit 200,000 downloads! Also, Our preprint on
+2.2, multi-animal DeepLabCut is released! - Jan 2021: [Pretraining boosts out-
+of-domain robustness for pose estimation](https://openaccess.thecvf.com/
+content/WACV2021/html/Mathis_Pretraining_Boosts_Out-of-
 Domain_Robustness_for_Pose_Estimation_WACV_2021_paper.html) published in the
 IEEE Winter Conference on Applications of Computer Vision. We also added
 EfficientNet backbones to DeepLabCut, those are best trained with cosine decay
 (see paper). To use them, just pass "`efficientnet-b0`" to "`efficientnet-b6`"
 when creating the trainingset! - Dec 2020: We released a real-time package that
 allows for online pose estimation and real-time feedback. See
 [DLClive.deeplabcut.org](http://DLClive.deeplabcut.org). - 5/22 2020: We
```

### Comparing `deeplabcut-2.3rc2/deeplabcut/__init__.py` & `deeplabcut-2.3rc3/deeplabcut/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/__main__.py` & `deeplabcut-2.3rc3/deeplabcut/__main__.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/benchmark/__init__.py` & `deeplabcut-2.3rc3/deeplabcut/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/benchmark/base.py` & `deeplabcut-2.3rc3/deeplabcut/benchmark/base.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/benchmark/benchmarks.py` & `deeplabcut-2.3rc3/deeplabcut/benchmark/benchmarks.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/benchmark/cli.py` & `deeplabcut-2.3rc3/deeplabcut/benchmark/cli.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/benchmark/metrics.py` & `deeplabcut-2.3rc3/deeplabcut/benchmark/metrics.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/benchmark/utils.py` & `deeplabcut-2.3rc3/deeplabcut/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/cli.py` & `deeplabcut-2.3rc3/deeplabcut/cli.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/create_project/add.py` & `deeplabcut-2.3rc3/deeplabcut/create_project/add.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/create_project/demo_data.py` & `deeplabcut-2.3rc3/deeplabcut/create_project/demo_data.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/create_project/modelzoo.py` & `deeplabcut-2.3rc3/deeplabcut/create_project/modelzoo.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,32 @@
 import yaml
 
 import deeplabcut
 from deeplabcut.utils import auxiliaryfunctions, auxfun_models
 
 Modeloptions = [
     "full_human",
+    "primate_face",
+    "mouse_pupil_vclose",
+    "horse_sideview",
+    "full_macaque",
+]  # just expand this list with new projects
+
+'''
+Modeloptions = [
+    "full_human",
     "full_cat",
     "full_dog",
     "primate_face",
     "mouse_pupil_vclose",
     "horse_sideview",
     "full_macaque",
     "full_cheetah",
 ]  # just expand this list with new projects
-
+'''
 
 def MakeTrain_pose_yaml(itemstochange, saveasconfigfile, defaultconfigfile):
     raw = open(defaultconfigfile).read()
     docs = []
     for raw_doc in raw.split("\n---"):
         try:
             docs.append(yaml.load(raw_doc, Loader=yaml.SafeLoader))
@@ -69,26 +78,26 @@
     working_directory=None,
     copy_videos=False,
     videotype="",
     createlabeledvideo=True,
     analyzevideo=True,
 ):
     """
-    LEGACY FUNCTION will be deprecated.
+    LEGACY FUNCTION will be deprecated in v2.3.
 
     Use deeplabcut.create_pretrained_project(project, experimenter, videos, model='full_human', ..)
 
     For now just calls that function....
 
     Creates a demo human project and analyzes a video with ResNet 101 weights pretrained on
     MPII Human Pose. This is from the DeeperCut paper by Insafutdinov et al. https://arxiv.org/abs/1605.03170
     Please make sure to cite it too if you use this code!
     """
     print(
-        "LEGACY FUNCTION will be deprecated.... use  deeplabcut.create_pretrained_project(project, experimenter, videos, model='full_human', ..) in the future!"
+        "LEGACY FUNCTION will be deprecated in v2.3.... use  deeplabcut.create_pretrained_project(project, experimenter, videos, model='full_human', ..) in the future!"
     )
     create_pretrained_project(
         project,
         experimenter,
         videos,
         model="full_human",
         working_directory=working_directory,
@@ -258,15 +267,19 @@
             os.path.join(
                 config["project_path"], Path(modelfoldername), "test", "pose_cfg.yaml"
             )
         )
 
         # Download the weights and put then in appropriate directory
         print("Downloading weights...")
-        auxfun_models.download_model(model, train_dir)
+
+        # AM: Rowland server down...
+        #auxfun_models.download_model(model, train_dir)
+        auxfun_models.download_hugginface_model(model, train_dir)
+
 
         pose_cfg = deeplabcut.auxiliaryfunctions.read_plainconfig(path_train_config)
         print(path_train_config)
         # Updating config file:
         dict_ = {
             "default_net_type": pose_cfg["net_type"],
             "default_augmenter": pose_cfg["dataset_type"],
```

### Comparing `deeplabcut-2.3rc2/deeplabcut/create_project/new.py` & `deeplabcut-2.3rc3/deeplabcut/create_project/new.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/create_project/new_3d.py` & `deeplabcut-2.3rc3/deeplabcut/create_project/new_3d.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/generate_training_dataset/frame_extraction.py` & `deeplabcut-2.3rc3/deeplabcut/generate_training_dataset/frame_extraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,17 +286,17 @@
             raise Exception(
                 "Perhaps consider extracting more, or a natural number of frames."
             )
         if videos_list is None:
             videos = cfg.get("video_sets_original") or cfg["video_sets"]
         else: #filter video_list by the ones in the config file
             videos = [v for v in cfg["video_sets"] if v in videos_list]
-            
+
         if opencv:
-            from deeplabcut.utils.auxfun_videos import VideoReader
+            from deeplabcut.utils.auxfun_videos import VideoWriter
         else:
             from moviepy.editor import VideoFileClip
 
         has_failed = []
         for video in videos:
             if userfeedback:
                 print(
@@ -314,15 +314,15 @@
                 or askuser == "Ja"
                 or askuser == "ha"
                 or askuser == "oui"
                 or askuser == "ouais"
             ):  # multilanguage support :)
 
                 if opencv:
-                    cap = VideoReader(video)
+                    cap = VideoWriter(video)
                     nframes = len(cap)
                 else:
                     # Moviepy:
                     clip = VideoFileClip(video)
                     fps = clip.fps
                     nframes = int(np.ceil(clip.duration * 1.0 / fps))
                 if not nframes:
@@ -351,22 +351,25 @@
                 if crop == "GUI":
                     cfg = select_cropping_area(config, [video])
                 try:
                     coords = cfg["video_sets"][video]["crop"].split(",")
                 except KeyError:
                     coords = cfg["video_sets_original"][video]["crop"].split(",")
 
-                if crop and not opencv:
-                    clip = clip.crop(
-                        y1=int(coords[2]),
-                        y2=int(coords[3]),
-                        x1=int(coords[0]),
-                        x2=int(coords[1]),
-                    )
-                elif not crop:
+                if crop:
+                    if opencv:
+                        cap.set_bbox(*map(int, coords))
+                    else:
+                        clip = clip.crop(
+                            y1=int(coords[2]),
+                            y2=int(coords[3]),
+                            x1=int(coords[0]),
+                            x2=int(coords[1]),
+                        )
+                else:
                     coords = None
 
                 print("Extracting frames based on %s ..." % algo)
                 if algo == "uniform":
                     if opencv:
                         frames2pick = frameselectiontools.UniformFramescv2(
                             cap, numframes2pick, start, stop
@@ -378,16 +381,14 @@
                 elif algo == "kmeans":
                     if opencv:
                         frames2pick = frameselectiontools.KmeansbasedFrameselectioncv2(
                             cap,
                             numframes2pick,
                             start,
                             stop,
-                            crop,
-                            coords,
                             step=cluster_step,
                             resizewidth=cluster_resizewidth,
                             color=cluster_color,
                         )
                     else:
                         frames2pick = frameselectiontools.KmeansbasedFrameselection(
                             clip,
@@ -411,34 +412,24 @@
                 output_path = (
                     Path(config).parents[0] / "labeled-data" / Path(video).stem
                 )
                 is_valid = []
                 if opencv:
                     for index in frames2pick:
                         cap.set_to_frame(index)  # extract a particular frame
-                        frame = cap.read_frame()
+                        frame = cap.read_frame(crop=True)
                         if frame is not None:
                             image = img_as_ubyte(frame)
                             img_name = (
                                 str(output_path)
                                 + "/img"
                                 + str(index).zfill(indexlength)
                                 + ".png"
                             )
-                            if crop:
-                                io.imsave(
-                                    img_name,
-                                    image[
-                                        int(coords[2]) : int(coords[3]),
-                                        int(coords[0]) : int(coords[1]),
-                                        :,
-                                    ],
-                                )  # y1 = int(coords[2]),y2 = int(coords[3]),x1 = int(coords[0]), x2 = int(coords[1]
-                            else:
-                                io.imsave(img_name, image)
+                            io.imsave(img_name, image)
                             is_valid.append(True)
                         else:
                             print("Frame", index, " not found!")
                             is_valid.append(False)
                     cap.close()
                 else:
                     for index in frames2pick:
```

### Comparing `deeplabcut-2.3rc2/deeplabcut/generate_training_dataset/multiple_individuals_trainingsetmanipulation.py` & `deeplabcut-2.3rc3/deeplabcut/generate_training_dataset/multiple_individuals_trainingsetmanipulation.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/generate_training_dataset/trainingsetmanipulation.py` & `deeplabcut-2.3rc3/deeplabcut/generate_training_dataset/trainingsetmanipulation.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/assets/icons/help.png` & `deeplabcut-2.3rc3/deeplabcut/gui/assets/icons/help.png`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/assets/icons/help2.png` & `deeplabcut-2.3rc3/deeplabcut/gui/assets/icons/help2.png`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/assets/icons/new_project.png` & `deeplabcut-2.3rc3/deeplabcut/gui/assets/icons/new_project.png`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/assets/icons/new_project2.png` & `deeplabcut-2.3rc3/deeplabcut/gui/assets/icons/new_project2.png`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/assets/icons/open.png` & `deeplabcut-2.3rc3/deeplabcut/gui/assets/icons/open.png`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/assets/icons/open2.png` & `deeplabcut-2.3rc3/deeplabcut/gui/assets/icons/open2.png`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/assets/logo.png` & `deeplabcut-2.3rc3/deeplabcut/gui/assets/logo.png`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/assets/logo_transparent.png` & `deeplabcut-2.3rc3/deeplabcut/gui/assets/logo_transparent.png`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/assets/welcome.png` & `deeplabcut-2.3rc3/deeplabcut/gui/assets/welcome.png`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/components.py` & `deeplabcut-2.3rc3/deeplabcut/gui/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             self.selected_videos_text.setText(f"{n_videos} videos selected")
             self.select_video_button.setText("Add more videos")
         else:
             self.selected_videos_text.setText("")
             self.select_video_button.setText("Select videos")
 
     def select_videos(self):
-        cwd = self.root.project_folder()
+        cwd = self.root.project_folder
         filenames = QtWidgets.QFileDialog.getOpenFileNames(
             self,
             "Select video(s) to analyze",
             cwd,
             f"Videos ({' *.'.join(DLCParams.VIDEOTYPES)[1:]})",
         )
```

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/dlc_params.py` & `deeplabcut-2.3rc3/deeplabcut/gui/dlc_params.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/launch_script.py` & `deeplabcut-2.3rc3/deeplabcut/gui/launch_script.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/media/dlc_1-01.png` & `deeplabcut-2.3rc3/deeplabcut/gui/media/dlc_1-01.png`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/media/logo.png` & `deeplabcut-2.3rc3/deeplabcut/gui/media/logo.png`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/tabs/__init__.py` & `deeplabcut-2.3rc3/deeplabcut/gui/tabs/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/tabs/analyze_videos.py` & `deeplabcut-2.3rc3/deeplabcut/gui/tabs/analyze_videos.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/tabs/create_project.py` & `deeplabcut-2.3rc3/deeplabcut/gui/tabs/create_project.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/tabs/create_training_dataset.py` & `deeplabcut-2.3rc3/deeplabcut/gui/tabs/create_training_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/tabs/create_videos.py` & `deeplabcut-2.3rc3/deeplabcut/gui/tabs/create_videos.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/tabs/evaluate_network.py` & `deeplabcut-2.3rc3/deeplabcut/gui/tabs/evaluate_network.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/tabs/extract_frames.py` & `deeplabcut-2.3rc3/deeplabcut/gui/tabs/extract_frames.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/tabs/extract_outlier_frames.py` & `deeplabcut-2.3rc3/deeplabcut/gui/tabs/extract_outlier_frames.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/tabs/label_frames.py` & `deeplabcut-2.3rc3/deeplabcut/gui/tabs/label_frames.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/tabs/manage_project.py` & `deeplabcut-2.3rc3/deeplabcut/gui/tabs/manage_project.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/tabs/open_project.py` & `deeplabcut-2.3rc3/deeplabcut/gui/tabs/open_project.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/tabs/refine_tracklets.py` & `deeplabcut-2.3rc3/deeplabcut/gui/tabs/refine_tracklets.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/tabs/train_network.py` & `deeplabcut-2.3rc3/deeplabcut/gui/tabs/train_network.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/tabs/unsupervised_id_tracking.py` & `deeplabcut-2.3rc3/deeplabcut/gui/tabs/unsupervised_id_tracking.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/tabs/video_editor.py` & `deeplabcut-2.3rc3/deeplabcut/gui/tabs/video_editor.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/tracklet_toolbox.py` & `deeplabcut-2.3rc3/deeplabcut/gui/tracklet_toolbox.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/utils.py` & `deeplabcut-2.3rc3/deeplabcut/gui/utils.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/widgets.py` & `deeplabcut-2.3rc3/deeplabcut/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/gui/window.py` & `deeplabcut-2.3rc3/deeplabcut/gui/window.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         return self._toolbar
 
     @cached_property
     def settings(self):
         return QtCore.QSettings()
 
     def load_settings(self):
-        filenames = self.settings.value("recent_files", [])
+        filenames = self.settings.value("recent_files") or []
         for filename in filenames:
             self.add_recent_filename(filename)
 
     def save_settings(self):
         recent_files = []
         for action in self.recentfiles_menu.actions()[::-1]:
             recent_files.append(action.text())
```

### Comparing `deeplabcut-2.3rc2/deeplabcut/inference_cfg.yaml` & `deeplabcut-2.3rc3/deeplabcut/inference_cfg.yaml`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_cfg.yaml` & `deeplabcut-2.3rc3/deeplabcut/pose_cfg.yaml`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_3d/camera_calibration.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_3d/camera_calibration.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_3d/plotting3D.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_3d/plotting3D.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_3d/triangulation.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_3d/triangulation.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/__init__.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/backbones/efficientnet_builder.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/backbones/efficientnet_builder.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/backbones/efficientnet_model.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/backbones/efficientnet_model.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/backbones/mobilenet.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/backbones/mobilenet.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/backbones/mobilenet_v2.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/config.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/config.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/evaluate.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/evaluate.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/evaluate_multianimal.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/evaluate_multianimal.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/openvino/mo_extensions/front/tf/unravel_index.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/openvino/mo_extensions/front/tf/unravel_index.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/openvino/session.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/openvino/session.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/predict.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/predict.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/predict_multianimal.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/predict_multianimal.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/test.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/test.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/train.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/train.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/core/train_multianimal.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/core/train_multianimal.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/__init__.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/augmentation.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/augmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
             if self.crop_sampling == "hybrid":
                 sampling = random_state.choice(["uniform", "density"])
             if sampling == "uniform":
                 center = random_state.uniform(size=2)
             else:
                 h, w = batch.images[n].shape[:2]
                 kpts = batch.keypoints[n].to_xy_array()
+                kpts = kpts[~np.isnan(kpts).all(axis=1)]
                 n_kpts = kpts.shape[0]
                 inds = np.arange(n_kpts)
                 if sampling == "density":
                     # Points located close to one another are sampled preferentially
                     # in order to augment crowded regions.
                     radius = 0.1 * min(h, w)
                     n_neighbors = self.calc_n_neighbors(kpts, radius)
```

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/factory.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/factory.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/pose_base.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/pose_base.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/pose_deterministic.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/pose_deterministic.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/pose_imgaug.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/pose_imgaug.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/pose_multianimal_imgaug.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/pose_multianimal_imgaug.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/pose_scalecrop.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/pose_scalecrop.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/pose_tensorpack.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/pose_tensorpack.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/datasets/utils.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/default_config.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/default_config.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/export.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/export.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/lib/crossvalutils.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/lib/crossvalutils.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/lib/inferenceutils.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/lib/inferenceutils.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/lib/trackingutils.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/lib/trackingutils.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/__init__.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/base.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/base.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/conv_blocks.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/conv_blocks.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/efficientnet.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/efficientnet.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/factory.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/factory.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/layers.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/layers.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/mobilenet.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/mobilenet.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/multi.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/multi.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/resnet.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/resnet.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/nnets/utils.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/nnets/utils.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/predict_multianimal.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/predict_multianimal.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/predict_videos.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/predict_videos.py`

 * *Files 1% similar despite different names*

```diff
@@ -853,65 +853,57 @@
 
 
 def GetPoseF_GTF(cfg, dlc_cfg, sess, inputs, outputs, cap, nframes, batchsize):
     """Batchwise prediction of pose"""
     PredictedData = np.zeros((nframes, 3 * len(dlc_cfg["all_joints_names"])))
     batch_ind = 0  # keeps track of which image within a batch should be written to
     batch_num = 0  # keeps track of which batch you are at
-    ny, nx = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT)), int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
+    ny = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
+    nx = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
     if cfg["cropping"]:
         ny, nx = checkcropping(cfg, cap)
 
-    pose_tensor = predict.extract_GPUprediction(
-        outputs, dlc_cfg
-    )  # extract_output_tensor(outputs, dlc_cfg)
-    frames = np.empty(
-        (batchsize, ny, nx, 3), dtype="ubyte"
-    )  # this keeps all frames in a batch
+    # Flip x, y, confidence and reshape
+    pose_tensor = predict.extract_GPUprediction(outputs, dlc_cfg)
+    pose_tensor = tf.gather(pose_tensor, [1, 0, 2], axis=1)
+    pose_tensor = tf.reshape(pose_tensor, (batchsize, -1))
+
+    frames = np.empty((batchsize, ny, nx, 3), dtype="ubyte")
     pbar = tqdm(total=nframes)
-    counter = 0
-    step = max(10, int(nframes / 100))
+    counter = -1
     inds = []
-    while cap.isOpened():
-        if counter != 0 and counter % step == 0:
-            pbar.update(step)
+    while cap.isOpened() and counter < nframes - 1:
         ret, frame = cap.read()
-        if ret:
-            frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
-            if cfg["cropping"]:
-                frames[batch_ind] = img_as_ubyte(
-                    frame[cfg["y1"] : cfg["y2"], cfg["x1"] : cfg["x2"]]
-                )
-            else:
-                frames[batch_ind] = img_as_ubyte(frame)
-            inds.append(counter)
-            if batch_ind == batchsize - 1:
-                # pose = predict.getposeNP(frames,dlc_cfg, sess, inputs, outputs)
-                pose = sess.run(pose_tensor, feed_dict={inputs: frames})
-                pose[:, [0, 1, 2]] = pose[
-                    :, [1, 0, 2]
-                ]  # change order to have x,y,confidence
-                pose = np.reshape(
-                    pose, (batchsize, -1)
-                )  # bring into batchsize times x,y,conf etc.
-                PredictedData[inds] = pose
-                batch_ind = 0
-                inds.clear()
-                batch_num += 1
-            else:
-                batch_ind += 1
-        elif counter >= nframes:
-            if batch_ind > 0:
-                # pose = predict.getposeNP(frames, dlc_cfg, sess, inputs, outputs) #process the whole batch (some frames might be from previous batch!)
-                pose = sess.run(pose_tensor, feed_dict={inputs: frames})
-                pose[:, [0, 1, 2]] = pose[:, [1, 0, 2]]
-                pose = np.reshape(pose, (batchsize, -1))
-                PredictedData[inds[:batch_ind]] = pose[:batch_ind]
-            break
         counter += 1
+        if not ret:
+            warnings.warn(f"Could not decode frame #{counter}.")
+            continue
+
+        if cfg["cropping"]:
+            frame = img_as_ubyte(
+                frame[cfg["y1"] : cfg["y2"], cfg["x1"] : cfg["x2"]]
+            )
+        else:
+            frame = img_as_ubyte(frame)
+        frames[batch_ind] = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
+        inds.append(counter)
+        if batch_ind == batchsize - 1:
+            pose = sess.run(pose_tensor, feed_dict={inputs: frames})
+            PredictedData[inds] = pose
+            batch_ind = 0
+            batch_num += 1
+            inds.clear()
+            pbar.update(batchsize)
+        else:
+            batch_ind += 1
+
+    if batch_ind > 0:
+        pose = sess.run(pose_tensor, feed_dict={inputs: frames})
+        PredictedData[inds[:batch_ind]] = pose[:batch_ind]
+        pbar.update(batch_ind)
 
     pbar.close()
     return PredictedData, nframes
 
 
 def getboundingbox(x, y, nx, ny, margin):
     x1 = max([0, int(np.amin(x)) - margin])
```

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/training.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/training.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/util/visualize.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/util/visualize.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/vis_dataset.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/vis_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_estimation_tensorflow/visualizemaps.py` & `deeplabcut-2.3rc3/deeplabcut/pose_estimation_tensorflow/visualizemaps.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/apis.py` & `deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/apis.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/create_dataset.py` & `deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/create_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/datasets/dlc_vec.py` & `deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/datasets/dlc_vec.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/datasets/make_dataloader.py` & `deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/datasets/make_dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/inference.py` & `deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/inference.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/model/backbones/vit_pytorch.py` & `deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/model/backbones/vit_pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/model/make_model.py` & `deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/model/make_model.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/processor/processor.py` & `deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/processor/processor.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/solver/cosine_lr.py` & `deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/solver/cosine_lr.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/solver/make_optimizer.py` & `deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/solver/make_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/solver/scheduler.py` & `deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/solver/scheduler.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/solver/scheduler_factory.py` & `deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/solver/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/tracking_utils/metrics.py` & `deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/tracking_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/tracking_utils/preprocessing.py` & `deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/tracking_utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/tracking_utils/reranking.py` & `deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/tracking_utils/reranking.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/pose_tracking_pytorch/train_dlctransreid.py` & `deeplabcut-2.3rc3/deeplabcut/pose_tracking_pytorch/train_dlctransreid.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/post_processing/analyze_skeleton.py` & `deeplabcut-2.3rc3/deeplabcut/post_processing/analyze_skeleton.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/post_processing/filtering.py` & `deeplabcut-2.3rc3/deeplabcut/post_processing/filtering.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/refine_training_dataset/outlier_frames.py` & `deeplabcut-2.3rc3/deeplabcut/refine_training_dataset/outlier_frames.py`

 * *Files 1% similar despite different names*

```diff
@@ -634,15 +634,17 @@
         from moviepy.editor import VideoFileClip
 
         clip = VideoFileClip(video)
         fps = clip.fps
         duration = clip.duration
 
     if cfg["cropping"]:  # one might want to adjust
-        coords = (cfg["x1"], cfg["x2"], cfg["y1"], cfg["y2"])
+        coords = cfg["video_sets"].get(video, {}).get("crop")
+        if coords is not None:
+            coords = list(map(int, coords.split(", ")))
     else:
         coords = None
 
     print("Duration of video [s]: ", duration, ", recorded @ ", fps, "fps!")
     print("Overall # of frames: ", nframes, "with (cropped) frame dimensions: ")
     if extractionalgorithm == "uniform":
         if opencv:
@@ -651,28 +653,30 @@
             )
         else:
             frames2pick = frameselectiontools.UniformFrames(
                 clip, numframes2extract, start, stop, Index
             )
     elif extractionalgorithm == "kmeans":
         if opencv:
+            if coords is not None:
+                vid.set_bbox(*coords)
             frames2pick = frameselectiontools.KmeansbasedFrameselectioncv2(
                 vid,
                 numframes2extract,
                 start,
                 stop,
-                cfg["cropping"],
-                coords,
                 Index,
                 resizewidth=cluster_resizewidth,
                 color=cluster_color,
             )
         else:
-            if cfg["cropping"]:
-                clip = clip.crop(y1=cfg["y1"], y2=cfg["x2"], x1=cfg["x1"], x2=cfg["x2"])
+            if coords is not None:
+                clip = clip.crop(
+                    y1=coords[2], y2=coords[3], x1=coords[0], x2=coords[1],
+                )
             frames2pick = frameselectiontools.KmeansbasedFrameselection(
                 clip,
                 numframes2extract,
                 start,
                 stop,
                 Index,
                 resizewidth=cluster_resizewidth,
@@ -689,16 +693,14 @@
     print("Let's select frames indices:", frames2pick)
     colors = visualization.get_cmap(len(bodyparts), cfg["colormap"])
     strwidth = int(np.ceil(np.log10(nframes)))  # width for strings
     for index in frames2pick:  ##tqdm(range(0,nframes,10)):
         if opencv:
             PlottingSingleFramecv2(
                 vid,
-                cfg["cropping"],
-                coords,
                 data,
                 bodyparts,
                 tmpfolder,
                 index,
                 cfg["dotsize"],
                 cfg["pcutoff"],
                 cfg["alphavalue"],
@@ -728,15 +730,15 @@
     else:
         clip.close()
         del clip
 
     # Extract annotations based on DeepLabCut and store in the folder (with name derived from video name) under labeled-data
     if len(frames2pick) > 0:
         try:
-            if cfg["cropping"]:
+            if coords is not None:
                 add.add_new_videos(
                     config, [video], coords=[coords], copy_videos=copy_videos,
                 )  # make sure you pass coords as a list
             else:
                 add.add_new_videos(config, [video], coords=None,  copy_videos=copy_videos)
         except:  # can we make a catch here? - in fact we should drop indices from DataCombined if they are in CollectedData.. [ideal behavior; currently this is pretty unlikely]
             print(
@@ -895,16 +897,14 @@
             plt.gca().invert_yaxis()
             plt.savefig(imagename2)
             plt.close("all")
 
 
 def PlottingSingleFramecv2(
     cap,
-    crop,
-    coords,
     Dataframe,
     bodyparts2plot,
     tmpfolder,
     index,
     dotsize,
     pcutoff,
     alphavalue,
@@ -921,24 +921,19 @@
     )
 
     if not os.path.isfile(
         os.path.join(tmpfolder, "img" + str(index).zfill(strwidth) + ".png")
     ):
         plt.axis("off")
         cap.set_to_frame(index)
-        frame = cap.read_frame()
+        frame = cap.read_frame(crop=True)
         if frame is None:
             print("Frame could not be read.")
             return
         image = img_as_ubyte(frame)
-        if crop:
-            image = image[
-                int(coords[2]) : int(coords[3]), int(coords[0]) : int(coords[1]), :
-            ]
-
         io.imsave(imagename1, image)
 
         if savelabeled:
             if np.ndim(image) > 2:
                 h, w, nc = np.shape(image)
             else:
                 h, w = np.shape(image)
```

### Comparing `deeplabcut-2.3rc2/deeplabcut/refine_training_dataset/stitch.py` & `deeplabcut-2.3rc3/deeplabcut/refine_training_dataset/stitch.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/refine_training_dataset/tracklets.py` & `deeplabcut-2.3rc3/deeplabcut/refine_training_dataset/tracklets.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/reid_cfg.yaml` & `deeplabcut-2.3rc3/deeplabcut/reid_cfg.yaml`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/utils/auxfun_multianimal.py` & `deeplabcut-2.3rc3/deeplabcut/utils/auxfun_multianimal.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/utils/auxfun_videos.py` & `deeplabcut-2.3rc3/deeplabcut/utils/auxfun_videos.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/utils/auxiliaryfunctions.py` & `deeplabcut-2.3rc3/deeplabcut/utils/auxiliaryfunctions.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/utils/auxiliaryfunctions_3d.py` & `deeplabcut-2.3rc3/deeplabcut/utils/auxiliaryfunctions_3d.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/utils/conversioncode.py` & `deeplabcut-2.3rc3/deeplabcut/utils/conversioncode.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/utils/frameselectiontools.py` & `deeplabcut-2.3rc3/deeplabcut/utils/frameselectiontools.py`

 * *Files 5% similar despite different names*

```diff
@@ -204,16 +204,14 @@
 
 
 def KmeansbasedFrameselectioncv2(
     cap,
     numframes2pick,
     start,
     stop,
-    crop,
-    coords,
     Index=None,
     step=1,
     resizewidth=30,
     batchsize=100,
     max_iter=50,
     color=False,
 ):
@@ -258,24 +256,16 @@
         if (
             np.mean(np.diff(Index)) > 1
         ):  # then non-consecutive indices are present, thus cap.set is required (which slows everything down!)
             print("Extracting and downsampling...", nframes, " frames from the video.")
             if color:
                 for counter, index in tqdm(enumerate(Index)):
                     cap.set_to_frame(index)  # extract a particular frame
-                    frame = cap.read_frame()
+                    frame = cap.read_frame(crop=True)
                     if frame is not None:
-                        if crop:
-                            frame = frame[
-                                int(coords[2]) : int(coords[3]),
-                                int(coords[0]) : int(coords[1]),
-                                :,
-                            ]
-
-                        # image=img_as_ubyte(cv2.resize(cv2.cvtColor(frame, cv2.COLOR_BGR2RGB),None,fx=ratio,fy=ratio))
                         image = img_as_ubyte(
                             cv2.resize(
                                 frame,
                                 None,
                                 fx=ratio,
                                 fy=ratio,
                                 interpolation=cv2.INTER_NEAREST,
@@ -290,23 +280,16 @@
                             allocated = True
                         DATA[counter, :, :] = np.hstack(
                             [image[:, :, 0], image[:, :, 1], image[:, :, 2]]
                         )
             else:
                 for counter, index in tqdm(enumerate(Index)):
                     cap.set_to_frame(index)  # extract a particular frame
-                    frame = cap.read_frame()
+                    frame = cap.read_frame(crop=True)
                     if frame is not None:
-                        if crop:
-                            frame = frame[
-                                int(coords[2]) : int(coords[3]),
-                                int(coords[0]) : int(coords[1]),
-                                :,
-                            ]
-                        # image=img_as_ubyte(cv2.resize(cv2.cvtColor(frame, cv2.COLOR_BGR2RGB),None,fx=ratio,fy=ratio))
                         image = img_as_ubyte(
                             cv2.resize(
                                 frame,
                                 None,
                                 fx=ratio,
                                 fy=ratio,
                                 interpolation=cv2.INTER_NEAREST,
@@ -320,24 +303,16 @@
                             )
                             allocated = True
                         DATA[counter, :, :] = np.mean(image, 2)
         else:
             print("Extracting and downsampling...", nframes, " frames from the video.")
             if color:
                 for counter, index in tqdm(enumerate(Index)):
-                    frame = cap.read_frame()
+                    frame = cap.read_frame(crop=True)
                     if frame is not None:
-                        if crop:
-                            frame = frame[
-                                int(coords[2]) : int(coords[3]),
-                                int(coords[0]) : int(coords[1]),
-                                :,
-                            ]
-
-                        # image=img_as_ubyte(cv2.resize(cv2.cvtColor(frame, cv2.COLOR_BGR2RGB),None,fx=ratio,fy=ratio))
                         image = img_as_ubyte(
                             cv2.resize(
                                 frame,
                                 None,
                                 fx=ratio,
                                 fy=ratio,
                                 interpolation=cv2.INTER_NEAREST,
@@ -351,23 +326,16 @@
                             )
                             allocated = True
                         DATA[counter, :, :] = np.hstack(
                             [image[:, :, 0], image[:, :, 1], image[:, :, 2]]
                         )
             else:
                 for counter, index in tqdm(enumerate(Index)):
-                    frame = cap.read_frame()
+                    frame = cap.read_frame(crop=True)
                     if frame is not None:
-                        if crop:
-                            frame = frame[
-                                int(coords[2]) : int(coords[3]),
-                                int(coords[0]) : int(coords[1]),
-                                :,
-                            ]
-                        # image=img_as_ubyte(cv2.resize(cv2.cvtColor(frame, cv2.COLOR_BGR2RGB),None,fx=ratio,fy=ratio))
                         image = img_as_ubyte(
                             cv2.resize(
                                 frame,
                                 None,
                                 fx=ratio,
                                 fy=ratio,
                                 interpolation=cv2.INTER_NEAREST,
```

### Comparing `deeplabcut-2.3rc2/deeplabcut/utils/make_labeled_video.py` & `deeplabcut-2.3rc3/deeplabcut/utils/make_labeled_video.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/utils/plotting.py` & `deeplabcut-2.3rc3/deeplabcut/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/utils/skeleton.py` & `deeplabcut-2.3rc3/deeplabcut/utils/skeleton.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/utils/video_processor.py` & `deeplabcut-2.3rc3/deeplabcut/utils/video_processor.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut/utils/visualization.py` & `deeplabcut-2.3rc3/deeplabcut/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `deeplabcut-2.3rc2/deeplabcut.egg-info/PKG-INFO` & `deeplabcut-2.3rc3/deeplabcut.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: deeplabcut
-Version: 2.3rc2
+Version: 2.3rc3
 Summary: Markerless pose-estimation of user-defined features with deep learning
 Home-page: https://github.com/DeepLabCut/DeepLabCut
 Author: A. & M. Mathis Labs
 Author-email: alexander@deeplabcut.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: gui
 Provides-Extra: openvino
 Provides-Extra: docs
 Provides-Extra: tf
 Provides-Extra: apple_mchips
+Provides-Extra: modelzoo
 License-File: LICENSE
+License-File: NOTICE.yml
 License-File: AUTHORS
 
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 ![Python package](https://github.com/DeepLabCut/DeepLabCut/workflows/Python%20package/badge.svg)
 [![PyPI version](https://badge.fury.io/py/deeplabcut.svg)](https://badge.fury.io/py/deeplabcut)
 [![Downloads](https://pepy.tech/badge/deeplabcut)](https://pepy.tech/project/deeplabcut)
 [![Downloads](https://pepy.tech/badge/deeplabcut/month)](https://pepy.tech/project/deeplabcut)
@@ -47,25 +49,27 @@
 <img src="https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/1619609897110-TKSTWKEM6HTGXID9D489/ke17ZwdGBToddI8pDm48kAvjv6tW_eojYQmNU0ncbllZw-zPPgdn4jUwVcJE1ZvWEtT5uBSRWt4vQZAgTJucoTqqXjS3CfNDSuuf31e0tVHBSTXHtjUKlhRtWJ1Vo6l1B2bxJtByvWSjL6Vz3amc5yb8BodarTVrzIWCp72ioWw/triMouseDLC.gif?format=300w" height="150">
 
 <img src="https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/5c3fbd0c898583417a040dfc/1547681053201/rat-grasp.gif?format=300w" height="150">
 </p>
 
 DeepLabCut is a toolbox for markerless pose estimation of animals performing various tasks. [Read a short development and application summary below](https://github.com/DeepLabCut/DeepLabCut#why-use-deeplabcut). As long as you can see (label) what you want to track, you can use this toolbox, as it is animal and object agnostic.
 
+**Quick start** read the docs: https://deeplabcut.github.io/DeepLabCut
+
 **Latest updates:**
 
 :purple_heart: **DeepLabCut supports multi-animal pose estimation!** maDLC is out of beta/rc mode and beta is deprecated, thanks to the testers out there for feedback! Your labeled data will be backwards compatible, but not all other steps. Please see the [new `2.2+` releases](https://github.com/DeepLabCut/DeepLabCut/releases) for what's new & how to install it, please see our new [paper, Lauer et al 2022](https://www.nature.com/articles/s41592-022-01443-0), and the [new docs]( https://deeplabcut.github.io/DeepLabCut) on how to use it!
 
 :purple_heart: We support multi-animal re-identification, see [Lauer et al 2022](https://www.nature.com/articles/s41592-022-01443-0).
 
 :purple_heart: We have a **real-time** package available! http://DLClive.deeplabcut.org
 
 # [Installation: how to install DeepLabCut](https://deeplabcut.github.io/DeepLabCut/docs/installation.html)
 
-Very quick start: `pip install "deeplabcut[gui]"` that includes all GUI functions, or `pip install deeplabcut` (headless version).
+Very quick start: `pip install "deeplabcut[gui,tf]"` that includes all functions plus GUIs, or `pip install deeplabcut[tf]` (headless version with PyTorch and TensorFlow).
 * We recommend using our conda file, see [here](https://github.com/DeepLabCut/DeepLabCut/blob/master/conda-environments/README.md) or the new [`deeplabcut-docker` package](https://github.com/DeepLabCut/DeepLabCut/tree/master/docker).
 
 # [Documentation: The DeepLabCut Process](https://deeplabcut.github.io/DeepLabCut)
 
 Our docs walk you through using DeepLabCut, and key API points. For an overview of the toolbox and workflow for project management, see our step-by-step at [Nature Protocols paper](https://doi.org/10.1038/s41596-019-0176-0).
 
 For a deeper understanding and more resources for you to get started with Python and DeepLabCut, please check out our free online course! http://DLCcourse.deeplabcut.org
@@ -76,15 +80,15 @@
 
 # [DEMO the code](/examples)
 
 We provide data and several Jupyter Notebooks: one that walks you through a demo dataset to test your installation, and another Notebook to run DeepLabCut from the beginning on your own data. We also show you how to use the code in Docker, and on Google Colab.
 
 # Why use DeepLabCut?
 
-In 2018, we demonstrated the capabilities for [trail tracking](https://vnmurthylab.org/), [reaching in mice](http://www.mousemotorlab.org/) and various Drosophila behaviors during egg-laying (see [Mathis et al.](https://www.nature.com/articles/s41593-018-0209-y) for details). There is, however, nothing specific that makes the toolbox only applicable to these tasks and/or species. The toolbox has already been successfully applied (by us and others) to [rats](http://www.mousemotorlab.org/deeplabcut), humans, various fish species, bacteria, leeches, various robots, cheetahs, [mouse whiskers](http://www.mousemotorlab.org/deeplabcut) and [race horses](http://www.mousemotorlab.org/deeplabcut). DeepLabCut utilized the feature detectors (ResNets + readout layers) of one of the state-of-the-art algorithms for human pose estimation by Insafutdinov et al., called DeeperCut, which inspired the name for our toolbox (see references below). Since this time, the package has changed substantially.  The code has been re-tooled and re-factored since 2.1+: We have added faster and higher performance variants with MobileNetV2s, EfficientNets, and our own DLCRNet backbones (see [Pretraining boosts out-of-domain robustness for pose estimation](https://arxiv.org/abs/1909.11229) and [Lauer et al 2021](https://www.biorxiv.org/content/10.1101/2021.04.30.442096v1)). Additionally, we have improved the inference speed and provided both additional and novel augmentation methods, added real-time, and multi-animal support. We currently provide state-of-the-art performance for animal pose estimation.
+In 2018, we demonstrated the capabilities for [trail tracking](https://vnmurthylab.org/), [reaching in mice](http://www.mousemotorlab.org/) and various Drosophila behaviors during egg-laying (see [Mathis et al.](https://www.nature.com/articles/s41593-018-0209-y) for details). There is, however, nothing specific that makes the toolbox only applicable to these tasks and/or species. The toolbox has already been successfully applied (by us and others) to [rats](http://www.mousemotorlab.org/deeplabcut), humans, various fish species, bacteria, leeches, various robots, cheetahs, [mouse whiskers](http://www.mousemotorlab.org/deeplabcut) and [race horses](http://www.mousemotorlab.org/deeplabcut). DeepLabCut utilized the feature detectors (ResNets + readout layers) of one of the state-of-the-art algorithms for human pose estimation by Insafutdinov et al., called DeeperCut, which inspired the name for our toolbox (see references below). Since this time, the package has changed substantially.  The code has been re-tooled and re-factored since 2.1+: We have added faster and higher performance variants with MobileNetV2s, EfficientNets, and our own DLCRNet backbones (see [Pretraining boosts out-of-domain robustness for pose estimation](https://arxiv.org/abs/1909.11229) and [Lauer et al 2022](https://www.nature.com/articles/s41592-022-01443-0)). Additionally, we have improved the inference speed and provided both additional and novel augmentation methods, added real-time, and multi-animal support. We currently provide state-of-the-art performance for animal pose estimation.
 
 <p align="center">
 <img src="https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/5c3e47258a922d548c483247/1547585339819/ErrorvsTrainingsetSize.png?format=750w" height="160">
 <img src="https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/5c3e469d8a922d548c4828fa/1547585194560/compressionrobustness.png?format=750w" height="160">
 <img src="https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/5c3fbed74fa51acecd63deeb/1547681534736/MouseLocomotion_warren.gif?format=500w" height="160">  
 <img src="https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/5c3fc1c6758d46950ce7eec7/1547682383595/cheetah.png?format=750w" height="160">
 </p>
@@ -95,15 +99,15 @@
 
 <p align="center">
 <img src="https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/1588292233203-FD1DVKAQYNV2TU91CO7R/ke17ZwdGBToddI8pDm48kIX24IsDPzy6M4KUaihfICJZw-zPPgdn4jUwVcJE1ZvWQUxwkmyExglNqGp0IvTJZamWLI2zvYWH8K3-s_4yszcp2ryTI0HqTOaaUohrI8PIxtGUdkzp028KVNnpOijF3PweOM5su6FUQHO6Wkh72Nw/dlc_eco.gif?format=1000w" width="80%">
 </p>
 
 ## Code contributors:
 
-DLC code was originally developed by [Alexander Mathis](https://github.com/AlexEMG) & [Mackenzie Mathis](https://github.com/MMathisLab), and was extended in 2.0 with [Tanmay Nath](http://www.mousemotorlab.org/team), and currently (2.1+) actively developed with our CZI DLC Fellow, [Jessy Lauer](https://github.com/jeylau). DeepLabCut is an open-source tool and has benefited from suggestions and edits by many individuals including  Mert Yuksekgonul, Tom Biasi, Richard Warren, Ronny Eichler, Hao Wu, Federico Claudi, Gary Kane and Jonny Saunders as well as the [contributors](https://github.com/DeepLabCut/DeepLabCut/graphs/contributors). Please see [AUTHORS](https://github.com/DeepLabCut/DeepLabCut/blob/master/AUTHORS) for more details!
+DLC code was originally developed by [Alexander Mathis](https://github.com/AlexEMG) & [Mackenzie Mathis](https://github.com/MMathisLab), and was extended in 2.0 with [Tanmay Nath](http://www.mousemotorlab.org/team), and currently (2.1+) actively developed with [Jessy Lauer](https://github.com/jeylau). DeepLabCut is an open-source tool and has benefited from suggestions and edits by many individuals including  Mert Yuksekgonul, Tom Biasi, Richard Warren, Ronny Eichler, Hao Wu, Federico Claudi, Gary Kane and Jonny Saunders as well as the [contributors](https://github.com/DeepLabCut/DeepLabCut/graphs/contributors). Please see [AUTHORS](https://github.com/DeepLabCut/DeepLabCut/blob/master/AUTHORS) for more details!
 
 This is an actively developed package and we welcome community development and involvement.
 
 ## Be part of the DLC Community✨:
 
 | 🚉 Platform                                                 | 🎯 Goal                                                                      | ⏱️ Estimated Response Time | 📢 Support Squad                        |
 |------------------------------------------------------------|-----------------------------------------------------------------------------|---------------------------|----------------------------------------|
@@ -114,20 +118,21 @@
 | 🚧 GitHub DeepLabCut/[Roadmap](https://github.com/DeepLabCut/DeepLabCut/blob/master/docs/roadmap.md)                             | To learn more about our journey✈️                                            | N/A                       | N/A                                    |
 | [![Twitter Follow](https://img.shields.io/twitter/follow/DeepLabCut.svg?label=DeepLabCut&style=social)](https://twitter.com/DeepLabCut)                                                   | To keep up with our latest news and updates 📢                               | Daily                     | DLC Team                               |
 | The DeepLabCut [AI Residency Program](https://www.deeplabcutairesidency.org/)                        | To come and work with us next summer👏                                       | Annually                  | DLC Team                               |
 
 
 ## References:
 
-If you use this code or data we kindly as that you please [cite Mathis et al, 2018](https://www.nature.com/articles/s41593-018-0209-y) and, if you use the Python package (DeepLabCut2.x) please also cite [Nath, Mathis et al, 2019](https://doi.org/10.1038/s41596-019-0176-0). If you utilize the MobileNetV2s or EfficientNets please cite [Mathis, Biasi et al. 2021](https://openaccess.thecvf.com/content/WACV2021/papers/Mathis_Pretraining_Boosts_Out-of-Domain_Robustness_for_Pose_Estimation_WACV_2021_paper.pdf). If you use multi-animal in beta mode, please contact us; if you use the 2.2rc1+, please cite [Lauer et al. 2021](https://www.biorxiv.org/content/10.1101/2021.04.30.442096v1).
+If you use this code or data we kindly as that you please [cite Mathis et al, 2018](https://www.nature.com/articles/s41593-018-0209-y) and, if you use the Python package (DeepLabCut2.x) please also cite [Nath, Mathis et al, 2019](https://doi.org/10.1038/s41596-019-0176-0). If you utilize the MobileNetV2s or EfficientNets please cite [Mathis, Biasi et al. 2021](https://openaccess.thecvf.com/content/WACV2021/papers/Mathis_Pretraining_Boosts_Out-of-Domain_Robustness_for_Pose_Estimation_WACV_2021_paper.pdf). If you use versions 2.2beta+ or 2.2rc1+, please cite [Lauer et al. 2022](https://www.nature.com/articles/s41592-022-01443-0).
 
 DOIs (#ProTip, for helping you find citations for software, check out [CiteAs.org](http://citeas.org/)!):
 
 - Mathis et al 2018: [10.1038/s41593-018-0209-y](https://doi.org/10.1038/s41593-018-0209-y)
 - Nath, Mathis et al 2019: [10.1038/s41596-019-0176-0](https://doi.org/10.1038/s41596-019-0176-0)
+- Lauer et al 2022: [10.1038/s41592-022-01443-0](https://doi.org/10.1038/s41592-022-01443-0)
 
 
 Please check out the following references for more details:
 
     @article{Mathisetal2018,
         title = {DeepLabCut: markerless pose estimation of user-defined body parts with deep learning},
         author = {Alexander Mathis and Pranav Mamidanna and Kevin M. Cury and Taiga Abe  and Venkatesh N. Murthy and Mackenzie W. Mathis and Matthias Bethge},
@@ -160,15 +165,15 @@
 
     @article{insafutdinov2016eccv,
         title = {DeeperCut: A Deeper, Stronger, and Faster Multi-Person Pose Estimation Model},
         author = {Eldar Insafutdinov and Leonid Pishchulin and Bjoern Andres and Mykhaylo Andriluka and Bernt Schiele},
         booktitle = {ECCV'16},
         url = {http://arxiv.org/abs/1605.03170}}
         
-Review articles:
+Review & Educational articles:
 
     @article{Mathis2020DeepLT,
         title={Deep learning tools for the measurement of animal behavior in neuroscience},
         author={Mackenzie W. Mathis and Alexander Mathis},
         journal={Current Opinion in Neurobiology},
         year={2020},
         volume={60},
@@ -192,27 +197,29 @@
         publisher = {Cold Spring Harbor Laboratory},
         URL = {https://www.biorxiv.org/content/early/2018/10/30/457242},
         eprint = {https://www.biorxiv.org/content/early/2018/10/30/457242.full.pdf},
         journal = {bioRxiv}}
 
 ## License:
 
-This project is licensed under the GNU Lesser General Public License v3.0. Note that the software is provided "as is", without warranty of any kind, express or implied. If you use the code or data, please cite us! Note, artwork (DeepLabCut logo) and images are copyrighted; please do not take or use these images without written permission.
+This project is primarily licensed under the GNU Lesser General Public License v3.0. Note that the software is provided "as is", without warranty of any kind, express or implied. If you use the code or data, please cite us! Note, artwork (DeepLabCut logo) and images are copyrighted; please do not take or use these images without written permission.
 
 ## Versions:
 
-VERSION 2.2: Multi-animal pose estimation and tracking with DeepLabCut is supported (as well as single-animal projects).
+VERSION 2.2: Multi-animal pose estimation, identification, and tracking with DeepLabCut is supported (as well as single-animal projects).
 
-VERSION 2.0-2.1: This is the **Python package** of [DeepLabCut](https://www.nature.com/articles/s41593-018-0209-y) that was originally released with our [Nature Protocols](https://doi.org/10.1038/s41596-019-0176-0) paper (preprint [here](https://www.biorxiv.org/content/10.1101/476531v1)).
+VERSION 2.0-2.1: This is the **Python package** of [DeepLabCut](https://www.nature.com/articles/s41593-018-0209-y) that was originally released in Oct 2018 with our [Nature Protocols](https://doi.org/10.1038/s41596-019-0176-0) paper (preprint [here](https://www.biorxiv.org/content/10.1101/476531v1)).
 This package includes graphical user interfaces to label your data, and take you from data set creation to automatic behavioral analysis. It also introduces an active learning framework to efficiently use DeepLabCut on large experimental projects, and data augmentation tools that improve network performance, especially in challenging cases (see [panel b](https://camo.githubusercontent.com/77c92f6b89d44ca758d815bdd7e801247437060b/68747470733a2f2f737461746963312e73717561726573706163652e636f6d2f7374617469632f3537663664353163396637343536366635356563663237312f742f3563336663316336373538643436393530636537656563372f313534373638323338333539352f636865657461682e706e673f666f726d61743d37353077)).
 
 VERSION 1.0: The initial, Nature Neuroscience version of [DeepLabCut](https://www.nature.com/articles/s41593-018-0209-y) can be found in the history of git, or here: https://github.com/DeepLabCut/DeepLabCut/releases/tag/1.11
 
 ## News (and in the news):
 
+- August 2022: DeepLabCut hit 400,000 downloads!
+
 - August 2021: 2.2 becomes the new stable release for DeepLabCut.
 
 - July 2021: Docs are now at https://deeplabcut.github.io/DeepLabCut and we now include TensorFlow 2 support!
 
 - May 2021: DeepLabCut hit 200,000 downloads! Also, Our preprint on 2.2, multi-animal DeepLabCut is released!
 
 - Jan 2021: [Pretraining boosts out-of-domain robustness for pose estimation](https://openaccess.thecvf.com/content/WACV2021/html/Mathis_Pretraining_Boosts_Out-of-Domain_Robustness_for_Pose_Estimation_WACV_2021_paper.html) published in the IEEE Winter Conference on Applications of Computer Vision. We also added EfficientNet backbones to DeepLabCut, those are best trained with cosine decay (see paper). To use them, just pass "`efficientnet-b0`" to "`efficientnet-b6`" when creating the trainingset!
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: deeplabcut Version: 2.3rc2 Summary: Markerless
+Metadata-Version: 2.1 Name: deeplabcut Version: 2.3rc3 Summary: Markerless
 pose-estimation of user-defined features with deep learning Home-page: https://
 github.com/DeepLabCut/DeepLabCut Author: A. & M. Mathis Labs Author-email:
 alexander@deeplabcut.org Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3
 (LGPLv3) Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown Provides-Extra: gui Provides-Extra: openvino Provides-
-Extra: docs Provides-Extra: tf Provides-Extra: apple_mchips License-File:
-LICENSE License-File: AUTHORS [Code_style:_black] ![Python package](https://
-github.com/DeepLabCut/DeepLabCut/workflows/Python%20package/badge.svg) [![PyPI
-version](https://badge.fury.io/py/deeplabcut.svg)](https://badge.fury.io/py/
-deeplabcut) [![Downloads](https://pepy.tech/badge/deeplabcut)](https://
-pepy.tech/project/deeplabcut) [![Downloads](https://pepy.tech/badge/deeplabcut/
-month)](https://pepy.tech/project/deeplabcut) [![GitHub stars](https://
-img.shields.io/github/stars/DeepLabCut/DeepLabCut.svg?style=social&label=Star)]
-(https://github.com/DeepLabCut/DeepLabCut) [![Generic badge](https://
-img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](CONTRIBUTING.md)
-[![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)]
-(https://www.gnu.org/licenses/lgpl-3.0) [![Image.sc forum](https://
-img.shields.io/badge/dynamic/
+Extra: docs Provides-Extra: tf Provides-Extra: apple_mchips Provides-Extra:
+modelzoo License-File: LICENSE License-File: NOTICE.yml License-File: AUTHORS
+[Code_style:_black] ![Python package](https://github.com/DeepLabCut/DeepLabCut/
+workflows/Python%20package/badge.svg) [![PyPI version](https://badge.fury.io/
+py/deeplabcut.svg)](https://badge.fury.io/py/deeplabcut) [![Downloads](https://
+pepy.tech/badge/deeplabcut)](https://pepy.tech/project/deeplabcut) [!
+[Downloads](https://pepy.tech/badge/deeplabcut/month)](https://pepy.tech/
+project/deeplabcut) [![GitHub stars](https://img.shields.io/github/stars/
+DeepLabCut/DeepLabCut.svg?style=social&label=Star)](https://github.com/
+DeepLabCut/DeepLabCut) [![Generic badge](https://img.shields.io/badge/
+Contributions-Welcome-brightgreen.svg)](CONTRIBUTING.md) [![License: LGPL v3]
+(https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/
+licenses/lgpl-3.0) [![Image.sc forum](https://img.shields.io/badge/dynamic/
 json.svg?label=forum&url=https%3A%2F%2Fforum.image.sc%2Ftag%2Fdeeplabcut.json&query=%24.topic_list.tags.0.topic_count&colorB=brightgreen&&suffix=%20topics&logo=data:
 image/
 png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+/
 /
 17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/
 cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://
 forum.image.sc/tag/deeplabcut) [![Gitter](https://badges.gitter.im/DeepLabCut/
@@ -51,38 +51,39 @@
      triMouseDLC.gif?format=300w] [https://static1.squarespace.com/static/
     57f6d51c9f74566f55ecf271/t/5c3fbd0c898583417a040dfc/1547681053201/rat-
                             grasp.gif?format=300w]
 DeepLabCut is a toolbox for markerless pose estimation of animals performing
 various tasks. [Read a short development and application summary below](https:/
 /github.com/DeepLabCut/DeepLabCut#why-use-deeplabcut). As long as you can see
 (label) what you want to track, you can use this toolbox, as it is animal and
-object agnostic. **Latest updates:** :purple_heart: **DeepLabCut supports
-multi-animal pose estimation!** maDLC is out of beta/rc mode and beta is
-deprecated, thanks to the testers out there for feedback! Your labeled data
-will be backwards compatible, but not all other steps. Please see the [new
-`2.2+` releases](https://github.com/DeepLabCut/DeepLabCut/releases) for what's
-new & how to install it, please see our new [paper, Lauer et al 2022](https://
+object agnostic. **Quick start** read the docs: https://deeplabcut.github.io/
+DeepLabCut **Latest updates:** :purple_heart: **DeepLabCut supports multi-
+animal pose estimation!** maDLC is out of beta/rc mode and beta is deprecated,
+thanks to the testers out there for feedback! Your labeled data will be
+backwards compatible, but not all other steps. Please see the [new `2.2+`
+releases](https://github.com/DeepLabCut/DeepLabCut/releases) for what's new &
+how to install it, please see our new [paper, Lauer et al 2022](https://
 www.nature.com/articles/s41592-022-01443-0), and the [new docs]( https://
 deeplabcut.github.io/DeepLabCut) on how to use it! :purple_heart: We support
 multi-animal re-identification, see [Lauer et al 2022](https://www.nature.com/
 articles/s41592-022-01443-0). :purple_heart: We have a **real-time** package
 available! http://DLClive.deeplabcut.org # [Installation: how to install
 DeepLabCut](https://deeplabcut.github.io/DeepLabCut/docs/installation.html)
-Very quick start: `pip install "deeplabcut[gui]"` that includes all GUI
-functions, or `pip install deeplabcut` (headless version). * We recommend using
-our conda file, see [here](https://github.com/DeepLabCut/DeepLabCut/blob/
-master/conda-environments/README.md) or the new [`deeplabcut-docker` package]
-(https://github.com/DeepLabCut/DeepLabCut/tree/master/docker). #
-[Documentation: The DeepLabCut Process](https://deeplabcut.github.io/
-DeepLabCut) Our docs walk you through using DeepLabCut, and key API points. For
-an overview of the toolbox and workflow for project management, see our step-
-by-step at [Nature Protocols paper](https://doi.org/10.1038/s41596-019-0176-0).
-For a deeper understanding and more resources for you to get started with
-Python and DeepLabCut, please check out our free online course! http://
-DLCcourse.deeplabcut.org
+Very quick start: `pip install "deeplabcut[gui,tf]"` that includes all
+functions plus GUIs, or `pip install deeplabcut[tf]` (headless version with
+PyTorch and TensorFlow). * We recommend using our conda file, see [here](https:
+//github.com/DeepLabCut/DeepLabCut/blob/master/conda-environments/README.md) or
+the new [`deeplabcut-docker` package](https://github.com/DeepLabCut/DeepLabCut/
+tree/master/docker). # [Documentation: The DeepLabCut Process](https://
+deeplabcut.github.io/DeepLabCut) Our docs walk you through using DeepLabCut,
+and key API points. For an overview of the toolbox and workflow for project
+management, see our step-by-step at [Nature Protocols paper](https://doi.org/
+10.1038/s41596-019-0176-0). For a deeper understanding and more resources for
+you to get started with Python and DeepLabCut, please check out our free online
+course! http://DLCcourse.deeplabcut.org
    [https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/
                       1609244903687-US1SN063QIFJS4BP4IJD/
 ke17ZwdGBToddI8pDm48kFG9xAYub2PPnmh56PTVg7gUqsxRUqqbr1mOJYKfIPR7LoDQ9mXPOjoJoqy81S2I8N_N4V1vUb5AoIIIbLZhVYxCRW4BPu10St3TBAUQYVKcAju5e7u9RZJEVbVQPZRu9xb_m-
                     kUO2M3I1IeDqD4l8YcGqu2nZPx1UhKV8wc1ELN/
                   dlc_overview_whitebkgrnd.png?format=2500w]
 # [DEMO the code](/examples) We provide data and several Jupyter Notebooks: one
 that walks you through a demo dataset to test your installation, and another
@@ -101,19 +102,18 @@
 (ResNets + readout layers) of one of the state-of-the-art algorithms for human
 pose estimation by Insafutdinov et al., called DeeperCut, which inspired the
 name for our toolbox (see references below). Since this time, the package has
 changed substantially. The code has been re-tooled and re-factored since 2.1+:
 We have added faster and higher performance variants with MobileNetV2s,
 EfficientNets, and our own DLCRNet backbones (see [Pretraining boosts out-of-
 domain robustness for pose estimation](https://arxiv.org/abs/1909.11229) and
-[Lauer et al 2021](https://www.biorxiv.org/content/10.1101/
-2021.04.30.442096v1)). Additionally, we have improved the inference speed and
-provided both additional and novel augmentation methods, added real-time, and
-multi-animal support. We currently provide state-of-the-art performance for
-animal pose estimation.
+[Lauer et al 2022](https://www.nature.com/articles/s41592-022-01443-0)).
+Additionally, we have improved the inference speed and provided both additional
+and novel augmentation methods, added real-time, and multi-animal support. We
+currently provide state-of-the-art performance for animal pose estimation.
       [https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/
 5c3e47258a922d548c483247/1547585339819/ErrorvsTrainingsetSize.png?format=750w]
       [https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/
 5c3e469d8a922d548c4828fa/1547585194560/compressionrobustness.png?format=750w]
       [https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/
 5c3fbed74fa51acecd63deeb/1547681534736/MouseLocomotion_warren.gif?format=500w]
       [https://static1.squarespace.com/static/57f6d51c9f74566f55ecf271/t/
@@ -137,28 +137,28 @@
                 ke17ZwdGBToddI8pDm48kIX24IsDPzy6M4KUaihfICJZw-
             zPPgdn4jUwVcJE1ZvWQUxwkmyExglNqGp0IvTJZamWLI2zvYWH8K3-
    s_4yszcp2ryTI0HqTOaaUohrI8PIxtGUdkzp028KVNnpOijF3PweOM5su6FUQHO6Wkh72Nw/
                            dlc_eco.gif?format=1000w]
 ## Code contributors: DLC code was originally developed by [Alexander Mathis]
 (https://github.com/AlexEMG) & [Mackenzie Mathis](https://github.com/
 MMathisLab), and was extended in 2.0 with [Tanmay Nath](http://
-www.mousemotorlab.org/team), and currently (2.1+) actively developed with our
-CZI DLC Fellow, [Jessy Lauer](https://github.com/jeylau). DeepLabCut is an
-open-source tool and has benefited from suggestions and edits by many
-individuals including Mert Yuksekgonul, Tom Biasi, Richard Warren, Ronny
-Eichler, Hao Wu, Federico Claudi, Gary Kane and Jonny Saunders as well as the
-[contributors](https://github.com/DeepLabCut/DeepLabCut/graphs/contributors).
-Please see [AUTHORS](https://github.com/DeepLabCut/DeepLabCut/blob/master/
-AUTHORS) for more details! This is an actively developed package and we welcome
-community development and involvement. ## Be part of the DLC Communityâ¨: |
-ð Platform | ð¯ Goal | â±ï¸ Estimated Response Time | ð¢ Support Squad
-| |------------------------------------------------------------|---------------
---------------------------------------------------------------|----------------
------------|----------------------------------------| | [![Image.sc forum]
-(https://img.shields.io/badge/dynamic/
+www.mousemotorlab.org/team), and currently (2.1+) actively developed with
+[Jessy Lauer](https://github.com/jeylau). DeepLabCut is an open-source tool and
+has benefited from suggestions and edits by many individuals including Mert
+Yuksekgonul, Tom Biasi, Richard Warren, Ronny Eichler, Hao Wu, Federico Claudi,
+Gary Kane and Jonny Saunders as well as the [contributors](https://github.com/
+DeepLabCut/DeepLabCut/graphs/contributors). Please see [AUTHORS](https://
+github.com/DeepLabCut/DeepLabCut/blob/master/AUTHORS) for more details! This is
+an actively developed package and we welcome community development and
+involvement. ## Be part of the DLC Communityâ¨: | ð Platform | ð¯ Goal |
+â±ï¸ Estimated Response Time | ð¢ Support Squad | |------------------------
+------------------------------------|------------------------------------------
+-----------------------------------|---------------------------|---------------
+-------------------------| | [![Image.sc forum](https://img.shields.io/badge/
+dynamic/
 json.svg?label=forum&url=https%3A%2F%2Fforum.image.sc%2Ftag%2Fdeeplabcut.json&query=%24.topic_list.tags.0.topic_count&colorB=brightgreen&&suffix=%20topics&logo=data:
 image/
 png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+/
 /
 17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/
 cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://
 forum.image.sc/tag/deeplabcut)
@@ -181,88 +181,88 @@
 come and work with us next summerð | Annually | DLC Team | ## References: If
 you use this code or data we kindly as that you please [cite Mathis et al,
 2018](https://www.nature.com/articles/s41593-018-0209-y) and, if you use the
 Python package (DeepLabCut2.x) please also cite [Nath, Mathis et al, 2019]
 (https://doi.org/10.1038/s41596-019-0176-0). If you utilize the MobileNetV2s or
 EfficientNets please cite [Mathis, Biasi et al. 2021](https://
 openaccess.thecvf.com/content/WACV2021/papers/Mathis_Pretraining_Boosts_Out-of-
-Domain_Robustness_for_Pose_Estimation_WACV_2021_paper.pdf). If you use multi-
-animal in beta mode, please contact us; if you use the 2.2rc1+, please cite
-[Lauer et al. 2021](https://www.biorxiv.org/content/10.1101/
-2021.04.30.442096v1). DOIs (#ProTip, for helping you find citations for
+Domain_Robustness_for_Pose_Estimation_WACV_2021_paper.pdf). If you use versions
+2.2beta+ or 2.2rc1+, please cite [Lauer et al. 2022](https://www.nature.com/
+articles/s41592-022-01443-0). DOIs (#ProTip, for helping you find citations for
 software, check out [CiteAs.org](http://citeas.org/)!): - Mathis et al 2018:
 [10.1038/s41593-018-0209-y](https://doi.org/10.1038/s41593-018-0209-y) - Nath,
 Mathis et al 2019: [10.1038/s41596-019-0176-0](https://doi.org/10.1038/s41596-
-019-0176-0) Please check out the following references for more details:
-@article{Mathisetal2018, title = {DeepLabCut: markerless pose estimation of
-user-defined body parts with deep learning}, author = {Alexander Mathis and
-Pranav Mamidanna and Kevin M. Cury and Taiga Abe and Venkatesh N. Murthy and
-Mackenzie W. Mathis and Matthias Bethge}, journal = {Nature Neuroscience}, year
-= {2018}, url = {https://www.nature.com/articles/s41593-018-0209-y}} @article
-{NathMathisetal2019, title = {Using DeepLabCut for 3D markerless pose
-estimation across species and behaviors}, author = {Nath*, Tanmay and Mathis*,
-Alexander and Chen, An Chi and Patel, Amir and Bethge, Matthias and Mathis,
-Mackenzie W}, journal = {Nature Protocols}, year = {2019}, url = {https://
-doi.org/10.1038/s41596-019-0176-0}} @InProceedings{Mathis_2021_WACV, author =
-{Mathis, Alexander and Biasi, Thomas and Schneider, Steffen and Yuksekgonul,
-Mert and Rogers, Byron and Bethge, Matthias and Mathis, Mackenzie W.}, title =
-{Pretraining Boosts Out-of-Domain Robustness for Pose Estimation}, booktitle =
-{Proceedings of the IEEE/CVF Winter Conference on Applications of Computer
-Vision (WACV)}, month = {January}, year = {2021}, pages = {1859-1868}} @article
-{Lauer2022MultianimalPE, title={Multi-animal pose estimation, identification
-and tracking with DeepLabCut}, author={Jessy Lauer and Mu Zhou and Shaokai Ye
-and William Menegas and Steffen Schneider and Tanmay Nath and Mohammed
-Mostafizur Rahman and Valentina Di Santo and Daniel Soberanes and Guoping Feng
-and Venkatesh N. Murthy and George Lauder and Catherine Dulac and M. Mathis and
-Alexander Mathis}, journal={Nature Methods}, year={2022}, volume={19}, pages=
-{496 - 504}} @article{insafutdinov2016eccv, title = {DeeperCut: A Deeper,
-Stronger, and Faster Multi-Person Pose Estimation Model}, author = {Eldar
-Insafutdinov and Leonid Pishchulin and Bjoern Andres and Mykhaylo Andriluka and
-Bernt Schiele}, booktitle = {ECCV'16}, url = {http://arxiv.org/abs/1605.03170}}
-Review articles: @article{Mathis2020DeepLT, title={Deep learning tools for the
-measurement of animal behavior in neuroscience}, author={Mackenzie W. Mathis
-and Alexander Mathis}, journal={Current Opinion in Neurobiology}, year={2020},
-volume={60}, pages={1-11}} @article{Mathis2020Primer, title={A Primer on Motion
-Capture with Deep Learning: Principles, Pitfalls, and Perspectives}, author=
-{Alexander Mathis and Steffen Schneider and Jessy Lauer and Mackenzie W.
-Mathis}, journal={Neuron}, year={2020}, volume={108}, pages={44-65}} Other
-open-access pre-prints related to our work on DeepLabCut: @article
-{MathisWarren2018speed, author = {Mathis, Alexander and Warren, Richard A.},
-title = {On the inference speed and video-compression robustness of
-DeepLabCut}, year = {2018}, doi = {10.1101/457242}, publisher = {Cold Spring
-Harbor Laboratory}, URL = {https://www.biorxiv.org/content/early/2018/10/30/
-457242}, eprint = {https://www.biorxiv.org/content/early/2018/10/30/
-457242.full.pdf}, journal = {bioRxiv}} ## License: This project is licensed
-under the GNU Lesser General Public License v3.0. Note that the software is
-provided "as is", without warranty of any kind, express or implied. If you use
-the code or data, please cite us! Note, artwork (DeepLabCut logo) and images
-are copyrighted; please do not take or use these images without written
-permission. ## Versions: VERSION 2.2: Multi-animal pose estimation and tracking
-with DeepLabCut is supported (as well as single-animal projects). VERSION 2.0-
-2.1: This is the **Python package** of [DeepLabCut](https://www.nature.com/
-articles/s41593-018-0209-y) that was originally released with our [Nature
-Protocols](https://doi.org/10.1038/s41596-019-0176-0) paper (preprint [here]
-(https://www.biorxiv.org/content/10.1101/476531v1)). This package includes
-graphical user interfaces to label your data, and take you from data set
-creation to automatic behavioral analysis. It also introduces an active
-learning framework to efficiently use DeepLabCut on large experimental
-projects, and data augmentation tools that improve network performance,
-especially in challenging cases (see [panel b](https://
-camo.githubusercontent.com/77c92f6b89d44ca758d815bdd7e801247437060b/
+019-0176-0) - Lauer et al 2022: [10.1038/s41592-022-01443-0](https://doi.org/
+10.1038/s41592-022-01443-0) Please check out the following references for more
+details: @article{Mathisetal2018, title = {DeepLabCut: markerless pose
+estimation of user-defined body parts with deep learning}, author = {Alexander
+Mathis and Pranav Mamidanna and Kevin M. Cury and Taiga Abe and Venkatesh N.
+Murthy and Mackenzie W. Mathis and Matthias Bethge}, journal = {Nature
+Neuroscience}, year = {2018}, url = {https://www.nature.com/articles/s41593-
+018-0209-y}} @article{NathMathisetal2019, title = {Using DeepLabCut for 3D
+markerless pose estimation across species and behaviors}, author = {Nath*,
+Tanmay and Mathis*, Alexander and Chen, An Chi and Patel, Amir and Bethge,
+Matthias and Mathis, Mackenzie W}, journal = {Nature Protocols}, year = {2019},
+url = {https://doi.org/10.1038/s41596-019-0176-0}} @InProceedings
+{Mathis_2021_WACV, author = {Mathis, Alexander and Biasi, Thomas and Schneider,
+Steffen and Yuksekgonul, Mert and Rogers, Byron and Bethge, Matthias and
+Mathis, Mackenzie W.}, title = {Pretraining Boosts Out-of-Domain Robustness for
+Pose Estimation}, booktitle = {Proceedings of the IEEE/CVF Winter Conference on
+Applications of Computer Vision (WACV)}, month = {January}, year = {2021},
+pages = {1859-1868}} @article{Lauer2022MultianimalPE, title={Multi-animal pose
+estimation, identification and tracking with DeepLabCut}, author={Jessy Lauer
+and Mu Zhou and Shaokai Ye and William Menegas and Steffen Schneider and Tanmay
+Nath and Mohammed Mostafizur Rahman and Valentina Di Santo and Daniel Soberanes
+and Guoping Feng and Venkatesh N. Murthy and George Lauder and Catherine Dulac
+and M. Mathis and Alexander Mathis}, journal={Nature Methods}, year={2022},
+volume={19}, pages={496 - 504}} @article{insafutdinov2016eccv, title =
+{DeeperCut: A Deeper, Stronger, and Faster Multi-Person Pose Estimation Model},
+author = {Eldar Insafutdinov and Leonid Pishchulin and Bjoern Andres and
+Mykhaylo Andriluka and Bernt Schiele}, booktitle = {ECCV'16}, url = {http://
+arxiv.org/abs/1605.03170}} Review & Educational articles: @article
+{Mathis2020DeepLT, title={Deep learning tools for the measurement of animal
+behavior in neuroscience}, author={Mackenzie W. Mathis and Alexander Mathis},
+journal={Current Opinion in Neurobiology}, year={2020}, volume={60}, pages={1-
+11}} @article{Mathis2020Primer, title={A Primer on Motion Capture with Deep
+Learning: Principles, Pitfalls, and Perspectives}, author={Alexander Mathis and
+Steffen Schneider and Jessy Lauer and Mackenzie W. Mathis}, journal={Neuron},
+year={2020}, volume={108}, pages={44-65}} Other open-access pre-prints related
+to our work on DeepLabCut: @article{MathisWarren2018speed, author = {Mathis,
+Alexander and Warren, Richard A.}, title = {On the inference speed and video-
+compression robustness of DeepLabCut}, year = {2018}, doi = {10.1101/457242},
+publisher = {Cold Spring Harbor Laboratory}, URL = {https://www.biorxiv.org/
+content/early/2018/10/30/457242}, eprint = {https://www.biorxiv.org/content/
+early/2018/10/30/457242.full.pdf}, journal = {bioRxiv}} ## License: This
+project is primarily licensed under the GNU Lesser General Public License v3.0.
+Note that the software is provided "as is", without warranty of any kind,
+express or implied. If you use the code or data, please cite us! Note, artwork
+(DeepLabCut logo) and images are copyrighted; please do not take or use these
+images without written permission. ## Versions: VERSION 2.2: Multi-animal pose
+estimation, identification, and tracking with DeepLabCut is supported (as well
+as single-animal projects). VERSION 2.0-2.1: This is the **Python package** of
+[DeepLabCut](https://www.nature.com/articles/s41593-018-0209-y) that was
+originally released in Oct 2018 with our [Nature Protocols](https://doi.org/
+10.1038/s41596-019-0176-0) paper (preprint [here](https://www.biorxiv.org/
+content/10.1101/476531v1)). This package includes graphical user interfaces to
+label your data, and take you from data set creation to automatic behavioral
+analysis. It also introduces an active learning framework to efficiently use
+DeepLabCut on large experimental projects, and data augmentation tools that
+improve network performance, especially in challenging cases (see [panel b]
+(https://camo.githubusercontent.com/77c92f6b89d44ca758d815bdd7e801247437060b/
 68747470733a2f2f737461746963312e73717561726573706163652e636f6d2f7374617469632f3537663664353163396637343536366635356563663237312f742f3563336663316336373538643436393530636537656563372f313534373638323338333539352f636865657461682e706e673f666f726d61743d37353077)).
 VERSION 1.0: The initial, Nature Neuroscience version of [DeepLabCut](https://
 www.nature.com/articles/s41593-018-0209-y) can be found in the history of git,
 or here: https://github.com/DeepLabCut/DeepLabCut/releases/tag/1.11 ## News
-(and in the news): - August 2021: 2.2 becomes the new stable release for
-DeepLabCut. - July 2021: Docs are now at https://deeplabcut.github.io/
-DeepLabCut and we now include TensorFlow 2 support! - May 2021: DeepLabCut hit
-200,000 downloads! Also, Our preprint on 2.2, multi-animal DeepLabCut is
-released! - Jan 2021: [Pretraining boosts out-of-domain robustness for pose
-estimation](https://openaccess.thecvf.com/content/WACV2021/html/
-Mathis_Pretraining_Boosts_Out-of-
+(and in the news): - August 2022: DeepLabCut hit 400,000 downloads! - August
+2021: 2.2 becomes the new stable release for DeepLabCut. - July 2021: Docs are
+now at https://deeplabcut.github.io/DeepLabCut and we now include TensorFlow 2
+support! - May 2021: DeepLabCut hit 200,000 downloads! Also, Our preprint on
+2.2, multi-animal DeepLabCut is released! - Jan 2021: [Pretraining boosts out-
+of-domain robustness for pose estimation](https://openaccess.thecvf.com/
+content/WACV2021/html/Mathis_Pretraining_Boosts_Out-of-
 Domain_Robustness_for_Pose_Estimation_WACV_2021_paper.html) published in the
 IEEE Winter Conference on Applications of Computer Vision. We also added
 EfficientNet backbones to DeepLabCut, those are best trained with cosine decay
 (see paper). To use them, just pass "`efficientnet-b0`" to "`efficientnet-b6`"
 when creating the trainingset! - Dec 2020: We released a real-time package that
 allows for online pose estimation and real-time feedback. See
 [DLClive.deeplabcut.org](http://DLClive.deeplabcut.org). - 5/22 2020: We
```

### Comparing `deeplabcut-2.3rc2/deeplabcut.egg-info/SOURCES.txt` & `deeplabcut-2.3rc3/deeplabcut.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 AUTHORS
 LICENSE
+NOTICE.yml
 README.md
 setup.py
 deeplabcut/__init__.py
 deeplabcut/__main__.py
 deeplabcut/cli.py
 deeplabcut/inference_cfg.yaml
 deeplabcut/pose_cfg.yaml
```

### Comparing `deeplabcut-2.3rc2/setup.py` & `deeplabcut-2.3rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 with open("README.md", encoding="utf-8", errors="replace") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="deeplabcut",
-    version="2.3rc2",
+    version="2.3rc3",
     author="A. & M. Mathis Labs",
     author_email="alexander@deeplabcut.org",
     description="Markerless pose-estimation of user-defined features with deep learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DeepLabCut/DeepLabCut",
     install_requires=[
@@ -53,14 +53,15 @@
             "qdarkstyle==3.1",
             "napari-deeplabcut",
         ],
         "openvino": ["openvino-dev==2022.1.0"],
         "docs": ["numpydoc"],
         "tf": ["tensorflow>=2.0"],
         "apple_mchips": [],
+        "modelzoo": ["huggingface_hub"],
     },
     scripts=["deeplabcut/pose_estimation_tensorflow/models/pretrained/download.sh"],
     packages=setuptools.find_packages(),
     data_files=[
         (
             "deeplabcut",
             [
```

