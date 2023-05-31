# Comparing `tmp/onetl-0.7.2.tar.gz` & `tmp/onetl-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onetl-0.7.2.tar", last modified: Wed May 24 19:09:31 2023, max compression
+gzip compressed data, was "onetl-0.8.0.tar", last modified: Wed May 31 12:25:25 2023, max compression
```

## Comparing `onetl-0.7.2.tar` & `onetl-0.8.0.tar`

### file list

```diff
@@ -1,171 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.681135 onetl-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-05-24 19:09:27.000000 onetl-0.7.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-24 19:09:27.000000 onetl-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17338 2023-05-24 19:09:31.681135 onetl-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-05-24 19:09:27.000000 onetl-0.7.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.669135 onetl-0.7.2/onetl/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/_internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.669135 onetl-0.7.2/onetl/base/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/base/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/base/base_db_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/base/base_file_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/base/base_file_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/base/base_file_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/base/contains_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/base/contains_get_df_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/base/path_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/base/path_stat_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.669135 onetl-0.7.2/onetl/connection/
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.669135 onetl-0.7.2/onetl/connection/db_connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/db_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.673135 onetl-0.7.2/onetl/connection/db_connection/dialect_mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/dialect_mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/dialect_mixins/support_columns_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/dialect_mixins/support_columns_none.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/dialect_mixins/support_df_schema_none.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/dialect_mixins/support_df_schema_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/dialect_mixins/support_hint_none.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/dialect_mixins/support_hint_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_none.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/dialect_mixins/support_table_with_dbschema.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/dialect_mixins/support_table_without_dbschema.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/dialect_mixins/support_where_str.py
--rw-r--r--   0 runner    (1001) docker     (123)    26511 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/greenplum.py
--rw-r--r--   0 runner    (1001) docker     (123)    32279 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/hive.py
--rw-r--r--   0 runner    (1001) docker     (123)    27892 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/jdbc_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    23510 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/jdbc_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    25845 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/mssql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/db_connection/teradata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.673135 onetl-0.7.2/onetl/connection/file_connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/file_connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25013 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/file_connection/file_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/file_connection/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/file_connection/ftps.py
--rw-r--r--   0 runner    (1001) docker     (123)    26222 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/file_connection/hdfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/file_connection/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/file_connection/sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/file_connection/webdav.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/connection/kerberos_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.673135 onetl-0.7.2/onetl/core/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.673135 onetl-0.7.2/onetl/core/db_reader/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/db_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21805 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/db_reader/db_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/db_reader/strategy_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.673135 onetl-0.7.2/onetl/core/db_writer/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/db_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/db_writer/db_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.673135 onetl-0.7.2/onetl/core/file_downloader/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/file_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/file_downloader/download_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    25273 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/file_downloader/file_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.673135 onetl-0.7.2/onetl/core/file_filter/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/file_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/file_filter/file_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/file_filter/file_hwm_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/file_filter/match_all_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.673135 onetl-0.7.2/onetl/core/file_limit/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/file_limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/file_limit/file_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/file_limit/limits_reached.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.673135 onetl-0.7.2/onetl/core/file_result/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/file_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/file_result/file_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/file_result/file_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.677135 onetl-0.7.2/onetl/core/file_uploader/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/file_uploader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/file_uploader/file_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/core/file_uploader/upload_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.677135 onetl-0.7.2/onetl/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/hooks/hook_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/hooks/hooks_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/hooks/method_inheritance_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)    20801 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/hooks/slot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/hooks/support_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.677135 onetl-0.7.2/onetl/hwm/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/hwm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/hwm/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.677135 onetl-0.7.2/onetl/hwm/store/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/hwm/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/hwm/store/base_hwm_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/hwm/store/hwm_class_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/hwm/store/hwm_store_class_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/hwm/store/hwm_store_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/hwm/store/memory_hwm_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/hwm/store/yaml_hwm_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.677135 onetl-0.7.2/onetl/impl/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/impl/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/impl/failed_local_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/impl/file_write_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/impl/frozen_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/impl/generic_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/impl/local_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/impl/path_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/impl/path_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/impl/remote_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/impl/remote_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/impl/remote_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/impl/remote_path_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.677135 onetl-0.7.2/onetl/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/plugins/import_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.681135 onetl-0.7.2/onetl/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/strategy/base_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/strategy/batch_hwm_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.681135 onetl-0.7.2/onetl/strategy/hwm_store/
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/strategy/hwm_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/strategy/hwm_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19047 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/strategy/incremental_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/strategy/snapshot_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/strategy/strategy_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-24 19:09:27.000000 onetl-0.7.2/onetl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.669135 onetl-0.7.2/onetl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17338 2023-05-24 19:09:31.000000 onetl-0.7.2/onetl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-24 19:09:31.000000 onetl-0.7.2/onetl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 19:09:31.000000 onetl-0.7.2/onetl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 19:09:31.000000 onetl-0.7.2/onetl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-24 19:09:31.000000 onetl-0.7.2/onetl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 19:09:31.000000 onetl-0.7.2/onetl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-24 19:09:27.000000 onetl-0.7.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.681135 onetl-0.7.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/ftp.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/hdfs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/kerberos.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/s3.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/sftp.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/spark.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 19:09:31.681135 onetl-0.7.2/requirements/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/tests/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/tests/clickhouse.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/tests/mongodb.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/tests/mssql.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/tests/mysql.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/tests/oracle.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/tests/postgres.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/tests/spark-2.4.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/tests/spark-3.2.3.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/tests/spark-3.3.2.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/tests/spark-3.4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-24 19:09:27.000000 onetl-0.7.2/requirements/webdav.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-24 19:09:31.681135 onetl-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-24 19:09:27.000000 onetl-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.988076 onetl-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-05-31 12:25:07.000000 onetl-0.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-31 12:25:07.000000 onetl-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-05-31 12:25:25.988076 onetl-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-05-31 12:25:07.000000 onetl-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.972076 onetl-0.8.0/onetl/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/_internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.972076 onetl-0.8.0/onetl/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/base_db_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19126 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/base_file_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/base_file_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/base_file_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/contains_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/contains_get_df_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/path_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/path_stat_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/pure_path_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/base/supports_rename_dir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.972076 onetl-0.8.0/onetl/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.976076 onetl-0.8.0/onetl/connection/db_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/db_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.976076 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_columns_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_columns_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_df_schema_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_df_schema_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_hint_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_hint_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_table_with_dbschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_table_without_dbschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_where_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26511 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/greenplum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32279 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/hive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27890 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/jdbc_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23506 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/jdbc_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25843 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/db_connection/teradata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.976076 onetl-0.8.0/onetl/connection/file_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24970 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/file_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/ftps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26369 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/hdfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.976076 onetl-0.8.0/onetl/connection/file_connection/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/mixins/rename_dir_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/file_connection/webdav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/connection/kerberos_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.976076 onetl-0.8.0/onetl/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/core/file_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/core/file_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/core/file_filter/file_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/core/file_limit/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/core/file_limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/core/file_limit/file_limit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/db/db_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/db/db_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21795 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/db/db_reader/db_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/db/db_reader/strategy_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/db/db_writer/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/db/db_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/db/db_writer/db_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/file/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/file/file_downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_downloader/download_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27219 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_downloader/file_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/file/file_mover/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_mover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17605 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_mover/file_mover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_mover/move_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18629 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/file/file_uploader/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_uploader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_uploader/file_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/file_uploader/upload_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/file/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/filter/exclude_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/filter/file_hwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/filter/glob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/filter/match_all_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/filter/regexp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.980076 onetl-0.8.0/onetl/file/limit/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/limit/limits_reached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/limit/limits_stop_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/limit/max_files_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/file/limit/reset_limits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.984076 onetl-0.8.0/onetl/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hooks/hook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hooks/hooks_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hooks/method_inheritance_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20801 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hooks/slot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hooks/support_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.984076 onetl-0.8.0/onetl/hwm/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hwm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hwm/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.984076 onetl-0.8.0/onetl/hwm/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hwm/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hwm/store/base_hwm_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hwm/store/hwm_class_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hwm/store/hwm_store_class_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hwm/store/hwm_store_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hwm/store/memory_hwm_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/hwm/store/yaml_hwm_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.984076 onetl-0.8.0/onetl/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/failed_local_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/file_write_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/frozen_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/generic_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/local_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/path_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/path_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/remote_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/remote_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/remote_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/impl/remote_path_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.984076 onetl-0.8.0/onetl/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/plugins/import_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.988076 onetl-0.8.0/onetl/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/strategy/base_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/strategy/batch_hwm_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.988076 onetl-0.8.0/onetl/strategy/hwm_store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/strategy/hwm_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/strategy/hwm_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19043 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/strategy/incremental_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/strategy/snapshot_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/strategy/strategy_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-31 12:25:07.000000 onetl-0.8.0/onetl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.972076 onetl-0.8.0/onetl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-05-31 12:25:25.000000 onetl-0.8.0/onetl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-05-31 12:25:25.000000 onetl-0.8.0/onetl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:25:25.000000 onetl-0.8.0/onetl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:25:25.000000 onetl-0.8.0/onetl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-31 12:25:25.000000 onetl-0.8.0/onetl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 12:25:25.000000 onetl-0.8.0/onetl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-31 12:25:07.000000 onetl-0.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.988076 onetl-0.8.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/ftp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/hdfs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/kerberos.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/s3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/sftp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/spark.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:25:25.988076 onetl-0.8.0/requirements/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/clickhouse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/mongodb.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/mssql.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/mysql.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/oracle.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/postgres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/spark-2.3.1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/spark-2.4.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/spark-3.2.3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/spark-3.3.2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/spark-3.4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/tests/spark-latest.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 12:25:07.000000 onetl-0.8.0/requirements/webdav.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-31 12:25:25.992076 onetl-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-31 12:25:08.000000 onetl-0.8.0/setup.py
```

### Comparing `onetl-0.7.2/LICENSE.txt` & `onetl-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/PKG-INFO` & `onetl-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetl
-Version: 0.7.2
+Version: 0.8.0
 Summary: One ETL tool to rule them all
 Home-page: https://github.com/MobileTeleSystems/onetl
 Author: DataOps.ETL
 Author-email: onetools@mts.ru
 License: Apache License 2.0
 Project-URL: Documentation, https://onetl.readthedocs.io/
 Project-URL: Source, https://github.com/MobileTeleSystems/onetl
@@ -159,15 +159,15 @@
 
 Minimal installation
 ~~~~~~~~~~~~~~~~~~~~
 
 Base ``onetl`` package contains:
 
 * ``DBReader``, ``DBWriter`` and related classes
-* ``FileDownloader``, ``FileUploader``, ``FileFilter``, ``FileLimit`` and related classes
+* ``FileDownloader``, ``FileUploader``, ``FileMover`` and related classes, like file filters & limits
 * Read Strategies & HWM classes
 * Plugins support
 
 It can be installed via:
 
 .. code:: bash
 
@@ -437,15 +437,16 @@
     .. code::
 
         127.0.0.1 hdfs
 
 .. note::
 
     To run Oracle tests you need to install `Oracle instantclient <https://www.oracle.com/database/technologies/instant-client.html>`__,
-    and pass its path to ``ONETL_ORA_CLIENT_PATH`` environment variable, e.g. ``ONETL_ORA_CLIENT_PATH=/path/to/client64/lib``.
+    and pass its path to ``ONETL_ORA_CLIENT_PATH`` and ``LD_LIBRARY_PATH`` environment variables,
+    e.g. ``ONETL_ORA_CLIENT_PATH=/path/to/client64/lib``.
 
     It may also require to add the same path into ``LD_LIBRARY_PATH`` environment variable
 
 .. note::
 
     To run Greenplum tests, you should:
```

### Comparing `onetl-0.7.2/README.rst` & `onetl-0.8.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
 Minimal installation
 ~~~~~~~~~~~~~~~~~~~~
 
 Base ``onetl`` package contains:
 
 * ``DBReader``, ``DBWriter`` and related classes
-* ``FileDownloader``, ``FileUploader``, ``FileFilter``, ``FileLimit`` and related classes
+* ``FileDownloader``, ``FileUploader``, ``FileMover`` and related classes, like file filters & limits
 * Read Strategies & HWM classes
 * Plugins support
 
 It can be installed via:
 
 .. code:: bash
 
@@ -392,15 +392,16 @@
     .. code::
 
         127.0.0.1 hdfs
 
 .. note::
 
     To run Oracle tests you need to install `Oracle instantclient <https://www.oracle.com/database/technologies/instant-client.html>`__,
-    and pass its path to ``ONETL_ORA_CLIENT_PATH`` environment variable, e.g. ``ONETL_ORA_CLIENT_PATH=/path/to/client64/lib``.
+    and pass its path to ``ONETL_ORA_CLIENT_PATH`` and ``LD_LIBRARY_PATH`` environment variables,
+    e.g. ``ONETL_ORA_CLIENT_PATH=/path/to/client64/lib``.
 
     It may also require to add the same path into ``LD_LIBRARY_PATH`` environment variable
 
 .. note::
 
     To run Greenplum tests, you should:
```

### Comparing `onetl-0.7.2/onetl/__init__.py` & `onetl-0.8.0/onetl/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/_internal.py` & `onetl-0.8.0/onetl/_internal.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/base/__init__.py` & `onetl-0.8.0/onetl/base/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,7 +16,9 @@
 from onetl.base.base_db_connection import BaseDBConnection
 from onetl.base.base_file_connection import BaseFileConnection
 from onetl.base.base_file_filter import BaseFileFilter
 from onetl.base.base_file_limit import BaseFileLimit
 from onetl.base.contains_exception import ContainsException
 from onetl.base.path_protocol import PathProtocol, PathWithStatsProtocol
 from onetl.base.path_stat_protocol import PathStatProtocol
+from onetl.base.pure_path_protocol import PurePathProtocol
+from onetl.base.supports_rename_dir import SupportsRenameDir
```

### Comparing `onetl-0.7.2/onetl/base/base_connection.py` & `onetl-0.8.0/onetl/base/base_connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,12 +20,25 @@
     Generic connection class
     """
 
     @abstractmethod
     def check(self):
         """Check source availability.
 
+        If not, an exception will be raised.
+
+        Returns
+        -------
+        Connection itself
+
         Raises
         ------
         RuntimeError
             If the connection is not available
+
+        Examples
+        --------
+
+        .. code:: python
+
+            connection.check()
         """
```

### Comparing `onetl-0.7.2/onetl/base/base_db_connection.py` & `onetl-0.8.0/onetl/base/base_db_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,39 +138,14 @@
 
     @property
     @abstractmethod
     def instance_url(self) -> str:
         """Instance URL"""
 
     @abstractmethod
-    def check(self):
-        """
-        Check if database is accessible.
-
-        If not, an exception will be raised.
-
-        Executes some simple query, like ``SELECT 1``, in the database.
-
-        Examples
-        --------
-
-        Database is online:
-
-        .. code:: python
-
-            connection.check()
-
-        Database is offline or not accessible:
-
-        .. code:: python
-
-            connection.check()  # raises RuntimeError exception
-        """
-
-    @abstractmethod
     # Some heirs may have a different number of parameters.
     # For example, the 'options' parameter may be present. This is fine.
     def read_df(
         self,
         source: str,
         columns: list[str] | None = None,
         hint: Any | None = None,
```

### Comparing `onetl-0.7.2/onetl/base/base_file_filter.py` & `onetl-0.8.0/onetl/impl/frozen_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,22 +10,13 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
+from onetl.impl.base_model import BaseModel
 
-from onetl.base.path_protocol import PathProtocol
 
-
-class BaseFileFilter(ABC):
-    """
-    Base file filter class
-    """
-
-    @abstractmethod
-    def match(self, path: PathProtocol) -> bool:
-        """
-        Checks if path should be handled
-        """
+class FrozenModel(BaseModel):
+    class Config:
+        frozen = True
```

### Comparing `onetl-0.7.2/onetl/base/base_file_limit.py` & `onetl-0.8.0/onetl/base/path_stat_protocol.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,35 +10,47 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
+from typing_extensions import Protocol, runtime_checkable
 
-from onetl.base.path_protocol import PathProtocol
 
-
-class BaseFileLimit(ABC):
+@runtime_checkable
+class PathStatProtocol(Protocol):
     """
-    Base file limit class
+    Protocol for ``os.stat_result``-like objects.
+
+    Includes only minimal set of fields supported by any file system
     """
 
-    @abstractmethod
-    def reset(self):
+    @property
+    def st_size(self) -> int:
+        """
+        Size of file, in bytes
+        """
+
+    @property
+    def st_mtime(self) -> float | None:
+        """
+        Unix timestamp of most recent content modification
+        """
+
+    @property
+    def st_uid(self) -> str | int | None:
         """
-        Resets the internal state
+        User identifier of the file owner
         """
 
-    @abstractmethod
-    def stops_at(self, path: PathProtocol) -> bool:
+    @property
+    def st_gid(self) -> str | int | None:
         """
-        Update internal state and check if it is reached. Returns ``True`` if limit is reached
+        Group identifier of the file owner
         """
 
     @property
-    @abstractmethod
-    def is_reached(self) -> bool:
+    def st_mode(self) -> int | None:
         """
-        Returns ``True`` if limit is reached
+        File mode bits
         """
```

### Comparing `onetl-0.7.2/onetl/base/contains_exception.py` & `onetl-0.8.0/onetl/base/contains_exception.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/base/contains_get_df_schema.py` & `onetl-0.8.0/onetl/base/contains_get_df_schema.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/base/path_protocol.py` & `onetl-0.8.0/onetl/base/pure_path_protocol.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,63 +8,92 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+from __future__ import annotations
+
+from typing import Sequence, TypeVar
+
 from typing_extensions import Protocol, runtime_checkable
 
-from onetl.base.path_stat_protocol import PathStatProtocol
+T = TypeVar("T", bound="PurePathProtocol", covariant=True)
 
 
 @runtime_checkable
-class PathProtocol(Protocol):
+class PurePathProtocol(Protocol[T]):
     """
-    Generic protocol for ``pathlib.Path``-like objects.
+    Generic protocol for :obj:`pathlib.PurePath` like objects.
 
-    Includes only minimal set of methods which allow to determine path type (file, directory) and existence
+    Includes only minimal set of methods which allow to get path items, like parent, name, etc
     """
 
-    def is_dir(self) -> bool:
+    def __fspath__(self) -> str:
         """
-        Checks if this path is a directory
+        Get string representation of path
         """
 
-    def is_file(self) -> bool:
+    def __eq__(self, other) -> bool:
         """
-        Checks if this path is a file
+        Check if two paths are equal
         """
 
-    def exists(self) -> bool:
+    def __hash__(self) -> int:
         """
-        Checks if this path exists
+        Get hash value for path
         """
 
+    def __truediv__(self, key) -> T:
+        """
+        Add items to path
+        """
 
-@runtime_checkable
-class PathWithStatsProtocol(Protocol):
-    """
-    Protocol for ``pathlib.Path``-like file objects.
+    def __rtruediv__(self, key) -> T:
+        """
+        Add items to path
+        """
 
-    Includes only minimal set of methods which allow to determine if file exists, or get stats, e.g. size
-    """
+    @property
+    def name(self) -> str:
+        """
+        Get path name
+        """
+
+    @property
+    def parent(self) -> T:
+        """
+        Get parent path
+        """
+
+    @property
+    def parents(self) -> Sequence[T]:
+        """
+        Get parent paths
+        """
+
+    @property
+    def parts(self) -> Sequence[str]:
+        """
+        Get path parts
+        """
 
-    def is_dir(self) -> bool:
+    def is_absolute(self) -> bool:
         """
-        Checks if this path is a directory
+        Checks if this path is absolute
         """
 
-    def is_file(self) -> bool:
+    def match(self, path_pattern) -> bool:
         """
-        Checks if this path is a file
+        Checks if path matches a glob pattern
         """
 
-    def exists(self) -> bool:
+    def relative_to(self, *other) -> T:
         """
-        Checks if this path exists
+        Return the relative path to another path
         """
 
-    def stat(self) -> PathStatProtocol:
+    def joinpath(self, *args) -> T:
         """
-        Returns stats object with file information
+        Add items to path
         """
```

### Comparing `onetl-0.7.2/onetl/base/path_stat_protocol.py` & `onetl-0.8.0/onetl/base/base_file_filter.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,47 +10,38 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from __future__ import annotations
 
-from typing_extensions import Protocol, runtime_checkable
+from abc import ABC, abstractmethod
 
+from onetl.base.path_protocol import PathProtocol
 
-@runtime_checkable
-class PathStatProtocol(Protocol):
+
+class BaseFileFilter(ABC):
     """
-    Protocol for ``os.stat_result``-like objects.
+    Base file filter interface.
+
+    Filters used by several onETL components, including :ref:`file-downloader` and :ref:`file-mover`,
+    to determine if a file should be handled or not.
 
-    Includes only minimal set of fields supported by any file system
+    All filters are stateless.
     """
 
-    @property
-    def st_size(self) -> int:
-        """
-        Size of file, in bytes
+    @abstractmethod
+    def match(self, path: PathProtocol) -> bool:
         """
+        Returns ``True`` if path is matching the filter, ``False`` otherwise
 
-    @property
-    def st_mtime(self) -> float | None:
-        """
-        Unix timestamp of most recent content modification
-        """
+        Examples
+        --------
 
-    @property
-    def st_uid(self) -> str | int | None:
-        """
-        User identifier of the file owner
-        """
+        .. code:: python
 
-    @property
-    def st_gid(self) -> str | int | None:
-        """
-        Group identifier of the file owner
-        """
+            from onetl.impl import LocalPath
 
-    @property
-    def st_mode(self) -> int | None:
-        """
-        File mode bits
+            assert filter.match(LocalPath("/path/to/file.csv"))
+            assert not filter.match(LocalPath("/path/to/excluded.csv"))
+            assert filter.match(LocalPath("/path/to/file.csv"))
         """
```

### Comparing `onetl-0.7.2/onetl/connection/__init__.py` & `onetl-0.8.0/onetl/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/connection/db_connection/clickhouse.py` & `onetl-0.8.0/onetl/connection/db_connection/clickhouse.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/connection/db_connection/db_connection.py` & `onetl-0.8.0/onetl/connection/db_connection/db_connection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/connection/db_connection/dialect_mixins/__init__.py` & `onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/connection/db_connection/dialect_mixins/support_hint_str.py` & `onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_hint_str.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_str.py` & `onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_str.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/connection/db_connection/dialect_mixins/support_where_str.py` & `onetl-0.8.0/onetl/connection/db_connection/dialect_mixins/support_where_str.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/connection/db_connection/greenplum.py` & `onetl-0.8.0/onetl/connection/db_connection/greenplum.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/connection/db_connection/hive.py` & `onetl-0.8.0/onetl/connection/db_connection/hive.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/connection/db_connection/jdbc_connection.py` & `onetl-0.8.0/onetl/connection/db_connection/jdbc_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -567,15 +567,15 @@
         """
         **Lazily** execute SELECT statement **on Spark executor** and return DataFrame.
 
         Same as ``spark.read.jdbc(query)``.
 
         .. note::
 
-            This method does not support :ref:`strategy`, use :obj:`onetl.core.db_reader.db_reader.DBReader` instead
+            This method does not support :ref:`strategy`, use :obj:`onetl.db.db_reader.db_reader.DBReader` instead
 
         .. note::
 
             Statement is executed in read-write connection,
             so if you're calling some functions/procedures with DDL/DML statements inside,
             they can change data in your database.
```

### Comparing `onetl-0.7.2/onetl/connection/db_connection/jdbc_mixin.py` & `onetl-0.8.0/onetl/connection/db_connection/jdbc_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
             Use it **ONLY** to execute queries with **one or just a few returning rows/columns**,
             like ``SELECT COUNT(*) FROM table`` or ``SELECT * FROM table WHERE id = ...``.
 
             This is because all the data is fetched through master host, not in a distributed way
             (even on clustered instances).
             Also the resulting dataframe is stored directly in driver's memory, which is usually quite limited.
 
-            Use :obj:`onetl.core.db_reader.db_reader.DBReader` for reading
+            Use :obj:`onetl.db.db_reader.db_reader.DBReader` for reading
             data from table via Spark executors, or for handling different :ref:`strategy`.
 
         .. note::
 
             Statement is executed in read-only connection, so it cannot change any data in the database.
 
         .. note::
@@ -278,15 +278,15 @@
 
             This is because all the data is fetched through master host, not in a distributed way
             (even on clustered instances).
             Also the resulting dataframe is stored directly in driver's memory, which is usually quite limited.
 
             Please **DO NOT** use this method to execute queries
             like ``INSERT INTO ... VALUES(a, lot, of, values)``,
-            use :obj:`onetl.core.db_writer.db_writer.DBWriter` instead
+            use :obj:`onetl.db.db_writer.db_writer.DBWriter` instead
 
         .. note::
 
             First call of the method opens the connection to a database.
             Call ``.close()`` method to close it, or use context manager to do it automatically.
 
         Parameters
```

### Comparing `onetl-0.7.2/onetl/connection/db_connection/mongodb.py` & `onetl-0.8.0/onetl/connection/db_connection/mongodb.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,15 +545,15 @@
 
             db.collection.aggregate([{"$match": ...}, {"$group": ...}])
 
         but pipeline is executed on Spark executors, in a distributed way.
 
         .. note::
 
-            This method does not support :ref:`strategy`, use :obj:`onetl.core.db_reader.db_reader.DBReader` instead
+            This method does not support :ref:`strategy`, use :obj:`onetl.db.db_reader.db_reader.DBReader` instead
 
         .. note::
 
             Statement is executed in read-write connection,
             so if you're calling some stored functions, you can make changes
             to the data source.
```

### Comparing `onetl-0.7.2/onetl/connection/db_connection/mssql.py` & `onetl-0.8.0/onetl/connection/db_connection/mssql.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/connection/db_connection/mysql.py` & `onetl-0.8.0/onetl/connection/db_connection/mysql.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/connection/db_connection/oracle.py` & `onetl-0.8.0/onetl/connection/db_connection/oracle.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     """Oracle JDBC connection.
 
     Based on Maven package ``com.oracle.database.jdbc:ojdbc8:23.2.0.0``
     (`official Oracle JDBC driver <https://www.oracle.com/cis/database/technologies/appdev/jdbc-downloads.html>`_).
 
     .. dropdown:: Version compatibility
 
-        * Oracle Server versions: 23c, 21c, 19c, 18c, and 12.2
+        * Oracle Server versions: 23c, 21c, 19c, 18c, 12.2 and probably 11.2 (tested, but that's not official).
         * Spark versions: 2.3.x - 3.4.x
         * Java versions: 8 - 17
 
         See `official documentation <https://www.oracle.com/cis/database/technologies/appdev/jdbc-downloads.html>`_.
 
     .. warning::
```

### Comparing `onetl-0.7.2/onetl/connection/db_connection/postgres.py` & `onetl-0.8.0/onetl/connection/db_connection/postgres.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/connection/db_connection/teradata.py` & `onetl-0.8.0/onetl/connection/db_connection/teradata.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/connection/file_connection/file_connection.py` & `onetl-0.8.0/onetl/connection/file_connection/file_connection.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,21 +23,22 @@
 
 from onetl.base import (
     BaseFileConnection,
     BaseFileFilter,
     BaseFileLimit,
     PathStatProtocol,
 )
-from onetl.core.file_filter import match_all_filters
-from onetl.core.file_limit import limits_reached
 from onetl.exception import (
     DirectoryNotEmptyError,
     DirectoryNotFoundError,
+    FileSizeMismatchError,
     NotAFileError,
 )
+from onetl.file.filter import match_all_filters
+from onetl.file.limit import limits_reached, limits_stop_at, reset_limits
 from onetl.impl import (
     FrozenModel,
     LocalPath,
     RemoteDirectory,
     RemoteFile,
     RemotePath,
     path_repr,
@@ -66,23 +67,23 @@
         Examples
         --------
 
         Get directory content and close connection:
 
         .. code:: python
 
-            content = connection.listdir("/mydir")
+            content = connection.list_dir("/mydir")
             assert content
             connection.close()
 
             # or
 
             with connection:
-                content = connection.listdir("/mydir")
-                content = connection.listdir("/mydir/abc")
+                content = connection.list_dir("/mydir")
+                content = connection.list_dir("/mydir/abc")
 
         """
 
         if self._client:
             self._close_client()
 
         self._client = None
@@ -94,15 +95,15 @@
         self.close()
 
     def check(self):
         log.info("|%s| Checking connection availability...", self.__class__.__name__)
         self._log_parameters()
 
         try:
-            self.listdir("/")
+            self.list_dir("/")
             log.info("|%s| Connection is available", self.__class__.__name__)
         except (RuntimeError, ValueError):
             # left validation errors intact
             log.exception("|%s| Connection is unavailable", self.__class__.__name__)
             raise
         except Exception as e:
             log.exception("|%s| Connection is unavailable", self.__class__.__name__)
@@ -124,29 +125,28 @@
         if not self.path_exists(remote_path):
             raise DirectoryNotFoundError(f"Directory '{remote_path}' does not exist")
 
         return self._is_dir(remote_path)
 
     def get_stat(self, path: os.PathLike | str) -> PathStatProtocol:
         remote_path = RemotePath(path)
-
         return self._get_stat(remote_path)
 
-    def get_directory(self, path: os.PathLike | str) -> RemoteDirectory:
+    def resolve_dir(self, path: os.PathLike | str) -> RemoteDirectory:
         is_dir = self.is_dir(path)
         stat = self.get_stat(path)
 
         if not is_dir:
             raise NotADirectoryError(
                 f"{path_repr(RemoteFile(path, stats=stat))} is not a directory",
             )
 
         return RemoteDirectory(path=path, stats=stat)
 
-    def get_file(self, path: os.PathLike | str) -> RemoteFile:
+    def resolve_file(self, path: os.PathLike | str) -> RemoteFile:
         is_file = self.is_file(path)
         stat = self.get_stat(path)
         remote_path = RemoteFile(path=path, stats=stat)
 
         if not is_file:
             raise NotAFileError(f"{path_repr(remote_path)} is not a file")
 
@@ -157,21 +157,21 @@
             "|%s| Reading string with encoding %r and options %r from '%s'",
             self.__class__.__name__,
             encoding,
             kwargs,
             path,
         )
 
-        remote_path = self.get_file(path)
+        remote_path = self.resolve_file(path)
         return self._read_text(remote_path, encoding=encoding, **kwargs)
 
     def read_bytes(self, path: os.PathLike | str, **kwargs) -> bytes:
         log.debug("|%s| Reading bytes with options %r from '%s'", self.__class__.__name__, kwargs, path)
 
-        remote_path = self.get_file(path)
+        remote_path = self.resolve_file(path)
         return self._read_bytes(remote_path, **kwargs)
 
     def write_text(self, path: os.PathLike | str, content: str, encoding: str = "utf-8", **kwargs) -> RemoteFile:
         if not isinstance(content, str):
             raise TypeError(f"content must be str, not '{content.__class__.__name__}'")
 
         log.debug(
@@ -180,117 +180,118 @@
             len(content),
             encoding,
             kwargs,
             path,
         )
 
         remote_path = RemotePath(path)
-        self.mkdir(remote_path.parent)
+        self.create_dir(remote_path.parent)
 
         if self.path_exists(remote_path):
-            file = self.get_file(remote_path)
+            file = self.resolve_file(remote_path)
             log.warning(
                 "|%s| File %s already exists and will be overwritten",
                 self.__class__.__name__,
                 path_repr(file),
             )
 
         self._write_text(remote_path, content=content, encoding=encoding, **kwargs)
 
-        return self.get_file(remote_path)
+        return self.resolve_file(remote_path)
 
     def write_bytes(self, path: os.PathLike | str, content: bytes, **kwargs) -> RemoteFile:
         if not isinstance(content, bytes):
             raise TypeError(f"content must be bytes, not '{content.__class__.__name__}'")
 
         log.debug(
             "|%s| Writing %s with options %e to '%s'",
             self.__class__.__name__,
             naturalsize(len(content)),
             kwargs,
             path,
         )
 
         remote_path = RemotePath(path)
-        self.mkdir(remote_path.parent)
+        self.create_dir(remote_path.parent)
 
         if self.path_exists(remote_path):
-            file = self.get_file(remote_path)
+            file = self.resolve_file(remote_path)
             log.warning(
                 "|%s| File %s already exists and will be overwritten",
                 self.__class__.__name__,
                 path_repr(file),
             )
 
         self._write_bytes(remote_path, content=content, **kwargs)
 
-        return self.get_file(remote_path)
+        return self.resolve_file(remote_path)
 
     def download_file(
         self,
         remote_file_path: os.PathLike | str,
         local_file_path: os.PathLike | str,
         replace: bool = True,
     ) -> LocalPath:
         log.debug(
             "|%s| Downloading file '%s' to local '%s'",
             self.__class__.__name__,
             remote_file_path,
             local_file_path,
         )
 
-        remote_file = self.get_file(remote_file_path)
+        remote_file = self.resolve_file(remote_file_path)
         local_file = LocalPath(local_file_path)
 
         if local_file.exists():
             if not local_file.is_file():
                 raise NotAFileError(f"{path_repr(local_file)} is not a file")
 
             if not replace:
                 raise FileExistsError(f"File {path_repr(local_file)} already exists")
 
-            log.warning("|LocalFS| File %s already exists, overwriting", path_repr(local_file))
+            log.warning("|Local FS| File %s already exists, overwriting", path_repr(local_file))
             local_file.unlink()
 
         log.debug("|Local FS| Creating target directory '%s'", local_file.parent)
         local_file.parent.mkdir(parents=True, exist_ok=True)
         self._download_file(remote_file, local_file)
 
         if local_file.stat().st_size != remote_file.stat().st_size:
-            raise RuntimeError(
+            raise FileSizeMismatchError(
                 f"The size of the downloaded file ({naturalsize(local_file.stat().st_size)}) does not match "
                 f"the size of the file on the source ({naturalsize(remote_file.stat().st_size)})",
             )
 
         log.info("|Local FS| Successfully downloaded file '%s'", local_file)
         return local_file
 
-    def remove_file(self, remote_file_path: os.PathLike | str) -> None:
-        log.debug("|%s| Removing file '%s'", self.__class__.__name__, remote_file_path)
+    def remove_file(self, path: os.PathLike | str) -> bool:
+        log.debug("|%s| Removing file '%s'", self.__class__.__name__, path)
 
-        if not self.path_exists(remote_file_path):
-            log.debug("|%s| File '%s' does not exist, nothing to remove", self.__class__.__name__, remote_file_path)
-            return
+        if not self.path_exists(path):
+            log.debug("|%s| File '%s' does not exist, nothing to remove", self.__class__.__name__, path)
+            return False
 
-        file = self.get_file(remote_file_path)
+        file = self.resolve_file(path)
         log.debug("|%s| File to remove: %s", self.__class__.__name__, path_repr(file))
 
         self._remove_file(file)
         log.info("|%s| Successfully removed file '%s'", self.__class__.__name__, file)
+        return True
 
-    def mkdir(self, path: os.PathLike | str) -> RemoteDirectory:
+    def create_dir(self, path: os.PathLike | str) -> RemoteDirectory:
         log.debug("|%s| Creating directory '%s'", self.__class__.__name__, path)
-        remote_directory = RemotePath(path)
+        remote_dir = RemotePath(path)
 
-        if self.path_exists(remote_directory):
-            return self.get_directory(remote_directory)
+        if self.path_exists(remote_dir):
+            return self.resolve_dir(remote_dir)
 
-        self._mkdir(remote_directory)
-        log.info("|%s| Successfully created directory '%s'", self.__class__.__name__, remote_directory)
-        return self.get_directory(remote_directory)
+        self._create_dir(remote_dir)
+        log.info("|%s| Successfully created directory '%s'", self.__class__.__name__, remote_dir)
+        return self.resolve_dir(remote_dir)
 
     def upload_file(
         self,
         local_file_path: os.PathLike | str,
         remote_file_path: os.PathLike | str,
         replace: bool = False,
     ) -> RemoteFile:
@@ -301,28 +302,28 @@
             raise FileNotFoundError(f"File '{local_file}' does not exist")
 
         if not local_file.is_file():
             raise NotAFileError(f"{path_repr(local_file)} is not a file")
 
         remote_file = RemotePath(remote_file_path)
         if self.path_exists(remote_file):
-            file = self.get_file(remote_file_path)
+            file = self.resolve_file(remote_file_path)
             if not replace:
                 raise FileExistsError(f"File {path_repr(file)} already exists")
 
             log.warning("|%s| File %s already exists, overwriting", self.__class__.__name__, path_repr(file))
             self._remove_file(remote_file)
 
-        self.mkdir(remote_file.parent)
+        self.create_dir(remote_file.parent)
 
         self._upload_file(local_file, remote_file)
-        result = self.get_file(remote_file)
+        result = self.resolve_file(remote_file)
 
         if result.stat().st_size != local_file.stat().st_size:
-            raise RuntimeError(
+            raise FileSizeMismatchError(
                 f"The size of the uploaded file ({naturalsize(result.stat().st_size)}) does not match "
                 f"the size of the file on the source ({naturalsize(local_file.stat().st_size)})",
             )
 
         log.info("|%s| Successfully uploaded file '%s'", self.__class__.__name__, remote_file)
         return result
 
@@ -330,178 +331,171 @@
         self,
         source_file_path: os.PathLike | str,
         target_file_path: os.PathLike | str,
         replace: bool = False,
     ) -> RemoteFile:
         log.debug("|%s| Renaming file '%s' to '%s'", self.__class__.__name__, source_file_path, target_file_path)
 
-        source_file = self.get_file(source_file_path)
+        source_file = self.resolve_file(source_file_path)
         target_file = RemotePath(target_file_path)
 
         if self.path_exists(target_file):
-            file = self.get_file(target_file)
+            file = self.resolve_file(target_file)
             if not replace:
                 raise FileExistsError(f"File {path_repr(file)} already exists")
 
             log.warning("|%s| File %s already exists, overwriting", self.__class__.__name__, path_repr(file))
             self._remove_file(target_file)
 
-        self.mkdir(target_file.parent)
-        self._rename(source_file, target_file)
+        self.create_dir(target_file.parent)
+        self._rename_file(source_file, target_file)
         log.info("|%s| Successfully renamed file '%s' to '%s'", self.__class__.__name__, source_file, target_file)
 
-        return self.get_file(target_file)
+        return self.resolve_file(target_file)
 
-    def listdir(
+    def list_dir(
         self,
-        directory: os.PathLike | str,
+        path: os.PathLike | str,
         filters: Iterable[BaseFileFilter] | None = None,
         limits: Iterable[BaseFileLimit] | None = None,
     ) -> list[RemoteDirectory | RemoteFile]:
-        log.debug("|%s| Listing directory '%s'", self.__class__.__name__, directory)
+        log.debug("|%s| Listing directory '%s'", self.__class__.__name__, path)
+        remote_dir = self.resolve_dir(path)
+        result: list[RemoteDirectory | RemoteFile] = []
 
         filters = filters or []
-        limits = limits or []
-
-        for limit in limits:
-            limit.reset()
+        limits = reset_limits(limits or [])
 
-        remote_directory = self.get_directory(directory)
-        result = []
-
-        for entry in self._scan_entries(remote_directory):
+        for entry in self._scan_entries(remote_dir):
             name = self._extract_name_from_entry(entry)
-            stat = self._extract_stat_from_entry(remote_directory, entry)
+            stat = self._extract_stat_from_entry(remote_dir, entry)
 
-            if self._is_dir_entry(remote_directory, entry):
+            if self._is_dir_entry(remote_dir, entry):
                 path = RemoteDirectory(path=name, stats=stat)
             else:
                 path = RemoteFile(path=name, stats=stat)
 
-            if match_all_filters(filters, path):
+            if match_all_filters(path, filters):
                 result.append(path)
 
-            if limits_reached(limits, path):
+            if limits_stop_at(path, limits):
                 break
 
         return result
 
     def walk(
         self,
-        top: os.PathLike | str,
+        root: os.PathLike | str,
         topdown: bool = True,
         filters: Iterable[BaseFileFilter] | None = None,
         limits: Iterable[BaseFileLimit] | None = None,
     ) -> Iterator[tuple[RemoteDirectory, list[RemoteDirectory], list[RemoteFile]]]:
-        filters = filters or []
-        limits = limits or []
+        root_dir = self.resolve_dir(root)
 
-        for limit in limits:
-            limit.reset()
-
-        yield from self._walk(top, topdown=topdown, filters=filters, limits=limits)
+        filters = filters or []
+        limits = reset_limits(limits or [])
+        yield from self._walk(root_dir, topdown=topdown, filters=filters, limits=limits)
 
-    def rmdir(self, path: os.PathLike | str, recursive: bool = False) -> None:
+    def remove_dir(self, path: os.PathLike | str, recursive: bool = False) -> bool:
         description = "RECURSIVELY" if recursive else "NON-recursively"
         log.debug("|%s| %s removing directory '%s'", self.__class__.__name__, description, path)
-        remote_directory = RemotePath(path)
+        remote_dir = RemotePath(path)
 
-        if not self.path_exists(remote_directory):
+        if not self.path_exists(remote_dir):
             log.debug(
                 "|%s| Directory '%s' does not exist, nothing to remove",
                 self.__class__.__name__,
-                remote_directory,
+                remote_dir,
             )
-            return
+            return False
 
-        directory_info = path_repr(self.get_directory(remote_directory))
-        if self.listdir(remote_directory) and not recursive:
+        directory_info = path_repr(self.resolve_dir(remote_dir))
+        if self.list_dir(remote_dir) and not recursive:
             raise DirectoryNotEmptyError(
                 "|%s| Cannot delete non-empty directory %s",
                 self.__class__.__name__,
                 directory_info,
             )
 
         log.debug("|%s| Directory to remove: %s", self.__class__.__name__, directory_info)
         if recursive:
-            self._rmdir_recursive(remote_directory)
+            self._remove_dir_recursive(remote_dir)
         else:
-            self._rmdir(remote_directory)
+            self._remove_dir(remote_dir)
 
-        log.info("|%s| Successfully removed directory '%s'", self.__class__.__name__, remote_directory)
+        log.info("|%s| Successfully removed directory '%s'", self.__class__.__name__, remote_dir)
+        return True
 
     def _walk(  # noqa: WPS231
         self,
-        top: os.PathLike | str,
+        root: RemoteDirectory,
         topdown: bool,
         filters: Iterable[BaseFileFilter],
         limits: Iterable[BaseFileLimit],
     ) -> Iterator[tuple[RemoteDirectory, list[RemoteDirectory], list[RemoteFile]]]:
         # no need to check nested directories if limit is already reached
-        for limit in limits:
-            if limit.is_reached:
-                return
+        if limits_reached(limits):
+            return
 
-        log.debug("|%s| Walking through directory '%s'", self.__class__.__name__, top)
-        root = self.get_directory(top)
+        log.debug("|%s| Walking through directory '%s'", self.__class__.__name__, root)
         dirs, files = [], []
 
         for entry in self._scan_entries(root):
             name = self._extract_name_from_entry(entry)
             stat = self._extract_stat_from_entry(root, entry)
 
             if self._is_dir_entry(root, entry):
                 if not topdown:
-                    yield from self._walk(top=root / name, topdown=topdown, filters=filters, limits=limits)
+                    yield from self._walk(root=root / name, topdown=topdown, filters=filters, limits=limits)
 
                 path = RemoteDirectory(path=root / name, stats=stat)
-                if match_all_filters(filters, path):
+                if match_all_filters(path, filters):
                     dirs.append(RemoteDirectory(path=name, stats=stat))
 
-                    if limits_reached(limits, path):
+                    if limits_stop_at(path, limits):
                         break
             else:
                 path = RemoteFile(path=root / name, stats=stat)
 
-                if match_all_filters(filters, path):
+                if match_all_filters(path, filters):
                     files.append(RemoteFile(path=name, stats=stat))
 
-                    if limits_reached(limits, path):
+                    if limits_stop_at(path, limits):
                         break
 
         if topdown:
             for name in dirs:
-                yield from self._walk(top=root / name, topdown=topdown, filters=filters, limits=limits)
+                yield from self._walk(root=root / name, topdown=topdown, filters=filters, limits=limits)
 
         log.debug(
             "|%s| Directory '%s' contains %d nested directories and %d files",
             self.__class__.__name__,
             root,
             len(dirs),
             len(files),
         )
         yield root, dirs, files
 
-    def _rmdir_recursive(self, root: RemotePath) -> None:
+    def _remove_dir_recursive(self, root: RemotePath) -> None:
         for entry in self._scan_entries(root):
             name = self._extract_name_from_entry(entry)
             stat = self._extract_stat_from_entry(root, entry)
 
             if self._is_dir_entry(root, entry):
                 path = RemoteDirectory(path=root / name, stats=stat)
                 log.debug("|%s| Directory to remove: %s", self.__class__.__name__, path_repr(path))
-                self._rmdir_recursive(path)
+                self._remove_dir_recursive(path)
                 log.debug("|%s| Successfully removed directory '%s'", self.__class__.__name__, path)
             else:
                 path = RemoteFile(path=root / name, stats=stat)
                 log.debug("|%s| File to remove: %s", self.__class__.__name__, path_repr(path))
                 self._remove_file(path)
                 log.debug("|%s| Successfully removed file '%s'", self.__class__.__name__, path)
 
-        self._rmdir(root)
+        self._remove_dir(root)
 
     @abstractmethod
     def _scan_entries(self, path: RemotePath) -> list:
         """
         The method returns a list that contains entries.
 
         Entry is an object containing information about a path, like file or nested directory.
@@ -709,43 +703,43 @@
         """"""
 
     @abstractmethod
     def _remove_file(self, remote_file_path: RemotePath) -> None:
         """"""
 
     @abstractmethod
-    def _mkdir(self, path: RemotePath) -> None:
+    def _create_dir(self, path: RemotePath) -> None:
         """"""
 
     @abstractmethod
     def _upload_file(self, local_file_path: LocalPath, remote_file_path: RemotePath) -> None:
         """"""
 
     @abstractmethod
-    def _rename(self, source: RemotePath, target: RemotePath) -> None:
+    def _rename_file(self, source: RemotePath, target: RemotePath) -> None:
         """"""
 
     @abstractmethod
-    def _rmdir(self, path: RemotePath) -> None:
+    def _remove_dir(self, path: RemotePath) -> None:
         """"""
 
     @abstractmethod
-    def _read_text(self, path: RemotePath, encoding: str, **kwargs) -> str:
+    def _read_text(self, path: RemotePath, encoding: str) -> str:
         """"""
 
     @abstractmethod
-    def _read_bytes(self, path: RemotePath, **kwargs) -> bytes:
+    def _read_bytes(self, path: RemotePath) -> bytes:
         """"""
 
     @abstractmethod
-    def _write_text(self, path: RemotePath, content: str, encoding: str, **kwargs) -> None:
+    def _write_text(self, path: RemotePath, content: str, encoding: str) -> None:
         """"""
 
     @abstractmethod
-    def _write_bytes(self, path: RemotePath, content: bytes, **kwargs) -> None:
+    def _write_bytes(self, path: RemotePath, content: bytes) -> None:
         """"""
 
     @abstractmethod
     def _is_dir(self, path: RemotePath) -> bool:
         """"""
 
     @abstractmethod
```

### Comparing `onetl-0.7.2/onetl/connection/file_connection/ftp.py` & `onetl-0.8.0/onetl/connection/file_connection/ftp.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,23 @@
 
 import ftplib  # noqa: S402
 import os
 import textwrap
 from logging import getLogger
 from typing import Optional
 
+from etl_entities.instance import Host
+from pydantic import SecretStr
+
+from onetl.base import PathStatProtocol
+from onetl.connection.file_connection.file_connection import FileConnection
+from onetl.connection.file_connection.mixins.rename_dir_mixin import RenameDirMixin
+from onetl.impl import LocalPath, RemotePath
+from onetl.impl.remote_path_stat import RemotePathStat
+
 try:
     from ftputil import FTPHost
     from ftputil import session as ftp_session
 except (ImportError, NameError) as e:
     raise ImportError(
         textwrap.dedent(
             """
@@ -34,26 +43,18 @@
 
             or
                 pip install onetl[files]
             """,
         ).strip(),
     ) from e
 
-from etl_entities.instance import Host
-from pydantic import SecretStr
-
-from onetl.base import PathStatProtocol
-from onetl.connection.file_connection.file_connection import FileConnection
-from onetl.impl import LocalPath, RemotePath
-from onetl.impl.remote_path_stat import RemotePathStat
-
 log = getLogger(__name__)
 
 
-class FTP(FileConnection):
+class FTP(FileConnection, RenameDirMixin):
     """FTP file connection.
 
     Based on `FTPUtil library <https://pypi.org/project/ftputil/>`_.
 
     .. warning::
 
         Since onETL v0.7.0 to use FTP connector you should install package as follows:
@@ -134,30 +135,32 @@
 
     def _is_client_closed(self) -> bool:
         return self._client.closed
 
     def _close_client(self) -> None:
         self._client.close()
 
-    def _rmdir(self, path: RemotePath) -> None:
+    def _remove_dir(self, path: RemotePath) -> None:
         self.client.rmdir(os.fspath(path))
 
     def _upload_file(self, local_file_path: LocalPath, remote_file_path: RemotePath) -> None:
         self.client.upload(os.fspath(local_file_path), os.fspath(remote_file_path))
 
-    def _rename(self, source: RemotePath, target: RemotePath) -> None:
+    def _rename_file(self, source: RemotePath, target: RemotePath) -> None:
         self.client.rename(os.fspath(source), os.fspath(target))
 
+    _rename_dir = _rename_file
+
     def _download_file(self, remote_file_path: RemotePath, local_file_path: LocalPath) -> None:
         self.client.download(os.fspath(remote_file_path), os.fspath(local_file_path))
 
     def _remove_file(self, remote_file_path: RemotePath) -> None:
         self.client.remove(os.fspath(remote_file_path))
 
-    def _mkdir(self, path: RemotePath) -> None:
+    def _create_dir(self, path: RemotePath) -> None:
         self.client.makedirs(os.fspath(path), exist_ok=True)
 
     def _scan_entries(self, path: RemotePath) -> list[str]:
         return self.client.listdir(os.fspath(path))
 
     def _is_dir(self, path: RemotePath) -> bool:
         return self.client.path.isdir(os.fspath(path))
```

### Comparing `onetl-0.7.2/onetl/connection/file_connection/ftps.py` & `onetl-0.8.0/onetl/connection/file_connection/ftps.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/connection/file_connection/hdfs.py` & `onetl-0.8.0/onetl/connection/file_connection/hdfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,24 @@
 
 import os
 import stat
 import textwrap
 from logging import getLogger
 from typing import TYPE_CHECKING, Optional, Tuple
 
+from etl_entities.instance import Cluster, Host
+from pydantic import Field, FilePath, SecretStr, root_validator, validator
+
+from onetl.base import PathStatProtocol
+from onetl.connection.file_connection.file_connection import FileConnection
+from onetl.connection.file_connection.mixins.rename_dir_mixin import RenameDirMixin
+from onetl.connection.kerberos_helpers import kinit
+from onetl.hooks import slot, support_hooks
+from onetl.impl import LocalPath, RemotePath, RemotePathStat
+
 try:
     from hdfs import InsecureClient
 
     if TYPE_CHECKING:
         from hdfs.ext.kerberos import KerberosClient
 except (ImportError, NameError) as err:
     raise ImportError(
@@ -36,28 +46,19 @@
 
             or
                 pip install onetl[files]
             """,
         ).strip(),
     ) from err
 
-from etl_entities.instance import Cluster, Host
-from pydantic import Field, FilePath, SecretStr, root_validator, validator
-
-from onetl.base import PathStatProtocol
-from onetl.connection.file_connection.file_connection import FileConnection
-from onetl.connection.kerberos_helpers import kinit
-from onetl.hooks import slot, support_hooks
-from onetl.impl import LocalPath, RemotePath, RemotePathStat
-
 log = getLogger(__name__)
 ENTRY_TYPE = Tuple[str, dict]
 
 
-class HDFS(FileConnection):
+class HDFS(FileConnection, RenameDirMixin):
     """HDFS file connection.
 
     Powered by `HDFS Python client <https://pypi.org/project/hdfs/>`_.
 
     .. warning::
 
         Since onETL v0.7.0 to use HDFS connector you should install package as follows:
@@ -696,26 +697,28 @@
         # Underlying client does not support closing
         return False
 
     def _close_client(self) -> None:  # NOSONAR
         # Underlying client does not support closing
         pass
 
-    def _rmdir(self, path: RemotePath) -> None:
+    def _remove_dir(self, path: RemotePath) -> None:
         self.client.delete(os.fspath(path), recursive=False)
 
-    def _mkdir(self, path: RemotePath) -> None:
+    def _create_dir(self, path: RemotePath) -> None:
         self.client.makedirs(os.fspath(path))
 
     def _upload_file(self, local_file_path: LocalPath, remote_file_path: RemotePath) -> None:
         self.client.upload(os.fspath(remote_file_path), os.fspath(local_file_path))
 
-    def _rename(self, source: RemotePath, target: RemotePath) -> None:
+    def _rename_file(self, source: RemotePath, target: RemotePath) -> None:
         self.client.rename(os.fspath(source), os.fspath(target))
 
+    _rename_dir = _rename_file
+
     def _download_file(self, remote_file_path: RemotePath, local_file_path: LocalPath) -> None:
         self.client.download(os.fspath(remote_file_path), os.fspath(local_file_path))
 
     def _remove_file(self, remote_file_path: RemotePath) -> None:
         self.client.delete(os.fspath(remote_file_path), recursive=False)
 
     def _scan_entries(self, path: RemotePath) -> list[ENTRY_TYPE]:
```

### Comparing `onetl-0.7.2/onetl/connection/file_connection/s3.py` & `onetl-0.8.0/onetl/connection/file_connection/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,25 +127,25 @@
         values["port"] = 443 if values["protocol"] == "https" else 80
         return values
 
     @property
     def instance_url(self) -> str:
         return f"s3://{self.host}:{self.port}"
 
-    def mkdir(self, path: os.PathLike | str) -> RemoteDirectory:
+    def create_dir(self, path: os.PathLike | str) -> RemoteDirectory:
         # the method is overridden because S3 does not create a directory
         # and the method must return the created directory
 
         log.debug("|%s| Creating directory '%s'", self.__class__.__name__, path)
         remote_directory = RemotePath(path)
 
         if self.path_exists(remote_directory):
-            return self.get_directory(remote_directory)
+            return self.resolve_dir(remote_directory)
 
-        self._mkdir(remote_directory)
+        self._create_dir(remote_directory)
         log.info("|%s| Successfully created directory '%s'", self.__class__.__name__, remote_directory)
         return RemoteDirectory(path=remote_directory, stats=RemotePathStat())
 
     def path_exists(self, path: os.PathLike | str) -> bool:
         remote_path = RemotePath(os.fspath(path))
         if self._is_root(remote_path):
             return True
@@ -207,23 +207,23 @@
         except Exception:  # noqa: B001,E722
             return RemotePathStat()
 
     def _remove_file(self, remote_file_path: RemotePath) -> None:
         path_str = self._delete_absolute_path_slash(remote_file_path)
         self.client.remove_object(self.bucket, path_str)
 
-    def _mkdir(self, path: RemotePath) -> None:
+    def _create_dir(self, path: RemotePath) -> None:
         # in s3 dirs do not exist
         pass
 
     def _upload_file(self, local_file_path: LocalPath, remote_file_path: RemotePath) -> None:
         path_str = self._delete_absolute_path_slash(remote_file_path)
         self.client.fput_object(self.bucket, path_str, os.fspath(local_file_path))
 
-    def _rename(self, source: RemotePath, target: RemotePath) -> None:
+    def _rename_file(self, source: RemotePath, target: RemotePath) -> None:
         source_str = self._delete_absolute_path_slash(source)
         target_str = self._delete_absolute_path_slash(target)
         self.client.copy_object(
             bucket_name=self.bucket,
             object_name=target_str,
             source=commonconfig.CopySource(self.bucket, source_str),
         )
@@ -249,15 +249,15 @@
     def _extract_stat_from_entry(self, top: RemotePath, entry: Object) -> RemotePathStat:
         return RemotePathStat(
             st_size=entry.size if entry.size else 0,
             st_mtime=entry.last_modified.timestamp() if entry.last_modified else None,
             st_uid=entry.owner_name or entry.owner_id,
         )
 
-    def _rmdir(self, path: RemotePath) -> None:
+    def _remove_dir(self, path: RemotePath) -> None:
         # Empty. S3 does not have directories.
         pass
 
     def _read_text(self, path: RemotePath, encoding: str, **kwargs) -> str:
         path_str = self._delete_absolute_path_slash(path)
         file_handler = self.client.get_object(
             self.bucket,
```

### Comparing `onetl-0.7.2/onetl/connection/file_connection/sftp.py` & `onetl-0.8.0/onetl/connection/file_connection/sftp.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,21 @@
 import contextlib
 import os
 import textwrap
 from logging import getLogger
 from stat import S_ISDIR, S_ISREG
 from typing import Optional
 
+from etl_entities.instance import Host
+from pydantic import FilePath, SecretStr
+
+from onetl.connection.file_connection.file_connection import FileConnection
+from onetl.connection.file_connection.mixins.rename_dir_mixin import RenameDirMixin
+from onetl.impl import LocalPath, RemotePath
+
 try:
     from paramiko import ProxyCommand, SSHClient, SSHConfig, WarningPolicy
     from paramiko.sftp_attr import SFTPAttributes
     from paramiko.sftp_client import SFTPClient
     from paramiko.ssh_exception import ConfigParseError
 except (ImportError, NameError) as e:
     raise ImportError(
@@ -37,26 +44,20 @@
 
             or
                 pip install onetl[files]
             """,
         ).strip(),
     ) from e
 
-from etl_entities.instance import Host
-from pydantic import FilePath, SecretStr
-
-from onetl.connection.file_connection.file_connection import FileConnection
-from onetl.impl import LocalPath, RemotePath
-
 SSH_CONFIG_PATH = LocalPath("~/.ssh/config").expanduser().resolve()
 
 log = getLogger(__name__)
 
 
-class SFTP(FileConnection):
+class SFTP(FileConnection, RenameDirMixin):
     """SFTP file connection.
 
     Based on `Paramiko library <https://pypi.org/project/paramiko/>`_.
 
     .. warning::
 
         Since onETL v0.7.0 to use SFTP connector you should install package as follows:
@@ -177,42 +178,44 @@
             if not (self.password or key_file) and host_info.get("identityfile"):
                 key_file = host_info.get("identityfile")[0]
         except ConfigParseError:
             log.exception("Failed to parse SSH config")
 
         return host_proxy, key_file
 
-    def _mkdir(self, path: RemotePath) -> None:
+    def _create_dir(self, path: RemotePath) -> None:
         try:
             self.client.stat(os.fspath(path))
         except Exception:
             for parent in reversed(path.parents):
                 try:  # noqa: WPS505
                     self.client.stat(os.fspath(parent))
                 except Exception:
                     self.client.mkdir(os.fspath(parent))
 
             self.client.mkdir(os.fspath(path))
 
     def _upload_file(self, local_file_path: RemotePath, remote_file_path: RemotePath) -> None:
         self.client.put(os.fspath(local_file_path), os.fspath(remote_file_path))
 
-    def _rename(self, source: RemotePath, target: RemotePath) -> None:
+    def _rename_file(self, source: RemotePath, target: RemotePath) -> None:
         with contextlib.suppress(OSError):
             self.client.posix_rename(os.fspath(source), os.fspath(target))
             return
 
         # posix rename extension is not supported by server
         # if OSError was caused by permissions error, client.rename will raise this exception again
         self.client.rename(os.fspath(source), os.fspath(target))
 
+    _rename_dir = _rename_file
+
     def _download_file(self, remote_file_path: RemotePath, local_file_path: RemotePath) -> None:
         self.client.get(os.fspath(remote_file_path), os.fspath(local_file_path))
 
-    def _rmdir(self, path: RemotePath) -> None:
+    def _remove_dir(self, path: RemotePath) -> None:
         self.client.rmdir(os.fspath(path))
 
     def _remove_file(self, remote_file_path: RemotePath) -> None:
         self.client.remove(os.fspath(remote_file_path))
 
     def _scan_entries(self, path: RemotePath) -> list[SFTPAttributes]:
         return self.client.listdir_attr(os.fspath(path))
```

### Comparing `onetl-0.7.2/onetl/connection/file_connection/webdav.py` & `onetl-0.8.0/onetl/connection/file_connection/webdav.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,22 @@
 import os
 import stat
 import textwrap
 from logging import getLogger
 from ssl import SSLContext
 from typing import Any, Optional, Union
 
+from etl_entities.instance import Host
+from pydantic import DirectoryPath, FilePath, SecretStr, root_validator
+from typing_extensions import Literal
+
+from onetl.connection.file_connection.file_connection import FileConnection
+from onetl.connection.file_connection.mixins.rename_dir_mixin import RenameDirMixin
+from onetl.impl import LocalPath, RemotePath, RemotePathStat
+
 try:
     from webdav3.client import Client
 except (ImportError, NameError) as e:
     raise ImportError(
         textwrap.dedent(
             """
             Cannot import module "webdav3".
@@ -36,26 +44,19 @@
 
             or
                 pip install onetl[files]
             """,
         ).strip(),
     ) from e
 
-from etl_entities.instance import Host
-from pydantic import DirectoryPath, FilePath, SecretStr, root_validator
-from typing_extensions import Literal
-
-from onetl.connection.file_connection.file_connection import FileConnection
-from onetl.impl import LocalPath, RemotePath, RemotePathStat
-
 log = getLogger(__name__)
 DATA_MODIFIED_FORMAT = "%a, %d %b %Y %H:%M:%S GMT"
 
 
-class WebDAV(FileConnection):
+class WebDAV(FileConnection, RenameDirMixin):
     """WebDAV file connection.
 
     Based on `WebdavClient3 library <https://pypi.org/project/webdavclient3/>`_.
 
     .. warning::
 
         Since onETL v0.7.0 to use WebDAV connector you should install package as follows:
@@ -172,34 +173,36 @@
             st_mtime=datetime.datetime.strptime(info["modified"], DATA_MODIFIED_FORMAT).timestamp(),
             st_uid=info["name"],
         )
 
     def _remove_file(self, remote_file_path: RemotePath) -> None:
         self.client.clean(os.fspath(remote_file_path))
 
-    def _mkdir(self, path: RemotePath) -> None:
+    def _create_dir(self, path: RemotePath) -> None:
         for directory in reversed(path.parents):  # from root to nested directory
             if not self.path_exists(directory):
                 self.client.mkdir(os.fspath(directory))
         self.client.mkdir(os.fspath(path))
 
     def _upload_file(self, local_file_path: LocalPath, remote_file_path: RemotePath) -> None:
         self.client.upload_sync(
             local_path=os.fspath(local_file_path),
             remote_path=os.fspath(remote_file_path),
         )
 
-    def _rename(self, source: RemotePath, target: RemotePath) -> None:
+    def _rename_file(self, source: RemotePath, target: RemotePath) -> None:
         res = self.client.resource(os.fspath(source))
         res.move(os.fspath(target))
 
+    _rename_dir = _rename_file
+
     def _scan_entries(self, path: RemotePath) -> list[dict]:
         return self.client.list(os.fspath(path), get_info=True)
 
-    def _rmdir(self, path: RemotePath) -> None:
+    def _remove_dir(self, path: RemotePath) -> None:
         self.client.clean(os.fspath(path))
 
     def _read_text(self, path: RemotePath, encoding: str) -> str:
         res = self.client.resource(os.fspath(path))
         stream = io.BytesIO()
         res.write_to(stream)
```

### Comparing `onetl-0.7.2/onetl/connection/kerberos_helpers.py` & `onetl-0.8.0/onetl/connection/kerberos_helpers.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/core/__init__.py` & `onetl-0.8.0/onetl/file/filter/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,13 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from onetl.core.db_reader import *
-from onetl.core.db_writer import *
-from onetl.core.file_downloader import *
-from onetl.core.file_filter import *
-from onetl.core.file_limit import *
-from onetl.core.file_result import *
-from onetl.core.file_uploader import *
+
+from onetl.file.filter.exclude_dir import ExcludeDir
+from onetl.file.filter.file_hwm import FileHWMFilter
+from onetl.file.filter.glob import Glob
+from onetl.file.filter.match_all_filters import match_all_filters
+from onetl.file.filter.regexp import Regexp
```

### Comparing `onetl-0.7.2/onetl/core/db_reader/__init__.py` & `onetl-0.8.0/onetl/db/db_reader/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from onetl.core.db_reader.db_reader import DBReader
+from onetl.db.db_reader.db_reader import DBReader
```

### Comparing `onetl-0.7.2/onetl/core/db_reader/db_reader.py` & `onetl-0.8.0/onetl/db/db_reader/db_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
 
     Examples
     --------
     Simple Reader creation:
 
     .. code:: python
 
-        from onetl.core import DBReader
+        from onetl.db import DBReader
         from onetl.connection import Postgres
         from pyspark.sql import SparkSession
 
         spark = (
             SparkSession.builder.appName("spark-app-name")
             .config("spark.jars.packages", Postgres.package)
             .getOrCreate()
@@ -220,15 +220,15 @@
         # read data from table "fiddle.dummy"
         df = reader.run()
 
     Reader creation with JDBC options:
 
     .. code:: python
 
-        from onetl.core import DBReader
+        from onetl.db import DBReader
         from onetl.connection import Postgres
         from pyspark.sql import SparkSession
 
         spark = (
             SparkSession.builder.appName("spark-app-name")
             .config("spark.jars.packages", Postgres.package)
             .getOrCreate()
@@ -251,15 +251,15 @@
         # read data from table "fiddle.dummy"
         df = reader.run()
 
     Reader creation with all parameters:
 
     .. code:: python
 
-        from onetl.core import DBReader
+        from onetl.db import DBReader
         from onetl.connection import Postgres
         from pyspark.sql import SparkSession
 
         spark = (
             SparkSession.builder.appName("spark-app-name")
             .config("spark.jars.packages", Postgres.package)
             .getOrCreate()
@@ -287,15 +287,15 @@
         # read data from table "fiddle.dummy"
         df = reader.run()
 
     Incremental Reader:
 
     .. code:: python
 
-        from onetl.core import DBReader
+        from onetl.db import DBReader
         from onetl.connection import Postgres
         from onetl.strategy import IncrementalStrategy
         from pyspark.sql import SparkSession
 
         spark = (
             SparkSession.builder.appName("spark-app-name")
             .config("spark.jars.packages", Postgres.package)
@@ -513,15 +513,15 @@
 
         .. code:: python
 
             df = reader.run()
         """
 
         # avoid circular imports
-        from onetl.core.db_reader.strategy_helper import (
+        from onetl.db.db_reader.strategy_helper import (
             HWMStrategyHelper,
             NonHWMStrategyHelper,
             StrategyHelper,
         )
 
         entity_boundary_log(msg="DBReader starts")
```

### Comparing `onetl-0.7.2/onetl/core/db_reader/strategy_helper.py` & `onetl-0.8.0/onetl/db/db_reader/strategy_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from logging import getLogger
 from typing import TYPE_CHECKING, NoReturn, Optional, Tuple
 
 from etl_entities import HWM, Column, ColumnHWM
 from pydantic import Field, root_validator, validator
 from typing_extensions import Protocol
 
-from onetl.core.db_reader.db_reader import DBReader
+from onetl.db.db_reader.db_reader import DBReader
 from onetl.hwm import Statement
 from onetl.hwm.store import HWMClassRegistry
 from onetl.impl import FrozenModel
 from onetl.strategy.batch_hwm_strategy import BatchHWMStrategy
 from onetl.strategy.hwm_strategy import HWMStrategy
 from onetl.strategy.strategy_manager import StrategyManager
```

### Comparing `onetl-0.7.2/onetl/core/db_writer/__init__.py` & `onetl-0.8.0/onetl/db/db_writer/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from onetl.core.db_writer.db_writer import DBWriter
+from onetl.db.db_writer.db_writer import DBWriter
```

### Comparing `onetl-0.7.2/onetl/core/db_writer/db_writer.py` & `onetl-0.8.0/onetl/db/db_writer/db_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     Examples
     --------
     Simple Writer creation:
 
     .. code:: python
 
         from onetl.connection import Postgres
-        from onetl.core import DBWriter
+        from onetl.db import DBWriter
         from pyspark.sql import SparkSession
 
         spark = (
             SparkSession.builder.appName("spark-app-name")
             .config("spark.jars.packages", Postgres.package)
             .getOrCreate()
         )
@@ -92,15 +92,15 @@
         )
 
     Writer creation with options:
 
     .. code:: python
 
         from onetl.connection import Postgres
-        from onetl.core import DBWriter
+        from onetl.db import DBWriter
         from pyspark.sql import SparkSession
 
         spark = (
             SparkSession.builder.appName("spark-app-name")
             .config("spark.jars.packages", Postgres.package)
             .getOrCreate()
         )
@@ -123,15 +123,15 @@
             options=options,
         )
 
     Writer to Hive with options:
 
     .. code:: python
 
-        from onetl.core import DBWriter
+        from onetl.db import DBWriter
         from onetl.connection import Hive
         from pyspark.sql import SparkSession
 
         spark = SparkSession.builder.appName("spark-app-name").enableHiveSupport().getOrCreate()
 
         hive = Hive(cluster="rnd-dwh", spark=spark)
```

### Comparing `onetl-0.7.2/onetl/core/file_downloader/__init__.py` & `onetl-0.8.0/onetl/core/file_limit/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,9 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from onetl.core.file_downloader.download_result import DownloadResult
-from onetl.core.file_downloader.file_downloader import FileDownloader
+from onetl.core.file_limit.file_limit import FileLimit
```

### Comparing `onetl-0.7.2/onetl/core/file_downloader/download_result.py` & `onetl-0.8.0/onetl/file/file_downloader/download_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from __future__ import annotations
 
 from pydantic import Field
 
-from onetl.core.file_result import FileResult, FileSet
+from onetl.file.file_result import FileResult, FileSet
 from onetl.impl import FailedRemoteFile, LocalPath, RemoteFile, RemotePath
 
 
 class DownloadResult(FileResult):
     """
     Representation of file download result.
 
@@ -35,15 +35,15 @@
     --------
 
     Download files
 
     .. code:: python
 
         from onetl.impl import LocalPath, RemoteFile, FailedLocalFile
-        from onetl.core import FileDownloader, DownloadResult
+        from onetl.file import FileDownloader, DownloadResult
 
         downloader = FileDownloader(local_path="/local", ...)
 
         downloaded_files = downloader.run(
             [
                 "/remote/file1",
                 "/remote/file2",
@@ -51,20 +51,20 @@
                 "/existing/file",
                 "/missing/file",
             ]
         )
 
         assert downloaded_files == DownloadResult(
             successful={
-                RemoteFile("/local/file1"),
-                RemoteFile("/local/file2"),
+                LocalPath("/local/file1"),
+                LocalPath("/local/file2"),
             },
             failed={FailedLocalFile("/failed/file")},
-            skipped={LocalPath("/existing/file")},
-            missing={LocalPath("/missing/file")},
+            skipped={RemoteFile("/existing/file")},
+            missing={RemotePath("/missing/file")},
         )
     """
 
     successful: FileSet[LocalPath] = Field(default_factory=FileSet)
     "File paths (local) which were downloaded successfully"
 
     failed: FileSet[FailedRemoteFile] = Field(default_factory=FileSet)
```

### Comparing `onetl-0.7.2/onetl/core/file_downloader/file_downloader.py` & `onetl-0.8.0/onetl/file/file_downloader/file_downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,47 +10,53 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from __future__ import annotations
 
+import logging
 import os
 import shutil
-from logging import getLogger
-from typing import Iterable, Optional, Tuple, Type
+import warnings
+from typing import Iterable, List, Optional, Tuple, Type
 
 from etl_entities import HWM, FileHWM, RemoteFolder
 from ordered_set import OrderedSet
-from pydantic import validator
+from pydantic import Field, validator
 
 from onetl._internal import generate_temp_path  # noqa: WPS436
 from onetl.base import BaseFileConnection, BaseFileFilter, BaseFileLimit
 from onetl.base.path_protocol import PathProtocol
-from onetl.core.file_downloader.download_result import DownloadResult
-from onetl.core.file_filter import FileHWMFilter
-from onetl.core.file_limit import FileLimit
-from onetl.core.file_result import FileSet
+from onetl.file.file_downloader.download_result import DownloadResult
+from onetl.file.file_set import FileSet
+from onetl.file.filter.file_hwm import FileHWMFilter
 from onetl.hwm.store import HWMClassRegistry
 from onetl.impl import (
     FailedRemoteFile,
     FileWriteMode,
     FrozenModel,
     GenericOptions,
     LocalPath,
     RemoteFile,
     RemotePath,
     path_repr,
 )
-from onetl.log import entity_boundary_log, log_lines, log_options, log_with_indent
+from onetl.log import (
+    entity_boundary_log,
+    log_collection,
+    log_lines,
+    log_options,
+    log_with_indent,
+)
 from onetl.strategy import StrategyManager
 from onetl.strategy.batch_hwm_strategy import BatchHWMStrategy
 from onetl.strategy.hwm_strategy import HWMStrategy
 
-log = getLogger(__name__)
+log = logging.getLogger(__name__)
 
 # source, target, temp
 DOWNLOAD_ITEMS_TYPE = OrderedSet[Tuple[RemotePath, LocalPath, Optional[LocalPath]]]
 
 
 class FileDownloader(FrozenModel):
     """Allows you to download files from a remote source with specified file connection
@@ -66,26 +72,26 @@
 
         It does NOT support direct file transfer between filesystems, like ``FTP -> SFTP``.
         You should use FileDownloader + :ref:`file-uploader` to implement ``FTP -> local dir -> SFTP``.
 
     Parameters
     ----------
     connection : :obj:`onetl.connection.FileConnection`
-        Class which contains File system connection properties. See in FileConnection section.
+        Class which contains File system connection properties. See :ref:`file-connections` section.
 
-    local_path : os.PathLike or str
+    local_path : :obj:`os.PathLike` or :obj:`str`
         Local path where you download files
 
-    source_path : os.PathLike or str, optional, default: ``None``
+    source_path : :obj:`os.PathLike` or :obj:`str`, optional, default: ``None``
         Remote path to download files from.
 
         Could be ``None``, but only if you pass absolute file paths directly to
         :obj:`~run` method
 
-    temp_path : os.PathLike or str, optional, default: ``None``
+    temp_path : :obj:`os.PathLike` or :obj:`str`, optional, default: ``None``
         If set, this path will be used for downloading a file, and then renaming it to the target file path.
         If ``None`` is passed, files are downloaded directly to ``target_path``.
 
         .. warning::
 
             In case of production ETL pipelines, please set a value for ``temp_path`` (NOT ``None``).
             This allows to properly handle download interruption,
@@ -95,20 +101,20 @@
         .. warning::
 
             In case of connections like SFTP or FTP, which can have multiple underlying filesystems,
             please pass to ``temp_path`` path on the SAME filesystem as ``target_path``.
             Otherwise instead of ``rename``, remote OS will move file between filesystems,
             which is NOT atomic operation.
 
-    filter : BaseFileFilter
-        Options of the file filtering. See :obj:`onetl.core.file_filter.file_filter.FileFilter`
+    filters : list of :obj:`BaseFileFilter <onetl.base.base_file_filter.BaseFileFilter>`
+        Return only files/directories matching these filters. See :ref:`file-filters`
 
-    limit : BaseFileLimit
-        Options of the file  limiting. See :obj:`onetl.core.file_limit.file_limit.FileLimit`
-        Default file count limit is 100
+    limits : list of :obj:`BaseFileLimit <onetl.base.base_file_limit.BaseFileLimit>`
+        Apply limits to the list of files/directories, and stop if one of the limits is reached.
+        See :ref:`file-limits`
 
     options : :obj:`~FileDownloader.Options`  | dict | None, default: ``None``
         File downloading options. See :obj:`~FileDownloader.Options`
 
     hwm_type : str | type[HWM] | None, default: ``None``
         HWM type to detect changes in incremental run. See :ref:`file-hwm`
 
@@ -118,15 +124,15 @@
     Examples
     --------
     Simple Downloader creation
 
     .. code:: python
 
         from onetl.connection import SFTP
-        from onetl.core import FileDownloader
+        from onetl.file import FileDownloader
 
         sftp = SFTP(...)
 
         # create downloader
         downloader = FileDownloader(
             connection=sftp,
             source_path="/path/to/remote/source",
@@ -137,41 +143,46 @@
         downloader.run()
 
     Downloader with all parameters
 
     .. code:: python
 
         from onetl.connection import SFTP
-        from onetl.core import FileDownloader, FileFilter, FileLimit
+        from onetl.file import FileDownloader
+        from onetl.file.filter import Glob, ExcludeDir
+        from onetl.file.limit import MaxFilesCount
 
         sftp = SFTP(...)
 
         # create downloader with a bunch of options
         downloader = FileDownloader(
             connection=sftp,
             source_path="/path/to/remote/source",
             local_path="/path/to/local",
             temp_path="/tmp",
-            filter=FileFilter(
-                glob="*.txt",
-                exclude_dirs=["/path/to/remote/source/exclude_dir"],
-            ),
-            limit=FileLimit(count_limit=10),
+            filters=[
+                Glob("*.txt"),
+                ExcludeDir("/path/to/remote/source/exclude_dir"),
+            ],
+            limits=[MaxFilesCount(100)],
             options=FileDownloader.Options(delete_source=True, mode="overwrite"),
         )
 
-        # download files to "/path/to/local"
+        # download files to "/path/to/local",
+        # but only *.txt,
+        # excluding files from "/path/to/remote/source/exclude_dir" directory
+        # and stop before downloading 101 file
         downloader.run()
 
     Incremental download:
 
     .. code:: python
 
         from onetl.connection import SFTP
-        from onetl.core import FileDownloader
+        from onetl.file import FileDownloader
         from onetl.strategy import IncrementalStrategy
 
         sftp = SFTP(...)
 
         # create downloader
         downloader = FileDownloader(
             connection=sftp,
@@ -183,15 +194,15 @@
         # download files to "/path/to/local", but only new ones
         with IncrementalStrategy():
             downloader.run()
 
     """
 
     class Options(GenericOptions):
-        """File downloader options"""
+        """File downloading options"""
 
         mode: FileWriteMode = FileWriteMode.ERROR
         """
         How to handle existing files in the local directory.
 
         Possible values:
             * ``error`` (default) - do nothing, mark file as failed
@@ -209,160 +220,136 @@
 
     connection: BaseFileConnection
 
     local_path: LocalPath
     source_path: Optional[RemotePath] = None
     temp_path: Optional[LocalPath] = None
 
-    filter: Optional[BaseFileFilter] = None
-    limit: Optional[BaseFileLimit] = FileLimit()
+    filters: List[BaseFileFilter] = Field(default_factory=list, alias="filter")
+    limits: List[BaseFileLimit] = Field(default_factory=list, alias="limit")
 
     hwm_type: Optional[Type[FileHWM]] = None
 
     options: Options = Options()
 
-    @validator("local_path", pre=True, always=True)
-    def resolve_local_path(cls, local_path):
-        return LocalPath(local_path).resolve()
-
-    @validator("source_path", pre=True, always=True)
-    def check_source_path(cls, source_path):
-        return RemotePath(source_path) if source_path else None
-
-    @validator("temp_path", pre=True, always=True)
-    def check_temp_path(cls, temp_path):
-        return LocalPath(temp_path).resolve() if temp_path else None
-
-    @validator("hwm_type", pre=True, always=True)
-    def check_hwm_type(cls, hwm_type, values):
-        source_path = values.get("source_path")
-
-        if hwm_type:
-            if not source_path:
-                raise ValueError("If `hwm_type` is passed, `source_path` must be specified")
-
-            if isinstance(hwm_type, str):
-                hwm_type = HWMClassRegistry.get(hwm_type)
-
-            cls._check_hwm_type(hwm_type)
-
-        return hwm_type
-
     def run(self, files: Iterable[str | os.PathLike] | None = None) -> DownloadResult:  # noqa: WPS231
         """
         Method for downloading files from source to local directory.
 
         .. note::
 
             This method can return different results depending on :ref:`strategy`
 
         Parameters
         ----------
 
         files : Iterable[str | os.PathLike] | None, default ``None``
             File list to download.
 
-            If empty, download files from ``source_path``,
+            If empty, download files from ``source_path`` to ``local_path``,
             applying ``filter``, ``limit`` and ``hwm_type`` to each one (if set).
 
-            If not, download **all** input files, **without**
+            If not, download to ``local_path`` **all** input files, **without**
             any filtering, limiting and excluding files covered by :ref:`file-hwm`
 
         Returns
         -------
-        downloaded_files : :obj:`onetl.core.file_downloader.download_result.DownloadResult`
+        downloaded_files : :obj:`DownloadResult <onetl.file.file_downloader.download_result.DownloadResult>`
 
             Download result object
 
         Raises
         -------
-        DirectoryNotFoundError
+        :obj:`onetl.exception.DirectoryNotFoundError`
 
             ``source_path`` does not found
 
         NotADirectoryError
 
             ``source_path`` or ``local_path`` is not a directory
 
         Examples
         --------
 
-        Download files from ``source_path``
+        Download files from ``source_path`` to ``local_path``
 
         .. code:: python
 
             from onetl.impl import RemoteFile, LocalPath
-            from onetl.core import FileDownloader
+            from onetl.file import FileDownloader
 
             downloader = FileDownloader(source_path="/remote", local_path="/local", ...)
             downloaded_files = downloader.run()
 
             assert downloaded_files.successful == {
-                LocalPath("/local/path/file1.txt"),
-                LocalPath("/local/path/file2.txt"),
-                LocalPath("/local/path/nested/file3.txt"),  # directory structure is preserved
+                LocalPath("/local/file1.txt"),
+                LocalPath("/local/file2.txt"),
+                LocalPath("/local/nested/path/file3.txt"),  # directory structure is preserved
             }
-            assert downloaded_files.failed == {FailedRemoteFile("/failed/file")}
-            assert downloaded_files.skipped == {RemoteFile("/existing/file")}
-            assert downloaded_files.missing == {RemotePath("/missing/file")}
+            assert downloaded_files.failed == {FailedRemoteFile("/remote/failed.file")}
+            assert downloaded_files.skipped == {RemoteFile("/remote/already.exists")}
+            assert downloaded_files.missing == {RemotePath("/remote/missing.file")}
 
         Download only certain files from ``source_path``
 
         .. code:: python
 
             from onetl.impl import RemoteFile, LocalPath
-            from onetl.core import FileDownloader
+            from onetl.file import FileDownloader
 
             downloader = FileDownloader(source_path="/remote", local_path="/local", ...)
 
+            # paths could be relative or absolute, but all should be in "/remote"
             downloaded_files = downloader.run(
                 [
-                    "/remote/path/file1.txt",
-                    "/remote/path/nested/file3.txt",
-                    # excluding "/remote/path/file2.txt"
+                    "/remote/file1.txt",
+                    "/remote/nested/path/file3.txt",
+                    # excluding "/remote/file2.txt"
                 ]
             )
 
             assert downloaded_files.successful == {
-                LocalPath("/local/path/file1.txt"),
-                LocalPath("/local/path/nested/file3.txt"),  # directory structure is preserved
+                LocalPath("/local/file1.txt"),
+                LocalPath("/local/nested/path/file3.txt"),  # directory structure is preserved
             }
             assert not downloaded_files.failed
             assert not downloaded_files.skipped
             assert not downloaded_files.missing
 
         Download certain files from any folder
 
         .. code:: python
 
             from onetl.impl import RemoteFile, LocalPath
-            from onetl.core import FileDownloader
+            from onetl.file import FileDownloader
 
             downloader = FileDownloader(local_path="/local", ...)  # no source_path set
 
+            # only absolute paths
             downloaded_files = downloader.run(
                 [
-                    "/remote/path/file1.txt",
-                    "/remote/path/nested/file3.txt",
+                    "/remote/file1.txt",
+                    "/any/nested/path/file2.txt",
                 ]
             )
 
             assert downloaded_files.successful == {
-                LocalPath("/local/path/file1.txt"),
-                LocalPath("/local/path/file3.txt"),  # directory structure is not preserved
+                LocalPath("/local/file1.txt"),
+                LocalPath("/local/file2.txt"),
+                # directory structure is NOT preserved without source_path
             }
             assert not downloaded_files.failed
             assert not downloaded_files.skipped
             assert not downloaded_files.missing
         """
 
         self._check_strategy()
 
         if files is None and not self.source_path:
-            raise ValueError("Neither file list nor ``source_path`` are passed")
+            raise ValueError("Neither file list nor `source_path` are passed")
 
         self._log_options(files)
 
         # Check everything
         self._check_local_path()
         self.connection.check()
         log_with_indent("")
@@ -401,23 +388,23 @@
 
         self._log_result(result)
         return result
 
     def view_files(self) -> FileSet[RemoteFile]:
         """
         Get file list in the ``source_path``,
-        after ``filter``, ``limit`` and ``hwm`` applied (if any)
+        after ``filter``, ``limit`` and ``hwm`` applied (if any).
 
         .. note::
 
             This method can return different results depending on :ref:`strategy`
 
         Raises
         -------
-        DirectoryNotFoundError
+        :obj:`onetl.exception.DirectoryNotFoundError`
 
             ``source_path`` does not found
 
         NotADirectoryError
 
             ``source_path`` is not a directory
 
@@ -430,54 +417,115 @@
         --------
 
         View files
 
         .. code:: python
 
             from onetl.impl import RemoteFile
-            from onetl.core import FileDownloader
+            from onetl.file import FileDownloader
 
-            downloader = FileDownloader(source_path="/remote/path", ...)
+            downloader = FileDownloader(source_path="/remote", ...)
 
             view_files = downloader.view_files()
 
             assert view_files == {
-                RemoteFile("/remote/path/file1.txt"),
-                RemoteFile("/remote/path/file3.txt"),
-                RemoteFile("/remote/path/nested/file3.txt"),
+                RemoteFile("/remote/file1.txt"),
+                RemoteFile("/remote/file3.txt"),
+                RemoteFile("/remote/nested/file3.txt"),
             }
         """
 
         log.info("|%s| Getting files list from path '%s'", self.connection.__class__.__name__, self.source_path)
 
         self._check_source_path()
         result = FileSet()
 
-        filters = []
-        if self.filter:
-            filters.append(self.filter)
+        filters = self.filters.copy()
         if self.hwm_type:
             filters.append(FileHWMFilter(hwm=self._init_hwm()))
 
-        limits = []
-        if self.limit:
-            limits.append(self.limit)
-
         try:
-            for root, _dirs, files in self.connection.walk(self.source_path, filters=filters, limits=limits):
+            for root, _dirs, files in self.connection.walk(self.source_path, filters=filters, limits=self.limits):
                 for file in files:
                     result.append(RemoteFile(path=root / file, stats=file.stats))
 
         except Exception as e:
             raise RuntimeError(
                 f"Couldn't read directory tree from remote dir '{self.source_path}'",
             ) from e
 
         return result
 
+    @validator("local_path", pre=True, always=True)
+    def _resolve_local_path(cls, local_path):
+        return LocalPath(local_path).resolve()
+
+    @validator("source_path", pre=True, always=True)
+    def _validate_source_path(cls, source_path):
+        return RemotePath(source_path) if source_path else None
+
+    @validator("temp_path", pre=True, always=True)
+    def _validate_temp_path(cls, temp_path):
+        return LocalPath(temp_path).resolve() if temp_path else None
+
+    @validator("hwm_type", pre=True, always=True)
+    def _validate_hwm_type(cls, hwm_type, values):
+        source_path = values.get("source_path")
+
+        if hwm_type:
+            if not source_path:
+                raise ValueError("If `hwm_type` is passed, `source_path` must be specified")
+
+            if isinstance(hwm_type, str):
+                hwm_type = HWMClassRegistry.get(hwm_type)
+
+            cls._check_hwm_type(hwm_type)
+
+        return hwm_type
+
+    @validator("filters", pre=True)
+    def _validate_filters(cls, filters):
+        if filters is None:
+            warnings.warn(
+                "filter=None is deprecated in v0.8.0, use filters=[] instead",
+                UserWarning,
+                stacklevel=3,
+            )
+            return []
+
+        if not isinstance(filters, list):
+            warnings.warn(
+                "filter=... is deprecated in v0.8.0, use filters=[...] instead",
+                UserWarning,
+                stacklevel=3,
+            )
+            filters = [filters]
+
+        return filters
+
+    @validator("limits", pre=True)
+    def _validate_limits(cls, limits):
+        if limits is None:
+            warnings.warn(
+                "limit=None is deprecated in v0.8.0, use limits=[] instead",
+                UserWarning,
+                stacklevel=3,
+            )
+            return []
+
+        if not isinstance(limits, list):
+            warnings.warn(
+                "limit=... is deprecated in v0.8.0, use limits=[...] instead",
+                UserWarning,
+                stacklevel=3,
+            )
+            limits = [limits]
+
+        return limits
+
     def _check_strategy(self):
         strategy = StrategyManager.get_current()
 
         if self.hwm_type:
             if not isinstance(strategy, HWMStrategy):
                 raise ValueError("`hwm_type` cannot be used in snapshot strategy.")
             elif getattr(strategy, "offset", None):  # this check should be somewhere in IncrementalStrategy,
@@ -511,37 +559,35 @@
         entity_boundary_log(msg="FileDownloader starts")
 
         log.info("|%s| -> |Local FS| Downloading files using parameters:", self.connection.__class__.__name__)
         log_with_indent("source_path = %s", f"'{self.source_path}'" if self.source_path else "None")
         log_with_indent("local_path = '%s'", self.local_path)
         log_with_indent("temp_path = '%s'", f"'{self.temp_path}'" if self.temp_path else "None")
 
-        if self.filter is not None:
-            log_with_indent("filter:")
-            self.filter.log_options(indent=4)
+        if self.filters:
+            log_collection("filters", self.filters)
         else:
-            log_with_indent("filter = None")
+            log_with_indent("filters = []")
 
-        if self.limit is not None:
-            log_with_indent("limit:")
-            self.limit.log_options(indent=4)
+        if self.limits:
+            log_collection("limits", self.limits)
         else:
-            log_with_indent("limit = None")
+            log_with_indent("limits = []")
 
         log_options(self.options.dict(by_alias=True))
 
         if self.options.delete_source:
             log.warning("|%s| SOURCE FILES WILL BE PERMANENTLY DELETED AFTER DOWNLOADING !!!", self.__class__.__name__)
 
         if self.options.mode == FileWriteMode.DELETE_ALL:
             log.warning("|%s| LOCAL DIRECTORY WILL BE CLEANED UP BEFORE DOWNLOADING FILES !!!", self.__class__.__name__)
 
         if files and self.source_path:
             log.warning(
-                "|%s| Passed both ``source_path`` and files list at the same time. Using explicit files list",
+                "|%s| Passed both `source_path` and files list at the same time. Using explicit files list",
                 self.__class__.__name__,
             )
 
     def _validate_files(  # noqa: WPS231
         self,
         remote_files: Iterable[os.PathLike | str],
         current_temp_dir: LocalPath | None,
@@ -552,15 +598,15 @@
             remote_file_path = file if isinstance(file, PathProtocol) else RemotePath(file)
             remote_file = remote_file_path
             tmp_file: LocalPath | None = None
 
             if not self.source_path:
                 # Download into a flat structure
                 if not remote_file_path.is_absolute():
-                    raise ValueError("Cannot pass relative file path with empty ``source_path``")
+                    raise ValueError("Cannot pass relative file path with empty `source_path`")
 
                 filename = remote_file_path.name
                 local_file = self.local_path / filename
                 if current_temp_dir:
                     tmp_file = current_temp_dir / filename  # noqa: WPS220
             else:
                 # Download according to source folder structure
@@ -577,22 +623,22 @@
                     if current_temp_dir:
                         tmp_file = current_temp_dir / remote_file_path  # noqa: WPS220
                 else:
                     # Wrong path (not relative path and source path not in the path to the file)
                     raise ValueError(f"File path '{remote_file}' does not match source_path '{self.source_path}'")
 
             if self.connection.path_exists(remote_file):
-                self.connection.get_file(remote_file)
+                remote_file = self.connection.resolve_file(remote_file)
 
             result.add((remote_file, local_file, tmp_file))
 
         return result
 
     def _check_source_path(self):
-        self.connection.get_directory(self.source_path)
+        self.connection.resolve_dir(self.source_path)
 
     def _check_local_path(self):
         if self.local_path.exists() and not self.local_path.is_dir():
             raise NotADirectoryError(f"{path_repr(self.local_path)} is not a directory")
 
         self.local_path.mkdir(exist_ok=True, parents=True)
 
@@ -634,38 +680,38 @@
     ) -> None:
         if not self.connection.path_exists(source_file):
             log.warning("|%s| Missing file '%s', skipping", self.__class__.__name__, source_file)
             result.missing.add(source_file)
             return
 
         try:
-            remote_file = self.connection.get_file(source_file)
+            remote_file = self.connection.resolve_file(source_file)
 
             replace = False
             if local_file.exists():
                 if self.options.mode == FileWriteMode.ERROR:
                     raise FileExistsError(f"File {path_repr(local_file)} already exists")
 
                 if self.options.mode == FileWriteMode.IGNORE:
-                    log.warning("|LocalFS| File %s already exists, skipping", path_repr(local_file))
+                    log.warning("|Local FS| File %s already exists, skipping", path_repr(local_file))
                     result.skipped.add(remote_file)
                     return
 
                 replace = True
 
             if tmp_file:
                 # Files are loaded to temporary directory before moving them to target dir.
                 # This prevents operations with partly downloaded files
 
                 self.connection.download_file(remote_file, tmp_file, replace=replace)
 
                 # remove existing file only after new file is downloaded
                 # to avoid issues then there is no free space to download new file, but existing one is already gone
                 if replace and local_file.exists():
-                    log.warning("|LocalFS| File %s already exists, overwriting", path_repr(local_file))
+                    log.warning("|Local FS| File %s already exists, overwriting", path_repr(local_file))
                     local_file.unlink()
 
                 local_file.parent.mkdir(parents=True, exist_ok=True)
                 shutil.move(tmp_file, local_file)
             else:
                 # Direct download
                 self.connection.download_file(remote_file, local_file, replace=replace)
@@ -678,20 +724,27 @@
             # Delete Remote
             if self.options.delete_source:
                 self.connection.remove_file(remote_file)
 
             result.successful.add(local_file)
 
         except Exception as e:
-            log.exception(
-                "|%s| Couldn't download file from source dir: %s",
-                self.__class__.__name__,
-                e,
-                exc_info=False,
-            )
+            if log.isEnabledFor(logging.DEBUG):
+                log.exception(
+                    "|%s| Couldn't download file from source dir",
+                    self.__class__.__name__,
+                    exc_info=e,
+                )
+            else:
+                log.exception(
+                    "|%s| Couldn't download file from source dir: %s",
+                    self.__class__.__name__,
+                    e,
+                    exc_info=False,
+                )
             result.failed.add(FailedRemoteFile(path=remote_file.path, stats=remote_file.stats, exception=e))
 
     def _remove_temp_dir(self, temp_dir: LocalPath) -> None:
         log.info("|Local FS| Removing temp directory '%s'", temp_dir)
 
         try:
             shutil.rmtree(temp_dir)
```

### Comparing `onetl-0.7.2/onetl/core/file_filter/__init__.py` & `onetl-0.8.0/onetl/file/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from onetl.core.file_filter.file_filter import FileFilter
-from onetl.core.file_filter.file_hwm_filter import FileHWMFilter
-from onetl.core.file_filter.match_all_filters import match_all_filters
+from onetl.file.file_downloader import DownloadResult, FileDownloader
+from onetl.file.file_mover import FileMover, MoveResult
+from onetl.file.file_uploader import FileUploader, UploadResult
```

### Comparing `onetl-0.7.2/onetl/core/file_filter/file_filter.py` & `onetl-0.8.0/onetl/core/file_filter/file_filter.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,26 +13,39 @@
 #  limitations under the License.
 
 from __future__ import annotations
 
 import glob
 import os
 import re
+import textwrap
+import warnings
 from typing import List, Optional, Union
 
+from deprecated import deprecated
 from pydantic import Field, root_validator, validator
 
 from onetl.base import BaseFileFilter, PathProtocol
 from onetl.impl import FrozenModel, RemotePath
 from onetl.log import log_with_indent
 
 
+@deprecated(
+    version="0.8.0",
+    reason="Use Glob, Regexp or ExcludeDir instead. Will be removed in 1.0.0",
+    action="ignore",
+)
 class FileFilter(BaseFileFilter, FrozenModel):
     r"""Filter files or directories by their path.
 
+    .. deprecated:: 0.8.0
+
+        Use :obj:`Glob <onetl.file.filter.glob.Glob>`, :obj:`Regexp <onetl.file.filter.regexp.Regexp>`
+        or :obj:`ExcludeDir <onetl.file.filter.exclude_dir.ExcludeDir>` instead.
+
     Parameters
     ----------
 
     glob : str | None, default ``None``
 
         Pattern (e.g. ``*.csv``) for which any **file** (only file) path should match
 
@@ -58,38 +71,46 @@
     Examples
     --------
 
     Create exclude_dir filter:
 
     .. code:: python
 
+        from onetl.core import FileFilter
+
         file_filter = FileFilter(exclude_dirs=["/export/news_parse/exclude_dir"])
 
     Create glob filter:
 
     .. code:: python
 
+        from onetl.core import FileFilter
+
         file_filter = FileFilter(glob="*.csv")
 
     Create regexp filter:
 
     .. code:: python
 
+        from onetl.core import FileFilter
+
         file_filter = FileFilter(regexp=r"\d+\.csv")
 
         # or
 
         import re
 
         file_filter = FileFilter(regexp=re.compile("\d+\.csv"))
 
     Not allowed:
 
     .. code:: python
 
+        from onetl.core import FileFilter
+
         FileFilter()  # will raise ValueError, at least one argument should be passed
     """
 
     class Config:
         arbitrary_types_allowed = True
 
     glob: Optional[str] = None
@@ -124,21 +145,70 @@
     @root_validator
     def disallow_both_glob_and_regexp(cls, value: dict) -> dict:
         if value.get("glob") and value.get("regexp"):
             raise ValueError("Only one of `glob`, `regexp` fields can passed, not both")
 
         return value
 
+    @root_validator
+    def log_deprecated(cls, value: dict) -> dict:
+        imports = []
+        old_filters = []
+        new_filters = []
+        glob = value.get("glob")  # noqa: WPS442
+        if glob is not None:
+            imports.append("Glob")
+            old_filters.append(f"glob={glob!r}")
+            new_filters.append(f"Glob({glob!r})")
+
+        regexp = value.get("regexp")
+        if regexp is not None:
+            imports.append("Regexp")
+            old_filters.append(f"regexp={regexp.pattern!r}")
+            new_filters.append(f"Regexp({regexp.pattern!r})")
+
+        exclude_dirs = value.get("exclude_dirs")
+        if exclude_dirs:
+            imports.append("ExcludeDir")
+            exclude_dirs_str = [repr(os.fspath(exclude_dir)) for exclude_dir in exclude_dirs]
+            old_filters.append(f"exclude_dirs=[{', '.join(exclude_dirs_str)}]")
+            new_filters.extend(f"ExcludeDir({item})" for item in exclude_dirs_str)
+
+        if not imports:
+            return value
+
+        message = f"""
+            Using FileFilter is deprecated since v0.8.0 and will be removed in v1.0.0.
+
+            Please replace:
+                from onetl.core import FileFilter
+
+                filter=FileFilter({', '.join(old_filters)})
+
+            With:
+                from onetl.file.filter import {', '.join(imports)}
+
+                filters=[{', '.join(new_filters)}]
+        """
+
+        warnings.warn(
+            textwrap.dedent(message).strip(),
+            category=UserWarning,
+            stacklevel=3,  # 1 is current method, 2 is BaseModel internals, 3 is user code
+        )
+        return value
+
     def match(self, path: PathProtocol) -> bool:
         """False means it does not match the template by which you want to receive files"""
 
         if self.exclude_dirs:
-            path = path if path.is_dir() else path.parent
             for exclude_dir in self.exclude_dirs:
-                if exclude_dir in path.parents or exclude_dir == path:
+                if path.is_dir() and exclude_dir == path:
+                    return False
+                if exclude_dir in path.parents:
                     return False
 
         if self.glob and path.is_file():
             return path.match(self.glob)
 
         if self.regexp and path.is_file():
             return self.regexp.search(os.fspath(path)) is not None
```

### Comparing `onetl-0.7.2/onetl/core/file_filter/file_hwm_filter.py` & `onetl-0.8.0/onetl/file/filter/file_hwm.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,41 +14,40 @@
 
 from __future__ import annotations
 
 from etl_entities import FileHWM
 
 from onetl.base import BaseFileFilter, PathProtocol
 from onetl.impl import FrozenModel
-from onetl.log import log_with_indent
 
 
 class FileHWMFilter(BaseFileFilter, FrozenModel):
-    """Filter files which are not covered by FileHWM
+    """Filter files which are not covered by FileHWM.
+
+    .. warning::
+
+        Only for onETL internal use.
 
     Parameters
     ----------
 
-    hwm : FileHWM
+    hwm : :obj:`etl_entities.FileHWM`
 
-        :obj:`etl_entities.FileHWM` instance
+        File HWM instance
     """
 
     class Config:
         arbitrary_types_allowed = True
 
     hwm: FileHWM
 
     def match(self, path: PathProtocol) -> bool:
         if path.is_dir():
             return True
 
         return not self.hwm.covers(path)
 
-    def log_options(self, indent: int = 0):
-        log_with_indent("hwm_type = %s", self.hwm.__class__.__name__, indent=indent)
-        log_with_indent("qualified_name = %r", self.hwm.qualified_name, indent=indent)
-
     def __str__(self):
         return self.hwm.qualified_name
 
     def __repr__(self):
         return f"{self.hwm.__class__.__name__}(qualified_name={self.hwm.qualified_name!r})"
```

### Comparing `onetl-0.7.2/onetl/core/file_limit/__init__.py` & `onetl-0.8.0/onetl/file/file_downloader/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from onetl.core.file_limit.file_limit import FileLimit
-from onetl.core.file_limit.limits_reached import limits_reached
+from onetl.file.file_downloader.download_result import DownloadResult
+from onetl.file.file_downloader.file_downloader import FileDownloader
```

### Comparing `onetl-0.7.2/onetl/core/file_limit/file_limit.py` & `onetl-0.8.0/onetl/core/file_limit/file_limit.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,24 +11,32 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from __future__ import annotations
 
 import logging
+import textwrap
+import warnings
+
+from pydantic import validator
 
 from onetl.base import BaseFileLimit, PathProtocol
 from onetl.impl import FrozenModel
 from onetl.log import log_with_indent
 
 log = logging.getLogger(__name__)
 
 
 class FileLimit(BaseFileLimit, FrozenModel):
-    """Limits the number of uploaded files
+    """Limits the number of downloaded files.
+
+    .. deprecated:: 0.8.0
+
+        Use :obj:`MaxFilesCount <onetl.file.limit.max_files_count.MaxFilesCount>` instead.
 
     Parameters
     ----------
 
     count_limit : int, default = 100
 
         Number of downloaded files at a time.
@@ -36,26 +44,29 @@
     Examples
     --------
 
     Create a FileLimit object and set the amount in it:
 
     .. code:: python
 
+        from onetl.core import FileLimit
+
         limit = FileLimit(count_limit=1500)
 
-    If you create a :obj:`onetl.core.file_downloader.file_downloader.FileDownloader` object without
+    If you create a :obj:`onetl.file.file_downloader.file_downloader.FileDownloader` object without
     specifying the limit option, it will download with a limit of 100 files.
     """
 
     count_limit: int = 100
 
     _counter: int = 0
 
     def reset(self):
         self._counter = 0
+        return self
 
     def stops_at(self, path: PathProtocol) -> bool:
         if self.is_reached:
             return True
 
         if path.is_dir():
             return False
@@ -67,7 +78,30 @@
     @property
     def is_reached(self) -> bool:
         return self._counter >= self.count_limit
 
     def log_options(self, indent: int = 0):
         for key, value in self.dict(by_alias=True).items():  # noqa: WPS528
             log_with_indent("%s = %r", key, value, indent=indent)
+
+    @validator("count_limit")
+    def log_deprecated(cls, value):
+        message = f"""
+            Using FileLimit is deprecated since v0.8.0 and will be removed in v1.0.0.
+
+            Please replace:
+                from onetl.core import FileLimit
+
+                limit=FileLimit(count_limit={value})
+
+            With:
+                from onetl.file.limit import MaxFilesCount
+
+                limits=[MaxFilesCount({value})]
+        """
+
+        warnings.warn(
+            textwrap.dedent(message).strip(),
+            category=UserWarning,
+            stacklevel=3,  # 1 is current method, 2 is BaseModel internals, 3 is user code
+        )
+        return value
```

### Comparing `onetl-0.7.2/onetl/core/file_limit/limits_reached.py` & `onetl-0.8.0/onetl/file/limit/reset_limits.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,26 +14,45 @@
 
 from __future__ import annotations
 
 import logging
 from typing import Iterable
 
 from onetl.base import BaseFileLimit
-from onetl.impl import RemotePath
 
 log = logging.getLogger(__name__)
 
 
-def limits_reached(limits: Iterable[BaseFileLimit], path: RemotePath) -> bool:
-    if not limits:
-        return False
-
-    reached = []
-    for limit in limits:
-        if limit.stops_at(path):
-            reached.append(limit)
-
-    if reached:
-        log.debug("|FileLimit| Limits %r are reached", reached)
-        return True
+def reset_limits(limits: Iterable[BaseFileLimit]) -> list[BaseFileLimit]:
+    """
+    Reset limits state.
 
-    return False
+    Parameters
+    ----------
+    limits : Iterable of :obj:`onetl.base.base_file_limit.BaseFileLimit`
+        Limits to reset.
+
+    Returns
+    -------
+    List with limits, but with reset state.
+
+    List may contain original filters with reset state, or new copies.
+    This is an implementation detail of :obj:`reset <onetl.base.base_file_limit.BaseFileLimit.reset>` method.
+
+    Examples
+    --------
+
+    .. code:: python
+
+        from onetl.file.limit import MaxFilesCount, limits_reached, reset_limits
+        from onetl.impl import LocalPath
+
+        limits = [MaxFilesCount(1)]
+
+        assert not limits_reached(limits)
+        # do something
+        assert limits_reached(limits)
+
+        new_limits = reset_limits(limits)
+        assert not limits_reached(new_limits)
+    """
+    return [limit.reset() for limit in limits]
```

### Comparing `onetl-0.7.2/onetl/core/file_result/__init__.py` & `onetl-0.8.0/onetl/file/file_uploader/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from onetl.core.file_result.file_result import FileResult, GenericPath
-from onetl.core.file_result.file_set import FileSet
+from onetl.file.file_uploader.file_uploader import FileUploader
+from onetl.file.file_uploader.upload_result import UploadResult
```

### Comparing `onetl-0.7.2/onetl/core/file_result/file_result.py` & `onetl-0.8.0/onetl/file/file_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from __future__ import annotations
 
 import os
-from typing import Iterable, TypeVar
+from typing import Iterable
 
 from humanize import naturalsize
 from pydantic import Field, validator
 
-from onetl.core.file_result.file_set import FileSet
+from onetl.base import PurePathProtocol
 from onetl.exception import (
     EmptyFilesError,
     FailedFilesError,
     MissingFilesError,
     SkippedFilesError,
 )
+from onetl.file.file_set import FileSet
 from onetl.impl import BaseModel
 
-GenericPath = TypeVar("GenericPath", bound=os.PathLike)
 INDENT = " " * 4
 
 
 class FileResult(BaseModel):
     """
     Result of some file manipulation process, e.g. download, upload, etc.
 
@@ -41,42 +41,42 @@
 
     * :obj`successful`
     * :obj`failed`
     * :obj`skipped`
     * :obj`missing`
     """
 
-    successful: FileSet[GenericPath] = Field(default_factory=FileSet)
+    successful: FileSet[PurePathProtocol] = Field(default_factory=FileSet)
     "Successfully handled files"
 
-    failed: FileSet[GenericPath] = Field(default_factory=FileSet)
+    failed: FileSet[PurePathProtocol] = Field(default_factory=FileSet)
     "File paths which were handled with some failures"
 
-    skipped: FileSet[GenericPath] = Field(default_factory=FileSet)
+    skipped: FileSet[PurePathProtocol] = Field(default_factory=FileSet)
     "File paths which were skipped because of some reason"
 
-    missing: FileSet[GenericPath] = Field(default_factory=FileSet)
+    missing: FileSet[PurePathProtocol] = Field(default_factory=FileSet)
     "Unknown paths which cannot be handled"
 
     @validator("successful", "failed", "skipped", "missing")
-    def validate_container(cls, value: Iterable[GenericPath]) -> FileSet[GenericPath]:
+    def validate_container(cls, value: Iterable[PurePathProtocol]) -> FileSet[PurePathProtocol]:
         return FileSet(value)
 
     @property
     def successful_count(self) -> int:
         """
         Get number of successful files
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import LocalPath
-            from onet.core import FileResult
+            from onet.file.file_result import FileResult
 
             file_result = FileResult(
                 successful={LocalPath("/some/file"), LocalPath("/some/another.file")},
             )
 
             assert file_result.successful_count == 2
         """
@@ -90,15 +90,15 @@
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import RemoteFile
-            from onet.core import FileResult
+            from onet.file.file_result import FileResult
 
             file_result = FileResult(
                 failed={RemoteFile("/some/file"), RemoteFile("/some/another.file")},
             )
 
             assert file_result.failed_count == 2
         """
@@ -112,15 +112,15 @@
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import LocalPath
-            from onet.core import FileResult
+            from onet.file.file_result import FileResult
 
             file_result = FileResult(
                 skipped={LocalPath("/some/file"), LocalPath("/some/another.file")},
             )
 
             assert file_result.skipped_count == 2
         """
@@ -134,15 +134,15 @@
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import LocalPath
-            from onet.core import FileResult
+            from onet.file.file_result import FileResult
 
             file_result = FileResult(
                 missing={LocalPath("/some/file"), LocalPath("/some/another.file")},
             )
 
             assert file_result.missing_count == 2
         """
@@ -156,15 +156,15 @@
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import RemoteFile, LocalPath
-            from onet.core import FileResult
+            from onet.file.file_result import FileResult
 
             file_result = FileResult(
                 successful={LocalPath("/local/file"), LocalPath("/local/another.file")},
                 failed={RemoteFile("/remote/file"), RemoteFile("/remote/another.file")},
                 skipped={LocalPath("/skipped/file")},
                 missing={LocalPath("/missing/file")},
             )
@@ -181,15 +181,15 @@
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import LocalPath
-            from onet.core import FileResult
+            from onet.file.file_result import FileResult
 
             file_result = FileResult(
                 successful={LocalPath("/some/file"), LocalPath("/some/another.file")},
             )
 
             assert file_result.successful_size == 1_000_000  # in bytes
         """
@@ -203,15 +203,15 @@
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import RemoteFile
-            from onet.core import FileResult
+            from onet.file.file_result import FileResult
 
             file_result = FileResult(
                 failed={RemoteFile("/some/file"), RemoteFile("/some/another.file")},
             )
 
             assert file_result.failed_size == 1_000_000  # in bytes
         """
@@ -225,15 +225,15 @@
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import LocalPath
-            from onet.core import FileResult
+            from onet.file.file_result import FileResult
 
             file_result = FileResult(
                 skipped={LocalPath("/some/file"), LocalPath("/some/another.file")},
             )
 
             assert file_result.skipped_size == 1_000_000  # in bytes
         """
@@ -247,15 +247,15 @@
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import RemoteFile, LocalPath
-            from onet.core import FileResult
+            from onet.file.file_result import FileResult
 
             file_result = FileResult(
                 successful={LocalPath("/local/file"), LocalPath("/local/another.file")},
                 failed={RemoteFile("/remote/file"), RemoteFile("/remote/another.file")},
                 skipped={LocalPath("/skipped/file")},
                 missing={LocalPath("/missing/file")},
             )
@@ -277,15 +277,15 @@
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import RemoteFile, LocalPath
-            from onet.core import FileResult
+            from onet.file.file_result import FileResult
 
             files_with_exception = [
                 FailedRemoteFile(
                     path="/remote/file1",
                     exception=NotAFileError("'/remote/file1' is not a file"),
                 ),
                 FailedRemoteFile(
@@ -322,15 +322,15 @@
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import RemoteFile, LocalPath
-            from onet.core import FileResult
+            from onet.file.file_result import FileResult
 
             file_result = FileResult(
                 missing={
                     LocalPath("/missing/file1"),
                     LocalPath("/missing/file2"),
                 },
             )
@@ -358,15 +358,15 @@
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import RemoteFile, LocalPath
-            from onet.core import FileResult
+            from onet.file.file_result import FileResult
 
             file_result = FileResult(
                 skipped={LocalPath("/skipped/file1"), LocalPath("/skipped/file2")},
             )
 
             file_result.raise_if_skipped()
             # will raise SkippedFilesError('''
@@ -391,15 +391,15 @@
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import RemoteFile, LocalPath
-            from onet.core import FileResult
+            from onet.file.file_result import FileResult
 
             file_result = FileResult(
                 successful={
                     LocalPath("/local/empty1.file"),
                     LocalPath("/local/empty2.file"),
                     LocalPath("/local/normal.file"),
                 },
@@ -422,15 +422,15 @@
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import LocalPath
-            from onet.core import FileResult
+            from onet.file.file_result import FileResult
 
             file_result1 = FileResult()
             assert file_result1.is_empty
 
             file_result2 = FileResult(
                 successful={LocalPath("/local/file"), LocalPath("/local/another.file")},
             )
@@ -451,15 +451,15 @@
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import RemoteFile, LocalPath
-            from onet.core import FileResult
+            from onet.file.file_result import FileResult
 
             file_result = FileResult()
 
             file_result.raise_if_empty()
             # will raise EmptyFilesError("There are no files in the result")
         """
 
@@ -473,15 +473,15 @@
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import RemoteFile, LocalPath
-            from onet.core import FileResult
+            from onet.file.file_result import FileResult
 
             file_result1 = FileResult(
                 successful={LocalPath("/local/file"), LocalPath("/local/another.file")},
                 failed={
                     FailedRemoteFile(
                         path="/remote/file1",
                         exception=NotAFileError("'/remote/file1' is not a file"),
@@ -553,15 +553,15 @@
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import RemoteFile, LocalPath
-            from onet.core import FileResult
+            from onet.file.file_result import FileResult
 
             file_result1 = FileResult(
                 successful={LocalPath("/local/file"), LocalPath("/local/another.file")},
                 failed={RemoteFile("/remote/file"), RemoteFile("/remote/another.file")},
                 skipped={LocalPath("/skipped/file")},
                 missing={LocalPath("/missing/file")},
             )
@@ -583,15 +583,15 @@
             file_result2 = FileResult()
             assert file_result1.summary == "No files"
         '''
 
         return self._total_message
 
     def __str__(self):
-        """Same as :obj:`onetl.core.file_result.FileResult.details`"""
+        """Same as :obj:`onetl.file.file_result.FileResult.details`"""
         return self.details
 
     @property
     def _total_summary(self) -> str:
         if self.successful or self.failed or self.missing or self.skipped:
             file_number_str = f"{self.total_count} files" if self.total_count > 1 else "1 file"
             return f"Total: {file_number_str} (size='{naturalsize(self.total_size)}')"
```

### Comparing `onetl-0.7.2/onetl/core/file_result/file_set.py` & `onetl-0.8.0/onetl/file/file_set.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 import os
 import textwrap
 from typing import Generic, TypeVar
 
 from humanize import naturalsize
 from ordered_set import OrderedSet
 
-from onetl.base import PathProtocol, PathWithStatsProtocol
+from onetl.base import PathProtocol, PathWithStatsProtocol, PurePathProtocol
 from onetl.exception import EmptyFilesError, ZeroFileSizeError
 from onetl.impl import path_repr
 
-T = TypeVar("T", bound=PathProtocol)
+T = TypeVar("T", bound=PurePathProtocol)
 INDENT = " " * 4
 
 
 class FileSet(OrderedSet[T], Generic[T]):
     """
     Ordered set of pathlib-like objects.
 
@@ -44,15 +44,15 @@
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import LocalPath
-            from onet.core import FileSet
+            from onet.file.file_set import FileSet
 
             file_set = FileSet({LocalPath("/some/file"), LocalPath("/some/another.file")})
 
             assert path_set.total_size == 1_000_000  # in bytes
         """
 
         return sum(
@@ -70,15 +70,15 @@
             File set is empty
 
         Examples
         --------
 
         .. code:: python
 
-            from onet.core import FileSet
+            from onet.file.file_set import FileSet
 
             file_set = FileSet()
 
             file_set.raise_if_empty()
             # will raise EmptyFilesError("There are no files in the set")
         """
 
@@ -97,15 +97,15 @@
 
         Examples
         --------
 
         .. code:: python
 
             from onetl.impl import RemoteFile, LocalPath
-            from onet.core import FileSet
+            from onet.file.file_set import FileSet
 
             file_set = FileSet(
                 LocalPath("/local/empty1.file"),
                 LocalPath("/local/empty2.file"),
                 LocalPath("/local/normal.file"),
             )
 
@@ -115,15 +115,18 @@
             #        '/local/empty1.file'
             #        '/local/empty2.file'
             # ''')
         """
 
         lines = []
         for file in self:
-            if not file.exists() or file.stat().st_size > 0:
+            if isinstance(file, PathProtocol) and not file.exists():
+                continue
+
+            if isinstance(file, PathWithStatsProtocol) and file.stat().st_size > 0:
                 continue
 
             lines.append(repr(os.fspath(file)))
 
         if not lines:
             return
 
@@ -139,21 +142,21 @@
         Return summary about files in the set
 
         Examples
         --------
 
         .. code:: python
 
-            from onetl.impl import LocalFile
-            from onet.core import FileSet
+            from onetl.impl import LocalPath
+            from onet.file.file_set import FileSet
 
             path_set1 = FileSet(
                 [
-                    LocalFile("/local/file"),
-                    LocalFile("/local/another.file"),
+                    LocalPath("/local/file"),
+                    LocalPath("/local/another.file"),
                 ]
             )
 
             assert path_set1.summary == "2 files (30.7 kB)"
 
             assert FileSet().summary == "No files"
         """
@@ -171,21 +174,21 @@
         Return detailed information about files in the set
 
         Examples
         --------
 
         .. code:: python
 
-            from onetl.impl import LocalFile
-            from onet.core import FileSet
+            from onetl.impl import LocalPath
+            from onet.file.file_set import FileSet
 
             path_set1 = FileSet(
                 [
-                    LocalFile("/local/file"),
-                    LocalFile("/local/another.file"),
+                    LocalPath("/local/file"),
+                    LocalPath("/local/another.file"),
                 ]
             )
 
             details1 = """
                 2 files (30.7 kB):
                     '/local/file' (10.2 kB)
                     '/local/another.file' (20.5 kB)
@@ -203,9 +206,9 @@
 
         summary = f"{self.summary}:{os.linesep}{INDENT}"
 
         lines_str = textwrap.indent(os.linesep.join(lines), INDENT).strip()
         return summary + lines_str
 
     def __str__(self) -> str:
-        """Same as :obj:`onetl.core.file_set.file_set.FileSet.details`"""
+        """Same as :obj:`onetl.file.file_set.file_set.FileSet.details`"""
         return self.details
```

### Comparing `onetl-0.7.2/onetl/core/file_uploader/__init__.py` & `onetl-0.8.0/onetl/impl/file_write_mode.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,9 +8,18 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from onetl.core.file_uploader.file_uploader import FileUploader
-from onetl.core.file_uploader.upload_result import UploadResult
+from enum import Enum
+
+
+class FileWriteMode(str, Enum):
+    ERROR = "error"
+    IGNORE = "ignore"
+    OVERWRITE = "overwrite"
+    DELETE_ALL = "delete_all"
+
+    def __str__(self):
+        return str(self.value)
```

### Comparing `onetl-0.7.2/onetl/core/file_uploader/file_uploader.py` & `onetl-0.8.0/onetl/file/file_uploader/file_uploader.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,38 +10,38 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from __future__ import annotations
 
+import logging
 import os
-from logging import getLogger
 from typing import Iterable, Optional, Tuple
 
 from ordered_set import OrderedSet
 from pydantic import validator
 
 from onetl._internal import generate_temp_path  # noqa: WPS436
 from onetl.base import BaseFileConnection
-from onetl.core.file_result import FileSet
-from onetl.core.file_uploader.upload_result import UploadResult
 from onetl.exception import DirectoryNotFoundError, NotAFileError
+from onetl.file.file_set import FileSet
+from onetl.file.file_uploader.upload_result import UploadResult
 from onetl.impl import (
     FailedLocalFile,
     FileWriteMode,
     FrozenModel,
     GenericOptions,
     LocalPath,
     RemotePath,
     path_repr,
 )
 from onetl.log import entity_boundary_log, log_lines, log_options, log_with_indent
 
-log = getLogger(__name__)
+log = logging.getLogger(__name__)
 
 # source, target, temp
 UPLOAD_ITEMS_TYPE = OrderedSet[Tuple[LocalPath, RemotePath, Optional[RemotePath]]]
 
 
 class FileUploader(FrozenModel):
     """Allows you to upload files to a remote source with specified file connection
@@ -50,18 +50,22 @@
     .. note::
 
         This class is used to upload files **only** from local directory to the remote one.
 
         It does NOT support direct file transfer between filesystems, like ``FTP -> SFTP``.
         You should use :ref:`file-downloader` + FileUploader to implement ``FTP -> local dir -> SFTP``.
 
+    .. warning::
+
+        This class does **not** support read strategies.
+
     Parameters
     ----------
     connection : :obj:`onetl.connection.FileConnection`
-        Class which contains File system connection properties. See in FileConnection section.
+        Class which contains File system connection properties. See :ref:`file-connections` section.
 
     target_path : os.PathLike or str
         Remote path where want you upload files to
 
     local_path : os.PathLike or str, optional, default: ``None``
         The local directory from which the data is loaded.
 
@@ -92,44 +96,44 @@
     Examples
     --------
     Simple Uploader creation
 
     .. code:: python
 
         from onetl.connection import HDFS
-        from onetl.core import FileUploader
+        from onetl.file import FileUploader
 
         hdfs = HDFS(...)
 
         uploader = FileUploader(
             connection=hdfs,
             target_path="/path/to/remote/source",
         )
 
     Uploader with all parameters
 
     .. code:: python
 
         from onetl.connection import HDFS
-        from onetl.core import FileUploader
+        from onetl.file import FileUploader
 
         hdfs = HDFS(...)
 
         uploader = FileUploader(
             connection=hdfs,
             target_path="/path/to/remote/source",
             temp_path="/user/onetl",
             local_path="/some/local/directory",
             options=FileUploader.Options(delete_local=True, mode="overwrite"),
         )
 
     """
 
     class Options(GenericOptions):
-        """File uploader options"""
+        """File uploading options"""
 
         mode: FileWriteMode = FileWriteMode.ERROR
         """
         How to handle existing files in the target directory.
 
         Possible values:
             * ``error`` (default) - do nothing, mark file as failed
@@ -150,109 +154,143 @@
     target_path: RemotePath
 
     local_path: Optional[LocalPath] = None
     temp_path: Optional[RemotePath] = None
 
     options: Options = Options()
 
-    @validator("local_path", pre=True, always=True)
-    def resolve_local_path(cls, local_path):
-        return LocalPath(local_path).resolve() if local_path else None
-
-    @validator("target_path", pre=True, always=True)
-    def check_target_path(cls, target_path):
-        return RemotePath(target_path)
-
-    @validator("temp_path", pre=True, always=True)
-    def check_temp_path(cls, temp_path):
-        return RemotePath(temp_path) if temp_path else None
-
     def run(self, files: Iterable[str | os.PathLike] | None = None) -> UploadResult:
         """
         Method for uploading files to remote host.
 
         Parameters
         ----------
 
         files : Iterator[str | os.PathLike] | None, default ``None``
             File list to upload.
 
             If empty, upload files from ``local_path``.
 
         Returns
         -------
-        uploaded_files : :obj:`onetl.core.file_uploader.upload_result.UploadResult`
+        uploaded_files : :obj:`UploadResult <onetl.file.file_uploader.upload_result.UploadResult>`
 
             Upload result object
 
         Raises
         -------
-        DirectoryNotFoundError
+        :obj:`onetl.exception.DirectoryNotFoundError`
 
             ``local_path`` does not found
 
         NotADirectoryError
 
             ``local_path`` is not a directory
 
         ValueError
 
             File in ``files`` argument does not match ``local_path``
 
         Examples
         --------
 
-        Upload files and get result
+        Upload files from ``local_path`` to ``target_path``
+
+        .. code:: python
+
+            from onetl.impl import (
+                RemoteFile,
+                LocalPath,
+            )
+            from onetl.file import FileUploader
+
+            uploader = FileUploader(local_path="/local", target_path="/remote", ...)
+            uploaded_files = uploader.run()
+
+            assert uploaded_files.successful == {
+                RemoteFile("/remote/file1"),
+                RemoteFile("/remote/file2"),
+                RemoteFile("/remote/nested/path/file3"),  # directory structure is preserved
+            }
+            assert uploaded_files.failed == {FailedLocalFile("/local/failed.file")}
+            assert uploaded_files.skipped == {LocalPath("/local/already.exists")}
+            assert uploaded_files.missing == {LocalPath("/local/missing.file")}
+
+        Upload only certain files from ``local_path``
 
         .. code:: python
 
             from onetl.impl import (
                 RemoteFile,
                 LocalPath,
             )
-            from onetl.core import FileUploader
+            from onetl.file import FileUploader
 
             uploader = FileUploader(local_path="/local", target_path="/remote", ...)
 
+            # paths could be relative or absolute, but all should be in "/local"
             uploaded_files = uploader.run(
                 [
                     "/local/file1",
-                    "/local/file2",
-                    "/failed/file",
-                    "/existing/file",
-                    "/missing/file",
+                    "/local/nested/path/file3",
+                    # excluding "/local/file2",
                 ]
             )
 
-            # or without the list of files
+            assert uploaded_files.successful == {
+                RemoteFile("/remote/file1"),
+                RemoteFile("/remote/nested/path/file3"),  # directory structure is preserved
+            }
+            assert not uploaded_files.failed
+            assert not uploaded_files.skipped
+            assert not uploaded_files.missing
+
+        Upload only certain files from any folder
+
+        .. code:: python
+
+            from onetl.impl import (
+                RemoteFile,
+                LocalPath,
+            )
+            from onetl.file import FileUploader
+
+            uploader = FileUploader(target_path="/remote", ...)  # no local_path set
 
-            uploaded_files = uploader.run()
+            # only absolute paths
+            uploaded_files = uploader.run(
+                [
+                    "/local/file1.txt",
+                    "/any/nested/path/file3.txt",
+                ]
+            )
 
             assert uploaded_files.successful == {
                 RemoteFile("/remote/file1"),
-                RemoteFile("/remote/file2"),
+                RemoteFile("/remote/file3"),
+                # directory structure is NOT preserved without local_path
             }
-            assert uploaded_files.failed == {FailedLocalFile("/failed/file")}
-            assert uploaded_files.skipped == {LocalPath("/existing/file")}
-            assert uploaded_files.missing == {LocalPath("/missing/file")}
+            assert not uploaded_files.failed
+            assert not uploaded_files.skipped
+            assert not uploaded_files.missing
         """
 
         if files is None and not self.local_path:
-            raise ValueError("Neither file list nor ``local_path`` are passed")
+            raise ValueError("Neither file list nor `local_path` are passed")
 
         self._log_options(files)
 
         # Check everything
         if self.local_path:
             self._check_local_path()
 
         self.connection.check()
         log_with_indent("")
 
-        self.connection.mkdir(self.target_path)
+        self.connection.create_dir(self.target_path)
 
         if files is None:
             log.info("|%s| File list is not passed to `run` method", self.__class__.__name__)
             files = self.view_files()
 
         if not files:
             log.info("|%s| No files to upload!", self.__class__.__name__)
@@ -262,35 +300,35 @@
         if self.temp_path:
             current_temp_dir = generate_temp_path(self.temp_path)
 
         to_upload = self._validate_files(files, current_temp_dir=current_temp_dir)
 
         # remove folder only after everything is checked
         if self.options.mode == FileWriteMode.DELETE_ALL:
-            self.connection.rmdir(self.target_path, recursive=True)
-            self.connection.mkdir(self.target_path)
+            self.connection.remove_dir(self.target_path, recursive=True)
+            self.connection.create_dir(self.target_path)
 
         if current_temp_dir:
-            current_temp_dir = self.connection.mkdir(current_temp_dir)
+            current_temp_dir = self.connection.create_dir(current_temp_dir)
 
         result = self._upload_files(to_upload)
 
         if current_temp_dir:
             self._remove_temp_dir(current_temp_dir)
 
         self._log_result(result)
         return result
 
     def view_files(self) -> FileSet[LocalPath]:
         """
-        Get file list in the ``local_path``
+        Get file list in the ``local_path``.
 
         Raises
         -------
-        DirectoryNotFoundError
+        :obj:`onetl.exception.DirectoryNotFoundError`
 
             ``local_path`` does not found
 
         NotADirectoryError
 
             ``local_path`` is not a directory
 
@@ -303,24 +341,24 @@
         --------
 
         View files
 
         .. code:: python
 
             from onetl.impl import LocalPath
-            from onetl.core import FileUploader
+            from onetl.file import FileUploader
 
-            uploader = FileUploader(local_path="/local/path", ...)
+            uploader = FileUploader(local_path="/local", ...)
 
             view_files = uploader.view_files()
 
             assert view_files == {
-                LocalPath("/local/path/file1.txt"),
-                LocalPath("/local/path/file3.txt"),
-                LocalPath("/local/path/nested/file3.txt"),
+                LocalPath("/local/file1.txt"),
+                LocalPath("/local/file3.txt"),
+                LocalPath("/local/nested/path/file3.txt"),
             }
         """
 
         log.info("|Local FS| Getting files list from path '%s'", self.local_path)
 
         self._check_local_path()
         result = FileSet()
@@ -332,14 +370,26 @@
         except Exception as e:
             raise RuntimeError(
                 f"Couldn't read directory tree from local dir '{self.local_path}'",
             ) from e
 
         return result
 
+    @validator("local_path", pre=True, always=True)
+    def _resolve_local_path(cls, local_path):
+        return LocalPath(local_path).resolve() if local_path else None
+
+    @validator("target_path", pre=True, always=True)
+    def _validate_target_path(cls, target_path):
+        return RemotePath(target_path)
+
+    @validator("temp_path", pre=True, always=True)
+    def _validate_temp_path(cls, temp_path):
+        return RemotePath(temp_path) if temp_path else None
+
     def _log_options(self, files: Iterable[str | os.PathLike] | None = None) -> None:
         entity_boundary_log(msg="FileUploader starts")
 
         log.info("|Local FS| -> |%s| Uploading files using parameters:'", self.connection.__class__.__name__)
         log_with_indent("local_path = %s", f"'{self.local_path}'" if self.local_path else "None")
         log_with_indent("target_path = '%s'", self.target_path)
         log_with_indent("temp_path = '%s'", f"'{self.temp_path}'" if self.temp_path else "None")
@@ -350,15 +400,15 @@
             log.warning("|%s| LOCAL FILES WILL BE PERMANENTLY DELETED AFTER UPLOADING !!!", self.__class__.__name__)
 
         if self.options.mode == FileWriteMode.DELETE_ALL:
             log.warning("|%s| TARGET DIRECTORY WILL BE CLEANED UP BEFORE UPLOADING FILES !!!", self.__class__.__name__)
 
         if files and self.local_path:
             log.warning(
-                "|%s| Passed both ``local_path`` and files list at the same time. Using explicit files list",
+                "|%s| Passed both `local_path` and files list at the same time. Using explicit files list",
                 self.__class__.__name__,
             )
 
     def _validate_files(  # noqa: WPS231
         self,
         local_files: Iterable[os.PathLike | str],
         current_temp_dir: RemotePath | None,
@@ -369,15 +419,15 @@
             local_file_path = LocalPath(file)
             local_file = local_file_path
             tmp_file: RemotePath | None = None
 
             if not self.local_path:
                 # Upload into a flat structure
                 if not local_file_path.is_absolute():
-                    raise ValueError("Cannot pass relative file path with empty ``local_path``")
+                    raise ValueError("Cannot pass relative file path with empty `local_path`")
 
                 filename = local_file_path.name
                 target_file = self.target_path / filename
                 if current_temp_dir:
                     tmp_file = current_temp_dir / filename  # noqa: WPS220
             else:
                 # Upload according to source folder structure
@@ -442,15 +492,15 @@
             log.warning("|%s| Missing file '%s', skipping", self.__class__.__name__, local_file)
             result.missing.add(local_file)
             return
 
         try:
             replace = False
             if self.connection.path_exists(target_file):
-                file = self.connection.get_file(target_file)
+                file = self.connection.resolve_file(target_file)
                 if self.options.mode == FileWriteMode.ERROR:
                     raise FileExistsError(f"File {path_repr(file)} already exists")
 
                 if self.options.mode == FileWriteMode.IGNORE:
                     log.warning("|%s| File %s already exists, skipping", self.__class__.__name__, path_repr(file))
                     result.skipped.add(local_file)
                     return
@@ -465,25 +515,29 @@
                 uploaded_file = self.connection.rename_file(tmp_file, target_file, replace=replace)
             else:
                 # Direct upload
                 uploaded_file = self.connection.upload_file(local_file, target_file, replace=replace)
 
             if self.options.delete_local:
                 local_file.unlink()
-                log.warning("|LocalFS| Successfully removed file %s", local_file)
+                log.warning("|Local FS| Successfully removed file %s", local_file)
 
             result.successful.add(uploaded_file)
 
         except Exception as e:
-            log.exception("|%s| Couldn't upload file to target dir: %s", self.__class__.__name__, e, exc_info=False)
+            if log.isEnabledFor(logging.DEBUG):
+                log.exception("|%s| Couldn't upload file to target dir", self.__class__.__name__, exc_info=e)
+            else:
+                log.exception("|%s| Couldn't upload file to target dir: %s", self.__class__.__name__, e, exc_info=False)
+
             result.failed.add(FailedLocalFile(path=local_file, exception=e))
 
     def _remove_temp_dir(self, temp_dir: RemotePath) -> None:
         try:
-            self.connection.rmdir(temp_dir, recursive=True)
+            self.connection.remove_dir(temp_dir, recursive=True)
         except Exception:
             log.exception("|%s| Error while removing temp directory", self.__class__.__name__)
 
     def _log_result(self, result: UploadResult) -> None:
         log.info("")
         log.info("|%s| Upload result:", self.__class__.__name__)
         log_lines(str(result))
```

### Comparing `onetl-0.7.2/onetl/core/file_uploader/upload_result.py` & `onetl-0.8.0/onetl/file/file_uploader/upload_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from __future__ import annotations
 
 from pydantic import Field
 
-from onetl.core import FileResult, FileSet
+from onetl.file.file_result import FileResult, FileSet
 from onetl.impl import FailedLocalFile, LocalPath, RemoteFile
 
 
 class UploadResult(FileResult):
     """
     Representation of file upload result.
 
@@ -35,15 +35,15 @@
     --------
 
     Upload files
 
     .. code:: python
 
         from onetl.impl import LocalPath, RemoteFile, FailedLocalFile
-        from onetl.core import FileUploader, UploadResult
+        from onetl.file import FileUploader, UploadResult
 
         uploader = FileUploader(target_path="/remote", ...)
 
         uploaded_files = uploader.run(
             [
                 "/local/file1",
                 "/local/file2",
```

### Comparing `onetl-0.7.2/onetl/exception.py` & `onetl-0.8.0/onetl/exception.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,26 @@
     """
     Like ``NotADirectoryError``, but for files.
 
     Cannot be replaced with ``FileNotFoundError``, it has different meaning
     """
 
 
+class FileSizeMismatchError(OSError):
+    """
+    File size mismatch
+    """
+
+
+class DirectoryExistsError(OSError):
+    """
+    Like ``FileExistsError``, but for directories.
+    """
+
+
 class DirectoryNotEmptyError(OSError):
     """
     Raised when trying to remove directory contains some files or other directories
     """
 
 
 class NoDataError(NeedEvacuation):
```

### Comparing `onetl-0.7.2/onetl/hooks/hook.py` & `onetl-0.8.0/onetl/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/hooks/hook_collection.py` & `onetl-0.8.0/onetl/hooks/hook_collection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/hooks/hooks_state.py` & `onetl-0.8.0/onetl/hooks/hooks_state.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/hooks/method_inheritance_stack.py` & `onetl-0.8.0/onetl/hooks/method_inheritance_stack.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/hooks/slot.py` & `onetl-0.8.0/onetl/hooks/slot.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/hooks/support_hooks.py` & `onetl-0.8.0/onetl/hooks/support_hooks.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/hwm/store/__init__.py` & `onetl-0.8.0/onetl/hwm/store/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/hwm/store/base_hwm_store.py` & `onetl-0.8.0/onetl/hwm/store/base_hwm_store.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/hwm/store/hwm_class_registry.py` & `onetl-0.8.0/onetl/hwm/store/hwm_class_registry.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/hwm/store/hwm_store_class_registry.py` & `onetl-0.8.0/onetl/hwm/store/hwm_store_class_registry.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/hwm/store/hwm_store_manager.py` & `onetl-0.8.0/onetl/hwm/store/hwm_store_manager.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/hwm/store/memory_hwm_store.py` & `onetl-0.8.0/onetl/hwm/store/memory_hwm_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     Examples
     --------
 
     .. code:: python
 
         from onetl.connection import Hive, Postgres
-        from onetl.core import DBReader
+        from onetl.db import DBReader
         from onetl.strategy import IncrementalStrategy
         from onetl.hwm.store import MemoryHWMStore
 
         from pyspark.sql import SparkSession
 
         spark = (
             SparkSession.builder.appName("spark-app-name")
```

### Comparing `onetl-0.7.2/onetl/hwm/store/yaml_hwm_store.py` & `onetl-0.8.0/onetl/hwm/store/yaml_hwm_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     --------
 
     Default parameters
 
     .. code:: python
 
         from onetl.connection import Hive, Postgres
-        from onetl.core import DBReader
+        from onetl.db import DBReader
         from onetl.strategy import IncrementalStrategy
         from onetl.hwm.store import YAMLHWMStore
 
         from pyspark.sql import SparkSession
 
         spark = (
             SparkSession.builder.appName("spark-app-name")
```

### Comparing `onetl-0.7.2/onetl/impl/__init__.py` & `onetl-0.8.0/onetl/impl/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/impl/base_model.py` & `onetl-0.8.0/onetl/impl/base_model.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/impl/failed_local_file.py` & `onetl-0.8.0/onetl/impl/failed_local_file.py`

 * *Files 21% similar despite different names*

```diff
@@ -32,10 +32,22 @@
     def __post_init__(self):
         # frozen=True does not allow to change any field in __post_init__, small hack here
         object.__setattr__(self, "path", LocalPath(self.path))  # noqa: WPS609
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({os.fspath(self.path)!r}, {self.exception!r})"
 
+    def exists(self) -> bool:
+        return self.path.exists()
+
+    def is_file(self) -> bool:
+        return self.path.is_file()
+
+    def is_dir(self) -> bool:
+        return self.path.is_dir()
+
+    def stat(self) -> os.stat_result:
+        return self.path.stat()
+
     # exceptions are not allowed to compare, another small hack
     def _compare_tuple(self, args) -> tuple:
         return tuple(str(arg) if isinstance(arg, Exception) else arg for arg in args)
```

### Comparing `onetl-0.7.2/onetl/impl/file_write_mode.py` & `onetl-0.8.0/onetl/impl/remote_path.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,18 +8,12 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from enum import Enum
+from pathlib import PurePosixPath
 
 
-class FileWriteMode(str, Enum):
-    ERROR = "error"
-    IGNORE = "ignore"
-    OVERWRITE = "overwrite"
-    DELETE_ALL = "delete_all"
-
-    def __str__(self):
-        return str(self.value)
+class RemotePath(PurePosixPath):
+    pass
```

### Comparing `onetl-0.7.2/onetl/impl/frozen_model.py` & `onetl-0.8.0/onetl/db/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,9 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from __future__ import annotations
-
-from onetl.impl.base_model import BaseModel
-
-
-class FrozenModel(BaseModel):
-    class Config:
-        frozen = True
+from onetl.db.db_reader import DBReader
+from onetl.db.db_writer import DBWriter
```

### Comparing `onetl-0.7.2/onetl/impl/generic_options.py` & `onetl-0.8.0/onetl/impl/generic_options.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/impl/local_path.py` & `onetl-0.8.0/onetl/impl/local_path.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/impl/path_container.py` & `onetl-0.8.0/onetl/impl/path_container.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,49 +12,48 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from __future__ import annotations
 
 import os
 from dataclasses import astuple, dataclass
-from typing import Generic, TypeVar
+from typing import Generic, Sequence, TypeVar
 
-GenericPath = TypeVar("GenericPath", bound=os.PathLike)
+from onetl.base import PurePathProtocol
+
+PurePath = TypeVar("PurePath", bound=PurePathProtocol)
 
 
 @dataclass(eq=False, frozen=True)
-class PathContainer(Generic[GenericPath]):
+class PathContainer(Generic[PurePath]):
     """
     Read-only container for ``pathlib.PurePath``-like classes with some custom logic.
 
     This is need to avoid creating objects of current class using ``PurePath``-like methods
     (e.g. ``path.with_name("new_name")``) or operators (e.g. ``path / "sub_path"``).
 
     It proxies all the method calls and operators to the underlying ``path`` field,
     so every method or operator returns new object of the same class as ``path`` field, without any magic.
     """
 
-    path: GenericPath
+    path: PurePath
 
     def __str__(self) -> str:
         return str(self.path)
 
     def __bytes__(self):
         return os.fsencode(self.path)
 
     def __fspath__(self) -> str:
         return os.fspath(self.path)
 
-    def __getattr__(self, attr: str):
-        return getattr(self.path, attr)
-
-    def __truediv__(self, other) -> GenericPath:
+    def __truediv__(self, other) -> PurePath:
         return self.path / other
 
-    def __rtruediv__(self, other) -> GenericPath:
+    def __rtruediv__(self, other) -> PurePath:
         return other / self.path
 
     def __hash__(self):
         return hash(self.path)
 
     def __eq__(self, other):
         if not isinstance(other, PathContainer):
@@ -82,9 +81,39 @@
 
     def __ge__(self, other):
         if not isinstance(other, PathContainer):
             return self.path >= other
 
         return self.path >= other.path
 
+    # typing_extensions 4.6+ implementation of `isinstance`` does not use __getattr__ anymore,
+    # so we need to create methods explicitly
+    @property
+    def name(self) -> str:
+        return self.path.name
+
+    @property
+    def parent(self) -> PurePathProtocol | PurePath:
+        return self.path.parent
+
+    @property
+    def parents(self) -> Sequence[PurePathProtocol | PurePath]:
+        return self.path.parents
+
+    @property
+    def parts(self) -> Sequence[str]:
+        return self.path.parts
+
+    def is_absolute(self) -> bool:
+        return self.path.is_absolute()
+
+    def match(self, path_pattern) -> bool:
+        return self.path.match(path_pattern)
+
+    def relative_to(self, *other) -> PurePathProtocol | PurePath:
+        return self.path.relative_to(*other)
+
+    def joinpath(self, *args) -> PurePathProtocol | PurePath:
+        return self.path.joinpath(*args)
+
     def _compare_tuple(self, args) -> tuple:
         return tuple(args)
```

### Comparing `onetl-0.7.2/onetl/impl/path_repr.py` & `onetl-0.8.0/onetl/impl/path_repr.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/impl/remote_directory.py` & `onetl-0.8.0/onetl/impl/remote_directory.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/impl/remote_file.py` & `onetl-0.8.0/onetl/impl/remote_file.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/impl/remote_path.py` & `onetl-0.8.0/onetl/file/file_mover/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,12 +8,9 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from pathlib import PurePosixPath
-
-
-class RemotePath(PurePosixPath):
-    pass
+from onetl.file.file_mover.file_mover import FileMover
+from onetl.file.file_mover.move_result import MoveResult
```

### Comparing `onetl-0.7.2/onetl/impl/remote_path_stat.py` & `onetl-0.8.0/onetl/impl/remote_path_stat.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/log.py` & `onetl-0.8.0/onetl/log.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/plugins/import_plugins.py` & `onetl-0.8.0/onetl/plugins/import_plugins.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/strategy/__init__.py` & `onetl-0.8.0/onetl/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/strategy/base_strategy.py` & `onetl-0.8.0/onetl/strategy/base_strategy.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/strategy/batch_hwm_strategy.py` & `onetl-0.8.0/onetl/strategy/batch_hwm_strategy.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/strategy/hwm_store/__init__.py` & `onetl-0.8.0/onetl/strategy/hwm_store/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,9 +55,8 @@
         Imports from module {__name__!r} are deprecated since v0.6.0 and will be removed in v1.0.0.
         Please use instead:
 
         from onetl.hwm.store import {name}
     """
 
     warnings.warn(textwrap.dedent(message).strip(), category=UserWarning, stacklevel=2)
-
     return getattr(import_module("onetl.hwm.store"), name)
```

### Comparing `onetl-0.7.2/onetl/strategy/hwm_strategy.py` & `onetl-0.8.0/onetl/strategy/hwm_strategy.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/strategy/incremental_strategy.py` & `onetl-0.8.0/onetl/strategy/incremental_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,16 +147,16 @@
                 with IncrementalStrategy():
                     download_result = downloader.run()  # something went wrong here
                     uploader.run(download_result.success)  # or here
                     # or here...
 
             When FileDownloader **will** update HWM in HWM Store, because:
 
-            * FileDownloader creates files on local filesystem, and file content may differ for different :obj:`modes <onetl.core.file_downloader.file_downloader.FileDownloader.Options.mode>`.
-            * It can remove files from the source if :obj:`delete_source <onetl.core.file_downloader.file_downloader.FileDownloader.Options.delete_source>` is set to ``True``.
+            * FileDownloader creates files on local filesystem, and file content may differ for different :obj:`modes <onetl.file.file_downloader.file_downloader.FileDownloader.Options.mode>`.
+            * It can remove files from the source if :obj:`delete_source <onetl.file.file_downloader.file_downloader.FileDownloader.Options.delete_source>` is set to ``True``.
 
     Parameters
     ----------
     offset : Any, default: ``None``
 
         If passed, the offset value will be used to read rows which appeared in the source after the previous read.
 
@@ -214,15 +214,15 @@
     --------
 
     Incremental run with :ref:`db-reader`:
 
     .. code:: python
 
         from onetl.connection import Postgres
-        from onetl.core import DBReader
+        from onetl.db import DBReader
         from onetl.strategy import IncrementalStrategy
 
         from pyspark.sql import SparkSession
 
         spark = (
             SparkSession.builder.appName("spark-app-name")
             .config("spark.jars.packages", Postgres.package)
@@ -305,15 +305,15 @@
         WHERE business_dt > CAST('2021-01-09' AS DATE);
 
     Incremental run with :ref:`file-downloader` and ``hwm_type="file_list"``:
 
     .. code:: python
 
         from onetl.connection import SFTP
-        from onetl.core import FileDownloader
+        from onetl.file import FileDownloader
         from onetl.strategy import SnapshotStrategy
 
         sftp = SFTP(
             host="sftp.domain.com",
             user="user",
             password="*****",
         )
@@ -470,15 +470,15 @@
     --------
 
     IncrementalBatch run:
 
     .. code:: python
 
         from onetl.connection import Postgres, Hive
-        from onetl.core import DBReader
+        from onetl.db import DBReader
         from onetl.strategy import IncrementalStrategy
 
         from pyspark.sql import SparkSession
 
         spark = (
             SparkSession.builder.appName("spark-app-name")
             .config("spark.jars.packages", Postgres.package)
```

### Comparing `onetl-0.7.2/onetl/strategy/snapshot_strategy.py` & `onetl-0.8.0/onetl/strategy/snapshot_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     --------
 
     Snapshot run with :ref:`db-reader`:
 
     .. code:: python
 
         from onetl.connection import Postgres
-        from onetl.core import DBReader
+        from onetl.db import DBReader
         from onetl.strategy import SnapshotStrategy
 
         from pyspark.sql import SparkSession
 
         spark = (
             SparkSession.builder.appName("spark-app-name")
             .config("spark.jars.packages", Postgres.package)
@@ -102,15 +102,15 @@
         # SELECT id, data FROM public.mydata;
 
     Snapshot run with :ref:`file-downloader`:
 
     .. code:: python
 
         from onetl.connection import SFTP
-        from onetl.core import FileDownloader
+        from onetl.file import FileDownloader
         from onetl.strategy import SnapshotStrategy
 
         sftp = SFTP(
             host="sftp.domain.com",
             user="user",
             password="*****",
         )
@@ -225,15 +225,15 @@
     --------
 
     SnapshotBatch run:
 
     .. code:: python
 
         from onetl.connection import Postgres, Hive
-        from onetl.core import DBReader
+        from onetl.db import DBReader
         from onetl.strategy import SnapshotBatchStrategy
 
         from pyspark.sql import SparkSession
 
         spark = (
             SparkSession.builder.appName("spark-app-name")
             .config("spark.jars.packages", Postgres.package)
```

### Comparing `onetl-0.7.2/onetl/strategy/strategy_manager.py` & `onetl-0.8.0/onetl/strategy/strategy_manager.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl/version.py` & `onetl-0.8.0/onetl/version.py`

 * *Files identical despite different names*

### Comparing `onetl-0.7.2/onetl.egg-info/PKG-INFO` & `onetl-0.8.0/onetl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetl
-Version: 0.7.2
+Version: 0.8.0
 Summary: One ETL tool to rule them all
 Home-page: https://github.com/MobileTeleSystems/onetl
 Author: DataOps.ETL
 Author-email: onetools@mts.ru
 License: Apache License 2.0
 Project-URL: Documentation, https://onetl.readthedocs.io/
 Project-URL: Source, https://github.com/MobileTeleSystems/onetl
@@ -159,15 +159,15 @@
 
 Minimal installation
 ~~~~~~~~~~~~~~~~~~~~
 
 Base ``onetl`` package contains:
 
 * ``DBReader``, ``DBWriter`` and related classes
-* ``FileDownloader``, ``FileUploader``, ``FileFilter``, ``FileLimit`` and related classes
+* ``FileDownloader``, ``FileUploader``, ``FileMover`` and related classes, like file filters & limits
 * Read Strategies & HWM classes
 * Plugins support
 
 It can be installed via:
 
 .. code:: bash
 
@@ -437,15 +437,16 @@
     .. code::
 
         127.0.0.1 hdfs
 
 .. note::
 
     To run Oracle tests you need to install `Oracle instantclient <https://www.oracle.com/database/technologies/instant-client.html>`__,
-    and pass its path to ``ONETL_ORA_CLIENT_PATH`` environment variable, e.g. ``ONETL_ORA_CLIENT_PATH=/path/to/client64/lib``.
+    and pass its path to ``ONETL_ORA_CLIENT_PATH`` and ``LD_LIBRARY_PATH`` environment variables,
+    e.g. ``ONETL_ORA_CLIENT_PATH=/path/to/client64/lib``.
 
     It may also require to add the same path into ``LD_LIBRARY_PATH`` environment variable
 
 .. note::
 
     To run Greenplum tests, you should:
```

### Comparing `onetl-0.7.2/onetl.egg-info/SOURCES.txt` & `onetl-0.8.0/onetl.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 onetl/base/base_file_connection.py
 onetl/base/base_file_filter.py
 onetl/base/base_file_limit.py
 onetl/base/contains_exception.py
 onetl/base/contains_get_df_schema.py
 onetl/base/path_protocol.py
 onetl/base/path_stat_protocol.py
+onetl/base/pure_path_protocol.py
+onetl/base/supports_rename_dir.py
 onetl/connection/__init__.py
 onetl/connection/kerberos_helpers.py
 onetl/connection/db_connection/__init__.py
 onetl/connection/db_connection/clickhouse.py
 onetl/connection/db_connection/db_connection.py
 onetl/connection/db_connection/greenplum.py
 onetl/connection/db_connection/hive.py
@@ -57,36 +59,50 @@
 onetl/connection/file_connection/file_connection.py
 onetl/connection/file_connection/ftp.py
 onetl/connection/file_connection/ftps.py
 onetl/connection/file_connection/hdfs.py
 onetl/connection/file_connection/s3.py
 onetl/connection/file_connection/sftp.py
 onetl/connection/file_connection/webdav.py
+onetl/connection/file_connection/mixins/__init__.py
+onetl/connection/file_connection/mixins/rename_dir_mixin.py
 onetl/core/__init__.py
-onetl/core/db_reader/__init__.py
-onetl/core/db_reader/db_reader.py
-onetl/core/db_reader/strategy_helper.py
-onetl/core/db_writer/__init__.py
-onetl/core/db_writer/db_writer.py
-onetl/core/file_downloader/__init__.py
-onetl/core/file_downloader/download_result.py
-onetl/core/file_downloader/file_downloader.py
 onetl/core/file_filter/__init__.py
 onetl/core/file_filter/file_filter.py
-onetl/core/file_filter/file_hwm_filter.py
-onetl/core/file_filter/match_all_filters.py
 onetl/core/file_limit/__init__.py
 onetl/core/file_limit/file_limit.py
-onetl/core/file_limit/limits_reached.py
-onetl/core/file_result/__init__.py
-onetl/core/file_result/file_result.py
-onetl/core/file_result/file_set.py
-onetl/core/file_uploader/__init__.py
-onetl/core/file_uploader/file_uploader.py
-onetl/core/file_uploader/upload_result.py
+onetl/db/__init__.py
+onetl/db/db_reader/__init__.py
+onetl/db/db_reader/db_reader.py
+onetl/db/db_reader/strategy_helper.py
+onetl/db/db_writer/__init__.py
+onetl/db/db_writer/db_writer.py
+onetl/file/__init__.py
+onetl/file/file_result.py
+onetl/file/file_set.py
+onetl/file/file_downloader/__init__.py
+onetl/file/file_downloader/download_result.py
+onetl/file/file_downloader/file_downloader.py
+onetl/file/file_mover/__init__.py
+onetl/file/file_mover/file_mover.py
+onetl/file/file_mover/move_result.py
+onetl/file/file_uploader/__init__.py
+onetl/file/file_uploader/file_uploader.py
+onetl/file/file_uploader/upload_result.py
+onetl/file/filter/__init__.py
+onetl/file/filter/exclude_dir.py
+onetl/file/filter/file_hwm.py
+onetl/file/filter/glob.py
+onetl/file/filter/match_all_filters.py
+onetl/file/filter/regexp.py
+onetl/file/limit/__init__.py
+onetl/file/limit/limits_reached.py
+onetl/file/limit/limits_stop_at.py
+onetl/file/limit/max_files_count.py
+onetl/file/limit/reset_limits.py
 onetl/hooks/__init__.py
 onetl/hooks/hook.py
 onetl/hooks/hook_collection.py
 onetl/hooks/hooks_state.py
 onetl/hooks/method_inheritance_stack.py
 onetl/hooks/slot.py
 onetl/hooks/support_hooks.py
@@ -135,11 +151,13 @@
 requirements/tests/base.txt
 requirements/tests/clickhouse.txt
 requirements/tests/mongodb.txt
 requirements/tests/mssql.txt
 requirements/tests/mysql.txt
 requirements/tests/oracle.txt
 requirements/tests/postgres.txt
+requirements/tests/spark-2.3.1.txt
 requirements/tests/spark-2.4.8.txt
 requirements/tests/spark-3.2.3.txt
 requirements/tests/spark-3.3.2.txt
-requirements/tests/spark-3.4.0.txt
+requirements/tests/spark-3.4.0.txt
+requirements/tests/spark-latest.txt
```

### Comparing `onetl-0.7.2/setup.cfg` & `onetl-0.8.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -205,15 +205,17 @@
 	WPS118,
 	WPS235,
 	WPS213,
 	WPS212,
 	F401,
 	F811,
 	F821,
-	WPS429
+	WPS429,
+	WPS342,
+	WPS520
 
 [darglint]
 docstring_style = sphinx
 
 [mypy]
 python_version = 3.7
 exclude = ^(?=.*file).*
```

### Comparing `onetl-0.7.2/setup.py` & `onetl-0.8.0/setup.py`

 * *Files identical despite different names*

