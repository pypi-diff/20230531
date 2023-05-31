# Comparing `tmp/hubitatcontrol-2.3.3.tar.gz` & `tmp/hubitatcontrol-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubitatcontrol-2.3.3.tar", max compression
+gzip compressed data, was "hubitatcontrol-3.0.0.tar", max compression
```

## Comparing `hubitatcontrol-2.3.3.tar` & `hubitatcontrol-3.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-03-12 19:21:22.061753 hubitatcontrol-2.3.3/LICENSE
--rw-r--r--   0        0        0     6311 2023-05-01 03:18:14.794797 hubitatcontrol-2.3.3/README.md
--rw-r--r--   0        0        0     3082 2023-05-11 03:27:49.032359 hubitatcontrol-2.3.3/hubitatcontrol/__init__.py
--rw-r--r--   0        0        0     3824 2023-05-01 03:18:14.794797 hubitatcontrol-2.3.3/hubitatcontrol/__main__.py
--rw-r--r--   0        0        0      172 2023-05-01 03:18:14.794797 hubitatcontrol-2.3.3/hubitatcontrol/environment.py
--rw-r--r--   0        0        0     1060 2023-04-23 03:06:31.104361 hubitatcontrol-2.3.3/hubitatcontrol/generic.py
--rw-r--r--   0        0        0     3073 2023-05-09 06:17:49.007286 hubitatcontrol-2.3.3/hubitatcontrol/hub.py
--rw-r--r--   0        0        0     2774 2023-04-23 03:06:31.104361 hubitatcontrol-2.3.3/hubitatcontrol/lights.py
--rw-r--r--   0        0        0      478 2023-05-09 03:28:26.350568 hubitatcontrol-2.3.3/hubitatcontrol/sensors.py
--rw-r--r--   0        0        0     2606 2023-05-11 03:45:25.239499 hubitatcontrol-2.3.3/pyproject.toml
--rw-r--r--   0        0        0     7193 1970-01-01 00:00:00.000000 hubitatcontrol-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-03-12 19:21:22.061753 hubitatcontrol-3.0.0/LICENSE
+-rw-r--r--   0        0        0     6482 2023-05-31 04:58:07.123388 hubitatcontrol-3.0.0/README.md
+-rw-r--r--   0        0        0     4381 2023-05-31 04:58:07.127388 hubitatcontrol-3.0.0/hubitatcontrol/__init__.py
+-rw-r--r--   0        0        0     3737 2023-05-31 04:58:07.127388 hubitatcontrol-3.0.0/hubitatcontrol/__main__.py
+-rw-r--r--   0        0        0      172 2023-05-01 03:18:14.794797 hubitatcontrol-3.0.0/hubitatcontrol/environment.py
+-rw-r--r--   0        0        0     1120 2023-05-31 04:58:07.127388 hubitatcontrol-3.0.0/hubitatcontrol/generic.py
+-rw-r--r--   0        0        0     3078 2023-05-31 04:58:07.127388 hubitatcontrol-3.0.0/hubitatcontrol/hub.py
+-rw-r--r--   0        0        0     2896 2023-05-31 04:58:07.127388 hubitatcontrol-3.0.0/hubitatcontrol/lights.py
+-rw-r--r--   0        0        0      587 2023-05-31 04:58:07.127388 hubitatcontrol-3.0.0/hubitatcontrol/sensors.py
+-rw-r--r--   0        0        0     2723 2023-05-31 05:03:46.551617 hubitatcontrol-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7364 1970-01-01 00:00:00.000000 hubitatcontrol-3.0.0/PKG-INFO
```

### Comparing `hubitatcontrol-2.3.3/LICENSE` & `hubitatcontrol-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-2.3.3/README.md` & `hubitatcontrol-3.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -38,39 +38,40 @@
 pip install git+https://github.com/Jelloeater/hubitatcontrol.git
 ```
 
 ## Usage
 
 ### API
 **Local Example**
+
 ```python
 import hubitatcontrol as hc
 
-hub = hc.get_hub(host='http://192.168.1.100', token='Maker_Token',
-                 app_id='Maker_App_ID')
-device = hc.lookup_device(hub, 'Device_Name')
+hub = hc.Hub(host='http://192.168.1.100', token='Maker_Token',
+app_id='Maker_App_ID') # Get Hub object to auth and poll against
 
-print(device.switch)
-device.turn_on()
-print(device.switch)
-```
+# If you have a cloud based maker API, you can include the cloud token
+# hub = hc.get_hub(host='https://cloud.hubitat.com', token='Maker_Token',
+#                  app_id='Maker_App_ID', cloud_token='Cloud_API_token')
 
-**Cloud Example**
-```python
-import hubitatcontrol as hc
+TEST_DEVICE = '1RGB'
 
-hub = hc.get_hub(host='https://cloud.hubitat.com', token='Maker_Token',
-                 app_id='Maker_App_ID', cloud_token='Cloud_API_token')
-device = hc.lookup_device(hub, 'Device_Name')
+device = hc.GetSingleDevice(hub).name(TEST_DEVICE)
 
+# Turn on all the switches (includes lights)
+device.turn_on() # Send command to device
 print(device.switch)
-device.turn_on()
-print(device.switch)
+
+# Get temprature from all sensors
+for i in hc.GetDevices(hub).TemperatureSensor():
+    print(f"{i.name} - {i.temperature}")
+
 ```
 
+
 ### CLI Interface
 - If you have all the needed API keys added to your .env file, all you need to do is add them to your keyring
 - Once loaded into the keyring, you can run the CLI from anywhere on your system
 
 ```bash
 hubitatcontrol --help
 hubitatcontrol load-env-to-keyring
@@ -106,14 +107,16 @@
 
 ## Docs
 
 [Located in /docs folder](docs)
 
 You will need a .dot file browser for the class diagrams
 
+**WIP: Setup ReadTheDocs auto gen**
+
 ## Issues / Features
 See:
 
 https://github.com/Jelloeater/hubitatcontrol/issues
 
 ## Structure
```

### Comparing `hubitatcontrol-2.3.3/hubitatcontrol/generic.py` & `hubitatcontrol-3.0.0/hubitatcontrol/generic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from hubitatcontrol.hub import Device
 
 
 class Switch(Device):
+    spec = ["Switch"]
+
     @property
     def switch(self) -> str:
         """Returns either (on or off)"""
         return [x for x in self.attributes if "switch" in x["name"]][0]["currentValue"]
 
     def turn_on(self):
         self.send_device_command(command="on")
 
     def turn_off(self):
         self.send_device_command(command="off")
 
 
 class ZigbeeOutlet(Switch):
+    spec = ["PowerMeter", "Outlet"]
+
     @property
     def power(self) -> int:
         """Returns power usage"""
         return [x for x in self.attributes if "power" in x["name"]][0]["currentValue"]
 
 
 class Thermostat(Device):
```

### Comparing `hubitatcontrol-2.3.3/hubitatcontrol/hub.py` & `hubitatcontrol-3.0.0/hubitatcontrol/hub.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 class Device:
     def __init__(self, hub: Hub, device_from_hub: dict):
         self.token = hub.token
         self.base_url_prefix = hub.base_url_prefix
         self.name = device_from_hub["name"]
         self.label = device_from_hub["label"]
         self.type = device_from_hub["type"]
-        self.id = device_from_hub["id"]
+        self.id = int(device_from_hub["id"])
 
     @property
     def commands(self):
         r = requests.get(
             url=self.base_url_prefix + "/" + str(self.id) + "/commands",
             params={"access_token": self.token},
             timeout=timeout,
```

### Comparing `hubitatcontrol-2.3.3/hubitatcontrol/lights.py` & `hubitatcontrol-3.0.0/hubitatcontrol/lights.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 import json
 from time import sleep
 
 from hubitatcontrol.generic import Switch
 
 
 class Dimmer(Switch):
+    spec = ["SwitchLevel"]
+
     @property
     def level(self) -> int:
         return [x for x in self.attributes if "level" in x["name"]][0]["currentValue"]
 
     def set_level(self, level: int):
         """0-100 valid range"""
         if level < 0 or level > 100:
             raise Exception("Invalid range")
         self.send_device_command(command="setLevel", secondary_command=str(level))
         sleep(2.5)
 
 
 class Bulb(Dimmer):
-    pass
+    spec = ["ChangeLevel"]
+
     # TODO May need to add more methods, as bulbs might have more functionality
 
 
 class ColorTempBulb(Bulb):
+    spec = ["ColorTemperature"]
+
     @property
     def color_temp(self) -> int:
         return [x for x in self.attributes if "colorTemperature" in x["name"]][0]["currentValue"]
 
     def set_color_temp(self, level: int):
         """Degrees Kelvin"""
         self.send_device_command(command="setColorTemperature", secondary_command=str(level))
         sleep(2)
 
 
 class RGBWBulb(ColorTempBulb):
+    spec = ["ColorControl", "ColorMode"]
+
     @property
     def color(self) -> str:
         return [x for x in self.attributes if "color" in x["name"]][0]["currentValue"]
 
     @property
     def hue(self) -> int:
         return [x for x in self.attributes if "hue" in x["name"]][0]["currentValue"]
```

### Comparing `hubitatcontrol-2.3.3/pyproject.toml` & `hubitatcontrol-3.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hubitatcontrol"
-version = "v2.3.3"
+version = "v3.0.0"
 description = "Hubitat Maker API Interface"
 authors = ["Jesse Schoepfer <jelloeater@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/Jelloeater/hubitatcontrol"
 keywords = ["hubitat", "makerapi","requests"]
 classifiers = ["Development Status :: 5 - Production/Stable",
@@ -29,14 +29,20 @@
 pythonpath = ["."]
 testpaths = "test/"
 log_cli = true
 log_cli_level = "DEBUG"
 log_cli_format = "[%(asctime)s] [%(levelname)8s] --- %(message)s (%(filename)s:%(funcName)s():%(lineno)s)"
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
 
+[tool.coverage.run]
+omit = [
+    "tests/*",
+    ]
+
+
 [tool.black]
 line-length = 120
 skip-string-normalization = true
 
 [tool.flake8]
 exclude =['./tests']
 max-line-length = 120
@@ -74,14 +80,16 @@
  {path-pattern = 'docs/source/(.*)\.rst'},
 ]
 exclude-entropy-patterns = [
     {path-pattern = '\.github/workflows/.*\.yml', pattern = 'uses: .*@[a-zA-Z0-9]{40}', reason = 'GitHub Actions'},
     {path-pattern = 'poetry\.lock', pattern = '.'},
     {path-pattern = 'Pipfile\.lock', pattern = '.'},
     {path-pattern = 'README\.md', pattern = '.'},
+    {path-pattern = 'index\.rst', pattern = '.'},
+
 ]
 
 [tool.poetry.group.test.dependencies]
 setuptools = "*"
 pytest = "*"
 pytest-cov = "*"
 python-dotenv = "*"
@@ -102,11 +110,12 @@
 bandit = "*"
 whispers = "*"
 mdformat-gfm ="*"
 mdformat-frontmatter ="*"
 flake8 = "*"
 Flake8-pyproject="*"
 tartufo="*"
+mdToRst = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hubitatcontrol-2.3.3/PKG-INFO` & `hubitatcontrol-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubitatcontrol
-Version: 2.3.3
+Version: 3.0.0
 Summary: Hubitat Maker API Interface
 Home-page: https://github.com/Jelloeater/hubitatcontrol
 License: MIT
 Keywords: hubitat,makerapi,requests
 Author: Jesse Schoepfer
 Author-email: jelloeater@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -63,39 +63,40 @@
 pip install git+https://github.com/Jelloeater/hubitatcontrol.git
 ```
 
 ## Usage
 
 ### API
 **Local Example**
+
 ```python
 import hubitatcontrol as hc
 
-hub = hc.get_hub(host='http://192.168.1.100', token='Maker_Token',
-                 app_id='Maker_App_ID')
-device = hc.lookup_device(hub, 'Device_Name')
+hub = hc.Hub(host='http://192.168.1.100', token='Maker_Token',
+app_id='Maker_App_ID') # Get Hub object to auth and poll against
 
-print(device.switch)
-device.turn_on()
-print(device.switch)
-```
+# If you have a cloud based maker API, you can include the cloud token
+# hub = hc.get_hub(host='https://cloud.hubitat.com', token='Maker_Token',
+#                  app_id='Maker_App_ID', cloud_token='Cloud_API_token')
 
-**Cloud Example**
-```python
-import hubitatcontrol as hc
+TEST_DEVICE = '1RGB'
 
-hub = hc.get_hub(host='https://cloud.hubitat.com', token='Maker_Token',
-                 app_id='Maker_App_ID', cloud_token='Cloud_API_token')
-device = hc.lookup_device(hub, 'Device_Name')
+device = hc.GetSingleDevice(hub).name(TEST_DEVICE)
 
+# Turn on all the switches (includes lights)
+device.turn_on() # Send command to device
 print(device.switch)
-device.turn_on()
-print(device.switch)
+
+# Get temprature from all sensors
+for i in hc.GetDevices(hub).TemperatureSensor():
+    print(f"{i.name} - {i.temperature}")
+
 ```
 
+
 ### CLI Interface
 - If you have all the needed API keys added to your .env file, all you need to do is add them to your keyring
 - Once loaded into the keyring, you can run the CLI from anywhere on your system
 
 ```bash
 hubitatcontrol --help
 hubitatcontrol load-env-to-keyring
@@ -131,14 +132,16 @@
 
 ## Docs
 
 [Located in /docs folder](docs)
 
 You will need a .dot file browser for the class diagrams
 
+**WIP: Setup ReadTheDocs auto gen**
+
 ## Issues / Features
 See:
 
 https://github.com/Jelloeater/hubitatcontrol/issues
 
 ## Structure
```

