# Comparing `tmp/rapidpe_rift_pipe-0.3.0.tar.gz` & `tmp/rapidpe_rift_pipe-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpe_rift_pipe-0.3.0.tar", last modified: Thu May 18 20:48:49 2023, max compression
+gzip compressed data, was "rapidpe_rift_pipe-0.3.1.tar", last modified: Tue May 30 23:55:42 2023, max compression
```

## Comparing `rapidpe_rift_pipe-0.3.0.tar` & `rapidpe_rift_pipe-0.3.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:49.696423 rapidpe_rift_pipe-0.3.0/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1128 2023-05-18 20:48:49.696423 rapidpe_rift_pipe-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:49.515417 rapidpe_rift_pipe-0.3.0/bin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:49.518417 rapidpe_rift_pipe-0.3.0/bin/postscripts/
--rw-rw-rw-   0 root         (0) root         (0)    10056 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/bin/postscripts/compute_posterior.py
--rwxrwxrwx   0 root         (0) root         (0)    12423 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/bin/postscripts/convert_result_to_txt.py
--rw-rw-rw-   0 root         (0) root         (0)     6342 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/bin/postscripts/cprofile_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     5579 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/bin/postscripts/create_summarypage.py
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/bin/postscripts/plot_skymap.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-18 20:48:49.698423 rapidpe_rift_pipe-0.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:49.515417 rapidpe_rift_pipe-0.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:49.685423 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-18 20:44:54.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    40087 2023-05-18 18:03:43.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    18503 2023-05-18 18:03:43.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:49.693423 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/config_files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-18 20:48:33.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/config_files/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:49.694423 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-18 20:48:33.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4536 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
--rwxrwxrwx   0 root         (0) root         (0)    31226 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/jacobians.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     4719 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/pastro.py
--rw-rw-rw-   0 root         (0) root         (0)    27658 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/postscript_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/search_bias_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:49.696423 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-18 20:48:33.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/static/stylesheet.css
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-05-18 05:13:30.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 20:48:49.693423 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1128 2023-05-18 20:48:49.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2023-05-18 20:48:49.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:48:49.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-18 20:48:49.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-05-18 20:48:49.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-18 20:48:49.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 20:48:49.000000 rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:55:42.395410 rapidpe_rift_pipe-0.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-05-30 23:55:42.395410 rapidpe_rift_pipe-0.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:55:42.391410 rapidpe_rift_pipe-0.3.1/bin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:55:42.392410 rapidpe_rift_pipe-0.3.1/bin/postscripts/
+-rw-rw-rw-   0 root         (0) root         (0)    10056 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/bin/postscripts/compute_posterior.py
+-rwxrwxrwx   0 root         (0) root         (0)    12423 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/bin/postscripts/convert_result_to_txt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6342 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/bin/postscripts/cprofile_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     5579 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/bin/postscripts/create_summarypage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/bin/postscripts/plot_skymap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-30 23:55:42.396410 rapidpe_rift_pipe-0.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:55:42.391410 rapidpe_rift_pipe-0.3.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:55:42.394410 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-30 23:55:28.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    44671 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    18503 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:55:42.395410 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/config_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/config_files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:55:42.395410 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+-rwxrwxrwx   0 root         (0) root         (0)    31454 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/jacobians.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4719 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/pastro.py
+-rw-rw-rw-   0 root         (0) root         (0)    27658 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/postscript_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/search_bias_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:55:42.395410 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/static/stylesheet.css
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-05-30 23:55:29.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 23:55:42.395410 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-05-30 23:55:42.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-05-30 23:55:42.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 23:55:42.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-30 23:55:42.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-05-30 23:55:42.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-30 23:55:42.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 23:55:42.000000 rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/zip-safe
```

### Comparing `rapidpe_rift_pipe-0.3.0/COPYING` & `rapidpe_rift_pipe-0.3.1/COPYING`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.0/PKG-INFO` & `rapidpe_rift_pipe-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe_rift_pipe
-Version: 0.3.0
+Version: 0.3.1
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.3.0/bin/postscripts/compute_posterior.py` & `rapidpe_rift_pipe-0.3.1/bin/postscripts/compute_posterior.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.0/bin/postscripts/convert_result_to_txt.py` & `rapidpe_rift_pipe-0.3.1/bin/postscripts/convert_result_to_txt.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.0/bin/postscripts/cprofile_summary.py` & `rapidpe_rift_pipe-0.3.1/bin/postscripts/cprofile_summary.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.0/bin/postscripts/create_summarypage.py` & `rapidpe_rift_pipe-0.3.1/bin/postscripts/create_summarypage.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.0/bin/postscripts/plot_skymap.py` & `rapidpe_rift_pipe-0.3.1/bin/postscripts/plot_skymap.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.0/setup.cfg` & `rapidpe_rift_pipe-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/cli.py` & `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 import time
 import glob
 import h5py
 import shutil
 import numpy as np
 import lal
+import requests.exceptions
 from rapid_pe import lalsimutils
 from argparse import ArgumentParser
 from ligo.gracedb.rest import GraceDb, HTTPError
 from rapidpe_rift_pipe.modules import (
     check_switch_m1m2s1s2,
     convert_injections_txt_to_objects,
     construct_event_time_string,
@@ -91,14 +92,16 @@
     if cli_args.verbose:
         logging_level = logging.DEBUG
     else:
         logging_level = logging.INFO
 
     logging.basicConfig(level=logging_level)
 
+    logging.info(os.uname())
+
     cfgname = os.path.abspath(cli_args.config)
     config = Config.load(cfgname)
 
     # TODO: make this a configuration option
     init_directory = os.getcwd()
     output_parent_directory = config.output_parent_directory
     use_skymap = config.use_skymap
@@ -146,16 +149,76 @@
             client = GraceDb(config.gracedb_url)
             event = None
             # TODO: check whether we should be getting the submitter name
 #            submitter = ""
             packet = ""
             lvalert = False
             if config.event.mode == 'sid':
-                sevent = client.superevent(config.event.superevent_id).json()
-                gracedb_id = sevent['preferred_event']
+                retry_times = [1]*2 + [5]*2 + [30]*2
+                alt_http_retry_times = {408:30, 429:60, 502:20, 503:20, 504:30}
+                tried_events = set()
+                gracedb_id = None
+                for retry_time in retry_times:
+                    is_failed = False
+                    try:
+                        sevent = client.superevent(config.event.superevent_id).json()
+                    except HTTPError as e:
+                        logging.exception(f'Failed while requesting superevent {config.event.superevent_id}')
+                        retry_time = alt_http_retry_times.get(e.status_code, retry_time) 
+                        is_failed = True
+                    except requests.exceptions.JSONDecodeError as e:
+                        logging.exception(f'Failed while parsing superevent {config.event.superevent_id}')
+                        is_failed = True
+                    if not is_failed:
+                        try:
+                            if sevent['preferred_event_data']['pipeline']=='gstlal':
+                                gracedb_id = sevent['preferred_event']
+                                logging.info(f"Using preferred_event: {gracedb_id}")
+                                break
+                            elif 'gstlal' in sevent['pipeline_preferred_events']:
+                                gracedb_id = sevent['pipeline_preferred_events']['gstlal']['graceid']
+                                logging.info(f"Using GstLAL preferred event: {gracedb_id}")
+                                break
+                            else:
+                                gw_events = sevent["gw_events"]
+                                new_gw_events = set(gw_events) - tried_events
+                                gstlal_event_snr = 0.0
+                                for event_name in new_gw_events:
+                                    try:
+                                        event = client.event(event_name).json()
+                                    except HTTPError as e:
+                                        logging.exception(f"Failed while requesting gevent {event_name}")
+                                        retry_time = alt_http_retry_time.get(e.status_code, retry_time)
+                                        continue
+                                    except requests.exceptions.JSONDecodeError as e:
+                                        logging.exception(f'Failed while parsing gevent {event_name}')
+                                        continue
+                                    try:
+                                        event_snr = event['extra_attributes']['CoincInspiral']['snr']
+                                        if event['pipeline'] == 'gstlal' and event_snr>gstlal_event_snr and event['search']=='AllSky':
+                                            gracedb_id = event_name
+                                            gstlal_event_snr = event_snr
+                                            logging.info(f'Updating selected event: {event_name}')
+                                        else:
+                                            logging.info(f'Skipping {event_name}')
+                                    except KeyError:
+                                        logging.exception(f'missing key in {event_name}')
+                                        continue
+                                    tried_events.add(event_name)
+                                if gracedb_id:
+                                    logging.info(f"Using highest snr trigger from GstLAL: {gracedb_id}")
+                                    break
+                        except KeyError:
+                            logging.exception('missing key')
+                    if gracedb_id is None:
+                        logging.info("No GstLAL event found, retrying in %s seconds", retry_time)
+                        time.sleep(retry_time)
+                if gracedb_id is None:
+                    logging.error("No GstLAL event found after %s seconds", sum(retry_times))
+                    sys.exit(1)
             elif config.event.mode == 'gid':
                 gracedb_id = config.event.gracedb_id
             else:
                 raise RuntimeError(f'Unknown mode {config.event.mode}')
             gracedb_id = get_graceid_after_superevent_check(
                 gracedb_id, client,
                 output_parent_directory,
@@ -390,34 +453,46 @@
                 logging.info(
                     "DONE Estimate duration: %s, %s, %s",
                     t_duration,
                     coinc["minimum_duration"],
                     lalsimutils.estimateWaveformDuration(P)
                 )
                 # Buffer for inverse spectrum truncation.
-                t_before = max(4, t_duration) * 1.2 + 30
-                # TODO: double-check these parentheses are intentionally placed
-                data_start_time = int(t_event - int(t_before))
-                data_end_time = int(t_event + 500)
+
+                t_before_cache = 200
+                t_after_cache = 14
+                t_mr_buffer = 10
+                t_duration_buffer = 50
+                data_start_time = int(t_event - t_duration_buffer)
+                data_end_time = int(t_event + t_mr_buffer)
+
+                event_info['data_start_time'] = int(t_event - t_before_cache)
+                event_info['data_end_time'] = int(t_event + t_after_cache)
 
                 data_type = config.event.frame_data_types[ifo]
                 # TODO: We should import gwdatafind and call the underlying
                 #       functions directly.
                 raw_cache_file_path = os.path.join(output_dir,f"{ifo[0]}_raw.cache")
                 dcmd = (
                     "python -m gwdatafind -u file "
                     f"-o {ifo[0]} -t {data_type} -s {data_start_time} "
                     f"-e {data_end_time} > {raw_cache_file_path}"
                 )
                 logging.info(dcmd)
-                exit_status = os.system(dcmd)
-                if exit_status != 0:
-                    logging.error(dcmd)
-                    sys.exit(f"ERROR: non zero exit status {exit_status}")
-
+                retry_times = [1] + [5] + [500]*2
+                for retry_time in retry_times:
+                    exit_status = os.system(dcmd)
+                    if exit_status == 0 and os.stat(raw_cache_file_path).st_size != 0:
+                        break
+                    else:
+                        logging.error(f"There is no data at the time when this triggered. Retry in {retry_time} seconds")
+                        time.sleep(retry_time)
+                else:
+                    logging.error(f"data not found after {sum(retry_times)} seconds")
+                    sys.exit(1)
                 num_ifos += 1
 
             if num_ifos == 0:
                 logging.error("Failed to load data from any IFOs.")
 
             # path2cache always assumes data is in output_dir, so that path
             # needs to be removed before passing output to data.cache
```

### Comparing `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/config.py` & `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json` & `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/create_submit_dag_one_event.py` & `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/create_submit_dag_one_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,17 @@
         sys.exit("ERROR: event specific info specified in LikelihoodIntegration of config and in command line or Event section of config. event_time, psd_file,cache_file and channel_name must be specified in the [Event] section or in the input event dictionary ")
     else:
         integrate_likelihood_cmds_dict["event-time"] = event_info["event_time"]
         integrate_likelihood_cmds_dict["psd-file"] = event_info["psd_file"]
         integrate_likelihood_cmds_dict["channel-name"] = event_info["channel_name"]
         integrate_likelihood_cmds_dict["cache-file"] = event_info["cache_file"]
         integrate_likelihood_cmds_dict["approximant"] = event_info["approximant"]
+        if "data_start_time" in event_info:
+            integrate_likelihood_cmds_dict["data-start-time"] = event_info["data_start_time"]
+            integrate_likelihood_cmds_dict["data-end-time"] = event_info["data_end_time"]
         if "skymap_file" in event_info:
             integrate_likelihood_cmds_dict["skymap-file"] = event_info["skymap_file"]
 
     if config.submit_only_at_exact_signal_position:
         #This is the filename for the output at each intrinsic grid point
         integration_output_file_name = os.path.join(output_dir,"results/ILE_iteration_exact_intrinsic")
         if 'injection_param' in event_info:
```

### Comparing `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/jacobians.py` & `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/jacobians.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/modules.py` & `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/modules.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/pastro.py` & `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/pastro.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/postscript_utils.py` & `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/postscript_utils.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/profiling.py` & `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/profiling.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/search_bias_bounds.py` & `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/search_bias_bounds.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/static/stylesheet.css` & `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/static/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe/test_config.py` & `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe/test_config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/PKG-INFO` & `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe-rift-pipe
-Version: 0.3.0
+Version: 0.3.1
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.3.0/src/rapidpe_rift_pipe.egg-info/SOURCES.txt` & `rapidpe_rift_pipe-0.3.1/src/rapidpe_rift_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

