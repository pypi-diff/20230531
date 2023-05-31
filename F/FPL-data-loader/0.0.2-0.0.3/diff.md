# Comparing `tmp/FPL-data-loader-0.0.2.tar.gz` & `tmp/FPL-data-loader-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FPL-data-loader-0.0.2.tar", last modified: Tue May 30 20:53:12 2023, max compression
+gzip compressed data, was "FPL-data-loader-0.0.3.tar", last modified: Wed May 31 20:14:40 2023, max compression
```

## Comparing `FPL-data-loader-0.0.2.tar` & `FPL-data-loader-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:53:12.947864 FPL-data-loader-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-30 20:52:45.000000 FPL-data-loader-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-30 20:53:12.947864 FPL-data-loader-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 20:52:45.000000 FPL-data-loader-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-30 20:52:45.000000 FPL-data-loader-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 20:53:12.947864 FPL-data-loader-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:53:12.943864 FPL-data-loader-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:53:12.947864 FPL-data-loader-0.0.2/src/FPL_data_loader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-30 20:53:12.000000 FPL-data-loader-0.0.2/src/FPL_data_loader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-30 20:53:12.000000 FPL-data-loader-0.0.2/src/FPL_data_loader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:53:12.000000 FPL-data-loader-0.0.2/src/FPL_data_loader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 20:53:12.000000 FPL-data-loader-0.0.2/src/FPL_data_loader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 20:53:12.000000 FPL-data-loader-0.0.2/src/FPL_data_loader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:53:12.947864 FPL-data-loader-0.0.2/src/fpl_data/
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-30 20:52:45.000000 FPL-data-loader-0.0.2/src/fpl_data/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-30 20:52:45.000000 FPL-data-loader-0.0.2/src/fpl_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:40.955365 FPL-data-loader-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-31 20:14:04.000000 FPL-data-loader-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-31 20:14:40.955365 FPL-data-loader-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-31 20:14:04.000000 FPL-data-loader-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-31 20:14:04.000000 FPL-data-loader-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 20:14:40.959365 FPL-data-loader-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:40.955365 FPL-data-loader-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:40.955365 FPL-data-loader-0.0.3/src/FPL_data_loader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-31 20:14:40.000000 FPL-data-loader-0.0.3/src/FPL_data_loader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-31 20:14:40.000000 FPL-data-loader-0.0.3/src/FPL_data_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:14:40.000000 FPL-data-loader-0.0.3/src/FPL_data_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-31 20:14:40.000000 FPL-data-loader-0.0.3/src/FPL_data_loader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 20:14:40.000000 FPL-data-loader-0.0.3/src/FPL_data_loader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:40.955365 FPL-data-loader-0.0.3/src/fpl_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-31 20:14:04.000000 FPL-data-loader-0.0.3/src/fpl_data/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-31 20:14:04.000000 FPL-data-loader-0.0.3/src/fpl_data/utils.py
```

### Comparing `FPL-data-loader-0.0.2/LICENSE` & `FPL-data-loader-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FPL-data-loader-0.0.2/pyproject.toml` & `FPL-data-loader-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 requires = [
   "setuptools>=67"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "FPL-data-loader"
-version = "0.0.2"
+version = "0.0.3"
 description = "Tools for working with Fantasy Premier League data"
 authors = [
   { name="James Leslie", email="contactjamesleslie@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
   "tqdm==4.65.0",
-  "jsonschema==4.17.3"
+  "jsonschema>=4.17.3",
+  "requests>=2.29.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/James-Leslie/fpl-data"
 "Bug Tracker" = "https://github.com/James-Leslie/fpl-data/issues"
 
 [tool.setuptools]
```

### Comparing `FPL-data-loader-0.0.2/src/fpl_data/api.py` & `FPL-data-loader-0.0.3/src/fpl_data/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,16 @@
 import requests
-# import time
-# from tqdm.auto import tqdm
+import time
+from tqdm.auto import tqdm
 from fpl_data.utils import drop_keys
 
 
 BASE_URL = 'https://fantasy.premierleague.com/api/'
 
 
-# def get_element_summary(player_id, type):
-#     '''Get all past season info for a given player_id,
-#        wait between requests to avoid API rate limit'''
-
-#     success = False
-#     # try until a result is returned
-#     while not success:
-#         try:
-#             # send GET request to BASE_URL/api/element-summary/{PID}/
-#             data = requests.get(
-#                 BASE_URL + 'element-summary/' + str(player_id) + '/').json()
-#             success = True
-#         except:
-#             # wait a bit to avoid API rate limits, if needed
-#             time.sleep(.3)
-
-#     # extract 'history_past' data from response into dataframe
-#     df = pd.json_normalize(data[type])
-
-#     # season history needs player id column added
-#     if type == 'history_past':
-#         df.insert(0, 'id', player_id)
-
-#     return df
-
-
 class FplApiData:
 
     def __init__(self):
         '''Downloads all relevant data from FPL API, including:
           - elements (players)
           - element_types (positions)
           - teams
@@ -59,7 +33,63 @@
         # fixture data
         fixtures = requests.get(BASE_URL+'fixtures/').json()
         # # drop unnecessary keys
         # drop_cols = ['code', 'finished_provisional', 'minutes',
         #              'provisional_start_time', 'started', 'stats', 'pulse_id']
         # fixtures = [drop_keys(f, drop_cols) for f in fixtures]
         self.fixtures = fixtures
+
+        # Get current season
+        first_deadline = self.events[0]['deadline_time']
+        # Extract the year portion from the date string
+        year = first_deadline[:4]
+        # Calculate the next year
+        self.season = f'{year}-{str(int(year) + 1)[-2:]}'
+
+
+    def get_all_element_summaries(self):
+        '''Get summaries for each element'''
+        history = []
+        history_past = []
+
+        # get all element_ids from self.elements
+        element_ids = [e['id'] for e in self.elements]
+
+        # loop through all element_ids and get summaries
+        for element_id in tqdm(element_ids):
+            summary = get_element_summary(element_id)
+            # combine summaries of all elements together
+            history += summary['history']
+            history_past += summary['history_past']
+
+        # return current and past season summaries together
+        all_summaries = {
+            'history': history,
+            'history_past': history_past
+        }
+        return all_summaries
+
+
+def get_element_summary(player_id):
+    '''Get all past gameweek/season info for a given player_id,
+       wait between requests to avoid API rate limit'''
+
+    success = False
+    # try until a result is returned
+    while not success:
+        try:
+            # send GET request to BASE_URL/api/element-summary/{PID}/
+            data = requests.get(
+                BASE_URL + 'element-summary/' + str(player_id) + '/').json()
+            success = True
+        except (
+            requests.exceptions.RequestException,
+            requests.exceptions.HTTPError
+        ):
+            # Wait a bit to avoid API rate limits, if needed
+            time.sleep(.3)
+
+    # history_past needs element id key added
+    for d in data['history_past']:
+        d['element'] = player_id
+
+    return data
```

