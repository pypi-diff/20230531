# Comparing `tmp/wellmet-0.9.6.tar.gz` & `tmp/wellmet-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wellmet-0.9.6.tar", last modified: Tue May 30 18:18:59 2023, max compression
+gzip compressed data, was "wellmet-0.9.7.tar", last modified: Tue May 30 18:24:44 2023, max compression
```

## Comparing `wellmet-0.9.6.tar` & `wellmet-0.9.7.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:18:59.725614 wellmet-0.9.6/
--rw-r--r--   0 user         (0) root         (0)     1093 2022-04-30 17:02:31.015990 wellmet-0.9.6/LICENSE
--rw-r--r--   0 user         (0) root         (0)     5845 2023-05-30 18:18:59.726401 wellmet-0.9.6/PKG-INFO
--rw-r--r--   0 user         (0) root         (0)     5175 2023-05-30 18:17:45.015990 wellmet-0.9.6/README.md
--rw-r--r--   0 user         (0) root         (0)       81 2023-05-30 15:14:52.016253 wellmet-0.9.6/pyproject.toml
--rw-r--r--   0 user         (0) root         (0)      784 2023-05-30 18:18:59.746586 wellmet-0.9.6/setup.cfg
--rw-r--r--   0 user         (0) root         (0)       54 2023-05-29 15:46:17.016253 wellmet-0.9.6/setup.py
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:18:59.274989 wellmet-0.9.6/wellmet/
--rw-r--r--   0 user         (0) root         (0)    30048 2023-05-28 14:15:30.016515 wellmet-0.9.6/wellmet/IS_stat.py
--rw-r--r--   0 user         (0) root         (0)       86 2023-05-28 15:34:51.016515 wellmet-0.9.6/wellmet/__init__.py
--rw-r--r--   0 user         (0) root         (0)       72 2022-04-30 16:53:41.016515 wellmet-0.9.6/wellmet/__main__.py
--rw-r--r--   0 user         (0) root         (0)    11243 2023-05-28 14:15:30.016515 wellmet-0.9.6/wellmet/candybox.py
--rw-r--r--   0 user         (0) root         (0)     6756 2023-05-28 14:15:30.016777 wellmet-0.9.6/wellmet/candynodes.py
--rw-r--r--   0 user         (0) root         (0)    50875 2023-05-29 17:12:11.016777 wellmet-0.9.6/wellmet/convex_hull.py
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:18:59.382730 wellmet-0.9.6/wellmet/dicebox/
--rw-r--r--   0 user         (0) root         (0)        6 2022-04-30 16:53:41.018612 wellmet-0.9.6/wellmet/dicebox/__init__.py
--rw-r--r--   0 user         (0) root         (0)     7865 2023-05-29 17:12:04.018874 wellmet-0.9.6/wellmet/dicebox/_exploration.py
--rw-r--r--   0 user         (0) root         (0)    14880 2023-05-30 15:54:19.018874 wellmet-0.9.6/wellmet/dicebox/circumtri.py
--rw-r--r--   0 user         (0) root         (0)    36893 2023-01-15 11:50:38.016777 wellmet-0.9.6/wellmet/estimation.py
--rw-r--r--   0 user         (0) root         (0)    52580 2023-01-15 11:51:29.017039 wellmet-0.9.6/wellmet/f_models.py
--rw-r--r--   0 user         (0) root         (0)    42237 2023-03-12 14:45:57.017039 wellmet-0.9.6/wellmet/g_models.py
--rw-r--r--   0 user         (0) root         (0)    21042 2023-05-28 14:15:30.017039 wellmet-0.9.6/wellmet/ghull.py
--rw-r--r--   0 user         (0) root         (0)     3234 2022-05-13 19:15:46.017301 wellmet-0.9.6/wellmet/misc.py
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:18:59.513802 wellmet-0.9.6/wellmet/mplot/
--rw-r--r--   0 user         (0) root         (0)     1407 2022-04-30 16:53:41.018874 wellmet-0.9.6/wellmet/mplot/__init__.py
--rw-r--r--   0 user         (0) root         (0)     9741 2022-04-30 16:53:41.019136 wellmet-0.9.6/wellmet/mplot/_axes3d.py
--rw-r--r--   0 user         (0) root         (0)      714 2022-04-30 16:53:41.019136 wellmet-0.9.6/wellmet/mplot/_axis3d_margins_patch.py
--rw-r--r--   0 user         (0) root         (0)    23492 2023-03-30 13:18:09.019136 wellmet-0.9.6/wellmet/mplot/mart.py
--rw-r--r--   0 user         (0) root         (0)    13647 2023-01-15 11:54:22.019398 wellmet-0.9.6/wellmet/mplot/mart3d.py
--rw-r--r--   0 user         (0) root         (0)    26324 2023-05-29 17:11:54.019398 wellmet-0.9.6/wellmet/mplot/maxes.py
--rw-r--r--   0 user         (0) root         (0)     5577 2022-04-30 16:53:41.019398 wellmet-0.9.6/wellmet/mplot/maxes3d.py
--rw-r--r--   0 user         (0) root         (0)    17778 2023-05-29 17:11:54.019660 wellmet-0.9.6/wellmet/mplot/mfigs.py
--rw-r--r--   0 user         (0) root         (0)    10463 2023-02-02 13:58:18.019660 wellmet-0.9.6/wellmet/mplot/mgraph.py
--rw-r--r--   0 user         (0) root         (0)     1132 2022-04-30 16:53:41.019660 wellmet-0.9.6/wellmet/mplot/misc.py
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:18:59.644087 wellmet-0.9.6/wellmet/qt_gui/
--rw-r--r--   0 user         (0) root         (0)        6 2022-04-30 16:53:41.019660 wellmet-0.9.6/wellmet/qt_gui/__init__.py
--rw-r--r--   0 user         (0) root         (0)    44438 2023-01-15 11:54:47.019923 wellmet-0.9.6/wellmet/qt_gui/gl_plot.py
--rw-r--r--   0 user         (0) root         (0)      348 2022-10-16 03:13:28.019923 wellmet-0.9.6/wellmet/qt_gui/gui_startup.py
--rw-r--r--   0 user         (0) root         (0)     1970 2022-10-07 12:30:43.019923 wellmet-0.9.6/wellmet/qt_gui/qt_box_functions.py
--rw-r--r--   0 user         (0) root         (0)    26222 2023-05-30 16:44:01.020185 wellmet-0.9.6/wellmet/qt_gui/qt_dicebox.py
--rw-r--r--   0 user         (0) root         (0)    35342 2023-01-17 14:19:12.020185 wellmet-0.9.6/wellmet/qt_gui/qt_graph_widgets.py
--rw-r--r--   0 user         (0) root         (0)    24721 2023-05-30 16:56:29.020185 wellmet-0.9.6/wellmet/qt_gui/qt_gui.py
--rw-r--r--   0 user         (0) root         (0)    99810 2023-05-29 17:13:09.020447 wellmet-0.9.6/wellmet/qt_gui/qt_plot.py
--rw-r--r--   0 user         (0) root         (0)     3244 2023-01-10 05:21:15.020447 wellmet-0.9.6/wellmet/qt_gui/qt_testcases.py
--rw-r--r--   0 user         (0) root         (0)    56858 2022-11-29 15:50:00.020447 wellmet-0.9.6/wellmet/qt_gui/qt_voronoi.py
--rw-r--r--   0 user         (0) root         (0)    10978 2023-05-30 15:55:36.017301 wellmet-0.9.6/wellmet/reader.py
--rw-r--r--   0 user         (0) root         (0)     4416 2023-01-15 11:56:01.017301 wellmet-0.9.6/wellmet/samplebox.py
--rw-r--r--   0 user         (0) root         (0)     6558 2022-04-30 16:53:42.017563 wellmet-0.9.6/wellmet/sball.py
--rw-r--r--   0 user         (0) root         (0)     6739 2023-05-29 17:11:42.017563 wellmet-0.9.6/wellmet/schemes.py
--rw-r--r--   0 user         (0) root         (0)     8309 2023-05-28 14:15:30.017563 wellmet-0.9.6/wellmet/shell.py
--rw-r--r--   0 user         (0) root         (0)   134283 2023-05-29 17:11:31.017825 wellmet-0.9.6/wellmet/simplex.py
--rw-r--r--   0 user         (0) root         (0)    13090 2023-05-28 14:15:30.017825 wellmet-0.9.6/wellmet/spring.py
--rw-r--r--   0 user         (0) root         (0)    10953 2022-04-30 16:53:42.017825 wellmet-0.9.6/wellmet/stm_df.py
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:18:59.712507 wellmet-0.9.6/wellmet/testcases/
--rw-r--r--   0 user         (0) root         (0)        0 2023-05-28 13:48:40.020709 wellmet-0.9.6/wellmet/testcases/__init__.py
--rw-r--r--   0 user         (0) root         (0)     8987 2023-03-12 15:00:08.020709 wellmet-0.9.6/wellmet/testcases/gaussian_2D.py
--rw-r--r--   0 user         (0) root         (0)     8183 2023-05-28 14:14:11.020709 wellmet-0.9.6/wellmet/testcases/testcases_2D.py
--rw-r--r--   0 user         (0) root         (0)     3741 2023-02-24 08:01:44.020971 wellmet-0.9.6/wellmet/testcases/testcases_2D_papers.py
--rw-r--r--   0 user         (0) root         (0)     2572 2023-01-14 08:20:10.020971 wellmet-0.9.6/wellmet/testcases/testcases_nD.py
--rw-r--r--   0 user         (0) root         (0)    11998 2023-01-30 12:29:31.020971 wellmet-0.9.6/wellmet/testcases/testcases_nD_papers.py
--rw-r--r--   0 user         (0) root         (0)    47956 2023-01-15 11:58:08.018087 wellmet-0.9.6/wellmet/voronoi.py
--rw-r--r--   0 user         (0) root         (0)     2465 2023-05-28 14:15:30.018087 wellmet-0.9.6/wellmet/welford.py
--rw-r--r--   0 user         (0) root         (0)    32101 2023-03-15 04:11:34.018087 wellmet-0.9.6/wellmet/whitebox.py
--rw-r--r--   0 user         (0) root         (0)    26468 2023-05-28 14:15:30.018350 wellmet-0.9.6/wellmet/wireframe.py
-drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:18:59.346292 wellmet-0.9.6/wellmet.egg-info/
--rw-r--r--   0 user         (0) root         (0)     5845 2023-05-30 18:18:58.018350 wellmet-0.9.6/wellmet.egg-info/PKG-INFO
--rw-r--r--   0 user         (0) root         (0)     1498 2023-05-30 18:18:58.018350 wellmet-0.9.6/wellmet.egg-info/SOURCES.txt
--rw-r--r--   0 user         (0) root         (0)        1 2023-05-30 18:18:58.018350 wellmet-0.9.6/wellmet.egg-info/dependency_links.txt
--rw-r--r--   0 user         (0) root         (0)       61 2023-05-30 18:18:58.018612 wellmet-0.9.6/wellmet.egg-info/requires.txt
--rw-r--r--   0 user         (0) root         (0)        8 2023-05-30 18:18:58.018612 wellmet-0.9.6/wellmet.egg-info/top_level.txt
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:24:44.571998 wellmet-0.9.7/
+-rw-r--r--   0 user         (0) root         (0)     1093 2022-04-30 17:02:31.062128 wellmet-0.9.7/LICENSE
+-rw-r--r--   0 user         (0) root         (0)     5835 2023-05-30 18:24:44.572784 wellmet-0.9.7/PKG-INFO
+-rw-r--r--   0 user         (0) root         (0)     5165 2023-05-30 18:24:25.062128 wellmet-0.9.7/README.md
+-rw-r--r--   0 user         (0) root         (0)       81 2023-05-30 15:14:52.062128 wellmet-0.9.7/pyproject.toml
+-rw-r--r--   0 user         (0) root         (0)      784 2023-05-30 18:24:44.598474 wellmet-0.9.7/setup.cfg
+-rw-r--r--   0 user         (0) root         (0)       54 2023-05-29 15:46:17.062390 wellmet-0.9.7/setup.py
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:24:43.914358 wellmet-0.9.7/wellmet/
+-rw-r--r--   0 user         (0) root         (0)    30048 2023-05-28 14:15:30.062390 wellmet-0.9.7/wellmet/IS_stat.py
+-rw-r--r--   0 user         (0) root         (0)       86 2023-05-28 15:34:51.062652 wellmet-0.9.7/wellmet/__init__.py
+-rw-r--r--   0 user         (0) root         (0)       72 2022-04-30 16:53:41.062652 wellmet-0.9.7/wellmet/__main__.py
+-rw-r--r--   0 user         (0) root         (0)    11243 2023-05-28 14:15:30.062652 wellmet-0.9.7/wellmet/candybox.py
+-rw-r--r--   0 user         (0) root         (0)     6756 2023-05-28 14:15:30.062914 wellmet-0.9.7/wellmet/candynodes.py
+-rw-r--r--   0 user         (0) root         (0)    50875 2023-05-29 17:12:11.062914 wellmet-0.9.7/wellmet/convex_hull.py
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:24:44.061866 wellmet-0.9.7/wellmet/dicebox/
+-rw-r--r--   0 user         (0) root         (0)        6 2022-04-30 16:53:41.064749 wellmet-0.9.7/wellmet/dicebox/__init__.py
+-rw-r--r--   0 user         (0) root         (0)     7865 2023-05-29 17:12:04.065011 wellmet-0.9.7/wellmet/dicebox/_exploration.py
+-rw-r--r--   0 user         (0) root         (0)    14880 2023-05-30 15:54:19.065011 wellmet-0.9.7/wellmet/dicebox/circumtri.py
+-rw-r--r--   0 user         (0) root         (0)    36893 2023-01-15 11:50:38.062914 wellmet-0.9.7/wellmet/estimation.py
+-rw-r--r--   0 user         (0) root         (0)    52580 2023-01-15 11:51:29.063176 wellmet-0.9.7/wellmet/f_models.py
+-rw-r--r--   0 user         (0) root         (0)    42237 2023-03-12 14:45:57.063176 wellmet-0.9.7/wellmet/g_models.py
+-rw-r--r--   0 user         (0) root         (0)    21042 2023-05-28 14:15:30.063176 wellmet-0.9.7/wellmet/ghull.py
+-rw-r--r--   0 user         (0) root         (0)     3234 2022-05-13 19:15:46.063176 wellmet-0.9.7/wellmet/misc.py
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:24:44.243007 wellmet-0.9.7/wellmet/mplot/
+-rw-r--r--   0 user         (0) root         (0)     1407 2022-04-30 16:53:41.065011 wellmet-0.9.7/wellmet/mplot/__init__.py
+-rw-r--r--   0 user         (0) root         (0)     9741 2022-04-30 16:53:41.065011 wellmet-0.9.7/wellmet/mplot/_axes3d.py
+-rw-r--r--   0 user         (0) root         (0)      714 2022-04-30 16:53:41.065273 wellmet-0.9.7/wellmet/mplot/_axis3d_margins_patch.py
+-rw-r--r--   0 user         (0) root         (0)    23492 2023-03-30 13:18:09.065273 wellmet-0.9.7/wellmet/mplot/mart.py
+-rw-r--r--   0 user         (0) root         (0)    13647 2023-01-15 11:54:22.065273 wellmet-0.9.7/wellmet/mplot/mart3d.py
+-rw-r--r--   0 user         (0) root         (0)    26324 2023-05-29 17:11:54.065536 wellmet-0.9.7/wellmet/mplot/maxes.py
+-rw-r--r--   0 user         (0) root         (0)     5577 2022-04-30 16:53:41.065536 wellmet-0.9.7/wellmet/mplot/maxes3d.py
+-rw-r--r--   0 user         (0) root         (0)    17778 2023-05-29 17:11:54.065536 wellmet-0.9.7/wellmet/mplot/mfigs.py
+-rw-r--r--   0 user         (0) root         (0)    10463 2023-02-02 13:58:18.065798 wellmet-0.9.7/wellmet/mplot/mgraph.py
+-rw-r--r--   0 user         (0) root         (0)     1132 2022-04-30 16:53:41.065798 wellmet-0.9.7/wellmet/mplot/misc.py
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:24:44.430440 wellmet-0.9.7/wellmet/qt_gui/
+-rw-r--r--   0 user         (0) root         (0)        6 2022-04-30 16:53:41.065798 wellmet-0.9.7/wellmet/qt_gui/__init__.py
+-rw-r--r--   0 user         (0) root         (0)    44438 2023-01-15 11:54:47.066060 wellmet-0.9.7/wellmet/qt_gui/gl_plot.py
+-rw-r--r--   0 user         (0) root         (0)      348 2022-10-16 03:13:28.066060 wellmet-0.9.7/wellmet/qt_gui/gui_startup.py
+-rw-r--r--   0 user         (0) root         (0)     1970 2022-10-07 12:30:43.066060 wellmet-0.9.7/wellmet/qt_gui/qt_box_functions.py
+-rw-r--r--   0 user         (0) root         (0)    26222 2023-05-30 16:44:01.066322 wellmet-0.9.7/wellmet/qt_gui/qt_dicebox.py
+-rw-r--r--   0 user         (0) root         (0)    35342 2023-01-17 14:19:12.066322 wellmet-0.9.7/wellmet/qt_gui/qt_graph_widgets.py
+-rw-r--r--   0 user         (0) root         (0)    24722 2023-05-30 18:23:10.066322 wellmet-0.9.7/wellmet/qt_gui/qt_gui.py
+-rw-r--r--   0 user         (0) root         (0)    99810 2023-05-29 17:13:09.066584 wellmet-0.9.7/wellmet/qt_gui/qt_plot.py
+-rw-r--r--   0 user         (0) root         (0)     3244 2023-01-10 05:21:15.066584 wellmet-0.9.7/wellmet/qt_gui/qt_testcases.py
+-rw-r--r--   0 user         (0) root         (0)    56858 2022-11-29 15:50:00.066584 wellmet-0.9.7/wellmet/qt_gui/qt_voronoi.py
+-rw-r--r--   0 user         (0) root         (0)    10978 2023-05-30 15:55:36.063439 wellmet-0.9.7/wellmet/reader.py
+-rw-r--r--   0 user         (0) root         (0)     4416 2023-01-15 11:56:01.063439 wellmet-0.9.7/wellmet/samplebox.py
+-rw-r--r--   0 user         (0) root         (0)     6558 2022-04-30 16:53:42.063439 wellmet-0.9.7/wellmet/sball.py
+-rw-r--r--   0 user         (0) root         (0)     6739 2023-05-29 17:11:42.063701 wellmet-0.9.7/wellmet/schemes.py
+-rw-r--r--   0 user         (0) root         (0)     8309 2023-05-28 14:15:30.063701 wellmet-0.9.7/wellmet/shell.py
+-rw-r--r--   0 user         (0) root         (0)   134283 2023-05-29 17:11:31.063701 wellmet-0.9.7/wellmet/simplex.py
+-rw-r--r--   0 user         (0) root         (0)    13090 2023-05-28 14:15:30.063963 wellmet-0.9.7/wellmet/spring.py
+-rw-r--r--   0 user         (0) root         (0)    10953 2022-04-30 16:53:42.063963 wellmet-0.9.7/wellmet/stm_df.py
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:24:44.547881 wellmet-0.9.7/wellmet/testcases/
+-rw-r--r--   0 user         (0) root         (0)        0 2023-05-28 13:48:40.066584 wellmet-0.9.7/wellmet/testcases/__init__.py
+-rw-r--r--   0 user         (0) root         (0)     8987 2023-03-12 15:00:08.066846 wellmet-0.9.7/wellmet/testcases/gaussian_2D.py
+-rw-r--r--   0 user         (0) root         (0)     8183 2023-05-28 14:14:11.066846 wellmet-0.9.7/wellmet/testcases/testcases_2D.py
+-rw-r--r--   0 user         (0) root         (0)     3741 2023-02-24 08:01:44.066846 wellmet-0.9.7/wellmet/testcases/testcases_2D_papers.py
+-rw-r--r--   0 user         (0) root         (0)     2572 2023-01-14 08:20:10.000000 wellmet-0.9.7/wellmet/testcases/testcases_nD.py
+-rw-r--r--   0 user         (0) root         (0)    11998 2023-01-30 12:29:31.000000 wellmet-0.9.7/wellmet/testcases/testcases_nD_papers.py
+-rw-r--r--   0 user         (0) root         (0)    47956 2023-01-15 11:58:08.063963 wellmet-0.9.7/wellmet/voronoi.py
+-rw-r--r--   0 user         (0) root         (0)     2465 2023-05-28 14:15:30.064225 wellmet-0.9.7/wellmet/welford.py
+-rw-r--r--   0 user         (0) root         (0)    32101 2023-03-15 04:11:34.064225 wellmet-0.9.7/wellmet/whitebox.py
+-rw-r--r--   0 user         (0) root         (0)    26468 2023-05-28 14:15:30.064225 wellmet-0.9.7/wellmet/wireframe.py
+drwxr-xr-x   0 user         (0) root         (0)        0 2023-05-30 18:24:44.006029 wellmet-0.9.7/wellmet.egg-info/
+-rw-r--r--   0 user         (0) root         (0)     5835 2023-05-30 18:24:43.064487 wellmet-0.9.7/wellmet.egg-info/PKG-INFO
+-rw-r--r--   0 user         (0) root         (0)     1498 2023-05-30 18:24:43.064487 wellmet-0.9.7/wellmet.egg-info/SOURCES.txt
+-rw-r--r--   0 user         (0) root         (0)        1 2023-05-30 18:24:43.064487 wellmet-0.9.7/wellmet.egg-info/dependency_links.txt
+-rw-r--r--   0 user         (0) root         (0)       61 2023-05-30 18:24:43.064749 wellmet-0.9.7/wellmet.egg-info/requires.txt
+-rw-r--r--   0 user         (0) root         (0)        8 2023-05-30 18:24:43.064749 wellmet-0.9.7/wellmet.egg-info/top_level.txt
```

### Comparing `wellmet-0.9.6/LICENSE` & `wellmet-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/PKG-INFO` & `wellmet-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wellmet
-Version: 0.9.6
+Version: 0.9.7
 Summary: a pure Python framework for spatial structural reliability analysis
 Home-page: https://rocketgit.com/iam-git/WellMet
 Author: Gerasimov Aleksei
 Author-email: ger-alex@seznam.cz
 License: MIT
 Keywords: failure probability,Monte Carlo,surrogate model,response surface
 Platform: UNKNOWN
@@ -46,15 +46,15 @@
 ```
 pip install wellmet
 ```
 
 WellMet relies on ```quadpy``` for simplex integration. However, quadpy became a closed source software and requires licence fee now.
 One probably could install official quadpy package and obtain a licence in order to support Nico Schloemer.
 However, WellMet has never been tested with commertial quadpy versions.
-So, we separately share the last GPL version of quadpy:
+So, we separately share the last GPL version:
 ```
 pip install quadpy-gpl
 ```
 
 
 # How to use:
 ## A. To run GUI with predefined benchmark problems:
```

### Comparing `wellmet-0.9.6/README.md` & `wellmet-0.9.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ```
 pip install wellmet
 ```
 
 WellMet relies on ```quadpy``` for simplex integration. However, quadpy became a closed source software and requires licence fee now.
 One probably could install official quadpy package and obtain a licence in order to support Nico Schloemer.
 However, WellMet has never been tested with commertial quadpy versions.
-So, we separately share the last GPL version of quadpy:
+So, we separately share the last GPL version:
 ```
 pip install quadpy-gpl
 ```
 
 
 # How to use:
 ## A. To run GUI with predefined benchmark problems:
```

### Comparing `wellmet-0.9.6/setup.cfg` & `wellmet-0.9.7/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wellmet
-version = 0.9.6
+version = 0.9.7
 author = Gerasimov Aleksei
 author_email = ger-alex@seznam.cz
 description = a pure Python framework for spatial structural reliability analysis
 url = https://rocketgit.com/iam-git/WellMet
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
```

### Comparing `wellmet-0.9.6/wellmet/IS_stat.py` & `wellmet-0.9.7/wellmet/IS_stat.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/candybox.py` & `wellmet-0.9.7/wellmet/candybox.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/candynodes.py` & `wellmet-0.9.7/wellmet/candynodes.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/convex_hull.py` & `wellmet-0.9.7/wellmet/convex_hull.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/dicebox/_exploration.py` & `wellmet-0.9.7/wellmet/dicebox/_exploration.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/dicebox/circumtri.py` & `wellmet-0.9.7/wellmet/dicebox/circumtri.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/estimation.py` & `wellmet-0.9.7/wellmet/estimation.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/f_models.py` & `wellmet-0.9.7/wellmet/f_models.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/g_models.py` & `wellmet-0.9.7/wellmet/g_models.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/ghull.py` & `wellmet-0.9.7/wellmet/ghull.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/misc.py` & `wellmet-0.9.7/wellmet/misc.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/mplot/__init__.py` & `wellmet-0.9.7/wellmet/mplot/__init__.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/mplot/_axes3d.py` & `wellmet-0.9.7/wellmet/mplot/_axes3d.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/mplot/_axis3d_margins_patch.py` & `wellmet-0.9.7/wellmet/mplot/_axis3d_margins_patch.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/mplot/mart.py` & `wellmet-0.9.7/wellmet/mplot/mart.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/mplot/mart3d.py` & `wellmet-0.9.7/wellmet/mplot/mart3d.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/mplot/maxes.py` & `wellmet-0.9.7/wellmet/mplot/maxes.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/mplot/maxes3d.py` & `wellmet-0.9.7/wellmet/mplot/maxes3d.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/mplot/mfigs.py` & `wellmet-0.9.7/wellmet/mplot/mfigs.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/mplot/mgraph.py` & `wellmet-0.9.7/wellmet/mplot/mgraph.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/mplot/misc.py` & `wellmet-0.9.7/wellmet/mplot/misc.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/qt_gui/gl_plot.py` & `wellmet-0.9.7/wellmet/qt_gui/gl_plot.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/qt_gui/qt_box_functions.py` & `wellmet-0.9.7/wellmet/qt_gui/qt_box_functions.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/qt_gui/qt_dicebox.py` & `wellmet-0.9.7/wellmet/qt_gui/qt_dicebox.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/qt_gui/qt_graph_widgets.py` & `wellmet-0.9.7/wellmet/qt_gui/qt_graph_widgets.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/qt_gui/qt_gui.py` & `wellmet-0.9.7/wellmet/qt_gui/qt_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pyqtgraph.Qt import QtGui, QtWidgets
 from pyqtgraph.Qt import QtCore
 
 from pyqtgraph import console
 
 import numpy as np
 from . import qt_graph_widgets as gw
-from . import qt_pairwise
+#from . import qt_pairwise
 from .. import reader
 
 
 ### Define a top-level widget to hold everything
 class QtGuiWindow(QtWidgets.QMainWindow):
     #č box_runned dublikuje slice_changed
     # do not redraw twice!
```

### Comparing `wellmet-0.9.6/wellmet/qt_gui/qt_plot.py` & `wellmet-0.9.7/wellmet/qt_gui/qt_plot.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/qt_gui/qt_testcases.py` & `wellmet-0.9.7/wellmet/qt_gui/qt_testcases.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/qt_gui/qt_voronoi.py` & `wellmet-0.9.7/wellmet/qt_gui/qt_voronoi.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/reader.py` & `wellmet-0.9.7/wellmet/reader.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/samplebox.py` & `wellmet-0.9.7/wellmet/samplebox.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/sball.py` & `wellmet-0.9.7/wellmet/sball.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/schemes.py` & `wellmet-0.9.7/wellmet/schemes.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/shell.py` & `wellmet-0.9.7/wellmet/shell.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/simplex.py` & `wellmet-0.9.7/wellmet/simplex.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/spring.py` & `wellmet-0.9.7/wellmet/spring.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/stm_df.py` & `wellmet-0.9.7/wellmet/stm_df.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/testcases/gaussian_2D.py` & `wellmet-0.9.7/wellmet/testcases/gaussian_2D.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/testcases/testcases_2D.py` & `wellmet-0.9.7/wellmet/testcases/testcases_2D.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/testcases/testcases_2D_papers.py` & `wellmet-0.9.7/wellmet/testcases/testcases_2D_papers.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/testcases/testcases_nD.py` & `wellmet-0.9.7/wellmet/testcases/testcases_nD.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/testcases/testcases_nD_papers.py` & `wellmet-0.9.7/wellmet/testcases/testcases_nD_papers.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/voronoi.py` & `wellmet-0.9.7/wellmet/voronoi.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/welford.py` & `wellmet-0.9.7/wellmet/welford.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/whitebox.py` & `wellmet-0.9.7/wellmet/whitebox.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet/wireframe.py` & `wellmet-0.9.7/wellmet/wireframe.py`

 * *Files identical despite different names*

### Comparing `wellmet-0.9.6/wellmet.egg-info/PKG-INFO` & `wellmet-0.9.7/wellmet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wellmet
-Version: 0.9.6
+Version: 0.9.7
 Summary: a pure Python framework for spatial structural reliability analysis
 Home-page: https://rocketgit.com/iam-git/WellMet
 Author: Gerasimov Aleksei
 Author-email: ger-alex@seznam.cz
 License: MIT
 Keywords: failure probability,Monte Carlo,surrogate model,response surface
 Platform: UNKNOWN
@@ -46,15 +46,15 @@
 ```
 pip install wellmet
 ```
 
 WellMet relies on ```quadpy``` for simplex integration. However, quadpy became a closed source software and requires licence fee now.
 One probably could install official quadpy package and obtain a licence in order to support Nico Schloemer.
 However, WellMet has never been tested with commertial quadpy versions.
-So, we separately share the last GPL version of quadpy:
+So, we separately share the last GPL version:
 ```
 pip install quadpy-gpl
 ```
 
 
 # How to use:
 ## A. To run GUI with predefined benchmark problems:
```

### Comparing `wellmet-0.9.6/wellmet.egg-info/SOURCES.txt` & `wellmet-0.9.7/wellmet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

