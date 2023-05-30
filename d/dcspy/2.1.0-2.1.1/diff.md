# Comparing `tmp/dcspy-2.1.0.tar.gz` & `tmp/dcspy-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcspy-2.1.0.tar", last modified: Tue May 30 20:51:40 2023, max compression
+gzip compressed data, was "dcspy-2.1.1.tar", last modified: Tue May 30 21:58:26 2023, max compression
```

## Comparing `dcspy-2.1.0.tar` & `dcspy-2.1.1.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 20:51:40.716291 dcspy-2.1.0/
--rw-rw-rw-   0        0        0     1092 2023-05-30 20:49:25.000000 dcspy-2.1.0/LICENSE.md
--rw-rw-rw-   0        0        0     6298 2023-05-30 20:51:40.716291 dcspy-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4776 2023-05-30 20:49:25.000000 dcspy-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 20:51:40.700665 dcspy-2.1.0/dcspy/
--rw-rw-rw-   0        0        0     7792 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/G13.png
--rw-rw-rw-   0        0        0    11136 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/G15v1.png
--rw-rw-rw-   0        0        0    11673 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/G15v2.png
--rw-rw-rw-   0        0        0    13267 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/G19.png
--rw-rw-rw-   0        0        0    10850 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/G510.png
--rw-rw-rw-   0        0        0     4819 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/__init__.py
--rw-rw-rw-   0        0        0    54818 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/aircraft.py
--rw-rw-rw-   0        0        0      476 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/config.yaml
--rw-rw-rw-   0        0        0     6139 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/dcsbios.py
--rw-rw-rw-   0        0        0    21694 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/dcspy.ico
--rw-rw-rw-   0        0        0    35819 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/dcspy.png
--rw-rw-rw-   0        0        0    21614 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/dcspy_white.ico
--rw-rw-rw-   0        0        0      236 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/license.txt
--rw-rw-rw-   0        0        0     1235 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/log.py
--rw-rw-rw-   0        0        0     7447 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/logitech.py
--rw-rw-rw-   0        0        0        0 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/py.typed
--rw-rw-rw-   0        0        0     1107 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/run.py
-drwxrwxrwx   0        0        0        0 2023-05-30 20:51:40.700665 dcspy-2.1.0/dcspy/sdk/
--rw-rw-rw-   0        0        0     1464 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/sdk/__init__.py
--rw-rw-rw-   0        0        0     8507 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/sdk/lcd_sdk.py
--rw-rw-rw-   0        0        0     7924 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/sdk/led_sdk.py
--rw-rw-rw-   0        0        0    31528 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/splash.png
--rw-rw-rw-   0        0        0     4343 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/starter.py
--rw-rw-rw-   0        0        0    43908 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/tk_gui.py
--rw-rw-rw-   0        0        0    12457 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-30 20:51:40.700665 dcspy-2.1.0/dcspy.egg-info/
--rw-rw-rw-   0        0        0     6298 2023-05-30 20:51:40.000000 dcspy-2.1.0/dcspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      790 2023-05-30 20:51:40.000000 dcspy-2.1.0/dcspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 20:51:40.000000 dcspy-2.1.0/dcspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-05-30 20:51:40.000000 dcspy-2.1.0/dcspy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      343 2023-05-30 20:51:40.000000 dcspy-2.1.0/dcspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-30 20:51:40.000000 dcspy-2.1.0/dcspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3463 2023-05-30 20:49:25.000000 dcspy-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 20:51:40.716291 dcspy-2.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-30 20:51:40.716291 dcspy-2.1.0/tests/
--rw-rw-rw-   0        0        0    18375 2023-05-30 20:49:25.000000 dcspy-2.1.0/tests/test_aircraft.py
--rw-rw-rw-   0        0        0      971 2023-05-30 20:49:25.000000 dcspy-2.1.0/tests/test_bios.py
--rw-rw-rw-   0        0        0     5197 2023-05-30 20:49:25.000000 dcspy-2.1.0/tests/test_dcsbios.py
--rw-rw-rw-   0        0        0     4908 2023-05-30 20:49:25.000000 dcspy-2.1.0/tests/test_lcd_sdk.py
--rw-rw-rw-   0        0        0     3586 2023-05-30 20:49:25.000000 dcspy-2.1.0/tests/test_led_sdk.py
--rw-rw-rw-   0        0        0     7035 2023-05-30 20:49:25.000000 dcspy-2.1.0/tests/test_logitech.py
--rw-rw-rw-   0        0        0     1323 2023-05-30 20:49:25.000000 dcspy-2.1.0/tests/test_starter.py
--rw-rw-rw-   0        0        0     8585 2023-05-30 20:49:25.000000 dcspy-2.1.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-30 21:58:26.254119 dcspy-2.1.1/
+-rw-rw-rw-   0        0        0     1092 2023-05-30 21:56:02.000000 dcspy-2.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0     6298 2023-05-30 21:58:26.254119 dcspy-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4776 2023-05-30 21:56:02.000000 dcspy-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 21:58:26.238493 dcspy-2.1.1/dcspy/
+-rw-rw-rw-   0        0        0     7792 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/G13.png
+-rw-rw-rw-   0        0        0    11136 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/G15v1.png
+-rw-rw-rw-   0        0        0    11673 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/G15v2.png
+-rw-rw-rw-   0        0        0    13267 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/G19.png
+-rw-rw-rw-   0        0        0    10850 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/G510.png
+-rw-rw-rw-   0        0        0     4819 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/__init__.py
+-rw-rw-rw-   0        0        0    54818 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/aircraft.py
+-rw-rw-rw-   0        0        0      476 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/config.yaml
+-rw-rw-rw-   0        0        0     6139 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/dcsbios.py
+-rw-rw-rw-   0        0        0    21694 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/dcspy.ico
+-rw-rw-rw-   0        0        0    35819 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/dcspy.png
+-rw-rw-rw-   0        0        0    21614 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/dcspy_white.ico
+-rw-rw-rw-   0        0        0    20420 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/falconded.ttf
+-rw-rw-rw-   0        0        0      236 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/license.txt
+-rw-rw-rw-   0        0        0     1235 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/log.py
+-rw-rw-rw-   0        0        0     7447 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/logitech.py
+-rw-rw-rw-   0        0        0        0 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/py.typed
+-rw-rw-rw-   0        0        0     1107 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/run.py
+drwxrwxrwx   0        0        0        0 2023-05-30 21:58:26.238493 dcspy-2.1.1/dcspy/sdk/
+-rw-rw-rw-   0        0        0     1464 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/sdk/__init__.py
+-rw-rw-rw-   0        0        0     8507 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/sdk/lcd_sdk.py
+-rw-rw-rw-   0        0        0     7924 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/sdk/led_sdk.py
+-rw-rw-rw-   0        0        0    31528 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/splash.png
+-rw-rw-rw-   0        0        0     4343 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/starter.py
+-rw-rw-rw-   0        0        0    43908 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/tk_gui.py
+-rw-rw-rw-   0        0        0    12457 2023-05-30 21:56:02.000000 dcspy-2.1.1/dcspy/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-30 21:58:26.238493 dcspy-2.1.1/dcspy.egg-info/
+-rw-rw-rw-   0        0        0     6298 2023-05-30 21:58:26.000000 dcspy-2.1.1/dcspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      810 2023-05-30 21:58:26.000000 dcspy-2.1.1/dcspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 21:58:26.000000 dcspy-2.1.1/dcspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-05-30 21:58:26.000000 dcspy-2.1.1/dcspy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      343 2023-05-30 21:58:26.000000 dcspy-2.1.1/dcspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-30 21:58:26.000000 dcspy-2.1.1/dcspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3477 2023-05-30 21:56:02.000000 dcspy-2.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 21:58:26.254119 dcspy-2.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 21:58:26.254119 dcspy-2.1.1/tests/
+-rw-rw-rw-   0        0        0    18375 2023-05-30 21:56:02.000000 dcspy-2.1.1/tests/test_aircraft.py
+-rw-rw-rw-   0        0        0      971 2023-05-30 21:56:02.000000 dcspy-2.1.1/tests/test_bios.py
+-rw-rw-rw-   0        0        0     5197 2023-05-30 21:56:02.000000 dcspy-2.1.1/tests/test_dcsbios.py
+-rw-rw-rw-   0        0        0     4908 2023-05-30 21:56:02.000000 dcspy-2.1.1/tests/test_lcd_sdk.py
+-rw-rw-rw-   0        0        0     3586 2023-05-30 21:56:02.000000 dcspy-2.1.1/tests/test_led_sdk.py
+-rw-rw-rw-   0        0        0     7035 2023-05-30 21:56:02.000000 dcspy-2.1.1/tests/test_logitech.py
+-rw-rw-rw-   0        0        0     1323 2023-05-30 21:56:02.000000 dcspy-2.1.1/tests/test_starter.py
+-rw-rw-rw-   0        0        0     8585 2023-05-30 21:56:02.000000 dcspy-2.1.1/tests/test_utils.py
```

### Comparing `dcspy-2.1.0/LICENSE.md` & `dcspy-2.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/PKG-INFO` & `dcspy-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcspy
-Version: 2.1.0
+Version: 2.1.1
 Summary: Integrating DCS (Digital Combat Simulator) planes with Logitech G13/G15/G510/G19 LCD
 Author: Michal Plichta
 Maintainer: Michal Plichta
 License: MIT License
 Project-URL: Homepage, https://github.com/emcek/dcspy
 Project-URL: Documentation, https://github.com/emcek/dcspy/wiki
 Project-URL: Repository, https://github.com/emcek/dcspy.git
@@ -27,15 +27,15 @@
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.md
 
-[![image](https://img.shields.io/badge/pypi-v2.1.0-blue.svg)](https://pypi.org/project/dcspy/)
+[![image](https://img.shields.io/badge/pypi-v2.1.1-blue.svg)](https://pypi.org/project/dcspy/)
 [![Python CI](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml/badge.svg?branch=master)](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml)
 [![Coverage Status](https://coveralls.io/repos/github/emcek/dcspy/badge.svg?branch=master)](https://coveralls.io/github/emcek/dcspy?branch=master)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/5270a4fc2ba24261a3bfa7361150e8ff)](https://www.codacy.com/gh/emcek/dcspy/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=emcek/dcspy&amp;utm_campaign=Badge_Grade)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE.md)
 [![Downloads](https://img.shields.io/github/downloads/emcek/dcspy/total?label=Downloads)](https://github.com/emcek/dcspy/releases)
 [![dcspy](https://snyk.io/advisor/python/dcspy/badge.svg)](https://snyk.io/advisor/python/dcspy)
 [![Patreon](https://img.shields.io/badge/Patreon-donate-ff424d?logo=patreon)](https://www.patreon.com/mplichta)
```

### Comparing `dcspy-2.1.0/README.md` & `dcspy-2.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![image](https://img.shields.io/badge/pypi-v2.1.0-blue.svg)](https://pypi.org/project/dcspy/)
+[![image](https://img.shields.io/badge/pypi-v2.1.1-blue.svg)](https://pypi.org/project/dcspy/)
 [![Python CI](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml/badge.svg?branch=master)](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml)
 [![Coverage Status](https://coveralls.io/repos/github/emcek/dcspy/badge.svg?branch=master)](https://coveralls.io/github/emcek/dcspy?branch=master)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/5270a4fc2ba24261a3bfa7361150e8ff)](https://www.codacy.com/gh/emcek/dcspy/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=emcek/dcspy&amp;utm_campaign=Badge_Grade)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE.md)
 [![Downloads](https://img.shields.io/github/downloads/emcek/dcspy/total?label=Downloads)](https://github.com/emcek/dcspy/releases)
 [![dcspy](https://snyk.io/advisor/python/dcspy/badge.svg)](https://snyk.io/advisor/python/dcspy)
 [![Patreon](https://img.shields.io/badge/Patreon-donate-ff424d?logo=patreon)](https://www.patreon.com/mplichta)
```

### Comparing `dcspy-2.1.0/dcspy/G13.png` & `dcspy-2.1.1/dcspy/G13.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/dcspy/G15v1.png` & `dcspy-2.1.1/dcspy/G15v1.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/dcspy/G15v2.png` & `dcspy-2.1.1/dcspy/G15v2.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/dcspy/G19.png` & `dcspy-2.1.1/dcspy/G19.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/dcspy/G510.png` & `dcspy-2.1.1/dcspy/G510.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/dcspy/__init__.py` & `dcspy-2.1.1/dcspy/__init__.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/dcspy/aircraft.py` & `dcspy-2.1.1/dcspy/aircraft.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/dcspy/dcsbios.py` & `dcspy-2.1.1/dcspy/dcsbios.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/dcspy/dcspy.ico` & `dcspy-2.1.1/dcspy/dcspy.ico`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/dcspy/dcspy.png` & `dcspy-2.1.1/dcspy/dcspy.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/dcspy/dcspy_white.ico` & `dcspy-2.1.1/dcspy/dcspy_white.ico`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/dcspy/log.py` & `dcspy-2.1.1/dcspy/log.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/dcspy/logitech.py` & `dcspy-2.1.1/dcspy/logitech.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/dcspy/run.py` & `dcspy-2.1.1/dcspy/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import customtkinter
 
 from dcspy import config
 from dcspy.tk_gui import DcspyGui
 from dcspy.utils import check_dcs_ver
 
 LOG = getLogger(__name__)
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 
 
 def run() -> None:
     """Start DCSpy GUI."""
     customtkinter.set_appearance_mode(config['theme_mode'])
     customtkinter.set_default_color_theme(config['theme_color'])
     LOG.info(f'dcspy {__version__} https://github.com/emcek/dcspy')
```

### Comparing `dcspy-2.1.0/dcspy/sdk/__init__.py` & `dcspy-2.1.1/dcspy/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/dcspy/sdk/lcd_sdk.py` & `dcspy-2.1.1/dcspy/sdk/lcd_sdk.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/dcspy/sdk/led_sdk.py` & `dcspy-2.1.1/dcspy/sdk/led_sdk.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/dcspy/splash.png` & `dcspy-2.1.1/dcspy/splash.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/dcspy/starter.py` & `dcspy-2.1.1/dcspy/starter.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from dcspy import MULTICAST_IP, RECV_ADDR, config
 from dcspy.dcsbios import ProtocolParser
 from dcspy.logitech import LogitechKeyboard
 from dcspy.utils import get_version_string
 
 LOG = getLogger(__name__)
 LOOP_FLAG = True
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 
 
 def _handle_connection(logi_keyboard: LogitechKeyboard, parser: ProtocolParser, sock: socket.socket, event: Event) -> None:
     """
     Handle main loop where all the magic is happened.
 
     :param logi_keyboard: type of Logitech keyboard with LCD
```

### Comparing `dcspy-2.1.0/dcspy/tk_gui.py` & `dcspy-2.1.1/dcspy/tk_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from dcspy import LCD_TYPES, LOCAL_APPDATA, config
 from dcspy.starter import dcspy_run
 from dcspy.utils import (ReleaseInfo, check_dcs_bios_entry, check_dcs_ver,
                          check_github_repo, check_ver_at_github, defaults_cfg,
                          download_file, get_default_yaml, get_version_string,
                          proc_is_running, save_cfg)
 
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 LOG = getLogger(__name__)
 
 
 class DcspyGui(tk.Frame):
     """Tkinter GUI."""
     def __init__(self, master: tk.Tk) -> None:
         """
```

### Comparing `dcspy-2.1.0/dcspy/utils.py` & `dcspy-2.1.1/dcspy/utils.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/dcspy.egg-info/PKG-INFO` & `dcspy-2.1.1/dcspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcspy
-Version: 2.1.0
+Version: 2.1.1
 Summary: Integrating DCS (Digital Combat Simulator) planes with Logitech G13/G15/G510/G19 LCD
 Author: Michal Plichta
 Maintainer: Michal Plichta
 License: MIT License
 Project-URL: Homepage, https://github.com/emcek/dcspy
 Project-URL: Documentation, https://github.com/emcek/dcspy/wiki
 Project-URL: Repository, https://github.com/emcek/dcspy.git
@@ -27,15 +27,15 @@
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.md
 
-[![image](https://img.shields.io/badge/pypi-v2.1.0-blue.svg)](https://pypi.org/project/dcspy/)
+[![image](https://img.shields.io/badge/pypi-v2.1.1-blue.svg)](https://pypi.org/project/dcspy/)
 [![Python CI](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml/badge.svg?branch=master)](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml)
 [![Coverage Status](https://coveralls.io/repos/github/emcek/dcspy/badge.svg?branch=master)](https://coveralls.io/github/emcek/dcspy?branch=master)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/5270a4fc2ba24261a3bfa7361150e8ff)](https://www.codacy.com/gh/emcek/dcspy/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=emcek/dcspy&amp;utm_campaign=Badge_Grade)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE.md)
 [![Downloads](https://img.shields.io/github/downloads/emcek/dcspy/total?label=Downloads)](https://github.com/emcek/dcspy/releases)
 [![dcspy](https://snyk.io/advisor/python/dcspy/badge.svg)](https://snyk.io/advisor/python/dcspy)
 [![Patreon](https://img.shields.io/badge/Patreon-donate-ff424d?logo=patreon)](https://www.patreon.com/mplichta)
```

### Comparing `dcspy-2.1.0/dcspy.egg-info/SOURCES.txt` & `dcspy-2.1.1/dcspy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 dcspy/__init__.py
 dcspy/aircraft.py
 dcspy/config.yaml
 dcspy/dcsbios.py
 dcspy/dcspy.ico
 dcspy/dcspy.png
 dcspy/dcspy_white.ico
+dcspy/falconded.ttf
 dcspy/license.txt
 dcspy/log.py
 dcspy/logitech.py
 dcspy/py.typed
 dcspy/run.py
 dcspy/splash.png
 dcspy/starter.py
```

### Comparing `dcspy-2.1.0/pyproject.toml` & `dcspy-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 
 [tool.setuptools.package-data]
 dcspy = [
     '*.txt',
     '*.yaml',
     '*.ico',
     '*.png',
+    '*.ttf',
     'py.typed',
 ]
 
 [tool.pytest.ini_options]
 addopts = ['--random', '-q']
 testpaths = ['tests']
 markers = ['dcsbios: marks tests for verfification of DCS-BIOS data']
```

### Comparing `dcspy-2.1.0/tests/test_aircraft.py` & `dcspy-2.1.1/tests/test_aircraft.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/tests/test_bios.py` & `dcspy-2.1.1/tests/test_bios.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/tests/test_dcsbios.py` & `dcspy-2.1.1/tests/test_dcsbios.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/tests/test_lcd_sdk.py` & `dcspy-2.1.1/tests/test_lcd_sdk.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/tests/test_led_sdk.py` & `dcspy-2.1.1/tests/test_led_sdk.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/tests/test_logitech.py` & `dcspy-2.1.1/tests/test_logitech.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/tests/test_starter.py` & `dcspy-2.1.1/tests/test_starter.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.1.0/tests/test_utils.py` & `dcspy-2.1.1/tests/test_utils.py`

 * *Files identical despite different names*

