# Comparing `tmp/ovos-PHAL-plugin-homeassistant-0.0.2a4.tar.gz` & `tmp/ovos-PHAL-plugin-homeassistant-0.0.2a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-homeassistant-0.0.2a4.tar", last modified: Tue May 30 20:31:11 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-homeassistant-0.0.2a5.tar", last modified: Wed May 31 20:14:30 2023, max compression
```

## Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a4.tar` & `ovos-PHAL-plugin-homeassistant-0.0.2a5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:31:11.553775 ovos-PHAL-plugin-homeassistant-0.0.2a4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 20:31:01.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-30 20:31:11.553775 ovos-PHAL-plugin-homeassistant-0.0.2a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-30 20:31:01.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:31:11.553775 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant/
--rw-r--r--   0 runner    (1001) docker     (123)    35559 2023-05-30 20:31:01.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-30 20:31:04.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:31:11.553775 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-30 20:31:11.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-30 20:31:11.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:31:11.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 20:31:11.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-30 20:31:11.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-30 20:31:11.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:31:11.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:31:11.549775 ovos-PHAL-plugin-homeassistant-0.0.2a4/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:31:11.553775 ovos-PHAL-plugin-homeassistant-0.0.2a4/res/desktop/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-30 20:31:01.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/res/desktop/ovos-phal-homeassistant.desktop
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:31:11.553775 ovos-PHAL-plugin-homeassistant-0.0.2a4/res/icon/
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-30 20:31:01.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/res/icon/ovos-phal-homeassistant.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 20:31:11.553775 ovos-PHAL-plugin-homeassistant-0.0.2a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-30 20:31:01.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:30.839793 ovos-PHAL-plugin-homeassistant-0.0.2a5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 20:14:17.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-31 20:14:30.839793 ovos-PHAL-plugin-homeassistant-0.0.2a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-31 20:14:17.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:30.839793 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant/
+-rw-r--r--   0 runner    (1001) docker     (123)    35559 2023-05-31 20:14:17.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-31 20:14:22.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:30.839793 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-31 20:14:30.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-31 20:14:30.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:14:30.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 20:14:30.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-31 20:14:30.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 20:14:30.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:14:30.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:30.835793 ovos-PHAL-plugin-homeassistant-0.0.2a5/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:30.839793 ovos-PHAL-plugin-homeassistant-0.0.2a5/res/desktop/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-31 20:14:17.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/res/desktop/ovos-phal-homeassistant.desktop
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:30.839793 ovos-PHAL-plugin-homeassistant-0.0.2a5/res/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-31 20:14:17.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/res/icon/ovos-phal-homeassistant.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 20:14:30.839793 ovos-PHAL-plugin-homeassistant-0.0.2a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-31 20:14:17.000000 ovos-PHAL-plugin-homeassistant-0.0.2a5/setup.py
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a4/LICENSE` & `ovos-PHAL-plugin-homeassistant-0.0.2a5/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a4/PKG-INFO` & `ovos-PHAL-plugin-homeassistant-0.0.2a5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-homeassistant
-Version: 0.0.2a4
+Version: 0.0.2a5
 Summary: Notifications and Widgets plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a4/README.md` & `ovos-PHAL-plugin-homeassistant-0.0.2a5/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant/__init__.py` & `ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO` & `ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-homeassistant
-Version: 0.0.2a4
+Version: 0.0.2a5
 Summary: Notifications and Widgets plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-homeassistant-0.0.2a5/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a4/res/icon/ovos-phal-homeassistant.svg` & `ovos-PHAL-plugin-homeassistant-0.0.2a5/res/icon/ovos-phal-homeassistant.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a4/setup.py` & `ovos-PHAL-plugin-homeassistant-0.0.2a5/setup.py`

 * *Files identical despite different names*

