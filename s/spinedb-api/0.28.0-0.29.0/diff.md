# Comparing `tmp/spinedb_api-0.28.0.tar.gz` & `tmp/spinedb_api-0.29.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spinedb_api-0.28.0.tar", last modified: Fri Mar 24 10:28:06 2023, max compression
+gzip compressed data, was "spinedb_api-0.29.0.tar", last modified: Wed May 31 12:28:58 2023, max compression
```

## Comparing `spinedb_api-0.28.0.tar` & `spinedb_api-0.29.0.tar`

### file list

```diff
@@ -1,112 +1,113 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 10:28:06.273061 spinedb_api-0.28.0/
--rw-rw-rw-   0        0        0    33114 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/COPYING
--rw-rw-rw-   0        0        0     7816 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/COPYING.LESSER
--rw-rw-rw-   0        0        0       53 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3913 2023-03-24 10:28:06.274058 spinedb_api-0.28.0/PKG-INFO
--rw-rw-rw-   0        0        0     2786 2023-01-23 15:02:29.000000 spinedb_api-0.28.0/README.md
--rw-rw-rw-   0        0        0       86 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/pyproject.toml
--rw-rw-rw-   0        0        0     1140 2023-03-24 10:28:06.276051 spinedb_api-0.28.0/setup.cfg
--rw-rw-rw-   0        0        0       91 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:28:05.642148 spinedb_api-0.28.0/spinedb_api/
--rw-rw-rw-   0        0        0     4409 2023-03-24 10:26:48.000000 spinedb_api-0.28.0/spinedb_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:28:05.342269 spinedb_api-0.28.0/spinedb_api/alembic/
-drwxrwxrwx   0        0        0        0 2023-03-24 10:28:05.825303 spinedb_api-0.28.0/spinedb_api/alembic/versions/
--rw-rw-rw-   0        0        0     1862 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/spinedb_api/alembic/versions/070a0eb89e88_drop_category_tables.py
--rw-rw-rw-   0        0        0     4103 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/spinedb_api/alembic/versions/0c7d199ae915_add_list_value_table.py
--rw-rw-rw-   0        0        0     2442 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/spinedb_api/alembic/versions/1892adebc00f_create_metadata_tables.py
--rw-rw-rw-   0        0        0     3012 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/spinedb_api/alembic/versions/1e4997105288_separate_type_from_value.py
--rw-rw-rw-   0        0        0     6138 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/spinedb_api/alembic/versions/39e860a11b05_add_alternatives_and_scenarios.py
--rw-rw-rw-   0        0        0     2751 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/spinedb_api/alembic/versions/51fd7b69acf7_add_parameter_tag_and_parameter_value_list.py
--rw-rw-rw-   0        0        0     1323 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/spinedb_api/alembic/versions/738d494a08ac_fix_foreign_key_constraints_in_object_.py
--rw-rw-rw-   0        0        0     1349 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/spinedb_api/alembic/versions/7d0b467f2f4e_fix_foreign_key_constraints_in_entity_.py
--rw-rw-rw-   0        0        0     2517 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/spinedb_api/alembic/versions/8c19c53d5701_rename_parameter_to_parameter_definition.py
--rw-rw-rw-   0        0        0     2615 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/spinedb_api/alembic/versions/989fccf80441_replace_values_with_reference_to_list_.py
--rw-rw-rw-   0        0        0     1282 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/spinedb_api/alembic/versions/9da58d2def22_create_entity_group_table.py
--rw-rw-rw-   0        0        0    20419 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/spinedb_api/alembic/versions/bba1e2ef5153_move_to_entity_based_design.py
--rw-rw-rw-   0        0        0     4423 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/spinedb_api/alembic/versions/bf255c179bce_get_rid_of_unused_fields_in_parameter_.py
--rw-rw-rw-   0        0        0     3708 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/spinedb_api/alembic/versions/defbda3bf2b5_add_tool_feature_tables.py
--rw-rw-rw-   0        0        0     6146 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/spinedb_api/alembic/versions/fbb540efbf15_add_support_for_mysql.py
--rw-rw-rw-   0        0        0     1271 2022-10-07 09:12:02.000000 spinedb_api-0.28.0/spinedb_api/alembic/versions/fd542cebf699_drop_on_update_clauses_from_object_and_.py
--rw-rw-rw-   0        0        0    29964 2023-01-16 10:09:04.000000 spinedb_api-0.28.0/spinedb_api/check_functions.py
--rw-rw-rw-   0        0        0    23565 2023-03-20 08:15:28.000000 spinedb_api-0.28.0/spinedb_api/db_cache.py
--rw-rw-rw-   0        0        0     2465 2023-01-16 10:09:04.000000 spinedb_api-0.28.0/spinedb_api/db_mapping.py
--rw-rw-rw-   0        0        0    25613 2023-03-03 12:44:18.000000 spinedb_api-0.28.0/spinedb_api/db_mapping_add_mixin.py
--rw-rw-rw-   0        0        0    94013 2023-03-10 11:19:02.000000 spinedb_api-0.28.0/spinedb_api/db_mapping_base.py
--rw-rw-rw-   0        0        0    42757 2023-01-16 10:09:04.000000 spinedb_api-0.28.0/spinedb_api/db_mapping_check_mixin.py
--rw-rw-rw-   0        0        0     3696 2023-03-13 13:35:20.000000 spinedb_api-0.28.0/spinedb_api/db_mapping_commit_mixin.py
--rw-rw-rw-   0        0        0    15627 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/db_mapping_query_mixin.py
--rw-rw-rw-   0        0        0    15975 2023-03-15 13:29:55.000000 spinedb_api-0.28.0/spinedb_api/db_mapping_remove_mixin.py
--rw-rw-rw-   0        0        0    16621 2023-03-03 12:44:18.000000 spinedb_api-0.28.0/spinedb_api/db_mapping_update_mixin.py
--rw-rw-rw-   0        0        0     9067 2023-01-16 10:09:04.000000 spinedb_api-0.28.0/spinedb_api/diff_db_mapping.py
--rw-rw-rw-   0        0        0     6590 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/diff_db_mapping_base.py
--rw-rw-rw-   0        0        0     5189 2023-01-16 10:09:04.000000 spinedb_api-0.28.0/spinedb_api/diff_db_mapping_commit_mixin.py
--rw-rw-rw-   0        0        0     3646 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/exception.py
--rw-rw-rw-   0        0        0    13548 2023-01-16 10:09:04.000000 spinedb_api-0.28.0/spinedb_api/export_functions.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:28:05.892088 spinedb_api-0.28.0/spinedb_api/export_mapping/
--rw-rw-rw-   0        0        0     1733 2023-02-24 11:19:55.000000 spinedb_api-0.28.0/spinedb_api/export_mapping/__init__.py
--rw-rw-rw-   0        0        0    63784 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/export_mapping/export_mapping.py
--rw-rw-rw-   0        0        0     4406 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/export_mapping/generator.py
--rw-rw-rw-   0        0        0     4225 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/export_mapping/group_functions.py
--rw-rw-rw-   0        0        0    10606 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/export_mapping/pivot.py
--rw-rw-rw-   0        0        0    31018 2023-02-24 11:19:55.000000 spinedb_api-0.28.0/spinedb_api/export_mapping/settings.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:28:05.958995 spinedb_api-0.28.0/spinedb_api/filters/
--rw-rw-rw-   0        0        0      989 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/filters/__init__.py
--rw-rw-rw-   0        0        0     6875 2023-03-07 12:11:53.000000 spinedb_api-0.28.0/spinedb_api/filters/alternative_filter.py
--rw-rw-rw-   0        0        0     6440 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/filters/execution_filter.py
--rw-rw-rw-   0        0        0    10023 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/filters/renamer.py
--rw-rw-rw-   0        0        0    10392 2023-01-13 12:44:21.000000 spinedb_api-0.28.0/spinedb_api/filters/scenario_filter.py
--rw-rw-rw-   0        0        0    10246 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/filters/tool_filter.py
--rw-rw-rw-   0        0        0    11086 2023-01-16 10:09:04.000000 spinedb_api-0.28.0/spinedb_api/filters/tools.py
--rw-rw-rw-   0        0        0    12995 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/filters/value_transformer.py
--rw-rw-rw-   0        0        0     7282 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/graph_layout_generator.py
--rw-rw-rw-   0        0        0    38433 2023-01-23 15:02:29.000000 spinedb_api-0.28.0/spinedb_api/helpers.py
--rw-rw-rw-   0        0        0    85858 2023-01-16 10:09:04.000000 spinedb_api-0.28.0/spinedb_api/import_functions.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:28:06.008900 spinedb_api-0.28.0/spinedb_api/import_mapping/
--rw-rw-rw-   0        0        0      989 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/import_mapping/__init__.py
--rw-rw-rw-   0        0        0    15791 2023-03-13 13:35:20.000000 spinedb_api-0.28.0/spinedb_api/import_mapping/generator.py
--rw-rw-rw-   0        0        0    44579 2023-02-24 11:19:55.000000 spinedb_api-0.28.0/spinedb_api/import_mapping/import_mapping.py
--rw-rw-rw-   0        0        0    18125 2023-02-24 11:19:55.000000 spinedb_api-0.28.0/spinedb_api/import_mapping/import_mapping_compat.py
--rw-rw-rw-   0        0        0     4136 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/import_mapping/type_conversion.py
--rw-rw-rw-   0        0        0     9197 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/mapping.py
--rw-rw-rw-   0        0        0    56635 2023-03-16 06:54:07.000000 spinedb_api-0.28.0/spinedb_api/parameter_value.py
--rw-rw-rw-   0        0        0     8596 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/perfect_split.py
--rw-rw-rw-   0        0        0     3421 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/purge.py
--rw-rw-rw-   0        0        0     4823 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/server_client_helpers.py
--rw-rw-rw-   0        0        0     4246 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/spine_db_client.py
--rw-rw-rw-   0        0        0    22585 2023-03-10 11:02:32.000000 spinedb_api-0.28.0/spinedb_api/spine_db_server.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:28:06.025429 spinedb_api-0.28.0/spinedb_api/spine_io/
--rw-rw-rw-   0        0        0     1106 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/spine_io/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:28:06.091885 spinedb_api-0.28.0/spinedb_api/spine_io/exporters/
--rw-rw-rw-   0        0        0     1115 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/spine_io/exporters/__init__.py
--rw-rw-rw-   0        0        0     2771 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/spine_io/exporters/csv_writer.py
--rw-rw-rw-   0        0        0    13214 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/spine_io/exporters/excel.py
--rw-rw-rw-   0        0        0     4616 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/spine_io/exporters/excel_writer.py
--rw-rw-rw-   0        0        0     5873 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/spine_io/exporters/gdx_writer.py
--rw-rw-rw-   0        0        0     6383 2023-03-13 07:33:38.000000 spinedb_api-0.28.0/spinedb_api/spine_io/exporters/sql_writer.py
--rw-rw-rw-   0        0        0     5395 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/spine_io/exporters/writer.py
--rw-rw-rw-   0        0        0     2734 2023-02-16 06:15:48.000000 spinedb_api-0.28.0/spinedb_api/spine_io/gdx_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:28:06.175352 spinedb_api-0.28.0/spinedb_api/spine_io/importers/
--rw-rw-rw-   0        0        0     1074 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/spinedb_api/spine_io/importers/__init__.py
--rw-rw-rw-   0        0        0     7604 2023-01-30 08:01:58.000000 spinedb_api-0.28.0/spinedb_api/spine_io/importers/csv_reader.py
--rw-rw-rw-   0        0        0     4204 2023-01-30 08:01:58.000000 spinedb_api-0.28.0/spinedb_api/spine_io/importers/datapackage_reader.py
--rw-rw-rw-   0        0        0    10869 2023-03-15 14:33:22.000000 spinedb_api-0.28.0/spinedb_api/spine_io/importers/excel_reader.py
--rw-rw-rw-   0        0        0     4937 2023-01-30 08:01:58.000000 spinedb_api-0.28.0/spinedb_api/spine_io/importers/gdx_connector.py
--rw-rw-rw-   0        0        0     3727 2023-01-30 08:01:58.000000 spinedb_api-0.28.0/spinedb_api/spine_io/importers/json_reader.py
--rw-rw-rw-   0        0        0     6736 2023-02-03 12:52:08.000000 spinedb_api-0.28.0/spinedb_api/spine_io/importers/reader.py
--rw-rw-rw-   0        0        0     3353 2023-02-03 13:25:24.000000 spinedb_api-0.28.0/spinedb_api/spine_io/importers/sqlalchemy_connector.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:28:05.675450 spinedb_api-0.28.0/spinedb_api.egg-info/
--rw-rw-rw-   0        0        0     3913 2023-03-24 10:28:05.000000 spinedb_api-0.28.0/spinedb_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4067 2023-03-24 10:28:05.000000 spinedb_api-0.28.0/spinedb_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 10:28:05.000000 spinedb_api-0.28.0/spinedb_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-10-07 10:27:53.000000 spinedb_api-0.28.0/spinedb_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      190 2023-03-24 10:28:05.000000 spinedb_api-0.28.0/spinedb_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-24 10:28:05.000000 spinedb_api-0.28.0/spinedb_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-24 10:28:06.272063 spinedb_api-0.28.0/tests/
--rw-rw-rw-   0        0        0    52595 2023-01-16 10:09:04.000000 spinedb_api-0.28.0/tests/test_DatabaseMapping.py
--rw-rw-rw-   0        0        0    74882 2023-01-16 10:09:04.000000 spinedb_api-0.28.0/tests/test_DiffDatabaseMapping.py
--rw-rw-rw-   0        0        0     9218 2023-01-16 10:09:04.000000 spinedb_api-0.28.0/tests/test_export_functions.py
--rw-rw-rw-   0        0        0     1939 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/tests/test_helpers.py
--rw-rw-rw-   0        0        0    74588 2022-11-10 07:42:15.000000 spinedb_api-0.28.0/tests/test_import_functions.py
--rw-rw-rw-   0        0        0     2257 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/tests/test_mapping.py
--rw-rw-rw-   0        0        0     8624 2022-11-03 13:53:25.000000 spinedb_api-0.28.0/tests/test_migration.py
--rw-rw-rw-   0        0        0    46929 2023-03-15 14:33:22.000000 spinedb_api-0.28.0/tests/test_parameter_value.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:28:58.179174 spinedb_api-0.29.0/
+-rw-rw-rw-   0        0        0    33114 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/COPYING
+-rw-rw-rw-   0        0        0     7816 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/COPYING.LESSER
+-rw-rw-rw-   0        0        0       53 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3358 2023-05-31 12:28:58.181160 spinedb_api-0.29.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2786 2023-01-23 15:02:29.000000 spinedb_api-0.29.0/README.md
+-rw-rw-rw-   0        0        0       86 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1140 2023-05-31 12:28:58.184150 spinedb_api-0.29.0/setup.cfg
+-rw-rw-rw-   0        0        0       91 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:28:57.441643 spinedb_api-0.29.0/spinedb_api/
+-rw-rw-rw-   0        0        0     4409 2023-05-31 12:27:55.000000 spinedb_api-0.29.0/spinedb_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:28:57.119232 spinedb_api-0.29.0/spinedb_api/alembic/
+drwxrwxrwx   0        0        0        0 2023-05-31 12:28:57.657486 spinedb_api-0.29.0/spinedb_api/alembic/versions/
+-rw-rw-rw-   0        0        0     1862 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/spinedb_api/alembic/versions/070a0eb89e88_drop_category_tables.py
+-rw-rw-rw-   0        0        0     4103 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/spinedb_api/alembic/versions/0c7d199ae915_add_list_value_table.py
+-rw-rw-rw-   0        0        0     2442 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/spinedb_api/alembic/versions/1892adebc00f_create_metadata_tables.py
+-rw-rw-rw-   0        0        0     3012 2023-05-19 09:15:42.000000 spinedb_api-0.29.0/spinedb_api/alembic/versions/1e4997105288_separate_type_from_value.py
+-rw-rw-rw-   0        0        0     6138 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/spinedb_api/alembic/versions/39e860a11b05_add_alternatives_and_scenarios.py
+-rw-rw-rw-   0        0        0     2751 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/spinedb_api/alembic/versions/51fd7b69acf7_add_parameter_tag_and_parameter_value_list.py
+-rw-rw-rw-   0        0        0     1323 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/spinedb_api/alembic/versions/738d494a08ac_fix_foreign_key_constraints_in_object_.py
+-rw-rw-rw-   0        0        0     1349 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/spinedb_api/alembic/versions/7d0b467f2f4e_fix_foreign_key_constraints_in_entity_.py
+-rw-rw-rw-   0        0        0     2517 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/spinedb_api/alembic/versions/8c19c53d5701_rename_parameter_to_parameter_definition.py
+-rw-rw-rw-   0        0        0     2615 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/alembic/versions/989fccf80441_replace_values_with_reference_to_list_.py
+-rw-rw-rw-   0        0        0     1282 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/spinedb_api/alembic/versions/9da58d2def22_create_entity_group_table.py
+-rw-rw-rw-   0        0        0    20419 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/spinedb_api/alembic/versions/bba1e2ef5153_move_to_entity_based_design.py
+-rw-rw-rw-   0        0        0     4423 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/spinedb_api/alembic/versions/bf255c179bce_get_rid_of_unused_fields_in_parameter_.py
+-rw-rw-rw-   0        0        0     3708 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/spinedb_api/alembic/versions/defbda3bf2b5_add_tool_feature_tables.py
+-rw-rw-rw-   0        0        0     6146 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/spinedb_api/alembic/versions/fbb540efbf15_add_support_for_mysql.py
+-rw-rw-rw-   0        0        0     1271 2022-10-07 09:12:02.000000 spinedb_api-0.29.0/spinedb_api/alembic/versions/fd542cebf699_drop_on_update_clauses_from_object_and_.py
+-rw-rw-rw-   0        0        0    29962 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/check_functions.py
+-rw-rw-rw-   0        0        0    23904 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/db_cache.py
+-rw-rw-rw-   0        0        0     2416 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/db_mapping.py
+-rw-rw-rw-   0        0        0    25564 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/db_mapping_add_mixin.py
+-rw-rw-rw-   0        0        0    93964 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/db_mapping_base.py
+-rw-rw-rw-   0        0        0    42708 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/db_mapping_check_mixin.py
+-rw-rw-rw-   0        0        0     3647 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/db_mapping_commit_mixin.py
+-rw-rw-rw-   0        0        0    15578 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/db_mapping_query_mixin.py
+-rw-rw-rw-   0        0        0    15926 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/db_mapping_remove_mixin.py
+-rw-rw-rw-   0        0        0    16572 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/db_mapping_update_mixin.py
+-rw-rw-rw-   0        0        0     9018 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/diff_db_mapping.py
+-rw-rw-rw-   0        0        0     6541 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/diff_db_mapping_base.py
+-rw-rw-rw-   0        0        0     5140 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/diff_db_mapping_commit_mixin.py
+-rw-rw-rw-   0        0        0     3597 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/exception.py
+-rw-rw-rw-   0        0        0    13504 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/export_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:28:57.726331 spinedb_api-0.29.0/spinedb_api/export_mapping/
+-rw-rw-rw-   0        0        0     1684 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/export_mapping/__init__.py
+-rw-rw-rw-   0        0        0    63974 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/export_mapping/export_mapping.py
+-rw-rw-rw-   0        0        0     4357 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/export_mapping/generator.py
+-rw-rw-rw-   0        0        0     4181 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/export_mapping/group_functions.py
+-rw-rw-rw-   0        0        0    10559 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/export_mapping/pivot.py
+-rw-rw-rw-   0        0        0    30774 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/export_mapping/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:28:57.830903 spinedb_api-0.29.0/spinedb_api/filters/
+-rw-rw-rw-   0        0        0      989 2022-11-03 13:53:25.000000 spinedb_api-0.29.0/spinedb_api/filters/__init__.py
+-rw-rw-rw-   0        0        0     6824 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/filters/alternative_filter.py
+-rw-rw-rw-   0        0        0     6389 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/filters/execution_filter.py
+-rw-rw-rw-   0        0        0     9981 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/filters/renamer.py
+-rw-rw-rw-   0        0        0    10341 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/filters/scenario_filter.py
+-rw-rw-rw-   0        0        0    10201 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/filters/tool_filter.py
+-rw-rw-rw-   0        0        0    11044 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/filters/tools.py
+-rw-rw-rw-   0        0        0    12953 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/filters/value_transformer.py
+-rw-rw-rw-   0        0        0     7399 2023-05-19 09:15:42.000000 spinedb_api-0.29.0/spinedb_api/graph_layout_generator.py
+-rw-rw-rw-   0        0        0    38388 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/helpers.py
+-rw-rw-rw-   0        0        0    85807 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/import_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:28:57.884742 spinedb_api-0.29.0/spinedb_api/import_mapping/
+-rw-rw-rw-   0        0        0      989 2022-11-03 13:53:25.000000 spinedb_api-0.29.0/spinedb_api/import_mapping/__init__.py
+-rw-rw-rw-   0        0        0    15740 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/import_mapping/generator.py
+-rw-rw-rw-   0        0        0    44530 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/import_mapping/import_mapping.py
+-rw-rw-rw-   0        0        0    18074 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/import_mapping/import_mapping_compat.py
+-rw-rw-rw-   0        0        0     4221 2023-05-19 09:47:07.000000 spinedb_api-0.29.0/spinedb_api/import_mapping/type_conversion.py
+-rw-rw-rw-   0        0        0     9148 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/mapping.py
+-rw-rw-rw-   0        0        0    56588 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/parameter_value.py
+-rw-rw-rw-   0        0        0     8552 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/perfect_split.py
+-rw-rw-rw-   0        0        0     3357 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/purge.py
+-rw-rw-rw-   0        0        0     4775 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/server_client_helpers.py
+-rw-rw-rw-   0        0        0     4200 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/spine_db_client.py
+-rw-rw-rw-   0        0        0    22540 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/spine_db_server.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:28:57.903659 spinedb_api-0.29.0/spinedb_api/spine_io/
+-rw-rw-rw-   0        0        0     1057 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/spine_io/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:28:57.984493 spinedb_api-0.29.0/spinedb_api/spine_io/exporters/
+-rw-rw-rw-   0        0        0     1067 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/spine_io/exporters/__init__.py
+-rw-rw-rw-   0        0        0     2723 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/spine_io/exporters/csv_writer.py
+-rw-rw-rw-   0        0        0    13129 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/spinedb_api/spine_io/exporters/excel.py
+-rw-rw-rw-   0        0        0     4568 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/spine_io/exporters/excel_writer.py
+-rw-rw-rw-   0        0        0     5825 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/spine_io/exporters/gdx_writer.py
+-rw-rw-rw-   0        0        0     6336 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/spine_io/exporters/sql_writer.py
+-rw-rw-rw-   0        0        0     5347 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/spine_io/exporters/writer.py
+-rw-rw-rw-   0        0        0     2687 2023-05-19 09:15:42.000000 spinedb_api-0.29.0/spinedb_api/spine_io/gdx_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:28:58.071174 spinedb_api-0.29.0/spinedb_api/spine_io/importers/
+-rw-rw-rw-   0        0        0     1025 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/spine_io/importers/__init__.py
+-rw-rw-rw-   0        0        0     7526 2023-05-19 09:47:07.000000 spinedb_api-0.29.0/spinedb_api/spine_io/importers/csv_reader.py
+-rw-rw-rw-   0        0        0     4148 2023-05-19 09:47:07.000000 spinedb_api-0.29.0/spinedb_api/spine_io/importers/datapackage_reader.py
+-rw-rw-rw-   0        0        0    10820 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/spine_io/importers/excel_reader.py
+-rw-rw-rw-   0        0        0     4888 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/spine_io/importers/gdx_connector.py
+-rw-rw-rw-   0        0        0     3714 2023-05-19 09:47:07.000000 spinedb_api-0.29.0/spinedb_api/spine_io/importers/json_reader.py
+-rw-rw-rw-   0        0        0     6687 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/spine_io/importers/reader.py
+-rw-rw-rw-   0        0        0     3304 2023-04-19 13:04:09.000000 spinedb_api-0.29.0/spinedb_api/spine_io/importers/sqlalchemy_connector.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:28:57.472537 spinedb_api-0.29.0/spinedb_api.egg-info/
+-rw-rw-rw-   0        0        0     3358 2023-05-31 12:28:56.000000 spinedb_api-0.29.0/spinedb_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4097 2023-05-31 12:28:56.000000 spinedb_api-0.29.0/spinedb_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 12:28:56.000000 spinedb_api-0.29.0/spinedb_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-10-07 10:27:53.000000 spinedb_api-0.29.0/spinedb_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      190 2023-05-31 12:28:56.000000 spinedb_api-0.29.0/spinedb_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-31 12:28:56.000000 spinedb_api-0.29.0/spinedb_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 12:28:58.177665 spinedb_api-0.29.0/tests/
+-rw-rw-rw-   0        0        0    52554 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/tests/test_DatabaseMapping.py
+-rw-rw-rw-   0        0        0    74831 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/tests/test_DiffDatabaseMapping.py
+-rw-rw-rw-   0        0        0     4278 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/tests/test_check_functions.py
+-rw-rw-rw-   0        0        0     9168 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/tests/test_export_functions.py
+-rw-rw-rw-   0        0        0     1888 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/tests/test_helpers.py
+-rw-rw-rw-   0        0        0    74537 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/tests/test_import_functions.py
+-rw-rw-rw-   0        0        0     2209 2023-04-19 13:04:10.000000 spinedb_api-0.29.0/tests/test_mapping.py
+-rw-rw-rw-   0        0        0     8579 2023-05-22 08:51:09.000000 spinedb_api-0.29.0/tests/test_migration.py
+-rw-rw-rw-   0        0        0    46881 2023-04-19 13:04:10.000000 spinedb_api-0.29.0/tests/test_parameter_value.py
```

### Comparing `spinedb_api-0.28.0/COPYING` & `spinedb_api-0.29.0/COPYING`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/COPYING.LESSER` & `spinedb_api-0.29.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/PKG-INFO` & `spinedb_api-0.29.0/spinedb_api.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,88 @@
 Metadata-Version: 2.1
-Name: spinedb_api
-Version: 0.28.0
+Name: spinedb-api
+Version: 0.29.0
 Summary: An API to talk to Spine databases.
 Home-page: https://github.com/spine-tools/Spine-Database-API
 Author: Spine Project consortium
 Author-email: spine_info@vtt.fi
 License: LGPL-3.0-or-later
-Description: # Spine Database API
-        
-        [![Documentation Status](https://readthedocs.org/projects/spine-database-api/badge/?version=latest)](https://spine-database-api.readthedocs.io/en/latest/?badge=latest)
-        [![Unit tests](https://github.com/spine-tools/Spine-Database-API/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/Spine-Database-API/actions?query=workflow%3A"Unit+tests")
-        [![codecov](https://codecov.io/gh/spine-tools/Spine-Database-API/branch/master/graph/badge.svg)](https://codecov.io/gh/spine-tools/Spine-Database-API)
-        [![PyPI version](https://badge.fury.io/py/spinedb-api.svg)](https://badge.fury.io/py/spinedb-api)
-        
-        A Python package to access and manipulate Spine databases in a customary, unified way.
-        
-        ## License
-        
-        Spine Database API is released under the GNU Lesser General Public License (LGPL) license. All accompanying
-        documentation and manual are released under the Creative Commons BY-SA 4.0 license.
-        
-        ## Getting started
-        
-        ### Installation
-        
-        To install the package run:
-        
-            $ pip install spinedb_api
-        
-        To upgrade to the most recent version, run:
-        
-            $ pip install --upgrade spinedb_api
-        
-        You can also specify a branch, or a tag, for instance:
-        
-            $ pip install spinedb_api==0.12.1
-        
-        To install the latest development version use the Git repository url:
-        
-            $ pip install --upgrade git+https://github.com/spine-tools/Spine-Database-API.git
-        
-        
-        ## Building the documentation
-        
-        Source files for the documentation can be found in `docs/source` directory. In order to 
-        build the HTML docs, you need to install the additional documentation building requirements
-        by running:
-        
-            $ pip install -r dev-requirements.txt 
-        
-        This installs Sphinx (among other things), which is required in building the documentation.
-        When Sphinx is installed, you can build the HTML pages from the source files by running:
-        
-            > docs\make.bat html
-            
-        or
-        
-            $ pushd docs
-            $ make html
-            $ popd
-            
-        depending on your operating system.        
-         
-        After running the build, the index page can be found in `docs/build/html/index.html`.
-        
-        &nbsp;
-        <hr>
-        <center>
-        <table width=500px frame="none">
-        <tr>
-        <td valign="middle" width=100px>
-        <img src=fig/eu-emblem-low-res.jpg alt="EU emblem" width=100%></td>
-        <td valign="middle">This project has received funding from European Climate, Infrastructure and Environment Executive Agency under the European Union’s HORIZON Research and Innovation Actions under grant agreement N°101095998.</td>
-        <tr>
-        <td valign="middle" width=100px>
-        <img src=fig/eu-emblem-low-res.jpg alt="EU emblem" width=100%></td>
-        <td valign="middle">This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 774629.</td>
-        </table>
-        </center>
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.12,>=3.8.1
 Description-Content-Type: text/markdown
+License-File: COPYING
+License-File: COPYING.LESSER
+
+# Spine Database API
+
+[![Documentation Status](https://readthedocs.org/projects/spine-database-api/badge/?version=latest)](https://spine-database-api.readthedocs.io/en/latest/?badge=latest)
+[![Unit tests](https://github.com/spine-tools/Spine-Database-API/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/Spine-Database-API/actions?query=workflow%3A"Unit+tests")
+[![codecov](https://codecov.io/gh/spine-tools/Spine-Database-API/branch/master/graph/badge.svg)](https://codecov.io/gh/spine-tools/Spine-Database-API)
+[![PyPI version](https://badge.fury.io/py/spinedb-api.svg)](https://badge.fury.io/py/spinedb-api)
+
+A Python package to access and manipulate Spine databases in a customary, unified way.
+
+## License
+
+Spine Database API is released under the GNU Lesser General Public License (LGPL) license. All accompanying
+documentation and manual are released under the Creative Commons BY-SA 4.0 license.
+
+## Getting started
+
+### Installation
+
+To install the package run:
+
+    $ pip install spinedb_api
+
+To upgrade to the most recent version, run:
+
+    $ pip install --upgrade spinedb_api
+
+You can also specify a branch, or a tag, for instance:
+
+    $ pip install spinedb_api==0.12.1
+
+To install the latest development version use the Git repository url:
+
+    $ pip install --upgrade git+https://github.com/spine-tools/Spine-Database-API.git
+
+
+## Building the documentation
+
+Source files for the documentation can be found in `docs/source` directory. In order to 
+build the HTML docs, you need to install the additional documentation building requirements
+by running:
+
+    $ pip install -r dev-requirements.txt 
+
+This installs Sphinx (among other things), which is required in building the documentation.
+When Sphinx is installed, you can build the HTML pages from the source files by running:
+
+    > docs\make.bat html
+    
+or
+
+    $ pushd docs
+    $ make html
+    $ popd
+    
+depending on your operating system.        
+ 
+After running the build, the index page can be found in `docs/build/html/index.html`.
+
+&nbsp;
+<hr>
+<center>
+<table width=500px frame="none">
+<tr>
+<td valign="middle" width=100px>
+<img src=fig/eu-emblem-low-res.jpg alt="EU emblem" width=100%></td>
+<td valign="middle">This project has received funding from European Climate, Infrastructure and Environment Executive Agency under the European Union’s HORIZON Research and Innovation Actions under grant agreement N°101095998.</td>
+<tr>
+<td valign="middle" width=100px>
+<img src=fig/eu-emblem-low-res.jpg alt="EU emblem" width=100%></td>
+<td valign="middle">This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 774629.</td>
+</table>
+</center>
```

#### html2text {}

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 2.1 Name: spinedb_api Version: 0.28.0 Summary: An API to talk
+Metadata-Version: 2.1 Name: spinedb-api Version: 0.29.0 Summary: An API to talk
 to Spine databases. Home-page: https://github.com/spine-tools/Spine-Database-
 API Author: Spine Project consortium Author-email: spine_info@vtt.fi License:
-LGPL-3.0-or-later Description: # Spine Database API [![Documentation Status]
-(https://readthedocs.org/projects/spine-database-api/badge/?version=latest)]
-(https://spine-database-api.readthedocs.io/en/latest/?badge=latest) [![Unit
-tests](https://github.com/spine-tools/Spine-Database-API/workflows/
-Unit%20tests/badge.svg)](https://github.com/spine-tools/Spine-Database-API/
+LGPL-3.0-or-later Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Operating System :: OS Independent Requires-Python: <3.12,>=3.8.1
+Description-Content-Type: text/markdown License-File: COPYING License-File:
+COPYING.LESSER # Spine Database API [![Documentation Status](https://
+readthedocs.org/projects/spine-database-api/badge/?version=latest)](https://
+spine-database-api.readthedocs.io/en/latest/?badge=latest) [![Unit tests]
+(https://github.com/spine-tools/Spine-Database-API/workflows/Unit%20tests/
+badge.svg)](https://github.com/spine-tools/Spine-Database-API/
 actions?query=workflow%3A"Unit+tests") [![codecov](https://codecov.io/gh/spine-
 tools/Spine-Database-API/branch/master/graph/badge.svg)](https://codecov.io/gh/
 spine-tools/Spine-Database-API) [![PyPI version](https://badge.fury.io/py/
 spinedb-api.svg)](https://badge.fury.io/py/spinedb-api) A Python package to
 access and manipulate Spine databases in a customary, unified way. ## License
 Spine Database API is released under the GNU Lesser General Public License
 (LGPL) license. All accompanying documentation and manual are released under
@@ -29,11 +33,7 @@
 the build, the index page can be found in `docs/build/html/index.html`.  
 ===============================================================================
 [EU     This project has received funding from European Climate, Infrastructure and
 emblem] Environment Executive Agency under the European Unionâs HORIZON Research and
         Innovation Actions under grant agreement NÂ°101095998.
 [EU     This project has received funding from the European Unionâs Horizon 2020
 emblem] research and innovation programme under grant agreement No 774629.
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent Requires-Python: <3.12,>=3.8.1
-Description-Content-Type: text/markdown
```

### Comparing `spinedb_api-0.28.0/README.md` & `spinedb_api-0.29.0/README.md`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/setup.cfg` & `spinedb_api-0.29.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/__init__.py` & `spinedb_api-0.29.0/spinedb_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,8 +124,8 @@
     config_to_shorthand,
     load_filters,
     pop_filter_configs,
     name_from_dict,
 )
 
 name = "spinedb_api"
-__version__ = "0.28.0"
+__version__ = "0.29.0"
```

### Comparing `spinedb_api-0.28.0/spinedb_api/alembic/versions/070a0eb89e88_drop_category_tables.py` & `spinedb_api-0.29.0/spinedb_api/alembic/versions/070a0eb89e88_drop_category_tables.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/alembic/versions/0c7d199ae915_add_list_value_table.py` & `spinedb_api-0.29.0/spinedb_api/alembic/versions/0c7d199ae915_add_list_value_table.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/alembic/versions/1892adebc00f_create_metadata_tables.py` & `spinedb_api-0.29.0/spinedb_api/alembic/versions/1892adebc00f_create_metadata_tables.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/alembic/versions/1e4997105288_separate_type_from_value.py` & `spinedb_api-0.29.0/spinedb_api/alembic/versions/1e4997105288_separate_type_from_value.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/alembic/versions/39e860a11b05_add_alternatives_and_scenarios.py` & `spinedb_api-0.29.0/spinedb_api/alembic/versions/39e860a11b05_add_alternatives_and_scenarios.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/alembic/versions/51fd7b69acf7_add_parameter_tag_and_parameter_value_list.py` & `spinedb_api-0.29.0/spinedb_api/alembic/versions/51fd7b69acf7_add_parameter_tag_and_parameter_value_list.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/alembic/versions/738d494a08ac_fix_foreign_key_constraints_in_object_.py` & `spinedb_api-0.29.0/spinedb_api/alembic/versions/738d494a08ac_fix_foreign_key_constraints_in_object_.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/alembic/versions/7d0b467f2f4e_fix_foreign_key_constraints_in_entity_.py` & `spinedb_api-0.29.0/spinedb_api/alembic/versions/7d0b467f2f4e_fix_foreign_key_constraints_in_entity_.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/alembic/versions/8c19c53d5701_rename_parameter_to_parameter_definition.py` & `spinedb_api-0.29.0/spinedb_api/alembic/versions/8c19c53d5701_rename_parameter_to_parameter_definition.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/alembic/versions/989fccf80441_replace_values_with_reference_to_list_.py` & `spinedb_api-0.29.0/spinedb_api/alembic/versions/989fccf80441_replace_values_with_reference_to_list_.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/alembic/versions/9da58d2def22_create_entity_group_table.py` & `spinedb_api-0.29.0/spinedb_api/alembic/versions/9da58d2def22_create_entity_group_table.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/alembic/versions/bba1e2ef5153_move_to_entity_based_design.py` & `spinedb_api-0.29.0/spinedb_api/alembic/versions/bba1e2ef5153_move_to_entity_based_design.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/alembic/versions/bf255c179bce_get_rid_of_unused_fields_in_parameter_.py` & `spinedb_api-0.29.0/spinedb_api/alembic/versions/bf255c179bce_get_rid_of_unused_fields_in_parameter_.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/alembic/versions/defbda3bf2b5_add_tool_feature_tables.py` & `spinedb_api-0.29.0/spinedb_api/alembic/versions/defbda3bf2b5_add_tool_feature_tables.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/alembic/versions/fbb540efbf15_add_support_for_mysql.py` & `spinedb_api-0.29.0/spinedb_api/alembic/versions/fbb540efbf15_add_support_for_mysql.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/alembic/versions/fd542cebf699_drop_on_update_clauses_from_object_and_.py` & `spinedb_api-0.29.0/spinedb_api/alembic/versions/fd542cebf699_drop_on_update_clauses_from_object_and_.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/check_functions.py` & `spinedb_api-0.29.0/spinedb_api/check_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,17 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """Functions for checking whether inserting data into a Spine database leads
 to the violation of integrity constraints.
 
-:author: Manuel Marin (KTH)
-:date:   4.6.2019
 """
 
-from .parameter_value import from_database, ParameterValueFormatError
+from .parameter_value import dump_db_value, from_database, ParameterValueFormatError
 from .exception import SpineIntegrityError
 
 # NOTE: We parse each parameter value or default value before accepting it. Is it too much?
 
 
 def check_alternative(item, current_items):
     try:
@@ -431,15 +429,15 @@
         parsed_value = from_database(value, value_type)
     except ParameterValueFormatError as err:
         raise SpineIntegrityError(f"Invalid {value_key} '{value}': {err}") from None
     if parsed_value is None:
         return False
     list_value_id = next((id_ for id_ in value_id_list if list_values.get(id_) == parsed_value), None)
     if list_value_id is None:
-        valid_values = ", ".join([f"'{list_values.get(id_)}'" for id_ in value_id_list])
+        valid_values = ", ".join(f"{dump_db_value(list_values.get(id_))[0].decode('utf8')!r}" for id_ in value_id_list)
         raise SpineIntegrityError(
             f"Invalid {value_key} '{parsed_value}' - it should be one from the parameter value list: {valid_values}."
         )
     item[value_key] = str(list_value_id).encode("UTF8")
     item[type_key] = "list_value_ref"
     item["list_value_id"] = list_value_id
     return True
```

### Comparing `spinedb_api-0.28.0/spinedb_api/db_cache.py` & `spinedb_api-0.29.0/spinedb_api/db_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,23 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 """
 DB cache utility.
 
-:author: Manuel Marin (ER)
-:date:   22.11.2022
 """
+from contextlib import suppress
 from operator import itemgetter
 
 
 class DBCache(dict):
     def __init__(self, advance_query, *args, **kwargs):
         """
-        A dictionary that maps table names to ids to items. Used to store and retreive database contents.
+        A dictionary that maps table names to ids to items. Used to store and retrieve database contents.
 
         Args:
             advance_query (function): A function to call when references aren't found.
                 It receives a table name (a.k.a item type) and should bring more items of that type into this cache.
         """
         super().__init__(*args, **kwargs)
         self._advance_query = advance_query
@@ -37,17 +36,22 @@
         item = table_cache.get(id_)
         if item is None:
             return {}
         return item
 
     def fetch_ref(self, item_type, id_):
         while self._advance_query(item_type):
-            ref = self.get(item_type, {}).get(id_)
-            if ref:
-                return ref
+            with suppress(KeyError):
+                return self[item_type][id_]
+        # It is possible that fetching was completed between deciding to call this function
+        # and starting the while loop above resulting in self._advance_query() to return False immediately.
+        # Therefore, we should try one last time if the ref is available.
+        with suppress(KeyError):
+            return self[item_type][id_]
+        return None
 
     def make_item(self, item_type, item):
         """Returns a cache item.
 
         Args:
             item_type (str): the item type, equal to a table name
             item (dict): the 'db item' to use as base
```

### Comparing `spinedb_api-0.28.0/spinedb_api/db_mapping.py` & `spinedb_api-0.29.0/spinedb_api/db_mapping.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Provides :class:`.DatabaseMapping`.
 
-:author: Manuel Marin (KTH)
-:date:   11.8.2018
 """
 
 from .db_mapping_query_mixin import DatabaseMappingQueryMixin
 from .db_mapping_base import DatabaseMappingBase
 from .db_mapping_add_mixin import DatabaseMappingAddMixin
 from .db_mapping_check_mixin import DatabaseMappingCheckMixin
 from .db_mapping_update_mixin import DatabaseMappingUpdateMixin
```

### Comparing `spinedb_api-0.28.0/spinedb_api/db_mapping_add_mixin.py` & `spinedb_api-0.29.0/spinedb_api/db_mapping_add_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """Provides :class:`.DatabaseMappingAddMixin`.
 
-:author: Manuel Marin (KTH)
-:date:   11.8.2018
 """
 # TODO: improve docstrings
 
 from datetime import datetime
 from sqlalchemy import func, Table, Column, Integer, String, null, select
 from sqlalchemy.exc import DBAPIError
 from .exception import SpineDBAPIError
```

### Comparing `spinedb_api-0.28.0/spinedb_api/db_mapping_base.py` & `spinedb_api-0.29.0/spinedb_api/db_mapping_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """Provides :class:`.DatabaseMappingBase`.
 
-:author: Manuel Marin (KTH)
-:date:   11.8.2018
 """
 # TODO: Finish docstrings
 import uuid
 import hashlib
 import os
 import logging
 import time
```

### Comparing `spinedb_api-0.28.0/spinedb_api/db_mapping_check_mixin.py` & `spinedb_api-0.29.0/spinedb_api/db_mapping_check_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """Provides :class:`.DatabaseMappingCheckMixin`.
 
-:author: Manuel Marin (KTH)
-:date:   11.8.2018
 """
 # TODO: Review docstrings, they are almost good
 
 from contextlib import contextmanager
 from itertools import chain
 from .exception import SpineIntegrityError
 from .check_functions import (
```

### Comparing `spinedb_api-0.28.0/spinedb_api/db_mapping_commit_mixin.py` & `spinedb_api-0.29.0/spinedb_api/db_mapping_commit_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Provides :class:`.QuickDatabaseMappingBase`.
 
-:author: Manuel Marin (KTH)
-:date:   11.8.2018
 """
 
 from datetime import datetime, timezone
 from .exception import SpineDBAPIError
 
 
 class DatabaseMappingCommitMixin:
```

### Comparing `spinedb_api-0.28.0/spinedb_api/db_mapping_query_mixin.py` & `spinedb_api-0.29.0/spinedb_api/db_mapping_query_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """Provides :class:`.DatabaseMappingQueryMixin`.
 
-:author: Manuel Marin (KTH)
-:date:   11.8.2018
 """
 # TODO: Deprecate and drop this module
 
 from sqlalchemy import func, or_
 
 
 class DatabaseMappingQueryMixin:
```

### Comparing `spinedb_api-0.28.0/spinedb_api/db_mapping_remove_mixin.py` & `spinedb_api-0.29.0/spinedb_api/db_mapping_remove_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """Provides :class:`.DiffDatabaseMappingRemoveMixin`.
 
-:author: Manuel Marin (KTH)
-:date:   11.8.2018
 """
 
 from sqlalchemy.exc import DBAPIError
 from .exception import SpineDBAPIError
 
 # TODO: improve docstrings
```

### Comparing `spinedb_api-0.28.0/spinedb_api/db_mapping_update_mixin.py` & `spinedb_api-0.29.0/spinedb_api/db_mapping_update_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """Provides :class:`DatabaseMappingUpdateMixin`.
 
-:author: Manuel Marin (KTH)
-:date:   11.8.2018
 """
 from collections import Counter
 from sqlalchemy.exc import DBAPIError
 from sqlalchemy.sql.expression import bindparam
 from .exception import SpineDBAPIError
```

### Comparing `spinedb_api-0.28.0/spinedb_api/diff_db_mapping.py` & `spinedb_api-0.29.0/spinedb_api/diff_db_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Provides :class:`DiffDatabaseMapping`.
 
-:author: Manuel Marin (KTH)
-:date:   11.8.2018
 """
 
 from sqlalchemy.sql.expression import bindparam
 from sqlalchemy.exc import DBAPIError
 from .db_mapping_query_mixin import DatabaseMappingQueryMixin
 from .db_mapping_check_mixin import DatabaseMappingCheckMixin
 from .db_mapping_add_mixin import DatabaseMappingAddMixin
```

### Comparing `spinedb_api-0.28.0/spinedb_api/diff_db_mapping_base.py` & `spinedb_api-0.29.0/spinedb_api/diff_db_mapping_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Provides :class:`.DiffDatabaseMappingBase`.
 
-:author: Manuel Marin (KTH)
-:date:   11.8.2018
 """
 
 from datetime import datetime, timezone
 from sqlalchemy import select
 from sqlalchemy.sql.expression import literal, union_all
 from .db_mapping_base import DatabaseMappingBase
 from .helpers import labelled_columns
```

### Comparing `spinedb_api-0.28.0/spinedb_api/diff_db_mapping_commit_mixin.py` & `spinedb_api-0.29.0/spinedb_api/diff_db_mapping_commit_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Provides :class:`DiffDatabaseMappingCommitMixin`.
 
-:author: Manuel Marin (KTH)
-:date:   11.8.2018
 """
 
 from datetime import datetime, timezone
 from sqlalchemy.exc import DBAPIError
 from sqlalchemy.sql.expression import bindparam
 from .exception import SpineDBAPIError
```

### Comparing `spinedb_api-0.28.0/spinedb_api/exception.py` & `spinedb_api-0.29.0/spinedb_api/exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Classes to handle exceptions while using the Spine database API.
 
-:author: Manuel Marin (KTH)
-:date:   15.8.2018
 """
 
 
 class SpineDBAPIError(Exception):
     """Basic exception for errors raised by the API."""
 
     def __init__(self, msg=None):
```

### Comparing `spinedb_api-0.28.0/spinedb_api/export_functions.py` & `spinedb_api-0.29.0/spinedb_api/export_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Functions for exporting data from a Spine database using entity names as references.
 
-:author: M. Marin (KTH)
-:date:   1.4.2020
 """
 from operator import itemgetter
 
 from sqlalchemy.util import KeyedTuple
 from .parameter_value import from_database
 from .helpers import Asterisk
```

### Comparing `spinedb_api-0.28.0/spinedb_api/export_mapping/__init__.py` & `spinedb_api-0.29.0/spinedb_api/export_mapping/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 """
 This package contains facilities to map a Spine database into tables.
 
-:author: A. Soininen (VTT)
-:date:   10.12.2020
 """
 
 from .generator import rows, titles
 from .settings import (
     alternative_export,
     feature_export,
     object_export,
```

### Comparing `spinedb_api-0.28.0/spinedb_api/export_mapping/export_mapping.py` & `spinedb_api-0.29.0/spinedb_api/export_mapping/export_mapping.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,19 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 """
 Contains export mappings for database items such as entities, entity classes and parameter values.
 
-:author: A. Soininen (VTT)
-:date:   10.12.2020
 """
 
 from dataclasses import dataclass
 from itertools import cycle, dropwhile, islice
-from sqlalchemy import and_, or_
+from sqlalchemy import and_
 from sqlalchemy.sql.expression import literal
 from ..parameter_value import (
     from_database_to_single_value,
     from_database,
     IndexedValue,
     from_database_to_dimension_count,
     map_dimensions,
@@ -53,15 +51,14 @@
 class _MappingWithLeafMixin:
     """Provides current_leaf field."""
 
     current_leaf = None
 
 
 class ExportMapping(Mapping):
-
     _TITLE_SEP = ","
 
     def __init__(self, position, value=None, header="", filter_re=""):
         """
         Args:
             position (int or Position): column index or Position
             value (Any, optional): A fixed value
@@ -738,95 +735,69 @@
     """Maps relationships classes.
 
     Can be used as the topmost mapping.
     """
 
     MAP_TYPE = "RelationshipClass"
 
+    def __init__(self, position, value=None, header="", filter_re="", highlight_dimension=None):
+        super().__init__(position, value, header, filter_re)
+        self.highlight_dimension = highlight_dimension
+
     def add_query_columns(self, db_map, query):
-        return query.add_columns(
+        query = query.add_columns(
             db_map.wide_relationship_class_sq.c.id.label("relationship_class_id"),
             db_map.wide_relationship_class_sq.c.name.label("relationship_class_name"),
             db_map.wide_relationship_class_sq.c.object_class_id_list,
             db_map.wide_relationship_class_sq.c.object_class_name_list,
         )
+        if self.highlight_dimension is not None:
+            query = query.add_columns(
+                db_map.ext_relationship_class_sq.c.object_class_id.label("highlighted_object_class_id")
+            )
+        return query
+
+    def filter_query(self, db_map, query):
+        if self.highlight_dimension is not None:
+            query = query.outerjoin(
+                db_map.ext_relationship_class_sq,
+                db_map.ext_relationship_class_sq.c.id == db_map.wide_relationship_class_sq.c.id,
+            ).filter(db_map.ext_relationship_class_sq.c.dimension == self.highlight_dimension)
+        return query
 
     @staticmethod
     def name_field():
         return "relationship_class_name"
 
     @staticmethod
     def id_field():
         # Use the class name here, for the sake of the standard excel export
         return "relationship_class_name"
 
     def query_parents(self, what):
-        if what != "dimension":
-            return super().query_parents(what)
-        return -1
+        if what == "dimension":
+            return -1
+        if what == "highlight_dimension":
+            return self.highlight_dimension
+        return super().query_parents(what)
 
     def _title_state(self, db_row):
         state = super()._title_state(db_row)
         state["object_class_id_list"] = getattr(db_row, "object_class_id_list")
         return state
 
-
-class RelationshipClassObjectHighlightingMapping(RelationshipClassMapping):
-    """Maps relationships classes.
-
-    Adds object class dimension chosen by highlight_dimension to the query.
-
-    Can be used as the topmost mapping.
-    """
-
-    MAP_TYPE = "RelationshipClassObjectHighlightingMapping"
-
-    def __init__(self, position, value=None, header="", filter_re="", highlight_dimension=0):
-        super().__init__(position, value, header, filter_re)
-        self._highlight_dimension = highlight_dimension
-
-    @property
-    def highlight_dimension(self):
-        return self._highlight_dimension
-
-    @highlight_dimension.setter
-    def highlight_dimension(self, dimension):
-        self._highlight_dimension = dimension
-
-    def add_query_columns(self, db_map, query):
-        query = super().add_query_columns(db_map, query)
-        return query.add_columns(db_map.object_class_sq.c.id.label("object_class_id"))
-
-    def filter_query(self, db_map, query):
-        highlighted_object_class_qry = db_map.query(db_map.relationship_class_sq).filter(
-            db_map.relationship_class_sq.c.dimension == self._highlight_dimension
-        )
-        conditions = (
-            and_(db_map.wide_relationship_class_sq.c.id == x.id, db_map.object_class_sq.c.id == x.object_class_id)
-            for x in highlighted_object_class_qry
-        )
-        return query.filter(or_(*conditions))
-
-    @staticmethod
-    def id_field():
-        return "relationship_class_id"
-
-    def query_parents(self, what):
-        if what != "highlight_dimension":
-            return super().query_parents(what)
-        return self._highlight_dimension
-
     def to_dict(self):
         mapping_dict = super().to_dict()
-        mapping_dict["highlight_dimension"] = self._highlight_dimension
+        if self.highlight_dimension is not None:
+            mapping_dict["highlight_dimension"] = self.highlight_dimension
         return mapping_dict
 
     @classmethod
     def reconstruct(cls, position, value, header, filter_re, ignorable, mapping_dict):
-        highlight_dimension = mapping_dict["highlight_dimension"]
+        highlight_dimension = mapping_dict.get("highlight_dimension")
         mapping = cls(position, value, header, filter_re, highlight_dimension)
         mapping.set_ignorable(ignorable)
         return mapping
 
 
 class RelationshipClassObjectClassMapping(ExportMapping):
     """Maps relationship class object classes.
@@ -869,26 +840,34 @@
 
     Cannot be used as the topmost mapping; one of the parents must be :class:`RelationshipClassMapping`.
     """
 
     MAP_TYPE = "Relationship"
 
     def add_query_columns(self, db_map, query):
-        return query.add_columns(
+        query = query.add_columns(
             db_map.wide_relationship_sq.c.id.label("relationship_id"),
             db_map.wide_relationship_sq.c.name.label("relationship_name"),
             db_map.wide_relationship_sq.c.object_id_list,
             db_map.wide_relationship_sq.c.object_name_list,
         )
+        if self.query_parents("highlight_dimension") is not None:
+            query = query.add_columns(db_map.ext_relationship_sq.c.object_id.label("highlighted_object_id"))
+        return query
 
     def filter_query(self, db_map, query):
-        return query.outerjoin(
+        query = query.outerjoin(
             db_map.wide_relationship_sq,
             db_map.wide_relationship_sq.c.class_id == db_map.wide_relationship_class_sq.c.id,
         )
+        if (highlight_dimension := self.query_parents("highlight_dimension")) is not None:
+            query = query.outerjoin(
+                db_map.ext_relationship_sq, db_map.ext_relationship_sq.c.id == db_map.wide_relationship_sq.c.id
+            ).filter(db_map.ext_relationship_sq.c.dimension == highlight_dimension)
+        return query
 
     @staticmethod
     def name_field():
         return "relationship_name"
 
     @staticmethod
     def id_field():
@@ -905,44 +884,14 @@
         return state
 
     @staticmethod
     def is_buddy(parent):
         return isinstance(parent, RelationshipClassMapping)
 
 
-class RelationshipObjectHighlightingMapping(RelationshipMapping):
-    """Maps relationships.
-
-    Adds object dimension chosen by highlight_dimension in relationship class mapping to the query.
-
-    Cannot be used as the topmost mapping;
-    one of the parents must be :class:`RelationshipClassObjectHighlightingMapping`.
-    """
-
-    MAP_TYPE = "RelationshipObjectHighlightingMapping"
-
-    def add_query_columns(self, db_map, query):
-        query = super().add_query_columns(db_map, query)
-        return query.add_columns(db_map.object_sq.c.id.label("object_id"))
-
-    def filter_query(self, db_map, query):
-        highlighted_object_qry = db_map.query(db_map.relationship_sq).filter(
-            db_map.relationship_sq.c.dimension == self.query_parents("highlight_dimension")
-        )
-        conditions = (
-            and_(db_map.wide_relationship_sq.c.id == x.id, db_map.object_sq.c.id == x.object_id)
-            for x in highlighted_object_qry
-        )
-        return query.filter(or_(*conditions))
-
-    @staticmethod
-    def is_buddy(parent):
-        return isinstance(parent, RelationshipClassObjectHighlightingMapping)
-
-
 class RelationshipObjectMapping(ExportMapping):
     """Maps relationship's objects.
 
     Cannot be used as the topmost mapping; must have :class:`RelationshipClassMapping` and :class:`RelationshipMapping`
     as parents.
     """
 
@@ -994,14 +943,20 @@
         column_names = {c["name"] for c in query.column_descriptions}
         if "object_class_id" in column_names:
             return query.outerjoin(
                 db_map.parameter_definition_sq,
                 db_map.parameter_definition_sq.c.object_class_id == db_map.object_class_sq.c.id,
             )
         if "relationship_class_id" in column_names:
+            if self.query_parents("highlight_dimension") is not None:
+                return query.outerjoin(
+                    db_map.parameter_definition_sq,
+                    db_map.parameter_definition_sq.c.object_class_id
+                    == db_map.ext_relationship_class_sq.c.object_class_id,
+                )
             return query.outerjoin(
                 db_map.parameter_definition_sq,
                 db_map.parameter_definition_sq.c.relationship_class_id == db_map.wide_relationship_class_sq.c.id,
             )
         raise RuntimeError("Logic error: this code should be unreachable.")
 
     @staticmethod
@@ -1179,14 +1134,21 @@
             return query.filter(
                 and_(
                     db_map.parameter_value_sq.c.object_id == db_map.object_sq.c.id,
                     db_map.parameter_value_sq.c.parameter_definition_id == db_map.parameter_definition_sq.c.id,
                 )
             )
         if "relationship_id" in column_names:
+            if self.query_parents("highlight_dimension") is not None:
+                return query.filter(
+                    and_(
+                        db_map.parameter_value_sq.c.object_id == db_map.ext_relationship_sq.c.object_id,
+                        db_map.parameter_value_sq.c.parameter_definition_id == db_map.parameter_definition_sq.c.id,
+                    )
+                )
             return query.filter(
                 and_(
                     db_map.parameter_value_sq.c.relationship_id == db_map.wide_relationship_sq.c.id,
                     db_map.parameter_value_sq.c.parameter_definition_id == db_map.parameter_definition_sq.c.id,
                 )
             )
         raise RuntimeError("Logic error: this code should be unreachable.")
@@ -1874,17 +1836,15 @@
             ParameterValueIndexMapping,
             ParameterValueListMapping,
             ParameterValueListValueMapping,
             ParameterValueMapping,
             ParameterValueTypeMapping,
             RelationshipClassMapping,
             RelationshipClassObjectClassMapping,
-            RelationshipClassObjectHighlightingMapping,
             RelationshipMapping,
-            RelationshipObjectHighlightingMapping,
             RelationshipObjectMapping,
             ScenarioActiveFlagMapping,
             ScenarioAlternativeMapping,
             ScenarioBeforeAlternativeMapping,
             ScenarioDescriptionMapping,
             ScenarioMapping,
             ToolMapping,
@@ -1893,14 +1853,16 @@
             ToolFeatureRequiredFlagMapping,
             ToolFeatureMethodEntityClassMapping,
             ToolFeatureMethodParameterDefinitionMapping,
         )
     }
     # Legacy
     mappings["ParameterIndex"] = ParameterValueIndexMapping
+    if any(m["map_type"] == "RelationshipClassObjectHighlightingMapping" for m in serialized):
+        _upgrade_legacy_object_highlighting_mapping(serialized)
     flattened = list()
     for mapping_dict in serialized:
         position = mapping_dict["position"]
         if isinstance(position, str):
             position = Position(position)
         ignorable = mapping_dict.get("ignorable", False)
         value = mapping_dict.get("value")
@@ -1926,14 +1888,30 @@
     for mapping_dict in serialized:
         group_fn = mapping_dict.get("group_fn")
         if group_fn is not None:
             return group_fn
     return NoGroup.NAME
 
 
+def _upgrade_legacy_object_highlighting_mapping(serialized):
+    """Upgrades legacy object highlighting mappings in place.
+
+    ``RelationshipClassObjectHighlightingMapping`` and ``RelationshipObjectHighlightingMapping``
+    have been replaced by a ``highlight_dimension`` argument in ``RelationshipClassObjectClassMapping``.
+
+    Args:
+        serialized (list of dict): serialized mappings
+    """
+    for mapping_dict in serialized:
+        if mapping_dict["map_type"] == "RelationshipClassObjectHighlightingMapping":
+            mapping_dict["map_type"] = RelationshipClassMapping.MAP_TYPE
+        elif mapping_dict["map_type"] == "RelationshipObjectHighlightingMapping":
+            mapping_dict["map_type"] = RelationshipMapping.MAP_TYPE
+
+
 def _expand_indexed_data(data, mapping):
     """Expands indexed data and updates the current_leaf attribute.
 
     Args:
         data (Any): data to expand
         mapping (ExportMapping): mapping whose data is being expanded
```

### Comparing `spinedb_api-0.28.0/spinedb_api/export_mapping/generator.py` & `spinedb_api-0.29.0/spinedb_api/export_mapping/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 """
 Contains generator functions that convert a Spine database into rows of tabular data.
 
-:author: A. Soininen (VTT)
-:date:   10.12.2020
 """
 from copy import deepcopy
 from ..mapping import Position
 from .pivot import make_pivot, make_regular
 from .export_mapping import pair_header_buddies
 from .group_functions import NoGroup
```

### Comparing `spinedb_api-0.28.0/spinedb_api/export_mapping/group_functions.py` & `spinedb_api-0.29.0/spinedb_api/export_mapping/group_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 """
 Contains functions to group values in pivot tables with hidden columns or rows.
 
-:author: M. Marin (KTH)
-:date:   7.3.2021
 """
 import numpy as np
 
 
 class GroupFunction:
     NAME = NotImplemented
     DISPLAY_NAME = NotImplemented
```

### Comparing `spinedb_api-0.28.0/spinedb_api/export_mapping/pivot.py` & `spinedb_api-0.29.0/spinedb_api/export_mapping/pivot.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 """
 Contains functions and methods to turn a regular export table into a pivot table
 
-:author: A. Soininen (VTT)
-:date:   1.2.2021
 """
 from copy import deepcopy
 
 from .export_mapping import RelationshipMapping
 from ..mapping import is_regular, is_pivoted, Position, unflatten, value_index
 from .group_functions import from_str as group_function_from_str, NoGroup
```

### Comparing `spinedb_api-0.28.0/spinedb_api/export_mapping/settings.py` & `spinedb_api-0.29.0/spinedb_api/export_mapping/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 """
 Contains convenience functions to set up different database export schemes.
 
-:author: A. Soininen (VTT)
-:date:   10.12.2020
 """
 from itertools import takewhile
 
 from .export_mapping import (
     AlternativeMapping,
     AlternativeDescriptionMapping,
     ExpandedParameterDefaultValueMapping,
@@ -34,17 +32,15 @@
     ParameterValueListMapping,
     ParameterValueListValueMapping,
     ParameterValueMapping,
     ParameterValueTypeMapping,
     Position,
     RelationshipClassMapping,
     RelationshipClassObjectClassMapping,
-    RelationshipClassObjectHighlightingMapping,
     RelationshipMapping,
-    RelationshipObjectHighlightingMapping,
     RelationshipObjectMapping,
     ScenarioActiveFlagMapping,
     ScenarioAlternativeMapping,
     ScenarioBeforeAlternativeMapping,
     ScenarioMapping,
     ScenarioDescriptionMapping,
     ToolFeatureEntityClassMapping,
@@ -319,17 +315,15 @@
         highlight_dimension (int): selected object class' relationship dimension
 
     Returns:
         ExportMapping: root mapping
     """
     root_mapping = unflatten(
         [
-            RelationshipClassObjectHighlightingMapping(
-                relationship_class_position, highlight_dimension=highlight_dimension
-            ),
+            RelationshipClassMapping(relationship_class_position, highlight_dimension=highlight_dimension),
             ParameterDefinitionMapping(definition_position),
         ]
     )
     _generate_dimensions(root_mapping.tail_mapping(), RelationshipClassObjectClassMapping, object_class_positions)
     _generate_default_value_mappings(
         root_mapping.tail_mapping(), value_type_position, value_position, index_name_positions, index_positions
     )
@@ -370,25 +364,23 @@
     Returns:
         ExportMapping: root mapping
     """
     if object_class_positions is None:
         object_class_positions = list()
     if object_positions is None:
         object_positions = list()
-    relationship_class = RelationshipClassObjectHighlightingMapping(
-        relationship_class_position, highlight_dimension=highlight_dimension
-    )
+    relationship_class = RelationshipClassMapping(relationship_class_position, highlight_dimension=highlight_dimension)
     object_or_relationship_class = _generate_dimensions(
         relationship_class, RelationshipClassObjectClassMapping, object_class_positions
     )
     value_list = ParameterValueListMapping(value_list_position)
     value_list.set_ignorable(True)
     definition = ParameterDefinitionMapping(definition_position)
     object_or_relationship_class.child = definition
-    relationship = RelationshipObjectHighlightingMapping(relationship_position)
+    relationship = RelationshipMapping(relationship_position)
     definition.child = value_list
     value_list.child = relationship
     object_or_relationship = _generate_dimensions(relationship, RelationshipObjectMapping, object_positions)
     _generate_parameter_value_mappings(
         object_or_relationship,
         alternative_position,
         value_type_position,
```

### Comparing `spinedb_api-0.28.0/spinedb_api/filters/__init__.py` & `spinedb_api-0.29.0/spinedb_api/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/filters/alternative_filter.py` & `spinedb_api-0.29.0/spinedb_api/filters/alternative_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Provides functions to apply filtering based on alternatives to parameter value subqueries.
 
-:author: Antti Soininen (VTT)
-:date:   21.8.2020
 """
 from functools import partial
 from ..exception import SpineDBAPIError
 
 
 ALTERNATIVE_FILTER_TYPE = "alternative_filter"
 ALTERNATIVE_FILTER_SHORTHAND_TAG = "alternatives"
```

### Comparing `spinedb_api-0.28.0/spinedb_api/filters/execution_filter.py` & `spinedb_api-0.29.0/spinedb_api/filters/execution_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Provides functions to apply filtering based on scenarios to parameter value subqueries.
 
-:author: Antti Soininen (VTT)
-:date:   21.8.2020
 """
 
 import json
 from functools import partial
 from sqlalchemy import func
 from ..exception import SpineDBAPIError
```

### Comparing `spinedb_api-0.28.0/spinedb_api/filters/renamer.py` & `spinedb_api-0.29.0/spinedb_api/filters/renamer.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Provides a database query manipulator that renames database items.
 
-:author: A. Soininen
-:date:   2.10.2020
 """
 from functools import partial
 from sqlalchemy import case
 
 
 ENTITY_CLASS_RENAMER_TYPE = "entity_class_renamer"
 ENTITY_CLASS_RENAMER_SHORTHAND_TAG = "entity_class_rename"
```

### Comparing `spinedb_api-0.28.0/spinedb_api/filters/scenario_filter.py` & `spinedb_api-0.29.0/spinedb_api/filters/scenario_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Provides functions to apply filtering based on scenarios to subqueries.
 
-:author: Antti Soininen (VTT)
-:date:   21.8.2020
 """
 
 from functools import partial
 from sqlalchemy import desc, func
 from ..exception import SpineDBAPIError
 
 SCENARIO_FILTER_TYPE = "scenario_filter"
```

### Comparing `spinedb_api-0.28.0/spinedb_api/filters/tool_filter.py` & `spinedb_api-0.29.0/spinedb_api/filters/tool_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Provides functions to apply filtering based on tools to entity subqueries.
 
-:author: M. Marin (KTH)
-:date:   23.9.2020
 """
 from functools import partial
 from uuid import uuid4
 from sqlalchemy import and_, or_, case, func, Table, Column, ForeignKey
 from ..exception import SpineDBAPIError
```

### Comparing `spinedb_api-0.28.0/spinedb_api/filters/tools.py` & `spinedb_api-0.29.0/spinedb_api/filters/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Tools and utilities to work with filters, manipulators and database URLs.
 
-:author: A. Soininen
-:date:   7.12.2020
 """
 from json import dump, load
 from urllib.parse import parse_qs, urlencode, urlparse, urlunparse
 from .alternative_filter import (
     ALTERNATIVE_FILTER_SHORTHAND_TAG,
     ALTERNATIVE_FILTER_TYPE,
     alternative_filter_config,
```

### Comparing `spinedb_api-0.28.0/spinedb_api/filters/value_transformer.py` & `spinedb_api-0.29.0/spinedb_api/filters/value_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Provides a database query manipulator that applies mathematical transformations to parameter values.
 
-:author: A. Soininen
-:date:   20.5.2021
 """
 from functools import partial
 from numbers import Number
 from sqlalchemy import case, literal, Integer, LargeBinary, String
 from sqlalchemy.sql.expression import label, select, cast, union_all
 
 from ..exception import SpineDBAPIError
```

### Comparing `spinedb_api-0.28.0/spinedb_api/graph_layout_generator.py` & `spinedb_api-0.29.0/spinedb_api/graph_layout_generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,60 +8,58 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains the GraphLayoutGenerator class.
 
-:authors: M. Marin (ER)
-:date:   18.5.2022
 """
 
 import math
 import numpy as np
 from numpy import atleast_1d as arr
 from scipy.sparse.csgraph import dijkstra
 
 
 class GraphLayoutGenerator:
     """Computes the layout for the Entity Graph View."""
 
     def __init__(
-        self, vertex_count, src_inds=(), dst_inds=(), spread=0, heavy_positions=None, max_iters=12, weight_exp=-2
+        self,
+        vertex_count,
+        src_inds=(),
+        dst_inds=(),
+        spread=0,
+        heavy_positions=None,
+        max_iters=12,
+        weight_exp=-2,
+        is_stopped=lambda: False,
+        preview_available=lambda x, y: None,
+        layout_available=lambda x, y: None,
+        layout_progressed=lambda iter: None,
+        message_available=lambda msg: None,
     ):
         super().__init__()
         if vertex_count == 0:
             vertex_count = 1
         if heavy_positions is None:
             heavy_positions = dict()
-        self._show_previews = False
         self.vertex_count = vertex_count
         self.src_inds = src_inds
         self.dst_inds = dst_inds
         self.spread = spread
         self.heavy_positions = heavy_positions
         self.max_iters = max(3, round(max_iters * (1 - len(heavy_positions) / self.vertex_count)))
         self.weight_exp = weight_exp
         self.initial_diameter = (self.vertex_count ** (0.5)) * self.spread
-        self._stopped = False
-        self.x = None
-        self.y = None
-
-    def stop(self):
-        self._stopped = True
-
-    def save_layout(self, x, y):
-        self.x = x
-        self.y = y
-
-    def emit_progressed(self, iteration):
-        """Emits progressed"""
-
-    def emit_msg(self, text):
-        """Emits msg"""
+        self._is_stopped = is_stopped
+        self._preview_available = preview_available
+        self._layout_available = layout_available
+        self._layout_progressed = layout_progressed
+        self._message_available = message_available
 
     def shortest_path_matrix(self):
         """Returns the shortest-path matrix."""
         if not self.src_inds:
             # Graph with no edges, just vertices. Introduce fake pair of edges to help 'spreadness'.
             self.src_inds = [self.vertex_count, self.vertex_count]
             self.dst_inds = [np.random.randint(0, self.vertex_count), np.random.randint(0, self.vertex_count)]
@@ -72,19 +70,19 @@
         try:
             dist[src_inds, dst_inds] = dist[dst_inds, src_inds] = self.spread
         except IndexError:
             pass
         start = 0
         slices = []
         iteration = 0
-        self.emit_msg("Step 1 of 2: Computing shortest-path matrix...")
+        self._message_available("Step 1 of 2: Computing shortest-path matrix...")
         while start < self.vertex_count:
-            if self._stopped:
+            if self._is_stopped():
                 return None
-            self.emit_progressed(iteration)
+            self._layout_progressed(iteration)
             stop = min(self.vertex_count, start + math.ceil(self.vertex_count / 10))
             slice_ = dijkstra(dist, directed=False, indices=range(start, stop))
             slices.append(slice_)
             start = stop
             iteration += 1
         matrix = np.vstack(slices)
         # Remove infinites and zeros
@@ -108,15 +106,15 @@
                 sets.append(s2)
         return sets
 
     def compute_layout(self):
         """Computes and returns x and y coordinates for each vertex in the graph, using VSGD-MS."""
         if self.vertex_count <= 1:
             x, y = np.array([0.0]), np.array([0.0])
-            self.save_layout(x, y)
+            self._layout_available(x, y)
             return
         matrix = self.shortest_path_matrix()
         if matrix is None:
             return
         mask = np.ones((self.vertex_count, self.vertex_count)) == 1 - np.tril(
             np.ones((self.vertex_count, self.vertex_count))
         )  # Upper triangular except diagonal
@@ -132,22 +130,21 @@
         if heavy_ind.any():
             layout[heavy_ind, :] = heavy_pos
         weights = matrix ** self.weight_exp  # bus-pair weights (lower for distant buses)
         maxstep = 1 / np.min(weights[mask])
         minstep = 1 / np.max(weights[mask])
         lambda_ = np.log(minstep / maxstep) / (self.max_iters - 1)  # exponential decay of allowed adjustment
         sets = self.sets()  # construct sets of bus pairs
-        self.emit_msg("Step 2 of 2: Generating layout...")
+        self._message_available("Step 2 of 2: Generating layout...")
         for iteration in range(self.max_iters):
-            if self._stopped:
+            if self._is_stopped():
                 break
-            if self._show_previews:
-                x, y = layout[:, 0], layout[:, 1]
-                self.save_layout(x, y)
-            self.emit_progressed(iteration)
+            x, y = layout[:, 0], layout[:, 1]
+            self._preview_available(x, y)
+            self._layout_progressed(iteration)
             # FIXME
             step = maxstep * np.exp(lambda_ * iteration)  # how big adjustments are allowed?
             rand_order = np.random.permutation(
                 self.vertex_count
             )  # we don't want to use the same pair order each iteration
             for s in sets:
                 v1, v2 = rand_order[s[:, 0]], rand_order[s[:, 1]]  # arrays of vertex1 and vertex2
@@ -157,8 +154,8 @@
                 dx1 = r * np.minimum(1, weights[v1, v2] * step)[:, None]
                 dx2 = -dx1
                 layout[v1, :] += dx1  # update position
                 layout[v2, :] += dx2
                 if heavy_ind.any():
                     layout[heavy_ind, :] = heavy_pos
         x, y = layout[:, 0], layout[:, 1]
-        self.save_layout(x, y)
+        self._layout_available(x, y)
```

### Comparing `spinedb_api-0.28.0/spinedb_api/helpers.py` & `spinedb_api-0.29.0/spinedb_api/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 General helper functions and classes.
 
-:author: Manuel Marin (KTH)
-:date:   15.8.2018
 """
 
 import os
 import json
 import warnings
 from operator import itemgetter
 from urllib.parse import urlparse, urlunparse
@@ -74,14 +72,15 @@
     "ck": "ck_%(table_name)s_%(constraint_name)s",
 }
 
 model_meta = MetaData(naming_convention=naming_convention)
 
 LONGTEXT_LENGTH = 2 ** 32 - 1
 
+
 # NOTE: Deactivated since foreign keys are too difficult to get right in the diff tables.
 # For example, the diff_object table would need a `class_id` field and a `diff_class_id` field,
 # plus a CHECK constraint that at least one of the two is NOT NULL.
 # @event.listens_for(Engine, "connect")
 def set_sqlite_pragma(dbapi_connection, connection_record):
     module_name = dbapi_connection.__class__.__module__
     if not module_name.lower().startswith("sqlite"):
@@ -178,14 +177,15 @@
     with engine.connect() as connection:
         migration_context = MigrationContext.configure(connection)
         current_rev = migration_context.get_current_revision()
         if current_rev == head:
             return True
         if not upgrade:
             return False
+
         # Upgrade function
         def fn(rev, context):
             return script._upgrade_revs("head", rev)
 
         with EnvironmentContext(
             config, script, fn=fn, as_sql=False, starting_rev=None, destination_rev="head", tag=None
         ) as environment_context:
```

### Comparing `spinedb_api-0.28.0/spinedb_api/import_functions.py` & `spinedb_api-0.29.0/spinedb_api/import_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Functions for importing data into a Spine database using entity names as references.
 
-:author: P. Vennström (VTT)
-:date:   17.12.2018
 """
 
 import uuid
 from .exception import SpineIntegrityError, SpineDBAPIError
 from .check_functions import (
     check_tool,
     check_feature,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spinedb_api-0.28.0/spinedb_api/import_mapping/__init__.py` & `spinedb_api-0.29.0/spinedb_api/import_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `spinedb_api-0.28.0/spinedb_api/import_mapping/generator.py` & `spinedb_api-0.29.0/spinedb_api/import_mapping/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains `get_mapped_data()` that converts rows of tabular data into a dictionary for import to a Spine DB,
 using ``import_functions.import_data()``
 
-:author: P. Vennström (VTT)
-:date:   22.02.2018
 """
 
 from copy import deepcopy
 from .import_mapping_compat import import_mapping_from_dict
 from .import_mapping import ImportMapping, check_validity
 from ..mapping import Position
 from ..parameter_value import (
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spinedb_api-0.28.0/spinedb_api/import_mapping/import_mapping.py` & `spinedb_api-0.29.0/spinedb_api/import_mapping/import_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 """
 Contains import mappings for database items such as entities, entity classes and parameter values.
 
-:author: A. Soininen (VTT)
-:date:   10.12.2020
 """
 
 from distutils.util import strtobool
 from enum import auto, Enum, unique
 from spinedb_api.mapping import Mapping, Position, unflatten, is_pivoted
 from spinedb_api.exception import InvalidMappingComponent
```

### Comparing `spinedb_api-0.28.0/spinedb_api/import_mapping/import_mapping_compat.py` & `spinedb_api-0.29.0/spinedb_api/import_mapping/import_mapping_compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Functions for creating import mappings from dicts.
 
-:author: P. Vennström (VTT)
-:date:   22.02.2018
 """
 from .import_mapping import (
     Position,
     ObjectClassMapping,
     RelationshipClassMapping,
     RelationshipClassObjectClassMapping,
     ObjectMapping,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spinedb_api-0.28.0/spinedb_api/import_mapping/type_conversion.py` & `spinedb_api-0.29.0/spinedb_api/import_mapping/type_conversion.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Type conversion functions.
 
-:author: P. Vennström (VTT)
-:date:   21.11.2019
 """
 
 import re
 from distutils.util import strtobool
 from spinedb_api.parameter_value import DateTime, Duration, ParameterValueFormatError
 
 
@@ -42,15 +40,20 @@
 
 
 class ConvertSpec:
     DISPLAY_NAME = ""
     RETURN_TYPE = str
 
     def __call__(self, value):
-        return self.RETURN_TYPE(value)
+        try:
+            return self.RETURN_TYPE(value)
+        except ValueError as error:
+            if not value:
+                return None
+            raise error
 
     def to_json_value(self):
         return self.DISPLAY_NAME
 
 
 class DateTimeConvertSpec(ConvertSpec):
     DISPLAY_NAME = "datetime"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spinedb_api-0.28.0/spinedb_api/mapping.py` & `spinedb_api-0.29.0/spinedb_api/mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 """
 Contains export mappings for database items such as entities, entity classes and parameter values.
 
-:author: A. Soininen (VTT)
-:date:   10.12.2020
 """
 
 from enum import Enum, unique
 from itertools import takewhile
 import re
```

### Comparing `spinedb_api-0.28.0/spinedb_api/parameter_value.py` & `spinedb_api-0.29.0/spinedb_api/parameter_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 or by their `to_database` member functions.
 
 Individual datetimes are represented as datetime objects from the standard Python library.
 Individual time steps are represented as relativedelta objects from the dateutil package.
 Datetime indexes (as returned by TimeSeries.indexes()) are represented as
 numpy.ndarray arrays holding numpy.datetime64 objects.
 
-:author: A. Soininen (VTT)
-:date:   3.6.2019
 """
 
 from collections.abc import Sequence
 from copy import copy
 from datetime import datetime
 import json
 from json.decoder import JSONDecodeError
```

### Comparing `spinedb_api-0.28.0/spinedb_api/perfect_split.py` & `spinedb_api-0.29.0/spinedb_api/perfect_split.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Functions for the perfect db split.
 
-:author: M. Marin (ER)
-:date:   27.1.2022
 """
 from .db_mapping import DatabaseMapping
 from .export_functions import export_data
 from .import_functions import import_data
 
 
 def perfect_split(input_urls, intersection_url, diff_urls):
```

### Comparing `spinedb_api-0.28.0/spinedb_api/purge.py` & `spinedb_api-0.29.0/spinedb_api/purge.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Functions to purge dbs.
 
-:authors: A. Soininen (VTT), M. Marin (ER)
-:date:   27.1.2022
 """
 
 from .db_mapping import DatabaseMapping
 from .exception import SpineDBAPIError, SpineDBVersionError
 from .filters.tools import clear_filter_configs
 from .helpers import remove_credentials_from_url
```

### Comparing `spinedb_api-0.28.0/spinedb_api/server_client_helpers.py` & `spinedb_api-0.29.0/spinedb_api/server_client_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Helpers for server and client.
 
-:author: Manuel Marin (ER)
-:date:   16.9.2022
 """
 
 import json
 from .import_functions import ImportErrorLogItem
 from .exception import SpineDBAPIError
 
 # Encode decode server messages
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_db_client.py` & `spinedb_api-0.29.0/spinedb_api/spine_db_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains the SpineDBClient class.
 
-:authors: M. Marin (KTH)
-:date:   19.2.2020
 """
 
 from urllib.parse import urlparse
 import socket
 from sqlalchemy.engine.url import URL
 from .server_client_helpers import ReceiveAllMixing, encode, decode
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_db_server.py` & `spinedb_api-0.29.0/spinedb_api/spine_db_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains the SpineDBServer class.
 
-:authors: M. Marin (KTH)
-:date:   2.2.2020
 """
 
 from urllib.parse import urlunsplit
 from contextlib import contextmanager
 import socketserver
 import multiprocessing as mp
 from multiprocessing.queues import Queue as MPQueue
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_io/__init__.py` & `spinedb_api-0.29.0/spinedb_api/spine_io/importers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,12 +6,10 @@
 # option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
-Init file for spine_io package. Intentionally empty.
+Intentionally empty.
 
-:author: P. Vennström (VTT)
-:date:   1.6.2019
 """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_io/exporters/__init__.py` & `spinedb_api-0.29.0/spinedb_api/spine_io/exporters/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,10 +8,8 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Init file for spine_io.exporters package. Intentionally empty.
 
-:author: A. Soininen (VTT)
-:date:   30.8.2019
 """
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_io/exporters/csv_writer.py` & `spinedb_api-0.29.0/spinedb_api/spine_io/exporters/csv_writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 """
 Module contains a .csv writer implementation.
 
-:author: A. Soininen (VTT)
-:date:   9.12.2020
 """
 import csv
 import os
 import os.path
 from .writer import Writer
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_io/exporters/excel.py` & `spinedb_api-0.29.0/spinedb_api/spine_io/exporters/excel.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Framework for exporting a database to Excel file.
 
-:author: P. Vennström (VTT), A. Soininen (VTT), M. Marin (KTH)
-:date:   31.1.2020
 """
 from spinedb_api.export_mapping.group_functions import GroupOneOrNone
 from spinedb_api.export_mapping.export_mapping import (
     Position,
     AlternativeMapping,
     AlternativeDescriptionMapping,
     ObjectClassMapping,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_io/exporters/excel_writer.py` & `spinedb_api-0.29.0/spinedb_api/spine_io/exporters/excel_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 A writer for exporting Spine databases to Excel files.
 
-:author: A. Soininen (VTT)
-:date:   15.1.2021
 """
 from pathlib import Path
 import re
 import numpy
 from openpyxl import load_workbook, Workbook
 from openpyxl.utils.exceptions import InvalidFileException
 from openpyxl.workbook.child import INVALID_TITLE_REGEX
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_io/exporters/gdx_writer.py` & `spinedb_api-0.29.0/spinedb_api/spine_io/exporters/gdx_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 """
 Module contains a .gdx writer implementation.
 
-:author: A. Soininen (VTT)
-:date:   9.12.2020
 """
 import math
 from gdx2py import GAMSSet, GAMSScalar, GAMSParameter, GdxFile
 from gdx2py.gdxfile import EPS_VALUE
 import gdxcc
 from .writer import Writer, WriterException
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_io/exporters/sql_writer.py` & `spinedb_api-0.29.0/spinedb_api/spine_io/exporters/sql_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 """
 Module contains an SQL writer implementation.
 
-:author: A. Soininen (VTT)
-:date:   7.4.2021
 """
 from sqlalchemy import Boolean, Column, create_engine, Float, Integer, MetaData, String, Table, DateTime
 from sqlalchemy.orm import Session
 from spinedb_api import parameter_value
 from .writer import Writer, WriterException
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_io/exporters/writer.py` & `spinedb_api-0.29.0/spinedb_api/spine_io/exporters/writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 """
 Module contains the :class:`Writer` base class and functions to write tabular data.
 
-:author: A. Soininen (VTT)
-:date:   8.12.2020
 """
 from contextlib import contextmanager
 from copy import copy
 from sqlalchemy.exc import OperationalError
 
 from spinedb_api import SpineDBAPIError
 from spinedb_api.export_mapping import rows, titles
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_io/gdx_utils.py` & `spinedb_api-0.29.0/spinedb_api/spine_io/gdx_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Utility functions for .gdx import/export.
 
-:author: A. Soininen (VTT)
-:date:   7.1.2020
 """
 
 import os
 import sys
 
 if sys.platform == "win32":
     import winreg
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_io/importers/__init__.py` & `spinedb_api-0.29.0/spinedb_api/spine_io/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,12 +6,10 @@
 # option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
-Intentionally empty.
+Init file for spine_io package. Intentionally empty.
 
-:author: P. Vennström (VTT)
-:date:   1.6.2019
 """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_io/importers/csv_reader.py` & `spinedb_api-0.29.0/spinedb_api/spine_io/importers/csv_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains CSVConnector class and a help function.
 
-:author: P. Vennström (VTT)
-:date:   1.6.2019
 """
 
 
 import csv
 from itertools import islice
 import chardet
 from .reader import SourceConnection
@@ -156,21 +154,19 @@
             max_rows += skip
         with open(self._filename, encoding=encoding) as text_file:
             csv_reader = csv.reader(text_file, **dialect)
             csv_reader = islice(csv_reader, skip, max_rows)
             yield from csv_reader
 
     def get_data_iterator(self, table, options, max_rows=-1):
-        """Creates an iterator for the file in self.filename
+        """Creates an iterator for the file in self.filename.
 
         Arguments:
             table (string): ignored, used in abstract IOWorker class
             options (dict): dict with options
-
-        Keyword Arguments:
             max_rows (int): how many rows of data to read, if -1 read all rows (default: {-1})
 
         Returns:
             tuple:
         """
         csv_iter = self.file_iterator(options, max_rows)
         try:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_io/importers/datapackage_reader.py` & `spinedb_api-0.29.0/spinedb_api/spine_io/importers/datapackage_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains DataPackageConnector class.
 
-:author: M. Marin (KTH)
-:date:   15.11.2020
 """
 import threading
 from itertools import chain
 
 from datapackage import Package
 from .reader import SourceConnection
 
@@ -65,16 +63,15 @@
             source (str): filepath of a datapackage.json file
         """
         if source:
             self._datapackage = Package(source)
             self._filename = source
 
     def disconnect(self):
-        """Disconnect from connected source.
-        """
+        """Disconnect from connected source."""
         if self._datapackage:
             self._datapackage = None
         self._filename = None
 
     def get_tables(self):
         """Returns resources' mappings and their options.
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_io/importers/excel_reader.py` & `spinedb_api-0.29.0/spinedb_api/spine_io/importers/excel_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains ExcelConnector class and a help function.
 
-:author: P. Vennström (VTT)
-:date:   1.6.2019
 """
 
 from itertools import islice, takewhile, chain
 import io
 from openpyxl import load_workbook
 from .reader import SourceConnection
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_io/importers/gdx_connector.py` & `spinedb_api-0.29.0/spinedb_api/spine_io/importers/gdx_connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains GDXConnector class and a help function.
 
-:author: P. Vennström (VTT)
-:date:   1.6.2019
 """
 
 from gdx2py import GdxFile, GAMSParameter, GAMSScalar, GAMSSet
 
 from spinedb_api import SpineDBAPIError
 from .reader import SourceConnection
 from ..gdx_utils import find_gams_directory
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_io/importers/json_reader.py` & `spinedb_api-0.29.0/spinedb_api/spine_io/importers/json_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains JSONConnector class.
 
-:author: M. Marin (KTH)
-:date:   10.2.2020
 """
 
 import sys
 import os
 import ijson
 from .reader import SourceConnection
 
@@ -38,49 +36,48 @@
         super().__init__(settings)
         self._filename = None
         self._root_prefix = None
 
     def connect_to_source(self, source):
         """saves filepath
 
-        Arguments:
-            source {str} -- filepath
+        Args:
+            source (str): filepath
         """
         self._filename = source
         self._root_prefix = os.path.splitext(os.path.basename(source))[0]
 
     def disconnect(self):
-        """Disconnect from connected source.
-        """
+        """Disconnect from connected source."""
 
     def get_tables(self):
         prefixes = dict()
         with open(self._filename) as f:
             for prefix, event, _ in ijson.parse(f):
                 if event in ("start_map", "start_array"):
                     prefixes[".".join([self._root_prefix, prefix])] = None
         return [self._root_prefix] + list(prefixes.keys())[1:]
 
     def file_iterator(self, table, options, max_rows=-1):
         if max_rows == -1:
             max_rows = sys.maxsize
-        max_depth = options["max_depth"]
+        max_depth = options.get("max_depth", self.OPTIONS["max_depth"]["default"])
         prefix = ".".join(table.split(".")[1:])
-        with open(self._filename) as f:
+        with open(self._filename, "rb") as f:
             row = 0
             for obj in ijson.items(f, prefix):
                 for x in _tabulize_json(obj):
                     if row > max_rows:
                         return
                     yield x[:max_depth]
                     row += 1
 
     def get_data_iterator(self, table, options, max_rows=-1):
         """
-        Return data read from data source table in table. If max_rows is
+        Returns data read from data source table in table. If max_rows is
         specified only that number of rows.
         """
         return self.file_iterator(table, options, max_rows=max_rows), []
 
 
 def _tabulize_json(obj):
     if isinstance(obj, dict):
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_io/importers/reader.py` & `spinedb_api-0.29.0/spinedb_api/spine_io/importers/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains a class template for a data source connector used in import ui.
 
-:author: P. Vennström (VTT)
-:date:   1.6.2019
 """
 
 from itertools import islice
 from spinedb_api.import_mapping.generator import get_mapped_data, identity
 from spinedb_api.import_mapping.import_mapping_compat import parse_named_mapping_spec
 from spinedb_api import DateTime, Duration, ParameterValueFormatError
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spinedb_api-0.28.0/spinedb_api/spine_io/importers/sqlalchemy_connector.py` & `spinedb_api-0.29.0/spinedb_api/spine_io/importers/sqlalchemy_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains SqlAlchemyConnector class.
 
-:author: P. Vennström (VTT)
-:date:   1.6.2019
 """
 
 
 from sqlalchemy import create_engine, MetaData
 from sqlalchemy.orm import Session
 from .reader import SourceConnection
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spinedb_api-0.28.0/spinedb_api.egg-info/PKG-INFO` & `spinedb_api-0.29.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,88 @@
 Metadata-Version: 2.1
-Name: spinedb-api
-Version: 0.28.0
+Name: spinedb_api
+Version: 0.29.0
 Summary: An API to talk to Spine databases.
 Home-page: https://github.com/spine-tools/Spine-Database-API
 Author: Spine Project consortium
 Author-email: spine_info@vtt.fi
 License: LGPL-3.0-or-later
-Description: # Spine Database API
-        
-        [![Documentation Status](https://readthedocs.org/projects/spine-database-api/badge/?version=latest)](https://spine-database-api.readthedocs.io/en/latest/?badge=latest)
-        [![Unit tests](https://github.com/spine-tools/Spine-Database-API/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/Spine-Database-API/actions?query=workflow%3A"Unit+tests")
-        [![codecov](https://codecov.io/gh/spine-tools/Spine-Database-API/branch/master/graph/badge.svg)](https://codecov.io/gh/spine-tools/Spine-Database-API)
-        [![PyPI version](https://badge.fury.io/py/spinedb-api.svg)](https://badge.fury.io/py/spinedb-api)
-        
-        A Python package to access and manipulate Spine databases in a customary, unified way.
-        
-        ## License
-        
-        Spine Database API is released under the GNU Lesser General Public License (LGPL) license. All accompanying
-        documentation and manual are released under the Creative Commons BY-SA 4.0 license.
-        
-        ## Getting started
-        
-        ### Installation
-        
-        To install the package run:
-        
-            $ pip install spinedb_api
-        
-        To upgrade to the most recent version, run:
-        
-            $ pip install --upgrade spinedb_api
-        
-        You can also specify a branch, or a tag, for instance:
-        
-            $ pip install spinedb_api==0.12.1
-        
-        To install the latest development version use the Git repository url:
-        
-            $ pip install --upgrade git+https://github.com/spine-tools/Spine-Database-API.git
-        
-        
-        ## Building the documentation
-        
-        Source files for the documentation can be found in `docs/source` directory. In order to 
-        build the HTML docs, you need to install the additional documentation building requirements
-        by running:
-        
-            $ pip install -r dev-requirements.txt 
-        
-        This installs Sphinx (among other things), which is required in building the documentation.
-        When Sphinx is installed, you can build the HTML pages from the source files by running:
-        
-            > docs\make.bat html
-            
-        or
-        
-            $ pushd docs
-            $ make html
-            $ popd
-            
-        depending on your operating system.        
-         
-        After running the build, the index page can be found in `docs/build/html/index.html`.
-        
-        &nbsp;
-        <hr>
-        <center>
-        <table width=500px frame="none">
-        <tr>
-        <td valign="middle" width=100px>
-        <img src=fig/eu-emblem-low-res.jpg alt="EU emblem" width=100%></td>
-        <td valign="middle">This project has received funding from European Climate, Infrastructure and Environment Executive Agency under the European Union’s HORIZON Research and Innovation Actions under grant agreement N°101095998.</td>
-        <tr>
-        <td valign="middle" width=100px>
-        <img src=fig/eu-emblem-low-res.jpg alt="EU emblem" width=100%></td>
-        <td valign="middle">This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 774629.</td>
-        </table>
-        </center>
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.12,>=3.8.1
 Description-Content-Type: text/markdown
+License-File: COPYING
+License-File: COPYING.LESSER
+
+# Spine Database API
+
+[![Documentation Status](https://readthedocs.org/projects/spine-database-api/badge/?version=latest)](https://spine-database-api.readthedocs.io/en/latest/?badge=latest)
+[![Unit tests](https://github.com/spine-tools/Spine-Database-API/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/Spine-Database-API/actions?query=workflow%3A"Unit+tests")
+[![codecov](https://codecov.io/gh/spine-tools/Spine-Database-API/branch/master/graph/badge.svg)](https://codecov.io/gh/spine-tools/Spine-Database-API)
+[![PyPI version](https://badge.fury.io/py/spinedb-api.svg)](https://badge.fury.io/py/spinedb-api)
+
+A Python package to access and manipulate Spine databases in a customary, unified way.
+
+## License
+
+Spine Database API is released under the GNU Lesser General Public License (LGPL) license. All accompanying
+documentation and manual are released under the Creative Commons BY-SA 4.0 license.
+
+## Getting started
+
+### Installation
+
+To install the package run:
+
+    $ pip install spinedb_api
+
+To upgrade to the most recent version, run:
+
+    $ pip install --upgrade spinedb_api
+
+You can also specify a branch, or a tag, for instance:
+
+    $ pip install spinedb_api==0.12.1
+
+To install the latest development version use the Git repository url:
+
+    $ pip install --upgrade git+https://github.com/spine-tools/Spine-Database-API.git
+
+
+## Building the documentation
+
+Source files for the documentation can be found in `docs/source` directory. In order to 
+build the HTML docs, you need to install the additional documentation building requirements
+by running:
+
+    $ pip install -r dev-requirements.txt 
+
+This installs Sphinx (among other things), which is required in building the documentation.
+When Sphinx is installed, you can build the HTML pages from the source files by running:
+
+    > docs\make.bat html
+    
+or
+
+    $ pushd docs
+    $ make html
+    $ popd
+    
+depending on your operating system.        
+ 
+After running the build, the index page can be found in `docs/build/html/index.html`.
+
+&nbsp;
+<hr>
+<center>
+<table width=500px frame="none">
+<tr>
+<td valign="middle" width=100px>
+<img src=fig/eu-emblem-low-res.jpg alt="EU emblem" width=100%></td>
+<td valign="middle">This project has received funding from European Climate, Infrastructure and Environment Executive Agency under the European Union’s HORIZON Research and Innovation Actions under grant agreement N°101095998.</td>
+<tr>
+<td valign="middle" width=100px>
+<img src=fig/eu-emblem-low-res.jpg alt="EU emblem" width=100%></td>
+<td valign="middle">This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 774629.</td>
+</table>
+</center>
```

#### html2text {}

```diff
@@ -1,15 +1,19 @@
-Metadata-Version: 2.1 Name: spinedb-api Version: 0.28.0 Summary: An API to talk
+Metadata-Version: 2.1 Name: spinedb_api Version: 0.29.0 Summary: An API to talk
 to Spine databases. Home-page: https://github.com/spine-tools/Spine-Database-
 API Author: Spine Project consortium Author-email: spine_info@vtt.fi License:
-LGPL-3.0-or-later Description: # Spine Database API [![Documentation Status]
-(https://readthedocs.org/projects/spine-database-api/badge/?version=latest)]
-(https://spine-database-api.readthedocs.io/en/latest/?badge=latest) [![Unit
-tests](https://github.com/spine-tools/Spine-Database-API/workflows/
-Unit%20tests/badge.svg)](https://github.com/spine-tools/Spine-Database-API/
+LGPL-3.0-or-later Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Operating System :: OS Independent Requires-Python: <3.12,>=3.8.1
+Description-Content-Type: text/markdown License-File: COPYING License-File:
+COPYING.LESSER # Spine Database API [![Documentation Status](https://
+readthedocs.org/projects/spine-database-api/badge/?version=latest)](https://
+spine-database-api.readthedocs.io/en/latest/?badge=latest) [![Unit tests]
+(https://github.com/spine-tools/Spine-Database-API/workflows/Unit%20tests/
+badge.svg)](https://github.com/spine-tools/Spine-Database-API/
 actions?query=workflow%3A"Unit+tests") [![codecov](https://codecov.io/gh/spine-
 tools/Spine-Database-API/branch/master/graph/badge.svg)](https://codecov.io/gh/
 spine-tools/Spine-Database-API) [![PyPI version](https://badge.fury.io/py/
 spinedb-api.svg)](https://badge.fury.io/py/spinedb-api) A Python package to
 access and manipulate Spine databases in a customary, unified way. ## License
 Spine Database API is released under the GNU Lesser General Public License
 (LGPL) license. All accompanying documentation and manual are released under
@@ -29,11 +33,7 @@
 the build, the index page can be found in `docs/build/html/index.html`.  
 ===============================================================================
 [EU     This project has received funding from European Climate, Infrastructure and
 emblem] Environment Executive Agency under the European Unionâs HORIZON Research and
         Innovation Actions under grant agreement NÂ°101095998.
 [EU     This project has received funding from the European Unionâs Horizon 2020
 emblem] research and innovation programme under grant agreement No 774629.
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent Requires-Python: <3.12,>=3.8.1
-Description-Content-Type: text/markdown
```

### Comparing `spinedb_api-0.28.0/spinedb_api.egg-info/SOURCES.txt` & `spinedb_api-0.29.0/spinedb_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -87,13 +87,14 @@
 spinedb_api/spine_io/importers/excel_reader.py
 spinedb_api/spine_io/importers/gdx_connector.py
 spinedb_api/spine_io/importers/json_reader.py
 spinedb_api/spine_io/importers/reader.py
 spinedb_api/spine_io/importers/sqlalchemy_connector.py
 tests/test_DatabaseMapping.py
 tests/test_DiffDatabaseMapping.py
+tests/test_check_functions.py
 tests/test_export_functions.py
 tests/test_helpers.py
 tests/test_import_functions.py
 tests/test_mapping.py
 tests/test_migration.py
 tests/test_parameter_value.py
```

### Comparing `spinedb_api-0.28.0/tests/test_DatabaseMapping.py` & `spinedb_api-0.29.0/tests/test_DatabaseMapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Unit tests for DatabaseMapping class.
 
-:author: A. Soininen
-:date:   2.7.2020
 """
 import unittest
 from unittest.mock import patch
 from sqlalchemy.engine.url import URL
 from spinedb_api import (
     DatabaseMapping,
     to_database,
```

### Comparing `spinedb_api-0.28.0/tests/test_DiffDatabaseMapping.py` & `spinedb_api-0.29.0/tests/test_DiffDatabaseMapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Unit tests for DiffDatabaseMapping class.
 
-:author: P. Vennström (VTT)
-:date:   29.11.2018
 """
 
 import os.path
 from tempfile import TemporaryDirectory
 import unittest
 from unittest import mock
 from sqlalchemy.engine.url import make_url, URL
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spinedb_api-0.28.0/tests/test_export_functions.py` & `spinedb_api-0.29.0/tests/test_export_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Unit tests for export_functions.
 
-:authors: A. Soininen (VTT)
-:date:    29.6.2020
 """
 
 import unittest
 from spinedb_api import (
     DiffDatabaseMapping,
     export_alternatives,
     export_data,
```

### Comparing `spinedb_api-0.28.0/tests/test_helpers.py` & `spinedb_api-0.29.0/tests/test_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Unit tests for helpers.py.
 
-:author: P. Vennström (VTT)
-:date:   17.12.2018
 """
 
 
 import unittest
 from spinedb_api.helpers import compare_schemas, create_new_spine_database
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spinedb_api-0.28.0/tests/test_import_functions.py` & `spinedb_api-0.29.0/tests/test_import_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Unit tests for import_functions.py.
 
-:author: P. Vennström (VTT)
-:date:   17.12.2018
 """
 
 import unittest
 
 from spinedb_api.spine_db_server import _unparse_value
 from spinedb_api.diff_db_mapping import DiffDatabaseMapping
 from spinedb_api.db_mapping import DatabaseMapping
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spinedb_api-0.28.0/tests/test_mapping.py` & `spinedb_api-0.29.0/tests/test_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Unit tests for :mod:`spinedb_api.mapping`.
 
-:author: A. Soininen (VTT)
-:date:   12.5.2021
 """
 import unittest
 from spinedb_api.mapping import Mapping, Position, value_index, unflatten
 
 
 class TestMapping(unittest.TestCase):
     def test_value_index(self):
```

### Comparing `spinedb_api-0.28.0/tests/test_migration.py` & `spinedb_api-0.29.0/tests/test_migration.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Unit tests for migration scripts.
 
-:author: M. Marin (KTH)
-:date:   19.9.2019
 """
 import os.path
 from tempfile import TemporaryDirectory
 import unittest
 from sqlalchemy import inspect
 from sqlalchemy.engine.url import URL
 from spinedb_api.helpers import create_new_spine_database, _create_first_spine_database, is_head_engine, schema_dict
```

### Comparing `spinedb_api-0.28.0/tests/test_parameter_value.py` & `spinedb_api-0.29.0/tests/test_parameter_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Tests for the parameter_value module.
 
-:authors: A. Soininen (VTT)
-:date:   7.6.2019
 """
 
 from datetime import datetime
 import json
 import unittest
 import dateutil.parser
 from dateutil.relativedelta import relativedelta
```

