# Comparing `tmp/spinetoolbox-0.6.8.tar.gz` & `tmp/spinetoolbox-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spinetoolbox-0.6.8.tar", last modified: Fri Jun  3 12:30:32 2022, max compression
+gzip compressed data, was "spinetoolbox-0.6.9.tar", last modified: Tue Jun  7 07:53:58 2022, max compression
```

## Comparing `spinetoolbox-0.6.8.tar` & `spinetoolbox-0.6.9.tar`

### file list

```diff
@@ -1,289 +1,289 @@
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:32.117941 spinetoolbox-0.6.8/
--rw-rw-rw-   0        0        0    35823 2019-06-13 10:03:34.000000 spinetoolbox-0.6.8/COPYING
--rw-rw-rw-   0        0        0     7815 2019-06-13 10:03:34.000000 spinetoolbox-0.6.8/COPYING.LESSER
--rw-rw-rw-   0        0        0       24 2021-06-29 09:23:47.000000 spinetoolbox-0.6.8/MANIFEST.in
--rw-rw-rw-   0        0        0    12592 2022-06-03 12:30:32.117941 spinetoolbox-0.6.8/PKG-INFO
--rw-rw-rw-   0        0        0    11965 2022-05-10 05:21:59.000000 spinetoolbox-0.6.8/README.md
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:28.933526 spinetoolbox-0.6.8/execution_tests/
--rw-rw-rw-   0        0        0        0 2021-03-04 13:14:27.000000 spinetoolbox-0.6.8/execution_tests/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:28.966818 spinetoolbox-0.6.8/execution_tests/scenario_filters/
--rw-rw-rw-   0        0        0        0 2022-03-01 07:13:30.000000 spinetoolbox-0.6.8/execution_tests/scenario_filters/__init__.py
--rw-rw-rw-   0        0        0     3159 2022-03-25 08:35:13.000000 spinetoolbox-0.6.8/execution_tests/scenario_filters/execution_test.py
--rw-rw-rw-   0        0        0      317 2021-03-04 13:14:27.000000 spinetoolbox-0.6.8/execution_tests/scenario_filters/tool.py
--rw-rw-rw-   0        0        0      131 2019-09-03 05:24:26.000000 spinetoolbox-0.6.8/pyproject.toml
--rw-rw-rw-   0        0        0     1459 2022-06-03 12:30:32.134664 spinetoolbox-0.6.8/setup.cfg
--rw-rw-rw-   0        0        0     1173 2021-06-29 09:23:47.000000 spinetoolbox-0.6.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:29.394221 spinetoolbox-0.6.8/spinetoolbox/
--rw-rw-rw-   0        0        0     1068 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/__init__.py
--rw-rw-rw-   0        0        0     1179 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/__main__.py
--rw-rw-rw-   0        0        0     6684 2022-03-14 06:44:04.000000 spinetoolbox-0.6.8/spinetoolbox/config.py
--rw-rw-rw-   0        0        0    11717 2021-11-01 09:17:28.000000 spinetoolbox-0.6.8/spinetoolbox/execution_managers.py
--rw-rw-rw-   0        0        0    20811 2022-06-03 11:35:20.000000 spinetoolbox-0.6.8/spinetoolbox/headless.py
--rw-rw-rw-   0        0        0    54363 2022-06-03 11:35:10.000000 spinetoolbox-0.6.8/spinetoolbox/helpers.py
--rw-rw-rw-   0        0        0    24325 2022-06-03 11:35:10.000000 spinetoolbox-0.6.8/spinetoolbox/link.py
--rw-rw-rw-   0        0        0     3487 2021-08-11 09:23:18.000000 spinetoolbox-0.6.8/spinetoolbox/load_project_items.py
--rw-rw-rw-   0        0        0     2208 2022-02-10 09:52:07.000000 spinetoolbox-0.6.8/spinetoolbox/log_mixin.py
--rw-rw-rw-   0        0        0     2279 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/logger_interface.py
--rw-rw-rw-   0        0        0     4590 2022-06-03 11:35:20.000000 spinetoolbox-0.6.8/spinetoolbox/main.py
--rw-rw-rw-   0        0        0     2103 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/metaobject.py
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:29.668198 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/
--rw-rw-rw-   0        0        0     1305 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/__init__.py
--rw-rw-rw-   0        0        0    10183 2021-06-09 09:03:40.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/array_model.py
--rw-rw-rw-   0        0        0    14938 2022-05-02 05:39:31.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/compound_table_model.py
--rw-rw-rw-   0        0        0     4681 2022-03-30 11:15:00.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/empty_row_model.py
--rw-rw-rw-   0        0        0    13414 2021-12-30 13:53:42.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/file_list_models.py
--rw-rw-rw-   0        0        0    14288 2021-11-01 09:17:28.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/filter_checkbox_list_model.py
--rw-rw-rw-   0        0        0     2040 2022-03-14 06:44:04.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/filter_execution_model.py
--rw-rw-rw-   0        0        0     3691 2021-06-09 09:03:40.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/indexed_value_table_model.py
--rw-rw-rw-   0        0        0    19094 2021-12-02 08:08:09.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/map_model.py
--rw-rw-rw-   0        0        0    10408 2022-05-02 05:39:31.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/minimal_table_model.py
--rw-rw-rw-   0        0        0    12631 2022-03-14 06:44:04.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/minimal_tree_model.py
--rw-rw-rw-   0        0        0    13126 2022-01-31 08:50:32.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/project_item_model.py
--rw-rw-rw-   0        0        0     7890 2022-01-31 08:50:32.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/project_item_specification_models.py
--rw-rw-rw-   0        0        0     7147 2022-01-25 09:58:33.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/project_tree_item.py
--rw-rw-rw-   0        0        0     8318 2022-02-24 06:05:42.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/resource_filter_model.py
--rw-rw-rw-   0        0        0     1152 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/shared.py
--rw-rw-rw-   0        0        0     5820 2021-10-18 10:21:24.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/time_pattern_model.py
--rw-rw-rw-   0        0        0     6972 2021-06-09 09:03:40.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/time_series_model_fixed_resolution.py
--rw-rw-rw-   0        0        0     8489 2021-07-05 05:59:49.000000 spinetoolbox-0.6.8/spinetoolbox/mvcmodels/time_series_model_variable_resolution.py
--rw-rw-rw-   0        0        0    25667 2022-04-20 07:20:21.000000 spinetoolbox-0.6.8/spinetoolbox/plotting.py
--rw-rw-rw-   0        0        0    10804 2021-09-24 12:50:45.000000 spinetoolbox-0.6.8/spinetoolbox/plugin_manager.py
--rw-rw-rw-   0        0        0    57400 2022-06-03 11:35:20.000000 spinetoolbox-0.6.8/spinetoolbox/project.py
--rw-rw-rw-   0        0        0    23892 2022-04-20 07:20:21.000000 spinetoolbox-0.6.8/spinetoolbox/project_commands.py
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:29.751342 spinetoolbox-0.6.8/spinetoolbox/project_item/
--rw-rw-rw-   0        0        0     1098 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/project_item/__init__.py
--rw-rw-rw-   0        0        0     2621 2022-04-20 07:20:21.000000 spinetoolbox-0.6.8/spinetoolbox/project_item/logging_connection.py
--rw-rw-rw-   0        0        0    18393 2022-03-25 08:35:13.000000 spinetoolbox-0.6.8/spinetoolbox/project_item/project_item.py
--rw-rw-rw-   0        0        0     5165 2021-06-07 08:43:02.000000 spinetoolbox-0.6.8/spinetoolbox/project_item/project_item_factory.py
--rw-rw-rw-   0        0        0    15018 2022-03-14 06:44:04.000000 spinetoolbox-0.6.8/spinetoolbox/project_item/specification_editor_window.py
--rw-rw-rw-   0        0        0    27848 2022-04-29 06:30:43.000000 spinetoolbox-0.6.8/spinetoolbox/project_item_icon.py
--rw-rw-rw-   0        0        0    29100 2021-12-29 13:41:06.000000 spinetoolbox-0.6.8/spinetoolbox/project_upgrader.py
--rw-rw-rw-   0        0        0   944939 2022-05-02 05:39:31.000000 spinetoolbox-0.6.8/spinetoolbox/resources_icons_rc.py
--rw-rw-rw-   0        0        0   443550 2022-04-29 06:30:43.000000 spinetoolbox-0.6.8/spinetoolbox/resources_logos_rc.py
--rw-rw-rw-   0        0        0    16471 2022-05-02 05:39:31.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_commands.py
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:29.801203 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/
--rw-rw-rw-   0        0        0     1101 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/__init__.py
--rw-rw-rw-   0        0        0    31726 2022-03-25 08:35:13.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/graphics_items.py
--rw-rw-rw-   0        0        0     1824 2021-11-09 06:04:47.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/main.py
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:30.101575 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/
--rw-rw-rw-   0        0        0     1300 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/__init__.py
--rw-rw-rw-   0        0        0     7830 2022-03-14 06:44:04.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/alternative_scenario_item.py
--rw-rw-rw-   0        0        0     6679 2021-10-18 10:21:24.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/alternative_scenario_model.py
--rw-rw-rw-   0        0        0     1147 2022-05-02 05:39:31.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/colors.py
--rw-rw-rw-   0        0        0    26481 2022-01-31 08:50:32.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/compound_parameter_models.py
--rw-rw-rw-   0        0        0    12466 2021-10-18 10:21:24.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/empty_parameter_models.py
--rw-rw-rw-   0        0        0    12114 2021-12-02 08:08:09.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/entity_tree_item.py
--rw-rw-rw-   0        0        0    13113 2021-11-15 07:59:53.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/entity_tree_models.py
--rw-rw-rw-   0        0        0     4311 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/frozen_table_model.py
--rw-rw-rw-   0        0        0     9976 2022-05-02 05:39:31.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/item_metadata_table_model.py
--rw-rw-rw-   0        0        0     6864 2022-05-02 05:39:31.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/metadata_table_model.py
--rw-rw-rw-   0        0        0    18387 2022-05-02 05:39:31.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/metadata_table_model_base.py
--rw-rw-rw-   0        0        0    17243 2022-05-02 05:39:31.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/multi_db_tree_item.py
--rw-rw-rw-   0        0        0     3255 2021-11-15 07:59:53.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/multi_db_tree_model.py
--rw-rw-rw-   0        0        0    23553 2021-09-15 11:40:52.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/parameter_mixins.py
--rw-rw-rw-   0        0        0     4471 2022-03-25 08:35:13.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/parameter_value_list_item.py
--rw-rw-rw-   0        0        0     4097 2022-03-25 08:35:13.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/parameter_value_list_model.py
--rw-rw-rw-   0        0        0    10476 2021-09-20 06:33:12.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/pivot_model.py
--rw-rw-rw-   0        0        0    58155 2022-01-31 08:50:32.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/pivot_table_models.py
--rw-rw-rw-   0        0        0    19461 2022-05-02 05:39:31.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/single_parameter_models.py
--rw-rw-rw-   0        0        0    12258 2022-03-14 06:44:04.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/tool_feature_item.py
--rw-rw-rw-   0        0        0    11403 2022-03-14 06:44:04.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/tool_feature_model.py
--rw-rw-rw-   0        0        0     8915 2022-03-14 06:44:04.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/tree_item_utility.py
--rw-rw-rw-   0        0        0     5808 2022-03-14 06:44:04.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/tree_model_base.py
--rw-rw-rw-   0        0        0     2209 2021-09-20 11:07:08.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/scenario_generation.py
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:30.151543 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/ui/
--rw-rw-rw-   0        0        0     1097 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/ui/__init__.py
--rw-rw-rw-   0        0        0     5909 2021-09-20 11:07:08.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/ui/scenario_generator.py
--rw-rw-rw-   0        0        0    42820 2022-05-02 05:39:31.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/ui/spine_db_editor_window.py
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:30.484629 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/
--rw-rw-rw-   0        0        0     1078 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/__init__.py
--rw-rw-rw-   0        0        0    47996 2021-10-04 12:46:07.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/add_items_dialogs.py
--rw-rw-rw-   0        0        0     8285 2021-12-29 06:38:28.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/commit_viewer.py
--rw-rw-rw-   0        0        0    36021 2022-05-02 05:39:31.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/custom_delegates.py
--rw-rw-rw-   0        0        0     9284 2021-06-02 06:15:48.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/custom_menus.py
--rw-rw-rw-   0        0        0    37937 2022-04-29 06:30:43.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/custom_qgraphicsviews.py
--rw-rw-rw-   0        0        0    41832 2022-06-03 11:35:10.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/custom_qtableview.py
--rw-rw-rw-   0        0        0    30453 2022-06-03 11:35:10.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/custom_qtreeview.py
--rw-rw-rw-   0        0        0     6185 2022-03-14 06:44:04.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/custom_qwidgets.py
--rw-rw-rw-   0        0        0    18946 2021-10-04 12:46:07.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/edit_or_remove_items_dialogs.py
--rw-rw-rw-   0        0        0     6533 2022-05-27 09:02:28.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/graph_layout_generator.py
--rw-rw-rw-   0        0        0    27337 2022-06-03 11:35:10.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/graph_view_mixin.py
--rw-rw-rw-   0        0        0     7429 2022-05-02 05:39:31.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/item_metadata_editor.py
--rw-rw-rw-   0        0        0     8679 2021-10-06 09:32:23.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/manage_items_dialogs.py
--rw-rw-rw-   0        0        0     7260 2022-03-29 12:53:01.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/mass_select_items_dialogs.py
--rw-rw-rw-   0        0        0     4057 2022-05-02 05:39:31.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/metadata_editor.py
--rw-rw-rw-   0        0        0     8554 2022-03-14 06:44:04.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/multi_spine_db_editor.py
--rw-rw-rw-   0        0        0     4400 2022-03-25 08:35:13.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/object_name_list_editor.py
--rw-rw-rw-   0        0        0    14428 2022-06-03 11:35:10.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/parameter_view_mixin.py
--rw-rw-rw-   0        0        0     6846 2021-09-20 11:07:08.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/pivot_table_header_view.py
--rw-rw-rw-   0        0        0     8104 2021-09-20 11:07:08.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/scenario_generator.py
--rw-rw-rw-   0        0        0     4425 2022-03-25 08:35:13.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/select_position_parameters_dialog.py
--rw-rw-rw-   0        0        0    58072 2022-06-03 11:35:10.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/spine_db_editor.py
--rw-rw-rw-   0        0        0     5258 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/tabular_view_header_widget.py
--rw-rw-rw-   0        0        0    42782 2022-06-03 11:35:10.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/tabular_view_mixin.py
--rw-rw-rw-   0        0        0    17330 2022-06-03 11:35:10.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/tree_view_mixin.py
--rw-rw-rw-   0        0        0    13880 2022-03-14 06:44:04.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/url_toolbar.py
--rw-rw-rw-   0        0        0     8127 2022-06-03 11:35:10.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_icon_manager.py
--rw-rw-rw-   0        0        0    94362 2022-06-03 11:35:10.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_manager.py
--rw-rw-rw-   0        0        0    15000 2022-05-10 13:02:08.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_parcel.py
--rw-rw-rw-   0        0        0    18671 2022-05-02 05:39:31.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_signaller.py
--rw-rw-rw-   0        0        0    19717 2022-05-10 05:21:59.000000 spinetoolbox-0.6.8/spinetoolbox/spine_db_worker.py
--rw-rw-rw-   0        0        0    10720 2022-05-10 05:21:59.000000 spinetoolbox-0.6.8/spinetoolbox/spine_engine_manager.py
--rw-rw-rw-   0        0        0    16058 2022-05-03 08:41:44.000000 spinetoolbox-0.6.8/spinetoolbox/spine_engine_worker.py
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:30.751530 spinetoolbox-0.6.8/spinetoolbox/ui/
--rw-rw-rw-   0        0        0     1090 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/ui/__init__.py
--rw-rw-rw-   0        0        0    24546 2021-04-09 12:18:00.000000 spinetoolbox-0.6.8/spinetoolbox/ui/about.py
--rw-rw-rw-   0        0        0     8383 2021-05-10 13:23:24.000000 spinetoolbox-0.6.8/spinetoolbox/ui/add_project_item.py
--rw-rw-rw-   0        0        0     6682 2021-06-09 09:03:40.000000 spinetoolbox-0.6.8/spinetoolbox/ui/array_editor.py
--rw-rw-rw-   0        0        0     3650 2021-05-10 13:23:24.000000 spinetoolbox-0.6.8/spinetoolbox/ui/datetime_editor.py
--rw-rw-rw-   0        0        0     3467 2021-05-10 13:23:24.000000 spinetoolbox-0.6.8/spinetoolbox/ui/duration_editor.py
--rw-rw-rw-   0        0        0     2626 2021-05-10 13:23:24.000000 spinetoolbox-0.6.8/spinetoolbox/ui/import_source_selector.py
--rw-rw-rw-   0        0        0     5070 2022-02-07 09:52:28.000000 spinetoolbox-0.6.8/spinetoolbox/ui/jump_properties.py
--rw-rw-rw-   0        0        0    21001 2021-03-31 12:11:44.000000 spinetoolbox-0.6.8/spinetoolbox/ui/kernel_editor_dialog.py
--rw-rw-rw-   0        0        0     3327 2022-02-25 07:20:57.000000 spinetoolbox-0.6.8/spinetoolbox/ui/link_properties.py
--rw-rw-rw-   0        0        0    41474 2022-02-25 10:16:01.000000 spinetoolbox-0.6.8/spinetoolbox/ui/mainwindow.py
--rw-rw-rw-   0        0        0     3488 2021-09-20 11:07:08.000000 spinetoolbox-0.6.8/spinetoolbox/ui/map_editor.py
--rw-rw-rw-   0        0        0     9012 2021-04-28 05:10:32.000000 spinetoolbox-0.6.8/spinetoolbox/ui/mini_kernel_editor_dialog.py
--rw-rw-rw-   0        0        0     6974 2021-05-10 13:23:24.000000 spinetoolbox-0.6.8/spinetoolbox/ui/open_project_dialog.py
--rw-rw-rw-   0        0        0     4818 2021-07-09 05:39:38.000000 spinetoolbox-0.6.8/spinetoolbox/ui/parameter_value_editor.py
--rw-rw-rw-   0        0        0     4589 2021-05-10 13:23:24.000000 spinetoolbox-0.6.8/spinetoolbox/ui/plain_parameter_value_editor.py
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:30.781267 spinetoolbox-0.6.8/spinetoolbox/ui/resources/
--rw-rw-rw-   0        0        0        0 2022-05-05 12:16:25.000000 spinetoolbox-0.6.8/spinetoolbox/ui/resources/__init__.py
--rw-rw-rw-   0        0        0    12254 2019-06-13 10:03:34.000000 spinetoolbox-0.6.8/spinetoolbox/ui/resources/app.ico
--rw-rw-rw-   0        0        0    25955 2022-05-04 09:15:52.000000 spinetoolbox-0.6.8/spinetoolbox/ui/resources/cat.py
--rw-rw-rw-   0        0        0    65674 2022-01-25 09:58:33.000000 spinetoolbox-0.6.8/spinetoolbox/ui/settings.py
--rw-rw-rw-   0        0        0    14516 2021-05-10 13:23:24.000000 spinetoolbox-0.6.8/spinetoolbox/ui/spine_datapackage_form.py
--rw-rw-rw-   0        0        0     3299 2021-09-20 06:33:12.000000 spinetoolbox-0.6.8/spinetoolbox/ui/time_pattern_editor.py
--rw-rw-rw-   0        0        0     7745 2021-06-09 09:03:40.000000 spinetoolbox-0.6.8/spinetoolbox/ui/time_series_fixed_resolution_editor.py
--rw-rw-rw-   0        0        0     4864 2021-06-09 09:03:40.000000 spinetoolbox-0.6.8/spinetoolbox/ui/time_series_variable_resolution_editor.py
--rw-rw-rw-   0        0        0     5330 2021-05-10 13:23:24.000000 spinetoolbox-0.6.8/spinetoolbox/ui/tool_configuration_assistant.py
--rw-rw-rw-   0        0        0   106766 2022-05-04 09:15:52.000000 spinetoolbox-0.6.8/spinetoolbox/ui_main.py
--rw-rw-rw-   0        0        0     2179 2022-06-03 12:30:00.000000 spinetoolbox-0.6.8/spinetoolbox/version.py
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:31.417933 spinetoolbox-0.6.8/spinetoolbox/widgets/
--rw-rw-rw-   0        0        0     1095 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/__init__.py
--rw-rw-rw-   0        0        0     6485 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/about_widget.py
--rw-rw-rw-   0        0        0     6073 2021-05-20 12:10:49.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/add_project_item_widget.py
--rw-rw-rw-   0        0        0    22171 2021-03-04 13:02:41.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/add_up_spine_opt_wizard.py
--rw-rw-rw-   0        0        0     6061 2021-06-09 09:03:40.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/array_editor.py
--rw-rw-rw-   0        0        0     2440 2021-05-31 05:32:28.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/array_value_editor.py
--rw-rw-rw-   0        0        0     6087 2021-12-13 12:55:05.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/code_text_edit.py
--rw-rw-rw-   0        0        0     3254 2021-09-15 11:40:52.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/commit_dialog.py
--rw-rw-rw-   0        0        0     2701 2021-11-15 08:00:02.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/console_window.py
--rw-rw-rw-   0        0        0     4266 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/custom_combobox.py
--rw-rw-rw-   0        0        0     6422 2021-07-05 05:59:49.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/custom_delegates.py
--rw-rw-rw-   0        0        0    18913 2022-03-25 08:35:13.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/custom_editors.py
--rw-rw-rw-   0        0        0     8230 2021-11-01 09:17:28.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/custom_menus.py
--rw-rw-rw-   0        0        0     1580 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/custom_qcombobox.py
--rw-rw-rw-   0        0        0    13578 2022-05-04 09:15:52.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/custom_qgraphicsscene.py
--rw-rw-rw-   0        0        0    19926 2022-04-20 07:20:21.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/custom_qgraphicsviews.py
--rw-rw-rw-   0        0        0     4525 2022-01-31 08:50:32.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/custom_qlineedits.py
--rw-rw-rw-   0        0        0    34304 2022-05-02 05:39:31.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/custom_qtableview.py
--rw-rw-rw-   0        0        0    10534 2022-03-14 06:44:04.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/custom_qtextbrowser.py
--rw-rw-rw-   0        0        0     3863 2021-03-17 11:51:57.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/custom_qtreeview.py
--rw-rw-rw-   0        0        0    23885 2022-06-03 11:35:10.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/custom_qwidgets.py
--rw-rw-rw-   0        0        0     3116 2021-03-01 11:44:55.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/datetime_editor.py
--rw-rw-rw-   0        0        0     2502 2021-03-01 11:44:55.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/duration_editor.py
--rw-rw-rw-   0        0        0    13246 2021-12-02 08:08:09.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/indexed_value_table_context_menu.py
--rw-rw-rw-   0        0        0    11034 2021-07-05 05:59:49.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/install_julia_wizard.py
--rw-rw-rw-   0        0        0     6089 2022-04-20 07:20:21.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/jump_properties_widget.py
--rw-rw-rw-   0        0        0    13366 2022-05-03 08:41:44.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/jupyter_console_widget.py
--rw-rw-rw-   0        0        0    56612 2021-09-06 09:57:11.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/kernel_editor.py
--rw-rw-rw-   0        0        0     4134 2022-03-29 12:53:01.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/link_properties_widget.py
--rw-rw-rw-   0        0        0     3739 2021-06-09 09:03:40.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/map_editor.py
--rw-rw-rw-   0        0        0     2758 2021-07-09 05:39:38.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/map_value_editor.py
--rw-rw-rw-   0        0        0     3380 2021-09-06 09:57:11.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/multi_tab_spec_editor.py
--rw-rw-rw-   0        0        0    21682 2022-04-20 07:20:21.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/multi_tab_window.py
--rw-rw-rw-   0        0        0    10077 2022-03-14 06:44:04.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/notification.py
--rw-rw-rw-   0        0        0    19787 2021-09-06 09:57:11.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/open_project_widget.py
--rw-rw-rw-   0        0        0     3636 2021-06-09 09:03:40.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/parameter_value_editor.py
--rw-rw-rw-   0        0        0     9369 2022-04-25 05:51:19.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/parameter_value_editor_base.py
--rw-rw-rw-   0        0        0    30386 2022-06-03 11:35:10.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/persistent_console_widget.py
--rw-rw-rw-   0        0        0     2943 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/plain_parameter_value_editor.py
--rw-rw-rw-   0        0        0     2254 2022-04-20 07:20:21.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/plot_canvas.py
--rw-rw-rw-   0        0        0     7420 2022-06-03 11:35:10.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/plot_widget.py
--rw-rw-rw-   0        0        0     6329 2021-03-04 09:18:53.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/plugin_manager_widgets.py
--rw-rw-rw-   0        0        0    19180 2022-01-31 08:50:32.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/project_item_drag.py
--rw-rw-rw-   0        0        0     3903 2022-03-14 06:50:13.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/properties_widget.py
--rw-rw-rw-   0        0        0     3091 2021-09-30 07:33:33.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/rename_project_dialog.py
--rw-rw-rw-   0        0        0     1329 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/report_plotting_failure.py
--rw-rw-rw-   0        0        0    44898 2022-01-25 09:58:33.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/settings_widget.py
--rw-rw-rw-   0        0        0     2818 2022-02-10 09:52:07.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/statusbars.py
--rw-rw-rw-   0        0        0     3098 2021-09-20 06:33:12.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/time_pattern_editor.py
--rw-rw-rw-   0        0        0     7905 2021-06-09 09:03:40.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/time_series_fixed_resolution_editor.py
--rw-rw-rw-   0        0        0     4613 2021-06-09 09:03:40.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/time_series_variable_resolution_editor.py
--rw-rw-rw-   0        0        0    12814 2021-12-02 08:08:09.000000 spinetoolbox-0.6.8/spinetoolbox/widgets/toolbars.py
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:29.434612 spinetoolbox-0.6.8/spinetoolbox.egg-info/
--rw-rw-rw-   0        0        0    12592 2022-06-03 12:30:25.000000 spinetoolbox-0.6.8/spinetoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11731 2022-06-03 12:30:28.000000 spinetoolbox-0.6.8/spinetoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-03 12:30:25.000000 spinetoolbox-0.6.8/spinetoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2022-06-03 12:30:25.000000 spinetoolbox-0.6.8/spinetoolbox.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2019-10-04 13:19:54.000000 spinetoolbox-0.6.8/spinetoolbox.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      268 2022-06-03 12:30:25.000000 spinetoolbox-0.6.8/spinetoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-06-03 12:30:25.000000 spinetoolbox-0.6.8/spinetoolbox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:31.518160 spinetoolbox-0.6.8/tests/
--rw-rw-rw-   0        0        0     1095 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/tests/__init__.py
--rw-rw-rw-   0        0        0    12423 2022-03-14 06:44:04.000000 spinetoolbox-0.6.8/tests/mock_helpers.py
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:31.634633 spinetoolbox-0.6.8/tests/mvcmodels/
--rw-rw-rw-   0        0        0     1103 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/tests/mvcmodels/__init__.py
--rw-rw-rw-   0        0        0     5595 2021-06-09 09:03:40.000000 spinetoolbox-0.6.8/tests/mvcmodels/test_ArrayModel.py
--rw-rw-rw-   0        0        0    18146 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/tests/mvcmodels/test_FilterCheckboxList.py
--rw-rw-rw-   0        0        0     3610 2021-06-09 09:03:40.000000 spinetoolbox-0.6.8/tests/mvcmodels/test_IndexedValueTableModel.py
--rw-rw-rw-   0        0        0    24434 2021-07-09 05:39:38.000000 spinetoolbox-0.6.8/tests/mvcmodels/test_MapModel.py
--rw-rw-rw-   0        0        0    12319 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/tests/mvcmodels/test_MinimalTableModel.py
--rw-rw-rw-   0        0        0     4443 2022-01-31 08:50:32.000000 spinetoolbox-0.6.8/tests/mvcmodels/test_ProjectItemModel.py
--rw-rw-rw-   0        0        0     6212 2021-10-18 10:21:24.000000 spinetoolbox-0.6.8/tests/mvcmodels/test_TimePatternModel.py
--rw-rw-rw-   0        0        0    10768 2021-06-09 09:03:40.000000 spinetoolbox-0.6.8/tests/mvcmodels/test_TimeSeriesModelFixedResolution.py
--rw-rw-rw-   0        0        0     9887 2021-06-09 09:03:40.000000 spinetoolbox-0.6.8/tests/mvcmodels/test_TimeSeriesModelVariableResolution.py
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:31.651280 spinetoolbox-0.6.8/tests/project_item/
--rw-rw-rw-   0        0        0     1107 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/tests/project_item/__init__.py
--rw-rw-rw-   0        0        0     3050 2021-05-20 12:10:49.000000 spinetoolbox-0.6.8/tests/project_item/test_ProjectItem.py
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:31.684625 spinetoolbox-0.6.8/tests/spine_db_editor/
--rw-rw-rw-   0        0        0     1070 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/tests/spine_db_editor/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:31.751205 spinetoolbox-0.6.8/tests/spine_db_editor/mvcmodels/
--rw-rw-rw-   0        0        0      979 2021-01-22 12:30:03.000000 spinetoolbox-0.6.8/tests/spine_db_editor/mvcmodels/__init__.py
--rw-rw-rw-   0        0        0     7521 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/tests/spine_db_editor/mvcmodels/test_PivotModel.py
--rw-rw-rw-   0        0        0     8395 2022-06-03 11:35:10.000000 spinetoolbox-0.6.8/tests/spine_db_editor/mvcmodels/test_PivotTableModel.py
--rw-rw-rw-   0        0        0    11479 2021-11-01 09:17:28.000000 spinetoolbox-0.6.8/tests/spine_db_editor/mvcmodels/test_alternative_scenario_model.py
--rw-rw-rw-   0        0        0    12538 2021-11-01 09:17:28.000000 spinetoolbox-0.6.8/tests/spine_db_editor/mvcmodels/test_compound_parameter_models.py
--rw-rw-rw-   0        0        0    10795 2022-03-14 06:44:04.000000 spinetoolbox-0.6.8/tests/spine_db_editor/mvcmodels/test_emptyParameterModels.py
--rw-rw-rw-   0        0        0     6114 2021-12-02 08:08:09.000000 spinetoolbox-0.6.8/tests/spine_db_editor/test_graphics_items.py
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:31.868159 spinetoolbox-0.6.8/tests/spine_db_editor/widgets/
--rw-rw-rw-   0        0        0     1081 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/tests/spine_db_editor/widgets/__init__.py
--rw-rw-rw-   0        0        0    18758 2022-04-29 06:30:43.000000 spinetoolbox-0.6.8/tests/spine_db_editor/widgets/test_SpineDBEditor.py
--rw-rw-rw-   0        0        0    10030 2021-11-15 07:59:53.000000 spinetoolbox-0.6.8/tests/spine_db_editor/widgets/test_SpineDBEditorAdd.py
--rw-rw-rw-   0        0        0     3497 2021-08-09 10:52:23.000000 spinetoolbox-0.6.8/tests/spine_db_editor/widgets/test_SpineDBEditorBase.py
--rw-rw-rw-   0        0        0     7580 2021-09-06 09:57:11.000000 spinetoolbox-0.6.8/tests/spine_db_editor/widgets/test_SpineDBEditorFilter.py
--rw-rw-rw-   0        0        0     8439 2021-09-06 09:57:11.000000 spinetoolbox-0.6.8/tests/spine_db_editor/widgets/test_SpineDBEditorRemove.py
--rw-rw-rw-   0        0        0     9118 2021-12-02 08:08:09.000000 spinetoolbox-0.6.8/tests/spine_db_editor/widgets/test_SpineDBEditorUpdate.py
--rw-rw-rw-   0        0        0     5064 2021-10-18 10:21:24.000000 spinetoolbox-0.6.8/tests/spine_db_editor/widgets/test_SpineDBEditorWithDBMapping.py
--rw-rw-rw-   0        0        0     5530 2022-03-14 06:44:04.000000 spinetoolbox-0.6.8/tests/spine_db_editor/widgets/test_addItemsDialog.py
--rw-rw-rw-   0        0        0     3944 2021-02-04 14:00:40.000000 spinetoolbox-0.6.8/tests/spine_db_editor/widgets/test_custom_qwidgets.py
--rw-rw-rw-   0        0        0    34960 2021-02-23 09:40:58.000000 spinetoolbox-0.6.8/tests/test_ProjectUpgrader.py
--rw-rw-rw-   0        0        0    11635 2022-05-02 05:39:31.000000 spinetoolbox-0.6.8/tests/test_SpineDBManager.py
--rw-rw-rw-   0        0        0    14786 2022-02-10 09:52:07.000000 spinetoolbox-0.6.8/tests/test_helpers.py
--rw-rw-rw-   0        0        0     2437 2021-12-14 12:06:17.000000 spinetoolbox-0.6.8/tests/test_load_project_items.py
--rw-rw-rw-   0        0        0    25004 2022-04-20 07:20:21.000000 spinetoolbox-0.6.8/tests/test_plotting.py
--rw-rw-rw-   0        0        0    27180 2022-04-20 07:20:21.000000 spinetoolbox-0.6.8/tests/test_spineToolboxProject.py
--rw-rw-rw-   0        0        0    54340 2022-06-03 11:35:10.000000 spinetoolbox-0.6.8/tests/test_toolboxUI.py
-drwxrwxrwx   0        0        0        0 2022-06-03 12:30:32.117941 spinetoolbox-0.6.8/tests/widgets/
--rw-rw-rw-   0        0        0     1101 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/tests/widgets/__init__.py
--rw-rw-rw-   0        0        0     5757 2021-04-19 12:30:41.000000 spinetoolbox-0.6.8/tests/widgets/test_AddProjectItemWidget.py
--rw-rw-rw-   0        0        0    12576 2021-03-04 09:18:53.000000 spinetoolbox-0.6.8/tests/widgets/test_AddUpSpineOptWizard.py
--rw-rw-rw-   0        0        0     5778 2021-09-28 12:37:12.000000 spinetoolbox-0.6.8/tests/widgets/test_ArrayTableView.py
--rw-rw-rw-   0        0        0     6859 2022-03-25 08:35:13.000000 spinetoolbox-0.6.8/tests/widgets/test_CopyPasteTableView.py
--rw-rw-rw-   0        0        0     1831 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/tests/widgets/test_DatetimeEditor.py
--rw-rw-rw-   0        0        0     1807 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/tests/widgets/test_DurationEditor.py
--rw-rw-rw-   0        0        0     8265 2021-09-28 12:37:12.000000 spinetoolbox-0.6.8/tests/widgets/test_IndexedValueTableView.py
--rw-rw-rw-   0        0        0     5308 2021-03-31 12:11:44.000000 spinetoolbox-0.6.8/tests/widgets/test_InstallJuliaWizard.py
--rw-rw-rw-   0        0        0     1847 2021-05-11 05:36:06.000000 spinetoolbox-0.6.8/tests/widgets/test_JupyterConsoleWidget.py
--rw-rw-rw-   0        0        0     1790 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/tests/widgets/test_MapEditor.py
--rw-rw-rw-   0        0        0     5067 2021-09-28 12:37:12.000000 spinetoolbox-0.6.8/tests/widgets/test_MapTableView.py
--rw-rw-rw-   0        0        0     4736 2021-10-18 10:21:24.000000 spinetoolbox-0.6.8/tests/widgets/test_ParameterValueEditor.py
--rw-rw-rw-   0        0        0     1788 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/tests/widgets/test_PlainParameterValueEditor.py
--rw-rw-rw-   0        0        0     1878 2021-10-18 10:21:24.000000 spinetoolbox-0.6.8/tests/widgets/test_TimePatternEditor.py
--rw-rw-rw-   0        0        0     2139 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/tests/widgets/test_TimeSeriesFixedResolutionEditor.py
--rw-rw-rw-   0        0        0     6004 2021-06-09 09:03:40.000000 spinetoolbox-0.6.8/tests/widgets/test_TimeSeriesFixedResolutionTableView.py
--rw-rw-rw-   0        0        0     2371 2021-01-15 05:49:31.000000 spinetoolbox-0.6.8/tests/widgets/test_TimeSeriesVariableResolutionEditor.py
--rw-rw-rw-   0        0        0     4620 2021-07-09 05:39:38.000000 spinetoolbox-0.6.8/tests/widgets/test_custom_editors.py
--rw-rw-rw-   0        0        0     3113 2022-02-25 10:16:01.000000 spinetoolbox-0.6.8/tests/widgets/test_custom_qtextbrowser.py
--rw-rw-rw-   0        0        0    18396 2021-12-02 08:08:09.000000 spinetoolbox-0.6.8/tests/widgets/test_indexed_value_table_context_menu.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:58.370620 spinetoolbox-0.6.9/
+-rw-rw-rw-   0        0        0    35823 2019-06-13 10:03:34.000000 spinetoolbox-0.6.9/COPYING
+-rw-rw-rw-   0        0        0     7815 2019-06-13 10:03:34.000000 spinetoolbox-0.6.9/COPYING.LESSER
+-rw-rw-rw-   0        0        0       24 2021-06-29 09:23:47.000000 spinetoolbox-0.6.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    12592 2022-06-07 07:53:58.370620 spinetoolbox-0.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11965 2022-05-10 05:21:59.000000 spinetoolbox-0.6.9/README.md
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:56.218491 spinetoolbox-0.6.9/execution_tests/
+-rw-rw-rw-   0        0        0        0 2021-03-04 13:14:27.000000 spinetoolbox-0.6.9/execution_tests/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:56.249741 spinetoolbox-0.6.9/execution_tests/scenario_filters/
+-rw-rw-rw-   0        0        0        0 2022-03-01 07:13:30.000000 spinetoolbox-0.6.9/execution_tests/scenario_filters/__init__.py
+-rw-rw-rw-   0        0        0     3159 2022-03-25 08:35:13.000000 spinetoolbox-0.6.9/execution_tests/scenario_filters/execution_test.py
+-rw-rw-rw-   0        0        0      317 2021-03-04 13:14:27.000000 spinetoolbox-0.6.9/execution_tests/scenario_filters/tool.py
+-rw-rw-rw-   0        0        0      131 2019-09-03 05:24:26.000000 spinetoolbox-0.6.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1460 2022-06-07 07:53:58.386285 spinetoolbox-0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2021-06-29 09:23:47.000000 spinetoolbox-0.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:56.534552 spinetoolbox-0.6.9/spinetoolbox/
+-rw-rw-rw-   0        0        0     1068 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/__init__.py
+-rw-rw-rw-   0        0        0     1179 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/__main__.py
+-rw-rw-rw-   0        0        0     6684 2022-03-14 06:44:04.000000 spinetoolbox-0.6.9/spinetoolbox/config.py
+-rw-rw-rw-   0        0        0    11717 2021-11-01 09:17:28.000000 spinetoolbox-0.6.9/spinetoolbox/execution_managers.py
+-rw-rw-rw-   0        0        0    20811 2022-06-03 11:35:20.000000 spinetoolbox-0.6.9/spinetoolbox/headless.py
+-rw-rw-rw-   0        0        0    54363 2022-06-03 11:35:10.000000 spinetoolbox-0.6.9/spinetoolbox/helpers.py
+-rw-rw-rw-   0        0        0    24325 2022-06-03 11:35:10.000000 spinetoolbox-0.6.9/spinetoolbox/link.py
+-rw-rw-rw-   0        0        0     3487 2021-08-11 09:23:18.000000 spinetoolbox-0.6.9/spinetoolbox/load_project_items.py
+-rw-rw-rw-   0        0        0     2208 2022-02-10 09:52:07.000000 spinetoolbox-0.6.9/spinetoolbox/log_mixin.py
+-rw-rw-rw-   0        0        0     2279 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/logger_interface.py
+-rw-rw-rw-   0        0        0     4590 2022-06-03 11:35:20.000000 spinetoolbox-0.6.9/spinetoolbox/main.py
+-rw-rw-rw-   0        0        0     2103 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/metaobject.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:56.719477 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/
+-rw-rw-rw-   0        0        0     1305 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/__init__.py
+-rw-rw-rw-   0        0        0    10183 2021-06-09 09:03:40.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/array_model.py
+-rw-rw-rw-   0        0        0    14938 2022-05-02 05:39:31.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/compound_table_model.py
+-rw-rw-rw-   0        0        0     4681 2022-03-30 11:15:00.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/empty_row_model.py
+-rw-rw-rw-   0        0        0    13414 2021-12-30 13:53:42.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/file_list_models.py
+-rw-rw-rw-   0        0        0    14288 2021-11-01 09:17:28.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/filter_checkbox_list_model.py
+-rw-rw-rw-   0        0        0     2040 2022-03-14 06:44:04.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/filter_execution_model.py
+-rw-rw-rw-   0        0        0     3691 2021-06-09 09:03:40.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/indexed_value_table_model.py
+-rw-rw-rw-   0        0        0    19094 2021-12-02 08:08:09.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/map_model.py
+-rw-rw-rw-   0        0        0    10408 2022-05-02 05:39:31.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/minimal_table_model.py
+-rw-rw-rw-   0        0        0    12631 2022-03-14 06:44:04.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/minimal_tree_model.py
+-rw-rw-rw-   0        0        0    13126 2022-01-31 08:50:32.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/project_item_model.py
+-rw-rw-rw-   0        0        0     7890 2022-01-31 08:50:32.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/project_item_specification_models.py
+-rw-rw-rw-   0        0        0     7147 2022-01-25 09:58:33.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/project_tree_item.py
+-rw-rw-rw-   0        0        0     8318 2022-02-24 06:05:42.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/resource_filter_model.py
+-rw-rw-rw-   0        0        0     1152 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/shared.py
+-rw-rw-rw-   0        0        0     5820 2021-10-18 10:21:24.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/time_pattern_model.py
+-rw-rw-rw-   0        0        0     6972 2021-06-09 09:03:40.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/time_series_model_fixed_resolution.py
+-rw-rw-rw-   0        0        0     8489 2021-07-05 05:59:49.000000 spinetoolbox-0.6.9/spinetoolbox/mvcmodels/time_series_model_variable_resolution.py
+-rw-rw-rw-   0        0        0    25667 2022-04-20 07:20:21.000000 spinetoolbox-0.6.9/spinetoolbox/plotting.py
+-rw-rw-rw-   0        0        0    10804 2021-09-24 12:50:45.000000 spinetoolbox-0.6.9/spinetoolbox/plugin_manager.py
+-rw-rw-rw-   0        0        0    57400 2022-06-03 11:35:20.000000 spinetoolbox-0.6.9/spinetoolbox/project.py
+-rw-rw-rw-   0        0        0    23892 2022-04-20 07:20:21.000000 spinetoolbox-0.6.9/spinetoolbox/project_commands.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:56.750767 spinetoolbox-0.6.9/spinetoolbox/project_item/
+-rw-rw-rw-   0        0        0     1098 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/project_item/__init__.py
+-rw-rw-rw-   0        0        0     2621 2022-04-20 07:20:21.000000 spinetoolbox-0.6.9/spinetoolbox/project_item/logging_connection.py
+-rw-rw-rw-   0        0        0    18393 2022-03-25 08:35:13.000000 spinetoolbox-0.6.9/spinetoolbox/project_item/project_item.py
+-rw-rw-rw-   0        0        0     5165 2021-06-07 08:43:02.000000 spinetoolbox-0.6.9/spinetoolbox/project_item/project_item_factory.py
+-rw-rw-rw-   0        0        0    15018 2022-03-14 06:44:04.000000 spinetoolbox-0.6.9/spinetoolbox/project_item/specification_editor_window.py
+-rw-rw-rw-   0        0        0    27848 2022-04-29 06:30:43.000000 spinetoolbox-0.6.9/spinetoolbox/project_item_icon.py
+-rw-rw-rw-   0        0        0    29100 2021-12-29 13:41:06.000000 spinetoolbox-0.6.9/spinetoolbox/project_upgrader.py
+-rw-rw-rw-   0        0        0   944939 2022-05-02 05:39:31.000000 spinetoolbox-0.6.9/spinetoolbox/resources_icons_rc.py
+-rw-rw-rw-   0        0        0   443550 2022-04-29 06:30:43.000000 spinetoolbox-0.6.9/spinetoolbox/resources_logos_rc.py
+-rw-rw-rw-   0        0        0    16471 2022-05-02 05:39:31.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_commands.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:56.788077 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/
+-rw-rw-rw-   0        0        0     1101 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/__init__.py
+-rw-rw-rw-   0        0        0    31726 2022-03-25 08:35:13.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/graphics_items.py
+-rw-rw-rw-   0        0        0     1824 2021-11-09 06:04:47.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/main.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:56.982239 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/
+-rw-rw-rw-   0        0        0     1300 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/__init__.py
+-rw-rw-rw-   0        0        0     7830 2022-03-14 06:44:04.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/alternative_scenario_item.py
+-rw-rw-rw-   0        0        0     6679 2021-10-18 10:21:24.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/alternative_scenario_model.py
+-rw-rw-rw-   0        0        0     1147 2022-05-02 05:39:31.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/colors.py
+-rw-rw-rw-   0        0        0    26481 2022-01-31 08:50:32.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/compound_parameter_models.py
+-rw-rw-rw-   0        0        0    12466 2021-10-18 10:21:24.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/empty_parameter_models.py
+-rw-rw-rw-   0        0        0    12114 2021-12-02 08:08:09.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/entity_tree_item.py
+-rw-rw-rw-   0        0        0    13113 2021-11-15 07:59:53.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/entity_tree_models.py
+-rw-rw-rw-   0        0        0     4311 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/frozen_table_model.py
+-rw-rw-rw-   0        0        0     9976 2022-05-02 05:39:31.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/item_metadata_table_model.py
+-rw-rw-rw-   0        0        0     6864 2022-05-02 05:39:31.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/metadata_table_model.py
+-rw-rw-rw-   0        0        0    18387 2022-05-02 05:39:31.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/metadata_table_model_base.py
+-rw-rw-rw-   0        0        0    17243 2022-05-02 05:39:31.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/multi_db_tree_item.py
+-rw-rw-rw-   0        0        0     3255 2021-11-15 07:59:53.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/multi_db_tree_model.py
+-rw-rw-rw-   0        0        0    23553 2021-09-15 11:40:52.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/parameter_mixins.py
+-rw-rw-rw-   0        0        0     4471 2022-03-25 08:35:13.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/parameter_value_list_item.py
+-rw-rw-rw-   0        0        0     4097 2022-03-25 08:35:13.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/parameter_value_list_model.py
+-rw-rw-rw-   0        0        0    10476 2021-09-20 06:33:12.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/pivot_model.py
+-rw-rw-rw-   0        0        0    58155 2022-01-31 08:50:32.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/pivot_table_models.py
+-rw-rw-rw-   0        0        0    19461 2022-05-02 05:39:31.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/single_parameter_models.py
+-rw-rw-rw-   0        0        0    12258 2022-03-14 06:44:04.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/tool_feature_item.py
+-rw-rw-rw-   0        0        0    11403 2022-03-14 06:44:04.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/tool_feature_model.py
+-rw-rw-rw-   0        0        0     8915 2022-03-14 06:44:04.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/tree_item_utility.py
+-rw-rw-rw-   0        0        0     5808 2022-03-14 06:44:04.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/tree_model_base.py
+-rw-rw-rw-   0        0        0     2209 2021-09-20 11:07:08.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/scenario_generation.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:57.005675 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/ui/
+-rw-rw-rw-   0        0        0     1097 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/ui/__init__.py
+-rw-rw-rw-   0        0        0     5909 2021-09-20 11:07:08.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/ui/scenario_generator.py
+-rw-rw-rw-   0        0        0    42820 2022-05-02 05:39:31.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/ui/spine_db_editor_window.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:57.251643 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/
+-rw-rw-rw-   0        0        0     1078 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/__init__.py
+-rw-rw-rw-   0        0        0    47996 2021-10-04 12:46:07.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/add_items_dialogs.py
+-rw-rw-rw-   0        0        0     8285 2021-12-29 06:38:28.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/commit_viewer.py
+-rw-rw-rw-   0        0        0    36021 2022-05-02 05:39:31.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/custom_delegates.py
+-rw-rw-rw-   0        0        0     9284 2021-06-02 06:15:48.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/custom_menus.py
+-rw-rw-rw-   0        0        0    37937 2022-04-29 06:30:43.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/custom_qgraphicsviews.py
+-rw-rw-rw-   0        0        0    41832 2022-06-03 11:35:10.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/custom_qtableview.py
+-rw-rw-rw-   0        0        0    30453 2022-06-03 11:35:10.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/custom_qtreeview.py
+-rw-rw-rw-   0        0        0     6185 2022-03-14 06:44:04.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/custom_qwidgets.py
+-rw-rw-rw-   0        0        0    18946 2021-10-04 12:46:07.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/edit_or_remove_items_dialogs.py
+-rw-rw-rw-   0        0        0     6533 2022-05-27 09:02:28.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/graph_layout_generator.py
+-rw-rw-rw-   0        0        0    27337 2022-06-03 11:35:10.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/graph_view_mixin.py
+-rw-rw-rw-   0        0        0     7429 2022-05-02 05:39:31.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/item_metadata_editor.py
+-rw-rw-rw-   0        0        0     8679 2021-10-06 09:32:23.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/manage_items_dialogs.py
+-rw-rw-rw-   0        0        0     7260 2022-03-29 12:53:01.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/mass_select_items_dialogs.py
+-rw-rw-rw-   0        0        0     4057 2022-05-02 05:39:31.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/metadata_editor.py
+-rw-rw-rw-   0        0        0     8554 2022-03-14 06:44:04.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/multi_spine_db_editor.py
+-rw-rw-rw-   0        0        0     4400 2022-03-25 08:35:13.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/object_name_list_editor.py
+-rw-rw-rw-   0        0        0    14428 2022-06-03 11:35:10.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/parameter_view_mixin.py
+-rw-rw-rw-   0        0        0     6846 2021-09-20 11:07:08.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/pivot_table_header_view.py
+-rw-rw-rw-   0        0        0     8104 2021-09-20 11:07:08.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/scenario_generator.py
+-rw-rw-rw-   0        0        0     4425 2022-03-25 08:35:13.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/select_position_parameters_dialog.py
+-rw-rw-rw-   0        0        0    58072 2022-06-03 11:35:10.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/spine_db_editor.py
+-rw-rw-rw-   0        0        0     5258 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/tabular_view_header_widget.py
+-rw-rw-rw-   0        0        0    42782 2022-06-03 11:35:10.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/tabular_view_mixin.py
+-rw-rw-rw-   0        0        0    17330 2022-06-03 11:35:10.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/tree_view_mixin.py
+-rw-rw-rw-   0        0        0    13880 2022-03-14 06:44:04.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/url_toolbar.py
+-rw-rw-rw-   0        0        0     8127 2022-06-03 11:35:10.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_icon_manager.py
+-rw-rw-rw-   0        0        0    94362 2022-06-03 11:35:10.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_manager.py
+-rw-rw-rw-   0        0        0    15000 2022-05-10 13:02:08.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_parcel.py
+-rw-rw-rw-   0        0        0    18671 2022-05-02 05:39:31.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_signaller.py
+-rw-rw-rw-   0        0        0    19717 2022-05-10 05:21:59.000000 spinetoolbox-0.6.9/spinetoolbox/spine_db_worker.py
+-rw-rw-rw-   0        0        0    10720 2022-05-10 05:21:59.000000 spinetoolbox-0.6.9/spinetoolbox/spine_engine_manager.py
+-rw-rw-rw-   0        0        0    16058 2022-05-03 08:41:44.000000 spinetoolbox-0.6.9/spinetoolbox/spine_engine_worker.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:57.420982 spinetoolbox-0.6.9/spinetoolbox/ui/
+-rw-rw-rw-   0        0        0     1090 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/ui/__init__.py
+-rw-rw-rw-   0        0        0    24546 2021-04-09 12:18:00.000000 spinetoolbox-0.6.9/spinetoolbox/ui/about.py
+-rw-rw-rw-   0        0        0     8383 2021-05-10 13:23:24.000000 spinetoolbox-0.6.9/spinetoolbox/ui/add_project_item.py
+-rw-rw-rw-   0        0        0     6682 2021-06-09 09:03:40.000000 spinetoolbox-0.6.9/spinetoolbox/ui/array_editor.py
+-rw-rw-rw-   0        0        0     3650 2021-05-10 13:23:24.000000 spinetoolbox-0.6.9/spinetoolbox/ui/datetime_editor.py
+-rw-rw-rw-   0        0        0     3467 2021-05-10 13:23:24.000000 spinetoolbox-0.6.9/spinetoolbox/ui/duration_editor.py
+-rw-rw-rw-   0        0        0     2626 2021-05-10 13:23:24.000000 spinetoolbox-0.6.9/spinetoolbox/ui/import_source_selector.py
+-rw-rw-rw-   0        0        0     5070 2022-02-07 09:52:28.000000 spinetoolbox-0.6.9/spinetoolbox/ui/jump_properties.py
+-rw-rw-rw-   0        0        0    21001 2021-03-31 12:11:44.000000 spinetoolbox-0.6.9/spinetoolbox/ui/kernel_editor_dialog.py
+-rw-rw-rw-   0        0        0     3327 2022-02-25 07:20:57.000000 spinetoolbox-0.6.9/spinetoolbox/ui/link_properties.py
+-rw-rw-rw-   0        0        0    41474 2022-02-25 10:16:01.000000 spinetoolbox-0.6.9/spinetoolbox/ui/mainwindow.py
+-rw-rw-rw-   0        0        0     3488 2021-09-20 11:07:08.000000 spinetoolbox-0.6.9/spinetoolbox/ui/map_editor.py
+-rw-rw-rw-   0        0        0     9012 2021-04-28 05:10:32.000000 spinetoolbox-0.6.9/spinetoolbox/ui/mini_kernel_editor_dialog.py
+-rw-rw-rw-   0        0        0     6974 2021-05-10 13:23:24.000000 spinetoolbox-0.6.9/spinetoolbox/ui/open_project_dialog.py
+-rw-rw-rw-   0        0        0     4818 2021-07-09 05:39:38.000000 spinetoolbox-0.6.9/spinetoolbox/ui/parameter_value_editor.py
+-rw-rw-rw-   0        0        0     4589 2021-05-10 13:23:24.000000 spinetoolbox-0.6.9/spinetoolbox/ui/plain_parameter_value_editor.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:57.436610 spinetoolbox-0.6.9/spinetoolbox/ui/resources/
+-rw-rw-rw-   0        0        0        0 2022-05-05 12:16:25.000000 spinetoolbox-0.6.9/spinetoolbox/ui/resources/__init__.py
+-rw-rw-rw-   0        0        0    12254 2019-06-13 10:03:34.000000 spinetoolbox-0.6.9/spinetoolbox/ui/resources/app.ico
+-rw-rw-rw-   0        0        0    25955 2022-05-04 09:15:52.000000 spinetoolbox-0.6.9/spinetoolbox/ui/resources/cat.py
+-rw-rw-rw-   0        0        0    65674 2022-01-25 09:58:33.000000 spinetoolbox-0.6.9/spinetoolbox/ui/settings.py
+-rw-rw-rw-   0        0        0    14516 2021-05-10 13:23:24.000000 spinetoolbox-0.6.9/spinetoolbox/ui/spine_datapackage_form.py
+-rw-rw-rw-   0        0        0     3299 2021-09-20 06:33:12.000000 spinetoolbox-0.6.9/spinetoolbox/ui/time_pattern_editor.py
+-rw-rw-rw-   0        0        0     7745 2021-06-09 09:03:40.000000 spinetoolbox-0.6.9/spinetoolbox/ui/time_series_fixed_resolution_editor.py
+-rw-rw-rw-   0        0        0     4864 2021-06-09 09:03:40.000000 spinetoolbox-0.6.9/spinetoolbox/ui/time_series_variable_resolution_editor.py
+-rw-rw-rw-   0        0        0     5330 2021-05-10 13:23:24.000000 spinetoolbox-0.6.9/spinetoolbox/ui/tool_configuration_assistant.py
+-rw-rw-rw-   0        0        0   106766 2022-05-04 09:15:52.000000 spinetoolbox-0.6.9/spinetoolbox/ui_main.py
+-rw-rw-rw-   0        0        0     2179 2022-06-07 07:53:42.000000 spinetoolbox-0.6.9/spinetoolbox/version.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:57.869079 spinetoolbox-0.6.9/spinetoolbox/widgets/
+-rw-rw-rw-   0        0        0     1095 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/__init__.py
+-rw-rw-rw-   0        0        0     6485 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/about_widget.py
+-rw-rw-rw-   0        0        0     6073 2021-05-20 12:10:49.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/add_project_item_widget.py
+-rw-rw-rw-   0        0        0    22171 2021-03-04 13:02:41.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/add_up_spine_opt_wizard.py
+-rw-rw-rw-   0        0        0     6061 2021-06-09 09:03:40.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/array_editor.py
+-rw-rw-rw-   0        0        0     2440 2021-05-31 05:32:28.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/array_value_editor.py
+-rw-rw-rw-   0        0        0     6087 2021-12-13 12:55:05.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/code_text_edit.py
+-rw-rw-rw-   0        0        0     3254 2021-09-15 11:40:52.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/commit_dialog.py
+-rw-rw-rw-   0        0        0     2701 2021-11-15 08:00:02.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/console_window.py
+-rw-rw-rw-   0        0        0     4266 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/custom_combobox.py
+-rw-rw-rw-   0        0        0     6422 2021-07-05 05:59:49.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/custom_delegates.py
+-rw-rw-rw-   0        0        0    18913 2022-03-25 08:35:13.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/custom_editors.py
+-rw-rw-rw-   0        0        0     8230 2021-11-01 09:17:28.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/custom_menus.py
+-rw-rw-rw-   0        0        0     1580 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/custom_qcombobox.py
+-rw-rw-rw-   0        0        0    13578 2022-05-04 09:15:52.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/custom_qgraphicsscene.py
+-rw-rw-rw-   0        0        0    19926 2022-04-20 07:20:21.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/custom_qgraphicsviews.py
+-rw-rw-rw-   0        0        0     4525 2022-01-31 08:50:32.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/custom_qlineedits.py
+-rw-rw-rw-   0        0        0    34304 2022-05-02 05:39:31.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/custom_qtableview.py
+-rw-rw-rw-   0        0        0    10534 2022-03-14 06:44:04.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/custom_qtextbrowser.py
+-rw-rw-rw-   0        0        0     3863 2021-03-17 11:51:57.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/custom_qtreeview.py
+-rw-rw-rw-   0        0        0    23885 2022-06-03 11:35:10.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/custom_qwidgets.py
+-rw-rw-rw-   0        0        0     3116 2021-03-01 11:44:55.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/datetime_editor.py
+-rw-rw-rw-   0        0        0     2502 2021-03-01 11:44:55.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/duration_editor.py
+-rw-rw-rw-   0        0        0    13246 2021-12-02 08:08:09.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/indexed_value_table_context_menu.py
+-rw-rw-rw-   0        0        0    11034 2021-07-05 05:59:49.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/install_julia_wizard.py
+-rw-rw-rw-   0        0        0     6089 2022-04-20 07:20:21.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/jump_properties_widget.py
+-rw-rw-rw-   0        0        0    13366 2022-05-03 08:41:44.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/jupyter_console_widget.py
+-rw-rw-rw-   0        0        0    56612 2021-09-06 09:57:11.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/kernel_editor.py
+-rw-rw-rw-   0        0        0     4134 2022-03-29 12:53:01.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/link_properties_widget.py
+-rw-rw-rw-   0        0        0     3739 2021-06-09 09:03:40.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/map_editor.py
+-rw-rw-rw-   0        0        0     2758 2021-07-09 05:39:38.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/map_value_editor.py
+-rw-rw-rw-   0        0        0     3380 2021-09-06 09:57:11.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/multi_tab_spec_editor.py
+-rw-rw-rw-   0        0        0    21682 2022-04-20 07:20:21.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/multi_tab_window.py
+-rw-rw-rw-   0        0        0    10077 2022-03-14 06:44:04.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/notification.py
+-rw-rw-rw-   0        0        0    19787 2021-09-06 09:57:11.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/open_project_widget.py
+-rw-rw-rw-   0        0        0     3636 2021-06-09 09:03:40.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/parameter_value_editor.py
+-rw-rw-rw-   0        0        0     9369 2022-04-25 05:51:19.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/parameter_value_editor_base.py
+-rw-rw-rw-   0        0        0    30386 2022-06-03 11:35:10.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/persistent_console_widget.py
+-rw-rw-rw-   0        0        0     2943 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/plain_parameter_value_editor.py
+-rw-rw-rw-   0        0        0     2254 2022-04-20 07:20:21.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/plot_canvas.py
+-rw-rw-rw-   0        0        0     7420 2022-06-03 11:35:10.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/plot_widget.py
+-rw-rw-rw-   0        0        0     6329 2021-03-04 09:18:53.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/plugin_manager_widgets.py
+-rw-rw-rw-   0        0        0    19180 2022-01-31 08:50:32.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/project_item_drag.py
+-rw-rw-rw-   0        0        0     3903 2022-03-14 06:50:13.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/properties_widget.py
+-rw-rw-rw-   0        0        0     3091 2021-09-30 07:33:33.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/rename_project_dialog.py
+-rw-rw-rw-   0        0        0     1329 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/report_plotting_failure.py
+-rw-rw-rw-   0        0        0    44898 2022-01-25 09:58:33.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/settings_widget.py
+-rw-rw-rw-   0        0        0     2818 2022-02-10 09:52:07.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/statusbars.py
+-rw-rw-rw-   0        0        0     3098 2021-09-20 06:33:12.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/time_pattern_editor.py
+-rw-rw-rw-   0        0        0     7905 2021-06-09 09:03:40.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/time_series_fixed_resolution_editor.py
+-rw-rw-rw-   0        0        0     4613 2021-06-09 09:03:40.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/time_series_variable_resolution_editor.py
+-rw-rw-rw-   0        0        0    12814 2021-12-02 08:08:09.000000 spinetoolbox-0.6.9/spinetoolbox/widgets/toolbars.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:56.565800 spinetoolbox-0.6.9/spinetoolbox.egg-info/
+-rw-rw-rw-   0        0        0    12592 2022-06-07 07:53:52.000000 spinetoolbox-0.6.9/spinetoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11731 2022-06-07 07:53:56.000000 spinetoolbox-0.6.9/spinetoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-07 07:53:52.000000 spinetoolbox-0.6.9/spinetoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2022-06-07 07:53:52.000000 spinetoolbox-0.6.9/spinetoolbox.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2019-10-04 13:19:54.000000 spinetoolbox-0.6.9/spinetoolbox.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      269 2022-06-07 07:53:52.000000 spinetoolbox-0.6.9/spinetoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2022-06-07 07:53:52.000000 spinetoolbox-0.6.9/spinetoolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:57.953774 spinetoolbox-0.6.9/tests/
+-rw-rw-rw-   0        0        0     1095 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/tests/__init__.py
+-rw-rw-rw-   0        0        0    12423 2022-03-14 06:44:04.000000 spinetoolbox-0.6.9/tests/mock_helpers.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:58.038509 spinetoolbox-0.6.9/tests/mvcmodels/
+-rw-rw-rw-   0        0        0     1103 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/tests/mvcmodels/__init__.py
+-rw-rw-rw-   0        0        0     5595 2021-06-09 09:03:40.000000 spinetoolbox-0.6.9/tests/mvcmodels/test_ArrayModel.py
+-rw-rw-rw-   0        0        0    18146 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/tests/mvcmodels/test_FilterCheckboxList.py
+-rw-rw-rw-   0        0        0     3610 2021-06-09 09:03:40.000000 spinetoolbox-0.6.9/tests/mvcmodels/test_IndexedValueTableModel.py
+-rw-rw-rw-   0        0        0    24434 2021-07-09 05:39:38.000000 spinetoolbox-0.6.9/tests/mvcmodels/test_MapModel.py
+-rw-rw-rw-   0        0        0    12319 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/tests/mvcmodels/test_MinimalTableModel.py
+-rw-rw-rw-   0        0        0     4443 2022-01-31 08:50:32.000000 spinetoolbox-0.6.9/tests/mvcmodels/test_ProjectItemModel.py
+-rw-rw-rw-   0        0        0     6212 2021-10-18 10:21:24.000000 spinetoolbox-0.6.9/tests/mvcmodels/test_TimePatternModel.py
+-rw-rw-rw-   0        0        0    10768 2021-06-09 09:03:40.000000 spinetoolbox-0.6.9/tests/mvcmodels/test_TimeSeriesModelFixedResolution.py
+-rw-rw-rw-   0        0        0     9887 2021-06-09 09:03:40.000000 spinetoolbox-0.6.9/tests/mvcmodels/test_TimeSeriesModelVariableResolution.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:58.054094 spinetoolbox-0.6.9/tests/project_item/
+-rw-rw-rw-   0        0        0     1107 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/tests/project_item/__init__.py
+-rw-rw-rw-   0        0        0     3050 2021-05-20 12:10:49.000000 spinetoolbox-0.6.9/tests/project_item/test_ProjectItem.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:58.069755 spinetoolbox-0.6.9/tests/spine_db_editor/
+-rw-rw-rw-   0        0        0     1070 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/tests/spine_db_editor/__init__.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:58.123155 spinetoolbox-0.6.9/tests/spine_db_editor/mvcmodels/
+-rw-rw-rw-   0        0        0      979 2021-01-22 12:30:03.000000 spinetoolbox-0.6.9/tests/spine_db_editor/mvcmodels/__init__.py
+-rw-rw-rw-   0        0        0     7521 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/tests/spine_db_editor/mvcmodels/test_PivotModel.py
+-rw-rw-rw-   0        0        0     8395 2022-06-03 11:35:10.000000 spinetoolbox-0.6.9/tests/spine_db_editor/mvcmodels/test_PivotTableModel.py
+-rw-rw-rw-   0        0        0    11479 2021-11-01 09:17:28.000000 spinetoolbox-0.6.9/tests/spine_db_editor/mvcmodels/test_alternative_scenario_model.py
+-rw-rw-rw-   0        0        0    12538 2021-11-01 09:17:28.000000 spinetoolbox-0.6.9/tests/spine_db_editor/mvcmodels/test_compound_parameter_models.py
+-rw-rw-rw-   0        0        0    10795 2022-03-14 06:44:04.000000 spinetoolbox-0.6.9/tests/spine_db_editor/mvcmodels/test_emptyParameterModels.py
+-rw-rw-rw-   0        0        0     6114 2021-12-02 08:08:09.000000 spinetoolbox-0.6.9/tests/spine_db_editor/test_graphics_items.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:58.207885 spinetoolbox-0.6.9/tests/spine_db_editor/widgets/
+-rw-rw-rw-   0        0        0     1081 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/tests/spine_db_editor/widgets/__init__.py
+-rw-rw-rw-   0        0        0    18758 2022-04-29 06:30:43.000000 spinetoolbox-0.6.9/tests/spine_db_editor/widgets/test_SpineDBEditor.py
+-rw-rw-rw-   0        0        0    10030 2021-11-15 07:59:53.000000 spinetoolbox-0.6.9/tests/spine_db_editor/widgets/test_SpineDBEditorAdd.py
+-rw-rw-rw-   0        0        0     3497 2021-08-09 10:52:23.000000 spinetoolbox-0.6.9/tests/spine_db_editor/widgets/test_SpineDBEditorBase.py
+-rw-rw-rw-   0        0        0     7580 2021-09-06 09:57:11.000000 spinetoolbox-0.6.9/tests/spine_db_editor/widgets/test_SpineDBEditorFilter.py
+-rw-rw-rw-   0        0        0     8439 2021-09-06 09:57:11.000000 spinetoolbox-0.6.9/tests/spine_db_editor/widgets/test_SpineDBEditorRemove.py
+-rw-rw-rw-   0        0        0     9118 2021-12-02 08:08:09.000000 spinetoolbox-0.6.9/tests/spine_db_editor/widgets/test_SpineDBEditorUpdate.py
+-rw-rw-rw-   0        0        0     5064 2021-10-18 10:21:24.000000 spinetoolbox-0.6.9/tests/spine_db_editor/widgets/test_SpineDBEditorWithDBMapping.py
+-rw-rw-rw-   0        0        0     5530 2022-03-14 06:44:04.000000 spinetoolbox-0.6.9/tests/spine_db_editor/widgets/test_addItemsDialog.py
+-rw-rw-rw-   0        0        0     3944 2021-02-04 14:00:40.000000 spinetoolbox-0.6.9/tests/spine_db_editor/widgets/test_custom_qwidgets.py
+-rw-rw-rw-   0        0        0    34960 2021-02-23 09:40:58.000000 spinetoolbox-0.6.9/tests/test_ProjectUpgrader.py
+-rw-rw-rw-   0        0        0    11635 2022-05-02 05:39:31.000000 spinetoolbox-0.6.9/tests/test_SpineDBManager.py
+-rw-rw-rw-   0        0        0    14786 2022-02-10 09:52:07.000000 spinetoolbox-0.6.9/tests/test_helpers.py
+-rw-rw-rw-   0        0        0     2437 2021-12-14 12:06:17.000000 spinetoolbox-0.6.9/tests/test_load_project_items.py
+-rw-rw-rw-   0        0        0    25004 2022-04-20 07:20:21.000000 spinetoolbox-0.6.9/tests/test_plotting.py
+-rw-rw-rw-   0        0        0    27180 2022-04-20 07:20:21.000000 spinetoolbox-0.6.9/tests/test_spineToolboxProject.py
+-rw-rw-rw-   0        0        0    54340 2022-06-03 11:35:10.000000 spinetoolbox-0.6.9/tests/test_toolboxUI.py
+drwxrwxrwx   0        0        0        0 2022-06-07 07:53:58.370620 spinetoolbox-0.6.9/tests/widgets/
+-rw-rw-rw-   0        0        0     1101 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/tests/widgets/__init__.py
+-rw-rw-rw-   0        0        0     5757 2021-04-19 12:30:41.000000 spinetoolbox-0.6.9/tests/widgets/test_AddProjectItemWidget.py
+-rw-rw-rw-   0        0        0    12576 2021-03-04 09:18:53.000000 spinetoolbox-0.6.9/tests/widgets/test_AddUpSpineOptWizard.py
+-rw-rw-rw-   0        0        0     5778 2021-09-28 12:37:12.000000 spinetoolbox-0.6.9/tests/widgets/test_ArrayTableView.py
+-rw-rw-rw-   0        0        0     6859 2022-03-25 08:35:13.000000 spinetoolbox-0.6.9/tests/widgets/test_CopyPasteTableView.py
+-rw-rw-rw-   0        0        0     1831 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/tests/widgets/test_DatetimeEditor.py
+-rw-rw-rw-   0        0        0     1807 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/tests/widgets/test_DurationEditor.py
+-rw-rw-rw-   0        0        0     8265 2021-09-28 12:37:12.000000 spinetoolbox-0.6.9/tests/widgets/test_IndexedValueTableView.py
+-rw-rw-rw-   0        0        0     5308 2021-03-31 12:11:44.000000 spinetoolbox-0.6.9/tests/widgets/test_InstallJuliaWizard.py
+-rw-rw-rw-   0        0        0     1847 2021-05-11 05:36:06.000000 spinetoolbox-0.6.9/tests/widgets/test_JupyterConsoleWidget.py
+-rw-rw-rw-   0        0        0     1790 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/tests/widgets/test_MapEditor.py
+-rw-rw-rw-   0        0        0     5067 2021-09-28 12:37:12.000000 spinetoolbox-0.6.9/tests/widgets/test_MapTableView.py
+-rw-rw-rw-   0        0        0     4736 2021-10-18 10:21:24.000000 spinetoolbox-0.6.9/tests/widgets/test_ParameterValueEditor.py
+-rw-rw-rw-   0        0        0     1788 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/tests/widgets/test_PlainParameterValueEditor.py
+-rw-rw-rw-   0        0        0     1878 2021-10-18 10:21:24.000000 spinetoolbox-0.6.9/tests/widgets/test_TimePatternEditor.py
+-rw-rw-rw-   0        0        0     2139 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/tests/widgets/test_TimeSeriesFixedResolutionEditor.py
+-rw-rw-rw-   0        0        0     6004 2021-06-09 09:03:40.000000 spinetoolbox-0.6.9/tests/widgets/test_TimeSeriesFixedResolutionTableView.py
+-rw-rw-rw-   0        0        0     2371 2021-01-15 05:49:31.000000 spinetoolbox-0.6.9/tests/widgets/test_TimeSeriesVariableResolutionEditor.py
+-rw-rw-rw-   0        0        0     4620 2021-07-09 05:39:38.000000 spinetoolbox-0.6.9/tests/widgets/test_custom_editors.py
+-rw-rw-rw-   0        0        0     3113 2022-02-25 10:16:01.000000 spinetoolbox-0.6.9/tests/widgets/test_custom_qtextbrowser.py
+-rw-rw-rw-   0        0        0    18396 2021-12-02 08:08:09.000000 spinetoolbox-0.6.9/tests/widgets/test_indexed_value_table_context_menu.py
```

### Comparing `spinetoolbox-0.6.8/COPYING` & `spinetoolbox-0.6.9/COPYING`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/COPYING.LESSER` & `spinetoolbox-0.6.9/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/PKG-INFO` & `spinetoolbox-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinetoolbox
-Version: 0.6.8
+Version: 0.6.9
 Summary: An application to define, manage, and execute various energy system simulation models
 Home-page: https://github.com/Spine-project/Spine-Toolbox
 Author: Spine Project consortium
 Author-email: spine_info@vtt.fi
 License: LGPL-3.0-or-later
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `spinetoolbox-0.6.8/README.md` & `spinetoolbox-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/execution_tests/scenario_filters/execution_test.py` & `spinetoolbox-0.6.9/execution_tests/scenario_filters/execution_test.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/setup.cfg` & `spinetoolbox-0.6.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -43,50 +43,50 @@
 000002a0: 6964 6532 203e 3d35 2e31 342c 203d 3d35  ide2 >=5.14, ==5
 000002b0: 2e31 342e 2a0d 0a09 6a75 7079 7465 722d  .14.*...jupyter-
 000002c0: 636c 6965 6e74 203c 372e 300d 0a09 746f  client <7.0...to
 000002d0: 726e 6164 6f20 3e3d 2036 2e31 0d0a 0971  rnado >= 6.1...q
 000002e0: 7463 6f6e 736f 6c65 203e 3d35 2e31 0d0a  tconsole >=5.1..
 000002f0: 0973 716c 616c 6368 656d 7920 3e3d 312e  .sqlalchemy >=1.
 00000300: 330d 0a09 7370 696e 6564 625f 6170 6920  3...spinedb_api 
-00000310: 3e3d 302e 3133 2e30 0d0a 0973 7069 6e65  >=0.13.0...spine
-00000320: 5f65 6e67 696e 6520 3e3d 302e 3131 2e30  _engine >=0.11.0
+00000310: 3e3d 302e 3138 2e30 0d0a 0973 7069 6e65  >=0.18.0...spine
+00000320: 5f65 6e67 696e 6520 3e3d 302e 3135 2e30  _engine >=0.15.0
 00000330: 0d0a 096e 756d 7079 203e 3d31 2e32 302e  ...numpy >=1.20.
 00000340: 320d 0a09 6d61 7470 6c6f 746c 6962 203e  2...matplotlib >
 00000350: 3d33 2e30 2c20 213d 332e 322e 312c 2021  =3.0, !=3.2.1, !
 00000360: 3d33 2e33 2e31 0d0a 0973 6369 7079 203e  =3.3.1...scipy >
 00000370: 3d31 2e37 2e31 0d0a 096e 6574 776f 726b  =1.7.1...network
 00000380: 7820 3e3d 322e 360d 0a09 7061 6e64 6173  x >=2.6...pandas
 00000390: 203e 3d31 2e33 2e32 0d0a 0970 7967 6d65   >=1.3.2...pygme
 000003a0: 6e74 7320 3e3d 322e 380d 0a09 6a69 6c6c  nts >=2.8...jill
 000003b0: 203e 3d30 2e39 2e32 0d0a 0970 797a 6d71   >=0.9.2...pyzmq
 000003c0: 203c 3232 2020 2320 6378 5f66 7265 657a   <22  # cx_freez
 000003d0: 6520 362e 3620 6861 7320 7472 6f75 626c  e 6.6 has troubl
 000003e0: 6520 6275 696c 6469 6e67 2070 797a 6d71  e building pyzmq
 000003f0: 3e3d 3232 0d0a 0973 7069 6e65 2d69 7465  >=22...spine-ite
-00000400: 6d73 203e 3d20 302e 382e 300d 0a69 6e63  ms >= 0.8.0..inc
-00000410: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
-00000420: 6120 3d20 5472 7565 0d0a 7079 7468 6f6e  a = True..python
-00000430: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-00000440: 372e 312c 203c 332e 392c 2021 3d33 2e38  7.1, <3.9, !=3.8
-00000450: 2e30 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  .0....[options.e
-00000460: 6e74 7279 5f70 6f69 6e74 735d 0d0a 636f  ntry_points]..co
-00000470: 6e73 6f6c 655f 7363 7269 7074 7320 3d20  nsole_scripts = 
-00000480: 0d0a 0973 7069 6e65 746f 6f6c 626f 783d  ...spinetoolbox=
-00000490: 7370 696e 6574 6f6f 6c62 6f78 2e6d 6169  spinetoolbox.mai
-000004a0: 6e3a 6d61 696e 0d0a 0973 7069 6e65 2d64  n:main...spine-d
-000004b0: 622d 6564 6974 6f72 3d73 7069 6e65 746f  b-editor=spineto
-000004c0: 6f6c 626f 782e 7370 696e 655f 6462 5f65  olbox.spine_db_e
-000004d0: 6469 746f 722e 6d61 696e 3a6d 6169 6e0d  ditor.main:main.
-000004e0: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-000004f0: 6167 6573 2e66 696e 645d 0d0a 6578 636c  ages.find]..excl
-00000500: 7564 6520 3d20 0d0a 0974 6573 7473 2a0d  ude = ...tests*.
-00000510: 0a09 6578 6563 7574 696f 6e5f 7465 7374  ..execution_test
-00000520: 732a 0d0a 0d0a 5b63 6f76 6572 6167 653a  s*....[coverage:
-00000530: 7275 6e5d 0d0a 736f 7572 6365 203d 2073  run]..source = s
-00000540: 7069 6e65 746f 6f6c 626f 780d 0a62 7261  pinetoolbox..bra
-00000550: 6e63 6820 3d20 5472 7565 0d0a 0d0a 5b63  nch = True....[c
-00000560: 6f76 6572 6167 653a 7265 706f 7274 5d0d  overage:report].
-00000570: 0a69 676e 6f72 655f 6572 726f 7273 203d  .ignore_errors =
-00000580: 2054 7275 650d 0a0d 0a5b 6567 675f 696e   True....[egg_in
-00000590: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-000005a0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-000005b0: 0a0d 0a                                  ...
+00000400: 6d73 203e 3d20 302e 3132 2e30 0d0a 696e  ms >= 0.12.0..in
+00000410: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
+00000420: 7461 203d 2054 7275 650d 0a70 7974 686f  ta = True..pytho
+00000430: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
+00000440: 2e37 2e31 2c20 3c33 2e39 2c20 213d 332e  .7.1, <3.9, !=3.
+00000450: 382e 300d 0a0d 0a5b 6f70 7469 6f6e 732e  8.0....[options.
+00000460: 656e 7472 795f 706f 696e 7473 5d0d 0a63  entry_points]..c
+00000470: 6f6e 736f 6c65 5f73 6372 6970 7473 203d  onsole_scripts =
+00000480: 200d 0a09 7370 696e 6574 6f6f 6c62 6f78   ...spinetoolbox
+00000490: 3d73 7069 6e65 746f 6f6c 626f 782e 6d61  =spinetoolbox.ma
+000004a0: 696e 3a6d 6169 6e0d 0a09 7370 696e 652d  in:main...spine-
+000004b0: 6462 2d65 6469 746f 723d 7370 696e 6574  db-editor=spinet
+000004c0: 6f6f 6c62 6f78 2e73 7069 6e65 5f64 625f  oolbox.spine_db_
+000004d0: 6564 6974 6f72 2e6d 6169 6e3a 6d61 696e  editor.main:main
+000004e0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
+000004f0: 6b61 6765 732e 6669 6e64 5d0d 0a65 7863  kages.find]..exc
+00000500: 6c75 6465 203d 200d 0a09 7465 7374 732a  lude = ...tests*
+00000510: 0d0a 0965 7865 6375 7469 6f6e 5f74 6573  ...execution_tes
+00000520: 7473 2a0d 0a0d 0a5b 636f 7665 7261 6765  ts*....[coverage
+00000530: 3a72 756e 5d0d 0a73 6f75 7263 6520 3d20  :run]..source = 
+00000540: 7370 696e 6574 6f6f 6c62 6f78 0d0a 6272  spinetoolbox..br
+00000550: 616e 6368 203d 2054 7275 650d 0a0d 0a5b  anch = True....[
+00000560: 636f 7665 7261 6765 3a72 6570 6f72 745d  coverage:report]
+00000570: 0d0a 6967 6e6f 7265 5f65 7272 6f72 7320  ..ignore_errors 
+00000580: 3d20 5472 7565 0d0a 0d0a 5b65 6767 5f69  = True....[egg_i
+00000590: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+000005a0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+000005b0: 0d0a 0d0a                                ....
```

### Comparing `spinetoolbox-0.6.8/setup.py` & `spinetoolbox-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/__init__.py` & `spinetoolbox-0.6.9/spinetoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/__main__.py` & `spinetoolbox-0.6.9/spinetoolbox/__main__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/config.py` & `spinetoolbox-0.6.9/spinetoolbox/config.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/execution_managers.py` & `spinetoolbox-0.6.9/spinetoolbox/execution_managers.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/headless.py` & `spinetoolbox-0.6.9/spinetoolbox/headless.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/helpers.py` & `spinetoolbox-0.6.9/spinetoolbox/helpers.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/link.py` & `spinetoolbox-0.6.9/spinetoolbox/link.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/load_project_items.py` & `spinetoolbox-0.6.9/spinetoolbox/load_project_items.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/log_mixin.py` & `spinetoolbox-0.6.9/spinetoolbox/log_mixin.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/logger_interface.py` & `spinetoolbox-0.6.9/spinetoolbox/logger_interface.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/main.py` & `spinetoolbox-0.6.9/spinetoolbox/main.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/metaobject.py` & `spinetoolbox-0.6.9/spinetoolbox/metaobject.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/__init__.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/array_model.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/array_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/compound_table_model.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/compound_table_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/empty_row_model.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/empty_row_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/file_list_models.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/file_list_models.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/filter_checkbox_list_model.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/filter_checkbox_list_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/filter_execution_model.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/filter_execution_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/indexed_value_table_model.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/indexed_value_table_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/map_model.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/map_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/minimal_table_model.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/minimal_table_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/minimal_tree_model.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/minimal_tree_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/project_item_model.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/project_item_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/project_item_specification_models.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/project_item_specification_models.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/project_tree_item.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/project_tree_item.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/resource_filter_model.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/resource_filter_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/shared.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/shared.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/time_pattern_model.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/time_pattern_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/time_series_model_fixed_resolution.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/time_series_model_fixed_resolution.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/mvcmodels/time_series_model_variable_resolution.py` & `spinetoolbox-0.6.9/spinetoolbox/mvcmodels/time_series_model_variable_resolution.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/plotting.py` & `spinetoolbox-0.6.9/spinetoolbox/plotting.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/plugin_manager.py` & `spinetoolbox-0.6.9/spinetoolbox/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/project.py` & `spinetoolbox-0.6.9/spinetoolbox/project.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/project_commands.py` & `spinetoolbox-0.6.9/spinetoolbox/project_commands.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/project_item/__init__.py` & `spinetoolbox-0.6.9/spinetoolbox/project_item/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/project_item/logging_connection.py` & `spinetoolbox-0.6.9/spinetoolbox/project_item/logging_connection.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/project_item/project_item.py` & `spinetoolbox-0.6.9/spinetoolbox/project_item/project_item.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/project_item/project_item_factory.py` & `spinetoolbox-0.6.9/spinetoolbox/project_item/project_item_factory.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/project_item/specification_editor_window.py` & `spinetoolbox-0.6.9/spinetoolbox/project_item/specification_editor_window.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/project_item_icon.py` & `spinetoolbox-0.6.9/spinetoolbox/project_item_icon.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/project_upgrader.py` & `spinetoolbox-0.6.9/spinetoolbox/project_upgrader.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/resources_icons_rc.py` & `spinetoolbox-0.6.9/spinetoolbox/resources_icons_rc.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/resources_logos_rc.py` & `spinetoolbox-0.6.9/spinetoolbox/resources_logos_rc.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_commands.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_commands.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/__init__.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/graphics_items.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/graphics_items.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/main.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/main.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/__init__.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/alternative_scenario_item.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/alternative_scenario_item.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/alternative_scenario_model.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/alternative_scenario_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/colors.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/colors.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/compound_parameter_models.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/compound_parameter_models.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/empty_parameter_models.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/empty_parameter_models.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/entity_tree_item.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/entity_tree_item.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/entity_tree_models.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/entity_tree_models.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/frozen_table_model.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/frozen_table_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/item_metadata_table_model.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/item_metadata_table_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/metadata_table_model.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/metadata_table_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/metadata_table_model_base.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/metadata_table_model_base.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/multi_db_tree_item.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/multi_db_tree_item.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/multi_db_tree_model.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/multi_db_tree_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/parameter_mixins.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/parameter_mixins.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/parameter_value_list_item.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/parameter_value_list_item.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/parameter_value_list_model.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/parameter_value_list_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/pivot_model.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/pivot_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/pivot_table_models.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/pivot_table_models.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/single_parameter_models.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/single_parameter_models.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/tool_feature_item.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/tool_feature_item.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/tool_feature_model.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/tool_feature_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/tree_item_utility.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/tree_item_utility.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/mvcmodels/tree_model_base.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/mvcmodels/tree_model_base.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/scenario_generation.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/scenario_generation.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/ui/__init__.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/ui/scenario_generator.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/ui/scenario_generator.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/ui/spine_db_editor_window.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/ui/spine_db_editor_window.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/__init__.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/add_items_dialogs.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/add_items_dialogs.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/commit_viewer.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/commit_viewer.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/custom_delegates.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/custom_delegates.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/custom_menus.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/custom_menus.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/custom_qgraphicsviews.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/custom_qgraphicsviews.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/custom_qtableview.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/custom_qtableview.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/custom_qtreeview.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/custom_qtreeview.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/custom_qwidgets.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/custom_qwidgets.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/edit_or_remove_items_dialogs.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/edit_or_remove_items_dialogs.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/graph_layout_generator.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/graph_layout_generator.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/graph_view_mixin.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/graph_view_mixin.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/item_metadata_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/item_metadata_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/manage_items_dialogs.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/manage_items_dialogs.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/mass_select_items_dialogs.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/mass_select_items_dialogs.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/metadata_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/metadata_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/multi_spine_db_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/multi_spine_db_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/object_name_list_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/object_name_list_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/parameter_view_mixin.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/parameter_view_mixin.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/pivot_table_header_view.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/pivot_table_header_view.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/scenario_generator.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/scenario_generator.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/select_position_parameters_dialog.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/select_position_parameters_dialog.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/spine_db_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/spine_db_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/tabular_view_header_widget.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/tabular_view_header_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/tabular_view_mixin.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/tabular_view_mixin.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/tree_view_mixin.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/tree_view_mixin.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_editor/widgets/url_toolbar.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_editor/widgets/url_toolbar.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_icon_manager.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_icon_manager.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_manager.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_manager.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_parcel.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_parcel.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_signaller.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_signaller.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_db_worker.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_db_worker.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_engine_manager.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_engine_manager.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/spine_engine_worker.py` & `spinetoolbox-0.6.9/spinetoolbox/spine_engine_worker.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/__init__.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/about.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/about.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/add_project_item.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/add_project_item.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/array_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/array_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/datetime_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/datetime_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/duration_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/duration_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/import_source_selector.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/import_source_selector.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/jump_properties.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/jump_properties.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/kernel_editor_dialog.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/kernel_editor_dialog.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/link_properties.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/link_properties.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/mainwindow.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/map_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/map_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/mini_kernel_editor_dialog.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/mini_kernel_editor_dialog.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/open_project_dialog.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/open_project_dialog.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/parameter_value_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/parameter_value_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/plain_parameter_value_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/plain_parameter_value_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/resources/app.ico` & `spinetoolbox-0.6.9/spinetoolbox/ui/resources/app.ico`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/resources/cat.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/resources/cat.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/settings.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/settings.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/spine_datapackage_form.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/spine_datapackage_form.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/time_pattern_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/time_pattern_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/time_series_fixed_resolution_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/time_series_fixed_resolution_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/time_series_variable_resolution_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/time_series_variable_resolution_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui/tool_configuration_assistant.py` & `spinetoolbox-0.6.9/spinetoolbox/ui/tool_configuration_assistant.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/ui_main.py` & `spinetoolbox-0.6.9/spinetoolbox/ui_main.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/version.py` & `spinetoolbox-0.6.9/spinetoolbox/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,12 +38,12 @@
             return version + f".dev{self.serial}"
         else:
             return version + f"-{self.releaselevel}.{self.serial}"
 
 
 major = 0
 minor = 6
-micro = 8
+micro = 9
 releaselevel = "final"
 serial = 0
 __version_info__ = VersionInfo(major, minor, micro, releaselevel, serial)
 __version__ = str(__version_info__)
```

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/__init__.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/about_widget.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/about_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/add_project_item_widget.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/add_project_item_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/add_up_spine_opt_wizard.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/add_up_spine_opt_wizard.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/array_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/array_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/array_value_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/array_value_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/code_text_edit.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/code_text_edit.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/commit_dialog.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/commit_dialog.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/console_window.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/console_window.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/custom_combobox.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/custom_combobox.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/custom_delegates.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/custom_delegates.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/custom_editors.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/custom_editors.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/custom_menus.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/custom_menus.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/custom_qcombobox.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/custom_qcombobox.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/custom_qgraphicsscene.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/custom_qgraphicsscene.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/custom_qgraphicsviews.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/custom_qgraphicsviews.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/custom_qlineedits.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/custom_qlineedits.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/custom_qtableview.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/custom_qtableview.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/custom_qtextbrowser.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/custom_qtextbrowser.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/custom_qtreeview.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/custom_qtreeview.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/custom_qwidgets.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/custom_qwidgets.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/datetime_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/datetime_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/duration_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/duration_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/indexed_value_table_context_menu.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/indexed_value_table_context_menu.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/install_julia_wizard.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/install_julia_wizard.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/jump_properties_widget.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/jump_properties_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/jupyter_console_widget.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/jupyter_console_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/kernel_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/kernel_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/link_properties_widget.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/link_properties_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/map_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/map_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/map_value_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/map_value_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/multi_tab_spec_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/multi_tab_spec_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/multi_tab_window.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/multi_tab_window.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/notification.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/notification.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/open_project_widget.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/open_project_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/parameter_value_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/parameter_value_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/parameter_value_editor_base.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/parameter_value_editor_base.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/persistent_console_widget.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/persistent_console_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/plain_parameter_value_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/plain_parameter_value_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/plot_canvas.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/plot_canvas.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/plot_widget.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/plot_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/plugin_manager_widgets.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/plugin_manager_widgets.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/project_item_drag.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/project_item_drag.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/properties_widget.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/properties_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/rename_project_dialog.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/rename_project_dialog.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/report_plotting_failure.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/report_plotting_failure.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/settings_widget.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/settings_widget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/statusbars.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/statusbars.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/time_pattern_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/time_pattern_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/time_series_fixed_resolution_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/time_series_fixed_resolution_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/time_series_variable_resolution_editor.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/time_series_variable_resolution_editor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox/widgets/toolbars.py` & `spinetoolbox-0.6.9/spinetoolbox/widgets/toolbars.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/spinetoolbox.egg-info/PKG-INFO` & `spinetoolbox-0.6.9/spinetoolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinetoolbox
-Version: 0.6.8
+Version: 0.6.9
 Summary: An application to define, manage, and execute various energy system simulation models
 Home-page: https://github.com/Spine-project/Spine-Toolbox
 Author: Spine Project consortium
 Author-email: spine_info@vtt.fi
 License: LGPL-3.0-or-later
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `spinetoolbox-0.6.8/spinetoolbox.egg-info/SOURCES.txt` & `spinetoolbox-0.6.9/spinetoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/__init__.py` & `spinetoolbox-0.6.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/mock_helpers.py` & `spinetoolbox-0.6.9/tests/mock_helpers.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/mvcmodels/__init__.py` & `spinetoolbox-0.6.9/tests/mvcmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/mvcmodels/test_ArrayModel.py` & `spinetoolbox-0.6.9/tests/mvcmodels/test_ArrayModel.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/mvcmodels/test_FilterCheckboxList.py` & `spinetoolbox-0.6.9/tests/mvcmodels/test_FilterCheckboxList.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/mvcmodels/test_IndexedValueTableModel.py` & `spinetoolbox-0.6.9/tests/mvcmodels/test_IndexedValueTableModel.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/mvcmodels/test_MapModel.py` & `spinetoolbox-0.6.9/tests/mvcmodels/test_MapModel.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/mvcmodels/test_MinimalTableModel.py` & `spinetoolbox-0.6.9/tests/mvcmodels/test_MinimalTableModel.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/mvcmodels/test_ProjectItemModel.py` & `spinetoolbox-0.6.9/tests/mvcmodels/test_ProjectItemModel.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/mvcmodels/test_TimePatternModel.py` & `spinetoolbox-0.6.9/tests/mvcmodels/test_TimePatternModel.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/mvcmodels/test_TimeSeriesModelFixedResolution.py` & `spinetoolbox-0.6.9/tests/mvcmodels/test_TimeSeriesModelFixedResolution.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/mvcmodels/test_TimeSeriesModelVariableResolution.py` & `spinetoolbox-0.6.9/tests/mvcmodels/test_TimeSeriesModelVariableResolution.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/project_item/__init__.py` & `spinetoolbox-0.6.9/tests/project_item/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/project_item/test_ProjectItem.py` & `spinetoolbox-0.6.9/tests/project_item/test_ProjectItem.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/spine_db_editor/__init__.py` & `spinetoolbox-0.6.9/tests/spine_db_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/spine_db_editor/mvcmodels/__init__.py` & `spinetoolbox-0.6.9/tests/spine_db_editor/mvcmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/spine_db_editor/mvcmodels/test_PivotModel.py` & `spinetoolbox-0.6.9/tests/spine_db_editor/mvcmodels/test_PivotModel.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/spine_db_editor/mvcmodels/test_PivotTableModel.py` & `spinetoolbox-0.6.9/tests/spine_db_editor/mvcmodels/test_PivotTableModel.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/spine_db_editor/mvcmodels/test_alternative_scenario_model.py` & `spinetoolbox-0.6.9/tests/spine_db_editor/mvcmodels/test_alternative_scenario_model.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/spine_db_editor/mvcmodels/test_compound_parameter_models.py` & `spinetoolbox-0.6.9/tests/spine_db_editor/mvcmodels/test_compound_parameter_models.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/spine_db_editor/mvcmodels/test_emptyParameterModels.py` & `spinetoolbox-0.6.9/tests/spine_db_editor/mvcmodels/test_emptyParameterModels.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/spine_db_editor/test_graphics_items.py` & `spinetoolbox-0.6.9/tests/spine_db_editor/test_graphics_items.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/spine_db_editor/widgets/__init__.py` & `spinetoolbox-0.6.9/tests/spine_db_editor/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/spine_db_editor/widgets/test_SpineDBEditor.py` & `spinetoolbox-0.6.9/tests/spine_db_editor/widgets/test_SpineDBEditor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/spine_db_editor/widgets/test_SpineDBEditorAdd.py` & `spinetoolbox-0.6.9/tests/spine_db_editor/widgets/test_SpineDBEditorAdd.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/spine_db_editor/widgets/test_SpineDBEditorBase.py` & `spinetoolbox-0.6.9/tests/spine_db_editor/widgets/test_SpineDBEditorBase.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/spine_db_editor/widgets/test_SpineDBEditorFilter.py` & `spinetoolbox-0.6.9/tests/spine_db_editor/widgets/test_SpineDBEditorFilter.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/spine_db_editor/widgets/test_SpineDBEditorRemove.py` & `spinetoolbox-0.6.9/tests/spine_db_editor/widgets/test_SpineDBEditorRemove.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/spine_db_editor/widgets/test_SpineDBEditorUpdate.py` & `spinetoolbox-0.6.9/tests/spine_db_editor/widgets/test_SpineDBEditorUpdate.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/spine_db_editor/widgets/test_SpineDBEditorWithDBMapping.py` & `spinetoolbox-0.6.9/tests/spine_db_editor/widgets/test_SpineDBEditorWithDBMapping.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/spine_db_editor/widgets/test_addItemsDialog.py` & `spinetoolbox-0.6.9/tests/spine_db_editor/widgets/test_addItemsDialog.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/spine_db_editor/widgets/test_custom_qwidgets.py` & `spinetoolbox-0.6.9/tests/spine_db_editor/widgets/test_custom_qwidgets.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/test_ProjectUpgrader.py` & `spinetoolbox-0.6.9/tests/test_ProjectUpgrader.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/test_SpineDBManager.py` & `spinetoolbox-0.6.9/tests/test_SpineDBManager.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/test_helpers.py` & `spinetoolbox-0.6.9/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/test_load_project_items.py` & `spinetoolbox-0.6.9/tests/test_load_project_items.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/test_plotting.py` & `spinetoolbox-0.6.9/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/test_spineToolboxProject.py` & `spinetoolbox-0.6.9/tests/test_spineToolboxProject.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/test_toolboxUI.py` & `spinetoolbox-0.6.9/tests/test_toolboxUI.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/__init__.py` & `spinetoolbox-0.6.9/tests/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_AddProjectItemWidget.py` & `spinetoolbox-0.6.9/tests/widgets/test_AddProjectItemWidget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_AddUpSpineOptWizard.py` & `spinetoolbox-0.6.9/tests/widgets/test_AddUpSpineOptWizard.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_ArrayTableView.py` & `spinetoolbox-0.6.9/tests/widgets/test_ArrayTableView.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_CopyPasteTableView.py` & `spinetoolbox-0.6.9/tests/widgets/test_CopyPasteTableView.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_DatetimeEditor.py` & `spinetoolbox-0.6.9/tests/widgets/test_DatetimeEditor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_DurationEditor.py` & `spinetoolbox-0.6.9/tests/widgets/test_DurationEditor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_IndexedValueTableView.py` & `spinetoolbox-0.6.9/tests/widgets/test_IndexedValueTableView.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_InstallJuliaWizard.py` & `spinetoolbox-0.6.9/tests/widgets/test_InstallJuliaWizard.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_JupyterConsoleWidget.py` & `spinetoolbox-0.6.9/tests/widgets/test_JupyterConsoleWidget.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_MapEditor.py` & `spinetoolbox-0.6.9/tests/widgets/test_MapEditor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_MapTableView.py` & `spinetoolbox-0.6.9/tests/widgets/test_MapTableView.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_ParameterValueEditor.py` & `spinetoolbox-0.6.9/tests/widgets/test_ParameterValueEditor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_PlainParameterValueEditor.py` & `spinetoolbox-0.6.9/tests/widgets/test_PlainParameterValueEditor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_TimePatternEditor.py` & `spinetoolbox-0.6.9/tests/widgets/test_TimePatternEditor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_TimeSeriesFixedResolutionEditor.py` & `spinetoolbox-0.6.9/tests/widgets/test_TimeSeriesFixedResolutionEditor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_TimeSeriesFixedResolutionTableView.py` & `spinetoolbox-0.6.9/tests/widgets/test_TimeSeriesFixedResolutionTableView.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_TimeSeriesVariableResolutionEditor.py` & `spinetoolbox-0.6.9/tests/widgets/test_TimeSeriesVariableResolutionEditor.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_custom_editors.py` & `spinetoolbox-0.6.9/tests/widgets/test_custom_editors.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_custom_qtextbrowser.py` & `spinetoolbox-0.6.9/tests/widgets/test_custom_qtextbrowser.py`

 * *Files identical despite different names*

### Comparing `spinetoolbox-0.6.8/tests/widgets/test_indexed_value_table_context_menu.py` & `spinetoolbox-0.6.9/tests/widgets/test_indexed_value_table_context_menu.py`

 * *Files identical despite different names*

