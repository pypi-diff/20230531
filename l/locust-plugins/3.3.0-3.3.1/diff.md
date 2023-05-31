# Comparing `tmp/locust-plugins-3.3.0.tar.gz` & `tmp/locust-plugins-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locust-plugins-3.3.0.tar", last modified: Fri Apr 28 13:19:17 2023, max compression
+gzip compressed data, was "locust-plugins-3.3.1.tar", last modified: Wed May 31 08:31:34 2023, max compression
```

## Comparing `locust-plugins-3.3.0.tar` & `locust-plugins-3.3.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:17.272642 locust-plugins-3.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:17.256641 locust-plugins-3.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:17.260641 locust-plugins-3.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:17.260641 locust-plugins-3.3.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-28 13:19:17.272642 locust-plugins-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:17.260641 locust-plugins-3.3.0/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/bin/locust-compose
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:17.264641 locust-plugins-3.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/appinsights_listener_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/cmd_line_examples.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/connection_pool_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/constant_total_ips_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/csvreader_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/embedded_resource_manager_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/jmeter_listener_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/kafka_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/mongoreader_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/mqtt_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/playwright-recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/playwright_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/reschedule_on_fail_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/rest_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/socketio_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/ssn.csv
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/ssn.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/transaction_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/transaction_example_as_library_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/transaction_example_as_library_master.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/transaction_example_as_library_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/tsvreader_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/examples/webdriver_ex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:17.264641 locust-plugins-3.3.0/locust_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 13:19:16.000000 locust-plugins-3.3.0/locust_plugins/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/appinsights_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)    12621 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/connection_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/csvreader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:17.268642 locust-plugins-3.3.0/locust_plugins/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/dashboards/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/dashboards/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/dashboards/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:17.268642 locust-plugins-3.3.0/locust_plugins/dashboards/locust-grafana/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/dashboards/locust-grafana/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/dashboards/locust-grafana/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)      563 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/dashboards/locust-grafana/create_datasource.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/dashboards/locust-grafana/grafana_setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/dashboards/locust-grafana/import_dashboards.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:17.268642 locust-plugins-3.3.0/locust_plugins/dashboards/locust-timescale/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/dashboards/locust-timescale/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/dashboards/locust-timescale/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/dashboards/locust-timescale/timescale_schema.sql
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/dashboards/locust-timescale/zz_hypertable.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:17.272642 locust-plugins-3.3.0/locust_plugins/dashboards/screenshots/
--rw-r--r--   0 runner    (1001) docker     (123)   392198 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/dashboards/screenshots/main_dashboard.png
--rw-r--r--   0 runner    (1001) docker     (123)   425926 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/dashboards/screenshots/main_dashboard_by_request_graphs.png
--rw-r--r--   0 runner    (1001) docker     (123)   267958 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/dashboards/screenshots/requests_table.png
--rw-r--r--   0 runner    (1001) docker     (123)   187305 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/dashboards/screenshots/scatter_plot.png
--rw-r--r--   0 runner    (1001) docker     (123)   372353 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/dashboards/screenshots/testruns.png
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/jmeter_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)    19773 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/listeners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/mongoreader.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/transaction_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:17.272642 locust-plugins-3.3.0/locust_plugins/users/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/users/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/users/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)    15609 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/users/playwright.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/users/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/users/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/users/socketio.py
--rw-r--r--   0 runner    (1001) docker     (123)    13293 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/users/webdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/locust_plugins/wait_time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:17.268642 locust-plugins-3.3.0/locust_plugins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-28 13:19:17.000000 locust-plugins-3.3.0/locust_plugins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-28 13:19:17.000000 locust-plugins-3.3.0/locust_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:19:17.000000 locust-plugins-3.3.0/locust_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:19:17.000000 locust-plugins-3.3.0/locust_plugins.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-28 13:19:17.000000 locust-plugins-3.3.0/locust_plugins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 13:19:17.000000 locust-plugins-3.3.0/locust_plugins.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 13:19:17.272642 locust-plugins-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:19:17.272642 locust-plugins-3.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/test/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/test/test_stuff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-28 13:19:06.000000 locust-plugins-3.3.0/tusk.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:34.697261 locust-plugins-3.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:34.685260 locust-plugins-3.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:34.689261 locust-plugins-3.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:34.689261 locust-plugins-3.3.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-31 08:31:34.697261 locust-plugins-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:34.689261 locust-plugins-3.3.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/bin/locust-compose
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:34.689261 locust-plugins-3.3.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/appinsights_listener_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/cmd_line_examples.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/connection_pool_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/constant_total_ips_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/csvreader_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/embedded_resource_manager_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/jmeter_listener_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/kafka_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/mongoreader_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/mqtt_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/playwright-recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/playwright_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/reschedule_on_fail_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/rest_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/socketio_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/ssn.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/ssn.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/transaction_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/transaction_example_as_library_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/transaction_example_as_library_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/transaction_example_as_library_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/tsvreader_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/examples/webdriver_ex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:34.689261 locust-plugins-3.3.1/locust_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 08:31:34.000000 locust-plugins-3.3.1/locust_plugins/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/appinsights_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12621 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/connection_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/csvreader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:34.693261 locust-plugins-3.3.1/locust_plugins/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/dashboards/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/dashboards/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/dashboards/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:34.693261 locust-plugins-3.3.1/locust_plugins/dashboards/locust-grafana/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/dashboards/locust-grafana/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/dashboards/locust-grafana/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)      563 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/dashboards/locust-grafana/create_datasource.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/dashboards/locust-grafana/grafana_setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/dashboards/locust-grafana/import_dashboards.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:34.693261 locust-plugins-3.3.1/locust_plugins/dashboards/locust-timescale/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/dashboards/locust-timescale/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/dashboards/locust-timescale/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/dashboards/locust-timescale/timescale_schema.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/dashboards/locust-timescale/zz_hypertable.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:34.693261 locust-plugins-3.3.1/locust_plugins/dashboards/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (123)   392198 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/dashboards/screenshots/main_dashboard.png
+-rw-r--r--   0 runner    (1001) docker     (123)   425926 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/dashboards/screenshots/main_dashboard_by_request_graphs.png
+-rw-r--r--   0 runner    (1001) docker     (123)   267958 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/dashboards/screenshots/requests_table.png
+-rw-r--r--   0 runner    (1001) docker     (123)   187305 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/dashboards/screenshots/scatter_plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)   372353 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/dashboards/screenshots/testruns.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/jmeter_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19773 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/mongoreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/transaction_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:34.697261 locust-plugins-3.3.1/locust_plugins/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/users/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/users/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15609 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/users/playwright.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/users/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/users/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/users/socketio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13293 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/users/webdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/locust_plugins/wait_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:34.693261 locust-plugins-3.3.1/locust_plugins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-31 08:31:34.000000 locust-plugins-3.3.1/locust_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-31 08:31:34.000000 locust-plugins-3.3.1/locust_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 08:31:34.000000 locust-plugins-3.3.1/locust_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 08:31:34.000000 locust-plugins-3.3.1/locust_plugins.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-31 08:31:34.000000 locust-plugins-3.3.1/locust_plugins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 08:31:34.000000 locust-plugins-3.3.1/locust_plugins.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 08:31:34.697261 locust-plugins-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:31:34.697261 locust-plugins-3.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/test/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/test/test_stuff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-31 08:31:23.000000 locust-plugins-3.3.1/tusk.yaml
```

### Comparing `locust-plugins-3.3.0/.github/workflows/tests.yml` & `locust-plugins-3.3.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/.pylintrc` & `locust-plugins-3.3.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/.vscode/launch.json` & `locust-plugins-3.3.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/.vscode/settings.json` & `locust-plugins-3.3.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/CONTRIBUTING.md` & `locust-plugins-3.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/LICENSE` & `locust-plugins-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/PKG-INFO` & `locust-plugins-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locust-plugins
-Version: 3.3.0
+Version: 3.3.1
 Summary: Useful plugins/extensions for Locust
 Home-page: https://github.com/SvenskaSpel/locust-plugins
 Author: Lars Holmberg
 License: Apache-2.0
 Classifier: Topic :: Software Development :: Testing :: Traffic Generation
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `locust-plugins-3.3.0/README.md` & `locust-plugins-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/examples/cmd_line_examples.sh` & `locust-plugins-3.3.1/examples/cmd_line_examples.sh`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/examples/connection_pool_ex.py` & `locust-plugins-3.3.1/examples/connection_pool_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/examples/constant_total_ips_ex.py` & `locust-plugins-3.3.1/examples/constant_total_ips_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/examples/embedded_resource_manager_ex.py` & `locust-plugins-3.3.1/examples/embedded_resource_manager_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/examples/kafka_ex.py` & `locust-plugins-3.3.1/examples/kafka_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/examples/mongoreader_ex.py` & `locust-plugins-3.3.1/examples/mongoreader_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/examples/mqtt_ex.py` & `locust-plugins-3.3.1/examples/mqtt_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/examples/playwright-recording.py` & `locust-plugins-3.3.1/examples/playwright-recording.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/examples/playwright_ex.py` & `locust-plugins-3.3.1/examples/playwright_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/examples/reschedule_on_fail_ex.py` & `locust-plugins-3.3.1/examples/reschedule_on_fail_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/examples/rest_ex.py` & `locust-plugins-3.3.1/examples/rest_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/examples/socketio_ex.py` & `locust-plugins-3.3.1/examples/socketio_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/examples/transaction_example.py` & `locust-plugins-3.3.1/examples/transaction_example.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/examples/transaction_example_as_library_local.py` & `locust-plugins-3.3.1/examples/transaction_example_as_library_local.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/examples/transaction_example_as_library_master.py` & `locust-plugins-3.3.1/examples/transaction_example_as_library_master.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/examples/transaction_example_as_library_worker.py` & `locust-plugins-3.3.1/examples/transaction_example_as_library_worker.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/examples/webdriver_ex.py` & `locust-plugins-3.3.1/examples/webdriver_ex.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/__init__.py` & `locust-plugins-3.3.1/locust_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/appinsights_listener.py` & `locust-plugins-3.3.1/locust_plugins/appinsights_listener.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/connection_pools.py` & `locust-plugins-3.3.1/locust_plugins/connection_pools.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/csvreader.py` & `locust-plugins-3.3.1/locust_plugins/csvreader.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/dashboards/README.md` & `locust-plugins-3.3.1/locust_plugins/dashboards/README.md`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/dashboards/docker-compose.yml` & `locust-plugins-3.3.1/locust_plugins/dashboards/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/dashboards/locust-grafana/create_datasource.sh` & `locust-plugins-3.3.1/locust_plugins/dashboards/locust-grafana/create_datasource.sh`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/dashboards/locust-grafana/grafana_setup.sh` & `locust-plugins-3.3.1/locust_plugins/dashboards/locust-grafana/grafana_setup.sh`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/dashboards/locust-grafana/import_dashboards.sh` & `locust-plugins-3.3.1/locust_plugins/dashboards/locust-grafana/import_dashboards.sh`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/dashboards/locust-timescale/timescale_schema.sql` & `locust-plugins-3.3.1/locust_plugins/dashboards/locust-timescale/timescale_schema.sql`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/dashboards/screenshots/main_dashboard.png` & `locust-plugins-3.3.1/locust_plugins/dashboards/screenshots/main_dashboard.png`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/dashboards/screenshots/main_dashboard_by_request_graphs.png` & `locust-plugins-3.3.1/locust_plugins/dashboards/screenshots/main_dashboard_by_request_graphs.png`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/dashboards/screenshots/requests_table.png` & `locust-plugins-3.3.1/locust_plugins/dashboards/screenshots/requests_table.png`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/dashboards/screenshots/scatter_plot.png` & `locust-plugins-3.3.1/locust_plugins/dashboards/screenshots/scatter_plot.png`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/dashboards/screenshots/testruns.png` & `locust-plugins-3.3.1/locust_plugins/dashboards/screenshots/testruns.png`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/jmeter_listener.py` & `locust-plugins-3.3.1/locust_plugins/jmeter_listener.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/listeners.py` & `locust-plugins-3.3.1/locust_plugins/listeners.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/mongoreader.py` & `locust-plugins-3.3.1/locust_plugins/mongoreader.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/transaction_manager.py` & `locust-plugins-3.3.1/locust_plugins/transaction_manager.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/users/kafka.py` & `locust-plugins-3.3.1/locust_plugins/users/kafka.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/users/mqtt.py` & `locust-plugins-3.3.1/locust_plugins/users/mqtt.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/users/playwright.py` & `locust-plugins-3.3.1/locust_plugins/users/playwright.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/users/resource.py` & `locust-plugins-3.3.1/locust_plugins/users/resource.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/users/rest.py` & `locust-plugins-3.3.1/locust_plugins/users/rest.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/users/socketio.py` & `locust-plugins-3.3.1/locust_plugins/users/socketio.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/users/webdriver.py` & `locust-plugins-3.3.1/locust_plugins/users/webdriver.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins/wait_time.py` & `locust-plugins-3.3.1/locust_plugins/wait_time.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/locust_plugins.egg-info/PKG-INFO` & `locust-plugins-3.3.1/locust_plugins.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locust-plugins
-Version: 3.3.0
+Version: 3.3.1
 Summary: Useful plugins/extensions for Locust
 Home-page: https://github.com/SvenskaSpel/locust-plugins
 Author: Lars Holmberg
 License: Apache-2.0
 Classifier: Topic :: Software Development :: Testing :: Traffic Generation
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `locust-plugins-3.3.0/locust_plugins.egg-info/SOURCES.txt` & `locust-plugins-3.3.1/locust_plugins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/setup.py` & `locust-plugins-3.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     packages=find_packages(exclude=["examples"]),
     include_package_data=True,
     package_data={"locust_plugins": ["py.typed"]},
     zip_safe=False,
     install_requires=[
         "playwright",
         "locust>=2.14.0",
+        "playwright>=1.34.0",
         "psycogreen",
         "psycopg2-binary",
         "websocket-client",
         "python-dateutil",
         "pymongo",
         "confluent-kafka",
         "selenium>=4.0.0",
```

### Comparing `locust-plugins-3.3.0/test/test_stuff.py` & `locust-plugins-3.3.1/test/test_stuff.py`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/tox.ini` & `locust-plugins-3.3.1/tox.ini`

 * *Files identical despite different names*

### Comparing `locust-plugins-3.3.0/tusk.yaml` & `locust-plugins-3.3.1/tusk.yaml`

 * *Files identical despite different names*

