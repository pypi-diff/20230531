# Comparing `tmp/naludaq-0.17.6.tar.gz` & `tmp/naludaq-0.17.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naludaq-0.17.6.tar", last modified: Tue May 23 23:00:05 2023, max compression
+gzip compressed data, was "naludaq-0.17.7.tar", last modified: Wed May 31 20:11:48 2023, max compression
```

## Comparing `naludaq-0.17.6.tar` & `naludaq-0.17.7.tar`

### file list

```diff
@@ -1,247 +1,247 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.447553 naludaq-0.17.6/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-23 22:59:48.000000 naludaq-0.17.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-05-23 23:00:05.447553 naludaq-0.17.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-05-23 22:59:48.000000 naludaq-0.17.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-23 22:59:48.000000 naludaq-0.17.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 23:00:05.447553 naludaq-0.17.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-23 22:59:48.000000 naludaq-0.17.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.415552 naludaq-0.17.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.419552 naludaq-0.17.6/src/naludaq/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.423552 naludaq-0.17.6/src/naludaq/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/backend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/backend/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/backend/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.423552 naludaq-0.17.6/src/naludaq/backend/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/backend/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/backend/managers/acquisitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/backend/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/backend/managers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/backend/managers/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/backend/managers/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.423552 naludaq-0.17.6/src/naludaq/backend/models/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/backend/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30392 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/backend/models/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/backend/models/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.423552 naludaq-0.17.6/src/naludaq/board/
--rw-r--r--   0 runner    (1001) docker     (123)    28790 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23941 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/board_inits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.423552 naludaq-0.17.6/src/naludaq/board/connections/
--rw-r--r--   0 runner    (1001) docker     (123)    18932 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/connections/_FTDI.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/connections/_MockUART.py
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/connections/_UART.py
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/connections/_USB.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/connections/base_ethernet.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/connections/base_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/connections/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/connections/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/connections/udp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.427552 naludaq-0.17.6/src/naludaq/board/initializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/initializers/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/initializers/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/initializers/init_aodsv2_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/initializers/init_hdsocv1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/initializers/init_udc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/initializers/init_upac96.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/initializers/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/board/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.427552 naludaq-0.17.6/src/naludaq/communication/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/communication/analog_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/communication/control_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/communication/digital_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/communication/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/communication/i2c_registers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28991 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/communication/registers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.427552 naludaq-0.17.6/src/naludaq/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/analog_debug_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.427552 naludaq-0.17.6/src/naludaq/controllers/biasing_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/biasing_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/biasing_mode/udc16.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.427552 naludaq-0.17.6/src/naludaq/controllers/board/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/board/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15185 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/board/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/board/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/board/oleas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/board/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/board/udc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/board/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/board/upac96.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.431553 naludaq-0.17.6/src/naludaq/controllers/connection/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21101 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/connection/connection_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/connection/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/connection/upac96.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.431553 naludaq-0.17.6/src/naludaq/controllers/external_dac/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/external_dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/external_dac/ad5671.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/external_dac/ad5675.py
--rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/external_dac/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/external_dac/dac7578.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/external_dac/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/external_dac/i2c_dac.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/external_dac/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/external_dac/upac32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.431553 naludaq-0.17.6/src/naludaq/controllers/gainstages/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/gainstages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/gainstages/aodsv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/gainstages/oddsock_aods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.431553 naludaq-0.17.6/src/naludaq/controllers/peripherals/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/peripherals/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/peripherals/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/peripherals/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/peripherals/peripherals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/peripherals/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/peripherals/upac96.py
--rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/project_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.431553 naludaq-0.17.6/src/naludaq/controllers/readout/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/readout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/readout/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/readout/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/readout/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/readout/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/si5341_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.431553 naludaq-0.17.6/src/naludaq/controllers/tia/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/tia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/tia/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/tia/hdsoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.435553 naludaq-0.17.6/src/naludaq/controllers/trigger/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/trigger/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/trigger/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/trigger/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/trigger/siread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/trigger/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/trigger/upac.py
--rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/controllers/trigger/upac96.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.435553 naludaq-0.17.6/src/naludaq/daq/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/daq/debugdaq.py
--rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/daq/lightdaq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/daq/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.435553 naludaq-0.17.6/src/naludaq/daq/workers/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/daq/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/daq/workers/answer_parser_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/daq/workers/csv_storage_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.435553 naludaq-0.17.6/src/naludaq/daq/workers/packager/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/daq/workers/packager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/daq/workers/packager/worker_packager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/daq/workers/packager/worker_packager_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/daq/workers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/daq/workers/worker_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/daq/workers/worker_serial_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/daq/workers/worker_usb_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.435553 naludaq-0.17.6/src/naludaq/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/devices/eeprom.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/devices/i2c_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/devices/ltc2990.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.435553 naludaq-0.17.6/src/naludaq/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/helpers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/helpers/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/helpers/register_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/helpers/semiton.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/helpers/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.439553 naludaq-0.17.6/src/naludaq/io/
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22338 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/io/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    35939 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/io/io_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.439553 naludaq-0.17.6/src/naludaq/models/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/models/acq_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/models/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)    15839 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/naludaq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.439553 naludaq-0.17.6/src/naludaq/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/parsers/aardvarcv3_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/parsers/answer_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/parsers/aodsoc_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/parsers/asocv3_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/parsers/hdsoc_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.439553 naludaq-0.17.6/src/naludaq/parsers/headers/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/parsers/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/parsers/headers/asoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/parsers/headers/asocv2.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/parsers/headers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/parsers/headers/siread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/parsers/headers/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/parsers/headers/upac32.py
--rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/parsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/parsers/trbhm_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/parsers/udc_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/parsers/upac96_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/parsers/upac_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.443553 naludaq-0.17.6/src/naludaq/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.443553 naludaq-0.17.6/src/naludaq/tools/adc2mv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/adc2mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/adc2mv/adc_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/adc2mv/adc_linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/adc2mv/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/adc2mv/pre_adc2mv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/autoaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.443553 naludaq-0.17.6/src/naludaq/tools/autotrigger/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/autotrigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/autotrigger/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/board_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.443553 naludaq-0.17.6/src/naludaq/tools/dac_sweep/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/dac_sweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/dac_sweep/dac_sweep_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/ft60x.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/ftdi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.443553 naludaq-0.17.6/src/naludaq/tools/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/optimizers/bayesian_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/optimizers/gainstagetuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.443553 naludaq-0.17.6/src/naludaq/tools/pedestals/
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/pedestals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.443553 naludaq-0.17.6/src/naludaq/tools/pedestals/_new/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/pedestals/_new/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/pedestals/_new/aav3.py
--rw-r--r--   0 runner    (1001) docker     (123)    25345 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/pedestals/_new/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/pedestals/_new/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/pedestals/pedestals_acq.py
--rw-r--r--   0 runner    (1001) docker     (123)    34274 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/pedestals/pedestals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/pedestals/pedestals_correcter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/pedestals/pedestals_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/pedestals/udc16_pedestals_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/pedestals/upac32_pedestals_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/pedestals/upac96_pedestals_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.447553 naludaq-0.17.6/src/naludaq/tools/threshold_scan/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/threshold_scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/threshold_scan/threshold_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.447553 naludaq-0.17.6/src/naludaq/tools/timing_cal/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/timing_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/timing_cal/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/timing_cal/correcter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.447553 naludaq-0.17.6/src/naludaq/tools/waiter/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/waiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-23 22:59:48.000000 naludaq-0.17.6/src/naludaq/tools/waiter/eventwaiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.423552 naludaq-0.17.6/src/naludaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-05-23 23:00:05.000000 naludaq-0.17.6/src/naludaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-05-23 23:00:05.000000 naludaq-0.17.6/src/naludaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:00:05.000000 naludaq-0.17.6/src/naludaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-23 23:00:05.000000 naludaq-0.17.6/src/naludaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 23:00:05.000000 naludaq-0.17.6/src/naludaq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:00:05.447553 naludaq-0.17.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-23 22:59:48.000000 naludaq-0.17.6/tests/test_naludaq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.674107 naludaq-0.17.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-31 20:11:29.000000 naludaq-0.17.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-05-31 20:11:48.674107 naludaq-0.17.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-05-31 20:11:29.000000 naludaq-0.17.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-31 20:11:29.000000 naludaq-0.17.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 20:11:48.674107 naludaq-0.17.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-31 20:11:29.000000 naludaq-0.17.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.638105 naludaq-0.17.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.646105 naludaq-0.17.7/src/naludaq/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.646105 naludaq-0.17.7/src/naludaq/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.646105 naludaq-0.17.7/src/naludaq/backend/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/managers/acquisitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/managers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/managers/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/managers/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.646105 naludaq-0.17.7/src/naludaq/backend/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35624 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/models/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/backend/models/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.646105 naludaq-0.17.7/src/naludaq/board/
+-rw-r--r--   0 runner    (1001) docker     (123)    28790 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23941 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/board_inits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.650106 naludaq-0.17.7/src/naludaq/board/connections/
+-rw-r--r--   0 runner    (1001) docker     (123)    18932 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/_FTDI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/_MockUART.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/_UART.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/_USB.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/base_ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/base_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/connections/udp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.650106 naludaq-0.17.7/src/naludaq/board/initializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/initializers/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/initializers/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/initializers/init_aodsv2_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/initializers/init_hdsocv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/initializers/init_udc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/initializers/init_upac96.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/initializers/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/board/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.650106 naludaq-0.17.7/src/naludaq/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/communication/analog_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/communication/control_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/communication/digital_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/communication/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/communication/i2c_registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28991 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/communication/registers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.650106 naludaq-0.17.7/src/naludaq/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/analog_debug_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.650106 naludaq-0.17.7/src/naludaq/controllers/biasing_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/biasing_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/biasing_mode/udc16.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.654106 naludaq-0.17.7/src/naludaq/controllers/board/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/board/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15185 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/board/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/board/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/board/oleas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/board/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/board/udc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/board/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/board/upac96.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.654106 naludaq-0.17.7/src/naludaq/controllers/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21101 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/connection/connection_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/connection/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/connection/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.654106 naludaq-0.17.7/src/naludaq/controllers/external_dac/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/external_dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/external_dac/ad5671.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/external_dac/ad5675.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/external_dac/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/external_dac/dac7578.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/external_dac/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/external_dac/i2c_dac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/external_dac/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/external_dac/upac32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.654106 naludaq-0.17.7/src/naludaq/controllers/gainstages/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/gainstages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/gainstages/aodsv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/gainstages/oddsock_aods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.658106 naludaq-0.17.7/src/naludaq/controllers/peripherals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/peripherals/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/peripherals/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/peripherals/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/peripherals/peripherals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/peripherals/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/peripherals/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/project_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.658106 naludaq-0.17.7/src/naludaq/controllers/readout/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/readout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/readout/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/readout/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/readout/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/readout/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/si5341_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.658106 naludaq-0.17.7/src/naludaq/controllers/tia/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/tia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/tia/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/tia/hdsoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.658106 naludaq-0.17.7/src/naludaq/controllers/trigger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/trigger/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/trigger/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/trigger/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/trigger/siread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/trigger/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/trigger/upac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/controllers/trigger/upac96.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.658106 naludaq-0.17.7/src/naludaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/debugdaq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/lightdaq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.662107 naludaq-0.17.7/src/naludaq/daq/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/answer_parser_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/csv_storage_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.662107 naludaq-0.17.7/src/naludaq/daq/workers/packager/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/packager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/packager/worker_packager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/packager/worker_packager_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/worker_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/worker_serial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/daq/workers/worker_usb_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.662107 naludaq-0.17.7/src/naludaq/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/devices/eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/devices/i2c_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/devices/ltc2990.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.662107 naludaq-0.17.7/src/naludaq/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/helpers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/helpers/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/helpers/register_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/helpers/semiton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/helpers/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.662107 naludaq-0.17.7/src/naludaq/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22338 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/io/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35939 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/io/io_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.662107 naludaq-0.17.7/src/naludaq/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/models/acq_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/models/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15839 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/naludaq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.666107 naludaq-0.17.7/src/naludaq/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/aardvarcv3_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/answer_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/aodsoc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/asocv3_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/hdsoc_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.666107 naludaq-0.17.7/src/naludaq/parsers/headers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/headers/asoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/headers/asocv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/headers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/headers/siread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/headers/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/headers/upac32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/trbhm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/udc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/upac96_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/parsers/upac_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.666107 naludaq-0.17.7/src/naludaq/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.666107 naludaq-0.17.7/src/naludaq/tools/adc2mv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/adc2mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/adc2mv/adc_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/adc2mv/adc_linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/adc2mv/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/adc2mv/pre_adc2mv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/autoaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.670107 naludaq-0.17.7/src/naludaq/tools/autotrigger/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/autotrigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/autotrigger/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/board_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.670107 naludaq-0.17.7/src/naludaq/tools/dac_sweep/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/dac_sweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/dac_sweep/dac_sweep_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/ft60x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/ftdi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.670107 naludaq-0.17.7/src/naludaq/tools/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/optimizers/bayesian_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/optimizers/gainstagetuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.670107 naludaq-0.17.7/src/naludaq/tools/pedestals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.670107 naludaq-0.17.7/src/naludaq/tools/pedestals/_new/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/_new/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/_new/aav3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25345 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/_new/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/_new/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/pedestals_acq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34274 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/pedestals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/pedestals_correcter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/pedestals_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/udc16_pedestals_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/upac32_pedestals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/pedestals/upac96_pedestals_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.670107 naludaq-0.17.7/src/naludaq/tools/threshold_scan/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/threshold_scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/threshold_scan/threshold_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.670107 naludaq-0.17.7/src/naludaq/tools/timing_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/timing_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/timing_cal/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/timing_cal/correcter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.670107 naludaq-0.17.7/src/naludaq/tools/waiter/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/waiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-31 20:11:29.000000 naludaq-0.17.7/src/naludaq/tools/waiter/eventwaiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.646105 naludaq-0.17.7/src/naludaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-05-31 20:11:48.000000 naludaq-0.17.7/src/naludaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-05-31 20:11:48.000000 naludaq-0.17.7/src/naludaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:11:48.000000 naludaq-0.17.7/src/naludaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-31 20:11:48.000000 naludaq-0.17.7/src/naludaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 20:11:48.000000 naludaq-0.17.7/src/naludaq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:11:48.670107 naludaq-0.17.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-31 20:11:29.000000 naludaq-0.17.7/tests/test_naludaq.py
```

### Comparing `naludaq-0.17.6/LICENSE.txt` & `naludaq-0.17.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/PKG-INFO` & `naludaq-0.17.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naludaq
-Version: 0.17.6
+Version: 0.17.7
 Summary: Backend package for Nalu Scientific hardware
 Home-page: 
 Author: Thomas Yang, Emily Lum, Terry Pham
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naludaq-0.17.6/README.md` & `naludaq-0.17.7/README.md`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/pyproject.toml` & `naludaq-0.17.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/setup.py` & `naludaq-0.17.7/setup.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/backend/client.py` & `naludaq-0.17.7/src/naludaq/backend/client.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/backend/context.py` & `naludaq-0.17.7/src/naludaq/backend/context.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/backend/exceptions.py` & `naludaq-0.17.7/src/naludaq/backend/exceptions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/backend/managers/acquisitions.py` & `naludaq-0.17.7/src/naludaq/backend/managers/acquisitions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/backend/managers/connection.py` & `naludaq-0.17.7/src/naludaq/backend/managers/connection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/backend/managers/io.py` & `naludaq-0.17.7/src/naludaq/backend/managers/io.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/backend/models/acquisition.py` & `naludaq-0.17.7/src/naludaq/backend/models/acquisition.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+import copy
 import gzip
 import mmap
 import os
 import pickle
 import struct
-from collections import defaultdict
+from collections import defaultdict, deque
 from copy import deepcopy
 from pathlib import Path
 from typing import Iterator
 
 import yaml
 
 from naludaq.backend.context import Context
 from naludaq.backend.exceptions import AcquisitionError, BackendError
 from naludaq.helpers.exceptions import BadDataError
+from naludaq.models import Acquisition
 from naludaq.parsers import get_parser
 from naludaq.tools.waiter import EventWaiter
 
 AVAILABLE_MISC_DATA_KEYS = ["pedestals", "caldata", "timingcal", "readout_metadata"]
 
 # Disallowed characters for names on windows/linux
 # https://stackoverflow.com/questions/4814040/allowed-characters-in-filename
@@ -114,14 +116,19 @@
     @property
     def length(self) -> int:
         """Get the number of events in the acquisition"""
         info = self._get_info_or_raise()
         return info["len"]
 
     @property
+    def path(self) -> str:
+        """Get the path to the acquisition on the remote"""
+        return self._get_info_or_raise()["path"]
+
+    @property
     def metadata(self) -> dict:
         """Get the acquisition metadata."""
         cache = RemoteAcquisition._METADATA_CACHE
         key = self._cache_key()
         metadata = cache.get(key, None)
         if metadata is None:
             info = self._get_info_or_raise()
@@ -481,15 +488,15 @@
     def name(self) -> str:
         """Acquisition name"""
         return self._name
 
     @property
     def metadata(self) -> dict:
         """Acquisition metadata"""
-        return self.metadata
+        return self._metadata
 
     @property
     def events(self) -> list[dict]:
         """List of events transferred from the remote"""
         return self._events
 
     @property
@@ -566,62 +573,134 @@
             parser (Parser): the parser to use
 
         Returns:
             list[dict]: list of parsed events
         """
         return [parser.parse(event) for event in self]
 
+    def to_legacy_acquisition(self, deepcopy: bool = False) -> Acquisition:
+        """Convert to a legacy acquisition object.
+
+        Not all information will be transferred, only the main stuff.
+        """
+        maybe_copy = lambda x: copy.deepcopy(x) if deepcopy else x
+
+        acq = Acquisition(name=self.name)
+        acq.events = deque(maybe_copy(self.events))
+        acq.pedestals = maybe_copy(self.pedestals)
+        acq.caldata = maybe_copy(self.caldata)
+        acq.timingcal = maybe_copy(self.timingcal)
+        acq.params = maybe_copy(self.metadata.get("params", {}))
+        acq.registers = maybe_copy(self.metadata.get("registers", {}))
+        acq.model = acq.params.get("model", None)
+
+        return acq
+
 
 class DiskChunk:
     INDEX_ENTRY_SIZE = 8
 
     def __init__(self, index_path: Path, bin_path: Path):
         """Utility for reading chunk files directly from disk.
 
+        The chunk will be opened on instantiation. It is recommended to use
+        this object as a context manager to ensure the chunk is closed when
+        it is no longer needed.
+
         Args:
             index_path (Path): path to index file
             bin_path (Path): path to binary file
         """
-        self._index_file = open(index_path, "rb+")
-        self._bin_file = open(bin_path, "rb+")
-        self._index_mmap = mmap.mmap(
-            self._index_file.fileno(), os.path.getsize(index_path)
-        )
-        self._bin_mmap = mmap.mmap(self._bin_file.fileno(), os.path.getsize(bin_path))
-
-        self._version = self._read_bin_header()["version"]
-        self._metadata = self._read_metadata()
-        self._parser = get_parser(self._metadata["params"])
+        if not isinstance(index_path, (Path, str)) or not isinstance(
+            bin_path, (Path, str)
+        ):
+            raise TypeError("Path must be a string or Path object")
+        self._index_path = Path(index_path)
+        self._bin_path = Path(bin_path)
+        self._open = False
+        self.open()
 
     @property
     def metadata(self) -> dict:
-        """Get the chunk metadata"""
+        """Get the chunk metadata
+
+        Raises:
+            IOError: if the chunk is not open
+        """
+        self._raise_if_closed()
         return self._metadata
 
     @property
     def version(self) -> int:
-        """Get the chunk format revision number"""
+        """Get the chunk format revision number.
+
+        Raises:
+            IOError: if the chunk is not open
+        """
+        self._raise_if_closed()
         return self._version
 
     def __len__(self) -> int:
-        """Get the number of events in the chunk"""
+        """Get the number of events in the chunk
+
+        Raises:
+            IOError: if the chunk is not open
+        """
+        self._raise_if_closed()
         return len(self._index_mmap) // DiskChunk.INDEX_ENTRY_SIZE
 
+    def __del__(self):
+        """Close the chunk file"""
+        self.close()
+
+    def __enter__(self):
+        """Context manager enter"""
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        """Context manager exit"""
+        self.close()
+
+    def open(self):
+        self._index_file = open(self._index_path, "rb+")
+        self._bin_file = open(self._bin_path, "rb+")
+        self._index_mmap = mmap.mmap(
+            self._index_file.fileno(), os.path.getsize(self._index_path)
+        )
+        self._bin_mmap = mmap.mmap(
+            self._bin_file.fileno(), os.path.getsize(self._bin_path)
+        )
+        self._open = True
+
+        self._version = self._read_bin_header()["version"]
+        self._metadata = self._read_metadata()
+        self._parser = get_parser(self._metadata["params"])
+
+    def close(self):
+        """Close the chunk file"""
+        if self._open:
+            self._index_mmap.close()
+            self._index_file.close()
+            self._bin_mmap.close()
+            self._bin_file.close()
+
     def raw_event(self, index: int) -> dict:
         """Get a raw event from the chunk.
 
         Args:
             index (int): index of the event in the chunk.
 
         Returns:
             dict: the raw event
 
         Raises:
             IndexError: if the index is out of bounds
+            IOError: if the chunk is closed
         """
+        self._raise_if_closed()
         index = _resolve_index_or_raise(index, len(self))
         start = index * DiskChunk.INDEX_ENTRY_SIZE
         end = start + DiskChunk.INDEX_ENTRY_SIZE
         entry = self._index_mmap[start:end]
         offset, length = struct.unpack("II", entry)
         event = self._bin_mmap[offset : offset + length]
         return _build_raw_event_dict(event, index)
@@ -635,74 +714,152 @@
             index (int): index of the event in the chunk.
 
         Returns:
             bytes: the parsed event
 
         Raises:
             IndexError: if the index is out of bounds
+            IOError: if the chunk is closed
         """
+        self._raise_if_closed()
         return self._parser.parse(self.raw_event(index))
 
     def _read_metadata(self) -> dict:
-        """Read metadata from the bin file."""
+        """Read metadata from the bin file.
+
+        Raises:
+            IOError: if the chunk is closed
+        """
+        self._raise_if_closed()
         metadata_length = self._read_bin_header()["metadata_length"]
         metadata = self._bin_mmap[8 : 8 + metadata_length]
         return yaml.safe_load(metadata)
 
     def _read_bin_header(self) -> dict:
         """Read the header from the binary file.
 
         Returns:
             dict: contains keys "version" and "metadata_length"
+
+        Raises:
+            IOError: if the chunk is closed
         """
+        self._raise_if_closed()
         version, _, metadata_length = struct.unpack("HHI", self._bin_mmap[:8])  # hello!
         return {
             "version": version,
             "metadata_length": metadata_length,
         }
 
+    def _raise_if_closed(self):
+        if not self._open:
+            raise IOError("Chunk is closed")
+
 
 class DiskAcquisition:
     def __init__(self, path: Path):
         """Utility for accessing acquisition directly from disk.
 
+        The acquisition will be opened on instantiation. It is recommended to use
+        this object as a context manager to ensure the acquisition is closed when
+        it is no longer needed.
+
         Important: the acquisition should not be mutated while this object is alive.
         If the acquisition changes, the DiskAcquisition must be recreated.
 
         Args:
             path (Path): path to the acquisition folder.
 
         Raises:
             InvalidAcquisitionError: if the path is not a valid acquisition.
         """
+        if not isinstance(path, (Path, str)):
+            raise TypeError("Path must be a string or Path object")
         path = Path(path).resolve()
         if not DiskAcquisition._is_acquisition(path):
             raise AcquisitionError("Not a valid acquisition")
         self._root = path
-        self._chunks = self._find_chunks()
-        self._event_count = sum(len(chunk) for chunk in self._chunks)
-
-        with open(path / "metadata.yml", "r") as f:
-            self._metadata = yaml.safe_load(f)
+        self._open = False
+        self.open()
 
     def __len__(self) -> int:
         """Get the number of events in the acquisition"""
         return self._event_count
 
+    def __del__(self):
+        """Close the acquisition"""
+        self.close()
+
+    def __enter__(self) -> "DiskAcquisition":
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.close()
+
+    def __getitem__(self, index: "int | slice") -> "dict | list[dict]":
+        """Get one or more parsed event from the acquisition.
+
+        Args:
+            index (int | slice): index(es) of the event(s) in the acquisition.
+
+        Returns:
+            "dict | list[dict]": the event(s)
+
+        Raises:
+            IndexError: if the index is out of bounds
+            IOError: if the acquisition is closed
+        """
+        self._raise_if_closed()
+        result = None
+        if isinstance(index, int):
+            index = _resolve_index_or_raise(index, len(self))
+            result = self.parsed_event(index)
+        elif isinstance(index, slice):
+            result = [self.parsed_event(i) for i in range(*index.indices(len(self)))]
+        else:
+            raise TypeError("Index must be an int or slice")
+        return result
+
+    def open(self):
+        """Open the acquisition for reading.
+
+        If the acquisition is already open, this is a no-op.
+        """
+        if self._open:
+            return
+        self._chunks = self._find_chunks()
+        self._event_count = sum(len(chunk) for chunk in self._chunks)
+        with open(self._root / "metadata.yml", "r") as f:
+            self._metadata = yaml.safe_load(f)
+        self._open = True
+
+    def close(self):
+        """Close the acquisition"""
+        for chunk in self._chunks:
+            chunk.close()
+        self._chunks = []
+        self._open = False
+
     @property
     def chunks(self) -> list[DiskChunk]:
         """Get a list of chunks in the acquisition"""
         return self._chunks.copy()
 
     @property
     def metadata(self) -> dict:
         """Get the acquisition metadata"""
+        self._raise_if_closed()
         return self._metadata
 
     @property
+    def params(self) -> dict:
+        """Get parameters describing the board"""
+        return self._metadata.get("params", {})
+
+    @property
     def readout_metadata(self) -> "dict | None":
         """Get/set the readout metadata for this acquisition"""
         return self._fetch_misc_data("readout_metadata")
 
     @readout_metadata.setter
     def readout_metadata(self, metadata: "dict | None"):
         self._store_misc_data("readout_metadata", metadata)
@@ -741,30 +898,34 @@
             index (int): index of the event
 
         Returns:
             bytes: the raw event data
 
         Raises:
             IndexError: if the index is out of bounds
+            IOError: if the acquisition is not open
         """
+        self._raise_if_closed()
         chunk, index_in_chunk = self._map_to_chunk(index)
         return chunk.raw_event(index_in_chunk)
 
     def parsed_event(self, index: int) -> bytes:
         """Get a parsed event from the acquisition.
 
         Args:
             index (int): index of the event
 
         Returns:
             bytes: the raw event data
 
         Raises:
             IndexError: if the index is out of bounds
+            IOError: if the acquisition is not open
         """
+        self._raise_if_closed()
         chunk, index_in_chunk = self._map_to_chunk(index)
         return chunk.parsed_event(index_in_chunk)
 
     def _map_to_chunk(self, index: int) -> tuple[DiskChunk, int]:
         """Map an absolute index to a chunk and a relative index.
 
         Args:
@@ -803,20 +964,22 @@
 
     def _fetch_misc_data(self, type: str):
         """Read misc data from the acquisition.
 
         Args:
             type (str): the type of misc data
 
-        Raises:
-            AcquisitionError: if the misc data is invalid
-
         Returns:
             object: The deserialized misc data
+
+        Raises:
+            AcquisitionError: if the misc data is invalid
+            IOError: if the acquisition is not open
         """
+        self._raise_if_closed()
         try:
             with open(self._root / type, "rb") as f:
                 data = f.read()
         except:  # means there is no misc data
             return None
         try:
             return _deserialize_misc_data(data)
@@ -829,22 +992,28 @@
         Args:
             type (str): the misc data type name
             obj (object): the misc data
 
         Raises:
             ValueError: if the misc type is invalid or the object could not
                 be serialized.
+            IOError: if the acquisition is not open
         """
+        self._raise_if_closed()
         try:
             data = _serialize_misc_data(obj)
         except ValueError:
             raise
         with open(self._root / type, "wb") as f:
             f.write(data)
 
+    def _raise_if_closed(self):
+        if not self._open:
+            raise IOError("Acquisition is not open")
+
     @staticmethod
     def _is_acquisition(root: Path) -> bool:
         """Check if the given path is a valid acquisition"""
         return root.is_dir() and (root / "metadata.yml").exists()
 
 
 def _build_raw_event_dict(rawdata: bytes, index: int) -> dict:
```

### Comparing `naludaq-0.17.6/src/naludaq/backend/models/device.py` & `naludaq-0.17.7/src/naludaq/backend/models/device.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/__init__.py` & `naludaq-0.17.7/src/naludaq/board/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/board_inits.py` & `naludaq-0.17.7/src/naludaq/board/board_inits.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/connections/_FTDI.py` & `naludaq-0.17.7/src/naludaq/board/connections/_FTDI.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/connections/_MockUART.py` & `naludaq-0.17.7/src/naludaq/board/connections/_MockUART.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/connections/_UART.py` & `naludaq-0.17.7/src/naludaq/board/connections/_UART.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/connections/_USB.py` & `naludaq-0.17.7/src/naludaq/board/connections/_USB.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/connections/base_connection.py` & `naludaq-0.17.7/src/naludaq/board/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/connections/connection_factory.py` & `naludaq-0.17.7/src/naludaq/board/connections/connection_factory.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/connections/tcp.py` & `naludaq-0.17.7/src/naludaq/board/connections/tcp.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/connections/udp.py` & `naludaq-0.17.7/src/naludaq/board/connections/udp.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/initializers/__init__.py` & `naludaq-0.17.7/src/naludaq/board/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/initializers/aardvarcv3.py` & `naludaq-0.17.7/src/naludaq/board/initializers/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/initializers/aodsoc.py` & `naludaq-0.17.7/src/naludaq/board/initializers/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/initializers/init_aodsv2_eval.py` & `naludaq-0.17.7/src/naludaq/board/initializers/init_aodsv2_eval.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/initializers/init_hdsocv1.py` & `naludaq-0.17.7/src/naludaq/board/initializers/init_hdsocv1.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/initializers/init_udc.py` & `naludaq-0.17.7/src/naludaq/board/initializers/init_udc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/initializers/init_upac96.py` & `naludaq-0.17.7/src/naludaq/board/initializers/init_upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/initializers/trbhm.py` & `naludaq-0.17.7/src/naludaq/board/initializers/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/board/params.py` & `naludaq-0.17.7/src/naludaq/board/params.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/communication/__init__.py` & `naludaq-0.17.7/src/naludaq/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/communication/analog_registers.py` & `naludaq-0.17.7/src/naludaq/communication/analog_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/communication/control_registers.py` & `naludaq-0.17.7/src/naludaq/communication/control_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/communication/digital_registers.py` & `naludaq-0.17.7/src/naludaq/communication/digital_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/communication/i2c.py` & `naludaq-0.17.7/src/naludaq/communication/i2c.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/communication/i2c_registers.py` & `naludaq-0.17.7/src/naludaq/communication/i2c_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/communication/registers.py` & `naludaq-0.17.7/src/naludaq/communication/registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/__init__.py` & `naludaq-0.17.7/src/naludaq/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/analog_debug_controller.py` & `naludaq-0.17.7/src/naludaq/controllers/analog_debug_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/biasing_mode/__init__.py` & `naludaq-0.17.7/src/naludaq/controllers/biasing_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/biasing_mode/udc16.py` & `naludaq-0.17.7/src/naludaq/controllers/biasing_mode/udc16.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/board/__init__.py` & `naludaq-0.17.7/src/naludaq/controllers/board/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/board/aodsoc.py` & `naludaq-0.17.7/src/naludaq/controllers/board/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/board/default.py` & `naludaq-0.17.7/src/naludaq/controllers/board/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/board/hdsoc.py` & `naludaq-0.17.7/src/naludaq/controllers/board/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/board/oleas.py` & `naludaq-0.17.7/src/naludaq/controllers/board/oleas.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/board/trbhm.py` & `naludaq-0.17.7/src/naludaq/controllers/board/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/board/udc.py` & `naludaq-0.17.7/src/naludaq/controllers/board/udc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/board/upac.py` & `naludaq-0.17.7/src/naludaq/controllers/board/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/board/upac96.py` & `naludaq-0.17.7/src/naludaq/controllers/board/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/connection/__init__.py` & `naludaq-0.17.7/src/naludaq/controllers/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/connection/connection_controller.py` & `naludaq-0.17.7/src/naludaq/controllers/connection/connection_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/connection/upac.py` & `naludaq-0.17.7/src/naludaq/controllers/connection/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/connection/upac96.py` & `naludaq-0.17.7/src/naludaq/controllers/connection/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/external_dac/__init__.py` & `naludaq-0.17.7/src/naludaq/controllers/external_dac/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/external_dac/ad5671.py` & `naludaq-0.17.7/src/naludaq/controllers/external_dac/ad5671.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/external_dac/ad5675.py` & `naludaq-0.17.7/src/naludaq/controllers/external_dac/ad5675.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/external_dac/base.py` & `naludaq-0.17.7/src/naludaq/controllers/external_dac/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/external_dac/dac7578.py` & `naludaq-0.17.7/src/naludaq/controllers/external_dac/dac7578.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/external_dac/hdsoc.py` & `naludaq-0.17.7/src/naludaq/controllers/external_dac/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/external_dac/i2c_dac.py` & `naludaq-0.17.7/src/naludaq/controllers/external_dac/i2c_dac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/external_dac/trbhm.py` & `naludaq-0.17.7/src/naludaq/controllers/external_dac/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/external_dac/upac32.py` & `naludaq-0.17.7/src/naludaq/controllers/external_dac/upac32.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/gainstages/__init__.py` & `naludaq-0.17.7/src/naludaq/controllers/gainstages/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/gainstages/aodsv2.py` & `naludaq-0.17.7/src/naludaq/controllers/gainstages/aodsv2.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/gainstages/oddsock_aods.py` & `naludaq-0.17.7/src/naludaq/controllers/gainstages/oddsock_aods.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/peripherals/__init__.py` & `naludaq-0.17.7/src/naludaq/controllers/peripherals/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/peripherals/aardvarcv3.py` & `naludaq-0.17.7/src/naludaq/controllers/peripherals/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/peripherals/aodsoc.py` & `naludaq-0.17.7/src/naludaq/controllers/peripherals/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/peripherals/hdsoc.py` & `naludaq-0.17.7/src/naludaq/controllers/peripherals/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/peripherals/peripherals_controller.py` & `naludaq-0.17.7/src/naludaq/controllers/peripherals/peripherals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/peripherals/upac.py` & `naludaq-0.17.7/src/naludaq/controllers/peripherals/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/peripherals/upac96.py` & `naludaq-0.17.7/src/naludaq/controllers/peripherals/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/project_controller.py` & `naludaq-0.17.7/src/naludaq/controllers/project_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/readout/__init__.py` & `naludaq-0.17.7/src/naludaq/controllers/readout/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/readout/aardvarcv3.py` & `naludaq-0.17.7/src/naludaq/controllers/readout/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/readout/default.py` & `naludaq-0.17.7/src/naludaq/controllers/readout/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/readout/hdsoc.py` & `naludaq-0.17.7/src/naludaq/controllers/readout/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/readout/trbhm.py` & `naludaq-0.17.7/src/naludaq/controllers/readout/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/si5341_controller.py` & `naludaq-0.17.7/src/naludaq/controllers/si5341_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/tia/__init__.py` & `naludaq-0.17.7/src/naludaq/controllers/tia/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/tia/base.py` & `naludaq-0.17.7/src/naludaq/controllers/tia/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/tia/hdsoc.py` & `naludaq-0.17.7/src/naludaq/controllers/tia/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/trigger/__init__.py` & `naludaq-0.17.7/src/naludaq/controllers/trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/trigger/aodsoc.py` & `naludaq-0.17.7/src/naludaq/controllers/trigger/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/trigger/default.py` & `naludaq-0.17.7/src/naludaq/controllers/trigger/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/trigger/hdsoc.py` & `naludaq-0.17.7/src/naludaq/controllers/trigger/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/trigger/trbhm.py` & `naludaq-0.17.7/src/naludaq/controllers/trigger/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/trigger/upac.py` & `naludaq-0.17.7/src/naludaq/controllers/trigger/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/controllers/trigger/upac96.py` & `naludaq-0.17.7/src/naludaq/controllers/trigger/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/daq/__init__.py` & `naludaq-0.17.7/src/naludaq/daq/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/daq/debugdaq.py` & `naludaq-0.17.7/src/naludaq/daq/debugdaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/daq/lightdaq.py` & `naludaq-0.17.7/src/naludaq/daq/lightdaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/daq/preprocess.py` & `naludaq-0.17.7/src/naludaq/daq/preprocess.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/daq/workers/__init__.py` & `naludaq-0.17.7/src/naludaq/daq/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/daq/workers/answer_parser_worker.py` & `naludaq-0.17.7/src/naludaq/daq/workers/answer_parser_worker.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/daq/workers/csv_storage_worker.py` & `naludaq-0.17.7/src/naludaq/daq/workers/csv_storage_worker.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/daq/workers/packager/__init__.py` & `naludaq-0.17.7/src/naludaq/daq/workers/packager/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/daq/workers/packager/worker_packager.py` & `naludaq-0.17.7/src/naludaq/daq/workers/packager/worker_packager.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/daq/workers/packager/worker_packager_debug.py` & `naludaq-0.17.7/src/naludaq/daq/workers/packager/worker_packager_debug.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py` & `naludaq-0.17.7/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/daq/workers/postprocessing.py` & `naludaq-0.17.7/src/naludaq/daq/workers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/daq/workers/worker_parser.py` & `naludaq-0.17.7/src/naludaq/daq/workers/worker_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/daq/workers/worker_serial_reader.py` & `naludaq-0.17.7/src/naludaq/daq/workers/worker_serial_reader.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/daq/workers/worker_usb_reader.py` & `naludaq-0.17.7/src/naludaq/daq/workers/worker_usb_reader.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/devices/eeprom.py` & `naludaq-0.17.7/src/naludaq/devices/eeprom.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/devices/i2c_device.py` & `naludaq-0.17.7/src/naludaq/devices/i2c_device.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/devices/ltc2990.py` & `naludaq-0.17.7/src/naludaq/devices/ltc2990.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/helpers/decorators.py` & `naludaq-0.17.7/src/naludaq/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/helpers/exceptions.py` & `naludaq-0.17.7/src/naludaq/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/helpers/helper_functions.py` & `naludaq-0.17.7/src/naludaq/helpers/helper_functions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/helpers/register_cache.py` & `naludaq-0.17.7/src/naludaq/helpers/register_cache.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/helpers/semiton.py` & `naludaq-0.17.7/src/naludaq/helpers/semiton.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/io/__init__.py` & `naludaq-0.17.7/src/naludaq/io/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/io/csv_writer.py` & `naludaq-0.17.7/src/naludaq/io/csv_writer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/io/hdf5.py` & `naludaq-0.17.7/src/naludaq/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/io/io_manager.py` & `naludaq-0.17.7/src/naludaq/io/io_manager.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/models/acq_converters.py` & `naludaq-0.17.7/src/naludaq/models/acq_converters.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/models/acquisition.py` & `naludaq-0.17.7/src/naludaq/models/acquisition.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/naludaq.py` & `naludaq-0.17.7/src/naludaq/naludaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/parsers/__init__.py` & `naludaq-0.17.7/src/naludaq/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/parsers/aardvarcv3_parser.py` & `naludaq-0.17.7/src/naludaq/parsers/aardvarcv3_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/parsers/answer_parser.py` & `naludaq-0.17.7/src/naludaq/parsers/answer_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/parsers/aodsoc_parser.py` & `naludaq-0.17.7/src/naludaq/parsers/aodsoc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/parsers/asocv3_parser.py` & `naludaq-0.17.7/src/naludaq/parsers/asocv3_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/parsers/hdsoc_parser.py` & `naludaq-0.17.7/src/naludaq/parsers/hdsoc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/parsers/headers/__init__.py` & `naludaq-0.17.7/src/naludaq/parsers/headers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/parsers/headers/asoc.py` & `naludaq-0.17.7/src/naludaq/parsers/headers/asoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/parsers/headers/asocv2.py` & `naludaq-0.17.7/src/naludaq/parsers/headers/asocv2.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/parsers/headers/base.py` & `naludaq-0.17.7/src/naludaq/parsers/headers/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/parsers/headers/siread.py` & `naludaq-0.17.7/src/naludaq/parsers/headers/siread.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/parsers/headers/trbhm.py` & `naludaq-0.17.7/src/naludaq/parsers/headers/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/parsers/headers/upac32.py` & `naludaq-0.17.7/src/naludaq/parsers/headers/upac32.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/parsers/parser.py` & `naludaq-0.17.7/src/naludaq/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/parsers/trbhm_parser.py` & `naludaq-0.17.7/src/naludaq/parsers/trbhm_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/parsers/udc_parser.py` & `naludaq-0.17.7/src/naludaq/parsers/udc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/parsers/upac96_parser.py` & `naludaq-0.17.7/src/naludaq/parsers/upac96_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/parsers/upac_parser.py` & `naludaq-0.17.7/src/naludaq/parsers/upac_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/adc2mv/adc_converter.py` & `naludaq-0.17.7/src/naludaq/tools/adc2mv/adc_converter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/adc2mv/adc_linear_regression.py` & `naludaq-0.17.7/src/naludaq/tools/adc2mv/adc_linear_regression.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/adc2mv/generate.py` & `naludaq-0.17.7/src/naludaq/tools/adc2mv/generate.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/adc2mv/pre_adc2mv.py` & `naludaq-0.17.7/src/naludaq/tools/adc2mv/pre_adc2mv.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/autoaction.py` & `naludaq-0.17.7/src/naludaq/tools/autoaction.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/autotrigger/default.py` & `naludaq-0.17.7/src/naludaq/tools/autotrigger/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/board_backup.py` & `naludaq-0.17.7/src/naludaq/tools/board_backup.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/dac_sweep/dac_sweep_controller.py` & `naludaq-0.17.7/src/naludaq/tools/dac_sweep/dac_sweep_controller.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import time
-from collections import deque
 
 import numpy as np
 
 from naludaq.communication import control_registers, digital_registers
 from naludaq.controllers import get_dac_controller
 from naludaq.helpers.exceptions import BoardParameterError, PedestalsDataCaptureError
 from naludaq.tools.pedestals import get_pedestals_controller
@@ -23,29 +22,31 @@
     the user to find the linear region and linear regression values on
     a per sample basis.
 
     Args:
         board (naludaq.board): Board object
 
     Attributes:
-        num_captures_for_peds_avg: How many datapoints/samplepoint used to calculate the average.
+        num_attempts: How many attempts to try a DAC value before skipping that dac value
 
     raises:
         BoardParameterError if ext_dac fields are not available amoung the board params.
     """
 
     def __init__(self, board):
         # The type of daq used depends on the connection type
         self._board = None
         self.board = board
-        self.num_evt_per_dacval = 10
-        self.dac_max_counts: int = self._get_max_counts()
+        self._num_attempts = 2
+        self._dac_min_counts: int = 0
+        self._dac_max_counts: int = self._get_max_counts()
         self._progress: list = []
         self._cancel = False
-        self.ped_ctrl = None
+        self.ped_ctrl = get_pedestals_controller(board)
+        self._dac_ctrl = get_dac_controller(board)
         self._backup_dac: dict = {}
 
     def _get_max_counts(self) -> int:
         try:
             return self.board.params["ext_dac"]["max_counts"]
         except KeyError as e:
             raise BoardParameterError(
@@ -67,23 +68,57 @@
         """
         return self._dac_max_counts
 
     @dac_max_counts.setter
     def dac_max_counts(self, value):
         if not isinstance(value, int):
             raise TypeError("dac max counts must be an int.")
-        min_val = self.board.params["ext_dac"].get("min_counts", 0)
-        max_val = self.board.params["ext_dac"].get("max_counts", 4095)
-        if not 0 < value <= max_val:
+        max_val = self._get_max_counts()
+        if not self.dac_min_counts <= value <= max_val:
             ValueError(
-                f"dac_max_counts must be a value between {min_val} and {max_val}"
+                f"dac_max_counts must be a value between {self.dac_min_counts} and {max_val}"
             )
         self._dac_max_counts = value
 
     @property
+    def dac_min_counts(self):
+        """Get/Set the min count value for the DAC.
+
+        The min count for a board should be 0, unless otherwise stated
+
+        Raises:
+            TypeError: if value is not an int
+            ValueError: if value is outside of the boards accepted range.
+        """
+        return self._dac_min_counts
+
+    @dac_min_counts.setter
+    def dac_min_counts(self, value):
+        if not isinstance(value, int):
+            raise TypeError("dac min counts must be an int.")
+        min_val = self.board.params["ext_dac"].get("min_counts", 0)
+        if not min_val <= value <= self.dac_max_counts:
+            ValueError(
+                f"dac_min_counts must be a value between {min_val} and {self.dac_max_counts}"
+            )
+        self._dac_min_counts = value
+
+    @property
+    def num_attempts(self):
+        return self._num_attempts
+
+    @num_attempts.setter
+    def num_attempts(self, value):
+        if not isinstance(value, int):
+            raise TypeError("num_attempts must be an int.")
+        if value < 0:
+            raise ValueError("num_attempts must be positive")
+        self._num_attempts = value
+
+    @property
     def board(self):
         return self._board
 
     @board.setter
     def board(self, board):
         self._board = board
 
@@ -109,93 +144,113 @@
             self.ped_ctrl.cancel()
 
     def dac_sweep(
         self,
         step_size: int = 50,
         min_counts: int = 0,
         max_counts: int = None,
-        events_per_datapt: int = 10,
+        num_captures: int = 3,
+        num_warmup_events: int = 1,
         channels: list = None,
     ):
         """Perform a dac sweep with a given step size.
         IMPORTANT: TURN OFF CONNECTED FUNCTION GENERATORS BEFORE RUNNING
         Ext-dac + signal = :(
 
             Args:
                 step_size (int): Step sizes for the ext-dac, from 0 to max_counts
+                min_counts (int): minimum DAC value to start sweep from
+                max_counts (int): maximum DAC value to stop sweep at
+                num_captures (int): number of events per data point
+                channels (list): list of channel numbers to sweep over
 
             Returns:
                 dac_sweep (dict): In form dac_sweep[Dac Val][Block #][Event #] or None
                     if the dac sweep was canceled.
-                min_counts (int): minimum DAC value to start sweep from
-                max_counts (int): maximum DAC value to stop sweep at
-                events_per_datapt (int): number of events per data point
-                channels (list): list of channel numbers to sweep over
         """
         self._cancel = False
 
         if step_size <= 0 or step_size > self.dac_max_counts:
             raise ValueError(f"Step size is out of bounds: 0-{self.dac_max_counts}")
         if channels is None:
             channels = list(range(self.board.channels))
         if max_counts is None:
             max_counts = self.board.params["ext_dac"]["max_counts"]
 
-        self._backup_dac_values()
+        self._backup_settings()
 
-        output2analyze = {}
+        output = {}
 
         ext_dac_values = np.arange(min_counts, max_counts + 1, step_size)
         LOGGER.info(
-            f"Starting DAC Sweep from {min_counts}-{self.dac_max_counts} with step {step_size}"
+            f"Starting DAC Sweep from {min_counts}-{max_counts} with step {step_size}"
         )
 
         for dac_idx, dac_val in enumerate(ext_dac_values):
             dac_val = int(dac_val)
             LOGGER.info(f"Currently running DAC_val: {dac_val}")
             # set dac value for all channels
             self.progress.append(
                 (
                     int(98 * (dac_val - min_counts) / (max_counts - min_counts)),
                     f"Collecting DAC value {dac_idx+1}/{len(ext_dac_values)}",
                 )
             )
-            get_dac_controller(self.board).set_dacs(dac_val, channels)
-            time.sleep(0.001)
-            data2analyze = deque()
-            try:
-                self.ped_ctrl = get_pedestals_controller(self.board, channels=channels)
-                self.ped_ctrl._capture_data_for_pedestals(events_per_datapt)
-                data2analyze = self.ped_ctrl.validated_blocks
-            except PedestalsDataCaptureError:
-                LOGGER.error("Couldn't capture DAC data")
-
-            # Readout data for all channels, all windows.
-            output2analyze[dac_val] = data2analyze
-            LOGGER.info(f"{dac_val} total data: {len(data2analyze)}")
-
+            output[dac_val] = self._run_dac_value(
+                dac_val, channels, num_captures, num_warmup_events
+            )
             if self._cancel:
                 break
 
         # Restore backups
-        self._restore_dac_backup()
+        self._restore_settings()
 
         # Data is probably bad if canceled, so return None
         if self._cancel:
             return None
 
         # save data
         try:
             self.progress.append((99, "Saving DAC Sweep"))
         except:
             LOGGER.debug("Status message couldn't append to self.progress")
-        return output2analyze
+        return output
+
+    def _run_dac_value(self, dac_val, channels, num_captures, num_warmup_events):
+        self._set_dacs(dac_val, channels)
+        for _ in range(self.num_attempts):
+            try:
+                output = self._capture_pedestals(num_captures, num_warmup_events)
+                LOGGER.info(f"{dac_val} total data: {len(output)}")
+                break
+            except PedestalsDataCaptureError:
+                LOGGER.error("Couldn't capture %d DAC data", dac_val)
+                continue
+            except KeyboardInterrupt:
+                self.cancel()
+                break
+        return output
+
+    def _set_dacs(self, dac_val, channels):
+        self._dac_ctrl.set_dacs(dac_val, channels)
+        time.sleep(0.01)
+
+    def _capture_pedestals(self, num_captures: int, num_warmup_events: int):
+        self.ped_ctrl.reset_pedestals()
+        self.ped_ctrl._reset_buffers()
+        self.ped_ctrl.num_captures = num_captures
+        self.ped_ctrl.num_warmup_events = num_warmup_events
+        self.ped_ctrl._capture_data_for_pedestals(num_captures, num_warmup_events)
+        self.ped_ctrl._generate_pedestals_data()
+        self.ped_ctrl._generate_pedestals_from_data()
+        return self.board.pedestals
 
-    def _backup_dac_values(self):
-        """Backup the old dac values during sweep"""
+    def _backup_settings(self):
+        self._backup_pedestals = self.board.pedestals
         self._backup_dac = (
             self.board.params.get("ext_dac", {}).get("channels", {}).copy()
         )
 
-    def _restore_dac_backup(self):
+    def _restore_settings(self):
+        self.board.pedestals = self._backup_pedestals
         for chan, value in self._backup_dac.items():
             get_dac_controller(self.board).set_single_dac(chan, value)
```

### Comparing `naludaq-0.17.6/src/naludaq/tools/data_collector.py` & `naludaq-0.17.7/src/naludaq/tools/data_collector.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/features.py` & `naludaq-0.17.7/src/naludaq/tools/features.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/ft60x.py` & `naludaq-0.17.7/src/naludaq/tools/ft60x.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/ftdi.py` & `naludaq-0.17.7/src/naludaq/tools/ftdi.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/metadata.py` & `naludaq-0.17.7/src/naludaq/tools/metadata.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/optimizers/bayesian_optimizer.py` & `naludaq-0.17.7/src/naludaq/tools/optimizers/bayesian_optimizer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/optimizers/gainstagetuner.py` & `naludaq-0.17.7/src/naludaq/tools/optimizers/gainstagetuner.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/pedestals/__init__.py` & `naludaq-0.17.7/src/naludaq/tools/pedestals/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/pedestals/_new/__init__.py` & `naludaq-0.17.7/src/naludaq/tools/pedestals/_new/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/pedestals/_new/aav3.py` & `naludaq-0.17.7/src/naludaq/tools/pedestals/_new/aav3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/pedestals/_new/default.py` & `naludaq-0.17.7/src/naludaq/tools/pedestals/_new/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/pedestals/_new/hdsoc.py` & `naludaq-0.17.7/src/naludaq/tools/pedestals/_new/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py` & `naludaq-0.17.7/src/naludaq/tools/pedestals/aardvarcv3_pedestals_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py` & `naludaq-0.17.7/src/naludaq/tools/pedestals/hdsoc_pedestals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/pedestals/pedestals_acq.py` & `naludaq-0.17.7/src/naludaq/tools/pedestals/pedestals_acq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/pedestals/pedestals_controller.py` & `naludaq-0.17.7/src/naludaq/tools/pedestals/pedestals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/pedestals/pedestals_correcter.py` & `naludaq-0.17.7/src/naludaq/tools/pedestals/pedestals_correcter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/pedestals/pedestals_processor.py` & `naludaq-0.17.7/src/naludaq/tools/pedestals/pedestals_processor.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/pedestals/udc16_pedestals_generator.py` & `naludaq-0.17.7/src/naludaq/tools/pedestals/udc16_pedestals_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/pedestals/upac32_pedestals_controller.py` & `naludaq-0.17.7/src/naludaq/tools/pedestals/upac32_pedestals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/pedestals/upac96_pedestals_generator.py` & `naludaq-0.17.7/src/naludaq/tools/pedestals/upac96_pedestals_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/threshold_scan/__init__.py` & `naludaq-0.17.7/src/naludaq/tools/threshold_scan/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py` & `naludaq-0.17.7/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/threshold_scan/threshold_scan.py` & `naludaq-0.17.7/src/naludaq/tools/threshold_scan/threshold_scan.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/timing_cal/__init__.py` & `naludaq-0.17.7/src/naludaq/tools/timing_cal/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/timing_cal/calibration.py` & `naludaq-0.17.7/src/naludaq/tools/timing_cal/calibration.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/timing_cal/correcter.py` & `naludaq-0.17.7/src/naludaq/tools/timing_cal/correcter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq/tools/waiter/eventwaiter.py` & `naludaq-0.17.7/src/naludaq/tools/waiter/eventwaiter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.17.6/src/naludaq.egg-info/PKG-INFO` & `naludaq-0.17.7/src/naludaq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naludaq
-Version: 0.17.6
+Version: 0.17.7
 Summary: Backend package for Nalu Scientific hardware
 Home-page: 
 Author: Thomas Yang, Emily Lum, Terry Pham
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naludaq-0.17.6/src/naludaq.egg-info/SOURCES.txt` & `naludaq-0.17.7/src/naludaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

