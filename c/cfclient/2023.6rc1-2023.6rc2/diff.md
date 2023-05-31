# Comparing `tmp/cfclient-2023.6rc1.tar.gz` & `tmp/cfclient-2023.6rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfclient-2023.6rc1.tar", last modified: Wed May 31 11:12:22 2023, max compression
+gzip compressed data, was "cfclient-2023.6rc2.tar", last modified: Wed May 31 13:45:42 2023, max compression
```

## Comparing `cfclient-2023.6rc1.tar` & `cfclient-2023.6rc2.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.509643 cfclient-2023.6rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-31 11:12:22.509643 cfclient-2023.6rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/gitversion.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 11:12:22.509643 cfclient-2023.6rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.493643 cfclient-2023.6rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.493643 cfclient-2023.6rc1/src/cfclient/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.497643 cfclient-2023.6rc1/src/cfclient/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.497643 cfclient-2023.6rc1/src/cfclient/configs/input/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/input/Generic_OS_X.json
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/input/Joystick.json
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/input/PS3_Mode_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/input/PS3_Mode_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/input/PS3_Mode_3.json
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/input/PS4_Mode_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/input/PS4_Mode_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/input/PS4_shoulder_btns_yaw.json
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/input/xbox360_mode1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.497643 cfclient-2023.6rc1/src/cfclient/configs/log/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/log/stabilizer.json
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/headless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.497643 cfclient-2023.6rc1/src/cfclient/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   123763 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/resources/log_param_doc.json
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/resources/map.html
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/resources/map.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.497643 cfclient-2023.6rc1/src/cfclient/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/connectivity_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.501643 cfclient-2023.6rc1/src/cfclient/ui/dialogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/about.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/about.ui
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/anchor_position_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/anchor_position_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/basestation_mode_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/basestation_mode_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)    22297 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/bootloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/bootloader.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/cf2config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/cf2config.ui
--rw-r--r--   0 runner    (1001) docker     (123)    17902 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/inputconfigdialogue.py
--rw-r--r--   0 runner    (1001) docker     (123)    24416 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/inputconfigdialogue.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/lighthouse_bs_geometry_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/lighthouse_bs_geometry_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/lighthouse_system_type_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/lighthouse_system_type_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)    22514 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/logconfigdialogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/logconfigdialogue.ui
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.501643 cfclient-2023.6rc1/src/cfclient/ui/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/icons/checkmark_black.png
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/icons/checkmark_white.png
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/icons/create.png
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/icons/delete.png
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/icons/icon-256.png
--rw-r--r--   0 runner    (1001) docker     (123)    36940 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    16092 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/main.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/pluginhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/pose_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tab_toolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.505643 cfclient-2023.6rc1/src/cfclient/ui/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/ConsoleTab.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/CrtpSharkToolbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/ExampleTab.py
--rw-r--r--   0 runner    (1001) docker     (123)    34668 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/FlightTab.py
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/GpsTab.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/LEDTab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/LogBlockDebugTab.py
--rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/LogBlockTab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/LogClientTab.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/LogTab.py
--rw-r--r--   0 runner    (1001) docker     (123)    15379 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/ParamTab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/PlotTab.py
--rw-r--r--   0 runner    (1001) docker     (123)    57266 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/QualisysTab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/TuningTab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/consoleTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/crtpSharkToolbox.ui
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/exampleTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/flightActionContainer.ui
--rw-r--r--   0 runner    (1001) docker     (123)    40263 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/flightTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/gpsTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/ledTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)    27424 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/lighthouse_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/lighthouse_tab.ui
--rw-r--r--   0 runner    (1001) docker     (123)    31493 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/locopositioning_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    16370 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/locopositioning_tab.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/logBlockDebugTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/logBlockTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/logClientTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/logTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/paramTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/plotTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)    32634 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/qualisysTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)    26596 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/tuningTab.ui
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.505643 cfclient-2023.6rc1/src/cfclient/ui/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/widgets/ai.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/widgets/hexspinbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/widgets/plotter.ui
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/widgets/plotwidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/widgets/super_slider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.505643 cfclient-2023.6rc1/src/cfclient/ui/wizards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/wizards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_2.png
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_3.png
--rw-r--r--   0 runner    (1001) docker     (123)    13664 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_4.png
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_5.png
--rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/wizards/lighthouse_geo_bs_estimation_wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.505643 cfclient-2023.6rc1/src/cfclient/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/config_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.505643 cfclient-2023.6rc1/src/cfclient/utils/input/
--rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.509643 cfclient-2023.6rc1/src/cfclient/utils/input/inputinterfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/inputinterfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/inputinterfaces/leapmotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/inputinterfaces/wiimote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/inputinterfaces/zmqpull.py
--rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/inputreaderinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.509643 cfclient-2023.6rc1/src/cfclient/utils/input/inputreaders/
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/inputreaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/inputreaders/linuxjsdev.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/inputreaders/pysdl2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.509643 cfclient-2023.6rc1/src/cfclient/utils/input/mux/
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/mux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/mux/nomux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/mux/takeovermux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/mux/takeoverselectivemux.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/logconfigreader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/logdatawriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/periodictimer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/zmq_led_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/zmq_param.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 11:12:22.000000 cfclient-2023.6rc1/src/cfclient/version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.497643 cfclient-2023.6rc1/src/cfclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-31 11:12:22.000000 cfclient-2023.6rc1/src/cfclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-31 11:12:22.000000 cfclient-2023.6rc1/src/cfclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:12:22.000000 cfclient-2023.6rc1/src/cfclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-31 11:12:22.000000 cfclient-2023.6rc1/src/cfclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-31 11:12:22.000000 cfclient-2023.6rc1/src/cfclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 11:12:22.000000 cfclient-2023.6rc1/src/cfclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.509643 cfclient-2023.6rc1/src/cfloader/
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfloader/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.509643 cfclient-2023.6rc1/src/cfzmq/
--rw-r--r--   0 runner    (1001) docker     (123)    14025 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfzmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfzmq/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.582404 cfclient-2023.6rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-31 13:45:42.582404 cfclient-2023.6rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/gitversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:45:42.582404 cfclient-2023.6rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.570404 cfclient-2023.6rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.570404 cfclient-2023.6rc2/src/cfclient/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.570404 cfclient-2023.6rc2/src/cfclient/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/configs/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.570404 cfclient-2023.6rc2/src/cfclient/configs/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/configs/input/Generic_OS_X.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/configs/input/Joystick.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/configs/input/PS3_Mode_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/configs/input/PS3_Mode_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/configs/input/PS3_Mode_3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/configs/input/PS4_Mode_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/configs/input/PS4_Mode_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/configs/input/PS4_shoulder_btns_yaw.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/configs/input/xbox360_mode1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.570404 cfclient-2023.6rc2/src/cfclient/configs/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/configs/log/stabilizer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/headless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.570404 cfclient-2023.6rc2/src/cfclient/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   123763 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/resources/log_param_doc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/resources/map.html
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/resources/map.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.574404 cfclient-2023.6rc2/src/cfclient/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/connectivity_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.574404 cfclient-2023.6rc2/src/cfclient/ui/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/about.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/anchor_position_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/anchor_position_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/basestation_mode_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/basestation_mode_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    22297 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/bootloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/bootloader.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/cf2config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/cf2config.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    17902 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/inputconfigdialogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24426 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/inputconfigdialogue.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/lighthouse_bs_geometry_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/lighthouse_bs_geometry_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/lighthouse_system_type_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/lighthouse_system_type_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    22514 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/logconfigdialogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/dialogs/logconfigdialogue.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.574404 cfclient-2023.6rc2/src/cfclient/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/icons/checkmark_black.png
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/icons/checkmark_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/icons/create.png
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/icons/delete.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/icons/icon-256.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36940 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16092 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/main.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/pluginhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/pose_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tab_toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.578405 cfclient-2023.6rc2/src/cfclient/ui/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/ConsoleTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/CrtpSharkToolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/ExampleTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34668 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/FlightTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/GpsTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/LEDTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/LogBlockDebugTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/LogBlockTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/LogClientTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/LogTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15379 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/ParamTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/PlotTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57266 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/QualisysTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/TuningTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/consoleTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/crtpSharkToolbox.ui
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/exampleTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/flightActionContainer.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    40263 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/flightTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/gpsTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/ledTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    27424 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/lighthouse_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/lighthouse_tab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    31493 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/locopositioning_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16370 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/locopositioning_tab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/logBlockDebugTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/logBlockTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/logClientTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/logTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/paramTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/plotTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    32634 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/qualisysTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    26596 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/tabs/tuningTab.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.578405 cfclient-2023.6rc2/src/cfclient/ui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/widgets/ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/widgets/hexspinbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/widgets/plotter.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/widgets/plotwidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-05-31 13:45:29.000000 cfclient-2023.6rc2/src/cfclient/ui/widgets/super_slider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.582404 cfclient-2023.6rc2/src/cfclient/ui/wizards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/ui/wizards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/ui/wizards/bslh_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/ui/wizards/bslh_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/ui/wizards/bslh_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13664 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/ui/wizards/bslh_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/ui/wizards/bslh_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/ui/wizards/lighthouse_geo_bs_estimation_wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.582404 cfclient-2023.6rc2/src/cfclient/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/config_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.582404 cfclient-2023.6rc2/src/cfclient/utils/input/
+-rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/input/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.582404 cfclient-2023.6rc2/src/cfclient/utils/input/inputinterfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/input/inputinterfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/input/inputinterfaces/leapmotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/input/inputinterfaces/wiimote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/input/inputinterfaces/zmqpull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/input/inputreaderinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.582404 cfclient-2023.6rc2/src/cfclient/utils/input/inputreaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/input/inputreaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/input/inputreaders/linuxjsdev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/input/inputreaders/pysdl2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.582404 cfclient-2023.6rc2/src/cfclient/utils/input/mux/
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/input/mux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/input/mux/nomux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/input/mux/takeovermux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/input/mux/takeoverselectivemux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/logconfigreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/logdatawriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/periodictimer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/zmq_led_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfclient/utils/zmq_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 13:45:42.000000 cfclient-2023.6rc2/src/cfclient/version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.570404 cfclient-2023.6rc2/src/cfclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-31 13:45:42.000000 cfclient-2023.6rc2/src/cfclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-31 13:45:42.000000 cfclient-2023.6rc2/src/cfclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:45:42.000000 cfclient-2023.6rc2/src/cfclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-31 13:45:42.000000 cfclient-2023.6rc2/src/cfclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-31 13:45:42.000000 cfclient-2023.6rc2/src/cfclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 13:45:42.000000 cfclient-2023.6rc2/src/cfclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.582404 cfclient-2023.6rc2/src/cfloader/
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfloader/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:45:42.582404 cfclient-2023.6rc2/src/cfzmq/
+-rw-r--r--   0 runner    (1001) docker     (123)    14025 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfzmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 13:45:30.000000 cfclient-2023.6rc2/src/cfzmq/__main__.py
```

### Comparing `cfclient-2023.6rc1/LICENSE.txt` & `cfclient-2023.6rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/PKG-INFO` & `cfclient-2023.6rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfclient
-Version: 2023.6rc1
+Version: 2023.6rc2
 Summary: Bitcraze Cazyflie quadcopter client
 Home-page: http://www.bitcraze.io
 Author: Bitcraze team
 Author-email: contact@bitcraze.se
 Keywords: quadcopter crazyflie
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `cfclient-2023.6rc1/README.md` & `cfclient-2023.6rc2/README.md`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/gitversion.py` & `cfclient-2023.6rc2/gitversion.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/setup.py` & `cfclient-2023.6rc2/setup.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/__init__.py` & `cfclient-2023.6rc2/src/cfclient/__init__.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/configs/config.json` & `cfclient-2023.6rc2/src/cfclient/configs/config.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/configs/input/Generic_OS_X.json` & `cfclient-2023.6rc2/src/cfclient/configs/input/Generic_OS_X.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/configs/input/Joystick.json` & `cfclient-2023.6rc2/src/cfclient/configs/input/Joystick.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/configs/input/PS3_Mode_1.json` & `cfclient-2023.6rc2/src/cfclient/configs/input/PS3_Mode_1.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/configs/input/PS3_Mode_2.json` & `cfclient-2023.6rc2/src/cfclient/configs/input/PS3_Mode_2.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/configs/input/PS3_Mode_3.json` & `cfclient-2023.6rc2/src/cfclient/configs/input/PS3_Mode_3.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/configs/input/PS4_Mode_1.json` & `cfclient-2023.6rc2/src/cfclient/configs/input/PS4_Mode_1.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/configs/input/PS4_Mode_2.json` & `cfclient-2023.6rc2/src/cfclient/configs/input/PS4_Mode_2.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/configs/input/PS4_shoulder_btns_yaw.json` & `cfclient-2023.6rc2/src/cfclient/configs/input/PS4_shoulder_btns_yaw.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/configs/input/xbox360_mode1.json` & `cfclient-2023.6rc2/src/cfclient/configs/input/xbox360_mode1.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/gui.py` & `cfclient-2023.6rc2/src/cfclient/gui.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/headless.py` & `cfclient-2023.6rc2/src/cfclient/headless.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/resources/log_param_doc.json` & `cfclient-2023.6rc2/src/cfclient/resources/log_param_doc.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/resources/map.js` & `cfclient-2023.6rc2/src/cfclient/resources/map.js`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/__init__.py` & `cfclient-2023.6rc2/src/cfclient/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/connectivity_manager.py` & `cfclient-2023.6rc2/src/cfclient/ui/connectivity_manager.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/about.py` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/about.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/about.ui` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/about.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/anchor_position_dialog.py` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/anchor_position_dialog.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/anchor_position_dialog.ui` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/anchor_position_dialog.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/basestation_mode_dialog.py` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/basestation_mode_dialog.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/basestation_mode_dialog.ui` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/basestation_mode_dialog.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/bootloader.py` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/bootloader.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/bootloader.ui` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/bootloader.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/cf2config.py` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/cf2config.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/cf2config.ui` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/cf2config.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/inputconfigdialogue.py` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/inputconfigdialogue.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/inputconfigdialogue.ui` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/inputconfigdialogue.ui`

 * *Files 1% similar despite different names*

#### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/inputconfigdialogue.ui` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/inputconfigdialogue.ui`

```diff
@@ -608,15 +608,15 @@
                       </item>
                       <item row="2" column="0">
                         <widget class="QCheckBox" name="killswitch">
                           <property name="enabled">
                             <bool>false</bool>
                           </property>
                           <property name="text">
-                            <string>Disarm/kill</string>
+                            <string>Emergency stop</string>
                           </property>
                           <property name="checkable">
                             <bool>true</bool>
                           </property>
                         </widget>
                       </item>
                       <item row="7" column="1">
@@ -651,15 +651,15 @@
                       </item>
                       <item row="3" column="0">
                         <widget class="QCheckBox" name="arm">
                           <property name="enabled">
                             <bool>false</bool>
                           </property>
                           <property name="text">
-                            <string>Arm</string>
+                            <string>Arm/disarm</string>
                           </property>
                           <property name="checkable">
                             <bool>true</bool>
                           </property>
                         </widget>
                       </item>
                       <item row="3" column="1">
```

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/lighthouse_bs_geometry_dialog.py` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/lighthouse_bs_geometry_dialog.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/lighthouse_bs_geometry_dialog.ui` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/lighthouse_bs_geometry_dialog.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/lighthouse_system_type_dialog.py` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/lighthouse_system_type_dialog.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/lighthouse_system_type_dialog.ui` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/lighthouse_system_type_dialog.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/logconfigdialogue.py` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/logconfigdialogue.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/dialogs/logconfigdialogue.ui` & `cfclient-2023.6rc2/src/cfclient/ui/dialogs/logconfigdialogue.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/icons/create.png` & `cfclient-2023.6rc2/src/cfclient/ui/icons/create.png`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/icons/icon-256.png` & `cfclient-2023.6rc2/src/cfclient/ui/icons/icon-256.png`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/main.py` & `cfclient-2023.6rc2/src/cfclient/ui/main.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/main.ui` & `cfclient-2023.6rc2/src/cfclient/ui/main.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/pluginhelper.py` & `cfclient-2023.6rc2/src/cfclient/ui/pluginhelper.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/pose_logger.py` & `cfclient-2023.6rc2/src/cfclient/ui/pose_logger.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tab_toolbox.py` & `cfclient-2023.6rc2/src/cfclient/ui/tab_toolbox.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/ConsoleTab.py` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/ConsoleTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/CrtpSharkToolbox.py` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/CrtpSharkToolbox.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/ExampleTab.py` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/ExampleTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/FlightTab.py` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/FlightTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/GpsTab.py` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/GpsTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/LEDTab.py` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/LEDTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/LogBlockDebugTab.py` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/LogBlockDebugTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/LogBlockTab.py` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/LogBlockTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/LogClientTab.py` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/LogClientTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/LogTab.py` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/LogTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/ParamTab.py` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/ParamTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/PlotTab.py` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/PlotTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/QualisysTab.py` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/QualisysTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/TuningTab.py` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/TuningTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/__init__.py` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/__init__.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/consoleTab.ui` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/consoleTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/crtpSharkToolbox.ui` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/crtpSharkToolbox.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/flightActionContainer.ui` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/flightActionContainer.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/flightTab.ui` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/flightTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/gpsTab.ui` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/gpsTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/ledTab.ui` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/ledTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/lighthouse_tab.py` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/lighthouse_tab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/lighthouse_tab.ui` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/lighthouse_tab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/locopositioning_tab.py` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/locopositioning_tab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/locopositioning_tab.ui` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/locopositioning_tab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/logBlockDebugTab.ui` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/logBlockDebugTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/logBlockTab.ui` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/logBlockTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/logClientTab.ui` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/logClientTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/logTab.ui` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/logTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/paramTab.ui` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/paramTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/plotTab.ui` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/plotTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/qualisysTab.ui` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/qualisysTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/tabs/tuningTab.ui` & `cfclient-2023.6rc2/src/cfclient/ui/tabs/tuningTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/widgets/__init__.py` & `cfclient-2023.6rc2/src/cfclient/ui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/widgets/ai.py` & `cfclient-2023.6rc2/src/cfclient/ui/widgets/ai.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/widgets/hexspinbox.py` & `cfclient-2023.6rc2/src/cfclient/ui/widgets/hexspinbox.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/widgets/plotter.ui` & `cfclient-2023.6rc2/src/cfclient/ui/widgets/plotter.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/widgets/plotwidget.py` & `cfclient-2023.6rc2/src/cfclient/ui/widgets/plotwidget.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/widgets/super_slider.py` & `cfclient-2023.6rc2/src/cfclient/ui/widgets/super_slider.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_1.png` & `cfclient-2023.6rc2/src/cfclient/ui/wizards/bslh_1.png`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_2.png` & `cfclient-2023.6rc2/src/cfclient/ui/wizards/bslh_2.png`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_3.png` & `cfclient-2023.6rc2/src/cfclient/ui/wizards/bslh_3.png`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_4.png` & `cfclient-2023.6rc2/src/cfclient/ui/wizards/bslh_4.png`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_5.png` & `cfclient-2023.6rc2/src/cfclient/ui/wizards/bslh_5.png`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/ui/wizards/lighthouse_geo_bs_estimation_wizard.py` & `cfclient-2023.6rc2/src/cfclient/ui/wizards/lighthouse_geo_bs_estimation_wizard.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/__init__.py` & `cfclient-2023.6rc2/src/cfclient/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/config.py` & `cfclient-2023.6rc2/src/cfclient/utils/config.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/config_manager.py` & `cfclient-2023.6rc2/src/cfclient/utils/config_manager.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/input/__init__.py` & `cfclient-2023.6rc2/src/cfclient/utils/input/__init__.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/input/inputinterfaces/__init__.py` & `cfclient-2023.6rc2/src/cfclient/utils/input/inputinterfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/input/inputinterfaces/leapmotion.py` & `cfclient-2023.6rc2/src/cfclient/utils/input/inputinterfaces/leapmotion.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/input/inputinterfaces/wiimote.py` & `cfclient-2023.6rc2/src/cfclient/utils/input/inputinterfaces/wiimote.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/input/inputinterfaces/zmqpull.py` & `cfclient-2023.6rc2/src/cfclient/utils/input/inputinterfaces/zmqpull.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/input/inputreaderinterface.py` & `cfclient-2023.6rc2/src/cfclient/utils/input/inputreaderinterface.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/input/inputreaders/__init__.py` & `cfclient-2023.6rc2/src/cfclient/utils/input/inputreaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/input/inputreaders/linuxjsdev.py` & `cfclient-2023.6rc2/src/cfclient/utils/input/inputreaders/linuxjsdev.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/input/inputreaders/pysdl2.py` & `cfclient-2023.6rc2/src/cfclient/utils/input/inputreaders/pysdl2.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/input/mux/__init__.py` & `cfclient-2023.6rc2/src/cfclient/utils/input/mux/__init__.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/input/mux/nomux.py` & `cfclient-2023.6rc2/src/cfclient/utils/input/mux/nomux.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/input/mux/takeovermux.py` & `cfclient-2023.6rc2/src/cfclient/utils/input/mux/takeovermux.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/input/mux/takeoverselectivemux.py` & `cfclient-2023.6rc2/src/cfclient/utils/input/mux/takeoverselectivemux.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/logconfigreader.py` & `cfclient-2023.6rc2/src/cfclient/utils/logconfigreader.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/logdatawriter.py` & `cfclient-2023.6rc2/src/cfclient/utils/logdatawriter.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/periodictimer.py` & `cfclient-2023.6rc2/src/cfclient/utils/periodictimer.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/singleton.py` & `cfclient-2023.6rc2/src/cfclient/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/ui.py` & `cfclient-2023.6rc2/src/cfclient/utils/ui.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/zmq_led_driver.py` & `cfclient-2023.6rc2/src/cfclient/utils/zmq_led_driver.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient/utils/zmq_param.py` & `cfclient-2023.6rc2/src/cfclient/utils/zmq_param.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfclient.egg-info/PKG-INFO` & `cfclient-2023.6rc2/src/cfclient.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfclient
-Version: 2023.6rc1
+Version: 2023.6rc2
 Summary: Bitcraze Cazyflie quadcopter client
 Home-page: http://www.bitcraze.io
 Author: Bitcraze team
 Author-email: contact@bitcraze.se
 Keywords: quadcopter crazyflie
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `cfclient-2023.6rc1/src/cfclient.egg-info/SOURCES.txt` & `cfclient-2023.6rc2/src/cfclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfloader/__init__.py` & `cfclient-2023.6rc2/src/cfloader/__init__.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.6rc1/src/cfzmq/__init__.py` & `cfclient-2023.6rc2/src/cfzmq/__init__.py`

 * *Files identical despite different names*

