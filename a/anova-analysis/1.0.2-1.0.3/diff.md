# Comparing `tmp/anova_analysis-1.0.2.tar.gz` & `tmp/anova_analysis-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anova_analysis-1.0.2.tar", last modified: Wed May 31 14:06:32 2023, max compression
+gzip compressed data, was "anova_analysis-1.0.3.tar", last modified: Wed May 31 19:35:09 2023, max compression
```

## Comparing `anova_analysis-1.0.2.tar` & `anova_analysis-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 14:06:32.812563 anova_analysis-1.0.2/
--rw-rw-rw-   0        0        0     1084 2023-05-31 13:55:24.000000 anova_analysis-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2336 2023-05-31 14:06:32.811539 anova_analysis-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1809 2023-05-27 13:20:41.000000 anova_analysis-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 14:06:32.801035 anova_analysis-1.0.2/anova_analysis/
--rw-rw-rw-   0        0        0     2689 2023-05-27 12:56:56.000000 anova_analysis-1.0.2/anova_analysis/ANOVA_RBD.py
--rw-rw-rw-   0        0        0        0 2023-05-27 05:22:10.000000 anova_analysis-1.0.2/anova_analysis/__init__.py
--rw-rw-rw-   0        0        0      154 2023-05-27 13:16:33.000000 anova_analysis-1.0.2/anova_analysis/example.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:06:32.810381 anova_analysis-1.0.2/anova_analysis.egg-info/
--rw-rw-rw-   0        0        0     2336 2023-05-31 14:06:32.000000 anova_analysis-1.0.2/anova_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-05-31 14:06:32.000000 anova_analysis-1.0.2/anova_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 14:06:32.000000 anova_analysis-1.0.2/anova_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-31 14:06:32.000000 anova_analysis-1.0.2/anova_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-31 14:06:32.000000 anova_analysis-1.0.2/anova_analysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 14:06:32.812563 anova_analysis-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      953 2023-05-31 14:04:40.000000 anova_analysis-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:35:09.507789 anova_analysis-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-31 19:34:57.000000 anova_analysis-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-31 19:35:09.507789 anova_analysis-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-31 19:34:57.000000 anova_analysis-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:35:09.507789 anova_analysis-1.0.3/anova_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-31 19:34:57.000000 anova_analysis-1.0.3/anova_analysis/ANOVA_RBD.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:34:57.000000 anova_analysis-1.0.3/anova_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-31 19:34:57.000000 anova_analysis-1.0.3/anova_analysis/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:35:09.507789 anova_analysis-1.0.3/anova_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-31 19:35:09.000000 anova_analysis-1.0.3/anova_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-31 19:35:09.000000 anova_analysis-1.0.3/anova_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:35:09.000000 anova_analysis-1.0.3/anova_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 19:35:09.000000 anova_analysis-1.0.3/anova_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 19:35:09.000000 anova_analysis-1.0.3/anova_analysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:35:09.507789 anova_analysis-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-31 19:34:57.000000 anova_analysis-1.0.3/setup.py
```

### Comparing `anova_analysis-1.0.2/LICENSE.txt` & `anova_analysis-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

