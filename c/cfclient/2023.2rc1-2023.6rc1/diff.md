# Comparing `tmp/cfclient-2023.2rc1.tar.gz` & `tmp/cfclient-2023.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfclient-2023.2rc1.tar", last modified: Mon Feb 20 15:06:41 2023, max compression
+gzip compressed data, was "cfclient-2023.6rc1.tar", last modified: Wed May 31 11:12:22 2023, max compression
```

## Comparing `cfclient-2023.2rc1.tar` & `cfclient-2023.6rc1.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.534717 cfclient-2023.2rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-02-20 15:06:41.534717 cfclient-2023.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/gitversion.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 15:06:41.534717 cfclient-2023.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.514717 cfclient-2023.2rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.514717 cfclient-2023.2rc1/src/cfclient/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.514717 cfclient-2023.2rc1/src/cfclient/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/configs/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.518717 cfclient-2023.2rc1/src/cfclient/configs/input/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/configs/input/Generic_OS_X.json
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/configs/input/Joystick.json
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/configs/input/PS3_Mode_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/configs/input/PS3_Mode_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/configs/input/PS3_Mode_3.json
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/configs/input/PS4_Mode_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/configs/input/PS4_Mode_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/configs/input/PS4_shoulder_btns_yaw.json
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/configs/input/xbox360_mode1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.518717 cfclient-2023.2rc1/src/cfclient/configs/log/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/configs/log/stabilizer.json
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/headless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.518717 cfclient-2023.2rc1/src/cfclient/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   122832 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/resources/log_param_doc.json
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/resources/map.html
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/resources/map.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.518717 cfclient-2023.2rc1/src/cfclient/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/connectivity_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.522717 cfclient-2023.2rc1/src/cfclient/ui/dialogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/about.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/about.ui
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/anchor_position_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/anchor_position_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/basestation_mode_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/basestation_mode_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)    22297 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/bootloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/bootloader.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/cf2config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/cf2config.ui
--rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/inputconfigdialogue.py
--rw-r--r--   0 runner    (1001) docker     (123)    23664 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/inputconfigdialogue.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/lighthouse_bs_geometry_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/lighthouse_bs_geometry_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/lighthouse_system_type_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/lighthouse_system_type_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)    22514 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/logconfigdialogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/dialogs/logconfigdialogue.ui
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.522717 cfclient-2023.2rc1/src/cfclient/ui/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/icons/checkmark_black.png
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/icons/checkmark_white.png
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/icons/create.png
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/icons/delete.png
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/icons/icon-256.png
--rw-r--r--   0 runner    (1001) docker     (123)    36273 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    14436 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/main.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/pluginhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/pose_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tab_toolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.526717 cfclient-2023.2rc1/src/cfclient/ui/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/ConsoleTab.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/CrtpSharkToolbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/ExampleTab.py
--rw-r--r--   0 runner    (1001) docker     (123)    31179 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/FlightTab.py
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/GpsTab.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/LEDTab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/LogBlockDebugTab.py
--rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/LogBlockTab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/LogClientTab.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/LogTab.py
--rw-r--r--   0 runner    (1001) docker     (123)    15379 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/ParamTab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/PlotTab.py
--rw-r--r--   0 runner    (1001) docker     (123)    57265 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/QualisysTab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/TuningTab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/consoleTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/crtpSharkToolbox.ui
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/exampleTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/flightActionContainer.ui
--rw-r--r--   0 runner    (1001) docker     (123)    36859 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/flightTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/gpsTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/ledTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)    27423 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/lighthouse_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/lighthouse_tab.ui
--rw-r--r--   0 runner    (1001) docker     (123)    31489 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/locopositioning_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    16370 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/locopositioning_tab.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/logBlockDebugTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/logBlockTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/logClientTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/logTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/paramTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/plotTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)    32634 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/qualisysTab.ui
--rw-r--r--   0 runner    (1001) docker     (123)    26596 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/tabs/tuningTab.ui
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.526717 cfclient-2023.2rc1/src/cfclient/ui/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/widgets/ai.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/widgets/hexspinbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/widgets/plotter.ui
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/widgets/plotwidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/widgets/super_slider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.530717 cfclient-2023.2rc1/src/cfclient/ui/wizards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/wizards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/wizards/bslh_1.png
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/wizards/bslh_2.png
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/wizards/bslh_3.png
--rw-r--r--   0 runner    (1001) docker     (123)    13664 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/wizards/bslh_4.png
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/wizards/bslh_5.png
--rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/ui/wizards/lighthouse_geo_bs_estimation_wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.530717 cfclient-2023.2rc1/src/cfclient/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/config_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.530717 cfclient-2023.2rc1/src/cfclient/utils/input/
--rw-r--r--   0 runner    (1001) docker     (123)    22101 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/input/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.534717 cfclient-2023.2rc1/src/cfclient/utils/input/inputinterfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/input/inputinterfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/input/inputinterfaces/leapmotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/input/inputinterfaces/wiimote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/input/inputinterfaces/zmqpull.py
--rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/input/inputreaderinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.534717 cfclient-2023.2rc1/src/cfclient/utils/input/inputreaders/
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/input/inputreaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/input/inputreaders/linuxjsdev.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/input/inputreaders/pysdl2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.534717 cfclient-2023.2rc1/src/cfclient/utils/input/mux/
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/input/mux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/input/mux/nomux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/input/mux/takeovermux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/input/mux/takeoverselectivemux.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/logconfigreader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/logdatawriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/periodictimer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/zmq_led_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfclient/utils/zmq_param.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-20 15:06:41.000000 cfclient-2023.2rc1/src/cfclient/version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.514717 cfclient-2023.2rc1/src/cfclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-02-20 15:06:41.000000 cfclient-2023.2rc1/src/cfclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-02-20 15:06:41.000000 cfclient-2023.2rc1/src/cfclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 15:06:41.000000 cfclient-2023.2rc1/src/cfclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-02-20 15:06:41.000000 cfclient-2023.2rc1/src/cfclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-20 15:06:41.000000 cfclient-2023.2rc1/src/cfclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-20 15:06:41.000000 cfclient-2023.2rc1/src/cfclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.534717 cfclient-2023.2rc1/src/cfloader/
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfloader/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 15:06:41.534717 cfclient-2023.2rc1/src/cfzmq/
--rw-r--r--   0 runner    (1001) docker     (123)    14025 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfzmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-20 15:06:29.000000 cfclient-2023.2rc1/src/cfzmq/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.509643 cfclient-2023.6rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-31 11:12:22.509643 cfclient-2023.6rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/gitversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 11:12:22.509643 cfclient-2023.6rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.493643 cfclient-2023.6rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.493643 cfclient-2023.6rc1/src/cfclient/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.497643 cfclient-2023.6rc1/src/cfclient/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.497643 cfclient-2023.6rc1/src/cfclient/configs/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/input/Generic_OS_X.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/input/Joystick.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/input/PS3_Mode_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/input/PS3_Mode_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/input/PS3_Mode_3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/input/PS4_Mode_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/input/PS4_Mode_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/input/PS4_shoulder_btns_yaw.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/input/xbox360_mode1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.497643 cfclient-2023.6rc1/src/cfclient/configs/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/configs/log/stabilizer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/headless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.497643 cfclient-2023.6rc1/src/cfclient/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   123763 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/resources/log_param_doc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/resources/map.html
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/resources/map.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.497643 cfclient-2023.6rc1/src/cfclient/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/connectivity_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.501643 cfclient-2023.6rc1/src/cfclient/ui/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/about.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/anchor_position_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/anchor_position_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/basestation_mode_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/basestation_mode_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    22297 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/bootloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/bootloader.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/cf2config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/cf2config.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    17902 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/inputconfigdialogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24416 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/inputconfigdialogue.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/lighthouse_bs_geometry_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/lighthouse_bs_geometry_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/lighthouse_system_type_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/lighthouse_system_type_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    22514 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/logconfigdialogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9128 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/dialogs/logconfigdialogue.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.501643 cfclient-2023.6rc1/src/cfclient/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/icons/checkmark_black.png
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/icons/checkmark_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/icons/create.png
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/icons/delete.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/icons/icon-256.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36940 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16092 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/main.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/pluginhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/pose_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tab_toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.505643 cfclient-2023.6rc1/src/cfclient/ui/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/ConsoleTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/CrtpSharkToolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/ExampleTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34668 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/FlightTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/GpsTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/LEDTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/LogBlockDebugTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/LogBlockTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/LogClientTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/LogTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15379 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/ParamTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/PlotTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57266 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/QualisysTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/TuningTab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/consoleTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/crtpSharkToolbox.ui
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/exampleTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/flightActionContainer.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    40263 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/flightTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/gpsTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/ledTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    27424 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/lighthouse_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15349 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/lighthouse_tab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    31493 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/locopositioning_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16370 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/locopositioning_tab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/logBlockDebugTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/logBlockTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/logClientTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/logTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/paramTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/plotTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    32634 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/qualisysTab.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    26596 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/tabs/tuningTab.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.505643 cfclient-2023.6rc1/src/cfclient/ui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/widgets/ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/widgets/hexspinbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/widgets/plotter.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/widgets/plotwidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/widgets/super_slider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.505643 cfclient-2023.6rc1/src/cfclient/ui/wizards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/wizards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13664 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_4.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_5.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/ui/wizards/lighthouse_geo_bs_estimation_wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.505643 cfclient-2023.6rc1/src/cfclient/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/config_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.505643 cfclient-2023.6rc1/src/cfclient/utils/input/
+-rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.509643 cfclient-2023.6rc1/src/cfclient/utils/input/inputinterfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/inputinterfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/inputinterfaces/leapmotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/inputinterfaces/wiimote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/inputinterfaces/zmqpull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/inputreaderinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.509643 cfclient-2023.6rc1/src/cfclient/utils/input/inputreaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/inputreaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/inputreaders/linuxjsdev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/inputreaders/pysdl2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.509643 cfclient-2023.6rc1/src/cfclient/utils/input/mux/
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/mux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/mux/nomux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/mux/takeovermux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/input/mux/takeoverselectivemux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/logconfigreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/logdatawriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/periodictimer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/zmq_led_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfclient/utils/zmq_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 11:12:22.000000 cfclient-2023.6rc1/src/cfclient/version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.497643 cfclient-2023.6rc1/src/cfclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-31 11:12:22.000000 cfclient-2023.6rc1/src/cfclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-31 11:12:22.000000 cfclient-2023.6rc1/src/cfclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:12:22.000000 cfclient-2023.6rc1/src/cfclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-31 11:12:22.000000 cfclient-2023.6rc1/src/cfclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-31 11:12:22.000000 cfclient-2023.6rc1/src/cfclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 11:12:22.000000 cfclient-2023.6rc1/src/cfclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.509643 cfclient-2023.6rc1/src/cfloader/
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfloader/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:12:22.509643 cfclient-2023.6rc1/src/cfzmq/
+-rw-r--r--   0 runner    (1001) docker     (123)    14025 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfzmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 11:12:07.000000 cfclient-2023.6rc1/src/cfzmq/__main__.py
```

### Comparing `cfclient-2023.2rc1/LICENSE.txt` & `cfclient-2023.6rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/PKG-INFO` & `cfclient-2023.6rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfclient
-Version: 2023.2rc1
+Version: 2023.6rc1
 Summary: Bitcraze Cazyflie quadcopter client
 Home-page: http://www.bitcraze.io
 Author: Bitcraze team
 Author-email: contact@bitcraze.se
 Keywords: quadcopter crazyflie
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `cfclient-2023.2rc1/README.md` & `cfclient-2023.6rc1/README.md`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/gitversion.py` & `cfclient-2023.6rc1/gitversion.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/setup.py` & `cfclient-2023.6rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,17 +86,17 @@
             'cfclient=cfclient.gui:main',
             'cfheadless=cfclient.headless:main',
             'cfloader=cfloader:main',
             'cfzmq=cfzmq:main'
         ],
     },
 
-    install_requires=['cflib>=0.1.21',
+    install_requires=['cflib>=0.1.23',
                       'appdirs~=1.4.0',
-                      'pyzmq~=22.3',
+                      'pyzmq~=25.0',
                       'pyqtgraph~=0.11',
                       'PyYAML~=5.3',
                       'qasync~=0.23.0',
                       'qtm~=2.1.1',
                       'numpy>=1.20,<1.25',
                       'vispy~=0.9.0',
                       'pyserial~=3.5',
```

### Comparing `cfclient-2023.2rc1/src/cfclient/__init__.py` & `cfclient-2023.6rc1/src/cfclient/__init__.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/configs/config.json` & `cfclient-2023.6rc1/src/cfclient/configs/config.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/configs/input/Generic_OS_X.json` & `cfclient-2023.6rc1/src/cfclient/configs/input/Generic_OS_X.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/configs/input/Joystick.json` & `cfclient-2023.6rc1/src/cfclient/configs/input/Joystick.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/configs/input/PS3_Mode_1.json` & `cfclient-2023.6rc1/src/cfclient/configs/input/PS3_Mode_1.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/configs/input/PS3_Mode_2.json` & `cfclient-2023.6rc1/src/cfclient/configs/input/PS3_Mode_2.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/configs/input/PS3_Mode_3.json` & `cfclient-2023.6rc1/src/cfclient/configs/input/PS3_Mode_3.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/configs/input/PS4_Mode_1.json` & `cfclient-2023.6rc1/src/cfclient/configs/input/PS4_Mode_1.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/configs/input/PS4_Mode_2.json` & `cfclient-2023.6rc1/src/cfclient/configs/input/PS4_Mode_2.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/configs/input/PS4_shoulder_btns_yaw.json` & `cfclient-2023.6rc1/src/cfclient/configs/input/PS4_shoulder_btns_yaw.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/configs/input/xbox360_mode1.json` & `cfclient-2023.6rc1/src/cfclient/configs/input/xbox360_mode1.json`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/gui.py` & `cfclient-2023.6rc1/src/cfclient/gui.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/headless.py` & `cfclient-2023.6rc1/src/cfclient/headless.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/resources/log_param_doc.json` & `cfclient-2023.6rc1/src/cfclient/resources/log_param_doc.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9887492791215142%*

 * *Differences: {"'logs'": "{'lighthouse': {'variables': {'rawAngle0xlh2': {'desc': '|\\xa0Base station type "*

 * *           '|\\xa0V1 |\\n| Base station | primary |\\n| Sweep |\\xa01 |\\n| Sensor | 1 |\\n\\n If '*

 * *           'a base station of type V2 is used, this will contain the V2 angles converted to V1 '*

 * *           'style for the base station with channel 1.\\n\\nThe V1 angle received by sensor 1, '*

 * *           'corrected using calibration data [rad]\\n\\n|\\xa0Base station type |\\xa0V1 |\\n| '*

 * *           'Base station | […]*

```diff
@@ -1298,15 +1298,15 @@
                     "core": false,
                     "desc": "|\u00a0Base station type |\u00a0V1 |\n| Base station | primary |\n| Sweep |\u00a01 |\n| Sensor | 0 |\n",
                     "short_desc": "The raw V1 angle received by sensor 0 [rad]. ",
                     "type": "LOG_FLOAT"
                 },
                 "rawAngle0xlh2": {
                     "core": false,
-                    "desc": "|\u00a0Base station type |\u00a0V1 |\n| Base station | primary |\n| Sweep |\u00a01 |\n| Sensor | 1 |\n\n If a base station of type V2 is used, this will contain the V2 angles converted to V1 style for the base station with channel 1. The V1 angle received by sensor 1, corrected using calibration data [rad]\n\n|\u00a0Base station type |\u00a0V1 |\n| Base station | primary |\n| Sweep |\u00a02 |\n| Sensor | 1 |\n\n If a base station of type V2 is used, this will contain the V2 angles converted to V1 style for the base station with channel 1. The V1 angle received by sensor 1, corrected using calibration data [rad]\n\n|\u00a0Base station type |\u00a0V1 |\n| Base station | secondary |\n| Sweep |\u00a01 |\n| Sensor | 1 |\n\n If a base station of type V2 is used, this will contain the V2 angles converted to V1 style for the base station with channel 2. The V1 angle received by sensor 1, corrected using calibration data [rad]\n\n|\u00a0Base station type |\u00a0V1 |\n| Base station | secondary |\n| Sweep |\u00a02 |\n| Sensor | 1 |\n\n If a base station of type V2 is used, this will contain the V2 angles converted to V1 style for the base station with channel 2. The raw V2 angle received by sensor 0 [rad]\n\n|\u00a0Base station type |\u00a0V2 |\n| Channel | 1 |\n| Sweep |\u00a01 |\n| Sensor | 0 |\n",
+                    "desc": "|\u00a0Base station type |\u00a0V1 |\n| Base station | primary |\n| Sweep |\u00a01 |\n| Sensor | 1 |\n\n If a base station of type V2 is used, this will contain the V2 angles converted to V1 style for the base station with channel 1.\n\nThe V1 angle received by sensor 1, corrected using calibration data [rad]\n\n|\u00a0Base station type |\u00a0V1 |\n| Base station | primary |\n| Sweep |\u00a02 |\n| Sensor | 1 |\n\n If a base station of type V2 is used, this will contain the V2 angles converted to V1 style for the base station with channel 1.\n\nThe V1 angle received by sensor 1, corrected using calibration data [rad]\n\n|\u00a0Base station type |\u00a0V1 |\n| Base station | secondary |\n| Sweep |\u00a01 |\n| Sensor | 1 |\n\n If a base station of type V2 is used, this will contain the V2 angles converted to V1 style for the base station with channel 2.\n\nThe V1 angle received by sensor 1, corrected using calibration data [rad]\n\n|\u00a0Base station type |\u00a0V1 |\n| Base station | secondary |\n| Sweep |\u00a02 |\n| Sensor | 1 |\n\n If a base station of type V2 is used, this will contain the V2 angles converted to V1 style for the base station with channel 2.\n\nThe raw V2 angle received by sensor 0 [rad]\n\n|\u00a0Base station type |\u00a0V2 |\n| Channel | 1 |\n| Sweep |\u00a01 |\n| Sensor | 0 |\n",
                     "short_desc": "The angle received by sensor 1, corrected using calibration data [rad]. ",
                     "type": "LOG_FLOAT"
                 },
                 "rawAngle0y": {
                     "core": false,
                     "desc": "|\u00a0Base station type |\u00a0V1 |\n| Base station | primary |\n| Sweep |\u00a02 |\n| Sensor | 0 |\n",
                     "short_desc": "The raw V1 angle received by sensor 0 [rad]. ",
@@ -1340,15 +1340,15 @@
                     "core": false,
                     "desc": "|\u00a0Base station type |\u00a0V2 |\n| Channel | 2 |\n| Sweep |\u00a02 |\n| Sensor | 0 |\n",
                     "short_desc": "The raw V2 angle received by sensor 0 [rad]. ",
                     "type": "LOG_FLOAT"
                 },
                 "status": {
                     "core": true,
-                    "desc": "|\u00a0Value |\u00a0Meaning |\n| - | - |\n| 0 | No lighthouse base stations are recevied |\n| 1 | One or more base stations are received but geometry or callibration data is missing |\n| 2 | Base station data is sent to the state estimator |\n ",
+                    "desc": "|\u00a0Value |\u00a0Meaning |\n| - | - |\n| 0 | No lighthouse base stations are recevied |\n| 1 | One or more base stations are received but geometry or callibration data is missing |\n| 2 | Base station data is sent to the state estimator |\n",
                     "short_desc": "Overall status of the lighthouse system. ",
                     "type": "LOG_UINT8"
                 },
                 "validAngles": {
                     "core": false,
                     "desc": "",
                     "short_desc": "",
@@ -1433,15 +1433,15 @@
             }
         },
         "loco": {
             "desc": "Log group for basic information about the Loco Positioning System ",
             "variables": {
                 "mode": {
                     "core": true,
-                    "desc": "| Value | Mode | \n| - | - | \n| 1 | TWR | \n| 2 | TDoA 2 | \n| 3 | TDoA 3 | \n ",
+                    "desc": "| Value | Mode | \n| - | - | \n| 1 | TWR | \n| 2 | TDoA 2 | \n| 3 | TDoA 3 | \n",
                     "short_desc": "The current mode of the Loco Positioning system. ",
                     "type": "LOG_UINT8"
                 },
                 "spiRe": {
                     "core": false,
                     "desc": "",
                     "short_desc": "",
@@ -1999,15 +1999,15 @@
                     "core": false,
                     "desc": "",
                     "short_desc": "BigQuad external voltage measurement [mV]. ",
                     "type": "LOG_UINT16"
                 },
                 "state": {
                     "core": true,
-                    "desc": "| State | Meaning | \n| - | - | \n| 0 | Battery | \n| 1 | Charging | \n| 2 | Charged | \n| 3 | Low power | \n| 4 | Shutdown | \n ",
+                    "desc": "| State | Meaning | \n| - | - | \n| 0 | Battery | \n| 1 | Charging | \n| 2 | Charged | \n| 3 | Low power | \n| 4 | Shutdown | \n",
                     "short_desc": "State of power management. ",
                     "type": "LOG_INT8"
                 },
                 "vbat": {
                     "core": true,
                     "desc": "",
                     "short_desc": "Battery voltage [V]. ",
@@ -2935,28 +2935,34 @@
                     "desc": "",
                     "short_desc": "If zero, arming system is preventing motors to start. ",
                     "type": "LOG_INT8"
                 },
                 "canfly": {
                     "core": true,
                     "desc": "",
-                    "short_desc": "If nonzero if system is ready to fly. ",
+                    "short_desc": "Nonzero if system is ready to fly. ",
                     "type": "LOG_UINT8"
                 },
                 "isFlying": {
                     "core": true,
                     "desc": "",
                     "short_desc": "Nonzero if the system thinks it is flying. ",
                     "type": "LOG_UINT8"
                 },
                 "isTumbled": {
                     "core": true,
                     "desc": "",
                     "short_desc": "Nonzero if the system thinks it is tumbled/crashed. ",
                     "type": "LOG_UINT8"
+                },
+                "testLogParam": {
+                    "core": false,
+                    "desc": "",
+                    "short_desc": "Test util for log and param. The value is set through the system.testLogParam parameter. ",
+                    "type": "LOG_INT8"
                 }
             }
         },
         "tdoa2": {
             "desc": "",
             "variables": {
                 "cc0": {
@@ -4324,15 +4330,15 @@
             }
         },
         "loco": {
             "desc": "The Loco Positioning System implements three different positioning modes: Two Way Ranging (TWR), Time Difference of Arrival 2 (TDoA 2) and Time Difference of Arrival 3 (TDoA 3)\n\n### TWR mode\n\nIn this mode, the tag pings the anchors in sequence, this allows it to measure the distance between the tag and the anchors. Using this information a theoretical minimum of 4 Anchors is required to calculate the 3D position of a Tag, but a more realistic number is 6 to add redundancy and accuracy. This mode is the most accurate mode and also works when the tag or quad leaves the space delimited by the anchors. The tag is actively communicating with the anchors in a time slotted fashion and in this mode only one tag or quad can be positioned with a maximum of 8 anchors.\n\n### TDoA 2 mode\n\nIn TDoA 2 mode, the anchor system is continuously sending synchronization packets. A tag listening to these packets can calculate the relative distance to two anchors by measuring the time difference of arrival of the packets. From the TDoA information it is possible to calculate the 3D position in space. In this mode the tag is only passively listening, so new tags do not add any load to the system which makes it possible to position any number of tags or quads simultaneously. This makes it a perfect mode for swarming.\n\nCompared to TWR, TDoA 2 is more restrictive when it comes to the space where positioning works, ideally the tag should be within, or very close to, the space delimited by the anchor system. This means that TDoA 2 works best with 8 anchors placed in the corners of the flying space. In this space the accuracy and precision is comparable to TWR.\n\nIn this mode the anchor system is time slotted and synchronized and the number of anchors is limited to 8.\n\n### TDoA 3 mode\n\nThe TDoA 3 mode has many similarities with TDoA 2 and supports any number of tags or quads. The main difference is that the time slotted scheme of TDoA 2 has been replaced by a randomized transmission schedule which makes it possible to add more anchors. By adding more anchors the system can be scaled to larger spaces or span multiple rooms without line of sight between all anchors. It also makes it more robust and can handle loss or addition of anchors dynamically. The estimated position in this mode might be slightly more noisy compared to TDoA 2. ",
             "variables": {
                 "mode": {
                     "core": true,
-                    "desc": "| Value | Mode |\n| - | - |\n| 0 | Auto |\n| 1 | TWR |\n| 2 | TDoA 2 |\n| 3 | TDoA 3 |\n ",
+                    "desc": "| Value | Mode |\n| - | - |\n| 0 | Auto |\n| 1 | TWR |\n| 2 | TDoA 2 |\n| 3 | TDoA 3 |\n",
                     "short_desc": "The Loco positioning mode to use (default: 0) ",
                     "type": "PARAM_UINT8"
                 }
             }
         },
         "memTst": {
             "desc": "",
@@ -4869,15 +4875,15 @@
             }
         },
         "ring": {
             "desc": "The LED ring expansion deck contains two powerful front-facing white LEDs and 12 bottom-facing RGB individually addressable LEDs (it uses the same LEDs as used in the NeoPixel products by Adafruit).\n\nThe deck is designed to be installed as the last deck on the bottom of the quad. It does not have pass-through holes for the expansion port connector. ",
             "variables": {
                 "effect": {
                     "core": true,
-                    "desc": "| Id | Effect | \n| - | - | \n| 0 | Off | \n| 1 | White spinner | \n| 2 | Color spinner | \n| 3 | Tilt | \n| 4 | Brightness | \n| 5 | Color spinner 2 | \n| 6 | Double spinner | \n| 7 | Solid color effect | \n| 8 | Factory test | \n| 9 | Battery status | \n| 10 | Boat lights | \n| 11 | Alert | \n| 12 | Gravity | \n| 13 | Virtual Memory | \n| 14 | Fade color | \n| 15 | Communication Signal Strength | \n| 16 | Status Localization Service | \n| 17 | LED timing from memory | \n| 18 | Lighthouse Positioning | \n ",
+                    "desc": "| Id | Effect | \n| - | - | \n| 0 | Off | \n| 1 | White spinner | \n| 2 | Color spinner | \n| 3 | Tilt | \n| 4 | Brightness | \n| 5 | Color spinner 2 | \n| 6 | Double spinner | \n| 7 | Solid color effect | \n| 8 | Factory test | \n| 9 | Battery status | \n| 10 | Boat lights | \n| 11 | Alert | \n| 12 | Gravity | \n| 13 | Virtual Memory | \n| 14 | Fade color | \n| 15 | Communication Signal Strength | \n| 16 | Status Localization Service | \n| 17 | LED timing from memory | \n| 18 | Lighthouse Positioning | \n",
                     "short_desc": "Id of effect to use (default: 6) ",
                     "type": "PARAM_UINT8, PARAM_PERSISTENT"
                 },
                 "emptyCharge": {
                     "core": true,
                     "desc": "",
                     "short_desc": "At what volt the Battery effect indicates empty. ",
@@ -4957,15 +4963,15 @@
             }
         },
         "sound": {
             "desc": "The buzzer deck contains a low profile piezo buzzer. ",
             "variables": {
                 "effect": {
                     "core": true,
-                    "desc": "| Id | Effect | \n| - | - | \n| 0 | Off | \n| 1 | Factory test | \n| 2 | USB connected | \n| 3 | USB disconnected | \n| 4 | Charging done | \n| 5 | Low battery | \n| 6 | Startup | \n| 7 | Calibrated | \n| 8 | Range slow | \n| 9 | Range fast | \n| 10 | Star Wars Imperial March | \n| 11 | Bypass | \n| 12 | Siren | \n| 13 | Tilt quad to play sound | \n ",
+                    "desc": "| Id | Effect | \n| - | - | \n| 0 | Off | \n| 1 | Factory test | \n| 2 | USB connected | \n| 3 | USB disconnected | \n| 4 | Charging done | \n| 5 | Low battery | \n| 6 | Startup | \n| 7 | Calibrated | \n| 8 | Range slow | \n| 9 | Range fast | \n| 10 | Star Wars Imperial March | \n| 11 | Bypass | \n| 12 | Siren | \n| 13 | Tilt quad to play sound | \n",
                     "short_desc": "Id of effect to use (default: 0) ",
                     "type": "PARAM_UINT8, PARAM_PERSISTENT"
                 },
                 "freq": {
                     "core": true,
                     "desc": "",
                     "short_desc": "Frequency to use for Bypass effect. ",
@@ -4976,15 +4982,15 @@
                     "desc": "",
                     "short_desc": "Number of effects available. ",
                     "type": "PARAM_UINT32, PARAM_RONLY"
                 }
             }
         },
         "stabilizer": {
-            "desc": "Parameters to set the estimator and controller type for the stabilizer module, or to do an emergency stop ",
+            "desc": "Parameters to set the estimator and controller type for the stabilizer module ",
             "variables": {
                 "controller": {
                     "core": true,
                     "desc": "",
                     "short_desc": "Controller type Auto select(0), PID(1), Mellinger(2), INDI(3), Brescianini(4) (Default: 0) ",
                     "type": "PARAM_UINT8"
                 },
@@ -4998,40 +5004,51 @@
                     "core": true,
                     "desc": "",
                     "short_desc": "If set to nonzero will turn off power. ",
                     "type": "PARAM_UINT8"
                 }
             }
         },
+        "superv": {
+            "desc": "The purpose of the supervisor is to monitor the system and its state. Depending on the situation, the supervisor can enable/disable functionality as well as take action to protect the system or humans close by. ",
+            "variables": {
+                "infdmp": {
+                    "core": false,
+                    "desc": "",
+                    "short_desc": "Set to nonzero to dump information about the current supervisor state to the console log. ",
+                    "type": "PARAM_UINT8"
+                }
+            }
+        },
         "syslink": {
             "desc": "",
             "variables": {
                 "probe": {
                     "core": false,
                     "desc": "",
                     "short_desc": "Trigger syslink debug probe in the NRF by setting to 1. ",
                     "type": "PARAM_UINT8"
                 }
             }
         },
         "system": {
             "desc": "",
             "variables": {
+                "arm": {
+                    "core": true,
+                    "desc": "",
+                    "short_desc": "Set to nonzero to arm the system. ",
+                    "type": "PARAM_INT8"
+                },
                 "assertInfo": {
                     "core": false,
                     "desc": "",
                     "short_desc": "Set to nonzero to trigger dump of assert information to the log. ",
                     "type": "PARAM_UINT8"
                 },
-                "forceArm": {
-                    "core": false,
-                    "desc": "",
-                    "short_desc": "Set to nonzero to force system to be armed. ",
-                    "type": "PARAM_INT8, PARAM_PERSISTENT"
-                },
                 "highlight": {
                     "core": true,
                     "desc": "Uses functionality available, such as LEDs to highlight a quad, useful for swarms. ",
                     "short_desc": "Highlight quad. ",
                     "type": "PARAM_UINT8"
                 },
                 "selftestPassed": {
@@ -5053,14 +5070,20 @@
                     "type": "PARAM_UINT8"
                 },
                 "taskDump": {
                     "core": true,
                     "desc": "",
                     "short_desc": "Set to nonzero to dump CPU and stack usage to console. ",
                     "type": "PARAM_UINT8"
+                },
+                "testLogParam": {
+                    "core": false,
+                    "desc": "",
+                    "short_desc": "Test util for log and param. This param sets the value of the sys.testLogParam log variable. ",
+                    "type": "PARAM_UINT8"
                 }
             }
         },
         "tdoa2": {
             "desc": "",
             "variables": {
                 "stddev": {
@@ -5237,14 +5260,25 @@
                     "core": true,
                     "desc": "",
                     "short_desc": "Controls if logging to the SD-card is active. Set to 1 to start logging, set to 0 to stop logging (default). ",
                     "type": "PARAM_UINT8"
                 }
             }
         },
+        "usec": {
+            "desc": "",
+            "variables": {
+                "reset": {
+                    "core": false,
+                    "desc": "Useful for time synchronization between UAVs, if reset is send as a broadcast. ",
+                    "short_desc": "Reset the time to zero. ",
+                    "type": "PARAM_UINT8"
+                }
+            }
+        },
         "velCtlPid": {
             "desc": "Tuning settings for the gains of the PID controller for the velocity of the Crazyflie \u00a8 in the body-yaw-aligned X & Y and global Z directions. ",
             "variables": {
                 "vxKFF": {
                     "core": false,
                     "desc": "",
                     "short_desc": "Feedforward gain for the velocity PID in the body-yaw-aligned X direction (in degrees per m/s) ",
```

### Comparing `cfclient-2023.2rc1/src/cfclient/resources/map.js` & `cfclient-2023.6rc1/src/cfclient/resources/map.js`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/__init__.py` & `cfclient-2023.6rc1/src/cfclient/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/connectivity_manager.py` & `cfclient-2023.6rc1/src/cfclient/ui/connectivity_manager.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/about.py` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/about.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/about.ui` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/about.ui`

 * *Files 1% similar despite different names*

#### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/about.ui` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/about.ui`

```diff
@@ -35,15 +35,15 @@
                   <item>
                     <layout class="QVBoxLayout" name="verticalLayout_3">
                       <item>
                         <layout class="QGridLayout" name="gridLayout_2">
                           <item row="1" column="0">
                             <widget class="QLabel" name="label_2">
                               <property name="text">
-                                <string>Copyright (c) 2011-2020, Bitcraze AB</string>
+                                <string>Copyright (c) 2011-2023, Bitcraze AB</string>
                               </property>
                             </widget>
                           </item>
                           <item row="2" column="0">
                             <widget class="QLabel" name="label">
                               <property name="text">
                                 <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;&lt;span style=&quot; font-size:12pt;&quot;&gt;The Crazyflie client is a multi-platform client&lt;br/&gt;for controlling, bootloading and logging the Crazyflie.&lt;br/&gt;For more info visit our homepage.&lt;/span&gt;&lt;/p&gt;&lt;p&gt;&lt;a href=&quot;http://www.bitcraze.io&quot;&gt;&lt;span style=&quot; text-decoration: underline; color:#0000ff;&quot;&gt;Bitcraze Homepage&lt;/span&gt;&lt;/a&gt;&lt;span style=&quot; font-size:12pt;&quot;&gt;&lt;br/&gt;&lt;/span&gt;&lt;a href=&quot;https://www.bitcraze.io/documentation/repository/crazyflie-clients-python/master/userguides/userguide_client/&quot;&gt;&lt;span style=&quot; text-decoration: underline; color:#0000ff;&quot;&gt;Client documentation&lt;/span&gt;&lt;/a&gt;&lt;span style=&quot; font-size:12pt;&quot;&gt;&lt;br/&gt;&lt;/span&gt;&lt;a href=&quot;http://discussions.bitcraze.io&quot;&gt;&lt;span style=&quot; text-decoration: underline; color:#0000ff;&quot;&gt;Bitcraze Discussions&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;&lt;p&gt;&lt;br/&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
```

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/anchor_position_dialog.py` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/anchor_position_dialog.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/anchor_position_dialog.ui` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/anchor_position_dialog.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/basestation_mode_dialog.py` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/basestation_mode_dialog.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/basestation_mode_dialog.ui` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/basestation_mode_dialog.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/bootloader.py` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/bootloader.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/bootloader.ui` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/bootloader.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/cf2config.py` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/cf2config.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/cf2config.ui` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/cf2config.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/inputconfigdialogue.py` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/inputconfigdialogue.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,16 +103,20 @@
                 "Press the button for Roll positive calibration"))
         self.detectRollNeg.clicked.connect(
             lambda: self._button_detect(
                 "rollNeg", "Roll Cal Negative",
                 "Press the button for Roll negative calibration"))
         self.detectKillswitch.clicked.connect(
             lambda: self._button_detect(
-                "killswitch", "Killswitch",
-                "Press the button for the killswitch (will disable motors)"))
+                "estop", "Disarm/Kill",
+                "Press the button to disarm/kill (will disable motors)"))
+        self.detectArm.clicked.connect(
+            lambda: self._button_detect(
+                "arm", "Arm system",
+                "Press the button to arm the system (will enable motor ouput)"))
         self.detectAlt1.clicked.connect(
             lambda: self._button_detect(
                 "alt1", "Alternative function 1",
                 "The alternative function 1 that will do a callback"))
         self.detectAlt2.clicked.connect(
             lambda: self._button_detect(
                 "alt2", "Alternative function 2",
@@ -138,17 +142,18 @@
         self._popup = None
         self._combined_button = None
         self._detection_buttons = [
             self.detectPitch, self.detectRoll,
             self.detectYaw, self.detectThrust,
             self.detectPitchPos, self.detectPitchNeg,
             self.detectRollPos, self.detectRollNeg,
-            self.detectKillswitch, self.detectExitapp,
-            self._detect_assisted_control, self.detectAlt1,
-            self.detectAlt2, self.detectMuxswitch]
+            self.detectKillswitch, self.detectArm,
+            self.detectExitapp, self._detect_assisted_control,
+            self.detectAlt1, self.detectAlt2,
+            self.detectMuxswitch]
 
         self._button_to_detect = ""
         self._axis_to_detect = ""
         self.combinedDetection = 0
         self._prev_combined_id = None
 
         self._maxed_axis = []
@@ -174,15 +179,16 @@
 
     def _reset_mapping(self):
         self._buttonindicators = {
             "pitchPos": self.pitchPos,
             "pitchNeg": self.pitchNeg,
             "rollPos": self.rollPos,
             "rollNeg": self.rollNeg,
-            "killswitch": self.killswitch,
+            "estop": self.killswitch,
+            "arm": self.arm,
             "alt1": self.alt1,
             "alt2": self.alt2,
             "exitapp": self.exitapp,
             "assistedControl": self._assisted_control,
             "muxswitch": self.muxswitch,
         }
```

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/inputconfigdialogue.ui` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/inputconfigdialogue.ui`

 * *Files 1% similar despite different names*

#### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/inputconfigdialogue.ui` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/inputconfigdialogue.ui`

```diff
@@ -501,150 +501,173 @@
                       </item>
                     </layout>
                   </widget>
                   <widget class="QWidget" name="gridLayoutWidget_2">
                     <property name="geometry">
                       <rect>
                         <x>600</x>
-                        <y>158</y>
+                        <y>150</y>
                         <width>292</width>
-                        <height>202</height>
+                        <height>221</height>
                       </rect>
                     </property>
                     <layout class="QGridLayout" name="gridLayout_5">
-                      <item row="5" column="1">
+                      <item row="6" column="1">
                         <widget class="QPushButton" name="detectAlt2">
                           <property name="enabled">
                             <bool>false</bool>
                           </property>
                           <property name="text">
                             <string>Detect</string>
                           </property>
                         </widget>
                       </item>
-                      <item row="4" column="0">
+                      <item row="2" column="1">
+                        <widget class="QPushButton" name="detectKillswitch">
+                          <property name="enabled">
+                            <bool>false</bool>
+                          </property>
+                          <property name="text">
+                            <string>Detect</string>
+                          </property>
+                        </widget>
+                      </item>
+                      <item row="7" column="0">
+                        <widget class="QCheckBox" name="muxswitch">
+                          <property name="enabled">
+                            <bool>false</bool>
+                          </property>
+                          <property name="text">
+                            <string>Mux switch</string>
+                          </property>
+                          <property name="checkable">
+                            <bool>true</bool>
+                          </property>
+                        </widget>
+                      </item>
+                      <item row="5" column="0">
                         <widget class="QCheckBox" name="alt1">
                           <property name="enabled">
                             <bool>false</bool>
                           </property>
                           <property name="text">
                             <string>Alt 1</string>
                           </property>
                           <property name="checkable">
                             <bool>true</bool>
                           </property>
                         </widget>
                       </item>
-                      <item row="3" column="1">
-                        <widget class="QPushButton" name="detectExitapp">
+                      <item row="1" column="1">
+                        <widget class="QPushButton" name="_detect_assisted_control">
                           <property name="enabled">
                             <bool>false</bool>
                           </property>
                           <property name="text">
                             <string>Detect</string>
                           </property>
                         </widget>
                       </item>
-                      <item row="2" column="1">
-                        <widget class="QPushButton" name="detectKillswitch">
+                      <item row="6" column="0">
+                        <widget class="QCheckBox" name="alt2">
                           <property name="enabled">
                             <bool>false</bool>
                           </property>
                           <property name="text">
-                            <string>Detect</string>
+                            <string>Alt 2</string>
+                          </property>
+                          <property name="checkable">
+                            <bool>true</bool>
                           </property>
                         </widget>
                       </item>
-                      <item row="2" column="0">
-                        <widget class="QCheckBox" name="killswitch">
+                      <item row="1" column="0">
+                        <widget class="QCheckBox" name="_assisted_control">
                           <property name="enabled">
                             <bool>false</bool>
                           </property>
                           <property name="text">
-                            <string>Killswitch</string>
+                            <string>Assisted control</string>
                           </property>
                           <property name="checkable">
                             <bool>true</bool>
                           </property>
                         </widget>
                       </item>
-                      <item row="3" column="0">
+                      <item row="4" column="0">
                         <widget class="QCheckBox" name="exitapp">
                           <property name="enabled">
                             <bool>false</bool>
                           </property>
                           <property name="text">
                             <string>Exit app</string>
                           </property>
                           <property name="checkable">
                             <bool>true</bool>
                           </property>
                         </widget>
                       </item>
-                      <item row="1" column="0">
-                        <widget class="QCheckBox" name="_assisted_control">
+                      <item row="2" column="0">
+                        <widget class="QCheckBox" name="killswitch">
                           <property name="enabled">
                             <bool>false</bool>
                           </property>
                           <property name="text">
-                            <string>Assisted control</string>
+                            <string>Disarm/kill</string>
                           </property>
                           <property name="checkable">
                             <bool>true</bool>
                           </property>
                         </widget>
                       </item>
-                      <item row="1" column="1">
-                        <widget class="QPushButton" name="_detect_assisted_control">
+                      <item row="7" column="1">
+                        <widget class="QPushButton" name="detectMuxswitch">
                           <property name="enabled">
                             <bool>false</bool>
                           </property>
                           <property name="text">
                             <string>Detect</string>
                           </property>
                         </widget>
                       </item>
-                      <item row="5" column="0">
-                        <widget class="QCheckBox" name="alt2">
+                      <item row="5" column="1">
+                        <widget class="QPushButton" name="detectAlt1">
                           <property name="enabled">
                             <bool>false</bool>
                           </property>
                           <property name="text">
-                            <string>Alt 2</string>
-                          </property>
-                          <property name="checkable">
-                            <bool>true</bool>
+                            <string>Detect</string>
                           </property>
                         </widget>
                       </item>
                       <item row="4" column="1">
-                        <widget class="QPushButton" name="detectAlt1">
+                        <widget class="QPushButton" name="detectExitapp">
                           <property name="enabled">
                             <bool>false</bool>
                           </property>
                           <property name="text">
                             <string>Detect</string>
                           </property>
                         </widget>
                       </item>
-                      <item row="6" column="0">
-                        <widget class="QCheckBox" name="muxswitch">
+                      <item row="3" column="0">
+                        <widget class="QCheckBox" name="arm">
                           <property name="enabled">
                             <bool>false</bool>
                           </property>
                           <property name="text">
-                            <string>Mux switch</string>
+                            <string>Arm</string>
                           </property>
                           <property name="checkable">
                             <bool>true</bool>
                           </property>
                         </widget>
                       </item>
-                      <item row="6" column="1">
-                        <widget class="QPushButton" name="detectMuxswitch">
+                      <item row="3" column="1">
+                        <widget class="QPushButton" name="detectArm">
                           <property name="enabled">
                             <bool>false</bool>
                           </property>
                           <property name="text">
                             <string>Detect</string>
                           </property>
                         </widget>
```

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/lighthouse_bs_geometry_dialog.py` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/lighthouse_bs_geometry_dialog.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/lighthouse_bs_geometry_dialog.ui` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/lighthouse_bs_geometry_dialog.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/lighthouse_system_type_dialog.py` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/lighthouse_system_type_dialog.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/lighthouse_system_type_dialog.ui` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/lighthouse_system_type_dialog.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/logconfigdialogue.py` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/logconfigdialogue.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/dialogs/logconfigdialogue.ui` & `cfclient-2023.6rc1/src/cfclient/ui/dialogs/logconfigdialogue.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/icons/create.png` & `cfclient-2023.6rc1/src/cfclient/ui/icons/create.png`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/icons/icon-256.png` & `cfclient-2023.6rc1/src/cfclient/ui/icons/icon-256.png`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/main.py` & `cfclient-2023.6rc1/src/cfclient/ui/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,14 +204,17 @@
         self.joystickReader.heighthold_input_updated.add_callback(
             lambda *args: self._disable_input or
             self.cf.commander.send_zdistance_setpoint(*args))
 
         self.joystickReader.hover_input_updated.add_callback(
             self.cf.commander.send_hover_setpoint)
 
+        # Emergency stop button
+        self.esButton.clicked.connect(self._emergency_stop)
+
         # Connection callbacks and signal wrappers for UI protection
         self.cf.connected.add_callback(self.connectionDoneSignal.emit)
         self.connectionDoneSignal.connect(self._connected)
         self.cf.disconnected.add_callback(self.disconnectedSignal.emit)
         self.disconnectedSignal.connect(self._disconnected)
         self.cf.connection_lost.add_callback(self.connectionLostSignal.emit)
         self.connectionLostSignal.connect(self._connection_lost)
@@ -362,15 +365,18 @@
 
     def _set_address(self):
         address = 0xE7E7E7E7E7
         try:
             link_uri = Config().get("link_uri")
             if link_uri.startswith("radio://"):
                 if len(link_uri) > 0:
-                    address = int(link_uri.split('/')[-1], 16)
+                    parts = link_uri.split('/')
+                    # The uri might not contain an address
+                    if len(parts) == 6:
+                        address = int(parts[-1], 16)
         except Exception as err:
             logger.warn('failed to parse address from config: %s' % str(err))
         finally:
             self.address.setValue(address)
 
     def _theme_selected(self, *args):
         """ Callback when a theme is selected. """
@@ -448,21 +454,25 @@
             self.menuItemConnect.setText("Connect to Crazyflie")
             self.menuItemConnect.setEnabled(canConnect)
             self._connectivity_manager.set_state(ConnectivityManager.UIState.DISCONNECTED)
             self.batteryBar.setValue(3000)
             self._menu_cf2_config.setEnabled(False)
             self.linkQualityBar.setValue(0)
             self.logConfigAction.setEnabled(False)
+            self.esButton.setStyleSheet("")
+            self.esButton.setEnabled(False)
         elif self.uiState == UIState.CONNECTED:
             s = "Connected on %s" % self._connectivity_manager.get_interface()
             self.setWindowTitle(s)
             self.menuItemConnect.setText("Disconnect")
             self.menuItemConnect.setEnabled(True)
             self._connectivity_manager.set_state(ConnectivityManager.UIState.CONNECTED)
             self.logConfigAction.setEnabled(True)
+            self.esButton.setEnabled(True)
+            self.esButton.setStyleSheet("background-color: red")
             # Find out if there's an I2C EEPROM, otherwise don't show the
             # dialog.
             if len(self.cf.mem.get_mems(MemoryElement.TYPE_I2C)) > 0:
                 self._menu_cf2_config.setEnabled(True)
         elif self.uiState == UIState.CONNECTING:
             s = "Connecting to {} ...".format(self._connectivity_manager.get_interface())
             self.setWindowTitle(s)
@@ -558,14 +568,21 @@
     def _show_input_device_config_dialog(self):
         self.inputConfig = InputConfigDialogue(self.joystickReader)
         self.inputConfig.show()
 
     def _show_connect_dialog(self):
         self.logConfigDialogue.show()
 
+    def _emergency_stop(self):
+        # send disarming command
+        if (self.uiState == UIState.CONNECTED):
+            # Send both emergency stop and disarm
+            # TODO krri Disarm?
+            self.cf.loc.send_emergency_stop()
+
     def _update_battery(self, timestamp, data, logconf):
         self.batteryBar.setValue(int(data["pm.vbat"] * 1000))
 
         color = UiUtils.COLOR_BLUE
         # TODO firmware reports fully-charged state as 'Battery',
         # rather than 'Charged'
         if data["pm.state"] in [BatteryStates.CHARGING, BatteryStates.CHARGED]:
```

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/main.ui` & `cfclient-2023.6rc1/src/cfclient/ui/main.ui`

 * *Files 10% similar despite different names*

#### Comparing `cfclient-2023.2rc1/src/cfclient/ui/main.ui` & `cfclient-2023.6rc1/src/cfclient/ui/main.ui`

```diff
@@ -2,16 +2,16 @@
 <ui version="4.0">
   <class>MainWindow</class>
   <widget class="QMainWindow" name="MainWindow">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>872</width>
-        <height>671</height>
+        <width>1354</width>
+        <height>592</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>Crazyflie Nano Quadcopter Control</string>
     </property>
     <property name="statusTip">
       <string/>
@@ -19,98 +19,34 @@
     <widget class="QWidget" name="centralwidget">
       <layout class="QGridLayout" name="gridLayout">
         <item row="0" column="0">
           <layout class="QVBoxLayout" name="verticalLayout_2">
             <item>
               <layout class="QGridLayout" name="gridLayout_2">
                 <item row="0" column="6">
-                  <widget class="QLineEdit" name="_aff_volts">
-                    <property name="sizePolicy">
-                      <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
-                        <horstretch>0</horstretch>
-                        <verstretch>0</verstretch>
-                      </sizepolicy>
-                    </property>
-                    <property name="minimumSize">
-                      <size>
-                        <width>60</width>
-                        <height>30</height>
-                      </size>
-                    </property>
-                    <property name="maximumSize">
-                      <size>
-                        <width>60</width>
-                        <height>40</height>
-                      </size>
-                    </property>
-                    <property name="alignment">
-                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                    </property>
-                    <property name="readOnly">
-                      <bool>true</bool>
-                    </property>
-                  </widget>
-                </item>
-                <item row="0" column="0">
-                  <widget class="QComboBox" name="interfaceCombo">
-                    <property name="minimumSize">
-                      <size>
-                        <width>160</width>
-                        <height>0</height>
-                      </size>
-                    </property>
-                    <property name="editable">
-                      <bool>false</bool>
-                    </property>
-                  </widget>
-                </item>
-                <item row="0" column="1">
-                  <widget class="QPushButton" name="connectButton">
-                    <property name="minimumSize">
-                      <size>
-                        <width>60</width>
-                        <height>0</height>
-                      </size>
-                    </property>
-                    <property name="toolTip">
-                      <string/>
+                  <widget class="QLabel" name="batteryLabel">
+                    <property name="text">
+                      <string>Battery:</string>
                     </property>
                   </widget>
                 </item>
                 <item row="0" column="2">
                   <widget class="QPushButton" name="scanButton">
                     <property name="minimumSize">
                       <size>
                         <width>50</width>
                         <height>0</height>
                       </size>
                     </property>
-                  </widget>
-                </item>
-                <item row="0" column="3">
-                  <spacer name="horizontalSpacer">
-                    <property name="orientation">
-                      <enum>Qt::Horizontal</enum>
-                    </property>
-                    <property name="sizeHint" stdset="0">
-                      <size>
-                        <width>40</width>
-                        <height>20</height>
-                      </size>
-                    </property>
-                  </spacer>
-                </item>
-                <item row="0" column="8">
-                  <widget class="QLabel" name="linkQualityLabel">
                     <property name="text">
-                      <string>Link Quality:</string>
+                      <string>Scan</string>
                     </property>
                   </widget>
                 </item>
-                <item row="0" column="9">
+                <item row="0" column="11">
                   <widget class="QProgressBar" name="linkQualityBar">
                     <property name="minimumSize">
                       <size>
                         <width>30</width>
                         <height>0</height>
                       </size>
                     </property>
@@ -131,21 +67,56 @@
                     </property>
                     <property name="format">
                       <string>Link quality %p%</string>
                     </property>
                   </widget>
                 </item>
                 <item row="0" column="4">
-                  <widget class="QLabel" name="batteryLabel">
+                  <widget class="QPushButton" name="esButton">
+                    <property name="sizePolicy">
+                      <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
+                        <horstretch>0</horstretch>
+                        <verstretch>0</verstretch>
+                      </sizepolicy>
+                    </property>
+                    <property name="minimumSize">
+                      <size>
+                        <width>130</width>
+                        <height>0</height>
+                      </size>
+                    </property>
                     <property name="text">
-                      <string>Battery:</string>
+                      <string>Emergency stop</string>
                     </property>
                   </widget>
                 </item>
-                <item row="0" column="5">
+                <item row="0" column="9">
+                  <widget class="QLabel" name="label">
+                    <property name="text">
+                      <string>volts</string>
+                    </property>
+                  </widget>
+                </item>
+                <item row="0" column="1">
+                  <widget class="QPushButton" name="connectButton">
+                    <property name="minimumSize">
+                      <size>
+                        <width>80</width>
+                        <height>0</height>
+                      </size>
+                    </property>
+                    <property name="toolTip">
+                      <string/>
+                    </property>
+                    <property name="text">
+                      <string>Connect</string>
+                    </property>
+                  </widget>
+                </item>
+                <item row="0" column="7">
                   <widget class="QProgressBar" name="batteryBar">
                     <property name="minimumSize">
                       <size>
                         <width>30</width>
                         <height>0</height>
                       </size>
                     </property>
@@ -174,21 +145,103 @@
                       <enum>QProgressBar::TopToBottom</enum>
                     </property>
                     <property name="format">
                       <string>Battery %v mV</string>
                     </property>
                   </widget>
                 </item>
-                <item row="0" column="7">
-                  <widget class="QLabel" name="label">
+                <item row="0" column="0">
+                  <widget class="QComboBox" name="interfaceCombo">
+                    <property name="sizePolicy">
+                      <sizepolicy hsizetype="Maximum" vsizetype="Fixed">
+                        <horstretch>2</horstretch>
+                        <verstretch>0</verstretch>
+                      </sizepolicy>
+                    </property>
+                    <property name="minimumSize">
+                      <size>
+                        <width>160</width>
+                        <height>0</height>
+                      </size>
+                    </property>
+                    <property name="maximumSize">
+                      <size>
+                        <width>250</width>
+                        <height>16777215</height>
+                      </size>
+                    </property>
+                    <property name="editable">
+                      <bool>false</bool>
+                    </property>
+                  </widget>
+                </item>
+                <item row="0" column="8">
+                  <widget class="QLineEdit" name="_aff_volts">
+                    <property name="enabled">
+                      <bool>true</bool>
+                    </property>
+                    <property name="sizePolicy">
+                      <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
+                        <horstretch>0</horstretch>
+                        <verstretch>0</verstretch>
+                      </sizepolicy>
+                    </property>
+                    <property name="minimumSize">
+                      <size>
+                        <width>60</width>
+                        <height>30</height>
+                      </size>
+                    </property>
+                    <property name="maximumSize">
+                      <size>
+                        <width>60</width>
+                        <height>40</height>
+                      </size>
+                    </property>
+                    <property name="alignment">
+                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                    </property>
+                    <property name="readOnly">
+                      <bool>true</bool>
+                    </property>
+                  </widget>
+                </item>
+                <item row="0" column="10">
+                  <widget class="QLabel" name="linkQualityLabel">
                     <property name="text">
-                      <string>volts</string>
+                      <string>Link Quality:</string>
                     </property>
                   </widget>
                 </item>
+                <item row="0" column="3">
+                  <spacer name="horizontalSpacer">
+                    <property name="orientation">
+                      <enum>Qt::Horizontal</enum>
+                    </property>
+                    <property name="sizeHint" stdset="0">
+                      <size>
+                        <width>40</width>
+                        <height>20</height>
+                      </size>
+                    </property>
+                  </spacer>
+                </item>
+                <item row="0" column="5">
+                  <spacer name="horizontalSpacer_3">
+                    <property name="orientation">
+                      <enum>Qt::Horizontal</enum>
+                    </property>
+                    <property name="sizeHint" stdset="0">
+                      <size>
+                        <width>40</width>
+                        <height>20</height>
+                      </size>
+                    </property>
+                  </spacer>
+                </item>
               </layout>
             </item>
             <item>
               <widget class="QGroupBox" name="groupBox">
                 <layout class="QHBoxLayout" stretch="0,0,0">
                   <item>
                     <widget class="QLabel" name="addressLabel">
@@ -250,16 +303,16 @@
                   <bool>true</bool>
                 </property>
                 <widget class="QWidget" name="scrollAreaWidgetContents">
                   <property name="geometry">
                     <rect>
                       <x>0</x>
                       <y>0</y>
-                      <width>846</width>
-                      <height>469</height>
+                      <width>1334</width>
+                      <height>414</height>
                     </rect>
                   </property>
                   <property name="sizePolicy">
                     <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
                       <horstretch>0</horstretch>
                       <verstretch>0</verstretch>
                     </sizepolicy>
@@ -302,16 +355,16 @@
       </layout>
     </widget>
     <widget class="QMenuBar" name="menubar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
-          <width>872</width>
-          <height>24</height>
+          <width>1354</width>
+          <height>22</height>
         </rect>
       </property>
       <widget class="QMenu" name="menuFile">
         <property name="title">
           <string>File</string>
         </property>
         <addaction name="separator"/>
```

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/pluginhelper.py` & `cfclient-2023.6rc1/src/cfclient/ui/pluginhelper.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/pose_logger.py` & `cfclient-2023.6rc1/src/cfclient/ui/pose_logger.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tab_toolbox.py` & `cfclient-2023.6rc1/src/cfclient/ui/tab_toolbox.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/ConsoleTab.py` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/ConsoleTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/CrtpSharkToolbox.py` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/CrtpSharkToolbox.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/ExampleTab.py` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/ExampleTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/FlightTab.py` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/FlightTab.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,18 +42,14 @@
 from cfclient.utils.config import Config
 from cflib.crazyflie.log import LogConfig
 
 from cfclient.utils.input import JoystickReader
 
 from cfclient.ui.tab_toolbox import TabToolbox
 
-LOG_NAME_ESTIMATE_X = 'stateEstimate.x'
-LOG_NAME_ESTIMATE_Y = 'stateEstimate.y'
-LOG_NAME_ESTIMATE_Z = 'stateEstimate.z'
-
 __author__ = 'Bitcraze AB'
 __all__ = ['FlightTab']
 
 logger = logging.getLogger(__name__)
 
 flight_tab_class = uic.loadUiType(cfclient.module_path +
                                   "/ui/tabs/flightTab.ui")[0]
@@ -96,27 +92,36 @@
 
     _log_data_signal = pyqtSignal(int, object, object)
     _pose_data_signal = pyqtSignal(object, object)
 
     _input_updated_signal = pyqtSignal(float, float, float, float)
     _rp_trim_updated_signal = pyqtSignal(float, float)
     _emergency_stop_updated_signal = pyqtSignal(bool)
+    _arm_updated_signal = pyqtSignal(bool)
     _assisted_control_updated_signal = pyqtSignal(bool)
     _heighthold_input_updated_signal = pyqtSignal(float, float, float, float)
     _hover_input_updated_signal = pyqtSignal(float, float, float, float)
 
     _log_error_signal = pyqtSignal(object, str)
 
     # UI_DATA_UPDATE_FPS = 10
 
     connectionFinishedSignal = pyqtSignal(str)
     disconnectedSignal = pyqtSignal(str)
 
     _limiting_updated = pyqtSignal(bool, bool, bool)
 
+    LOG_NAME_THRUST = 'stabilizer.thrust'
+    LOG_NAME_MOTOR_1 = 'motor.m1'
+    LOG_NAME_MOTOR_2 = 'motor.m2'
+    LOG_NAME_MOTOR_3 = 'motor.m3'
+    LOG_NAME_MOTOR_4 = 'motor.m4'
+    LOG_NAME_CAN_FLY = 'sys.canfly'
+    LOG_NAME_SUPERVISOR_INFO = 'supervisor.info'
+
     def __init__(self, helper):
         super(FlightTab, self).__init__(helper, 'Flight Control')
         self.setupUi(self)
 
         self.disconnectedSignal.connect(self.disconnected)
         self.connectionFinishedSignal.connect(self.connected)
         # Incomming signals
@@ -129,14 +134,16 @@
             self._input_updated_signal.emit)
         self._rp_trim_updated_signal.connect(self.calUpdateFromInput)
         self._helper.inputDeviceReader.rp_trim_updated.add_callback(
             self._rp_trim_updated_signal.emit)
         self._emergency_stop_updated_signal.connect(self.updateEmergencyStop)
         self._helper.inputDeviceReader.emergency_stop_updated.add_callback(
             self._emergency_stop_updated_signal.emit)
+        self._arm_updated_signal.connect(self.updateArm)
+        self._helper.inputDeviceReader.arm_updated.add_callback(self._arm_updated_signal.emit)
 
         self._helper.inputDeviceReader.heighthold_input_updated.add_callback(
             self._heighthold_input_updated_signal.emit)
         self._heighthold_input_updated_signal.connect(
             self._heighthold_input_updated)
         self._helper.inputDeviceReader.hover_input_updated.add_callback(
             self._hover_input_updated_signal.emit)
@@ -150,37 +157,45 @@
             self._assisted_control_updated)
 
         self._pose_data_signal.connect(self._pose_data_received)
         self._log_data_signal.connect(self._log_data_received)
 
         self._log_error_signal.connect(self._logging_error)
 
+        self._isConnected = False
+
         # Connect UI signals that are in this tab
         self.flightModeCombo.currentIndexChanged.connect(self.flightmodeChange)
         self.minThrust.valueChanged.connect(self.minMaxThrustChanged)
         self.maxThrust.valueChanged.connect(self.minMaxThrustChanged)
         self.thrustLoweringSlewRateLimit.valueChanged.connect(self.thrustLoweringSlewRateLimitChanged)
         self.slewEnableLimit.valueChanged.connect(self.thrustLoweringSlewRateLimitChanged)
         self.targetCalRoll.valueChanged.connect(self._trim_roll_changed)
         self.targetCalPitch.valueChanged.connect(self._trim_pitch_changed)
         self.maxAngle.valueChanged.connect(self.maxAngleChanged)
         self.maxYawRate.valueChanged.connect(self.maxYawRateChanged)
         self.uiSetupReadySignal.connect(self.uiSetupReady)
         self.isInCrazyFlightmode = False
 
         # Command Based Flight Control
-        self._can_fly = 0
+        self._can_fly_deprecated = 0
         self.commanderTakeOffButton.clicked.connect(lambda: self._flight_command(CommanderAction.TAKE_OFF))
         self.commanderLandButton.clicked.connect(lambda: self._flight_command(CommanderAction.LAND))
         self.commanderLeftButton.clicked.connect(lambda: self._flight_command(CommanderAction.LEFT))
         self.commanderRightButton.clicked.connect(lambda: self._flight_command(CommanderAction.RIGHT))
         self.commanderForwardButton.clicked.connect(lambda: self._flight_command(CommanderAction.FORWARD))
         self.commanderBackButton.clicked.connect(lambda: self._flight_command(CommanderAction.BACK))
         self.commanderUpButton.clicked.connect(lambda: self._flight_command(CommanderAction.UP))
         self.commanderDownButton.clicked.connect(lambda: self._flight_command(CommanderAction.DOWN))
+        self._update_flight_commander(False)
+
+        # Supervisor
+        self._supervisor_info_bitfield = 0
+        self.armButton.clicked.connect(self.updateArm)
+        self._update_arm_button(False)
 
         self.uiSetupReady()
 
         self._led_ring_headlight.clicked.connect(
             lambda enabled: self._helper.cf.param.set_value("ring.headlightEnable", int(enabled)))
 
         self._helper.cf.param.add_update_callback(
@@ -266,27 +281,32 @@
 
     def _logging_error(self, log_conf, msg):
         QMessageBox.about(self, "Log error",
                           "Error when starting log config [%s]: %s" % (
                               log_conf.name, msg))
 
     def _log_data_received(self, timestamp, data, logconf):
-        if self.isVisible():
-            self.actualM1.setValue(data["motor.m1"])
-            self.actualM2.setValue(data["motor.m2"])
-            self.actualM3.setValue(data["motor.m3"])
-            self.actualM4.setValue(data["motor.m4"])
+        if self.isVisible() and self._isConnected:
+            self.actualM1.setValue(data[self.LOG_NAME_MOTOR_1])
+            self.actualM2.setValue(data[self.LOG_NAME_MOTOR_2])
+            self.actualM3.setValue(data[self.LOG_NAME_MOTOR_3])
+            self.actualM4.setValue(data[self.LOG_NAME_MOTOR_4])
 
             self.estimateThrust.setText(
-                "%.2f%%" % self.thrustToPercentage(data["stabilizer.thrust"]))
+                "%.2f%%" % self.thrustToPercentage(data[self.LOG_NAME_THRUST]))
 
-            if data["sys.canfly"] != self._can_fly:
-                self._can_fly = data["sys.canfly"]
+            if data[self.LOG_NAME_CAN_FLY] != self._can_fly_deprecated:
+                self._can_fly_deprecated = data[self.LOG_NAME_CAN_FLY]
                 self._update_flight_commander(True)
 
+            if self.LOG_NAME_SUPERVISOR_INFO in data:
+                self._supervisor_info_bitfield = data[self.LOG_NAME_SUPERVISOR_INFO]
+
+            self._update_arm_button(True)
+
     def _pose_data_received(self, pose_logger, pose):
         if self.isVisible():
             estimated_z = pose[2]
             roll = pose[3]
             pitch = pose[4]
 
             self.estimateX.setText(("%.2f" % pose[0]))
@@ -331,62 +351,93 @@
         else:
             pitch, roll, yaw = 'Pitch', 'Roll', 'Yaw'
 
         self.inputPitchLabel.setText(pitch)
         self.inputRollLabel.setText(roll)
         self.inputYawLabel.setText(yaw)
 
+    def _update_arm_button(self, connected):
+        if not connected:
+            self.armButton.setStyleSheet("")
+            self.armButton.setText("Arm")
+            self.armButton.setEnabled(False)
+            return
+
+        if self._is_flying():
+            self.armButton.setEnabled(True)
+            self.armButton.setText("Emergency stop")
+            self.armButton.setStyleSheet("background-color: red")
+            return
+
+        if self._is_armed():
+            self.armButton.setStyleSheet("background-color: red")
+            if self._auto_arming():
+                self.armButton.setEnabled(False)
+                self.armButton.setText("Auto armed")
+            else:
+                self.armButton.setEnabled(True)
+                self.armButton.setText("Disarm")
+        else:
+            self.armButton.setText("Arm")
+            if self._can_arm():
+                self.armButton.setEnabled(True)
+                self.armButton.setStyleSheet("background-color: lightgreen")
+            else:
+                self.armButton.setStyleSheet("")
+                self.armButton.setEnabled(False)
+
     def _update_flight_commander(self, connected):
         self.commanderBox.setToolTip(str())
         if not connected:
             self.commanderBox.setEnabled(False)
             return
 
-        if self._can_fly == 0:
+        if self._can_fly_deprecated == 0:
             self.commanderBox.setEnabled(False)
-            self.commanderBox.setToolTip(
-                'The Crazyflie reports that flight is not possible'
-            )
+            self.commanderBox.setToolTip('The Crazyflie reports that flight is not possible')
             return
 
         # We cannot know if we have a positioning deck until we get params
         if not self._helper.cf.param.is_updated:
             self.commanderBox.setEnabled(False)
             return
 
         #                  flowV1    flowV2     LightHouse       LPS
         position_decks = ['bcFlow', 'bcFlow2', 'bcLighthouse4', 'bcLoco', 'bcDWM1000']
         for deck in position_decks:
             if int(self._helper.cf.param.values['deck'][deck]) == 1:
                 self.commanderBox.setEnabled(True)
                 break
         else:
-            self.commanderBox.setToolTip(
-                'You need a positioning deck to use Command Based Flight'
-            )
+            self.commanderBox.setToolTip('You need a positioning deck to use Command Based Flight')
             self.commanderBox.setEnabled(False)
             return
 
         # To prevent conflicting commands from the controller and the flight panel
         if JoystickReader().available_devices():
             self.commanderBox.setToolTip(
                 'Cant use both an controller and Command Based Flight'
             )
             self.commanderBox.setEnabled(False)
             return
 
     def connected(self, linkURI):
+        self._isConnected = True
         # MOTOR & THRUST
         lg = LogConfig("Motors", Config().get("ui_update_period"))
-        lg.add_variable("stabilizer.thrust", "uint16_t")
-        lg.add_variable("motor.m1")
-        lg.add_variable("motor.m2")
-        lg.add_variable("motor.m3")
-        lg.add_variable("motor.m4")
-        lg.add_variable("sys.canfly")
+        lg.add_variable(self.LOG_NAME_THRUST, "uint16_t")
+        lg.add_variable(self.LOG_NAME_MOTOR_1)
+        lg.add_variable(self.LOG_NAME_MOTOR_2)
+        lg.add_variable(self.LOG_NAME_MOTOR_3)
+        lg.add_variable(self.LOG_NAME_MOTOR_4)
+        lg.add_variable(self.LOG_NAME_CAN_FLY)
+
+        # Add supervisor info if it exists to keep backwards compatibility
+        if self._helper.cf.log.toc.get_element_by_complete_name(self.LOG_NAME_SUPERVISOR_INFO):
+            lg.add_variable(self.LOG_NAME_SUPERVISOR_INFO)
 
         try:
             self._helper.cf.log.add_config(lg)
             lg.data_received_cb.add_callback(self._log_data_signal.emit)
             lg.error_cb.add_callback(self._log_error_signal.emit)
             lg.start()
         except KeyError as e:
@@ -396,21 +447,22 @@
 
     def _enable_estimators(self, should_enable):
         self.estimateX.setEnabled(should_enable)
         self.estimateY.setEnabled(should_enable)
         self.estimateZ.setEnabled(should_enable)
 
     def _set_available_sensors(self, name, available):
-        logger.info("[%s]: %s", name, available)
+        logger.debug("[%s]: %s", name, available)
         available = eval(available)
 
         self._enable_estimators(True)
         self._helper.inputDeviceReader.set_alt_hold_available(available)
 
     def disconnected(self, linkURI):
+        self._isConnected = False
         self.ai.setRollPitch(0, 0)
         self.actualM1.setValue(0)
         self.actualM2.setValue(0)
         self.actualM3.setValue(0)
         self.actualM4.setValue(0)
 
         self.estimateRoll.setText("")
@@ -446,14 +498,35 @@
             # Signal was not connected
             pass
         self._assist_mode_combo.setEnabled(False)
         self._assist_mode_combo.clear()
 
         self._update_flight_commander(False)
 
+        self._supervisor_info_bitfield = 0
+        self._update_arm_button(False)
+
+    def _can_arm(self):
+        return bool(self._supervisor_info_bitfield & 0x0001)
+
+    def _is_armed(self):
+        return bool(self._supervisor_info_bitfield & 0x0002)
+
+    def _auto_arming(self):
+        return bool(self._supervisor_info_bitfield & 0x0004)
+
+    def _can_fly(self):
+        return bool(self._supervisor_info_bitfield & 0x0008)
+
+    def _is_flying(self):
+        return bool(self._supervisor_info_bitfield & 0x0010)
+
+    def _is_tumbled(self):
+        return bool(self._supervisor_info_bitfield & 0x0020)
+
     def minMaxThrustChanged(self):
         self._helper.inputDeviceReader.min_thrust = self.minThrust.value()
         self._helper.inputDeviceReader.max_thrust = self.maxThrust.value()
         if (self.isInCrazyFlightmode is True):
             Config().set("min_thrust", self.minThrust.value())
             Config().set("max_thrust", self.maxThrust.value())
 
@@ -514,17 +587,31 @@
         return ("<html><head/><body><p>"
                 "<span style='font-weight:600; color:#7b0005;'>{}</span>"
                 "</p></body></html>".format(text))
 
     def updateEmergencyStop(self, emergencyStop):
         if emergencyStop:
             self.setMotorLabelsEnabled(False)
+            self._helper.cf.loc.send_emergency_stop()
+            # TODO krri disarm?
         else:
             self.setMotorLabelsEnabled(True)
 
+    def updateArm(self):
+        if self._is_flying():
+            self._helper.cf.loc.send_emergency_stop()
+            # TODO krri disarm?
+        else:
+            if self._is_armed():
+                self._helper.cf.platform.send_arming_request(False)
+            else:
+                if self._can_arm():
+                    self.armButton.setStyleSheet("background-color: orange")
+                    self._helper.cf.platform.send_arming_request(True)
+
     def flightmodeChange(self, item):
         Config().set("flightmode", str(self.flightModeCombo.itemText(item)))
         logger.debug("Changed flightmode to %s",
                      self.flightModeCombo.itemText(item))
         self.isInCrazyFlightmode = False
         if (item == 0):  # Normal
             self.maxAngle.setValue(Config().get("normal_max_rp"))
@@ -594,14 +681,15 @@
     def alt2_updated(self, state):
         self._helper.cf.param.set_value("ring.headlightEnable", str(state))
 
     def _all_params_updated(self):
         self._ring_populate_dropdown()
         self._populate_assisted_mode_dropdown()
         self._update_flight_commander(True)
+        self._update_arm_button(True)
 
     def _ring_populate_dropdown(self):
         try:
             nbr = int(self._helper.cf.param.values["ring"]["neffect"])
             current = int(self._helper.cf.param.values["ring"]["effect"])
         except KeyError:
             return
@@ -648,15 +736,15 @@
             self._led_ring_effect.setEnabled(True)
             self._led_ring_headlight.setEnabled(True)
 
     def _ring_effect_changed(self, index):
         self._ring_effect = index
         if index > -1:
             i = self._led_ring_effect.itemData(index)
-            logger.info("Changed effect to {}".format(i))
+            logger.debug("Changed effect to {}".format(i))
             if i != int(self._helper.cf.param.values["ring"]["effect"]):
                 self._helper.cf.param.set_value("ring.effect", str(i))
 
     def _ring_effect_updated(self, name, value):
         if self._helper.cf.param.is_updated:
             self._led_ring_effect.setCurrentIndex(int(value))
```

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/GpsTab.py` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/GpsTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/LEDTab.py` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/LEDTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/LogBlockDebugTab.py` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/LogBlockDebugTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/LogBlockTab.py` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/LogBlockTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/LogClientTab.py` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/LogClientTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/LogTab.py` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/LogTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/ParamTab.py` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/ParamTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/PlotTab.py` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/PlotTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/QualisysTab.py` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/QualisysTab.py`

 * *Files 0% similar despite different names*

```diff
@@ -1388,15 +1388,15 @@
         else:
             self._helper.mainUI.disable_input(True)
 
         self._event.clear()
         # Threadsafe call
         self._machine.postEvent(FlightModeEvent(mode))
 
-        logger.info('Switching Flight Mode to: %s', mode)
+        logger.debug('Switching Flight Mode to: %s', mode)
 
     def send_setpoint(self, pos):
         # Wraps the send command to the crazyflie
         if self._cf is not None:
             self._cf.commander.send_position_setpoint(pos.x, pos.y, pos.z, 0.0)
```

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/TuningTab.py` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/TuningTab.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/__init__.py` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/__init__.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/consoleTab.ui` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/consoleTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/crtpSharkToolbox.ui` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/crtpSharkToolbox.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/flightActionContainer.ui` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/flightActionContainer.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/flightTab.ui` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/flightTab.ui`

 * *Files 5% similar despite different names*

#### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/flightTab.ui` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/flightTab.ui`

```diff
@@ -2,16 +2,16 @@
 <ui version="4.0">
   <class>Form</class>
   <widget class="QWidget" name="Form">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>1228</width>
-        <height>916</height>
+        <width>1326</width>
+        <height>930</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>Form</string>
     </property>
     <layout class="QHBoxLayout" name="horizontalLayout">
       <item>
@@ -237,52 +237,128 @@
                         <item row="1" column="0">
                           <widget class="QLabel" name="label_32">
                             <property name="text">
                               <string>Max Yaw angle/rate</string>
                             </property>
                           </widget>
                         </item>
-                        <item row="2" column="1">
-                          <widget class="QDoubleSpinBox" name="maxThrust"/>
-                        </item>
-                        <item row="3" column="1">
-                          <widget class="QDoubleSpinBox" name="minThrust"/>
-                        </item>
-                        <item row="4" column="1">
-                          <widget class="QDoubleSpinBox" name="slewEnableLimit"/>
-                        </item>
-                        <item row="5" column="1">
-                          <widget class="QDoubleSpinBox" name="thrustLoweringSlewRateLimit"/>
-                        </item>
                         <item row="1" column="1">
                           <widget class="QSpinBox" name="maxYawRate">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="minimumSize">
+                              <size>
+                                <width>57</width>
+                                <height>0</height>
+                              </size>
+                            </property>
                             <property name="minimum">
                               <number>0</number>
                             </property>
                             <property name="maximum">
                               <number>500</number>
                             </property>
                             <property name="value">
                               <number>0</number>
                             </property>
                           </widget>
                         </item>
                         <item row="0" column="1">
                           <widget class="QSpinBox" name="maxAngle">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="minimumSize">
+                              <size>
+                                <width>57</width>
+                                <height>0</height>
+                              </size>
+                            </property>
                             <property name="minimum">
                               <number>0</number>
                             </property>
                             <property name="maximum">
                               <number>500</number>
                             </property>
                             <property name="value">
                               <number>0</number>
                             </property>
                           </widget>
                         </item>
+                        <item row="2" column="1">
+                          <widget class="QSpinBox" name="maxThrust">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="minimumSize">
+                              <size>
+                                <width>57</width>
+                                <height>0</height>
+                              </size>
+                            </property>
+                          </widget>
+                        </item>
+                        <item row="3" column="1">
+                          <widget class="QSpinBox" name="minThrust">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="minimumSize">
+                              <size>
+                                <width>57</width>
+                                <height>0</height>
+                              </size>
+                            </property>
+                          </widget>
+                        </item>
+                        <item row="4" column="1">
+                          <widget class="QSpinBox" name="slewEnableLimit">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="minimumSize">
+                              <size>
+                                <width>57</width>
+                                <height>0</height>
+                              </size>
+                            </property>
+                          </widget>
+                        </item>
+                        <item row="5" column="1">
+                          <widget class="QSpinBox" name="thrustLoweringSlewRateLimit">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="Fixed" vsizetype="Fixed">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="minimumSize">
+                              <size>
+                                <width>57</width>
+                                <height>0</height>
+                              </size>
+                            </property>
+                          </widget>
+                        </item>
                       </layout>
                     </item>
                   </layout>
                 </widget>
               </item>
               <item>
                 <widget class="QGroupBox" name="groupBox_4">
@@ -336,26 +412,53 @@
                     <size>
                       <width>20</width>
                       <height>40</height>
                     </size>
                   </property>
                 </spacer>
               </item>
+              <item>
+                <widget class="QPushButton" name="armButton">
+                  <property name="enabled">
+                    <bool>true</bool>
+                  </property>
+                  <property name="sizePolicy">
+                    <sizepolicy hsizetype="Minimum" vsizetype="Minimum">
+                      <horstretch>0</horstretch>
+                      <verstretch>0</verstretch>
+                    </sizepolicy>
+                  </property>
+                  <property name="minimumSize">
+                    <size>
+                      <width>0</width>
+                      <height>100</height>
+                    </size>
+                  </property>
+                  <property name="font">
+                    <font>
+                      <pointsize>20</pointsize>
+                    </font>
+                  </property>
+                  <property name="text">
+                    <string>Arm</string>
+                  </property>
+                </widget>
+              </item>
             </layout>
           </widget>
           <widget class="QWidget" name="layoutWidget">
             <layout class="QHBoxLayout" name="horizontalLayout_2">
               <property name="sizeConstraint">
                 <enum>QLayout::SetDefaultConstraint</enum>
               </property>
               <item>
                 <widget class="QGroupBox" name="groupBox">
                   <property name="sizePolicy">
                     <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
-                      <horstretch>2</horstretch>
+                      <horstretch>0</horstretch>
                       <verstretch>0</verstretch>
                     </sizepolicy>
                   </property>
                   <property name="title">
                     <string>Flight Data</string>
                   </property>
                   <layout class="QGridLayout" name="gridLayout">
@@ -364,15 +467,15 @@
                         <property name="orientation">
                           <enum>Qt::Vertical</enum>
                         </property>
                         <widget class="QWidget" name="layoutWidget">
                           <layout class="QVBoxLayout" name="verticalLayout_4"/>
                         </widget>
                         <widget class="QWidget" name="layoutWidget">
-                          <layout class="QGridLayout" name="gridLayout_5" rowstretch="0,0,0,0,0,0,0,0,0">
+                          <layout class="QGridLayout" name="gridLayout_5" rowstretch="0,0,0,0,0,0,0,0">
                             <property name="sizeConstraint">
                               <enum>QLayout::SetMinimumSize</enum>
                             </property>
                             <property name="horizontalSpacing">
                               <number>6</number>
                             </property>
                             <property name="verticalSpacing">
@@ -689,15 +792,15 @@
                                 </property>
                                 <property name="title">
                                   <string>Command Based Flight Control</string>
                                 </property>
                                 <property name="alignment">
                                   <set>Qt::AlignCenter</set>
                                 </property>
-                                <property name="Enabled">
+                                <property name="Enabled" stdset="0">
                                   <bool>false</bool>
                                 </property>
                                 <layout class="QGridLayout" name="horizontalLayout">
                                   <property name="leftMargin">
                                     <number>2</number>
                                   </property>
                                   <property name="topMargin">
```

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/gpsTab.ui` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/gpsTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/ledTab.ui` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/ledTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/lighthouse_tab.py` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/lighthouse_tab.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,15 @@
 
     def _set_up_plots(self):
         self._plot_3d = Plot3dLighthouse()
         self._plot_layout.addWidget(self._plot_3d.native)
 
     def _connected(self, link_uri):
         """Callback when the Crazyflie has been connected"""
-        logger.info("Crazyflie connected to {}".format(link_uri))
+        logger.debug("Crazyflie connected to {}".format(link_uri))
 
         self._basestation_geometry_dialog.reset()
         self._is_connected = True
 
         if self._helper.cf.param.get_value('deck.bcLighthouse4') == '1':
             self._lighthouse_deck_detected()
```

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/lighthouse_tab.ui` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/lighthouse_tab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/locopositioning_tab.py` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/locopositioning_tab.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,39 +518,39 @@
         self._id_anchor_button.setEnabled(True)
 
     def _clear_anchors(self):
         self._anchors = {}
 
     def _connected(self, link_uri):
         """Callback when the Crazyflie has been connected"""
-        logger.info("Crazyflie connected to {}".format(link_uri))
+        logger.debug("Crazyflie connected to {}".format(link_uri))
         self._request_param_to_detect_loco_deck()
 
     def _request_param_to_detect_loco_deck(self):
         """Send a parameter request to detect if the Loco deck is installed"""
         group = 'deck'
 
         def register(group, param):
             if self._is_in_param_toc(group, param):
-                logger.info("Requesting loco deck parameter")
+                logger.debug("Requesting loco deck parameter")
                 self._helper.cf.param.add_update_callback(group=group,
                                                           name=param,
                                                           cb=self._cb_param_to_detect_loco_deck_signal.emit)
 
         register(group, 'bcLoco')
         register(group, 'bcDWM1000')  # For backwards compatibility
 
     def _cb_param_to_detect_loco_deck(self, name, value):
         """Callback from the parameter sub system when the Loco deck detection
         parameter has been updated"""
         if value == '1':
-            logger.info("Loco deck installed, enabling LPS tab")
+            logger.debug("Loco deck installed, enabling LPS tab")
             self._loco_deck_detected()
         else:
-            logger.info("No Loco deck installed")
+            logger.debug("No Loco deck installed")
 
     def _loco_deck_detected(self):
         """Called when the loco deck has been detected. Enables the tab,
         starts logging and polling of the memory sub system as well as starts
         timers for updating graphics"""
         if not self.is_loco_deck_active:
             self.is_loco_deck_active = True
```

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/locopositioning_tab.ui` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/locopositioning_tab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/logBlockDebugTab.ui` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/logBlockDebugTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/logBlockTab.ui` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/logBlockTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/logClientTab.ui` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/logClientTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/logTab.ui` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/logTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/paramTab.ui` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/paramTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/plotTab.ui` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/plotTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/qualisysTab.ui` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/qualisysTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/tabs/tuningTab.ui` & `cfclient-2023.6rc1/src/cfclient/ui/tabs/tuningTab.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/widgets/__init__.py` & `cfclient-2023.6rc1/src/cfclient/ui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/widgets/ai.py` & `cfclient-2023.6rc1/src/cfclient/ui/widgets/ai.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/widgets/hexspinbox.py` & `cfclient-2023.6rc1/src/cfclient/ui/widgets/hexspinbox.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/widgets/plotter.ui` & `cfclient-2023.6rc1/src/cfclient/ui/widgets/plotter.ui`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/widgets/plotwidget.py` & `cfclient-2023.6rc1/src/cfclient/ui/widgets/plotwidget.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/widgets/super_slider.py` & `cfclient-2023.6rc1/src/cfclient/ui/widgets/super_slider.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/wizards/bslh_1.png` & `cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_1.png`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/wizards/bslh_2.png` & `cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_2.png`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/wizards/bslh_3.png` & `cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_3.png`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/wizards/bslh_4.png` & `cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_4.png`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/wizards/bslh_5.png` & `cfclient-2023.6rc1/src/cfclient/ui/wizards/bslh_5.png`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/ui/wizards/lighthouse_geo_bs_estimation_wizard.py` & `cfclient-2023.6rc1/src/cfclient/ui/wizards/lighthouse_geo_bs_estimation_wizard.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/__init__.py` & `cfclient-2023.6rc1/src/cfclient/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/config.py` & `cfclient-2023.6rc1/src/cfclient/utils/config.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/config_manager.py` & `cfclient-2023.6rc1/src/cfclient/utils/config_manager.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/input/__init__.py` & `cfclient-2023.6rc1/src/cfclient/utils/input/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,15 @@
 
         self.input_updated = Caller()
         self.assisted_input_updated = Caller()
         self.heighthold_input_updated = Caller()
         self.hover_input_updated = Caller()
         self.rp_trim_updated = Caller()
         self.emergency_stop_updated = Caller()
+        self.arm_updated = Caller()
         self.device_discovery = Caller()
         self.device_error = Caller()
         self.assisted_control_updated = Caller()
         self.alt1_updated = Caller()
         self.alt2_updated = Caller()
 
         # Call with 3 bools (rp_limiting, yaw_limiting, thrust_limiting)
@@ -415,15 +416,20 @@
 
                 if data.toggled.estop:
                     try:
                         self.emergency_stop_updated.call(data.estop)
                     except Exception as e:
                         logger.warning("Exception while doing callback from"
                                        "input-device for estop: {}".format(e))
-
+                if data.toggled.arm and data._prev_btn_values["arm"]:
+                    try:
+                        self.arm_updated.call(data.arm)
+                    except Exception as e:
+                        logger.warning("Exception while doing callback from"
+                                       "input-device for arm: {}".format(e))
                 if data.toggled.alt1:
                     try:
                         self.alt1_updated.call(data.alt1)
                     except Exception as e:
                         logger.warning("Exception while doing callback from"
                                        "input-device for alt1: {}".format(e))
                 if data.toggled.alt2:
```

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/input/inputinterfaces/__init__.py` & `cfclient-2023.6rc1/src/cfclient/utils/input/inputinterfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/input/inputinterfaces/leapmotion.py` & `cfclient-2023.6rc1/src/cfclient/utils/input/inputinterfaces/leapmotion.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/input/inputinterfaces/wiimote.py` & `cfclient-2023.6rc1/src/cfclient/utils/input/inputinterfaces/wiimote.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/input/inputinterfaces/zmqpull.py` & `cfclient-2023.6rc1/src/cfclient/utils/input/inputinterfaces/zmqpull.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/input/inputreaderinterface.py` & `cfclient-2023.6rc1/src/cfclient/utils/input/inputreaderinterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,17 @@
 
 
 class InputData:
 
     def __init__(self):
         # self._toggled = {}
         self._axes = ("roll", "pitch", "yaw", "thrust")
-        self._buttons = ("alt1", "alt2", "estop", "exit", "pitchNeg",
-                         "pitchPos", "rollNeg", "rollPos", "assistedControl",
-                         "muxswitch")
+        self._buttons = ("pitchNeg", "pitchPos", "rollNeg", "rollPos",
+                         "assistedControl", "estop", "arm",
+                         "exitapp", "alt1", "alt2", "muxswitch")
         for axis in self._axes:
             self.__dict__[axis] = 0.0
         self.toggled = _ToggleState()
         self._prev_btn_values = {}
         for button in self._buttons:
             self.__dict__[button] = False
             self.toggled[button] = False
```

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/input/inputreaders/__init__.py` & `cfclient-2023.6rc1/src/cfclient/utils/input/inputreaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/input/inputreaders/linuxjsdev.py` & `cfclient-2023.6rc1/src/cfclient/utils/input/inputreaders/linuxjsdev.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/input/inputreaders/pysdl2.py` & `cfclient-2023.6rc1/src/cfclient/utils/input/inputreaders/pysdl2.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/input/mux/__init__.py` & `cfclient-2023.6rc1/src/cfclient/utils/input/mux/__init__.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/input/mux/nomux.py` & `cfclient-2023.6rc1/src/cfclient/utils/input/mux/nomux.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/input/mux/takeovermux.py` & `cfclient-2023.6rc1/src/cfclient/utils/input/mux/takeovermux.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/input/mux/takeoverselectivemux.py` & `cfclient-2023.6rc1/src/cfclient/utils/input/mux/takeoverselectivemux.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/logconfigreader.py` & `cfclient-2023.6rc1/src/cfclient/utils/logconfigreader.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/logdatawriter.py` & `cfclient-2023.6rc1/src/cfclient/utils/logdatawriter.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/periodictimer.py` & `cfclient-2023.6rc1/src/cfclient/utils/periodictimer.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/singleton.py` & `cfclient-2023.6rc1/src/cfclient/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/ui.py` & `cfclient-2023.6rc1/src/cfclient/utils/ui.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/zmq_led_driver.py` & `cfclient-2023.6rc1/src/cfclient/utils/zmq_led_driver.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient/utils/zmq_param.py` & `cfclient-2023.6rc1/src/cfclient/utils/zmq_param.py`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfclient.egg-info/PKG-INFO` & `cfclient-2023.6rc1/src/cfclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfclient
-Version: 2023.2rc1
+Version: 2023.6rc1
 Summary: Bitcraze Cazyflie quadcopter client
 Home-page: http://www.bitcraze.io
 Author: Bitcraze team
 Author-email: contact@bitcraze.se
 Keywords: quadcopter crazyflie
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `cfclient-2023.2rc1/src/cfclient.egg-info/SOURCES.txt` & `cfclient-2023.6rc1/src/cfclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfclient-2023.2rc1/src/cfloader/__init__.py` & `cfclient-2023.6rc1/src/cfloader/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,19 @@
                 )
                 for target in connected_targets:
                     print(target)
 
             # flash_full called with no filename will not flash, just call
             # our info callback
             bl.flash_full(None, None, warm_boot, None, print_info)
-        elif action == "flash" and filename and targets:
+        elif action == "flash" and filename:
+            is_target_required = not filename.endswith('.zip')
+            if (is_target_required and not targets):
+                print("The flash action with a non .zip file requires a target")
+                sys.exit(-1)
             try:
                 bl.flash_full(None, filename, warm_boot, targets)
             except Exception as e:
                 print("Failed to flash: {}".format(e))
                 exit_result = -1
         elif action == "reset":
             bl.reset_to_firmware()
```

### Comparing `cfclient-2023.2rc1/src/cfzmq/__init__.py` & `cfclient-2023.6rc1/src/cfzmq/__init__.py`

 * *Files identical despite different names*

