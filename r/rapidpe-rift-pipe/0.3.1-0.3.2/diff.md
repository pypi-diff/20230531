# Comparing `tmp/rapidpe_rift_pipe-0.3.1.tar.gz` & `tmp/rapidpe_rift_pipe-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpe_rift_pipe-0.3.1.tar", last modified: Tue May 30 23:55:42 2023, max compression
+gzip compressed data, was "rapidpe_rift_pipe-0.3.2.tar", last modified: Wed May 31 13:37:38 2023, max compression
```

## Comparing `rapidpe_rift_pipe-0.3.1.tar` & `rapidpe_rift_pipe-0.3.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:55:42.395410 rapidpe_rift_pipe-0.3.1/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1128 2023-05-30 23:55:42.395410 rapidpe_rift_pipe-0.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:55:42.391410 rapidpe_rift_pipe-0.3.1/bin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:55:42.392410 rapidpe_rift_pipe-0.3.1/bin/postscripts/
--rw-rw-rw-   0 root         (0) root         (0)    10056 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/bin/postscripts/compute_posterior.py
--rwxrwxrwx   0 root         (0) root         (0)    12423 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/bin/postscripts/convert_result_to_txt.py
--rw-rw-rw-   0 root         (0) root         (0)     6342 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/bin/postscripts/cprofile_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     5579 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/bin/postscripts/create_summarypage.py
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/bin/postscripts/plot_skymap.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-30 23:55:42.396410 rapidpe_rift_pipe-0.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:55:42.391410 rapidpe_rift_pipe-0.3.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:55:42.394410 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    44671 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    18503 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:55:42.395410 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/config_files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/config_files/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:55:42.395410 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4536 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
--rwxrwxrwx   0 root         (0) root         (0)    31454 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/jacobians.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     4719 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/pastro.py
--rw-rw-rw-   0 root         (0) root         (0)    27658 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/postscript_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/search_bias_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:55:42.395410 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/static/stylesheet.css
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:55:42.395410 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1128 2023-05-30 23:55:42.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2023-05-30 23:55:42.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 23:55:42.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-30 23:55:42.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-05-30 23:55:42.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-30 23:55:42.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 23:55:42.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:37:38.420310 rapidpe_rift_pipe-0.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-05-31 13:37:38.420310 rapidpe_rift_pipe-0.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:37:38.410310 rapidpe_rift_pipe-0.3.2/bin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:37:38.413310 rapidpe_rift_pipe-0.3.2/bin/postscripts/
+-rw-rw-rw-   0 root         (0) root         (0)    10056 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/bin/postscripts/compute_posterior.py
+-rwxrwxrwx   0 root         (0) root         (0)    12423 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/bin/postscripts/convert_result_to_txt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6342 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/bin/postscripts/cprofile_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     5579 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/bin/postscripts/create_summarypage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/bin/postscripts/plot_skymap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-31 13:37:38.421310 rapidpe_rift_pipe-0.3.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:37:38.410310 rapidpe_rift_pipe-0.3.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:37:38.417310 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    44671 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    18503 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:37:38.419310 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/config_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/config_files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:37:38.419310 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+-rwxrwxrwx   0 root         (0) root         (0)    31454 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/jacobians.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4719 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/pastro.py
+-rw-rw-rw-   0 root         (0) root         (0)    27658 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/postscript_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/search_bias_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:37:38.420310 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/static/stylesheet.css
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-05-31 13:37:26.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:37:38.418310 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-05-31 13:37:38.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-05-31 13:37:38.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 13:37:38.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-31 13:37:38.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-05-31 13:37:38.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-31 13:37:38.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 13:37:38.000000 rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe.egg-info/zip-safe
```

### Comparing `rapidpe_rift_pipe-0.3.1/COPYING` & `rapidpe_rift_pipe-0.3.2/COPYING`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.1/PKG-INFO` & `rapidpe_rift_pipe-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe_rift_pipe
-Version: 0.3.1
+Version: 0.3.2
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.3.1/bin/postscripts/compute_posterior.py` & `rapidpe_rift_pipe-0.3.2/bin/postscripts/compute_posterior.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.1/bin/postscripts/convert_result_to_txt.py` & `rapidpe_rift_pipe-0.3.2/bin/postscripts/convert_result_to_txt.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.1/bin/postscripts/cprofile_summary.py` & `rapidpe_rift_pipe-0.3.2/bin/postscripts/cprofile_summary.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.1/bin/postscripts/create_summarypage.py` & `rapidpe_rift_pipe-0.3.2/bin/postscripts/create_summarypage.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.1/bin/postscripts/plot_skymap.py` & `rapidpe_rift_pipe-0.3.2/bin/postscripts/plot_skymap.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.1/setup.cfg` & `rapidpe_rift_pipe-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/cli.py` & `rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,19 +458,19 @@
                 )
                 # Buffer for inverse spectrum truncation.
 
                 t_before_cache = 200
                 t_after_cache = 14
                 t_mr_buffer = 10
                 t_duration_buffer = 50
-                data_start_time = int(t_event - t_duration_buffer)
-                data_end_time = int(t_event + t_mr_buffer)
+                data_start_time = int(t_event - t_before_cache)
+                data_end_time = int(t_event + t_after_cache)
 
-                event_info['data_start_time'] = int(t_event - t_before_cache)
-                event_info['data_end_time'] = int(t_event + t_after_cache)
+                event_info['data_start_time'] = int(t_event - t_duration_buffer)
+                event_info['data_end_time'] = int(t_event + t_mr_buffer)
 
                 data_type = config.event.frame_data_types[ifo]
                 # TODO: We should import gwdatafind and call the underlying
                 #       functions directly.
                 raw_cache_file_path = os.path.join(output_dir,f"{ifo[0]}_raw.cache")
                 dcmd = (
                     "python -m gwdatafind -u file "
```

### Comparing `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/config.py` & `rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json` & `rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/create_submit_dag_one_event.py` & `rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/create_submit_dag_one_event.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/jacobians.py` & `rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/jacobians.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/modules.py` & `rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/modules.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/pastro.py` & `rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/pastro.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/postscript_utils.py` & `rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/postscript_utils.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/profiling.py` & `rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/profiling.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/search_bias_bounds.py` & `rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/search_bias_bounds.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/static/stylesheet.css` & `rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/static/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/test_config.py` & `rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe/test_config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/PKG-INFO` & `rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe-rift-pipe
-Version: 0.3.1
+Version: 0.3.2
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/SOURCES.txt` & `rapidpe_rift_pipe-0.3.2/src/rapidpe_rift_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

