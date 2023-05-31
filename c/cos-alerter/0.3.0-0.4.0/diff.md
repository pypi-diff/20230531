# Comparing `tmp/cos-alerter-0.3.0.tar.gz` & `tmp/cos-alerter-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cos-alerter-0.3.0.tar", last modified: Mon May  1 12:53:08 2023, max compression
+gzip compressed data, was "cos-alerter-0.4.0.tar", last modified: Wed May 31 14:36:34 2023, max compression
```

## Comparing `cos-alerter-0.3.0.tar` & `cos-alerter-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-01 12:53:08.597228 cos-alerter-0.3.0/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)    11357 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/LICENSE
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1923 2023-05-01 12:53:08.597228 cos-alerter-0.3.0/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1300 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/README.md
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-01 12:53:08.597228 cos-alerter-0.3.0/cos_alerter/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     6442 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/cos_alerter/alerter.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     3738 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/cos_alerter/daemon.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1126 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/cos_alerter/logging.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1554 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/cos_alerter/server.py
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-01 12:53:08.597228 cos-alerter-0.3.0/cos_alerter.egg-info/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1923 2023-05-01 12:53:08.000000 cos-alerter-0.3.0/cos_alerter.egg-info/PKG-INFO
--rw-rw-r--   0 dylan     (1000) dylan     (1000)      398 2023-05-01 12:53:08.000000 cos-alerter-0.3.0/cos_alerter.egg-info/SOURCES.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)        1 2023-05-01 12:53:08.000000 cos-alerter-0.3.0/cos_alerter.egg-info/dependency_links.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)       56 2023-05-01 12:53:08.000000 cos-alerter-0.3.0/cos_alerter.egg-info/entry_points.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)       93 2023-05-01 12:53:08.000000 cos-alerter-0.3.0/cos_alerter.egg-info/requires.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)       12 2023-05-01 12:53:08.000000 cos-alerter-0.3.0/cos_alerter.egg-info/top_level.txt
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     1518 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/pyproject.toml
--rw-rw-r--   0 dylan     (1000) dylan     (1000)       38 2023-05-01 12:53:08.597228 cos-alerter-0.3.0/setup.cfg
-drwxrwxr-x   0 dylan     (1000) dylan     (1000)        0 2023-05-01 12:53:08.597228 cos-alerter-0.3.0/tests/
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     6547 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/tests/test_alerter.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     2522 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/tests/test_daemon.py
--rw-rw-r--   0 dylan     (1000) dylan     (1000)     2607 2023-05-01 11:30:40.000000 cos-alerter-0.3.0/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:36:34.383051 cos-alerter-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 14:36:24.000000 cos-alerter-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-31 14:36:24.000000 cos-alerter-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-31 14:36:34.383051 cos-alerter-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-31 14:36:24.000000 cos-alerter-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:36:34.379051 cos-alerter-0.4.0/cos_alerter/
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-31 14:36:24.000000 cos-alerter-0.4.0/cos_alerter/alerter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-31 14:36:24.000000 cos-alerter-0.4.0/cos_alerter/config-defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-31 14:36:24.000000 cos-alerter-0.4.0/cos_alerter/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-31 14:36:24.000000 cos-alerter-0.4.0/cos_alerter/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-31 14:36:24.000000 cos-alerter-0.4.0/cos_alerter/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:36:34.383051 cos-alerter-0.4.0/cos_alerter/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   328338 2023-05-31 14:36:24.000000 cos-alerter-0.4.0/cos_alerter/static/vanilla-framework-version-3.14.0.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:36:34.383051 cos-alerter-0.4.0/cos_alerter/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-31 14:36:24.000000 cos-alerter-0.4.0/cos_alerter/templates/dashboard.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:36:34.383051 cos-alerter-0.4.0/cos_alerter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-31 14:36:34.000000 cos-alerter-0.4.0/cos_alerter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-31 14:36:34.000000 cos-alerter-0.4.0/cos_alerter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:36:34.000000 cos-alerter-0.4.0/cos_alerter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 14:36:34.000000 cos-alerter-0.4.0/cos_alerter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-31 14:36:34.000000 cos-alerter-0.4.0/cos_alerter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 14:36:34.000000 cos-alerter-0.4.0/cos_alerter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-31 14:36:24.000000 cos-alerter-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:36:34.383051 cos-alerter-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:36:34.383051 cos-alerter-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-31 14:36:24.000000 cos-alerter-0.4.0/tests/test_alerter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-31 14:36:24.000000 cos-alerter-0.4.0/tests/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-31 14:36:24.000000 cos-alerter-0.4.0/tests/test_server.py
```

### Comparing `cos-alerter-0.3.0/LICENSE` & `cos-alerter-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cos-alerter-0.3.0/PKG-INFO` & `cos-alerter-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cos-alerter
-Version: 0.3.0
+Version: 0.4.0
 Summary: A watcher for Alertmanager
 Author-email: Dylan Stephano-Shachter <dylan.stephano-shachter@canonical.com>
 Project-URL: Homepage, https://github.com/canonical/cos-alerter
 Project-URL: Bug Tracker, https://github.com/canonical/cos-alerter/issues
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
```

### Comparing `cos-alerter-0.3.0/README.md` & `cos-alerter-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cos-alerter-0.3.0/cos_alerter/alerter.py` & `cos-alerter-0.4.0/cos_alerter/alerter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # Copyright 2023 Canonical Ltd.
 # See LICENSE file for licensing details.
 
 """Main logic for COS Alerter."""
 
 import datetime
 import logging
+import os
 import textwrap
 import threading
 import time
+import typing
 from pathlib import Path
 
 import apprise
 import durationpy
 import yaml
 
 logger = logging.getLogger(__name__)
@@ -26,24 +28,43 @@
 
     def set_path(self, path: str):
         """Set the config file path."""
         self.path = Path(path)
 
     def reload(self):
         """Reload config values from the disk."""
-        with open(self.path, "r") as f:
+        with open(
+            os.path.join(os.path.dirname(os.path.realpath(__file__)), "config-defaults.yaml")
+        ) as f:
             self.data = yaml.safe_load(f)
+        with open(self.path, "r") as f:
+            user_data = yaml.safe_load(f)
+        deep_update(self.data, user_data)
         self.data["watch"]["down_interval"] = durationpy.from_str(
             self.data["watch"]["down_interval"]
         ).total_seconds()
         self.data["notify"]["repeat_interval"] = durationpy.from_str(
             self.data["notify"]["repeat_interval"]
         ).total_seconds()
 
 
+def deep_update(base: dict, new: typing.Optional[dict]):
+    """Deep dict update.
+
+    Same as dict.update() except it recurses into dubdicts.
+    """
+    if new is None:
+        return
+    for key in base:
+        if key in new and type(base[key]) == dict:
+            deep_update(base[key], new[key])
+        elif key in new:
+            base[key] = new[key]
+
+
 config = Config()
 state = {}
 
 
 class AlerterState:
     """Class representing the state of COS Alerter.
 
@@ -103,14 +124,20 @@
             alert_time = None if config["watch"]["wait_for_first_connection"] else current_time
             state["clients"][client] = {
                 "lock": threading.Lock(),
                 "alert_time": alert_time,
                 "notify_time": None,
             }
 
+    @staticmethod
+    def clients():
+        """Return a list of clientids."""
+        for client in state["clients"]:
+            yield client
+
     def reset_alert_timeout(self):
         """Set the "last alert time" to right now."""
         logger.debug("Resetting alert timeout for %s.", self.clientid)
         self.data["alert_time"] = time.monotonic()
 
     def _set_notify_time(self):
         """Set the "last notification time" to right now."""
@@ -126,49 +153,62 @@
         """Determine if a notification has been previously sent within the repeat interval."""
         return (
             state["clients"][self.clientid]["notify_time"]
             and not time.monotonic() - self.data["notify_time"]
             > config["notify"]["repeat_interval"]
         )
 
-    def _last_alert_datetime(self) -> datetime.datetime:
+    def last_alert_datetime(self) -> typing.Optional[datetime.datetime]:
         """Return the actual time the last alert was received.
 
         Returns:
             A datetime.datetime object representing the time of the last alert.
         """
+        if self.data["alert_time"] is None or self.data["alert_time"] == self.start_time:
+            return None
         actual_alert_timestamp = (self.data["alert_time"] - self.start_time) + self.start_date
         return datetime.datetime.fromtimestamp(actual_alert_timestamp, datetime.timezone.utc)
 
     def notify(self):
         """Send out notifications of the missing Alertmanager if necessary."""
         # If we have already notified recently, do nothing.
         if self._recently_notified():
             logger.debug("Recently notified. Skipping.")
             return
 
         logger.info("Sending notifications for %s.", self.clientid)
         self._set_notify_time()
-        last_alert_time = self._last_alert_datetime().isoformat()
+        last_alert_datetime = self.last_alert_datetime()
+        last_alert_string = (
+            f"since {last_alert_datetime.isoformat()} UTC"
+            if last_alert_datetime is not None
+            else "ever"
+        )
         title = "**Alertmanager is Down!**"
         body = textwrap.dedent(
             f"""
             Your Alertmanager instance: {self.clientid} seems to be down!
-            It has not alerted COS-Alerter since {last_alert_time} UTC.
+            It has not alerted COS-Alerter {last_alert_string}.
             """
         )
 
         # Sending notifications can be a long operation so handle that in a separate thread.
         # This avoids interfering with the execution of the main loop.
         notify_thread = threading.Thread(
             target=send_notifications, kwargs={"title": title, "body": body}
         )
         notify_thread.start()
 
 
+def now_datetime():
+    """Return the current datetime using the monotonic clock."""
+    now_timestamp = (time.monotonic() - state["start_time"]) + state["start_date"]
+    return datetime.datetime.fromtimestamp(now_timestamp, datetime.timezone.utc)
+
+
 def up_time():
     """Return number of seconds that the daemon has been running."""
     return time.monotonic() - state["start_time"]
 
 
 def send_notifications(title: str, body: str):
     """Send a notification to all receivers."""
```

### Comparing `cos-alerter-0.3.0/cos_alerter/daemon.py` & `cos-alerter-0.4.0/cos_alerter/daemon.py`

 * *Files identical despite different names*

### Comparing `cos-alerter-0.3.0/cos_alerter/logging.py` & `cos-alerter-0.4.0/cos_alerter/logging.py`

 * *Files identical despite different names*

### Comparing `cos-alerter-0.3.0/cos_alerter/server.py` & `cos-alerter-0.4.0/cos_alerter/server.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,47 @@
 # Copyright 2023 Canonical Ltd.
 # See LICENSE file for licensing details.
 
 """HTTP server for COS Alerter."""
 
 import logging
 
-from flask import Flask, request
+import timeago
+from flask import Flask, render_template, request
 from prometheus_flask_exporter import PrometheusMetrics
 
-from .alerter import AlerterState, config
+from .alerter import AlerterState, config, now_datetime
 
 app = Flask(__name__)
 metrics = PrometheusMetrics(app)
 logger = logging.getLogger(__name__)
 
 
+@app.route("/", methods=["GET"])
+def dashboard():
+    """Endpoint for the COS Alerter dashboard."""
+    clients = []
+    now = now_datetime()
+    for clientid in AlerterState.clients():
+        with AlerterState(clientid) as state:
+            last_alert = state.last_alert_datetime()
+            alert_time = timeago.format(last_alert, now) if last_alert is not None else "never"
+            status = "up" if not state.is_down() else "down"
+            if last_alert is None:
+                status = "unknown"
+            clients.append(
+                {
+                    "clientid": clientid,
+                    "status": status,
+                    "alert_time": alert_time,
+                }
+            )
+    return render_template("dashboard.html", clients=clients)
+
+
 @app.route("/alive", methods=["POST"])
 def alive():
     """Endpoint for Alertmanager instances to send their heartbeat alerts."""
     # TODO Decide if we should validate the request.
     params = request.args
     clientid_list = params.getlist("clientid")  # params is a werkzeug.datastructures.MultiDict
     if len(clientid_list) < 1:
```

### Comparing `cos-alerter-0.3.0/cos_alerter.egg-info/PKG-INFO` & `cos-alerter-0.4.0/cos_alerter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cos-alerter
-Version: 0.3.0
+Version: 0.4.0
 Summary: A watcher for Alertmanager
 Author-email: Dylan Stephano-Shachter <dylan.stephano-shachter@canonical.com>
 Project-URL: Homepage, https://github.com/canonical/cos-alerter
 Project-URL: Bug Tracker, https://github.com/canonical/cos-alerter/issues
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
```

### Comparing `cos-alerter-0.3.0/pyproject.toml` & `cos-alerter-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cos-alerter"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="Dylan Stephano-Shachter", email="dylan.stephano-shachter@canonical.com" }
 ]
 description = "A watcher for Alertmanager"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -19,16 +19,17 @@
   "Development Status :: 3 - Alpha",
 ]
 dependencies = [
   "apprise~=1.3",
   "durationpy",
   "flask~=2.2",
   "prometheus_flask_exporter~=0.22",
+  "pyyaml~=6.0",
+  "timeago~=1.0",
   "waitress~=2.1",
-  "pyyaml~=6.0"
 ]
 
 [project.urls]
 Homepage = "https://github.com/canonical/cos-alerter"
 "Bug Tracker" = "https://github.com/canonical/cos-alerter/issues"
 
 [project.scripts]
```

### Comparing `cos-alerter-0.3.0/tests/test_alerter.py` & `cos-alerter-0.4.0/tests/test_alerter.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,56 +3,52 @@
 
 import textwrap
 import threading
 import unittest.mock
 
 import apprise
 import freezegun
-import pytest
 import yaml
+from helpers import DESTINATIONS
 
 from cos_alerter.alerter import AlerterState, config, send_test_notification, up_time
 
-DESTINATIONS = [
-    "mailtos://user:pass@domain/?to=example-0@example.com,example-1@example.com",
-    "slack://xoxb-1234-1234-4ddbc191d40ee098cbaae6f3523ada2d/#general",
-]
-
-CONFIG = {
-    "watch": {
-        "down_interval": "5m",
-        "wait_for_first_connection": False,
-        "clients": ["client0"],
-    },
-    "notify": {
-        "destinations": DESTINATIONS,
-        "repeat_interval": "1h",
-    },
-}
-
-
-@pytest.fixture
-def fake_fs(fs):
-    fs.create_file("/etc/cos-alerter.yaml")
-    with open("/etc/cos-alerter.yaml", "w") as f:
-        f.write(yaml.dump(CONFIG))
-    config.set_path("/etc/cos-alerter.yaml")
-    config.reload()
-    return fs
-
 
 def assert_notifications(notify_mock, add_mock, title, body):
     add_mock.assert_has_calls([unittest.mock.call(x) for x in DESTINATIONS])
     notify_mock.assert_called_with(title=title, body=body)
 
 
 def test_config_gets_item(fake_fs):
     assert config["watch"]["down_interval"] == 300
 
 
+def test_config_default_empty_file(fake_fs):
+    with open("/etc/cos-alerter.yaml", "w") as f:
+        f.write("")
+    config.reload()
+    assert config["watch"]["down_interval"] == 300
+
+
+def test_config_default_partial_file(fake_fs):
+    conf = yaml.dump({"log_level": "info"})
+    with open("/etc/cos-alerter.yaml", "w") as f:
+        f.write(conf)
+    config.reload()
+    assert config["watch"]["down_interval"] == 300
+
+
+def test_config_default_override(fake_fs):
+    conf = yaml.dump({"watch": {"down_interval": "1m"}})
+    with open("/etc/cos-alerter.yaml", "w") as f:
+        f.write(conf)
+    config.reload()
+    assert config["watch"]["down_interval"] == 60
+
+
 @freezegun.freeze_time("2023-01-01")
 @unittest.mock.patch("time.monotonic")
 def test_initialize(monotonic_mock, fake_fs):
     monotonic_mock.return_value = 1000
     AlerterState.initialize()
     state = AlerterState(clientid="client0")
     with state:
@@ -167,15 +163,15 @@
     assert_notifications(
         notify_mock,
         add_mock,
         title="**Alertmanager is Down!**",
         body=textwrap.dedent(
             """
             Your Alertmanager instance: client0 seems to be down!
-            It has not alerted COS-Alerter since 2023-01-01T00:00:00+00:00 UTC.
+            It has not alerted COS-Alerter ever.
             """
         ),
     )
 
     # Make sure if we try again, nothing is sent
     notify_mock.reset_mock()
```

### Comparing `cos-alerter-0.3.0/tests/test_daemon.py` & `cos-alerter-0.4.0/tests/test_daemon.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 DESTINATIONS = [
     "mailtos://user:pass@domain/?to=example-0@example.com,example-1@example.com",
     "slack://xoxb-1234-1234-4ddbc191d40ee098cbaae6f3523ada2d/#general",
 ]
 
 
 @pytest.fixture
-def fake_fs(fs):
-    fs.create_file("/etc/cos-alerter.yaml")
+def mock_fs(fake_fs):
     with open("/etc/cos-alerter.yaml", "w") as f:
         f.write(
             yaml.dump(
                 {
                     "watch": {
                         "down_interval": "4s",
                         "wait_for_first_connection": False,
@@ -38,21 +37,21 @@
                     },
                     "log_level": "info",
                 }
             )
         )
     config.set_path("/etc/cos-alerter.yaml")
     config.reload()
-    return fs
+    return fake_fs
 
 
 @pytest.mark.slow
 @unittest.mock.patch.object(apprise.Apprise, "add")
 @unittest.mock.patch.object(apprise.Apprise, "notify")
-def test_main(notify_mock, add_mock, fake_fs):
+def test_main(notify_mock, add_mock, mock_fs):
     main_thread = threading.Thread(target=main, kwargs={"run_for": 13, "argv": ["cos-alerter"]})
     try:
         main_thread.start()
         time.sleep(2)  # Should not be considered down yet.
         notify_mock.assert_not_called()
         subprocess.call(["curl", "-X", "POST", "http://localhost:8080/alive?clientid=client0"])
         time.sleep(3)  # Would be considered down but we just sent an alive call.
@@ -67,10 +66,10 @@
         main_thread.join()
 
 
 # TODO We need a test here for multiple clients. The problem is that the waitress thread does not
 # close when the previous test ends and so the socket is held open.
 
 
-def test_log_level_arg(fake_fs):
+def test_log_level_arg(mock_fs):
     main(run_for=0, argv=["cos-alerter", "--log-level", "DEBUG"])
     assert logging.getLogger("cos_alerter").getEffectiveLevel() == logging.DEBUG
```

### Comparing `cos-alerter-0.3.0/tests/test_server.py` & `cos-alerter-0.4.0/tests/test_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,37 @@
 # Copyright 2023 Canonical Ltd.
 # See LICENSE file for licensing details.
 
 import copy
 
 import pytest
 import yaml
+from helpers import CONFIG
 from werkzeug.datastructures import MultiDict
 
 from cos_alerter.alerter import AlerterState, config
 from cos_alerter.server import app
 
 PARAMS = {"clientid": "client0"}
-CONFIG = {
-    "watch": {
-        "down_interval": "5m",
-        "wait_for_first_connection": True,
-        "clients": ["client0"],
-    },
-    "notify": {
-        "destinations": [],
-        "repeat_interval": "1h",
-    },
-    "log_level": "info",
-}
 
 
 @pytest.fixture
 def flask_client():
     return app.test_client()
 
 
 @pytest.fixture
-def fake_fs(fs):
-    fs.create_file("/etc/cos-alerter.yaml")
-    with open("/etc/cos-alerter.yaml", "w") as f:
-        f.write(yaml.dump(CONFIG))
-    config.set_path("/etc/cos-alerter.yaml")
-    config.reload()
-    return fs
-
-
-@pytest.fixture
 def state_init():
     AlerterState.initialize()
 
 
+def test_dashboard_succeeds(flask_client, fake_fs, state_init):
+    assert flask_client.get("/").status_code == 200
+
+
 def test_alive_succeeds(flask_client, fake_fs, state_init):
     assert flask_client.post("/alive", query_string=PARAMS).status_code == 200
 
 
 def test_alive_other_methods_fail(flask_client, fake_fs, state_init):
     assert flask_client.get("/alive", query_string=PARAMS).status_code == 405
     assert flask_client.head("/alive", query_string=PARAMS).status_code == 405
```

