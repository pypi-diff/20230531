# Comparing `tmp/Gammalearn-0.8.tar.gz` & `tmp/Gammalearn-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Gammalearn-0.8.tar", last modified: Thu Jan 20 14:32:12 2022, max compression
+gzip compressed data, was "Gammalearn-0.9.tar", last modified: Thu May  5 20:13:09 2022, max compression
```

## Comparing `Gammalearn-0.8.tar` & `Gammalearn-0.9.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-20 14:32:12.879533 Gammalearn-0.8/
--rw-rw-rw-   0 root         (0) root         (0)     1643 2022-01-20 12:21:53.000000 Gammalearn-0.8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     3218 2022-01-20 14:31:53.000000 Gammalearn-0.8/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-20 14:32:12.839533 Gammalearn-0.8/Docker/
--rw-rw-rw-   0 root         (0) root         (0)      341 2022-01-20 12:21:53.000000 Gammalearn-0.8/Docker/Dockerfile
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-20 14:32:12.842533 Gammalearn-0.8/Gammalearn.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5318 2022-01-20 14:32:12.000000 Gammalearn-0.8/Gammalearn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1921 2022-01-20 14:32:12.000000 Gammalearn-0.8/Gammalearn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-20 14:32:12.000000 Gammalearn-0.8/Gammalearn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2022-01-20 14:32:12.000000 Gammalearn-0.8/Gammalearn.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      158 2022-01-20 14:32:12.000000 Gammalearn-0.8/Gammalearn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-01-20 14:32:12.000000 Gammalearn-0.8/Gammalearn.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1068 2022-01-20 12:21:53.000000 Gammalearn-0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5318 2022-01-20 14:32:12.879533 Gammalearn-0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4781 2022-01-20 12:58:16.000000 Gammalearn-0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2679 2022-01-20 12:58:16.000000 Gammalearn-0.8/codemeta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-20 14:32:12.847533 Gammalearn-0.8/docs/
--rw-rw-rw-   0 root         (0) root         (0)     2702 2022-01-20 12:21:53.000000 Gammalearn-0.8/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-01-20 12:21:53.000000 Gammalearn-0.8/docs/doc_requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     2050 2022-01-20 12:21:53.000000 Gammalearn-0.8/docs/gammalearn.rst
--rw-rw-rw-   0 root         (0) root         (0)      734 2022-01-20 12:21:53.000000 Gammalearn-0.8/docs/gammalearn.tests.rst
--rw-rw-rw-   0 root         (0) root         (0)      460 2022-01-20 12:21:53.000000 Gammalearn-0.8/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      477 2022-01-20 12:58:16.000000 Gammalearn-0.8/environment.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-20 14:32:12.855533 Gammalearn-0.8/gammalearn/
--rw-rw-rw-   0 root         (0) root         (0)      319 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      373 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/_dev_version.py
--rw-r--r--   0 root         (0) root         (0)       19 2022-01-20 14:32:12.000000 Gammalearn-0.8/gammalearn/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    27254 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/callbacks.py
--rw-rw-rw-   0 root         (0) root         (0)       45 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/constants.py
--rwxrwxrwx   0 root         (0) root         (0)    21284 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/criterions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-20 14:32:12.859533 Gammalearn-0.8/gammalearn/data/
--rw-rw-rw-   0 root         (0) root         (0)   521000 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/data/camera_parameters.h5
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-20 14:32:12.862533 Gammalearn-0.8/gammalearn/data/example_settings/
--rw-rw-rw-   0 root         (0) root         (0)    13219 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_autoencoder.py
--rw-rw-rw-   0 root         (0) root         (0)    13196 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_file_spawn.py
--rw-rw-rw-   0 root         (0) root         (0)    14268 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_profiler.py
--rw-rw-rw-   0 root         (0) root         (0)    13098 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_square_pixels.py
--rw-rw-rw-   0 root         (0) root         (0)    13457 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_square_pixels_bicubic.py
--rw-rw-rw-   0 root         (0) root         (0)    13809 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_square_pixels_over.py
--rw-rw-rw-   0 root         (0) root         (0)    13252 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_test_MC.py
--rw-rw-rw-   0 root         (0) root         (0)    13976 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_test_real.py
--rw-rw-rw-   0 root         (0) root         (0)    13590 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_train_MC.py
--rw-rw-rw-   0 root         (0) root         (0)    13154 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_val.py
--rwxrwxrwx   0 root         (0) root         (0)    35696 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/data/nets.py
--rw-rw-rw-   0 root         (0) root         (0)    44648 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/data/nice_lst.npy
--rw-rw-rw-   0 root         (0) root         (0)     9190 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/data_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)    26161 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/datasets.py
--rwxrwxrwx   0 root         (0) root         (0)    33586 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/experiment_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     1648 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     2056 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    31353 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/open_blackbox.py
--rw-rw-rw-   0 root         (0) root         (0)     4597 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/optimizers.py
--rw-rw-rw-   0 root         (0) root         (0)     6630 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/steps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-20 14:32:12.864533 Gammalearn-0.8/gammalearn/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6773 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/tests/test_criterions.py
--rw-rw-rw-   0 root         (0) root         (0)    20623 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/tests/test_datasets.py
--rw-rw-rw-   0 root         (0) root         (0)    10056 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/tests/test_version.py
--rw-rw-rw-   0 root         (0) root         (0)    25998 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2022-01-20 12:21:53.000000 Gammalearn-0.8/gammalearn/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-20 14:32:12.864533 Gammalearn-0.8/notebook/
--rw-rw-rw-   0 root         (0) root         (0)    14708 2022-01-20 12:21:53.000000 Gammalearn-0.8/notebook/geometry_convert.ipynb
--rw-r--r--   0 root         (0) root         (0)       38 2022-01-20 14:32:12.879533 Gammalearn-0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1602 2022-01-20 12:21:53.000000 Gammalearn-0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-20 14:32:12.866533 Gammalearn-0.8/share/
--rw-rw-rw-   0 root         (0) root         (0)     5415 2022-01-20 12:21:53.000000 Gammalearn-0.8/share/create_camera_parameter_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-20 14:32:12.834533 Gammalearn-0.8/share/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-20 14:32:12.872533 Gammalearn-0.8/share/data/MC_data/
--rw-rw-rw-   0 root         (0) root         (0)   731132 2022-01-20 12:21:53.000000 Gammalearn-0.8/share/data/MC_data/dl1_gamma_example.h5
--rw-rw-rw-   0 root         (0) root         (0)   734886 2022-01-20 12:21:53.000000 Gammalearn-0.8/share/data/MC_data/dl1_proton_example.h5
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-20 14:32:12.876533 Gammalearn-0.8/share/data/real_data/
--rw-rw-rw-   0 root         (0) root         (0)  1064866 2022-01-20 12:21:53.000000 Gammalearn-0.8/share/data/real_data/dl1_realdata_example.h5
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 20:13:09.971770 Gammalearn-0.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1666 2022-05-05 15:23:21.000000 Gammalearn-0.9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3212 2022-05-05 19:28:16.000000 Gammalearn-0.9/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      341 2022-05-05 15:23:21.000000 Gammalearn-0.9/Dockerfile
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 20:13:09.919771 Gammalearn-0.9/Gammalearn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5318 2022-05-05 20:13:09.000000 Gammalearn-0.9/Gammalearn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2088 2022-05-05 20:13:09.000000 Gammalearn-0.9/Gammalearn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-05-05 20:13:09.000000 Gammalearn-0.9/Gammalearn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2022-05-05 20:13:09.000000 Gammalearn-0.9/Gammalearn.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2022-05-05 20:13:09.000000 Gammalearn-0.9/Gammalearn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2022-05-05 20:13:09.000000 Gammalearn-0.9/Gammalearn.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2022-05-05 14:49:21.000000 Gammalearn-0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5318 2022-05-05 20:13:09.970770 Gammalearn-0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4781 2022-05-05 14:49:21.000000 Gammalearn-0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     3072 2022-05-05 16:48:43.000000 Gammalearn-0.9/codemeta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 20:13:09.921771 Gammalearn-0.9/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     2702 2022-05-05 14:49:21.000000 Gammalearn-0.9/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      120 2022-05-05 14:49:21.000000 Gammalearn-0.9/docs/doc_requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2050 2022-05-05 14:49:21.000000 Gammalearn-0.9/docs/gammalearn.rst
+-rw-rw-rw-   0 root         (0) root         (0)      734 2022-05-05 14:49:21.000000 Gammalearn-0.9/docs/gammalearn.tests.rst
+-rw-rw-rw-   0 root         (0) root         (0)      460 2022-05-05 14:49:21.000000 Gammalearn-0.9/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      475 2022-05-05 15:23:21.000000 Gammalearn-0.9/environment.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 20:13:09.933771 Gammalearn-0.9/gammalearn/
+-rw-rw-rw-   0 root         (0) root         (0)      319 2022-05-05 14:49:21.000000 Gammalearn-0.9/gammalearn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      373 2022-05-05 14:49:21.000000 Gammalearn-0.9/gammalearn/_dev_version.py
+-rw-r--r--   0 root         (0) root         (0)       19 2022-05-05 20:13:09.000000 Gammalearn-0.9/gammalearn/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    28380 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/callbacks.py
+-rw-rw-rw-   0 root         (0) root         (0)       66 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/constants.py
+-rwxrwxrwx   0 root         (0) root         (0)    21408 2022-05-05 14:49:21.000000 Gammalearn-0.9/gammalearn/criterions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 20:13:09.940770 Gammalearn-0.9/gammalearn/data/
+-rw-rw-rw-   0 root         (0) root         (0)   521000 2022-05-05 14:49:21.000000 Gammalearn-0.9/gammalearn/data/camera_parameters.h5
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 20:13:09.945770 Gammalearn-0.9/gammalearn/data/example_settings/
+-rw-rw-rw-   0 root         (0) root         (0)    12366 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_autoencoder.py
+-rw-rw-rw-   0 root         (0) root         (0)    14056 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_clean_channel.py
+-rw-rw-rw-   0 root         (0) root         (0)    15305 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_domain_adaptation.py
+-rw-rw-rw-   0 root         (0) root         (0)    14164 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_file_spawn.py
+-rw-rw-rw-   0 root         (0) root         (0)    15069 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_profiler.py
+-rw-rw-rw-   0 root         (0) root         (0)    14032 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_square_pixels.py
+-rw-rw-rw-   0 root         (0) root         (0)    14104 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_square_pixels_bicubic.py
+-rw-rw-rw-   0 root         (0) root         (0)    14303 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_square_pixels_over.py
+-rw-rw-rw-   0 root         (0) root         (0)    13961 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_test_MC.py
+-rw-rw-rw-   0 root         (0) root         (0)    14843 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_test_real.py
+-rw-rw-rw-   0 root         (0) root         (0)    14179 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_train_MC.py
+-rw-rw-rw-   0 root         (0) root         (0)    12878 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_val.py
+-rwxrwxrwx   0 root         (0) root         (0)    38683 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/data/nets.py
+-rw-rw-rw-   0 root         (0) root         (0)    44648 2022-05-05 14:49:21.000000 Gammalearn-0.9/gammalearn/data/nice_lst.npy
+-rw-rw-rw-   0 root         (0) root         (0)     9808 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/data_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)    28376 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/datasets.py
+-rwxrwxrwx   0 root         (0) root         (0)    35206 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/experiment_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1648 2022-05-05 14:49:21.000000 Gammalearn-0.9/gammalearn/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     2056 2022-05-05 14:49:21.000000 Gammalearn-0.9/gammalearn/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    31353 2022-05-05 14:49:21.000000 Gammalearn-0.9/gammalearn/open_blackbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     4871 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/optimizers.py
+-rw-rw-rw-   0 root         (0) root         (0)    10045 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/steps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 20:13:09.947770 Gammalearn-0.9/gammalearn/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-05 14:49:21.000000 Gammalearn-0.9/gammalearn/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6897 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/tests/test_criterions.py
+-rw-rw-rw-   0 root         (0) root         (0)    20623 2022-05-05 14:49:21.000000 Gammalearn-0.9/gammalearn/tests/test_datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)     2509 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/tests/test_nets.py
+-rw-rw-rw-   0 root         (0) root         (0)    11053 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2022-05-05 14:49:21.000000 Gammalearn-0.9/gammalearn/tests/test_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    27636 2022-05-05 15:23:21.000000 Gammalearn-0.9/gammalearn/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2022-05-05 14:49:21.000000 Gammalearn-0.9/gammalearn/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 20:13:09.948770 Gammalearn-0.9/notebook/
+-rw-rw-rw-   0 root         (0) root         (0)    14708 2022-05-05 14:49:21.000000 Gammalearn-0.9/notebook/geometry_convert.ipynb
+-rw-r--r--   0 root         (0) root         (0)       38 2022-05-05 20:13:09.971770 Gammalearn-0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1602 2022-05-05 15:23:21.000000 Gammalearn-0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 20:13:09.950770 Gammalearn-0.9/share/
+-rw-rw-rw-   0 root         (0) root         (0)     5415 2022-05-05 14:49:21.000000 Gammalearn-0.9/share/create_camera_parameter_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 20:13:09.907771 Gammalearn-0.9/share/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 20:13:09.956771 Gammalearn-0.9/share/data/MC_data/
+-rw-rw-rw-   0 root         (0) root         (0)   731132 2022-05-05 14:49:21.000000 Gammalearn-0.9/share/data/MC_data/dl1_gamma_example.h5
+-rw-rw-rw-   0 root         (0) root         (0)   734886 2022-05-05 14:49:21.000000 Gammalearn-0.9/share/data/MC_data/dl1_proton_example.h5
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-05 20:13:09.959770 Gammalearn-0.9/share/data/real_data/
+-rw-rw-rw-   0 root         (0) root         (0)  1064866 2022-05-05 14:49:21.000000 Gammalearn-0.9/share/data/real_data/dl1_realdata_example.h5
```

### Comparing `Gammalearn-0.8/.gitignore` & `Gammalearn-0.9/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 parts/
 sdist/
 var/
 wheels/
 *.egg-info/
 .installed.cfg
 *.egg
+gammalearn/_version.py
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
```

### Comparing `Gammalearn-0.8/.gitlab-ci.yml` & `Gammalearn-0.9/.gitlab-ci.yml`

 * *Files 17% similar despite different names*

```diff
@@ -24,14 +24,16 @@
         - gammalearn experiment_settings_test_real.py
         - gammalearn experiment_settings_square_pixels.py
         - gammalearn experiment_settings_square_pixels_over.py
         - gammalearn experiment_settings_square_pixels_bicubic.py
         - gammalearn experiment_settings_file_spawn.py
         - gammalearn experiment_settings_profiler.py
         - gammalearn experiment_settings_autoencoder.py
+        - gammalearn experiment_settings_domain_adaptation.py
+        - gammalearn experiment_settings_clean_channel.py
 
     artifacts:
       reports:
         cobertura: coverage.xml
 
 
 pages:
@@ -45,45 +47,40 @@
     artifacts:
       paths:
         - public
     only:
       - master
 
 
-build_docker:
-  stage: build_container
-  image: docker:20.10.7
-  services:
-    - docker:20.10.7-dind
-  before_script:
-    - cat /etc/os-release
-    - apk add git
-    - export LAST_RELEASE=`git ls-remote --tags --refs --sort="v:refname" $CI_PROJECT_URL.git | tail -n1 | sed 's/.*\///'`
-    - echo $LAST_RELEASE
-  script:
-    - echo "user $CI_REGISTRY_USER"
-    - echo "registry $CI_REGISTRY"
-    - echo "$CI_REGISTRY_PASSWORD" | docker login -u "$CI_REGISTRY_USER" "$CI_REGISTRY" --password-stdin
-    - docker build -t $CI_REGISTRY_IMAGE:$LAST_RELEASE Docker
-    - docker push $CI_REGISTRY_IMAGE:$LAST_RELEASE
-    - docker tag $CI_REGISTRY_IMAGE:$LAST_RELEASE $CI_REGISTRY_IMAGE:latest
-    - docker push $CI_REGISTRY_IMAGE:latest
-  only:
-    - tags
+# memory issues to solve: https://gitlab.in2p3.fr/gammalearn/gammalearn/-/jobs/480738
+# build_docker:
+#   stage: build_container
+#   image:
+#     name: gcr.io/kaniko-project/executor:debug
+#     entrypoint: [""]
+#   script:
+#     - mkdir -p /kaniko/.docker
+#     - echo "{\"auths\":{\"${CI_REGISTRY}\":{\"auth\":\"$(printf "%s:%s" "${CI_REGISTRY_USER}" "${CI_REGISTRY_PASSWORD}" | base64 | tr -d '\n')\"}}}" > /kaniko/.docker/config.json
+#     - >-
+#       /kaniko/executor
+#       --context "${CI_PROJECT_DIR}"
+#       --dockerfile "${CI_PROJECT_DIR}/Dockerfile"
+#       --destination "${CI_REGISTRY_IMAGE}:${CI_COMMIT_TAG}"
+#       --destination "${CI_REGISTRY_IMAGE}:latest"
+#   rules:
+#     - if: $CI_COMMIT_TAG
 
 
 deploy_zenodo:
   stage: deploy_zenodo
-  image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:v0.3.3
+  image: gitlab-registry.in2p3.fr/escape2020/wp3/eossr:v0.6
   before_script:
-    - eossr-check-connection-zenodo --token $ZENODO_TOKEN --sandbox False -p $CI_PROJECT_DIR
+    - eossr-check-connection-zenodo --token $ZENODO_TOKEN -p $CI_PROJECT_DIR
   script:
-    - gitlab_prepare_upload_zenodo.sh $CI_PROJECT_NAME $CI_PROJECT_DIR zenodo_build
-    - ls zenodo_build
-    - eossr-upload-repository -t $ZENODO_TOKEN -s False -i zenodo_build -id $ZENODO_PROJECT_ID
+    - eossr-upload-repository -t $ZENODO_TOKEN -i $CI_PROJECT_DIR --archive-name $CI_PROJECT_NAME.zip -id $ZENODO_PROJECT_ID
   only:
     - tags
 
 
 pypi_publish:
   stage: pypi_publish
   image: python:3.8
```

### Comparing `Gammalearn-0.8/Gammalearn.egg-info/PKG-INFO` & `Gammalearn-0.9/Gammalearn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Gammalearn
-Version: 0.8
+Version: 0.9
 Summary: A framework to easily train deep learning model on Imaging Atmospheric Cherenkov Telescopes data
 Home-page: https://gitlab.lapp.in2p3.fr/GammaLearn/GammaLearn
 Author: M. Jacquemont, T. Vuillaume
 Author-email: jacquemont@lapp.in2p3.fr
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Gammalearn-0.8/Gammalearn.egg-info/SOURCES.txt` & `Gammalearn-0.9/Gammalearn.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .gitignore
 .gitlab-ci.yml
+Dockerfile
 LICENSE
 README.md
 codemeta.json
 environment.yml
 setup.py
-Docker/Dockerfile
 Gammalearn.egg-info/PKG-INFO
 Gammalearn.egg-info/SOURCES.txt
 Gammalearn.egg-info/dependency_links.txt
 Gammalearn.egg-info/entry_points.txt
 Gammalearn.egg-info/requires.txt
 Gammalearn.egg-info/top_level.txt
 docs/conf.py
@@ -33,26 +33,29 @@
 gammalearn/steps.py
 gammalearn/utils.py
 gammalearn/version.py
 gammalearn/data/camera_parameters.h5
 gammalearn/data/nets.py
 gammalearn/data/nice_lst.npy
 gammalearn/data/example_settings/experiment_settings_autoencoder.py
+gammalearn/data/example_settings/experiment_settings_clean_channel.py
+gammalearn/data/example_settings/experiment_settings_domain_adaptation.py
 gammalearn/data/example_settings/experiment_settings_file_spawn.py
 gammalearn/data/example_settings/experiment_settings_profiler.py
 gammalearn/data/example_settings/experiment_settings_square_pixels.py
 gammalearn/data/example_settings/experiment_settings_square_pixels_bicubic.py
 gammalearn/data/example_settings/experiment_settings_square_pixels_over.py
 gammalearn/data/example_settings/experiment_settings_test_MC.py
 gammalearn/data/example_settings/experiment_settings_test_real.py
 gammalearn/data/example_settings/experiment_settings_train_MC.py
 gammalearn/data/example_settings/experiment_settings_val.py
 gammalearn/tests/__init__.py
 gammalearn/tests/test_criterions.py
 gammalearn/tests/test_datasets.py
+gammalearn/tests/test_nets.py
 gammalearn/tests/test_utils.py
 gammalearn/tests/test_version.py
 notebook/geometry_convert.ipynb
 share/create_camera_parameter_file.py
 share/data/MC_data/dl1_gamma_example.h5
 share/data/MC_data/dl1_proton_example.h5
 share/data/real_data/dl1_realdata_example.h5
```

### Comparing `Gammalearn-0.8/LICENSE` & `Gammalearn-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Gammalearn-0.8/PKG-INFO` & `Gammalearn-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Gammalearn
-Version: 0.8
+Version: 0.9
 Summary: A framework to easily train deep learning model on Imaging Atmospheric Cherenkov Telescopes data
 Home-page: https://gitlab.lapp.in2p3.fr/GammaLearn/GammaLearn
 Author: M. Jacquemont, T. Vuillaume
 Author-email: jacquemont@lapp.in2p3.fr
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Gammalearn-0.8/README.md` & `Gammalearn-0.9/README.md`

 * *Files identical despite different names*

### Comparing `Gammalearn-0.8/codemeta.json` & `Gammalearn-0.9/codemeta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9337474120082815%*

 * *Differences: {"'author'": "{insert: [(2, OrderedDict([('@type', 'Person'), ('@id', "*

 * *             "'https://orcid.org/0000-0002-5221-0240'), ('givenName', 'Michaël'), ('familyName', "*

 * *             '"Dell\'aiera"), (\'email\', \'michael.dellaiera@lapp.in2p3.fr\'), (\'affiliation\', '*

 * *             "OrderedDict([('@type', 'Organization'), ('name', 'Univ. Savoie Mont-Blanc, CNRS, "*

 * *             "LAPP')]))]))]}",*

 * * "'downloadUrl'": "'https://gitlab.in2p3.fr/gammalearn/gammalearn/-/archive/v0.9/gammalearn-v0.9.tar.gz'",*

 * * "'key […]*

```diff
@@ -20,14 +20,25 @@
             "affiliation": {
                 "@type": "Organization",
                 "name": "Univ. Savoie Mont-Blanc, CNRS, LAPP"
             },
             "email": "thomas.vuillaume@lapp.in2p3.fr",
             "familyName": "Vuillaume",
             "givenName": "Thomas"
+        },
+        {
+            "@id": "https://orcid.org/0000-0002-5221-0240",
+            "@type": "Person",
+            "affiliation": {
+                "@type": "Organization",
+                "name": "Univ. Savoie Mont-Blanc, CNRS, LAPP"
+            },
+            "email": "michael.dellaiera@lapp.in2p3.fr",
+            "familyName": "Dell'aiera",
+            "givenName": "Micha\u00ebl"
         }
     ],
     "codeRepository": "git+https://gitlab.in2p3.fr/gammalearn/gammalearn.git",
     "contIntegration": "https://gitlab.in2p3.fr/gammalearn/gammalearn/-/pipelines",
     "contributor": [
         {
             "@id": "https://orcid.org/0000-0003-1536-9241",
@@ -42,32 +53,31 @@
         }
     ],
     "dateCreated": "2017-07-01",
     "dateModified": "2022-01-20",
     "datePublished": "2022-01-20",
     "description": "GammaLearn is a collaborative project to apply deep learning to the analysis of low-level Imaging Atmospheric Cherenkov Telescopes such as CTA.\nIt provides a framework to easily train and apply models from a configuration file.\nLearn more at https://purl.org/gammalearn ",
     "developmentStatus": "active",
-    "downloadUrl": "https://gitlab.in2p3.fr/gammalearn/gammalearn/-/archive/v0.8/gammalearn-v0.8.tar.gz",
+    "downloadUrl": "https://gitlab.in2p3.fr/gammalearn/gammalearn/-/archive/v0.9/gammalearn-v0.9.tar.gz",
     "funder": {
         "@type": "Organization",
         "name": "European Union\u2019s Horizon 2020 research and innovation programme"
     },
     "funding": "824064",
     "issueTracker": "https://gitlab.in2p3.fr/gammalearn/gammalearn/-/issues",
     "keywords": [
         "deep learning",
-        "telescope",
-        "cherenkov",
-        "iact",
+        "machine learning",
+        "Gamma-ray telescopes",
         "cta"
     ],
     "license": "https://spdx.org/licenses/MIT",
     "name": "GammaLearn",
     "programmingLanguage": [
         "Python 3"
     ],
     "relatedLink": [
         "https://purl.org/gammalearn"
     ],
     "releaseNotes": "",
-    "version": "v0.8"
+    "version": "v0.9"
 }
```

### Comparing `Gammalearn-0.8/docs/conf.py` & `Gammalearn-0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Gammalearn-0.8/docs/gammalearn.rst` & `Gammalearn-0.9/docs/gammalearn.rst`

 * *Files identical despite different names*

### Comparing `Gammalearn-0.8/docs/gammalearn.tests.rst` & `Gammalearn-0.9/docs/gammalearn.tests.rst`

 * *Files identical despite different names*

### Comparing `Gammalearn-0.8/gammalearn/callbacks.py` & `Gammalearn-0.9/gammalearn/callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import pandas as pd
 import tables
 from ctapipe.instrument import CameraGeometry
 from ctapipe.visualization import CameraDisplay
 from ctapipe.io import HDF5TableWriter
 from lstchain.io import write_dl2_dataframe
 from lstchain.reco.utils import add_delta_t_key
+from lstchain.io.io import dl1_params_lstcam_key
 from PIL import Image
 from torchvision import transforms
 import torchvision.utils as t_utils
 from indexedconv.engine import IndexedConv
 from indexedconv.utils import create_index_matrix, img2mat, pool_index_matrix, build_hexagonal_position
 from astropy.table import Table
 
@@ -51,15 +52,21 @@
     Returns
     -------
     """
     def on_train_epoch_end(self, trainer, pl_module):
         if isinstance(pl_module.experiment.compute_loss, criterions.MultilossBalancing):
             log_vars = pl_module.experiment.compute_loss.log_vars
             vars_dict = {}
-            for i, task in enumerate(pl_module.experiment.targets.keys()):
+
+            targets = pl_module.experiment.targets.copy()
+            for k, v in targets.items():
+                if not v['mt_balancing']:
+                    targets.pop(k)
+
+            for i, task in enumerate(targets.keys()):
                 vars_dict['Logvar_' + task] = log_vars[i].detach().cpu()
             pl_module.log('Log_vars', vars_dict, on_epoch=True, on_step=False)
 
 
 class LogGradNormWeights(Callback):
     """
     Callback to send GradNorm weights to logger
@@ -163,14 +170,17 @@
     def on_train_batch_end(self, trainer, pl_module, outputs, batch, batch_idx):
         for hook in self.hooks:
             hook.remove()
 
 
 def make_linear_gradient_logger(pl_module, name):
     def log_grad(m, grad_input, grad_output):
+        # if torch.isnan(grad_input[0].data.cpu()).any():
+        #     print(name)
+        #     print(grad_input[0].data.cpu())
         pl_module.logger.experiment.add_histogram(name + 'grad_in', grad_input[0].data.cpu(),
                                                   bins='tensorflow', global_step=pl_module.current_epoch)
     return log_grad
 
 
 class LogLinearGradient(Callback):
     """
@@ -396,59 +406,62 @@
 
         Returns
         -------
         """
     def on_test_end(self, trainer, pl_module):
 
         # Retrieve test data
-        merged_outputs = utils.merge_list_of_dict(pl_module.test_data['output'])
-        merged_dl1_params = utils.merge_list_of_dict(pl_module.test_data['dl1_params'])
-
-        for k, v in merged_outputs.items():
-            merged_outputs[k] = torch.cat(v).detach().to('cpu').numpy()
-        for k, v in merged_dl1_params.items():
-            merged_dl1_params[k] = torch.cat(v).detach().to('cpu').numpy()
+        merged_outputs = pd.concat([pd.DataFrame(utils.prepare_dict_of_tensors(output))
+                                    for output in pl_module.test_data['output']], ignore_index=True )
+        merged_dl1_params = pd.concat([pd.DataFrame(utils.prepare_dict_of_tensors(dl1))
+                                       for dl1 in pl_module.test_data['dl1_params']], ignore_index=True )
 
         particle_dict = pl_module.experiment.dataset_parameters['particle_dict']
         swapped_particle_dict = {v: k for k, v in particle_dict.items()}
 
         # Prepare data
-        data_pd = pd.DataFrame()
-        for param_name, param_value in merged_dl1_params.items():
-            if param_name in ['mc_core_x', 'mc_core_y', 'tel_pos_x', 'tel_pos_y', 'tel_pos_z', 'mc_x_max']:
-                data_pd[param_name] = 1000 * param_value
-            else:
-                data_pd[param_name] = param_value
-        for target, output in merged_outputs.items():
+        for param_name in ['mc_core_x', 'mc_core_y', 'tel_pos_x', 'tel_pos_y', 'tel_pos_z', 'mc_x_max']:
+            if param_name in merged_dl1_params.columns:
+                merged_dl1_params[param_name] *= 1000
+
+        dl2_params = merged_dl1_params.copy(deep=True)
+
+        for target in merged_outputs.columns:
             if target == 'energy':
-                data_pd['reco_energy'] = 10 ** output
+                dl2_params['reco_energy'] = 10 ** merged_outputs[target]
             if target == 'xmax':
-                data_pd['reco_x_max'] = output * 1000
+                dl2_params['reco_x_max'] = merged_outputs[target] * 1000
             if target == 'impact':
-                data_pd['reco_core_x'] = output[:, 0] * 1000
-                data_pd['reco_core_y'] = output[:, 1] * 1000
+                dl2_params[['reco_core_x', 'reco_core_y']] = pd.DataFrame(merged_outputs[target].tolist(),
+                                                                          index=dl2_params.index)
+                dl2_params['reco_core_x'] *= 1000
+                dl2_params['reco_core_y'] *= 1000
                 if pl_module.experiment.dataset_parameters['group_by'] == 'image':
-                    data_pd['reco_core_x'] += data_pd['tel_pos_x']
-                    data_pd['reco_core_y'] += data_pd['tel_pos_y']
+                    dl2_params['reco_core_x'] += dl2_params['tel_pos_x']
+                    dl2_params['reco_core_y'] += dl2_params['tel_pos_y']
             if target == 'direction':
-                data_pd['reco_alt'] = output[:, 0]
-                data_pd['reco_az'] = output[:, 1]
+                dl2_params[['reco_alt', 'reco_az']] = pd.DataFrame(merged_outputs[target].tolist(),
+                                                                   index=dl2_params.index)
                 if pl_module.experiment.dataset_parameters['group_by'] == 'image':
-                    alt_tel = data_pd['mc_alt_tel'] if 'mc_alt_tel' in data_pd else data_pd['alt_tel']
-                    az_tel = data_pd['mc_az_tel'] if 'mc_az_tel' in data_pd else data_pd['az_tel']
-                    data_pd['reco_alt'] += alt_tel
-                    data_pd['reco_az'] += az_tel
+                    alt_tel = dl2_params['mc_alt_tel'] if 'mc_alt_tel' in dl2_params.columns else dl2_params['alt_tel']
+                    az_tel = dl2_params['mc_az_tel'] if 'mc_az_tel' in dl2_params.columns else dl2_params['az_tel']
+                    dl2_params['reco_alt'] += alt_tel
+                    dl2_params['reco_az'] += az_tel
             if target == 'class':
-                data_pd['reco_particle'] = np.vectorize(swapped_particle_dict.get)(np.argmax(output, 1))
-                data_pd['gammaness'] = np.exp(output[:, particle_dict[csts.GAMMA_ID]])
+                probabilities = torch.nn.functional.softmax(torch.tensor(list(merged_outputs[target].values)), dim=1)
+                dl2_params['reco_particle'] = np.vectorize(swapped_particle_dict.get)(np.argmax(probabilities, 1))
+                dl2_params['gammaness'] = probabilities[:, particle_dict[csts.GAMMA_ID]]
                 for k, v in particle_dict.items():
-                    data_pd['reco_proba_{}'.format(k)] = np.exp(output[:, v])
+                    dl2_params['reco_proba_{}'.format(k)] = probabilities[:, v]
+
+        if pl_module.experiment.data_module_test is None or pl_module.experiment.merge_test_datasets:
+            # Test has be done on the validation set or test dl1 have been merge in datasets by particle type
+
+            ratio = pl_module.experiment.validating_ratio if pl_module.experiment.data_module_test is None else 1.0
 
-        if pl_module.experiment.test_folders is None:
-            # Test has be done on the validation set
             # Retrieve MC config information
             mc_configuration = {}
 
             def fetch_dataset_info(d):
                 if isinstance(d, torch.utils.data.ConcatDataset):
                     for d_c in d.datasets:
                         fetch_dataset_info(d_c)
@@ -456,30 +469,29 @@
                     fetch_dataset_info(d.dataset)
                 elif issubclass(pl_module.experiment.dataset_class, dsets.BaseLSTDataset):
                     particle_type = d.dl1_params['mc_type'][0]
                     if particle_type not in mc_configuration:
                         mc_configuration[particle_type] = {'mc_energies': [], 'run_configs': []}
                     if d.simu:
                         mc_energies = d.trig_energies
-                        if not pl_module.experiment.split_by_file and pl_module.experiment.test_folders is None:
-                            np.random.shuffle(mc_energies)
-                            mc_energies = mc_energies[:int(len(mc_energies) * pl_module.experiment.validating_ratio)]
-                            d.run_config['mcheader']['num_showers'] *= pl_module.experiment.validating_ratio
+                        np.random.shuffle(mc_energies)
+                        mc_energies = mc_energies[:int(len(mc_energies) * ratio)]
+                        d.run_config['mcheader']['num_showers'] *= ratio
                         mc_configuration[particle_type]['mc_energies'].extend(mc_energies)
                     mc_configuration[particle_type]['run_configs'].append(d.run_config)
                 else:
                     pl_module.console_logger.error('Unknown dataset type, MC configuration cannot be retrieved')
                     raise ValueError
 
             for dataloader in trainer.test_dataloaders:
                 fetch_dataset_info(dataloader.dataset)
 
             # Write one file per particle type
             for mc_type in mc_configuration:
-                particle_mask = data_pd['mc_type'] == mc_type
+                particle_mask = merged_dl1_params['mc_type'] == mc_type
 
                 gb_file_path = pl_module.experiment.main_directory + '/' + pl_module.experiment.experiment_name + '/' + \
                                pl_module.experiment.experiment_name + '_' + str(mc_type) + '.h5'
                 if os.path.exists(gb_file_path):
                     os.remove(gb_file_path)
 
                 writer = HDF5TableWriter(gb_file_path)
@@ -549,15 +561,21 @@
                 pd.DataFrame(
                     {
                         'mc_trig_energies': np.array(mc_configuration[mc_type]['mc_energies'])
                     }
                 ).to_hdf(gb_file_path,
                          key='triggered_events')
 
-                data_pd[particle_mask].to_hdf(gb_file_path, key='data')
+                if mc_type == csts.REAL_DATA_ID:
+                    # Post dl2 ops for real data
+                    dl2_params = add_delta_t_key(dl2_params)
+
+                utils.write_dataframe(merged_dl1_params[particle_mask], outfile=gb_file_path,
+                                      table_path=dl1_params_lstcam_key)
+                write_dl2_dataframe(dl2_params[particle_mask], gb_file_path)
         else:
             # Prepare output
             if pl_module.experiment.dl2_path is not None:
                 output_dir = pl_module.experiment.dl2_path
             else:
                 output_dir = pl_module.experiment.main_directory + '/' + pl_module.experiment.experiment_name + '/dl2/'
             if not os.path.exists(output_dir):
@@ -565,15 +583,15 @@
             dataset = trainer.test_dataloaders[0].dataset
             output_name = os.path.basename(dataset.hdf5_file_path)
             output_name = output_name.replace('dl1', 'dl2')
             output_path = os.path.join(output_dir, output_name)
             if os.path.exists(output_path):
                 os.remove(output_path)
 
-            mc_type = dataset.dl1_params['mc_type'][0]
+            mc_type = merged_dl1_params['mc_type'][0]
             mc_energies = dataset.trig_energies
 
             metadata = dataset.run_config['metadata']
             metadata['mc_type'] = mc_type
             metadata['GAMMALEARN_VERSION'] = gl_version.__version__
             # Copy dl1 info except images
             with tables.open_file(dataset.hdf5_file_path) as dl1:
@@ -591,16 +609,16 @@
                             propindexes=False,
                             upgradeflavors=False,
                             allow_padding=True,
                         )
             # Write dl2 info
             if not dataset.simu:
                 # Post dl2 ops for real data
-                data_pd = add_delta_t_key(data_pd)
-            write_dl2_dataframe(data_pd, output_path)
+                dl2_params = add_delta_t_key(dl2_params)
+            write_dl2_dataframe(dl2_params, output_path)
             # Write metadata
             if mc_energies is not None:
                 pd.DataFrame({'mc_trig_energies': np.array(mc_energies)}).to_hdf(output_path, key='triggered_events')
             with tables.open_file(output_path, mode='a') as file:
                 for k, item in metadata.items():
                     if k in file.root._v_attrs and type(file.root._v_attrs) is list:
                         attribute = file.root._v_attrs[k].extend(metadata[k])
@@ -637,15 +655,15 @@
             if param_name in ['mc_core_x', 'mc_core_y', 'tel_pos_x', 'tel_pos_y', 'tel_pos_z', 'mc_x_max']:
                 data_pd[param_name] = 1000 * param_value
             else:
                 data_pd[param_name] = param_value
         for target, output in merged_outputs.items():
             data_pd[target] = output
 
-        if pl_module.experiment.test_folders is None:
+        if pl_module.experiment.data_module_test is None:
             # Test has be done on the validation set
             # Write one file
             output_path = os.path.join(pl_module.experiment.main_directory, pl_module.experiment.experiment_name,
                                        pl_module.experiment.experiment_name + '_ae_validation_results.h5')
             if os.path.exists(output_path):
                 os.remove(output_path)
         else:
```

### Comparing `Gammalearn-0.8/gammalearn/criterions.py` & `Gammalearn-0.9/gammalearn/criterions.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,15 +319,19 @@
 
     Returns
     -------
     The function to compute the loss
     """
     def __init__(self, targets, conditional=False, gamma_class=None, logvar_coeff=None, penalty=0):
         super(MultilossBalancing, self).__init__()
-        self.targets = targets
+        self.targets = targets.copy()
+        for k, v in self.targets.items():
+            if not v['mt_balancing']:
+                self.targets.pop(k)
+
         self.conditional = conditional
         self.penalty = penalty
         if self.conditional:
             assert 'class' in self.targets, 'The conditional loss is defined based on particle type'
             assert gamma_class is not None, 'To mask loss, one must provide the class of gamma'
         self.gamma_class = gamma_class
         self.log_vars = nn.Parameter(torch.rand(len(self.targets.keys())), requires_grad=True)
```

### Comparing `Gammalearn-0.8/gammalearn/data/camera_parameters.h5` & `Gammalearn-0.9/gammalearn/data/camera_parameters.h5`

 * *Files identical despite different names*

### Comparing `Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_autoencoder.py` & `Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_autoencoder.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from gammalearn.constants import GAMMA_ID, PROTON_ID, ELECTRON_ID
 from gammalearn.metrics import AUCMultiClass
 
 
 # Experiment settings
 main_directory = str(Path.home()) + '/gammalearn_experiments'  # TODO change directory if needed
 """str: mandatory, where the experiments are stored"""
-experiment_name = 'auto_encoder'
+experiment_name = 'test_install'
 """str: mandatory, the name of the experiment. Should be different
 for each experiment, except if one wants to resume an old experiment
 """
 info = ''
 """str: optional"""
 gpus = None
 """int or list: mandatory, the umber of gpus to use. If -1, run on all GPUS, 
@@ -46,159 +46,130 @@
 If save_every < 1, the model is not saved.
 If not provided, the model is not saved.
 """
 random_seed = 1
 """int: optional, the manual seed to make experiments more reproducible"""
 monitor_gpus = True
 """bool: optional, whether or not monitoring the gpu utilization"""
+particle_dict = {GAMMA_ID: 0,
+                 PROTON_ID: 1,
+                 # ELECTRON_ID: 2,
+                 }
+"""particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0"""
+targets = collections.OrderedDict({
+})
+"""dict: mandatory, defines for every objectives of the experiment
+the loss function and its weight
+"""
 
 dataset_class = dsets.MemoryLSTDataset
 # dataset_class = dsets.FileLSTDataset
 """Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
 loads images in memory, and FileLSTDataset that loads images from files during training.
 """
-dataset_parameters = {'camera_type': 'LST_LSTCam',
-                      'group_by': 'image',
-                      'use_time': True,
-                      'particle_dict': {GAMMA_ID: 0,
-                                        PROTON_ID: 1,
-                                        # ELECTRON_ID: 2,
-                                        },
-                      # 'subarray': [1],
-                      }
+dataset_parameters = {
+    'camera_type': 'LST_LSTCam',
+    'group_by': 'image',
+    'use_time': True,
+    'particle_dict': particle_dict,
+    'targets': list(targets.keys()),
+    # 'subarray': [1],
+}
 """dict: mandatory, the parameters of the dataset.
 camera_type is mandatory and can be:
 'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
 group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
 particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0, 
 proton (101) is class 1 and electron (1) is class 2.
 use_time (optional): whether or not to use time information
 subarray (optional): the list of telescope ids to select as a subarray
 """
-data_transform = {'data': [dsets.ResampleImage('bilinear_interpolation', (64, 64, 1)),
-                           ],
-                  'target': [
-                  ],
-                  }
-"""dict: optional, dictionary of transform functions to apply to the samples of data from the Dataset"""
 preprocessing_workers = 4
 """int: optional, the max number of workers to create dataset."""
 dataloader_workers = 4
 """int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
 mp_start_method = 'fork'
 """str: optional, the method to start new process in [fork, spawn]"""
-targets = collections.OrderedDict({
-    # 'energy': {
-    #     'output_shape': 1,
-    #     'loss': torch.nn.L1Loss(reduction='none'),
-    #     'loss_weight': 1,
-    #     'metrics': {
-    #         # 'functions': ,
-    #     }
-    # },
-    # 'impact': {
-    #     'output_shape': 2,
-    #     'loss': torch.nn.L1Loss(reduction='none'),
-    #     'loss_weight': 1,
-    #     'metrics': {}
-    # },
-    # 'direction': {
-    #     'output_shape': 2,
-    #     'loss': torch.nn.L1Loss(reduction='none'),
-    #     'loss_weight': 1,
-    #     'metrics': {}
-    # },
-    # 'class': {
-    #     'label_shape': 1,
-    #     'loss': criterions.nll_nn,
-    #     'loss_weight': 1,
-    #     'metrics': {
-    #         'Accuracy': Accuracy(threshold=0.5),
-    #         'AUC': AUCMultiClass(buffer_size=window_size,
-    #                              compute_on_step=True),
-    #         # 'AUC': AUROC(pos_label=dataset_parameters['particle_dict'][GAMMA_ID],
-    #         #              num_classes=len(dataset_parameters['particle_dict']),
-    #         #              compute_on_step=True
-    #         #              )
-    #     }
-    # },
-})
-"""dict: mandatory, defines for every objectives of the experiment
-the loss function and its weight
-"""
 
 # Net settings
 net_definition_file = utils.nets_definition_path()
 """str: mandatory, the file where to find the net definition to use"""
 # Load the network definitions module #
 spec = importlib.util.spec_from_file_location("nets", net_definition_file)
 nets = importlib.util.module_from_spec(spec)
 spec.loader.exec_module(nets)
 ########################################
-model_net = nets.ConvAutoEncoder
-"""nn.Module: mandatory, the network for the experiment. Is a class
-inheriting from nn.Module defining the operations of the network and
-the forward method to pass data through it
-"""
 net_parameters_dic = {
-    'num_channels': 2,
-    'n_features': 16,
-    'batchnorm': True,
-    'drop_rate': 0,
+    'model': nets.ConvAutoEncoder,
+    'parameters': {
+        'num_channels': 2,
+        'n_features': 16,
+        'batchnorm': True,
+        'drop_rate': 0,
+    }
 }
 """dict: mandatory, the parameters of the network. Depends on the
-network chosen
+network chosen. Must include at least a model and a parameters field.
 """
 # checkpoint_path = main_directory + '/test_install/checkpoint_epoch=3.ckpt'
 """str: optional, the path where to find the backup of the model to resume"""
 
 profiler = None
 # profiler = {'profiler': SimpleProfiler,
 #             'options': dict(extended=True)
 #             }
 """str: optional, the profiler to use"""
 
 ######################################################################################################################
 train = True
 """bool: mandatory, whether or not to train the model"""
 # Data settings
-train_folders = [
-    Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
-]  # TODO fill your folder path
-"""list: mandatory, the folders where to find the hdf5 data files"""
+data_module_train = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
+        ], # TODO fill your folder path
+        'image_filter': {
+            # utils.intensity_filter: {'intensity': [50, np.inf]},
+            # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': dsets.ResampleImage('bilinear_interpolation', (64, 64, 1)),
+        'target_transform': None
+    },
+    'target': {
+        'paths': [],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': None,
+        'target_transform': None
+    }
+}
+"""paths->list: mandatory, the folders where to find the hdf5 data files"""
+"""image_filter->dict: optional, the filter(s) to apply to the dataset at image level"""
+"""event_filter->dict: optional, the filter(s) to apply to the dataset"""
 
 validating_ratio = 0.2
 """float: mandatory, the ratio of data to create the validating set"""
 split_by_file = False
 """bool: optional, whether to split data at the file level or at the data level"""
 max_epochs = 4
 """int: mandatory, the maximum number of epochs for the experiment"""
 batch_size = 8
 """int: mandatory, the size of the mini-batch"""
-image_filter = {
-    # utils.intensity_filter: {'intensity': [50, np.inf]},
-    # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset at image level"""
-event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset"""
 
-# data_augment = {'function': dsets.augment_via_rotation,
-#                 'kwargs': {'thetas': [2 * math.pi / 3, 4 * math.pi / 3],
-#                            'num_workers': 8}
-#                 }
-"""dict: optional, dictionary describing the function to use for dataset augmentation"""
 # dataset_size = 2000
 """int: optional, the max size of the dataset"""
 # files_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 
 pin_memory = True
 """bool: optional, whether or not to pin memory in dataloader"""
@@ -220,15 +191,15 @@
     'network': optimizers.load_sgd,
     # 'loss_balancing': optimizers.load_adam
 }
 """dict: mandatory, the optimizers to use for the experiment.
 One may want to use several optimizers in case of GAN for example
 """
 optimizer_parameters = {
-    'network': {'learning_rate': 1e-4,
+    'network': {'lr': 1e-4,
                 'weight_decay': 1e-7,
                 'momentum': 0.9,
                 'nesterov': True
                 },
     # 'loss_balancing': {'learning_rate': 0.025,
     #                    'weight_decay': 1e-4,
     #                    },
@@ -244,29 +215,37 @@
 # training_step = steps.training_step_mt_gradient_penalty
 """function: mandatory, the function to compute the training step"""
 eval_step = steps.eval_step_ae
 """function: mandatory, the function to compute the validating step"""
 check_val_every_n_epoch = 1
 """int: optional, the interval in term of epoch for validating the model"""
 lr_schedulers = {
-    lr_scheduler.StepLR: {'network': {'gamma': 0.1,
-                                      'step_size': 10,
-                                      },
-                          },
-    # lr_scheduler.ReduceLROnPlateau: {'network': {'factor': 0.1,
-    #                                              'patience': 30,
-    #                                              },
-    #                                  },
-    # lr_scheduler.MultiStepLR: {'network': {'gamma': 0.1,
-    #                                        'milestones': [10, 15, 18],
-    #                                        },
-    #                            },
-    # lr_scheduler.ExponentialLR: {'network': {'gamma': 0.9,
-    #                                          },
-    #                              },
+    'network': {
+        lr_scheduler.StepLR: {
+            'gamma': 0.1,
+            'step_size': 10,
+        }
+    },
+    # 'network': {
+    #     lr_scheduler.ReduceLROnPlateau: {
+    #         'factor': 0.1,
+    #         'patience': 30,
+    #     }
+    # },
+    # 'network': {
+    #     lr_scheduler.MultiStepLR: {
+    #         'gamma': 0.1,
+    #         'milestones': [10, 15, 18],
+    #     }
+    # },
+    # 'network': {
+    #     lr_scheduler.ExponentialLR: {
+    #         'gamma': 0.9,
+    #     }
+    # },
 }
 """dict: optional, defines the learning rate schedulers"""
 # callbacks
 training_callbacks = [
     LogGradientNorm(),
     LogModelWeightNorm(),
     LogModelParameters(),
@@ -279,43 +258,61 @@
 """dict: list of callbacks
 """
 
 ######################################################################################################################
 # Testing settings
 test = True
 """bool: mandatory, whether or not to test the model at the end of training"""
+merge_test_datasets = False
+"""bool: optional, whether or not to merge test datasets"""
+data_module_test = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
+        ],
+        'image_filter': {
+            utils.intensity_filter: {'intensity': [10, np.inf]},
+            # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': dsets.ResampleImage('bilinear_interpolation', (64, 64, 1)),
+        'target_transform': None
+    },
+    'target': {
+        'paths': [],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': None,
+        'target_transform': None
+    }
+}
+"""
+dict: optional, must at least contain a non-empty 'source':{'paths:[]'}
+path->list of str: optional, the folders containing the hdf5 data files for the test
+image_filter->dict: optional, filter(s) to apply to the test set at image level
+event_filter->dict: optional, filter(s) to apply to the test set
+"""
+
 test_step = steps.test_step_ae
 """function: mandatory, the function to compute the validating step"""
-test_folders = [
-    Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
-]
-"""list of str: optional, the folders containing the hdf5 data files for the test
-"""
 dl2_path = ''
 """str: optional, path to store dl2 files"""
 test_dataset_parameters = {
     # 'subarray': [1],
 }
-"""dict: optional, the parameters of the dataset specific to the test operation.
-"""
-test_image_filter = {
-    utils.intensity_filter: {'intensity': [10, np.inf]},
-    # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, filter(s) to apply to the test set at image level"""
-test_event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, filter(s) to apply to the test set"""
+"""dict: optional, the parameters of the dataset specific to the test operation."""
 # test_file_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 test_batch_size = 10
 """int: optional, the size of the mini-batch for the test"""
 test_callbacks = [
     WriteAEOutput()
 ]
```

### Comparing `Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_file_spawn.py` & `Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_clean_channel.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,191 +19,207 @@
 import gammalearn.utils as utils
 import gammalearn.datasets as dsets
 from gammalearn.constants import GAMMA_ID, PROTON_ID, ELECTRON_ID
 from gammalearn.metrics import AUCMultiClass
 
 
 # Experiment settings
-main_directory = str(Path.home()) + '/gammalearn_experiments'  # TODO change directory if needed
+main_directory = str(Path.home()) + '/gammalearn_experiments/'  # TODO change directory if needed
 """str: mandatory, where the experiments are stored"""
 experiment_name = 'test_install'
 """str: mandatory, the name of the experiment. Should be different
 for each experiment, except if one wants to resume an old experiment
 """
 info = ''
 """str: optional"""
-gpus = None
+gpus = 1
 """int or list: mandatory, the umber of gpus to use. If -1, run on all GPUS, 
 if None/0 run on CPU. If list, run on GPUS of list.
 """
-log_every_n_steps = 3
+log_every_n_steps = 5
 """int: optional, the interval in term of iterations for on screen
 data printing during experiment
 """
 window_size = 100
 """int: optional, the interval in term of stored values for metric moving computation"""
 save_every = 1
 """int: optional, the interval in term of epochs for saving the model parameters.
 If save_every < 1, the model is not saved.
 If not provided, the model is not saved.
 """
 random_seed = 1
 """int: optional, the manual seed to make experiments more reproducible"""
 monitor_gpus = True
 """bool: optional, whether or not monitoring the gpu utilization"""
-
-# dataset_class = dsets.MemoryLSTDataset
-dataset_class = dsets.FileLSTDataset
-# dataset_class = dsets.MockLSTDataset
-"""Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
-loads images in memory, and FileLSTDataset that loads images from files during training.
-"""
-dataset_parameters = {'camera_type': 'LST_LSTCam',
-                      'group_by': 'image',
-                      'use_time': True,
-                      'particle_dict': {GAMMA_ID: 0,
-                                        PROTON_ID: 1,
-                                        # ELECTRON_ID: 2,
-                                        },
-                      # 'subarray': [1],
-                      }
-"""dict: mandatory, the parameters of the dataset.
-camera_type is mandatory and can be:
-'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
-group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
-particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0, 
-proton (101) is class 1 and electron (1) is class 2.
-use_time (optional): whether or not to use time information
-subarray (optional): the list of telescope ids to select as a subarray
-"""
-data_transform = {'data': [dsets.NumpyToTensor(),
-                           ],
-                  'target': [
-                      dsets.NumpyToTensor()
-                  ],
-                  'telescope': [
-                      dsets.NumpyToTensor()
-                  ]
-                  }
-"""dict: optional, dictionary of transform functions to apply to the samples of data from the Dataset"""
-preprocessing_workers = 4
-"""int: optional, the max number of workers to create dataset."""
-dataloader_workers = 4
-"""int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
-mp_start_method = 'spawn'
-"""str: optional, the method to start new process in [fork, spawn]"""
+particle_dict = {GAMMA_ID: 0,
+                 PROTON_ID: 1,
+                 # ELECTRON_ID: 2,
+                 }
+"""particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0"""
 targets = collections.OrderedDict({
     'energy': {
         'output_shape': 1,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
         'metrics': {
             # 'functions': ,
-        }
+        },
+        'mt_balancing': True
     },
     'impact': {
         'output_shape': 2,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
-        'metrics': {}
+        'metrics': {},
+        'mt_balancing': True
     },
     'direction': {
         'output_shape': 2,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
-        'metrics': {}
+        'metrics': {},
+        'mt_balancing': True
     },
     'class': {
         'label_shape': 1,
+        'output_shape': len(particle_dict),
         'loss': criterions.nll_nn,
         'loss_weight': 1,
         'metrics': {
-            'Accuracy': Accuracy(threshold=0.5),
-            'AUC': AUCMultiClass(buffer_size=window_size,
+            'Accuracy_particle': Accuracy(threshold=0.5),
+            'AUC_particle': AUCMultiClass(buffer_size=window_size,
                                  compute_on_step=True),
             # 'AUC': AUROC(pos_label=dataset_parameters['particle_dict'][GAMMA_ID],
             #              num_classes=len(dataset_parameters['particle_dict']),
             #              compute_on_step=True
             #              )
-        }
-    },
+        },
+        'mt_balancing': True
+    }
 })
 """dict: mandatory, defines for every objectives of the experiment
 the loss function and its weight
 """
 
+dataset_class = dsets.MemoryLSTDataset
+# dataset_class = dsets.FileLSTDataset
+"""Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
+loads images in memory, and FileLSTDataset that loads images from files during training.
+"""
+dataset_parameters = {
+    'camera_type': 'LST_LSTCam',
+    'group_by': 'image',
+    'use_time': True,
+    'particle_dict': particle_dict,
+    'targets': list(targets.keys()),
+    # 'subarray': [1],
+}
+"""dict: mandatory, the parameters of the dataset.
+camera_type is mandatory and can be:
+'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
+group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
+particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0, 
+proton (101) is class 1 and electron (1) is class 2.
+use_time (optional): whether or not to use time information
+subarray (optional): the list of telescope ids to select as a subarray
+"""
+preprocessing_workers = 4
+"""int: optional, the max number of workers to create dataset."""
+dataloader_workers = 4
+"""int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
+mp_start_method = 'fork'
+"""str: optional, the method to start new process in [fork, spawn]"""
+
 # Net settings
 net_definition_file = utils.nets_definition_path()
 """str: mandatory, the file where to find the net definition to use"""
 # Load the network definitions module #
 spec = importlib.util.spec_from_file_location("nets", net_definition_file)
 nets = importlib.util.module_from_spec(spec)
 spec.loader.exec_module(nets)
 ########################################
-model_net = nets.GLNetIndexConv42
-"""nn.Module: mandatory, the network for the experiment. Is a class
-inheriting from nn.Module defining the operations of the network and
-the forward method to pass data through it
-"""
 net_parameters_dic = {
-    'num_channels': 2,
-    'n_features': 16,
-    'batchnorm': True,
-    'drop_rate': 0,
+    'model': nets.GammaPhysNet,
+    'parameters': {
+        'backbone': {
+            'model': nets.ResNetAttentionIndexed,
+            'parameters': {
+                'num_layers': 3,
+                'init': 'kaiming',
+                'batch_norm': True,
+                'num_channels': 3,
+                'block_features': [16, 32, 64],
+                'attention_layer': (nets.DualAttention, {'ratio': 16}),
+                'non_linearity': torch.nn.ReLU,
+            }
+        },
+        'fc_width': 256,
+        'non_linearity': torch.nn.ReLU,
+        'last_bias_init': None,
+        'targets': {k: v.get('output_shape', 0) for k, v in targets.items()}
+    }
 }
 """dict: mandatory, the parameters of the network. Depends on the
-network chosen
+network chosen. Must include at least a model and a parameters field.
 """
 # checkpoint_path = main_directory + '/test_install/checkpoint_epoch=3.ckpt'
 """str: optional, the path where to find the backup of the model to resume"""
 
 profiler = None
 # profiler = {'profiler': SimpleProfiler,
 #             'options': dict(extended=True)
 #             }
 """str: optional, the profiler to use"""
 
 ######################################################################################################################
 train = True
 """bool: mandatory, whether or not to train the model"""
 # Data settings
-train_folders = [
-    Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
-]  # TODO fill your folder path
-"""list: mandatory, the folders where to find the hdf5 data files"""
+data_module_train = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
+        ], # TODO fill your folder path
+        'image_filter': {
+            # utils.intensity_filter: {'intensity': [50, np.inf]},
+            # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': dsets.CleanImages(new_channel=True),
+        'target_transform': None
+    },
+    'target': {
+        'paths': [],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': None,
+        'target_transform': None
+    }
+}
+"""paths->list: mandatory, the folders where to find the hdf5 data files"""
+"""image_filter->dict: optional, the filter(s) to apply to the dataset at image level"""
+"""event_filter->dict: optional, the filter(s) to apply to the dataset"""
 
 validating_ratio = 0.2
 """float: mandatory, the ratio of data to create the validating set"""
 split_by_file = False
 """bool: optional, whether to split data at the file level or at the data level"""
-max_epochs = 1
+max_epochs = 4
 """int: mandatory, the maximum number of epochs for the experiment"""
 batch_size = 8
 """int: mandatory, the size of the mini-batch"""
-image_filter = {
-    # utils.intensity_filter: {'intensity': [50, np.inf]},
-    # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset at image level"""
-event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset"""
-
-# data_augment = {'function': dsets.augment_via_rotation,
-#                 'kwargs': {'thetas': [2 * math.pi / 3, 4 * math.pi / 3],
-#                            'num_workers': 8}
-#                 }
-"""dict: optional, dictionary describing the function to use for dataset augmentation"""
 # dataset_size = 2000
 """int: optional, the max size of the dataset"""
 # files_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 
 pin_memory = True
 """bool: optional, whether or not to pin memory in dataloader"""
@@ -218,27 +234,28 @@
 }
 """dict: mandatory, defines for every objectives of the experiment
 the loss function and its weight
 """
 compute_loss = criterions.MultilossBalancing(targets, **loss_options)
 """function: mandatory, the function to compute the loss"""
 optimizer_dic = {
-    'network': optimizers.load_sgd,
+    # 'network': optimizers.load_sgd,
+    'network': optimizers.load_adam,
     'loss_balancing': optimizers.load_adam
 }
 """dict: mandatory, the optimizers to use for the experiment.
 One may want to use several optimizers in case of GAN for example
 """
 optimizer_parameters = {
-    'network': {'learning_rate': 1e-4,
+    'network': {'lr': 1e-2,
                 'weight_decay': 1e-7,
-                'momentum': 0.9,
-                'nesterov': True
+                # 'momentum': 0.9,
+                # 'nesterov': True
                 },
-    'loss_balancing': {'learning_rate': 0.025,
+    'loss_balancing': {'lr': 0.025,
                        'weight_decay': 1e-4,
                        },
 }
 """dict: mandatory, defines the parameters for every optimizers to use"""
 # regularization = {'function': 'gradient_penalty',
 #                   'weight': 10}
 """dict: optional, regularization to use during the training process. See in optimizers.py for 
@@ -249,29 +266,37 @@
 # training_step = steps.training_step_mt_gradient_penalty
 """function: mandatory, the function to compute the training step"""
 eval_step = steps.eval_step_mt
 """function: mandatory, the function to compute the validating step"""
 check_val_every_n_epoch = 1
 """int: optional, the interval in term of epoch for validating the model"""
 lr_schedulers = {
-    lr_scheduler.StepLR: {'network': {'gamma': 0.1,
-                                      'step_size': 10,
-                                      },
-                          },
-    # lr_scheduler.ReduceLROnPlateau: {'network': {'factor': 0.1,
-    #                                              'patience': 30,
-    #                                              },
-    #                                  },
-    # lr_scheduler.MultiStepLR: {'network': {'gamma': 0.1,
-    #                                        'milestones': [10, 15, 18],
-    #                                        },
-    #                            },
-    # lr_scheduler.ExponentialLR: {'network': {'gamma': 0.9,
-    #                                          },
-    #                              },
+    'network': {
+        lr_scheduler.StepLR: {
+            'gamma': 0.1,
+            'step_size': 10,
+        }
+    },
+    # 'network': {
+    #     lr_scheduler.ReduceLROnPlateau: {
+    #         'factor': 0.1,
+    #         'patience': 30,
+    #     }
+    # },
+    # 'network': {
+    #     lr_scheduler.MultiStepLR: {
+    #         'gamma': 0.1,
+    #         'milestones': [10, 15, 18],
+    #     }
+    # },
+    # 'network': {
+    #     lr_scheduler.ExponentialLR: {
+    #         'gamma': 0.9,
+    #     }
+    # },
 }
 """dict: optional, defines the learning rate schedulers"""
 # callbacks
 training_callbacks = [
     LogGradientNorm(),
     LogModelWeightNorm(),
     LogModelParameters(),
@@ -284,44 +309,62 @@
 """dict: list of callbacks
 """
 
 ######################################################################################################################
 # Testing settings
 test = True
 """bool: mandatory, whether or not to test the model at the end of training"""
+merge_test_datasets = False
+"""bool: optional, whether or not to merge test datasets"""
+data_module_test = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
+        ],
+        'image_filter': {
+            utils.intensity_filter: {'intensity': [10, np.inf]},
+            # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': dsets.CleanImages(new_channel=True),
+        'target_transform': None
+    },
+    'target': {
+        'paths': [],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': None,
+        'target_transform': None
+    }
+}
+"""
+dict: optional, must at least contain a non-empty 'source':{'paths:[]'}
+path->list of str: optional, the folders containing the hdf5 data files for the test
+image_filter->dict: optional, filter(s) to apply to the test set at image level
+event_filter->dict: optional, filter(s) to apply to the test set
+"""
+
 test_step = steps.test_step_mt
 """function: mandatory, the function to compute the validating step"""
-test_folders = [
-]
-"""list of str: optional, the folders containing the hdf5 data files for the test
-"""
 dl2_path = ''
 """str: optional, path to store dl2 files"""
 test_dataset_parameters = {
     # 'subarray': [1],
 }
-"""dict: optional, the parameters of the dataset specific to the test operation.
-"""
-test_image_filter = {
-    utils.intensity_filter: {'intensity': [10, np.inf]},
-    # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, filter(s) to apply to the test set at image level"""
-test_event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, filter(s) to apply to the test set"""
-# test_file_max_number = 1
+"""dict: optional, the parameters of the dataset specific to the test operation."""
+test_file_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 test_batch_size = 10
 """int: optional, the size of the mini-batch for the test"""
 test_callbacks = [
-    # WriteDL2Files()
+    WriteDL2Files()
 ]
-"""dict: list of callbacks
-"""
+"""dict: list of callbacks"""
```

### Comparing `Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_profiler.py` & `Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_val.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 from gammalearn.constants import GAMMA_ID, PROTON_ID, ELECTRON_ID
 from gammalearn.metrics import AUCMultiClass
 
 
 # Experiment settings
 main_directory = str(Path.home()) + '/gammalearn_experiments'  # TODO change directory if needed
 """str: mandatory, where the experiments are stored"""
-experiment_name = 'test_install3'
+experiment_name = 'test_install'
 """str: mandatory, the name of the experiment. Should be different
 for each experiment, except if one wants to resume an old experiment
 """
 info = ''
 """str: optional"""
-gpus = 1
+gpus = None
 """int or list: mandatory, the umber of gpus to use. If -1, run on all GPUS, 
 if None/0 run on CPU. If list, run on GPUS of list.
 """
 log_every_n_steps = 3
 """int: optional, the interval in term of iterations for on screen
 data printing during experiment
 """
@@ -46,181 +46,183 @@
 If save_every < 1, the model is not saved.
 If not provided, the model is not saved.
 """
 random_seed = 1
 """int: optional, the manual seed to make experiments more reproducible"""
 monitor_gpus = True
 """bool: optional, whether or not monitoring the gpu utilization"""
-
-dataset_class = dsets.MemoryLSTDataset
-# dataset_class = dsets.FileLSTDataset
-"""Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
-loads images in memory, and FileLSTDataset that loads images from files during training.
-"""
-dataset_parameters = {'camera_type': 'LST_LSTCam',
-                      'group_by': 'image',
-                      'use_time': True,
-                      'particle_dict': {GAMMA_ID: 0,
-                                        PROTON_ID: 1,
-                                        # ELECTRON_ID: 2,
-                                        },
-                      # 'subarray': [1],
-                      }
-"""dict: mandatory, the parameters of the dataset.
-camera_type is mandatory and can be:
-'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
-group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
-particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0, 
-proton (101) is class 1 and electron (1) is class 2.
-use_time (optional): whether or not to use time information
-subarray (optional): the list of telescope ids to select as a subarray
-"""
-data_transform = {'data': [dsets.NumpyToTensor(),
-                           ],
-                  'target': [
-                      dsets.NumpyToTensor()
-                  ],
-                  'telescope': [
-                      dsets.NumpyToTensor()
-                  ]
-                  }
-"""dict: optional, dictionary of transform functions to apply to the samples of data from the Dataset"""
-preprocessing_workers = 4
-"""int: optional, the max number of workers to create dataset."""
-dataloader_workers = 4
-"""int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
-mp_start_method = 'fork'
-"""str: optional, the method to start new process in [fork, spawn]"""
+particle_dict = {GAMMA_ID: 0,
+                 PROTON_ID: 1,
+                 # ELECTRON_ID: 2,
+                 }
+"""particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0"""
 targets = collections.OrderedDict({
     'energy': {
         'output_shape': 1,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
         'metrics': {
             # 'functions': ,
-        }
+        },
+        'mt_balancing': True
     },
     'impact': {
         'output_shape': 2,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
-        'metrics': {}
+        'metrics': {},
+        'mt_balancing': True
     },
     'direction': {
         'output_shape': 2,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
-        'metrics': {}
+        'metrics': {},
+        'mt_balancing': True
     },
     'class': {
         'label_shape': 1,
-        'loss': criterions.nll_nn,
+        'output_shape': len(particle_dict),
+        'loss': torch.nn.CrossEntropyLoss(),
         'loss_weight': 1,
         'metrics': {
-            'Accuracy': Accuracy(threshold=0.5),
-            'AUC': AUCMultiClass(buffer_size=window_size,
-                                 compute_on_step=True),
+            'Accuracy_particle': Accuracy(threshold=0.5),
+            'AUC_particle': AUCMultiClass(buffer_size=window_size,
+                                          compute_on_step=True),
             # 'AUC': AUROC(pos_label=dataset_parameters['particle_dict'][GAMMA_ID],
             #              num_classes=len(dataset_parameters['particle_dict']),
             #              compute_on_step=True
             #              )
-        }
-    },
+        },
+        'mt_balancing': True
+    }
 })
 """dict: mandatory, defines for every objectives of the experiment
 the loss function and its weight
 """
 
+dataset_class = dsets.MemoryLSTDataset
+# dataset_class = dsets.FileLSTDataset
+"""Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
+loads images in memory, and FileLSTDataset that loads images from files during training.
+"""
+dataset_parameters = {
+    'camera_type': 'LST_LSTCam',
+    'group_by': 'image',
+    'use_time': True,
+    'particle_dict': particle_dict,
+    'targets': list(targets.keys()),
+    # 'subarray': [1],
+}
+"""dict: mandatory, the parameters of the dataset.
+camera_type is mandatory and can be:
+'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
+group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
+particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0,
+proton (101) is class 1 and electron (1) is class 2.
+use_time (optional): whether or not to use time information
+subarray (optional): the list of telescope ids to select as a subarray
+"""
+preprocessing_workers = 4
+"""int: optional, the max number of workers to create dataset."""
+dataloader_workers = 4
+"""int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
+mp_start_method = 'fork'
+"""str: optional, the method to start new process in [fork, spawn]"""
+
 # Net settings
 net_definition_file = utils.nets_definition_path()
 """str: mandatory, the file where to find the net definition to use"""
 # Load the network definitions module #
 spec = importlib.util.spec_from_file_location("nets", net_definition_file)
 nets = importlib.util.module_from_spec(spec)
 spec.loader.exec_module(nets)
 ########################################
-model_net = nets.GLNetIndexConv42
-"""nn.Module: mandatory, the network for the experiment. Is a class
-inheriting from nn.Module defining the operations of the network and
-the forward method to pass data through it
-"""
 net_parameters_dic = {
-    'num_channels': 2,
-    'n_features': 16,
-    'batchnorm': True,
-    'drop_rate': 0,
+    'model': nets.GammaPhysNet,
+    'parameters': {
+        'backbone': {
+            'model': nets.ResNetAttentionIndexed,
+            'parameters': {
+                'num_layers': 3,
+                'init': 'kaiming',
+                'batch_norm': True,
+                # 'init': 'orthogonal',
+                'num_channels': 2,
+                'block_features': [16, 32, 64],
+                'attention_layer': (nets.DualAttention, {'ratio': 16}),
+                # 'attention_layer': (nets.SqueezeExcite, {'ratio': 4}),
+                # 'attention_layer': None,
+                'non_linearity': torch.nn.ReLU,
+            }
+        },
+        'fc_width': 256,
+        'non_linearity': torch.nn.ReLU,
+        'last_bias_init': None,
+        'targets': {k: v.get('output_shape', 0) for k, v in targets.items()}
+    }
 }
 """dict: mandatory, the parameters of the network. Depends on the
-network chosen
+network chosen. Must include at least a model and a parameters field.
 """
 # checkpoint_path = main_directory + '/test_install/checkpoint_epoch=3.ckpt'
 """str: optional, the path where to find the backup of the model to resume"""
 
-profiler = {'profiler': PyTorchProfiler,
-            'options': dict(
-                activities=[
-                    torch.profiler.ProfilerActivity.CUDA,
-                    torch.profiler.ProfilerActivity.CPU
-                ],
-                schedule=torch.profiler.schedule(wait=1,
-                                                 warmup=1,
-                                                 active=3,
-                                                 repeat=4  # Repeat the cycle wait - warmup - active
-                                                 ),
-                on_trace_ready=torch.profiler.tensorboard_trace_handler(dir_name=os.path.join(main_directory,
-                                                                                              'runs',
-                                                                                              experiment_name,
-                                                                                              'log_profile'),
-                                                                        ),
-                record_shapes=True,
-                profile_memory=True,
-                with_stack=True,
-                with_flops=True,
-            )
-            }
+profiler = None
+# profiler = {'profiler': SimpleProfiler,
+#             'options': dict(extended=True)
+#             }
 """str: optional, the profiler to use"""
 
 ######################################################################################################################
 train = True
 """bool: mandatory, whether or not to train the model"""
 # Data settings
-train_folders = [
-    Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
-]  # TODO fill your folder path
-"""list: mandatory, the folders where to find the hdf5 data files"""
+data_module_train = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
+        ], # TODO fill your folder path
+        'image_filter': {
+            # utils.intensity_filter: {'intensity': [50, np.inf]},
+            # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': None,
+        'target_transform': None
+    },
+    'target': {
+        'paths': [],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': None,
+        'target_transform': None
+    }
+}
+"""paths->list: mandatory, the folders where to find the hdf5 data files"""
+"""image_filter->dict: optional, the filter(s) to apply to the dataset at image level"""
+"""event_filter->dict: optional, the filter(s) to apply to the dataset"""
 
 validating_ratio = 0.2
 """float: mandatory, the ratio of data to create the validating set"""
 split_by_file = False
 """bool: optional, whether to split data at the file level or at the data level"""
 max_epochs = 4
 """int: mandatory, the maximum number of epochs for the experiment"""
 batch_size = 4
 """int: mandatory, the size of the mini-batch"""
-image_filter = {
-    # utils.intensity_filter: {'intensity': [50, np.inf]},
-    # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset at image level"""
-event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset"""
-
-# data_augment = {'function': dsets.augment_via_rotation,
-#                 'kwargs': {'thetas': [2 * math.pi / 3, 4 * math.pi / 3],
-#                            'num_workers': 8}
-#                 }
-"""dict: optional, dictionary describing the function to use for dataset augmentation"""
 # dataset_size = 2000
 """int: optional, the max size of the dataset"""
 # files_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 
 pin_memory = True
 """bool: optional, whether or not to pin memory in dataloader"""
@@ -242,20 +244,20 @@
     'network': optimizers.load_sgd,
     'loss_balancing': optimizers.load_adam
 }
 """dict: mandatory, the optimizers to use for the experiment.
 One may want to use several optimizers in case of GAN for example
 """
 optimizer_parameters = {
-    'network': {'learning_rate': 1e-4,
+    'network': {'lr': 1e-4,
                 'weight_decay': 1e-7,
                 'momentum': 0.9,
                 'nesterov': True
                 },
-    'loss_balancing': {'learning_rate': 0.025,
+    'loss_balancing': {'lr': 0.025,
                        'weight_decay': 1e-4,
                        },
 }
 """dict: mandatory, defines the parameters for every optimizers to use"""
 # regularization = {'function': 'gradient_penalty',
 #                   'weight': 10}
 """dict: optional, regularization to use during the training process. See in optimizers.py for 
@@ -266,29 +268,37 @@
 # training_step = steps.training_step_mt_gradient_penalty
 """function: mandatory, the function to compute the training step"""
 eval_step = steps.eval_step_mt
 """function: mandatory, the function to compute the validating step"""
 check_val_every_n_epoch = 1
 """int: optional, the interval in term of epoch for validating the model"""
 lr_schedulers = {
-    lr_scheduler.StepLR: {'network': {'gamma': 0.1,
-                                      'step_size': 10,
-                                      },
-                          },
-    # lr_scheduler.ReduceLROnPlateau: {'network': {'factor': 0.1,
-    #                                              'patience': 30,
-    #                                              },
-    #                                  },
-    # lr_scheduler.MultiStepLR: {'network': {'gamma': 0.1,
-    #                                        'milestones': [10, 15, 18],
-    #                                        },
-    #                            },
-    # lr_scheduler.ExponentialLR: {'network': {'gamma': 0.9,
-    #                                          },
-    #                              },
+    'network': {
+        lr_scheduler.StepLR: {
+            'gamma': 0.1,
+            'step_size': 10,
+        }
+    },
+    # 'network': {
+    #     lr_scheduler.ReduceLROnPlateau: {
+    #         'factor': 0.1,
+    #         'patience': 30,
+    #     }
+    # },
+    # 'network': {
+    #     lr_scheduler.MultiStepLR: {
+    #         'gamma': 0.1,
+    #         'milestones': [10, 15, 18],
+    #     }
+    # },
+    # 'network': {
+    #     lr_scheduler.ExponentialLR: {
+    #         'gamma': 0.9,
+    #     }
+    # },
 }
 """dict: optional, defines the learning rate schedulers"""
 # callbacks
 training_callbacks = [
     LogGradientNorm(),
     LogModelWeightNorm(),
     LogModelParameters(),
@@ -301,44 +311,33 @@
 """dict: list of callbacks
 """
 
 ######################################################################################################################
 # Testing settings
 test = True
 """bool: mandatory, whether or not to test the model at the end of training"""
+merge_test_datasets = False
+"""bool: optional, whether or not to merge test datasets"""
+data_module_test = None
+"""
+dict: optional, must at least contain a non-empty 'source':{'paths:[]'}
+path->list of str: optional, the folders containing the hdf5 data files for the test
+image_filter->dict: optional, filter(s) to apply to the test set at image level
+event_filter->dict: optional, filter(s) to apply to the test set
+"""
+
 test_step = steps.test_step_mt
 """function: mandatory, the function to compute the validating step"""
-test_folders = [
-]
-"""list of str: optional, the folders containing the hdf5 data files for the test
-"""
 dl2_path = ''
 """str: optional, path to store dl2 files"""
 test_dataset_parameters = {
     # 'subarray': [1],
 }
-"""dict: optional, the parameters of the dataset specific to the test operation.
-"""
-test_image_filter = {
-    utils.intensity_filter: {'intensity': [10, np.inf]},
-    # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, filter(s) to apply to the test set at image level"""
-test_event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, filter(s) to apply to the test set"""
+"""dict: optional, the parameters of the dataset specific to the test operation."""
 # test_file_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
-test_batch_size = 10
+test_batch_size = 3
 """int: optional, the size of the mini-batch for the test"""
 test_callbacks = [
     WriteDL2Files()
 ]
-"""dict: list of callbacks
-"""
+"""dict: list of callbacks"""
```

### Comparing `Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_square_pixels.py` & `Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_square_pixels.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import importlib
 from pathlib import Path
 import math
 import numpy as np
 import torch
 from torch.optim import lr_scheduler
+from torchvision.models.mobilenet import mobilenet_v2
 
 from torchmetrics.classification import Accuracy, AUROC
 from pytorch_lightning.profiler import SimpleProfiler, AdvancedProfiler, PyTorchProfiler
 
 import gammalearn.criterions as criterions
 import gammalearn.optimizers as optimizers
 import gammalearn.steps as steps
@@ -46,157 +47,179 @@
 If save_every < 1, the model is not saved.
 If not provided, the model is not saved.
 """
 random_seed = 1
 """int: optional, the manual seed to make experiments more reproducible"""
 monitor_gpus = True
 """bool: optional, whether or not monitoring the gpu utilization"""
-
-dataset_class = dsets.MemoryLSTDataset
-# dataset_class = dsets.FileLSTDataset
-"""Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
-loads images in memory, and FileLSTDataset that loads images from files during training.
-"""
-dataset_parameters = {'camera_type': 'LST_LSTCam',
-                      'group_by': 'image',
-                      'use_time': True,
-                      'particle_dict': {GAMMA_ID: 0,
-                                        PROTON_ID: 1,
-                                        # ELECTRON_ID: 2,
-                                        },
-                      # 'subarray': [1],
-                      }
-"""dict: mandatory, the parameters of the dataset.
-camera_type is mandatory and can be:
-'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
-group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
-particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0, 
-proton (101) is class 1 and electron (1) is class 2.
-use_time (optional): whether or not to use time information
-subarray (optional): the list of telescope ids to select as a subarray
-"""
-data_transform = {'data': [dsets.ResampleImage('bilinear_interpolation', (55, 55, 1)),
-                           ],
-                  'target': [
-                  ],
-                  }
-"""dict: optional, dictionary of transform functions to apply to the samples of data from the Dataset"""
-preprocessing_workers = 4
-"""int: optional, the max number of workers to create dataset."""
-dataloader_workers = 4
-"""int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
-mp_start_method = 'fork'
-"""str: optional, the method to start new process in [fork, spawn]"""
+particle_dict = {GAMMA_ID: 0,
+                 PROTON_ID: 1,
+                 # ELECTRON_ID: 2,
+                 }
+"""particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0"""
 targets = collections.OrderedDict({
     'energy': {
         'output_shape': 1,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
         'metrics': {
             # 'functions': ,
-        }
+        },
+        'mt_balancing': True
     },
     'impact': {
         'output_shape': 2,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
-        'metrics': {}
+        'metrics': {},
+        'mt_balancing': True
     },
     'direction': {
         'output_shape': 2,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
-        'metrics': {}
+        'metrics': {},
+        'mt_balancing': True
     },
     'class': {
         'label_shape': 1,
-        'loss': criterions.nll_nn,
+        'output_shape': len(particle_dict),
+        'loss': torch.nn.CrossEntropyLoss(),
         'loss_weight': 1,
         'metrics': {
-            'Accuracy': Accuracy(threshold=0.5),
-            'AUC': AUCMultiClass(buffer_size=window_size,
-                                 compute_on_step=True),
+            'Accuracy_particle': Accuracy(threshold=0.5),
+            'AUC_particle': AUCMultiClass(buffer_size=window_size,
+                                          compute_on_step=True),
             # 'AUC': AUROC(pos_label=dataset_parameters['particle_dict'][GAMMA_ID],
             #              num_classes=len(dataset_parameters['particle_dict']),
             #              compute_on_step=True
             #              )
-        }
-    },
+        },
+        'mt_balancing': True
+    }
 })
 """dict: mandatory, defines for every objectives of the experiment
 the loss function and its weight
 """
 
+dataset_class = dsets.MemoryLSTDataset
+# dataset_class = dsets.FileLSTDataset
+"""Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
+loads images in memory, and FileLSTDataset that loads images from files during training.
+"""
+dataset_parameters = {
+    'camera_type': 'LST_LSTCam',
+    'group_by': 'image',
+    'use_time': True,
+    'particle_dict': particle_dict,
+    'targets': list(targets.keys()),
+    # 'subarray': [1],
+}
+"""dict: mandatory, the parameters of the dataset.
+camera_type is mandatory and can be:
+'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
+group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
+particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0, 
+proton (101) is class 1 and electron (1) is class 2.
+use_time (optional): whether or not to use time information
+subarray (optional): the list of telescope ids to select as a subarray
+"""
+preprocessing_workers = 4
+"""int: optional, the max number of workers to create dataset."""
+dataloader_workers = 4
+"""int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
+mp_start_method = 'fork'
+"""str: optional, the method to start new process in [fork, spawn]"""
+
 # Net settings
 net_definition_file = utils.nets_definition_path()
 """str: mandatory, the file where to find the net definition to use"""
 # Load the network definitions module #
 spec = importlib.util.spec_from_file_location("nets", net_definition_file)
 nets = importlib.util.module_from_spec(spec)
 spec.loader.exec_module(nets)
 ########################################
-model_net = nets.ResNet18MT
-"""nn.Module: mandatory, the network for the experiment. Is a class
-inheriting from nn.Module defining the operations of the network and
-the forward method to pass data through it
-"""
 net_parameters_dic = {
-    'num_channels': 2,
-    'drop_rate': 0,
+    'model': nets.GammaPhysNet,
+    'parameters': {
+        'backbone': {
+            'model': nets.TorchModel,
+            'parameters': {
+                'model': mobilenet_v2,
+                'parameters': {
+                    'num_channels': 2,
+                    'output_size': (14, 14),
+                    'pretrained': False,
+                }
+            }
+        },
+        'fc_width': 256,
+        'non_linearity': torch.nn.ReLU,
+        'last_bias_init': None,
+        'targets': {k: v.get('output_shape', 0) for k, v in targets.items()}
+    }
 }
 """dict: mandatory, the parameters of the network. Depends on the
-network chosen
+network chosen. Must include at least a model and a parameters field.
 """
 # checkpoint_path = main_directory + '/test_install/checkpoint_epoch=3.ckpt'
 """str: optional, the path where to find the backup of the model to resume"""
 
 profiler = None
 # profiler = {'profiler': SimpleProfiler,
 #             'options': dict(extended=True)
 #             }
 """str: optional, the profiler to use"""
 
 ######################################################################################################################
 train = True
 """bool: mandatory, whether or not to train the model"""
 # Data settings
-train_folders = [
-    Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
-]  # TODO fill your folder path
-"""list: mandatory, the folders where to find the hdf5 data files"""
+data_module_train = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
+        ], # TODO fill your folder path
+        'image_filter': {
+            # utils.intensity_filter: {'intensity': [50, np.inf]},
+            # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': dsets.ResampleImage('bilinear_interpolation', (55, 55, 1)),
+        'target_transform': None
+    },
+    'target': {
+        'paths': [],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': None,
+        'target_transform': None
+    }
+}
+"""paths->list: mandatory, the folders where to find the hdf5 data files"""
+"""image_filter->dict: optional, the filter(s) to apply to the dataset at image level"""
+"""event_filter->dict: optional, the filter(s) to apply to the dataset"""
 
 validating_ratio = 0.2
 """float: mandatory, the ratio of data to create the validating set"""
 split_by_file = False
 """bool: optional, whether to split data at the file level or at the data level"""
 max_epochs = 4
 """int: mandatory, the maximum number of epochs for the experiment"""
 batch_size = 8
 """int: mandatory, the size of the mini-batch"""
-image_filter = {
-    # utils.intensity_filter: {'intensity': [50, np.inf]},
-    # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset at image level"""
-event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset"""
-
-# data_augment = {'function': dsets.augment_via_rotation,
-#                 'kwargs': {'thetas': [2 * math.pi / 3, 4 * math.pi / 3],
-#                            'num_workers': 8}
-#                 }
-"""dict: optional, dictionary describing the function to use for dataset augmentation"""
 # dataset_size = 2000
 """int: optional, the max size of the dataset"""
 # files_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 
 pin_memory = True
 """bool: optional, whether or not to pin memory in dataloader"""
@@ -218,20 +241,20 @@
     'network': optimizers.load_sgd,
     'loss_balancing': optimizers.load_adam
 }
 """dict: mandatory, the optimizers to use for the experiment.
 One may want to use several optimizers in case of GAN for example
 """
 optimizer_parameters = {
-    'network': {'learning_rate': 1e-4,
+    'network': {'lr': 1e-4,
                 'weight_decay': 1e-7,
                 'momentum': 0.9,
                 'nesterov': True
                 },
-    'loss_balancing': {'learning_rate': 0.025,
+    'loss_balancing': {'lr': 0.025,
                        'weight_decay': 1e-4,
                        },
 }
 """dict: mandatory, defines the parameters for every optimizers to use"""
 # regularization = {'function': 'gradient_penalty',
 #                   'weight': 10}
 """dict: optional, regularization to use during the training process. See in optimizers.py for 
@@ -242,29 +265,37 @@
 # training_step = steps.training_step_mt_gradient_penalty
 """function: mandatory, the function to compute the training step"""
 eval_step = steps.eval_step_mt
 """function: mandatory, the function to compute the validating step"""
 check_val_every_n_epoch = 1
 """int: optional, the interval in term of epoch for validating the model"""
 lr_schedulers = {
-    lr_scheduler.StepLR: {'network': {'gamma': 0.1,
-                                      'step_size': 10,
-                                      },
-                          },
-    # lr_scheduler.ReduceLROnPlateau: {'network': {'factor': 0.1,
-    #                                              'patience': 30,
-    #                                              },
-    #                                  },
-    # lr_scheduler.MultiStepLR: {'network': {'gamma': 0.1,
-    #                                        'milestones': [10, 15, 18],
-    #                                        },
-    #                            },
-    # lr_scheduler.ExponentialLR: {'network': {'gamma': 0.9,
-    #                                          },
-    #                              },
+    'network': {
+        lr_scheduler.StepLR: {
+            'gamma': 0.1,
+            'step_size': 10,
+        }
+    },
+    # 'network': {
+    #     lr_scheduler.ReduceLROnPlateau: {
+    #         'factor': 0.1,
+    #         'patience': 30,
+    #     }
+    # },
+    # 'network': {
+    #     lr_scheduler.MultiStepLR: {
+    #         'gamma': 0.1,
+    #         'milestones': [10, 15, 18],
+    #     }
+    # },
+    # 'network': {
+    #     lr_scheduler.ExponentialLR: {
+    #         'gamma': 0.9,
+    #     }
+    # },
 }
 """dict: optional, defines the learning rate schedulers"""
 # callbacks
 training_callbacks = [
     LogGradientNorm(),
     LogModelWeightNorm(),
     LogModelParameters(),
@@ -277,43 +308,61 @@
 """dict: list of callbacks
 """
 
 ######################################################################################################################
 # Testing settings
 test = True
 """bool: mandatory, whether or not to test the model at the end of training"""
+merge_test_datasets = False
+"""bool: optional, whether or not to merge test datasets"""
+data_module_test = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
+        ],
+        'image_filter': {
+            utils.intensity_filter: {'intensity': [10, np.inf]},
+            # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': dsets.ResampleImage('bilinear_interpolation', (55, 55, 1)),
+        'target_transform': None
+    },
+    'target': {
+        'paths': [],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': None,
+        'target_transform': None
+    }
+}
+"""
+dict: optional, must at least contain a non-empty 'source':{'paths:[]'}
+path->list of str: optional, the folders containing the hdf5 data files for the test
+image_filter->dict: optional, filter(s) to apply to the test set at image level
+event_filter->dict: optional, filter(s) to apply to the test set
+"""
+
 test_step = steps.test_step_mt
 """function: mandatory, the function to compute the validating step"""
-test_folders = [
-    Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
-]
-"""list of str: optional, the folders containing the hdf5 data files for the test
-"""
 dl2_path = ''
 """str: optional, path to store dl2 files"""
 test_dataset_parameters = {
     # 'subarray': [1],
 }
-"""dict: optional, the parameters of the dataset specific to the test operation.
-"""
-test_image_filter = {
-    utils.intensity_filter: {'intensity': [10, np.inf]},
-    # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, filter(s) to apply to the test set at image level"""
-test_event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, filter(s) to apply to the test set"""
+"""dict: optional, the parameters of the dataset specific to the test operation."""
 # test_file_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 test_batch_size = 10
 """int: optional, the size of the mini-batch for the test"""
 test_callbacks = [
     WriteDL2Files()
 ]
```

### Comparing `Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_square_pixels_bicubic.py` & `Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_test_MC.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 """str: mandatory, where the experiments are stored"""
 experiment_name = 'test_install'
 """str: mandatory, the name of the experiment. Should be different
 for each experiment, except if one wants to resume an old experiment
 """
 info = ''
 """str: optional"""
-gpus = None
+gpus = 1
 """int or list: mandatory, the umber of gpus to use. If -1, run on all GPUS, 
 if None/0 run on CPU. If list, run on GPUS of list.
 """
 log_every_n_steps = 3
 """int: optional, the interval in term of iterations for on screen
 data printing during experiment
 """
@@ -46,167 +46,180 @@
 If save_every < 1, the model is not saved.
 If not provided, the model is not saved.
 """
 random_seed = 1
 """int: optional, the manual seed to make experiments more reproducible"""
 monitor_gpus = True
 """bool: optional, whether or not monitoring the gpu utilization"""
-
-dataset_class = dsets.MemoryLSTDataset
-# dataset_class = dsets.FileLSTDataset
-"""Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
-loads images in memory, and FileLSTDataset that loads images from files during training.
-"""
-dataset_parameters = {'camera_type': 'LST_LSTCam',
-                      'group_by': 'image',
-                      'use_time': True,
-                      'particle_dict': {GAMMA_ID: 0,
-                                        PROTON_ID: 1,
-                                        # ELECTRON_ID: 2,
-                                        },
-                      # 'subarray': [1],
-                      }
-"""dict: mandatory, the parameters of the dataset.
-camera_type is mandatory and can be:
-'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
-group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
-particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0, 
-proton (101) is class 1 and electron (1) is class 2.
-use_time (optional): whether or not to use time information
-subarray (optional): the list of telescope ids to select as a subarray
-"""
-data_transform = {'data': [dsets.ResampleImage('bicubic_interpolation', (55, 55, 1)),
-                           ],
-                  'target': [
-                  ],
-                  }
-"""dict: optional, dictionary of transform functions to apply to the samples of data from the Dataset"""
-preprocessing_workers = 4
-"""int: optional, the max number of workers to create dataset."""
-dataloader_workers = 4
-"""int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
-mp_start_method = 'fork'
-"""str: optional, the method to start new process in [fork, spawn]"""
+particle_dict = {GAMMA_ID: 0,
+                 PROTON_ID: 1,
+                 # ELECTRON_ID: 2,
+                 }
+"""particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0"""
 targets = collections.OrderedDict({
     'energy': {
         'output_shape': 1,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
         'metrics': {
             # 'functions': ,
-        }
+        },
+        'mt_balancing': True
     },
     'impact': {
         'output_shape': 2,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
-        'metrics': {}
+        'metrics': {},
+        'mt_balancing': True
     },
     'direction': {
         'output_shape': 2,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
-        'metrics': {}
+        'metrics': {},
+        'mt_balancing': True
     },
     'class': {
         'label_shape': 1,
-        'loss': criterions.nll_nn,
+        'output_shape': len(particle_dict),
+        'loss': torch.nn.CrossEntropyLoss(),
         'loss_weight': 1,
         'metrics': {
-            'Accuracy': Accuracy(threshold=0.5),
-            'AUC': AUCMultiClass(buffer_size=window_size,
+            'Accuracy_particle': Accuracy(threshold=0.5),
+            'AUC_particle': AUCMultiClass(buffer_size=window_size,
                                  compute_on_step=True),
             # 'AUC': AUROC(pos_label=dataset_parameters['particle_dict'][GAMMA_ID],
             #              num_classes=len(dataset_parameters['particle_dict']),
             #              compute_on_step=True
             #              )
-        }
-    },
+        },
+        'mt_balancing': True
+    }
 })
 """dict: mandatory, defines for every objectives of the experiment
 the loss function and its weight
 """
 
+dataset_class = dsets.MemoryLSTDataset
+# dataset_class = dsets.FileLSTDataset
+"""Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
+loads images in memory, and FileLSTDataset that loads images from files during training.
+"""
+dataset_parameters = {
+    'camera_type': 'LST_LSTCam',
+    'group_by': 'image',
+    'use_time': True,
+    'particle_dict': particle_dict,
+    'targets': list(targets.keys()),
+    # 'subarray': [1],
+}
+"""dict: mandatory, the parameters of the dataset.
+camera_type is mandatory and can be:
+'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
+group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
+particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0, 
+proton (101) is class 1 and electron (1) is class 2.
+use_time (optional): whether or not to use time information
+subarray (optional): the list of telescope ids to select as a subarray
+"""
+preprocessing_workers = 4
+"""int: optional, the max number of workers to create dataset."""
+dataloader_workers = 4
+"""int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
+mp_start_method = 'fork'
+"""str: optional, the method to start new process in [fork, spawn]"""
+
 # Net settings
 net_definition_file = utils.nets_definition_path()
 """str: mandatory, the file where to find the net definition to use"""
 # Load the network definitions module #
 spec = importlib.util.spec_from_file_location("nets", net_definition_file)
 nets = importlib.util.module_from_spec(spec)
 spec.loader.exec_module(nets)
 ########################################
-model_net = nets.GammaPhysNetCartesian
-"""nn.Module: mandatory, the network for the experiment. Is a class
-inheriting from nn.Module defining the operations of the network and
-the forward method to pass data through it
-"""
 net_parameters_dic = {
-    "num_layers": 3,
-    "init": "kaiming",
-    "batch_norm": True,
-    # "init": "orthogonal",
-    "num_channels": 2,
-    "block_features": [16, 32, 64],
-    "attention_layer": (nets.DualAttention, {"ratio": 16}),
-    # "attention_layer": (nets.SqueezeExcite, {"ratio": 4}),
-    # "attention_layer": None,
-    "fc_width": 256,
-    "non_linearity": torch.nn.ReLU,
-    "last_bias_init": None,
+    'model': nets.GammaPhysNet,
+    'parameters': {
+        'backbone': {
+            'model': nets.ResNetAttentionIndexed,
+            'parameters': {
+                'num_layers': 3,
+                'init': 'kaiming',
+                'batch_norm': True,
+                'num_channels': 2,
+                'block_features': [16, 32, 64],
+                'attention_layer': (nets.DualAttention, {'ratio': 16}),
+                'non_linearity': torch.nn.ReLU,
+            }
+        },
+        'fc_width': 256,
+        'non_linearity': torch.nn.ReLU,
+        'last_bias_init': None,
+        'targets': {k: v.get('output_shape', 0) for k, v in targets.items()}
+    }
 }
 """dict: mandatory, the parameters of the network. Depends on the
-network chosen
+network chosen. Must include at least a model and a parameters field.
 """
-# checkpoint_path = main_directory + '/test_install/checkpoint_epoch=3.ckpt'
+checkpoint_path = main_directory + '/test_install/checkpoint_epoch=3.ckpt'
 """str: optional, the path where to find the backup of the model to resume"""
 
 profiler = None
 # profiler = {'profiler': SimpleProfiler,
 #             'options': dict(extended=True)
 #             }
 """str: optional, the profiler to use"""
 
 ######################################################################################################################
-train = True
+train = False
 """bool: mandatory, whether or not to train the model"""
 # Data settings
-train_folders = [
-    Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
-]  # TODO fill your folder path
-"""list: mandatory, the folders where to find the hdf5 data files"""
+data_module_train = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
+        ], # TODO fill your folder path
+        'image_filter': {
+            # utils.intensity_filter: {'intensity': [50, np.inf]},
+            # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': None,
+        'target_transform': None
+    },
+    'target': {
+        'paths': [],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': None,
+        'target_transform': None
+    }
+}
+"""paths->list: mandatory, the folders where to find the hdf5 data files"""
+"""image_filter->dict: optional, the filter(s) to apply to the dataset at image level"""
+"""event_filter->dict: optional, the filter(s) to apply to the dataset"""
 
 validating_ratio = 0.2
 """float: mandatory, the ratio of data to create the validating set"""
 split_by_file = False
 """bool: optional, whether to split data at the file level or at the data level"""
 max_epochs = 4
 """int: mandatory, the maximum number of epochs for the experiment"""
 batch_size = 8
 """int: mandatory, the size of the mini-batch"""
-image_filter = {
-    # utils.intensity_filter: {'intensity': [50, np.inf]},
-    # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset at image level"""
-event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset"""
-
-# data_augment = {'function': dsets.augment_via_rotation,
-#                 'kwargs': {'thetas': [2 * math.pi / 3, 4 * math.pi / 3],
-#                            'num_workers': 8}
-#                 }
-"""dict: optional, dictionary describing the function to use for dataset augmentation"""
 # dataset_size = 2000
 """int: optional, the max size of the dataset"""
 # files_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 
 pin_memory = True
 """bool: optional, whether or not to pin memory in dataloader"""
@@ -228,20 +241,20 @@
     'network': optimizers.load_sgd,
     'loss_balancing': optimizers.load_adam
 }
 """dict: mandatory, the optimizers to use for the experiment.
 One may want to use several optimizers in case of GAN for example
 """
 optimizer_parameters = {
-    'network': {'learning_rate': 1e-4,
+    'network': {'lr': 1e-4,
                 'weight_decay': 1e-7,
                 'momentum': 0.9,
                 'nesterov': True
                 },
-    'loss_balancing': {'learning_rate': 0.025,
+    'loss_balancing': {'lr': 0.025,
                        'weight_decay': 1e-4,
                        },
 }
 """dict: mandatory, defines the parameters for every optimizers to use"""
 # regularization = {'function': 'gradient_penalty',
 #                   'weight': 10}
 """dict: optional, regularization to use during the training process. See in optimizers.py for 
@@ -252,29 +265,37 @@
 # training_step = steps.training_step_mt_gradient_penalty
 """function: mandatory, the function to compute the training step"""
 eval_step = steps.eval_step_mt
 """function: mandatory, the function to compute the validating step"""
 check_val_every_n_epoch = 1
 """int: optional, the interval in term of epoch for validating the model"""
 lr_schedulers = {
-    lr_scheduler.StepLR: {'network': {'gamma': 0.1,
-                                      'step_size': 10,
-                                      },
-                          },
-    # lr_scheduler.ReduceLROnPlateau: {'network': {'factor': 0.1,
-    #                                              'patience': 30,
-    #                                              },
-    #                                  },
-    # lr_scheduler.MultiStepLR: {'network': {'gamma': 0.1,
-    #                                        'milestones': [10, 15, 18],
-    #                                        },
-    #                            },
-    # lr_scheduler.ExponentialLR: {'network': {'gamma': 0.9,
-    #                                          },
-    #                              },
+    'network': {
+        lr_scheduler.StepLR: {
+            'gamma': 0.1,
+            'step_size': 10,
+        }
+    },
+    # 'network': {
+    #     lr_scheduler.ReduceLROnPlateau: {
+    #         'factor': 0.1,
+    #         'patience': 30,
+    #     }
+    # },
+    # 'network': {
+    #     lr_scheduler.MultiStepLR: {
+    #         'gamma': 0.1,
+    #         'milestones': [10, 15, 18],
+    #     }
+    # },
+    # 'network': {
+    #     lr_scheduler.ExponentialLR: {
+    #         'gamma': 0.9,
+    #     }
+    # },
 }
 """dict: optional, defines the learning rate schedulers"""
 # callbacks
 training_callbacks = [
     LogGradientNorm(),
     LogModelWeightNorm(),
     LogModelParameters(),
@@ -287,45 +308,62 @@
 """dict: list of callbacks
 """
 
 ######################################################################################################################
 # Testing settings
 test = True
 """bool: mandatory, whether or not to test the model at the end of training"""
+merge_test_datasets = False
+"""bool: optional, whether or not to merge test datasets"""
+data_module_test = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
+        ],
+        'image_filter': {
+            utils.intensity_filter: {'intensity': [10, np.inf]},
+            # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': None,
+        'target_transform': None
+    },
+    'target': {
+        'paths': [],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': None,
+        'target_transform': None
+    }
+}
+"""
+dict: optional, must at least contain a non-empty 'source':{'paths:[]'}
+path->list of str: optional, the folders containing the hdf5 data files for the test
+image_filter->dict: optional, filter(s) to apply to the test set at image level
+event_filter->dict: optional, filter(s) to apply to the test set
+"""
+
 test_step = steps.test_step_mt
 """function: mandatory, the function to compute the validating step"""
-test_folders = [
-    Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
-]
-"""list of str: optional, the folders containing the hdf5 data files for the test
-"""
 dl2_path = ''
 """str: optional, path to store dl2 files"""
 test_dataset_parameters = {
     # 'subarray': [1],
 }
-"""dict: optional, the parameters of the dataset specific to the test operation.
-"""
-test_image_filter = {
-    utils.intensity_filter: {'intensity': [10, np.inf]},
-    # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, filter(s) to apply to the test set at image level"""
-test_event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, filter(s) to apply to the test set"""
+"""dict: optional, the parameters of the dataset specific to the test operation."""
 # test_file_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 test_batch_size = 10
 """int: optional, the size of the mini-batch for the test"""
 test_callbacks = [
     WriteDL2Files()
 ]
-"""dict: list of callbacks
-"""
+"""dict: list of callbacks"""
```

### Comparing `Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_square_pixels_over.py` & `Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_square_pixels_bicubic.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,168 +46,181 @@
 If save_every < 1, the model is not saved.
 If not provided, the model is not saved.
 """
 random_seed = 1
 """int: optional, the manual seed to make experiments more reproducible"""
 monitor_gpus = True
 """bool: optional, whether or not monitoring the gpu utilization"""
-
-dataset_class = dsets.MemoryLSTDataset
-# dataset_class = dsets.FileLSTDataset
-"""Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
-loads images in memory, and FileLSTDataset that loads images from files during training.
-"""
-dataset_parameters = {'camera_type': 'LST_LSTCam',
-                      'group_by': 'image',
-                      'use_time': True,
-                      'particle_dict': {GAMMA_ID: 0,
-                                        PROTON_ID: 1,
-                                        # ELECTRON_ID: 2,
-                                        },
-                      # 'subarray': [1],
-                      }
-"""dict: mandatory, the parameters of the dataset.
-camera_type is mandatory and can be:
-'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
-group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
-particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0, 
-proton (101) is class 1 and electron (1) is class 2.
-use_time (optional): whether or not to use time information
-subarray (optional): the list of telescope ids to select as a subarray
-"""
-data_transform = {'data': [dsets.ResampleImage('oversampling', (55, 55, 1)),
-                           ],
-                  'target': [
-                  ],
-                  }
-"""dict: optional, dictionary of transform functions to apply to the samples of data from the Dataset"""
-preprocessing_workers = 4
-"""int: optional, the max number of workers to create dataset."""
-dataloader_workers = 4
-"""int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
-mp_start_method = 'fork'
-"""str: optional, the method to start new process in [fork, spawn]"""
+particle_dict = {GAMMA_ID: 0,
+                 PROTON_ID: 1,
+                 # ELECTRON_ID: 2,
+                 }
+"""particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0"""
 targets = collections.OrderedDict({
     'energy': {
         'output_shape': 1,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
         'metrics': {
             # 'functions': ,
-        }
+        },
+        'mt_balancing': True
     },
     'impact': {
         'output_shape': 2,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
-        'metrics': {}
+        'metrics': {},
+        'mt_balancing': True
     },
     'direction': {
         'output_shape': 2,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
-        'metrics': {}
+        'metrics': {},
+        'mt_balancing': True
     },
     'class': {
         'label_shape': 1,
-        'loss': criterions.nll_nn,
+        'output_shape': len(particle_dict),
+        'loss': torch.nn.CrossEntropyLoss(),
         'loss_weight': 1,
         'metrics': {
-            'Accuracy': Accuracy(threshold=0.5),
-            'AUC': AUCMultiClass(buffer_size=window_size,
+            'Accuracy_particle': Accuracy(threshold=0.5),
+            'AUC_particle': AUCMultiClass(buffer_size=window_size,
                                  compute_on_step=True),
             # 'AUC': AUROC(pos_label=dataset_parameters['particle_dict'][GAMMA_ID],
             #              num_classes=len(dataset_parameters['particle_dict']),
             #              compute_on_step=True
             #              )
-        }
-    },
+        },
+        'mt_balancing': True
+    }
 })
 """dict: mandatory, defines for every objectives of the experiment
 the loss function and its weight
 """
 
+dataset_class = dsets.MemoryLSTDataset
+# dataset_class = dsets.FileLSTDataset
+"""Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
+loads images in memory, and FileLSTDataset that loads images from files during training.
+"""
+dataset_parameters = {
+    'camera_type': 'LST_LSTCam',
+    'group_by': 'image',
+    'use_time': True,
+    'particle_dict': particle_dict,
+    'targets': list(targets.keys()),
+    # 'subarray': [1],
+}
+"""dict: mandatory, the parameters of the dataset.
+camera_type is mandatory and can be:
+'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
+group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
+particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0, 
+proton (101) is class 1 and electron (1) is class 2.
+use_time (optional): whether or not to use time information
+subarray (optional): the list of telescope ids to select as a subarray
+"""
+preprocessing_workers = 4
+"""int: optional, the max number of workers to create dataset."""
+dataloader_workers = 4
+"""int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
+mp_start_method = 'fork'
+"""str: optional, the method to start new process in [fork, spawn]"""
+
 # Net settings
 net_definition_file = utils.nets_definition_path()
 """str: mandatory, the file where to find the net definition to use"""
 # Load the network definitions module #
 spec = importlib.util.spec_from_file_location("nets", net_definition_file)
 nets = importlib.util.module_from_spec(spec)
 spec.loader.exec_module(nets)
 ########################################
-model_net = nets.ResNet18MT
-"""nn.Module: mandatory, the network for the experiment. Is a class
-inheriting from nn.Module defining the operations of the network and
-the forward method to pass data through it
-"""
 net_parameters_dic = {
-    'num_channels': 2,
-    'drop_rate': 0,
+    'model': nets.GammaPhysNet,
+    'parameters': {
+        'backbone': {
+            'model': nets.ResNetAttention,
+            'parameters': {
+                'num_layers': 3,
+                'init': 'kaiming',
+                'batch_norm': True,
+                'num_channels': 2,
+                'block_features': [16, 32, 64],
+                'attention_layer': (nets.DualAttention, {'ratio': 16}),
+                'non_linearity': torch.nn.ReLU,
+                'output_size': (14, 14)
+            }
+        },
+        'fc_width': 256,
+        'non_linearity': torch.nn.ReLU,
+        'last_bias_init': None,
+        'targets': {k: v.get('output_shape', 0) for k, v in targets.items()}
+    }
 }
 """dict: mandatory, the parameters of the network. Depends on the
-network chosen
+network chosen. Must include at least a model and a parameters field.
 """
 # checkpoint_path = main_directory + '/test_install/checkpoint_epoch=3.ckpt'
 """str: optional, the path where to find the backup of the model to resume"""
 
-# profiler = {'profiler': PyTorchProfiler,
-#             'options': dict(activities=[torch.profiler.ProfilerActivity.CUDA,
-#                                         torch.profiler.ProfilerActivity.CPU],
-#                             profiled_functions=['training_step_and_backward',
-#                                                 'training_step',
-#                                                 'backward',
-#                                                 'validation_step',
-#                                                 'test_step',
-#                                                 'predict_step',
-#                                                 'IndexedConv'
-#                                                 ])
+profiler = None
+# profiler = {'profiler': SimpleProfiler,
+#             'options': dict(extended=True)
 #             }
-profiler = {'profiler': SimpleProfiler,
-            'options': dict(extended=True)
-            }
 """str: optional, the profiler to use"""
 
 ######################################################################################################################
 train = True
 """bool: mandatory, whether or not to train the model"""
 # Data settings
-train_folders = [
-    Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
-]  # TODO fill your folder path
-"""list: mandatory, the folders where to find the hdf5 data files"""
+data_module_train = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
+        ], # TODO fill your folder path
+        'image_filter': {
+            # utils.intensity_filter: {'intensity': [50, np.inf]},
+            # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': dsets.ResampleImage('bicubic_interpolation', (55, 55, 1)),
+        'target_transform': None
+    },
+    'target': {
+        'paths': [],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': None,
+        'target_transform': None
+    }
+}
+"""paths->list: mandatory, the folders where to find the hdf5 data files"""
+"""image_filter->dict: optional, the filter(s) to apply to the dataset at image level"""
+"""event_filter->dict: optional, the filter(s) to apply to the dataset"""
 
 validating_ratio = 0.2
 """float: mandatory, the ratio of data to create the validating set"""
 split_by_file = False
 """bool: optional, whether to split data at the file level or at the data level"""
 max_epochs = 4
 """int: mandatory, the maximum number of epochs for the experiment"""
 batch_size = 8
 """int: mandatory, the size of the mini-batch"""
-image_filter = {
-    # utils.intensity_filter: {'intensity': [50, np.inf]},
-    # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset at image level"""
-event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset"""
-
-# data_augment = {'function': dsets.augment_via_rotation,
-#                 'kwargs': {'thetas': [2 * math.pi / 3, 4 * math.pi / 3],
-#                            'num_workers': 8}
-#                 }
-"""dict: optional, dictionary describing the function to use for dataset augmentation"""
 # dataset_size = 2000
 """int: optional, the max size of the dataset"""
 # files_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 
 pin_memory = True
 """bool: optional, whether or not to pin memory in dataloader"""
@@ -229,20 +242,20 @@
     'network': optimizers.load_sgd,
     'loss_balancing': optimizers.load_adam
 }
 """dict: mandatory, the optimizers to use for the experiment.
 One may want to use several optimizers in case of GAN for example
 """
 optimizer_parameters = {
-    'network': {'learning_rate': 1e-4,
+    'network': {'lr': 1e-4,
                 'weight_decay': 1e-7,
                 'momentum': 0.9,
                 'nesterov': True
                 },
-    'loss_balancing': {'learning_rate': 0.025,
+    'loss_balancing': {'lr': 0.025,
                        'weight_decay': 1e-4,
                        },
 }
 """dict: mandatory, defines the parameters for every optimizers to use"""
 # regularization = {'function': 'gradient_penalty',
 #                   'weight': 10}
 """dict: optional, regularization to use during the training process. See in optimizers.py for 
@@ -253,29 +266,37 @@
 # training_step = steps.training_step_mt_gradient_penalty
 """function: mandatory, the function to compute the training step"""
 eval_step = steps.eval_step_mt
 """function: mandatory, the function to compute the validating step"""
 check_val_every_n_epoch = 1
 """int: optional, the interval in term of epoch for validating the model"""
 lr_schedulers = {
-    lr_scheduler.StepLR: {'network': {'gamma': 0.1,
-                                      'step_size': 10,
-                                      },
-                          },
-    # lr_scheduler.ReduceLROnPlateau: {'network': {'factor': 0.1,
-    #                                              'patience': 30,
-    #                                              },
-    #                                  },
-    # lr_scheduler.MultiStepLR: {'network': {'gamma': 0.1,
-    #                                        'milestones': [10, 15, 18],
-    #                                        },
-    #                            },
-    # lr_scheduler.ExponentialLR: {'network': {'gamma': 0.9,
-    #                                          },
-    #                              },
+    'network': {
+        lr_scheduler.StepLR: {
+            'gamma': 0.1,
+            'step_size': 10,
+        }
+    },
+    # 'network': {
+    #     lr_scheduler.ReduceLROnPlateau: {
+    #         'factor': 0.1,
+    #         'patience': 30,
+    #     }
+    # },
+    # 'network': {
+    #     lr_scheduler.MultiStepLR: {
+    #         'gamma': 0.1,
+    #         'milestones': [10, 15, 18],
+    #     }
+    # },
+    # 'network': {
+    #     lr_scheduler.ExponentialLR: {
+    #         'gamma': 0.9,
+    #     }
+    # },
 }
 """dict: optional, defines the learning rate schedulers"""
 # callbacks
 training_callbacks = [
     LogGradientNorm(),
     LogModelWeightNorm(),
     LogModelParameters(),
@@ -288,45 +309,62 @@
 """dict: list of callbacks
 """
 
 ######################################################################################################################
 # Testing settings
 test = True
 """bool: mandatory, whether or not to test the model at the end of training"""
+merge_test_datasets = False
+"""bool: optional, whether or not to merge test datasets"""
+data_module_test = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
+        ],
+        'image_filter': {
+            utils.intensity_filter: {'intensity': [10, np.inf]},
+            # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': dsets.ResampleImage('bicubic_interpolation', (55, 55, 1)),
+        'target_transform': None
+    },
+    'target': {
+        'paths': [],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': None,
+        'target_transform': None
+    }
+}
+"""
+dict: optional, must at least contain a non-empty 'source':{'paths:[]'}
+path->list of str: optional, the folders containing the hdf5 data files for the test
+image_filter->dict: optional, filter(s) to apply to the test set at image level
+event_filter->dict: optional, filter(s) to apply to the test set
+"""
+
 test_step = steps.test_step_mt
 """function: mandatory, the function to compute the validating step"""
-test_folders = [
-    Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
-]
-"""list of str: optional, the folders containing the hdf5 data files for the test
-"""
 dl2_path = ''
 """str: optional, path to store dl2 files"""
 test_dataset_parameters = {
     # 'subarray': [1],
 }
-"""dict: optional, the parameters of the dataset specific to the test operation.
-"""
-test_image_filter = {
-    utils.intensity_filter: {'intensity': [10, np.inf]},
-    # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, filter(s) to apply to the test set at image level"""
-test_event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, filter(s) to apply to the test set"""
+"""dict: optional, the parameters of the dataset specific to the test operation."""
 # test_file_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 test_batch_size = 10
 """int: optional, the size of the mini-batch for the test"""
 test_callbacks = [
     WriteDL2Files()
 ]
-"""dict: list of callbacks
-"""
+"""dict: list of callbacks"""
```

### Comparing `Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_test_MC.py` & `Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_domain_adaptation.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import importlib
 from pathlib import Path
 import math
 import numpy as np
 import torch
 from torch.optim import lr_scheduler
+from torchvision import transforms
 
 from torchmetrics.classification import Accuracy, AUROC
 from pytorch_lightning.profiler import SimpleProfiler, AdvancedProfiler, PyTorchProfiler
 
 import gammalearn.criterions as criterions
 import gammalearn.optimizers as optimizers
 import gammalearn.steps as steps
@@ -19,190 +20,235 @@
 import gammalearn.utils as utils
 import gammalearn.datasets as dsets
 from gammalearn.constants import GAMMA_ID, PROTON_ID, ELECTRON_ID
 from gammalearn.metrics import AUCMultiClass
 
 
 # Experiment settings
-main_directory = str(Path.home()) + '/gammalearn_experiments'  # TODO change directory if needed
+# TODO change directory if needed
+main_directory = str(Path.home()) + '/gammalearn_experiments/'
 """str: mandatory, where the experiments are stored"""
 experiment_name = 'test_install'
 """str: mandatory, the name of the experiment. Should be different
 for each experiment, except if one wants to resume an old experiment
 """
 info = ''
 """str: optional"""
-gpus = None
+gpus = 1
 """int or list: mandatory, the umber of gpus to use. If -1, run on all GPUS, 
 if None/0 run on CPU. If list, run on GPUS of list.
 """
-log_every_n_steps = 3
+log_every_n_steps = 1
 """int: optional, the interval in term of iterations for on screen
 data printing during experiment
 """
 window_size = 100
 """int: optional, the interval in term of stored values for metric moving computation"""
 save_every = 1
 """int: optional, the interval in term of epochs for saving the model parameters.
 If save_every < 1, the model is not saved.
 If not provided, the model is not saved.
-"""
+""" 
 random_seed = 1
 """int: optional, the manual seed to make experiments more reproducible"""
 monitor_gpus = True
 """bool: optional, whether or not monitoring the gpu utilization"""
-
-dataset_class = dsets.MemoryLSTDataset
-# dataset_class = dsets.FileLSTDataset
-"""Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
-loads images in memory, and FileLSTDataset that loads images from files during training.
-"""
-dataset_parameters = {'camera_type': 'LST_LSTCam',
-                      'group_by': 'image',
-                      'use_time': True,
-                      'particle_dict': {GAMMA_ID: 0,
-                                        PROTON_ID: 1,
-                                        # ELECTRON_ID: 2,
-                                        },
-                      # 'subarray': [1],
-                      }
-"""dict: mandatory, the parameters of the dataset.
-camera_type is mandatory and can be:
-'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
-group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
-particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0, 
-proton (101) is class 1 and electron (1) is class 2.
-use_time (optional): whether or not to use time information
-subarray (optional): the list of telescope ids to select as a subarray
-"""
-data_transform = {'data': [dsets.NumpyToTensor(),
-                           ],
-                  'target': [
-                      dsets.NumpyToTensor()
-                  ],
-                  'telescope': [
-                      dsets.NumpyToTensor()
-                  ]
-                  }
-"""dict: optional, dictionary of transform functions to apply to the samples of data from the Dataset"""
-preprocessing_workers = 4
-"""int: optional, the max number of workers to create dataset."""
-dataloader_workers = 4
-"""int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
-mp_start_method = 'fork'
-"""str: optional, the method to start new process in [fork, spawn]"""
+particle_dict = {GAMMA_ID: 0,
+                 PROTON_ID: 1,
+                 # ELECTRON_ID: 2,
+                 }
+"""particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0"""
 targets = collections.OrderedDict({
     'energy': {
         'output_shape': 1,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
         'metrics': {
             # 'functions': ,
-        }
+        },
+        'mt_balancing': True
     },
     'impact': {
         'output_shape': 2,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
-        'metrics': {}
+        'metrics': {},
+        'mt_balancing': True
     },
     'direction': {
         'output_shape': 2,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
-        'metrics': {}
+        'metrics': {},
+        'mt_balancing': True
     },
     'class': {
         'label_shape': 1,
-        'loss': criterions.nll_nn,
+        'output_shape': len(particle_dict),
+        'loss': torch.nn.CrossEntropyLoss(),
         'loss_weight': 1,
         'metrics': {
-            'Accuracy': Accuracy(threshold=0.5),
-            'AUC': AUCMultiClass(buffer_size=window_size,
+            'Accuracy_particle': Accuracy(threshold=0.5),
+            'AUC_particle': AUCMultiClass(buffer_size=window_size,
                                  compute_on_step=True),
             # 'AUC': AUROC(pos_label=dataset_parameters['particle_dict'][GAMMA_ID],
             #              num_classes=len(dataset_parameters['particle_dict']),
             #              compute_on_step=True
             #              )
-        }
+        },
+        'mt_balancing': True
     },
+    'domain_class': {
+        'metrics': {
+            'Accuracy_domain': Accuracy(threshold=0.5),
+            'AUC_domain': AUCMultiClass(buffer_size=window_size,
+                                 compute_on_step=True)
+        },
+        'mt_balancing': False
+    }
 })
 """dict: mandatory, defines for every objectives of the experiment
 the loss function and its weight
 """
 
+dataset_class = dsets.MemoryLSTDataset
+# dataset_class = dsets.FileLSTDataset
+"""Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
+loads images in memory, and FileLSTDataset that loads images from files during training.
+"""
+dataset_parameters = {
+    'camera_type': 'LST_LSTCam',
+    'group_by': 'image',
+    'use_time': True,
+    'particle_dict': particle_dict,
+    'targets': list(targets.keys()),
+    # 'subarray': [1],
+}
+"""dict: mandatory, the parameters of the dataset.
+camera_type is mandatory and can be:
+'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
+group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
+particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0, 
+proton (101) is class 1 and electron (1) is class 2.
+use_time (optional): whether or not to use time information
+subarray (optional): the list of telescope ids to select as a subarray
+"""
+preprocessing_workers = 4
+"""int: optional, the max number of workers to create dataset."""
+dataloader_workers = 4
+"""int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
+mp_start_method = 'fork'
+"""str: optional, the method to start new process in [fork, spawn]"""
+
 # Net settings
 net_definition_file = utils.nets_definition_path()
 """str: mandatory, the file where to find the net definition to use"""
 # Load the network definitions module #
 spec = importlib.util.spec_from_file_location("nets", net_definition_file)
 nets = importlib.util.module_from_spec(spec)
 spec.loader.exec_module(nets)
 ########################################
-model_net = nets.GLNetIndexConv42
-"""nn.Module: mandatory, the network for the experiment. Is a class
-inheriting from nn.Module defining the operations of the network and
-the forward method to pass data through it
-"""
 net_parameters_dic = {
-    'num_channels': 2,
-    'n_features': 16,
-    'batchnorm': True,
-    'drop_rate': 0,
+    'model': nets.DANN,
+    'parameters': {
+        'main_task': {
+            'model': nets.GammaPhysNet,
+            'parameters': {
+                'backbone': {
+                    'model': nets.ResNetAttention,
+                    'parameters': {
+                        'num_layers': 3,
+                        'init': 'kaiming',
+                        'batch_norm': True,
+                        # 'init': 'orthogonal',
+                        'num_channels': 2,
+                        'block_features': [16, 32, 64],
+                        'attention_layer': (nets.DualAttention, {'ratio': 16}),
+                        # 'attention_layer': (nets.SqueezeExcite, {'ratio': 4}),
+                        # 'attention_layer': None,
+                        'non_linearity': torch.nn.ReLU,
+                        'output_size': (14, 14)
+                    }
+                },
+                'fc_width': 256,
+                'non_linearity': torch.nn.ReLU,
+                'last_bias_init': None,
+                'targets': {k: v.get('output_shape', 0) for k, v in targets.items()}
+            },
+        },
+        'fc1_features': 100,
+
+    },
 }
+
 """dict: mandatory, the parameters of the network. Depends on the
-network chosen
+network chosen. Must include at least a model and a parameters field.
 """
-checkpoint_path = main_directory + '/test_install/checkpoint_epoch=3.ckpt'
+# checkpoint_path = main_directory + '/test_install/checkpoint_epoch=3.ckpt'
 """str: optional, the path where to find the backup of the model to resume"""
 
 profiler = None
 # profiler = {'profiler': SimpleProfiler,
 #             'options': dict(extended=True)
 #             }
 """str: optional, the profiler to use"""
 
 ######################################################################################################################
-train = False
+train = True
 """bool: mandatory, whether or not to train the model"""
 # Data settings
-train_folders = [
-    Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
-]  # TODO fill your folder path
-"""list: mandatory, the folders where to find the hdf5 data files"""
+data_module_train = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath(
+                '../../../share/data/MC_data').resolve().as_posix(),
+        ],  # TODO fill your folder path
+        'image_filter': {
+            # utils.intensity_filter: {'intensity': [50, np.inf]},
+            # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': dsets.ResampleImage('bilinear_interpolation', (55, 55, 1)),
+        'target_transform': None
+    },
+    'target': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath(
+                '../../../share/data/real_data').resolve().as_posix(),
+        ],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': transforms.Compose([
+            dsets.AddPoissonNoise(0.4),
+            dsets.ResampleImage('bilinear_interpolation', (55, 55, 1))
+        ]),
+        'target_transform': None
+    }
+}
+"""paths->list: mandatory, the folders where to find the hdf5 data files"""
+"""image_filter->dict: optional, the filter(s) to apply to the dataset at image level"""
+"""event_filter->dict: optional, the filter(s) to apply to the dataset"""
 
 validating_ratio = 0.2
 """float: mandatory, the ratio of data to create the validating set"""
 split_by_file = False
 """bool: optional, whether to split data at the file level or at the data level"""
 max_epochs = 4
 """int: mandatory, the maximum number of epochs for the experiment"""
-batch_size = 8
+batch_size = 4
 """int: mandatory, the size of the mini-batch"""
-image_filter = {
-    # utils.intensity_filter: {'intensity': [50, np.inf]},
-    # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset at image level"""
-event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset"""
-
-# data_augment = {'function': dsets.augment_via_rotation,
-#                 'kwargs': {'thetas': [2 * math.pi / 3, 4 * math.pi / 3],
-#                            'num_workers': 8}
-#                 }
-"""dict: optional, dictionary describing the function to use for dataset augmentation"""
 # dataset_size = 2000
 """int: optional, the max size of the dataset"""
 # files_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 
 pin_memory = True
 """bool: optional, whether or not to pin memory in dataloader"""
@@ -217,60 +263,66 @@
 }
 """dict: mandatory, defines for every objectives of the experiment
 the loss function and its weight
 """
 compute_loss = criterions.MultilossBalancing(targets, **loss_options)
 """function: mandatory, the function to compute the loss"""
 optimizer_dic = {
-    'network': optimizers.load_sgd,
+    # 'network': optimizers.load_sgd,
+    'main_task_model': optimizers.load_sgd,
+    'domain_classifier': optimizers.load_sgd,
     'loss_balancing': optimizers.load_adam
 }
 """dict: mandatory, the optimizers to use for the experiment.
 One may want to use several optimizers in case of GAN for example
 """
+mu_0 = 1e-2
 optimizer_parameters = {
-    'network': {'learning_rate': 1e-4,
-                'weight_decay': 1e-7,
-                'momentum': 0.9,
-                'nesterov': True
-                },
-    'loss_balancing': {'learning_rate': 0.025,
-                       'weight_decay': 1e-4,
-                       },
+    'main_task_model': {
+        'lr': mu_0,
+        'weight_decay': 1e-4,
+        'momentum': 0.9,
+        # 'nesterov': True
+    },
+    'domain_classifier': {
+        'lr': mu_0,
+        'weight_decay': 1e-4,
+        'momentum': 0.9,
+        # 'nesterov': True
+    },
+    'loss_balancing': {
+        'lr': 0.025,
+        'weight_decay': 1e-4,
+    },
 }
 """dict: mandatory, defines the parameters for every optimizers to use"""
 # regularization = {'function': 'gradient_penalty',
 #                   'weight': 10}
 """dict: optional, regularization to use during the training process. See in optimizers.py for 
 available regularization functions. If `function` is set to 'gradient_penalty', the training step must be 
 `training_step_mt_gradient_penalty`."""
-training_step = steps.training_step_mt
+training_step = steps.training_step_dann
 # training_step = steps.training_step_gradnorm
 # training_step = steps.training_step_mt_gradient_penalty
 """function: mandatory, the function to compute the training step"""
-eval_step = steps.eval_step_mt
+eval_step = steps.eval_step_dann
 """function: mandatory, the function to compute the validating step"""
 check_val_every_n_epoch = 1
 """int: optional, the interval in term of epoch for validating the model"""
 lr_schedulers = {
-    lr_scheduler.StepLR: {'network': {'gamma': 0.1,
-                                      'step_size': 10,
-                                      },
-                          },
-    # lr_scheduler.ReduceLROnPlateau: {'network': {'factor': 0.1,
-    #                                              'patience': 30,
-    #                                              },
-    #                                  },
-    # lr_scheduler.MultiStepLR: {'network': {'gamma': 0.1,
-    #                                        'milestones': [10, 15, 18],
-    #                                        },
-    #                            },
-    # lr_scheduler.ExponentialLR: {'network': {'gamma': 0.9,
-    #                                          },
-    #                              },
+    'main_task_model': {
+        optimizers.DANNLR: {
+            "domain_classifier": False
+        }
+    },
+    'domain_classifier': {
+        optimizers.DANNLR: {
+            "domain_classifier": True
+        }
+    },
 }
 """dict: optional, defines the learning rate schedulers"""
 # callbacks
 training_callbacks = [
     LogGradientNorm(),
     LogModelWeightNorm(),
     LogModelParameters(),
@@ -283,45 +335,67 @@
 """dict: list of callbacks
 """
 
 ######################################################################################################################
 # Testing settings
 test = True
 """bool: mandatory, whether or not to test the model at the end of training"""
-test_step = steps.test_step_mt
-"""function: mandatory, the function to compute the validating step"""
-test_folders = [
-    Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
-]
-"""list of str: optional, the folders containing the hdf5 data files for the test
+merge_test_datasets = False
+"""bool: optional, whether or not to merge test datasets"""
+data_module_test = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath(
+                '../../../share/data/MC_data').resolve().as_posix(),
+        ],
+        'image_filter': {
+            utils.intensity_filter: {'intensity': [10, np.inf]},
+            # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': dsets.ResampleImage('bilinear_interpolation', (55, 55, 1))
+    },
+    'target': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath(
+                '../../../share/data/real_data').resolve().as_posix(),
+        ],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': transforms.Compose([
+                    dsets.AddPoissonNoise(0.4),
+                    dsets.ResampleImage('bilinear_interpolation', (55, 55, 1))
+                ]),
+    }
+}
+"""
+dict: optional, must at least contain a non-empty 'source':{'paths:[]'}
+path->list of str: optional, the folders containing the hdf5 data files for the test
+image_filter->dict: optional, filter(s) to apply to the test set at image level
+event_filter->dict: optional, filter(s) to apply to the test set
 """
+
+test_step = steps.test_step_dann
+"""function: mandatory, the function to compute the validating step"""
 dl2_path = ''
 """str: optional, path to store dl2 files"""
 test_dataset_parameters = {
     # 'subarray': [1],
 }
-"""dict: optional, the parameters of the dataset specific to the test operation.
-"""
-test_image_filter = {
-    utils.intensity_filter: {'intensity': [10, np.inf]},
-    # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, filter(s) to apply to the test set at image level"""
-test_event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, filter(s) to apply to the test set"""
-# test_file_max_number = 1
+"""dict: optional, the parameters of the dataset specific to the test operation."""
+test_file_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 test_batch_size = 10
 """int: optional, the size of the mini-batch for the test"""
 test_callbacks = [
     WriteDL2Files()
 ]
-"""dict: list of callbacks
-"""
+"""dict: list of callbacks"""
```

### Comparing `Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_test_real.py` & `Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_train_MC.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,201 +19,210 @@
 import gammalearn.utils as utils
 import gammalearn.datasets as dsets
 from gammalearn.constants import GAMMA_ID, PROTON_ID, ELECTRON_ID
 from gammalearn.metrics import AUCMultiClass
 
 
 # Experiment settings
-main_directory = str(Path.home()) + '/gammalearn_experiments'  # TODO change directory if needed
+main_directory = str(Path.home()) + '/gammalearn_experiments/'  # TODO change directory if needed
 """str: mandatory, where the experiments are stored"""
 experiment_name = 'test_install'
 """str: mandatory, the name of the experiment. Should be different
 for each experiment, except if one wants to resume an old experiment
 """
 info = ''
 """str: optional"""
-gpus = None
+gpus = 1
 """int or list: mandatory, the umber of gpus to use. If -1, run on all GPUS, 
 if None/0 run on CPU. If list, run on GPUS of list.
 """
-log_every_n_steps = 3
+log_every_n_steps = 5
 """int: optional, the interval in term of iterations for on screen
 data printing during experiment
 """
 window_size = 100
 """int: optional, the interval in term of stored values for metric moving computation"""
 save_every = 1
 """int: optional, the interval in term of epochs for saving the model parameters.
 If save_every < 1, the model is not saved.
 If not provided, the model is not saved.
 """
 random_seed = 1
 """int: optional, the manual seed to make experiments more reproducible"""
 monitor_gpus = True
 """bool: optional, whether or not monitoring the gpu utilization"""
-
-dataset_class = dsets.MemoryLSTDataset
-# dataset_class = dsets.FileLSTDataset
-"""Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
-loads images in memory, and FileLSTDataset that loads images from files during training.
-"""
-dataset_parameters = {'camera_type': 'LST_LSTCam',
-                      'group_by': 'image',
-                      'use_time': True,
-                      'particle_dict': {GAMMA_ID: 0,
-                                        PROTON_ID: 1,
-                                        # ELECTRON_ID: 2,
-                                        },
-                      # 'subarray': [1],
-                      }
-"""dict: mandatory, the parameters of the dataset.
-camera_type is mandatory and can be:
-'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
-group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
-particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0, 
-proton (101) is class 1 and electron (1) is class 2.
-use_time (optional): whether or not to use time information
-subarray (optional): the list of telescope ids to select as a subarray
-"""
-data_transform = {'data': [dsets.NumpyToTensor(),
-                           ],
-                  'target': [
-                      dsets.NumpyToTensor()
-                  ],
-                  'telescope': [
-                      dsets.NumpyToTensor()
-                  ]
-                  }
-"""dict: optional, dictionary of transform functions to apply to the samples of data from the Dataset"""
-preprocessing_workers = 4
-"""int: optional, the max number of workers to create dataset."""
-dataloader_workers = 4
-"""int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
-mp_start_method = 'fork'
-"""str: optional, the method to start new process in [fork, spawn]"""
+particle_dict = {GAMMA_ID: 0,
+                 PROTON_ID: 1,
+                 # ELECTRON_ID: 2,
+                 }
+"""particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0"""
 targets = collections.OrderedDict({
     'energy': {
         'output_shape': 1,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
         'metrics': {
             # 'functions': ,
-        }
+        },
+        'mt_balancing': True
     },
     'impact': {
         'output_shape': 2,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
-        'metrics': {}
+        'metrics': {},
+        'mt_balancing': True
     },
     'direction': {
         'output_shape': 2,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
-        'metrics': {}
+        'metrics': {},
+        'mt_balancing': True
     },
     'class': {
         'label_shape': 1,
-        'loss': criterions.nll_nn,
+        'output_shape': len(particle_dict),
+        'loss': torch.nn.CrossEntropyLoss(label_smoothing=0.1),
         'loss_weight': 1,
         'metrics': {
-            'Accuracy': Accuracy(threshold=0.5),
-            'AUC': AUCMultiClass(buffer_size=window_size,
+            'Accuracy_particle': Accuracy(threshold=0.5),
+            'AUC_particle': AUCMultiClass(buffer_size=window_size,
                                  compute_on_step=True),
             # 'AUC': AUROC(pos_label=dataset_parameters['particle_dict'][GAMMA_ID],
             #              num_classes=len(dataset_parameters['particle_dict']),
             #              compute_on_step=True
             #              )
-        }
-    },
+        },
+        'mt_balancing': True
+    }
 })
 """dict: mandatory, defines for every objectives of the experiment
 the loss function and its weight
 """
 
+dataset_class = dsets.MemoryLSTDataset
+# dataset_class = dsets.FileLSTDataset
+"""Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
+loads images in memory, and FileLSTDataset that loads images from files during training.
+"""
+dataset_parameters = {
+    'camera_type': 'LST_LSTCam',
+    'group_by': 'image',
+    'use_time': True,
+    'particle_dict': particle_dict,
+    'targets': list(targets.keys()),
+    # 'subarray': [1],
+}
+"""dict: mandatory, the parameters of the dataset.
+camera_type is mandatory and can be:
+'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
+group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
+particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0, 
+proton (101) is class 1 and electron (1) is class 2.
+use_time (optional): whether or not to use time information
+subarray (optional): the list of telescope ids to select as a subarray
+"""
+preprocessing_workers = 4
+"""int: optional, the max number of workers to create dataset."""
+dataloader_workers = 4
+"""int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
+mp_start_method = 'fork'
+"""str: optional, the method to start new process in [fork, spawn]"""
+
 # Net settings
 net_definition_file = utils.nets_definition_path()
 """str: mandatory, the file where to find the net definition to use"""
 # Load the network definitions module #
 spec = importlib.util.spec_from_file_location("nets", net_definition_file)
 nets = importlib.util.module_from_spec(spec)
 spec.loader.exec_module(nets)
 ########################################
-model_net = nets.GLNetIndexConv42
-"""nn.Module: mandatory, the network for the experiment. Is a class
-inheriting from nn.Module defining the operations of the network and
-the forward method to pass data through it
-"""
 net_parameters_dic = {
-    'num_channels': 2,
-    'n_features': 16,
-    'batchnorm': True,
-    'drop_rate': 0,
+    'model': nets.GammaPhysNet,
+    'parameters': {
+        'backbone': {
+            'model': nets.ResNetAttentionIndexed,
+            'parameters': {
+                'num_layers': 3,
+                'init': 'kaiming',
+                'batch_norm': True,
+                # 'init': 'orthogonal',
+                'num_channels': 2,
+                'block_features': [16, 32, 64],
+                'attention_layer': (nets.DualAttention, {'ratio': 16}),
+                # 'attention_layer': (nets.SqueezeExcite, {'ratio': 4}),
+                # 'attention_layer': None,
+                'non_linearity': torch.nn.ReLU,
+            }
+        },
+        'fc_width': 256,
+        'non_linearity': torch.nn.ReLU,
+        'last_bias_init': None,
+        'targets': {k: v.get('output_shape', 0) for k, v in targets.items()}
+    }
 }
 """dict: mandatory, the parameters of the network. Depends on the
-network chosen
+network chosen. Must include at least a model and a parameters field.
 """
 # checkpoint_path = main_directory + '/test_install/checkpoint_epoch=3.ckpt'
 """str: optional, the path where to find the backup of the model to resume"""
 
-# profiler = {'profiler': PyTorchProfiler,
-#             'options': dict(activities=[torch.profiler.ProfilerActivity.CUDA,
-#                                         torch.profiler.ProfilerActivity.CPU],
-#                             profiled_functions=['training_step_and_backward',
-#                                                 'training_step',
-#                                                 'backward',
-#                                                 'validation_step',
-#                                                 'test_step',
-#                                                 'predict_step',
-#                                                 'IndexedConv'
-#                                                 ])
+profiler = None
+# profiler = {'profiler': SimpleProfiler,
+#             'options': dict(extended=True)
 #             }
-profiler = {'profiler': SimpleProfiler,
-            'options': dict(extended=True)
-            }
 """str: optional, the profiler to use"""
 
 ######################################################################################################################
 train = True
 """bool: mandatory, whether or not to train the model"""
 # Data settings
-train_folders = [
-    Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
-]  # TODO fill your folder path
-"""list: mandatory, the folders where to find the hdf5 data files"""
+data_module_train = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
+        ], # TODO fill your folder path
+        'image_filter': {
+            # utils.intensity_filter: {'intensity': [50, np.inf]},
+            # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': None,
+        'target_transform': None
+    },
+    'target': {
+        'paths': [],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': None,
+        'target_transform': None
+    }
+}
+"""paths->list: mandatory, the folders where to find the hdf5 data files"""
+"""image_filter->dict: optional, the filter(s) to apply to the dataset at image level"""
+"""event_filter->dict: optional, the filter(s) to apply to the dataset"""
 
 validating_ratio = 0.2
 """float: mandatory, the ratio of data to create the validating set"""
 split_by_file = False
 """bool: optional, whether to split data at the file level or at the data level"""
 max_epochs = 4
 """int: mandatory, the maximum number of epochs for the experiment"""
 batch_size = 8
 """int: mandatory, the size of the mini-batch"""
-image_filter = {
-    # utils.intensity_filter: {'intensity': [50, np.inf]},
-    # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset at image level"""
-event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset"""
-
-# data_augment = {'function': dsets.augment_via_rotation,
-#                 'kwargs': {'thetas': [2 * math.pi / 3, 4 * math.pi / 3],
-#                            'num_workers': 8}
-#                 }
-"""dict: optional, dictionary describing the function to use for dataset augmentation"""
 # dataset_size = 2000
 """int: optional, the max size of the dataset"""
 # files_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 
 pin_memory = True
 """bool: optional, whether or not to pin memory in dataloader"""
@@ -228,27 +237,28 @@
 }
 """dict: mandatory, defines for every objectives of the experiment
 the loss function and its weight
 """
 compute_loss = criterions.MultilossBalancing(targets, **loss_options)
 """function: mandatory, the function to compute the loss"""
 optimizer_dic = {
-    'network': optimizers.load_sgd,
+    # 'network': optimizers.load_sgd,
+    'network': optimizers.load_adam,
     'loss_balancing': optimizers.load_adam
 }
 """dict: mandatory, the optimizers to use for the experiment.
 One may want to use several optimizers in case of GAN for example
 """
 optimizer_parameters = {
-    'network': {'learning_rate': 1e-4,
+    'network': {'lr': 1e-2,
                 'weight_decay': 1e-7,
-                'momentum': 0.9,
-                'nesterov': True
+                # 'momentum': 0.9,
+                # 'nesterov': True
                 },
-    'loss_balancing': {'learning_rate': 0.025,
+    'loss_balancing': {'lr': 0.025,
                        'weight_decay': 1e-4,
                        },
 }
 """dict: mandatory, defines the parameters for every optimizers to use"""
 # regularization = {'function': 'gradient_penalty',
 #                   'weight': 10}
 """dict: optional, regularization to use during the training process. See in optimizers.py for 
@@ -259,29 +269,37 @@
 # training_step = steps.training_step_mt_gradient_penalty
 """function: mandatory, the function to compute the training step"""
 eval_step = steps.eval_step_mt
 """function: mandatory, the function to compute the validating step"""
 check_val_every_n_epoch = 1
 """int: optional, the interval in term of epoch for validating the model"""
 lr_schedulers = {
-    lr_scheduler.StepLR: {'network': {'gamma': 0.1,
-                                      'step_size': 10,
-                                      },
-                          },
-    # lr_scheduler.ReduceLROnPlateau: {'network': {'factor': 0.1,
-    #                                              'patience': 30,
-    #                                              },
-    #                                  },
-    # lr_scheduler.MultiStepLR: {'network': {'gamma': 0.1,
-    #                                        'milestones': [10, 15, 18],
-    #                                        },
-    #                            },
-    # lr_scheduler.ExponentialLR: {'network': {'gamma': 0.9,
-    #                                          },
-    #                              },
+    'network': {
+        lr_scheduler.StepLR: {
+            'gamma': 0.1,
+            'step_size': 10,
+        }
+    },
+    # 'network': {
+    #     lr_scheduler.ReduceLROnPlateau: {
+    #         'factor': 0.1,
+    #         'patience': 30,
+    #     }
+    # },
+    # 'network': {
+    #     lr_scheduler.MultiStepLR: {
+    #         'gamma': 0.1,
+    #         'milestones': [10, 15, 18],
+    #     }
+    # },
+    # 'network': {
+    #     lr_scheduler.ExponentialLR: {
+    #         'gamma': 0.9,
+    #     }
+    # },
 }
 """dict: optional, defines the learning rate schedulers"""
 # callbacks
 training_callbacks = [
     LogGradientNorm(),
     LogModelWeightNorm(),
     LogModelParameters(),
@@ -294,45 +312,62 @@
 """dict: list of callbacks
 """
 
 ######################################################################################################################
 # Testing settings
 test = True
 """bool: mandatory, whether or not to test the model at the end of training"""
+merge_test_datasets = False
+"""bool: optional, whether or not to merge test datasets"""
+data_module_test = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
+        ],
+        'image_filter': {
+            utils.intensity_filter: {'intensity': [10, np.inf]},
+            # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': None,
+        'target_transform': None
+    },
+    'target': {
+        'paths': [],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': None,
+        'target_transform': None
+    }
+}
+"""
+dict: optional, must at least contain a non-empty 'source':{'paths:[]'}
+path->list of str: optional, the folders containing the hdf5 data files for the test
+image_filter->dict: optional, filter(s) to apply to the test set at image level
+event_filter->dict: optional, filter(s) to apply to the test set
+"""
+
 test_step = steps.test_step_mt
 """function: mandatory, the function to compute the validating step"""
-test_folders = [
-    Path(__file__).parent.absolute().joinpath('../../../share/data/real_data').resolve().as_posix(),
-]
-"""list of str: optional, the folders containing the hdf5 data files for the test
-"""
 dl2_path = ''
 """str: optional, path to store dl2 files"""
 test_dataset_parameters = {
     # 'subarray': [1],
 }
-"""dict: optional, the parameters of the dataset specific to the test operation.
-"""
-test_image_filter = {
-    utils.intensity_filter: {'intensity': [10, np.inf]},
-    # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, filter(s) to apply to the test set at image level"""
-test_event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, filter(s) to apply to the test set"""
-# test_file_max_number = 1
+"""dict: optional, the parameters of the dataset specific to the test operation."""
+test_file_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 test_batch_size = 10
 """int: optional, the size of the mini-batch for the test"""
 test_callbacks = [
     WriteDL2Files()
 ]
-"""dict: list of callbacks
-"""
+"""dict: list of callbacks"""
```

### Comparing `Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_train_MC.py` & `Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_file_spawn.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,198 +19,212 @@
 import gammalearn.utils as utils
 import gammalearn.datasets as dsets
 from gammalearn.constants import GAMMA_ID, PROTON_ID, ELECTRON_ID
 from gammalearn.metrics import AUCMultiClass
 
 
 # Experiment settings
-main_directory = str(Path.home()) + '/gammalearn_experiments/'  # TODO change directory if needed
+main_directory = str(Path.home()) + '/gammalearn_experiments'  # TODO change directory if needed
 """str: mandatory, where the experiments are stored"""
 experiment_name = 'test_install'
 """str: mandatory, the name of the experiment. Should be different
 for each experiment, except if one wants to resume an old experiment
 """
 info = ''
 """str: optional"""
-gpus = 1
+gpus = None
 """int or list: mandatory, the umber of gpus to use. If -1, run on all GPUS, 
 if None/0 run on CPU. If list, run on GPUS of list.
 """
-log_every_n_steps = 5
+log_every_n_steps = 3
 """int: optional, the interval in term of iterations for on screen
 data printing during experiment
 """
 window_size = 100
 """int: optional, the interval in term of stored values for metric moving computation"""
 save_every = 1
 """int: optional, the interval in term of epochs for saving the model parameters.
 If save_every < 1, the model is not saved.
 If not provided, the model is not saved.
 """
 random_seed = 1
 """int: optional, the manual seed to make experiments more reproducible"""
 monitor_gpus = True
 """bool: optional, whether or not monitoring the gpu utilization"""
-
-dataset_class = dsets.MemoryLSTDataset
-# dataset_class = dsets.FileLSTDataset
-"""Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
-loads images in memory, and FileLSTDataset that loads images from files during training.
-"""
-dataset_parameters = {'camera_type': 'LST_LSTCam',
-                      'group_by': 'image',
-                      'use_time': True,
-                      'particle_dict': {GAMMA_ID: 0,
-                                        PROTON_ID: 1,
-                                        # ELECTRON_ID: 2,
-                                        },
-                      # 'subarray': [1],
-                      }
-"""dict: mandatory, the parameters of the dataset.
-camera_type is mandatory and can be:
-'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
-group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
-particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0, 
-proton (101) is class 1 and electron (1) is class 2.
-use_time (optional): whether or not to use time information
-subarray (optional): the list of telescope ids to select as a subarray
-"""
-data_transform = {'data': [dsets.NumpyToTensor(),
-                           ],
-                  'target': [
-                      dsets.NumpyToTensor()
-                  ],
-                  'telescope': [
-                      dsets.NumpyToTensor()
-                  ]
-                  }
-"""dict: optional, dictionary of transform functions to apply to the samples of data from the Dataset"""
-preprocessing_workers = 4
-"""int: optional, the max number of workers to create dataset."""
-dataloader_workers = 4
-"""int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
-mp_start_method = 'fork'
-"""str: optional, the method to start new process in [fork, spawn]"""
+particle_dict = {GAMMA_ID: 0,
+                 PROTON_ID: 1,
+                 # ELECTRON_ID: 2,
+                 }
+"""particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0"""
 targets = collections.OrderedDict({
     'energy': {
         'output_shape': 1,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
         'metrics': {
             # 'functions': ,
-        }
+        },
+        'mt_balancing': True
     },
     'impact': {
         'output_shape': 2,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
-        'metrics': {}
+        'metrics': {},
+        'mt_balancing': True
     },
     'direction': {
         'output_shape': 2,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
-        'metrics': {}
+        'metrics': {},
+        'mt_balancing': True
     },
     'class': {
         'label_shape': 1,
-        'loss': criterions.nll_nn,
+        'output_shape': len(particle_dict),
+        'loss': torch.nn.CrossEntropyLoss(),
         'loss_weight': 1,
         'metrics': {
-            'Accuracy': Accuracy(threshold=0.5),
-            'AUC': AUCMultiClass(buffer_size=window_size,
+            'Accuracy_particle': Accuracy(threshold=0.5),
+            'AUC_particle': AUCMultiClass(buffer_size=window_size,
                                  compute_on_step=True),
             # 'AUC': AUROC(pos_label=dataset_parameters['particle_dict'][GAMMA_ID],
             #              num_classes=len(dataset_parameters['particle_dict']),
             #              compute_on_step=True
             #              )
-        }
-    },
+        },
+        'mt_balancing': True
+    }
 })
 """dict: mandatory, defines for every objectives of the experiment
 the loss function and its weight
 """
 
+# dataset_class = dsets.MemoryLSTDataset
+dataset_class = dsets.FileLSTDataset
+# dataset_class = dsets.MockLSTDataset
+"""Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
+loads images in memory, and FileLSTDataset that loads images from files during training.
+"""
+dataset_parameters = {
+    'camera_type': 'LST_LSTCam',
+    'group_by': 'image',
+    'use_time': True,
+    'particle_dict': particle_dict,
+    'targets': list(targets.keys()),
+    # 'subarray': [1],
+}
+"""dict: mandatory, the parameters of the dataset.
+camera_type is mandatory and can be:
+'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
+group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
+particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0, 
+proton (101) is class 1 and electron (1) is class 2.
+use_time (optional): whether or not to use time information
+subarray (optional): the list of telescope ids to select as a subarray
+"""
+preprocessing_workers = 4
+"""int: optional, the max number of workers to create dataset."""
+dataloader_workers = 4
+"""int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
+mp_start_method = 'spawn'
+"""str: optional, the method to start new process in [fork, spawn]"""
+
 # Net settings
 net_definition_file = utils.nets_definition_path()
 """str: mandatory, the file where to find the net definition to use"""
 # Load the network definitions module #
 spec = importlib.util.spec_from_file_location("nets", net_definition_file)
 nets = importlib.util.module_from_spec(spec)
 spec.loader.exec_module(nets)
 ########################################
-model_net = nets.GammaPhysNet
-"""nn.Module: mandatory, the network for the experiment. Is a class
-inheriting from nn.Module defining the operations of the network and
-the forward method to pass data through it
-"""
 net_parameters_dic = {
-    "num_layers": 3,
-    "init": "kaiming",
-    "batch_norm": True,
-    # "init": "orthogonal",
-    "num_channels": 2,
-    "block_features": [16, 32, 64],
-    "attention_layer": (nets.DualAttention, {"ratio": 16}),
-    # "attention_layer": (nets.SqueezeExcite, {"ratio": 4}),
-    # "attention_layer": None,
-    "fc_width": 256,
-    "non_linearity": torch.nn.ReLU,
-    "last_bias_init": None,
+    'model': nets.GammaPhysNet,
+    'parameters': {
+        'backbone': {
+            'model': nets.ResNetAttentionIndexed,
+            'parameters': {
+                'num_layers': 3,
+                'init': 'kaiming',
+                'batch_norm': True,
+                # 'init': 'orthogonal',
+                'num_channels': 2,
+                'block_features': [16, 32, 64],
+                'attention_layer': (nets.DualAttention, {'ratio': 16}),
+                # 'attention_layer': (nets.SqueezeExcite, {'ratio': 4}),
+                # 'attention_layer': None,
+                'non_linearity': torch.nn.ReLU,
+            }
+        },
+        'fc_width': 256,
+        'non_linearity': torch.nn.ReLU,
+        'last_bias_init': None,
+        'targets': {k: v.get('output_shape', 0) for k, v in targets.items()}
+    }
 }
 """dict: mandatory, the parameters of the network. Depends on the
-network chosen
+network chosen. Must include at least a model and a parameters field.
 """
 # checkpoint_path = main_directory + '/test_install/checkpoint_epoch=3.ckpt'
 """str: optional, the path where to find the backup of the model to resume"""
 
 profiler = None
 # profiler = {'profiler': SimpleProfiler,
 #             'options': dict(extended=True)
 #             }
 """str: optional, the profiler to use"""
 
 ######################################################################################################################
 train = True
 """bool: mandatory, whether or not to train the model"""
 # Data settings
-train_folders = [
-    Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
-]  # TODO fill your folder path
-"""list: mandatory, the folders where to find the hdf5 data files"""
+data_module_train = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
+        ], # TODO fill your folder path
+        'image_filter': {
+            # utils.intensity_filter: {'intensity': [50, np.inf]},
+            # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': None,
+        'target_transform': None
+    },
+    'target': {
+        'paths': [],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': None,
+        'target_transform': None
+    }
+}
+"""paths->list: mandatory, the folders where to find the hdf5 data files"""
+"""image_filter->dict: optional, the filter(s) to apply to the dataset at image level"""
+"""event_filter->dict: optional, the filter(s) to apply to the dataset"""
 
 validating_ratio = 0.2
 """float: mandatory, the ratio of data to create the validating set"""
 split_by_file = False
 """bool: optional, whether to split data at the file level or at the data level"""
-max_epochs = 4
+max_epochs = 1
 """int: mandatory, the maximum number of epochs for the experiment"""
 batch_size = 8
 """int: mandatory, the size of the mini-batch"""
-image_filter = {
-    # utils.intensity_filter: {'intensity': [50, np.inf]},
-    # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset at image level"""
-event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset"""
 
-# data_augment = {'function': dsets.augment_via_rotation,
-#                 'kwargs': {'thetas': [2 * math.pi / 3, 4 * math.pi / 3],
-#                            'num_workers': 8}
-#                 }
-"""dict: optional, dictionary describing the function to use for dataset augmentation"""
 # dataset_size = 2000
 """int: optional, the max size of the dataset"""
 # files_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 
 pin_memory = True
 """bool: optional, whether or not to pin memory in dataloader"""
@@ -225,28 +239,27 @@
 }
 """dict: mandatory, defines for every objectives of the experiment
 the loss function and its weight
 """
 compute_loss = criterions.MultilossBalancing(targets, **loss_options)
 """function: mandatory, the function to compute the loss"""
 optimizer_dic = {
-    # 'network': optimizers.load_sgd,
-    'network': optimizers.load_adam,
+    'network': optimizers.load_sgd,
     'loss_balancing': optimizers.load_adam
 }
 """dict: mandatory, the optimizers to use for the experiment.
 One may want to use several optimizers in case of GAN for example
 """
 optimizer_parameters = {
-    'network': {'learning_rate': 1e-2,
+    'network': {'lr': 1e-4,
                 'weight_decay': 1e-7,
-                # 'momentum': 0.9,
-                # 'nesterov': True
+                'momentum': 0.9,
+                'nesterov': True
                 },
-    'loss_balancing': {'learning_rate': 0.025,
+    'loss_balancing': {'lr': 0.025,
                        'weight_decay': 1e-4,
                        },
 }
 """dict: mandatory, defines the parameters for every optimizers to use"""
 # regularization = {'function': 'gradient_penalty',
 #                   'weight': 10}
 """dict: optional, regularization to use during the training process. See in optimizers.py for 
@@ -257,29 +270,37 @@
 # training_step = steps.training_step_mt_gradient_penalty
 """function: mandatory, the function to compute the training step"""
 eval_step = steps.eval_step_mt
 """function: mandatory, the function to compute the validating step"""
 check_val_every_n_epoch = 1
 """int: optional, the interval in term of epoch for validating the model"""
 lr_schedulers = {
-    # lr_scheduler.StepLR: {'network': {'gamma': 0.1,
-    #                                   'step_size': 2,
-    #                                   },
-    #                       },
-    lr_scheduler.ReduceLROnPlateau: {'network': {'factor': 0.1,
-                                                 'patience': 2,
-                                                 },
-                                     },
-    # lr_scheduler.MultiStepLR: {'network': {'gamma': 0.1,
-    #                                        'milestones': [10, 15, 18],
-    #                                        },
-    #                            },
-    # lr_scheduler.ExponentialLR: {'network': {'gamma': 0.9,
-    #                                          },
-    #                              },
+    'network': {
+        lr_scheduler.StepLR: {
+            'gamma': 0.1,
+            'step_size': 10,
+        }
+    },
+    # 'network': {
+    #     lr_scheduler.ReduceLROnPlateau: {
+    #         'factor': 0.1,
+    #         'patience': 30,
+    #     }
+    # },
+    # 'network': {
+    #     lr_scheduler.MultiStepLR: {
+    #         'gamma': 0.1,
+    #         'milestones': [10, 15, 18],
+    #     }
+    # },
+    # 'network': {
+    #     lr_scheduler.ExponentialLR: {
+    #         'gamma': 0.9,
+    #     }
+    # },
 }
 """dict: optional, defines the learning rate schedulers"""
 # callbacks
 training_callbacks = [
     LogGradientNorm(),
     LogModelWeightNorm(),
     LogModelParameters(),
@@ -292,45 +313,62 @@
 """dict: list of callbacks
 """
 
 ######################################################################################################################
 # Testing settings
 test = True
 """bool: mandatory, whether or not to test the model at the end of training"""
+merge_test_datasets = False
+"""bool: optional, whether or not to merge test datasets"""
+data_module_test = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
+        ],
+        'image_filter': {
+            utils.intensity_filter: {'intensity': [10, np.inf]},
+            # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': None,
+        'target_transform': None
+    },
+    'target': {
+        'paths': [],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': None,
+        'target_transform': None
+    }
+}
+"""
+dict: optional, must at least contain a non-empty 'source':{'paths:[]'}
+path->list of str: optional, the folders containing the hdf5 data files for the test
+image_filter->dict: optional, filter(s) to apply to the test set at image level
+event_filter->dict: optional, filter(s) to apply to the test set
+"""
+
 test_step = steps.test_step_mt
 """function: mandatory, the function to compute the validating step"""
-test_folders = [
-    Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
-]
-"""list of str: optional, the folders containing the hdf5 data files for the test
-"""
 dl2_path = ''
 """str: optional, path to store dl2 files"""
 test_dataset_parameters = {
     # 'subarray': [1],
 }
-"""dict: optional, the parameters of the dataset specific to the test operation.
-"""
-test_image_filter = {
-    utils.intensity_filter: {'intensity': [10, np.inf]},
-    # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, filter(s) to apply to the test set at image level"""
-test_event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, filter(s) to apply to the test set"""
-test_file_max_number = 1
+"""dict: optional, the parameters of the dataset specific to the test operation."""
+# test_file_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 test_batch_size = 10
 """int: optional, the size of the mini-batch for the test"""
 test_callbacks = [
-    WriteDL2Files()
+    # WriteDL2Files()
 ]
-"""dict: list of callbacks
-"""
+"""dict: list of callbacks"""
```

### Comparing `Gammalearn-0.8/gammalearn/data/example_settings/experiment_settings_val.py` & `Gammalearn-0.9/gammalearn/data/example_settings/experiment_settings_square_pixels_over.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,163 +46,178 @@
 If save_every < 1, the model is not saved.
 If not provided, the model is not saved.
 """
 random_seed = 1
 """int: optional, the manual seed to make experiments more reproducible"""
 monitor_gpus = True
 """bool: optional, whether or not monitoring the gpu utilization"""
-
-dataset_class = dsets.MemoryLSTDataset
-# dataset_class = dsets.FileLSTDataset
-"""Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
-loads images in memory, and FileLSTDataset that loads images from files during training.
-"""
-dataset_parameters = {'camera_type': 'LST_LSTCam',
-                      'group_by': 'image',
-                      'use_time': True,
-                      'particle_dict': {GAMMA_ID: 0,
-                                        PROTON_ID: 1,
-                                        # ELECTRON_ID: 2,
-                                        },
-                      # 'subarray': [1],
-                      }
-"""dict: mandatory, the parameters of the dataset.
-camera_type is mandatory and can be:
-'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
-group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
-particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0, 
-proton (101) is class 1 and electron (1) is class 2.
-use_time (optional): whether or not to use time information
-subarray (optional): the list of telescope ids to select as a subarray
-"""
-data_transform = {'data': [dsets.NumpyToTensor(),
-                           ],
-                  'target': [
-                      dsets.NumpyToTensor()
-                  ],
-                  'telescope': [
-                      dsets.NumpyToTensor()
-                  ]
-                  }
-"""dict: optional, dictionary of transform functions to apply to the samples of data from the Dataset"""
-preprocessing_workers = 4
-"""int: optional, the max number of workers to create dataset."""
-dataloader_workers = 4
-"""int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
-mp_start_method = 'fork'
-"""str: optional, the method to start new process in [fork, spawn]"""
+particle_dict = {GAMMA_ID: 0,
+                 PROTON_ID: 1,
+                 # ELECTRON_ID: 2,
+                 }
+"""particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0"""
 targets = collections.OrderedDict({
     'energy': {
         'output_shape': 1,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
         'metrics': {
             # 'functions': ,
-        }
+        },
+        'mt_balancing': True
     },
     'impact': {
         'output_shape': 2,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
-        'metrics': {}
+        'metrics': {},
+        'mt_balancing': True
     },
     'direction': {
         'output_shape': 2,
         'loss': torch.nn.L1Loss(reduction='none'),
         'loss_weight': 1,
-        'metrics': {}
+        'metrics': {},
+        'mt_balancing': True
     },
     'class': {
         'label_shape': 1,
-        'loss': criterions.nll_nn,
+        'output_shape': len(particle_dict),
+        'loss': torch.nn.CrossEntropyLoss(),
         'loss_weight': 1,
         'metrics': {
-            'Accuracy': Accuracy(threshold=0.5),
-            'AUC': AUCMultiClass(buffer_size=window_size,
-                                 compute_on_step=True),
+            'Accuracy_particle': Accuracy(threshold=0.5),
+            'AUC_particle': AUCMultiClass(buffer_size=window_size,
+                                          compute_on_step=True),
             # 'AUC': AUROC(pos_label=dataset_parameters['particle_dict'][GAMMA_ID],
             #              num_classes=len(dataset_parameters['particle_dict']),
             #              compute_on_step=True
             #              )
-        }
-    },
+        },
+        'mt_balancing': True
+    }
 })
 """dict: mandatory, defines for every objectives of the experiment
 the loss function and its weight
 """
 
+dataset_class = dsets.MemoryLSTDataset
+# dataset_class = dsets.FileLSTDataset
+"""Dataset: mandatory, the Dataset class to load the data. Currently 2 classes are available, MemoryLSTDataset that 
+loads images in memory, and FileLSTDataset that loads images from files during training.
+"""
+dataset_parameters = {
+    'camera_type': 'LST_LSTCam',
+    'group_by': 'image',
+    'use_time': True,
+    'particle_dict': particle_dict,
+    'targets': list(targets.keys()),
+    # 'subarray': [1],
+}
+"""dict: mandatory, the parameters of the dataset.
+camera_type is mandatory and can be:
+'LST_LSTCam', 'MST_NectarCam', 'MST_FlashCam', 'SST_ASTRICam', 'SST1M_DigiCam', 'SST_CHEC', 'MST-SCT_SCTCam'.
+group_by is mandatory and can be 'image', 'event_all_tels', 'event_triggered_tels'.
+particle_dict is mandatory and maps cta particle types with class id. e.g. gamma (0) is class 0, 
+proton (101) is class 1 and electron (1) is class 2.
+use_time (optional): whether or not to use time information
+subarray (optional): the list of telescope ids to select as a subarray
+"""
+preprocessing_workers = 4
+"""int: optional, the max number of workers to create dataset."""
+dataloader_workers = 4
+"""int: optional, the max number of workers for the data loaders. If 0, data are loaded from the main thread."""
+mp_start_method = 'fork'
+"""str: optional, the method to start new process in [fork, spawn]"""
+
 # Net settings
 net_definition_file = utils.nets_definition_path()
 """str: mandatory, the file where to find the net definition to use"""
 # Load the network definitions module #
 spec = importlib.util.spec_from_file_location("nets", net_definition_file)
 nets = importlib.util.module_from_spec(spec)
 spec.loader.exec_module(nets)
 ########################################
-model_net = nets.GLNetIndexConv42
-"""nn.Module: mandatory, the network for the experiment. Is a class
-inheriting from nn.Module defining the operations of the network and
-the forward method to pass data through it
-"""
 net_parameters_dic = {
-    'num_channels': 2,
-    'n_features': 16,
-    'batchnorm': True,
-    'drop_rate': 0,
+    'model': nets.ResNet18MT,
+    'parameters': {
+        'num_channels': 2,
+        'drop_rate': 0,
+        'targets': {k: v.get('output_shape', 0) for k, v in targets.items()}
+    }
 }
 """dict: mandatory, the parameters of the network. Depends on the
-network chosen
+network chosen. Must include at least a model and a parameters field.
 """
 # checkpoint_path = main_directory + '/test_install/checkpoint_epoch=3.ckpt'
 """str: optional, the path where to find the backup of the model to resume"""
 
-profiler = None
-# profiler = {'profiler': SimpleProfiler,
-#             'options': dict(extended=True)
+# profiler = {'profiler': PyTorchProfiler,
+#             'options': dict(activities=[torch.profiler.ProfilerActivity.CUDA,
+#                                         torch.profiler.ProfilerActivity.CPU],
+#                             profiled_functions=['training_step_and_backward',
+#                                                 'training_step',
+#                                                 'backward',
+#                                                 'validation_step',
+#                                                 'test_step',
+#                                                 'predict_step',
+#                                                 'IndexedConv'
+#                                                 ])
 #             }
+profiler = {'profiler': SimpleProfiler,
+            'options': dict(extended=True)
+            }
 """str: optional, the profiler to use"""
 
 ######################################################################################################################
 train = True
 """bool: mandatory, whether or not to train the model"""
 # Data settings
-train_folders = [
-    Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
-]  # TODO fill your folder path
-"""list: mandatory, the folders where to find the hdf5 data files"""
+data_module_train = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
+        ], # TODO fill your folder path
+        'image_filter': {
+            # utils.intensity_filter: {'intensity': [50, np.inf]},
+            # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': dsets.ResampleImage('oversampling', (55, 55, 1)),
+        'target_transform': None
+    },
+    'target': {
+        'paths': [],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': None,
+        'target_transform': None
+    }
+}
+"""paths->list: mandatory, the folders where to find the hdf5 data files"""
+"""image_filter->dict: optional, the filter(s) to apply to the dataset at image level"""
+"""event_filter->dict: optional, the filter(s) to apply to the dataset"""
 
 validating_ratio = 0.2
 """float: mandatory, the ratio of data to create the validating set"""
 split_by_file = False
 """bool: optional, whether to split data at the file level or at the data level"""
 max_epochs = 4
 """int: mandatory, the maximum number of epochs for the experiment"""
-batch_size = 4
+batch_size = 8
 """int: mandatory, the size of the mini-batch"""
-image_filter = {
-    # utils.intensity_filter: {'intensity': [50, np.inf]},
-    # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset at image level"""
-event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, the filter(s) to apply to the dataset"""
-
-# data_augment = {'function': dsets.augment_via_rotation,
-#                 'kwargs': {'thetas': [2 * math.pi / 3, 4 * math.pi / 3],
-#                            'num_workers': 8}
-#                 }
-"""dict: optional, dictionary describing the function to use for dataset augmentation"""
 # dataset_size = 2000
 """int: optional, the max size of the dataset"""
 # files_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 
 pin_memory = True
 """bool: optional, whether or not to pin memory in dataloader"""
@@ -224,20 +239,20 @@
     'network': optimizers.load_sgd,
     'loss_balancing': optimizers.load_adam
 }
 """dict: mandatory, the optimizers to use for the experiment.
 One may want to use several optimizers in case of GAN for example
 """
 optimizer_parameters = {
-    'network': {'learning_rate': 1e-4,
+    'network': {'lr': 1e-4,
                 'weight_decay': 1e-7,
                 'momentum': 0.9,
                 'nesterov': True
                 },
-    'loss_balancing': {'learning_rate': 0.025,
+    'loss_balancing': {'lr': 0.025,
                        'weight_decay': 1e-4,
                        },
 }
 """dict: mandatory, defines the parameters for every optimizers to use"""
 # regularization = {'function': 'gradient_penalty',
 #                   'weight': 10}
 """dict: optional, regularization to use during the training process. See in optimizers.py for 
@@ -248,29 +263,37 @@
 # training_step = steps.training_step_mt_gradient_penalty
 """function: mandatory, the function to compute the training step"""
 eval_step = steps.eval_step_mt
 """function: mandatory, the function to compute the validating step"""
 check_val_every_n_epoch = 1
 """int: optional, the interval in term of epoch for validating the model"""
 lr_schedulers = {
-    lr_scheduler.StepLR: {'network': {'gamma': 0.1,
-                                      'step_size': 10,
-                                      },
-                          },
-    # lr_scheduler.ReduceLROnPlateau: {'network': {'factor': 0.1,
-    #                                              'patience': 30,
-    #                                              },
-    #                                  },
-    # lr_scheduler.MultiStepLR: {'network': {'gamma': 0.1,
-    #                                        'milestones': [10, 15, 18],
-    #                                        },
-    #                            },
-    # lr_scheduler.ExponentialLR: {'network': {'gamma': 0.9,
-    #                                          },
-    #                              },
+    'network': {
+        lr_scheduler.StepLR: {
+            'gamma': 0.1,
+            'step_size': 10,
+        }
+    },
+    # 'network': {
+    #     lr_scheduler.ReduceLROnPlateau: {
+    #         'factor': 0.1,
+    #         'patience': 30,
+    #     }
+    # },
+    # 'network': {
+    #     lr_scheduler.MultiStepLR: {
+    #         'gamma': 0.1,
+    #         'milestones': [10, 15, 18],
+    #     }
+    # },
+    # 'network': {
+    #     lr_scheduler.ExponentialLR: {
+    #         'gamma': 0.9,
+    #     }
+    # },
 }
 """dict: optional, defines the learning rate schedulers"""
 # callbacks
 training_callbacks = [
     LogGradientNorm(),
     LogModelWeightNorm(),
     LogModelParameters(),
@@ -283,44 +306,62 @@
 """dict: list of callbacks
 """
 
 ######################################################################################################################
 # Testing settings
 test = True
 """bool: mandatory, whether or not to test the model at the end of training"""
+merge_test_datasets = False
+"""bool: optional, whether or not to merge test datasets"""
+data_module_test = {
+    'module': 'GLearnDataModule',
+    'source': {
+        'paths': [
+            Path(__file__).parent.absolute().joinpath('../../../share/data/MC_data').resolve().as_posix(),
+        ],
+        'image_filter': {
+            utils.intensity_filter: {'intensity': [10, np.inf]},
+            # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
+            # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+            # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
+            #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
+        },
+        'event_filter': {
+            # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
+            # utils.emission_cone_filter: {'max_angle': 0.0698},
+            # utils.impact_distance_filter: {'max_distance': 200},
+            # utils.telescope_multiplicity_filter: {'multiplicity': 2},
+        },
+        'transform': dsets.ResampleImage('oversampling', (55, 55, 1)),
+        'target_transform': None
+    },
+    'target': {
+        'paths': [],
+        'image_filter': {},
+        'event_filter': {},
+        'transform': None,
+        'target_transform': None
+    }
+}
+"""
+dict: optional, must at least contain a non-empty 'source':{'paths:[]'}
+path->list of str: optional, the folders containing the hdf5 data files for the test
+image_filter->dict: optional, filter(s) to apply to the test set at image level
+event_filter->dict: optional, filter(s) to apply to the test set
+"""
+
 test_step = steps.test_step_mt
 """function: mandatory, the function to compute the validating step"""
-test_folders = [
-]
-"""list of str: optional, the folders containing the hdf5 data files for the test
-"""
 dl2_path = ''
 """str: optional, path to store dl2 files"""
 test_dataset_parameters = {
     # 'subarray': [1],
 }
-"""dict: optional, the parameters of the dataset specific to the test operation.
-"""
-test_image_filter = {
-    utils.intensity_filter: {'intensity': [10, np.inf]},
-    # # utils.cleaning_filter: {'picture_thresh': 6, 'boundary_thresh': 3,
-    # #                         'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-    # utils.leakage_filter: {'leakage2_cut': 0.2, 'picture_thresh': 6, 'boundary_thresh': 3,
-    #                        'keep_isolated_pixels': False, 'min_number_picture_neighbors': 2},
-}
-"""dict: optional, filter(s) to apply to the test set at image level"""
-test_event_filter = {
-    # utils.energyband_filter: {'energy': [0.02, 2], 'filter_only_gammas': True},  # in TeV
-    # utils.emission_cone_filter: {'max_angle': 0.0698},
-    # utils.impact_distance_filter: {'max_distance': 200},
-    # utils.telescope_multiplicity_filter: {'multiplicity': 2},
-}
-"""dict: optional, filter(s) to apply to the test set"""
+"""dict: optional, the parameters of the dataset specific to the test operation."""
 # test_file_max_number = 1
 """int: optional, the max number of files to use for the dataset"""
 test_batch_size = 10
 """int: optional, the size of the mini-batch for the test"""
 test_callbacks = [
     WriteDL2Files()
 ]
-"""dict: list of callbacks
-"""
+"""dict: list of callbacks"""
```

### Comparing `Gammalearn-0.8/gammalearn/data/nets.py` & `Gammalearn-0.9/gammalearn/data/nets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 import math
+from modulefinder import Module
 import torch
 from torch.nn.functional import upsample
-from torchvision.models import resnet18
+from torchvision.models import resnet18, ResNet, EfficientNet, MobileNetV2, MobileNetV3
+import torchvision
 import torch.nn as nn
 import torch.nn.functional as F
 import indexedconv.utils as cvutils
 from indexedconv.engine import IndexedConv, IndexedMaxPool2d, IndexedAveragePool2d
 from gammalearn.utils import get_camera_layout_from_geom
 
 
@@ -262,51 +264,40 @@
     def forward(self, x):
         out = []
         for t in self.children():
             out.append(t(x))
         return torch.cat(out, dim=1)
 
 
-class GammaPhysNet(nn.Module):
+class ResNetAttentionIndexed(nn.Module):
     """
-        Gamma-PhysNet with ResNet like Network with indexed convolutions as backbone.
-        Please cite and see details: https://www.scitepress.org/Link.aspx?doi=10.5220/0010297405340544 
-        Backbone based on https://arxiv.org/abs/1603.05027, CIFAR version
-        full pre-activation
+        ResNet like Network based on https://arxiv.org/abs/1603.05027, CIFAR version with full pre-activation,
+        augmented with attention (see backbone definition :
+        https://www.scitepress.org/Link.aspx?doi=10.5220/0010297405340544) and implemented with indexedconv.
     """
-
-    def __init__(self, net_parameters_dic, camera_geometry):
+    def __init__(self, net_parameters_dic):
         """
-
         Parameters
         ----------
         net_parameters_dic (dict): a dictionary describing the parameters of the network
         camera_geometry (CameraGeometry)
         """
-        super(GammaPhysNet, self).__init__()
-        self.logger = logging.getLogger(__name__ + '.GammaPhysNet')
+        super(ResNetAttentionIndexed, self).__init__()
+        self.logger = logging.getLogger(__name__ + '.ResNetAttentionIndexed')
 
-        index_matrix0, camera_layout = get_camera_layout_from_geom(camera_geometry)
+        index_matrix0, camera_layout = get_camera_layout_from_geom(net_parameters_dic['camera_geometry'])
 
         num_layers = net_parameters_dic['num_layers']
         num_channels = [net_parameters_dic['num_channels']]
         attention = net_parameters_dic['attention_layer']
         num_channels.extend(net_parameters_dic['block_features'])
-        fc_width = net_parameters_dic['fc_width']
         non_linearity = net_parameters_dic['non_linearity']
-        last_bias_init = net_parameters_dic['last_bias_init']
 
-        if 'class' in net_parameters_dic['targets'].keys():
-            num_class = net_parameters_dic['targets']['class']
-        else:
-            num_class = 0
-        regressor = {t: net_parameters_dic['targets'][t] for t in net_parameters_dic['targets'].keys() if
-                     t != 'class'}
-        if len(regressor) == 0:
-            regressor = None
+        self.num_features = num_channels[-1]
+
         if 'init' in net_parameters_dic.keys():
             init = net_parameters_dic['init']
         else:
             init = 'kaiming'
         if 'batch_norm' in net_parameters_dic.keys():
             batch_norm = net_parameters_dic['batch_norm']
         else:
@@ -348,30 +339,77 @@
                                                                batch_norm=batch_norm, non_linearity=non_linearity))
             if attention is not None:
                 self.feature.add_module('attention_block' + str(i), attention[0](n_out, **attention[1]))
 
         self.feature.add_module('last_' + non_linearity.__name__, non_linearity())
 
         # Compute the number of pixels (where idx is not -1 in the index matrix) of the last features
-        n_pixels = int(torch.sum(torch.ge(index_matrix1[0, 0], 0)).data)
-        self.logger.info('num pixels after last pooling : {}'.format(n_pixels))
+        self.n_pixels = int(torch.sum(torch.ge(index_matrix1[0, 0], 0)).data)
+        self.logger.debug('num pixels after last pooling : {}'.format(self.n_pixels))
+
+        # Init conv weights
+        for m in self.modules():
+            if isinstance(m, IndexedConv):
+                if init == 'orthogonal':
+                    nn.init.orthogonal_(m.weight)
+                elif init == 'kaiming':
+                    nn.init.kaiming_uniform_(m.weight, mode='fan_out')
+                else:
+                    self.logger.warning('Unknown initialization, use default one')
+
+    def forward(self, x):
+        return self.feature(x)
+
+
+class GammaPhysNet(nn.Module):
+    """
+        Gamma-PhysNet with ResNet
+        Please cite and see details: https://www.scitepress.org/Link.aspx?doi=10.5220/0010297405340544
+    """
+
+    def __init__(self, net_parameters_dic):
+        """
+
+        Parameters
+        ----------
+        net_parameters_dic (dict): a dictionary describing the parameters of the network
+        camera_geometry (CameraGeometry)
+        """
+        super(GammaPhysNet, self).__init__()
+        self.logger = logging.getLogger(__name__ + '.GammaPhysNet')
+
+        fc_width = net_parameters_dic['fc_width']
+        non_linearity = net_parameters_dic['non_linearity']
+        last_bias_init = net_parameters_dic['last_bias_init']
+
+        if 'class' in net_parameters_dic['targets'].keys():
+            num_class = net_parameters_dic['targets']['class']
+        else:
+            num_class = 0
+        regressor = {t: net_parameters_dic['targets'][t] for t in net_parameters_dic['targets'].keys() if
+                     t != 'class'}
+        if len(regressor) == 0:
+            regressor = None
+
+        # Backbone
+        self.feature = net_parameters_dic['backbone']['model'](net_parameters_dic['backbone']['parameters'])
 
         # Multitasking block
         if regressor is not None:
             if 'energy' in regressor:
                 self.energy = nn.Sequential()
-                self.energy.add_module('en_layer1', nn.Linear(num_channels[-1], fc_width))
+                self.energy.add_module('en_layer1', nn.Linear(self.feature.num_features, fc_width))
                 self.energy.add_module(non_linearity.__name__ + '1', non_linearity())
                 self.energy.add_module('en_out', nn.Linear(fc_width, regressor['energy']))
                 if last_bias_init is not None and 'energy' in last_bias_init:
                     self.energy.en_out.bias = nn.Parameter(torch.tensor(last_bias_init['energy']))
             else:
                 self.energy = None
             if 'impact' in regressor or 'direction' in regressor:
-                self.fusion = nn.Linear(n_pixels * num_channels[-1], fc_width)
+                self.fusion = nn.Linear(self.feature.n_pixels * self.feature.num_features, fc_width)
                 if 'impact' in regressor:
                     self.impact = nn.Linear(fc_width, regressor['impact'])
                     if last_bias_init is not None and 'impact' in last_bias_init:
                         self.impact.bias = nn.Parameter(torch.tensor(last_bias_init['impact']))
                 else:
                     self.impact = None
                 if 'direction' in regressor:
@@ -384,84 +422,111 @@
                 self.fusion = None
         else:
             self.energy = None
             self.fusion = None
             self.direction = None
             self.impact = None
         if num_class > 0:
-            self.classifier = nn.Linear(n_pixels * num_channels[-1], num_class)
+            self.classifier = nn.Linear(self.feature.n_pixels * self.feature.num_features, num_class)
             if last_bias_init is not None and 'class' in last_bias_init:
                 self.classifier.bias = nn.Parameter(torch.tensor(last_bias_init['class']))
         else:
             self.classifier = None
 
         self.non_linearity = non_linearity()
 
-        for m in self.modules():
-            if isinstance(m, IndexedConv):
-                if init == 'orthogonal':
-                    nn.init.orthogonal_(m.weight)
-                elif init == 'kaiming':
-                    nn.init.kaiming_uniform_(m.weight, mode='fan_out')
-                else:
-                    self.logger.warning('Unknown initialization, use default one')
-
     def forward(self, x):
         out = self.feature(x)
+        out = torch.flatten(out, start_dim=2)
         out_e = torch.mean(out, 2)  # Global average pooling
         out = out.view(out.size(0), -1)
         out_tot = {}
         if self.energy is not None:
             out_tot['energy'] = self.energy(out_e)
         if self.fusion is not None:
             out_f = self.non_linearity(self.fusion(out))
             if self.impact is not None:
                 out_tot['impact'] = self.impact(out_f)
             if self.direction is not None:
                 out_tot['direction'] = self.direction(out_f)
         if self.classifier is not None:
-            out_tot['class'] = nn.LogSoftmax(1)(self.classifier(out))
+            out_tot['class'] = self.classifier(out)
         return out_tot
 
 
-class GammaPhysNetCartesian(nn.Module):
+class TorchModel(nn.Module):
     """
-        Gamma-PhysNet with ResNet like Network with indexed convolutions as backbone.
-        Please cite and see details: https://www.scitepress.org/Link.aspx?doi=10.5220/0010297405340544
-        Backbone based on https://arxiv.org/abs/1603.05027, CIFAR version
-        full pre-activation
+    Extracts backbone from torchvision models
     """
+    def __init__(self, net_parameters_dic):
+        super(TorchModel, self).__init__()
+        self.logger = logging.getLogger(__name__ + '.ResNetAttentionIndexed')
 
-    def __init__(self, net_parameters_dic, *args, **kwargs):
+        pretrained = net_parameters_dic['parameters'].get('pretrained', False)
+
+        model = net_parameters_dic['model'](pretrained=pretrained)
+        num_channels = net_parameters_dic['parameters']['num_channels']
+        output_size = net_parameters_dic['parameters']['output_size']
+
+        if isinstance(model, ResNet):
+            self.feature = torch.nn.Sequential(*list(model.children())[:-2])
+            self.feature[0] = torch.nn.Conv2d(num_channels, self.feature[0].out_channels,
+                                              kernel_size=self.feature[0].kernel_size,
+                                              stride=self.feature[0].stride,
+                                              padding=self.feature[0].padding,
+                                              bias=False,
+                                              )
+            self.num_features = self.feature[-1][-1].conv1.out_channels
+
+        elif isinstance(model, (EfficientNet, MobileNetV2, MobileNetV3)):
+            self.feature = model.features
+            self.feature[0][0] = torch.nn.Conv2d(num_channels, self.feature[0][0].out_channels,
+                                                 kernel_size=self.feature[0][0].kernel_size,
+                                                 stride=self.feature[0][0].stride,
+                                                 padding=self.feature[0][0].padding,
+                                                 bias=False
+                                                 )
+            self.num_features = self.feature[-1][0].out_channels
+        else:
+            raise ValueError('Unknown torch model')
+
+        self.feature.add_module('avgpool', torch.nn.AdaptiveAvgPool2d(output_size))
+        self.n_pixels = torch.prod(torch.tensor(output_size))
+
+    def forward(self, x):
+        return self.feature(x)
+
+
+class ResNetAttention(nn.Module):
+    """
+        ResNet like Network based on https://arxiv.org/abs/1603.05027, CIFAR version with full pre-activation,
+        augmented with attention (see backbone definition :
+        https://www.scitepress.org/Link.aspx?doi=10.5220/0010297405340544)
+    """
+
+    def __init__(self, net_parameters_dic):
         """
 
         Parameters
         ----------
         net_parameters_dic (dict): a dictionary describing the parameters of the network
         camera_parameters (dict): a dictionary containing the parameters of the camera used with this network
         """
-        super(GammaPhysNetCartesian, self).__init__()
-        self.logger = logging.getLogger(__name__ + '.GammaPhysNetCartesian')
+        super(ResNetAttention, self).__init__()
+        self.logger = logging.getLogger(__name__ + '.ResNetAttention')
 
         num_layers = net_parameters_dic['num_layers']
         num_channels = [net_parameters_dic['num_channels']]
         attention = net_parameters_dic['attention_layer']
         num_channels.extend(net_parameters_dic['block_features'])
-        fc_width = net_parameters_dic['fc_width']
         non_linearity = net_parameters_dic['non_linearity']
-        last_bias_init = net_parameters_dic['last_bias_init']
+        output_size = net_parameters_dic['output_size']
+
+        self.num_features = num_channels[-1]
 
-        if 'class' in net_parameters_dic['targets'].keys():
-            num_class = net_parameters_dic['targets']['class']
-        else:
-            num_class = 0
-        regressor = {t: net_parameters_dic['targets'][t] for t in net_parameters_dic['targets'].keys() if
-                     t != 'class'}
-        if len(regressor) == 0:
-            regressor = None
         if 'init' in net_parameters_dic.keys():
             init = net_parameters_dic['init']
         else:
             init = 'kaiming'
         if 'batch_norm' in net_parameters_dic.keys():
             batch_norm = net_parameters_dic['batch_norm']
         else:
@@ -499,94 +564,40 @@
                                                 _ResidualLayerCartesian(n_out, n_out,
                                                                         batch_norm=batch_norm,
                                                                         non_linearity=non_linearity))
             if attention is not None:
                 self.feature.add_module('attention_block' + str(i), attention[0](n_out, **attention[1]))
 
         self.feature.add_module('last_' + non_linearity.__name__, non_linearity())
-        self.adaptive_pooling = nn.AdaptiveAvgPool2d((14, 14))
+        self.adaptive_pooling = nn.AdaptiveAvgPool2d(output_size)
         self.feature.add_module('adaptive_pooling2D', self.adaptive_pooling)
 
         # Compute the number of pixels (where idx is not -1 in the index matrix) of the last features
-        n_pixels = 14*14
-        self.logger.info('num pixels after last pooling : {}'.format(n_pixels))
-
-        # Multitasking block
-        if regressor is not None:
-            if 'energy' in regressor:
-                self.energy = nn.Sequential()
-                self.energy.add_module('en_layer1', nn.Linear(num_channels[-1], fc_width))
-                self.energy.add_module(non_linearity.__name__ + '1', non_linearity())
-                self.energy.add_module('en_out', nn.Linear(fc_width, regressor['energy']))
-                if last_bias_init is not None and 'energy' in last_bias_init:
-                    self.energy.en_out.bias = nn.Parameter(torch.tensor(last_bias_init['energy']))
-            else:
-                self.energy = None
-            if 'impact' in regressor or 'direction' in regressor:
-                self.fusion = nn.Linear(n_pixels * num_channels[-1], fc_width)
-                if 'impact' in regressor:
-                    self.impact = nn.Linear(fc_width, regressor['impact'])
-                    if last_bias_init is not None and 'impact' in last_bias_init:
-                        self.impact.bias = nn.Parameter(torch.tensor(last_bias_init['impact']))
-                else:
-                    self.impact = None
-                if 'direction' in regressor:
-                    self.direction = nn.Linear(fc_width, regressor['direction'])
-                    if last_bias_init is not None and 'direction' in last_bias_init:
-                        self.direction.bias = nn.Parameter(torch.tensor(last_bias_init['direction']))
-                else:
-                    self.direction = None
-            else:
-                self.fusion = None
-        else:
-            self.energy = None
-            self.fusion = None
-            self.direction = None
-            self.impact = None
-        if num_class > 0:
-            self.classifier = nn.Linear(n_pixels * 64, num_class)
-            if last_bias_init is not None and 'class' in last_bias_init:
-                self.classifier.bias = nn.Parameter(torch.tensor(last_bias_init['class']))
-        else:
-            self.classifier = None
+        self.n_pixels = torch.prod(torch.tensor(output_size))
+        self.logger.info('num pixels after last pooling : {}'.format(self.n_pixels))
 
         self.non_linearity = non_linearity()
 
         for m in self.modules():
-            if isinstance(m, IndexedConv):
+            if isinstance(m, nn.Conv2d):
                 if init == 'orthogonal':
                     nn.init.orthogonal_(m.weight)
                 elif init == 'kaiming':
                     nn.init.kaiming_uniform_(m.weight, mode='fan_out')
                 else:
                     self.logger.warning('Unknown initialization, use default one')
 
     def forward(self, x):
-        out = self.feature(x)
-        out_e = torch.mean(out, dim=tuple(range(out.dim())[2:]))  # Global average pooling
-        out = out.view(out.size(0), -1)
-        out_tot = {}
-        if self.energy is not None:
-            out_tot['energy'] = self.energy(out_e)
-        if self.fusion is not None:
-            out_f = self.non_linearity(self.fusion(out))
-            if self.impact is not None:
-                out_tot['impact'] = self.impact(out_f)
-            if self.direction is not None:
-                out_tot['direction'] = self.direction(out_f)
-        if self.classifier is not None:
-            out_tot['class'] = nn.LogSoftmax(1)(self.classifier(out))
-        return out_tot
+        return self.feature(x)
 
 
 class ConvAutoEncoder(nn.Module):
-    def __init__(self, net_parameters_dic, camera_geometry, mode='train'):
+    def __init__(self, net_parameters_dic):
         super(ConvAutoEncoder, self).__init__()
-        self.logger = logging.getLogger(__name__ + '.GLNetIndexConv42')
-        self.targets = net_parameters_dic['targets']
+        self.logger = logging.getLogger(__name__ + '.ConvAutoEncoder')
 
         # encoder layers
         # conv layer (depth from 2 --> 16), 3x3 kernels
         self.conv1 = nn.Conv2d(2, 16, 3, padding=1)
         self.relu1 = nn.ReLU()
         self.pool1 = nn.MaxPool2d(2, 2)
         # conv layer (depth from 16 --> 8), 3x3 kernels
@@ -625,27 +636,27 @@
 
 class GLNetIndexConv42(nn.Module):
     """
         Network with indexed convolutions and pooling.
         4 CL (after each conv layer, pooling is executed)
         2 FC
     """
-    def __init__(self, net_parameters_dic, camera_geometry, mode='train'):
+    def __init__(self, net_parameters_dic):
         """
         Parameters
         ----------
         net_parameters_dic (dict): a dictionary describing the parameters of the network
         camera_parameters (dict): a dictionary containing the parameters of the camera used with this network
         mode (str): explicit mode to use the network (different from the nn.Module.train() or evaluate()). For GANs
         """
         super(GLNetIndexConv42, self).__init__()
         self.logger = logging.getLogger(__name__ + '.GLNetIndexConv42')
         self.targets = net_parameters_dic['targets']
 
-        index_matrix1, camera_layout = get_camera_layout_from_geom(camera_geometry)
+        index_matrix1, camera_layout = get_camera_layout_from_geom(net_parameters_dic['camera_geometry'])
         pooling_kernel = camera_layout
 
         # Channels
         num_outputs = sum(net_parameters_dic['targets'].values())
         self.num_channel = n1 = net_parameters_dic['num_channels']
         n_features = net_parameters_dic['n_features']
         n2 = n_features*2
@@ -740,27 +751,27 @@
         out = drop(self.relu5(out))
 
         out_linear2 = self.lin2(out)
         i = 0
         output = {}
         for t, v in self.targets.items():
             if t == 'class':
-                output[t] = nn.LogSoftmax(1)(out_linear2[:, i:i + v])
+                output[t] = out_linear2[:, i:i + v]
             else:
                 output[t] = out_linear2[:, i:i+v]
             i += v
 
         return output
 
 
 class ResNet18MT(nn.Module):
     """
         ResNet18 for multitask IACT reco
     """
-    def __init__(self, net_parameters_dic, camera_geometry):
+    def __init__(self, net_parameters_dic):
         """
         Parameters
         ----------
         net_parameters_dic (dict): a dictionary describing the parameters of the network
         camera_parameters (dict): a dictionary containing the parameters of the camera used with this network
         mode (str): explicit mode to use the network (different from the nn.Module.train() or evaluate()). For GANs
         """
@@ -791,13 +802,103 @@
         out = drop(self.relu5(out))
 
         out_linear2 = self.lin2(out)
         i = 0
         output = {}
         for t, v in self.targets.items():
             if t == 'class':
-                output[t] = nn.LogSoftmax(1)(out_linear2[:, i:i + v])
+                output[t] = out_linear2[:, i:i + v]
             else:
                 output[t] = out_linear2[:, i:i+v]
             i += v
 
         return output
+
+
+class GammaDumbNet(nn.Module):
+    def __init__(self, net_parameters_dic, *args, **kwargs):
+        super().__init__()
+
+        num_channels = net_parameters_dic['block_features'][-1]
+
+        # Encoder backbone
+        self.feature = nn.Sequential()
+        self.feature.add_module('f_conv1', nn.Conv2d(2, num_channels, 3, padding=1))
+        self.feature.add_module('f_relu1', nn.ReLU())
+        self.feature.add_module('f_pool1', nn.AdaptiveAvgPool2d((14, 14)))
+
+        output_size = 14 * 14 * num_channels
+
+        # Energy
+        self.energy = nn.Sequential()
+        self.energy.add_module('energy_fc1', nn.Linear(output_size, 1))
+
+        # Impact
+        self.impact = nn.Sequential()
+        self.impact.add_module('impact_fc1', nn.Linear(output_size, 2))
+
+        # Direction
+        self.direction = nn.Sequential()
+        self.direction.add_module('direction_fc1', nn.Linear(output_size, 2))
+
+        # Classifier
+        self.classifier = nn.Sequential()
+        self.classifier.add_module('classifier_fc1', nn.Linear(output_size, 2))
+
+    def forward(self, x):
+        out = self.feature(x).view(out.size(0), -1)
+        out_tot = {}
+        out_tot['energy'] = self.energy(out)
+        out_tot['impact'] = self.impact(out)
+        out_tot['direction'] = self.direction(out)
+        out_tot['class'] = self.classifier(out)
+
+        return out_tot
+
+
+class DANN(nn.Module):
+    """
+    Domain Adversarial Neural Network based on https://arxiv.org/abs/1505.07818
+    """
+    def __init__(self, net_parameters_dic):
+        super().__init__()
+
+        self.logger = logging.getLogger(__name__ + '.DANN')
+        fc1_features = net_parameters_dic['fc1_features']
+
+        self.main_task_model = net_parameters_dic['main_task']['model'](net_parameters_dic['main_task']['parameters'])
+
+        self.domain_classifier = nn.Sequential()
+        self.domain_classifier.add_module('d_fc1', nn.Linear(self.main_task_model.feature.n_pixels *
+                                                             self.main_task_model.feature.num_features,
+                                                             fc1_features))
+        self.domain_classifier.add_module('d_bn1', nn.BatchNorm1d(fc1_features))
+
+        self.domain_classifier.add_module('d_relu1', nn.ReLU())
+        self.domain_classifier.add_module('d_fc2', nn.Linear(fc1_features, 2))
+
+        self.feature_output = None
+
+        def get_feature_output(module, input, output):
+            self.feature_output = output
+
+        self.main_task_model.feature.register_forward_hook(get_feature_output)
+
+    def forward(self, x):
+        out_tot = self.main_task_model(x)
+        out = self.feature_output.view(self.feature_output.size(0), -1)
+
+        reverse_layer = GradientReverseLayer.apply
+        out_tot['domain_class'] = self.domain_classifier(reverse_layer(out))
+
+        return out_tot
+
+
+class GradientReverseLayer(torch.autograd.Function):
+
+    @staticmethod
+    def forward(ctx, x):
+        return x
+
+    @staticmethod
+    def backward(ctx, grad_output):
+        return grad_output.neg()
```

### Comparing `Gammalearn-0.8/gammalearn/data/nice_lst.npy` & `Gammalearn-0.9/gammalearn/data/nice_lst.npy`

 * *Files identical despite different names*

### Comparing `Gammalearn-0.8/gammalearn/data_handlers.py` & `Gammalearn-0.9/gammalearn/data_handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,124 +1,161 @@
 import logging
 import torch.multiprocessing as mp
 from functools import partial
+import tqdm
 
 from pytorch_lightning import LightningDataModule
 import torch
 from torch.utils.data import DataLoader, Dataset, ConcatDataset, Subset
 from torchvision import transforms
+from gammalearn.datasets import DADataset
 
 from gammalearn import utils as utils
 from gammalearn.logging import LOGGING_CONFIG
 
 
 def create_dataset_worker(file,
-                          data_transform,
                           dataset_class,
-                          targets,
-                          dataset_parameters,
-                          image_filter,
-                          event_filter,
-                          train):
+                          train,
+                          **kwargs):
     torch.set_num_threads(1)
     # Reload logging config (lost by spawn)
     logging.config.dictConfig(LOGGING_CONFIG)
 
-    if data_transform is not None:
-        transform = transforms.Compose(data_transform['data'])
-        target_transform = transforms.Compose(data_transform['target'])
-    else:
-        transform = None
-        target_transform = None
-
     if utils.is_datafile_healthy(file):
         dataset = dataset_class(file,
-                                targets=targets,
-                                transform=transform,
-                                target_transform=target_transform,
-                                **dataset_parameters,
-                                train=train
+                                train=train,
+                                **kwargs
                                 )
-        if image_filter is not None:
-            dataset.filter_image(image_filter)
-        if event_filter is not None:
-            dataset.filter_event(event_filter)
+        if kwargs.get('image_filter') is not None:
+            dataset.filter_image(kwargs.get('image_filter'))
+        if kwargs.get('event_filter') is not None:
+            dataset.filter_event(kwargs.get('event_filter'))
         if len(dataset) > 0:
             return dataset
 
 
-def create_datasets(datafiles_list, experiment, train=True):
+def create_datasets(datafiles_list, experiment, train=True, **kwargs):
     """
     Create datasets from datafiles list, data are loaded in memory.
     Parameters
     ----------
     datafiles (List) : files to load data from
     experiment (Experiment): the experiment
 
     Returns
     -------
     Datasets
     """
+
     logger = logging.getLogger('gammalearn')
     assert datafiles_list, 'The data file list is empty !'
 
     logger.info('length of data file list : {}'.format(len(datafiles_list)))
     # We get spawn context because fork can cause deadlock in sub-processes
     # in multi-threaded programs (especially with logging)
     ctx = mp.get_context('spawn')
     if experiment.preprocessing_workers > 0:
         num_workers = experiment.preprocessing_workers
     else:
         num_workers = 1
     pool = ctx.Pool(processes=num_workers)
-    datasets = pool.map(partial(create_dataset_worker,
-                                data_transform=experiment.data_transform,
-                                dataset_class=experiment.dataset_class,
-                                targets=list(experiment.targets.keys()),
-                                dataset_parameters=experiment.dataset_parameters,
-                                image_filter=experiment.image_filter,
-                                event_filter=experiment.event_filter,
-                                train=train),
-                        datafiles_list)
+    datasets = list(tqdm.tqdm(pool.imap(partial(create_dataset_worker,
+                                                dataset_class=experiment.dataset_class,
+                                                train=train,
+                                                **kwargs),
+                                        datafiles_list),
+                              total=len(datafiles_list),
+                              desc='Load data files'
+                              )
+                    )
 
     return datasets
 
 
-def split_dataset(datasets, ratio, split_by_file=False):
+def split_dataset(datasets, ratio):
     """Split a list of datasets into a train and a validation set
     Parameters
     ----------
     datasets (list of Dataset): the list of datasets
     ratio (float): the ratio of data for validation
-    split_by_file (bool): whether to divide at the file or at the sample level
 
     Returns
     -------
     train set, validation set
 
     """
     # Creation of subset train and test
     assert 1 > ratio > 0, 'Validating ratio must be greater than 0 and smaller than 1.'
-    if split_by_file:
-        train_max_index = int(len(datasets) * (1 - ratio))
-        shuffled_indices = torch.randperm(len(datasets)).numpy()
-        train_datasets = [datasets[i] for i in shuffled_indices[:train_max_index]]
-        val_datasets = [datasets[i] for i in shuffled_indices[train_max_index:]]
-    else:
-        datasets = ConcatDataset(datasets)
-        train_max_index = int(len(datasets) * (1 - ratio))
-        shuffled_indices = torch.randperm(len(datasets)).numpy()
-        assert isinstance(datasets, Dataset)
-        train_datasets = [Subset(datasets, shuffled_indices[:train_max_index])]
-        val_datasets = [Subset(datasets, shuffled_indices[train_max_index:])]
+
+    train_max_index = int(len(datasets) * (1 - ratio))
+    shuffled_indices = torch.randperm(len(datasets)).numpy()
+    assert isinstance(datasets, Dataset)
+    train_datasets = Subset(datasets, shuffled_indices[:train_max_index])
+    val_datasets = Subset(datasets, shuffled_indices[train_max_index:])
 
     return train_datasets, val_datasets
 
 
-class GLearnDataModule(LightningDataModule):
+def get_dataset_from_path(experiment, logger, data_type='source', train=True):
+    if train:
+        data_module = experiment.data_module_train[data_type]
+    else:
+        data_module = experiment.data_module_test[data_type]
+
+    file_list = utils.find_datafiles(data_module['paths'], experiment.files_max_number)
+
+    if train:
+        logger.debug(file_list)
+
+    file_list = list(file_list)
+    file_list.sort()
+
+    datasets = create_datasets(file_list, experiment, train=train, **data_module, **experiment.dataset_parameters)
+
+    if train:
+        return ConcatDataset(datasets)
+    else:
+        if experiment.merge_test_datasets:
+            particle_dict = {}
+
+            for dset in datasets:
+                if dset.simu:
+                    particle_type = dset.dl1_params['mc_type'][0]
+
+                    if particle_type in particle_dict:
+                        particle_dict[particle_type].append(dset)
+                    else:
+                        particle_dict[particle_type] = [dset]
+                else:
+                    if 'real_list' in particle_dict:
+                        particle_dict['real_list'].append(dset)
+                    else:
+                        particle_dict['real_list'] = [dset]
+
+            return [ConcatDataset(dset) for dset in particle_dict.values()]
+        else:
+            return datasets
+
+
+def get_DA_dataset(experiment, logger, train=True):
+    source_datasets = get_dataset_from_path(experiment, logger, data_type='source', train=train)
+    target_datasets = get_dataset_from_path(experiment, logger, data_type='target', train=train)
+
+    max_index = min(len(source_datasets), len(target_datasets))
+    shuffled_indices_source = torch.randperm(len(source_datasets)).numpy()
+    shuffled_indices_target = torch.randperm(len(target_datasets)).numpy()
+
+    source_datasets = Subset(source_datasets, shuffled_indices_source[:max_index])
+    target_datasets = Subset(target_datasets, shuffled_indices_target[:max_index])
+
+    return DADataset(source_datasets, target_datasets)
+
+
+class BaseDataModule(LightningDataModule):
     """
     Create datasets and dataloaders.
     Parameters
     ----------
     experiment (Experiment): the experiment
 
     Returns
@@ -129,86 +166,93 @@
         self.experiment = experiment
         self.logger = logging.getLogger(__name__)
         self.train_set = None
         self.val_set = None
         self.test_sets = None
 
     def setup(self, stage=None):
+        raise NotImplementedError
+
+    def train_dataloader(self):
+        training_loader = DataLoader(self.train_set,
+                                     batch_size=self.experiment.batch_size,
+                                     shuffle=True,
+                                     drop_last=True,
+                                     num_workers=self.experiment.dataloader_workers,
+                                     pin_memory=self.experiment.pin_memory)
+        self.logger.info('training loader length : {} batches'.format(len(training_loader)))
+        return training_loader
+
+    def val_dataloader(self):
+        validating_loader = DataLoader(self.val_set,
+                                       batch_size=self.experiment.batch_size,
+                                       shuffle=False,
+                                       num_workers=self.experiment.dataloader_workers,
+                                       drop_last=False,
+                                       pin_memory=self.experiment.pin_memory)
+        self.logger.info('validating loader length : {} batches'.format(len(validating_loader)))
+        return validating_loader
+
+    def test_dataloaders(self):
+        test_loaders = [DataLoader(test_set, batch_size=self.experiment.test_batch_size, shuffle=False,
+                                   drop_last=False, num_workers=self.experiment.dataloader_workers)
+                        for test_set in self.test_sets]
+        self.logger.info('test loader length : {} batches'.format(torch.tensor([len(t) for t in test_loaders]).sum()))
+        return test_loaders
+
+
+class GLearnDataModule(BaseDataModule):
+    """
+    Create datasets and dataloaders.
+    Parameters
+    ----------
+    experiment (Experiment): the experiment
+
+    Returns
+    -------
+    """
+    def __init__(self, experiment):
+        super().__init__(experiment)
+
+    def setup(self, stage=None):
 
         self.logger.info('Start creating datasets')
 
         if self.experiment.train:
             self.logger.info('look for data files')
-            train_file_list = utils.find_datafiles(self.experiment.train_folders, self.experiment.files_max_number)
-            self.logger.debug(train_file_list)
-            train_file_list = list(train_file_list)
-            train_file_list.sort()
-            datasets = create_datasets(train_file_list, self.experiment)
+
+            if not self.experiment.data_module_train['target']['paths']: # source only
+                datasets = get_dataset_from_path(self.experiment, self.logger)
+            else: # source + target
+                datasets = get_DA_dataset(self.experiment, self.logger)
 
             assert datasets, 'Dataset is empty !'
 
             # Creation of subset train and test
-            train_datasets, val_datasets = split_dataset(datasets, self.experiment.validating_ratio,
-                                                         self.experiment.split_by_file)
+            train_datasets, val_datasets = split_dataset(datasets, self.experiment.validating_ratio)
 
-            if self.experiment.data_augment is not None:
-                self.logger.info('Start data augmentation')
-                train_datasets = self.experiment.data_augment['function'](train_datasets,
-                                                                          **self.experiment.data_augment['kwargs'])
-            self.train_set = ConcatDataset(train_datasets)
+            self.train_set = train_datasets
             self.logger.info('training set length : {}'.format(len(self.train_set)))
 
-            self.val_set = ConcatDataset(val_datasets)
+            self.val_set = val_datasets
             try:
                 assert len(self.val_set) > 0
             except AssertionError as e:
                 self.logger.exception('Validating set must contain data')
                 raise e
             self.logger.info('validating set length : {}'.format(len(self.val_set)))
         else:
             self.train_set = None
             self.val_set = None
         if self.experiment.test:
-            if self.experiment.test_folders is not None:
+            if self.experiment.data_module_test is not None:
                 # Look for specific data parameters
                 if self.experiment.test_dataset_parameters is not None:
                     self.experiment.dataset_parameters.update(self.experiment.test_dataset_parameters)
-                # Update data filters
-                self.experiment.image_filter = self.experiment.test_image_filter
-                self.experiment.event_filter = self.experiment.test_event_filter
                 # Create data sets
-                test_file_list = utils.find_datafiles(self.experiment.test_folders,
-                                                      self.experiment.test_file_max_number)
-                test_file_list = list(test_file_list)
-                test_file_list.sort()
-                self.test_sets = create_datasets(test_file_list, self.experiment, train=False)
+                self.test_sets = get_dataset_from_path(self.experiment, self.logger, train=False)
+                if self.experiment.data_module_test['target']['paths']: # if target are provided
+                    self.test_sets.extend(get_dataset_from_path(self.experiment, self.logger, data_type='target', train=False))
             else:
                 assert self.val_set is not None, 'Test is required but no test file is provided and val_set is None'
                 self.test_sets = [self.val_set]
             self.logger.info('test set length : {}'.format(torch.tensor([len(t) for t in self.test_sets]).sum()))
-
-    def train_dataloader(self):
-        training_loader = DataLoader(self.train_set,
-                                     batch_size=self.experiment.batch_size,
-                                     shuffle=True,
-                                     drop_last=True,
-                                     num_workers=self.experiment.dataloader_workers,
-                                     pin_memory=self.experiment.pin_memory)
-        self.logger.info('training loader length : {} batches'.format(len(training_loader)))
-        return training_loader
-
-    def val_dataloader(self):
-        validating_loader = DataLoader(self.val_set,
-                                       batch_size=self.experiment.batch_size,
-                                       shuffle=False,
-                                       num_workers=self.experiment.dataloader_workers,
-                                       drop_last=False,
-                                       pin_memory=self.experiment.pin_memory)
-        self.logger.info('validating loader length : {} batches'.format(len(validating_loader)))
-        return validating_loader
-
-    def test_dataloaders(self):
-        test_loaders = [DataLoader(test_set, batch_size=self.experiment.test_batch_size, shuffle=False,
-                                   drop_last=False, num_workers=self.experiment.dataloader_workers)
-                        for test_set in self.test_sets]
-        self.logger.info('test loader length : {} batches'.format(torch.tensor([len(t) for t in test_loaders]).sum()))
-        return test_loaders
```

### Comparing `Gammalearn-0.8/gammalearn/datasets.py` & `Gammalearn-0.9/gammalearn/datasets.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,27 +7,59 @@
 from astropy.table import Table
 import astropy.units as u
 from ctapipe.instrument import CameraGeometry
 from ctapipe.image import tailcuts_clean
 from lstchain.io.io import read_simu_info_merged_hdf5
 from lstchain.io.io import dl1_images_lstcam_key, dl1_params_lstcam_key
 from dl1_data_handler.image_mapper import ImageMapper
+import pandas as pd
 
 
 
 DL1_SUBARRAY_TRIGGER_KEY = 'dl1/event/subarray/trigger'
 DL1_SUBARRAY_LAYOUT = 'configuration/instrument/subarray/layout'
 
+
+def fetch_dataset_geometry(dataset):
+    if isinstance(dataset, torch.utils.data.Subset):
+        fetch_dataset_geometry(dataset.dataset)
+    elif isinstance(dataset, torch.utils.data.ConcatDataset):
+        fetch_dataset_geometry(dataset.datasets[0])
+    else:
+        return dataset.camera_geometry
+
+
+class DADataset(Dataset):
+    def __init__(self, source_dataset, target_dataset):
+        super().__init__()
+        assert len(source_dataset) == len(target_dataset)
+        self.source_dataset = source_dataset
+        self.target_dataset = target_dataset
+        self.camera_geometry = self.source_dataset.dataset.datasets[0].camera_geometry
+        #self.camera_geometry = fetch_dataset_geometry(self.source_dataset)
+
+    def __len__(self):
+        return len(self.source_dataset)
+
+    def __getitem__(self, idx):
+        sample_source = {k + '_source': v for k, v in self.source_dataset[idx].items()}
+        sample_target = {k + '_target': v for k, v in self.target_dataset[idx].items()}
+        sample = {**sample_source, **sample_target}
+
+        return sample
+
+
 class WrongGeometryError(Exception):
     pass
 
-class MockLSTDataset(Dataset):
 
+class MockLSTDataset(Dataset):
+    
     def __init__(self, hdf5_file_path, camera_type, group_by, targets=None, particle_dict=None, use_time=False, train=True,
-                 subarray=None, transform=None, target_transform=None):
+                 subarray=None, transform=None, target_transform=None, **kwargs):
 
         self.images = np.random.rand(50, 1855).astype(np.float32)
         self.times = np.random.rand(50, 1855).astype(np.float32)
 
         self.particle_dict = {0: 0, 101: 1}
 
         self.camera_type = 'LST_LSTCam'
@@ -77,16 +109,15 @@
         pass
 
 
 class BaseLSTDataset(Dataset):
     """camera simulation dataset for lstchain DL1 hdf5 files. """
 
     def __init__(self, hdf5_file_path, camera_type, group_by, targets=None, particle_dict=None, use_time=False,
-                 train=True,
-                 subarray=None, transform=None, target_transform=None):
+                 train=True, subarray=None, transform=None, target_transform=None, **kwargs):
         """
         Parameters
         ----------
             hdf5_file_path (str): path to hdf5 file containing the data
             camera_type (str) : name of the camera used (e.g. camera_type='LST_LSTCam)
             group_by (str): the way to group images in the dataset (e.g. 'event_triggered_tels' :
             by event only for telescopes which triggered)
@@ -163,16 +194,23 @@
             # LST subarray
             layout = hdf5_file.root[DL1_SUBARRAY_LAYOUT][:]
             lst_layout_mask = layout['name'] == b'LST'
             self.layout_tel_ids = layout['tel_id'][lst_layout_mask]
 
             # Keep a copy of triggered energies for gammaboard
             if self.simu:
-                _, indices = np.unique(self.dl1_params[:]['event_id'], return_index=True)
-                self.trig_energies = self.dl1_params['mc_energy'][indices]
+                dl1_params_df = pd.DataFrame(
+                    {
+                        'obs_id': self.dl1_params['obs_id'],
+                        'event_id': self.dl1_params['event_id']
+                    }
+                )
+                dl1_params_df = dl1_params_df.set_index(['obs_id', 'event_id'])
+                unique_event_mask = ~dl1_params_df.index.duplicated(keep='first')
+                self.trig_energies = self.dl1_params['mc_energy'][unique_event_mask]
                 self.trig_tels = hdf5_file.root[DL1_SUBARRAY_TRIGGER_KEY][:]['tels_with_trigger']
             else:
                 self.trig_energies = None
                 self.trig_tels = np.full((len(self.dl1_params), 6), False)
                 self.trig_tels[:, np.searchsorted(layout['tel_id'], self.dl1_params[
                     'tel_id'])] = True  # TODO fix when real data has several tels
             # Select sub-subarray
@@ -185,28 +223,34 @@
             event_mask = np.in1d(self.dl1_params['tel_id'], self.layout_tel_ids)
             self.dl1_params = self.dl1_params[event_mask]
             self.filtered_indices = self.filtered_indices[event_mask]
 
             # Load event info
             self.unique_event_ids = np.unique(self.dl1_params[:]['event_id'])
 
+            if not self.simu and 'mc_type' not in self.dl1_params.dtype.names:
+                self.dl1_params['mc_type'] = np.full(len(self.dl1_params), -9999)
+
             if self.simu:
                 # Turn distances into km
                 self.dl1_params['mc_x_max'] /= 1000
                 self.dl1_params['mc_core_x'] /= 1000
                 self.dl1_params['mc_core_y'] /= 1000
             self.dl1_params['tel_pos_x'] /= 1000
             self.dl1_params['tel_pos_y'] /= 1000
             self.dl1_params['tel_pos_z'] /= 1000
 
         # setup the ImageMapper transform
         if self.transform is not None:
-            for t in self.transform.transforms:
-                if hasattr(t, 'setup_geometry'):
-                    t.setup_geometry(self.camera_geometry)
+            if hasattr(self.transform, 'setup_geometry'):
+                self.transform.setup_geometry(self.camera_geometry)
+            else:
+                for t in self.transform.transforms:
+                    if hasattr(t, 'setup_geometry'):
+                        t.setup_geometry(self.camera_geometry)
 
     def __len__(self):
         if self.group_by == 'image':
             return len(self.filtered_indices)
         else:
             return len(self.unique_event_ids)
 
@@ -265,14 +309,16 @@
                 elif t == 'xmax':
                     labels[t] = np.array([dl1_params['mc_x_max']])
                 elif t == 'class':  # TODO replace by try except
                     labels[t] = self.particle_dict.get(dl1_params['mc_type'], -1)
                     if labels[t] == -1:
                         print(dl1_params['mc_type'])
                         print(self.hdf5_file_path)
+                elif t == 'domain_class':
+                    pass
                 else:
                     raise ValueError('Unknown target')
         else:
             labels = None
 
         # We reogranize the pixels to match the 'LSTCam' geometry
         sample = {'image': data[..., self.inj_table]}
@@ -319,19 +365,18 @@
 
         raise NotImplementedError
 
 
 class MemoryLSTDataset(BaseLSTDataset):
 
     def __init__(self, hdf5_file_path, camera_type, group_by, targets=None, particle_dict=None, use_time=False,
-                 train=True,
-                 subarray=None, transform=None, target_transform=None):
+                 train=True, subarray=None, transform=None, target_transform=None, **kwargs):
 
         super(MemoryLSTDataset, self).__init__(hdf5_file_path, camera_type, group_by, targets, particle_dict,
-                                               use_time, train, subarray, transform, target_transform)
+                                               use_time, train, subarray, transform, target_transform, **kwargs)
 
         with tables.File(hdf5_file_path, 'r') as hdf5_file:
             # Load images and peak times
             self.images = hdf5_file.root[dl1_images_lstcam_key].col('image').astype(np.float32)[self.filtered_indices]
             self.images = np.nan_to_num(self.images)
             if self.use_time:
                 self.times = hdf5_file.root[dl1_images_lstcam_key].col('peak_time').astype(np.float32)[
@@ -371,19 +416,18 @@
             self.times = self.times[image_mask]
         self.filtered_indices = np.arange(len(self.images))
 
 
 class FileLSTDataset(BaseLSTDataset):
 
     def __init__(self, hdf5_file_path, camera_type, group_by, targets=None, particle_dict=None, use_time=False,
-                 train=True,
-                 subarray=None, transform=None, target_transform=None):
+                 train=True, subarray=None, transform=None, target_transform=None, **kwargs):
 
         super(FileLSTDataset, self).__init__(hdf5_file_path, camera_type, group_by, targets, particle_dict,
-                                             use_time, train, subarray, transform, target_transform)
+                                             use_time, train, subarray, transform, target_transform, **kwargs)
 
     def __getitem__(self, idx):
         if self.hdf5_file is None:
             self.hdf5_file = tables.File(self.hdf5_file_path, 'r')
         return self._get_sample(idx)
 
     def _get_image_data(self, idx):
@@ -586,27 +630,36 @@
         self.max = max_pix
 
     def __call__(self, data):
         return data / self.max
 
 
 class CleanImages(TransformIACT):
-
-    def __init__(self, **opts):
+    """
+    Cleaning transform.
+    Parameters
+    ----------
+    new_channel (Bool): if True, adds the cleaning mask to the data as a new channel.
+    If False, apply the cleaning mask to the data.
+    """
+    def __init__(self, new_channel=False, **opts):
         self.opts = opts
+        self.new_channel = new_channel
         self.camera_geometry = None
 
     def setup_geometry(self, camera_geometry):
         self.camera_geometry = camera_geometry
 
     def __call__(self, data):
         image = data if data.ndim == 1 else data[0]
         clean_mask = tailcuts_clean(self.camera_geometry, image, **self.opts)
-
-        return data * clean_mask
+        if self.new_channel:
+            return np.concatenate([data, np.expand_dims(clean_mask, axis=0).astype(np.float32)])
+        else:
+            return data * clean_mask
 
 
 # Augment data functions
 
 def augment_via_duplication(datasets, scale, num_workers):
     """
     Augment data by duplicating events based on the inverse detected energies distribution
```

### Comparing `Gammalearn-0.8/gammalearn/experiment_runner.py` & `Gammalearn-0.9/gammalearn/experiment_runner.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,25 +10,28 @@
 import faulthandler
 
 import torch
 import torch.backends.cudnn as cudnn
 
 from pytorch_lightning import LightningModule
 from pytorch_lightning.loggers import TensorBoardLogger
-from pytorch_lightning.callbacks import ModelCheckpoint, DeviceStatsMonitor, LearningRateMonitor
+from pytorch_lightning.callbacks import ModelCheckpoint, DeviceStatsMonitor, LearningRateMonitor, GPUStatsMonitor
 import pytorch_lightning as pl
 
 from gammalearn.version import __version__ as _version
 from gammalearn.utils import (check_particle_mapping, compute_total_parameter_number, get_dataset_geom,
-                              prepare_experiment_folder, dump_experiment_config)
+                              prepare_experiment_folder, dump_experiment_config, inject_geometry_into_parameters)
 from gammalearn.data_handlers import GLearnDataModule
 from gammalearn.datasets import WrongGeometryError
 
 from gammalearn.logging import LOGGING_CONFIG
 
+from gammalearn.optimizers import DANNLR
+
+
 faulthandler.enable()
 
 
 class Experiment(object):
     """Loads the settings of the experiment from the settings object,
     check them and defines default values for not specified ones.
     """
@@ -71,33 +74,22 @@
 
         self._has_mandatory('dataset_parameters', 'the parameters of the dataset (camera type, group by option...)')
         self.dataset_parameters = settings.dataset_parameters
         check_particle_mapping(self.dataset_parameters['particle_dict'])
 
         self._has_mandatory('targets', 'the targets to reconstruct')
         self.targets = settings.targets
-        if 'class' in self.targets:
-            try:
-                assert 'output_shape' not in self.targets['class']
-            except AssertionError:
-                self._logger.warning('Output shape of target class defined in settings will be overwritten with '
-                                     'particle_dict length')
-            self.targets['class']['output_shape'] = len(self.dataset_parameters['particle_dict'])
 
         # Net settings
         self._has_mandatory('net_definition_file', 'the file containing the net class')
         self.net_definition_file = settings.net_definition_file
 
-        self._has_mandatory('model_net', 'the net to use')
-        self.model_net = settings.model_net
-
         self._has_mandatory('net_parameters_dic', 'the parameters of the net described by a dictionary')
         assert isinstance(getattr(settings, 'net_parameters_dic'), dict), 'The net parameters must be a dict !'
         self.net_parameters_dic = settings.net_parameters_dic
-        self.net_parameters_dic['targets'] = {k: v['output_shape'] for k, v in self.targets.items()}
 
         self._has_mandatory('train', 'whether to test the model after training')
         self._is_of_type('train', bool)
         self.train = settings.train
 
         self._has_mandatory('test', 'whether to test the model after training')
         self._is_of_type('test', bool)
@@ -170,16 +162,17 @@
 
         self.profiler = settings.profiler if hasattr(settings, 'profiler') else None
 
         #################################################################################################
         # Train settings
         if self.train:
             # Data settings
-            self._has_mandatory('train_folders', 'the training and validating data folders')
-            self.train_folders = settings.train_folders
+            self._has_mandatory('data_module_train', 'the training and validating data folders')
+            self.data_module_train = settings.data_module_train
+            self._check_data_module(self.data_module_train)
 
             self._has_mandatory('validating_ratio', 'the ratio of data for validation')
             self.validating_ratio = settings.validating_ratio
 
             self._has_mandatory('max_epochs', 'the maximum number of epochs')
             self.max_epochs = settings.max_epochs
 
@@ -202,31 +195,14 @@
             self.training_step = settings.training_step
 
             self._has_mandatory('eval_step', 'the function for the evaluation step')
             self._is_function('eval_step', 2)
             self.eval_step = settings.eval_step
 
             # Optional settings
-            if hasattr(settings, 'image_filter'):
-                self._is_of_type('image_filter', dict)
-                self.image_filter = settings.image_filter
-            else:
-                self.image_filter = {}
-
-            if hasattr(settings, 'event_filter'):
-                self._is_of_type('event_filter', dict)
-                self.event_filter = settings.event_filter
-            else:
-                self.event_filter = {}
-            if hasattr(settings, 'data_augment'):
-                self._is_of_type('data_augment', dict)
-                self.data_augment = settings.data_augment
-            else:
-                self.data_augment = None
-
             if hasattr(settings, 'dataset_size'):
                 self._is_of_type('dataset_size', int)
                 self.dataset_size = settings.dataset_size
             else:
                 self.dataset_size = None
 
             if hasattr(settings, 'files_max_number'):
@@ -265,26 +241,23 @@
 
             if hasattr(settings, 'training_callbacks'):
                 self.training_callbacks = settings.training_callbacks
             else:
                 self.training_callbacks = []
 
         else:
-            self.train_folders = None
+            self.data_module_train = None
             self.validating_ratio = None
             self.max_epochs = 0
             self.batch_size = None
             self.compute_loss = None
             self.optimizer_parameters = None
             self.optimizer_dic = None
             self.training_step = None
             self.eval_step = None
-            self.image_filter = {}
-            self.event_filter = {}
-            self.data_augment = None
             self.dataset_size = None
             self.files_max_number = None
             self.pin_memory = False
             self.split_by_file = True
             self.regularization = None
             self.check_val_every_n_epoch = 1
             self.lr_schedulers = None
@@ -293,41 +266,31 @@
         ########################################################################################################
         # Test settings
         if self.test:
             self._has_mandatory('test_step', 'the test iteration')
             self._is_function('test_step', 2)
             self.test_step = settings.test_step
 
+            if hasattr(settings, 'merge_test_datasets'):
+                self._is_of_type('merge_test_datasets', bool)
+                self.merge_test_datasets = settings.merge_test_datasets
+            else:
+                self.merge_test_datasets = False
+
             if hasattr(settings, 'test_dataset_parameters'):
                 self._is_of_type('test_dataset_parameters', dict)
                 self.test_dataset_parameters = settings.test_dataset_parameters
             else:
                 self.test_dataset_parameters = None
 
-            if hasattr(settings, 'test_image_filter'):
-                self._is_of_type('test_image_filter', dict)
-                self.test_image_filter = settings.test_image_filter
-            else:
-                self.test_image_filter = {}
-
-            if hasattr(settings, 'test_event_filter'):
-                self._is_of_type('test_event_filter', dict)
-                self.test_event_filter = settings.test_event_filter
-            else:
-                self.test_event_filter = {}
-
-            if hasattr(settings, 'test_folders'):
-                self._is_of_type('test_folders', list)
-                self.test_folders = settings.test_folders
-                if not self.test_folders:
-                    self.test_folders = None
-            else:
-                self.test_folders = None
-            if not self.test_folders:
-                self.test_folders = None
+            if hasattr(settings, 'data_module_test') and settings.data_module_test is not None:
+                self.data_module_test = settings.data_module_test
+                self._check_data_module(self.data_module_test, train=False)
+            else:
+                self.data_module_test = None
 
             if hasattr(settings, 'dl2_path'):
                 self._is_of_type('dl2_path', str)
                 self.dl2_path = settings.dl2_path
                 if not self.dl2_path:
                     self.dl2_path = None
             else:
@@ -349,17 +312,16 @@
             if hasattr(settings, 'test_callbacks'):
                 self.test_callbacks = settings.test_callbacks
             else:
                 self.test_callbacks = []
 
         else:
             self.test_step = None
-            self.test_image_filter = {}
-            self.test_event_filter = {}
-            self.test_folders = None
+            self.data_module_test = None
+            self.merge_test_datasets = False
             self.test_batch_size = None
             self.test_callbacks = []
             self.test_dataset_parameters = None
 
     def _has_mandatory(self, parameter, message):
         try:
             assert hasattr(self._settings, parameter)
@@ -394,28 +356,67 @@
             raise err
         try:
             assert len(inspect.getfullargspec(getattr(self._settings, parameter))[0]) == n_args
         except AssertionError as err:
             self._logger.exception(message)
             raise err
 
+    def _check_data_module(self, data_module, train=True):
+        '''
+        Checks have been conducted before the call of this function to ensure that :
+            - 'data_module_train' exists
+            - 'data_module_test' is not None when this function is called
+        This function realize these tests :
+            - Check if source and target keys are provided
+            - Train source paths must be provided (minimum required)
+            - At least one of source or target paths must be provided for test, otherwise user must set 'data_module_test' to None
+            - Target paths, 'image_filter' and 'event_filter' are set to {} if not provided
+        '''
+
+        data_module['source'] = data_module.get('source', {})
+        data_module['target'] = data_module.get('target', {})
+
+        data_module['target']['paths'] = data_module['target'].get('paths', [])
+
+        if train: # Train source paths are mandatory
+            message = 'Specification error on  {param}. It must non-empty'.format(param="data_module_train['source']['paths']")
+            try:
+                assert data_module['source']['paths'] and isinstance(data_module['source']['paths'], list)
+            except AssertionError as err:
+                self._logger.exception(message)
+                raise err
+        else: # For test, at least one of source and target paths must be non-empty
+            data_module['source']['paths'] = data_module['source'].get('paths', [])
+
+            message = 'Specification error on  {param}. At list one path must be non-empty, otherwise data_module_test must be set to None'.format(param="data_module_test")
+            try:
+                assert (data_module['target']['paths'] and isinstance(data_module['target']['paths'], list)) or (data_module['source']['paths'] and isinstance(data_module['source']['paths'], list))
+            except AssertionError as err:
+                self._logger.exception(message)
+                raise err
+        
+        data_module['source']['image_filter'] = data_module['source'].get('image_filter', {})
+        data_module['source']['event_filter'] = data_module['source'].get('event_filter', {})
+
+        data_module['target']['image_filter'] = data_module['target'].get('image_filter', {})
+        data_module['target']['event_filter'] = data_module['target'].get('event_filter', {})
 
-class LitGLearnModule(LightningModule):
 
+class LitGLearnModule(LightningModule):
     def __init__(self, experiment):
         super().__init__()
         # TODO save hyperparameters
         # self.save_hyperparameters(dict from experiment)
         self.automatic_optimization = False
         self.experiment = experiment
         self.console_logger = logging.getLogger(__name__)
         self.grad_norm = 0
 
         # create network
-        self.net = self.experiment.model_net(self.experiment.net_parameters_dic, self.experiment.camera_geometry)
+        self.net = self.experiment.net_parameters_dic['model'](self.experiment.net_parameters_dic['parameters'])
         self.console_logger.info(
             'network parameters number : {}'.format(compute_total_parameter_number(self.net))
         )
         self.metrics = torch.nn.ModuleDict()
         for task, param in self.experiment.targets.items():
             self.metrics[task] = torch.nn.ModuleDict()
             for name, metric in param['metrics'].items():
@@ -433,15 +434,15 @@
         optimizers = self.optimizers(use_pl_optimizer=True)
         if isinstance(optimizers, list):
             for optim in optimizers:
                 optim.zero_grad()
         else:
             optimizers.zero_grad()
 
-        if self.global_step == 0:
+        if batch_idx == 0 and self.trainer.current_epoch == 0:
             self.console_logger.info(('Experiment running on {}'.format(self.device)))  # TODO handle multi gpus
             if self.device.type == 'cuda':
                 self.console_logger.info('GPU name : {}'.format(torch.cuda.get_device_name(self.device.index)))
 
         output, labels, loss_data, loss = self.experiment.training_step(self, batch)
 
         self.manual_backward(loss)
@@ -454,15 +455,15 @@
         if isinstance(optimizers, list):
             for optim in optimizers:
                 optim.step()
         else:
             optimizers.step()
 
         # log losses
-        if self.global_step == 0:
+        if batch_idx == 0 and self.trainer.current_epoch == 0:
             self.logger.experiment.add_scalars('Training', {'Loss_' + n: v for n, v in loss_data.items()})
         self.log('Training', {'Loss_' + n: v for n, v in loss_data.items()}, on_step=False, on_epoch=True)
         training_loss = 0
         for v in loss_data.values():
             training_loss += v
         self.log('Loss', {'training': training_loss}, on_step=False, on_epoch=True)
         self.log('Loss_weighted', {'training': loss.detach()}, on_step=False, on_epoch=True)
@@ -472,55 +473,62 @@
                 if task == 'class':
                     m_value = metric(torch.exp(output[task]), labels[task])
                 else:
                     m_value = metric(output[task], labels[task])
                 self.log(name, {'training': m_value}, on_step=False, on_epoch=True)
         # Log in console
         n_batches = len(self.trainer.train_dataloader)
-        iteration = self.global_step % n_batches + 1
-        if iteration % self.experiment.log_every_n_steps == 0:
-            self.console_logger.info('Epoch[{}] Iteration[{}/{}]'.format(self.current_epoch, iteration, n_batches))
+        if (batch_idx + 1) % self.experiment.log_every_n_steps == 0:
+            self.console_logger.info('Epoch[{}] Iteration[{}/{}]'.format(self.current_epoch, batch_idx+1, n_batches))
             # log losses
             for n, v in loss_data.items():
                 self.console_logger.info('Training Loss ' + n + ' {}'.format(v))
             # log other metrics
             for task, all_metrics in self.metrics.items():
                 for name, metric in all_metrics.items():
-                    if task == 'class':
+                    if 'class' in task:
                         m_value = metric(torch.exp(output[task]), labels[task])
                     else:
                         m_value = metric(output[task], labels[task])
                     self.console_logger.info('Training ' + name + ' {}'.format(m_value))
         return loss
 
     def training_epoch_end(self, outputs):
         lr_schedulers = self.lr_schedulers()
         if lr_schedulers is not None:
             lr_schedulers = [lr_schedulers] if not isinstance(lr_schedulers, list) else lr_schedulers
             for scheduler in lr_schedulers:
                 if isinstance(scheduler, torch.optim.lr_scheduler.ReduceLROnPlateau):
                     scheduler.step(self.trainer.callback_metrics["Loss_validating"])
-                else:
+                elif not isinstance(scheduler, DANNLR):
                     scheduler.step()
 
+    def training_step_end(self, batch_parts):
+        lr_schedulers = self.lr_schedulers()
+        if lr_schedulers is not None:
+            lr_schedulers = [lr_schedulers] if not isinstance(lr_schedulers, list) else lr_schedulers
+            for scheduler in lr_schedulers:
+                if isinstance(scheduler, DANNLR):
+                    scheduler.step(self)
+
     def validation_step(self, batch, batch_idx):
         output, labels, loss_data, loss = self.experiment.eval_step(self, batch)
         # log losses
         self.log('Validating', {'Loss_' + n: v for n, v in loss_data.items()})
         val_loss = 0
         for n, v in loss_data.items():
             # self.console_logger.info('Validating ' + n + ' {}'.format(v))
             val_loss += v
         self.log('Loss', {'validating': val_loss})
         self.log('Loss_validating', loss.detach())
         self.log('Loss_weighted', {'validating': loss.detach()})
         # log other metrics
         for task, all_metrics in self.metrics.items():
             for name, metric in all_metrics.items():
-                if task == 'class':
+                if 'class' in task:
                     metric(torch.exp(output[task]), labels[task])
                 else:
                     metric(output[task], labels[task])
 
     def validation_epoch_end(self, *args, **kwargs):
         self.console_logger.info('Epoch[{}] Validation]'.format(self.current_epoch))
         # log other metrics
@@ -548,34 +556,38 @@
                 'You need an optimizer for every subparts of the net.'
 
         optimizers = {}
         for key in self.experiment.optimizer_dic.keys():
             if key == 'network':
                 optimizers[key] = self.experiment.optimizer_dic[key](self.net,
                                                                      self.experiment.optimizer_parameters[key])
-            elif key == 'feature':
-                optimizers[key] = self.experiment.optimizer_dic[key](self.net.feature,
-                                                                     self.experiment.optimizer_parameters[key])
-            elif key == 'classifier':
-                optimizers[key] = self.experiment.optimizer_dic[key](self.net.classifier,
-                                                                     self.experiment.optimizer_parameters[key])
-            elif key == 'regressor':
-                optimizers[key] = self.experiment.optimizer_dic[key](self.net.regressor,
-                                                                     self.experiment.optimizer_parameters[key])
             elif key == 'loss_balancing':
                 assert isinstance(self.experiment.compute_loss, torch.nn.Module)
                 optimizers[key] = self.experiment.optimizer_dic[key](self.experiment.compute_loss,
                                                                      self.experiment.optimizer_parameters[key])
+            else:
+                try:
+                    assert getattr(self.net, key, None) is not None
+                except AssertionError as e:
+                    self.console_logger.error(e)
+                    print(key)
+                    print(self.net)
+                    raise e
+                optimizers[key] = self.experiment.optimizer_dic[key](getattr(self.net, key),
+                                                                     self.experiment.optimizer_parameters[key])
 
         if self.experiment.lr_schedulers is not None:
             schedulers = []
-            for scheduler, options in self.experiment.lr_schedulers.items():
-                for net_param, scheduler_param in options.items():
+            for net_param, scheduler_param in self.experiment.lr_schedulers.items():
+                for scheduler, params in scheduler_param.items():
                     if optimizers[net_param] is not None:
-                        schedulers.append(scheduler(optimizers[net_param], **scheduler_param))
+                        schedulers.append({
+                            'scheduler': scheduler(optimizers[net_param], **params),
+                            'name': 'lr_' + net_param
+                        })
         else:
             schedulers = None
 
         return list(optimizers.values()), schedulers
 
 
 def main():
@@ -660,15 +672,15 @@
     geometries = []
     get_dataset_geom(gl_data_module.train_set, geometries)
     get_dataset_geom(gl_data_module.test_sets, geometries)
     # testing if all geometries are equal
     if len(set(geometries)) != 1:
         raise WrongGeometryError("There are different geometries in the train and the test datasets")
 
-    experiment.camera_geometry = geometries[0]
+    experiment.net_parameters_dic = inject_geometry_into_parameters(experiment.net_parameters_dic, geometries[0])
 
     # Define multiprocessing start method
     try:
         assert torch.multiprocessing.get_start_method() == experiment.mp_start_method
     except AssertionError:
         torch.multiprocessing.set_start_method(experiment.mp_start_method, force=True)
     logger.info('mp start method: {}'.format(torch.multiprocessing.get_start_method()))
@@ -688,17 +700,19 @@
                                           monitor='Loss_validating', filename='checkpoint_{epoch}',
                                           every_n_epochs=experiment.save_every, save_top_k=-1)
 
     # Log learning rates
     callbacks = [
         checkpoint_callback,
         LearningRateMonitor(logging_interval='epoch'),
-        DeviceStatsMonitor()
     ]
 
+    if experiment.monitor_gpus and experiment.gpus not in [None, 0]:
+        callbacks.append(GPUStatsMonitor())
+
     callbacks.extend(experiment.training_callbacks)
     callbacks.extend(experiment.test_callbacks)
 
     # Prepare profiler
     if experiment.profiler is not None:
         profiler = experiment.profiler['profiler'](
             dirpath=os.path.join(experiment.main_directory, experiment.experiment_name),
@@ -721,24 +735,23 @@
                 filename=os.path.join(experiment.experiment_name + '.prof'),
                 **experiment.profiler['options'])
             trainer.profiler = profiler
 
         trainer.test(gl_lightning_module,
                      dataloaders=gl_data_module.test_dataloader())
     else:
-        trainer = pl.Trainer(
-            default_root_dir=os.path.join(experiment.main_directory, experiment.experiment_name),
-            gpus=experiment.gpus, strategy=experiment.ddp, max_epochs=experiment.max_epochs,
-            resume_from_checkpoint=experiment.checkpoint_path, logger=tb_logger,
-            log_every_n_steps=experiment.log_every_n_steps,
-            check_val_every_n_epoch=experiment.check_val_every_n_epoch,
-            callbacks=callbacks, profiler=profiler
-        )
-
         if experiment.train:
+            trainer = pl.Trainer(
+                default_root_dir=os.path.join(experiment.main_directory, experiment.experiment_name),
+                gpus=experiment.gpus, strategy=experiment.ddp, max_epochs=experiment.max_epochs,
+                resume_from_checkpoint=experiment.checkpoint_path, logger=tb_logger,
+                log_every_n_steps=experiment.log_every_n_steps,
+                check_val_every_n_epoch=experiment.check_val_every_n_epoch,
+                callbacks=callbacks, profiler=profiler, 
+            )
             logger.info('Train model')
             trainer.fit(gl_lightning_module,
                         train_dataloaders=gl_data_module.train_dataloader(),
                         val_dataloaders=gl_data_module.val_dataloader())
             if experiment.test:
                 logger.info('Test model')
                 for dataloader in gl_data_module.test_dataloaders():
@@ -750,14 +763,20 @@
                             **experiment.profiler['options'])
                         trainer.profiler = profiler
 
                     trainer.test(gl_lightning_module,
                                  dataloaders=dataloader)
                     gl_lightning_module.reset_test_data()
         elif experiment.test:
+            trainer = pl.Trainer(
+                default_root_dir=os.path.join(experiment.main_directory, experiment.experiment_name),
+                gpus=experiment.gpus, strategy=experiment.ddp,
+                resume_from_checkpoint=experiment.checkpoint_path, logger=tb_logger,
+                callbacks=callbacks
+            )
             logger.info('Test model')
             assert experiment.checkpoint_path is not None, 'To test a model w/o training, there must be a checkpoint'
             map_location = torch.device('cpu') if experiment.gpus == 0 else None
             ckpt = torch.load(experiment.checkpoint_path, map_location=map_location)
             gl_lightning_module.load_state_dict(ckpt['state_dict'])
             for dataloader in gl_data_module.test_dataloaders():
                 # TODO remove when lightning bug is fixed
@@ -767,10 +786,9 @@
                         filename=os.path.join(experiment.experiment_name + '.prof'),
                         **experiment.profiler['options'])
                     trainer.profiler = profiler
 
                 trainer.test(gl_lightning_module, dataloaders=dataloader)
                 gl_lightning_module.reset_test_data()
 
-
 if __name__ == '__main__':
     main()
```

### Comparing `Gammalearn-0.8/gammalearn/logging.py` & `Gammalearn-0.9/gammalearn/logging.py`

 * *Files identical despite different names*

### Comparing `Gammalearn-0.8/gammalearn/metrics.py` & `Gammalearn-0.9/gammalearn/metrics.py`

 * *Files identical despite different names*

### Comparing `Gammalearn-0.8/gammalearn/open_blackbox.py` & `Gammalearn-0.9/gammalearn/open_blackbox.py`

 * *Files identical despite different names*

### Comparing `Gammalearn-0.8/gammalearn/tests/test_criterions.py` & `Gammalearn-0.9/gammalearn/tests/test_criterions.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,28 +21,31 @@
         self.targets = {
             'energy': {
                 'output_shape': 1,
                 'loss': torch.nn.L1Loss(reduction='none'),
                 'loss_weight': 1,
                 'metrics': {
                     # 'functions': ,
-                }
+                },
+                'mt_balancing': True
             },
             'impact': {
                 'output_shape': 2,
                 'loss': torch.nn.L1Loss(reduction='none'),
                 'loss_weight': 1,
-                'metrics': {}
+                'metrics': {},
+                'mt_balancing': True
             },
             'class': {
                 'output_shape': 2,
                 'label_shape': 1,
-                'loss': criterions.nll_nn,
+                'loss': torch.nn.CrossEntropyLoss(),
                 'loss_weight': 1,
-                'metrics': {}
+                'metrics': {},
+                'mt_balancing': True
             },
         }
         self.particle_dict = {0: 1, 1: 2, 101: 0}
         self.loss_options_masked = {
             'conditional': True,
             'gamma_class': self.particle_dict[csts.GAMMA_ID],
         }
```

### Comparing `Gammalearn-0.8/gammalearn/tests/test_datasets.py` & `Gammalearn-0.9/gammalearn/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `Gammalearn-0.8/gammalearn/tests/test_utils.py` & `Gammalearn-0.9/gammalearn/tests/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,34 @@
 
         self.multiplicity_parameters = {'multiplicity': 2}
         self.multiplicity_true_mask = [True, True, False, False]
         self.multiplicity_strict_parameters = {'multiplicity': 1, 'strict': True}
         self.multiplicity_strict_true_mask = [False, False, True, True]
         self.multiplicity_strict_true_trig_energies = np.array([0.010, 0.12, 0.8])
 
+        self.net_parameters_dic = {
+            'model': 'GammaPhysNet',
+            'parameters': {
+                'backbone': {
+                    'model': 'ResNetAttentionIndexed',
+                    'parameters': {
+                        'num_layers': 3,
+                        'init': 'kaiming',
+                        'batch_norm': True,
+                        # 'init': 'orthogonal',
+                        'num_channels': 2,
+                        'block_features': [16, 32, 64],
+                        'attention_layer': ('DualAttention', {'ratio': 16}),
+                    }
+                },
+                'fc_width': 256,
+                'last_bias_init': None,
+            }
+        }
+
     def test_emission_cone(self):
         self.dataset = MockLSTDataset()
         assert np.all(utils.emission_cone_filter(self.dataset, **self.emission_cone_parameters) ==
                       self.emission_cone_true_mask)
 
     def test_impact_distance(self):
         self.dataset = MockLSTDataset()
@@ -113,14 +133,18 @@
         np.testing.assert_array_equal(utils.rotated_indices(pix_pos, np.pi/2), [1, 2, 3, 0])
         np.testing.assert_array_equal(utils.rotated_indices(pix_pos, -np.pi / 2), [3, 0, 1, 2])
 
     def test_nets_definition_path(self):
         path = utils.nets_definition_path()
         assert os.path.exists(path)
 
+    def test_inject_geometry_into_parameters(self):
+        self.net_parameters_dic = utils.inject_geometry_into_parameters(self.net_parameters_dic, 'LSTCam_geometry')
+        assert self.net_parameters_dic['parameters']['backbone']['parameters']['camera_geometry'] == 'LSTCam_geometry'
+
 
 class TestIndexMatrix(unittest.TestCase):
 
     def setUp(self):
         lstcam_geom = CameraGeometry.from_name('LSTCam-002')
         self.minihex = deepcopy(lstcam_geom)
         self.minihex.camera_name = 'minihex'
@@ -253,15 +277,14 @@
 
         np.testing.assert_array_equal(idx_mat, [[ 0,  1,  2, -1, -1],
                                                 [ 3,  4,  5,  6, -1],
                                                 [ 7,  8,  9, 10, 11],
                                                 [-1, 12, 13, 14, 15],
                                                 [-1, -1, 16, 17, 18]])
 
-
     def test_compare_indexedconv_method(self):
         """
         Test that the new method gives the same result as the previous one for the LSTCam geometry
         """
         import indexedconv.utils as cvutils
         from gammalearn.utils import load_camera_parameters
 
@@ -270,12 +293,9 @@
         lst_geom = CameraGeometry.from_name('LSTCam')
         new_idx_mat, camera_layout = utils.get_camera_layout_from_geom(lst_geom)
 
         assert camera_layout == 'Hex'
         np.testing.assert_array_equal(idx_mat.numpy(), new_idx_mat.numpy())
 
 
-
-
-
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `Gammalearn-0.8/gammalearn/utils.py` & `Gammalearn-0.9/gammalearn/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -88,53 +88,14 @@
     if not os.path.exists(test_directory):
         os.makedirs(test_directory)
         os.chmod(test_directory, 0o775)
     logger.debug('Gammaboard runs directory: {} '.format(test_directory))
     return test_directory
 
 
-def record_experiment(experiment):
-    """
-    Record the main parameters of the experiment in a file containing all the experiments
-
-    Parameters
-    ----------
-    experiment (Experiment) : experiment
-
-    Returns
-    -------
-
-    """
-    with open(experiment.main_directory + '/experiments.csv', 'a', newline='') as f:
-        writer = csv.writer(f)
-
-        optim = {
-            key: experiment.optimizer_dic[key].__name__
-            for key in experiment.optimizer_dic.keys()
-        }
-
-        criterion = {
-            task: param['loss'].__name__
-            if inspect.isfunction(param['loss'])
-            else param['loss'].__class__.__name__
-            for task, param in experiment.targets.items()
-        }
-
-        writer.writerow([experiment.experiment_name,
-                         experiment.model_net.__name__,
-                         optim,
-                         experiment.optimizer_parameters,
-                         criterion,
-                         experiment.batch_size,
-                         experiment.nepochs,
-                         experiment.image_filter,
-                         experiment.event_filter,
-                         experiment.files_folders])
-
-
 def resume_model(model, path):
     """
     Resume the model with the one stored in the path.
     https://discuss.pytorch.org/t/how-to-load-part-of-pre-trained-model/1113/16
     Parameters
     ----------
     model (torch.Module)
@@ -271,64 +232,74 @@
     """
     exp_settings = collections.OrderedDict({'exp_name': experiment.experiment_name,
                                             'gammalearn': version.__version__,
                                             'dataset_class': format_name(experiment.dataset_class),
                                             'dataset_parameters': experiment.dataset_parameters,
 
                                             })
-    exp_settings['network'] = {format_name(experiment.model_net): {k: format_name(v)
-                                                                   for k, v in experiment.net_parameters_dic.items()}}
+    exp_settings['network'] = {
+        format_name(experiment.net_parameters_dic['model']): {k: format_name(v)
+                                                              for k, v in
+                                                              experiment.net_parameters_dic['parameters'].items()}}
     if experiment.checkpoint_path is not None:
         exp_settings['resume_checkpoint'] = os.path.join(os.path.dirname(experiment.checkpoint_path).split('/')[-1],
                                                          os.path.basename(experiment.checkpoint_path))
     if experiment.info is not None:
         exp_settings['info'] = experiment.info
+
     if experiment.train:
-        exp_settings['files_folders'] = experiment.train_folders
         exp_settings['num_epochs'] = experiment.max_epochs
         exp_settings['batch_size'] = experiment.batch_size
-        if experiment.image_filter:
-            exp_settings['image filters'] = {format_name(filter_func): filter_param
-                                             for filter_func, filter_param
-                                             in experiment.image_filter.items()}
-        if experiment.event_filter:
-            exp_settings['event filters'] = {format_name(filter_func): filter_param
-                                             for filter_func, filter_param
-                                             in experiment.event_filter.items()}
-        if experiment.data_augment is not None:
-            exp_settings['data_augmentation'] = {
-                format_name(experiment.data_augment['function']): experiment.data_augment['kwargs']
-            }
+        for data_type in ['source', 'target']:
+            data_module = experiment.data_module_train[data_type]
+            exp_settings['files_folders ' + data_type] = data_module['paths']
+            if data_module['image_filter']:
+                image_filter = data_module['image_filter']
+                exp_settings['image filters ' + data_type] = {format_name(filter_func): filter_param
+                                                              for filter_func, filter_param
+                                                              in image_filter.items()}
+            if data_module['event_filter']:
+                event_filter = data_module['event_filter']
+                exp_settings['event filters ' + data_type] = {format_name(filter_func): filter_param
+                                                              for filter_func, filter_param
+                                                              in event_filter.items()}
+
         exp_settings['losses'] = {
             k: {
-                'loss': format_name(v['loss']),
-                'weight': v['loss_weight']
+                'loss': format_name(v.get('loss', None)),
+                'weight': v.get('loss_weight', None)
             }
             for k, v in experiment.targets.items()
         }
 
         exp_settings['loss_function'] = format_name(experiment.compute_loss)
         exp_settings['optimizer'] = {key: format_name(value) for key, value in experiment.optimizer_dic.items()}
         exp_settings['optimizer_parameters'] = {opt: {key: format_name(value)
                                                       for key, value in param.items()}
                                                 for opt, param in experiment.optimizer_parameters.items()}
         if experiment.lr_schedulers is not None:
-            exp_settings['lr_schedulers'] = {format_name(handler): param
-                                             for handler, param in experiment.lr_schedulers.items()}
+            exp_settings['lr_schedulers'] = {net_param: {format_name(scheduler):param for scheduler, param in scheduler_param.items()}
+                                             for net_param, scheduler_param in experiment.lr_schedulers.items()}
+
     if experiment.test:
-        if experiment.test_folders is not None:
-            exp_settings['test_folders'] = experiment.test_folders
-        if experiment.test_image_filter:
-            exp_settings['test image filters'] = {format_name(filter_func): filter_param
-                                                  for filter_func, filter_param
-                                                  in experiment.test_image_filter.items()}
-        if experiment.test_event_filter:
-            exp_settings['test event filters'] = {format_name(filter_func): filter_param
-                                                  for filter_func, filter_param
-                                                  in experiment.test_event_filter.items()}
+        if experiment.data_module_test is not None:
+            for data_type in ['source', 'target']:
+                data_module = experiment.data_module_test[data_type]
+                if data_module['paths']:
+                    exp_settings['test_folders ' + data_type] = data_module['paths']
+                if data_module['image_filter']:
+                    image_filter = data_module['image_filter']
+                    exp_settings['test image filters ' + data_type] = {format_name(filter_func): filter_param
+                                                                       for filter_func, filter_param
+                                                                       in image_filter.items()}
+                if data_module['event_filter']:
+                    event_filter = data_module['event_filter']
+                    exp_settings['test event filters ' + data_type] = {format_name(filter_func): filter_param
+                                                                       for filter_func, filter_param
+                                                                       in event_filter.items()}
 
     experiment_path = experiment.main_directory + '/' + experiment.experiment_name + '/'
     settings_path = experiment_path + experiment.experiment_name + '_settings.json'
     with open(settings_path, 'w') as f:
         json.dump(exp_settings, f)
 
 
@@ -349,14 +320,46 @@
             if k not in merge_dict:
                 merge_dict[k] = [v]
             else:
                 merge_dict[k].append(v)
     return merge_dict
 
 
+def prepare_dict_of_tensors(dic):
+    for k, v in dic.items():
+        dic[k] = v.squeeze(1).tolist() if v.ndim > 1 else v.tolist()
+    return dic
+
+
+# TODO Remove when corresponding lstchain function is exposed
+def write_dataframe(dataframe, outfile, table_path, mode="a", index=False):
+    """
+    From lstchain
+    Write a pandas dataframe to a HDF5 file using pytables formatting.
+    Parameters
+    ----------
+    dataframe: `pandas.DataFrame`
+    outfile: path
+    table_path: str
+        path to the table to write in the HDF5 file
+    """
+    if not table_path.startswith("/"):
+        table_path = "/" + table_path
+
+    with tables.open_file(outfile, mode=mode) as f:
+        path, table_name = table_path.rsplit("/", maxsplit=1)
+
+        f.create_table(
+            path,
+            table_name,
+            dataframe.to_records(index=index),
+            createparents=True,
+        )
+
+
 ###########
 # Filters #
 ###########
 ##################################################################################################
 # Event base filters
 
 def energyband_filter(dataset, energy=None, filter_only_gammas=False):
@@ -765,29 +768,57 @@
     Parameters
     ----------
     d: list or `torch.utils.ConcatDataset` or `torch.utils.data.Subset` or `torch.utils.data.Dataset`
     geometries: list
 
     """
     if isinstance(d, list):
-        print('d is a list')
         for d_l in d:
             get_dataset_geom(d_l, geometries)
     elif isinstance(d, torch.utils.data.ConcatDataset):
         for d_c in d.datasets:
             get_dataset_geom(d_c, geometries)
     elif isinstance(d, torch.utils.data.Subset):
         get_dataset_geom(d.dataset, geometries)
     elif isinstance(d, torch.utils.data.Dataset):
         geometries.append(d.camera_geometry)
 
 
+def inject_geometry_into_parameters(parameters: dict, camera_geometry):
+    """
+    Adds camera geometry in model backbone parameters
+    """
+    for k, v in parameters.items():
+        if k == 'backbone':
+            v['parameters']['camera_geometry'] = camera_geometry
+        elif isinstance(v, dict):
+            parameters[k] = inject_geometry_into_parameters(v, camera_geometry)
+    return parameters
+
+
 def nets_definition_path():
     """
     Return the path to the net definition file
 
     Returns
     -------
     str
     """
     return pkg_resources.resource_filename('gammalearn', 'data/nets.py')
 
+
+def compute_dann_hparams(module, gamma=10, alpha=10, beta=0.75): # TO DO (check if max_steps updated when trainer is created)
+    current_step = module.trainer.fit_loop.total_batch_idx + 1  # The current step (does not reset each epoch)
+    max_steps = module.trainer.estimated_stepping_batches  # Stop training after this number of steps
+
+    mu = None
+    for model, params in module.experiment.optimizer_parameters.items():
+        if model == 'domain_classifier':
+            mu = params['lr']
+
+    assert mu is not None, "No domain classifier found in optimizer parameters."
+
+    p = torch.tensor(current_step / max_steps, dtype=torch.float32)  # Training progress (from 0 to 1)
+    lambda_p = 2.0 / (1.0 + torch.exp(-gamma * p)) - 1.0
+    mu_p = mu / torch.pow(1.0 + alpha * p, torch.tensor(beta))
+
+    return lambda_p, mu_p
```

### Comparing `Gammalearn-0.8/gammalearn/version.py` & `Gammalearn-0.9/gammalearn/version.py`

 * *Files identical despite different names*

### Comparing `Gammalearn-0.8/notebook/geometry_convert.ipynb` & `Gammalearn-0.9/notebook/geometry_convert.ipynb`

 * *Files identical despite different names*

### Comparing `Gammalearn-0.8/setup.py` & `Gammalearn-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     install_requires=[
         "torch>=1.7",
         "tensorboard",
         "torchvision",
         "numpy",
         "matplotlib",
         "tables",
-        "pytorch-lightning>=1.4",
+        "pytorch-lightning>=1.6",
         "indexedconv>=1.3",
         "ctapipe>=0.10",
         "ctaplot",
         "dl1_data_handler~=0.10",
         "lstchain>=0.7",
     ],
     setup_requires=["setuptools_scm"],
```

### Comparing `Gammalearn-0.8/share/create_camera_parameter_file.py` & `Gammalearn-0.9/share/create_camera_parameter_file.py`

 * *Files identical despite different names*

### Comparing `Gammalearn-0.8/share/data/MC_data/dl1_gamma_example.h5` & `Gammalearn-0.9/share/data/MC_data/dl1_gamma_example.h5`

 * *Files identical despite different names*

### Comparing `Gammalearn-0.8/share/data/MC_data/dl1_proton_example.h5` & `Gammalearn-0.9/share/data/MC_data/dl1_proton_example.h5`

 * *Files identical despite different names*

### Comparing `Gammalearn-0.8/share/data/real_data/dl1_realdata_example.h5` & `Gammalearn-0.9/share/data/real_data/dl1_realdata_example.h5`

 * *Files identical despite different names*

