# Comparing `tmp/pytest-embedded-serial-1.2.5.tar.gz` & `tmp/pytest-embedded-serial-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-embedded-serial-1.2.5.tar", last modified: Tue Apr 11 05:40:50 2023, max compression
+gzip compressed data, was "dist/pytest-embedded-serial-1.3.0.tar", last modified: Wed May 31 13:09:02 2023, max compression
```

## Comparing `pytest-embedded-serial-1.2.5.tar` & `pytest-embedded-serial-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:50.000000 pytest-embedded-serial-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-11 05:40:50.000000 pytest-embedded-serial-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-11 05:40:39.000000 pytest-embedded-serial-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:50.000000 pytest-embedded-serial-1.2.5/pytest_embedded_serial/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 05:40:39.000000 pytest-embedded-serial-1.2.5/pytest_embedded_serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-11 05:40:39.000000 pytest-embedded-serial-1.2.5/pytest_embedded_serial/dut.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-11 05:40:39.000000 pytest-embedded-serial-1.2.5/pytest_embedded_serial/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 05:40:50.000000 pytest-embedded-serial-1.2.5/pytest_embedded_serial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-11 05:40:50.000000 pytest-embedded-serial-1.2.5/pytest_embedded_serial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-11 05:40:50.000000 pytest-embedded-serial-1.2.5/pytest_embedded_serial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 05:40:50.000000 pytest-embedded-serial-1.2.5/pytest_embedded_serial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 05:40:50.000000 pytest-embedded-serial-1.2.5/pytest_embedded_serial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 05:40:50.000000 pytest-embedded-serial-1.2.5/pytest_embedded_serial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 05:40:50.000000 pytest-embedded-serial-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-11 05:40:39.000000 pytest-embedded-serial-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-31 13:08:52.000000 pytest-embedded-serial-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-31 13:08:52.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-31 13:08:52.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial/dut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-31 13:08:52.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-31 13:08:52.000000 pytest-embedded-serial-1.3.0/setup.py
```

### Comparing `pytest-embedded-serial-1.2.5/PKG-INFO` & `pytest-embedded-serial-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pytest-embedded-serial
-Version: 1.2.5
+Version: 1.3.0
 Summary: pytest embedded plugin for testing serial ports
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded-serial
```

### Comparing `pytest-embedded-serial-1.2.5/pytest_embedded_serial/dut.py` & `pytest-embedded-serial-1.3.0/pytest_embedded_serial/dut.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-serial-1.2.5/pytest_embedded_serial/serial.py` & `pytest-embedded-serial-1.3.0/pytest_embedded_serial/serial.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-serial-1.2.5/pytest_embedded_serial.egg-info/PKG-INFO` & `pytest-embedded-serial-1.3.0/pytest_embedded_serial.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pytest-embedded-serial
-Version: 1.2.5
+Version: 1.3.0
 Summary: pytest embedded plugin for testing serial ports
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded-serial
```

### Comparing `pytest-embedded-serial-1.2.5/setup.py` & `pytest-embedded-serial-1.3.0/setup.py`

 * *Files identical despite different names*

