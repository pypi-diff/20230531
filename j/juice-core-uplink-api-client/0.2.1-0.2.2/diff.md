# Comparing `tmp/juice_core_uplink_api_client-0.2.1.tar.gz` & `tmp/juice_core_uplink_api_client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juice_core_uplink_api_client-0.2.1.tar", max compression
+gzip compressed data, was "juice_core_uplink_api_client-0.2.2.tar", max compression
```

## Comparing `juice_core_uplink_api_client-0.2.1.tar` & `juice_core_uplink_api_client-0.2.2.tar`

### file list

```diff
@@ -1,104 +1,103 @@
--rw-r--r--   0        0        0     8876 2023-04-05 13:28:26.992686 juice_core_uplink_api_client-0.2.1/README.md
--rw-r--r--   0        0        0     6917 2023-04-05 13:43:27.929788 juice_core_uplink_api_client-0.2.1/juice_core/SHTRestInterface.py
--rw-r--r--   0        0        0      246 2022-11-28 08:37:35.932458 juice_core_uplink_api_client-0.2.1/juice_core/__init__.py
--rw-r--r--   0        0        0      165 2023-04-05 13:15:57.880718 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/__init__.py
--rw-r--r--   0        0        0       47 2023-04-05 13:15:58.034053 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 13:15:58.050720 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/api_token_auth/__init__.py
--rw-r--r--   0        0        0     3310 2023-04-05 13:15:59.557404 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/api_token_auth/api_token_auth_create.py
--rw-r--r--   0        0        0        0 2023-04-05 13:15:58.090721 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/api_token_refresh/__init__.py
--rw-r--r--   0        0        0     3844 2023-04-05 13:15:59.527404 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/api_token_refresh/api_token_refresh_create.py
--rw-r--r--   0        0        0        0 2023-04-05 13:15:58.090721 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/__init__.py
--rw-r--r--   0        0        0     1519 2023-04-05 13:15:59.497403 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_checks_list.py
--rw-r--r--   0        0        0     2068 2023-04-05 13:15:59.487403 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_checks_read.py
--rw-r--r--   0        0        0     2393 2023-04-05 13:15:59.514070 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_config_list.py
--rw-r--r--   0        0        0     3369 2023-04-05 13:15:59.537404 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_detailed_scenario_create.py
--rw-r--r--   0        0        0     2970 2023-04-05 13:15:59.530737 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_detailed_scenario_list.py
--rw-r--r--   0        0        0     3257 2023-04-05 13:15:59.550737 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_detailed_scenario_read.py
--rw-r--r--   0        0        0     1880 2023-04-05 13:28:26.996019 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_eps_package_create.py
--rw-r--r--   0        0        0     5092 2023-04-05 13:15:59.657405 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_events_list.py
--rw-r--r--   0        0        0     1782 2023-04-05 13:15:59.590738 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_file_read.py
--rw-r--r--   0        0        0     2326 2023-04-05 13:15:59.647405 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_mode_list.py
--rw-r--r--   0        0        0     2878 2023-04-05 13:15:59.634072 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_observation_definition_list.py
--rw-r--r--   0        0        0     3487 2023-04-05 13:15:59.660739 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_observation_definition_read.py
--rw-r--r--   0        0        0     3039 2023-04-05 13:28:26.996019 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_create.py
--rw-r--r--   0        0        0     2915 2023-04-05 13:15:59.737406 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_delete.py
--rw-r--r--   0        0        0     2816 2023-04-05 13:15:59.684072 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_list.py
--rw-r--r--   0        0        0     1925 2023-04-05 13:28:26.996019 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_ptr_create.py
--rw-r--r--   0        0        0     2163 2023-04-05 13:15:59.737406 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_ptr_list.py
--rw-r--r--   0        0        0     1940 2023-04-05 13:28:26.996019 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_ptr_skeleton_create.py
--rw-r--r--   0        0        0     1935 2023-04-05 13:28:26.996019 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_ptr_xml_create.py
--rw-r--r--   0        0        0     3141 2023-04-05 13:15:59.787407 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_read.py
--rw-r--r--   0        0        0     1996 2023-04-05 13:15:59.757407 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_simphony_groups_read.py
--rw-r--r--   0        0        0     6843 2023-04-05 13:15:59.920742 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_simphony_opps_read.py
--rw-r--r--   0        0        0     6793 2023-04-05 13:15:59.964076 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_simphony_read.py
--rw-r--r--   0        0        0     6891 2023-04-05 13:15:59.967409 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_simphony_timeline_read.py
--rw-r--r--   0        0        0     2995 2023-04-05 13:15:59.894075 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_stats_list.py
--rw-r--r--   0        0        0     3026 2023-04-05 13:15:59.897408 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_update.py
--rw-r--r--   0        0        0     3292 2023-04-05 13:15:59.924075 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_segment_definition_read.py
--rw-r--r--   0        0        0     5118 2023-04-05 13:15:59.944075 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_series_list.py
--rw-r--r--   0        0        0     1466 2023-04-05 13:15:59.884075 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_session_flush_list.py
--rw-r--r--   0        0        0     3746 2023-04-05 13:16:00.024076 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_detailed_scenario_list.py
--rw-r--r--   0        0        0     3756 2023-04-05 13:16:00.044077 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_engineering_segment_types_list.py
--rw-r--r--   0        0        0     3674 2023-04-05 13:16:00.074077 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_engineering_segments_list.py
--rw-r--r--   0        0        0     3725 2023-04-05 13:16:00.064077 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_event_list.py
--rw-r--r--   0        0        0     2736 2023-04-05 13:16:00.127411 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_list.py
--rw-r--r--   0        0        0     3472 2023-04-05 13:16:00.084077 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_plan_list.py
--rw-r--r--   0        0        0     2267 2023-04-05 13:16:00.070744 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_ptr_list.py
--rw-r--r--   0        0        0     3128 2023-04-05 13:16:00.094077 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_read.py
--rw-r--r--   0        0        0     3646 2023-04-05 13:16:00.160745 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_series_list.py
--rw-r--r--   0        0        0     3255 2023-04-05 13:16:00.190745 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_user_read.py
--rw-r--r--   0        0        0     2816 2023-04-05 13:16:00.184078 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_version_list.py
--rw-r--r--   0        0        0     3727 2023-04-05 13:16:00.214079 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/trajectory_segment_definitions.py
--rw-r--r--   0        0        0     1821 2023-04-05 13:16:00.160745 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/client.py
--rw-r--r--   0        0        0     3404 2023-04-05 13:15:58.030720 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/__init__.py
--rw-r--r--   0        0        0     1379 2023-04-05 13:16:00.180745 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/api_version.py
--rw-r--r--   0        0        0     9152 2023-04-05 13:16:00.457415 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/configuration.py
--rw-r--r--   0        0        0     1566 2023-04-05 13:16:00.217412 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/configuration_item.py
--rw-r--r--   0        0        0     2511 2023-04-05 13:16:00.290746 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/data_profile.py
--rw-r--r--   0        0        0     3176 2023-04-05 13:16:00.317413 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/detailed_scenario.py
--rw-r--r--   0        0        0     4050 2023-04-05 13:16:00.387414 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/detailed_scenario_list.py
--rw-r--r--   0        0        0     2476 2023-04-05 13:16:00.304080 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/engineering_segment.py
--rw-r--r--   0        0        0     2197 2023-04-05 13:16:00.297413 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/engineering_segment_type.py
--rw-r--r--   0        0        0     2433 2023-04-05 13:16:00.347413 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/event.py
--rw-r--r--   0        0        0     1877 2023-04-05 13:16:00.344080 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/instrument_membership.py
--rw-r--r--   0        0        0      165 2023-04-05 13:15:59.097399 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/instrument_membership_type.py
--rw-r--r--   0        0        0     2264 2023-04-05 13:16:00.404081 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/instrument_resource_profile.py
--rw-r--r--   0        0        0     2075 2023-04-05 13:16:00.407414 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/instrument_type.py
--rw-r--r--   0        0        0     1584 2023-04-05 13:16:00.380747 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/json_web_token.py
--rw-r--r--   0        0        0     3416 2023-04-05 13:16:00.560749 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/mode.py
--rw-r--r--   0        0        0     6628 2023-04-05 13:16:00.720751 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/observation_definition.py
--rw-r--r--   0        0        0     9265 2023-04-05 13:16:00.734084 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/observation_definition_extend.py
--rw-r--r--   0        0        0     2816 2023-04-05 13:16:00.544082 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/phase.py
--rw-r--r--   0        0        0     4960 2023-04-05 13:16:00.597416 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/plan.py
--rw-r--r--   0        0        0     3890 2023-04-05 13:16:00.624083 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/plan_list.py
--rw-r--r--   0        0        0     2532 2023-04-05 13:16:00.537416 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/plan_stats.py
--rw-r--r--   0        0        0     1740 2023-04-05 13:16:00.550749 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/platform_power_profile.py
--rw-r--r--   0        0        0     2472 2023-04-05 13:16:00.684084 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/power_profile.py
--rw-r--r--   0        0        0     2552 2023-04-05 13:16:00.667417 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/read_only_instrument_resource_profile.py
--rw-r--r--   0        0        0     4723 2023-04-05 13:16:00.750751 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/read_only_plan.py
--rw-r--r--   0        0        0     2554 2023-04-05 13:16:00.680751 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/read_only_resource_profile.py
--rw-r--r--   0        0        0     3899 2023-04-05 13:28:26.996019 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/read_only_segment_group.py
--rw-r--r--   0        0        0     1410 2023-04-05 13:16:00.697417 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/refresh_json_web_token.py
--rw-r--r--   0        0        0     1793 2023-04-05 13:16:00.760752 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/resource_category.py
--rw-r--r--   0        0        0     2261 2023-04-05 13:16:00.797419 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/resource_profile.py
--rw-r--r--   0        0        0      176 2023-04-05 13:15:59.150733 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/rest_api_plan_simphony_opps_read_mode.py
--rw-r--r--   0        0        0      172 2023-04-05 13:15:59.110732 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/rest_api_plan_simphony_read_mode.py
--rw-r--r--   0        0        0      180 2023-04-05 13:15:59.097399 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/rest_api_plan_simphony_timeline_read_mode.py
--rw-r--r--   0        0        0     8108 2023-04-05 13:16:01.000754 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/segment.py
--rw-r--r--   0        0        0     7666 2023-04-05 13:28:26.996019 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/segment_definition.py
--rw-r--r--   0        0        0     4488 2023-04-05 13:16:00.920753 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/segment_group.py
--rw-r--r--   0        0        0     1709 2023-04-05 13:16:00.827419 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/series_data.py
--rw-r--r--   0        0        0     2416 2023-04-05 13:16:00.877420 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/series_definition.py
--rw-r--r--   0        0        0     5547 2023-04-05 13:16:00.960754 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/simphony_plan.py
--rw-r--r--   0        0        0     1678 2023-04-05 13:16:00.850752 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/spice_kernel.py
--rw-r--r--   0        0        0     3258 2023-04-05 13:16:00.950754 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/trajectory.py
--rw-r--r--   0        0        0     2137 2023-04-05 13:16:00.934087 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/trajectory_list.py
--rw-r--r--   0        0        0     1962 2023-04-05 13:28:26.996019 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/unit.py
--rw-r--r--   0        0        0     4162 2023-04-05 13:16:01.020754 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/user.py
--rw-r--r--   0        0        0     1934 2023-04-05 13:16:01.007421 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/working_group_membership.py
--rw-r--r--   0        0        0      175 2023-04-05 13:15:59.080732 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/working_group_membership_type.py
--rw-r--r--   0        0        0       25 2023-04-05 13:15:57.880718 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/py.typed
--rw-r--r--   0        0        0      974 2023-04-05 13:16:00.984087 juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/types.py
--rw-r--r--   0        0        0      862 2023-04-05 13:44:33.913882 juice_core_uplink_api_client-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    10078 1970-01-01 00:00:00.000000 juice_core_uplink_api_client-0.2.1/setup.py
--rw-r--r--   0        0        0     9532 1970-01-01 00:00:00.000000 juice_core_uplink_api_client-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     8876 2023-04-05 13:28:26.992686 juice_core_uplink_api_client-0.2.2/README.md
+-rw-r--r--   0        0        0     7963 2023-05-25 11:56:20.797517 juice_core_uplink_api_client-0.2.2/juice_core/SHTRestInterface.py
+-rw-r--r--   0        0        0      362 2023-05-25 11:56:04.200669 juice_core_uplink_api_client-0.2.2/juice_core/__init__.py
+-rw-r--r--   0        0        0      165 2023-04-05 13:15:57.880718 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-05 13:15:58.034053 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-05 13:15:58.050720 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/api_token_auth/__init__.py
+-rw-r--r--   0        0        0     3310 2023-04-05 13:15:59.557404 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/api_token_auth/api_token_auth_create.py
+-rw-r--r--   0        0        0        0 2023-04-05 13:15:58.090721 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/api_token_refresh/__init__.py
+-rw-r--r--   0        0        0     3844 2023-04-05 13:15:59.527404 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/api_token_refresh/api_token_refresh_create.py
+-rw-r--r--   0        0        0        0 2023-04-05 13:15:58.090721 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/__init__.py
+-rw-r--r--   0        0        0     1519 2023-04-05 13:15:59.497403 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_checks_list.py
+-rw-r--r--   0        0        0     2068 2023-04-05 13:15:59.487403 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_checks_read.py
+-rw-r--r--   0        0        0     2393 2023-04-05 13:15:59.514070 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_config_list.py
+-rw-r--r--   0        0        0     3369 2023-04-05 13:15:59.537404 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_detailed_scenario_create.py
+-rw-r--r--   0        0        0     2970 2023-04-05 13:15:59.530737 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_detailed_scenario_list.py
+-rw-r--r--   0        0        0     3257 2023-04-05 13:15:59.550737 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_detailed_scenario_read.py
+-rw-r--r--   0        0        0     1880 2023-04-05 13:28:26.996019 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_eps_package_create.py
+-rw-r--r--   0        0        0     5092 2023-04-05 13:15:59.657405 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_events_list.py
+-rw-r--r--   0        0        0     1782 2023-04-05 13:15:59.590738 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_file_read.py
+-rw-r--r--   0        0        0     2326 2023-04-05 13:15:59.647405 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_mode_list.py
+-rw-r--r--   0        0        0     2878 2023-04-05 13:15:59.634072 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_observation_definition_list.py
+-rw-r--r--   0        0        0     3487 2023-04-05 13:15:59.660739 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_observation_definition_read.py
+-rw-r--r--   0        0        0     3039 2023-04-05 13:28:26.996019 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_create.py
+-rw-r--r--   0        0        0     2915 2023-04-05 13:15:59.737406 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_delete.py
+-rw-r--r--   0        0        0     2816 2023-04-05 13:15:59.684072 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_list.py
+-rw-r--r--   0        0        0     1925 2023-04-05 13:28:26.996019 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_ptr_create.py
+-rw-r--r--   0        0        0     2163 2023-04-05 13:15:59.737406 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_ptr_list.py
+-rw-r--r--   0        0        0     1940 2023-04-05 13:28:26.996019 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_ptr_skeleton_create.py
+-rw-r--r--   0        0        0     1935 2023-04-05 13:28:26.996019 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_ptr_xml_create.py
+-rw-r--r--   0        0        0     3141 2023-04-05 13:15:59.787407 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_read.py
+-rw-r--r--   0        0        0     1996 2023-04-05 13:15:59.757407 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_simphony_groups_read.py
+-rw-r--r--   0        0        0     6843 2023-04-05 13:15:59.920742 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_simphony_opps_read.py
+-rw-r--r--   0        0        0     6793 2023-04-05 13:15:59.964076 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_simphony_read.py
+-rw-r--r--   0        0        0     6891 2023-04-05 13:15:59.967409 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_simphony_timeline_read.py
+-rw-r--r--   0        0        0     2995 2023-04-05 13:15:59.894075 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_stats_list.py
+-rw-r--r--   0        0        0     3026 2023-04-05 13:15:59.897408 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_update.py
+-rw-r--r--   0        0        0     3292 2023-04-05 13:15:59.924075 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_segment_definition_read.py
+-rw-r--r--   0        0        0     5118 2023-04-05 13:15:59.944075 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_series_list.py
+-rw-r--r--   0        0        0     1466 2023-04-05 13:15:59.884075 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_session_flush_list.py
+-rw-r--r--   0        0        0     3746 2023-04-05 13:16:00.024076 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_detailed_scenario_list.py
+-rw-r--r--   0        0        0     3756 2023-04-05 13:16:00.044077 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_engineering_segment_types_list.py
+-rw-r--r--   0        0        0     3674 2023-04-05 13:16:00.074077 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_engineering_segments_list.py
+-rw-r--r--   0        0        0     3725 2023-04-05 13:16:00.064077 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_event_list.py
+-rw-r--r--   0        0        0     2736 2023-04-05 13:16:00.127411 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_list.py
+-rw-r--r--   0        0        0     3472 2023-04-05 13:16:00.084077 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_plan_list.py
+-rw-r--r--   0        0        0     2267 2023-04-05 13:16:00.070744 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_ptr_list.py
+-rw-r--r--   0        0        0     3128 2023-04-05 13:16:00.094077 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_read.py
+-rw-r--r--   0        0        0     3646 2023-04-05 13:16:00.160745 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_series_list.py
+-rw-r--r--   0        0        0     3255 2023-04-05 13:16:00.190745 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_user_read.py
+-rw-r--r--   0        0        0     2816 2023-04-05 13:16:00.184078 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_version_list.py
+-rw-r--r--   0        0        0     3727 2023-04-05 13:16:00.214079 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/trajectory_segment_definitions.py
+-rw-r--r--   0        0        0     1821 2023-04-05 13:16:00.160745 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/client.py
+-rw-r--r--   0        0        0     3404 2023-04-05 13:15:58.030720 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/__init__.py
+-rw-r--r--   0        0        0     1379 2023-04-05 13:16:00.180745 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/api_version.py
+-rw-r--r--   0        0        0     9152 2023-04-05 13:16:00.457415 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/configuration.py
+-rw-r--r--   0        0        0     1566 2023-04-05 13:16:00.217412 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/configuration_item.py
+-rw-r--r--   0        0        0     2511 2023-04-05 13:16:00.290746 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/data_profile.py
+-rw-r--r--   0        0        0     3176 2023-04-05 13:16:00.317413 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/detailed_scenario.py
+-rw-r--r--   0        0        0     4050 2023-04-05 13:16:00.387414 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/detailed_scenario_list.py
+-rw-r--r--   0        0        0     2476 2023-04-05 13:16:00.304080 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/engineering_segment.py
+-rw-r--r--   0        0        0     2197 2023-04-05 13:16:00.297413 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/engineering_segment_type.py
+-rw-r--r--   0        0        0     2433 2023-04-05 13:16:00.347413 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/event.py
+-rw-r--r--   0        0        0     1877 2023-04-05 13:16:00.344080 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/instrument_membership.py
+-rw-r--r--   0        0        0      165 2023-04-05 13:15:59.097399 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/instrument_membership_type.py
+-rw-r--r--   0        0        0     2264 2023-04-05 13:16:00.404081 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/instrument_resource_profile.py
+-rw-r--r--   0        0        0     2075 2023-04-05 13:16:00.407414 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/instrument_type.py
+-rw-r--r--   0        0        0     1584 2023-04-05 13:16:00.380747 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/json_web_token.py
+-rw-r--r--   0        0        0     3416 2023-04-05 13:16:00.560749 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/mode.py
+-rw-r--r--   0        0        0     6628 2023-04-05 13:16:00.720751 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/observation_definition.py
+-rw-r--r--   0        0        0     9265 2023-04-05 13:16:00.734084 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/observation_definition_extend.py
+-rw-r--r--   0        0        0     2816 2023-04-05 13:16:00.544082 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/phase.py
+-rw-r--r--   0        0        0     4960 2023-04-05 13:16:00.597416 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/plan.py
+-rw-r--r--   0        0        0     3890 2023-04-05 13:16:00.624083 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/plan_list.py
+-rw-r--r--   0        0        0     2532 2023-04-05 13:16:00.537416 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/plan_stats.py
+-rw-r--r--   0        0        0     1740 2023-04-05 13:16:00.550749 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/platform_power_profile.py
+-rw-r--r--   0        0        0     2472 2023-04-05 13:16:00.684084 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/power_profile.py
+-rw-r--r--   0        0        0     2552 2023-04-05 13:16:00.667417 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/read_only_instrument_resource_profile.py
+-rw-r--r--   0        0        0     4723 2023-04-05 13:16:00.750751 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/read_only_plan.py
+-rw-r--r--   0        0        0     2554 2023-04-05 13:16:00.680751 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/read_only_resource_profile.py
+-rw-r--r--   0        0        0     3899 2023-04-05 13:28:26.996019 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/read_only_segment_group.py
+-rw-r--r--   0        0        0     1410 2023-04-05 13:16:00.697417 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/refresh_json_web_token.py
+-rw-r--r--   0        0        0     1793 2023-04-05 13:16:00.760752 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/resource_category.py
+-rw-r--r--   0        0        0     2261 2023-04-05 13:16:00.797419 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/resource_profile.py
+-rw-r--r--   0        0        0      176 2023-04-05 13:15:59.150733 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/rest_api_plan_simphony_opps_read_mode.py
+-rw-r--r--   0        0        0      172 2023-04-05 13:15:59.110732 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/rest_api_plan_simphony_read_mode.py
+-rw-r--r--   0        0        0      180 2023-04-05 13:15:59.097399 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/rest_api_plan_simphony_timeline_read_mode.py
+-rw-r--r--   0        0        0     8108 2023-04-05 13:16:01.000754 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/segment.py
+-rw-r--r--   0        0        0     7666 2023-04-05 13:28:26.996019 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/segment_definition.py
+-rw-r--r--   0        0        0     4488 2023-04-05 13:16:00.920753 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/segment_group.py
+-rw-r--r--   0        0        0     1709 2023-04-05 13:16:00.827419 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/series_data.py
+-rw-r--r--   0        0        0     2416 2023-04-05 13:16:00.877420 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/series_definition.py
+-rw-r--r--   0        0        0     5547 2023-04-05 13:16:00.960754 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/simphony_plan.py
+-rw-r--r--   0        0        0     1678 2023-04-05 13:16:00.850752 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/spice_kernel.py
+-rw-r--r--   0        0        0     3258 2023-04-05 13:16:00.950754 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/trajectory.py
+-rw-r--r--   0        0        0     2137 2023-04-05 13:16:00.934087 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/trajectory_list.py
+-rw-r--r--   0        0        0     1962 2023-04-05 13:28:26.996019 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/unit.py
+-rw-r--r--   0        0        0     4162 2023-04-05 13:16:01.020754 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/user.py
+-rw-r--r--   0        0        0     1934 2023-04-05 13:16:01.007421 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/working_group_membership.py
+-rw-r--r--   0        0        0      175 2023-04-05 13:15:59.080732 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/working_group_membership_type.py
+-rw-r--r--   0        0        0       25 2023-04-05 13:15:57.880718 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/py.typed
+-rw-r--r--   0        0        0      974 2023-04-05 13:16:00.984087 juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/types.py
+-rw-r--r--   0        0        0      865 2023-05-29 11:46:47.211425 juice_core_uplink_api_client-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     9511 1970-01-01 00:00:00.000000 juice_core_uplink_api_client-0.2.2/PKG-INFO
```

### Comparing `juice_core_uplink_api_client-0.2.1/README.md` & `juice_core_uplink_api_client-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core/SHTRestInterface.py` & `juice_core_uplink_api_client-0.2.2/juice_core/SHTRestInterface.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import json
 import logging
 from functools import cache, partial
-from typing import List, Union
+import re
+from typing import List, Union, Optional
 
 import pandas as pd
 from attrs import define
 from merge_args import merge_args  # also makefun has a decorator that does this
 
 from juice_core_uplink_api_client.api.rest_api import (
     rest_api_events_list,
@@ -24,23 +25,56 @@
 
 DEFAULT_START = "2020"
 DEFAULT_END = "2040"
 DEFAULT_TRAJECTORY = "CREMA_5_1_150lb_23_1"
 DEFAULT_URL = "https://juicesoc.esac.esa.int"
 
 
+def expand_description(tab: pd.DataFrame) -> pd.DataFrame:
+    """Some tables have a description column that contains additional information.
+
+    This function expands the description column into multiple columns.
+
+    Parameters
+    ----------
+    tab (pd.DataFrame): 
+        table to expand, must have a description column
+
+    Returns
+    -------
+    pd.DataFrame: 
+        a new dataframe with the description column expanded
+
+    """
+    additional_columns = []
+    for d in tab.description:
+        values = {}
+        for item in d.split(";"):
+            key, value = item.split("=")
+            values[key.strip()] = value.strip()
+
+        additional_columns.append(values)
+        
+    tab_ = tab.drop(columns=["description"], inplace=False)
+    newd = pd.DataFrame(additional_columns)
+    
+    return tab_.join(newd)
+
 def convert_times(table, columns=[]):
     if isinstance(columns, str):
         columns = [columns]
 
     if len(columns) == 0 or columns is None:
         return table
 
     for col in columns:
-        table[col] = pd.to_datetime(table[col]).dt.tz_localize(None)
+        try:
+            table[col] = pd.to_datetime(table[col]).dt.tz_localize(None)
+        except Exception:
+            log.warning(f"Could not convert column {col} to datetime. Maybe is a point event?")
 
     return table
 
 
 def table_to_timeseries(table, name=None):
     return pd.Series(data=table.value.values, index=table.epoch.values, name=name)
 
@@ -60,14 +94,15 @@
             time_fields_ += ["epoch"]
             if "series_name" in kwargs:
                 series_name = kwargs["series_name"]
             else:
                 series_name = args[1]
 
         result = func(*args, **kwargs)  # call actual function
+        log.debug("Got result from API:\n%s", result)
 
         # convert to pandas if needed
         if as_pandas:
             table = convert_times(
                 pd.DataFrame([d.to_dict() if hasattr(d, "to_dict") else d for d in result]), columns=time_fields_
             )
 
@@ -97,15 +132,15 @@
 
 @define(auto_attribs=True, eq=False)
 class SHTRestInterface:
     """
     Main entry point for interacting with the Juice Core Uplink API
     """
 
-    client: [None, Client] = None
+    client: Optional[Client] = None
     timeout: float = 40.0
 
     def __attrs_post_init__(self):
         if not self.client:
             self.client = Client(DEFAULT_URL)
         self.client.timeout = self.timeout
```

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/api_token_auth/api_token_auth_create.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/api_token_auth/api_token_auth_create.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/api_token_refresh/api_token_refresh_create.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/api_token_refresh/api_token_refresh_create.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_checks_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_checks_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_checks_read.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_checks_read.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_config_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_config_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_detailed_scenario_create.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_detailed_scenario_create.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_detailed_scenario_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_detailed_scenario_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_detailed_scenario_read.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_detailed_scenario_read.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_eps_package_create.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_eps_package_create.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_events_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_events_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_file_read.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_file_read.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_mode_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_mode_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_observation_definition_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_observation_definition_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_observation_definition_read.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_observation_definition_read.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_create.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_create.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_delete.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_delete.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_ptr_create.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_ptr_create.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_ptr_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_ptr_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_ptr_skeleton_create.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_ptr_skeleton_create.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_ptr_xml_create.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_ptr_xml_create.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_read.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_read.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_simphony_groups_read.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_simphony_groups_read.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_simphony_opps_read.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_simphony_opps_read.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_simphony_read.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_simphony_read.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_simphony_timeline_read.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_simphony_timeline_read.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_stats_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_stats_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_plan_update.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_plan_update.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_segment_definition_read.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_segment_definition_read.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_series_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_series_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_session_flush_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_session_flush_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_detailed_scenario_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_detailed_scenario_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_engineering_segment_types_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_engineering_segment_types_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_engineering_segments_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_engineering_segments_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_event_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_event_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_plan_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_plan_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_ptr_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_ptr_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_read.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_read.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_series_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_trajectory_series_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_user_read.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_user_read.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/rest_api_version_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/rest_api_version_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/api/rest_api/trajectory_segment_definitions.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/api/rest_api/trajectory_segment_definitions.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/client.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/client.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/__init__.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/api_version.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/api_version.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/configuration.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/configuration.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/configuration_item.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/configuration_item.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/data_profile.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/data_profile.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/detailed_scenario.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/detailed_scenario.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/detailed_scenario_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/detailed_scenario_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/engineering_segment.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/engineering_segment.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/engineering_segment_type.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/engineering_segment_type.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/event.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/event.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/instrument_membership.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/instrument_membership.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/instrument_resource_profile.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/instrument_resource_profile.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/instrument_type.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/instrument_type.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/json_web_token.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/json_web_token.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/mode.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/mode.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/observation_definition.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/observation_definition.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/observation_definition_extend.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/observation_definition_extend.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/phase.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/phase.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/plan.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/plan.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/plan_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/plan_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/plan_stats.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/plan_stats.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/platform_power_profile.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/platform_power_profile.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/power_profile.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/power_profile.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/read_only_instrument_resource_profile.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/read_only_instrument_resource_profile.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/read_only_plan.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/read_only_plan.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/read_only_resource_profile.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/read_only_resource_profile.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/read_only_segment_group.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/read_only_segment_group.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/refresh_json_web_token.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/refresh_json_web_token.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/resource_category.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/resource_category.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/resource_profile.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/resource_profile.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/segment.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/segment.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/segment_definition.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/segment_definition.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/segment_group.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/segment_group.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/series_data.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/series_data.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/series_definition.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/series_definition.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/simphony_plan.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/simphony_plan.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/spice_kernel.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/spice_kernel.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/trajectory.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/trajectory.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/trajectory_list.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/trajectory_list.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/unit.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/unit.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/user.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/user.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/models/working_group_membership.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/models/working_group_membership.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/juice_core_uplink_api_client/types.py` & `juice_core_uplink_api_client-0.2.2/juice_core_uplink_api_client/types.py`

 * *Files identical despite different names*

### Comparing `juice_core_uplink_api_client-0.2.1/pyproject.toml` & `juice_core_uplink_api_client-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # small change
 [tool.poetry]
 name = "juice-core-uplink-api-client"
-version = "0.2.1"
+version = "0.2.2"
 description = "A client library for accessing Juice Core Uplink API"
 
 authors = []
 
 readme = "README.md"
 packages = [
     {include = "juice_core_uplink_api_client"},
@@ -13,17 +13,17 @@
 ]
 include = ["CHANGELOG.md", "juice_core_uplink_api_client/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0" 
 httpx = ">=0.15.4,<0.24.0"
 attrs = ">=21.3.0"
-python-dateutil = "^2.8.0"
-pandas = "^1.5.2"
-merge-args = "^0.1.5"
+python-dateutil = ">=2.8.0"
+pandas = ">=1.5.2"
+merge-args = ">=0.1.5"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `juice_core_uplink_api_client-0.2.1/setup.py` & `juice_core_uplink_api_client-0.2.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,207 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: juice-core-uplink-api-client
+Version: 0.2.2
+Summary: A client library for accessing Juice Core Uplink API
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: attrs (>=21.3.0)
+Requires-Dist: httpx (>=0.15.4,<0.24.0)
+Requires-Dist: merge-args (>=0.1.5)
+Requires-Dist: pandas (>=1.5.2)
+Requires-Dist: python-dateutil (>=2.8.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['juice_core',
- 'juice_core_uplink_api_client',
- 'juice_core_uplink_api_client.api',
- 'juice_core_uplink_api_client.api.api_token_auth',
- 'juice_core_uplink_api_client.api.api_token_refresh',
- 'juice_core_uplink_api_client.api.rest_api',
- 'juice_core_uplink_api_client.models']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['attrs>=21.3.0',
- 'httpx>=0.15.4,<0.24.0',
- 'merge-args>=0.1.5,<0.2.0',
- 'pandas>=1.5.2,<2.0.0',
- 'python-dateutil>=2.8.0,<3.0.0']
-
-setup_kwargs = {
-    'name': 'juice-core-uplink-api-client',
-    'version': '0.2.1',
-    'description': 'A client library for accessing Juice Core Uplink API',
-    'long_description': '# SHT Rest Interface\n\nIt is made by two modules to interact with the Juice Core Uplink \nAPI.\n\n## Install\n\nThe module is now contributed to PyPI, just call\n\n```bash\npip install juice_core_uplink_api_client\n```\n\nto install the module. If you use poetry to build your package and you want to add it as a dependency use:\n\n```bash\npoetry add juice_core_uplink_api_client\n```\n\nif you need to test development version (the main branch in this repository):\n\n```bash\npip install "git+https://www.ict.inaf.it/gitlab/juice-janus/sht_rest_interface.git#egg=juice-core-uplink-api-client&subdirectory=juice-core-uplink-api-client"\n```\n\n## juice-core-uplink-api-client\n\nThis module is automatically generated using the command below. It must not be \nmodified manually.\n\n```bash \n openapi-python-client update --path openapi.json \n```\n\nor just using the makefile `make` shortcut. The command is expected to be runt \nfrom the root of the repository (where the makefile is located) and requires \n`openapi-python-client` to be installed in the host system.\n\nThe module is generated from the openapi definition available at \nhttps://juicesoc.esac.esa.int/docs/, but **notice** that the openapi.json definition is a modified version of the one \navailable at that link. The file was modified by:\n\n- updating the file to openapi 3.1\n- making several changes to fix inconsistencies in the definition\n\nThe original files are mantained here for simplicity:\n\n1. `openapi_source.json` -> as downloaded from [swagger](https://juicesoc.esac.esa.int/docs/)\n2. `openapi_converted.json` -> updated to version 3.x using [https://converter.swagger.io/#/Converter/convertByUrl](swagger converter service)\n3. `openapi.json` -> used to generate the module with openapi-python-client\n\nAlso note that only some issues were corrected in the openapi.json file,\nhence the generated module is not complete, and it is not granted to work.\nIf you find any additional inconsistency, please report it to the repo issue \ntracker.\n\n\n## juice_core \n\nthis module is a wrapper around the automatically generated module. It is made \nby a class with several methods to interact with the API. It is just a stub to \nstart disucssing the API interface. It is not complete and it is not guaranteed \nto work.\n\n## Usage example\n\nFirst, create a client:\n\n```python\nfrom juice_core import SHTRestInterface\ni = SHTRestInterface()\n```\n\nand access the list of available plans on the server:\n\n```python\ni.plans()\n```\n\nwill output a pandas dataframe with the list of plans (just some here):\n\n|    | trajectory   | name                       | mnemonic                   | is_public   | created                    |   id | author   | description                                                                                                                                                           | refine_log   | ptr_file                                                                |\n|---:|:-------------|:---------------------------|:---------------------------|:------------|:---------------------------|-----:|:---------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------|:------------------------------------------------------------------------|\n|  0 | CREMA_3_0    | CASE4                      | CASE4                      | True        | 2021-03-04 13:29:58.835199 |   17 | rlorente | Demonstration Case 4                                                                                                                                                  |              |                                                                         |\n|  1 | CREMA_5_0    | CREMA_5_0_OPPORTUNITIES_v0 | CREMA_5_0_OPPORTUNITIES_v0 | True        | 2021-08-26 09:12:06.767139 |   31 | cvallat  | 1st run opf opportunities generation (UC22), based on existing definitions of oppportunities (inherited from crema 3_0)                                               |              | https://juicesoc.esac.esa.int/rest_api/file/trajectory%23CREMA_5_0.ptx/ |\n|  2 | CREMA_5_0    | CREMA_5_0_OPPORTUNITIES_v1 | CREMA_5_0_OPPORTUNITIES_v1 | True        | 2021-10-04 13:49:49.262682 |   36 | cvallat  | Added two opportunities for JMAG_CALROL for the last 2 perijoves before JOI (PJ69 not considered since too clsoe to GoI for observations to take place --> MPAD rule) |              | https://juicesoc.esac.esa.int/rest_api/file/trajectory%23CREMA_5_0.ptx/ |\n|  3 | CREMA_5_0    | CREMA_5_0_OPPORTUNITIES_v2 | CREMA_5_0_OPPORTUNITIES_v2 | True        | 2021-10-05 07:24:07.742653 |   37 | cvallat  | Modified GANYMEDE_GM opportunity around 3G3 for WG3 prime allocation (1 hour centered at CA)                                                                          |              | https://juicesoc.esac.esa.int/rest_api/file/trajectory%23CREMA_5_0.ptx/ |\n\n\nYou can also directly interact with the underalying `juice-core-uplink-api-client` module:\n\n\n### juice-core-uplink-api-client\n\nA client library for accessing Juice Core Uplink API\n\ndocs at https://juicesoc.esac.esa.int/docs/\n\nbrowsable at https://juicesoc.esac.esa.int/readonly_admin/core/\n\n## Usage\n\nFirst, create a client:\n\n```python\nfrom juice_core_uplink_api_client import Client\n\nclient = Client(base_url="https://api.example.com")\n```\n\nIf the endpoints you\'re going to hit require authentication, use `AuthenticatedClient` instead:\n\n```python\nfrom juice_core_uplink_api_client import AuthenticatedClient\n\nclient = AuthenticatedClient(base_url="https://api.example.com", token="SuperSecretToken")\n```\n\nNow call your endpoint and use your models:\n\n```python\nfrom juice_core_uplink_api_client.models import MyDataModel\nfrom juice_core_uplink_api_client.api.my_tag import get_my_data_model\nfrom juice_core_uplink_api_client.types import Response\n\nmy_data: MyDataModel = get_my_data_model.sync(client=client)\n# or if you need more info (e.g. status_code)\nresponse: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)\n```\n\nOr do the same thing with an async version:\n\n```python\nfrom juice_core_uplink_api_client.models import MyDataModel\nfrom juice_core_uplink_api_client.api.my_tag import get_my_data_model\nfrom juice_core_uplink_api_client.types import Response\n\nmy_data: MyDataModel = await get_my_data_model.asyncio(client=client)\nresponse: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)\n```\n\nBy default, when you\'re calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken",\n    verify_ssl="/path/to/certificate_bundle.pem",\n)\n```\n\nYou can also disable certificate validation altogether, but beware that **this is a security risk**.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken", \n    verify_ssl=False\n)\n```\n\nThings to know:\n1. Every path/method combo becomes a Python module with four functions:\n\n    1. `sync`: Blocking request that returns parsed data (if successful) or `None`\n    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.\n    1. `asyncio`: Like `sync` but async instead of blocking\n    1. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking\n\n1. All path/query params, and bodies become method arguments.\n1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)\n1. Any endpoint which did not have a tag will be in `juice_core_uplink_api_client.api.default`\n\n## Building / publishing this Client\n\nThis project uses [Poetry](https://python-poetry.org/) to manage dependencies  and packaging.  Here are the basics:\n\n1. Update the metadata in pyproject.toml (e.g. authors, version)\n1. If you\'re using a private repository, configure it with Poetry\n    1. `poetry config repositories.<your-repository-name> <url-to-your-repository>`\n    1. `poetry config http-basic.<your-repository-name> <username> <password>`\n1. Publish the client with `poetry publish --build -r <your-repository-name>` or, if for public PyPI, just `poetry publish --build`\n\nIf you want to install this client into another project without publishing it (e.g. for development) then:\n\n1. If that project **is using Poetry**, you can simply do `poetry add <path-to-this-client>` from that project\n1. If that project is not using Poetry:\n    1. Build a wheel with `poetry build -f wheel`\n    1. Install that wheel from the other project `pip install <path-to-wheel>`\n',
-    'author': 'None',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+# SHT Rest Interface
 
+It is made by two modules to interact with the Juice Core Uplink 
+API.
+
+## Install
+
+The module is now contributed to PyPI, just call
+
+```bash
+pip install juice_core_uplink_api_client
+```
+
+to install the module. If you use poetry to build your package and you want to add it as a dependency use:
+
+```bash
+poetry add juice_core_uplink_api_client
+```
+
+if you need to test development version (the main branch in this repository):
+
+```bash
+pip install "git+https://www.ict.inaf.it/gitlab/juice-janus/sht_rest_interface.git#egg=juice-core-uplink-api-client&subdirectory=juice-core-uplink-api-client"
+```
+
+## juice-core-uplink-api-client
+
+This module is automatically generated using the command below. It must not be 
+modified manually.
+
+```bash 
+ openapi-python-client update --path openapi.json 
+```
+
+or just using the makefile `make` shortcut. The command is expected to be runt 
+from the root of the repository (where the makefile is located) and requires 
+`openapi-python-client` to be installed in the host system.
+
+The module is generated from the openapi definition available at 
+https://juicesoc.esac.esa.int/docs/, but **notice** that the openapi.json definition is a modified version of the one 
+available at that link. The file was modified by:
+
+- updating the file to openapi 3.1
+- making several changes to fix inconsistencies in the definition
+
+The original files are mantained here for simplicity:
+
+1. `openapi_source.json` -> as downloaded from [swagger](https://juicesoc.esac.esa.int/docs/)
+2. `openapi_converted.json` -> updated to version 3.x using [https://converter.swagger.io/#/Converter/convertByUrl](swagger converter service)
+3. `openapi.json` -> used to generate the module with openapi-python-client
+
+Also note that only some issues were corrected in the openapi.json file,
+hence the generated module is not complete, and it is not granted to work.
+If you find any additional inconsistency, please report it to the repo issue 
+tracker.
+
+
+## juice_core 
+
+this module is a wrapper around the automatically generated module. It is made 
+by a class with several methods to interact with the API. It is just a stub to 
+start disucssing the API interface. It is not complete and it is not guaranteed 
+to work.
+
+## Usage example
+
+First, create a client:
+
+```python
+from juice_core import SHTRestInterface
+i = SHTRestInterface()
+```
+
+and access the list of available plans on the server:
+
+```python
+i.plans()
+```
+
+will output a pandas dataframe with the list of plans (just some here):
+
+|    | trajectory   | name                       | mnemonic                   | is_public   | created                    |   id | author   | description                                                                                                                                                           | refine_log   | ptr_file                                                                |
+|---:|:-------------|:---------------------------|:---------------------------|:------------|:---------------------------|-----:|:---------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------|:------------------------------------------------------------------------|
+|  0 | CREMA_3_0    | CASE4                      | CASE4                      | True        | 2021-03-04 13:29:58.835199 |   17 | rlorente | Demonstration Case 4                                                                                                                                                  |              |                                                                         |
+|  1 | CREMA_5_0    | CREMA_5_0_OPPORTUNITIES_v0 | CREMA_5_0_OPPORTUNITIES_v0 | True        | 2021-08-26 09:12:06.767139 |   31 | cvallat  | 1st run opf opportunities generation (UC22), based on existing definitions of oppportunities (inherited from crema 3_0)                                               |              | https://juicesoc.esac.esa.int/rest_api/file/trajectory%23CREMA_5_0.ptx/ |
+|  2 | CREMA_5_0    | CREMA_5_0_OPPORTUNITIES_v1 | CREMA_5_0_OPPORTUNITIES_v1 | True        | 2021-10-04 13:49:49.262682 |   36 | cvallat  | Added two opportunities for JMAG_CALROL for the last 2 perijoves before JOI (PJ69 not considered since too clsoe to GoI for observations to take place --> MPAD rule) |              | https://juicesoc.esac.esa.int/rest_api/file/trajectory%23CREMA_5_0.ptx/ |
+|  3 | CREMA_5_0    | CREMA_5_0_OPPORTUNITIES_v2 | CREMA_5_0_OPPORTUNITIES_v2 | True        | 2021-10-05 07:24:07.742653 |   37 | cvallat  | Modified GANYMEDE_GM opportunity around 3G3 for WG3 prime allocation (1 hour centered at CA)                                                                          |              | https://juicesoc.esac.esa.int/rest_api/file/trajectory%23CREMA_5_0.ptx/ |
+
+
+You can also directly interact with the underalying `juice-core-uplink-api-client` module:
+
+
+### juice-core-uplink-api-client
+
+A client library for accessing Juice Core Uplink API
+
+docs at https://juicesoc.esac.esa.int/docs/
+
+browsable at https://juicesoc.esac.esa.int/readonly_admin/core/
+
+## Usage
+
+First, create a client:
+
+```python
+from juice_core_uplink_api_client import Client
+
+client = Client(base_url="https://api.example.com")
+```
+
+If the endpoints you're going to hit require authentication, use `AuthenticatedClient` instead:
+
+```python
+from juice_core_uplink_api_client import AuthenticatedClient
+
+client = AuthenticatedClient(base_url="https://api.example.com", token="SuperSecretToken")
+```
+
+Now call your endpoint and use your models:
+
+```python
+from juice_core_uplink_api_client.models import MyDataModel
+from juice_core_uplink_api_client.api.my_tag import get_my_data_model
+from juice_core_uplink_api_client.types import Response
+
+my_data: MyDataModel = get_my_data_model.sync(client=client)
+# or if you need more info (e.g. status_code)
+response: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)
+```
+
+Or do the same thing with an async version:
+
+```python
+from juice_core_uplink_api_client.models import MyDataModel
+from juice_core_uplink_api_client.api.my_tag import get_my_data_model
+from juice_core_uplink_api_client.types import Response
+
+my_data: MyDataModel = await get_my_data_model.asyncio(client=client)
+response: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)
+```
+
+By default, when you're calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.
+
+```python
+client = AuthenticatedClient(
+    base_url="https://internal_api.example.com", 
+    token="SuperSecretToken",
+    verify_ssl="/path/to/certificate_bundle.pem",
+)
+```
+
+You can also disable certificate validation altogether, but beware that **this is a security risk**.
+
+```python
+client = AuthenticatedClient(
+    base_url="https://internal_api.example.com", 
+    token="SuperSecretToken", 
+    verify_ssl=False
+)
+```
+
+Things to know:
+1. Every path/method combo becomes a Python module with four functions:
+
+    1. `sync`: Blocking request that returns parsed data (if successful) or `None`
+    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.
+    1. `asyncio`: Like `sync` but async instead of blocking
+    1. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking
+
+1. All path/query params, and bodies become method arguments.
+1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)
+1. Any endpoint which did not have a tag will be in `juice_core_uplink_api_client.api.default`
+
+## Building / publishing this Client
+
+This project uses [Poetry](https://python-poetry.org/) to manage dependencies  and packaging.  Here are the basics:
+
+1. Update the metadata in pyproject.toml (e.g. authors, version)
+1. If you're using a private repository, configure it with Poetry
+    1. `poetry config repositories.<your-repository-name> <url-to-your-repository>`
+    1. `poetry config http-basic.<your-repository-name> <username> <password>`
+1. Publish the client with `poetry publish --build -r <your-repository-name>` or, if for public PyPI, just `poetry publish --build`
+
+If you want to install this client into another project without publishing it (e.g. for development) then:
+
+1. If that project **is using Poetry**, you can simply do `poetry add <path-to-this-client>` from that project
+1. If that project is not using Poetry:
+    1. Build a wheel with `poetry build -f wheel`
+    1. Install that wheel from the other project `pip install <path-to-wheel>`
 
-setup(**setup_kwargs)
```

