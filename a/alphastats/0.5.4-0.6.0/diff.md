# Comparing `tmp/alphastats-0.5.4.tar.gz` & `tmp/alphastats-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphastats-0.5.4.tar", last modified: Mon May 15 09:35:58 2023, max compression
+gzip compressed data, was "alphastats-0.6.0.tar", last modified: Wed May 31 13:55:36 2023, max compression
```

## Comparing `alphastats-0.5.4.tar` & `alphastats-0.6.0.tar`

### file list

```diff
@@ -1,75 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:35:58.572090 alphastats-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-15 09:35:24.000000 alphastats-0.5.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-15 09:35:24.000000 alphastats-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-15 09:35:58.572090 alphastats-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-15 09:35:24.000000 alphastats-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:35:58.556090 alphastats-0.5.4/alphastats/
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/DataSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    19551 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/DataSet_Pathway.py
--rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/DataSet_Plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/DataSet_Preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/DataSet_Statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:35:58.556090 alphastats-0.5.4/alphastats/data/
--rw-r--r--   0 runner    (1001) docker     (123)    70534 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/data/contaminations.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:35:58.556090 alphastats-0.5.4/alphastats/gui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:35:58.556090 alphastats-0.5.4/alphastats/gui/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/AlphaPeptStats.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31042 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/alphapeptstats_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    30529 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/alphastats_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    20433 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/alphastats_logo_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:35:58.556090 alphastats-0.5.4/alphastats/gui/pages/
--rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/pages/02_Import Data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/pages/03_Data Overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/pages/03_Preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/pages/04_Analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/pages/06_Results.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:35:58.560090 alphastats-0.5.4/alphastats/gui/sample_data/
--rw-r--r--   0 runner    (1001) docker     (123)    26661 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/sample_data/metadata.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)  9509624 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/sample_data/proteinGroups.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:35:58.568090 alphastats-0.5.4/alphastats/gui/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/utils/analysis_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/utils/software_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/gui/utils/ui_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/load_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:35:58.568090 alphastats-0.5.4/alphastats/loader/
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/loader/AlphaPeptLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/loader/BaseLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/loader/DIANNLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/loader/FragPipeLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/loader/MaxQuantLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/loader/SpectronautLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/loader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:35:58.572090 alphastats-0.5.4/alphastats/multicova/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/multicova/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29756 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/multicova/multicova.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:35:58.572090 alphastats-0.5.4/alphastats/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/plots/ClusterMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/plots/DimensionalityReduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/plots/IntensityPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/plots/PlotUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/plots/SampleHistogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/plots/VolcanoPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:35:58.572090 alphastats-0.5.4/alphastats/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/statistics/Anova.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/statistics/DifferentialExpressionAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/statistics/MultiCovaAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/statistics/StatisticUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-15 09:35:24.000000 alphastats-0.5.4/alphastats/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:35:58.556090 alphastats-0.5.4/alphastats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-15 09:35:58.000000 alphastats-0.5.4/alphastats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-15 09:35:58.000000 alphastats-0.5.4/alphastats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:35:58.000000 alphastats-0.5.4/alphastats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-15 09:35:58.000000 alphastats-0.5.4/alphastats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-15 09:35:58.000000 alphastats-0.5.4/alphastats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 09:35:58.000000 alphastats-0.5.4/alphastats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 09:35:58.572090 alphastats-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-15 09:35:24.000000 alphastats-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.877228 alphastats-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-31 13:55:10.000000 alphastats-0.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-31 13:55:10.000000 alphastats-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-31 13:55:36.877228 alphastats-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-05-31 13:55:10.000000 alphastats-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.865228 alphastats-0.6.0/alphastats/
+-rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/DataSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19551 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/DataSet_Pathway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/DataSet_Plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/DataSet_Preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/DataSet_Statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.865228 alphastats-0.6.0/alphastats/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    70534 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/data/contaminations.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.865228 alphastats-0.6.0/alphastats/gui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.865228 alphastats-0.6.0/alphastats/gui/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/AlphaPeptStats.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31042 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/alphapeptstats_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30529 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/alphastats_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20433 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/alphastats_logo_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.865228 alphastats-0.6.0/alphastats/gui/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/pages/02_Import Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/pages/03_Data Overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/pages/03_Preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/pages/04_Analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/pages/06_Results.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.865228 alphastats-0.6.0/alphastats/gui/sample_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    26661 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/sample_data/metadata.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)  9509624 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/sample_data/proteinGroups.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.877228 alphastats-0.6.0/alphastats/gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/utils/analysis_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/utils/software_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/gui/utils/ui_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.877228 alphastats-0.6.0/alphastats/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/loader/AlphaPeptLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/loader/BaseLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/loader/DIANNLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/loader/FragPipeLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/loader/MaxQuantLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/loader/SpectronautLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/loader/mzTabLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.877228 alphastats-0.6.0/alphastats/multicova/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/multicova/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29756 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/multicova/multicova.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.877228 alphastats-0.6.0/alphastats/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/plots/ClusterMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/plots/DimensionalityReduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/plots/IntensityPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/plots/PlotUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/plots/SampleHistogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/plots/VolcanoPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.877228 alphastats-0.6.0/alphastats/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/statistics/Anova.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/statistics/DifferentialExpressionAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/statistics/MultiCovaAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/statistics/StatisticUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-31 13:55:10.000000 alphastats-0.6.0/alphastats/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.865228 alphastats-0.6.0/alphastats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-31 13:55:36.000000 alphastats-0.6.0/alphastats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-31 13:55:36.000000 alphastats-0.6.0/alphastats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:55:36.000000 alphastats-0.6.0/alphastats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-31 13:55:36.000000 alphastats-0.6.0/alphastats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-31 13:55:36.000000 alphastats-0.6.0/alphastats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 13:55:36.000000 alphastats-0.6.0/alphastats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:55:36.877228 alphastats-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-31 13:55:10.000000 alphastats-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:55:36.877228 alphastats-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    35022 2023-05-31 13:55:10.000000 alphastats-0.6.0/tests/test_DataSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-31 13:55:10.000000 alphastats-0.6.0/tests/test_DataSet_Pathway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-05-31 13:55:10.000000 alphastats-0.6.0/tests/test_loaders.py
```

### Comparing `alphastats-0.5.4/LICENSE.txt` & `alphastats-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/PKG-INFO` & `alphastats-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphastats
-Version: 0.5.4
+Version: 0.6.0
 Summary: An open-source Python package for Mass Spectrometry Analysis
 Home-page: https://github.com/MannLabs/alphastats
 Author: Mann Labs
 Author-email: elena.krismer@hotmail.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: GitHub, https://github.com/MannLabs/alphapeptstats
@@ -43,14 +43,27 @@
 </div>
 
 <br>
 <br>
 
 [link]:https://alphapeptstats.readthedocs.io/en/main/
 
+<div align = center>
+<br>
+<br>
+
+[<kbd> <br> Streamlit WebApp <br> </kbd>][link_streamlit]
+
+</div>
+
+<br>
+<br>
+
+[link_streamlit]:https://mannlabs-alphapeptstats-alphastatsguialphapeptstats-qyzgwd.streamlit.app/
+
 An open-source Python package for downstream mass spectrometry downstream data analysis from the [Mann Group at the University of Copenhagen](https://www.cpr.ku.dk/research/proteomics/mann/).
 
 
 * [**Citation**](#citation)
 * [**Installation**](#installation)
 * [**Troubleshooting**](#troubleshooting)
 * [**License**](#license)
```

### Comparing `alphastats-0.5.4/README.md` & `alphastats-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,27 @@
 </div>
 
 <br>
 <br>
 
 [link]:https://alphapeptstats.readthedocs.io/en/main/
 
+<div align = center>
+<br>
+<br>
+
+[<kbd> <br> Streamlit WebApp <br> </kbd>][link_streamlit]
+
+</div>
+
+<br>
+<br>
+
+[link_streamlit]:https://mannlabs-alphapeptstats-alphastatsguialphapeptstats-qyzgwd.streamlit.app/
+
 An open-source Python package for downstream mass spectrometry downstream data analysis from the [Mann Group at the University of Copenhagen](https://www.cpr.ku.dk/research/proteomics/mann/).
 
 
 * [**Citation**](#citation)
 * [**Installation**](#installation)
 * [**Troubleshooting**](#troubleshooting)
 * [**License**](#license)
```

### Comparing `alphastats-0.5.4/alphastats/DataSet.py` & `alphastats-0.6.0/alphastats/DataSet.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import plotly
 
 from alphastats.loader.AlphaPeptLoader import AlphaPeptLoader
 from alphastats.loader.DIANNLoader import DIANNLoader
 from alphastats.loader.FragPipeLoader import FragPipeLoader
 from alphastats.loader.MaxQuantLoader import MaxQuantLoader
 from alphastats.loader.SpectronautLoader import SpectronautLoader
+from alphastats.loader.mzTabLoader import mzTabLoader
 
 from alphastats.DataSet_Plot import Plot
 from alphastats.DataSet_Preprocess import Preprocess
 from alphastats.DataSet_Pathway import Enrichment
 from alphastats.DataSet_Statistics import Statistics
 from alphastats.utils import LoaderError
 
@@ -92,15 +93,15 @@
     def _check_loader(self, loader):
         """Checks if the Loader is from class AlphaPeptLoader, MaxQuantLoader, DIANNLoader, FragPipeLoader
 
         Args:
             loader : loader
         """
         if not isinstance(
-            loader, (AlphaPeptLoader, MaxQuantLoader, DIANNLoader, FragPipeLoader, SpectronautLoader)
+            loader, (AlphaPeptLoader, MaxQuantLoader, DIANNLoader, FragPipeLoader, SpectronautLoader, mzTabLoader)
         ):
             raise LoaderError(
                 "loader must be from class: AlphaPeptLoader, MaxQuantLoader, DIANNLoader, FragPipeLoader or SpectronautLoader"
             )
 
         if not isinstance(loader.rawinput, pd.DataFrame) or loader.rawinput.empty:
             raise ValueError(
```

### Comparing `alphastats-0.5.4/alphastats/DataSet_Pathway.py` & `alphastats-0.6.0/alphastats/DataSet_Pathway.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/DataSet_Plot.py` & `alphastats-0.6.0/alphastats/DataSet_Plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,37 +115,39 @@
         )
         return dimensionality_reduction.plot
 
     def plot_volcano(
         self,
         group1,
         group2,
-        column=None,
-        method="ttest",
-        labels=False,
-        min_fc=1,
-        alpha=0.05,
-        draw_line=True,
-        perm=100, 
-        fdr=0.05,
-        compare_preprocessing_modes=False
+        column:str=None,
+        method:str="ttest",
+        labels:bool=False,
+        min_fc:float=1.0,
+        alpha:float=0.05,
+        draw_line:bool=True,
+        perm:int=100, 
+        fdr:float=0.05,
+        compare_preprocessing_modes:bool=False,
+        color_list:list=[]
     ):
         """Plot Volcano Plot
 
         Args:
             column (str): column name in the metadata file with the two groups to compare
             group1 (str/list): name of group to compare needs to be present in column or list of sample names to compare
             group2 (str/list): name of group to compare needs to be present in column  or list of sample names to compare
             method (str): "anova", "wald", "ttest", "SAM" Defaul ttest.
             labels (bool): Add text labels to significant Proteins, Default False.
             alpha(float,optional): p-value cut off.
             min_fc (float): Minimum fold change.
             draw_line(boolean): whether to draw cut off lines.
             perm(float,optional): number of permutations when using SAM as method. Defaults to 100.
             fdr(float,optional): FDR cut off when using SAM as method. Defaults to 0.05.
+            color_list (list): list with ProteinIDs that should be highlighted.
             compare_preprocessing_modes(bool): Will iterate through normalization and imputation modes and return a list of VolcanoPlots in different settings, Default False.
 
 
         Returns:
             plotly.graph_objects._figure.Figure: Volcano Plot
         """
 
@@ -162,15 +164,16 @@
                 column=column,
                 method=method,
                 labels=labels,
                 min_fc=min_fc,
                 alpha=alpha,
                 draw_line=draw_line,
                 perm=perm, 
-                fdr=fdr
+                fdr=fdr,
+                color_list=color_list
             )
 
             return volcano_plot.plot
 
     def plot_correlation_matrix(self, method="pearson"):
         """Plot Correlation Matrix
 
@@ -237,15 +240,15 @@
     ):
         """Plot Intensity of individual Protein/ProteinGroup
 
         Args:
             ID (str): ProteinGroup ID
             group (str, optional): A metadata column used for grouping. Defaults to None.
             subgroups (list, optional): Select variables from the group column. Defaults to None.
-            method (str, optional):  Violinplot = "violin", Boxplot = "box", Scatterplot = "scatter". Defaults to "box".
+            method (str, optional):  Violinplot = "violin", Boxplot = "box", Scatterplot = "scatter" or "all". Defaults to "box".
             add_significance (bool, optional): add p-value bar, only possible when two groups are compared. Defaults False.
             log_scale (bool, optional): yaxis in logarithmic scale. Defaults to False.
 
         Returns:
             plotly.graph_objects._figure.Figure: Plotly Plot
         """
         if compare_preprocessing_modes:
```

### Comparing `alphastats-0.5.4/alphastats/DataSet_Preprocess.py` & `alphastats-0.6.0/alphastats/DataSet_Preprocess.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/DataSet_Statistics.py` & `alphastats-0.6.0/alphastats/DataSet_Statistics.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/__init__.py` & `alphastats-0.6.0/alphastats/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __project__ = "alphastats"
-__version__ = "0.5.4"
+__version__ = "0.6.0"
 __license__ = "Apache"
 __description__ = "An open-source Python package for Mass Spectrometry Analysis"
 __author__ = "Mann Labs"
 __author_email__ = "elena.krismer@hotmail.com"
 __github__ = "https://github.com/MannLabs/alphapeptstats"
 __keywords__ = [
     "bioinformatics",
```

### Comparing `alphastats-0.5.4/alphastats/data/contaminations.txt` & `alphastats-0.6.0/alphastats/data/contaminations.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/gui/AlphaPeptStats.py` & `alphastats-0.6.0/alphastats/gui/AlphaPeptStats.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/gui/alphapeptstats_logo.png` & `alphastats-0.6.0/alphastats/gui/alphapeptstats_logo.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/gui/alphastats_logo.png` & `alphastats-0.6.0/alphastats/gui/alphastats_logo.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/gui/alphastats_logo_2.png` & `alphastats-0.6.0/alphastats/gui/alphastats_logo_2.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/gui/gui.py` & `alphastats-0.6.0/alphastats/gui/gui.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/gui/pages/02_Import Data.py` & `alphastats-0.6.0/alphastats/gui/pages/02_Import Data.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/gui/pages/03_Data Overview.py` & `alphastats-0.6.0/alphastats/gui/pages/03_Data Overview.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/gui/pages/03_Preprocessing.py` & `alphastats-0.6.0/alphastats/gui/pages/03_Preprocessing.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/gui/pages/04_Analysis.py` & `alphastats-0.6.0/alphastats/gui/pages/04_Analysis.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/gui/pages/06_Results.py` & `alphastats-0.6.0/alphastats/gui/pages/06_Results.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/gui/sample_data/metadata.xlsx` & `alphastats-0.6.0/alphastats/gui/sample_data/metadata.xlsx`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/gui/sample_data/proteinGroups.txt` & `alphastats-0.6.0/alphastats/gui/sample_data/proteinGroups.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/gui/utils/analysis_helper.py` & `alphastats-0.6.0/alphastats/gui/utils/analysis_helper.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/gui/utils/options.py` & `alphastats-0.6.0/alphastats/gui/utils/options.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/gui/utils/software_options.py` & `alphastats-0.6.0/alphastats/gui/utils/software_options.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/gui/utils/ui_helper.py` & `alphastats-0.6.0/alphastats/gui/utils/ui_helper.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/load_data.py` & `alphastats-0.6.0/alphastats/load_data.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/loader/AlphaPeptLoader.py` & `alphastats-0.6.0/alphastats/loader/AlphaPeptLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/loader/BaseLoader.py` & `alphastats-0.6.0/alphastats/loader/BaseLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/loader/DIANNLoader.py` & `alphastats-0.6.0/alphastats/loader/DIANNLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/loader/FragPipeLoader.py` & `alphastats-0.6.0/alphastats/loader/FragPipeLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/loader/MaxQuantLoader.py` & `alphastats-0.6.0/alphastats/loader/MaxQuantLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/loader/SpectronautLoader.py` & `alphastats-0.6.0/alphastats/loader/SpectronautLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/multicova/multicova.py` & `alphastats-0.6.0/alphastats/multicova/multicova.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/plots/ClusterMap.py` & `alphastats-0.6.0/alphastats/plots/ClusterMap.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/plots/DimensionalityReduction.py` & `alphastats-0.6.0/alphastats/plots/DimensionalityReduction.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/plots/IntensityPlot.py` & `alphastats-0.6.0/alphastats/plots/IntensityPlot.py`

 * *Files 11% similar despite different names*

```diff
@@ -124,14 +124,20 @@
             )
 
         elif self.method == "scatter":
             fig = px.scatter(
                  self.prepared_df, y=self.protein_id, x=self.group, color=self.group, labels={self.protein_id: self.y_label}
             )
 
+        elif self.method == "all":
+            fig = px.violin(
+                 self.prepared_df, y=self.protein_id, x=self.group, color=self.group, labels={self.protein_id: self.y_label},
+                 box=True, points="all"
+            )
+
         else:
             raise ValueError(
                 f"{self.method} is not available."
                 + "Please select from 'violin' for Violinplot, 'box' for Boxplot and 'scatter' for Scatterplot."
             )
 
         if self.log_scale:
```

### Comparing `alphastats-0.5.4/alphastats/plots/PlotUtils.py` & `alphastats-0.6.0/alphastats/plots/PlotUtils.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/plots/SampleHistogram.py` & `alphastats-0.6.0/alphastats/plots/SampleHistogram.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/plots/VolcanoPlot.py` & `alphastats-0.6.0/alphastats/plots/VolcanoPlot.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 class VolcanoPlot(PlotUtils):
     def __init__(
         self, dataset, group1, group2, 
         column=None, method=None, 
         labels=None, min_fc=None, 
         alpha=None, draw_line=None, 
-        plot=True, perm=100, fdr=0.05
+        plot=True, perm=100, fdr=0.05,
+        color_list=[]
     ):  
         self.dataset = dataset
         self.group1 = group1
         self.group2 = group2
         self.column = column
         self.method = method
         self.labels = labels
@@ -27,14 +28,15 @@
         self.fdr = fdr
         self.alpha = alpha
         self.draw_line = draw_line
         self.hover_data = None
         self.res = None
         self.pvalue_column = None
         self.perm=perm
+        self.color_list = color_list
         self._check_input()
        
         if plot:
             self._perform_differential_expression_analysis()
             self._annotate_result_df()
             self._add_hover_data_columns()
             self._plot()
@@ -262,14 +264,18 @@
                 (self.res["log2fc"] < 0) & (self.res["FDR"] == "sig"),
                 (self.res["log2fc"] > 0) & (self.res["FDR"] == "sig"),
             ]
 
 
         value = ["down", "up"]
         self.res["color"] = np.select(condition, value, default="non_sig")   
+
+        if len(self.color_list) > 0:
+            self.res["color"] = np.where(self.res[self.dataset.index_column].isin(self.color_list), 
+                                          "color", "no_color")   
         
 
     def _add_labels_plot(self):
         """
         add gene names as hover data if they are given
         """
 
@@ -323,28 +329,38 @@
         self.plot.add_trace(go.Scatter(
             x=self.fdr_line[self.fdr_line.fc_s < 0].fc_s,
             y=-np.log10(self.fdr_line[self.fdr_line.fc_s < 0].pvals),
             line_color="black",
             line_shape='spline',
             showlegend=False)
         )
+    
+    def _color_data_points(self):
+         # update coloring
+        if len(self.color_list) == 0:
+            color_dict = {"non_sig": "#404040", "up": "#B65EAF", "down": "#009599"}
+    
+        else:
+            color_dict = {"no_color": "#404040", "color": "#B65EAF"}
+        
+        self.plot = self._update_colors_plotly(self.plot, color_dict=color_dict)
+
 
 
     def _plot(self):
         self.plot = px.scatter(
             self.res,
             x="log2fc",
             y="-log10(p-value)",
             color="color",
             hover_data=self.hover_data,
         )
         
         # update coloring
-        color_dict = {"non_sig": "#404040", "up": "#B65EAF", "down": "#009599"}
-        self.plot = self._update_colors_plotly(self.plot, color_dict=color_dict)
+        self._color_data_points()
 
         if self.labels:
             self._add_labels_plot()
         
         if self.draw_line:
             if self.method == "sam":
                 self._draw_fdr_line()
```

### Comparing `alphastats-0.5.4/alphastats/statistics/Anova.py` & `alphastats-0.6.0/alphastats/statistics/Anova.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/statistics/DifferentialExpressionAnalysis.py` & `alphastats-0.6.0/alphastats/statistics/DifferentialExpressionAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/statistics/MultiCovaAnalysis.py` & `alphastats-0.6.0/alphastats/statistics/MultiCovaAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/statistics/StatisticUtils.py` & `alphastats-0.6.0/alphastats/statistics/StatisticUtils.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats/utils.py` & `alphastats-0.6.0/alphastats/utils.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.5.4/alphastats.egg-info/PKG-INFO` & `alphastats-0.6.0/alphastats.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphastats
-Version: 0.5.4
+Version: 0.6.0
 Summary: An open-source Python package for Mass Spectrometry Analysis
 Home-page: https://github.com/MannLabs/alphastats
 Author: Mann Labs
 Author-email: elena.krismer@hotmail.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: GitHub, https://github.com/MannLabs/alphapeptstats
@@ -43,14 +43,27 @@
 </div>
 
 <br>
 <br>
 
 [link]:https://alphapeptstats.readthedocs.io/en/main/
 
+<div align = center>
+<br>
+<br>
+
+[<kbd> <br> Streamlit WebApp <br> </kbd>][link_streamlit]
+
+</div>
+
+<br>
+<br>
+
+[link_streamlit]:https://mannlabs-alphapeptstats-alphastatsguialphapeptstats-qyzgwd.streamlit.app/
+
 An open-source Python package for downstream mass spectrometry downstream data analysis from the [Mann Group at the University of Copenhagen](https://www.cpr.ku.dk/research/proteomics/mann/).
 
 
 * [**Citation**](#citation)
 * [**Installation**](#installation)
 * [**Troubleshooting**](#troubleshooting)
 * [**License**](#license)
```

### Comparing `alphastats-0.5.4/alphastats.egg-info/SOURCES.txt` & `alphastats-0.6.0/alphastats.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -41,20 +41,24 @@
 alphastats/loader/AlphaPeptLoader.py
 alphastats/loader/BaseLoader.py
 alphastats/loader/DIANNLoader.py
 alphastats/loader/FragPipeLoader.py
 alphastats/loader/MaxQuantLoader.py
 alphastats/loader/SpectronautLoader.py
 alphastats/loader/__init__.py
+alphastats/loader/mzTabLoader.py
 alphastats/multicova/__init__.py
 alphastats/multicova/multicova.py
 alphastats/plots/ClusterMap.py
 alphastats/plots/DimensionalityReduction.py
 alphastats/plots/IntensityPlot.py
 alphastats/plots/PlotUtils.py
 alphastats/plots/SampleHistogram.py
 alphastats/plots/VolcanoPlot.py
 alphastats/plots/__init__.py
 alphastats/statistics/Anova.py
 alphastats/statistics/DifferentialExpressionAnalysis.py
 alphastats/statistics/MultiCovaAnalysis.py
-alphastats/statistics/StatisticUtils.py
+alphastats/statistics/StatisticUtils.py
+tests/test_DataSet.py
+tests/test_DataSet_Pathway.py
+tests/test_loaders.py
```

### Comparing `alphastats-0.5.4/setup.py` & `alphastats-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     return required
     
 
 def create_pip_wheel():
     requirements = get_requirements()
     setuptools.setup(
         name="alphastats",
-        version="0.5.4",
+        version="0.6.0",
         license="Apache",
         description="An open-source Python package for Mass Spectrometry Analysis",
         long_description=get_long_description(),
         long_description_content_type="text/markdown",
         author="Mann Labs",
         author_email="elena.krismer@hotmail.com",
         url="https://github.com/MannLabs/alphastats",
```

