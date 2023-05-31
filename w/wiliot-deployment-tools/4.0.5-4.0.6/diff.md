# Comparing `tmp/wiliot-deployment-tools-4.0.5.tar.gz` & `tmp/wiliot-deployment-tools-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-deployment-tools-4.0.5.tar", last modified: Sun May 28 12:18:09 2023, max compression
+gzip compressed data, was "wiliot-deployment-tools-4.0.6.tar", last modified: Wed May 31 15:25:22 2023, max compression
```

## Comparing `wiliot-deployment-tools-4.0.5.tar` & `wiliot-deployment-tools-4.0.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.551898 wiliot-deployment-tools-4.0.5/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.539898 wiliot-deployment-tools-4.0.5/.devcontainer/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.543898 wiliot-deployment-tools-4.0.5/.devcontainer/private/
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/.devcontainer/private/devcontainer.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.543898 wiliot-deployment-tools-4.0.5/.devcontainer/public/
--rw-rw-rw-   0 root         (0) root         (0)     1057 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/.devcontainer/public/devcontainer.json
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     7307 2023-05-28 12:18:09.551898 wiliot-deployment-tools-4.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6816 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)     8812 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/ci.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/dep-tools-public.dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/dep-tools.dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-28 12:18:09.551898 wiliot-deployment-tools-4.0.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3457 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.543898 wiliot-deployment-tools-4.0.5/unittests/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/unittests/test_debug_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2250 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/unittests/test_extended_api_edge.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/unittests/test_extended_api_platform.py
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/unittests/test_power_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     2710 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/unittests/test_slack_alerts.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/unittests/test_test_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     2129 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/unittests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.543898 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.547898 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    41989 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/api/extended_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1187 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/api/gw_ssid.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.547898 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/automatic_configuration_tool/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15257 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     3178 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.547898 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    68575 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/analysis_data_bricks.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/debug.py
--rw-rw-rw-   0 root         (0) root         (0)     6004 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3112 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/utils_defines.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.547898 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/firmware_update/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/firmware_update/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23066 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/firmware_update/firmware_update.py
--rw-rw-rw-   0 root         (0) root         (0)     4348 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.547898 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/log_viewer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/log_viewer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1896 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.547898 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/power_mgmt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/power_mgmt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4653 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
--rw-rw-rw-   0 root         (0) root         (0)    26335 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/power_mgmt/power_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     4143 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.547898 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6057 2023-05-28 12:17:48.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-28 12:18:09.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-28 12:18:09.547898 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     7307 2023-05-28 12:18:09.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2061 2023-05-28 12:18:09.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-28 12:18:09.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-05-28 12:18:09.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-28 12:18:09.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      362 2023-05-28 12:18:09.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-28 12:18:09.000000 wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.570601 wiliot-deployment-tools-4.0.6/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.554601 wiliot-deployment-tools-4.0.6/.devcontainer/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.558601 wiliot-deployment-tools-4.0.6/.devcontainer/private/
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/.devcontainer/private/devcontainer.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.558601 wiliot-deployment-tools-4.0.6/.devcontainer/public/
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/.devcontainer/public/devcontainer.json
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     7408 2023-05-31 15:25:22.570601 wiliot-deployment-tools-4.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6917 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     8812 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/dep-tools-public.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/dep-tools.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-31 15:25:22.570601 wiliot-deployment-tools-4.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3457 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.558601 wiliot-deployment-tools-4.0.6/unittests/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/unittests/test_debug_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/unittests/test_extended_api_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/unittests/test_extended_api_platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/unittests/test_power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2710 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/unittests/test_slack_alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/unittests/test_test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/unittests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.562601 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.562601 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    43300 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/api/extended_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/api/gw_ssid.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.562601 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/automatic_configuration_tool/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15516 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     3191 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.566601 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    68575 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/analysis_data_bricks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     6004 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3112 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/utils_defines.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.566601 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/firmware_update/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/firmware_update/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23066 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/firmware_update/firmware_update.py
+-rw-rw-rw-   0 root         (0) root         (0)     4348 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.566601 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/log_viewer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/log_viewer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.566601 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/power_mgmt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/power_mgmt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4653 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
+-rw-rw-rw-   0 root         (0) root         (0)    28031 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/power_mgmt/power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     4827 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.570601 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6057 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-31 15:25:22.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.562601 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     7408 2023-05-31 15:25:22.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2023-05-31 15:25:22.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-31 15:25:22.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-05-31 15:25:22.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-31 15:25:22.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      362 2023-05-31 15:25:22.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-31 15:25:22.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/top_level.txt
```

### Comparing `wiliot-deployment-tools-4.0.5/.devcontainer/private/devcontainer.json` & `wiliot-deployment-tools-4.0.6/.devcontainer/private/devcontainer.json`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/.devcontainer/public/devcontainer.json` & `wiliot-deployment-tools-4.0.6/.devcontainer/public/devcontainer.json`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/LICENSE` & `wiliot-deployment-tools-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/PKG-INFO` & `wiliot-deployment-tools-4.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-deployment-tools
-Version: 4.0.5
+Version: 4.0.6
 Summary: A library for interacting with Wiliot's Deployment Tools
 Home-page: 
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Classifier: Programming Language :: Python :: 3
@@ -86,15 +86,15 @@
   example usage: wlt-firmware -o wiliot update -gw GW0123 -all_brgs
   ```
 ### Power Management
 Use Wiliot Bridge power management functionality
 #### Enter Power Management
 Configure Specified Bridges to work in power management configuration.
 ```
-usage: wlt-power-mgmt -o OwnerID -brg BridgeID enter -sleepduration SLEEPDURATION -onduration ONDURATION [-keepalive KEEPALIVE] [-scan SCAN] [-ledoff] [-gw GW] [-timeout TIMEOUT]
+usage: wlt-power-mgmt -o OwnerID enter -brg BridgeID -sleepduration SLEEPDURATION -onduration ONDURATION [-keepalive KEEPALIVE] [-scan SCAN] [-ledoff] [-gw GW] [-timeout TIMEOUT]
 
 required arguments:
   -owner OWNER  Owner ID
   -brg BRG      Bridge ID
 
 optional arguments:
   -sleepduration SLEEPDURATION
@@ -103,31 +103,31 @@
                         On duration (seconds) *rounds to nearest 30 second interval*
   -keepalive KEEPALIVE  Keep alive period (seconds) *rounds to nearest 5 second interval* (not required, defaults to 30 seconds)
   -scan SCAN            Keep alive scan (milliseconds) *rounds to nearest 10 millisecond interval* (not required, defaults to 300 milliseconds)
   -ledoff               Configure LEDs off (on by default)
   -gw GW                GW ID to configure bridge (required only for broadcast mode)
   -timeout TIMEOUT      Minutes timeout (not required, defaults to 5 minutes)
 
-  example usage: wlt-power-mgmt -o wiliot -brg 0123ABCD enter -sleepduration 5 -onduration 60
+  example usage: wlt-power-mgmt -o wiliot enter -brg 0123ABCD -sleepduration 5 -onduration 60
 ```
 #### Exit Power Management
 Return specified bridges out of power management mode and into normal working mode.
 ```
-usage: wlt-power-mgmt -o OwnerID -brg BridgeID exit [-gw GW] [-no_config] [-timeout TIMEOUT]
+usage: wlt-power-mgmt -o OwnerID exit -brg BridgeID [-gw GW] [-no_config] [-timeout TIMEOUT]
 
 required arguments:
   -owner OWNER  Owner ID
   -brg BRG      Bridge ID
 
 optional arguments:
   -gw GW            GW ID to configure bridge (not required)
   -no_config        If used, GW will not change to optimal configuration
   -timeout TIMEOUT  Minutes timeout (not required, defaults to 5 minutes)
 
-example usage: wlt-power-mgmt -o wiliot -brg 0123ABCD exit
+example usage: wlt-power-mgmt -o wiliot exit -brg BridgeID
 ```
 
 ### Log Viewer
 View Wiliot Gatewa logs
 ```
 usage: wlt-log -owner OWNER -gw GW
 
@@ -141,14 +141,18 @@
 ------------------
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.0.6:
+* Support for android in power management mode
+* Bugfix when no gateway logs found
+  
 Version 4.0.4:
 * Bugfixes, add relevant printouts to CLI to help understand errors.
 
 Version 4.0.3:
 * Initial release of CLI tools suite - Automatic Configuration Tool, Firmware Update, Power Management, Log Viewer.
 
 Version 4.0.0:
```

### Comparing `wiliot-deployment-tools-4.0.5/README.md` & `wiliot-deployment-tools-4.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
   example usage: wlt-firmware -o wiliot update -gw GW0123 -all_brgs
   ```
 ### Power Management
 Use Wiliot Bridge power management functionality
 #### Enter Power Management
 Configure Specified Bridges to work in power management configuration.
 ```
-usage: wlt-power-mgmt -o OwnerID -brg BridgeID enter -sleepduration SLEEPDURATION -onduration ONDURATION [-keepalive KEEPALIVE] [-scan SCAN] [-ledoff] [-gw GW] [-timeout TIMEOUT]
+usage: wlt-power-mgmt -o OwnerID enter -brg BridgeID -sleepduration SLEEPDURATION -onduration ONDURATION [-keepalive KEEPALIVE] [-scan SCAN] [-ledoff] [-gw GW] [-timeout TIMEOUT]
 
 required arguments:
   -owner OWNER  Owner ID
   -brg BRG      Bridge ID
 
 optional arguments:
   -sleepduration SLEEPDURATION
@@ -87,31 +87,31 @@
                         On duration (seconds) *rounds to nearest 30 second interval*
   -keepalive KEEPALIVE  Keep alive period (seconds) *rounds to nearest 5 second interval* (not required, defaults to 30 seconds)
   -scan SCAN            Keep alive scan (milliseconds) *rounds to nearest 10 millisecond interval* (not required, defaults to 300 milliseconds)
   -ledoff               Configure LEDs off (on by default)
   -gw GW                GW ID to configure bridge (required only for broadcast mode)
   -timeout TIMEOUT      Minutes timeout (not required, defaults to 5 minutes)
 
-  example usage: wlt-power-mgmt -o wiliot -brg 0123ABCD enter -sleepduration 5 -onduration 60
+  example usage: wlt-power-mgmt -o wiliot enter -brg 0123ABCD -sleepduration 5 -onduration 60
 ```
 #### Exit Power Management
 Return specified bridges out of power management mode and into normal working mode.
 ```
-usage: wlt-power-mgmt -o OwnerID -brg BridgeID exit [-gw GW] [-no_config] [-timeout TIMEOUT]
+usage: wlt-power-mgmt -o OwnerID exit -brg BridgeID [-gw GW] [-no_config] [-timeout TIMEOUT]
 
 required arguments:
   -owner OWNER  Owner ID
   -brg BRG      Bridge ID
 
 optional arguments:
   -gw GW            GW ID to configure bridge (not required)
   -no_config        If used, GW will not change to optimal configuration
   -timeout TIMEOUT  Minutes timeout (not required, defaults to 5 minutes)
 
-example usage: wlt-power-mgmt -o wiliot -brg 0123ABCD exit
+example usage: wlt-power-mgmt -o wiliot exit -brg BridgeID
 ```
 
 ### Log Viewer
 View Wiliot Gatewa logs
 ```
 usage: wlt-log -owner OWNER -gw GW
 
@@ -125,14 +125,18 @@
 ------------------
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.0.6:
+* Support for android in power management mode
+* Bugfix when no gateway logs found
+  
 Version 4.0.4:
 * Bugfixes, add relevant printouts to CLI to help understand errors.
 
 Version 4.0.3:
 * Initial release of CLI tools suite - Automatic Configuration Tool, Firmware Update, Power Management, Log Viewer.
 
 Version 4.0.0:
```

### Comparing `wiliot-deployment-tools-4.0.5/bitbucket-pipelines.yml` & `wiliot-deployment-tools-4.0.6/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/ci.py` & `wiliot-deployment-tools-4.0.6/ci.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/dep-tools.dockerfile` & `wiliot-deployment-tools-4.0.6/dep-tools.dockerfile`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/setup.py` & `wiliot-deployment-tools-4.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/unittests/test_extended_api_edge.py` & `wiliot-deployment-tools-4.0.6/unittests/test_extended_api_edge.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/unittests/test_extended_api_platform.py` & `wiliot-deployment-tools-4.0.6/unittests/test_extended_api_platform.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/unittests/test_power_mgmt.py` & `wiliot-deployment-tools-4.0.6/unittests/test_power_mgmt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/unittests/test_slack_alerts.py` & `wiliot-deployment-tools-4.0.6/unittests/test_slack_alerts.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/unittests/test_test_tool.py` & `wiliot-deployment-tools-4.0.6/unittests/test_test_tool.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/unittests/test_utils.py` & `wiliot-deployment-tools-4.0.6/unittests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/api/extended_api.py` & `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/api/extended_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,29 +31,34 @@
 
 class GatewayAction(Enum):
     ADD_SSID = 'addSsid'
     TOGGLE_SSID = 'toggleDefaultSsid'
     REBOOT_GW = 'rebootGw'
     START_BRIDGE_OTA = '!send_msg_to_brg'
 
+class AndroidGatewayAction(Enum):
+    DISABLE_UPLINK = -2
+    ENABLE_UPLINK = -3
+    DISABLE_BLE_LOGS = -4
+    ENABLE_BLE_LOGS = -5
 
 class BridgeThroughGatewayAction(Enum):
     REBOOT = '01'
     BLINK = '02'
     POWER_MGMT = '03'
     RESTORE_DEFAULTS = '04'
     SEND_HB = '05'
     PRODUCTION_MODE = '06'
 
 
 class BoardTypes(Enum):
     ENERGOUS = 'Energous Dual-Band (v0)'
     FANSTEL_SINGLE = 'Fanstel Single-Band (v0)'
     FANSTEL_DUAL = 'Fanstel Dual-Band (v0)'
-    MINEW = 'Minew Single-Band (v0)'
+    MINEW_SINGLE = 'Minew Single-Band (v0)'
     MINEW_DUAL = 'Minew Dual-Band (v0)'
     MOKO = 'Moko Dual-Band (v0)'
 
 
 # API Clients
 
 class ParamMissingError(Exception):
@@ -243,15 +248,20 @@
     def send_action_to_gateway(self, gateway_id, action, **kwargs):
         """
         Send an action to a gateway
         :param gateway_id: String - the ID of the gateway to send the action to
         :param action: GatewayAction - Required
         :return: True if the cloud successfully sent the action to the gateway, False otherwise
         """
-        assert action in GatewayAction, 'Action not valid GW Action'
+        gw_type = self.get_gateway_type(gateway_id)
+        assert gw_type in [GatewayType.WIFI, GatewayType.MOBILE], 'gateway does not support action API!'
+        if gw_type == GatewayType.WIFI:
+            assert action in GatewayAction, 'action not valid for WIFI GW!'
+        if gw_type == GatewayType.MOBILE:
+            assert action in AndroidGatewayAction, 'action not valid for Mobile GW!'
         if action == GatewayAction.ADD_SSID:
             assert 'ssid' in kwargs.keys(), "Missing a 'ssid' parameter"
         if action == GatewayAction.START_BRIDGE_OTA:
             assert 'bridge_id' in kwargs.keys(), "Missing a 'bridge_id' parameter"
         path = "gateway/{}/action".format(gateway_id)
         action_payload = action.value
         if action == GatewayAction.START_BRIDGE_OTA:
@@ -266,37 +276,45 @@
             res = self._post(path, payload)
             return res['data'].lower().find("ok") != -1
         except WiliotCloudError as e:
             print("Failed to send action to gateway")
             raise WiliotCloudError(
                 "Failed to send action to gateway. Received the following error: {}".format(e.args[0]))
 
-    def send_bridge_action_through_gw(self, gateway_id, action_type, payload='0', bridge_id=None, broadcast=False, reps=8):
+    def send_bridge_action_through_gw(self, gateway_id, action_type, payload='0', bridge_id=None, broadcast=False, reps=8, ms_to_send=1200):
         """
         Send an action to a bridge through a gateway
-        :param broadcast:
+        :param broadcast: whether to broadcast
         :param gateway_id: String - the ID of the gateway to send the action Through
         :param bridge_id: String - the ID of the bridge to send the action to
         :param action_type: BridgeThroughGatewayAction - Required
         :param payload: 28 bytes (hex string)
+        :param reps: repetition (wifi gw only)
+        :param ms_to_send: milliseconds to send (android gw only)
         :return: True if the cloud successfully sent the action to the gateway, False otherwise
         """
         assert action_type in BridgeThroughGatewayAction, 'Not valid action type'
         assert (bridge_id is not None and broadcast is False) or (bridge_id is None and broadcast is True), \
             'Must supply bridgeId / set broadcast to True'
         assert reps > 0, 'Repetitions must be a positive value!'
+        assert ms_to_send > 0, 'Milliseconds to send must be a positive value!'
         assert len(bridge_id) == 12
         payload = str(payload).ljust(28, '0')
 
         # Packet Header: 0-5 ADVA, 6 Length, 7 AD Type, 8-9 UUID, 10-12 Group ID, 13 MSG type, 14 API Ver.
-        header = '1E16AFFD0000ED0705'
+        header = '1E16C6FC0000ED0707'
         # Randomize Sequence ID
         seq_id = random.getrandbits(8).to_bytes(1, 'big').hex().upper()
+        gw_type = self.get_gateway_type(gateway_id)
+        if gw_type == GatewayType.MOBILE:
+            arg = ms_to_send
+        else:
+            arg = reps
         payload = {
-            "action": f'!sp {header}{seq_id}{bridge_id}{action_type.value}{payload} {reps}'
+            "action": f'!sp {header}{seq_id}{bridge_id}{action_type.value}{payload} {arg}'
         }
         path = "gateway/{}/action".format(gateway_id)
         try:
             res = self._post(path, payload)
             return res['data'].lower().find("ok") != -1
         except WiliotCloudError as e:
             print("Failed to send action to gateway")
@@ -361,14 +379,17 @@
     def print_gateway_logs(self, gateway_id):
         """
         prints gateway logs nicely
         :type gateway_id: str
         :param gateway_id: Gateway ID
         """
         logs = self.get_gateway_logs(gateway_id)
+        if logs is None:
+            print(f'---No logs for GW {gateway_id}---')
+            return None
         logs = logs.reindex(index=logs.index[::-1])
         logs = logs.reset_index()
         datetime_format = "%Y-%m-%dT%H:%M:%SZ"
 
         for row in logs.itertuples():
             timestamp = datetime.datetime.strptime(row.timestamp, datetime_format).replace(tzinfo=pytz.UTC).timestamp()
             local_datetime = datetime.datetime.fromtimestamp(timestamp)
@@ -400,16 +421,21 @@
         try:
             logs = self.get_gateway_logs(gateway_id, hours_back=hours_back)
         except Exception as e:
             debug_print(f'Exception {e} Caught when getting Acks from GW {gateway_id}')
             logs = None
         if logs is None:
             return None
-        logs = logs[list(map(lambda x: x.startswith(' RecievedAction'), logs['message']))]
-        logs['rawPacket'] = logs['message'].apply(lambda x: x.split('=')[1][6:-1])
+        gw_type = self.get_gateway_type(gateway_id)
+        if gw_type == GatewayType.MOBILE:
+            logs = logs[list(map(lambda x: x.startswith(' ReceivedAction'), logs['message']))]
+            logs['rawPacket'] = logs['message'].apply(lambda x: x.split('=')[1][16:-1]).str.upper()
+        else:
+            logs = logs[list(map(lambda x: x.startswith(' RecievedAction') or x.startswith(' ReceivedAction'), logs['message']))]
+            logs['rawPacket'] = logs['message'].apply(lambda x: x.split('=')[1][6:-1])
         logs['bridgeId'] = logs['rawPacket'].apply(lambda x: x[:12])
         logs['actionType'] = logs['rawPacket'].apply(lambda x: BridgeThroughGatewayAction(str(x[12:14])))
         logs['payload'] = logs['rawPacket'].apply(lambda x: x[14:])
         return logs
 
     # Versions & Version-Dependent
     def get_gw_version(self, gw_id):
```

### Comparing `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/api/gw_ssid.py` & `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/api/gw_ssid.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py` & `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 import datetime
 
 from appdirs import user_data_dir
 import numpy as np
 from collections import defaultdict
 
 # Internal Imports
-from wiliot_deployment_tools.api.extended_api import ExtendedEdgeClient, ExtendedPlatformClient
+from wiliot_deployment_tools.api.extended_api import ExtendedEdgeClient, ExtendedPlatformClient, GatewayType
 from wiliot_deployment_tools.firmware_update.firmware_update import FirmwareUpdate
 from wiliot_deployment_tools.common.analysis_data_bricks import create_logfile, db_utils, initialize_logger
 from wiliot_deployment_tools.common.debug import debug_print, is_databricks, print_package_gitinfo
 from wiliot_deployment_tools.common.utils_defines import ATC_GW_CONFIG, ATC_REGION_DICT
 
 IS_DATABRICKS = is_databricks()
 
@@ -184,32 +184,35 @@
             raise ConfigurationToolError(f'No gateways connected to any bridge in location {self.location}!')
         self.gw_by_type = self.edge.get_gateways_types(self.gw_ids)
 
     def init_stage(self):
         # Change GW config
         gw_init_status = []
         self.gw_by_type = self.edge.get_gateways_types(self.gw_ids)
-        for gw_type in self.gw_by_type:
+        for gw_type, gws_by_type in self.gw_by_type.items():
             gw_init_status.extend(self.edge.change_gw_config(
-                self.gw_ids, ATC_GW_CONFIG[gw_type.value]))
+                gws_by_type, ATC_GW_CONFIG[gw_type.value]))
         if set(gw_init_status) != set(self.gw_ids):
             raise ConfigurationToolError('Cannot initialize GWs!')
 
         # Connect to bridges and change to brownout
         debug_print(f'Connecting to bridges in {self.location}...', center=True)
         (self.connected_bridges, self.board_type_dict) = \
             self.edge.connect_gw_bridges(expected_brgs=self.expected_bridges_ids,
                                          expected_num_brgs=self.expected_num_brgs,
                                          do_brown_out=True,
                                          minutes_timeout=2)
 
         # Firmware Upgrade
         if self.ota_upgrade is True:
-            debug_print('Starting OTA Process...', center=True)
-            self.fw_update.firmware_update(self.gw_ids, self.connected_bridges, update_to_latest=True,
+            if GatewayType.WIFI not in self.gw_by_type.keys():
+                debug_print('Can only do OTA with WiFi Gateway! Connect WiFi Gateway in zone and run tool again')
+            else:
+                debug_print('Starting OTA Process...', center=True)
+                self.fw_update.firmware_update(self.gw_by_type[GatewayType.WIFI], self.connected_bridges, update_to_latest=True,
                                            ignore_bridges=self.ignore_bridges, update_all_connected_bridges=False, action=True)
         
         # Configure Bridges
         debug_print('Configuring bridges...', center=True)        
         
         # Calculate Configuration Parameters
         rx_tx_cycle = max(min((2 * len(self.connected_bridges)), 255), 15)
```

### Comparing `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py` & `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         print('Edge Management credentials saved/upload from {}'.format(user_config_file_path))
     else:
         raise Exception('invalid Edge Management credentials - please try again to login')
 
     act = AutomaticConfigurationTool(edge_api_key=edge_api_key, asset_api_key=asset_api_key, owner=args.owner,
                                      location=args.location, env='prod', ota_upgrade=args.ota,
                                      ignore_bridges=args.ignore_bridges, pacing_interval=args.pacer,
-                                     use_gp_zone=args.no_gp_zone, expected_num_brgs=args.expected_num_brgs)
+                                     use_gp_zone=args.no_gp_zone, expected_num_brgs=args.expected_num_brgs, region='IL')
     act.init_stage()
 
 def main_cli():
     main()
 
 if __name__ == '__main__':
     main()
```

### Comparing `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/analysis_data_bricks.py` & `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/analysis_data_bricks.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/debug.py` & `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/debug.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/utils.py` & `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/common/utils_defines.py` & `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/utils_defines.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/firmware_update/firmware_update.py` & `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/firmware_update/firmware_update.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/firmware_update/firmware_update_cli.py` & `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/firmware_update/firmware_update_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/log_viewer/log_viewer_cli.py` & `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/log_viewer/log_viewer_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import pprint
-from wiliot_deployment_tools.api.extended_api import ExtendedEdgeClient
+from wiliot_deployment_tools.api.extended_api import AndroidGatewayAction, ExtendedEdgeClient
 from argparse import ArgumentParser
 from wiliot_core import check_user_config_is_ok
 import colorama
 
 def main():
     parser = ArgumentParser(prog='wlt-log',
                             description='Log Viewer - CLI Tool to view Wiliot Gateway logs')
     required = parser.add_argument_group('required arguments')
     required.add_argument('-owner', type=str, help="Owner ID", required=True)
     required.add_argument('-gw', type=str, help="Gateway ID", required=True)
     parser.add_argument('-test', action='store_true',
                     help='If flag used, use test environment (prod is used by default)')
-
+    parser.add_argument('--mobile_ble_logging', choices=['on', 'off'], help='set mobile BLE logging to on or off')
+    
     args = parser.parse_args()
     if args.test:
         env = 'test'
     else:
         env = 'prod'
 
     owner_id = args.owner
@@ -24,23 +25,32 @@
     user_config_file_path, api_key, is_success = check_user_config_is_ok(owner_id, conf_env, 'edge')
     if is_success:
         print('credentials saved/upload from {}'.format(user_config_file_path))
     else:
         raise Exception('invalid credentials - please try again to login')
 
     colorama.init()
-    print(colorama.Fore.LIGHTBLACK_EX, end=None)
-    print(colorama.Fore.GREEN +
-          f'---Printing info for {args.gw}---' + colorama.Style.RESET_ALL)
-    print(colorama.Style.RESET_ALL)
+
     e = ExtendedEdgeClient(api_key, args.owner, env)
-    try:
-        print_gw(e, args.gw)
-    except AttributeError:
-        parser.print_help()
+    if args.mobile_ble_logging is not None:
+        print(colorama.Fore.LIGHTBLACK_EX, end=None)
+        print(colorama.Fore.GREEN +
+          f'---Setting mobile BLE Logging {args.gw} to {args.mobile_ble_logging}---' + colorama.Style.RESET_ALL)        
+        mode = {'on': AndroidGatewayAction.ENABLE_BLE_LOGS, 'off': AndroidGatewayAction.DISABLE_BLE_LOGS}
+        res = e.send_action_to_gateway(args.gw, mode[args.mobile_ble_logging])
+        print({args.gw: res})
+    else:
+        print(colorama.Fore.LIGHTBLACK_EX, end=None)
+        print(colorama.Fore.GREEN +
+            f'---Printing info for {args.gw}---' + colorama.Style.RESET_ALL)
+        print(colorama.Style.RESET_ALL)
+        try:
+            print_gw(e, args.gw)
+        except AttributeError as e:
+            print(e)
 
 def print_gw(e, gw):
     info = e.get_gateway_info(gw)
 
     print(colorama.Fore.GREEN +
         f'---Gateway Info---' + colorama.Style.RESET_ALL)
     pprint.pprint(info)
```

### Comparing `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py` & `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/power_mgmt/power_mgmt.py` & `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/power_mgmt/power_mgmt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 from doctest import debug
 import sys
 import time
 import bitstruct
-from wiliot_deployment_tools.api.extended_api import BridgeThroughGatewayAction, ExtendedEdgeClient, GatewayType
+from wiliot_deployment_tools.api.extended_api import EXCEPTIONS_TO_CATCH, AndroidGatewayAction, BridgeThroughGatewayAction, ExtendedEdgeClient, GatewayType
 from wiliot_deployment_tools.common.debug import debug_print
 from wiliot_deployment_tools.common.utils_defines import KEEP_ALIVE_PERIOD, KEEP_ALIVE_SCAN_DURATION, SEC_TO_SEND, BROADCAST_DST_MAC, EXIT_POWER_MGMT_GW_DICT
 
 
 class PowerManagementError(Exception):
     pass
 
@@ -152,27 +152,29 @@
         sleep_duration_mins = sleep_duration
         on_duration_secs = on_duration * 30
         keep_alive_period_secs = keep_alive_period * 5
         keep_alive_scan_ms = keep_alive_scan * 10
         return sleep_duration_mins, on_duration_secs, keep_alive_period_secs, keep_alive_scan_ms, leds_on
 
 
-class PowerManagementClient(ExtendedEdgeClient):
-    
+class BridgePowerManagementClient(ExtendedEdgeClient):
+        
     def check_gw_compatible_for_pwr_mgmt(self, gateway_id):
         """
         checks if gateway is compatible to send and receive power management configurations
         :type gateway_id: str
         :param gateway_id: gateway ID
         :rtype: bool
         """
         gateway_type = self.get_gateway_type(gateway_id)
         if gateway_type != GatewayType.WIFI:
-            debug_print(gateway_type)
-            return False
+            if gateway_type == GatewayType.MOBILE: 
+                return True
+            else:
+                return False
         gw_dict = self.get_gateway(gateway_id)        
         ble_ver = gw_dict["reportedConf"]["bleChipSwVersion"]
         if gw_dict['online'] and \
            self.check_ble_power_mgmt_support(ble_ver):
             if gw_dict['reportedConf']['additional']['gwMgmtMode'] == 'transparent':
                 support = self.check_gw_ble_transparent_power_mgmt_support(ble_ver)
                 if not support:
@@ -187,23 +189,21 @@
         Returns relevant GW for sending actions to bridge
         :param bridge_id: Bridge ID
         :rtype: str
         :return: relevant Gateway ID
         """
 
         # TODO - return list of potential GWs
-        potential_gws = list()
         owner_gws = self.get_gateways()
         owner_gw_ids = []
         owner_gw_ids.extend(g['gatewayId'] for g in owner_gws)
         for gw in self.get_bridge(bridge_id)['connections']:
             if gw['gatewayId'] not in owner_gw_ids:
                 continue
             gw_id = gw['gatewayId']
-            gw_dict = self.get_gateway(gw_id)
             if gw['connected'] and \
                     bridge_id in self.get_seen_bridges(gw_id) and \
                     self.check_gw_compatible_for_pwr_mgmt(gw_id):
                 if bridge_id in self.get_seen_bridges(gw['gatewayId']):
                             return gw['gatewayId']
         raise PowerManagementError(f'No relevant GW connected to bridge! Check deployment')
 
@@ -273,30 +273,45 @@
         :rtype: bool
         :return: True if sent, False otherwise
         """
         if gateway_id is None:
             via_gw = self.get_bridge_relevant_gw(bridge_id)
         else:
             via_gw = gateway_id
+        reps = 8
+        ms_to_send = 1200
+        seconds_to_send = datetime.timedelta(seconds=seconds_to_send)
+        # Check BRG Compatability
         brg_version = None
         if bridge_id is not BROADCAST_DST_MAC:
             brg_version = self.get_brg_ble_version(bridge_id)
-        gw_version = self.get_gw_ble_version(via_gw)
-        for version in filter(None, [brg_version, gw_version]):
-            if not self.check_ble_power_mgmt_support(version):
-                return False
-        rxtx = datetime.timedelta(milliseconds=
-                                  self.get_gateway(via_gw)['reportedConf']['additional']['rxTxPeriodMs'])
-        seconds_to_send = datetime.timedelta(seconds=seconds_to_send)
-        reps = seconds_to_send // rxtx + 1
-        if not silent:
-            debug_print(f'Sending packet through GW {via_gw} for {seconds_to_send.total_seconds()} seconds, rxTx = {int(rxtx.total_seconds()*1000)} ms, reps = {reps}')
-        res = self.send_bridge_action_through_gw(gateway_id,
+        # Check GW Compatability
+        gw_type = self.get_gateway_type(via_gw)
+        if gw_type == GatewayType.WIFI:
+            gw_version = self.get_gw_ble_version(via_gw)
+            for version in filter(None, [brg_version, gw_version]):
+                if not self.check_ble_power_mgmt_support(version):
+                    return False
+            rxtx = datetime.timedelta(milliseconds=
+                                    self.get_gateway(via_gw)['reportedConf']['additional']['rxTxPeriodMs'])
+            reps = seconds_to_send // rxtx + 1
+            if not silent:
+                debug_print(f'Sending packet through WIFI GW {via_gw} for {seconds_to_send.total_seconds()} seconds, rxTx = {int(rxtx.total_seconds()*1000)} ms, reps = {reps}')
+        if gw_type == GatewayType.MOBILE:
+            if not silent:
+                debug_print(f'Sending packet through ANDROID GW {via_gw} for {seconds_to_send.total_seconds()} seconds')
+            ms_to_send = int(seconds_to_send.total_seconds()*1000)
+        try:
+            res = self.send_bridge_action_through_gw(gateway_id,
                                                  BridgeThroughGatewayAction.POWER_MGMT,
-                                                 packet.payload, bridge_id, reps=reps)
+                                                 packet.payload, bridge_id, reps=reps, ms_to_send=ms_to_send)
+        except EXCEPTIONS_TO_CATCH as e:
+            debug_print('Exception caught when sending power mgmt packet!')
+            debug_print(e)
+            return False
         return res
 
     def broadcast_pwr_mgmt_packet(self, packet, gateway_id, silent=False, seconds_to_send=1):
         """
         broadcast packet to all bridges connected to GW
         :type packet: PowerManagementPacket
         :param packet: packet to broadcast
@@ -527,25 +542,45 @@
             raise PowerManagementError('Must specify bridgeId / set broadcast to True')
         if broadcast:
             if gateway_id is None:
                 raise PowerManagementError('Must specify GW ID to broadcast')
         via_gw = self.get_bridge_relevant_gw(bridge_id) if gateway_id is None else gateway_id
         if not self.check_gw_compatible_for_pwr_mgmt(via_gw):
             raise PowerManagementError(f'GW {via_gw} Not compatible for power management!')
-        gw_dict = self.get_gateway(via_gw)['reportedConf']['additional']
+        gateway_type = self.get_gateway_type(via_gw)
         need_to_update = False
-        for param in EXIT_POWER_MGMT_GW_DICT:
-            if gw_dict[param] != EXIT_POWER_MGMT_GW_DICT[param]:
-                need_to_update = True
-        if need_to_update and update_gw:
-            debug_print('Changing GW Params to rxTxPeriod = 15 ms, gwRxChannel = Ch. 39')
+        if gateway_type == GatewayType.WIFI:
+            gw_dict = self.get_gateway(via_gw)['reportedConf']['additional']
+            for param in EXIT_POWER_MGMT_GW_DICT:
+                if gw_dict[param] != EXIT_POWER_MGMT_GW_DICT[param]:
+                    need_to_update = True
+            if need_to_update and update_gw:
+                debug_print('Changing GW Params to rxTxPeriod = 15 ms, gwRxChannel = Ch. 39')
             self.change_gw_config([via_gw], EXIT_POWER_MGMT_GW_DICT)
         if broadcast:
             res = self.broadcast_packet_until_ack(gateway_id, packet, minutes_timeout)
         else:
             res = self.send_packet_until_ack(via_gw, bridge_id, packet, minutes_timeout)
         if need_to_update and update_gw:
             debug_print('Finished sending exit packets, returning GW to old state')
             self.change_gw_config([via_gw], gw_dict)
         return res
 
 
+class AndroidPowerManagementClient(ExtendedEdgeClient):
+    def set_uplink_mode(self, gateway_id, uplink_mode):
+        """
+        set uplink mode (on/off) for android GW
+        :param gateway_id: gateway ID
+        :type gateway_id: str
+        :param uplink_mode: uplink mode
+        :type uplink_mode: bool
+        """
+        payload = {True: AndroidGatewayAction.ENABLE_UPLINK,
+                   False: AndroidGatewayAction.DISABLE_UPLINK}
+        gw_type = self.get_gateway_type(gateway_id)
+        assert gw_type == GatewayType.MOBILE, f'GW {gateway_id} not an android GW!'
+        debug_print(f'Setting GW {gateway_id} uplink to {uplink_mode}')
+        return self.send_action_to_gateway(gateway_id, payload[uplink_mode])
+
+class PowerManagementClient(BridgePowerManagementClient, AndroidPowerManagementClient):
+    pass
```

### Comparing `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py` & `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,53 @@
+from numpy import require
 from wiliot_deployment_tools.power_mgmt.power_mgmt import PowerManagementClient
 from wiliot_core import check_user_config_is_ok
 from wiliot_deployment_tools.common.utils_defines import *
 from argparse import ArgumentParser
 import sys
 
 
 def main():
     # parser
     parser = ArgumentParser(prog='wlt-power-mgmt',
                             description='Power Management - CLI Tool for using Wiliot Bridge power management functionality')
     required = parser.add_argument_group('required arguments')
     required.add_argument('-owner', type=str, help="Owner ID", required=True)
-    parser.add_argument('-brg', type=str, help="Bridge ID", required=True)
     parser.add_argument('-test', action='store_true',
                         help='if flag used, use test environment (prod is used by default)')
 
     subparsers = parser.add_subparsers()
     parser_enter = subparsers.add_parser('enter',
                                          help='Configure Specified Bridges to work in power management configuration',
-                                         epilog="example usage: wlt-power-mgmt -o wiliot -brg 0123ABCD enter -sleepduration 5 -onduration 60")
+                                         epilog="example usage: wlt-power-mgmt -o wiliot enter -brg 0123ABCD -sleepduration 5 -onduration 60")
     parser_enter.set_defaults(func=enter_contex)
+    parser_enter.add_argument('-brg', type=str, help="Bridge ID", required=True)
     parser_enter.add_argument('-sleepduration', type=int, help="Sleep duration (minutes)", required=True)
     parser_enter.add_argument('-onduration', type=int, help="On duration (seconds) *rounds to nearest 30 second interval*", required=True)
     parser_enter.add_argument('-keepalive', type=int, help="Keep alive period (seconds) *rounds to nearest 5 second interval* (not required, defaults to 30 seconds)", required=False, default=KEEP_ALIVE_PERIOD)
     parser_enter.add_argument('-scan', type=int, help="Keep alive scan (milliseconds) *rounds to nearest 10 millisecond interval* (not required, defaults to 300 milliseconds)", required=False, default=KEEP_ALIVE_SCAN_DURATION)
     parser_enter.add_argument('-ledoff', action='store_false', help="Configure LEDs off (on by default)", required=False)
     parser_enter.add_argument('-gw', type=str, help="GW ID to configure bridge (required only for broadcast mode)", required=False)
     parser_enter.add_argument('-timeout', type=int, help="Minutes timeout (not required, defaults to 5 minutes)", required=False, default=5)
 
     parser_exit = subparsers.add_parser(
         'exit', help='Return specified bridges out of power management mode and into normal working mode',
-        epilog="example usage: wlt-power-mgmt -o wiliot -brg 0123ABCD exit")
+        epilog="example usage: wlt-power-mgmt -o wiliot exit -brg 0123ABCD")
     parser_exit.set_defaults(func=exit_contex)
+    parser_exit.add_argument('-brg', type=str, help="Bridge ID", required=True)
     parser_exit.add_argument('-gw', type=str, help="GW ID to configure bridge (not required)", required=False)
     parser_exit.add_argument('-no_config', action='store_false', help="If used, GW will not change to optimal configuration", required=False)
     parser_exit.add_argument('-timeout', type=int, help="Minutes timeout (not required, defaults to 5 minutes)", required=False, default=5)
 
+    parser_mobile = subparsers.add_parser(
+        'android', help='Change mobile uplink mode',
+        epilog="example usage: wlt-power-mgmt -o wiliot exit -brg 0123ABCD")
+    parser_mobile.set_defaults(func=android)
+    parser_mobile.add_argument('-gw', type=str, help="Gateway ID", required=True)
+    parser_mobile.add_argument('-uplink', choices=['on', 'off'], help='set uplink mode to on or off')
 
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         sys.exit(1)
 
     args, unknown = parser.parse_known_args()
     if args.test:
@@ -67,11 +75,17 @@
 
 
 def exit_contex(args):
     res = args.pm.exit_power_mgmt(gateway_id=args.gw, update_gw=args.no_config, 
                                   bridge_id=args.brg, minutes_timeout=args.timeout)
     print(res)
 
+def android(args):
+    mode = {'on': True, 'off': False}
+    res = args.pm.set_uplink_mode(gateway_id=args.gw, uplink_mode=mode[args.uplink])
+    print({args.gw: res})
+
+
 def main_cli():
     main()
 if __name__ == '__main__':
     main()
```

### Comparing `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools/utils/get_version.py` & `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/PKG-INFO` & `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-deployment-tools
-Version: 4.0.5
+Version: 4.0.6
 Summary: A library for interacting with Wiliot's Deployment Tools
 Home-page: 
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Classifier: Programming Language :: Python :: 3
@@ -86,15 +86,15 @@
   example usage: wlt-firmware -o wiliot update -gw GW0123 -all_brgs
   ```
 ### Power Management
 Use Wiliot Bridge power management functionality
 #### Enter Power Management
 Configure Specified Bridges to work in power management configuration.
 ```
-usage: wlt-power-mgmt -o OwnerID -brg BridgeID enter -sleepduration SLEEPDURATION -onduration ONDURATION [-keepalive KEEPALIVE] [-scan SCAN] [-ledoff] [-gw GW] [-timeout TIMEOUT]
+usage: wlt-power-mgmt -o OwnerID enter -brg BridgeID -sleepduration SLEEPDURATION -onduration ONDURATION [-keepalive KEEPALIVE] [-scan SCAN] [-ledoff] [-gw GW] [-timeout TIMEOUT]
 
 required arguments:
   -owner OWNER  Owner ID
   -brg BRG      Bridge ID
 
 optional arguments:
   -sleepduration SLEEPDURATION
@@ -103,31 +103,31 @@
                         On duration (seconds) *rounds to nearest 30 second interval*
   -keepalive KEEPALIVE  Keep alive period (seconds) *rounds to nearest 5 second interval* (not required, defaults to 30 seconds)
   -scan SCAN            Keep alive scan (milliseconds) *rounds to nearest 10 millisecond interval* (not required, defaults to 300 milliseconds)
   -ledoff               Configure LEDs off (on by default)
   -gw GW                GW ID to configure bridge (required only for broadcast mode)
   -timeout TIMEOUT      Minutes timeout (not required, defaults to 5 minutes)
 
-  example usage: wlt-power-mgmt -o wiliot -brg 0123ABCD enter -sleepduration 5 -onduration 60
+  example usage: wlt-power-mgmt -o wiliot enter -brg 0123ABCD -sleepduration 5 -onduration 60
 ```
 #### Exit Power Management
 Return specified bridges out of power management mode and into normal working mode.
 ```
-usage: wlt-power-mgmt -o OwnerID -brg BridgeID exit [-gw GW] [-no_config] [-timeout TIMEOUT]
+usage: wlt-power-mgmt -o OwnerID exit -brg BridgeID [-gw GW] [-no_config] [-timeout TIMEOUT]
 
 required arguments:
   -owner OWNER  Owner ID
   -brg BRG      Bridge ID
 
 optional arguments:
   -gw GW            GW ID to configure bridge (not required)
   -no_config        If used, GW will not change to optimal configuration
   -timeout TIMEOUT  Minutes timeout (not required, defaults to 5 minutes)
 
-example usage: wlt-power-mgmt -o wiliot -brg 0123ABCD exit
+example usage: wlt-power-mgmt -o wiliot exit -brg BridgeID
 ```
 
 ### Log Viewer
 View Wiliot Gatewa logs
 ```
 usage: wlt-log -owner OWNER -gw GW
 
@@ -141,14 +141,18 @@
 ------------------
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.0.6:
+* Support for android in power management mode
+* Bugfix when no gateway logs found
+  
 Version 4.0.4:
 * Bugfixes, add relevant printouts to CLI to help understand errors.
 
 Version 4.0.3:
 * Initial release of CLI tools suite - Automatic Configuration Tool, Firmware Update, Power Management, Log Viewer.
 
 Version 4.0.0:
```

### Comparing `wiliot-deployment-tools-4.0.5/wiliot_deployment_tools.egg-info/SOURCES.txt` & `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

