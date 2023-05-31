# Comparing `tmp/ovos-microphone-plugin-alsa-0.0.0a2.tar.gz` & `tmp/ovos-microphone-plugin-alsa-0.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-microphone-plugin-alsa-0.0.0a2.tar", last modified: Wed May 17 19:45:06 2023, max compression
+gzip compressed data, was "ovos-microphone-plugin-alsa-0.0.0a3.tar", last modified: Fri May 19 23:58:06 2023, max compression
```

## Comparing `ovos-microphone-plugin-alsa-0.0.0a2.tar` & `ovos-microphone-plugin-alsa-0.0.0a3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:45:06.813443 ovos-microphone-plugin-alsa-0.0.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-17 19:44:57.000000 ovos-microphone-plugin-alsa-0.0.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-17 19:44:57.000000 ovos-microphone-plugin-alsa-0.0.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-17 19:45:06.813443 ovos-microphone-plugin-alsa-0.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-17 19:44:57.000000 ovos-microphone-plugin-alsa-0.0.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:45:06.809443 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa/
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-17 19:44:57.000000 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-17 19:45:00.000000 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:45:06.809443 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-17 19:45:06.000000 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-17 19:45:06.000000 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:45:06.000000 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-17 19:45:06.000000 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-17 19:45:06.000000 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 19:45:06.000000 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:45:06.000000 ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:45:06.813443 ovos-microphone-plugin-alsa-0.0.0a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3121 2023-05-17 19:44:57.000000 ovos-microphone-plugin-alsa-0.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:58:06.506909 ovos-microphone-plugin-alsa-0.0.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-19 23:57:58.000000 ovos-microphone-plugin-alsa-0.0.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-19 23:57:58.000000 ovos-microphone-plugin-alsa-0.0.0a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-19 23:58:06.506909 ovos-microphone-plugin-alsa-0.0.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 23:57:58.000000 ovos-microphone-plugin-alsa-0.0.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:58:06.502909 ovos-microphone-plugin-alsa-0.0.0a3/ovos_microphone_plugin_alsa/
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-19 23:57:58.000000 ovos-microphone-plugin-alsa-0.0.0a3/ovos_microphone_plugin_alsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-19 23:58:01.000000 ovos-microphone-plugin-alsa-0.0.0a3/ovos_microphone_plugin_alsa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 23:58:06.506909 ovos-microphone-plugin-alsa-0.0.0a3/ovos_microphone_plugin_alsa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-19 23:58:06.000000 ovos-microphone-plugin-alsa-0.0.0a3/ovos_microphone_plugin_alsa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-19 23:58:06.000000 ovos-microphone-plugin-alsa-0.0.0a3/ovos_microphone_plugin_alsa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 23:58:06.000000 ovos-microphone-plugin-alsa-0.0.0a3/ovos_microphone_plugin_alsa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-19 23:58:06.000000 ovos-microphone-plugin-alsa-0.0.0a3/ovos_microphone_plugin_alsa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-19 23:58:06.000000 ovos-microphone-plugin-alsa-0.0.0a3/ovos_microphone_plugin_alsa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-19 23:58:06.000000 ovos-microphone-plugin-alsa-0.0.0a3/ovos_microphone_plugin_alsa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 23:58:06.000000 ovos-microphone-plugin-alsa-0.0.0a3/ovos_microphone_plugin_alsa.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 23:58:06.506909 ovos-microphone-plugin-alsa-0.0.0a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3121 2023-05-19 23:57:58.000000 ovos-microphone-plugin-alsa-0.0.0a3/setup.py
```

### Comparing `ovos-microphone-plugin-alsa-0.0.0a2/LICENSE` & `ovos-microphone-plugin-alsa-0.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-microphone-plugin-alsa-0.0.0a2/PKG-INFO` & `ovos-microphone-plugin-alsa-0.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-microphone-plugin-alsa
-Version: 0.0.0a2
+Version: 0.0.0a3
 Summary: A alsa microphone implementation for OVOS
 Home-page: https://github.com/OpenVoiceOS/ovos-microphone-plugin-alsa
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: ovos plugin listener microphone alsa
```

### Comparing `ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa/__init__.py` & `ovos-microphone-plugin-alsa-0.0.0a3/ovos_microphone_plugin_alsa/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-microphone-plugin-alsa-0.0.0a2/ovos_microphone_plugin_alsa.egg-info/PKG-INFO` & `ovos-microphone-plugin-alsa-0.0.0a3/ovos_microphone_plugin_alsa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-microphone-plugin-alsa
-Version: 0.0.0a2
+Version: 0.0.0a3
 Summary: A alsa microphone implementation for OVOS
 Home-page: https://github.com/OpenVoiceOS/ovos-microphone-plugin-alsa
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: ovos plugin listener microphone alsa
```

### Comparing `ovos-microphone-plugin-alsa-0.0.0a2/setup.py` & `ovos-microphone-plugin-alsa-0.0.0a3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         if 'MYCROFT_LOOSE_REQUIREMENTS' in os.environ:
             print('USING LOOSE REQUIREMENTS!')
             requirements = [r.replace('==', '>=').replace('~=', '>=') for r in requirements]
         return [pkg for pkg in requirements
                 if pkg.strip() and not pkg.startswith("#")]
 
 
-PLUGIN_ENTRY_POINT = 'ovos-microphone-plugin-alsa = ovos_microphone_plugin_alsa:alsaMicrophone'
+PLUGIN_ENTRY_POINT = 'ovos-microphone-plugin-alsa = ovos_microphone_plugin_alsa:AlsaMicrophone'
 
 
 setup(
     name='ovos-microphone-plugin-alsa',
     version=get_version(),
     description='A alsa microphone implementation for OVOS',
     url='https://github.com/OpenVoiceOS/ovos-microphone-plugin-alsa',
```

