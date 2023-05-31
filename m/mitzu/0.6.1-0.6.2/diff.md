# Comparing `tmp/mitzu-0.6.1.tar.gz` & `tmp/mitzu-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitzu-0.6.1.tar", max compression
+gzip compressed data, was "mitzu-0.6.2.tar", max compression
```

## Comparing `mitzu-0.6.1.tar` & `mitzu-0.6.2.tar`

### file list

```diff
@@ -1,136 +1,136 @@
--rw-r--r--   0        0        0     1082 2023-05-29 11:48:37.423694 mitzu-0.6.1/LICENSE.txt
--rw-r--r--   0        0        0     2235 2023-05-29 11:48:37.423694 mitzu-0.6.1/README.md
--rw-r--r--   0        0        0     6148 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/.DS_Store
--rw-r--r--   0        0        0      860 2023-05-29 11:50:04.368327 mitzu-0.6.1/mitzu/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/__init__.py
--rw-r--r--   0        0        0     1918 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/adapter_factory.py
--rw-r--r--   0        0        0     5148 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/athena_adapter.py
--rw-r--r--   0        0        0     6262 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/bigquery_adapter.py
--rw-r--r--   0        0        0     6026 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/databricks_adapter.py
--rw-r--r--   0        0        0     2261 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/file_adapter.py
--rw-r--r--   0        0        0     2533 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/generic_adapter.py
--rw-r--r--   0        0        0      898 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/helper.py
--rw-r--r--   0        0        0     3422 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/mysql_adapter.py
--rw-r--r--   0        0        0     2297 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/postgresql_adapter.py
--rw-r--r--   0        0        0     3765 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/redshift_adapter.py
--rw-r--r--   0        0        0     3298 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/snowflake_adapter.py
--rw-r--r--   0        0        0        0 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/__init__.py
--rw-r--r--   0        0        0      701 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5071 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6415 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
--rw-r--r--   0        0        0     9751 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1844 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
--rw-r--r--   0        0        0        0 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/__init__.py
--rw-r--r--   0        0        0     2146 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2412 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py
--rw-r--r--   0        0        0     5071 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py
--rw-r--r--   0        0        0     4770 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py
--rw-r--r--   0        0        0    38550 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     8638 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py
--rw-r--r--   0        0        0     9854 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py
--rw-r--r--   0        0        0     7361 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py
--rw-r--r--   0        0        0     1131 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py
--rw-r--r--   0        0        0        0 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/__init__.py
--rw-r--r--   0        0        0      713 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5010 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6601 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
--rw-r--r--   0        0        0    10073 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1848 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
--rw-r--r--   0        0        0    40105 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlalchemy_adapter.py
--rw-r--r--   0        0        0     4963 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/sqlite_adapter.py
--rw-r--r--   0        0        0     7705 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/adapters/trino_adapter.py
--rw-r--r--   0        0        0     1835 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/helper.py
--rw-r--r--   0        0        0    53991 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/model.py
--rw-r--r--   0        0        0        0 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/notebook/__init__.py
--rw-r--r--   0        0        0     6845 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/notebook/model_loader.py
--rw-r--r--   0        0        0     2550 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/project_discovery.py
--rw-r--r--   0        0        0     2102 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/project_serialization.py
--rw-r--r--   0        0        0      785 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/samples/__init__.py
--rw-r--r--   0        0        0     3794 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/samples/data_ingestion.py
--rw-r--r--   0        0        0    10141 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/samples/sample_data_generator.py
--rw-r--r--   0        0        0    11933 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/serialization.py
--rw-r--r--   0        0        0        0 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/visualization/__init__.py
--rw-r--r--   0        0        0     7305 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/visualization/charts.py
--rw-r--r--   0        0        0     1866 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/visualization/common.py
--rw-r--r--   0        0        0      941 2023-05-29 11:48:37.851695 mitzu-0.6.1/mitzu/visualization/labels.py
--rw-r--r--   0        0        0     7802 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/visualization/plot.py
--rw-r--r--   0        0        0     5767 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/visualization/titles.py
--rw-r--r--   0        0        0     3181 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/visualization/tooltips.py
--rw-r--r--   0        0        0     3289 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/visualization/transform_conv.py
--rw-r--r--   0        0        0     1222 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/visualization/transform_retention.py
--rw-r--r--   0        0        0     6148 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/__init__.py
--rw-r--r--   0        0        0     5347 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/explore_page.css
--rw-r--r--   0        0        0   147145 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/favicon.ico
--rw-r--r--   0        0        0    46702 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/logo.png
--rw-r--r--   0        0        0    43472 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/mitzu-logo-light.svg
--rw-r--r--   0        0        0    49422 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/athena.png
--rw-r--r--   0        0        0    20802 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/bigquery.png
--rw-r--r--   0        0        0    10321 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/clickhouse.png
--rw-r--r--   0        0        0   119554 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/databricks.png
--rw-r--r--   0        0        0     3008 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/mysql.png
--rw-r--r--   0        0        0     2446 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/pandas.png
--rw-r--r--   0        0        0     5338 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/postgresql.png
--rw-r--r--   0        0        0     8512 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/redshift.png
--rw-r--r--   0        0        0    93500 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/snowflake.png
--rw-r--r--   0        0        0    48681 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/sqlite.png
--rw-r--r--   0        0        0    34219 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/assets/warehouse/trino.png
--rw-r--r--   0        0        0    15436 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/auth/authorizer.py
--rw-r--r--   0        0        0     3557 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/auth/cognito.py
--rw-r--r--   0        0        0     1305 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/auth/decorator.py
--rw-r--r--   0        0        0     2777 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/auth/google.py
--rw-r--r--   0        0        0     7481 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/cache.py
--rw-r--r--   0        0        0     2920 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/caching_dataset_adapter.py
--rw-r--r--   0        0        0     1664 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/configs.py
--rw-r--r--   0        0        0     3432 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/dependencies.py
--rw-r--r--   0        0        0     4984 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/helper.py
--rw-r--r--   0        0        0     8375 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/model.py
--rw-r--r--   0        0        0      309 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/navbar.py
--rw-r--r--   0        0        0     5435 2023-05-29 11:48:37.855695 mitzu-0.6.1/mitzu/webapp/offcanvas.py
--rw-r--r--   0        0        0        0 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/connections/__init__.py
--rw-r--r--   0        0        0    22633 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/connections/manage_connections_component.py
--rw-r--r--   0        0        0     4428 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/connections_page.py
--rw-r--r--   0        0        0        0 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/dashboards/__init__.py
--rw-r--r--   0        0        0    20561 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
--rw-r--r--   0        0        0     9628 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/dashboards_page.py
--rw-r--r--   0        0        0    14456 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/edit_user.py
--rw-r--r--   0        0        0        0 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/__init__.py
--rw-r--r--   0        0        0     5738 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/complex_segment_handler.py
--rw-r--r--   0        0        0     6488 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/dates_selector_handler.py
--rw-r--r--   0        0        0     5564 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/event_segment_handler.py
--rw-r--r--   0        0        0    21704 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/explore_page.py
--rw-r--r--   0        0        0    10100 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/graph_handler.py
--rw-r--r--   0        0        0    10940 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/metric_config_handler.py
--rw-r--r--   0        0        0     2375 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/metric_segments_handler.py
--rw-r--r--   0        0        0     1565 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/metric_type_handler.py
--rw-r--r--   0        0        0     9772 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/simple_segment_handler.py
--rw-r--r--   0        0        0     4644 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore/toolbar_handler.py
--rw-r--r--   0        0        0     1221 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/explore_project.py
--rw-r--r--   0        0        0     1751 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/home.py
--rw-r--r--   0        0        0     3947 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/login.py
--rw-r--r--   0        0        0     5023 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/manage_connection.py
--rw-r--r--   0        0        0     1288 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/manage_dashboard.py
--rw-r--r--   0        0        0    10104 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/manage_event_defs.py
--rw-r--r--   0        0        0    11845 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/manage_project.py
--rw-r--r--   0        0        0     9470 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/manage_saved_metrics.py
--rw-r--r--   0        0        0     1738 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/paths.py
--rw-r--r--   0        0        0        0 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/projects/__init__.py
--rw-r--r--   0        0        0    35694 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/projects/event_tables_config.py
--rw-r--r--   0        0        0      587 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/projects/helper.py
--rw-r--r--   0        0        0     9400 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/projects/manage_project_component.py
--rw-r--r--   0        0        0     5075 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/projects_page.py
--rw-r--r--   0        0        0     3114 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/pages/users.py
--rw-r--r--   0        0        0        0 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/service/__init__.py
--rw-r--r--   0        0        0     2156 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/service/events_service.py
--rw-r--r--   0        0        0     5064 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/service/navbar_service.py
--rw-r--r--   0        0        0      670 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/service/notification_service.py
--rw-r--r--   0        0        0     2105 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/service/secret_service.py
--rw-r--r--   0        0        0     6650 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/service/tracking_service.py
--rw-r--r--   0        0        0     4719 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/service/user_service.py
--rw-r--r--   0        0        0    23895 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/storage.py
--rw-r--r--   0        0        0    25760 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/storage_model.py
--rw-r--r--   0        0        0     4700 2023-05-29 11:48:37.859695 mitzu-0.6.1/mitzu/webapp/webapp.py
--rw-r--r--   0        0        0     3422 2023-05-29 11:50:04.364327 mitzu-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 mitzu-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-31 08:36:53.494480 mitzu-0.6.2/LICENSE.txt
+-rw-r--r--   0        0        0     2235 2023-05-31 08:36:53.494480 mitzu-0.6.2/README.md
+-rw-r--r--   0        0        0     6148 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/.DS_Store
+-rw-r--r--   0        0        0      752 2023-05-31 08:37:47.398121 mitzu-0.6.2/mitzu/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/__init__.py
+-rw-r--r--   0        0        0     1918 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/adapter_factory.py
+-rw-r--r--   0        0        0     5148 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/athena_adapter.py
+-rw-r--r--   0        0        0     6262 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/bigquery_adapter.py
+-rw-r--r--   0        0        0     6026 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/databricks_adapter.py
+-rw-r--r--   0        0        0     2261 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/file_adapter.py
+-rw-r--r--   0        0        0     2533 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/generic_adapter.py
+-rw-r--r--   0        0        0      898 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/helper.py
+-rw-r--r--   0        0        0     3422 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/mysql_adapter.py
+-rw-r--r--   0        0        0     2297 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/postgresql_adapter.py
+-rw-r--r--   0        0        0     3765 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/redshift_adapter.py
+-rw-r--r--   0        0        0     3298 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/snowflake_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/__init__.py
+-rw-r--r--   0        0        0      701 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5071 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6415 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0     9751 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1844 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/__init__.py
+-rw-r--r--   0        0        0     2146 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2412 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py
+-rw-r--r--   0        0        0     5071 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py
+-rw-r--r--   0        0        0     4770 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py
+-rw-r--r--   0        0        0    38550 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     8638 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py
+-rw-r--r--   0        0        0     9854 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py
+-rw-r--r--   0        0        0     7361 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0     1131 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/__init__.py
+-rw-r--r--   0        0        0      713 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5010 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6601 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0    10073 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1848 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
+-rw-r--r--   0        0        0    40105 2023-05-31 08:36:53.922470 mitzu-0.6.2/mitzu/adapters/sqlalchemy_adapter.py
+-rw-r--r--   0        0        0     4963 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/adapters/sqlite_adapter.py
+-rw-r--r--   0        0        0     7705 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/adapters/trino_adapter.py
+-rw-r--r--   0        0        0     1835 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/helper.py
+-rw-r--r--   0        0        0    53055 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/model.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/notebook/__init__.py
+-rw-r--r--   0        0        0     6845 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/notebook/model_loader.py
+-rw-r--r--   0        0        0     2550 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/project_discovery.py
+-rw-r--r--   0        0        0     2102 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/project_serialization.py
+-rw-r--r--   0        0        0      785 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/samples/__init__.py
+-rw-r--r--   0        0        0     3794 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/samples/data_ingestion.py
+-rw-r--r--   0        0        0    10141 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/samples/sample_data_generator.py
+-rw-r--r--   0        0        0    11933 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/serialization.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/visualization/__init__.py
+-rw-r--r--   0        0        0     7305 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/visualization/charts.py
+-rw-r--r--   0        0        0     1866 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/visualization/common.py
+-rw-r--r--   0        0        0      941 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/visualization/labels.py
+-rw-r--r--   0        0        0     7802 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/visualization/plot.py
+-rw-r--r--   0        0        0     5767 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/visualization/titles.py
+-rw-r--r--   0        0        0     3181 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/visualization/tooltips.py
+-rw-r--r--   0        0        0     3289 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/visualization/transform_conv.py
+-rw-r--r--   0        0        0     1222 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/visualization/transform_retention.py
+-rw-r--r--   0        0        0     6148 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/__init__.py
+-rw-r--r--   0        0        0     5347 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/explore_page.css
+-rw-r--r--   0        0        0   147145 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/favicon.ico
+-rw-r--r--   0        0        0    46702 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/logo.png
+-rw-r--r--   0        0        0    43472 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/mitzu-logo-light.svg
+-rw-r--r--   0        0        0    49422 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/athena.png
+-rw-r--r--   0        0        0    20802 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/bigquery.png
+-rw-r--r--   0        0        0    10321 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/clickhouse.png
+-rw-r--r--   0        0        0   119554 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/databricks.png
+-rw-r--r--   0        0        0     3008 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/mysql.png
+-rw-r--r--   0        0        0     2446 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/pandas.png
+-rw-r--r--   0        0        0     5338 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/postgresql.png
+-rw-r--r--   0        0        0     8512 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/redshift.png
+-rw-r--r--   0        0        0    93500 2023-05-31 08:36:53.926470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/snowflake.png
+-rw-r--r--   0        0        0    48681 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/sqlite.png
+-rw-r--r--   0        0        0    34219 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/assets/warehouse/trino.png
+-rw-r--r--   0        0        0    15538 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/auth/authorizer.py
+-rw-r--r--   0        0        0     3557 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/auth/cognito.py
+-rw-r--r--   0        0        0     1305 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/auth/decorator.py
+-rw-r--r--   0        0        0     2777 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/auth/google.py
+-rw-r--r--   0        0        0     7481 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/cache.py
+-rw-r--r--   0        0        0     2920 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/caching_dataset_adapter.py
+-rw-r--r--   0        0        0     1664 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/configs.py
+-rw-r--r--   0        0        0     3432 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/dependencies.py
+-rw-r--r--   0        0        0     4984 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/helper.py
+-rw-r--r--   0        0        0     8631 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/model.py
+-rw-r--r--   0        0        0      309 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/navbar.py
+-rw-r--r--   0        0        0     5435 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/offcanvas.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/connections/__init__.py
+-rw-r--r--   0        0        0    22704 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/connections/manage_connections_component.py
+-rw-r--r--   0        0        0     4428 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/connections_page.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/dashboards/__init__.py
+-rw-r--r--   0        0        0    20561 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
+-rw-r--r--   0        0        0     9628 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/dashboards_page.py
+-rw-r--r--   0        0        0    14456 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/edit_user.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/__init__.py
+-rw-r--r--   0        0        0     5738 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/complex_segment_handler.py
+-rw-r--r--   0        0        0     6488 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/dates_selector_handler.py
+-rw-r--r--   0        0        0     5564 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/event_segment_handler.py
+-rw-r--r--   0        0        0    21704 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/explore_page.py
+-rw-r--r--   0        0        0    10100 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/graph_handler.py
+-rw-r--r--   0        0        0    10940 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/metric_config_handler.py
+-rw-r--r--   0        0        0     2375 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/metric_segments_handler.py
+-rw-r--r--   0        0        0     1565 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/metric_type_handler.py
+-rw-r--r--   0        0        0     9772 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/simple_segment_handler.py
+-rw-r--r--   0        0        0     4644 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore/toolbar_handler.py
+-rw-r--r--   0        0        0     1221 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/explore_project.py
+-rw-r--r--   0        0        0     1751 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/home.py
+-rw-r--r--   0        0        0     3947 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/login.py
+-rw-r--r--   0        0        0     5023 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/manage_connection.py
+-rw-r--r--   0        0        0     1288 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/manage_dashboard.py
+-rw-r--r--   0        0        0    10095 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/manage_event_defs.py
+-rw-r--r--   0        0        0    11845 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/manage_project.py
+-rw-r--r--   0        0        0     9470 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/manage_saved_metrics.py
+-rw-r--r--   0        0        0     1738 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/paths.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/projects/__init__.py
+-rw-r--r--   0        0        0    35694 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/projects/event_tables_config.py
+-rw-r--r--   0        0        0      587 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/projects/helper.py
+-rw-r--r--   0        0        0     9400 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/projects/manage_project_component.py
+-rw-r--r--   0        0        0     5090 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/projects_page.py
+-rw-r--r--   0        0        0     3114 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/pages/users.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/service/__init__.py
+-rw-r--r--   0        0        0     1919 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/service/events_service.py
+-rw-r--r--   0        0        0     4974 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/service/navbar_service.py
+-rw-r--r--   0        0        0      670 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/service/notification_service.py
+-rw-r--r--   0        0        0     2105 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/service/secret_service.py
+-rw-r--r--   0        0        0     6650 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/service/tracking_service.py
+-rw-r--r--   0        0        0     4719 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/service/user_service.py
+-rw-r--r--   0        0        0    24085 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/storage.py
+-rw-r--r--   0        0        0    25095 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/storage_model.py
+-rw-r--r--   0        0        0     4700 2023-05-31 08:36:53.930470 mitzu-0.6.2/mitzu/webapp/webapp.py
+-rw-r--r--   0        0        0     3422 2023-05-31 08:37:47.398121 mitzu-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 mitzu-0.6.2/PKG-INFO
```

### Comparing `mitzu-0.6.1/LICENSE.txt` & `mitzu-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/README.md` & `mitzu-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/.DS_Store` & `mitzu-0.6.2/mitzu/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/__init__.py` & `mitzu-0.6.2/mitzu/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 from mitzu.model import (
     Connection,
     ConnectionType,
     DiscoveredProject,
     EventDataTable,
     Project,
-    PromptSecretResolver,
     ConstSecretResolver,
-    EnvVarSecretResolver,
     TimeWindow,
     TimeGroup,
     DiscoverySettings,
     WebappSettings,
 )
 from mitzu.samples import get_sample_discovered_project
 
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 
 __all__ = [
     "Connection",
     "ConnectionType",
     "Project",
     "EventDataTable",
     "DiscoveredProject",
-    "PromptSecretResolver",
     "ConstSecretResolver",
-    "EnvVarSecretResolver",
     "TimeWindow",
     "TimeGroup",
     "get_sample_discovered_project",
     "DiscoverySettings",
     "WebappSettings",
 ]
```

### Comparing `mitzu-0.6.1/mitzu/adapters/adapter_factory.py` & `mitzu-0.6.2/mitzu/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/athena_adapter.py` & `mitzu-0.6.2/mitzu/adapters/athena_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/bigquery_adapter.py` & `mitzu-0.6.2/mitzu/adapters/bigquery_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/databricks_adapter.py` & `mitzu-0.6.2/mitzu/adapters/databricks_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/file_adapter.py` & `mitzu-0.6.2/mitzu/adapters/file_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/generic_adapter.py` & `mitzu-0.6.2/mitzu/adapters/generic_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/helper.py` & `mitzu-0.6.2/mitzu/adapters/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/mysql_adapter.py` & `mitzu-0.6.2/mitzu/adapters/mysql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/postgresql_adapter.py` & `mitzu-0.6.2/mitzu/adapters/postgresql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/redshift_adapter.py` & `mitzu-0.6.2/mitzu/adapters/redshift_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/snowflake_adapter.py` & `mitzu-0.6.2/mitzu/adapters/snowflake_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_helpers.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_struct.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/_types.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/geography.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/parse_url.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/bigquery/sqlalchemy/version.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlalchemy_adapter.py` & `mitzu-0.6.2/mitzu/adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/sqlite_adapter.py` & `mitzu-0.6.2/mitzu/adapters/sqlite_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/adapters/trino_adapter.py` & `mitzu-0.6.2/mitzu/adapters/trino_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/helper.py` & `mitzu-0.6.2/mitzu/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/model.py` & `mitzu-0.6.2/mitzu/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import os
 import pathlib
 from urllib import parse
 from abc import ABC
 from copy import copy
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 from enum import Enum, auto
@@ -447,62 +446,28 @@
     """
 
     def resolve_secret(self) -> str:
         raise NotImplementedError()
 
 
 @dataclass(frozen=True)
-class PromptSecretResolver(SecretResolver):
-    """
-    Prompts for a secret value on the first query execution in an interactive Python environment.
-
-    :param title: the title of the prompt
-    """
-
-    title: str = "Secret"
-
-    def resolve_secret(self) -> str:
-        import getpass
-
-        return getpass.getpass(prompt=self.title)
-
-
-@dataclass(frozen=True)
 class ConstSecretResolver(SecretResolver):
     """
     Resolves a secret with a preconfigured static value.
 
     :param secret: the secret value
     """
 
     secret: str
 
     def resolve_secret(self) -> str:
         return self.secret
 
 
 @dataclass(frozen=True)
-class EnvVarSecretResolver(SecretResolver):
-    """
-    Resolves a secret from an environmental variable or raises an exception if the environment variable is not found.
-
-    :param variable_name: name of the environment variable with containing the secret
-    """
-
-    variable_name: str
-
-    def resolve_secret(self) -> str:
-        secret = os.getenv(self.variable_name)
-        if secret is not None:
-            return secret
-        else:
-            raise Exception(f"Environmental variable {self.variable_name} was not set.")
-
-
-@dataclass(frozen=True)
 class Connection(Identifiable):
     """
     Contains all details needed to connect to a data warehouse.
 
     :param connection_type: type of the connection
     :param user_name: username
     :param secret_resolver: secret resolver to get the user password
```

### Comparing `mitzu-0.6.1/mitzu/notebook/model_loader.py` & `mitzu-0.6.2/mitzu/notebook/model_loader.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/project_discovery.py` & `mitzu-0.6.2/mitzu/project_discovery.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/project_serialization.py` & `mitzu-0.6.2/mitzu/project_serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/samples/__init__.py` & `mitzu-0.6.2/mitzu/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/samples/data_ingestion.py` & `mitzu-0.6.2/mitzu/samples/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/samples/sample_data_generator.py` & `mitzu-0.6.2/mitzu/samples/sample_data_generator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/serialization.py` & `mitzu-0.6.2/mitzu/serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/visualization/charts.py` & `mitzu-0.6.2/mitzu/visualization/charts.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/visualization/common.py` & `mitzu-0.6.2/mitzu/visualization/common.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/visualization/labels.py` & `mitzu-0.6.2/mitzu/visualization/labels.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/visualization/plot.py` & `mitzu-0.6.2/mitzu/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/visualization/titles.py` & `mitzu-0.6.2/mitzu/visualization/titles.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/visualization/tooltips.py` & `mitzu-0.6.2/mitzu/visualization/tooltips.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/visualization/transform_conv.py` & `mitzu-0.6.2/mitzu/visualization/transform_conv.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/visualization/transform_retention.py` & `mitzu-0.6.2/mitzu/visualization/transform_retention.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/.DS_Store` & `mitzu-0.6.2/mitzu/webapp/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/assets/explore_page.css` & `mitzu-0.6.2/mitzu/webapp/assets/explore_page.css`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/assets/favicon.ico` & `mitzu-0.6.2/mitzu/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/assets/logo.png` & `mitzu-0.6.2/mitzu/webapp/assets/logo.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/assets/mitzu-logo-light.svg` & `mitzu-0.6.2/mitzu/webapp/assets/mitzu-logo-light.svg`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/assets/warehouse/athena.png` & `mitzu-0.6.2/mitzu/webapp/assets/warehouse/athena.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/assets/warehouse/bigquery.png` & `mitzu-0.6.2/mitzu/webapp/assets/warehouse/bigquery.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/assets/warehouse/clickhouse.png` & `mitzu-0.6.2/mitzu/webapp/assets/warehouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/assets/warehouse/databricks.png` & `mitzu-0.6.2/mitzu/webapp/assets/warehouse/databricks.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/assets/warehouse/mysql.png` & `mitzu-0.6.2/mitzu/webapp/assets/warehouse/mysql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/assets/warehouse/pandas.png` & `mitzu-0.6.2/mitzu/webapp/assets/warehouse/pandas.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/assets/warehouse/postgresql.png` & `mitzu-0.6.2/mitzu/webapp/assets/warehouse/postgresql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/assets/warehouse/redshift.png` & `mitzu-0.6.2/mitzu/webapp/assets/warehouse/redshift.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/assets/warehouse/snowflake.png` & `mitzu-0.6.2/mitzu/webapp/assets/warehouse/snowflake.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/assets/warehouse/sqlite.png` & `mitzu-0.6.2/mitzu/webapp/assets/warehouse/sqlite.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/assets/warehouse/trino.png` & `mitzu-0.6.2/mitzu/webapp/assets/warehouse/trino.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/auth/authorizer.py` & `mitzu-0.6.2/mitzu/webapp/auth/authorizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,17 +111,19 @@
             P.SIGN_OUT_URL,
             P.HEALTHCHECK_PATH,
             "/assets/",
             "/_dash-component-suites/",
         ]
 
     def get_home_url(self):
+        home_url = flask.request.url_root
         if configs.HOME_URL:
-            return configs.HOME_URL
-        return flask.request.url_root
+            home_url = configs.HOME_URL
+        # trailing slashes can cause issues with SSO login
+        return home_url.strip("/")
 
     def get_auth_token(self):
         return flask.request.cookies.get(self._config.token_cookie_name)
 
     def _get_unauthenticated_response(
         self, redirect_url: Optional[str] = None
     ) -> werkzeug.wrappers.response.Response:
```

### Comparing `mitzu-0.6.1/mitzu/webapp/auth/cognito.py` & `mitzu-0.6.2/mitzu/webapp/auth/cognito.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/auth/decorator.py` & `mitzu-0.6.2/mitzu/webapp/auth/decorator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/auth/google.py` & `mitzu-0.6.2/mitzu/webapp/auth/google.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/cache.py` & `mitzu-0.6.2/mitzu/webapp/cache.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/caching_dataset_adapter.py` & `mitzu-0.6.2/mitzu/webapp/caching_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/configs.py` & `mitzu-0.6.2/mitzu/webapp/configs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/dependencies.py` & `mitzu-0.6.2/mitzu/webapp/dependencies.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/helper.py` & `mitzu-0.6.2/mitzu/webapp/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/model.py` & `mitzu-0.6.2/mitzu/webapp/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,7 +269,19 @@
     """
 
     email: str
     password_hash: Optional[str]
     password_salt: Optional[str]
     id: str = field(default_factory=create_unique_id)
     role: Role = Role.MEMBER
+
+
+@dataclass(frozen=True)
+class ProjectInfo:
+    """
+    Contains the minimal set of details of a project.
+
+    Use this instance to quickly render UI elements without querying the event data tables or discovered fields.
+    """
+
+    id: str
+    name: str
```

### Comparing `mitzu-0.6.1/mitzu/webapp/offcanvas.py` & `mitzu-0.6.2/mitzu/webapp/offcanvas.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/connections/manage_connections_component.py` & `mitzu-0.6.2/mitzu/webapp/pages/connections/manage_connections_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -611,26 +611,28 @@
     if delete is None:
         return no_update, no_update
     deps = DEPS.Dependencies.get()
     if ctx.triggered_id == CONNECTION_DELETE_BUTTON:
         connection_id = P.get_path_value(
             P.CONNECTIONS_MANAGE_PATH, pathname, P.CONNECTION_ID_PATH_PART
         )
-        project_ids = deps.storage.list_projects()
-        for p_id in project_ids:
-            prj = deps.storage.get_project(p_id)
+        projects = deps.storage.list_projects()
+        for project in projects:
+            prj = deps.storage.get_project(project.id)
             if prj.get_connection_id() == connection_id:
                 return False, html.Div(
                     children=[
                         html.Span(
                             "You can't delete this connection because it is used by  "
                         ),
                         dcc.Link(
                             prj.project_name,
-                            P.create_path(P.PROJECTS_MANAGE_PATH, project_id=p_id),
+                            P.create_path(
+                                P.PROJECTS_MANAGE_PATH, project_id=project.id
+                            ),
                         ),
                     ],
                     className="my-3 text-danger lead",
                 )
         return True, ""
 
     return False, ""
```

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/connections_page.py` & `mitzu-0.6.2/mitzu/webapp/pages/connections_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/dashboards/manage_dashboards_component.py` & `mitzu-0.6.2/mitzu/webapp/pages/dashboards/manage_dashboards_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/dashboards_page.py` & `mitzu-0.6.2/mitzu/webapp/pages/dashboards_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/edit_user.py` & `mitzu-0.6.2/mitzu/webapp/pages/edit_user.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/explore/complex_segment_handler.py` & `mitzu-0.6.2/mitzu/webapp/pages/explore/complex_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/explore/dates_selector_handler.py` & `mitzu-0.6.2/mitzu/webapp/pages/explore/dates_selector_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/explore/event_segment_handler.py` & `mitzu-0.6.2/mitzu/webapp/pages/explore/event_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/explore/explore_page.py` & `mitzu-0.6.2/mitzu/webapp/pages/explore/explore_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/explore/graph_handler.py` & `mitzu-0.6.2/mitzu/webapp/pages/explore/graph_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/explore/metric_config_handler.py` & `mitzu-0.6.2/mitzu/webapp/pages/explore/metric_config_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/explore/metric_segments_handler.py` & `mitzu-0.6.2/mitzu/webapp/pages/explore/metric_segments_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/explore/metric_type_handler.py` & `mitzu-0.6.2/mitzu/webapp/pages/explore/metric_type_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/explore/simple_segment_handler.py` & `mitzu-0.6.2/mitzu/webapp/pages/explore/simple_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/explore/toolbar_handler.py` & `mitzu-0.6.2/mitzu/webapp/pages/explore/toolbar_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/explore_project.py` & `mitzu-0.6.2/mitzu/webapp/pages/explore_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/home.py` & `mitzu-0.6.2/mitzu/webapp/pages/home.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/login.py` & `mitzu-0.6.2/mitzu/webapp/pages/login.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/manage_connection.py` & `mitzu-0.6.2/mitzu/webapp/pages/manage_connection.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/manage_dashboard.py` & `mitzu-0.6.2/mitzu/webapp/pages/manage_dashboard.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/manage_event_defs.py` & `mitzu-0.6.2/mitzu/webapp/pages/manage_event_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,24 +90,24 @@
 
 def no_project_layout():
     return layout(None)
 
 
 @restricted_layout
 def layout(project_id: Optional[str], **query_params) -> bc.Component:
-    events_service = DEPS.Dependencies.get().events_service
+    storage = DEPS.Dependencies.get().storage
 
-    projects = events_service.list_all_projects()
+    projects = storage.list_projects()
     selected_project: Optional[M.Project] = None
     for p in projects:
         if p.id == project_id:
-            selected_project = p
+            selected_project = storage.get_project(p.id)
             break
 
-    options = [{"label": p.project_name, "value": p.id} for p in projects]
+    options = [{"label": p.name, "value": p.id} for p in projects]
 
     return html.Div(
         [
             NB.create_mitzu_navbar("events-navbar"),
             dbc.Container(
                 [
                     html.H4("Discovered events and properties"),
```

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/manage_project.py` & `mitzu-0.6.2/mitzu/webapp/pages/manage_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/manage_saved_metrics.py` & `mitzu-0.6.2/mitzu/webapp/pages/manage_saved_metrics.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/paths.py` & `mitzu-0.6.2/mitzu/webapp/pages/paths.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/projects/event_tables_config.py` & `mitzu-0.6.2/mitzu/webapp/pages/projects/event_tables_config.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/projects/helper.py` & `mitzu-0.6.2/mitzu/webapp/pages/projects/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/projects/manage_project_component.py` & `mitzu-0.6.2/mitzu/webapp/pages/projects/manage_project_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/projects_page.py` & `mitzu-0.6.2/mitzu/webapp/pages/projects_page.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,21 +60,21 @@
             ),
         ]
     )
 
 
 def create_projects_children() -> List[bc.Component]:
     depenednecies = DEPS.Dependencies.get()
-    project_ids = depenednecies.storage.list_projects()
+    stored_projects = depenednecies.storage.list_projects()
 
     projects = []
-    if len(project_ids) > 0:
-        for p in project_ids:
+    if len(stored_projects) > 0:
+        for p in stored_projects:
             try:
-                projects.append(create_project_selector(p, depenednecies))
+                projects.append(create_project_selector(p.id, depenednecies))
             except Exception as exc:
                 traceback.print_exc()
                 projects.append(
                     dbc.Col(
                         dbc.Card(
                             dbc.CardBody(html.P(str(exc), className="text-danger")),
                             class_name="mb-3",
```

### Comparing `mitzu-0.6.1/mitzu/webapp/pages/users.py` & `mitzu-0.6.2/mitzu/webapp/pages/users.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/service/events_service.py` & `mitzu-0.6.2/mitzu/webapp/service/events_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 from dataclasses import dataclass
 import mitzu.webapp.storage as S
-from typing import Callable, Dict, List, Optional
+from typing import Callable, Dict, Optional
 import mitzu.model as M
 
 
 class EventServiceException(Exception):
     pass
 
 
 @dataclass
 class EventsService:
 
     storage: S.MitzuStorage
 
-    def list_all_projects(self) -> List[M.Project]:
-        project_ids = self.storage.list_projects()
-        return [
-            self.storage.get_project(pid) for pid in project_ids
-        ]  # todo move this logic to storage
-
     def populate_discovered_project(self, discovered_project: M.DiscoveredProject):
         self.storage.populate_discovered_project(discovered_project)
 
     def get_project_definition(
         self, project_id: str
     ) -> Dict[M.EventDataTable, Dict[str, M.Reference[M.EventDef]]]:
         project = self.storage.get_project(project_id)
```

### Comparing `mitzu-0.6.1/mitzu/webapp/service/navbar_service.py` & `mitzu-0.6.2/mitzu/webapp/service/navbar_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,20 +44,19 @@
             storage: Optional[S.MitzuStorage] = None,
             **kwargs,
         ) -> Optional[bc.Component]:
             if create_explore_button:
                 if storage is None:
                     storage = DEPS.Dependencies.get().storage
 
-                project_ids = storage.list_projects()
-                projects = [storage.get_project(p_id) for p_id in project_ids]
+                projects = storage.list_projects()
                 return dbc.DropdownMenu(
                     children=[
                         dbc.DropdownMenuItem(
-                            children=p.project_name,
+                            children=p.name,
                             href=P.create_path(
                                 P.PROJECTS_EXPLORE_PATH, project_id=p.id
                             ),
                         )
                         for p in projects
                     ],
                     size="sm",
```

### Comparing `mitzu-0.6.1/mitzu/webapp/service/notification_service.py` & `mitzu-0.6.2/mitzu/webapp/service/notification_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/service/secret_service.py` & `mitzu-0.6.2/mitzu/webapp/service/secret_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/service/tracking_service.py` & `mitzu-0.6.2/mitzu/webapp/service/tracking_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/service/user_service.py` & `mitzu-0.6.2/mitzu/webapp/service/user_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/mitzu/webapp/storage.py` & `mitzu-0.6.2/mitzu/webapp/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import multiprocessing
 from typing import Dict, List, Optional
 
 from mitzu.helper import LOGGER
 import mitzu.model as M
 import mitzu.webapp.model as WM
 import mitzu.webapp.storage_model as SM
+import mitzu.webapp.dependencies as DEPS
 from mitzu.samples.data_ingestion import create_and_ingest_sample_project
 import sqlalchemy as SA
 from sqlalchemy.orm import Session
 
-import flask
 
 SAMPLE_PROJECT_NAME = "sample_project"
 SAMPLE_PROJECT_ID = "sample_project_id"
 SAMPLE_CONNECTION_ID = "sample_connection_id"
 
 
 DEFAULT_CONNECTION_STRING = "sqlite://?check_same_thread=False"
@@ -34,17 +34,21 @@
     ):
         super().__init__(id=id, value=value)
         self.event_data_table = event_data_table
 
     def get_value(self) -> Optional[M.EventDef]:
         res = self._value_state.get_value()
         if res is None:
-            deps = flask.current_app.config.get("dependencies")
-            if deps is None:
-                raise InvalidStorageReference("No storage in request dependencies")
+            try:
+                deps = DEPS.Dependencies.get()
+            except Exception as e:
+                raise InvalidStorageReference("No dependencies in request state") from e
+
+            if self._id is None:
+                raise ValueError("Event definition reference id is missing")
             res = deps.storage.get_event_definition(
                 event_definition_id=self._id, event_data_table=self.event_data_table
             )
             self.restore_value(res)
         return res
 
 
@@ -357,19 +361,19 @@
         if record is None:
             raise ValueError(
                 f"Webapp settings not found with project_id={webapp_settings_id}"
             )
 
         return record.as_model_instance()
 
-    def list_projects(self) -> List[str]:
+    def list_projects(self) -> List[WM.ProjectInfo]:
         result = []
         with self._new_db_session() as session:
             for record in session.query(SM.ProjectStorageRecord):
-                result.append(record.project_id)
+                result.append(WM.ProjectInfo(record.project_id, record.name))
             return result
 
     def set_connection(self, connection_id: str, connection: M.Connection):
         with self._new_db_session() as session:
             self._set_connection(connection_id, connection, session)
             session.commit()
```

### Comparing `mitzu-0.6.1/mitzu/webapp/storage_model.py` & `mitzu-0.6.2/mitzu/webapp/storage_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,23 +178,19 @@
 
     secret_resolver_type = SA.Column(SA.String, nullable=True, default=None)
     secret_resolver_arg = SA.Column(SA.String, nullable=True, default=None)
 
     def update(self, connection: M.Connection):
         secret_resolver_type = None
         secret_resolver_arg = None
-        if isinstance(connection.secret_resolver, M.EnvVarSecretResolver):
-            secret_resolver_type = "env"
-            secret_resolver_arg = connection.secret_resolver.variable_name
-        elif isinstance(connection.secret_resolver, M.ConstSecretResolver):
+        if isinstance(connection.secret_resolver, M.ConstSecretResolver):
             secret_resolver_type = "const"
             secret_resolver_arg = connection.secret_resolver.resolve_secret()
-        elif isinstance(connection.secret_resolver, M.PromptSecretResolver):
-            secret_resolver_type = "prompt"
-            secret_resolver_arg = connection.secret_resolver.title
+        elif connection.secret_resolver is not None:
+            raise ValueError("Unknown secret resolver type")
 
         self.connection_name = connection.connection_name
         self.connection_type = connection.connection_type.value
         self.user_name = connection.user_name
         self.host = connection.host
         self.port = connection.port
         self.url = connection.url
@@ -207,20 +203,18 @@
             else None
         )
         self.secret_resolver_type = secret_resolver_type
         self.secret_resolver_arg = secret_resolver_arg
 
     def as_model_instance(self) -> M.Connection:
         secret_resolver: Optional[M.SecretResolver] = None
-        if self.secret_resolver_type == "env":
-            secret_resolver = M.EnvVarSecretResolver(self.secret_resolver_arg)
-        elif self.secret_resolver_type == "const":
+        if self.secret_resolver_type == "const":
             secret_resolver = M.ConstSecretResolver(self.secret_resolver_arg)
-        elif self.secret_resolver_type == "prompt":
-            secret_resolver = M.PromptSecretResolver(self.secret_resolver_arg)
+        elif self.secret_resolver_type is not None:
+            raise ValueError("Unknown secret resolver type")
 
         return M.Connection(
             connection_name=self.connection_name,
             connection_type=M.ConnectionType(self.connection_type),
             id=self.connection_id,
             user_name=self.user_name,
             host=self.host,
@@ -233,23 +227,19 @@
             secret_resolver=secret_resolver,
         )
 
     @classmethod
     def from_model_instance(self, model: M.Connection) -> ConnectionStorageRecord:
         secret_resolver_type = None
         secret_resolver_arg = None
-        if isinstance(model.secret_resolver, M.EnvVarSecretResolver):
-            secret_resolver_type = "env"
-            secret_resolver_arg = model.secret_resolver.variable_name
-        elif isinstance(model.secret_resolver, M.ConstSecretResolver):
+        if isinstance(model.secret_resolver, M.ConstSecretResolver):
             secret_resolver_type = "const"
             secret_resolver_arg = model.secret_resolver.resolve_secret()
-        elif isinstance(model.secret_resolver, M.PromptSecretResolver):
-            secret_resolver_type = "prompt"
-            secret_resolver_arg = model.secret_resolver.title
+        elif model.secret_resolver is not None:
+            raise ValueError("Unknown secret resolver type")
 
         return ConnectionStorageRecord(
             connection_id=model.id,
             connection_name=model.connection_name,
             connection_type=model.connection_type.value,
             user_name=model.user_name,
             host=model.host,
```

### Comparing `mitzu-0.6.1/mitzu/webapp/webapp.py` & `mitzu-0.6.2/mitzu/webapp/webapp.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.1/pyproject.toml` & `mitzu-0.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mitzu"
-version = "0.6.1"
+version = "0.6.2"
 description = "Product analytics over your data warehouse"
 authors = ["Istvan Meszaros <istvan.meszaros.88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mitzu.io"
 repository = "https://github.com/mitzu-io/mitzu"
 documentation = "https://mitzu.io/documentation/"
```

### Comparing `mitzu-0.6.1/PKG-INFO` & `mitzu-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitzu
-Version: 0.6.1
+Version: 0.6.2
 Summary: Product analytics over your data warehouse
 Home-page: https://mitzu.io
 License: MIT
 Author: Istvan Meszaros
 Author-email: istvan.meszaros.88@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

