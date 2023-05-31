# Comparing `tmp/ovos-stt-http-server-0.0.2a7.tar.gz` & `tmp/ovos-stt-http-server-0.0.2a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-stt-http-server-0.0.2a7.tar", last modified: Tue May 30 20:36:35 2023, max compression
+gzip compressed data, was "ovos-stt-http-server-0.0.2a8.tar", last modified: Wed May 31 12:06:34 2023, max compression
```

## Comparing `ovos-stt-http-server-0.0.2a7.tar` & `ovos-stt-http-server-0.0.2a8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:36:35.836945 ovos-stt-http-server-0.0.2a7/
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-30 20:36:35.836945 ovos-stt-http-server-0.0.2a7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:36:35.832945 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:36:35.836945 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/
--rw-r--r--   0 runner    (1001) docker     (123)    58605 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/ca.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    54765 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/de.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    50925 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/en.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    55341 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/es.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    57453 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/fr.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    62637 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/it.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    68781 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/nl.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    48813 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/pt.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    67821 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/uk.mp3
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/gradio_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:36:35.836945 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/ovos_stt_http_server.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 20:36:35.836945 ovos-stt-http-server-0.0.2a7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3049 2023-05-30 20:36:35.000000 ovos-stt-http-server-0.0.2a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:06:34.238623 ovos-stt-http-server-0.0.2a8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-31 12:06:33.000000 ovos-stt-http-server-0.0.2a8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-31 12:06:34.238623 ovos-stt-http-server-0.0.2a8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:06:34.238623 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-31 12:06:33.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-31 12:06:33.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:06:34.238623 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)    58605 2023-05-31 12:06:33.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/ca.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    54765 2023-05-31 12:06:33.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/de.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    50925 2023-05-31 12:06:33.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/en.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    55341 2023-05-31 12:06:33.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/es.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    57453 2023-05-31 12:06:33.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/fr.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    62637 2023-05-31 12:06:33.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/it.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    68781 2023-05-31 12:06:33.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/nl.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    48813 2023-05-31 12:06:33.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/pt.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    67821 2023-05-31 12:06:33.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/uk.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-31 12:06:33.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/gradio_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-31 12:06:33.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:06:34.238623 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-31 12:06:34.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-31 12:06:34.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:06:34.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-31 12:06:34.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-31 12:06:34.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-31 12:06:34.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:06:34.000000 ovos-stt-http-server-0.0.2a8/ovos_stt_http_server.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 12:06:34.238623 ovos-stt-http-server-0.0.2a8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3049 2023-05-31 12:06:33.000000 ovos-stt-http-server-0.0.2a8/setup.py
```

### Comparing `ovos-stt-http-server-0.0.2a7/LICENSE.md` & `ovos-stt-http-server-0.0.2a8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a7/PKG-INFO` & `ovos-stt-http-server-0.0.2a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-stt-http-server
-Version: 0.0.2a7
+Version: 0.0.2a8
 Summary: simple aiohttp server to host OpenVoiceOS stt plugins as a service
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-http-server
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: plugin STT OVOS OpenVoiceOS
 Platform: UNKNOWN
```

### Comparing `ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/__init__.py` & `ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/__main__.py` & `ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/__main__.py`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/ca.mp3` & `ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/ca.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/de.mp3` & `ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/de.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/en.mp3` & `ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/en.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/es.mp3` & `ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/es.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/fr.mp3` & `ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/fr.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/it.mp3` & `ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/it.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/nl.mp3` & `ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/nl.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/pt.mp3` & `ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/pt.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/audio/uk.mp3` & `ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/audio/uk.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a7/ovos_stt_http_server/gradio_app.py` & `ovos-stt-http-server-0.0.2a8/ovos_stt_http_server/gradio_app.py`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a7/ovos_stt_http_server.egg-info/PKG-INFO` & `ovos-stt-http-server-0.0.2a8/ovos_stt_http_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-stt-http-server
-Version: 0.0.2a7
+Version: 0.0.2a8
 Summary: simple aiohttp server to host OpenVoiceOS stt plugins as a service
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-http-server
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: plugin STT OVOS OpenVoiceOS
 Platform: UNKNOWN
```

### Comparing `ovos-stt-http-server-0.0.2a7/ovos_stt_http_server.egg-info/SOURCES.txt` & `ovos-stt-http-server-0.0.2a8/ovos_stt_http_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a7/setup.py` & `ovos-stt-http-server-0.0.2a8/setup.py`

 * *Files identical despite different names*

