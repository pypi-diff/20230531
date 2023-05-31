# Comparing `tmp/pyalarmdotcomajax-0.5.0b6.tar.gz` & `tmp/pyalarmdotcomajax-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalarmdotcomajax-0.5.0b6.tar", last modified: Sun May 28 04:00:39 2023, max compression
+gzip compressed data, was "pyalarmdotcomajax-0.5.1.tar", last modified: Wed May 31 00:06:38 2023, max compression
```

## Comparing `pyalarmdotcomajax-0.5.0b6.tar` & `pyalarmdotcomajax-0.5.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:00:39.127723 pyalarmdotcomajax-0.5.0b6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18040 2023-05-28 04:00:39.131723 pyalarmdotcomajax-0.5.0b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:00:39.123723 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/
--rw-r--r--   0 runner    (1001) docker     (123)    46317 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20995 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:00:39.127723 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/garage_door.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/image_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14829 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/water_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22829 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:00:39.127723 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:00:39.127723 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/garage_door.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/water_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:00:39.127723 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18040 2023-05-28 04:00:39.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-28 04:00:39.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 04:00:39.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-28 04:00:39.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-28 04:00:39.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-28 04:00:39.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 04:00:38.000000 pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-28 04:00:39.131723 pyalarmdotcomajax-0.5.0b6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:00:39.127723 pyalarmdotcomajax-0.5.0b6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:00:39.127723 pyalarmdotcomajax-0.5.0b6/tests/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-28 04:00:27.000000 pyalarmdotcomajax-0.5.0b6/tests/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-28 04:00:28.000000 pyalarmdotcomajax-0.5.0b6/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-28 04:00:28.000000 pyalarmdotcomajax-0.5.0b6/tests/test_device_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-28 04:00:28.000000 pyalarmdotcomajax-0.5.0b6/tests/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-28 04:00:28.000000 pyalarmdotcomajax-0.5.0b6/tests/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-28 04:00:28.000000 pyalarmdotcomajax-0.5.0b6/tests/test_thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:38.627253 pyalarmdotcomajax-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-05-31 00:06:38.627253 pyalarmdotcomajax-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:38.623253 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/
+-rw-r--r--   0 runner    (1001) docker     (123)    46790 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20995 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:38.627253 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/garage_door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/image_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14829 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22829 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:38.627253 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:38.627253 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/garage_door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:38.623253 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-05-31 00:06:38.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-31 00:06:38.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:06:38.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 00:06:38.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-31 00:06:38.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 00:06:38.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 00:06:38.000000 pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-31 00:06:38.631253 pyalarmdotcomajax-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:38.627253 pyalarmdotcomajax-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 00:06:38.627253 pyalarmdotcomajax-0.5.1/tests/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/tests/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/tests/test_device_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/tests/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/tests/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-31 00:06:18.000000 pyalarmdotcomajax-0.5.1/tests/test_thermostat.py
```

### Comparing `pyalarmdotcomajax-0.5.0b6/LICENSE` & `pyalarmdotcomajax-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/PKG-INFO` & `pyalarmdotcomajax-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalarmdotcomajax
-Version: 0.5.0b6
+Version: 0.5.1
 Summary: Python Interface for Alarm.com
 Home-page: https://github.com/pyalarmdotcom/pyalarmdotcomajax
 Author: Justin Wong
 Author-email: 46082645+uvjustin@users.noreply.github.com
 Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b6 Summary: Python
+Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.1 Summary: Python
 Interface for Alarm.com Home-page: https://github.com/pyalarmdotcom/
 pyalarmdotcomajax Author: Justin Wong Author-email:
 46082645+uvjustin@users.noreply.github.com Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
 466460+elahd@users.noreply.github.com License: MIT Keywords: Alarm.com,Security
 System,Home Assistant Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English Classifier: Environment :: Web
```

### Comparing `pyalarmdotcomajax-0.5.0b6/README.md` & `pyalarmdotcomajax-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/__init__.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Alarmdotcom API Controller."""
 from __future__ import annotations
 
 import asyncio
+import contextlib
 import json
 import logging
 import re
 from collections.abc import Callable, Coroutine
 from contextlib import suppress
 from datetime import datetime, timedelta
 from typing import Any, TypedDict
@@ -41,15 +42,15 @@
     CameraSkybellControllerExtension,
     ConfigurationOption,
     ControllerExtensions_t,
     ExtendedProperties,
 )
 from pyalarmdotcomajax.websockets.client import WebSocketClient, WebSocketState
 
-__version__ = "0.5.0-beta.6"
+__version__ = "0.5.1"
 
 log = logging.getLogger(__name__)
 
 
 class ExtensionResults(TypedDict):
     """Results of multi-device extension calls."""
 
@@ -480,16 +481,20 @@
             ) as resp:
                 if re.search("m=login_fail", str(resp.url)) is not None:
                     log.exception("Login failed.")
                     log.exception("\nResponse URL:\n%s\n", str(resp.url))
                     log.exception("\nRequest Headers:\n%s\n", str(resp.request_info.headers))
                     raise AuthenticationFailed("Invalid username and password.")
 
-                # Update anti-forgery cookie
-                self._ajax_headers["ajaxrequestuniquekey"] = resp.cookies["afg"].value
+                # Update anti-forgery cookie.
+                # AFG cookie is not always present in the response. This seems to depend on the specific Alarm.com vendor, so a missing AFG key should not cause a failure.
+                # Ref: https://www.alarm.com/web/system/assets/addon-tree-output/@adc/ajax/services/adc-ajax.js
+
+                with contextlib.suppress(KeyError):
+                    self._ajax_headers["ajaxrequestuniquekey"] = resp.cookies["afg"].value
 
         except (aiohttp.ClientResponseError, KeyError) as err:
             log.exception("Failed to get AJAX key from Alarm.com.")
             raise UnexpectedResponse from err
 
         self._last_session_refresh = datetime.now()
 
@@ -577,15 +582,20 @@
             raise ConfigureTwoFactorAuthentication
 
         enabled_otp_types_bitmask = attribs.get("enabledTwoFactorTypes")
         enabled_2fa_methods = [
             otp_type for otp_type in OtpType if bool(enabled_otp_types_bitmask & otp_type.value)
         ]
 
-        if (OtpType.disabled in enabled_2fa_methods) or (attribs.get("isCurrentDeviceTrusted") is True):
+        if (
+            (OtpType.disabled in enabled_2fa_methods)
+            or (attribs.get("isCurrentDeviceTrusted") is True)
+            or not enabled_otp_types_bitmask
+            or not enabled_2fa_methods
+        ):
             # 2FA is disabled, we can skip 2FA altogether.
             return
 
         log.info(f"Requires two-factor authentication. Enabled methods are {enabled_2fa_methods}")
 
         raise OtpRequired(enabled_2fa_methods)
```

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/cli.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/cli.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/const.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/const.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/__init__.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/garage_door.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/garage_door.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/gate.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/gate.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/image_sensor.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/image_sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/light.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/light.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/lock.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/lock.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/partition.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/registry.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/registry.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/sensor.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/system.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/system.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/devices/thermostat.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/devices/thermostat.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/exceptions.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/extensions.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/extensions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/helpers.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/helpers.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/client.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/client.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/const.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/const.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/__init__.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/garage_door.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/garage_door.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/gate.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/gate.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/light.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/light.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/lock.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/lock.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/partition.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/sensor.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/thermostat.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/thermostat.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/handler/water_sensor.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/handler/water_sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax/websockets/messages.py` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax/websockets/messages.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/PKG-INFO` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalarmdotcomajax
-Version: 0.5.0b6
+Version: 0.5.1
 Summary: Python Interface for Alarm.com
 Home-page: https://github.com/pyalarmdotcom/pyalarmdotcomajax
 Author: Justin Wong
 Author-email: 46082645+uvjustin@users.noreply.github.com
 Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b6 Summary: Python
+Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.1 Summary: Python
 Interface for Alarm.com Home-page: https://github.com/pyalarmdotcom/
 pyalarmdotcomajax Author: Justin Wong Author-email:
 46082645+uvjustin@users.noreply.github.com Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
 466460+elahd@users.noreply.github.com License: MIT Keywords: Alarm.com,Security
 System,Home Assistant Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English Classifier: Environment :: Web
```

### Comparing `pyalarmdotcomajax-0.5.0b6/pyalarmdotcomajax.egg-info/SOURCES.txt` & `pyalarmdotcomajax-0.5.1/pyalarmdotcomajax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/pyproject.toml` & `pyalarmdotcomajax-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/setup.cfg` & `pyalarmdotcomajax-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/tests/__init__.py` & `pyalarmdotcomajax-0.5.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/tests/conftest.py` & `pyalarmdotcomajax-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/tests/test_controller.py` & `pyalarmdotcomajax-0.5.1/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/tests/test_device_extensions.py` & `pyalarmdotcomajax-0.5.1/tests/test_device_extensions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/tests/test_partition.py` & `pyalarmdotcomajax-0.5.1/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/tests/test_sensors.py` & `pyalarmdotcomajax-0.5.1/tests/test_sensors.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b6/tests/test_thermostat.py` & `pyalarmdotcomajax-0.5.1/tests/test_thermostat.py`

 * *Files identical despite different names*

