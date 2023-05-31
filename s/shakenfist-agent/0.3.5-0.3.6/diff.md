# Comparing `tmp/shakenfist-agent-0.3.5.tar.gz` & `tmp/shakenfist-agent-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shakenfist-agent-0.3.5.tar", last modified: Tue Mar 14 06:50:44 2023, max compression
+gzip compressed data, was "shakenfist-agent-0.3.6.tar", last modified: Wed May 31 07:25:32 2023, max compression
```

## Comparing `shakenfist-agent-0.3.5.tar` & `shakenfist-agent-0.3.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-03-14 06:50:44.323469 shakenfist-agent-0.3.5/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      266 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.5/.coveragerc
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-03-14 06:50:44.315469 shakenfist-agent-0.3.5/.github/
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-03-14 06:50:44.323469 shakenfist-agent-0.3.5/.github/workflows/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1301 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.5/.github/workflows/python-unit-tests.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       55 2022-03-31 06:16:40.000000 shakenfist-agent-0.3.5/.stestr.conf
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       60 2023-03-14 06:50:44.000000 shakenfist-agent-0.3.5/AUTHORS
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.5/LICENSE
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      907 2023-03-14 06:50:44.323469 shakenfist-agent-0.3.5/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      190 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.5/README.md
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      857 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.5/release.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      174 2022-08-07 23:05:27.000000 shakenfist-agent-0.3.5/requirements.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      729 2023-03-14 06:50:44.323469 shakenfist-agent-0.3.5/setup.cfg
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1148 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.5/setup.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-03-14 06:50:44.323469 shakenfist-agent-0.3.5/shakenfist_agent/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.5/shakenfist_agent/__init__.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-03-14 06:50:44.323469 shakenfist-agent-0.3.5/shakenfist_agent/commandline/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     7825 2023-03-14 06:50:30.000000 shakenfist-agent-0.3.5/shakenfist_agent/commandline/daemon.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      613 2022-08-07 23:05:27.000000 shakenfist-agent-0.3.5/shakenfist_agent/main.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8638 2023-03-12 21:15:16.000000 shakenfist-agent-0.3.5/shakenfist_agent/protocol.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-03-14 06:50:44.323469 shakenfist-agent-0.3.5/shakenfist_agent/tests/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-03-31 06:16:40.000000 shakenfist-agent-0.3.5/shakenfist_agent/tests/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4848 2023-03-08 21:01:13.000000 shakenfist-agent-0.3.5/shakenfist_agent/tests/test_daemon.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3815 2023-03-06 10:12:52.000000 shakenfist-agent-0.3.5/shakenfist_agent/tests/test_protocol.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-03-14 06:50:44.323469 shakenfist-agent-0.3.5/shakenfist_agent.egg-info/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      907 2023-03-14 06:50:44.000000 shakenfist-agent-0.3.5/shakenfist_agent.egg-info/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      738 2023-03-14 06:50:44.000000 shakenfist-agent-0.3.5/shakenfist_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-03-14 06:50:44.000000 shakenfist-agent-0.3.5/shakenfist_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       56 2023-03-14 06:50:44.000000 shakenfist-agent-0.3.5/shakenfist_agent.egg-info/entry_points.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-03-14 06:50:44.000000 shakenfist-agent-0.3.5/shakenfist_agent.egg-info/not-zip-safe
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       46 2023-03-14 06:50:44.000000 shakenfist-agent-0.3.5/shakenfist_agent.egg-info/pbr.json
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       83 2023-03-14 06:50:44.000000 shakenfist-agent-0.3.5/shakenfist_agent.egg-info/requires.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       17 2023-03-14 06:50:44.000000 shakenfist-agent-0.3.5/shakenfist_agent.egg-info/top_level.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      164 2022-08-07 23:05:27.000000 shakenfist-agent-0.3.5/test-requirements.txt
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-03-14 06:50:44.323469 shakenfist-agent-0.3.5/tools/
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      573 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.5/tools/flake8wrap.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      867 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.5/tox.ini
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 07:25:32.138316 shakenfist-agent-0.3.6/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      266 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.6/.coveragerc
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 07:25:32.126316 shakenfist-agent-0.3.6/.github/
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 07:25:32.134316 shakenfist-agent-0.3.6/.github/workflows/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1301 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.6/.github/workflows/python-unit-tests.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       55 2022-03-31 06:16:40.000000 shakenfist-agent-0.3.6/.stestr.conf
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       60 2023-05-31 07:25:31.000000 shakenfist-agent-0.3.6/AUTHORS
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.6/LICENSE
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      907 2023-05-31 07:25:32.138316 shakenfist-agent-0.3.6/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      190 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.6/README.md
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      857 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.6/release.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      174 2022-08-07 23:05:27.000000 shakenfist-agent-0.3.6/requirements.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      729 2023-05-31 07:25:32.138316 shakenfist-agent-0.3.6/setup.cfg
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1148 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.6/setup.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 07:25:32.134316 shakenfist-agent-0.3.6/shakenfist_agent/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-03-16 08:23:02.000000 shakenfist-agent-0.3.6/shakenfist_agent/__init__.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 07:25:32.134316 shakenfist-agent-0.3.6/shakenfist_agent/commandline/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8357 2023-05-31 07:25:02.000000 shakenfist-agent-0.3.6/shakenfist_agent/commandline/daemon.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      613 2022-08-07 23:05:27.000000 shakenfist-agent-0.3.6/shakenfist_agent/main.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8638 2023-03-12 21:15:16.000000 shakenfist-agent-0.3.6/shakenfist_agent/protocol.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 07:25:32.138316 shakenfist-agent-0.3.6/shakenfist_agent/tests/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-03-31 06:16:40.000000 shakenfist-agent-0.3.6/shakenfist_agent/tests/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4848 2023-03-08 21:01:13.000000 shakenfist-agent-0.3.6/shakenfist_agent/tests/test_daemon.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3815 2023-03-06 10:12:52.000000 shakenfist-agent-0.3.6/shakenfist_agent/tests/test_protocol.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 07:25:32.134316 shakenfist-agent-0.3.6/shakenfist_agent.egg-info/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      907 2023-05-31 07:25:31.000000 shakenfist-agent-0.3.6/shakenfist_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      738 2023-05-31 07:25:32.000000 shakenfist-agent-0.3.6/shakenfist_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-05-31 07:25:31.000000 shakenfist-agent-0.3.6/shakenfist_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       56 2023-05-31 07:25:31.000000 shakenfist-agent-0.3.6/shakenfist_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-05-31 07:25:31.000000 shakenfist-agent-0.3.6/shakenfist_agent.egg-info/not-zip-safe
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       46 2023-05-31 07:25:31.000000 shakenfist-agent-0.3.6/shakenfist_agent.egg-info/pbr.json
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       83 2023-05-31 07:25:31.000000 shakenfist-agent-0.3.6/shakenfist_agent.egg-info/requires.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       17 2023-05-31 07:25:31.000000 shakenfist-agent-0.3.6/shakenfist_agent.egg-info/top_level.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      164 2022-08-07 23:05:27.000000 shakenfist-agent-0.3.6/test-requirements.txt
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 07:25:32.138316 shakenfist-agent-0.3.6/tools/
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      573 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.6/tools/flake8wrap.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      867 2023-03-06 10:11:43.000000 shakenfist-agent-0.3.6/tox.ini
```

### Comparing `shakenfist-agent-0.3.5/.github/workflows/python-unit-tests.yml` & `shakenfist-agent-0.3.6/.github/workflows/python-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.5/LICENSE` & `shakenfist-agent-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.5/PKG-INFO` & `shakenfist-agent-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakenfist-agent
-Version: 0.3.5
+Version: 0.3.6
 Summary: An in-guest agent for instances running on Shaken Fist
 Home-page: https://madebymikal.com/shakenfist
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: Python side channel agent for Shaken Fist
         =========================================
```

### Comparing `shakenfist-agent-0.3.5/release.sh` & `shakenfist-agent-0.3.6/release.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.5/setup.cfg` & `shakenfist-agent-0.3.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.5/setup.py` & `shakenfist-agent-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.5/shakenfist_agent/commandline/daemon.py` & `shakenfist-agent-0.3.6/shakenfist_agent/commandline/daemon.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from linux_utils.fstab import find_mounted_filesystems
 import multiprocessing
 import os
 from oslo_concurrency import processutils
 from pbr.version import VersionInfo
 import psutil
 import select
+import shutil
 import signal
 import sys
 import time
 
 from shakenfist_agent import protocol
 
 
@@ -29,14 +30,16 @@
 
         self.watched_files = {}
         self.executing_commands = []
 
         self.add_command('is-system-running', self.is_system_running)
         self.add_command('gather-facts', self.gather_facts)
         self.add_command('put-file-response', self.put_file_response)
+        self.add_command('chmod', self.chmod)
+        self.add_command('chown', self.chown)
         self.add_command('get-file', self.get_file)
         self.add_command('watch-file', self.watch_file)
         self.add_command('execute', self.execute)
 
         self.send_packet({
             'command': 'agent-start',
             'message': 'version %s' % VersionInfo('shakenfist_agent').version_string(),
@@ -110,14 +113,28 @@
             del self.incomplete_file_gets[path]
             self.log.with_fields(packet).info('File put complete')
             return
 
         d = base64.b64decode(packet['chunk'])
         self.incomplete_file_gets[path]['flo'].write(d)
 
+    def chmod(self, packet):
+        os.chmod(packet['path'], packet['mode'])
+        self.send_packet({
+            'command': 'chmod-response',
+            'path': packet['path']
+        })
+
+    def chown(self, packet):
+        shutil.chown(packet['path'], user=packet.get('user'), group=packet.get('group'))
+        self.send_packet({
+            'command': 'chown-response',
+            'path': packet['path']
+        })
+
     def get_file(self, packet):
         self._send_file('get-file', packet.get('path'))
 
     def watch_file(self, packet):
         path = packet.get('path')
         if not self._path_is_a_file('watch-file', path):
             return
```

### Comparing `shakenfist-agent-0.3.5/shakenfist_agent/main.py` & `shakenfist-agent-0.3.6/shakenfist_agent/main.py`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.5/shakenfist_agent/protocol.py` & `shakenfist-agent-0.3.6/shakenfist_agent/protocol.py`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.5/shakenfist_agent/tests/test_daemon.py` & `shakenfist-agent-0.3.6/shakenfist_agent/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.5/shakenfist_agent/tests/test_protocol.py` & `shakenfist-agent-0.3.6/shakenfist_agent/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.5/shakenfist_agent.egg-info/PKG-INFO` & `shakenfist-agent-0.3.6/shakenfist_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakenfist-agent
-Version: 0.3.5
+Version: 0.3.6
 Summary: An in-guest agent for instances running on Shaken Fist
 Home-page: https://madebymikal.com/shakenfist
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: Python side channel agent for Shaken Fist
         =========================================
```

### Comparing `shakenfist-agent-0.3.5/shakenfist_agent.egg-info/SOURCES.txt` & `shakenfist-agent-0.3.6/shakenfist_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.5/tools/flake8wrap.sh` & `shakenfist-agent-0.3.6/tools/flake8wrap.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-agent-0.3.5/tox.ini` & `shakenfist-agent-0.3.6/tox.ini`

 * *Files identical despite different names*

