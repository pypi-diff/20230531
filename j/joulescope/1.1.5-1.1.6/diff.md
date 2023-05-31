# Comparing `tmp/joulescope-1.1.5.tar.gz` & `tmp/joulescope-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joulescope-1.1.5.tar", last modified: Wed May 24 19:33:40 2023, max compression
+gzip compressed data, was "joulescope-1.1.6.tar", last modified: Wed May 31 12:18:21 2023, max compression
```

## Comparing `joulescope-1.1.5.tar` & `joulescope-1.1.6.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.876642 joulescope-1.1.5/
--rw-rw-rw-   0        0        0    21821 2023-05-24 14:34:53.000000 joulescope-1.1.5/CHANGELOG.md
--rw-rw-rw-   0        0        0     6771 2020-08-11 21:29:57.000000 joulescope-1.1.5/CREDITS.html
--rw-rw-rw-   0        0        0    11558 2020-05-30 15:27:09.000000 joulescope-1.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0      132 2022-11-07 18:35:15.000000 joulescope-1.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3628 2023-05-24 19:33:40.876642 joulescope-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1762 2020-11-25 13:12:14.000000 joulescope-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.816069 joulescope-1.1.5/joulescope/
--rw-rw-rw-   0        0        0     2291 2023-03-20 19:38:30.000000 joulescope-1.1.5/joulescope/__init__.py
--rw-rw-rw-   0        0        0      730 2020-05-30 15:27:09.000000 joulescope-1.1.5/joulescope/__main__.py
--rw-rw-rw-   0        0        0    54968 2023-03-11 15:21:25.000000 joulescope-1.1.5/joulescope/data_recorder.py
--rw-rw-rw-   0        0        0    26397 2022-09-09 13:37:25.000000 joulescope-1.1.5/joulescope/datafile.py
-drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.852582 joulescope-1.1.5/joulescope/entry_points/
--rw-rw-rw-   0        0        0        0 2020-05-30 15:27:09.000000 joulescope-1.1.5/joulescope/entry_points/__init__.py
--rw-rw-rw-   0        0        0     1325 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/entry_points/bootloader_go.py
--rw-rw-rw-   0        0        0     4040 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/entry_points/capture.py
--rw-rw-rw-   0        0        0     1530 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/entry_points/gpo_demo.py
--rw-rw-rw-   0        0        0     2103 2023-04-19 20:18:48.000000 joulescope-1.1.5/joulescope/entry_points/info.py
--rw-rw-rw-   0        0        0     2110 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/entry_points/parameter_set.py
--rw-rw-rw-   0        0        0     5043 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/entry_points/program.py
--rw-rw-rw-   0        0        0     6546 2022-09-10 13:15:16.000000 joulescope-1.1.5/joulescope/entry_points/recording.py
--rw-rw-rw-   0        0        0     3609 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/entry_points/runner.py
--rw-rw-rw-   0        0        0      865 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/entry_points/scan.py
--rw-rw-rw-   0        0        0     2883 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/entry_points/statistics.py
--rw-rw-rw-   0        0        0     2814 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/entry_points/stream_test.py
--rw-rw-rw-   0        0        0     3000 2020-05-30 15:27:09.000000 joulescope-1.1.5/joulescope/file_replace.py
--rw-rw-rw-   0        0        0     5532 2023-02-22 12:49:19.000000 joulescope-1.1.5/joulescope/jls_v2_writer.py
--rw-rw-rw-   0        0        0     3056 2022-09-09 13:37:25.000000 joulescope-1.1.5/joulescope/parameter.py
--rw-rw-rw-   0        0        0    11070 2022-11-07 22:01:01.000000 joulescope-1.1.5/joulescope/parameters_v1.py
--rw-rw-rw-   0        0        0     8797 2022-12-20 13:24:03.000000 joulescope-1.1.5/joulescope/span.py
--rw-rw-rw-   0        0        0      653 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/stream_buffer.py
-drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.856091 joulescope-1.1.5/joulescope/test/
--rw-rw-rw-   0        0        0        0 2020-05-30 15:27:09.000000 joulescope-1.1.5/joulescope/test/__init__.py
--rw-rw-rw-   0        0        0    16330 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/test/test_data_recorder.py
--rw-rw-rw-   0        0        0     5407 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/test/test_data_recorder_downsampled.py
--rw-rw-rw-   0        0        0     2484 2020-05-30 15:27:09.000000 joulescope-1.1.5/joulescope/test/test_file_replace.py
--rw-rw-rw-   0        0        0     4237 2022-11-21 18:21:24.000000 joulescope-1.1.5/joulescope/test/test_jls_v2_writer.py
--rw-rw-rw-   0        0        0     2902 2021-03-09 14:36:24.000000 joulescope-1.1.5/joulescope/test/test_span.py
--rw-rw-rw-   0        0        0     1179 2020-05-30 15:27:09.000000 joulescope-1.1.5/joulescope/test/test_time.py
--rw-rw-rw-   0        0        0     4631 2021-11-19 14:35:42.000000 joulescope-1.1.5/joulescope/test/test_units.py
--rw-rw-rw-   0        0        0    10876 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/test_datafile.py
--rw-rw-rw-   0        0        0     2189 2020-05-30 15:27:09.000000 joulescope-1.1.5/joulescope/time.py
--rw-rw-rw-   0        0        0     4736 2021-11-19 14:35:42.000000 joulescope-1.1.5/joulescope/units.py
-drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.859599 joulescope-1.1.5/joulescope/v0/
--rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/__init__.py
--rw-rw-rw-   0        0        0     6362 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/array_storage.py
--rw-rw-rw-   0        0        0    12568 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/bootloader.py
--rw-rw-rw-   0        0        0     9922 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/calibration.py
--rw-rw-rw-   0        0        0    85576 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/decimators.py
--rw-rw-rw-   0        0        0    58006 2023-03-20 19:36:21.000000 joulescope-1.1.5/joulescope/v0/driver.py
--rw-rw-rw-   0        0        0   957021 2023-04-26 20:01:19.000000 joulescope-1.1.5/joulescope/v0/filter_fir.c
--rw-rw-rw-   0        0        0     6132 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/firmware_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.860599 joulescope-1.1.5/joulescope/v0/native/
--rw-rw-rw-   0        0        0     3763 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/native/filter_fir.c
--rw-rw-rw-   0        0        0     2904 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/native/filter_fir.h
--rw-rw-rw-   0        0        0     2647 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/native/running_statistics.c
--rw-rw-rw-   0        0        0     2891 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/native/running_statistics.h
-drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.862103 joulescope-1.1.5/joulescope/v0/native/test/
--rw-rw-rw-   0        0        0    57119 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/native/test/acutest.h
--rw-rw-rw-   0        0        0     2942 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/native/test/test_filter_fir.c
--rw-rw-rw-   0        0        0     1913 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/notification_handler.py
--rw-rw-rw-   0        0        0   433682 2023-04-26 20:01:19.000000 joulescope-1.1.5/joulescope/v0/pattern_buffer.c
--rw-rw-rw-   0        0        0     1245 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/public_keys.py
--rw-rw-rw-   0        0        0  2675267 2023-04-26 20:01:20.000000 joulescope-1.1.5/joulescope/v0/stream_buffer.c
-drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.866613 joulescope-1.1.5/joulescope/v0/test/
--rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/test/__init__.py
--rw-rw-rw-   0        0        0     2999 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/test/test_array_storage.py
--rw-rw-rw-   0        0        0     3717 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/test/test_calibration.py
--rw-rw-rw-   0        0        0     4551 2023-03-10 18:03:29.000000 joulescope-1.1.5/joulescope/v0/test/test_device.py
--rw-rw-rw-   0        0        0     2308 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/test/test_filter_fir.py
--rw-rw-rw-   0        0        0     1418 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/test/test_parameter.py
--rw-rw-rw-   0        0        0     3379 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/test/test_pattern_buffer.py
--rw-rw-rw-   0        0        0     3670 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/test/test_stats.py
--rw-rw-rw-   0        0        0    24677 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/test/test_stream_buffer.py
--rw-rw-rw-   0        0        0     1793 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/test/test_view.py
-drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.869116 joulescope-1.1.5/joulescope/v0/usb/
--rw-rw-rw-   0        0        0      758 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/__init__.py
--rw-rw-rw-   0        0        0     8886 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/api.py
--rw-rw-rw-   0        0        0     5114 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/core.py
--rw-rw-rw-   0        0        0     8111 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/device_thread.py
--rw-rw-rw-   0        0        0     4046 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/hw_tests.py
--rw-rw-rw-   0        0        0     1542 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/impl_tools.py
-drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.870122 joulescope-1.1.5/joulescope/v0/usb/libusb/
--rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/libusb/__init__.py
--rw-rw-rw-   0        0        0    40907 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/libusb/device.py
--rw-rw-rw-   0        0        0     2406 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/scan_info.py
-drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.872626 joulescope-1.1.5/joulescope/v0/usb/winusb/
--rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/winusb/__init__.py
--rw-rw-rw-   0        0        0    35453 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/winusb/device.py
--rw-rw-rw-   0        0        0     8061 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/winusb/kernel32.py
--rw-rw-rw-   0        0        0     6017 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/winusb/setupapi.py
--rw-rw-rw-   0        0        0     5280 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v0/usb/winusb/win32_device_notify.py
-drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.875643 joulescope-1.1.5/joulescope/v1/
--rw-rw-rw-   0        0        0      690 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v1/__init__.py
--rw-rw-rw-   0        0        0    28495 2023-05-24 15:39:07.000000 joulescope-1.1.5/joulescope/v1/device.py
--rw-rw-rw-   0        0        0     7317 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v1/driver.py
--rw-rw-rw-   0        0        0     5627 2023-04-19 20:18:51.000000 joulescope-1.1.5/joulescope/v1/js110.py
--rw-rw-rw-   0        0        0     7534 2023-01-25 15:11:30.000000 joulescope-1.1.5/joulescope/v1/js220.py
--rw-rw-rw-   0        0        0     6630 2023-02-15 17:15:30.000000 joulescope-1.1.5/joulescope/v1/sample_buffer.py
--rw-rw-rw-   0        0        0   888760 2023-04-26 20:01:21.000000 joulescope-1.1.5/joulescope/v1/stats.c
--rw-rw-rw-   0        0        0    16328 2023-04-12 13:39:59.000000 joulescope-1.1.5/joulescope/v1/stream_buffer.py
-drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.876642 joulescope-1.1.5/joulescope/v1/test/
--rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.5/joulescope/v1/test/__init__.py
--rw-rw-rw-   0        0        0     3047 2022-11-10 15:29:05.000000 joulescope-1.1.5/joulescope/v1/test/test_sample_buffer.py
--rw-rw-rw-   0        0        0      470 2023-05-24 14:34:59.000000 joulescope-1.1.5/joulescope/version.py
--rw-rw-rw-   0        0        0    21187 2022-11-11 15:21:00.000000 joulescope-1.1.5/joulescope/view.py
-drwxrwxrwx   0        0        0        0 2023-05-24 19:33:40.829095 joulescope-1.1.5/joulescope.egg-info/
--rw-rw-rw-   0        0        0     3628 2023-05-24 19:33:40.000000 joulescope-1.1.5/joulescope.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3265 2023-05-24 19:33:40.000000 joulescope-1.1.5/joulescope.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 19:33:40.000000 joulescope-1.1.5/joulescope.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-05-24 19:33:40.000000 joulescope-1.1.5/joulescope.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      201 2023-05-24 19:33:40.000000 joulescope-1.1.5/joulescope.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-24 19:33:40.000000 joulescope-1.1.5/joulescope.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      851 2022-11-30 15:24:46.000000 joulescope-1.1.5/pyproject.toml
--rw-rw-rw-   0        0        0      117 2023-05-24 19:33:40.884675 joulescope-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     6883 2023-05-24 14:34:05.000000 joulescope-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:18:21.722723 joulescope-1.1.6/
+-rw-rw-rw-   0        0        0    21884 2023-05-31 11:51:23.000000 joulescope-1.1.6/CHANGELOG.md
+-rw-rw-rw-   0        0        0     6771 2020-08-11 21:29:57.000000 joulescope-1.1.6/CREDITS.html
+-rw-rw-rw-   0        0        0    11558 2020-05-30 15:27:09.000000 joulescope-1.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      132 2022-11-07 18:35:15.000000 joulescope-1.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3628 2023-05-31 12:18:21.722723 joulescope-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1762 2020-11-25 13:12:14.000000 joulescope-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 12:18:21.685174 joulescope-1.1.6/joulescope/
+-rw-rw-rw-   0        0        0     2291 2023-03-20 19:38:30.000000 joulescope-1.1.6/joulescope/__init__.py
+-rw-rw-rw-   0        0        0      730 2020-05-30 15:27:09.000000 joulescope-1.1.6/joulescope/__main__.py
+-rw-rw-rw-   0        0        0    54968 2023-03-11 15:21:25.000000 joulescope-1.1.6/joulescope/data_recorder.py
+-rw-rw-rw-   0        0        0    26397 2022-09-09 13:37:25.000000 joulescope-1.1.6/joulescope/datafile.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:18:21.699204 joulescope-1.1.6/joulescope/entry_points/
+-rw-rw-rw-   0        0        0        0 2020-05-30 15:27:09.000000 joulescope-1.1.6/joulescope/entry_points/__init__.py
+-rw-rw-rw-   0        0        0     1325 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/entry_points/bootloader_go.py
+-rw-rw-rw-   0        0        0     4040 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/entry_points/capture.py
+-rw-rw-rw-   0        0        0     1530 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/entry_points/gpo_demo.py
+-rw-rw-rw-   0        0        0     2103 2023-04-19 20:18:48.000000 joulescope-1.1.6/joulescope/entry_points/info.py
+-rw-rw-rw-   0        0        0     2110 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/entry_points/parameter_set.py
+-rw-rw-rw-   0        0        0     5043 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/entry_points/program.py
+-rw-rw-rw-   0        0        0     6546 2022-09-10 13:15:16.000000 joulescope-1.1.6/joulescope/entry_points/recording.py
+-rw-rw-rw-   0        0        0     3609 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/entry_points/runner.py
+-rw-rw-rw-   0        0        0      865 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/entry_points/scan.py
+-rw-rw-rw-   0        0        0     2883 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/entry_points/statistics.py
+-rw-rw-rw-   0        0        0     2814 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/entry_points/stream_test.py
+-rw-rw-rw-   0        0        0     3000 2020-05-30 15:27:09.000000 joulescope-1.1.6/joulescope/file_replace.py
+-rw-rw-rw-   0        0        0     5532 2023-02-22 12:49:19.000000 joulescope-1.1.6/joulescope/jls_v2_writer.py
+-rw-rw-rw-   0        0        0     3056 2022-09-09 13:37:25.000000 joulescope-1.1.6/joulescope/parameter.py
+-rw-rw-rw-   0        0        0    11070 2022-11-07 22:01:01.000000 joulescope-1.1.6/joulescope/parameters_v1.py
+-rw-rw-rw-   0        0        0     8797 2022-12-20 13:24:03.000000 joulescope-1.1.6/joulescope/span.py
+-rw-rw-rw-   0        0        0      653 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/stream_buffer.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:18:21.703203 joulescope-1.1.6/joulescope/test/
+-rw-rw-rw-   0        0        0        0 2020-05-30 15:27:09.000000 joulescope-1.1.6/joulescope/test/__init__.py
+-rw-rw-rw-   0        0        0    16330 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/test/test_data_recorder.py
+-rw-rw-rw-   0        0        0     5407 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/test/test_data_recorder_downsampled.py
+-rw-rw-rw-   0        0        0     2484 2020-05-30 15:27:09.000000 joulescope-1.1.6/joulescope/test/test_file_replace.py
+-rw-rw-rw-   0        0        0     4237 2022-11-21 18:21:24.000000 joulescope-1.1.6/joulescope/test/test_jls_v2_writer.py
+-rw-rw-rw-   0        0        0     2902 2021-03-09 14:36:24.000000 joulescope-1.1.6/joulescope/test/test_span.py
+-rw-rw-rw-   0        0        0     1179 2020-05-30 15:27:09.000000 joulescope-1.1.6/joulescope/test/test_time.py
+-rw-rw-rw-   0        0        0     4631 2021-11-19 14:35:42.000000 joulescope-1.1.6/joulescope/test/test_units.py
+-rw-rw-rw-   0        0        0    10876 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/test_datafile.py
+-rw-rw-rw-   0        0        0     2189 2020-05-30 15:27:09.000000 joulescope-1.1.6/joulescope/time.py
+-rw-rw-rw-   0        0        0     4736 2021-11-19 14:35:42.000000 joulescope-1.1.6/joulescope/units.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:18:21.707218 joulescope-1.1.6/joulescope/v0/
+-rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/__init__.py
+-rw-rw-rw-   0        0        0     6362 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/array_storage.py
+-rw-rw-rw-   0        0        0    12568 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/bootloader.py
+-rw-rw-rw-   0        0        0     9922 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/calibration.py
+-rw-rw-rw-   0        0        0    85576 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/decimators.py
+-rw-rw-rw-   0        0        0    58006 2023-03-20 19:36:21.000000 joulescope-1.1.6/joulescope/v0/driver.py
+-rw-rw-rw-   0        0        0   957868 2023-05-31 12:05:24.000000 joulescope-1.1.6/joulescope/v0/filter_fir.c
+-rw-rw-rw-   0        0        0     6132 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/firmware_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:18:21.708217 joulescope-1.1.6/joulescope/v0/native/
+-rw-rw-rw-   0        0        0     3763 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/native/filter_fir.c
+-rw-rw-rw-   0        0        0     2904 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/native/filter_fir.h
+-rw-rw-rw-   0        0        0     2647 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/native/running_statistics.c
+-rw-rw-rw-   0        0        0     2891 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/native/running_statistics.h
+drwxrwxrwx   0        0        0        0 2023-05-31 12:18:21.709217 joulescope-1.1.6/joulescope/v0/native/test/
+-rw-rw-rw-   0        0        0    57119 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/native/test/acutest.h
+-rw-rw-rw-   0        0        0     2942 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/native/test/test_filter_fir.c
+-rw-rw-rw-   0        0        0     1913 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/notification_handler.py
+-rw-rw-rw-   0        0        0   434405 2023-05-31 12:05:25.000000 joulescope-1.1.6/joulescope/v0/pattern_buffer.c
+-rw-rw-rw-   0        0        0     1245 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/public_keys.py
+-rw-rw-rw-   0        0        0  2676551 2023-05-31 12:05:25.000000 joulescope-1.1.6/joulescope/v0/stream_buffer.c
+drwxrwxrwx   0        0        0        0 2023-05-31 12:18:21.713217 joulescope-1.1.6/joulescope/v0/test/
+-rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/test/__init__.py
+-rw-rw-rw-   0        0        0     2999 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/test/test_array_storage.py
+-rw-rw-rw-   0        0        0     3717 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/test/test_calibration.py
+-rw-rw-rw-   0        0        0     4551 2023-03-10 18:03:29.000000 joulescope-1.1.6/joulescope/v0/test/test_device.py
+-rw-rw-rw-   0        0        0     2308 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/test/test_filter_fir.py
+-rw-rw-rw-   0        0        0     1418 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/test/test_parameter.py
+-rw-rw-rw-   0        0        0     3379 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/test/test_pattern_buffer.py
+-rw-rw-rw-   0        0        0     3670 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/test/test_stats.py
+-rw-rw-rw-   0        0        0    24677 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/test/test_stream_buffer.py
+-rw-rw-rw-   0        0        0     1793 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/test/test_view.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:18:21.716218 joulescope-1.1.6/joulescope/v0/usb/
+-rw-rw-rw-   0        0        0      758 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/usb/__init__.py
+-rw-rw-rw-   0        0        0     8886 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/usb/api.py
+-rw-rw-rw-   0        0        0     5114 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/usb/core.py
+-rw-rw-rw-   0        0        0     8111 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/usb/device_thread.py
+-rw-rw-rw-   0        0        0     4046 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/usb/hw_tests.py
+-rw-rw-rw-   0        0        0     1542 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/usb/impl_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:18:21.716720 joulescope-1.1.6/joulescope/v0/usb/libusb/
+-rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/usb/libusb/__init__.py
+-rw-rw-rw-   0        0        0    40907 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/usb/libusb/device.py
+-rw-rw-rw-   0        0        0     2406 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/usb/scan_info.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:18:21.718723 joulescope-1.1.6/joulescope/v0/usb/winusb/
+-rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/usb/winusb/__init__.py
+-rw-rw-rw-   0        0        0    35453 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/usb/winusb/device.py
+-rw-rw-rw-   0        0        0     8061 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/usb/winusb/kernel32.py
+-rw-rw-rw-   0        0        0     6017 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/usb/winusb/setupapi.py
+-rw-rw-rw-   0        0        0     5280 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v0/usb/winusb/win32_device_notify.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:18:21.721723 joulescope-1.1.6/joulescope/v1/
+-rw-rw-rw-   0        0        0      690 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v1/__init__.py
+-rw-rw-rw-   0        0        0    28495 2023-05-24 15:39:07.000000 joulescope-1.1.6/joulescope/v1/device.py
+-rw-rw-rw-   0        0        0     7317 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v1/driver.py
+-rw-rw-rw-   0        0        0     5627 2023-04-19 20:18:51.000000 joulescope-1.1.6/joulescope/v1/js110.py
+-rw-rw-rw-   0        0        0     7534 2023-01-25 15:11:30.000000 joulescope-1.1.6/joulescope/v1/js220.py
+-rw-rw-rw-   0        0        0     6630 2023-02-15 17:15:30.000000 joulescope-1.1.6/joulescope/v1/sample_buffer.py
+-rw-rw-rw-   0        0        0   889576 2023-05-31 12:05:26.000000 joulescope-1.1.6/joulescope/v1/stats.c
+-rw-rw-rw-   0        0        0    16328 2023-04-12 13:39:59.000000 joulescope-1.1.6/joulescope/v1/stream_buffer.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:18:21.722723 joulescope-1.1.6/joulescope/v1/test/
+-rw-rw-rw-   0        0        0        0 2022-10-30 18:42:53.000000 joulescope-1.1.6/joulescope/v1/test/__init__.py
+-rw-rw-rw-   0        0        0     3047 2022-11-10 15:29:05.000000 joulescope-1.1.6/joulescope/v1/test/test_sample_buffer.py
+-rw-rw-rw-   0        0        0      470 2023-05-31 11:51:37.000000 joulescope-1.1.6/joulescope/version.py
+-rw-rw-rw-   0        0        0    21187 2022-11-11 15:21:00.000000 joulescope-1.1.6/joulescope/view.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:18:21.688683 joulescope-1.1.6/joulescope.egg-info/
+-rw-rw-rw-   0        0        0     3628 2023-05-31 12:18:21.000000 joulescope-1.1.6/joulescope.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3265 2023-05-31 12:18:21.000000 joulescope-1.1.6/joulescope.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 12:18:21.000000 joulescope-1.1.6/joulescope.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-31 12:18:21.000000 joulescope-1.1.6/joulescope.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      201 2023-05-31 12:18:21.000000 joulescope-1.1.6/joulescope.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-31 12:18:21.000000 joulescope-1.1.6/joulescope.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      851 2022-11-30 15:24:46.000000 joulescope-1.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0      117 2023-05-31 12:18:21.723723 joulescope-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     6883 2023-05-31 11:51:01.000000 joulescope-1.1.6/setup.py
```

### Comparing `joulescope-1.1.5/CHANGELOG.md` & `joulescope-1.1.6/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to pyjoulescope.
 
 
+## 1.1.6
+
+2023 May 31
+
+* Bumped dependency revisions.
+
+
 ## 1.1.5
 
 2023 May 24
 
 * Added JS110 on-instrument (sensor) statistics option to v1 backend.
```

### Comparing `joulescope-1.1.5/CREDITS.html` & `joulescope-1.1.6/CREDITS.html`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/LICENSE.txt` & `joulescope-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/PKG-INFO` & `joulescope-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope
-Version: 1.1.5
+Version: 1.1.6
 Summary: Joulescope™ host driver and utilities
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope-1.1.5/README.md` & `joulescope-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/__init__.py` & `joulescope-1.1.6/joulescope/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/__main__.py` & `joulescope-1.1.6/joulescope/__main__.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/data_recorder.py` & `joulescope-1.1.6/joulescope/data_recorder.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/datafile.py` & `joulescope-1.1.6/joulescope/datafile.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/entry_points/bootloader_go.py` & `joulescope-1.1.6/joulescope/entry_points/bootloader_go.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/entry_points/capture.py` & `joulescope-1.1.6/joulescope/entry_points/capture.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/entry_points/gpo_demo.py` & `joulescope-1.1.6/joulescope/entry_points/gpo_demo.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/entry_points/info.py` & `joulescope-1.1.6/joulescope/entry_points/info.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/entry_points/parameter_set.py` & `joulescope-1.1.6/joulescope/entry_points/parameter_set.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/entry_points/program.py` & `joulescope-1.1.6/joulescope/entry_points/program.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/entry_points/recording.py` & `joulescope-1.1.6/joulescope/entry_points/recording.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/entry_points/runner.py` & `joulescope-1.1.6/joulescope/entry_points/runner.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/entry_points/scan.py` & `joulescope-1.1.6/joulescope/entry_points/scan.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/entry_points/statistics.py` & `joulescope-1.1.6/joulescope/entry_points/statistics.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/entry_points/stream_test.py` & `joulescope-1.1.6/joulescope/entry_points/stream_test.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/file_replace.py` & `joulescope-1.1.6/joulescope/file_replace.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/jls_v2_writer.py` & `joulescope-1.1.6/joulescope/jls_v2_writer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/parameter.py` & `joulescope-1.1.6/joulescope/parameter.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/parameters_v1.py` & `joulescope-1.1.6/joulescope/parameters_v1.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/span.py` & `joulescope-1.1.6/joulescope/span.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/stream_buffer.py` & `joulescope-1.1.6/joulescope/stream_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/test/test_data_recorder.py` & `joulescope-1.1.6/joulescope/test/test_data_recorder.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/test/test_data_recorder_downsampled.py` & `joulescope-1.1.6/joulescope/test/test_data_recorder_downsampled.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/test/test_file_replace.py` & `joulescope-1.1.6/joulescope/test/test_file_replace.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/test/test_jls_v2_writer.py` & `joulescope-1.1.6/joulescope/test/test_jls_v2_writer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/test/test_span.py` & `joulescope-1.1.6/joulescope/test/test_span.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/test/test_time.py` & `joulescope-1.1.6/joulescope/test/test_time.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/test/test_units.py` & `joulescope-1.1.6/joulescope/test/test_units.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/test_datafile.py` & `joulescope-1.1.6/joulescope/test_datafile.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/time.py` & `joulescope-1.1.6/joulescope/time.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/units.py` & `joulescope-1.1.6/joulescope/units.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/array_storage.py` & `joulescope-1.1.6/joulescope/v0/array_storage.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/bootloader.py` & `joulescope-1.1.6/joulescope/v0/bootloader.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/calibration.py` & `joulescope-1.1.6/joulescope/v0/calibration.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/decimators.py` & `joulescope-1.1.6/joulescope/v0/decimators.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/driver.py` & `joulescope-1.1.6/joulescope/v0/driver.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/filter_fir.c` & `joulescope-1.1.6/joulescope/v0/filter_fir.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "C:\\bin\\Python3_11_3\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
             "C:\\bin\\Python3_11_3\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
@@ -30,16 +30,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -99,16 +99,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -2120,30 +2124,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -18611,15 +18615,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_array_obj *p;
@@ -18803,15 +18807,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -18925,15 +18929,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -19189,15 +19193,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -19338,15 +19342,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -19975,70 +19979,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -22901,18 +22874,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -22958,22 +22931,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -24562,15 +24535,15 @@
                         } else if (8 * sizeof(uint32_t) >= 4 * PyLong_SHIFT) {
                             return (uint32_t) (((((((((uint32_t)digits[3]) << PyLong_SHIFT) | (uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -24834,15 +24807,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -25030,15 +25003,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -25264,15 +25237,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `joulescope-1.1.5/joulescope/v0/firmware_manager.py` & `joulescope-1.1.6/joulescope/v0/firmware_manager.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/native/filter_fir.c` & `joulescope-1.1.6/joulescope/v0/native/filter_fir.c`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/native/filter_fir.h` & `joulescope-1.1.6/joulescope/v0/native/filter_fir.h`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/native/running_statistics.c` & `joulescope-1.1.6/joulescope/v0/native/running_statistics.c`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/native/running_statistics.h` & `joulescope-1.1.6/joulescope/v0/native/running_statistics.h`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/native/test/acutest.h` & `joulescope-1.1.6/joulescope/v0/native/test/acutest.h`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/native/test/test_filter_fir.c` & `joulescope-1.1.6/joulescope/v0/native/test/test_filter_fir.c`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/notification_handler.py` & `joulescope-1.1.6/joulescope/v0/notification_handler.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/pattern_buffer.c` & `joulescope-1.1.6/joulescope/v0/pattern_buffer.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "C:\\bin\\Python3_11_3\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
             "C:\\bin\\Python3_11_3\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
@@ -27,16 +27,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -96,16 +96,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1692,30 +1696,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -6100,15 +6104,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -6387,70 +6391,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -8718,18 +8691,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -8775,22 +8748,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -9538,15 +9511,15 @@
                         } else if (8 * sizeof(uint64_t) >= 4 * PyLong_SHIFT) {
                             return (uint64_t) (((((((((uint64_t)digits[3]) << PyLong_SHIFT) | (uint64_t)digits[2]) << PyLong_SHIFT) | (uint64_t)digits[1]) << PyLong_SHIFT) | (uint64_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -9810,15 +9783,15 @@
                         } else if (8 * sizeof(uint8_t) >= 4 * PyLong_SHIFT) {
                             return (uint8_t) (((((((((uint8_t)digits[3]) << PyLong_SHIFT) | (uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -10044,15 +10017,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -10278,15 +10251,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `joulescope-1.1.5/joulescope/v0/public_keys.py` & `joulescope-1.1.6/joulescope/v0/public_keys.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/stream_buffer.c` & `joulescope-1.1.6/joulescope/v0/stream_buffer.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "C:\\bin\\Python3_11_3\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
             "C:\\bin\\Python3_11_3\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
@@ -30,16 +30,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -99,16 +99,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -2689,30 +2693,30 @@
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -50515,15 +50519,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_10joulescope_2v0_13stream_buffer_RawProcessor __pyx_vtable_10joulescope_2v0_13stream_buffer_RawProcessor;
 
 static PyObject *__pyx_tp_new_10joulescope_2v0_13stream_buffer_RawProcessor(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_10joulescope_2v0_13stream_buffer_RawProcessor *p;
@@ -50680,15 +50684,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_10joulescope_2v0_13stream_buffer_Statistics __pyx_vtable_10joulescope_2v0_13stream_buffer_Statistics;
 
 static PyObject *__pyx_tp_new_10joulescope_2v0_13stream_buffer_Statistics(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_10joulescope_2v0_13stream_buffer_Statistics *p;
@@ -50837,15 +50841,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_10joulescope_2v0_13stream_buffer_UsbBulkProcessor __pyx_vtable_10joulescope_2v0_13stream_buffer_UsbBulkProcessor;
 
 static PyObject *__pyx_tp_new_10joulescope_2v0_13stream_buffer_UsbBulkProcessor(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_10joulescope_2v0_13stream_buffer_UsbBulkProcessor *p;
@@ -50975,15 +50979,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_10joulescope_2v0_13stream_buffer_StreamBuffer __pyx_vtable_10joulescope_2v0_13stream_buffer_StreamBuffer;
 
 static PyObject *__pyx_tp_new_10joulescope_2v0_13stream_buffer_StreamBuffer(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_10joulescope_2v0_13stream_buffer_StreamBuffer *p;
@@ -51312,15 +51316,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_10joulescope_2v0_13stream_buffer_DownsamplingStreamBuffer __pyx_vtable_10joulescope_2v0_13stream_buffer_DownsamplingStreamBuffer;
 
 static PyObject *__pyx_tp_new_10joulescope_2v0_13stream_buffer_DownsamplingStreamBuffer(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_10joulescope_2v0_13stream_buffer_DownsamplingStreamBuffer *p;
@@ -51600,15 +51604,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_10joulescope_2v0_13stream_buffer___pyx_scope_struct__samples_get *__pyx_freelist_10joulescope_2v0_13stream_buffer___pyx_scope_struct__samples_get[8];
 static int __pyx_freecount_10joulescope_2v0_13stream_buffer___pyx_scope_struct__samples_get = 0;
 
@@ -51739,15 +51743,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_array_obj *p;
@@ -51931,15 +51935,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -52053,15 +52057,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -52317,15 +52321,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -52466,15 +52470,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"usb_packet_factory_signal", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10joulescope_2v0_13stream_buffer_17usb_packet_factory_signal, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10joulescope_2v0_13stream_buffer_16usb_packet_factory_signal},
   {"single_stat_to_api", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10joulescope_2v0_13stream_buffer_19single_stat_to_api, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10joulescope_2v0_13stream_buffer_18single_stat_to_api},
@@ -53885,76 +53889,43 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(6, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(6, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(5, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(5, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(5, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(5, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(5, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(5, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(5, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(5, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(5, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(5, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(5, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(5, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(5, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(5, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(5, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(5, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(5, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(5, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(5, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(5, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(5, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(5, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(5, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(5, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(5, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(5, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(5, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(5, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(5, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(5, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("joulescope.v0.filter_fir"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10joulescope_2v0_10filter_fir_FilterFir = __Pyx_ImportType(__pyx_t_1, "joulescope.v0.filter_fir", "FilterFir", sizeof(struct __pyx_obj_10joulescope_2v0_10filter_fir_FilterFir), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_10joulescope_2v0_10filter_fir_FilterFir),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_10joulescope_2v0_10filter_fir_FilterFir) __PYX_ERR(7, 20, __pyx_L1_error)
+  __pyx_ptype_10joulescope_2v0_10filter_fir_FilterFir = __Pyx_ImportType_0_29_35(__pyx_t_1, "joulescope.v0.filter_fir", "FilterFir", sizeof(struct __pyx_obj_10joulescope_2v0_10filter_fir_FilterFir), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10joulescope_2v0_10filter_fir_FilterFir),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10joulescope_2v0_10filter_fir_FilterFir) __PYX_ERR(7, 20, __pyx_L1_error)
   __pyx_vtabptr_10joulescope_2v0_10filter_fir_FilterFir = (struct __pyx_vtabstruct_10joulescope_2v0_10filter_fir_FilterFir*)__Pyx_GetVtable(__pyx_ptype_10joulescope_2v0_10filter_fir_FilterFir->tp_dict); if (unlikely(!__pyx_vtabptr_10joulescope_2v0_10filter_fir_FilterFir)) __PYX_ERR(7, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -58740,15 +58711,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -59986,18 +59960,18 @@
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -60043,22 +60017,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -61246,15 +61220,15 @@
                         } else if (8 * sizeof(uint8_t) >= 4 * PyLong_SHIFT) {
                             return (uint8_t) (((((((((uint8_t)digits[3]) << PyLong_SHIFT) | (uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -61556,15 +61530,15 @@
                         } else if (8 * sizeof(int32_t) >= 4 * PyLong_SHIFT) {
                             return (int32_t) (((((((((int32_t)digits[3]) << PyLong_SHIFT) | (int32_t)digits[2]) << PyLong_SHIFT) | (int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -61752,15 +61726,15 @@
                         } else if (8 * sizeof(uint32_t) >= 4 * PyLong_SHIFT) {
                             return (uint32_t) (((((((((uint32_t)digits[3]) << PyLong_SHIFT) | (uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -61948,15 +61922,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -62220,15 +62194,15 @@
                         } else if (8 * sizeof(uint64_t) >= 4 * PyLong_SHIFT) {
                             return (uint64_t) (((((((((uint64_t)digits[3]) << PyLong_SHIFT) | (uint64_t)digits[2]) << PyLong_SHIFT) | (uint64_t)digits[1]) << PyLong_SHIFT) | (uint64_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -62454,15 +62428,15 @@
                         } else if (8 * sizeof(int64_t) >= 4 * PyLong_SHIFT) {
                             return (int64_t) (((((((((int64_t)digits[3]) << PyLong_SHIFT) | (int64_t)digits[2]) << PyLong_SHIFT) | (int64_t)digits[1]) << PyLong_SHIFT) | (int64_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -62650,15 +62624,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -62884,15 +62858,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -63080,15 +63054,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `joulescope-1.1.5/joulescope/v0/test/test_array_storage.py` & `joulescope-1.1.6/joulescope/v0/test/test_array_storage.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/test/test_calibration.py` & `joulescope-1.1.6/joulescope/v0/test/test_calibration.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/test/test_device.py` & `joulescope-1.1.6/joulescope/v0/test/test_device.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/test/test_filter_fir.py` & `joulescope-1.1.6/joulescope/v0/test/test_filter_fir.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/test/test_parameter.py` & `joulescope-1.1.6/joulescope/v0/test/test_parameter.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/test/test_pattern_buffer.py` & `joulescope-1.1.6/joulescope/v0/test/test_pattern_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/test/test_stats.py` & `joulescope-1.1.6/joulescope/v0/test/test_stats.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/test/test_stream_buffer.py` & `joulescope-1.1.6/joulescope/v0/test/test_stream_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/test/test_view.py` & `joulescope-1.1.6/joulescope/v0/test/test_view.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/usb/__init__.py` & `joulescope-1.1.6/joulescope/v0/usb/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/usb/api.py` & `joulescope-1.1.6/joulescope/v0/usb/api.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/usb/core.py` & `joulescope-1.1.6/joulescope/v0/usb/core.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/usb/device_thread.py` & `joulescope-1.1.6/joulescope/v0/usb/device_thread.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/usb/hw_tests.py` & `joulescope-1.1.6/joulescope/v0/usb/hw_tests.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/usb/impl_tools.py` & `joulescope-1.1.6/joulescope/v0/usb/impl_tools.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/usb/libusb/device.py` & `joulescope-1.1.6/joulescope/v0/usb/libusb/device.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/usb/scan_info.py` & `joulescope-1.1.6/joulescope/v0/usb/scan_info.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/usb/winusb/device.py` & `joulescope-1.1.6/joulescope/v0/usb/winusb/device.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/usb/winusb/kernel32.py` & `joulescope-1.1.6/joulescope/v0/usb/winusb/kernel32.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/usb/winusb/setupapi.py` & `joulescope-1.1.6/joulescope/v0/usb/winusb/setupapi.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v0/usb/winusb/win32_device_notify.py` & `joulescope-1.1.6/joulescope/v0/usb/winusb/win32_device_notify.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v1/__init__.py` & `joulescope-1.1.6/joulescope/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v1/device.py` & `joulescope-1.1.6/joulescope/v1/device.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v1/driver.py` & `joulescope-1.1.6/joulescope/v1/driver.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v1/js110.py` & `joulescope-1.1.6/joulescope/v1/js110.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v1/js220.py` & `joulescope-1.1.6/joulescope/v1/js220.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v1/sample_buffer.py` & `joulescope-1.1.6/joulescope/v1/sample_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v1/stats.c` & `joulescope-1.1.6/joulescope/v1/stats.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "C:\\bin\\Python3_11_3\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
             "C:\\bin\\Python3_11_3\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
@@ -27,16 +27,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -96,16 +96,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -2027,30 +2031,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -17945,15 +17949,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -18067,15 +18071,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -18331,15 +18335,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -18480,15 +18484,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -19082,70 +19086,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
-  __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -21511,18 +21484,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -21568,22 +21541,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -23187,15 +23160,15 @@
                         } else if (8 * sizeof(uint64_t) >= 4 * PyLong_SHIFT) {
                             return (uint64_t) (((((((((uint64_t)digits[3]) << PyLong_SHIFT) | (uint64_t)digits[2]) << PyLong_SHIFT) | (uint64_t)digits[1]) << PyLong_SHIFT) | (uint64_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -23421,15 +23394,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -23617,15 +23590,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -23889,15 +23862,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `joulescope-1.1.5/joulescope/v1/stream_buffer.py` & `joulescope-1.1.6/joulescope/v1/stream_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/v1/test/test_sample_buffer.py` & `joulescope-1.1.6/joulescope/v1/test/test_sample_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope/view.py` & `joulescope-1.1.6/joulescope/view.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/joulescope.egg-info/PKG-INFO` & `joulescope-1.1.6/joulescope.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope
-Version: 1.1.5
+Version: 1.1.6
 Summary: Joulescope™ host driver and utilities
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope-1.1.5/joulescope.egg-info/SOURCES.txt` & `joulescope-1.1.6/joulescope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/pyproject.toml` & `joulescope-1.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.5/setup.py` & `joulescope-1.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,16 +177,16 @@
     python_requires='~=3.8',
 
     # See https://packaging.python.org/en/latest/requirements.html
     # https://numpy.org/neps/nep-0029-deprecation_policy.html
     install_requires=[
         'numpy',
         'psutil',
-        'pyjls>=0.6.2',
-        'pyjoulescope_driver>=1.3.11',
+        'pyjls>=0.7.0',
+        'pyjoulescope_driver>=1.3.12',
         'python-dateutil>=2.7.3',
         'pymonocypher>=3.1.3',
         "pywin32; platform_system=='Windows'",
     ],
 
     extras_require={
         'dev': ['check-manifest', 'coverage', 'Cython', 'wheel', 'sphinx', 'myst-parser'],
```

