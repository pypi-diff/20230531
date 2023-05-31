# Comparing `tmp/robodyno-1.6.1b0.tar.gz` & `tmp/robodyno-1.6.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robodyno-1.6.1b0.tar", last modified: Fri May 19 05:49:23 2023, max compression
+gzip compressed data, was "robodyno-1.6.1b1.tar", last modified: Mon May 22 07:30:52 2023, max compression
```

## Comparing `robodyno-1.6.1b0.tar` & `robodyno-1.6.1b1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.532642 robodyno-1.6.1b0/
--rw-rw-rw-   0        0        0    11028 2023-05-19 05:49:23.531642 robodyno-1.6.1b0/PKG-INFO
--rw-rw-rw-   0        0        0      126 2023-05-19 05:43:33.000000 robodyno-1.6.1b0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-19 05:49:23.532642 robodyno-1.6.1b0/setup.cfg
--rw-rw-rw-   0        0        0     4940 2023-05-19 05:49:15.000000 robodyno-1.6.1b0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.459128 robodyno-1.6.1b0/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.468128 robodyno-1.6.1b0/src/robodyno/
--rw-rw-rw-   0        0        0     1606 2023-05-17 09:30:59.000000 robodyno-1.6.1b0/src/robodyno/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.486643 robodyno-1.6.1b0/src/robodyno/components/
--rw-rw-rw-   0        0        0     2999 2023-05-18 03:40:55.000000 robodyno-1.6.1b0/src/robodyno/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.497642 robodyno-1.6.1b0/src/robodyno/components/can_bus/
--rw-rw-rw-   0        0        0        0 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/adaptive_gripper.py
--rw-rw-rw-   0        0        0     3772 2023-05-17 02:08:48.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/can_bus_device.py
--rw-rw-rw-   0        0        0        0 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/gps_sensor.py
--rw-rw-rw-   0        0        0     9038 2023-05-18 03:30:30.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/imu_sensor.py
--rw-rw-rw-   0        0        0        0 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/led_driver.py
--rw-rw-rw-   0        0        0    32976 2023-05-19 04:18:34.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/motor.py
--rw-rw-rw-   0        0        0     4768 2023-05-18 03:30:47.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/pwm_driver.py
--rw-rw-rw-   0        0        0     5720 2023-05-17 04:06:44.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/slider_module.py
--rw-rw-rw-   0        0        0     6833 2023-05-18 03:31:00.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/stepper_driver.py
--rw-rw-rw-   0        0        0        0 2023-05-16 14:51:18.000000 robodyno-1.6.1b0/src/robodyno/components/can_bus/vacuum_gripper.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.500643 robodyno-1.6.1b0/src/robodyno/components/config/
--rw-rw-rw-   0        0        0        0 2023-05-16 06:59:20.000000 robodyno-1.6.1b0/src/robodyno/components/config/__init__.py
--rw-rw-rw-   0        0        0     2149 2023-05-17 05:24:55.000000 robodyno-1.6.1b0/src/robodyno/components/config/model.py
--rw-rw-rw-   0        0        0     5980 2023-05-19 03:28:35.000000 robodyno-1.6.1b0/src/robodyno/components/config/robottime_config.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.505643 robodyno-1.6.1b0/src/robodyno/components/webots/
--rw-rw-rw-   0        0        0        0 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/components/webots/__init__.py
--rw-rw-rw-   0        0        0    19697 2023-05-16 03:47:38.000000 robodyno-1.6.1b0/src/robodyno/components/webots/motor.py
--rw-rw-rw-   0        0        0     3456 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/components/webots/slider_module.py
--rw-rw-rw-   0        0        0     1543 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/components/webots/webots_device.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.508642 robodyno-1.6.1b0/src/robodyno/interfaces/
--rw-rw-rw-   0        0        0      533 2023-05-18 03:40:10.000000 robodyno-1.6.1b0/src/robodyno/interfaces/__init__.py
--rw-rw-rw-   0        0        0     9768 2023-05-19 05:14:39.000000 robodyno-1.6.1b0/src/robodyno/interfaces/can_bus.py
--rw-rw-rw-   0        0        0     3069 2023-05-16 05:58:37.000000 robodyno-1.6.1b0/src/robodyno/interfaces/webots.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.509642 robodyno-1.6.1b0/src/robodyno/robots/
--rw-rw-rw-   0        0        0      309 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.511642 robodyno-1.6.1b0/src/robodyno/robots/four_dof_palletizing_robot/
--rw-rw-rw-   0        0        0       50 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/four_dof_palletizing_robot/__init__.py
--rw-rw-rw-   0        0        0     7949 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/four_dof_palletizing_robot/four_dof_pallet_robot.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.513642 robodyno-1.6.1b0/src/robodyno/robots/four_dof_scara_robot/
--rw-rw-rw-   0        0        0       46 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/four_dof_scara_robot/__init__.py
--rw-rw-rw-   0        0        0     8412 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/four_dof_scara_robot/four_dof_scara_robot.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.516642 robodyno-1.6.1b0/src/robodyno/robots/six_dof_collaborative_robot/
--rw-rw-rw-   0        0        0       51 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/six_dof_collaborative_robot/__init__.py
--rw-rw-rw-   0        0        0    10624 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/six_dof_collaborative_robot/six_dof_collab_robot.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.518651 robodyno-1.6.1b0/src/robodyno/robots/three_dof_delta_robot/
--rw-rw-rw-   0        0        0       48 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/three_dof_delta_robot/__init__.py
--rw-rw-rw-   0        0        0     9792 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/three_dof_delta_robot/three_dof_delta_robot.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.521643 robodyno-1.6.1b0/src/robodyno/robots/three_dof_palletizing_robot/
--rw-rw-rw-   0        0        0       50 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/three_dof_palletizing_robot/__init__.py
--rw-rw-rw-   0        0        0     7512 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/three_dof_palletizing_robot/three_dof_pallet_robot.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.524643 robodyno-1.6.1b0/src/robodyno/robots/utils/
--rw-rw-rw-   0        0        0        0 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/utils/__init__.py
--rw-rw-rw-   0        0        0      626 2023-05-05 06:04:00.000000 robodyno-1.6.1b0/src/robodyno/robots/utils/interpolations.py
--rw-rw-rw-   0        0        0    59522 2023-05-19 05:16:51.000000 robodyno-1.6.1b0/src/robodyno/robots/utils/transformations.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.530645 robodyno-1.6.1b0/src/robodyno/tools/
--rw-rw-rw-   0        0        0        0 2023-05-18 09:35:59.000000 robodyno-1.6.1b0/src/robodyno/tools/__init__.py
--rw-rw-rw-   0        0        0     4183 2023-05-18 04:13:40.000000 robodyno-1.6.1b0/src/robodyno/tools/can_bus_monitor.py
--rw-rw-rw-   0        0        0    16396 2023-05-19 05:11:28.000000 robodyno-1.6.1b0/src/robodyno/tools/cli.py
--rw-rw-rw-   0        0        0     3407 2023-05-19 03:16:35.000000 robodyno-1.6.1b0/src/robodyno/tools/cli_param_types.py
--rw-rw-rw-   0        0        0     3992 2023-05-18 07:23:21.000000 robodyno-1.6.1b0/src/robodyno/tools/motor_info_table.py
-drwxrwxrwx   0        0        0        0 2023-05-19 05:49:23.484644 robodyno-1.6.1b0/src/robodyno.egg-info/
--rw-rw-rw-   0        0        0    11028 2023-05-19 05:49:23.000000 robodyno-1.6.1b0/src/robodyno.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2202 2023-05-19 05:49:23.000000 robodyno-1.6.1b0/src/robodyno.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 05:49:23.000000 robodyno-1.6.1b0/src/robodyno.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1039 2023-05-19 05:49:23.000000 robodyno-1.6.1b0/src/robodyno.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      121 2023-05-19 05:49:23.000000 robodyno-1.6.1b0/src/robodyno.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-19 05:49:23.000000 robodyno-1.6.1b0/src/robodyno.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 07:30:52.860891 robodyno-1.6.1b1/
+-rw-rw-rw-   0        0        0    11028 2023-05-22 07:30:52.860891 robodyno-1.6.1b1/PKG-INFO
+-rw-rw-rw-   0        0        0      126 2023-05-19 05:43:33.000000 robodyno-1.6.1b1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 07:30:52.861897 robodyno-1.6.1b1/setup.cfg
+-rw-rw-rw-   0        0        0     4939 2023-05-19 05:52:20.000000 robodyno-1.6.1b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:30:52.802368 robodyno-1.6.1b1/src/
+drwxrwxrwx   0        0        0        0 2023-05-22 07:30:52.811370 robodyno-1.6.1b1/src/robodyno/
+-rw-rw-rw-   0        0        0     1272 2023-05-22 07:30:46.000000 robodyno-1.6.1b1/src/robodyno/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:30:52.818367 robodyno-1.6.1b1/src/robodyno/components/
+-rw-rw-rw-   0        0        0     2999 2023-05-18 03:40:55.000000 robodyno-1.6.1b1/src/robodyno/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:30:52.829378 robodyno-1.6.1b1/src/robodyno/components/can_bus/
+-rw-rw-rw-   0        0        0        0 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/components/can_bus/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/components/can_bus/adaptive_gripper.py
+-rw-rw-rw-   0        0        0     3772 2023-05-17 02:08:48.000000 robodyno-1.6.1b1/src/robodyno/components/can_bus/can_bus_device.py
+-rw-rw-rw-   0        0        0        0 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/components/can_bus/gps_sensor.py
+-rw-rw-rw-   0        0        0     9038 2023-05-18 03:30:30.000000 robodyno-1.6.1b1/src/robodyno/components/can_bus/imu_sensor.py
+-rw-rw-rw-   0        0        0        0 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/components/can_bus/led_driver.py
+-rw-rw-rw-   0        0        0    32976 2023-05-19 04:18:34.000000 robodyno-1.6.1b1/src/robodyno/components/can_bus/motor.py
+-rw-rw-rw-   0        0        0     4768 2023-05-18 03:30:47.000000 robodyno-1.6.1b1/src/robodyno/components/can_bus/pwm_driver.py
+-rw-rw-rw-   0        0        0     5720 2023-05-17 04:06:44.000000 robodyno-1.6.1b1/src/robodyno/components/can_bus/slider_module.py
+-rw-rw-rw-   0        0        0     6833 2023-05-18 03:31:00.000000 robodyno-1.6.1b1/src/robodyno/components/can_bus/stepper_driver.py
+-rw-rw-rw-   0        0        0        0 2023-05-16 14:51:18.000000 robodyno-1.6.1b1/src/robodyno/components/can_bus/vacuum_gripper.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:30:52.832376 robodyno-1.6.1b1/src/robodyno/components/config/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:59:20.000000 robodyno-1.6.1b1/src/robodyno/components/config/__init__.py
+-rw-rw-rw-   0        0        0     2149 2023-05-17 05:24:55.000000 robodyno-1.6.1b1/src/robodyno/components/config/model.py
+-rw-rw-rw-   0        0        0     5980 2023-05-19 03:28:35.000000 robodyno-1.6.1b1/src/robodyno/components/config/robottime_config.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:30:52.836377 robodyno-1.6.1b1/src/robodyno/components/webots/
+-rw-rw-rw-   0        0        0        0 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/components/webots/__init__.py
+-rw-rw-rw-   0        0        0    19697 2023-05-16 03:47:38.000000 robodyno-1.6.1b1/src/robodyno/components/webots/motor.py
+-rw-rw-rw-   0        0        0     3456 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/components/webots/slider_module.py
+-rw-rw-rw-   0        0        0     1543 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/components/webots/webots_device.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:30:52.839377 robodyno-1.6.1b1/src/robodyno/interfaces/
+-rw-rw-rw-   0        0        0      533 2023-05-18 03:40:10.000000 robodyno-1.6.1b1/src/robodyno/interfaces/__init__.py
+-rw-rw-rw-   0        0        0     9768 2023-05-19 05:14:39.000000 robodyno-1.6.1b1/src/robodyno/interfaces/can_bus.py
+-rw-rw-rw-   0        0        0     3069 2023-05-16 05:58:37.000000 robodyno-1.6.1b1/src/robodyno/interfaces/webots.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:30:52.840377 robodyno-1.6.1b1/src/robodyno/robots/
+-rw-rw-rw-   0        0        0      309 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/robots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:30:52.842377 robodyno-1.6.1b1/src/robodyno/robots/four_dof_palletizing_robot/
+-rw-rw-rw-   0        0        0       50 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/robots/four_dof_palletizing_robot/__init__.py
+-rw-rw-rw-   0        0        0     7949 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/robots/four_dof_palletizing_robot/four_dof_pallet_robot.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:30:52.844890 robodyno-1.6.1b1/src/robodyno/robots/four_dof_scara_robot/
+-rw-rw-rw-   0        0        0       46 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/robots/four_dof_scara_robot/__init__.py
+-rw-rw-rw-   0        0        0     8412 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/robots/four_dof_scara_robot/four_dof_scara_robot.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:30:52.846891 robodyno-1.6.1b1/src/robodyno/robots/six_dof_collaborative_robot/
+-rw-rw-rw-   0        0        0       51 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/robots/six_dof_collaborative_robot/__init__.py
+-rw-rw-rw-   0        0        0    10624 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/robots/six_dof_collaborative_robot/six_dof_collab_robot.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:30:52.848893 robodyno-1.6.1b1/src/robodyno/robots/three_dof_delta_robot/
+-rw-rw-rw-   0        0        0       48 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/robots/three_dof_delta_robot/__init__.py
+-rw-rw-rw-   0        0        0     9792 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/robots/three_dof_delta_robot/three_dof_delta_robot.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:30:52.850889 robodyno-1.6.1b1/src/robodyno/robots/three_dof_palletizing_robot/
+-rw-rw-rw-   0        0        0       50 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/robots/three_dof_palletizing_robot/__init__.py
+-rw-rw-rw-   0        0        0     7512 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/robots/three_dof_palletizing_robot/three_dof_pallet_robot.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:30:52.853889 robodyno-1.6.1b1/src/robodyno/robots/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/robots/utils/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-05-05 06:04:00.000000 robodyno-1.6.1b1/src/robodyno/robots/utils/interpolations.py
+-rw-rw-rw-   0        0        0    59522 2023-05-19 05:16:51.000000 robodyno-1.6.1b1/src/robodyno/robots/utils/transformations.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:30:52.859893 robodyno-1.6.1b1/src/robodyno/tools/
+-rw-rw-rw-   0        0        0        0 2023-05-18 09:35:59.000000 robodyno-1.6.1b1/src/robodyno/tools/__init__.py
+-rw-rw-rw-   0        0        0     4183 2023-05-18 04:13:40.000000 robodyno-1.6.1b1/src/robodyno/tools/can_bus_monitor.py
+-rw-rw-rw-   0        0        0    16396 2023-05-19 05:11:28.000000 robodyno-1.6.1b1/src/robodyno/tools/cli.py
+-rw-rw-rw-   0        0        0     3407 2023-05-19 03:16:35.000000 robodyno-1.6.1b1/src/robodyno/tools/cli_param_types.py
+-rw-rw-rw-   0        0        0     3992 2023-05-18 07:23:21.000000 robodyno-1.6.1b1/src/robodyno/tools/motor_info_table.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:30:52.817365 robodyno-1.6.1b1/src/robodyno.egg-info/
+-rw-rw-rw-   0        0        0    11028 2023-05-22 07:30:52.000000 robodyno-1.6.1b1/src/robodyno.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2202 2023-05-22 07:30:52.000000 robodyno-1.6.1b1/src/robodyno.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 07:30:52.000000 robodyno-1.6.1b1/src/robodyno.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1039 2023-05-22 07:30:52.000000 robodyno-1.6.1b1/src/robodyno.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      121 2023-05-22 07:30:52.000000 robodyno-1.6.1b1/src/robodyno.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 07:30:52.000000 robodyno-1.6.1b1/src/robodyno.egg-info/top_level.txt
```

### Comparing `robodyno-1.6.1b0/PKG-INFO` & `robodyno-1.6.1b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robodyno
-Version: 1.6.1b0
+Version: 1.6.1b1
 Summary: The Robodyno Robot SDK for Python 3
 Home-page: http://101.42.250.169/
 Author: song
 Author-email: zhaosongy@126.com
 Maintainer: robottime
 Maintainer-email: lab@robottime.cn
 License: MIT License
```

### Comparing `robodyno-1.6.1b0/setup.py` & `robodyno-1.6.1b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     mode='r',
     encoding='utf-8',
 ) as f:
     long_description = f.read()
 
 setup(
     name='robodyno',
-    version='1.6.1-beta',
+    version=__version__,
     maintainer='robottime',
     maintainer_email='lab@robottime.cn',
     author='song',
     author_email='zhaosongy@126.com',
     description='The Robodyno Robot SDK for Python 3',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `robodyno-1.6.1b0/src/robodyno/__init__.py` & `robodyno-1.6.1b1/src/robodyno/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,23 +18,10 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-"""Reads the version from the CHANGELOG.md file."""
+"""Version information for Robodyno package."""
 
-import os
-import re
-
-with open(
-    os.path.join(os.path.dirname(__file__), '..', '..', 'CHANGELOG.md'),
-    mode='r',
-    encoding='utf-8',
-) as f:
-    for line in f:
-        if line.startswith('##'):
-            match = re.search(r'\d+\.\d+\.\d+', line)
-            if match:
-                __version__ = match.group(0)
-                break
+__version__ = '1.6.1-beta1'
```

### Comparing `robodyno-1.6.1b0/src/robodyno/components/__init__.py` & `robodyno-1.6.1b1/src/robodyno/components/__init__.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/components/can_bus/can_bus_device.py` & `robodyno-1.6.1b1/src/robodyno/components/can_bus/can_bus_device.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/components/can_bus/imu_sensor.py` & `robodyno-1.6.1b1/src/robodyno/components/can_bus/imu_sensor.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/components/can_bus/motor.py` & `robodyno-1.6.1b1/src/robodyno/components/can_bus/motor.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/components/can_bus/pwm_driver.py` & `robodyno-1.6.1b1/src/robodyno/components/can_bus/pwm_driver.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/components/can_bus/slider_module.py` & `robodyno-1.6.1b1/src/robodyno/components/can_bus/slider_module.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/components/can_bus/stepper_driver.py` & `robodyno-1.6.1b1/src/robodyno/components/can_bus/stepper_driver.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/components/config/model.py` & `robodyno-1.6.1b1/src/robodyno/components/config/model.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/components/config/robottime_config.py` & `robodyno-1.6.1b1/src/robodyno/components/config/robottime_config.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/components/webots/motor.py` & `robodyno-1.6.1b1/src/robodyno/components/webots/motor.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/components/webots/slider_module.py` & `robodyno-1.6.1b1/src/robodyno/components/webots/slider_module.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/components/webots/webots_device.py` & `robodyno-1.6.1b1/src/robodyno/components/webots/webots_device.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/interfaces/__init__.py` & `robodyno-1.6.1b1/src/robodyno/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/interfaces/can_bus.py` & `robodyno-1.6.1b1/src/robodyno/interfaces/can_bus.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/interfaces/webots.py` & `robodyno-1.6.1b1/src/robodyno/interfaces/webots.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/robots/four_dof_palletizing_robot/four_dof_pallet_robot.py` & `robodyno-1.6.1b1/src/robodyno/robots/four_dof_palletizing_robot/four_dof_pallet_robot.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/robots/four_dof_scara_robot/four_dof_scara_robot.py` & `robodyno-1.6.1b1/src/robodyno/robots/four_dof_scara_robot/four_dof_scara_robot.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/robots/six_dof_collaborative_robot/six_dof_collab_robot.py` & `robodyno-1.6.1b1/src/robodyno/robots/six_dof_collaborative_robot/six_dof_collab_robot.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/robots/three_dof_delta_robot/three_dof_delta_robot.py` & `robodyno-1.6.1b1/src/robodyno/robots/three_dof_delta_robot/three_dof_delta_robot.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/robots/three_dof_palletizing_robot/three_dof_pallet_robot.py` & `robodyno-1.6.1b1/src/robodyno/robots/three_dof_palletizing_robot/three_dof_pallet_robot.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/robots/utils/interpolations.py` & `robodyno-1.6.1b1/src/robodyno/robots/utils/interpolations.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/robots/utils/transformations.py` & `robodyno-1.6.1b1/src/robodyno/robots/utils/transformations.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/tools/can_bus_monitor.py` & `robodyno-1.6.1b1/src/robodyno/tools/can_bus_monitor.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/tools/cli.py` & `robodyno-1.6.1b1/src/robodyno/tools/cli.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/tools/cli_param_types.py` & `robodyno-1.6.1b1/src/robodyno/tools/cli_param_types.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno/tools/motor_info_table.py` & `robodyno-1.6.1b1/src/robodyno/tools/motor_info_table.py`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno.egg-info/PKG-INFO` & `robodyno-1.6.1b1/src/robodyno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robodyno
-Version: 1.6.1b0
+Version: 1.6.1b1
 Summary: The Robodyno Robot SDK for Python 3
 Home-page: http://101.42.250.169/
 Author: song
 Author-email: zhaosongy@126.com
 Maintainer: robottime
 Maintainer-email: lab@robottime.cn
 License: MIT License
```

### Comparing `robodyno-1.6.1b0/src/robodyno.egg-info/SOURCES.txt` & `robodyno-1.6.1b1/src/robodyno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robodyno-1.6.1b0/src/robodyno.egg-info/entry_points.txt` & `robodyno-1.6.1b1/src/robodyno.egg-info/entry_points.txt`

 * *Files identical despite different names*

