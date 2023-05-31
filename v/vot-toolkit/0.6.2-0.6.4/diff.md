# Comparing `tmp/vot-toolkit-0.6.2.tar.gz` & `tmp/vot-toolkit-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vot-toolkit-0.6.2.tar", last modified: Tue May 16 14:36:57 2023, max compression
+gzip compressed data, was "vot-toolkit-0.6.4.tar", last modified: Wed May 31 07:41:25 2023, max compression
```

## Comparing `vot-toolkit-0.6.2.tar` & `vot-toolkit-0.6.4.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.862747 vot-toolkit-0.6.2/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      211 2022-03-25 11:28:05.000000 vot-toolkit-0.6.2/MANIFEST.in
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3646 2023-05-16 14:36:57.862747 vot-toolkit-0.6.2/PKG-INFO
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2716 2023-05-09 11:09:24.000000 vot-toolkit-0.6.2/README.md
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      295 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/requirements.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       38 2023-05-16 14:36:57.862747 vot-toolkit-0.6.2/setup.cfg
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1427 2023-05-09 11:09:24.000000 vot-toolkit-0.6.2/setup.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.834747 vot-toolkit-0.6.2/vot/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1889 2023-05-10 17:51:17.000000 vot-toolkit-0.6.2/vot/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      158 2021-04-20 09:19:05.000000 vot-toolkit-0.6.2/vot/__main__.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.834747 vot-toolkit-0.6.2/vot/analysis/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16084 2023-05-16 13:31:56.000000 vot-toolkit-0.6.2/vot/analysis/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    21427 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/analysis/_processor.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7601 2023-05-16 13:31:56.000000 vot-toolkit-0.6.2/vot/analysis/accuracy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2535 2023-05-16 13:31:56.000000 vot-toolkit-0.6.2/vot/analysis/failures.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16995 2023-05-16 13:31:56.000000 vot-toolkit-0.6.2/vot/analysis/longterm.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12289 2023-05-16 13:31:56.000000 vot-toolkit-0.6.2/vot/analysis/multistart.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8860 2023-05-16 13:31:56.000000 vot-toolkit-0.6.2/vot/analysis/supervised.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.838747 vot-toolkit-0.6.2/vot/dataset/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16723 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/dataset/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14672 2020-12-04 15:25:26.000000 vot-toolkit-0.6.2/vot/dataset/cow.png
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3079 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/dataset/dummy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5356 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/dataset/got10k.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    11511 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/dataset/otb.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4924 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/dataset/proxy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3753 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/dataset/trackingnet.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10365 2023-05-16 14:28:55.000000 vot-toolkit-0.6.2/vot/dataset/vot.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.842747 vot-toolkit-0.6.2/vot/document/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12362 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/document/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      465 2020-12-04 15:25:26.000000 vot-toolkit-0.6.2/vot/document/commands.tex
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5298 2023-05-16 13:31:56.000000 vot-toolkit-0.6.2/vot/document/common.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5217 2021-04-15 12:10:29.000000 vot-toolkit-0.6.2/vot/document/html.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    89476 2020-12-04 15:25:26.000000 vot-toolkit-0.6.2/vot/document/jquery.js
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5748 2022-03-11 09:29:31.000000 vot-toolkit-0.6.2/vot/document/latex.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16184 2020-12-04 15:25:26.000000 vot-toolkit-0.6.2/vot/document/pure.css
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      647 2020-12-04 15:25:26.000000 vot-toolkit-0.6.2/vot/document/report.css
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1212 2020-12-04 15:25:26.000000 vot-toolkit-0.6.2/vot/document/report.js
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9933 2020-12-04 15:25:26.000000 vot-toolkit-0.6.2/vot/document/table.js
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        0 2022-03-23 08:48:42.000000 vot-toolkit-0.6.2/vot/document/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.842747 vot-toolkit-0.6.2/vot/experiment/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7631 2023-05-16 07:48:27.000000 vot-toolkit-0.6.2/vot/experiment/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      798 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/experiment/helpers.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7180 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/experiment/multirun.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3044 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/experiment/multistart.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3214 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/experiment/transformer.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.842747 vot-toolkit-0.6.2/vot/region/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2373 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/region/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9258 2023-05-16 07:48:27.000000 vot-toolkit-0.6.2/vot/region/io.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9593 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/region/raster.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10172 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/region/shapes.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3238 2023-05-16 07:48:27.000000 vot-toolkit-0.6.2/vot/region/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.846747 vot-toolkit-0.6.2/vot/stack/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3047 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      253 2022-03-25 11:28:05.000000 vot-toolkit-0.6.2/vot/stack/otb100.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      251 2022-03-25 11:28:05.000000 vot-toolkit-0.6.2/vot/stack/otb50.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.846747 vot-toolkit-0.6.2/vot/stack/tests/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      183 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/tests/basic.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      541 2023-05-16 13:31:56.000000 vot-toolkit-0.6.2/vot/stack/tests/multiobject.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      638 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/tests/segmentation.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      863 2022-03-25 11:28:05.000000 vot-toolkit-0.6.2/vot/stack/tests.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      351 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2013.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      374 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2014.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.846747 vot-toolkit-0.6.2/vot/stack/vot2015/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      405 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2015/rgb.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      322 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2015/tir.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.846747 vot-toolkit-0.6.2/vot/stack/vot2016/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      540 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2016/rgb.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2016/tir.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      856 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2017.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.850747 vot-toolkit-0.6.2/vot/stack/vot2018/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2018/longterm.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      791 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2018/shortterm.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.850747 vot-toolkit-0.6.2/vot/stack/vot2019/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2019/longterm.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2019/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2019/rgbtir.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      789 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2019/shortterm.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.850747 vot-toolkit-0.6.2/vot/stack/vot2020/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2020/longterm.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2020/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2020/rgbtir.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2020/shortterm.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.854747 vot-toolkit-0.6.2/vot/stack/vot2021/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2021/lt.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2021/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2021/st.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.854747 vot-toolkit-0.6.2/vot/stack/vot2022/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      422 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/stack/vot2022/depth.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      482 2022-03-25 11:28:05.000000 vot-toolkit-0.6.2/vot/stack/vot2022/lt.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      424 2022-03-25 11:28:05.000000 vot-toolkit-0.6.2/vot/stack/vot2022/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2022-03-25 11:28:05.000000 vot-toolkit-0.6.2/vot/stack/vot2022/stb.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2022-03-25 11:28:05.000000 vot-toolkit-0.6.2/vot/stack/vot2022/sts.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      193 2023-05-10 17:51:17.000000 vot-toolkit-0.6.2/vot/stack/vots2023.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.858747 vot-toolkit-0.6.2/vot/tracker/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    19774 2023-05-16 07:48:27.000000 vot-toolkit-0.6.2/vot/tracker/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      763 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/tracker/dummy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6642 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/tracker/results.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      476 2021-04-20 09:19:05.000000 vot-toolkit-0.6.2/vot/tracker/tests.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    19771 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/tracker/trax.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.858747 vot-toolkit-0.6.2/vot/utilities/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12740 2023-05-16 14:21:10.000000 vot-toolkit-0.6.2/vot/utilities/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16476 2023-05-10 17:51:17.000000 vot-toolkit-0.6.2/vot/utilities/cli.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2635 2021-04-15 12:10:29.000000 vot-toolkit-0.6.2/vot/utilities/data.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8255 2021-04-15 12:10:29.000000 vot-toolkit-0.6.2/vot/utilities/draw.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3609 2020-12-04 15:25:26.000000 vot-toolkit-0.6.2/vot/utilities/migration.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5130 2023-05-16 14:33:12.000000 vot-toolkit-0.6.2/vot/utilities/net.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     8133 2022-03-25 11:28:05.000000 vot-toolkit-0.6.2/vot/utilities/notebook.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       45 2023-05-16 13:31:56.000000 vot-toolkit-0.6.2/vot/version.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.858747 vot-toolkit-0.6.2/vot/workspace/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7013 2023-05-05 11:01:43.000000 vot-toolkit-0.6.2/vot/workspace/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10512 2023-05-12 11:16:07.000000 vot-toolkit-0.6.2/vot/workspace/storage.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1786 2023-05-16 07:48:27.000000 vot-toolkit-0.6.2/vot/workspace/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-16 14:36:57.862747 vot-toolkit-0.6.2/vot_toolkit.egg-info/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3646 2023-05-16 14:36:57.000000 vot-toolkit-0.6.2/vot_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2409 2023-05-16 14:36:57.000000 vot-toolkit-0.6.2/vot_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        1 2023-05-16 14:36:57.000000 vot-toolkit-0.6.2/vot_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       48 2023-05-16 14:36:57.000000 vot-toolkit-0.6.2/vot_toolkit.egg-info/entry_points.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2023-05-16 14:36:57.000000 vot-toolkit-0.6.2/vot_toolkit.egg-info/requires.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        4 2023-05-16 14:36:57.000000 vot-toolkit-0.6.2/vot_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.533292 vot-toolkit-0.6.4/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      211 2022-03-25 11:28:05.000000 vot-toolkit-0.6.4/MANIFEST.in
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3769 2023-05-31 07:41:25.533292 vot-toolkit-0.6.4/PKG-INFO
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2823 2023-05-31 07:22:20.000000 vot-toolkit-0.6.4/README.md
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      295 2023-05-31 07:14:15.000000 vot-toolkit-0.6.4/requirements.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       38 2023-05-31 07:41:25.533292 vot-toolkit-0.6.4/setup.cfg
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1427 2023-05-09 11:09:24.000000 vot-toolkit-0.6.4/setup.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.501293 vot-toolkit-0.6.4/vot/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3368 2023-05-25 09:52:52.000000 vot-toolkit-0.6.4/vot/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      254 2023-05-20 18:58:54.000000 vot-toolkit-0.6.4/vot/__main__.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.501293 vot-toolkit-0.6.4/vot/analysis/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    24213 2023-05-22 14:54:27.000000 vot-toolkit-0.6.4/vot/analysis/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    11736 2023-05-19 09:42:24.000000 vot-toolkit-0.6.4/vot/analysis/accuracy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3878 2023-05-29 15:05:06.000000 vot-toolkit-0.6.4/vot/analysis/failures.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    26037 2023-05-19 11:07:21.000000 vot-toolkit-0.6.4/vot/analysis/longterm.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    17278 2023-05-29 15:05:26.000000 vot-toolkit-0.6.4/vot/analysis/multistart.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    30789 2023-05-19 11:11:46.000000 vot-toolkit-0.6.4/vot/analysis/processor.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    13994 2023-05-19 11:09:41.000000 vot-toolkit-0.6.4/vot/analysis/supervised.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.505293 vot-toolkit-0.6.4/vot/dataset/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    38943 2023-05-30 13:49:40.000000 vot-toolkit-0.6.4/vot/dataset/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    11781 2023-05-30 15:42:52.000000 vot-toolkit-0.6.4/vot/dataset/common.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14672 2020-12-04 15:25:26.000000 vot-toolkit-0.6.4/vot/dataset/cow.png
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3545 2023-05-30 11:19:19.000000 vot-toolkit-0.6.4/vot/dataset/dummy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4216 2023-05-30 13:47:46.000000 vot-toolkit-0.6.4/vot/dataset/got10k.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    11337 2023-05-30 10:50:38.000000 vot-toolkit-0.6.4/vot/dataset/otb.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12655 2023-05-30 11:11:21.000000 vot-toolkit-0.6.4/vot/dataset/proxy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3917 2023-05-30 13:50:11.000000 vot-toolkit-0.6.4/vot/dataset/trackingnet.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.509292 vot-toolkit-0.6.4/vot/document/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16066 2023-05-30 14:50:52.000000 vot-toolkit-0.6.4/vot/document/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      465 2020-12-04 15:25:26.000000 vot-toolkit-0.6.4/vot/document/commands.tex
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6115 2023-05-19 11:23:17.000000 vot-toolkit-0.6.4/vot/document/common.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5950 2023-05-19 11:31:01.000000 vot-toolkit-0.6.4/vot/document/html.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    89476 2020-12-04 15:25:26.000000 vot-toolkit-0.6.4/vot/document/jquery.js
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6911 2023-05-19 11:31:15.000000 vot-toolkit-0.6.4/vot/document/latex.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16184 2020-12-04 15:25:26.000000 vot-toolkit-0.6.4/vot/document/pure.css
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      647 2020-12-04 15:25:26.000000 vot-toolkit-0.6.4/vot/document/report.css
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1212 2020-12-04 15:25:26.000000 vot-toolkit-0.6.4/vot/document/report.js
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9933 2020-12-04 15:25:26.000000 vot-toolkit-0.6.4/vot/document/table.js
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        0 2022-03-23 08:48:42.000000 vot-toolkit-0.6.4/vot/document/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.509292 vot-toolkit-0.6.4/vot/experiment/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    13067 2023-05-31 07:39:21.000000 vot-toolkit-0.6.4/vot/experiment/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1702 2023-05-20 19:07:07.000000 vot-toolkit-0.6.4/vot/experiment/helpers.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10048 2023-05-30 15:28:37.000000 vot-toolkit-0.6.4/vot/experiment/multirun.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4945 2023-05-29 15:08:02.000000 vot-toolkit-0.6.4/vot/experiment/multistart.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4567 2023-05-29 15:08:15.000000 vot-toolkit-0.6.4/vot/experiment/transformer.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.509292 vot-toolkit-0.6.4/vot/region/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3728 2023-05-20 18:47:22.000000 vot-toolkit-0.6.4/vot/region/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10387 2023-05-30 15:43:52.000000 vot-toolkit-0.6.4/vot/region/io.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14049 2023-05-20 18:36:18.000000 vot-toolkit-0.6.4/vot/region/raster.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16612 2023-05-25 09:54:33.000000 vot-toolkit-0.6.4/vot/region/shapes.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3706 2023-05-20 18:08:57.000000 vot-toolkit-0.6.4/vot/region/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.513292 vot-toolkit-0.6.4/vot/stack/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4320 2023-05-20 10:50:01.000000 vot-toolkit-0.6.4/vot/stack/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      249 2023-05-30 10:06:51.000000 vot-toolkit-0.6.4/vot/stack/otb100.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      247 2023-05-30 10:06:43.000000 vot-toolkit-0.6.4/vot/stack/otb50.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.517292 vot-toolkit-0.6.4/vot/stack/tests/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      184 2023-05-30 11:25:27.000000 vot-toolkit-0.6.4/vot/stack/tests/basic.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      541 2023-05-16 13:31:56.000000 vot-toolkit-0.6.4/vot/stack/tests/multiobject.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      638 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/tests/segmentation.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      969 2023-05-20 10:42:49.000000 vot-toolkit-0.6.4/vot/stack/tests.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      351 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2013.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      374 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2014.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.517292 vot-toolkit-0.6.4/vot/stack/vot2015/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      405 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2015/rgb.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      322 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2015/tir.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.517292 vot-toolkit-0.6.4/vot/stack/vot2016/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      540 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2016/rgb.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2016/tir.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      856 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2017.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.517292 vot-toolkit-0.6.4/vot/stack/vot2018/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2018/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      791 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2018/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.521292 vot-toolkit-0.6.4/vot/stack/vot2019/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2019/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2019/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2019/rgbtir.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      789 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2019/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.521292 vot-toolkit-0.6.4/vot/stack/vot2020/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2020/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2020/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2020/rgbtir.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2020/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.521292 vot-toolkit-0.6.4/vot/stack/vot2021/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2021/lt.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2021/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2021/st.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.525292 vot-toolkit-0.6.4/vot/stack/vot2022/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      422 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2022/depth.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      482 2022-03-25 11:28:05.000000 vot-toolkit-0.6.4/vot/stack/vot2022/lt.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      424 2022-03-25 11:28:05.000000 vot-toolkit-0.6.4/vot/stack/vot2022/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2022-03-25 11:28:05.000000 vot-toolkit-0.6.4/vot/stack/vot2022/stb.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2022-03-25 11:28:05.000000 vot-toolkit-0.6.4/vot/stack/vot2022/sts.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      193 2023-05-10 17:51:17.000000 vot-toolkit-0.6.4/vot/stack/vots2023.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.525292 vot-toolkit-0.6.4/vot/tracker/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    33330 2023-05-30 13:51:34.000000 vot-toolkit-0.6.4/vot/tracker/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      808 2023-05-20 10:05:10.000000 vot-toolkit-0.6.4/vot/tracker/dummy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9243 2023-05-20 10:44:10.000000 vot-toolkit-0.6.4/vot/tracker/results.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      631 2023-05-30 11:22:50.000000 vot-toolkit-0.6.4/vot/tracker/tests.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    29316 2023-05-20 10:43:30.000000 vot-toolkit-0.6.4/vot/tracker/trax.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.529292 vot-toolkit-0.6.4/vot/utilities/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    18320 2023-05-30 15:21:21.000000 vot-toolkit-0.6.4/vot/utilities/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    17701 2023-05-30 11:19:42.000000 vot-toolkit-0.6.4/vot/utilities/cli.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5740 2023-05-20 10:01:49.000000 vot-toolkit-0.6.4/vot/utilities/data.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10476 2023-05-19 11:41:40.000000 vot-toolkit-0.6.4/vot/utilities/draw.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4351 2023-05-20 09:57:10.000000 vot-toolkit-0.6.4/vot/utilities/migration.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7113 2023-05-20 10:02:38.000000 vot-toolkit-0.6.4/vot/utilities/net.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10059 2023-05-29 15:09:15.000000 vot-toolkit-0.6.4/vot/utilities/notebook.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       45 2023-05-29 11:34:41.000000 vot-toolkit-0.6.4/vot/version.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.529292 vot-toolkit-0.6.4/vot/workspace/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7526 2023-05-20 18:57:16.000000 vot-toolkit-0.6.4/vot/workspace/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    13864 2023-05-20 18:55:39.000000 vot-toolkit-0.6.4/vot/workspace/storage.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1840 2023-05-20 18:48:56.000000 vot-toolkit-0.6.4/vot/workspace/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.533292 vot-toolkit-0.6.4/vot_toolkit.egg-info/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3769 2023-05-31 07:41:25.000000 vot-toolkit-0.6.4/vot_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2411 2023-05-31 07:41:25.000000 vot-toolkit-0.6.4/vot_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        1 2023-05-31 07:41:25.000000 vot-toolkit-0.6.4/vot_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       48 2023-05-31 07:41:25.000000 vot-toolkit-0.6.4/vot_toolkit.egg-info/entry_points.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2023-05-31 07:41:25.000000 vot-toolkit-0.6.4/vot_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        4 2023-05-31 07:41:25.000000 vot-toolkit-0.6.4/vot_toolkit.egg-info/top_level.txt
```

### Comparing `vot-toolkit-0.6.2/PKG-INFO` & `vot-toolkit-0.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: vot-toolkit
-Version: 0.6.2
+Version: 0.6.4
 Summary: Perform visual object tracking experiments and analyze results
 Home-page: https://github.com/votchallenge/toolkit
 Author: Luka Cehovin Zajc
 Author-email: luka.cehovin@gmail.com
 License: UNKNOWN
 Description: 
         The VOT evaluation toolkit
         ==========================
         
+        [![PyPI package version](https://badge.fury.io/py/vot-toolkit.svg)](https://badge.fury.io/py/vot-toolkit)
+        
         This repository contains the official evaluation toolkit for the [Visual Object Tracking (VOT) challenge](http://votchallenge.net/). This is the official version of the toolkit, implemented in Python 3 language. If you are looking for the old Matlab version, you can find an archived repository [here](https://github.com/votchallenge/toolkit-legacy).
         
         For more detailed informations consult the documentation available in the source or a compiled version of the documentation [here](http://www.votchallenge.net/howto/). You can also subscribe to the VOT [mailing list](https://liste.arnes.si/mailman3/lists/votchallenge.lists.arnes.si/) to receive news about challenges and important software updates or join our [support form](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help) to ask questions.
         
         Developers
         ----------
```

### Comparing `vot-toolkit-0.6.2/README.md` & `vot-toolkit-0.6.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
 The VOT evaluation toolkit
 ==========================
 
+[![PyPI package version](https://badge.fury.io/py/vot-toolkit.svg)](https://badge.fury.io/py/vot-toolkit)
+
 This repository contains the official evaluation toolkit for the [Visual Object Tracking (VOT) challenge](http://votchallenge.net/). This is the official version of the toolkit, implemented in Python 3 language. If you are looking for the old Matlab version, you can find an archived repository [here](https://github.com/votchallenge/toolkit-legacy).
 
 For more detailed informations consult the documentation available in the source or a compiled version of the documentation [here](http://www.votchallenge.net/howto/). You can also subscribe to the VOT [mailing list](https://liste.arnes.si/mailman3/lists/votchallenge.lists.arnes.si/) to receive news about challenges and important software updates or join our [support form](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help) to ask questions.
 
 Developers
 ----------
```

### Comparing `vot-toolkit-0.6.2/setup.py` & `vot-toolkit-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.2/vot/analysis/__init__.py` & `vot-toolkit-0.6.4/vot/analysis/multistart.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,443 +1,439 @@
-import logging
-import functools
-import threading
-from collections import namedtuple
-from enum import Enum, Flag, auto
-from typing import List, Optional, Tuple, Dict, Any, Set, Union, NamedTuple
-from abc import ABC, abstractmethod
-from concurrent.futures import Executor
-import importlib
+"""This module contains the implementation of the accuracy-robustness analysis and EAO analysis for the multistart experiment."""
 
-from cachetools import Cache
-from class_registry import ClassRegistry
+from typing import List, Tuple, Any
 
-from attributee import Attributee, String
+import numpy as np
 
-from vot import ToolkitException
-from vot.tracker import Tracker
+from attributee import Integer, Boolean, Float, Include
+
+from vot.tracker import Tracker, Trajectory
 from vot.dataset import Sequence
+from vot.dataset.proxy import FrameMapSequence
 from vot.experiment import Experiment
-from vot.region import Region, RegionType
-from vot.utilities import class_fullname, arg_hash
+from vot.experiment.multistart import MultiStartExperiment, find_anchors
+from vot.region import calculate_overlaps
+from vot.analysis import MissingResultsException, Measure, Plot, Analysis, Axes, \
+    Sorting, SeparableAnalysis, Curve, Point, analysis_registry, SequenceAggregator
 from vot.utilities.data import Grid
 
-analysis_registry = ClassRegistry("vot_analysis")
-
-class MissingResultsException(ToolkitException):
-    """Exception class that denotes missing results during analysis
-    """
-    def __init__(self, *args: object) -> None:
-        if not args:
-            args = ["Missing results"]
-        super().__init__(*args)
+def compute_eao_partial(overlaps: List, success: List[bool], curve_length: int):
+    """Compute the EAO curve for a single sequence. The curve is computed as the average overlap at each frame.
+    
+    Args:
+        overlaps (List): List of overlaps for each frame.
+        success (List[bool]): List of success flags for each frame.
+        curve_length (int): Length of the curve.
         
-class Sorting(Enum):
-    """Sorting direction enumeration class
+    Returns:
+        List[float]: EAO curve.
     """
-    UNSORTABLE = auto()
-    DESCENDING = auto()
-    ASCENDING = auto()
+    phi = curve_length * [float(0)]
+    active = curve_length * [float(0)]
 
-class Axes(Enum):
-    """Semantic information for axis in analysis grid
-    """
-    NONE = auto()
-    TRACKERS = auto()
-    SEQUENCES = auto()
-    BOTH = auto()
+    for o, success in zip(overlaps, success):
 
-class Result(ABC):
-    """Abstract result object base. This is the base class for all result descriptions.
-    """
+        o_array = np.array(o)
 
-    def __init__(self, name: str, abbreviation: Optional[str] = None, description: Optional["str"] = ""):
-        """Constructor
+        for j in range(1, curve_length):
 
-        Arguments:
-            name {str} -- Name of the result, used in reports
+            if j < len(o):
+                phi[j] += np.mean(o_array[1:j+1])
+                active[j] += 1
+            elif not success:
+                phi[j] += np.sum(o_array[1:len(o)]) / (j - 1)
+                active[j] += 1
 
-        Keyword Arguments:
-            abbreviation {Optional[str]} -- Abbreviation, if empty, then name is used. 
-            Can be used to define a shorter text representation. (default: {None})
-        """
-        self._name = name
-        if abbreviation is None:
-            self._abbreviation = name
-        else:
-            self._abbreviation = abbreviation
+    phi = [p / a if a > 0 else 0 for p, a in zip(phi, active)]
+    return phi, active
 
-        self._description = description
 
-    @property
-    def name(self) -> str:
-        return self._name
+@analysis_registry.register("multistart_ar")
+class AccuracyRobustness(SeparableAnalysis):
+    """This analysis computes the accuracy-robustness curve for the multistart experiment."""
 
-    @property
-    def abbreviation(self) -> str:
-        return self._abbreviation
+    burnin = Integer(default=10, val_min=0)
+    grace = Integer(default=10, val_min=0)
+    bounded = Boolean(default=True)
+    threshold = Float(default=0.1, val_min=0, val_max=1)
 
     @property
-    def description(self) -> str:
-        return self._description
+    def _title_default(self):
+        """Title of the analysis."""
+        return "AR Analysis"
 
-class Label(Result):
+    def describe(self):
+        """Return the description of the analysis."""
+        return Measure("Accuracy", "A", minimal=0, maximal=1, direction=Sorting.DESCENDING), \
+             Measure("Robustness", "R", minimal=0, direction=Sorting.DESCENDING), \
+             Point("AR plot", dimensions=2, abbreviation="AR",
+                minimal=(0, 0), maximal=(1, 1), labels=("Robustness", "Accuracy"), trait="ar"), \
+             None, None
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def compatible(self, experiment: Experiment):
+        """Check if the experiment is compatible with the analysis. The experiment must be a multistart experiment."""
+        return isinstance(experiment, MultiStartExperiment)
 
-class Measure(Result):
-    """Measure describes a single value numerical output of an analysis. Can have minimum and maximum value as well
-    as direction of sorting.
-    """
+    def subcompute(self, experiment: Experiment, tracker: Tracker, sequence: Sequence, dependencies: List[Grid]) -> Tuple[Any]:
+        """Compute the accuracy-robustness for each sequence.
+        
+        Args:
+            experiment (Experiment): Experiment.
+            tracker (Tracker): Tracker.
+            sequence (Sequence): Sequence.
+            dependencies (List[Grid]): List of dependencies.
+            
+        Returns:
+            Tuple[Any]: Accuracy, robustness, AR curve, robustness, length of the sequence.
+        """
 
-    def __init__(self, name: str, abbreviation: Optional[str] = None, minimal: Optional[float] = None, \
-        maximal: Optional[float] = None, direction: Optional[Sorting] = Sorting.UNSORTABLE):
+        results = experiment.results(tracker, sequence)
 
-        super().__init__(name, abbreviation)
-        self._minimal = minimal
-        self._maximal = maximal
-        self._direction = direction
+        forward, backward = find_anchors(sequence, experiment.anchor)
 
-    @property
-    def minimal(self) -> float:
-        return self._minimal
+        if not forward and not backward:
+            raise RuntimeError("Sequence does not contain any anchors")
 
-    @property
-    def maximal(self) -> float:
-        return self._maximal
+        robustness = 0
+        accuracy = 0
+        total = 0
+        for i, reverse in [(f, False) for f in forward] + [(f, True) for f in backward]:
+            name = "%s_%08d" % (sequence.name, i)
 
-    @property
-    def direction(self) -> Sorting:
-        return self._direction
+            if not Trajectory.exists(results, name):
+                raise MissingResultsException()
 
-class Drawable(Result):
-    """Base class for results that can be visualized in plots.
-    """
+            if reverse:
+                proxy = FrameMapSequence(sequence, list(reversed(range(0, i + 1))))
+            else:
+                proxy = FrameMapSequence(sequence, list(range(i, len(sequence))))
 
-    def __init__(self, name: str, abbreviation: Optional[str] = None, trait: Optional[str] = None):
-        """[summary]
+            trajectory = Trajectory.read(results, name)
 
-        Args:
-            name (str): [description]
-            abbreviation (Optional[str], optional): [description]. Defaults to None.
-            trait (Optional[str], optional): Trait of the data, used for specification . Defaults to None.
-        """
-        super().__init__(name, abbreviation)
-        self._trait = trait
+            overlaps = calculate_overlaps(trajectory.regions(), proxy.groundtruth(), (proxy.size) if self.burnin else None)
 
-    @property
-    def trait(self):
-        return self._trait
+            grace = self.grace
+            progress = len(proxy)
 
-class Multidimensional(Drawable):
-    def __init__(self, name: str, dimensions: int, abbreviation: Optional[str] = None, minimal: Optional[Tuple[float]] = None, \
-        maximal: Optional[Tuple[float]] = None, labels: Optional[Tuple[str]] = None, trait: Optional[str] = None):
-        assert(dimensions > 1)
-        super().__init__(name, abbreviation, trait)
-        self._dimensions = dimensions
-        self._minimal = minimal
-        self._maximal = maximal
-        self._labels = labels
+            for j, overlap in enumerate(overlaps):
+                if overlap <= self.threshold and not proxy.groundtruth(j).is_empty():
+                    grace = grace - 1
+                    if grace == 0:
+                        progress = j + 1 - self.grace  # subtract since we need actual point of the failure
+                        break
+                else:
+                    grace = self.grace
 
-    @property
-    def dimensions(self):
-        return self._dimensions
+            robustness += progress  # simplified original equation: len(proxy) * (progress / len(proxy))
+            accuracy += sum(overlaps[0:progress])
+            total += len(proxy)
 
-    def minimal(self, i):
-        return self._minimal[i]
+        ar = (robustness / total, accuracy / robustness if robustness > 0 else 0)
 
-    def maximal(self, i):
-        return self._maximal[i]
+        return accuracy / robustness if robustness > 0 else 0, robustness / total, ar, robustness, len(sequence)
 
-    def label(self, i):
-        return self._labels[i]
+@analysis_registry.register("multistart_average_ar")
+class AverageAccuracyRobustness(SequenceAggregator):
+    """This analysis computes the average accuracy-robustness curve for the multistart experiment."""
 
-class Point(Multidimensional):
-    """Point is a two or more dimensional numerical output that can be visualized in a scatter plot.
-    """
+    analysis = Include(AccuracyRobustness)
 
-class Plot(Drawable):
-    """Plot describes a result in form of a list of values with optional minimum and maximum with respect to some unit. The
-    results of the same analysis for different trackers should have the same number of measurements (independent variable).
-    """
+    @property
+    def _title_default(self):
+        """Title of the analysis."""
+        return "AR Analysis"
 
-    def __init__(self, name: str, abbreviation: Optional[str] = None, wrt: str = "frames", minimal: Optional[float] = None, \
-        maximal: Optional[float] = None, trait: Optional[str] = None):
-        super().__init__(name, abbreviation, trait)
-        self._wrt = wrt
-        self._minimal = minimal
-        self._maximal = maximal
+    def dependencies(self):
+        """Return the dependencies of the analysis."""
+        return self.analysis, 
 
-    @property
-    def minimal(self):
-        return self._minimal
+    def describe(self):
+        """Return the description of the analysis."""
+        return Measure("Accuracy", "A", minimal=0, maximal=1, direction=Sorting.DESCENDING), \
+             Measure("Robustness", "R", minimal=0, direction=Sorting.DESCENDING), \
+             Point("AR plot", dimensions=2, abbreviation="AR",
+                minimal=(0, 0), maximal=(1, 1), labels=("Robustness", "Accuracy"), trait="ar"), \
+             None, None
 
-    @property
-    def maximal(self):
-        return self._maximal
+    def compatible(self, experiment: Experiment):
+        """Check if the experiment is compatible with the analysis. The experiment must be a multistart experiment."""
+        return isinstance(experiment, MultiStartExperiment)
 
+    def aggregate(self, tracker: Tracker, sequences: List[Sequence], results: Grid):
+        """Aggregate the results of the analysis.
+        
+        Args:
+            tracker (Tracker): Tracker.
+            sequences (List[Sequence]): List of sequences.
+            results (Grid): Grid of results.
+            
+        Returns:
+            Tuple[Any]: Aggregated results.
+        """
+        total_accuracy = 0
+        total_robustness = 0
+        weight_accuracy = 0
+        weight_robustness = 0
+
+        for accuracy, robustness, _, accuracy_w, robustness_w in results:
+            total_accuracy += accuracy * accuracy_w
+            total_robustness += robustness * robustness_w
+            weight_accuracy += accuracy_w
+            weight_robustness += robustness_w
+
+        ar = (total_robustness / weight_robustness, total_accuracy / weight_accuracy)
+
+        return total_accuracy / weight_accuracy, total_robustness / weight_robustness, ar, weight_accuracy, weight_robustness
+
+@analysis_registry.register("multistart_fragments")
+class MultiStartFragments(SeparableAnalysis):
+    """This analysis computes the accuracy-robustness curve for the multistart experiment."""
+
+    burnin = Integer(default=10, val_min=0)
+    grace = Integer(default=10, val_min=0)
+    bounded = Boolean(default=True)
+    threshold = Float(default=0.1, val_min=0, val_max=1)
+
+    @property
+    def _title_default(self):
+        """Title of the analysis."""
+        return "Fragment Analysis"
+
+    def describe(self):
+        """Return the description of the analysis."""
+        return Curve("Success", 2, "Sc", minimal=(0, 0), maximal=(1,1), trait="points"), Curve("Accuracy", 2, "Ac", minimal=(0, 0), maximal=(1,1), trait="points")
 
-    @property
-    def wrt(self):
-        return self._wrt
+    def compatible(self, experiment: Experiment):
+        """Check if the experiment is compatible with the analysis. The experiment must be a multistart experiment."""
+        return isinstance(experiment, MultiStartExperiment)
 
-class Curve(Multidimensional):
-    """Curve is a list of 2+ dimensional results. The number of elements in a list can vary between samples.
-    """
+    def subcompute(self, experiment: Experiment, tracker: Tracker, sequence: Sequence, dependencies: List[Grid]) -> Tuple[Any]:
+        """Compute the analysis for a single sequence. The sequence must contain at least one anchor.
+        
+        Args:
+            experiment (Experiment): Experiment.
+            tracker (Tracker): Tracker.
+            sequence (Sequence): Sequence.
+            dependencies (List[Grid]): List of dependencies.
+            
+        Returns:
+            Tuple[Any]: Results of the analysis."""
 
-class Analysis(Attributee):
+        results = experiment.results(tracker, sequence)
 
-    name = String(default=None)
+        forward, backward = find_anchors(sequence, experiment.anchor)
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self._identifier_cache = None
+        if not forward and not backward:
+            raise RuntimeError("Sequence does not contain any anchors")
 
-    def compatible(self, experiment: Experiment):
-        raise NotImplementedError()
+        accuracy = []
+        success = []
 
-    @property
-    def title(self) -> str:
-        if self.name is None:
-            return self._title_default
-        else:
-            return self.name
+        for i, reverse in [(f, False) for f in forward] + [(f, True) for f in backward]:
+            name = "%s_%08d" % (sequence.name, i)
 
-    @property
-    def _title_default(self) -> str:
-        raise NotImplementedError()
+            if not Trajectory.exists(results, name):
+                raise MissingResultsException()
 
-    def dependencies(self) -> List["Analysis"]:
-        return []
+            if reverse:
+                proxy = FrameMapSequence(sequence, list(reversed(range(0, i + 1))))
+            else:
+                proxy = FrameMapSequence(sequence, list(range(i, len(sequence))))
 
-    @property
-    def identifier(self) -> str:
-        if not self._identifier_cache is None:
-            return self._identifier_cache
+            trajectory = Trajectory.read(results, name)
 
-        params = self.dump()
-        del params["name"]
+            overlaps = calculate_overlaps(trajectory.regions(), proxy.groundtruth(), (proxy.size) if self.burnin else None)
 
-        confighash = arg_hash(**params)
+            grace = self.grace
+            progress = len(proxy)
 
-        self._identifier_cache = class_fullname(self) + "@" + confighash
-        
-        return self._identifier_cache
+            for j, overlap in enumerate(overlaps):
+                if overlap <= self.threshold and not proxy.groundtruth(j).is_empty():
+                    grace = grace - 1
+                    if grace == 0:
+                        progress = j + 1 - self.grace  # subtract since we need actual point of the failure
+                        break
+                else:
+                    grace = self.grace
 
-    def describe(self) -> Tuple["Result"]:
-        """Returns a tuple of descriptions of results
-        """
-        raise NotImplementedError()
+            success.append( (i / len(sequence), progress / len(proxy)))
+            accuracy.append( (i / len(sequence), sum(overlaps[0:progress] / len(proxy))))
 
-    def compute(self, experiment: Experiment, trackers: List[Tracker], sequences: List[Sequence], dependencies: List[Grid]) -> Grid:
-        raise NotImplementedError()
+        return success, accuracy
 
-    @property
-    def axes(self) -> Axes:
-        """ Returns axes semantic description for the result grid """
-        raise NotImplementedError()
-
-    def commit(self, experiment: Experiment, trackers: List[Tracker], sequences: List[Sequence]):
-        return AnalysisProcessor.commit_default(self, experiment, trackers, sequences)
-
-    def run(self, experiment: Experiment, trackers: List[Tracker], sequences: List[Sequence]):
-        return AnalysisProcessor.run_default(self, experiment, trackers, sequences)
-
-class SeparableAnalysis(Analysis):
-    """Analysis that is separable with respect to trackers and/or sequences, each part can be processed in parallel
-    as a separate job. The separation is determined by the result of the axes() method: Axes.BOTH means separation
-    in tracker-sequence pairs, Axes.TRACKER means separation according to  
-    """
+# TODO: remove high
+@analysis_registry.register("multistart_eao_curves")
+class EAOCurves(SeparableAnalysis):
+    """This analysis computes the expected average overlap curve for the multistart experiment."""
 
-    SeparablePart = namedtuple("SeparablePart", ["trackers", "sequences", "tid", "sid"])
+    burnin = Integer(default=10, val_min=0)
+    grace = Integer(default=10, val_min=0)
+    bounded = Boolean(default=True)
+    threshold = Float(default=0.1, val_min=0, val_max=1)
 
-    @abstractmethod
-    def subcompute(self, experiment: Experiment, tracker, sequence, dependencies: List[Grid]) -> Tuple[Any]:
-        """This method is called for every part of the analysis.
+    high = Integer()
 
-        Args:
-            experiment (Experiment): [description]
-            tracker ([type]): [description]
-            sequence ([type]): [description]
-            dependencies (List[Grid]): Dependencies of the analysis, 
-                note that each dependency is processed using select function to only contain 
-                information relevant for the current part of the analysis
+    @property
+    def _title_default(self):
+        """Title of the analysis."""
+        return "EAO Curve"
 
-        Raises:
-            NotImplementedError: [description]
+    def describe(self):
+        """Return the description of the analysis."""
+        return Plot("Expected average overlap", "EAO", minimal=0, maximal=1, wrt="frames", trait="eao"),
 
+    def compatible(self, experiment: Experiment):
+        """Check if the experiment is compatible with the analysis. The experiment must be a multistart experiment."""
+        return isinstance(experiment, MultiStartExperiment)
+
+    def subcompute(self, experiment: Experiment, tracker: Tracker, sequence: Sequence, dependencies: List[Grid]) -> Tuple[Any]:
+        """Compute the analysis for a single sequence. The sequence must contain at least one anchor.
+        
+        Args:
+            experiment (Experiment): Experiment.
+            tracker (Tracker): Tracker.
+            sequence (Sequence): Sequence.
+            dependencies (List[Grid]): List of dependencies.
+            
         Returns:
-            Tuple[Any]: [description]
+            Tuple[Any]: Results of the analysis.
         """
-        raise NotImplementedError()
+        
+        results = experiment.results(tracker, sequence)
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+        forward, backward = find_anchors(sequence, experiment.anchor)
 
-        # All dependencies should be mappable to individual parts. If parts contain 
-        # separation only across trackers or sequences then we are unable to properly
-        # assign dependencies that contain individual 
-        if self.axes != Axes.BOTH:
-            assert all([dependency.axes != Axes.BOTH for dependency in self.dependencies()])
-
-    def separate(self, trackers: List[Tracker], sequences: List[Sequence]) -> List["SeparablePart"]:
-        if self.axes == Axes.BOTH:
-            parts = []
-            for i, tracker in enumerate(trackers):
-                for j, sequence in enumerate(sequences):
-                    parts.append(SeparableAnalysis.SeparablePart([tracker], [sequence], i, j))
-            return parts
-        elif self.axes == Axes.TRACKERS:
-            parts = []
-            for i, tracker in enumerate(trackers):
-                parts.append(SeparableAnalysis.SeparablePart([tracker], sequences, i, None))
-            return parts
-        elif self.axes == Axes.SEQUENCES:
-            parts = []
-            for j, sequence in enumerate(sequences):
-                parts.append(SeparableAnalysis.SeparablePart(trackers, [sequence], None, j))
-            return parts
-
-    def join(self, trackers: List[Tracker], sequences: List[Sequence], results: List[Tuple[Any]]):
-        if self.axes == Axes.BOTH:
-            transformed_results = Grid(len(trackers), len(sequences))
-            k = 0
-            for i, _ in enumerate(trackers):
-                for j, _ in enumerate(sequences):
-                    transformed_results[i, j] = results[k][0,0]
-                    k += 1
-            return transformed_results
-        elif self.axes == Axes.TRACKERS:
-            transformed_results = Grid(len(trackers), 1)
-            k = 0
-            for i, _ in enumerate(trackers):
-                transformed_results[i, 0] = results[k][0,0]
-                k += 1
-            return transformed_results
-        elif self.axes == Axes.SEQUENCES:
-            transformed_results = Grid(1, len(sequences))
-            k = 0
-            for i, _ in enumerate(sequences):
-                transformed_results[0, i] = results[k][0,0]
-                k += 1
-            return transformed_results
-
-    @staticmethod
-    def select(meta: Analysis, data: Grid, tracker: int, sequence: int) -> Grid:
-        """Select appropriate subpart of dependency results for the part, used internally by sequential and
-        parallel processor. This method handles propagation across "singleton" dimension. 
-        
-        The idea is that a certain part of the analysis will only require the part of the result corresponding
-        to the tracker and/or sequence that it is processing.
+        if len(forward) == 0 and len(backward) == 0:
+            raise RuntimeError("Sequence does not contain any anchors")
 
-        Args:
-            meta (Analysis): Description of the dependency analysis
-            data (Grid): Returned data of the dependency
-            tracker (int): Index of the tracker required by the part or None
-            sequence (int): Index of the sequence required by the part or None
+        overlaps_all = []
+        success_all = []
 
-        Returns:
-            Grid: Subsection of the result, still in Grid format.
-        """
-        if meta.axes == Axes.BOTH:
-            return data.cell(tracker, sequence)
-        elif meta.axes == Axes.TRACKERS:
-            return data.row(tracker)
-        elif meta.axes == Axes.SEQUENCES:
-            return data.column(sequence)
-        else:
-            return data
+        for i, reverse in [(f, False) for f in forward] + [(f, True) for f in backward]:
+            name = "%s_%08d" % (sequence.name, i)
 
-    def compute(self, experiment: Experiment, trackers: List[Tracker], sequences: List[Sequence], dependencies: List[Grid]) -> Grid:
-        """The blocking non-parallel version of computation that can be called directly. Splits the job in parts and
-        runs them sequentially. For parallel execution use the analysis processor.
+            if not Trajectory.exists(results, name):
+                raise MissingResultsException()
 
-        Args:
-            experiment (Experiment): Experiment from which to take results
-            trackers (List[Tracker]): Trackers to run analysis on
-            sequences (List[Sequence]): Sequences to run analysis on
-            dependencies (List[Grid]): Results from depndencies, if you override the class and add dependencies, you also
-            have to override this function and handle them.
+            if reverse:
+                proxy = FrameMapSequence(sequence, list(reversed(range(0, i + 1))))
+            else:
+                proxy = FrameMapSequence(sequence, list(range(i, len(sequence))))
 
-        Returns:
-            Grid: Results in a data grid object
-        """
+            trajectory = Trajectory.read(results, name)
+
+            overlaps = calculate_overlaps(trajectory.regions(), proxy.groundtruth(), proxy.size if self.burnin else None)
+
+            grace = self.grace
+            progress = len(proxy)
+
+            for j, overlap in enumerate(overlaps):
+                if overlap <= self.threshold and not proxy.groundtruth(j).is_empty():
+                    grace = grace - 1
+                    if grace == 0:
+                        progress = j + 1 - self.grace  # subtract since we need actual point of the failure
+                        break
+                else:
+                    grace = self.grace
+
+            success = True
+            if progress < len(overlaps):
+                # tracker has failed during this run
+                overlaps[progress:] = (len(overlaps) - progress) * [float(0)]
+                success = False
 
-        if self.axes == Axes.BOTH and len(trackers) == 1 and len(sequences) == 1:
-            return Grid.scalar(self.subcompute(experiment, trackers[0], sequences[0], dependencies))
-        elif self.axes == Axes.TRACKERS and len(trackers) == 1:
-            return Grid.scalar(self.subcompute(experiment, trackers[0], sequences, dependencies))
-        elif self.axes == Axes.SEQUENCES and len(sequences) == 1:
-            return Grid.scalar(self.subcompute(experiment, trackers, sequences[0], dependencies))
-        else:
-            parts = self.separate(trackers, sequences)
-            results = []
-            for part in parts:
-                partdependencies = [SeparableAnalysis.select(meta, data, part.tid, part.sid) 
-                    for meta, data in zip(self.dependencies(), dependencies)]
-                results.append(self.compute(experiment, part.trackers, part.sequences, partdependencies))
+            overlaps_all.append(overlaps)
+            success_all.append(success)
 
-            return self.join(trackers, sequences, results)
+        return compute_eao_partial(overlaps_all, success_all, self.high), 1
 
+#TODO: remove high
+@analysis_registry.register("multistart_eao_curve")
+class EAOCurve(SequenceAggregator):
+    """This analysis computes the expected average overlap curve for the multistart experiment. It is an aggregator of the curves for individual sequences."""
+
+    curves = Include(EAOCurves)
+    
     @property
-    def axes(self) -> Axes:
-        return Axes.BOTH
+    def _title_default(self):
+        """Title of the analysis."""
+        return "EAO Curve"
+
+    def describe(self):
+        """Return the description of the analysis."""
+        return Plot("Expected average overlap", "EAO", minimal=0, maximal=1, wrt="frames", trait="eao"),
 
-class SequenceAggregator(Analysis): # pylint: disable=W0223
+    def compatible(self, experiment: Experiment):
+        """Check if the experiment is compatible with the analysis. The experiment must be a multistart experiment."""
+        return isinstance(experiment, MultiStartExperiment)
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        # We only support one dependency in aggregator ...
-        assert len(self.dependencies()) == 1
-        # ... it should produce a grid of results that can be averaged over sequences
-        assert self.dependencies()[0].axes == Axes.BOTH
+    def dependencies(self):
+        """Return the dependencies of the analysis."""
+        return self.curves,
 
-    @abstractmethod
     def aggregate(self, tracker: Tracker, sequences: List[Sequence], results: Grid) -> Tuple[Any]:
-        raise NotImplementedError()
+        """Aggregate the results of the analysis for multiple sequences. The sequences must contain at least one anchor.
+        
+        Args:
+            tracker (Tracker): Tracker.
+            sequences (List[Sequence]): List of sequences.
+            results (Grid): Grid of results.
 
-    def compute(self, _: Experiment, trackers: List[Tracker], sequences: List[Sequence], dependencies: List[Grid]) -> Grid:
-        results = dependencies[0]
-        transformed_results = Grid(len(trackers), 1)
+        Returns:
+            Tuple[Any]: Results of the analysis.
+        """
 
-        for i, tracker in enumerate(trackers):
-            transformed_results[i, 0] = self.aggregate(tracker, sequences, results.row(i))
+        eao_curve = self.curves.high * [float(0)]
+        eao_weights = self.curves.high * [float(0)]
 
-        return transformed_results
+        for (seq_eao_curve, eao_active), seq_w in results:
+            for i, (eao_, active_) in enumerate(zip(seq_eao_curve, eao_active)):
+                eao_curve[i] += eao_ * active_ * seq_w
+                eao_weights[i] += active_ * seq_w
 
-    @property
-    def axes(self) -> Axes:
-        return Axes.TRACKERS
+        return [eao_ / w_ if w_ > 0 else 0 for eao_, w_ in zip(eao_curve, eao_weights)],
 
-class TrackerSeparableAnalysis(SeparableAnalysis):
-    """Separate analysis into multiple per-tracker tasks, each of them is non-separable.
-    """
+@analysis_registry.register("multistart_eao_score")
+class EAOScore(Analysis):
+    """This analysis computes the expected average overlap score for the multistart experiment. It does this by computing the EAO curve and then integrating it."""
 
-    @abstractmethod
-    def subcompute(self, experiment: Experiment, tracker: Tracker, sequences: List[Sequence], dependencies: List[Grid]) -> Tuple[Any]:
-        raise NotImplementedError()
+    low = Integer()
+    high = Integer()
+    eaocurve = Include(EAOCurve)
 
     @property
-    def axes(self) -> Axes:
-        return Axes.TRACKERS
+    def _title_default(self):
+        """Title of the analysis."""
+        return "EAO analysis"
 
-class SequenceSeparableAnalysis(SeparableAnalysis):
-    """Separate analysis into multiple per-tracker tasks, each of them is non-separable.
-    """
+    def describe(self):
+        """Return the description of the analysis."""
+        return Measure("Expected average overlap", "EAO", minimal=0, maximal=1, direction=Sorting.DESCENDING),
+
+    def compatible(self, experiment: Experiment):
+        """Check if the experiment is compatible with the analysis. The experiment must be a multistart experiment."""
+        return isinstance(experiment, MultiStartExperiment)
 
-    @abstractmethod
-    def subcompute(self, experiment: Experiment, trackers: List[Tracker], sequence: Sequence, dependencies: List[Grid]) -> Tuple[Any]:
-        raise NotImplementedError
+    def dependencies(self):
+        """Return the dependencies of the analysis."""
+        return self.eaocurve,
+
+    def compute(self, experiment: Experiment, trackers: List[Tracker], sequences: List[Sequence], dependencies: List[Grid]) -> Grid:
+        """Compute the analysis for multiple sequences. The sequences must contain at least one anchor.
+        
+        Args:
+            experiment (Experiment): Experiment.
+            trackers (List[Tracker]): List of trackers.
+            sequences (List[Sequence]): List of sequences.
+            dependencies (List[Grid]): List of dependencies.
+            
+        Returns:
+            Grid: Grid of results.
+        """
+
+        return dependencies[0].foreach(lambda x, i, j: (float(np.mean(x[0][self.low:self.high + 1])), ) )
 
     @property
-    def axes(self) -> Axes:
-        return Axes.SEQUENCES
+    def axes(self):
+        """Return the axes of the analysis."""
+        return Axes.TRACKERS
 
-def is_special(region: Region, code=None) -> bool:
-    if code is None:
-        return region.type == RegionType.SPECIAL
-    return region.type == RegionType.SPECIAL and region.code == code
-
-from ._processor import process_stack_analyses, AnalysisProcessor, AnalysisError
-for module in [".multistart", ".supervised", ".accuracy", ".failures", ".longterm"]:
-    importlib.import_module(module, package="vot.analysis")
```

### Comparing `vot-toolkit-0.6.2/vot/analysis/multistart.py` & `vot-toolkit-0.6.4/vot/analysis/accuracy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,337 +1,291 @@
-import math
+"""Accuracy analysis. Computes average overlap between predicted and groundtruth regions."""
+
 from typing import List, Tuple, Any
 
 import numpy as np
 
-from attributee import Integer, Boolean, Float, Include
+from attributee import Boolean, Integer, Include, Float
 
-from vot.tracker import Tracker, Trajectory
+from vot.analysis import (Measure,
+                          MissingResultsException,
+                          SequenceAggregator, Sorting,
+                          is_special, SeparableAnalysis,
+                          analysis_registry, Curve)
 from vot.dataset import Sequence
-from vot.dataset.proxy import FrameMapSequence
 from vot.experiment import Experiment
-from vot.experiment.multistart import MultiStartExperiment, find_anchors
-from vot.region import calculate_overlaps
-from vot.analysis import MissingResultsException, Measure, Plot, Analysis, Axes, \
-    Sorting, SeparableAnalysis, Curve, Point, analysis_registry, SequenceAggregator
+from vot.experiment.multirun import (MultiRunExperiment)
+from vot.region import Region, calculate_overlaps
+from vot.tracker import Tracker, Trajectory
 from vot.utilities.data import Grid
 
-def compute_eao_partial(overlaps: List, success: List[bool], curve_length: int):
-    phi = curve_length * [float(0)]
-    active = curve_length * [float(0)]
-
-    for o, success in zip(overlaps, success):
-
-        o_array = np.array(o)
-
-        for j in range(1, curve_length):
-
-            if j < len(o):
-                phi[j] += np.mean(o_array[1:j+1])
-                active[j] += 1
-            elif not success:
-                phi[j] += np.sum(o_array[1:len(o)]) / (j - 1)
-                active[j] += 1
-
-    phi = [p / a if a > 0 else 0 for p, a in zip(phi, active)]
-    return phi, active
-
-
-@analysis_registry.register("multistart_ar")
-class AccuracyRobustness(SeparableAnalysis):
+def gather_overlaps(trajectory: List[Region], groundtruth: List[Region], burnin: int = 10, 
+    ignore_unknown: bool = True, ignore_invisible: bool = False, bounds = None, threshold: float = None) -> np.ndarray:
+    """Gather overlaps between trajectory and groundtruth regions. 
+    
+    Args:
+        trajectory (List[Region]): List of regions predicted by the tracker.
+        groundtruth (List[Region]): List of groundtruth regions.
+        burnin (int, optional): Number of frames to skip at the beginning of the sequence. Defaults to 10.
+        ignore_unknown (bool, optional): Ignore unknown regions in the groundtruth. Defaults to True.
+        ignore_invisible (bool, optional): Ignore invisible regions in the groundtruth. Defaults to False.
+        bounds ([type], optional): Bounds of the sequence. Defaults to None.
+        threshold (float, optional): Minimum overlap to consider. Defaults to None.
+        
+    Returns:
+        np.ndarray: List of overlaps."""
+
+    overlaps = np.array(calculate_overlaps(trajectory, groundtruth, bounds))
+    mask = np.ones(len(overlaps), dtype=bool)
+
+    if threshold is None: threshold = -1
+
+    for i, (region_tr, region_gt) in enumerate(zip(trajectory, groundtruth)):
+        # Skip if groundtruth is unknown
+        if is_special(region_gt, Sequence.UNKNOWN):
+            mask[i] = False
+        elif ignore_invisible and region_gt.is_empty():
+            mask[i] = False
+        # Skip if predicted is unknown
+        elif is_special(region_tr, Trajectory.UNKNOWN) and ignore_unknown:
+            mask[i] = False
+        # Skip if predicted is initialization frame
+        elif is_special(region_tr, Trajectory.INITIALIZATION):
+            for j in range(i, min(len(trajectory), i + burnin)):
+                mask[j] = False
+        elif is_special(region_tr, Trajectory.FAILURE):
+            mask[i] = False
+        elif overlaps[i] <= threshold:
+            mask[i] = False
+
+    return overlaps[mask]
+
+@analysis_registry.register("accuracy")
+class SequenceAccuracy(SeparableAnalysis):
+    """Sequence accuracy analysis. Computes average overlap between predicted and groundtruth regions."""
+
+    burnin = Integer(default=10, val_min=0, description="Number of frames to skip after the initialization.")
+    ignore_unknown = Boolean(default=True, description="Ignore unknown regions in the groundtruth.")
+    ignore_invisible = Boolean(default=False, description="Ignore invisible regions in the groundtruth.")    
+    bounded = Boolean(default=True, description="Consider only the bounded region of the sequence.")
+    threshold = Float(default=None, val_min=0, val_max=1, description="Minimum overlap to consider.")
 
-    burnin = Integer(default=10, val_min=0)
-    grace = Integer(default=10, val_min=0)
-    bounded = Boolean(default=True)
-    threshold = Float(default=0.1, val_min=0, val_max=1)
+    def compatible(self, experiment: Experiment):
+        """Check if the experiment is compatible with the analysis."""
+        return isinstance(experiment, MultiRunExperiment)
 
     @property
     def _title_default(self):
-        return "AR Analysis"
+        """Default title of the analysis."""
+        return "Sequence accurarcy"
 
     def describe(self):
-        return Measure("Accuracy", "A", minimal=0, maximal=1, direction=Sorting.DESCENDING), \
-             Measure("Robustness", "R", minimal=0, direction=Sorting.DESCENDING), \
-             Point("AR plot", dimensions=2, abbreviation="AR",
-                minimal=(0, 0), maximal=(1, 1), labels=("Robustness", "Accuracy"), trait="ar"), \
-             None, None
-
-    def compatible(self, experiment: Experiment):
-        return isinstance(experiment, MultiStartExperiment)
+        """Describe the analysis."""
+        return Measure(self.title, "", 0, 1, Sorting.DESCENDING),
 
     def subcompute(self, experiment: Experiment, tracker: Tracker, sequence: Sequence, dependencies: List[Grid]) -> Tuple[Any]:
-
-        results = experiment.results(tracker, sequence)
-
-        forward, backward = find_anchors(sequence, experiment.anchor)
-
-        if not forward and not backward:
-            raise RuntimeError("Sequence does not contain any anchors")
-
-        robustness = 0
-        accuracy = 0
-        total = 0
-        for i, reverse in [(f, False) for f in forward] + [(f, True) for f in backward]:
-            name = "%s_%08d" % (sequence.name, i)
-
-            if not Trajectory.exists(results, name):
+        """Compute the analysis for a single sequence. 
+        
+        Args:
+            experiment (Experiment): Experiment.
+            tracker (Tracker): Tracker.
+            sequence (Sequence): Sequence.
+            dependencies (List[Grid]): List of dependencies.
+            
+        Returns:
+            Tuple[Any]: Tuple of results.
+        """
+        assert isinstance(experiment, MultiRunExperiment)
+
+        objects = sequence.objects()
+        objects_accuracy = 0
+        bounds = (sequence.size) if self.bounded else None
+
+        for object in objects:
+            trajectories = experiment.gather(tracker, sequence, objects=[object])
+            if len(trajectories) == 0:
                 raise MissingResultsException()
 
-            if reverse:
-                proxy = FrameMapSequence(sequence, list(reversed(range(0, i + 1))))
-            else:
-                proxy = FrameMapSequence(sequence, list(range(i, sequence.length)))
-
-            trajectory = Trajectory.read(results, name)
-
-            overlaps = calculate_overlaps(trajectory.regions(), proxy.groundtruth(), (proxy.size) if self.burnin else None)
+            cummulative = 0
 
-            grace = self.grace
-            progress = len(proxy)
+            for trajectory in trajectories:
+                overlaps = gather_overlaps(trajectory.regions(), sequence.object(object), self.burnin, 
+                                        ignore_unknown=self.ignore_unknown, ignore_invisible=self.ignore_invisible, bounds=bounds, threshold=self.threshold)
+                if overlaps.size > 0:
+                    cummulative += np.mean(overlaps)
 
-            for j, overlap in enumerate(overlaps):
-                if overlap <= self.threshold and not proxy.groundtruth(j).is_empty():
-                    grace = grace - 1
-                    if grace == 0:
-                        progress = j + 1 - self.grace  # subtract since we need actual point of the failure
-                        break
-                else:
-                    grace = self.grace
+            objects_accuracy += cummulative / len(trajectories)
 
-            robustness += progress  # simplified original equation: len(proxy) * (progress / len(proxy))
-            accuracy += sum(overlaps[0:progress])
-            total += len(proxy)
+        return objects_accuracy / len(objects),
 
-        ar = (robustness / total, accuracy / robustness if robustness > 0 else 0)
+@analysis_registry.register("average_accuracy")
+class AverageAccuracy(SequenceAggregator):
+    """Average accuracy analysis. Computes average overlap between predicted and groundtruth regions."""
 
-        return accuracy / robustness if robustness > 0 else 0, robustness / total, ar, robustness, len(sequence)
+    analysis = Include(SequenceAccuracy, description="Sequence accuracy analysis.")
+    weighted = Boolean(default=True, description="Weight accuracy by the number of frames.")
 
-@analysis_registry.register("multistart_average_ar")
-class AverageAccuracyRobustness(SequenceAggregator):
-
-    analysis = Include(AccuracyRobustness)
+    def compatible(self, experiment: Experiment):
+        """Check if the experiment is compatible with the analysis. This analysis requires a multirun experiment."""
+        return isinstance(experiment, MultiRunExperiment)
 
     @property
     def _title_default(self):
-        return "AR Analysis"
+        """Default title of the analysis."""
+        return "Accurarcy"
 
     def dependencies(self):
-        return self.analysis, 
-
-    def describe(self):
-        return Measure("Accuracy", "A", minimal=0, maximal=1, direction=Sorting.DESCENDING), \
-             Measure("Robustness", "R", minimal=0, direction=Sorting.DESCENDING), \
-             Point("AR plot", dimensions=2, abbreviation="AR",
-                minimal=(0, 0), maximal=(1, 1), labels=("Robustness", "Accuracy"), trait="ar"), \
-             None, None
-
-    def compatible(self, experiment: Experiment):
-        return isinstance(experiment, MultiStartExperiment)
-
-    def aggregate(self, tracker: Tracker, sequences: List[Sequence], results: Grid):
-        total_accuracy = 0
-        total_robustness = 0
-        weight_accuracy = 0
-        weight_robustness = 0
-
-        for accuracy, robustness, _, accuracy_w, robustness_w in results:
-            total_accuracy += accuracy * accuracy_w
-            total_robustness += robustness * robustness_w
-            weight_accuracy += accuracy_w
-            weight_robustness += robustness_w
-
-        ar = (total_robustness / weight_robustness, total_accuracy / weight_accuracy)
-
-        return total_accuracy / weight_accuracy, total_robustness / weight_robustness, ar, weight_accuracy, weight_robustness
-
-@analysis_registry.register("multistart_fragments")
-class MultiStartFragments(SeparableAnalysis):
-
-    burnin = Integer(default=10, val_min=0)
-    grace = Integer(default=10, val_min=0)
-    bounded = Boolean(default=True)
-    threshold = Float(default=0.1, val_min=0, val_max=1)
-
-    @property
-    def _title_default(self):
-        return "Fragment Analysis"
+        """List of dependencies."""
+        return self.analysis,
 
     def describe(self):
-        return Curve("Success", 2, "Sc", minimal=(0, 0), maximal=(1,1), trait="points"), Curve("Accuracy", 2, "Ac", minimal=(0, 0), maximal=(1,1), trait="points")
-
-    def compatible(self, experiment: Experiment):
-        return isinstance(experiment, MultiStartExperiment)
+        """Describe the analysis."""
+        return Measure(self.title, "", 0, 1, Sorting.DESCENDING),
 
-    def subcompute(self, experiment: Experiment, tracker: Tracker, sequence: Sequence, dependencies: List[Grid]) -> Tuple[Any]:
+    def aggregate(self, _: Tracker, sequences: List[Sequence], results: Grid):
+        """Aggregate the results of the analysis.
+        
+        Args:    
+            tracker (Tracker): Tracker.
+            sequences (List[Sequence]): List of sequences.
+            results (Grid): Grid of results.
+            
+        Returns:
+            Tuple[Any]: Tuple of results.
+        """
 
-        results = experiment.results(tracker, sequence)
-
-        forward, backward = find_anchors(sequence, experiment.anchor)
-
-        if not forward and not backward:
-            raise RuntimeError("Sequence does not contain any anchors")
-
-        accuracy = []
-        success = []
-
-        for i, reverse in [(f, False) for f in forward] + [(f, True) for f in backward]:
-            name = "%s_%08d" % (sequence.name, i)
-
-            if not Trajectory.exists(results, name):
-                raise MissingResultsException()
+        accuracy = 0
+        frames = 0
 
-            if reverse:
-                proxy = FrameMapSequence(sequence, list(reversed(range(0, i + 1))))
+        for i, sequence in enumerate(sequences):
+            if results[i, 0] is None:
+                continue
+
+            if self.weighted:
+                accuracy += results[i, 0][0] * len(sequence)
+                frames += len(sequence)
             else:
-                proxy = FrameMapSequence(sequence, list(range(i, sequence.length)))
-
-            trajectory = Trajectory.read(results, name)
-
-            overlaps = calculate_overlaps(trajectory.regions(), proxy.groundtruth(), (proxy.size) if self.burnin else None)
+                accuracy += results[i, 0][0]
+                frames += 1
 
-            grace = self.grace
-            progress = len(proxy)
+        return accuracy / frames,
 
-            for j, overlap in enumerate(overlaps):
-                if overlap <= self.threshold and not proxy.groundtruth(j).is_empty():
-                    grace = grace - 1
-                    if grace == 0:
-                        progress = j + 1 - self.grace  # subtract since we need actual point of the failure
-                        break
-                else:
-                    grace = self.grace
+@analysis_registry.register("success_plot")
+class SuccessPlot(SeparableAnalysis):
+    """Success plot analysis. Computes the success plot of the tracker."""
+
+    ignore_unknown = Boolean(default=True, description="Ignore unknown regions in the groundtruth.")
+    ignore_invisible = Boolean(default=False, description="Ignore invisible regions in the groundtruth.")
+    burnin = Integer(default=0, val_min=0, description="Number of frames to skip after the initialization.")
+    bounded = Boolean(default=True, description="Consider only the bounded region of the sequence.")
+    threshold = Float(default=None, val_min=0, val_max=1, description="Minimum overlap to consider.")
+    resolution = Integer(default=100, val_min=2, description="Number of points in the plot.")
 
-            success.append( (i / len(sequence), progress / len(proxy)))
-            accuracy.append( (i / len(sequence), sum(overlaps[0:progress] / len(proxy))))
-
-        return success, accuracy
-
-# TODO: remove high
-@analysis_registry.register("multistart_eao_curves")
-class EAOCurves(SeparableAnalysis):
-
-    burnin = Integer(default=10, val_min=0)
-    grace = Integer(default=10, val_min=0)
-    bounded = Boolean(default=True)
-    threshold = Float(default=0.1, val_min=0, val_max=1)
-
-    high = Integer()
+    def compatible(self, experiment: Experiment):
+        """Check if the experiment is compatible with the analysis. This analysis is only compatible with multi-run experiments."""
+        return isinstance(experiment, MultiRunExperiment)
 
     @property
     def _title_default(self):
-        return "EAO Curve"
+        """Default title of the analysis."""
+        return "Sequence success plot"
 
     def describe(self):
-        return Plot("Expected average overlap", "EAO", minimal=0, maximal=1, wrt="frames", trait="eao"),
-
-    def compatible(self, experiment: Experiment):
-        return isinstance(experiment, MultiStartExperiment)
+        """Describe the analysis."""
+        return Curve("Plot", 2, "S", minimal=(0, 0), maximal=(1, 1), labels=("Threshold", "Success"), trait="success"),
 
     def subcompute(self, experiment: Experiment, tracker: Tracker, sequence: Sequence, dependencies: List[Grid]) -> Tuple[Any]:
+        """Compute the analysis for a single sequence. 
 
-        results = experiment.results(tracker, sequence)
+        Args:
+            experiment (Experiment): Experiment.
+            tracker (Tracker): Tracker.
+            sequence (Sequence): Sequence.
+            dependencies (List[Grid]): List of dependencies.
 
-        forward, backward = find_anchors(sequence, experiment.anchor)
+        Returns:
+            Tuple[Any]: Tuple of results.
+        """
 
-        if len(forward) == 0 and len(backward) == 0:
-            raise RuntimeError("Sequence does not contain any anchors")
+        assert isinstance(experiment, MultiRunExperiment)
 
-        overlaps_all = []
-        success_all = []
+        objects = sequence.objects()
+        bounds = (sequence.size) if self.bounded else None
 
-        for i, reverse in [(f, False) for f in forward] + [(f, True) for f in backward]:
-            name = "%s_%08d" % (sequence.name, i)
+        axis_x = np.linspace(0, 1, self.resolution)
+        axis_y = np.zeros_like(axis_x)
 
-            if not Trajectory.exists(results, name):
+        for object in objects:
+            trajectories = experiment.gather(tracker, sequence, objects=[object])
+            if len(trajectories) == 0:
                 raise MissingResultsException()
 
-            if reverse:
-                proxy = FrameMapSequence(sequence, list(reversed(range(0, i + 1))))
-            else:
-                proxy = FrameMapSequence(sequence, list(range(i, sequence.length)))
+            object_y = np.zeros_like(axis_x) 
 
-            trajectory = Trajectory.read(results, name)
+            for trajectory in trajectories:
+                overlaps = gather_overlaps(trajectory.regions(), sequence.object(object), burnin=self.burnin, ignore_unknown=self.ignore_unknown, ignore_invisible=self.ignore_invisible, bounds=bounds, threshold=self.threshold)
 
-            overlaps = calculate_overlaps(trajectory.regions(), proxy.groundtruth(), proxy.size if self.burnin else None)
+                for i, threshold in enumerate(axis_x):
+                    if threshold == 1:
+                        # Nicer handling of the edge case
+                        object_y[i] += np.sum(overlaps >= threshold) / len(overlaps)
+                    else:
+                        object_y[i] += np.sum(overlaps > threshold) / len(overlaps)
 
-            grace = self.grace
-            progress = len(proxy)
+            axis_y += object_y / len(trajectories)
 
-            for j, overlap in enumerate(overlaps):
-                if overlap <= self.threshold and not proxy.groundtruth(j).is_empty():
-                    grace = grace - 1
-                    if grace == 0:
-                        progress = j + 1 - self.grace  # subtract since we need actual point of the failure
-                        break
-                else:
-                    grace = self.grace
+        axis_y /= len(objects)
 
-            success = True
-            if progress < len(overlaps):
-                # tracker has failed during this run
-                overlaps[progress:] = (len(overlaps) - progress) * [float(0)]
-                success = False
+        return [(x, y) for x, y in zip(axis_x, axis_y)],
 
-            overlaps_all.append(overlaps)
-            success_all.append(success)
 
-        return compute_eao_partial(overlaps_all, success_all, self.high), 1
+@analysis_registry.register("average_success_plot")
+class AverageSuccessPlot(SequenceAggregator):
+    """Average success plot analysis. Computes the average success plot of the tracker."""
 
-#TODO: remove high
-@analysis_registry.register("multistart_eao_curve")
-class EAOCurve(SequenceAggregator):
-
-    curves = Include(EAOCurves)
-    
-    @property
-    def _title_default(self):
-        return "EAO Curve"
-
-    def describe(self):
-        return Plot("Expected average overlap", "EAO", minimal=0, maximal=1, wrt="frames", trait="eao"),
-
-    def compatible(self, experiment: Experiment):
-        return isinstance(experiment, MultiStartExperiment)
+    resolution = Integer(default=100, val_min=2)
+    analysis = Include(SuccessPlot)
 
     def dependencies(self):
-        return self.curves,
-
-    def aggregate(self, tracker: Tracker, sequences: List[Sequence], results: Grid) -> Tuple[Any]:
-
-        eao_curve = self.curves.high * [float(0)]
-        eao_weights = self.curves.high * [float(0)]
+        """List of dependencies."""
+        return self.analysis,
 
-        for (seq_eao_curve, eao_active), seq_w in results:
-            for i, (eao_, active_) in enumerate(zip(seq_eao_curve, eao_active)):
-                eao_curve[i] += eao_ * active_ * seq_w
-                eao_weights[i] += active_ * seq_w
-
-        return [eao_ / w_ if w_ > 0 else 0 for eao_, w_ in zip(eao_curve, eao_weights)],
-
-@analysis_registry.register("multistart_eao_score")
-class EAOScore(Analysis):
-
-    low = Integer()
-    high = Integer()
-    eaocurve = Include(EAOCurve)
+    def compatible(self, experiment: Experiment):
+        """Check if the experiment is compatible with the analysis. This analysis is only compatible with multi-run experiments."""
+        return isinstance(experiment, MultiRunExperiment)
 
     @property
     def _title_default(self):
-        return "EAO analysis"
+        """Default title of the analysis."""
+        return "Success plot"
 
     def describe(self):
-        return Measure("Expected average overlap", "EAO", minimal=0, maximal=1, direction=Sorting.DESCENDING),
+        """Describe the analysis."""
+        return Curve("Plot", 2, "S", minimal=(0, 0), maximal=(1, 1), labels=("Threshold", "Success"), trait="success"),
 
-    def compatible(self, experiment: Experiment):
-        return isinstance(experiment, MultiStartExperiment)
-
-    def dependencies(self):
-        return self.eaocurve,
+    def aggregate(self, _: Tracker, sequences: List[Sequence], results: Grid):
+        """Aggregate the results of the analysis.
+        
+        Args:    
+            tracker (Tracker): Tracker. 
+            sequences (List[Sequence]): List of sequences.
+            results (Grid): Grid of results.
+            
+        Returns:
+            Tuple[Any]: Tuple of results.
+        """
+        
+        axis_x = np.linspace(0, 1, self.resolution)
+        axis_y = np.zeros_like(axis_x)
+
+        for i, _ in enumerate(sequences):
+            if results[i, 0] is None:
+                continue
 
-    def compute(self, experiment: Experiment, trackers: List[Tracker], sequences: List[Sequence], dependencies: List[Grid]) -> Grid:
+            curve = results[i, 0][0]
 
-        return dependencies[0].foreach(lambda x, i, j: (float(np.mean(x[0][self.low:self.high + 1])), ) )
+            for j, (_, y) in enumerate(curve):
+                axis_y[j] += y
 
-    @property
-    def axes(self):
-        return Axes.TRACKERS
+        axis_y /= len(sequences)
 
+        return [(x, y) for x, y in zip(axis_x, axis_y)],
```

### Comparing `vot-toolkit-0.6.2/vot/dataset/__init__.py` & `vot-toolkit-0.6.4/vot/region/shapes.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,646 +1,507 @@
-import os
-import logging
+""" Module for region shapes. """
 
-from numbers import Number
-from collections import namedtuple
-from abc import abstractmethod, ABC
-from typing import List, Mapping, Optional, Set, Tuple
+from copy import copy
+from functools import reduce
+from typing import Tuple, List
+from abc import ABC, abstractmethod
 
-from PIL.Image import Image
 import numpy as np
-from trax import Region
-
-from vot import ToolkitException
-
+from numba import jit
 import cv2
 
-logger = logging.getLogger("vot")
-
-class DatasetException(ToolkitException):
-    """Dataset and sequence related exceptions
-    """
-    pass
+from vot.region import Region, ConversionException, RegionType, RegionException
+from vot.utilities.draw import DrawHandle
 
-class Channel(ABC):
-    """Abstract representation of individual image channel, a sequence of images
+class Shape(Region, ABC):
+    """ Base class for all shape regions. """
 
-    """
+    @abstractmethod
+    def draw(self, handle: DrawHandle) -> None:
+        """ Draw the region to the given handle. 
+ 
+        """
+        pass
 
-    def __init__(self):
+    @abstractmethod
+    def resize(self, factor=1) -> "Shape":
+        """ Resize the region by the given factor. """
         pass
 
-    @property
     @abstractmethod
-    def length(self) -> int:
-        """Returns the length of channel
+    def move(self, dx=0, dy=0) -> "Shape":
+        """ Move the region by the given offset. 
+        
+        Args:
+            dx (float, optional): X offset. Defaults to 0.
+            dy (float, optional): Y offset. Defaults to 0.
+            
+        Returns:
+            Shape: Moved region.
         """
         pass
 
     @abstractmethod
-    def frame(self, index: int) -> "Frame":
-        """Returns frame object for the given index
+    def rasterize(self, bounds: Tuple[int, int, int, int]) -> np.ndarray:
+        """ Rasterize the region to a binary mask.
 
         Args:
-            index (int): _description_
+            bounds (Tuple[int, int, int, int]): Bounds of the mask.
 
         Returns:
-            Frame: _description_
-        """
+            np.ndarray: Binary mask.
+        """ 
         pass
 
     @abstractmethod
-    def filename(self, index: int) -> str:
-        pass
+    def bounds(self) -> Tuple[int, int, int, int]:
+        """ Get the bounding box of the region.
+        
+        Returns:
+            Tuple[int, int, int, int]: Bounding box (x, y, width, height).
+        """
 
-    @property
-    @abstractmethod
-    def size(self) -> int:
         pass
 
-class Frame(object):
-
-    def __init__(self, sequence, index):
-        self._sequence = sequence
-        self._index = index
-
-    @property
-    def index(self) -> int:
-        return self._index
-
-    @property
-    def sequence(self) -> 'Sequence':
-        return self._sequence
-
-    def channels(self):
-        return self._sequence.channels()
-
-    def channel(self, channel: Optional[str] = None):
-        channelobj = self._sequence.channel(channel)
-        if channelobj is None:
-            return None
-        return channelobj.frame(self._index)
-
-    def filename(self, channel: Optional[str] = None):
-        channelobj = self._sequence.channel(channel)
-        if channelobj is None:
-            return None
-        return channelobj.filename(self._index)
-
-    def image(self, channel: Optional[str] = None):
-        channelobj = self._sequence.channel(channel)
-        if channelobj is None:
-            return None
-        return channelobj.frame(self._index)
-
-    def objects(self):
-        objects = {}
-        for o in self._sequence.objects():
-            region = self._sequence.object(o, self._index)
-            if region is not None:
-                objects[o] = region
-        return objects
-
-    def object(self, id: str):
-        return self._sequence.object(id, self._index)
-
-    def groundtruth(self):
-        return self._sequence.groundtruth(self._index)
-
-    def tags(self):
-        return self._sequence.tags(self._index)
-
-    def values(self):
-        return self._sequence.values(self._index)
-
-class SequenceIterator(object):
-
-    def __init__(self, sequence: "Sequence"):
-        self._position = 0
-        self._sequence = sequence
-
-    def __iter__(self):
-        return self
-
-    def __next__(self) -> Frame:
-        if self._position >= len(self._sequence):
-            raise StopIteration()
-        index = self._position
-        self._position += 1
-        return Frame(self._sequence, index)
-
-class InMemoryChannel(Channel):
-
-    def __init__(self):
-        super().__init__()
-        self._images = []
-        self._width = 0
-        self._height = 0
-        self._depth = 0
-
-    def append(self, image):
-        if isinstance(image, Image):
-            image = np.asarray(image)
-
-        if len(image.shape) == 3:
-            height, width, depth = image.shape
-        elif len(image.shape) == 2:
-            height, width = image.shape
-            depth = 1
-        else:
-            raise DatasetException("Illegal image dimensions")
-
-        if self._width > 0:
-            if not (self._width == width and self._height == height):
-                raise DatasetException("Size of images does not match")
-            if not self._depth == depth:
-                raise DatasetException("Channels of images does not match")
-        else:
-            self._width = width
-            self._height = height
-            self._depth = depth
-
-        self._images.append(image)
-
-    @property
-    def length(self):
-        return len(self._images)
-
-    def frame(self, index):
-        if index < 0 or index >= self.length:
-            return None
-
-        return self._images[index]
-
-    @property
-    def size(self):
-        return self._width, self._height
-
-    def filename(self, index):
-        raise DatasetException("Sequence is available in memory, image files not available")
-
-class PatternFileListChannel(Channel):
-    """Sequence channel implementation where each frame is stored in a file and all file names
-    follow a specific pattern.
+class Rectangle(Shape):
     """
+    Rectangle region class for representing rectangular regions.
+    """
+    def __init__(self, x=0, y=0, width=0, height=0):
+        """ Constructor for rectangle region.
 
-    def __init__(self, path, start=1, step=1, end=None):
-        super().__init__()
-        base, pattern = os.path.split(path)
-        self._base = base
-        self._pattern = pattern
-        self.__scan(pattern, start, step, end)
-
-    @property
-    def base(self) -> str:
-        """_summary_
-
-        Returns:
-            _type_: _description_
+        Args:
+            x (float, optional): X coordinate of the top left corner. Defaults to 0.
+            y (float, optional): Y coordinate of the top left corner. Defaults to 0.
+            width (float, optional): Width of the rectangle. Defaults to 0.
+            height (float, optional): Height of the rectangle. Defaults to 0.
         """
-        return self._base
-
-    @property
-    def pattern(self):
-        return self._pattern
-
-    def __scan(self, pattern, start, step, end):
-
-        extension = os.path.splitext(pattern)[1]
-        if not extension in {'.jpg', '.png'}:
-            raise DatasetException("Invalid extension in pattern {}".format(pattern))
-
-        i = start
-        self._files = []
-
-        fullpattern = os.path.join(self.base, pattern)
-
-        while True:
-            image_file = os.path.join(fullpattern % i)
-
-            if not os.path.isfile(image_file):
-                break
-            self._files.append(os.path.basename(image_file))
-            i = i + step
-
-            if end is not None and i > end:
-                break
-
-        if i <= start:
-            raise DatasetException("Empty sequence, no frames found.")
+        super().__init__()
+        self._data = np.array([[x], [y], [width], [height]], dtype=np.float32)
 
-        im = cv2.imread(self.filename(0))
-        self._width = im.shape[1]
-        self._height = im.shape[0]
-        self._depth = im.shape[2]
+    def __str__(self):
+        """ Create string from class """
+        return '{},{},{},{}'.format(self.x, self.y, self.width, self.height)
 
     @property
-    def length(self):
-        return len(self._files)
-
-    def frame(self, index):
-        if index < 0 or index >= self.length:
-            return None
-
-        bgr = cv2.imread(self.filename(index))
-        return cv2.cvtColor(bgr, cv2.COLOR_BGR2RGB)
+    def x(self):
+        """ X coordinate of the top left corner. """
+        return float(self._data[0, 0])
 
     @property
-    def size(self):
-        return self._width, self._height
+    def y(self):
+        """ Y coordinate of the top left corner. """
+        return float(self._data[1, 0])
 
     @property
     def width(self):
-        return self._width
+        """ Width of the rectangle."""
+        return float(self._data[2, 0])
 
     @property
     def height(self):
-        return self._height
-
-    def filename(self, index):
-        if index < 0 or index >= self.length:
-            return None
-
-        return os.path.join(self.base, self._files[index])
-
-    def __len__(self):
-        return self.length
-
-class FrameList(ABC):
-    """Abstract base for all sequences, just a list of frame objects
-    """
-
-    def __iter__(self):
-        return SequenceIterator(self)
-
-    @abstractmethod
-    def __len__(self) -> int:
-        pass
-
-    @abstractmethod
-    def frame(self, index: int) -> Frame:
-        pass
-
-class Sequence(FrameList):
-    """_summary_
-
-    """
-
-    UNKNOWN = 0
-    INVISIBLE = 1
-
-    def __init__(self, name: str, dataset: "Dataset" = None):
-        self._name = name
-        self._dataset = dataset
-
-    def __len__(self) -> int:
-        return self.length
-
-    @property
-    def name(self) -> str:
-        return self._name
+        """ Height of the rectangle."""
+        return float(self._data[3, 0])
 
     @property
-    def identifier(self) -> str:
-        return self._name
-
-    @property
-    def dataset(self):
-        return self._dataset
-
-    @abstractmethod
-    def metadata(self, name, default=None):
-        pass
-
-    @abstractmethod
-    def channel(self, channel=None) -> Channel:
-        pass
-
-    @abstractmethod
-    def channels(self) -> Set[str]:
-        pass
+    def type(self):
+        """ Type of the region."""
+        return RegionType.RECTANGLE
 
-    @abstractmethod
-    def objects(self) -> Set[str]:
-        pass
+    def copy(self):
+        """ Copy region to another object. """
+        return copy(self)
 
-    @abstractmethod
-    def object(self, id, index=None):
-        pass
+    def convert(self, rtype: RegionType):
+        """ Convert region to another type. Note that some conversions degrade information.
+        
+        Args:
+            rtype (RegionType): Desired type.
+        
+        Raises:
+            ConversionException: Unable to convert rectangle region to {rtype}
+        """
+        if rtype == RegionType.RECTANGLE:
+            return self.copy()
+        elif rtype == RegionType.POLYGON:
+            points = []
+            points.append((self.x, self.y))
+            points.append((self.x + self.width - 1, self.y))
+            points.append((self.x + self.width - 1, self.y + self.height - 1))
+            points.append((self.x, self.y + self.height - 1))
+            return Polygon(points)
+        elif rtype == RegionType.MASK:
+            return Mask(np.ones((int(round(self.height)), int(round(self.width))), np.uint8), (int(round(self.x)), int(round(self.y))))
+        else:
+            raise ConversionException("Unable to convert rectangle region to {}".format(rtype), source=self)
 
-    @abstractmethod
-    def groundtruth(self, index: int) -> Region:
-        pass
+    def is_empty(self):
+        """ Check if the region is empty.
+        
+        Returns:
+            bool: True if the region is empty, False otherwise.
+        """
+        if self.width > 0 and self.height > 0:
+            return False
+        else:
+            return True
 
-    @abstractmethod
-    def tags(self, index=None) -> List[str]:
-        pass
+    def draw(self, handle: DrawHandle):
+        """ Draw the region to the given handle.
+        
+        Args:
+            handle (DrawHandle): Handle to draw to.
+        """
+        polygon = [(self.x, self.y), (self.x + self.width, self.y), \
+            (self.x + self.width, self.y + self.height), \
+            (self.x, self.y + self.height)]
+        handle.polygon(polygon)
+
+    def resize(self, factor=1):
+        """ Resize the region by the given factor.
+        
+        Args:
+            factor (float, optional): Resize factor. Defaults to 1.
+            
+        Returns:
+            Rectangle: Resized region.
+        """
+        return Rectangle(self.x * factor, self.y * factor,
+                         self.width * factor, self.height * factor)
 
-    @abstractmethod
-    def values(self, index=None) -> Mapping[str, Number]:
-        pass
+    def center(self):
+        """ Get the center of the region.
+        
+        Returns:
+            tuple: Center coordinates (x,y).
+        """
+        return (self.x + self.width / 2, self.y + self.height / 2)
 
-    @property
-    @abstractmethod
-    def size(self) -> Tuple[int, int]:
-        pass
+    def move(self, dx=0, dy=0):
+        """ Move the region by the given offset.
+        
+        Args:
+            dx (float, optional): X offset. Defaults to 0.
+            dy (float, optional): Y offset. Defaults to 0.
+            
+        Returns:
+            Rectangle: Moved region.
+        """
+        return Rectangle(self.x + dx, self.y + dy, self.width, self.height)
 
-    @property
-    @abstractmethod
-    def length(self) -> int:
-        pass
+    def rasterize(self, bounds: Tuple[int, int, int, int]):
+        """ Rasterize the region to a binary mask.
+        
+        Args:
+            bounds (tuple): Bounds of the mask (x1,y1,x2,y2).
+        """
+        from vot.region.raster import rasterize_rectangle
+        return rasterize_rectangle(self._data, np.array(bounds))
 
-    def describe(self):
-        data = dict(length=self.length, size=self.size)
-        return data
+    def bounds(self):
+        """ Get the bounding box of the region.
+        
+        Returns:
+            tuple: Bounding box (x1,y1,x2,y2).
+        """
+        return int(round(self.x)), int(round(self.y)), int(round(self.width + self.x)), int(round(self.height + self.y))
 
-class Dataset(ABC):
-    """Base class for a tracking dataset, a list of image sequences addressable by their names.
+class Polygon(Shape):
+    """
+    Polygon region defined by a list of points. The polygon is closed, i.e. the first and last point are connected.
     """
+    def __init__(self, points):
+        """
+        Constructor
 
-    def __init__(self, path):
-        self._path = path
+        Args:
+            points (list): List of points as tuples [(x1,y1), (x2,y2),...,(xN,yN)]
+        """
+        super().__init__()
+        assert(points)
+        self._points = np.array(points, dtype=np.float32)
+        assert(self._points.shape[0] >= 3 and self._points.shape[1] == 2)  # pylint: disable=E1136
 
-    def __len__(self):
-        return self.length
 
-    @property
-    def path(self):
-        return self._path
+    def __str__(self):
+        """ Create string from class """
+        return ','.join(['{},{}'.format(p[0], p[1]) for p in self._points])
 
     @property
-    @abstractmethod
-    def length(self):
-        pass
+    def type(self):
+        """ Get the region type. """
+        return RegionType.POLYGON
 
-    @abstractmethod
-    def __getitem__(self, key):
-        pass
+    @property
+    def size(self):
+        """ Get the number of points. """
+        return self._points.shape[0] # pylint: disable=E1136
 
-    @abstractmethod
-    def __contains__(self, key):
-        return False
+    def __getitem__(self, i):
+        """ Get the i-th point."""
+        return self._points[i, 0], self._points[i, 1]
+
+    def points(self):
+        """ Get the list of points. 
+        
+        Returns:
+            list: List of points as tuples [(x1,y1), (x2,y2),...,(xN,yN)]
+        """
+        return [self[i] for i in range(self.size)]
 
-    @abstractmethod
-    def __iter__(self):
-        pass
+    def copy(self):
+        """ Create a copy of the polygon. """
+        return copy(self)
+
+    def convert(self, rtype: RegionType):
+        """ Convert the polygon to another region type.
+        
+        Args:
+            rtype (RegionType): Target region type.
+            
+        Returns:
+            Region: Converted region.
+        """
+        if rtype == RegionType.POLYGON:
+            return self.copy()
+        elif rtype == RegionType.RECTANGLE:
+            top = np.min(self._points[:, 1])
+            bottom = np.max(self._points[:, 1])
+            left = np.min(self._points[:, 0])
+            right = np.max(self._points[:, 0])
+
+            return Rectangle(left, top, right - left, bottom - top)
+        elif rtype == RegionType.MASK:
+            bounds = self.bounds()
+            mask = self.rasterize(bounds)
+            return Mask(mask, offset=(bounds[0], bounds[1]))
+        else:
+            raise ConversionException("Unable to convert polygon region to {}".format(rtype), source=self)
 
-    @abstractmethod
-    def list(self) -> List[str]:
-        """Returns a list of unique sequence names
+    def draw(self, handle: DrawHandle):
+        """ Draw the polygon on the given handle.
+        
+        Args:
+            handle (DrawHandle): Handle to draw on.
+        """
+        handle.polygon([(p[0], p[1]) for p in self._points])
 
+    def resize(self, factor=1):
+        """ Resize the polygon by a factor.
+        
+        Args:
+            factor (float): Resize factor.
+            
         Returns:
-            List[str]: List of sequence names
+            Polygon: Resized polygon.
         """
-        return []
-
-    def keys(self) -> List[str]:
-        """Returns a list of unique sequence names
+        return Polygon([(p[0] * factor, p[1] * factor) for p in self._points])
 
+    def move(self, dx=0, dy=0):
+        """ Move the polygon by a given offset.
+        
+        Args:
+            dx (float): X offset.
+            dy (float): Y offset.
+            
         Returns:
-            List[str]: List of sequence names
+            Polygon: Moved polygon.
         """
-        return self.list()
+        return Polygon([(p[0] + dx, p[1] + dy) for p in self._points])
 
-SequenceData = namedtuple("SequenceData", ["channels", "objects", "tags", "values", "length"])
+    def is_empty(self):
+        """ Check if the polygon is empty.
+        
+        Returns:
+            bool: True if the polygon is empty, False otherwise.
+            
+        """
+        top = np.min(self._points[:, 1])
+        bottom = np.max(self._points[:, 1])
+        left = np.min(self._points[:, 0])
+        right = np.max(self._points[:, 0])
+        return top == bottom or left == right
+
+    def rasterize(self, bounds: Tuple[int, int, int, int]):
+        """ Rasterize the polygon into a binary mask.
+        
+        Args:
+            bounds (tuple): Bounding box of the mask as (left, top, right, bottom).
+            
+        Returns:
+            numpy.ndarray: Binary mask.
+        """
+        from vot.region.raster import rasterize_polygon
+        return rasterize_polygon(self._points, bounds)
 
-class BaseSequence(Sequence):
+    def bounds(self):
+        """ Get the bounding box of the polygon.
 
-    def __init__(self, name, dataset=None):
-        super().__init__(name, dataset)
-        self._metadata = self._read_metadata()
-        self._data = None
+        Returns:
+            tuple: Bounding box as (left, top, right, bottom).
+        """
+        top = np.min(self._points[:, 1])
+        bottom = np.max(self._points[:, 1])
+        left = np.min(self._points[:, 0])
+        right = np.max(self._points[:, 0])
+        return int(round(left)), int(round(top)), int(round(right)), int(round(bottom))
 
-    @abstractmethod
-    def _read_metadata(self):
-        raise NotImplementedError
+from vot.region.raster import mask_bounds
+from vot.region.io import mask_to_rle
 
-    @abstractmethod
-    def _read(self) -> SequenceData:
-        raise NotImplementedError
+class Mask(Shape):
+    """Mask region defined by a binary mask. The mask is defined by a binary image and an offset.
+    """
 
-    def __preload(self):
-        if self._data is None:
-            self._data = self._read()
-
-    def metadata(self, name, default=None):
-        return self._metadata.get(name, default)
-
-    def channels(self):
-        self.__preload()
-        return self._data.channels.keys()
-
-    def channel(self, channel=None):
-        self.__preload()
-        if channel is None:
-            channel = self.metadata("channel.default")
-        return self._data.channels.get(channel, None)
-
-    def frame(self, index):
-        return Frame(self, index)
-
-    def objects(self):
-        self.__preload()
-        return self._data.objects.keys()
-
-    def object(self, id, index=None):
-        self.__preload()
-        obj = self._data.objects.get(id, None)
-        if index is None:
-            return obj
-        if obj is None:
-            return None
-        return obj[index]
-
-    def groundtruth(self, index=None):
-        self.__preload()
-        if len(self.objects()) != 1:
-            raise DatasetException("More than one object in sequence")
-
-        id = next(iter(self._data.objects))
-        return self.object(id, index)
-
-    def tags(self, index=None):
-        self.__preload()
-        if index is None:
-            return self._data.tags.keys()
-        return [t for t, sq in self._data.tags.items() if sq[index]]
-
-    def values(self, index=None):
-        self.__preload()
-        if index is None:
-            return self._data.values.keys()
-        return {v: sq[index] for v, sq in self._data.values.items()}
+    def __init__(self, mask: np.array, offset: Tuple[int, int] = (0, 0), optimize=False):
+        """ Constructor
+        
+        Args:
+            mask (numpy.ndarray): Binary mask.
+            offset (tuple): Offset of the mask as (x, y). 
+            optimize (bool): Optimize the mask by removing empty rows and columns.
+            
+        """
+        super().__init__()
+        self._mask = mask.astype(np.uint8)
+        self._mask[self._mask > 0] = 1
+        self._offset = offset
+        if optimize:  # optimize is used when mask without an offset is given (e.g. full-image mask)
+            self._optimize()
+            
+    def __str__(self):
+        """ Create string from class """
+        offset_str = '%d,%d' % self.offset
+        region_sz_str = '%d,%d' % (self.mask.shape[1], self.mask.shape[0])
+        rle_str = ','.join([str(el) for el in mask_to_rle(self.mask)])
+        return 'm%s,%s,%s' % (offset_str, region_sz_str, rle_str)
+
+    def _optimize(self):
+        """ Optimize the mask by removing empty rows and columns. If the mask is empty, the mask is set to zero size.
+         Do not call this method directly, it is called from the constructor. """
+        bounds = mask_bounds(self.mask)
+        if bounds[2] == 0:
+            # mask is empty
+            self._mask = np.zeros((0, 0), dtype=np.uint8)
+            self._offset = (0, 0)
+        else:
 
-    @property
-    def size(self):
-        return self.channel().size
+            self._mask = np.copy(self.mask[bounds[1]:bounds[3]+1, bounds[0]:bounds[2]+1])
+            self._offset = (bounds[0] + self.offset[0], bounds[1] + self.offset[1])
 
     @property
-    def width(self):
-        return self.channel().width
+    def mask(self):
+        """ Get the mask. Note that you should not modify the mask directly. Also make sure to
+        take into account the offset when using the mask."""
+        return self._mask
 
     @property
-    def height(self):
-        return self.channel().height
+    def offset(self):
+        """ Get the offset of the mask in pixels."""
+        return self._offset
 
     @property
-    def length(self):
-        self.__preload()
-        return self._data.length
-
-class InMemorySequence(BaseSequence):
-
-    def __init__(self, name, channels):
-        super().__init__(name, None)
-        self._channels = {c: InMemoryChannel() for c in channels}
-        self._tags = {}
-        self._values = {}
-        self._groundtruth = []
-
-    def _read_metadata(self):
-        return dict()
+    def type(self):
+        """ Get the region type."""
+        return RegionType.MASK
 
-    def _read(self):
-        return SequenceData(self._channels, {"object" : self._groundtruth}, self._tags, self._values)
+    def copy(self):
+        """ Create a copy of the mask."""
+        return copy(self)
 
-    def append(self, images: dict, region: "Region", tags: list = None, values: dict = None):
-
-        if not set(images.keys()).issuperset(self._channels.keys()):
-            raise DatasetException("Images not provided for all channels")
-
-        for k, channel in self._channels.items():
-            channel.append(images[k])
-
-        if tags is None:
-            tags = set()
+    def convert(self, rtype: RegionType):
+        """ Convert the mask to another region type. The mask is converted to a rectangle or polygon by approximating bounding box of the mask.
+        
+        Args:
+            rtype (RegionType): Target region type.
+            
+        Returns:
+            Shape: Converted region.
+        """
+        if rtype == RegionType.MASK:
+            return self.copy()
+        elif rtype == RegionType.RECTANGLE:
+            bounds = mask_bounds(self.mask)
+            return Rectangle(bounds[0] + self.offset[0], bounds[1] + self.offset[1],
+                            bounds[2] - bounds[0], bounds[3] - bounds[1])
+        elif rtype == RegionType.POLYGON:
+            bounds = mask_bounds(self.mask)
+            if None in bounds:
+                return Polygon([(0, 0), (0, 0), (0, 0), (0, 0)])
+            return Polygon([
+                (bounds[0] + self.offset[0], bounds[1] + self.offset[1]),
+                (bounds[2] + self.offset[0], bounds[1] + self.offset[1]),
+                (bounds[2] + self.offset[0], bounds[3] + self.offset[1]),
+                (bounds[0] + self.offset[0], bounds[3] + self.offset[1])])
         else:
-            tags = set(tags)
-        for tag in tags:
-            if not tag in self._tags:
-                self._tags[tag] = [False] * self.length
-            self._tags[tag].append(True)
-        for tag in set(self._tags.keys()).difference(tags):
-                self._tags[tag].append(False)
-
-        if values is None:
-            values = dict()
-        for name, value in values.items():
-            if not name in self._values:
-                self._values[name] = [0] * self.length
-            self._values[tag].append(value)
-        for name in set(self._values.keys()).difference(values.keys()):
-                self._values[name].append(0)
-
-        self._groundtruth.append(region)
-
-def download_bundle(url: str, path: str = "."):
-    """Downloads a dataset bundle as a ZIP file and decompresses it.
-
-    Args:
-        url (str): Source bundle URL
-        path (str, optional): Destination directory. Defaults to ".".
+            raise ConversionException("Unable to convert mask region to {}".format(rtype), source=self)
 
-    Raises:
-        DatasetException: If the bundle cannot be downloaded or is not supported.
-    """
-
-    from vot.utilities.net import download_uncompress, NetworkException
+    def draw(self, handle: DrawHandle):
+        """ Draw the mask into an image.
+        
+        Args:
+            handle (DrawHandle): Handle to the image.
+        """
+        handle.mask(self._mask, self.offset)
 
-    if not url.endswith(".zip"):
-        raise DatasetException("Unknown bundle format")
+    def rasterize(self, bounds: Tuple[int, int, int, int]):
+        """ Rasterize the mask into a binary mask. The mask is cropped to the given bounds.
+        
+        Args:
+            bounds (tuple): Bounding box of the mask as (left, top, right, bottom).
 
-    logger.info('Downloading sequence bundle from "%s". This may take a while ...', url)
+        Returns:
+            numpy.ndarray: Binary mask. The mask is a copy of the original mask.
+        """
+        from vot.region.raster import copy_mask
+        return copy_mask(self._mask, self._offset, np.array(bounds))
 
-    try:
-        download_uncompress(url, path)
-    except NetworkException as e:
-        raise DatasetException("Unable do download dataset bundle, Please try to download the bundle manually from {} and uncompress it to {}'".format(url, path))
-    except IOError as e:
-        raise DatasetException("Unable to extract dataset bundle, is the target directory writable and do you have enough space?")
-
-from .vot import VOTDataset, VOTSequence
-from .got10k import GOT10kSequence, GOT10kDataset
-from .otb import OTBDataset, OTBSequence
-from .trackingnet import TrackingNetDataset, TrackingNetSequence
-
-def download_dataset(url: str, path: str):
-    """Downloads a dataset from a given url or an alias.
-
-    Args:
-        url (str): URL to the data bundle or metadata description file
-        path (str): Destination directory
+    def is_empty(self):
+        """ Check if the mask is empty.
+        
+        Returns:
+            bool: True if the mask is empty, False otherwise.
+        """
+        bounds = mask_bounds(self.mask)
+        return bounds[2] == 0 or bounds[3] == 0
 
-    Raises:
-        DatasetException: If the dataset is not found or a network error occured
-    """
-    from urllib.parse import urlsplit
+    def resize(self, factor=1):
+        """ Resize the mask by a given factor. The mask is resized using nearest neighbor interpolation.
+        
+        Args:
+            factor (float): Resize factor.
+            
+        Returns:
+            Mask: Resized mask.
+        """
 
-    try:
-        res = urlsplit(url)
+        offset = (int(self.offset[0] * factor), int(self.offset[1] * factor))
+        height = max(1, int(self.mask.shape[0] * factor))
+        width = max(1, int(self.mask.shape[1] * factor))
 
-        if res.scheme in ["http", "https"]:
-            if res.path.endswith(".json"):
-                from .vot import download_dataset_meta
-                download_dataset_meta(url, path)
-            else:
-                download_bundle(url, path)
-        elif res.scheme == "otb":
-            from .otb import download_dataset as download_otb
-            download_otb(path, res.path == "otb50")
+        if self.mask.size == 0:
+            mask = np.zeros((0, 0), dtype=np.uint8)
         else:
-            raise DatasetException("Unknown dataset domain: {}".format(res.scheme))
+            mask = cv2.resize(self.mask, dsize=(width, height), interpolation=cv2.INTER_NEAREST)
 
-    except ValueError:
-        raise DatasetException("Illegal dataset URI format")
+        return Mask(mask, offset, False)
 
+    def move(self, dx=0, dy=0):
+        """ Move the mask by a given offset.
 
-def load_dataset(path: str) -> Dataset:
-    """Loads a dataset from a local directory
-
-    Args:
-        path (str): The path to the local dataset data
-
-    Raises:
-        DatasetException: When a folder does not exist or the format is not recognized.
-
-    Returns:
-        Dataset: Dataset object
-    """
-
-    if not os.path.isdir(path):
-        raise DatasetException("Dataset directory does not exist")
-
-    if VOTDataset.check(path):
-        return VOTDataset(path)
-    elif GOT10kDataset.check(path):
-        return GOT10kDataset(path)
-    elif OTBDataset.check(path):
-        return OTBDataset(path)
-    elif TrackingNetDataset.check(path):
-        return TrackingNetDataset(path)
-    else:
-        raise DatasetException("Unsupported dataset type")
-
-def load_sequence(path: str) -> Sequence:
-    """Loads a sequence from a given path (directory), tries to guess the format of the sequence.
-
-    Args:
-        path (str): The path to the local sequence data
+        Args:
+            dx (int): Horizontal offset.
+            dy (int): Vertical offset.
 
-    Raises:
-        DatasetException: If an loading error occures, unsupported format or other issues.
+        Returns:
+            Mask: Moved mask.
+        """
+        return Mask(self._mask, (self.offset[0] + dx, self.offset[1] + dy))
 
-    Returns:
-        Sequence: Sequence object
-    """
+    def bounds(self):
+        """ Get the bounding box of the mask.
 
-    if VOTSequence.check(path):
-        return VOTSequence(path)
-    elif GOT10kSequence.check(path):
-        return GOT10kSequence(path)
-    elif OTBSequence.check(path):
-        return OTBSequence(path)
-    elif TrackingNetSequence.check(path):
-        return TrackingNetSequence(path)
-    else:
-        raise DatasetException("Unsupported sequence type")
+        Returns:
+            tuple: Bounding box of the mask as (left, top, right, bottom).
+        """
+        bounds = mask_bounds(self.mask)
+        return bounds[0] + self.offset[0], bounds[1] + self.offset[1], bounds[2] + self.offset[0], bounds[3] + self.offset[1]
```

### Comparing `vot-toolkit-0.6.2/vot/dataset/cow.png` & `vot-toolkit-0.6.4/vot/dataset/cow.png`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.2/vot/dataset/dummy.py` & `vot-toolkit-0.6.4/vot/dataset/dummy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,97 @@
+""" Dummy sequences for testing purposes."""
 
 import os
 import math
 import tempfile
 
-from vot.dataset import VOTSequence
+from vot.dataset import BasedSequence
 from vot.region import Rectangle
 from vot.region.io import write_trajectory
 from vot.utilities import write_properties
 
 from PIL import Image
 import numpy as np
 
-class DummySequence(VOTSequence):
+def _generate(base, length, size, objects):
+    """Generate a new dummy sequence.
+    
+    Args:
+        base (str): The base directory for the sequence.
+        length (int): The length of the sequence.
+        size (tuple): The size of the sequence.
+        objects (int): The number of objects in the sequence.
+    """
+
+    background_color = Image.fromarray(np.random.normal(15, 5, (size[1], size[0], 3)).astype(np.uint8))
+    background_depth = Image.fromarray(np.ones((size[1], size[0]), dtype=np.uint8) * 200)
+    background_ir = Image.fromarray(np.zeros((size[1], size[0]), dtype=np.uint8))
+
+    template = Image.open(os.path.join(os.path.dirname(__file__), "cow.png"))
+
+    dir_color = os.path.join(base, "color")
+    dir_depth = os.path.join(base, "depth")
+    dir_ir = os.path.join(base, "ir")
+
+    os.makedirs(dir_color, exist_ok=True)
+    os.makedirs(dir_depth, exist_ok=True)
+    os.makedirs(dir_ir, exist_ok=True)
+
+    path_color = os.path.join(dir_color, "%08d.jpg")
+    path_depth = os.path.join(dir_depth, "%08d.png")
+    path_ir = os.path.join(dir_ir, "%08d.png")
+
+    groundtruth = {i : [] for i in range(objects)}
+
+    center_x = size[0] / 2
+    center_y = size[1] / 2
+
+    radius = min(center_x - template.size[0], center_y - template.size[1])
+
+    speed = (math.pi * 2) / length
+    offset = (math.pi * 2) / objects
+
+    for i in range(length):
+        frame_color = background_color.copy()
+        frame_depth = background_depth.copy()
+        frame_ir = background_ir.copy()
+
+        for o in range(objects):
+
+            x = int(center_x + math.cos(i * speed + offset * o) * radius - template.size[0] / 2)
+            y = int(center_y + math.sin(i * speed + offset * o) * radius - template.size[1] / 2)
+
+            frame_color.paste(template, (x, y), template)
+            frame_depth.paste(10, (x, y), template)
+            frame_ir.paste(240, (x, y), template)
+
+            groundtruth[o].append(Rectangle(x, y, template.size[0], template.size[1]))
+
+        frame_color.save(path_color % (i + 1))
+        frame_depth.save(path_depth % (i + 1))
+        frame_ir.save(path_ir % (i + 1))
+
+    if objects == 1:
+        write_trajectory(os.path.join(base, "groundtruth.txt"), groundtruth[0])
+    else:
+        for i, g in groundtruth.items():
+            write_trajectory(os.path.join(base, "groundtruth_%03d.txt" % i), g)
+
+    metadata = {"name": "dummy", "fps" : 30, "format" : "dummy",
+                        "channel.default": "color"}
+    write_properties(os.path.join(base, "sequence"), metadata)
+
+def generate_dummy(length=100, size=(640, 480), objects=1):
+        """Create a new dummy sequence.
+        
+        Args:
+            length (int, optional): The length of the sequence. Defaults to 100.
+            size (tuple, optional): The size of the sequence. Defaults to (640, 480).
+            objects (int, optional): The number of objects in the sequence. Defaults to 1.
+        """
+        from vot.dataset import load_sequence
 
-    def __init__(self, length=100, size=(640, 480), objects=1):
         base = os.path.join(tempfile.gettempdir(), "vot_dummy_%d_%d_%d_%d" % (length, size[0], size[1], objects))
         if not os.path.isdir(base) or not os.path.isfile(os.path.join(base, "sequence")):
-            DummySequence._generate(base, length, size, objects)
-        super().__init__(base, None)
-
-    @staticmethod
-    def _generate(base, length, size, objects):
-
-        background_color = Image.fromarray(np.random.normal(15, 5, (size[1], size[0], 3)).astype(np.uint8))
-        background_depth = Image.fromarray(np.ones((size[1], size[0]), dtype=np.uint8) * 200)
-        background_ir = Image.fromarray(np.zeros((size[1], size[0]), dtype=np.uint8))
-
-        template = Image.open(os.path.join(os.path.dirname(__file__), "cow.png"))
-
-        dir_color = os.path.join(base, "color")
-        dir_depth = os.path.join(base, "depth")
-        dir_ir = os.path.join(base, "ir")
-
-        os.makedirs(dir_color, exist_ok=True)
-        os.makedirs(dir_depth, exist_ok=True)
-        os.makedirs(dir_ir, exist_ok=True)
-
-        path_color = os.path.join(dir_color, "%08d.jpg")
-        path_depth = os.path.join(dir_depth, "%08d.png")
-        path_ir = os.path.join(dir_ir, "%08d.png")
-
-        groundtruth = {i : [] for i in range(objects)}
-
-        center_x = size[0] / 2
-        center_y = size[1] / 2
-
-        radius = min(center_x - template.size[0], center_y - template.size[1])
-
-        speed = (math.pi * 2) / length
-        offset = (math.pi * 2) / objects
-
-        for i in range(length):
-            frame_color = background_color.copy()
-            frame_depth = background_depth.copy()
-            frame_ir = background_ir.copy()
-
-            for o in range(objects):
-
-                x = int(center_x + math.cos(i * speed + offset * o) * radius - template.size[0] / 2)
-                y = int(center_y + math.sin(i * speed + offset * o) * radius - template.size[1] / 2)
-
-                frame_color.paste(template, (x, y), template)
-                frame_depth.paste(10, (x, y), template)
-                frame_ir.paste(240, (x, y), template)
-
-                groundtruth[o].append(Rectangle(x, y, template.size[0], template.size[1]))
-
-            frame_color.save(path_color % (i + 1))
-            frame_depth.save(path_depth % (i + 1))
-            frame_ir.save(path_ir % (i + 1))
-
-        if objects == 1:
-            write_trajectory(os.path.join(base, "groundtruth.txt"), groundtruth[0])
-        else:
-            for i, g in groundtruth.items():
-                write_trajectory(os.path.join(base, "groundtruth_%03d.txt" % i), g)
-
-        metadata = {"name": "dummy", "fps" : 30, "format" : "dummy",
-                          "channel.default": "color"}
-        write_properties(os.path.join(base, "sequence"), metadata)
+            _generate(base, length, size, objects)
 
+        return load_sequence(base)
```

### Comparing `vot-toolkit-0.6.2/vot/dataset/got10k.py` & `vot-toolkit-0.6.4/vot/dataset/got10k.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,160 +1,128 @@
+""" GOT-10k dataset adapter module. The format of GOT-10k dataset is very similar to a subset of VOT, so there
+is a lot of code duplication."""
 
 import os
 import glob
-import logging
-from collections import OrderedDict
 import configparser
 
 import six
 
 from vot import get_logger
-from vot.dataset import Dataset, DatasetException, BaseSequence, \
+from vot.dataset import DatasetException, BasedSequence, \
      PatternFileListChannel, SequenceData, Sequence
 from vot.region import Special
 from vot.region.io import read_trajectory
-from vot.utilities import Progress
 
 logger = get_logger()
 
 def load_channel(source):
-
+    """ Load channel from the given source.
+    
+    Args:
+        source (str): Path to the source. If the source is a directory, it is
+            assumed to be a pattern file list. If the source is a file, it is
+            assumed to be a video file.
+            
+    Returns:
+        Channel: Channel object.
+    """
     extension = os.path.splitext(source)[1]
 
     if extension == '':
         source = os.path.join(source, '%08d.jpg')
     return PatternFileListChannel(source)
 
-class GOT10kSequence(BaseSequence):
-
-    def __init__(self, base, name=None, dataset=None):
-        self._base = base
-        if name is None:
-            name = os.path.basename(base)
-        super().__init__(name, dataset)
-
-    @staticmethod
-    def check(path: str):
-        return os.path.isfile(os.path.join(path, 'groundtruth.txt')) and not os.path.isfile(os.path.join(path, 'sequence'))
-
-    def _read_metadata(self):
-        metadata = dict(fps=30, format="default")
-
-        if os.path.isfile(os.path.join(self._base, 'meta_info.ini')):
-            config = configparser.ConfigParser()
-            config.read(os.path.join(self._base, 'meta_info.ini'))
-            metadata.update(config["METAINFO"])
-            metadata["fps"] = int(metadata["anno_fps"][:-3])
-
-        metadata["channel.default"] = "color"
-
-        return metadata
-
-    def _read(self):
-
-        channels = {}
-        tags = {}
-        values = {}
-        groundtruth = []
-
-        channels["color"] = load_channel(os.path.join(self._base, "%08d.jpg"))
-        self._metadata["channel.default"] = "color"
-        self._metadata["width"], self._metadata["height"] = six.next(six.itervalues(channels)).size
-
-        groundtruth_file = os.path.join(self._base, self.metadata("groundtruth", "groundtruth.txt"))
-        groundtruth = read_trajectory(groundtruth_file)
-
-        if len(groundtruth) == 1 and channels["color"].length > 1:
-            # We are dealing with testing dataset, only first frame is available, so we pad the
-            # groundtruth with unknowns. Only unsupervised experiment will work, but it is ok
-            groundtruth.extend([Special(Sequence.UNKNOWN)] * (channels["color"].length - 1))
-
-        self._metadata["length"] = len(groundtruth)
-
-        tagfiles = glob.glob(os.path.join(self._base, '*.label'))
-
-        for tagfile in tagfiles:
-            with open(tagfile, 'r') as filehandle:
-                tagname = os.path.splitext(os.path.basename(tagfile))[0]
-                tag = [line.strip() == "1" for line in filehandle.readlines()]
-                while not len(tag) >= len(groundtruth):
-                    tag.append(False)
-                tags[tagname] = tag
-
-        valuefiles = glob.glob(os.path.join(self._base, '*.value'))
-
-        for valuefile in valuefiles:
-            with open(valuefile, 'r') as filehandle:
-                valuename = os.path.splitext(os.path.basename(valuefile))[0]
-                value = [float(line.strip()) for line in filehandle.readlines()]
-                while not len(value) >= len(groundtruth):
-                    value.append(0.0)
-                values[valuename] = value
-
-        for name, channel in channels.items():
-            if not channel.length == len(groundtruth):
-                raise DatasetException("Length mismatch for channel %s" % name)
-
-        for name, tag in tags.items():
-            if not len(tag) == len(groundtruth):
-                tag_tmp = len(groundtruth) * [False]
-                tag_tmp[:len(tag)] = tag
-                tag = tag_tmp
-
-        for name, value in values.items():
-            if not len(value) == len(groundtruth):
-                raise DatasetException("Length mismatch for value %s" % name)
-
-        objects = {"object" : groundtruth}
-
-        return SequenceData(channels, objects, tags, values, len(groundtruth)) 
-
-class GOT10kDataset(Dataset):
-
-    def __init__(self, path, sequence_list="list.txt"):
-        super().__init__(path)
-
-        if not os.path.isabs(sequence_list):
-            sequence_list = os.path.join(path, sequence_list)
-
-        if not os.path.isfile(sequence_list):
-            raise DatasetException("Sequence list does not exist")
-
-        with open(sequence_list, 'r') as handle:
-            names = handle.readlines()
-
-        self._sequences = OrderedDict()
-
-        with Progress("Loading dataset", len(names)) as progress:
-
-            for name in names:
-                self._sequences[name.strip()] = GOT10kSequence(os.path.join(path, name.strip()), dataset=self)
-                progress.relative(1)
-
-    @staticmethod
-    def check(path: str):
-        if not os.path.isfile(os.path.join(path, 'list.txt')):
-            return False
-
-        with open(os.path.join(path, 'list.txt'), 'r') as handle:
-            sequence = handle.readline().strip()
-            return GOT10kSequence.check(os.path.join(path, sequence))
-
-    @property
-    def path(self):
-        return self._path
-
-    @property
-    def length(self):
-        return len(self._sequences)
 
-    def __getitem__(self, key):
-        return self._sequences[key]
+def _read_data(metadata):
+    """ Read data from the given metadata.
+    
+    Args:
+        metadata (dict): Metadata dictionary.
+    """
+    channels = {}
+    tags = {}
+    values = {}
+    groundtruth = []
+
+    base = metadata["root"]
+
+    channels["color"] = load_channel(os.path.join(base, "%08d.jpg"))
+    metadata["channel.default"] = "color"
+    metadata["width"], metadata["height"] = six.next(six.itervalues(channels)).size
+
+    groundtruth_file = os.path.join(base, metadata.get("groundtruth", "groundtruth.txt"))
+    groundtruth = read_trajectory(groundtruth_file)
+
+    if len(groundtruth) == 1 and channels["color"].length > 1:
+        # We are dealing with testing dataset, only first frame is available, so we pad the
+        # groundtruth with unknowns. Only unsupervised experiment will work, but it is ok
+        groundtruth.extend([Special(Sequence.UNKNOWN)] * (channels["color"].length - 1))
+
+    metadata["length"] = len(groundtruth)
+
+    tagfiles = glob.glob(os.path.join(base, '*.label'))
+
+    for tagfile in tagfiles:
+        with open(tagfile, 'r') as filehandle:
+            tagname = os.path.splitext(os.path.basename(tagfile))[0]
+            tag = [line.strip() == "1" for line in filehandle.readlines()]
+            while not len(tag) >= len(groundtruth):
+                tag.append(False)
+            tags[tagname] = tag
+
+    valuefiles = glob.glob(os.path.join(base, '*.value'))
+
+    for valuefile in valuefiles:
+        with open(valuefile, 'r') as filehandle:
+            valuename = os.path.splitext(os.path.basename(valuefile))[0]
+            value = [float(line.strip()) for line in filehandle.readlines()]
+            while not len(value) >= len(groundtruth):
+                value.append(0.0)
+            values[valuename] = value
+
+    for name, channel in channels.items():
+        if not channel.length == len(groundtruth):
+            raise DatasetException("Length mismatch for channel %s" % name)
+
+    for name, tag in tags.items():
+        if not len(tag) == len(groundtruth):
+            tag_tmp = len(groundtruth) * [False]
+            tag_tmp[:len(tag)] = tag
+            tag = tag_tmp
+
+    for name, value in values.items():
+        if not len(value) == len(groundtruth):
+            raise DatasetException("Length mismatch for value %s" % name)
+
+    objects = {"object" : groundtruth}
+
+    return SequenceData(channels, objects, tags, values, len(groundtruth)) 
+
+from vot.dataset import sequence_reader
+
+@sequence_reader.register("GOT-10k")
+def read_sequence(path):
+    """ Read GOT-10k sequence from the given path.
+    
+    Args:
+        path (str): Path to the sequence.
+    """
+
+    if not (os.path.isfile(os.path.join(path, 'groundtruth.txt')) and os.path.isfile(os.path.join(path, 'meta_info.ini'))):
+        return None
+
+    metadata = dict(fps=30, format="default")
+
+    if os.path.isfile(os.path.join(path, 'meta_info.ini')):
+        config = configparser.ConfigParser()
+        config.read(os.path.join(path, 'meta_info.ini'))
+        metadata.update(config["METAINFO"])
+        metadata["fps"] = int(metadata["anno_fps"][:-3])
+
+    metadata["root"] = path
+    metadata["name"] = os.path.basename(path)
+    metadata["channel.default"] = "color"
 
-    def __contains__(self, key):
-        return key in self._sequences
+    return BasedSequence(metadata["name"], _read_data, metadata)
 
-    def __iter__(self):
-        return self._sequences.values().__iter__()
 
-    def list(self):
-        return list(self._sequences.keys())
```

### Comparing `vot-toolkit-0.6.2/vot/dataset/otb.py` & `vot-toolkit-0.6.4/vot/dataset/otb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+""" OTB dataset adapter module. OTB is one of the earliest tracking benchmarks. It is a collection of 50/100 sequences 
+with ground truth annotations. The dataset is available at http://cvlab.hanyang.ac.kr/tracker_benchmark/datasets.html.
+"""
 
-from collections import OrderedDict
 import os
-import logging
 import six
 
 from vot import get_logger
-from vot.dataset import BaseSequence, Dataset, DatasetException, PatternFileListChannel, SequenceData
+from vot.dataset import BasedSequence, DatasetException, PatternFileListChannel, SequenceData
 from vot.utilities import Progress
 from vot.region.io import parse_region
 
 logger = get_logger()
 
 _BASE_URL = "http://cvlab.hanyang.ac.kr/tracker_benchmark/seq/"
 
@@ -120,129 +121,114 @@
     "Tiger1": {"attributes": ["IV", "OCC", "DEF", "MB", "FM", "IPR", "OPR"]},
     "Toy": {"attributes": ["SV", "FM", "IPR", "OPR"]},
     "Trans": {"attributes": ["IV", "SV", "OCC", "DEF"]},
     "Twinnings": {"attributes": ["SV", "OPR"]},
     "Vase": {"attributes": ["SV", "FM", "IPR"]},
 }
 
-class OTBSequence(BaseSequence):
+def _load_sequence(metadata):
+    """Load a sequence from the OTB dataset.
+    
+    Args:
+        metadata (dict): Sequence metadata.
+    """
 
-    def __init__(self, root, name=None, dataset=None):
-        super().__init__(name or os.path.basename(root), dataset)
-        self._base = root
+    channels = {}
+    groundtruth = []
 
-    @staticmethod
-    def check(path: str):
-        return os.path.isfile(os.path.join(path, 'groundtruth_rect.txt'))
+    attributes = metadata.get("attributes", {})
 
-    def _read_metadata(self):
-        metadata = _SEQUENCES[self.name]
-        return {"attributes": metadata["attributes"]}
+    channels["color"] = PatternFileListChannel(os.path.join(metadata["path"], "img", "%%0%dd.jpg" % attributes.get("zeros", 4)),
+        start=attributes.get("start", 1), end=attributes.get("stop", None))
 
-    def _read(self):
+    metadata["channel.default"] = "color"
+    metadata["width"], metadata["height"] = six.next(six.itervalues(channels)).size
 
-        channels = {}
-        groundtruth = []
+    groundtruth_file = os.path.join(metadata["path"], attributes.get("groundtruth", "groundtruth_rect.txt"))
 
-        metadata = _SEQUENCES[self.name]
+    with open(groundtruth_file, 'r') as filehandle:
+        for region in filehandle.readlines():
+            groundtruth.append(parse_region(region.replace("\t", ",").replace(" ", ",")))
 
-        channels["color"] = PatternFileListChannel(os.path.join(self._base, "img", "%%0%dd.jpg" % metadata.get("zeros", 4)),
-            start=metadata.get("start", 1), end=metadata.get("stop", None))
+    metadata["length"] = len(groundtruth)
 
-        self._metadata["channel.default"] = "color"
-        self._metadata["width"], self._metadata["height"] = six.next(six.itervalues(channels)).size
+    if not len(channels["color"]) == len(groundtruth):
+        raise DatasetException("Length mismatch between groundtruth and images %d != %d" % (len(channels["color"]), len(groundtruth)))
+    
+    objects = {"object" : groundtruth}
 
-        groundtruth_file = os.path.join(self._base, metadata.get("groundtruth", "groundtruth_rect.txt"))
+    return SequenceData(channels, objects, {}, {}, len(groundtruth)) 
 
-        with open(groundtruth_file, 'r') as filehandle:
-            for region in filehandle.readlines():
-                groundtruth.append(parse_region(region.replace("\t", ",").replace(" ", ",")))
+from vot.dataset import sequence_reader
 
-        self._metadata["length"] = len(groundtruth)
+@sequence_reader.register("otb")
+def read_sequence(path: str):
+    """Reads a sequence from OTB dataset. The sequence is identified by the name of the folder and the
+    groundtruth_rect.txt file is expected to be present in the folder.
+    
+    Args:
+        path (str): Path to the sequence folder.
+    
+    Returns:
+        Sequence: The sequence object.
+    """
 
-        if not channels["color"].length == len(groundtruth):
-            raise DatasetException("Length mismatch between groundtruth and images %d != %d" % (channels["color"].length, len(groundtruth)))
-        
-        objects = {"object" : groundtruth}
+    if not os.path.isfile(os.path.join(path, 'groundtruth_rect.txt')):
+        return None
 
-        return SequenceData(channels, objects, {}, {}, len(groundtruth)) 
+    name = os.path.basename(path)
 
-class OTBDataset(Dataset):
+    if name not in _SEQUENCES:
+        return None
 
-    def __init__(self, path):
-        super().__init__(path)
+    metadata =  {"attributes": _SEQUENCES[name], "path": path}
+    return BasedSequence(name.strip(), _load_sequence, metadata)
 
-        dataset = _SEQUENCES
+from vot.dataset import dataset_downloader
 
-        if not OTBDataset.check(path):
-            raise DatasetException("Unknown dataset format, expected OTB")
-
-        otb50 = all([not OTBSequence.check(os.path.join(path, sequence)) for sequence in dataset.keys() - _OTB50_SUBSET])
-
-        if otb50:
-            logger.debug("Loading OTB-50 dataset")
-        else:
-            logger.debug("Loading OTB-100 dataset")
-
-        if otb50:
-            dataset = {k: v for k, v in dataset.items() if k in _OTB50_SUBSET}
-
-        self._sequences = OrderedDict()
-
-        with Progress("Loading dataset", len(dataset)) as progress:
-
-            for name in sorted(list(dataset.keys())):
-                self._sequences[name.strip()] = OTBSequence(os.path.join(path, name), name, dataset=self)
-                progress.relative(1)
-
-    @staticmethod
-    def check(path: str):
-        for sequence in _OTB50_SUBSET:
-            return OTBSequence.check(os.path.join(path, sequence))
-
-
-    @property
-    def path(self):
-        return self._path
-
-    @property
-    def length(self):
-        return len(self._sequences)
-
-    def __getitem__(self, key):
-        return self._sequences[key]
-
-    def __contains__(self, key):
-        return key in self._sequences
-
-    def __iter__(self):
-        return self._sequences.values().__iter__()
-
-    def list(self):
-        return list(self._sequences.keys())
+@dataset_downloader.register("otb50")
+def download_otb50(path: str):
+    """Downloads OTB50 dataset to the given path.
+    
+    Args:
+        path (str): Path to the dataset folder.
+    """
+    dataset = _SEQUENCES
+    dataset = {k: v for k, v in dataset.items() if k in _OTB50_SUBSET}
+    _download_dataset(path, dataset)
 
+@dataset_downloader.register("otb100")
+def download_otb100(path: str):
+    """Downloads OTB100 dataset to the given path.
+    
+    Args:
+        path (str): Path to the dataset folder.
+    """
+    dataset = _SEQUENCES
+    _download_dataset(path, dataset)
 
-def download_dataset(path: str, otb50: bool = False):
+def _download_dataset(path: str, dataset: dict):
+    """Downloads the given dataset to the given path.
+    
+    Args:
+        path (str): Path to the dataset folder.
+    """
 
     from vot.utilities.net import download_uncompress, join_url, NetworkException
 
-    dataset = _SEQUENCES
-
-    if otb50:
-        dataset = {k: v for k, v in dataset.items() if k in _OTB50_SUBSET}
-
     with Progress("Downloading", len(dataset)) as progress:
         for name, metadata in dataset.items():
             name = metadata.get("base", name)
             if not os.path.isdir(os.path.join(path, name)):
                 try:
                     download_uncompress(join_url(_BASE_URL, "%s.zip" % name), path)
                 except NetworkException as ex:
                     raise DatasetException("Unable do download sequence data") from ex
                 except IOError as ex:
                     raise DatasetException("Unable to extract sequence data, is the target directory writable and do you have enough space?") from ex
 
             progress.relative(1)
 
-
-if __name__ == "__main__":
-    download_dataset("")
+    # Write sequence list to a list.txt file
+    with open(os.path.join(path, "list.txt"), 'w') as filehandle:
+        for name in dataset.keys():
+            filehandle.write("%s\n" % name)
```

### Comparing `vot-toolkit-0.6.2/vot/dataset/vot.py` & `vot-toolkit-0.6.4/vot/dataset/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,173 +1,207 @@
+"""This module contains functionality for reading sequences from the storage using VOT compatible format."""
 
 import os
 import glob
 import logging
-from collections import OrderedDict
 
 import six
 
 import cv2
 
-from vot.dataset import Dataset, DatasetException, Sequence, BaseSequence, PatternFileListChannel, SequenceData
+from vot.dataset import Dataset, DatasetException, Sequence, BasedSequence, PatternFileListChannel, SequenceData
 from vot.region.io import write_trajectory, read_trajectory
 from vot.region import Special
 from vot.utilities import Progress, localize_path, read_properties, write_properties
 
 logger = logging.getLogger("vot")
 
-def load_channel(source):
+def convert_int(value: str) -> int:
+    """Converts the given value to an integer. If the value is not a valid integer, None is returned.
+    
+    Args:
+        value (str): The value to convert.
+    
+    Returns:
+        int: The converted value or None if the value is not a valid integer.
+    """
+    try:
+        if value is None:
+            return None
+        return int(value)
+    except ValueError:
+        return None
+    
+def _load_channel(source, length=None):
+    """Loads a channel from the given source.
+
+    Args:
+        source (str): The source to load the channel from.
+        length (int): The length of the channel. If not specified, the channel is loaded from a pattern file list.
+
+    Returns:
+        Channel: The loaded channel.
+    """
 
     extension = os.path.splitext(source)[1]
 
     if extension == '':
         source = os.path.join(source, '%08d.jpg')
-    return PatternFileListChannel(source)
+    return PatternFileListChannel(source, end=length, check_files=length is None)
 
-class VOTSequence(BaseSequence):
-
-    def __init__(self, base, name=None, dataset=None):
-        self._base = base
-        if name is None:
-            name = os.path.basename(base)
-        super().__init__(name, dataset)
-
-    @staticmethod
-    def check(path):
-        return os.path.isfile(os.path.join(path, 'sequence'))
-
-    def _read_metadata(self):
-        metadata = dict(fps=30, format="default")
-        metadata["channel.default"] = "color"
-
-        metadata_file = os.path.join(self._base, 'sequence')
-        metadata.update(read_properties(metadata_file))
-
-        return metadata
-
-    def _read(self):
-
-        channels = {}
-        tags = {}
-        values = {}
-
-        for c in ["color", "depth", "ir"]:
-            channel_path = self.metadata("channels.%s" % c, None)
-            if not channel_path is None:
-                channels[c] = load_channel(os.path.join(self._base, localize_path(channel_path)))
-
-        # Load default channel if no explicit channel data available
-        if len(channels) == 0:
-            channels["color"] = load_channel(os.path.join(self._base, "color", "%08d.jpg"))
-        else:
-            self._metadata["channel.default"] = next(iter(channels.keys()))
-
-        self._metadata["width"], self._metadata["height"] = six.next(six.itervalues(channels)).size
-
-        lenghts = [len(t) for t in channels.values()]
-        assert all([x == lenghts[0] for x in lenghts]), "Sequence channels have different lengths"
-        length = lenghts[0]
-
-        objectsfiles = glob.glob(os.path.join(self._base, 'groundtruth_*.txt'))
-        objects = {}
-        if len(objectsfiles) > 0:
-            for objectfile in objectsfiles:
-                groundtruth = read_trajectory(os.path.join(objectfile))
-                if len(groundtruth) < length: groundtruth += [Special(Sequence.UNKNOWN)] * (length - len(groundtruth))
-                objectid = os.path.basename(objectfile)[12:-4]
-                objects[objectid] = groundtruth
-        else:
-            groundtruth_file = os.path.join(self._base, self.metadata("groundtruth", "groundtruth.txt"))
-            groundtruth = read_trajectory(groundtruth_file)
-            if len(groundtruth) < length: groundtruth += [Special(Sequence.UNKNOWN)] * (length - len(groundtruth))
-            objects["object"] = groundtruth
-
-        self._metadata["length"] = length
-
-        tagfiles = glob.glob(os.path.join(self._base, '*.tag')) + glob.glob(os.path.join(self._base, '*.label'))
-
-        for tagfile in tagfiles:
-            with open(tagfile, 'r') as filehandle:
-                tagname = os.path.splitext(os.path.basename(tagfile))[0]
-                tag = [line.strip() == "1" for line in filehandle.readlines()]
-                while not len(tag) >= length:
-                    tag.append(False)
-                tags[tagname] = tag
-
-        valuefiles = glob.glob(os.path.join(self._base, '*.value'))
-
-        for valuefile in valuefiles:
-            with open(valuefile, 'r') as filehandle:
-                valuename = os.path.splitext(os.path.basename(valuefile))[0]
-                value = [float(line.strip()) for line in filehandle.readlines()]
-                while not len(value) >= length:
-                    value.append(0.0)
-                values[valuename] = value
-
-        for name, tag in tags.items():
-            if not len(tag) == length:
-                tag_tmp = length * [False]
-                tag_tmp[:len(tag)] = tag
-                tag = tag_tmp
-
-        for name, value in values.items():
-            if not len(value) == length:
-                raise DatasetException("Length mismatch for value %s" % name)
-
-        return SequenceData(channels, objects, tags, values, length) 
-
-class VOTDataset(Dataset):
-
-    def __init__(self, path):
-        super().__init__(path)
-
-        if not os.path.isfile(os.path.join(path, "list.txt")):
-            raise DatasetException("Dataset not available locally")
-
-        with open(os.path.join(path, "list.txt"), 'r') as fd:
-            names = fd.readlines()
-
-        self._sequences = OrderedDict()
-
-        with Progress("Loading dataset", len(names)) as progress:
-
-            for name in names:
-                self._sequences[name.strip()] = VOTSequence(os.path.join(path, name.strip()), dataset=self)
-                progress.relative(1)
-
-    @staticmethod
-    def check(path: str):
-        if not os.path.isfile(os.path.join(path, 'list.txt')):
-            return False
-
-        with open(os.path.join(path, 'list.txt'), 'r') as handle:
-            sequence = handle.readline().strip()
-            return VOTSequence.check(os.path.join(path, sequence))
-
-    @property
-    def path(self):
-        return self._path
-
-    @property
-    def length(self):
-        return len(self._sequences)
-
-    def __getitem__(self, key):
-        return self._sequences[key]
-
-    def __contains__(self, key):
-        return key in self._sequences
-
-    def __iter__(self):
-        return self._sequences.values().__iter__()
+def _read_data(metadata):
+    """Reads data from the given metadata.
+    
+    Args:
+        metadata (dict): The metadata to read data from.
+        
+    Returns:
+        dict: The data read from the metadata.
+    """
+
+    channels = {}
+    tags = {}
+    values = {}
+    length = metadata["length"]
+
+    root = metadata["root"]
+
+    for c in ["color", "depth", "ir"]:
+        channel_path = metadata.get("channels.%s" % c, None)
+        if not channel_path is None:
+            channels[c] = _load_channel(os.path.join(root, localize_path(channel_path)), length)
+
+    # Load default channel if no explicit channel data available
+    if len(channels) == 0:
+        channels["color"] = _load_channel(os.path.join(root, "color", "%08d.jpg"), length=length) 
+    else:
+        metadata["channel.default"] = next(iter(channels.keys()))
 
-    def list(self):
-        return list(self._sequences.keys())
+    if metadata.get("width", None) is None or metadata.get("height", None) is None:
+        metadata["width"], metadata["height"] = six.next(six.itervalues(channels)).size
 
-def download_dataset_meta(url, path):
+    lengths = [len(t) for t in channels.values()]
+    assert all([x == lengths[0] for x in lengths]), "Sequence channels have different lengths"
+    length = lengths[0]
+
+    objectsfiles = glob.glob(os.path.join(root, 'groundtruth_*.txt'))
+    objects = {}
+    if len(objectsfiles) > 0:
+        for objectfile in objectsfiles:
+            groundtruth = read_trajectory(os.path.join(objectfile))
+            if len(groundtruth) < length: groundtruth += [Special(Sequence.UNKNOWN)] * (length - len(groundtruth))
+            objectid = os.path.basename(objectfile)[12:-4]
+            objects[objectid] = groundtruth
+    else:
+        groundtruth_file = os.path.join(root, metadata.get("groundtruth", "groundtruth.txt"))
+        groundtruth = read_trajectory(groundtruth_file)
+        if len(groundtruth) < length: groundtruth += [Special(Sequence.UNKNOWN)] * (length - len(groundtruth))
+        objects["object"] = groundtruth
+
+    metadata["length"] = length
+
+    tagfiles = glob.glob(os.path.join(root, '*.tag')) + glob.glob(os.path.join(root, '*.label'))
+
+    for tagfile in tagfiles:
+        with open(tagfile, 'r') as filehandle:
+            tagname = os.path.splitext(os.path.basename(tagfile))[0]
+            tag = [line.strip() == "1" for line in filehandle.readlines()]
+            while not len(tag) >= length:
+                tag.append(False)
+            tags[tagname] = tag
+
+    valuefiles = glob.glob(os.path.join(root, '*.value'))
+
+    for valuefile in valuefiles:
+        with open(valuefile, 'r') as filehandle:
+            valuename = os.path.splitext(os.path.basename(valuefile))[0]
+            value = [float(line.strip()) for line in filehandle.readlines()]
+            while not len(value) >= length:
+                value.append(0.0)
+            values[valuename] = value
+
+    for name, tag in tags.items():
+        if not len(tag) == length:
+            tag_tmp = length * [False]
+            tag_tmp[:len(tag)] = tag
+            tag = tag_tmp
+
+    for name, value in values.items():
+        if not len(value) == length:
+            raise DatasetException("Length mismatch for value %s" % name)
+
+    return SequenceData(channels, objects, tags, values, length) 
+
+def _read_metadata(path):
+    """Reads metadata from the given path. The metadata is read from the sequence file in the given path.
+    
+    Args:
+        path (str): The path to read metadata from.
+        
+    Returns:
+        dict: The metadata read from the given path.
+    """
+    metadata = dict(fps=30, format="default")
+    metadata["channel.default"] = "color"
+
+    metadata_file = os.path.join(path, 'sequence')
+    metadata.update(read_properties(metadata_file))
+
+    metadata["height"] = convert_int(metadata.get("height", None))
+    metadata["width"] = convert_int(metadata.get("width", None))
+    metadata["length"] = convert_int(metadata.get("length", None))
+    metadata["fps"] = convert_int(metadata.get("fps", None))
+
+    metadata["root"] = path
+
+    return metadata
+
+from vot.dataset import sequence_reader
+
+@sequence_reader.register("default")
+def read_sequence(path):
+    """Reads a sequence from the given path.
+
+    Args:
+        path (str): The path to read the sequence from.
+
+    Returns:
+        Sequence: The sequence read from the given path.
+    """
+    if not os.path.isfile(os.path.join(path, "sequence")):
+        return None
+
+    return BasedSequence(os.path.basename(path), _read_data, _read_metadata(path))
+
+def read_sequence_legacy(path):
+    """Reads a sequence from the given path.
+
+    Args:
+        path (str): The path to read the sequence from.
+
+    Returns:
+        Sequence: The sequence read from the given path.
+    """
+    if not os.path.isfile(os.path.join(path, "groundtruth.txt")):
+        return None
+
+    metadata = dict(fps=30, format="default")
+    metadata["channel.default"] = "color"
+    metadata["channel.color"] = "%08d.jpg"
+
+    return BasedSequence(os.path.basename(path), _read_data, metadata=metadata)
+
+def download_dataset_meta(url: str, path: str) -> None:
+    """Downloads the metadata of a dataset from a given URL and stores it in the given path.
+    
+    Args:
+        url (str): The URL to download the metadata from.
+        path (str): The path to store the metadata in.
+        
+    """
     from vot.utilities.net import download_uncompress, download_json, get_base_url, join_url, NetworkException
     from vot.utilities import format_size
 
     meta = download_json(url)
 
     total_size = 0
     for sequence in meta["sequences"]:
@@ -184,15 +218,15 @@
     with Progress("Downloading", len(meta["sequences"])) as progress:
         for sequence in meta["sequences"]:
             sequence_directory = os.path.join(path, sequence["name"])
             os.makedirs(sequence_directory, exist_ok=True)
 
             if os.path.isfile(os.path.join(sequence_directory, "sequence")):
                 refdata = read_properties(os.path.join(sequence_directory, "sequence"))
-                if refdata["uid"] == sequence["annotations"]["uid"]:
+                if "uid" in refdata and refdata["uid"] == sequence["annotations"]["uid"]:
                     logger.info('Sequence "%s" already downloaded.', sequence["name"])
                     progress.relative(1)
                     continue
 
             data = {'name': sequence["name"], 'fps': sequence["fps"], 'format': 'default'}
 
             annotations_url = join_url(base_url, sequence["annotations"]["url"])
@@ -246,36 +280,44 @@
     else:
         logger.info('Successfully downloaded all sequences.')
         with open(os.path.join(path, "list.txt"), "w") as fp:
             for sequence in meta["sequences"]:
                 fp.write('{}\n'.format(sequence["name"]))
 
 def write_sequence(directory: str, sequence: Sequence):
+    """Writes a sequence to a directory. The sequence is written as a set of images in a directory structure
+    corresponding to the channel names. The sequence metadata is written to a file called sequence in the root
+    directory.
+    
+    Args:
+        directory (str): The directory to write the sequence to.
+        sequence (Sequence): The sequence to write.
+    """
 
     channels = sequence.channels()
 
     metadata = dict()
     metadata["channel.default"] = sequence.metadata("channel.default", "color")
     metadata["fps"] = sequence.metadata("fps", "30")
 
     for channel in channels:
         cdir = os.path.join(directory, channel)
         os.makedirs(cdir, exist_ok=True)
 
         metadata["channels.%s" % channel] = os.path.join(channel, "%08d.jpg")
 
-        for i in range(sequence.length):
+        for i in range(len(sequence)):
             frame = sequence.frame(i).channel(channel)
             cv2.imwrite(os.path.join(cdir, "%08d.jpg" % (i + 1)), cv2.cvtColor(frame, cv2.COLOR_RGB2BGR))
 
     for tag in sequence.tags():
-        data = "\n".join(["1" if tag in sequence.tags(i) else "0" for i in range(sequence.length)])
+        data = "\n".join(["1" if tag in sequence.tags(i) else "0" for i in range(len(sequence))])
         with open(os.path.join(directory, "%s.tag" % tag), "w") as fp:
             fp.write(data)
 
     for value in sequence.values():
-        data = "\n".join([ str(sequence.values(i).get(value, "")) for i in range(sequence.length)])
+        data = "\n".join([ str(sequence.values(i).get(value, "")) for i in range(len(sequence))])
         with open(os.path.join(directory, "%s.value" % value), "w") as fp:
             fp.write(data)
 
     write_trajectory(os.path.join(directory, "groundtruth.txt"), [f.groundtruth() for f in sequence])
     write_properties(os.path.join(directory, "sequence"), metadata)
```

### Comparing `vot-toolkit-0.6.2/vot/document/__init__.py` & `vot-toolkit-0.6.4/vot/document/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+""" This module contains classes for generating reports and visualizations. """
 
-import os
 import typing
 from abc import ABC, abstractmethod
 import json
 import inspect
 import threading
 import datetime
 import collections
@@ -27,17 +27,28 @@
 from vot.dataset import Sequence
 from vot.tracker import Tracker
 from vot.analysis import Axes
 from vot.utilities import class_fullname
 from vot.utilities.data import Grid
 
 class Plot(object):
+    """ Base class for all plots. """
 
     def __init__(self, identifier: str, xlabel: str, ylabel: str,
         xlimits: typing.Tuple[float, float], ylimits: typing.Tuple[float, float], trait = None):
+        """ Initializes the plot.
+        
+        Args:
+            identifier (str): The identifier of the plot.
+            xlabel (str): The label of the x axis.
+            ylabel (str): The label of the y axis.
+            xlimits (tuple): The limits of the x axis.
+            ylimits (tuple): The limits of the y axis.
+            trait (str): The trait of the plot.    
+        """
 
         self._identifier = identifier
 
         self._manager = StyleManager.default()
 
         self._figure, self._axes = self._manager.make_figure(trait)
 
@@ -48,43 +59,52 @@
             self._axes.set_xlim(xlimits)
             self._axes.autoscale(False, axis="x")
         if not ylimits is None and not any([y is None for y in ylimits]):
             self._axes.set_ylim(ylimits)
             self._axes.autoscale(False, axis="y")
 
     def __call__(self, key, data):
+        """ Draws the data on the plot."""
         self.draw(key, data)
 
     def draw(self, key, data):
+        """ Draws the data on the plot."""
         raise NotImplementedError
     
     @property
     def axes(self) -> Axes:
+        """ Returns the axes of the plot."""
         return self._axes
 
     def save(self, output, fmt):
+        """ Saves the plot to a file."""
         self._figure.savefig(output, format=fmt, bbox_inches='tight', transparent=True)
 
     @property
     def identifier(self):
+        """ Returns the identifier of the plot."""
         return self._identifier
 
 class ScatterPlot(Plot):
+    """ A scatter plot."""
 
     def draw(self, key, data):
+        """ Draws the data on the plot. """
         if data is None or len(data) != 2:
             return
 
         style = self._manager.plot_style(key)
         handle = self._axes.scatter(data[0], data[1], **style.point_style())
         #handle.set_gid("report_%s_%d" % (self._identifier, style["number"]))
 
 class LinePlot(Plot):
+    """ A line plot."""
 
     def draw(self, key, data):
+        """ Draws the data on the plot."""
         if data is None or len(data) < 1:
             return
 
         if isinstance(data[0], tuple):
             # Drawing curve
             if len(data[0]) != 2:
                 return
@@ -95,32 +115,37 @@
 
         style = self._manager.plot_style(key)
 
         handle = self._axes.plot(x, y, **style.line_style())
        # handle[0].set_gid("report_%s_%d" % (self._identifier, style["number"]))
 
 class ResultsJSONEncoder(json.JSONEncoder):
+    """ JSON encoder for results. """
 
     def default(self, o):
+        """ Default encoder. """
         if isinstance(o, Grid):
             return list(o)
         elif isinstance(o, datetime.date):
             return o.strftime('%Y/%m/%d')
         elif isinstance(o, np.ndarray):
             return o.tolist()
         else:
             return super().default(o)
 
 class ResultsYAMLEncoder(yaml.Dumper):
+    """ YAML encoder for results."""
 
     def represent_tuple(self, data):
+        """ Represents a tuple. """
         return self.represent_list(list(data))
 
 
     def represent_object(self, o):
+        """ Represents an object. """
         if isinstance(o, Grid):
             return self.represent_list(list(o))
         elif isinstance(o, datetime.date):
             return o.strftime('%Y/%m/%d')
         elif isinstance(o, np.ndarray):
             return self.represent_list(o.tolist())
         else:
@@ -130,14 +155,15 @@
 ResultsYAMLEncoder.add_representer(tuple, ResultsYAMLEncoder.represent_tuple)
 ResultsYAMLEncoder.add_representer(Grid, ResultsYAMLEncoder.represent_object)
 ResultsYAMLEncoder.add_representer(np.ndarray, ResultsYAMLEncoder.represent_object)
 ResultsYAMLEncoder.add_multi_representer(np.integer, ResultsYAMLEncoder.represent_int)
 ResultsYAMLEncoder.add_multi_representer(np.inexact, ResultsYAMLEncoder.represent_float)
 
 def generate_serialized(trackers: typing.List[Tracker], sequences: typing.List[Sequence], results, storage: "Storage", serializer: str):
+    """ Generates a serialized report of the results.  """
 
     doc = dict()
     doc["toolkit"] = version
     doc["timestamp"] = datetime.datetime.now().isoformat()
     doc["trackers"] = {t.reference : t.describe() for t in trackers}
     doc["sequences"] = {s.name : s.describe() for s in sequences}
 
@@ -156,169 +182,230 @@
     elif serializer == "yaml":
         with storage.write("results.yaml") as handle:
             yaml.dump(doc, handle, Dumper=ResultsYAMLEncoder)
     else:
         raise RuntimeError("Unknown serializer")
 
 def configure_axes(figure, rect=None, _=None):
+    """ Configures the axes of the plot. """
 
     axes = PlotAxes(figure, rect or [0, 0, 1, 1])
 
     figure.add_axes(axes)
 
     return axes
 
 def configure_figure(traits=None):
+    """ Configures the figure of the plot. """
 
     args = {}
     if traits == "ar":
         args["figsize"] = (5, 5)
     elif traits == "eao":
         args["figsize"] = (7, 5)
     elif traits == "attributes":
         args["figsize"] = (10, 5)
 
     return Figure(**args)
 
 class PlotStyle(object):
+    """ A style for a plot."""
 
     def line_style(self, opacity=1):
+        """ Returns the style for a line."""
         raise NotImplementedError
 
     def point_style(self):
+        """ Returns the style for a point."""
         raise NotImplementedError
 
 class DefaultStyle(PlotStyle):
+    """ The default style for a plot."""
 
     colormap = get_cmap("tab20b")
     colorcount = 20
     markers = ["o", "v", "<", ">", "^", "8", "*"]
 
     def __init__(self, number):
+        """ Initializes the style. 
+        
+        Args:
+            number (int): The number of the style.
+        """
         super().__init__()
         self._number = number
 
     def line_style(self, opacity=1):
+        """ Returns the style for a line.
+        
+        Args:
+            opacity (float): The opacity of the line.
+        """
         color = DefaultStyle.colormap((self._number % DefaultStyle.colorcount + 1) / DefaultStyle.colorcount)
         if opacity < 1:
             color = colors.to_rgba(color, opacity)
         return dict(linewidth=1, c=color)
 
     def point_style(self):
+        """ Returns the style for a point.
+        
+        Args:
+            color (str): The color of the point.
+            opacity (float): The opacity of the line.
+        """
         color = DefaultStyle.colormap((self._number % DefaultStyle.colorcount + 1) / DefaultStyle.colorcount)
         marker = DefaultStyle.markers[self._number % len(DefaultStyle.markers)]
         return dict(marker=marker, c=[color])
 
 class Legend(object):
+    """ A legend for a plot."""
 
     def __init__(self, style_factory=DefaultStyle):
+        """ Initializes the legend.
+        
+        Args:
+            style_factory (PlotStyleFactory): The style factory.
+        """
         self._mapping = collections.OrderedDict()
         self._counter = 0
         self._style_factory = style_factory
 
     def _number(self, key):
+        """ Returns the number for a key."""
         if not key in self._mapping:
             self._mapping[key] = self._counter
             self._counter += 1
         return self._mapping[key]
 
     def __getitem__(self, key) -> PlotStyle:
+        """ Returns the style for a key."""
         number = self._number(key)
         return self._style_factory(number)
 
     def _style(self, number):
+        """ Returns the style for a number."""
         raise NotImplementedError
 
     def keys(self):
+        """ Returns the keys of the legend."""
         return self._mapping.keys()
 
     def figure(self, key):
+        """ Returns a figure for a key."""
         style = self[key]
         figure = Figure(figsize=(0.1, 0.1))  # TODO: hardcoded
         axes = PlotAxes(figure, [0, 0, 1, 1], yticks=[], xticks=[], frame_on=False)
         figure.add_axes(axes)
         axes.patch.set_visible(False)
         marker_style = style.point_style()
         marker_style["s"] = 40 # Reset size
         axes.scatter(0, 0, **marker_style)
         return figure
 
 class StyleManager(Attributee):
+    """ A manager for styles. """
 
     plots = Callable(default=DefaultStyle)
     axes = Callable(default=configure_axes)
     figure = Callable(default=configure_figure)
 
     _context = threading.local()
 
     def __init__(self, **kwargs):
+        """ Initializes a new instance of the StyleManager class."""
         super().__init__(**kwargs)
         self._legends = dict()
 
     def __getitem__(self, key) -> PlotStyle:
+        """ Gets the style for the given key."""
         return self.plot_style(key)
 
     def legend(self, key) -> Legend:
+        """ Gets the legend for the given key."""
         if inspect.isclass(key):
             klass = key
         else:
             klass = type(key)
 
         if not klass in self._legends:
             self._legends[klass] = Legend(self.plots)
 
         return self._legends[klass]
 
     def plot_style(self, key) -> PlotStyle:
+        """ Gets the plot style for the given key."""
         return self.legend(key)[key]
 
     def make_axes(self, figure, rect=None, trait=None) -> Axes:
+        """ Makes the axes for the given figure."""
         return self.axes(figure, rect, trait)
 
     def make_figure(self, trait=None) -> typing.Tuple[Figure, Axes]:
+        """ Makes the figure for the given trait.
+        
+        Args:
+            trait: The trait for which to make the figure.
+
+        Returns:
+            A tuple containing the figure and the axes.
+        """
         figure = self.figure(trait)
         axes = self.make_axes(figure, trait=trait)
 
         return figure, axes
 
     def __enter__(self):
+        """Enters the context of the style manager."""
 
         manager = getattr(StyleManager._context, 'style_manager', None)
 
         if manager == self:
             return self
 
         StyleManager._context.style_manager = self
 
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
+        """Exits the context of the style manager."""
         manager = getattr(StyleManager._context, 'style_manager', None)
 
         if manager == self:
             StyleManager._context.style_manager = None
 
     @staticmethod
     def default() -> "StyleManager":
+        """ Gets the default style manager."""
 
         manager = getattr(StyleManager._context, 'style_manager', None)
         if manager is None:
             get_logger().info("Creating new style manager")
             manager = StyleManager()
             StyleManager._context.style_manager = manager
 
         return manager
 
 class TrackerSorter(Attributee):
+    """ A sorter for trackers. """
 
     experiment = String(default=None)
     analysis = String(default=None)
     result = Integer(val_min=0, default=0)
 
     def __call__(self, experiments, trackers, sequences):
+        """ Sorts the trackers. 
+        
+        Arguments:
+            experiments (list of Experiment): The experiments.
+            trackers (list of Tracker): The trackers.
+            sequences (list of Sequence): The sequences.
+            
+        Returns:
+            A list of indices of the trackers in the sorted order.
+        """
         from vot.analysis import AnalysisError
 
         if self.experiment is None or self.analysis is None:
             return range(len(trackers))
 
         experiment = next(filter(lambda x: x.identifier == self.experiment, experiments), None)
 
@@ -339,14 +426,15 @@
 
         scores = [x[self.result] for x in result]
         indices = [i[0] for i in sorted(enumerate(scores), reverse=True, key=lambda x: x[1])]
 
         return indices
 
 class Generator(Attributee):
+    """ A generator for reports."""
 
     async def generate(self, experiments, trackers, sequences):
         raise NotImplementedError
 
     async def process(self, analyses, experiment, trackers, sequences):
         if sys.version_info >= (3, 3):
             _Iterable = collections.abc.Iterable
@@ -364,21 +452,33 @@
 
         if len(futures) == 1:
             return futures[0].result()
         else:
             return (future.result() for future in futures)
 
 class ReportConfiguration(Attributee):
+    """ A configuration for reports."""
 
     style = Nested(StyleManager)
     sort = Nested(TrackerSorter)
     generators = List(Object(subclass=Generator), default=[])
 
 # TODO: replace this with report generator and separate json/yaml dump
 def generate_document(format: str, config: ReportConfiguration, trackers: typing.List[Tracker], sequences: typing.List[Sequence], results, storage: "Storage"):
+    """ Generates a report document.
+    
+    Args:
+        format: The format of the report.
+        config: The configuration of the report.
+        trackers: The trackers to include in the report.
+        sequences: The sequences to include in the report.
+        results: The results to include in the report.
+        storage: The storage to use for the report.
+        
+    """
 
     from .html import generate_html_document
     from .latex import generate_latex_document
 
     if format == "json":
         generate_serialized(trackers, sequences, results, storage, "json")
     elif format == "yaml":
```

### Comparing `vot-toolkit-0.6.2/vot/document/common.py` & `vot-toolkit-0.6.4/vot/document/common.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,32 @@
+"""Common functions for document generation."""
 import os
 import math
 
 from vot.document import ScatterPlot, LinePlot
 from vot.analysis import Measure, Point, Plot, Curve, Sorting, Axes
 
 def read_resource(name):
+    """Reads a resource file from the package directory. The file is read as a string."""
     path = os.path.join(os.path.dirname(__file__), name)
     with open(path, "r") as filehandle:
         return filehandle.read()
 
 def per_tracker(a):
+    """Returns true if the analysis is per-tracker."""
     return a.axes == Axes.TRACKERS
 
 def extract_measures_table(trackers, results):
+    """Extracts a table of measures from the results. The table is a list of lists, where each list is a column. 
+    The first column is the tracker name, the second column is the measure name, and the rest of the columns are the values for each tracker.
+    
+    Args:
+        trackers (list): List of trackers.
+        results (dict): Dictionary of results.
+    """
     table_header = [[], [], []]
     table_data = dict()
     column_order = []
 
     for experiment, eresults in results.items():
         for analysis, aresults in eresults.items():
             descriptions = analysis.describe()
@@ -66,14 +76,15 @@
             value = v[0]
             order[v[1]] = j
         table_order.append(order)
 
     return table_header, table_data, table_order
 
 def extract_plots(trackers, results, order=None):
+    """Extracts a list of plots from the results. The list is a list of tuples, where each tuple is a pair of strings and a plot."""
     plots = dict()
     j = 0
 
     for experiment, eresults in results.items():
         experiment_plots = list()
         for analysis, aresults in eresults.items():
             descriptions = analysis.describe()
@@ -116,25 +127,27 @@
                 experiment_plots.append((analysis.title + " - " + description.name, plot))
 
         plots[experiment] = experiment_plots
 
     return plots
 
 def format_value(data):
+    """Formats a value for display."""
     if data is None:
         return "N/A"
     if isinstance(data, str):
         return data
     if isinstance(data, int):
         return "%d" % data
     if isinstance(data, float):
         return "%.3f" % data
     return str(data)
 
 def merge_repeats(objects):
+    """Merges repeated objects in a list into a list of tuples (object, count)."""
     
     if not objects:
         return []
 
     repeats = []
     previous = objects[0]
     count = 1
```

### Comparing `vot-toolkit-0.6.2/vot/document/html.py` & `vot-toolkit-0.6.4/vot/document/html.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+"""HTML report generation. This module is used to generate HTML reports from the results of the experiments."""
 import os
 import io
 import logging
 import datetime
 from typing import List
 
 import dominate
@@ -16,29 +16,32 @@
 from vot.document.common import format_value, read_resource, merge_repeats, extract_measures_table, extract_plots
 from vot.document import StyleManager
 from vot.utilities.data import Grid
 
 ORDER_CLASSES = {1: "first", 2: "second", 3: "third"}
 
 def insert_cell(value, order):
+    """Inserts a cell into the data table."""
     attrs = dict(data_sort_value=order, data_value=value)
     if order in ORDER_CLASSES:
         attrs["cls"] = ORDER_CLASSES[order]
     td(format_value(value), **attrs)
 
 def table_cell(value):
+    """Returns a cell for the data table."""
     if isinstance(value, str):
         return value
     elif isinstance(value, Tracker):
         return value.label
     elif isinstance(value, Sequence):
         return value.name
     return format_value(value)
 
 def grid_table(data: Grid, rows: List[str], columns: List[str]):
+    """Generates a table from a grid object."""
 
     assert data.dimensions == 2
     assert data.size(0) == len(rows) and data.size(1) == len(columns)
 
     with table() as element:
         with thead():
             with tr():
@@ -53,32 +56,44 @@
                             if len(value) == 1:
                                 value = value[0]
                         insert_cell(value, None)
 
     return element
 
 def generate_html_document(trackers: List[Tracker], sequences: List[Sequence], results, storage: Storage):
+    """Generates an HTML document from the results of the experiments.
+    
+    Args:
+        trackers (list): List of trackers.
+        sequences (list): List of sequences.
+        results (dict): Dictionary of results.
+        storage (Storage): Storage object.
+    """
 
     def insert_figure(figure):
+        """Inserts a matplotlib figure into the document."""
         buffer = io.StringIO()
         figure.save(buffer, "SVG")
         raw(buffer.getvalue())
 
     def insert_mplfigure(figure):
+        """Inserts a matplotlib figure into the document."""
         buffer = io.StringIO()
         figure.savefig(buffer, format="SVG", bbox_inches='tight', pad_inches=0.01, dpi=200)
         raw(buffer.getvalue())
 
     def add_style(name, linked=False):
+        """Adds a style to the document."""
         if linked:
             link(rel='stylesheet', href='file://' + os.path.join(os.path.dirname(__file__), name))
         else:
             style(read_resource(name))
 
     def add_script(name, linked=False):
+        """Adds a script to the document."""
         if linked:
             script(type='text/javascript', src='file://' + os.path.join(os.path.dirname(__file__), name))
         else:
             with script(type='text/javascript'):
                 raw("//<![CDATA[\n" + read_resource(name) + "\n//]]>")
 
     logger = logging.getLogger("vot")
```

### Comparing `vot-toolkit-0.6.2/vot/document/jquery.js` & `vot-toolkit-0.6.4/vot/document/jquery.js`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.2/vot/document/latex.py` & `vot-toolkit-0.6.4/vot/document/latex.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+"""This module contains functions for generating LaTeX documents with results."""
 import io
 import tempfile
 import datetime
 from typing import List
 
 from pylatex.base_classes import Container
 from pylatex.package import Package
@@ -15,49 +15,68 @@
 from vot.workspace import Storage
 from vot.document.common import format_value, read_resource, merge_repeats, extract_measures_table, extract_plots
 from vot.document import StyleManager
 
 TRACKER_GROUP = "default"
 
 class Chunk(Container):
+    """A container that does not add a newline after the content."""
 
     def dumps(self):
+        """Returns the LaTeX representation of the container."""
         return self.dumps_content()
 
 def strip_comments(src, wrapper=True):
+    """Strips comments from a LaTeX source file."""
     return "\n".join([line for line in src.split("\n") if not line.startswith("%") and (wrapper or not line.startswith(r"\makeat"))])
 
 def insert_figure(figure):
+    """Inserts a figure into a LaTeX document."""
     buffer = io.StringIO()
     figure.save(buffer, "PGF")
     return NoEscape(strip_comments(buffer.getvalue()))
 
 def insert_mplfigure(figure, wrapper=True):
+    """Inserts a matplotlib figure into a LaTeX document."""
     buffer = io.StringIO()
     figure.savefig(buffer, format="PGF", bbox_inches='tight', pad_inches=0.01)
     return NoEscape(strip_comments(buffer.getvalue(), wrapper))
 
 
 def generate_symbols(container, trackers):
+    """Generates a LaTeX command for each tracker. The command is named after the tracker reference and contains the tracker symbol."""
 
     legend = StyleManager.default().legend(Tracker)
 
     container.append(Command("makeatletter"))
     for tracker in trackers:
         container.append(UnsafeCommand('DefineTracker', [tracker.reference, TRACKER_GROUP],
              extra_arguments=insert_mplfigure(legend.figure(tracker), False) + r' \replunderscores{%s}' % tracker.label))
 
     container.append(Command("makeatother"))
 
 
-def generate_latex_document(trackers: List[Tracker], sequences: List[Sequence], results, storage: Storage, build=False, multipart=True, order=None):
+def generate_latex_document(trackers: List[Tracker], sequences: List[Sequence], results, storage: Storage, build=False, multipart=True, order=None) -> str:
+    """Generates a LaTeX document with the results. The document is returned as a string. If build is True, the document is compiled and the PDF is returned.
+    
+    Args:
+        
+        trackers (list): List of trackers.
+        sequences (list): List of sequences.
+        results (dict): Dictionary of results.
+        storage (Storage): Storage object.
+        build (bool): If True, the document is compiled and the PDF is returned.
+        multipart (bool): If True, the document is split into multiple files.
+        order (list): List of tracker indices to use for ordering.
+    """
 
     order_marks = {1: "first", 2: "second", 3: "third"}
 
     def format_cell(value, order):
+        """Formats a cell in the data table."""
         cell = format_value(value)
         if order in order_marks:
             cell = Command(order_marks[order], cell)
         return cell
 
     logger = get_logger()
```

### Comparing `vot-toolkit-0.6.2/vot/document/pure.css` & `vot-toolkit-0.6.4/vot/document/pure.css`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.2/vot/document/report.css` & `vot-toolkit-0.6.4/vot/document/report.css`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.2/vot/document/report.js` & `vot-toolkit-0.6.4/vot/document/report.js`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.2/vot/document/table.js` & `vot-toolkit-0.6.4/vot/document/table.js`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.2/vot/region/__init__.py` & `vot-toolkit-0.6.4/vot/region/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,77 @@
+""" This module contains classes for region representation and manipulation. Regions are also used to represent results
+    of trackers as well as groundtruth trajectories. The module also contains functions for calculating overlaps between
+    regions and for converting between different region types."""
+
 from abc import abstractmethod, ABC
 from enum import Enum
 
 from vot import ToolkitException
 from vot.utilities.draw import DrawHandle
 
 class RegionException(ToolkitException):
     """General region exception"""
 
 class ConversionException(RegionException):
     """Region conversion exception, the conversion cannot be performed
     """
     def __init__(self, *args, source=None):
+        """Constructor
+
+        Args:
+            *args: Arguments for the base exception
+
+        Keyword Arguments:
+            source (Region): Source region (default: {None})
+
+        """
         super().__init__(*args)
         self._source = source
 
 class RegionType(Enum):
     """Enumeration of region types
     """
     SPECIAL = 0
     RECTANGLE = 1
     POLYGON = 2
     MASK = 3
 
 class Region(ABC):
     """
-    Base class for all region containers
-
-    :var type: type of the region
+    Base class for all region containers.
     """
     def __init__(self):
+        """Base constructor"""
         pass
 
     @property
     @abstractmethod
     def type(self):
+        """Return type of the region
+
+        Returns:
+            RegionType -- Type of the region
+        """
         pass
 
     @abstractmethod
     def copy(self):
         """Copy region to another object
+
+        Returns:
+            Region -- Copy of the region
         """
 
     @abstractmethod
     def convert(self, rtype: RegionType):
         """Convert region to another type. Note that some conversions
         degrade information.
-        Arguments:
-            rtype {RegionType} -- Desired type.
+        
+        Args:
+            rtype (RegionType): Target region type to convert to.
         """
 
     @abstractmethod
     def is_empty(self):
         """Check if region is empty (not annotated or not reported)
         """
 
@@ -60,45 +81,66 @@
 
     :var code: Code value
     """
 
     def __init__(self, code):
         """ Constructor
 
-        :param code: Special code
+        Args:
+            code (int): Code value
         """
         super().__init__()
         self._code = int(code)
 
     def __str__(self):
         """ Create string from class """
         return '{}'.format(self._code)
 
     @property
     def type(self):
+        """Return type of the region"""
         return RegionType.SPECIAL
 
     def copy(self):
+        """Copy region to another object"""
         return Special(self._code)
 
     def convert(self, rtype: RegionType):
+        """Convert region to another type. Note that some conversions degrade information.
+
+        Args:
+            rtype (RegionType): Target region type to convert to.
+
+        Raises:
+            ConversionException: Unable to convert special region to another type
+
+        Returns:
+            Region -- Converted region
+        """
+
         if rtype == RegionType.SPECIAL:
             return self.copy()
         else:
             raise ConversionException("Unable to convert special region to {}".format(rtype))
 
     @property
     def code(self):
-        """Retiurns special code for this region
+        """Retiurns special code for this region.
         Returns:
             int -- Type code
         """
         return self._code
 
     def draw(self, handle: DrawHandle):
+        """Draw region to the image using the provided handle.
+
+        Args:
+            handle (DrawHandle): Draw handle
+        """
         pass
 
     def is_empty(self):
+        """ Check if region is empty. Special regions are always empty by definition."""
         return True
 
 from .raster import calculate_overlap, calculate_overlaps
 from .shapes import Rectangle, Polygon, Mask
```

### Comparing `vot-toolkit-0.6.2/vot/region/io.py` & `vot-toolkit-0.6.4/vot/region/io.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,26 @@
+""" Utilities for reading and writing regions from and to files. """
+
 import math
 from typing import List, Union, TextIO
-import struct
 import io
 
 import numpy as np
-from numba import jit
+import numba
 
-@jit(nopython=True)
+@numba.njit(cache=True)
 def mask_to_rle(m, maxstride=100000000):
-    """
-    # Input: 2-D numpy array
-    # Output: list of numbers (1st number = #0s, 2nd number = #1s, 3rd number = #0s, ...)
+    """ Converts a binary mask to RLE encoding. This is a Numba decorated function that is compiled just-in-time for faster execution.
+
+    Args:
+        m (np.ndarray): 2-D binary mask
+        maxstride (int): Maximum number of consecutive 0s or 1s in the RLE encoding. If the number of consecutive 0s or 1s is larger than maxstride, it is split into multiple elements.
+    
+    Returns:
+        List[int]: RLE encoding of the mask
     """
     # reshape mask to vector
     v = m.reshape((m.shape[0] * m.shape[1]))
 
     if v.size == 0:
         return [0]
 
@@ -53,38 +59,43 @@
                 rle.append(length)
         else:
             # last element is different than one element before - add 1
             rle.append(1)
 
     return rle
 
-@jit(nopython=True)
+@numba.njit(cache=True)
 def rle_to_mask(rle, width, height):
+    """ Converts RLE encoding to a binary mask. This is a Numba decorated function that is compiled just-in-time for faster execution.
+
+    Args:
+        rle (List[int]): RLE encoding of the mask
+        width (int): Width of the mask
+        height (int): Height of the mask
+
+    Returns:
+        np.ndarray: 2-D binary mask
     """
-    rle: input rle mask encoding
-    each evenly-indexed element represents number of consecutive 0s
-    each oddly indexed element represents number of consecutive 1s
-    width and height are dimensions of the mask
-    output: 2-D binary mask
-    """
+
     # allocate list of zeros
-    v = [0] * (width * height)
+    v = np.zeros(width * height, dtype=np.uint8)
 
     # set id of the last different element to the beginning of the vector
     idx_ = 0
     for i in range(len(rle)):
         if i % 2 != 0:
             # write as many 1s as RLE says (zeros are already in the vector)
             for j in range(rle[i]):
                 v[idx_+j] = 1
         idx_ += rle[i]
 
     # reshape vector into 2-D mask
     # return np.reshape(np.array(v, dtype=np.uint8), (height, width)) # numba bug / not supporting np.reshape
-    return np.array(v, dtype=np.uint8).reshape((height, width))
+    #return np.array(v, dtype=np.uint8).reshape((height, width))
+    return v.reshape((height, width))
 
 def create_mask_from_string(mask_encoding):
     """
     mask_encoding: a string in the following format: x0, y0, w, h, RLE
     output: mask, offset
     mask: 2-D binary mask, size defined in the mask encoding
     offset: (x, y) offset of the mask in the image coordinates
@@ -97,20 +108,21 @@
     mask = rle_to_mask(rle, region_w, region_h)
 
     return mask, (tl_x, tl_y)
 
 from vot.region.raster import mask_bounds
 
 def encode_mask(mask):
-    """
-    mask: input binary mask, type: uint8
-    output: full RLE encoding in the format: (x0, y0, w, h), RLE
-    first get minimal axis-aligned region which contains all positive pixels
-    extract this region from mask and calculate mask RLE within the region
-    output position and size of the region, dimensions of the full mask and RLE encoding
+    """ Encode a binary mask to a string in the following format: x0, y0, w, h, RLE.
+
+    Args:
+        mask (np.ndarray): 2-D binary mask
+
+    Returns:
+        str: Encoded mask
     """
     # calculate coordinates of the top-left corner and region width and height (minimal region containing all 1s)
     x_min, y_min, x_max, y_max = mask_bounds(mask)
 
     # handle the case when the mask empty
     if x_min is None:
         return (0, 0, 0, 0), [0]
@@ -124,30 +136,30 @@
         # do not use full mask to optimize speed and space
         target_mask = mask[tl_y:tl_y+region_h, tl_x:tl_x+region_w]
         rle = mask_to_rle(np.array(target_mask))
 
         return (tl_x, tl_y, region_w, region_h), rle
 
 def parse_region(string: str) -> "Region":
-    """   
-        Parse input string to the appropriate region format and return Region object
+    """Parse input string to the appropriate region format and return Region object
 
     Args:
         string (str): comma separated list of values
 
     Returns:
         Region: resulting region
     """
+    from vot import config
     from vot.region import Special
     from vot.region.shapes import Rectangle, Polygon, Mask
 
     if string[0] == 'm':
         # input is a mask - decode it
         m_, offset_ = create_mask_from_string(string[1:].split(','))
-        return Mask(m_, offset=offset_)
+        return Mask(m_, offset=offset_, optimize=config.mask_optimize_read)
     else:
         # input is not a mask - check if special, rectangle or polygon
         tokens = [float(t) for t in string.split(',')]
         if len(tokens) == 1:
             return Special(tokens[0])
         if len(tokens) == 4:
             if any([math.isnan(el) for el in tokens]):
@@ -158,26 +170,36 @@
             if any([math.isnan(el) for el in tokens]):
                 return Special(0)
             else:
                 return Polygon([(x_, y_) for x_, y_ in zip(tokens[::2], tokens[1::2])])
     return None
 
 def read_trajectory_binary(fp: io.RawIOBase):
+    """Reads a trajectory from a binary file and returns a list of regions.
+    
+    Args:
+        fp (io.RawIOBase): File pointer to the binary file
+        
+    Returns:
+        list: List of regions
+    """
     import struct
     from cachetools import LRUCache, cached
     from vot.region import Special
     from vot.region.shapes import Rectangle, Polygon, Mask
 
     buffer = dict(data=fp.read(), offset = 0)
 
     @cached(cache=LRUCache(maxsize=32))
     def calcsize(format):
+        """Calculate size of the struct format"""
         return struct.calcsize(format)
 
     def read(format: str):
+        """Read struct from the buffer and update offset"""
         unpacked = struct.unpack_from(format, buffer["data"], buffer["offset"])
         buffer["offset"] += calcsize(format)
         return unpacked
 
     _, length = read("<hI")
 
     trajectory = []
@@ -196,14 +218,20 @@
             r = Mask(rle_to_mask(rle, region_w, region_h), (tl_x, tl_y))
         else:
             raise IOError("Wrong region type")
         trajectory.append(r)
     return trajectory
 
 def write_trajectory_binary(fp: io.RawIOBase, data: List["Region"]):
+    """Writes a trajectory to a binary file.
+
+    Args:
+        fp (io.RawIOBase): File pointer to the binary file
+        data (list): List of regions
+    """
     import struct
     from vot.region import Special
     from vot.region.shapes import Rectangle, Polygon, Mask
 
     fp.write(struct.pack("<hI", 1, len(data)))
 
     for r in data:
@@ -213,14 +241,22 @@
         elif isinstance(r, Mask): 
             rle = mask_to_rle(r.mask, maxstride=255*255)
             fp.write(struct.pack("<BhhHHH%dH" % len(rle), 3, r.offset[0], r.offset[1], r.mask.shape[1], r.mask.shape[0], len(rle), *rle))
         else:
             raise IOError("Wrong region type")
 
 def read_trajectory(fp: Union[str, TextIO]):
+    """Reads a trajectory from a file and returns a list of regions.
+    
+    Args:
+        fp (str or TextIO): File path or file pointer to the trajectory file
+        
+    Returns:
+        list: List of regions
+    """
     if isinstance(fp, str):
         try:
             import struct
             with open(fp, "r+b") as tfp:
                 v, = struct.unpack("<h", tfp.read(struct.calcsize("<h")))
                 binary = v == 1
                 # TODO: we can use the same file handle in case of binary format
@@ -242,23 +278,23 @@
 
     if close:
         fp.close()
 
     return regions
 
 def write_trajectory(fp: Union[str, TextIO], data: List["Region"]):
-    """ Write a trajectory to a file handle or a file with a given name.
-
-    Based on the suffix of a file or properties of a file handle, the output may be either text based
+    """ Write a trajectory to a file handle or a file with a given name. Based on the suffix of a file or properties of a file handle, the output may be either text based
     or binary.
 
     Args:
         fp (Union[str, TextIO]): File handle or file name
         data (List[Region]): Trajectory, a list of region objects
 
+    Raises:
+        IOError: If the file format is not supported
     """
 
     if isinstance(fp, str):
         binary = fp.endswith(".bin")
         close = True
         fp = open(fp, "wb" if binary else "w")
     else:
```

### Comparing `vot-toolkit-0.6.2/vot/region/raster.py` & `vot-toolkit-0.6.4/vot/region/raster.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+""" Rasterization of regions. This module contains functions for rasterizing different region types."""
+
 from typing import List, Tuple, Optional
 
 import numba
 import numpy as np
 
 _TYPE_EMPTY = 0
 _TYPE_RECTANGLE = 1
 _TYPE_POLYGON = 2
 _TYPE_MASK = 3
 
-@numba.njit()
+@numba.njit(cache=True)
 def mask_bounds(mask: np.ndarray):
-    """
-    mask: 2-D array with a binary mask
-    output: coordinates of the top-left and bottom-right corners of the minimal axis-aligned region containing all positive pixels
+    """ Compute bounds of a binary mask. Bounds are defined as the minimal axis-aligned region containing all positive pixels.
+    This is a Numba implementation of the function that is compiled to machine code for faster execution.
+
+    Args:
+        mask: 2-D array with a binary mask
+
+    Returns:
+        coordinates of the top-left and bottom-right corners of the minimal axis-aligned region containing all positive pixels
     """
     ii32 = np.iinfo(np.int32)
     top = ii32.max
     bottom = ii32.min
     left = ii32.max
     right = ii32.min
 
@@ -30,16 +37,25 @@
 
     if top == ii32.max:
         return (0, 0, 0, 0)
 
     return (left, top, right, bottom)
 
 
-@numba.njit()
+@numba.njit(cache=True)
 def rasterize_rectangle(data: np.ndarray, bounds: Tuple[int, int, int, int]):
+    """ Rasterize a rectangle. This is a Numba implementation of the function that is compiled to machine code for faster execution.
+
+    Args:
+        data: 4x1 array with rectangle coordinates (x, y, width, height)
+        bounds: 4-tuple with the bounds of the image (left, top, right, bottom)
+
+    Returns:
+        2-D array with the rasterized rectangle
+    """
     width = bounds[2] - bounds[0] + 1
     height = bounds[3] - bounds[1] + 1
 
     mask = np.zeros((height, width), dtype=np.uint8)
 
     if data[0, 0] > bounds[2] or data[0, 0] + data[2, 0] - 1 < bounds[0] or data[1, 0] > bounds[3] or data[1, 0] + data[3, 0] - 1 < bounds[1]:
         return mask
@@ -49,18 +65,25 @@
     right = min(bounds[2], data[0, 0] + data[2, 0] - 1 - bounds[0])
     bottom = min(bounds[3], data[1, 0] + data[3, 0] - 1 - bounds[1])
 
     mask[top:bottom+1, left:right+1] = 1
 
     return mask
 
-
-#@numba.njit(numba.uint8[:, ::1](numba.float32[:, ::1], numba.types.UniTuple(numba.int64, 4)))
-@numba.njit()
+@numba.njit(cache=True)
 def rasterize_polygon(data: np.ndarray, bounds: Tuple[int, int, int, int]):
+    """ Rasterize a polygon. This is a Numba implementation of the function that is compiled to machine code for faster execution.
+
+    Args:
+        data: Nx2 array with polygon coordinates
+        bounds: 4-tuple with the bounds of the image (left, top, right, bottom)
+
+    Returns:
+        2-D array with the rasterized polygon
+    """
 
     #int nodes, pixelY, i, j, swap;
     #region_polygon polygon = polygon_input;
     count = data.shape[0]
 
     width = bounds[2] - bounds[0] + 1
     height = bounds[3] - bounds[1] + 1
@@ -126,16 +149,27 @@
                 for j in range(nodeX[i], nodeX[i + 1] + 1):
                     mask[pixelY, j] = 1
             i += 2
 
     return mask
 
 
-@numba.njit()
+@numba.njit(cache=True)
 def copy_mask(mask: np.ndarray, offset: Tuple[int, int], bounds: Tuple[int, int, int, int]):
+    """ Copy a mask to a new location. This is a Numba implementation of the function that is compiled to machine code for faster execution.
+     
+    Args:
+        mask: 2-D array with the mask
+        offset: 2-tuple with the offset of the mask
+        bounds: 4-tuple with the bounds of the image (left, top, right, bottom)
+        
+    Returns:
+        2-D array with the copied mask
+    """
+
     tx = max(offset[0], bounds[0])
     ty = max(offset[1], bounds[1])
 
     ox = tx - bounds[0]
     oy = ty - bounds[1]
     gx = tx - offset[0]
     gy = ty - offset[1]
@@ -147,63 +181,123 @@
 
     for i in range(th):
         for j in range(tw):
             copy[i + oy, j + ox] = mask[i + gy, j + gx]
 
     return copy
 
-@numba.njit()
+@numba.njit(cache=True)
 def _bounds_rectangle(a):
+    """ Calculate the bounds of a rectangle. This is a Numba implementation of the function that is compiled to machine code for faster execution.
+    
+    Args:
+        a: 4x1 array with the rectangle coordinates
+        
+    Returns:
+        4-tuple with the bounds of the rectangle (left, top, right, bottom)
+    """
     return (int(round(a[0, 0])), int(round(a[1, 0])), int(round(a[0, 0] + a[2, 0] - 1)), int(round(a[1, 0] + a[3, 0] - 1)))
 
-@numba.njit()
+@numba.njit(cache=True)
 def _bounds_polygon(a):
+    """ Calculate the bounds of a polygon. This is a Numba implementation of the function that is compiled to machine code for faster execution.
+    
+    Args:
+        a: Nx2 array with the polygon coordinates
+    
+    Returns:
+        4-tuple with the bounds of the polygon (left, top, right, bottom)
+    """
     fi32 = np.finfo(np.float32)
     top = fi32.max
     bottom = fi32.min
     left = fi32.max
     right = fi32.min
 
     for i in range(a.shape[0]):
         top = min(top, a[i, 1])
         bottom = max(bottom, a[i, 1])
         left = min(left, a[i, 0])
         right = max(right, a[i, 0])
     return (int(round(left)), int(round(top)), int(round(right)), int(round(bottom)))
 
-@numba.njit()
+@numba.njit(cache=True)
 def _bounds_mask(a, o):
+    """ Calculate the bounds of a mask. This is a Numba implementation of the function that is compiled to machine code for faster execution.
+    
+    Args:
+        a: 2-D array with the mask
+        o: 2-tuple with the offset of the mask
+        
+    Returns:
+        4-tuple with the bounds of the mask (left, top, right, bottom)
+    """
     bounds = mask_bounds(a)
     return (bounds[0] + o[0], bounds[1] + o[1], bounds[2] + o[0], bounds[3] + o[1])
 
-@numba.njit()
+@numba.njit(cache=True)
 def _region_bounds(a: np.ndarray, t: int, o: Optional[Tuple[int, int]] = None):
+    """ Calculate the bounds of a region. This is a Numba implementation of the function that is compiled to machine code for faster execution.
+    
+    Args:
+        a: 2-D array with the mask
+        t: type of the region
+        o: 2-tuple with the offset of the mask
+        
+    Returns:
+        4-tuple with the bounds of the region (left, top, right, bottom)
+    """
     if t == _TYPE_RECTANGLE:
         return _bounds_rectangle(a)
     elif t == _TYPE_POLYGON:
         return _bounds_polygon(a)
     elif t == _TYPE_MASK:
         return _bounds_mask(a, o)
     return (0, 0, 0, 0)
 
-@numba.njit()
+@numba.njit(cache=True)
 def _region_raster(a: np.ndarray, bounds: Tuple[int, int, int, int], t: int, o: Optional[Tuple[int, int]] = None):
+    """ Rasterize a region. This is a Numba implementation of the function that is compiled to machine code for faster execution.
+
+    Args:
+        a: 2-D array with the mask
+        bounds: 4-tuple with the bounds of the image (left, top, right, bottom)
+        t: type of the region
+        o: 2-tuple with the offset of the mask
+        
+    Returns:
+        2-D array with the rasterized region
+    """
 
     if t == _TYPE_RECTANGLE:
         return rasterize_rectangle(a, bounds)
     elif t == _TYPE_POLYGON:
         return rasterize_polygon(a, bounds)
     elif t == _TYPE_MASK:
         return copy_mask(a, o, bounds)
     
     return np.zeros((bounds[3] - bounds[1] + 1, bounds[2] - bounds[0] + 1), dtype=np.uint8)
 
 @numba.njit(cache=True)
 def _calculate_overlap(a: np.ndarray, b: np.ndarray, at: int, bt: int, ao: Optional[Tuple[int, int]] = None,
         bo: Optional[Tuple[int, int]] = None, bounds: Optional[Tuple[int, int]] = None):
+    """ Calculate the overlap between two regions. This is a Numba implementation of the function that is compiled to machine code for faster execution.
+    
+    Args:
+        a: 2-D array with the mask of the first region
+        b: 2-D array with the mask of the second region
+        at: type of the first region
+        bt: type of the second region
+        ao: 2-tuple with the offset of the first mask
+        bo: 2-tuple with the offset of the second mask
+        bounds: 2-tuple with the bounds of the image (left, top, right, bottom)
+    
+    Returns:
+        float with the overlap between the two regions. Note that overlap is one by definition if both regions are empty.
+    """
 
     bounds1 = _region_bounds(a, at, ao)
     bounds2 = _region_bounds(b, bt, bo)
 
     union = (min(bounds1[0], bounds2[0]), min(bounds1[1], bounds2[1]), max(bounds1[2], bounds2[2]), max(bounds1[3], bounds2[3]))
 
     if union[0] >= union[2] or union[1] >= union[3]:
@@ -238,18 +332,24 @@
 
 from vot.region import Region, RegionException
 from vot.region.shapes import Shape, Rectangle, Polygon, Mask
 
 Bounds = Tuple[int, int]
 
 def calculate_overlap(reg1: Shape, reg2: Shape, bounds: Optional[Bounds] = None):
-    """
-    Inputs: reg1 and reg2 are Region objects (Rectangle, Polygon or Mask)
-    bounds: size of the image, format: [width, height]
-    function first rasterizes both regions to 2-D binary masks and calculates overlap between them
+    """ Calculate the overlap between two regions. The function first rasterizes both regions to 2-D binary masks and calculates overlap between them
+
+    Args:
+        reg1: first region
+        reg2: second region
+        bounds: 2-tuple with the bounds of the image (width, height)
+
+    Returns:
+        float with the overlap between the two regions. Note that overlap is one by definition if both regions are empty.
+    
     """
 
     if isinstance(reg1, Rectangle):
         data1 = np.round(reg1._data)
         offset1 = (0, 0)
         type1 = _TYPE_RECTANGLE
     elif isinstance(reg1, Polygon):
@@ -281,15 +381,23 @@
         data2 = np.zeros((1, 1))
         offset2 = (0, 0)
         type2 = _TYPE_EMPTY
 
     return _calculate_overlap(data1, data2, type1, type2, offset1, offset2, bounds)
 
 def calculate_overlaps(first: List[Region], second: List[Region], bounds: Optional[Bounds] = None):
-    """
-    first and second are lists containing objects of type Region
-    bounds is in the format [width, height]
-    output: list of per-frame overlaps (floats)
+    """ Calculate the overlap between two lists of regions. The function first rasterizes both regions to 2-D binary masks and calculates overlap between them
+
+    Args:
+        first: first list of regions
+        second: second list of regions
+        bounds: 2-tuple with the bounds of the image (width, height)
+
+    Returns:
+        list of floats with the overlap between the two regions. Note that overlap is one by definition if both regions are empty.
+
+    Raises:
+        RegionException: if the lists are not of the same size
     """
     if not len(first) == len(second):
         raise RegionException("List not of the same size {} != {}".format(len(first), len(second)))
     return [calculate_overlap(pairs[0], pairs[1], bounds=bounds) for i, pairs in enumerate(zip(first, second))]
```

### Comparing `vot-toolkit-0.6.2/vot/region/tests.py` & `vot-toolkit-0.6.4/vot/region/tests.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 
+"""Tests for the region module. """
+
 import unittest
 
 import numpy as np
 
 from vot.region.raster import rasterize_polygon, rasterize_rectangle, copy_mask, calculate_overlap
 
 class TestRasterMethods(unittest.TestCase):
+    """Tests for the raster module."""
 
     def test_rasterize_polygon(self):
+        """Tests if the polygon rasterization works correctly. """
         points = np.array([[0, 0], [0, 100], [100, 100], [100, 0]], dtype=np.float32)
         np.testing.assert_array_equal(rasterize_polygon(points, (0, 0, 99, 99)), np.ones((100, 100), dtype=np.uint8))
 
     def test_rasterize_rectangle(self):
+        """Tests if the rectangle rasterization works correctly."""
         np.testing.assert_array_equal(rasterize_rectangle(np.array([[0], [0], [100], [100]], dtype=np.float32), (0, 0, 99, 99)), np.ones((100, 100), dtype=np.uint8))
 
     def test_copy_mask(self):
+        """Tests if the mask copy works correctly."""
         mask = np.ones((100, 100), dtype=np.uint8)
         np.testing.assert_array_equal(copy_mask(mask, (0, 0), (0, 0, 99, 99)), np.ones((100, 100), dtype=np.uint8))
 
     def test_calculate_overlap(self):
+        """Tests if the overlap calculation works correctly."""
         from vot.region import Rectangle
 
         r1 = Rectangle(0, 0, 100, 100)
         self.assertEqual(calculate_overlap(r1, r1), 1)
 
         r1 = Rectangle(0, 0, 0, 0)        
         self.assertEqual(calculate_overlap(r1, r1), 1)
 
     def test_empty_mask(self):
+        """Tests if the empty mask is correctly detected."""
         from vot.region import Mask
 
         mask = Mask(np.zeros((100, 100), dtype=np.uint8))
         self.assertTrue(mask.is_empty())
 
         mask = Mask(np.ones((100, 100), dtype=np.uint8))
         self.assertFalse(mask.is_empty())
 
     def test_binary_format(self):
-        """ Tests if the binary format of a region matched the plain-text one"""
+        """ Tests if the binary format of a region matched the plain-text one."""
         import io
 
         from vot.region import Rectangle, Polygon, Mask
         from vot.region.io import read_trajectory, write_trajectory
         from vot.region.raster import calculate_overlaps
 
         trajectory = [
@@ -68,14 +76,15 @@
         o1 = calculate_overlaps(bint, txtt, None)
         o2 = calculate_overlaps(bint, trajectory, None)
 
         self.assertTrue(np.all(np.array(o1) == 1))
         self.assertTrue(np.all(np.array(o2) == 1))
 
     def test_rle(self):
+        """ Test if RLE encoding works for limited stride representation."""
         from vot.region.io import rle_to_mask, mask_to_rle 
         rle = [0, 2, 122103, 9, 260, 19, 256, 21, 256, 22, 254, 24, 252, 26, 251, 27, 250, 28, 249, 28, 250, 28, 249, 28, 249, 29, 249, 30, 247, 33, 245, 33, 244, 34, 244, 37, 241, 39, 239, 41, 237, 41, 236, 43, 235, 45, 234, 47, 233, 47, 231, 48, 230, 48, 230, 11, 7, 29, 231, 9, 9, 29, 230, 8, 11, 28, 230, 7, 12, 28, 230, 7, 13, 27, 231, 5, 14, 27, 233, 2, 16, 26, 253, 23, 255, 22, 256, 20, 258, 19, 259, 17, 3]
         rle = np.array(rle)
         m1 = rle_to_mask(np.array(rle, dtype=np.int32), 277, 478)
 
         r2 = mask_to_rle(m1, maxstride=255)
         m2 = rle_to_mask(np.array(r2, dtype=np.int32), 277, 478)
```

### Comparing `vot-toolkit-0.6.2/vot/stack/__init__.py` & `vot-toolkit-0.6.4/vot/stack/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,32 @@
+"""Stacks are collections of experiments that are grouped together for convenience. Stacks are used to organize experiments and to run them in 
+batch mode.
+"""
 import os
-import json
-import glob
-import collections
 from typing import List, Mapping
 
 import yaml
 
 from attributee import Attributee, String, Boolean, Map, Object
 
 from vot.experiment import Experiment, experiment_registry
 from vot.utilities import import_class
 
 def experiment_resolver(typename, context, **kwargs):
+    """Resolves experiment objects from stack definitions. This function is used by the stack module to resolve experiment objects from stack
+    definitions. It is not intended to be used directly.
+
+    Args:
+        typename (str): Name of the experiment class
+        context (Attributee): Context of the experiment
+        kwargs (dict): Additional arguments
+
+    Returns:
+        Experiment: Experiment object
+    """
 
     identifier = context.key
     storage = None
 
     if getattr(context.parent, "workspace", None) is not None:
         storage = context.parent.workspace.storage
 
@@ -25,42 +36,63 @@
         return experiment
     else:
         experiment_class = import_class(typename)
         assert issubclass(experiment_class, Experiment)
         return experiment_class(_identifier=identifier, _storage=storage, **kwargs)
 
 class Stack(Attributee):
+    """Stack class represents a collection of experiments. Stacks are used to organize experiments and to run them in batch mode.
+    """
 
     title = String(default="Stack")
     dataset = String(default=None)
     url = String(default="")
     deprecated = Boolean(default=False)
     experiments = Map(Object(experiment_resolver))
 
     def __init__(self, name: str, workspace: "Workspace", **kwargs):
+        """Creates a new stack object.
+
+        Args:
+            name (str): Name of the stack
+            workspace (Workspace): Workspace object
+        """
         self._workspace = workspace
         self._name = name
 
         super().__init__(**kwargs)
 
     @property
     def workspace(self):
+        """Returns the workspace object for the stack."""
         return self._workspace
 
     @property
     def name(self):
+        """Returns the name of the stack."""
         return self._name
 
     def __iter__(self):
+        """Iterates over experiments in the stack."""
         return iter(self.experiments.values())
 
     def __len__(self):
+        """Returns the number of experiments in the stack."""
         return len(self.experiments)
 
     def __getitem__(self, identifier):
+        """Returns the experiment with the given identifier.
+
+        Args:
+            identifier (str): Identifier of the experiment
+        
+        Returns:
+            Experiment: Experiment object
+
+        """
         return self.experiments[identifier]
 
 def resolve_stack(name: str, *directories: List[str]) -> str:
     """Searches for stack file in the given directories and returns its absolute path. If given an absolute path as input
     it simply returns it.
 
     Args:
```

### Comparing `vot-toolkit-0.6.2/vot/stack/tests/multiobject.yaml` & `vot-toolkit-0.6.4/vot/stack/tests/multiobject.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.2/vot/stack/tests/segmentation.yaml` & `vot-toolkit-0.6.4/vot/stack/tests/segmentation.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.2/vot/stack/vot2016/rgb.yaml` & `vot-toolkit-0.6.4/vot/stack/vot2016/rgb.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.2/vot/stack/vot2017.yaml` & `vot-toolkit-0.6.4/vot/stack/vot2017.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.2/vot/stack/vot2018/shortterm.yaml` & `vot-toolkit-0.6.4/vot/stack/vot2018/shortterm.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.2/vot/stack/vot2019/shortterm.yaml` & `vot-toolkit-0.6.4/vot/stack/vot2019/shortterm.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.2/vot/stack/vot2020/shortterm.yaml` & `vot-toolkit-0.6.4/vot/stack/vot2020/shortterm.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.2/vot/stack/vot2021/st.yaml` & `vot-toolkit-0.6.4/vot/stack/vot2021/st.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.2/vot/stack/vot2022/stb.yaml` & `vot-toolkit-0.6.4/vot/stack/vot2022/stb.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.2/vot/stack/vot2022/sts.yaml` & `vot-toolkit-0.6.4/vot/stack/vot2022/sts.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.2/vot/tracker/__init__.py` & `vot-toolkit-0.6.4/vot/utilities/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,618 +1,608 @@
+""" This module contains various utility functions and classes used throughout the toolkit. """
 
 import os
+import sys
+import csv
 import re
-import configparser
+import hashlib
 import logging
-import copy
-from typing import Tuple, List, Union
-from collections import OrderedDict, namedtuple
-from abc import abstractmethod, ABC
-
-import yaml
-
-from vot import ToolkitException
-from vot.dataset import Frame
-from vot.region import Region
-from vot.utilities import to_string
-
-logger = logging.getLogger("vot")
+import inspect
+import time
+import concurrent.futures as futures
+from logging import Formatter, LogRecord
+
+from numbers import Number
+from typing import Any, Mapping, Tuple
+import typing
+from vot import get_logger
+
+import six
+import colorama
+
+__ALIASES = dict()
+
+def import_class(classpath: str) -> typing.Type:
+    """Import a class from a string by importing parent packages. 
+
+    Args:
+        classpath (str): String representing a canonical class name with all parent packages.
+
+    Raises:
+        ImportError: Raised when
+
+    Returns:
+        [type]: [description]
+    """
+    delimiter = classpath.rfind(".")
+    if delimiter == -1:
+        if classpath in __ALIASES:
+            return __ALIASES[classpath]
+        else:
+            raise ImportError("Class alias '{}' not found".format(classpath))
+    else:
+        classname = classpath[delimiter+1:len(classpath)]
+        module = __import__(classpath[0:delimiter], globals(), locals(), [classname])
+        return getattr(module, classname)
+
+def alias(*args):
+    """ Decorator for registering class aliases. Aliases are used to refer to classes by a short name.
+
+    Args:
+        *args: A list of strings representing aliases for the class.
+    """
+
+    def register(cls: typing.Type):
+        """ Register the class with the given aliases.  """
+        assert cls is not None
+        for name in args:
+            if name in __ALIASES:
+                if not __ALIASES[name] == cls:
+                    raise ImportError("Alias already taken")
+            else:
+                __ALIASES[name] = cls
+        return cls
+    return register
+
+def class_fullname(o):
+    """Returns the full name of the class of the given object.
+    
+    Args:
+        o: The object to get the class name from.
+        
+    Returns:
+        The full name of the class of the given object.
+    """
+    return class_string(o.__class__)
+
+def class_string(kls):
+    """Returns the full name of the given class.
+
+    Args:
+        kls: The class to get the name from.
+
+    Returns:
+        The full name of the given class.
+    """
+    assert inspect.isclass(kls)
+    module = kls.__module__
+    if module is None or module == str.__class__.__module__:
+        return kls.__name__  # Avoid reporting __builtin__
+    else:
+        return module + '.' + kls.__name__
+
+def flip(size: Tuple[Number, Number]) -> Tuple[Number, Number]:
+    """Flips the given size tuple.
+
+    Args:
+        size: The size tuple to flip.
+        
+    Returns:
+        The flipped size tuple.
+    """
+    return (size[1], size[0])
+
+def flatten(nested_list):
+    """Flattens a nested list.
+
+    Args:
+        nested_list: The nested list to flatten.
+
+    Returns:
+        The flattened list.
+    """
+    return [item for sublist in nested_list for item in sublist]
+
+from vot.utilities.notebook import is_notebook
+
+if is_notebook():
+    try:
+        from ipywidgets import IntProgress
+        from tqdm._tqdm_notebook import tqdm_notebook as tqdm
+    except ImportError:
+        from tqdm import tqdm
+else:
+    from tqdm import tqdm
+
+class Progress(object):
+    """Wrapper around tqdm progress bar, enables silecing the progress output and some more
+    costumizations.
+    """
+
+    class StreamProxy(object):
+        """Proxy class for tqdm to enable silent mode."""
+
+        def write(self, x):
+            """Write function used by tqdm."""
+            # Avoid print() second call (useless \n)
+            if len(x.rstrip()) > 0:
+                tqdm.write(x)
+
+        def flush(self):
+            """Flush function used by tqdm."""
+            #return getattr(self.file, "flush", lambda: None)()
+            pass
 
-class TrackerException(ToolkitException):
-    """ Base class for all tracker related exceptions."""
+    @staticmethod
+    def logstream():
+        """Returns a stream proxy that can be used to redirect output to the progress bar."""
+        return Progress.StreamProxy()
 
-    def __init__(self, *args, tracker, tracker_log=None):
-        """ Initialize the exception.
+    def __init__(self, description="Processing", total=100):
+        """Creates a new progress bar.
 
         Args:
-            tracker (Tracker): Tracker that caused the exception.
-            tracker_log (str, optional): Optional log message. Defaults to None.
-        """
-        super().__init__(*args)
-        self._tracker_log = tracker_log
-        self._tracker = tracker
-
-    @property
-    def log(self) -> str:
-        """ Returns the log message of the tracker.
-
-        Returns:
-            sts: Log message of the tracker.
+            description: The description of the progress bar.
+            total: The total number of steps.
         """
-        return self._tracker_log
-
-    @property
-    def tracker(self):
-        """ Returns the tracker that caused the exception."""
-        return self._tracker
-
-class TrackerTimeoutException(TrackerException):
-    pass
-
-VALID_IDENTIFIER = re.compile("^[a-zA-Z0-9-_]+$")
-
-VALID_REFERENCE = re.compile("^([a-zA-Z0-9-_]+)(@[a-zA-Z0-9-_]*)?$")
-
-def is_valid_identifier(identifier):
-    """Checks if the identifier is valid."""
-    return not VALID_IDENTIFIER.match(identifier) is None
-
-def is_valid_reference(reference):
-    """Checks if the reference is valid."""
-    return not VALID_REFERENCE.match(reference) is None
-
-def parse_reference(reference):
-    """Parses the reference into identifier and version."""
-    matches = VALID_REFERENCE.match(reference)
-    if not matches:
-        return None, None
-    return matches.group(1), matches.group(2)[1:] if not matches.group(2) is None else None
+        silent = get_logger().level > logging.INFO
 
-_runtime_protocols = {}
+        if not silent:
+            self._tqdm = tqdm(disable=False if is_notebook() else None,
+                bar_format=" {desc:20.20} |{bar}| {percentage:3.0f}% [{elapsed}<{remaining}]")
+            self._tqdm.desc = description
+            self._tqdm.total = total
+        if silent or self._tqdm.disable:
+            self._tqdm = None
+            self._value = 0
+            self._total = total if not silent else 0
 
-class Registry(object):
-    """ Repository of known trackers. Trackers are loaded from a manifest files in one or more directories. """
-
-    def __init__(self, directories, root=os.getcwd()):
-        trackers = dict()
-        registries = []
-
-        for directory in directories:
-            if not os.path.isabs(directory):
-                directory = os.path.normpath(os.path.abspath(os.path.join(root, directory)))
-
-            if os.path.isdir(directory):
-                registries.append(os.path.join(directory, "trackers.yaml"))
-                registries.append(os.path.join(directory, "trackers.ini"))
-
-            if os.path.isfile(directory):
-                registries.append(directory)
-
-        for registry in list(dict.fromkeys(registries)):
-            if not os.path.isfile(registry):
-                continue
-
-            logger.debug("Scanning registry %s", registry)
-
-            extension = os.path.splitext(registry)[1].lower()
-
-            if extension == ".yaml":
-                with open(registry, 'r') as fp:
-                    metadata = yaml.load(fp, Loader=yaml.BaseLoader)
-                for k, v in metadata.items():
-                    if not is_valid_identifier(k):
-                        logger.warning("Invalid tracker identifier %s in %s", k, registry)
-                        continue
-                    if k in trackers:
-                        logger.warning("Duplicate tracker identifier %s in %s", k, registry)
-                        continue
-
-                    trackers[k] = Tracker(_identifier=k, _source=registry, **v)
-
-            if extension == ".ini":
-                config = configparser.ConfigParser()
-                config.read(registry)
-                for section in config.sections():
-                    if not is_valid_identifier(section):
-                        logger.warning("Invalid identifier %s in %s", section, registry)
-                        continue
-                    if section in trackers:
-                        logger.warning("Duplicate tracker identifier %s in %s", section, registry)
-                        continue
-
-                    trackers[section] = Tracker(_identifier=section, _source=registry, **config[section])
-
-        self._trackers = OrderedDict(sorted(trackers.items(), key=lambda t: t[0]))
-        logger.debug("Found %d trackers", len(self._trackers))
-
-    def __getitem__(self, reference) -> "Tracker":
-        """ Returns the tracker for the given reference. """
-
-        return self.resolve(reference, skip_unknown=False, resolve_plural=False)[0]
-
-    def __contains__(self, reference) -> bool:
-        """ Checks if the tracker is registered. """
-        identifier, _ = parse_reference(reference)
-        return identifier in self._trackers
-
-    def __iter__(self):
-        return iter(self._trackers.values())
-
-    def __len__(self):
-        return len(self._trackers)
-
-    def resolve(self, *references, storage=None, skip_unknown=True, resolve_plural=True):
-        """ Resolves the references to trackers.
+    def _percent(self, n):
+        """Returns the percentage of the given value.
 
         Args:
-            storage (_type_, optional): Sto . Defaults to None.
-            skip_unknown (bool, optional): _description_. Defaults to True.
-            resolve_plural (bool, optional): _description_. Defaults to True.
-
-        Raises:
-            ToolkitException: _description_
+            n: The value to compute the percentage of.
 
         Returns:
-            _type_: _description_
-        """        """"""
-
-        trackers = []
-
-        for reference in references:
-
-            if resolve_plural and reference.startswith("#"):
-                tag = reference[1:]
-                if not is_valid_identifier(tag):
-                    continue
-                for tracker in self._trackers.values():
-                    if tracker.tagged(tag):
-                        trackers.extend(self._find_versions(tracker.identifier, storage))
-                continue
-
-            identifier, version = parse_reference(reference)
-
-            if not identifier in self._trackers:
-                if not skip_unknown:
-                    raise ToolkitException("Unable to resolve tracker reference: {}".format(reference))
-                else:
-                    continue
-
-            base = self._trackers[identifier]
-
-            if version == "":
-                trackers.extend(self._find_versions(identifier, storage))
-            else:
-                trackers.append(base.reversion(version))
-
-        return trackers
-
-    def _find_versions(self, identifier, storage):
-
-        trackers = []
-
-        if storage is None:
-            return trackers
-
-        for reference in storage.folders():
-            if reference.startswith(identifier + "@"):
-                identifier, version = parse_reference(reference)
-                base = self._trackers[identifier]
-                trackers.append(base.reversion(version))
-
-        return trackers
-
-    def references(self):
-        return [t.reference for t in self._trackers.values()]
-
-    def identifiers(self):
-        return [t.identifier for t in self._trackers.values()]
-
-class Tracker(object):
-    """ Tracker definition class. """
-
-    @staticmethod
-    def _collect_envvars(**kwargs):
-        envvars = dict()
-        other = dict()
-
-        if "env" in kwargs:
-            if isinstance(kwargs["env"], dict):
-                envvars.update({k: os.path.expandvars(v) for k, v in kwargs["env"].items()})
-            del kwargs["env"]
-
-        for name, value in kwargs.items():
-            if name.startswith("env_") and len(name) > 4:
-                envvars[name[4:].upper()] = os.path.expandvars(value)
-            else:
-                other[name] = value
-
-        return envvars, other
-
-    @staticmethod
-    def _collect_arguments(**kwargs):
-        arguments = dict()
-        other = dict()
-
-        if "arguments" in kwargs:
-            if isinstance(kwargs["arguments"], dict):
-                arguments.update(kwargs["arguments"])
-            del kwargs["arguments"]
-
-        for name, value in kwargs.items():
-            if name.startswith("arg_") and len(name) > 4:
-                arguments[name[4:].lower()] = value
-            else:
-                other[name] = value
-
-        return arguments, other
-
-    @staticmethod
-    def _collect_metadata(**kwargs):
-        metadata = dict()
-        other = dict()
-
-        if "metadata" in kwargs:
-            if isinstance(kwargs["metadata"], dict):
-                metadata.update(kwargs["metadata"])
-            del kwargs["arguments"]
-
-        for name, value in kwargs.items():
-            if name.startswith("meta_") and len(name) > 5:
-                metadata[name[5:].lower()] = value
-            else:
-                other[name] = value
-
-        return metadata, other
-
-    def __init__(self, _identifier, _source, command, protocol=None, label=None, version=None, tags=None, storage=None, **kwargs):
-        from vot.workspace import LocalStorage
-        self._identifier = _identifier
-        self._source = _source
-        self._command = command
-        self._protocol = protocol
-        self._storage = LocalStorage(storage) if storage is not None else None
-        self._label = label if label is not None else _identifier
-        self._version = to_string(version) if not version is None else None
-        self._envvars, args = Tracker._collect_envvars(**kwargs)
-        self._metadata, args = Tracker._collect_metadata(**args)
-        self._arguments, self._args = Tracker._collect_arguments(**args)
-
-        if tags is None:
-            self._tags = []
-        elif isinstance(tags, str):
-            self._tags = tags.split(",")
-        self._tags = [tag.strip() for tag in self._tags]
-        self._tags = [tag for tag in self._tags if is_valid_identifier(tag)]
-
-        if not self._version is None and not is_valid_identifier(self._version):
-            raise TrackerException("Illegal version format", tracker=self)
-
-    def reversion(self, version=None) -> "Tracker":
-        """Creates a new tracker instance for specified version
+            The percentage of the given value.
+        """
+        return int((n * 100) / self._total)
 
-        Keyword Arguments:
-            version {[type]} -- New version (default: {None})
+    def absolute(self, value):
+        """Sets the progress to the given value.
 
-        Returns:
-            Tracker -- [description]
+        Args:
+            value: The value to set the progress to.
         """
-        if self.version == version or version is None:
-            return self
-        tracker = copy.copy(self)
-        tracker._version = version
-        return tracker
-
-    def runtime(self, log=False) -> "TrackerRuntime":
-        """Creates a new runtime instance for this tracker instance."""
-        if not self._command:
-            raise TrackerException("Tracker does not have an attached executable", tracker=self)
-
-        if not self._protocol in _runtime_protocols:
-            raise TrackerException("Runtime protocol '{}' not available".format(self._protocol), tracker=self)
-
-        return _runtime_protocols[self._protocol](self, self._command, log=log, envvars=self._envvars, arguments=self._arguments, **self._args)
-
-    def __eq__(self, other):
-        if other is None or not isinstance(other, Tracker):
-            return False
-
-        return self.reference == other.identifier
-
-    def __hash__(self):
-        return hash(self.reference)
-
-    def __repr__(self):
-        return self.reference
-
-    @property
-    def source(self):
-        return self._source
-
-    @property
-    def storage(self) -> "Storage":
-        return self._storage
-
-    @property
-    def identifier(self) -> str:
-        return self._identifier
-
-    @property
-    def label(self):
-        if self._version is None:
-            return self._label
+        if self._tqdm is None:
+            if self._total == 0:
+                return
+            prev = self._value
+            self._value = max(0, min(value, self._total))
+            if self._percent(prev) != self._percent(self._value):
+                print("%d %%" % self._percent(self._value))
         else:
-            return self._label + " (" + self._version + ")"
+            self._tqdm.update(value - self._tqdm.n)  # will also set self.n = b * bsize
+        
+    def relative(self, n):
+        """Increments the progress by the given value.
 
-    @property
-    def version(self) -> str:
-        return self._version
-
-    @property
-    def reference(self) -> str:
-        if self._version is None:
-            return self._identifier
+        Args:
+            n: The value to increment the progress by.
+        """
+        if self._tqdm is None:
+            if self._total == 0:
+                return
+            prev = self._value
+            self._value = max(0, min(self._value + n, self._total))
+            if self._percent(prev) != self._percent(self._value):
+                print("%d %%" % self._percent(self._value))
         else:
-            return self._identifier + "@" + self._version
+            self._tqdm.update(n)  # will also set self.n = b * bsize 
 
-    @property
-    def protocol(self) -> str:
-        """Returns the communication protocol used by this tracker.
+    def total(self, t):
+        """Sets the total number of steps.
 
-        Returns:
-            str: Communication protocol
+        Args:
+            t: The total number of steps.
         """
-        return self._protocol
-
-    def describe(self):
-        data = dict(command=self._command, label=self.label, protocol=self.protocol, arguments=self._arguments, env=self._envvars)
-        data.update(self._args)
-        return data
-
-    def metadata(self, key):
-        """Returns the metadata value for specified key."""
-        if not key in self._metadata:
-            return None
-        return self._metadata[key]
-
-    def tagged(self, tag):
-        """Returns true if the tracker is tagged with specified tag."""
-
-        return tag in self._tags
-
-ObjectStatus = namedtuple("ObjectStatus", ["region", "properties"])
-
-Objects = Union[List[ObjectStatus], ObjectStatus]
-class TrackerRuntime(ABC):
-    """Base class for tracker runtime implementations. """
-
-    def __init__(self, tracker: Tracker):
-        self._tracker = tracker
-
-    @property
-    def tracker(self) -> Tracker:
-        return self._tracker
+        if self._tqdm is None:
+            if self._total == 0:
+                return
+            self._total = t
+        else:
+            if self._tqdm.total == t:
+                return
+            self._tqdm.total = t
+            self._tqdm.refresh()
 
     def __enter__(self):
+        """Enters the context manager."""
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.stop()
-
-    @property
-    def multiobject(self):
-        return False
-
-    @abstractmethod
-    def stop(self):
-        pass
-
-    @abstractmethod
-    def restart(self):
-        """Restarts the tracker runtime, usually stars a new process."""
-        pass
-
-    @abstractmethod
-    def initialize(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
-        pass
-
-    @abstractmethod
-    def update(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
-        pass
-
-class RealtimeTrackerRuntime(TrackerRuntime):
-
-    def __init__(self, runtime: TrackerRuntime, grace: int = 1, interval: float = 0.1):
-        super().__init__(runtime.tracker)
-        self._runtime = runtime
-        self._grace = grace
-        self._interval = interval
-        self._countdown = 0
-        self._time = 0
-        self._out = None
-
-    @property
-    def multiobject(self):
-        return self._runtime.multiobject
-
-    def stop(self):
-        self._runtime.stop()
-        self._time = 0
-        self._out = None
-
-    def restart(self):
-        self._runtime.restart()
-        self._time = 0
-        self._out = None
-
-    def initialize(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
-        self._countdown = self._grace
-        self._out = None
-
-        out, prop, time = self._runtime.initialize(frame, new, properties)
-
-        if time > self._interval:
-            if self._countdown > 0:
-                self._countdown = self._countdown - 1
-                self._time = 0
-            else:
-                self._time = time - self._interval
-                self._out = out
-        else:
-            self._time = 0
-
-        return out, prop, time
-
+    def __exit__(self, exc_type, exc_value, traceback):
+        """Exits the context manager."""
+        self.close()
+
+    def close(self):
+        """Closes the progress bar."""
+        if self._tqdm:
+            self._tqdm.close()
+
+def extract_files(archive, destination, callback = None):
+    """Extracts all files from the given archive to the given destination.
+
+    Args:
+        archive: The archive to extract the files from.
+        destination: The destination to extract the files to.
+        callback: An optional callback function that is called after each file is extracted.
+    """
+    from zipfile import ZipFile
+
+    with ZipFile(file=archive) as zip_file:
+        # Loop over each file
+        total=len(zip_file.namelist())
+        for file in zip_file.namelist():
+
+            # Extract each file to another directory
+            # If you want to extract to current working directory, don't specify path
+            zip_file.extract(member=file, path=destination)
+            if callback:
+                callback(1, total)
+
+def read_properties(filename: str, delimiter: str = '=') -> typing.Dict[str, str]:
+    """Reads a given properties file with each line of the format key=value. Returns a dictionary containing the pairs.
+
+    Args:
+        filename (str): The name of the file to be read.
+        delimiter (str, optional): Key-value delimiter. Defaults to '='.
+
+    Returns:
+        [typing.Dict[str, str]]: Resuting properties as a dictionary
+    """
+    if not os.path.exists(filename):
+        return {}
+    open_kwargs = {'mode': 'r', 'newline': ''} if six.PY3 else {'mode': 'rb'}
+    matcher = re.compile("^([a-zA-Z0-9_\\-.]+) *{} *(.*)$".format(delimiter))
+    with open(filename, **open_kwargs) as pfile:
+        properties = dict()
+        for line in pfile.readlines():
+            groups = matcher.match(line.strip())
+            if not groups:
+                continue
+            properties[groups.group(1)] = groups.group(2)
+        return properties
 
-    def update(self, frame: Frame, _: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
+def write_properties(filename: str, dictionary: Mapping[str, Any], delimiter: str = '='):
+    """Writes the provided dictionary in key sorted order to a properties
+        file with each line in the format: key<delimiter>value
+
+    Args:
+        filename (str): the name of the file to be written
+        dictionary (Mapping[str, str]): a dictionary containing the key/value pairs.
+        delimiter (str, optional): _description_. Defaults to '='.
+    """
+
+    open_kwargs = {'mode': 'w', 'newline': ''} if six.PY3 else {'mode': 'wb'}
+    with open(filename, **open_kwargs) as csvfile:
+        writer = csv.writer(csvfile, delimiter=delimiter, escapechar='\\',
+                            quoting=csv.QUOTE_NONE)
+        writer.writerows(sorted(dictionary.items()))
+
+def file_hash(filename: str) -> Tuple[str, str]:
+    """Calculates MD5 and SHA1 hashes based on file content
+
+    Args:
+        filename (str): Filename of the file to open and analyze
+
+    Returns:
+        Tuple[str, str]: MD5 and SHA1 hashes as hexadecimal strings.
+    """
+    
+    bufsize = 65536  # lets read stuff in 64kb chunks!
+
+    md5 = hashlib.md5()
+    sha1 = hashlib.sha1()
+
+    with open(filename, 'rb') as f:
+        while True:
+            data = f.read(bufsize)
+            if not data:
+                break
+            md5.update(data)
+            sha1.update(data)
+
+    return md5.hexdigest(), sha1.hexdigest()
+
+def arg_hash(*args, **kwargs) -> str:
+    """Computes hash based on input positional and keyword arguments. 
+
+    The algorithm tries to convert all arguments to string, then enclose them with delimiters. The
+    positonal arguments are listed as is, keyword arguments are sorted and encoded with their keys as 
+    well as values.
+
+    Returns:
+        str: SHA1 hash as hexadecimal string
+    """
+    sha1 = hashlib.sha1()
+
+    for arg in args:
+        sha1.update(("(" + str(arg) + ")").encode("utf-8"))
+
+    for (key, val) in sorted(kwargs.items()):
+        sha1.update(("(" + str(key) + ":" + str(val) + ")").encode("utf-8"))
+
+    return sha1.hexdigest()
+
+def which(program: str) -> str:
+    """Locates an executable in system PATH list by its name.
+
+    Args:
+        program (str): Name of the executable
+
+    Returns:
+        str: Full path or None if not found
+    """
+
+    def is_exe(fpath):
+        """Checks if the given path is an executable file.
+        
+        Args:
+            fpath (str): Path to check
+            
+        Returns:
+            bool: True if the path is an executable file
+        """
+        return os.path.isfile(fpath) and os.access(fpath, os.X_OK)
 
-        if self._time > self._interval:
-            self._time = self._time - self._interval
-            return self._out, dict(), 0
+    fpath, _ = os.path.split(program)
+    if fpath:
+        if is_exe(program):
+            return program
+    else:
+        for path in os.environ["PATH"].split(os.pathsep):
+            exe_file = os.path.join(path, program)
+            if is_exe(exe_file):
+                return exe_file
+
+    return None
+
+def normalize_path(path, root=None):
+    """Normalizes the given path by making it absolute and removing redundant parts.
+
+    Args:
+        path (str): Path to normalize
+        root (str, optional): Root path to use if the given path is relative. Defaults to None.
+
+    Returns:
+        str: Normalized path
+    """
+    if os.path.isabs(path):
+        return path
+    if not root:
+        root = os.getcwd()
+    return os.path.normpath(os.path.join(root, path))
+
+def localize_path(path):
+    """Converts path to local format (backslashes on Windows, slashes on Linux)
+
+    Args:
+        path (str): Path to convert
+
+    Returns:
+        str: Converted path
+    """
+    if sys.platform.startswith("win"):
+        return path.replace("/", "\\")
+    else:
+        return path.replace("\\", "/")
+
+def to_string(n: Any) -> str:
+    """Converts object to string, returs empty string if object is None (so a bit different behaviour than
+    the original string conversion).
+
+    Args:
+        n (Any): Object of any kind
+
+    Returns:
+        str: String representation (using built-in conversion)
+    """
+    if n is None:
+        return ""
+    else:
+        return str(n)
+
+def to_number(val, max_n = None, min_n = None, conversion=int):
+    """Converts the given value to a number and checks if it is within the given range. If the value is not a number, 
+     a RuntimeError is raised.
+      
+    Args:
+        val (Any): Value to convert
+        max_n (int, optional): Maximum allowed value. Defaults to None.
+        min_n (int, optional): Minimum allowed value. Defaults to None.
+        conversion (function, optional): Conversion function. Defaults to int.
+    
+    Returns:
+        int: Converted value
+    """
+    try:
+        n = conversion(val)
+
+        if not max_n is None:
+            if n > max_n:
+                raise RuntimeError("Parameter higher than maximum allowed value ({}>{})".format(n, max_n))
+        if not min_n is None:
+            if n < min_n:
+                raise RuntimeError("Parameter lower than minimum allowed value ({}<{})".format(n, min_n))
+
+        return n
+    except ValueError:
+        raise RuntimeError("Number conversion error")
+
+def to_logical(val):
+    """Converts the given value to a logical value (True/False). If the value is not a logical value,
+    a RuntimeError is raised.
+
+    Args:
+        val (Any): Value to convert
+
+    Returns:
+        bool: Converted value
+    """
+    try:
+        if isinstance(val, str):
+            return val.lower() in ['true', '1', 't', 'y', 'yes']
         else:
-            self._out = None
-            self._time = 0
-
-        out, prop, time = self._runtime.update(frame, properties)
-
-        if time > self._interval:
-            if self._countdown > 0:
-                self._countdown = self._countdown - 1
-                self._time = 0
-            else:
-                self._time = time - self._interval
-                self._out = out
-
-        return out, prop, time
-
+            return bool(val)
 
-class PropertyInjectorTrackerRuntime(TrackerRuntime):
+    except ValueError:
+        raise RuntimeError("Logical value conversion error")
 
-    def __init__(self, runtime: TrackerRuntime, **kwargs):
-        super().__init__(runtime.tracker)
-        self._runtime = runtime
-        self._properties = {k : str(v) for k, v in kwargs.items()}
+def format_size(num, suffix="B"):
+    """Formats the given number as a human-readable size string. 
 
-    @property
-    def multiobject(self):
-        return self._runtime.multiobject
+    Args:
+        num (int): Number to format
+        suffix (str, optional): Suffix to use. Defaults to "B".
+
+    Returns:
+        str: Formatted string
+    """
+    for unit in ["", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"]:
+        if abs(num) < 1024.0:
+            return f"{num:3.1f}{unit}{suffix}"
+        num /= 1024.0
+    return f"{num:.1f}Yi{suffix}"
+
+def singleton(class_):
+    """Singleton decorator for classes. 
+
+    Args:
+        class_ (class): Class to decorate
+
+    Returns:
+        class: Decorated class
+
+    Example:
+        @singleton
+        class MyClass:
+            pass
+            
+        a = MyClass()
+    """
+    instances = {}
+    def getinstance(*args, **kwargs):
+        """Returns the singleton instance of the class. If the instance does not exist, it is created."""
+        if class_ not in instances:
+            instances[class_] = class_(*args, **kwargs)
+        return instances[class_]
+    return getinstance
+
+class ColoredFormatter(Formatter):
+    """Colored log formatter using colorama package.
+    """
 
-    def stop(self):
-        self._runtime.stop()
+    class Empty(object):
+        """An empty class used to copy :class:`~logging.LogRecord` objects without reinitializing them."""
 
-    def restart(self):
-        self._runtime.restart()
-
-    def initialize(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
-
-        if not properties is None:
-            tproperties = dict(properties)
-        else:
-            tproperties = dict()
-
-        tproperties.update(self._properties)
-
-        return self._runtime.initialize(frame, new, tproperties)
-
-
-    def update(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
-        return self._runtime.update(frame, new, properties)
+    def __init__(self, **kwargs):
+        """Initializes the formatter.
 
+        Args:
+            **kwargs: Keyword arguments passed to the base class
 
-class SingleObjectTrackerRuntime(TrackerRuntime):
+        """
+        super().__init__(**kwargs)
+        colorama.init()
 
-    def __init__(self, runtime: TrackerRuntime):
-        super().__init__(runtime.tracker)
-        self._runtime = runtime
+        self._styles = dict(
+            debug=colorama.Fore.GREEN,
+            verbose=colorama.Fore.BLACK,
+            info="",
+            notice=colorama.Fore.MAGENTA,
+            warning=colorama.Fore.YELLOW,
+            error=colorama.Fore.RED,
+            critical=colorama.Fore.RED + colorama.Style.BRIGHT,
+        )
 
-    @property
-    def multiobject(self):
-        return False
+    def format(self, record: LogRecord) -> str:
+        """Formats message by injecting colorama terminal codes for text coloring.
 
-    def stop(self):
-        self._runtime.stop()
+        Args:
+            record (LogRecord): Input log record
 
-    def restart(self):
-        self._runtime.restart()
+        Returns:
+            str: Formatted string
+        """
+        style = self._styles[record.levelname.lower()]
 
-    def initialize(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
+        copy = ColoredFormatter.Empty()
+        copy.__class__ = record.__class__
+        copy.__dict__.update(record.__dict__)
+        msg = record.msg if isinstance(record.msg, str) else str(record.msg)
+        copy.msg = style + msg + colorama.Style.RESET_ALL
+        record = copy
+        # Delegate the remaining formatting to the base formatter.
+        return Formatter.format(self, record)
+
+
+class ThreadPoolExecutor(futures.ThreadPoolExecutor):
+    """Thread pool executor with a shutdown method that waits for all threads to finish. 
+    """
+
+    def __init__(self, *args, **kwargs):
+        """Initializes the thread pool executor."""
+        super().__init__(*args, **kwargs)
+        #self._work_queue = Queue.Queue(maxsize=maxsize)
 
-        if isinstance(new, list) and len(new) != 1: raise TrackerException("Only supports single object tracking", tracker=self.tracker)
-        status = self._runtime.initialize(frame, new, properties)
-        if isinstance(status, list): status = status[0]
-        return status
+    def shutdown(self, wait=True):
+        """Shuts down the thread pool executor. If wait is True, waits for all threads to finish.
 
-    def update(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
+        Args:
+            wait (bool, optional): Wait for all threads to finish. Defaults to True.
+        """
+        import queue
+        with self._shutdown_lock:
+            self._shutdown = True
+            try:
+                while True:
+                    item = self._work_queue.get_nowait()
+                    item.future.cancel()
+            except queue.Empty:
+                pass
+            self._work_queue.put(None)
+        if wait:
+            for t in self._threads:
+                t.join()
 
-        if not new is None: raise TrackerException("Only supports single object tracking", tracker=self.tracker)
-        status = self._runtime.update(frame, new, properties)
-        if isinstance(status, list): status = status[0]
-        return status
+class Timer(object):
+    """Simple timer class for measuring elapsed time."""
 
-class MultiObjectTrackerRuntime(TrackerRuntime):
-    """ This is a wrapper for tracker runtimes that do not support multi object tracking. It is still work in progress."""
+    def __init__(self, name=None):
+        """Initializes the timer.
 
-    def __init__(self, runtime: TrackerRuntime):
-        super().__init__(runtime.tracker)
-        if self._runtime.multiobject:
-            self._runtime = runtime
-        else:
-            self._runtime = [runtime]
-            self._used = 0
+        Args:
+            name (str, optional): Name of the timer. Defaults to None.
+        """
+        self.name = name
 
-    @property
-    def multiobject(self):
-        return True
-
-    def stop(self):
-        if isinstance(self._runtime, TrackerRuntime):
-            self._runtime.stop()
-        else:
-            for r in self._runtime:
-                r.stop()
+    def __enter__(self):
+        """Starts the timer."""
+        self._tstart = time.time()
 
-    def restart(self):
-        if isinstance(self._runtime, TrackerRuntime):
-            self._runtime.restart()
+    def __exit__(self, type, value, traceback):
+        """Stops the timer and prints the elapsed time."""
+        elapsed = time.time() - self._tstart
+        if self.name:
+            print('[%s]: %.4fs' % (self.name, elapsed))
         else:
-            for r in self._runtime:
-                r.restart()
-
-    def initialize(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
-        if isinstance(self._runtime, TrackerRuntime):
-            return self._runtime.initialize(frame, new, properties)
-        if isinstance(new, ObjectStatus):
-            new = [new]
-
-        self._used = 0
-        status = []
-        for i, o in enumerate(new):
-            if i >= len(self._runtime):
-                self._runtime.append(self._tracker.runtime())
-                self._runtime.initialize(frame, new, properties)
-
-        if isinstance(status, list): status = status[0]
-        return status
-
-    def update(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
-
-        if not new is None: raise TrackerException("Only supports single object tracking")
-        status = self._runtime.update(frame, new, properties)
-        if isinstance(status, list): status = status[0]
-        return status
-
-try:
-
-    from vot.tracker.trax import TraxTrackerRuntime, trax_matlab_adapter, trax_python_adapter, trax_octave_adapter
-
-    _runtime_protocols["trax"] = TraxTrackerRuntime
-    _runtime_protocols["traxmatlab"] = trax_matlab_adapter
-    _runtime_protocols["traxpython"] = trax_python_adapter
-    _runtime_protocols["traxoctave"] = trax_octave_adapter
-
-except OSError:
-    pass
-
-except ImportError:
-    logger.error("Unable to import support for TraX protocol")
-    pass
-
-from vot.tracker.results import Trajectory, Results
+            print('Elapsed: %.4fs' % elapsed)
```

### Comparing `vot-toolkit-0.6.2/vot/tracker/dummy.py` & `vot-toolkit-0.6.4/vot/tracker/dummy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+""" Dummy tracker for testing purposes. """
+
 from __future__ import absolute_import
 import os
 from sys import path
 import time
 
 def _main():
     """ Dummy tracker main function for testing purposes."""
```

### Comparing `vot-toolkit-0.6.2/vot/utilities/cli.py` & `vot-toolkit-0.6.4/vot/utilities/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Command line interface for the toolkit. This module provides a command line interface for the toolkit. It is used to run experiments, manage trackers and datasets, and to perform other tasks."""
+
 import os
 import sys
 import argparse
 import logging
 import yaml
 from datetime import datetime
 
@@ -14,37 +16,39 @@
 
 logger = get_logger()
 
 class EnvDefault(argparse.Action):
     """Argparse action that resorts to a value in a specified envvar if no value is provided via program arguments.
     """
     def __init__(self, envvar, required=True, default=None, separator=None, **kwargs):
+        """Initialize the action"""
         if not default and envvar:
             if envvar in os.environ:
                 default = os.environ[envvar]
         if separator:
             default = default.split(separator)
         if required and default:
             required = False
         self.separator = separator
         super(EnvDefault, self).__init__(default=default, required=required,
                                          **kwargs)
 
     def __call__(self, parser, namespace, values, option_string=None):
+        """Call the action"""
         if self.separator:
             values = values.split(self.separator)
         setattr(namespace, self.dest, values)
 
 def do_test(config: argparse.Namespace):
     """Run a test for a tracker
 
     Args:
         config (argparse.Namespace): Configuration
     """
-    from vot.dataset.dummy import DummySequence
+    from vot.dataset.dummy import generate_dummy
     from vot.dataset import load_sequence, Frame
     from vot.tracker import ObjectStatus
     from vot.experiment.helpers import MultiObjectHelper
 
     trackers = Registry(config.registry)
 
     if not config.tracker:
@@ -57,14 +61,23 @@
     if not config.tracker in trackers:
         logger.error("Tracker does not exist")
         return
 
     tracker = trackers[config.tracker]
 
     def visualize(axes, frame: Frame, reference, state):
+        """Visualize the frame and the state of the tracker. 
+        
+        Args:
+            axes (matplotlib.axes.Axes): The axes to draw on.
+            frame (Frame): The frame to draw.
+            reference (list): List of references.
+            state (ObjectStatus): The state of the tracker.
+            
+        """
         axes.clear()
         handle.image(frame.channel())
         if not isinstance(state, list):
             state = [state]
         for gt, st in zip(reference, state):
             handle.style(color="green").region(gt)
             handle.style(color="red").region(st.region)
@@ -72,23 +85,28 @@
     try:
 
         runtime = tracker.runtime(log=True)
 
         logger.info("Generating dummy sequence")
 
         if config.sequence is None:
-            sequence = DummySequence(50, objects=3 if runtime.multiobject else 1)
+            sequence = generate_dummy(50, objects=3 if runtime.multiobject else 1)
         else:
             sequence = load_sequence(normalize_path(config.sequence))
 
         logger.info("Obtaining runtime for tracker %s", tracker.identifier)
 
         context = {"continue" : True}
 
         def on_press(event):
+            """Callback for key press event.
+            
+            Args:
+                event (matplotlib.backend_bases.Event): The event.
+            """
             if event.key == 'q':
                 context["continue"] = False
 
         if config.visualize:
             import matplotlib.pylab as plt
             from vot.utilities.draw import MatplotlibDrawHandle
             figure = plt.figure()
@@ -109,15 +127,15 @@
 
         if config.visualize:
             visualize(axes, frame, [frame.object(x) for x in helper.objects(0)], state)
             figure.canvas.draw()
 
         for i in range(1, len(sequence)):
             
-            logger.info("Processing frame %d/%d", i, sequence.length-1)
+            logger.info("Processing frame %d/%d", i, len(sequence)-1)
             frame = sequence.frame(i)
             state, _ = runtime.update(frame, [ObjectStatus(frame.object(x), {}) for x in helper.new(i)])
 
             if config.visualize:
                 visualize(axes, frame, [frame.object(x) for x in helper.objects(i)], state)
                 figure.canvas.draw()
                 figure.canvas.flush_events()
@@ -136,14 +154,19 @@
         if runtime:
             runtime.stop()
     except KeyboardInterrupt:
         if runtime:
             runtime.stop()
 
 def do_workspace(config: argparse.Namespace):
+    """Initialize / manage a workspace.
+
+    Args:
+        config (argparse.Namespace): Configuration
+    """
 
     from vot.workspace import WorkspaceException
 
     if config.stack is None and os.path.isfile(os.path.join(config.workspace, "configuration.m")):
         from vot.utilities.migration import migrate_matlab_workspace
         migrate_matlab_workspace(config.workspace)
         return
@@ -167,14 +190,19 @@
     try:
         Workspace.initialize(config.workspace, default_config, download=not config.nodownload)
         logger.info("Initialized workspace in '%s'", config.workspace)
     except WorkspaceException as we:
         logger.error("Error during workspace initialization: %s", we)
 
 def do_evaluate(config: argparse.Namespace):
+    """Run an evaluation for a tracker on an experiment stack and a set of sequences.
+    
+    Args:
+        config (argparse.Namespace): Configuration    
+    """
 
     from vot.experiment import run_experiment
 
     workspace = Workspace.load(config.workspace)
 
     logger.debug("Loaded workspace in '%s'", config.workspace)
 
@@ -203,14 +231,19 @@
 
     except KeyboardInterrupt:
         logger.info("Evaluation interrupted by the user")
     except TrackerException as te:
         logger.error("Evaluation interrupted by tracker error: {}".format(te))
 
 def do_analysis(config: argparse.Namespace):
+    """Run an analysis for a tracker on an experiment stack and a set of sequences.
+
+    Args:
+        config (argparse.Namespace): Configuration
+    """
 
     from vot.analysis import AnalysisProcessor, process_stack_analyses
     from vot.document import generate_document
 
     workspace = Workspace.load(config.workspace)
 
     logger.debug("Loaded workspace in '%s'", config.workspace)
@@ -231,15 +264,15 @@
         return
 
     logger.debug("Running analysis for %d trackers", len(trackers))
 
     if config.workers == 1:
 
         if config.debug:
-            from vot.analysis._processor import DebugExecutor
+            from vot.analysis.processor import DebugExecutor
             logging.getLogger("concurrent.futures").setLevel(logging.DEBUG)
             executor = DebugExecutor()
         else:
             from vot.utilities import ThreadPoolExecutor
             executor = ThreadPoolExecutor(1)
 
     else:
@@ -277,20 +310,19 @@
         executor.shutdown(wait=True)
 
     
 def do_pack(config: argparse.Namespace):
     """Package results to a ZIP file so that they can be submitted to a challenge.
 
     Args:
-        config ([type]): [description]
+        config (argparse.Namespace): Configuration
     """
 
     import zipfile, io
     from shutil import copyfileobj
-    from vot.utilities import flatten
 
     workspace = Workspace.load(config.workspace)
 
     logger.debug("Loaded workspace in '%s'", config.workspace)
 
     registry = Registry(list(workspace.registry) + config.registry, root=config.workspace)
 
@@ -393,14 +425,15 @@
 
         logger.setLevel(logging.INFO)
 
         if args.debug or check_debug():
             logger.setLevel(logging.DEBUG)
 
         def check_version():
+            """Check if a newer version of the toolkit is available."""
             update, version = check_updates()
             if update:
                 logger.warning("A newer version of the VOT toolkit is available (%s), please update.", version)
 
         if args.action == "test":
             check_version()
             do_test(args)
```

### Comparing `vot-toolkit-0.6.2/vot/utilities/migration.py` & `vot-toolkit-0.6.4/vot/utilities/migration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,46 @@
-
+""" Migration utilities for old workspaces (legacy Matlab toolkit)"""
 
 import os
 import re
 import logging
 
 import yaml
 import numpy as np
 
 from vot.tracker import is_valid_identifier
 from vot.stack import resolve_stack
 from vot.workspace import WorkspaceException
 
-def migrate_matlab_workspace(directory):
+def migrate_matlab_workspace(directory: str):
+    """ Migrates a legacy matlab workspace to the new format.
+    
+    Args:
+        directory (str): The directory of the workspace.
+        
+    Raises:
+        WorkspaceException: If the workspace is already initialized.
+        WorkspaceException: If the workspace is not a legacy workspace.
+    """
 
     logger = logging.getLogger("vot")
 
     logger.info("Attempting to migrate workspace in %s", directory)
 
     def scan_text(pattern, content, default=None):
+        """ Scans the text for a pattern and returns the first match.
+        
+        Args:
+            pattern (str): The pattern to search for.
+            content (str): The content to search in.
+            default (str): The default value if no match is found.
+            
+        Returns:
+            str: The first match or the default value.
+        """
         matches = re.findall(pattern, content)
         if not len(matches) == 1:
             return default
         return matches[0]
 
     config_file = os.path.join(directory, "config.yaml")
     if os.path.isfile(config_file):
```

### Comparing `vot-toolkit-0.6.2/vot/utilities/notebook.py` & `vot-toolkit-0.6.4/vot/utilities/notebook.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+""" This module contains functions for visualization in Jupyter notebooks. """
 
 import os
 import io
 from threading import Thread, Condition
 
 def is_notebook():
+    """ Returns True if the current environment is a Jupyter notebook. 
+    
+    Returns:
+        bool: True if the current environment is a Jupyter notebook.    
+    """
     try:
         from IPython import get_ipython
         if get_ipython() is None:
             raise ImportError("console")
         if 'IPKernelApp' not in get_ipython().config:  # pragma: no cover
             raise ImportError("console")
         if 'VSCODE_PID' in os.environ:  # pragma: no cover
@@ -20,16 +26,22 @@
 if is_notebook():
    
     from IPython.display import display
     from ipywidgets import widgets
     from vot.utilities.draw import ImageDrawHandle
 
     class SequenceView(object):
+        """ A widget for visualizing a sequence. """
 
         def __init__(self):
+            """ Initializes a new instance of the SequenceView class. 
+            
+            Args:
+                sequence (Sequence): The sequence to visualize.
+            """
 
             self._handle = ImageDrawHandle(sequence.frame(0).image())
 
             self._button_restart = widgets.Button(description='Restart')
             self._button_next = widgets.Button(description='Next')
             self._button_play = widgets.Button(description='Run')
             self._frame = widgets.Label(value="")
@@ -39,24 +51,42 @@
 
             state = dict(frame=0, auto=False, alive=True, region=None)
             condition = Condition()
 
             self._buttons = widgets.HBox(children=(frame, self._button_restart, self._button_next, button_play, frame2))
 
         def _push_image(handle):
+            """ Pushes an image to the widget. 
+
+            Args:
+                handle (ImageDrawHandle): The image handle.
+            """
             with io.BytesIO() as output:
                 handle.snapshot.save(output, format="PNG")
                 return output.getvalue()
 
     def visualize_tracker(tracker: "Tracker", sequence: "Sequence"):
+        """ Visualizes a tracker in a Jupyter notebook.
+
+        Args:
+            tracker (Tracker): The tracker to visualize.
+            sequence (Sequence): The sequence to visualize.
+        """
         from IPython.display import display
         from ipywidgets import widgets
         from vot.utilities.draw import ImageDrawHandle
 
         def encode_image(handle):
+            """ Encodes an image so that it can be displayed in a Jupyter notebook.
+            
+            Args:
+                handle (ImageDrawHandle): The image handle.
+            
+            Returns:
+                bytes: The encoded image."""
             with io.BytesIO() as output:
                 handle.snapshot.save(output, format="PNG")
                 return output.getvalue()
 
         handle = ImageDrawHandle(sequence.frame(0).image())
 
         button_restart = widgets.Button(description='Restart')
@@ -71,14 +101,15 @@
         condition = Condition()
 
         buttons = widgets.HBox(children=(frame, button_restart, button_next, button_play, frame2))
 
         image.value = encode_image(handle)
 
         def run():
+            """ Runs the tracker. """
 
             runtime = tracker.runtime()
 
             while state["alive"]:
 
                 if state["frame"] == 0:
                     state["region"], _, _ = runtime.initialize(sequence.frame(0), sequence.groundtruth(0))
@@ -86,30 +117,32 @@
                     state["region"], _, _ = runtime.update(sequence.frame(state["frame"]))
 
                 update_image()
 
                 with condition:
                     condition.wait()
 
-                    if state["frame"] == sequence.length:
+                    if state["frame"] == len(sequence):
                         state["alive"] = False
                         continue
 
                     state["frame"] = state["frame"] + 1
 
 
         def update_image():
+            """ Updates the image. """
             handle.image(sequence.frame(state["frame"]).image())
             handle.style(color="green").region(sequence.frame(state["frame"]).groundtruth())
             if state["region"]:
                 handle.style(color="red").region(state["region"])
             image.value = encode_image(handle)
             frame.value = "Frame: " + str(state["frame"] - 1)
 
         def on_click(button):
+            """ Handles a button click. """
             if button == button_next:
                 with condition:
                     state["auto"] = False
                     condition.notify()
             if button == button_restart:
                 with condition:
                     state["frame"] = 0
@@ -122,30 +155,48 @@
 
         button_next.on_click(on_click)
         button_restart.on_click(on_click)
         button_play.on_click(on_click)
         widgets.jslink((frame, "value"), (frame2, "value"))
 
         def on_update(_):
+            """ Handles a widget update."""
             with condition:
                 if state["auto"]:
                     condition.notify()
 
         frame2.observe(on_update, names=("value", ))
 
         thread = Thread(target=run)
         display(widgets.Box([widgets.VBox(children=(image, buttons))]))
         thread.start()
 
     def visualize_results(experiment: "Experiment", sequence: "Sequence"):
+        """ Visualizes the results of an experiment in a Jupyter notebook.
+        
+        Args:
+            experiment (Experiment): The experiment to visualize.
+            sequence (Sequence): The sequence to visualize.
+            
+        """
+
         from IPython.display import display
         from ipywidgets import widgets
         from vot.utilities.draw import ImageDrawHandle
 
         def encode_image(handle):
+            """ Encodes an image so that it can be displayed in a Jupyter notebook.
+            
+            Args:
+                handle (ImageDrawHandle): The image handle.
+            
+            Returns:
+                bytes: The encoded image.
+            """
+
             with io.BytesIO() as output:
                 handle.snapshot.save(output, format="PNG")
                 return output.getvalue()
 
         handle = ImageDrawHandle(sequence.frame(0).image())
 
         button_restart = widgets.Button(description='Restart')
@@ -160,14 +211,15 @@
         condition = Condition()
 
         buttons = widgets.HBox(children=(frame, button_restart, button_next, button_play, frame2))
 
         image.value = encode_image(handle)
 
         def run():
+            """ Runs the tracker. """
 
             runtime = tracker.runtime()
 
             while state["alive"]:
 
                 if state["frame"] == 0:
                     state["region"], _, _ = runtime.initialize(sequence.frame(0), sequence.groundtruth(0))
@@ -175,30 +227,32 @@
                     state["region"], _, _ = runtime.update(sequence.frame(state["frame"]))
 
                 update_image()
 
                 with condition:
                     condition.wait()
 
-                    if state["frame"] == sequence.length:
+                    if state["frame"] == len(sequence):
                         state["alive"] = False
                         continue
 
                     state["frame"] = state["frame"] + 1
 
 
         def update_image():
+            """ Updates the image. """
             handle.image(sequence.frame(state["frame"]).image())
             handle.style(color="green").region(sequence.frame(state["frame"]).groundtruth())
             if state["region"]:
                 handle.style(color="red").region(state["region"])
             image.value = encode_image(handle)
             frame.value = "Frame: " + str(state["frame"] - 1)
 
         def on_click(button):
+            """ Handles a button click. """
             if button == button_next:
                 with condition:
                     state["auto"] = False
                     condition.notify()
             if button == button_restart:
                 with condition:
                     state["frame"] = 0
@@ -211,14 +265,15 @@
 
         button_next.on_click(on_click)
         button_restart.on_click(on_click)
         button_play.on_click(on_click)
         widgets.jslink((frame, "value"), (frame2, "value"))
 
         def on_update(_):
+            """ Handles a widget update."""
             with condition:
                 if state["auto"]:
                     condition.notify()
 
         frame2.observe(on_update, names=("value", ))
 
         thread = Thread(target=run)
```

### Comparing `vot-toolkit-0.6.2/vot/workspace/__init__.py` & `vot-toolkit-0.6.4/vot/workspace/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""This module contains the Workspace class that represents the main junction of trackers, datasets and experiments."""
 
 import os
 import typing
 import importlib
 
 import yaml
 from lazy_object_proxy import Proxy
@@ -10,29 +11,38 @@
 
 from .. import ToolkitException, get_logger
 from ..dataset import Dataset, load_dataset
 from ..tracker import Registry, Tracker
 from ..stack import Stack, resolve_stack
 from ..utilities import normalize_path
 from ..document import ReportConfiguration
-from .storage import LocalStorage, Storage, NullStorage, StorageConfiguration
+from .storage import LocalStorage, Storage, NullStorage
 
 
 _logger = get_logger()
 
 class WorkspaceException(ToolkitException):
     """Errors related to workspace raise this exception
     """
     pass
 
 class StackLoader(Attribute):
     """Special attribute that converts a string or a dictionary input to a Stack object.
     """
 
     def coerce(self, value, context: typing.Optional[CoerceContext]):
+        """Coerce a value to a Stack object
+        
+        Args:
+            value (typing.Any): Value to coerce
+            context (typing.Optional[CoerceContext]): Coercion context
+            
+        Returns:
+            Stack: Coerced value
+        """
         importlib.import_module("vot.analysis")
         importlib.import_module("vot.experiment")
         if isinstance(value, str):
 
             stack_file = resolve_stack(value, context.parent.directory)
 
             if stack_file is None:
@@ -40,30 +50,37 @@
 
             with open(stack_file, 'r') as fp:
                 stack_metadata = yaml.load(fp, Loader=yaml.BaseLoader)
                 return Stack(value, context.parent, **stack_metadata)
         else:
             return Stack(None, context.parent, **value)
 
-    def dump(self, value):
+    def dump(self, value: "Stack") -> str:
+        """Dump a Stack object to a string or a dictionary
+        
+        Args:
+            value (Stack): Value to dump
+            
+        Returns:
+            str: Dumped value
+        """
         if value.name is None:
             return value.dump()
         else:
             return value.name
 
 class Workspace(Attributee):
     """Workspace class represents the main junction of trackers, datasets and experiments. Each workspace performs 
     given experiments on a provided dataset.
     """
 
     registry = List(String(transformer=lambda x, ctx: normalize_path(x, ctx.parent.directory)))
     stack = StackLoader()
     sequences = String(default="sequences")
     report = Nested(ReportConfiguration)
-    results = Nested(StorageConfiguration)
 
     @staticmethod
     def initialize(directory: str, config: typing.Optional[typing.Dict] = None, download: bool = True) -> None:
         """Initialize a new workspace in a given directory with the given config
 
         Args:
             directory (str): Root for workspace storage
@@ -147,15 +164,15 @@
         instead use the static Workspace.load method.
 
         Args:
             directory ([type]): [description]
         """
         self._directory = directory
 
-        self._storage = Proxy(lambda: LocalStorage(directory, self.results) if directory is not None else NullStorage())
+        self._storage = Proxy(lambda: LocalStorage(directory) if directory is not None else NullStorage())
         
         super().__init__(**kwargs)
 
         
         dataset_directory = normalize_path(self.sequences, directory)
 
         if not self.stack.dataset is None:
```

### Comparing `vot-toolkit-0.6.2/vot/workspace/storage.py` & `vot-toolkit-0.6.4/vot/experiment/multirun.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,375 +1,249 @@
+"""Multi-run experiments. This module contains the implementation of multi-run experiments. 
+ Multi-run experiments are used to run a tracker multiple times on the same sequence. """
+from typing import Callable
 
-import os
-import pickle
+from vot.dataset import Sequence
+from vot.region import Special, calculate_overlap
 
-from abc import ABC, abstractmethod
-import typing
+from attributee import Boolean, Integer, Float, List, String
 
-import cachetools
+from vot.experiment import Experiment, experiment_registry
+from vot.tracker import Tracker, Trajectory, ObjectStatus
 
-from attributee.object import class_fullname
+class MultiRunExperiment(Experiment):
+    """Base class for multi-run experiments. Multi-run experiments are used to run a tracker multiple times on the same sequence."""
 
-from ..experiment import Experiment
-from ..dataset import Sequence
-from ..tracker import Tracker, Results
+    repetitions = Integer(val_min=1, default=1)
+    early_stop = Boolean(default=True)
 
-from attributee import Attributee, Boolean
+    def _can_stop(self, tracker: Tracker, sequence: Sequence):
+        """Check whether the experiment can be stopped early.
+        
+        Args:
+            tracker (Tracker): The tracker to be checked.
+            sequence (Sequence): The sequence to be checked.
+            
+        Returns:
+            bool: True if the experiment can be stopped early, False otherwise.
+        """
+        if not self.early_stop:
+            return False
+        
+        for o in sequence.objects():
 
-class StorageConfiguration(Attributee):
-    binary = Boolean(default=True)
+            trajectories = self.gather(tracker, sequence, objects=[o])
+            if len(trajectories) < 3:
+                return False
+        
+            for trajectory in trajectories[1:]:
+                if not trajectory.equals(trajectories[0]):
+                    return False
 
-class Storage(ABC):
-    """Abstract superclass for workspace storage abstraction
-    """
+        return True
 
-    @abstractmethod
-    def results(self, tracker: Tracker, experiment: Experiment, sequence: Sequence) -> Results:
-        """Returns results object for the given tracker, experiment, sequence combination
+    def scan(self, tracker: Tracker, sequence: Sequence):
+        """Scan the results of the experiment for the given tracker and sequence.
 
         Args:
-            tracker (Tracker): Selected tracker
-            experiment (Experiment): Selected experiment
-            sequence (Sequence): Selected sequence
-        """
-        pass
+            tracker (Tracker): The tracker to be scanned.
+            sequence (Sequence): The sequence to be scanned.
 
-    @property
-    def config(self) -> StorageConfiguration:
-        return StorageConfiguration()
-
-    @abstractmethod
-    def documents(self) -> typing.List[str]:
-        """Lists documents in the storage.
+        Returns:
+            [tuple]: A tuple containing three elements. The first element is a boolean indicating whether the experiment is complete. The second element is a list of files that are present. The third element is the results object.
         """
-        pass
+        
+        results = self.results(tracker, sequence)
 
-    @abstractmethod
-    def folders(self) -> typing.List[str]:
-        """Lists folders in the storage.
-        """
-        pass
+        files = []
+        complete = True
+        multiobject = len(sequence.objects()) > 1
+        assert self._multiobject or not multiobject
+
+        for o in sequence.objects():
+            prefix = sequence.name if not multiobject else "%s_%s" % (sequence.name, o)
+            for i in range(1, self.repetitions+1):
+                name = "%s_%03d" % (prefix, i)
+                if Trajectory.exists(results, name):
+                    files.extend(Trajectory.gather(results, name))
+                elif self._can_stop(tracker, sequence):
+                    break
+                else:
+                    complete = False
+                    break
 
-    @abstractmethod
-    def write(self, name:str, binary: bool = False):
-        """Opens the given file entry for writing, returns opened handle.
+        return complete, files, results
 
+    def gather(self, tracker: Tracker, sequence: Sequence, objects = None, pad = False):
+        """Gather trajectories for the given tracker and sequence.
+        
         Args:
-            name (str): File name.
-            binary (bool, optional): Open file in binary mode. Defaults to False.
+            tracker (Tracker): The tracker to be used.
+            sequence (Sequence): The sequence to be used.
+            objects (list, optional): The list of objects to be gathered. Defaults to None.
+            pad (bool, optional): Whether to pad the list of trajectories with None values. Defaults to False.
+            
+        Returns:
+            list: The list of trajectories.
         """
-        pass
+        trajectories = list()
 
-    @abstractmethod
-    def read(self, name, binary=False):
-        """Opens the given file entry for reading, returns opened handle.
+        multiobject = len(sequence.objects()) > 1
 
-        Args:
-            name (str): File name.
-            binary (bool, optional): Open file in binary mode. Defaults to False.
-        """
-        pass
+        assert self._multiobject or not multiobject
+        results = self.results(tracker, sequence)
 
-    @abstractmethod
-    def isdocument(self, name: str) -> bool:
-        """Checks if given name is a document/file in this storage.
+        if objects is None:
+            objects = list(sequence.objects())
 
-        Args:
-            name (str): Name of the entry to check
+        for o in objects:
+            prefix = sequence.name if not multiobject else "%s_%s" % (sequence.name, o)
+            for i in range(1, self.repetitions+1):
+                name =  "%s_%03d" % (prefix, i)
+                if Trajectory.exists(results, name):
+                    trajectories.append(Trajectory.read(results, name))
+                elif pad:
+                    trajectories.append(None)
+        return trajectories
 
-        Returns:
-            bool: Returns True if entry is a document, False otherwise.
-        """
-        pass
+@experiment_registry.register("unsupervised")
+class UnsupervisedExperiment(MultiRunExperiment):
+    """Unsupervised experiment. This experiment is used to run a tracker multiple times on the same sequence without any supervision."""
 
-    @abstractmethod
-    def isfolder(self, name) -> bool:
-        """Checks if given name is a folder in this storage.
+    multiobject = Boolean(default=False)
 
-        Args:
-            name (str): Name of the entry to check
+    @property
+    def _multiobject(self) -> bool:
+        """Whether the experiment is multi-object or not.
 
         Returns:
-            bool: Returns True if entry is a folder, False otherwise.
+            bool: True if the experiment is multi-object, False otherwise.
         """
-        pass
+        return self.multiobject
 
-    @abstractmethod
-    def delete(self, name) -> bool:
-        """Deletes a given document.
+    def execute(self, tracker: Tracker, sequence: Sequence, force: bool = False, callback: Callable = None):
+        """Execute the experiment for the given tracker and sequence.
 
         Args:
-            name (str): File name.
+            tracker (Tracker): The tracker to be used.
+            sequence (Sequence): The sequence to be used.
+            force (bool, optional): Whether to force the execution. Defaults to False.
+            callback (Callable, optional): The callback to be used. Defaults to None.
+        """
 
+        from .helpers import MultiObjectHelper
 
-        Returns:
-            bool: Returns True if successful, False otherwise.
-        """
-        pass
+        results = self.results(tracker, sequence)
 
-    @abstractmethod
-    def substorage(self, name: str) -> "Storage":
-        """Returns a substorage, storage object with root in a subfolder.
+        multiobject = len(sequence.objects()) > 1
+        assert self._multiobject or not multiobject
 
-        Args:
-            name (str): Name of the entry, must be a folder
+        helper = MultiObjectHelper(sequence)
 
-        Returns:
-            Storage: Storage object
-        """
-        pass
+        def result_name(sequence, o, i):
+            """Get the name of the result file."""
+            return "%s_%s_%03d" % (sequence.name, o, i) if multiobject else "%s_%03d" % (sequence.name, i)
 
-    @abstractmethod
-    def copy(self, localfile: str, destination: str):
-        """Copy a document to another location
+        with self._get_runtime(tracker, sequence, self._multiobject) as runtime:
 
-        Args:
-            localfile (str): Original location
-            destination (str): New location
-        """
-        pass
+            for i in range(1, self.repetitions+1):
 
-class NullStorage(Storage):
-    """An implementation of dummy storage that does not save anything
-    """
-
-    #docstr_coverage:inherited
-    def results(self, tracker: Tracker, experiment: Experiment, sequence: Sequence):
-        return Results(self)
-
-    def __repr__(self) -> str:
-        return "<Null storage: {}>".format(self._root)
-
-    #docstr_coverage:inherited
-    def write(self, name, binary=False):
-        if binary:
-            return open(os.devnull, "wb")
-        else:
-            return open(os.devnull, "w")
-
-    #docstr_coverage:inherited
-    def documents(self):
-        return []
-
-    #docstr_coverage:inherited
-    def folders(self):
-        return []
-
-    #docstr_coverage:inherited
-    def read(self, name, binary=False):
-        return None
-
-    #docstr_coverage:inherited
-    def isdocument(self, name):
-        return False
-
-    #docstr_coverage:inherited
-    def isfolder(self, name):
-        return False
-
-    #docstr_coverage:inherited
-    def delete(self, name) -> bool:
-        return False
-
-    #docstr_coverage:inherited
-    def substorage(self, name):
-        return NullStorage()
-
-    #docstr_coverage:inherited
-    def copy(self, localfile, destination):
-        return
-
-class LocalStorage(Storage):
-    """Storage backed by the local filesystem.
-    """
-
-    def __init__(self, root: str, config: StorageConfiguration = None):
-        self._root = root
-        self._results = os.path.join(root, "results")
-        self._config = config if config is not None else StorageConfiguration()
+                trajectories = {}
 
-    def __repr__(self) -> str:
-        return "<Local storage: {}>".format(self._root)
+                for o in helper.all(): trajectories[o] = Trajectory(len(sequence))
 
-    @property
-    def config(self) -> StorageConfiguration:
-        return self._config
+                if all([Trajectory.exists(results, result_name(sequence, o, i)) for o in trajectories.keys()]) and not force:
+                    continue
 
-    @property
-    def base(self) -> str:
-        return self._root
+                if self._can_stop(tracker, sequence):
+                    return
+
+                _, elapsed = runtime.initialize(sequence.frame(0), [ObjectStatus(self._get_initialization(sequence, 0, x), {}) for x in helper.new(0)])
+
+                for x in helper.new(0):
+                    trajectories[x].set(0, Special(Trajectory.INITIALIZATION), {"time": elapsed})
+
+                for frame in range(1, len(sequence)):
+                    state, elapsed = runtime.update(sequence.frame(frame), [ObjectStatus(self._get_initialization(sequence, 0, x), {}) for x in helper.new(frame)])
+
+                    if not isinstance(state, list):
+                        state = [state]
+
+                    for x, object in zip(helper.objects(frame), state):
+                        object.properties["time"] = elapsed # TODO: what to do with time stats?
+                        trajectories[x].set(frame, object.region, object.properties)
 
-    def results(self, tracker: Tracker, experiment: Experiment, sequence: Sequence):
-        storage = LocalStorage(os.path.join(self._results, tracker.reference, experiment.identifier, sequence.name))
-        return Results(storage)
-
-    def documents(self):
-        return [name for name in os.listdir(self._root) if os.path.isfile(os.path.join(self._root, name))]
-
-    def folders(self):
-        return [name for name in os.listdir(self._root) if os.path.isdir(os.path.join(self._root, name))]
-
-    def write(self, name: str, binary: bool = False):
-        full = os.path.join(self.base, name)
-        os.makedirs(os.path.dirname(full), exist_ok=True)
-
-        if binary:
-            return open(full, mode="wb")
-        else:
-            return open(full, mode="w", newline="")
-
-    def read(self, name, binary=False):
-        full = os.path.join(self.base, name)
-
-        if binary:
-            return open(full, mode="rb")
-        else:
-            return open(full, mode="r", newline="")
-
-    def delete(self, name) -> bool:
-        full = os.path.join(self.base, name)
-        if os.path.isfile(full):
-            os.unlink(full)
-            return True
-        return False
-
-    def isdocument(self, name):
-        return os.path.isfile(os.path.join(self._root, name))
-
-    def isfolder(self, name):
-        return os.path.isdir(os.path.join(self._root, name))
-
-    def substorage(self, name):
-        return LocalStorage(os.path.join(self.base, name), self._config)
-
-    def copy(self, localfile, destination):
-        import shutil
-        if os.path.isabs(destination):
-            raise IOError("Only relative paths allowed")
-
-        full = os.path.join(self.base, destination)
-        os.makedirs(os.path.dirname(full), exist_ok=True)
-
-        shutil.move(localfile, os.path.join(self.base, full))
-
-    def directory(self, *args):
-        segments = []
-        for arg in args:
-            if arg is None:
-                continue
-            if isinstance(arg, str):
-                segments.append(arg)
-            elif isinstance(arg, (int, float)):
-                segments.append(str(arg))
-            else:
-                segments.append(class_fullname(arg))
-
-        path = os.path.join(self._root, *segments)
-        os.makedirs(path, exist_ok=True)
-
-        return path
-
-class Cache(cachetools.Cache):
-    """Persistent cache, extends the cache from cachetools package by storing cached objects (using picke serialization) to
-    the underlying storage. 
-    """
+                    if callback:
+                        callback(float(i-1) / self.repetitions + (float(frame) / (self.repetitions * len(sequence))))
 
-    def __init__(self, storage: Storage):
-        """Creates a new cache backed by the given storage.
+                for o, trajectory in trajectories.items():
+                    trajectory.write(results, result_name(sequence, o, i))
+
+
+@experiment_registry.register("supervised")
+class SupervisedExperiment(MultiRunExperiment):
+    """Supervised experiment. This experiment is used to run a tracker multiple times on the same sequence with supervision (reinitialization in case of failure)."""
+
+    FAILURE = 2
+
+    skip_initialize = Integer(val_min=1, default=1)
+    skip_tags = List(String(), default=[])
+    failure_overlap = Float(val_min=0, val_max=1, default=0)
+
+    def execute(self, tracker: Tracker, sequence: Sequence, force: bool = False, callback: Callable = None):
+        """Execute the experiment for the given tracker and sequence.
 
         Args:
-            storage (Storage): The storage used to save objects.
+            tracker (Tracker): The tracker to be used.
+            sequence (Sequence): The sequence to be used.
+            force (bool, optional): Whether to force the execution. Defaults to False.
+            callback (Callable, optional): The callback to be used. Defaults to None.
         """
-        super().__init__(10000)
-        self._storage = storage
 
-    def _filename(self, key: typing.Union[typing.Tuple, str]) -> str:
-        """Generates a filename for the given object key.
+        results = self.results(tracker, sequence)
 
-        Args:
-            key (typing.Union[typing.Tuple, str]): Cache key, either tuple or a single string
+        with self._get_runtime(tracker, sequence) as runtime:
 
-        Returns:
-            str: Relative path as a string
-        """
-        if isinstance(key, tuple):
-            filename = key[-1]
-            if len(key) > 1:
-                directory = self._storage.directory(*key[:-1])
-            else:
-                directory = ""
-        else:
-            filename = str(key)
-            directory = ""
-        return os.path.join(directory, filename)
+            for i in range(1, self.repetitions+1):
+                name = "%s_%03d" % (sequence.name, i)
 
-    def __getitem__(self, key: str) -> typing.Any:
-        """Retrieves an image from cache. If it does not exist, a KeyError is raised
+                if Trajectory.exists(results, name) and not force:
+                    continue
 
-        Args:
-            key (str): Key of the item
+                if self._can_stop(tracker, sequence):
+                    return
 
-        Raises:
-            KeyError: Entry does not exist or cannot be retrieved
-            PickleError: Unable to 
+                trajectory = Trajectory(len(sequence))
 
-        Returns:
-            typing.Any: item value
-        """
-        try:
-            return super().__getitem__(key)
-        except KeyError as e:
-            filename = self._filename(key)
-            if not self._storage.isdocument(filename):
-                raise e
-            try:
-                with self._storage.read(filename, binary=True) as filehandle:
-                    data = pickle.load(filehandle)
-                    super().__setitem__(key, data)
-                    return data
-            except pickle.PickleError as e:
-                raise KeyError(e)
+                frame = 0
+                while frame < len(sequence):
 
-    def __setitem__(self, key: str, value: typing.Any) -> None:
-        """Sets an item for given key
+                    _, elapsed = runtime.initialize(sequence.frame(frame), self._get_initialization(sequence, frame))
 
-        Args:
-            key (str): Item key
-            value (typing.Any): Item value
+                    trajectory.set(frame, Special(Trajectory.INITIALIZATION), {"time" : elapsed})
 
-        """
-        super().__setitem__(key, value)
+                    frame = frame + 1
 
-        filename = self._filename(key)
-        try:
-            with self._storage.write(filename, binary=True) as filehandle:
-                pickle.dump(value, filehandle)
-        except pickle.PickleError:
-            pass
+                    while frame < len(sequence):
 
-    def __delitem__(self, key: str) -> None:
-        """Operator for item deletion.
+                        object, elapsed = runtime.update(sequence.frame(frame))
 
-        Args:
-            key (str): Key of object to remove
-        """
-        try:
-            super().__delitem__(key)
-            filename = self._filename(key)
-            try:
-                self._storage.delete(filename)
-            except IOError:
-                pass
-        except KeyError:
-            pass
+                        object.properties["time"] = elapsed
 
-    def __contains__(self, key: str) -> bool:
-        """Magic method, does the cache include an item for a given key.
+                        if calculate_overlap(object.region, sequence.groundtruth(frame), sequence.size) <= self.failure_overlap:
+                            trajectory.set(frame, Special(SupervisedExperiment.FAILURE), object.properties)
+                            frame = frame + self.skip_initialize
+ 
+                            if self.skip_tags:
+                                while frame < len(sequence):
+                                    if not [t for t in sequence.tags(frame) if t in self.skip_tags]:
+                                        break
+                                    frame = frame + 1
+                            break
+                        else:
+                            trajectory.set(frame, object.region, object.properties)
+                        frame = frame + 1
 
-        Args:
-            key (str): Item key
+                if  callback:
+                    callback(i / self.repetitions)
 
-        Returns:
-            bool: True if object exists for a given key
-        """
-        filename = self._filename(key)
-        return self._storage.isdocument(filename)
+                trajectory.write(results, name)
```

### Comparing `vot-toolkit-0.6.2/vot/workspace/tests.py` & `vot-toolkit-0.6.4/vot/workspace/tests.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+"""Tests for workspace related methods and classes."""
 
 import logging
 import tempfile
 import unittest
 from vot import get_logger
 from vot.workspace.storage import Cache, LocalStorage
```

### Comparing `vot-toolkit-0.6.2/vot_toolkit.egg-info/PKG-INFO` & `vot-toolkit-0.6.4/vot_toolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: vot-toolkit
-Version: 0.6.2
+Version: 0.6.4
 Summary: Perform visual object tracking experiments and analyze results
 Home-page: https://github.com/votchallenge/toolkit
 Author: Luka Cehovin Zajc
 Author-email: luka.cehovin@gmail.com
 License: UNKNOWN
 Description: 
         The VOT evaluation toolkit
         ==========================
         
+        [![PyPI package version](https://badge.fury.io/py/vot-toolkit.svg)](https://badge.fury.io/py/vot-toolkit)
+        
         This repository contains the official evaluation toolkit for the [Visual Object Tracking (VOT) challenge](http://votchallenge.net/). This is the official version of the toolkit, implemented in Python 3 language. If you are looking for the old Matlab version, you can find an archived repository [here](https://github.com/votchallenge/toolkit-legacy).
         
         For more detailed informations consult the documentation available in the source or a compiled version of the documentation [here](http://www.votchallenge.net/howto/). You can also subscribe to the VOT [mailing list](https://liste.arnes.si/mailman3/lists/votchallenge.lists.arnes.si/) to receive news about challenges and important software updates or join our [support form](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help) to ask questions.
         
         Developers
         ----------
```

### Comparing `vot-toolkit-0.6.2/vot_toolkit.egg-info/SOURCES.txt` & `vot-toolkit-0.6.4/vot_toolkit.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 README.md
 requirements.txt
 setup.py
 vot/__init__.py
 vot/__main__.py
 vot/version.py
 vot/analysis/__init__.py
-vot/analysis/_processor.py
 vot/analysis/accuracy.py
 vot/analysis/failures.py
 vot/analysis/longterm.py
 vot/analysis/multistart.py
+vot/analysis/processor.py
 vot/analysis/supervised.py
 vot/dataset/__init__.py
+vot/dataset/common.py
 vot/dataset/cow.png
 vot/dataset/dummy.py
 vot/dataset/got10k.py
 vot/dataset/otb.py
 vot/dataset/proxy.py
 vot/dataset/trackingnet.py
-vot/dataset/vot.py
 vot/document/__init__.py
 vot/document/commands.tex
 vot/document/common.py
 vot/document/html.py
 vot/document/jquery.js
 vot/document/latex.py
 vot/document/pure.css
```

