# Comparing `tmp/firmetix-7.0.2.tar.gz` & `tmp/firmetix-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/firmetix/firmetix/dist/.tmp-8khmkhko/firmetix-7.0.2.tar", last modified: Tue May 16 16:24:00 2023, max compression
+gzip compressed data, was "/home/runner/work/firmetix/firmetix/dist/.tmp-y_lwo70v/firmetix-7.1.0.tar", last modified: Wed May 31 00:51:59 2023, max compression
```

## Comparing `firmetix-7.0.2.tar` & `firmetix-7.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:24:00.000000 firmetix-7.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 16:23:48.000000 firmetix-7.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-16 16:24:00.000000 firmetix-7.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-16 16:23:48.000000 firmetix-7.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:24:00.000000 firmetix-7.0.2/firmetix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:23:48.000000 firmetix-7.0.2/firmetix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   103004 2023-05-16 16:23:48.000000 firmetix-7.0.2/firmetix/firmetix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-16 16:23:48.000000 firmetix-7.0.2/firmetix/private_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:24:00.000000 firmetix-7.0.2/firmetix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-16 16:24:00.000000 firmetix-7.0.2/firmetix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-16 16:24:00.000000 firmetix-7.0.2/firmetix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 16:24:00.000000 firmetix-7.0.2/firmetix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 16:24:00.000000 firmetix-7.0.2/firmetix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 16:24:00.000000 firmetix-7.0.2/firmetix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-16 16:23:48.000000 firmetix-7.0.2/pypi_desc.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 16:24:00.000000 firmetix-7.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-16 16:23:48.000000 firmetix-7.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:51:59.000000 firmetix-7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-31 00:51:46.000000 firmetix-7.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-31 00:51:59.000000 firmetix-7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-31 00:51:46.000000 firmetix-7.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:51:59.000000 firmetix-7.1.0/firmetix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 00:51:46.000000 firmetix-7.1.0/firmetix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104627 2023-05-31 00:51:46.000000 firmetix-7.1.0/firmetix/firmetix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-31 00:51:46.000000 firmetix-7.1.0/firmetix/private_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:51:59.000000 firmetix-7.1.0/firmetix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-31 00:51:59.000000 firmetix-7.1.0/firmetix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-31 00:51:59.000000 firmetix-7.1.0/firmetix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:51:59.000000 firmetix-7.1.0/firmetix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-31 00:51:59.000000 firmetix-7.1.0/firmetix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 00:51:59.000000 firmetix-7.1.0/firmetix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-31 00:51:46.000000 firmetix-7.1.0/pypi_desc.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 00:51:59.000000 firmetix-7.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-31 00:51:46.000000 firmetix-7.1.0/setup.py
```

### Comparing `firmetix-7.0.2/PKG-INFO` & `firmetix-7.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firmetix
-Version: 7.0.2
+Version: 7.1.0
 Summary: Remotely Control And Monitor Arduino and Esp devices
 Home-page: https://github.com/Nilon123456789/firmetix
 Download-URL: https://github.com/Nilon123456789/firmetix
 Author: Nils Lahaye
 Author-email: nils.lahaye@icloud.com
 Keywords: firmetix,Arduino,Protocol,Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `firmetix-7.0.2/README.md` & `firmetix-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `firmetix-7.0.2/firmetix/firmetix.py` & `firmetix-7.1.0/firmetix/firmetix.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     It includes the public API methods as well as
     a set of private methods.
 
     """
 
     # noinspection PyPep8,PyPep8,PyPep8
     def __init__(self, com_port=None, arduino_instance_id=1, connection_type=0,
-                 arduino_wait=4, sleep_tune=0.000001,
+                 arduino_wait=1, sleep_tune=0.000001,
                  shutdown_on_exception=True,
                  ip_address=None, ip_port=31335, baudrate=115200,
                  send_delay=0.01, ble_mac_address=None, ble_name=None):
 
         """
 
         :param com_port: e.g. COM3 or /dev/ttyACM0.
@@ -350,36 +350,41 @@
 
             # no com_port found - raise a runtime exception
             else:
                 if self.shutdown_on_exception:
                     self.shutdown()
                 raise RuntimeError('No Arduino Found or User Aborted Program')
         elif self.connection_type == Connection_type.TCP_IP:
+            if(self.ip_address is None):
+                print("No IP address specified, starting wifi auto discovery for Firmetix4ESP devices...")
+                try:
+                    self.ip_address = socket.gethostbyname(PrivateConstants.DEFAULT_WIFI_NAME + str(arduino_instance_id) + ".local")
+                except socket.gaierror:
+                    print("No Firmetix4ESP devices found on the network, please specify the IP address manually.")
+                    self.shutdown()
+                else:
+                    print(f'\tFound Firmetix4ESP device at {self.ip_address}')
             self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.sock.connect((self.ip_address, self.ip_port))
 
             print(f'Successfully connected to: {self.ip_address}:{self.ip_port}')
         elif self.connection_type == Connection_type.BLE:
             
             if self.ble_name is None: # if no name is given, use the default
-                self.ble_name = "Firmetix4ESP_BLE_" + str(arduino_instance_id)
+                self.ble_name = PrivateConstants.DEFAULT_BLE_NAME + str(arduino_instance_id)
                 
             adapters = simplepyble.Adapter.get_adapters()
 
             if len(adapters) == 0:
                 raise RuntimeError('No Bluetooth adapters found')
             
             print(f'Found {len(adapters)} Bluetooth adapters')
             self.adapter = adapters[0] # use the first adapter
             print(f'\tUsing adapter 0: {self.adapter.identifier()}')
 
-            
-            if self.ble_name is None: # if no name is given, use the default
-                self.ble_name = "Firmetix4ESP_BLE_" + str(arduino_instance_id)
-
             # if the user did not specify a mac address
             if self.ble_mac_address == None:
                 self._find_arduino_ble()
             else:
                 self._manual_open_ble()
             
             if self.ble_device == None:
@@ -407,31 +412,30 @@
             self.ble_device.notify(PrivateConstants.SERVICE_UUID, PrivateConstants.CHARACTERISTIC_UUID_RX, self._ble_receiver)
             
         else:
             raise RuntimeError('Invalid connection type specified')
 
         # allow the threads to run
         self._run_threads()
-        print(f'Waiting for Arduino to reset')
-        print(f'Reset Complete')
+        print(f'\nWaiting for Arduino to reset')
+        print(f'\tReset Complete')
 
         # get firmetix firmware version and print it
         print('\nRetrieving Firmetix4Arduino firmware ID...')
         self._get_firmware_version()
         if not self.firmware_version:
             if self.shutdown_on_exception:
                 self.shutdown()
             raise RuntimeError(f'Firmetix4Arduino firmware version not found')
 
         else:
-            if self.firmware_version[0] < PrivateConstants.FIRMETIX4ARDUINO_MAJOR_VERSION:
+            if self.firmware_version[0] < PrivateConstants.FIRMETIX4ARDUINO_MAJOR_VERSION or  self.firmware_version[1] < PrivateConstants.FIRMETIX4ARDUINO_MINOR_VERSION:
                 raise RuntimeError('Please upgrade the server firmware to version ' + str(
-                    PrivateConstants.FIRMETIX4ARDUINO_MAJOR_VERSION) + ' or greater')
-            print(f'FirmetixArduino firmware version: {self.firmware_version[0]}.'
-                  f'{self.firmware_version[1]}.{self.firmware_version[2]}')
+                    PrivateConstants.FIRMETIX4ARDUINO_MAJOR_VERSION) + '.' +  str(PrivateConstants.FIRMETIX4ARDUINO_MINOR_VERSION) + ' or greater (current is version: ' + str(self.firmware_version[0]) + '.' + str(self.firmware_version[1]) + ')''')
+            print(f'FirmetixArduino firmware version: {self.firmware_version[0]}.'f'{self.firmware_version[1]}.{self.firmware_version[2]}')
         command = [PrivateConstants.ENABLE_ALL_REPORTS]
         self._add_command(command, False)
 
         # get the features list
         command = [PrivateConstants.GET_FEATURES]
         self._add_command(command, False)
         time.sleep(.2)
@@ -2013,24 +2017,39 @@
 
                 except (RuntimeError, SerialException, OSError):
                     # ignore error on shutdown
                     pass
             elif self.connection_type == Connection_type.TCP_IP:
                 if not self.sock:
                     raise Exception('')
-                
+
                 self.sock.shutdown(socket.SHUT_RDWR)
                 self.sock.close()
             elif self.connection_type == Connection_type.BLE:
                 if not self.ble_device:
                     raise Exception('')
                 
                 self.ble_device.disconnect()
         except Exception:
             raise RuntimeError('Shutdown failed - could not send stop streaming message')
+        
+    def sonar_disable(self):
+        """
+        Disable sonar scanning for all sonar sensors
+        """
+        command = [PrivateConstants.SONAR_DISABLE]
+        self._add_command(command)
+
+    def sonar_enable(self):
+        """
+        Enable sonar scanning for all sonar sensors
+        """
+        command = [PrivateConstants.SONAR_ENABLE]
+        self._add_command(command)
+
 
     def spi_cs_control(self, chip_select_pin, select):
         """
         Control an SPI chip select line
         :param chip_select_pin: pin connected to CS
 
         :param select: 0=select, 1=deselect
@@ -2389,15 +2408,18 @@
         pin = data[0]
         value = (data[1] << 8) + data[2]
         # set the current value in the pin structure
         time_stamp = time.time()
         # self.digital_pins[pin].event_time = time_stamp
         if self.analog_callbacks[pin]:
             message = [PrivateConstants.ANALOG_REPORT, pin, value, time_stamp]
-            self.analog_callbacks[pin](message)
+            try:
+                self.analog_callbacks[pin](message)
+            except KeyError:
+                print(f'Warning: No callback for pin {pin} in analog_callbacks (the error is harmless)')
 
     def _dht_report(self, data):
         """
         This is the dht report handler method.
 
         :param data:            data[0] = report error return
                                     No Errors = 0
@@ -2429,27 +2451,32 @@
         if data[0]:  # DHT_ERROR
             # error report
             # data[0] = report sub type, data[1] = pin, data[2] = error message
             if self.dht_callbacks[data[1]]:
                 # Callback 0=DHT REPORT, DHT_ERROR, PIN, Time
                 message = [PrivateConstants.DHT_REPORT, data[0], data[1], data[2],
                            time.time()]
-                self.dht_callbacks[data[1]](message)
+                try:
+                    self.dht_callbacks[data[1]](message)
+                except KeyError:
+                 print(f'Warning: Error in dht_callbacks (the error is harmless)')
         else:
             # got valid data DHT_DATA
             f_humidity = float(data[5] + data[6] / 100)
             if data[3]:
                 f_humidity *= -1.0
             f_temperature = float(data[7] + data[8] / 100)
             if data[4]:
                 f_temperature *= -1.0
             message = [PrivateConstants.DHT_REPORT, data[0], data[1], data[2],
                        f_humidity, f_temperature, time.time()]
-
-            self.dht_callbacks[data[1]](message)
+            try:
+                self.dht_callbacks[data[1]](message)
+            except KeyError:
+                print(f'Warning: Error in dht_callbacks (the error is harmless)')
 
     def _digital_message(self, data):
         """
         This is a private message handler method.
         It is a message handler for Digital Messages.
 
         :param data: digital message
@@ -2457,15 +2484,18 @@
         """
         pin = data[0]
         value = data[1]
 
         time_stamp = time.time()
         if self.digital_callbacks[pin]:
             message = [PrivateConstants.DIGITAL_REPORT, pin, value, time_stamp]
-            self.digital_callbacks[pin](message)
+            try:
+                self.digital_callbacks[pin](message)
+            except KeyError:
+                print(f'Warning: No callback for pin {pin} in digital_callbacks (the error is harmless)')
 
     def _firmware_message(self, data):
         """
         Firmetix4Arduino firmware version message
 
         :param data: data[0] = major number, data[1] = minor number.
```

### Comparing `firmetix-7.0.2/firmetix/private_constants.py` & `firmetix-7.1.0/firmetix/private_constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,17 +78,19 @@
     STEPPER_SET_3_PINS_INVERTED = 48
     STEPPER_SET_4_PINS_INVERTED = 49
     STEPPER_IS_RUNNING = 50
     STEPPER_GET_CURRENT_POSITION = 51
     STEPPER_GET_DISTANCE_TO_GO = 52
     STEPPER_GET_TARGET_POSITION = 53
     GET_FEATURES = 54
-    TONE = 55
-    NO_TONE = 56
-    GET_MAX_PINS = 57
+    SONAR_DISABLE = 55
+    SONAR_ENABLE = 56
+    TONE = 70
+    NO_TONE = 71
+    GET_MAX_PINS = 72
 
     # reports
     # debug data from Arduino
     DIGITAL_REPORT = DIGITAL_WRITE
     ANALOG_REPORT = ANALOG_WRITE
     FIRMWARE_REPORT = GET_FIRMWARE_VERSION
     I_AM_HERE_REPORT = ARE_U_THERE
@@ -106,16 +108,17 @@
     STEPPER_RUNNING_REPORT = 18
     STEPPER_RUN_COMPLETE_REPORT = 19
     FEATURES = 20
     NOT_IMPLEMENTED = 21
     DEBUG_PRINT = 99
     MAX_PIN_REPORT = GET_MAX_PINS
 
-    FIRMETIX_VERSION = "7.0.2"
+    FIRMETIX_VERSION = "7.1.0"
     FIRMETIX4ARDUINO_MAJOR_VERSION = 7
+    FIRMETIX4ARDUINO_MINOR_VERSION = 1
 
     # reporting control
     REPORTING_DISABLE_ALL = 0
     REPORTING_ANALOG_ENABLE = 1
     REPORTING_DIGITAL_ENABLE = 2
     REPORTING_ANALOG_DISABLE = 3
     REPORTING_DIGITAL_DISABLE = 4
@@ -145,11 +148,15 @@
     ONEWIRE_FEATURE = 0x01
     DHT_FEATURE = 0x02
     STEPPERS_FEATURE = 0x04
     SPI_FEATURE = 0x08
     SERVO_FEATURE = 0x10
     SONAR_FEATURE = 0x20
 
+    # default names
+    DEFAULT_WIFI_NAME = "Firmetix4ESP-WIFI-"
+    DEFAULT_BLE_NAME =  "Firmetix4ESP_BLE_"
+
     # BLE UID
     SERVICE_UUID = "6e400001-b5a3-f393-e0a9-e50e24dcca9e" # UART service UUID
     CHARACTERISTIC_UUID_TX = "6e400002-b5a3-f393-e0a9-e50e24dcca9e" # RX characteristic UUID
     CHARACTERISTIC_UUID_RX = "6e400003-b5a3-f393-e0a9-e50e24dcca9e" # TX characteristic UUID
```

### Comparing `firmetix-7.0.2/firmetix.egg-info/PKG-INFO` & `firmetix-7.1.0/firmetix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firmetix
-Version: 7.0.2
+Version: 7.1.0
 Summary: Remotely Control And Monitor Arduino and Esp devices
 Home-page: https://github.com/Nilon123456789/firmetix
 Download-URL: https://github.com/Nilon123456789/firmetix
 Author: Nils Lahaye
 Author-email: nils.lahaye@icloud.com
 Keywords: firmetix,Arduino,Protocol,Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `firmetix-7.0.2/pypi_desc.md` & `firmetix-7.1.0/pypi_desc.md`

 * *Files identical despite different names*

### Comparing `firmetix-7.0.2/setup.py` & `firmetix-7.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 setup(
     name='firmetix',
     packages=['firmetix'],
     install_requires=['pyserial', 'simplepyble'],
 
-    version='7.0.2',
+    version='7.1.0',
     description="Remotely Control And Monitor Arduino and Esp devices",
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     author='Nils Lahaye',
     author_email='nils.lahaye@icloud.com',
     url='https://github.com/Nilon123456789/firmetix',
@@ -28,8 +28,8 @@
         'Intended Audience :: Education',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
-)
+)
```

