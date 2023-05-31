# Comparing `tmp/wiliot-deployment-tools-4.0.6.tar.gz` & `tmp/wiliot-deployment-tools-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-deployment-tools-4.0.6.tar", last modified: Wed May 31 15:25:22 2023, max compression
+gzip compressed data, was "wiliot-deployment-tools-4.0.7.tar", last modified: Wed May 31 15:37:46 2023, max compression
```

## Comparing `wiliot-deployment-tools-4.0.6.tar` & `wiliot-deployment-tools-4.0.7.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.570601 wiliot-deployment-tools-4.0.6/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.554601 wiliot-deployment-tools-4.0.6/.devcontainer/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.558601 wiliot-deployment-tools-4.0.6/.devcontainer/private/
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/.devcontainer/private/devcontainer.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.558601 wiliot-deployment-tools-4.0.6/.devcontainer/public/
--rw-rw-rw-   0 root         (0) root         (0)     1057 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/.devcontainer/public/devcontainer.json
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     7408 2023-05-31 15:25:22.570601 wiliot-deployment-tools-4.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6917 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)     8812 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/ci.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/dep-tools-public.dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/dep-tools.dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-31 15:25:22.570601 wiliot-deployment-tools-4.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3457 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.558601 wiliot-deployment-tools-4.0.6/unittests/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/unittests/test_debug_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2250 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/unittests/test_extended_api_edge.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/unittests/test_extended_api_platform.py
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/unittests/test_power_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     2710 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/unittests/test_slack_alerts.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/unittests/test_test_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     2129 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/unittests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.562601 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.562601 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    43300 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/api/extended_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1187 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/api/gw_ssid.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.562601 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/automatic_configuration_tool/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15516 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     3191 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.566601 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    68575 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/analysis_data_bricks.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/debug.py
--rw-rw-rw-   0 root         (0) root         (0)     6004 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3112 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/utils_defines.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.566601 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/firmware_update/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/firmware_update/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23066 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/firmware_update/firmware_update.py
--rw-rw-rw-   0 root         (0) root         (0)     4348 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.566601 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/log_viewer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/log_viewer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2541 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.566601 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/power_mgmt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/power_mgmt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4653 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
--rw-rw-rw-   0 root         (0) root         (0)    28031 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/power_mgmt/power_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     4827 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.570601 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6057 2023-05-31 15:24:58.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-31 15:25:22.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:25:22.562601 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     7408 2023-05-31 15:25:22.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2061 2023-05-31 15:25:22.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-31 15:25:22.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-05-31 15:25:22.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-31 15:25:22.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      362 2023-05-31 15:25:22.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-31 15:25:22.000000 wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.448201 wiliot-deployment-tools-4.0.7/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.424200 wiliot-deployment-tools-4.0.7/.devcontainer/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.436200 wiliot-deployment-tools-4.0.7/.devcontainer/private/
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/.devcontainer/private/devcontainer.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.436200 wiliot-deployment-tools-4.0.7/.devcontainer/public/
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/.devcontainer/public/devcontainer.json
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     7396 2023-05-31 15:37:46.448201 wiliot-deployment-tools-4.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6905 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     8812 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/dep-tools-public.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/dep-tools.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-31 15:37:46.448201 wiliot-deployment-tools-4.0.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3457 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.436200 wiliot-deployment-tools-4.0.7/unittests/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/unittests/test_debug_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/unittests/test_extended_api_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/unittests/test_extended_api_platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/unittests/test_power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2710 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/unittests/test_slack_alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/unittests/test_test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/unittests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.436200 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.440201 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    43300 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/api/extended_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/api/gw_ssid.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.444201 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/automatic_configuration_tool/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15516 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     3178 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.444201 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    68575 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/analysis_data_bricks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     6004 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3112 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/utils_defines.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.444201 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/firmware_update/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/firmware_update/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23066 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/firmware_update/firmware_update.py
+-rw-rw-rw-   0 root         (0) root         (0)     4348 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.444201 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/log_viewer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/log_viewer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.444201 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/power_mgmt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/power_mgmt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4653 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
+-rw-rw-rw-   0 root         (0) root         (0)    28031 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/power_mgmt/power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     4827 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.448201 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6057 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-31 15:37:46.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.440201 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     7396 2023-05-31 15:37:46.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2023-05-31 15:37:46.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-31 15:37:46.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-05-31 15:37:46.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-31 15:37:46.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      362 2023-05-31 15:37:46.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-31 15:37:46.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/top_level.txt
```

### Comparing `wiliot-deployment-tools-4.0.6/.devcontainer/private/devcontainer.json` & `wiliot-deployment-tools-4.0.7/.devcontainer/private/devcontainer.json`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/.devcontainer/public/devcontainer.json` & `wiliot-deployment-tools-4.0.7/.devcontainer/public/devcontainer.json`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/LICENSE` & `wiliot-deployment-tools-4.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/PKG-INFO` & `wiliot-deployment-tools-4.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-deployment-tools
-Version: 4.0.6
+Version: 4.0.7
 Summary: A library for interacting with Wiliot's Deployment Tools
 Home-page: 
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Classifier: Programming Language :: Python :: 3
@@ -141,16 +141,16 @@
 ------------------
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
-Version 4.0.6:
-* Support for android in power management mode
+Version 4.0.7:
+* Android power management support
 * Bugfix when no gateway logs found
   
 Version 4.0.4:
 * Bugfixes, add relevant printouts to CLI to help understand errors.
 
 Version 4.0.3:
 * Initial release of CLI tools suite - Automatic Configuration Tool, Firmware Update, Power Management, Log Viewer.
```

### Comparing `wiliot-deployment-tools-4.0.6/README.md` & `wiliot-deployment-tools-4.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -125,16 +125,16 @@
 ------------------
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
-Version 4.0.6:
-* Support for android in power management mode
+Version 4.0.7:
+* Android power management support
 * Bugfix when no gateway logs found
   
 Version 4.0.4:
 * Bugfixes, add relevant printouts to CLI to help understand errors.
 
 Version 4.0.3:
 * Initial release of CLI tools suite - Automatic Configuration Tool, Firmware Update, Power Management, Log Viewer.
```

### Comparing `wiliot-deployment-tools-4.0.6/bitbucket-pipelines.yml` & `wiliot-deployment-tools-4.0.7/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/ci.py` & `wiliot-deployment-tools-4.0.7/ci.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/dep-tools.dockerfile` & `wiliot-deployment-tools-4.0.7/dep-tools.dockerfile`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/setup.py` & `wiliot-deployment-tools-4.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/unittests/test_extended_api_edge.py` & `wiliot-deployment-tools-4.0.7/unittests/test_extended_api_edge.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/unittests/test_extended_api_platform.py` & `wiliot-deployment-tools-4.0.7/unittests/test_extended_api_platform.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/unittests/test_power_mgmt.py` & `wiliot-deployment-tools-4.0.7/unittests/test_power_mgmt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/unittests/test_slack_alerts.py` & `wiliot-deployment-tools-4.0.7/unittests/test_slack_alerts.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/unittests/test_test_tool.py` & `wiliot-deployment-tools-4.0.7/unittests/test_test_tool.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/unittests/test_utils.py` & `wiliot-deployment-tools-4.0.7/unittests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/api/extended_api.py` & `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/api/extended_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/api/gw_ssid.py` & `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/api/gw_ssid.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py` & `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py` & `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         print('Edge Management credentials saved/upload from {}'.format(user_config_file_path))
     else:
         raise Exception('invalid Edge Management credentials - please try again to login')
 
     act = AutomaticConfigurationTool(edge_api_key=edge_api_key, asset_api_key=asset_api_key, owner=args.owner,
                                      location=args.location, env='prod', ota_upgrade=args.ota,
                                      ignore_bridges=args.ignore_bridges, pacing_interval=args.pacer,
-                                     use_gp_zone=args.no_gp_zone, expected_num_brgs=args.expected_num_brgs, region='IL')
+                                     use_gp_zone=args.no_gp_zone, expected_num_brgs=args.expected_num_brgs)
     act.init_stage()
 
 def main_cli():
     main()
 
 if __name__ == '__main__':
     main()
```

### Comparing `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/analysis_data_bricks.py` & `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/analysis_data_bricks.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/debug.py` & `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/debug.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/utils.py` & `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/common/utils_defines.py` & `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/utils_defines.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/firmware_update/firmware_update.py` & `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/firmware_update/firmware_update.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/firmware_update/firmware_update_cli.py` & `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/firmware_update/firmware_update_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/log_viewer/log_viewer_cli.py` & `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/log_viewer/log_viewer_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py` & `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/power_mgmt/power_mgmt.py` & `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/power_mgmt/power_mgmt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py` & `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools/utils/get_version.py` & `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/PKG-INFO` & `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-deployment-tools
-Version: 4.0.6
+Version: 4.0.7
 Summary: A library for interacting with Wiliot's Deployment Tools
 Home-page: 
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Classifier: Programming Language :: Python :: 3
@@ -141,16 +141,16 @@
 ------------------
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
-Version 4.0.6:
-* Support for android in power management mode
+Version 4.0.7:
+* Android power management support
 * Bugfix when no gateway logs found
   
 Version 4.0.4:
 * Bugfixes, add relevant printouts to CLI to help understand errors.
 
 Version 4.0.3:
 * Initial release of CLI tools suite - Automatic Configuration Tool, Firmware Update, Power Management, Log Viewer.
```

### Comparing `wiliot-deployment-tools-4.0.6/wiliot_deployment_tools.egg-info/SOURCES.txt` & `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

