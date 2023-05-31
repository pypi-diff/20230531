# Comparing `tmp/lnxlink-2023.5.0.tar.gz` & `tmp/lnxlink-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnxlink-2023.5.0.tar", last modified: Fri Apr 28 21:27:57 2023, max compression
+gzip compressed data, was "lnxlink-2023.6.0.tar", last modified: Wed May 31 20:44:02 2023, max compression
```

## Comparing `lnxlink-2023.5.0.tar` & `lnxlink-2023.6.0.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:27:57.010689 lnxlink-2023.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-04-28 21:27:57.010689 lnxlink-2023.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:27:57.010689 lnxlink-2023.5.0/lnxlink/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12861 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5692 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:27:57.010689 lnxlink-2023.5.0/lnxlink/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/boot_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/camera_used.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/disk_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/idle.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/keep_alive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/microphone_used.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/network_download.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/network_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/notify.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/nvidia_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/required_restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/screen_onoff.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/send_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/suspend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/sys_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/webcam.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/modules/xdg_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/lnxlink/system_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:27:57.010689 lnxlink-2023.5.0/lnxlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-04-28 21:27:56.000000 lnxlink-2023.5.0/lnxlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-28 21:27:57.000000 lnxlink-2023.5.0/lnxlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 21:27:56.000000 lnxlink-2023.5.0/lnxlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 21:27:56.000000 lnxlink-2023.5.0/lnxlink.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-28 21:27:56.000000 lnxlink-2023.5.0/lnxlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 21:27:56.000000 lnxlink-2023.5.0/lnxlink.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1132 2023-04-28 21:27:43.000000 lnxlink-2023.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-28 21:27:57.010689 lnxlink-2023.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:44:02.037674 lnxlink-2023.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-05-31 20:44:02.037674 lnxlink-2023.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:44:02.033674 lnxlink-2023.6.0/lnxlink/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14770 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5692 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:44:02.037674 lnxlink-2023.6.0/lnxlink/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/boot_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/camera_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/disk_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/keep_alive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/microphone_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/notify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/nvidia_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/required_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/screen_onoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/send_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/suspend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/sys_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/webcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/modules/xdg_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/lnxlink/system_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:44:02.037674 lnxlink-2023.6.0/lnxlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-05-31 20:44:01.000000 lnxlink-2023.6.0/lnxlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-31 20:44:02.000000 lnxlink-2023.6.0/lnxlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:44:01.000000 lnxlink-2023.6.0/lnxlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-31 20:44:01.000000 lnxlink-2023.6.0/lnxlink.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-31 20:44:01.000000 lnxlink-2023.6.0/lnxlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 20:44:01.000000 lnxlink-2023.6.0/lnxlink.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1132 2023-05-31 20:43:48.000000 lnxlink-2023.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-31 20:44:02.037674 lnxlink-2023.6.0/setup.cfg
```

### Comparing `lnxlink-2023.5.0/LICENSE.md` & `lnxlink-2023.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.5.0/PKG-INFO` & `lnxlink-2023.6.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: lnxlink
-Version: 2023.5.0
-Summary: Internet Of Things (IOT) integration with Linux using MQTT
-Home-page: https://bkbilly.github.io/lnxlink
-Author-email: bkbilly <bkbilly@hotmail.com>
-Project-URL: Source Code, https://github.com/bkbilly/lnxlink
-Project-URL: Home Page, https://bkbilly.github.io/lnxlink
-Keywords: lnxlink
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 [![license](https://img.shields.io/badge/license-MIT-blue)](LICENSE.md)
 [![OS - Linux](https://img.shields.io/badge/OS-Linux-blue?logo=linux&logoColor=white)]()
 [![Python 3.5](https://img.shields.io/badge/Python-3.5-blue?logo=python&logoColor=white)]()
 [![PyPI](https://img.shields.io/pypi/v/lnxlink?logo=pypi&logoColor=white)](https://pypi.python.org/pypi/lnxlink/)
 [![Last commit](https://img.shields.io/github/last-commit/bkbilly/lnxlink?color=blue&logo=github&logoColor=white)]()
 
 <img align="right" width="170" height="100" src="https://github.com/bkbilly/lnxlink/blob/master/logo.png?raw=true">
@@ -155,15 +139,15 @@
 data:
   media_player: media_player.desktop_linux
 target:
   entity_id: camera.demo_camera
 ```
 
 ### Create a custom module
-You can create custom modules and import them to your configuration with their full path. Check out examples [here](https://github.com/bkbilly/lnxlink/tree/master/lnxlink/modules) and this is an example of how to add the `mytest` module to your configuration.
+You can create custom modules and import them to your configuration with their full path. Check out examples [here](lnxlink/modules) and this is an example of how to add the `mytest` module to your configuration.
 ```yaml
 modules:
 - /home/user/mytest.py
 ```
 
 
 # FAQ
@@ -180,24 +164,69 @@
 If you want to create the service from scratch, you will have to disable the running service and start lnxlink again:
 ```shell
 systemctl --user disable lnxlink.service
 lnxlink -c config.yaml
 ```
 
 ## One of my integration is not working
-Make sure you have these packages on your system:
- - xdotool
- - shutdown
- - systemctl
- - xprintidle
- - xdg-open
- - upower
- - xset
+By default all modules are automatically loaded. This happens when the modules section is empty like this:
+```yaml
+modules:
+```
+You should select the ones you want to load. All supported modules can be found [here](lnxlink/modules) and the configuration should look like this:
+```yaml
+modules:
+- notify
+- camera_used
+- idle
+- keep_alive
+- shutdown
+- brightness
+```
+
+## LNXlink doesn't become unavailable after shutdown
+Just before LNXlink stops, it sends to MQTT an OFF command, but sometimes it doesn't stop gracefouly.
+To fix this, you will have to create an automation on Home Assistant which checks for when was the last time one of the sensors got a value and if it exceeds it sends the OFF command to the MQTT server.
+
+This is an example of the automation which checks events for the idle sensor:
+```yaml
+alias: lnxlink powered down
+description: ""
+mode: single
+trigger:
+  - platform: template
+    value_template: >-
+      {{ (now() | as_timestamp -
+      states.sensor.desktop_linux_idle.last_changed | as_timestamp) >
+      10 }}
+condition: []
+action:
+  - service: mqtt.publish
+    data:
+      qos: 0
+      retain: true
+      topic: lnxlink/desktop-linux/lwt
+      payload: "OFF"
+```
 
 ## Use Boot Select addon
 This control needs to run as root, but it's not recomended to run lnxlink as a super user. To fix this, you need to allow the command `grub-reboot` to run without asking for password:
 ```bash
 # Edit the sudoers file:
 sudo visudo
 # Add this line at the end (replace USER with your username):
 USER ALL=(ALL) NOPASSWD: /usr/sbin/grub-reboot
 ```
+
+## How to help the development
+In case you have found the solution to a bug or you want to create a new feature, follow these instructions to get you started:
+```bash
+# Install system dependencies
+sudo apt install git patchelf meson libdbus-glib-1-dev libglib2.0-dev libasound2-dev python3-pip
+# Fork my repository and then download it
+git clone git@github.com:<yourusername>/lnxlink.git
+# Install lnxlink as editable package
+cd lnxlink
+pip3 install -e .
+# Run it manually
+lnxlink -c config.yaml
+```
```

### Comparing `lnxlink-2023.5.0/README.md` & `lnxlink-2023.6.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: lnxlink
+Version: 2023.6.0
+Summary: Internet Of Things (IOT) integration with Linux using MQTT
+Home-page: https://bkbilly.github.io/lnxlink
+Author-email: bkbilly <bkbilly@hotmail.com>
+Project-URL: Source Code, https://github.com/bkbilly/lnxlink
+Project-URL: Home Page, https://bkbilly.github.io/lnxlink
+Keywords: lnxlink
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Unix
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 [![license](https://img.shields.io/badge/license-MIT-blue)](LICENSE.md)
 [![OS - Linux](https://img.shields.io/badge/OS-Linux-blue?logo=linux&logoColor=white)]()
 [![Python 3.5](https://img.shields.io/badge/Python-3.5-blue?logo=python&logoColor=white)]()
 [![PyPI](https://img.shields.io/pypi/v/lnxlink?logo=pypi&logoColor=white)](https://pypi.python.org/pypi/lnxlink/)
 [![Last commit](https://img.shields.io/github/last-commit/bkbilly/lnxlink?color=blue&logo=github&logoColor=white)]()
 
 <img align="right" width="170" height="100" src="https://github.com/bkbilly/lnxlink/blob/master/logo.png?raw=true">
@@ -139,15 +155,15 @@
 data:
   media_player: media_player.desktop_linux
 target:
   entity_id: camera.demo_camera
 ```
 
 ### Create a custom module
-You can create custom modules and import them to your configuration with their full path. Check out examples [here](https://github.com/bkbilly/lnxlink/tree/master/lnxlink/modules) and this is an example of how to add the `mytest` module to your configuration.
+You can create custom modules and import them to your configuration with their full path. Check out examples [here](lnxlink/modules) and this is an example of how to add the `mytest` module to your configuration.
 ```yaml
 modules:
 - /home/user/mytest.py
 ```
 
 
 # FAQ
@@ -164,24 +180,69 @@
 If you want to create the service from scratch, you will have to disable the running service and start lnxlink again:
 ```shell
 systemctl --user disable lnxlink.service
 lnxlink -c config.yaml
 ```
 
 ## One of my integration is not working
-Make sure you have these packages on your system:
- - xdotool
- - shutdown
- - systemctl
- - xprintidle
- - xdg-open
- - upower
- - xset
+By default all modules are automatically loaded. This happens when the modules section is empty like this:
+```yaml
+modules:
+```
+You should select the ones you want to load. All supported modules can be found [here](lnxlink/modules) and the configuration should look like this:
+```yaml
+modules:
+- notify
+- camera_used
+- idle
+- keep_alive
+- shutdown
+- brightness
+```
+
+## LNXlink doesn't become unavailable after shutdown
+Just before LNXlink stops, it sends to MQTT an OFF command, but sometimes it doesn't stop gracefouly.
+To fix this, you will have to create an automation on Home Assistant which checks for when was the last time one of the sensors got a value and if it exceeds it sends the OFF command to the MQTT server.
+
+This is an example of the automation which checks events for the idle sensor:
+```yaml
+alias: lnxlink powered down
+description: ""
+mode: single
+trigger:
+  - platform: template
+    value_template: >-
+      {{ (now() | as_timestamp -
+      states.sensor.desktop_linux_idle.last_changed | as_timestamp) >
+      10 }}
+condition: []
+action:
+  - service: mqtt.publish
+    data:
+      qos: 0
+      retain: true
+      topic: lnxlink/desktop-linux/lwt
+      payload: "OFF"
+```
 
 ## Use Boot Select addon
 This control needs to run as root, but it's not recomended to run lnxlink as a super user. To fix this, you need to allow the command `grub-reboot` to run without asking for password:
 ```bash
 # Edit the sudoers file:
 sudo visudo
 # Add this line at the end (replace USER with your username):
 USER ALL=(ALL) NOPASSWD: /usr/sbin/grub-reboot
 ```
+
+## How to help the development
+In case you have found the solution to a bug or you want to create a new feature, follow these instructions to get you started:
+```bash
+# Install system dependencies
+sudo apt install git patchelf meson libdbus-glib-1-dev libglib2.0-dev libasound2-dev python3-pip
+# Fork my repository and then download it
+git clone git@github.com:<yourusername>/lnxlink.git
+# Install lnxlink as editable package
+cd lnxlink
+pip3 install -e .
+# Run it manually
+lnxlink -c config.yaml
+```
```

### Comparing `lnxlink-2023.5.0/lnxlink/__main__.py` & `lnxlink-2023.6.0/lnxlink/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 import os
 import yaml
 import time
-import threading
 import json
+import distro
+import threading
 import traceback
 import importlib.metadata
 import platform
 import argparse
 import paho.mqtt.client as mqtt
 from . import modules
 from . import config
@@ -45,14 +46,22 @@
         if pub_data is None:
             return
         if isinstance(pub_data, bool):
             if pub_data is True:
                 pub_data = 'ON'
             if pub_data is False:
                 pub_data = 'OFF'
+        if type(pub_data) == dict:
+            if all(v is None for v in pub_data.values()):
+                return
+        if type(pub_data) == list:
+            if all(v is None for v in pub_data):
+                return
+        if pub_data is None:
+            return
         if type(pub_data) in [dict, list]:
             pub_data = json.dumps(pub_data)
         self.client.publish(
             topic,
             payload=pub_data,
             retain=self.config['mqtt']['lwt']['retain']
         )
@@ -186,16 +195,16 @@
 
         discovery = discovery_template.copy()
         discovery['name'] = f"{self.config['mqtt']['clientId']} {addon.name}"
         discovery['unique_id'] = f"{self.config['mqtt']['clientId']}_{service}"
         discovery['state_topic'] = state_topic
         discovery['topic'] = state_topic
         if addon.getInfo.__annotations__.get('return') == dict:
-            discovery['json_attributes_topic'] = state_topic
             discovery['value_template'] = "{{ value_json.status }}"
+            discovery['json_attributes_topic'] = state_topic
             discovery['json_attributes_template'] = "{{ value_json | tojson }}"
         if hasattr(addon, 'icon'):
             discovery['icon'] = addon.icon
         if hasattr(addon, 'unit'):
             discovery['unit_of_measurement'] = addon.unit
         if hasattr(addon, 'title'):
             discovery['title'] = addon.title
@@ -203,51 +212,79 @@
             discovery['entity_picture'] = addon.entity_picture
         if hasattr(addon, 'device_class'):
             discovery['device_class'] = addon.device_class
         if hasattr(addon, 'state_class'):
             discovery['state_class'] = addon.state_class
 
         sensor_type = getattr(addon, 'sensor_type', None)
+        if sensor_type in ['sensor', 'binary_sensor']:
+            discovery['expire_after'] = self.config.get('update_interval', 5) * 2
         if sensor_type is not None:
             self.client.publish(
                 f"homeassistant/{sensor_type}/lnxlink/{discovery['unique_id']}/config",
                 payload=json.dumps(discovery),
                 retain=self.config['mqtt']['lwt']['retain'])
 
     def setup_discovery_control(self, discovery_template, addon, service, control_name, options):
         '''Send discovery information on Home Assistant for controls'''
         subtopic = addon.name.lower().replace(' ', '/')
         state_topic = f"{self.pref_topic}/monitor_controls/{subtopic}"
+        command_topic = f"{self.pref_topic}/commands/{service}/{control_name.replace(' ', '_')}/"
         discovery = discovery_template.copy()
         discovery['name'] = f"{self.config['mqtt']['clientId']} {control_name}"
         discovery['unique_id'] = f"{self.config['mqtt']['clientId']}_{control_name.lower().replace(' ', '_')}"
         discovery['enabled_by_default'] = options.get('enabled', True)
-        discovery["command_topic"] = f"{self.pref_topic}/commands/{service}/{control_name.replace(' ', '_')}/"
         if 'value_template' in options:
             discovery["value_template"] = options['value_template']
+            if options['type'] != 'camera':
+                discovery['json_attributes_topic'] = state_topic
+                discovery['json_attributes_template'] = "{{ value_json | tojson }}"
         if 'icon' in options:
             discovery['icon'] = options.get('icon', '')
-
-        if options['type'] == 'button':
+        if 'unit' in options:
+            discovery['unit_of_measurement'] = options.get('unit', '')
+        if 'title' in options:
+            discovery['title'] = options.get('title', '')
+        if 'entity_picture' in options:
+            discovery['entity_picture'] = options.get('entity_picture', '')
+        if 'device_class' in options:
+            discovery['device_class'] = options.get('device_class', '')
+        if 'state_class' in options:
+            discovery['state_class'] = options.get('state_class', '')
+        if 'entity_category' in options:
+            discovery['entity_category'] = options.get('entity_category', '')
+
+        if options['type'] in ['sensor', 'binary_sensor']:
+            discovery['state_topic'] = state_topic
+            discovery['expire_after'] = self.config.get('update_interval', 5) * 2
+        elif options['type'] in ['camera', 'update']:
+            discovery['state_topic'] = state_topic
+        elif options['type'] == 'button':
+            discovery["command_topic"] = command_topic
             discovery['state_topic'] = f"{self.pref_topic}/lwt"
         elif options['type'] == 'switch':
+            discovery["command_topic"] = command_topic
             discovery["state_topic"] = state_topic
             discovery["payload_off"] = "OFF"
             discovery["payload_on"] = "ON"
         elif options['type'] == 'text':
+            discovery["command_topic"] = command_topic
             discovery["state_topic"] = state_topic
         elif options['type'] == 'number':
+            discovery["command_topic"] = command_topic
             discovery["state_topic"] = state_topic
             discovery["min"] = options.get('min', 1)
             discovery["max"] = options.get('max', 100)
             discovery["step"] = options.get('step', 1)
         elif options['type'] == 'select':
+            discovery["command_topic"] = command_topic
             discovery["state_topic"] = state_topic
             discovery["options"] = addon.options
         else:
+            print("Not supported:", options['type'])
             return
         self.client.publish(
             f"homeassistant/{options['type']}/lnxlink/{discovery['unique_id']}/config",
             payload=json.dumps(discovery),
             retain=self.config['mqtt']['lwt']['retain'])
 
     def setup_discovery(self):
@@ -257,16 +294,17 @@
                 "topic": f"{self.pref_topic}/lwt",
                 "payload_available": "ON",
                 "payload_not_available": "OFF",
             },
             "device": {
                 "identifiers": [self.config['mqtt']['clientId']],
                 "name": self.config['mqtt']['clientId'],
-                "model": self.config['mqtt']['prefix'],
-                "manufacturer": f"LNXlink {version}"
+                "model": f"{distro.name()} {distro.version()}",
+                "manufacturer": f"LNXlink",
+                "sw_version": version,
             },
         }
         for service, addon in self.Addons.items():
             addon = self.Addons[service]
             if hasattr(addon, 'getInfo'):
                 try:
                     self.setup_discovery_monitoring(discovery_template, addon, service)
```

### Comparing `lnxlink-2023.5.0/lnxlink/config.py` & `lnxlink-2023.6.0/lnxlink/config.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.5.0/lnxlink/consts.py` & `lnxlink-2023.6.0/lnxlink/consts.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.5.0/lnxlink/modules/__init__.py` & `lnxlink-2023.6.0/lnxlink/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.5.0/lnxlink/modules/boot_select.py` & `lnxlink-2023.6.0/lnxlink/modules/boot_select.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.5.0/lnxlink/modules/brightness.py` & `lnxlink-2023.6.0/lnxlink/modules/brightness.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.5.0/lnxlink/modules/camera_used.py` & `lnxlink-2023.6.0/lnxlink/modules/camera_used.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.5.0/lnxlink/modules/disk_usage.py` & `lnxlink-2023.6.0/lnxlink/modules/disk_usage.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.5.0/lnxlink/modules/keep_alive.py` & `lnxlink-2023.6.0/lnxlink/modules/keep_alive.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.5.0/lnxlink/modules/media.py` & `lnxlink-2023.6.0/lnxlink/modules/media.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.5.0/lnxlink/modules/microphone_used.py` & `lnxlink-2023.6.0/lnxlink/modules/microphone_used.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import glob
 import subprocess
 import json
+import re
 
 
 class Addon():
 
     def __init__(self, lnxlink):
         self.name = 'Microphone used'
         self.icon = 'mdi:microphone'
         self.sensor_type = 'binary_sensor'
 
         self.use_pactl = subprocess.run(
-            f"which pactl && pactl -f json list",
+            f"which pactl && pactl -f json list short source-outputs",
             shell=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE).returncode == 0
 
 
     def getInfo(self):
         if self.use_pactl:
-            stdout = subprocess.run(f"pactl -f json list", shell=True,
+            stdout = subprocess.run(f"pactl -f json list short source-outputs", shell=True,
                                     stdout=subprocess.PIPE,
                                     stderr=subprocess.PIPE).stdout.decode("UTF-8")
+            # Replace 0,00 values with 0.00
+            stdout = re.sub(r'(\s*[+-]?[0-9]+),([0-9]+\s*)',r'\1.\2', stdout)
             data = json.loads(stdout)
-            if 'source_outputs' in data and len(data['source_outputs']) > 0:
+            if len(data) > 0:
                 return 'ON'
             return "OFF"
         else:
             mics = glob.glob('/proc/asound/**/*c/sub*/status', recursive=True)
             for mic in mics:
                 with open(mic) as mic_content:
                     mic_status = mic_content.read().strip().lower()
```

### Comparing `lnxlink-2023.5.0/lnxlink/modules/notify.py` & `lnxlink-2023.6.0/lnxlink/modules/notify.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.5.0/lnxlink/modules/nvidia_gpu.py` & `lnxlink-2023.6.0/lnxlink/modules/nvidia_gpu.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.5.0/lnxlink/modules/screen_onoff.py` & `lnxlink-2023.6.0/lnxlink/modules/screen_onoff.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.5.0/lnxlink/modules/screenshot.py` & `lnxlink-2023.6.0/lnxlink/modules/screenshot.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         return False
 
     def exposedControls(self):
         return {
             "Screenshot": {
                 "type": "switch",
                 "icon": "mdi:monitor-screenshot",
+                "entity_category": "config",
             }
         }
 
     def startControl(self, topic, data):
         if data.lower() == 'off':
             self.sct = None
         elif data.lower() == 'on':
```

### Comparing `lnxlink-2023.5.0/lnxlink/modules/sys_updates.py` & `lnxlink-2023.6.0/lnxlink/modules/sys_updates.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,20 +2,27 @@
 import time
 
 
 class Addon():
 
     def __init__(self, lnxlink):
         self.name = 'System Updates'
-        self.icon = 'mdi:package-variant'
-        self.sensor_type = 'binary_sensor'
         self.last_time = 0
         self.update_interval = 7200  # Check for updates every 2 hours
 
-    def getInfo(self):
+    def exposedControls(self):
+        return {
+            "System Updates": {
+                "type": "binary_sensor",
+                "icon": "mdi:package-variant",
+                "entity_category": "diagnostic",
+            },
+        }
+
+    def getControlInfo(self):
         packages = [
             {
                 'command': 'apt list --upgradable | wc -l',
                 'logic': '> 2',
             },
             {
                 'command': 'yum -q updateinfo list updates | wc -l',
```

### Comparing `lnxlink-2023.5.0/lnxlink/modules/update.py` & `lnxlink-2023.6.0/lnxlink/modules/update.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,31 +4,37 @@
 import traceback
 
 
 class Addon():
 
     def __init__(self, lnxlink):
         self.name = 'LNXlink'
-        self.icon = 'mdi:update'
-        self.device_class = "firmware"
-        self.title = "LNXlink"
-        self.entity_picture = "https://github.com/bkbilly/lnxlink/raw/master/logo.png?raw=true"
-        self.sensor_type = "update"
-
         self.last_time = 0
         self.update_interval = 86400  # Check for updates every 24 hours
         version = importlib.metadata.version('lnxlink')
         self.message = {
           "installed_version": version,
           "latest_version": version,
           "release_summary": "",
           "release_url": "https://github.com/bkbilly/lnxlink/releases/latest",
         }
 
-    def getInfo(self):
+    def exposedControls(self):
+        return {
+            "Update": {
+                "type": "update",
+                "title": "LNXlink",
+                "icon": "mdi:update",
+                "device_class": "firmware",
+                "entity_category": "diagnostic",
+                "entity_picture": "https://github.com/bkbilly/lnxlink/raw/master/logo.png?raw=true",
+            },
+        }
+
+    def getControlInfo(self):
         cur_time = time.time()
         if cur_time - self.last_time > self.update_interval:
             self._latest_version()
             self.last_time = cur_time
 
         return self.message
```

### Comparing `lnxlink-2023.5.0/lnxlink/modules/webcam.py` & `lnxlink-2023.6.0/lnxlink/modules/webcam.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         return False
 
     def exposedControls(self):
         return {
             "Webcam": {
                 "type": "switch",
                 "icon": "mdi:webcam",
+                "entity_category": "config",
             }
         }
 
     def startControl(self, topic, data):
         if data.lower() == 'off':
             self.vid.release()
             self.vid = None
```

### Comparing `lnxlink-2023.5.0/lnxlink/system_monitor.py` & `lnxlink-2023.6.0/lnxlink/system_monitor.py`

 * *Files identical despite different names*

### Comparing `lnxlink-2023.5.0/lnxlink.egg-info/PKG-INFO` & `lnxlink-2023.6.0/lnxlink.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnxlink
-Version: 2023.5.0
+Version: 2023.6.0
 Summary: Internet Of Things (IOT) integration with Linux using MQTT
 Home-page: https://bkbilly.github.io/lnxlink
 Author-email: bkbilly <bkbilly@hotmail.com>
 Project-URL: Source Code, https://github.com/bkbilly/lnxlink
 Project-URL: Home Page, https://bkbilly.github.io/lnxlink
 Keywords: lnxlink
 Classifier: Programming Language :: Python :: 3
@@ -155,15 +155,15 @@
 data:
   media_player: media_player.desktop_linux
 target:
   entity_id: camera.demo_camera
 ```
 
 ### Create a custom module
-You can create custom modules and import them to your configuration with their full path. Check out examples [here](https://github.com/bkbilly/lnxlink/tree/master/lnxlink/modules) and this is an example of how to add the `mytest` module to your configuration.
+You can create custom modules and import them to your configuration with their full path. Check out examples [here](lnxlink/modules) and this is an example of how to add the `mytest` module to your configuration.
 ```yaml
 modules:
 - /home/user/mytest.py
 ```
 
 
 # FAQ
@@ -180,24 +180,69 @@
 If you want to create the service from scratch, you will have to disable the running service and start lnxlink again:
 ```shell
 systemctl --user disable lnxlink.service
 lnxlink -c config.yaml
 ```
 
 ## One of my integration is not working
-Make sure you have these packages on your system:
- - xdotool
- - shutdown
- - systemctl
- - xprintidle
- - xdg-open
- - upower
- - xset
+By default all modules are automatically loaded. This happens when the modules section is empty like this:
+```yaml
+modules:
+```
+You should select the ones you want to load. All supported modules can be found [here](lnxlink/modules) and the configuration should look like this:
+```yaml
+modules:
+- notify
+- camera_used
+- idle
+- keep_alive
+- shutdown
+- brightness
+```
+
+## LNXlink doesn't become unavailable after shutdown
+Just before LNXlink stops, it sends to MQTT an OFF command, but sometimes it doesn't stop gracefouly.
+To fix this, you will have to create an automation on Home Assistant which checks for when was the last time one of the sensors got a value and if it exceeds it sends the OFF command to the MQTT server.
+
+This is an example of the automation which checks events for the idle sensor:
+```yaml
+alias: lnxlink powered down
+description: ""
+mode: single
+trigger:
+  - platform: template
+    value_template: >-
+      {{ (now() | as_timestamp -
+      states.sensor.desktop_linux_idle.last_changed | as_timestamp) >
+      10 }}
+condition: []
+action:
+  - service: mqtt.publish
+    data:
+      qos: 0
+      retain: true
+      topic: lnxlink/desktop-linux/lwt
+      payload: "OFF"
+```
 
 ## Use Boot Select addon
 This control needs to run as root, but it's not recomended to run lnxlink as a super user. To fix this, you need to allow the command `grub-reboot` to run without asking for password:
 ```bash
 # Edit the sudoers file:
 sudo visudo
 # Add this line at the end (replace USER with your username):
 USER ALL=(ALL) NOPASSWD: /usr/sbin/grub-reboot
 ```
+
+## How to help the development
+In case you have found the solution to a bug or you want to create a new feature, follow these instructions to get you started:
+```bash
+# Install system dependencies
+sudo apt install git patchelf meson libdbus-glib-1-dev libglib2.0-dev libasound2-dev python3-pip
+# Fork my repository and then download it
+git clone git@github.com:<yourusername>/lnxlink.git
+# Install lnxlink as editable package
+cd lnxlink
+pip3 install -e .
+# Run it manually
+lnxlink -c config.yaml
+```
```

### Comparing `lnxlink-2023.5.0/lnxlink.egg-info/SOURCES.txt` & `lnxlink-2023.6.0/lnxlink.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 lnxlink/modules/cpu.py
 lnxlink/modules/disk_usage.py
 lnxlink/modules/idle.py
 lnxlink/modules/keep_alive.py
 lnxlink/modules/media.py
 lnxlink/modules/memory.py
 lnxlink/modules/microphone_used.py
-lnxlink/modules/network_download.py
-lnxlink/modules/network_upload.py
+lnxlink/modules/network.py
 lnxlink/modules/notify.py
 lnxlink/modules/nvidia_gpu.py
 lnxlink/modules/required_restart.py
 lnxlink/modules/restart.py
 lnxlink/modules/screen_onoff.py
 lnxlink/modules/screenshot.py
 lnxlink/modules/send_keys.py
```

### Comparing `lnxlink-2023.5.0/pyproject.toml` & `lnxlink-2023.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name              = "lnxlink"
-version           = "2023.5.0"
+version           = "2023.6.0"
 description       = "Internet Of Things (IOT) integration with Linux using MQTT"
 readme            = "README.md"
 keywords          = ["lnxlink"]
 requires-python   = ">=3.7.0"
 authors     = [
     {name="bkbilly", email="bkbilly@hotmail.com"}
 ]
```

