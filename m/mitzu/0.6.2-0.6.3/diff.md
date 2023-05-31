# Comparing `tmp/mitzu-0.6.2.tar.gz` & `tmp/mitzu-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitzu-0.6.2.tar", max compression
+gzip compressed data, was "mitzu-0.6.3.tar", max compression
```

## Comparing `mitzu-0.6.2.tar` & `mitzu-0.6.3.tar`

### file list

```diff
@@ -1,136 +1,136 @@
--rw-r--r--   0        0        0     1082 2023-05-31 08:36:53.494480 mitzu-0.6.2/LICENSE.txt
--rw-r--r--   0        0        0     2235 2023-05-31 08:36:53.494480 mitzu-0.6.2/README.md
--rw-r--r--   0        0        0     6148 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/.DS_Store
--rw-r--r--   0        0        0      752 2023-05-31 08:37:47.398121 mitzu-0.6.2/mitzu/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/__init__.py
--rw-r--r--   0        0        0     1918 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/adapter_factory.py
--rw-r--r--   0        0        0     5148 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/athena_adapter.py
--rw-r--r--   0        0        0     6262 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/bigquery_adapter.py
--rw-r--r--   0        0        0     6026 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/databricks_adapter.py
--rw-r--r--   0        0        0     2261 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/file_adapter.py
--rw-r--r--   0        0        0     2533 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/generic_adapter.py
--rw-r--r--   0        0        0      898 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/helper.py
--rw-r--r--   0        0        0     3422 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/mysql_adapter.py
--rw-r--r--   0        0        0     2297 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/postgresql_adapter.py
--rw-r--r--   0        0        0     3765 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/redshift_adapter.py
--rw-r--r--   0        0        0     3298 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/snowflake_adapter.py
--rw-r--r--   0        0        0        0 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/__init__.py
--rw-r--r--   0        0        0      701 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5071 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6415 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
--rw-r--r--   0        0        0     9751 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1844 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
--rw-r--r--   0        0        0        0 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/__init__.py
--rw-r--r--   0        0        0     2146 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2412 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py
--rw-r--r--   0        0        0     5071 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py
--rw-r--r--   0        0        0     4770 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py
--rw-r--r--   0        0        0    38550 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     8638 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py
--rw-r--r--   0        0        0     9854 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py
--rw-r--r--   0        0        0     7361 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py
--rw-r--r--   0        0        0     1131 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py
--rw-r--r--   0        0        0        0 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/__init__.py
--rw-r--r--   0        0        0      713 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5010 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6601 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
--rw-r--r--   0        0        0    10073 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1848 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
--rw-r--r--   0        0        0    40105 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy_adapter.py
--rw-r--r--   0        0        0     4963 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/adapters/sqlite_adapter.py
--rw-r--r--   0        0        0     7705 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/adapters/trino_adapter.py
--rw-r--r--   0        0        0     1835 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/helper.py
--rw-r--r--   0        0        0    53055 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/model.py
--rw-r--r--   0        0        0        0 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/notebook/__init__.py
--rw-r--r--   0        0        0     6845 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/notebook/model_loader.py
--rw-r--r--   0        0        0     2550 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/project_discovery.py
--rw-r--r--   0        0        0     2102 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/project_serialization.py
--rw-r--r--   0        0        0      785 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/samples/__init__.py
--rw-r--r--   0        0        0     3794 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/samples/data_ingestion.py
--rw-r--r--   0        0        0    10141 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/samples/sample_data_generator.py
--rw-r--r--   0        0        0    11933 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/serialization.py
--rw-r--r--   0        0        0        0 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/visualization/__init__.py
--rw-r--r--   0        0        0     7305 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/visualization/charts.py
--rw-r--r--   0        0        0     1866 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/visualization/common.py
--rw-r--r--   0        0        0      941 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/visualization/labels.py
--rw-r--r--   0        0        0     7802 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/visualization/plot.py
--rw-r--r--   0        0        0     5767 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/visualization/titles.py
--rw-r--r--   0        0        0     3181 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/visualization/tooltips.py
--rw-r--r--   0        0        0     3289 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/visualization/transform_conv.py
--rw-r--r--   0        0        0     1222 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/visualization/transform_retention.py
--rw-r--r--   0        0        0     6148 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/__init__.py
--rw-r--r--   0        0        0     5347 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/explore_page.css
--rw-r--r--   0        0        0   147145 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/favicon.ico
--rw-r--r--   0        0        0    46702 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/logo.png
--rw-r--r--   0        0        0    43472 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/mitzu-logo-light.svg
--rw-r--r--   0        0        0    49422 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/athena.png
--rw-r--r--   0        0        0    20802 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/bigquery.png
--rw-r--r--   0        0        0    10321 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/clickhouse.png
--rw-r--r--   0        0        0   119554 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/databricks.png
--rw-r--r--   0        0        0     3008 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/mysql.png
--rw-r--r--   0        0        0     2446 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/pandas.png
--rw-r--r--   0        0        0     5338 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/postgresql.png
--rw-r--r--   0        0        0     8512 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/redshift.png
--rw-r--r--   0        0        0    93500 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/snowflake.png
--rw-r--r--   0        0        0    48681 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/sqlite.png
--rw-r--r--   0        0        0    34219 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/trino.png
--rw-r--r--   0        0        0    15538 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/auth/authorizer.py
--rw-r--r--   0        0        0     3557 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/auth/cognito.py
--rw-r--r--   0        0        0     1305 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/auth/decorator.py
--rw-r--r--   0        0        0     2777 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/auth/google.py
--rw-r--r--   0        0        0     7481 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/cache.py
--rw-r--r--   0        0        0     2920 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/caching_dataset_adapter.py
--rw-r--r--   0        0        0     1664 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/configs.py
--rw-r--r--   0        0        0     3432 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/dependencies.py
--rw-r--r--   0        0        0     4984 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/helper.py
--rw-r--r--   0        0        0     8631 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/model.py
--rw-r--r--   0        0        0      309 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/navbar.py
--rw-r--r--   0        0        0     5435 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/offcanvas.py
--rw-r--r--   0        0        0        0 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/connections/__init__.py
--rw-r--r--   0        0        0    22704 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/connections/manage_connections_component.py
--rw-r--r--   0        0        0     4428 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/connections_page.py
--rw-r--r--   0        0        0        0 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/dashboards/__init__.py
--rw-r--r--   0        0        0    20561 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
--rw-r--r--   0        0        0     9628 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/dashboards_page.py
--rw-r--r--   0        0        0    14456 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/edit_user.py
--rw-r--r--   0        0        0        0 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/__init__.py
--rw-r--r--   0        0        0     5738 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/complex_segment_handler.py
--rw-r--r--   0        0        0     6488 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/dates_selector_handler.py
--rw-r--r--   0        0        0     5564 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/event_segment_handler.py
--rw-r--r--   0        0        0    21704 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/explore_page.py
--rw-r--r--   0        0        0    10100 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/graph_handler.py
--rw-r--r--   0        0        0    10940 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/metric_config_handler.py
--rw-r--r--   0        0        0     2375 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/metric_segments_handler.py
--rw-r--r--   0        0        0     1565 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/metric_type_handler.py
--rw-r--r--   0        0        0     9772 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/simple_segment_handler.py
--rw-r--r--   0        0        0     4644 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/toolbar_handler.py
--rw-r--r--   0        0        0     1221 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore_project.py
--rw-r--r--   0        0        0     1751 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/home.py
--rw-r--r--   0        0        0     3947 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/login.py
--rw-r--r--   0        0        0     5023 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/manage_connection.py
--rw-r--r--   0        0        0     1288 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/manage_dashboard.py
--rw-r--r--   0        0        0    10095 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/manage_event_defs.py
--rw-r--r--   0        0        0    11845 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/manage_project.py
--rw-r--r--   0        0        0     9470 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/manage_saved_metrics.py
--rw-r--r--   0        0        0     1738 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/paths.py
--rw-r--r--   0        0        0        0 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/projects/__init__.py
--rw-r--r--   0        0        0    35694 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/projects/event_tables_config.py
--rw-r--r--   0        0        0      587 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/projects/helper.py
--rw-r--r--   0        0        0     9400 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/projects/manage_project_component.py
--rw-r--r--   0        0        0     5090 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/projects_page.py
--rw-r--r--   0        0        0     3114 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/users.py
--rw-r--r--   0        0        0        0 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/service/__init__.py
--rw-r--r--   0        0        0     1919 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/service/events_service.py
--rw-r--r--   0        0        0     4974 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/service/navbar_service.py
--rw-r--r--   0        0        0      670 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/service/notification_service.py
--rw-r--r--   0        0        0     2105 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/service/secret_service.py
--rw-r--r--   0        0        0     6650 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/service/tracking_service.py
--rw-r--r--   0        0        0     4719 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/service/user_service.py
--rw-r--r--   0        0        0    24085 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/storage.py
--rw-r--r--   0        0        0    25095 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/storage_model.py
--rw-r--r--   0        0        0     4700 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/webapp.py
--rw-r--r--   0        0        0     3422 2023-05-31 08:37:47.398121 mitzu-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 mitzu-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-31 12:07:13.017261 mitzu-0.6.3/LICENSE.txt
+-rw-r--r--   0        0        0     2235 2023-05-31 12:07:13.017261 mitzu-0.6.3/README.md
+-rw-r--r--   0        0        0     6148 2023-05-31 12:07:13.409266 mitzu-0.6.3/mitzu/.DS_Store
+-rw-r--r--   0        0        0      752 2023-05-31 12:08:07.509981 mitzu-0.6.3/mitzu/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:07:13.409266 mitzu-0.6.3/mitzu/adapters/__init__.py
+-rw-r--r--   0        0        0     1918 2023-05-31 12:07:13.409266 mitzu-0.6.3/mitzu/adapters/adapter_factory.py
+-rw-r--r--   0        0        0     5148 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/athena_adapter.py
+-rw-r--r--   0        0        0     6262 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/bigquery_adapter.py
+-rw-r--r--   0        0        0     6026 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/databricks_adapter.py
+-rw-r--r--   0        0        0     2261 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/file_adapter.py
+-rw-r--r--   0        0        0     2533 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/generic_adapter.py
+-rw-r--r--   0        0        0      898 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/helper.py
+-rw-r--r--   0        0        0     3422 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/mysql_adapter.py
+-rw-r--r--   0        0        0     2297 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/postgresql_adapter.py
+-rw-r--r--   0        0        0     3765 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/redshift_adapter.py
+-rw-r--r--   0        0        0     3298 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/snowflake_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/__init__.py
+-rw-r--r--   0        0        0      701 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5071 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6415 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0     9751 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1844 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/__init__.py
+-rw-r--r--   0        0        0     2146 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2412 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py
+-rw-r--r--   0        0        0     5071 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py
+-rw-r--r--   0        0        0     4770 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py
+-rw-r--r--   0        0        0    38550 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     8638 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py
+-rw-r--r--   0        0        0     9854 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py
+-rw-r--r--   0        0        0     7361 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0     1131 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/__init__.py
+-rw-r--r--   0        0        0      713 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5010 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6601 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0    10073 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1848 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
+-rw-r--r--   0        0        0    40105 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlalchemy_adapter.py
+-rw-r--r--   0        0        0     4963 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/sqlite_adapter.py
+-rw-r--r--   0        0        0     7705 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/adapters/trino_adapter.py
+-rw-r--r--   0        0        0     1835 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/helper.py
+-rw-r--r--   0        0        0    53055 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/model.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/notebook/__init__.py
+-rw-r--r--   0        0        0     6845 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/notebook/model_loader.py
+-rw-r--r--   0        0        0     2550 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/project_discovery.py
+-rw-r--r--   0        0        0     2102 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/project_serialization.py
+-rw-r--r--   0        0        0      785 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/samples/__init__.py
+-rw-r--r--   0        0        0     3794 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/samples/data_ingestion.py
+-rw-r--r--   0        0        0    10141 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/samples/sample_data_generator.py
+-rw-r--r--   0        0        0    11933 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/serialization.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/visualization/__init__.py
+-rw-r--r--   0        0        0     7305 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/visualization/charts.py
+-rw-r--r--   0        0        0     1866 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/visualization/common.py
+-rw-r--r--   0        0        0      941 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/visualization/labels.py
+-rw-r--r--   0        0        0     7802 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/visualization/plot.py
+-rw-r--r--   0        0        0     5767 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/visualization/titles.py
+-rw-r--r--   0        0        0     3181 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/visualization/tooltips.py
+-rw-r--r--   0        0        0     3289 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/visualization/transform_conv.py
+-rw-r--r--   0        0        0     1222 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/visualization/transform_retention.py
+-rw-r--r--   0        0        0     6148 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/webapp/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/webapp/__init__.py
+-rw-r--r--   0        0        0     5347 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/webapp/assets/explore_page.css
+-rw-r--r--   0        0        0   147145 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/webapp/assets/favicon.ico
+-rw-r--r--   0        0        0    46702 2023-05-31 12:07:13.413266 mitzu-0.6.3/mitzu/webapp/assets/logo.png
+-rw-r--r--   0        0        0    43472 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/mitzu-logo-light.svg
+-rw-r--r--   0        0        0    49422 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/athena.png
+-rw-r--r--   0        0        0    20802 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/bigquery.png
+-rw-r--r--   0        0        0    10321 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/clickhouse.png
+-rw-r--r--   0        0        0   119554 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/databricks.png
+-rw-r--r--   0        0        0     3008 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/mysql.png
+-rw-r--r--   0        0        0     2446 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/pandas.png
+-rw-r--r--   0        0        0     5338 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/postgresql.png
+-rw-r--r--   0        0        0     8512 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/redshift.png
+-rw-r--r--   0        0        0    93500 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/snowflake.png
+-rw-r--r--   0        0        0    48681 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/sqlite.png
+-rw-r--r--   0        0        0    34219 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/assets/warehouse/trino.png
+-rw-r--r--   0        0        0    15538 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/auth/authorizer.py
+-rw-r--r--   0        0        0     3557 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/auth/cognito.py
+-rw-r--r--   0        0        0     1305 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/auth/decorator.py
+-rw-r--r--   0        0        0     2777 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/auth/google.py
+-rw-r--r--   0        0        0     7481 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/cache.py
+-rw-r--r--   0        0        0     2920 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/caching_dataset_adapter.py
+-rw-r--r--   0        0        0     1664 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/configs.py
+-rw-r--r--   0        0        0     3432 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/dependencies.py
+-rw-r--r--   0        0        0     4984 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/helper.py
+-rw-r--r--   0        0        0     8631 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/model.py
+-rw-r--r--   0        0        0      309 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/navbar.py
+-rw-r--r--   0        0        0     5435 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/offcanvas.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/connections/__init__.py
+-rw-r--r--   0        0        0    22704 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/connections/manage_connections_component.py
+-rw-r--r--   0        0        0     4428 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/connections_page.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/dashboards/__init__.py
+-rw-r--r--   0        0        0    20561 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
+-rw-r--r--   0        0        0     9628 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/dashboards_page.py
+-rw-r--r--   0        0        0    14456 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/edit_user.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/__init__.py
+-rw-r--r--   0        0        0     5738 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/complex_segment_handler.py
+-rw-r--r--   0        0        0     6488 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/dates_selector_handler.py
+-rw-r--r--   0        0        0     5564 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/event_segment_handler.py
+-rw-r--r--   0        0        0    21704 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/explore_page.py
+-rw-r--r--   0        0        0    10100 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/graph_handler.py
+-rw-r--r--   0        0        0    10940 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/metric_config_handler.py
+-rw-r--r--   0        0        0     2375 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/metric_segments_handler.py
+-rw-r--r--   0        0        0     1565 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/metric_type_handler.py
+-rw-r--r--   0        0        0     9772 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/simple_segment_handler.py
+-rw-r--r--   0        0        0     4644 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore/toolbar_handler.py
+-rw-r--r--   0        0        0     1221 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/explore_project.py
+-rw-r--r--   0        0        0     1751 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/home.py
+-rw-r--r--   0        0        0     3947 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/login.py
+-rw-r--r--   0        0        0     5023 2023-05-31 12:07:13.417266 mitzu-0.6.3/mitzu/webapp/pages/manage_connection.py
+-rw-r--r--   0        0        0     1288 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/manage_dashboard.py
+-rw-r--r--   0        0        0    10095 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/manage_event_defs.py
+-rw-r--r--   0        0        0    11845 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/manage_project.py
+-rw-r--r--   0        0        0     9470 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/manage_saved_metrics.py
+-rw-r--r--   0        0        0     1738 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/paths.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/projects/__init__.py
+-rw-r--r--   0        0        0    35694 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/projects/event_tables_config.py
+-rw-r--r--   0        0        0      587 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/projects/helper.py
+-rw-r--r--   0        0        0     9400 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/projects/manage_project_component.py
+-rw-r--r--   0        0        0     5090 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/projects_page.py
+-rw-r--r--   0        0        0     3114 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/pages/users.py
+-rw-r--r--   0        0        0        0 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/service/__init__.py
+-rw-r--r--   0        0        0     1955 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/service/events_service.py
+-rw-r--r--   0        0        0     4974 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/service/navbar_service.py
+-rw-r--r--   0        0        0      670 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/service/notification_service.py
+-rw-r--r--   0        0        0     2105 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/service/secret_service.py
+-rw-r--r--   0        0        0     6650 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/service/tracking_service.py
+-rw-r--r--   0        0        0     4755 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/service/user_service.py
+-rw-r--r--   0        0        0    24085 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/storage.py
+-rw-r--r--   0        0        0    25095 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/storage_model.py
+-rw-r--r--   0        0        0     4700 2023-05-31 12:07:13.421266 mitzu-0.6.3/mitzu/webapp/webapp.py
+-rw-r--r--   0        0        0     3422 2023-05-31 12:08:07.509981 mitzu-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 mitzu-0.6.3/PKG-INFO
```

### Comparing `mitzu-0.6.2/LICENSE.txt` & `mitzu-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/README.md` & `mitzu-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/.DS_Store` & `mitzu-0.6.3/mitzu/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/__init__.py` & `mitzu-0.6.3/mitzu/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     TimeWindow,
     TimeGroup,
     DiscoverySettings,
     WebappSettings,
 )
 from mitzu.samples import get_sample_discovered_project
 
-__version__ = "0.6.2"
+__version__ = "0.6.3"
 
 
 __all__ = [
     "Connection",
     "ConnectionType",
     "Project",
     "EventDataTable",
```

### Comparing `mitzu-0.6.2/mitzu/adapters/adapter_factory.py` & `mitzu-0.6.3/mitzu/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/athena_adapter.py` & `mitzu-0.6.3/mitzu/adapters/athena_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/bigquery_adapter.py` & `mitzu-0.6.3/mitzu/adapters/bigquery_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/databricks_adapter.py` & `mitzu-0.6.3/mitzu/adapters/databricks_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/file_adapter.py` & `mitzu-0.6.3/mitzu/adapters/file_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/generic_adapter.py` & `mitzu-0.6.3/mitzu/adapters/generic_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/helper.py` & `mitzu-0.6.3/mitzu/adapters/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/mysql_adapter.py` & `mitzu-0.6.3/mitzu/adapters/mysql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/postgresql_adapter.py` & `mitzu-0.6.3/mitzu/adapters/postgresql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/redshift_adapter.py` & `mitzu-0.6.3/mitzu/adapters/redshift_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/snowflake_adapter.py` & `mitzu-0.6.3/mitzu/adapters/snowflake_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlalchemy_adapter.py` & `mitzu-0.6.3/mitzu/adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/sqlite_adapter.py` & `mitzu-0.6.3/mitzu/adapters/sqlite_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/adapters/trino_adapter.py` & `mitzu-0.6.3/mitzu/adapters/trino_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/helper.py` & `mitzu-0.6.3/mitzu/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/model.py` & `mitzu-0.6.3/mitzu/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/notebook/model_loader.py` & `mitzu-0.6.3/mitzu/notebook/model_loader.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/project_discovery.py` & `mitzu-0.6.3/mitzu/project_discovery.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/project_serialization.py` & `mitzu-0.6.3/mitzu/project_serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/samples/__init__.py` & `mitzu-0.6.3/mitzu/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/samples/data_ingestion.py` & `mitzu-0.6.3/mitzu/samples/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/samples/sample_data_generator.py` & `mitzu-0.6.3/mitzu/samples/sample_data_generator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/serialization.py` & `mitzu-0.6.3/mitzu/serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/visualization/charts.py` & `mitzu-0.6.3/mitzu/visualization/charts.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/visualization/common.py` & `mitzu-0.6.3/mitzu/visualization/common.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/visualization/labels.py` & `mitzu-0.6.3/mitzu/visualization/labels.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/visualization/plot.py` & `mitzu-0.6.3/mitzu/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/visualization/titles.py` & `mitzu-0.6.3/mitzu/visualization/titles.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/visualization/tooltips.py` & `mitzu-0.6.3/mitzu/visualization/tooltips.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/visualization/transform_conv.py` & `mitzu-0.6.3/mitzu/visualization/transform_conv.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/visualization/transform_retention.py` & `mitzu-0.6.3/mitzu/visualization/transform_retention.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/.DS_Store` & `mitzu-0.6.3/mitzu/webapp/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/assets/explore_page.css` & `mitzu-0.6.3/mitzu/webapp/assets/explore_page.css`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/assets/favicon.ico` & `mitzu-0.6.3/mitzu/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/assets/logo.png` & `mitzu-0.6.3/mitzu/webapp/assets/logo.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/assets/mitzu-logo-light.svg` & `mitzu-0.6.3/mitzu/webapp/assets/mitzu-logo-light.svg`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/assets/warehouse/athena.png` & `mitzu-0.6.3/mitzu/webapp/assets/warehouse/athena.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/assets/warehouse/bigquery.png` & `mitzu-0.6.3/mitzu/webapp/assets/warehouse/bigquery.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/assets/warehouse/clickhouse.png` & `mitzu-0.6.3/mitzu/webapp/assets/warehouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/assets/warehouse/databricks.png` & `mitzu-0.6.3/mitzu/webapp/assets/warehouse/databricks.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/assets/warehouse/mysql.png` & `mitzu-0.6.3/mitzu/webapp/assets/warehouse/mysql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/assets/warehouse/pandas.png` & `mitzu-0.6.3/mitzu/webapp/assets/warehouse/pandas.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/assets/warehouse/postgresql.png` & `mitzu-0.6.3/mitzu/webapp/assets/warehouse/postgresql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/assets/warehouse/redshift.png` & `mitzu-0.6.3/mitzu/webapp/assets/warehouse/redshift.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/assets/warehouse/snowflake.png` & `mitzu-0.6.3/mitzu/webapp/assets/warehouse/snowflake.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/assets/warehouse/sqlite.png` & `mitzu-0.6.3/mitzu/webapp/assets/warehouse/sqlite.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/assets/warehouse/trino.png` & `mitzu-0.6.3/mitzu/webapp/assets/warehouse/trino.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/auth/authorizer.py` & `mitzu-0.6.3/mitzu/webapp/auth/authorizer.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/auth/cognito.py` & `mitzu-0.6.3/mitzu/webapp/auth/cognito.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/auth/decorator.py` & `mitzu-0.6.3/mitzu/webapp/auth/decorator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/auth/google.py` & `mitzu-0.6.3/mitzu/webapp/auth/google.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/cache.py` & `mitzu-0.6.3/mitzu/webapp/cache.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/caching_dataset_adapter.py` & `mitzu-0.6.3/mitzu/webapp/caching_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/configs.py` & `mitzu-0.6.3/mitzu/webapp/configs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/dependencies.py` & `mitzu-0.6.3/mitzu/webapp/dependencies.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/helper.py` & `mitzu-0.6.3/mitzu/webapp/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/model.py` & `mitzu-0.6.3/mitzu/webapp/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/offcanvas.py` & `mitzu-0.6.3/mitzu/webapp/offcanvas.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/connections/manage_connections_component.py` & `mitzu-0.6.3/mitzu/webapp/pages/connections/manage_connections_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/connections_page.py` & `mitzu-0.6.3/mitzu/webapp/pages/connections_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/dashboards/manage_dashboards_component.py` & `mitzu-0.6.3/mitzu/webapp/pages/dashboards/manage_dashboards_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/dashboards_page.py` & `mitzu-0.6.3/mitzu/webapp/pages/dashboards_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/edit_user.py` & `mitzu-0.6.3/mitzu/webapp/pages/edit_user.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/explore/complex_segment_handler.py` & `mitzu-0.6.3/mitzu/webapp/pages/explore/complex_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/explore/dates_selector_handler.py` & `mitzu-0.6.3/mitzu/webapp/pages/explore/dates_selector_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/explore/event_segment_handler.py` & `mitzu-0.6.3/mitzu/webapp/pages/explore/event_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/explore/explore_page.py` & `mitzu-0.6.3/mitzu/webapp/pages/explore/explore_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/explore/graph_handler.py` & `mitzu-0.6.3/mitzu/webapp/pages/explore/graph_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/explore/metric_config_handler.py` & `mitzu-0.6.3/mitzu/webapp/pages/explore/metric_config_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/explore/metric_segments_handler.py` & `mitzu-0.6.3/mitzu/webapp/pages/explore/metric_segments_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/explore/metric_type_handler.py` & `mitzu-0.6.3/mitzu/webapp/pages/explore/metric_type_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/explore/simple_segment_handler.py` & `mitzu-0.6.3/mitzu/webapp/pages/explore/simple_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/explore/toolbar_handler.py` & `mitzu-0.6.3/mitzu/webapp/pages/explore/toolbar_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/explore_project.py` & `mitzu-0.6.3/mitzu/webapp/pages/explore_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/home.py` & `mitzu-0.6.3/mitzu/webapp/pages/home.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/login.py` & `mitzu-0.6.3/mitzu/webapp/pages/login.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/manage_connection.py` & `mitzu-0.6.3/mitzu/webapp/pages/manage_connection.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/manage_dashboard.py` & `mitzu-0.6.3/mitzu/webapp/pages/manage_dashboard.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/manage_event_defs.py` & `mitzu-0.6.3/mitzu/webapp/pages/manage_event_defs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/manage_project.py` & `mitzu-0.6.3/mitzu/webapp/pages/manage_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/manage_saved_metrics.py` & `mitzu-0.6.3/mitzu/webapp/pages/manage_saved_metrics.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/paths.py` & `mitzu-0.6.3/mitzu/webapp/pages/paths.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/projects/event_tables_config.py` & `mitzu-0.6.3/mitzu/webapp/pages/projects/event_tables_config.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/projects/helper.py` & `mitzu-0.6.3/mitzu/webapp/pages/projects/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/projects/manage_project_component.py` & `mitzu-0.6.3/mitzu/webapp/pages/projects/manage_project_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/projects_page.py` & `mitzu-0.6.3/mitzu/webapp/pages/projects_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/pages/users.py` & `mitzu-0.6.3/mitzu/webapp/pages/users.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/service/events_service.py` & `mitzu-0.6.3/mitzu/webapp/service/events_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
 import mitzu.webapp.storage as S
 from typing import Callable, Dict, Optional
 import mitzu.model as M
 
 
 class EventServiceException(Exception):
```

### Comparing `mitzu-0.6.2/mitzu/webapp/service/navbar_service.py` & `mitzu-0.6.3/mitzu/webapp/service/navbar_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/service/notification_service.py` & `mitzu-0.6.3/mitzu/webapp/service/notification_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/service/secret_service.py` & `mitzu-0.6.3/mitzu/webapp/service/secret_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/service/tracking_service.py` & `mitzu-0.6.3/mitzu/webapp/service/tracking_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/service/user_service.py` & `mitzu-0.6.3/mitzu/webapp/service/user_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import List, Optional, Tuple
 import random
 import string
 import hashlib
 import mitzu.webapp.storage as S
 import mitzu.webapp.model as WM
 import mitzu.webapp.service.notification_service as NS
```

### Comparing `mitzu-0.6.2/mitzu/webapp/storage.py` & `mitzu-0.6.3/mitzu/webapp/storage.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/storage_model.py` & `mitzu-0.6.3/mitzu/webapp/storage_model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/mitzu/webapp/webapp.py` & `mitzu-0.6.3/mitzu/webapp/webapp.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.2/pyproject.toml` & `mitzu-0.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mitzu"
-version = "0.6.2"
+version = "0.6.3"
 description = "Product analytics over your data warehouse"
 authors = ["Istvan Meszaros <istvan.meszaros.88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mitzu.io"
 repository = "https://github.com/mitzu-io/mitzu"
 documentation = "https://mitzu.io/documentation/"
```

### Comparing `mitzu-0.6.2/PKG-INFO` & `mitzu-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitzu
-Version: 0.6.2
+Version: 0.6.3
 Summary: Product analytics over your data warehouse
 Home-page: https://mitzu.io
 License: MIT
 Author: Istvan Meszaros
 Author-email: istvan.meszaros.88@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

