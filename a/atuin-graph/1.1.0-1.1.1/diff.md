# Comparing `tmp/atuin_graph-1.1.0.tar.gz` & `tmp/atuin_graph-1.1.1.tar.gz`

## Comparing `atuin_graph-1.1.0.tar` & `atuin_graph-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 atuin_graph-1.1.0/.python-version
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 atuin_graph-1.1.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 atuin_graph-1.1.0/.github/workflows/ruff.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atuin_graph-1.1.0/atuin_graph/__init__.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 atuin_graph-1.1.0/atuin_graph/cli.py
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 atuin_graph-1.1.0/atuin_graph/generate_calendar.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 atuin_graph-1.1.0/atuin_graph/web.py
--rw-r--r--   0        0        0  2038139 2020-02-02 00:00:00.000000 atuin_graph-1.1.0/img/shell.history.gif
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 atuin_graph-1.1.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 atuin_graph-1.1.0/LICENSE
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 atuin_graph-1.1.0/README.md
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 atuin_graph-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 atuin_graph-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 atuin_graph-1.1.1/.python-version
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 atuin_graph-1.1.1/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 atuin_graph-1.1.1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atuin_graph-1.1.1/atuin_graph/__init__.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 atuin_graph-1.1.1/atuin_graph/cli.py
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 atuin_graph-1.1.1/atuin_graph/generate_calendar.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 atuin_graph-1.1.1/atuin_graph/web.py
+-rw-r--r--   0        0        0  2038139 2020-02-02 00:00:00.000000 atuin_graph-1.1.1/img/shell.history.gif
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 atuin_graph-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 atuin_graph-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 atuin_graph-1.1.1/README.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 atuin_graph-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 atuin_graph-1.1.1/PKG-INFO
```

### Comparing `atuin_graph-1.1.0/.github/workflows/release.yaml` & `atuin_graph-1.1.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `atuin_graph-1.1.0/atuin_graph/cli.py` & `atuin_graph-1.1.1/atuin_graph/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,18 +12,20 @@
     parser.add_argument("--user", help="user to draw the graph for", required=True)
     parser.add_argument(
         "--from",
         dest="from_",
         metavar="FROM",
         help="day (yyyy-mm-dd) to query from",
     )
+
     parser.add_argument(
         "--until",
         help="day (yyyy-mm-dd) to query until",
     )
+
     parser.add_argument("--atuin_server_config", help="atuin server config path")
     args = parser.parse_args()
 
     if args.atuin_server_config:
         config = args.atuin_server_config
     else:
         config = os.environ["HOME"] + "/.config/atuin/server.toml"
```

### Comparing `atuin_graph-1.1.0/atuin_graph/generate_calendar.py` & `atuin_graph-1.1.1/atuin_graph/generate_calendar.py`

 * *Files identical despite different names*

### Comparing `atuin_graph-1.1.0/atuin_graph/web.py` & `atuin_graph-1.1.1/atuin_graph/web.py`

 * *Files identical despite different names*

### Comparing `atuin_graph-1.1.0/img/shell.history.gif` & `atuin_graph-1.1.1/img/shell.history.gif`

 * *Files identical despite different names*

### Comparing `atuin_graph-1.1.0/LICENSE` & `atuin_graph-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atuin_graph-1.1.0/README.md` & `atuin_graph-1.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -12,22 +12,29 @@
 ## installation
 
 ```bash
 pip install atuin-graph
 ```
 
 ## cli / standalone
-***- `atuin-graph`***: takes a username as input and creates a `user.png` file
+***- `atuin-graph`***: takes a username as input and outputs a `atuin-{user}.png` file
 
-The `-until` parameters allows to query up to a max date, this is useful to create one png per day and create a gif with `imagemagick` for example (`convert -delay 10 -loop 1 *.png atuin.gif`)
+The `-until` and `--from` parameters allow to query from / up to a specified date, this is useful to create one png per day and create a gif with `imagemagick` for example (`convert -delay 10 -loop 1 *.png atuin.gif`)
 
 ```bash
-usage: atuin-graph [-h] --user USER [--until UNTIL]
+atuin-graph -h
+usage: atuin-graph [-h] --user USER [--from FROM] [--until UNTIL] [--atuin_server_config ATUIN_SERVER_CONFIG]
 
-                      [--atuin_server_config ATUIN_SERVER_CONFIG]
+options:
+  -h, --help            show this help message and exit
+  --user USER           user to draw the graph for
+  --from FROM           day (yyyy-mm-dd) to query from
+  --until UNTIL         day (yyyy-mm-dd) to query until
+  --atuin_server_config ATUIN_SERVER_CONFIG
+                        atuin server config path
 ```
 ##  web app
 This package also ships a Flask app which dynamically serves a png for a given user and optional dates
 
  |📅️ | |
 |--------------- | --------------- |
 |from a date| `https://my-atuin-server/graph/username/from/yyyy-mm-dd`|
```

### Comparing `atuin_graph-1.1.0/pyproject.toml` & `atuin_graph-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atuin_graph-1.1.0/PKG-INFO` & `atuin_graph-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atuin-graph
-Version: 1.1.0
+Version: 1.1.1
 Summary: activity graph for atuin
 Project-URL: Homepage, https://github.com/tieum/atuin-graph
 Project-URL: Bug Tracker, https://github.com/tieum/atuin-graph/issues
 Author-email: matthieu@bluegreen.sh
 License-Expression: MIT
 License-File: LICENSE
 Requires-Python: >=3.11
@@ -50,22 +50,29 @@
 ## installation
 
 ```bash
 pip install atuin-graph
 ```
 
 ## cli / standalone
-***- `atuin-graph`***: takes a username as input and creates a `user.png` file
+***- `atuin-graph`***: takes a username as input and outputs a `atuin-{user}.png` file
 
-The `-until` parameters allows to query up to a max date, this is useful to create one png per day and create a gif with `imagemagick` for example (`convert -delay 10 -loop 1 *.png atuin.gif`)
+The `-until` and `--from` parameters allow to query from / up to a specified date, this is useful to create one png per day and create a gif with `imagemagick` for example (`convert -delay 10 -loop 1 *.png atuin.gif`)
 
 ```bash
-usage: atuin-graph [-h] --user USER [--until UNTIL]
+atuin-graph -h
+usage: atuin-graph [-h] --user USER [--from FROM] [--until UNTIL] [--atuin_server_config ATUIN_SERVER_CONFIG]
 
-                      [--atuin_server_config ATUIN_SERVER_CONFIG]
+options:
+  -h, --help            show this help message and exit
+  --user USER           user to draw the graph for
+  --from FROM           day (yyyy-mm-dd) to query from
+  --until UNTIL         day (yyyy-mm-dd) to query until
+  --atuin_server_config ATUIN_SERVER_CONFIG
+                        atuin server config path
 ```
 ##  web app
 This package also ships a Flask app which dynamically serves a png for a given user and optional dates
 
  |📅️ | |
 |--------------- | --------------- |
 |from a date| `https://my-atuin-server/graph/username/from/yyyy-mm-dd`|
```

